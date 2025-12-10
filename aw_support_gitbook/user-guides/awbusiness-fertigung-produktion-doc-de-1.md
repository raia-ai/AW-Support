---
description: "DE_AWBusiness_Fertigung_5_1"
---


# A+W Fertigung

**A+W Business**

A+W - Software for Glass, Windows and Doors

---

---
## Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version/Datum | Beschreibung                                                                                                                                                                                            |
| :----------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1.00/03-1998       | Ersterstellung.                                                                                                                                                                                         |
| 2.00/08-2000       | Überarbeitung Fertigung.                                                                                                                                                                                |
| 3.00/12-2003       | Struktureller Umbau auf Programmstruktur 4.0.                                                                                                                                                           |
| 3.01/08-2008       | Rechtschreibkorrekturen.                                                                                                                                                                                |
| 3.02/09-2008       | Abbildungen und Part-Nummer angepasst.                                                                                                                                                                  |
| 4.00/04-2011       | Vollständige Überarbeitung und Umstellung auf Doku-Konzept 2010.                                                                                                                                          |
| 4.01/01-2012       | Korrektur Angebotsübergabe an Produktion.                                                                                                                                                               |
| 5.00/07-2013       | Überarbeitung der ALFAK-Dokumentation und Anpassung auf A+W Business.                                                                                                                                     |
| 5.01/01-2017       | Produkt- und Firmennamen angepasst.                                                                                                                                                                     |
| 5.10/07-2017       | Strukturelle Überarbeitung. Dialog Versanddaten ändern neu (ersetzt Dialog Touren/Liefertermine umsetzen), Dialog Gestellbelegung neu, Dialog Terminübersicht aktualisiert.                                |
| 5.11/01-2018       | Kapitel Gestellverwaltung – Historie korrigiert.                                                                                                                                                        |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen
- Kontakte

**Anmerkungen zu diesem Dokument**

Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Business gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Dieses Dokument beschreibt die volle Ausbaustufe von A+W Business.

**Urheberrechte**

© 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß des Lizenzvertrages ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung von A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

**Warenzeichen**

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

**Kontakte**

A+W Software GmbH
Am Pfahlgraben 4-10
D-35415 Pohlheim
📞 +49 6404 2051-0
📠 +49 6404 2051-877
📧 aw.zentrale@a-w.com
🌐 http://www.a-w.com

---

## Inhalt

- **Vorspann** E-3
    - Revisionsübersicht E-3
    - Editorial E-3
- **Tutorial** E-11
    - Überblick E-13
        - Dokumentation E-14
        - Aufbau des Tutorials E-14
        - Darstellungskonventionen E-15
        - Menü-Übersicht E-16
    - Grundgedanken zu Fertigung und Versand E-18
    - Produktionsübergabe E-20
        - Varianten der Produktionsübergabe E-21
        - Schematische Abläufe der Varianten E-23
        - Schematischer Ablauf ohne Kapazitätsplanung E-23
        - Schematischer Ablauf mit Kapazitätsplanung E-24
        - Schematischer Ablauf mit Bestellung und Positionsänderung E-25
        - Änderung von übergebenen Positionen E-26
        - Übergabe von Aufträgen mit Bestellungen E-26
        - Produktionsübergabe per Workflow-Task E-26
        - Produktionsübergabe ohne Kapazitätsplanung E-29
        - Produktionsübergabe einrichten E-31
        - Auftragsdaten an die Produktion übergeben E-37
        - Produktionsübergabe stornieren E-39
        - Übungen E-42
    - Produktionsübergabe mit A+W Business Kapazitätsplanung E-43
        - Einstellungen in den Firmendaten E-44
    - Produktionsübergabe mit A+W Production Capacity Planner E-47
        - Einstellungen für A+W Production Capacity Planner E-48
    - Übergabe zur Angebotsoptimierung E-52
        - Optimierung von Angeboten E-53
        - Angebotsübergabe einrichten E-54
        - Angebote an die Produktion übergeben E-55
        - Übungen E-57
    - Rückmeldungen aus der Produktion E-58
        - Produktionsrückmeldungen per Datei E-59
        - Rückmeldedateien E-60
        - Erfassungsstellen für Produktionsrückmeldungen E-62
        - Erfassungsstelle zuordnen E-63
        - Einstellungen in den Firmendaten festlegen E-65
        - Einstellungen für Schnittstellen festlegen E-66
        - Status der Positionen und Aufträge prüfen E-69
        - Dateilose Produktionsrückmeldung E-70
        - Erfassungsstellen für dateilose Rückmeldungen prüfen E-71
        - Einstellungen in den Firmendaten festlegen E-73
        - Dateilose Rückmeldung und online-Produktionsübersicht E-75
        - Übermengen E-78
        - Dateilose Rückmeldungen und Kapazitätsplanung E-78
    - A+W Business Interface Service E-79
        - Einstellungen für den A+W Business Interface Service festlegen E-80
    - Lieferwesen E-81
        - Tourenplanung E-82
        - Definierte Touren E-83
        - Neue Tour definieren E-84
        - Sperrkennzeichen E-86
        - Tour planen E-87
        - Versanddaten ändern E-89
        - Tourenliste drucken E-91
        - Übungen E-93
    - Statusmeldung E-94
        - Auftragsstatus E-95
        - Statusverwaltung und -zuordnung prüfen E-95
        - Manuelle Statusumsetzung E-97
        - Einstellungen für manuelle Statusmeldungen E-98
        - Status manuell umsetzen E-99
        - Scan-Vorlage herstellen E-103
        - Übungen E-104
    - Kommissionierung E-105
        - Organisation der Auslieferung E-106
        - Fahrzeug anlegen E-107
        - Fahrerdaten anlegen E-108
        - Fahrzeugbeladung zusammenstellen E-109
        - Listendruck für den Fahrer E-113
        - Listen drucken E-113
        - Übungen E-115
    - Übersichten E-116
        - Terminübersicht E-117
        - Materialbedarf pro Zeitraum E-118
        - Terminübersicht erstellen E-121
        - Übungen E-124
    - Kapazitätsübersicht E-125
        - Kapazitätsvorschau E-126
        - Kapazitätsvorschau zu einem Liefertermin erstellen E-126
        - Übungen E-128
    - Zusatzfunktionen E-129
        - Produktionsaufträge E-130
        - Lagerartikel im Produktionsauftrag E-131
        - Rückmeldung zu Produktionsaufträgen E-132
        - Einstellungen in den Firmendaten festlegen E-133
        - Produktionsauftrag fertigmelden E-134
        - Übungen E-138
    - Frachtkosten E-139
        - Berechnungen E-140
        - Einstellungen zur Berechnung von kalkulatorischen Frachtkosten E-141
        - Darstellung der kalkulatorischen Frachtkosten E-143
        - Speditionskosten verteilen E-145
        - Übungen E-147
    - Warenausgang Kisten E-148
        - Kistenausbuchung E-149
        - Kiste ausbuchen E-150
        - Übungen E-158
    - Gestellverwaltung E-159
    - Fertigungsvorschau E-161
