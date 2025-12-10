---
title: "D-HB-AWBusiness_35"
source: "D-HB-AWBusiness_35.pdf"
tags: ["A+W Business", "Software Reference", "ERP", "Crate Management", "Barcode Manager", "Inventory Management", "Order Processing", "German"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for A+W Business, covering modules for Crate Management and the Barcode Manager. It provides detailed instructions on inventory searches, future stock analysis, order placement, goods receipt and issue for crates, and barcode-based data entry."
long_description: "This comprehensive technical document serves as a software reference manual for the A+W Business enterprise resource planning (ERP) system. The guide is written in German and is divided into several key modules, primarily focusing on inventory and logistics management. The first major section, 'Kistenmanagement' (Crate Management), details functionalities such as 'Lagersuche' (Inventory Search) for future stock levels, allowing users to check material availability and lead times. It explains how to manage and place stock orders ('Lagerbestellung'), including workflows for order pools and supplier interactions. A significant part is dedicated to 'Kisten – Ein- und Ausgang' (Crate Goods Receipt and Issue), which outlines the procedures for registering incoming and outgoing crates, assigning unique identification numbers (Identnummern), and managing stock on a positional basis. The second major part of the document introduces the 'A+W Business Barcode Manager (EL)'. This section functions as a tutorial and reference for using barcode scanners for online shop floor data collection (BDE). It covers the initial setup and configuration of scanners, the creation of data entry points within A+W Business, and the functions available through the scanner interface, such as goods receipt, production reporting (completion and breakage), and various stock movements (withdrawal, receipt, transfer, and crate-specific operations). The manual includes numerous screenshots of the user interface, explanations of all fields and options, and step-by-step instructions for performing key tasks. It concludes with a detailed specification of the barcode formats used and a comprehensive alphabetical index for quick reference."
---

# Softwarereferenz

---
## Lagersuche – Zukünftiger Lagerbestand

*Lagerwirtschaft > Suche > Register Zukünftiger Lagerbestand*

*Abb. K-58: Lagersuche - Zukünftiger Lagerbestand*

In diesem Register können Sie prüfen, ob die Wiederbeschaffungszeiten für ein bestimmtes Produkt ausreichen, um einen Auftrag termingerecht ausliefern zu können. Die Farbe Rot zeigt an, dass die Termine nicht eingehalten werden können. Gelb zeigt an, dass die Wiederbeschaffungszeit ausreicht, sofern die Bestellungen termingerecht eintreffen.

Die Wiederbeschaffungszeit ergibt sich aus der Lieferzeit, die in der Lieferantenkartei für den Artikel hinterlegt ist, und aus den Tourentagen des Lieferanten, die in der Tourenverwaltung hinterlegt sind.

### Vorschau bis

Die Vorschau beginnt immer mit dem aktuellen Tagesdatum. Die Anzahl der Tage für die Vorschau stellen Sie in den Firmendaten ein, z. B. 14 Tage.
- In der oberen Übersicht werden die Daten in einer Zeile pro gewähltem Produkt aufgelistet.
- In der mittleren Übersicht werden die aktuellen Bestände pro Tag wiedergegeben.
- In der unteren Übersicht werden Details zum gewählten Produkt angezeigt.

Die Zeilen sind rot, wenn die Produktion nicht möglich ist, weil die Reservierungen den Bestand überschreiten.

Um die Performance zu erhöhen, können Sie die Anzeige der Vorschau durch folgende Einstellungen einschränken:
- Im Dialog *Produktverwaltung > Register Lager/Einkauf > Checkbox keine Verfügbarkeitsprüfung* können Sie bestimmte Artikel aus der Lagervorschau und der Verfügbarkeitsprüfung herausnehmen, indem Sie die Verfügbarkeitsprüfung für diese Artikel ausschalten.
- Im Dialog *Firmendaten* können Sie einstellen, über welchen Zeitraum die Vorschau dargestellt werden soll.
- Im Dialog *Lagerverwaltung* können Sie mehrere Lagermaße miteinander verknüpfen, damit die Bestandsprüfung nur für den definierten Lager-Hauptartikel durchgeführt wird.
  *⇨ "Hauptartikel" auf Seite K-3381*

## Lagerbestellung

*Lagerwirtschaft > Lagerbestellung*

In diesem Dialog können Sie alle vorgeschlagenen Lagerbestellungen prüfen und an den Einkauf übergeben.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menüs im Bestellpool" auf Seite K-3403
- "Bestellpool" auf Seite K-3406

### Menüs im Bestellpool

Über die Menüs können Sie automatisch die Datumsfelder aktualisieren lassen und zusätzlich andere Dialoge öffnen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite K-3403
- "Menü Optionen" auf Seite K-3404

### Menü Funktionen

*Lagerwirtschaft > Lagerbestellung > Menü Funktionen*

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Bestellübergabe zu schließen. Folgende Einträge werden angezeigt:
- **Lieferant/Liefertermin ändern:**
  Öffnet den Dialog Lieferant und Liefertermin ändern.
  *"Lieferant und Liefertermin ändern" auf Seite C-1949*
- **Markierungsoptionen:**
  Öffnet den Dialog Markierungsoptionen.
  *⇨ "Markierungsoptionen" auf Seite C-1950*
- **Lieferantenpreise:**
  Öffnet den Dialog Preisvergleich.
  *⇨ "Preisvergleich" auf Seite C-1951*

### Menü Optionen

*Lagerwirtschaft > Lagerbestellung > Menü Optionen*

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

> **Aktivierte Optionen nach dem Öffnen des Dialogs**
> Bitte beachten Sie, dass geänderte Optionen erst beim nächsten Öffnen des Dialogs wirksam werden.
> Wenn durch eine aktivierte Option eine Prüfung gestartet wurde, kann sich das Öffnen eines Dokuments verzögern. Der Grad der Verzögerung hängt von der Leistungsfähigkeit des Rechners ab.
> Die folgenden Beschreibungen stellen die aktivierte Option dar.

**Gruppe Übergabe**
- **Auftragsbezogene Übergabe:**
  Die Bestellungen werden pro Auftrag übergeben. Wenn diese Option nicht aktiviert ist, können Sammelbestellungen erzeugt werden.
- **Bestellnummer = Auftragsnummer:**
  Diese Option ist nur freigeschaltet, wenn die Option Auftragsbezogene Übergabe aktiviert ist.
- **Bestellpool pro Mitarbeiter:**
  Pro Mitarbeiter kann ein eigener Bestellpool angelegt werden.

**Gruppe Liefertermin**
- **Lieferterminprüfung:**
  Der Liefertermin wird automatisch geprüft. Ändern Sie einen Liefertermin, der nicht an einem Tourentag liegt, wird eine entsprechende Meldung angezeigt.
- **Lieferantentour berücksichtigen:**
  Wenn die Bestellung auf einen Liefertermin fällt, der nicht an einem Tourentag liegt, wird eine entsprechende Meldung angezeigt. Dazu müssen die Lieferantentouren in den Stammdaten hinterlegt werden.
  *⇨Stammdaten, "Touren" auf Seite B-995*
- **Vorlauftage mit Kombiwarengruppen ermitteln:**
  Wenn in den Kombiwarengruppen Vorlauftage hinterlegt sind, sollen diese zur Berechnung des Liefertermins herangezogen werden.
  *⇨ Stammdaten, "Vorlauftage" auf Seite B-681*

**Gruppe Produktbezeichnung**
- **Produktbezeichnungen aus Lieferantenkartei:**
  Die Bezeichnung der bestellten Produkte wird aus der Lieferantenkartei übernommen.
- **Produktbezeichnungen aus Basisdaten (interne Best.):**
  Für interne Bestellungen wird die Bezeichnung der bestellten Produkte aus den Produktstammdaten übernommen.

**Gruppe Sonstige**
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

**Gruppe Erweitert**
- **Einstellungen:**
  Öffnet den Dialog Erweiterte Einstellungen, um Angaben zum Druck von Texten und Dateianhängen festzulegen.

## Bestellpool

*Lagerwirtschaft > Lagerbestellung*

*Abb. K-59: Lagerbestellung*

In diesem Dialog können Sie alle vorgeschlagenen Bestellungen für Artikel sehen, deren Mindestbestand unterschritten wurde. Die Bestellmenge wird nach der Menge berechnet, die im Dialog Lagerverwaltung festgelegt ist.

Mit der Übergabe werden die Bestellungen angelegt und können gedruckt und versendet werden.
*⇨Tutorial, "Lagerbestellung von Kisten" auf Seite K-3355*
*⇨ Tutorial, "Manuelle und automatische Lagerbestellung" auf Seite K-3347*

### Lagerort

**Warenhaus, Gang, Regal, Fach** Sie können die Anzeige auf einzelne Lagerorte einschränken. Bedenken Sie dabei, dass auch auf den Lagerort <k.A.> Lagerartikel gebucht sein können. Wenn Sie die Auswahl nicht einschränken, werden Bestellvorschläge zu allen Artikeln angezeigt, deren Mindestbestand unterschritten ist.
Die Bezeichnung der Lagerorte kann in den Stammdaten geändert werden.

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
  *Verkauf, "Lieferant und Liefertermin ändern" auf Seite C-1949*
  *Verkauf, "Preisvergleich" auf Seite C-1951*

**Position für** Die Bestellvorschläge sind in unterschiedlichen Farben dargestellt:
- **Rot: interner Auftrag:**
  Interne Aufträge sind Produktionsaufträge, die erzeugt werden, um den Lagerbestand aufzufüllen. Der Vorschlag wird automatisch erzeugt, wenn in der Lieferantenkartei für das Produkt die entsprechende Option aktiviert ist.
- **Blau: Anfrage:**
  Bestellanfragen an einen Lieferanten, um z. B. Preise und Liefertermine zu erfragen.
- **Grün: Liefertermin für Auftr./Best. gefährdet:**
  Als Liefertermin wird automatisch das aktuelle Tagesdatum eingesetzt. Damit ist die Lieferung i. d. R. nicht termingerecht möglich. Wenn Sie das Datum ändern, wechselt die Schriftfarbe für den Eintrag zu Schwarz.

### Ziel-Nummernverwalter

**Mitarbeiter** Name des Mitarbeiters, der sich in A+W Business angemeldet hat oder der den Nummernverwalter eingerichtet hat. Wenn Sie einen neuen Nummernverwalter anlegen, können Sie diesen einem bestimmten Mitarbeiter zuweisen.

**Name** Name des Nummernverwalters, in den die Bestellungen übergeben werden sollen. Wenn Sie einen neuen Namen eintragen, wird ein neuer Nummernverwalter angelegt.

### Ziel-Nummernkreis

**Mandant** Wenn Sie für Ihre Mandanten gesonderte Nummernkreise eingerichtet haben, können Sie den gewünschten Mandanten auswählen.

**AV-Bereich** Wenn Sie mit AV-Bereichen arbeiten, können Sie die Bestellung einem bestimmten AV-Bereich zuordnen.

## Kisten – Ein- und Ausgang

Vollständige Beschreibungen von Wareneingang und Warenausgang finden Sie in den Parts Fertigung und Einkauf.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Wareneingang (Kisten)" auf Seite K-3409
- "Einstellungen (ID)" auf Seite K-3420
- "Warenausgang Kisten" auf Seite K-3421

### Wareneingang (Kisten)

*Dokumente > Bestellung > Wareneingang > Wareneingang*

In diesem Dialog können Sie den Wareneingang zu einzelnen Bestellungen oder zu den Bestellungen in einem Nummernverwalter erfassen.
Für die jeweilige Bestandsbuchung können Sie Vorgaben für die Identifikationsnummern (ID) festlegen, die automatisch vergeben wird, wenn in der Lagerbestellung Positionen mit einer Menge größer als 1 erfasst sind. Die Identnummern werden für Kisten und Gläser (Lagerplatten) vergeben.

> **Voraussetzung**
> In den Firmendaten muss die Checkbox für die virtuelle Vergabe von Positionsnummern markiert sein.
> *⇨ "Firmendaten" auf Seite K-3323*

In diesem Dialog finden Sie folgende Register:
- "Wareneingang – Auswahl" auf Seite K-3410
- "Wareneingang - Komplett" auf Seite K-3412
- "Wareneingang – Positionsweise" auf Seite K-3414
- "Wareneingang – Identnummer" auf Seite K-3417
- "Wareneingang – Protokoll (Identnummern)" auf Seite K-3419

### Wareneingang – Auswahl

*Dokumente > Bestellung > Wareneingang > Wareneingang > Register Auswahl*

*Abb. K-60: Wareneingang - Auswahl*

In diesem Register können Sie die Auswahl und Anzeige der Dokumente filtern, zu denen Sie Wareneingänge prüfen und/oder erfassen möchten.
*⇨Tutorial, "Wareneingang" auf Seite D-2154*

**Auswahl**
Mit der Wahl der Option legen Sie fest, wie die Bestellungen gefiltert werden. Die offenen Bestellungen werden nach der Suche im Register *Komplett* angezeigt, damit die Wareneingänge verbucht werden können.
- **Nach Bestellnummer:**
  Das Eingabefeld für die Bestellnummer wird freigeschaltet. Im Register *Komplett* werden die gesuchte Bestellung und alle referenzierten Aufträge angezeigt.
- **Nach Auftragsnummer:**
  Das Eingabefeld für die Auftragsnummer wird freigeschaltet. Im Register *Komplett* werden alle Bestellungen angezeigt, die zur eingetragenen Auftragsnummer erzeugt wurden.
- **Nach Lieferanten:**
  Das Eingabefeld für die Lieferantennummer wird freigeschaltet. Im Register *Komplett* werden alle Bestellungen beim gewählten Lieferanten angezeigt.
- **Nach Lieferscheinnummer / Lieferavis, Gesamtliefermenge:**
  Das Eingabefeld für die Nummer des Lieferscheins oder des Lieferavis und das Feld für die Gesamtmenge werden freigeschaltet. Wurde ein Lieferavis importiert, müssen die tatsächlich gelieferten Mengen eingetragen werden.
- **Nach Anliefertermin des Lieferanten:**
  Das Eingabefeld für den Liefertermin wird freigeschaltet. Im Register *Komplett* werden alle Bestellungen angezeigt, die zum gewählten Termin angeliefert werden sollen.
- **Nach Nummernverwalter:**
  Die Kombobox zur Auswahl des Nummernverwalters wird freigeschaltet. Im Register *Komplett* werden alle Bestellungen im gewählten Nummernverwalter angezeigt.
- **Nach Scanner / Dokument:**
  Die Felder für den Barcode der Bestellnummer oder einer Bestellposition werden freigeschaltet.

**Ziel-Nummernverwalter**

**Ziel-Nummernverwalter** Die Lagerbestellungen können nach dem Buchen des Wareneingangs automatisch in einen anderen Nummernverwalter gestellt werden.
Die Lagerbestellungen werden nicht in einen anderen Nummernverwalter gestellt.
Die Felder im Bereich Ziel-Nummernverwalter werden freigeschaltet. Die Lagerbestellungen werden in den gewählten Nummernverwalter gestellt.

**Mitarbeiter** Name des Mitarbeiters, dem der Ziel-Nummernverwalter zugeordnet ist.

**Nummernverwalter** Nummernverwalter, in den die Lagerbestellungen mit (vollständigen) Wareneingängen gestellt werden sollen.

### Wareneingang – Komplett

*Dokumente > Bestellung > Wareneingang > Wareneingang > Register Komplett*

*Abb. K-61: Wareneingang - Komplett*

In diesem Register werden alle Bestellungen angezeigt, die den Suchkriterien entsprechen. Wenn Sie eine Bestellung markieren, werden die referenzierten Aufträge aufgelistet.
*⇨Tutorial, "Wareneingang erfassen" auf Seite D-2161*

**Liefertermin**

**Anliefertermin des Lieferanten** Anzeige des aktuellen Tagesdatums. Sie können es überschreiben, wenn Sie eine Lieferung erfassen wollen, die vor diesem Datum eingetroffen ist. Das Datum wird nur für die Dokumente übernommen, die in der Übersicht markiert sind.

**AB-Lieferant** Sie können zu einem Wareneingang auch die Nummer der Auftragsbestätigung durch den Lieferanten erfassen.

**Dokumente**

Mit den Schaltflächen können Sie alle oder einige Dokumente markieren oder die Markierung entfernen.

In der Übersicht werden alle Bestellungen angezeigt, die den Suchkriterien im Register Auswahl entsprechen. Der vollständige Wareneingang wird für die Dokumente erfasst, bei denen die Checkbox komplett buchen markiert ist.
- **Bestell-Nr.:**
  Nummer der Bestellung.
- **Komplett buchen:**
  Eine Bestellung kann als komplett gebucht werden, wenn alle Positionen vollständig geliefert wurden.
  - Der Wareneingang ist nicht vollständig. Es stehen noch Lieferungen aus.
  - Der Wareneingang ist vollständig und die Bestellung soll als komplett verbucht werden.
- **Status:**
  Aktueller Status. Der Status wird nach der Erfassung des Wareneingangs umgesetzt.
- **Lieferant:**
  Nummer und Name des Lieferanten.
- **Anlief.-Term. d. Lieferant:**
  Anliefertermin des Lieferanten. Der Termin wird aus der Bestellung oder der AB übernommen. Wenn Sie den Wareneingang erfasst haben, wird der Termin auf das aktuelle Tagesdatum oder das von Ihnen gewählte Datum umgesetzt.
- **Enthält Kisten:**
  Anzeige der Bestellungen, in denen Kisten enthalten sind. Die Markierung der Checkbox kann nicht geändert werden.

**Zugehörige Aufträge**

In der Übersicht werden nur die referenzierten Aufträge angezeigt, die zu der ausgewählten Bestellung gehören. Wenn mehrere Bestellungen ausgewählt sind, bleibt die Liste leer.

**Anliefertermin bei Kunde** Das Datum wird aus dem referenzierten Auftrag übernommen. Sie können es überschreiben, wenn der ursprüngliche Termin nicht eingehalten werden kann.

### Wareneingang – Positionsweise

*Dokumente > Bestellung > Wareneingang > Wareneingang Kiste > Register Positionsweise*

*Abb. K-62: Wareneingang - Positionsweise*

In diesem Register können Sie Wareneingänge positionsweise für eine Bestellung erfassen, die im Register Komplett ausgewählt wurde.

**Warenein-/ausgang**

**Menge Eingang** Menge, die für die markierte Position geliefert wurde.

**Menge bestellt, Bereits geliefert, Menge avisiert** In diesen Feldern werden die entsprechenden Mengen für die markierte Position angezeigt. Die Felder werden nach der Erfassung aktualisiert.

**Lagerort** Zur markierten Position können Sie einen Lagerort auswählen, an dem der Lagerartikel verbucht werden soll. Beachten Sie dabei, dass Lagerartikel auch auf den Lagerort `<k.A.>` gebucht werden können. Der Lagerort aus der Bestellung kann über das Menü Optionen vorgeblendet werden.

**Über-/Unterlieferung akzeptieren** Die Stückzahl der Lieferung kann sich von der Bestellung unterscheiden. Sie können die abweichenden Stückzahlen akzeptieren und damit die Lieferung für die Position als komplett erfassen.
- Über- oder Untermengen werden nicht akzeptiert.
- Die eingegebene Stückzahl wird akzeptiert und die Position wird als komplett gebucht. Wenn ein Lagerartikel geliefert wurde, wird der Lagerbestand der gelieferten Menge entsprechend aktualisiert. Die geänderte Menge wird in die Bestellung zurückgeschrieben.

**Bestätigung**

**AB-Lieferant** Nummer der Auftragsbestätigung des Lieferanten für die markierte Position.

**AB-Liefertermin** Liefertermin für die Position.

**Positionen**

In der Übersicht werden die Positionen der gewählten Bestellung angezeigt.
- **Pos:**
  Nummer der Bestellposition.
- **Komplett buchen:**
  Eine Position kann als komplett gebucht werden, wenn die gesamte Stückzahl geliefert wurde.
  - Der Wareneingang ist nicht vollständig.
  - Die Position soll als komplett verbucht werden.
- **Auftr.Nr.:**
  Auftragsnummer.
- **Artikel:**
  Bezeichnung des bestellten Produkts.
- **Farbe:**
  (Farb-) Varianten, die zu dem bestellten Produkt erfasst sind.
- **Breite/Höhe:**
  Maße der bestellten Position.
- **Bestellt:**
  Stückzahl der Bestellung für diese Position.
- **Avisiert:**
  Avisierte Stückzahl der Position.
- **Geliefert:**
  Menge, die für diese Position bereits geliefert wurde. Bei Teillieferungen ist dies die Summe der Stückzahlen, die bisher zu dieser Bestellung geliefert wurden.
- **Eingang:**
  Menge, die für die markierte Position geliefert wurde.
- **Akzeptieren:**
  Wenn die Stückzahl der Lieferung höher oder niedriger ist als die der Bestellung, kann diese Stückzahl übernommen werden. Die nicht bestellten Scheiben werden im Lager nur verbucht, wenn es Lagerartikel sind, die in einer Lagerbestellung bestellt wurden. Wenn die Bestellung aus einem Auftrag erzeugt worden ist, werden die Lagerbestände nicht aktualisiert.
  - Die Liefermenge entspricht der Bestellung und braucht nicht gesondert gekennzeichnet zu werden.
  - Die Lieferung ist größer oder kleiner als die Bestellung und wird akzeptiert. Die gelieferte Stückzahl wird in die Bestellung zurückgeschrieben. Der referenzierte Auftrag wird nicht geändert. Die überzähligen Scheiben können ggf. als Bestand verbucht werden.
- **Enthält Kisten:**
  Anzeige der Bestellungen, in denen Kisten enthalten sind. Die Markierung der Checkbox kann nicht geändert werden.
- **AB-Lieferant:**
  Nummer der Auftragsbestätigung des Lieferanten.
- **AB-Liefertermin:**
  Liefertermin aus der Auftragsbestätigung des Lieferanten.
- **Lagerort:**
  Standard-Lagerort des Lagerartikels. Beachten Sie dabei, dass Lagerartikel auch auf den Lagerort `<k.A.>` gebucht werden können.
- **Artikelbezeichnung 2 + 3:**
  Bezeichnungen des bestellten Produkts, die in den Stammdaten hinterlegt sind. Bei Float-Glas ist in der Regel nur die Bezeichnung 1 hinterlegt, die in der Spalte Artikel angezeigt wird.

**Zugehörige Aufträge**

In der Übersicht werden die referenzierten Aufträge zu den Positionen angezeigt. Die Felder sind zum Register Komplett beschrieben.
*⇨ "Wareneingang - Komplett" auf Seite K-3412*

### Wareneingang - Identnummer

*Dokumente > Bestellung > Wareneingang > Wareneingang > Register Identnummer*

*Abb. K-63: Wareneingang - Identnummer*

In diesem Register werden die Positionen einer Bestellung mit Kisten angezeigt. Dabei wird für jede Kiste einer Bestellposition eine Unterposition (virtuelle Positionsnummer) erzeugt, der eine Kiste mit einer eigenen Identnummer (Identifikationsnummer, ID) zugewiesen werden kann. Die Vorgabe für die ID können Sie festlegen.
*⇨ "Einstellungen (ID)" auf Seite K-3420*

> **Voraussetzung**
> In den Firmendaten muss die Checkbox für die Vergabe von virtuellen Positionsnummern markiert sein.
> *⇨ Stammdaten, "Fälligkeitsberechnung für Februar (28 oder 29 Tage)" auf Seite B-1080*

**Kistendaten**

**Lieferanten-Identnummer** Die Kisten-ID, die der Lieferant für diese Position der Lieferung vergeben hat. Wenn die Nummer eingegeben ist, wird im Feld *Identnummer* die automatische Kisten-ID angezeigt.

**Identnummer** Die automatische Kisten-ID wird angezeigt, sobald Sie die Lieferanten-ID eingetragen haben. Für jede Kiste einer Bestellposition wird beim Erfassen des Wareneingangs eine eigene Kisten-ID erzeugt. Wenn z. B. 5 Kisten mit Float 5 à 1200 x 800 mm bestellt und geliefert wurden, werden die IDs XXXX00001, XXXX00002, ..., XXXX00005 vergeben. Die Vorgabe für XXXX können Sie selbst bestimmen.
*⇨ "Einstellungen (ID)" auf Seite K-3420*

**Lagerort** Sie können jeder Position einen eigenen Lagerort zuweisen. Beachten Sie dabei, dass Sie auch den Lagerort `<k.A.>` zuweisen können.

**Bemerkung** Bei Besonderheiten, z. B. in der Zuweisung des Lagerortes oder bei Reservierungen, können Sie eine Anmerkung eintragen.

**Inhalt** Inhalt der Kiste, die in der Übersicht markiert ist. Der Wert kann ggf. geändert werden.

**Prod. Datum** Datum, bis zu dem die Produktion mit der bestellten Lieferung abgeschlossen sein sollte. Dieses Datum ist für die Lagerentnahme nach dem FiFo-Prinzip wichtig, z. B. für beschichtetes Glas.

**EK/ME** Einkaufspreis und Preiseinheit der bestellten Position. Wenn Sie den Preis ändern, wird die Änderung in die Bestellung zurückgeschrieben.

**Kistenpositionen**
- **Pos:**
  Positionsnummer aus der Bestellung. Eine Positionsunternummer wird beim Buchen automatisch dann vergeben, wenn die Stückzahl der Bestellposition größer als 1 ist, z. B. 1.1, 1.2 usw.
- **Bezeichnung:**
  Bezeichnung aus der Bestellung.
- **Breite / Höhe:**
  Lagermaße der Scheiben in der Kiste.
- **Lieferanten-Identnummer:**
  Kisten-ID des Lieferanten wie im Bereich Kistendaten eingetragen.
- **Inhalt:**
  Kisteninhalten wie im Bereich Kistendaten eingetragen.
- **Identnummer:**
  (Automatische) ID wie im Bereich Kistendaten eingetragen.
- **Lagerort:**
  Lagerort wie im Bereich Kistendaten eingetragen.
- **Prod. Datum:**
  Produktionsdatum wie im Bereich Kistendaten eingetragen.
- **Pr./ME:**
  EK-Preis pro Mengeneinheit wie im Bereich Kistendaten eingetragen.
- **Pr. Einh.:**
  Preiseinheit für den angezeigten Preis.

### Wareneingang – Protokoll (Identnummern)

*Dokumente > Bestellung > Wareneingang > Wareneingang > Register Protokoll (Identnummern)*

*Abb. K-64: Wareneingang – Protokoll (Identnummern)*

In diesem Register können Sie sich einen Überblick über die vergebenen Kisten-IDs verschaffen.

### Einstellungen (ID)

*Dokumente > Bestellung > Wareneingang > Wareneingang > Menü Optionen > Gruppe Identnummernvergabe > Einstellungen*

*Abb. K-65: Einstellungen*

In diesem Dialog legen Sie die Vorgabe für die Identifikationsnummern (ID) für Kisten fest. Diese Einstellung ist notwendig, um eigene Kisten-IDs automatisch zu vergeben.

Wenn in einer Lieferung z. B. eine Position mit 5 Kisten aufgeführt ist, werden beim Erfassen des Wareneingangs 5 (virtuelle) Unternummern vergeben. Diese Nummern müssen Sie mit einem Kennzeichen versehen, so dass z. B. statt der gescannten Kistennummer 12345 die Unternummern LieferantA00001, LieferantA00002, ..., LieferantA00005 vergeben werden.
*⇨ Tutorial, "Kistengeschäft" auf Seite D-2170*

> **Voraussetzung**
> In den Firmendaten muss die Checkbox für die virtuelle Vergabe von Positionsnummern markiert sein.
> *⇨ Stammdaten, "Fälligkeitsberechnung für Februar (28 oder 29 Tage)" auf Seite B-1080*

**Lageridentnummer**

**Vorgabe** Sie können einen Text (oder Zahlen) mit max. 15 Zeichen eingeben, der durch XXXXX ergänzt wird. XXXXX steht für die automatisch vergebene Nummer. Der Text wird so lange beibehalten, bis Sie ihn ändern.
Wenn Sie von unterschiedlichen Lieferanten Kisten beziehen und diese getrennt kennzeichnen möchten, müssen Sie vor dem Erfassen des Wareneingangs die Vorgabe jeweils entsprechend anpassen.

### Warenausgang Kisten

*Fertigung > Lieferwesen > Warenausgang Kisten > Register Identnummern*

*Abb. K-66: Warenausgang von Kisten – Kiste ausbuchen*

In diesem Register können Sie eine Kiste reservieren oder aus dem Lagerbestand ausbuchen. Sie können nur Kisten reservieren, die beim Lagereingang mit einer Kisten-ID erfasst wurden.
*⇨Tutorial, "Warenausgang Kisten" auf Seite E-2443*

---

## A+W Business Barcode Manager (EL)

**Revisionsübersicht des Moduls:**
*03-2023: Ersterstellung, Überführung aus docx-Dokument*

Zu diesem Modul finden Sie folgende Kapitel:
*⇨ Tutorial*

---

## Tutorial

### In diesem Kapitel finden Sie folgende Themen:
*⇨ Einleitung*
*⇨ Einstellungen*
*⇨ Funktionen*
*⇨ Barcodes*

- Einleitung Y-3427
- Einstellungen Y-3428
  - Scanner Y-3428
  - Erfassungsstellen in A+W Business Y-3430
  - Mitarbeiterverwaltung in A+W Business Y-3431
  - Interface Service Y-3431
  - Kapazitätsplanung Y-3432
- Funktionen Y-3433
  - Anmeldung Y-3433
  - Hauptmenü Y-3434
  - Wareneingang Y-3435
  - Produktionsmeldung Y-3436
    - Fertigmeldung Y-3437
    - Bruchmeldung Y-3438
  - Lagerbewegungen Y-3439
    - Lagerentnahme Y-3440
    - Lagerzugang Y-3441
    - Umbuchung Y-3442
    - Kisten Y-3444
  - Gestelle Y-3450
    - Übersicht über Gestellmenü Y-3450
    - Gestelle beladen Y-3451
    - Gestelle leeren Y-3453
    - Gestelle anzeigen Y-3454
  - Sonstiges Y-3455
    - Auftragsinformation Y-3455
    - Anmeldeinformation Y-3456
    - Mitarbeiterwechsel Y-3456
- Barcodes Y-3457
  - Ausdrucken von Barcodes Y-3458
  - Buchungshistorie Y-3459

### Einleitung

Die Online - Betriebsdatenerfassung mittels Barcode-Scanner erfolgt mittels eines Windows-CE basierten Scanner der Firma Datalogic (Scorpio). Das eigentliche Programm läuft dabei auf einem Terminal-Server, an den sich der Scanner via Remote-Desktop verbindet. Alle Lesungen die am Scanner vorgenommen werden, sendet der Scanner als Tastatureingabe in das jeweils aktive Datenfeld.

Damit das Programm für die BDE nach der Anmeldung des Scanners am Terminal-Server automatisch startet, ist es erforderlich eine Verknüpfung zum BDE-Programm für den Benutzer in die Autostart-Gruppe zu kopieren. Das zu verknüpfende Programm hat den Namen abcscanner.exe und befindet sich im A+W Business Programme Ordner (z.B. C:\\Program Files\\A+W\\ALFAK 2011\\Program\\German). Bevor das Programm gestartet wird muss auf dem Rechner das A+W Business Startprogramm einmalig ausgeführt werden und es muss die richtige Datenbankverbindung im Login-Dialog eingegeben werden. Das BDE-Programm verbindet sich ab diesem Moment immer mit den gerade eingegebenen Informationen an die Datenbank.

Das automatische Starten des Programmes kann ab A+W Business 5.5 Update 3 durch ein Konfigurationsprogramm (A+W Business 5 Scanner AutoStart Config) im Startmenu Config Tools eingestellt werden. In diesem Programm kann für den aktuelle angemeldeten Benutzer das Scannerprogramm (sprachabhängig) ausgewählt werden, das beim Anmelden dieses Benutzers gestartet werden soll.

### Einstellungen

#### Scanner

Die Konfiguration des Scanners kann auf einem beliebigen Arbeitsplatz durchgeführt werden. Zuerst wird die dem Scanner beiliegende Konfigurations-Software auf einem PC installiert und anschließend wird der Scanner per USB verbunden. Dann wird die Konfigurations-Software gestartet (Datalogic Configuration Utility). In dem Programm wird zunächst die Einstellung Postamble im Menü *Hw Configuration > Laser > Parameters > Reader Parameters > Text Formatting* vorgenommen. Hier wird einfach ein Tabulator eingegeben. Die Eingabe des Tabulators kann auf zwei Arten erfolgen. Entweder man gibt ein Tabulator in einem Editor (z.B. Notepad oder Word) ein und kopiert diesen über die Zwischenablage in das Datenfeld. Oder man drückt die Taste ALT, hält sie gedrückt währen man auf dem Nummernblock die Ziffern 0 0 9 nacheinander eingibt und die ALT Taste wieder los lässt.

Dadurch wird am Ende einer jeden Lesung ein [TAB] an das BDE-Programm gesendet um eine vollständige Lesung des Barcodes zu signalisieren.

*Abb. Y-67: Vollständigkeit der Barcode- Lesung*

Die zweite und letzte Einstellung lautet CheckEvaluation im Menü *Hw Configuration > Laser > Parameters > Reader Parameters > Code39 > Standard*. Diese Einstellung muss auf Enabled gesetzt werden, damit die Prüfziffern des Code39 Barcodes überprüft und nicht als gültige Daten an das Programm gesendet werden.

*Abb. Y-68: Code 39 Einstellung*

Die zweite und letzte Einstellung lautet CheckEvaluation im Menü *Hw Configuration > Laser > Parameters > Reader Parameters > Code39 > Standard*. Diese Einstellung muss auf Enabled gesetzt werden, damit die Prüfziffern des Code39 Barcodes überprüft und nicht als gültige Daten an das Programm gesendet werden).

