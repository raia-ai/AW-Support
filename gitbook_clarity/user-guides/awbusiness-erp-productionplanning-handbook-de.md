---
description: "A+W Business Software - Production, Delivery, and Rack Management"
---


# Produktionsdaten

---
## Produktionsdaten – Buchung

**Fertigung > Produktion > Produktionsdaten > Register Buchung**

*Abb. E-98 Produktionsdaten - Buchung*

In diesem Register können Sie die erfassten Daten verbuchen. Die Daten werden in komprimierter Form pro Aggregat (Maschine) angezeigt.

Die Buchung wird nur für die Einträge ausgeführt, die im Zeilenkopf mit einem x markiert sind. Mit der Verbuchung werden die Rohmaterialien vom Lager ab- und die produzierten Positionen zugebucht.

# Lieferwesen

**Fertigung > Lieferwesen**

Sie können die Lieferung von produzierten Aufträgen planen und steuern, indem Sie Aufträge nach Touren, Datum, Gestell usw. zusammenfassen.

In diesem Abschnitt finden Sie Informationen zu folgenden Dialogen des Programmbereichs:
- "Tourenliste" auf Seite E-2505
- "Statusmeldung und Packmittelzuordnung" auf Seite E-2518
- "Kommissionierung" auf Seite E-2528
- "Listendruck" auf Seite E-2533
- "Warenausgang Kisten" auf Seite E-2537

## Tourenliste

**Fertigung > Lieferwesen > Tourenliste**

Mit Hilfe der Tourenliste können Sie den Versand planen. Die Liste können Sie sich nach verschiedenen Auswahlkriterien anzeigen und ausdrucken lassen, z. B. nach Liefertermin, Tour, Status.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menüs im Dialog Tourenliste" auf Seite E-2503
- "Tourenliste" auf Seite E-2505
- "Versanddaten ändern" auf Seite E-2514
- "Einstellungen (KAPS-Datei)" auf Seite E-2515

### Menüs im Dialog Tourenliste

Über die Menüs im Dialog Tourenliste können Sie die Standardeinstellung des Dialoges bestimmen und andere Dialoge öffnen, ohne die Tourenliste zu schließen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite E-2503
- "Menü Optionen" auf Seite E-2504

### Menü Funktionen

**Fertigung > Lieferwesen > Tourenliste**

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Tourenliste zu schließen.

**Gruppe Tour**

- **Historie:**
  Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des markierten Dokuments.
  ⇨ Verkauf, "Historie" auf Seite C-1834
- **Teillieferung:**
  Öffnet den Dialog Dokumente kopieren im Modus Teillieferung, in dem Sie eine Teillieferung erstellen können.
  ⇨ Verkauf, "Dokumente kopieren" auf Seite C-1813
- **Versanddaten ändern:**
  Öffnet den Dialog Touren/Liefertermine umsetzen, in dem Sie die Tour und/oder den Liefertermin ändern können.
  ⇨ "Versanddaten ändern" auf Seite E-2514
- **Selektierte, Alle in Nummernverwalter kopieren:**
  Öffnet den Dialog NV Auswahl, in dem Sie alle Aufträge in einen anderen Nummernverwalter stellen können.
  ⇨ Verkauf, "NV Auswahl" auf Seite C-1838

### Gruppe Navigation

- **Vorheriger Tag/Tour, Nächster Tag/Tour:**
  Wechselt die Darstellung in der Übersicht im Register Tabelle.

### Gruppe KAPS

- **Datei erstellen:**
  Mit dieser Funktion starten Sie die Erstellung der KAPS-Datei. Wenn sich sehr viele Aufträge im gewählten Nummernverwalter befinden, kann dieser Vorgang einige Zeit in Anspruch nehmen.
- **Pfad für Datei:**
  Öffnet einen Dialog zum Festlegen des Speicherorts.
  ⇨ "Einstellungen (KAPS-Datei)" auf Seite E-2515

### Gruppe Sonstiges

- **Einstellungen:**
  Dieser Eintrag ist nur kundenspezifisch freigeschaltet. Über ihn können die Höchstmaße des Glases für die Tourenliste festgelegt werden.
- **Dokument anzeigen:**
  Öffnet die Vorschau auf das Dokument.

### Menü Optionen

**Fertigung > Lieferwesen > Tourenliste**

Über dieses Menü können Sie die Standardeinstellung für den Druck bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

**Gruppe Tabelle**

- **Mehrere Zeilen selektierbar:**
  Mit dieser Option können Sie in der Übersicht mehrere Zeilen markieren, wenn Sie die Taste <Strg> gedrückt halten.

**Gruppe Druckoptionen**

- **Name des Lieferanten:**
  Der Name des Lieferanten wird auf der Tourenliste gedruckt. Diese Option ist sinnvoll, wenn in der Lieferung Bestellartikel enthalten sind.
- **Ersten Positionstext:**
  Der Positionstext 1 aus dem Auftrag wird auf der Tourenliste gedruckt.
- **Produktbezeichnung 1 - 3:**
  Die Produktbezeichnungen 1 - 3 werden auf der Tourenliste gedruckt.
- **Bleiverglasung:**
  Scheiben mit Bleiverglasung werden auf der Tourenliste gekennzeichnet, damit der Versand die Scheiben entsprechend verpackt.
- **Zuschlags- und Leistungspositionen:**
  Zuschläge und Leistungen werden auf der Tourenliste gedruckt.

## Tourenliste (Dialog)

**Fertigung > Lieferwesen > Tourenliste**

> **i Angaben auf der Tourenliste nicht gedruckt**
> Wenn Sie sehr viele Optionen für den Druck der Tourenliste gewählt haben, sollten Sie im Drucker-Dialog die Einstellung Querformat wählen. Die gewünschten Spalten werden sonst nicht auf dem Bildschirm oder in der Liste dargestellt.

Mit Hilfe der Tourenliste können Sie den Versand planen. Die Aufträge einer Tour können Sie sich nach verschiedenen Auswahlkriterien zusammenstellen, z. B. nach Liefertermin, Produkt, Status.

In diesem Dialog finden Sie folgende Register:
- "Tourenliste - Selektion" auf Seite E-2506
- "Tourenliste - Tabelle" auf Seite E-2510

### Tourenliste – Selektion

**Fertigung > Lieferwesen > Tourenliste > Register Selektion**

*Abb. E-99 Tourenliste - Selektion*

In diesem Register legen Sie die Kriterien fest, nach denen die Tour zusammengestellt werden soll.

**Kriterien**

Mit der Wahl der Option legen Sie fest, nach welchen Kriterien die Touren angezeigt werden sollen.

- **Versand:** Das angegebene Datum betrifft den Versandtag.
- **Anlieferung:** Das angegebene Datum betrifft den Tag der Anlieferung beim Kunden.

**(Termin) von ... bis** Diese Felder sind nur freigeschaltet, wenn Sie keinen Nummernverwalter ausgewählt haben. Sie können dann Touren nach einer gewünschten Zeitspanne zusammenstellen.
Wenn Sie einen Nummernverwalter gewählt haben, sind die Felder gesperrt und das aktuelle Tagesdatum wird angezeigt.

**Tourenstamm** Mit der Wahl dieser Option legen Sie fest, welche Touren im Feld Verfügbare Touren angezeigt werden.
- **Stammdaten:** Alle Touren aus A+W Business werden angezeigt.
- **Routenoptimierung:** Alle optimierten Routen aus OTR werden angezeigt.

**Verfügbare Touren** In der Liste werden alle Touren angezeigt, die in den Stammdaten angelegt sind. Touren, die in das Feld Anzuzeigende Touren/Reihenfolge übernommen wurden, werden in der Liste nicht mehr angezeigt.

**Anzuzeigende Touren / Reihenfolge** In der Liste werden alle Touren angezeigt, zu denen Tourenlisten zusammengestellt werden sollen. Die Reihenfolge der Touren kann mit den Pfeilschaltflächen unter dem Feld geändert werden.

**Status von, Status bis** Sie können einen Anfangs- und einen End-Status einstellen, um nur die Aufträge auszuwählen, die diesen Kriterien entsprechen. Die Felder sind gesperrt, wenn Sie einen Nummernverwalter ausgewählt haben.

**Nummernverwalter** Sie können die Aufträge für die Tourenplanung vorab in einem Nummernverwalter zusammenstellen.
- ☐ Die Aufträge werden nicht aus einem Nummernverwalter angezeigt.
- ☑ Die Tourenlisten sollen aus den Aufträgen in einem Nummernverwalter zusammengestellt werden. Das Feld zur Auswahl des Nummernverwalters wird freigeschaltet.

**AV-Bereiche** Sie können als zusätzliches Kriterium einen oder mehrere AV-Bereiche auswählen. Für die Mehrfachauswahl halten Sie die Taste <Strg> gedrückt.

**Auflösungstiefe**

Mit der Wahl der Option legen Sie fest, wie die Liste auf dem Monitor und im Druck ausgegeben werden soll:
- **Auftrag:** Nur die Auftragsnummern werden angezeigt bzw. gedruckt.
- **Position:** Die Auftrags- und die Positionsnummern werden angezeigt bzw. gedruckt.

Wenn Sie den Liefertermin gewählt und bestätigt haben, können Sie die Einstellungen im Register Tabelle prüfen.

**Inklusive Bearbeitungen** Unabhängig von der Option zur Auflösungstiefe können Sie festlegen, ob Bearbeitungen angezeigt werden sollen.
- ☐ Bearbeitungen werden nicht ausgegeben.
- ☑ Bearbeitungen werden in der Tourenliste mit einem X in der Spalte Bearb. angezeigt.

**Sortierung innerhalb der Touren**

Mit der Wahl der Option legen Sie fest, wie die Reihenfolge der Lieferungen innerhalb einer Tour sortiert werden soll.
- **AV-Bereich/Rangfolge/Kundennummer:** Die Lieferungen werden zunächst nach AV-Bereichen sortiert. Innerhalb des AV-Bereiches wird die Tour nach der Rangfolgenummer sortiert, die in den Stammdaten der jeweiligen Kunden eingetragen ist.
- **Kundennummer/Status:** Die Lieferungen werden zunächst nach Kundennummern und dann nach Status sortiert. Diese Option ist dann sinnvoll, wenn in den Stammdaten keine Rangfolgenummern eingetragen sind.
- **Rangfolge/Kundennummer:** Die Lieferungen werden zunächst nach der Rangfolgenummer und dann nach Kunden sortiert.
- **Kundennummer/Lieferanschrift (PLZ, Ort, Str.):** Die Lieferungen werden zunächst nach Kundennummern und dann nach Lieferanschrift sortiert.
- **Routenoptimierung:** Die Lieferungen werden nach Routenoptimierung sortiert. Diese Option ist nur freigeschaltet, wenn beim Feld Tourenstamm die Option Routenoptimierung gewählt ist.

**Seitenwechsel bei Druck**

Mit der Wahl der Option legen Sie fest, wie die Liste gedruckt werden soll. Die Wahl richtet sich auch nach den Kriterien, mit denen Sie die Tourenliste zusammengestellt haben.
- **Tour/Datum:** Beim Wechsel der Tour und/oder des Datums wird eine neue Seite gedruckt.
- **Tour/Datum/Kunde:** Für jede Tour wird pro Datum und Kunde eine neue Seite gedruckt.
- **Kein Wechsel:** Die Tourenliste wird ohne Seitenwechsel gedruckt.
- **Tour/Datum/Kunde/Lieferanschr.:** Für jede Tour wird pro Datum und Kunde und Lieferanschrift eine neue Seite gedruckt.

**Auszuschließender Status bei Druck**

Sie können Aufträge mit einem bestimmten Status vom Druck ausschließen. Für die Mehrfachauswahl brauchen Sie keine Taste zu drücken. Diese Einstellung ist sinnvoll, wenn Sie die Touren nach Liefertermin zusammenstellen.
Wenn Sie eine Auswahl getroffen haben, werden die entsprechenden Aufträge im Register Tabelle in blauer Schrift dargestellt.

**Optionen**

**Druck von ausgewählter Tour/Datum** Sie können den Druck auf die aktuell angezeigte Tour begrenzen.
- ☐ Alle Touren zum eingestellten Datum oder aus dem gewählten Nummernverwalter werden gedruckt.
- ☑ Nur die im Register Tabelle ausgewählte Tour wird gedruckt.

**Ohne Direktanlieferung** Sie können den Druck von Auftragspositionen ausschließen, die direkt von Lieferanten geliefert werden.
- ☐ Alle Auftragspositionen zur ausgewählten Tour werden gedruckt.
- ☑ Auftragspositionen mit Direktanlieferung werden nicht gedruckt.

**NV komplett füllen** Sie können die Aufträge einer Tourenliste in einen bestimmten Nummernverwalter stellen.
- ☐ Kein Nummernverwalter wird gefüllt.
- ☑ Die Aufträge der Tourenlisten werden in einen Nummernverwalter gestellt. Sie können einen Nummernverwalter auswählen oder einen neuen Nummernverwalter anlegen, indem Sie den Namen eintragen. Diese Einstellung ist sinnvoll, wenn Sie nach der Kommissionierung Listen drucken wollen.
  ⇨ "Listendruck" auf Seite E-2533

**NV löschen** Sie können die Aufträge einer Tourenliste aus einem Nummernverwalter löschen. Die Checkbox ist nur freigeschaltet, wenn Sie die Checkbox NV komplett füllen markiert haben.
- ☐ In dem gewählten Nummernverwalter werden keine Aufträge gelöscht.
- ☑ Im gewählten Nummernverwalter werden alle Aufträge gelöscht, so dass nur die neuen Aufträge darin stehen. Diese Einstellung ist sinnvoll, wenn Sie immer denselben Nummernverwalter verwenden wollen.

### Tourenliste – Tabelle

**Fertigung > Lieferwesen > Tourenliste > Register Tabelle**

*Abb. E-100 Tourenliste - Tabelle (Auflösungstiefe Auftrag)*

In diesem Register werden alle Aufträge aufgelistet, die den Auswahlkriterien im Register Selektion entsprechen. Sie können die Tourenliste in unterschiedlichen Sortierungen für den Druck anzeigen lassen.

Wenn Sie im Register Selektion > Auszuschließender Status bei Druck eine Auswahl getroffen haben, werden die entsprechenden Aufträge in blauer Schrift dargestellt.

In der Auflösungstiefe Position werden die Kopfdaten in roter Schrift angezeigt.

**Auswahl**

- **Datum Tour:** In diesem Feld können Sie jede Tour pro Datum auswählen. Aufgelistet werden nur die Touren, die den Auswahlkriterien entsprechen.
- **[<], [>]**: Mit diesen Schaltflächen können Sie die Liste der Touren im Feld Datum Tour durchblättern.
- **Vorschau:** In diesem Feld werden die Termine und/oder Lieferungen angezeigt, die zur ausgewählten Tour gehören. Mit der Wahl der Option können Sie die Vorschau ändern:
    - **Nach Datum:** In der Vorschau werden alle Touren zum gewählten Datum angezeigt.
    - **Nach Tour:** In der Vorschau werden zur gewählten Tour alle Termine für 14 Tage im Voraus angezeigt. Anhand der Spalten Menge, Fläche und Gewicht können Sie prüfen, ob ein Lkw genügend ausgelastet ist. Ist die Auslastung eines Lkws z. B. nicht ausreichend, kann in der Übersicht nach einer anderen Tour gesucht werden. Dazu müssen die Fahrzeuge in den Stammdaten angelegt sein. Darüber hinaus wird Ihnen der Netto-Verkaufspreis sowie die Anzahl der Lieferstellen angezeigt. Die Felder können in der Bildschirmtabelle ein- und ausgeblendet werden. ⇨ Stammdaten, "Lkw" auf Seite B-998
- **[Alle], [Keine]:** Mit diesen Schaltflächen können Sie alle Lieferungen in der Übersicht markieren oder an allen die Markierung entfernen.

Sie können die Tour und/oder das Lieferdatum der angezeigten Aufträge ändern. Dazu müssen die Aufträge markiert werden. Sie können einzelne Einträge in der Übersicht mit einem Doppelklick in den Zeilenkopf markieren. Sie können beliebig viele Einträge markieren.
⇨ "Versanddaten ändern" auf Seite E-2514

> **i Markieren**
> Ein Auftrag ist erst dann markiert, wenn im Zeilenkopf ein x angezeigt wird.

- **[Tabelle neu sortieren nach...]**: Mit dieser Schaltfläche sortieren Sie die markierten Lieferungen in der Übersicht nach der gewählten Option im Register Selektion. ⇨ "Tourenliste - Selektion" auf Seite E-2506