- **Softwarereferenz** E-165
    - Übersicht E-167
    - Produktion E-169
        - Übergabe Produktion E-170
        - Einstellungen Produktionsübergabe E-174
        - Einstellungen Produktionsübergabe - Schnittstelle E-175
        - Einstellungen Produktionsübergabe - Übergabe Parameter E-177
        - Einstellungen Produktionsübergabe - Zusätzliche Schnittstellen E-184
        - Einstellungen Produktionsübergabe - Texte/Anlagen E-186
    - Modellliste E-187
    - Gestellbelegung prüfen E-188
        - Einstellungen (Gestellbelegung prüfen) E-190
        - Einstellungen - Gemeinsam E-191
        - Einstellungen – Kunden E-192
    - Barcode-Übergabe E-193
        - Menü Funktionen E-193
        - Übergabe Barcode Produktion E-194
        - Übergabe Barcode Produktion – Übersicht E-194
        - Übergabe Barcode Produktion - Details E-195
    - Produktionsdaten E-198
        - Produktionsdaten (Dialog) E-198
        - Produktionsdaten - Auftrag E-199
        - Produktionsdaten - Tabelle E-201
        - Produktionsdaten - Buchung E-202
    - Lieferwesen E-203
    - Tourenliste E-204
        - Menüs im Dialog Tourenliste E-204
        - Menü Funktionen E-204
        - Menü Optionen E-205
        - Tourenliste E-206
        - Tourenliste - Selektion E-207
        - Tourenliste - Tabelle E-210
        - Versanddaten ändern E-214
        - Einstellungen (KAPS-Datei) E-215
    - Statusmeldung E-216
        - Menüs im Dialog Statusmeldung E-216
        - Menü Funktionen E-216
        - Menü Optionen E-217
        - Statusmeldung und Packmittelzuordnung E-218
        - Statusmeldung - Auftrag E-218
        - Statusmeldung - Position E-220
        - Statusmeldung - Manuelle Packmittelzuordnung E-222
        - Optionen in Statusmeldung E-223
        - Auswahl Gestell E-224
    - Kommissionierung E-226
        - Menüs im Dialog Kommissionierung E-226
        - Menü Funktionen E-226
        - Menü Optionen E-227
        - Kommissionierung E-228
        - Gestelltransfer E-231
        - Export Optionen E-232
        - Listendruck E-233
        - Gestellausgabe E-236
    - Warenausgang Kisten E-237
        - Warenausgang E-237
    - Gestelle E-238
        - Menüs im Dialog Gestelle E-238
        - Menü Optionen E-238
        - Menü Funktionen E-239
        - Gestelle E-240
        - Gestellverwaltung - Gestelle E-241
        - Gestellverwaltung - Ausgang E-244
        - Gestellverwaltung - Eingang E-247
        - Gestellverwaltung - Historie E-248
        - Gestellverwaltung - Mahnung E-250
    - Gestellverwaltung E-253
        - Gestellarten E-254
        - Gestellübersicht E-256
        - Übersicht Partner E-257
        - Gestell umbuchen E-258
        - Mahnstatus zurücksetzen E-259
    - Gestellbelegung E-259
        - Gestellbelegung - Nach Auftrag E-260
        - Gestellbelegung - Nach Gestell E-262
    - Kundenkommissionen E-264
        - Kundenkommissionen - Kommission E-264
        - Kundenkommissionen - Abladestelle E-265
        - Kundenkommissionen – Zuordnung E-266
    - Terminübersicht E-267
        - Menüs in der Terminübersicht E-267
        - Menü Funktionen E-267
        - Menü Optionen E-268
        - Terminübersicht (Dialog) E-268
        - Terminübersicht - Auswahl E-269
        - Terminübersicht - Tabelle E-274
        - Exportieren E-275
    - Kapazitätsübersicht E-276
    - Fertigungsvorschau E-278
        - Menü Optionen E-278
        - Fertigungsvorschau (Dialog) E-279
        - Definition Vorschauspalten E-280
        - GA-Ausschluss bei Fertigungsvorschau E-281
    - Zollverwaltung E-282
        - Zollverwaltungsliste E-282
        - Ladeliste - Nummernverwalter E-283
        - Ladeliste - Zollverwaltungslisten E-285
        - Listennummer zurücksetzen E-286
        - Produktgruppe mit Positionsmenge E-286
    - Zoll-Export E-287
        - Menü Funktionen E-287
        - Zoll-Export (Dialog) E-287
        - Export Artikelstammdaten E-289
    - Angebotsoptimierung E-290
    - Versandsteuerung E-290
        - Versand (Spedition) E-290
        - Menü Funktionen E-291
        - Versandsteuerung - Sammeln E-292
        - Versandsteuerung - Versandinfo E-294
        - Versandsteuerung - Verpackung + Transport E-295
        - Versandaufträge löschen E-297
    - Gestell-Packliste E-298
        - Menü Funktionen E-298
        - Gestell-Packliste (Dialog) E-298
    - Teillieferung E-299
    - Ladelisten E-301
        - Menü Funktionen E-301
        - Ladeliste - Versandinfo E-302
        - Ladeliste - Aufträge E-304
- **Anhang** E-307
    - Übersicht E-309
    - Produktion E-310
        - Stücklisten-Ansicht E-310
        - Einstellungen (Stücklistenansicht) E-311
    - Sprossenkonstruktion E-312
        - Menüs in der Sprossenkonstruktion E-312
        - Menü Einstellungen E-313
        - Menü Sprossentypen E-313
        - Menü Dokument E-313
    - NV-Sprossenkonstruktion E-314
    - Sprossenkonstruktion (Dialog) E-316
        - Sprossenkonstruktion - Grafik E-316
        - Sprossenkonstruktion - Info E-318
    - Einstellungen (Sprossen) E-319
    - Sonderkonstruktionen E-320
    - Teilberechnung E-321
- **Partindex** E-323
    - Index Fertigung E-325

---

## Tutorial

### Überblick

Das Tutorial zum Modul *Fertigung* beschäftigt sich mit den Grundlagen der Produktionsübergabe und dem Versand in A+W Business. Es baut auf den Kenntnissen zu den Stammdaten auf.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

#### Themenblöcke
Zur Schulung des Moduls Fertigung gehören folgende Themenblöcke:
- Grundgedanken zu Fertigung und Versand
- Produktionsübergabe
- Rückmeldungen aus der Produktion
- Lieferwesen
- Übersichten
- Zusatzfunktionen

#### Vorausgesetzte Kenntnisse
Das Tutorial richtet sich an Teilnehmer, die in A+W Business den Versand organisieren. Die Teilnehmer müssen das Konzept der Stammdaten und die Auftragserfassung in A+W Business kennen.

### Dokumentation
Für das Modul *Fertigung* stehen folgende Dokumente zur Verfügung:

| Typ | Beschreibung |
| :--- | :--- |
| **Handout** | Ausdruck des Tutorials für die Schulung |
| **PDF** | Vollständige Unterlagen: <br> - Tutorial <br> - Softwarereferenz <br> - Index |
| **Online-Hilfe `<F1>`** | Kontextsensitive Dialog-Hilfe der A+W Business-Softwarereferenzen und Tutorials der Basisversion |

### Aufbau des Tutorials
Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

- **Überblick**
Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
  - Lernziele: Was soll vermittelt werden?
  - Nutzen: Wofür können Sie dieses Wissen einsetzen?
  - Merksätze: Welche Zusammenhänge müssen Sie sich merken?

- **Konzepte**
Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.

- **Übungen**
Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen.

- **Querverweise**
Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf ergänzende Informationen in der Softwarereferenz und in anderen Parts hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.

#### Lesehinweis
Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.
Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

### Darstellungskonventionen
Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

| Darstellung | Bedeutung |
| :--- | :--- |
| *Kursiv* | sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Produktionsübergabe*. |
| **Fett** | sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: Geben Sie den Wert **0** ein. |
| > | Mit dem sogenannten Brotkrumenpfad ist der Weg kennzeichnet, auf dem Sie einen Dialog öffnen, z. B. *Fertigung > Produktion > Produktionsübergabe*. |
| [] | Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit [OK] speichern Sie die Daten. |
| `< >` | Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit `<F1>` öffnen Sie die Online-Hilfe. |

### Menü-Übersicht
In diesem Abschnitt finden Sie eine kurze Übersicht über die Programmbereiche, die in den Themenblöcken dieser Schulung angesprochen werden.

