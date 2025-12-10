---
description: "DE_AWBusiness_Verkauf_4_8"
---


---
## Objektabrechnung

### Objekte – Dokumente

**Navigation:** `Dokumente > Auftrag > Objektabrechnung > Abrechnung > Register Abrechnungen > [Dokumente/Info]`

*Abb. C-370 Objekte - Dokumente*

In diesem Dialog werden alle Dokumente aufgelistet, die dem aktuellen Objekt zugeordnet sind. Der Dialog steht nur in der Standard-Objektverwaltung zur Verfügung.

Der Dialog wird auch angezeigt, wenn die Positionserfassung geschlossen wird. Dann werden jedoch nur die Aufträge aufgelistet, die für den aktuellen Kunden zu dem Objekt erfasst wurden.

### Stundenforderung

**Navigation:** `Dokumente > Auftrag > Objektabrechnung > Abrechnung > Menü Funktionen > Stundenforderungen hinzufügen`

*Abb. C-371 Stundenforderung hinzufügen*

In diesem Dialog hinterlegen Sie den Betrag, der für Zusatzleistungen erbracht wurde, z. B. für Montage-Arbeiten. Der Betrag wird dem ausgewählten Projekt zugeordnet.

Die Funktion ist nur freigeschaltet, wenn Sie den Modus Abrechnungsverwaltung mit zugeordneten Aufträgen aktiviert haben.

*   **Abrechnungsnummer:** Nummer der Abrechnung, zu der die Stundenforderung hinzugefügt werden soll.
*   **Wert:** Betrag der Stundenforderung.

### Einkaufsforderung

**Navigation:** `Dokumente > Auftrag > Objektabrechnung > Abrechnung > Menü Funktionen > Einkaufsforderungen hinzufügen`

*Abb. C-372 Einkaufsforderung hinzufügen*

In diesem Dialog hinterlegen Sie den Betrag, der für Zusatzkäufe erbracht wurde, z. B. für Montagematerial. Der Betrag wird dem ausgewählten Projekt zugeordnet.

Die Funktion ist nur freigeschaltet, wenn Sie den Modus Abrechnungsverwal-tung mit zugeordneten Aufträgen aktiviert haben.

*   **Abrechn.Nr.:** Nummer der Abrechnung, zu der die Einkaufsforderung hinzugefügt werden soll.
*   **Wert:** Betrag der Einkaufsforderung.

### Forderungsberechnung

**Navigation:** `Dokumente > Auftrag > Objektabrechnung > Abrechnung > Menü Funktionen > Forderungsrechnung erstellen`

Dieser Dialog wird je nach aktivierter Objektverwaltung unterschiedlich angezeigt:

*   "Abrechnungsverwaltung + Zugeordnete Aufträge" auf Seite C-704
*   "Abrechnungsverwaltung" auf Seite C-705

#### Abrechnungsverwaltung + Zugeordnete Aufträge

*Abb. C-373 Abrechnungsverwaltung mit zugeordneten Aufträgen – Forderungsrechnung*

In diesem Dialog wird angezeigt, welche Summen bereits durch Forderungsrechnungen abgedeckt sind. Zu den verbliebenen Mengen können Sie dann weitere Forderungsrechnungen erstellen, indem Sie in der Spalte `zu ber. Menge` den gewünschten Wert eingeben.

Über den eingegebenen Wert wird ein Dokument vom Typ Forderung erstellt, das Sie in der Dokumentenverwaltung für Aufträge öffnen und bearbeiten können. Die Nummer des neuen Dokuments können Sie sich in der Forderungshistorie anzeigen lassen.
⇨ "Forderungs-Historie" auf Seite C-706

Der Dialog wird auch angezeigt, wenn die Standard Objektverwaltung + Zuge-ordnete Aufträge aktiviert ist.

### Abrechnungsverwaltung

*Abb. C-374 Abrechnungsverwaltung – Forderungsrechnung*

In diesem Dialog können Sie die Forderungen erfassen, die zu einem Abrechnungsobjekt entstanden sind. Der Dialog ist nur kundenspezifisch freigeschaltet.

### Forderungs-Historie

**Navigation:** `Dokumente > Auftrag > Objektabrechnung > Abrechnung > Register Rahmenauftrag > Kontextmenü auf eine der angezeigten Positionen`

*Abb. C-375 Objekte - Forderungs-Historie*

In diesem Dialog wird angezeigt, welche Summen bereits durch Forderungsrechnungen abgedeckt sind.

Je nach der Wahl des Eintrags im Kontextmenü werden folgende Details angezeigt:

*   **Forderungshistorie nach Dokumenten:** Alle Dokumente zum Rahmenauftrag werden angezeigt.
*   **Forderungshistorie nach Positionen:** Nur die Dokumente zur aktuellen Position werden angezeigt.

## Auswertungen

**Navigation:** `Dokumente > Auftrag > Auswertungen`

In diesem Bereich finden Sie Dialoge, über die Sie verschiedene Auswertungen erstellen können.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Preisänderung (Report)" auf Seite C-707
*   "Null-Preisreport" auf Seite C-709
*   "Deckungsbeitrags-Analyse" auf Seite C-710
*   "Kalkulatorische Frachtkosten" auf Seite C-714

### Preisänderung (Report)

**Navigation:** `Dokumente > Auftrag > Auswertungen > Preisänderung`

*Abb. C-376 Preisänderungsreport*

In diesem Dialog können Sie sich eine Übersicht über die Preisänderungen für Aufträge und Angebote anzeigen oder drucken lassen.

#### Auswahl

*   **Datum von, Datum bis:** Sie können die Auswertung auf einen beliebigen Zeitraum.
*   **Auftragsnummer von, Auftragsnummer bis:** Sie können die Auswertung auf eine Spanne von Auftragsnummern einschränken.
*   **Kunde von, Kunde bis:** Sie können die Auswertung auf eine Spanne von Kundennummern einschränken.
*   **Aufträge, Angebote:** Sie können die Auswertung auf Aufträge oder Angebote einschränken.
*   **Archive mit einbeziehen:** Außerdem können Sie die Archive in die Auswertung einbeziehen.
    *   Die Auswertung zieht archivierte Dokumente nicht mit ein.
    *   Die Auswertung sucht auch in den Archiven nach entsprechenden Dokumenten. Beachten Sie dabei, dass die Auswertung u. U. sehr lange dauert.

#### Preise

Mit der Wahl der Option legen Sie fest, nach welchen Preisänderungen gesucht werden soll:
*   **Alle geänderten:** Alle Aufträge mit geänderten Preisen sollen angezeigt werden.
*   **Nur geänderte, die niedriger sind:** Nur Aufträge mit niedrigeren Preisen sollen angezeigt werden.
*   **Nur geänderte, die höher sind:** Nur Aufträge mit höheren Preisen sollen angezeigt werden.

#### Preisänderungen

In der Übersicht werden alle Dokumente angezeigt, die den Filterbedingungen entsprechen.

### Null-Preisreport

**Navigation:** `Dokumente > Auftrag > Auswertungen > Null-Preisreport`

*Abb. C-377 Null-Preisreport*

In diesem Dialog können Sie sich Übersichten zu kostenlosen Auftragspositionen anzeigen lassen. Zum Anzeigen der Übersicht wählen Sie jeweils einen Nummernverwalter aus.

#### Kostenlose Auftragspositionen

*   **Handelsvertreter:** Name des zuständigen Vertreters.
*   **Bearbeiter:** Name des Bearbeiters, der den Auftrag erfasst hat.
*   **Auftrag:** Auftragsnummer. Wenn in einem Auftrag mehrere Positionen ohne Berechnung aufgeführt sind, wird die Auftragsnummer mehrfach aufgelistet.
*   **Position:** Positionsnummer aus dem Auftrag.
*   **Status:** Auftragsstatus.
*   **AB Datum:** Datum der zugehörigen Auftragsbestätigung.
*   **Lieferdatum:** Lieferdatum aus dem Auftragskopf.
*   **Rechnung:** Rechnungsnummer. Das Feld bleibt leer, wenn noch keine Rechnung erstellt wurde.
*   **Kunden-Nr.:** Kundennummer aus dem Auftragskopf.
*   **Kunde:** Name des Kunden.
*   **Produkt-Nr.:** Produktnummer aus der Position.
*   **Produkt-Bezeichnung:** Produktbezeichnung aus der Position.
*   **Produziert/Gekauft:** Kennzeichnung, ob die kostenlose Position produziert oder eingekauft wurde.
*   **Kosten:** Kosten, die durch die Produktion oder den Einkauf zu dieser Position verursacht wurden.
*   **Verkaufs-Preis:** In dieser Übersicht ist der VK-Preis immer 0.
*   **Gewinn:** Wenn Kosten in der Position entstanden sind, wird der Gewinn als negativer Betrag angezeigt.
*   **Gewinn%:** In dieser Übersicht ist der Gewinn immer 0.
*   **Grund:** Wenn Sie die Begründung für manuelle Preisvorgaben aktiviert und eine entsprechende Bemerkung eingetragen haben, wird dieser Text angezeigt.

### Deckungsbeitrags-Analyse

**Navigation:** `Dokumente > Auftrag > Auswertungen > Deckungsbeitrags-Analyse`

In diesem Dialog können Sie die Deckungsbeiträge auswerten.

> **Voraussetzung**
> Deckungsbeitrag wird nur angezeigt, wenn entweder Standardwerte in den Firmendaten hinterlegt sind, oder wenn für die Kombination von Kunde/Kundengruppe und Warengruppe abweichende Werte festgelegt wurden.
>
> Die prozentualen Werte für die Deckungsbeiträge können für jede Kombination von Kunde/Kundengruppe und Warengruppe festgelegt sein. Sind für eine mögliche Kombination keine Werte festgelegt, werden die Standardwerte aus den Firmendaten herangezogen.
>
> ⇨ Stammdaten, "Deckungsbeitrags-Grenzwerte" auf Seite B-847
> ⇨ Stammdaten, "Default-Deckungsbeiträge" auf Seite B-982

In diesem Dialog finden Sie folgende Register:
*   "Deckungsbeitrags-Analyse – Auswahl" auf Seite C-711
*   "Deckungsbeitrags-Analyse – Tabelle" auf Seite C-713

### Deckungsbeitrags-Analyse – Auswahl

**Navigation:** `Dokumente > Auftrag > Auswertungen > Deckungsbeitrags-Analyse > Auswahl`

*Abb. C-378 Deckungsbeitrags-Analyse – Auswahl*

In diesem Register wählen Sie aus, in welchen Aufträgen die Deckungsbeiträge analysiert werden sollen.

#### Auftragsfilter

Mit der Wahl der Option legen Sie fest, welche Aufträge analysiert werden sollen:

*   **Nummernverwalter:** Alle Aufträge des gewählten Nummernverwalters werden herangezogen.
*   **Kundengruppe von – bis:** Sie können eine einzelne Kundengruppe oder eine Folge von Kundengruppen auswählen. Die Deckungsbeiträge werden in allen Aufträgen der Kunden analysiert, die zur gewählten Gruppe gehören. Dabei spielt es keine Rolle, in welchem Nummernverwalter die Aufträge stehen.
*   **Kunde von – bis:** Sie können einen einzelnen Kunden oder eine Folge von Kunden auswählen. Die Deckungsbeiträge werden in allen Aufträgen der gewählten Kunden analysiert. Dabei spielt es keine Rolle, in welchem Nummernverwalter die Aufträge stehen.

#### Positionsfilter

Mit der Wahl der Option legen Sie fest, welche Produkte betrachtet werden sollen.

*   **Warengruppe:** Sie können eine einzelne Warengruppe oder eine Folge von Warengruppen auswählen. Die Deckungsbeiträge werden in allen Positionen analysiert, die zur gewählten Gruppe gehören.
*   **Produkt:** Sie können ein einzelnes Produkt oder eine Folge von Produkten auswählen. Die Deckungsbeiträge werden in allen Positionen analysiert, in denen die betreffenden Produkte gefunden werden.

#### Restriktionen

Sie können die Analyse der Deckungsbeiträge weiter einschränken.