**Legende**

- **Blau:** Dokumente werden nicht gedruckt.
- **Rot:** Dokumente werden gedruckt.

**Übersicht**

In der Übersicht werden alle Aufträge zu einer Tour und einem Liefertermin aufgelistet. Die Übersicht wird automatisch aktualisiert, wenn Sie mit den Pfeil-Schaltflächen oder im Feld Datum Tour eine andere Tour wählen.
Die Spalten werden je nach Auflösungstiefe gefüllt. Die Einträge in blauer Schrift werden auf der Liste nicht gedruckt, z. B., weil ihr Status vom Druck ausgeschlossen ist.

- **Kunde:** Name des Kunden aus dem Auftrag.
- **Auftrag:** Auftragsnummer.
- **Menge:** Gesamtstückzahl des Auftrags.
- **Pos:** Diese Spalte wird nur angezeigt, wenn als Auflösungstiefe die Option Position gewählt wurde. Die folgenden Spalten werden dann pro Position dargestellt.
- **Fläche:** Gesamtfläche des Glases pro Auftrag oder Position.
- **Gewicht:** Gesamtgewicht pro Auftrag oder Position.
- **Status:** Status des Auftrags.
- **Lieferanschrift:** Anzeige einer abweichenden Lieferanschrift aus dem Auftrag. Je nach Auflösungstiefe wird zusätzlich auch die Produktbeschreibung angezeigt.
- **Kommission:** Kommission der ersten Position des Auftrags.
- **Mod.:** Modellnummer für eine Position mit Modell.
- **Rang:** Tourrangfolge aus den Kundenstammdaten.
- **Erf. Datum:** Erfassungsdatum des Auftrags.
- **QM/Position:** Gesamtfläche der Position.
- **Gewicht/Position:** Gesamtgewicht der Position.
- **Bearb.:** Bearbeitungen. Wenn im Register Selektion die Auflösungstiefe auf Positionsebene gewählt wurde, wird hier mit einem x gekennzeichnet, wenn in der Position Bearbeitungen enthalten sind.
- **AV-Bereich:** Name des AV-Bereichs, dem der Auftrag zugeordnet ist.
- **Bearbeitungen:** Nummer der Produktgruppe der einzelnen Bearbeitungen. Die Nummern sind durch ein Semikolon (;) getrennt.
- **Teillieferung:** Auftragsnummer der Teillieferung.
- **Haupt-Auftrag:** Nummer des Auftrags, zu dem der angezeigte Auftrag eine Teillieferung darstellt.
- **Dokumententyp:** Ein Dokumententyp wird nur angezeigt, wenn er vom Auftrag abweicht, z. B. Reklamation.
- **Summe:** Gesamtsumme der aufgelisteten Lieferungen für Menge, Fläche und Gewicht.

**Gesamt**

Anzeige der Summen über alle Aufträge, die in der Übersicht angezeigt werden.

**Beispiel: Gedruckte Tourenliste**

*Abb. E-101 Tourenliste als Bildschirmausgabe*

### Versanddaten ändern

**Fertigung > Lieferwesen > Tourenliste > Menü Funktionen > Gruppe Tour > Versanddaten ändern**

*Abb. E-102 Versanddaten ändern*

In diesem Dialog können Sie die Tour, den Liefertermin, die Lieferbedingungen von Aufträgen, den Fahrer und/oder den LKW der Tour ändern. Im Dialog werden alle Aufträge angezeigt, die Sie im Dialog Tourenliste – Tabelle markiert haben.

**Markierte Aufträge**

In der Übersicht werden alle Aufträge angezeigt, die Sie im Dialog Tourenliste - Tabelle markiert haben.

**Änderung von**

Änderungen gelten immer für alle angezeigten Aufträge. Mit der Wahl der Option legen Sie fest, was geändert werden soll:

- **Liefertermin:** Sie können ein anderes Datum aus der Liste eintragen.
- **Tour:** Sie können eine andere Tour aus der Liste auswählen.
  - ☐ Die Tour wird nicht geändert.
  - ☑ Die ausgewählte Tour wird für die Aufträge übernommen.
- **Lieferbed.:** Sie können eine andere Lieferbedingung aus der Liste auswählen.
  - ☐ Die Lieferbedingung wird nicht geändert.
  - ☑ Die ausgewählte Lieferbedingung wird für die Aufträge übernommen.
- **Fahrer:** Sie können einen anderen Fahrer aus der Liste auswählen.
  - ☐ Der Fahrer wird nicht geändert.
  - ☑ Der ausgewählte Fahrer wird für die Aufträge übernommen.
- **LKW:** Sie können einen anderen LKW aus der Liste auswählen.
  - ☐ Der LKW wird nicht geändert.
  - ☑ Der ausgewählte LKW wird für die Aufträge übernommen.

### Einstellungen (KAPS-Datei)

**Fertigung > Lieferwesen > Tourenliste > Menü Funktionen > Gruppe KAPS > Pfad für Datei**

*Abb. E-103 Einstellungen KAPS-Datei*

In diesem Dialog können Sie den Pfad und den Dateinamen für die KAPS-Datei festlegen. Dies ist eine Datei für die KAPS-Turbosoft-Schnittstelle. Die Ausgabe bezieht sich immer auf den aktuellen Nummernverwalter.

**KAPS-Datei**

- **Pfad:** In diesem Feld geben Sie den Pfad und Ordner an, in dem die KAPS-Datei gespeichert werden soll.
- **Dateiname ... +Tag+Monat+_Lfd.Nr.:** In diesem Feld geben Sie eine Kennzeichnung für die KAPS-Datei an. Sie können 2 Zeichen eintragen. Der Dateiname wird um das Datum und eine laufende Nummer erweitert.
- **Endung (ohne Punkt!):** In diesem Feld geben Sie die Datei-Endung für die KAPS-Datei an.

# Statusmeldung

**Fertigung > Lieferwesen > Statusmeldung**

Wenn Sie nicht mit Rückmeldungen aus der Betriebsdatenerfassung (BDE) arbeiten, können Sie über den Dialog Statusmeldung und Packmittelzuordnung Aufträge einscannen und den Status umsetzen.

Mit dem Tastatur-Scanner kann einem Auftrag ein neuer Status zugewiesen und das notwendige Packmittel zugeordnet werden. Die benötigten Barcodes können Sie dazu selber herstellen.
⇨ Tutorial, "Scan-Vorlage herstellen" auf Seite E-2398

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menüs im Dialog Statusmeldung" auf Seite E-2516
- "Statusmeldung und Packmittelzuordnung" auf Seite E-2518
- "Auswahl Gestell" auf Seite E-2524

## Menüs im Dialog Statusmeldung

**Fertigung > Lieferwesen > Statusmeldung**

Über die Menüs können Sie die Standardeinstellung des Dialoges bestimmen, Funktionen starten und andere Dialoge öffnen, ohne den Dialog zu schließen.

- "Menü Funktionen" auf Seite E-2516
- "Menü Optionen" auf Seite E-2517

### Menü Funktionen

**Fertigung > Lieferwesen > Statusmeldung**

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Dokumentenverwaltung zu schließen. Folgende Einträge werden angezeigt:

**Gruppe Packmittel**

Die Einträge sind nur im Register Manuelle Packmittelzuordnung freigeschaltet.
- **Hinzufügen:** Ordnet einem markierten Auftrag ein anderes Packmittel zu.
- **Löschen:** Löscht die Zuordnung.

**Gruppe Funktionen**

- **Alles markieren:**
  Der Eintrag ist nur im Register Manuelle Packmittelzuordnung freigeschaltet. Sie können damit alle Aufträge in der Liste markieren.
- **Einstellungen:**
  Öffnet den Dialog Optionen, um festzulegen, welche Statusänderungen erlaubt sind.
  ⇨ "Optionen in Statusmeldung" auf Seite E-2523

### Menü Optionen

**Fertigung > Lieferwesen > Statusmeldung**

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen.

**Gruppe Gestelltyp**

- **Eingabe Gestelltyp:** Mit dieser Einstellung springt der Fokus bei der Gestellzuordnung im Register Manuelle Packmittelzuordnung auf das Feld Packmittel statt auf das Feld für die Gestellnummer.
- **Ausgabe verfügbarer Gestelle:** Die Anzeige wird auf die Gestelle eingeschränkt, die verfügbar sind.

**Gruppe Datum**

- **Produktionsdatum vorgeben:** Schaltet das Feld Produktionsendedatum frei, um das Datum während dieser Sitzung manuell vorzugeben.
- **Anlieferdatum vorgeben:** Schaltet das Feld Anlieferdatum frei, um das Datum während dieser Sitzung manuell vorzugeben.

**Gruppe Produktion**

- **Prod.freigabe Auftrag, falls Subauftrag produziert:** Aufträge werden zur Produktion freigegeben, wenn der durch sie notwendige interne Auftrag fertig gemeldet wurde.

## Statusmeldung und Packmittelzuordnung

**Fertigung > Lieferwesen > Statusmeldung**

Mit einem Tastatur-Scanner können Sie den Auftragsstatus manuell umsetzen. Den fertigen Aufträgen können Packmittel zugeordnet werden. Diese Zuordnungen können als Listen für den Versand gedruckt werden.
- "Listendruck" auf Seite E-2533

In diesem Dialog finden Sie folgende Register:
- "Statusmeldung - Auftrag" auf Seite E-2518
- "Statusmeldung – Position" auf Seite E-2520
- "Statusmeldung – Manuelle Packmittelzuordnung" auf Seite E-2522

### Statusmeldung – Auftrag

**Fertigung > Lieferwesen > Statusmeldung > Register Statusmeldung – Auftrag**

*Abb. E-104 Statusmeldung – Auftrag*

In diesem Register können Sie den Auftragsstatus umsetzen, um den Auftrag für den Versand fertig zu machen.
⇨ Tutorial, "Manuelle Statusumsetzung" auf Seite E-2392

> **i Reihenfolge der Eingaben beachten**
> Tragen Sie zuerst alle Vorgaben ein, die für diese Sitzung gelten sollen. Beginnen Sie beim Scannen dann mit dem Status und lesen Sie erst danach den Auftrag ein. Lesen die dazu die Handlungsbeschreibungen im Tutorial.

**Zuordnung**

- **Auftrag/Statuspunkt:** In dieses Feld stellen Sie den Cursor, bevor Sie den Auftrag oder den Status scannen. Sie können den Auftrag oder den Status manuell eingeben. Dazu tragen Sie ein S (Status) oder ein O (Order) ein und ergänzen die Status- oder Auftragsnummer. Nach dem Einlesen des Auftrags wird der Status automatisch umgesetzt.

**Vorgabe**

- **Produktionsende:** Dieses Feld ist nur freigeschaltet, wenn Sie im Menü Einstellungen die Option Produktionsdatum vorgeben aktiviert haben. Sie können vor dem Einlesen eines Auftrags ein neues Datum eingeben, an dem die Produktion abgeschlossen sein wird. Das neue Datum wird nicht in den Auftrag zurückgeschrieben.
- **Anlieferdatum:** Dieses Feld ist nur freigeschaltet, wenn Sie im Menü Einstellungen die Option Anlieferdatum vorgeben aktiviert haben. Sie können vor dem Einlesen eines Auftrags ein neues Lieferdatum eingeben, z. B., wenn sich der Produktionstermin verschoben hat. Das neue Datum wird in den Auftrag zurückgeschrieben.

**Zielnummernverwalter**

- **(Zielnummernverwalter):** Sie können vor dem Einlesen einen Nummernverwalter auswählen oder einen Namen eintragen, um die eingelesenen Aufträge in diesen Nummernverwalter zu stellen. Dies ist sinnvoll, wenn Sie anschließend z. B. Versandpapiere drucken wollen. Das Feld wird freigeschaltet, wenn die Checkbox In NV kopieren markiert ist.
- **In NV kopieren:** Wenn die Checkbox In NV kopieren markiert ist, wird das Feld Zielnummernverwalter freigeschaltet, um einen Nummernverwalter einzutragen.
  Damit der im Feld Zielnummernverwalter eingetragene Nummernverwalter gefüllt wird, muss die Checkbox In NV kopieren aktiviert sein.
  - ☐ Die eingelesenen Aufträge werden nicht in den Nummernverwalter kopiert.
  - ☑ Die eingelesenen Aufträge werden automatisch in den gewählten Nummernverwalter kopiert.

**Übersicht**

Der Status der Aufträge wird beim Einlesen umgesetzt. Alle während einer Sitzung eingelesenen Aufträge werden in der Übersicht angezeigt.
- **Nummer:** Nummer des eingelesenen Auftrags.
- **Kunde/Lieferant:** Nummer des Kunden.
- **Name:** Name des Kunden.
- **Status:** Neuer Auftragsstatus.
- **Datum Erfass.:** Datum, an dem der Auftrag erfasst wurde.
- **Datum AB:** Datum der Auftragsbestätigung.
- **Datum Lieferung:** Lieferdatum aus dem Auftrag oder geändertes Datum aus dem Feld Anlieferdatum.
- **Anz. Positionen:** Anzahl der Auftragspositionen.

### Statusmeldung – Position

**Fertigung > Lieferwesen > Statusmeldung > Register Statusmeldung – Position**

*Abb. E-105 Statusmeldung – Position*

In diesem Register können Sie den Status für einzelne Auftragspositionen umsetzen. Der Auftragsstatus wird erst umgesetzt, wenn alle Auftragspositionen denselben Status haben. Den einzelnen Positionen können keine Packmittel zugeordnet werden.

Die Felder in den Bereichen Zuordnung, Vorgabe und Zielnummernverwalter sind ausführlich zum Register Statusmeldung – Auftrag beschrieben.
⇨ "Statusmeldung - Auftrag" auf Seite E-2518

**Positionsübersicht**

- **Aktueller Auftrag:** In diesem Feld wird die Auftragsnummer angezeigt, zu der die Positionen aufgelistet sind.

In der Übersicht sind alle Positionen des aktuellen Auftrags aufgeführt:
- **Pos:** Nummer der Auftragsposition.
- **Status:** Status der Auftragsposition. Er kann sich von dem der anderen Positionen unterscheiden.
- **Menge:** Stückzahl der Position.
- **Breite, Höhe:** Maße der Position.
- **Bezeichnung:** Bezeichnung des Glases.

### Statusmeldung – Manuelle Packmittelzuordnung

**Fertigung > Lieferwesen > Statusmeldung > Register Manuelle Packmittelzuordnung**

*Abb. E-106 Statusmeldung – Manuelle Packmittelzuordnung*

In diesem Register können Sie den Positionen eines Auftrags Packmittel (Gestelle und deren Gestellnummern) zuordnen. Gestelle können wahlweise per Scanner oder manuell zugeordnet werden.

**Zuordnung**

- **Packmittel:** In der Kombobox werden alle Packmittel angeboten, die im System hinterlegt sind. Das können Gestellarten, Kisten, Container usw. sein.
- **[Ordner]:** Mit dieser Schaltfläche öffnen Sie den Dialog Auswahl Gestell, um eine freie Gestellnummer aus der gewählten Gestellart zu suchen.
  ⇨ "Auswahl Gestell" auf Seite E-2524

### Optionen in Statusmeldung

**Fertigung > Lieferwesen > Statusmeldung > Menü Funktionen > Gruppe Funktionen > Einstellungen**

*Abb. E-107 Optionen in Statusmeldung*

In diesem Dialog stellen Sie ein, welche Statuspunkte geändert werden können. Die Einstellungen können so eingerichtet werden, dass sie nur für den jeweils angemeldeten Mitarbeiter gelten.

> **i Administratorrechte erforderlich**
> Die Optionen im Dialog Statusmeldung kann nur der Systemadministrator ändern.

- **Verfügbare Statuspunkte:** In der Liste sind alle Statuspunkte aufgeführt, die in den Stammdaten eingerichtet wurden.
- **Änderbare Statuspunkte:** In der Liste werden alle Statuspunkte aufgeführt, die als neuer Status gewählt werden dürfen.
- **Statusverminderung erlauben:** Standardmäßig wird der Status mit der Statusmeldung hochgesetzt. In einzelnen Fällen kann es jedoch notwendig sein, den Status zurückzusetzen, z. B., wenn ein Auftrag versehentlich als fertig gebucht wurde.
  - ☐ Der Status eines Auftrags oder einer Position kann nicht zurückgesetzt werden. Wenn Sie dennoch einen Fehler korrigieren müssen, kann der Status des einzelnen Auftrags in der Dokumentenverwaltung zurückgesetzt werden. ⇨ Verkauf, "Menü Funktionen" auf Seite C-1669
  - ☑ Der Status kann zurückgesetzt werden. Die Checkbox Meldung bei erreichtem Sperrstatus wird freigeschaltet.