[Abb. E-1: Menü Fertigung. Ein Screenshot des A+W Business Fensters mit dem geöffneten Menübaum für "Fertigung" und dem Dialog "Übergabe Produktion" im Vordergrund.]

**Produktion**
In diesem Bereich übergeben Sie die Aufträge an die Produktion.
- ⇨ “Produktionsübergabe" auf Seite E-20
- ⇨ Softwarereferenz, "Produktion" auf Seite E-169

**Lieferwesen**
In diesem Bereich organisieren Sie den Versand mit Ihrem eigenen Fuhrpark.
- ⇨ "Lieferwesen" auf Seite E-81
- ⇨ Softwarereferenz, "Lieferwesen" auf Seite E-203

**Gestellverwaltung**
In diesem Bereich können Sie eigene und Fremdgestelle verwalten und sich einen Überblick über den aktuellen Bestand verschaffen.
- ⇨ "Gestellverwaltung" auf Seite E-159
- ⇨ Softwarereferenz, "Gestellverwaltung" auf Seite E-253

**Terminübersicht**
In diesem Bereich können Sie sich einen Überblick über die Termine und die Kapazitäten verschaffen.
- ⇨ "Terminübersicht" auf Seite E-117
- ⇨ Softwarereferenz, "Terminübersicht" auf Seite E-267

**Zollverwaltung**
In diesem Bereich können Sie Zoll-Listen für den Warenexport erstellen.
- ⇨ Softwarereferenz, "Zollverwaltung" auf Seite E-282

**Angebotsoptimierung**
In diesem Bereich können Sie die Angebote zur Optimierung an die Produktion übergeben.
- ⇨ "Übergabe zur Angebotsoptimierung" auf Seite E-52
- ⇨ Softwarereferenz, "Angebotsoptimierung" auf Seite E-290

**Dokumentendaten**
In diesem Bereich können Sie sich Übersichten über Aufträge und korrespondierende Bestellungen anzeigen lassen und ggf. die Termine korrigieren. Eine ausführliche Beschreibung zu diesem Dialog finden Sie im Part Verkauf.
- ⇨ Verkauf, "Dokumentendaten" auf Seite C-728

**Artikel-Info**
In diesem Bereich können Sie sich Informationen zu den Produkten anzeigen lassen, die in A+W Business angelegt sind. Sie können dabei den Produktaufbau, die Preise und die Verfügbarkeit prüfen. Eine ausführliche Beschreibung zu diesem Dialog finden Sie im Part Verkauf.
- ⇨ Verkauf, "Artikel-Informationen" auf Seite C-595

**Faxnachrichten**
In diesem Bereich können Sie direkt aus A+W Business Faxnachrichten an Ihre Kunden und Lieferanten erstellen und versenden. Eine ausführliche Beschreibung zu diesem Dialog finden Sie im Part Überblick.
- ⇨ Einleitung, "Standard-Menüs" auf Seite A-53

**Ergänzende Informationen**
- ⇨ Einleitung, "Elemente des Programmfensters" auf Seite A-52
- ⇨ Verkauf: Softwarereferenz, "Dokument - Kopfdaten" auf Seite C-414

### Grundgedanken zu Fertigung und Versand
Über die Dokumentenverwaltung sind Aufträge erfasst worden, deren Positionen gefertigt werden müssen. Dazu müssen die Aufträge bzw. die Positionen in die Produktion weitergeleitet werden. Die für die Produktion relevanten Daten werden dabei in eine Datei geschrieben, die von der Produktionssoftware eingelesen werden kann.

Mit Hilfe des ERP-Webservices können diese Übergabedateien direkt an die Produktionssoftware A+W Production weitergeleitet und dort eingelesen werden.

[Abb. E-2: Produktionsübergabe und Versandorganisation. Ein Flussdiagramm, das den Prozess von der Auftragserfassung in A+W Business über die Produktionsübergabe an A+W Production, Rückmeldungen, Terminüberwachung und Versand bis zum Kunden darstellt.]

In dieser Übersicht sehen Sie, wie die Übergabe von Aufträgen an die Produktion, die Rückmeldungen aus der Produktion und die Organisation des Versands zusammenspielen.

Über den Auftragsstatus wird die korrekte Abfolge der Buchungen gesichert, so dass z. B. kein Auftrag an die Produktion übergeben werden kann, der nicht den erforderlichen Status hat. Der aktuelle Stand der Produktion wird als Rückmeldung an A+W Business gesendet. Damit wird der Status pro Auftragsposition und schließlich für den gesamten Auftrag umgesetzt. Je nach betrieblicher Organisation wird der Status automatisch oder manuell hochgesetzt. Die Daten einschließlich der Statusumsetzung können über Barcodes erfasst werden, womit Eingabefehler erheblich reduziert werden.

Über die Prüfung der Kapazitäten können Produktions- und Liefertermine geprüft und ggf. angepasst werden, so dass der Versand optimal organisiert werden kann.

Für den Versand werden Touren- und Beladungslisten erstellt, bei denen die Fahrzeuge anhand des zugelassenen Gewichts und der Tour optimal beladen werden können.

#### Ablauf für Fertigung und Versand
Die Reihenfolge der einzelnen Aktionen für die Fertigung und Auslieferung eines Auftrags hängt von den Gegebenheiten in Ihrem Betrieb ab.

Beispielsweise kann der Ablauf folgendermaßen organisiert sein:
1. Produktionsübergabe
2. Rückmeldung aus der Produktion prüfen
3. Lieferscheine drucken
4. Tourenplanung
5. Beladungsliste und Empfangsbestätigungsliste drucken
6. Auslieferung

---

## Produktionsübergabe
In diesem Themenblock lernen Sie, wie Sie Aufträge oder Angebote an die Produktion übergeben.

Dazu gehören folgende Lerneinheiten:
- "Varianten der Produktionsübergabe" auf Seite E-21
- "Produktionsübergabe ohne Kapazitätsplanung" auf Seite E-29
- "Produktionsübergabe mit A+W Business Kapazitätsplanung" auf Seite E-43
- "Produktionsübergabe mit A+W Production Capacity Planner" auf Seite E-47
- "Übergabe zur Angebotsoptimierung" auf Seite E-52

### Varianten der Produktionsübergabe
Die Daten der Aufträge werden zur Produktion an A+W Production oder ein anderes Produktionsprogramm übergeben, nachdem sie den dafür festgelegten Mindeststatus erreicht haben. Für diese Übergabe stehen folgende Varianten zur Verfügung:

- **Ohne Kapazitätsplanung:** Die Aufträge werden direkt an die Produktion übergeben, ohne sie zuvor in eine Kapazitätsplanung einzulasten.
- **Mit A+W Business Kapazitätsplanung**
- **Mit A+W Production Capacity Planner**

Bei diesen beiden Varianten durchlaufen die Aufträge folgende Schritte:
- Die Aufträge werden zunächst an die Kapazitätsplanung übergeben.
- Nach der Bestätigung oder Änderung der Produktions- und Liefertermine wird der Auftragsstatus hoch gesetzt.
- Die Maschinenkapazitäten sind damit reserviert.
- Anschließend werden die Aufträge an die Produktion übergeben und können produziert werden.

Die unterschiedlichen Abläufe werden Sie in getrennten Einheiten kennenlernen.

#### Datenübergabe
Die Daten Ihrer Aufträge werden zur Weiterverarbeitung an A+W Production zur Produktion bzw. A+W Standard Optimizer zur Zuschnittsoptimierung übergeben. Dazu müssen die Produkt- und Artikelnummern in A+W Business und A+W Production einander zugeordnet sein. Bei anderen Produktionsprogrammen können Sie für die Zuordnung einen entsprechenden Schlüssel in der *Produktverwaltung > Register Fertigung* im Feld *Schlüssel Optimierung* hinterlegen.