#### Erfassungsstellen in A+W Business

*Fertigung > Erfassungsstellen Produktion*

*Abb. Y-69: Erfassungsstellen Produktion*

In diesem Dialog hinterlegen Sie BDE-Typ der jeweilige Typ der Erfassungsstelle. Diese werden für den Wareneingang und die Fertigmeldung benötigt. Ist beispielsweise eine eindeutige Zuordnung von Erfassungsstelle zu BDETyp gemacht (in der obigen Abbildung z.B. für den Wareneingang) so ist es nicht mehr nötig die Erfassungsstelle am Scanner einzulesen, wenn man den entsprechenden Programmpunkt wählt.

#### Mitarbeiterverwaltung in A+W Business

*Abb. Y-70: Mitarbeiterverwaltung - Einstellung*

In der Mitarbeiterverwaltung ist es erforderlich für diejenigen Mitarbeiter die Personalnummer einzugeben, die sich per Mitarbeiter-Barcode an dem Scanner anmelden sollen.

#### Interface Service

Um Fertigmeldungen per Scanner zu buchen, werden die gelesenen Fertigmeldungen in der Datenbank gepuffert und anschließend vom AIS verarbeitet. Damit der AIS die gelesenen Buchungen zuordnen kann, ist es wichtig den Instanz-Namen des AIS als „sysadm" zu definieren.

