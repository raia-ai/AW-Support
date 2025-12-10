---
description: "DE_HB_AWProduction_1"
---


# A+W Production Handbuch

**Software for Glass, Windows & Doors**

---
## Editorial

### Revisionsübersicht der Dokumentation

| Datum | Änderung |
| :--- | :--- |
| 10-2024 | Gesamthandbuch für PDF und HTML5-Format aktualisiert. |

### Anmerkungen

Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Production gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.

Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von A+W Production.

### Urheberrechte

© 2024, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

### Darstellungskonventionen

Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

| Stil | Bedeutung |
| :--- | :--- |
| *Kursiv* | sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Preiseigenschaften*. |
| **Fett** | sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: Geben Sie den Wert **5** ein. |
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

## Inhalt

### Überblick (A)
- **Tutorial** A-19
- **Überblick** A-22
  - Aufbau des Tutorials A-22
  - Produktportfolio der A+W Software GmbH A-24
  - A+W Production stellt sich vor A-25
- **Basismodul A+W Production** A-27
  - Einlastung A-28
    - Einlastung allgemein A-29
  - Grobplanung A-31
    - Grobplanung allgemein A-32
    - Die Auftrags-Anzeige (Pool) A-33
    - Die Auftragsübersicht A-34
    - Die Topf-Anzeige A-34
    - Die Positions-Anzeige A-35
    - Die Glasarten-Anzeige A-36
    - Die Detail-Anzeige A-36
    - Die Bearbeitungs-Anzeige A-37
    - Die Füllauftrag-Anzeige A-37
    - Die Lauf-Anzeige A-37
  - Läufe bilden A-38
    - Bildung von Läufen A-38
    - Allgemeine Regeln A-39
  - Feinplanung A-40
    - Feinplanung allgemein A-41
    - Ablauf der Feinplanung A-41
    - Gruppierungen und Sortierungen A-43
    - Abstellplatz- und Stapellogik A-44
    - Abstellmodi für A-Böcke A-45
    - Abstellmodi für Fächerwagen A-45
  - Optimierungs-Modi A-46
    - Optimierungsmodus XOPTS 6.2 - Feste Reihenfolge A-46
    - Optimierungsmodus XOPTS 6.1 - Kunden zusammenhalten A-46
    - Optimierungsmodus XOPTS 5.2 - Standard. A-47
    - Optimierungsmodus XOPTS 5.1 - ISO auf Fächerwagen oder viele A-Böcke A-47
  - Organisationsformen A-49
    - Orga-Typ und Los-Typ A-49
  - Maschinenzuordnung A-50
    - Bestandteile der Maschinenzuordnung A-52
    - Maschinen in der Maschinenzuordnung A-53
    - Arbeitsgänge in der Maschinenzuordnung A-54
    - Arbeitsgangzuordnung A-55
    - Bearbeitungstypen in der Maschinenzuordnung A-56
    - Bearbeitungsartikel in der Maschinenzuordnung A-56
- **Ausbaumodule A+W Production** A-58
  - Kapazitätsplanung A-59
    - A+W Capacity Planner A-61
    - Produktionsmonitor A-62
    - Kampagneneditor A-63
    - Schichteditor A-64
    - Grafisch-orientierte Terminumlastung A-65
  - Optimierungssysteme A-66
    - Realtime Optimizer A-67
    - Tischoptimierungen A-68
    - Tischansteuerung A-68
    - Stammdaten A-68
    - Sequence Optimizer A-69
    - Shape Optimizer A-70
    - Rack Optimizer A-71
    - DynOpt A-72
    - Furnace Optimizer A-73
  - Barcode Manager A-74
    - Allgemein A-75
    - Scanner A-75
  - Anzeige- und Leitrechnersysteme A-77
    - Production Terminal A-78
    - Manual Cutting A-78
    - Order A-79
    - Processing A-80
    - IG-In A-81
    - IG-Assembly A-82
    - IG-Out A-83
    - TG-In A-84
    - TG-Out A-85
    - Ziel der Production Terminals A-85
  - Statistiksysteme A-86
    - A+W Discovery A-87
    - Production Cockpit A-88
- **Konventionen** A-89
  - Bedienoberfläche A-91
    - Dialoge A-91
    - Schaltflächen A-92
  - Dokumentation A-96
    - Aufbau des Handbuchs A-96
    - Online-Hilfe A-98
    - Hilfethemen A-98
    - Register Inhalt A-99
    - Register Index A-100
    - Register Suchen A-101
    - Hilfetext nicht gefunden A-101

### Grobplanung (C)
- **Tutorial** C-105
  - Überblick C-107
    - Aufbau des Tutorials C-107
  - Grobplanung C-109
    - Prozess der Arbeitsvorbereitung C-110
  - Ansichten C-113
    - Ansichten in der Grobplanung C-114
    - Konfigurieren von und arbeiten mit Ansichten C-117
    - Register anlegen und konfigurieren C-117
    - Spalten anlegen und konfigurieren C-119
    - Summenzeile anlegen und konfigurieren C-121
    - Neue Spalte oder Summenzeile definieren C-123
    - Filter anlegen und konfigurieren C-126
    - Weißer Screen in einer Ansicht C-129
    - Übungen: Konfigurieren von und arbeiten mit Ansichten C-130
  - Aufträge / Pool C-131
    - Aufträge in der Grobplanung C-132
  - Töpfe C-134
    - Töpfe in der Grobplanung C-135
  - Läufe und Laufstrategien C-140
    - Läufe in der Grobplanung C-141
  - Positionen C-147
    - Positionen in der Grobplanung C-148
    - Vorgang suchen C-150
- **Softwarereferenz** C-151
  - Grobplanung C-154
  - Aufträge in der Grobplanung C-155
    - Aufträge C-156
    - Auftragsübersicht C-159
    - Füllaufträge C-162
    - Übermengen-Editor C-165
    - Änderung der Beschaffungsart C-167
  - Töpfe in der Grobplanung C-169
    - Töpfe C-170
    - Reservierungsaufträge-Topf C-173
    - Bestellteile-Topf C-177
    - Topf-Bildung C-180
    - Topfbezeichnung ändern C-182
  - Läufe in der Grobplanung C-183
    - Läufe C-184
    - Lauf-Bildung C-187
    - Sonderglas-Lauf bilden C-189
    - Laufbezeichnung ändern C-190
    - Freigabe Lauf (Name): AUW – Wiederholung C-191
  - Positionen in der Grobplanung C-194
    - Positionen C-195
    - Auftrag zu Positionen hinzufügen C-198
    - Positionssplit C-199
    - Felddefinition C-201
    - Export/Import Positionsansicht C-203
  - Bearbeitungen in der Grobplanung C-204
    - Bearbeitungen C-205
    - Vorgabezeiten ändern C-208
  - Glasarten, Details, BDE und Lose C-209
    - Glasarten C-210
    - Details C-213
    - BDE C-217
    - Lose C-221
  - Übergreifende Dialoge C-224
    - Arbeitsplan C-225
    - Eigenschaften von (Register) C-228
    - Spaltendefinition C-229
    - (Filter Name) C-230
    - Filter-Definition C-231
    - Dokumentenverknüpfungen C-233
    - Entschichtungsflächen C-234
  - Übergreifende Kontextmenüs C-236