- **Meldung bei erreichtem Sperrstatus:** Sie können festlegen, ob bei einer Statusverminderung eine Meldung ausgeben wird. Diese Checkbox ist nur freigeschaltet, wenn die Checkbox Statusverminderung erlaubt aktiviert ist.
  - ☐ Es wird keine Meldung ausgegeben.
  - ☑ Wenn bei einer Statusverminderung der Sperrstatus höher ist, als der Auftragsstatus, wird eine Meldung ausgegeben. Sie können dann entscheiden, ob Sie den Status ändern wollen.
- **Keine Laufnr., dann 9999 eintragen:** Standardmäßig wird eine Laufnummer vom System vergeben, wenn ein Produktionslauf angelegt wird. Mit dieser Option legen Sie fest, ob Läufen ohne eigene Laufnummer eine Laufnummer zugeordnet wird. Diese Checkbox ist nur freigeschaltet, wenn ein Eintrag im Feld änderbare Statuspunkte markiert ist.
  - ☐ Für den Lauf wird keine Laufnummer vergeben.
  - ☑ Die Laufnummer 9999 wird vergeben, wenn keine eigene Laufnummer vorhanden ist.

### Auswahl Gestell

**Fertigung > Lieferwesen > Statusmeldung > Register Manuelle Packmittelzuordnung > [Ordner]**

*Abb. E-108 Manuelle Packmittelzuordnung – Gestell auswählen*

Wenn Sie nicht mit einem Tastatur-Scanner arbeiten, können Sie in diesem Dialog ein freies Gestell auswählen, um es dem aktuellen Auftrag zuzuordnen.

**Filter**

- **Gestellart:** In der Kombobox werden alle Gestellarten zur Auswahl angeboten, die in den Stammdaten angelegt sind.
- **Gestellnummer von, bis:** Sie können die Anzeige von Gestellen auf eine Folge von Gestellnummern eingrenzen. Die Gestellnummern werden im Dialog Gestelle hinterlegt. ⇨ "Gestelle" auf Seite E-2540
- **Nicht verfügbare Gestelle:** Wenn Gestelle außer Haus gemeldet sind, können sie nicht nochmals belegt werden. Sie können die Anzeige dieser Gestellnummern ausschließen.
  - ☐ Nur die Gestelle werden angezeigt, die für den aktuellen Auftrag verwendet werden können.
  - ☑ Alle Gestelle werden angezeigt.

**Übersicht**

In der Übersicht werden alle Gestelle angezeigt, die den Suchkriterien entsprechen.
- **Gestellnummer:** Gestellnummer, die in den Stammdaten hinterlegt wurde.
- **Bezeichnung:** Bezeichnung, die in den Stammdaten hinterlegt wurde.
- **Gestellart:** Wenn Sie die Suche nicht auf eine bestimmte Gestellart eingegrenzt haben, dient die Anzeige der Gestellart zur weiteren Differenzierung.
- **Ausgegeben:** Anzeige, ob das Gestell aktuell verwendet wird.
- **Ausgabedatum:** Ein Ausgabedatum wird nur angezeigt, wenn die Gestellnummer einem Auftrag zugeordnet ist. Wenn das Gestell wieder als frei gebucht wurde, bleibt das Feld leer.

# Kommissionierung

**Fertigung > Lieferwesen > Kommissionierung**

Mit der Kommissionierung planen Sie die Beladung Ihrer Fahrzeuge.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menüs im Dialog Kommissionierung" auf Seite E-2526
- "Kommissionierung" auf Seite E-2528
- "Gestelltransfer" auf Seite E-2531
- "Export Optionen" auf Seite E-2532

## Menüs im Dialog Kommissionierung

**Fertigung > Lieferwesen > Kommissionierung**

Über die Menüs können Sie die Standardeinstellung des Dialoges bestimmen, Funktionen starten und andere Dialoge öffnen, ohne den Dialog zu schließen.

- "Menü Funktionen" auf Seite E-2526
- "Menü Optionen" auf Seite E-2527

### Menü Funktionen

**Fertigung > Lieferwesen > Kommissionierung**

Über dieses Menü können Sie verschiedene Funktionen ausführen, ohne die Kommissionierung zu schließen.

**Gruppe Dokument**
- **Historie:** Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des markierten Dokuments. Der Dialog ist ausführlich im Part Verkauf beschrieben. ⇨ Verkauf, "Historie" auf Seite C-1834
- **Alles markieren:** Markiert alle Aufträge in der Übersicht.

**Gruppe Position**
- **Initialisierung:** Öffnet den Dialog Export-Optionen, in dem Sie die Zuordnung von Gestellnummern umorganisieren können. ⇨ "Export Optionen" auf Seite E-2532
- **Auf Position vererben:** Überträgt die Packmittelgruppe auf alle Positionen des Auftrags.

**Gruppe Packmittelgruppen**
- **Packmittelgruppen:** Öffnet den Dialog Packmittelgruppen, um eine neue Packmittelgruppe zu vergeben. Diese Funktion wird in der Regel nur in älteren Installation der Software genutzt.

**Gruppe Gestellzuordnung**
- **Gestellzuordnung:** Öffnet den Dialog Statusmeldung – Manuelle Packmittelzuordnung, um Gestelle zuordnen. ⇨ "Statusmeldung - Manuelle Packmittelzuordnung" auf Seite E-2522

### Menü Optionen

**Fertigung > Lieferwesen > Kommissionierung**

**Gruppe Optionen**
- **Eingabe von einzelnen Auftragsnummern:** Nur dieser Auftrag wird in der Tabelle selektiert. Das Standardverhalten, dass die eingegebenen Auftragsnummern zusätzlich zu den bereits Selektierten für eine Änderung markiert werden, bleibt bestehen, wenn die Option nicht gesetzt ist.

## Kommissionierung (Dialog)

**Fertigung > Lieferwesen > Kommissionierung**

*Abb. E-109 Kommissionierung*

In diesem Dialog können Sie den Versand mit Ihrem eigenen Fuhrpark organisieren. Sie können die Tour, den Lkw und das Lieferdatum für einzelne oder mehrere Aufträge gleichzeitig ändern. Sie können sich das Ergebnis der Kommissionierung nach dem Speichern am Bildschirm anzeigen und/oder drucken lassen.

Wenn Sie mit Spediteuren arbeiten, können Sie den Versand über den Dialog Versand organisieren.
⇨ "Versand (Spedition)" auf Seite E-2591

> **i Anzeige der Aufträge**
> Bevor Sie sich die Aufträge anzeigen lassen, können Sie über Lieferwesen > Nummernverwalter einen Nummernverwalter aktivieren. Die in ihm enthaltenen Aufträge werden aufgelistet. Sie können Aufträge aber auch einzeln auswählen und in den gewünschten Nummernverwalter stellen.

### Auftrag

- **Nummer:** Sie können eine Auftragsnummer eingeben oder den Auftrag über die Suche auswählen. Der Auftrag wird mit [OK] übernommen und im Bereich Aufträge aufgelistet.
- **In NV übernehmen:** Sie können die bearbeiteten Aufträge automatisch in einen anderen Nummernverwalter stellen.
  - ☐ Die Aufträge werden nicht in einen (anderen) Nummernverwalter gestellt.
  - ☑ Das Feld Name (Nummernverwalter) wird freigeschaltet. Die Aufträge werden in den gewählten Nummernverwalter gestellt. Wenn in dem Nummernverwalter bereits Aufträge enthalten sind, werden diese im Bereich Aufträge angezeigt.
- **Name (Nummernverwalter):** Das Feld ist nur freigeschaltet, wenn die Checkbox in NV übernehmen aktiviert ist. Sie können den Nummernverwalter auswählen, in den die bearbeiteten Aufträge gestellt werden sollen.

### Eingabe

- **Tour:** Sie können jedem im Feld Aufträge markierten Auftrag eine andere Tour zuweisen. Die Änderungen werden in den Auftrag und ggf. in die Ausgangsbuchung des Gestells zurückgeschrieben.
- **Lieferbedingung:** Sie können jedem im Feld Aufträge markierten Auftrag eine andere Lieferbedingung zuweisen. Die Lieferbedingungen sind unter Stammdaten > Versand definiert. ⇨ Stammdaten, "Lieferbedingungen" auf Seite B-994
- **Anlieferung:** Sie können für jeden im Feld Aufträge markierten Auftrag einen neuen Liefertermin angeben. Die Änderungen werden in die Aufträge zurückgeschrieben.
- **Lkw:** Sie können jedem im Feld Aufträge markierten Auftrag einem Lkw zuweisen, indem Sie die Nummer (ID) eingeben oder ihn über die Kombobox auswählen. Die Fahrzeuge sind unter Stammdaten > Versand definiert. ⇨ Stammdaten, "Lkw" auf Seite B-998
- **Fahrer:** Sie können jedem im Feld Aufträge markierten Auftrag einen Fahrer zuweisen. Die Fahrer sind unter Stammdaten > Versand definiert. ⇨ Stammdaten, "Fahrer" auf Seite B-999
- **Status:** Sie können jedem im Feld Aufträge markierten Auftrag einen anderen Status zuweisen. ⇨ "Optionen in Statusmeldung" auf Seite E-2523

### Aufträge

Alle ausgewählten Aufträge werden in der Übersicht angezeigt. Um die Daten einer Auslieferung zu ändern, müssen Sie den entsprechenden Auftrag markieren. Die Mehrfachauswahl ist mit den Tasten <Strg> oder <Shift> möglich.

- **Nummer, Status:** Nummer und Status des Auftrags.
- **Tour, Lieferbedingung:** Nummer der zugewiesenen Tour und Lieferbedingung, z. B. Lkw, Spedition.
- **Lieferdatum:** Datum der Lieferung.
- **Kundennummer, Name:** Nummer und Name des Kunden.
- **Abw. Straße, Abw. PLZ, Abw. Ort:** Eine abweichende Lieferanschrift wird nur dargestellt, wenn diese im Auftrag angegeben ist.
- **Menge:** Gesamtmenge aller Positionen des Auftrags.
- **Gewicht:** Gesamtgewicht aller Positionen des Auftrags.
- **LKW, Fahrer:** Nummer des Lkws und Name des Fahrers.

### Positionen

> **i Keine Verwaltung von einzelnen Positionen**
> Sie können in diesem Dialog nur gesamte Aufträge verwalten, die fertig gemeldet sind. Wenn nur einzelne Positionen fertiggemeldet sind, müssen Sie einen Teillieferungsauftrag für den Versand fertigmachen. Diese Funktion ist ausführlich im Part Verkauf beschrieben.
> ⇨ Verkauf, "Teillieferung zu einem Auftrag" auf Seite C-1518

In der Übersicht werden alle Positionen des Auftrags angezeigt, der in der Auftragsübersicht markiert ist. Wenn mehrere Aufträge markiert sind, werden keine Positionen angezeigt.

- **Pos.:** Nummer der Auftragsposition.
- **Bezeichnung:** Name des Produkts.
- **Gestell:** Nummer des Gestells.
- **Gestelltyp:** In diesem Feld können Sie den passenden Gestelltyp auswählen. Wenn Sie den Cursor in das Feld setzen, wird die Schaltfläche zum Öffnen der Kombobox angezeigt.
- **Packmittelgruppe:** Sie können eine Packmittelgruppe eintragen.
- **Menge:** Stückzahl der Auftragsposition.

### Summen selektierter LKW

- **Menge, Gewicht:** Anzeige von Gesamtmenge und Gesamtgewicht für den Lkw, der für diese Tour an diesem Termin fährt. Die Werte werden in roter Schrift dargestellt, wenn das Gewicht höher ist, als für den Lkw zulässig.
- **Maximalgewicht:** Gewicht, das der zugewiesene Lkw laden kann.

### Summen selektierte Aufträge

- **Menge, Gewicht:** Anzeige von Menge und Gewicht der markierten Aufträge.

## Gestelltransfer

**Fertigung > Lieferwesen > Kommissionierung > Menü Funktionen > Gruppe Position > Initialisierung**

*Abb. E-110 Kommissionierung – Gestelltransfer*

In diesem Dialog können Sie die Gestellverwaltung reorganisieren. Diese Funktion dürfen Sie nur nach Absprache mit der A+W Software GmbH ausführen.

## Export Optionen

**Fertigung > Lieferwesen > Kommissionierung > Tabelleneigenschaften > Export > Optionen**

*Abb. E-111 Export*

Mit dieser Funktion können Sie die Gestellzuordnung aus einer alten Datenbanktabelle in die neuen Felder übertragen. Wenn Sie Ihre Gestellzuordnung umorganisieren wollen, setzen Sie sich bitte mit dem Support der A+W Software GmbH in Verbindung.

## Listendruck

**Fertigung > Lieferwesen > Listendruck**

*Abb. E-112 Listendruck*

In diesem Dialog können Sie verschiedene Listen nach der Kommissionierung ausdrucken oder auf dem Monitor anzeigen lassen.

### Nummernverwalter

- **(Nummernverwalter):** In diesem Feld wählen Sie den Nummernverwalter aus, in dem die Aufträge gesammelt sind, zu denen Sie die Liste drucken wollen.
- **[Gestellausgabe]:** Mit dieser Schaltfläche öffnen Sie den Dialog Gestellausgabe, in dem Sie die Gestellbelegung prüfen können.
  ⇨ "Gestellausgabe" auf Seite E-2536

### Übersicht

In der Übersicht werden alle Aufträge angezeigt, die im ausgewählten Nummernverwalter stehen.

- **Nummer:** Nummer des Auftrags.
- **Kunde/Lieferant, Name:** Nummer und Name des Kunden.
- **Status:** Auftragsstatus.
- **Datum Erfass.:** Datum, an dem der Auftrag erfasst wurde.
- **Datum AB:** Datum der Auftragsbestätigung.
- **Datum Lieferung:** Lieferdatum aus dem Auftrag.
- **Lieferschein:** Nummer des Lieferscheins.

### Druckeinstellungen

Mit der Wahl der Option legen Sie fest, in welche Liste das Ergebnis der Kommissionierung gedruckt werden soll:

- **Transportmittelbeladungsliste:** In dieser Liste wird angezeigt, welche Gestelle auf dem Lkw stehen (sollen).
- **Empfangsbestätigungsliste:** In dieser Liste werden pro Auftrag Details zu den Positionen angezeigt, deren Empfang sich der Fahrer bestätigen lassen muss.
- **Gestellliste (auswärtig):** In dieser Liste werden pro Tour alle Gestelle aufgeführt, die derzeit außer Haus sind.

> **i Seitenwechsel**
> Bei den beiden ersten Listen wird jeweils ein Seitenwechsel eingefügt, wenn sich der Lkw, die Tour und/oder der Liefertermin ändern.

### Beispiele:

*Abb. E-113 Transportmittelbeladungsliste*
*Abb. E-114 Empfangsbestätigungsliste*

## Gestellausgabe

**Fertigung > Lieferwesen > Listendruck > [Gestellausgabe]**

*Abb. E-115 Gestellausgabe*

In diesem Dialog können Sie die Gestellbelegung analysieren. Dabei wird geprüft, ob auf einem Gestell nur Aufträge eines Kunden sind.
Mit [OK] werden die Gestelle aus der Gestellverwaltung ausgebucht bzw. als auswärtig verbucht. Danach können Sie die Gestellbelegungsliste drucken.

### Tabelle

In der Übersicht werden alle auswärtigen Gestelle aufgelistet.

- **Gestellnr.:** Nummer des auswärtigen Gestells.
- **Gestellart:** Gestellart des auswärtigen Gestells.
- **Auftrag/Kunde:** Auftragsnummer und Kunde, bei dem das Gestell steht.
- **Auftrag:** Auftrag, der mit dem das Gestell ausgeliefert wurde.
- **Latten, Räder, Wagen:** Zubehör des auswärtigen Gestells.

### Optionen

**Keine Gestellausgabe für Positionen mit Menge 0** Sie können die Zuweisung zu Positionen ohne Menge unterdrücken.
- ☐ Allen Positionen werden Gestelle zugewiesen.
- ☑ Positionen ohne Menge wird kein Gestell zugeordnet.

## Warenausgang Kisten

**Fertigung > Lieferwesen > Warenausgang Kisten**

Der Dialog Warenausgang Kiste ist im Part Einkauf beschrieben:
⇨ Einkauf, "Wareneingang – Identnummer" auf Seite D-2274