Für das Produzieren von ESG, VSG, Gießharz usw. wird für A+W Production eine Auflösung des Produktes auf Stücklistenebene durchgeführt. Der Produktionsstart wird stückbezogen an A+W Business zurückgemeldet. Je nach Einstellung wird der Auftragsstatus dann erhöht. Diese Einstellungen werden Sie in der Einheit *Rückmeldungen* kennenlernen.
- ⇨ "Rückmeldungen aus der Produktion" auf Seite E-58

Unabhängig davon, ob zuerst die Kapazitäten geplant werden, können Sie die Aufträge auf unterschiedliche Weise übergeben:
- **Manuelle Produktionsübergabe:** Für die manuelle Übergabe von Aufträgen steht der Dialog *Produktionsübergabe* zur Verfügung, in dem Sie alle Aufträge eines Nummernverwalters mit Status größer oder gleich *Produktionsfreigabe* und kleiner dem Status *feingeplant* übergeben können.
- **Automatische Produktionsübergabe mit Workflow-Task:** Für die automatische Übergabe wird ein Workflow-Task mit einem Intervall eingerichtet, damit in definierten Abständen nach Aufträgen gesucht wird, die an die Kapazitätsplanung oder die Produktion übergeben werden sollen. Die Beschreibung des Workflow-Tasks lernen Sie in einem eigenen Abschnitt kennen.
    - ⇨ "Produktionsübergabe per Workflow-Task" auf Seite E-26

#### OrderXML
Das OrderXML-Format basiert auf der genormten OpenTrans-Schnittstelle mit spezifischen Erweiterungen für produktionsrelevante Daten wie Gläser, Sprossen oder Bearbeitungen.

Das Format wird von der Produktionssoftware als Auftrag erkannt. Für jeden an die Produktion übergebenen Auftrag wird eine eigene Datei erstellt. Der Speicherort für die Übergabedatei muss in A+W Business und A+W Production angegeben werden.

#### Statusprüfung
Sowohl für die manuelle als auch für die automatische Produktionsübergabe müssen die Statuspunkte vollständig eingerichtet und zugeordnet sein. Über diese Statuszuordnungen prüft das System, ob die Auftragsdaten übergeben werden können.
Diese Zuordnungen wurden vor der Installation von A+W Business auf Ihren Betrieb abgestimmt und eingerichtet. Grundsätzliches zu den Statuspunkten und den Zuordnungen haben Sie bereits den Schulungen zu den Stammdaten und zum Verkauf kennengelernt. Daher wird das Thema hier nicht weiter erläutert.

#### Stornieren
Jeder Auftrag kann bis zu einem gewissen Zeitpunkt storniert werden. Dieser Zeitpunkt muss betriebsintern geregelt werden.
Bei der Stornierung einer Produktionsübergabe wird der übergebene Auftrag erneut an die Produktion übergeben. Dabei wird ein Stornokennzeichen gesetzt, an dem der Mitarbeiter in der Produktion die Stornierung erkennt.

#### Sonderfall Angebotsoptimierung
Angebote können an die Produktion übergeben werden, um den Zuschnitt zu berechnen. Diese Funktion steht zur Verfügung, wenn eine der folgenden Varianten für die Produktionsübergabe genutzt wird:
- Keine Kapazitätsplanung
- A+W Business Kapazitätsplanung

Die Funktion ist blockiert, wenn die Produktionsübergabe von Angeboten per Workflow-Task aktiviert wird.
Die Übergabe von Angeboten zur Optimierung ist ausführlich in einer eigenen Einheit beschrieben.
- ⇨ "Übergabe zur Angebotsoptimierung" auf Seite E-52

### Schematische Abläufe der Varianten
In diesem Abschnitt sind die unterschiedlichen Abläufe der Produktionsübergabe schematisch dargestellt. Die Darstellungen mit Kapazitätsplanung bauen aufeinander auf, so dass die zuvor aufgeführten Schritte zusammengefasst werden.

Die Abläufe sind als Beispiele zu verstehen. In Ihrem Betrieb kann der Übergabeprozess durchaus auch anders organisiert sein.

#### Schematischer Ablauf ohne Kapazitätsplanung
[Flussdiagramm: Auftrag erfasst -> Produktionsfreigabe (Statuspunkt 35) -> Produktionsübergabe (Statuspunkt 40) -> Einlastung in A+W Production -> Produktions-Rückmeldungen. Ein paralleler Pfad zeigt, dass ein Auftrag mit Statuspunkt 810 storniert werden kann.]

Für die Produktionsübergabe werden der Mindest- und der Sperrstatus geprüft. Aufträge, die diese Bedingungen nicht erfüllten, können nicht übergeben werden.

#### Schematischer Ablauf mit Kapazitätsplanung
[Flussdiagramm: Auftrag erfasst -> Prüfung: Produktionsfreigabe? (ja/nein) -> `nein`: Status ändern, `ja`: Kapazitätsplanung -> Prüfung: Einlastung erfolgreich? (ja/nein) -> `nein`: Termine ändern, `ja`: Auftragsbestätigung drucken -> Produktionsfreigabe -> Produktionsübergabe -> Einlastung in A+W Production -> Produktionsübergabe -> Produktions-Rückmeldungen.]

#### Schematischer Ablauf mit Bestellung und Positionsänderung
[Flussdiagramm: Auftrag erfasst -> Kapazitätsplanung -> Auftragsbestätigung drucken -> Prüfung: Bestellteile enthalten? (ja/nein) -> `ja`: Bestellung schreiben, Wareneingang abwarten -> `nein`: Produktionsfreigabe -> Produktionsübergabe -> Prüfung: Position geändert? (ja/nein) -> `nein`: Produktion -> Produktions-Rückmeldungen.]

Aus der Kapazitätsplanung werden nach erfolgreicher Planung die Zeitkosten und das Produktionsdatum zurückgemeldet.

### Änderung von übergebenen Positionen
Ein Auftrag, der an die Produktion übergeben wurde, hat Status 40. Wenn ein solcher Auftrag geändert wird, müssen zwei Fälle unterschieden werden:
- Änderungen von Preisen, Rabatten usw., die nicht produktionsrelevant sind, verändern weder den Status noch muss der Auftrag erneut übergeben werden.
- Nach einer Änderung von Mengen, Maßen, Gläsern u. Ä. erhält der Auftrag ein entsprechendes Kennzeichen und wird sofort durch den Workflow-Task an die Produktion übergeben.

In der Betriebsorganisation muss geklärt werden, was mit Positionen geschehen soll, die bereits produziert sind. Es kann z. B. festgelegt werden, dass eine Auftragsposition storniert und neu angelegt werden muss.

### Übergabe von Aufträgen mit Bestellungen
Wenn Sie z. B. ISO mit ESG-Scheiben produzieren, das ESG aber nicht selbst herstellen, hängt der Produktionsprozess von der Lieferung der ESG-Scheiben ab. Nach der Buchung der Waren im Wareneingang können die Daten automatisch an A+W Production übergeben werden. Sind in dem gemeldeten Wareneingang solche ESG-Scheiben enthalten, wird für die betreffenden ISO-Einheiten der Produktionsstart initiiert.
Diese automatische Übergabe von Wareneingangsdaten steht in Verbindung mit dem Wareneingang für den Einkauf.

### Produktionsübergabe per Workflow-Task
Ein Workflow-Task dient der weitgehenden automatischen Verarbeitung von Aufträgen. Inwieweit manuelle Eingriffe zwischen aufeinander folgenden Workflow-Tasks notwendig sind, hängt davon ab, wie die Abläufe in Ihrem Betrieb organisiert sind. Die notwendigen Einstellungen werden bei der Installation festgelegt und sollten nachträglich nicht geändert werden. In diesem Abschnitt werden daher nur die schematischen Abläufe dargestellt.