- **Help Cards** C-241
  - Informationen zu den Help Cards C-243
  - Läufe C-244
    - Läufe bilden C-245
    - Läufe ergänzen C-246
    - Läufe zusammenfügen C-247
    - Läufe auflösen C-248
    - Aufträge aus Läufen entfernen C-249
    - Läufe archivieren oder löschen C-250
  - Ansichten C-251
    - Spalte oder Summenzeile hinzufügen C-252

### Feinplanung (D)
- **Tutorial** D-255
  - Dokumentations-Hinweise D-258
    - Wichtige Hinweise D-258
    - Aufbau des Tutorials D-259
  - Überblick Feinplanung D-260
    - Ablauf der A+W Production D-261
    - Begriffe der A+W Production D-263
    - Lostyp D-263
    - Lose D-264
    - Böcke (Abstellplätze) D-264
    - Läufe D-265
    - Archivierungsmethode D-267
    - Teilebaum D-270
    - Organisation (Orga) D-271
  - Gruppierungen und Sortierungen D-272
    - Überblick D-273
    - Einführung D-274
    - Gruppierung D-275
    - Sortierung D-276
    - Zusatz-Sortierung D-279
    - Sonderteile D-281
    - Demos und Übungen D-285
  - Abstellplätze und -modi D-287
    - Überblick D-288
    - Abstellplätze D-289
    - Logische Abstellplätze D-289
    - Abstellregeln D-290
    - Vordefinierte Abstellmodi für A-Böcke D-292
    - Robot-Böcke D-298
    - Abstellmodi für Fächerwagen D-298
    - Standard-Einstellungen in der Konfiguration D-299
    - Einstellungen in den Stammdaten D-300
    - Demos und Übungen D-303
  - Optimierungsmodi D-306
    - Überblick D-307
    - Unterschiedliche Optimierungs-Modi D-308
    - Demos und Übungen D-317
  - Orgas D-319
    - Organisationsformen D-320
    - Allgemein D-321
    - Produktionsreihenfolge D-333
    - Allgemein D-334
    - A+W Standard-Orgas D-336
  - Abstellplatzorganisation D-337
    - A-Böcke SZR D-338
    - ISO-A-Böcke D-345
    - A-Böcke Versand D-351
    - Fächerwagen ohne Auffüllen D-356
    - Aufgefüllte Fächerwagen D-361
    - Demos und Übungen D-366
- **Softwarereferenz** D-369
  - Übersicht D-371
  - Organisationen D-372
    - Register Master-Orga D-372
    - Register Produktionsreihenfolge D-374
    - Register Prüfreihenfolge D-376
    - Master-Orga D-378
    - Orga D-383
    - Orga-Gruppen D-385
    - Einstellungen-Abstellplatz D-387
    - Voreinstellungen D-391
  - Gruppierung und Sortierung D-392
    - Gruppierung/Sortierung - Dialog D-392
  - Abstellplätze D-398
    - Abstellplätze D-398
  - Lose D-403
    - Lostypen und Bearbeitungen D-403
  - Läufe feinplanen D-410
    - Feinplanung für Lauf D-410
    - Register Glasarten D-411
    - Register Bockbelegung D-414
    - Register Ergebnisse D-419
    - Register Spezial D-421
    - Register Zusammenlegen D-421
    - Register Füllaufträge D-423
    - Register Restblätter D-425
    - Register Bruchscheiben D-426
    - Register Eilscheiben D-428
    - Register Glasdicken D-429
    - Register Freie Optimierung D-431
    - Register Teilmengen D-432
    - Register Orga D-434
    - Register Orga-Optionen D-436
    - Register Optionen D-438
    - Register Auswahl Lagermaß D-440
    - Ändern der minimalen Anzahl A-Böcke D-441
    - Reihenfolge der Maschinen D-442

### Kapazitätsplanung (E)
- **Tutorial** E-447
  - Überblick E-450
    - Aufbau des Tutorials E-451
  - Grundlagen E-452
    - Terminoptimierung E-453
    - Terminfindung E-454
  - Planung und Einlastung E-459
    - Produktionsmonitor E-460
    - Tagesaktuelle Anpassungen der Arbeitsschichten E-462
    - Produktionsmonitor einrichten E-469
    - Arbeitsplan exportieren E-472
  - Einlastung und Umlastung E-473
    - Aufträge einlasten E-474
    - Umlastungen E-475
    - Bearbeitungen umlasten E-477
    - Fehlerhafte Einlastung E-479
    - Eingelastete Aufträge nachbearbeiten E-480
  - Kampagnenplanung E-482
    - Definition der Kampagnen E-483
    - Kampagnen in der Terminfindung E-485
    - Kampagnen anlegen und verwalten E-485
    - Übungen zu Kampagnen E-492
  - Reservierungen E-493
    - Reservierung von Kapazitäten E-494
    - Reservierungen anlegen und verwalten E-495
    - Übungen zu Reservierungen E-501
  - Bearbeitungserzeugung E-502
    - Bearbeitungserzeugung für die Einlastung E-503
    - Bearbeitungen erzeugen E-504
  - Stammdaten der Kapazitätsplanung E-507
    - Schichten E-508
    - Schichtpläne E-509
    - Arbeitsfreie Tage anlegen E-511
    - Schichtplan erstellen E-514
    - Schichtregel erstellen E-517
    - Schichtgruppe erstellen E-522
    - Übungen E-526
  - Kostenkalkulation E-527
    - Definition der Kostenkalkulation E-528
    - Kosten anlegen und verwalten E-529
    - Übungen E-531
  - Übergangszeiten E-532
    - Übergangszeiten in Schichten oder Stunden E-534
    - Definition von Übergangszeiten E-538
    - Übergangszeiten anlegen und verwalten E-541
    - Übungen E-544
  - Vorgabezeiten E-545
    - Definition der Vorgabezeiten E-546
    - Struktur von Vorgabezeitformeln E-547
    - Berechnung von Zeitzuschlägen E-550
    - Editor für Formelelemente E-552
    - Zeitformel-Objekte E-556
    - Vorgabezeitformeln anlegen und verwalten E-557
    - Zeitformel testen E-563
    - Übungen E-569
  - Maschinengruppen E-570
    - Definition der Maschinengruppen E-571
    - Maschinengruppen anlegen und verwalten E-572
    - Übungen E-575
  - Lastverteilung E-576
    - Definition der Lastverteilung E-577
    - Lastverteilung einrichten und bearbeiten E-578
    - Übungen E-581
- **Softwarereferenz** E-583
  - Überblick E-586
  - Einlastung E-587
    - Produktionsmonitor E-588
    - Angezeigte Maschinen E-592
    - Einstellungen E-593
    - Bitte wählen Sie einen Auftrag / Lauf aus (Filtern) E-596
    - Maschine (Name) E-600
    - Schichten für Maschine anpassen E-602
    - Schichteigenschaften E-603
    - Reservierungsanzeige E-605
    - Arbeitsplan aus Produktionsmonitor E-606
  - Einlastung E-610
    - Stücklistenkonfiguration E-611
    - Aktion E-612
  - Umlastung E-613
    - Maschinenumlastung E-618
    - Nachbearbeitung Einlastung E-619
    - Fehlerhafte Aufträge E-622
    - Asynchrone Verarbeitung E-623
    - Änderung bereits verplanter Aufträge E-624
    - Positionssplit E-625
  - Kampagnen und Reservierungen E-627
    - Kampagnen E-628
    - Abgelaufene Reservierungen E-632
    - Reservierungen E-634
  - Bearbeitungen E-640
    - Bearbeitungserzeugung E-641
  - Stammdaten für Zeiten E-645
    - Vorgabezeiten E-646
    - Vorgabezeitformel E-648
    - Elemente hinzufügen E-652
    - Eigenschaften des Formelobjekts E-663
    - Formel (Name) E-665
    - Verlauf der Formelauswertung E-666
    - Übergangszeiten E-667
  - Stammdaten der Schichten E-670
    - Schichten E-671
    - Schichtkalender E-673
    - Schichtplan E-674
    - Schichtregel E-676
    - Schichtgruppe E-678
  - Maschine E-680
    - Maschinen und Kosten E-682
    - Kostenkalkulation E-683
    - Maschinengruppen E-685
  - Lastverteilung E-687