*   **Status:** Sie können einen einzelnen Status oder eine Folge auswählen. Die Deckungsbeiträge werden in allen Aufträgen analysiert, in einen betreffenden Status haben.
*   **Erfassung:** Sie können den Zeitraum bestimmen, in dem die Aufträge erfasst wurden, die Sie analysieren möchten.

#### Sortierung

Mit der Wahl der Option legen Sie fest, wie das Suchergebnis im Register Tabelle sortiert werden soll.

### Deckungsbeitrags-Analyse – Tabelle

**Navigation:** `Dokumente > Auftrag > Auswertungen > Deckungsbeitrags-Analyse > Tabelle`

*Abb. C-379 Deckungsbeitrags-Analyse - Tabelle*

In diesem Register werden alle Aufträge mit den Angaben zu den Deckungsbeiträgen aufgelistet, die Sie im Register Auswahl herausgefiltert haben. Diese Auswahl können Sie weiter filtern.

#### Deckungsbeitrags-Filter

Mit der Wahl der Option wird das Suchergebnis weiter gefiltert:

*   **Kein Filter:** Das Suchergebnis wird nicht weiter gefiltert.
*   **Größer Maximalwert:** Aus dem Suchergebnis werden nur die Auftragspositionen angezeigt, deren Deckungsbeitrag größer ist, als der festgelegte Maximalwert.
*   **Kleiner Minimalwert:** Aus dem Suchergebnis werden nur die Auftragspositionen angezeigt, deren Deckungsbeitrag kleiner ist, als der festgelegte Minimalwert.
*   **Größer Maximalwert oder kleiner Minimalwert:** Aus dem Suchergebnis werden alle die Auftragspositionen angezeigt, deren Deckungsbeitrag größer ist, als der festgelegte Maximalwert oder kleiner als der festgelegte Minimalwert ist.
*   **Benutzerdefinierter Deckungsbeitrag:** Aus dem Suchergebnis werden alle Auftragspositionen angezeigt, deren Deckungsbeitrag zwischen einem unteren und einem oberen Wert liegt, den Sie selbst bestimmen können.
*   **Minimal - maximal:** Diese Felder sind nur freigeschaltet, wenn Sie die Option Benutzerdefinierter Deckungsbeitrag gewählt haben. Tragen Sie in den Feldern die Werte ein, zwischen denen der Deckungsbeitrag liegen soll.

### Kalkulatorische Frachtkosten

**Navigation:** `Dokumente > Auftrag > Auswertungen > Kalkulatorische Frachtkosten`

Mit der Bestellübergabe werden die Produkte aus den Aufträgen herausgefiltert, die bestellt werden müssen.

> **Voraussetzung**
> Die Frachtkosten können nur berechnet und geprüft werden, wenn die Entfernungen in den Kundenstammdaten und die Kilometerpauschale in den Touren hinterlegt sind.

In diesem Dialog finden Sie folgende Register:
*   "Kalkulatorische Frachtkosten - Druck" auf Seite C-715
*   "Kalkulatorische Frachtkosten - Speditionskosten" auf Seite C-716

### Kalkulatorische Frachtkosten – Druck

**Navigation:** `Dokumente > Auftrag > Auswertungen > Kalkulatorische Frachtkosten > Druck`

*Abb. C-380 Kalkulatorische Frachtkosten - Druck*

In diesem Register lassen Sie sich die Verteilung der Frachtkosten über einen bestimmten Zeitraum anzeigen lassen. In der Übersicht können Sie Touren mit zu hohen Frachtkosten in Bezug auf den Umsatz identifizieren.

Im Auftrag können Sie sich die Frachtkosten ebenfalls anzeigen lassen.
⇨ "Kalkulatorische Frachtkosten" auf Seite C-574

#### Liefertermine, Kunden

*   **Von, bis:** Einschränkung der Auswertung auf einen Zeitraum und einen oder eine Reihe von Kunden. Wenn Sie in beiden Feldern denselben Wert eingeben, wird die Auswertung auf einen Tag oder einen Kunden eingeschränkt.

#### Darstellung

Mit der Wahl der Option legen Sie fest, wie die Frachtkosten dargestellt werden sollen:
*   **Tour:** Die Auswertung wird pro Tour und Datum nach Kunden sortiert.
*   **Kunde:** Die Auswertung wird pro Kunde und Datum nach Touren sortiert.
*   **Kumuliert:** Die Auswertung kann detailliert oder kumuliert dargestellt werden.
    *   Die Daten werden detailliert pro Lieferdatum angezeigt.
    *   Die Daten werden summiert pro Lieferdatum angezeigt.

#### Tourenauswahl

In der Auswahl werden alle Touren aufgelistet, die in den Stammdaten hinterlegt sind. Sie müssen mindestens eine Tour in das rechte Feld verschieben, damit die Daten ausgewertet werden können.

#### Aufträge

In der Übersicht werden alle Aufträge und Touren aufgelistet, die den Auswahlkriterien entsprechen. Die einzelnen Aufträge werden nur angezeigt, wenn für die Darstellung die Checkbox Kumuliert nicht markiert ist.

### Kalkulatorische Frachtkosten – Speditionskosten

**Navigation:** `Dokumente > Auftrag > Auswertungen > Kalkulatorische Frachtkosten > Speditionskosten`

*Abb. C-381 Kalkulatorische Frachtkosten - Speditionskosten*

In diesem Register erfassen Sie die Speditionskosten. Dazu muss mindestens eine Tour Spedition angelegt sein.

Speditionskosten, die durch ein Speditionsunternehmen entstehen, können folgendermaßen auf mehrere Aufträge verteilt werden:
*   Verteilung von Speditionskosten auf Aufträge nach Liefertermin und Tour.
*   Verteilung der gesamten Speditionskosten im Verhältnis zur Entfernung und zur transportierten Glasfläche.

Zur Berechnung des Anteils wird die tatsächliche Glasfläche ohne Maßrundungen betrachtet.

#### Selektion

*   **Liefertermin:** Tag, an dem die Spedition die Tour fährt.
*   **Tour:** Auswahl der Tour, die von der Spedition gefahren wird. Zur Auswahl stehen nur die Touren, für die keine Kilometerpauschale angegeben ist.

#### Speditionskosten

*   **Betrag (Netto):** Angabe des Rechnungsbetrags aus der Speditionsrechnung.

#### Aufträge

In der Übersicht werden nur die Aufträge angezeigt, auf die der Liefertermin und die gewählte (Speditions-)Tour zutreffen.

## Interne Kontrolle

**Navigation:** `Dokumente > Auftrag > Interne Kontrolle`

In diesem Bereich können Sie Auswertungen zu Gutschriftsgründen und zu Preisänderungen erstellen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Gutschriftgründe" auf Seite C-718
*   "Änderungen am Kundenstamm" auf Seite C-719
*   "Preis-/Rabattänderungen” auf Seite C-720
*   "Verspätete Lieferung/Lieferung ohne Berechnung" auf Seite C-721

### Gutschriftgründe

**Navigation:** `Dokumente > Auftrag > Interne Kontrolle > Gutschriftgründe`

*Abb. C-382 Gutschriftgründe*

In diesem Dialog können Sie über einen definierten Zeitraum auswerten, aus welchen Gründen Gutschriften erstellt wurden.

#### Selektion

*   **Datum von, bis:** Eingrenzung des Zeitraums, in dem nach Gutschriften gesucht wird. Wenn Sie einen großen Zeitraum angeben, sollten Sie die Archive mit einbeziehen.
*   **Archive mit einbeziehen:** Die Auswertung kann auch die Archive einbeziehen.
    *   Die Suche bezieht sich nur auf die Hauptdatenbank.
    *   Die archivierten Dokumente werden in die Suche bezogen.

#### Gutschriften

Liste der Gutschriften, die den Auswahlkriterien entsprechen.

#### Zusammenfassung

In der Übersicht werden die Gutschriften nach Gründen zusammengefasst.

### Änderungen am Kundenstamm

**Navigation:** `Dokumente > Auftrag > Interne Kontrolle > Änderungen am Kundenstamm`

*Abb. C-383 Änderung am Kundenstamm*

In diesem Dialog können Sie sich Änderungen der Kundenstammdaten über einen bestimmten Zeitraum anzeigen lassen. Der Dialog ist nur kundenspezifisch freigeschaltet.

### Preis-/Rabattänderungen

**Navigation:** `Dokumente > Auftrag > Interne Kontrolle > Preis-/Rabattänderungen`

*Abb. C-384 Preis-/Rabattänderungen*

In diesem Dialog können Sie sich Änderungen der Preise und Rabatte über einen bestimmten Zeitraum anzeigen lassen. Der Dialog ist nur kundenspezifisch freigeschaltet.

### Verspätete Lieferung/Lieferung ohne Berechnung

**Navigation:** `Dokumente > Auftrag > Interne Kontrolle > Verspätete Lieferung/Lieferung ohne Berechnung`

*Abb. C-385 Verspätete Lieferung/Lieferung ohne Berechnung*

In diesem Dialog können Sie auswerten, bei welchen Aufträgen das Lieferdatum überschritten ist, bzw. bei welchen Aufträgen noch keine Rechnung geschrieben wurde. Dazu können Sie ein Vergleichsdatum angegeben.

#### Selektion

Mit der Wahl der Option legen Sie fest, welche Suchkriterien Sie nutzen wollen:
*   **Nummernverwalter:** Die Suche bezieht sich auf die Dokumente im gewählten Nummernverwalter.
*   **Eigene Auswahl:** Für die Suche können der Status und das Lieferdatum als Kriterien angegeben werden.
*   **Status von, bis:** Die Suche wird über den Status eingegrenzt.
*   **Lieferdatum von, bis:** Die Suche wird auf den Zeitraum eingegrenzt, in dem die Lieferung erfolgen sollte.

#### Lieferungen

In der Übersicht werden alle Aufträge aufgelistet, die den Suchkriterien entsprechen. Diese Trefferliste kann weiter gefiltert werden.

#### Filter

Mit der Wahl der Option legen Sie fest, welche Aufträge angezeigt werden sollen.
*   **Verspätete Lieferung:** In der Trefferliste werden alle Aufträge angezeigt, die in Bezug auf das Vergleichsdatum verspätet sind.
*   **Lieferung ohne Berechnung (Ware geliefert und noch keine Rechnung geschrieben):** In der Trefferliste werden alle Aufträge angezeigt, zu denen trotz der Lieferung noch keine Rechnung erstellt wurde.

*   **Vergleichsdatum:** Vergleichsdatum für die Filterung der Trefferliste.

## Gutschrift

**Navigation:** `Dokumente > Gutschrift`

Über das Menü Gutschrift erreichen Sie sich folgende Programmpunkte:
*   **NV Gutschrift:** Die Funktion des Nummernverwalters ist für alle Dokumente gleich. Sie wird am Beispiel Auftrag beschrieben. ⇨ "Nummernverwalter" auf Seite C-629
*   **Gutschrift:** Die Erfassung von Dokumenten ist für alle Dokumentenarten gleich. Sie wird am Beispiel Auftrag beschrieben. ⇨ "Dokumentenverwaltung" auf Seite C-409, "Dokument - Positionen" auf Seite C-451
*   **Druck Gutschrift:** Der Formular- und Etikettendruck ist für alle Dokumente gleich. Er wird am Beispiel Auftrag beschrieben. ⇨ "Druck" auf Seite C-637
*   **FiBu-Übergabe:** Die FiBu-Übergabe ist für Aufträge, Gutschriften und Bestellungen gleich. Sie wird am Beispiel Auftrag beschrieben. ⇨ "FiBu-Übergabe" auf Seite C-679
*   **Journal:** Der Journaldruck ist für alle Dokumente gleich. Er wird am Beispiel Auftrag beschrieben. ⇨ "Journal" auf Seite C-725
*   **Anzahlungen Gutschriften:** Die Anzahlungen sind für alle Dokumente gleich. Sie werden am Beispiel Auftrag beschrieben. ⇨ "Anzahlungen" auf Seite C-673
*   **Übergabe Archiv:** Die Archivübergabe ist für alle Dokumente gleich. Sie wird am Beispiel Auftrag beschrieben. ⇨ "Übergabe Archiv" auf Seite C-686
*   **Suche:** Die Suche ist für alle Dokumente gleich. Sie wird am Beispiel Auftrag beschrieben. ⇨ "Dokument suchen" auf Seite C-523
*   **Bankbelege:** Die Bankbelege sind für Aufträge und Gutschriften gleich. Sie werden am Beispiel Auftrag beschrieben. ⇨ "Bankbelege" auf Seite C-674
*   **Import:** Mit dieser Funktion werden elektronische Dokumente importiert. ⇨ "Import" auf Seite C-688

