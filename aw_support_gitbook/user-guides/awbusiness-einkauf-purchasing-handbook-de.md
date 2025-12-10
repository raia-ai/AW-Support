---
description: "D-HB-AWBusiness_21"
---


# Teil C: A+W Business Verkauf

---
## Auswertungen

### Kostenlose Positionen

Hier werden kostenlose Positionen ausgewertet.

-   **Kunden-Nr.:** Kundennummer aus dem Auftragskopf.
-   **Kunde:** Name des Kunden.
-   **Produkt-Nr.:** Produktnummer aus der Position.
-   **Produkt-Bezeichnung:** Produktbezeichnung aus der Position.
-   **Produziert/Gekauft:** Kennzeichnung, ob die kostenlose Position produziert oder eingekauft wurde.
-   **Kosten:** Kosten, die durch die Produktion oder den Einkauf zu dieser Position verursacht wurden.
-   **Verkaufs-Preis:** In dieser Übersicht ist der VK-Preis immer 0.
-   **Gewinn:** Wenn Kosten in der Position entstanden sind, wird der Gewinn als negativer Betrag angezeigt.
-   **Gewinn%:** In dieser Übersicht ist der Gewinn immer 0.
-   **Grund:** Wenn Sie die Begründung für manuelle Preisvorgaben aktiviert und eine entsprechende Bemerkung eingetragen haben, wird dieser Text angezeigt.

## Deckungsbeitrags-Analyse

**Pfad:** `Dokumente > Auftrag > Auswertungen > Deckungsbeitrags-Analyse`

In diesem Dialog können Sie die Deckungsbeiträge auswerten.

> **Voraussetzung**
> Deckungsbeitrag wird nur angezeigt, wenn entweder Standardwerte in den Firmendaten hinterlegt sind, oder wenn für die Kombination von Kunde/Kundengruppe und Warengruppe abweichende Werte festgelegt wurden.
> Die prozentualen Werte für die Deckungsbeiträge können für jede Kombination von Kunde/Kundengruppe und Warengruppe festgelegt sein. Sind für eine mögliche Kombination keine Werte festgelegt, werden die Standardwerte aus den Firmendaten herangezogen.
>
> ⇨ Stammdaten, "Deckungsbeitrags-Grenzwerte" auf Seite B-978
> ⇨ Stammdaten, "Default-Deckungsbeiträge" auf Seite B-1121

In diesem Dialog finden Sie folgende Register:
-   "Deckungsbeitrags-Analyse – Auswahl" auf Seite C-2003
-   "Deckungsbeitrags-Analyse – Tabelle" auf Seite C-2005

### Deckungsbeitrags-Analyse – Auswahl

**Pfad:** `Dokumente > Auftrag > Auswertungen > Deckungsbeitrags-Analyse > Auswahl`

*Abb. C-381 Deckungsbeitrags-Analyse – Auswahl*

In diesem Register wählen Sie aus, in welchen Aufträgen die Deckungsbeiträge analysiert werden sollen.

#### Auftragsfilter

Mit der Wahl der Option legen Sie fest, welche Aufträge analysiert werden sollen:

-   **Nummernverwalter:** Alle Aufträge des gewählten Nummernverwalters werden herangezogen.
-   **Kundengruppe von – bis:** Sie können eine einzelne Kundengruppe oder eine Folge von Kundengruppen auswählen. Die Deckungsbeiträge werden in allen Aufträgen der Kunden analysiert, die zur gewählten Gruppe gehören. Dabei spielt es keine Rolle, in welchem Nummernverwalter die Aufträge stehen.
-   **Kunde von – bis:** Sie können einen einzelnen Kunden oder eine Folge von Kunden auswählen. Die Deckungsbeiträge werden in allen Aufträgen der gewählten Kunden analysiert. Dabei spielt es keine Rolle, in welchem Nummernverwalter die Aufträge stehen.

#### Positionsfilter

Mit der Wahl der Option legen Sie fest, welche Produkte betrachtet werden sollen.

-   **Warengruppe:** Sie können eine einzelne Warengruppe oder eine Folge von Warengruppen auswählen. Die Deckungsbeiträge werden in allen Positionen analysiert, die zur gewählten Gruppe gehören.
-   **Produkt:** Sie können ein einzelnes Produkt oder eine Folge von Produkten auswählen. Die Deckungsbeiträge werden in allen Positionen analysiert, in denen die betreffenden Produkte gefunden werden.

#### Restriktionen

Sie können die Analyse der Deckungsbeiträge weiter einschränken.

**Status** Sie können einen einzelnen Status oder eine Folge auswählen. Die Deckungsbeiträge werden in allen Aufträgen analysiert, in einen betreffenden Status haben.

**Erfassung** Sie können den Zeitraum bestimmen, in dem die Aufträge erfasst wurden, die Sie analysieren möchten.

#### Sortierung

Mit der Wahl der Option legen Sie fest, wie das Suchergebnis im Register Tabelle sortiert werden soll.

### Deckungsbeitrags-Analyse – Tabelle

**Pfad:** `Dokumente > Auftrag > Auswertungen > Deckungsbeitrags-Analyse > Tabelle`

*Abb. C-382 Deckungsbeitrags-Analyse - Tabelle*

In diesem Register werden alle Aufträge mit den Angaben zu den Deckungsbeiträgen aufgelistet, die Sie im Register Auswahl herausgefiltert haben. Diese Auswahl können Sie weiter filtern.

#### Deckungsbeitrags-Filter

Mit der Wahl der Option wird das Suchergebnis weiter gefiltert:

-   **Kein Filter:** Das Suchergebnis wird nicht weiter gefiltert.
-   **Größer Maximalwert:** Aus dem Suchergebnis werden nur die Auftragspositionen angezeigt, deren Deckungsbeitrag größer ist, als der festgelegte Maximalwert.
-   **Kleiner Minimalwert:** Aus dem Suchergebnis werden nur die Auftragspositionen angezeigt, deren Deckungsbeitrag kleiner ist, als der festgelegte Minimalwert.
-   **Größer Maximalwert oder kleiner Minimalwert:** Aus dem Suchergebnis werden alle die Auftragspositionen angezeigt, deren Deckungsbeitrag größer ist, als der festgelegte Maximalwert oder kleiner als der festgelegte Minimalwert ist.
-   **Benutzerdefinierter Deckungsbeitrag:** Aus dem Suchergebnis werden alle Auftragspositionen angezeigt, deren Deckungsbeitrag zwischen einem unteren und einem oberen Wert liegt, den Sie selbst bestimmen können.
-   **Minimal - maximal:** Diese Felder sind nur freigeschaltet, wenn Sie die Option Benutzerdefinierter Deckungsbeitrag gewählt haben. Tragen Sie in den Feldern die Werte ein, zwischen denen der Deckungsbeitrag liegen soll.

## Kalkulatorische Frachtkosten

**Pfad:** `Dokumente > Auftrag > Auswertungen > Kalkulatorische Frachtkosten`

Mit der Bestellübergabe werden die Produkte aus den Aufträgen herausgefiltert, die bestellt werden müssen.

> **Voraussetzung**
> Die Frachtkosten können nur berechnet und geprüft werden, wenn die Entfernungen in den Kundenstammdaten und die Kilometerpauschale in den Touren hinterlegt sind.

In diesem Dialog finden Sie folgende Register:
-   "Kalkulatorische Frachtkosten - Druck" auf Seite C-2007
-   "Kalkulatorische Frachtkosten - Speditionskosten" auf Seite C-2009

### Kalkulatorische Frachtkosten - Druck

**Pfad:** `Dokumente > Auftrag > Auswertungen > Kalkulatorische Frachtkosten > Druck`

*Abb. C-383 Kalkulatorische Frachtkosten - Druck*

In diesem Register lassen Sie sich die Verteilung der Frachtkosten über einen bestimmten Zeitraum anzeigen lassen. In der Übersicht können Sie Touren mit zu hohen Frachtkosten in Bezug auf den Umsatz identifizieren.

Im Auftrag können Sie sich die Frachtkosten ebenfalls anzeigen lassen.
"Kalkulatorische Frachtkosten" auf Seite C-1858

#### Liefertermine, Kunden

**Von, bis** Einschränkung der Auswertung auf einen Zeitraum und einen oder eine Reihe von Kunden. Wenn Sie in beiden Feldern denselben Wert eingeben, wird die Auswertung auf einen Tag oder einen Kunden eingeschränkt.

#### Darstellung

Mit der Wahl der Option legen Sie fest, wie die Frachtkosten dargestellt werden sollen:
-   **Tour:** Die Auswertung wird pro Tour und Datum nach Kunden sortiert.
-   **Kunde:** Die Auswertung wird pro Kunde und Datum nach Touren sortiert.

**Kumuliert** Die Auswertung kann detailliert oder kumuliert dargestellt werden.
-   ☐ Die Daten werden detailliert pro Lieferdatum angezeigt.
-   ☑ Die Daten werden summiert pro Lieferdatum angezeigt.

#### Tourenauswahl

In der Auswahl werden alle Touren aufgelistet, die in den Stammdaten hinterlegt sind. Sie müssen mindestens eine Tour in das rechte Feld verschieben, damit die Daten ausgewertet werden können.

#### Aufträge

In der Übersicht werden alle Aufträge und Touren aufgelistet, die den Auswahlkriterien entsprechen. Die einzelnen Aufträge werden nur angezeigt, wenn für die Darstellung die Checkbox Kumuliert nicht markiert ist.

### Kalkulatorische Frachtkosten – Speditionskosten

**Pfad:** `Dokumente > Auftrag > Auswertungen > Kalkulatorische Frachtkosten > Speditionskosten`

*Abb. C-384 Kalkulatorische Frachtkosten – Speditionskosten*

In diesem Register erfassen Sie die Speditionskosten. Dazu muss mindestens eine Tour Spedition angelegt sein.

Speditionskosten, die durch ein Speditionsunternehmen entstehen, können folgendermaßen auf mehrere Aufträge verteilt werden:
-   Verteilung von Speditionskosten auf Aufträge nach Liefertermin und Tour.
-   Verteilung der gesamten Speditionskosten im Verhältnis zur Entfernung und zur transportierten Glasfläche.

Zur Berechnung des Anteils wird die tatsächliche Glasfläche ohne Maßrundungen betrachtet.

#### Selektion

**Liefertermin** Tag, an dem die Spedition die Tour fährt.
**Tour** Auswahl der Tour, die von der Spedition gefahren wird. Zur Auswahl stehen nur die Touren, für die keine Kilometerpauschale angegeben ist.

#### Speditionskosten

**Betrag (Netto)** Angabe des Rechnungsbetrags aus der Speditionsrechnung.

#### Aufträge

In der Übersicht werden nur die Aufträge angezeigt, auf die der Liefertermin und die gewählte (Speditions-)Tour zutreffen.

## Interne Kontrolle

**Pfad:** `Dokumente > Auftrag > Interne Kontrolle`

In diesem Bereich können Sie Auswertungen zu Gutschriftsgründen und zu Preisänderungen erstellen.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
-   "Gutschriftgründe" auf Seite C-2011
-   "Änderungen am Kundenstamm" auf Seite C-2012
-   "Preis-/Rabattänderungen" auf Seite C-2013
-   "Verspätete Lieferung/Lieferung ohne Berechnung" auf Seite C-2014

### Gutschriftgründe

**Pfad:** `Dokumente > Auftrag > Interne Kontrolle > Gutschriftgründe`

*Abb. C-385 Gutschriftgründe*

In diesem Dialog können Sie über einen definierten Zeitraum auswerten, aus welchen Gründen Gutschriften erstellt wurden.

#### Selektion

**Datum von, bis** Eingrenzung des Zeitraums, in dem nach Gutschriften gesucht wird. Wenn Sie einen großen Zeitraum angeben, sollten Sie die Archive mit einbeziehen.

**Archive mit einbeziehen**
Die Auswertung kann auch die Archive einbeziehen.
-   ☐ Die Suche bezieht sich nur auf die Hauptdatenbank.
-   ☑ Die archivierten Dokumente werden in die Suche bezogen.

#### Gutschriften

Liste der Gutschriften, die den Auswahlkriterien entsprechen.

#### Zusammenfassung

In der Übersicht werden die Gutschriften nach Gründen zusammengefasst.

### Änderungen am Kundenstamm

**Pfad:** `Dokumente > Auftrag > Interne Kontrolle > Änderungen am Kundenstamm`

*Abb. C-386 Änderung am Kundenstamm*

In diesem Dialog können Sie sich Änderungen der Kundenstammdaten über einen bestimmten Zeitraum anzeigen lassen. Der Dialog ist nur kundenspezifisch freigeschaltet.

### Preis-/Rabattänderungen

**Pfad:** `Dokumente > Auftrag > Interne Kontrolle > Preis-/Rabattänderungen`

*Abb. C-387 Preis-/Rabattänderungen*

In diesem Dialog können Sie sich Änderungen der Preise und Rabatte über einen bestimmten Zeitraum anzeigen lassen. Der Dialog ist nur kundenspezifisch freigeschaltet.

### Verspätete Lieferung/Lieferung ohne Berechnung

**Pfad:** `Dokumente > Auftrag > Interne Kontrolle > Verspätete Lieferung/Lieferung ohne Berechnung`

*Abb. C-388 Verspätete Lieferung/Lieferung ohne Berechnung*

In diesem Dialog können Sie auswerten, bei welchen Aufträgen das Lieferdatum überschritten ist, bzw. bei welchen Aufträgen noch keine Rechnung geschrieben wurde. Dazu können Sie ein Vergleichsdatum angegeben.

#### Selektion

Mit der Wahl der Option legen Sie fest, welche Suchkriterien Sie nutzen wollen:
-   **Nummernverwalter:** Die Suche bezieht sich auf die Dokumente im gewählten Nummernverwalter.
-   **Eigene Auswahl:** Für die Suche können der Status und das Lieferdatum als Kriterien angegeben werden.

**Status von, bis** Die Suche wird über den Status eingegrenzt.
**Lieferdatum von, bis** Die Suche wird auf den Zeitraum eingegrenzt, in dem die Lieferung erfolgen sollte.

#### Lieferungen

In der Übersicht werden alle Aufträge aufgelistet, die den Suchkriterien entsprechen. Diese Trefferliste kann weiter gefiltert werden.

#### Filter

Mit der Wahl der Option legen Sie fest, welche Aufträge angezeigt werden sollen.
-   **Verspätete Lieferung:** In der Trefferliste werden alle Aufträge angezeigt, die in Bezug auf das Vergleichsdatum verspätet sind.
-   **Lieferung ohne Berechnung (Ware geliefert und noch keine Rechnung geschrieben):** In der Trefferliste werden alle Aufträge angezeigt, zu denen trotz der Lieferung noch keine Rechnung erstellt wurde.

**Vergleichsdatum** Vergleichsdatum für die Filterung der Trefferliste.

## Gutschrift

**Pfad:** `Dokumente > Gutschrift`

Über das Menü Gutschrift erreichen Sie sich folgende Programmpunkte:

-   **NV Gutschrift:** Die Funktion des Nummernverwalters ist für alle Dokumente gleich. Sie wird am Beispiel Auftrag beschrieben.
    ⇨ "Nummernverwalter" auf Seite C-1914