### Warenausgang

**Fertigung > Lieferwesen > Warenausgang Kisten > Register Identnummern**

*Abb. E-116 Warenausgang von Kisten – Kiste ausbuchen*

In diesem Register können Sie eine Kiste reservieren oder aus dem Lagerbestand ausbuchen. Sie können nur Kisten reservieren, die beim Lagereingang mit einer Kisten-ID erfasst wurden.
⇨ Tutorial, "Warenausgang Kisten" auf Seite E-2443

# Gestellverwaltung

**Fertigung > Gestellverwaltung**

Sie können die Verpackung von produzierten Aufträgen auf Gestellen planen und steuern. Dazu stehen im Menü Gestellverwaltung folgende Dialoge zur Verfügung:
- Gestellarten
- Gestelle
- Kundenkommissionen

In diesem Abschnitt finden Sie Informationen zu folgenden Dialogen des Programmbereichs:
- "Gestellarten" auf Seite E-2555
- "Gestellübersicht" auf Seite E-2557
- "Übersicht Partner" auf Seite E-2558
- "Gestell umbuchen" auf Seite E-2559
- "Mahnstatus zurücksetzen" auf Seite E-2560
- "Kundenkommissionen" auf Seite E-2565

## Gestelle

**Fertigung > Gestellverwaltung > Gestelle**

Über den Dialog Gestelle können Sie die Verwendung der Gestelle überwachen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menüs im Dialog Gestelle" auf Seite E-2538
- "Gestelle" auf Seite E-2540

Über den Dialog Gestelle können Sie außerdem folgende Dialoge öffnen:
- "Gestellübersicht" auf Seite E-2557
- "Übersicht Partner" auf Seite E-2558
- "Mahnstatus zurücksetzen" auf Seite E-2560
- "Gestell umbuchen" auf Seite E-2559

### Menüs im Dialog Gestelle

**Fertigung > Gestellverwaltung > Gestelle**

Über die Menüs der Gestellverwaltung können Sie die Standardeinstellung des Dialoges bestimmen und andere Dialoge öffnen, ohne die Gestellverwaltung zu schließen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Optionen" auf Seite E-2538
- "Menü Funktionen" auf Seite E-2539

#### Menü Optionen

**Fertigung > Gestellverwaltung > Gestelle > Menü Optionen**

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

**Gruppe Gestelle**
- **Erweiterte Gestellsuche:** Mit dieser Option können Sie die Suche auch mit Teilen der Gestellnummer durchführen. Wenn Sie z. B. im Feld Nummer eine 5 eingeben, werden alle Gestelle gesucht, in deren Gestellnummer eine 5 vorkommt.

**Gruppe Ausgabe**
- **Ausgabe verfügbarer Gestelle:** Die Anzeige wird auf verfügbare Gestelle eingeschränkt. Die Option ist nur im Register Ausgang freigeschaltet.
- **Ausgabe an gesperrte Kunden:** Gestelle können keinem Kunden zugeordnet werden, der gesperrt ist. Die Option ist nur im Register Ausgang freigeschaltet.
- **Auswärtige Gestelle mit Ausgabeinfos:** Beim Druck einer Liste aller auswärtigen Gestelle werden zusätzlich der Name der Tour und des Kunden angegeben.
- **Faxnummer im Druckjobname:** Angabe der Faxnummer, wenn Sie den Druck über einen Druckjob steuern.
- **Gestellbelegung in Historiendruck:** Die Belegung der Gestelle aus der Historientabelle wird beim Historiendruck mitgedruckt.

**Gruppe Mahnstufen**
- **Verwendung von Mahnstufen:** Die Option ist nur im Register Mahnung freigeschaltet.
- **Neue Seite bei Wechsel der Mahnstufe:** Beim Druck der angemahnten Gestelle/Kunden wird jeweils ein Seitenvorschub geschaltet, wenn eine andere Mahnstufe beginnt. Die Option ist nur im Register Mahnung freigeschaltet.

#### Menü Funktionen

**Fertigung > Gestellverwaltung > Gestelle > Menü Funktionen**

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Gestellverwaltung zu schließen.

**Gruppe Ausführen**
- **Gestell umbuchen:** Öffnet den Dialog Gestelle umbuchen, in dem Sie ein Gestell auf einen anderen Partner umbuchen können. ⇨ "Gestell umbuchen" auf Seite E-2559
- **Ausgang ändern:** Schaltet die Felder für Änderungen frei.
- **Mahnstatus zurücksetzen:** Öffnet den Dialog Mahnstatus zurücksetzen, in dem Sie den Mahnstatus zurücksetzen können. ⇨ "Mahnstatus zurücksetzen" auf Seite E-2560
- **Gestellhistoriendetails initialisieren:** Alle vorhandenen Historiensätze der Gestellbelegung werden gelöscht und die aktuelle Belegung der Gestelle wird eingetragen. Diese Funktion sollte nur ausgeführt werden, bevor Sie A+W Business in Betrieb nehmen.
- **Barcodes für Gestelle drucken:** Öffnet den Dialog Druck – Gestell Barcodes, in dem Sie Barcodes für Gestelle drucken können.
- **Gestellbelegung:** Öffnet den Dialog Gestellbelegung, in dem Sie den Gestellen Auftragspositionen zuordnen können. ⇨ "Gestellbelegung" auf Seite E-2560

### Gestelle (Dialog)

**Fertigung > Gestellverwaltung > Gestelle**

In diesem Dialog können Sie Gestelle anlegen und deren Ein- und Ausgang buchen. Für säumige Rückgabe können Sie Mahnungen erstellen.

In diesem Dialog finden Sie folgende Register:
- "Gestellverwaltung – Gestelle” auf Seite E-2541
- "Gestellverwaltung - Ausgang" auf Seite E-2545
- "Gestellverwaltung – Eingang" auf Seite E-2548
- "Gestellverwaltung – Historie" auf Seite E-2549
- "Gestellverwaltung – Mahnung" auf Seite E-2551

### Gestellverwaltung – Gestelle

**Fertigung > Gestellverwaltung > Gestelle > Register Gestelle**

*Abb. E-117 Gestellverwaltung - Gestelle*

In diesem Register können Sie neue Gestelle hinzufügen oder die Daten der Gestelle bearbeiten.

**Gestelldaten**

- **Nummer:** Beim Anlegen kann die Gestellnummer alphanumerisch eingegeben werden. Jede Nummer darf nur einmal verwendet werden. Sie können sich die freien Nummern anzeigen lassen, indem Sie auf die Schaltfläche [Ordner] klicken. ⇨ "Gestellübersicht" auf Seite E-2557
- **Art:** Sie können nur die Gestellarten zuordnen, die im Dialog Gestellarten angelegt sind.
- **Bezeichnung:** Sie können eine alphanumerische Bezeichnung für das Gestell eintragen, z. B. einen Typnamen. Diese Bezeichnung kann auf den Listen gedruckt werden.
- **Bemerkung:** Sie können eine Bemerkung zum Gestell eintragen, z. B. bei Kundengestellen den Namen des Kunden.
- **Latten/Räder/Wagen:** Sie können angeben, wie viele Latten, Räder oder Wagen das Gestell hat.
- **Mietsatz/Tage frei:** Wenn Sie für Ihre Gestelle eine Miete berechnen, können Sie hier den Tagessatz und die Anzahl der Tage eingeben, die das Gestell kostenlos zur Verfügung steht.
- **Änderung:** Name des letzten Bearbeiters und Datum der letzten Bearbeitung.

**Eigenschaften**

Mit der Wahl der Eigenschaft geben Sie an, ob und wie das Gestell verwendet wird. Mit Kombinationen von Suchkriterien können Sie die Suche weiter einschränken. Bitte beachten Sie, dass nicht jede Kombination sinnvoll ist.

- **Verfügbar:** Als verfügbar gelten alle Gestelle, die nicht belegt und nicht verloren oder gesperrt sind.
  - ☐ Das Gestell ist nicht verfügbar.
  - ☑ Das Gestell ist verfügbar und kann belegt werden.
- **Gesperrt:** Ein Gestell kann für die Verwendung gesperrt werden, z. B., weil es zur Reparatur ist.
  - ☐ Das Gestell ist nicht gesperrt. Dies bedeutet jedoch nicht automatisch, dass es verfügbar ist.
  - ☑ Das Gestell ist gesperrt und kann nicht belegt werden.
- **Verloren:** Gestelle können auf unterschiedliche Weise abhandenkommen.
  - ☐ Das Gestell ist nicht verloren. Dies bedeutet jedoch nicht automatisch, dass es verfügbar ist.
  - ☑ Das Gestell ist verloren.
- **Stationär:** Gestelle können fest an einen Ort in der Produktion gebunden sein.
  - ☐ Das Gestell wird nicht stationär verwendet.
  - ☑ Das Gestell wird stationär verwendet. Es kann nicht für eine Lieferung außer Haus eingesetzt werden.
- **Keine Mahnung:** Gestelle können vorübergehend beim Kunden stehen. Wenn Sie Miete berechnen oder nur über eine geringe Anzahl von Gestellen verfügen, können Sie die säumige Rückgabe anmahnen.
  - ☐ Das Gestell soll nicht angemahnt werden, z. B. bei Fremdgestellen.
  - ☑ Das Gestell kann angemahnt werden.
- **Automatisch angelegt:** Gestelle können automatisch angelegt werden, wenn ein Barcode gescannt wurde, der im System nicht bekannt ist.
  - ☐ Das Gestell wurde manuell angelegt.
  - ☑ Das Gestell wurde automatisch angelegt.
- **Gestelltyp:** Aus der Kombobox wählen Sie den entsprechenden Gestelltyp aus. Folgende Werte stehen zur Verfügung:
  - Produktion
  - Versand
  - Mix (steht gleichzeitig für Produktion und Versand zur Verfügung).
- **Fremdgestell:** Gestelle können von einem Lieferanten oder dem Kunden zur Verfügung gestellt worden sein.
  - ☐ Das Gestell gehört zum Unternehmen.
  - ☑ Das Gestell gehört einem Lieferanten oder Kunden. In diesem Falle wird der Name mit angegeben.
- **Auswärtig von bis:** Das Gestell kann für einen bestimmten Zeitraum außer Haus gebucht werden, z. B., weil es an einen Kunden vermietet wurde.
  - ☐ Das Gestell ist nicht für einen Zeitraum ausgebucht.
  - ☑ Das Gestell ist für einen bestimmten Zeitraum außer Haus. Zusätzlich wird der Zeitraum angegeben.
- **Bei Kunde:** Der Kunde, an den das Gestell für einen bestimmten Zeitraum verliehen wurde.
- **Abw. Adresse:** Wenn das vermietete Gestell an einen anderen Standort als die Kundenadresse geliefert wurde, kann der aktuelle Standort eingetragen werden.
- **Tour:** Das Gestell wurde für eine Tour ausgewählt.
- **Gemahnt:** Gestelle können vorübergehend beim Kunden stehen. Wenn Sie Miete berechnen oder nur über eine geringe Anzahl von Gestellen verfügen, können Sie die säumige Rückgabe anmahnen.
  - ☐ Das Gestell ist nicht angemahnt.
  - ☑ Das Gestell ist angemahnt, was gleichzeitig bedeutet, dass es nicht verfügbar ist.
- **Abholbereit:** Datum, ab dem das Gestell beim Kunden abgeholt werden kann.

**Wiedervorlage**
- **Am:** Datum der Wiedervorlage zur Erinnerung.
- **An:** Partner, der die Erinnerung erhalten soll.

**Gestelle (Übersichtstabelle)**

In der Übersicht werden alle Gestelle angezeigt, die den Suchkriterien entsprechen. In den einzelnen Spalten werden die Gestelldaten und Eigenschaften angezeigt, die oben beschrieben sind.
Zusätzlich werden folgende Spalten angezeigt:
- **Partner:** Kunde oder Lieferant, an den das Gestell ausgegeben wurde.
- **Ausgabedatum:** Datum, an dem die Ausgabe gebucht wurde.
- **Lieferant:** Lieferant, wenn das Gestell (Fremdgestell) von diesem zur Verfügung gestellt wurde.
- **Auswärtig:** Das Gestell ist außer Haus und damit nicht verfügbar.
- **Nicht mahnbar:** Das Gestell kann nicht angemahnt werden.
- **Tour-Nr.:** Nummer der Tour, mit der das Gestell außer Haus gebucht wurde.

### Gestellverwaltung - Ausgang

**Fertigung > Gestellverwaltung > Gestelle > Register Ausgang**

*Abb. E-118 Gestellverwaltung – Ausgang*

In diesem Register können Sie Gestelle aus dem verfügbaren Bestand ausbuchen und sich einen Überblick über die verfügbaren Gestelle anzeigen lassen.

**Ausgabe**
Mit der Wahl der Option legen Sie die Suchkriterien fest:
- **Gestell:** Die Suche bezieht sich auf Gestelle.
- **Zubehör:** Die Suche bezieht sich auf Zubehör.

**An**
Mit der Wahl der Option legen Sie die fest, an wen das Gestell ausgeliehen ist:
- **Kunde:** Die Suche bezieht sich auf Gestelle, die an Kunden ausgegeben wurden.
- **Lieferant:** Die Suche bezieht sich auf Gestelle, die an Lieferanten ausgegeben wurden.

**Ausgabeinformationen**

Die Felder werden erst freigeschaltet, wenn Sie ein neues Gestell anlegen oder wenn Sie in der Übersicht eines der verfügbaren Gestelle markiert haben, für das Sie einen Ausgang buchen wollen.

- **Nummer:** Nummer des Gestells.
- **Art:** Gestellart, z. B. A-Gestell groß.
- **Kunde:** Nummer des Kunden, an den die Lieferung geht.
- **Straße, PLZ/Ort:** Sie können eine abweichende Lieferanschrift für alle angezeigten Aufträge eintragen. Die Adressfelder werden freigeschaltet, wenn Sie die Checkbox abw. Lieferadresse markiert haben.
- **Datum:** Datum der Gestellbelegung. Standardmäßig ist das aktuelle Tagesdatum angezeigt. Es kann überschrieben werden.
- **Versand:** Bemerkung zum Versand. Diese Bemerkung wird in der Übersicht in der Spalte Versandinfo angezeigt.
- **Fahrer, Tour:** Fahrer und Tour, mit der das Gestell ausgeliefert wird.
- **Spannlatten/Räder/Wagen:** Zubehör, das zusätzlich zum Gestell ausgeliefert wird.
- **Lieferschein:** Nummer des Lieferscheins.
- **Abw. Lieferadresse:** Sie können eine abweichende Lieferadresse eintragen.
  - ☐ Das Gestell wird an die Adresse des Auftrags geliefert.
  - ☑ Das Gestell soll an eine abweichende Adresse geliefert werden. Die Adressfelder für Straße und Ort werden freigeschaltet.

**Wiedervorlage**
- **Am:** Datum der Wiedervorlage zur Erinnerung.
- **An:** Partner, der die Erinnerung erhalten soll.
- **Bemerkung:** Anmerkung zur Erinnerung.

**Verfügbare Gestelle**

> **i Anzeige filtern**
> Nur wenn Sie die Option Ausgabe verfügbarer Gestelle aktiviert haben, werden alle Gestelle ausgeblendet, die nicht verfügbar sind. Die Option muss vor dem Start der Suche ausgewählt sein. Nicht verfügbare Gestelle werden nicht aus der Übersicht entfernt, wenn die Option nach der Suche aktiviert wurde.

In der Übersicht werden alle (verfügbaren) Gestelle mit folgenden Details angezeigt:
- **Nummer:** Gestellnummer.
- **Art:** Gestellart.
- **Ausgabe:** Datum der Ausgabe.
- **Partner:** Kunde oder Lieferant, an den das Gestell ausgegeben wurde.
- **Spannlatten, Räder, Wagen:** Jeweilige Anzahl des Zubehörs.
- **Versandinfo:** Text, der im Feld Versand eingegeben wurde.
- **Fremdgestell:** Gestell des Kunden oder Lieferanten.
- **Fahrer:** Fahrer, der das Gestell ausgeliefert hat.
- **Tour:** Tournummer, mit der das Gestell ausgeliefert wurde.
- **Tourbezeichnung:** Name der Tour.

### Gestellverwaltung – Eingang

**Fertigung > Gestellverwaltung > Gestelle > Register Eingang**

*Abb. E-119 Gestellverwaltung – Eingang*