Jeder Workflow-Task besteht aus einer oder mehreren Customizing-Formeln. In diesen Formeln sind die einzelnen Aktionen definiert, die ausgeführt werden sollen. Der A+W Business Interface Service führt die Tasks entweder periodisch oder zu einem festen Zeitpunkt aus.

#### Einstellungen für den Workflow-Task
Um einen Workflow-Task einzurichten, sind drei Schritte erforderlich:
1. Formel für die automatische Produktionsübergabe unter *Stammdaten > Firma > Formeln* anlegen.
2. Formel zu einem Workflow-Task unter *Stammdaten > Firma > Customizing > Register Workflow Tasks* zuordnen.
3. Workflow-Task unter *Stammdaten > Firma > Customizing > Register Autom. Prozessausführung* einstellen.

Wenn Sie die Produktionsübergabe auf den Workflow-Task umstellen, lassen Sie sich von Ihrem Service-Mitarbeiter bei der A+W Software GmbH unterstützen.
In dieser Einheit werden die Einstellungen an einem Beispiel gezeigt, das sich von den Einstellungen in Ihrem Unternehmen unterscheiden kann.

**So prüfen Sie die Einstellungen für den Workflow-Task**
1. Wählen Sie im Menü *Stammdaten > Firma > Customizing* und wechseln Sie zum Register *Workflow Tasks*.

    [Abb. E-3: Beispiel Workflow-Tasks. Screenshot des Customizing-Fensters mit dem Reiter "Workflow tasks", der eine Liste von Workflow-Tasks und deren zugehörigen Formeln zeigt.]

    In diesem Register sind die definierten Workflow-Tasks für A+W Business mit den zugeordneten Formeln aufgeführt.
2. Markieren Sie den Workflow Task, den Sie bearbeiten wollen.
3. Wechseln Sie zum Register *Autom. Prozessausführung*.

    [Abb. E-4: Prozessausführung für Workflow-Tasks. Screenshot des Reiters "Autom. Prozessausführung", der die Einstellungen für die Ausführung eines ausgewählten Workflow-Tasks zeigt, einschließlich Sequenz, Startzeit/Intervall (A) und Ausführungstyp (B).]

    In diesem Register sind die Startzeiten und die Intervalle für die definierten Workflow-Tasks festgelegt.
4. Ändern Sie ggf. die Startzeit und das Intervall:
    - Wenn die Daten zyklisch übergeben werden sollen, wählen Sie die Zeit **00:01**.
    - Wenn die Daten zu einem bestimmten Zeitpunkt übergeben werden sollen, tragen Sie in der Spalte *hh:mm* die Uhrzeit ein.
5. Wenn mehrere Workflow-Tasks definiert sind, wird in der Spalte *Sequenz* angezeigt, in welcher Reihenfolge sie ausgeführt werden.
6. Wählen Sie im Menü *Start > Speichern*, um die Änderungen zu speichern.
    Die Daten werden gespeichert und der Workflow-Task wird nach den neuen Einstellungen ausgeführt.

---

## Produktionsübergabe ohne Kapazitätsplanung

**Lernziele**
- Einstellungen zur Produktionsübergabe ohne Kapazitätsplanung kennenlernen.
- Aufträge an die Produktion übergeben.
- Übergabe stornieren.

**Nutzen**
- Sie übergeben Auftragsdaten aus A+W Business direkt an A+W Production oder A+W Standard Optimizer zur Fertigung.
- Wenn Sie ESG, VSG, Gießharz usw. produzieren, können Sie die Stücklistenauflösung ohne weitere Eingriffe übergeben und vermeiden damit eine fehlerhafte Datenübergabe.
- Bei der automatischen Übergabe per Workflow-Task werden die Aufträge nach einem definierten Intervall direkt an die Produktion übergeben.

> **Merke**
> - **Aufträge an die Produktion übergeben:** Sie können die Aufträge manuell aus einem Nummernverwalter oder (automatisch) per Workflow-Task an die Produktion übergeben.
> - **Übergabedaten:** Die Übergabedaten werden in eine Datei geschrieben, die von A+W Production ausgelesen wird. Der Speicherort dieser Datei muss A+W Business und A+W Production bekannt sein.
> - **Übergabe von SN-Dateien:** Für die Übergabe von Shaping+Nesting-Dateien (SN-Dateien) müssen folgende Einstellungen festgelegt werden:
>   - In den Firmendaten muss die automatische Generierung aktiviert werden.
>   - In den Utilities müssen Regeln eingerichtet sein, nach denen die SN-Datei erzeugt wird.
> - **Auftragsstatus:** Statusprüfungen vor der Übergabe verhindern, dass Aufträge mit falschem Status übergeben werden. Bei der manuellen Produktionsübergabe wird immer nach dem Mindest- und Sperrstatus übergeben.
> - **Nummernkreis:** Die Nummernkreise für Aufträge und Angebote müssen getrennt sein, damit sich die Dokumente bei der Übergabe nicht gegenseitig überschreiben.
> - **Workflow-Task:** Für die automatische Produktionsübergabe muss ein Workflow-Task eingerichtet werden. Den Workflow-Task legen Sie im Dialog *Customizing* (pro Mandant) fest.
> - **Formel:** Der Workflow-Task wird mit einer Formel definiert.
> - **Datenübertragung:** Bei der automatischen Produktionsübergabe werden die Auftragsdaten per A+W Business-Interface-Service übertragen.
> - **Voreinstellungen:**
>   - **Firmendaten:** Register *Produktion*; Register *Produktion > Einstellungen Aufträge*; Register *System* (für SN-Dateien)
>   - **Stammdaten:** *Firma > Customizing > Register Workflow Tasks*

> **Beschreibung der Einstellungen**
> In dieser Lerneinheit werden die allgemeinen Einstellungen und Funktionen beschrieben, die für die Produktionsübergabe ohne Kapazitätsplanung gelten. In den Lerneinheiten zur Produktionsübergabe mit Kapazitätsplanung werden Sie dann nur noch auf die Unterschiede und Besonderheiten aufmerksam gemacht. Daher sollten Sie der Einheit *Produktionsübergabe ohne Kapazitätsplanung* besondere Aufmerksamkeit widmen.

### Produktionsübergabe einrichten
Die Einstellungen für die Datenübergabe können nur von einem Mitarbeiter mit Administratorrechten eingerichtet werden.
In dieser Einheit lernen Sie, wie Sie die Parameter für die manuelle Produktionsübergabe (ohne Kapazitätsplanung) einrichten. Die Einstellungen gelten dann sowohl für die manuelle Produktionsübergabe als auch für die automatische per Workflow-Task.

> **Geänderte Einstellungen können schwerwiegende Fehler erzeugen**
> In der Regel werden die Einstellungen für die Produktionsübergabe bei der Installation von A+W Business auf die Bedingungen im Betrieb abgestimmt. Wenn Sie diese Einstellungen ändern, greifen Sie tief in die Funktionalität der Produktionsübergabe ein. Das kann zu schwerwiegenden Fehlern führen, so dass die Daten von Aufträgen und Angeboten nicht mehr übergeben werden können. Die Beschreibung der Einstellungen dient also in erster Linie dazu, Ihnen die Vorgänge deutlicher zu machen und ggf. bei Rücksprachen mit dem Service der A+W Software GmbH Fragen zu den Einstellungen schnell beantworten zu können.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
- "So prüfen Sie die Einstellungen in den Firmendaten" auf Seite E-32
- "So prüfen Sie die Voreinstellungen für die Produktionsübergabe" auf Seite E-33