- **Help Cards** E-689
  - Informationen zu den Help Cards E-691
  - Kapazitätsplanung E-692
    - Schichtplan erstellen E-693
    - Schichtregeln erstellen E-694
    - Schichtgruppe erstellen und zuordnen E-695
    - Neue Maschine integrieren E-696
    - Maschine verschieben E-697
    - Vorgabezeiten anlegen E-698
    - Kostensätze definieren E-699
    - Schichteigenschaft flexibel ändern E-700
    - Bearbeitungstermin umlasten E-701
    - Versandtermin umlasten E-702

### Formeleditor (F)
- **Tutorial** F-705
  - Der Formeleditor F-707
    - Ziele des Formeleditors F-707
    - Elemente des Formeleditors: Stufe I F-707
    - Elemente des Formeleditors: Stufe II F-713
    - Elemente des Formeleditors: Stufe III F-717
  - Notation Formula.dll F-719
    - Syntax F-719
    - Ergebnisprüfung F-723
    - Bedingungen für Abstellplätze F-724
    - Bedingungen für Orga-Gruppen F-727
    - Modus für Gruppenbildung F-730
    - Bedingungen für Fertigungsabschnitte F-732
    - Weitere Beispiele F-735
    - Übersicht der betroffenen Dialoge F-738
- **Softwarereferenz** F-739
  - Formel-Editor F-741
    - Auswahl Bedingungen F-742
    - Bedingungen - Erzeuger F-744
    - Bedingung F-747
    - Name der Bedingung F-749
    - Info F-750
    - Übergebene Menge F-751
    - Eingabe Zahlenwert F-752
    - Auswahl Mengen F-754
    - Mengen - Erzeuger F-756
    - Name der Menge F-760
    - Info F-762
    - Auswahl Formeln F-763
    - Formel - Editor F-765
    - Auswahl Zuweisung F-768
    - Zuweisung - Editor F-769

### Maschinenzuordnung (G)
- **Tutorial** G-773
  - Überblick G-775
    - Aufbau des Tutorials G-775
  - Grundlagen G-776
  - Maschinenzuordnung G-778
  - Maschinen G-779
    - Maschinen in der Maschinenzuordnung G-780
    - Maschinen anlegen und verwalten G-786
    - Restriktionen von Maschinen anlegen und bearbeiten G-790
    - Übungen zu Maschinen G-796
  - Logische Maschinen G-797
    - Logische Maschinen in der Maschinenzuordnung G-798
    - Logische Maschinen anlegen und verwalten G-800
    - Übungen zu logischen Maschinen G-804
  - Arbeitsgänge G-805
    - Arbeitsgänge in der Maschinenzuordnung G-806
    - Arbeitsgänge anlegen und verwalten G-812
    - Übungen zu Arbeitsgängen G-815
  - Arbeitsgangzuordnung G-816
    - Angepasste Arbeitsgangzuordnung G-817
    - Arbeitsgänge und logische Maschinen zuordnen G-822
    - Übungen zur Arbeitsgangzuordnung G-826
  - Bedingungen, Formeln, Restriktionen G-827
    - Bedingungen und Formeln in der Maschinenzuordnung G-828
    - Übungen zum Auswählen von Bedingungen G-832
  - Bearbeitungstypen und Bearbeitungsartikel G-833
    - Bearbeitungstypen in der Maschinenzuordnung G-834
    - Bearbeitungsartikel in der Maschinenzuordnung G-835
    - Bearbeitungstypen anlegen und verwalten G-837
    - Bearbeitungsartikel anlegen und verwalten G-840
    - Übungen zur Maschinenzuordnung G-844
  - Schaltflächen in der Maschinenzuordnung G-845
- **Softwarereferenz** G-847
  - Maschinenzuordnung G-849
    - MZO-Editor G-850
    - MZO-Editor - Maschinen G-851
    - MZO-Editor - Logische Maschinen G-853
    - MZO-Editor - Arbeitsgänge G-855
    - MZO-Editor - Arbeitsgangzuordnung G-857
    - MZO-Editor - Maschinentypen G-859
    - Neue Maschine G-861
    - Formeln in der Maschinenzuordnung G-881
    - Bearbeitungen in der Maschinenzuordnung G-892
    - Bearbeitungstypen G-893
    - Bearbeitungsartikel G-895
    - Spalten anpassen G-898
    - Spaltendefinition G-899
- **Help Cards** G-901
  - Informationen zu den Help Cards G-903
  - Maschinenzuordnung (MZO) G-904
    - Neue Maschine einfügen G-905
    - Neue Maschine einfügen G-906
    - Neue Maschine für Production Terminal G-907

### Betriebsdatenerfassung (H)
- **Tutorial** H-911
  - Überblick H-914
    - Aufbau des Tutorials H-915
  - Grundgedanken H-916
    - Die Betriebsdatenerfassung H-917
    - Zweck der AWP H-917
    - Buchungselemente H-918
    - Produkte H-919
    - Grundsätzliches H-920
    - Buchungsarten H-921
    - Buchungsorte H-922
    - Erfassungsstellen H-923
    - Abstellplätze H-930
    - Gestelle H-931
    - Kisten H-932
    - Gestelle verwalten H-933
    - Personal H-936
    - Mitarbeiter H-937
    - Mitarbeiter verwalten H-938
    - Status H-940
    - Zustände H-941
    - Zustände verwalten H-943
  - Datenerfassung H-945
    - Scanner H-946
    - Scanner-Typen H-947
    - Konfiguration der Scanner H-948
    - Barcodes H-949
    - Buchungsbeispiele H-950
    - Die Reihenfolge des Scannens H-951
    - Scannen von Einheiten H-953
    - Scannen im Versand H-955
    - Erfassungsstellen scannen H-957
    - Erfassungsstelle LKW H-960
    - Übungen: H-961
    - Gestelle bzw. Kisten scannen H-963
    - Status scannen H-965
    - Korrigieren von Fehlbuchungen H-966
  - Production Terminals H-967
    - Production Terminals H-968
    - Einführung H-969
  - Bruchmanagement H-972
    - Überblick H-973
    - Bruchbehandlung (intern) H-974
  - Statistik, Reporting und Monitoring H-976
    - Überblick H-977
    - BDE-Reporting H-978
    - Monitoring: A+W Dashboard H-983
    - Statistik: A+W Discovery H-987
- **Softwarereferenz** H-991
  - Übersicht H-993
  - Stammdaten H-994
    - Barcode-Optionen H-995
    - Barcode-Typen H-996
    - Erfassungsstellen-Typen H-997
    - Erfassungsstellen H-998
    - Gestelle H-1002
    - Gestellfilter H-1006
    - Zustandstypen H-1007
    - Zustände H-1008
    - Mitarbeiter H-1010
    - Spaltenzuordnung H-1012
    - Spalten H-1013
  - Nachbearbeitung H-1014