Das ist auch der Default nach der Installation. Wenn bei einer Installation mehr als eine Instanz des AIS zum Einsatz kommt ist es wichtig diese Einstellung zu prüfen.

#### Kapazitätsplanung

*Kapazitätsplanung > Stammdaten > Organisation > Aggregate*

*Abb. Y-71: Aggregat-Zuordnung für Erfassungsstelle*

Soll die Verbuchung der Fertigmeldungen mit der A+W Business Kapazitätsplanung erfolgen, so ist es nötig für das jeweilige Aggregat eine eindeutige Erfassungsstelle einzutragen. Das geschieht in der Aggregat-Verwaltung unter *Kapazitätsplanung > Stammdaten > Organisation > Aggregate*. Die jeweils zu verwendende Arbeitsart wird dabei immer über den Barcode eingelesen.

### Funktionen

Im Folgenden sind die einzelnen Dialoge der BDE aufgeführt und deren Funktionsweise erläutert:
*⇨ "Anmeldung" auf Seite Y-3433*
*⇨ "Hauptmenü" auf Seite Y-3434*
*⇨ "Wareneingang" auf Seite Y-3435*
*⇨ "Produktionsmeldung" auf Seite Y-3436*
*⇨ "Lagerbewegungen" auf Seite Y-3439*
*⇨ "Gestelle" auf Seite Y-3450*
*⇨ "Sonstiges" auf Seite Y-3455*

#### Anmeldung

**Scanner-Start**

*Abb. Y-72: BDE - Anmeldung über Personalbarcode39 Einstellung*

Nach erfolgreicher Anmeldung eines Anwenders gelangt man direkt in das Hauptmenü. Von hier aus gelangt man in den jeweiligen Dialog um Wareneingänge, Lagerbuchungen, Gestell-Belegungen oder Fertigmeldungen durchzuführen.
*⇨ "Hauptmenü" auf Seite Y-3434*

#### Hauptmenü

*Scanner > Hauptmenü*

*Abb. Y-73: BDE - Hauptmenü*

Über die Hauptmenü des Scanners erreichen Sie folgende Funktionen:
*⇨ "Wareneingang" auf Seite Y-3435*
*⇨ "Produktionsmeldung" auf Seite Y-3436*
*⇨ "Lagerbewegungen" auf Seite Y-3439*
*⇨ "Gestelle" auf Seite Y-3450*
*⇨ "Sonstiges" auf Seite Y-3455*
Mit der Option [Back/ Zurück] kehren Sie zu vorherigem Dialog.

#### Wareneingang

*Scanner > Hauptmenü > Wareneingang*

*Abb. Y-74: BDE - Wareneingang*

Hier werden die Barcodes der Bestellpositionen eingelesen, für die ein Wareneingang verbucht werden soll:

Nachdem der Barcode mit der Bestellposition gelesen wurde wird die Eingangsmeng per Tastatur eingegeben. Standardmäßig zeigt das Programm hier die komplette Menge der Bestellposition an und muss nur bei einer abweichenden Menge geändert werden. Sollte keine Änderung nötig sein, wird mit dem Barcode der nächsten Bestellposition fortgefahren. Das Programm sammelt diese Lesungen zunächst ohne eine tatsächliche Buchung durchzuführen. Das passiert erst, wenn man auf dem Scanner die ENTER-Taste getätigt, oder den Barcode einer anderen Bestellung einliest. Wird der ZURÜCK-Button oder die ESC-Taste betätigt und es sind noch nicht verbuchte Bestellpositionen im Speicher, so fragt das Programm nach, ob diese jetzt verbucht werden sollen.

Wenn es sich bei der gerade eingelesenen Bestellposition um eine Kiste handelt, so kann direkt danach ein Kisten-Identnummern-Barcode eingelesen werden und ggf. der Inhalt der Kiste geändert werden. Es wird dann automatisch nur eine Menge von 1 Stück eingetragen und diese ist auch nicht mehr änderbar. Für Kisten mit Identnummern kann ein abweichender Inhalt eingegeben werden.

Nach jeder Lesung einer Bestellposition wird in dem unteren Mengen-Feld angezeigt wie viel Artikel bestellt wurden und wie viele bereits geliefert wurden.

#### Produktionsmeldung

*Scanner > Hauptmenü > Produktionsmeldung*

*Abb. Y-75: BDE - Produktionsmeldung*

Die Fertig- und Bruchmeldungen befinden sich im Untermenü Produktionsmeldung, welches im Hauptmenü des Scanners die bisherige Fertigmeldung ersetzt.
*⇨ "Fertigmeldung" auf Seite Y-3437*
*⇨ "Bruchmeldung" auf Seite Y-3438*

#### Fertigmeldung

*Scanner > Hauptmenü > Produktionsmeldung > Fertigmeldung Report*

*Abb. Y-76: BDE - Produktions-Rückmeldung*

Über den Dialog der Fertigmeldung lassen sich Statusänderungen an Auftragspositionen durchführen. Alle Lesungen die hier durchgeführt werden, werden zunächst in der Datenbank gespeichert und durch den AIS als STSD-Rückmeldung verarbeitet. Statusänderungen an den Aufträgen werden daher Zeit versetzt ausgeführt. Näheres zur Konfiguration des AIS für STSD-Rückmeldungen sind dem vorherigen Kapitel zu entnehmen.

Nachdem eine Auftragsposition gelesen wurde, wird die Menge eingetragen, die fertig gemeldet werden soll. Das Programm blendet hier immer die komplette Positionsmenge vor. Zum Speichern der Fertigmeldung ist die ENTER-Taste zu drücken. Der Datensatz wird danach vom AIS verarbeitet und der Status des Auftrages ggf. angepasst. Soll pro Scannung nur ein Stück verarbeitet werden, kann die Option „Menge=1" gewählt werden. Ist diese Option aktiviert, wird beim Scannen eines Barcodes sofort 1 Stück als fertig eingetragen. Eine zusätzliche Eingabeder Menge oder ein Bestätigen mit Enter ist damit nicht mehr nötig.

Über den Dialog Bruchmeldung lassen sich ebenfalls Statusänderungen an Aufträgen durchführen, im Gegensatz zur Fertigmeldung allerdings nur negative.

#### Bruchmeldung

*Scanner > Hauptmenü > Produktionsmeldung > Bruchmeldung - Report*

*Abb. Y-77: BDE - Bruchmeldung*

Bedienung und Verbuchung funktionieren analog zur Fertigmeldung, allerdings ist es möglich, Bruchgrund und -erfasser mit anzugeben. Diese können entweder per Druck auf die Schaltfläche auf dem Scanner oder per Barcode ausgewählt werden. Die Barcodes können in den Programmen Reklamationsgrund und -verursacher über das Formular Etiketten ausgedruckt werden.

Nach der Buchung eines Satzes werden die Informatonen zur letzten Buchung zusammengefasst auf dem Scanner angezeigt.

#### Lagerbewegungen

*Scanner > Hauptmenü > Lagerbewegung*

*Abb. Y-78: BDE - Menü Lagerbewegung*

Beim Start der Lagerbuchung wird zuerst gewählt, ob ein Zugang oder ein Abgang von Ware erfolgen soll. Zusätzlich ist das Menü für Kisten von hier erreichbar.
*⇨ "Lagerentnahme" auf Seite Y-3440*
*⇨ "Lagerzugang" auf Seite Y-3441*
*⇨ "Umbuchung" auf Seite Y-3442*
*⇨"Kisten" auf Seite Y-3444*

#### Lagerentnahme

*Scanner > Hauptmenü > Lagerbewegung > Entnahme*

*Abb. Y-79: BDE - Lagerentnahme*

Der darauf folgende Dialog funktioniert für den Zugang und Abgang größten Teils identisch. Nachdem der Lagerortbarcode gelesen worden ist, kann der Lagerartikelbarcode gelesen werden und die jeweilige Menge für die Zugangs- bzw. Abgangsbuchung eingegeben werden. Durch Betätigung der ENTER-Taste wird die Buchung direkt ausgeführt.

#### Lagerzugang

*Scanner > Hauptmenü > Lagerbewegung > Zugang*

*Abb. Y-80: BDE - Lagerzugang*

#### Umbuchung

*Scanner > Hauptmenü > Lagerbewegung > Umbuchung*

*Abb. Y-81: BDE - Lagerort wählen*

Es gibt nun unter dem Menüpunkt Lagerbewegung die Funktion Umbuchung. Wählt man diesen muss man zunächst einmal einen Lagerort – Barcode scannen.

Danach gelangt man in den Dialog zur Umbuchung von Lagerartikeln. Hier muss der Anwender ein Lagerartikel scannen, also eine LagerID eines Lagerartikels, woraufhin der aktuelle Bestand angezeigt wird. Nun sollte man zunächst die Menge, die umgebucht werden soll, definieren.

*Abb. Y-82: BDE - Umbuchung Lagerartikel*

Dann kann der Anwender einen neuen Lagerort vorgeben und die Buchung ausführen. Auf dem Schirm erscheint eine Erfolgsmeldung:

*Abb. Y-83: BDE - erfolgreiche Umbuchung*

#### Kisten

*Scanner > Hauptmenü > Lagerbewegung > Kisten*

*Abb. Y-84: BDE - Kistenlager Menü*

Ab der A+W Business Version 12.5 steht zusätzlich noch das Untermenü Kisten zur Verfügung. Mit diesem Menü können die folgenden Funktionen aufgerufen werden:
- "Kisteninhalt ändern" auf Seite Y-3445
- "Auflösen von Kisten" auf Seite Y-3446
- "Lagerort von Kisten ändern" auf Seite Y-3447
- "Kiste auf Inventur setzen" auf Seite Y-3448
- "Warenausgang Kiste" auf Seite Y-3449

#### Kisteninhalt ändern

*Scanner > Hauptmenü > Lagerbewegung > Kisten > Inhalt ändern*

*Abb. Y-85: BDE - Kisteninhalt ändern*

Mit dieser Funktion kann die Blattanzahl in einer Kiste reduziert werden. Dazu wird erst ein Kistenbarcode gescannt und danach die angezeigte Menge auf den neuen Wert gesetzt. Durch Bestätigen der Enter Taste wird die Buchung ausgelöst.

#### Auflösen von Kisten

*Scanner > Hauptmenü > Lagerbewegung > Kisten > Auflösen*

*Abb. Y-86: BDE - Kistenlager Menü*

Mit dieser Funktion kann eine Kiste aufgelöst werden (d.h. die Kiste wird gelöscht und die verbleibenden Scheiben werden auf das Lager gebucht). Hierzu wird erst eine Kiste gescannt und danach kann der Inhalt noch editiert werden. Durch Bestätigen der Enter Taste wird die Buchung ausgelöst.

#### Lagerort von Kisten ändern

*Scanner > Hauptmenü > Lagerbewegung > Kisten > Lagerort ändern*

*Abb. Y-87: BDE - Kistenlager Menü*

Mit dieser Funktion kann der Lagerort einer Kiste verändert werden. Dazu wird erst eine Kiste gescannt und danach der Barcode des neuen Lagerortes. Die Buchung wird dann sofort ausgelöst.

#### Kiste auf Inventur setzen

*Scanner > Hauptmenü > Lagerbewegung > Kisten > Zu Inventur Liste*

*Abb. Y-88: BDE - Kisten auf Inventur setzen*

Mit dieser Funktion wird eine Kiste auf die aktuelle Inventurliste gesetzt. Nachdem die Kiste gescannt wurde kann der neue Lagerort gescannt werden. Nachdem beide Scannungen durchgeführt wurden, kann die aktuelle Menge der Scheiben in der Kiste noch editiert werden. Durch Bestätigen der Enter Taste wird die Buchung ausgelöst.

#### Warenausgang Kiste

*Scanner > Hauptmenü > Lagerbewegung > Kisten > Warenausgang Kiste*

*Abb. Y-89: BDE - Kisten Warenausgang*

Mit dieser Funktion können Kisten mit Identnummer einer Auftragsposition zugeordnet werden. Zunächst muss ein Auftragspositions-Barcode gescannt werden. Danach wird per Scannen des Kisten-Barcodes die Blattanzahl der Kiste ermittelt. Dieser kann dementsprechend editiert werden. Durch Bestätigen der Enter Taste wird die Buchung ausgelöst.

### Gestelle

Damit Gestelle verarbeitet werden können, müssen die folgenden Bedingungen vorher geprüft werden:
- Gestellnummern müssen eindeutig sein. Es darf also nicht ein Gestell mit der gleichen Nummer aber unterschiedlicher Gestellart angelegt werden. Wenn die gleiche Nummer verwendet wird, sollte der Gestellnummer ein Buchstabe (Für die Gestellart) vorangestellt werden.
- Beim Verbuchen von Gestellen wird die Breite und Höhe des Gestells und das Beladungsgewicht geprüft. Diese Werte können pro Gestellart eingestellt werden.
- Die Verbuchung von Gestellen ist für den Versand entwickelt worden, d.h. es können nur Hauptpositionen einem Gestell hinzugefügt werden.
- Es können nur Gestelle beladen werden, die nicht außer Haus gebucht sind, nicht als verloren gemeldet und nicht gesperrt sind.
- Mit Punkt 5 ist sichergestellt, das beim Gestellausgang die Zuordnung des Gestells vollständig gebucht sein sollte.