### Gutschrift (Dokumentenverwaltung)

**Navigation:** `Dokumente > Gutschrift > Gutschrift`

In diesem Dialog erfassen und bearbeiten Sie Gutschriften.
Die Felder im Dialog Kopfdaten und in der Positionserfassung sind für alle Dokumententypen gleich. Sie werden in dieser Anleitung am Beispiel Auftrag beschrieben.
⇨ "Dokument - Kopfdaten" auf Seite C-417
⇨ "Dokument - Positionen" auf Seite C-451

## Journal

**Navigation:** `Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Journal`

Die Ausgabe eines Journals ist für alle Dokumente gleich. Sie wird in dieser Anleitung am Beispiel Auftrag beschrieben.
⇨ "Eingangs-/Ausgangs-Journal" auf Seite C-725

### Eingangs-/Ausgangs-Journal

**Navigation:** `Dokumente > Auftrag > Journal`

*Abb. C-386 Eingangs/Ausgangs-Journal*

In diesem Dialog können Sie sich Listen zu den Dokumenten ausgeben lassen.
⇨Tutorial, "Journal" auf Seite C-384

#### Auswahl Bereich

Mit der Wahl der Option geben Sie an, für welche Dokumente Sie das Journal erstellen wollen:
*   Angebot
*   Auftrag
*   Gutschrift
*   Bestellanfrage
*   Bestellung

#### Datenbank

Wenn Sie mit mehreren Datenbanken arbeiten, müssen Sie auswählen, aus welcher das Journal erstellt werden soll. Zur Wahl stehen auch die Archive.

#### Modus

Mit der Wahl der Option geben Sie die Bedingungen für die Erstellung der Liste an:
*   **Nach Nummernverwalter:** Die Liste soll alle Dokumente aus einem bestimmten Nummernverwalter auflisten. Im Bereich Identifikation/Nummernverwalter wird das Feld Nummernverwalter wird freigeschaltet.
*   **Nach Auswahlkriterien:** Die Liste soll alle Dokumente nach Kriterien auflisten, die Sie selbst bestimmen. Im Bereich Auswahl Kriterien werden die Felder wird freigeschaltet.

#### Auswahl Liste

Zur Auswahl stehen verschiedene fest definierte Listen. Jede Liste schließt mit der Gesamtsumme pro Spalte.
⇨Tutorial, "Journal" auf Seite C-384

#### Zwischensummen

Die Ausgabe der Zwischensumme können Sie selbst bestimmen. Im Tutorial finden Sie eine Beschreibung der Darstellungen im Report.
⇨Tutorial, "Journal" auf Seite C-384

*   **Pro Kunde, Pro Rechnung, Pro Vertreter:** Eine Zwischensumme kann pro Kunde, Rechnung und/oder Vertreter eingefügt werden.
    *   Die Zwischensumme wird nicht ausgegeben.
    *   Die Zwischensumme wird an der gewählten Stelle ausgegeben.

#### Identifikation/Nummernverwalter

*   **Mitarbeiter:** Name des Mitarbeiters, der sich in A+W Business angemeldet hat.
*   **Nummernverwalter:** Auswahl des Nummernkreises, dessen Dokumente aufgelistet werden sollen. Das Feld ist gesperrt, wenn im Bereich Modus die Option nach Auswahlkriterien gewählt wurde.

#### Auswahl Kriterien von, bis

Die Felder sind gesperrt, wenn im Bereich Modus die Option nach Nummernverwalter gewählt wurde.

*   **Statusbereich von, bis:** Eingabe von Statusnummern der Dokumente. Wenn Sie in beiden Feldern dieselbe Nummer eingeben, werden nur die Dokumente mit diesem Status aufgelistet.
*   **Erfassungsdatum von, bis:** Das Journal wertet nur die Dokumente im gewählten Erfassungszeitraum aus.
*   **Datum AB von, bis:** Das Journal wertet nur die Dokumente aus, deren Auftragsbestätigung im gewählten Erfassungszeitraum gedruckt wurde.
*   **Lieferdatum von, bis:** Das Journal wertet nur die Dokumente im gewählten Lieferzeitraum aus.
*   **Rechnungsdatum von, bis:** Das Journal wertet nur die Dokumente aus, deren Rechnungsdatum im gewählten Erfassungszeitraum liegt.

#### Druck-Optionen

Mit der Wahl der Option legen Sie fest, wie die Maße ausgedruckt werden sollen:
*   **Dimensionsangaben real:** Im Druck wird die tatsächliche Fläche angegeben.
*   **Dimensionsangaben fakturiert:** Im Druck wird die fakturierte Fläche angegeben, in der z. B. die Maßrundungen berücksichtigt sind.

*   **Erste Kommission auf Versandliste:** Für die Versandliste kann zusätzlich die Kommission ausgegeben werden.
    *   Die erste Kommission wird nicht ausgegeben.
    *   Die Kommission wird aus der ersten Position in der Positionserfassung übernommen.
        ⇨ "Kommission" auf Seite C-456

## Bestandslisten

**Navigation:** `Dokumente > Bestandslisten`

In diesem Programmbereich können Sie Übersichten über Dokumente verschaffen, die aktuell in der Hauptdatenbank verwaltet werden.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Nummernbereiche" auf Seite C-728
*   "Warengruppen" auf Seite C-730

### Nummernbereiche

**Navigation:** `Dokumente > Bestandslisten > Nummernbereiche`

*Abb. C-387 Bestandslisten – Nummernbereiche*

Wenn Sie mit Nummernbereichen arbeiten, können Sie sich in diesem Dialog Übersichten über den aktuellen Bestand an Dokumenten in den Nummernkreisen verschaffen.

Das Programm schaut in den Nummernkreisen in den Stammdaten nach der letzten Nummer. Anschließend listet es hier alle Dokumente hier auf, die noch nicht gedruckt wurden.

Mit der Bestätigung, dass der Ausdruck OK war, wird die letzte Nummer hier angezeigt und gleichzeitig in den Stammdaten aktualisiert.
⇨ Stammdaten, "Nummernkreise" auf Seite B-891

#### Nummernkreis

*   **Mandant:** Mandanten, für den die Übersicht erstellt wird.
    ⇨ Stammdaten, "Firmendaten - Mandant" auf Seite B-919
*   **AV-Bereich:** AV-Bereichen, zu dem die Dokumente gehören. Das Feld ist gesperrt, wenn die Checkbox Alle im AV-Bereich drucken markiert ist.
*   **Alle im AV-Bereich drucken:** Sie können wahlweise alle Dokumente eines AV-Bereichs drucken oder einen bestimmten auswählen. Mit der Schaltfläche öffnen Sie den Dialog Nummernkreise.
    *   Die Dokumente aus dem Nummernkreis des gewählten AV-Bereichs werden gedruckt.
    *   Alle Dokumente aus den Nummernkreisen des gewählten Mandanten werden gedruckt. Das Feld AV-Bereich wird gesperrt.

#### Dokumententyp

Mit der Wahl der Option bestimmen Sie, für welchen Dokumententyp eine Bestandsliste erstellt werden soll.

Nach dem erfolgreichen Erstellen der Übersicht wird jeweils die letzte Nummer für den Dokumententyp angezeigt. Diese Nummer wird auch im Dialog Nummernkreise angezeigt.
⇨ Stammdaten, "Nach Zeitraum" auf Seite B-893

### Warengruppen

**Navigation:** `Dokumente > Bestandslisten > Warengruppen`

*Abb. C-388 Bestandslisten – Warengruppen*

In diesem Dialog können Sie sich Übersichten über den aktuellen Dokumentenbestand in den Nummernverwaltern oder nach Zeiträumen für die Erfassung oder Lieferung verschaffen. Die Übersicht ist nach Warengruppen geordnet. Sie wird mit der Druckfunktion ausgegeben.
⇨Tutorial, "Bestandslisten" auf Seite C-383

#### Druckparameter Selektion

Mit der Wahl der Optionen legen Sie fest, nach welchen Kriterien die Dokumente gesucht werden sollen.

*   **Nummernverwalter:** Die Bestandsliste prüft alle Dokumente im gewählten Nummernverwalter. Die Auswahlmöglichkeiten richten sich nach dem gewählten Dokumententyp. Die Eingabefelder für Erfassungsdatum, Liefertermin und Status sind gesperrt.
*   **Erfassungsdatum von, bis:** Die Bestandsliste stellt nur die Dokumente im gewählten Erfassungszeitraum dar.
*   **Liefertermin von, bis:** Die Bestandsliste stellt nur die Dokumente im gewählten Lieferzeitraum dar.
*   **Status von, bis:** Die Bestandsliste stellt nur die Dokumente mit den gewählten Statusnummern dar.

#### Dokumententyp

Mit der Wahl der Option bestimmen Sie, für welchen Dokumententyp eine Bestandsliste erstellt werden soll.

#### Auswertungstiefe von - bis

Mit der Wahl der Option legen Sie fest, nach welcher Ebene von Warengruppen die Bestandslisten zusammengefasst werden.
Für die Auswahl der Dokumente kann ein Bereich angegeben werden. Die Felder von und bis sind gesperrt, wenn die Checkbox Alle drucken markiert ist.

*   **Alle drucken:** Sie können in der Bestandsliste alle Dokumente berücksichtigen, die zu einer Warenhauptgruppe, Warenobergruppe oder Warengruppe gehören.
    *   Nur die Dokumente des eingestellten Bereichs der Warengruppenebene werden berücksichtigt.
    *   Alle Dokumente der gewählten Warengruppenebene werden berücksichtigt. Die Felder von und bis sind gesperrt.
*   **Nur Gesamtsummen der WGR drucken:** Sie können nur die Gesamtsumme je Warengruppen drucken.
    *   Alle Werte des eingestellten Bereichs der Warengruppenebene werden dargestellt.
    *   Nur die Gesamtsummen des eingestellten Bereichs der Warengruppenebene werden dargestellt.
*   **Einkaufspreis nicht drucken:** Sie können die Einkaufspreise ausschließen.
    *   Alle Werte des eingestellten Bereichs der Warengruppenebene werden dargestellt.
    *   Die Einkaufspreise werden nicht dargestellt.
*   **Erste Kommission des Auftrags drucken:** Sie können die Angaben zur Kommission aus dem Auftrag übernehmen.
    *   Alle Werte des eingestellten Bereichs der Warengruppenebene werden dargestellt.
    *   Zusätzlich zur Auftragsnummer wird die Kommissionsnummer dargestellt. ⇨ "Kommission" auf Seite C-456

## Mahnwesen

**Navigation:** `Dokumente > Mahnwesen`

Die ausgegangenen Rechnungen können über die Rückmeldung der offenen Posten geprüft werden. Mahnungen können für Rechnungen ausgegeben werden.
⇨Tutorial, "Mahnung senden" auf Seite C-215

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   Menüs im Dialog Mahnwesen
*   "Mahnwesen" auf Seite C-733
*   "Offene-Posten-Tabelle füllen" auf Seite C-736

### Menüs im Dialog Mahnwesen

**Navigation:** `Dokumente > Mahnwesen`

Über die Menüs im Dialog Mahnwesen können Sie die Standardeinstellung des Dialoges bestimmen und andere Dialoge öffnen, ohne den Dialog Dokumente zu schließen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menü Zahlung" auf Seite C-732
*   "Menü Optionen" auf Seite C-732
*   "Menü Funktionen" auf Seite C-733

#### Menü Zahlung

**Navigation:** `Dokumente > Mahnwesen > Menü Zahlung`