#### So prüfen Sie die Einstellungen in den Firmendaten
1. Wählen Sie im Menü *Stammdaten > Firma > Firmendaten* und wechseln Sie zum Register *Produktion*. Diese Einstellungen gelten sowohl für die manuelle Produktionsübergabe als auch für die automatische Übergabe per Workflow-Task.

   [Abb. E-5: Stammdaten - Einstellungen für automatische Produktionsübergabe. Screenshot des Firmendaten-Dialogs, Reiter "Produktion", mit den Bereichen für Aufträge (A), Angebote (B), PPS-Webservice (C), ERP-Webservice (E) und Meldungen (D).]

   - A: Einstellungen für die Produktionsübergabe von Aufträgen festlegen
   - B: Einstellungen für die Produktionsübergabe von Angeboten festlegen
   - C: Adresse für den PPS-Webservice eingeben
   - D: Einstellung zur Meldung des Wareneingangs an A+W Production
   - E: Adresse für ERP-Webservice eingeben

2. Tragen Sie in den Bereichen *A+W Production Anbindung* und *ERP-Webservice* die Adressen für den Datenaustausch ein:
   - Die Angabe im Feld *ERP-Webservice (E)* benötigen Sie für Datenübertragungen per OrderXML. Achten Sie darauf, dass Sie den ERP-Webservice wählen, der zu der installierten Version von A+W Business passt.
   - Die Angabe im Feld *PPS-Webservice-URL (C)* benötigen Sie für folgende Datenübertragungen:
     - Stornierung von Aufträgen per Workflow-Task
     - Meldung des Wareneingangs (D) direkt an A+W Production. Diese Meldungen werden bei Positionen benötigt, zu deren Fertigung auf Bestellungen gewartet werden muss. Wenn Sie den PPS-Webservice wählen, müssen Sie auch die URL eintragen.
     - Dateilose Rückmeldungen. Diese Funktion lernen Sie in der Einheit *Rückmeldungen* kennen. (⇨ "Rückmeldungen aus der Produktion" auf Seite E-58)
3. Wählen Sie im Menü *Start > Speichern*, um die Änderungen zu speichern.

#### So prüfen Sie die Voreinstellungen für die Produktionsübergabe
> **Benutzerabhängige Einstellung**
> Der Dialog kann von unterschiedlichen Stellen aus geöffnet werden, z. B. aus dem Dialog *Produktionsübergabe*. In dieser Anleitung wird er von den Firmendaten aus geöffnet, weil Sie hier auch die Einstellungen für die Angebotsoptimierung und die Rückmeldungen festlegen können. Wenn Sie die Einstellungen benutzerabhängig eingerichtet haben wollen, müssen Sie folgenden Weg wählen: *Menü Fertigung > Übergabe Produktion > Menü Funktionen > Einstellungen*

1. Klicken Sie im Dialog *Firmendaten > Register Produktion* auf **[Einstellungen Aufträge]**.

   [Abb. E-6: Produktionsübergabe für Aufträge. Screenshot des Dialogs "Einstellungen - Produktionsübergabe" mit den Reitern für Schnittstellen, Parameter etc. Gezeigt wird der Reiter "Schnittstelle" mit Optionen für das Übertragungsformat (A), CAD Designer (B), OrderXML-Version (C) und Statusprüfung (D).]

2. Prüfen Sie im Register *Schnittstelle*, ob die Versionen und die Pfade korrekt eingestellt sind. Standardmäßig ist im Bereich *Schnittstelle Produktion (A)* die OrderXML-Übergabe aktiviert. Wenn Sie mit *AWPool* arbeiten, müssen Sie die entsprechende Version auswählen.
3. Geben Sie den Pfad der Übergabedatei an, der von A+W Production überwacht wird, damit die Daten automatisch eingelesen werden.
4. Tragen Sie ggf. die Daten für die Übergabe an *AWDesign (B)* ein. Achten Sie dabei darauf, dass der Speicherpfad auch in *CAD Designer* bekannt ist.
5. Prüfen Sie die Einstellungen im Bereich *OrderXML (C)*. Die Adresse des ERP-Webservices wird aus den Einstellungen in den Firmendaten übernommen. Wenn Sie mit der *AWPool-Übergabe* arbeiten entfällt diese Angabe.
6. Wählen Sie im Bereich *Modus der Übergabe* die Option **nach Mindest- und Sperrstatus Produktionsübergabe (D)**. Mit dieser Einstellung werden die Aufträge nach der Statusprüfung direkt an die Produktion übergeben.
7. Wechseln Sie zum Register *Übergabe Parameter*.

   [Abb. E-7: Einstellungen – Übergabeparameter. Screenshot des gleichnamigen Dialogs, der eine Reihe von Checkboxen zur Konfiguration der zu übergebenden Daten anzeigt.]

8. Wenn Sie mit A+W Production arbeiten, müssen Sie die Checkbox **A+W Production** markieren. Für alle anderen Programme bleibt die Checkbox leer.
9. Markieren Sie die Checkboxen für die Daten, die an die Produktion übergeben werden sollen. Die Bedeutung der Checkboxen ist ausführlich in der Softwarereferenz beschrieben.
   - ⇨ Softwarereferenz, “Einstellungen Produktionsübergabe – Übergabe Parameter" auf Seite E-177
10. Wechseln Sie zum Register *Zusätzliche Schnittstellen*, wenn Sie mit einer Schnittstelle zu RONA arbeiten, und tragen Sie die Pfade für die Schnittstellendatei ein.
11. Wechseln Sie zum Register *Texte/Anlage* und markieren Sie die Textkennzeichen und Dateianhänge, die Sie zusätzlich übergeben wollen.

    [Abb. E-8: Einstellungen - Texte/Anlagen. Screenshot des gleichnamigen Dialogs zur Auswahl der zu übertragenden Texte und Dateianhänge.]

12. Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern. Die Daten werden gespeichert.

### Auftragsdaten an die Produktion übergeben
Die Auftragsdaten können manuell oder per Workflow-Task an die Produktion übergeben werden. In diesem Abschnitt lernen Sie, wie Sie Auftragsdaten aus einem Nummernverwalter manuell direkt an die Produktion übergeben.

**So übergeben Sie die Aufträge manuell**
1. Wählen Sie im Menü *Fertigung > Produktion > Übergabe Produktion*.
2. Wählen Sie den *Nummernverwalter (A)* aus, in dem Sie die Aufträge für die Produktion gesammelt haben.
3. Prüfen Sie, ob alle angezeigten Aufträge den Mindeststatus erreicht haben (B). Aufträge, deren Status nicht zwischen dem Mindest- und dem Sperrstatus liegen, werden nicht übergeben.

   [Abb. E-9: Produktionsübergabe starten. Screenshot des Dialogs "Übergabe Produktion", der eine Liste von Aufträgen anzeigt. Hervorgehoben sind die Auswahl des Nummernverwalters (A) und die Status-Spalte (B).]

4. Wählen Sie im Menü *Start > Ausführen*, um die Übertragung zu starten. Im Bereich *Ausgabe* wird angezeigt, welcher Auftrag und welche Auftragsposition aktuell verarbeitet werden. Die Daten werden als Datei in dem Verzeichnis gespeichert, das Sie im Dialog *Einstellungen-Produktionsübergabe* angegeben haben.

   [Abb. E-10: Produktionsübergabe abgeschlossen. Screenshot des gleichen Dialogs nach der Übergabe. Der Status der Aufträge (A) ist auf 40 aktualisiert und die Anzahl der übergebenen Positionen (B) wird angezeigt.]

   Wenn ein Auftrag vollständig verarbeitet wurde, wird der Status umgesetzt. Die Anzahl der nicht übergebenen Aufträge wird in einer Meldung angezeigt.