#### Übersicht über Gestellmenü

*Scanner > Hauptmenü > Gestelle*

*Abb. Y-90: BDE - Menü Gestelle*

Im Untermenü Gestelle sind folgende Funktionen verfügbar:
- "Gestelle beladen" auf Seite Y-3451
- "Gestelle leeren" auf Seite Y-3453
- "Gestelle anzeigen" auf Seite Y-3454

#### Gestelle beladen

*Scanner > Hauptmenü > Gestelle > Beladen*

*Abb. Y-91: BDE - Gestelle Beladen*

Zum Beladen von Gestellen muss zuerst das Gestell ausgewählt werden, das beladen werden soll. Ab dem Scannen des Gestellbarcode, können dann im darauf folgenden Dialog Auftragspositionen dem Gestell hinzugefügt werden.

*Abb. Y-92: BDE - Gestelle Beladen - Auftragspositionen*

Nach der erfolgreichen Auswahl eines Gestells kann man Auftragspositionen dem Gestell hinzufügen. Hierbei werden zwei unterschiedliche Modi unterstützt, die mit den Knöpfen „Menge = 1“ und „Eingabe Menge" ausgewählt werden können. Der aktuell eingestellte Modus ist grün markiert.

Für das Hinzufügen von Auftragspositionen muss der T2 Barcode verwendet werden.

Im Modus „Eingabe Menge" wird nach dem der Positionsbarcode gescannt wurde, die noch nicht auf Gestellen abgestellte Menge im Mengenfeld des Dialoges angezeigt. Diese kann dann editiert werden, wenn eine kleinere Anzahl abgestellt werden soll. Durch ein Drücken der Enter Taste auf dem Scanner wird die Buchung gestätigt.

Im Modus „Menge = 1" wird die Verbuchung sofort nach dem Scannen des Auftragspositionsbarcodes ausgeführt. Hierbei wird immer nur 1 Stück verbucht.

Das Ergebnis der letzten Buchung wird immer im Fenster „Letzte Buchung" angezeigt.

Um das Gestell zu wechseln, kann der Zurück Knopf getätigt werden und dann ein anderes Gestell ausgewählt werden.

#### Gestelle leeren

*Scanner > Hauptmenü > Gestelle > Leeren*

*Abb. Y-93: BDE - Gestelle Leeren*

Mit diesem Dialog kann ein Gestell als leer gemeldet werden. Dabei werden alle Zuordnungen der vorher auf dem Gestell abgestellten Auftragspositionen gelöscht.

> **Keine Sicherungsabfrage**
> Beim Leeren eines Gestells erfolgt keine Bestätigungsabfrage!

#### Gestelle anzeigen

*Scanner > Hauptmenü > Gestelle > Anzeigen*

*Abb. Y-94: BDE - Gestelle anzeigen*

Mit diesem Dialog kann die aktuelle Zuordnung von Auftragspositionen auf einem Gestell angezeigt werden. Wird ein Gestellbarcode gescannt, werden im Belegungsfenster die Auftragspositionen mit der jeweils abgestellten Menge angezeigt. Zusätzlich wird noch die Kundennummer mit ausgegeben. Die Liste enthält jeweils sechs Einträge. Mit dem Vor und Zurück Knopf kann diese geblättert werden.

### Sonstiges

*Scanner > Hauptmenü > Sonstiges*

Über den Menüpunkt Sonstiges erreicht man die Dialoge für die Auftragspositionsinfo, die Anmeldeinfo und den Dialog zum Wechseln des Mitarbeiters:
*⇨ "Auftragsinformation" auf Seite Y-3455*
*⇨ "Anmeldeinformation" auf Seite Y-3456*
*⇨ "Mitarbeiterwechsel" auf Seite Y-3456*

#### Auftragsinformation

*Scanner > Hauptmenü > Sonstiges > Auftragsinformation*

*Abb. Y-95: BDE - Auftragsinformation*

Die Auftragspositionsinfo zeigt nach der Lesung eines Auftragspositions-Barcodes die Bezeichnung der Position, deren Abmessung, die Stückzahl, die gelieferte Menge den Preis pro Preiseinheit und das Lieferdatum an.

#### Anmeldeinformation

*Scanner > Hauptmenü > Sonstiges > Anmeldeinformation*

*Abb. Y-96: BDE - Sonstiges*

Der Dialog für die Anmeldeinformationen zeigt den aktuell angemeldeten Benutzer, die Datenbank, das Datenbanksystem (Microsoft SQL Server oder Unify SQL Base), die Erfassungsstelle, das Aggregat und die Arbeitsart an.

#### Mitarbeiterwechsel

*Scanner > Hauptmenü > Sonstiges > Mitarbeiterwechsel*

*Abb. Y-97: BDE - Anmelden*

Der Dialog zum Mitarbeiterwechsel ist in folgenden Abschnitt beschrieben:
*⇨ "Anmeldung" auf Seite Y-3433*
Nach der Lesung eines gültigen Mitarbeiterbarcodes wird der aktuelle Mitarbeiter abgemeldet und der neue Mitarbeiter angemeldet.

### Barcodes

Für die einzelnen Dialoge und Funktionen sind bestimmte Barcodes erforderlich. Bei den Barcodes handelt es sich um Code39 Barcodes mit Prüfziffer und einem Stern als Anfangs- und Ende-Zeichen.

| Bezeichnung | Präfix | Nutzdaten | Beispiel |
| :--- | :--- | :--- | :--- |
| Personalbarcode | PE | Die Personalnummer aus der Mitarbeiterverwaltung | *PE000000199F* |
| Erfassungsstellenbarcode ohne Arbeitsart für Wareneingang | ES | Die ID der Erfassungsstelle | *ES00000000166* |
| Erfassungsstellenbarcode mit Arbeitsart für Fertigmeldung | EA | :Die ID der Erfassungsstelle und die ID der Arbeitsart getrennt mit Bindestrich | *EA0000000015-101P* |
| Auftragsbarcode für Fertigmeldung und Scheiben-Gestell-Zuordnung | T2 | Auftragsnummer + Positionsnummer (3stellig) + Teilenummer (3stellig) | *T200000243001001%* |
| Auftragsbarcode für Auftragsinfo | D2 oder T2 | Auftragsnummer + Positionsnummer (3stellig) + Teilenummer (3stellig) (Nur T2) | *D200000243002Q* oder *T200000243002001Q* |
| Bestellbarcode für Wareneingang | D5 | Bestellnummer + Positionsnummer (3stellig) | *D50000070650001.* |
| Kistenbarcode für Lagerabgang und Wareneingang | BO | Identnummer einer Kiste. Achtung Identnummer darf keine führende Null enthalten! | *BOBC00002H* |
| Lagerortbarcode für Lagerbuchung | LA | Die ID des Lagerortes | *LA0000000001W* oder *L0000000001W* |
| Lagerartikel Barcode für Lagerbuchung | LP | Die LagerID des Lagerartikels | *LP0000000164E* |
| Gestellnummer | GE | Die Gestellnummer | *GE9099E* |
| Reklamationsgrund | BR | Die Nummer des Reklamationsgrundes | *BR1$* |
| Reklamationsverursacher | BC | Die Nummer des Reklamationsverursachers | *BC2P* |

#### Ausdrucken von Barcodes

In den folgenden Programmen im A+W Business wurde eine Barcode-Druckfunktionalität für die Online - Betriebsdatenerfassung (mittels Barcode-Scanner) implementiert:
- Mitarbeiterverwaltung (Stammdaten > Firma > Mitarbeiter)
- Erfassungsstellen Produktion (z.B. Stammdaten > Fertigung > Sonstige > Erfassungsstellen Produktion)
- Vorgabezeiten (Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten)
- Druckprogramm (z.B. Dokumente > Auftrag > Druck Auftrag)
- Lagerdefinition (Stammdaten > Lager > Lagerdefinition)
- Lagerverwaltung (Lagerwirtschaft > Lagerverwaltung)
- Gestelle (Fertigung > Gestellverwaltung > Gestelle)
- Reklamatuiongrund (Stammdaten > Produkte > Allgemein > Reklamationsgrund)
- Reklamationsverursacher (Stammdaten > Produkte > Allgemein > Reklamationsverursacher)

Die Barcodes werden, wenn die Nutzdaten nicht die mögliche Datenlänge überschreiten, mit Nullen (0) aufgefüllt (Ausnahme Gestellbarcodes). Des Weiteren erhalten alle Barcodes eine abschließende Prüfziffer. In der Mitarbeiterverwaltung (1) wurde zudem eine allgemeine Druckfunktionalität eingebaut. Die Barcodes enthalten die Personalnummer (hier 199) des Mitarbeiters (Beispiel: PE000000199F). Der Erfassungsstellenbarcode (2) wird aus der ID der Erfassungsstelle gebildet (Beispiel: ES00000000166). In dem Programm Vorgabezeiten (3) hat der Anwender jetzt die Möglichkeit einen Erfassungsstellenbarcode mit Arbeitsart für die Fertigmeldung in der Online - BDE zu drucken. Dieser setzt sich aus der ID der Erfassungsstelle und der ID der Arbeitsart getrennt mit Bindestrich zusammen (Beispiel: EA0000000015-101P). Das Druckprogramm für den Formulardruck (4) kann ab sofort auch einen Auftragsbarcode (Auftragsinfo in Online - BDE) oder einen Bestellbarcode (Wareneingang in Online - BDE) drucken. Dieser Barcode beinhaltet die Dokumentennummer, die 3-stellige Positionsnummer und eine 3 stellige Teilenummer (immer 000, da hier nur Hauptpositionen ausgegeben werden) (Beispiel Auftrag: T200000243002000Q - Beispiel Bestellung: D50000070650001.). Für die Lagerbuchung in der BDE muss entsprechend der Lagerort gescannt werden. Hierfür wurde zum einen der Barcode-Druck in dem Lagerdefinition-Dialog (5) überarbeitet und zum anderen die Online - BDE erweitert. Die Online - BDE kann ab sofort solche Lagerortbarcodes mit einem L-Präfix verarbeiten. Der Barcode beinhaltet die ID des Lagerortes (Beispiel: *L0000000001W*). Abschließend sind für die Lagerbuchung Barcodes der Lagerartikel (5) notwendig. In der Lagerverwaltung können nun die entsprechenden Barcodes, die die ID des Lagerartikels enthalten, gedruckt werden (Beispiel: LP0000000164E). Für Gestelle kann in der Gestellverwaltung (7) eine Liste von Gestellen selektiert werden und dann für diese der Barcode ausgedruckt werden (Funktionen > Gestellbarcodes drucken). Da Gestelle alphanummerisch sind, werden diese nicht mit führenden Nullen aufgefüllt.

Hinweis: Alle Barcodes werden in die Report-Variable F_IDENT_C39 des jeweiligen Formulars/Reports geschrieben.

#### Buchungshistorie

Es ist jetzt möglich, sich die getätigten Fertig- und Bruchmeldungen protokollieren zu lassen. Um die Funktionalität zu aktivieren, muss in den Firmenstammdaten auf Register 15.Kapazitätsplanung der Schalter 'Historientabelle für Fertigmeldungen füllen' aktiviert werden.

Wurde der Schalter aktiviert, werden die verarbeiteten Meldungen in der Tabelle FS_BOOK_HISTORY protokolliert. Ist die Verbuchung in die A+W Business Kapazitätsplanung aktiv, so werden die Meldungen auch bei Verbuchung in selbige protokolliert. Das gilt auch für Meldungen, die per Dialog im A+W Business getätigt werden. Ansonsten werden die Buchungen in die PD_AWBAR protokolliert.

Dabei werden folgende Daten gespeichert
- Auftragsnummer
- Positionsnummer
- Stücklistenelement
- Zeitpunkt der Scannung
- Mitarbeiter
- Erfassungsstelle
- Arbeitsart (Nur bei Buchung in Kapazitätsplanung, ansonsten 0)
- Bruchgrund (Nur bei Bruchmeldungen)
- Bruchverursacher (Nur bei Bruchmeldungen)
- Verbuchte Menge
- Ursprung (BDE, manuell, implizit)

Außerdem gibt es einen Dialog zur Auswertung der Buchungshistorie (Statistik > Buchugshistorie). Man kann dort per QBE Modus die anzuzeigenden Sätze filtern, so dass man hier genaue Statistiken z.B. pro Mitarbeiter erstellen kann.

*Abb. Y-98: BDE - Anmelden*

Beim Druck kann man sich die angezeigten Sätze dann noch zusätzlich nach zwei dynamischen Kriterien gruppieren lassen, die ebenfalls im Dialog eingestellt werden.

---

## A+W Business Gesamtindex

### Numerics
- 1 zu 1 (Register in Dokumente kopieren) C-1817

### A
- A+W B2B Purchasing Service D-2193
- A+W Business 6 Interface Service
  - Einstellungen E-2375
- A+W Production
  - Bearbeitungskatalog B-608
  - Produktverwaltung B-737
  - Übergabedatei B-606
  - übergebene Daten B-606
- AB Lieferant D-2234
  - Auftragsdaten D-2237
  - Bestelldaten D-2236
  - Bestellpositionen D-2238
  - Liefertermin D-2240
- AB siehe auch Auftragsbestätigung
- Abfragen G-2881
- Abkleben C-1759
- Abladestelle
  - Kundenkommission E-2566
  - Zuordnung E-2567
- Ablaufschema der Versandorganisation E-2313
- AB-Lieferant
  - Wareneingang D-2235
  - Wareneingang pro Position D-2239
- Abrechnungsverwaltung
  - aufgelaufene Summen B-962, C-1989
  - Details zur Abrechnung B-958
  - Einkaufsforderung B-967, C-1994
  - Forderung B-968, C-1995
  - Forderungshistorie B-969, C-1997
  - mit zugeordneten Aufträgen B-581
  - Objekt B-954, C-1983
  - Rahmenauftrag B-958, B-959, C-1986
  - Rahmenauftrag abrechnen B-582
  - Rahmenauftrag erstellen B-583
  - Stundenforderung B-966, C-1993
  - Tabelle C-1991
  - Varianten B-569
  - veranschlagte Mengen B-963, C-1990
  - zugeordnete Aufträge B-960, C-1987
  - zugeordnete Bestellungen B-961, C-1988
- Abschlag
  - Versicherungspreise B-830
- Abschlag für Serien H-2984
- Abstandhalter
  - mit Sprossen bestellen B-1097
  - Restriktion überschreiben, Passwort B-767
- Abstandhalterrestriktionen B-767
- Abweichende Anschriften (Register in Dokumentenverwaltung) C-1694
- Abweichende WGR B-732
- Abweichendes Produktkennzeichen B-238
- AD-Bereiche
  - Vertreter B-173
- AE siehe Auftragserfassung
- Aggregat H-2932
  - anlegen H-2940
  - Arbeitsgang überspringen H-3182
  - Ausfall H-3218
  - Auswahl Arbeitsart H-3107
  - Auswahl bei Ausweich-Arbeitsart H-3004
  - Auswahl bei Kapazitätsengpass H-3212
  - Auswahl beim Einlasten H-3000
  - Auswahl für manuelle Fertigmeldung H-3234
  - Folge-Aggregat überspringen H-3178
  - für Produkt sperren H-3177
  - für Produktgruppe sperren H-3175
  - für WGR sperren H-3174
  - in Fertigungsstraße sperren H-3181
  - Kalender H-3129
  - kundenbezogen sperren H-3179
  - nach Einlastung ändern H-3087
  - Priorität H-2968
  - Restriktionen angeben H-2943
  - sperren H-3005, H-3118
  - überspringen H-3005
  - vollständig, vorübergehend sperren H-3007
  - Vorgabezeit H-2967
  - Vorgabezeit festlegen H-2985
  - Zeiten und Kosten A-53, H-2935
  - Zeitkosten H-3070
  - zugeordnete Arbeitsarten H-3125