Über dieses Menü können Sie Zahlungen zu einer angemahnten Rechnung erfassen oder bearbeiten.
*   **Neue Zahlung:** Schaltet die Felder frei, um zu einer markierten Rechnung eine Zahlung zu erfassen.
*   **Zahlung löschen:** Löscht die Zahlung, die zu einer Rechnung erfasst wurde.
*   **Zahlung ändern:** Schaltet die Felder einer markierten Rechnung frei, um die Werte einer erfassten Zahlung zu ändern.

#### Menü Optionen

**Navigation:** `Dokumente > Mahnwesen > Menü Optionen`

Über dieses Menü können Sie eine erfasste Mahnung per Fax versenden.
*   **Faxversand:** Mahnungen können per Fax versendet werden. Dazu muss eine Fax-Nummer in der Rechnung erfasst sein.

#### Menü Funktionen

**Navigation:** `Dokumente > Mahnwesen > Menü Funktionen`

Über dieses Menü können Sie die Mahnstufen bearbeiten und das Mahnkennzeichen von einer Rechnung löschen.
*   **Mahnstufen:** Öffnet den Dialog Mahnstufen, in dem Sie neue Mahnstufen erfassen können. ⇨ "Mahnstufen" auf Seite C-735
*   **Mahnstufe zurücksetzen:** Setzt das Mahnkennzeichen der markierten Rechnungen zurück.
*   **Offene-Posten-Tabelle füllen:** Öffnet einen Dialog, um den Nummernverwalter mit den offenen Rechnungen auszuwählen. Diese Funktion ist abhängig von der aktuellen FiBu. ⇨ "Offene-Posten-Tabelle füllen" auf Seite C-736

### Mahnwesen Dialog

**Navigation:** `Dokumente > Mahnwesen`

*Abb. C-389 Mahnwesen*

In diesem Dialog können Sie eingegangene Zahlungen zu offenen Rechnungen verbuchen oder Mahnungen erstellen. Sie können die Daten einzeln einlesen oder die Dokumente aus einem Nummernverwalter anzeigen lassen.
⇨ Tutorial, "Mahnung" auf Seite C-211

#### Rechnung

*   **Nr./Datum:** Nummer und Datum der Rechnung, die in der Übersicht markiert ist. Die Felder sind nur freigeschaltet, wenn Sie eine neue Rechnung erfassen möchten.
*   **Mahnstufe:** Mahnstufen sind in den Stammdaten hinterlegt. Mit der Auswahl einer Mahnstufe wird gleichzeitig die Gebühr angezeigt.
*   **Gebühr/Datum:** Die Gebühr wird automatisch angezeigt, wenn mit der Mahnstufe eine Gebühr erhoben wird. Der Betrag kann überschrieben werden. Das Datum wird nur angezeigt, wenn zu einer Rechnung bereits eine Mahnung verschickt wurde.
*   **Ausgeglichen:** Sie können Rechnungen als ausgeglichen kennzeichnen, wenn die Differenz zwischen dem Rechnungsbetrag und der Zahlung so geringfügig ist, dass sie vernachlässigt werden kann.
    *   Wenn noch ein Betrag offen ist, soll die Rechnung nicht als ausgeglichen gelten.
    *   Die Rechnung soll als ausgeglichen gelten, obwohl noch ein Betrag offen ist.
*   **Betrag:** Betrag der Rechnung, die in der Übersicht markiert ist.
*   **Geleistet:** Der als Zahlung erfasste Betrag.
*   **Offen:** Die Differenz zwischen dem Rechnungsbetrag und der erfassten Zahlung wird automatisch angezeigt. Eine offene Differenz wird in roter Schrift dargestellt, eine Überzahlung in blauer Schrift.

#### Kunde

Die Felder in diesem Bereich sind nur freigeschaltet, wenn Sie eine neue Rechnung anlegen.

*   **Nr./Name:** Nummer und Name des Kunden, dessen Rechnung noch offen ist.
*   **Anschrift:** Rechnungsanschrift wird aus dem Auftrag.
*   **Fax:** Fax-Nummer aus dem Auftrag.

#### Geleistete Zahlungen

In diesem Bereich werden die zu einer Rechnung erfassten Zahlungen aufgelistet.

#### Zahlung

Die Felder in diesem Bereich sind nur freigeschaltet, wenn Sie eine Zahlung erfassen möchten.

*   **Betrag:** Betrag der neuen Zahlung. Wenn er nicht mit dem Rechnungsbetrag übereinstimmt, wird die Differenz im Feld offen ausgewiesen.
*   **Datum:** Aktuelles Datum (Systemdatum). Es kann überschrieben werden.
*   **Abgezogenes Skonto:** Wenn mit dem Kunden ein Skonto vereinbart wurde, kann der Betrag eingetragen werden. Auf diese Weise können offene Rechnungen aus Kulanzgründen als ausgeglichen erfasst werden, obwohl der Zahlungstermin überschritten wurde.
*   **Rechnung:** Betrag angezeigt, der als Zahlung erfasst wurde.

#### Rechnungen

In der Übersicht werden alle Rechnungen aufgelistet, die gemahnt werden müssen, weil ihr Zahlungstermin überschritten ist.

### Mahnstufen

**Navigation:** `Dokumente > Mahnwesen > Menü Funktionen > Mahnstufen`

*Abb. C-390 Mahnstufen*

In diesem Dialog können Sie die Mahnstufen einrichten und bearbeiten.

### Offene-Posten-Tabelle füllen

**Navigation:** `Dokumente > Mahnwesen > Menü Funktionen > Offene Posten-Tabelle füllen`

*Abb. C-391 OP-Tabelle füllen*

In diesem Dialog können Sie einen Nummernverwalter auswählen, um die offenen Rechnungen in den Dialog Mahnwesen einzulesen. Diese Funktion ist abhängig von der aktuellen FiBu.

## Dokumentendaten

**Navigation:** `Dokumente > Dokumentendaten`

Die Bestell- und Lieferdaten von Dokumenten in einem Nummernverwalter können bearbeitet werden, ohne die Dokumente einzeln zu suchen und zu öffnen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menüs im Dialog Dokumente" auf Seite C-737
*   "Dokumentendaten" auf Seite C-738

### Menüs im Dialog Dokumente

**Navigation:** `Dokumente > Dokumentendaten`

Über die Menüs im Dialog Dokumente können Sie die Standardeinstellung des Dialoges bestimmen und andere Dialoge öffnen, ohne den Dialog Dokumente zu schließen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menü Funktionen" auf Seite C-737
*   "Menü Optionen" auf Seite C-737

#### Menü Funktionen

**Navigation:** `Dokumente > Dokumentendaten > Menü Funktionen`

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Dialog Dokumente zu schließen. Folgende Einträge werden angezeigt:
*   **Historie:** Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des Dokuments. ⇨ "Historie" auf Seite C-552
*   **Dokument anzeigen:** Öffnet den Dialog Dokumentenansicht als Vorschau auf das Dokument. ⇨ "Dokument anzeigen" auf Seite C-548

#### Menü Optionen

**Navigation:** `Dokumente > Dokumentendaten > Menü Optionen`

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Option aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.
*   **Dokumente in Hauptdatenbank und Archiv suchen:** Standardmäßig werden die Dokumente nur aus der Hauptdatenbank ausgelesen. Mit dieser Option legen Sie fest, dass die Dokumente sowohl aus der Hauptdatenbank als auch aus dem Archiv ausgelesen werden. ⇨ Stammdaten, "Firmendaten - Archiv" auf Seite B-965

### Dokumentendaten Dialog

**Navigation:** `Dokumente > Dokumentendaten`

*Abb. C-392 Dokumentdaten*

In diesem Dialog können Sie die Auftrags- und die Bestelldaten zu den Dokumenten prüfen.

#### Auswahlkriterien

*   **Dokument:** Auswahl des Dokumententyps, der angezeigt werden soll.
*   **Nummer:** Mit der Eingabe der Nummer lassen Sie sich ein ganz bestimmtes Dokument anzeigen. Das Feld ist gesperrt, wenn Sie die Checkbox Nummernverwalter markiert haben.
*   **Nummernverwalter:** Nummernverwalter, dessen Dokumente Sie prüfen wollen. Wenn Sie ein Dokument geändert haben, wird es im angezeigten Nummernverwalter abgelegt.
    *   Die Auswahl des Nummernverwalters ist gesperrt. Das Feld Nummer ist freigeschaltet.
    *   Die Dokumente aus einem Nummernverwalter sollen angezeigt werden. Das Auswahlfeld ist freigeschaltet.

#### Auftrag

*   **Nummer:** Die Auftragsnummer wird nur angezeigt, wenn ein einzelner Auftrag ausgewählt wurde.
*   **Versand Plan:** Das geplante Versanddatum wird nur angezeigt, wenn ein einzelner Auftrag ausgewählt wurde.
*   **Versandtag:** Versandtag aus dem Auftrag. Wenn der Liefertermin geändert wurde, können Sie das Datum entsprechend anpassen.
*   **Anlieferung:** Datum der Anlieferung beim Kunden aus dem Auftrag. Wenn der Liefertermin geändert wurde, können Sie das Datum entsprechend anpassen.
*   **Status:** Status des Auftrags. Sie können ihn bei Bedarf anpassen.
*   **Tour:** Tour aus dem Auftrag. Sie können sie bei Bedarf ändern.
*   **Lieferbed.:** Lieferbedingung aus dem Auftrag. Sie können sie bei Bedarf ändern.
*   **Kunde, Telefon:** Die Daten werden nur angezeigt, wenn ein einzelner Auftrag ausgewählt wurde.
*   **Ziel-NV:** Die Dokumentendaten können in einen anderen Nummernverwalter gestellt werden.
    *   Die Dokumentendaten werden nicht in einen anderen Nummernverwalter gestellt.
    *   Die Kombobox für den Ziel-Nummernverwalter wird freigeschaltet. Die Dokumentendaten werden in den gewählten Nummernverwalter gestellt.

#### Übersicht (Auftrag)

In der Übersicht wird das gewählte Dokument oder alle Dokumente aus dem Nummernverwalter angezeigt.

#### Bestellung

*   **Nummer:** Die Bestellnummer wird nur angezeigt, wenn ein einzelner Auftrag ausgewählt ist, zu dem eine Bestellung erzeugt wurde.
*   **Anlief. Plan:** Geplantes Anlieferungsdatum aus der Bestellung.
*   **Anlief. Termin:** Termin der Anlieferung aus der Bestellung. Wenn der Lieferant einen späteren Termin bestätigt hat, können Sie das Datum ändern. Der neue Termin wird in den Auftrag und die Bestellung übernommen, der Kunde kann eine Terminberichtigung erhalten. ⇨ “Kundenbenachrichtigung (Lieferterminkontrolle)" auf Seite C-565
*   **Status:** Status der Bestellung. Sie können ihn bei Bedarf ändern.
*   **Tour:** Tour aus der Bestellung. Sie können sie bei Bedarf ändern.
*   **Lieferbed.:** Lieferbedingung aus der Bestellung. Sie können sie bei Bedarf ändern.
*   **Lieferant, Telefon:** Name und Telefonnummer des Lieferanten aus der Bestellung.
*   **AB-Lieferant:** Die Auftragsbestätigung durch den Lieferanten wird nur angezeigt, wenn das Dokument über den Wareneingang erfasst wurde. ⇨ Einkauf, "AB-Lieferant" auf Seite D-197

#### Übersicht (Bestellung)

In der Übersicht werden alle Bestellungen zum gewählten Auftrag angezeigt.

## Lagersuche

**Navigation:** `Dokumente > Lagersuche`

Die Lagersuche können Sie auch während der Erfassung einer Position öffnen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Lagerinfo" auf Seite C-741
*   "Dokumentenübersicht" auf Seite C-746

### Lagerinfo

**Navigation:** `Dokumente > Lagersuche`

Über die Lagersuche können Sie den Lagerort für ein Produkt feststellen und den Bestand prüfen.

In diesem Dialog finden Sie folgende Register:
*   "Lagerinfo - Lagersuche" auf Seite C-742
*   "Lagerinfo - Zukünftiger Lagerbestand" auf Seite C-745

### Lagerinfo – Lagersuche

**Navigation:** `Dokumente > Lagersuche > Register Lagersuche`

*Abb. C-393 Lagerinfo - Lagersuche*

