---
title: "A+W Business Software Reference - Warehouse Management and Capacity Planning"
source: "D-HB-AWBusiness_30.pdf"
tags: ["A+W Business Pro", "Kapazitätsplanung", "Lagerwirtschaft", "ERP", "Software Reference", "Warehouse Management", "Inventory Valuation", "Capacity Planning", "LIFO", "FIFO"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical software reference guide for A+W Business Pro, covering modules for warehouse management (Lagerwirtschaft) and capacity planning (Kapazitätsplanung). It details functionalities like stock ordering, inventory valuation (LIFO/FIFO), and production capacity management."
long_description: "This document is a comprehensive software reference manual for A+W Business Pro, specifically focusing on the Warehouse Management (Lagerwirtschaft) and Capacity Planning (Kapazitätsplanung) modules. The first section on Warehouse Management details processes for stock ordering, including menu functions in the order pool and handling supplier information. It also provides an in-depth guide to inventory valuation, explaining the periodic LIFO and FIFO methods with clear examples and tables. The manual describes the dialogs for setting valuation criteria and reviewing the calculated inventory values. The second major part of the document is a tutorial and reference for the Capacity Planning module. It outlines the fundamental concepts, master data setup (machines, production areas, work shifts, time specifications), and the process of scheduling and monitoring production capacities. It covers how to handle capacity problems, use the control station (Leitstand), and manage production feedback. The guide is structured to help users understand the interplay of various master data components to accurately model and plan their production workflow."
---

# Softwarereferenz

---
## Lagerbestellung

> Lagerwirtschaft > Lagerbestellung

In diesem Dialog können Sie alle vorgeschlagenen Lagerbestellungen prüfen und an den Einkauf übergeben.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menüs im Bestellpool" auf Seite G-2901
- "Lagerbestellung" auf Seite G-2904

### Menüs im Bestellpool

Über die Menüs können Sie automatisch die Datumsfelder aktualisieren lassen und zusätzlich andere Dialoge öffnen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite G-2901
- "Menü Optionen" auf Seite G-2902

### Menü Funktionen

> Lagerwirtschaft > Lagerbestellung > Menü Funktionen

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Bestellübergabe zu schließen. Folgende Einträge werden angezeigt:

- **Lieferant/Liefertermine ändern:**
  Öffnet den Dialog Lieferant und Liefertermine ändern.
  ⇨ "Lieferant und Liefertermin ändern" auf Seite C-1949
- **Markierungsoptionen:**
  Öffnet den Dialog Markierungsoptionen.
  ⇨ "Markierungsoptionen" auf Seite C-1950
- **Lieferantenpreise:**
  Öffnet den Dialog Preisvergleich.
  ⇨ "Preisvergleich" auf Seite C-1951

---
*A+W Business Lagerwirtschaft*
*G-2901*
---

### Menü Optionen

> Lagerwirtschaft > Lagerbestellung > Menü Optionen

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

> **Aktivierte Optionen nach dem Öffnen des Dialogs**
> Bitte beachten Sie, dass geänderte Optionen erst beim nächsten Öffnen des Dialogs wirksam werden.
> Wenn durch eine aktivierte Option eine Prüfung gestartet wurde, kann sich das Öffnen eines Dokuments verzögern. Der Grad der Verzögerung hängt von der Leistungsfähigkeit des Rechners ab.
> Die folgenden Beschreibungen stellen die aktivierte Option dar.

Das Menü ist in folgende Gruppen gegliedert:
- Gruppe Übergabe
- Gruppe Liefertermin
- Gruppe Produktbezeichnung
- Gruppe Sonstige
- Gruppe Erweitert

#### Gruppe Übergabe

- **Auftragsbezogene Übergabe:**
  Die Bestellungen werden pro Auftrag übergeben. Wenn diese Option nicht aktiviert ist, können Sammelbestellungen erzeugt werden.
- **Bestellnummer = Auftragsnummer:**
  Diese Option ist nur freigeschaltet, wenn die Option Auftragsbezogene Übergabe aktiviert ist.
- **Bestellpool pro Mitarbeiter:**
  Pro Mitarbeiter kann ein eigener Bestellpool angelegt werden.

#### Gruppe Liefertermin

- **Lieferterminprüfung:**
  Der Liefertermin wird automatisch geprüft. Ändern Sie einen Liefertermin, der nicht an einem Tourentag liegt, wird eine entsprechende Meldung angezeigt.
- **Lieferantentour berücksichtigen:**
  Wenn die Bestellung auf einen Liefertermin fällt, der nicht an einem Tourentag liegt, wird eine entsprechende Meldung angezeigt. Dazu müssen die Lieferantentouren in den Stammdaten hinterlegt werden.
  ⇨ Stammdaten, "Touren" auf Seite B-995
- **Vorlauftage mit Kombiwarengruppe ermitteln:**
  Wenn in den Kombiwarengruppen Vorlauftage hinterlegt sind, sollen diese zur Berechnung des Liefertermins herangezogen werden.
  ⇨ Stammdaten, "Vorlauftage" auf Seite B-681

---
*G-2902*
*A+W Business Lagerwirtschaft*
---

#### Gruppe Produktbezeichnung

- **Produktbezeichnungen aus Lieferantenkartei:**
  Die Bezeichnung der bestellten Produkte wird aus der Lieferantenkartei übernommen.
- **Produktbezeichnungen aus Basisdaten (interne Best.):**
  Für interne Bestellungen wird die Bezeichnung der bestellten Produkte aus den Produktstammdaten übernommen.

#### Gruppe Sonstige

- **Keine Kostenrückschreibung:**
  Die Kosten werden nicht in die EK-Preise des Auftrags zurückgeschrieben.
- **Maßzuschläge berücksichtigen:**
  Bei der Bestellung sollen die Maßzuschläge mit übergeben werden.
- **Druckkennzeichen für Bearbeitungen immer setzen:**
  In der Bestellung sollen Bearbeitungen immer gedruckt werden. Wenn die Option deaktiviert ist, werden die Druckkennzeichen unverändert aus dem Auftrag in die Bestellung übernommen.
- **Statistikwarengruppe aus dem Auftrag:**
  Die Angabe zur Statistikwarengruppe wird aus dem Auftrag übernommen, wenn für Auftrag und Bestellung unterschiedliche Statistikwarengruppen definiert sind.
- **Geschäftsart aus dem Auftrag:**
  Die Geschäftsart wird aus dem Auftrag übernommen, wenn für Auftrag und Bestellung unterschiedliche Geschäftsarten definiert sind.
- **AV-Bereich aus dem Auftrag:**
  Der AV-Bereich wird aus dem Auftrag übernommen, wenn für Auftrag und Bestellung unterschiedliche AV-Bereiche definiert sind.
- **Fachberater = Erfasser bei Neuanlage:**
  In der Bestellung wird automatisch der Name des Mitarbeiters eingetragen, der sich in A+W Business angemeldet hat.
- **Statusänderung erfragen:**
  Die Abfrage zur Änderung des Status wird angezeigt.
- **Wiederholte Übergabe nur bis Sperrstatus:**
  Bestellungen können mehrfach übergeben werden, allerdings nur, bis der Sperrstatus erreicht ist.

#### Gruppe Erweitert

- **Einstellungen:**
  Öffnet den Dialog Erweiterte Einstellungen, um Angaben zum Druck von Texten und Dateianhängen festzulegen.

---
*A+W Business Lagerwirtschaft*
*G-2903*
---

## Lagerbestellung

> Lagerwirtschaft > Lagerbestellung

*Abb. G-114 Lagerbestellung*
*(Screenshot des Dialogs 'Lagerbestellung' mit den Tabs 'Warenhaus', 'Bestellpool' und Feldern wie 'Gang', 'Regal', 'Fach', 'Lieferant', 'Artikel/Farbe', etc.)*

In diesem Dialog können Sie alle vorgeschlagenen Bestellungen für Artikel sehen, deren Mindestbestand unterschritten wurde. Die Bestellmenge wird nach der Menge berechnet, die im Dialog Lagerverwaltung festgelegt ist.

Mit der Übergabe werden die Bestellungen angelegt und können gedruckt und versendet werden.

⇨ Tutorial, "Lagerbestellung (automatisch)" auf Seite G-2782
⇨ Tutorial, "Bestellmenge nach Bestandsprüfung" auf Seite G-2810

### Lagerort

**Warenhaus, Gang, Regal, Fach:** Sie können die Anzeige auf einzelne Lagerorte einschränken. Bedenken Sie dabei, dass auch auf den Lagerort <k.A.> Lagerartikel gebucht sein können. Wenn Sie die Auswahl nicht einschränken, werden Bestellvorschläge zu allen Artikeln angezeigt, deren Mindestbestand unterschritten ist.
Die Bezeichnung der Lagerorte kann in den Stammdaten geändert werden.
⇨ Tutorial, "Lagerebenen festlegen" auf Seite G-2697

---
*G-2904*
*A+W Business Lagerwirtschaft*
---

### Übersicht

In der Übersicht werden die Daten zu den Bestellvorschlägen angezeigt. Sie können einen anderen Lieferanten auswählen und sich einen Preisvergleich anzeigen lassen.

- **Lieferant:**
  Der Lieferant wird aus der Lieferantenkartei übernommen. Wenn kein Lieferant eingetragen ist oder wenn Ihnen Lieferschwierigkeiten Ihres Standard-Lieferanten bekannt sind, können Sie den Namen ändern.
- **Artikel/Farbe:**
  Nummer und ggf. Variante des Produkts, das bestellt werden soll.
- **Ident-Nr.:**
  Kisten-ID (manuelle Buchung oder aus dem Wareneingang)
- **Lagerort:**
  Lagerort, an dem der Bestand des Lagerartikels unterschritten ist.
- **Menge:**
  Menge, die bestellt werden soll. Die Standard-Bestellmenge wird so oft multipliziert, bis der Mindestbestand überschritten ist. Sie können den Wert direkt in der Übersicht überschreiben.
- **Breite, Höhe:**
  Maße der Scheibe, die bestellt werden soll.
- **Inhalt:**
  Der Inhalt wird nur bei Kisten angezeigt.
- **Anlief.-Lief.:**
  Der Liefertermin des Lieferanten wird aus den Angaben in der Lieferantenkartei errechnet. Wenn Ihnen Lieferschwierigkeiten Ihres Standard-Lieferanten bekannt sind, können Sie den Termin ändern.
  ⇨ Verkauf, "Lieferant und Liefertermin ändern" auf Seite C-1949
  ⇨ Verkauf, "Preisvergleich" auf Seite C-1951

**Position für:** Die Bestellvorschläge sind in unterschiedlichen Farben dargestellt:
- **Rot: interner Auftrag:**
  Interne Aufträge sind Produktionsaufträge, die erzeugt werden, um den Lagerbestand aufzufüllen. Der Vorschlag wird automatisch erzeugt, wenn in der Lieferantenkartei für das Produkt die entsprechende Option aktiviert ist.
- **Blau: Anfrage:**
  Bestellanfragen an einen Lieferanten, um z. B. Preise und Liefertermine zu erfragen.
- **Grün: Liefertermin für Auftr./Best. gefährdet:**
  Als Liefertermin wird automatisch das aktuelle Tagesdatum eingesetzt. Damit ist die Lieferung i. d. R. nicht termingerecht möglich. Wenn Sie das Datum ändern, wechselt die Schriftfarbe für den Eintrag zu Schwarz.

---
*A+W Business Lagerwirtschaft*
*G-2905*
---

### Ziel-Nummernverwalter

**Mitarbeiter:** Name des Mitarbeiters, der sich in A+W Business angemeldet hat oder der den Nummernverwalter eingerichtet hat. Wenn Sie einen neuen Nummernverwalter anlegen, können Sie diesen einem bestimmten Mitarbeiter zuweisen.

**Name:** Name des Nummernverwalters, in den die Bestellungen übergeben werden sollen. Wenn Sie einen neuen Namen eintragen, wird ein neuer Nummernverwalter angelegt.

### Ziel-Nummernkreis

**Mandant:** Wenn Sie für Ihre Mandanten gesonderte Nummernkreise eingerichtet haben, können Sie den gewünschten Mandanten auswählen.

**AV-Bereich:** Wenn Sie mit AV-Bereichen arbeiten, können Sie die Bestellung einem bestimmten AV-Bereich zuordnen.

---
*G-2906*
*A+W Business Lagerwirtschaft*
---

## Lagerbewertung

Bei der Lagerbewertung werden die Lagerbestände nach dem periodischen Verfahren bewertet. Dazu werden die Lagerabgänge der gesamten Periode zunächst summiert. Anschließend werden die Lagerabgänge von den Wareneingängen abgezogen. Dieser Vorgang hängt vom gewählten Verfahren ab:

- **LIFO:** Die zuletzt eingegangenen Artikel werden zuerst abgezogen.
- **FIFO:** Die zuerst eingegangenen Artikel werden zuerst abgezogen.

Der Lagerwert wird jeweils aus der nicht verbrauchten Menge berechnet. Dabei wird der Zeitraum von der letzten Lagerbewertung bis zum Auswertungszeitpunkt berücksichtigt.

### Beispiel

**Tabelle: Nach LIFO**
| Lager | Artikel | Datum | Wert in € | Menge (Nach LIFO) | Wert |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 111 | 1.5.2016 | 8,50 | 15 (15) | 15*8,50 |
| 1 | 111 | 4.5.2016 | 8,70 | 20 (10) | 15*8,50 + 20*8,70 |
| 1 | 111 | 5.5.2016 | 8,20 | 10 (0) | 15*8,50 + 20*8,70 + 10*8,20 |
*Der LIFO Wert beträgt (15*8,50+10*8,70) / 25 = 8,58*

**Tabelle: Nach FIFO**
| Lager | Artikel | Datum | Wert in € | Menge (Nach FIFO) | Wert |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 111 | 1.5.2016 | 8,50 | 15 (15) | 15*8,50 |
| 1 | 111 | 4.5.2016 | 8,70 | 20 (10) | 15*8,50 + 20*8,70 |
| 1 | 111 | 5.5.2016 | 8,20 | 10 (0) | 15*8,50 + 20*8,70 + 10*8,20 |
*Der FIFO Wert beträgt (15*8,70+10*8,20) / 25 = 8,50*

*Tab. G-1 Berechnungsbeispiele*

> **Lagerartikel mit ID**
> Lagerartikel mit Identnummern können nicht nach FIFO/LIFO bewertet werden, da diese eindeutig identifizierbar sind. Von diesen Lagerartikeln ist entweder 1 oder kein Stück vorhanden. Daher gibt es keine Entnahmereihenfolge.
>
> Bei der Erstbewertung darf der Lagerbestand nicht negativ sein. Die Erstbewertung kann nur nach durchschnittlichem EK oder manuellem Wert erfolgen. Ab dem Zeitpunkt der Erstbewertung kann dann mit dem FIFO oder LIFO Verfahren gerechnet werden.

---
*A+W Business Lagerwirtschaft*
*G-2907*
---

## Lagerbewertung

> Lagerwirtschaft > Lagerbewertung > Selektion

In diesem Dialog starten Sie die Berechnung des Lagerwerts.
Im Dialog Lagerbewertung finden Sie folgende Register:
- Lagerbewertung – Selektion
- Lagerbewertung - Bewertung

### Menü Optionen

> Lagerwirtschaft > Lagerbewertung

Folgende Einträge werden angezeigt:
- **Erstbewertung nach:**
  Für die Erstbewertung des Lagerbestands können Sie eines der folgenden Verfahren auswählen:
  - FIFO, LIFO
  - Durch. EK
  - Manuell

---
*G-2908*
*A+W Business Lagerwirtschaft*
---

### Lagerbewertung – Selektion

> Lagerwirtschaft > Lagerbewertung > Selektion

*Abb. G-115 Lagerbewertung – Selektion*
*(Screenshot des Dialogs 'Lagerbewertung zum 09.12.2016' mit den Tabs 'Selektion' und 'Bewertung'. Der Tab 'Selektion' ist aktiv und zeigt Auswahlkriterien wie 'Nicht bewertet seit', 'Produkt', 'Produktart', etc.)*

In diesem Register stellen Sie die Kriterien ein, nach denen der Lagerwert berechnet werden soll. Zusätzlich können Sie in den Firmendaten festlegen, wie der EK berechnet werden soll.
⇨ "Inventurliste" auf Seite G-2844

#### Auswahl

- **Nicht bewertet seit:** Angabe des letzten Bewertungsdatums. Sie können ein beliebiges Datum in der Vergangenheit wählen. Damit werden nur die Produkte bewertet, deren letzte Bewertung vor diesem Datum liegt. Der Bewertungszeitraum liegt zwischen diesem Datum und dem Datum, das Sie im Feld Bewertung eintragen.
- **Produkt von ... bis:** Auswahl der Produkte, die bewertet werden sollen.
- **Produktart:** Auswahl der Produktart, deren Produkte bewertet werden sollen.
- **Stat. Warengruppe:** Auswahl der Statistik-Warengruppe, die dem Produkt zugewiesen ist.
- **Warenhaus, Gang, Regal, Fach:** Auswahl des Lagerorts, dessen Produkte bewertet werden sollen.

---
*A+W Business Lagerwirtschaft*
*G-2909*
---

- **Nur gültige Bestände (Bestand nicht negativ):** Sie können Produkte von der Bewertung ausschließen, deren Bestand aufgrund von Reservierungen negativ ist.
  - Alle Produkte werden bewertet, die den Auswahlkriterien in den Feldern Produkt und Produktart entsprechen.
  - Nur die Produkte werden bewertet, deren Bestand nicht negativ ist. Darin sind auch Produkte enthalten, deren Bestand = 0 ist.

- **Kein Glas mit Abmessungen (0x0):** Für die kombinierte Lagerführung werden Produkte mit den Abmessungen 0x0 angelegt, auf die reservierte Mengen bis zum Abbuchen der verbrauchten Lagerplatten gebucht werden.
  - Alle Produkte werden bewertet, die den Auswahlkriterien in den Feldern Produkt und Produktart entsprechen.
  - Produkte mit den Abmessungen 0x0 werden nicht bewertet.

- **Bewertung:** Angabe des Datums, zu dem die Lagerwertung berechnet werden soll. Damit können Sie eine Lagerbewertung in der Vergangenheit durchzuführen. Die Lagerbestände werden zu diesem Datum berechnet.

---
*G-2910*
*A+W Business Lagerwirtschaft*
---

### Lagerbewertung – Bewertung

> Lagerwirtschaft > Lagerbewertung > Bewertung

*Abb. G-116 Lagerbewertung – Bewertung*
*(Screenshot des Dialogs 'Lagerbewertung zum 09.12.2016', Tab 'Bewertung' ist aktiv. Eine Tabelle zeigt Produkte mit Details wie Bezeichnung, Maße, Lagerort, Lagerbestand und Bewertungsdaten nach FIFO/LIFO.)*

In diesem Register werden zunächst die Artikel angezeigt, die den Auswahlkriterien entsprechen. Wenn Sie die Bewertung über eine der Schaltflächen gestartet haben, werden die berechneten Werte angezeigt.

Diese Werte werden auch in der Lagerstatistik angezeigt:
⇨ "Lagerstatistik – FIFO/LIFO" auf Seite G-2894

Die Werte können gespeichert werden. Vor dem Speichern werden alle eingestellten Bewertungen nochmal auf ihre Konsistenz geprüft. Wenn hierbei ein Fehler festgestellt wird, wird dieser angezeigt und keiner der Sätze gespeichert. Sie müssen den Fehler bereinigen, um anschließend die Datensätze speichern zu können.

Wenn Sie die Daten gespeichert haben, können Sie die Bewertung nicht mehr ändern.

#### Bewertung

- **Alle selektieren:** Sie können aus der Liste einzelne Produkte auswählen. Mit der Mehrfachauswahl können Sie beliebig viele Produkte markieren. Über die Schaltflächen können Sie alle Produkte auswählen oder die Auswahl vollständig aufheben.
- **[LIFO berechnen]:** startet die Bewertung der markierten Produkte nach dem LIFO-Verfahren.

---
*A+W Business Lagerwirtschaft*
*G-2911*
---

- **[FIFO berechnen]:** startet die Bewertung der markierten Produkte nach dem FIFO-Verfahren.
- **[Beide berechnen]:** startet die Bewertung der markierten Produkte nach den beiden Verfahren.
- **Bewertungsart ändern:** Auswahl der Bewertungsart. Die Änderung der Bewertungsart wirkt sich nur auf die markierten Einträge aus.

#### Übersicht

Folgende Spalten können angezeigt werden:
- **Produkt, Bezeichnung:** Nummer und Bezeichnung des Produkts.
- **Breite, Höhe:** Maße der Scheibe.
- **Inhalt:** Inhalt eine Kiste.
- **Farbe:** Farbvariante des Glases.
- **Lagerort:** Vollständiger Lagerort.
- **PE:** Preiseinheit des Produkts.
- **Lagerbestand:** Aktueller Lagerbestand ohne Reservierungen.
- **ME:** Mengeneinheit, in der das Produkt im Lager geführt wird.
- **Bewertung:** Art der Bewertung:
  - **Keine:** Der Bestand dieses Produkts wurde nicht berechnet.
  - **LIFO, FIFO:** Der Lagerwert ist als LIFO-, FIFO-Wert berechnet.
  - **Durch. EK:** Der Lagerwert ist ein durchschnittlicher EK-Wert.
  - **Manuell:** Der Lagerwert ist manuell eingetragen.
- **FIFO, LIFO:** Berechneter Lagerwert des Produkts.
- **Durch. EK:** Durchschnittlicher Einkaufspreis. Dieser Preis wird nur berechnet, wenn in den Firmendaten die entsprechende Option aktiviert ist.
- **Manuell:** Der Wert der manuellen Eingabe wird als Lagerwert eingetragen.

---
*G-2912*
*A+W Business Lagerwirtschaft*
---

- **Bemerkung FIFO/LIFO:** Anzeige des Status nach der Bewertung:
  - **OK:** Der Bestand dieses Produkts wurde berechnet. Dieser Status ist bei der Erstbewertung nicht möglich.
  - **Bestand ist negativ!:** Der Bestand dieses Produkts kann nicht berechnet werden, weil der Bestand negative Werte enthält.
  - **Es wurde kein Anfangssatz gefunden:** Der Bestand dieses Produkts kann nur nach durchschnittlichen EK oder manuell bewertet werden.
  - **Menge muss größer 0 sein:** Der Bestand dieses Produkts kann nicht berechnet werden, weil kein Bestand vorhanden ist.
- **Letzte Bewertung:** Datum der letzten Lagerbewertung.
- **Bewertung:** Wert der letzten Bewertung.

---
*A+W Business Lagerwirtschaft*
*G-2913*
---
*G-2914*
*A+W Business Lagerwirtschaft*
---

# A+W Business Pro Kapazitätsplanung

---
*A+W Software for Glass, Windows & Doors*
---

## Revisionsübersicht des Moduls:

| Datum | Änderungen |
| :--- | :--- |
| 08-2017 | Strukturelle Überarbeitung. Dialoge Aggregate, Positionssplit, Vorgabezeiten aktualisiert. |
| 01-2017 | Produkt- und Firmennamen angepasst. |
| 02-2015 | Anpassung an A+W Business Pro. Rechtschreibkorrekturen |
| 04-2014 | Vollständige Überarbeitung. |
| 08-2013 | Anpassung der ALFAK-Dokumentation auf A+W Business. |
| 05-2012 | Ersterstellung des Tutorials; Softwarereferenz vollständig überarbeitet |
| 09-2010 | Layout an Doku-Konzept 2010 angepasst |
| 08-2008 | Rechtschreibkorrekturen, grafische Tabellen umgewandelt, Abbildungen und Part-Nummerierung angepasst |
| 12-2003 | Ersterstellung |

Zu diesem Modul finden Sie folgende Kapitel:
⇨ Tutorial
⇨ Softwarereferenz

---
*H-2916*
*A+W Business Pro Kapazitätsplanung*
---

# A+W Business Pro Kapazitätsplanung - Tutorial

---
*A+W Software for Glass, Windows & Doors*
---

## In diesem Kapitel finden Sie folgende Themen:

⇨ Überblick
⇨ Stammdaten
⇨ Kapazitätsplanung

### Inhaltsverzeichnis

- **Überblick** ... H-2920
- **Aufbau des Tutorials** ... H-2920
- **Menü-Übersicht** ... H-2922
  - Modul Kapazitätsplanung ... H-2922
  - Modul Fertigung ... H-2924
- **Grundgedanken der Kapazitätsplanung** ... H-2926
- **Nutzung der Kapazitätsplanung** ... H-2927
- **Stammdaten** ... H-2928
- **Maschinen und Produktionsbereiche** ... H-2930
  - Aggregattypen und Aggregate ... H-2932
  - Arbeitsarten ... H-2936
  - Produktionsbereiche (Arbeitszentren) ... H-2938
  - Produktionsbereich anlegen ... H-2939
  - Aggregat anlegen ... H-2940
  - Übungen ... H-2944
- **Schicht- und Arbeitszeiten** ... H-2945
  - Arbeitszeiten ... H-2946
  - Arbeitstage und Schichten ... H-2946
  - Maximale Kapazität pro Tag ... H-2948
  - Arbeitseinheiten ... H-2950
  - Voreinstellungen für Schichten und Kapazitäten ... H-2955
  - Kalender anpassen ... H-2957
  - Übungen ... H-2963
- **Zeitvorgaben** ... H-2964
  - Basiskomponenten der Zeitplanung ... H-2965
  - Vorgabezeiten ... H-2967
  - Sonderzeiten ... H-2970
  - Arbeitsarten und Zeitzuschläge ... H-2971
  - Fallbeispiel ISO und Modell ... H-2972
  - Berechnungsreihenfolge für Zuschläge und Faktoren ... H-2976
  - Übergangsmatrix und Übergangszeiten ... H-2977
  - Rüstzeiten ... H-2983
  - Zeitfaktoren für Serien ... H-2984
  - Vorgabezeiten festlegen ... H-2985
  - Sonderzeit anlegen ... H-2989
  - Übungen ... H-2994
- **Auswahl der Aggregate** ... H-2995
  - Prioritäten ... H-2996
  - Restriktionen ... H-2997
  - Priorität vs. Restriktion ... H-2998
  - Automatische Einlastung ... H-3000
  - Maschinenauswahl bei Ausweicharbeitsart ... H-3004
  - Sperren ... H-3005
  - Fertigungsstraße definieren ... H-3008
  - Voreinstellungen zur Aggregatauswahl ... H-3010
- **Zuordnen der A+W Business Pro-Stammdaten** ... H-3012
  - Produktionsreihenfolge ... H-3013
  - Kombi-Produktart, Kombi-Produktgruppe ... H-3017
  - Zuordnung festlegen ... H-3018
  - Übungen ... H-3021
- **Kapazitätsplanung** ... H-3022
  - Einlastung der Aufträge ... H-3023
  - Terminberechnung ... H-3024
  - Einlastung ... H-3028
  - Kapazitätsprobleme ... H-3029
  - Voreinstellungen für automatische Einlastung ... H-3033
  - Auftrag einlasten ... H-3034
  - Kapazitätsproblem lösen ... H-3040
  - Übungen ... H-3046
- **Produktion** ... H-3047
  - Rückmeldungen zum Produktionsstand ... H-3048
  - Erfassungsstellen ... H-3050
  - Statusmeldungen ... H-3052
  - Fertigmeldung ... H-3054
  - Restmengen vom Vortag ... H-3055
  - Bruchrückmeldung ... H-3056
  - Produktionspapiere drucken ... H-3057
  - Auftrag manuell fertig melden ... H-3059
  - Bruchmeldung manuell erfassen ... H-3062
  - Fertigungsstand prüfen ... H-3064
  - Fertigmeldungen nachholen ... H-3066
  - Übungen ... H-3068
- **Produktionskosten** ... H-3069
  - Zeitkosten ... H-3070
  - Kostenstellen ... H-3072
  - Kostenkalkulation im Auftrag ... H-3075
  - Kostenkalkulation für Angebote ... H-3075
  - Übungen ... H-3076
- **Leitstand** ... H-3077
  - Konzept des Leitstands ... H-3078
  - Leitstand - Auftrag ... H-3080
  - Leitstand - Aggregat ... H-3081
  - Einlastung für einzelnen Auftrag verschieben ... H-3082
  - Aggregat ändern ... H-3087
  - Übungen ... H-3089

---
*H-2918 & H-2919*
*A+W Business Pro Kapazitätsplanung*
---

## Überblick

Das Tutorial zum Modul Kapazitätsplanung beschäftigt sich mit den Grundlagen der Planung von Produktionskapazitäten in A+W Business Pro. Das Tutorial baut auf den Kenntnissen zu den Stammdaten und zu Dokumenten auf.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

### Themenblöcke

In diesem Tutorial finden Sie folgende Themenblöcke:
- Stammdaten
- Kapazitätsplanung

### Vorausgesetzte Kenntnisse

Das Tutorial richtet sich an Teilnehmer, die in A+W Business die Kapazitäten planen und damit die Auslastung der Maschinen überwachen. Die Teilnehmer müssen das Konzept der Stammdaten in A+W Business und das Modul Dokumente kennen. Kenntnisse der Module Fertigung und Lagerwirtschaft sind von Vorteil.

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
  Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen und Lösungsvorschlägen.

- **Querverweise**
  Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf ergänzende Informationen in der Softwarereferenz und in anderen Parts hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.

### Lesehinweis

Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.
Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

---
*H-2920 & H-2921*
*A+W Business Pro Kapazitätsplanung*
---

## Menü-Übersicht

Die Kapazitätsplanung in A+W Business Pro gliedert sich in zwei Bereiche: das Einrichten der Kapazitätsplanung und die Planung und Überwachung der Kapazitäten. Die zugehörigen Dialoge finden Sie in den Modulen Kapazitätsplanung und Fertigung. Diese beiden Module werden im Folgenden kurz vorgestellt.

### Modul Kapazitätsplanung

Im Modul Kapazitätsplanung richten Sie die Stammdaten und weitere Vorgaben für die Planung der Kapazitäten ein.

*Abb. H-1 Modul Kapazitätsplanung*
*(Screenshot des Moduls Kapazitätsplanung mit den Menüpunkten Stammdaten, Allgemein, Organisation, Vorgabezeiten, Zuordnen, Sperren, Übersicht etc.)*

#### Stammdaten

Das Menü Stammdaten ist in drei Untermenüs gegliedert:

- **Allgemein:**
  In diesem Bereich richten Sie die allgemeinen Daten ein, z. B. Aggregat-Typen (Maschinentypen), Arbeitsarten, Übergangzeiten.
  ⇨ Softwarereferenz, "Allgemein" auf Seite H-3104
- **Organisation:**
  In diesem Bereich richten Sie die Stammdaten zur betrieblichen Organisation ein, z. B. Produktionsbereiche, Maschinen, Kalender und Restriktionen.
  ⇨ Softwarereferenz, "Organisation" auf Seite H-3114
- **Vorgabezeiten:**
  In diesem Bereich richten Sie die Daten zur Berechnung von Produktionszeiten ein, z. B. Vorgabezeiten und Sonderzeiten.
  ⇨ Softwarereferenz, "Vorgabezeiten" auf Seite H-3140

#### Zuordnen

Hier ordnen Sie den Arbeitsarten z. B. die Produkte oder Warengruppen (WGR) zu. Zu einigen Arbeitsarten legen Sie einen Faktor für die Berechnung der Zeiten fest, wenn ein besonderer Aufwand dies erforderlich macht, z. B. bei der Fertigung von Modellen.
⇨ Softwarereferenz, "Zuordnen" auf Seite H-3153

#### Sperren

Hier legen Sie fest, welche Maschinen nicht eingesetzt werden dürfen, wenn z. B. bestimmte Produkte oder Warengruppen in einem Auftrag erfasst sind.
⇨ Softwarereferenz, "Sperren" auf Seite H-3173

#### Übersicht

Hier können Sie sich Übersichten über die Auslastung der Maschinen und Produktionsbereiche erstellen lassen.
⇨ Softwarereferenz, "Übersichten" auf Seite H-3184

---
*H-2922 & H-2923*
*A+W Business Pro Kapazitätsplanung*
---

### Modul Fertigung

Im Modul Fertigung lasten Sie die Aufträge in die Kapazitätsplanung ein und überwachen die Rückmeldungen aus der Produktion.
In diesem Modul finden Sie auch die Programmbereiche, in denen Sie die Aufträge an die Produktion übergeben. Diese werden im Part Fertigung beschrieben.

*Abb. H-2 Menü Kapazitätsplanung*
*(Screenshot des Moduls Fertigung mit einer tabellarischen Übersicht der Auslastung von Aggregaten wie Zuschnitt/Cutting, CNC, ESG Ofen über verschiedene Tage.)*

#### Einlasten

Im Menü Einlasten finden Sie folgende Dialoge:
- **Nummernverwalter:**
  Im Nummernverwalter sammeln Sie die Aufträge für die manuelle Einlastung.
- **Einlasten NV:**
  Über diesen Dialog lasten Sie die Aufträge ein.
- **Einlasten Auftrag:**
  Über diesen Dialog lasten Sie einen einzelnen Auftrag ein.
- **Aggregate Ausfall:**
  In diesem Dialog sperren Sie ein Aggregat für die Einlastung.
  ⇨ Softwarereferenz, "Einlastung" auf Seite H-3197

#### Fertigmeldung

Im Menü Fertigmeldung finden Sie folgende Dialoge:
- **Datum:**
  In diesem Dialog melden Sie die Aufträge an einem Aggregat fertig.
- **Lauf:**
  In diesem Dialog melden Sie Aufträge pro Lauf fertig.
- **Manuell:**
  In diesem Dialog melden Sie Aufträge komplett oder in Teilen fertig.
  ⇨ Softwarereferenz, "Produktionsmeldungen" auf Seite H-3222

#### Produktionslisten

Hier erstellen Sie pro Maschine Listen über die Stückzahlen, die gefertigt werden müssen.
⇨ Softwarereferenz, "Produktionsmeldungen" auf Seite H-3222

#### Fertigungsstand Auftrag

Hier können Sie den aktuellen Stand der Fertigung pro Auftrag prüfen und ggf. ausgelassene Fertigmeldungen nachholen.
⇨ Softwarereferenz, "Fertigungsstand Auftrag" auf Seite H-3240

#### Leitstand

Hier prüfen Sie die Auslastung der Maschinen und schichten ggf. Aufträge um, indem Sie zugewiesene Aggregate, Schichten, Produktions- oder Liefertermine ändern.
⇨ Softwarereferenz, "Leitstand" auf Seite H-3260

> **A+W Business Pro Capacity Planning vs. A+W Production Capacity Planning**
> In dieser Anleitung ist immer die Kapazitätsplanung in A+W Business Pro gemeint. Capacity Planning meint die Kapazitätsplanung von A+W Production.

---
*H-2924 & H-2925*
*A+W Business Pro Kapazitätsplanung*
---

### Grundgedanken der Kapazitätsplanung

Mit der Kapazitätsplanung können Sie die Auslastung Ihrer Produktionskapazitäten vorplanen und Produktions- und Zeitkosten ermitteln. Die Planungsdaten helfen Ihnen, Kapazitätsengpässe frühzeitig zu erkennen. Sie können dann in die Planung eingreifen und manuell korrigieren.

Dazu müssen Sie die Stammdaten der Kapazitätsplanung anlegen und so aufeinander abstimmen, dass die Abläufe in Ihrer Produktion abgebildet werden. Die nachfolgende Abbildung zeigt wie diese Stammdaten zusammenwirken am Beispiel der Vorgaben, aus denen die Termine für den Produktionsbeginn errechnet werden.

*Abb. H-3 Zusammenwirken der Stammdaten der Kapazitätsplanung*
*(Diagramm, das zeigt, wie Stammdaten der Kapazitätsplanung (Aggregattypen, Produktionsbereiche, Aggregate, Arbeitsarten, Kalender, Vorgabezeiten) mit A+W Business Pro-Produktstammdaten zusammenwirken, um den Termin für den Produktionsbeginn zu berechnen.)*

In dieser Übersicht sehen Sie, wie z. B. Aggregate (Maschinen) bei der Planung der Kapazitäten eingesetzt werden:
- Für die einzelnen Arbeitsarten sind pro Aggregat Vorgabezeiten hinterlegt, aus denen die (freie) Kapazität und die benötigte Zeit für eine Auftragsposition berechnet werden.
- Pro Aggregat ist festlegt, an welchen Tagen es wie lange verplant werden kann (Schichtzeiten im Kalender).
- Aus den Zeiten, die eine Position in einem Produktionsbereich verweilt (Übergangsmatrix, Übergangzeiten), den Schichtzeiten (Kalender) und Vorgabezeiten wird der Termin für die Fertigung einer Auftragsposition berechnet.

Wenn die Stammdaten der Kapazitätsplanung erfasst sind, können die Aufträge in die Kapazitätsplanung eingelastet werden. Alle Auftragspositionen und deren Stücklisten-Komponenten werden den entsprechenden Arbeitsarten zugeordnet. Danach werden die benötigten Maschinenzeiten und die Kosten berechnet. Gleichzeitig wird der Liefertermin geprüft und der Termin zum Beginn der Produktion berechnet. Während und/oder nach der Einlastung können Sie in die Planung eingreifen und Arbeitsgänge einer Auftragsposition manuell auf andere gleichartige Maschinen umbuchen.

Die aktuelle Planung überwachen Sie im Dialog Leitstand. Von diesem Dialog aus können Sie in die Planung eingreifen und sich verschiedenen Übersichten und Grafiken zur Auslastung anzeigen lassen.

Bei Anbindung an die Produktionssoftware A+W Production werden die Ergebnisse der Kapazitätsplanung (Grobplanung) an A+W Production übergeben. Von A+W Production werden wiederum Rückmeldungen an A+W Business Pro übergeben, wenn Aufträge bzw. Positionen in der Produktion fertig gemeldet wurden. Dies führt in A+W Business Pro u. a. zur Erhöhung des Auftrags- bzw. Positionsstatus. Die Daten über Maschinenkosten und -zeiten werden nach der Fertigstellung des Auftrags aktualisiert.

> **Zeit- und Kostenermittlung**
> Aus den Vorgaben der Kapazitätsplanung werden die Zeit- und Maschinenkosten errechnet. Mit dieser Grobplanung wird auch geprüft, ob die Aufträge termingerecht versandfertig werden. Die Kapazitätsplanung in A+W Business Pro hat keinen Einfluss darauf, an welchen realen Maschinen im Produktionsprozess die Aufträge tatsächlich gefertigt werden.

### Nutzung der Kapazitätsplanung

Sie können mit der Kapazitätsplanung die Produktionskapazitäten aufgrund der Auftrags-, Maschinen- und Zeitdaten in A+W Business Pro planen. Dazu ist keine Anbindung an A+W Production erforderlich.

Folgende Hauptmerkmale charakterisieren die Kapazitätsplanung von A+W Business Pro:
- Flexibles Anlegen der Stammdaten für die Kapazitätsplanung
- Ermittlung von Kapazitätsengpässen
- Prüfung des Liefertermins
- Kalkulation der Produktionskosten
- Leitstand mit Übersichten und Funktionen zum Umlasten
- Bei Anbindung an die Produktions-Software A+W Production:
  - Übergabe der Plandaten an A+W Production
  - Rückmeldung der Ist-Daten an A+W Business Pro
  - Vergleich von Soll- und Ist-Werten

> **Begriffsklärung**
> In A+W Business Pro und in dieser Dokumentation werden die Begriffe Kapazitätsplanung und Zeitwirtschaft synonym verwendet.

---
*H-2926 & H-2927*
*A+W Business Pro Kapazitätsplanung*
---

## Stammdaten

Die Kapazitätsplanung kann mit Hilfe der Stammdaten an unterschiedliche Unternehmensstrukturen und Produktionsprozesse angepasst werden.
In diesem Themenblock lernen Sie, wie die Stammdaten der Kapazitätsplanung zusammenwirken und wie Sie diese Daten anlegen und pflegen.

Dazu gehören folgende Lerneinheiten:
- "Maschinen und Produktionsbereiche" auf Seite H-2930
- "Schicht- und Arbeitszeiten" auf Seite H-2945
- "Zeitvorgaben" auf Seite H-2964
- "Auswahl der Aggregate" auf Seite H-2995
- "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-3012

### Rechteverwaltung
Fast alle Zugriffe auf die Stammdatendialoge der Kapazitätsplanung können über die Rechteverwaltung eingeschränkt werden. Damit kann die Kapazitätsplanung noch besser an die Abläufe in Ihrem Unternehmen angepasst werden. Das bedeutet aber auch, dass Sie die vollen Zugriffsrechte benötigen, wenn Sie die Übungen in diesem Tutorial nachvollziehen möchten.

### Historie
Jede Änderung des Auftragsstatus pro Produktionsbereich wird automatisch in der Auftrags-Historie dokumentiert. Damit können die Mitarbeiter, die nur Zugriffsrechte auf die Dokumente haben, immer erkennen, wann und welche Statusänderung im Auftragskopf durch die Kapazitätsplanung und die Rückmeldungen aus der Produktion verursacht wurde.

> **Stammdaten der Kapazitätsplanung**
> Die Stammdaten für Maschinen und Produktionsbereiche legen Sie im Modul Kapazitätsplanung an. Diese Stammdaten können nicht über die Dialoge im Modul Stammdaten angelegt werden.
> Wenn Sie die Einstellungen in den Stammdaten der Kapazitätsplanung geändert haben, müssen Sie A+W Business Pro neu starten, damit die Daten neu eingelesen werden.

### Reihenfolge zur Erfassung der Stammdaten

Beim Anlegen der maschinenbezogenen Stammdaten ist es sinnvoll, diese Reihenfolge einzuhalten:

1.  **Aggregattypen**, z. B. Schneidtische, ESG-Öfen, Versand usw.:
    Art und Umfang technischer Restriktionen von Maschinen werden u. a. über die Zuweisung zu Aggregattypen definiert.
    ⇨ "Aggregattypen und Aggregate" auf Seite H-2932
2.  **Produktionsbereiche (Arbeitszentren)**
    Produktion und Versand werden in Bereiche unterteilt, z. B. Zuschnitt, Kantenbearbeitung, Bohren, Kontrolle, Verpacken, usw.
    ⇨ "Produktionsbereiche (Arbeitszentren)" auf Seite H-2938
3.  **Arbeitseinheiten:**
    Zu jedem einzelnen Aggregat wird festgelegt, wie viele Arbeitseinheiten die Berechnungsgrundlage der Kapazität bilden.
    ⇨ "Arbeitseinheiten" auf Seite H-2950
4.  **Aggregate**, z. B. Bystronic-Schneidtisch, Lisec-Schneidtisch, ESG-Ofen A, ESG-Ofen B usw.:
    Nachdem Sie die Produktionsbereiche und Aggregattypen angelegt haben, erfassen Sie die einzelnen Maschinen und ordnen Sie den Produktionsbereichen und Aggregattypen zu.
    ⇨ "Aggregat anlegen" auf Seite H-2940
5.  **Arbeitsarten (Vorgänge):**
    Alle Arbeiten, für die Zeiten berechnet werden, müssen als Arbeitsart definiert werden, z. B. Schneiden, Schleifen, Bohren, Verpacken usw.
    ⇨ "Arbeitsarten" auf Seite H-2936
6.  **Vorgabezeiten:**
    Die Zeiten für Arbeitsarten sind von den jeweiligen Maschinen abhängig. Die Zeiten der Arbeitsart Bohren sind z. B. von der Glasstärke und der Maschine abhängig, mit der gebohrt wird. Pro Maschine und Arbeitsart müssen daher Zeiten gemessen und erfasst werden. Über diese Vorgabezeiten werden den Arbeitsarten die Maschinen zugeordnet.
    ⇨ "Vorgabezeiten" auf Seite H-2967
7.  **Zeitzuschläge:**
    Zusätzlich zu den Vorgabezeiten können Zeitzuschläge definiert werden, die auf den Basiswert aufgeschlagen werden, z. B. für den Zuschnitt von Modellen.

---
*H-2928 & H-2929*
*A+W Business Pro Kapazitätsplanung*
---

### Maschinen und Produktionsbereiche

**Lernziele**
- Zusammenhang von Aggregat-Typen und Aggregaten (Maschinen) kennenlernen.
- Produktionsbereiche anlegen.
- Arbeitsarten definieren und anlegen.

**Nutzen**
- Mit den Stammdaten der Kapazitätsplanung bilden Sie die Abläufe in Ihrer Produktion ab. Damit beziehen sich die Plandaten auf die vorhandenen Maschinen.

**Merke**

| Begriff | Definition |
| :--- | :--- |
| **Aggregattyp** | Aggregattypen sind die Maschinentypen, die Sie in Ihrer Produktion einsetzen, z. B. Schneidtische, Bohrmaschinen, Schleifmaschinen, ESG-Öfen usw. Ein Aggregattyp kann mehrere einzelne Arbeitsstationen zusammenfassen, z. B. die ISO-Linie. Zu jedem Aggregattyp legen Sie fest, welche Restriktionen jeweils geprüft werden. |
| **Aggregat** | Aggregate sind alle Stationen, an denen Zeiten verbraucht werden. Neben den eigentlichen Maschinen zum Schneiden, Bohren usw. gilt auch Kontrolle, Versand, Verpacken als Aggregat. In A+W Business Pro gibt es keine logischen Maschinen. |
| **Produktionsbereich** | Produktionsbereiche fassen die Aggregate zusammen, die die gleichen Tätigkeiten ausführen oder in denen eine Folge von Tätigkeiten ausgeführt wird, z. B. ISO-Fertigung. |
| **Arbeitsart** | Die Arbeitsart bezeichnet die Tätigkeit, die an einem Aggregat ausgeführt wird. Alle Tätigkeiten, für die Zeiten berechnet werden, müssen als Arbeitsart definiert werden, z. B. Schneiden, Schleifen, Bohren, Verpacken usw. |
| **Arbeitsgang** | Der Begriff bezeichnet in dieser Dokumentation die Ausführung einer Arbeitsart für eine Auftragsposition. In der Regel sind in einer Auftragsposition mehrere Arbeitsgänge nötig. |
| **Restriktionen** | Einschränkungen bei bestimmten Aggregaten (Maschinen), müssen geprüft werden. Diese Prüfungen werden übergreifend für den Aggregattyp aktiviert. In der Definition eines Aggregats legen Sie die Werte fest, die für die Prüfung herangezogen werden sollen und nicht über- oder unterschritten werden dürfen. ⇨ "Arbeitsarten und Zeitzuschläge" auf Seite H-2971 |

---
*H-2930 & H-2931*
*A+W Business Pro Kapazitätsplanung*
---

#### Aggregattypen und Aggregate

Als Aggregate werden in der Kapazitätsplanung alle technischen Arbeitsmittel bezeichnet, an denen die Arbeitsschritte ausgeführt werden. Das können sowohl einzelne Maschinen als auch ganze Linien oder der Versand sein. Da unterschiedliche Maschinen gleiche Arbeitsschritte ausführen können, können jedem Aggregattyp mehrere Maschinen zugeordnet sein.

*Abb. H-4 Beispiel: Aggregattyp Zuschnitt und zugeordnete Aggregate*
*(A) Screenshot der Aggregattypen-Liste, zeigt Prüfoptionen wie Maß-Check, SZR, Gesamtstärke. (B) Screenshot des Dialogs für ein Aggregat "Zuschnitt / Cutting", das dem Aggregattyp "Zuschnitt" zugeordnet ist.*

Als Beispiel sehen Sie hier den Aggregattyp Zuschnitt, zu dem mehrere Aggregate (Maschinen) (B) gehören.
Bei der Planung der Kapazitäten werden die jeweils zur Verfügung stehenden Aggregate auf ihre Auslastung hin abgefragt. Dabei wird auch geprüft, ob beim jeweiligen Aggregattyp Einschränkungen (Restriktionen) geprüft werden müssen (A) und ob die für die Maschine hinterlegten Werte durch die Auftragsposition verletzt werden.

##### Restriktionen
Zu jedem Aggregattyp legen Sie fest, welche Restriktionen jeweils geprüft werden müssen.

**Beispiel**
Bei Aggregattyp Zuschnitt sollen folgende Werte geprüft werden:
- **Maße:** Einer der Schneidtische kann eine bestimmte Größe der Lagerplatten nicht mehr aufnehmen.
- **Einzelstärke:** Der Schneidkopf muss bei bestimmten Glasstärken geändert werden.
- **Gewicht:** Je nach Gewicht ist ein zweiter Werker erforderlich, der an nur einem der Schneidtische arbeitet.
- **Modell:** Der automatische Zuschnitt ist für Modelle nicht geeignet.
- **Drehbarkeit:** Ornamentgläser dürfen nicht gedreht werden.

Bei den Aggregaten sind die Felder freigeschaltet, in denen die Werte für die aktivierten Prüfungen eingetragen werden.

*Abb. H-5 Prüfungswerte für Aggregat Automatischer Zuschnitt*
*(Screenshot des Restriktions-Dialogs, der zeigt, dass für Höhe und Breite Werte hinterlegt sind (A), aber für die Glasstärke keine Prüfung aktiviert ist (B).)*

In diesem Beispiel sehen Sie, dass das Aggregat Zuschnitt keine Schnitte unter 100 mm (A) machen kann. Außerdem kann es nur Glasstärken von 4 bis 10 mm (B) schneiden. Im Handzuschnitt könnte die Glasstärke z. B. zwischen 2 und 99 mm angegeben werden, was bedeutet, dass dann Auftragspositionen mit einer Glasstärke von 12 mm von Hand zugeschnitten werden müssen.

> **Aktivierte Restriktionsprüfungen**
> Wenn eine Restriktion geprüft wird, darf das entsprechende Feld nicht leer bleiben. Wenn der Wert nicht geprüft werden soll, tragen Sie in den Feldern Werte ein, die nicht unter- oder überschritten werden können, z. B. 0,1 und 9999.
> ⇨ "Produktionsbereich anlegen" auf Seite H-2939

*Abb. H-6 Prüfungen für Aggregat Zuschnitt*
*(Screenshot zeigt die Einstellungen für ein Aggregat: (A) Checkbox "Scheiben drehbar" ist aktiv. (B) Checkbox "Modelle möglich" ist nicht aktiv. (C) Die Prüfung für den Aggregattyp ist nicht aktiviert. (D) Das Feld "Gewicht" ist editierbar.)*

In diesem Beispiel sehen Sie, dass der Zuschnitt von Modellen bei dem Aggregat Zuschnitt nicht möglich ist. Darum wird die Auftragsposition geprüft und nicht an diese Maschine weitergegeben, wenn ein Modell enthalten ist. Für das Aggregat Handzuschnitt wäre der Modellzuschnitt möglich, die Checkbox ist dann markiert.

Beim Aggregat Handzuschnitt ist das Gewicht auf 30 kg eingestellt. Für den normalen Zuschnitt könnte hier z. B. das Gewicht 999 kg eintragen sein, weil die Scheiben automatisch transportiert werden.

#### Zeit und Kosten pro Aggregat

Zu jedem Aggregat (Maschine) hinterlegen Sie Angaben, aus denen die Kosten für die Maschine und die Zeit errechnet werden, die bei der Produktion einer Auftragsposition anfallen.

Aus den Angaben für die Zeit werden die Kapazitäten der einzelnen Maschine und des gesamten Produktionsbereichs berechnet.

*Abb. H-7 Angaben zur Berechnung von Zeiten und Kosten pro Aggregat (Maschine)*
*(Diagramm, das zeigt, wie sich die Kosten und Zeiten eines Aggregats aus "Anzahl der Einheiten pro Stunde", "Kosten pro Std." (Lohn, Maschine, Variable) und "Arbeitsarten" zusammensetzen.)*

Zu jedem Aggregat werden die Kosten hinterlegt, die pro Einheit entstehen. Die Anzahl der Einheiten pro Stunde ergibt sich aus der gemessenen Zeit für die Arbeitsart. Die Kapazität des Aggregats ergibt sich aus:
- Einheiten pro Stunde
- Anzahl der Stunden pro Schicht
- Anzahl der Schichten, in denen das Aggregat arbeitet.

Die Ermittlung der Einheiten pro Aggregat und die Berechnung der Zeit- und Maschinenkosten pro Auftrag sind in separaten Einheiten beschrieben.
⇨ "Arbeitseinheiten" auf Seite H-2950
⇨ "Produktionskosten" auf Seite H-3069

Zur Definition der Daten eines neuen Aggregats gehören weitere Angaben, z. B. technische Restriktionen und Prioritäten, die in den folgenden Abschnitten beschrieben werden. Anschließend finden Sie dann eine ausführliche Handlungsanleitung, nach der Sie die Daten erfassen können.
⇨ "Aggregat anlegen" auf Seite H-2940

Wie Sie die Auswahl eines Aggregats bei der automatischen Auslastung steuern können, lernen Sie in einer separaten Einheit.
⇨ "Auswahl der Aggregate" auf Seite H-2995

---
*H-2932 to H-2935*
*A+W Business Pro Kapazitätsplanung*
---

#### Arbeitsarten

Arbeitsarten (Vorgänge, Tätigkeiten) bilden die Grundlage für die Produktionsreihenfolge. Den Arbeitsarten werden jeweils die Aggregate zugeordnet, die diese Arbeitsarten ausführen können. Eine Arbeitsart kann von mehreren Maschinen ausgeführt werden. Manche Aggregate können mehrere Arbeitsarten ausführen.

**Beispiel**
Arbeitsart Polieren kann auf mehreren Aggregaten ausgeführt werden:
- Einseitige Schleifmaschine
- Zweiseitige Schleifmaschine
- Schleifmaschine für Serien
- CNC-Maschine

Ein Produktionsprozess kann mehrere Arbeitsarten umfassen, z. B. bei der VSG-Fertigung eine Arbeitsart VSG-Vorverbund und eine Arbeitsart VSG-Autoklav.

*Abb. H-8 Arbeitsarten*
*(Screenshot des Dialogs 'Arbeitsarten' mit Spalten für Nr., Bezeichnung, Sequenz, Manuelle Agg.-Auswahl, Ausweich-Arbeitsart. Verschiedene Arbeitsarten für Zuschnitt sind hervorgehoben (A).)*

In diesem Beispiel sehen Sie, dass für den Zuschnitt (A) mehrere Arbeitsarten eingerichtet sind: maschineller Zuschnitt, Handzuschnitt und Zuschnitt von VSG-Glas. Diese Unterscheidung ist notwendig, weil für diese Arbeitsarten unterschiedliche Maschinen eingesetzt werden und unterschiedliche Kosten anfallen.

Die Sequenz (B) gibt die Produktionsreihenfolge der einzelnen Arbeitsarten innerhalb der Kapazitätsplanung an. Die ersten Arbeitsarten betreffen in aller Regel den Zuschnitt, die anschließenden Arbeitsarten müssen dann so definiert werden, dass die Reihenfolge stimmt. Da z. B. bei der Fertigung einer ISO-Einheit auch eine ESG-Scheibe verwendet werden könnte, muss die Arbeitsart ESG-Vorspannen immer vor der ISO-Fertigung ausgeführt werden, sie hat also eine höhere Priorität als ISO-Fertigung.

Arbeitsarten, für die bei der Planung eine Maschine nur manuell ausgewählt werden darf, müssen gekennzeichnet werden (C), z. B. da Aggregat Handzuschnitt.

Den Arbeitsarten werden die Maschinen über die Vorgabezeiten zugeordnet. Die Vorgabezeiten werden ausführlich in der Einheit Zeitvorgaben beschrieben.
⇨ "Zeitvorgaben" auf Seite H-2964

##### Ausweich-Arbeitsart

Ausweich-Arbeitsarten (D) werden festgelegt, um auf besondere Situationen zu reagieren, z. B. auf das Bohren dicker Scheiben, für die andere Zeiten und andere Aggregate erforderlich sind. Das System erkennt anhand der technischen Vorgaben und der Auftragsposition, wann die Ausweich-Arbeitsart gewählt werden muss und berechnet die Zeit und die Kosten dann entsprechend.

*Abb. H-9 Ausweicharbeitsart für dicke Scheiben*
*(Diagramm: Ein Auftrag für 'Float 12 mm' führt zur Arbeitsart 'Bohren dicke Scheiben' (Ausweich-Arbeitsart) auf 'Bohrmaschine II', da die Standard-'Bohrmaschine I' nur bis 10 mm bohren kann.)*

In diesem Beispiel sehen Sie, dass die Ausweich-Arbeitsart gewählt wird, weil die Standard-Maschine die dicke Scheibe nicht bohren kann. Die Bohrmaschine II wird gewählt, weil der Ausweich-Arbeitsart diese Maschine zugewiesen ist.

> **Neue Arbeitsart anlegen**
> Planen Sie Ihre Arbeitsarten so, dass anhand der Nummer eine Gruppierung verwandter Arbeitsarten oder der Arbeitsarten eines Produktionsprozesses zu erkennen ist.
> Neue Arbeitsarten legen Sie in der gleichen Weise an, wie alle Basistabellen. Das Vorgehen ist am Beispiel Produktionsbereich beschrieben.

---
*H-2936 & H-2937*
*A+W Business Pro Kapazitätsplanung*
---

#### Produktionsbereiche (Arbeitszentren)

Ein Betrieb ist in der Regel in verschiedene Produktionsbereiche untergliedert, z. B. Zuschnitt, Schleiferei, Bohren usw. In jedem Produktionsbereich können mehrere Maschinen stehen, die von einer festen Anzahl von Werkern bedient werden. Gleichartige Maschinen können in unterschiedlichen Produktionsbereichen stehen.

*Abb. H-10 Produktionsbereiche*
*(Screenshot des Dialogs 'Produktionsbereich' mit Spalten für Nr., Produktionsbereich, Max. Einheit/Std, Min. Verweiltage, Status Rückmeldung.)*

Von den Produktionsbereichen werden Statusmeldungen aus der Produktion gesendet, wenn die Position fertig produziert ist. Dazu geben Sie die Erfassungsstelle an, von der die Meldung gesendet wird. In diesem Beispiel werden die Meldungen über die Betriebsdatenerfassung (BDE) gesendet.

Sie sehen, dass auch für den Versand ein Produktionsbereich angelegt ist. Dies ist wichtig, damit auch die Zeiten im Versand mit eingeplant werden und die Aufträge versandfertig gemeldet werden können.

Statusmeldungen können nur von Produktionsbereichen gesendet werden, nicht von Aggregaten. Wenn Sie z. B. bei der ESG-Fertigung zwei Statusmeldungen benötigen, müssen Sie dazu zwei Produktionsbereiche einrichten: ESG-Ofen und Heat-Soak.

##### Produktionsbereich anlegen

Wenn Sie die Produktionsbereiche ganz neu einrichten, sollten Sie zunächst planen, welche Maschinen und Arbeitsarten zu ihnen gehören.

> **Voraussetzungen**
> Um die Daten sofort vollständig anlegen zu können, müssen Sie die Werte für die Einheiten pro Stunde, die Übergangszeiten und die Erfassungsstellen für die Rückmeldungen kennen. Sie können die Daten aber auch später nachtragen.

**So legen Sie die Daten für einen Produktionsbereich an**

1.  Wählen Sie im Modul Kapazitätsplanung > Stammdaten > Organisation > Produktionsbereich.
    Der Dialog *Produktionsbereiche* wird geöffnet.
    Eine Beschreibung des Dialogs finden Sie in der Softwarereferenz.
    ⇨ Softwarereferenz, "Produktionsbereich" auf Seite H-3115

2.  Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wechseln.
    Die Nummer des Produktionsbereichs wird automatisch eingesetzt und kann geändert werden.

    *Abb. H-11 Zeile für neuen Produktionsbereich eingefügt*

3.  Tragen Sie den Namen des Produktionsbereichs ein und überschreiben Sie ggf. die Nummer.
    Wenn Sie die Werte für die übrigen Felder bereits kennen, dann tragen Sie diese in die entsprechenden Felder ein.

4.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.

Die Daten werden gespeichert. Sie können jetzt die Aggregate anlegen, die dem neuen Produktionsbereich zugeordnet werden sollen.

---
*H-2938 & H-2939*
*A+W Business Pro Kapazitätsplanung*
---

##### Aggregat anlegen

Sie können alle Daten eines neuen Aggregats einzeln eingeben. Wenn Sie jedoch bereits ein vergleichbares Aggregat in Ihrem Bestand haben, sollten Sie dessen Daten als Basis verwenden. Sie erleichtern sich damit die Arbeit erheblich. In der folgenden Handlungsanleitung wird dieser Weg vorgeführt.

> **Voraussetzungen**
> Um die Daten sofort vollständig anlegen zu können, müssen Sie die Werte für die Kosten und die technischen Restriktionen bereithalten. Welche Werte Sie brauchen, können Sie der Softwarereferenz entnehmen. Sie können die fehlenden Daten aber auch später nachtragen.
> ⇨ Softwarereferenz, "Aggregate" auf Seite H-3117

**So legen Sie die Daten für eine neue Maschine an**

1.  Wählen Sie im Modul **Kapazitätsplanung > Stammdaten > Organisation > Aggregate**.

    *Abb. H-12 Produktionsbereich auswählen*
    *(Screenshot des leeren Aggregat-Dialogs)*

2.  Wählen Sie den Produktionsbereich aus, dem die neue Maschine zugeordnet werden soll, z. B. Bearbeitungen.

3.  Wählen Sie im Menü **Start > Suchen**, um die Daten der Maschinen aus diesem Produktionsbereich einzulesen.

    *Abb. H-13 Aggregate im Produktionsbereich*
    *(Screenshot des Aggregat-Dialogs, gefüllt mit Daten eines bestehenden Aggregats. A: Vorbelegte Felder. B: Name des Aggregats. C: Liste der Aggregate. D: Erfassungsstelle.)*
    In der Übersicht (C) werden alle Aggregate aufgeführt, die diesem Produktionsbereich zugeordnet sind. Die Felder der Werte (A) sind mit den Daten des markierten Aggregats vorbelegt.

4.  Markieren Sie in der Übersicht das Aggregat, dessen Werte Sie übernehmen wollen.

5.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    Das Feld für die Aggregatnummer (B) wird freigeschaltet.

6.  Überschreiben Sie die Nummer und den Namen des Aggregats.

7.  Wählen ggf. einen anderen Produktionsbereich aus.

8.  Passen in den Feldern für die Kosten (A) die Werte an.

9.  Tragen Sie im Feld Erfassungsstelle (D) die ID der Erfassungsstelle ein, von der die Fertigmeldung kommt.

    *Abb. H-14 Werte für das Aggregat anpassen*
    *(Screenshot des angepassten Aggregat-Dialogs. A: Aktivierte Prüfungen. B: Aggregat sperren.)*

10. Wählen Sie im Menü **Start > Speichern**, um die neuen Daten zu speichern.
    Damit haben Sie die neue Maschine angelegt. Die Maschine wird in der Übersicht aufgeführt. Sie können jetzt die Prüfungen (A) aktivieren und die Angaben für die technischen Restriktionen anpassen.

> **Neues Aggregat sperren**
> Wenn Sie ein neues Aggregat angelegt haben, auf das noch nicht eingelastet werden soll, dann müssen Sie es unbedingt sperren (B).

**So passen Sie die technischen Restriktionen an**

1.  Wechseln Sie zum Register **Restriktionen**.

    *Abb. H-15 Technische Restriktionen anpassen*
    *(Screenshot des Restriktionen-Tabs. A: Zugeordnete Arbeitsarten. B: Technische Restriktionen.)*

2.  Prüfen Sie im Bereich Technische Restriktionen (B), welche Werte für die Maschine gelten.
    Wenn eine benötigte Prüfung gesperrt ist, haben Sie unter Umständen im Register Aggregat den falschen Aggregattyp zugewiesen. Wenn der Aggregattyp richtig eingestellt ist, sollten Sie im Dialog Aggregattypen prüfen, ob die Checkboxen für die Prüfungen korrekt markiert sind.

> **Neue Restriktionsprüfung aktiviert**
> Wenn Sie im Aggregattyp eine Restriktionsprüfung aktivieren, müssen Sie in allen Aggregaten die entsprechenden Felder füllen. Tragen Sie mindestens null (0) ein, damit das Feld nicht leer bleibt.

3.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert. Die Angaben zu den zugewiesenen Arbeitsarten (A) werden erst angezeigt, wenn Sie diese in den Dialogen zur Zuordnung festgelegt haben.

---
*H-2940 to H-2943*
*A+W Business Pro Kapazitätsplanung*
---

### Übungen

- Überlegen Sie, wie die Produktion räumlich organisiert ist und wie Sie diese Organisation in den Stammdaten mit Produktionsbereichen und Maschinen abbilden können.
- Legen Sie einen Produktionsbereich ISO-2 und die zugehörigen Maschinen an.
- Die Übungen bauen aufeinander auf. Sie sollten sich daher mehrere unterschiedliche Maschinen anlegen, um in den Übungen der nächsten Einheiten Vergleichsmöglichkeiten zu haben.
- Legen Sie eine Arbeitsart für 3-fach-ISO an.

> **Übungen im realen Betrieb**
> Wenn Ihre Kapazitätsplanung bereits im Tagesgeschäft eingesetzt wird, dann müssen Sie neue Maschinen unbedingt sperren, damit diese nicht in der Planung berücksichtigt werden.

#### Ergänzende Informationen
⇨ Softwarereferenz, "Aggregattypen" auf Seite H-3104
⇨ Softwarereferenz, "Arbeitsarten" auf Seite H-3107
⇨ Softwarereferenz, "Zugeordnete Aggregate" auf Seite H-3110
⇨ Softwarereferenz, "Produktionsbereich" auf Seite H-3115
⇨ Softwarereferenz, "Aggregate" auf Seite H-3117

---
*H-2944*
*A+W Business Pro Kapazitätsplanung*
---

### Schicht- und Arbeitszeiten

**Lernziele**
- Schichtzeiten und Kalender einrichten.
- Arbeitseinheiten kennenlernen.
- Kapazitäten pro Produktionsbereich und pro Aggregat berechnen.

**Nutzen**
- Mit den hinterlegten Schichten und den Angaben zu Arbeitseinheiten wird die Kapazität eines jeden Produktionsbereichs errechnet. Anhand dieser Kapazität wird die Terminierung der eingelasteten Aufträge durchgeführt.

**Merke**

| Begriff | Definition |
| :--- | :--- |
| **Schicht** | Die Schichten in den verschiedenen Produktionsbereichen können unterschiedlich lang sein. Der Schichtbeginn muss für alle Produktionsbereiche zur selben Uhrzeit festgelegt werden, damit keine Überschneidungen beim Schichtwechsel und Übergang von einem zum nächsten Produktionsbereich entstehen. |
| **Arbeitseinheit** | Mit Arbeitseinheiten geben Sie an, wie viel pro Stunde gefertigt werden kann. Arbeitseinheiten können als Mannstunden oder als Maschinenstunden angegeben werden. |
| **Kapazität** | Die Kapazität einer Maschine ist das Produkt aus Arbeitseinheiten und Schichtstunden. Die Kapazität eines Produktionsbereichs ist die Summe aller Maschinenkapazitäten im Produktionsbereich. |
| **Geschlossene Kapazität**| Bei geschlossenen Kapazitäten wird automatisch nach einem anderen Termin gesucht, wenn die verfügbaren Schichten und Maschinen ausgelastet sind. |
| **Offene Kapazität** | Bei offenen Kapazitäten wird die Schichtzeit nicht geprüft. |
| **Voreinstellungen** | Firmendaten: Register Kapa-Planung > Anzahl der Schichten |

---
*H-2945*
*A+W Business Pro Kapazitätsplanung*
---

#### Arbeitszeiten

Für die Berechnung von Terminen werden Vorgaben herangezogen, die Sie in unterschiedlichen Dialogen hinterlegen. Dies sind z. B. Werte für:
- Zeit, die eine Maschine eingesetzt werden kann (Schichtzeit).
- Zeit, die benötigt wird, um ein Stück zu fertigen (Vorgabezeit).
- Zeit, die mehr aufgewendet wird, wenn der Arbeitsgang aufwendiger ist (Zeitzuschlag).
- Rüstzeit.
Im Folgenden werden die Zusammenhänge der unterschiedlichen Zeitvorgaben und der Voreinstellungen für die Arbeitszeiten näher erklärt.

##### Arbeitstage und Schichten

Für die Terminberechnung in der Kapazitätsplanung ist es wichtig, ob Ihr Betrieb in Schichten arbeitet oder nicht.
- Wenn nicht in Schichten gearbeitet wird, greift die Kapazitätsplanung auf den A+W Business Pro-Standard-Kalender zu.
- Wenn in Schichten gearbeitet wird, können die Schichtzeiten pro Produktionsbereich hinterlegt werden.

Wenn nicht alle Produktionsbereiche in allen Schichten arbeiten, richtet sich die Anzahl der Schichten nach dem Produktionsbereich mit den meisten Schichten. Die Anzahl der Schichten legen Sie im Modul Stammdaten > Firma > Firmendaten fest.

*Abb. H-16 Firmendaten - Register Kapa-Planung*
*(Screenshot des Firmendaten-Dialogs, Register 'Kapazitätsplanung', mit dem Feld 'Schichtenzahl' auf 3 gesetzt.)*

Die Länge einer Schicht wird im Kalender pro Aggregat oder Produktionsbereich festgelegt. Wenn z. B. mehrere Produktionsbereiche in drei Schichten mit unterschiedlichen Schichtlängen arbeiten, dann müssen Sie die Schichten so einteilen, dass die Schichten 2 und 3 in allen Produktionsbereichen zur gleichen Uhrzeit beginnen.

Die Schichten der verschiedenen Produktionsbereiche dürfen sich zeitlich nicht überlagern, weil sonst der Übergang von einer Schicht in die nächste beim Wechsel des Produktionsbereichs nicht eindeutig ist.

**Beispiel**

| Produktions-Bereich | Beginn 1. Schicht | Anzahl Std. | Beginn 2. Schicht | Anzahl Std. | Beginn 3. Schicht | Anzahl Std. | Ende |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Zuschnitt | 06:00 | 6 | 12:00 | 4 | 16:00 | 4 | 20:00 |
| VSG | 08:00 | 4 | 12:00 | 4 | 16:00 | 4 | 20:00 |
| Bohren | 10:00 | 2 | 12:00 | 4 | 16:00 | 2 | 18:00 |
| Heat-Soak-Test | 08:00 | 12 | | 0 | | 0 | 20:00 |

Bei einer solchen Schichtorganisation ist gewährleistet, dass sich keine Arbeitsverzögerungen von einer Schicht zur anderen ergeben, da die Schichtwechsel in den Produktionsbereichen zur selben Zeit stattfinden.

Die Zeiten des Schichtwechsels legen Sie im Modul **Kapazitätsplanung > Stammdaten > Organisation > Kalender > Menü Funktionen > Schichtzeiten** fest.

*Abb. H-17 Einstellungen für Schichtwechsel*
*(Screenshot des Dialogs 'Einstellungen Schichten' mit Feldern für Schichtwechselzeiten, z.B. Schicht 1 > Schicht 2 um 12:00 Uhr.)*

In diesem Beispiel sehen Sie, dass die Schicht 2 um 12:00 Uhr beginnt und um 16:00 Uhr endet. Darauf folgt, dass Schicht 1 bei einer Schichtzeit von 6 Std. um 6:00 Uhr beginnt. Der Übergang von Schicht 2 zu Schicht 3 ist um 16:00 Uhr, was bedeutet, dass die Schicht 2 nur 4 Stunden lang ist.

---
*H-2946 & H-2947*
*A+W Business Pro Kapazitätsplanung*
---

##### Maximale Kapazität pro Tag

Die Kapazität einer Maschine pro Tag wird in Arbeitseinheiten gerechnet. Die Kapazität für den jeweiligen Produktionsbereich setzt sich aus den Einheiten pro Stunde aller Maschinen zusammen, die zum Produktionsbereich gehören.

*Abb. H-18 Berechnungen von Zeiten pro Aggregat (Maschine) und Produktionsbereich*
*(Diagramm, das zeigt, wie die Kapazität eines Produktionsbereichs aus der Summe der Kapazitäten der einzelnen Aggregate (z.B. Schneidtisch A und B) berechnet wird.)*

Die maximale Kapazität einer Maschine ergibt sich aus den im Kalender eingetragenen Summen der Stunden pro Tag, multipliziert mit den Arbeitseinheiten pro Stunde, die für die Maschine im Dialog Aggregat hinterlegt sind.

**Beispiel**
Tag: Dienstag, Produktionsbereich Zuschnitt, Maschine Schneidtisch.
Am Schneidtisch können 4 Arbeitseinheiten pro Stunde gemacht werden.

| Schicht | Stunden | x 4 Arbeitseinh./Std | = Max. Arbeitseinh./Schicht |
| :--- | :--- | :--- | :--- |
| 1. Schicht | 6 Std. | x 4 A.Einh./Std. | = 24 A.Einh./Schicht |
| 2. Schicht | 4 Std. | x 4 A.Einh./Std. | = 16 A.Einh./Schicht |
| 3. Schicht | 4 Std. | x 4 A.Einh./Std. | = 16 A.Einh./Schicht |
| **Max. Kapazität pro Tag am Schneidtisch** | | | **= 56 A.Einh./Tag** |

⇨ "Arbeitseinheiten" auf Seite H-2950
⇨ "Kalender anpassen" auf Seite H-2957

Die Kapazität eines Produktionsbereichs ergibt sich aus der Summe der Tageskapazitäten aller Maschinen in diesem Produktionsbereich.
Sie müssen dabei jedoch berücksichtigen, ob alle Aggregate jederzeit einsetzbar sind. Wenn Sie z. B. 6 Schleifmaschinen haben, aber nur drei Werker, die an diesen Maschinen arbeiten können, können Sie die Gesamtkapazität nur für drei Maschinen berechnen. Die Prüfung der freien Kapazitäten bezieht sich daher nicht nur auf die Maschinen selbst, sondern auch auf die maximale Anzahl von Einheiten, die in einem Produktionsbereich gefertigt werden können.

*Abb. H-19 Anzahl der Einheiten*
*(A: Screenshot-Ausschnitt zeigt 'Max. Einheit/Std' im Produktionsbereich. B: Screenshot-Ausschnitt zeigt 'Einheiten' im Aggregat.)*

Wie Sie die Arbeitseinheiten bestimmen, lernen Sie in der folgenden Einheit.

---
*H-2948 & H-2949*
*A+W Business Pro Kapazitätsplanung*
---

##### Arbeitseinheiten

Arbeitseinheiten kann sowohl für jedes einzelne Aggregat als auch für den gesamten Produktionsbereich angegeben werden. Für beide Angaben legen Sie dieselbe Berechnungsart der Arbeitseinheit zugrunde.

Bevor Sie die Werte hinterlegen, müssen Sie festlegen, welche Arbeitseinheit verwendet wird. Es gibt viele Möglichkeiten, z. B.:
- Arbeitseinheit = Mannstunde
- Arbeitseinheit = Maschinenstunde

Folgende Fragen müssen Sie beantworten, um die Arbeitseinheiten pro Stunde und die Vorgabezeiten einrichten zu können:
- In welcher Arbeitseinheit soll die Kapazitätsberechnung der Maschine erfolgen?
- Was ist unter Mannstunde, Maschinenstunde usw. zu verstehen?
  ⇨ "Arbeitseinheit = Mannstunde" auf Seite H-2951
  ⇨ "Arbeitseinheit = Maschinenstunde" auf Seite H-2954
- Welcher Wert muss für die Einheit/Std. eingetragen werden?
  ⇨ Softwarereferenz, "Aggregate" auf Seite H-3117
- Wie viel Zeit braucht die Maschine für eine Einheit (lfm, qm, Stück) bezogen auf die Arbeitseinheit?
  ⇨ "Ermittlung der Mannstunden" auf Seite H-2952

###### Arbeitseinheit = Mannstunde

Anhand der Arbeitseinheiten wird beim Einlasten geprüft, ob noch Kapazitäten für diesen Tag zur Verfügung stehen.

**Beispiel**
Im Produktionsbereich Bohren (5 Maschinen) arbeiten 12 Personen in insgesamt drei Schichten pro Tag. Pro Schicht arbeiten also vier Personen. Diese vier Personen entsprechen vier Arbeitseinheiten im Produktionsbereich Bohren.
Auch wenn nur vier Personen im Produktionsbereich für fünf Maschinen zur Verfügung stehen, kann theoretisch jede Maschine die ganze Schichtzeit, z. B. acht Stunden, laufen. Das heißt, Sie tragen bei jeder Maschine die Arbeitseinheit gleich 1 ein. Welche vier der fünf Maschinen jedoch letztlich eingesetzt werden, hängt von den Einlastungsdaten ab.

Folgendes wird geprüft:
- Ist die Maschine ausgelastet?
- Wenn ja, stehen noch andere Maschinen zur Verfügung? Das heißt: Ist die maximale Kapazität des Produktionsbereiches von vier Arbeitseinheiten bereits erreicht?
  - Wenn ja, kann auf eine freie Maschine eingelastet werden.
  - Wenn nein, muss der Arbeitsgang auf den nächsten Tag oder die nächste Schicht verschoben werden oder es wird entschieden, dass Überstunden gemacht werden müssen.

> **Anwesende Werker**
> Die Kapazitätsplanung geht davon aus, dass immer alle Personen (Werker) da sind.

###### Ermittlung der Mannstunden

Um die Mannstunden zu ermitteln, müssen die Zeitwerte mit der Anzahl der Personen, die an der Maschine arbeiten, multipliziert werden. Je nachdem, ob Sie Einzelzeiten oder eine Staffelung, z. B. nach Dicke, definieren, wird die Vorgabezeit anders berechnet. Die folgenden Beispiele sind reine Berechnungsbeispiele.

**Beispiel: 3 Personen, Einzelzeit**
Berechnung von Mannstunden am Schneidtisch:
- 3 Personen arbeiten am Schneidtisch.
- In einer Stunde können 200 qm zugeschnitten werden.
- Die Vorgabezeit wird als Einzelzeit hinterlegt.

**Formel:**
Vorgabezeit 1 qm = (1 Std / Anzahl qm pro Stunde) x Anzahl Personen [Mannstunden]

**Rechenbeispiel:**
Vorgabezeit 1 qm = (1 Std / 200 qm) x 3 Personen = 0,015 [Mannstunden]

**Beispiel: gestaffelte Zeit (Vektor)**
Berechnung von Mannstunden am Schneidtisch, gestaffelt nach Dicke:
- 3 Personen arbeiten am Schneidtisch.
- Gestoppte Zeit pro gefertigte Einheit, nach Dicke des Glases gestaffelt.
- Die Vorgabezeiten werden im Vektor-Format hinterlegt.

**Formel:**
Vorgabezeit 1 qm = gestoppte Zeit x Anzahl Personen [Mannstunden]

**Rechenbeispiel:**
Vorgabezeit 1 qm Float 4 mm = 0,009 Std. x 3 Personen = 0,027 Mannstunden
Vorgabezeit 1 qm Float 6 mm = 0,010 Std. x 3 Personen = 0,03 Mannstunden

**Beispiel: 2 Personen, Einzelzeit**
Berechnung von Mannstunden an der Schleifmaschine:
- 2 Personen arbeiten an der Schleifmaschine.
- In einer Stunde können 3 Laufmeter geschliffen werden.
- Die Vorgabezeit wird als Einzelzeit hinterlegt.

**Formel:**
Vorgabezeit = (1 Std / Anzahl Ifm pro Stunde) x Anzahl Personen [Mannstunden]

**Rechenbeispiel:**
Vorgabezeit = (1 Std / 3 lfm) x 2 Personen = 0,66 [Mannstunden]

---
*H-2950 to H-2953*
*A+W Business Pro Kapazitätsplanung*
---

###### Arbeitseinheit = Maschinenstunde

Wenn die Zeiten unabhängig von der Anzahl der Werker an der Maschine sind, können Sie die Arbeitseinheit Maschinenstunden einsetzen.
In diesem Fall muss als Arbeitseinheit für das Aggregat immer eine 1 eingetragen werden.

*Abb. H-20 Dialog Aggregate – Einheiten und Kosten*
*(Screenshot-Ausschnitt zeigt die Kosten- und Einheiten-Felder für ein Aggregat, wobei 'Einheiten' auf '1,0 pro Stunde' gesetzt ist.)*

Standardmäßig wird der Wert 1 für die Anzahl der Einheiten eingegeben. Damit können Sie besser nachvollziehen, wie die Kapazitäten berechnet werden.

###### Arbeitseinheiten pro Produktionsbereich

Im Normalfall entspricht die Anzahl der Arbeitseinheiten je Produktionsbereich der Anzahl der Maschinen, die dort eingesetzt werden. Wenn 3 Maschinen eingesetzt werden, dann ist die Anzahl der Arbeitseinheiten gleich 3.

Die Bedingungen in einem Betrieb könnten jedoch folgendermaßen eingeschränkt sein:
- Sie setzen in Ihrem Produktionsbereich z. B. 3 Maschinen ein.
- Die Stromversorgung lässt aber nur den gleichzeitigen Betrieb von 2 Maschinen zu. Das heißt, dass eine Maschine immer abgeschaltet sein muss.

In diesem Fall müssen Sie als Arbeitseinheit pro Stunde für den gesamten Produktionsbereich den Wert 2 eintragen.

*Abb. H-21 Einheiten pro Produktionsbereich*
*(Screenshot-Ausschnitt zeigt die Spalte 'Max. Einheit/Std' in der Produktionsbereichsliste, z.B. für 'Zuschnitt / Cutting' ist der Wert 2 eingetragen.)*

---
*H-2954*
*A+W Business Pro Kapazitätsplanung*
---

##### Voreinstellungen für Schichten und Kapazitäten

Im Modul Stammdaten legen Sie die Grundeinstellungen für die Kapazitätsplanung in A+W Business Pro fest.

*Abb. H-22 Firmendaten – Kapa-Planung*
*(Screenshot des Firmendaten-Dialogs, Register 'Kapa-Planung', mit den Feldern A: Schichtenzahl, B: Fertigungsterminmodus, C: Schichtfüllung bei Positionssplit.)*

Die **Anzahl der Schichten (A)** richtet sich nach dem Produktionsbereich, in dem die meisten Schichten gefahren werden. Die Schichten werden u. a. bei der Berechnung von Übergangsmatrix und Übergangszeiten berücksichtigt.

Sie müssen festlegen, ob Sie mit **geschlossenen oder offenen Kapazitäten** arbeiten wollen.
- Bei **geschlossenen Kapazitäten** wird automatisch nach einem anderen Termin gesucht, wenn die verfügbaren Schichten und Maschinen ausgelastet sind.
- Bei **offenen Kapazitäten** wird die Schichtzeit nicht geprüft.

Außerdem müssen Sie festlegen, wie stark eine Schicht ausgelastet werden darf, wenn die Aufträge automatisch an die Kapazitätsplanung übergeben werden. Wenn Sie die Schichten immer voll oder nahezu voll auslasten, haben Sie keinen Spielraum mehr für Umlastungen, für Eilaufträge oder für Restmengen vom Vortag.

Folgende Einstellungen im Feld **Fertigungsterminmodus (B)** stehen für den Auslastungsgrad zur Verfügung.
- **Automatisch Normalkapazität:**
  Die Aufträge werden entsprechend der zur Verfügung stehenden Schichtzeiten eingelastet. Die Überbuchung ist nicht möglich. Dies ist die Standard-Einstellung.
- **Automatisch volle Tage:**
  Bei dieser Einstellung werden die Angaben im Kalender für die Anzahl Schichten und Stunden ignoriert. Die Einlastung geht dann von einem Arbeitstag mit 24 Stunden aus. Dies gilt jedoch nur für reguläre Arbeitstage, nicht für Feiertage.
- **Nur Aggregatwechsel:**
  Bei ausgelasteten Kapazitäten soll automatisch nur nach einem anderen Aggregat gesucht werden. Wenn das ebenfalls ausgelastet wird, wird die Einlastung unterbrochen und Sie müssen manuell eingreifen.
- **Einlasten ohne Kontrolle:**
  Diese Einstellung entspricht der offenen Schicht. Das heißt z. B., dass trotz der Schichtzeit von 8 Std. auch 16 Std. eingelastet werden können. Dabei wird keine Meldung ausgegeben, wenn ein Tag voll ausgelastet ist.

Große Positionen können auf mehrere Aggregate, Schichten oder Tage verteilt werden. Dazu geben Sie im Feld **Schichtfüllung bei Positionssplit (C)** an, zu wie viel Prozent die Schicht eines Aggregats durch das Splitting gefüllt werden darf, um Platz für andere Aufträge zu behalten.

> **Einstellungen ändern**
> Wenn Sie Einstellungen in den Firmendaten geändert haben, sollten Sie A+W Business Pro neu starten.

Die weiteren Einstellungen für Arbeitstage und Schichten werden Sie in den zugehörigen Lerneinheiten kennenlernen.

---
*H-2955 & H-2956*
*A+W Business Pro Kapazitätsplanung*
---

##### Kalender anpassen

Standardmäßig geht die Kapazitätsplanung von einer Schicht pro Tag aus. Wenn Sie jedoch in Ihrem Betrieb mit mehr als einer Schicht arbeiten wollen, dann müssen Sie als ersten Schritt die Anzahl der Schichten in den Firmendaten festlegen.

Danach können Sie pro Arbeitsart und Aggregat oder pro Produktionsbereich einen eigenen Kalender mit den jeweiligen Schichten bzw. Schichtzeiten anlegen. Wenn Sie für einen Produktionsbereich oder ein Aggregat keinen eigenen Kalender anlegen, gilt der allgemeine Kalender.

> **Jahreswechsel**
> Wenn Sie die Kapazitäten über den Jahreswechsel hinaus planen wollen, müssen Sie den Kalender für das neue Jahr mit allen Schichtzeiten angelegt haben.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
- "So legen Sie die Anzahl der Schichten fest" auf Seite H-2957
- "So legen Sie einen neuen Kalender an" auf Seite H-2958
- "So richten Sie weitere Schichtzeiten ein" auf Seite H-2961
- "So richten Sie eine Sonderschicht ein" auf Seite H-2962

> **Kalender ändern**
> Wenn Sie einen Kalender bearbeitet oder angelegt haben, müssen Sie A+W Business Pro neu starten, damit die Daten beim Einlasten zur Verfügung stehen.

**So legen Sie die Anzahl der Schichten fest**

1.  Wählen Sie im Modul **Stammdaten > Firma > Firmendaten**.
2.  Wechseln Sie zum Register **Kapa-Planung**.
3.  Tragen Sie im Bereich **A+W Business Kapazitätsplanung** die Anzahl der Schichten ein.

    *Abb. H-23 Firmendaten - Register Kapa-Planung*

4.  Wählen Sie im Menü **Start > Speichern**, um die Änderungen zu speichern.
    Die Daten werden gespeichert. Im Kalender der Kapazitätsplanung werden die Felder für die Schichtzeiten freigeschaltet.

**So legen Sie einen neuen Kalender an**

1.  Wählen Sie im Modul **Kapazitätsplanung > Stammdaten > Organisation > Kalender**.

    *Abb. H-24 Kalender anlegen*
    *(Screenshot des Kalender-Dialogs mit Auswahl für Modus (Arbeitsart/Aggregat oder Produktionsbereich/Mandant) und den entsprechenden Feldern.)*
    Eine Beschreibung des Dialogs finden Sie in der Softwarereferenz.
    ⇨ Softwarereferenz, "Kalender" auf Seite H-3127

2.  Wählen Sie den Modus (C):
    - **Arbeitsart/Aggregat:** Der neue Kalender soll für ein Aggregat und/oder eine Arbeitsart eingerichtet werden.
    - **Produktionsbereich/Mandant:** Der neue Kalender soll für einen Produktionsbereich und/oder einen Mandanten eingerichtet werden.
    Die Beschriftung der Felder (A) hängt vom Modus ab. In diesem Beispiel wird der Kalender für ein Aggregat angelegt.

3.  Wählen Sie die Arbeitsart und das Aggregat aus.

4.  Wählen Sie das Jahr (B) aus.
    Wenn Sie eine neue Jahreszahl eingeben, wird der Kalender für dieses Jahr angelegt.

5.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.

    *Abb. H-25 Kalender für Aggregat einrichten*

6.  Wechseln Sie zum Register **Kalender**.

    *Abb. H-26 Schichtzeiten eintragen*
    *(Screenshot des Kalenderregisters mit Wochentagen und Feldern für Stunden pro Schicht. A: Wochentage, B: Stunden, C: Kalenderübersicht, D: Übertragen-Button.)*

7.  Tragen Sie pro Arbeitstag und Schicht die Schichtzeit (B) ein.
    Achten Sie darauf, dass die Checkboxen (A) der Tage, an denen Sie Schichtzeiten eingetragen haben, markiert sind.
    Wenn Sie die Zeiten eingetragen haben, werden die Schaltflächen zur Übertragung freigeschaltet.

8.  Klicken Sie auf die Schaltfläche **[Auf Jahr übertragen]** (D).
    Die Daten werden in die Übersicht Kalender (C) übernommen. Wenn Sie eine neue Jahreszahl eingegeben haben, wird der neue Kalender angelegt.

9.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert. Die Schicht wird bei der Planung berücksichtigt, nachdem Sie A+W Business Pro neu gestartet haben. Sie können nun die Schichtzeiten weiter bearbeiten.

---
*H-2957 to H-2960*
*A+W Business Pro Kapazitätsplanung*
---

**So richten Sie weitere Schichtzeiten ein**

1.  Wählen Sie im Modul **Kapazitätsplanung > Stammdaten > Organisation > Kalender**.
2.  Wählen Sie das aktuelle Kalenderjahr aus.
3.  Wählen Sie im Menü **Start > Suchen**, um die Suche zu starten. Alle Kalender, die den Auswahlkriterien entsprechen, werden eingelesen.
4.  Markieren Sie den gewünschten Kalender und wechseln Sie zum Register **Kalender**.
5.  Markieren Sie in der Übersicht Kalender eine Woche, damit die Schichtzeiten eingelesen werden.
6.  Tragen Sie im Bereich **Stunden pro Schicht** die Stunden für die neue Schicht ein. Achten Sie darauf, dass Sie die Stunden für alle Schichten eingetragen sein müssen. Wenn Sie die Felder der schon bestehenden Schichtzeiten leer lassen, werden die Zeiten bei der Übertragung auf die Woche oder das Jahr gelöscht.

    *Abb. H-27 Schichtzeiten ergänzen*
7.  Prüfen Sie, ob alle Checkboxen der Wochentage, für die Sie die Stunden eingetragen haben, markiert sind.
8.  Klicken Sie auf die Schaltfläche **[Auf Jahr übertragen]**. Damit werden die Schichtzeiten auf das gesamte Kalenderjahr übertragen.
9.  Wählen Sie im Menü **Start > Speichern**, um die Änderungen zu speichern. Die Daten werden gespeichert. Die Schichtzeiten werden bei der Planung berücksichtigt, nachdem Sie A+W Business Pro neu gestartet haben.

**So richten Sie eine Sonderschicht ein**

1.  Wählen Sie den gewünschten Kalender und wechseln Sie zum Register **Kalender**.

    *Abb. H-28 Sonderschicht einrichten*
    *(Screenshot des Kalenderregisters. A: Stunden der Sonderschicht, B: Kalenderwoche der Sonderschicht, C: "Auf KW übertragen" Button.)*

2.  Wählen Sie die Kalenderwoche (B) aus, in der die Sonderschicht gefahren werden soll.
3.  Tragen Sie die Stunden (A) der neuen Sonderschicht ein.
4.  Klicken Sie auf die Schaltfläche **[Auf KW übertragen]** (C). Damit werden die Schichtzeiten nur für die gewählte Kalenderwoche übernommen.
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Daten werden gespeichert. Die Sonderschicht wird bei der Planung berücksichtigt, nachdem Sie A+W Business Pro neu gestartet haben.

### Übungen
- Skizzieren Sie auf Papier den Schichtenplan Ihrer Produktionsbereiche.
- Legen Sie fest, dass in 3 Schichten gearbeitet werden soll (Firmendaten!).
- Tragen Sie die Stunden im Kalender ein. Beachten Sie dabei, dass die Arbeitszeit in den verschiedenen Produktionsbereichen und an den verschiedenen Wochentagen unterschiedlich ist. Beispiel Versand: Sind 8 Stunden in Schicht 3 am Freitag sinnvoll?
- Erhöhen Sie die Anzahl der Schichten und prüfen Sie, wie sich dies im Kalender auswirkt.

#### Ergänzende Informationen
⇨ Softwarereferenz, "Voreinstellungen Firmendaten" auf Seite H-3098
⇨ Softwarereferenz, "Kalender" auf Seite H-3127
⇨ Softwarereferenz, "Einstellungen Schichten" auf Seite H-3102

---
*H-2961 to H-2963*
*A+W Business Pro Kapazitätsplanung*
---

### Zeitvorgaben

**Lernziele**
- Unterschiedliche Konzepte der Zeitberechnung kennenlernen.
- Zeitvorgaben definieren.

**Nutzen**
- Anhand der zeitlichen Vorgaben und der freien Kapazitäten wird berechnet, wann welcher Produktionsschritt eines Auftrags ausgeführt werden kann.

**Merke**

| Begriff | Definition |
| :--- | :--- |
| **Vorgabezeiten** | Für alle Tätigkeiten (Arbeitsarten) werden die Zeiten gemessen, die benötigt werden, um diese eine Tätigkeit auszuführen. Diese gemessenen Zeiten werden als Vorgabezeiten angegeben. |
| **Basiszeit** | Gestoppte Zeit, die eine Arbeitsart an einem Aggregat benötigt, um eine Einheit zu fertigen. Diese Zeit kann durch Zuschläge erhöht oder vermindert werden. |
| **Zeitzuschlag** | Ein Zeitzuschlag ist ein Erschwerniszuschlag, z. B. für Mehrfach-ISO oder Modelle. Der Zeitzuschlag bezieht sich immer auf die Basiszeit, die für eine Arbeitsart an einem Aggregat hinterlegt ist. Zuschläge werden addiert. Die Basiszeit + 100% ergibt also eine Verdoppelung der Zeit. |
| **Faktor** | Faktoren werden mit der Basiszeit der Arbeitsart multipliziert. Der Faktor 1 bedeutet, dass die Zeit nicht erhöht wird. Der Faktor 0,5 bedeutet, dass die Zeit um die Hälfte reduziert wird. |
| **Sonderzeiten** | Sonderzeiten sind immer Zuschläge auf die Basiszeit einer Arbeitsart. Sonderzeiten werden verwendet, um z. B. darauf zu reagieren, wenn zwei Werker statt eines einzelnen eine Maschine bedienen müssen. Sonderzeiten können gestaffelt angegeben werden. |
| **Übergangszeiten**| Die Übergangszeit gibt an, wie lange eine Einheit braucht, um von einem Arbeitsgang oder einem Produktionsbereich zum nächsten zu kommen. Die Zeit wird in Schichten angegeben. |
| **Verweilzeiten** | Diese Zeiten geben an, wie lange eine Einheit in einem Produktionsbereich verweilt. |
| **Rüstzeiten** | Rüstzeiten werden als Arbeitsart definiert und dem Aggregat und der Bearbeitung zugeordnet. |

---
*H-2964*
*A+W Business Pro Kapazitätsplanung*
---

#### Basiskomponenten der Zeitplanung

In die Planung der Zeit fließen neben der Stückzahl aus dem Auftrag folgende Vorgaben ein:

*Abb. H-29 Zeiten*
*(Diagramm, das die verschiedenen Zeitkomponenten zeigt: Vorgabezeit (Basiszeit) für eine Arbeitsart/Aggregat wird durch Zuschläge (z.B. für Dicke) oder Faktoren (z.B. für Modelle) modifiziert. Verweiltage und Übergangszeiten zwischen Produktionsbereichen fließen ebenfalls in die Berechnung ein.)*

In dieser Übersicht sehen Sie, welche Zeitvorgaben definiert werden können:
- **Vorgabezeiten**
  geben an, wie viel Zeit eine Arbeitsart an einer bestimmten Maschine benötigt. Diese Zeiten werden im Dialog Vorgabezeiten hinterlegt.
- **Zeitzuschläge**
  sind in der Regel gestaffelte Zuschläge, die unter bestimmten Voraussetzungen die Vorgabezeiten bei rechteckigen Scheiben erhöhen. Diese Zeiten werden im Dialog Sonderzeiten hinterlegt.
- **Zeitzuschläge und Faktoren**
  erhöhen oder vermindern unter bestimmten Voraussetzungen die Vorgabezeit bei der Fertigung von nicht rechteckigen Scheiben (Modellen). Diese Zeiten werden in den Dialogen im Menü Zuordnen hinterlegt.
- **Verweiltage**
  geben an, wie lange eine Einheit in einem bestimmten Produktionsbereich verweilt. Diese Zeiten werden im Dialog Produktionsbereich hinterlegt.
- **Übergangszeiten**
  geben an, wie lange eine Einheit braucht, um von einer bestimmten Arbeitsart zu einer bestimmten anderen oder von einem bestimmten Produktionsbereich in einen bestimmten anderen zu kommen. Diese Zeiten werden in den Dialogen Übergangsmatrix und Übergangszeiten hinterlegt.
- **Rüstzeiten**
  geben an, wie viel Zeit benötigt wird, um eine Maschine für den nächsten Arbeitsgang einzurichten. In der Regel werden Rüstzeiten als Zeitzuschlag festgelegt.

In den folgenden Einheiten werden die Konzepte erläutert, mit denen Sie diese Zeitkomponenten einsetzen. Daran anschließend wird anhand der Dialoge in Handlungsabläufen gezeigt, wie Sie die verschiedenen Vorgaben hinterlegen.

> **Stammdaten bearbeiten**
> Wenn Sie im Modul Kapazitätsplanung die Stammdaten - und dabei insbesondere die Zeitvorgaben - bearbeitet haben, sollten Sie die Kapazitätsplanung neu starten.

---
*H-2965 & H-2966*
*A+W Business Pro Kapazitätsplanung*
---

#### Vorgabezeiten

Vorgabezeiten werden für jede einzelne Arbeitsart pro Aggregat angegeben. Diese Zeiten können mit bis zu drei Grenztypen gestaffelt werden.

*Abb. H-30 Vorgabezeiten*
*(Screenshot des Dialogs 'Vorgabezeiten' mit Registern für Zeitstaffelung (A), Priorität (B), Auswahl für Zuschläge (C) und einer Liste der Arbeitsarten (D), Aggregate (E) und Vorgabezeittypen (F).)*

Für alle Tätigkeiten werden die Zeiten pro Maschine und Einheit gestoppt. Ob Sie die Zeiten pro Stück, qm oder Kantenlänge stoppen, hängt von dem zu fertigenden Produkt, der Arbeitsart und der Maschine ab. Je nach definierter Arbeitseinheit wird auch die Anzahl der Werker einbezogen, die an der Maschine arbeiten. Diese Zeiten hinterlegen Sie für jede Maschine und alle die Arbeitsart, die an der Maschine ausgeführt werden.

##### Typ der Vorgabezeit

Die Vorgabezeiten können auf unterschiedliche Weise in die Berechnung einfließen. Dabei unterscheidet A+W Business Pro vier verschiedene Typen (F):
- **Basiszeit:**
  Das ist die gestoppte Vorgabezeit für eine Arbeitsart, z. B. für die Arbeitsart Zuschnitt. Da der Zeitbedarf für einen Arbeitsgang i. a. R. von der Größe abhängig ist, können diese Zeiten mit bis zu drei Grenztypen gestaffelt werden.
- **Zeitzuschlag:**
  Ein Zeitzuschlag wird z. B. für das Zuschneiden von Modellen benötigt. Das bedeutet, dass für das Zuschneiden von Modellen keine eigene Vorgabezeit gemessen wird, sondern die normale Vorgabezeit um einen Zuschlag erhöht wird. Die Zeitzuschläge werden ausführlich in einer separaten Einheit besprochen.
  ⇨ "Arbeitsarten und Zeitzuschläge" auf Seite H-2971
- **Alternativer Vorgang:**
  Diese Vorgabezeit wird nur herangezogen, wenn für die Arbeitsart eine alternative Arbeitsart existiert. In diesem Fall müssen Sie im Feld `altern. Masch.-Nr.` die alternative Maschinennummer eintragen.
- **Alternative ohne Stückliste:**
  Als VSG-Produzent ist Ihr VSG-Artikel standardmäßig mit einer Stückliste hinterlegt. Wenn aber z. B. eine VSG-Scheibe in einzelnen Fällen nicht produziert, sondern direkt aus einer VSG-Platte geschnitten werden soll, dann darf die Stückliste in der Produktion nicht berücksichtigt werden. Für die Arbeitsart VSG schneiden müssen Sie die Option Alternative ohne Stückliste einsetzen. In diesem Fall müssen Sie im Feld `altern. Masch.-Nr.` die alternative Maschinennummer eintragen.
- **Vorgang ignorieren:**
  Bei einem Eckausschnitt fallen z. B. 3 Arbeitsgänge an: 1. Bohren (von Eckloch), 2. Zuschnitt und 3. Schleifen. Die CNC-Maschine kann alle drei Vorgänge als einen Arbeitsgang ausführen, d. h., dass Sie dann nur der Arbeitsart Bohren eine Vorgabezeit zuweisen müssen. Den anderen beiden Arbeitsarten weisen Sie auf dieser Maschine den Wert Vorgang ignorieren zu.

##### Priorität

Wenn mehrere Maschinen für eine Arbeitsart zur Verfügung stehen, müssen Sie festlegen, welche Maschine bei der Suche nach freien Kapazitäten zuerst abgefragt wird.

Wenn zwei Maschinen die gleiche Priorität (B) haben, dann prüft die Kapazitätsplanung die Kosten, die pro Maschine definiert sind. In diesem Fall wird automatisch die günstigere Maschine ausgewählt.

Wenn Sie keine Kosten pro Maschine hinterlegen, muss die Priorität bei gleichen Maschinen eindeutig sein, d. h. unterschiedlich.
- **9:** höchste Priorität (Standard-Maschine). Diese Maschinen werden immer zuerst ausgelastet.
- **8 bis 1:** absteigende Prioritäten. Diese Maschinen werden je nach Auslastung ausgewählt.
- **0:** niedrigste Priorität. Diese Maschinen werden nur dann eingesetzt, wenn alle anderen (gleichwertigen) Maschinen ausgelastet sind.
- **-1:** zur manuellen Einlastung. Diese Maschinen werden von der automatischen Einlastung nur bei Engpässen ausgewählt.
- **-2, -3:** nur zur manuellen Einlastung. Diese Maschinen werden nie von der automatischen Einlastung ausgewählt.

---
*H-2967 & H-2968*
*A+W Business Pro Kapazitätsplanung*
---

##### Grenztypen und Staffelung

Die Zeiten können mit bis zu drei Grenztypen gestaffelt werden:
- **Vektor:**
  Bei einem Vektor erfassen Sie Zeiten in Abhängigkeit von einem Grenztypen, z. B. Meter, Fläche.
- **Matrix:**
  Bei einer Matrix erfassen Sie Zeiten in Abhängigkeit von zwei Grenztypen, z. B. Breite und Höhe. Dabei haben Sie die Möglichkeit, die Matrix in Dreiecksform anzulegen, so dass die Grenztypen austauschbar sind, z. B. Höhe und Breite.
- **Würfel:**
  Der Würfel wird ähnlich wie die Matrix-Zeiten aufgebaut, bietet jedoch drei Grenztypen, z. B. Breite, Höhe und Dicke.

Die Grenztypen und Staffelungen haben Sie bei der Preisdefinition in der Schulung der Stammdaten kennengelernt.
Eine Übersicht über die verfügbaren Grenztypen finden Sie im Part Stammdaten.
⇨ Stammdaten: Tutorial 2, "Verfügbare Grenztypen" auf Seite B-594

**Dreiecksform**
Sie können in einer Matrix oder in einem Würfel Zeiten so erfassen, dass die angegebenen Grenzwerte vertauscht werden dürfen, z. B. Höhe und Breite. Damit müssen Sie nur jeweils eine der Kombinationen erfassen.

**Zeiten in Stunden**
Die Zeiten werden nicht in Minuten sondern in Stunden hinterlegt. Das bedeutet, dass Sie die in Minuten gemessenen Zeiten in Stunden umrechnen müssen.

**Beispiel**
Formel: Gestoppte Minuten / 60 = Zeitwert in Stunden

| Minuten | Eintrag des Zeitwerts (in Stunden) |
| :--- | :--- |
| 60 | 1 |
| 30 | 0,5 |
| 15 | 0,25 |
| 7,5 | 0,125 |
| 3,75 | 0,0625 |
| 1,875 | 0,03125 |

Wenn Sie also für eine Arbeitsart die Zeit 2,5 Minuten gemessen haben, tragen Sie dafür den Zeitwert 0,0417 als Basiswert ein.

---
*H-2969*
*A+W Business Pro Kapazitätsplanung*
---

> **Vorgabezeit kopieren**
> Wenn zwei gleichartige Maschinen die gleiche Zeit benötigen, können Sie mit der Kopierfunktion die Zeiten von einer Maschine auf die andere übertragen und anpassen. Dies ist besonders hilfreich bei gestaffelten Zeiten.

#### Sonderzeiten

Die gemessenen Zeiten können nicht eingehalten werden, wenn z. B. eine besonders große Scheibe in der Produktion mehr Zeit benötigt. Für solche Fälle definieren Sie eine Sonderzeit als Zuschlag, die in der Regel auf die Basisposition aufgeschlagen wird.

Sonderzeiten bieten sich an, wenn Größe, Material oder Dicke der Scheibe eine besondere Herausforderung darstellen.

*Abb. H-31 Dialog Sonderzeiten*
*(Screenshot des Dialogs 'Sonderzeiten' mit einer Tabelle für gestaffelte Zuschläge. A: Nummer der Tabelle, B: Gestaffelter Zuschlag, C: Grenzwert, D: Grenztyp, E: Höhe des Zuschlags, F: Einheit, G: Zuschlagsart.)*

In diesem Beispiel sehen Sie, dass die Zeit der Basisposition um 100 % erhöht wird, wenn die Scheibe besonders klein (kleinste Kantenlänge 300 mm) ist oder wenn sie besonders groß (Breite über 1400 mm, Höhe über 2400 mm) ist. Der Bereich zwischen diesen Maßen wird ohne Zeitzuschlag kalkuliert.

Sonderzeiten werden in der gleichen Weise angelegt wie die Sonstigen Zuschläge der A+W Business Pro-Stammdaten.

---
*H-2970*
*A+W Business Pro Kapazitätsplanung*
---

#### Arbeitsarten und Zeitzuschläge

In der Regel legen Sie für jede Tätigkeit eine eigene Arbeitsart an und hinterlegen für diese dann eine Basiszeit (Vorgabezeit). Wenn Sie Tätigkeiten zu einem Arbeitsgang zusammenfassen können, muss die grundlegende Tätigkeit durch einen Faktor erhöht werden.

**Beispiel**
Die Fertigung einer Einheit 3-fach ISO dauert 2,5-mal so lange wie die Fertigung einer ISO-Einheit mit zwei Scheiben.
An der ISO-Linie geben Sie einen Faktor an, der den Wert der Basiszeit (für das 2-Fach-ISO) entsprechend erhöht.
Dazu finden Sie ausführliche Berechnungsbeispiele unter:
⇨ "Fallbeispiel ISO und Modell" auf Seite H-2972

Auch ein Mehraufwand für Modelle wird als Vorgabezeit vom Typ **Zeitzuschlag** für die jeweilige Arbeitsart hinterlegt.

Für jeden Zeitzuschlag, den Sie definieren wollen, müssen Sie eine Arbeitsart einrichten. Das bedeutet, dass Sie z. B. eine Arbeitsart für den Zuschnitt von Modellen und eine Arbeitsart für die Bearbeitung von Modellen einrichten müssen.

Einfacher ist es jedoch, wenn Sie eine Arbeitsart **Modellzuschläge** einrichten und die Höhe des jeweiligen Zeitzuschlags für diese Arbeitsart bei den Aggregaten definieren, an denen die Arbeitsart ausgeführt wird.

*Abb. H-32 Arbeitsart Modellzuschläge für Zeitzuschläge an unterschiedlichen Maschinen*
*(Diagramm: Die Arbeitsart "Modellzuschläge" löst je nach Maschine (Schneidtisch, Schleifmaschine, ISO-Linie) unterschiedliche Zeitzuschläge (A, B, C) aus.)*

> **Umlasten von Aufträgen bei Engpässen**
> Mit Zeitzuschlägen vereinfachen Sie außerdem die Vorgänge beim Umlasten. Wenn Sie z. B. die Produktion einer (komplexen) ISO-Einheit ohne Zeitzuschläge verschieben müssen, kann das bedeuten, dass Sie alle vorgelagerten Arbeitsgänge einzeln verschieben müssen.

Modelle gehören zur Stammdaten-Produktart `Modelle`. Durch die Zuordnung der Produktart `Modelle` zur Arbeitsart `Modellzuschläge` werden die Modelle beim Einlasten erkannt. Die Zeiten pro Auftragsposition werden dann bei Modellen um den Zuschlag erhöht, der an der jeweiligen Maschine hinterlegt ist. Diese Zuordnungen werden Sie im nächsten Themenblock kennenlernen.
⇨ "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-3012

---
*H-2971*
*A+W Business Pro Kapazitätsplanung*
---

#### Fallbeispiel ISO und Modell

Mit einem Fallbeispiel für die Produktion von ISO-Einheiten wird im Folgenden gezeigt, in welcher Reihenfolge Zeitzuschläge eingerichtet werden und wie beim Einlasten die benötigte Zeit berechnet wird.

Die Fertigung von ISO-Einheiten mit drei und mehr Scheiben und als Modell erfordert viele Zeitvorgaben. Ein mögliches Konzept soll in diesem Beispiel vorgestellt werden. Dabei wird angestrebt, die Vorgaben so einzurichten, dass sie zur Berechnung von ISO-Scheiben und Modellen angewendet werden können und der Aufwand zum Einrichten und zur Pflege der Daten verringert wird.

*Abb. H-33 Definition der Vorgaben für Beispiel ISO-Fertigung*
*(Diagramm: Für das Aggregat 'ISO-Linie' wird eine Vorgabezeit (Basiszeit 0,018 Std.) für die Arbeitsart 'ISO Fertigen' definiert. Über Zuordnungen wird diese Zeit für '3-fach-ISO' mit Faktor 2,5 multipliziert und für 'Modellzuschläge' um 50% erhöht.)*

**Vorgaben**
Im Folgenden werden die Vorgaben gezeigt, die in den verschiedenen Dialogen hinterlegt werden müssen. Genauere Handlungsanleitungen finden Sie im Anschluss an das Beispiel. Das Beispiel geht von folgenden Vorgaben aus:
- Die Tageskapazität von 450 ISO-Einheiten ergibt:
  8 Std. / 450 Einheiten = 0,018 Std. pro Einheit.
- Für die ISO-Linie ist daher eine Vorgabezeit als Einzelzeit vom Typ Basiszeit hinterlegt.
  *Abb. H-34 Dialog Vorgabezeit - Einzelzeit für ISO-Einheit*
- Für Modellzuschläge und 3-Fach-ISO sind gleichnamige Arbeitsarten angelegt.
  *Abb. H-35 Arbeitsarten für Modelle und 3-fach-ISO*
- Die Produktart `Modelle` ist der Arbeitsart `Modellzuschläge` zugeordnet.
  *Abb. H-36 Zuordnung der Produktart zur Arbeitsart Modellzuschläge*
- Als Vorgabezeit für die Arbeitsart `Modellzuschläge` wird ein Zeitzuschlag von 50 % am Aggregat ISO-Linie berechnet.
  *Abb. H-37 Dialog Vorgabezeit - Zeitzuschlag für Modelle*
- 3-fach ISOs sind in der Produktgruppe `Dreifach ISO` zusammengefasst.
- Der Produktgruppe `Dreifach ISO` wird die Arbeitsart `ISO Fertigen` zugeordnet.
- Für 3-fach ISO soll der Faktor 2,5 berechnet werden.
  *Abb. H-38 Zuordnungen Dialog Produktgruppe – Faktor für 3-fach ISO*
- Außerdem soll ein Zuschlag für Übergrößen berechnet werden. Dieser ist als Sonderzuschlag angelegt.
  *Abb. H-39 Dialog Sonderzeit - Sonderzuschlag für große und kleine Scheiben*

**Faktoren und Zuschläge bei der Berechnung**
Faktoren werden mit der Basiszeit des Arbeitsgangs multipliziert. Der Faktor 1 bedeutet, dass die Zeit nicht erhöht wird. Der Faktor 0,5 bedeutet, dass die Zeit um die Hälfte reduziert wird.
Sonstige Zuschläge werden als prozentuale Zuschläge addiert. Die Basiszeit + 100% ergibt also eine Verdoppelung der Zeit. Diese Zuschläge sind als Sonderzeiten über Zuschlagstabellen angelegt und werden der Vorgabezeit zugeordnet.
Im Einlastungsergebnis werden nur Zeiten für die Arbeitsarten angezeigt für die eine Basiszeit hinterlegt ist. Alle Zeitzuschläge, die auf Basiszeiten aufgeschlagen werden, sind in diesen Ergebnissen enthalten und werden nicht ausgewiesen.

---
*H-2972 to H-2975*
*A+W Business Pro Kapazitätsplanung*
---

#### Berechnungsreihenfolge für Zuschläge und Faktoren

| Position | Berechnung | Zeit (Std.) |
| :--- | :--- | :--- |
| ISO | Zeit | 0,018 |
| ISO + Modell | 0,018<br>+ Zeitzuschlag 50 % | 0,018<br>+ 0,009<br>= 0,027 |
| ISO + Übergröße | 0,018<br>+ Sonderzuschlag 100 % | 0,018<br>+ 0,018<br>= 0,036 |
| ISO + Modell + Übergröße| 0,018<br>+ Zeitzuschlag 50 %<br>= 0,027<br>+ Sonderzuschlag 100 % | 0,018<br>+ 0,009<br>= 0,027<br>+ 0,027<br>= 0,054 |
| 3-fach ISO | 0,018 x Faktor 2,5 | 0,018 x 2,5<br>= 0,045 |
| 3-fach ISO + Modell | 0,018 x Faktor 2,5<br>+ Zeitzuschlag 50 % | 0,0450<br>+ 0,0225<br>= 0,0675 |
| 3-fach ISO + Übergröße | 0,018 x Faktor 2,5<br>+ Sonderzuschlag 100 % | 0,045<br>+ 0,045<br>= 0,090 |
| 3-fach ISO + Modell + Übergröße | 0,018 x Faktor 2,5<br>+ Zeitzuschlag 50 %<br>= 0,0675<br>+ Sonderzuschlag 100 % | 0,0450<br>+ 0,0225<br>= 0,0675<br>+ 0,0675<br>= 0,1350 |

Aus diesen Beispielen sehen Sie, in welcher Reihenfolge Faktoren, Zuschläge und Sonderzuschläge in die Berechnung einfließen.

---
*H-2976*
*A+W Business Pro Kapazitätsplanung*
---

#### Übergangsmatrix und Übergangszeiten

Neben der Zeit für den Arbeitsgang benötigen die Einheiten zusätzlich Zeit, um von einem Produktionsbereich zum nächsten zu gelangen.
Diese Zeiten werden als Verweil- und Übergangszeiten in folgenden Dialogen hinterlegt:
- **Produktionsbereich:**
  Welche Zeit bleibt eine Einheit in einem Produktionsbereich? Die Dauer wird in Tagen oder Bruchteilen von Tagen angegeben. Bei dieser Angabe wird der nachfolgende Produktionsbereich nicht berücksichtigt.
  ⇨ Softwarereferenz, "Produktionsbereich" auf Seite H-3115
- **Übergangszeiten:**
  Welche Zeit benötigt eine Einheit, um von einer Arbeitsart zur nächsten oder von einem Produktionsbereich in den Folge-Bereich zu kommen? Die Dauer wird in Schichten angegeben.
  ⇨ Softwarereferenz, “Übergangszeiten" auf Seite H-3112
- **Übergangsmatrix:**
  Welche Zeit benötigt eine Einheit, um von einem Produktionsbereich in den nächsten Produktionsbereich zu gelangen? Die Dauer wird in Tagen oder Bruchteilen von Tagen angegeben.
  ⇨ Softwarereferenz, “Übergangsmatrix” auf Seite H-3134

Wenn zur Zeitkalkulation für eine Auftragsposition in allen drei Dialogen Werte gefunden werden, berücksichtigt das Programm jeweils den größeren Wert. Zusätzlich wird die Anzahl der Schichten berücksichtigt, in denen die einzelnen Bereiche arbeiten.
Schichten und Tage können auch in Werten <1 eingegeben werden. Wie groß die Zeit dann letztlich ist, hängt von den Schichten und den Zeiten des Arbeitstags ab, die im Kalender definiert sind.

**Beispiel**
Wenn für die Übergangzeit der Wert 0,1 (Schichten) eingetragen ist, liegt genau eine Schicht zwischen den Arbeitsgängen.
⇨ Softwarereferenz, “Beispiele für die Berechnung des Übergangs" auf Seite H-3135

> **Auftragspriorität berücksichtigen**
> Wenn außer der Auftragspriorität `Normal` auch z. B. die Priorität `Eilt` berücksichtigt werden soll, dann müssen dafür eigene Werte für die Übergangsmatrix und Übergangszeiten eingerichtet sein. Dies gilt für alle Zeiten, die für Eilaufträge auch verkürzt werden können.

**Zusammenwirken von Verweil- und Übergangszeiten**

*Abb. H-40 Beispiel 1: Verweiltage im Bereich + Übergangsmatrix*
- **Vorgaben:** Heat-Soak hat 0,2 Tage Verweildauer. Übergang von Heat-Soak zu Versand ist 1 Tag.
- **Planung:** Nach Zuschnitt (Do, S1) verbleibt die Position einen Tag (größerer Wert) im Heat-Soak, bevor sie am Freitag (S1) in den Versand geht.

*Abb. H-41 Beispiel 2: Verweiltage im Bereich + Übergangsmatrix*
- **Vorgaben:** (wie oben)
- **Planung:** Nach Zuschnitt (Do, S3) ist die Position am Freitag (S1) im Heat-Soak und am Freitag (S3) im Versand.

*Abb. H-42 Beispiel 3: Verweiltage im Bereich + Übergangszeit*
- **Vorgaben:** Übergang von Heat-Soak zur Folge-Arbeitsart ISO ist 3 Schichten.
- **Planung:** Nach Zuschnitt (Do, S1) könnte das ESG am Donnerstag (S3) in den Folge-Bereich kommen, aber erst am Freitag (S2) in das ISO eingebaut werden.

*Abb. H-43 Beispiel 4: Verweiltage im Bereich + Übergangszeit*
- **Vorgaben:** (wie oben)
- **Planung:** Bei einem Zuschnitt am Donnerstag (S3) würde das ESG erst am Montag (S1) in das ISO eingebaut werden.
Weitere Berechnungsbeispiele finden Sie unter:
⇨ "Terminberechnung" auf Seite H-3024

**Formel für Übergangszeit**
Wenn z. B. 50 Scheiben vom Zuschnitt zum Nassbereich kommen müssen, wird die Zeit in Tagen oder Schichten nur unzureichend genau berechnet. Für diese Fälle kann eine Formel hinterlegt werden, die die Anzahl der Scheiben berücksichtigt.

*Abb. H-44 Übergangsmatrix und Formel*
*(Screenshot zeigt die Übergangsmatrix, in der für den Übergang von ESG-Fertigung zu Versand eine Formel F(500) eingetragen ist. Die Formel (B) selbst setzt das Ergebnis auf 1 (Tag) und ab 11 Stück auf 3 (Tage).)*

Um die Formel im Dialog Übergangsmatrix auszuwählen, setzen Sie den Cursor in das Feld Übergangszeit und drücken die rechte Maustaste.
Die Formel selbst wird über **A+W Business Pro-Stammdaten > Firma > Formeln** angelegt. Im Dialog **Formelverwaltung > Register Formel** kann die Formel eingetragen und bearbeitet werden.
Falls Sie Formeln einsetzen wollen, wenden Sie sich an Ihren Service-Mitarbeiter bei der A+W Software GmbH.

---
*H-2977 to H-2982*
*A+W Business Pro Kapazitätsplanung*
---

#### Rüstzeiten

Rüstzeiten werden als Arbeitsart definiert und dem Aggregat und der Bearbeitung zugeordnet. Folgende Schritte sind dazu notwendig:
- Arbeitsart `Rüstzeit` anlegen.
- Arbeitsart `Rüstzeit` dem Aggregat als Typ `Basiszeit` zuordnen, z. B. der CNC-Maschine.
- Einzelzeit mit der Einheit `Stk` (einmal) festlegen, denn die Maschine wird pro Arbeitsgang nur einmal eingerichtet.
- Arbeitsart den Produktgruppen zuordnen, die auf dem Aggregat gefertigt werden, z. B. Produktgruppe `Bearbeitungen/Eckausschnitte` an der CNC-Maschine.
- Fertigungsstraße definieren, um die Rüstzeit für aufeinanderfolgende Bearbeitungen nicht doppelt zu berechnen.

*Abb. H-45 Arbeitsart Rüstzeit für Folge-Aggregat sperren*
*(Screenshot des Dialogs 'Fertigungsstraße definieren'. Zeigt an, dass für Aggregat 3100-CNC die Arbeitsart Rüstzeit gesperrt wird, wenn das Folge-Aggregat ebenfalls 3100-CNC ist.)*

In diesem Beispiel sehen Sie, dass die Rüstzeit für das Aggregat CNC-Maschine übersprungen wird, wenn das Folge-Aggregat wieder die CNC-Maschine ist. Die Maschine wird dann einmal für alle aufeinander folgenden Bearbeitungen eingerichtet.
Wenn die CNC-Maschine für die nachfolgende Bearbeitung aber neu eingerichtet werden muss, müssen die Rüstzeiten gesondert angelegt und berechnet werden. Sie können dann durch die Definition einer Fertigungsstraße gesperrt werden.

#### Zeitfaktoren für Serien

Für Serien kann der normale Zeitbedarf durchaus sinken, da z. B. Rüstzeiten entfallen. Die Maschine steht also früher wieder zur Verfügung und kann für den nächsten Auftrag eingeplant werden.
Für diese Zeitkalkulation legen Sie Serientabellen mit den Faktoren für die Serienfertigung an.

*Abb. H-46 Serienfaktoren*
*(Screenshot des Dialogs 'Serienfaktoren'. A: Gestaffelte Stückzahlen. B: Zeitfaktor pro Staffelung. Eine Tabelle 'Serien/Series 1' wird gezeigt.)*

In diesem Beispiel sehen Sie einen gestaffelten Abschlag für die Berechnung des Zeitbedarfs. Wie hoch die Reduktion tatsächlich ist, hängt von der Vorgabezeit ab, die für den jeweiligen Arbeitsgang angegeben ist.

Serientabellen werden unabhängig von einer bestimmten Maschine oder einer Arbeitsart angelegt. Wenn Sie für die Fertigung mit bestimmten Arbeitsarten unterschiedliche Abschläge einsetzen wollen, müssen Sie also mehrere Tabellen für Serien anlegen. Verwenden Sie dann für die Bezeichnung einen Begriff, aus dem deutlich wird, wofür die Tabelle eingesetzt werden soll, z. B. `Bohren Serie`.

Damit die Serienfaktoren berücksichtigt werden, müssen Sie im Dialog **Aggregat** und im Dialog **Besondere technische Restriktionen** angeben, welche Serientabelle gelten soll.

---
*H-2983 & H-2984*
*A+W Business Pro Kapazitätsplanung*
---

#### Vorgabezeiten festlegen

Bevor Sie Vorgabezeiten eintragen, sollten Sie sich einen Plan erstellen, in dem folgende Fragen geklärt sind:
- Welche Arbeitsarten kann jede Ihren Maschinen ausführen. Welche Arbeitsart kann die neue Maschine ausführen.
- In welcher Einheit soll die Zeit eintragen werden, z. B. pro Meter, pro Kante, pro Fläche.
- Soll die gestoppte Zeit eingetragen werden (Basiszeit) oder ein Zeitzuschlag.
- Soll die Zeit als Einzelzeit oder mit einer Staffelung eingetragen werden.
- Nach welchen Grenztypen und welchen Grenzwerten soll die Zeit gestaffelt werden.

> **Tipp**
> Wenn Sie zuvor die Vorgabezeit für ein gleichartiges Aggregat oder eine gleichwertige Arbeitsart auswählen, können Sie die Daten als Vorbelegung übernehmen und bearbeiten.
> In den folgenden Handlungssequenzen wird die Zeit vollständig neu angelegt.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
- "So legen Sie die Grunddaten der Vorgabezeit fest" auf Seite H-2985
- "So legen Sie die Zeiten für eine Arbeitsart fest" auf Seite H-2987

**So legen Sie die Grunddaten der Vorgabezeit fest**

1.  Wählen Sie im Modul **Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten**.

    *Abb. H-47 Vorgabezeit für Arbeitsart anlegen*

2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.

    *Abb. H-48 Vorgabezeit anlegen: Grunddaten eintragen*
    *(A: Arbeitsart und Aggregat auswählen. B: Typ der Vorgabezeit. C: Priorität.)*
    Die Felder werden freigeschaltet. Sie sind mit den Daten des ersten Aggregats vorbelegt.

3.  Wählen Sie zuerst die Arbeitsart und dann das Aggregat (A) aus.
    Wenn ein Aggregat mehr als eine Arbeitsart ausführen kann, müssen Sie die gesamte Handlungssequenz für jede Arbeitsart wiederholen und die entsprechenden Zeiten festlegen.
    Alternativ dazu können Sie eine neue Arbeitsart anlegen, die alle Tätigkeiten umfasst, die das Aggregat ausführen kann. Die Vorgabezeit gilt dann für den gesamten Ablauf der Tätigkeiten.

4.  Wählen Sie den Typ (B) der Vorgabezeit.
    In diesem Beispiel wird `Basiszeit` gewählt. Die Handlungsschritte für Zeitzuschläge unterscheiden sich nicht von denen für Arbeitsgänge.

5.  Legen Sie die Priorität (C) fest.
    Die Priorität steuert die Auswahl des Aggregats, je nach der Arbeitsart, die für die Fertigung der Auftragsposition erforderlich ist.

6.  Legen Sie das Format der Vorgabezeit fest, indem Sie zu dem entsprechenden Register wechseln.
    Damit haben Sie die Grunddaten festgelegt. Sie müssen jetzt die Zeiten eintragen.

**So legen Sie die Zeiten für eine Arbeitsart fest**

1.  Wechseln Sie zum Register **Matrix**.
    Staffelungen und Zeiten werden in den Registern **Vektor** und **Würfel** auf die gleiche Art eingetragen.

    *Abb. H-49 Grenzwerte für Vorgabezeiten*
    *(A: Grenzwert 1, Grenzwert 2. B: Grenztyp 1, Grenztyp 2. C: Zeilenkopf. D: Spaltenkopf.)*
    Die Grenztypen und die Einheit sind vorbelegt. Sie müssen diese ändern.

2.  Wählen Sie die Grenztypen (B) 1 und 2 aus, z. B. Dicke und qm Rechteck.
    Als nächstes müssen Sie die Grenzwerte für die Staffelung festlegen.

3.  Öffnen Sie das Kontextmenü (rechte Maustaste) zum Spaltenkopf (D).

4.  Wählen Sie im Kontext-Menü den Eintrag **Einfügen**. Das Feld für den Grenzwert (A) wird freigeschaltet.

5.  Tragen Sie den ersten Grenzwert ein, z. B. 4,00 für die Dicke, und springen Sie mit der `<Tab>`-Taste in das nächste Feld. Die neue Spalte wird eingefügt.

6.  Wiederholen Sie die Schritte 3 bis 5, bis Sie die gesamte Staffelung für den Grenztyp 1 angelegt haben.

7.  Öffnen Sie das Kontextmenü (rechte Maustaste) zum Zeilenkopf (C) und wiederholen Sie die Schritte 4 und 5 für den Grenztyp 2.

8.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Daten werden gespeichert.

9.  Tragen Sie jetzt in jede Zelle der Zeittabelle den entsprechenden Wert ein.

    *Abb. Vorgabezeiten Matrix*

10. Prüfen Sie im Feld **Zeiteinheit**, ob der Eintrag richtig gewählt ist.
    In diesem Beispiel wird die Einheit `qm` gewählt. Das bedeutet, dass die eingetragenen Zeiten sich auf die Fläche beziehen, also z. B. 0,013 Std. pro qm.

11. Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert. Die neuen Daten werden im Register **Zeitauswahl** in der Übersicht aufgeführt.

    *Abb. H-50 Neue Vorgabezeiten angelegt*

Wenn Sie die Staffelung in Würfelform anlegen wollen, lesen Sie die entsprechende Anleitung für Preise im Part Stammdaten.

---
*H-2985 to H-2989*
*A+W Business Pro Kapazitätsplanung*
---

#### Sonderzeit anlegen

Sonderzeiten legen Sie als Zuschläge an, um Besonderheiten berechnen zu können, z. B. ein Zuschlag für Übergrößen. Sie können pro Datensatz zwei Grenztypen berücksichtigen, wobei die Grenztypen zwischen den Datensätzen einer Zuschlagstabelle wechseln können.
In den folgenden Beispielen wird die Tabelle für Größenzuschläge kopiert und angepasst.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
- "So legen Sie eine neue Zuschlagstabelle an" auf Seite H-2990
- "So legen Sie weitere Stufen zur Staffelung des Zuschlags an" auf Seite H-2991

**So legen Sie eine neue Zuschlagstabelle an**

1.  Wählen Sie im Modul **Kapazitätsplanung > Stammdaten > Vorgabezeiten > Sonderzeiten**.

    *Abb. H-51 Sonderzuschlag anlegen*

    Eine Beschreibung des Dialogs finden Sie in der Softwarereferenz.
    ⇨ Softwarereferenz, "Sonderzeiten" auf Seite H-3150
    Wenn bereits Tabellen angelegt sind, können Sie einen Eintrag markieren. Die Zuschlagswerte werden dann in die neue Tabelle übernommen.

2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.

    *Abb. H-52 Neue Tabelle anlegen*
    *(A: Frei wählbare Nummer. B: Name.)*
    Die Felder werden freigeschaltet. Sie sind mit den Werten der markierten Tabelle vorbelegt.

3.  Tragen Sie die Nummer (A) und die Bezeichnung (B) der neuen Tabelle ein. Überschreiben Sie dazu die Einträge in den beiden Feldern.

4.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Daten werden gespeichert.

5.  Tragen Sie den Wert für den neuen Zuschlag ein. Sie können die vorhandenen Grenztypen und Zuschlagswerte überschreiben oder durch weitere Werte ergänzen.

In diesem Beispiel basiert die neue Tabelle auf der Größentabelle. Sie soll jetzt angepasst werden für die Kantenbearbeitung. In der folgenden Handlungssequenz werden daher die Grenztypen und die Stufung geändert.

**So legen Sie weitere Stufen zur Staffelung des Zuschlags an**

1.  Lassen Sie sich den Zuschlag anzeigen, den Sie bearbeiten wollen.

    *Abb. H-53 Gestaffelter Sonderzuschlag*
    *(A: Grenzwert 1, 2. B: Grenztyp 1, 2. C: Wert. D: Einheit. E: Berechnungsbasis.)*

2.  Ändern Sie in der ersten Zeile Grenztyp 1 (B), z. B. in `Dicke` und Grenztyp 2, z. B. in `Größte Kantenlänge`.

3.  Passen Sie die Grenzwerte (A) entsprechend an.

    *Abb. H-54 Zuschlag bearbeiten*
    *(A: Zeilenkopf. B: Höhe des Zuschlags.)*
    In diesem Beispiel wird also für die Glasdicke bis 5 mm und die Kantenlänge bis 1200 mm kein Zuschlag erhoben. Bei gleicher Dicke wird für die Kantenlängen zwischen 1201 mm bis 1800 mm ein Zuschlag von 50 % (B) berechnet.
    Die nächsten Stufen sollen sich auf die gleichen Kantenlängen auf die Dicke 6 mm beziehen.

4.  Überschreiben Sie die letzte Zeile mit den erforderlichen Werten für die Grenztypen, die Grenzwerte und den Zuschlag. Für die nächste Stufe muss eine neue Zeile eingefügt werden.

5.  Klicken Sie doppelt in den Zeilenkopf (A) der letzten Stufe. Das Kontext-Menü wird angezeigt.

6.  Wählen Sie den Eintrag **Einfügen**. Eine neue Zeile wird eingefügt. Die Grenztypen und Zuschlagseinheit sind mit den Einträgen aus der vorigen Zeile vorbelegt.

    *Abb. H-55 Neuen Grenzwert ergänzen*

7.  Ergänzen Sie den neuen Grenzwert im ersten Feld und passen Sie ggf. die Einträge in den übrigen Feldern an.

8.  Legen Sie auf diese Weise die gewünschten Zuschlagsstufen an.

9.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Daten werden gespeichert.

> **Einträge löschen**
> Um einen Eintrag zu löschen, wählen Sie den entsprechenden Befehl im Kontextmenü. Wenn Sie den Befehl aus dem Menü **Start > Löschen** wählen, wird die gesamte Tabelle gelöscht.

---
*H-2990 to H-2993*
*A+W Business Pro Kapazitätsplanung*
---

### Übungen
- Legen Sie zu Ihrem Übungsaggregat die Vorgabezeiten fest.
- Legen Sie einen Zuschlag für Sprossen mit dem Faktor 1,5 an.
- Legen Sie eine Sonderzeit für den Zuschnitt von Drahtglas an. Beachten Sie dabei 2 Grenzwerte.
- Legen Sie einen Zeitzuschlag für 3-fach-ISO an.
- Legen Sie einen Zeitzuschlag für Rüstzeit an, der bei Serien nur einmal berechnet wird.

#### Ergänzende Informationen
⇨ Softwarereferenz, "Serienfaktoren" auf Seite H-3111
⇨ Softwarereferenz, “Übergangszeiten" auf Seite H-3112
⇨ Softwarereferenz, "Übergangsmatrix" auf Seite H-3134
⇨ Softwarereferenz, "Vorgabezeiten (Dialog)" auf Seite H-3141
⇨ Softwarereferenz, "Sonderzeiten" auf Seite H-3150

---
*H-2994*
*A+W Business Pro Kapazitätsplanung*
---

### Auswahl der Aggregate

**Lernziele**
- Einschränkungen und Prioritäten der Aggregate so einsetzen, dass der Produktionsfluss gewährleistet ist.
- Einstellungen in den Firmendaten prüfen.

**Nutzen**
- Die Aggregate werden beim automatischen Einlasten eines Auftrags geprüft und danach ausgewählt, ob sie technisch und zeitlich in der Lage sind, die erforderlichen Aufgaben auszuführen.

**Merke**

| Begriff | Definition |
| :--- | :--- |
| **Technische Restriktionen** | Einschränkungen zur automatischen Auswahl eines Aggregats werden im Dialog `Aggregate` und im Dialog `Besondere technische Restriktionen` festgelegt. |
| **Automatisch Einlasten** | Beim automatischen Einlasten von Aufträgen in die Kapazitätsplanung werden die Vorgaben zu Prioritäten und Restriktionen ausgewertet und danach nach einer passenden freien Maschine gesucht. |
| **Auslastung** | Die mögliche Auslastung eines Aggregats richtet sich nach der Kapazität des Aggregats und den Einstellungen in den Firmendaten. Für die manuelle Einlastung und das Aufarbeiten von Resten aus dem Vortag sollte daher ein Spielraum gelassen werden. |
| **Manuelle Einlastung** | Ein Auftrag kann manuell eingelastet werden, wenn die Vorgaben für die Auslastung dies zulassen. |
| **Voreinstellungen** | Firmendaten: Register Kapa-Planung |

---
*H-2995*
*A+W Business Pro Kapazitätsplanung*
---

#### Prioritäten

Bei gleichartigen Aggregaten für eine Arbeitsart, z. B. Bohren, hängt die Auswahl durch die Kapazitätsplanung von der Priorität ab, die pro Maschine und Arbeitsart angegeben ist. Bei zwei Maschinen für die gleiche Arbeitsart, die beide die gleiche Priorität haben, entscheidet sich das System für die schnellere und günstigere Maschine.

Über die Prioritäten können Sie außerdem steuern, dass spezielle Aggregate, z. B. der Handzuschnitt, von der automatischen Maschinenzuordnung ausgenommen werden.

Die Prioritäten werden im Dialog **Vorgabezeiten** angegeben.

> **Prioritäten bei gleichwertigen Maschinen**
> Es ist möglich, gleichwertigen Maschinen dieselbe Priorität zu geben, wenn Sie z. B. mit zwei Bistronic-Schneidtischen arbeiten. Wenn diese Maschinen unterschiedlichen AV-Bereichen oder Mandanten zugeordnet sind, ist die Auswahl dennoch eindeutig. Bei gleichwertigen Maschinen, deren Auswahl nicht durch andere Kriterien eingeschränkt ist, sollten die Prioritäten jedoch unterschiedlich vergeben werden.

##### Abweichende Prioritäten
Eine weitere Möglichkeit zum Steuern der Auswahl haben Sie mit abweichenden Prioritäten, die im Dialog **Besondere Prioritäten** angegeben werden.

*Abb. H-56 Besondere Priorität (Beispiel 5, gestrichelte Linie = 40 Stk.)*
*(Diagramm: Ein Auftrag mit 40 Stück wird an Bohrmaschine II (Prio -2) geleitet, weil unter "Besondere Prioritäten" festgelegt ist, dass ab 11 Stück die Priorität auf 9 geändert wird, während Bohrmaschine I (Prio 9) nur bis 10 Stück verarbeitet.)*

In diesem Beispiel sehen Sie, dass die Bohrmaschine II die Priorität -2 hat. Das bedeutet, dass sie nur manuell ausgewählt werden kann. Im Dialog **Besondere Prioritäten** ist jedoch angegeben, dass sie bei Stückzahlen ab 11 die Priorität 9 hat. Damit haben Sie erreicht, dass diese Maschine nur für große Stückzahlen eingesetzt wird. Sie wird auch dann nicht automatisch ausgewählt, wenn die Bohrmaschine I ausgelastet ist.

---
*H-2996*
*A+W Business Pro Kapazitätsplanung*
---

#### Restriktionen

Eine Restriktion stellt eine Einschränkung für die Auswahl der Maschine dar. Diese Einschränkung kann z. B. mit den Maßen, der Glasstärke, der Geschwindigkeit zusammenhängen. Eine Restriktion liegt z. B. vor, wenn eine Bohrmaschine nur bis zu einer Glasstärke von 12 mm eingesetzt werden kann. Wenn das Rüsten einer Maschine sehr aufwendig ist, wird der Einsatz der Maschine von der Stückzahl abhängig gemacht. Maschinen können durch Restriktionen auch für bestimmte Arbeitsarten gesperrt werden.

Diese einfachen Restriktionen werden beim Anlegen der Maschinendaten angegeben. Komplizierte Restriktionen können nur über Sperrformeln angegeben werden.

**Beispiel**
Auf der Schleifmaschine B sollen nur Modelle, sehr kleine und sehr große Scheiben gefertigt werden, da diese Maschine sehr langsam ist.
Alle Rechteckscheiben mit einer Breite >200 und <2600 mm sowie einer Höhe >300 und <1600 mm sollen nicht auf dieser Maschine geschliffen werden.
Diese Restriktion kann nur über eine Formel angegeben werden.

In diesem Fall geben Sie in den Minimal- und Maximal-Werten für die Maschine an, bis zu welchen Maßen das Schleifen technisch möglich ist, z. B. für die Breite 40 bis 3210 mm und für die Höhe 100 bis 6000 mm.
Der Bereich dazwischen (Breite >200 und <2600 mm, Höhe >300 und <3600 mm) wird durch eine Formel gesperrt.

Das Ergebnis für dieses Beispiel könnte zusammengefasst wie folgt aussehen:

*Abb. H-57 Technische Restriktionen und Sperrformel*
*(A: Screenshot der technisch möglichen Werte für ein Aggregat. B: Auswahl der Sperrformel im Sperren-Bereich. C: Auszug aus dem Inhalt einer Sperrformel, die Rechtecke innerhalb bestimmter Maße ausschließt.)*

In den Stammdaten des Aggregats sind im Register **Allgemein** die Werte für Breite und Höhe (A) so angegeben, wie das Aggregat arbeiten kann, also der gesamte Bereich. Im Bereich **Sperre** wird die Nummer der Sperrformel (B) hinterlegt.
Die Sperrformel selbst wird über **A+W Business Pro-Stammdaten > Firma > Formeln** angelegt. Im Dialog **Formelverwaltung > Register Formel** (C) kann die Formel eingetragen und bearbeitet werden.
Falls Sie Formeln einsetzen wollen, wenden Sie sich an Ihren Service-Mitarbeiter bei der A+W Software GmbH.

#### Priorität vs. Restriktion
Die Möglichkeiten, die automatische Auswahl der Maschinen zu steuern, wirken zusammen. Das ist schon im Beispiel mit der Restriktionsformel deutlich geworden. Aber auch ohne Formeln können Sie die Auswahl sehr genau steuern:
- Eine Maschine mit der Priorität 9 und der Restriktion Stückzahl >10 wird immer erst ausgewählt, wenn in der Position mindestens 11 Stück angegeben sind. Liegt die Stückzahl unter oder gleich 10, so wird die Maschine mit der nächstniedrigeren Priorität ausgewählt.
- Wenn eine Maschine mit der Priorität 9 keine großen Scheiben bearbeiten kann, wird sie nur für Positionen mit Standard-Maßen ausgewählt.

Sie können solche Kombinationen im Dialog **Besondere Prioritäten** hinterlegen.

*Abb. H-58 Besondere Prioritäten*
*(Screenshot des Dialogs 'Bes. Prioritäten', der zeigt, wie für die Arbeitsart 'Bohrungen / Drillings' und das Aggregat 'CNC-Maschine' die Priorität auf 9 gesetzt wird, wenn die Stückzahl größer 10 ist.)*

In diesem Beispiel sehen Sie, dass die CNC-Maschine bei einer Stückzahl über 10 mit der Priorität 9 bei Bohrungen eingesetzt werden soll. Standardmäßig hat diese Maschine für die Arbeitsart `Bohren` nur die Priorität 4.

Wenn beim Einlasten eines Auftrags eine Restriktion verletzt wird, wird die Maschine nicht für diesen Auftrag eingesetzt. Sie kann dann auch nicht manuell ausgewählt werden, da sie nicht zur Auswahl angeboten wird.

> **Verfügbare Felder für Prüfwerte (Sperrwerte)**
> Die Eingabefelder für Prüfwerte müssen bei den Aggregattypen freigeschaltet werden. Wenn Sie Prüfungen nachträglich aktivieren, müssen Sie alle Aggregate prüfen, die zu dem geänderten Aggregattyp gehören. Prüffelder ohne Werte verhindern beim Einlasten die Auswahl des Aggregats – auch dann, wenn es geeignet wäre, die Position zu fertigen.
> ⇨ Softwarereferenz, "Aggregattypen" auf Seite H-3104

---
*H-2997 to H-2999*
*A+W Business Pro Kapazitätsplanung*
---

#### Automatische Einlastung

Bei der automatischen Einlastung werden die Aggregate (Maschinen) ausgewählt, die der jeweiligen Arbeitsart zugeordnet sind. Sie haben die Möglichkeit, einer Arbeitsart, z. B. dem Bohren, mehrere Bohrmaschinen zuzuordnen. Aus der Kombination von Arbeitsart und Aggregat ergeben sich der zeitliche Aufwand (reservierte Kapazität) und die Kosten. Die automatische Auswahl der Bohrmaschine wird u. a. anhand der freien Kapazitäten, der technischen Restriktionen und der Kosten entschieden.

Die Auswahl eines Aggregats kann daher über folgende Einstellungen gesteuert werden:
- Priorität des Aggregats (9 bis -2)
- Arbeitsart
- Sperren der Maschine, z. B. für bestimmte Produktarten
- Restriktionen, die sich auf die Anforderungen aus der Auftragsposition beziehen, z. B. die Maße, Stückzahl.

In den folgenden beiden Grafiken wird gezeigt, wie diese Einstellungen zusammenwirken. Prioritäten und Restriktionen sind anschließend in separaten Einheiten ausführlich beschrieben.

*Abb. H-59 Priorität und Technische Restriktionen (Beispiel 1, gestrichelte Linie = 40 Stk.)*
*(Diagramm zeigt, dass ein Auftrag mit 40 Stück wegen einer Restriktion (bis 10 Stück) von der Bohrmaschine I (Prio. 9) abgelehnt und an die Bohrmaschine II (Prio. 8) weitergeleitet wird.)*

Im eingelasteten Auftrag wird zunächst geprüft, welche Arbeitsart ausgeführt werden soll. Anhand der Arbeitsart werden die möglichen Maschinen ermittelt und geprüft, welche Restriktionen jeweils vorliegen. Maschinen, die für die Fertigung nicht geeignet sind, werden nach dieser Prüfung nicht mehr zur Auswahl angeboten. Sie stehen dann auch nicht zur manuellen Auswahl zur Verfügung.

In Beispiel 1 sehen Sie, dass die Standard-Maschine mit der Priorität 9 (Bohrmaschine I) nur für die erste Position angesteuert wird. Bei der Prüfung der Restriktionen wird erkannt, dass die 40 Stk. der zweiten Auftragsposition nicht auf Bohrmaschine I gefertigt werden dürfen. Die Bohrmaschine II wird gewählt. Wenn es eine Bohrmaschine III mit derselben Priorität gibt, die ebenfalls die technischen Restriktionen erfüllt, entscheidet das System nach den Kosten, welche Maschine ausgewählt wird.

---
*H-3000*
*A+W Business Pro Kapazitätsplanung*
---