In diesem Register können Sie die Gestelle wieder in den verfügbaren Bestand übernehmen, wenn sie von einer Lieferung oder einem Kunden zurückgekommen sind.
Die Felder sind ausführlich zum Register Ausgang beschrieben.
⇨ "Gestellverwaltung - Ausgang" auf Seite E-2545

Sie können über das Menü Funktionen ein Gestell von einem Kunden an einen anderen umbuchen.
⇨ "Gestell umbuchen" auf Seite E-2559

### Gestellverwaltung – Historie

**Fertigung > Gestellverwaltung > Gestelle > Register Historie**

*Abb. E-120 Gestellverwaltung – Historie*

In diesem Register können Sie die Historie einzelner Gestelle verfolgen. Wenn Sie ein Gestell in der Übersicht markiert haben, können Sie sich über die Schaltfläche [Ordner] anzeigen lassen, welche weiteren Gestelle bei dem Partner stehen.
⇨ "Übersicht Partner" auf Seite E-2558

**Auswahl**
- **Gestellnummer:** Sie können die Auswahl auf eine bestimmte Gestellnummer einschränken. Wenn Sie keine Nummer eingeben, werden alle Gestelle aufgelistet, die den übrigen Kriterien entsprechen.
- **Letzte Buchung zuerst:** Sie können die Übersicht der Gestelle nach dem Buchungsdatum sortieren. Wenn Sie die Option aktivieren, bleibt die Sortierung auch in späteren Sitzungen aktiviert.
  - ☐ Die Übersicht ist nach Spalte Art sortiert.
  - ☑ Die Übersicht wird sortiert. Die zuletzt gebuchten Gestelle stehen am Anfang der Liste.
- **Gestellart:** Sie können die Auswahl auf eine bestimmte Gestellart einschränken. Wenn Sie keine Gestellart angeben, werden alle Gestelle aufgelistet, die den übrigen Kriterien entsprechen.
- **Zeitraum von ... bis:** Sie können die Auswahl auf einen Zeitraum einschränken, in dem Ausgang und/oder Eingang gebucht wurden.
- **Buchungstyp:** Sie können Sie Auswahl auf einen der folgenden Buchungstypen einschränken:
  - **Gestellbelegung:** Mit dieser Option werden die Buchungen der Gestelle angezeigt.
  - **Gestellbewegung:** Mit dieser Option werden alle Gestelle angezeigt, für die es eine Ausgangs- und/oder Eingangsbuchung gibt.

**Auswahl Partner**
Mit der Wahl der Option legen Sie fest, nach welchen Kriterien die Gestelle in der Übersicht angezeigt werden sollen:
- **Alle:** Mit dieser Option werden alle Gestelle angezeigt, unabhängig davon, ob sie sich bei einem Kunden oder Lieferanten befinden.
- **Kunden, Lieferanten:** Mit dieser Option werden nur die Gestelle angezeigt, die sich bei einem Kunden oder einem Lieferanten befinden. In diesem Fall werden die Felder von und bis freigeschaltet.
- **Sammelgestelle:** Sammelgestelle können gesondert angezeigt werden.
  - ☐ Alle Gestelle werden angezeigt, die den übrigen Kriterien entsprechen.
  - ☑ Die Anzeige wird auf Sammelgestelle eingeschränkt.
- **[Ordner]:** Mit dieser Schaltfläche öffnen Sie den Dialog Übersicht Partner, in dem alle Gestelle aufgelistet sind, die bei dem aktuellen Partner stehen. ⇨ "Übersicht Partner" auf Seite E-2558
- **Von, bis:** Sie können die Anzeige auf Gestelle einschränken, die sich bei einem bestimmten Kunden oder Lieferanten befinden. Wenn Sie eine Anfangs- und eine Endnummer eingeben, werden alle Partner berücksichtigt, deren Nummer in dieser Spanne liegt.

**Gestelle (Übersichtstabelle)**
In der Übersicht werden alle Gestelle aufgelistet, die den Auswahlkriterien entsprechen.
- **Nummer:** Gestellnummer.
- **Art:** Gestellart.
- **Partner:** Kunde oder Lieferant, bei dem sich das Gestell befindet.
- **Ausgabe:** Datum, zu dem das Gestell außer Haus gebucht wurde.
- **Rückgabe:** Datum, zu dem der Gestelleingang gebucht wurde.
- **Buchung:** Datum der Buchung. Bei automatischen Buchungen sind das Datum der Rückgabe und das Datum der Buchung identisch.
- **Mitarbeiter:** Mitarbeiter, der die Buchung veranlasst hat.
- **Latten, Räder, Wagen:** Anzahl der Latten, Räder oder Wagen, die zu dem Gestell gehören.
- **Buchungstyp:** Bei Buchungen werden folgende Typen unterschieden: manuelle Buchung, Gestellausgang, Gestelleingang, Gestellzuordnung zu Auftrag.

### Gestellverwaltung – Mahnung

**Fertigung > Gestellverwaltung > Gestelle > Register Mahnung**

*Abb. E-121 Gestellverwaltung – Mahnung*

In diesem Register können Sie prüfen, welche Gestelle überfällig sind und angemahnt werden sollen. Die Mahnung bezieht sich immer auf alle Gestelle, die in der Übersicht mit einem Häkchen aktiviert sind.

> **i Einheitlicher Kunde**
> Achten Sie darauf, dass Sie zum Druck nur Gestelle aktivieren, die an einen einzigen Kunden oder Lieferanten gegangen sind. Markieren Sie die Zeile mit einem Doppelklick in die erste Zelle. Für jeden Kunden wird eine Mahnung gedruckt.

**Auswahl**
- **Kunde von, bis:** Sie können eine einzelne Kundennummer eingeben oder eine Spanne von Nummern. Der Name des ersten und des letzten Kunden wird angezeigt.
- **Auswärtig ... Tage:** Sie können nach Gestellen suchen, die seit einer bestimmten Anzahl von Tagen außer Haus sind, z. B. 30 - 60 Tage.
- **Mahnstatus:** Sie können die Anzeige auf die Gestelle einschränken, die bereits angemahnt wurden. Wenn Sie die Suche nicht auf eine bestimmte Mahnstufe einschränken, werden alle Gestelle angezeigt.

> **i Mahnstatus zurücksetzen**
> Wenn Sie in diesem Register den Mahnstatus zurücksetzen, wird bei allen in der Übersicht angezeigten Gestellen der Mahnstatus auf Null gesetzt. Wenn Sie den Mahnstatus für einzelne Gestelle zurücksetzen wollen, müssen Sie entweder nur das entsprechende Gestell in die Übersicht holen oder den Dialog Mahnstatus zurücksetzen im Auswahlmodus starten.
> ⇨ "Mahnstatus zurücksetzen" auf Seite E-2560

**Optionen**
- **Wiederholungsdruck:** Den Wiederholungsdruck müssen Sie dann starten, wenn Sie eine Mahnung erneut drucken wollen.
  - ☐ Die Mahnung wird zum ersten Mal gedruckt.
  - ☑ Die Mahnung wird erneut gedruckt.
- **(Versandart):** Die Mahnung kann auf verschiedene Arten versendet werden.
  - **Postversand:** Die Mahnung wird per Post versendet. Das Dokument wird ausgedruckt.
  - **Faxversand:** Die Mahnung wird per Fax versendet.
  - **Faxversand Vertreter:** Die Mahnung wird per Fax an den zuständigen Vertreter versendet.
  - **Mail:** Die Mahnung wird per Mail versendet.
  - **Mail Vertreter:** Die Mahnung wird per Mail an den zuständigen Vertreter versendet.

**Mahntexte**
- **Kopf, Fuß:** Sie können für die Kopf- und Fußzeilen der Mahnung unterschiedliche Texte auswählen. Alternativ zu den hinterlegten Texten können Sie auch in beiden Feldern einen eigenen Text schreiben.

**Auswärtige Gestelle**
In der Übersicht werden alle Gestelle angezeigt, die den Auswahlkriterien entsprechen.
- **Nummer:** Gestellnummer.
- **Art:** Gestellart.
- **Kunde:** Name des Kunden, an den das Gestell ausgeliefert wurde.
- **Faxnummer:** Faxnummer des Kunden.
- **Mail:** Mail-Adresse des Kunden. Über den Druckmodus Gestellmahnungen haben Sie die Möglichkeit, eine abweichende Mailadresse zu hinterlegen. Der Mahnungsdruck erfolgt dann bevorzugt an diese Adresse. Ist keine Mailadresse in dem Feld Gestellmahnung eingetragen, wird die Standard-Adresse verwendet.
- **Mahnstatus:** Nur bei bereits gemahnten Gestellen wird ein Mahnstatus angezeigt.
- **Ausgabedatum:** Datum, zu dem das Gestell ausgebucht wurde.
- **Tage ausw.:** Anzahl der Tage seit dem Ausgabedatum.
- **Latten, Räder, Wagen:** Anzahl der Latten, Räder und Wagen, die zum Gestell gehören.
- **Gesperrt:** Das Gestell ist für weitere Buchungen gesperrt.
- **Verloren:** Das Gestell ist nicht im Bestand, sein Verbleib kann nicht geklärt werden.
- **Stationär:** Das Gestell wird nur stationär verwendet.

## Gestellarten

**Fertigung > Gestellverwaltung > Gestellarten**

*Abb. E-122 Gestellarten*

In diesem Dialog können Sie unterschiedliche Gestellarten anlegen. Die Gestellarten werden den Gestellen zugewiesen. Sie dienen zur Organisation von Gestellen gleicher Machart.

### Gestellart

- **Bezeichnung:** Name der Gestellart.
- **Bemerkung:** Anmerkung zur Gestellart, z. B. Verwendung nicht außer Haus.
- **Max. Breite / Max. Höhe:** Größte zulässige Breite und Höhe der Scheiben, die das Gestell aufnehmen kann.
- **Eigengewicht / Max. Gew.:** Eigengewicht der Gestellart und Höchstgewicht im beladenen Zustand. Die Differenz ergibt die zulässige Beladung.
- **Gestellwert:** Als Wert des Gestells können Sie z. B. den Anschaffungspreis angeben, oder den Verleihwert.
- **Gestelltyp:** Typ des Gestells, z. B. A-Gestell oder Fächerwagen.

### Standard bei Neuanlage

- **Anzahl Spannlatten:** Die Angabe der Spannlatten dient dazu, bei der Rückgabe des Gestells dessen Vollständigkeit zu prüfen.
- **Anzahl Räder:** Die Angabe der Räder dient dazu, bei der Rückgabe des Gestells dessen Vollständigkeit zu prüfen.
- **Anzahl Wagen:** Die Angabe der Wagen dient dazu, bei der Rückgabe des Gestells dessen Vollständigkeit zu prüfen.
- **Stationär:** Gestelle können sowohl zum Transport von Gläsern dienen, als auch als Abstellplatz.
  - ☐ Das Gestell kann frei verwendet werden, z. B. auch für Lieferungen außer Haus.
  - ☑ Das Gestell hat einen festen Standort. Es kann nicht für Lieferungen verwendet werden.

### Tabelle

In der Übersicht werden alle Gestellarten aufgelistet, die den Suchkriterien entsprechen.
- **Bezeichnung:** Name der Gestellart.
- **Bemerkung:** Bemerkung zur besonderen Verwendung, Größe usw.
- **Max. Breite, max. Höhe:** Höchste zulässige Größe der Scheiben.
- **Eigengewicht:** Gewicht ohne Beladung.
- **Max. Gewicht:** Höchstgewicht im beladenen Zustand.
- **Wert:** Anschaffungs- oder Verleihwert.
- **Latten, Räder, Wagen:** Anzahl der Spannlatten, Räder und Wagen.
- **Stat.:** Angabe, ob das Gestell stationär verwendet wird.

## Gestellübersicht

**Fertigung > Gestellverwaltung > Gestelle > Register Gestelle > Schaltfläche am Feld Nummer**

*Abb. E-123 Gestellübersicht*

In diesem Dialog prüfen Sie die Gestellnummern, wenn Sie ein neues Gestell anlegen möchten.

### Gestelle

- **Gesamt:** Anzahl der angelegten Gestellnummern.
- **Verfügbar:** Anzahl der verfügbaren Gestelle.

### Auswahl

- **Gestellnummer:** Nummer des Gestells.
- **Gestellart:** Art des Gestells.
- **Kundennummer, Name:** Nummer und Name des Kunden.
- **Ausgabedatum:** Datum, zu dem das Gestell außer Haus gebucht wurde.

## Übersicht Partner

**Fertigung > Gestellverwaltung > Gestelle > Register Historie > [Ordner]**

*Abb. E-124 Gestelle - Übersicht Partner*

In diesem Dialog prüfen Sie, welche Gestelle bei einem bestimmten Marktpartner stehen oder gestanden haben.

### Auswärtig

In diesen Feldern werden die Summen angezeigt:
- **Gestelle:** Anzahl der Gestelle, die zurzeit bei diesem Partner sind.
- **Latten:** Anzahl der Latten, die zurzeit beim Partner sind.
- **Räder:** Anzahl der Räder, die zurzeit beim Partner sind.
- **Wagen:** Anzahl der Wagen, die zurzeit beim Partner sind.

### Gestelle

- **Gestellnr.:** Nummer des angelegten Gestells.
- **Gestellart:** Art des Gestells.
- **Ausgabe:** Datum, zu dem das Gestell außer Haus gebucht wurde.
- **Rückgabe:** Datum, zu dem der Gestelleingang gebucht wurde.
- **Latten, Räder, Wagen:** Anzahl der Latten, Räder oder Wagen, die zu dem Gestell gehören.

## Gestell umbuchen

**Fertigung > Gestellverwaltung > Gestelle > Menü Funktionen > Gruppe Ausführen > Gestell umbuchen**

*Abb. E-125 Gestell umbuchen*

In diesem Dialog buchen Sie ein Gestell von einem Partner auf einen anderen um.

### Auswärtige Gestelle

In der Übersicht werden alle Gestelle angezeigt, die zurzeit außer Haus sind.
- **Nummer:** Nummer des angelegten Gestells.
- **Gestellart:** Art des Gestells.
- **Kunde:** Nummer des Kunden.
- **Ausgabe:** Datum, zu dem das Gestell außer Haus gebucht wurde.

### Gestell

- **Nummer:** Nummer des markierten Gestells
- **Art:** Gestellart des markierten Gestells

### Umbuchen

- **Von:** Nummer und Name des Partners, auf den das auswärtige Gestell gebucht ist.
- **Nach:** Sie können die Nummer des neuen Partners eintragen oder über die Suche auswählen.

## Mahnstatus zurücksetzen

**Fertigung > Gestellverwaltung > Gestelle > Menü Funktionen > Gruppe Ausführen > Mahnstatus zurücksetzen**

*Abb. E-126 Mahnstatus zurücksetzen*

In diesem Dialog setzen Sie den Mahnstatus für einzelne Gestelle zurück.

## Gestellbelegung

**Fertigung > Gestellverwaltung > Gestelle > Register Gestelle > Menü Funktionen > Gruppe Ausführen > Gestellbelegung**

In diesem Dialog können Sie die Zuordnung von Auftragspositionen zu Gestellen festlegen.

> **i Voraussetzung**
> Sie können eine Zuordnung nur festlegen, wenn Sie Gestelle angelegt haben und die Gestelle verfügbar sind. Gestelle können Sie in der Gestellverwaltung im Register Gestelle anlegen.

In diesem Dialog finden Sie folgende Register:
- "Gestellbelegung - Nach Auftrag" auf Seite E-2561
- "Gestellbelegung - Nach Gestell" auf Seite E-2563

### Gestellbelegung – Nach Auftrag

**Fertigung > Gestellverwaltung > Gestelle > Menü Funktionen > Gruppe Ausführen > Gestellbelegung > Register Nach Auftrag**

*Abb. E-127 Gestellbelegung – Nach Auftrag*

In diesem Register ordnen Sie den einzelnen Positionen eines Auftrags die Gestelle zu. Sie können zusätzlich festlegen, welche Menge einer Position auf dem Gestell abgestellt werden soll. Sie können mehrere Positionen demselben Gestell zuordnen.

#### Auswahl

- **Auftrag:** Nummer des Auftrags.
- **Kunde:** Nummer und Name des Kunden. Die Felder werden gefüllt, wenn Sie die Auftragsnummer eintragen.
- **[Zuordnungen entfernen]:** Löscht alle Zuordnungen der Auftragspositionen zu den Gestellen aus der Übersicht. Wenn Sie nur eine Auftragsposition aus der Zuordnung löschen wollen, müssen Sie im Menü Start auf [Löschen] klicken.

#### Übersicht