-   **Gutschrift:** Die Erfassung von Dokumenten ist für alle Dokumentenarten gleich. Sie wird am Beispiel Auftrag beschrieben.
    ⇨ "Dokumentenverwaltung" auf Seite C-1679
    ⇨ "Dokument - Positionen" auf Seite C-1724
-   **Druck Gutschrift:** Der Formular- und Etikettendruck ist für alle Dokumente gleich. Er wird am Beispiel Auftrag beschrieben.
    ⇨ "Druck" auf Seite C-1923
-   **FiBu-Übergabe:** Die FiBu-Übergabe ist für Aufträge, Gutschriften und Bestellungen gleich. Sie wird am Beispiel Auftrag beschrieben.
    ⇨ "FiBu-Übergabe" auf Seite C-1967
-   **Journal:** Der Journaldruck ist für alle Dokumente gleich. Er wird am Beispiel Auftrag beschrieben.
    ⇨ "Journal" auf Seite C-2018
-   **Anzahlungen Gutschriften:** Die Anzahlungen sind für alle Dokumente gleich. Sie werden am Beispiel Auftrag beschrieben.
    ⇨ "Anzahlungen" auf Seite C-1961
-   **Übergabe Archiv:** Die Archivübergabe ist für alle Dokumente gleich. Sie wird am Beispiel Auftrag beschrieben.
    ⇨ "Übergabe Archiv" auf Seite C-1974
-   **Suche:** Die Suche ist für alle Dokumente gleich. Sie wird am Beispiel Auftrag beschrieben.
    ⇨ "Dokument suchen" auf Seite C-1803
-   **Bankbelege:** Die Bankbelege sind für Aufträge und Gutschriften gleich. Sie werden am Beispiel Auftrag beschrieben.
    ⇨ "Bankbelege" auf Seite C-1962
-   **Import:** Mit dieser Funktion werden elektronische Dokumente importiert.
    ⇨ "Import" auf Seite C-1976

### Gutschrift (Dokumentenverwaltung)

**Pfad:** `Dokumente > Gutschrift > Gutschrift`

In diesem Dialog erfassen und bearbeiten Sie Gutschriften.
Die Felder im Dialog Kopfdaten und in der Positionserfassung sind für alle Dokumententypen gleich. Sie werden in dieser Anleitung am Beispiel Auftrag beschrieben.
⇨ "Dokument - Kopfdaten" auf Seite C-1687
⇨ "Dokument - Positionen" auf Seite C-1724

## Journal

**Pfad:** `Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Journal`

Die Ausgabe eines Journals ist für alle Dokumente gleich. Sie wird in dieser Anleitung am Beispiel Auftrag beschrieben.
⇨"Eingangs-/Ausgangs-Journal" auf Seite C-2018

### Eingangs-/Ausgangs-Journal

**Pfad:** `Dokumente > Auftrag > Journal`

*Abb. C-389 Eingangs/Ausgangs-Journal*

In diesem Dialog können Sie sich Listen zu den Dokumenten ausgeben lassen.
⇨ Tutorial, "Journal" auf Seite C-1646

#### Auswahl Bereich

Mit der Wahl der Option geben Sie an, für welche Dokumente Sie das Journal erstellen wollen:
-   Angebot
-   Auftrag
-   Gutschrift
-   Bestellanfrage
-   Bestellung

#### Datenbank

Wenn Sie mit mehreren Datenbanken arbeiten, müssen Sie auswählen, aus welcher das Journal erstellt werden soll. Zur Wahl stehen auch die Archive.

#### Modus

Mit der Wahl der Option geben Sie die Bedingungen für die Erstellung der Liste an:
-   **Nach Nummernverwalter:** Die Liste soll alle Dokumente aus einem bestimmten Nummernverwalter auflisten. Im Bereich Identifikation/Nummernverwalter wird das Feld Nummernverwalter wird freigeschaltet.
-   **Nach Auswahlkriterien:** Die Liste soll alle Dokumente nach Kriterien auflisten, die Sie selbst bestimmen. Im Bereich Auswahl Kriterien werden die Felder wird freigeschaltet.

#### Auswahl Liste

Zur Auswahl stehen verschiedene fest definierte Listen. Jede Liste schließt mit der Gesamtsumme pro Spalte.
⇨ Tutorial, "Journal" auf Seite C-1646

#### Zwischensummen

Die Ausgabe der Zwischensumme können Sie selbst bestimmen. Im Tutorial finden Sie eine Beschreibung der Darstellungen im Report.
⇨ Tutorial, "Journal" auf Seite C-1646

**Pro Kunde, Pro Rechnung, Pro Vertreter** Eine Zwischensumme kann pro Kunde, Rechnung und/oder Vertreter eingefügt werden.
-   ☐ Die Zwischensumme wird nicht ausgegeben.
-   ☑ Die Zwischensumme wird an der gewählten Stelle ausgegeben.

#### Identifikation/Nummernverwalter

**Mitarbeiter** Name des Mitarbeiters, der sich in A+W Business angemeldet hat.
**Nummernverwalter** Auswahl des Nummernkreises, dessen Dokumente aufgelistet werden sollen. Das Feld ist gesperrt, wenn im Bereich Modus die Option nach Auswahlkriterien gewählt wurde.

#### Auswahl Kriterien von, bis

Die Felder sind gesperrt, wenn im Bereich Modus die Option nach Nummernverwalter gewählt wurde.

**Statusbereich von, bis** Eingabe von Statusnummern der Dokumente. Wenn Sie in beiden Feldern dieselbe Nummer eingeben, werden nur die Dokumente mit diesem Status aufgelistet.
**Erfassungsdatum von, bis** Das Journal wertet nur die Dokumente im gewählten Erfassungszeitraum aus.
**Datum AB von, bis** Das Journal wertet nur die Dokumente aus, deren Auftragsbestätigung im gewählten Erfassungszeitraum gedruckt wurde.
**Lieferdatum von, bis** Das Journal wertet nur die Dokumente im gewählten Lieferzeitraum aus.
**Rechnungsdatum von, bis** Das Journal wertet nur die Dokumente aus, deren Rechnungsdatum im gewählten Erfassungszeitraum liegt.

#### Druck-Optionen

Mit der Wahl der Option legen Sie fest, wie die Maße ausgedruckt werden sollen:
-   **Dimensionsangaben real:** Im Druck wird die tatsächliche Fläche angegeben.
-   **Dimensionsangaben fakturiert:** Im Druck wird die fakturierte Fläche angegeben, in der z. B. die Maßrundungen berücksichtigt sind.

**Erste Kommission auf Versandliste** Für die Versandliste kann zusätzlich die Kommission ausgegeben werden.
-   ☐ Die erste Kommission wird nicht ausgegeben.
-   ☑ Die Kommission wird aus der ersten Position in der Positionserfassung übernommen.
    ⇨ "Kommission" auf Seite C-1730

## Bestandslisten

**Pfad:** `Dokumente > Bestandslisten`

In diesem Programmbereich können Sie Übersichten über Dokumente verschaffen, die aktuell in der Hauptdatenbank verwaltet werden.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
-   "Nummernbereiche" auf Seite C-2021
-   "Warengruppen" auf Seite C-2023

### Nummernbereiche

**Pfad:** `Dokumente > Bestandslisten > Nummernbereiche`

*Abb. C-390 Bestandslisten – Nummernbereiche*

Wenn Sie mit Nummernbereichen arbeiten, können Sie sich in diesem Dialog Übersichten über den aktuellen Bestand an Dokumenten in den Nummernkreisen verschaffen.
Das Programm schaut in den Nummernkreisen in den Stammdaten nach der letzten Nummer. Anschließend listet es hier alle Dokumente hier auf, die noch nicht gedruckt wurden.
Mit der Bestätigung, dass der Ausdruck OK war, wird die letzte Nummer hier angezeigt und gleichzeitig in den Stammdaten aktualisiert.
⇨ Stammdaten, "Nummernkreise" auf Seite B-1028

#### Nummernkreis

**Mandant** Mandanten, für den die Übersicht erstellt wird.
⇨ Stammdaten, "Firmendaten - Mandant" auf Seite B-1056

**AV-Bereich** AV-Bereichen, zu dem die Dokumente gehören. Das Feld ist gesperrt, wenn die Checkbox Alle im AV-Bereich drucken markiert ist.

**Alle im AV-Bereich drucken** Sie können wahlweise alle Dokumente eines AV-Bereichs drucken oder einen bestimmten auswählen. Mit der Schaltfläche öffnen Sie den Dialog Nummernkreise.
-   ☐ Die Dokumente aus dem Nummernkreis des gewählten AV-Bereichs werden gedruckt.
-   ☑ Alle Dokumente aus den Nummernkreisen des gewählten Mandanten werden gedruckt. Das Feld AV-Bereich wird gesperrt.

#### Dokumententyp

Mit der Wahl der Option bestimmen Sie, für welchen Dokumententyp eine Bestandsliste erstellt werden soll.
Nach dem erfolgreichen Erstellen der Übersicht wird jeweils die letzte Nummer für den Dokumententyp angezeigt. Diese Nummer wird auch im Dialog Nummernkreise angezeigt.
⇨ Stammdaten, "Nach Zeitraum" auf Seite B-1029

### Warengruppen

**Pfad:** `Dokumente > Bestandslisten > Warengruppen`

*Abb. C-391 Bestandslisten – Warengruppen*

In diesem Dialog können Sie sich Übersichten über den aktuellen Dokumentenbestand in den Nummernverwaltern oder nach Zeiträumen für die Erfassung oder Lieferung verschaffen. Die Übersicht ist nach Warengruppen geordnet. Sie wird mit der Druckfunktion ausgegeben.
⇨ Tutorial, "Bestandslisten" auf Seite C-1645

#### Druckparameter Selektion

Mit der Wahl der Optionen legen Sie fest, nach welchen Kriterien die Dokumente gesucht werden sollen.

**Nummernverwalter** Die Bestandsliste prüft alle Dokumente im gewählten Nummernverwalter. Die Auswahlmöglichkeiten richten sich nach dem gewählten Dokumententyp.
Die Eingabefelder für Erfassungsdatum, Liefertermin und Status sind gesperrt.

**Erfassungsdatum von, bis** Die Bestandsliste stellt nur die Dokumente im gewählten Erfassungszeitraum dar.
**Liefertermin von, bis** Die Bestandsliste stellt nur die Dokumente im gewählten Lieferzeitraum dar.
**Status von, bis** Die Bestandsliste stellt nur die Dokumente mit den gewählten Statusnummern dar.

#### Dokumententyp

Mit der Wahl der Option bestimmen Sie, für welchen Dokumententyp eine Bestandsliste erstellt werden soll.

#### Auswertungstiefe von - bis

Mit der Wahl der Option legen Sie fest, nach welcher Ebene von Warengruppen die Bestandslisten zusammengefasst werden.
Für die Auswahl der Dokumente kann ein Bereich angegeben werden. Die Felder von und bis sind gesperrt, wenn die Checkbox Alle drucken markiert ist.

**Alle drucken** Sie können in der Bestandsliste alle Dokumente berücksichtigen, die zu einer Warenhauptgruppe, Warenobergruppe oder Warengruppe gehören.
-   ☐ Nur die Dokumente des eingestellten Bereichs der Warengruppenebene werden berücksichtigt.
-   ☑ Alle Dokumente der gewählten Warengruppenebene werden berücksichtigt. Die Felder von und bis sind gesperrt.

**Nur Gesamtsummen der WGR drucken** Sie können nur die Gesamtsumme je Warengruppen drucken.
-   ☐ Alle Werte des eingestellten Bereichs der Warengruppenebene werden dargestellt.
-   ☑ Nur die Gesamtsummen des eingestellten Bereichs der Warengruppenebene werden dargestellt.

**Einkaufspreis nicht drucken** Sie können die Einkaufspreise ausschließen.
-   ☐ Alle Werte des eingestellten Bereichs der Warengruppenebene werden dargestellt.
-   ☑ Die Einkaufspreise werden nicht dargestellt.

**Erste Kommission des Auftrags drucken** Sie können die Angaben zur Kommission aus dem Auftrag übernehmen.
-   ☐ Alle Werte des eingestellten Bereichs der Warengruppenebene werden dargestellt.
-   ☑ Zusätzlich zur Auftragsnummer wird die Kommissionsnummer dargestellt.
    ⇨ "Kommission" auf Seite C-1730

## Mahnwesen

**Pfad:** `Dokumente > Mahnwesen`

Die ausgegangenen Rechnungen können über die Rückmeldung der offenen Posten geprüft werden. Mahnungen können für Rechnungen ausgegeben werden.
⇨ Tutorial, "Mahnung senden" auf Seite C-1475

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
-   Menüs im Dialog Mahnwesen
-   "Mahnwesen" auf Seite C-2026
-   "Offene-Posten-Tabelle füllen" auf Seite C-2029

### Menüs im Dialog Mahnwesen

**Pfad:** `Dokumente > Mahnwesen`

Über die Menüs im Dialog Mahnwesen können Sie die Standardeinstellung des Dialoges bestimmen und andere Dialoge öffnen, ohne den Dialog Dokumente zu schließen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
-   "Menü Zahlung" auf Seite C-2025
-   "Menü Optionen" auf Seite C-2025
-   "Menü Funktionen" auf Seite C-2026

#### Menü Zahlung

**Pfad:** `Dokumente > Mahnwesen > Menü Zahlung`

Über dieses Menü können Sie Zahlungen zu einer angemahnten Rechnung erfassen oder bearbeiten.

-   **Neue Zahlung:** Schaltet die Felder frei, um zu einer markierten Rechnung eine Zahlung zu erfassen.
-   **Zahlung löschen:** Löscht die Zahlung, die zu einer Rechnung erfasst wurde.
-   **Zahlung ändern:** Schaltet die Felder einer markierten Rechnung frei, um die Werte einer erfassten Zahlung zu ändern.

#### Menü Optionen

**Pfad:** `Dokumente > Mahnwesen > Menü Optionen`

Über dieses Menü können Sie eine erfasste Mahnung per Fax versenden.
-   **Faxversand:** Mahnungen können per Fax versendet werden. Dazu muss eine Fax-Nummer in der Rechnung erfasst sein.

#### Menü Funktionen

**Pfad:** `Dokumente > Mahnwesen > Menü Funktionen`

Über dieses Menü können Sie die Mahnstufen bearbeiten und das Mahnkennzeichen von einer Rechnung löschen.

-   **Mahnstufen:** Öffnet den Dialog Mahnstufen, in dem Sie neue Mahnstufen erfassen können.
    "Mahnstufen" auf Seite C-2028
-   **Mahnstufe zurücksetzen:** Setzt das Mahnkennzeichen der markierten Rechnungen zurück.
-   **Offene-Posten-Tabelle füllen:** Öffnet einen Dialog, um den Nummernverwalter mit den offenen Rechnungen auszuwählen. Diese Funktion ist abhängig von der aktuellen FiBu.
    "Offene-Posten-Tabelle füllen" auf Seite C-2029

### Mahnwesen Dialog

**Pfad:** `Dokumente > Mahnwesen`

**Zu Dialogbeschreibung:**
-   Mahnstufen
-   Offene-Posten-Tabelle füllen

