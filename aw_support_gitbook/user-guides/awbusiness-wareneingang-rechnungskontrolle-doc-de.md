---
title: "D-AWBusiness-HB_23"
source: "D-AWBusiness-HB_23.pdf"
tags: ["A+W Business", "Wareneingang", "Rechnungskontrolle", "Produktionsübergabe", "Kapazitätsplanung", "ERP", "Software", "Einkauf", "Fertigung", "Goods Receipt", "Invoice Verification"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical software reference guide for the A+W Business Einkauf (Purchasing) and Fertigung (Manufacturing) modules. It details procedures for goods receipt, handling over/under deliveries, invoice verification (both manual and electronic), and handing over orders to production, including capacity planning and feedback mechanisms."
long_description: "This document serves as a comprehensive software reference for the A+W Business system, specifically focusing on the 'Einkauf' (Purchasing) and 'Fertigung' (Manufacturing) modules. It is intended for end-users and administrators of the A+W Business software. The 'Wareneingang' (Goods Receipt) section explains how to process incoming deliveries, accept or reject quantity discrepancies, manage stock levels, and handle items linked to specific customer orders. It also covers the management of items in crates using unique identification numbers (`Identnummer`). The 'Rechnung' (Invoice) section details the `Rechnungskontrolle` (Invoice Verification) process, allowing users to check and approve supplier invoices before passing them to accounting. This includes both manual and `Elektronische Rechnungskontrolle` (Electronic Invoice Verification) via document import. The 'Fertigung' (Manufacturing) part of the manual outlines the `Produktionsübergabe` (Production Handover) process, describing how orders are transferred from the business system to the production environment (e.g., A+W Production). It explains various handover scenarios, such as with or without `Kapazitätsplanung` (Capacity Planning), and using tools like the A+W Production Capacity Planner. The document also covers handling feedback from production (`Rückmeldungen aus der Produktion`), managing delivery processes (`Lieferwesen`), and other related functionalities, providing tutorials, schematics, and detailed descriptions of dialogs and settings within the software."
---

# A+W Business Einkauf: Softwarereferenz

## Wareneingang

### Über-/Unterlieferung akzeptieren

Die Stückzahl der Lieferung kann sich von der Bestellung unterscheiden. Sie können die abweichenden Stückzahlen akzeptieren und damit die Lieferung für die Position als komplett erfassen.
- Über- oder Untermengen werden nicht akzeptiert.
- Die eingegebene Stückzahl wird akzeptiert und die Position wird als komplett gebucht.
  - Wenn ein Lagerartikel geliefert wurde, wird der Lagerbestand der gelieferten Menge entsprechend aktualisiert. Die geänderte Menge wird in die Bestellung zurückgeschrieben.
  - Wenn die Lieferung zu einem Auftrag bestellt wurde, wird die neuen Mengen in den Auftrag als Über- oder Untermenge eingetragen.
    - Ist der Auftrag bereits in der Produktion, wird die Mengenänderung an das Produktionssystem übergeben.
    - Ist der Auftrag noch nicht in der Produktion, wird die Über-/Untermenge mit der Produktionsübergabe an das Produktionssystem gemeldet.
- Dazu muss in den Firmendaten die Checkbox **Bestellung und Auftrag ändern, wenn Über/-Unterlieferung akzeptiert** aktiviert werden.
  - ⇨ Stammdaten, "Firmendaten – Lager/EK/EDI" auf Seite B-970

### Bestätigung

- **AB-Lieferant**: Nummer der Auftragsbestätigung des Lieferanten für die markierte Position.
- **AB-Liefertermin**: Liefertermin für die Position.

### Positionen

In der Übersicht werden die Positionen der gewählten Bestellung angezeigt.
- **Pos**.: Nummer der Bestellposition.
- **Komplett buchen**:
  - Eine Position kann als komplett gebucht werden, wenn die gesamte Stückzahl geliefert wurde.
  - Der Wareneingang ist nicht vollständig.
  - Die Position soll als komplett verbucht werden.
- **Auftr.Nr**.: Auftragsnummer.
- **Artikel**: Bezeichnung des bestellten Produkts.
- **Farbe**: (Farb-) Varianten, die zu dem bestellten Produkt erfasst sind.
- **Breite/Höhe**: Maße der bestellten Position.
- **Bestellt**: Stückzahl der Bestellung für diese Position.
- **Avisiert**: Avisierte Stückzahl der Position.
- **Geliefert**: Menge, die für diese Position bereits geliefert wurde. Bei Teillieferungen ist dies die Summe der Stückzahlen, die bisher zu dieser Bestellung geliefert wurden.
- **Eingang**: Menge, die für die markierte Position geliefert wurde.
- **Akzeptieren**:
  - Wenn die Stückzahl der Lieferung höher oder niedriger ist als die der Bestellung, kann diese Stückzahl übernommen werden. Die nicht bestellten Scheiben werden im Lager nur verbucht, wenn es Lagerartikel sind, die in einer Lagerbestellung bestellt wurden. Wenn die Bestellung aus einem Auftrag erzeugt worden ist, werden die Lagerbestände nicht aktualisiert.
  - Die Liefermenge entspricht der Bestellung und braucht nicht gesondert gekennzeichnet zu werden.
  - Die Lieferung ist größer oder kleiner als die Bestellung und wird akzeptiert. Die gelieferte Stückzahl wird in die Bestellung zurückgeschrieben. Der referenzierte Auftrag wird nicht geändert. Die überzähligen Scheiben können ggf. als Bestand verbucht werden.
- **Enthält Kisten**: Anzeige der Bestellungen, in denen Kisten enthalten sind. Die Markierung der Checkbox kann nicht geändert werden.
- **AB-Lieferant**: Nummer der Auftragsbestätigung des Lieferanten.
- **AB-Liefertermin**: Liefertermin aus der Auftragsbestätigung des Lieferanten.
- **Lagerort**: Standard-Lagerort des Lagerartikels. Beachten Sie dabei, dass Lagerartikel auch auf den Lagerort <k.A.> gebucht werden können.
- **Artikelbezeichnung 2 + 3**: Bezeichnungen des bestellten Produkts, die in den Stammdaten hinterlegt sind. Bei Float-Glas ist in der Regel nur die Bezeichnung 1 hinterlegt, die in der Spalte Artikel angezeigt wird.

### Zugehörige Aufträge

In der Übersicht werden die referenzierten Aufträge zu den Positionen angezeigt. Die Felder sind zum Register Komplett beschrieben.
⇨ "Wareneingang - Komplett" auf Seite D-232

## Wareneingang - Identnummer
*Dokumente > Bestellung > Wareneingang > Wareneingang > Register Identnummer*

[Image: Abb. D-138 Wareneingang - Identnummer]

In diesem Register werden die Positionen einer Bestellung mit Kisten angezeigt. Dabei wird für jede Kiste einer Bestellposition eine Unterposition (virtuelle Positionsnummer) erzeugt, der eine Kiste mit einer eigenen Identnummer (Identifikationsnummer, ID) zugewiesen werden kann. Die Vorgabe für die ID können Sie festlegen.
⇨ "Einstellungen (ID)" auf Seite D-240

> **Voraussetzung**
> In den Firmendaten muss die Checkbox für die Vergabe von virtuellen Positionsnummern markiert sein.
> ⇨ Stammdaten, "Fälligkeitsberechnung für Februar (28 oder 29 Tage)" auf Seite B-955

### Kistendaten

- **Lieferanten-Identnummer**: Die Kisten-ID, die der Lieferant für diese Position der Lieferung vergeben hat. Wenn die Nummer eingegeben ist, wird im Feld Identnummer die automatische Kisten-ID angezeigt.
- **Identnummer**: Die automatische Kisten-ID wird angezeigt, sobald Sie die Lieferanten-ID eingetragen haben. Für jede Kiste einer Bestellposition wird beim Erfassen des Wareneingangs eine eigene Kisten-ID erzeugt. Wenn z. B. 5 Kisten mit Float 5 à 1200 x 800 mm bestellt und geliefert wurden, werden die IDs XXXX00001, XXXX00002, ..., XXXX00005 vergeben. Die Vorgabe für XXXX können Sie selbst bestimmen.
  ⇨ "Einstellungen (ID)" auf Seite D-240
- **Lagerort**: Sie können jeder Position einen eigenen Lagerort zuweisen. Beachten Sie dabei, dass Sie auch den Lagerort <k.A.> zuweisen können.
- **Bemerkung**: Bei Besonderheiten, z. B. in der Zuweisung des Lagerortes oder bei Reservierungen, können Sie eine Anmerkung eintragen.
- **Inhalt**: Inhalt der Kiste, die in der Übersicht markiert ist. Der Wert kann ggf. geändert werden.
- **Prod. Datum**: Datum, bis zu dem die Produktion mit der bestellten Lieferung abgeschlossen sein sollte. Dieses Datum ist für die Lagerentnahme nach dem FiFo-Prinzip wichtig, z. B. für beschichtetes Glas.
- **EK / ME**: Einkaufspreis und Preiseinheit der bestellten Position. Wenn Sie den Preis ändern, wird die Änderung in die Bestellung zurückgeschrieben.

### Kistenpositionen
Sie können mehrere Kisten auf einmal auswählen, um diese in einem Schritt zu buchen. Wenn mehr als eine Kiste ausgewählt ist und die Lieferanten-Identnummer eingegeben ist, berechnet das System die Kisten-Identnummern für alle markierte Einträge.

- **Pos**: Positionsnummer aus der Bestellung. Eine Positionsunternummer wird beim Buchen automatisch dann vergeben, wenn die Stückzahl der Bestellposition größer als 1 ist, z. B. 1.1, 1.2 usw.
- **Bezeichnung**: Bezeichnung aus der Bestellung.
- **Breite / Höhe**: Lagermaße der Scheiben in der Kiste.
- **Lieferanten-Identnummer**: Kisten-ID des Lieferanten wie im Bereich Kistendaten eingetragen.
- **Inhalt**: Kisteninhalten wie im Bereich Kistendaten eingetragen.
- **Identnummer**: (Automatische) ID wie im Bereich Kistendaten eingetragen.
- **Lagerort**: Lagerort wie im Bereich Kistendaten eingetragen.
- **Prod. Datum**: Produktionsdatum wie im Bereich Kistendaten eingetragen.
- **Pr./ME**: EK-Preis pro Mengeneinheit wie im Bereich Kistendaten eingetragen.
- **Pr. Einh.**: Preiseinheit für den angezeigten Preis.

## Wareneingang – Protokoll (Identnummern)
*Dokumente > Bestellung > Wareneingang > Wareneingang > Register Protokoll (Identnummern)*

[Image: Abb. D-139 Wareneingang – Protokoll (Identnummern)]

In diesem Register können Sie sich einen Überblick über die vergebenen Kisten-IDs verschaffen.

## Einstellungen (ID)
*Dokumente > Bestellung > Wareneingang > Wareneingang > Menü Optionen > Gruppe Identnummernvergabe > Einstellungen*

[Image: Abb. D-140 Einstellungen]

In diesem Dialog legen Sie die Vorgabe für die Identifikationsnummern (ID) für Kisten fest. Diese Einstellung ist notwendig, um eigene Kisten-IDs automatisch zu vergeben.

Wenn in einer Lieferung z. B. eine Position mit 5 Kisten aufgeführt ist, werden beim Erfassen des Wareneingangs 5 (virtuelle) Unternummern vergeben. Diese Nummern müssen Sie mit einem Kennzeichen versehen, so dass z. B. statt der gescannten Kistennummer 12345 die Unternummern LieferantA00001, LieferantA00002, ..., LieferantA00005 vergeben werden.
⇨ Tutorial, "Kistengeschäft" auf Seite D-136

> **Voraussetzung**
> In den Firmendaten muss die Checkbox für die virtuelle Vergabe von Positionsnummern markiert sein.
> ⇨ Stammdaten, "Fälligkeitsberechnung für Februar (28 oder 29 Tage)" auf Seite B-955

### Lageridentnummer
**Vorgabe** Sie können einen Text (oder Zahlen) mit max. 15 Zeichen eingeben, der durch XXXXX ergänzt wird. XXXXX steht für die automatisch vergebene Nummer. Der Text wird so lange beibehalten, bis Sie ihn ändern.
Wenn Sie von unterschiedlichen Lieferanten Kisten beziehen und diese getrennt kennzeichnen möchten, müssen Sie vor dem Erfassen des Wareneingangs die Vorgabe jeweils entsprechend anpassen.

## Eingangskontrolle
*Dokumente > Bestellung > Wareneingang > Eingangskontrolle*

Im Dialog Wareneingangskontrolle können Sie für Bestellungen prüfen, welche Bestellungen komplett und welche unvollständig geliefert sind.

Wenn Sie beim Buchen von Wareneingängen einen Ziel-Nummernverwalter angegeben haben, werden die Bestellungen automatisch in diesen verschoben.
⇨ "Ziel-Nummernverwalter" auf Seite D-231

In diesem Dialog finden Sie folgende Register:
- "Eingangskontrolle – Komplette Bestellungen" auf Seite D-241
- "Eingangskontrolle – Mengendiskrepanzen" auf Seite D-243

### Eingangskontrolle – Komplette Bestellungen
*Dokumente > Bestellung > Wareneingang > Eingangskontrolle > Register Komplette Bestellungen*

[Image: Abb. D-141 Eingangskontrolle – Komplette Bestellungen]

In diesem Register können Sie sich alle Bestellungen eines bestimmten Nummernverwalters anzeigen lassen und prüfen, ob sie vollständig geliefert sind.
⇨ Tutorial, "Wareneingang kontrollieren" auf Seite D-133

### Nummernverwalter

**Bestell-Nummernverwalter** Nummernverwalter, in dem die Bestellungen (mit Wareneingängen) verwaltet werden. Zur Auswahl werden nur die Nummernverwalter angeboten, die im Menü Bestellung > NV Bestellung angelegt wurden.

### Wareneingang komplett

In der Übersicht werden alle Bestellungen aus dem gewählten Nummernverwalter angezeigt.
- **Nr.**: Nummer der Bestellung.
- **Lieferant**: Name des Lieferanten, an den die Bestellung geschickt wurde.
- **Status**: Status der Bestellung. Der Status wird umgesetzt, wenn die Bestellung vollständig erfasst ist.

> **Alte Bestellungen im Nummernverwalter**
> In der Regel werden Bestellungen nach der Archivierung aus der Hauptdatenbank gelöscht. Die Einstellungen dazu finden Sie in den Firmendaten.
> ⇨ Stammdaten, “Firmendaten – Archiv" auf Seite B-978
> Wenn der Nummernverwalter für Bestellungen mit Wareneingängen zu voll wird, sollten Sie ihn gelegentlich leeren bzw. einen neuen anlegen.
> ⇨ Verkauf, "So leeren Sie einen Nummernverwalter" auf Seite C-193

### Eingangskontrolle – Mengendiskrepanzen
*Dokumente > Bestellung > Wareneingang > Eingangskontrolle > Register Mengendiskrepanzen*

[Image: Abb. D-142 Eingangskontrolle – Mengendiskrepanzen]

In diesem Register können Sie sich alle Positionen von Bestellungen anzeigen lassen, deren Wareneingang noch nicht vollständig verbucht ist.
Sie können Bestellungen als komplett buchen. Teillieferungen können Sie jedoch nur über den Dialog Wareneingang erfassen.
⇨ "Wareneingang (Dialog)" auf Seite D-227

#### Mengendiskrepanzen
In der Übersicht sind alle Bestellungen mit den Positionen angezeigt, deren Wareneingang noch nicht vollständig ist.
- **Nr.**: Nummer der Bestellung.
- **Pos.**: Nummer der Bestellposition, zu der ein Wareneingang offen ist.
- **Artikel**: Bezeichnung der Position.
- **Best. Menge**: Stückzahl der Position, die bestellt wurde.
- **Gel. Menge**: Stückzahl der Lieferung dieser Position. Bei Teillieferungen kann dieser Wert sich von der bestellten Menge unterscheiden.
- **OK**: Wenn die Restlieferung inzwischen eingetroffen ist, können Sie die komplett-Buchung nachholen, indem Sie die Checkbox markieren.
- **Lief. Datum**: Das Lieferdatum wird aus der Bestellung übernommen. Wenn es bei teilweisen Wareneingängen geändert wurde, wird auch hier das neue Datum angezeigt.
- **Lieferant**: Name des Lieferanten, an den die Bestellung geschickt wurde.

## Rechnung
*Dokumente > Bestellung > Rechnung > Rechnungskontrolle*

Sie können die Rechnungen Ihrer Lieferanten in A+W Business erfassen und prüfen, bevor Sie diese an Ihre Buchhaltung und/oder Finanzbuchhaltung (FiBu) übergeben. Dazu steht Ihnen der Dialog Rechnungskontrolle zur Verfügung.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Rechnungskontrolle – Bestellungen" auf Seite D-248
- "Rechnungsdatum" auf Seite D-255

### Rechnungskontrolle
*Dokumente > Bestellung > Rechnung > Rechnungskontrolle*

**Zu Dialogbeschreibung:**
⇨ Elektronische Rechnungskontrolle - Dokumentenimport
⇨ Rechnungsdatum
⇨ Auswahl (Prod. Nr. für Ausgleichspos.)
⇨ Einstellungen für Xternal

In diesem Dialog können Sie die Lieferantenrechnungen erfassen und kontrollieren und zur Übergabe an die FiBu in einen entsprechenden Nummernverwalter stellen.

Angezeigt werden nur die Bestellungen, die den definierten Mindeststatus erreicht haben, z. B. Wareneingang komplett.
⇨ Tutorial, "Preis- und Rechnungskontrolle" auf Seite D-143

> **Sammelrechnung**
> Wenn Ihr Lieferant mehrere Bestellungen in einer Sammelrechnung zusammengefasst hat, kann diese nur geprüft und akzeptiert werden, wenn in allen Bestellungen derselbe MwSt.-Satz und dieselbe Währung angegeben sind.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite D-248
- "Menü Optionen" auf Seite D-248
- "Rechnungskontrolle - Bestellungen" auf Seite D-248
- "Rechnungskontrolle - Positionen" auf Seite D-251
- "Rechnungskontrolle – Stückliste" auf Seite D-253

### Menü Funktionen
*Dokumente > Bestellung > Rechnung > Rechnungskontrolle > Menü Funktionen*

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Rechnungskontrolle zu schließen.

Folgende Einträge werden angezeigt:
- **Teillieferung erstellen:** Öffnet den Dialog Dokumente kopieren, um eine Teillieferung zu erfassen.
  ⇨ Verkauf, "Dokumente kopieren" auf Seite C-543
- **Anlieferpauschale einfügen:** Die Lieferpauschale wird automatisch als Position im Register Positionen eingefügt. Wenn in der Bestellung bereits eine Lieferpauschale enthalten ist, wird die Option nicht ausgeführt.
- **Bestellerfassung öffnen:** Während der Preiskontrolle sind alle aufgelisteten Bestellungen für die Bearbeitung (durch andere Mitarbeiter) gesperrt. Mit dieser Funktion öffnen Sie den Dialog Dokumentenverwaltung, um eine der angezeigten Bestellungen zu bearbeiten. Geänderte Werte werden in die Preiskontrolle übernommen.
  ⇨ Verkauf, "Dokument - Kopfdaten" auf Seite C-424
- **Bestelldaten aktualisieren:** Mit dieser Funktion werden die geänderten Werte sofort in die Bestellung zurückgeschrieben.

### Menü Optionen
*Dokumente > Bestellung > Rechnung > Rechnungskontrolle > Menü Optionen*

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

In diesem Menü finden Sie folgende Gruppen:
- Gruppe Standard
- Gruppe Verhalten
- Gruppe Einstellungen
- Gruppe Xternal

#### Gruppe Standard
- **NettoMwst.**: Nettobeträge werden inkl. Mwst. angezeigt.
- **BruttoMwst.**: Bruttobeträge werden inkl. Mwst. angezeigt.
- **Netto**: Nettobeträge werden ohne Mwst. angezeigt.

#### Gruppe Verhalten
- **Schnellerfassung**: Mit dieser Option springt der Cursor nach der Eingabe einer Bestellnummer in das Feld Auftragssumme. Diese Einstellung wird benutzerbezogen gespeichert.
- **Einschränkung bei Rech.dat.**: Öffnet den Dialog Rechnungsdatum, um eine Abweichung in Tagen festzulegen.
  ⇨ "Rechnungsdatum" auf Seite D-255
- **Ziel-NV füllen**: Schaltet die Felder im Bereich Ziel-Nummernverwalter frei, um einen Mitarbeiter und den zugehörigen Nummernverwalter auszuwählen.

#### Gruppe Einstellungen
- **Rabatt einfrieren**: Der Rabatt wird fixiert. Diese Option sollten Sie aktivieren, wenn Sie neue Rabatte festgelegt haben, in den alten Bestellungen aber die alten Rabatte angewendet werden sollen. Die Preise werden dann nach der Preiskontrolle nicht neu errechnet.
- **Auftragskosten nicht in Statistik korrigieren**: Die EK-Preise im referenzierten Auftrag werden nur korrigiert, solange der Auftrag noch in der Hauptdatenbank vorhanden ist und nicht an die Statistik übergeben wurde.
- **Hinweis auf Lieferterminüberschreitung**: Wenn der Liefertermin beim Kunden nicht eingehalten werden kann, wird eine Meldung angezeigt.

#### Gruppe Xternal
- **Xternal-XML-Datei erstellen**: Diese Option ist nur kundenspezifisch aktiviert.
- **Einstellungen für Xternal**: Öffnet den Dialog Einstellungen, um Vorgaben für den XML-Export festzulegen. Diese Funktion ist nur freigeschaltet, wenn die Option Xternal-XML-Datei erstellen aktiviert ist.

### Rechnungskontrolle – Bestellungen
*Dokumente > Bestellung > Rechnung > Rechnungskontrolle > Register Bestellungen*

[Image: Abb. D-143 Rechnungskontrolle – Bestellungen]

In diesem Register können Sie Lieferantenrechnungen erfassen und zur Übergabe an die FiBu in einen anderen Nummernverwalter weiterleiten.
⇨ Tutorial, "Rechnung kontrollieren" auf Seite D-146

#### Rechnungsdaten
- **Rechnungsnummer**: Pflichtfeld. Sie müssen die Nummer der Lieferantenrechnung eingeben.
- **Rechnungsdatum**: Pflichtfeld. Datum, das auf der Rechnung angegeben ist. Standardmäßig wird immer das zuletzt vergebene Rechnungsdatum vorgeschlagen. Sie können das Datum über den Kalender auswählen oder manuell eingeben, z. B. als 16052013.

#### Bestelldaten
Mit der Wahl einer der beiden Optionen werden die zugehörigen Felder freigeschaltet, um die Bestellung (en) auszuwählen, zu denen die Rechnungen geprüft werden sollen.
- **Bestellnummer, bis**: Wenn Sie in beiden Feldern dieselbe Nummer eintragen, wird nur diese eine Bestellung im Bereich Bestellungen angezeigt. Wenn zu einer Rechnung mehrere Bestellungen gehören, können Sie nacheinander mehrere Bestellnummern eingeben und in die Übersicht übernehmen. Dazu müssen alle Bestellungen zum selben Lieferanten gehören und denselben MwSt.-Satz haben.
- **Nummernverwalter**: Wenn Sie einen Nummernverwalter ausgewählt haben, werden im Bereich Bestellungen alle Bestellungen aufgelistet, die in diesem Nummernverwalter stehen.

#### Summen
Erst wenn Sie den Betrag aus der Rechnung des Lieferanten eingegeben und mit [Ausführen] bestätigt haben, können Sie zu einem der anderen Register wechseln.
- **Rechnungssumme, Mwst.**: Pflichtfeld. Gesamtbetrag der Rechnung und der Mehrwertsteuer. Der Betrag der Mehrwertsteuer wird nicht angezeigt, wenn der Modus Netto ausgewählt ist.
- **Modus**: Mit der Wahl des Modus wird die Mehrwertsteuer angezeigt oder ausgeblendet. Den Standard-Modus können Sie im Menü Optionen > Gruppe Standard festlegen.
  - **Netto mit Mwst.**: Der Gesamtbetrag wird als Nettobetrag gewertet, der Betrag der Mehrwertsteuer wird angezeigt.
  - **Brutto mit Mwst.**: Der Gesamtbetrag wird als Bruttobetrag gewertet, der Betrag der Mehrwertsteuer wird angezeigt.
  - **Netto**: Der Gesamtbetrag wird als Nettobetrag gewertet, der Betrag der Mehrwertsteuer wird nicht kontrolliert.
- **Währung**: Sie können nur dann eine andere Währung auswählen, wenn Sie mit mehreren Währungen arbeiten.
In der Kombobox werden alle Währungen zur Auswahl angeboten, die in den Stammdaten hinterlegt sind. Mit der Auswahl einer anderen Währung als Euro werden in der Übersicht die Beträge der Bestellungen und die Mehrwertsteuer zusätzlich in der gewählten Währung angezeigt.
  ⇨ Stammdaten, "Währungen" auf Seite B-464
- **Kurs**: Wenn Sie mit mehreren Währungen arbeiten, wird der Wechselkurs angezeigt, der in den Stammdaten hinterlegt ist. Er kann überschrieben werden. Wenn Sie nur mit Euro arbeiten, muss in diesem Feld 1 stehen.

> **Wechselkurs fixieren**
> Sie können pro Bestellung einen abweichenden Wechselkurs vereinbaren. Dieser wird automatisch zur Berechnung in der Rechnungskontrolle herangezogen. Sie können ihn nur überschreiben, wenn er in der Bestellung nicht fixiert ist.
> ⇨ Verkauf, "Kurs fixiert für Rechnungsdruck" auf Seite C-440

#### Ziel-Nummernverwalter
Diese beiden Felder sind nur freigeschaltet, wenn die Option Ziel-NV füllen aktiviert ist. Die Rechnungen werden dann nach der Rechnungskontrolle in den angegebenen Nummernverwalter verschoben, z. B. um sie dann anzuweisen.
⇨ "Menü Optionen" auf Seite D-206

- **Mitarbeiter**: Name des Mitarbeiters, dem der Ziel-Nummernverwalter zugeordnet ist.
- **Nummernverwalter**: Nummernverwalter, in den die Rechnungen nach der Prüfung gestellt werden sollen.

#### Bestellungen
In der Übersicht werden alle Bestellungen angezeigt, die sich im Nummernverwalter befinden. Wenn Sie im Bereich Bestelldaten über die Bestellnummern gefiltert haben, werden nur die entsprechenden Bestellungen angezeigt.
Die Spalten mit den Beträgen der Mehrwertsteuer und der Fremdwährung werden nur angezeigt, wenn ein Modus mit Mehrwertsteuer und/oder eine Fremdwährung ausgewählt ist.

**Summe**: In diesen Feldern werden die Gesamtsumme der aufgelisteten Bestellungen und der Gesamtbetrag der Mehrwertsteuer angezeigt.

**Zugrundeliegender Mwst-Satz**: In diesem Feld wird der Prozentsatz zur Berechnung der Mehrwertsteuer angezeigt, der in der Bestellung angegeben ist, die zu dieser Rechnung gehört.
⇨ Verkauf, "Steuersatz" auf Seite C-532

### Rechnungskontrolle – Positionen
*Dokumente > Bestellung > Rechnung > Rechnungskontrolle > Register Positionen*

[Image: Abb. D-144 Rechnungskontrolle – Positionen]

In diesem Register können Sie die Positionen aller Bestellungen prüfen, zu der Sie eine Lieferantenrechnung erfasst haben.
Das Register wird nur angezeigt, wenn im Register Bestellungen die Pflichtfelder gefüllt sind und mit [Ausführen] bestätigt wurden.
⇨ Tutorial, "Rechnung kontrollieren" auf Seite D-146

#### Bestellpositionen
In der Übersicht werden alle Positionen der Bestellungen aufgeführt, auf die sich die Rechnung bezieht.
- **Bestell-Nr.**: Nummer, mit der die Bestellung in der Datenbank gespeichert ist.
- **Pos**: Nummer der Bestellposition.
- **Artikel**: Bezeichnung der bestellten Position.
- **Breite / Höhe**: Maße der bestellten Position.
- **Euro-Netto**: Preis der Position in der Landeswährung (hier Euro). Wenn Sie mit einer anderen Währung arbeiten, ändert sich die Bezeichnung entsprechend. Wenn Sie mit zwei Währungen arbeiten, wird für die zweite Währung eine weitere Spalte mit dem entsprechenden Betrag angezeigt.
- **Mwst.-Euro**: Betrag der Mehrwertsteuer in der Landeswährung (hier Euro). Die Spalte wird nicht angezeigt, wenn im Register Bestellungen die Option Netto gewählt ist. Für die Anzeige der Mehrwert-Steuer im Mehrwährungssystem gilt das gleiche, wie für die Anzeige des Betrags.
- **Stückl.genaue Eingabe**: In dieser Spalte wird angezeigt, ob Sie Preisdifferenzen auf der Ebene der Stücklisten-Komponenten oder der Positionen korrigiert haben.
  - **Deaktiv**: Der Preis wurde nicht geändert oder der Preis der gesamten Position wurde geändert.
  - **Aktiv**: Der Preis wurde in der Stückliste geändert.
- **Menge**: Gelieferte Menge.
- **Lieferant**: Nummer und Name des Lieferanten.

**Gesamtbetrag**: Anzeige der Summe der (eingegebenen) Positionsbeträge.
**Gesamtmenge**: Summe der Positionsmengen.
**Differenz**: Anzeige der Differenz zwischen der Rechnungssumme im Register Bestellungen und der Summe der (eingegebenen) Positionsbeträge. In diesem Fall kann der Preis nicht bestätigt werden, bevor Sie die Preise der Positionen oder der Stücklisten geändert haben.

> **Differenz**
> Eine Differenz wird auch angezeigt, wenn Sie im Register Bestellungen versehentlich eine falsche Rechnungssumme eingetragen haben oder der Wechselkurs nicht korrekt ist.

### Rechnungskontrolle – Stückliste
*Dokumente > Bestellung > Rechnung > Rechnungskontrolle > Register Stückliste*

[Image: Abb. D-145 Rechnungskontrolle – Stückliste]

In diesem Register können Sie sich den Preis einer Position auf der Ebene der Stückliste und der Stücklisten-Komponenten anzeigen lassen. Das Register ist nur aktiv, wenn im Register Positionen eine Position mit Stückliste markiert ist.
⇨ Tutorial, "Rechnung kontrollieren" auf Seite D-146

#### Stücklistenaufbau
In diesem Feld wird die Stückliste der Position angezeigt, die im Register Positionen markiert ist.

#### Preise
Die Anzeige der Felder hängt davon ab, welche Stücklisten-Komponente markiert ist.
Sie können die Preise auf der Hauptebene oder an den Stücklisten-Komponenten korrigieren. Sie können die Austauschzuschläge und Preise der einzelnen Komponenten ändern.
- **Preis / PE**: Anzeige des Preises und der Preiseinheit aus der Bestellung.
- **Rabatt**: Anzeige des Rabattes aus der Bestellung. Der Wert kann nicht geändert werden.
- **Netto / Positionsmenge**: Anzeige des Preises und der Menge aus der Bestellung, wenn die Hauptposition markiert ist. Der Wert kann nicht geändert werden.
- **Netto / Stücklistenmenge**: Anzeige des Preises und der Menge aus der Bestellung, wenn eine Komponente markiert ist. Der Wert kann nicht geändert werden.
- **Netto ges.**: Anzeige des Positions-Preises aus der Bestellung, wenn die Hauptposition markiert ist. Der Wert kann geändert werden.
- **Netto ges. / Pos. Menge**: Anzeige des Komponenten-Preises und der Menge, wenn eine Komponente markiert ist. Der Wert kann geändert werden.
- **Gesamtsumme**: Anzeige des Komponenten-Preises pro Position, wenn eine Komponente markiert ist. Der Wert kann geändert werden.

### Rechnungsdatum
*Dokumente > Bestellung > Auftragsbestätigung > Preiskontrolle > Menü Optionen > Gruppe Verhalten > Einschränkung bei Rech.dat.*
*Dokumente > Bestellung > Rechnung > Rechnungskontrolle > Menü Optionen > Gruppe Verhalten > Einschränkung bei Rech.dat.*

[Image: Abb. D-146 Einschränkungen für Rechnungsdatum]

In diesem Dialog können Sie angeben, um wie viele Tage das Rechnungsdatum vom aktuellen Tagesdatum höchstens abweichen darf. Damit können fehlerhafte Eingaben des Datums verhindert werden.
Die Einstellung ist nur für die Rechnungskontrolle sinnvoll.

#### Abweichung
**In Tagen**: Der Wert gibt die Anzahl der Tage an, um die das Rechnungsdatum vom aktuellen Tagesdatum abweichen darf. Wenn der erlaubte Zeitraum durch eine fehlerhafte Eingabe des Datums überschritten wird, wird automatisch das maximal erlaubte Datum eingesetzt.

> **Beispiel**
> Angezeigt: 24.08. - erlaubt sind 10 Tage
> Eingabe 13.08. - Korrektur auf 14.08.

Wenn Sie eine 0 (Null) eintragen, ist die Funktion abgeschaltet.

## Elektronische Rechnungskontrolle
*Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle*

**Zu Dialogbeschreibung:**
⇨ Auswahl (Prod. Nr. für Ausgleichspos.)
⇨ Positionen manuell zuordnen
⇨ Fußzuschläge/-rabatte verteilen
⇨ Filtereinstellungen

Wenn Sie Rechnungen Ihrer Lieferanten elektronisch erhalten, können Sie die Zuordnung der Positionen zu Ihren Bestellungen, die Preise und Termine prüfen. Dazu steht Ihnen die elektronische Rechnungskontrolle zur Verfügung.
⇨ Tutorial, “Export/Import (openTRANS)" auf Seite D-151
⇨ Tutorial, "Elektronisches Dokument prüfen" auf Seite D-170

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite D-256
- "Menü Optionen" auf Seite D-257
- "Elektronische Rechnungskontrolle – Dokumentenimport" auf Seite D-259
- "Elektronische Rechnungskontrolle – Positionsübersicht" auf Seite D-262

### Menü Funktionen
*Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Menü Funktionen*

Über dieses Menü können Sie andere Dialoge öffnen, ohne die elektronische Rechnungskontrolle zu schließen.
Folgende Einträge werden angezeigt:
- **Anlieferpauschale einfügen**: Die Lieferpauschale wird automatisch als Position im Register Positionen eingefügt. Wenn in der Bestellung bereits eine Lieferpauschale enthalten ist, wird die Option nicht ausgeführt.
- **Bestellerfassung öffnen**: Während der Rechnungskontrolle sind alle aufgelisteten Bestellungen für die Bearbeitung (durch andere Mitarbeiter) gesperrt. Mit dieser Funktion können Sie den Dialog Dokumentenverwaltung öffnen, um eine der angezeigten Bestellungen zu bearbeiten. Geänderte Werte werden in die Rechnungskontrolle übernommen.
  ⇨ Verkauf, "Dokument - Kopfdaten" auf Seite C-424
- **Positionen manuell zuordnen**: Öffnet den Dialog Positionen manuell zuordnen, um die Positionen des elektr. Dokuments den Positionen der Bestellung(en) zuzuordnen.
  ⇨ "Positionen manuell zuordnen" auf Seite D-221
- **Fußzuschläge/-rabatte auf Bestellungen verteilen**: Öffnet den Dialog Fußzuschläge/-rabatte auf Bestellungen verteilen, um den Zuschlag/Rabatt aus dem elektr. Dokument auf die zugeordneten Bestellungen zu verteilen.
  ⇨ "Fußzuschläge/-rabatte verteilen" auf Seite D-222
- **Manuelle Positionszuordnung aufheben**: Hebt die manuelle Zuordnung der markierten Rechnungs-/Bestellpositionen wieder auf.
- **Alle Positionszuordnungen aufheben**: Hebt alle manuellen Zuordnungen von Rechnungs- und Bestellpositionen wieder auf.

### Menü Optionen
*Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Menü Optionen*

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

In diesem Menü finden Sie folgende Gruppen:
- Gruppe Allgemein
- Gruppe Einstellungen
- Gruppe Xternal

#### Gruppe Allgemein
- **Betragsdifferenzen akzeptieren**: Bei der elektronischen Rechnungskontrolle können Betragsdifferenzen, die durch Rundungen auftreten können, generell akzeptiert werden.
- **Hinweis auf Betragsdiff./Ausgl.pos.**: Wenn Rundungsdifferenzen automatisch einer Ausgleichsposition zugeordnet wurden, wird ein Hinweis angezeigt.
- **Rabatt einfrieren**: Mit dieser Option wird der Rabatt fixiert. Diese Option sollten Sie aktivieren, wenn Sie neue Rabatte festgelegt haben, in den alten Bestellungen aber die alten Rabatte angewendet werden sollen. Die Preise werden dann nach der Rechnungskontrolle nicht neu errechnet.
- **Auftr.-EK nur korrigieren bis in Statistik**: Die Korrekturen des EK-Preises im referenzierten Auftrag werden nur durchgeführt, solange der Auftrag noch in der Hauptdatenbank vorhanden ist und nicht an die Statistik übergeben wurde.
- **Prod.Nr. für Ausgleichspos.**: Öffnet den Dialog Auswahl, um eine Ausgleichposition für Rundungsdifferenzen zuzuordnen.
  ⇨ "Auswahl (Prod. Nr. für Ausgleichspos.)" auf Seite D-220

#### Gruppe Einstellungen
- **Hinweis auf Lieferterminüberschreitung**: Bei Überschreitung des geplanten Liefertermins wird eine Meldung angezeigt.
- **Automatische Zuordnung unterdrücken**: Im Dialog Positionen manuell zuordnen können Sie die Checkbox für die automatische Zuordnung aktivieren, damit die Fußzuschläge/-rabatte der Auftragsbestätigung automatisch einem A+W Business-Produkt zugeordnet werden. Diese automatische Zuordnung können Sie unterdrücken.
  ⇨ "Zuordnung des Fußzuschlags/-rabatts zukünftig automatisch auflösen" auf Seite D-222
  Wenn diese Option geändert wurde, muss das aktuell eingelesene Dokument nochmals eingelesen werden.
  ⇨ Tutorial, "So lesen Sie ein XML-Dokument ein" auf Seite D-169
- **Referenzierenden Produktnummern des Lieferanten vertrauen**: Wenn im importierten Dokument eine A+W Business-Produktnummer als Referenz angegeben ist, kann die Zuordnung automatisch durchgeführt werden.

#### Gruppe Xternal
- **Xternal-XML-Datei erstellen**: Für den elektronischen Datenaustausch wird eine XML-Datei erzeugt.
- **Einstellungen für Xternal**: Öffnet den Dialog Einstellungen, um Vorgaben für den XML-Export festzulegen. Diese Funktion ist nur freigeschaltet, wenn die Option Xternal-XML-Datei erstellen aktiviert ist.

### Elektronische Rechnungskontrolle – Dokumentenimport
*Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Register Dokumentenimport*

[Image: Abb. D-147 Elektronische Rechnungskontrolle – Dokumentenimport]

In diesem Register prüfen Sie die importieren Rechnungen. Nur wenn der Dokumentenstatus fehlerfrei ist, kann die Rechnungskontrolle erfolgreich abgeschlossen werden.
⇨ Tutorial, "Export/Import (openTRANS)" auf Seite D-151
⇨ Tutorial, "Elektronisches Dokument prüfen" auf Seite D-170

#### Buchungsart
Mit der Wahl der Option legen Sie fest, wie das elektronische Dokument verarbeitet werden soll. Die Optionen sind dem Dokumentenstatus entsprechend freigeschaltet.
- **Ablehnen**: Mit dieser Option werden die Dokumente nicht übernommen. Die Rechnungskontrolle wird nicht durchgeführt.
- **Akzeptieren**: Mit dieser Option wird die Rechnungskontrolle bestätigt. Die AB-Nummer, Preise und Liefertermine aus dem importierten Dokument werden in die Bestellungen zurückgeschrieben. Die Dokumentenhistorie wird aktualisiert.
- **Teillieferung erstellen**: Zu den im Dokument (Teilrechnung) enthaltenen Positionen wird eine (neue) Teillieferung erstellt und wie bei Akzeptieren verbucht. Die restlichen Positionen bleiben in der ursprünglichen Bestellung erhalten. Der Status dieser Bestellung wird entsprechend angepasst. Bei einem Lieferavis wird mit dieser Buchungsart eine Teilbestellung erzeugt.

#### Rechnungen
In der Übersicht sind alle importierten Rechnungen aufgelistet. Diese können auch von unterschiedlichen Lieferanten stammen.
Wenn Sie einen Eintrag markieren, werden die referenzierten Dokumente in der Übersicht Bestellungen / Teillieferungen angezeigt.
- **Rechnungsnummer**: Rechnungsnummer, die der Lieferant angegeben hat.
- **Lieferant**: Name des Lieferanten.
- **Netto**: Gesamtbetrag der Lieferung.
- **Mwst**: Betrag der Mehrwertsteuer dieser Rechnung.
- **Währung**: Währung, in der der Betrag in der Rechnung angegeben ist. Diese Anzeige ist nur dann von Bedeutung, wenn Sie mit einem Mehrwährungssystem arbeiten.

**Anzeige**: Sie können die Anzeige der Dokumente einschränken.

**Filtereinstellungen**: Sie können Filter für die Anzeige der importierten Dokumente festlegen.
⇨ "Filtereinstellungen" auf Seite D-223

#### Dokumentenstatus
Die rote oder grüne Markierung gibt an, ob Unstimmigkeiten festgestellt wurden oder nicht. Die Optionen im Bereich Buchungsart sind entsprechend gesperrt oder freigeschaltet.
- **Kein Dokument ausgewählt**: Die Anzeige des Dokumentenstatus kann nicht aktualisiert werden, da kein Dokument in der Übersicht markiert ist. Dieser Eintrag wird nicht angezeigt, wenn eine Rechnung markiert ist.
- **Mindestens ein Fußzuschlag/-rabatt einer Bestellung konnte dem Dokument nicht zugeordnet werden**: Dieser Eintrag wird nur angezeigt, wenn eine Rechnung mit einem entsprechenden Fehler markiert ist.
- **Bestellungen vollständig referenziert**: Bei einer roten Anzeige stimmt mindestens eine der referenzierten Positionen nicht vollständig mit der importierten Rechnung überein. Die unvollständig referenzierten Bestellungen werden in der Übersicht gekennzeichnet.
- **Fehlende Artikelpositionen in Bestellungen**: In der Rechnung sind Positionen enthalten, die in der Bestellung nicht aufgeführt sind.
- **Fehlende Fußzuschläge/-rabatte in Bestellungen**: Fußzuschläge/-rabatte werden nicht mitbestellt. Da sie aber in der Rechnung aufgeführt sind, müssen sie für die Rechnungskontrolle als Positionen in den Bestellungen vorhanden sein. Die fehlenden Fußzuschläge/-rabatte müssen in der Bestellung manuell erfasst werden.
- **Preisdifferenz**: Die Gesamtpreise von Bestellung und Rechnung sind unterschiedlich. In zugehörigen Feldern wird die Abweichung als Betrag und prozentual angezeigt.
- **Mengendifferenz**: Die Positionsmengen von Bestellung und Rechnung sind unterschiedlich.

**[Dokument anzeigen]**: Öffnet die Dokumentenansicht des markierten Dokuments.

#### Bestellungen / Teillieferungen
In der Übersicht werden die referenzierten Dokumente angezeigt, wenn Sie einen Eintrag im Bereich Rechnungen markiert haben. Teillieferungen werden in blauer Schrift angezeigt.
- **Bestellnummer**: Nummer der Bestellung, die von A+W Business erzeugt wurde.
- **Netto**: Gesamtbetrag der Bestellung.
- **Mwst**: Betrag der Mehrwertsteuer dieser Bestellung.
- **Währung**: Währung, in der der Betrag in der Bestellung angegeben ist. Diese Anzeige ist nur dann von Bedeutung, wenn Sie mit einem Mehrwährungssystem arbeiten.
- **Auftr.Nr.**: Nummer des referenzierten Auftrags.
- **Kundenliefertermin**: Datum der Anlieferung beim Kunden.
- **Bemerkung**: Wenn die Verknüpfung zwischen der Bestellung und dem importierten Dokument nicht vollständig ist, wird ggf. ein Hinweis auf den Fehler angezeigt.

### Elektronische Rechnungskontrolle – Positionsübersicht
*Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Register Positionsübersicht*

[Image: Abb. D-148 Elektronische Rechnungskontrolle – Positionsübersicht]

In diesem Register können Sie die Positionen der Rechnung prüfen, die Ihr Lieferant gesendet hat.
Die Optionen im Bereich Buchungsart sind zu Register Dokumentenimport erklärt.
⇨ "Elektronische Rechnungskontrolle - Dokumentenimport" auf Seite D-259

#### Positionsübersicht
In der Übersicht sind alle Positionen der Rechnung aufgeführt. Wenn Sie eine Position markieren, werden die Details in den Bereichen Dokumentenposition und Bestellposition angezeigt.
- **Pos-Nr.**: Positionsnummer aus der AB.
- **Bestell-Nummer**: Nummer der referenzierten Bestellung.
- **Bestell-Position**: Positionsnummer aus der Bestellung.
- **Netto Dokument/Netto 1 Bestellung**: Positionspreis aus der importierten AB und aus der Bestellung.
- **Menge Dokument/Menge 1 Bestellung**: Positionsmenge aus der importierten AB und aus der Bestellung.
- **Abmessung Dokument/Abmessung 1 Bestellung**: Positionsmaße aus der importierten AB und aus der Bestellung.
- **Differenz Preis**: Differenz aus Spalte Netto Dokumente und Netto Bestellung.
- **Differenz 1 Preis %**: Preisdifferenz in Prozent.
- **Differenz 2 Menge**: Differenz aus Spalte Menge Dokumente und Menge Bestellung.
- **Auftr.Nr.**: Nummer des referenzierten Auftrags.
- **Kundenliefertermin**: Datum der Anlieferung beim Kunden.

#### Dokumentenposition, Bestellposition
In diesen beiden Bereichen werden Details zu der Position angezeigt, die in der Positionsübersicht markiert ist.

## Basisglasverrechnung
*Dokumente > Bestellung > Basisglasverrechnung*

Diese Funktion ist nur kundenspezifisch freigeschaltet.
In der Basisglasverrechnung werden Modellscheiben mit ihrer tatsächlichen Fläche anstatt der fakturierten Fläche übergeben und verrechnet.

# A+W Fertigung
---
[Image: A+W Business Logo]

## Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Version/Datum | Beschreibung |
| :--- | :--- |
| **5.50/06-2023** | Aktualisierung der Softwarereferenz. |
| **5.20/04-2020** | Einstellungen zur Produktionsübergabe und Tourenliste aktualisiert. |
| **5.11/01-2018** | Kapitel Gestellverwaltung – Historie korrigiert. |
| **5.10/07-2017** | Strukturelle Überarbeitung. Dialog Versanddaten ändern neu (ersetzt Dialog Touren/Liefertermine umsetzen), Dialog Gestellbelegung neu, Dialog Terminübersicht aktualisiert. |
| **5.01/01-2017** | Produkt- und Firmennamen angepasst. |
| **5.00/07-2013** | Überarbeitung der ALFAK-Dokumentation und Anpassung auf A+W Business. |
| **4.01/01-2012** | Korrektur Angebotsübergabe an Produktion. |
| **4.00/04-2011** | Vollständige Überarbeitung und Umstellung auf Doku-Konzept 2010. |
| **3.02/09-2008** | Abbildungen und Part-Nummer angepasst. |
| **3.01/08-2008** | Rechtschreibkorrekturen. |
| **3.00/12-2003** | Struktureller Umbau auf Programmstruktur 4.0. |
| **2.00/08-2000** | Überarbeitung Fertigung. |
| **1.00/03-1998** | Ersterstellung. |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen
- Kontakte

#### Anmerkungen zu diesem Dokument
Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Business gedacht.
Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.
Dieses Dokument beschreibt die volle Ausbaustufe von A+W Business.

#### Urheberrechte
© 2023, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.
Die Dokumentation darf nur gemäß des Lizenzvertrages ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung von A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

#### Warenzeichen
Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

#### Kontakte
**A+W Software GmbH**
Siemensstr. 3
D-35463 Fernwald
Germany
+49 641 96620-0
aw.zentrale@a-w.com
http://www.a-w.com

---

## Tutorial

### Überblick
Das Tutorial zum Modul Fertigung beschäftigt sich mit den Grundlagen der Produktionsübergabe und dem Versand in A+W Business. Es baut auf den Kenntnissen zu den Stammdaten auf.

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
Für das Modul Fertigung stehen folgende Dokumente zur Verfügung:
- **Handout**: Ausdruck des Tutorials für die Schulung
- **PDF**: Vollständige Unterlagen
  - Tutorial
  - Softwarereferenz
  - Index
- **Online-Hilfe <F1>**: Kontextsensitive Dialog-Hilfe der A+W Business-Softwarereferenzen und Tutorials der Basisversion

### Aufbau des Tutorials
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

### Darstellungskonventionen
Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:
- *Kursiv*: sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Produktionsübergabe*.
- **Fett**: sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: Geben Sie den Wert **0** ein.
- >: Mit dem sogenannten Brotkrumenpfad ist der Weg gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B. *Fertigung > Produktion > Produktionsübergabe*.
- []: Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit **[OK]** speichern Sie die Daten.
- <>: Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit **<F1>** öffnen Sie die Online-Hilfe.

### Menü-Übersicht
In diesem Abschnitt finden Sie eine kurze Übersicht über die Programmbereiche, die in den Themenblöcken dieser Schulung angesprochen werden.

[Image: Abb. E-1 Menü Fertigung]

#### Produktion
In diesem Bereich übergeben Sie die Aufträge an die Produktion.
⇨ "Produktionsübergabe" auf Seite E-20
⇨ Softwarereferenz, "Produktion" auf Seite E-169

#### Lieferwesen
In diesem Bereich organisieren Sie den Versand mit Ihrem eigenen Fuhrpark.
⇨ "Lieferwesen" auf Seite E-81
⇨ Softwarereferenz, "Lieferwesen" auf Seite E-204

#### Gestellverwaltung
In diesem Bereich können Sie eigene und Fremdgestelle verwalten und sich einen Überblick über den aktuellen Bestand verschaffen.
⇨ "Gestellverwaltung" auf Seite E-159
⇨ Softwarereferenz, "Gestellverwaltung" auf Seite E-255

#### Terminübersicht
In diesem Bereich können Sie sich einen Überblick über die Termine und die Kapazitäten verschaffen.
⇨ "Terminübersicht" auf Seite E-117
⇨ Softwarereferenz, "Terminübersicht" auf Seite E-269

#### Zollverwaltung
In diesem Bereich können Sie Zoll-Listen für den Warenexport erstellen.
⇨ Softwarereferenz, "Zollverwaltung" auf Seite E-284

#### Angebotsoptimierung
In diesem Bereich können Sie die Angebote zur Optimierung an die Produktion übergeben.
⇨ "Übergabe zur Angebotsoptimierung" auf Seite E-52
⇨ Softwarereferenz, “Angebotsoptimierung" auf Seite E-292

#### Dokumentendaten
In diesem Bereich können Sie sich Übersichten über Aufträge und korrespondierende Bestellungen anzeigen lassen und ggf. die Termine korrigieren. Eine ausführliche Beschreibung zu diesem Dialog finden Sie im Part Verkauf.
⇨ Verkauf, "Dokumentendaten" auf Seite C-755

#### Artikel-Info
In diesem Bereich können Sie sich Informationen zu den Produkten anzeigen lassen, die in A+W Business angelegt sind. Sie können dabei den Produktaufbau, die Preise und die Verfügbarkeit prüfen. Eine ausführliche Beschreibung zu diesem Dialog finden Sie im Part Verkauf.
⇨ Verkauf, "Artikel-Informationen" auf Seite C-616

#### Faxnachricht
In diesem Bereich können Sie direkt aus A+W Business Faxnachrichten an Ihre Kunden und Lieferanten erstellen und versenden. Eine ausführliche Beschreibung zu diesem Dialog finden Sie im Part Überblick.
⇨ Einleitung, "Standard-Menüs" auf Seite A-53

#### Ergänzende Informationen
⇨ Einleitung, "Elemente des Programmfensters" auf Seite A-52
⇨ Verkauf: Softwarereferenz, "Dokument - Kopfdaten" auf Seite C-424

### Grundgedanken zu Fertigung und Versand
Über die Dokumentenverwaltung sind Aufträge erfasst worden, deren Positionen gefertigt werden müssen. Dazu müssen die Aufträge bzw. die Positionen in die Produktion weitergeleitet werden. Die für die Produktion relevanten Daten werden dabei in eine Datei geschrieben, die von der Produktionssoftware eingelesen werden kann.

Mit Hilfe des ERP-Webservices können diese Übergabedateien direkt an die Produktionssoftware A+W Production weitergeleitet und dort eingelesen werden.

[Image: Abb. E-2 Produktionsübergabe und Versandorganisation]
*Diagramm, das den Datenfluss von A+W Business (Auftrag, Terminüberwachung, Tourenplanung) zur A+W Production (Produktions-Software) über Produktionsübergabe, Bestellung und Wareneingang sowie die Rückmeldung von der Produktion zeigt.*

In dieser Übersicht sehen Sie, wie die Übergabe von Aufträgen an die Produktion, die Rückmeldungen aus der Produktion und die Organisation des Versands zusammenspielen.

Über den Auftragsstatus wird die korrekte Abfolge der Buchungen gesichert, so dass z. B. kein Auftrag an die Produktion übergeben werden kann, der nicht den erforderlichen Status hat. Der aktuelle Stand der Produktion wird als Rückmeldung an A+W Business gesendet. Damit wird der Status pro Auftragsposition und schließlich für den gesamten Auftrag umgesetzt. Je nach betrieblicher Organisation wird der Status automatisch oder manuell hochgesetzt. Die Daten einschließlich der Statusumsetzung können über Barcodes erfasst werden, womit Eingabefehler erheblich reduziert werden.

Über die Prüfung der Kapazitäten können Produktions- und Liefertermine geprüft und ggf. angepasst werden, so dass der Versand optimal organisiert werden kann.

Für den Versand werden Touren- und Beladungslisten erstellt, bei denen die Fahrzeuge anhand des zugelassenen Gewichts und der Tour optimal beladen werden können.

#### Ablauf für Fertigung und Versand
Die Reihenfolge der einzelnen Aktionen für die Fertigung und Auslieferung eines Auftrags hängt von den Gegebenheiten in Ihrem Betrieb ab.
Beispielsweise kann der Ablauf folgendermaßen organisiert sein:
- Produktionsübergabe
- Rückmeldung aus der Produktion prüfen
- Lieferscheine drucken
- Tourenplanung
- Beladungsliste und Empfangsbestätigungsliste drucken
- Auslieferung

### Produktionsübergabe
In diesem Themenblock lernen Sie, wie Sie Aufträge oder Angebote an die Produktion übergeben.
Dazu gehören folgende Lerneinheiten:
- "Varianten der Produktionsübergabe" auf Seite E-21
- "Produktionsübergabe ohne Kapazitätsplanung" auf Seite E-29
- "Produktionsübergabe mit A+W Business Kapazitätsplanung" auf Seite E-43
- "Produktionsübergabe mit A+W Production Capacity Planner" auf Seite E-47
- "Übergabe zur Angebotsoptimierung" auf Seite E-52

#### Varianten der Produktionsübergabe
Die Daten der Aufträge werden zur Produktion an A+W Production oder ein anderes Produktionsprogramm übergeben, nachdem sie den dafür festgelegten Mindeststatus erreicht haben. Für diese Übergabe stehen folgende Varianten zur Verfügung:
- **Ohne Kapazitätsplanung**: Die Aufträge werden direkt an die Produktion übergeben, ohne sie zuvor in eine Kapazitätsplanung einzulasten.
- **Mit A+W Business Kapazitätsplanung**
- **Mit A+W Production Capacity Planner**

Bei diesen beiden Varianten durchlaufen die Aufträge folgende Schritte:
- Die Aufträge werden zunächst an die Kapazitätsplanung übergeben.
- Nach der Bestätigung oder Änderung der Produktions- und Liefertermine wird der Auftragsstatus hoch gesetzt.
- Die Maschinenkapazitäten sind damit reserviert.
- Anschließend werden die Aufträge an die Produktion übergeben und können produziert werden.
Die unterschiedlichen Abläufe werden Sie in getrennten Einheiten kennenlernen.

##### Datenübergabe
Die Daten Ihrer Aufträge werden zur Weiterverarbeitung an A+W Production zur Produktion bzw. A+W Standard Optimizer zur Zuschnittsoptimierung übergeben. Dazu müssen die Produkt- und Artikelnummern in A+W Business und A+W Production einander zugeordnet sein. Bei anderen Produktionsprogrammen können Sie für die Zuordnung einen entsprechenden Schlüssel in der Produktverwaltung > Register Fertigung im Feld Schlüssel Optimierung hinterlegen.

Für das Produzieren von ESG, VSG, Gießharz usw. wird für A+W Production eine Auflösung des Produktes auf Stücklistenebene durchgeführt. Der Produktionsstart wird stückbezogen an A+W Business zurückgemeldet. Je nach Einstellung wird der Auftragsstatus dann erhöht. Diese Einstellungen werden Sie in der Einheit Rückmeldungen kennenlernen.
⇨ “Rückmeldungen aus der Produktion" auf Seite E-58

Unabhängig davon, ob zuerst die Kapazitäten geplant werden, können Sie die Aufträge auf unterschiedliche Weise übergeben:
- **Manuelle Produktionsübergabe**: Für die manuelle Übergabe von Aufträgen steht der Dialog *Produktionsübergabe* zur Verfügung, in dem Sie alle Aufträge eines Nummernverwalters mit Status größer oder gleich Produktionsfreigabe und kleiner dem Status feingeplant übergeben können.
- **Automatische Produktionsübergabe mit Workflow-Task**: Für die automatische Übergabe wird ein Workflow-Task mit einem Intervall eingerichtet, damit in definierten Abständen nach Aufträgen gesucht wird, die an die Kapazitätsplanung oder die Produktion übergeben werden sollen. Die Beschreibung des Workflow-Tasks lernen Sie in einem eigenen Abschnitt kennen.
  ⇨ "Produktionsübergabe per Workflow-Task" auf Seite E-26

##### OrderXML
Das OrderXML-Format basiert auf der genormten OpenTrans-Schnittstelle mit spezifischen Erweiterungen für produktionsrelevante Daten wie Gläser, Sprossen oder Bearbeitungen.
Das Format wird von der Produktionssoftware als Auftrag erkannt. Für jeden an die Produktion übergebenen Auftrag wird eine eigene Datei erstellt. Der Speicherort für die Übergabedatei muss in A+W Business und A+W Production angegeben werden.

##### Statusprüfung
Sowohl für die manuelle als auch für die automatische Produktionsübergabe müssen die Statuspunkte vollständig eingerichtet und zugeordnet sein. Über diese Statuszuordnungen prüft das System, ob die Auftragsdaten übergeben werden können.
Diese Zuordnungen wurden vor der Installation von A+W Business auf Ihren Betrieb abgestimmt und eingerichtet. Grundsätzliches zu den Statuspunkten und den Zuordnungen haben Sie bereits den Schulungen zu den Stammdaten und zum Verkauf kennengelernt. Daher wird das Thema hier nicht weiter erläutert.

##### Stornieren
Jeder Auftrag kann bis zu einem gewissen Zeitpunkt storniert werden. Dieser Zeitpunkt muss betriebsintern geregelt werden.
Bei der Stornierung einer Produktionsübergabe wird der übergebene Auftrag erneut an die Produktion übergeben. Dabei wird ein Stornokennzeichen gesetzt, an dem der Mitarbeiter in der Produktion die Stornierung erkennt.

##### Sonderfall Angebotsoptimierung
Angebote können an die Produktion übergeben werden, um den Zuschnitt zu berechnen. Diese Funktion steht zur Verfügung, wenn eine der folgenden Varianten für die Produktionsübergabe genutzt wird:
- Keine Kapazitätsplanung
- A+W Business Kapazitätsplanung

Die Funktion ist blockiert, wenn die Produktionsübergabe von Angeboten per Workflow-Task aktiviert wird.
Die Übergabe von Angeboten zur Optimierung ist ausführlich in einer eigenen Einheit beschrieben.
⇨ "Übergabe zur Angebotsoptimierung" auf Seite E-52

#### Schematische Abläufe der Varianten
In diesem Abschnitt sind die unterschiedlichen Abläufe der Produktionsübergabe schematisch dargestellt. Die Darstellungen mit Kapazitätsplanung bauen aufeinander auf, so dass die zuvor aufgeführten Schritte zusammengefasst werden.
Die Abläufe sind als Beispiele zu verstehen. In Ihrem Betrieb kann der Übergabeprozess durchaus auch anders organisiert sein.

##### Schematischer Ablauf ohne Kapazitätsplanung
[Diagram showing: Auftrag erfasst -> Produktionsfreigabe (Statuspunkt 35) -> Produktionsübergabe (Statuspunkt 40) -> Einlastung in A+W Production -> Produktions-Rückmeldungen. A separate path shows "Auftrag storniert (Statuspunkt 810)".]
Für die Produktionsübergabe werden der Mindest- und der Sperrstatus geprüft. Aufträge, die diese Bedingungen nicht erfüllten, können nicht übergeben werden.

##### Schematischer Ablauf mit Kapazitätsplanung
[Diagram showing: Auftrag erfasst -> Produktionsfreigabe? (yes/no). 'no' leads to "Status ändern". 'yes' leads to Kapazitätsplanung -> Einlastung erfolgreich? (yes/no). 'no' leads to "Termine ändern". 'yes' leads to Auftragsbestätigung drucken -> Produktionsfreigabe -> Produktionsübergabe -> Einlastung in A+W Production -> Produktionsübergabe -> Produktions-Rückmeldungen.]

##### Schematischer Ablauf mit Bestellung und Positionsänderung
[Diagram showing: Auftrag erfasst -> Kapazitätsplanung -> Auftragsbestätigung drucken -> Bestellteile enthalten? (yes/no). 'yes' leads to "Bestellung schreiben, Wareneingang abwarten" before returning to the main flow. 'no' continues to Produktionsfreigabe -> Produktionsübergabe -> Position geändert? (yes/no). 'yes' leads back to Produktionsübergabe. 'no' continues to Produktion -> Produktions-Rückmeldungen.]
Aus der Kapazitätsplanung werden nach erfolgreicher Planung die Zeitkosten und das Produktionsdatum zurückgemeldet.

#### Änderung von übergebenen Positionen
Ein Auftrag, der an die Produktion übergeben wurde, hat Status 40. Wenn ein solcher Auftrag geändert wird, müssen zwei Fälle unterschieden werden:
- Änderungen von Preisen, Rabatten usw., die nicht produktionsrelevant sind, verändern weder den Status noch muss der Auftrag erneut übergeben werden.
- Nach einer Änderung von Mengen, Maßen, Gläsern u. Ä. erhält der Auftrag ein entsprechendes Kennzeichen und wird sofort durch den Workflow-Task an die Produktion übergeben.
In der Betriebsorganisation muss geklärt werden, was mit Positionen geschehen soll, die bereits produziert sind. Es kann z. B. festgelegt werden, dass eine Auftragsposition storniert und neu angelegt werden muss.

#### Übergabe von Aufträgen mit Bestellungen
Wenn Sie z. B. ISO mit ESG-Scheiben produzieren, das ESG aber nicht selbst herstellen, hängt der Produktionsprozess von der Lieferung der ESG-Scheiben ab. Nach der Buchung der Waren im Wareneingang können die Daten automatisch an A+W Production übergeben werden. Sind in dem gemeldeten Wareneingang solche ESG-Scheiben enthalten, wird für die betreffenden ISO-Einheiten der Produktionsstart initiiert.
Diese automatische Übergabe von Wareneingangsdaten steht in Verbindung mit dem Wareneingang für den Einkauf.

#### Produktionsübergabe per Workflow-Task
Ein Workflow-Task dient der weitgehenden automatischen Verarbeitung von Aufträgen. Inwieweit manuelle Eingriffe zwischen aufeinander folgenden Workflow-Tasks notwendig sind, hängt davon ab, wie die Abläufe in Ihrem Betrieb organisiert sind. Die notwendigen Einstellungen werden bei der Installation festgelegt und sollten nachträglich nicht geändert werden. In diesem Abschnitt werden daher nur die schematischen Abläufe dargestellt.
Jeder Workflow-Task besteht aus einer oder mehreren Customizing-Formeln. In diesen Formeln sind die einzelnen Aktionen definiert, die ausgeführt werden sollen. Der A+W Business Interface Service führt die Tasks entweder periodisch oder zu einem festen Zeitpunkt aus.

##### Einstellungen für den Workflow-Task
Um einen Workflow-Task einzurichten, sind drei Schritte erforderlich:
- Formel für die automatische Produktionsübergabe unter *Stammdaten > Firma > Formeln* anlegen.
- Formel zu einem Workflow-Task unter *Stammdaten > Firma > Customizing > Register Workflow Tasks* zuordnen.
- Workflow-Task unter *Stammdaten > Firma > Customizing > Register Autom. Prozessausführung* einstellen.

Wenn Sie die Produktionsübergabe auf den Workflow-Task umstellen, lassen Sie sich von Ihrem Service-Mitarbeiter bei der A+W Software GmbH unterstützen.
In dieser Einheit werden die Einstellungen an einem Beispiel gezeigt, das sich von den Einstellungen in Ihrem Unternehmen unterscheiden kann.

**So prüfen Sie die Einstellungen für den Workflow-Task**
1. Wählen Sie im Menü *Stammdaten > Firma > Customizing* und wechseln Sie zum Register *Workflow Tasks*.

   [Image: Abb. E-3 Beispiel Workflow-Tasks]
   *In diesem Register sind die definierten Workflow-Tasks für A+W Business mit den zugeordneten Formeln aufgeführt.*

2. Markieren Sie den Workflow Task, den Sie bearbeiten wollen.
3. Wechseln Sie zum Register *Autom. Prozessausführung*.

   [Image: Abb. E-4 Prozessausführung für Workflow-Tasks]
   *A: Startzeit oder Intervall je nach Art der Ausführung*
   *B: Zeitpunkt oder Intervall*

   In diesem Register sind die Startzeiten und die Intervalle für die definierten Workflow-Tasks festgelegt. In der Spalte Ausführung werden die möglichen Einstellungen zur Auswahl angeboten, wenn Sie in ein Feld klicken.

4. Ändern Sie ggf. die Startzeit und das Intervall:
   - Wenn die Daten zyklisch übergeben werden sollen, wählen Sie die Zeit **00:01**.
   - Wenn die Daten zu einem bestimmten Zeitpunkt übergeben werden sollen, tragen Sie in der Spalte hh:mm die Uhrzeit ein.
5. Wenn mehrere Workflow-Tasks definiert sind, wird in der Spalte Sequenz angezeigt, in welcher Reihenfolge sie ausgeführt werden.
6. Wählen Sie im Menü *Start > Speichern*, um die Änderungen zu speichern.
   Die Daten werden gespeichert und der Workflow-Task wird nach den neuen Einstellungen ausgeführt.

#### Produktionsübergabe ohne Kapazitätsplanung
**Lernziele**
- Einstellungen zur Produktionsübergabe ohne Kapazitätsplanung kennenlernen.
- Aufträge an die Produktion übergeben.
- Übergabe stornieren.

**Nutzen**
- Sie übergeben Auftragsdaten aus A+W Business direkt an A+W Production oder A+W Standard Optimizer zur Fertigung.
- Wenn Sie ESG, VSG, Gießharz usw. produzieren, können Sie die Stücklistenauflösung ohne weitere Eingriffe übergeben und vermeiden damit eine fehlerhafte Datenübergabe.
- Bei der automatischen Übergabe per Workflow-Task werden die Aufträge nach einem definierten Intervall direkt an die Produktion übergeben.

**Merke**
- **Aufträge an die Produktion übergeben**: Sie können die Aufträge manuell aus einem Nummernverwalter oder (automatisch) per Workflow-Task an die Produktion übergeben.
- **Übergabedaten**: Die Übergabedaten werden in eine Datei geschrieben, die von A+W Production ausgelesen wird. Der Speicherort dieser Datei muss A+W Business und A+W Production bekannt sein.
- **Übergabe von SN-Dateien**: Für die Übergabe von Shaping+Nesting-Dateien (SN-Dateien) müssen folgende Einstellungen festgelegt werden:
  - In den Firmendaten muss die automatische Generierung aktiviert werden.
  - In den Utilities müssen Regeln eingerichtet sein, nach denen die SN-Datei erzeugt wird.
- **Auftragsstatus**: Statusprüfungen vor der Übergabe verhindern, dass Aufträge mit falschem Status übergeben werden. Bei der manuellen Produktionsübergabe wird immer nach dem Mindest- und Sperrstatus übergeben.
- **Nummernkreis**: Die Nummernkreise für Aufträge und Angebote müssen getrennt sein, damit sich die Dokumente bei der Übergabe nicht gegenseitig überschreiben.
- **Workflow-Task**: Für die automatische Produktionsübergabe muss ein Workflow-Task eingerichtet werden. Den Workflow-Task legen Sie im Dialog *Customizing* (pro Mandant) fest.
- **Formel**: Der Workflow-Task wird mit einer Formel definiert.
- **Datenübertragung**: Bei der automatischen Produktionsübergabe werden die Auftragsdaten per A+W Business-Interface-Service übertragen.
- **Voreinstellungen**:
  - **Firmendaten**:
    - Register *Produktion*
    - Register *Produktion > Einstellungen Aufträge*
    - Register *System* (für SN-Dateien)
  - **Stammdaten**:
    - *Firma > Customizing > Register Workflow Tasks*

> **Beschreibung der Einstellungen**
> In dieser Lerneinheit werden die allgemeinen Einstellungen und Funktionen beschrieben, die für die Produktionsübergabe ohne Kapazitätsplanung gelten. In den Lerneinheiten zur Produktionsübergabe mit Kapazitätsplanung werden Sie dann nur noch auf die Unterschiede und Besonderheiten aufmerksam gemacht. Daher sollten Sie der Einheit Produktionsübergabe ohne Kapazitätsplanung besondere Aufmerksamkeit widmen.

##### Produktionsübergabe einrichten

> **Geänderte Einstellungen können schwerwiegende Fehler erzeugen**
> In der Regel werden die Einstellungen für die Produktionsübergabe bei der Installation von A+W Business auf die Bedingungen im Betrieb abgestimmt. Wenn Sie diese Einstellungen ändern, greifen Sie tief in die Funktionalität der Produktionsübergabe ein. Das kann zu schwerwiegenden Fehlern führen, so dass die Daten von Aufträgen und Angeboten nicht mehr übergeben werden können.
> Die Beschreibung der Einstellungen dient also in erster Linie dazu, Ihnen die Vorgänge deutlicher zu machen und ggf. bei Rücksprachen mit dem Service der A+W Software GmbH Fragen zu den Einstellungen schnell beantworten zu können.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
- "So prüfen Sie die Einstellungen in den Firmendaten" auf Seite E-32
- "So prüfen Sie die Voreinstellungen für die Produktionsübergabe" auf Seite E-33

**So prüfen Sie die Einstellungen in den Firmendaten**
1. Wählen Sie im Menü *Stammdaten > Firma > Firmendaten* und wechseln Sie zum Register *Produktion*.
   Diese Einstellungen gelten sowohl für die manuelle Produktionsübergabe als auch für die automatische Übergabe per Workflow-Task.

   [Image: Abb. E-5 Stammdaten – Einstellungen für automatische Produktionsübergabe]
   *A: Einstellungen für die Produktionsübergabe von Aufträgen festlegen*
   *B: Einstellungen für die Produktionsübergabe von Angeboten festlegen*
   *C: Adresse für den PPS-Webservice eingeben*
   *D: Einstellung zur Meldung des Wareneingangs an A+W Production*
   *E: Adresse für ERP-Webservice eingeben*
   ⇨ Stammdaten, "Firmendaten - Parameter" auf Seite B-948

2. Tragen Sie in den Bereichen *A+W Production Anbindung* und *ERP-Webservice* die Adressen für den Datenaustausch ein:
   - Die Angabe im Feld **ERP-Webservice (E)** benötigen Sie für Datenübertragungen per OrderXML. Achten Sie darauf, dass Sie den ERP-Webservice wählen, der zu der installierten Version von A+W Business passt.
   - Die Angabe im Feld **PPS-Webservice-URL (C)** benötigen Sie für folgende Datenübertragungen:
     - Stornierung von Aufträgen per Workflow-Task
     - Meldung des Wareneingangs (D) direkt an A+W Production. Diese Meldungen werden bei Positionen benötigt, zu deren Fertigung auf Bestellungen gewartet werden muss. Wenn Sie den PPS-Webservice wählen, müssen Sie auch die URL eintragen.
     - Dateilose Rückmeldungen. Diese Funktion lernen Sie in der Einheit Rückmeldungen kennen.
       ⇨ “Rückmeldungen aus der Produktion" auf Seite E-58
3. Wählen Sie im Menü *Start > Speichern*, um die Änderungen zu speichern.
   Sie können nun die Einstellungen für die Übergabe von Aufträgen (A) und Angeboten (B) prüfen. Diese Einstellungen sind in der folgenden Handlungssequenz beschrieben.
   Die Einstellungen für die Angebote werden in der Regel identisch zu denen für Aufträge eingerichtet. Weitere Informationen zur Übergabe von Angeboten werden in einer eigenen Lerneinheit beschrieben.

**So prüfen Sie die Voreinstellungen für die Produktionsübergabe**

> **Benutzerabhängige Einstellung**
> Der Dialog kann von unterschiedlichen Stellen aus geöffnet werden, z. B. aus dem Dialog *Produktionsübergabe*. In dieser Anleitung wird er von den Firmendaten aus geöffnet, weil Sie hier auch die Einstellungen für die Angebotsoptimierung und die Rückmeldungen festlegen können.
> Wenn Sie die Einstellungen benutzerabhängig eingerichtet haben wollen, müssen Sie folgenden Weg wählen:
> *Menü Fertigung > Übergabe Produktion > Menü Funktionen > Einstellungen*

1. Klicken Sie im Dialog *Firmendaten > Register Produktion* auf **[Einstellungen Aufträge]**.
   [Image: Abb. E-6 Produktionsübergabe für Aufträge]
   *A: Auswahl des Übertragungsformats*
   *B: Einstellung für CAD Designer (Bars)-Übergabe*
   *C: Auswahl der OrderXML-Version*
   *D: Statusprüfung vor Übergabe*

2. Im Folgenden werden nur die wichtigsten Einstellungen beschrieben. Eine vollständige Beschreibung aller Register des Dialogs finden Sie in der Softwarereferenz.
   ⇨ Softwarereferenz, "Einstellungen Produktionsübergabe" auf Seite E-174
3. Prüfen Sie im Register *Schnittstelle*, ob die Versionen und die Pfade korrekt eingestellt sind. Standardmäßig ist im Bereich *Schnittstelle Produktion* (A) die OrderXML-Übergabe aktiviert. Wenn Sie mit AWPool arbeiten, müssen Sie die entsprechende Version auswählen.
4. Geben Sie den Pfad der Übergabedatei an, der von A+W Production überwacht wird, damit die Daten automatisch eingelesen werden.
5. Tragen Sie ggf. die Daten für die Übergabe an *AWDesign* (B) ein. Achten Sie dabei darauf, dass der Speicherpfad auch in CAD Designer bekannt ist.
6. Prüfen Sie die Einstellungen im Bereich *OrderXML* (C). Die Adresse des ERP-Webservices wird aus den Einstellungen in den Firmendaten übernommen. Wenn Sie mit der AWPool-Übergabe arbeiten entfällt diese Angabe.
7. Wählen Sie im Bereich *Modus der Übergabe* die Option **nach Mindest- und Sperrstatus Produktionsübergabe** (D). Mit dieser Einstellung werden die Aufträge nach der Statusprüfung direkt an die Produktion übergeben.
8. Wechseln Sie zum Register *Übergabe Parameter*.
   [Image: Abb. E-7 Einstellungen – Übergabeparameter]
9. Wenn Sie mit A+W Production arbeiten, müssen Sie die Checkbox **A+W Production** markieren. Für alle anderen Programme bleibt die Checkbox leer.
10. Markieren Sie die Checkboxen für die Daten, die an die Produktion übergeben werden sollen. Die Bedeutung der Checkboxen ist ausführlich in der Softwarereferenz beschrieben.
    ⇨ Softwarereferenz, “Einstellungen Produktionsübergabe – Übergabe Parameter" auf Seite E-178
11. Wechseln Sie zum Register *Zusätzliche Schnittstellen*, wenn Sie mit einer Schnittstelle zu RONA arbeiten, und tragen Sie die Pfade für die Schnittstellendatei ein.
12. Wechseln Sie zum Register *Texte/Anlagen* und markieren Sie die Textkennzeichen und Dateianhänge, die Sie zusätzlich übergeben wollen.
    [Image: Abb. E-8 Einstellungen - Texte/Anlagen]
    Die Textkennzeichen haben Sie bereits in der Schulung zu Stammdaten kennengelernt. Die Dateianhänge wurden in der Schulung zum Verkauf besprochen.
13. Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern. Die Daten werden gespeichert.

##### Auftragsdaten an die Produktion übergeben
Die Auftragsdaten können manuell oder per Workflow-Task an die Produktion übergeben werden. In diesem Abschnitt lernen Sie, wie Sie Auftragsdaten aus einem Nummernverwalter manuell direkt an die Produktion übergeben.

**So übergeben Sie die Aufträge manuell**
1. Wählen Sie im Menü *Fertigung > Produktion > Übergabe Produktion*.
   [Image: Abb. E-9 Produktionsübergabe starten]
   *A: Auswahl Nummernverwalter*
   *B: Auftragsstatus vor Übergabe*
   ⇨ Softwarereferenz, "Übergabe Produktion" auf Seite E-170
2. Wählen Sie den Nummernverwalter (A) aus, in dem Sie die Aufträge für die Produktion gesammelt haben.
3. Prüfen Sie, ob alle angezeigten Aufträge den Mindeststatus erreicht haben (B). Aufträge, deren Status nicht zwischen dem Mindest- und dem Sperrstatus liegen, werden nicht übergeben.
4. Wählen Sie im Menü *Start > Ausführen*, um die Übertragung zu starten.
   Im Bereich *Ausgabe* wird angezeigt, welcher Auftrag und welche Auftragsposition aktuell verarbeitet werden. Die Daten werden als Datei in dem Verzeichnis gespeichert, das Sie im Dialog *Einstellungen-Produktionsübergabe* angegeben haben.
   [Image: Abb. E-10 Produktionsübergabe abgeschlossen]
   *A: Auftragsstatus nach Übergabe*
   *B: Anzahl der übergebenen Positionen*
   Wenn ein Auftrag vollständig verarbeitet wurde, wird der Status umgesetzt. Die Anzahl der nicht übergebenen Aufträge wird in einer Meldung angezeigt.

##### Produktionsübergabe stornieren
Sie können einen Auftrag nach der Übergabe stornieren, damit er nicht produziert wird. Dazu übergeben Sie den Auftrag erneut, setzen dabei aber ein Stornokennzeichen.
- Um einen Auftrag mit der automatischen Produktionsübergabe zu stornieren, müssen die Mengen der Auftragspositionen auf 0 gesetzt werden. Anschließend wird der Auftrag wieder an die Produktion übergeben.
- Danach wird der PPS-Webservice zur Stornierung der Produktionsübergabe automatisch aufgerufen. Der Auftrag wird mit den neuen Werten sofort durch den Workflow-Task übergeben.
- Ist der Statuspunkt *810 Übergabe AW-Pool storniert* einem Anwenderstatus zugeordnet, wird durch die Stornierung der Auftragsstatus auf den gewünschten Anwenderstatus gesetzt, z. B. durch das Heruntersetzen des Status. Ist der Statuspunkt 810 nicht zugeordnet, behält der Auftrag den bisherigen Status.
- Eine Stornierung ist nur bis zur Bestellübergabe möglich.

> **Beispiel**
> Ein Auftrag, der an die Produktion übergeben wurde, hat Status 40. Eine Stornierung verändert den Status nicht. Nach der Änderung der Menge erhält der Auftrag ein Stornokennzeichen und wird daher sofort von der automatischen Produktionsübergabe durch den Workflow-Task übergeben.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
- "So stornieren Sie die Produktionsübergabe manuell" auf Seite E-40
- "So stornieren Sie die Produktion, wenn Sie Aufträge automatisch übergeben" auf Seite E-41

**So stornieren Sie die Produktionsübergabe manuell**
Sie können einen manuell übergebenen Auftrag nach der Übergabe vollständig stornieren, damit er nicht produziert wird. Dazu übergeben Sie den Auftrag erneut manuell, setzen dabei aber ein Stornokennzeichen.
1. Stellen Sie den Auftrag, den Sie stornieren wollen, in einen neuen Nummernverwalter.
2. Wählen Sie im Menü *Fertigung > Produktion > Übergabe Produktion*. Der Dialog *Übergabe Produktion* wird geöffnet.
3. Wählen Sie den Nummernverwalter aus, in dem der Auftrag steht.
   [Image: Abb. E-11 Auftrag stornieren]
   *A: Nummernverwalter mit dem Auftrag, der storniert werden soll*
   *B: Kennzeichen zur Stornierung*
4. Wählen Sie den Modus **Stornieren** (B).
5. Wählen Sie im Menü *Start > Ausführen*, um die Stornierung zu starten.
   Die Daten werden mit einem Storno-Kennzeichen als Datei im angegebenen Verzeichnis gespeichert. Der Status des Auftrags wird auf *Übergabe Produktion storniert* umgesetzt.

**So stornieren Sie die Produktion, wenn Sie Aufträge automatisch übergeben**
1. Öffnen Sie den Auftrag und wechseln Sie zum Register *Positionen*.
2. Markieren Sie die Position, die Sie stornieren wollen.
   - Wenn Sie z. B. die Stückzahl ändern wollen, fahren Sie mit Schritt 3 fort.
   - Wenn Sie die gesamte Position stornieren wollen, dann wählen Sie im Menü *Bearbeiten > Löschen* und fahren Sie mit Schnitt 5 fort.
   [Image: Abb. E-12 Übergebene Position stornieren]
3. Wählen Sie im Menü *Funktionen > Gruppe Position > Gesperrte Position ändern*. Das Eingabefeld *Stück* wird freigeschaltet.
4. Tragen Sie die neue Stückzahl ein.
5. Wählen Sie im Menü *Start > Speichern*, um die Änderung zu speichern.
6. Wiederholen Sie die Schritte 2 bis 5 für alle Positionen, die geändert werden sollen.
7. Schließen Sie die Positionserfassung und den Auftrag.
   Der geänderte Auftrag wird durch den Workflow-Task automatisch an die Produktion übergeben.

##### Übungen
- Richten Sie einen Nummernverwalter ein, in dem Sie Aufträge sammeln, die an Sie die Produktion übergeben wollen.
- Übergeben Sie die Aufträge manuell an die Produktion.
- Prüfen Sie, ob der Status aller Aufträge im Nummernverwalter umgesetzt ist.
- Prüfen Sie, warum einige Aufträge nicht übergeben wurden. Ist bei diesen Aufträgen der Mindeststatus erreicht?

> **Ergänzende Informationen**
> ⇨ Stammdaten, "Firmendaten - Produktion" auf Seite B-1000
> ⇨ Softwarereferenz, "Übergabe Produktion" auf Seite E-170
> ⇨ Softwarereferenz, "Einstellungen Produktionsübergabe" auf Seite E-174

#### Produktionsübergabe mit A+W Business Kapazitätsplanung
**Lernziele**
- Einstellungen zur Übergabe an die A+W Business Kapazitätsplanung kennenlernen.

**Nutzen**
- Die Auftragsdaten aus A+W Business werden automatisch zuerst an die Kapazitätsplanung übergeben.
- Terminverschiebungen aufgrund von Kapazitätsengpässen werden nach der Bestätigung durch den Auftragserfasser in den Auftrag zurückgeschrieben.
- Bei der automatischen Übergabe per Workflow-Task werden die Aufträge nach einem definierten Intervall zunächst an die Kapazitätsplanung übergeben. Nach der erfolgreichen Einlastung werden sie automatisch an die Produktion übergeben.

**Merke**
- **Auftragsstatus**: Statusprüfungen vor der Übergabe verhindern, dass Aufträge mit falschem Status übergeben werden.
- **Nummernkreis**: Die Nummernkreise für Aufträge und Angebote müssen getrennt sein, damit sich die Dokumente bei der Übergabe nicht gegenseitig überschreiben.
- **Übergabe an die Kapazitätsplanung**: Für die Planung der Kapazitäten werden die Daten im OrderXML-Format übergeben. Dazu muss der ERP-Webservice eingerichtet sein.
- **Voreinstellungen**:
  - **Firmendaten**:
    - Register *Produktion*
    - Register *Kapa-Planung*
    - Register *Produktion > Einstellungen Aufträge*
  - **Stammdaten**:
    - *Firma > Customizing > Register Workflow Tasks*

> **Beschreibung der Einstellungen**
> Die grundlegenden Einstellungen und Funktionen sind in der Einheit *Produktionsübergabe ohne Kapazitätsplanung* erklärt worden. In dieser Lerneinheit werden daher nur die Unterschiede oder zusätzlichen Einstellungen behandelt, die für die Übergabe an die A+W Business Kapazitätsplanung gelten.
> ⇨ "Produktionsübergabe ohne Kapazitätsplanung" auf Seite E-25

##### Einstellungen in den Firmendaten
Die Einstellungen für die Datenübergabe können nur von einem Mitarbeiter mit Administratorrechten eingerichtet werden.
Für die Produktionsübergabe mit der A+W Business Kapazitätsplanung müssen Sie folgende Einstellungen prüfen:
- Einstellungen für die automatische Produktionsübergabe. Diese Einstellungen haben Sie bereits kennengelernt.
  ⇨ "So prüfen Sie die Einstellungen in den Firmendaten" auf Seite E-32
- Aktivierung der A+W Business Kapazitätsplanung
- Voreinstellungen der Parameter.

In dieser Einheit lernen Sie, wie Sie die Einstellungen für die Produktionsübergabe mit A+W Business Kapazitätsplanung prüfen. Die Beschreibung bezieht die Einstellungen für den Workflow-Task mit ein. Die Übergabe kann jedoch auch manuell ausgelöst werden.

> **Geänderte Einstellungen können schwerwiegende Fehler erzeugen**
> In der Regel werden die Einstellungen für die Produktionsübergabe bei der Installation von A+W Business auf die Bedingungen im Betrieb abgestimmt. Wenn Sie diese Einstellungen ändern, greifen Sie tief in die Funktionalität der Produktionsübergabe ein. Das kann zu schwerwiegenden Fehlern führen, so dass die Daten von Aufträgen und Angeboten nicht mehr übergeben werden können.
> Die Beschreibung der Einstellungen dient also in erster Linie dazu, Ihnen die Vorgänge deutlicher zu machen und ggf. bei Rücksprachen mit dem Service der A+W Software GmbH Fragen zu den Einstellungen schnell beantworten zu können.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
- "So prüfen Sie die Einstellungen für die Produktionsübergabe mit A+W Business Kapazitätsplanung" auf Seite E-45
- "So prüfen Sie die Voreinstellungen für die Produktionsübergabe" auf Seite E-46

**So prüfen Sie die Einstellungen für die Produktionsübergabe mit A+W Business Kapazitätsplanung**
1. Wählen Sie im Menü *Stammdaten > Firma > Firmendaten* und wechseln Sie zum Register *Kapa-Planung*.
   [Image: Abb. E-13 Stammdaten – Einstellungen für Produktionsübergabe mit A+W Business Kapazitätsplanung]
   *A: Kapazitätsplanung auswählen*
   *B: Empfänger für Fehlermeldungen festlegen*
   ⇨ Stammdaten, "Firmendaten – Kapa-Planung" auf Seite B-1011
2. Wählen Sie im Bereich *Kapazitätsplanung* (A) die Version **0-Kapazitätsplanung** aus.
3. Markieren Sie im Bereich *Fehlermeldung aus autom. Kapazitätsplanung* eine der Optionen:
   - **An Auftragserfasser**: Mit dieser Einstellung werden die Fehlermeldungen an den Mitarbeiter gesendet, der den jeweiligen Auftrag erfasst hat. Solche Fehlermeldungen beziehen sich in aller Regel auf Termine, die nicht eingehalten werden können, weil nicht genügend Kapazitäten zur Verfügung stehen.
   - **An Mitarbeiter**: Mit dieser Einstellung wird das Feld für die Auswahl eines Mitarbeiters freigeschaltet. Wählen Sie diese Option, wenn nur ein einziger Mitarbeiter die Aufträge bearbeitet, die nicht problemlos eingelastet werden konnten.
4. Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern. Die Einstellungen im Bereich *A+W Business-Kapazitätsplanung* lernen Sie in einer gesonderten Schulung zur Kapazitätsplanung kennen.

**So prüfen Sie die Voreinstellungen für die Produktionsübergabe**
1. Klicken Sie im Dialog *Firmendaten > Register Produktion* auf **[Einstellungen Aufträge]**.
   [Image: Abb. E-14 Produktionsübergabe für Aufträge]
   *A: Auswahl des Übertragungsformats*
   *B: Einstellung für CAD Designer (Bars)-Übergabe*
   *C: Auswahl der OrderXML-Version*
   *D: Statusprüfung vor Übergabe*
2. Wählen Sie im Bereich *Modus der Übergabe* die Option (D) **Nach Mindest- und Sperrstatus Produktionsübergabe**. Für die automatische Produktionsübergabe wird der Auftragsstatus mit dem Mindest- und Sperrstatus für die Produktionsübergabe verglichen. Liegt der Auftragsstatus dazwischen, wird der Auftrag automatisch an die Produktion übergeben. Dies ist die Standardeinstellung.
3. Klicken Sie auf **[OK]**, um die Änderung zu übernehmen.

#### Produktionsübergabe mit A+W Production Capacity Planner
**Lernziele**
- Einstellungen zur Übergabe an A+W Production Capacity Planner kennenlernen.

**Nutzen**
- Die Auftragsdaten aus A+W Business werden automatisch zuerst an A+W Production Capacity Planner übergeben.
- Terminverschiebungen aufgrund von Kapazitätsengpässen werden nach der Bestätigung durch den Auftragserfasser in den Auftrag zurückgeschrieben.
- Bei der automatischen Übergabe per Workflow-Task werden die Aufträge nach einem definierten Intervall zunächst an die Kapazitätsplanung übergeben. Nach der erfolgreichen Einlastung werden sie automatisch an die Produktion übergeben.

**Merke**
- **Auftragsstatus**: Statusprüfungen vor der Übergabe verhindern, dass Aufträge mit falschem Status übergeben werden.
- **Nummernkreis**: Die Nummernkreise für Aufträge und Angebote müssen getrennt sein, da sonst auch Angebote an A+W Production Capacity Planner übergeben werden.
- **Übergabe an die Kapazitätsplanung**: Für die Planung der Kapazitäten werden die Daten im OrderXML-Format übergeben. Dazu muss der ERP-Webservice eingerichtet sein.
- **Voreinstellungen**:
  - **Firmendaten**:
    - Register *Produktion*
    - Register *Kapa-Planung*
    - Register *Produktion > Einstellungen Aufträge*
  - **Stammdaten**:
    - *Firma > Customizing > Register Workflow Tasks*

> **Beschreibung der Einstellungen**
> Die grundlegenden Einstellungen und Funktionen sind in der Einheit *Produktionsübergabe ohne Kapazitätsplanung* erklärt worden. In dieser Lerneinheit werden daher nur die Unterschiede oder zusätzlichen Einstellungen behandelt, die für die Übergabe an A+W Production Capacity Planner gelten.
> ⇨ "Produktionsübergabe ohne Kapazitätsplanung" auf Seite E-25

##### Einstellungen für A+W Production Capacity Planner
Die Einstellungen für die Datenübergabe können nur von einem Mitarbeiter mit Administratorrechten eingerichtet werden.
Für die Produktionsübergabe mit der A+W Production Capacity Planner müssen Sie folgende Einstellungen prüfen:
- Einstellungen für die automatische Produktionsübergabe. Diese Einstellungen haben Sie bereits kennen gelernt.
  ⇨ "So prüfen Sie die Einstellungen in den Firmendaten" auf Seite E-32
- Aktivierung der A+W Production Capacity Planner
- Voreinstellungen der Parameter.

In dieser Einheit lernen Sie, wie Sie die Einstellungen für die Produktionsübergabe mit A+W Production Capacity Planner prüfen. Die Beschreibung bezieht die Einstellungen für den Workflow-Task mit ein. Die Übergabe kann jedoch auch manuell ausgelöst werden.

> **Geänderte Einstellungen können schwerwiegende Fehler erzeugen**
> In der Regel werden die Einstellungen für die Produktionsübergabe bei der Installation von A+W Business auf die Bedingungen im Betrieb abgestimmt. Wenn Sie diese Einstellungen ändern, greifen Sie tief in die Funktionalität der Produktionsübergabe ein. Das kann zu schwerwiegenden Fehlern führen, so dass die Daten von Aufträgen und Angeboten nicht mehr übergeben werden können.
> Die Beschreibung der Einstellungen dient also in erster Linie dazu, Ihnen die Vorgänge deutlicher zu machen und ggf. bei Rücksprachen mit dem Service der A+W Software GmbH Fragen zu den Einstellungen schnell beantworten zu können.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
- "So aktivieren Sie die Übergabe an A+W Production Capacity Planner" auf Seite E-49
- "So prüfen Sie die Voreinstellungen für die Produktionsübergabe" auf Seite E-51

**So aktivieren Sie die Übergabe an A+W Production Capacity Planner**
1. Wählen Sie im Menü *Stammdaten > Firma > Firmendaten* und wechseln Sie zum Register *Kapa-Planung*.
   [Image: Abb. E-15 Stammdaten – Einstellungen für Produktionsübergabe A+W Production Capacity Planner]
   *A: Version auswählen*
   *B: Empfänger für Fehlermeldungen festlegen*
   *C: Einstellungen für die Kapazitätsplanung*
   ⇨ Stammdaten, "Firmendaten - Kapa-Planung" auf Seite B-1004
2. Wählen Sie im Bereich *Kapazitätsplanung* (A) die Version **1-A+W Production Capacity Planning** aus.
3. Markieren Sie im Bereich *Fehlermeldungen aus autom. Kapazitätsplanung* eine der Optionen:
   - **An Auftragserfasser**: Mit dieser Einstellung werden die Fehlermeldungen an den Mitarbeiter gesendet, der den jeweiligen Auftrag erfasst hat. Solche Fehlermeldungen beziehen sich in aller Regel auf Termine, die nicht eingehalten werden können, weil nicht genügend Kapazitäten zur Verfügung stehen.
   - **An Mitarbeiter**: Mit dieser Einstellung wird das Feld für die Auswahl eines Mitarbeiters freigeschaltet. Wählen Sie diese Option, wenn nur ein einziger Mitarbeiter die Aufträge bearbeitet, die nicht problemlos eingelastet werden konnten.
4. Markieren Sie im Bereich *A+W Production-Kapazitätsplanung* die Option für die Planungsrückmeldungen:
   - **Angebot oder Auftrag wird gesucht**: Angebote und Aufträge werden auf die gleiche Weise in die Kapazitätsplanung eingelastet. Wenn Sie diese Option wählen, müssen Sie Angebote, die zur Optimierung übergeben wurden, manuell stornieren, damit sie nicht gefertigt werden.
   - **Immer als Auftrag (muss bei kapazitativer Übergabe aktiv sein)**: Mit dieser Einstellung werden nur die Aufträge in die Kapazitätsplanung eingelastet. Dies ist die Standardeinstellung. Wenn Sie versuchen, ein Angebot manuell zu übergeben, ist die Funktion blockiert.
5. Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern.
6. Wechseln Sie zum Register *Produktion* und prüfen Sie die Einstellungen für die Datenübertragung durch den A+W Business Interface Service. Diese Einstellungen sind ausführlich in der Einheit für die A+W Business Kapazitätsplanung behandelt.
   ⇨ "Einstellungen in den Firmendaten" auf Seite E-44
   Die Einstellungen im Bereich *A+W Production-Kapazitätsplanung* lernen Sie in einer gesonderten Schulung zur Kapazitätsplanung kennen.

**So prüfen Sie die Voreinstellungen für die Produktionsübergabe**
1. Klicken Sie im Dialog *Firmendaten > Register Produktion* auf **[Einstellungen Aufträge]**.
2. Prüfen Sie die Einstellungen, wie in der Einheit *Manuelle Produktionsübergabe* beschrieben.
   [Image: Abb. E-16 Produktionsübergabe für Aufträge]
   *A: Übergabe an A+W Production Capacity Planner*
3. Wählen Sie im Bereich *Modus der Übergabe* die Option (A):
   **Dokumente im Kapazitätsplanungs-Pool**: Mit dieser Einstellung wird die Kapazitätsplanung durch A+W Production Capacity Planner vor der Übergabe an die Produktion durchgeführt. Sobald ein Auftrag neu erfasst oder geändert wird, landet er im Pool für die Kapazitätsplanung. Wenn die automatische Produktionsübergabe aktiviert ist, wird ein Auftrag in diesem Pool automatisch übergeben. Nach der Übergabe wird der Auftrag aus diesem Pool entfernt. Bei dieser Einstellung ist die Angebotsoptimierung nicht möglich.
4. Klicken Sie auf **[OK]**, um die Daten zu speichern. Die Daten werden gespeichert.

#### Übergabe zur Angebotsoptimierung
**Lernziele**
- Übergabe von Angeboten zur Optimierung des Zuschnitts.
- Unterschiede zur Produktionsübergabe kennenlernen.

**Nutzen**
Wenn Sie seltene Gläser in einem Angebot erfasst haben, können Sie das Dokument zur Optimierung an die Produktion übergeben. Nach der Berechnung der Anzahl der benötigten Lagerplatten und des tatsächlichen Verschnitts können Sie die Preise für das Angebot prüfen und entsprechend korrigieren.

**Merke**
- **Angebotsoptimierung**: Übergebene Angebote werden nicht produziert.
- **Rückmeldungen**: Rückmeldungen über die Anzahl der verschnittenen Lagerplatten müssen Sie mündlich von dem zuständigen Sachbearbeiter in der Produktion einholen.
- **Nummernkreis**: Die Nummernkreise für Aufträge und Angebote müssen getrennt sein, damit sich die Dokumente bei der Übergabe nicht gegenseitig überschreiben.
- **Voreinstellungen**:
  - **Stammdaten**:
    - *Auftrag > Nummernkreise*
  - **Firmendaten**:
    - *Register Produktion*
    - *Register Produktion > Einstellungen Angebot*

> **Angebot mit aktivierter A+W Production Capacity Planner**
> Sie können Angebote nur zur Optimierung an die Produktion übergeben, wenn Sie ohne Kapazitätsplanung oder mit der A+W Business Kapazitätsplanung arbeiten. Die Funktion ist blockiert, wenn die Produktionsübergabe von Angeboten per Workflow-Task aktiviert wird.

##### Optimierung von Angeboten
Wenn Sie in einem Angebot seltene Gläser erfasst haben, ist es besonders wichtig, den Verkaufspreis so zu bestimmen, dass keine Verluste erwirtschaftet werden. Sie können dazu das Angebot an die Produktion übergeben, um den Zuschnitt zu planen und so den Glasbedarf und Verschnitt zu ermitteln.
Dabei werden die Angebote mit einem Angebotskennzeichen an die Produktion übergeben. Die Positionen des Angebots werden nicht produziert.
Für Angebote werden keine Rückmeldungen erzeugt. Nach der Optimierung müssen Sie die Anzahl der verschnittenen Lagerplatten mündlich oder schriftlich von dem zuständigen Sachbearbeiter in der Produktion einholen. Diese Auskünfte dienen Ihnen dazu, den Verkaufspreis im Angebot oder anschließend im Auftrag besser kalkulieren.

> **Übergabe per Workflow-Task**
> In der Regel werden die Angebote durch einen eigenen Workflow-Task übergeben. Diese Form der Übergabe unterscheidet sich nicht von der Übergabe der Aufträge.
> ⇨ "Produktionsübergabe per Workflow-Task" auf Seite E-26

##### Angebotsübergabe einrichten
Die Übergabe von Angeboten zur Optimierung wird genauso eingerichtet, wie die Produktionsübergabe von Aufträgen. Das Vorgehen haben Sie bei der Produktionsübergabe für Aufträge kennengelernt.
Bei der OrderXML-Übergabe können Sie die Übergabe von Angeboten identisch zu den Aufträgen festlegen. Mit der Übergabe wird auch ein Kennzeichen übergeben, anhand dessen die Unterscheidung zwischen Angebot und Auftrag möglich ist.

> **Allgemeine Einstellung**
> Die meisten Einstellungen für die Angebotsoptimierung unterscheiden sich nicht von denen der Übergabe von Aufträgen. In dieser Handlungssequenz werden nur die Einstellungen beschrieben, die ausschließlich für die Angebote gelten.
> ⇨ "So prüfen Sie die Voreinstellungen für die Produktionsübergabe" auf Seite E-33

**So prüfen Sie die Voreinstellungen für die Angebotsoptimierung**
1. Klicken Sie im Dialog *Firmendaten > Register Produktion* auf **[Einstellungen Angebote]**.
   [Image: Abb. E-17 Angebotsoptimierung]
   *A: Einstellung für die Übergabe von Angeboten*
   ⇨ Softwarereferenz, "Übergabe Produktion" auf Seite E-170
2. Prüfen Sie die Einstellungen, wie in der Einheit *Manuelle Produktionsübergabe* beschrieben.
3. Achten darauf, dass im Bereich *Modus der Übergabe* die Option **nach Mindest- und Sperrstatus Produktionsübergabe (A)** eingestellt ist.
   Wenn Sie die Angebote auch in die Kapazitätsplanung übergeben, werden die entsprechenden Kapazitäten reserviert, ohne dass die Positionen anschließend produziert werden. Damit würden Maschinenzeiten blockiert, die dann nicht für die Produktion genutzt werden können.
4. Klicken Sie auf **[OK]**, um die Daten zu speichern. Die Daten werden gespeichert.

##### Angebote an die Produktion übergeben
In diesem Abschnitt lernen Sie, wie Sie ein Angebot manuell zur Optimierung an die Produktion übergeben. Dabei wird der Zuschnitt berechnet, ohne dass die Positionen produziert werden.
Die Handlungsschritte für die Übergabe von Angeboten entsprechen denen für die Übergabe von Aufträgen.

**So übergeben Sie die Angebotsdaten manuell zur Optimierung**
1. Wählen Sie im Menü *Fertigung > Produktion > Angebotsoptimierung > Übergabe Produktion*.
   [Image: Abb. E-18 Produktionsübergabe – Angebotsübergabe starten]
   *A: Nummernverwalter mit Angeboten*
   *B: Modus Kostenkalkulation*
   ⇨ Softwarereferenz, "Übergabe Produktion" auf Seite E-170
2. Wählen Sie den Nummernverwalter (A) aus, in den Sie das Angebot für die Optimierung gestellt haben.
3. Prüfen Sie, ob der Modus **Kostenkalkulation** (B) eingestellt ist.
4. Wählen Sie im Menü *Start > Ausführen*, um die Übertragung zu starten.
   Im Bereich *Ausgabe* wird angezeigt, welche Angebotsposition aktuell verarbeitet wird. Die Daten werden als Datei in dem Verzeichnis gespeichert, das Sie im Dialog *Einstellungen-Produktionsübergabe* angegeben haben.
   Wenn Sie mehr als ein Angebot übergeben haben, wird die Anzahl der nicht übergebenen Angebote in einer Meldung angezeigt.
   Pro Angebot wird eine OrderXML-Datei erstellt. Dem Dateinamen werden die Angebotsnummer und ein Zeitstempel angefügt. Bei der AWPool-Übergabe werden alle Daten in eine einzige Datei geschrieben.
   Der Status der übergebenen Angebote wird umgesetzt.
   Nach der Optimierung müssen Sie sich über den Verbrauch der Lagerplatten beim zuständigen Sachbearbeiter in der Produktion informieren.

##### Übungen
- Richten Sie einen Nummernverwalter ein, in dem Sie Angebote sammeln, die Sie zur Optimierung übergeben wollen.
- Erstellen Sie einige unterschiedliche Angebote.
- Übergeben Sie die Angebote.

> **Ergänzende Informationen**
> ⇨ Stammdaten, "Firmendaten – Lager/EK/EDI" auf Seite B-970
> ⇨ Softwarereferenz, "Übergabe Produktion" auf Seite E-170
> ⇨ Softwarereferenz, "Einstellungen Produktionsübergabe" auf Seite E-174

### Rückmeldungen aus der Produktion
In diesem Themenblock lernen Sie die Rückmeldungen aus der Produktion kennen. Dazu lernen Sie, wie Sie A+W Business so einrichten, dass Sie die Rückmeldungen empfangen können.
Dazu gehören folgende Lerneinheiten:
- "Produktionsrückmeldungen per Datei" auf Seite E-59
- "Dateilose Produktionsrückmeldung" auf Seite E-70
- "A+W Business Interface Service" auf Seite E-79

#### Produktionsrückmeldungen
Produktionsrückmeldungen dienen in A+W Business dazu, Informationen über den Fortgang der Produktion zu liefern. Durch die Rückmeldungen wird der Status von Positionen und von Aufträgen aktualisiert.
Rückmeldungen können auf folgende Arten erstellt und eingelesen werden:
- **Rückmeldedatei**: Die Rückmeldedateien werden vom A+W Production erstellt und durch den A+W Business-Interface-Service eingelesen. Dieses Programm läuft zentral auf dem Server und prüft periodisch die definierten Verzeichnisse nach Neueingängen.
- **Dateilose Rückmeldung**: A+W Business ruft die Daten online aus A+W Production ab. Diese Online-Abfrage ist zeit- und mengengenau und gibt den genauen Produktionsstand eines Auftrags wieder.

#### Produktionsrückmeldungen per Datei
**Lernziele**
- Rückmeldedateien kennenlernen.
- Grundverständnis der Betriebsdatenerfassung.
- Einrichten von Erfassungsstellen für Produktionsrückmeldungen aus A+W Production.
- Einrichten der Übertragungswege für die Rückmeldedateien.

**Nutzen**
- Erfassungsstellen ermöglichen, den Produktionsfortgang zu überwachen und damit den jeweiligen Status eines Auftrags bzw. der Auftragspositionen zu prüfen.
- Übersichten über den Status von Positionen und Aufträgen können pro Erfassungsstelle angezeigt werden.
- Versandpapiere können zeitnahe gedruckt werden.

**Merke**
- **Erfassungsstelle**: Eine Erfassungsstelle (ES) ist ein Ort in der Produktion, an dem ein Produktionsschritt erfasst wird, z. B. der Zuschnitt der ersten Scheibe eines Auftrags. In A+W Business wird diesen ES ein Statuspunkt zugeordnet, so dass durch die Rückmeldungen der jeweiligen ES den Auftragsstatus umgesetzt wird.
- **Betriebsdatenerfassung**: Mit der Betriebsdatenerfassung (BDE) von A+W Production wird jeder einzelne Auftrag im Verlauf der Produktion überwacht.
- **Rückmeldung aus A+W Production**: Rückmeldungsdateien von A+W Production werden auf einen Server gestellt und von A+W Business ausgewertet.
- **Intervall zum Einlesen der Dateien**: Die Rückmeldedateien werden vom A+W Business-Interface-Service eingelesen. Das Intervall können Sie selbst festlegen.
- **Voreinstellungen**:
  - **Stammdaten**:
    - Erfassungsstellen Produktion
    - Schnittstellendienst
  - **Firmendaten**:
    - Register Lager/EK/EDI
    - Register Produktion

##### Rückmeldedateien
In A+W Production werden an allen wichtigen Stellen im Produktionsfluss die Daten von Erfassungsstellen (ES) erfasst und als Rückmeldedateien gesendet. Diese Produktionsrückmeldungen dienen in A+W Business dazu, den Produktionsfortgang zu überwachen. Damit können Sie den jeweiligen Status eines Auftrags prüfen.
Diese Dateien können in zwei unterschiedlichen Formaten gesendet werden:
- STS*.ASC-Dateien von den Erfassungsstellen
- AWB_STAT-Dateien aus der Betriebsdatenerfassung (BDE)

Zusätzlich zu den Erfassungsstellen in A+W Business können nach Absprache mit A+W Production weitere Erfassungsstellen angelegt werden, z. B. Zuordnungen zu Maschinen. Diese werden i. d. R. per STSD-Datei an A+W Business gemeldet. Das Kennzeichen solcher Erfassungsstellen muss größer 200 sein, damit es ordnungsgemäß verarbeitet wird.

| A+W Production-Datei | Rückmeldung aus | Aktion in A+W Business |
| :--- | :--- | :--- |
| **STSP** | Produktion, z. B. A+W Production-ES 600, 700, 800 und 900 | Die Rückmeldung erfolgt überwiegend pro Stück. In A+W Business kann eingestellt werden, ob der Status schon bei der ersten Scheibe oder erst bei Rückmeldung aller Scheiben des Auftrages hochgesetzt werden soll. |
| **STSL** | Planung, z. B. ES 0, 100, 150 und 200 | Sobald eine neue Auftragsnummer in A+W Production eingelesen wurde, wird der Auftrag in A+W Business auf den Status gesetzt, der in A+W Business der Erfassungsstelle zugeordnet ist. Bei Erfassungsstelle 0 wird der Status zurückgesetzt auf den in der Statusverwaltung angelegten Wert. Ist eine Erfassungsstelle aufgeführt, der kein Status zugeordnet ist, erfolgen die Verarbeitung und die Umsetzung des Status in der Zeitwirtschaft. |
| **STSD** | BDE, z. B. von Aggregaten | Die BDE-Rückmeldung dient im A+W Business dazu den Auftragsstatus, das Produktionsdatum und die Kopf- bzw. Positionslaufnummer zu aktualisieren. Die Rückmeldung erfolgt überwiegend pro Stück. In A+W Business kann eingestellt werden, ob der Status schon bei der ersten Scheibe oder erst bei Rückmeldung aller Scheiben des Auftrages hochgesetzt werden soll. Ist eine Erfassungsstelle aufgeführt, der kein Status zugeordnet ist, erfolgen die Verarbeitung und die Umsetzung des Status in der Zeitwirtschaft. |
| **STSG** | Gestell, ES 900 | Die Rückmeldung der Erfassungsstelle 900 gibt an, dass das Gestell unter dem angegebenen Datum als ausgeliefert verbucht ist. |
| **STSK** | Gestell | Nach einer Überprüfung, ob das Gestell existiert oder nicht, wird abhängig von der Erfassungsstelle das Gestell gebucht. Existiert das Gestell noch nicht, wird es zuvor angelegt. Die ES kann folgende Werte haben: 10: außer Haus, Erstmeldung; 20: außer Haus, Änderung; 40: Gestell im Haus. Bei 10 und 20 wird das Ausgabedatum aktualisiert, bei 40 das Rücknahmedatum. Die Kundennummer wird immer aktualisiert. |
| **STSB** | | Mit dieser Rückmeldung werden die Reklamationen und die bei der Produktion zu Bruch gegangenen Scheiben gesendet. A+W Business erstellt daraus Reklamationsaufträge. |
*Tab. E-1: Beispiele für Rückmeldedateien von Erfassungsstellen*

Wenn STSP, STSL, STSD, STSB, STSG im Einsatz sind, muss in den Firmendaten eine Erfassungsstelle ausgewählt werden, die einem Statuspunkt zugewiesen ist. Wenn eine solche Erfassungsstelle nicht zugewiesen wurde, erzeugt die Rückmeldung einen Fehler.
Die Rückmeldungen aus der Feinplanung und von produzierten Einheiten werden in A+W Business in separate Datenbanktabellen mit den entsprechenden Feldern, z. B. pro Auftrag, Position und Stücklisten-ID, geschrieben.
Die fertigen Positionen werden in A+W Production über Barcode eingelesen. Diese Information wird als Rückmeldung an A+W Business weitergeleitet und dadurch der A+W Business-Positionsstatus erhöht.

##### Erfassungsstellen für Produktionsrückmeldungen
Erfassungsstellen (ES) in A+W Production überwachen den Stand der Produktion und senden Rückmeldung an A+W Business. Diese werden über den A+W Business Interface Service eingelesen.
In A+W Business wird den Erfassungsstellen jeweils ein Statuspunkt zugeordnet, so dass die Rückmeldungen je nach ES den Status der Position oder des Auftrags umsetzen.
Produktionsrückmeldungen werden standardmäßig von folgenden Erfassungsstellen erwartet:

| Erfassungsstelle = A+W Production-Status | Bedeutung |
| :--- | :--- |
| 0 | unverplant |
| 100 | in Lauf verplant |
| 150 | Feinplanung |
| 200 | Freigabe zur Produktion |
| 300 | in Produktion |
| 350 | Bruch in Produktion |
| 700 | produziert |
| 800 | versandfertig |
| 900 | ausgeliefert |

Damit ist in A+W Business ein Überblick über den Stand der gefertigten Positionen bzw. Aufträge möglich. Die Informationen aus den Rückmeldungen zeigen pro Position mindestens den Positionsstatus, die gefertigte Menge und das Datum. Weiteren Daten werden je nach Typ der Datei zurückgemeldet.
Für Aufträge bzw. Teilaufträge, die komplett fertig gemeldet wurden und zum Versand bereitstehen, kann der Druck von Versandpapieren zeitnah angestoßen werden.

##### Erfassungsstelle zuordnen
Wenn Sie die Rückmeldungen aus A+W Production in A+W Business auswerten wollen, müssen Sie den Erfassungsstellen einen Statuspunkt zuordnen und die entsprechenden Daten im Schnittstellen-Dienst anpassen. Diese Zuordnungen werden für Produktionsrückmeldungen und BDE-Rückmeldungen benötigt.
In diesem Abschnitt lernen Sie, wie Sie für die Rückmeldungen von einer Erfassungsstelle in A+W Production einen Statuspunkt zuordnen. Wie Sie die Schnittstellen einrichten, erfahren Sie in der nächsten Lerneinheit.

**So ordnen Sie eine Erfassungsstelle für die Rückmeldung per Datei zu**
1. Wählen Sie im Menü *Stammdaten > Fertigung > Erfassungsstellen Produktion*. Der gleichnamige Dialog wird geöffnet.
2. Wählen Sie im Menü *Start > Neu*, um in den Erfassungs-Modus zu wechseln.
   [Image: Abb. E-19 Erfassungsstelle für Produktionsrückmeldungen zuordnen]
   *A: Bezeichnung*
   *B: Statuspunkte, die in A+W Business angelegt sind.*
   *C: Nummer der Erfassungsstelle in A+W Production*
   *D: Typ der Datei, die aus A+W Production gesendet wird.*
   *E: Zeitpunkt der Statuserhöhung*
   *F: Kennzeichnung: ES für Bestellungen*
3. Geben Sie die Bezeichnung (A) der Erfassungsstelle von A+W Production ein. Geben Sie z. B. eine Erfassungsstelle an, mit der Sie einen Auftrag als ausgeliefert melden können.
4. Wählen Sie den Statuspunkt (B) und den Typ (D) aus. Die möglichen Einträge in diesen Spalten sind in Auswahllisten hinterlegt, die Sie mit einem Klick in die jeweilige Zelle öffnen können.
5. Wählen Sie den Zeitpunkt der Statuserhöhung (E) aus:
   - **0 - erste Scheibe fertig**: Der Status wird erhöht, wenn die erste Scheibe des Auftrags fertig gemeldet wurde.
   - **1 - erste Position fertig**: Der Status wird erhöht, wenn die gesamte erste Position des Auftrags fertig gemeldet wurde.
   - **2 - alle Scheiben fertig**: Der Status wird erhöht, wenn alle Scheiben des Auftrags fertig gemeldet wurden.
6. Wenn Sie einen Statuspunkt einer Erfassungsstelle zuordnen, der den Wareneingang von Bestellartikeln zurückmeldet, müssen Sie die Checkbox **Bestellkennzeichen** (F) markieren.
7. Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern. Die Daten werden gespeichert.
8. Wiederholen Sie ggf. die Schritte 2 bis 7, um weitere Erfassungsstellen zuzuordnen.
   Wenn Sie die Erfassungsstelle aus der Produktion zugeordnet haben, müssen Sie diese auch im Schnittstellen-Dienst in den Einstellungen für Rückmeldungen angeben.
   ⇨ "Einstellungen für Schnittstellen festlegen" auf Seite E-66

##### Einstellungen in den Firmendaten festlegen
In den Firmendaten müssen Sie die Einstellungen für die Produktionsrückmeldung prüfen. Die URL des ERP-Webservice ist für Produktionsübergabe und Produktionsrückmeldung im OrderXML-Format gültig. Diese Einstellungen sind im Themenblock Produktionsübergabe ausführlich beschrieben.
⇨ "So prüfen Sie die Einstellungen in den Firmendaten" auf Seite E-32

**So ordnen Sie die Erfassungsstelle für Fertigmeldungen zu**
1. Wählen Sie im Menü *Stammdaten > Firma > Firmendaten* und wechseln Sie zum Register *Lager / EK / EDI*.
   [Image: Abb. E-20 Stammdaten – Erfassungsstelle für Rückmeldung]
   *A: Fertigmeldung bei Rückmeldung von der ausgewählten Erfassungsstelle*
   ⇨ Stammdaten, "Firmendaten - Parameter" auf Seite B-948
2. Wählen Sie im Bereich **Auftrag produziert bei** die Erfassungsstelle aus. Über die gewählte Erfassungsstelle wird bei einer Rückmeldung der jeweilige Auftrag in A+W Business fertig gemeldet.
3. Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern. Die Daten werden gespeichert.

##### Einstellungen für Schnittstellen festlegen
In diesem Abschnitt lernen Sie, wie die Parameter für die Rückmeldedateien eingerichtet werden können.

**So legen Sie die Einstellungen für Rückmeldedateien fest**
1. Wählen Sie im Menü *Stammdaten > Firma > Schnittstellen-Dienst*.
   [Image: Abb. E-21 Schnittstellen-Dienst für Rückmeldungen]
   *A: Mitarbeiter, für den die Einstellungen festgelegt werden.*
   *B: Formate, die aus A+W Production zurückgemeldet werden, z. B. Produktionsrückmeldungen.*
   *C: Fertigmeldung bei Rückmeldung von der ausgewählten Erfassungsstelle.*

> **Gesperrte Felder**
> Die Felder sind gesperrt, wenn im Register *Einstellungen weitere Formate* die Checkbox *Import von Produktionsrückmeldungen* aktiviert ist. Sie können dann keine Einstellungen für A+W Production-Formate festlegen.
> Wenn Sie Rückmeldungen nicht aus A+W Production erhalten, wechseln Sie zum Register *Einstellungen weitere Formate* oder *Optionen*, um die Einstellungen zu prüfen oder festzulegen.

2. Markieren Sie die Checkboxen für die Daten, zu denen Sie Rückmeldungen aus A+W Production empfangen möchten, und wählen Sie das zugehörige Verzeichnis aus, aus dem die Rückmeldedateien von A+W Business ausgelesen werden. Dieselben Verzeichnisse müssen in A+W Production angegeben werden, damit die Dateien korrekt gespeichert werden.
3. Wenn Sie die Einstellungen benutzerspezifisch festlegen wollen, wählen Sie im Feld *Einstellungen für* (A) den gewünschten Benutzer aus. Wenn die Einstellungen für alle Benutzer gelten sollen, wählen Sie den Eintrag **Administrator**. Bei dieser Einstellung muss im Bereich **Auftrag produziert bei** (C) dieselbe Erfassungsstelle ausgewählt sein, wie in den Firmendaten > Register *Lager / EK / EDI*. Wenn Sie die Einstellungen für einen bestimmten Benutzer festlegen, können Sie im Bereich **Auftrag produziert bei** (C) eine abweichende Erfassungsstelle angeben. Über die ausgewählte Erfassungsstelle können die Rückmeldungen folgende (zusätzliche) Aktionen auslösen:
   - Im Auftrag werden das Produktionsdatum und die Laufnummer erhöht.
   - Bei Produktionsaufträgen wird der Warenzugang im Lager gebucht.
4. Wechseln Sie zum Register *Einstellungen weitere Formate*.
   [Image: Abb. E-22 Schnittstellen-Dienst für weitere Formate]
   *A: AWPool-Import*
5. Wenn Sie mit AWPool arbeiten, müssen Sie die Checkbox **Import von AWPool-Dateien** markieren. Die BDE- und ALFERT-Formate können Sie nur übernehmen, wenn Sie im Register *Einstellungen A+W Production-Formate* den Import von Produktionsrückmeldungen nicht aktiviert haben.
6. Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern.
7. Wechseln Sie zum Register *Optionen*, um das Intervall zum Einlesen von Rückmeldedateien anzugeben.
   [Image: Abb. E-23 Schnittstellen-Dienst – Optionen]
   *A: Intervall für Rückmeldedatei*
8. Legen Sie das Intervall (A) für den A+W Business Interface Service fest. Wenn Sie z. B. eine 2 eintragen, prüft der Service alle 2 Minuten, ob neue Rückmeldungen aus der Produktion vorliegen, und liest diese ein.
9. Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern. Die Daten werden gespeichert.

##### Status der Positionen und Aufträge prüfen
Im Dialog *Übersicht Statusrückmeldung* können Sie den zuletzt gemeldeten Produktionsstatus jeder einzelnen Auftragsposition prüfen.

**So prüfen Sie den Status im Auftrag**
1. Wählen Sie im Menü *Dokumente > Auftrag > Auftrag > Menü Ansicht > Gruppe Produktion > Produktionsübersicht*.
   [Image: Abb. E-24 Übersicht Statusrückmeldung – Aktueller Status von Auftragspositionen]
   *A: Aktueller Status pro Position*
   *B: Stückzahl, die versandbereit ist*
   *C: Stückzahl, die fertig gemeldet ist*

   Die Anzeige wird aktualisiert, wenn im nächsten Intervall neue Rückmeldedateien zu diesem Auftrag eingelesen werden.

> **Ergänzende Informationen**
> ⇨ Stammdaten, "Erfassungsstellen Produktion" auf Seite B-882
> ⇨ Stammdaten, "Firmendaten - Lager/EK/EDI" auf Seite B-970
> ⇨ Stammdaten, "Firmendaten - Produktion" auf Seite B-1000
> ⇨ Stammdaten, "Schnittstellen-Dienst" auf Seite B-1046

#### Dateilose Produktionsrückmeldung
**Lernziele**
- Einrichten der Übertragungswege für dateilose Rückmeldungen aus A+W Production.

**Nutzen**
- Der genaue Produktionsfortschritt eines Auftrags wird online aus A+W Production abgerufen und im Dialog *Übersicht Statusrückmeldung* angezeigt.
- Mit der Online-Abfrage lassen sich Fehlfunktionen (fehlende Buchungen, doppelte Buchungen) nahezu ausschließen, so dass es nicht zu Unterschieden im Produktionsfortschritt zwischen A+W Production und der Anzeige in A+W Business kommen kann.

**Merke**
- **Erfassungsstelle**: Auch bei den dateilosen Rückmeldungen müssen in A+W Business Erfassungsstellen in den Stammdaten zugeordnet sein. Alle notwendigen Erfassungsstellen müssen mit dem Typ 1-Sonstige angelegt werden.
- **Online-Rückmeldung aus A+W Production**: Die Rückmeldungen werden von A+W Production über den ERP-Webservice eingelagert und vom A+W Business Interface Service verbucht.
- **Voreinstellungen**:
  - **Stammdaten**:
    - Erfassungsstellen Produktion
  - **Firmendaten**:
    - Register Lager/EK/EDI
    - Register Produktion
  - In A+W Production muss der CommonBase-Schalter WebService statt STS*.ASC benutzen aktiviert sein.