In der Übersicht werden alle Positionen des ausgewählten Auftrags mit den Zuordnungen zu den Gestellen angezeigt. Sie können Zuordnungen zu einem Gestell bearbeiten oder neue Zuordnungen erstellen. Nur die Felder Gestell, Suche und Scheiben auf Gestell können bearbeitet werden, die anderen Felder werden automatisch gefüllt.
- **Pos:** Nummer der Auftragsposition.
- **Bezeichnung:** Bezeichnung des Glases.
- **Breite, Höhe:** Maße der Position.
- **Positionsmenge:** Stückzahl der Position.
- **Gewicht pro Stück:** Gewicht eines Stücks der Position.
- **Noch nicht abgestellt:** Stückzahl der Position, die noch keinem Gestell zugeordnet ist.
- **Gestell:** Nummer des Gestells, dem die Position zugeordnet werden soll.
- **Max. Höhe, Max Breite:** Höchste zulässige Maße der Scheiben. Die Felder werden automatisch gefüllt, wenn eine Gestellnummer eingetragen ist.
- **Max. Gewicht:** Höchstgewicht im beladenen Zustand. Das Feld wird automatisch gefüllt, wenn eine Gestellnummer eintragen ist.
- **Suche:** Öffnet den Dialog Gestellübersicht, in dem Sie ein Gestell wählen können. Die Maße und das Gewicht des gewählten Gestells werden in der Tabelle übernommen. Das Feld Scheiben auf Gestell wird standardmäßig mit der Stückzahl aus dem Feld Positionsmenge gefüllt.
- **Scheiben auf Gestell:** Stückzahl der Scheiben, die dem gewählten Gestell zugeordnet werden sollen. Wenn Sie dem Gestell weniger Scheiben zuordnen als die Gesamtstückzahl der Position, wird automatisch eine neue Zeile mit der Differenzstückzahl der Position angezeigt. Sie können diese Stückzahl einem anderen Gestell zuordnen.

- **Gesamt:** Gesamtstückzahl der Auftragspositionen.
- **Rest:** Gesamtstückzahl der Positionen, die keinem Gestell zugeordnet sind.
- **Auf Gestell:** Gesamtstückzahl der Positionen, die einem Gestell zugeordnet sind.

### Gestellbelegung – Nach Gestell

**Fertigung > Gestellverwaltung > Gestelle > Menü Funktionen > Gruppe Ausführen > Gestellbelegung > Register Nach Gestell**

*Abb. E-128 Gestellbelegung – Nach Gestell*

In diesem Register ordnen Sie einem Gestell einzelne Positionen eines Auftrags zu. Sie können zusätzlich festlegen, welche Menge einer Position auf dem Gestell abgestellt werden soll.

#### Auswahl

- **Gestell/Gestellart:** Nummer und Art des Gestells. Sie können nur die Nummer des Gestells angeben, dem Positionen zugeordnet werden sollen. Das Feld Gestellart wird gefüllt.
- **Max. Breite/Höhe/Gewicht:** Höchste zulässige Maße der Scheiben und Höchstgewicht des beladenen Gestells. Die Felder werden gefüllt, wenn Sie eine Gestellnummer eintragen.
- **[Gestell leeren]:** Löscht alle Zuordnungen der Auftragspositionen zu dem markierten Gestell aus der Übersicht. Wenn Sie nur eine Auftragsposition aus der Zuordnung löschen wollen, müssen Sie im Menü Start auf [Löschen] klicken.

#### Übersicht

In der Übersicht werden alle Positionen angezeigt, die dem ausgewählten Gestell zugeordnet sind. Sie können die Zuordnungen bearbeiten oder Positionen neu zuordnen. Nur die Felder Auftrag, Pos und Scheiben auf Gestell können bearbeitet werden, die anderen Felder werden automatisch gefüllt.

- **Auftrag:** Nummer des Auftrags.
- **Pos:** Nummer der Auftragsposition.
- **Bezeichnung:** Bezeichnung des Glases.
- **Maße:** Maße der Position.
- **Kunde:** Nummer des Kunden.
- **Maximal abstellbar:** Stückzahl der Position, die noch keinem Gestell zugeordnet ist.
- **Gewicht:** Gewicht der Stückzahl einer Position, die einem Gestell zugeordnet ist.
- **Scheiben auf Gestell:** Stückzahl der Scheiben, die dem gewählten Gestell zugeordnet werden sollen.

- **Gesamt:** Gesamtstückzahl der Auftragspositionen.
- **(Gewicht) Auf Gestell:** Gesamtgewicht der Positionen, die dem Gestell zugeordnet sind.
- **Auf Gestell:** Gesamtstückzahl der Positionen, die dem Gestell zugeordnet sind.

## Kundenkommissionen

**Fertigung > Gestellverwaltung > Kundenkommissionen**

Mit der Kundenkommission werden weitere Details für den Versand festgelegt.

In diesem Dialog finden Sie folgende Register:
- "Kundenkommissionen - Kommission" auf Seite E-2565
- "Kundenkommissionen - Abladestelle" auf Seite E-2566
- "Kundenkommissionen – Zuordnung" auf Seite E-2567

### Kundenkommissionen – Kommission

**Fertigung > Gestellverwaltung > Kundenkommissionen > Register Kommission**

*Abb. E-129 Kundenkommissionen - Kommission*

In diesem Register legen Sie die Standard-Kommission des Kunden fest. Dadurch können Sie im Auftrag bei der Positionserfassung die gewünschte Kommission auswählen.
⇨ Softwarereferenz, "Kommission" auf Seite C-1730

### Kundenkommissionen – Abladestelle

**Fertigung > Gestellverwaltung > Kundenkommissionen > Register Abladestelle**

*Abb. E-130 Kundenkommissionen - Abladestelle*

In diesem Register geben Sie an, welche Abladestellen beim Kunden in der Regel angefahren werden.

### Kundenkommissionen – Zuordnung

**Fertigung > Gestellverwaltung > Kundenkommissionen > Register Zuordnung**

*Abb. E-131 Kundenkommissionen – Zuordnung*

In diesem Register ordnen Sie die Kommissionen den Abladestellen zu.

# Terminübersicht

**Fertigung > Terminübersicht > Terminübersicht**

In der Terminübersicht können Sie sich anzeigen lassen, was in einem bestimmten Zeitraum produziert werden muss und welche Materialien dazu benötigt werden.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menüs in der Terminübersicht" auf Seite E-2568
- "Terminübersicht (Dialog)" auf Seite E-2569
- "Exportieren" auf Seite E-2576

## Menüs in der Terminübersicht

Über die Menüs im Dialog Terminübersicht können Sie die Standardeinstellung des Dialoges festlegen und andere Dialoge öffnen, ohne die Terminübersicht zu schließen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite E-2568
- "Menü Optionen" auf Seite E-2569

### Menü Funktionen

**Fertigung > Terminübersicht > Terminübersicht > Menü Funktionen**

Im Register Tabelle können Sie über dieses Menü andere Dialoge öffnen, ohne die Terminübersicht zu schließen.

**Gruppe Dokument**
- **Historie:** Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des markierten Dokuments. Eine ausführliche Beschreibung finden Sie im Part Verkauf. ⇨ Verkauf, "Historie" auf Seite C-1834
- **Anzeigen:** Öffnet den Dialog Dokumentenansicht zu einer Vorschau auf das Dokument. Eine ausführliche Beschreibung finden Sie im Part Verkauf. ⇨ Verkauf, "Reklamationen" auf Seite C-1875

**Gruppe Auswahl**
- **Exportieren:** Öffnet den Dialog Export, in dem Sie auswählen können, welche Daten in eine Exportdatei geschrieben werden sollen. ⇨ "Exportieren" auf Seite E-2576

### Menü Optionen

**Fertigung > Terminübersicht > Terminübersicht > Menü Optionen**

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellungen werden nicht zurückgesetzt, wenn Sie den Dialog schließen. Folgende Einträge werden angezeigt:

- **Automatischer Seitenvorschub aktiv:** Im Druck wird nach jedem Datum und Auftrag ein Seitenumbruch eingefügt.
- **Archiv:** Das Archiv wird herangezogen, z. B. um Vergleichszeiträume des Vorjahrs zu auszuwerten.

## Terminübersicht (Dialog)

**Fertigung > Terminübersicht > Terminübersicht**

In der Terminübersicht wird angezeigt, welche Mengen in einem bestimmten Zeitraum produziert werden müssen und welche Materialien dazu benötigt werden. Die Auswertungen können gedruckt oder exportiert werden.

In diesem Dialog finden Sie folgende Register:
- "Terminübersicht - Auswahl" auf Seite E-2570
- "Terminübersicht - Tabelle" auf Seite E-2575

### Terminübersicht – Auswahl

**Fertigung > Terminübersicht > Terminübersicht > Register Auswahl**

*Abb. E-132 Terminübersicht - Auswahl*

In diesem Register legen Sie die Kriterien für die Aufträge fest, die im Register Tabelle angezeigt werden sollen.
⇨ "Terminübersicht - Tabelle" auf Seite E-2575

#### Quelle

Mit der Wahl der Option legen Sie fest, wie Sie nach Aufträgen suchen wollen:
- **Nummer:** Sie können sich einen einzelnen Auftrag anzeigen lassen. Die Felder für die Eingabe der Auftragsnummer und den Auswertungszeitraum werden freigeschaltet.
- **Nummernverwalter:** Sie können sich die Aufträge eines Nummernverwalters anzeigen lassen. Das Feld für die Auswahl des Nummernverwalters wird freigeschaltet.

> **i Material pro Auftrag**
> Wenn Sie einen einzelnen Auftrag auswählen, können Sie sich über den Auswertungsmodus und die Auflösungstiefe eine Liste aller Materialien erstellen, die in dem gewählten Auftrag verbraucht werden.

- **Mandant:** Wenn Sie mit Mandanten arbeiten, können Sie die Auswahl auf einen bestimmten einschränken.
- **AV-Bereich:** Wenn Sie mit AV-Bereichen arbeiten, können Sie die Auswahl auf einen bestimmten einschränken.

#### Auswertungsmodus

Mit der Wahl der Option legen Sie fest, wie die Aufträge ausgewertet werden sollen:
- **Produktionsbereich:** Die Felder in Bereich Produktionsbereich werden freigeschaltet, so dass Sie den gewünschten Bereich wählen können.
- **Warengruppen:** Die Felder in Bereich Auswahl Warengruppe werden freigeschaltet, so dass Sie eine WGR wählen können.
- **Produkt:** Die Felder in Bereich Auswahl Produkt werden freigeschaltet, so dass Sie ein Produkt wählen können.

#### Auswertungszeitraum

Die Felder in diesem Bereich sind nur freigeschaltet, wenn Sie im Bereich Quelle die Option Nummer gewählt haben und das Feld leer lassen. Sie können sich dann alle Aufträge eines bestimmten Zeitraums anzeigen lassen.
- **Nach Liefertermin:** Der eingegebene Zeitraum bezieht sich auf den Liefertermin.
- **Nach Produktionstermin:** Der eingegebene Zeitraum bezieht sich auf den Produktionstermin.
- **Von, bis:** Zeitraum, der ausgewertet werden soll. Wenn Sie in beiden Feldern dasselbe Datum eingeben, wird nur ein Tag ausgewertet.

#### Produktionsbereiche

Mit der Wahl der Option legen Sie fest, welchen Produktionsbereich Sie betrachten wollen. Die Felder sind nur freigeschaltet, wenn Sie den Auswertungsmodus nach Produktionsbereich gewählt haben.
- **Isolierglas:** Nur Aufträge mit ISO-Positionen werden angezeigt.
- **VSG:** Nur Aufträge mit VSG-Positionen werden angezeigt.
- **ESG:** Nur Aufträge mit ESG-Positionen werden angezeigt.
- **EFG:** Nur die Aufträge werden angezeigt, in denen Einfachglas (EFG) erfasst ist. Dies gilt auch für Einfachglas, das in ISO verarbeitet wird.
- **Zuschnitt:** Alle Aufträge werden angezeigt, in denen Glas zugeschnitten werden soll.
- **ISO Hilfsstoffe:** Alle Aufträge werden angezeigt, in denen ISO-Hilfsstoffe erfasst sind.
- **Alles:** Alle Aufträge werden angezeigt.

#### Restriktionen

Sie können die Auswertung zusätzlich auf eine der angezeigten Nebenbedingungen einschränken. Die Checkboxen Modellzuschnitt bis Bearbeitungen sind nur freigeschaltet, wenn Sie den Auswertungsmodus nach Produktionsbereich gewählt haben.

- **Modellzuschnitt:** Sie können die Auswertung auf Modelle einschränken.
  - ☐ Die Auswertung ist nicht auf Modelle eingeschränkt.
  - ☑ In der Auswertung werden nur Positionen mit Modell angezeigt.
- **Sprossenproduktion:** Sie können die Auswertung auf Sprossenkonstruktionen einschränken.
  - ☐ Die Auswertung ist nicht auf Sprossen eingeschränkt.
  - ☑ In der Auswertung werden nur Positionen mit Sprossenkonstruktionen angezeigt.
- **Stufung:** Sie können die Auswertung auf Stufungen einschränken.
  - ☐ Die Auswertung ist nicht auf Stufungen eingeschränkt.
  - ☑ In der Auswertung werden nur Positionen mit Stufungen angezeigt.
- **Bearbeitungen:** Sie können die Auswertung auf Bearbeitungen einschränken.
  - ☐ Die Auswertung ist nicht auf Bearbeitungen eingeschränkt.
  - ☑ In der Auswertung werden nur Positionen mit Bearbeitungen angezeigt.
- **Eigenfertigung:** Sie können die Auswertung auf Eigenfertigungen einschränken. Als Eigenfertigungen gelten Aufträge mit den Beschaffungsarten Zuschnitt, Produktion, Bearbeitung.
  - ☐ Die Auswertung ist nicht auf Eigenfertigungen eingeschränkt.
  - ☑ In der Auswertung werden nur Positionen mit Eigenfertigungen angezeigt.
- **Lager:** Sie können die Auswertung auf Lagerartikel einschränken.
  - ☐ Die Auswertung ist nicht auf Lagerartikel eingeschränkt.
  - ☑ In der Auswertung werden nur Positionen mit Lagerartikeln angezeigt.
- **Einkauf:** Sie können die Auswertung auf Zukaufartikel einschränken.
  - ☐ Die Auswertung ist nicht auf Zukaufartikel eingeschränkt.
  - ☑ In der Auswertung werden nur Positionen mit Zukaufartikeln angezeigt.

#### Auswahl Statusbereich

Mit der Eingrenzung auf einen Status können Sie z. B. Angebote oder Aufträge auswählen, die noch nicht an die Produktion übergeben wurden.
- **Von, Bis:** In den Komboboxen werden alle Statuspunkte angezeigt, die in den Stammdaten definiert sind.

#### Auswahl Warengruppe

Mit der Wahl der Option legen Sie fest, welche Warengruppe Sie betrachten wollen. Die Felder sind nur freigeschaltet, wenn Sie den Auswertungsmodus nach Warengruppen gewählt haben.

- **WGR:** Alle Aufträge mit Produkten aus einer bestimmten Warengruppe werden betrachtet. Das Feld zur Auswahl der Warengruppe wird freigeschaltet. Sie können die WGR aus jeder der drei Ebenen der Warengruppen auswählen. Wenn Sie das Feld frei lassen, werden alle Warengruppen angezeigt.
- **WGR-Statistik:** Das Feld zur Auswahl der Statistik-Warengruppe wird freigeschaltet. Sie können eine Warengruppe (WGR), Warenobergruppe (WOG) oder Warenhauptgruppe (WHG) auswählen. Die Auswertung selbst zeigt jedoch immer nur die WHG. Wenn für Ihre Übersicht auch Warengruppen (WGR) oder Warenobergruppen (WOG) wichtig sind, können Sie zum Dialog Kapazitätsübersicht wechseln. ⇨ "Kapazitätsübersicht" auf Seite E-2577

- **Kombinations-Warengruppe:** Die Auswertung kann Kombinations-Warengruppen (Kombi-WGR) einbeziehen.
  - ☐ Die Original-WGR der Produkte werden angezeigt.
  - ☑ Die Kombi-WGR werden angezeigt.

> **Beispiel:**
> Float 4 = WGR 100
> Lochbohrung = WGR 801
> Float 4 mit Lochbohrung (Kombination 100 und 801) = Kombi-WGR 860
> - ☐ Die Auswertung auf WGR-Ebene zeigt die WGR 100 und 801 an.
> - ☑ Die WGR 860 wird angezeigt.

