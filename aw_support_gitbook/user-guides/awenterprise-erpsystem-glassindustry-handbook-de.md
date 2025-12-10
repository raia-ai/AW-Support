---
title: "DE-HB-AWEnterprise_1"
source: "DE-HB-AWEnterprise_1.pdf"
tags: ["A+W Enterprise", "ERP-System", "Glass Industry", "Windows and Doors", "Software Manual", "Stammdaten", "Verkauf", "Einkauf", "Lager", "Handbuch"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is the comprehensive German-language user manual ('Handbuch') for A+W Enterprise, an ERP software solution designed for the glass, windows, and doors industry. It covers master data management, sales, purchasing, inventory, and logistics processes."
long_description: "This is the complete user manual ('Handbuch') for A+W Enterprise, a sophisticated ERP system by A+W Software GmbH, tailored for the flat glass processing industry, as well as window and door manufacturers. The manual provides a thorough overview of the software's architecture, modules, and functionalities. It begins with an introduction to the system, its modular structure, and the business processes it supports, from sales and purchasing to production and logistics. The document is divided into several major sections, each corresponding to a key module of the software: Overview (Überblick), Master Data (Stammdaten), Prices and Conditions (Preise und Konditionen), Sales (Verkauf), Purchasing (Einkauf), Inventory (Lager), and Shipping Control (Versandsteuerung). The 'Stammdaten' section is particularly detailed, explaining how to manage core data for market partners (customers, suppliers), articles, bills of materials (BOM), and system keys. Subsequent sections provide step-by-step tutorials and software reference guides for each functional area, including creating orders, managing pricing, handling purchasing processes, and controlling inventory. The manual is intended for end-users and administrators, offering both introductory tutorials and in-depth technical references. It details user interface conventions, search functions, and how to navigate the system's various dialogs and menus."
---

# A+W Enterprise Handbuch

**A+W Software for Glass, Windows & Doors**
**Deutsch**

---

---
## Editorial

### Revisionsübersicht der Dokumentation

| Datum | Änderung |
| --- | --- |
| 04-2024 | Gesamthandbuch für HTML5-Format aktualisiert. |
| 09-2021 | Gesamthandbuch erstellt |
| 08-2021 | Part Stammdaten vollständig überarbeitet. |
| 05-2020 | Part Preise und Konditionen neu. |
| 08-2020 | Part Einkauf vollständig überarbeitet. |
| 08-2019 | Part Verkauf vollständig überarbeitet. |
| 08-2019 | Part Preise neu. |
| 03-2017 | Produkt- und Firmennamen angepasst. |
| 03-2016 | Part Lager neu. |
| 03-2014 | Part Einkauf neu. |
| 08-2013 | Umsetzung auf CI 2013. |
| 11-2012 | Part Versandplanung neu. |
| 01-2010 | Ergänzung Stammdaten Preise/Konditionen. |
| 02-2007 | Änderung Zusammenführung Verkauf/Einkauf. Ergänzung Einkauf. |
| 12-2006 | Änderung im Verkauf. Ergänzung Überblick. Ergänzung Stammdaten. |
| 02-2006 | Ersterstellung. |

### Anmerkungen

Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Enterprise gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.

Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von A+W Enterprise.

### Urheberrechte

© 2024, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

### Darstellungskonventionen

Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

| Stil | Bedeutung |
| --- | --- |
| *Kursiv* | sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Preiseigenschaften*. |
| **Fett** | sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: **Geben Sie den Wert 5 ein.** |
| > | Mit dem sogenannten Brotkrumenpfad ist der Weg gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B. Stammdaten > Preise > ISO-Preise. |
| [ ] | Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit [OK] speichern Sie die Daten. |
| < > | Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit <F1> öffnen Sie die Online-Hilfe. |

### Kontakt

**A+W Software GmbH**
Siemensstr. 3
D-35463 Fernwald
Deutschland

**Tel.:** +49 641 96620 0
**E-Mail:** info@a-w.com
**Web:** http://www.a-w.com

---

## Inhalt

### A - Überblick
- **Tutorial** A-17
- **Vorwort** A-20
- **A+W Enterprise stellt sich vor** A-21
  - Produktbeschreibung A-22
  - Produktportfolio A-23
  - Leistungsmerkmale A-24
  - Systemumfeld A-31
  - Benefit von A+W Enterprise in Abgrenzung zu A+W Business A-33
- **Unterstützte Unternehmensprozesse** A-34
- **Geschäftsbereiche in A+W Enterprise - Modulen** A-36
  - Verkauf A-37
  - Produktion A-44
  - Lager A-45
  - Logistik (Versand) A-47
  - Einkauf A-47
  - Management A-48
  - Vertrieb A-49
  - Informations-System (MIS) A-49
  - Benutzerdefinierte Abfragen A-50
- **Zusammenarbeiten der A+W Enterprise Module** A-51
- **Allgemeine Grundlagen zur Arbeit mit A+W Enterprise** A-52
  - A+W Enterprise starten und beenden A-53
  - Startbildschirm A-54
  - Menüs aufrufen A-57
  - Dialog A-60
  - Suchen A-65

### B - Stammdaten
- **Tutorial** B-69
  - Einführung B-71
  - Stammdaten B-72
  - Stammdaten organisieren und pflegen B-74
  - Übungen B-82
- **Softwarereferenz** B-89
  - Stammdaten - Übersicht B-96
  - **Marktpartner** B-97
    - Marktpartner-Kopf B-97
    - Marktpartner - Kontextmenü B-99
    - Marktpartnersuche B-100
    - Register Adresse B-103
    - Marktpartner - Anmerkungstexte B-106
    - Register Identifikation B-108
    - Register Bezüge B-111
    - Register Auftrag B-113
    - Register Lieferung B-116
    - Register Rechnung B-120
    - Register Kundenspezifisch B-122
    - Register Zahlung B-124
    - Register Ausdruck B-127
    - Register Limits B-130
    - Register Bewertung B-133
    - Register Produktion B-135
    - Register Modifikation B-136
    - Register Privat B-137
    - Ansprechpartner B-138
    - Adressen B-140
    - Bankverbindungen B-145
    - E-Mailadressen B-146
    - E-Mailadressen - Detail B-148
    - Rabatte B-150
    - Rabatte Details B-151
    - Austausch-/Zusatzregeln B-152
    - Gestelltypen B-153
    - Gestelltypen - Details B-154
    - Konfigurierte MP-Felder B-155
    - Vertreterzuordnung B-156
    - Erfasserzuordnung B-157
    - Gruppenzuordnung B-158
    - Objektzuordnung B-159
    - Objekttexte B-160
    - Farbzuordnung B-161
    - Bonuszuordnung B-162
    - Artikelzuordnung B-163
    - Marktpartnertexte B-165
    - Stammtexte B-166
    - Marktpartner-Artikeltexte B-167
    - Formulare B-168
    - Dokumentenarten B-169
    - Vorgangs-Recherche B-170
    - Marktpartner-Info B-171
    - Replikationsdaten B-172
    - DFÜ-Konfiguration B-174
    - Hausspezifische Angaben B-175
  - **Mitarbeiter** B-176
    - Mitarbeiter / Berechtigungsgruppen B-177
    - Mitarbeiter - Rechte B-182
  - **Abteilungen** B-184
  - **Marktpartnerschlüssel** B-186
    - Anreden-Bezeichnungen B-188
    - Bonus B-189
    - Gruppen B-191
    - Gruppenbezeichnungen B-192
    - Branchenbezeichnungen B-193
    - Etikettentexte B-194
  - **Kalender** B-195
    - Spezielle Kalender B-197
    - Kundenkalender B-199
    - Mandantenkalender B-201
    - FIBU-Mandanten B-203
  - **Länder** B-204
    - Wirtschaftsraumbezeichnungen B-206
    - Regionen / Bundesländerbezeichnungen B-207
  - **Qualitätsskalen**
    - Allgemeine Qualitätsskala B-208
    - Termin-Qualitätsskala B-210
    - Preise-Qualitätsskala B-212
    - Mengen-Qualitätsskala B-214
    - Spezial-Qualitätsskala B-216
  - **Reklamationen**
    - Reklamationsgründe B-218
    - Reklamationsorte B-220
    - Reklamationstypen B-222
  - **Rabatte**
    - Rabattmethoden B-224
    - Rabatte B-228
    - Rabatte - Details B-230
  - **Hausspezifische Marktpartner-Angaben** B-235
  - **Systemschlüssel** B-236
    - Positionsbezeichnungen B-238
    - Postleitzahlen B-239
    - Sprachen B-241
    - Textzusatzbezeichnungen B-244
    - Dokumentenarten B-245
    - Mengeneinheitenbezeichnung B-247
    - Kantenzuordnung B-249
    - Modellbezeichnungen B-251
    - Produktionsbereich B-253
    - Verpackungsart B-254
    - Gestell-Verpackungsarten B-255
    - Versandart B-256
    - Lieferarten B-258
    - Routen B-259
    - Routenangaben II B-262
    - Tourenplan B-263
    - Versandregionen-Bezeichnung B-264
    - Fahrzeuge B-265
    - Ausgangszoll B-266
    - Bestimmungszoll B-268
    - Versandgruppen B-269
    - Gestellstatusbezeichnungen B-270
    - Gestellgruppenbezeichnungen B-271
    - Verpackungsmethodenbezeichnung B-272
    - Gestell-Verpackungszuordnung B-273
    - Währung B-274
    - Steuertypen B-277
    - Steuersätze B-279
    - Zahlungsweisebezeichnungen B-280
    - Skontogruppen B-282
    - Skontogruppenbezeichnung B-284
    - Periodenende B-285
    - Adhocsql-Gruppenbezeichnungen B-286
    - Report-Texte B-287
  - **Firmen / Gesellschaften** B-289
    - Firmenzuordnung B-290
  - **Produktschlüssel** B-292
    - Farbvarianten B-296
    - Farbbezeichnungen B-298
    - Maßvarianten B-299
    - Maßbezeichnungen B-301
    - Größenvarianten B-302
    - Größenbezeichnungen B-303
    - Austausch-/Zusatzregeln B-304
    - Austausch-/Zusatzregel - Details B-308
    - Austausch-/Zusatzregel - Testmodus B-310
    - dB-Gruppen B-312
    - U-Gruppen B-313
    - g-Gruppen B-314
    - Transmissionsgruppen B-315
    - Maßrestriktions-Gruppen B-316
    - Dickengruppen B-317
    - Biegefestigkeitsgruppen B-318
    - Vektoren für Schalldämmung (dB) B-319
    - Vektoren für thermische Eigenschaften (U) B-321
    - Vektoren für Gesamtenergiedurchlass (g) B-323
    - Vektoren für Transmission B-325
    - Vektoren für Maßrestriktionen B-327
    - Vektoren für Windlast B-329
    - Notifizierungsstellen B-330
    - Produktnormen B-331
    - Prioritäten B-333
    - Produktkennzeichnung (CEKAL) B-334
    - CE-Kennzeichen (CPIP) B-336
    - Leistungserklärung B-336
    - Produktverschlüsselung B-338
    - Bezeichnungen für Produktverwendungszwecke B-341
    - Parameterbeschreibung B-343
    - Leistungserklärung (Erfassung) B-344
    - Bezeichnungen für Analysegruppen B-345
    - Bezeichnungen für Beschlagstypen B-346
    - Bezeichnungen für Folientypen B-348
    - Produktionstypen B-349
    - Bezeichnungen für Rahmentypen B-350
    - Bezeichnungen für Versiegelungstypen B-352
    - Motivzuordnung B-353
    - Stapel B-355
    - Bezeichnungen für Kistensignatur B-355
    - Shaping/Nesting-Artikel B-357
    - Template Parameter B-358
    - ¡TOE-Austauschregeln B-359
    - Bemaßungsset B-361
    - Kundenprodukte B-362
    - Bestellte Bearbeitungen B-364
    - Hausspezifische Angaben B-366
    - VSG/GH Vererbung B-367
    - Artikelgruppen-Bezeichnungen B-368
    - Bearbeitungszuordnung B-369
    - Bearbeitungszuordnung - Details B-370
    - Bearbeitungen für Modellkanten B-372
    - Austauschgruppen-Bezeichnungen B-374
    - Gruppenzuordnung (Artikel) B-375
    - Gruppenzuordnung (Rahmen) B-376
  - **Artikel** B-377
    - Artikel-Kopf B-378
    - Artikel - Kontextmenü B-379
    - Identifikation B-381
    - Artikel - Anmerkungstexte B-386
    - Physikalische Eigenschaften B-388
    - Maßrestriktionen B-394
    - Einbaurestriktionen B-396
    - Beschaffung B-398
    - Produktion B-401
    - Preise B-405
    - Lager B-409
    - Technische Werte B-412
    - Statistik B-415
    - Modifikation B-417
    - Privat B-418
    - Lieferanten - Zuordnung B-419
    - Marktpartnerangaben B-421
    - Maßvarianten B-424
    - Maßvarianten - Details B-425
    - Farben- / Größenvarianten B-427
    - Farben- / Größenvarianten - Details B-429
    - Zwingende Maßangaben – Maßparameter-Auswahl B-431
    - Zwingende Maßangaben – Ansicht 1 B-432
    - Zwingende Maßangaben – Ansicht 2 B-434
    - Artikel-Vermaßung – Maßparameter B-437
    - Artikel-Vermaßung - Texte B-440
    - Artikel-Vermaßung - Positionsmaße B-442
    - Artikel-Vermaßung - Sonstige Parameter B-444
    - Modell-Vermaßung B-445
    - Stückliste B-447
    - Stücklisten-Restriktionen B-448
    - Preiseigenschaften B-449
    - Weitere Artikelbezeichnungen B-452
    - Artikeltexte B-454
    - Kunden-Artikeltexte B-455
    - Objekt-Artikeltexte B-456
    - Formulare B-457
    - Stammtexte - Texteditor B-458
    - Beschaffungsarten B-459
    - Artikel an A+W CAD Designer (Bars) senden B-462
    - Beschlagartikel-Abgleich B-463
    - Replikationsdaten B-464
    - Produktkennzeichnung B-466
    - Konfigurierte Felder B-472
    - Artikelbilder B-473
    - Hausspezifische Artikel-Angaben B-475
    - Hausspezifische Artikelangaben – Details B-476
    - Hausspezifische Lieferanten-Angaben B-480
    - Hausspezifische Varianten-Angaben B-481
    - Hausspezifische Farben/Größen-Angaben B-483
    - Stückliste B-485
    - Stückliste B-486
    - Formeleditor B-489
  - **Warengruppen** B-491
    - Warengruppen B-492
    - Einzelne Warengruppen B-494
    - Hausspezifische Warengruppen B-495
  - **Fertige Produkte** B-497
    - Produktfixierung B-498
    - Produktset B-499
  - **Feldkonfiguration** B-501
    - MP-Feldkonfiguration B-502
    - Artikel-Feldkonfiguration B-504
    - Vorgangs-Feldkonfiguration B-506
    - Konfiguration Bezugnahme B-508
  - **Provisionen** B-510
    - Provisionskürzel B-511
    - Provisionszuordnung B-512
  - **Textverwaltung** B-513
    - Aktuelle Texte B-514
    - Gruppentexte B-515
    - Objekttexte B-516
    - Warengruppentexte B-517
    - Konfigurierbare Texte B-518
    - Floskeln B-519
    - Variablenbezeichnung B-520
    - Textformeln B-521
  - **Kostenstamm** B-522
    - Kostenarten B-523
    - Kostenträger B-524
    - Kostenstellen B-526
  - **Preise** B-528
  - **Konditionen** B-529
  - **Listendruck** B-530

### C - Preise und Konditionen
- **Tutorial** C-533
  - Einführung C-536
  - Menü-Übersicht C-538
  - Grundgedanken der Preisermittlung C-539
  - Charakteristika von Preisen und Konditionen C-541
  - Preisberechnung im Auftrag C-542
  - Artikelstammdaten C-543
  - ISO- und PKZ-Preise C-544
  - Preisdefinitionen C-546
  - Preisschlüssel C-547
  - PLKZ-Logiken C-558
  - Komponenten der Preisberechnung C-566
  - Übungen C-579
- **Stammdaten für Preise** C-580
  - Workflow: Preise anlegen C-581
  - Preismatrizen für ISO-Scheiben C-582
  - Preisvektoren C-596
  - Austausch- und Zusatzpreise C-614
  - Sprossenpreise C-626
  - Zuschläge C-632
  - Globale Preisänderungen C-644
- **Konditionen** C-645
  - Prioritäten der Konditionsermittlung C-646
  - Komponenten der Konditionen C-650
  - Stammdaten für Konditionen C-652
  - Allgemeine und spezielle Konditionen C-653
  - Spezielle Preise C-669
  - Komplexübung C-675
- **Kostenkalkulation** C-676
  - Materialkosten C-678
  - Zusammenhang von Beschaffungsart und Kostenkalkulation C-681
- **Softwarereferenz** C-683
  - Übersicht C-689
  - Menü Preise C-690
  - Menü Konditionen C-693
  - Preisschlüssel C-695
  - Preislisten (PLKZ) C-696
  - Preiskennzeichen (PKZ) C-697
  - Matrizen C-698
  - Austausch-/Zusatzlisten C-699
  - Artikelvektoren C-700
  - Bearbeitungsvektoren C-701
  - Sprossenpreiskennzeichen C-702
  - Sprossenpreisklassen C-703
  - **Preise** C-704
    - Globale Preispflege C-705
    - Matrizen exportieren C-709
    - ISO-Preise C-710
    - ISO-Grundpreise C-711
    - Preise für ISO-Einzelscheiben C-717
    - Matrix-Editor C-722
    - Matrix-Grenzmaße C-726
    - Matrix-Flächengrenzmaße C-728
    - Matrix-Übernahme C-730
    - Matrixberechnung C-731
    - Gussglas-Klassen C-734
    d- Gussglas-Austauschpreise C-735
    - ESG/VSG/Sonder Austauschpreise C-737
    - SZR-Zuschläge C-743
    - UV-Abdeckung C-745
  - **PKZ-Preise** C-748
    - Artikelvektoren C-749
    - Spezielle Artikelvektoren C-756
    - Artikel-Vektor-Zuordnung C-758
    - Spezielle Artikel-Vektor-Zuordnung C-759
    - Bearbeitungsvektoren C-760
    - Spezielle Bearbeitungsvektoren C-765
    - Bearbeitung-Vektorzuordnung C-768
    - Bearbeitung-Matrixzuordnung C-769
    - Mindestbearbeitungspreise C-771
    - VSG-Grundpreise C-773
    - Spezielle VSG-Grundpreise C-777
    - VSG-Austausch-/Zusatzpreise C-779
    - PKZ-Preise für farbige Artikel C-784
    - Spezielle PKZ-Preise für farbige Artikel C-789
    - Variantenpreise C-791
    - Spezielle Variantenpreise C-795
    - PKZ-Verglasungspreise C-797
    - Sprossenpreise C-800
    - Sprossenpreisklassen C-800
    - Sprossenzuordnung C-806
  - **Zuschläge** C-807
    - Modellzuschläge C-808
    - Spezielle Modellzuschläge C-812
    - Zuschlagsmatrizen C-814
    - Dickenzuschlagsvektoren C-817
    - Größenzuschläge C-819
    - Bearbeitungsgruppenzuschläge C-825
  - **Preissteuerung** C-827
    - Preissteuerung C-828
    - Regelwerk VK-EK-Faktor C-830
    - Bonusregelwerk C-831
    - Preislisten-Steuerung C-832
    - Preislisten-Schranken C-833
  - **Konditionen** C-834
    - Tageskonditionen C-835
    - Allgemeine Tageskonditionen C-836
    - Warengruppenkonditionen C-843
    - Spezielle Konditionen C-849
    - Spezielle Allgemeine Konditionen C-850
    - Spezielle Warengruppenkonditionen C-859
    - Spezielle Artikelkonditionen C-868
    - Rabattstaffeln C-876
    - Warengruppenfaktoren C-878
    - Artikelfaktoren C-881
    - Sprossenfaktoren C-884
    - Modellzuschläge C-887
    - SZR-Zuschläge C-891
    - Austauschlistenfaktoren C-895
    - ISO-Einzelscheiben Artikelfaktoren C-899
    - ISO-Einzelscheiben-Konditionen
    - Warengruppenfaktoren C-902
  - **Spezielle Preise** C-905
    - Artikelpreise C-906
    - Spezielle Preise für Artikelvarianten C-914
    - Preise für farbige Artikel C-919
    - Sprossenpreise C-925
    - Bearbeitungspreise C-930
    - ISO-Austauschpreise C-937
    - Spezielle Preise für ISO-Einzelscheiben C-944
    - Spezielle ISO-Grundpreise C-949
    - UV-Abdeckungspreise C-958
    - Verglasungspreise C-962
    - Austauschpreise Gussklassen C-966
    - Spezielle VSG-Austausch-/Zusatzpreise C-970

### D - Verkauf
- **Tutorial** D-979
  - Einführung D-982
  - Allgemeine Bedienung und Tastenkürzel D-983
  - Bedienung im Auftrag D-983
  - Tastenkürzel D-984
  - Glossar D-985
  - Vorgänge suchen D-986
  - Übersicht im Menü Verkauf D-988
  - Angebote D-989
  - Aufträge D-991
  - Auftrags-Kopf- und Fußbereich D-992
  - Positionserfassung D-1006
  - ITOE - Erfassung und Nachbearbeitung D-1031
  - Produktaustausch D-1035
  - Preislose Erfassung D-1038
  - Lieferscheine D-1041
  - Rechnungen D-1042
  - Gutschriften D-1043
  - Auftragsfreischaltung D-1044
  - Druck D-1046
  - Listendruck D-1048
  - Übersicht-Funktionen im Verkauf D-1049
  - Hintergrund-Kontrollen D-1050
  - Wiedervorlagen D-1051
  - Modifikations-Funktionen im Verkauf D-1054
  - Vorgangsänderung D-1055
- **Softwarereferenz** D-1059
  - Übersicht D-1065
  - Menü Verkauf D-1066
  - Zusatzmenü D-1068
  - Infomenü D-1074
  - Suchfunktionen D-1076
  - Suche Aufträge D-1077
  - Suche Aufträge - Trefferliste D-1082
  - Marktpartnersuche D-1091
  - Mitarbeiter/Berechtigungsgruppen D-1095
  - Suche Bezugsvorgang D-1097
  - Adressen Suche D-1099
  - Artikel-Suche D-1101
  - Artikel-Suche nach Typen D-1110
  - Produktsuche nach Elementen D-1111
  - Objekt-Suche D-1118
  - Werteingabe - Erweiterte Suche D-1123
- **Vorgangsverwaltung** D-1127
  - Symbolerklärung D-1128
  - Schnellerfassung D-1131
  - Angebotserfassung D-1132
  - Preislose Erfassung D-1133
  - Auftragserfassung D-1134
  - Auftragspositionen D-1167
  - Hauswechsel D-1192
  - Neue Lieferadresse D-1192
  - Endkundenanschrift D-1195
  - Marktpartner-Info D-1197
  - Ansprechpartner D-1199
  - Storno D-1200
  - Mitarbeiterzuordnung - Spezial D-1201
  - Konfigurierbare Felder D-1201
  - Übersicht D-1202
  - Produktsets (Sash Master) D-1203
  - Artikel-Maßangaben D-1205
  - Bestandsprognose D-1206
  - Produktaustausch D-1209
  - Reklamation D-1214
  - Auftragsarten D-1215
  - Artikelangaben für bemaßte Varianten D-1217
  - Varianten- und Farben-/Dickenauswahl D-1220
  - Private Felder D-1221
  - Fremddaten-Import D-1222
  - Dokumentenarten D-1224
  - Dokumentenartenzuordnung D-1225
  - Dateizuordnung D-1228
  - DXF Import D-1229
  - Änderungs-Protokoll D-1230
  - Lieferterminänderungs-Protokoll D-1232
  - Modellkatalog D-1233
  - Modell-Maßangaben D-1234
  - Zahlungsverwaltung D-1236
  - Zahlungsplan D-1238
  - Fehlerinformationssystem D-1240
  - Produktionsmonitor D-1242
  - Technische Werte D-1243
  - Leistungserklärung D-1243
  - Auftragserfassung - Technische Werte D-1244
  - Stückliste D-1252
  - Stücklistendarstellung D-1252
  - Kantenzuordnung D-1275
  - Bearbeitungen zu Position D-1276
  - Maße der einzelnen Stücklistenteile D-1277
  - Einstand D-1279
  - Versiegelungstiefen D-1280
  - Stufenerfassung (relevante Teile) D-1281
  - Stufen Abzugsmaße D-1283
  - Sprossenerfassung D-1284
  - Sprossenstückliste - Sprossenartikel D-1288
  - Sprosseneditor D-1289
  - Bohrpunkt D-1290
  - Lichtes Feld D-1291
  - Sprossenabschnitte D-1292
  - Sprossenaufteilung D-1293
- **Packmittelplanung** D-1295
  - Vorgaben Packmittelplanung D-1295
  - Packmittelplanung D-1301
- **Anmerkungen** D-1304
  - Vorgangs-Anmerkungen D-1306
  - Marktpartner-, Objekt-, Artikel-Anmerkungen D-1307
  - Marktpartner-Artikel-Anmerkungen D-1310
- **Texte** D-1312
  - Kopf- und Fußtexte D-1313
  - Artikel- und Positionstexte D-1315
  - Spezielle Texte D-1316
  - Floskeln D-1317
  - Fremdinformationen D-1319
  - Kistensignatur D-1320
- **Preise und Konditionen** D-1322
  - Auftragskonditionen D-1323
  - Auftragspreise D-1328
  - Auftragssprossenpreise D-1330
  - Auftragsaustauschpreise D-1333
  - Auftragsunterteilpreise D-1335
  - Nachkalkulation D-1336
  - Stufenpreise D-1339
  - Positionskonditionen D-1340
  - Produktionskostenkalkulation D-1372
  - Preiskalkulation D-1379
- **Freischaltung** D-1380
  - Auftragsfreischaltung D-1380
  - Autorisierung D-1383
- **Lieferung** D-1385
  - Lieferplan D-1386
  - Lieferinformation - Details der Auslieferung D-1388
  - Lieferscheine (automatisch) D-1392
  - Lieferscheine (manuell) D-1394
  - Lieferscheinprotokoll D-1396
- **Rechnungen** D-1397
  - Rechnungen (automatisch) D-1398
  - Positionsinfo D-1401
  - Rechnungen (manuell) D-1403
  - Thekenrechnung D-1404
  - Rechnungen buchen D-1405
  - Abschlagsrechnung (automatisch) D-1408
  - Abschlagsrechnung (manuell) D-1410
  - Schlussrechnung (automatisch) D-1411
  - Schlussrechnung (manuell) D-1412
  - Rechnungsprotokoll D-1413
- **Gutschriften** D-1414
  - Gutschriften D-1414
  - Gutschriften buchen D-1416
- **Formulare** D-1419
  - Direktdruck D-1419
  - Formulardruck D-1420
  - E-Mail D-1424
  - Drucken auf D-1427
  - Listendruck D-1428
- **Auftragsstatus** D-1429
  - Auftragsinformation D-1429
  - Recherche zu Vorgängen D-1445
  - Vorgangs-Recherche D-1445
  - Positionen D-1457
- **Übersichten zu Vorgängen** D-1461
  - Auftragsanzeige D-1461
  - Angebotsanzeige D-1462
  - Wiedervorlage D-1463
  - Fertigmeldung D-1464
  - Vorgangsänderung D-1466
  - Übersicht zu Vorgängen D-1471
  - Vertrieb D-1473
- **Help Cards** D-1475
  - Informationen zu den Help Cards D-1478
  - **Angebot** D-1479
    - Schnellerfassung D-1480
    - Angebot erfassen D-1481
  - **Auftrag** D-1482
    - Kopfdaten erfassen D-1483
    - Auftrag mit Bezug erfassen D-1484
    - Auftragsart festlegen D-1485
    - Eigenschaften bearbeiten D-1486
    - Lieferanschrift bearbeiten D-1487
    - Lieferplan bearbeiten D-1488
    - Zahlungsoptionen bearbeiten D-1489
    - Auftrag freischalten D-1490
    - Auftragsinformationen anzeigen D-1491
    - Text im Auftrag bearbeiten D-1492
    - Anmerkungen bearbeiten D-1493
    - Datei anhängen D-1494
  - **Auftragsposition** D-1495
    - Position erfassen D-1496
    - Lieferant bearbeiten D-1497
    - Glas austauschen D-1498
    - Modell erfassen D-1499
    - Bearbeitung erfassen D-1500
    - Bearbeitung aus SN-Datei übernehmen D-1501
    - SN-Datei anhängen D-1502
    - Änderungen mit SN-Datei abgleichen D-1503
    - Position in CAD erfassen D-1504
    - Stufenglas erfassen D-1505
    - Sprossen erfassen D-1506
    - Sprossenaufbau bearbeiten D-1507
    - Einstand und Versiegelungstiefe D-1508
    - Randentschichtung erfassen D-1509
    - Produkt austauschen D-1510
    - Artikel fixieren D-1511
    - Leistungserklärung zuordnen D-1512
    - Technische Werte erfassen D-1513
  - **Preisberechnung** D-1514
    - Positionskonditionen ändern D-1515
    - Artikelpreise ändern D-1516
    - Fußrabatt, Zuschlag bearbeiten D-1517
    - Produktionskosten prüfen D-1518
    - Preisprotokoll für VSG D-1519
  - **Rechnung** D-1520
    - Rechnung manuell erstellen D-1521
    - Rechnungen automatisch erzeugen D-1522
    - Rechnung buchen D-1523
    - Rechnung drucken D-1524
    - Elektronische Rechnung (E-Invoicing) versenden D-1525
    - Kunden für elektronische Rechnungen konfigurieren D-1526
  - Gutschrift erfassen D-1527
- **Weitere Themen** D-1528
  - Vorgang suchen D-1529
  - Vorgangsänderung D-1530

### E - Einkauf
- **Softwarereferenz** E-1533
  - Übersicht E-1537
  - Menü Einkauf E-1537
  - Zusatzmenü E-1540
  - Infomenü E-1544
  - Zusatzmenü zum Wareneingang E-1546
  - Suchfunktionen E-1547
  - Suche Bestellungen E-1547
  - Suche Bestellungen - Trefferliste E-1552
  - Bestellpool E-1560
  - Spezielle Menüs zum Bestellpool E-1561
  - Bestellungen erzeugen E-1563
- **Vorgangsverwaltung** E-1574
  - Symbolerklärung E-1574
  - Lieferanten-Anfragen E-1577
  - Bestellerfassung E-1578
  - Bestellpositionen E-1598
  - Abholadresse E-1620
  - Bestellarten E-1622
  - Dokumentenartenzuordnung E-1623
  - Texte E-1624
  - Auftragstexte E-1624
  - Formulardruck E-1625
- **Bestellfreigabe** E-1626
  - Bestellfreigabe - Auswahl E-1626
  - Bestellfreigabe - Details E-1628
  - Bestellfreigabe – Weitere Felder E-1630
- **Wareneingang** E-1632
  - Lieferavis E-1632
  - Lieferplan E-1641
  - Wareneingang (automatisch) E-1644
  - Positionsinfo E-1646
  - Buchung Gestelle E-1647
  - Wareneingang (manuell) E-1648
  - Gestellbezogener Wareneingang E-1650
  - Wareneingangskontrolle E-1654
  - Fehlmengenkontrollpool E-1655
  - Wareneingangsprotokoll E-1656
- **Rechnungen und Gutschriften** E-1657
  - Rechnungskontrolle E-1657
  - Lieferanten-Rechnung (automatisch) E-1664
  - Übertragene Rechnungen E-1666
  - Lieferanten-Rechnung (manuell) E-1667
  - Lieferanten-Rechnung (Sammelrechnung) E-1668
  - Rechnungen buchen E-1669
  - Bestellungen abschließen E-1670
  - Rechnungsprotokoll E-1671
  - Lieferanten-Gutschrift E-1671
- **Übersichten** E-1673
  - Bestellinformation E-1673
  - Übersicht zu Vorgängen E-1674
  - Einkaufs-Recherche E-1674

### F - Lager
- **Softwarereferenz** F-1681
  - Übersicht F-1685
  - Menüs im Modul Lager F-1685
  - Suchfunktionen F-1691
  - Lager-Buchungen F-1692
  - Lagereingang F-1693
  - Lagerausgang F-1702
  - Kistenlagereingang F-1703
  - Kistenlagerausgang F-1710
  - Fachlagereingang F-1711
  - Fachlagerausgang F-1716
  - Stapellagereingang F-1717
  - Stapellageränderung F-1718
  - Gestelllagereingang F-1721
  - Gestelllagerausgang F-1723
  - Lagerausgang (Auftragsbezogen) F-1727
  - Buchungskorrektur – Übersicht F-1729
  - Buchungskorrektur – Details F-1731
- **Stammdatenverwaltung** F-1733
  - Lagerraumverwaltung F-1733
  - Artikelstammdaten Lager F-1735
- **Inventurverwaltung** F-1738
  - Inventur - Standardlager F-1738
  - Inventur - Kistenlager F-1742
  - Inventur - Fachlager F-1744
  - Inventur - Stapellager F-1745
  - Inventur - Gestelllager F-1746
- **Bewertung** F-1749
  - Bestandsbewertung - Standardlager F-1749
  - Bestandsbewertung - Kistenlager F-1752
  - Bestandsbewertung - Fachlager F-1753
  - Bestandsbewertung - Stapellager F-1754
  - Bestandsbewertung - Gestelllager F-1755
- **Informationssystem** F-1756
  - Info-Lager-Artikel F-1757
  - Info-Lager-Varianten F-1761
  - Info-Lager-Fächer F-1765
  - Info-Lager-Gestelle F-1768
  - Info-Lager-Stapel F-1771
  - Info-Lager-Blätter F-1775
  - Info-Lager-Historie F-1778
  - Aufträge/Bestellungen F-1783
  - Buchungsstatus F-1787
  - Lagerinformationen - Pickliste F-1794
  - Lagerinformationen - Trefferliste F-1795
  - LVR-Status F-1796
  - Reichweite - Bestandsprognose F-1796
  - Reichweite - Trefferliste F-1797
  - Dispositiver Bestand F-1798
  - Bestandsprognose F-1800
- **Druck** F-1802
  - Kistenetiketten drucken F-1802
  - Listendruck F-1803
- **Systemverwaltung** F-1804
  - Lagerprotokoll löschen F-1804
  - Lager-Preiskorrektur F-1805
  - Lagersicherung F-1806
- **Help Cards** F-1807
  - Informationen zu den HelpCards F-1809
  - Stammdatenverwaltung F-1810
  - Lagerraum anlegen F-1811
  - Lagerartikel festlegen F-1812
  - Lagerverwaltung F-1813
  - Lagereingang buchen F-1814
  - Lagerausgang buchen F-1815
  - Fachlagereingang buchen F-1816
  - Fachlagerausgang buchen F-1817
  - Kistenlagereingang buchen F-1818
  - Kistenlagerausgang buchen F-1819
  - Einzelblattkistenlager einbuchen F-1820
  - Einzelblattkistenlager ausbuchen F-1821
  - Gestelllagereingang buchen F-1822
  - Gestelle auftragsbezogen ausbuchen F-1823
  - Gestelllager Artikel umbuchen F-1824
  - Auftragsbezogene Ausgänge buchen F-1825
  - Stapellagereingang buchen F-1826
  - Änderung im Stapellager buchen F-1827
  - Buchungskorrektur buchen F-1828
  - Inventurverwaltung F-1829
  - Inventur im Lager durchführen F-1830
  - Bewertung F-1831
  - Bewertung im Lager vornehmen F-1832
  - Infosystem F-1833
  - Infos zu Artikeln einsehen F-1834
  - Lagerhistorie einsehen F-1835
  - Aufträge / Bestellungen einsehen F-1836
  - Buchungsstatus einsehen F-1837
  - Dispositiven Lagerbestand einsehen F-1838
  - Bestandsprognose einsehen F-1839
  - Druck F-1840
  - Kistenetiketten drucken F-1841
  - System F-1842
  - Lagerprotokoll löschen F-1843
  - Durchschnittspreis korrigieren F-1844

### G - Versandsteuerung
- **Tutorial** G-1847
  - Einführung G-1849
  - Menü-Übersicht G-1850
  - Allgemeine Bedienschritte G-1851
  - Navigieren im Versand G-1853
  - Versandmodus G-1855
  - Versand-Explorer G-1856
  - Versandsteuerung ohne Explorer G-1856
  - Versandsteuerung mit Explorer G-1858
  - Verschieben G-1861
  - Tour verschieben G-1863
  - Auftrag verschieben G-1864
  - Position verschieben G-1865
  - Versand vorbereiten G-1868
  - Fehlmengekontrolle durchführen G-1868
  - Verpackte Menge korrigieren G-1869
  - Lieferscheine G-1870
  - Ladefolge bearbeiten G-1871
  - Gestelle G-1873
  - Gestellmeldungen aus A+W Production G-1873
  - Anbindung des A+W Logistics Optimizer G-1876
  - Zusatzfunktionen G-1877
  - Touren-Übersicht G-1877
  - Auftragsinformation in der Versandsteuerung G-1879
  - Servicefunktion G-1881
  - Funktionstest (F-Test) starten G-1881
  - Funktionstest (F-Test) stoppen G-1881
- **Softwarereferenz** G-1883
  - Übersicht G-1887
  - Startfunktionen G-1888
  - Programmstart G-1889
  - Auftragssuche G-1891
  - Marktpartnersuche G-1892
  - Versand-Explorer G-1893
  - Explorer - Baumstruktur G-1894
  - Versandsteuerung – Menüs G-1900
  - Zusatzmenü G-1900
  - Infomenü G-1903
  - Schaltflächen G-1905
- **Touren** G-1906
  - Register - TourenInfo G-1907
  - Register - Gestellinfo G-1910
  - Register - FahrzeugInfo G-1912
  - Register - Optimierung G-1914
- **Auftragsebene** G-1916
  - Register - AuftragsInfo G-1917
  - Register- AuftragsInfo/Gestell G-1922
  - Register- Lieferanschrift G-1924
  - Register - VersandInfo I G-1926
  - Register - VersandInfo II G-1929
  - Register - Zusatzinfo G-1931
- **Positionsebene** G-1934
  - Register - PositionsInfo I G-1935
  - Register - PositionsInfo II G-1938
- **Funktionen im Versand** G-1940
  - Suchen G-1941
  - Springen G-1942
  - Verschieben G-1944
  - Verschieben mehrerer Pos. - Auswahl G-1946
  - Verschiebung mehrerer Pos. - Aktion G-1947
  - Auftragsinfo G-1948
  - Liefereingang buchen G-1951
  - Storno des Liefereingangs G-1952
  - Fehlmengenkontrolle - Auswahl G-1953
  - Fehlmengenkontrolle - Aktion G-1955
  - Buchen auf Transport G-1957
  - Transport zurückbuchen G-1958
  - Barcode Gestellanzeige G-1959
  - Ergebnisse der Gestellplanung G-1960
  - Packmittelplanung G-1961
  - Lieferanschrift suchen G-1962
  - Neue Lieferanschrift G-1963
  - Gestellinformationen G-1964
  - Toursperre setzen/löschen G-1965
  - Alle Touren sperren G-1966
  - Transportdaten G-1967
  - Lagerkommissionierung G-1968
- **Storno** G-1969
  - Lieferscheinstorno G-1969
  - Auftragsstorno G-1970
  - Wareneingangsstorno G-1971
  - Storno des Versandstatus G-1972
- **Gestelle** G-1973
  - Gestellzuordnung - Auswahl G-1974
  - Gestellzuordnung - Anzeige G-1975
  - Gestellauflösung - Auswahl G-1977
  - Gestellauflösung - Anzeige G-1977
  - Freie Gestelle (Übersicht) G-1979
  - Gebuchte Gestelle (Übersicht) G-1981
  - Alle Gestelle (Übersicht) G-1982
  - Einzelne Gestelle G-1984
  - Gestelle zu Auftrag G-1985
  - Scheibenzuordnung G-1987
- **VK/EK Information** G-1990
  - VK/EK Info (Global) G-1992
- **Versandsteuerung - Übersicht** G-1994
  - Lieferterminänderungen G-1997
  - Versandinformationen G-1998
  - Via Details G-1999
  - Fertigwarenlager G-2000
  - Grafische Tourenübersicht G-2006
- **Drucken** G-2007
  - Drucken einer Ladeliste G-2008
  - Drucken aller Ladelisten G-2009
  - Drucken Ergänzungsladelisten G-2010
  - Listendruck G-2011
  - Vorablieferschein Druck G-2012
  - Lief./Wareneing. Freigabe + Druck G-2014
  - Druckformat G-2015
  - Druckerauswahl G-2015
- **Help Cards** G-2017
  - Informationen zu den HelpCards G-2019
  - Versand-Explorer G-2020
  - Arbeiten ohne VS-Explorer G-2021
  - Arbeiten mit VS-Explorer G-2022
  - Tour bearbeiten G-2023
  - Tour verschieben G-2024
  - Auftrag verschieben G-2025
  - Position verschieben G-2026
  - Mehrere Positionen verschieben G-2027
  - Verschieben mit Kontext-Menü G-2028
  - Versand vorbereiten G-2029
  - Fehlmenge kontrollieren G-2030
  - Verpackte Menge korrigieren G-2031
  - Lieferanschrift ändern G-2032
  - Lieferschein erstellen G-2033
  - Ladefolge bearbeiten G-2034
  - Vorgang stornieren G-2035
- **Zusatzfunktionen** G-2036
  - Tourgrafik anzeigen G-2037
  - Auftragsinfos einsehen G-2038

### Z - Gesamtindex

---

# A. Überblick

## Revisionsübersicht des Moduls

| Datum | Änderung |
| --- | --- |
| 01-2024 | Überarbeitung des Tutorials |
| 02-2022 | Grafiken im Part Überblick aktualisiert |
| 02-2014 | Anpassung an neues CI. |
| 10-2006 | Ersterstellung. |

**Zu diesem Modul finden Sie folgendes Kapitel**
- Tutorial

---

## Tutorial: Überblick

**In diesem Kapitel finden Sie folgende Themen:**
- Vorwort
- A+W Enterprise stellt sich vor
- Unterstützte Unternehmensprozesse
- Allgemeine Grundlagen zur Arbeit mit A+W Enterprise

### Vorwort
A+W Enterprise ist ein voll integriertes, mehrmandantenfähiges ERP-System für Konzerne und gehobene Mittelstandsunternehmen der Flachglas verarbeitenden Industrie.

Das Gesamtsystem umfasst die Bereiche Verkaufsmanagement, Vertriebsunterstützung, Einkaufsmanagement, Lagerführung und Versandplanung.

A+W Enterprise gliedert sich in drei Architekturschichten: Präsentation, Anwendungslogik und Datenbank. Diese können auf unterschiedlichen Rechnern installiert und betrieben werden. Dies erhöht die Skalierbarkeit und Ausfallsicherheit des Systems. Die Anwendung stützt sich auf eine relationale Datenbank und ist als LINUX-/ UNIX-Version verfügbar. Das Benutzer- Frontend ist auf MS Windows verfügbar.

A+W Enterprise kann in der gesamte Glasbranche vom typischen Handelsbetrieb über den ISO-, ESG- oder VSG-Produzenten bis hin zum konzernartigen Unternehmensverbund und in mehrstufigen Betrieben eingesetzt werden.

Ein gutes Verständnis für die Systemarchitektur und den modularen Aufbau von A+W Enterprise erleichtert die Handhabung und Bedienung der einzelnen Bereiche und den hierfür notwendigen Wissenserwerb.

#### Themenblöcke
In diesem Tutorial finden Sie folgende Themenblöcke:
- A+W Enterprise stellt sich vor
- Unterstützte Unternehmensprozesse
- Allgemeine Grundlagen zur Arbeit mit A+W Enterprise

> **Vorausgesetzte Kenntnisse**
> EDV-Grundkenntnisse bzw. Windows-Kenntnisse werden bei der Anwendung von A+W Enterprise vorausgesetzt.

### A+W Enterprise stellt sich vor
Diese Einführung vermittelt Ihnen einen Überblick über A+W Enterprise einer ERP-Softwarelösung für die Flachglas verarbeitende Industrie.

Nachdem das Programm kurz beschrieben und auf seine Vorteile hingewiesen wird, wird im folgenden Abschnitt das Leistungsspektrum von A+W Enterprise dargestellt. Es wird skizziert, welche Unternehmen mit welchen Unternehmensstrukturen und mit welchen Tätigkeitsfeldern A+W Enterprise unterstützt.

Nach der allgemeinen Übersicht wird auf die Bedienung von A+W Enterprise mit seinen Besonderheiten eingegangen. Eine bedeutende Rolle spielt hier die Bedienung mit der Tastatur. Es stehen viele Tastaturbefehle zur Verfügung, die ein schnelles und effizientes Arbeiten ermöglichen.

Im Weiteren wird auf einige der Stammdaten eingegangen. Hier werden die Daten zu den Bereichen Marktpartner, Artikel, Stückliste, Warengruppe und Preise/Konditionen gepflegt. Alle Geschäftsbereiche (Verkauf, Einkauf, Produktion, Lager, Versand) greifen auf diese Daten zu. Sie bilden somit die Grundlage des Programmes.

Im Anschluss werden die Unternehmensprozesse die A+W Enterprise unterstützt beschrieben. Es sind viele Unternehmensprozesse in A+W Enterprise integriert und auch automatisiert. Damit entfallen die Überwachung und das Anstoßen einzelner Workflows.

Weiterführende Informationen zu A+W Enterprise finden Sie im A+W Enterprise Handbuch, in der A+W Enterprise Produktbeschreibung sowie in der Online-Hilfe.

#### Produktbeschreibung
A+W Enterprise ist ein datenbankgestütztes ERP-System (Enterprise-Resource-Planning), das sämtliche Prozesse eines flachglasveredelnden oder -produzierenden Betriebes unterstützt. A+W Enterprise kann in der gesamten Glasbranche eingesetzt werden, beginnend beim typischen Handelsbetrieb über den ISO-, ESG- oder VSG-Produzenten bis hin zum konzernartigen Unternehmensverbund.

A+W Enterprise ist eine umfassende Lösung für die Bereiche:
- Angebotswesen
- Auftragsbearbeitung
- Fakturierung
- Disposition
- Produktionsplanung und -steuerung (in Verbindung mit A+W Production)
- Bestellwesen und Einkauf
- Versandplanung und -steuerung
- Tourenoptimierung (mit A+W Logistics Optimizer)
- Lager und Kopplung mit Portalsystemen
- EDI und eCommerce
- Objektverwaltung
- Gestellverwaltung

Über die operativen Module hinaus stellt A+W Enterprise eine Vielzahl von Statistiken, Auswertungen und Informationssystemen zur Verfügung. Ebenfalls werden Schnittstellen zu externen Analysetools und Software bereitgestellt. Dadurch ist auch die Auswertung und Analyse mit Standardsoftware jederzeit möglich.

A+W Enterprise bietet eine Vielzahl von Integrationsmöglichkeiten zu Fremdsystemen. Standardisiert oder individuell können z.B. FIBU, KORE und Controlling Systeme angebunden werden. Auch eine Kopplung mit dem Gestellpool Europe ist möglich

Welche Funktionen und Funktionalitäten im Einzelnen zur Verfügung stehen, hängt von der individuellen Konfiguration des A+W Enterprise-Systems ab. Zusätzliche Module können problemlos jederzeit nachträglich integriert werden. A+W Enterprise kann als kleines, schlankes System beginnen und nach und nach zum Vollsystem ausgebaut werden.

#### Produktportfolio
In dieser Abbildung wird A+W Enterprise als ERP-System zu Beginn des Geschäftsprozesses im gesamten Unternehmensprozess dargestellt.

[Image: Abb. A-1 - A+W Software GmbH Produktportfolio - Diagramm, das den Workflow von Sales, Purchase, Production, Logistics unter dem Dach von A+W Clarity zeigt.]

#### Leistungsmerkmale
In diesem Themenblock lernen Sie den Aufbau und das Systemumfeld von A+W Enterprise kennen.
- Skalierung - modularer Aufbau
- A+W Enterprise im Glashandel
- A+W Enterprise in Betrieben mit ein- oder mehrstufiger Produktion
- Konzernartige Unternehmen

**Lernziele**
- Unterschiedliche Unternehmensziele und -strukturen aus der Glasbranche kennenlernen und wissen wie A+W Enterprise diese mit seinem modularen Aufbau unterstützt
- Das Softwarekonzept mit seiner Systemarchitektur kennenlernen

**Nutzen**
Ein gutes Verständnis für die Systemarchitektur und den modularen Aufbau von A+W Enterprise erleichtert die Handhabung und Bedienung der einzelnen Bereiche und den hierfür notwendigen Wissenserwerb.

**Definitionen**
- **Bestellkopplung:** Vollautomatische Handling von gruppeninternen Bestellungen zwischen verschiedenen A+W Enterprise Systemen (Mandanten). Änderungen werden bis zum Zeitpunkt des Sperrens automatisch über alle betroffenen Mandanten positionsgenau verbucht.

**Merke**
- **Skalierbarkeit:** A+W Enterprise besitzt durch seinen modularen Aufbau und seiner Systemarchitektur eine hohe Skalierbarkeit. Dadurch kann sich A+W Enterprise den sich ändernden Anforderungen eines Unternehmens an die Funktionalitäten des Systems anpassen und so den Anwender bestmöglich unterstützen.
- **Glashandelsbetriebe:** Sind Unternehmen, die ESG, VSG und Isolierglas zukaufen und Zuschnitt sowie kleine Bearbeitungen selber durchführen. A+W Enterprise unterstütz hauptsächlich den kaufmännischen Ablauf des Betriebes.
- **ISO-, ESG- oder VSG-Hersteller mit Glashandelshaus:** Sind Unternehmen, die neben dem Handel zusätzlich Funktionsgläser produzieren. Diese Unternehmensart nutzt die kaufmännischen Funktionen aus A+W Enterprise und die Funktionalität des Produktionsplanungs- und Steuerungssystem A+W Production.
- **Konzernartige Unternehmen:** Sind Unternehmen in einem losen oder streng organisierten Verbund.
- **Mehrstufige Produktionen:** Sind Unternehmen mit großer Produktionstiefe, die mehrere klassische Produktionsbereiche vereinseigen (ESG+VSG+ISO).
- **Systemumfeld:** Das auf Unix basierende A+W Enterprise besitzt eine grafische Benutzeroberfläche (MS Windows) und kann aufgrund der Client-Server-Architektur (3-Tier-Modell) den betrieblichen Erfordernissen schrittweise angepasst und jederzeit erweitert werden.

#### Skalierung - modularer Aufbau
Moderne Softwarepakete zeichnen sich durch eine tragfähige Systemarchitektur und fundierte fachliche Branchenkenntnisse aus.

A+W Enterprise ist durchgängig skalierbar. Das bedeutet, A+W Enterprise kann sehr genau auf die Anforderungen und die jeweilige Unternehmensgröße der Betriebe angepasst werden. Der modulare Aufbau des Systems erlaubt es, bestimmte Bausteine erst in einem späteren Projektabschnitt zu aktivieren.

So werden Glashändler, ISO-, ESG-, oder VSG-Produzenten und konzernartige Glasunternehmen in ihren jeweiligen Strukturen und Geschäftsprozessen optimal unterstützt.

Durch genaue Analyse der betrieblichen Situation und der daraus resultierenden Auswahl geeigneter Funktionen und Module kann mit A+W Enterprise eine Applikation konfektioniert werden, die sich an die unterschiedlichsten Unternehmensstrukturen flexibel anpasst - egal ob Handelsbetrieb, und ISOESG-, VSG-Hersteller oder großer integrierter Konzern.

#### A+W Enterprise im Glashandel
Unter Handelsbetrieben verstehen wir Unternehmen, in denen ESG, VSG und Isolierglas zugekauft, Zuschnitte und einfache Bearbeitungen jedoch selbst durchgeführt werden.

In diesem Unternehmen bedeutet der Einsatz von A+W Enterprise und von weiteren A+W Produkten eine starke Unterstützung für die Bereiche Einkauf, Verkauf, Vorgangsverfolgung und Fakturierung. Für die Angebotsbearbeitung stehen komfortable Funktionen zur Bildung von Alternativangeboten, übergreifendem Produktaustausch und gezielter Neukalkulation zur Verfügung. Diese beinhalten:
- Vorgangserfassung
- Eingangs- und Ausgangsschnittstellen
- Zuschnittsoptimierung
- Lagerverwaltung
- Versandsteuerung und -optimierung
- Management-Informations-System (MIS)
- Anbindung von Verkaufsniederlassungen
- Workflow-Unterstützung

**Vorgangserfassung**
Bei immer kürzer werdenden Lieferfristen zum Kunden ist es von entscheidender Bedeutung, eingehende Aufträge schnell und einfach abzuwickeln. Aus diesem Grund unterstützt A+W Enterprise Ihre Vorgangserfassung mit Produkt- und Modellabbildungen, Auswahldialogen, Vorgabewerten und diversen technischen und logischen Plausibilitätsprüfungen. Der große Variantenreichtum, aufgrund unterschiedlicher Bearbeitungen, und die vielfältigen Kombinationsmöglichkeiten im Isolierglasbereich werden über eine Stücklistenbeschreibung sehr einfach abgebildet.

**Eingangs- und Ausgangsschnittstellen**
Neben der manuellen Erfassung bietet A+W Enterprise auch verschiedene Auftragseingangsschnittstellen, um Kundenaufträge direkt aus deren EDVSystem zu übernehmen. Damit werden Erfassungszeiten und etwaige Eingabefehler reduziert, die Kundenbindung dagegen erhöht.

Aufträge können mittels der A+W Standardschnittstelle oder individuellen Kundenschnittstellen automatisch entgegen genommen werden.

Auch ein lieferantenseitiger Datentransfer kann mit A+W Enterprise erreicht werden. Unter der Voraussetzung, dass sich beim jeweiligen Lieferanten ebenfalls ein A+W Enterprise-System im Einsatz befindet, können auf bequeme Art und Weise Preisinformationen, Anfragen oder Bestellaufträge online übertragen werden. Auch eine Übertragung von Bestellungen an Fremdsysteme ist mit der A+W Standardschnittstellen oder lieferantenindividuellen Verfahren möglich (z.B. Dorma Bestellservice) möglich.

Eine weitere Möglichkeit, die Kommunikation mit Kunden und Lieferanten zu beschleunigen, besteht in der integrierten E-Mail-Anbindung, die es Ihnen erlaubt, Angebote, Aufträge oder Bestellungen in höchster Qualität direkt aus der Anwendung zu erstellen und an die Kunden/Lieferanten zu versenden.

[Image: Abb. A-2 Informationsaustausch in einem Glashandelfirmenverbund]

**Lagerverwaltung**
Je nach Größe und Komplexität des Glashandelsbetriebes kann in einer weiteren Ausbaustufe das Lagerverwaltungsmodul eingesetzt werden. Es erlaubt die Lagerführung aller Gläser im Unternehmen und kann zusätzlich für Beschläge und sonstige Zubehörartikel eingesetzt werden.

Das neue App A+W Smart Companion kann zur Verwaltung des Lagers im A+W Enterprise eingesetzt werden. Mithilfe des A+W Smart Companion Stock Moduls können z.B. Bestellungen ins Lager eingebucht werden (zusätzlich werden Bestellteile direkt ans A+W Production gemeldet), es können Lagerbewegungen vorgenommen oder Lagerausbuchungen erfolgen. Außerdem kann man direkt am mobilen Endgerät eine Inventur eines Lagers durchführen. Das Stock Modul umfasst den vollen Funktionsumfang des Inventur Moduls.

**Versandsteuerung**
Zur Versandunterstützung steht Ihnen das A+W Enterprise-Versandplanungs- und Steuerungssystem zur Verfügung. Dieses Modul verschafft dem Touren-disponenten jederzeit detaillierte Informationen über geplante Touren, Mengen, Tonnagen und die dazu benötigten Transportmittel. Der Disponent kann auf jeder Ebene des Systems ganze Touren, einzelne Aufträge oder Teilpositionen verschieben bzw. stornieren. Auch die augenblicklich verfügbaren Einheiten werden dargestellt, und über eine Fehlmengenkontrolle können Rückstands- oder Bruchpositionen auf zukünftige Touren verschoben werden. Mithilfe des A+W Logistics Optimizers können einzelne Touren oder die komplette Versandaktivität optimiert werden

**Management-Informations-System (MIS)**
Zur Steuerung der Marktaktivitäten nutzt der Glashandel die vielfältigen Möglichkeiten des Management-Informations-Systems. Neben diversen vordefinierten Statistiken steht Ihnen als Anwender auch die freie SQL-Schnittstelle zur Formulierung eigener Abfragen zur Verfügung. Damit erhalten Sie wertvolle Informationen über die augenblickliche Marktsituation, das Kundenverhalten oder über die Entwicklung des Unternehmens. Mithilfe des integrierten Reportgenerators können alle Listen in individuellem Format ausgegeben werden.

**Anbindung von Verkaufsniederlassungen**
Nehmen wir an, dass unsere Glashandlung zur Verbesserung ihrer Marktpräsenz ein Verkaufsbüro in einer nahe gelegenen Kleinstadt eröffnet. Auch dort wird zur Abwicklung des Verkaufs eine geeignete EDV-Unterstützung benötigt. Die Vernetzungsmöglichkeiten erlauben es in diesem Fall, die Arbeitsplätze in der Filiale direkt an den im Firmenstammsitz befindlichen A+W Enterprise-Server zu koppeln.

Um die Filiale als separates Profitcenter zu führen, kann auch ein eigenständiges Filialsystem aufgebaut werden, das ebenfalls mit dem Hauptsitz verbunden ist. In diesem Fall sind beide Mandanten einzeln bewertbar, jedoch über eine automatische Vorgangsübertragung miteinander gekoppelt.

#### A+W Enterprise in Betrieben mit ein- oder mehrstufiger Produktion
Ein typischer ISO-, ESG- oder VSG-Hersteller mit angeschlossenem Handelshaus nutzt im kaufmännischen Bereich sämtliche zuvor beschriebenen Funktionen wie beim Glashandel. Zusätzlich benötigt er eine detaillierte Produktions- und Kapazitätsplanung sowie eine flexible Produktionssteuerung. Als moderner Betrieb soll die Produktion per Betriebsdatenerfassung (BDE) überwacht werden.
- Freie Formen - Modelle
- Übergabe an Produktionsplanung und Fertigung (A+W Production)
- Fertigungssteuerung (A+W Production) und Betriebsdatenerfassung (BDE)
- A+W Smart Companion für BDE und Lager

[Image: Abb. A-3 Informationsaustausch im Firmenverbund mit eigener Produktion]

**Freie Formen- Modelle**
Da Betriebe einen wachsenden Anteil an Modellscheiben zu verzeichnen haben, kann zur fertigungstechnischen Beschreibung freier Formen A+W CAD Designer (Shapes) genutzt werden. Die integrierte iTOE (Integration der CAD-Software und A+W Enterprise -Vorgangsbearbeitung) erlaubt sowohl die vollgrafische Erfassung als auch die klassischen Erfassung (Eingabe von Parametern für Modelle und Bearbeitungen) in der Auftragserfassung parallel und situationsbedingt zu nutzen, Auch der Import von CAD Dateien zu einer Position ist möglich. Dabei werden CAD Konstruktion und die A+W Enterprise Stücklisten bidirektional synchronisiert.

**Übergabe an A+W Production**
Für alle fertigungsrelevanten Aufträge führt das Produktionsplanungs- und Steuerungssystem (A+W Production), ausgehend vom Kundenwunschtermin, eine Produktionsterminierung durch. Die terminliche und kapazitive Produktionsvorplanung wird dabei von Maschinenrestriktionen, Auslastung, Durchlaufzeiten, technologischen Zuordnungen, Lager, Bestellwesen, usw. beeinflusst. Aufgrund der Durchlauf- und Beschaffungszeiten werden die einzelnen Arbeitsgänge schichtgenau vorterminiert und die benötigten Maschinenkapazitäten reserviert.

Die Länge einer Schicht oder die Vereinbarung von Sonderschichten können vom Betriebsleiter jederzeit verändert werden und stehen dem Planungssystem sofort zur Verfügung. Die Überschreitung von Produktionskapazitäten führt automatisch dazu, dass ganze Fertigungsaufträge verschoben werden. Wenn Maschinenrestriktionen nicht erfüllt werden können, dann wird automatisch auf Ausweichtechnologien zugegriffen. Ein Informationssystem gibt jederzeit online Auskunft über den aktuellen Stand der verplanten Technologien und Kapazitäten.

Mit dem Produktionsabruf werden die zuvor erzeugten Produktionsläufe zur Fertigung freigegeben. Dies ist sowohl automatisch als auch interaktiv möglich. Nach der Optimierung durchgeführt ist, dann werden die Steuerdaten für die einzelnen Maschinen bereitgestellt.

Durch den Einsatz von Produktionsrückmeldung und BDE ist im A+W Enterprise der aktuelle Produktionsstatus jederzeit ersichtlich.

#### Konzernartige Unternehmen
Die zu unterstützende Struktur bei konzernartigen Unternehmen kann sehr unterschiedlich sein. Sie reicht vom losen Zusammenschluss selbstständiger Einzelbetriebe bis hin zum streng hierarchisch geführten Großunternehmen. Entsprechend unterschiedlich sind auch die Anforderungen an die eingesetzte Software. Zusätzlich zu den zuvor beschriebenen Funktionen für Glashandel und ISO-ESG-, VSG-Hersteller bietet A+W Enterprise darüber hinaus eine Reihe von Funktionalitäten für konzernartige Unternehmen.
- Zentrale Stammdatenverwaltung
- Bestellkopplung
- Leistungsverrechnung beim gruppeninternen Geschäftsverkehr
- Konzern-Berichtswesen
- Übergreifende Versandplanung (via Plant)

[Image: Abb. A-4 Konzernartiges Unternehmen.]

**Zentrale Stammdatenverwaltung**
Die Stammdaten können innerhalb einer Unternehmensgruppe mit mehreren A+W Enterprise-Mandanten zentral verwaltet und verteilt werden. A+W Enterprise stellt dafür unterschiedliche Übertragungsfunktionen zur Verfügung, die es ermöglichen, bestimmte Stammdaten ganz oder teilweise, automatisiert oder interaktiv zu verteilen. Dabei kann im Detail (bis auf Feldebene) definiert werden welche Stammdaten zentral und welche Be-standteile der Stammdaten lokal verwaltet werden.

**Bestellkopplung**
Die Vorgangsübertragung vom Handelshaus zu den angeschlossenen Produktionsbetrieben sowie die Rückmeldung von Terminverschiebungen, Produktionsfreigaben und die Information über bereits verfügbare Stückzahlen kann über A+W Enterprise vollständig automatisiert erfolgen.

**Konzern-Berichtswesen**
Zur Erhöhung der marktpolitischen Reaktionsfähigkeit steht der Unternehmensleitung eine integrierte Konzernstatistik zur Verfügung, die statistische Daten der Einzelunternehmen übergreifend zusammenfasst.

#### Systemumfeld
Um den grundlegenden Anforderungen eines leistungsfähigen IT-Systems gerecht zu werden, wurden schon in der Planungsphase folgende Themen berücksichtigt:
- Betriebssicherheit
- Systemverfügbarkeit
- unterstützte Hardwareplattformen
- Erweiterbarkeit
- Vernetzungsmöglichkeiten
- Zugangsbeschränkung und -kontrolle

A+W Enterprise besitzt eine grafische Benutzeroberfläche und kann aufgrund der Client-Server-Architektur den betrieblichen Erfordernissen schrittweise angepasst und jederzeit erweitert werden.

[Image: Abb. A-5 3-Schichten-Architektur]

Die gewählte Systemarchitektur dient der langfristigen Investitionssicherung und der Einsetzbarkeit in den unterschiedlichsten Unternehmen.

In diesem Abschnitt finden Sie Informationen zu folgenden Punkten:
- Systemarchitektur
- Datensicherheit
- Benutzeroberfläche
- Wartung und Pflege

**Systemarchitektur**
A+W Enterprise baut auf dem Betriebssystem Unix auf und kann auf AIX bzw. Linux-Servern betrieben werden.

Durch die klare Trennung von Datenbank, Datenverarbeitung und Oberfläche (3-Schichten-Architektur) lässt sich das System sehr flexibel an die betrieblichen Erfordernisse anpassen. So ist es bei wachsender Benutzerzahl problemlos möglich, mehr Rechnerleistung in die Applikationsschicht einzubringen, ohne dass Datenbanken und Oberfläche (Benutzer-PCs) verändert werden müssen.

Als Datenhaltungssystem kommt die relationale Datenbank INFORMIX zum Einsatz. Das zugrunde liegende Datenmodell ist offen gelegt und kann über eine Online-Dokumentation eingesehen werden. Sie können die Daten jederzeit mit Standardsoftware auswerten und analysieren. Beispielsweise können Sie mit Microsoft Word oder Excel direkt auf den A+W Enterprise-Datenbestand lesend zugreifen. Im Gegenzug ist es möglich, aus jedem beliebigen Dialog des A+W Enterprise-Systems die Daten unmittelbar an Microsoft Excel oder Word zu übergeben.

A+W Enterprise lässt sich vollständig in eine Netzwerklandschaft einbinden. Lokale Netze werden ebenso unterstützt wie Weitverkehrsnetze (WAN) unter Nutzung von Wählverbindungen oder Standleitungen. Schnittstellen zu E-Mail, Telefax und zu Telefonanlagen sind ebenfalls möglich.

**Datensicherheit**
Die Anwendung ist vollständig transaktionsgesichert. Dies bedeutet, dass A+W Enterprise Aktionen (z. B. Rechnungen erzeugen und Statistiken buchen) entweder vollständig oder gar nicht ausführt. Die eingesetzten Komponenten ermöglichen selbst im Falle eines Systemabsturzes, die Daten fast vollständig und in jedem Falle konsistent wieder herzustellen. Die Datensicherung erfolgt automatisch zur einstellbaren Uhrzeit oder parallel zum laufenden Betrieb.

**Benutzeroberfläche**
Die A+W Enterprise-Oberfläche wird von typischen Windows-Dialogen geprägt. Sie verfügen über Schaltflächen, Symbolleisten, Kontextmenüs, Icons und vielen weiteren Windows-Bedienelementen.

Da die Benutzeroberfläche in einer eigenen Windows-Applikation (FIX/Win) ausgeführt wird, während das eigentliche A+W Enterprise-Programm getrennt davon auf einem Applikations-Server läuft, erfordert das System nur geringe Rechenleistung am Benutzer-PC.

**Wartung und Pflege**
Zu jeder A+W Enterprise-Installation gehört ein leistungsfähiges Betreuungskonzept. Zur Betreuung gehören regelmäßige Updates, die über das Netz verschickt und außerhalb der normalen Betriebszeit installiert werden. Die Wartung erfolgt grundsätzlich über eine Netzwerkkopplung, so dass ein gleichzeitiger Datentransfer stattfinden kann. So ist ein sehr effektiver Support möglich.

### Benefit von A+W Enterprise in Abgrenzung zu A+W Business
Im Hause der A+W Software GmbH gibt es zwei kaufmännische Softwarelösungen: A+W Enterprise und A+W Business. Beide Systeme sind auf die Flachglasindustrie ausgerichtet und erfüllen deren Anforderungen im kaufmännisch-administrativen Bereich in sehr guter Weise. Abhängig von der Unternehmensgröße und -struktur empfiehlt sich jedoch in einem Fall mehr die A+W Business- im anderen Fall die A+W Enterprise-Lösung.

Größere Unternehmen mit einer ausgeprägten Niederlassungsstruktur profitieren in der Regel eher von der Architektur des A+W Enterprise Systems. Für Einzelbetriebe oder Unternehmensgruppen, die wie Einzelbetriebe agieren, empfiehlt sich hingegen oft die A+W Business Lösung.

Unternehmen die eine integrierte und ggf. automatisierte Prozessverarbeitung wünschen, sind mit A+W Enterprise besser bedient, während sich für Betriebe die einen vom Benutzer getriebenen Workflow präferieren das A+W Business System besser eignet.

Die A+W Enterprise Multisite Funktionalität ermöglicht es mehrere Niederlassungen in einem System abzubilden und eine Reihe niederlassungsübergreifende Funktionalitäten zu nutzen (Versandplanung, Lager, übergreifenden Auswertungen, gemeinsame Stammdaten, ...). Ein ausgeklügeltes Berechtigungssystem regelt dabei, wer auf welche Daten zugreifen darf (übergreifend oder lokal, lesend oder schreibend). Der EDV-Verwaltungsaufwand wir so ebenfalls drastisch reduziert.

### Unterstützte Unternehmensprozesse
In diesem Themenblock lernen Sie die Geschäftsprozesse und das Zusammenspiel der einzelnen Module bei den Prozessen kennen

**Lernziele**
- Die Geschäftsprozesse und das Zusammenspiel der einzelnen Module bei den Prozessen kennenzulernen.

**Nutzen**
A+W Enterprise unterstützt durch seine modulare Struktur alle kommerziellen Geschäftsbereiche eines Unternehmens und bietet integrierte Schnittstellen zur Produktion. Die fundierte Kenntnis der A+W Enterprise Module ist daher die Grundlage für ein effizientes, prozessorientiertes Arbeiten im System.

**Definitionen**
- **Grafische Produkterfassung:** Unterstützt in der Auftragserfassung mit einem Sprosseneditor, einer Modellerfassung, einem Stücklistenbaum und mit A+W CAD Designer (Shapes).
- **A+W Production:** Ein Produktionsplanungs- und Steuerungssystem für eine ein- oder mehrstufigen Produktion.
- **Fertigmeldung/BDE:** Eine permanente Statusmeldung und -kontrolle.
- **Bestellpool:** Im Bestellpool werden alle Bestellvorschläge gesammelt.

**Merke**
- **Verkaufsmodul:** Im Verkaufsmodul werden kaufmännische Vorgänge unter Berücksichtigung der gepflegten Stammdaten (Austauschzusatzregeln, Plausibilitäts-und Restriktionsprüfung) erfasst und an das System zur Weiterverarbeitung übergeben. Dies bedeutet z.B. eine terminliche Disponierung von Bearbeitungen, Reservierung von Teilen im Lager oder auch Zukaufsteile an den Bestellpool melden.
- **Kostenkalkulation:** Die Kostenkalkulation berücksichtigt konfigurationsabhängig Material-, Personal-, und Maschinenkosten.
- **Produktionsmodul:** Das Produktionsmodul A+W Production umfasst die Bedarfsmeldung, Produktionsplanung, Fertigungssteuerung und die Fertigmeldung (BDE). Alle produktionsrelevanten Daten (Bedarf, Termin etc.) werden aus dem Auftrag und den Stammdaten automatisch ermittelt.
- **Produktionsplanung:** Die Produktionsplanung ermittelt aus den kaufmännischen Informationen alle produktionsrelevanten Daten und unterwirft diese einer logischen Restriktionsprüfung.
- **Fertigungssteuerung:** Bei der Fertigungssteuerung werden zuvor erstellte Produktionslose an das Optimierungsprogramme A+W Sequence Optimizer übergeben, und aus dem Ergebnis wird die Maschinenansteuerung erstellt.
- **Lagermodul:** Das Lagermodul übernimmt die interne Bestandsführung und Inventur. Bedarf wird im Lager bei Unterschreitung von Mindestbeständen automatisch gemeldet.
- **Versandsteuerung:** Die Versandsteuerung übernimmt die Tourenplanung und -organisation, die Gestellverwaltung, die Lieferüberwachung, die Fehlmengenkontrolle und die Erzeugung von Lieferscheinen.
- **Einkaufsmodul:** Das Einkaufsmodul bietet die Möglichkeit Artikel zu bestellen und den Eingang bestellter Artikel im System zu verbuchen.
- **Informationssystem:** Neben dem MIS bietet Ihnen A+W Enterprise die Möglichkeit benutzerdefinierte Abfragen erstellen zu können. Für die SQL-Abfragen steht Ihnen das Datenmodell von A+W Enterprise zur Verfügung.

#### Geschäftsbereiche in A+W Enterprise - Modulen
Die im Schaubild dargestellten Unternehmensprozesse und Geschäftsbereiche bündeln sich in A+W Enterprise in den einzelnen Modulen. A+W Enterprise gewährleistet das nahtlose Zusammenspiel zwischen den einzelnen Modulen und zu anderen Programmen mit Hilfe einer Reihe von Funktionen wie Schnittstellen, einer übergreifenden Workflow-Unterstützung, einer Archivierung und Druck.

[Image: Abb. A-6 Schematische Übersicht der A+W Enterprise Funktionalität]

Die einzelnen Unternehmensprozesse in A+W Enterprise vorzustellen, sprengt den Rahmen einer Einführung, dennoch soll ein Eindruck der einzelnen Module und dessen Zusammenspiel vermittelt werden. Aus diesem Grund empfiehlt es sich bei der Präsentation die einzelnen Module und ihr Zusammenspiel anhand der Hauptüberschriften und Hauptdialoge in A+W Enterprise vorzustellen. Programmbereiche und einzelne Dialoge werden gezeigt und erläutert. Der Trainer hat darauf zu achten, dass sinnvolle Daten in den Dialogen vorhanden sind.

#### Verkauf
Im Verkauf werden Angebote ausgearbeitet, Aufträge erfasst und die Preiskalkulation durchgeführt. Die Mitarbeiter erstellen hier Lieferscheine, Rechnungen und Gutschriften. Folgende Bereiche werden hier bearbeitet:
- Angebots- und Auftragserfassung
- Grafische Module in der Vorgangserfassung
- Preislose Erfassung
- Kostenkalkulation
- Freigaben
- Rechnungen
- Gutschriften

**Angebots- und Auftragserfassung**
[Image: Abb. A-7 Auftragserfassung]

Bei der Vorgangserfassung stehen komfortable Funktionen zur Bildung von Alternativangeboten, übergreifendem Produktaustausch und gezielter Neukalkulation zur Verfügung.

Die Erfassung und Verwaltung der einzelnen Positionen im Vorgang wird durch viele Komponenten erleichtert, wie z. B. Auswahlhilfen, Modellabbildungen, visualisierte Artikelsuche, Positionsstatus usw. Es werden nur die Daten abgefragt, die zur vollständigen Beschreibung des Produktes notwendig sind.

Die Variationsmöglichkeiten von Produkten aufgrund unterschiedlicher Bearbeitungen, Farben, Formen, Größen und Kombinationen werden in den Stammdaten zu Stücklisten zusammengefügt. Über eine Stücklistenbeschreibung können Produkte abgebildet und im Vorgang auf Wunsch verändert werden.

Austauschregeln, Plausibilitäts- und Restriktionsprüfungen kontrollieren die "Machbarkeit" des Produktes.

Mit der Auftragserfassung werden die eingehenden Bestellungen aufgenommen und anschließend zur weiteren Bearbeitung dem System übergeben. Unter Berücksichtigung des vom Kunden gewünschten Liefertermins werden die erforderlichen Bearbeitungen terminlich disponiert. Die am Lager befindlichen Teile werden für den Vorgang reserviert, während die Zukaufteile dem Bestellpool übergeben werden.

**Grafische Unterstützung zur Erfassung von Produkten in der Vorgangserfassung**
A+W Enterprise bietet verschiedene grafische Module, um die Erfassung von Standardformen und Modellen visuell zu unterstützen. Folgende Module sind enthalten oder können in A+W Enterprise eingebunden werden.

**A+W Enterprise Modellerfassung**
A+W Enterprise bietet eine Möglichkeit zum Erfassen von Modellen an. Standardmäßig geschieht dies über einen umfangreichen Modellkatalog. Zusätzlich können Sie freie Formen selbst definieren oder beispielsweise aus dem Programm A+W CAD Designer (Shapes) importieren.

[Image: Abb. A-8 Modellerfassung]

**Grafischer Sprosseneditor**
Der Sprosseneditor ermöglicht die Feinbearbeitung der Sprossen. Hier können Sie mit einem Mausklick waagerechte und senkrechte Sprossenteile entfernen oder auf eine andere Bohrpunktposition verschieben.

[Image: Abb. A-9 Sprossenerfassung in der Auftragserfassung]

**Grafischer Stücklistenbaum**
Der grafische Stücklistenbaum erlaubt die Navigation durch die Stückliste mit der Maus. Stücklistenebenen können einfach geöffnet und eingesehen werden. Sie erhalten somit eine genauere Vorstellung des gesamten Produktaufbaus. Zur besseren Übersicht wurden bestimmten Artikeltypen grafische Symbole (Icons) zugeordnet. Dies ermöglicht eine einfache Unterscheidung zwischen Gläsern, Rahmen, Sprossen oder Bearbeitungen. Bei Gläsern stellt A+W Enterprise neben der Bezeichnung die Einbauposition und - falls vorhanden - die Struktur bzw. die Beschichtung dar.

[Image: Abb. A-10 Stücklisten-Darstellung in der Auftragserfassung]

**A+W CAD Designer (Shapes) - ITOE**
In der Vorgangserfassung steht eine Visualisierung des Produktes mit allen Bearbeitungen zur Verfügung. Diese Visualisierung dient dem Anwender als grafische Kontrollmöglichkeit zur Prüfung der bearbeiteten Scheiben. Nach der Vermaßung des Produktes und der eingefügten Bearbeitung wird automatisch eine A+W CAD Designer (Shapes)-Skizze generiert und Online im Positionsdialog präsentiert.

[Image: Abb. A-11 Grafische Anzeige der Bearbeitungen mit A+W CAD Designer (Shapes)]

**Kostenkalkulation**
[Image: Abb. A-12 Kostenkalkulation für ein Floatglas]

Sie können in A+W Enterprise folgende Kostenarten heranziehen, um die Gesamtkosten für ein Produkt zu ermitteln: Materialkosten Lagermaterial, Materialkosten Zukaufteile, Maschinenkosten und Personalkosten.

A+W Enterprise ermittelt die Materialkosten während der Angebots-/Auftragserfassung. Die Maschinen- und Personalkosten ermittelt das Produktionsplanungs- und Steuerungssystem A+W Production im Rahmen der Produktionsplanung. Bei der Einrichtung der Kostenkalkulation können Sie entscheiden, ob A+W Enterprise nur Materialkosten oder Material-, Maschinen- und Personalkosten zur Kostenkalkulation heranziehen soll.

**Materialkosten Lagermaterial**
A+W Enterprise berechnet die Materialkosten für Lagermaterialien auf der Grundlage einer Materialkostenliste. Diese Liste enthält den durchschnittlichen EK-Preis zuzüglich der Lagerkosten, Materialgemeinkosten etc. Zusätzlich kann beim Artikel ein durchschnittlicher Verlust hinterlegt werden, den A+W Enterprise automatisch bei der Kalkulation einbezieht.

**Materialkosten Zukaufteile**
Die Materialkosten für Zukaufteile (auch zugekaufte Unterteile einer Stückliste) ermittelt A+W Enterprise direkt aus den beim Lieferanten hinterlegten Preisen und Konditionen. Beim Einsatz des Moduls Einkauf aktualisieren sich mit jeder Preisänderung im Einkauf die Kosten für die entsprechende Verkaufsposition.

**Maschinenkosten**
Die Maschinenkosten berechnen sich aus der Laufzeit des Betriebsmittels und den Kostensätzen, die dem Betriebsmittel zugeordnet sind. Die Laufzeit ermittelt dabei das PPS-System A+W Production.

**Personalkosten**
Die Personalkosten ergeben sich aus der im PPS-System A+W Production ermittelten Zeit und den Kosten der Arbeitsplatzbesetzung (Team oder Einzelperson).

**Freigaben**
Mit einer Freigabe verlässt der Auftrag die Erfassungsebene. Alle notwendigen Bearbeitungs- und Bestellvorkehrungen des Vorganges werden dem Bestellpool oder dem Produktions-Management-System übergeben. Darüber hinaus wird der Auftrag im Rahmen der Freischaltung auch dem Versandsteuerungssystem gemeldet.

**Rechnungen**
Die Rechnungsstellung richtet sich nach den im Vorgang hinterlegten Lieferungs- und Zahlungsbedingungen. Es können Teil- oder Sammelrechnungen vereinbart werden, die in der Regel nach Lieferung der Ware zur Auslösung kommen. Eine fakturierte Rechnung ist prinzipiell nicht mehr korrigierbar.

Sollen preisliche Änderungen vorgenommen werden, so ist dies nur noch über die Ausstellung einer Gutschrift oder Nachbelastung möglich. Neben der Komplett-, Teil- oder Sammelrechnung dient die Thekenrechnung der gleichzeitigen Erfassung von Vorgang, Lieferschein und Rechnung, was bei Selbstabholern sinnvoll genutzt werden kann. Unter bestimmten Voraussetzungen kann auch eine Glasverrechnung zwischen Produktion und Handel abgerufen werden.

**Gutschriften**
Vorgangsstornierungen, Transportschäden oder Reklamationen können zu einer kompletten oder teilweisen Gutschrift des Vorgangs führen. Möglich ist auch eine Gutschrift über eine Pauschalsumme, unter Bezugnahme der betreffenden Rechnung.

#### Produktion
Das Produktionsplanungs- und Steuerungssystem A+W Production übernimmt die komplette Steuerung und Abwicklung einer ein- oder mehrstufigen Produktion.
- Bedarfsmeldung
- Produktionsplanung (Ablauf- und Materialoptimierung)
- Fertigungssteuerung
- Fertigmeldung/Betriebsdatenerfassung

**Bedarfsmeldung**
Das Produktionsplanungs- und Steuerungssystem ermittelt aufgrund kaufmännischer Informationen aus Auftrag und Stammdaten den Bedarf und die Produktionstermine. Daraus werden produktionsrelevante Daten zusammengestellt. Das Ergebnis dieser Planung wird in den Vorgang zurückgeschrieben, kann im Produktions-Management-System manipuliert oder übernommen und nach individuellen Kriterien in übergreifende Produktionslose umgesetzt werden.

Um eine Übersicht über vergangene, gegenwärtige und zukünftige Produktionsmengen zu bekommen, bietet das Produktions-Management-System Auswertungen nach verschiedenen Gesichtspunkten.

**Produktionsplanung**
Die Produktionsplanung setzt in Verbindung mit A+W Production die kaufmännischen Informationen in produktionstechnische Daten um. Die Planung berücksichtigt dabei produktionsrelevante Stammdaten, Termine, Kapazitäten und technische sowie logische Restriktionen. Die Arbeitspläne können virtuell manipuliert (umgelastet, editiert) oder übernommen werden. Änderungen eines Termins oder Betriebsmittels, das Splitten einer Vorgangsposition usw. sind möglich. In der Produktionsplanung können Betriebsmittel bei Bedarf tageweise gesperrt (langfristig angekündigte Reparaturarbeiten) oder die Kapazitätsgrenzen im Einzelfall geändert werden (kurzfristiger Maschinen- oder Personalausfall). Die vorgangsbezogenen und gespeicherten Planungsdaten sind Grundlage für die folgende Fertigungssteuerung.

**Fertigungssteuerung**
Die erstellten Produktionslose werden über Schnittstellen an Optimierungsprogramme übergeben, die dann aus den Daten Maschinenansteuerungen erzeugen.

**Fertigmeldung/Betriebsdatenerfassung**
Durch bereitgestellte Daten aus einer Betriebsdatenerfassung (BDE), kann der Status der Produktion global oder pro Vorgang verfolgt werden.

#### Lager
Die Lagerverwaltung übernimmt Führung, Pflege und Kontrolle von Lagerbeständen. Dieser Vorgang beginnt bei der Vorgangsfreigabe und den damit verbundenen Lagerdispositionen und reicht hin bis zur Inventurbearbeitung.

A+W Enterprise unterstützt die folgenden Lagertypen:
- Standardlager für alle Artikel, Varianten usw.
- Kistenlager für komplette Kisten mit Gläsern
- Fachlager, um Artikel den Fächern zuzuordnen

A+W Enterprise führt die Lager im Allgemeinen in zählbaren Mengen (Stück). Es findet eine automatische Umrechnung in die entsprechenden Grundmengeneinheiten (qm, lfm) statt.

Die Lagerverwaltung selbst stellt Module für den manuellen Eingang, den manuellen Ausgang und die Inventur zur Verfügung. Zusätzlich ist ein Lagerinformationssystem vorhanden, welches die Materialbewegungen detailliert darstellt.

Das Lager ist eng gekoppelt mit den Modulen Verkauf und Einkauf. Diese Module erzeugen im Rahmen von Buchungen automatisch Lagerzu- und Lagerabgänge.

Über die verkauften und bestellten Mengen errechnet A+W Enterprise zeitnah dispositive Bestände. So ist es jederzeit möglich, die Bestandsentwicklung vorauszusehen. Mithilfe von Mindest- und Alarmbestand erzeugt das Lager auf der Basis physikalischer und dispositiver Bestände automatisch Bestellvorschläge im Einkauf.
- Bedarfsmeldung
- Bestandsführung
- Inventur
- Bewertung

**Bedarfsmeldung**
Wenn die Artikel eine bestimmte Anzahl unterschreiten, so sollte dieser Artikel nachbestellt werden, um die Produktion nicht zu behindern. In A+W Enterprise können Sie zwei Schwellenwerte angeben, den Alarmbestand und den Mindestbestand. Diese sind individuell für jeden Artikel konfigurierbar. Wenn der Alarmbestand unterschritten wird, dann löst A+W Enterprise eine Meldung aus, dass der betreffende Artikel nachbestellt werden muss. Der Mindestbestand ist eine Kenngröße, die nicht unterschritten werden sollte, und zwar weder real noch im Rahmen einer Prognose aufgrund der Kapazitätsplanung. Auch in diesem Fall meldet A+W Enterprise die Unterschreitung.

**Bestandsführung**
Lagerbestände werden durch die permanente Inventur gepflegt. Dazu werden alle Lagerein- und Lagerausgänge in A+W Enterprise verbucht. Der jeweilige aktuelle Lagerbestand kann so über das A+W Enterprise-System jederzeit erfragt werden.

**Inventur**
Als gesetzlich vorgeschriebene Jahresinventur wird die permanente Inventur empfohlen. Die permanente Inventur ermöglicht es, den am Abschlussstichtag vorhandenen Bestand des Vorratsvermögens nach Art, Menge und Wert auch ohne gleichzeitige körperliche Bestandsaufnahme festzustellen. In jedem Geschäftsjahr muss mindestens einmal durch körperliche Bestandsaufnahme geprüft werden, ob der jeweilige Buch- bzw. Soll-Bestand im A+W Enterprise-Lagersystem mit dem tatsächlich vorhandenen Bestand (Ist-Bestand) übereinstimmt. Die Bestandsaufnahme kann so z. B. zu einem Zeitpunkt erfolgen, an dem der Bestand am niedrigsten ist.

**Bewertung**
Ein eingetretener Wertverlust muss im Allgemeinen bei der Inventur nach dem Niederstwertprinzip behandelt werden. Das Niederstwertprinzip besagt, dass alle Gegenstände des Umlaufvermögens höchstens mit ihrem Anschaffungsbzw. Herstellungskosten anzusetzen sind. Ist jedoch der Tageswert am Bilanzstichtag niedriger als die Anschaffungs- bzw. Herstellungskosten, so muss der niedrigere Tageswert in die Schlussbilanz eingesetzt werden.

#### Logistik (Versand)
Die Planung der Touren eines Tages wird mithilfe der Versandsteuerung organisiert.
- Tourenplanung und -organisation
- Lieferüberwachung
- Fehlmengenkontrolle
- Lieferschein

**Tourenplanung und -organisation**
A+W Enterprise bietet mit der Versandsteuerung die Möglichkeit, tagesweise Tourenpläne einzusehen und zu bearbeiten. Touren, komplette Aufträge oder nur einzelne Auftragspositionen können über die Steuerungskomponente der Versandsteuerung auf einen anderen Tag verschoben werden. Mit dem Vorablieferschein und der Ladeliste bzw. der Ergänzungsladeliste stehen frühzeitig Versandinformationen zur Verfügung.

**Lieferüberwachung**
Die Lieferplanverwaltung ermöglicht es, Großaufträge zu erfassen und auszuwerten, für die bereits mit der Vorgangserfassung ein genauer Plan über einzelne Teilabrufe (Teillieferungen) vorliegt. Nach der Vorgangsfreigabe sind Änderungen des Lieferplans immer noch möglich.

**Fehlmengenkontrolle**
Mithilfe der Fehlmengenkontrolle können Sie prüfen, ob alle Stückzahlen einer Position bzw. eines Vorgangs verpackt sind und für den Versand bereitstehen. Gegebenenfalls können Sie die Mengen ändern, wenn z. B. Barcodes fehlerhaft eingelesen wurden. Sie können einen Lieferschein erst dann erstellen, wenn die gesamte Stückzahl eines Vorgangs als Verpackt gemeldet ist.

**Lieferschein**
Für jede Auslieferung eines Vorganges wird ein Lieferschein ausgestellt. Dieser dient zum einen als Nachweis, zum anderen als Auskunft über den jeweiligen Status der Vorgangsabwicklung. Lieferscheine können als Komplettlieferschein oder als Teillieferscheine ausgestellt werden. Letzteres kommt dann in Betracht, wenn die Auslieferung nicht komplett, sondern in mehreren Teilen notwendig oder gewünscht wird.

#### Einkauf
Der Bereich Einkauf bietet die Möglichkeit, Artikel zu bestellen sowie den Eingang bestellter Artikel im System zu verbuchen.
- Bestellpool
- Anfrage und Bestellung
- Avisierung und Wareneingang
- Rechnungsprüfung

**Bestellpool**
Artikel, die in A+W Enterprise als Zukaufteile angelegt sind, laufen als Bestellvorschläge in den Bestellpool. Wenn durch Entnahme von Artikeln im Lager der aktuelle Bestand eine bestimmte Schwelle unterschreitet, dann generiert das Lagermodul ebenfalls Bestellvorschläge, die in den Bestellpool eingehen. Das gleiche gilt für die Reservierung von Artikeln durch die Fertigungsplanung, wenn der prognostizierte Bestand eine bestimmte Schwelle unterschreitet. Zusätzlich können Sie Bestellungen manuell eingeben.

**Anfrage und Bestellung**
Der Einkaufsmitarbeiter analysiert die Bestellvorschläge, gruppiert sie nach Artikeltypen und Reservierungsdatum. Er fragt bei Lieferanten an, prüft Lieferantenalternativen und bestellt Artikel.

**Avisierung und Wareneingang**
Geplante und eingegangene Lieferungen werden vom Mitarbeiter im Einkauf in das System verbucht. Die Lieferbestätigung eines Lieferanten können Sie dabei als Avisierung erfassen. So können Sie zum einen den Bestandsverlauf eines Artikels für die Bestellplanung fortschreiben, zum anderen können Sie einen termingerechten Wareneingang überprüfen.

**Rechnungsprüfung**
Nachdem der Wareneingang erfasst wurde folgt die Prüfung der Eingangsrechnungen. Dabei können sowohl Einzelvorgänge als auch Teil- oder Sammelvorgänge verwaltet werden. Die Prüfung der Wareneingänge und Rechnungen findet zunächst auf der Ebene des Gesamtauftrages statt. Erst bei einer Abweichung erfolgt eine erneute Prüfung auf der Ebene der Einzelpositionen, und zwar solange, bis der Vorgang vom Benutzer abgeschlossen wird. Mit Abschluss der Rechnungsprüfung werden die entsprechenden Daten an die Lieferanten- bzw. Einkaufsstatistik geschickt. Außerdem können Daten für die Finanzbuchhaltung und Kostenrechnung bereitgestellt werden.

#### Management
Voraussetzung für ein systematisches Controlling als Grundlage für Managemententscheidungen sind die Erfassung und die kontinuierliche Kontrolle von Unternehmensdaten. A+W Enterprise bietet folgende Ansätze, um notwendige Informationen zur Unternehmenssteuerung zu beschaffen und zu präsentieren:
- Informations-System (MIS)
- Benutzerdefinierte Abfragen

#### Vertrieb
**Budgets**
Dem Vertrieb steht ein Budgetierungstool zur Verfügung. Hier können fürs gesamte Unternehmen wie für einzelne Objekte auch Etats definiert und verwaltet werden. So können Sie beispielsweise Verteilungsmatrizen, Verteilungsvektoren, Budgetierung und Soll-Ist-Vergleiche für das Unternehmen erstellen. Die Objektbudgetierung umfasst eine Vielzahl von Anwendungsmöglichkeiten, von der Verwaltung von Objektkonten und Objektlisten, Montagekosten bis hin zur Lohnabrechnung.

**Provisionen**
A+W Enterprise berücksichtigt Provisionen bereits bei der Vorgangserfassung. Es berechnet die Provisionen anhand von Schlüsseln, die abhängig von Kunden, Warengruppen oder vom Deckungsbeitrag (Spanne) sein können. Wenn eine Rechnung oder eine Gutschrift freigegeben wurde, bucht A+W Enterprise die entsprechenden vorgangsbezogenen Provisionen.

#### Informations-System (MIS)
Für Auswertungen und Statistiken steht der gesamte Datenbestand des A+W Enterprise-Systems zur Verfügung. Zusätzlich sind bestimmte Verdichtungsebenen des Datenbestandes abrufbar. Im Verkaufsbereich sind dies beispielsweise die klassischen Statistikdaten Vertreter, Kunde, Warengruppe, Branche, Umsatzmengen und -beträge; im Einkaufsbereich analog dazu Daten über Lieferanten, Artikel, gelieferte Mengen, Preise, und vieles mehr. Auf diese Daten kann jederzeit anwenderfreundlich zugegriffen werden. Der Anwender hat die Möglichkeit, gezielt in Ergebnissen von Abfragen zu arbeiten oder beliebige Anfragen an die Datenbank zu formulieren. Die erzeugten Ergebnisdaten werden in tabellarischer Form präsentiert und können auf vielfältige Weise aufbereitet und ausgedruckt werden. Für den Bereich Lager sind Informationen über durchschnittliche Bestände, Durchsatz sowie Reichweiten verfügbar. In den Bereichen Produktion und BDE finden Sie Informationen über Maschinen, gefertigte Mengen, Ausfallzeiten, Durchlaufzeiten und Personal.

Ein zusätzliches Hilfsmittel ist die Vorgangs-Recherche. Damit können Angebote, Aufträge, Lieferscheine und Rechnungen nach einer ganzen Reihe von Kriterien durchsucht und identifiziert werden. Die Informationsmöglichkeiten schließen Kopfdaten (Kunde, Datum, Liefertermin), Kommissionsdaten, Bestelltexte und positionsgenaue Daten (Abmessungen, Mengen, Deckungsbeiträgen usw.) ein. Auch stehen bereits vorbereitete Abfragen zu teilgefertigten, teilgelieferten und teilberechneten Vorgängen im System zur Verfügung.

#### Benutzerdefinierte Abfragen
Neben den vordefinierten Abfragemöglichkeiten über das A+W Enterprise-Informationssystem bietet A+W Enterprise im Systemmenü die Funktion SQL-Abfragen an. Mithilfe dieser Funktion können Sie bereits angelegte Abfragen anpassen und eigene Abfragen neu zusammenstellen und ausführen. Um das Zusammenstellen der Abfragen zu erleichtern, finden Sie in der Softwarereferenz des jeweiligen Parts neben den Feldbeschreibungen auch die entsprechenden Datenbankfelder. Zusätzlich können Sie über das Systemmenü die Tabellendokumentation einsehen.

#### Zusammenarbeiten der A+W Enterprise - Module
Diese Abbildung zeigt den gesamten modularen Aufbau von A+W Enterprise in einem Ein- und Mehrmandatensystem. Alle sind grafisch hervorgehoben und in die einzelnen Bereiche eingeordnet.

[Image: Abb. A-13 Modulplan]

### Allgemeine Grundlagen zur Arbeit mit A+W Enterprise
In diesem Themenblock lernen Sie, die erste Schritte mit A+W Enterprise zu gehen und Grundbegriffe, über die Sie dabei verfügen müssen.

**Lernziele**
- Aufbau des Programms verstehen
- Aufbau der Dialoge mit seinen Icons kennenlernen
- Arbeitsweise im Dialog beherrschen
- Arbeitsprozesse zwischen Dialogen beherrschen
- Tastaturbefehle erlernen
- Die Bedienung von A+W Enterprise mit seinen Besonderheiten erlernen

**Nutzen**
Die Bedienung in A+W Enterprise ist geprägt durch spezielle Arbeitsweisen in Dialogen und dialogübergreifenden Prozessen. Das erlernen dieser Prinzipien ist die grundlegende Voraussetzung schnell und effizient mit A+W Enterprise zu arbeiten.

**Definitionen**
- **FIX/Win:** Grafische Oberfläche, in die A+W Enterprise eingebettet ist
- **SELO:** Numerische Suchfunktionalität <F9>
- **Matchcode:** Alphanumerische Suchfunktionalität <F8>
- **Dialog:** Bezeichnung der Eingabeoberfläche in A+W Enterprise

**Merke**
- **Tastenkombinationen:** Im A+W Enterprise stehen viele Tastenkombinationen für die Bedienung der Anwendung zur Verfügung.

#### A+W Enterprise starten und beenden
In Anschluss wird erklärt wie das Programm A+W Enterprise gestartet und beendet wird.

**So starten Sie A+W Enterprise:**
1. Um A+W Enterprise zu starten, öffnen Sie den A+W Ordner auf Ihrem Desktop. Wählen Sie A+W Enterprise in der gewünschten Konfiguration und starten Sie mit einem Doppelklick den Anmeldedialog.
2. Wählen Sie in der Programm-Liste das Modul, welches Sie starten wollen. Geben Sie anschließend Ihren Benutzernamen und Ihr Passwort (wird vom Administrator vergeben) in die entsprechenden Felder ein.
3. Betätigen Sie die Schaltfläche [Verbinden]. A+W Enterprise startet das gewählte Modul. A+W Enterprise öffnet das gewählte Modul in einem Programmfenster.

[Image: Abb. A-14 A+W Enterprise-Anmeldedialog]

**So beenden Sie A+W Enterprise:**
1. Um A+W Enterprise korrekt zu beenden, schließen Sie den Dialog mit der Taste <Ende> oder <Pos1> und betätigen Sie <Ende>, bis A+W Enterprise eine Sicherheitsabfrage anzeigt, ob Sie das Programm beenden möchten.
2. Betätigen Sie die Schaltfläche [JA]. A+W Enterprise schließt die Anwendung auf Ihrem Rechner und meldet Sie auf der Datenbank ab.

#### Startbildschirm
Wenn Sie im Anmeldedialog A+W Enterprise ausgewählt haben, dann zeigt das Programmfenster den A+W Enterprise-Startbildschirm an.

[Image: Abb. A-15 Programmfenster und Startbildschirm]
- **A:** FIX/WIN-Menüleiste
- **B:** Symbolleiste
- **C:** A+W Enterprise-Menüleiste
- **D:** A+W Enterprise-Menü mit Untermenüs
- **E:** Statuszeile

**FIX/Win-Menüleiste (A)**
Mithilfe der Menüleiste können Sie grundlegende Einstellungen vornehmen. Es stehen folgende Menüs zur Verfügung:
- **Enterprise:** Mit den Einträgen dieses Menüs können Sie das Programmfenster schließen. Außerdem können Sie die aktuelle Anzeige der A+W Enterprise-Oberfläche drucken und die Druckeinstellungen anpassen.
- **Anzeige:** Mit diesem Menü steuern Sie die Anzeige des Meldungsdialogs, die Anzeige der Symbolleiste und die Anzeige einer zusätzlichen Statuszeile. Des Weiteren können Sie Kopierregeln einstellen.
- **Einstellungen:** Mithilfe der Einträge dieses Menüs steuern Sie die Größe und das Aussehen der Dialoge. Außerdem können Sie die Kopierfunktionen detailliert einstellen.
- **Hilfe:** Über diesen Menüpunkt erhalten Sie Info über A+W Enterprise. Anwenderhilfe über das Produkt können Sie aus jedem Dialog mit <F1> aufrufen.

**Symbolleiste (B)**
In der Symbolleiste stellt das Programmfenster die wichtigsten Funktionen der A+W Enterprise-Software über Symbol-Schaltflächen bereit. Die Auswahl der angezeigten Schaltflächen ändert sich in Abhängigkeit des geöffneten Dialoges. In der Start-Ansicht befinden sich folgende Symbole:

| Schaltfläche | Funktion | Schaltfläche | Funktion |
| :---: | :--- | :---: | :--- |
| X | Ende | K | Erster Satz |
| ? | Nachschlaghilfe | < | Letzter Satz |
| ⬆️ | Maskenvariante | ⬇️ | Eine Seite nach unten |
| ↕️ | Sortiermenü | ⬆️ | Eine Seite nach oben |
| ➕ | Zusatzmenü | 🔽 | Runter |
| i | Infomenü | 🔼 | Hoch |
| 📋 | Satz einfügen | 📧 | E-Mail empfang |
| ➕📋 | Satz hinzufügen | ? | Hilfe anzeigen |
| X📋 | Satz löschen | | |

**Menü und Untermenüs (C, D)**
A+W Enterprise ist menüorientiert. Jede Funktion und viele Dialoge können über ein Menü aufgerufen werden. Die Menüs des Startbildschirms sind nach Modulen bzw. Aufgabenbereichen gegliedert. Folgende Menüs stehen zur Verfügung:
- **Verkauf:** Der Bereich Verkauf gehört aufbauorganisatorisch zu den kaufmännischen Abteilungen. In diesem Bereich können Sie Angebote ausarbeiten, Preiskalkulationen durchführen und Aufträge erfassen oder komplettieren. Darüber hinaus ist die Erstellung von Lieferscheinen und Rechnungen sowie das Ausstellen von Gutschriften diesem Menüpunkt zugeordnet.
- **Einkauf:** Der Bereich Einkauf bietet die Möglichkeit, Artikel zu bestellen sowie den Eingang bestellter Artikel im System zu erfassen.
- **Produktion:** In diesem Menü finden Sie Funktion zur auftragsorientierten XOPT-Übergabe, die eine vorangehende Konfiguration benötigt. Die Übergabe an die A+W Production erfolgt über die A+W - Dienste und Programme-Installation im Absprache mit A+W Mitarbeiter und gemäß der Vereinbarungen.
- **Logistik:** Dieses Menü umfasst Funktionen zum Thema Versandsteuerung, Lieferplanung, Gestell- und Lagerverwaltung.
- **Analyse:** Das Menü Analyse umfasst verschiedene Funktionen zum Abruf und Anzeigen von Verkaufs- und Einkaufsstatistiken, zum Drucken von Listen verschiedenster Statistiken und Funktionen zum Erstellen eigener Abfragen.
- **Stammdaten:** Stammdaten sind zeitunabhängige Daten, die selten verändert werden. Sie sind der Dreh- und Angelpunkt des gesamten Systems, da Bezüge zu allen anderen Bereichen bestehen. Dieses Menü bietet den Zugriff auf die Dialoge, um Stammdaten anzulegen und zu pflegen.
- **System:** Über das Systemmenü haben Sie Zugriff auf verschiedene Systemeinstellungen, Abfrage- und Auswertungsmöglichkeiten.
- **User:** Bei diesem Menüpunkt handelt es sich um Favoriten, die Sie über das Systemmenü User-Menüpunkt definieren hinterlegen können. Sie besitzen hiermit einen Schnellzugriff auf die von Ihnen über das Systemmenü definierten Menüpunkte.

**Statuszeile (E)**
In der Statuszeile sind die Benutzerinformationen des angemeldeten Mitarbeiters ersichtlich.

#### Menüs aufrufen
A+W Enterprise bietet Ihnen dialog- und feldabhängig die Möglichkeit, zusätzliche Informationen zum gewählten Feld aufzurufen, einzugeben, Daten nach eigenen Kriterien zu sortieren und zusätzliche benutzerspezifische Einstellungen vorzunehmen.

**Zusatzmenü aufrufen**
[Image: Abb. A-16 Zusatzmenü in der Auftragserfassung auf Kopfebene]

Mit `<F4>` können Sie von nahezu allen Feldern das verkürzte oder das erweiterte Zusatzmenü aufrufen. Sie haben dort die Möglichkeit, ergänzende Menüpunkte zum Vorgang auszuwählen. Sie verlassen das Zusatzmenü mit `<Ende>`.

**Infomenü aufrufen**
[Image: Abb. A-17 Infomenü in der Auftragserfassung auf Positionsebene]

Das Infomenü beinhaltet Informationen zum aktuellen Vorgang, wie beispielsweise Anmerkungen oder den Status. Mit `<Shift> + <F4>` rufen Sie das Infomenü auf. Sie verlassen das Infomenü mit `<Ende>`.

**Systemmenü aufrufen**
[Image: Abb. A-18 Systemmenü]

Im Systemmenü können Sie benutzerspezifische und systemrelevante Konfigurationen vornehmen. Mit `<Strg> + <F4>` rufen Sie das Systemmenü auf. Sie verlassen das Systemmenü mit `<Ende>`.

**Sortiermenü aufrufen**
[Image: Abb. A-19 Sortiermenü]

Das Sortiermenü ist aus nahezu alle Tabellendialogen heraus aufrufbar. Es bietet neben verschiedenen Sortierweisen auch die Möglichkeit, in den Sätzen nach Mustern zu suchen, Sätze zu kumulieren, zu löschen oder Druckformate zu bedienen. Mit `<Strg> + <F5>` rufen Sie das Sortiermenü auf. Sie verlassen das Sortiermenü mit `<Ende>`.

**Kontextmenü aufrufen**
[Image: Abb. A-20 Kontextmenü auf dem Feld Menge in der Auftragserfassung auf Positionsebene]

Mit der rechten Maustaste auf einem Feld öffnen Sie das Kontextmenü. Im Kontextmenü werden alle Funktionen angezeigt, die in diesem Feld zur Verfügung stehen.

#### Dialog
Vom Startbildschirm aus rufen Sie die einzelnen Dialoge auf. Bei Bedarf können Sie weitere Module direkt aufrufen, die in einem eigenen Programmfenster gestartet werden.

[Image: Abb. A-21 Programmfenster mit Dialog]
- **A:** Dialog
- **B:** Infozeile
- **C:** Prompt
- **D:** Statuszeile

**Dialog (A)**
Über die einzelnen Menüpunkte oder direkt aus Dialogen heraus können Sie weitere Dialoge öffnen. In den Dialogen werden Ihre Daten erfasst.

**Infozeile (B)**
Die Infozeile wird oberhalb des Prompts eingeblendet, um zusätzliche Informationen und Statusmeldungen anzuzeigen.

**Prompt (C)**
Am unteren Rand des A+W Enterprise-Bildschirms wird eine zusätzliche Zeile mit weiteren Bedienmöglichkeiten und zusätzlichen Menüs eingeblendet. Diese Zeile nennt man Prompt. Die zur Auswahl stehenden Bedienmöglichkeiten und zusätzlichen Menüs sind von der aktuellen Position des Cursors im Dialog abhängig. Diese können entweder per Mausklick auf die Schaltfläche, die im Prompt angezeigt wird, oder mit der Tastenkombination, die auf der Schaltfläche genannt wird, per Tastatur aufgerufen oder ausgeführt werden. Weiter können diese Funktionalitäten aus dem Prompt über das Kontextmenü aufgerufen werden.

**Statuszeile (D)**
In der Statuszeile sind die Benutzerinformationen des angemeldeten Mitarbeiters ersichtlich.

#### Arbeiten in Dialogen
Dieser Abschnitt beschreibt, wie Sie innerhalb eines Dialogs Eingaben tätigen können, zwischen Ansichten wechseln, Suchen durchführen und zusätzliche Informationen abrufen können.

**Vorbelegte Felder**
Wenn Sie Dialoge öffnen oder Auswahlen in bestimmten Feldern treffen, werden einige Felder in den Dialogen bereits mit Daten aus den Stammdaten vorbelegt.

**<Enter> Eingaben bestätigen, Felder überspringen**
A+W Enterprise füllt die Felder mit den Daten aus, die in den Stammdaten hinterlegt sind. Mit `<Enter>` bestätigen Sie die Auswahl oder überspringen Felder, wenn Sie keine Änderung des Feldinhalts vornehmen möchten.
Wenn Sie Felder überspringen möchten, für die ein Eintrag zwingend erforderlich ist, weist A+W Enterprise in der Infozeile auf die fehlende Eingabe hin. Der Cursor bleibt so lange in diesem Feld, bis ein Eintrag vorgenommen wurde.

**<Leertaste> (Toggle) Zwischen vordefinierten Feldinhalten wechseln**
In einigen Feldern ist es möglich, durch Betätigen der `<Leertaste>` aus hinterlegten Feldinhalten einen auszuwählen (Toggle-Felder). Die Auswahl kann alternativ per Maus erfolgen, nachdem die Taste `<F9>` gedrückt oder der Pfeil neben dem Feld angeklickt wurde.

**<F12> Zurück**
Mit `<F12>` wechseln Sie von einem Feld in das vorherige. Sie können `<F12>` mehrmals hintereinander betätigen, um mehrere Felder zurückzugehen. Das Springen zum vorherigen bzw. zum nächsten Feld ist auch mit den `<Pfeiltasten>` möglich. Die Feldreihenfolge ist fest vom Programm vorgegeben.

**<Pos1> und <Ende> Dialogbereiche wechseln**
Innerhalb von Dialogen mit mehreren Bereichen können Sie sich mit `<Pos1>` Sprung in den übergeordneten Bereich des Dialoges und `<Ende>` Sprung in den untergeordneten Bereich des Dialoges bewegen (Beispielsweise von den Kopfdaten zu den Rumpfdaten und wieder zurück).

#### Ansicht oder Register im Dialog wechseln
Im Anschluss erläutern wir Ihnen wie Sie eine Ansicht oder ein Register im Dialog wechseln.

**<F2> zwischen verschiedenen Ansichten oder Registern wechseln**
In Dialogen zur Eingabe von Datensätzen wie beispielsweise in der Auftragserfassung können in den Kopfdaten, Rumpfdaten und Fußdaten jeweils verschiedene Register bzw. Ansichten zur Verfügung stehen. Mit `<F2>` können Sie in das nächste Register wechseln. Einige Dialoge besitzen weitere Ansichten. Mit `<F2>` können Sie die Ansicht wechseln.

**<Pos1> und <Ende> Dialog verlassen, zurück zur Hauptansicht**
Sie verlassen mit `<Pos1>` oder `<Ende>` einen Dialog bzw. kehren in die Hauptansicht zurück, wenn Sie zuvor mit `<F2>` eine andere Ansicht gewählt haben.

#### Die wichtigsten Tastenfunktionen und Symbol-schaltflächen
Nachfolgend finden Sie eine Übersicht über die wichtigsten Funktionen, die betreffenden Tastenkombinationen und die entsprechenden Symbol-Schaltflächen, die in A+W Enterprise benötigt werden.

| Taste | Tastenkombination | Schaltfläche | Funktion |
| --- | --- | :---: | --- |
| `<F1>` | `<F1>` | ? | Hilfe aufrufen |
| | `<Schift> + <F1>` | | Feld-Hilfe anzeigen lassen |
| | `<Strg> + <F1>` | | Anwendereigene Feld-Hilfe aufrufen |
| `<F2>` | `<F2>` | 🗂️ | Ansicht/Register wechseln |
| `<F3>` | `<F3>` | | Aktion auslösen |
| | `<Schift> + <F3>` | | Drucken |
| | `<Strg> + <F3>` | | Alten Feldinhalt zurückholen |
| `<F4>` | `<F4>` | 📄 | Zusatzmenü aufrufen |
| | `<Schift> + <F4>` | i | Infomenü aufrufen |
| | `<Strg> + <F4>` | | Systemmenü aufrufen |
| `<F5>` | `<F5>` | | Detail anzeigen |
| | `<Strg> + <F5>` | 📊 | Sortiermenü aufrufen |
| `<F6>` | `<F6>` | | Neuen Satz anhängen |
| | `<Schift> + <F6>` | | Neuen Satz einfügen |
| | `<Strg> + <F6>` | | Neue Zeile einfügen |
| `<F7>` | `<F7>` | X | Satz löschen |
| | `<Schift> + <F7>` | | Feldinhalt löschen |
| | `<Strg> + <F7>` | | Zeile löschen |
| `<F8>` | `<F8>` | | Matchcodesuche starten |
| `<F9>` | `<F9>` | | Suche SELO starten |
| `<F12>` | `<F12>` | F | Zurück ins vorherige Feld |
| `<Strg>` | `<Strg> + <C>` | | Feldinhalt kopieren |
| | `<Strg> + <V>` | | Kopierter Feldinhalt einfügen |
| `<Leertaste>` | `<Leertaste>` (<Toggle>) | | Zwischen vordefinierten Feldinhalten wechseln |
| `<Pos1>` | `<Pos1>` | | Verwerfen, oder innerhalb der Dialoge in den übergeordneten Bereich des Dialoges wechseln. Zurück zur Hauptansicht, wenn Sie mit `<F2>` eine andere Ansicht gewählt haben. |
| `<Ende>` | `<Ende>` | X | Speichern und verlassen oder innerhalb der Dialoge in den untergeordneten Bereich des Dialoges wechseln. Zurück zur Hauptansicht, wenn Sie mit `<F2>` eine andere Ansicht gewählt haben. |

> **Tastaturhilfe**
> Zur Unterstützung bei der Arbeit mit A+W Enterprise können Sie eine Tastaturhilfe (Schablone) nutzen. Diese Hilfe ist eine Kurzerläuterung der Funktionstasten. Bei Interesse wenden Sie sich bitte an den zuständigen A+W Enterprise Mitarbeiter.

#### Suchen
Je nach Art des gewählten Feldes bietet A+W Enterprise verschiedene Arten von Suchfunktionen und Nachschlagehilfen.

**<F8> (Matchcode)**
[Image: Abb. A-22 Dialog einer Matchcode-Suche]

Sie können in vielen Feldern die Suche nach einem alphanumerischen Wert (max. 8 Stellen) durchführen (Matchcode/Wiederholung der Artikelbezeichnung). Der Matchcode ist ein frei definiertes Stichwort in den Artikel- oder Marktpartnerstammdaten, beispielsweise ein Firmenname. Der Matchcode kann aus Buchstaben und Zahlen bestehen. Die Eingabe eines Startwertes schränkt die Suche ein. Wird kein Wert eingegeben, werden alle Ergebnisse, alphanumerisch sortiert, aufgelistet.

> **Erweiterte SELO**
> In der aktuellen Version ist standardmäßig eine erweiterte Selo-Logik aktiv. Ein Suchdialog beinhaltet gleich mehrere Felder, nach deren Werte-Eingabe die Treffermenge entsprechend reduziert werden kann. Wird die Suche mit `<F8>` gestartet, so ist der Werte-Eingabefeld Matchcode beim Start mit `<F9>` das nummerische Feld, z. B.: Auftragsnummer.
> Eine ausführliche Beschreibung finden Sie in den einzelnen Kapiteln, z. B.:
> - Verkauf, "Suche Aufträge" auf Seite D-1077
> - Verkauf, "Marktpartnersuche" auf Seite D-1091
> - Verkauf, "Artikel-Suche" auf Seite D-1101

**<F9> (<SELO>)**
[Image: Abb. A-23 Dialog einer Selo-Suche]

A+W Enterprise öffnet eine Nachschlagehilfe, mit der Sie die Suche nach einem numerischen Wert (max. 8 Stellen) durchführen können. Die Eingabe eines Startwertes schränkt die Suche ein. Erfolgt keine Eingabe oder bei Eingabe des Wertes 0 werden alle Ergebnisse aufgelistet.

**Erweiterte Suche**
[Image: Abb. A-24 Dialog einer erweiterten Suche]

In der neuen erweiterten Suchfunktion sind die `<F8>`, `<F9>` und auch `<F2>` stehen an vielen Stellen vereint als eine erweiterte Suche zur Verfügung.

---
# B. Stammdaten

## Revisionsübersicht des Moduls

| Datum | Änderung |
| --- | --- |
| 02-2023 | Erweitert um neue Dialoge im Bereich Schlüssel |
| 03-2022 | Feldbeschreibung in den Bereichen Marktpartner, Artikel, Anmerkungen und Rabatte aktualisiert |
| 11-2020 | Vollständige Überarbeitung |
| 08-2013 | Umsetzung auf CI 2013. |
| 01-2010 | Neu: Kapitel Preise und Konditionen. |
| 10-2006 | Ersterstellung. |

**Zu diesem Modul finden Sie folgende Kapitel:**
- Softwarereferenz
- Tutorial

---
## Tutorial: Stammdaten

**In diesem Kapitel finden Sie folgende Themen:**
- Einführung
- Stammdaten
- Stammdaten organisieren und pflegen
  - Marktpartner
  - Artikel
  - Stückliste
    - Stücklisten im Handelshaus
    - Stücklisten im Produktionsbetrieb
  - Maßberechnung
  - Warengruppe
  - Preise und Konditionen
  - Arbeiten mit Shared Memory
- Übungen

### Einführung
A+W Enterprise ist ein voll integriertes, mehrmandantenfähiges ERP-System für Konzerne und gehobene Mittelstandsunternehmen der Flachglas verarbeitenden Industrie.

Das Gesamtsystem umfasst die Bereiche Verkaufsmanagement, Vertriebsunterstützung, Einkaufsmanagement, Lagerführung und Versandplanung. Als Basis aller Module gelten die Stammdaten.

Ein gutes Verständnis für die Systemarchitektur und den modularen Aufbau von A+W Enterprise erleichtert die Handhabung und Bedienung der einzelnen Bereiche und den hierfür notwendigen Wissenserwerb.

Das Tutorial zum Modul Stammdaten beschäftigt sich mit den Basisdaten des gesamten A+W Enterprise.

Bitte beachten Sie, dass die unterschiedliche Dialoge im Zusammenhang mit bestimmten Funktionen stehen, und so müssen separat freigeschaltet haben. Wenn Sie dazu Fragen haben, wenden Sie sich bitte an die A+W Software GmbH.

**Themenblöcke**
In diesem Tutorial finden Sie folgende Themenblöcke:
- "Stammdaten organisieren und pflegen" auf Seite B-74
- "Übungen" auf Seite B-82

> **Zielgruppe und vorausgesetzte Kenntnisse**
> Dieses Tutorial richtet sich an Teilnehmer, die im A+W Enterprise Stammdaten einrichten und pflegen. EDV-Grundkenntnisse bzw. Windows-Kenntnisse werden bei der Stammdaten-Pflege von A+W Enterprise vorausgesetzt.

### Stammdaten
Die Stammdaten bilden sich den Kern aller Module und Funktionen und haben Auswirkungen auf allen Nutzungsebenen.
Der Bereich Stammdaten kann in mehrere Untergruppen aufteilen:
- Schlüsseln
- Marktpartner
- Artikeln
- Preise und Konditionen
- Sonstiges

**Lernziele**
- die einzelnen Bereiche der Stammdaten (Marktpartner, Artikel, Stückliste, Warengruppen, Preise und Konditionen) und dessen Struktur und Eigenschaften kennenlernen
- Funktion der Shared Memory wissen

**Nutzen**
Alle A+W Enterprise-Module (Geschäftsbereiche) greifen auf die in den Stammdaten hinterlegten Daten zu. Gut angelegte und gepflegte Stammdaten ermöglicht es Ihnen Arbeitsprozesse mit A+W Enterprise schneller und vereinfacht durchzuführen.

**Definitionen**
- **Marktpartner:** sind Kunden, (Bau-) Objekte, Lieferanten, (Gestell-) Eigentümer und Sonstige.
- **Artikel:** Beschreibt ein Produkt mit seinen Eigenschaften und Merkmalen.
- **Stückliste:** Artikelaufbau mit Bearbeitungen und Restriktionen.
- **Warengruppe:** Alphanumerischer Wert. Hierunter werden mehrere Artikel gebündelt.
- **Shared Memory:** Ein extra Zwischenspeicher für große Datenmengen im Bereich des Artikelstamms.

**Merke**
- **Basis des Systems:** Die Organisation und Pflege der Stammdaten ist die Basis des Systems und seiner Module. Alle Geschäftsbereiche greifen auf die gleichen Daten zu.
- **Stückliste:** Die Stückliste beschreibt den Aufbau eines Artikels mit seinen Bearbeitungen und bildet die Grundlage für das in A+W Enterprise integrierte Warenwirtschafts- und Produktionsmanagement-System. In einer Stückliste können mehrere Artikel eingebunden sein.
- **Warengruppe:** Jedem Artikel muss eine eindeutige Warengruppe zugeordnet werden. Die Warengruppe bestimmt die Preiskonditionen des Artikels und ist die Basis für statistische Auswertungen.
- **Preise und Konditionen:** Basis der Stammdaten für Preise und Kondition sind regionale, nationale und ausländische Preislisten. Konditionen haben eine höhere Priorität als Preise.

### Stammdaten organisieren und pflegen
Die Organisation und Pflege der Stammdaten ist die Basis des Systems und seiner Module. Die im Artikelstamm hinterlegten Daten haben Auswirkung auf viele Bereiche des Systems. Dies umfasst Vorgangserfassung, Produktion, Lager, Einkauf, Versand, Statistik und die Datenreplikation. Alle Geschäftsbereiche greifen auf die gleichen Basis-Stammdaten zu. Darüber hinaus verfügen die einzelnen Bereiche über bereichsspezifische Stammdaten. In den Stammdaten sind sämtliche Daten hinterlegt, vom Artikel über Preislisten bis hin zu Zuschlägen.

Der Themenblock beinhaltet folgende Schulungseinheiten:
- Marktpartner
- Artikel
- Stückliste
- Warengruppe
- Preise und Konditionen
- Arbeiten mit Shared Memory

Musterstammdaten, also ein vollständiger Artikel-, Stücklisten- und Warengruppenstamm, können im Rahmen der Installation zur Verfügung gestellt werden.

#### Marktpartner
[Image: Abb. B-1 Dialog Marktpartner]

Die Marktpartnerstruktur umfasst Kunden, Objekte, Lieferanten, Eigentümer und Sonstige. Zu den verschiedenen Marktpartnern können alle relevanten Informationen erfasst werden, wie Adressen, Ansprechpartner, Bankverbindungen, Limits, Gruppenzugehörigkeiten, Klassifizierungen und vieles mehr. Objekte sind in der Regel größere Bauvorhaben oder Projekte. Zur Unterstützung des Objektgeschäfts stehen drei Funktionsbereiche zur Verfügung:
- ein konzernübergreifendes Objektinformationssystem für den Informationsaustausch über Objekte
- ein Objektüberwachungssystem für die mengen- und wertmäßige Überwachung und Budgetierung von Objekten
- ein Objektkonditionssystem zur gesonderten Preisberechnung für die dem Objekt zugeordneten Angebote und Aufträge

#### Artikel
[Image: Abb. B-2 Dialog - Artikelstamm]

Der Artikelstamm dient der zentralen Beschreibung aller Produkte. Jeder Artikel wird dabei durch eine Vielzahl von Merkmalen und Eigenschaften beschrieben, die das Produkt kennzeichnen. Dazu gehören unter anderem die Produktbezeichnung, Artikeltyp, Warengruppe, vorhandene Varianten, Beschaffungsarten sowie technische Restriktionen und gesetzlich vorgeschriebene Kennzeichnung der Produkte. Ebenso können mehrsprachige Artikelbezeichnungen hinterlegt werden. Stücklisten beschreiben die Struktur eines Produktes, das aus verschiedenen Komponenten zusammengesetzt sein kann. In A+W Enterprise können Artikel einfach in eine Stückliste eingebunden werden.

#### Stückliste
**Stammdaten > Stückliste**

[Image: Abb. B-3 Angabe des Ursprungsartikels für die Anzeige des Stücklistendialoges]

Im Dialog Stückliste können Sie die Struktur der einzelnen Produkte einsehen. Zum Einstieg geben Sie die Nummer des gesuchten Produktes ein oder wählen es mit Selo aus.
- Mit `<F3>` springen Sie jeweils eine Ebene tiefer.
- Mit `<Ende>` kehren Sie zur vorherigen Ebene zurück.
In diesen Dialogen können Sie nur Änderungen in der ersten Ebene vornehmen.

[Image: Abb. B-4 Anzeige der 1. Auflösungsebene des Artikels 410710]
[Image: Abb. B-5 Alle Auflösungsebenen des Artikels 410710]

[Image: Abb. B-6 Aufruf der Stückliste aus dem Artikelstamm]

A+W Enterprise beinhaltet als integriertes Warenwirtschafts- und Produktions-Management-System ein leistungsfähiges Stücklistenkonzept. In den Stücklistenstammdaten wird der Original-Artikelaufbau für jeden einzelnen Artikel bzw. die Baugruppe mit den Bearbeitungen festgelegt. Durch Austausch-/Zusatzregeln ist es möglich, bestimmte Artikel oder Bearbeitungen der Stückliste eines Produktes gegen andere auszutauschen. Stücklisten können entweder artikelübergreifend geändert werden oder auch kundenindividuell. So können beispielsweise während der Vorgangserfassung Stücklisten für den Kunden individuell angepasst und gespeichert werden. Die Original-Stückliste bleibt jedoch in den Stammdaten erhalten. Ob bei der Vorgangserfassung der Stücklistenbaum geändert werden darf oder nicht, kann vorher im Artikelstamm festgelegt werden. Die Stückliste bildet die Grundlage für die Materialwirtschaft. Anhand dieser wird der benötige Bedarf an Material ermittelt. Aufgaben und Zielsetzung von Stücklisten können sich bei reinen Handelsbetrieben und Produktionsbetrieben unter Umständen stark unterscheiden.

**Stücklisten im Handelshaus**
Für den Handelsbetrieb bietet das Stücklistenkonzept im Wesentlichen zwei Vorteile:
- **Preisfindung:** Da jede Stücklistenkomponente (Teil, Baugruppe oder Bearbeitung) in die Preisberechnung einfließen kann, wird es möglich, den Gesamtpreis eines Produktes aus der Summe seiner Komponenten zu ermitteln.
- **Vertextung:** Auch die textuelle Darstellung eines Produktes kann über die Stückliste automatisiert erfolgen, da jede Stücklistenkomponente in die Vertextung einfließen kann. Jedes Teil der Stückliste trägt dazu ein Druckkennzeichen, das vom A+W Enterprise-Textgenerator ausgewertet wird.

**Stücklisten im Produktionsbetrieb**
Ein zu fertigendes Produkt setzt sich aus unterschiedlichen Teilen und Baugruppen zusammen, die im Rahmen der Materialwirtschaft verwaltet werden müssen. Dazu enthält die Stückliste alle Verbrauchsmaterialien und Baugruppen mit den entsprechenden Mengenangaben. Um lagermäßige Mindeststückzahlen zu garantieren oder die Beschaffung von Lagerartikeln zu gewährleisten, muss der erwartete Verbrauch von Materialien frühzeitig erkennbar sein. Für diese Mengenplanung bilden die Stücklisten eine Grundvoraussetzung. Da alle fertigungsrelevanten Bearbeitungsschritte in der Stückliste enthalten sind, bildet sie die Grundlage für die Einlastung der Arbeitsgänge auf den zugehörigen Maschinen. Die daraus resultierenden Zeitvorgaben führen nach dem Just-in-time-Prinzip zur Findung des letztmöglichen Produktionsstarttermins.

Folgende Aspekte bilden die Grundfunktionalität der Stückliste:
- Preisberechnung
- Vertextung von Dokumenten
- Planung der Materialwirtschaft
- Organisation der Fertigungssteuerung
- Ermittlung von Fertigungszeiten

#### Maßberechnung
Neben der strukturellen Beschreibung eines Produktes (Stückliste) sind Maßangaben zur konkreten Dimensionierung eines Artikels notwendig. Im Artikelstamm können zu jedem Artikel Maßeinheiten und in der Stückliste Maßberechnungsformeln hinterlegt werden. Zusätzlich können in den Artikelstammdaten eventuelle Zuschläge oder Zuschnittskorrekturen erfasst werden. Diese Maßberechnung wird an die verschiedenen Unterteile der Stückliste vererbt. In der Vorgangserfassung werden dann die Maße für das fertige Produkt abgefragt. A+W Enterprise rechnet Zuschläge und Zuschnittskorrekturen automatisch für die Produktion hinzu.

#### Warengruppe
Die Warengruppen-Struktur beschreibt eine sinnvolle und übersichtliche Produktgliederung. In den Artikelstammdaten muss jeder Artikel einer Warengruppe und einer Produktgruppe zugeordnet werden. Dadurch können alle Verkaufsstatistiken und Umsätze oder Artikelpreise warengruppen- und produktgruppengenau erstellt werden. Dies spielt auch bei der Vergabe von Konditionen eine große Rolle.

#### Preise und Konditionen
Basis der Stammdaten für Preise und Kondition sind regionale, nationale und ausländische Preislisten. Es ist möglich, auf mehrere Preislisten gleichzeitig zuzugreifen, um Vergleichskalkulationen durchführen zu können. Konditionen erlauben die korrekte Auswahl bzw. Abweichung von allgemein hinterlegten Preisen.

Bei der Zuweisung von Konditionen wird folgende Hierarchie durchlaufen:
1. Allgemeine Vereinbarungen
2. Kunden-/lieferantenbezogene Vereinbarungen
3. Objektbezogene Vereinbarungen
4. Auftrags-/angebotsbezogene Vereinbarungen

Innerhalb dieser Hierarchiestufen können allgemeine Preise und Konditionen (für Warengruppen, Artikel usw.) hinterlegt werden. In den Preispflegemodulen gibt es umfangreiche Funktionen zum Kopieren und Verändern von Preisen, entweder betragsgenau oder prozentual. Eine automatische Umstellung aller Preislisten zu einem Stichtag ist ebenso möglich wie die zeitliche Begrenzung von Konditionsvereinbarungen. Durch die Erfassung von Preislisten in Fremdwährungen kann die Vorgangserfassung und die Kalkulation direkt in einer Fremdwährung erfolgen. Die Statistiken werden allerdings in der Landeswährung geführt.

#### Arbeiten mit Shared Memory
Da der Artikelstamm sehr umfangreich ist und daher auch viel Speicherplatz benötigt, gibt es die Möglichkeit, dass Artikelstammdaten in einem Zwischenspeicher (Shared Memory) abgelegt werden. Dies erleichtert den Datenfluss und die Ladezeit bei gleichzeitigen Zugriffen auf die Datenbank wird minimiert. Während man Änderungen an dem Artikelstamm vornimmt sollte das Shared Memory ausgeschaltet werden, damit die Änderungen sofort wirksam werden und z.B. in der Auftragserfassung getestet werden können.

### Übungen
Alle Geschäftsbereiche greifen auf die in den Stammdaten hinterlegten Daten zu. Um Ihnen einen Eindruck von den Stammdaten zu vermitteln, werden in diesem Übungsabschnitt ein neuer Marktpartner und ein ESG-Artikel angelegt. Bei der Pflege der Daten wird auf eine Vielzahl von bereits zuvor angelegten Stammdaten (z.B. Farben, definierte Routen) zugegriffen.

> **Trainerinfo:**
> Der Trainer sollte vor der jeweiligen Übung den Teilnehmer den Dialog Marktpartner sowie den Dialog Artikel kurz vorstellen, da die Komplexität der Stammdaten einen Anfänger überfordert. Bei der Vorstellung sollten auf die in der Übung zu ändernden Felder sowie auf die Bedienung der Dialoge hingewiesen werden.

#### Übung 1: Anlegen eines Marktpartners
> **Trainerinfo:**
> Der Trainer sollte vor der Übung den Teilnehmern den als Kopiervorlage dienenden Marktpartner vorstellen und hierbei auf die zu ändernden Felder hinweisen und erklären.

Das Anlegen eines Marktpartners ist sehr umfangreich und komplex. Aus diesem Grund wird hier bei der Neuanlage ein bestehender Marktpartner kopiert.
Legen Sie einen neuen Kunden an, indem ein bestehender Kunde kopiert wird. Verschiedene Felder in verschiedenen Registern sollen mit den neuen Kundendaten überschrieben werden.
- Alle Felder im Register **Adresse**
- Im Register **Identifikation** die Felder:
  - Umsatzsteuer-Identifikationsnummer
  - FA-Steuernummer
  - Erlösvertreter
  - Außendienst
  - Innendienst
  - Sachbearbeiter
- Im Register **Lieferung** das Feld:
  - Standardroute
- Im Register **Rechnung** das Feld:
  - Rechnungsart
- Im Register **Zahlung** die Felder:
  - Skonto 1
  - Skonto 2
  - Skonto 3
  - Währung

Sie erreichen den Dialog im Menü **Stammdaten > Marktpartner**. Der Kopiervorgang wird über die Tastenfunktion `<F6>` ausgelöst.

**Übung 1: Lösung**
Die Lösung zur Übung erfolgt in folgenden Arbeitsschritten:
- Kopiervorgang auslösen.
- Kopierte Daten anpassen.
Die Daten des Marktpartners befinden sich in A+W Enterprise in verschiedenen Registern.
  - Register Adresse
  - Register Identifikation
  - Register Bezüge
  - Register Auftrag
  - Register Lieferung
  - Register Rechnung
  - Register Kundenspezifisch
  - Register Zahlung
  - Register Ausdruck
  - Register Limits
  - Register Bewertung
  - Register Produktion
  - Register Modifikation
  - Register Privat
- Neuangelegte Daten speichern

Zur besseren Übersicht fassen wir die Handlungsschritte gemäß den Registern zusammen:

**Einen bestehenden Marktpartner kopieren**
1. Öffnen Sie den Dialog Marktpartner.
2. Wählen Sie im Feld Partnertyp den Typ Kunde.
3. Im Feld Marktpartner drücken Sie die Taste Nummernvergabe `<F6>`. Das System trägt in das Feld Marktpartner die neue Kundennummer ein und es erscheint die Meldung: Achtung (10420): Soll zur NEUAUFNAHME ein bestehender Marktpartner als Muster dienen?
Bestätigen Sie diese Meldung mit [Ja].
4. Im folgenden Dialog wählen Sie im Feld Muster-Partnertyp den Typ Kunde aus.
5. Im Feld Muster-Marktpartner wählen Sie einen bestehen Kunden aus (z. B. 140). Den Dialog verlassen Sie mit `<F3>` Auslösen. Die Daten dieses Kunden werden automatisch in den Dialog übernommen. Das Register Adresse ist aktiv.

**Die Felder des kopierten Marktpartners anpassen (Register Adresse)**
1. Im nächsten Schritt passen Sie das Feld Matchcode an. Dieses Feld ist automatisch als das aktive Feld gewählt. Sie können den Eintrag überschreiben.
2. Im Feld Name überschreiben Sie den Namen des Marktpartners.
3. Im Feld Vorname überschreiben Sie den Vornamen des Marktpartners.
4. Im Feld Anrede können Sie sich über `<F9>` die unterschiedlichen Einträge anzeigen lassen und den gewünschten auswählen.
5. Im Feld z. Hd. geben Sie den Ansprechpartner für Schriftverkehr ein (z. B. Frau Gleich).
6. Das Feld Zusatz ist ein freies Textfeld. Hier kann ein beliebiger Adresszusatz eingetragen werden.
7. Im Feld Straße überschreiben Sie den Straßennamen des Marktpartners.
8. Im Feld PLZ überschreiben Sie die Postleitzahl des Marktpartners, die zum Postfach gehört.
9. Im Feld Fach überschreiben Sie das Postfach des Marktpartners.
10. Im Feld PLZ überschreiben Sie die Postleitzahl des Marktpartners.
11. Im Feld Ort überschreiben Sie den Ort des Marktpartners.
12. Im Feld Fach überschreiben Sie das Postfach des Marktpartners.
13. Im Feld KFZ überschreiben Sie den KFZ-Code (Ländercode) des Marktpartners. Sie ordnen dem Marktpartner damit ein Land zu. Im Dialog Länder im Stammdatenbereich (Stammdaten > Schlüssel > Marktpartnerschlüssel > Länder) kann jedem Land ein sogenannter KFZ-Code, ein Ländercode, zugeordnet werden. Geben Sie einen bereits existierenden KFZ-Code ein, wird die Länderbezeichnung automatisch ergänzt. Geben Sie einen noch nicht vorhandenen KFZ-Code ein, können Sie im folgenden Feld selbst die Bezeichnung eintragen.
14. Im Feld Entfer überschreiben Sie die Entfernung des Marktpartners zu seinem Lieferanten. Es wird die Entfernung in Kilometern angegeben, die zwischen dem A+W Enterprise-Standort (Lieferant) und der aktuell eingegebenen Marktpartneradresse liegt.
15. Im Feld Telefon überschreiben Sie die Telefonnummer des Marktpartners.
16. Im Feld Fax überschreiben Sie die Faxnummer des Marktpartners. Über das hinter dem Feld liegende Ja/Nein Toggel können Sie angeben, ob an diesen Kunden aus dem Verkauf heraus Faxe versendet werden dürfen oder nicht.
17. Im Feld E-Mail überschreiben Sie die E-Mailadresse des Marktpartners.
18. Im Feld Webseite überschreiben Sie den Namen der Webseite des Marktpartners. Der Eintrag kann mit und ohne Präfix http:// gepflegt werden.
19. Im Feld Sprache überschreiben Sie das Sprachkennzeichen des Marktpartners. Mit `<F9>` können Sie sich die Sprachkennzeichen anzeigen lassen und das gewünschte auswählen. Bei der automatischen Generierung von Texten wird das Sprachkennzeichen ausgewertet.

**Die Felder des kopierten Marktpartners anpassen (Register Identifikation)**
1. Mit `<F2>`, den Pfeiltasten neben den Registern oder mit klicken auf das Register Identifikation wechseln Sie in das Register Identifikation.
2. Passen Sie das Feld Umsatzsteuer-Identifikationsnummer an. Dieses Feld ist automatisch als das aktive Feld gewählt. Sie können den Eintrag überschreiben.
3. Im Feld FA-Steuernummer überschreiben Sie die Steuernummer, die der Marktpartner vom Finanzamt erhalten hat.
4. Im Bereich Provision überschreiben Sie das Feld Vertr. (Erlös) des Marktpartners. Hier wird der Mitarbeiter eingetragen, der für abgearbeitete Aufträge Provisionen erhält.
5. Im Feld Außendienst überschreiben Sie den zuständigen Außendienstmitarbeiter des Marktpartners.
6. Im Feld Innendienst überschreiben Sie den zuständigen internen Mitarbeiter des Marktpartners.
7. Im Feld Sachbearbeiter überschreiben Sie den Sachbearbeiter des Marktpartners. Der Sachbearbeiter ist Ansprechpartner für die Auftragserfassung.

**Die Felder des kopierten Marktpartners anpassen (Register Lieferung)**
1. Mit `<F2>`, den Pfeiltasten neben den Registern oder mit klicken auf das Register Lieferung wechseln Sie in das Register Lieferung.
2. Passen Sie das Feld Std.-Route an. Dieses Feld ist automatisch als das aktive Feld gewählt. Sie können sich über `<F9>` die unterschiedlichen Routen anzeigen lassen und die gewünschte auswählen. Der Eintrag wird so überschreiben.
Die Route beschreibt den Streckenverlauf und an welchen Tagen die Strecke gefahren wird. Der Marktpartner wird standardmäßig mit der angegebenen Route angefahren.

**Die Felder des kopierten Marktpartners anpassen (Register Rechnung)**
1. Mit `<F2>` oder den Pfeiltasten neben den Registern oder mit Klicken auf das Register Rechnung wechseln Sie in das Register Rechnung.
2. Im Feld Rechnungsart ändern Sie die Rechnungsart per `<Leertaste>` auf Sammelrechnung: wöchentlich.

**Die Felder des kopierten Marktpartners anpassen (Register Zahlung)**
1. Mit `<F2>`, den Pfeiltasten neben den Registern oder mit Klicken auf das Register Zahlung wechseln Sie in das Register Zahlung.
2. Im Feld Skonto 1 überschreiben Sie die Skontoangabe des Marktpartners. Bei der Auswahl der Daten steht Ihnen ein Selo `<F9>` zur Verfügung.
3. Im Feld Skonto 2 überschreiben Sie die Skontoangabe des Marktpartners. Bei der Auswahl der Daten steht Ihnen ein Selo `<F9>` zur Verfügung.
4. Im Feld Skonto 3 überschreiben Sie die Skontoangabe des Marktpartners. Bei der Auswahl der Daten steht Ihnen ein Selo `<F9>` zur Verfügung.
5. Im Feld Währung überschreiben Sie die Währung des Marktpartners. Bei der Auswahl der Daten steht Ihnen ein Selo `<F9>` zur Verfügung.

**Kunden speichern**
1. Verlassen Sie den Kunden speichernd mit `<Ende>`. Es erscheint die Meldung: Achtung (10431): Wollen Sie speichern? Bestätigen Sie diese Meldung mit [Ja].
2. Nun erscheint die Meldung: Hinweis: Wünschen Sie eine FIBU-Übergabe? Bestätigen Sie diese Meldung mit [Ja]. Der neu angelegte Kunde wird somit automatisch an die angebundene Software für die Finanzbuchhaltung übergeben.

#### Übung 2: Anlegen eines ESG-Artikels
> **Trainerinfo:**
> Der Trainer sollte vor der Übung den Teilnehmern den Artikel 350008 vorstellen und auf die zu ändernden Felder hinweisen und diese erklären. Hierbei steht die Onlinehilfe zur verfügung

Das Anlegen eines neuen Artikels ist sehr umfangreich und komplex. Aus diesem Grund wird hier bei der Neuanlage ein bestehender Artikel kopiert.
Legen Sie eine neue ESG-Scheibe mit der Dicke von 10 mm mit der Artikelnummer 99350010 an. Als Kopiervorlage dient eine bestehende ESG-Scheibe mit der Stärke von 8 mm (Artikelnummer: 350008). Verschiedene Felder in verschiedenen Registern sollen überschrieben werden:
- Im Register **Identifikation** die Felder:
  - Matchcode
  - Hauptbezeichnung
  - Internbez.
  - Kurzbezeichnung
  - Warengruppe
- Im Register **Phys. Eigenschaften** das Feld:
  - Dickenmaß
- Im Register **Rechnung** das Feld:
  - Rechnungsart
- Im Register **Beschaffung** die Felder:
  - Beschaffungsart

Sie erreichen den Dialog im Menü **Stammdaten > Artikelstamm**.

**Übung 2: Lösung**
Die Lösung zur Übung kann mit folgenden Arbeitsschritten erarbeitet werden:
- Kopiervorgang auslösen
- Kopierte Daten anpassen. Die Daten des Artikels befinden sich in A+W Enterprise in verschiedenen Registern.
  - Register Identifikation
  - Register Phys. Eigenschaften
  - Register Maßrestriktionen
  - Register Einbaurestriktionen
  - Register Beschaffung
  - Register Produktion
  - Register Preise
  - Register Lager
  - Register Techn. Werte
  - Register Statistik
  - Register Modifikation
  - Register Privat
- Neuangelegte Daten speichern

Zur besseren Übersicht fassen wir die Handlungsschritte gemäß den Registern zusammen:

**Einen bestehenden Artikel kopieren**
1. Öffnen Sie den Dialog Artikelstamm.
2. Im Feld Artikel tragen Sie die neue Artikelnummer **99350010** ein (99 steht für Test-Artikel 35 für die Warengruppe und 10 für die Dicke).
Es erscheint die Meldung: Achtung (10061): Soll zur NEUAUFNAHME ein alter Artikel als Muster dienen?
Bestätigen Sie diese Meldung mit [Ja].
3. Im folgenden Dialog tragen Sie in das Feld Musterartikel die Artikelnummer **350008** ein. Den Dialog verlassen Sie mit `<Enter>`. Die Daten werden automatisch in den Dialog Artikel übernommen. Das Register Identifikation ist aktiv.

**Die Felder des kopierten Artikels anpassen (Register Identifikation)**
1. In nächsten Schritt passen Sie das Feld Matchcode an. Dieses Feld ist automatisch als das aktive Feld gewählt. Sie können den Eintrag überschreiben.
2. Im Feld Hauptbezeichnung überschreiben Sie die Hauptbezeichnung.
3. Im Feld Internbez. überschreiben Sie die interne Bezeichnung des Artikels.
4. Im Feld Kurzbezeichnung überschreiben Sie die Kurzbezeichnung des Artikels.
5. Im Feld Warengruppe überschreiben Sie die Warengruppe des Artikels mit der Warengruppe **35F700 ESG Float normal unbearbeitet**. Dieser Eintrag wird über ein Selo ausgewählt. Dies geschieht, in dem Sie in dem Feld Warengruppe stehen und `<F9>` drücken. Jetzt geben Sie bitte **35** in das Feld Warengruppen für ESG ein und drücken `<Enter>`. Es erscheint ein Dialog mit einer zusammengefassten Treffermenge von Warengruppen für ESG. Hieraus wählen Sie bitte die Warengruppe **35F700** aus.

**Die Felder des kopierten Artikels anpassen (Register Phys. Eigenschaften)**
1. Mit `<F2>`, den Pfeiltasten neben den Registern oder mit klicken auf das Register Phys. Eigenschaften wechseln Sie in das Register physikalische Eigenschaften.
2. Im nächsten Schritt passen Sie das Feld Dickenmaß an. Sie erreichen das Feld in dem Sie in das Feld mit der Maus klicken oder Sie laufen mit den Pfeiltasten zu dem Feld. Sie überschreiben den Eintrag mit **10**.

**Die Felder des kopierten Artikels anpassen (Register Beschaffung)**
1. Mit `<F2>`, den Pfeiltasten neben den Registern oder mit klicken auf das Register Beschaffung wechseln Sie in das Register Beschaffung.
2. Im nächsten Schritt passen Sie das Feld Beschaffungsart an. Dieses Feld ist automatisch als das aktive Feld gewählt. Sie überschreiben den Eintrag mit **3** und setzen so die Beschaffungsart auf Produktion. Der Wert kann auch über eine Selo `<F9>` ausgewählt werden.

**Artikel speichern**
Um die neu angelegte Daten zu speichern, drücken Sie `<Ende>`. Es erscheint die Meldung: Achtung (10066): Wollen Sie speichern? Bestätigen Sie diese Meldung mit [Ja].

---
## Softwarereferenz: Stammdaten

**In diesem Kapitel finden Sie folgende Themen:**
- Stammdaten – Übersicht
- Marktpartner
- Mitarbeiter
- Abteilungen
- Marktpartnerschlüssel
- Systemschlüssel
- Produktschlüssel
- Artikel
- Stückliste
- Warengruppen
- Fertige Produkte
- Feldkonfiguration
- Provisionen
- Textverwaltung
- Kostenstamm
- Preise
- Konditionen
- Listendruck

### Stammdaten – Übersicht
Stammdaten sind zeitunabhängige Daten, die nie bzw. nur selten verändert werden. Sie sind der Dreh- und Angelpunkt des gesamten Systems, da Bezüge zu allen anderen Bereichen bestehen. Ziel der Stammdatenverwaltung ist es, einen einzigen, durchgängigen Datenbestand für alle im Einsatz befindlichen Anwendungen zu schaffen.

Alle Dialoge und Funktionen, die die Stammdaten betreffen, befinden sich in diesem Menü:

| Short Cut | Beschreibung |
|---|---|
| a | "Marktpartner" auf Seite B-97 |
| b | "Mitarbeiter" auf Seite B-176 |
| c | "Abteilungen" auf Seite B-184 |
| da | "Marktpartnerschlüssel" auf Seite B-186 |
| db | "Systemschlüssel" auf Seite B-236 |
| dc | "Produktschlüssel" auf Seite B-292 |
| dd | Preisschlüssel finden Sie in einem separaten Dokument |
| e | "Artikel" auf Seite B-377 |
| f | "Stückliste" auf Seite B-485 |
| g | "Warengruppen" auf Seite B-491 |
| h | "Fertige Produkte" auf Seite B-497 |
| i | "Feldkonfiguration" auf Seite B-501 |
| k | "Provisionen" auf Seite B-510 |
| l | "Textverwaltung" auf Seite B-513 |
| m | "Kostenstamm" auf Seite B-522 |
| n | "Preise" auf Seite B-528 |
| o | "Konditionen" auf Seite B-529 |
| p | "Listendruck" auf Seite B-530 |

> **Preise und Konditionen**
> Die Themen Preise, Konditionen und Listendruck sind in einem getrennten Dokument beschrieben!

### Marktpartner
Im Marktpartnerstamm werden alle kunden-, objekt- und lieferantenbezogenen Angaben hinterlegt sowie Einmal-Daten (Partnertyp Sonstiger).
Die Angaben reichen von der Erfassung der Firmenadresse bis hin zu Lieferanschriften, Routen, Zahlungskonditionen und Bewertungen.

#### Marktpartner-Kopf
Nachdem Sie den Dialog geöffnet haben, müssen Sie zunächst im Kopfbereich den Marktpartner auswählen.
Die Inhalte der einzelnen Register beziehen sich immer auf den im Kopf gewählten Marktpartner.
Im A+W Enterprise werden folgende Marktpartnertypen unterschieden:
- Kunde
- Lieferant
- Sonstiger
- Objekt
- Eigentümer (Gestelle)

[Image: Abb. B-7 Marktpartner - Kopf]

- **Partnertyp:** Toggle-Feld für Marktpartnertyp. Folgende Auswahlmöglichkeiten stehen zur Verfügung:
  - **Kunde:** Im Kundenstamm sind alle kundenbezogenen Angaben enthalten, inklusive der kundenindividuellen Artikeldefinitionen. Marktpartner vom Typ Kunde benötigen Sie vor allem in der Erfassung von Verkaufsvorgängen.
  - **Lieferant:** Im Lieferantenstamm werden alle lieferantenbezogenen Angaben hinterlegt inklusive lieferantenindividueller Artikelangaben. Marktpartner vom Typ Lieferant benötigen Sie vor allem in der Erfassung von Einkaufsvorgängen. Lieferanten können direkt in Aufträgen und im Artikelstamm als Lieferanten für zu bestellende Artikel eingegeben werden.
  - **Sonstiger:** Unter diesem Typ werden gewöhnlich Einmal-Kunden geführt, für die dann auch nur die Adresse angelegt wird. Innerhalb der erweiterten internen Mandantentrennung werden die Firmen als Sonstiges angelegt.
  - **Objekt:** Unter einem Objekt wird üblicherweise ein größeres Bauvorhaben (Projekt) verstanden. Unter diesem Oberbegriff werden Definitionen technischer Art, Konditionen preislicher Art (EK und VK) und weitere geschäftliche Vereinbarungen (Mengen, Zeiten etc.) zusammengefasst.
  - **Eigentümer:** Eigentümer für Gestelle.
    Technische Info: Toggle-Feld, DB-Feld: mp.kuliflag
- **Marktpartner:** Auswahl der Nummer oder wenn bekannt, Eingabe derselben. Soll ein neuer Marktpartner angelegt werden, drücken Sie `<F6>`.
  "Marktpartnersuche" auf Seite B-100
  Technische Info: `<F9>`, DB-Feld: mp.kunr
- **Matchcode:** Bei der Wahl eines bestehenden Marktpartners wird der Matchcode angezeigt und bei der Erfassung eines neuen Marktpartners muss man einen Matchcode eingeben. Der Matchcode ist ein freies Textfeld in dem eine Kurzbezeichnung für den Marktpartner eingegeben wird. Der Matchcode dient vor allem der vereinfachten Suche.

#### Register
Der Dialog beinhaltet verschiedene Register. Die Inhalte der einzelnen Register können - abhängig vom Partnertyp - unterschiedlich sein:
- "Register Adresse" auf Seite B-103
- "Register Identifikation" auf Seite B-108
- "Register Bezüge" auf Seite B-111
- "Register Auftrag" auf Seite B-113
- "Register Lieferung" auf Seite B-116
- "Register Rechnung" auf Seite B-120
- "Register Kundenspezifisch" auf Seite B-122
- "Register Zahlung" auf Seite B-124
- "Register Ausdruck" auf Seite B-127
- "Register Limits" auf Seite B-130
- "Register Bewertung" auf Seite B-133
- "Register Produktion" auf Seite B-135
- "Register Modifikation" auf Seite B-136
- "Register Privat" auf Seite B-137

### Marktpartner - Kontextmenü
**Stammdaten > Marktpartner > F4**
Über das Kontextmenü (`<F4>`) haben Sie Zugriff auf folgende Bereiche:

| Short Cut | Eintrag | Beschreibung |
| --- | --- | --- |
| a | Kontaktdaten | "Ansprechpartner" auf Seite B-138, "Adressen" auf Seite B-140, "Bankverbindungen" auf Seite B-145, "E-Mailadressen" auf Seite B-146 |
| b | Rabatte | "Rabatte" auf Seite B-150 |
| c | Austausch-/Zusatzregeln | "Austausch-/Zusatzregeln" auf Seite B-152 |
| d | Gestelltypen | "Gestelltypen" auf Seite B-153 |
| e | Konfigurierte MP-Felder | "Konfigurierte MP-Felder" auf Seite B-155 |
| f | Mitarbeiterzuordnungen | "Vertreterzuordnung" auf Seite B-156, "Erfasserzuordnung" auf Seite B-157 |
| g | Gruppenzuordnung | "Gruppenzuordnung" auf Seite B-158 |
| | Objektzuordnung | "Objektzuordnung" auf Seite B-159 |
| | Farbzuordnung | "Farbzuordnung" auf Seite B-161 |
| h | Bonuszuordnung | "Bonuszuordnung" auf Seite B-162 |
| i | Artikelzuordnung | "Artikelzuordnung" auf Seite B-163 |
| k | Texte/Druck | "Marktpartnertexte" auf Seite B-165, "Marktpartner-Artikeltexte" auf Seite B-167, "Formulare" auf Seite B-168, "Dokumentenarten" auf Seite B-169 |
| l | Vorgangs-Recherche | "Vorgangs-Recherche" auf Seite B-170 |
| m | Marktpartner-Info | "Marktpartner-Info" auf Seite B-171 |
| n | Replikationsdaten | "Replikationsdaten" auf Seite B-172 |
| o | DFÜ-Konfiguration | "DFÜ-Konfiguration" auf Seite B-174 |
| p | Hausspezifische Angaben | "Hausspezifische Angaben" auf Seite B-175 |

> **Kontextmenü**
> Das Kontextmenü ist abhängig vom Marktpartnertyp aufgebaut.

### Marktpartnersuche
**Stammdaten > Marktpartner > Feld Marktpartner > <F9>**

[Image: Abb. B-8 Marktpartnersuche]

In diesem Such-Dialog legen Sie die Auswahlkriterien für die Marktpartnersuche fest.
Sobald Sie in den Suchfeldern eine Eingabe machen, wird die Treffermenge automatisch angepasst.
Über die Schaltfläche Details starten Sie einen Dialog, der Ihnen die zugeordneten Häuser auflistet (für Multi-Site).

> **Daten**
> Die Daten dieses Suchdialogs werden in den Speicher geladen und sind nur zum Zeitpunkt des Ladens aktuell. Haben Sie im Marktpartnerstamm eine Änderung vorgenommen, müssen Sie die Schaltfläche [Refresh] drücken, um die angezeigten Daten im Suchdialog zu aktualisieren.

Die Register Adresse und Identifikation im Trefferbereich liefern Ihnen eine Übersicht zu häufig verwendete Daten der Marktpartner.

> **Anzahl der angezeigten Daten**
> Da die anzuzeigende Datenmenge extrem hoch sein kann (z. B. alle Kunden eines Landes) werden für die Suche nicht alle existierenden Daten automatisch in den Zwischenspeicher geladen. Eine Information hierzu