- Aggregat siehe auch Maschine
- Aggregate H-3117
  - Auslastung Leitstand Auftrag H-3308
  - Fertigungsmaße prüfen H-3105
  - im Produktionsbereich H-3139
  - Kalender H-3127
  - Kapazitätsplanung Y-3432
  - Leitstand Auftrag H-3298
  - Prioritäten H-2996
  - pro Aggregattyp H-3110
  - pro Arbeitsart H-3110
  - pro Produktionsbereich H-3110
  - SZR prüfen H-3105
  - technische Restriktion H-3124
  - Typ H-3104
- Aggregattyp H-2932, H-3104
  - Restriktionen H-2933
- zugeordnete Aggregate H-3110
- Alarmspinne C-1759
- Allgemein (Register in Erweiterte Einstellungen) C-1954
- Allgemneine Schaltflächen A-67
- Alternativangebotsübersicht C-1592
- Alternative
  - alle Gläser ersetzen C-1599
  - Angebot C-1591
  - Position C-1591
  - Position erfassen C-1593
  - Rechnung C-1402
  - Sprossen, Modell, Bearbeitung C-1600
  - zu Angebot erfassen C-1596
- Alternative (Register in Alternativen) C-1673
- Alternative ohne Stückliste H-3143
- Alternativen
  - Alternative C-1673
  - Bearbeitungen/Modelle C-1675
  - Menü Funktionen C-1669
  - Menü Optionen C-1668
  - Original C-1670
  - Sprossen C-1676
  - Texte C-1674
  - Übersicht C-1677
- Alternativen (Angebot) C-1668
- Alternativer Vorgang H-2968, H-3143
- Analyse
  - Verbrauch F-2669
- Änderungshistorie B-861
- Änderungsüberwachung
  - Historie B-603
  - Verwaltung B-603
- Anfrage
  - Referenz D-2145
  - Schnellanfrage C-1871
  - über Bestellpool erzeugen D-2147
  - unabhängige Bestellung erzeugen D-2149
  - zu Kundenauftrag erzeugen D-2146
  - zu Kundenposition D-2145
- Anfrage (Menü) D-2221
- Angebot
  - Alternative C-1591
  - Alternative erfassen C-1596
  - Alternativen C-1668
  - an Produktion übergeben E-2350
  - auswerten C-1612
  - automatische Benachrichtigung
    - aktivieren C-1606
  - Einstellungen für Produktionsübergabe B-1126
  - Erfolgsquote C-1611
  - kopieren bei Kreditlimitsperre B-1079
  - nachAuftrag kopieren B-1079
  - Optimierung C-1592, E-2348, E-2591
  - Statistik C-1666
  - Übersicht C-1660
  - Wiedervorlage C-1605, C-1663
  - Wiedervorlage abfragen C-1607
  - Zeitkosten H-3075
- Angebotsoptimierung E-2591
- Angebotsstatistik C-1666
- Anhang
  - Datei in Kundenverwaltung B-918
  - hinzufügen Drag & Drop C-1311
  - hinzufügen über Verknüpfung C-1311
  - Pfad für Datei B-1071
- Anlage (Register in Dokumentenverwaltung) C-1706
- Anlagen (Register in Artikel-Info) C-1891
- Anlagen (Register in Positionserfassung) C-1793
- Anlieferpauschale B-995
  - Zuschlag B-397
- Anmeldung Y-3433
  - Windows-Login B-1116
- Anschrift (Dokumentenverwaltung) C-1689
- Ansicht E-2612
  - Stücklisten E-2612
- Anwenderstatus B-495, B-1020, C-1485
  - für Fertigung prüfen E-2390
- Anwendungsbeispiele
  - EK-Kalkulation ISO B-621
- Anzahl
  - Komponenten in Stückliste B-1123
- Anzahlung
  - erfassen C-1538
  - fakturierte C-1536
  - mit Fakturierung erfassen C-1538
  - öffnen C-1540
  - ohne Fakturierung erfassen C-1541
  - Position C-1537
- Anzahlungen (Dialog) C-1961
- Anzahlungsdruck C-1961
- Anzahlungsrechnung C-1536
- Anzahlungssumme C-1801
- Anzahlungsübersicht C-1537, C-1844
- Anzeige
  - Artikel-, Kunden-, Lager-Info C-1292
  - Dokumentenansicht C-1582
  - im elektr. Dokument filtern D-2260
  - Übersichten C-1292
- Anzeige Beträge F-2648
- Arbeitsart
  - Aggregate H-3125
  - Ausweich-Arbeitsart H-2937
  - Faktor für Produktart H-3154
  - Lagerartikeln zuordnen H-3171
  - Leitstand H-3271
  - Leitstand Auftrag H-3302
  - speziell für Zuordnung H-3018
  - überspringen H-3005
  - Vorgabezeit festlegen H-2985, H-2987
  - Vorgänge, Tätigkeiten H-2936
  - Zeitzuschlag H-2971
  - zugeordnete Aggregate H-3107, H-3110
- Arbeitseinheit
  - Mannstunde H-2951
  - Maschinenstunde H-2954
- Arbeitsgang
  - überspringen H-3005, H-3182
- Arbeitstage H-2946
  - Kalender B-672
  - Kapazität pro Produktionsbereich H-2948
  - Zeit festlegen B-163
- Arbeitszentren siehe Produktionsbereiche
- Archiv
  - Datenbank B-1104
  - Dokument zurückholen C-1509
  - Firmendaten B-1104
- Archivierung B-440, B-441
  - automatisch C-1632
  - AV-Bereich B-1110
  - Dokument C-1632
  - Dokument löschen B-1106
  - Dokumente übergeben C-1633
  - manuell C-1632
  - mehrfach B-1107, C-1632
  - Mindeststatus B-1108
  - Modus B-1110
  - nach Erfassungsdatum B-1106
  - ohne Rechnungsnummer C-1633
  - Pfad für DMS B-1124
  - Pfad für Meldedatei B-1110
  - Referenzprüfung C-1632
- Artikel
  - Export von Stammdaten (Zoll) E-2590
  - fixiert C-1326
- Artikel fixieren C-1895
- Artikel siehe auch Produkt
- Artikel-Info
  - Anlagen C-1891
  - Info C-1888
  - Preise C-1889
- Artikel-Informationen (Dialog) C-1887
- Aufbau
  - Auswahl der Statistik F-2658
  - Ergebnis der Statistik F-2661
  - Statistik F-2658
- Aufbruch einer Kiste G-2879, K-3395
- Auflistung nach F-2634
- Auflösungstiefe
- Terminübersicht E-2574
- Aufschlag
  - Versicherungspreise B-830
- Auftrag
  - an Produktion übergeben E-2332
  - Anzahlung C-1536
  - Bestellposition C-1559
  - Direktdruck definieren B-560
  - Dokument C-1283
  - Druckauftrag anlegen B-562
  - Dummy-Kiste zuweisen E-2445, K-3361
  - Einlastung löschen H-3040
  - Einstellungen für Produktionsübergabe B-1126
  - erfassen C-1304
  - Faktura bei Teillieferung C-1520
  - Fertigungsstand H-3240
  - Festpreis festlegen C-1412
  - Folgeauftrag B-1127
  - für Stammdatentest erfassen B-486
  - Gestell zuordnen E-2397
  - importieren C-1639
  - in Kapazitätsplanung einlasten H-3034
  - intern G-2809, K-3348
  - interner Auftrag B-1127
  - kalkulatorische Frachtkosten anzeigen E-2439
  - Kapazitätsengpass lösen H-3040
  - Kopfdaten C-1297
  - Kundenverwaltung B-894
  - Lagerartikel erfassen G-2795
  - Lieferant pro Position D-2086
  - manuell einlasten H-3204
  - manuell fertig melden H-3059, H-3230
  - manuelle Preisänderung C-1398
  - nach Übergabe ändern E-2321
  - Nummernkreis C-1283
  - Nummernkreis prüfen B-1077
  - Objekt zuordnen B-573
  - Position C-1325, C-1348
  - Position erfassen C-1351
  - Produktionsauftrag G-2807
  - Produktionsdaten E-2498
  - Produktionsrückmeldungen E-2364
  - Produktionstermin ändern H-3256
  - Produktionsübergabe stornieren E-2334
  - Rechnung C-1287
  - Reklamation C-1544
  - Reservierung A-46
  - Schnellanfrage C-1350, C-1357
  - Schnittstellen C-1285
  - Sperrkennzeichen C-1286
  - Status scannen E-2394
  - Status umsetzen E-2518
  - Steuer C-1288
  - Stücklisten-Kiste K-3341
  - Teillieferung C-1518
  - Termine C-1299
  - Text erfassen C-1308
  - überrechnen C-1964
  - umlasten H-3082
  - versandfertig melden E-2394
  - Zeitkosten H-3075
  - zum Objekt B-960, C-1987
  - zum Rahmenauftrag erfassen B-586
  - Zuschläge C-1404
- Auftrag (Menü) C-1958
- Aufträge
  - zusammenstellen (Versand) E-2593
- Auftrags-/Bestell-Info C-1845
- Auftragsbestand B-911
- Auftragsbestätigung
  - des Lieferanten erfassen D-2123
  - drucken C-1463
  - Einkauf D-2121
  - elektr. Preiskontrolle D-2250
  - für Position erfassen D-2125
  - Lieferant D-2234
  - Preis pro Position D-2247
  - Preise prüfen D-2180
  - Preiskontrolle D-2241
  - Stücklistenpreise D-2249
- Auftragsbezogen (Register in Suchdialog) C-1804
- Auftragsdaten
  - AB Lieferant D-2237
- Auftragsformulare
  - Direktdruck B-557, B-1213
- Auftragsinfo
  - Vorhaltetage B-1111
- Auftragsinformation F-2630
  - Druckeinstellung F-2641
  - Erfasst F-2636
  - Fakturiert F-2638
  - Grafik F-2640
  - Offen F-2639
  - Optionen F-2632
  - Produziert F-2637
- Auftragskopf
  - Geschäftsart C-1298
- Auftragsposition C-1348
  - Buchung prüfen G-2799
  - einzeln einlasten H-3038
  - kostenlos C-2000
  - Split H-3030
  - splitten H-3042
- Auftragsstatus
- manuell umsetzen E-2392
- Auftragsverwaltungsbereich siehe AV-Bereich
- Ausfall
  - Aggregat H-3218
- Ausgangs-Journal C-2018
- Ausgleichposition D-2257
- Auslastung
  - Aggregate (Leitstand) H-3264
  - Aufträge (Leitstand) H-3265
  - Fertigmeldungen H-3223
  - Grafik H-3291
  - pro Produktionsbereich (Leitstand) H-3263
  - Schichten H-3275
  - Status einstellen H-3293
  - Übersicht drucken H-3292
  - Übersicht zu Datum H-3286
  - Voreinstellungen H-2955
  - Vorprozesse (Leitstand) H-3276
  - zum Datum H-3287
- Austausch
  - Bearbeitung in Stückliste beibehalten B-1080
  - Gas mit SZR B-1077
  - Vererbung B-1077
- Austauschrabatt (Rabattverwaltung) B-940
- Austauschzuschlag B-358, B-788
  - anlegen B-361, B-364
  - auf Austauschglas B-364
  - dickenabhängiger Austauschzuschlag B-358
  - einem Partner zuordnen B-361
  - kopieren B-366
  - produktabhängiger Austauschzuschlag B-358
  - Produktverwaltung B-719
  - Übernahme Rabatt B-1089
  - unabhängiger Austauschzuschlag B-358
  - Zuschlag auf Eintauschglas B-361
- Auswahl
  - Lagerhistorie G-2885
  - nach Klassifikatoren (Register in Produktsuche) C-1870
  - nach Produkt (Register in Produktsuche) C-1867
  - nach technischen Parametern (Register in Produktsuche) C-1869
  - Rubriken in Umsatzstatistik F-2647
  - Umsatz VK, EK F-2644
  - Verbrauchsanalyse F-2669
- Auswärtig
  - Gestell mahnen E-2552
- Auswärtiges Gestell, Ausgang
  - Gestell E-2545
- Ausweich-Arbeitsart H-2937
  - Arbeitsarten H-3107
  - Auswahl des Aggregats H-3004
- Ausweichartikel
  - Produktverwaltung B-710
- Auswertung
  - Deckungsbeitrag C-2002
  - Kalkulatorische Frachtkosten C-2006
- Auswertungen
  - Null-Preisreport C-2000
- Auswertungen (Auftrag) C-1998
- Außendienst B-173
- Außendienstbereich B-1161
- Außendienstmitarbeiter B-1161
- Autoaufleger
  - Kennzeichen B-1012
- Automatisch
  - Archivierung C-1632
  - Gestell anlegen E-2542
  - Wiedervorlage von Angeboten C-1606
- Automatische Zuschläge B-395
  - verfügbare Zuschläge/Rabatte B-397
- Automatischer Zuschlag B-396
- Automatischer Zuschnitt
  - Kennzeichen (Produktverwaltung) B-726
- Avalara WebService B-1060
- AV-Bereich B-510
  - Dialog B-1160
  - Dokumententyp B-1153
  - Geschäftsart (Dokumentenkopf) C-1298
  - Gestellrechnung B-1135
  - Kundenstatistik F-2663
  - Laufnummer B-1110
  - Nummernkreis einrichten B-511
  - Nummernkreis prüfen B-1077
  - Nummernkreis sperren B-513
- AV-Bereichsstatistik
  - kurz H-3192
  - lang H-3188
- AW Common Base Service D-2193
- AW-Broke B-713
- AWDesign
  - Schnittstelle E-2472
- AWProtocolService D-2193
- AWRack
  - Gestellrechnung B-1135

### B
- Bank
  - allgemeine Banken B-1044
  - Bankkonten der Firma B-1167
  - Bankverbindung anlegen B-445
  - IBAN, BIC B-151
  - Mandant B-151
  - zur Filiale anlegen B-445
- Bankbelege
  - Wechseldruck Verwaltung C-1962
- Bankeinzug B-905
- Barcode
  - Positionsübergabe E-2493
  - Scanvorlage herstellen E-2398
  - Status umsetzen E-2394
- Barcodeübergabe
  - Details E-2494
  - Prüfziffer E-2495
- Basisnummernkreise B-675
- Basistabelle B-93
  - Eintrag sperren B-94
  - neuen Eintrag anlegen B-93
- Basiszeit H-3143
  - Arbeitsgang H-2967
  - Staffelung H-2969
  - Staffelung anlegen H-2985
  - Zeitwert eintragen H-2987
- BDE
  - Anmeldeinformation Y-3456
  - Anmeldung Y-3433
  - Auftragsinformation Y-3455
  - Ausdrucken von Barcodes Y-3457, Y-3458
  - Barcodes Y-3457
  - Funktionen Y-3433
  - Gestelle Y-3450
  - Gestellfunktionen Y-3451, Y-3453, Y-3454
  - Gestellmenü Y-3450
  - Hauptmenü Y-3434
  - Lagerbewegungen Y-3439
  - Mitarbeiterwechsel Y-3456
  - Produktionsmeldung Y-3436
  - Sonstige Funktionen Y-3455
  - Statusmeldungen E-2394
  - Statusvergabe B-498
- BDE-Buchungen
  - lückenlose Buchung A-59
- Bearbeitung
  - als Vorlage speichern C-1430
  - bei Austausch beibehalten B-1080
  - Bezeichnung 3 B-707
  - in Position erfassen C-1373
  - Produktionsstücklistenauflösung B-242
  - Rabatt aus Hauptposition B-1089
- Bearbeitungen B-777
  - Abkleben C-1759
  - Alarmspinne C-1759
  - Beschichtung C-1754
  - Biegen (Glas) C-1756
  - Durchsprechöffnung C-1752
  - Eckausschnitte C-1750
  - Emaillierung C-1758
  - Entschichtung C-1759
  - Flächen-Emaillierung C-1754
  - Handgriffe C-1752
  - Innenausschnitte C-1752
  - Kantenbearbeitung C-1746
  - Kantenschutz C-1757
  - Kolorieren C-1754
  - Lochbohrung C-1747
  - Logo C-1757
  - Mattierung C-1754
  - Nachschleifen C-1757
  - Parameter C-1745
  - Produktverwaltung B-728
  - Randentschichtungen C-1756
  - Randsiebdruck C-1760
  - Rillenschliff C-1756
  - Rundecken C-1749
  - Sandstrahlen C-1754
  - Schaltflächen C-1320
  - Schrägschnitte C-1750, C-1751
  - Senkbohrung C-1748
  - Siebdruck C-1754
  - SN Makro C-1758
  - Stempel C-1757
  - Stufenbohrung C-1749
  - Verklebung C-1746