### Produktionsübergabe stornieren
Sie können einen Auftrag nach der Übergabe stornieren, damit er nicht produziert wird. Dazu übergeben Sie den Auftrag erneut, setzen dabei aber ein Stornokennzeichen.
- Um einen Auftrag mit der automatischen Produktionsübergabe zu stornieren, müssen die Mengen der Auftragspositionen auf 0 gesetzt werden. Anschließend wird der Auftrag wieder an die Produktion übergeben. Danach wird der PPS-Webservice zur Stornierung der Produktionsübergabe automatisch aufgerufen. Der Auftrag wird mit den neuen Werten sofort durch den Workflow-Task übergeben.
- Ist der Statuspunkt **810 Übergabe AW-Pool storniert** einem Anwenderstatus zugeordnet, wird durch die Stornierung der Auftragsstatus auf den gewünschten Anwenderstatus gesetzt, z. B. durch das Heruntersetzen des Status. Ist der Statuspunkt 810 nicht zugeordnet, behält der Auftrag den bisherigen Status.
- Eine Stornierung ist nur bis zur Bestellübergabe möglich.

> **Beispiel**
> Ein Auftrag, der an die Produktion übergeben wurde, hat Status 40. Eine Stornierung verändert den Status nicht. Nach der Änderung der Menge erhält der Auftrag ein Stornokennzeichen und wird daher sofort von der automatischen Produktionsübergabe durch den Workflow-Task übergeben.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
- "So stornieren Sie die Produktionsübergabe manuell" auf Seite E-40
- "So stornieren Sie die Produktion, wenn Sie Aufträge automatisch übergeben" auf Seite E-41

#### So stornieren Sie die Produktionsübergabe manuell
Sie können einen manuell übergebenen Auftrag nach der Übergabe vollständig stornieren, damit er nicht produziert wird. Dazu übergeben Sie den Auftrag erneut manuell, setzen dabei aber ein Stornokennzeichen.

1. Stellen Sie den Auftrag, den Sie stornieren wollen, in einen neuen Nummernverwalter.
2. Wählen Sie im Menü *Fertigung > Produktion > Übergabe Produktion*. Der Dialog *Produktionsübergabe* wird geöffnet.
3. Wählen Sie den Nummernverwalter aus, in dem der Auftrag steht (A).
4. Wählen Sie den Modus **Stornieren (B)**.
5. Wählen Sie im Menü *Start > Ausführen*, um die Stornierung zu starten.
   Die Daten werden mit einem Storno-Kennzeichen als Datei im angegebenen Verzeichnis gespeichert. Der Status des Auftrags wird auf *Übergabe Produktion storniert* umgesetzt.

[Abb. E-11: Auftrag stornieren. Screenshot des Dialogs "Übergabe Produktion", wobei der Nummernverwalter (A) und der Modus "Storno" (B) hervorgehoben sind.]

#### So stornieren Sie die Produktion, wenn Sie Aufträge automatisch übergeben
1. Öffnen Sie den Auftrag und wechseln Sie zum Register *Positionen*.
2. Markieren Sie die Position, die Sie stornieren wollen.
   - Wenn Sie z. B. die Stückzahl ändern wollen, fahren Sie mit Schritt 3 fort.
   - Wenn Sie die gesamte Position stornieren wollen, dann wählen Sie im Menü *Bearbeiten > Löschen* und fahren Sie mit Schritt 5 fort.
   
   [Abb. E-12: Übergebene Position stornieren. Screenshot der Auftragspositionenansicht, in der eine Zeile markiert ist.]

3. Wählen Sie im Menü *Funktionen > Gruppe Position > Gesperrte Position ändern*. Das Eingabefeld *Stück* wird freigeschaltet.
4. Tragen Sie die neue Stückzahl ein.
5. Wählen Sie im Menü *Start > Speichern*, um die Änderung zu speichern.
6. Wiederholen Sie die Schritte 2 bis 5 für alle Positionen, die geändert werden sollen.
7. Schließen Sie die Positionserfassung und den Auftrag.
   Der geänderte Auftrag wird durch den Workflow-Task automatisch an die Produktion übergeben.

### Übungen
- Richten Sie einen Nummernverwalter ein, in dem Sie Aufträge sammeln, die an Sie die Produktion übergeben wollen.
- Übergeben Sie die Aufträge manuell an die Produktion.
- Prüfen Sie, ob der Status aller Aufträge im Nummernverwalter umgesetzt ist.
- Prüfen Sie, warum einige Aufträge nicht übergeben wurden. Ist bei diesen Aufträgen der Mindeststatus erreicht?

**Ergänzende Informationen**
- ⇨ Stammdaten, "Firmendaten - Produktion" auf Seite B-972
- ⇨ Softwarereferenz, “Übergabe Produktion" auf Seite E-170
- ⇨ Softwarereferenz, "Einstellungen Produktionsübergabe" auf Seite E-174

---

## Produktionsübergabe mit A+W Business Kapazitätsplanung

**Lernziele**
- Einstellungen zur Übergabe an die A+W Business Kapazitätsplanung kennenlernen.

**Nutzen**
- Die Auftragsdaten aus A+W Business werden automatisch zuerst an die Kapazitätsplanung übergeben.
- Terminverschiebungen aufgrund von Kapazitätsengpässen werden nach der Bestätigung durch den Auftragserfasser in den Auftrag zurückgeschrieben.
- Bei der automatischen Übergabe per Workflow-Task werden die Aufträge nach einem definierten Intervall zunächst an die Kapazitätsplanung übergeben. Nach der erfolgreichen Einlastung werden sie automatisch an die Produktion übergeben.

> **Merke**
> - **Auftragsstatus:** Statusprüfungen vor der Übergabe verhindern, dass Aufträge mit falschem Status übergeben werden.
> - **Nummernkreis:** Die Nummernkreise für Aufträge und Angebote müssen getrennt sein, damit sich die Dokumente bei der Übergabe nicht gegenseitig überschreiben.
> - **Übergabe an die Kapazitätsplanung:** Für die Planung der Kapazitäten werden die Daten im OrderXML-Format übergeben. Dazu muss der ERP-Webservice eingerichtet sein.
> - **Voreinstellungen:**
>   - **Firmendaten:** Register *Produktion*; Register *Kapa-Planung*; Register *Produktion > Einstellungen Aufträge*
>   - **Stammdaten:** *Firma > Customizing > Register Workflow Tasks*

> **Beschreibung der Einstellungen**
> Die grundlegenden Einstellungen und Funktionen sind in der Einheit *Produktionsübergabe ohne Kapazitätsplanung* erklärt worden. In dieser Lerneinheit werden daher nur die Unterschiede oder zusätzlichen Einstellungen behandelt, die für die Übergabe an die A+W Business Kapazitätsplanung gelten.

### Einstellungen in den Firmendaten
Die Einstellungen für die Datenübergabe können nur von einem Mitarbeiter mit Administratorrechten eingerichtet werden. Für die Produktionsübergabe mit der A+W Business Kapazitätsplanung müssen Sie folgende Einstellungen prüfen:
- Einstellungen für die automatische Produktionsübergabe. Diese Einstellungen haben Sie bereits kennengelernt.
  - ⇨ "So prüfen Sie die Einstellungen in den Firmendaten" auf Seite E-32
- Aktivierung der A+W Business Kapazitätsplanung
- Voreinstellungen der Parameter.

In dieser Einheit lernen Sie, wie Sie die Einstellungen für die Produktionsübergabe mit A+W Business Kapazitätsplanung prüfen. Die Beschreibung bezieht die Einstellungen für den Workflow-Task mit ein. Die Übergabe kann jedoch auch manuell ausgelöst werden.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
- "So prüfen Sie die Einstellungen für die Produktionsübergabe mit A+W Business Kapazitätsplanung" auf Seite E-45
- "So prüfen Sie die Voreinstellungen für die Produktionsübergabe" auf Seite E-46