### Packmitteloptimierung (I)
- **Tutorial** I-1017
  - Grundgedanke I-1019
    - Allgemeines I-1020
  - Stammdaten I-1023
    - Optimierungsregeln (*.RUL-Datei) I-1023
    - Einstellwerte (*.VAL-Datei) I-1023
  - Anzeigen I-1029
    - Packmittelgruppen-Anzeige I-1029
    - Restriktionen I-1030
  - Optimierung ansehen I-1033
    - Ansichten I-1034
    - Modi I-1043
    - Ungültige Platzierungen I-1051
    - Minimale Dickenunterschiede I-1051
    - Zwischenablage I-1053
- **Softwarereferenz** I-1077
  - Menüs I-1079
  - Regeln I-1081
  - Werte I-1083
  - Packmittelgruppen I-1086
    - Packmittelgruppen-Anzeige I-1089
  - PackView I-1095
    - Menü-Zeile I-1096
    - Symbol-Schaltflächen I-1101
    - Ansichten I-1105
    - Info-Zeile am unteren Bildschirmrand I-1113

### A+W Realtime Optimizer (J)
- **Tutorial** J-1117
  - Grundgedanken J-1120
    - Leistungsmerkmale J-1121
  - Arbeiten mit A+W Production J-1122
    - Überblick J-1123
    - Datenübernahme J-1124
  - Erfassung J-1128
    - Überblick J-1129
    - Bruch, Eilscheiben und Füllaufträge J-1130
    - Scheiben manuell erfassen J-1131
    - Manuelle Planerstellung J-1134
    - Chargen-Editor J-1135
  - Optimierung J-1136
    - Überblick J-1137
    - Tischoptimierungen J-1138
    - Tischansteuerung J-1146
  - Zuschnitt J-1147
    - Überblick J-1148
    - Läufe zum Zuschnitt auswählen J-1149
    - Optimierung prüfen und schneiden J-1152
    - Arbeit unterbrechen und fortsetzen J-1154
    - Die Zuschnitt-Übersicht J-1155
    - Schneidstatus zurücksetzen J-1157
  - Zusammenarbeit mit anderen Modulen J-1158
    - Überblick J-1159
    - A+W Residual Stock Manager J-1159
    - A+W Planning Web J-1159
    - A+W Pattern Viewer J-1168
    - Bruchscheiben J-1182
    - A+W PlanEditor J-1183
    - A+W Continuous Cutting J-1184
    - A+W Defect Optimizer J-1191
    - A+W DynOpt Compact J-1192
- **Softwarereferenz** J-1195
  - Übersicht J-1198
  - Menüs J-1198
  - Symbol-Schaltflächen J-1199
  - Erfassung J-1200
    - Eilscheiben J-1201
    - Manuelle Planerstellung J-1208
    - Chargen-Editor J-1211
  - Optimierung J-1213
    - Selektieren Sie die zu optimierenden Gläser J-1214
    - Tischoptimierung in der Variante Standard J-1214
    - Optimieren J-1222
    - Parameter J-1228
  - Zuschnitt J-1237
    - Wählen Sie einen Lauf aus J-1238
  - Help Cards J-1281
    - Informationen zu den Help Cards J-1283
    - Erfassung J-1284

### A+W Production Terminals (L)
- **Tutorial** L-1305
  - Überblick L-1309
    - Aufbau des Tutorials L-1309
  - Production Terminal Systeme L-1310
    - Ziele der Leitrechner-Technologie L-1312
    - Bedienung der Leitrechner L-1312
  - Überblick Production Terminal IG L-1314
    - Arbeiten mit Production Terminal IG-In L-1315
    - Arbeiten mit Production Terminal IG-Assembly L-1329
    - Arbeiten mit Production Terminal IG-Out L-1336
  - Überblick Production Terminal Manual Cutting L-1344
    - Arbeiten mit Production Terminal Manual Cutting L-1345
  - Überblick Production Terminal Georgian Bars L-1356
    - Arbeiten mit Production Terminal Georgian Bars L-1357
  - Überblick Production Terminal Order L-1364
    - Arbeiten mit Production Terminal Order L-1365
  - Überblick Production Terminal Processing L-1373
    - Arbeiten mit Production Terminal Processing L-1374
  - Überblick Production Terminal TG L-1383
    - Arbeiten mit Production Terminal TG-In L-1384
    - Überblick Production Terminal TG-Out L-1391
    - Arbeiten mit Production Terminal TG-Out L-1392
  - Überblick Production Terminal LG L-1398
    - Arbeiten mit Production Terminal LG-In L-1399
    - Arbeiten mit Production Terminal LG-Assembly L-1405
  - Überblick Production Terminal Edit L-1410
    - Arbeiten mit Production Terminal Edit L-1411
- **Softwarereferenz** L-1419
  - Bedienung der Module L-1422
    - Softwarebegriffe L-1422
    - Programm beenden L-1424
  - Übersicht allgemein L-1425
    - Übersicht Production Terminal IG L-1426
    - Übersicht Production Terminal Manual Cutting L-1445
    - Übersicht Production Terminal Georgian Bars L-1452
    - Übersicht Production Terminal Order L-1455
    - Übersicht Production Terminal Processing L-1456
    - Übersicht Production Terminal TG L-1458
    - Übersicht Production Terminal LG L-1462
    - Übersicht Production Terminal Edit L-1466
    - Reports L-1467
- **Help Cards** L-1475
  - Informationen zu den Help Cards L-1477
  - Terminal IG-IN L-1478
    - Prozessablauf L-1479

### Index (Z)
*(This section is a detailed index and is replaced by the search functionality of the digital document.)*

---
## A. Überblick

### Revisionsübersicht des Moduls

| Datum | Änderung |
| :--- | :--- |
| 02-2017 | Screenshots aktualisiert. |
| 01-2017 | Produkt- und Firmennamen angepasst. |
| 08-2013 | Vollständige Überarbeitung der ALCIM-Dokumentation und Anpassung auf A+W Production. |
| 11-2012 | Überarbeitungen |
| 03-2003 | Ersterstellung |

Zu diesem Modul finden Sie folgende Kapitel:
- Tutorial
- Konventionen

---
## A. Tutorial

### Überblick

Die Zielgruppe der Schulung zum Produkt A+W Production sind ISO-, ESG- oder VSG-Produzenten sowie Bearbeitungs- und Veredelungsunternehmen, welche sich einen Überblick über die Leistungen und die Prozesse in und mit A+W Production verschaffen wollen.

Ziel dieses Systemüberblickes ist es, Ihnen einen grundlegenden Überblick über die Leistungen und Möglichkeiten von A+W Production zu geben. Alle hier beschriebenen Inhalte und Module werden in separaten Schulungen und Tutorials tiefer und ausführlicher behandelt.

Ein gutes Verständnis für die Systemarchitektur und den modularen Aufbau von A+W Production sind die Grundvoraussetzung für die Handhabung und Bedienung der einzelnen Bereiche und den hierfür notwendigen Wissenserwerb.

#### Themenblöcke
In diesem Tutorial finden Sie folgende Themenblöcke:
- A+W Production stellt sich vor
- Basismodul A+W Production
- Ausbaumodule A+W Production

> **Vorausgesetzte Kenntnisse**
> EDV-Grundkenntnisse bzw. Windows-Kenntnisse werden bei den Anwendungen von A+W Production vorausgesetzt.