In diesem Register können Sie den Bestand Ihrer Lager(orte) prüfen und sich Details zu den gelagerten Gläsern anzeigen lassen.

> **Auswahl in den Auftrag übernehmen**
> Wenn Sie den Dialog Lagerinfo aus der Positionserfassung heraus geöffnet haben, können Sie das gewünschte Produkt mit einem Doppelklick in den Auftrag übernehmen.

#### Auswahl

In den Feldern werden die Details zu der Position angezeigt, die in der Übersicht markiert ist.

*   **Produkt:** Produktnummer, unter der das Produkt in den Stammdaten erfasst ist.
*   **Art:** Produktart, der das Produkt in den Stammdaten zugeordnet ist.
*   **Gruppe:** Produktgruppe, der das Produkt in den Stammdaten zugeordnet ist.
*   **Identnr.:** Identifikationsnummer, unter der der Lagerartikel im Lager erfasst wurde, z. B. für eine Kiste.
*   **Kateg.:** Wenn in Ihrem Unternehmen Lagerkategorien definiert sind, können diese zum Filtern eingesetzt werden. ⇨ Stammdaten, "Lagerkategorien" auf Seite B-739
*   **Farbe:** (Farb-) Varianten, die zu dem markierten Produkt erfasst sind.
*   **WGR von, bis:** Zur Suche können Sie auch Warengruppen oder Warengruppenbereiche eintragen. In der Übersicht werden dann alle Produkte der gewählten Warengruppen angezeigt.
*   **Dicke / Breite / Höhe:** Diese Angaben werden aus der Lagerverwaltung übernommen. Breite und Höhe werden nur angezeigt, wenn die markierte Position als Lagermaß oder Kiste mit den entsprechenden Angaben erfasst wurde.
*   **Lagerort:** Wenn Sie mit mehreren Lagerorten arbeiten, wird der Lagerort der markierten Position mit allen definierten Ebenen angezeigt. ⇨ Stammdaten, "Lagerdefinition" auf Seite B-737
*   **Lief. Ident:** Identifikationsnummer der Lieferung aus der Lagerverwaltung. Sie ist nicht identisch mit der Angabe in der Spalte `Ident` in der Übersicht.
*   **Bemerkung:** Information, die zur markierten Position bei der Lieferung hinterlegt wurde.
*   **Inhalt von, bis:** Im Auswahlmodus kann der Inhalt als Suchkriterium angegeben werden, z. B. alle Kisten mit einem Inhalt von 50 Stück. Inhalt = 1 bedeutet immer Lagermaß.
*   **Verfügbarkeit:** Anzeige der vorrätigen Stückzahlen.

#### Filteroptionen

Wenn keine Filter gesetzt sind, werden keine Bestände angezeigt. Der Filter ist gesetzt, wenn die jeweilige Checkbox markiert ist. Folgende Filter stehen zur Wahl:
*   **Lagerware:** Lagerartikel sollen angezeigt werden.
*   **Kisten (Inhalt > 1):** Kisten mit einem Inhalt > 1 sollen angezeigt werden.
*   **Lagertafeln (Inhalt = 1):** Lagermaße sollen angezeigt werden. Die Anzeige der Anzahl (= 1) dient zur Unterscheidung von Kisten mit identischen Größen.
*   **Artikel ohne Abmessung:** Auch Lagerartikel ohne Abmessungen sollen angezeigt werden.
*   **Kisten mit Identnummer:** Kisten, die mit eine ID im Wareneingang erfasst wurden, sollen angezeigt werden.
*   **Mindestmenge > 0:** Nur die Lagerartikel, deren Mindestmenge größer als 0 definiert wurde, sollen angezeigt werden.
*   **Bestand > 0:** Nur Lagerartikel mit einem Bestand sollen angezeigt werden.
*   **Bestand = 0:** Nur Lagerartikel ohne Bestand sollen angezeigt werden.
*   **Bestand < 0:** Nur die Lagerartikel sollen angezeigt werden, zu denen Reservierungen vorliegen, aber kein Bestand.

#### Druckoptionen

Sie können die Sortierung für den Druck der Übersicht bestimmen. Mit der Wahl der Option werden die entsprechenden Checkboxen freigeschaltet. Sie können dann zusätzlich festlegen, wo eine Zwischensumme gedruckt werden soll.

Folgende Einträge werden angezeigt:
*   **Gruppierung nach Produktnummer:** Die Checkbox `Zwischensumme n. Warengruppe` wird freigeschaltet.
*   **Gruppierung nach Produktart/Produktgruppe gruppieren:** Die Checkbox `Zwischensummen. Warenobergrp.` wird freigeschaltet.
*   **Gruppierung nach Warengruppen:** Die Checkbox `Zwischensumme n. Warenhauptgrp.` wird freigeschaltet.

#### Übersicht

In der Übersicht werden alle Produkte angezeigt, die mit der Suche ausgewählt wurden. Die Spalten zeigen die Details zu den gelagerten Produkten an. Die reservierten Mengen werden aktualisiert, sobald eine entsprechende Position im Auftrag gespeichert wurde. Mit dem Druck des Lieferscheins werden die Angaben in der Spalte `Bestand` aktualisiert.
Die Einträge in der Trefferliste sind mit folgenden Farben gekennzeichnet:
*   **Schwarze Schrift:** Lagerartikel mit Mengenführung
*   **Blaue Schrift:** Lagerartikel ohne Mengenführung
*   **Rote Schrift:**
    *   Kein Lagerartikel: Artikel, die nicht im Lager geführt werden.
    *   Dies gilt auch für Produkte, die nicht mehr verfügbar sind oder mit negativen Beständen angezeigt werden. Ein negativer Bestand entsteht, wenn der Bestand und die bestellte Menge abzüglich der reservierten Menge <= 0 sind.

#### Summen

Die Summen des ausgewählten Produkts werden angezeigt. Wenn Sie eine WGR mit verschiedenen Produkten ausgewählt haben, werden die Summen des markierten Produkts angezeigt.

### Lagerinfo – Zukünftiger Lagerbestand

**Navigation:** `Dokumente > Lagersuche > Register Zukünftiger Lagerbestand`

*Abb. C-394 Lagerinfo - Zukünftiger Lagerbestand*

In diesem Register können Sie prüfen, wie viele Gläser bestellt wurden und wie viele bereits reserviert sind.

#### Aktueller Lagerbestand

*   **Vorschau bis:** Die Vorschau beginnt immer mit dem aktuellen Tagesdatum. Die Anzahl der Tage für die Vorschau stellen Sie in den Firmendaten ein, z. B. 14 Tage.
    *   In der oberen Übersicht werden die Daten in einer Zeile pro gewähltem Produkt aufgelistet.
    *   In der mittleren Übersicht werden die aktuellen Bestände pro Tag wiedergegeben.
    *   In der unteren Übersicht werden Details zum gewählten Produkt angezeigt. In der Spalte `Kritischer Lagerbestand` wird die Menge angezeigt, die in der Lagerwirtschaft für den Artikel hinterlegt ist.
        ⇨Lagerwirtschaft, "Lagerverwaltung - Lagerartikel" auf Seite G-186

Die Zeilen sind rot, wenn die Produktion nicht möglich ist, weil die Reservierungen den Bestand überschreiten.
⇨ Stammdaten, "Lagervorschau" auf Seite B-961

### Dokumentenübersicht

**Navigation:** `Dokumente > Lagersuche > Register Zukünftiger Lagerbestand > Übersicht > Doppelklick auf Produkt`

*Abb. C-395 Dokumentenübersicht*

In diesem Dialog wird eine Liste der Dokumente angezeigt, in denen das betreffende Lagermaß erfasst ist.

## Partindex

**A+W Business**
A+W - Software for Glass, Windows and Doors

## Index Verkauf

### Nummern
*   **1 zu 1 (Register in Dokumente kopieren)** C-536

### A
*   **Abkleben** C-483
*   **Abrechnungsverwaltung**
    *   aufgelaufene Summen C-698
    *   Einkaufsforderung C-703
    *   Forderung C-704
    *   Forderungshistorie C-706
    *   Objekt C-692
    *   Rahmenauftrag C-695
    *   Stundenforderung C-702
    *   Tabelle C-700
    *   veranschlagte Mengen C-699
    *   zugeordnete Aufträge C-696
    *   zugeordnete Bestellungen C-697
*   **Abweichende Anschriften (Register in Dokumentenverwaltung)** C-424
*   **AE** siehe Auftragserfassung
*   **Alarmspinne** C-483
*   **Allgemein (Register in Erweiterte Einstellungen)** C-666
*   **Alternativangebotsübersicht** C-330
*   **Alternative**
    *   alle Gläser ersetzen C-337
    *   Angebot C-329
    *   Position C-329
    *   Position erfassen C-331
    *   Rechnung C-144
    *   Sprossen, Modell, Bearbeitung C-338
    *   zu Angebot erfassen C-334
*   **Alternative (Register in Alternativen)** C-403
*   **Alternativen**
    *   Alternative C-403
    *   Bearbeitungen/Modelle C-405
    *   Menü Funktionen C-400
    *   Menü Optionen C-399
    *   Original C-401
    *   Sprossen C-406
    *   Texte C-404
    *   Übersicht C-407
*   **Alternativen (Angebot)** C-399
*   **Anfrage**
    *   Schnellanfrage C-587
*   **Angebot**
    *   Alternative C-329
    *   Alternative erfassen C-334
    *   Alternativen C-399
    *   auswerten C-350
    *   automatische Benachrichtigung aktivieren C-344
    *   Erfolgsquote C-349
    *   Optimierung C-330
    *   Statistik C-397
    *   Übersicht C-392
    *   Wiedervorlage C-343, C-394
    *   Wiedervorlage abfragen C-345
*   **Angebotsstatistik** C-397
*   **Anhang**
    *   hinzufügen C-57
*   **Anlage (Register in Dokumentenverwaltung)** C-435
*   **Anlagen (Register in Artikel-Info)** C-606
*   **Anlagen (Register in Positionserfassung)** C-514
*   **Anschrift (Dokumentenverwaltung)** C-419
*   **Anwenderstatus** C-224
*   **Anzahlung**
    *   erfassen C-277
    *   fakturierte C-275
    *   mit Fakturierung erfassen C-277
    *   öffnen C-279
    *   ohne Fakturierung erfassen C-279
    *   Position C-276
*   **Anzahlungen (Dialog)** C-673
*   **Anzahlungsdruck** C-673
*   **Anzahlungsrechnung** C-275
*   **Anzahlungssumme** C-521
*   **Anzahlungsübersicht** C-276, C-561
*   **Anzeige**
    *   Artikel-, Kunden-, Lager-Info C-38
    *   Dokumentenansicht C-320
    *   Übersichten C-38
*   **Archiv**
    *   Dokument zurückholen C-248
*   **Archivierung**
    *   automatisch C-370
    *   Dokument C-370
    *   Dokumente übergeben C-371
    *   manuell C-370
    *   mehrfach C-370
    *   ohne Rechnungsnummer C-371
    *   Referenzprüfung C-370
*   **Artikel**
    *   fixiert C-70
*   **Artikel fixieren** C-610
*   **Artikel-Info**
    *   Anlagen C-606
    *   Info C-603
    *   Preise C-604
*   **Artikel-Informationen (Dialog)** C-602
*   **Auftrag**
    *   Anzahlung C-275
    *   Bestellposition C-297
    *   Dokument C-29
    *   erfassen C-50
    *   Faktura bei Teillieferung C-259
    *   Festpreis festlegen C-153
    *   importieren C-377
    *   Kopfdaten C-43
    *   manuelle Preisänderung C-140
    *   Nummernkreis C-29
    *   Position C-69, C-92
    *   Position erfassen C-95
    *   Rechnung C-33
    *   Reklamation C-282
    *   Schnellanfrage C-94, C-101
    *   Schnittstellen C-31
    *   Sperrkennzeichen C-32
    *   Steuer C-34
    *   Teillieferung C-257
    *   Termine C-45
    *   Text erfassen C-54
    *   überrechnen C-676
    *   zum Objekt C-696
    *   Zuschläge C-146