*Abb. C-392 Mahnwesen*

In diesem Dialog können Sie eingegangene Zahlungen zu offenen Rechnungen verbuchen oder Mahnungen erstellen. Sie können die Daten einzeln einlesen oder die Dokumente aus einem Nummernverwalter anzeigen lassen.
⇨ Tutorial, "Mahnung" auf Seite C-1471

#### Rechnung

**Nr./Datum** Nummer und Datum der Rechnung, die in der Übersicht markiert ist. Die Felder sind nur freigeschaltet, wenn Sie eine neue Rechnung erfassen möchten.

**Mahnstufe** Mahnstufen sind in den Stammdaten hinterlegt. Mit der Auswahl einer Mahnstufe wird gleichzeitig die Gebühr angezeigt.

**Gebühr/Datum** Die Gebühr wird automatisch angezeigt, wenn mit der Mahnstufe eine Gebühr erhoben wird. Der Betrag kann überschrieben werden. Das Datum wird nur angezeigt, wenn zu einer Rechnung bereits eine Mahnung verschickt wurde.

**Ausgeglichen** Sie können Rechnungen als ausgeglichen kennzeichnen, wenn die Differenz zwischen dem Rechnungsbetrag und der Zahlung so geringfügig ist, dass sie vernachlässigt werden kann.
-   ☐ Wenn noch ein Betrag offen ist, soll die Rechnung nicht als ausgeglichen gelten.
-   ☑ Die Rechnung soll als ausgeglichen gelten, obwohl noch ein Betrag offen ist.

**Betrag** Betrag der Rechnung, die in der Übersicht markiert ist.

**Geleistet** Der als Zahlung erfasste Betrag.

**Offen** Die Differenz zwischen dem Rechnungsbetrag und der erfassten Zahlung wird automatisch angezeigt. Eine offene Differenz wird in roter Schrift dargestellt, eine Überzahlung in blauer Schrift.

#### Kunde

Die Felder in diesem Bereich sind nur freigeschaltet, wenn Sie eine neue Rechnung anlegen.

**Nr./Name** Nummer und Name des Kunden, dessen Rechnung noch offen ist.

**Anschrift** Rechnungsanschrift wird aus dem Auftrag.

**Fax** Fax-Nummer aus dem Auftrag.

#### Geleistete Zahlungen

In diesem Bereich werden die zu einer Rechnung erfassten Zahlungen aufgelistet.

#### Zahlung

Die Felder in diesem Bereich sind nur freigeschaltet, wenn Sie eine Zahlung erfassen möchten.

**Betrag** Betrag der neuen Zahlung. Wenn er nicht mit dem Rechnungsbetrag übereinstimmt, wird die Differenz im Feld offen ausgewiesen.

**Datum** Aktuelles Datum (Systemdatum). Es kann überschrieben werden.

**Abgezogenes Skonto** Wenn mit dem Kunden ein Skonto vereinbart wurde, kann der Betrag eingetragen werden. Auf diese Weise können offene Rechnungen aus Kulanzgründen als ausgeglichen erfasst werden, obwohl der Zahlungstermin überschritten wurde.

**Rechnung** Betrag angezeigt, der als Zahlung erfasst wurde.

#### Rechnungen

In der Übersicht werden alle Rechnungen aufgelistet, die gemahnt werden müssen, weil ihr Zahlungstermin überschritten ist.

### Mahnstufen

**Pfad:** `Dokumente > Mahnwesen > Menü Funktionen > Mahnstufen`

*Abb. C-393 Mahnstufen*

In diesem Dialog können Sie die Mahnstufen einrichten und bearbeiten.

### Offene-Posten-Tabelle füllen

**Pfad:** `Dokumente > Mahnwesen > Menü Funktionen > Offene Posten-Tabelle füllen`

*Abb. C-394 OP-Tabelle füllen*

In diesem Dialog können Sie einen Nummernverwalter auswählen, um die offenen Rechnungen in den Dialog Mahnwesen einzulesen. Diese Funktion ist abhängig von der aktuellen FiBu.

## Dokumentendaten

**Pfad:** `Dokumente > Dokumentendaten`

Die Bestell- und Lieferdaten von Dokumenten in einem Nummernverwalter können bearbeitet werden, ohne die Dokumente einzeln zu suchen und zu öffnen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
-   "Menüs im Dialog Dokumente" auf Seite C-2030
-   "Dokumentendaten" auf Seite C-2031

### Menüs im Dialog Dokumente

**Pfad:** `Dokumente > Dokumentendaten`

Über die Menüs im Dialog Dokumente können Sie die Standardeinstellung des Dialoges bestimmen und andere Dialoge öffnen, ohne den Dialog Dokumente zu schließen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
-   "Menü Funktionen" auf Seite C-2030
-   "Menü Optionen" auf Seite C-2030

#### Menü Funktionen

**Pfad:** `Dokumente > Dokumentendaten > Menü Funktionen`

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Dialog Dokumente zu schließen. Folgende Einträge werden angezeigt:

-   **Historie:** Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des Dokuments.
    ⇨ "Historie" auf Seite C-1834
-   **Dokument anzeigen:** Öffnet den Dialog Dokumentenansicht als Vorschau auf das Dokument.
    ⇨ "Dokument anzeigen" auf Seite C-1829

#### Menü Optionen

**Pfad:** `Dokumente > Dokumentendaten > Menü Optionen`

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Option aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

-   **Dokumente in Hauptdatenbank und Archiv suchen:** Standardmäßig werden die Dokumente nur aus der Hauptdatenbank ausgelesen. Mit dieser Option legen Sie fest, dass die Dokumente sowohl aus der Hauptdatenbank als auch aus dem Archiv ausgelesen werden.
    ⇨ Stammdaten, "Firmendaten - Archiv" auf Seite B-1104

### Dokumentendaten Dialog

**Pfad:** `Dokumente > Dokumentendaten`

*Abb. C-395 Dokumentdaten*

In diesem Dialog können Sie die Auftrags- und die Bestelldaten zu den Dokumenten prüfen.

#### Auswahlkriterien

**Dokument** Auswahl des Dokumententyps, der angezeigt werden soll.

**Nummer** Mit der Eingabe der Nummer lassen Sie sich ein ganz bestimmtes Dokument anzeigen. Das Feld ist gesperrt, wenn Sie die Checkbox Nummernverwalter markiert haben.

**Nummernverwalter** Nummernverwalter, dessen Dokumente Sie prüfen wollen. Wenn Sie ein Dokument geändert haben, wird es im angezeigten Nummernverwalter abgelegt.
-   ☐ Die Auswahl des Nummernverwalters ist gesperrt. Das Feld Nummer ist freigeschaltet.
-   ☑ Die Dokumente aus einem Nummernverwalter sollen angezeigt werden. Das Auswahlfeld ist freigeschaltet.

#### Auftrag

**Nummer** Die Auftragsnummer wird nur angezeigt, wenn ein einzelner Auftrag ausgewählt wurde.

**Versand Plan** Das geplante Versanddatum wird nur angezeigt, wenn ein einzelner Auftrag ausgewählt wurde.

**Versandtag** Versandtag aus dem Auftrag. Wenn der Liefertermin geändert wurde, können Sie das Datum entsprechend anpassen.

**Anlieferung** Datum der Anlieferung beim Kunden aus dem Auftrag. Wenn der Liefertermin geändert wurde, können Sie das Datum entsprechend anpassen.

**Status** Status des Auftrags. Sie können ihn bei Bedarf anpassen.

**Tour** Tour aus dem Auftrag. Sie können sie bei Bedarf ändern.

**Lieferbed.** Lieferbedingung aus dem Auftrag. Sie können sie bei Bedarf ändern.

**Kunde, Telefon** Die Daten werden nur angezeigt, wenn ein einzelner Auftrag ausgewählt wurde.

**Ziel-NV** Die Dokumentendaten können in einen anderen Nummernverwalter gestellt werden.
-   ☐ Die Dokumentendaten werden nicht in einen anderen Nummernverwalter gestellt.
-   ☑ Die Kombobox für den Ziel-Nummernverwalter wird freigeschaltet. Die Dokumentendaten werden in den gewählten Nummernverwalter gestellt.

#### Übersicht (Auftrag)

In der Übersicht wird das gewählte Dokument oder alle Dokumente aus dem Nummernverwalter angezeigt.

#### Bestellung

**Nummer** Die Bestellnummer wird nur angezeigt, wenn ein einzelner Auftrag ausgewählt ist, zu dem eine Bestellung erzeugt wurde.

**Anlief. Plan** Geplantes Anlieferungsdatum aus der Bestellung.

**Anlief. Termin** Termin der Anlieferung aus der Bestellung. Wenn der Lieferant einen späteren Termin bestätigt hat, können Sie das Datum ändern. Der neue Termin wird in den Auftrag und die Bestellung übernommen, der Kunde kann eine Terminberichtigung erhalten.
⇨ “Kundenbenachrichtigung (Lieferterminkontrolle)" auf Seite C-1848

**Status** Status der Bestellung. Sie können ihn bei Bedarf ändern.

**Tour** Tour aus der Bestellung. Sie können sie bei Bedarf ändern.

**Lieferbed.** Lieferbedingung aus der Bestellung. Sie können sie bei Bedarf ändern.

**Lieferant, Telefon** Name und Telefonnummer des Lieferanten aus der Bestellung.

**AB-Lieferant** Die Auftragsbestätigung durch den Lieferanten wird nur angezeigt, wenn das Dokument über den Wareneingang erfasst wurde.
⇨ Einkauf, "AB-Lieferant" auf Seite D-2234

#### Übersicht (Bestellung)

In der Übersicht werden alle Bestellungen zum gewählten Auftrag angezeigt.

## Lagersuche

**Pfad:** `Dokumente > Lagersuche`

Die Lagersuche können Sie auch während der Erfassung einer Position öffnen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
-   "Lagerinfo" auf Seite C-2034
-   "Dokumentenübersicht" auf Seite C-2039

### Lagerinfo

**Pfad:** `Dokumente > Lagersuche`

Über die Lagersuche können Sie den Lagerort für ein Produkt feststellen und den Bestand prüfen.

In diesem Dialog finden Sie folgende Register:
-   "Lagerinfo - Lagersuche" auf Seite C-2035
-   "Lagerinfo - Zukünftiger Lagerbestand" auf Seite C-2038

#### Lagerinfo – Lagersuche

**Pfad:** `Dokumente > Lagersuche > Register Lagersuche`

*Abb. C-396 Lagerinfo - Lagersuche*

In diesem Register können Sie den Bestand Ihrer Lager(orte) prüfen und sich Details zu den gelagerten Gläsern anzeigen lassen.

> **Auswahl in den Auftrag übernehmen**
> Wenn Sie den Dialog Lagerinfo aus der Positionserfassung heraus geöffnet haben, können Sie das gewünschte Produkt mit einem Doppelklick in den Auftrag übernehmen.

##### Auswahl

In den Feldern werden die Details zu der Position angezeigt, die in der Übersicht markiert ist.

**Produkt** Produktnummer, unter der das Produkt in den Stammdaten erfasst ist.
**Art** Produktart, der das Produkt in den Stammdaten zugeordnet ist.
**Gruppe** Produktgruppe, der das Produkt in den Stammdaten zugeordnet ist.
**Identnr.** Identifikationsnummer, unter der der Lagerartikel im Lager erfasst wurde, z. B. für eine Kiste.
**Kateg.** Wenn in Ihrem Unternehmen Lagerkategorien definiert sind, können diese zum Filtern eingesetzt werden.
⇨ Stammdaten, "Lagerkategorien" auf Seite B-867
**Farbe** (Farb-) Varianten, die zu dem markierten Produkt erfasst sind.
**WGR von, bis** Zur Suche können Sie auch Warengruppen oder Warengruppenbereiche eintragen. In der Übersicht werden dann alle Produkte der gewählten Warengruppen angezeigt.
**Dicke / Breite / Höhe** Diese Angaben werden aus der Lagerverwaltung übernommen. Breite und Höhe werden nur angezeigt, wenn die markierte Position als Lagermaß oder Kiste mit den entsprechenden Angaben erfasst wurde.
**Lagerort** Wenn Sie mit mehreren Lagerorten arbeiten, wird der Lagerort der markierten Position mit allen definierten Ebenen angezeigt.
⇨ Stammdaten, "Lagerdefinition" auf Seite B-865
**Lief. Ident** Identifikationsnummer der Lieferung aus der Lagerverwaltung. Sie ist nicht identisch mit der Angabe in der Spalte Ident in der Übersicht.
**Bemerkung** Information, die zur markierten Position bei der Lieferung hinterlegt wurde.
**Inhalt von, bis** Im Auswahlmodus kann der Inhalt als Suchkriterium angegeben werden, z. B. alle Kisten mit einem Inhalt von 50 Stück. Inhalt = 1 bedeutet immer Lagermaß.
**Verfügbarkeit** Anzeige der vorrätigen Stückzahlen.

##### Filteroptionen

Wenn keine Filter gesetzt sind, werden keine Bestände angezeigt. Der Filter ist gesetzt, wenn die jeweilige Checkbox markiert ist. Folgende Filter stehen zur Wahl:
-   **Lagerware:** Lagerartikel sollen angezeigt werden.
-   **Kisten (Inhalt > 1):** Kisten mit einem Inhalt > 1 sollen angezeigt werden.
-   **Lagertafeln (Inhalt = 1):** Lagermaße sollen angezeigt werden. Die Anzeige der Anzahl (= 1) dient zur Unterscheidung von Kisten mit identischen Größen.
-   **Artikel ohne Abmessung:** Auch Lagerartikel ohne Abmessungen sollen angezeigt werden.
-   **Kisten mit Identnummer:** Kisten, die mit eine ID im Wareneingang erfasst wurden, sollen angezeigt werden.
-   **Mindestmenge > 0:** Nur die Lagerartikel, deren Mindestmenge größer als 0 definiert wurde, sollen angezeigt werden.
-   **Bestand > 0:** Nur Lagerartikel mit einem Bestand sollen angezeigt werden.
-   **Bestand = 0:** Nur Lagerartikel ohne Bestand sollen angezeigt werden.
-   **Bestand < 0:** Nur die Lagerartikel sollen angezeigt werden, zu denen Reservierungen vorliegen, aber kein Bestand.

##### Druckoptionen

Sie können die Sortierung für den Druck der Übersicht bestimmen. Mit der Wahl der Option werden die entsprechenden Checkboxen freigeschaltet. Sie können dann zusätzlich festlegen, wo eine Zwischensumme gedruckt werden soll.

Folgende Einträge werden angezeigt:
-   **Gruppierung nach Produktnummer:** Die Checkbox Zwischensumme n. Warengruppe wird freigeschaltet.
-   **Gruppierung nach Produktart/Produktgruppe gruppieren:** Die Checkbox Zwischensummen. Warenobergrp. wird freigeschaltet.
-   **Gruppierung nach Warengruppen:** Die Checkbox Zwischensumme n. Warenhauptgrp. wird freigeschaltet.

##### Übersicht

In der Übersicht werden alle Produkte angezeigt, die mit der Suche ausgewählt wurden. Die Spalten zeigen die Details zu den gelagerten Produkten an.