- Bearbeitungen (Positionserfassung) C-1744
- Bearbeitungen/Modelle (Register in Alternativen) C-1675
- Bearbeitungsindex B-318
  - Produktverwaltung B-721
- Bearbeitungskatalog B-608
- Bearbeitungsrestriktionen B-772
- Bearbeitungsvariable B-707
- Bearbeitungszuschlag
  - Modellzuschlag anlegen B-372
- Bedienelemente
  - Dokumentenverwaltung C-1294
  - Positionserfassung C-1315
  - Voreinstellungen C-1315
- Bedienoberfläche
  - Standard-Menüs A-66
  - Standard-Schaltflächen A-67
- Beispiel
  - Berechnung bei Übergangs- und Verweilzeiten H-2978
  - Berechnung der Kapazitäten H-3024
  - bohrpunkt-symmetrisch B-228, C-1328
  - Dreiecksform (Matrix) B-316
  - feld-symmetrisch B-228, C-1328
  - Fremdwährung B-158, B-531
  - Grenztyp B-316
  - Gruppen- und Mitarbeiterrechte B-457
  - Lieferdauer B-183, C-1300
  - Nummer für Kombi-WGR B-208
  - Nummernkreise B-508, C-1284
  - Planzeit für ISO H-2972
  - Rundung B-516
  - Rundung im Auftrag B-519
  - Skontoberechnung B-159
  - Sonstiger Zuschlag B-376
  - Textkennzeichen B-129, B-537
  - Zuschlag auf Basisposition B-382
  - Zuschlag auf Basisposition + Bearbeitung B-383
  - Zuschlag auf Basisposition + Modell B-384
  - Zuschlag auf Basispreis B-381
  - Zuschlag auf vorherige Bearbeitung B-384
  - Zuschlag auf vorherige Position B-385
  - Zuschlag mit additiver Berechnung B-386
  - Zuschlag mit nicht additiver Berechnung B-386
- Beladung
  - Gewicht E-2531
  - Liste drucken E-2408
- Bemerkung zur Lagerbewegung G-2880, K-3396
- Benachrichtigung
  - Terminänderung C-1851
- Benutzeroberfläche A-26
- Berechnung
  - Ablauf EK-Preisberechnung G-2729
  - Bearbeitung nach Menge B-1089
  - Bohrung für Sprossen B-228, C-1328
  - Einzelpreis B-1088
  - Fremdwährung B-158, B-531
  - Lieferdauer B-183, C-1300
  - nach Zuschlagsart B-379
  - Preise im Auftrag C-1399
  - preisrelevant VK/EK B-233
  - Provision B-1076
  - Rundung B-184, B-516
  - Rundungsbeispiel B-519
  - Rundungspunkt B-518
  - sonstige Zuschläge B-388
  - sonstige Zuschläge aus Stückliste B-1090
  - Sprossen pro Gitter B-1088
  - Sprossenkonstruktion B-228, C-1328
  - Steuer pro Position in Stückliste B-1078
  - Verschnitt G-2718
  - Zuschlag auf Bearbeitung B-387
- Berechnungsgröße
  - Preiseinheiten B-297
- Beschaffungsart G-2715
  - in Produktverwaltung B-236
- Kennzeichensuche B-1076
- Produktverwaltung B-725
- Beschichtetes Glas
  - Produktverwaltung B-715
- Beschichtung B-225, C-1754
- Beschichtungsart B-225, B-694
- Beschichtungsseite B-693
- Beschlagszuordnung B-776
- Besondere Priorität H-2996, H-3151
- Bestandslisten
  - Nummernbereiche C-2021
  - Warengruppen C-2023
- Bestandslisten (Menü) C-2021
- Bestellanfrage D-2221
- Bestellarten
  - Lagerbestellung D-2114
  - referenzierte Bestellung D-2079
  - unabhängige Bestellung D-2114
- Bestellartikel
  - komplett (Produktverwaltung) B-725
- Bestelldaten
  - AB Lieferant D-2236
- Bestellkennzeichen
  - Einkauf D-2056
- Bestellmengenfaktor
  - Produktverwaltung B-725
- Bestellnummern (Register in Bestellübergabe) C-1943
- Bestellpool D-2096
  - Anfrage erzeugen D-2147
  - Lieferant ändern D-2106
  - Preise vergleichen D-2108
  - Sammelbestellung D-2101
- Bestellpool (Register in Bestellübergabe) C-1946
- Bestellposition
  - AB erfassen D-2125
  - im Auftrag erfassen D-2088
  - Produktion D-2156
- Bestellte Position ändern D-2091
- Bestellteile
  - Auftrag (Fertigungsstand) H-3249
  - Fertigmeldungen H-3225
  - Leitstand H-3278
  - Leitstand Auftrag H-3304
- Bestellübergabe
  - Bestellnummern C-1943
  - Bestellpool C-1946
  - Erweiterte Einstellungen C-1953
  - Lieferant/Termin ändern C-1949
  - Markierungsoptionen C-1950
  - Menü Funktionen C-1940, G-2901, K-3403
  - Menü Optionen C-1941, G-2902, K-3404
  - Preisvergleich C-1951
  - Stücklistenübersicht C-1957
- Bestellung
  - an Einkauf übergeben G-2784
  - Auftragsbestätigung D-2121
  - aus Kundenauftrag D-2085
  - aus unabhängiger Anfrage erzeugen D-2149
  - automatisch D-2094, G-2783, K-3355
  - Bestellmenge nach Bestandsprüfung G-2810, K-3347
  - Bestellpool D-2096
  - bestellte Position ändern D-2087, D-2091
  - Bestellübergabe C-1562
  - Bestellvorschlag übergeben G-2784
  - Eingangskontrolle D-2159
  - elektr. Preiskontrolle D-2250
  - elektr. Rechnungskontrolle D-2293
  - Export (Dokument) D-2229
  - Fremdwährung D-2179
  - geänderten Wert zurückschreiben B-1076
  - ISO ohne Eigenfertigung B-1097
  - Kennzeichen ändern C-1572
  - Kiste erfassen D-2117, K-3357
  - Kundenbestellung D-2085
  - Lager G-2901, K-3403
  - Lagerbestellung erfassen D-2117
  - Lieferanten ändern C-1568, D-2106, G-2787
  - Lieferantenauswahl C-1562
  - Lieferantenkartei C-1560
  - Liefertermin D-2099
  - Mahnung D-2122
  - manuell D-2079
  - manuell erfassen D-2115
  - Mengendiskrepanzen D-2280
  - Mindestmenge und Bestellmenge G-2783, K-3355
  - Position C-1577
  - Position im Auftrag C-1559
  - Preiskontrolle D-2244
  - Preisvergleich C-1570, D-2099, G-2789
  - Produktionsübergabe E-2321
  - Produktkennzeichen C-1559
  - Rechnungskontrolle D-2285
  - Referenzen C-1578
  - Sammelbestellung D-2101
  - Teilbestellung D-2296
  - Termin ändern G-2787
  - Terminüberwachung D-2135
  - Übergabe C-1940
  - übergeben C-1564, D-2102
  - unabhängige Bestellung D-2114
  - unabhängige Bestellung erfassen D-2115
  - Vorlauftage B-681
  - Vorschlag G-2783, K-3355
  - Wareneingang komplett D-2278
  - zum Objekt B-961, C-1988
- Bestellung (Menü) D-2223
- Beträge durch Tausend geteilt F-2635
- Betragsdifferenz
  - elektronisches Dokument D-2192
  - Produktzuordnung D-2257
- Betriebsdatenerfassung siehe BDE
- Betriebsferien
  - eintragen B-163
  - Zahlungstagverschiebung B-145
- Betriebsnummer B-1058
- Bewertung
  - FIFO/LIFO G-2911
- Bezeichnung 3 (bei Bearbeitungsprodukt) B-707
- Bezugsschein
  - Zollverwaltung E-2584
- Biegen (Glas) C-1756
- Blattanzahl einer Kiste G-2878, K-3394
- Blattanzahl korrigieren K-3371
- Bleiverglasung C-1759, C-1767
- Bleiverglasungstyp B-602
- BMECat
  - Firmendaten B-1145
- Bohrpunkt
  - Beispiel C-1328
  - Sprossen B-228
- Bohrpunkt für Sprossen A-32
- Bonität B-1043
  - Kundenverwaltung B-907
- Branchen B-878
- Breite
  - in Stückliste (Produktverwaltung) B-732
  - Mindestmaß für Produktion (Produktverwaltung) B-709
- Bruch
  - Meldung manuell erfassen H-3062
  - Rückmeldung H-3052
- Bruchgründe B-1014
- Bruchmeldung Y-3438
- Bruttotage C-1469
- Buchen
  - Teillieferung D-2253
  - Wareneingang D-2161
- Buchung
  - Aggregate (Produktionsdaten) E-2501
  - für Auftragsposition prüfen G-2799
- Buchungsart
  - Dokumentenimport D-2190
  - elektronische Preiskontrolle D-2253
  - für Lager B-870
  - für Lagerbuchung G-2721
  - Lager G-2754
  - Preiskontrolle D-2253
- Buchungshistorie Y-3459
- Buchungsjournal G-2881
  - für Lager erstellen G-2765
  - Lagerwirtschaft A-62, G-2764
- Buchungsperiode B-1170

### C
- CE
  - CPIP-Code B-1233
  - ISO-Daten B-1235
  - Maßrestriktionen B-1234
- CEKAL B-1222
  - Ergebnis B-1225
  - Klasse B-1223
  - Parameter B-1072
  - Produkttext B-1231
  - Restriktion B-1229
  - Textzuordnung B-1227
  - Zuordnung B-1224
- Common Base B-1135
- CPIP
  - CE-Kennzeichen B-1233

### D
- Darstellungskonventionen -3
- Datei
  - anhängen C-1311
  - Pfad für Anhang B-1071
- Dateianhang
  - Bemerkungen B-1194
- Dateilose Produktionsrückmeldungen E-2370
- Daten
  - Archivierung B-440
  - Reihenfolge beim Anlegen B-91
  - Statistik B-442
  - Übergabe an A+W Production B-606
- Datenaustausch D-2184
  - Artikelimport B-1259
  - Dokument D-2185
  - EDI-Einstellungen B-1237
  - Fremdartikel kopieren B-1245
  - Fremdschnittstellenverwaltung D-2212
  - Gas B-1247
  - Marktpartner B-1249
  - open Trans B-1255
  - open TRANS-Dokument einlesen D-2203
  - SN-Regeln B-1258
  - SZR-Daten B-1246
  - Tour B-1248
  - XML-Datei einlesen D-2203
- Datenbank
- Archiv B-1104
- Kundenkürzel B-1115
- Mandanten B-442
- Maßsystem B-1113
- Datenexport
- EDI D-2211
- Datenformate
- Rückmeldedateien E-2355
- Datensicherheit A-26
- Datenübergabe
- an Produktion E-2316
- FiBu C-1617
- OrderXML E-2317
- Übergabedatei C-1619
- Datum
- Format B-1114
- Teillieferung B-1074
- Deckungsbeitrag B-1121
- Analyse C-2002
- Grenzwerte B-978
- Defaultrabatt B-936
- Definition
- Vorschauspalten E-2581
- Definition von Kostenstellen (Kapa) H-3194
- Detail
- Leitstand H-3273
- Leitstand Auftrag H-3300
- Detailübersicht (Register in Suchdialog) C-1812
- Dialog
- Preisanzeigen C-1396
- Dicke B-709
- metrisch, imperial B-1113
- Dickenabhängiger Austauschzuschlag B-358
- Dienste
- A+W B2B Purchasing Service D-2193
- AW Common Base Service D-2193
- AWProtocolService D-2193
- ERP-WebService D-2193
- Differenz
- Rechnungskontrolle D-2288
- Direktdruck B-557, C-1455
- Auftragsformulare B-1213
- definieren B-560
- Direkthilfe C-1316
- Dokument
- ändern C-1291
- Angebot C-1591, C-1660
- anhängen C-1311
- Anzahlung C-1536
- Anzahlung suchen C-1540
- anzeigen C-1829
- Auftrag C-1283
- aus dem Archiv zurückholen C-1509
- automatisch löschen B-1108
- Bestellung C-1576, D-2079
- Dokumentendaten C-2031
- doppelt erfasst C-1291, C-1648
- E-Mail-Versandart B-1067
- Erfassung C-1289
- Faxversand gesammelt B-1067
- Festpreis erfassen C-1412
- Folgedokument C-1281
- Formular C-1451
- Formularzuordnung B-547
- Gutschrift C-1553
- Historie C-1477
- Historie prüfen C-1479
- Journal C-1646
- Kopfdaten C-1297, C-1679
- Kopie aus dem Archiv C-1508
- kopieren C-1813
- Kopieren (Dialog) C-1509
- löschen C-1307
- löschen (Automatikoptionen) B-1108
- manuelle Statusvergabe C-1497
- nach Archivierung löschen B-1106
- Nummernkreis C-1283
- Nummernverwalter ändern C-1448
- ohne Referenzprüfung löschen B-1106
- Organisation im Ablauf C-1441
- Positionen C-1711
- Positionserfassung C-1725
- Positionspreis C-1348
- positionsweise kopieren C-1513
- referenzierte Dokumente C-1581
- Reklamation suchen C-1546
- sperren B-1078
- Status C-1481
- suchen C-1306
- Teillieferung C-1517
- Teillieferung erfassen C-1521
- Teillieferung suchen C-1526
- Text erfassen C-1308
- Typ B-593
- Übersicht in Objektverwaltung B-965, C-1992
- verfügbare Dokumententypen B-593
- Verkauf C-1281
- vollständig kopieren C-1509
- Dokument (Register in Dokumentenverwaltung) C-1688
- Dokument (Register in Fremddokumentenverwaltung) C-1980
- Dokumente
- Anfrage, Bestellung A-42
- Angebot, Auftrag A-38
- Bestellanfrage D-2221
- Bestellung D-2223
- Einkauf D-2220
- Hotkeys zur Erfassung A-68
- Nummernkreise B-1028
- Dokumente (Register ...)
  - Firma B-1066
  - Nummernkreise B-1028
- Dokumente kopieren
  - Kopieren 1 zu 1 C-1817
  - Menü Optionen C-1813
  - Menü Übersichten C-1816
  - Optionen Quelldokument C-1827
  - Optionen Zieldokument C-1825
  - positionsweise C-1823
  - Texte C-1828
- Dokumentenarchivierung
  - Kennzeichen B-1214
- Dokumentenaustausch D-2184
  - Dienste D-2193
  - openTRANS D-2185
  - Referenzen D-2188
  - XML-Datei D-2185
- Dokumentendaten C-2030
  - Dokument C-2031
  - Menü Funktionen C-2030
  - Menü Optionen C-2030
- Dokumentenexport
  - Formulardruck C-1935
- Dokumentenimport D-2189
  - Buchungsart D-2190
  - Fußzuschläge/-rabatte D-2191
  - openTRANS-Datei einlesen D-2203
  - Positionszuordnung D-2191
  - Rundungsdifferenz D-2192
  - XML-Datei einlesen D-2203