#### Aufbau des Tutorials
Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

- **Überblick**: Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
    - Lernziele: Was soll vermittelt werden?
    - Nutzen: Wofür können Sie dieses Wissen einsetzen?
    - Merksätze: Welche Zusammenhänge müssen Sie sich merken?
- **Konzepte**: Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.
- **Übungen**: Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen.
- **Querverweise**: Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf ergänzende Informationen in der Softwarereferenz und in anderen Parts hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.

#### Lesehinweis
Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.

Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

### Produktportfolio der A+W Software GmbH
In dieser Abbildung wird A+W Production als Produktionsplanungs- und Steuerungs-System im Anschluss an das ERP-System im gesamten Unternehmensprozess dargestellt.

**Prozessfluss:**
1.  **ERP (Enterprise Resource Planning)**
    - ERP Solution: A+W Enterprise, A+W Business
    - Funktionen: Verkauf, Einkauf, Lager, Versand, Statistik, eCommerce
2.  **PPS (Produktionsplanungs- und Steuerungssystem)**
    - PPS Solution: A+W Production
    - Funktionen: Kapazitätsplanung, Produktionsplanung (Grob- und Feinplanung), Verschnittoptimierung
3.  **Maschinensteuerung**
    - Control Units: Production Terminal, Realtime Optimizer, Rack Optimizer, DynOpt, Monitoring, Controlling, Barcoding
4.  **Maschinen**
    - Beispiele: Zuschnittslinie, ISO Linie, VSG Linie

**Zusätzliche Komponente:**
- **CAD Konstruktion**: A+W CAD Designer (Bars) (Shapes + Bars)

### A+W Production stellt sich vor
Steigende Anforderungen an die Produktion erfordern immer leistungsfähigere Planungs- und Steuerungsapplikationen.

A+W Production ist die Produktions-Planungs- und Steuerungs-Software aus dem Hause A+W Software GmbH. Die modulare Architektur erlaubt die optimale Anpassung an Ihre Anforderungen. Welche der angebotenen Lösungen in welcher Ausbaustufe für Ihr Unternehmen in Frage kommt, wird in Gesprächen mit Ihnen eingehend analysiert.

A+W Production stellt Ihnen eine Vielzahl an modernen Methoden und Werkzeugen zur Verfügung, mit welchen Sie Ihre komplette Produktion planen, steuern, überwachen und auswerten können - von der Einlastung der Auftragsdaten bis hin zur Erzeugung von NC-Code und Buchung von BDE-Daten. Zusätzlich zu diesen standardisierten Prozessen, können Sie direkt und dynamisch in die Produktion eingreifen um bspw. wichtige Eilaufträge einzusteuern oder Engpässe zu beseitigen. So haben Sie stets die volle Kontrolle über alle produktionsrelevanten Ressourcen und Daten - Maschinen, Kosten, Zeiten und Kapazitäten.

Sowohl durch die Vernetzung mit Maschinen und anderen Softwaremodulen aus dem Hause A+W Software GmbH als auch durch die Prozessvisualisierung und -steuerung mittels Production Terminals an den Arbeitsstationen wird ein hohes Maß an Qualität erreicht.

Die Software ist zur Zeit in 12 Sprachen weltweit im Einsatz.

Um die modulare Struktur von A+W Production abbilden zu können, wurde die Software in zwei Kategorien unterteilt:
- **Basissystem**: Umfasst die Bereiche Einlastung, Grobplanung, Feinplanung, Maschinenzuordnung.
- **Ausbaumodule**:
    - Kapazitätsplanung
    - Optimierungssysteme (Realtime Optimizer, Sequence Optimizer, Shape Optimizer, Rack Optimizer, DynOpt, Furnace Optimizer)
    - Barcode Manager
    - Anzeige- und Leitrechnersysteme (Production Terminal)
    - Statistiksysteme (A+W Discovery, Production Cockpit)

#### Prozessablauf mit A+W Production
1.  **Auftragserfassung (ERP)**: Ein Auftrag wird erfasst und geprüft.
2.  **Auftragsanalyse**: Nach erfolgreicher Prüfung gelangen die Daten in die Produktionsplanung.
3.  **Produktions-Planung (A+W Production)**:
    - **Auftrags-Pool**: Aufträge werden gesammelt.
    - **Grobgeplante Läufe**: Aufträge werden zu Läufen gruppiert.
    - **Feingeplante Läufe**: Nach Qualitätskontrolle werden die Läufe feingeplant.
    - **Job Release**: Die Läufe werden zur Produktion freigegeben.
4.  **Produktionsausführung**:
    - **Zuschnitt**: Gesteuert durch den *Realtime Optimizer*.
    - **Glas-Bearbeitung (ESG/VSG, ISO)**: Gesteuert durch *Production Terminals*.
    - **Versand**: Verwaltet durch den *Barcode Manager*.
5.  **Monitoring**: Der gesamte Prozess wird über die Datenbank von *A+W Discovery* überwacht.

### Basismodul A+W Production
In diesem Themenblock lernen Sie, wie Sie mit dem Basismodul arbeiten. Der Themenblock beinhaltet folgende Schulungseinheiten:
- Einlastung
- Grobplanung
- Feinplanung
- Maschinenzuordnung

#### Einlastung
In diesem Themenblock lernen Sie die Funktionsweise des Einlastungsprozesses von A+W Production kennen.

**Lernziele:**
- Die Arbeitsweise der Einlastung kennenlernen
- Über beteiligte Module, Prozesse und Abläufe informiert sein.

**Definitionen:**
- **Items4ALCIM**: Modulname des Einlastungsdienstes. Wird als Begriff häufig synonym verwendet.

> **Merke: Dienst**
> Die Einlastung ist ein Windows-Dienst und kann aktiv und interaktiv laufen. Aktiv wird er durch den Benutzer gesteuert oder interaktiv läuft er als Hintergrundprozess. Es ist möglich, mehrere Einlastungsprozesse parallel laufen zu lassen.

**Einlastung allgemein**
Mittels des Einlastungsprozesses (Windowsdienst) werden die Auftragsdaten aus dem ERP-System aktiv in die Produktionsdatenbank geschrieben. Die Daten können auf zwei Wegen zwischen den Systemen übertragen werden:
- **Direkter Datenimport**: Durch direkten Zugriff auf eine A+W Enterprise-Datenbank.
- **Mittels einer XML-basierten Standard-Schnittstelle** (z. B. aus A+W Business).

Im Verlauf der Einlastung werden folgende Prozessschritte je Auftragsposition ausgeführt:
1.  Was? - Stammdaten
2.  Wo? - Maschinenzuordnung
3.  Wie lange? - Kapazitätsplanung
4.  Wann? - Kapazitätsplanung
5.  Erstellung der SN-Dateien
6.  Füllen der sogenannten "Pool_"-Tabellen
7.  Laden und Ausführen von Kundenanpassungen
8.  Geometrieberechnung
9.  BDE-Initialisierung
10. Rückmeldung ERP-System (über WebService)

Nach dem Einlesen der letzten Position werden die Auftragsdaten gespeichert. Die eingelesenen Aufträge finden Sie nun in der sogenannten **Pool-Anzeige** (erster Schritt im Prozess der Grobplanung).

#### Grobplanung
In diesem Themenblock lernen Sie die Grobplanung von A+W Production kennen.

**Lernziele:**
- Die unterschiedlichen Anzeigen kennenlernen