Die reservierten Mengen werden aktualisiert, sobald eine entsprechende Position im Auftrag gespeichert wurde. Mit dem Druck des Lieferscheins werden die Angaben in der Spalte Bestand aktualisiert.

Die Einträge in der Trefferliste sind mit folgenden Farben gekennzeichnet:
-   **Schwarze Schrift:** Lagerartikel mit Mengenführung
-   **Blaue Schrift:** Lagerartikel ohne Mengenführung
-   **Rote Schrift:**
    -   Kein Lagerartikel: Artikel, die nicht im Lager geführt werden.
    -   Dies gilt auch für Produkte, die nicht mehr verfügbar sind oder mit negativen Beständen angezeigt werden. Ein negativer Bestand entsteht, wenn der Bestand und die bestellte Menge abzüglich der reservierten Menge <= 0 sind.

##### Summen

Die Summen des ausgewählten Produkts werden angezeigt. Wenn Sie eine WGR mit verschiedenen Produkten ausgewählt haben, werden die Summen des markierten Produkts angezeigt.

#### Lagerinfo – Zukünftiger Lagerbestand

**Pfad:** `Dokumente > Lagersuche > Register Zukünftiger Lagerbestand`

*Abb. C-397 Lagerinfo - Zukünftiger Lagerbestand*

In diesem Register können Sie prüfen, wie viele Gläser bestellt wurden und wie viele bereits reserviert sind.

##### Aktueller Lagerbestand

##### Vorschau bis

Die Vorschau beginnt immer mit dem aktuellen Tagesdatum. Die Anzahl der Tage für die Vorschau stellen Sie in den Firmendaten ein, z. B. 14 Tage.
-   In der oberen Übersicht werden die Daten in einer Zeile pro gewähltem Produkt aufgelistet.
-   In der mittleren Übersicht werden die aktuellen Bestände pro Tag wiedergegeben.
-   In der unteren Übersicht werden Details zum gewählten Produkt angezeigt. In der Spalte Kritischer Lagerbestand wird die Menge angezeigt, die in der Lagerwirtschaft für den Artikel hinterlegt ist.
    ⇨ Lagerwirtschaft, "Lagerverwaltung - Lagerartikel" auf Seite G-2863

Die Zeilen sind rot, wenn die Produktion nicht möglich ist, weil die Reservierungen den Bestand überschreiten.
⇨ Stammdaten, "Lagervorschau" auf Seite B-1101

### Dokumentenübersicht

**Pfad:** `Dokumente > Lagersuche > Register Zukünftiger Lagerbestand > Übersicht > Doppelklick auf Produkt`

*Abb. C-398 Dokumentenübersicht*

In diesem Dialog wird eine Liste der Dokumente angezeigt, in denen das betreffende Lagermaß erfasst ist.

---

# Teil D: A+W Business Einkauf

### Revisionsübersicht des Moduls:

| Datum | Änderung |
| :--- | :--- |
| 06-2023 | Aktualisierung der Softwarereferenz. |
| 04-2020 | Wareneingang aktualisiert. |
| 11-2019 | Softwarereferenz: Aktualisierung Dialog Wareneingang, Tutorial: Kapitel für Kisten in den Part Kistenmanagement verschoben. |
| 10-2017 | Strukturelle Überarbeitung, neuer Dialog Nachbestellung, Dialog AB-Lieferant aktualisiert. |
| 01-2017 | Produkt- und Firmennamen angepasst. |
| 06-2013 | Vollständige Überarbeitung der ALFAK-Dokumentation und Anpassung auf A+W Business. |
| 02-2012 | Aktualisierung der Kapitel zum Wareneingang. |
| 02-2010 | Aktualisierung und Umstellung auf Doku-Konzept 2010. |
| 10-2008 | Part Einkauf neu. Aus Part Dokumente ausgegliedert. |

**Zu diesem Modul finden Sie folgende Kapitel:**
⇨ Tutorial
⇨ Softwarereferenz

## Tutorial

### In diesem Kapitel finden Sie folgende Themen:

-   **Überblick** (D-2046)
    -   Aufbau des Tutorials (D-2046)
    -   Menü-Übersicht (D-2048)
-   **Grundgedanken zum Einkauf** (D-2051)
-   **Stammdaten für den Einkauf** (D-2054)
    -   Produktdefinition (D-2055)
    -   Bestellkennzeichen (D-2056)
    -   Stammdaten eines Produkts prüfen (D-2059)
    -   Lagermaß anlegen (D-2061)
    -   Lieferanten (D-2064)
    -   Marktpartner Lieferant (D-2065)
    -   Stammdaten eines Lieferanten prüfen (D-2066)
    -   Lieferantenkartei anpassen (D-2067)
    -   EK-Preise (D-2070)
    -   Preislisten (D-2071)
    -   Stammdaten der Preise prüfen (D-2072)
    -   Dokumentenstatus (D-2074)
    -   Statuszuordnung (D-2075)
    -   Statusvergabe (D-2076)
-   **Bestellungen** (D-2077)
    -   Bestellübergabe vs. manuelle Bestellung (D-2078)
    -   Dokument Bestellung (D-2079)
    -   Voreinstellungen für Bestellungen prüfen (D-2081)
    -   Bestellpositionen im Auftrag (D-2084)
    -   Kundenbestellung (D-2085)
    -   Lieferant für Auftragsposition (D-2086)
    -   Änderung in bestellten Positionen (D-2087)
    -   Bestellposition im Auftrag erfassen (D-2088)
    -   Lieferanten im Auftrag ändern (D-2090)
    -   Bestellte Auftragsposition ändern (D-2091)
    -   Bestellübergabe (D-2094)
    -   Bestellpool (D-2096)
    -   Dokument in den Bestellpool stellen (D-2102)
    -   Bestellung im Bestellpool ändern (D-2106)
    -   Preise im Bestellpool vergleichen (D-2108)
    -   Auftrags- und Bestell-Info (D-2112)
    -   Manuelle Bestellung (D-2113)
    -   Unabhängige Bestellungen (D-2114)
    -   Unabhängige Bestellung erfassen (D-2115)
    -   Lagerbestellung erfassen (D-2117)
    -   Auftragsbestätigung des Lieferanten (D-2120)
    -   Lieferanten-AB (D-2121)
    -   Überfällige Lieferungen (D-2122)
    -   Auftragsbestätigung erfassen (D-2123)
    -   AB erfassen und Preise prüfen (D-2127)
    -   Lieferanten anmahnen (D-2131)
    -   Lieferterminkontrolle (D-2134)
    -   Prüfung und Korrektur von Lieferterminen (D-2135)
    -   Liefertermine ändern und Kunden benachrichtigen (D-2136)
    -   Alle Termine prüfen und ändern (D-2139)
-   **Anfrage** (D-2144)
    -   Anfrage zu Bestellpositionen oder Bestellungen (D-2145)
    -   Anfrage zu einer Bestellposition erzeugen (D-2146)
    -   Bestellung aus unabhängiger Anfrage erstellen (D-2149)
-   **Übungen** (D-2151)
-   **Lieferungen im Wareneingang** (D-2153)
    -   Wareneingang (D-2154)
    -   Lieferungen (D-2155)
    -   Voreinstellungen für Wareneingang prüfen (D-2160)
    -   Wareneingang erfassen (D-2161)
    -   Wareneingang kontrollieren (D-2167)
    -   Wareneingang von Kisten (D-2169)
    -   Kistengeschäft (D-2170)
    -   Firmendaten prüfen (D-2170)
    -   Einstellungen für Identnummern prüfen (D-2171)
    -   Wareneingang von Kisten erfassen (D-2172)
-   **Preis- und Rechnungskontrolle** (D-2177)
    -   Eingangsrechnung (D-2178)
    -   Rechnung kontrollieren (D-2180)
-   **Übungen** (D-2183)
-   **Elektronischer Dokumentenaustausch** (D-2184)
    -   Export/Import (openTRANS) (D-2185)
    -   Dokumentenaustausch (D-2187)
    -   Dokumentenkontrolle (D-2190)
    -   Dienste prüfen (D-2193)
    -   Statusvergabe (D-2194)
    -   Voreinstellungen für Datenaustausch prüfen (D-2195)
    -   Währungseinstellungen prüfen (D-2196)
    -   Statusdefinitionen prüfen (D-2197)
    -   Datenexport per openTRANS einstellen (D-2200)
    -   Partnerstammdaten prüfen (D-2202)
    -   Elektronisches Dokument einlesen (D-2203)
    -   Elektronisches Dokument prüfen (D-2204)
    -   Teillieferung aus elektronischem Dokument erstellen (D-2206)
    -   Positionen im elektronischen Dokument zuordnen (D-2207)
    -   Zuschläge/Rabatte manuell zuordnen (D-2209)
    -   Datenexport/-import (EDI) (D-2211)
    -   Datenaustausch im ASC-Format (D-2212)
    -   Firmendaten prüfen (D-2212)
    -   Einstellungen prüfen (D-2212)
    -   Bestellung exportieren (D-2216)

### Überblick

Das Tutorial zum Modul Einkauf beschäftigt sich mit den Grundlagen des Einkaufs in A+W Business. Das Tutorial baut auf den Kenntnissen zu den Stammdaten und zum Verkauf auf.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

#### Themenblöcke

In diesem Tutorial finden Sie folgende Themenblöcke:
-   Grundgedanken zum Einkauf
-   Stammdaten für den Einkauf
-   Bestellungen
-   Lieferungen im Wareneingang
-   Elektronischer Dokumentenaustausch

#### Vorausgesetzte Kenntnisse

Das Tutorial richtet sich an Teilnehmer, die in A+W Business den Einkauf abwickeln. Die Teilnehmer müssen das Konzept der Stammdaten in A+W Business und den Dialog Dokumentenverwaltung kennen.

#### Aufbau des Tutorials

Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

-   **Überblick:** Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
    -   Lernziele: Was soll vermittelt werden?
    -   Nutzen: Wofür können Sie dieses Wissen einsetzen?
    -   Merksätze: Welche Zusammenhänge müssen Sie sich merken?
-   **Konzepte:** Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.
-   **Übungen:** Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen und Lösungsvorschlägen.
-   **Querverweise:** Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf ergänzende Informationen in der Softwarereferenz und in anderen Parts hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.

#### Lesehinweis

Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.
Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

### Menü-Übersicht

In diesem Abschnitt finden Sie eine kurze Übersicht über die Programmbereiche, die in den Themenblöcken dieser Schulung angesprochen werden.
Im Menü Dokumente finden Sie auch die Programmbereiche, mit denen Sie den Verkauf abwickeln. Diese werden im Part Verkauf beschrieben.

*Abb. D-1 Modul Dokumente - Menü Bestellung*

**Bestellung**
In diesem Bereich erstellen und verwalten Sie Bestellungen.
⇨ "Bestellungen" auf Seite D-2077

**Nachbestellung**
In diesem Dialog verwalten Sie Aufträge mit Bestellteilen, die als Bruch gemeldet sind und entscheiden ob diese nachbestellt, reklamiert, verrechnet oder von der Auftragsmenge abgezogen werden sollen.
⇨ Softwarereferenz, "Nachbestellung" auf Seite D-2227

**Druck Bestellung**
In diesem Dialog drucken Sie die Bestellungen, die Sie an Lieferanten senden wollen. Diese Funktion ist ausführlich im Part Verkauf beschrieben.
⇨ Verkauf, "Druck" auf Seite C-1450

**Export**
In diesem Dialog exportieren Sie Bestellungen, um sie über die EDI-Schnittstelle an den betreffenden Lieferanten zu übertragen.
⇨ "Bestellung exportieren" auf Seite D-2216

**Journal**
In diesem Dialog verschaffen Sie sich einen Überblick über die Bestellungen. Diese Funktion ist ausführlich im Part Verkauf beschrieben.
⇨ Verkauf, "Journal" auf Seite C-1646

**AB Lieferant**
In diesem Dialog erfassen Sie die Auftragsbestätigungen, die Ihre Lieferanten gesendet haben.
⇨ "Lieferanten-AB" auf Seite D-2121

**Auftragsbestätigung**
In diesem Bereich prüfen Sie die Preise von Auftragsbestätigungen.
⇨ "Rechnung kontrollieren" auf Seite D-2180

**Wareneingang**
In diesem Bereich prüfen und erfassen Sie den Wareneingang zu Ihren Bestellungen.
⇨ "Wareneingang" auf Seite D-2154

**Rechnung**
In diesem Bereich erfassen und kontrollieren Sie die Lieferantenrechnungen.
⇨ "Elektronisches Dokument prüfen" auf Seite D-2204

**FiBu-Übergabe**
In diesem Dialog übergeben Sie die eingegangenen Rechnungen an Ihre Finanzbuchhaltung. Diese Funktion ist ausführlich im Part Verkauf beschrieben.
⇨ Verkauf, "Sollstellung FiBu" auf Seite C-1970

**Übergabe Archiv**
In diesem Dialog übergeben Sie Ihre Bestellungen an das Archiv. Diese Funktion ist ausführlich im Part Verkauf beschrieben.
⇨ Verkauf, "Übergabe Archiv" auf Seite C-1974

**Dokumentendaten**
In diesem Dialog können Sie sich Übersichten über Bestellungen und korrespondierende Aufträge anzeigen lassen und ggf. die Termine korrigieren. Diese Funktion ist ausführlich im Part Verkauf beschrieben.
⇨ Verkauf, "Dokumentendaten" auf Seite C-2030

**Lagersuche**
In diesem Dialog können Sie die Verfügbarkeit von Produkten prüfen und nach Lagermaßen suchen. Diese Funktion ist ausführlich im Part Verkauf beschrieben.
⇨ Verkauf, "Lagersuche" auf Seite C-2034

**Artikel-Info**
In diesem Dialog können Sie sich Informationen zu den Produkten anzeigen lassen, die in A+W Business angelegt sind. Sie können dabei den Produktaufbau, die Preise und die Verfügbarkeit prüfen. Diese Funktion ist ausführlich im Part Verkauf beschrieben.
⇨ Verkauf, "Artikel-Informationen" auf Seite C-1887

**Faxnachricht**
In diesem Dialog können Sie direkt aus A+W Business Faxnachrichten an Ihre Kunden und Lieferanten erstellen und versenden. Diese Funktion ist ausführlich im Part Überblick beschrieben.
⇨ Überblick: Tutorial, "Standard-Menüs" auf Seite A-66

### Grundgedanken zum Einkauf

Der Einkauf gehört zu den kaufmännischen Aufgaben im Unternehmen. Ein typischer Einkauf ist in A+W Business so oder ähnlich aufgebaut:

*Abb. D-2 Schema des Einkaufs in A+W Business (Eine Grafik, die den Fluss von Anfrage -> Bestellung -> AB+Preiskontrolle -> Wareneingang -> AB+Preiskontrolle zeigt. Parallel dazu geht ein Kunden-Auftrag in eine Übergabe, die ebenfalls in die Bestellung mündet. Vom Wareneingang gibt es Abzweigungen zu Lager und Produktion.)*

**Legende:**
-   **Dokument:** Blaue Boxen
-   **Bereich:** Gelbe Boxen
-   **optional:** Gestrichelte Linien

Alle kaufmännischen Vorgänge in A+W Business basieren auf den Stammdaten. Nur wenn diese korrekt gepflegt sind, kann der Einkauf problemlos abgewickelt werden:

-   **Anfrage:** Mit der Anfrage holen Sie Angebote Ihrer Lieferanten ein. Wenn Sie das Angebot überzeugt, können Sie aus der Anfrage direkt die Bestellung erzeugen, ohne die Daten erneut eingeben zu müssen.
    ⇨ "Anfrage" auf Seite D-2144
-   **Bestellung:** Als manuelle Bestellung erfassen Sie die Bestellpositionen und wählen den gewünschten Lieferanten aus. Die referenzierte Bestellung wird aus dem Kundenauftrag über den Bestellpool erzeugt.
    ⇨ "Manuelle Bestellung" auf Seite D-2113
-   **Auftragsbestätigung (AB) vom Lieferanten:** Sie erfassen die Nummer der AB und prüfen die Preise und Liefertermine. Bei Verzögerungen benachrichtigen Sie ggf. den Kunden. Geänderte und bestätigte Preise können in die EK-Kalkulation zurückgeschrieben werden.
    ⇨ "Auftragsbestätigung und Liefertermin" auf Seite D-2121
-   **Wareneingang:** Sie prüfen den Wareneingang und buchen automatisch die Lagerbestellungen in den Lagerbestand. Referenzierte Bestellungen werden als Eingang an die Produktion und/oder den Verkauf übergeben, um den zugehörigen Kundenauftrag weiterzubearbeiten oder abzuschließen.
    ⇨ "Wareneingang erfassen" auf Seite D-2161
-   **Rechnungskontrolle:** Sie prüfen die Rechnung und korrigieren ggf. Ihre Einkaufspreise, sofern Sie die geänderten Preise akzeptieren. Anschließend kann die Rechnung zur Anweisung freigegeben werden.
    ⇨ "Preis- und Rechnungskontrolle" auf Seite D-2177

#### Handlungsablauf im Einkauf

Üblicherweise bearbeiten Sie ein Einkaufsdokument in folgenden Schritten:
-   Anfrage erstellen (optional)
-   Bestellung
    -   Kopfdaten erfassen
    -   Positionen erfassen
    -   Stückliste bearbeiten
-   Bestellung drucken (senden per Fax, E-Mail, elektronisch)
-   Auftragsbestätigung vom Lieferanten erfassen
-   Preise prüfen
-   Termine und Tourenplanung nach Rückmeldungen korrigieren
-   Wareneingang erfassen
-   Rechnung prüfen
-   Übergabe an Archiv und Statistik
-   Dokument aus der Hauptdatenbank löschen

Wenn die Bestellung durch die Bestellübergabe aus einem Kundenauftrag erzeugt wurde, müssen die Daten nicht manuell erfasst werden.

> **Täglicher Arbeitsablauf**
> Am einfachsten gestalten Sie Ihren täglichen Arbeitsablauf über die Nummernverwalter. Leeren Sie dazu den entsprechenden Nummernverwalter oder legen Sie für den aktuellen Tag einen neuen an.
> Erstellen Sie dann die neuen Dokumente in diesem Nummernverwalter.
> Auf diese Weise behalten Sie am besten im Blick, welche Dokumente neu sind und weiterverarbeitet werden können oder müssen.

### Stammdaten für den Einkauf

In diesem Themenblock lernen Sie, wie Sie die Stammdaten für den Einkauf anpassen.
Dazu gehören folgende Lerneinheiten:
-   "Produktdefinition" auf Seite D-2055
-   "Lieferanten" auf Seite D-2064
-   "EK-Preise" auf Seite D-2070
-   "Dokumentenstatus" auf Seite D-2074

#### Produktdefinition

**Lernziele**
-   Stammdaten der Produkte für den Einkauf anpassen.
-   Beschaffungsarten für Bestellung kennenlernen.
-   Nutzen des Bestellkennzeichens im Auftrag kennenlernen.

**Nutzen**
-   Anhand des Bestellkennzeichens erkennt A+W Business die Produkte, die bestellt werden müssen.
-   Über das Bestellkennzeichen wird zu einem Kundenauftrag im Bestellpool automatisch eine Bestellung erzeugt. Die Bestellung muss daher nicht manuell erfasst werden.

**Merke**

| Begriff | Beschreibung |
| :--- | :--- |
| **Beschaffungsart** | Das Kennzeichen Beschaffungsart legt fest, wie das im Auftrag oder in der Bestellung erfasste Produkt beschafft werden soll, z. B. durch Produktion, Lagerentnahme, Bestellung. |
| **Bestellkennzeichen** | Als Bestellkennzeichen werden folgende Beschaffungsarten bezeichnet: <ul><li>Bestellung</li><li>Bestellung (komplett)</li></ul> |
| **Bestellung (komplett)** | Dieses Kennzeichen wird bei Produkten mit Stückliste verwendet, die als Ganzes bestellt werden sollen, z. B. eine komplette Tür mit Beschlägen. |
| **Bestellung** | Dieses Kennzeichen wird bei Produkten verwendet, deren einzelne Komponenten bestellt werden sollen, z. B. nur die Beschläge. |
| **Voreinstellungen** | Stammdaten<br>Produktverwaltung: <ul><li>Register Preis/Zuschlag</li><li>Register Lager/Einkauf</li></ul><br>Firmendaten: <ul><li>Register Lager/EK/EDI</li><li>Register Dokumente</li><li>Register Parameter</li><li>Register Kalkulation</li></ul> |

##### Bestellkennzeichen

Der Einkauf bezieht sich auf die Produkte, die in A+W Business verwaltet werden. Um ein Produkt einzukaufen, muss es in einer Bestellung erfasst werden.
Zu jedem Produkt legen Sie fest, wie es für die Preisberechnung, die Rabattfindung, die Fertigung oder Bestellung usw. herangezogen wird. Nur mit den entsprechenden Kennzeichen sind z. B. automatische Übergaben an die Schnittstellen, Berechnungen und Druck in den Dokumenten möglich.
Im Rahmen des Einkaufs muss die Beschaffungsart gesondert betrachtet werden, denn über sie erkennt A+W Business, wenn ein Produkt oder eine Komponente eines Produkts eingekauft werden muss.

-   **Bestellartikel (komplett):** Bestellung erfolgt inklusive aller Bearbeitungen, die in der Stückliste erfasst wurden. Besteht z. B. ein VSG aus einem Float 5 mm, einer Folie und einem ESG 5 mm, so wird das VSG als Ganzes bestellt. (Beachten Sie hierzu auch die Abgrenzung zu Bestellartikel.)
-   **Bestellartikel:** Nur das betreffende Produkt wird bestellt, ohne den Inhalt der Stückliste (z. B. Bearbeitungen) zu beachten. Besteht wiederum z. B. ein VSG aus einem Float, einer Folie und einem ESG und ist das Kennzeichen Bestellartikel nun für das ESG gesetzt, so wird nur das ESG beim Lieferanten bestellt. Das VSG wird in Eigenfertigung produziert.

Dieses Bestellkennzeichen wird automatisch in die Auftragsposition übernommen. Im Auftrag kann aber außerdem jeder Position ein Bestellkennzeichen zugeordnet werden.

##### Beschaffungsart

Diese Beschaffungsarten für die Bestellung (Bestellkennzeichen) werden in den Stammdaten der Produkte festgelegt. Es wird standardmäßig herangezogen, wenn ein Produkt im Dokument erfasst wird. Im Auftrag und in der Bestellung kann es überschrieben werden.

*Abb. D-3 Bestellkennzeichen in der Stückliste (Zeigt ein Diagramm, wie unterschiedliche Bestellkennzeichen (*, **) auf Komponenten einer ISO-Glaseinheit die Bestellung beeinflussen. `*` führt zur Bestellung der Komponente, `**` zur Bestellung der gesamten Einheit.)*

Wenn eine Hauptposition oder eine übergeordnete Stücklisten-Komponente mit der Beschaffungsart Bestellung (komplett) gekennzeichnet ist, werden die zugehörigen Stücklisten-Komponenten nicht vom Lager abgebucht, wenn deren Beschaffungsart auf Lagerentnahme eingestellt ist. Die Beschaffungsart dieser Komponenten kann dann nicht geändert werden.

Die Beschaffungsart kann pro Mandant und/oder AV-Bereich festgelegt werden. In diesem Fall muss in den Firmendaten die Option **Abweichende Beschaffungsart pro Mandant/AV-Bereich aktivieren** aktiviert werden.

*Abb. D-4 Firmendaten – Register Parameter (Screenshot zeigt die Aktivierungs-Checkbox)*

##### Preise und Zuschläge

Preistabellen werden sowohl für den Einkauf als auch für den Verkauf angelegt. Sie müssen jedem einzelnen Produkt zugewiesen werden, damit die entsprechenden Preise automatisch berechnet werden.

#### Stammdaten eines Produkts prüfen

Für den Einkauf müssen besonders all die Produktdaten vollständig erfasst sein, die standardmäßig bestellt werden.
Im Part Stammdaten ist ausführlich beschrieben, wie Sie die Stammdaten zu Ihren Produkten anlegen. In der folgenden Beschreibung wird daher nur auf die Besonderheiten eingegangen, die Sie für den Einkauf beachten müssen.

**So prüfen Sie die Stammdaten eines Produkts**
1.  Wählen Sie `Stammdaten > Produkte > Artikel > Artikel`. Der Dialog Produktverwaltung wird geöffnet.
    ⇨ Stammdaten, "Produktverwaltung - Lager/Einkauf" auf Seite B-723
2.  Suchen Sie das Produkt, das Sie prüfen möchten, und wechseln Sie zum Register **Preis/Zuschlag**.
    *Abb. D-5 Produktverwaltung – Preis/Zuschlag (Screenshot zeigt die Preisparameter eines Produkts, mit Markierungen für Verkauf (A) und Einkauf (B).)*
3.  Prüfen Sie, ob die Preistabellen und die Checkboxen **Preisrelevant für VK (A)** und **EK (B)** richtig gewählt sind.
    Die Checkbox Preisrelevant EK muss nur dann markiert sein, wenn Sie mit der EK-Kalkulation arbeiten.
    Weitere Informationen zu den Preisen finden Sie unter: "EK-Preise" auf Seite D-2070
4.  Wechseln Sie zum Register **Lager/Einkauf**.
    *Abb. D-6 Produktverwaltung – Lager/Einkauf (Screenshot zeigt die Bestell- und Lagerparameter, mit Auswahl der Beschaffungsart (A) und abweichenden Kennzeichen (B).)*
5.  Prüfen Sie, ob die **Beschaffungsart (A)** richtig eingestellt ist.
    Für Bestellartikel können Sie folgende Einträge auswählen:
    -   **Bestellung (komplett):** Produkt mit Stückliste und Produkt, das als Ganzes bestellt wird, z. B. eine komplette Tür mit Beschlägen.
    -   **Bestellung:** Produkt ohne Stückliste und Produkt, das als Stücklisten-Komponenten (ganz oder teilweise) bestellt wird.
6.  Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern.
    Die Daten werden gespeichert.

#### Lagermaß anlegen

Für die korrekte Preisberechnung können Sie Lagermaße zu den Produkten anlegen, z. B. Gläser mit festen Maßen. Wenn ein Produkt auch als Lagerartikel geführt werden soll, müssen Sie es außerdem in der Lagerverwaltung anlegen. Eine Beschreibung dazu finden Sie im Part Lagerwirtschaft.

**So legen Sie Lagermaße in den Stammdaten an**
1.  Wählen Sie `Stammdaten > Produkte > Artikel > Lagermaße`.
    Der Dialog Produktverwaltung Lagermaße wird geöffnet.
    ⇨ Stammdaten, "Lagermaße" auf Seite B-753
2.  Wählen Sie im Menü `Start > Neu`, um in den Erfassungs-Modus zu wechseln.
    *Abb. D-7 Felder für Lagermaß freigeschaltet (Screenshot des Dialogs mit Markierungen für Maße (A), Inhalt (B), Preistabellen (C) und Preisermittlung im Lager (D).)*
3.  Geben Sie die Maße (A) an.
    Falls Sie in der Lagerverwaltung bereits einen entsprechenden Lagerartikel definiert haben sollten, tragen Sie die gleichen Werte für Breite und Höhe ein.
4.  Wenn das Lagermaß als Kiste verwaltet wird, geben Sie an, wie viele Blätter (B) in der Kiste enthalten sind.
5.  Sie können zusätzlich folgende abweichende Angaben einstellen:
    -   Preisschlüssel (C) für den Verkauf und den Einkauf.
    -   Bezeichnung und Kurzbezeichnung (Matchcode), z. B. um den Lagerartikel besser identifizieren zu können.
    -   Beschaffungsart, z. B. Lagerentnahme bei Lagermaßen, die auch als Lagerartikeln vorhanden sind.
    Wenn Sie das Lagermaß auch als Lagerartikel anlegen wollen, müssen Sie entscheiden, ob die Preisermittlung auch im Lager durchgeführt werden soll.
6.  Markieren Sie die Checkbox **EK Suche Lager (D)**, wenn das Lagermaß in die Preisermittlung einbezogen werden soll.
    *Abb. D-8 Neues Lagermaß für die Preisberechnung*
7.  Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern.
    Die Daten werden gespeichert. Anschließend wird die Abfrage angezeigt, ob Sie dieses Lagermaß auch als Lagerartikel anlegen möchten.
8.  Wählen Sie `[Ja]`, wenn das Lagermaß auch als Lagerartikel verwaltet werden soll.
    Der Dialog **Lagerverwaltung** wird geöffnet. Wie Sie Lagerartikel anlegen, ist ausführlich im Part Lagerwirtschaft beschrieben.
    ⇨ Lagerwirtschaft, "Lagerartikel anlegen" auf Seite G-2749

#### Lieferanten

**Lernziele**
-   Lieferanten als Marktpartner anlegen.
-   Standard-Lieferant zuordnen.
-   Lieferantenkartei kennenlernen.

**Nutzen**
-   Bestellungen können über die hinterlegten Kommunikationswege direkt an den Lieferanten gesendet werden.
-   Standard-Lieferanten werden in der Bestellung automatisch erfasst. Sie können jedoch geändert werden, wenn dies erforderlich ist.
-   Über die Angaben zur Lieferdauer werden die Termine für Bestellungen und referenzierte Aufträge errechnet.

**Merke**

| Begriff | Beschreibung |
| :--- | :--- |
| **Marktpartner** | Alle Lieferanten werden im Dialog Partnerverwaltung angelegt. |
| **Lieferantenkartei** | In der Lieferantenkartei wird festgelegt, welche Lieferanten welche Produkte bzw. Warengruppen liefern. Diese Angaben werden u. a. für die Übergabe von Bestellpositionen an den Einkauf benötigt. |
| **Standard-Lieferant** | Wenn für ein Produkt oder eine Warengruppe mehrere Lieferanten eingetragen sind, wird ein Standard-Lieferant festgelegt. |
| **Voreinstellungen** | Stammdaten: <ul><li>Lieferantendaten (Marktpartner)</li><li>Lieferantenkartei</li></ul> |

##### Marktpartner Lieferant

