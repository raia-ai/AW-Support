---
title: "DE_AWEnterprise_Verkauf_4_9"
source: "DE_AWEnterprise_Verkauf_4_9.pdf"
tags: ["A+W Enterprise", "Verkauf", "ERP", "Software Reference", "Fertigmeldung", "Vorgangsänderung", "Auftragserfassung", "German", "Index"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for the A+W Enterprise Sales (Verkauf) module, detailing functionalities such as transaction overviews, completion reporting (Fertigmeldung), and bulk transaction changes (Vorgangsänderung)."
long_description: "This document is a section of the A+W Enterprise software reference manual, specifically focusing on the 'Verkauf' (Sales) module. It provides detailed descriptions of various functions and dialogs available to users. Key topics covered include an overview of transactions ('Übersichten zu Vorgängen'), the process for reporting production completion ('Fertigmeldung'), and the dialog for making simultaneous changes to multiple transactions ('Vorgangsänderung'). The guide explains UI elements, fields, their purposes, and associated technical database information (DB-Felder). It also includes a comprehensive alphabetical index ('Partindex') for quick reference to specific features and terms within the sales module documentation. This manual is intended for users and administrators of the A+W Enterprise system to understand and effectively utilize its sales-related functionalities."
---

---
## Übersichten zu Vorgängen

- **Aktive Wiedervorlage:**
  Alle Nachrichten werden beim Starten des Programms auf dem Bildschirm angezeigt.
- **direktes Löschen des Vorgangs:**
  Die Funktion ist nur zulässig bei Kundenangeboten und Lieferantenanfragen. Damit wird die Wiedervorlage für den Vorgang beim Erreichen des Vorlagedatums storniert.

**Technische Info:** Toggle-Feld, DB-Feld: `vorlage.modus`

**Vorlage an Mitarbeiter**
Nummer des Mitarbeiters, der die Wiedervorlage erhält. Standardmäßig ist der Vorgangserfasser voreingestellt. Wenn Sie eine Nummer angeben, wird der Name des Mitarbeiters im Klartext angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: `vorlage.outmanr`

**Textfelder**
Felder für Informationstexte zum Vorgang, die zum Wiedervorlagezeitpunkt angezeigt werden. Wenn Sie eine vorgangsbezogene Wiedervorlage erfassen, wird vor dem ersten Textfeld die Nummer des Angebots angezeigt.
**Technische Info:** alphanumerische Felder, DB-Felder: `vorlage.text1`, `vorlage.text2`

## Fertigmeldung

**Pfad:** Verkauf > Fertigmeldung

*(Abb. D-179 Fertigmeldung: Screenshot des Dialogs "Fertigmeldung" mit einer Tabelle, die Auftragspositionen mit Gesamt-, Bisher- und Fertigmengen anzeigt.)*

In diesem Dialog können Sie Positionen zu einem Auftrag fertig melden.

In der Regel werden Fertigmeldungen aus der Produktion oder aus dem Einkauf gemeldet und müssen nicht manuell übermittelt werden.

- Mit `<F5>` löschen Sie die Positionen, deren gesamte Positionsmenge bereits fertig gemeldet ist. Bei den Positionen ist das Feld `Fertig` leer.
- Mit `<F3>` buchen Sie die Fertigmeldung.

### Kopfbereich

- **Haus:** Anzeige der Mandantennummer (Hausnummer).
  **Technische Info:** Anzeigefeld, DB-Feld: `kauf.hausnr`

- **Auftrag:** Auftragsnummer.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: `kauf.auftrnr`

- **Abteilg:** Nummer der Abteilung des Auftrag-Erfassers.
  **Technische Info:** numerisches Feld, DB-Feld: `kauf.abtnr`

- **Liefertermin:** Geplanter Liefertermin des Auftrags.
  **Technische Info:** Anzeigefeld, DB-Feld: `kauf.ltplan`

- **Fertigmeldung:** Datum im Format TT.MM.JJJJ, an dem der Auftrag fertig gemeldet werden soll. Standardmäßig ist das aktuelle Datum voreingestellt.
  **Technische Info:** Pflichtfeld, Datumsfeld, DB-Feld: `kauf.bdat`

### Übersicht

- **Auftrag:** Auftragsnummer.
  **Technische Info:** Anzeigefeld, DB-Feld: `kauf.auftrnr`

- **Pos:** Positionsnummer im Auftrag.
  **Technische Info:** Anzeigefeld, DB-Feld: `kpos.posnr`

- **Artikel:** Bezeichnung des Artikels aus der gewählten Position.
  **Technische Info:** Anzeigefeld, DB-Feld: `kpos.artnr`, `kpos.artbez1`

- **Gesamt:** Gesamtmenge der Position.
  **Technische Info:** Anzeigefeld, DB-Feld: `kpos.menge`

- **Bisher:** Bisher fertig gemeldete Menge der Position.
  **Technische Info:** Anzeigefeld, DB-Feld:

- **Fertig:** Menge der Position, die fertig gemeldet werden soll. Standardmäßig ist hier die Differenz aus der Gesamtmenge der Position und der bisher fertig gemeldeten Menge festgelegt. Sie können die Menge, die fertig gemeldet werden soll, bearbeiten.
  **Technische Info:** numerisches Feld, DB-Feld:

### Fußbereich

- **Buchen:** Bucht die Fertigmeldung.
- **Abbrechen:** Bricht die Fertigmeldung ab.

## Vorgangsänderung

**Pfad:** Verkauf > Vorgangsänderung

*(Abb. D-180 Vorgangsänderung: Screenshot des Dialogs "Vorgangsänderung" mit zwei Ansichten. Die erste zeigt eine Liste von Vorgängen (Auftrag, Lief., Angeb.) mit Status-Checkboxen. Die zweite Ansicht zeigt dieselben Vorgänge mit Versand- und Zollinformationen.)*

In diesem Dialog können Sie mehrere Vorgänge gleichzeitig korrigieren. Die Vorgänge können schneller korrigiert werden als in anderen Dialogen, da keine Zeit für das Laden eines gesamten Vorgangs benötigt wird. Korrekturen an Vorgängen können Sie nicht jederzeit durchführen, sie sind abhängig vom Positionsstatus.
⇨ "Positionsstatus und Positionskennzeichen" auf Seite D-76

Der Dialog hat eine zweite Ansicht, in der weitere Spalten der Tabelle angezeigt werden.

- **Mit `<F2>`** wechseln Sie zwischen den zwei Ansichten im Dialog.
- **Mit `<Strg>` + `<F10>`** suchen Sie nach Vorgängen mit Leistungserklärungen zu einem Liefertermin. Es werden alle Vorgänge mit Leistungserklärungen für den gesuchten Liefertermin angezeigt.
- **Mit `<Strg>` + `<F11>`** werden alle Sätze, ab dem aktuellen markiert.
- **Mit `<Strg>` + `<F8>`** importieren Sie die Daten für die Vorgangsänderung. Die Daten werden über eine frei konfigurierbare SQL-Abfrage importiert. Die Anzahl der importierten Daten ist von der jeweiligen SQL-Abfrage abhängig.
- **Mit `<F5>`** wird die Zusatzinformation zum Vorgang angezeigt, wenn eine hinterlegt ist.
- **Mit `<F3>`** lösen Sie die Buchung der Korrekturen aus.
- **Mit `<Shift>` + `<F5>`** wechseln Sie in die Auftragserfassung.
  ⇨ "Auftragserfassung" auf Seite D-82

### Tabelle (Ansicht 1)

- **Vorgang:** Art des Vorgangs.
  - Auftrag
  - Lief: Lieferung
  - Angeb: Angebot
  **Technische Info:** Toggle-Feld, DB-Feld: `zuaufint.vorgang`

- **Nummer:** Vorgangsnummer.
  **Technische Info:** numerisches Feld, DB-Feld: `zuaufint.auftrnr`

- **Subnr.:** Sub-Nummer des Vorgangs.
  **Technische Info:** Anzeigefeld, DB-Feld: `zuaufint.subr`

- **Info:** Anzeige, ob es Zusatzinformationen zu dem Vorgang gibt.
  - `(leer)`: Es gibt keine Zusatzinformationen.
  - `/`: Es gibt Zusatzinformationen.
  **Technische Info:** Anzeigefeld, Toggle-Feld

- **Lokale Korrekt.:** Information, ob sich der Vorgang im Status der lokalen Korrektur befindet. Der Hinweis wird nur angezeigt, wenn sich der Vorgang in diesem Status befindet. Das Feld ist gesperrt.
  **Technische Info:** Anzeigefeld, DB-Feld:

- **Sto.:** Stornierung. Angabe, ob der Vorgang storniert werden soll.
  - ☑ Der Vorgang wird storniert.
  - ☐ Der Vorgang wird nicht storniert.
  **Technische Info:** Checkbox, DB-Feld: `zuaufint.storno`

- **Haus:** Mandantennummer (Hausnummer), die dem Vorgang zugeordnet ist.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: `zuaufint.hnr`

- **Route:** Nummer der Versandroute.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: `zuaufint.route`

- **Termin:** Datum der geplanten Lieferung im Format TT.MM.JJJJ.
  **Technische Info:** Datumsfeld, DB-Feld: `zuaufint.ltideal`

- **PMS:** Angabe, ob der Vorgang an das Produktions-Management-System übergeben werden soll. Die Angabe ist nur gültig, wenn das Produktions-Management-System genutzt wird.
  - ☑ Der Vorgang wird an das Produktions-Management-System übergeben.
  - ☐ Der Vorgang wird nicht übergeben.
  **Technische Info:** Checkbox, DB-Feld: `zuaufint.pmsflag`

- **Vrs.:** Versandsteuerung. Angabe, ob der Vorgang an die Versandsteuerung übergeben werden soll.
  - ☑ Der Vorgang wird an die Versandsteuerung übergeben.
  - ☐ Der Vorgang wird nicht übergeben.
  **Technische Info:** Checkbox, DB-Feld: `zuaufint.lapoolflag`

- **Txt.:** Angabe, ob die Texte für den Vorgang neu generiert werden sollen.
  - ☑ Die Texte werden vom System neu generiert.
  - ☐ Die Texte werden vom System nicht neu generiert.
  **Technische Info:** Checkbox, DB-Feld: `zuaufint.txtflag`

- **WGR:** Angabe, ob die Warengruppenzuordnung für den Vorgang erneut erstellt werden soll.
  - ☑ Die Zuordnung wird für den Vorgang aktualisiert.
  - ☐ Die Zuordnung für den Vorgang wird nicht aktualisiert.
  **Technische Info:** Checkbox, DB-Feld: `zuaufint.wgrpflag`

- **Frei:** Angabe, ob der Vorgang freigeschaltet werden soll.
  - ☑ Der Vorgang wird freigeschaltet.
  - ☐ Der Vorgang wird nicht freigeschaltet.
  **Technische Info:** Checkbox, DB-Feld: `kauf.tekapkz`

### Tabelle (Ansicht 2, mit <F2>)

Mit `<F2>` werden folgende weitere Felder zum Dialog Vorgangsänderung angezeigt:

- **Auftrag:** Vorgangsnummer.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: `zuaufint.auftrnr`

- **Versandart:** Nummer der Versandart.
  **Technische Info:** numerisches Feld, DB-Feld: `zuaufint.sfill1`

- **Lieferart:** Nummer der Lieferart.
  **Technische Info:** numerisches Feld, DB-Feld: `zuaufint.sfill2`

- **A-Zoll:** Schlüsselnummer der Ausgangs-Zollstelle.
  **Technische Info:** numerisches Feld, DB-Feld: `zuaufint.sfill3`

- **B-Zoll:** Schlüsselnummer der Bestimmungs-Zollstelle.
  **Technische Info:** numerisches Feld, DB-Feld: `zuaufint.lfill1`

- **Versandinfo:** Firmeninterner Informationstext zum Versand.
  **Technische Info:** alphanumerisches Feld, DB-Feld: `zuaufint.cfill1`

- **LE:** Angabe, ob eine Leistungserklärung vorliegt.
  - ☑ Es liegt eine Leistungserklärung vor.
  - ☐ Es liegt keine Leistungserklärung vor.
  **Technische Info:** Checkbox

## Übersicht zu Vorgängen

**Pfad:** Verkauf > Übersicht > Unberechnete Aufträge, Ungebuchte Rechnungen, Unvollständige Lieferungen, Aufträge mit Fakturasperre > Datum eingeben > [OK]

*(Abb. D-181: Collagen von Screenshots verschiedener Übersichtsfenster wie "Unberechnete Aufträge", "Ungebuchte Rechnungen" und "Aufträge mit Fakturasperre", die jeweils Listen von Aufträgen mit Details wie Kunde, Datum und Wert anzeigen.)*

In diesen Dialogen werden die Übersichten zu folgenden Vorgängen im gewählten Zeitraum angezeigt:

- **Unberechnete Aufträge:**
  Zeigt alle Aufträge an, zu denen noch keine Rechnung erstellt wurde.
- **Ungebuchte Rechnungen:**
  Zeigt alle Vorgänge an, zu denen eine Rechnung erstellt ist, die noch nicht gebucht wurde.
- **Unvollständige Lieferungen:**
  Zeigt alle Vorgänge an, bei denen noch unvollständige Lieferungen ausstehen.
- **Aufträge mit Fakturasperre:**
  Zeigt alle Aufträge an, für die die Rechnungsstellung gesperrt ist.

Wenn Sie eine der Übersichten öffnen wollen, müssen Sie zunächst in einem Dialog das Startdatum der Suche eingeben. Wenn Sie kein Datum angeben, werden in der Übersicht alle entsprechenden Vorgänge angezeigt.

Die Anzeige der Spalten ist frei konfigurierbar und hängt von der kundenindividuellen Formatierung der jeweiligen SQL-Abfrage ab.

Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

## Vertrieb

Im Vertrieb werden Ihnen Informationen zur Akquise und Provisionsberechnung angezeigt und Sie können die Objektbudgetierung verwalten.

Alle Dialoge, die Sie über den Menüpunkt Vertrieb öffnen können, sind kundenindividuelle Programmanpassungen.

Für weitere Informationen zu diesem Bereich kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

## Index

### A
- **Abschlagsrechnung**
  - buchen D-348, D-350
- **Abzugsmaß**
  - Stufen D-225
- **Adresse**
  - neue Lieferadresse D-138
  - suchen D-47
- **Allgemein**
  - Position im Auftrag D-113
- **Angebot**
  - Datei zuordnen D-169
  - erfassen D-80
  - Information D-399
- **Anmerkungen**
  - zu Artikeln D-248
  - zu Kundenartikeln D-251
  - zu Lieferantenartikeln D-251
  - zu Marktpartnern D-248
  - zu Objektartikeln D-251
  - zu Objekten D-248
  - zu Vorgängen D-247
- **Anmerkungstext** D-245
- **Anschrift**
  - Auftrag D-90
  - siehe auch Adresse
- **Ansprechpartner** D-144
- **Anzahlung**
  - erfassen, prüfen D-179
- **Anzeige**
  - Angebot D-399
  - Auftragsinformation D-398
  - Modus im Auftrag D-76
  - Positionskennzeichen im Auftrag D-76
  - Status im Auftrag D-76
  - Vorgangsänderung D-403
  - Vorgangsübersicht D-406
- **Artikel**
  - fixieren D-161
  - suchen D-49
  - Texte drucken D-98
  - verdeckte Maßangabe D-150
- **Artikelsuche**
  - Artikelcodes D-55
  - Bezeichnungen D-53
  - Details D-56
  - nach Typen D-58
- **Auftrag**
  - Allgemeines zur Position D-113
  - Änderungs-Protokoll D-173
  - Anschrift D-90
  - Auslieferungsdetails D-102
  - Austauschpreis D-274, D-304
  - Autorisierung D-324
  - Bezugnahme D-84
  - CAD-Datei D-129
  - CE-Kennzeichen D-129
  - Datei zuordnen D-169
  - Direkte Suche D-29
  - Druckoption D-96
  - Eigenschaft der Position D-126
  - Eigenschaften D-93
  - Eilauftrag D-97
  - erfassen D-82
  - Fakturasperre D-97
  - festbemaßtes Produkt D-121
  - freischalten D-321
  - Kistensignatur D-261
  - Konditionen D-264
  - Kopf-, Fußbereich D-83
  - Kosten der Position D-136
  - Leistungserklärung D-186
  - Leistungsmerkmal D-190
  - Leistungserklärung hinterlegen D-129
  - Lieferadresse bearbeiten D-92, D-138
  - Lieferant zuweisen D-118
  - Lieferplan D-327
  - Lieferschein D-333, D-335
  - Mitarbeiterzuordnung D-93
  - Modusanzeige D-76
  - Nachkalkulation D-277
  - Position erfassen D-113, D-121
  - Preis der Position D-131
  - Preis überschreiben D-269
  - preislos D-81
  - Private Felder D-101
  - Produktionskosten D-313
  - Rabatte D-104
  - Rabatte, Detailansicht D-108
  - Rechnungsoption D-96
  - Reklamationsinformation D-99
  - Sammelrechnung D-96
  - schnell erfassen D-79
  - Status der Position D-134
  - Statusanzeige D-76
  - Storno D-145
  - suchen D-25
  - suchen - Trefferliste D-30
  - suchen über Positions-Schlüssel D-28
  - Summen D-104
  - Technische Werte D-119
  - Teilfaktura D-97
  - Teillieferung D-97
  - Unterteilpreis D-276
  - Versandinformation D-94
  - Verschiedenes D-99
  - Zahlungsoption D-100
- **Auftragsarten** D-159
- **Auftragsinformation**
  - Einkauf D-370
  - Lager D-378, D-379
  - Position D-369
  - Produktion D-373
  - Produktionsrückmeldung D-380
  - verbundene Produktion D-380
  - Versand D-375
  - Vorgang D-368
  - Wareneingang D-372
  - Zwischenversand D-381
- **Auftragskondition**
  - für Basisglas D-282
  - für ESG D-286
  - für Farbartikel D-297
  - für Glastüren D-300
  - für ISO D-288
  - für ISO (Schweiz) D-293
  - für PKZ-Preise D-298
  - für Veredelung D-282
  - für VSG D-286
  - in Position D-281
  - manuelle Preise D-303
- **Auftragsstatus**
  - Info D-367
- **Auftragssuche**
  - nach Werteingaben D-71
- **Auslieferung**
  - Auftrag, Details im D-102
- **Autorisierung**
  - Auftrag D-324

### B
- **Bearbeitung**
  - DXF-Datei importieren D-172
  - Position D-218
  - Preis drucken D-98
  - Wiedervorlage D-400
- **Bearbeitungspreis**
  - Position D-307
- **Berechtigungsgruppe**
  - suchen D-43
- **Bestandsprognose**
  - Lagerartikel D-151
- **Bezug**
  - suchen D-45
- **Bezugnahme**
  - Auftrag D-84
- **Bohrpunkt**
  - Parameter bearbeiten D-232
- **Bruttopreis**
  - drucken D-97
- **Buchen**
  - Abschlagsrechnung D-348, D-350
  - Gutschrift D-356
  - Rechnung D-339, D-344, D-346
  - Schlussrechnung D-351, D-352
  - Thekenrechnung D-345

### C
- **CAD-Datei**
  - Auftrag D-129
- **CE-Kennzeichen**
  - Auftrag D-129

### D
- **Datei**
  - im Vorgang zuordnen D-169
- **Dateizuordnung**
  - Motiv für Bearbeitung D-171
- **Dickenvarianten** D-164
- **Dokumentenarten**
  - Ausgabeart D-168
- **Druck**
  - Artikeltexte D-98
  - Bearbeitungspreis D-98
  - Bruttopreis D-97
  - drucken D-365
  - Floskel D-258
  - Formular D-359
  - Fremdinformation D-260
  - Kundenfaktor D-97
  - Liste D-366
  - Modellskizze D-98
  - Option im Auftrag D-96
- **DXF**
  - für Bearbeitung D-172

### E
- **Eigenschaft**
  - Position im Auftrag D-126
- **Eilauftrag** D-97
- **Einkauf**
  - Status D-370
- **Einstand**
  - Stufenerfassung D-221
- **E-Mail**
  - versenden D-363
- **Endkundenanschrift**
  - erfassen D-140

### F
- **Fakturasperre**
  - Auftrag D-97
- **Farbvarianten** D-164
- **Fertigmeldung** D-401
- **Festbemaßtes Produkt**
  - Artikelangaben für bemaßte Variante D-161
  - Auftrag D-121
  - kundenindividuell D-162
  - lieferantenindividuell D-163
- **Floskel**
  - Druck D-258
- **Formular**
  - Ausgabeform D-365
  - Direktdruck D-358
  - Druck D-359
  - E-Mail D-363
- **Formularausgabe** D-168
- **Freischalten**
  - Auftrag D-321
- **Fremddaten importieren** D-166
- **Fremdinformation**
  - Druck D-260
- **Fehler** D-183

### G
- **Grafische Darstellung**
  - Produktaufbau D-121
- **Gutschrift**
  - buchen D-356
  - erfassen D-354

### H
- **Haus suchen** D-137
- **Hauswechsel** D-137
- **Historie**
  - Vorgang D-368

### I
- **Import von Fremddaten** D-166
- **Information**
  - Anmerkungstext D-245
  - Auftragsanzeige D-398

### K
- **Kantenzuordnung** D-217
- **Kapazitätsübersicht** D-185
- **Kistensignatur** D-261
- **Kommission** D-115
- **Kondition**
  - Auftrags- D-264
  - Preiskalkulation D-320
- **Konfigurierbare Felder** D-146
- **Kosten**
  - Position im Auftrag D-136
  - Kosten der Verglasung D-98
- **Kundenartikel**
  - Produktsuche D-62
- **Kundenindividuelles Produkt**
  - Produktaustausch D-154

### L
- **Lager**
  - Auftragsinformation D-378, D-379
  - Status D-378, D-379
- **Lagerartikel**
  - Bestandsprognose D-151
- **Leistungserklärung**
  - Auftrag, hinterlegen im D-129
  - techn. Werte anpassen D-187
  - zuordnen D-186
- **Lichtes Feld** D-233
- **Lieferadresse**
  - bearbeiten D-92, D-138
- **Lieferant**
  - zuweisen, im Auftrag D-118
- **Lieferinformation** D-329
- **Lieferplan**
  - Auftrag D-327
- **Lieferschein**
  - Auftrag D-333, D-335
  - Protokoll D-337
- **Liefertermin**
  - Änderungs-Protokoll D-175
- **Lieferung**
  - Details D-329
  - Lieferplan D-327
- **Liste**
  - Druck D-366

### M
- **Marktpartner**
  - Ansprechpartner D-144
  - Information D-142
  - suchen D-39
- **Maßangabe**
  - Stückliste D-219
- **Maßangaben**
  - erfassen, verdeckte D-120
- **Menü**
  - Adressen D-18
  - Auftragspreise D-20
  - Infomenü D-22
  - Preisangaben D-19
  - Produktangaben D-20
  - Rechnungen D-15
  - Spezielle Texte D-19
  - Technische Werte D-21
  - Texte D-18
  - Verkauf D-14
  - Zusatzmenü D-16
- **Mitarbeiter**
  - suchen D-43
- **Mitarbeiterzuordnung** D-146
  - Auftragserfassung D-93
- **Modell**
  - Katalog D-176
  - Maßangaben D-177
  - Skizze drucken D-98
- **Modus**
  - Auftrag, Anzeige im D-76
- **Motiv**
  - für Bearbeitung zuordnen D-171

### N
- **Nachkalkulation**
  - Auftrag D-277

### O
- **Objekt**
  - suchen D-66
- **Objektsuche**
  - Adressen D-69
  - Identifikatoren D-70

### P
- **Packmittel**
  - Sortierung D-238
  - Vorgaben D-236
- **Packmittelplanung** D-242
- **Position**
  - Auftragsinformation D-369
  - erfassen D-121
  - Grafische Darstellung D-121
  - im Auftrag D-113
  - Konditionen D-281
  - Kosten D-136
  - Preis D-131
  - Status D-134, D-369
- **Positionskennzeichen**
  - Anzeige im Auftrag D-76
- **Positionskondition**
  - Bearbeitungspreis D-307
  - Sprossenpreis D-310
- **Positionspreise**
  - unterdrücken D-98
- **Positionsübersicht**
  - Vorgang D-394
- **Preise**
  - Auftrag, überschreiben im D-269
  - Austausch im Auftrag D-274
  - Austausch zum Auftrag D-304
  - Kalkulation D-320
  - Nachkalkulation im Auftrag D-277
  - Position im Auftrag D-131
  - Sprossen im Auftrag D-271
  - Stufenpreise D-280
  - Unterteile im Auftrag D-276
- **Preislose Erfassung** D-81
- **Private Felder** D-165
  - im Auftrag D-101
- **Produkt**
  - Aufbau ändern D-155
- **Produktaustausch**
  - kundenindividuelles Produkt D-154
  - Positionen D-157
- **Produktion**
  - Auftragsinformation D-373
  - Status D-373
- **Produktionskosten**
  - Auftrag D-313
  - Kalkulation D-313
- **Produktionsmonitor** D-185
- **Produktionsskizze** D-200
- **Produktmerkmale deklarieren** D-190
- **Produktsets (Sash Master)** D-148
- **Produktsuche**
  - nach Bezeichnungen D-64
  - nach Elementen D-59
  - nach Kundenartikeln D-62
  - nach Techn. Werten D-65
- **Produkttausch**
  - Produktaufbau ändern D-155
- **Protokoll**
  - Auftrags- D-173
  - Lieferschein D-337
  - Liefertermin D-175
  - Rechnung D-353

### R
- **Recherche**
  - Details zum Vorgang D-389, D-392
  - Mitarbeiter zum Vorgang D-388
  - Positionen im Vorgang D-394
  - Positionsdetails D-396
  - Übersicht Positionen D-394
  - Übersicht Vorgänge D-386
  - Vorgang D-382
- **Rechnung**
  - Abschlagsrechnung automatisch D-348
  - Abschlagsrechnung manuell D-350
  - automatisch erstellen D-339
  - buchen D-339, D-344, D-346
  - manuell erstellen D-344
  - Positionsinfo D-342
  - Protokoll D-353
  - Schlussrechnung automatisch D-351
  - Schlussrechnung manuell D-352
  - Thekenrechnung D-345
  - Zahlungsplan D-181
- **Rechnungsoption**
  - Auftrag D-96
- **Reklamation** D-158
- **Reklamationsinformation**
  - Auftrag D-99

### S
- **Sammelrechnung**
  - Auftrag, im D-96
- **Sash Master (Produktsets)** D-148
- **Schlussrechnung**
  - bearbeiten D-181
  - buchen D-351, D-352
- **Schnellerfassung** D-79
- **Sprossen**
  - Abschnitte bearbeiten D-233
  - Artikel bearbeiten D-230
  - Aufteilung bearbeiten D-234
  - Editor D-231
  - Konstruktion bearbeiten D-231
  - Preise im Auftrag D-271
- **Sprossenerfassung** D-226
- **Zusatzinfo** D-229
- **Sprossenpreis** D-310
- **Status**
  - Auftrag, Anzeige im D-76
  - Einkauf D-370
  - Lager D-378, D-379
  - Position D-369
  - Position im Auftrag D-134
  - Produktion D-373
  - Versand D-375
  - Wareneingang D-372
  - Zukaufteil D-370
- **Storno** D-145
- **Stückliste**
  - Adressen D-208
  - Bearbeitungsparameter D-207
  - Darstellung D-195
  - Einbauposition D-197
  - Maßangabe D-219
  - Parameter D-209
  - Produktaufbau D-199
  - Produktionsskizze D-200
  - Sprossen D-230
  - Stücklistenaufbau D-196
  - Stücklistenebene D-202
- **Stufenerfassung** D-223
  - Abzugsmaß D-225
  - Einstand D-221
- **Stufenpreise**
  - im Auftrag D-280
- **Suche**
  - Adresse D-47
  - Artikel D-49
  - Auftrag D-25
  - Berechtigungsgruppe D-43
  - Bezug D-45
  - erweiterte, Werteingabe D-71
  - Marktpartner D-39
  - Mitarbeiter D-43
  - Objekt D-66
  - Produkt, nach Elementen D-59
  - Vorgang D-25
- **Symbole** D-76

### T
- **Technische Werte**
  - im Auftrag D-119
  - im Auftrag anpassen D-187
- **Teilfaktura**
  - Auftrag D-97
- **Teillieferung**
  - Auftrag D-97