*   **Auftrag (Menü)** C-670
*   **Auftrags-/Bestell-Info** C-562
*   **Auftragsbestätigung**
    *   drucken C-203
*   **Auftragsbezogen (Register in Suchdialog)** C-524
*   **Auftragskopf**
    *   Geschäftsart C-44
*   **Auftragsposition** C-92
    *   kostenlos C-709
*   **Ausgangs-Journal** C-725
*   **Auswahl**
    *   nach Klassifikatoren (Register in Produktsuche) C-586
    *   nach Produkt (Register in Produktsuche) C-583
    *   nach technischen Parametern (Register in Produktsuche) C-585
*   **Auswertung**
    *   Deckungsbeitrag C-710
    *   Kalkulatorische Frachtkosten C-714
*   **Auswertungen**
    *   Null-Preisreport C-709
*   **Auswertungen (Auftrag)** C-707
*   **Automatisch**
    *   Archivierung C-370
    *   Wiedervorlage von Angeboten C-344
*   **AV-Bereich**
    *   Geschäftsart (Dokumentenkopf) C-44

### B
*   **Bankbelege**
    *   Wechseldruck Verwaltung C-674
*   **Bearbeitung**
    *   als Vorlage speichern C-170
    *   in Position erfassen C-117
*   **Bearbeitungen**
    *   Abkleben C-483
    *   Alarmspinne C-483
    *   Beschichtung C-478
    *   Biegen (Glas) C-480
    *   Durchsprechöffnung C-476
    *   Eckausschnitte C-474
    *   Emaillierung C-482
    *   Entschichtung C-483
    *   Flächen-Emaillierung C-478
    *   Handgriffe C-476
    *   Innenausschnitte C-476
    *   Kantenbearbeitung C-470
    *   Kantenschutz C-481
    *   Kolorieren C-478
    *   Lochbohrung C-471
    *   Logo C-481
    *   Mattierung C-478
    *   Nachschleifen C-481
    *   Parameter C-469
    *   Randentschichtungen C-480
    *   Randsiebdruck C-484
    *   Rillenschliff C-480
    *   Rundecken C-473
    *   Sandstrahlen C-478
    *   Schaltflächen C-66
    *   Schrägschnitte C-474, C-475
    *   Senkbohrung C-472
    *   Siebdruck C-478
    *   SN Makro C-482
    *   Stempel C-481
    *   Stufenbohrung C-473
    *   Verklebung C-470
*   **Bearbeitungen (Positionserfassung)** C-468
*   **Bearbeitungen/Modelle (Register in Alternativen)** C-405
*   **Bedienelemente**
    *   Dokumentenverwaltung C-40
    *   Positionserfassung C-61
    *   Voreinstellungen C-61
*   **Beispiel**
    *   bohrpunkt-symmetrisch C-72
    *   feld-symmetrisch C-72
    *   Lieferdauer C-46
    *   Nummernkreise C-30
*   **Benachrichtigung**
    *   Terminänderung C-568
*   **Berechnung**
    *   Bohrung für Sprossen C-72
    *   Lieferdauer C-46
    *   Preise im Auftrag C-141
    *   Sprossenkonstruktion C-72
*   **Beschichtung** C-478
*   **Bestandslisten**
    *   Nummernbereiche C-728
    *   Warengruppen C-730
*   **Bestandslisten (Menü)** C-728
*   **Bestellnummern (Register in Bestellübergabe)** C-657
*   **Bestellpool (Register in Bestellübergabe)** C-659
*   **Bestellübergabe**
    *   Bestellnummern C-657
    *   Bestellpool C-659
    *   Erweiterte Einstellungen C-665
    *   Lieferant/Termin ändern C-662
    *   Markierungsoptionen C-663
    *   Menü Funktionen C-654
    *   Menü Optionen C-655
    *   Preisvergleich C-664
    *   Stücklistenübersicht C-669
*   **Bestellung**
    *   Bestellübergabe C-300
    *   Kennzeichen ändern C-310
    *   Lieferanten ändern C-306
    *   Lieferantenauswahl C-300
    *   Lieferantenkartei C-298
    *   Position C-315
    *   Position im Auftrag C-297
    *   Preisvergleich C-308
    *   Produktkennzeichen C-297
    *   Referenzen C-316
    *   Übergabe C-654
    *   übergeben C-302
    *   zum Objekt C-697
*   **Biegen (Glas)** C-480
*   **Bleiverglasung** C-483, C-490
*   **Bohrpunkt**
    *   Beispiel C-72
*   **Bruttotage** C-209

### D
*   **Darstellungskonventionen** C-19
*   **Datei**
    *   anhängen C-57
*   **Datenübergabe**
    *   FiBu C-355
    *   Übergabedatei C-357
*   **Deckungsbeitrag**
    *   Analyse C-710
*   **Detailübersicht (Register in Suchdialog)** C-531
*   **Dialog**
    *   Preisanzeigen C-138
*   **Direktdruck** C-195
*   **Direkthilfe** C-62
*   **Dokument**
    *   ändern C-37
    *   Angebot C-329, C-392
    *   anhängen C-57
    *   Anzahlung C-275
    *   Anzahlung suchen C-279
    *   anzeigen C-548
    *   Auftrag C-29
    *   aus dem Archiv zurückholen C-248
    *   Bestellung C-314
    *   Dokumentendaten C-738
    *   doppelt erfasst C-37, C-386
    *   Erfassung C-35
    *   Festpreis erfassen C-153
    *   Folgedokument C-27
    *   Formular C-191
    *   Gutschrift C-291
    *   Historie C-217
    *   Historie prüfen C-219
    *   Journal C-384
    *   Kopfdaten C-43, C-409
    *   Kopie aus dem Archiv C-247
    *   kopieren C-532
    *   Kopieren (Dialog) C-248
    *   löschen C-53
    *   manuelle Statusvergabe C-236
    *   Nummernkreis C-29
    *   Nummernverwalter ändern C-188
    *   Organisation im Ablauf C-181
    *   Positionen C-440
    *   Positionserfassung C-452
    *   Positionspreis C-92
    *   positionsweise kopieren C-252
    *   referenzierte Dokumente C-319
    *   Reklamation suchen C-284
    *   Status C-221
    *   suchen C-52
    *   Teillieferung C-256
    *   Teillieferung erfassen C-260
    *   Teillieferung suchen C-265
    *   Text erfassen C-54
*   **Übersicht in Objektverwaltung** C-701
*   **Verkauf** C-27
*   **vollständig kopieren** C-248
*   **Dokument (Register in Dokumentenverwaltung)** C-418
*   **Dokument (Register in Fremddokumentenverwaltung)** C-689
*   **Dokumente kopieren**
    *   Kopieren 1 zu 1 C-536
    *   Menü Optionen C-532
    *   Menü Übersichten C-534
    *   Optionen Quelldokument C-546
    *   Optionen Zieldokument C-544
    *   positionsweise C-542
    *   Texte C-547
*   **Dokumentendaten** C-737
    *   Dokument C-738
    *   Menü Funktionen C-737
    *   Menü Optionen C-737
*   **Dokumentenexport**
    *   Formulardruck C-649
*   **Dokumentenüberwachung** C-386
*   **Dokumentenverwaltung**
    *   Abweichende Anschriften C-424
    *   Alternativangebotsübersicht C-407
    *   Anhang C-435
    *   Anzahlungsübersicht C-561
    *   Auftrags-/Bestell-Info C-562
    *   Bedienelemente C-40
    *   Dokument C-418
    *   Dokument löschen C-53
    *   Dokumentenkopf C-409
    *   Duplikate C-564
    *   Historie C-552
    *   Infos C-522
    *   Interne Kontrolle C-718
    *   Kalkulatorische Frachtkosten C-574
    *   Kapazitätsinfo C-570
    *   Kapazitätsübersicht C-550
    *   Konditionen C-429
    *   Kopfdaten erfassen C-50
    *   Kosten-/Aufschlagskalkulation C-575
    *   Kosten-/Aufschlagskalkulation (Position) C-613
    *   Kreditlimitsperre C-573
    *   Kundeninfo C-438
    *   Lieferterminkontrolle C-565
    *   Menü Ansicht C-410, C-441
    *   Menü Aufbau C-416, C-450
    *   Menü Customizing C-416, C-451
    *   Menü Druck C-409, C-441
    *   Menü Funktionen C-411, C-443
    *   Menü Optionen C-414, C-445
    *   Menü Start C-441
    *   NV Auswahl C-555
    *   OP Abfrage C-572
    *   Optionen zur Bedienung C-41
    *   Positionen C-452
    *   Produktion C-410
    *   Referenzen C-522
    *   Reklamationsübersicht C-560
    *   Startmodus C-41
    *   Statusänderung C-554
    *   Statusrückmeldung C-576
    *   Summen C-518
    *   Technische Parameter C-436
    *   Teillieferungen C-616
    *   Teillieferungsübersicht C-558
    *   Texte C-433
    *   Zusatz C-426
*   **Druck** C-637
    *   Direktdruck C-195
    *   Dokumentenexport C-649
    *   Druckauftrag C-195
    *   Druckmodus C-193
    *   Einstellung für Modelle C-197
    *   Einstellung für Sprossen C-197
    *   Einstellungen für Preis C-202
    *   Etiketten (Dokumente) C-647
    *   Formular C-191
    *   Formular-/Etikettendruck (Dialog) C-640
    *   Formulare (Dokumente) C-641
    *   Kalkulatorische Frachtkosten C-715
    *   Modus C-639
    *   Preisdarstellung C-200
    *   Rechnung C-194
    *   Skizze C-196
    *   Stückliste C-196
    *   vermaßte Skizze C-198
    *   Vermaßte Skizze (Dialog) C-650
    *   Voreinstellungen C-196
*   **Druckauftrag** C-195
*   **Drucken**
    *   Auftragsbestätigung, Rechnung, Lieferschein C-203
    *   Etiketten C-204
    *   Formular C-203
    *   Lieferschein, Rechnung, Teilrechnung C-203
*   **Duplikate**
    *   anzeigen C-564
*   **Durchsprechöffnung** C-476

### E
*   **Eckausschnitte** C-474
*   **Eingangs-Journal** C-725
*   **Einkaufsforderung** C-703
*   **Einstellungen**
    *   FiBu-Übergabe C-684
*   **Emaillierung** C-482
*   **Entschichtung** C-483
*   **Erfassen**
    *   Auftrag C-50
*   **Erfassung**
    *   automatisiert C-92
    *   Daten über Nummernblock eingeben C-41
    *   Dokument C-35
    *   Kreditlimit C-47
    *   Makro C-161
    *   Position C-95
    *   Position über Schnellerfassung C-100
    *   Schnellanfrage C-94
    *   Schnellanfrage beantworten C-101
    *   Schnellerfassung C-93
    *   Stückliste C-70
    *   über Nummernblock C-41
*   **Erfolgsquote** C-349
    *   auswerten C-350
*   **Erlöskonten** C-358
*   **Erweiterte Einstellungen**
    *   allgemein C-666
    *   Bestellübergabe C-665
    *   Sortierung C-667
*   **Etiketten**
    *   Druck (Dokumente) C-647
    *   drucken C-204
*   **Exklusiv-Status**
    *   Mitarbeiterverwaltung C-242
*   **Explizit (Preisdarstellung)** C-462
*   **Export**
    *   Zahlungen C-685

### F
*   **Fachberater=Erfasser (AE)** C-415
*   **Fälligkeit**
    *   Berechnung C-209
    *   Bezugsdatum C-210
    *   Kennzeichen C-209
*   **Festpreis**
    *   für gesamte Position C-155
    *   für gesamten Auftrag C-153
    *   für mehrere Positionen C-153
    *   in Position C-153
    *   pro Stück festlegen C-155
*   **FiBu**
    *   Datenübergabe C-355
    *   OP-Meldung C-360
    *   Rechnung übergeben C-361
    *   Tagesabschluss C-356
    *   Übergabedatei C-357
*   **FiBu-Übergabe**
    *   Auftrag, Gutschrift C-679
    *   Einstellungen C-684
    *   Menü Funktionen C-680
    *   Menü Optionen C-680
    *   Verkauf - Sollstellung C-682
    *   Verkauf, Einkauf C-682