**Nutzen:**
Ziel und Nutzen der Grobplanung im Rahmen der Arbeitsvorbereitung verstehen. Nur wenn Sie die Arbeitsweise der Grobplanung kennen und verstehen, können Sie Läufe effizient bilden und verwalten.

**Definitionen:**
- **Grobplanung**: Der Prozess der Grobplanung und die dazu zur Verfügung gestellten Anzeigen und Werkzeuge dienen einer effizienten Auftragsvorbereitung (Laufplanung und -verwaltung).
- **Pool**: Nach dem Einlasten der Aufträge, finden Sie diese in der sog. Pool-Anzeige. Diese zeigt alle unverplanten Produkte und Zwischenprodukte.
- **Topf**: Sie können vor der Laufbildung Produkte bzw. einzelne Positionen zusammenfassen, um sich einen generellen Überblick der Mengen zu verschaffen.
- **Lauf**: Läufe sind das Ergebnis der Grobplanung. Sie können zur Produktion freigegeben oder auch wieder aufgelöst werden.
- **Freigabeteil**: Unter Freigabeteilen sind explizit für die Produktion zu planende Teile zu verstehen.
- **Stückliste**: Listet alle Komponenten hierarchisch und beschreibt exakt deren Abhängigkeiten.
- **Bearbeitung**: Arbeitsschritte an einem Glas/Produkt, z. B. Zuschnitt, Härten, Versand.

**Grobplanung allgemein**
Die Grobplanung ist ein Prozess, in welchem Sie sich einen Gesamtüberblick über die zu produzierenden Aufträge verschaffen und sie dann in geeignete Läufe zur Produktion einteilen. Dies geschieht durch verschieden konfigurierbare Anzeigen.

**Übersicht der Anzeigen:**
- **Pool-Anzeige**: Zeigt alle unverplanten Aufträge.
- **Topf-Anzeige**: Zeigt alle vorgruppierten Aufträge.
- **Lauf-Anzeige**: Zeigt alle grobgeplanten Aufträge.
- **Detail-Anzeige**: Zeigt alle Freigabeteile und deren besondere Merkmale.
- **Glasarten-Anzeige**: Zeigt alle Teile inklusive Basisgläser.
- **Positions-Anzeige**: Zeigt die Stücklistenstruktur.
- **Bearbeitungs-Anzeige**: Zeigt alle Teile und deren Bearbeitungen.
- **Füllauftrag-Anzeige**: Zeigt alle Freigabeteile, die als Füllaufträge markiert sind.
- **Auftragsübersicht**: Zeigt die komplette Stücklistenstruktur.
- **BDE-Anzeige**: Zeigt Status und Historie.
- **Produktionslos-Anzeige**: Zeigt Ergebnisdaten der Feinplanung.

**Die Auftrags-Anzeige (Pool)**
Nach dem Import der Auftragsdaten werden alle fehlerfrei übernommenen Daten in einen Pool gestellt. Die Auftrags-Anzeige stellt den unverplanten Auftragsbestand dar.

**Die Auftragsübersicht**
In dieser Anzeige bekommen Sie eine übersichtliche Gliederung und Darstellung der kompletten Stücklistenstruktur.

**Die Topf-Anzeige**
Aufträge, Produkte und Zwischenprodukte können zu Töpfen zusammengefasst werden. Töpfe dienen als Hilfsmittel zur Voreinteilung.

**Die Positions-Anzeige**
In dieser Ansicht werden die Auftragsdaten für eine Auswahl angezeigt.

**Die Glasarten-Anzeige**
In der Glasarten-Anzeige werden die Bestandteile der Produkte dargestellt, was besonders für die Zusammenstellung von Läufen für den Zuschnitt nützlich ist.

**Die Detail-Anzeige**
Entspricht der Auftrags-Anzeige, arbeitet aber mit einer beliebig selektierten Menge.

**Die Bearbeitungs-Anzeige**
Gibt einen Überblick über die Teile und deren Bearbeitung.

**Die Füllauftrag-Anzeige**
Zeigt nur Aufträge, die zuvor als Füllaufträge gekennzeichnet wurden.

**Die Lauf-Anzeige**
Gibt einen Überblick über die vorhandenen Läufe und deren Status.

**Läufe bilden**
Läufe können aus folgenden Anzeigen heraus gebildet werden:
- Auftrags-Anzeige
- Topf-Anzeige
- Füllauftrag-Anzeige
- Detail-Anzeige
- Bearbeitungs-Anzeige
- Glasarten-Anzeige

**Bildung von Läufen**
Der Planungsprozess erfolgt in Stufen: Erst Trennung nach Hauptkriterien, dann Überprüfung und Aufteilung in verschiedene Läufe. Kriterien können sein:
- Nach Glasart
- Nach Produktart
- Nach Bearbeitung
- Nach Produktionsdatum
- Nach Auftrag oder Position

**Allgemeine Regeln**
Ein Lauf sollte eine angemessene Größe haben (ca. 2 Arbeitsstunden). Spezialprodukte sollten mit Standardläufen gemischt werden. Eine gute Strategie zur Laufbildung ist eine, die für den Betrieb funktioniert.

#### Feinplanung
In diesem Themenblock lernen Sie die Feinplanung kennen.

**Lernziele:**
- Ziele und Rahmenbedingungen der Feinplanung kennenlernen
- Unterschiedliche Optimierungsmodi kennenlernen
- Unterschiedliche Organisationsformen kennenlernen

**Definitionen:**
- **Gruppierung**: Erfolgt nach eindeutigen Werten (z. B. Kundennummer).
- **Sortierung**: Erfolgt nach fortlaufenden Werten (z. B. Glasdicke).
- **Physikalischer Abstellplatz**: Gestell (A-Bock, L-Bock).
- **Logischer Abstellplatz**: Mehrere Glasstapel auf einem physikalischen Abstellplatz.
- **Orga**: Abbildung der Produktion in Sequenz und Laufwegen.

**Feinplanung allgemein**
Die Feinplanung ist der zweite Schritt der Arbeitsvorbereitung. Ihre Aufgabe ist es, für die in den Läufen enthaltenen Teile die Produktionsreihenfolge zu erstellen und die Abstellplätze zu definieren. Die Produktionsreihenfolge kann sich durch Kundenvorgaben, Ergebnisse der Gestelloptimierung oder fertigungstechnische Restriktionen ergeben.

> **Optimierungsergebnis**
> Die Optimierung mit dem geringsten Verschnitt muss nicht immer oberstes Ziel sein, wenn z.B. der Sortierungsaufwand unverhältnismäßig hoch wird.

**Ablauf der Feinplanung**
1.  Daten werden aus der Datenbank geladen.
2.  Feinplanung weist Teile den verfügbaren Orgas und Abstellplatztypen zu.
3.  Gruppierungen und Sortierungen innerhalb der Orga-Gruppen und auf den Abstellplätzen erfolgen.
4.  Abstellen der Scheiben auf den Abstellplätzen wird behandelt.
Im Spannungsfeld von Verschnitt, Reihenfolge und Flexibilität wird die Produktion justiert.

**Gruppierungen und Sortierungen**
Dienen dazu, den Abstellplätzen die gewünschte Produktionsreihenfolge zuzuweisen. Die Optimierung berechnet den bestmöglichen Verschnitt unter Einhaltung der definierten Produktionssequenz.