#### Auswahl Produkt

Sie können die Auswertung auf Aufträge einschränken, in denen ein bestimmtes Produkt erfasst ist. Die Felder sind nur freigeschaltet, wenn Sie den Auswertungsmodus nach Produkt gewählt haben.
- **Produktart:** Sie können die Auswertung auf eine Produktart einschränken, z. B. auf die Produktart Artikel, um zu prüfen, welches Zubehör für die Produktion bestellt werden muss.
- **Produktgruppe:** Eine Produktgruppe können Sie nur auswählen, nachdem Sie eine Produktart gewählt haben.
- **Produkt:** Sie können die Auswertung auf ein ganz bestimmtes Produkt einschränken.

#### Auflösungstiefe

Die Auflösungstiefe bestimmt, wie detailliert die Aufträge dargestellt werden. Sie können mehrere Checkboxen markieren.

- **Pro Datum:** Die Aufträge können pro Liefertermin angezeigt werden. Diese Einstellung ist dann sinnvoll, wenn Sie sich z. B. einen Überblick über die Produkte verschaffen wollen, die in der nächsten Woche produziert werden sollen.
  - ☐ Der Liefertermin wird nicht herangezogen.
  - ☑ Die Aufträge werden nach Lieferterminen gruppiert.
- **Pro Auftrag:** Die Auswertung betrachtet jeden Auftrag einzeln. Diese Einstellung ist z. B. dann sinnvoll, wenn Sie einen Produktionsbereich ausgewählt haben.
  - ☐ Einzelne Aufträge werden nicht dargestellt.
  - ☑ Die Anzeige wird nach Aufträgen gruppiert.
- **Pro Position:** Die Auswertung betrachtet jede einzelne Position der Aufträge. Die Checkbox ist nur freigeschaltet, wenn die Checkbox pro Auftrag markiert ist. Diese Einstellung ist z. B. dann sinnvoll, wenn Sie Aufträge mit vielen Positionen und großen Stückzahlen auswerten.
  - ☐ Einzelne Positionen werden nicht dargestellt.
  - ☑ In der Anzeige werden für jeden Auftrag die Positionen angezeigt.
- **Pro Kunde:** Die Aufträge können pro Kunde angezeigt werden. Diese Einstellung ist z. B. dann sinnvoll, wenn Sie die Aufträge eines Kunden auswerten wollen.
  - ☐ Einzelne Kunden werden nicht dargestellt.
  - ☑ Die Aufträge werden nach Kunden gruppiert.
- **Zwischensumme pro ME:** Sie können Sie jeweils eine Zwischensumme anzeigen lassen.
  - ☐ Die Zwischensumme wird nicht angezeigt.
  - ☑ Pro Auftrag wird die Zwischensumme für die Mengeneinheiten angezeigt, die in den Positionen erfasst sind.

#### Berechnung Gas

- **Gasberechnung individuell:** Sie können die Anzeige der Mengeneinheit von Gas ändern. Wenn z. B. das Produkt Gas in den Produktstammdaten mit der Mengeneinheit kg angelegt ist, können Sie verbrauchte Menge in Liter anzeigen lassen.
  - ☐ Die Gasberechnung wird nicht umgerechnet.
  - ☑ Die Gasberechnung wird auf die neue Mengeneinheit umgerechnet.
- **Mengeneinheit:** Angabe der neuen Mengeneinheit. Die Menge wird nur umgerechnet, wenn die Checkbox Gasberechnung individuell aktiviert ist.

### Terminübersicht – Tabelle

**Fertigung > Terminübersicht > Terminübersicht > Register Tabelle**

*Abb. E-133 Terminübersicht - Tabelle*

Im diesem Register werden alle Aufträge angezeigt, die den Kriterien entsprechen, die Sie im Register Auswahl festgelegt haben.
⇨ "Terminübersicht - Auswahl" auf Seite E-2570

#### Ergebnis

In der Übersicht wird die Auswertung angezeigt. Die Darstellung der Spalten hängt von den gewählten Kriterien ab. Sie können sich jeden Auftrag über das Menü Funktionen > Dokument > Anzeigen in der Dokumentenansicht anzeigen lassen.

#### Summen

In der Übersicht werden die Gesamtsummen über alle Aufträge im Bereich Ergebnis angezeigt.

## Exportieren

**Fertigung > Terminübersicht > Terminübersicht > Menü Funktionen > Gruppe Auswahl > Exportieren**

*Abb. E-134 Export der Terminübersicht*

Mit der Funktion Exportieren haben Sie die Möglichkeit, die Daten für weitere Auswertungen in eine ASCII-Datei zu exportieren.

- **Pfad/Dateiname:** In diesem Feld tragen Sie den Pfad und den Dateinamen für die Übergabedatei ein. Schreiben Sie als Format ASC oder TXT. Im Feld Exportiert wird nach dem Export angezeigt, wie viele Datensätze in die Datei geschrieben wurden.
- **Export-Felder:** In diesem Bereich sind die Felder angezeigt, aus denen Daten exportiert werden können. Das jeweilige Kennzeichen für das Darstellungsformat wird zur Information angezeigt.

## Kapazitätsübersicht

**Fertigung > Terminübersicht > Kapazitätsübersicht**

*Abb. E-135 Kapazitätsübersicht*

In diesem Dialog können Sie sich pro Liefertermin eine Vorschau auf die Kapazitäten anzeigen lassen, die für die Produktion von bestimmten Warengruppen benötigt werden.

> **i Keine Verbindung zur Kapazitätsplanung**
> Die Kapazitätsübersicht steht nicht in Verbindung mit der A+W Business-Kapazitätsplanung und verarbeitet keine Rückmeldungen aus der Produktion.

### Auflösung nach

Mit der Wahl der Option legen Sie die Auflösungstiefe fest. Dazu können Sie zusätzlich einzelne Warengruppen auswählen.
- **Warenhauptgruppe:** Nur Warenhauptgruppen (WHG) werden ausgewertet.
- **Warenobergruppe:** Innerhalb der WHG wird nach Warenobergruppen (WOG) differenziert.
- **Warengruppe:** Innerhalb der WOG wird nach Warengruppen (WGR) differenziert.

### Warengruppen

- **Alle:** Sie können einzelne Warengruppen auswählen. Die Auswahl ist abhängig von der gewählten Auflösung.
  - ☐ Einzelne Warengruppen sollen ausgewertet werden. Die Felder zur Auswahl sind freigeschaltet. Sie können eine Anfangs- und eine Endnummer eingeben. Wenn Sie zusätzlich die Stücklisten mit auswerten, werden deren Warengruppen durch die eingestellte Auswahl nicht ausgeblendet.
  - ☑ Alle Warengruppen sollen ausgewertet werden.
- **Mit Stückl.:** Bei der Auswertung können die Stücklisten mit einbezogen werden.
  - ☐ Die Stücklisten werden nicht ausgewertet. Das bedeutet z. B., dass das für die Produktion von ISO benötigte Float nicht berücksichtigt wird.
  - ☑ Die Stücklisten werden mit ausgewertet. Diese Einstellung ist z. B. sinnvoll, wenn Sie wissen wollen, wie viele Rahmen oder Sprossen erfasst sind.

### Auftragsstatus

- **Von, bis:** Sie können die Auswertung auf den Status der Aufträge eingrenzen. Um eine Vorschau zu erhalten, ist es sinnvoll, den Status bis vor Produktionsübergabe einzustellen.

### Lieferdatum

- **Von, bis:** Sie können die Auswertung auf Aufträge eingrenzen, die in einem bestimmten Zeitraum geliefert werden müssen.

### Übersicht

In der Übersicht werden pro Datum alle WHG, WOG oder WGR aufgelistet, die den Auswahlkriterien entsprechen.
- **Lieferdatum:** Lieferdatum innerhalb des gewählten Zeitraums. Nach dem letzten Eintrag zum angezeigten Datum wird eine Summenzeile eingefügt, in der die Werte in roter Schrift angezeigt sind.
- **WHG, WOG, WGR:** Nummer der Warengruppe. Die Anzeige richtet sich nach der Wahl der Auflösung.
- **Bezeichnung:** Bezeichnung der Warengruppe.
- **Anzahl:** Stückzahl aller Auftragspositionen, die zu der Warengruppe gehören.
- **Fläche:** Gesamtfläche aller Auftragspositionen, die zu der Warengruppe gehören.
- **Gewicht:** Gesamtgewicht aller Auftragspositionen, die zu der Warengruppe gehören.
- **Betrag netto:** Verkaufswert aller Auftragspositionen, die zu der Warengruppe gehören.

Im unteren Bereich der Übersicht werden die Gesamtsummen der angezeigten Warengruppe angezeigt.

## Fertigungsvorschau

**Fertigung > Terminübersicht > Fertigungsvorschau**

Pro Liefertermin können Sie zu den Produktarten Isolierglas, Einfachglas, ESG und VSG die Summe der Glasflächen anzeigen lassen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Fertigungsvorschau (Dialog)" auf Seite E-2580
- "Definition Vorschauspalten" auf Seite E-2581
- "Ausschluss von Geschäftsarten" auf Seite E-2582

### Menü Optionen

**Fertigung > Terminübersicht > Fertigungsvorschau**

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Fertigungsvorschau zu schließen. Folgende Einträge werden angezeigt:

**Gruppe Anzeige**
- **Spaltendefinition:** Öffnet den Dialog Definition Vorschauspalten, in dem Sie festlegen können, welche Spalten angezeigt werden. ⇨ "Definition Vorschauspalten" auf Seite E-2581
- **Geschäftsarten ausblenden:** Öffnet den Dialog Ausschluss von Geschäftsarten, in dem Sie festlegen können, welche Geschäftsarten nicht angezeigt werden sollen. ⇨ "Ausschluss von Geschäftsarten" auf Seite E-2582

**Gruppe Termin**
Über dieses Menü können Sie auswählen, auf welchen Termin sich die Vorschau beziehen soll:
- **Nach Liefertermin:** Die Vorschau bezieht sich auf den Liefertermin.
- **Nach Produktionsende:** Die Vorschau bezieht sich auf das Produktionsende.

## Fertigungsvorschau (Dialog)

**Fertigung > Terminübersicht > Fertigungsvorschau**

*Abb. E-136 Fertigungsvorschau*

In diesem Dialog können Sie sich eine Vorschau auf die Mengen einzelner Produkte oder Produktarten anzeigen lassen. In den verschiedenen Registern werden die Vorschaudaten für die jeweilige Glasart angezeigt.

Die Spalten können pro Arbeitsplatz individuell eingestellt werden.
⇨ Tutorial, "Fertigungsvorschau" auf Seite E-2456

Die Fertigungsvorschau analysiert alle Aufträge nach quantitativen Gesichtspunkten und informiert über die zukünftige Auslastung nach Produktarten und Produktgruppen. Für die Auswertung werden alle aktuellen Aufträge mit Versandtag größer gleich dem aktuellen Tagesdatum herangezogen. Die Auswertungskriterien sind jeweils eine Kombination von Produktart und Produktgruppe.

Das Auswertungsergebnis wird jeweils in einer Datenbanktabelle gespeichert und beim Aufruf des Dialogs sofort angezeigt. Die Anzeige kann manuell aktualisiert werden. Das letzte Aktualisierungsdatum wird mit Stunde und Minute angezeigt.

## Definition Vorschauspalten

**Fertigung > Terminübersicht > Fertigungsvorschau > Menü Optionen > Gruppe Anzeige > Spaltendefinition**

*Abb. E-137 Spaltendefinition für die Fertigungsvorschau*

In diesem Dialog legen Sie fest, welche Einstellungen firmenübergreifend gelten sollen. Sie brauchen Administratorrechte, um diesen Dialog zu öffnen.

### Spalten

- **Nr.:** Der fortlaufende Zähler wird bei der Spalteneingabe gesetzt.
- **Bezeichnung:** Der Titel für die Spaltenüberschrift ist frei wählbar, z. B. Isolierglas.
- **Bezeichnung 2:** Der Titel für die Spaltenüberschrift ist frei wählbar, z. B. die Mengeneinheit.
- **Typ HP:** Die Typauswahl auf Basis des Hauptprodukts:
  - 1 = Produktart
  - 2 = Produktgruppe
- **HP:** Das Hauptprodukt entspricht der Schlüsselnummer der in den Artikelstammdaten hinterlegten Produktart oder Produktgruppe.
- **Typ 0:** Die Typauswahl auf Basis des Hauptprodukts:
  - 1 = Produktart
  - 2 = Produktgruppe
- **Nr. 0:** Die Schlüsselnummer für die Produktart oder die Produktgruppe je nach Typ.
- **ST/QM:** Darstellung der Mengen (Maßeinheit)
  - 1 = Stück
  - 2 = Qm
- **GR.-Klasse:** Die Größenklassen werden durch Von-bis-Werte festgelegt, die sich auf die Maßeinheit beziehen.

## Ausschluss von Geschäftsarten

**Fertigung > Terminübersicht > Fertigungsvorschau > Menü Optionen > Gruppe Anzeige > Geschäftsarten ausblenden**

*Abb. E-138 Ausschluss von Geschäftsarten*

In diesem Dialog legen Sie fest, welche Geschäftsarten nicht angezeigt werden sollen. Sie brauchen Administratorrechte, um diesen Dialog zu öffnen.
Zur Wahl stehen alle Geschäftsarten, die in den Stammdaten > Auftrag hinterlegt sind.

# Zollverwaltung

**Fertigung > Zollverwaltung**

In diesem Bereich können Sie verschiedene Zoll-Listen für den Warenexport erstellen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Zollverwaltungsliste" auf Seite E-2583
- "Listennummer zurücksetzen" auf Seite E-2587
- "Produktgruppe mit Positionsmenge" auf Seite E-2587
- "Zoll-Export" auf Seite E-2588
- "Export Artikelstammdaten" auf Seite E-2590

## Zollverwaltungsliste

**Fertigung > Zollverwaltung > Zollvw.-Liste**

Für die Zollpapiere können Sie verschiedene Ladelisten erstellen.

In diesem Dialog finden Sie folgende Register:
- "Ladeliste - Nummernverwalter" auf Seite E-2584
- "Ladeliste - Zollverwaltungslisten" auf Seite E-2586

### Menü Funktionen

In diesem Menü finden Sie folgende Einträge:
- **Listennummer zurücksetzen:** Öffnet den gleichnamigen Dialog, in dem Sie die zuletzt verwendete Nummer der Zoll-Liste zurücksetzen können. ⇨ "Listennummer zurücksetzen" auf Seite E-2587
- **Produktgruppe ohne Stkl.-Auflösung:** Öffnet den Dialog Produktgruppe mit Positionsmengen, in dem Sie bestimmte Produkte ausschließen können. ⇨ "Produktgruppe mit Positionsmenge" auf Seite E-2587

### Ladeliste – Nummernverwalter

**Fertigung > Zollverwaltung > Zollvw.-Liste > Register Nummernverwalter**

*Abb. E-139 Ladeliste - Nummernverwalter*

In diesem Dialog können Sie den Nummernverwalter auswählen, in dem Sie die Aufträge für die Zollverwaltungsliste gesammelt haben.

> **i Voraussetzungen**
> Sie können Zollpapiere nur drucken, wenn den Produkten und/oder Warengruppen Zolltarifnummern zugeordnet sind.

#### Identifikation

- **Mandant:** Wenn Sie mit unterschiedlichen Mandanten arbeiten, werden diese zur Auswahl angeboten.
- **Mitarbeiter:** Name des Mitarbeiters, der sich in A+W Business angemeldet hat.
- **Nummernverwalter:** Auswahl des Nummernverwalters, in dem Sie die Aufträge für den Warenexport gesammelt haben.

#### Eingabe

- **Zollübergang von, Zollübergang nach:** Auswahl der Grenzübergänge, die der Lkw benutzen wird. Zur Auswahl werden alle Grenzübergänge angeboten, die Sie in den Stammdaten hinterlegt haben. Eine Beschreibung finden Sie im Part Stammdaten. ⇨ Stammdaten, "Zolltouren" auf Seite B-1000
- **NV Proforma Rechnung:** Auswahl des Nummernverwalters, in dem die Proforma-Rechnungen gesammelt werden.
- **Gewichtsfaktor:** Angabe des Gewichtsfaktors, wenn das Bruttogewicht als Bemessungsgrundlage für die Berechnung des Zolls herangezogen wird.
- **Liefertermin:** Angabe des Liefertermins, der in die Zollpapiere gedruckt werden soll.

#### Übersicht