#### So prüfen Sie die Einstellungen für die Produktionsübergabe mit A+W Business Kapazitätsplanung
1. Wählen Sie im Menü *Stammdaten > Firma > Firmendaten* und wechseln Sie zum Register *Kapa-Planung*.

   [Abb. E-13: Stammdaten – Einstellungen für Produktionsübergabe mit A+W Business Kapazitätsplanung. Screenshot des Firmendaten-Dialogs, Reiter "Kapa-Planung".]

2. Wählen Sie im Bereich *Kapazitätsplanung (A)* die Version **0-Kapazitätsplanung** aus.
3. Markieren Sie im Bereich *Fehlermeldungen aus autom. Kapazitätsplanung* eine der Optionen:
   - **An Auftragserfasser:** Mit dieser Einstellung werden die Fehlermeldungen an den Mitarbeiter gesendet, der den jeweiligen Auftrag erfasst hat. Solche Fehlermeldungen beziehen sich in aller Regel auf Termine, die nicht eingehalten werden können, weil nicht genügend Kapazitäten zur Verfügung stehen.
   - **An Mitarbeiter:** Mit dieser Einstellung wird das Feld für die Auswahl eines Mitarbeiters freigeschaltet. Wählen Sie diese Option, wenn nur ein einziger Mitarbeiter die Aufträge bearbeitet, die nicht problemlos eingelastet werden konnten.
4. Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern.
Die Einstellungen im Bereich *A+W Business-Kapazitätsplanung* lernen Sie in einer gesonderten Schulung zur Kapazitätsplanung kennen.

#### So prüfen Sie die Voreinstellungen für die Produktionsübergabe
1. Klicken Sie im Dialog *Firmendaten > Register Produktion* auf **[Einstellungen Aufträge]**.

   [Abb. E-14: Produktionsübergabe für Aufträge. Screenshot des Dialogs "Einstellungen - Produktionsübergabe", Reiter "Schnittstelle", der dieselben Optionen wie in Abb. E-6 zeigt.]

2. Wählen Sie im Bereich *Modus der Übergabe* die Option **(D) Nach Mindest- und Sperrstatus Produktionsübergabe**. Für die automatische Produktionsübergabe wird der Auftragsstatus mit dem Mindest- und Sperrstatus für die Produktionsübergabe verglichen. Liegt der Auftragsstatus dazwischen, wird der Auftrag automatisch an die Produktion übergeben. Dies ist die Standardeinstellung.
3. Klicken Sie auf **[OK]**, um die Änderung zu übernehmen.

---

## Produktionsübergabe mit A+W Production Capacity Planner

**Lernziele**
- Einstellungen zur Übergabe an A+W Production Capacity Planner kennenlernen.

**Nutzen**
- Die Auftragsdaten aus A+W Business werden automatisch zuerst an A+W Production Capacity Planner übergeben.
- Terminverschiebungen aufgrund von Kapazitätsengpässen werden nach der Bestätigung durch den Auftragserfasser in den Auftrag zurückgeschrieben.
- Bei der automatischen Übergabe per Workflow-Task werden die Aufträge nach einem definierten Intervall zunächst an die Kapazitätsplanung übergeben. Nach der erfolgreichen Einlastung werden sie automatisch an die Produktion übergeben.

> **Merke**
> - **Auftragsstatus:** Statusprüfungen vor der Übergabe verhindern, dass Aufträge mit falschem Status übergeben werden.
> - **Nummernkreis:** Die Nummernkreise für Aufträge und Angebote müssen getrennt sein, da sonst auch Angebote an A+W Production Capacity Planner übergeben werden.
> - **Übergabe an die Kapazitätsplanung:** Für die Planung der Kapazitäten werden die Daten im OrderXML-Format übergeben. Dazu muss der ERP-Webservice eingerichtet sein.
> - **Voreinstellungen:**
>   - **Firmendaten:** Register *Produktion*; Register *Kapa-Planung*; Register *Produktion > Einstellungen Aufträge*
>   - **Stammdaten:** *Firma > Customizing > Register Workflow Tasks*

> **Beschreibung der Einstellungen**
> Die grundlegenden Einstellungen und Funktionen sind in der Einheit *Produktionsübergabe ohne Kapazitätsplanung* erklärt worden. In dieser Lerneinheit werden daher nur die Unterschiede oder zusätzlichen Einstellungen behandelt, die für die Übergabe an A+W Production Capacity Planner gelten.

### Einstellungen für A+W Production Capacity Planner
Die Einstellungen für die Datenübergabe können nur von einem Mitarbeiter mit Administratorrechten eingerichtet werden. Für die Produktionsübergabe mit der A+W Production Capacity Planner müssen Sie folgende Einstellungen prüfen:
- Einstellungen für die automatische Produktionsübergabe. Diese Einstellungen haben Sie bereits kennen gelernt.
  - ⇨ "So prüfen Sie die Einstellungen in den Firmendaten" auf Seite E-32
- Aktivierung der A+W Production Capacity Planner
- Voreinstellungen der Parameter.

In dieser Einheit lernen Sie, wie Sie die Einstellungen für die Produktionsübergabe mit A+W Production Capacity Planner prüfen.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
- “So aktivieren Sie die Übergabe an A+W Production Capacity Planner" auf Seite E-49
- "So prüfen Sie die Voreinstellungen für die Produktionsübergabe" auf Seite E-51

#### So aktivieren Sie die Übergabe an A+W Production Capacity Planner
1. Wählen Sie im Menü *Stammdaten > Firma > Firmendaten* und wechseln Sie zum Register *Kapa-Planung*.

   [Abb. E-15: Stammdaten – Einstellungen für Produktionsübergabe A+W Production Capacity Planner. Screenshot des Firmendaten-Dialogs, Reiter "Kapa-Planung", mit hervorgehobener Version (A), Empfänger (B) und Planungseinstellungen (C).]

2. Wählen Sie im Bereich *Kapazitätsplanung (A)* die Version **1-A+W Production Capacity Planner** aus.
3. Markieren Sie im Bereich *Fehlermeldungen aus autom. Kapazitätsplanung* eine der Optionen:
   - **An Auftragserfasser:** Mit dieser Einstellung werden die Fehlermeldungen an den Mitarbeiter gesendet, der den jeweiligen Auftrag erfasst hat.
   - **An Mitarbeiter:** Mit dieser Einstellung wird das Feld für die Auswahl eines Mitarbeiters freigeschaltet.
4. Markieren Sie im Bereich *A+W Production-Kapazitätsplanung* die Option für die Planungsrückmeldungen:
   - **Angebot oder Auftrag wird gesucht:** Angebote und Aufträge werden auf die gleiche Weise in die Kapazitätsplanung eingelastet. Wenn Sie diese Option wählen, müssen Sie Angebote, die zur Optimierung übergeben wurden, manuell stornieren, damit sie nicht gefertigt werden.
   - **Immer als Auftrag (muss bei kapazitativer Übergabe aktiv sein):** Mit dieser Einstellung werden nur die Aufträge in die Kapazitätsplanung eingelastet. Dies ist die Standardeinstellung. Wenn Sie versuchen, ein Angebot manuell zu übergeben, ist die Funktion blockiert.
5. Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern.
6. Wechseln Sie zum Register *Produktion* und prüfen Sie die Einstellungen für die Datenübertragung durch den A+W Business Interface Service.
Diese Einstellungen sind ausführlich in der Einheit für die A+W Business Kapazitätsplanung behandelt.
   - ⇨ "Einstellungen in den Firmendaten" auf Seite E-44

Die Einstellungen im Bereich *A+W Production-Kapazitätsplanung* lernen Sie in einer gesonderten Schulung zur Kapazitätsplanung kennen.