**Abstellplatz- und Stapellogik**
In der Feinplanung gibt es verschiedene Kriterien, um Scheiben auf Abstellplätze zu stellen. Dies verbessert Durchlaufzeiten und vermeidet unnötiges Umsortieren. A+W Production bietet verschiedene Standardorganisationen an:
- Für A-Böcke
- Für Fächerwagen
- Für Einheiten (ISO, VSG)
- Für mehrstufige Produktionsformen
- Für Los-basierte Produktionsformen

**Abstellmodi für A-Böcke:**
- **Glas**: Eine Glasart pro Abstellplatz.
- **Einheit**: Jede Einheit auf einem logischen Abstellplatz.
- **Produktion**: Verschiedene Glasarten auf einem logischen Abstellplatz kombinierbar.
- **VABGLA**: Pro Glasart ein logischer Abstellplatz mit einem Stapel.

**Abstellmodi für Fächerwagen:**
- **Zusammen**: Scheibe und Gegenscheibe(n) immer zusammen.
- **Glas**: Scheiben immer getrennt.

#### Optimierungs-Modi
Bei der Wahl der Optimierung muss ein Kompromiss zwischen bestem Ergebnis (geringer Verschnitt) und bester Produktionsreihenfolge gefunden werden.

**Verfügbare Modi:**
- **XOPTS 6.2 - Feste Reihenfolge**: Strikte Reihenfolge der Gruppen und der Gläser innerhalb der Gruppen.
- **XOPTS 6.1 - Kunden zusammenhalten**: Reihenfolge der Gläser innerhalb der Gruppen fest, Gruppen können aber umsortiert werden.
- **XOPTS 5.2 - Standard**: Standard-Modus. Teile innerhalb der Gruppen können frei optimiert werden.
- **XOPTS 5.1 - ISO auf Fächerwagen oder viele A-Böcke**: Freie Optimierung, nur Einheiten (z.B. ISO) werden zusammengehalten.
- **XOPT**: Standardoptimierung für Scheiben auf Fächerwagen.

#### Organisationsformen (Orgas)
Eine Orga ist ein datentechnisches Regelwerk zur Abbildung der Produktion. Sie organisieren die Abstellplätze vor den Produktionsschritten (ISO-Linie, Ofen etc.).

**Orga-Typ und Los-Typ**
Jedes Teil hat einen Teiletyp und eine Beschaffungsart. Abhängig davon wird es einem Lostyp zugewiesen. Jede Orga hat einen Orga-Typ, der festlegt, welche Teile ihr zugewiesen werden. Produktionslose werden für unterschiedliche Teiletypen und Glasarten im Zuschnitt gebildet.

#### Maschinenzuordnung
Hier wird der physikalische Maschinenpark abgebildet und bildet die Basis zur Steuerung der Produktion.

**Definitionen:**
- **Maschinen**: Bilden physikalische Maschinen ab.
- **Logische Maschine**: Datentechnische Beschreibung eines Teils einer Maschine oder eines Betriebszustandes (z.B. Ofen für Härten vs. Vorspannen).
- **Maschinentypen**: Definieren den technischen Typ einer Maschine (z.B. Zuschnitt).
- **Arbeitsgänge**: Verbinden Bearbeitungstyp-Eigenschaften mit Werkstück-Eigenschaften.
- **Bearbeitungstypen**: Beschreiben die technische Form einer Bearbeitung (z.B. Zuschnitt).
- **Bearbeitungsartikel**: Detaillieren einen Bearbeitungstyp (z.B. Facetten-Schliff für den Typ Schleifen).

> **Merke: Arbeitsgangzuordnung**
> Verbindet logische Maschinen mit Arbeitsgängen und ermöglicht dem Anwender, in den Produktionsprozess einzugreifen.

> **Merke: Prioritäten**
> Mit der Arbeitsgangzuordnung werden Prioritäten der logischen Maschinen festgelegt, um sicherzustellen, dass Arbeitsgänge auf der optimalen und kostengünstigsten Maschine durchgeführt werden.

**Bestandteile der Maschinenzuordnung**
Maschinen werden durch Maschinentyp, Eigenschaften und Restriktionen definiert. Logische Maschinen, Arbeitsgänge, Bearbeitungstypen und -artikel werden zugeordnet, um den Produktionsfluss und Maschinencode zu steuern.

### Ausbaumodule A+W Production
In diesem Themenblock lernen Sie die Ausbau- und Zusatzmodule von A+W Production kennen.
- Kapazitätsplanung
- Optimierungssysteme
- Barcode Manager
- Anzeige- und Leitrechnersysteme
- Statistiksysteme

#### Kapazitätsplanung
Mit der Kapazitätsplanung können Sie schnell Auskunft über Produktionsmöglichkeiten, Auslastung und Kosten geben.

**Definitionen:**
- **Übergangszeiten**: Ruhephasen für das Glas zwischen Arbeitsgängen (z.B. Autoklavprozess).
- **Kapazität**: Zeitspanne, in der eine Maschine verfügbar ist (z.B. 1 Schicht = 8 Stunden).
- **Auslastung**: Zeitspanne, in der Arbeit auf die Maschine eingelastet ist.
- **Reservierung**: Zeitspanne, die für besondere Aufträge reserviert ist.
- **Kampagne**: Zeitspanne, in der eine Maschine nur einen bestimmten Arbeitsgang ausführt.
- **Maschine**: Physikalische Maschine, definiert in der Maschinenzuordnung.

**A+W Capacity Planner**
Dient zur Verplanung der vorhandenen Produktionskapazitäten. Er ermöglicht ein frühzeitiges Erkennen von Engpässen und eine Überprüfung von Lieferterminen und Kosten. Das System unterscheidet zwischen Normal- und Eilraster.

**Produktionsmonitor**
Bietet eine detaillierte Kapazitätsübersicht. Daten können direkt bearbeitet werden, um z.B. Schichten zu sperren oder Engpässe umzulasten. Grafische Symbole zeigen:
- Arbeitsrückstand (rot/gelb/grün)
- Schicht (grauer Balken)
- Arbeitsauslastung (grüner Balken)
- Überlast (%-Angabe)
- Arbeitsfortschritt (blauer Balken)
- Reservierungen (schraffierter Bereich)

**Kampagneneditor**
Hier können ausgewählte Arbeitsgänge an genau festgelegten Terminen eingeplant werden.

**Schichteditor**
Hier können Schichten angelegt und konfiguriert werden, was für die Kapazitätsplanung unerlässlich ist.

**Grafisch-orientierte Terminumlastung**
Mit dem Umlastungseditor können einzelne oder Gruppen von Bearbeitungen auf alternative Maschinen und Schichten umgelastet werden.

#### Optimierungssysteme
Diese Systeme haben die Aufgabe, Prozesse und Verschnitt bestmöglich zu optimieren.

- **A+W Realtime Optimizer**: Online-Zuschnitt-Leitrechner für dynamische Eingriffe in Fertigungsläufe. Erlaubt Nach-Optimierung von Eil-, Bruch- oder Füllscheiben.
- **A+W Sequence Optimizer**: Optimiert den Verschnitt einzelner Glasarten unter Berücksichtigung der Sortierreihenfolge.
- **A+W Shape Optimizer**: Legt Modelle flächensparend innerhalb eines Rechtecks zusammen.
- **A+W Rack Optimizer**: Ermöglicht die Direktverpackung auf Versandgestelle und optimiert die Scheiben auf den Gestellen.
- **A+W DynOpt**: Dynamisches Optimierungs- und Zuschnittkontrollsystem, das bei Einhaltung von Fertigungssequenzen den höchsten Ertrag erzielt.
- **A+W Furnace Optimizer**: Ermittelt die optimale Belegung des Ofenbetts.