*   **Firmendaten**
    *   Erlöskonten C-358
*   **Fixierter Artikel** C-70
*   **Fixierter Preis** C-142
*   **Flächen-Emaillierung** C-478
*   **Folgedokument** C-27
*   **Forderung**
    *   Historie C-706
*   **Forderung, Forderungsberechnung** C-704
*   **Formular**
    *   drucken C-203
*   **Formular-/Etikettendruck** C-637
    *   drucken C-203
    *   Etiketten drucken C-204
    *   Gruppe Druckmodi C-639
    *   Menü Funktionen C-637
    *   Menü Optionen C-638
*   **Formulardruck**
    *   Übertragungspool C-649
*   **Formulardruck (Dokumente)** C-641
*   **Fremddokumente (Import Dokumente)** C-689
*   **Fremddokumentenverwaltung**
    *   Dokument C-689

### G
*   **Gebogenes Glas** C-483, C-488
*   **Globale Änderungen (Positionserfassung)** C-595
*   **Gruppe**
    *   Druckmodi (Formular-/Etikettendruck) C-639
*   **Gutschrift**
    *   erfassen C-291
*   **Gutschrift (Menü)** C-723

### H
*   **Handgriffe** C-476
*   **Hilfe**
    *   Direkthilfe C-62
    *   Tooltipp C-62
*   **Historie** C-217, C-552
    *   prüfen C-219
*   **Referenzen** C-218

### I
*   **Implizit**
    *   Preisdarstellung C-462
    *   pro Mengeneinheit C-462
*   **Import**
    *   Auftrag C-377
    *   Dokument C-377
    *   Fremddokumente C-689
    *   Kundenauftrag C-688
    *   Zahlungen C-685
*   **Importieren**
    *   automatisch C-379
    *   Kundenauftrag C-377
    *   manuell C-381
*   **Info (Register in Artikel-Info)** C-603
*   **Innenausschnitte** C-476
*   **Interne Kontrolle**
    *   Änderungen am Kundenstamm C-719
    *   Gutschriftgründe C-718
    *   Lieferung C-721
    *   Rabatt-/Preisänderungen C-720
*   **ISO (Register in Positionserfassung)** C-452

### J
*   **Journal** C-384, C-725
    *   Ausgangs-Journal C-725
    *   Eingangs-Journal C-725

### K
*   **Kalkulatorische Frachtkosten** C-574
    *   Druck C-715
    *   Speditionskosten C-716
*   **Kantenbearbeitung** C-470
*   **Kantenschutz** C-481
*   **Kapazitäten**
    *   Information C-570
*   **Kapazitätsübersicht** C-550
*   **Katalog** C-71
*   **Keine Meldung bei Fehlern in Preisfindung** C-447
*   **Kennzeichen**
    *   Fälligkeit C-209
    *   für Bestellung ändern C-310
*   **Klassifikatoren**
    *   in Positionserfassung C-517
*   **Kolorieren** C-478
*   **Kommission (Positionserfassung)** C-456, C-457
*   **Konditionen (Anzeige)** C-597
*   **Konditionen (Register in Dokumentenverwaltung)** C-429
*   **Konstruktionstyp**
    *   Sprossen C-73
*   **Kopfdaten** C-43
    *   erfassen C-50
*   **Kopieren**
    *   Dokument C-248, C-532
    *   Dokument aus dem Archiv C-247
    *   Makro C-166
    *   Nummernverwalter C-186, C-634
    *   Position C-92, C-133
    *   Positionen aus Dokument C-252
    *   Statusänderung C-247
*   **Korrekturen** C-37
*   **Kosten-/Aufschlagskalkulation** C-575, C-613
*   **Kreditlimit**
    *   Auftrag C-47
    *   Status C-49
    *   Vorauskasse C-49
*   **Kreditlimitsperre**
    *   löschen C-573
*   **Kunde übernehmen (AE)** C-415
*   **Kundenauftrag**
    *   importieren C-377
*   **Kundeninfo** C-549
*   **Kundeninfo (Register in Dokumentenverwaltung)** C-438
*   **Kundenobjekt (AE)** C-431
*   **Kundenobjekte** C-692
*   **Kundenposition (Positionserfassung)** C-456, C-457
*   **Kurs (AE)** C-432

### L
*   **Lagerinfo**
    *   Dokumentenübersicht C-746
    *   Lagersuche C-742
    *   zukünftiger Lagerbestand C-745
*   **Lagersuche** C-741
    *   Dokumentenübersicht C-746
*   **Lagersuche (Register in Lagerinfo)** C-742
*   **Leistung**
    *   in Position erfassen C-129
    *   in Position löschen C-130
*   **Leistungserfassung (Register in Positionserfassung)** C-502
*   **Lieferant**
    *   in Bestellung ändern C-306
*   **Lieferant / Name / Lieferantenobjekt (AE)** C-431
*   **Lieferant und Liefertermin ändern (Dialog)** C-662
*   **Lieferdauer**
    *   Beispiel C-46
    *   Berechnung C-46
*   **Lieferschein**
    *   drucken C-203
*   **Liefertermin**
    *   ändern C-321, C-579
    *   Benachrichtigung C-323
    *   prüfen C-321
*   **Liefertermin nach Touren suchen (AE)** C-414
*   **Lieferterminbestimmung** C-578
*   **Lieferterminkontrolle** C-565
*   **Lieferung**
    *   erfassen C-260
*   **Lieferanschrift** C-44
*   **Lieferdaten** C-319
*   **Lieferschein** C-44
*   **Terminkontrolle** C-320, C-565
*   **Lochbohrung** C-471
*   **Logo** C-481
*   **Löschen**
    *   Dokument C-53
    *   Position C-134
    *   Stücklisten-Komponente in Position C-133

### M
*   **Mahnstufe**
    *   setzen C-215
*   **Mahnung** C-207
    *   erfassen C-215
*   **Mahnstufen** C-735
*   **Mahnwesen** C-733
*   **offene Posten** C-736
*   **Makro** C-159
    *   ändern C-164, C-624
    *   kopieren C-627
    *   löschen C-168
    *   Position erfassen C-163
    *   sichern C-623
    *   speichern C-161
    *   suchen C-626
*   **Makro kopieren** C-166
*   **Makros** C-623
*   **Markierungsoptionen (Bestellübergabe)** C-663
*   **Mattierung** C-478
*   **Menge**
    *   in der Positionserfassung ändern C-69
*   **Menü**
    *   Ansicht (Dokumentenverwaltung) C-410, C-441
    *   Aufbau (Dokumentenverwaltung) C-416, C-450
    *   Customizing (Dokumentenverwaltung) C-416, C-451
    *   Druck (Dokumentenverwaltung) C-409, C-441
    *   Funktionen (Alternativen) C-400
    *   Funktionen (Bestellübergabe) C-654
    *   Funktionen (Dokumentendaten) C-737
    *   Funktionen (Dokumentenverwaltung) C-411, C-443
    *   Funktionen (FiBu-Übergabe) C-680
    *   Funktionen (Formular-/Etikettendruck) C-637
    *   Funktionen (Nummernverwalter) C-629
    *   Optionen (Alternativen) C-399
    *   Optionen (Bestellübergabe) C-655
    *   Optionen (Dokumente kopieren) C-532
    *   Optionen (Dokumentendaten) C-737
    *   Optionen (Dokumentenverwaltung) C-414, C-445
    *   Optionen (FiBu-Übergabe) C-680
    *   Optionen (Formular-/Etikettendruck) C-638
    *   Start (Dokumentenverwaltung) C-441
    *   Übersichten (Dokumente kopieren) C-534
*   **Mindestwert**
    *   Rechnung C-145
*   **Mitarbeiter (Dokumentenverwaltung)** C-420
*   **Modell**
    *   als Vorlage speichern C-170
    *   aus SN-Datei übernehmen C-173
    *   Bearbeitung erfassen C-112
    *   Datei C-171
    *   in Position erfassen C-112
    *   Katalog C-71
    *   Maße erfassen C-96
    *   Skizzendruck C-197
    *   SN-Datei übernehmen C-175
    *   Stufung erfassen C-114
    *   Template übernehmen C-177
*   **Modell/Bearbeitungen (Positionserfassung)** C-465
*   **Modell-Template** C-491
*   **Modul**
    *   Funktion C-17
*   **Monatsrechnung** C-33
*   **Muster (Register in Sprossen)** C-501

### N
*   **Nachschleifen** C-481
*   **Nettopreiserfassung (AE)** C-415
*   **Neuerfassung als Standard (AE)** C-415
*   **Null-Preisreport** C-709
*   **Nummernbereiche**
    *   Bestandlisten C-728
*   **Nummernblock** C-41
*   **Nummernkreis**
    *   Beispiel C-30
*   **Nummernkreise** C-29
*   **Nummernverwalter** C-180, C-629
    *   Bestellkennzeichen ändern C-310, C-635
    *   Druckmodus C-193
    *   erstellen C-183
    *   kopieren C-186, C-634
    *   leeren C-187
    *   Menü Funktionen C-629
    *   Sortierung C-633
    *   überschreiben C-187
    *   Zuordnung im Dokument ändern C-188
*   **Nummernverwalter (Dialog)** C-631
*   **NV Auswahl (Dokumentenverwaltung)** C-555

### O
*   **Objekt**
    *   Abrechnung C-692
*   **Objektverwaltung** C-692
    *   aufgelaufene Summen C-698
    *   Forderung C-704
    *   Forderungshistorie C-706
    *   Rahmenauftrag C-695
    *   Tabelle C-700
    *   veranschlagte Mengen C-699
    *   zugeordnete Aufträge C-696
    *   zugeordnete Bestellungen C-697
    *   zugeordnete Dokumente C-701
*   **Offene Posten** siehe OP
*   **OP-Abfrage** C-572
*   **Optionen (Register in Suchdialog)** C-529
*   **Optionen Quelldokument (Register in Dokumente kopieren)** C-546
*   **Original (Register in Alternativen)** C-401

### P
*   **Plausibilitätsprüfung** C-63
*   **Position**
    *   als SN-Datei speichern C-173
    *   Alternative C-329
    *   alternative Position erfassen C-331
    *   Anzahlung C-276
    *   Auftrag C-92
    *   automatisiert erfassen C-92
    *   bearbeiten C-133
    *   Bearbeitung erfassen C-117
    *   Bestellung ändern C-133
    *   erfassen C-95
    *   Festpreis eingeben C-155
    *   Festpreis pro Stück C-155
    *   hinzufügen C-133
    *   kopieren C-133, C-611
    *   Leistung erfassen C-129
    *   Leistung löschen C-130
    *   löschen C-134
    *   mit Makro erfassen C-163
    *   Modell erfassen C-112
    *   Preis/PE ändern C-146
    *   Preise C-92
    *   regelmäßige Sprossenkonstruktion C-107
    *   Schnellanfrage C-94
    *   Schnellanfrage beantworten C-101
    *   Schnellerfassung C-100
    *   SN-Datei übernehmen C-175
    *   Sprossen erfassen C-107
    *   Sprossenpreis ändern C-146
    *   Status C-228
    *   Stückliste erweitern C-117
    *   Stücklistenaufbau ändern C-130
    *   Stücklisten-Komponente löschen C-133
    *   Stufung erfassen C-114
    *   unregelmäßige Sprossenkonstruktion C-110
    *   Verfügbarkeit von Produkten prüfen C-104
*   **Position kopieren** C-611
*   **Positionsbezogen (Register in Suchdialog)** C-525
*   **Positionserfassung**
    *   Anlagen C-514
    *   Artikel fixieren C-610
    *   Bearbeitungen C-468
    *   Bedienelemente C-61
    *   Bleiverglasung C-490
    *   Dokument anzeigen C-548
    *   Eingabemodus C-62
    *   Erfassungszeile C-69, C-456
    *   gebogenes Glas C-488
    *   Infos C-582
    *   ISO C-452
    *   Klassifikatoren C-517
    *   Konditionen C-597
    *   Kundeninfo C-549
    *   Leistungserfassung C-502
    *   Makro C-623
    *   Modell/Bearbeitungen C-465
    *   Modell-Template C-491
    *   Positionen C-440
    *   Preisrecorder C-608
    *   Produktion C-442
    *   Prüfungen C-63
    *   Referenzen C-582
    *   Reklamation C-591
    *   Schaltflächen C-65
    *   Sprossen C-493
    *   Startmodus C-62
    *   Stückliste - Ergänzungen C-607
    *   Stufung C-487
    *   Symbole C-64
