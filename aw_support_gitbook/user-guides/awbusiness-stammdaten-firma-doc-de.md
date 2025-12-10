---
title: "D-AWBusiness-HB_12"
source: "D-AWBusiness-HB_12.pdf"
tags: ["Software Reference", "A+W Business", "Stammdaten", "Firma", "Rechteverwaltung", "Provisionen", "Schnittstellen", "Formulare", "CE-Kennzeichen", "B2B"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for the 'Firma' (Company) and 'B2B' master data sections of the A+W Business software. It provides detailed instructions on configuring user rights, commission structures, interfaces, forms, and B2B data exchange protocols. The guide is intended for administrators and advanced users responsible for system setup and maintenance."
long_description: "This comprehensive software reference manual details the configuration of master data within the A+W Business system, focusing on the 'Firma' (Company) and 'B2B' modules. The 'Firma' section covers fundamental company settings, including the management of user rights ('Rechte'). It explains how to activate or deactivate permissions for changing, inserting, deleting, and executing data, and how to copy these rights between users and groups. It also describes the setup for status management in document workflows, allowing for fine-grained control over document state changes. The manual outlines the configuration of various organizational areas such as 'AV-Bereiche' (work preparation areas) and 'AD-Bereiche' (sales areas), and provides an in-depth guide to setting up sales representative commissions ('Vertreterprovision'), including different commission types and calculation bases. Furthermore, it covers the management of company bank details, branches, booking periods, and product surcharges. A significant portion is dedicated to the 'Schnittstellen-Dienst' (Interface Service), detailing the setup for data exchange with A+W Production and other external systems. This includes configuring feedback for production, planning, machine data, and breakage, as well as interfaces for financial accounting. The 'Formulare' (Forms) section explains the administration of print templates for documents like order confirmations, invoices, and delivery notes. It also touches on the setup for CE and CEKAL certifications, which are crucial for compliance in specific markets. The 'B2B' section outlines the configuration for electronic data interchange (EDI) with customers and suppliers. This includes managing product references, spacers (SZR), gas types, tours, and other EDI-specific parameters, ensuring seamless data exchange for orders and other business documents."
---

# Softwarereferenz Firma

---
## Rechte

Folgende Rechte können aktiviert bzw. deaktiviert werden:

-   **Ändern:** Daten dürfen bearbeitet werden.
-   **Einfügen:** Neue Datensätze dürfen angelegt werden.
-   **Löschen:** Datensätze dürfen gelöscht werden.
-   **Ausführen/Lesen:** Der Dialog darf geöffnet werden.

> **Recht zum Ändern mit Recht zum Ausführen kombinieren**
> Soll ein Mitarbeiter das Recht zum Ändern von Daten haben, muss er unbedingt auch das Recht haben, den entsprechenden Dialog auszuführen. Ohne das Recht zum Ausführen kann er den Dialog nicht öffnen, selbst wenn er darin ändern und löschen darf.

### Übersicht

In der Übersicht sind alle vergebenen Rechte angezeigt, die den Auswahlkriterien entsprechen.

## Rechte kopieren

**Pfad:** `Stammdaten > Firma > Mitarbeiterrechte > Menü Funktionen`

*Abb. B-604: Mitarbeiterrechte kopieren*

In diesem Dialog übertragen Sie die Rechte eines Mitarbeiters oder einer Gruppe auf einen (anderen) Mitarbeiter oder eine (andere) Gruppe.

### Quelle, Ziel

Mit der Wahl der Option legen Sie fest, aus welcher Quelle (Datensatz) die Rechte auf welches Ziel übertragen werden sollen.

-   **Gruppe**
-   **Mitarbeiter**

#### Vorhandene Rechte des Ziels löschen

Die Rechte des Ziels können überschrieben oder ergänzt werden.

-   Die Rechte der Zielgruppe oder des Mitarbeiters werden durch die Rechte der Quelle überschrieben und ggf. durch zusätzliche Rechte ergänzt.
-   Die bestehenden Rechte der Zielgruppe oder des Mitarbeiters werden gelöscht und durch die Rechte aus der Quelle ersetzt.

## Statusverwaltung pro Mitarbeitergruppe

**Pfad:** `Stammdaten > Firma > Statusverwaltung pro Mitarbeiter(gruppe)`

*Abb. B-605: Statusverwaltung pro Mitarbeiter(gruppe)*

In diesem Dialog definieren Sie die Statusbereiche für einen der Dokumententypen Angebot, Auftrag, Gutschrift, Anfrage oder Bestellung pro Mitarbeiter oder Mitarbeitergruppe festlegen. Die Einstellungen werden bei einer manuellen Statusänderung abgefragt.

Wenn der Status des aktuellen Dokuments in einem der angegebenen Statusbereiche liegt, darf der angemeldete Mitarbeiter den Status ändern.

### Identifikation

Mit der Wahl der Option legen Sie fest, für welche Mitarbeitergruppe oder für welchen Mitarbeiter die Zuordnungen gelten soll:

-   **Gruppe:** Die Einstellungen gelten für die Mitarbeiter der gewählten Mitarbeitergruppe.
-   **Mitarbeiter:** Die Einstellungen gelten nur für den gewählten Mitarbeiter.

### Dokumententyp

Dokumententyp, dem die Statusbereiche zugeordnet sind.

### Statusbereich Zuordnung

**Bereiche 1, 2, 3, 4 (von - bis)**
Auswahl des Anfangs- und End-Status, in dem der Status des Dokuments manuell geändert werden kann.

### Übersicht

In der Übersicht werden alle Zuordnungen angezeigt, die den aktuellen Filtereinstellungen entsprechen.

## AV-Bereiche

**Pfad:** `Stammdaten > Firma > AV-Bereiche`

*Abb. B-606: AV-Bereiche*

In diesem Dialog definieren Sie die AV-Bereiche und ordnen diesen die entsprechenden Geschäftsarten und Dokumententypen zu. Die Angaben werden in den Dokumenten angezeigt und können überschrieben werden.

Der AV-Bereich dient auch als Sortierkriterium in der A+W Business-Umsatzstatistik.

Den AV-Bereichen können Mitarbeiter zugeordnet werden. Außerdem können Sie zu jedem AV-Bereich eigene Nummernkreise einrichten.

-   "Nummernkreise" auf Seite B-903
-   "Mitarbeiter - Einstellungen" auf Seite B-1026

### Übersicht

**Bezeichnung**
Namen des AV-Bereichs, z. B. Isolierglasfertigung, ESG-Fertigung.

**Geschäftsart**
Geschäftsart des AV-Bereiches, die in der Dokumentenerfassung automatisch übernommen wird.
"Geschäftsart" auf Seite B-900

**Dokumententyp**
Dokumententyp des AV-Bereiches, der in der Dokumentenerfassung automatisch übernommen wird.

**Fremdschlüssel**
Fremdschlüssel für die Kommunikation mit anderen Programmen.

**Gesperrt**
Ein AV-Bereich kann gesperrt werden, wenn er nicht mehr benötigt wird.
-   Der AV-Bereich kann zugewiesen werden.
-   Der AV-Bereich ist gesperrt und kann nicht mehr zugewiesen werden. Wenn er zugewiesen ist, wird er jedoch weiterhin angezeigt.

**Default-Lagerort**
Abweichender Lagerort, von dem der jeweilige AV-Bereich standardmäßig die benötigten Materialien bezieht.

## AD-Bereiche

**Pfad:** `Stammdaten > Firma > AD-Bereiche`

*Abb. B-607: Außendienst-Bereiche*

In diesem Dialog legen Sie die Außendienstmitarbeiter (Vertreter) fest. Jedem Außendienstmitarbeiter können Sie anhand von Postleitzahlen oder Vorwahlnummern ein Einsatzgebiet zuweisen.

Der AD-Bereich dient als auch Sortierkriterium in der A+W Business-Umsatzstatistik.

**Außendienst**
Außendienstmitarbeiter. Zur Auswahl werden alle Mitarbeiter angezeigt, die im Dialog Mitarbeiter angelegt sind.
"Mitarbeiter" auf Seite B-1022

**Bemerkungen**
Zusatzinformation, z. B. Name des Gebiets.

**Von PLZ, bis PLZ**
In diesen Feldern können Sie den Bereich nach Postleitzahlen differenzieren.

**Fremdschlüssel**
Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Finanzbuchhaltung oder für statistische Auswertungen.

**Vorwahlbereiche**
Vorwahlnummern der Gebiete, für die der Vertreter zuständig ist.

> **Beispiel**
>
> Eingaben: 400 – 440, 490 – 510, 750 – 760, 789, 865, 900 – 960
>
> Bei der Erfassung eines Auftrags wird der entsprechende Vertreter automatisch herangezogen, wenn Sie im Feld Telefon eine Telefonnummer eintragen und die Vorwahl durch ein Leerzeichen oder einen Bindestrich von der Rufnummer trennen.

**Typ**
Typ, der für das Provisionssplitting herangezogen wird:
-   **<k.A.>** Dem Mitarbeiter ist kein Typ zugeordnet.
-   **Vertreter 1, Vertreter 2:** Beim Provisionssplitting wird der Prozentsatz für den ausgewählten Typ herangezogen.

## Vertreterprovision

**Pfad:** `Stammdaten > Firma > Vertreterprovision`

*Abb. B-608: Verwaltung - Vertreterprovision*

In diesem Dialog legen Sie die Details für die Standard-Provisionssätze pro Vertreter fest. Sie können zwischen unterschiedlichen Provisionsarten wählen.

Die Provision kann im Modul Statistik ausgewertet werden.

### Menü Funktionen

In diesem Menü werden folgende Einträge angezeigt:

-   **Provisionssätze kopieren:** Öffnet den Dialog Vertreter - Provisionssätze kopieren, um die Provisionssätze auf einen anderen Vertreter zu übertragen.
    -   "Vertreter - Provisionssätze kopieren" auf Seite B-1038
-   **Alle Provisionssätze löschen:** Löscht alle Provisionssätze.

### Auswahl Vertreter / Warengruppe

**Jahrgang, Schlüssel**
Die Provision kann nach verschiedenen Preislisten unterschieden werden. Wenn Sie in beiden Feldern den Eintrag <k.A.> auswählen, ist der Provisionssatz allgemein gültig.

**Vertreter**
Vertreter, für den die Angaben gelten. Sie müssen für jeden Vertreter und mindestens für jede Warenhauptgruppe (WHG) einen Provisionssatz anlegen.

**Gültigkeit bis**
Datum, bis zu dem der Provisionssatz gültig ist.

**Kunde**
Der Provisionssatz kann für alle Kunden oder nur für einen einzelnen Kunden gelten:
-   **0:** Die Vertreterprovision gilt für alle Kunden.
-   **1-9999999:** Die Vertreterprovision ist auf diesen Kunden beschränkt.

**WGR**
Der Provisionssatz kann für eine Warengruppe (WHG, WOG, WGR) gelten. Sie sollten mindestens einen Satz pro WHG und pro Vertreter anlegen.

**Produkt**
Der Provisionssatz kann für alle Produkte oder nur für ein bestimmtes Produkt gelten:
-   **0:** Die Vertreterprovision gilt für alle Produkte.
-   **1-9999999:** Die Vertreterprovision ist auf dieses Produkt beschränkt.

### Provisionsart

Provision wird auf bestimmt Kennziffern vergeben, z. B. auf den Umsatz. Mit der Wahl der Option legen Sie diese Berechnungsgrundlage für die Provision fest:

-   **Rabatt %:** Rabatt-Wert in Prozent. Bei dieser Einstellung bietet sich z. B. eine Staffelung an, nach der ein Vertreter mehr Provision erhält, wenn der Rabatt geringer ist.
-   **Deckungsbeitrag %:** Deckungsbeitrag in Prozent (Deckungsbeitrag = Umsatz Verkauf - Eigenkosten). Bei dieser Einstellung bietet sich z. B. eine Staffelung an, nach der ein Vertreter umso mehr Provision erhält, je höher der Deckungsbeitrag ist.
-   **Umsatz:** Umsatzbetrag. Bei dieser Einstellung bietet sich z. B. eine feste Provision an.
-   **Deckungsbeitrag:** Betrag des Deckungsbeitrags. Bei dieser Einstellung bietet sich z. B. eine feste Provision an.
-   **Preis/PE:** Preis pro Preiseinheit. Bei dieser Einstellung bietet sich z. B. eine feste Provision an.

**Staffelmenge**
Menge, nach der Sie die Provision staffeln wollen.

> **Beispiel**
>
| Menge | % Provision |
| :--- | :--- |
| 20 | 0,500 |
| 100 | 0,750 |
| 9999 | 1,250 |
>
> Bei Auswahl der Provisionsart nach Umsatz: 13-stelliges numerisches Feld.

**Provision %**
Prozentsatz, der zur Berechnung der Provision herangezogen wird. 8-stelliges numerisches Feld.
Die Eingabe eines negativen Wertes mit bis zu 4 Nachkommastellen ist möglich. Mit einem negativen Wert würde die Provision reduziert.

**Fremdschlüssel**
Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Finanzbuchhaltung.

**Gültigkeit ab**
Datum, ab dem der Provisionssatz gültig ist.

### Übersicht

In der Übersicht werden die Felder mit den Werten angezeigt, die zur Definition des Provisionssatzes gefüllt wurden. Zusätzlich müssen Sie in den folgenden Spalten Angaben zur Berechnung der Provision machen.

## Vertreter - Provisionssätze kopieren

**Pfad:** `Stammdaten > Firma > Vertreterprovision > Menü Funktionen > Provisionssätze kopieren`

*Abb. B-609: Provisionssätze kopieren*

In diesem Dialog übertragen Sie die Provisionssätze eines Vertreters auf einen anderen.

### Quelle, Ziel

**Vertreter**
Wenn Sie in beiden Feldern denselben Vertreter auswählen, können Sie seine bisherigen Provisionssätze kopieren und dabei mit anderen Jahrgängen, Schlüsseln und mit einem neuen Gültigkeitsdatum speichern, um anschließend die Staffelmengen und Prozentangaben zu bearbeiten.

**Jahrgang, Schlüssel**
Preislisten der Quelle und des Ziels.

**Kunde**
Kunden, auf den die Provisionssätze beschränkt sind.

**Gültigkeitsdatum, Vorgabe Gültigkeitsdatum**
Gültigkeitsdatum, ab dem die Provision in der neuen Form berechnet werden soll. Für das Ziel können Sie ein Datum in der Zukunft wählen.

**Ziel überschreiben**
Die Provisionssätze des Ziels können überschrieben oder ergänzt werden.
-   Die Provisionssätze des Vertreters werden durch die Provisionssätze der Quelle überschrieben und ggf. durch zusätzliche Provisionssätze ergänzt.
-   Die bestehenden Provisionssätze des Vertreters werden gelöscht und durch die Provisionssätze aus der Quelle ersetzt.

## Banken

**Pfad:** `Stammdaten > Firma > Banken`

*Abb. B-610: Banken*

In diesem Dialog tragen Sie die firmeneigenen Bankverbindungen ein. Sie können mehrere Konten pro Mandant bei unterschiedlichen Bankverbindungen hinterlegen. Nur die Banken können angegeben werden, die im Dialog Banken hinterlegt sind.

-   "Banken" auf Seite B-920

**Mandant**
Mandant, dessen Banken in der Übersicht angezeigt werden.

### Bankverbindung

**BLZ/BIC**
Bankleitzahl und BIC (Business Identifier Code). Über die Lupe können Sie nach der gewünschten Bank suchen. Über den Ordner können Sie weitere Bankdaten hinterlegen oder die vorhandenen ergänzen.

**Name, Sitz**
Namen und Standort der Bank werden automatisch angezeigt.

**Konto**
Kontonummer des Mandanten.

**Hauptbank**
Wenn Sie mehrere Konten für einen Mandanten eingetragen haben, müssen Sie einen Eintrag als Hauptbank kennzeichnen.
-   Die Daten des aktuell angezeigten Kontos sind nicht als Hauptbank gekennzeichnet.
-   Die Daten des aktuell angezeigten Kontos sind als Hauptbank gekennzeichnet.

**IBAN**
International Bank Account Number zum angegebenen Konto.

### Banken

In der Übersicht werden alle Bankverbindungen des aktuellen Mandanten angezeigt.

## Filialen

**Pfad:** `Stammdaten > Firma > Filialen`

*Abb. B-611: Filialen*

In diesem Dialog pflegen Sie Filialen Ihrer Mandanten. Die Daten dienen nur zur Information.

### Anschrift

**Name**
Namen der Filiale, so wie sie im Handelsregister angegeben ist oder offiziell bezeichnet wird.

**Straße**
Adresse der Filiale.

### Kommunikation

**Telefon 1-4, Fax, Mail**
Telefonnummern, Faxnummer und E-Mail-Adresse der Filiale.

### Übersicht

In der Übersicht werden alle Filialen für den jeweils ausgewählten Mandanten angezeigt.

## Buchungsperioden

**Pfad:** `Stammdaten > Firma > Buchungsperioden`

*Abb. B-612: Buchungsperioden*

In diesem Dialog tragen Sie die Buchungsperioden ein. Die Einträge werden bei der Übergabe an Ihr FiBu-Programm geprüft.

Damit Aufträge, Bestellungen und Gutschriften zum gewünschten Zeitpunkt automatisch übergeben werden, definieren Sie unterschiedliche Buchungsperioden. Auslöser für die Übergabe ist der von Ihnen jeweils festgelegte Status.

Wenn das eingetragene Datum z. B. für Aufträge erreicht ist, kann kein Auftrag mehr in diese Buchungsperiode übergeben werden.

**Abgeschlossene Buchungsperiode**
Datum, an dem die Buchungsperiode abgeschlossen ist. Für die Prüfung der Dokumente ist immer nur das Datum relevant, das dem aktuellen Datum am nächsten ist.

**Auftrag, Gutschrift, Bestellung**
Die Buchungsperiode gilt nur für den jeweils markierten Typ.
-   Die Buchungsperiode gilt nicht.
-   Die Buchungsperiode gilt für diesen Dokumententyp.

## Produktzuordnung Zuschläge

**Pfad:** `Stammdaten > Firma > Produktzuordnung Zuschläge`

*Abb. B-613: Produktzuordnung Zuschläge*

In diesem Dialog verwalten Sie Ihre Sonderrabatte und Teuerungszuschläge. Zusätzlich zu den hinterlegten Teuerungszuschlägen existieren zehn Sonderrabatte, die Sie entweder als Sonderrabatte oder Teuerungszuschläge nutzen können, z. B. Zuschläge für Transport-/Mautkosten, L-Gestelle.

> **i Zuschlagsprodukt**
> Jeder Zuschlag oder Sonderrabatt, der wie ein Produkt erfasst werden soll, muss als Produkt angelegt sein.

### Zuordnung

**Mandant**
Mandant, für den die Zuschläge gelten.

**Allgemein, Kunde**
Mit der Wahl der Option legen Sie fest, ob der Zuschlag für alle Kunden oder nur für einen bestimmten gilt. Die entsprechenden Eingabefelder werden freigeschaltet.

**Zuschlag**
Zur Auswahl werden die hinterlegten Zuschläge und Sonderrabatte angeboten.
-   Tutorial 1, "Verfügbare Teuerungszuschläge/Sonderrabatte" auf Seite B-335
-   Tutorial 1, "Automatischen Zuschlag definieren" auf Seite B-337

**Produkt**
Produkt, mit dem der Zuschlag oder der Rabatt berechnet werden soll. Als Produktbezeichnung wird die Bezeichnung 1 aus der Produktverwaltung angezeigt. Diese wird auch in der Produkt- und Kundenverwaltung im Bereich Zuschläge/Rabatte anwenden angezeigt.

**Gültig von - bis**
Zeitraum, in dem der Rabatt bzw. Zuschlag gültig sein soll.

**Position im Dokument**
Mit der Positionsnummer wird die Reihenfolge angegeben, in der die Sonderrabatte bzw. Teuerungszuschläge als Position im Dokument eingefügt werden. Sie bestimmen damit auch die Berechnungsreihenfolge. Die Nummern können mehrfach vergeben werden.

-   **0:** Positionsbezogene Sonderrabatte oder Teuerungszuschläge werden mit Position 0 definiert, z. B. Struktur innen-Zuschlag, Zuschlag bei Überschreitung der maximalen Fläche.
-   **950-999:** Die Sonderrabatte oder Teuerungszuschläge, die auf alle vorherigen oder Teile der vorherigen Positionen wirken, werden mit einer Positionsnummer zwischen 950 und 999 definiert.

Beim Mindermengenzuschlag werden alle Positionen mit demselben Mindermengenzuschlag (Produkt) geprüft und für alle zusammen eine Zuschlagsposition eingefügt. Als Positionsnummer muss eine Zahl eingetragen werden zwischen der Null (0), die sich auf eine einzelne Position bezieht, und 900, die am Ende des Dokuments eingefügt werden.

> **i Anlieferpauschale bei Abholung**
> Damit bei der Tour Abholung die Anlieferpauschale nicht automatisch während der Dokumentenerfassung eingefügt wird, muss in der Tourenverwaltung bei dieser Tour die Checkbox ohne Lief.Pausch. aktiviert sein.
>
> "Touren" auf Seite B-873

### Zuschlagszuordnung

In der Übersicht werden alle Zuschläge aller Mandanten aufgeführt. Wenn Sie einen Eintrag markieren, können Sie die Werte in den freigeschalteten Feldern überschreiben.

## Formeln

**Pfad:** `Stammdaten > Firma > Formeln`

*Abb. B-614: Formelverwaltung*

In diesem Dialog sind alle Formeln hinterlegt, mit denen Sie bestimmte Aufgaben in A+W Business automatisieren können. Im Register `Formel` wird jeweils die Syntax der Formel angezeigt, die im Register `Tabelle` markiert ist.

> **i Formel einfügen oder bearbeiten**
> Wenn Sie weitere Formeln benötigen oder eine Formel anpassen müssen, wenden Sie sich bitte an die A+W Software GmbH.

### Menü Optionen

Über dieses Menü können Sie die Prüfung der Formel während der Eingabe aktivieren. Fehler werden beim Speichern angezeigt.

## Schnittstellen-Dienst

**Pfad:** `Stammdaten > Firma > Schnittstellen-Dienst`

In diesem Dialog definieren Sie die Schnittstellen, über die Daten zwischen A+W Business und anderen Programmen ausgetauscht werden sollen.

Im Dialog Schnittstellen-Dienst finden Sie folgende Register:

-   Schnittstellen-Dienst - Einstellungen A+W Production-Formate
-   Schnittstellen-Dienst – Einstellungen weitere Formate
-   Schnittstellen-Dienst - Optionen

### Schnittstellen-Dienst – Einstellungen A+W Production-Formate

**Pfad:** `Stammdaten > Firma > Schnittstellen-Dienst > Register Einstellungen A+W Production-Formate`

*Abb. B-615: Produktionsrückmeldungen – Einstellungen A+W Production-Formate*

In diesem Register wählen Sie die Rückmeldungen aus, die Sie von A+W Production per Datei empfangen und einlesen wollen.

Wenn STSP-, STSL-, STSD-, STSB-, STSG-Dateien für die Rückmeldungen genutzt werden, muss im Bereich `Auftrag produziert bei` eine Erfassungsstelle ausgewählt werden, die einem Statuspunkt zugewiesen ist. Wenn eine solche Erfassungsstelle nicht zugewiesen wurde, erzeugt die Rückmeldung einen Fehler.

Die Erfassungsstellen werden im Dialog `Erfassungsstellen Produktion` hinterlegt.

-   "Erfassungsstellen Produktion" auf Seite B-882

> **i Gesperrte Felder**
> Die Felder sind gesperrt, wenn im Register `Einstellungen weitere Formate` die Checkbox `Import von Produktionsrückmeldungen` aktiviert ist. Sie können dann keine Einstellungen für A+W Production-Formate festlegen.

#### Identifikation

**Einstellungen für**
Mitarbeiter, für den die Einstellungen gelten. Wenn die Einstellungen für alle Benutzer gelten sollen, wählen Sie den Eintrag `Administrator`. Bei dieser Einstellung muss im Bereich `Auftrag produziert bei` dieselbe Erfassungsstelle ausgewählt sein, wie in den `Firmendaten > Register Lager/EK/EDI`.

#### A+W Production-Formate

In diesem Bereich wählen Sie aus, welche Rückmeldungen aus A+W Production eingelesen werden sollen. Das Verzeichnis für die Rückmeldedatei können Sie dann im jeweils freigeschalteten Feld angeben. Dieselben Verzeichnisse müssen in A+W Production angegeben werden, damit die Dateien korrekt gespeichert werden. Die Dateien werden über den A+W Commercial Exchange Service eingelesen.

**Import von Produktionsrückmeldungen**
Die STSP-Rückmeldung erfolgt überwiegend pro Stück. Sie können für die entsprechende Erfassungsstelle einstellen, ob der Status schon bei der ersten Scheibe oder erst bei Rückmeldung aller Scheiben des Auftrages hochgesetzt werden soll.
-   Rückmeldedateien aus der Produktion werden nicht eingelesen.
-   Die Rückmeldung aus der Produktion wird als STSP-Datei gesendet. Der Auftragsstatus, das Produktionsdatum und die Kopf- bzw. Positionslaufnummer werden aktualisiert.

**Prod.freigabe Auftrag, falls Subauftrag produziert**
Das Feld ist nur freigeschaltet, wenn Produktionsrückmeldungen importiert werden. Zu einem Auftrag kann ein Teilauftrag erfasst sein. Wenn eine Produktionsrückmeldung einen solchen Subauftrag betrifft, kann der Status des Gesamtauftrags umgesetzt werden.
-   Ein Auftrag wird nicht automatisch auf den Status zur Produktionsfreigabe gesetzt.
-   Wenn die Subaufträge als produziert zurückgemeldet werden, erhöht sich der Status des Hauptauftrags automatisch auf Produktionsfreigabe.

**Laufnummer aus dem Auftragskopf übernehmen**
Das Feld ist nur freigeschaltet, wenn Produktionsrückmeldungen importiert werden. Wenn eine Erfassungsstelle aufgeführt ist, der kein Status zugeordnet ist, wird die Rückmeldung in der A+W Business-Kapazitätsplanung verarbeitet und der Status entsprechend umgesetzt.
-   Die Laufnummern der Positionen werden unabhängig von der Laufnummer des Auftragskopfes aktualisiert.
-   Nach der Aktualisierung des Auftragskopfes erhalten alle Positionen die Laufnummer auf den Auftragskopf, deren Positionsstatus größer/gleich dem Status der Erfassungsstelle für `produziert` ist.
    -   "Erfassungsstellenzuordnung" auf Seite B-977

**Import von Planungsrückmeldungen**
Aus der Produktion können die STSL-Daten der Grob- und Feinplanung importiert werden. Wenn eine Erfassungsstelle aufgeführt ist, der kein Status zugeordnet ist, wird die Rückmeldung in der Kapazitätsplanung verarbeitet und der Status entsprechend umgesetzt.
-   Rückmeldungen aus Grob- und Feinplanung werden nicht eingelesen.
-   Die Rückmeldungen aus Grob- und Feinplanung werden eingelesen. Der Auftragsstatus wird dann der angegebenen Erfassungsstelle entsprechend hoch gesetzt. Dazu müssen im Bereich Optionen die Erfassungsstellen für die Kapazitätsplanung (Zeitwirtschaft) angegeben werden.
    -   "Erfassungsstellen Produktion" auf Seite B-882

**Import von BDE-Rückmeldungen**
Die STSD-Rückmeldung aus der Betriebsdatenerfassung (BDE) dient im A+W Business dazu, den Auftragsstatus, das Produktionsdatum und die Kopf- und/oder Positionslaufnummer zu aktualisieren. Die Rückmeldung erfolgt überwiegend pro Stück. Sie können einstellen, ob der Status schon bei der ersten Scheibe oder erst bei Rückmeldung aller Scheiben des Auftrages hochgesetzt werden soll. Wenn eine Erfassungsstelle angegeben ist, der kein Status zugeordnet ist, wird die Rückmeldung in der Kapazitätsplanung verarbeitet und der Status entsprechend umgesetzt. Dazu müssen im Bereich Optionen die Erfassungsstellen für die Kapazitätsplanung (Zeitwirtschaft) angegeben werden.
-   BDE-Rückmeldungen werden nicht eingelesen.
-   Die BDE-Rückmeldung wird als STSD-Datei gesendet.

**Produktionsgestellnummer in Position übernehmen**
Das Feld ist nur freigeschaltet, wenn BDE-Rückmeldungen importiert werden. Wenn in der BDE-Rückmeldung Gestellnummern zu Positionen enthalten sind, können diese in A+W Business der Position zugewiesen werden.
-   Gestellnummern werden nicht in die Position übernommen.
-   Die gemeldeten Gestellnummern werden in den Auftrag zurückgeschrieben und der jeweiligen Position zugeordnet.

**Import von Gestellzuordnung-Rückmeldungen**
Die STSG-Rückmeldung gibt an, welches Gestell der jeweiligen Auftragsposition zugeordnet ist und welche Mengen produziert sind. Die Gestellnummer wird auf dem Lieferschein gedruckt.
-   Rückmeldungen von Gestellzuordnungen werden nicht importiert.
-   Die Rückmeldung der Gestellzuordnung wird als STSG-Datei gesendet.

> **Gestell-Rückmeldung für Teillieferung**
> Bei Teillieferung besteht die Möglichkeit, die Menge der Teillieferungsposition durch die per STSG zurückgemeldete verpackte Menge bestimmen zu lassen. Dazu muss beim Kopieren des Auftrags die Option `Teillieferungsmenge > Gestellrückmeldung bei Teillieferung berücksichtigen` aktiviert werden. Die Menge der Teillieferungsposition ist dann mit der Gesamtmenge aus den STSG-Meldungen zur betreffenden Auftragsposition vorbelegt. Sie kann nicht mehr geändert werden.

**Update der Produktionsübersicht durch Erfassungsstelle**
Das Feld ist nur freigeschaltet, wenn Rückmeldungen von Gestellzuordnungen importiert werden. In diesem Feld wählen Sie die Erfassungsstelle aus, über die Gestellrückmeldungen den Status hochsetzen. Über die gewählte Erfassungsstelle wird die Produktionsübersicht im Dialog `Übersicht Statusrückmeldung` aktualisiert.
-   Verkauf, "Übersicht Statusrückmeldung" auf Seite C-590

**Import von Gestell-Ein-/Ausgang-Rückmeldungen**
Die STSK-Rückmeldung meldet den Status des Gestells und das jeweilige Eingangs- und Ausgangsdatum.
-   Rückmeldungen zum Gestelleingang und -ausgang werden nicht importiert.
-   Die Rückmeldung von Gestelleingang und -ausgang wird eingelesen. Nach einer Überprüfung, ob der Kunde und das Gestell existieren, wird die Ausgabe bzw. die Rücknahme des Gestells verbucht. Existiert das Gestell in A+W Business noch nicht, wird es mit dem Typ `<k.A.>` angelegt.

**Import von Bruch-Rückmeldungen**
Mit der STSB-Rückmeldung werden die Reklamationen und die bei der Produktion zu Bruch gegangenen Scheiben gemeldet. A+W Business kann daraus automatisch Reklamationsaufträge erstellen. Wenn eine Erfassungsstelle angegeben ist, der kein Status zugeordnet ist, wird die Rückmeldung in der Kapazitätsplanung verarbeitet und der Status entsprechend umgesetzt. Dazu müssen im Bereich Optionen die Erfassungsstellen für die Kapazitätsplanung (Zeitwirtschaft) angegeben werden.
-   Bruch-Rückmeldungen werden nicht importiert.
-   Die Bruch-Rückmeldung wird als STSB-Datei gesendet.

**Reklamationsaufträge erstellen**
Das Feld ist nur freigeschaltet, wenn Bruch-Rückmeldungen importiert werden.
-   Reklamationsaufträge werden nicht automatisch erstellt.
-   Bei einer Bruchmeldung wird automatisch ein Reklamationsauftrag erstellt. Dieser Funktion können ein Standard-Verursacher und ein Standard-Grund zugeordnet werden, die jeweils im Reklamationsauftrag überschrieben werden können.

**Verursacher**
Das Feld ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden. Sie können einen Verursacher auswählen, der in den automatisch erstellten Reklamationsauftrag übernommen wird. Dieser wird unabhängig von der Einstellung in den `Firmendaten > Register Archiv` ausgelesen.
-   "Default Reklamationsort" auf Seite B-982

**Grund**
Das Feld ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden. Sie können einen Reklamationsgrund auswählen, der in den automatisch erstellten Reklamationsauftrag übernommen wird.

**Kostenlos**
Die Checkbox ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden.
-   Der automatisch erstellte Reklamationsauftrag ist nicht standardmäßig kostenlos.
-   Der automatisch erstellte Reklamationsauftrag ist standardmäßig kostenlos. Die Einstellung kann in dem Reklamationsauftrag überschieben werden.

**AV-Bereich**
Das Feld ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden. Sie können dann einen AV-Bereich auswählen, aus dessen Nummernkreis die Auftragsnummer gezogen wird.

**Ziel-NV**
Das Feld ist nur freigeschaltet, wenn automatisch Reklamationsaufträge erstellt werden. Sie können einen Nummernverwalter auswählen, in den der automatisch erstellte Reklamationsauftrag gestellt wird.

**Import von XTV-Rückmeldungen**
Mit der XTV-Rückmeldung werden die Lagermaße abgebucht, die für einen Auftrag zugeschnitten werden. Außerdem werden für Artikel mit Lagermodus kombiniert die qm-Reservierungen in den Aufträgen gelöscht.
-   XTV-Rückmeldungen werden nicht importiert.
-   Die Rückmeldung aus der Optimierung wird als PRODBDA*-Datei gesendet.

#### Optionen

Die Felder in diesem Bereich sind nur freigeschaltet, wenn Sie Rückmeldungen importieren, zu denen weitere Angaben möglich sind.

**Menge größer Positionsmenge in STSB, STSD, STSG, STSL, STSP zulassen**
Aus der Produktion können größere Stückzahlen pro Position zurückgemeldet werden, als im Auftrag enthalten sind.
-   Größere Stückzahlen pro Position werden nicht zugelassen.
-   Die Meldungen können auch bei größeren Stückzahlen verarbeitet werden.

**Zeitwirtschaft verarbeitet STSD und STSB**
STSD- und STSB-Meldungen können über die Kapazitätsplanung (Zeitwirtschaft) verarbeitet werden.
-   Die Kapazitätsplanung verarbeitet keine Daten aus den STSD- und STSB-Dateien.
-   STSD- und STSB-Dateien werden von der Kapazitätsplanung verarbeitet.

**Erfassungsstelle STSD**
Erfassungsstelle, über die der Status umgesetzt wird, wenn die STSD-Meldung über die Kapazitätsplanung verarbeitet wird.

**Erfassungsstelle STSB**
Erfassungsstelle, über die der Status umgesetzt wird, wenn die STSB-Meldung über die Kapazitätsplanung verarbeitet wird.

**Auftrag produziert bei**
Damit ein Auftrag fertiggemeldet werden kann, müssen Sie für die Rückmeldungen eine Erfassungsstelle angeben.
Wenn die Einstellungen für alle Benutzer gelten sollen, müssen Sie dieselbe Erfassungsstelle auswählen, wie im Dialog `Firmendaten`.
-   "Firmendaten - Lager/EK/EDI" auf Seite B-970

**Erfassungsstelle**
Erfassungsstelle, die bei Rückmeldungen folgende (zusätzliche) Aktionen auslösen kann:
-   Im Auftrag werden das Produktionsdatum und die Laufnummer erhöht.
-   Bei Produktionsaufträgen wird der Warenzugang im Lager gebucht.

### Schnittstellen-Dienst – Einstellungen weitere Formate

**Pfad:** `Stammdaten > Firma > Schnittstellen-Dienst > Register Einstellungen weitere Formate`

*Abb. B-616: Produktionsrückmeldungen – Einstellungen weitere Formate*

In diesem Register wählen Sie die Rückmeldungen aus, die Sie aus der Betriebsdatenerfassung (BDE), von ALFERT und von der FiBu erhalten und einlesen wollen.

#### BDE- und ALFERT-Formate

> **i Gesperrte Felder**
> Die Felder im Bereich BDE- und ALFERT-Formate sind gesperrt, wenn im Register `Einstellungen A+W Production-Formate` die Checkbox `Import von Produktionsrückmeldungen` aktiviert ist. Sie können dann keine Einstellungen für BDE-Formate festlegen.

**Import von Produktionsrückmeldungen**
Die Rückmeldung erfolgt überwiegend pro Stück. In A+W Business kann für die entsprechende Erfassungsstelle eingestellt werden, ob der Status schon bei der ersten Scheibe oder erst bei Rückmeldung aller Scheiben des Auftrages hochgesetzt werden soll.
-   Rückmeldedateien aus der Produktion werden nicht importiert.
-   Die Rückmeldung aus der Produktion wird aus der AWB_STAT-Datei eingelesen.

**Laufnummer aus dem Auftragskopf übernehmen**
Das Feld ist nur freigeschaltet, wenn Produktionsrückmeldungen importiert werden. Die Laufnummer aus dem Auftragskopf kann für die Positionen übernommen werden.
-   Die Laufnummern der Positionen werden unabhängig von der Laufnummer des Auftragskopfes aktualisiert.
-   Nach der Aktualisierung des Auftragskopfes erhalten alle die Positionen die Laufnummer auf den Auftragskopf, deren Positionsstatus größer/gleich dem Status der Erfassungsstelle für `produziert` ist.

**Import von Gestell-Rückmeldedateien**
Die AH_GEST.DAT-Rückmeldung meldet den Status des Gestells und das jeweilige Eingangs- und Ausgangsdatum.
-   Rückmeldungen zum Gestelleingang und -ausgang werden nicht importiert.
-   Rückmeldungen von Gestelleingang und -ausgang werden eingelesen.

**Import von AWPool-Dateien**
Mit der AWPool-Rückmeldung werden in A+W Business Auftragsstatus, Produktionsdatum, Kopf- und Positionslaufnummer aktualisiert. Die Zuordnung der AWPool-Status zu einem A+W Business-Status ist fest programmiert.
-   AWPool-Rückmeldungen werden nicht importiert.
-   AWPool-Rückmeldungen werden als POOL*.DAT-Dateien eingelesen. Das Feld `Update Produktionsdatum ab Status` wird freigeschaltet.

**Update Produktionsdatum ab Status**
Das Feld ist nur freigeschaltet, wenn AWPool-Rückmeldungen importiert werden.
-   Das Produktionsdatum im Auftrag wird nicht aktualisiert.
-   Das Produktionsdatum im Auftrag wird aktualisiert, wenn einer der Status eingestellt ist, die zur Wahl stehen.

#### FiBu

In diesem Bereich legen Sie die Einstellungen für die Meldung der Offenen Posten fest, die automatisiert über den A+W Commercial Exchange Service eingelesen werden.

**Import von Offen-Posten-Rückmeldungen**
Offene Posten (OP) können aus dem FiBu-Programm per Datei gemeldet werden. Dies betrifft nur die Kundenkonten.
-   OP-Rückmeldungen werden nicht importiert.
-   OP-Rückmeldungen werden als Datei eingelesen. Die Felder für den Ablageort, eine Sicherungs- und eine Batch-Datei werden freigeschaltet.

**Sicherungsdatei anlegen**
Das Feld ist nur freigeschaltet, wenn OP-Rückmeldungen importiert werden. Sie können dann eine zusätzliche Sicherungsdatei speichern und festlegen, wie viele Tage diese gespeichert bleibt.
-   Zur OP-Rückmeldedatei wird keine Sicherungsdatei gespeichert.
-   OP-Rückmeldungen sollen als Sicherung (mit Zeitstempel) zusätzlich an einem anderen Ort gespeichert werden. Die Felder zur Auswahl des Verzeichnisses und für die Vorhaltetage werden freigeschaltet.

**Vorhaltetage für Sicherungsdateien**
Das Feld wird nur freigeschaltet, wenn eine Sicherungsdatei gespeichert werden soll. Sie können eintragen, wie viele Tage diese Datei nicht überschrieben werden darf.

**Batch-Datei**
Namen der Batch-Datei, die zum Kopieren der Dateien benötigt wird.

### Schnittstellen-Dienst – Optionen

**Pfad:** `Stammdaten > Firma > Schnittstellen-Dienst > Register Optionen`

*Abb. B-617: Produktionsrückmeldungen – Optionen*

In diesem Register legen Sie die Intervalle fest, mit denen regelmäßig nach neuen Rückmeldungen gesucht werden soll.

#### Intervall

**Standard Minute(n)**
Intervall für den A+W Commercial Exchange Service. Wenn Sie z. B. eine 2 eintragen, prüft der Service alle 2 Minuten, ob neue Rückmeldungen aus der Produktion vorliegen, und liest diese ein.

**OP-Rückmeldung – Minute(n)**
Intervall für die Rückmeldung der Offenen Posten (OP). Wenn Sie z. B. eine 120 eintragen, werden alle 2 Stunden neuen Rückmeldungen per Batch eingelesen.
OP-Rückmeldungen können nur importiert werden, wenn die Funktion im Register `Einstellungen weitere Formate` aktiviert ist.
Für die Rückmeldungen müssen Sie im Dialog `Firmendaten` die Checkboxen für die OP-Meldungen aktivieren.
-   "Firmendaten - FiBu" auf Seite B-936

#### Einstellungen für automatischen Mailversand

**Mailversand**
Mails eines bestimmten Absenders können automatisch an eine bestimmte Adresse gesendet werden.
-   Mails nicht werden gesendet.
-   Mails werden gesendet. Die Felder werden freigeschaltet.

**Server**
Name des Servers, über den der Mailversand gesteuert wird.

**Port**
Nummer des Ports für den Mailversand.

**Absender Adresse, Empfänger Adresse**
E-Mail-Adressen, die standardmäßig für verwendet werden sollen.

**Authentifizierung**
Für die Datenübertragung kann eine Authentifizierung verwendet werden.
-   Die Sendebestätigung wird nicht ohne Authentifizierung gesendet.
-   Für die Sendebestätigung ist Authentifizierung erforderlich. Die Felder zur Eingabe der Anmeldedaten werden freigeschaltet.

**SSL Verschlüsselung verwenden**
Secure Sockets Layer (SSL); Verschlüsselungsprogramm zur sicheren Datenübertragung im Internet.
-   Die Sendebestätigung wird nicht verschlüsselt.
-   Die Sendebestätigung wird nach dem SSL-Protokoll verschlüsselt.

**Benutzer, Passwort**
Anmeldedaten, mit denen der Sender sich authentifiziert.

## Customizing

**Pfad:** `Stammdaten > Firma > Customizing`

*Abb. B-618: Customizing*

In diesem Dialog stellen Sie A+W Business und seine Funktionen auf die Bedürfnisse in Ihrem Unternehmen ein.
Sie können den Dialog nur öffnen, wenn Sie als Administrator mit den entsprechenden Rechten angemeldet sind.

> **i Anpassungen einrichten**
> Mit dem Customizing greifen Sie unter Umständen tief in die Funktionen von A+W Business ein. Wenn Sie A+W Business für Ihr Unternehmen weiter anpassen wollen, setzen Sie sich bitte mit der A+W Software GmbH in Verbindung, um die Anpassungen abzustimmen.

## Datencontainer

**Pfad:** `Stammdaten > Firma > Datencontainer`

*Abb. B-619: Customizingdaten - Datencontainer*

In diesem Dialog verwalten Sie Daten, die für das Customizing benötigt werden, mit der A+W Business-Datenbank. Die Bezeichnung der Register und der Tabellenspalten kann dabei ebenfalls konfiguriert werden.

# Texte

**Pfad:** `Stammdaten > Texte`

In diesem Programmbereich werden die Texte und die Textkennzeichen verwaltet, die in der Dokumentenbearbeitung benötigt werden.

Im Menü Texte finden Sie folgende Einträge:

-   "Textkennzeichen" auf Seite B-1058
-   "Texte" auf Seite B-1059
-   "Systemtexte" auf Seite B-1060
-   "Mahntexte" auf Seite B-1061
-   "Dateianhangs-Typen" auf Seite B-1062
-   "Dateianhangs-Bemerkungen" auf Seite B-1063
-   "Technische Werte" auf Seite B-1063

## Textkennzeichen

**Pfad:** `Stammdaten > Texte > Textkennzeichen`

*Abb. B-620: Textkennzeichen*

In diesem Dialog hinterlegen Sie die Textkennzeichen. Die Textkennzeichen dienen der Zuordnung von Textblöcken zu Themenbereichen, z. B. P für Produktion, L für Lieferschein, T für allgemeine Texte. Über die Textkennzeichen können Sie steuern, welche Texte in welchen Dokumenten gedruckt werden sollen.
-   Tutorial 2, "Textarten" auf Seite B-469

**Kennzeichen**
Textkennzeichen, z. B. P für Produktionstexte, V für Terminverschiebungen.

**Bezeichnung**
Namen, z. B. Produktion für Texte, die an die Produktion übergeben werden sollen.

## Texte

**Pfad:** `Stammdaten > Texte > Texte`

*Abb. B-621: Texte bei Mehrsprachigkeit*

In diesem Dialog erfassen Sie Standardtexte, die häufig verwendet werden, z. B. die Rahmentexte oder Texte für die Terminverschiebung. In den Texten können Platzhalter verwendet werden, die erst beim Druck eines Dokuments mit Werten gefüllt werden.

-   Tutorial 2, "Textkennzeichen und Standardtexte" auf Seite B-471

Wenn Sie mit der Mehrsprachigkeit arbeiten, müssen alle Texte auch in der jeweiligen Sprache erfasst werden. Achten Sie dabei darauf, dass die Textnummern in den Übersetzungen nicht geändert werden.

-   "Sprachen" auf Seite B-564

**Sprache**
Auswahl der Sprache, in der der Text gedruckt werden soll.

**Nummer**
Beliebige Nummer für den Text. Sie sollten die Texte pro Textkennzeichen in Nummernbereichen zusammenfassen, z. B. 1-99 für Rechnungstexte, 100-199 für Angebotstexte.
Wenn Sie mit dem Modul Mehrsprachigkeit arbeiten, muss zu Beginn der Erfassung der fremdsprachlichen Texte in jedem Sprachregister mindestens ein Text mit der Nummer 0 angelegt sein.

**Matchcode**
Die Eingabe des Matchcodes ist optional.

**Kennzeichen**
Über das Textkennzeichen wird der Text für den Druck zugeordnet. Durch die Angabe des Kennzeichens L für Lieferschein können Sie z. B. Dialog Formulare steuern, ob der Text gedruckt werden soll oder nicht.

**Texttyp AWProd.**
Positionstexte werden an die Produktion übergeben, wenn das Textkennzeichen (P) für die Produktionsübergabe die Übergabe erlaubt. Für diese Texte können Sie den Texttyp (Fremdschlüssel) angeben, der in A+W Production für diese Texte genutzt wird. Ist kein Texttyp eingetragen, wird standardmäßig der Texttyp 1 übergeben.

### Auswahl

In der Übersicht werden alle Texte angezeigt, die den Auswahlkriterien entsprechen.

### Textbearbeitung

**Schaltflächen**
Sie können die Schriftart und -größe ändern und Hyperlinks, Bilder und Tabellen einfügen.
-   Tutorial, "Text erfassen" auf Seite C-54

**(Eingabefeld)**
Standardtext oder Rahmentext. Bei Rahmentexten und bei bestimmten Standardtexten können Sie mit Variablen (Platzhaltern) arbeiten.
-   Tutorial 2, "Texte anlegen" auf Seite B-477

## Systemtexte

**Pfad:** `Stammdaten > Texte > Systemtexte`

*Abb. B-622: Systemtexte*

In diesem Dialog pflegen Sie die Systemtexte. Diese Texte sind sowohl in Dialogen als auch in Formularen fest verknüpft. Sie können (sinngemäß) geändert werden, z. B. für eine andere Sprache.
-   Tutorial 2, "Systemtexte" auf Seite B-469

> **i Texte nicht löschen**
> Die sinngemäße Änderung von Systemtexten ist erlaubt. Sie dürfen aber weder gelöscht noch dürfen neue hinzugefügt werden. Das Verschieben von Variablen (Platzhaltern) an eine andere Stelle im Text ist möglich.

**Sprache**
Auswahl der Sprache, in der der Text gedruckt werden soll.

**Nummer**
Anzeige der Textnummer.

**Textbearbeitung**
Sie können den Systemtext bearbeiten, z. B. in eine andere Sprache übersetzen.

### Auswahl

In der Übersicht werden die Nummern der Systemtexte angezeigt.

## Mahntexte

**Pfad:** `Stammdaten > Texte > Mahntexte`

*Abb. B-623: Mahntexte*

In diesem Dialog tragen Sie die Mahntexte ein, die Sie bei Mahnungen verwenden wollen. Die Texte dienen nur zur Information.
-   Verkauf, "Mahnwesen" auf Seite C-750

**Bezeichnung**
Namen des Mahntextes.

**Fremdschlüssel**
Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Finanzbuchhaltung.

**Gesperrt**
Einen Mahntext kann für die Erfassung in den Dokumenten gesperrt werden, wenn er nicht mehr benötigt wird.
-   Der Mahntext kann zugewiesen werden.
-   Der Mahntext ist gesperrt und kann nicht mehr zugewiesen werden. Wenn er in Dokumenten zugewiesen ist, wird er jedoch weiterhin angezeigt und gedruckt.

## Dateianhangs-Typen

**Pfad:** `Stammdaten > Texte > Dateianhangs-Typen`

*Abb. B-624: Typen der Dateianhänge*

In diesem Dialog tragen Sie Kennzeichen für Dateianhänge ein. Standardmäßig sind alle Anhänge mit dem Typ A (alle) gekennzeichnet und werden außer bei der Bestellübergabe immer übergeben.

Über die Kennzeichen können Sie die Übergabe von angehängten Dateien (Dokumenten, Abbildungen) steuern:

-   **Produktionsübergabe:** Dateianhänge für Übergabe in OrderXML, z. B. Produktinformationen.
    -   Fertigung, "Einstellungen Produktionsübergabe - Texte/Anlagen" auf Seite E-187
-   **Dokumente kopieren:** Angebot zu Auftrag, z. B. Kalkulationsinformationen.
    -   Verkauf, "Dokumente kopieren - Texte/Anlagen" auf Seite C-559
-   **Bestellübergabe, z. B. Produktinformationen.**
    -   Verkauf, "Erweiterte Einstellungen - Allgemein" auf Seite C-682

## Dateianhangs-Bemerkungen

**Pfad:** `Stammdaten > Texte > Dateianhangs-Bemerkungen`

*Abb. B-625: Bemerkungen für Dateianhänge*

In diesem Dialog hinterlegen Sie Standard-Bemerkungen, die sehr oft benutzt werden. Diese Standard-Bemerkungen werden in der Auftragserfassung > Register Anlagen zur Auswahl angeboten.
-   Verkauf, "Kopfdaten - Anlagen" auf Seite C-443

## Technische Werte

**Pfad:** `Stammdaten > Texte > Technische Werte`

*Abb. B-626: Texte der technischen Werte für Leistungserklärungen*

In diesem Dialog hinterlegen Sie die technischen Werte für die Erzeugung von Leistungserklärungen.

Die Texte müssen für jede Sprache eingetragen werden, damit Leistungserklärung mit den entsprechende Übersetzung der Merkmale in der jeweiligen Sprache erzeugt werden können.

Diese Informationen werden nicht benötigt, wenn der Anwender bereits fertige Leistungserklärungen vorliegen.

# Formulare

**Pfad:** `Stammdaten > Formulare`

Als Formulare werden sowohl die Ausgaben im Druck als auch auf dem Bildschirm bezeichnet. Dazu zählen neben den Dokumenten auch die Listen und Berichte (Reports).

Im Menü Formulare finden Sie folgende Einträge:

-   "Formularverwaltung" auf Seite B-1064
-   "Auftragsformulare" auf Seite B-1082
-   "Druckaufträge" auf Seite B-1083
-   "Crystal Reports" auf Seite B-1089

## Formularverwaltung

**Pfad:** `Stammdaten > Formulare > Formularverwaltung`

In der Formularverwaltung können Sie allgemeine Einstellungen zum Formulardruck bearbeiten. Die Formulare selbst können nur von der A+W Software GmbH geändert werden.

Im Dialog Formularverwaltung finden Sie folgende Register:

-   Formularverwaltung – Formular
-   Formularverwaltung – Kopf-/Fußtexte
-   Formularverwaltung - Texte
-   Formularverwaltung - Optionen 1
-   Formularverwaltung - Optionen 2
-   Formularverwaltung – Skizzendruck
-   Formularverwaltung – Customizing

Die Einstellungen werden für die Druckfunktionen verwendet, z. B. von Auftragsbestätigungen.
-   Verkauf, "Formular-/Etikettendruck" auf Seite C-655

> **i Anbindung an das DMS-System Algeier scanView**
> Bei dem Druckvorgang kann aus dem aktuellen Dokument eine PDF-Datei erstellt und für die DMS Archivierung an das Allgeier scanView System übertragen werden. Diese Funktionalität kann mandanten-übergreifend genutzt werden. Wenden Sie sich an die A+W Software GmbH, wenn Sie Funktionalität nutzen wollen.

### Formularverwaltung – Formular

**Pfad:** `Stammdaten > Formulare > Formularverwaltung > Register Formular`

*Abb. B-627: Formularverwaltung – Formular*

In diesem Register legen Sie zu den einzelnen Druckpunkten fest, welche Formulare für den Druck verwendet werden. Der Druckpunkt entspricht dem Statuspunkt, der programmintern genutzt wird.
-   "Statuszuordnung" auf Seite B-899

#### Druckpunkte

Mit der Wahl der Option legen Sie fest, ob Sie sich Kunden oder Lieferantenformulare anzeigen lassen oder ändern möchten.

-   **Standard:** Die Formulare gelten allgemein.
-   **Kunden, Lieferanten:** Die Formulare gelten für einen Kunden oder einen Lieferanten. Das Feld zur Auswahl des Partners wird freigeschaltet.

**Druckpunkt**
Druckpunkt, dem ein Formular zugeordnet ist. Sie können jedem Druckpunkt beliebig viele Formulare zuordnen. Nachdem einem Formular nach der Ersterfassung ein Druckpunkt zugeordnet ist, kann dieser Druckpunkt nachträglich im Formular nicht geändert werden. Wird z. B. eine Auftragsbestätigung mit dem Druckpunkt `100-AB Druck` gedruckt, so erhält der Auftrag automatisch den Anwenderstatus 21.

#### Formulareinstellungen

**Bezeichnung**
Ihre (firmeninterne) Bezeichnung des Formulars.

**Anzahl**
Nummer der Druckausgaben. Dabei wird jede Seite des Formulars jeweils mehrfach gedruckt. Die Anzahl der Kopien (Durchschläge) geben Sie im Register Optionen 1 an.

**Standard**
Wenn in Ihrer Firma unterschiedliche Formulare für den Druck eines Dokumentes verwendet werden, müssen Sie festlegen, welches der Formulare standardmäßig verwendet wird.
-   Das Formular wird nicht standardmäßig verwendet.
-   Das Formular wird standardmäßig ausgewählt, wenn Sie den entsprechenden Druck starten, z. B. eine Auftragsbestätigung für einen bestimmten Kunden.

**Sprache**
Sprache, der das markierte Formular zugeordnet ist. Dazu muss für jede Sprache je ein entsprechendes Formular angelegen sein. Diese Funktion ist nur aktiv, wenn A+W Business in der mehrsprachigen Variante installiert ist. Jedem Kunden und allen seinen Dokumenten ist eine Sprache zugeordnet. Während des Dokumentendrucks wird das Sprachkennzeichen geprüft und für den Druck das entsprechende Formular ausgewählt. Die Texte werden in der entsprechenden Sprache gedruckt.

**Übersteuerung der Dokumentensprache**
Mit dieser Einstellung können Sie die Sprache übersteuern, die im Feld `Sprache` ausgewählt ist.
-   Das Formular wird der gewählten Sprache entsprechend gedruckt (Standardeinstellung).
-   Die gewählte Sprache wird übersteuert. Markieren Sie die Checkbox dann, wenn Sie z. B. ein Formular als Produktionspapier verwenden. In diesem Fall ist es wichtig, dass das Produktionspapier immer in Ihrer Landessprache gedruckt wird (unabhängig vom Sprachkennzeichen des Dokumentes).

#### Report

**Dateiname**
Zuordnung des Formulars zu einer Report-Datei. Ohne diese Zuordnung können die Berichte nicht erstellt werden. Beispiele von Zuordnungen, die standardmäßig in A+W Business verwendet werden:
-   Angebot = ANGEB.QRP
-   Auftragsbestätigung = AUFTRAG.QRP
-   Lieferschein = LIEFER.QRP
-   Rechnung = RECHN.QRP
-   Gutschrift = GUTSCH.QRP
-   Bestellanfrage = ANFRAGE.QRP
-   Bestellung = BESTELL.QRP

**Druckservice Report**
Auswahl des Druckpunkts, über den der Report erstellt wird. Für Leistungserklärungen muss z. B. der Wert 006 – Declaration of Performance zusammen mit der zum Bericht passenden Sprache eingetragen werden. Zusätzlich kann die Übertragung an das DMS System aktiviert werden.
-   "Dokumentenarchivierung" auf Seite B-1073

**Transfer an iQuote**
Ausgegebene Formulare können auch an iQuote übergeben werden.
-   Das gedruckte Formular wird nicht an iQuote übergeben.
-   Das gedruckte Formular wird an iQuote übergeben.

#### Abweichender Formularstatus

**Statuspunkt**
Sie können jedem Formular einen abweichenden Statuspunkt zuordnen. Diese Zuordnung ist in der Regel nur bei einem Barverkaufsformular nötig. In diesem Fall wählen Sie den Statuspunkt `Barverkauf` aus.
Für den Barverkauf wird standardmäßig eine Barverkaufsrechnung gedruckt. Der Kunden zahlt bar in die Kasse. Für bar bezahlte Aufträge darf keine Rechnung gedruckt werden und die Beträge dürfen nicht an die FiBu übergeben werden.
Sollte in Ihrem System kein Statuspunkt für den Barverkauf existieren, dann legen Sie ihn bitte nur in Absprache mit der A+W Software GmbH an.

#### Leistungserklärung

**Versand per Mail**
Sie können festlegen, mit welchem Druck die Leistungserklärung gesendet werden soll.
-   Beim Druck des ausgewählten Formulars wird keine Leistungserklärung gesendet.
-   Beim Druck des ausgewählten Formulars wird automatisch eine Leistungserklärung per E-Mail gesendet.

#### Formulare

In der Übersicht werden alle Formulare aufgelistet, die den Auswahlkriterien entsprechen.

### Formularverwaltung – Kopf-/Fußtexte

**Pfad:** `Stammdaten > Formulare > Formularverwaltung > Register Kopf-/Fußtext`

*Abb. B-628: Formularverwaltung – Kopf-/Fußtexte*

In diesem Register wählen Sie die Texte aus, die immer auf dem ausgewählten Formular gedruckt werden, z. B., wenn Sie auf allen Ihren Auftragsbestätigungen eine Information über Ihre nächsten Betriebsferien drucken möchten.

> **i Voraussetzung**
> Der gewünschte Text muss im Dialog `Texte` hinterlegt sein.
>
> Die Felder im Bereich `Formulare` sind zum Register `Formular` beschrieben.
> - "Formularverwaltung - Formular" auf Seite B-1065

#### Texte

Über die Lupe können Sie pro Kopf- und Fußtext einen der hinterlegten Text auswählen.
-   "Texte" auf Seite B-1059

**Kopftext**
Der gewählte Text wird im Formularkopf gedruckt.

**Fußtext**
Der gewählte Text wird im Formularfuß gedruckt.

### Formularverwaltung - Texte

**Pfad:** `Stammdaten > Formulare > Formularverwaltung > Register Texte`

*Abb. B-629: Formularverwaltung – Texte*

In diesem Register tragen Sie alle Abweichungen von Standarddruck ein. Die Felder im Bereich `Druckpunkte` und `Formulare` sind zum Register `Formular` beschrieben.
-   "Formularverwaltung - Formular" auf Seite B-1065

**Nicht zu druckende Textkennzeichen**
Kennzeichen der Texte, die nicht auf dem gewählten Formular gedruckt werden sollen. Auf der Auftragsbestätigung sollen z. B. keine Texte mit dem Textkennzeichen `L` für Lieferschein und `P` für Produktion gedruckt werden. Die Einstellung betrifft immer alle Texte des gewählten Textkennzeichens. Um einzelne, ganz bestimmte Texte vom Druck auszuschließen, tragen Sie diese im Feld `Variable Texte` ein.
-   "Textkennzeichen" auf Seite B-1058

**Variable Texte**
Zu jedem Formular können bis zu 10 variable Texte verwaltet werden. Diese Texte werden im Formulardruck beliebig verwendet, z. B. als alternative Überschrift. Die Einstellungen können insbesondere für lieferanten- und kundenspezifische Texte verwendet werden. Die verwendeten Texte müssen in der Textverwaltung angelegt sein.

> **Beispiel**
> Für den Druck von Aufträgen wird nur ein Formular verwendet. Als variable Texte sind die Texte Auftragsbestätigung (1) und Lieferschein (2) eingetragen.
> Wenn der Druck der Auftragsbestätigung gestartet wird, wird automatisch der variable Text 1 ausgewählt und gedruckt. Beim Druck des Lieferscheins wird der Text 2 gedruckt.

### Formularverwaltung – Optionen 1

**Pfad:** `Stammdaten > Formulare > Formularverwaltung > Register Optionen 1`

*Abb. B-630: Formularverwaltung – Optionen 1*

In diesem Register legen Sie fest, wie die Angaben zu den Auftragspositionen gedruckt werden. Die Felder im Bereich `Druckpunkte` und `Formulare` sind zum Register `Formular` beschrieben.
-   "Formularverwaltung - Formular" auf Seite B-1065

#### Kopfwechsel

Mit der Wahl der Option legen Sie den Druck der Produktbezeichnungen fest:
-   **Standard:** Bezeichnung 1 und 2
-   **Kurzbezeichnung:** Kurzinfo
-   **ISO-Aufbau:** Glasbezeichnungen aus Stückliste
-   **Immer:** Der Positionskopf wird immer ausgegeben
    -   "Produktverwaltung" auf Seite B-598

**Mit Modellskizze (siehe Register Skizzendruck)**
Sie können pro Formular festlegen, ob eine Modellskizze gedruckt werden soll. Die Größe und Position der Skizze legen Sie im Register `Skizzendruck` fest.
-   Auf dem gewählten Formular wird keine Modellskizze gedruckt. Diese Einstellung kann nicht durch die Angaben im Auftrag oder in den Stammdaten des Produkts übersteuert werden.
-   Zu jeder Modellposition kann eine Modellskizze gedruckt werden. Die Skizze wird nur dann gedruckt, wenn im Auftrag oder in den Stammdaten des Produktes die entsprechenden Checkboxen markiert sind.
    -   Tutorial 2, "Skizzendruck" auf Seite B-486
    -   "Modellskizze, Sprossenskizze" auf Seite B-609
    -   "Modellskizze, Sprossenskizze" auf Seite B-1080

**SZR in Bezeichnung**
In der Bezeichnung des Produktes kann der Abstandhalter (SZR) mit aufgeführt werden. Dies kann z. B. auf Produktionspapieren wichtig sein.
-   Die Bezeichnung des Abstandhalters wird nicht gedruckt.
-   Die Bezeichnung des Abstandhalters wird der Produktbezeichnung hinzugefügt.

**Modellparameter drucken in**
Mit der Wahl der Option legen Sie die Einheit für die Angabe der Modellmaße fest.
-   **mm/Inch:** Die Maße werden in Millimeter angegeben.
-   **cm/Inch:** Die Maße werden in Zentimeter angegeben.

Die Angabe in Inch wird über die Firmendaten gesteuert:
-   "Maßsystem" auf Seite B-987
Die Größe der Skizze wird im Register `Skizzendruck` festgelegt.
-   "Formularverwaltung - Skizzendruck" auf Seite B-1079

#### Stücklistendruck

Mit der Wahl der Option legen Sie fest, wie die Stückliste gedruckt werden soll:
-   **Standard-Druck:** Die Produktbezeichnungen 1, 2 und 3 aus den Produktstammdaten werden gedruckt.
-   **Stückliste immer drucken:** Die Stückliste wird immer gedruckt, unabhängig vom Druckkennzeichen in den Produktstammdaten. Die Beschaffungsart der Stücklisten-Komponenten wird mit gedruckt.
-   **Entsprechend Druck-Kennz.:** Für den Druck wird das Druckkennzeichen jeder Stücklisten-Komponente abgefragt.
-   **Produktionsrel. Stücklisten:** Nur die produktionsrelevante Stückliste wird gedruckt.

Die Größe der Skizze wird im Register `Skizzendruck` festgelegt.
-   "Formularverwaltung - Skizzendruck" auf Seite B-1079

#### Preisdruck

Sie können pro Formular festlegen, ob die Preise der Auftragspositionen gedruckt werden sollen:
-   **0 - Standard:** Die Einstellung aus dem Auftrag wird für den Druck übernommen. Das Kennzeichen im Auftrag wird aus den Kundendaten übernommen und kann pro Auftrag geändert werden.
-   **1 - Preise immer drucken:** Die Preise werden immer gedruckt, unabhängig davon, was im Auftrag angegeben ist. Diese Einstellung wird z. B. für Rechnungen benutzt.
-   **2- Preise immer drucken (Summenmodus):** Die Einstellung aus dem Auftrag wird für den Druck ausgelesen.
    -   Verkauf, "Darstellung der Preise im Druck" auf Seite C-206
    -   Verkauf, "Formularverwaltung" auf Seite C-207

#### Positionen

**Auf verschiedene Formulare**
Angabe, ob Auftragspositionen auf unterschiedliche Formulare gedruckt werden sollen.
-   Alle Auftragspositionen werden auf dasselbe Formular gedruckt (Standardeinstellung).
-   Die Auftragspositionen können auf unterschiedliche Formulare gedruckt werden. Wenn Sie den Druck starten, wird ein weiterer Dialog angezeigt, der die Gruppierung von verschiedenen Positionen ermöglicht. Sie können dann z. B. ISO-Positionen auf die Produktionspapiere für die ISO-Linie drucken. Positionen, die eine Bearbeitung enthalten, sollen auf dem Produktionspapier gedruckt werden, z. B. das Kantenschleifen auf Papiere für die Schleifmaschine.

#### Dokumentenarchivierung

**Aktiv**
Angabe, ob beim Druck automatisch eine Archivdatei für ein Dokumenten-Management-System (DMS) erstellt wird.
-   Beim Druck des Formulars wird keine Archivdatei erstellt (Standardeinstellung).
-   Beim Druck des Formulars wird automatisch eine Archivdatei erstellt. Diese Einstellung ist dann sinnvoll, wenn Sie mit einem DMS arbeiten, z. B. ELO (Elektronischer Leitz Ordner). Zusätzlich müssen Sie in den Firmendaten den Drucker angeben und das entsprechende Archivierungssystem angeben.
    -   "Dokumentenmanagement" auf Seite B-999
    -   "Wiederholungsdruck für Dokumentenarchivierung" auf Seite B-998

**PDF-Template**
Für den AWSOA Reporting Service kann der Template-Name für PDF-Dateien gespeichert werden. Bei dem Druckvorgang liest der AWSOA Reporting Service die Informationen zu dem jeweiligen Dokument und erstellt die PDF-Datei für die DMS Archivierung in dem Ablageverzeichnis für das Allgeier scanView System. Damit können auch Leistungserklärungen an das Allgeier scanView System erstellt werden.

#### Durchschläge

**Drucker schließen pro Dokument**
Angabe ob der Drucker nach jedem Dokument geschlossen wird.
-   Der Drucker wird nach dem Druck des Formulars nicht geschlossen (Standardeinstellung).
-   Der Drucker wird nach jeder Ausgabe des Formulars geschlossen. Dies ist wichtig, wenn der Drucker z. B. über eine automatische Hefter-Funktion verfügt.

**Anzahl**
Anzahl der Druckausgaben. Dabei wird der Ausdruck pro Dokument mehrfach wiederholt, ohne dass er jeweils neu angestoßen werden muss. Die Einstellung 0 bedeutet, dass genau ein Exemplar gedruckt wird. Mit der Einstellung 1 wird ein zusätzliches Exemplar gedruckt (also zwei identische Exemplare).

### Formularverwaltung – Optionen 2

**Pfad:** `Stammdaten > Formulare > Formularverwaltung > Register Optionen 2`

*Abb. B-631: Formularverwaltung – Optionen 2*

In diesem Register wählen Sie weitere Vorgaben für den Druck auf den Formularen aus. Die Felder im Bereich `Druckpunkte` und `Formulare` sind zum Register `Formular` beschrieben.
-   "Formularverwaltung - Formular" auf Seite B-1065

#### Weitere Optionen

**Kundendaten lesen (Bank)**
Die Bankverbindung kann auf dem gewählten Formular gedruckt werden. Dazu müssen in den Stammdaten des Kunden die entsprechenden Daten in den Feldern `PLZ/Postfach` eingetragen werden.
-   Die Bankverbindungen werden nicht auf dem Formular gedruckt. Dies ist z. B. auf Liefer- und Produktionspapieren sinnvoll.
-   Die Bankverbindungen werden auf dem Formular gedruckt. Dies ist z. B. bei Rechnungsformularen sinnvoll.
    -   "PLZ/Postfach" auf Seite B-773

**Referenzen drucken**
Die Referenzen können auf dem gewählten Formular gedruckt werden, z. B. die Auftragsnummer, zu der eine Bestellung gehört.
-   Die Referenzen werden nicht gedruckt.
-   Die Referenzen werden gedruckt, z. B. bei Bestellungen die zugehörigen Auftrags- und Positionsnummern.

**Preise explizit drucken**
Die impliziten Preise der Stücklisten-Komponenten Bearbeitung können auf dem gewählten Formular gedruckt werden. Die Preise werden nur gedruckt, wenn im Register `Optionen 1` die Optionen `Standard-Druck` oder `Stückliste immer drucken` aktiviert sind.
-   Die Preise der Stücklisten-Komponenten werden nicht explizit gedruckt.
-   Auf dem Formular werden auch die Stücklistenpreise gedruckt.
    -   "Stücklistendruck" auf Seite B-1072
    -   Verkauf: Tutorial, "Manuelle Preisänderung" auf Seite C-144
    -   Verkauf, "Preisdruck" auf Seite C-429

**Gestelldaten drucken**
Die Angaben zu den Packmitteln auf dem gewählten Formular gedruckt werden.
-   Die Angaben zu den Packmitteln werden nicht auf dem Formular gedruckt.
-   Die bei der Kommissionierung dem Auftrag zugeordneten Packmittel werden auf dem Formular gedruckt.

**Kundenindividuelle Artikel drucken**
Die kundenindividuellen Artikel können auf dem gewählten Formular gedruckt werden.
-   Kundenindividuelle Artikel werden nicht auf dem Formular gedruckt.
-   Die im Auftrag enthaltenen kundenindividuellen Artikel werden mit auf das gewählte Formular gedruckt.

**Gestaffelte Zahlungsziele drucken**
Gestaffelte Zahlungsziele und die zugehörigen Beträge aus einem Auftrag können auf dem gewählten Formular gedruckt werden.
-   Die gestaffelten Zahlungsziele werden nicht auf dem Formular gedruckt. Dies ist z. B. bei Produktionspapieren sinnvoll.
-   Die gestaffelten Zahlungsziele werden auf dem Formular gedruckt. Dies ist z. B. bei Rechnungen sinnvoll.
    -   Verkauf: Tutorial, “Fälligkeitsberechnung" auf Seite C-215

**Auswärtige Gestelle drucken**
Angaben zu ausgeliehenen Gestellen können auf dem gewählten Formular gedruckt werden.
-   Die Angaben zu ausgeliehenen Gestellen werden nicht auf das Formular gedruckt.
-   Die Angaben zu ausgeliehenen Gestellen werden auf das Formular gedruckt. Dies ist z. B. sinnvoll, um einen Kunden daran zu erinnern, dass er noch Gestelle zurückzugeben hat.

**Kommission in jeder Position drucken**
Sie können im Dokument pro Auftragsposition einen Kommissionstext eingeben. Dieser Text kann auf dem gewählten Formular gedruckt werden.
-   Der Kommissionstext wird nur für die erste Position gedruckt.
-   Für jede Position wird der Kommissionstext gedruckt, auch wenn der Kommissionstext sich wiederholt.
    -   Verkauf, "Kommission" auf Seite C-467

**Produkttexte nicht wiederholen**
In einem Dokument können mehrere Positionen mit demselben Produkt enthalten sein. Sie können festlegen, ob auf dem gewählten Formular die entsprechenden Produkttexte für jede Position gedruckt werden. Die Produkttexte werden in den Stammdaten des Produktes hinterlegt.
-   Der Produkttext wird immer gedruckt.
-   Wiederholt sich der Produkttext für mehrere aufeinanderfolgende Positionen, dann wird der Text nur für die erste Position aus dieser Gruppe gedruckt.

**Zeitwirtschaftsdaten drucken**
Die Aggregate (Maschinen) zur Anfertigung der Position und der Stückliste können auf dem gewählten Formular gedruckt werden. Diese Daten werden nur für Gläser gedruckt. Diese Einstellung betrifft nur das Modul Kapazitätsplanung.
-   Daten zur Kapazitätsplanung werden nicht gedruckt.
-   Wenn für eine Position Daten zur Kapazitätsplanung vorhanden sind, werden diese auf dem Formular gedruckt.

**Klassifikator-Abfrage**
Zusätzliche Kundeninformationen aus den Klassifikatoren können auf dem gewählten Formular gedruckt werden. Diese Informationen müssen in den Stammdaten des Kunden hinterlegt sein.
-   Die Klassifikatoren werden nicht abgefragt.
-   Die Klassifikatoren werden auf dem Formular gedruckt.
    -   "Partnerverwaltung - Klassifikatoren" auf Seite B-784

**Vorherige Rechnungswerte lesen**
Die Daten der Rechnungen können geprüft werden, bevor das Dokument auf dem gewählten Formular gedruckt wird.

**Produktdaten lesen**
Sie können festlegen, ob die Produktdaten vor dem Druck neu eingelesen werden.
-   Die Produktdaten werden nicht neu eingelesen.
-   Die Produktdaten werden vor dem Druck neu eingelesen.

### Formularverwaltung – Optionen 3

**Pfad:** `Stammdaten > Formulare > Formularverwaltung > Register Optionen 3`

*Abb. B-632: Formularverwaltung – Optionen 3*

In diesem Register wählen Sie weitere Vorgaben für den Druck auf den Formularen aus. Die Felder im Bereich `Druckpunkte` sind zum Register `Formular` beschrieben.
-   "Formularverwaltung - Formular" auf Seite B-1065

#### Optionen für Druckservice

**Abw. Absender bei Mailversand**
In diesem Feld stellen Sie ein, welche Absenderadresse beim Versand der Formulare über Email verwendet werden soll. So lässt sich der Absender auf die Mailadresse des Mitarbeiters ändern wenn diese eingetragen ist. Die Adresse des Mitarbeiters hat bei aktivierter Option immer Vorrang.

**Mail-Betreff**

**Mail-Text**
In diesem Feld können Sie einen oder mehrere Platzhalter für den Mail-Betreff einragen. Diese Platzhalter können vom Druckprogramm mit einem beliebigen Text versehen werden, um eine Möglichkeit zu erhalten, die Mail individuell zu gestalten. Dazu sind in dem Systemtext die Platzhalter in dem Format `<<text1>>`, `<<text2>>` usw. zu verwenden. Es ist zu beachten, dass jeder Platzhalter vom Druckprogramm aus mit einem Text versorgt werden muss. Ansonsten erscheint beim Start des Ausdruckes eine Fehlermeldung. Sobald im Druckprogramm das Formular für den Mailversand ausgewählt wird, aktiviert sich die Lasche `4.Anschreiben(Mail)` und Sie müssen dort die benötigten Platzhalter mit Texten versehen. Es können dafür vorgefertigte Textbausteine in der Textverwaltung angelegt werden, die hier ausgewählt und ggf. noch angepasst werden können.

**Absender des Mitarbeiters**
In diesem Feld haben Sie Möglichkeit, die E-Mailadresse des Mitarbeiters als Absender zu verwenden. Dadurch ist eine direktere Kommunikation zwischen dem Endkunden und dem Mitarbeiter möglich, da der Endkunde direkt auf die E-Mail antworten kann.

**Pfad für PDF-Datei**
Um die Ausgabe des Formular-Druckes in eine Datei umzuleiten, existiert hier die Möglichkeit, einen Pfad und einen Dateinamen zu hinterlegen. Es wird empfohlen für den Pfad ein UNC Pfad zu verwenden auf den der Reporting Service Zugriff hat. Der Dateiname kann mit Platzhaltern versehen werden, um so auf den Inhalt der Datei hinzuweisen. Die möglichen Platzhalter werden durch klicken auf die Schaltfläche vor dem Dateinamen angezeigt und können so auch gleich übernommen werden.

**PDF Datei abfragen**
Wenn Sie diese Checkbox aktivieren, können Sie den Dateinamen vor dem Speichern noch anzupassen.

### Formularverwaltung – Skizzendruck

**Pfad:** `Stammdaten > Formulare > Formularverwaltung > Skizzendruck`

*Abb. B-633: Formularverwaltung – Skizzendruck*

In diesem Register legen Sie fest, wie groß eine Modellskizze und der zugehörige Text gedruckt werden. Im Register `Optionen 1` legen Sie fest, ob Modell- und/oder Sprossenskizzen gedruckt werden sollen.
Die Felder im Bereich `Druckpunkte` und `Formulare` sind zum Register `Formular` beschrieben.
-   "Formularverwaltung - Formular" auf Seite B-1065

> **i Voraussetzung**
> Sie benötigen für den Skizzendruck Shaping & Nesting für A+W Business. Die Einträge aus diesem Register werden nur dann berücksichtigt, wenn im Register `Optionen 1` die Checkbox mit `Modellskizze` aktiviert ist.
>
> In A+W Business besteht auch die Möglichkeit, eine Seite pro Modellposition zu drucken. Hierfür muss ein entsprechendes Formular für den Druckpunkt 544 Modellskizze angelegt werden.

#### Modellskizze, Sprossenskizze

**Druckmodus (Einschränkung)**
Auswahl zur Einschränkung des Skizzendrucks:
-   **Kein Druck:** Auf dem gewählten Formular wird keine Skizze gedruckt.
-   **Modell (maßstäblich), Sprosse (maßstäblich):** Auf dem gewählten Formular können maßstabsgetreue Skizzen gedruckt werden. Für den Druck werden die Maße aus den Feldern `Höhe x Breite der Skizze` herangezogen.
-   **Modell (schematisch), Sprosse (schematisch):** Auf dem gewählten Formular werden die Standardskizzen gedruckt, ohne die Maße zu berücksichtigen. Maßstäbliche Druckeinstellungen im Auftrag werden nicht berücksichtigt.

**Breite x Höhe der Skizze**
Max. Breite und Höhe der maßstabsgetreuen Skizze. Der Druck von Sprossenkonstruktionen muss in den Firmendaten aktiviert werden.
-   "Skizzendruck" auf Seite B-997

**Maßangaben**
Textgröße bei Sprossen, damit diese Angaben im gedruckten Dokument gut gelesen werden können. Der Standardwert ist x 1,00. Das bedeutet, dass die Texte in Originalgröße gedruckt werden.

#### Textgröße der Modellskizzen

Sie können die Textgröße auf die Größe der Modellskizze abstimmen.

**Maßangaben**
Textgröße der Maße, damit die Werte im gedruckten Dokument gut gelesen werden können. Der Standardwert ist 12 px (Pixel).

**Segmenttext**
Textgröße der Segmenttexte, damit die Texte im gedruckten Dokument gut gelesen werden können. Der Standardwert ist 12 px.

**Decotexte**
Textgröße in Formen, damit diese im gedruckten Dokument gut gelesen werden können. Der Standardwert ist 6 px.

### Formularverwaltung – Customizing

**Pfad:** `Stammdaten > Formulare > Formularverwaltung > Register Customizing`

*Abb. B-634: Formularverwaltung – Customizing*

In diesem Register legen Sie fest, an welcher Position auf dem gewählten Formular ein bestimmter Abschnitt beginnt. Dafür müssen die entsprechenden Formeln hinterlegt sein.
-   "Formeln" auf Seite B-1045

> **i Formel für den Formulardruck**
> Wenn Sie Formeln benötigen oder eine Formel anpassen müssen, wenden Sie sich bitte an die A+W Software GmbH.

Die Felder im Bereich `Druckpunkte` und `Formulare` sind zum Register `Formular` beschrieben.
-   "Formularverwaltung - Formular" auf Seite B-1065

## Auftragsformulare

**Pfad:** `Stammdaten > Formulare > Auftragsformulare`

*Abb. B-635: Formularverwaltung für den Direktdruck*

In diesem Dialog ordnen Sie Formulare für den Direktdruck zu. Diese Zuordnungen werden im Dialog `Dokumentenverwaltung` in der Gruppe `Druck > Direktdruck` aufgelistet.
-   Verkauf, "Menü Start" auf Seite C-415

### Einstellungen

**Bezeichnung**
Namen, mit dem der Direktdruck in der Dokumentenverwaltung angezeigt wird.

**Dokumententyp**
Zuordnungen des Direktdrucks zum Dokumententyp. Die Zuordnung ist für alle Dokumententypen möglich, die in der Liste angezeigt werden:
-   Angebot
-   Auftrag, inklusive Auftragsbestätigung, Lieferschein, Rechnung, Reklamation usw.
-   Bestellanfrage
-   Bestellung
-   Gutschrift

**Druckpunkt**
Druckpunkt, der durch den Druck mit dem gewählten Formular vergeben wird. Daraus resultiert der Anwenderstatus, den das Dokument erhält.
-   "Statusverwaltung" auf Seite B-897

**Drucker**
In der Regel wird der Direktdruck einen Systemdrucker zugeordnet. Der gewählte Drucker muss allen Arbeitsplätzen zur Verfügung stehen, an denen der Druck gestartet wird.

**Formular**
Formular für den Direktdruck.

**Rückfrage vor Druck**
Der Direktdruck kann wahlweise sofort oder nach einer Abfrage gestartet werden.
-   Der Formulardruck wird sofort und ohne weitere Abfrage gestartet.
-   Nach der Auswahl des Direktdruckformulars werden Sie gefragt, ob Sie das Formular drucken möchten (Ja/Nein). Erst nach Bestätigung mit Ja wird der Formulardruck gestartet.

## Druckaufträge

**Pfad:** `Stammdaten > Formulare > Druckaufträge`

*Abb. B-636: Druckaufträge*

In diesem Dialog verwalten Sie die Druckaufträge. Sie können über die Definition von Druckaufträgen mehrere Druckläufe hintereinanderschalten, die automatisch auf dem Printserver ausgeführt werden, z. B.:
-   Drucken der Auftragsbestätigungen für interne Zwecke.
-   Wiederholungsdruck für ein Fax pro Kunde.
-   Wiederholungsdruck als E-Mail an den Vertreter.

Abhängig von der Rechnerleistung des Printservers kann außerdem eingestellt werden, wie viele Ausgabeprozesse von unterschiedlichen Mitarbeitern gleichzeitig laufen können.

> **i Druckläufe auf dem Printserver anlegen**
> Wenn Sie keinen lokalen Drucker verwenden, erfassen Sie die Druckläufe am besten direkt auf dem Server, da in der Kombobox `Drucker` nur die auf dem Rechner installierten Drucker angezeigt werden.

### Druckauftrag

Alle Einstellungen in diesem Bereich gelten jeweils nur für den ausgewählten Druckauftrag.

**Bezeichnung**
Namen des Druckauftrags, z. B. AB Druck 2-fach.

**Dokumententyp**
Dokumententyp, für den der Druckauftrag eingerichtet ist, z. B. für Angebote.

### Nummernkreis

**Nummer aus AV-Bereich Dokument**
Wenn Sie mit Mandanten und/oder AV-Bereichen arbeiten, können Sie in einem Druckauftrag festlegen, dass die Dokumenten-Nummer aus den zugeordneten Nummernkreisen genommen wird. Damit können Sie Druckläufe für bestimmte Mandanten und/oder AV-Bereiche festlegen.
-   Mit diese Einstellung müssen Sie in den Mandanten und den AV-Bereich auswählen, die für die Vergabe der Rechnungs- und Lieferscheinnummer relevant sind.
-   Für die Vergabe der Rechnungs- und Lieferscheinnummer wird der Mandant und AV-Bereich aus dem Dokument genommen. Die Felder zur Auswahl des Mandanten und der AV-Bereich werden gesperrt.

**Mandant**
Mandant, aus dessen Nummernkreis die Dokumenten-Nummer genommen werden soll. Diese Kombobox ist nur freigeschaltet, wenn die Checkbox `Nummer aus AV-Bereich Dokument` deaktiviert ist.

**Bereich**
AV-Bereich, aus dessen Nummernkreis die Dokumenten-Nummer genommen werden soll. Diese Kombobox ist nur freigeschaltet, wenn die Checkbox `Nummer aus AV-Bereich Dokument` deaktiviert ist.

### Formularauswahl

Zu einem Druckauftrag können ein oder mehrere Druckläufe definiert werden. Auf dem Printserver werden diese Druckaufträge in der Reihenfolge abgearbeitet, in der sie in der Übersicht angezeigt werden.
Bei der Sortierung müssen Sie unbedingt die Reihenfolge der Statusvergabe beachten. Die Position der Druckläufe können Sie über die Pfeil-Schaltflächen verschieben.
Die Mehrzahl der nachfolgenden Einstellungen für den Druck über den Server kann während des Formulardrucks nicht mehr verändert werden.
-   Verkauf, "Formular-/Etikettendruck" auf Seite C-655

> **i Reihenfolge gemäß Statusvergabe**
> Achten Sie bei der Formularzuordnung auf die Reihenfolge im Hinblick auf die Statusvergabe: Nach jedem Drucklauf wird der Status des Dokuments aktualisiert, vor dem Druck werden der Sperr- und der Mindeststatus geprüft.
> Zum Beispiel kann der Lieferschein immer erst nach dem Druck einer Auftragsbestätigung gedruckt werden.

**Formular**
In diesem Feld wählen Sie das Formular aus. Von dem im Formular vergebenen Druckpunkt hängt ab, welche der nachfolgenden Checkboxen freigeschaltet sind.
-   "Formularverwaltung" auf Seite B-1064

**Drucker**
In diesem Feld wählen Sie das Gerät aus, auf dem die Dokumente ausgegeben werden sollen, z. B. Drucker, Fax.

**Übersicht**
In der Übersicht werden alle Druckläufe aufgelistet, die in dem gewählten Druckauftrag enthalten sind. Die Druckläufe werden in der angegebenen Reihenfolge gestartet. Bei der Sortierung müssen Sie unbedingt die Reihenfolge der Statusvergabe beachten. Die Position der Druckläufe können Sie über die Pfeil-Schaltflächen verschieben.

-   **[Hinzufügen]** Fügt ein weiteres Formular hinzu.
-   **[Entfernen]** Entfernt ein markiertes Formular aus dem Drucklauf.

### Druckmodus

Mit der Wahl der Option legen Sie den Druck von Etiketten fest. Die Optionen werden freigeschaltet, wenn Sie ein Formular für Etiketten ausgewählt haben.
-   **Pro Einheit:** Pro Stück wird ein Etikett gedruckt.
-   **Pro Position:** Pro Position wird ein Etikett gedruckt.
-   **Pro Auftrag:** Pro Auftrag wird ein Etikett gedruckt.
-   **Nach Dokumenteneinstellung:** Die Einstellungen aus dem Dokument sollen übernommen werden.

### Sonderdruck

**Wiederholungsdruck**
Die Checkbox kann nicht manuell markiert werden. Sie ist automatisch mit der Auswahl eines Formulars für den Wiederholungsdruck (WH) aktiviert.
-   Der Wiederholungsdruck ist nicht aktiv, wenn Sie z. B. ein Formular für Auftragsbestätigungen gewählt haben, dem der Druckpunkt 100 - AB Druck zugewiesen wurde.
-   Der Wiederholungsdruck ist aktiv, wenn Sie ein Formular für den Wiederholungsdruck gewählt haben, dem z. B. der Druckpunkt 200 - Auftragsbestätigung WH zugewiesen wurde.

**Dokumentenarchivierung**
Wenn Sie mit einem Dokumenten-Management-System (DMS) arbeiten, können Sie die Dokumente in diesem DMS zusätzlich archivieren, z. B. in Saperion. Dazu muss die entsprechende Schnittstelle eingerichtet sein.
-   Die Dokumente werden nicht an ein DMS übergeben.
-   Die Dokumente werden während dieses Drucklaufs automatisch an das angeschlossene DMS übergeben.
    -   "Schnittstellen-Dienst" auf Seite B-1046

**Sammelausdruck**
Rechnungen können als Sammeldruck ausgegeben werden, wenn diese Option in den Stammdaten des Kunden aktiviert ist. Zu einer Sammelrechnung werden alle Aufträge eines Kunden zusammengefasst, in denen das entsprechende Kennzeichen aktiviert ist. Für den Sammeldruck müssen die Dokumente im Nummernverwalter nach Kunden und dem Auswahlkriterium sortiert sein.
-   In diesem Druckauftrag werden keine Sammelrechnungen gedruckt. Die Kombobox für die Auswahl der Kriterien ist gesperrt.
-   Die Dokumente eines Kunden, bei dem das Kennzeichen Sammelrechnung aktiviert ist, werden beim Druck zusammengefasst. Die Kombobox für die Auswahl der Kriterien ist freigeschaltet:
    -   **Immer:** Diese Einstellung überschreibt die Einstellung zum Sammeldruck aus den Stammdaten.
    -   **Pro Bestelltext 1:** Alle Dokumente für einen Kunden werden nach dem Bestelltext 1 gefiltert und zusammengefasst. Wenn z. B. für einen Kunden 10 Aufträge vorhanden sind, von denen fünf den gleichen Bestelltext 1 haben, werden sechs Auftragsbestätigungen gedruckt.
    -   **Pro Lieferadresse:** Alle Dokumente mit derselben Lieferanschrift werden zusammengefasst.
    -   **Standard:** Alle Dokumente mit demselben Kunden/Lieferanten werden zusammengefasst, wenn das Kennzeichen für den Sammeldruck gesetzt ist.
        -   "Partnerverwaltung - Finanzen" auf Seite B-785
        -   Verkauf: Tutorial, “Sammelrechnungsdruck" auf Seite C-33
        -   Verkauf, "Teillieferung, Teilfaktura, Sammelrechnung" auf Seite C-434

**Einschränkung Betrag**
Sie können festlegen, ob der Betrag vor dem Druck abgefragt wird:
-   **Alle Dokumente:** Alle Dokumente werden gedruckt, der Betrag wird nicht geprüft.
-   **Betrag ungleich 0:** Dokumente ohne Betrag oder mit einem Betrag = 0 werden bei Druck übersprungen. Das können auch Dokumente mit negativem Wert sein.
-   **Betrag größer 0:** Nur die Dokumente werden gedruckt, per Fax oder per E-Mail versendet, deren Auftragssumme größer als Null ist.

**Nur Postversand**
Der Druckauftrag gilt nur für Dokumente, die per Post versendet werden.
-   Alle Dokumente werden dem Formular entsprechend ausgegeben.
-   Die Dokumente werden auf Papier gedruckt, damit sie per Post versendet werden können.

**Faxversand**
Diese Checkbox ist automatisch markiert, wenn Sie ein Fax-Formular ausgewählt haben. Der Faxversand muss in den Stammdaten des Marktpartners aktiviert und eine Faxnummer hinterlegt sein. Für den Faxversand muss die entsprechende Faxschnittstelle und Software eingerichtet sein.
-   Die Dokumente werden nicht per Fax versendet.
-   Die Dokumente werden automatisch als Fax versendet.
    -   "Partnerverwaltung - Adresse" auf Seite B-771
    -   "Schnittstellen-Dienst" auf Seite B-1046

**Faxversand an Vertreter**
Diese Checkbox ist nur freigeschaltet, wenn Sie ein Fax-Formular ausgewählt haben.
-   Die Dokumente werden nicht per Fax an den Vertreter gesendet.
-   Die Dokumente werden per Fax an den Vertreter gesendet. Die Faxnummer muss in den Mitarbeiterdaten hinterlegt sein.
    -   "Mitarbeiter" auf Seite B-1022

**Mail**
Diese Checkbox kann nicht manuell markiert werden. Für den E-Mail-Versand muss die entsprechende Schnittstelle und Software eingerichtet sein.
-   Das gewählte Formular kann nicht als E-Mails gesendet werden.
-   Das gewählte Formular kann als E-Mail gesendet werden. Die Optionen werden freigeschaltet:
    -   **an Kunde:** Mit dieser Option wird ein Dokument an die E-Mail-Adresse des Kunden geschickt. In den Stammdaten des Kunden muss der Dokumentenversand per E-Mail aktiviert und eine E-Mail-Adresse hinterlegt sein.
    -   **an Vertreter:** Mit dieser Option wird ein Dokument an die E-Mail-Adresse des Vertreters geschickt. Sie muss in den Mitarbeiterdaten hinterlegt sein.
        -   "Dokumentenversand" auf Seite B-776
        -   "Mitarbeiter" auf Seite B-1022
        -   "Schnittstellen-Dienst" auf Seite B-1046

**Archivjahr abfragen**
Sie können in einem Druckauftrag definieren, ob das Archivjahr berücksichtigt werden soll, das im Formulardruck eingestellt ist. Dies ist beim Jahreswechsel sinnvoll, wenn die gedruckten Dokumente anschließend automatisch archiviert werden.
-   Das Archivjahr wird nicht abgefragt.
-   Das Archivjahr wird beim Druck abgefragt.
    -   Verkauf, "Archiv" auf Seite C-550

**Druckdatum abfragen**
Sie können in einem Druckauftrag definieren, ob das (manuell eingegebene) Druckdatum berücksichtigt werden soll. Beim Druck von Rechnungen im Dialog `Formulardruck` kann das Rechnungsdatum im Feld `Druckdatum` verändert werden.
-   Das Druckdatum wird nicht abgefragt.
-   Das Druckdatum wird abgefragt. Dies ist z. B. für den Rechnungsdruck sinnvoll.
    -   Verkauf, "Druckdatum" auf Seite C-657

**Nicht optimierte Gläser**
Die Checkbox ist freigeschaltet, wenn Sie ein Formular für Etiketten ausgewählt haben.
-   Für Positionen mit Gläsern, die nicht optimiert wurden, werden keine Etiketten gedruckt.
-   Auch für Positionen mit Gläsern, die nicht optimiert wurden, werden Etiketten gedruckt.

### Druckaufträge

In der Übersicht werden alle gespeicherten Druckaufträge aufgelistet. Wenn Sie einen Eintrag markieren, können Sie die zugehörigen Einstellungen bearbeiten.

## Crystal Reports

**Pfad:** `Stammdaten > Formulare > Crystal Reports`

*Abb. B-637: Verfügbare Reports*

In diesem Dialog hinterlegen Sie Hyperlinks zu Crystal Reports `*.RPT`-Dateien. Zusätzlich können Sie für jeden Report eine Beschreibung eingeben und eine Datenquelle und Mitarbeiter bzw. Mitarbeitergruppen zuordnen. Die Ausführung der Reports kann über Mitarbeiterrechte für bestimmte Mitarbeiter verhindert bzw. zugelassen werden.
Der Ausdruck der Crystal Reports wird in einem gesonderten Modul erzeugt, das über das A+W Business-Startmenü erreichbar ist.

### Zuordnung

**Pfad:** `Stammdaten > Formulare > Crystal Reports > Report markieren > Kontextmenü (rechte Maustaste) > Mitarbeiter, Gruppe zuordnen`

*Abb. B-638: Zuordnung*

In diesem Dialog ordnen Sie einem Report einen Mitarbeiter oder eine Mitarbeitergruppe zu.

# CEKAL

**Pfad:** `Stammdaten > CEKAL`

In Frankreich wird mit dem Zertifikat CEKAL gearbeitet. Isoliergläser, die mit diesem Zertifikat gekennzeichnet sind, müssen definierten Qualitätskriterien entsprechen. Diese Kriterien legen Sie in den Dialogen dieses Menüs fest.

> **i Voraussetzungen**
> Die Dialoge zur CEKAL-Zertifizierung sind nur freigeschaltet, wenn in den Firmendaten das Produktkennzeichen `CEKAL-Klassifizierung` ausgewählt ist.
>
> - "Produktkennzeichnung" auf Seite B-946

Im Menü CEKAL finden Sie folgende Einträge:

-   "Klassen" auf Seite B-1092
-   "Zuordnung" auf Seite B-1093
-   "Ergebnisse" auf Seite B-1094
-   "Textzuordnung" auf Seite B-1095
-   "Restriktionen" auf Seite B-1097
-   "Produkttexte" auf Seite B-1099

## Klassen

**Pfad:** `Stammdaten > CEKAL > Klassen`

*Abb. B-639: CEKAL Klassen*

In diesem Dialog legen Sie Variablen (Platzhalter) für die verschiedenen CEKAL-Klassen an. Diese Variablen werden für die Standardtexte benötigt. Sie werden in der Dokumentenerfassung automatisch durch die Texte ersetzt, die aus den CEKAL-Regeln resultieren.

> **i Voraussetzungen**
> Der Dialog ist nur freigeschaltet, wenn in den Firmendaten das Produktkennzeichen `CEKAL-Klassifizierung` ausgewählt ist.
>
> - "Produktkennzeichnung" auf Seite B-946

### Tabelle

**Nr.**
Nummer der Klasse.

**Bezeichnung**
Name der Klasse.

**Platzhalter**
Selbst definierter Platzhalter (Variable) für die Klasse. Beachten Sie dabei, dass einige Variablen eine feste Bedeutung in A+W Business haben.
-   Tutorial 2, "Verfügbare Variablen (Platzhalter)" auf Seite B-533

**Ebene**
Stücklistenebene, bis zu der die CEKAL-Prüfung durchgeführt werden soll. Standardmäßig steht dieser Eintrag auf Null.
-   0: Prüfung auf Hauptproduktebene
-   1: Prüfung auf der ersten Stücklistenebene

**Fremdschlüssel**
Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Produktion.

## Zuordnung

**Pfad:** `Stammdaten > CEKAL > Zuordnung`

*Abb. B-640: CEKAL-Zuordnung*

In diesem Dialog ordnen Sie jedem einzelnen Glasprodukt, das in eine ISO-Einheit eingebaut wird, eine Klasse zu und tragen den dazugehörigen Wert ein.

> **i Voraussetzungen**
> Der Dialog ist nur freigeschaltet, wenn in den Firmendaten das Produktkennzeichen `CEKAL-Klassifizierung` ausgewählt ist.
>
> - "Produktkennzeichnung" auf Seite B-946

**Produkt**
Produkt, dem eine Klasse zugeordnet ist.

**Klasse**
Zugeordnete Klasse.

**Ebene**
Strukturseite, für die die Zuordnung gilt.

**Wert**
CEKAL-Wert des Produkts. Mehrere Produkte können den gleichen CEKAL-Wert haben. Wurde er bereits einmal erfasst, steht er in der Kombobox zur Auswahl. Die Werte werden im Dialog `Ergebnisse` zur Auswahl angeboten.

**Bemerkung**
Bemerkung zur weiteren Information.

## Ergebnisse

**Pfad:** `Stammdaten > CEKAL > Ergebnisse`

*Abb. B-641: CEKAL Ergebnisse*

In diesem Dialog können Sie die CEKAL-Werte, die Sie im Dialog `Zuordnung` den unterschiedlichen Produkten zugeordnet haben, miteinander kombinieren. Aus diesen Kombinationen resultieren die verschiedenen CEKAL-Ergebnisse.

Während der Positionserfassung werden die Kombinationen abgefragt. Das für die Position zutreffende CEKAL-Ergebnis wird als Positionstext in das Dokument übernommen.

> **i Voraussetzungen**
> Der Dialog ist nur freigeschaltet, wenn in den Firmendaten das Produktkennzeichen `CEKAL-Klassifizierung` ausgewählt ist.
>
> - "Produktkennzeichnung" auf Seite B-946

### Zuordnung

**Klasse**
Klasse, für die das Ergebnis angelegt ist.

**Ergebnis**
Bezeichnung für das Ergebnis. Den Ergebnissen können im Dialog `Textzuordnung` die Texte zugeordnet werden, die der Klassifizierung entsprechen.

**Bemerkung**
Bemerkung zur Zuordnung.

### Elemente

**Elemente 1 - 10**
Pro CEKAL-Ergebnis können Sie maximal 10 unterschiedliche CEKAL-Werte zuordnen. Die Werte der Elemente sind im Dialog `Zuordnung` hinterlegt.

## Textzuordnung

**Pfad:** `Stammdaten > CEKAL > Textzuordnung`

*Abb. B-642: CEKAL Textzuordnung*

In diesem Dialog geben Sie an, welche Texte bei welchen Ergebnissen gedruckt werden sollen. Nur die Texte können zugeordnet werden, die im Dialog `Texte` hinterlegt sind.
-   "Texte" auf Seite B-1059

> **i Voraussetzungen**
> Der Dialog ist nur freigeschaltet, wenn in den Firmendaten das Produktkennzeichen `CEKAL-Klassifizierung` ausgewählt ist.
>
> - "Produktkennzeichnung" auf Seite B-946

### Klassen

In diesem Bereich werden Felder für alle Klassen angezeigt, die im Dialog `Klassen` angelegt sind.
-   "Klassen" auf Seite B-1092

**Klasse 1 bis 10**
Ergebnis, zu dem ein Text ausgegeben werden soll. Wenn Sie einen Standard-CEKAL-Text anlegen wollen, lassen Sie alle Klassenfelder leer. In den Textfeldern tragen Sie die Nummern für den Standard-CEKAL-Text ein. Dieser wird immer dann übernommen, wenn in der Dokumentenerfassung keinerlei Ergebnisse zu den Klassen gefunden wurden.

### Bieger

**Nummer**
Textnummer, die an den Bieger übergeben werden soll. Wenn Sie eine Textnummer eingetragen haben, wird der unten angegebene Biegertext nicht mehr berücksichtigt.

### Texte

Nummer des Textes, der jeweils angezeigt werden soll.

**Allgemein**
Dieser Text wird auf den Formularen gedruckt und kann bis zu 80 Zeichen betragen.

**Etikett**
Dieser Text wird auf den Etiketten gedruckt und muss entsprechend kurz sein.

**Produktion**
Dieser Text wird auf den Produktionspapieren (in A+W Business oder Produktionssoftware) gedruckt. Er dient internen Zwecken.

**Bieger**
Dieser Text kann an den Rahmenbieger übergeben werden, vorausgesetzt der Bieger kann diese Texte einlesen. Wenn Sie im Bereich `Bieger` im Feld `Nummer` eine Nummer eingetragen haben, wird der Text aus dem Feld `Bieger` nicht berücksichtigt.

### Textzuordnung

In der Übersicht werden die Textzuordnungen pro Klasse aufgelistet.

## Restriktionen

**Pfad:** `Stammdaten > CEKAL > Restriktionen`

*Abb. B-643: CEKAL Restriktionen*

In diesem Dialog hinterlegen Sie die Restriktionen, die bei der CEKAL-Prüfung berücksichtigt werden.

Mit Hilfe dieser Restriktionen können technische Werte abgefragt werden, z. B. das Scheibenmaß oder die Sprossendicke. Bei Über- oder Unterschreitung der Werte erfolgt keine CEKAL-Klassifizierung.

> **i Voraussetzungen**
> Der Dialog ist nur freigeschaltet, wenn in den Firmendaten das Produktkennzeichen `CEKAL-Klassifizierung` ausgewählt ist.
>
> - "Produktkennzeichnung" auf Seite B-946

### Restriktionswerte

**Nummer**
Die Nummern sind vom System vorgegeben.

**Parameter 1 bis 4**
Werte für die einzelnen Parameter der Restriktion. Die Anzahl der änderbaren Parameter hängt von der ausgewählten Restriktion ab.

**Bemerkung**
Anzeige der vorgegebenen Texte zur Restriktion.

### Texte

**Allgemein**
Dieser Text wird auf den Formularen gedruckt und kann bis zu 80 Zeichen betragen.

**Etikett**
Dieser Text wird auf den Etiketten gedruckt und muss entsprechend kurz sein.

**Produktion**
Dieser Text wird auf den Produktionspapieren (in A+W Business oder Produktionssoftware) gedruckt. Er dient internen Zwecken.

**Bieger**
Dieser Text kann an den Rahmenbieger übergeben werden, vorausgesetzt der Bieger kann diese Texte einlesen. Wenn Sie im Bereich `Bieger` im Feld `Nummer` eine Nummer eingetragen haben, wird der Text aus dem Feld `Bieger` nicht berücksichtigt.

**Bieger Nummer**
Textnummer, die an den Bieger übergeben werden soll. Wenn Sie eine Textnummer eingetragen haben, wird der oben angegebene Biegertext nicht berücksichtigt.

### Restriktionen

In der Übersicht werden alle Restriktionen aufgelistet, die bei der Prüfung berücksichtigt werden können.

## Produkttexte

**Pfad:** `Stammdaten > CEKAL > Produkttexte`

*Abb. B-644: CEKAL-Produkttexte*

In diesem Dialog hinterlegen Sie für spezielle Produkte CEKAL-Texte, die sich auf eine bestimmte Strukturebene beziehen. Wenn ein solches Produkt Bestandteil einer Isolierglaseinheit ist, hat dieser CEKAL-Text absolute Priorität vor den anderen CEKAL-Texten.

> **i Voraussetzungen**
> Der Dialog ist nur freigeschaltet, wenn in den Firmendaten das Produktkennzeichen `CEKAL-Klassifizierung` ausgewählt ist.
>
> - "Produktkennzeichnung" auf Seite B-946

### Produktauswahl

**Produkt**
Produkt, dem ein spezieller Produkttext zugeordnet ist.

**Ebene**
Strukturebene, für die der Text gilt.

**Bemerkung**
Kurze Beschreibung, die den Text erläutert.

### Texte

**Allgemein**
Dieser Text wird auf den Formularen gedruckt und kann bis zu 80 Zeichen betragen.

**Etikett**
Dieser Text wird auf den Etiketten gedruckt und muss entsprechend kurz sein.

**Produktion**
Dieser Text wird auf den Produktionspapieren (in A+W Business oder Produktionssoftware) gedruckt. Er dient also internen Zwecken.

**Bieger**
Dieser Text kann an den Rahmenbieger übergeben werden, vorausgesetzt der Bieger kann diese Texte einlesen. Wenn Sie im Bereich Bieger im Feld `Nummer` eine Nummer eingetragen haben, wird der Text aus dem Feld `Bieger` nicht berücksichtigt.

**Bieger Nummer**
Dieser Text kann an den Rahmenbieger übergeben werden, vorausgesetzt der Bieger kann diese Texte einlesen. Wenn Sie im Bereich Texte eine Bieger-Nummer eingetragen haben, wird der hier eingetragene Biegertext nicht berücksichtigt.

### Textzuordnung

In der Übersicht werden die strukturbezogenen Textzuordnungen aufgelistet.

# CE-Kennzeichen

**Pfad:** `Stammdaten > CE-Kennzeichen`

Isoliergläser, die mit diesem Zertifikat gekennzeichnet sind, müssen fest definierten Qualitätskriterien entsprechen.

Der CPIP-Code (Characteristic Performance Identification Paper) wird nur in Frankreich benötigt. Er enthält Kenndaten zu den Eigenschaften und dem Leistungsverhalten.

Im Menü CE-Kennzeichen finden Sie folgende Einträge:
-   "CPIP-Code" auf Seite B-1101
-   "Maßrestriktionen" auf Seite B-1102
-   "ISO-Suchdaten" auf Seite B-1103
-   "Restriktionen" auf Seite B-1097
-   "Einstellungen" auf Seite B-1104

## CPIP-Code

**Pfad:** `Stammdaten > CE-Kennzeichen > CPIP-Code`

*Abb. B-645: CE-Kennzeichen - CPIP-Code*

In diesem Dialog legen Sie Details zu einem CPIP-Code fest, z. B. die Gültigkeit, ob er zertifiziert wurde und ob er einer CE-Norm entspricht.

Die Standards und Regeln zur CPIP-Bildung können im Dialog `Einstellungen` eingelesen werden.
-   "Einstellungen" auf Seite B-1104

In der Produktverwaltung muss der CPIP-Code bei den entsprechenden Produkten angegeben werden.

> **i CE-Kennzeichen mit CPIP-Code**
> Der CPIP-Code (Characteristic Performance Identification Paper) wird nur in Frankreich benötigt. Er enthält Kenndaten zu den Eigenschaften und dem Leistungsverhalten.

## Maßrestriktionen

**Pfad:** `Stammdaten > CE-Kennzeichen > Maßrestriktionen`

*Abb. B-646: CE-Kennzeichen - Maßrestriktionen*

In diesem Dialog hinterlegen Sie die Maßrestriktionen für CPIP-Codes.

Während der Auftragserfassung wird geprüft, ob CE relevante Maßrestriktionen an der aktuellen Position überschritten sind. Bei Verletzung einer Restriktion wird ein entsprechender Hinweis angezeigt.

## ISO-Suchdaten

**Pfad:** `Stammdaten > CE-Kennzeichen > ISO-Suchdaten`

*Abb. B-647: ISO-Suchdaten*

In diesem Dialog pflegen Sie die Daten für den CPIP-Code für Isoliergläser. Diese Daten steuern das Verhalten der Auftragserfassung.

> **i Neuen Datensatz anlegen**
> Wenn Sie einen neuen Datensatz anlegen, müssen Sie für Sprossen einen Default-Wert eintragen.
>
> Werte, die im ISO nicht vorgegeben sind, werden mit Standards belegt, um in den Suchdaten den CPIP-Code zu ermitteln.

### Tabelle

In diesem Bereich werden alle Suchdaten aufgelistet, die im System hinterlegt sind.

## Einstellungen

**Pfad:** `Stammdaten > CE-Kennzeichen > Einstellungen`

*Abb. B-648: CE-Kennzeichen – Einstellungen*

In diesem Dialog importieren Sie die Dateien mit den erforderlichen CPIP-Codes und weiteren Definitionen. Die Schnittstellendateien werden mit dem `^`-Zeichen getrennt. Außerdem muss die erste Zeile die Spaltennamen enthalten.

Der Import kann je nach Größe der Datei einige Zeit dauern.

### Standardwerte für ISO-Suchfunktion

In diesem Bereich werden die Standard-Werte für Nicht-Glas-Komponenten gepflegt.

### Datei-Update CPIP-Code

In diesem Bereich können einzelne Datenbank-Tabellen über Schnittstellendateien gefüllt werden. Dazu wählen Sie die Datei aus und starten den Vorgang anschließend über die Schaltfläche [Laden].

# B2B

**Pfad:** `Stammdaten > B2B`

In diesem Programmbereich sind Schnittstellen-Daten für den Datenaustausch hinterlegt.

Im Menü B2B finden Sie folgende Einträge:
-   "Produkte (Kunde, Lieferant)" auf Seite B-1105
-   "Kopieren von Fremdartikeln" auf Seite B-1113
-   "SZR (Kunde, Lieferant)" auf Seite B-1114
-   "Gas (Kunde, Lieferant)" auf Seite B-1115
-   "Touren (Kunde, Lieferant)" auf Seite B-1116
-   "Kunde, Lieferant" auf Seite B-1117
-   "Dokumentenexport" auf Seite B-1123
-   "SN-Datei-Regeln" auf Seite B-1126
-   "Artikelimport" auf Seite B-1127
-   "Preisimport" auf Seite B-1129

## Produkte (Kunde, Lieferant)

**Pfad:** `Stammdaten > B2B > Kunde, Lieferant > Produkt`

Aufträge können über EDI importiert und Bestellungen können exportiert werden. Für Kunden und Lieferanten werden die Produktdaten für diesen Datenaustausch getrennt gepflegt. Die Dialoge sind identisch aufgebaut. Sie werden in dieser Anleitung am Beispiel Kunde beschrieben.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
-   "Menü Funktionen" auf Seite B-1105
-   "Produkte - Stückliste" auf Seite B-1106
-   "Produkte - Parameter" auf Seite B-1108
-   "Produkte - Tabelle" auf Seite B-1109
-   "Produkte - Modelle/Bearbeitungen" auf Seite B-1110
-   "Produkte - Sprossen" auf Seite B-1111

### Menü Funktionen

**Pfad:** `Stammdaten > B2B > Kunde, Lieferant > Produkt > Menü Funktionen`

Über dieses Menü können Sie die Daten exportieren. Folgende Einträge werden angezeigt:

-   **Dorma-Referenz erstellen:** Bezüge zu den Dorma-Artikeln erstellen. Mit dieser Funktion wird im Matchcode immer die Fremdartikelnummer des Produktes bei Dorma angelegt. Die Funktion ist nur für Lieferanten freigeschaltet.
-   **Artikel kopieren:** Öffnet den Dialog `Kopieren von Fremdartikeln`, um die Artikel des aktuellen Kunden zu kopieren.
    -   "Kopieren von Fremdartikeln" auf Seite B-1113

### Produkte – Stückliste

**Pfad:** `Stammdaten > B2B > Kunde, Lieferant > Produkt > Register Stückliste`

*Abb. B-649: Produkte – Stückliste*

In diesem Register ordnen Sie die eigenen Glas-Produkte den Produkten des Marktpartners zu.

#### Fremdartikel

**Partner**
Marktpartner, für den die Zuordnung gilt.

**Gültig ab**
Datum, ab dem die Zuordnung gilt.

**Artikelnummer**
Alphanumerische Artikelnummer, die der Marktpartner verwendet.

**Bezeichnung**
Bezeichnung, die der Marktpartner verwendet.

#### Identifikation

**Artikel/MCode**
Artikelnummer (Produktnummer) aus den Stammdaten von A+W Business.

**Bezeichnung**
Bezeichnung aus den Stammdaten.

**Breite / Höhe**
Maße, die für den Marktpartner gelten.

**Farbe**
Farbvariante, die für den Markpartner gilt.

**Preise / PE**
Preis pro Preiseinheit.

#### Stücklistenartikel

Die Felder in diesem Bereich sind nur freigeschaltet, wenn in der Stückliste eine Komponente markiert ist.

**Artikel/MCode**
Artikelnummer (Produktnummer) der markierten Stücklisten-Komponente.

**Bezeichnung**
Bezeichnung der markierten Stücklisten-Komponente.

**Menge / Breite / Höhe**
Angaben bei Kisten.

**Farbe**
Farbvariante der markierten Stücklisten-Komponente.

**Strukturebene**
Strukturebene der markierten Stücklisten-Komponente.

**Strukturverlauf**
Strukturverlauf der markierten Stücklisten-Komponente.

**Beschichtungsseite**
Beschichtungsseite der markierten Stücklisten-Komponente.

#### Stückliste

In der Übersicht wird die Stückliste des ausgewählten Produkts angezeigt. Wenn Sie eine Komponente markieren, werden die Details im Bereich `Stückliste` angezeigt.

### Produkte – Parameter

**Pfad:** `Stammdaten > B2B > Kunde, Lieferant > Produkt > Register Parameter`

*Abb. B-650: Produkte - Parameter*

In diesem Register geben Sie an, ob bei der Rechnungskontrolle die korrespondierende Produktnummer automatisch gesucht und eingetragen wird.
Wenn Sie mit der elektronischen Rechnungskontrolle über openTRANS arbeiten, können Sie die Referenzen automatisch eintragen lassen.

### Produkte - Tabelle

**Pfad:** `Stammdaten > B2B > Kunde, Lieferant > Produkt > Register Tabelle`

*Abb. B-651: Produkte - Tabelle*

In diesem Register werden alle zugeordneten Produkte aufgelistet.

### Produkte – Modelle/Bearbeitungen

**Pfad:** `Stammdaten > B2B > Kunde, Lieferant > Produkt > Register Modelle/Bearbeitungen`

*Abb. B-652: Produkte – Modelle/Bearbeitungen*

In diesem Register legen Sie die Parameter für Modelle und Bearbeitungen fest. Die Felder sind ausführlich zu den Stammdaten der Produkte und im Part Verkauf beschrieben.
-   "Produktverwaltung - Modelle/Bearbeitungen" auf Seite B-622

### Produkte – Sprossen

**Pfad:** `Stammdaten > B2B > Kunde, Lieferant > Produkt > Register Sprossen`

*Abb. B-653: Produkte - Sprossen*

In diesem Register legen Sie die Parameter für Sprossen(-Konstruktionen) fest. Die Felder sind ausführlich zu den Stammdaten der Produkte und im Part Verkauf beschrieben.
-   "Produktverwaltung - Sprossen" auf Seite B-636

### Produkte – Anlagen

**Pfad:** `Stammdaten > B2B > Kunde, Lieferant > Produkt > Register Anlagen`

*Abb. B-654: Produkte – Anlagen*

In der Definition der Referenzen für B2B Produkte können jetzt Dateianhänge hinterlegt werden. Diese Anhänge werden beim Import in die jeweiligen Auftragspositionen übertragen. Hierbei werden allerdings nur die Verweise auf die Dateien übertragen. Eine Kopie der eigentlichen Dateien in die Ordner-Strukturen der Dokumentenanhänge erfolgt nicht. Dieses Verhalten wird in der Tabelle in der Positionserfassung mit einem entsprechenden Link-Symbol dargestellt.

## Kopieren von Fremdartikeln

**Pfad:** `Stammdaten > B2B > Kunde, Lieferant > Produkt > Menü Funktionen > Artikel kopieren`

*Abb. B-655: B2B – Kopieren von Fremdartikeln*

In diesem Dialog können Sie die Daten eines Partners kopieren und auf einen anderen Partner übertragen.

## SZR (Kunde, Lieferant)

**Pfad:** `Stammdaten > B2B > Kunde, Lieferant > SZR`

*Abb. B-656: B2B - Abstandhalter (SZR)*

In diesem Dialog ordnen Sie die eigenen SZR-Produkte den Produkten des Marktpartners zu.

Für Kunden und Lieferanten werden die Daten der Abstandhalter für den Datenaustausch getrennt gepflegt. Die Dialoge sind identisch aufgebaut.

Die Felder sind ausführlich zum Dialog `Produkte` beschrieben.
-   "Produkte - Stückliste" auf Seite B-1106

## Gas (Kunde, Lieferant)

**Pfad:** `Stammdaten > B2B > Kunde, Lieferant > Gas`

*Abb. B-657: B2B - Gas*

In diesem Dialog ordnen Sie die eigenen Gas-Produkte den Produkten des Marktpartners zu.

Für Kunden und Lieferanten werden die Daten der Gase für den Datenaustausch getrennt gepflegt. Die Dialoge sind identisch aufgebaut.

Die Felder sind ausführlich zum Dialog `Produkte` beschrieben.
-   "Produkte - Stückliste" auf Seite B-1106

## Touren (Kunde, Lieferant)

**Pfad:** `Stammdaten > B2B > Kunde, Lieferant > Touren`

*Abb. B-658: B2B - Touren*

In diesem Dialog ordnen Sie die eigenen Touren den Touren des Marktpartners zu.

Für Kunden und Lieferanten werden die Daten der Touren für den Datenaustausch getrennt gepflegt. Die Dialoge sind identisch aufgebaut.

Die Felder sind ausführlich zum Dialog `Produkte` beschrieben.
-   "Produkte - Stückliste" auf Seite B-1106

## Kunde, Lieferant

**Pfad:** `Stammdaten > B2B > Kunde, Lieferant > Kunde, Lieferant`

Für Kunden und Lieferanten werden die Einstellungen für den Datenaustausch per EDI getrennt gepflegt. Die Dialoge sind identisch aufgebaut. Sie werden in dieser Anleitung am Beispiel Kunde beschrieben.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
-   "Menü Funktionen" auf Seite B-1105
-   "Kunde, Lieferant - Auswahl" auf Seite B-1117
-   "Kunde, Lieferant - Parameter" auf Seite B-1119
-   "Kunde, Lieferant - Tabelle" auf Seite B-1122

### Menü Funktionen

**Pfad:** `Stammdaten > B2B > Kunde, Lieferant > Kunde, Lieferant > Menü Funktionen`

Über dieses Menü können Sie ein Command-Skript importieren oder exportieren.

### Kunde, Lieferant – Auswahl

**Pfad:** `Stammdaten > B2B > Kunde, Lieferant > Kunde, Lieferant > Register Auswahl`

*Abb. B-659: B2B - Partnerauswahl*

In diesem Register legen Sie die Einstellungen für die EDI-Schnittstelle pro Marktpartner fest.

#### Partner

**Nummer**
Nummer des Marktpartners, mit dem Sie Daten per EDI austauschen wollen.

**Filialnummer**
Nummer der Filiale des Marktpartners.

**Abweichender Partner für Artikelreferenzierung**
Nummer des Marktpartners, auf dessen Artikel verwiesen werden soll, wenn für den aktuellen Marktpartner keine eigenen Referenzen hinterlegt sind.

#### Schnittstelle

**Typ**
Schnittstellenversion. Wenn Sie Auftragsbestätigungen und Rechnungen ebenfalls elektronisch austauschen (openTRANS-Format), müssen Sie die Version wählen, mit der Sie die Daten bisher übertragen haben. Die Version wird bei der Installation von A+W Business festgelegt.

#### Laufnummer der Zieldatei

**Von, Aktuell, Bis**
Erste und letzte und zuletzt vergebene Nummer des Nummernkreises für die Laufnummern der Übergabe.

#### Pfadangaben

**Quellpfad, Quelldatei**
Verzeichnis und Dateinamen für die Import-/Exportdatei.

**Eine Datei pro Dokument**
Diese Checkbox wird nur für Lieferanten angezeigt.
-   Alle Bestellungen eines Lieferanten werden in eine Datei geschrieben.
-   Beim Export wird eine Datei pro Bestellung erzeugt.

**Protokollpfad, Protokolldatei, Sicherungspfad**
Angabe der Verzeichnisse und Dateinamen für die Protokoll- und die Sicherungsdatei.

#### Command-Skript

In diesem Bereich können Sie ein Skript eintragen, mit dem Sie die EDI-Dateien modifizieren und kopieren können.

### Kunde, Lieferant – Parameter

**Pfad:** `Stammdaten > B2B > Kunde, Lieferant > Kunde, Lieferant > Register Parameter`

*Abb. B-660: B2B – Schnittstellenparameter*

In diesem Register legen Sie die Parameter für den Datenaustausch per EDI fest. Die Felder in den Bereichen `Partner` bis `Laufnummer` sind zum Register `Auswahl` beschrieben.
-   “Kunde, Lieferant - Auswahl" auf Seite B-1117

#### Parameter

**Zwangsreferenzierung**
In der Regel sind die Referenzen auf die Kunden- oder Lieferantenprodukte vollständig eingerichtet. Sie müssen jedoch entscheiden, was bei fehlenden Referenzen gemacht werden soll.
-   Die Produktnummer aus den Stammdaten wird in die Schnittstellendatei geschrieben. Das ist z. B. dann sinnvoll, wenn das sendende und das empfangende System den gleichen Produktstammdaten benutzen. In dem Fall ist es nicht nötig, Daten in die Referenztabellen einzutragen.
-   Wenn eine Position ohne Referenz auf ein (externes) Produkt gesendet wird, kann diese Position ignoriert werden. In diesem Fall wird eine Fehlermeldung im Logbuch eingetragen.

**Locking aktiv, Maximale Lock-Zeit**
Wenn mehrere Mitarbeiter mit den gesendeten Daten arbeiten, kann das Ihr System stark belasten.
-   Die Schnittstellendatei wird nicht gesperrt. Diese Einstellung ist sinnvoll, wenn nur ein Programm auf die Datei zugreift.
-   Für den eingegebenen Zeitraum kann nur ein Programm auf dieselbe Schnittstellendatei zugreifen. Das Feld für die Angabe des Zeitraums wird freigeschaltet.

**Vorgabe der Dokumentennummer erlaubt**
Die Dokumentennummer kann importiert oder von A+W Business vergeben werden.
-   Die Dokumentennummer wird von A+W Business vergeben.
-   Die Dokumentennummer kann aus der EDI-Datei importiert werden, sofern noch keine Nummer vergeben wurde. Wenn bereits eine Nummer vergeben ist, wird eine Fehlermeldung angezeigt.

**Stückliste komplett aus Schnittstellendatei übernehmen**
Die Stückliste kann aus der Schnittstellendatei oder aus den Stammdaten der Produkte erstellt werden.
-   Die Stückliste wird aus den Stammdaten der Produkte übernommen.
-   Die Stückliste wird aus dem Aufbau in der EDI-Referenzierung ausgewählt.

**Maßsystem**
Mit der Wahl der Option legen Sie fest, wie die Maße in der Schnittstellendatei interpretiert werden sollen. Die Einstellung zum Maßsystem wird übergreifend in den Firmendaten festgelegt. Diese Standard-Einstellung kann pro Kunde in den Stammdaten und in den Dokumenten übersteuert werden. Für den Import müssen Sie daher angeben, welches Maßsystem importiert wird.

**Maß-Präzision = 1/**
Bei Aktivierung des imperialen Maßsystems für die Schnittstellendatei geben Sie den Wert 32, 64 oder 128 ein, je nachdem, mit welchem Faktor die Berechnungen erfolgen sollen. Wenn Sie mit dem metrischen Maßsystem arbeiten, tragen Sie im Feld `Maß-Präzision` den Wert 1 ein.

**Dokument im Fehlerfall nicht generieren**
In der Schnittstellendatei können Fehler enthalten sein, auf die das System reagieren muss.
-   Aus den Daten der Schnittstellendatei wird immer ein Auftrag erzeugt.
-   Wenn Fehler in der Schnittstellendatei enthalten sind, wird kein Auftrag erzeugt. Beim Import wird ein entsprechender Hinweis angezeigt. Im Protokoll können Sie den Fehler suchen und korrigieren. Danach können die Daten erneut eingelesen werden.

**Restriktionsüberschreitung weist Position zurück**
In der Schnittstellendatei können Positionen enthalten sein, die die Restriktionen in A+W Business verletzen.
-   Positionen mit Restriktionsverletzungen werden unverändert übernommen. Die Aufträge müssen anschließend manuell nachbearbeitet werden.
-   Positionen mit Restriktionsverletzungen werden nicht übernommen. Im Protokoll können Sie den Fehler prüfen und korrigieren.

**Austausch bei Restriktionsverletzung**
Wenn in der Schnittstellendatei Positionen enthalten sind, die die Restriktionen in A+W Business verletzen, können automatisch Austauschprodukte eingesetzt werden.
-   Positionen mit Restriktionsverletzungen werden unverändert übernommen. Die Aufträge müssen anschließend manuell nachbearbeitet werden.
-   Bei Positionen mit Restriktionsverletzungen werden automatisch die in A+W Business definierten Austauschprodukte eingesetzt.

**Reklamationen zulassen**
Reklamationen können wahlweise über die Schnittstelle eingelesen werden.
-   In aller Regel werden Reklamationen nicht zugelassen, sondern als "normaler" Auftrag importiert. Danach wird geprüft, ob es eine Reklamation ist.
-   Reklamationen sind nicht zugelassen.
-   Reklamationen sind zugelassen.

**Grundproduktwechsel bei 2x Austausch**
Wenn in einer Position mehr als 2 Komponenten ausgetauscht sind, kann ein automatisch anderes A+W Business-Produkt eingesetzt werden.
-   Die Positionen werden unverändert übernommen.
-   Wenn in einer Position zwei Komponenten ausgetauscht sind, wird automatisch das Grundprodukt eingesetzt, das in der Produktverwaltung angegeben ist.
    -   "Grundprodukt" auf Seite B-613

**Geringerwertige Kantenbearbeitung entfernen**
Angabe, ob bei Kantenbearbeitungen alle Bearbeitungen auch dann ausgeführt werden sollen, wenn sie sich nur in der Qualität unterscheiden, z. B. Säumen und Polieren am ESG.
-   Alle Kantenbearbeitungen werden so ausgeführt, wie sie erfasst sind.
-   Nur die höherwertige Kantenbearbeitung wird ausgeführt. Die geringerwertige Kantenbearbeitung wird ignoriert. Sollte dadurch eine Kantenbearbeitung auf keine Kante mehr wirken, so wird die komplette Bearbeitung aus der Stückliste entfernt. Siehe dazu auch die Einstellung in den Firmendaten.
    -   "Firmendaten - Parameter" auf Seite B-948

**Bearbeitungsparameter prüfen**
Beim EDI-Import können die Bearbeitungsparameter im Bearbeitungssatz geprüft werden.
-   Bearbeitungsparameter werden nicht geprüft.
-   Bearbeitungsparameter werden nicht geprüft. Wenn Parameter nicht gesetzt oder Werte unzulässig sind, werden diese automatisch korrigiert. Bei Kantenbearbeitungen wird z. B. die Anzahl der markierten Kanten geprüft, d. h. wenn kein Modell vorhanden ist, können logischerweise maximal 4 Kanten bearbeitet werden.

**Import von Marktpartner individuellen Texten**
Angabe, ob individuelle Texte des Marktpartners importiert werden sollen.
-   Diese Texte werden nicht importiert.
-   Diese Texte werden importiert.

#### Preise

**Preisimport/-export zulassen**
Angabe, ob Preise importiert und exportiert werden oder nicht.

**Berechnung von Zuschlägen/Rabatten deaktivieren**
Angabe, ob Zuschläge und Rabatte berechnet werden sollen.
-   Zuschläge und Rabatte werden berechnet. Damit wird der in der EDI-Datei definierte Preis unverändert in das Dokument übernommen.
-   Zuschläge und Rabatte werden nicht berechnet.

### Kunde, Lieferant – Tabelle

**Pfad:** `Stammdaten > B2B > Kunde, Lieferant > Kunde, Lieferant > Register Tabelle`

*Abb. B-661: B2B - Tabelle der Kunden, Lieferanten*

In diesem Register sind alle Kunden oder Lieferanten aufgelistet, die angelegt sind. Für die Marktpartner, für die die Datenübergabe per EDI eingerichtet wurde, wird der Pfad der Schnittstellendatei angezeigt.

## Dokumentenexport

**Pfad:** `Stammdaten > B2B > Kunde > Dokumentenexport`

*Abb. B-662: Einstellungen für den openTrans-Export*

In diesem Dialog legen Sie die Einstellungen für den Export im openTrans-Format pro Kunde fest. In diesem Format können Auftragsbestätigungen, Lieferavise und Rechnungen übertragen werden.

Die openTRANS-Dateien haben die Dateiendung *.awotdis, *.awotres oder .awotinv.

### Kunde

**Nummer**
Nummer des Marktpartners, dem Sie Dokumente im openTrans-Format senden wollen.

### Schnittstelle

**Typ**
Schnittstellenversion. Wenn Sie Auftragsbestätigungen und Rechnungen ebenfalls elektronisch austauschen (openTRANS-Format), müssen Sie die Version wählen, mit der Sie die Daten bisher übertragen haben. Die Version wird bei der Installation von A+W Business festgelegt.

**Exportart**
Dokumente können als Datei oder als Anhang in einer E-Mail gesendet werden:
-   **Export in eine Datei:** Mit dieser Einstellung werden die Daten in eine Datei geschrieben. Das Feld für den Zielpfad wird freigeschaltet. Sie können ein Verzeichnis auswählen oder den Pfad manuell eintragen.
-   **Export per e-Mail:** Mit dieser Einstellung werden die Daten als Anhang einer E-Mail gesendet. Die Checkbox für die abweichende E-Mail-Adresse wird freigeschaltet.

**Auftragsbestätigungen, Rechnungen, Lieferavis, Gutschriften exportieren**
Diese Dokumentenarten können im openTrans-Format ausgetauscht werden.
-   Die jeweilige Dokumentenart wird nicht im openTrans-Format exportiert.
-   Die jeweilige Dokumentenart wird im openTrans-Format exportiert.

### Einstellungen

In diesem Bereich haben Sie die Möglichkeit in eine Komma - separierte Liste Artikelnummern (z. B. 6530, 6600) einzutragen, die beim Export nicht berücksichtigt werden sollen. Diese Artikelnummern werden dann nicht in die openTRANS Datei geschrieben. Die Einstellung kann man nur für openTRANS 2.1 vornehmen. Des Weiteren gilt dies nur für Auftragsbestätigungen.

### Export in Datei

Das Feld für den Zielpfad ist nur freigeschaltet, wenn Sie `Export in eine Datei` gewählt haben.

**Zielpfad**
Sie können ein Verzeichnis auswählen oder den Pfad manuell eintragen.

**Dateiendung**
Es stehen Ihnen folgende Dateiendungen zur Auswahl zur Verfügung:
-   0 - Default
-   1 - XML Datei (*.XML).

### Export per E-Mail

**Spezielle E-Mail-Adresse für den Export verwenden**
Die Checkbox ist nur freigeschaltet, wenn Sie `Export per E-Mail` gewählt haben.
-   Für die Übertragung per E-Mail werden die Adressen aus den Stammdaten verwendet. Dazu müssen Sie prüfen, ob in den Stammdaten des Kunden die E-Mail-Adresse korrekt eingetragen ist.
-   Für die Übertragung per E-Mail sollen abweichende E-Mail-Adressen verwendet werden. Die Felder für die jeweilige Dokumentenart werden freigeschaltet.

**Für ABs, Rechnungen, Lieferavis**
Pro Dokumentenart können Sie eine eigene E-Mail-Adresse angeben.

### Register Tabelle

In diesem Register sind alle Kunden aufgelistet, die angelegt sind.

## SN-Datei-Regeln

**Pfad:** `Stammdaten > B2B > Kunde > SN-Datei Regeln`

*Abb. B-663: Regeln für die Erzeugung einer SN-Datei*

In diesem Dialog legen Sie fest, für welche Produktarten/-gruppen bei der Produktionsübergabe (OrderXML) automatisch eine SN-Datei erzeugt werden soll. Diese Datei wird in die Stückliste gehängt. Damit entfällt die manuelle Erstellung pro Position.

Bei der Übergabe an A+W Production wird diese SN-Datei in aller Regel von A+W Production erzeugt.

## Artikelimport

**Pfad:** `Stammdaten > B2B > Artikelimport`

*Abb. B-664: Artikelimport*

In diesem Dialog können Sie alle Artikelstammdaten importiert, die nicht über BMECat importiert werden können und in der Auswählliste vorkommen.

Die Einstellungen für den BMECat-Import legen Sie in den Firmendaten fest.
- "Firmendaten - Sonstiges" auf Seite B-1018

### Parameter

**Artikelliste**
Auswahl der Artikelliste. Zur Auswahl werden alle Artikellisten angeboten, die in dem Verzeichnis abgelegt sind, das im Feld `Quell-Datei` angegeben ist.

**Matchcode-Präfix**
Die Artikelnummern können beim Import mit einem Präfix versehen werden, z. B. mit den Anfangsbuchstaben des Lieferanten. Damit sind sie in den Stammdaten deutlich zu erkennen.

**Mandant**
Der Artikelimport für eine bestimmte Datenbank bestimmt sein.

**Quell-Datei**
Auswahl der Artikel-Datei, die importiert werden soll.

**Produktart, Produktgruppe**
Produktart und Produktgruppe, denen die importierten Artikel zugeordnet werden sollen.

**WGR, WGR-Statistik**
Warengruppe und Warengruppe für die Statistik, denen die importierten Artikel zugeordnet werden sollen.

**Jahrgang, Schlüssel**
Preisjahrgang und -schlüssel, in denen die Preise für die importierten Artikel gepflegt werden.

**Artikelnummer von, bis**
Auswahl der Artikelnummern, die importiert werden sollen.

**Erste Preistabelle für Produktfarben**
Für die Varianten können unterschiedliche Preistabellen verwendet werden. Das bedeutet, dass zu einem Produkt mehr als eine Preistabelle vorhanden ist. Darum müssen Sie angeben ab welcher freien (Tabellen-)Nummer die Preistabellen angelegt werden sollen.

**Skizzen**
Verzeichnis, in dem die importierten Artikelskizzen gespeichert werden sollen.

**Beschaffungsart**
Auswahl der Beschaffungsart, die den importierten Artikeln zugeordnet werden soll.

**Lagerbuchungsart**
Auswahl der Lagerbuchungsart, die den importierten Artikeln zugeordnet werden sollen. Das Feld ist nur freigeschaltet, wenn die Beschaffungsart `Lagerentnahme` gewählt wurde. Eine ausführliche Beschreibung der Lagerbuchungsarten finden Sie im Part Lagerverwaltung.

### Übersicht Artikel

In der Übersicht sind alle Artikel aufgeführt, die in der ausgewählten Artikelliste enthalten sind. Die Checkbox `Neu` ist direkt nach dem Import/Update markiert. Sie können daran erkennen, welche Einträge geändert sind.

## Preisimport

**Pfad:** `Stammdaten > B2B > Preisimport`

*Abb. B-665: Preisimport*

In diesem Dialog können Sie die VEGLA-Preisdaten importiert.