In der Übersicht werden alle Aufträge aus dem Nummernverwalter aufgelistet.
- **Auftrag:** Auftragsnummer.
- **Nummer Kunde/Lief., Kunde/Lieferant:** Nummer und Name des Kunden oder Lieferanten.
- **Status:** Auftragsstatus.
- **Lieferschein:** Nummer des Lieferscheins.
- **Datum Lieferung:** Lieferdatum aus dem Auftrag.
- **Stückzahl gesamt:** Stückzahl aller Positionen pro Auftrag.
- **Gewicht gesamt:** Gewicht aller Positionen pro Auftrag.

### Ladeliste – Zollverwaltungslisten

**Fertigung > Zollverwaltung > Zollvw.-Liste > Register Zollverwaltungslisten**

*Abb. E-140 Ladeliste - Zollverwaltungslisten*

In diesem Register können Sie sich die Zollverwaltungslisten anzeigen und drucken lassen.

#### Eingabe

- **Zollverwaltungsliste Nr.:** In diesem Feld wird die Nummer der Zollverwaltungsliste angezeigt. Die Nummer wird automatisch von System vergeben, wenn eine neue Liste erstellt wird. Im Auswahlmodus können Sie sich jede Liste anzeigen lassen, die zuvor erstellt wurde.

Mit der Wahl der Option legen Sie die Art der Liste fest:
- **Zollverwaltungsliste anzeigen:** Mit dieser Option können Sie die erfassten Zollverwaltungslisten anzeigen.
- **Zollverwaltungslistennachweis:** Mit dieser Option können Sie die erfassten Artikel einer Zollverwaltungsliste anzeigen lassen.

## Listennummer zurücksetzen

**Fertigung > Zollverwaltung > Zollvw.-Liste > Menü Funktionen > Listennummer zurücksetzen**

*Abb. E-141 Listennummer zurücksetzen*

In diesem Dialog können Sie die Nummer der Zollverwaltungsliste zurücksetzen.

## Produktgruppe mit Positionsmenge

**Fertigung > Zollverwaltung > Zollvw.-Liste > Menü Funktionen > Produktgruppe ohne Stkl.-Auflösung**

*Abb. E-142 Produktgruppe ohne Stücklisten-Auflösung*

In diesem Dialog können Sie die Produktgruppe auswählen, bei der die Stücklistenmenge nicht berücksichtigt werden soll.
Damit wird bei Produktgruppen mit der Produktart Artikel nur die Menge der Position in die Zollverwaltungsliste übernommen.

## Zoll-Export

**Fertigung > Zollverwaltung > Zollexport**

### Menü Funktionen

**Fertigung > Zollverwaltung > Zollexport > Menü Funktionen**

Über dieses Menü können Sie den Dialog öffnen, in dem Sie den Pfad für eine Schnittstellendatei für Stammdaten erstellen können.
⇨ "Export Artikelstammdaten" auf Seite E-2590

### Zoll-Export (Dialog)

**Fertigung > Zollverwaltung > Zollexport**

*Abb. E-143 Zoll-Export*

In diesem Dialog können Sie eine Schnittstellendatei schreiben, die von Zoll-Programmen importiert werden kann.

#### Modus

Die Datei kann für verschiedene Schnittstellen angefertigt werden. In der Kombobox sind alle Schnittstellen aufgeführt, für die eine Exportdatei geschrieben werden kann.

#### Identifikation

- **Nummernverwalter:** Nur die Aufträge werden in der Übersicht angezeigt, die dem eingestellten Nummernverwalter entsprechen.
- **Status von, bis:** Sie können die Anzeige der Aufträge auf einen Status eingrenzen, z. B. auf Lieferschein oder Rechnung gedruckt.

#### Pfad der Ausgabedatei

Angabe des Orts, an dem die Schnittstellendateien gespeichert werden sollen.

#### Mandant

Wenn Sie mit Mandaten arbeiten, können Sie die Schnittstellendatei für jeden Mandanten einzeln erstellen. In diesem Feld tragen Sie den Namen des Mandanten ein.

#### Format der Ausgabedatei

Mit der Wahl der Option legen Sie das Dateiformat fest:
- **ANSI:** Diese Einstellung erzeugt eine reine ASCII-Datei nach dem ANSI-Standard.
- **OEM:** Diese Einstellung erzeugt eine Datei nach dem Format anderer Hersteller, das dem Standard entspricht.

#### Dokumente

In der Übersicht werden alle Aufträge angezeigt, die den Auswahlkriterien entsprechen.
- **Auftragsnummer:** Nummer des Auftrags.
- **Kundennummer, Kunde:** Nummer und Name des Kunden aus dem Auftrag.
- **PLZ, Ort:** Geschäftsort des Kunden.
- **Land:** Land, in dem der Kunde seinen Geschäftssitz hat.
- **Nettobetrag, Nettobetrag FW:** Nettobetrag des Auftrags in Eigen- und in Fremdwährung.
- **Datum Rechnung:** Datum der Rechnung.
- **Status:** Status des Auftrags.
- **Produktnummer:** Nummer des Produkts aus den Stammdaten.
- **Anzahl Produkte:** Menge der Produkte.
- **ISO-Glas, VSG-Glas:** Stückzahl ISO, VSG.

## Export Artikelstammdaten

**Fertigung > Zollverwaltung > Zoll-Export > Menü Funktionen > Stammdaten-Export**

*Abb. E-144 Export von Artikelstammdaten*

In diesem Dialog können Sie die Stammdaten der Produkte oder der Kundenprodukte in eine Schnittstellendatei schreiben. Exportiert werden nur die Daten der Aufträge, die im Dialog Zoll-Export angezeigt werden.

- **Pfad Ausgabedatei:** In diesem Feld tragen Sie den Pfad ein, unter dem die Schnittstellendatei gespeichert werden soll.
- **Export:** Mit der Wahl der Option legen Sie fest, wessen Stammdaten exportiert werden sollen.
  - **Artikel:** Die Stammdaten der Artikel werden exportiert.
  - **Kunden:** Die Stammdaten des Kunden werden exportiert.

# Angebotsoptimierung

**Fertigung > Angebotsoptimierung**

In diesem Bereich können Sie Ihre Angebote probehalber an die Produktion übergeben, um z. B. festzustellen, wie viele Bandmaße für den Zuschnitt benötigt werden. Dies kann bei besonderen Gläsern zur Preisgestaltung berücksichtigt werden.

Die Dialoge sind bereits an anderer Stelle ausführlich beschrieben.
- **Nummernverwalter:** Der Dialog Nummernverwalter ist im Part Verkauf beschreiben. ⇨ Verkauf, "Nummernverwalter" auf Seite C-1917
- **Übergabe Produktion:** Die Funktion dieses Dialogs entspricht der Übergabe von Aufträgen. Im Unterschied zu den Aufträgen sind die übergebenen Angebote jedoch nicht für die Produktion freigegeben. ⇨ "Übergabe Produktion" auf Seite E-2466

# Versandsteuerung

**Fertigung > Versandsteuerung**

In diesem Bereich können Sie den Versand organisieren, der nicht über den eigenen Fuhrpark abgewickelt wird. Sie können für Ihre Spediteure verschiedene Versandpapiere und Ladelisten erstellen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Versand (Spedition)" auf Seite E-2591
- "Versandaufträge löschen" auf Seite E-2598
- "Gestell-Packliste" auf Seite E-2599
- "Teillieferung" auf Seite E-2601
- "Ladelisten" auf Seite E-2603

## Versand (Spedition)

**Fertigung > Versandsteuerung > Versand**

Im Dialog Versand ordnen Sie Aufträge, Gestelle und Lagerorte einander zu.

In diesem Dialog finden Sie folgende Register:
- "Versandsteuerung - Sammeln" auf Seite E-2593
- "Versandsteuerung - Versandinfo" auf Seite E-2595
- "Versandsteuerung - Verpackung + Transport" auf Seite E-2596

### Menü Funktionen

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Versandsteuerung zu schließen.

**Gruppe Versand**
- **Aufträge gruppieren:** Aufträge können zu Gruppen zusammengefasst werden.
- **Versanddatei erstellen:** Speichert die Versandliste als Datei.
- **Auflösen von Versandaufträgen:** Öffnet den Dialog Versandaufträge löschen, in dem Sie Aufträge aus einem Versandauftrag herausnehmen können. ⇨ "Versandaufträge löschen" auf Seite E-2598

**Gruppe Drucken**
Über die Schaltflächen öffnen Sie den Dialog Formular-/Etikettendruck im jeweiligen Druckmodus. Folgende Druckmodi stehen zur Wahl:
- Versandetiketten
- Containerliste
- Ladeliste
- Packliste

Eine ausführliche Beschreibung finden Sie im Part Verkauf.
⇨ Verkauf, "Formular-/Etikettendruck" auf Seite C-1926

### Versandsteuerung – Sammeln

**Fertigung > Versandsteuerung > Versand > Register Sammeln**

*Abb. E-145 Versand – Sammeln*

In diesem Register stellen Sie die Aufträge für eine Ladeliste zusammen. Die Aufträge müssen alle für denselben Kunden ausgestellt sein.

> **i Auftrag aus der Liste entfernen**
> Wenn Sie versehentlich einen (falschen) Auftrag ausgewählt haben, können Sie diesen über Menü Funktionen > Auflösen von Versandaufträgen aus der Liste entfernen.
> ⇨ "Versandaufträge löschen" auf Seite E-2598

#### Selektion nach

Mit der Wahl der Option legen Sie fest, nach welchem Kriterium Sie die Aufträge zusammenstellen wollen. Die gleichnamigen Felder werden freigeschaltet.
- **Ident-/Gestellnummer:** Angabe der Identnummer oder der Nummer des Gestells, auf dem die Auftragspositionen abgestellt sind.
- **Auftragsnummer:** Angabe der Auftragsnummer des fertig gemeldeten Auftrags ein.
- **Lagerort:** Auswahl des Lagerorts, an dem die gefertigten Auftragspositionen abgestellt sind.

#### Ziel

- **Nummernverwalter:** Die gesammelten Aufträge werden automatisch in einen Nummernverwalter kopiert. Wenn Sie einen neuen Namen eintragen, wird der Nummernverwalter angelegt.
- **AV-Bereich:** Wenn Sie mit AV-Bereichen arbeiten, können Sie in diesem Feld den Bereich auswählen, dem die Aufträge zugeordnet sind.

#### Aufträge

In der Übersicht werden alle Aufträge angezeigt, die Sie zusammengestellt haben.
- **Auftrag:** Nummer des Auftrags
- **Pos.:** Nummer der Auftragsposition
- **Menge:** Stückzahl der Position
- **Gewicht:** Gewicht der Position
- **Breite, Höhe:** Breite und Höhe der Scheiben
- **Bezeichnung:** Bezeichnung des Produkts
- **Ident/Gestell:** ID oder Gestellnummer

### Versandsteuerung – Versandinfo

**Fertigung > Versandsteuerung > Versand > Register Versandinfo**

*Abb. E-146 Versand - Versandinfo*

In diesem Register geben Sie die Details zu der Ladeliste an, für die Sie die Aufträge zusammengestellt haben.

#### Versandangaben

- **Ladeliste:** Nummer der Ladeliste.
- **LKW:** Sie können einen LKW aus der Liste wählen.
- **Fahrer:** Sie können einen Fahrer aus der Liste wählen.

#### Versandtext

- **Nummer:** Sie können das Textkennzeichen eingeben oder den gewünschten Text suchen. Den gewählten Text können Sie im Anzeigefeld modifizieren.
Sie können einen Text aus den hinterlegten Texten auswählen oder einen eigenen Text einfügen. Der Text wird auf der Ladeliste gedruckt.

### Versandsteuerung – Verpackung + Transport

**Fertigung > Versandsteuerung > Versand > Register Verpackung + Transport**

*Abb. E-147 Versand - Verpackung + Transport*

In diesem Register können Sie einen Zuschlag für die Verpackung und/oder den Transport hinzufügen.

#### Zuschlag

- **Produkt:** Sie können einen Zuschlag auswählen, der allen oder einzelnen Aufträgen in der Übersicht hinzugefügt wird. Über die Suche werden Ihnen alle Produkte der Produktart Leistungen/Zuschläge zur Auswahl angeboten.
- **Menge:** Angabe, wie oft der gewählte Zuschlag berechnet werden soll.
- **Preis/PE, (ME):** Angabe des Betrags pro Mengeneinheit und Auswahl der Mengeneinheit, auf die sich der Betrag bezieht.
- **[Einfügen]:** Mit dieser Schaltfläche übernehmen Sie den Zuschlag in die markierten Aufträge. Wenn kein Auftrag markiert ist, wird der Zuschlag nicht berechnet.

#### Preisdarstellung

Die Zuschläge können einzeln ausgewiesen werden und/oder der Stückliste hinzugefügt werden.

- **Explizit:** Sie können die Art der Preisdarstellung wählen.
  - ☐ Der Zuschlag wird in die Auftragspositionen mit eingerechnet (implizit).
  - ☑ Der Zuschlag wird als eigene Position ausgewiesen.

#### Einfügemodus

Mit der Wahl der Option legen Sie fest, wo der Zuschlag eingefügt werden soll. Wenn der Zuschlag z. B. für Kantenschutz erhoben wird, ist es sinnvoll, ihn in der Stückliste einzufügen, wenn er für eine Transportversicherung erhoben wird, ist er als eigene Position sinnvoll.
- **In Stückliste:** Der Zuschlag wird in die Stückliste eingefügt. Bei einer impliziten Preisdarstellung wird er in die Komponenten der Stückliste eingerechnet.
- **Als Position:** Der Zuschlag wird im Auftrag als eigene Position eingefügt. Für die Preisdarstellung sollte dann explizit gewählt sein.

#### Versandaufträge

- **[Alle], [Keine]:** Mit diesen Schaltflächen markieren Sie alle Aufträge, für die der Zuschlag gelten soll, oder Sie entfernen die Markierung von allen Aufträgen. Wenn kein Auftrag markiert ist, wird der Zuschlag nicht berechnet.

In der Übersicht sind alle Aufträge dargestellt, die Sie im Register Sammeln eingefügt haben.
- **Versand-Nr:** Auftragsnummer für den Versand
- **Kunde/Ort:** Name und Geschäftssitz des Kunden aus dem Auftrag
- **Gewicht:** Gesamtgewicht aller Positionen
- **Netto Wert:** Gesamtwert des Auftrags

## Versandaufträge löschen

**Fertigung > Versandsteuerung > Versand > Menü Funktionen > Auflösen von Versandaufträgen**

*Abb. E-148 Versandaufträge löschen*

In diesem Dialog können Sie einzelne Aufträge aus der Aufstellung im Dialog Versand löschen.

### Dokument

- **Versand-Nr.:** Angabe der Auftragsnummer, aus dem Sie einen Auftrag löschen wollen. Der Name und der Ort des Kunden werden automatisch angezeigt.

### Zu löschende Dokumente

In der Übersicht sind alle Dokumente aufgeführt, die zu der jeweiligen Versandnummer gehören.
- **Versand-Nr.:** Nummer des Versandauftrags
- **Container:** Nummer des Packmittels
- **Kundenauftrag:** Nummer des Auftrags aus A+W Business
- **Status:** Auftragsstatus

## Gestell-Packliste

**Fertigung > Versandsteuerung > Gestell-Packliste**

### Menü Funktionen

**Fertigung > Versandsteuerung > Gestell-Packliste > Menü Funktionen**

- **Tabelle leeren:** Über dieses Menü löschen Sie alle Einträge aus der Tabellenübersicht.

### Gestell-Packliste (Dialog)

**Fertigung > Versandsteuerung > Gestell-Packliste**

*Abb. E-149 Gestell-Packliste*

In diesem Dialog prüfen Sie sich die Beladung der Gestelle.

#### Selektion

Mit der Wahl der Option legen Sie die Darstellung in der Übersicht fest.
- **Alle nicht gedruckten:** Nur die Gestelle werden angezeigt, die noch nicht ausgedruckt wurden.
- **Gestell:** Die Beladung eines einzelnen Gestells wird angezeigt.

#### Tabelle

In der Übersicht sind die Gestelle je nach der gewählten Einstellung aufgeführt.
- **Gestell:** Gestellnummer.
- **Einheit:** Einheit, wenn Auftragsposition aus mehreren Einheiten besteht.
- **Auftrag:** Auftragsnummer.
- **Pos.:** Nummer der Position im Auftrag.
- **Menge:** Stückzahl der Position.
- **Breite, Höhe:** Breite und Höhe der Position.
- **Produkt:** Produktnummer der Position.