Lieferanten werden in A+W Business angelegt, damit Bestellungen automatisiert abgearbeitet werden können. Bei der Erfassung von Aufträgen und Bestellungen müssen die Daten der Lieferanten daher nicht gesondert erfasst werden.
Lieferanten werden wie die Kunden im Dialog **Partnerverwaltung** angelegt. In den Stammdaten der Lieferanten müssen die Daten für die Kommunikation korrekt hinterlegt sein, damit Dokumente direkt aus A+W Business heraus versendet werden können.

##### Lieferantenkartei

In der Lieferantenkartei wird festgelegt, welche Lieferanten welche Produkte bzw. Warengruppen liefern. Werden für einen Lieferanten ein Produkt und die dazugehörigen Warengruppen angegeben, berücksichtigt die Bestellübergabe das Produkt vorrangig.
Die Angaben aus der Lieferantenkartei werden ignoriert, wenn im Dokumentenkopf zu einer Position oder zu einer Stücklisten-Komponente ein abweichender Lieferant eingegeben ist.
Wenn für ein Produkt mehrere Lieferanten angegeben sind, kann bei der Bestellübergabe ein Preisvergleich gestartet werden. Gleichzeitig wird die Lieferdauer angezeigt, so dass auch hinterlegte Lieferzeiten berücksichtig werden können.

##### Standard-Lieferant

Wenn ein Standard-Lieferant festgelegt ist, muss die Bestellung nicht über den Bestellpool gesendet werden. Der Standard-Lieferant wird mit der Rangnummer 1 gekennzeichnet, alle weiteren Lieferanten erhalten die Folgenummern in der Reihenfolge, die ihrer Bedeutung für den Einkauf entspricht.
Pro Produkt gibt es nur einen Standard-Lieferanten. Wenn aber ein bestimmtes Produkt in großer Stückzahl bestellt wird, die der Standard-Lieferant nicht produzieren kann, kann zusätzlich ein Standard-Lieferant für Serienaufträge angelegt werden. In der Auftragserfassung aktivieren Sie in einem solchen Fall den Dokumententyp **Serienauftrag**. Bei der Bestellübergabe wird dann automatisch der Lieferant für Serienaufträge herangezogen.

#### Stammdaten eines Lieferanten prüfen

Damit die Bestellungen korrekt abgewickelt werden können, müssen Sie die Stammdaten eines Lieferanten und die Zuordnung von Produkten zu Lieferanten einrichten.
Im Part Stammdaten ist ausführlich beschrieben, wie Sie die Stammdaten zu Ihren Partnern anlegen. In der folgenden Beschreibung wird daher nur auf die Besonderheiten eingegangen, die Sie für den Einkauf beachten müssen.

**So prüfen Sie die Stammdaten der Lieferanten**
1.  Wählen Sie `Stammdaten > Marktpartner > Lieferant > Lieferanten`.
    ⇨ Stammdaten, "Partnerverwaltung" auf Seite B-884
2.  Suchen Sie den Lieferanten, dessen Daten Sie prüfen wollen.
    *Abb. D-9 Stammdaten - Lieferanten (Screenshot des Partnerverwaltungsdialogs, mit Markierungen für E-Mail-Adresse (A) und Sprache für Formulare (B).)*
3.  Prüfen Sie im Register **Adresse**, ob die Daten für den Schriftverkehr und die Kommunikation vollständig und aktuell sind.
    Die E-Mail-Adresse kann auch für den Austausch von elektronischen Dokumenten genutzt werden, z. B. von PDF-Dateien. Achten Sie auf die korrekte und vollständige Schreibweise.
4.  Wechseln Sie zum Register **Auftrag** und prüfen Sie, ob der Dokumentenversand richtig aktiviert ist.
    *Abb. D-10 Fax- und E-Mail-Versand (Beispiel für Einstellungen)*
5.  Wählen Sie im Menü `Start > Speichern`, um die Änderungen zu speichern.
    Die Daten werden gespeichert.

#### Lieferantenkartei anpassen

In der Lieferantenkartei legen Sie fest, welche Lieferanten welche Produkte bzw. Warengruppen liefern und wie lange die Lieferzeiten sind.

**So prüfen Sie die Lieferantenkartei**
1.  Wählen Sie `Stammdaten > Marktpartner > Lieferant > Kartei`.
    Der Dialog Lieferantenkartei wird mit dem Register **Produkte** geöffnet.
2.  Wählen Sie im Menü `Start > Filter`, um in den Such-Modus zu wechseln.
    *Abb. D-11 Lieferantenkartei – Produktsuche (Screenshot der Suchmaske mit Optionen für Produkt (A) und Varianten (B).)*
3.  Wählen Sie die Option **Produkt (A)** und tragen Sie die Nummer des Produkts ein.
4.  Wählen Sie im Menü `Start > Suchen`, um in die Suche zu starten.
    Im Bereich **Produkt - Lieferanten** werden alle Lieferanten aufgeführt, die das gewählte Produkt liefern können. Mit dem Rang 1 ist der Standard-Lieferant gekennzeichnet.
    *Abb. D-12 Lieferantenkartei - Produkte (Screenshot zeigt eine Liste von Lieferanten für ein Produkt mit abweichenden Bezeichnungen (A), Lieferzeit (B), Standard-Lieferant Rang 1 (C) und Rangfolge-Pfeilen (D).)*
5.  Tragen Sie die Anzahl (B) der Tage ein, die zur Berechnung der Lieferzeit herangezogen werden soll.
    Die Lieferzeit wird bei der Bestellübergabe im Preisvergleich und bei der Lieferterminkontrolle berücksichtigt.
6.  Prüfen Sie die Rangfolge der Lieferanten und korrigieren Sie diese ggf., indem Sie einen Eintrag markieren und mit den Pfeilschaltflächen (D) nach oben oder unten verschieben.
    Die Rangnummer 1 (C) bezeichnet den Standard-Lieferanten. Er wird automatisch bei Bestellungen eingesetzt, die nicht im Bestellpool geprüft werden.
7.  Wenn Ihr Lieferant abweichende Produktbezeichnungen benutzt, tragen Sie diese ein (A).
    Diese Bezeichnungen werden in der Bestellung aufgeführt und helfen, Missverständnisse zu vermeiden.
8.  Wählen Sie im Menü `Start > Speichern`, um die Änderungen zu speichern.
    Wenn Sie ganze Warengruppen prüfen möchten, wechseln Sie zum Register **Warengruppen** und verfahren analog.

#### EK-Preise

**Lernziele**
-   Preisjahrgang, Preisschlüssel und Tarife für Einkaufspreise (EK) kennenlernen.
-   EK-Preise bearbeiten.

**Nutzen**
-   Einkaufspreise werden bei der Erfassung von Aufträgen und Bestellungen berechnet, so dass der Deckungsbeitrag automatisch berechnet werden kann.
-   EK-Preise können in der Bestellung überschrieben werden.

**Merke**

| Begriff | Beschreibung |
| :--- | :--- |
| **Preisliste** | Preisjahrgänge, -schlüssel und Tarife bilden den Rahmen für die Preislisten. |
| **Individualpreise** | Individuelle Preise von Lieferanten können Sie mit allen Bezugsgrößen einrichten, die auch für die allgemeinen Preislisten und Zuschläge gelten. |
| **Voreinstellungen** | Stammdaten: <ul><li>Jahrgang</li><li>Schlüssel</li><li>Tarife</li><li>Preise</li></ul> Firmendaten: <ul><li>Register Lager / EK / EDI</li><li>Register Preisberechnung</li><li>Register Fibu</li></ul> Referenzen: Preisimport VEGLA<br>Utilities: Preislistenimport |

##### Preislisten

Die Preisberechnung in A+W Business ist aus flexiblen Bausteinen zusammengesetzt, die alle Berechnungsmöglichkeiten abdecken. Sie können jedem Produkt die passende Art der Preisberechnung zuordnen.
Preisjahrgänge, -schlüssel und Tarife bilden den Rahmen für die Preislisten. In den Preistabellen selbst sind die Beträge hinterlegt, die in den Dokumenten herangezogen werden.
Preise legen Sie als Standard-Preislisten oder als Preislisten für bestimmte Kunden- oder Lieferantengruppen, für einzelne Kunden oder für einzelne Lieferanten fest.
Im Einkauf arbeiten Sie in der Regel nur mit einem Preisschlüssel, z. B. dem Schlüssel EK. Sie können aber auch im Einkaufsbereich nach verschiedenen Preisschlüsseln differenzieren.

Bei der Preisfindung wird folgende Hierarchie durchlaufen:
1.  Manuelle Preiseingaben im Auftrag oder Angebot (oberste Priorität)
2.  Objektbezogene Vereinbarungen
3.  Kunden-/lieferantenbezogene Vereinbarungen
4.  Gruppenspezifische Vereinbarungen
5.  Allgemeine Vereinbarungen

Innerhalb dieser Hierarchiestufen können allgemeine Preise, Sonderbedingungen für Warengruppen und einzelne Produkte, Austauschpreise und Zuschläge für Modelle und Sprossen hinterlegt werden.

##### Individualpreise

Bei der Gestaltung individueller Preise für Kunden und Lieferanten können Sie alle Bezugsgrößen nutzen, die auch für die allgemeinen Preislisten und Zuschläge gelten. So können Sie entweder Preistabellen für Ihre einzelnen Kunden oder Lieferanten anlegen oder die Preise im Dokument vereinbarungsgemäß anpassen.

##### Preislistenimport

Preislisten Ihrer Lieferanten können Sie importieren, wenn diese als Datei vorliegen.

> **Historie der Preisänderungen**
> Wenn Sie mit einer Gupta-Datenbank arbeiten, können Sie Änderungen der Preise in einer Historie verfolgen. Diese Funktion ist im Part Stammdaten beschrieben.

#### Stammdaten der Preise prüfen

In Bestellungen können die Preise nur berechnet werden, wenn die Einkaufspreise korrekt sind. Im Part Stammdaten ist ausführlich beschrieben, wie Sie die Stammdaten zu Ihren Preisen anlegen. In der folgenden Beschreibung wird daher nur auf die Besonderheiten eingegangen, die Sie für den Einkauf beachten müssen.

**So prüfen Sie die Stammdaten Ihrer Preislisten**
1.  Wählen Sie `Stammdaten > Preise > Preise` und prüfen Sie, ob der Jahrgang, der Schlüssel und der Tarif für die Einkaufspreise (EK) richtig definiert sind.
2.  Wechseln Sie zum Dialog Preise und lassen Sie sich die Tabelle und den Tarif für die EK-Preise anzeigen.
    Wenn Sie die Suche nicht einschränken, werden alle Preistabellen aufgelistet.
    *Abb. D-13 EK-Preistabellen - Preisauswahl (Screenshot zeigt die Preisauswahl mit Markierung für Einzelpreis (A) und Preistabelle (B).)*
    ⇨ Stammdaten, "Preise - Preisauswahl" auf Seite B-840
3.  Markieren Sie die Preistabelle (B), die Sie prüfen wollen, und wechseln Sie zu dem Register, in dem der Preis festgelegt ist.
    In diesem Beispiel ist der Einzelpreis (A) geprüft.
    *Abb. D-14 Preisauswahl – Einzelpreis (Screenshot zeigt die Detailansicht eines Einzelpreises mit Preis (A), Preiseinheit (B) und Währung (C).)*
    In der Übersicht sind alle Tarife der ausgewählten Preistabelle aufgeführt. Die nicht definierten Preise sind in roter Schrift angezeigt.
4.  Prüfen Sie, ob der Preis auf dem aktuellen Stand ist, oder korrigieren Sie ihn. Setzen Sie dazu den Cursor in die Zelle Preis und überschreiben Sie den Eintrag.
5.  Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern.
    Die Daten werden gespeichert.

**Ergänzende Informationen**
-   ⇨ Stammdaten, "Stammdaten für Preise" auf Seite B-276
-   ⇨ Stammdaten, "Einzelpreise anlegen" auf Seite B-301
-   ⇨ Stammdaten, "Firmendaten - Kalkulation" auf Seite B-1120

#### Dokumentenstatus

**Lernziele**
-   Statusumsetzung von referenzierten Dokumenten kennenlernen.
-   Statuszuordnung prüfen.

**Nutzen**
-   Statuszuordnungen für referenzierte Dokumente werden neben den Statuszuordnungen für unabhängige Dokumente gepflegt. Anhand des Status kann also erkannt werden, ob eine Bestellung referenziert ist.
-   Wareneingänge zu einer Bestellung setzen den Status des referenzierten Auftrags um. So kann am Auftrag der aktuelle Stand erkannt werden.

**Merke**

| Begriff | Beschreibung |
| :--- | :--- |
| **Statuszuordnungen** | Statuszuordnungen für referenzierte Dokumente müssen den gleichen Mindeststatus haben. |
| **Statusumsetzung** | Der Status des referenzierten Auftrags wird beim Wareneingang der Bestellung umgesetzt. |
| **Voreinstellungen** | Stammdaten: <ul><li>Statuszuordnung</li></ul> |

##### Statuszuordnung

Die Einkaufsdokumente durchlaufen von der Erfassung bis zur Archivierung mehrere Programmpunkte, die jeweils durch einen Status gekennzeichnet sind. An diesen Status können Bedingungen und Sperren geknüpft sein.
Wie Sie die Statuspunkte und -zuordnungen einrichten, hängt von den Geschäftsabläufen in Ihrem Unternehmen ab. Eine ausführliche Beschreibung finden Sie dazu im Part Stammdaten.

*Abb. D-15 Statuszuordnung für referenzierte Dokumente (Screenshot zeigt die Statuszuordnung mit einem Status für einen Auftrag mit referenzierter Bestellung (A) und dem korrespondierenden Status für die Bestellung selbst (B).)*

Statuszuordnungen werden für referenzierte Dokumente und für unabhängige Dokumente getrennt eingerichtet, z. B. für den Wareneingang.

##### Statusvergabe

Der Status der Dokumente wird in der Regel umgesetzt, wenn eine Bestellung geändert, versendet usw. wird. Dabei wird unterschieden, ob die Bestellung durch einen Auftrag oder unabhängig erzeugt wurde.

**Beispiele**

| für Aufträge | für Bestellungen |
| :--- | :--- |
| 30 - Auftrag in Einkauf übergeben | |
| 31 - AB Lieferant teilweise/Auftrag | 62 - AB Lieferant teilweise/Bestellung |
| 32 - AB Lieferant komplett/Auftrag | 63 - AB Lieferant komplett/Bestellung |
| 33 - Wareneingang teilweise/Auftrag | 64 - Wareneingang teilweise/Bestellung |
| 34 - Wareneingang komplett/Auftrag | 65 - Wareneingang komplett/Bestellung |
| | 66 - Rechnungskontrolle |

Wenn im Wareneingang die Nummer der Auftragsbestätigung (AB) des Lieferanten eingegeben ist, wird der Status der Bestellung umgesetzt.
Wenn ein Wareneingang zu einer Bestellung aus einem Kundenauftrag (referenzierte Bestellung) verbucht wird, zu dem weitere Bestellungen noch offen sind, wird der Status des Auftrages auf **Wareneingang teilweise/Auftrag** gesetzt.

**Ergänzende Informationen**
-   Verkauf, "Status" auf Seite C-1481
-   Stammdaten, "Geschäftsabläufe abbilden" auf Seite B-493
-   Stammdaten, "Statuszuordnung" auf Seite B-1022