- Dokumentenstatus D-2254
- Dokumententyp B-1036
- Dokumentenüberwachung C-1648
- Dokumentenverwaltung
  - Abweichende Anschriften C-1694
  - Alternativangebotsübersicht C-1677
  - Anhang C-1706
  - Anzahlungsübersicht C-1844
  - Auftrags-/Bestell-Info C-1845
  - Bedienelemente C-1294
  - Dokument C-1688
  - Dokument löschen C-1307
  - Dokumentenkopf C-1679
  - Duplikate C-1847
  - Historie C-1834
  - Infos C-1802
  - Interne Kontrolle C-2011
  - Kalkulatorische Frachtkosten C-1858
  - Kapazitätsinfo C-1854
  - Kapazitätsübersicht C-1831
  - Konditionen C-1700
  - Kopfdaten erfassen C-1304
  - Kosten-/Aufschlagskalkulation C-1859
  - Kosten-/Aufschlagskalkulation (Position) C-1898
  - Kreditlimitsperre C-1857
  - Kundeninfo C-1709
  - Lieferterminkontrolle C-1848
  - Menü Ansicht C-1680, C-1712
  - Menü Aufbau C-1686, C-1722
  - Menü Customizing C-1686, C-1723
  - Menü Druck C-1679, C-1712
  - Menü Funktionen C-1681, C-1714
  - Menü Optionen C-1684, C-1717
  - Menü Start C-1712
  - NV Auswahl C-1838
  - OP Abfrage C-1856
  - Optionen zur Bedienung C-1295
  - Positionen C-1725
  - Produktion C-1680
  - Referenzen C-1802
  - Reklamationsübersicht C-1843
  - Startmodus C-1295
  - Statusänderung C-1836
  - Statusrückmeldung C-1860
  - Summen C-1797
  - Technische Parameter C-1707
  - Teillieferungen C-1901
  - Teillieferungsübersicht C-1841
  - Texte C-1704
  - Zusatz C-1696
- Dreiecksform H-2969
  - Vorgabezeit H-3145
- Dreiecksform (Matrix) B-323
  - Beispiel B-316
- Druck C-1923
  - Auftragsinfo F-2641
  - Ausgabeformate B-549
  - Direktdruck C-1455
  - Dokumentenexport C-1935
  - Druckauftrag C-1455
  - Druckmodus C-1453
  - Einstellung für Modelle B-554, C-1457
  - Einstellung für Sprossen B-554, C-1457
  - Einstellungen für Preis B-552, C-1462
  - Etiketten (Dokumente) C-1933
  - Firmendaten B-1122
  - Formular C-1451
  - Formular-/Etikettendruck (Dialog) C-1926
  - Formulare (Dokumente) C-1927
  - Kalkulatorische Frachtkosten C-2007
  - Kundenverwaltung B-886
  - Modus C-1925
  - Monatsrechnung B-1122
  - Preisdarstellung B-550, C-1460
  - Rechnung C-1454
  - Rechnungsdruck sperren B-1078
  - Servername B-1123
  - Skizze B-552, C-1456
  - Stückliste C-1456
  - Stückliste (Produktverwaltung) B-733
  - vermaßte Skizze B-555, C-1458
  - Vermaßte Skizze (Dialog) C-1936
  - Voreinstellungen C-1456
- Druckauftrag B-558, C-1455
  - anlegen B-562
- Drucken
  - Auftragsbestätigung, Rechnung, Lieferschein C-1463
  - Etiketten C-1465
  - Formular C-1463
  - Lieferschein, Rechnung, Teilrechnung C-1463
- Drucklauf B-558
  - anlegen B-562
- Druckoptionen
  - Formularverwaltung B-1201, B-1205, B-1208
- Druckpunkt B-546, B-1021
- Druckvorlagen B-546
- Duplikat
  - für gesperrten Kunden B-1079
- Duplikate
  - anzeigen C-1847
- Durchschnitts-EK G-2728
- Durchschnittspreis (Lager) G-2730
- Durchsprechöffnung C-1752

### E
- Ebene
  - Struktur, Beschichtung B-226
- Eckausschnitte C-1750
- EDI
  - autom. Einlastung in Kapa B-1102
  - Einstellungen für Datenexport D-2212
  - Export D-2211
  - Firmendaten B-1096
  - Fremdartikel B-1238
  - Fremdartikel kopieren B-1245
  - Fremdschnittstellenverwaltung D-2212
  - Marktpartner B-1249
  - Parameter B-1251
  - Schnittstelle B-1237
  - Sicherungsdatei B-1111
  - Vorhaltetage B-1111
- Eigenständige Filiale B-890
- Eigenwährung B-1059
- Eilzuschlag B-896
- Eingang
  - Gestell E-2548
- Eingangs-Journal C-2018
- Eingangskontrolle D-2278
- Einheit
  - Preis B-824
- Einkauf
  - Anfrage D-2144, D-2221
  - Beschaffungsart D-2057
  - Bestellkennzeichen D-2056
  - Bestellübergabe aus Auftrag D-2094
  - Bestellung D-2225
  - Dokumente D-2220
  - Firmendaten für Bestellung prüfen D-2081
  - Firmendaten prüfen D-2195
  - Firmendaten prüfen (Kisten) D-2170
  - Grundgedanken D-2051
  - Handlungsablauf D-2052
  - Liefertermin D-2121
  - Menü-Übersicht D-2048
  - Nachbestellung D-2227
  - Preiskontrollen D-2177
  - Preislisten D-2071
  - Produktverwaltung B-723
  - Rechnungskontrolle D-2178
  - Reklamationsstatistik F-2666
  - Schema D-2051
  - Schnittstellenverwaltung prüfen D-2212
  - Stammdaten Lieferant prüfen D-2066
  - Stammdaten Preise prüfen D-2072
  d - Stammdaten Produkt prüfen D-2059
  - Stammdaten Währung prüfen D-2196
  - Status D-2075
  - Status für elektr. Dokument prüfen D-2197
  - Statuszuordnung D-2075
  - Umsatz F-2665
- Einkaufsforderung B-967, C-1994
- Einkaufspreis G-2733
  - Durchschnitt B-1096
  - ermitteln B-1096
- Einlasten
  - Aggregat automatisch wählen B-1140, H-3100
  - Auftrag H-3034
  - automatisch H-3028
  - automatisch in Kapazitätsplanung B-1102
  - Einstellungen für automatisches Einlasten H-3010
  - einzelne Position in Kapazitätsplanung H-3038
  - Engpass auflösen H-3041
  - Ergebnis prüfen H-3209
  - in Kapazitätsplanung H-3028
  - Kapazitätsengpass H-3212
  - Kapazitätsprobleme H-3029
  - manuell H-3028
  - nach Auftrag H-3204
  - nach Nummernverwalter H-3198
  - Position splitten H-3042
  - Positionssplit H-3215
  - Sperrstunde H-3032
  - Suche nach Liefertermin B-1142, H-3101
  - Terminberechnung A-55, H-3024
  - Terminsuche H-3201
  - Workflow-Task H-3028
- Einlastung
  - Aggregat ändern H-3087
  - Auftrag verschieben H-3082
- Einstellung
  - Superstatistik F-2653
- Einstellungen
  - A+W Business 6 Interface Service E-2375
  - automatisch einlasten H-3010
  - FiBu-Übergabe C-1972
  - für automatische Produktionsübergabe E-2327
  - für dateilose Produktionsrückmeldung E-2366
  - für Produktionsübergabe prüfen (A+W Business-Kapazitätsplanung) E-2340
  - für Produktionsübergabe prüfen (A+W Production Capacity Planner) E-2346
  - für Produktionsübergabe prüfen (Aufträge) E-2341
  - für Produktionsübergabe prüfen (ohne Kapa) E-2328
  - Gestellbelegung E-2489
  - kalkulatorische Frachtkosten E-2436
  - KAPS-Datei E-2515
  - Kisten-ID D-2277, K-3420
  - Lauf H-3229
  - Leitstand H-3293
  - manuelle Fertigmeldung H-3234
  - Produktionsliste H-3239
  - Produktionsübergabe E-2470
  - Produktionsübergabe mit A+W Business-Kapazitätsplanung E-2339
  - Produktionsübergabe mit A+W Production Capacity Planner E-2343
  - Produktionsübergabe ohne Kapa E-2326
  - Produktionsübergabe von Angeboten E-2349
  - Rückmeldungen H-3049
  - Rückmeldungen aus der Produktion E-2361
  - Scanner Y-3428
  - Sprossenkonstruktion E-2621
  - Statusmeldung E-2523
  - Stücklistenansicht E-2613
  - Voreinstellungen in Firmendaten H-3010
- Einzelpreis B-296
  - anlegen B-301
  - Berechnung B-1088
- EK
  - Firmendaten B-1096
- EK-Kalkulation
  - Anwendungsbeispiel (ISO) B-621
  - ISO B-621
  - Vorgaben B-765
  - Vorgaben festlegen B-619
- EK-Preis
  - durchschnittlicher EK G-2728
  - Einstellungen prüfen G-2732
  - kombinierter Lagermodus G-2728
- EK-Rückschreibung
  - Lagerbewertung D-2179
- Elektr. Dokument
  - Status D-2194
- Elektronische Rechnungskontrolle D-2293
- Elektronischer Datenaustausch D-2184
  - Anzeige D-2260
  - Dokumentenstatus D-2254
  - EDI-Schnittstelle (Einstellungen) D-2212
  - Filtereinstellungen D-2260
  - openTRANS-Einstellungen D-2200
  - Preiskontrolle D-2250
  - Rechnungskontrolle D-2293
  - Referenzen D-2195
  - Schnittstellenverwaltung D-2200
  - Währungen D-2196
- Elektronischer Dokumentenaustausch
  - Dienste D-2193
  - Firmendaten D-2195
  - Partnerstammdaten D-2202
  - Position zuordnen D-2258
- Elektronisches Dokument
  - Betragsdifferenz D-2192
  - Position zuordnen D-2207
  - prüfen D-2204
  - Teillieferung erstellen D-2206
  - Zuschlag/Rabatt verteilen D-2209
- Elektronsicher Dokumentenaustausch
  - Statusdefinition D-2197
- E-Mail
  - Adressen für Export B-1255
  - Mandant B-1057
  - Versandart B-1067
- Emaillierung C-1758
- Empfangsbetätigungsliste E-2533
- Engpass
- auflösen H-3041
- Wahl des Liefertermins H-3034
- Entfernungspauschale E-2380
- Entschichtung C-1759
- Entschichtungszuschlag B-398
- Erfassen
  - Auftrag C-1304
- Erfassung
  - automatisiert C-1348
  - Daten über Nummernblock eingeben C-1295
  - Dokument C-1289
  - Kreditlimit C-1301
  - Makro C-1420
  - Position C-1351
  - Position über Schnellerfassung C-1356
  - Schnellanfrage C-1350
  - Schnellanfrage beantworten C-1357
  - Schnellerfassung C-1349
  - Stückliste C-1326
  - über Nummernblock C-1295
- Erfassungsstelle
  - A+W Production-Beispiele E-2355
  - für dateilose Rückmeldung prüfen E-2366
  - für Fertigmeldung zuordnen E-2360
  - für Produktionsauftrag zuweisen E-2428
  - für Produktionsrückmeldungen E-2357
  - für Rückmeldung aus Produktionsauftrag E-2427
  - Produktion B-1004
  - Rückmeldung (Firmendaten) B-1103
  - zuordnen E-2358
- Erfassungsstellen
  - A+W Business Stammdaten Y-3430
- Erfolgsquote C-1611
  - auswerten C-1612
- Ergebnis
  - Verbrauchsanalyse F-2674
- Erlöskonten C-1620
  - kopieren B-1049
- ERP-System A-22
- ERP-WebService D-2193
- ERP-Webservice E-2472
- Erstinventur G-2834
- Erweiterte Einstellungen
  - allgemein C-1954
  - Bestellübergabe C-1953
  - Sortierung C-1955
- Erweiterte Objektverwaltung B-575
  - Details zum Objekt B-956
- Etikett
  - für Kiste drucken D-2176
- Etiketten
  - Druck (Dokumente) C-1933
  - drucken C-1465
- Exakte Laufmeter
  - Kantenbearbeitung B-1073
- Exklusiv-Status
  - Mitarbeiterverwaltung C-1503
- Explizit B-231
  - Preisdarstellung B-718
- Explizit (Preisdarstellung) C-1737
- Export
  - Artikelstammdaten (Zollverwaltung) E-2590
  - Bestellung D-2231
  - Datenexport per EDI D-2229
  - Dokument (openTRANS) D-2187
  - Dokumente B-1255
  - EDI-Einstellungen D-2212
  - Superstatistik B-1105, F-2655
  - Terminübersicht E-2576
  - Übertragungspool D-2233
  - Zahlungen C-1973
- Externe Kundennummer D-2202

### F
- Fachberater=Erfasser (AE) C-1685
- Fahrer
  - anlegen E-2403
  - Empfangsbestätigungsliste drucken E-2408
  - Kommissionierung E-2528
  - Stammdaten anlegen E-2403
- Fahrer (Dialog) B-999
- Fahrzeug
  - Beladung zusammenstellen E-2404
  - Beladungsliste drucken E-2408
  - Stammdaten anlegen E-2402
  - Zuladung E-2401
- Faktor
  - Berechnungsbeispiel für Zeitplanung H-2976
  - Serien H-2984
  - Zeitvorgaben H-2975
- Faktor für
  - Arbeitsart H-3154
  - Folgebearbeitung H-3161
  - Folgebearbeitung+Modell H-3167
  - Kantenbearbeitung H-3165
  - Kombi-Produktart H-3159
  - Kombi-Produktgruppe H-3169
  - Modell H-3163
  - Produkt H-3158
  - Produktgruppe H-3157
  - Sonderzeit H-2984
  - WGR H-3156
- Faktoren
  - Mischkalkulation B-1068
- Faktura
  - Steuern B-529
- Fälligkeit
  - Berechnung C-1469
  - Bezugsdatum B-144, C-1470
  - Kennzeichen B-143, C-1469
- Fälligkeiten
  - kundenspezifische Einstellungen B-142
- Faxversand
  - Druckauftrag B-1214
  - Partnerverwaltung B-892
  - pro Dokument B-1067
- Feiertage B-163
- Fertigmeldung Y-3437
  - Auftrag manuell fertig melden H-3230
  - Bestellteile H-3225
  - Einstellung für Lauf H-3229
  - Fertigungsdatum H-3223
  - Grafik H-3226
  - manuell H-3059
  - nachholen H-3066
  - pro Position H-3224
  - Produktionslauf H-3227
  - Restmengen H-3295
  - Rückmeldungen H-3048
  - stückweise H-3224
  - Übersicht H-3223
  - Übersicht Rückmeldungen H-3252
- Fertigung
  - Angebotsoptimierung A-46
  - Anwenderstatus prüfen E-2390
  - Bruchgründe B-1014
  - Materialübersicht A-45
  - Produktverwaltung B-711
  - Reservierungsauftrag A-46
  - Routenoptimierung A-50
  - Statuszuordnung prüfen E-2391
  - Übersicht A-43
  - Übersicht erstellen E-2416
- Fertigungsstand
  - Auftrag H-3240, H-3244
  - Berechnung H-3244
  - Bestellteile H-3249
  - Positionen H-3245
  - prüfen H-3064
  - Stückliste H-3247
  - Übersicht Rückmeldungen H-3252
- Fertigungsstand Auftrag
  - Navigation durch die Register H-3240
- Fertigungsstraße H-3181
  - definieren H-3008