*   **Technische Werte** C-515
*   **Texte** C-512
*   **Versicherungsleistung** C-614
*   **Weitere Angaben** C-508
*   **Zusatz** C-504
*   **Positionserfassung (Dialog)** C-451
*   **Positionsweise (Register in Dokumente kopieren)** C-542
*   **Preis**
    *   Anzeigen im Dialog C-138
    *   Austauschglas ändern C-146
    *   Berechnungseinstellung C-141
    *   Darstellung im Druck C-200
    *   Druckeinstellungen C-202
    *   Festpreis erfassen C-153
    *   fixieren C-142
    *   Formel C-144
    *   im Auftrag manuell ändern C-140
    *   Preisrecorder C-143
    *   Sprossenpreis ändern C-151
    *   Stücklistenpreis ändern C-150
    *   Vergleich im Bestellpool C-308
    *   Zuschlag im Auftrag C-146
*   **Preis/PE**
    *   in Position ändern C-146
*   **Preisänderungsreport** C-707
*   **Preisdruck**
    *   Einstellungen C-201
*   **Preise (Register in)**
    *   Artikel-Info C-604
    *   Sprossen C-498
*   **Preisfindung**
    *   Stückliste C-463
*   **Preisrecorder** C-143, C-608
*   **Preisvergleich (Bestellübergabe)** C-664
*   **Produkt** C-69
    *   Bestellkennzeichen C-297
    *   Verfügbarkeit prüfen C-104
*   **Produktfeld**
    *   Schnellerfassung C-93
*   **Produktion**
    *   Datenübergabe C-31
    *   Dokumentenverwaltung C-410
    *   Positionserfassung C-442
    *   Rückmeldung C-235
*   **Produktionsstücklistenauflösung** C-596
*   **Produktsuche** C-582
    *   nach Klassifikatoren C-586
    *   nach Produkt C-583
    *   nach technischen Parametern C-585
*   **Prüfung**
    *   Bestellübergabe C-300
*   **Prüfungen**
    *   Positionserfassung C-63
    *   Verarbeitungsgeschwindigkeit C-63

### R
*   **Rahmenauftrag**
    *   Forderung C-704
*   **Randausschnitte** C-475
*   **Randentschichtungen** C-480
*   **Randsiebdruck** C-484
*   **Rechnung**
    *   Alternativen C-144
    *   an FiBu übergeben C-361
    *   Dokument C-33
    *   Druck C-194
    *   drucken C-203
    *   Faktura bei Teillieferung C-259
    *   Mahnung C-207, C-211
    *   Mahnung senden C-215
    *   Mindestwert C-145
    *   Monatsrechnung C-33
    *   Sammelrechnung C-33
    *   Teilrechnung C-33
    *   Zahlungseingang C-207, C-211
    *   Zahlungseingang erfassen C-212
    *   Zahlungsplan C-34
*   **Rechnungslegungstag**
    *   in Auftragserfassung C-432
    *   Zahlungszielberechnung C-209
*   **Reklamation** C-282
    *   erfassen C-285
    *   Grund, Verursacher C-283
    *   öffnen C-284
*   **Reklamation (Positionserfassung)** C-591
*   **Reklamationsübersicht** C-284, C-560
*   **Rillenschliff** C-480
*   **Rückmeldung** C-235
*   **Rundecken** C-473

### S
*   **Sammelrechnung** C-33
*   **Sandstrahlen** C-478
*   **Schaltflächen**
    *   Bearbeitungen C-66
    *   Positionserfassung C-65
    *   Suche C-42
*   **Schnellanfrage** C-94, C-101, C-587
    *   Daten in Auftrag übernehmen C-102
*   **Schnellerfassung**
    *   Regeln C-93
*   **Schnittstellen**
    *   Auftrag C-31
*   **Schrägschnitte** C-474
*   **Senkbohrung** C-472
*   **Siebdruck** C-478
*   **Skizze**
    *   Druck C-196
    *   vermaßte Skizze C-198
*   **SN Makro** C-482
*   **SN-Datei**
    *   aus Position speichern C-173
    *   erstellen C-170
    *   in Position übernehmen C-175
    *   speichern C-173
*   **Sollstellung (Register in FiBu-Übergabe)** C-682
*   **Sortierung**
    *   Bestellübergabe C-667
    *   Nummernverwalter C-633
*   **Sperrkennzeichen** C-32, C-227
    *   zuordnen C-230
*   **Sprossen** C-493
    *   Gitterpreis ändern C-151
    *   in Position erfassen C-107
    *   Muster C-501
    *   Preis ändern C-151
    *   Preis in Position ändern C-146
    *   Preise C-498
    *   Skizzendruck C-197
    *   Wegfallsprossen C-500
*   **Sprossen (Register in Alternativen)** C-406
*   **Sprossenkonstruktion** C-71
    *   Bohrung C-72
    *   Typ C-73
*   **Stammdaten**
    *   Anwenderstatus C-224
    *   automatische Statusvergabe C-234
*   **Statistik**
    *   Dokumente übergeben C-365
    *   Übergabe C-364
*   **Status**
    *   ändern C-236
    *   Anwenderstatus C-224
    *   automatische Statusvergabe C-234
    *   Dokument C-221
    *   Exklusiv-Status C-226
    *   Exklusiv-Status zulassen C-242
    *   interne Prozesse C-222
    *   Kreditlimit C-49
    *   manuelle Statusvergabe C-236
    *   mehrere Dokumente ändern C-238
    *   Mindeststatus C-226
    *   Position C-228
    *   Rechte über Mitarbeiterrechte C-242
    *   Sperrstatus C-226
    *   Statuserhöhung C-233
    *   Statuspunkt C-223
    *   Statuspunkt zuordnen C-229
    *   Statusvergabe C-232
    *   Statusverwaltung C-224
    *   Statuszuordnung C-225
*   **Statusänderung** C-554
*   **Statusrückmeldung** C-576
*   **Statuszeile**
    *   Hilfetext C-62
*   **Stempel** C-481
*   **Steuer** C-34
*   **Struktur Ebene 1-6 (Positionserfassung)** C-450
*   **Stückliste**
    *   Druck C-196
    *   Komponente einfügen C-117
    *   Komponente in Position ändern C-130
    *   Komponente löschen C-133
    *   Positionserfassung C-461
    *   Preis in Position ändern C-150
    *   Zusatz C-607
*   **Stückliste (Register in Positionserfassung)** C-461
*   **Stücklistenaufbau**
    *   in Position ändern C-130
*   **Stücklistenbezogen (Register in Suchdialog)** C-526
*   **Stücklistenübersicht** C-669
*   **Stufenbohrung** C-473
*   **Stufung** C-487
    *   in Position erfassen C-114
*   **Stundenforderung** C-702
*   **Suche**
    *   auftragsbezogen C-524
    *   Detailübersicht C-531
    *   Dokument C-52
    *   Optionen C-529
    *   positionsbezogen C-525
    *   Produkt C-582
    *   Schaltflächen C-42
    *   stücklistenbezogen C-526
    *   Tabelle C-527
*   **Suche (Dokumente)** C-523
*   **Summen (Register in Dokumentenverwaltung)** C-518
*   **Summen zwangsweise errechnen** C-142
*   **Symbole**
    *   Positionserfassung C-64

### T
*   **Tabelle (Register in Suchdialog)** C-527
*   **Tagesabschluss** C-356, C-364
    *   Übergabedatum C-364
*   **Technische Parameter (Register in Dokumentenverwaltung)** C-436
*   **Technische Werte (Register in Positionserfassung)** C-515
*   **Teillieferung**
    *   Dokument C-256
    *   erfassen C-260
    *   Faktura C-259
    *   öffnen C-265
*   **Teillieferungen**
    *   Dokumentenverwaltung C-616
    *   pro Fertigmeldung/Wareneingang C-617
    *   pro Gestell C-620
*   **Teillieferungsübersicht** C-258, C-558
*   **Teilrechnung** C-33, C-259
    *   drucken C-203
*   **Template**
    *   für Position übernehmen C-177
    *   Modell C-171
*   **Termine**
    *   Änderung an den Kunden senden C-568
    *   Änderung in mehreren Dokumenten C-325
    *   Auftrag C-420
    *   Dokument C-45
    *   im Bestellpool ändern C-306
    *   Lieferdauer C-45
    *   übernehmen (AE) C-414
*   **Text**
    *   als Dateianhang C-49
    *   erfassen C-54
    *   Schriftgröße C-55
    *   zum Auftrag C-49
*   **Texte (Register in Alternativen)** C-404
*   **Texte (Register in Dokumente kopieren)** C-547
*   **Texte (Register in Dokumentenverwaltung)** C-433
*   **Texte (Register in Positionserfassung)** C-512
*   **Tooltipp** C-62
*   **Touren/Fahrer Zuordnung** C-653
    *   Druck C-653
*   **Typ**
    *   Sprossenkonstruktionstyp C-73

### U
*   **Übergabe**
    *   Archiv C-370
    *   Bestellung C-302
    *   Produktion C-31
    *   Rückmeldung C-235
    *   Statistik C-364
*   **Übergabe Archiv**
    *   Verkauf C-686
*   **Überrechnen** C-142, C-676
*   **Überschreiben**
    *   Nummernverwalter C-187
*   **Übersicht**
    *   Alternativangebote C-407
    *   Anzahlungen C-561
    *   Dokumente (Lagerinfo) C-746
    *   Kapazitäten C-550
    *   Kopie/Blatt/Info C-550
    *   Reklamationen C-560
    *   Statusrückmeldung C-576
    *   Stückliste C-669
    *   Teillieferungen C-558
*   **Übersichten**
    *   im Verkauf C-38

### V
*   **Verkauf**
    *   Angebot C-392
    *   Berechnung C-140
    *   Dokument C-27
    *   Folgedokument C-27
    *   Grundgedanken C-23
    *   Handlungsablauf C-24
    *   Informationen C-38
    *   Menü-Übersicht C-20
    *   Preise C-140
    *   täglicher Ablauf C-25
    *   Übersichten C-38
*   **Verklebung** C-470
*   **Verpackungseinheit (Positionserfassung)** C-507
*   **Versicherungsleistung** C-614
*   **Vorauskasse** C-47, C-275
*   **Vorauszahlung erfassen** C-277
*   **Vorgaben**
    *   Position löschen C-444
    *   Stücklistenposition löschen C-444
*   **Vorlage**
    *   für Modell speichern C-170
    *   für Modell übernehmen C-177
*   **Vorlage siehe Template**
*   **Vorlagen** C-71

### W
*   **Warengruppen**
    *   Bestandslisten C-730
*   **Wechseldruck Verwaltung** C-674
*   **Wegfallsprossen (Register in Sprossen)** C-500
*   **Weitere Angaben (Register in Positionserfassung)** C-508
*   **Weitere Optionen (Register in Dokumente kopieren)** C-544
*   **Wiedervorlage**
    *   abfragen C-345
*   **Wiedervorlage (Angebot)** C-343, C-394
*   **Wunschtermin übernehmen (AE)** C-414

### Z
*   **Zahltag** siehe Zahlungstag
*   **Zahlungseingang** C-207
    *   erfassen C-212
*   **Zahlungsplan** C-34
*   **Zahlungstag**
    *   in Auftragserfassung C-432
    *   Zahlungszielberechnung C-209
*   **Zahlungsweg (AE)** C-429
*   **Zahlungsziel**
    *   Berechnungsbeispiele C-210
    *   Zahlungsplan C-34
    *   Zahlungszielberechnung C-209
*   **Zukünftiger Lagerbestand (Register in Lagerinfo)** C-745
*   **Zusatz (Register in Dokumentenverwaltung)** C-426
*   **Zusatz (Register in Positionserfassung)** C-504
*   **Zuschlagsart (Positionserfassung)** C-463

