---
title: "DE_AWBusiness_Kistenmanagement_1_3"
source: "DE_AWBusiness_Kistenmanagement_1_3.pdf"
tags: ["Kistenmanagement", "Wareneingang", "Warenausgang", "Lagerverwaltung", "Identnummer", "Bestellung", "A+W Business", "ERP", "Glasindustrie", "Software-Referenz"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for the A+W Business Crate Management module. It details the processes for handling stock orders, goods receipt (Wareneingang), and goods issue (Warenausgang) for crates, including the assignment and tracking of unique identification numbers (IDs)."
long_description: "This comprehensive software reference guide provides detailed instructions on using the A+W Business Crate Management module. It covers the entire lifecycle of crate handling within the system, starting with stock orders and moving through goods receipt and goods issue. The guide explains how to configure number ranges and assign orders to specific mandates or work areas. The core of the document focuses on the 'Goods Receipt (Crates)' process, broken down into several tabs: 'Selection' for filtering orders, 'Complete' for booking in full deliveries, 'By Position' for handling partial deliveries and discrepancies, and 'ID Number' for assigning unique system-generated IDs to individual crates. It also covers the settings for configuring these ID formats and logging their creation. The final section describes the 'Goods Issue Crates' process for booking crates out of inventory. This guide is intended for users responsible for inventory, logistics, and purchasing within the glass, window, and door industries."
---

---
## Softwarereferenz Lagerbestellung

### Name
Name des Nummernverwalters, in den die Bestellungen übergeben werden sollen. Wenn Sie einen neuen Namen eintragen, wird ein neuer Nummernverwalter angelegt.

### Ziel-Nummernkreis

**Mandant**: Wenn Sie für Ihre Mandanten gesonderte Nummernkreise eingerichtet haben, können Sie den gewünschten Mandanten auswählen.

**AV-Bereich**: Wenn Sie mit AV-Bereichen arbeiten, können Sie die Bestellung einem bestimmten AV-Bereich zuordnen.

## Kisten – Ein- und Ausgang

Vollständige Beschreibungen von Wareneingang und Warenausgang finden Sie in den Parts Fertigung und Einkauf.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Wareneingang (Kisten)" auf Seite K-102
- "Einstellungen (ID)" auf Seite K-113
- "Warenausgang Kisten" auf Seite K-114

### Wareneingang (Kisten)

**Pfad:** `Dokumente > Bestellung > Wareneingang > Wareneingang`

In diesem Dialog können Sie den Wareneingang zu einzelnen Bestellungen oder zu den Bestellungen in einem Nummernverwalter erfassen.

Für die jeweilige Bestandsbuchung können Sie Vorgaben für die Identifikationsnummern (ID) festlegen, die automatisch vergeben wird, wenn in der Lagerbestellung Positionen mit einer Menge größer als 1 erfasst sind. Die Identnummern werden für Kisten und Gläser (Lagerplatten) vergeben.

> **Voraussetzung**
> In den Firmendaten muss die Checkbox für die virtuelle Vergabe von Positionsnummern markiert sein.
> ⇨ "Firmendaten" auf Seite K-18

In diesem Dialog finden Sie folgende Register:
- "Wareneingang – Auswahl" auf Seite K-103
- "Wareneingang - Komplett" auf Seite K-105
- "Wareneingang – Positionsweise" auf Seite K-107
- "Wareneingang – Identnummer" auf Seite K-110
- "Wareneingang – Protokoll (Identnummern)" auf Seite K-112

### Wareneingang – Auswahl

**Pfad:** `Dokumente > Bestellung > Wareneingang > Wareneingang > Register Auswahl`

In diesem Register können Sie die Auswahl und Anzeige der Dokumente filtern, zu denen Sie Wareneingänge prüfen und/oder erfassen möchten.

> ⇨ Tutorial, "Wareneingang" auf Seite D-120

#### Auswahl
Mit der Wahl der Option legen Sie fest, wie die Bestellungen gefiltert werden. Die offenen Bestellungen werden nach der Suche im Register Komplett angezeigt, damit die Wareneingänge verbucht werden können.

- **Nach Bestellnummer:** Das Eingabefeld für die Bestellnummer wird freigeschaltet. Im Register Komplett werden die gesuchte Bestellung und alle referenzierten Aufträge angezeigt.
- **Nach Auftragsnummer:** Das Eingabefeld für die Auftragsnummer wird freigeschaltet. Im Register Komplett werden alle Bestellungen angezeigt, die zur eingetragenen Auftragsnummer erzeugt wurden.
- **Nach Lieferanten:** Das Eingabefeld für die Lieferantennummer wird freigeschaltet. Im Register Komplett werden alle Bestellungen beim gewählten Lieferanten angezeigt.
- **Nach Lieferscheinnummer / Lieferavis, Gesamtliefermenge:** Das Eingabefeld für die Nummer des Lieferscheins oder des Lieferavis und das Feld für die Gesamtmenge werden freigeschaltet. Wurde ein Lieferavis importiert, müssen die tatsächlich gelieferten Mengen eingetragen werden.
- **Nach Anliefertermin des Lieferanten:** Das Eingabefeld für den Liefertermin wird freigeschaltet. Im Register Komplett werden alle Bestellungen angezeigt, die zum gewählten Termin angeliefert werden sollen.
- **Nach Nummernverwalter:** Die Kombobox zur Auswahl des Nummernverwalters wird freigeschaltet. Im Register Komplett werden alle Bestellungen im gewählten Nummernverwalter angezeigt.
- **Nach Scanner / Dokument:** Die Felder für den Barcode der Bestellnummer oder einer Bestellposition werden freigeschaltet.

#### Ziel-Nummernverwalter
Die Lagerbestellungen können nach dem Buchen des Wareneingangs automatisch in einen anderen Nummernverwalter gestellt werden.
- **(Checkbox nicht aktiv):** Die Lagerbestellungen werden nicht in einen anderen Nummernverwalter gestellt.
- **(Checkbox aktiv):** Die Felder im Bereich Ziel-Nummernverwalter werden freigeschaltet. Die Lagerbestellungen werden in den gewählten Nummernverwalter gestellt.

**Mitarbeiter**: Name des Mitarbeiters, dem der Ziel-Nummernverwalter zugeordnet ist.

**Nummernverwalter**: Nummernverwalter, in den die Lagerbestellungen mit (vollständigen) Wareneingängen gestellt werden sollen.

### Wareneingang – Komplett

**Pfad:** `Dokumente > Bestellung > Wareneingang > Wareneingang > Register Komplett`

In diesem Register werden alle Bestellungen angezeigt, die den Suchkriterien entsprechen. Wenn Sie eine Bestellung markieren, werden die referenzierten Aufträge aufgelistet.

> ⇨ Tutorial, "Wareneingang erfassen" auf Seite D-127

#### Liefertermin

**Anliefertermin des Lieferanten**: Anzeige des aktuellen Tagesdatums. Sie können es überschreiben, wenn Sie eine Lieferung erfassen wollen, die vor diesem Datum eingetroffen ist. Das Datum wird nur für die Dokumente übernommen, die in der Übersicht markiert sind.

**AB-Lieferant**: Sie können zu einem Wareneingang auch die Nummer der Auftragsbestätigung durch den Lieferanten erfassen.

#### Dokumente
Mit den Schaltflächen können Sie alle oder einige Dokumente markieren oder die Markierung entfernen.
In der Übersicht werden alle Bestellungen angezeigt, die den Suchkriterien im Register Auswahl entsprechen. Der vollständige Wareneingang wird für die Dokumente erfasst, bei denen die Checkbox komplett buchen markiert ist.

- **Bestell-Nr.:** Nummer der Bestellung.
- **Komplett buchen:** Eine Bestellung kann als komplett gebucht werden, wenn alle Positionen vollständig geliefert wurden.
    - **(Checkbox nicht aktiv):** Der Wareneingang ist nicht vollständig. Es stehen noch Lieferungen aus.
    - **(Checkbox aktiv):** Der Wareneingang ist vollständig und die Bestellung soll als komplett verbucht werden.
- **Status:** Aktueller Status. Der Status wird nach der Erfassung des Wareneingangs umgesetzt.
- **Lieferant:** Nummer und Name des Lieferanten.
- **Anlief.-Term. d. Lieferant:** Anliefertermin des Lieferanten. Der Termin wird aus der Bestellung oder der AB übernommen. Wenn Sie den Wareneingang erfasst haben, wird der Termin auf das aktuelle Tagesdatum oder das von Ihnen gewählte Datum umgesetzt.
- **Enthält Kisten:** Anzeige der Bestellungen, in denen Kisten enthalten sind. Die Markierung der Checkbox kann nicht geändert werden.

#### Zugehörige Aufträge
In der Übersicht werden nur die referenzierten Aufträge angezeigt, die zu der ausgewählten Bestellung gehören. Wenn mehrere Bestellungen ausgewählt sind, bleibt die Liste leer.

**Anliefertermin bei Kunde**: Das Datum wird aus dem referenzierten Auftrag übernommen. Sie können es überschreiben, wenn der ursprüngliche Termin nicht eingehalten werden kann.

### Wareneingang – Positionsweise

**Pfad:** `Dokumente > Bestellung > Wareneingang > Wareneingang Kiste > Register Positionsweise`

In diesem Register können Sie Wareneingänge positionsweise für eine Bestellung erfassen, die im Register Komplett ausgewählt wurde.

#### Warenein-/ausgang

**Menge Eingang**: Menge, die für die markierte Position geliefert wurde.

**Menge bestellt, Bereits geliefert, Menge avisiert**: In diesen Feldern werden die entsprechenden Mengen für die markierte Position angezeigt. Die Felder werden nach der Erfassung aktualisiert.

**Lagerort**: Zur markierten Position können Sie einen Lagerort auswählen, an dem der Lagerartikel verbucht werden soll. Beachten Sie dabei, dass Lagerartikel auch auf den Lagerort `<k.A.>` gebucht werden können. Der Lagerort aus der Bestellung kann über das Menü Optionen vorgeblendet werden.

**Über-/Unterlieferung akzeptieren**: Die Stückzahl der Lieferung kann sich von der Bestellung unterscheiden. Sie können die abweichenden Stückzahlen akzeptieren und damit die Lieferung für die Position als komplett erfassen.
- **(Checkbox nicht aktiv):** Über- oder Untermengen werden nicht akzeptiert.
- **(Checkbox aktiv):** Die eingegebene Stückzahl wird akzeptiert und die Position wird als komplett gebucht. Wenn ein Lagerartikel geliefert wurde, wird der Lagerbestand der gelieferten Menge entsprechend aktualisiert. Die geänderte Menge wird in die Bestellung zurückgeschrieben.

#### Bestätigung

**AB-Lieferant**: Nummer der Auftragsbestätigung des Lieferanten für die markierte Position.

**AB-Liefertermin**: Liefertermin für die Position.

#### Positionen
In der Übersicht werden die Positionen der gewählten Bestellung angezeigt.

- **Pos:** Nummer der Bestellposition.
- **Komplett buchen:** Eine Position kann als komplett gebucht werden, wenn die gesamte Stückzahl geliefert wurde.
    - **(Checkbox nicht aktiv):** Der Wareneingang ist nicht vollständig.
    - **(Checkbox aktiv):** Die Position soll als komplett verbucht werden.
- **Auftr.Nr.:** Auftragsnummer.
- **Artikel:** Bezeichnung des bestellten Produkts.
- **Farbe:** (Farb-) Varianten, die zu dem bestellten Produkt erfasst sind.
- **Breite/Höhe:** Maße der bestellten Position.
- **Bestellt:** Stückzahl der Bestellung für diese Position.
- **Avisiert:** Avisierte Stückzahl der Position.
- **Geliefert:** Menge, die für diese Position bereits geliefert wurde. Bei Teillieferungen ist dies die Summe der Stückzahlen, die bisher zu dieser Bestellung geliefert wurden.
- **Eingang:** Menge, die für die markierte Position geliefert wurde.
- **Akzeptieren:** Wenn die Stückzahl der Lieferung höher oder niedriger ist als die der Bestellung, kann diese Stückzahl übernommen werden. Die nicht bestellten Scheiben werden im Lager nur verbucht, wenn es Lagerartikel sind, die in einer Lagerbestellung bestellt wurden. Wenn die Bestellung aus einem Auftrag erzeugt worden ist, werden die Lagerbestände nicht aktualisiert.
    - **(Checkbox nicht aktiv):** Die Liefermenge entspricht der Bestellung und braucht nicht gesondert gekennzeichnet zu werden.
    - **(Checkbox aktiv):** Die Lieferung ist größer oder kleiner als die Bestellung und wird akzeptiert. Die gelieferte Stückzahl wird in die Bestellung zurückgeschrieben. Der referenzierte Auftrag wird nicht geändert. Die überzähligen Scheiben können ggf. als Bestand verbucht werden.
- **Enthält Kisten:** Anzeige der Bestellungen, in denen Kisten enthalten sind. Die Markierung der Checkbox kann nicht geändert werden.
- **AB-Lieferant:** Nummer der Auftragsbestätigung des Lieferanten.
- **AB-Liefertermin:** Liefertermin aus der Auftragsbestätigung des Lieferanten.
- **Lagerort:** Standard-Lagerort des Lagerartikels. Beachten Sie dabei, dass Lagerartikel auch auf den Lagerort `<k.A.>` gebucht werden können.
- **Artikelbezeichnung 2 + 3:** Bezeichnungen des bestellten Produkts, die in den Stammdaten hinterlegt sind. Bei Float-Glas ist in der Regel nur die Bezeichnung 1 hinterlegt, die in der Spalte Artikel angezeigt wird.

#### Zugehörige Aufträge
In der Übersicht werden die referenzierten Aufträge zu den Positionen angezeigt. Die Felder sind zum Register Komplett beschrieben.
> ⇨ "Wareneingang - Komplett" auf Seite K-105

### Wareneingang - Identnummer

**Pfad:** `Dokumente > Bestellung > Wareneingang > Wareneingang > Register Identnummer`

In diesem Register werden die Positionen einer Bestellung mit Kisten angezeigt. Dabei wird für jede Kiste einer Bestellposition eine Unterposition (virtuelle Positionsnummer) erzeugt, der eine Kiste mit einer eigenen Identnummer (Identifikationsnummer, ID) zugewiesen werden kann. Die Vorgabe für die ID können Sie festlegen.

> ⇨ "Einstellungen (ID)" auf Seite K-113

> **Voraussetzung**
> In den Firmendaten muss die Checkbox für die Vergabe von virtuellen Positionsnummern markiert sein.
> ⇨ Stammdaten, "Virtuelle Positionsnummern verwenden" auf Seite B-943

#### Kistendaten

**Lieferanten-Identnummer**: Die Kisten-ID, die der Lieferant für diese Position der Lieferung vergeben hat. Wenn die Nummer eingegeben ist, wird im Feld Identnummer die automatische Kisten-ID angezeigt.

**Identnummer**: Die automatische Kisten-ID wird angezeigt, sobald Sie die Lieferanten-ID eingetragen haben. Für jede Kiste einer Bestellposition wird beim Erfassen des Wareneingangs eine eigene Kisten-ID erzeugt. Wenn z. B. 5 Kisten mit Float 5 à 1200 x 800 mm bestellt und geliefert wurden, werden die IDs XXXX00001, XXXX00002, ..., XXXX00005 vergeben. Die Vorgabe für XXXX können Sie selbst bestimmen.
> ⇨ "Einstellungen (ID)" auf Seite K-113

**Lagerort**: Sie können jeder Position einen eigenen Lagerort zuweisen. Beachten Sie dabei, dass Sie auch den Lagerort `<k.A.>` zuweisen können.

**Bemerkung**: Bei Besonderheiten, z. B. in der Zuweisung des Lagerortes oder bei Reservierungen, können Sie eine Anmerkung eintragen.

**Inhalt**: Inhalt der Kiste, die in der Übersicht markiert ist. Der Wert kann ggf. geändert werden.

**Prod. Datum**: Datum, bis zu dem die Produktion mit der bestellten Lieferung abgeschlossen sein sollte. Dieses Datum ist für die Lagerentnahme nach dem FiFo-Prinzip wichtig, z. B. für beschichtetes Glas.

**EK / ME**: Einkaufspreis und Preiseinheit der bestellten Position. Wenn Sie den Preis ändern, wird die Änderung in die Bestellung zurückgeschrieben.

#### Kistenpositionen

- **Pos:** Positionsnummer aus der Bestellung. Eine Positionsunternummer wird beim Buchen automatisch dann vergeben, wenn die Stückzahl der Bestellposition größer als 1 ist, z. B. 1.1, 1.2 usw.
- **Bezeichnung:** Bezeichnung aus der Bestellung.
- **Breite / Höhe:** Lagermaße der Scheiben in der Kiste.
- **Lieferanten-Identnummer:** Kisten-ID des Lieferanten wie im Bereich Kistendaten eingetragen.
- **Inhalt:** Kisteninhalten wie im Bereich Kistendaten eingetragen.
- **Identnummer:** (Automatische) ID wie im Bereich Kistendaten eingetragen.
- **Lagerort:** Lagerort wie im Bereich Kistendaten eingetragen.
- **Prod. Datum:** Produktionsdatum wie im Bereich Kistendaten eingetragen.
- **Pr./ME:** EK-Preis pro Mengeneinheit wie im Bereich Kistendaten eingetragen.
- **Pr. Einh.:** Preiseinheit für den angezeigten Preis.

### Wareneingang – Protokoll (Identnummern)

**Pfad:** `Dokumente > Bestellung > Wareneingang > Wareneingang > Register Protokoll (Identnummern)`

In diesem Register können Sie sich einen Überblick über die vergebenen Kisten-IDs verschaffen.

### Einstellungen (ID)

**Pfad:** `Dokumente > Bestellung > Wareneingang > Wareneingang > Menü Optionen > Gruppe Identnummernvergabe > Einstellungen`

In diesem Dialog legen Sie die Vorgabe für die Identifikationsnummern (ID) für Kisten fest. Diese Einstellung ist notwendig, um eigene Kisten-IDs automatisch zu vergeben.

Wenn in einer Lieferung z. B. eine Position mit 5 Kisten aufgeführt ist, werden beim Erfassen des Wareneingangs 5 (virtuelle) Unternummern vergeben. Diese Nummern müssen Sie mit einem Kennzeichen versehen, so dass z. B. statt der gescannten Kistennummer 12345 die Unternummern LieferantA00001, LieferantA00002, ..., LieferantA00005 vergeben werden.

> ⇨ Tutorial, "Kistengeschäft" auf Seite D-136

> **Voraussetzung**
> In den Firmendaten muss die Checkbox für die virtuelle Vergabe von Positionsnummern markiert sein.
> ⇨ Stammdaten, "Virtuelle Positionsnummern verwenden" auf Seite B-943

#### Lageridentnummer

**Vorgabe**: Sie können einen Text (oder Zahlen) mit max. 15 Zeichen eingeben, der durch XXXXX ergänzt wird. XXXXX steht für die automatisch vergebene Nummer. Der Text wird so lange beibehalten, bis Sie ihn ändern.
Wenn Sie von unterschiedlichen Lieferanten Kisten beziehen und diese getrennt kennzeichnen möchten, müssen Sie vor dem Erfassen des Wareneingangs die Vorgabe jeweils entsprechend anpassen.

### Warenausgang Kisten

**Pfad:** `Fertigung > Lieferwesen > Warenausgang Kisten > Register Identnummern`

In diesem Register können Sie eine Kiste reservieren oder aus dem Lagerbestand ausbuchen. Sie können nur Kisten reservieren, die beim Lagereingang mit einer Kisten-ID erfasst wurden.

> ⇨ Tutorial, "Warenausgang Kisten" auf Seite E-148