- Fertigungsübersicht siehe Terminübersicht
- Fertigungsvorschau
- Funktionsprinzip E-2456
- Geschäftsarten E-2582
- Spaltendefinition E-2581
- Festpreis
- für gesamte Position C-1414
- für gesamten Auftrag C-1412
- für mehrere Positionen C-1412
- in Position C-1412
- pro Stück festlegen C-1414
- FiBu
- auswählen B-1062
- Buchungskreis B-1062
- Datenbank B-1065
- Datenübergabe C-1617
- Firmendaten B-1061
- Nummernkreise B-1032
- OP-Meldung C-1622
- Rechnung übergeben C-1623
- Tagesabschluss C-1618
- Übergabe B-440
- Übergabedatei C-1619
- FiBu-Server B-1065
- FiBu-Übergabe
- Auftrag, Gutschrift C-1967
- Einstellungen C-1972
- Menü Funktionen C-1968
- Menü Optionen C-1968
- Verkauf - Sollstellung C-1970
- Verkauf, Einkauf C-1970
- Filiale
- Bankverbindung anlegen B-445
- eigenständige Filiale B-890
- Export Superstatistik B-1105
- Kundenverwaltung B-924
- Mandant B-1169
- Replikation aktiv B-1118
- zum Kunden anlegen B-124
- Finanzamt B-1058
- Finanzbuchhaltung siehe FiBu
- Firma
- Bankverbindung anlegen B-445
- Kunde B-890
- Mitarbeiter B-454
- Mitarbeiter anlegen B-461
- Nummer B-1056
- Firmendaten
- Archiv B-1104
- Archivierung B-440, B-441
- AV-Bereich B-510
- BMECat-Import B-1145
- Druck B-1122
- Einstellung für dateilose Rückmeldung E-2368
- Einstellungen G-2706, K-3323
- Einstellungen für Kapazitätsplanung H-3010
- Einstellungen für Wareneingang D-2160
- EK-Berechnung aktivieren G-2732
- E-Mail-Versandart B-1067
- Erfassungsstelle für Fertigmeldung E-2360
- Erlöskonten C-1620
- FiBu B-440, B-1061
- Filiale B-442
- Kalkulation (Gemeinkosten) B-1120
- Kapa-Planung B-1138
- Lager/EK/EDI B-1096
- Lagerführungsmodus aktivieren G-2708, K-3325
- Mandant B-442, B-1056
- OP-Meldung B-440
- Outlook-Koppelung B-1145
- Parameter B-1073
- Preisberechnung B-1085
- Produktion B-1126
- Referenzen D-2195
- Statistik B-442
- Steuer B-1058
- Steuer, Finanzamt B-1058
- Superstatistik B-1105
- System B-1113
- Systemeinstellungen B-440
- Tagesabschluss B-442, B-1111
- Versand B-1134
- virtuelle Positionsnummer D-2081, D-2170
- Währungen B-157, B-530
- Firmenmitarbeiter siehe Mitarbeiter
- Fixierter Artikel C-1326
- Fixierter Preis C-1400
- Flächen-Emaillierung C-1754
- Flächenkapazität
- pro Wochentag hinterlegen B-1121
- Folge-Aggregate
- überspringen H-3178
- Folgeauftrag B-1127
- Folgebearbeitung H-3161, H-3167
- Folgedokument C-1281
- Folgeschlüssel B-283
- Forderung B-968
- Historie B-969, C-1997
- Forderung, Forderungsberechnung C-1995
- Forderungsrechnung
- zu Rahmenauftrag erstellen B-588
- Format
- Datum, Zeit B-1114
- Formel
- für Workflow-Task zum Einlasten H-3028
- Formular
- Auftragsformulare B-557
- Direktdruck B-1213
- Druckauftrag B-558
- drucken C-1463
- Druckvorlagen B-546
- Formularverwaltung B-1196
- Formular-/Etikettendruck C-1923
- drucken C-1463
- Etiketten drucken C-1465
- Gruppe Druckmodi C-1925
- Menü Funktionen C-1923
- Menü Optionen C-1924
- Formulardruck
- Druckformate B-549
- Übertragungspool C-1935
- Formulardruck (Dokumente) C-1927
- Formularverwaltung
- Dialog B-1195
- Druckoptionen B-1201
- Druckpunkt B-546
- Einstellung für Preisdruck B-550
- Formular B-1196
- Kopf-/Fußtexte B-1199
- nicht zu druckende Texte B-1200
- Zuordnung B-547
- Frachtkosten
- anzeigen E-2438
- Berechnung E-2435
- Einstellungen für kalkulatorische Frachtkosten E-2436
- kritische Grenze festlegen B-1136
- Pauschale in Tour E-2380
- Speditionskosten E-2440
- Franz.Preisberechnung
- Einstellungen B-1094
- Fremdartikel
- EDI-Daten kopieren B-1245
- Gas B-1247
- Produkte B-1237
- SZR B-1246
- Fremddokumente (Import Dokumente) C-1980
- Fremddokumentenverwaltung
- Dokument C-1980
- Fremdschlüssel B-710
- Grenzty B-681
- Warengruppe B-331
- Fremdschnittstelle
- Export (EDI) D-2229
- Übertragungs-Pool D-2233
- Fremdwährung B-157, B-530, B-1059
- Beispiel B-158, B-531
- Berechnung aus Stückpreis B-1089
- Funktion freigeschaltet H-2920
- Funktionen
- Kiste auflösen Y-3446
- Kistenbuchungen Y-3444
- Kisteninhalt ändern Y-3445
- Kistenort ändern Y-3447
- Kistenwarenausgang Y-3449
- Lagerentnahme Y-3440
- Lagerumbuchungen Y-3442
- Lagerzugang Y-3441
- Lagerbewertung
- Berechnungsbeispiele G-2907
- Bewertung G-2911
- Inventur G-2845
- Selection G-2909
- Lagerbuchung
- Ab- und Zugang G-2755
- Ab-/Zugang manuell buchen G-2756, G-2759, K-3368
- Anwenderstatus G-2710, K-3326
- bei Stückliste G-2737
- Bestand manuell ändern K-3367
- Buchungsart G-2754
- Buchungsart auswählen G-2721
- Erfassungsstelle G-2815, K-3323, K-3356
- Journal anzeigen G-2765
- Journal erstellen G-2765
- Kiste K-3354
- Kiste auflösen K-3372
- Kisteninhalt korrigieren K-3371
- kombinierte Lagerführung G-2716
- Lagerort ändern G-2760, K-3370
- manuell G-2754, G-2755
- reservierte Lagerartikel drucken G-2767
- Statistik anzeigen G-2769
- Statuszuordnung G-2711
- Lagerbuchungsart G-2715
- Lagerdefinition B-865
- Lagerebenen B-866
- Lagerentnahme Y-3440
- Lagerführung
- auf Stücklisten-Ebene G-2737
- kombiniert G-2716
- Lagerkennzeichen G-2715
- Lagerort G-2692
- Parameter für Produkt B-727
- Stückliste einrichten G-2740
- Lagerführungsmodus G-2705, K-3317
- EK-Ermittlung G-2728
- in Firmendaten aktivieren G-2708, K-3325
- Lagerhistorie G-2884
- Auswahl G-2885
- Tabelle G-2888
- Lagerinfo A-61
- Dokumentenübersicht C-2039
- Lagersuche C-2035
- zukünftiger Lagerbestand C-2038
- Lagerkategorien B-867
- Lagerkennzeichen G-2715
- Lagermaß
- in Stammdaten anlegen B-270, D-2061, G-2723, K-3330
- Lagerartikel B-270, D-2061, G-2718, G-2723, K-3330
- Produktverwaltung G-2717, K-3318
- Stammdaten, Lagerverwaltung G-2718
- Lagermaße
- für Preisfindung B-753
- Lagerort
- Artikel umbuchen G-2760, K-3370
- Bestand G-2692
- Suche Aggregate B-869
- Lagerort für Aggregate B-868
- Lagerstatistik G-2889
- Produkte G-2890
- Statistik G-2892, G-2894
- Lagersuche C-2034
- Dokumentenübersicht C-2039
- Lagersuche (Register in Lagerinfo) C-2035
- Lagerumbuchung Y-3442
- Lagerverwaltung A-60, G-2863, K-3379
- Grundgedanken G-2691, K-3317
- Handlungsablauf G-2692
- Lagerartikel G-2863, K-3380
- Lagerartikel anlegen G-2749, K-3331
- Lagerbestellung manuell erfassen G-2803
- Lager-Hauptartikel G-2745
- Preise G-2868, K-3384
- Preisentwicklung G-2747
- Stücklisten-Kiste K-3340
- Zusatz G-2871, K-3387
- Lagervorschau B-1101
- Lagerwert
- EK-Bewertung G-2727
- Lagerwirtschaft G-2842, K-3377
- Buchungsjournal A-62, G-2764
- EK-Berechnung aktivieren G-2732
- Historie A-62, G-2764
- Lagerwert A-62, G-2764
- Menü-Übersicht G-2689, K-3316
- Statistik A-62, G-2764
- Lagerzugang G-2874, K-3390, Y-3441
- durch Produktionsauftrag G-2815, K-3323, K-3356
- Landeskürzel B-671
- Landeswährung B-1059
- Lastkraftwagen B-998
- Lauf
- Einstellung für manuelle Fertigmeldung H-3229
- fertig melden H-3227
- Leistung
- in Position erfassen C-1386
- in Position löschen C-1388
- Leistungserfassung (Register in Positionserfassung) C-1780
- Leistungsmerkmale A-23
- Leitstand
- Aggregat (Dialog) H-3279
- Aggregat (Register) H-3264
- Arbeitsarten H-3271
- Auftrag (Dialog) H-3296
- Auftrag umlasten H-3267
- Aufträge (Register) H-3265
- Auslastung pro Schicht H-3275
- Bestellteile H-3278
- Einstellungen H-3293
- mit dem Leitstand arbeiten H-3078
- Navigation durch die Register H-3262
- Position umlasten H-3269
- Produktionsbereiche H-3263
- Vorprozesse prüfen H-3276
- Leitstand Aggregat
- Auslastung H-3285
- Auslastung der Schichten H-3281
- Belegung H-3283
- mit dem Leitstand arbeiten H-3081
- Leitstand Auftrag
- Aggregate H-3298
- Arbeitsarten H-3302
- Auslastung H-3308
- Bestellteile H-3304
- mit dem Leitstand arbeiten H-3080
- Navigation durch die Register H-3296
- verschieben H-3300, H-3306
- Letzte Änderung F-2648
- Lieferant B-986
- AB erfassen D-2123
- für Auftragsposition D-2086
- im Bestellpool ändern D-2106
- in Bestellposition ändern D-2090
- in Bestellung ändern C-1568, G-2787
- Katalog B-985
- Lieferung anmahnen D-2131
- Parameter B-947
- Preis in AB prüfen D-2127
- Preisberechnung bei Bestellartikel B-1086
- Preise vergleichen D-2108
- Preisvergleich D-2099
- Produktverwaltung B-732
- Rabatt B-414
- Rabatte B-934
- Rundungszuordnungen B-970
- Sammel-AB erfassen D-2129
- siehe auch Partner
- Stammdaten D-2065
- Vorlauftage B-1115
- Lieferant / Name / Lieferantenobjekt (AE) C-1702
- Lieferant und Liefertermin ändern (Dialog) C-1949
- Lieferanten
- Gruppen B-875
- Lieferanten mahnen D-2262
- Lieferantengruppen
- Rundungszuordnungen B-971
- Lieferantenkartei B-192, B-987, D-2065, K-3318
- interner Kunde G-2809, K-3348
- Produktionsauftrag G-2809, K-3348
- Standard-Lieferant D-2067
- Lieferantenkartei prüfen D-2067
- Lieferantennachweis B-993
- Lieferantenobjekte B-952
- Lieferantenrabatte B-934
- Lieferantenrechnung
- importierte Rechnung prüfen D-2204
- Kontrolle D-2282
- prüfen D-2180
- Lieferbedingung
- Kommissionierung E-2529
- Lieferbedingungen B-994
- Lieferdatum
- einlasten in Kapazitätsplanung H-3203
- verschieben beim Einlasten H-3203
- Lieferdauer
- Beispiel B-183, C-1300
- Berechnung B-183, C-1300
- Kunde B-951
- Lieferant B-951
- Lieferschein
- drucken C-1463
- Liefertermin
- AB Lieferant D-2240
- ändern C-1583, C-1863, D-2136, D-2139
- bei Engpass H-3034
- Benachrichtigung C-1585
- Bestellung D-2121
- im Bestellpool ändern D-2106
- in mehreren Dokumenten ändern D-2142
- in Tourenliste ändern E-2384
- Kapazitäten anzeigen E-2421
- Kontrolle und Korrektur D-2135
- Kunden benachrichtigen D-2136
- manuell wählen H-3203
- prüfen C-1583, D-2139
- Liefertermin nach Touren suchen (AE) C-1684
- Lieferterminbestimmung C-1862
- Lieferterminkontrolle C-1848
- Liefertreue F-2667
- Lieferung
- buchen D-2161
- erfassen C-1521
- Lieferanschrift C-1298
- Lieferdaten C-1581
- Lieferschein C-1298
- Lkw E-2528
- Teilmenge D-2272, K-3415
- Terminkontrolle C-1582, C-1848
- Wareneingang D-2155
- Wareneingang mit AB D-2236
- Liste
- Beispiel Transportmittelbelegung E-2534
- drucken E-2408
- Empfangsbestätigung E-2533
- Gestellausgabe E-2536
- Gestellbelegung E-2533
- Kommissionierung E-2533
- Nummer zurücksetzen (Zollverwaltung) E-2587
- Tourenliste drucken E-2386
- Tourenliste zusammenstellen E-2382
- Transportmittel E-2533
- Zollverwaltung E-2583
- Lkw B-998
- anlegen E-2402
- Kommissionierung E-2528
- Lochbohrung C-1747
- Login
- A+W Business B-1116
- Logo C-1757
- Logoposition B-972
- Lohnkosten
- Aggregate H-3118
- Lohnnebenkosten B-1120
- Löschen
- Dokument C-1307
- Position C-1392
- Stücklisten-Komponente in Position C-1391
- Systemlogbuch B-1112

### M
- Mahnsperre
- Kundenverwaltung B-907
- Mahnstufe
- setzen C-1475
- Mahntext B-1192
- Partnerverwaltung B-907
- Mahnung C-1467
- erfassen C-1475
- für Gestelle zurücksetzen E-2560
- Gestell E-2551
- Lieferung D-2131
- Mahnstufen C-2028
- Mahnwesen C-2026
- offene Posten C-2029
- Makro C-1418
- ändern C-1423, C-1909
- kopieren C-1912
- löschen C-1428
- Position erfassen C-1422
- sichern C-1908
- speichern C-1420
- suchen C-1911
- Makro kopieren C-1426
- Makros C-1908
- Mandant B-442
- anlegen B-444
- Bankverbindung B-151
- Filiale B-442, B-1169
- Firmendaten B-1056
- Matchcode B-1056
- Nummer B-1056
- Mannstunde H-2951
- Manuell
- Auftrag fertig melden H-3230
- Einstellung für Fertigmeldung H-3234
- Referenzpreis B-1092
- Manuell einlasten
- Aggregat wählen H-3212
- Auftrag H-3207
- Ergebnis H-3209
- Position splitten H-3215
- Zeiten prüfen H-3217
- Manuelle Packmittelzuordnung
- Gestellauswahl E-2524
- Statusmeldung E-2522
- Markierungsoptionen (Bestellübergabe) C-1950
- Marktpartner
- abweichende Gruppen B-105
- anlegen B-110
- Auftrags-, Bestellparameter B-182
- Datenaustausch B-1249
- Fälligkeit B-143
- Gruppen B-103
- Kreditlimit B-156
- Kreditlimit-Snapshot B-156
- Monatsrechnung B-117
- Objekt B-185
- Partnerverwaltung B-98
- Teilliferierung B-117
- zulassen (Partnerverwaltung) B-897
- Teilrechnung E-2601
- aus elektr. Dokument erstellen D-2206
- Datum B-1074
- Dokument C-1517
- erfassen C-1521
- Faktura C-1520
- öffnen C-1526
- Position löschen B-1074
- Sperrkennzeichen B-1034, B-1067
- Wareneingang D-2157
- Wareneingang erfassen D-2164
- zulassen (Partnerverwaltung) B-897
- Teillieferungen
- Dokumentenverwaltung C-1901
- pro Fertigmeldung/Wareneingang C-1902
- pro Gestell C-1905
- Teillieferungsübersicht C-1519, C-1841
- Teilrechnung C-1287, C-1520
- drucken C-1463
- Template
- für Position übernehmen C-1437
- Modell C-1431
- Template Editor B-769
- Termin
- Berechnungsbeispiel H-3024
- Modus für Terminsuche H-3201
- Produktionstermin ändern H-3256, H-3258
- Terminberechnung
- Beispiel Übergangszeiten + Verweiltage H-3026
- Beispiel Übergangzeiten H-3027
- Beispiel Verweiltage H-3025
- Rückwärtsterminierung A-55, H-3024
- Vorwärtsterminierung A-55, H-3024
- Termine
- Änderung an den Kunden senden C-1851
- Änderung in mehreren Dokumenten C-1587
- Auftrag C-1690
- Dokument C-1299
- im Bestellpool ändern C-1568