### Bestellungen

In diesem Themenblock lernen Sie, wie Sie Bestellungen erzeugen und Termine prüfen.
Dazu gehören folgende Lerneinheiten:
-   "Bestellübergabe vs. manuelle Bestellung" auf Seite D-2078
-   "Bestellpositionen im Auftrag" auf Seite D-2084
-   "Bestellübergabe" auf Seite D-2094
-   "Manuelle Bestellung" auf Seite D-2113
-   "Auftragsbestätigung des Lieferanten" auf Seite D-2120
-   "Lieferterminkontrolle" auf Seite D-2134
-   "Anfrage" auf Seite D-2144

Üblicherweise erfassen Sie eine Bestellung in folgenden Schritten:
1.  Anfrage erstellen (optional)
2.  Bestellung erfassen
3.  Bestellung an den Lieferanten senden
4.  Auftragsbestätigung vom Lieferanten erfassen
    -   Preise prüfen
    -   Termine und Tourenplanung nach Rückmeldungen korrigieren
    -   Kunden über Terminänderungen informieren
5.  Auftragsbestätigung des Lieferanten anmahnen

Diese Reihenfolge entspricht im Wesentlichen auch der Reihenfolge der Dialoganordnung in A+W Business. Einige der Schritte können jedoch über mehrere Dialoge ausgeführt werden. Sie sind daher in einer Lerneinheit zusammengefasst.
Die Preise können bereits auf einer Auftragsbestätigung des Lieferanten geprüft werden. In der Praxis kann durchaus vorkommen, dass Auftragsbestätigung und Lieferung zusammen mit der Rechnung eintreffen. Da die Dialoge für die Preiskontrolle und die Rechnungskontrolle identisch sind, wird das Konzept der Preis- und Rechnungskontrolle im Themenblock Wareneingang beschrieben.
⇨ "Eingangsrechnung" auf Seite D-2178

Eine Anfrage wird logischerweise vor der Bestellung erstellt, sie ist jedoch nicht zwingend erforderlich. In diesem Tutorial wird die Anfrage nach den Bestellungen behandelt, weil Sie dann bereits mit allen Details der Bestellung vertraut sind.

#### Bestellübergabe vs. manuelle Bestellung

**Lernziele**
-   Unterschied zwischen automatischer (referenzierter) und unabhängiger Bestellung kennenlernen.

**Nutzen**
-   Auftragspositionen, die bestellt werden müssen, können automatisch in eine (referenzierte) Bestellung geleitet werden.
-   Lagerbestände werden durch Lagerbestellungen ergänzt. Diese werden manuell erfasst. Sie können auch durch Unterschreitung von Mindestbeständen angelegt werden. (Diese Funktion ist im Part Lagerwirtschaft beschrieben.)

**Merke**

| Begriff | Beschreibung |
| :--- | :--- |
| **Bestellung aus Auftrag** | Auftragspositionen, die bestellt werden müssen, werden im Bestellpool an den Einkauf übergeben. Mit der Übergabe wird automatisch eine Bestellung erzeugt. |
| **Referenzierte Bestellung** | Aus einer Auftragsposition, die an den Einkauf übergeben wurde, wird eine referenzierte Bestellung mit einer eigenen Dokumentennummer erzeugt. |
| **Unabhängige Bestellung** | Unabhängige Bestellungen werden manuell erfasst. Bei unabhängigen Bestellungen wird der Lagerbestand nicht aktualisiert, wenn der Wareneingang gebucht wird. |
| **Lagerbestellung** | Lagerbestellungen dienen dazu, den Lagerbestand aufzufüllen. Sie können manuell erfasst werden. |
| **Voreinstellungen** | Stammdaten: <ul><li>Lieferantendaten (Marktpartner)</li><li>Lieferantenkartei</li></ul> Firmendaten: <ul><li>Register Dokumente</li><li>Register Parameter</li><li>Register Lager/EK/EDI</li></ul> |

##### Dokument Bestellung

Bestellungen können entweder auftragsabhängig oder unabhängig eingegeben werden:
-   **Auftragsabhängige (referenzierte) Bestellungen** beziehen sich auf eine Position im Kundenauftrag. Sie werden durch die Bestellübergabe erzeugt. Im Bestellpool schlägt A+W Business aufgrund der Daten aus der Lieferantenkartei einen Lieferanten vor.
-   **Unabhängige Bestellungen** dienen in der Regel nicht dazu, den Lagerbestand aufzufüllen, da der Wareneingang nicht automatisch den Lagerbestand aktualisiert. Sie werden manuell erfasst.
-   **Lagerbestellungen** dienen dazu, den Lagerbestand aufzufüllen. Sie können manuell erfasst oder durch Unterschreitung eines Mindestbestands erzeugt werden.

*Abb. D-16 Arten der Bestellung (Diagramm zeigt, dass auftragsabhängige und unabhängige Bestellungen in den Wareneingang und dann in den Auftrag fließen, während manuelle und automatische Lagerbestellungen den Lagerbestand beeinflussen.)*

In dieser vereinfachten Darstellung sehen Sie, wozu die unterschiedlichen Bestellungen erfasst werden. In den folgenden Einheiten werden die auftragsabhängigen und die unabhängigen Bestellungen ausführlich beschrieben.
Lagerbestellungen werden ausführlich im Part Lagerwirtschaft beschrieben.

Alle Bestellungen sind eigene Dokumente mit einem eigenen Nummernkreis. Sie werden im Dialog zur Dokumentenverwaltung angezeigt und können unabhängig davon, wie sie erzeugt wurden, bearbeitet werden.
*Abb. D-17 Dokument Bestellung (Screenshot des Kopfdatendialogs einer Bestellung, der Anliefertermine (A), Zusatzinformationen (B) und den Dokumententyp (C) zeigt.)*
Bestellungen müssen an den Lieferanten gesendet werden. Dazu steht neben dem Fax- und dem E-Mail-Versand auch die Datenübertragung über Schnittstellen zur Verfügung.

#### Voreinstellungen für Bestellungen prüfen

Für die Bestellungen müssen Sie die Voreinstellungen in den Firmendaten prüfen. Im Part Stammdaten ist ausführlich beschrieben, wie Sie die Stammdaten zu Ihrer Firma einrichten. In der folgenden Beschreibung wird daher nur auf die Besonderheiten eingegangen, die Sie für den Einkauf beachten müssen.

> **A+W Business neu starten**
> Nach Änderungen der Firmendaten sollten Sie A+W Business neu starten.

**So prüfen Sie die Einstellungen für Bestellungen**
1.  Wählen Sie `Stammdaten > Firma > Firmendaten`.
    Der Dialog Firmendaten wird geöffnet.
    ⇨ Stammdaten, "Firmendaten" auf Seite B-1055
2.  Wechseln Sie zum Register **Dokumente** und prüfen Sie die Einstellungen für den Fax- und E-Mail-Versand.
    *Abb. D-18 Firmendaten - Dokumente (Screenshot zeigt Fax- (A) und E-Mail-Optionen (B) sowie das Dateiformat (C) für Anhänge.)*
3.  Wechseln Sie zum Register **Parameter** und prüfen Sie die Einstellungen wie in der folgenden Abbildung gezeigt.
    *Abb. D-19 Firmendaten - Parameter (Screenshot zeigt diverse Parameter, u.a. für die Rückschreibung von Änderungen (A), Übernahme von Bestelltexten (B), automatische Bestellkennzeichnung (C) und virtuelle Positionsnummern für Kisten (D).)*
    Die Einstellungen werden in separaten Einheiten ausführlich beschrieben.
    -   Checkbox A: ⇨ "Bestellte Auftragsposition ändern" auf Seite D-2091
    -   Checkboxen B und D: ⇨ "Kistengeschäft" auf Seite D-2170, ⇨ "Export/Import (openTRANS)" auf Seite D-2185
    -   Lagerbestellungen (C) sind ausführlich im Part Lagerwirtschaft beschrieben.
4.  Wechseln Sie zum Register **Lager/EK/EDI** und prüfen Sie die Einstellung im Bereich **Einkauf**.
    *Abb. D-20 Firmendaten – Lager/EK/EDI (Screenshot zeigt Einstellungen für ISO-Bestellartikel (A) und die Anzeige von Positionen aus Lagerbestellungen (B).)*
5.  Markieren Sie die Checkbox **ISO als Bestellartikel (Bearb. können Eigenfertigung sein) (A)**.
    Wenn bei Isolierglas (ISO) Bearbeitungen mit der Beschaffungsart Produktion (Eigenfertigung) in der Stückliste vorhanden sind, können diese mit bestellt werden. Diese Einstellung ist sinnvoll, wenn Sie ISO-Einheiten nur bei Engpässen in der Produktion bestellen.
6.  Wählen Sie im Menü `Start > Speichern`, um die Änderungen zu speichern.
    Die Daten werden gespeichert.

#### Bestellpositionen im Auftrag

**Lernziele**
-   Bestellposition erfassen und Kennzeichen zuordnen.
-   Lieferanten in der Auftragsposition ändern.
-   Lieferanten für den gesamten Auftrag ändern.
-   Bestellte Position ändern.

**Nutzen**
-   Aus Auftragspositionen können Bestellungen erzeugt werden, ohne die Positionen als Bestellung neu zu erfassen.

**Merke**

| Begriff | Beschreibung |
| :--- | :--- |
| **Bestellposition** | Bestellpositionen aus Aufträgen erzeugen pro Standard-Lieferant eine eigene Bestellung. |
| **Bestellkennzeichen** | Als Bestellkennzeichen werden folgende Beschaffungsarten bezeichnet: <ul><li>Bestellung</li><li>Bestellung (komplett)</li></ul> |
| **Bestellung (komplett)** | Dieses Kennzeichen wird bei Produkten mit Stückliste verwendet, die als Ganzes bestellt werden sollen, z. B. eine komplette Tür mit Beschlägen. |
| **Bestellung** | Dieses Kennzeichen wird bei Produkten verwendet, deren einzelne Komponenten bestellt werden sollen, z. B. nur die Beschläge. |
| **Voreinstellungen** | Stammdaten: <ul><li>Lieferantendaten (Marktpartner)</li><li>Lieferantenkartei</li></ul> Firmendaten: <ul><li>Register Dokumente</li><li>Register Parameter</li><li>Register Lager/EK/EDI</li></ul> |

##### Kundenbestellung

Im Kundenauftrag können Positionen enthalten sein, die aus unterschiedlichen Gründen bestellt werden müssen, z. B., weil das Produkt nicht im Lager geführt wird oder weil Engpässe in der Produktion den Liefertermin gefährden und darum die Position komplett bestellt werden muss. Grundsätzlich kann also jede Position eines Auftrags bestellt werden.
Bestellungen zu Auftragspositionen können aus den Aufträgen heraus erzeugt werden. Dazu muss mindestens eine Stücklisten-Komponente oder die gesamte Position als Bestellung gekennzeichnet sein.
Bestellungen werden nicht automatisch an den Einkauf übergeben. Sind Bestellartikel in einem Auftrag enthalten, können Sie sich dies durch eine Meldung anzeigen lassen, wenn Sie die Positionserfassung schließen.

*Abb. D-21 Bestellkennzeichen für Stücklisten-Komponente (Screenshot einer Auftragsposition, bei der eine Komponente (A) die Beschaffungsart "Bestellung" (B) erhält.)*

Für die Bestellpositionen in einem Auftrag wird ein neues Dokument erzeugt: eine Bestellung. Dieses Dokument wird durch die Übergabe des Auftrags an den Einkauf erzeugt. Die Bestellübergabe ist einer separaten Einheit beschrieben.
⇨ "Bestellübergabe" auf Seite D-2094
Sind in einem Auftrag verschiedene Bestellpositionen enthalten, werden so viele Bestellungen erzeugt, wie unterschiedliche Standard-Lieferanten aus der Lieferantenkartei ausgelesen wurden.

##### Lieferant für Auftragsposition

Achten Sie im Auftrag darauf, dass Sie für Bestellartikel den gewünschten Lieferanten auswählen. Sie haben dazu verschiedene Möglichkeiten:
-   **Dokumentenerfassung - Register Konditionen:** Diese Einstellung gilt übergreifend für alle Positionen im aktuellen Auftrag, sofern sie nicht (anschließend) auf den Ebenen der Position oder der Stückliste überschrieben werden.
-   **Positionserfassung - Register Zusatz:** Diese Einstellung gilt nur für die jeweils markierte Position.
-   **Positionserfassung - Register Stückliste:** Diese Einstellung gilt nur für die jeweils markierte Stücklisten-Komponente.
-   **Bestellübergabe:** Wenn bei den oben genannten Möglichkeiten keine Angaben gemacht sind, wird in der Bestellung automatisch der Standard-Lieferant eingesetzt. Die Einstellungen aus dem Auftrag und/oder den Produktstammdaten können im Bestellpool überschrieben werden.

Die Bestellübergabe ist einer separaten Einheit beschrieben.
⇨ "Bestellübergabe" auf Seite D-2094

##### Änderung in bestellten Positionen

Auftragspositionen, die bereits bestellt wurden, werden für die weitere Bearbeitung gesperrt. Sie können nachträglich in der Positionserfassung des Auftrags (oder der Bestellung) erst geändert werden, wenn die Sperrung manuell aufgehoben wird. Änderungen können sich z. B. auf Preise, Mengen oder Maße beziehen. Der Tarif kann trotz der Sperrung geändert werden.
Die Änderungen müssen in die referenzierten Bestellungen übernommen werden. Wenn Sie Maße oder Stückzahl einer bestellten Position ändern, können Sie die Änderungen in der ursprünglichen Bestellung eintragen. Die Bestellung muss dann mit einem Hinweis auf die Änderungen erneut an den Lieferanten gesendet werden.
Der geänderte Auftrag muss anschließend wieder über den Bestellpool an den Einkauf übergeben werden.

#### Bestellposition im Auftrag erfassen

In einer Auftragsposition können Komponenten oder ganze Positionen erfasst sein, aus denen eine Bestellung erzeugt werden muss. Dazu muss die richtige Beschaffungsart (Bestellkennzeichen) zugewiesen sein.

**So erfassen Sie im Auftrag eine Position zur Bestellung**
1.  Erfassen Sie den Auftragskopf und wechseln Sie zum Register Positionen.
2.  Erfassen Sie das Produkt, das Ihr Kunde haben möchte.
    *Abb. D-22 Bestellposition im Auftrag (Screenshot zeigt eine neu erfasste Auftragsposition (B) und die zugewiesene Beschaffungsart "Bestellung (komplett)" (A).)*
3.  Prüfen Sie die korrekte Einstellung der Beschaffungsart (A).
4.  Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern.
5.  Erfassen Sie eine weitere Position, in der jedoch nur eine Komponente der Stückliste bestellt werden soll.
6.  Wechseln Sie zum Register Stückliste.
    *Abb. D-23 Beschaffungsart für Stücklisten-Komponente (Screenshot zeigt eine Stücklisten-Komponente (A), für die der Lieferant (B) und die Beschaffungsart (C) geändert werden.)*