#### Barcode Manager
Bietet die Möglichkeit einer scheiben- und chargengenauen Nachverfolgung aller Teile. Das System ist ein wichtiges Planungs-, Steuerungs- und Controllinginstrument.

**Allgemein**
Erfasst den Produktionsfluss an Erfassungsstellen mittels Barcodes, Scannern, etc.

**Scanner**
- **Online-Scanner**: Übertragen Daten direkt, ohne eigenen Speicher (z.B. serielle Scanner).
- **Offline-Scanner**: Verfügen über einen Speicher und übertragen Daten bei Verbindung (z.B. Denso-Scanner).

#### Anzeige- und Leitrechnersysteme
Diese Systeme visualisieren Produktionsdaten und steuern den Produktionsprozess an den Arbeitsstationen.

- **A+W Production Terminals**: Leitrechnersysteme zur Anzeige und Steuerung des Arbeitsvorrates.
- **A+W Production Cockpit**: Online-Monitoring und Controlling-System, das aktuelle Produktionsdaten visualisiert.

**Production Terminal Varianten:**
- **Manual Cutting**: Visualisiert den Arbeitsplan am Handzuschnitttisch.
- **Order**: Für auftrags- oder laufbasierte Bearbeitung von einem zentralen Punkt aus.
- **Processing**: An Bearbeitungsmaschinen, steuert diese automatisch an.
- **IG-In**: Visualisiert den Arbeitsvorrat am Einlauf der Isolierglaslinie.
- **IG-Assembly**: Zwischen Waschmaschine und Rahmensetzstation, visualisiert technische Daten.
- **IG-Out**: Am Auslauf der Isolierglaslinie, visualisiert versandorientierte Daten.
- **TG-In**: Anzeigesystem am Ofeneinlauf, zur interaktiven Belegung des Ofenbettes.
- **TG-Out**: Anzeigesystem am Ofenauslauf.

**Ziel der Production Terminals**
- Geplante Jobs auf Arbeitsplätze verteilen.
- Durchgeführte Arbeiten buchen.
- Abweichungen erfassen.
- Produktionsfortschritt anzeigen.
- Nachläufer automatisch generieren.

#### Statistiksysteme
Diese Systeme bereiten umfangreiche, heterogene Daten optisch auf.

- **A+W Discovery**: Modernes Business Intelligence System, das Daten aus multiplen Quellen integriert und in Microsoft Excel (ab Version 2010) darstellt.
- **A+W Production Cockpit**: Online Produktionsbenchmarking, das Nutzungsgrad, Status, Produktivität und weitere Kennzahlen von Maschinen in Echtzeit anzeigt.

---
## Konventionen

### Bedienoberfläche
Dieses Kapitel gibt einen Überblick über die Bedienelemente, die Sie in der Software finden.

#### Dialoge
- **Register**: Teilen den Dialog zur besseren Übersicht nach Themen auf.
- **Schnelltaste/Hot-Key**: Die meisten Funktionen können über Tastenkombinationen (<Alt> + unterstrichener Buchstabe) ausgelöst werden.
- **Optionsschalter (Radio button)**: Erlauben nur eine Auswahl aus einer Gruppe von Optionen.
- **Kombobox**: Bietet eine Drop-down-Liste von Optionen zur Auswahl.
- **Checkbox**: Bietet Optionen, die getrennt voneinander aktiviert/deaktiviert werden können.
- **Feld**: Eingabefeld für Daten.
- **Titelleiste**: Zeigt den Namen des Dialogs.
- **Menüleiste/Menüpunkt**: Bietet Zugang zu verschiedenen Funktionen.
- **Symbolleiste**: Bietet schnellen Zugriff auf häufig verwendete Funktionen.

#### Schaltflächen
- **[...]**: Öffnet einen zugehörigen Dialog.
- **Abbrechen**: Schließt den Dialog ohne zu speichern.
- **Ändern**: Bearbeitet einen markierten Datensatz.
- **Aktualisieren**: Lädt den Inhalt des Dialogs neu.
- **BDE-Anzeige**: Öffnet den Dialog BDE-Anzeige.
- **Datenübernahme**: Startet die Datenübernahme in A+W Production.
- **Drucken**: Öffnet den Druckdialog.
- **Einfügen**: Fügt einen kopierten Datensatz ein.
- **Filtern**: Erstellt einen neuen Filter für die Anzeige.
- **Kopieren**: Kopiert einen markierten Datensatz in die Zwischenablage.
- **Lauf-Anzeige**: Öffnet den Dialog Lauf-Anzeige.
- **Löschen**: Löscht den markierten Datensatz.
- **Manuelle Nachbearbeitung**: Öffnet den Dialog für manuelle Nachbearbeitung.
- **Neu**: Erfasst einen neuen Datensatz.
- **OK**: Übernimmt alle Eingaben, speichert Änderungen und schließt den Dialog.
- **Hilfe**: Öffnet das Online-Hilfesystem.
- **Packmittelgruppen-Anzeige**: Öffnet den Dialog Packmittelgruppen-Anzeige.
- **Pool-Anzeige**: Öffnet den Dialog Pool-Anzeige.
- **Schließen**: Schließt den Dialog.
- **Speichern**: Übernimmt Eingaben in die Datenbank.
- **Suchen**: Öffnet den Suchdialog.
- **Topf-Anzeige**: Öffnet den Dialog Topf-Anzeige.
- **Verwerfen**: Verwirft alle Änderungen.

### Dokumentation
Dieses Kapitel gibt Informationen zur Gesamtdokumentation für A+W Production.

#### Aufbau des Handbuchs
Die Dokumentation ist in Parts unterteilt (A-Z).
- **Part A Überblick**: Allgemeine Erläuterungen, Softwarebegriffe.
- **Part C Grobplanung**: Einstellungen und Durchführung der Grobplanung.
- **Part D Feinplanung**: Einstellungen und Funktionsprinzip der Feinplanung.
- **Part E Kapazitätsplanung**: Funktionsweise und Einstellungen der Kapazitätsplanung.
- **Part F Formeleditor**: Erstellung von Bedingungen zur Eigenschaftstrennung.
- **Part G Maschinenzuordnung**: Funktionsweise und Einstellungen der Maschinenzuordnung.
- **Part H Betriebsdatenerfassung**: Grundlagen zur Betriebsdatenerfassung (BDE).
- **Part I Packmitteloptimierung**: Funktionsweise und Einstellungen der Packmitteloptimierung.
- **Part J A+W Realtime Optimizer**: Nutzung des Einsparpotentials beim Zuschnitt.
- **Part L A+W Production Terminals**: Nutzung der Leitrechner-Technologie.

#### Online-Hilfe
Die Online-Hilfe kann auf unterschiedliche Weise geöffnet werden:
- Menü *Hilfe*
- Schaltfläche `[Hilfe]`
- Taste `<F1>`

Die Hilfe ist zu den meisten Dialogen kontext-sensitiv.

**Hilfethemen**
- **Register Inhalt**: Zeigt Module und Kataloge in einer Baumstruktur an.
- **Register Index**: Ermöglicht die Suche nach Hauptthemen.
- **Register Suchen**: Ermöglicht eine Volltextsuche.
- **Hilfetext nicht gefunden**: Wenn kein spezifisches Thema verfügbar ist, wird die Startseite der Hilfe angezeigt.