7.  Markieren Sie die Komponente (A), die bestellt werden muss.
8.  Wählen Sie die Beschaffungsart (C) und den Lieferanten (B) aus.
9.  Wählen Sie im Menü `Start > Speichern`, um die Änderungen zu speichern.
    Sie können jetzt weitere Positionen erfassen oder die erfassten Positionen ändern.
    Wenn Sie alle Bestellpositionen bei demselben Lieferanten bestellen wollen, wählen im Auftragskopf Sie im Register **Konditionen** den neuen Lieferanten aus.
    ⇨ "So ändern Sie den Lieferanten aller Bestellpositionen" auf Seite D-2090
10. Schließen Sie die Positionserfassung.
    Wenn für die Bestellpositionen kein Standard-Lieferant angegeben war, muss der Lieferant im Dialog **Bestellübergabe – Bestellpool** angegeben werden.
    ⇨ "So erzeugen Sie eine Bestellung zu einem Kundenauftrag" auf Seite D-2102

#### Lieferanten im Auftrag ändern

Sie können im Auftragskopf einen anderen Lieferanten für die Bestellungen auswählen. Dieser Lieferant gilt dann für alle Bestellpositionen des Auftrags.

> **Bestellkennzeichen im Nummernverwalter ändern**
> Wenn Sie in mehreren Aufträgen das Bestellkennzeichen ändern müssen, können Sie diese Aufträge in einem neuen Nummernverwalter sammeln. In diesem Nummernverwalter können Sie über das Menü `Funktionen > Kennzeichenänderung` die Beschaffungsart und den Lieferanten für alle Dokumente gemeinsam ändern.

**So ändern Sie den Lieferanten aller Bestellpositionen**
1.  Öffnen Sie den Auftrag mit den Bestellpositionen.
2.  Wechseln Sie zum Register **Konditionen**.
    *Abb. D-24 Auftragskopf – Register Konditionen (Screenshot des Auftragskopfs, der das Feld zur Auswahl eines Lieferanten (A) für alle Bestellpositionen zeigt.)*
3.  Wählen Sie den gewünschten Lieferanten (A) aus.
4.  Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern.
5.  Die Abfrage wird angezeigt: Soll das Bestellkennzeichen komplett für alle Positionen gesetzt werden. Wählen Sie:
    -   `[Ja]`: Der gesamte Auftrag wird an den Einkauf zur Bestellung bei dem gewählten Lieferanten übergeben.
    -   `[Nein]`: Nur die Bestellpositionen werden an den Einkauf übergeben.
6.  Schließen Sie den Auftrag.
    Sie können jetzt die Bestellungen an den Einkauf übergeben.
    ⇨ "So erzeugen Sie eine Bestellung zu einem Kundenauftrag" auf Seite D-2102

#### Bestellte Auftragsposition ändern

Sie können eine bestellte Position im Auftrag nachträglich ändern und die Bestellung neu erzeugen. Vergessen Sie dabei nicht, dem Lieferanten deutlich zu machen, welche Bestellung neu ist und welche frühere Bestellung durch sie ersetzt wird.

> **Bestellte Position ändern**
> Sie können eine bestellte Position nur so lange ändern, wie keine Auftragsbestätigung des Lieferanten oder ein Wareneingang erfasst wurde oder ein Sperrstatus erreicht ist.

**So ändern Sie eine bestellte Position**
1.  Öffnen Sie das Dokument, in dem Sie eine bestellte Position ändern möchten, und wechseln Sie zur Positionserfassung.
2.  Markieren Sie die Position, die Sie ändern wollen.
    *Abb. D-25 Beschaffungsart für Stücklisten-Komponente (Screenshot der Positionserfassung, der eine gesperrte Position (B) und einen gesperrten Produktaufbau (A) zeigt. Ein Hinweis besagt, dass die Position bestellt ist.)*
    Die Felder (A) der bestellten Positionen sind gesperrt. In der Spalte **Hinweis (B)** wird der entsprechende Text angezeigt.
3.  Wählen Sie im Menü `Funktionen > Gruppe Position > Gesperrte Position ändern`.
    Die Felder werden freigeschaltet.
4.  Geben Sie die Änderungen ein, z. B. die Stückzahl.
5.  Wählen Sie im Menü `Start > Speichern`, um die Änderung zu speichern.
    Die Änderungen werden gespeichert. Sie können weitere Änderungen eintragen.
6.  Schließen Sie die Positionserfassung.
    Der Dialog **Bestellübergabe – Bestellpool** wird geöffnet und Sie können die Bestellungen an den Einkauf übergeben.
    ⇨ "So erzeugen Sie eine Bestellung zu einem Kundenauftrag" auf Seite D-2102
    *Abb. D-26 Bestellübergabe - Bestellpool*
7.  Übergeben Sie die geänderte Bestellung wie unter Bestellung übergeben beschrieben.
    ⇨ "Dokument in den Bestellpool stellen" auf Seite D-2102

> **Lieferanten informieren**
> Vergessen Sie nicht, Ihren Lieferanten über die Änderung zu informieren, wenn Sie die ursprüngliche Bestellung bereits an ihn weitergeleitet hatten.

#### Bestellübergabe

**Lernziele**
-   Auftrag mit Bestellpositionen in den Bestellpool stellen.
-   Bestellpositionen im Bestellpool prüfen.
-   Lieferant und Liefertermin ändern.
-   Bestellpositionen an den Einkauf übergeben.

**Nutzen**
-   Auftragspositionen können direkt an den Einkauf übergeben werden. Die Bestellpositionen brauchen nicht im Bestellpool geprüft zu werden.
-   Im Bestellpool kann ein Preisvergleich geöffnet werden, um den günstigsten (oder schnellsten) Lieferanten auszuwählen.
-   Termine, Preise und Lieferanten von Bestellungen können vor der Übergabe geprüft werden.

**Merke**

| Begriff | Beschreibung |
| :--- | :--- |
| **Bestellübergabe** | Durch die Bestellübergabe werden die Bestellungen zu Auftragspositionen erzeugt. Die Übergabe einer Bestellung muss manuell angestoßen werden. Aus dem Bestellpool werden nur die Auftragspositionen mit einem Bestellkennzeichen an den Einkauf übergeben. |
| **Bestellpool** | Der Bestellpool wird manuell gefüllt. Er listet immer alle Dokumente auf, die im gewählten Nummernverwalter stehen. |
| **Bestellungen** | Bestellpositionen aus unterschiedlichen Aufträgen können zu einer Sammelbestellung zusammengefasst werden, wenn für diese Positionen der Lieferant und das Lieferdatum identisch sind. |
| **Lieferant** | Wenn in einem Auftrag mehrere Positionen mit Bestellkennzeichen erfasst wurden, wird für jeden Lieferanten eine eigene Bestellung erzeugt. |
| **Preisvergleich** | Vor der Übergabe der Bestellung können Sie die Preise der Lieferanten vergleichen, die das Produkt liefern können. Dazu muss die Lieferantenkartei gepflegt werden. |
| **Terminänderung** | Wird im Bestellpool das Anlieferdatum beim Kunden geändert, wird diese Änderung auch in den referenzierten Auftrag übernommen. |
| **Bestellung senden** | Bestellungen, die über den Bestellpool erzeugt wurden, müssen über den Dialog Formular-/ Etikettendruck gedruckt und an den Lieferanten gesendet werden. |

**Voreinstellungen**

Bestellübergabe > Menü Optionen:
-   **Auftragsbezogene Übergabe:** Die Bestellungen werden pro Auftrag übergeben. Wenn diese Option nicht aktiviert ist, können Sammelbestellungen erzeugt werden.
-   **Bestellnummer = Auftragsnummer:** Diese Option ist nur freigeschaltet, wenn die Option Auftragsbezogene Übergabe aktiviert ist. Diese Einstellung darf nicht aktiviert sein, wenn unterschiedliche Lieferanten in einem Auftrag erfasst sind.

Stammdaten:
-   Nummernkreise
-   Lieferantenkartei

Firmendaten:
-   Register Produktion (Profit-Center-Abrechnung)
-   Register Lager/EK/EDI (Abstandhalter mitbestellen)

##### Bestellpool

Bestellungen aus Kundenaufträgen werden automatisch erzeugt.

*Abb. D-27 Bestellpositionen im Bestellpool (Screenshot des Bestellpools mit Spalten für Auftragsnummer (A), Positionsnummer (B), Lieferant (C), Produkt (D), Optionen zum Erzeugen einer Bestellung (E) oder Anfrage (F), Dokumentennummer (G) und Stücklisten-Anzeige (H).)*

Dazu werden die Auftragspositionen über den Bestellpool an den Einkauf übergeben. Auftragspositionen ohne Bestellartikel werden nicht weiterverarbeitet. Anhand des Dokumentenstatus erkennt das Programm, welche Positionen zur Bestellung übergeben werden können.
Die Prüfung der Kundenaufträge im Bestellpool bezieht sich nur auf Produkte mit der Beschaffungsart **Bestellung** oder **Bestellung (komplett)**.

*Abb. D-28 Ablauf der Prüfung von Aufträgen im Bestellpool (Flussdiagramm: Auftrag -> Bestellpool -> Prüfung auf Bestellteile -> Hauptposition -> Stückliste Komponente -> untergeordnete Komponente. Bei 'ja' wird 'Pro Lieferant eine Bestellung' erzeugt.)*

Die Kundenaufträge werden zunächst auf der Ebene der Hauptposition und dann auf der Ebene der Stückliste nach Komponenten mit einer der beiden Beschaffungsarten durchsucht. Die Produkte werden dabei nach einfachen Bestellteilen und solchen Bestellteilen unterschieden, bei denen alle untergeordneten Produkte mitbestellt werden.
Wenn in einem Kundenauftrag mehrere Positionen erfasst sind, die bei unterschiedlichen Lieferanten bestellt werden, wird für jeden Lieferanten eine eigene Bestellung erzeugt.
Wenn in einem Kundenauftrag Lagerartikel in einer Stückzahl angegeben sind, die den aktuellen Lagerbestand überschreitet, müssen diese Lagerartikel durch eine (manuelle) Lagerbestellung erfasst und bestellt werden.

**Prüfungen**
Über das Menü **Optionen** können verschiedene Prüfungen aktiviert werden, z. B.:
-   **Lieferterminprüfung:** Der Liefertermin wird automatisch geprüft. Ändern Sie einen Liefertermin, der nicht an einem Tourentag liegt, wird eine entsprechende Meldung angezeigt.
-   **Lieferantentour berücksichtigen:** Wenn die Bestellung auf einen Liefertermin fällt, der nicht an einem Tourentag liegt, wird eine entsprechende Meldung angezeigt. Dazu müssen die Lieferantentouren in den Stammdaten hinterlegt werden.
-   **Vorlauftage mit Kombiwarengruppe ermitteln:** Wenn in den Kombiwarengruppen Vorlauftage hinterlegt sind, sollen diese zur Berechnung des Liefertermins herangezogen werden.
    ⇨ Stammdaten, "Vorlauftage" auf Seite B-681
-   **Produktbezeichnung aus Lieferantenkartei:** Die Bezeichnung der bestellten Produkte wird aus der Lieferantenkartei übernommen.
-   **Keine Kostenrückschreibung:** Die Kosten werden nicht in die EK-Preise des Auftrags zurückgeschrieben.
-   **Maßzuschläge berücksichtigen:** Bei der Bestellung sollen die Maßzuschläge mit übergeben werden.

**Bestellübergabe**
Vor der Übergabe der Bestellpositionen können Sie den Modus auswählen.
*Abb. D-29 Bestellmodus (Screenshot der Optionen: Pool füllen, Sofort bestellen, Sofort anfragen)*

*Abb. D-30 Lieferanten im Bestellpool ändern (Flussdiagramm zeigt, wie Aufträge in den Bestellpool gelangen. Dort kann ein Preisvergleich, eine Terminprüfung oder eine Änderung des Lieferanten stattfinden, bevor eine Bestellung oder Anfrage erzeugt wird.)*

Mit der Option **Sofort bestellen**, werden die Bestellungen erzeugt, ohne sie in den Bestellpool zu stellen. Im Bestellpool können die Termine und die Lieferanten geändert werden.

##### Lieferantenauswahl und Preisvergleich

Bei gefährdeten Terminen können andere Lieferanten ausgewählt werden. Diese werden aus der Lieferantenkartei ausgelesen. Wenn dort auch Preise pro Lieferant hinterlegt sind, ist ein Preisvergleich möglich, so dass Sie unabhängig von Terminproblemen auch zu dem günstigsten Lieferanten wechseln können.

*Abb. D-31 Lieferanten im Bestellpool ändern (Diagramm zeigt, wie aus Aufträgen im Nummernverwalter (NV) Bestellpositionen in den Bestellpool kommen, Standard-Lieferanten zugeordnet werden und dann zu Sammel-Bestellungen pro Lieferant zusammengefasst werden.)*

**Liefertermine**
Damit Liefertermine berechnet werden können, muss in der Lieferantenkartei die Lieferzeit für jeden einzelnen Lieferanten hinterlegt sein. Bei der Übergabe von Kundenaufträgen wird der Termin der Auslieferung beim Kunden geprüft. Dazu wird angezeigt, ob der Lieferant aufgrund seiner spezifischen Lieferzeit in der Lage ist, die Bestellung rechtzeitig zu liefern.
Der Liefertermin des Lieferanten im Bestellpool wird aus dem Versandtag minus der hinterlegten Vorlauftage zur jeweiligen WGR ermittelt.
Dabei werden die Wochentage und die Tour berücksichtigt. Wenn keine Vorlauftage eintragen sind, wird der Versandtag als Liefertermin übernommen.
Im Bestellpool wird farblich hervorgehoben, wenn ein Liefertermin aus dem Auftrag aufgrund der Liefertage aus der Lieferantenkartei für die Bestellung nicht eingehalten werden kann.
Der Lieferant und/oder der Liefertermin kann dann schon im Bestellpool geändert werden. Die Änderungen werden in den Auftrag zurückgeschrieben.

##### Erzeugte Bestellungen

Nachdem die Übergabe abgeschlossen ist, zeigt eine Meldung an, wie viele Dokumente nicht übergeben (verarbeitet) wurden.
*Abb. D-32 Fehlerhafte Dokumente (Screenshot zeigt eine Liste von Aufträgen mit einer Fehlermeldung, dass 4 Dokumente nicht verarbeitet wurden.)*

Diese müssen Sie dann einzeln prüfen und ggf. korrigieren. Dies können z. B. folgende Fehler sein:
-   Keine Bestellkennzeichen gefunden.
-   Auftrag ist noch geöffnet.
-   Status lässt die Übergabe nicht zu.

Aus den Auftragspositionen mit Bestellkennzeichen wurden Bestellungen erzeugt, die Sie in der Dokumentenverwaltung für Bestellungen öffnen und prüfen können. Diese Bestellungen senden Sie auf die übliche Weise an die betreffenden Lieferanten.
Für alle übergebenen Positionen wird der Status umgesetzt. In den referenzierten Aufträgen wird der Status umgesetzt.

**Bestellnummern**
Üblicherweise erhalten die automatisch erzeugten Bestellungen Nummern aus dem entsprechenden Nummernkreis. Sie können bei der Übergabe jedoch entscheiden, ob die Auftragsnummer auch als Bestellnummer verwendet werden soll.
