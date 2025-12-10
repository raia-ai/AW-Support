---
title: "D-AWBusiness-HB_7"
source: "D-AWBusiness-HB_7.pdf"
tags: ["A+W Business", "Stammdaten", "Softwarereferenz", "Kalkulation", "Preisberechnung", "Tutorial", "German", "ERP", "Produktionsdaten", "Änderungsüberwachung"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document serves as a technical reference and tutorial for the A+W Business software, focusing on master data (Stammdaten) management. It covers various supplementary information for Tutorial 2, including price definitions, system texts, and variables. Additionally, it provides a detailed software reference for configuring products, pricing, calculations, and data exchange with A+W Production."
long_description: "A comprehensive guide and software reference for the A+W Business system, presented in German. The first part of the document, 'Tutorial 2 - Zusatzinformationen', provides supplementary details for a tutorial session. This includes tables and explanations for price definition types, available system texts and placeholders (variables), handling of special glass types like leaded glass, and change tracking (Änderungsüberwachung). It also details the process for data transfer between A+W Business and A+W Production. Key topics covered are mixed pricing calculations (Mischkalkulation), French pricing methods, general cost calculation (Kalkulation), and managing contribution margin limits (Deckungsbeitrags-Grenzwerte). The second, larger part of the document is a 'Softwarereferenz' (Software Reference). This section provides an in-depth overview of the master data module, detailing configurations for general settings (languages, calendars), products (product types, groups, variants), pricing structures, and inventory management. It elaborates on the 'Produktverwaltung' (Product Management) dialog, covering the configuration of articles across various aspects like production, pricing, warehousing, and BOMs (Stückliste). The document is intended for system administrators and advanced users responsible for setting up and maintaining the master data that drives the A+W Business ERP system."
---
---
## Tutorial 2: Zusatzinformationen

### Grenztypen für die Preisdefinition

**Tab. B-25 Grenztypen für die Preisdefinition (Abschnitt 4 von 4)**

| Grenztyp | Beschreibung | Beispiel |
| :--- | :--- | :--- |
| **WGR Fremdkey** | Mit Hilfe des Fremdschlüssels können Preise nach Warengruppen berechnet werden. | **Beispiel:** Bearbeitungen für ESG und VSG. |
| **WGR Fremdkey exakt** | | |
| **Zuschlagsnettobasis** | Energiezuschlag in Prozent für Gläser. Basis für den Energiezuschlag ist die Summe der Nettopreise aller Gläser innerhalb eines Auftrages. Der Zuschlag wird automatisch als Auftragsposition 900 eingefügt. | **Beispiel:**<br>bis zu 1000,00 = 5% Zuschlag<br>ab 1000,00 = 2% Zuschlag |

---

### Verfügbare Systemtexte

**Tab. B-26 Systemtexte**

| Nr. | Text | |
| :--- | :--- | :--- |
| 1 | Modell | |
| 2 | ;unten:;rechts:;oben:;links:;Scheibe; S | Vermaßung der Stufe |
| 3 | Glas wird mitgeliefert! | |
| 50 | Rechnung <ar> v. <ard> f. Anzahlung v. <ad> | Anzahlungen |
| 51 | Anzahlung v. <ad> für Auftr. <aa> vom <aad> | Anzahlungen |
| 100 | Abrechnungssumme original %X1 | Nr. 100 bis 108: |
| 101 | Vorherige Veränderungen %X2 | Objektverwaltung DMS |
| 102 | Veränderungen mit dieser Rechnung %X3 | |
| 103 | Gesamtveränderung %X4 | |
| 104 | Abrechnungssumme neu %X5 | |
| 105 | - Nicht fertige Arbeiten %X6 | |
| 106 | Wert der kompletten Arbeit %X7 | |
| 107 | - Vorherige Forderungsrechnung %X8 | |
| 108 | HEUTIGE FORDERUNG NR.%X9 %X10 | |
| 110 | Ug-Wert in W/qm | Techn. ISO-Parameter |
| 111 | Ug-Wert nach DIN 4108-4 | Techn. ISO-Parameter |
| 112 | Lichtdurchl. in % | Techn. ISO-Parameter |
| 113 | g-Wert in % | Techn. ISO-Parameter |
| 114 | b-Faktor | Techn. ISO-Parameter |
| 115 | Schalldämmmaß in dB | Techn. ISO-Parameter |
| 116 | Dickentoleranz in mm | Techn. ISO-Parameter |
| 117 | Größentoleranz mm (<200 cm) | Techn. ISO-Parameter |
| 118 | Größentoleranz mm (>=200 cm) | Techn. ISO-Parameter |
| 119 | Sprossen im SZR, einfach | Versicherungspreisliste |
| 120 | Sprossen im SZR, mehrfach | Versicherungspreisliste |

⇨ Softwarereferenz, "Systemtexte" auf Seite B-1060
⇨ Tutorial 2, "Texte anlegen" auf Seite B-477

---

### Verfügbare Variablen (Platzhalter)

In Texten können Variablen eingefügt werden, die erst im Dokument gefüllt werden.

**Formel**
<@Formelnummer@> = Ausführung einer Formel mit der Nummer (nn)

⇨ "Variablen" auf Seite B-473

#### Allgemein

**Tab. B-27 Variablen**

| Bereich | Variable | Bedeutung |
| :--- | :--- | :--- |
| **Allgemein** | %X1, %X2, %X3 usw. | Variablen, die durch A+W Business mit den entsprechenden Werten gefüllt werden.<br>⇨ Softwarereferenz, "Systemtexte" auf Seite B-1060 |
| **Anzahlung** | <aa> | Anzahlungsauftragsnummer |
| **Anzahlung** | <aad> | Anzahlungsauftragsdatum |
| **Anzahlung** | <ad> | Anzahlungsdatum |
| **Anzahlung** | <ar> | Anzahlungsrechnungsnummer |
| **Anzahlung** | <ard> | Anzahlungsrechnungsdatum |
| **CEKAL** | <h> | Firmennummer aus den Firmendaten |
| **CEKAL** | <jj> | Jahr und Quartal im Format JJJJ-QQ |
| **CEKAL** | <p1> | Bezeichnung 1 |

---

### Bearbeitungen

| Variable | Bedeutung |
| :--- | :--- |
| `<%>` | Anzahl (Kanten, Bohrungen, Eckausschnitte, ...) |
| `<$>` | Hauptparameter (Durchmesser, Radius, Breite, Höhe) |
| `<§>` | Ergänzungsparameter (welche Kanten, Ecken oder x, y, d bei Bohrungen) |
| `<=>` | Berechnete Ifm |
| `<?>` | Berechnete qm |

| Bezeichnung 3 in Produktverwaltung | Bearbeitungsdialog, Positionserfassung |
| :--- | :--- |
| <%> Kanten [<§>] mit Gehrung 45° poliert (<=> Ifm) | 2 Kanten [2/3] mit Gehrung 45° poliert (2,45 Ifm) |
| Sägen von <%> Kanten *<>* | Sägen von 3 Kanten *2/3/4* |
| <%> Lochbohrung(en) mit d = <$> mm | 2 Lochbohrungen mit d = 20 mm |
| <%> Bohrung(en) d=<$>mm X, Y [<§>] | 2 Bohrungen d = 20 mm X, Y [100, 100] |
| <%> x <$> mm Rundecke [<§>] | 4 x 15 mm Rundecke [1/2/3/4] |
| <$> Eckausschnitte / <%> Stück / [<§>] | 100 x 75 Eckausschnitte / 2 Stück / [3/4] |

### Rahmentexte

Die Rahmentexte können im Produkt eingetragen werden und verweisen auf die Standardtexte. Soll beim Kunden nur eine Nummer übergeben werden, so muss dort eine Nummer in den Standardtext eingetragen werden. Der gesamte Text kann mit Variablen übergeben werden.

**Tab. B-28 Variablen für Rahmentexte**

| Variable | Bedeutung |
| :--- | :--- |
| <ab> | Abstandhalterkurzbezeichnung |
| <ak> | Abstandhalterkennzeichen |
| <an> | Auftragsnummer, ohne führende Null oder Leerzeichen |
| <br> | Breite, ohne führende Null oder Leerzeichen |
| <c1> | Kundenname 1 |
| <cn> | Kundennummer |
| <esg> | ESG Kurzbezeichnung |
| <g> | Gas |
| <gt> | Gütetext |
| <ho> | Höhe, ohne führende Null oder Leerzeichen |
| <kp> | Kundenposition |
| <no> | Auftragsnummer/Position |
| <p1> | Produktbezeichnung 1 |
| <p2> | Scheibenaufbau |
| <pd> | Produktionsdatum |
| <pn> | Produktnummer |
| <po> | Positionsnummer mit führenden Nullen, 3-stellig |
| <ps> | Positionsnummer, ohne führende Null oder Leerzeichen |
| <sn> | Schlüsselnummer |
| <vs> | VSG Bezeichnung |
| <vsg> | VSG Kurzbezeichnung |
| <wh> | Maße der Position |
| <kk> | Bestellübergabe: Kundenkommission |

**Beispiel**
Eingabe: `<c1> <p1> <p2> <wh> <no>`
Ausgabe: `John+Partner Standard ISO FL4/18/ORN528 540x1030 109384/001`

---

### Konstruktionstypen Bleiverglasung

Für die Verarbeitung von Bleiverglasungen sind folgende Konstruktionstypen standardmäßig hinterlegt:

| Typ 1 | Typ 2 |
| :--- | :--- |
| Gothic | Stuart |
| **Typ 3** | **Typ 4** |
| Diamonds | Cumberland |
| **Typ 5** | **Typ 6** |
| Hanover | Jacobean |
| **Typ 7** | **Typ 8** |
| Northumberland | Queen Anne |
| **Typ 9** | **Typ 10** |
| Queen Caroline | Rectangles |
| **Typ 11** | **Typ 12** |
| Square Gothic | Diamond Pillar |
| **Typ 13** | **Typ 14** |
| Westmorland | Windsor |

---

### Änderungsüberwachung

Änderungen in der Kunden-, Lieferanten-, Preis- und Rabattverwaltung können überwacht werden. Dazu steht in den entsprechenden Dialogen das Menü **Historie** zur Verfügung.

Für alle Datenbank-Tabellen, auf die ein Dialog zugreift, kann festgelegt werden, wie Änderungen überwacht werden sollen. Eine sehr detaillierte Überwachung wird möglich, wenn die betreffenden Tabellen auf der Ebene der Felder überwacht werden.

Die Änderungsüberwachung wird für jeden der genannten Dialoge getrennt eingestellt und aktiviert. In Allgemeinen werden in der Auswertung die Änderungen des aktuell ausgewählten Datensatzes angezeigt. Daneben kann die Auswertung aber auch nach Nummernverwaltern oder für alle Datensätze angezeigt werden.

Sowohl die Einstellungen als auch die Auswertungen beziehen sich immer auf den gerade eingestellten Laufzeit-Modus. Zum Beispiel betrifft das in der Preisverwaltung die Auswertung von Änderungen der Standardpreise, der Kundenpreise, der Kundengruppenpreise usw.

Daneben können die Auswertungen zusätzlich durch verschiedene Filter eingeschränkt werden, z. B. auf einen bestimmten Mitarbeiter oder einen Zeitraum.

#### Änderungsüberwachung Verwaltung

**Utilities > System > Änderungsüberwachung Verwaltung**

In diesem Dialog legen Sie fest, welche Änderungen überwacht und dokumentiert werden sollen.

Diese Funktion ist nur freigeschaltet, wenn Sie die entsprechenden Lizenzen erworben haben.

**Menü Initialisierung**
Über den Eintrag **Auswertung initialisieren** wird die Auswertung vorbereitet. Danach kann sie über das Menü **Historie > Auswertung** angezeigt oder gedruckt werden.

**Allgemeine Einstellungen**

*   **Sprache**: Sprache, in der die Auswertungen ausgegeben werden.
*   **Trigger erstellen**: Die Schaltfläche ist nur freigeschaltet, wenn:
    *   eine Änderungsüberwachung initialisiert wurde.
    *   die Einstellung für eine Tabelle oder ein Feld bearbeitet wurde.

> **Info:** Die Datenbank-Trigger für die Überwachung müssen neu gebildet werden, wenn die Einstellungen neu festgelegt oder geändert wurden. Dies kann manuell gestartet werden (empfohlen). Es erfolgt automatisch beim Beenden des Dialogs. Dieser Vorgang kann einige Zeit in Anspruch nehmen.

**Tabelleneinstellungen**

*   **Übergreifende Einstellungen**: Wenn Sie die Einstellungen zur Überwachung von Änderungen über den Programmbereich **Utilities > System > Änderungsüberwachung Verwaltung** festlegen, gelten sie für alle verfügbaren Tabellen. Sie können die Einstellungen aber auch für den aktuellen Dialog festlegen.
*   **Name**: Bezeichnung der Tabelle. Sie kann geändert werden. Die Bezeichnungen werden in der Auswertung angezeigt.
    Wenn die Überwachung aktiviert ist, werden alle Felder dieser Tabelle im Bereich **Feldbeschreibungen** angezeigt.
*   **Historie**: In den Komboboxen der Spalte **Historie** stehen folgende Einstellungen zur Wahl:
    *   **Keine**: Die Änderungen werden nicht überwacht. Mit dieser Einstellung kann keine Auswertung angezeigt werden.
    *   **Komplett**: Die Änderungen werden für die gesamte Datenbank-Tabelle überwacht. In der Preisverwaltung müssen Sie diese Einstellung für alle Preistabellen wählen, wenn Sie sich auch alte Stände anzeigen lassen möchten.
    *   **Detailliert**: Die Änderungen werden auch auf Feldebene überwacht.

**Feldeinstellungen**
Wenn die Tabelle auf Feldebene überwacht wird, kann eingestellt werden, welche Felder eine Überwachung auslösen.

*   **Name**: Bezeichnung des Feldes. Sie kann geändert werden. Die Bezeichnungen werden in der Auswertung angezeigt.
*   **Referenziert auf**: Zum Identifizieren von Änderungen werden die Schlüsselspalten der jeweiligen Tabelle herangezogen. Handelt es sich bei den Schlüsselfeldern um referenzierende Felder, so wird in dieser Spalte die referenzierte Tabelle angegeben.
*   **Anzeigespalte**: In einer Tabelle, auf die verwiesen wird, kann neben dem Schlüsselwert auch eine Bezeichnung angezeigt werden. Die möglichen Bezeichnungen können aus der Kombobox in dieser Spalte ausgewählt werden. Z. B. verweist das Feld **Preisschlüssel** auf die Datenbank-Tabelle **Preisschlüssel**. Aus dieser Tabelle kann die Preisschlüsselnummer oder die Bezeichnung angezeigt werden. Wenn neben dem Schlüsselwert keine Bezeichnungen zur Verfügung stehen, ist die Kombobox leer.
*   **An/aus**: Diese Spalte und die Checkboxen werden nur angezeigt, wenn in den Tabelleneinstellungen in der Spalte **Historie** der Wert **detailliert** ausgewählt ist. In der Auswertung werden nur die Felder angezeigt, die über diese Checkboxen aktiviert sind. Sie können höchstens 80 Felder anzeigen lassen.
*   **Auswahl**: Über die beiden Schaltflächen zur Auswahl können alle Checkboxen in der Spalte **an/aus** aktiviert oder deaktiviert werden. Die Checkboxen können danach einzeln aktiviert oder deaktiviert werden.

---

### A+W Production

Produktionsrelevante Daten können an **A+W Production** übergeben werden. A+W Production verwendet die gleichen Stammdaten wie A+W Business. Änderungen in den Stammdaten müssen an A+W Production übergeben werden. Über die Produktnummer ist sichergestellt, dass beide Programme das gleiche Produkt verwenden. In jedem Produkt wird in **A+W Business** ein Kennzeichen zur Bearbeitung gesetzt. Dieses erzeugt die sogenannten Produktionsstücklisten für die Übergabe.

#### Übergabedatei

Für die Übergabe wird eine ASCII-Datei in das Verzeichnis AWPOOL geschrieben. Für diese legen Sie fest, welche Parameter übergeben werden sollen.

**Beispiel**
*   Kundenspezifische Logo-Nummer
*   Relevante Textkennzeichen
*   Kantenschutz pro Auftrag (Aluband, nur ISO)
*   Abstandhalter (über den Fremdschlüssel aus der Produktdefinition)
*   Kennzeichen für das Gas

#### Stammdatentransfer von A+W Business an A+W Production

Wenn das Zusatz-Modul **Stammdatentransfer** installiert ist, können folgende Daten übertragen werden. Ohne das Modul müssen die Daten in beiden Programmen identisch angelegt werden.

**Tab. B-29 Übergabe der Stammdaten aus A+W Business an A+W Production**

| Dialog in A+W Business | Feld | Dialog in A+W Production | Feld |
| :--- | :--- | :--- | :--- |
| **Produktverwaltung** | | **Artikelstammdaten:** | |
| Register Produkt: | Bezeichnung (1 - 3)<br>bei Produktarten:<br>• HW<br>• TVG<br>• ESG<br>• ISO<br>• VSG<br>• GH<br>Sprossendicke | | Bezeichnung<br>Artikeltext (1 - 2)<br>Checkbox Freigabeteil aktiv<br><br><br><br><br><br><br>Dicke |
| Bei Bearbeitungen | Produktgruppe<br>Mengeneinheit | **Bearbeitungsartikel:** | Klasse<br>Dauer s/ |
| Kurzinfo und Produktinfo werden nicht übergeben | | | |
| Die Schleifgruppe wird aus A+W Production übernommen | | | |
| Register Fertigung: | Struktur - Verlauf | **Glasarten:** | Struktur |
| Register Lager/Einkauf: | Beschaffungsart<br>Automatischer Zuschnitt<br>Technische Artikelnummer | **Artikelstammdaten:**<br>**Glasartikel:** | Beschaffungsart<br>Optimierbar<br>Artikelcode |
| Register A+W Production: | Glasart<br>Schleifgruppe<br>Modell<br>Bruchränder (o, u, r, I)<br>Max. Traverenbreite<br>Min. Abst. X-Z Schnitte<br>Reihenf. Opti.<br>Strukturlage<br>Beschichtungslage | **Artikelstammdaten:**<br>**Glasartikel:** | Glasart<br>Schleifgruppe<br>Modellbruchrand<br>Bruchränder<br>Max. Traverenbreite<br>Mindestabstand X-Z<br>Opti-Rang<br>Strukturlage<br>Schichtlage |
| Die Übergangszeit wird nicht übergeben (Feld leer lassen) | | | |
| **Glasarten** | Bezeichnung<br>Produktgruppe<br>Glasartgruppe<br>Struktur<br>Beschichtung | **Glasarten:**<br>**Artikelstammdaten:** | Bezeichnung<br>Artikeltyp<br>Glasartgruppe<br>Struktur<br>Beschichtung |
| **Glasart-Jumbos** | Produktgruppe<br>Bezeichnung<br>Breite / Höhe Jumbo<br>Priorität für Opti.<br>Traverenflag:<br>• X-Richtung<br>• Y-Richtung<br>• wahlweise | **Artikelstammdaten:**<br>**Lagermaße:** | Artikeltyp<br>Bezeichnung<br>Breite / Höhe<br>Preis<br>Traveren |
| Jumbo-Zuschneidetische | Auflegercode<br>Anzahl | **Lagermaße:** | Auflegercode<br>Anzahl |
| **Zuschneidetische** | | | |
| Register Werte: | Bezeichnung<br>Breite / Höhe<br>Referenzpunkt<br>Z-Schnitt<br>Brechbeginn<br>Böcke per Zyklus<br>Spezial<br>Rang | **Tische:** | Beschreibung<br>Breite / Höhe<br>Referenz<br>Z-Schnitt<br>Brechbeginn<br>Böcke / Zyklus<br>Spezial<br>Rang |
| Register Einstellungen: | Autobrechen<br>Autoaufleger<br>Formen<br>VSG<br>Entschichten<br>Handzuschnitt<br>max. Traverenbreite darf | **Tische:** | Autobrechen<br>Autoaufleger<br>Formen<br>VSG<br>Entschichten<br>Handzuschnitt<br>maximale Traverenbreite |
| Register Schnitte: | Min. Abst. Y-Y Schnitte<br>Min. Abst. X-X Schnitte<br>Max. Abst. Y-Y Schnitte<br>Max. Abst. X-X Schnitte | **Tische:** | Min X-X<br>Max X-X<br>Min Y-Y |
| Die Werte zum maximalen Verschnitt werden nicht übergeben. | | | |

#### Bearbeitungskatalog

Der hinterlegte Bearbeitungskatalog enthält alle Bearbeitungstypen und die erforderlichen Parameter. Er dient als zentrales Bindeglied zwischen den bestehenden Programmen der A+W Software GmbH.

Damit können aus A+W Business die Bearbeitungen inklusive aller dazugehöriger Daten an A+W Production oder per OrderXML übergeben werden.

Um immer wiederkehrende komplizierte Kombinationen von Bearbeitungen schnell erfassen zu können, kann zusätzlich ein von Shaping & Nesting generiertes Bearbeitungsmakro angehängt werden.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Produktverwaltung - A+W Production" auf Seite B-630
⇨ Softwarereferenz, "Firmendaten - Produktion" auf Seite B-1000
⇨ Verkauf, "Parameter" auf Seite C-480

---

### Mischkalkulation

Für die Preisberechnung von kundenspezifischen Preisen kann statt eines Austauschzuschlages die sogenannte Mischkalkulation angewendet werden. Diese Art der Kalkulation wird in Österreich verwendet.

Dazu werden bis zu drei Produkte herangezogen, bei deren Kombination ein gemischter Preis kalkuliert werden soll. Für die Kalkulation wird angegeben, auf welche (kundenspezifische) Preistabelle dabei zurückgegriffen werden soll.

Die Berechnungsfaktoren für die Mischkalkulation werden in den Firmendaten hinterlegt. Außerdem wird dort festgelegt, ob eine Rabatt- und/oder Individualpreissuche bei der ISO-Mischkalkulation möglich sein soll.

Standardmäßig ist die Suche nach Individualpreisen und nach Rabatten bei der Mischkalkulation ausgeschaltet.

**Beispiel**
*   **Basispreis 2-fach Isolierglas =**
    50 % ISO-Preistabelle 1 + 50 % ISO-Preistabelle 2.
*   **Basispreis 3-fach Isolierglas =**
    50 % ISO-Preistab. 1 + 80 % ISO-Preistab. 2 + 50 % ISO-Preistab. 3.

Für die erste Scheibe der ISO-Einheit wird der Preis für aus der ISO-Preistabelle 1 und für die zweite Scheibe der ISO-Einheit der Preis aus der ISO-Preistabelle 2 genommen. Bei einem 3-fach Isolierglas wird für die dritte Scheibe der ISO-Einheit der Preis aus der ISO-Preistabelle 3 genommen.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Mischkalkulation" auf Seite B-707
⇨ Softwarereferenz, "Mischkalkulationsfaktoren" auf Seite B-943
⇨ Softwarereferenz, "Rabattsuche bei ISO-Mischkalkulation" auf Seite B-961
⇨ Softwarereferenz, "Individualpreissuche bei ISO-Mischkalkulation" auf Seite B-962

---

### Französische Preisberechnung

Bei der sog. französischen Preisberechnung von ISO setzt sich der Preis für das ISO aus folgenden Komponenten zusammen:
*   Basispreis für den Zusammenbau des ISO
*   Einzelpreise für die Gläser

Dafür werden in der Regel eigene Schlüssel und Tarife definiert. Die Preise für die jeweiligen Einzelgläser werden in der gewohnten Form definiert. Sie müssen im selben Preisschlüssel liegt wie der ISO-Basispreis. Für das ISO muss die Preiseinheit `<qm+EP>` gewählt werden.

Die Produkte werden in der üblichen Form angelegt. Für die Abstandhalter wird ein Sonstiger Zuschlag angelegt und dem ISO-Preis zugeordnet.

> **ISO und VSG**
> Bei der frz. Preisberechnung darf in den Firmendaten die Option **Iso und VSG-Einzelpreisberechnung** nicht aktiviert werden.
> ⇨ Softwarereferenz, "ISO + VSG Einzelpreisberechnung" auf Seite B-962

---

### Kalkulation

**Lernziele**
*   Komponenten der Kostenkalkulation.
*   Vorgaben für die Eigenkosten-Kalkulation festlegen.
*   Kalkulation des Deckungsbeitrags festlegen.

**Nutzen**
*   Die Höhe der Eigenkosten wird übergreifend eingestellt und in die Kalkulationen des Deckungsbeitrags und der Einkaufspreise einbezogen.
*   Der Deckungsbeitrag wird automatisch neu berechnet, wenn im Dokument die Preise bei der Erfassung von Positionen geändert werden.

**Merke**
| Begriff | Beschreibung |
| :--- | :--- |
| **Herstellkosten** | Die Herstellkosten setzen sich zusammen aus: Material-, Maschinen- und Personalkosten zuzüglich Gemeinkosten. |
| **Gemeinkosten** | Die prozentualen Anteile für die Gemeinkosten legen Sie in den Firmendaten fest. |
| **Kalkulation** | Die Kostenkalkulation wird pro Tarif (Preisjahrgang und -schlüssel) aktiviert: <ul><li>Wenn die Kalkulation in den Tarifen nur für die EK-Preisberechnung aktiviert ist, wird die Kosten- und Aufschlagskalkulation nur bis zum Selbstkostenpreis durchgeführt.</li><li>Wenn auch in den VK-Tarifen die Kalkulation aktiviert ist, geht die Kalkulation weiter bis zum Verkaufspreis.</li></ul> |
| **Teilmaterialkosten** | Die Teilmaterialkosten errechnen sich aus der Menge (inkl. produktbezogenem Verschnitt) und dem Preis pro Mengeneinheit. |
| **Vollmaterialkosten** | Auf die Teilmaterialkosten wird ein Gemeinkostenzuschlag berechnet, der die Beschaffungsart des Produkts berücksichtigt. |
| **Deckungsbeitrag** | Für die Ermittlung des Deckungsbeitrags werden Mindest- und Höchstwerte pro Kunde und Warengruppe gepflegt.<br>Die aktuellen Deckungsbeiträge werden pro Dokument ermittelt und angezeigt. Die Deckungsbeitrags-Analyse ermittelt die Deckungsbeiträge über einen beliebigen Zeitraum. |

---

### Deckungsbeitrags-Grenzwerte

Deckungsbeiträge werden im Auftrag direkt angezeigt und beziehen sich nur auf die im Auftrag enthaltenen Positionen.

Mit Hilfe der Deckungsbeitrags-Analyse kann der Deckungsbeitrag von Auftragspositionen über einen beliebigen Zeitraum untersucht und gedruckt werden. Diese Auswertung wird im Modul **Dokumente** gestartet.

Die minimalen und maximalen Deckungsbeiträge werden im Dialog **Deckungsbeitrags-Grenzen** pro Kunde und Warengruppe gepflegt.

Die Grenzwerte legen Sie pro Kunde oder Kundengruppe (A) fest. Die Analyse bezieht sich jeweils auf eine Warengruppe (B), wobei Sie alle drei Ebenen (WGR, WOG, WHG) wählen können.

Für jede Kombination von (A) und (B) können Sie prozentualen Werte (C) für die Deckungsobergrenze und die Deckungsuntergrenze festlegen. Damit können Sie z. B. leichter prüfen, ob der Deckungsbeitrag für den Kunden oder die Kundengruppe im gewünschten Rahmen liegt.

Da jede Kalkulation von Preisen im einzelnen Auftrag überschrieben werden kann, können ein Höchst- und ein Mindestbetrag für Deckungsbeiträge hinterlegt werden. Damit werden grobe Fehlkalkulationen bei der manuellen Preisgestaltung im Auftrag verhindert, z. B. ein Verkaufspreis unter den Selbstkosten.

Für alle nicht explizit definierten Kombinationen von Kunden und WGR gelten die Standardwerte, die in den Firmendaten im Register **Kalkulation** festgelegt sind.
*   **A Mindestbeitrag für Deckungsbeiträge**
*   **B Höchstbeitrag für Deckungsbeiträge**

---

### Kosten- und Aufschlagskalkulation

Mit der Kosten-/Aufschlagkalkulation wird der Preis pro Preiseinheit ermittelt. Dazu werden die Anteile der Selbstkosten aus den Firmendaten berücksichtigt.

#### Herstellungskosten

Auf der Basis von Material-, Maschinen- und Personalkosten werden Herstellkosten ermittelt. Zuzüglich der Gemeinkostenzuschläge für Material und Sondereinzelkosten ergeben sich daraus die Vollherstellkosten.

Zu den Materialgemeinkosten zählen die Beschaffungsarten:
*   Bestellung
*   Lagerentnahme
*   Produktion

Auf diese werden Gemeinkosten für Verwaltung und Vertrieb aufgeschlagen. Zuzüglich einer prozentualen Gewinnerwartung ergibt sich daraus der Verkaufspreis.

Zu den Gemeinkosten zählen:
*   **Lohnnebenkosten**: z. B. Kosten für Sozialversicherungen.
*   **Vertriebsgemeinkosten**: Kosten, die den Produkten nicht im Einzelnen zugeordnet werden können, z. B. Provisionen.
*   **Verwaltungsgemeinkosten**: z. B. Kosten für Büro, Energie, Verwaltungsmitarbeiter usw.
*   **Gewinnspanne**

Die prozentualen Anteile für die Gemeinkosten legen Sie in den Firmendaten fest.

Diese prozentualen Aufschläge (A, B) beziehen sich auf die Einkaufspreise (netto).
Die Kostenkalkulation wird pro Tarif (Preisjahrgang und -schlüssel) aktiviert.

Wenn die Kalkulation in den Tarifen nur für die EK-Preisberechnung aktiviert ist, wird die Kosten- und Aufschlagskalkulation nur bis zum Selbstkostenpreis durchgeführt. Wenn auch in den VK-Tarifen die Kalkulation aktiviert ist, geht die Kalkulation weiter bis zum Verkaufspreis.

Im Dokument und in den Positionen können Sie sich die Kalkulationen für den aktuellen Auftrag anzeigen lassen.

In den Beispielen sehen Sie die Kalkulation für eine Position (A). In der Positionserfassung kann die Kalkulation für die Stückliste (B) geprüft werden. Preise, die implizit in einem Produkt enthalten sind, werden dabei nicht angezeigt.

Die Kalkulation kann pro Position angepasst werden, z. B. um bestimmte Nebenkosten mit einem abweichenden Prozentsatz zu kalkulieren oder um Sonderkosten zu berücksichtigen.

Die Kostenkalkulation kann pro Position auch um Sonderzuschläge erweitert werden. Wenn diese Zuschläge als negativer Wert angegeben werden, entspricht das einem Sonderrabatt für diese eine Position.

> **Info: Maschinen- und Personalkosten aus der Produktion**
> Die Anteile aus Maschinen- und Personalkosten werden über die zugehörigen Basisdaten aus der Kapazitätsplanung errechnet. Diese Kostenfaktoren stehen daher nur zur Verfügung, wenn die A+W Business-Kapazitätsplanung freigeschaltet ist und wenn Rückmeldungen zu den tatsächlichen Kosten aus der Produktion vorliegen.

---

### Kalkulation der Eigenkosten festlegen

Für die Kalkulation der Eigenkosten für Isolierglas legen Sie pro Abstandhalter den durchschnittlichen Verbrauch von Hilfsstoffen wie Butyl, Thiokol usw. fest. Ein ausführliches Beispiel finden Sie in einer separaten Einheit.

⇨ "Komplexbeispiel: Kalkulation ISO" auf Seite B-555

> **Voraussetzung**
> Die Verbrauchsartikel, die im Bereich **Stücklistenprodukt** eingetragen werden sollen, müssen als Produkte angelegt sein.

**So legen Sie Vorgaben für die Kalkulation der Eigenkosten fest**

1.  Wählen Sie im Menü **Stammdaten > Produkte > Artikel > EK-Kalkulation**. Der Dialog Kalkulationsvorgaben wird geöffnet.
    ⇨ Softwarereferenz, "EK-Kalkulation" auf Seite B-656
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
3.  Geben Sie die Artikelnummer des Abstandhalters (A) ein, dem der Verbrauch an Gas, Trockenmittel oder Randverbund zugeordnet werden soll.
4.  Tragen Sie die gewünschten Werte in die Felder ein:
    *   **Rückschnitt (einfach)** in mm (B)
    *   **Entspannte Menge für Gas** in Liter (C)
5.  Wechseln Sie zum Register **Stückliste**.
6.  Markieren Sie im Bereich **Stückliste** eine Zeile mit der Artikelnummer 0.
7.  Tragen Sie im Bereich **Stücklistenprodukt** (D) die Produktnummer, den Verbrauch des Artikels und dessen Bezugseinheit ein. Die Einträge werden im Bereich **Stückliste** angezeigt.
8.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Daten werden gespeichert.

> **Info: Rückschnitt**
> Mit dem **Rückschnitt (einfach)** ist der Abstand von der Glasaußenkante bis zum Alurahmen außen gemeint. Er ist wichtig für den Bieger der Alurahmen.
> Beträgt das Glasmaß z. B. 1000 x 1000 mm, der **Rückschnitt (einfach)** 5 mm, so beträgt das Rahmenmaß 990 x 990 mm.

---

### Komplexbeispiel: Kalkulation ISO

In diesem Beispiel wird gezeigt, wie die Eigenkalkulation (EK) einer Isolierglas-Einheit bei Eigenfertigung eingerichtet und im Auftrag angezeigt wird.

Die Kalkulation wird in folgenden Einheiten dargestellt:
*   Berechnung der Scheiben
*   Berechnung des Rahmens
*   Berechnung für das Gas
*   Berechnung der Verbrauchsmaterialien

Bei der Beispielberechnung wurde auf Rundungen, Rabatte und Zuschläge verzichtet, damit die Kalkulation einfach nachzuvollziehen ist.

#### Anzeige in der Positionserfassung

Die EK-Preise einer Auftragsposition können über das Menü **Ansicht** angezeigt werden. Die im Beispiel angezeigten Werte sind in der folgenden Berechnung enthalten:

**Tab. B-30 Berechnung des Einkaufspreises**

| Legende | Produkt | Preis |
| :--- | :--- | :--- |
| 1 | 1. Scheibe | + 8,57 |
| 2 | + 2. Scheibe | + 10,91 |
| 3 | + Verbrauchsmaterialien | + 3,68 |
| 4 | + Rahmen | + 1,60 |
| 5 | + Gas | + 0,12 |
| **6** | **Stückkosten** | **= 24,88** |

Die Kalkulation der Nummern 1 - 5 wird im Folgenden detailliert dargestellt.

#### Berechnung der Scheiben

Bei der Berechnung der Scheiben werden der Einkaufpreis aus der zugeordneten Preistabelle, der Verschnitt und die Rundung berücksichtigt. Im gezeigten Beispiel ist keine Rundung der Fläche definiert.

**Erste Scheibe**
Der EK-Preis aus der Preistabelle wird mit der Fläche multipliziert. In diesem Beispiel ist die Höhe x Breite = 1 qm. Zum errechneten Wert wird ein Betrag für den Verschnitt addiert.

**Tab. B-31 EK-Berechnung der ersten Scheibe**
| EK | x | (Fläche + Verschnitt) | EK |
| :--- | :--- | :--- | :--- |
| 8,24 | x | (1 + 4/100) | 8,57 |

**Verschnitt**
In den Produktstammdaten werden im Register **Preis/Zuschlag** die Preistabellen für den VK und den EK zugeordnet und der mittlere Verschnitt definiert.

**Preis**
In der Preistabelle wird der Einkaufspreis hinterlegt, den Sie mit Ihrem Lieferanten vereinbart haben.

**Zweite Scheibe**
Die Berechnung der zweiten Scheibe basiert ebenfalls auf den Stammdaten. Die Werte können sich von der ersten Scheibe unterscheiden.

**Tab. B-32 Berechnung der zweiten Scheibe**
| EK | x | (Fläche + Verschnitt) | EK |
| :--- | :--- | :--- | :--- |
| 10,20 | x | (1 + 7/100) | 10,91 |

Verschnitt und Preis werden so wie bei der ersten Scheibe in den Stammdaten festgelegt.

#### Berechnung des Rahmens

In diesem Beispiel beträgt die Kantenlänge genau 1000 mm. Die Gesamtlänge des Rahmens beträgt also 4 m.

**Tab. B-33 Berechnung des Rahmens**
| EK Rahmen | x | effektive Lfm | EK |
| :--- | :--- | :--- | :--- |
| 0,40 | x | 4 | 1,60 * |
*Nr. 4 der Tabelle "Berechnung des Einkaufspreises" auf Seite B-555*

Der Preis wird ebenfalls als Einzelpreis in den Stammdaten festgelegt. In der Preistabelle wird der Einkaufspreis pro Preiseinheit hinterlegt, den Sie mit Ihrem Lieferanten vereinbart haben. In diesem Beispiel ist das 0,40/lfm.

#### Berechnung für das Gas

Zur Berechnung des Gases wird die hinterlegte Gasmenge mit der Dicke des Scheibenzwischenraums multipliziert.

**Tab. B-34 Berechnung des Gases**
| m³ | x | SZR/Entspannte Menge Gas | x | EK Gas (1 + Verschnitt/100) | EK |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | x | 12/21000 | x | 215,90/(1 + 0/100)* | 0,12** |
*\* In diesem Beispiel wird ohne Verschnitt für das Gas gerechnet.*
*\*\* Nr. 5 der Tabelle "Berechnung des Einkaufspreises” auf Seite B-555*

**Kalkulationsgrundlage**
Unter **Stammdaten > Produkte > Artikel > EK Kalkulation** wird die entspannte Menge des Gases (ohne Druck, ohne Kühlung) pro Kubikmeter angegeben.

Der Preis wird ebenfalls als Einzelpreis in den Stammdaten festgelegt. In der Preistabelle wird der Einkaufspreis pro Preiseinheit hinterlegt, den Sie mit Ihrem Lieferanten vereinbart haben.

#### Berechnung der Verbrauchsmaterialien

Zusätzlich zu Scheiben, Rahmen und Gasfüllung können Verbrauchsmaterialien angegeben werden, die bei der Produktion der ISO-Einheit benötigt werden.

**Tab. B-35 Berechnung der Verbrauchsmaterialien**
| | EK |
| :--- | :--- |
| EK Butyl | 2,2 |
| + EK Thiokol | 0,028696 |
| + EK Trockenmittel | 1,4484 |
| | **3,68*** |
*\* Nr. 3 der Tabelle "Berechnung des Einkaufspreises" auf Seite B-555*

In den folgenden Abschnitten ist dargestellt, wie die drei Einzelbeträge errechnet wurden.

**Berechnung für das Butyl**

**Tab. B-36 Berechnung des Butyls**
| EK Butyl | x | tatsächliche Laufmeter | x | Verbrauch pro Einheit | EK |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 100 | x | 4 | x | 0,0055 | 2,20 |

Zur Berechnung des Verbrauchs ist die Menge pro Einheit festgelegt. In diesem Beispiel werden 0,0055 kg pro laufendem Meter (Rahmen) berechnet. Der Preis wird ebenfalls als Einzelpreis in den Stammdaten festgelegt. In der Preistabelle wird der Einkaufspreis pro Preiseinheit hinterlegt, den Sie mit Ihrem Lieferanten vereinbart haben.

**Berechnung für das Thiokol**

**Tab. B-37 Berechnung des Thiokols**
| EK Thiokol | x | effektive Lfm | x | Verbrauch pro Einheit | EK |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1,17 | x | 4 | x | 0,0422 | 0,028696 |

Zur Berechnung des Verbrauchs ist die Menge pro Einheit festgelegt. In diesem Beispiel werden 0,0422 Liter pro laufendem Meter (Rahmen) berechnet. In der Preistabelle wird der Einkaufspreis pro Preiseinheit als Einzelpreis hinterlegt.

**Berechnung der Trockenmittel**

**Tab. B-38 Berechnung des Trockenmittels**
| EK Trockenmittel | x | effektive lfm | x | Verbrauch pro Einheit | EK |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 8,50 | x | 4 | x | 0,0426 | 1,4484 |

Zur Berechnung des Verbrauchs ist die Menge pro Einheit festgelegt. In diesem Beispiel werden 0,0426 kg pro laufendem Meter (Rahmen) berechnet. In der Preistabelle wird der Einkaufspreis pro Preiseinheit als Einzelpreis hinterlegt.

**Ergänzende Informationen**
⇨ Tutorial 2, "Kalkulation der Eigenkosten festlegen" auf Seite B-553
⇨ Softwarereferenz, "Einkauf" auf Seite B-970
⇨ Softwarereferenz, "Firmendaten - Kalkulation" auf Seite B-994

---
---

## Softwarereferenz: A+W Business

### Übersicht

Im Modul **Stammdaten** werden alle Daten zu A+W Business eingerichtet und gepflegt, die übergreifend von allen Modulen genutzt werden.

Die Stammdaten sind in folgende Menüs gegliedert:
*   "Allgemein" auf Seite B-564
*   "Produkte" auf Seite B-572
*   "Preise" auf Seite B-670
*   "Lager" auf Seite B-746
*   "Marktpartner" auf Seite B-754
*   "Versand" auf Seite B-872
*   "Fertigung" auf Seite B-881
*   "Auftrag" auf Seite B-893
*   "Finanzen" auf Seite B-916
*   "Firma" auf Seite B-929
*   "Texte" auf Seite B-1058
*   "Formulare" auf Seite B-1064
*   "CEKAL" auf Seite B-1091
*   "CE-Kennzeichen" auf Seite B-1101
*   "B2B" auf Seite B-1105

> **Info: Schaltflächen in den Dialogen**
> Die Standard-Schaltflächen und -menüs sind ausführlich im Part **Übersicht** und in den **Tutorials** beschrieben. Auf sie wird daher in der Beschreibung der Dialoge nicht eingegangen.

---

### Allgemein

**Stammdaten > Allgemein**

In diesem Programmbereich sind allgemeine Daten hinterlegt.
Im Menü **Allgemein** finden Sie folgende Einträge:
*   "Sprachen" auf Seite B-564
*   "Monate" auf Seite B-566
*   "Tage" auf Seite B-566
*   "Landeskürzel" auf Seite B-567
*   "Kalender" auf Seite B-568
*   "Basisnummernkreise" auf Seite B-570

#### Sprachen

**Stammdaten > Allgemein > Sprachen**

In diesem Dialog tragen Sie alle Sprachen ein, in denen Sie mit Ihren Kunden in schriftlicher Form korrespondieren. An erster Stelle steht immer Ihre Korrespondenzsprache. Sie können diese nicht nachträglich ändern.
Dieser Dialog steht nur mit dem Modul Mehrsprachigkeit zur Verfügung.

*   **Bezeichnung**: Name der Sprache.
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Produktion oder die Finanzbuchhaltung.

**Menü Funktionen**
Über dieses Menü können Sie den Dialog **Anlage Preis-/Mengeneinheit für Mehrsprachigkeit** öffnen, um die Bezeichnungen für Preis- und Mengeneinheiten in eine neu angelegte Sprache zu kopieren.
⇨ "Preis-/Mengeneinheit für Mehrsprachigkeit" auf Seite B-565

#### Preis-/Mengeneinheit für Mehrsprachigkeit

**Stammdaten > Allgemein > Sprachen > Menü Funktionen > Einheiten kopieren**

In diesem Dialog kopieren Sie die Bezeichnungen für Preis- und Mengeneinheiten in eine neu angelegte Sprache, wenn Sie das Modul Mehrsprachigkeit einsetzen. Anschließend müssen Sie diese Bezeichnungen in die neue Sprache übersetzen.

*   **Quellsprache**: Standardmäßig wird die Basissprache vorgeschlagen. Sie können jede andere Sprache auswählen, in der die Preis- und Mengeneinheiten vorhanden sind.
*   **Zielsprache**: Zielsprache, in die die Preis- und Mengeneinheiten kopiert werden sollen.

Im Dialog **Preis/Menge** müssen anschließend Sie die Bezeichnungen in dem entsprechenden Sprachregister übersetzen.
⇨ "Preis- und Mengeneinheit" auf Seite B-711

#### Monate

**Stammdaten > Allgemein > Monate**

Die Monatsnamen sind standardmäßig mit der Basissprache vorbelegt und sollten nicht geändert werden.

*   **Bezeichnung**: Name des Monats.
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für statistische Auswertungen.

#### Tage

**Stammdaten > Allgemein > Tage**

Die Tagesnamen sind standardmäßig mit der Basissprache vorbelegt und sollten nicht geändert werden.

*   **Bezeichnung**: Name des Wochentags.
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für statistische Auswertungen.

#### Landeskürzel

**Stammdaten > Allgemein > Landeskürzel**

In diesem Dialog verwalten Sie die internationalen Landeskürzel und ordnen die Standardrundung für die Steuer zu.

*   **Landeskürzel**: Landeskürzel, z. B. D = Deutschland, F = Frankreich, USA = United States of America. Das Kürzel weisen Sie im Dialog **Partnerverwaltung** Ihren Kunden und Lieferanten zu, damit die Texte in der Sprache des Partners angezeigt und gedruckt werden, z. B. die Mengeneinheiten.
    ⇨ “(Land, Provinz)" auf Seite B-772
*   **Bezeichnung**: Name des Landes, z. B. Deutschland, Frankreich.
*   **Rundung Mwst**: Sie können für jedes Land festlegen, auf welchen Wert die Mehrwertsteuer gerundet werden soll. Zum Beispiel bedeutet 1, dass auf den nächsten Wert auf- oder abgerundet wird, bei 5 wird auf die nächste 5 auf- oder abgerundet.
    *   Tutorial 2, "Rundungen" auf Seite B-449
    *   "Rundung (Kunde, Lieferant)" auf Seite B-851
    *   "Rundung" auf Seite B-893
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für statistische Auswertungen.
*   **Gesperrt**: Ein Landeskürzel kann für die Erfassung in der Partnerverwaltung und in den Dokumenten gesperrt werden, wenn es nicht mehr benötigt wird.
    *   ☐ Das Landeskürzel kann zugewiesen werden.
    *   ☑ Das Landeskürzel ist gesperrt und kann nicht mehr zugewiesen werden. Wenn es Partnern und in Dokumenten zugewiesen ist, wird es jedoch weiterhin angezeigt.
*   **Internationales Kennzeichen**: Zweistelliges internationales Landeskürzel, z. B. DE = Deutschland, FR = Frankreich, US = United States of America.

#### Kalender

**Stammdaten > Allgemein > Kalender**

In diesem Dialog pflegen Sie die Feiertage und die täglichen Arbeitsstunden in Ihrem Unternehmen. Wenn im Feld **Stunden** ein Wert größer 0 steht, gilt dieser als Arbeitstag. Wenn Sie einen Tag als Feiertag definieren möchten, müssen Sie den Wert 0 eintragen.
⇨ Tutorial 1, "Allgemeinen Kalender anlegen" auf Seite B-103

**Arbeitswoche**
*   **Wochentag**: Anzahl der regulären Arbeitsstunden für jeden Wochentag. Die Feiertage müssen Sie auf 0 (Stunden) setzen.
    *   ☐ Der Wochentag wird nicht in die Arbeitswoche aufgenommen.
    *   ☑ Der Wochentag wird in die Arbeitswoche aufgenommen.

**Auswahl**
*   **Jahr, KW**: Auswahl des Jahres und der Kalenderwoche, um die entsprechende Kalenderwoche in der Übersicht anzuzeigen.
*   **[Auf Jahr übertragen]**: Überträgt die Änderungen auf alle entsprechenden Wochentage des gesamten Kalenderjahrs. Die Freitage müssen Sie danach auf 0 setzen.
*   **[Auf KW übertragen]**: Überträgt die Änderungen auf alle Tage der aktuellen Kalenderwoche. Die entsprechenden Wochentage des restlichen Kalenderjahrs bleiben unverändert.
*   **[Zur aktuellen KW]**: Mit dieser Schaltfläche lassen Sie sich die aktuelle Kalenderwoche anzeigen.

**Übersicht**
In der Übersicht werden alle Kalenderwochen des aktuellen Kalenderjahrs mit den Tagesarbeitszeiten angezeigt. Die Wochenenden sind in roter Schrift dargestellt.

#### Länder Kalender

**Stammdaten > Allgemein > Länder Kalender**

In diesem Dialog pflegen Sie die Feiertage in den Ländern und Provinzen, in denen die Unternehmen angesiedelt sind, mit denen Sie arbeiten.

**Identifikation**
*   **Provinz**: Auswahl der Provinz, für die der Feiertagskalender gilt. Die Provinzen sind unter **Marktpartner > Allgemein** hinterlegt.
    ⇨ "Provinz" auf Seite B-763
*   **Jahr**: Auswahl des Jahres, in dem die Feiertage gelten.
*   **Land**: Auswahl des Landes, zu dem die Provinz gehört. Die Länder sind unter **Stammdaten > Allgemein** hinterlegt.
    ⇨ "Landeskürzel" auf Seite B-567

**Tabelle**
In der Tabelle werden alle Kalender zu den Provinzen angezeigt, für die besondere Feiertage gelten.

**Übersicht**
In der Übersicht werden alle Kalenderwochen des aktuellen Kalenderjahrs mit den Tagesarbeitszeiten angezeigt. Die Wochenenden sind in roter Schrift dargestellt.

#### Basisnummernkreise

**Stammdaten > Allgemein > Basisnummernkreise**

In diesem Dialog wird angezeigt, wie viele Datensätze Sie in der jeweiligen Stammdatentabelle anlegen können und wie viele Nummern bereits vergeben sind. Die Start- und Endnummern sind in der Regel fest vorgegeben und müssen nicht angepasst werden.

Diese Nummern können pro Datenbank (DB) gepflegt werden. D. h., dass sich die Nummernkreise der Master-DB und der Slave-DBs unterscheiden können. Diese Einstellungen werden nicht repliziert.

In den aufgeführten Stammdatendialogen ist die Anzahl der möglichen Datensätze auf die höchste Nummer begrenzt. Wenn weitere Datensätze angelegt werden sollen, müssen Sie die höchste Nummer erhöhen.

> **Info: Nummernkreise für Dokumente**
> Nummernkreise für die Dokumente legen Sie im Programmbereich **Auftrag** fest.
> ⇨ "Nummernkreise" auf Seite B-903

**Übersicht**
*   **Tabelle**: Namen der Stammdatentabellen, zu denen Nummernkreise geführt werden.
*   **Letzte Nummer**: Nummer des Datensatzes, die in diesem Nummernkreis zuletzt vergeben wurde.
*   **Höchste Nummer**: Höchste Nummer, die in diesem Nummernkreis vergeben werden kann.

---

### Produkte

**Stammdaten > Produkte**

In diesem Programmbereich definieren Sie die allgemeinen Daten für die Verwaltung von Produkten und die Produktstammdaten.
Im Menü **Produkte** finden Sie folgende Einträge:
*   "Allgemein" auf Seite B-572
*   "Artikel" auf Seite B-646

#### Allgemein

**Stammdaten > Produkte > Allgemein**

In diesem Programmbereich sind die allgemeinen Daten zu den Produkten hinterlegt.
Im Menü **Allgemein** finden Sie folgende Einträge:
*   "Produktarten" auf Seite B-573
*   "Produktgruppen" auf Seite B-574
*   "WGR" auf Seite B-575
*   "Kombi-WGR" auf Seite B-577
*   "Top-WGR" auf Seite B-579
*   "Varianten" auf Seite B-580
*   "Sprossentypen” auf Seite B-581
*   "Reklamationsverursacher" auf Seite B-583
*   "Reklamationsgrund" auf Seite B-584
*   "Struktur" auf Seite B-585
*   "Strukturseite" auf Seite B-586
*   "Beschichtungsseite" auf Seite B-587
*   "Beschichtungsart" auf Seite B-588
*   "Glasartgruppen" auf Seite B-589
*   "Gütetext" auf Seite B-590
*   "Leistungserklärung Verwaltung" auf Seite B-592
*   "Austauschgruppen" auf Seite B-593
*   "Austauschzuordnung" auf Seite B-594
*   "Klassifikatoren - Produkt" auf Seite B-595

#### Produktarten

**Stammdaten > Produkte > Allgemein > Produktarten**

In diesem Dialog werden die Produktarten angezeigt, die in A+W Business zur Verfügung stehen. Sie können diese nicht umbenennen oder ergänzen.
⇨ Tutorial 1, “Produktarten und Produktgruppen" auf Seite B-142

*   **Bezeichnung**: Name der Produktart.
*   **Schlüssel**: Schlüsselnummer (ID), mit der die Produktart im System eindeutig identifiziert wird.
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Produktion.
*   **Gesperrt**: Eine Produktart kann für die Erfassung in der Produktverwaltung und in den Dokumenten gesperrt werden, wenn sie nicht mehr benötigt wird.
    *   ☐ Die Produktart kann zugewiesen werden.
    *   ☑ Die Produktart ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie Produkten und in Dokumenten zugewiesen ist, wird sie jedoch weiterhin angezeigt.

> **Info: Produktarten erweitern**
> Wenn Sie weitere Produktarten benötigen, sprechen Sie Ihren Service-Mitarbeiter bei der A+W Software GmbH an.

#### Produktgruppen

**Stammdaten > Produkte > Allgemein > Produktgruppen**

In diesem Dialog pflegen Sie die Produktgruppen, mit denen Sie in A+W Business arbeiten. Den Namen einer neuen Produktgruppe können Sie frei wählen. Anschließend ordnen Sie die Produktart zu.
⇨ Tutorial 1, "Produktarten und Produktgruppen" auf Seite B-142

*   **Produktart**: Produktart, die einer Produktgruppe zugeordnet ist.
*   **Bezeichnung**: Name der Produktgruppe.
*   **Schlüssel**: Schlüsselnummer, über die die Produktgruppe in System eindeutig identifiziert wird.
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Produktion.
*   **Schlüssel A+W Production**: Fremdschlüssel, der für den Datenaustausch mit A+W Production genutzt wird. Dieser Schlüssel muss auch in A+W Production bei der entsprechenden Produktgruppe hinterlegt sein.
*   **Gesperrt**: Eine Produktgruppe kann für die Erfassung in der Produktverwaltung und in den Dokumenten gesperrt werden, wenn sie nicht mehr benötigt wird.
    *   ☐ Die Produktgruppe kann zugewiesen werden.
    *   ☑ Die Produktgruppe ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie Produkten und in Dokumenten zugewiesen ist, wird sie jedoch weiterhin angezeigt.

#### WGR

**Stammdaten > Produkte > Allgemein > WGR**

In diesem Dialog verwalten Sie die Warengruppen, mit denen Sie in A+W Business arbeiten. Die Warengruppen werden in drei Ebenen klassifiziert:
*   Warenhauptgruppe (WHG)
*   Warenobergruppe (WOG)
*   Warengruppe (WGR)

Die Abkürzung wird WGR auch für Warengruppen im Allgemeinen verwendet. Die WHG 0**, WOG 00* und WGR 000 sind fest angelegt.
Der Warengruppe 000 werden in der Regel nur Modelle zugeordnet. So kann in der Statistik z. B. der Modellumsatz automatisch dem Umsatz des Hauptproduktes zugeordnet werden.
Sprossen und Bearbeitungen haben in der Regel eine eigene Warengruppe.
⇨ Tutorial 1, "Warengruppen" auf Seite B-144

> **Info: Kombi-Warengruppen**
> Wenn Sie mit Kombi-Warengruppen arbeiten möchten, müssen Sie diese wie jede andere WGR anlegen. Im Dialog Kombi-WGR können Sie dann die gewünschten Warengruppen kombinieren und zuordnen.
> ⇨ "Kombi-WGR" auf Seite B-577

*   **Warengruppe**
    *   **Nummer**: Nummer der WGR. Sie können je nach Ebene bis zu 3 Stellen alphanumerisch angeben, z. B. 1AT.
    *   **Vorlauftage**: Vorlauftage für die Berechnung des Versandtags. Dies gilt nur für Bestellartikel. Der Wert gibt an, wie viele Tage ein Bestellartikel im Voraus beim Lieferanten bestellt werden muss, damit der Artikel rechtzeitig zur Produktion bereitsteht.
    *   **Bezeichnung**: Eindeutiger Name der WGR.
    *   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Produktion oder die Finanzbuchhaltung. Mit Hilfe eines Fremdschlüssels können Preise nach Warengruppen berechnet werden. Im Dialog zur Preisdefinition können Sie ihn für den Grenztyp WGR Fremdkey einsetzen.
        ⇨ "Preise" auf Seite B-725
        > **Info: Exakte Grenzmenge für WGR-Fremdkey**
        > Um eine exakte Grenzmenge für den WGR-Fremdkey zu haben, steht die Grenzmenge 140 WGR Fremdkey exakt zur Verfügung. Die entsprechende Funktion kann in den Firmendaten aktiviert werden.
        > ⇨ "WGR-Fremdkey als nicht exakte Grenzmenge berechnen" auf Seite B-968

*   **Kosten und Aufschlagskalkulation**
    *   **Sonderzuschlag**: Prozentualer Zuschlag für eine Warengruppe. Dieser Sonderzuschlag wird bei der Berechnung der Selbstkosten berücksichtigt und entsprechend ausgewiesen.
    *   **Steuercode**: Zur Steuerberechnung können die Daten an den Avalara Web-Service übergeben werden. Für die korrekte Steuerberechnung müssen sogenannte Steuercodes zu jeder Warengruppe eingetragen werden. Während der Übergabe wird für jede Position der Steuercode anhand der Kombi-Warengruppe des Hauptproduktes ermittelt und an Avalara übergeben. Die Zugangsdaten müssen in den Firmendaten eingerichtet werden.
        ⇨ "Firmendaten - Steuer" auf Seite B-933
    *   **Bitmap**: Piktogramme, die einer WGR zugeordnet werden können. So können Sie die Produktart oder -gruppe schnell erkennen.
    *   **Top-Warengruppen**: Top-Warengruppen aus dem Dialog Top-WGR. Sie können eine Warengruppe nur auf Warengruppenebene (WGR), nicht auf Warenhaupt- oder Warenobergruppenebene einer Top-Warengruppe zuordnen.
        *   ☐ Die Warengruppe ist nicht zugeordnet.
        *   ☑ Die Warengruppe ist der Top-WGR zugeordnet.
        *   ⇨ Tutorial 1, "Top-WGR" auf Seite B-151
        *   ⇨ "Top-WGR" auf Seite B-579

#### Kombi-WGR

**Stammdaten > Produkte > Allgemein > Kombi-WGR**

In diesem Dialog legen Sie Kombi-Warengruppen (Kombi-WGR) an. Wenn Sie in der Übersicht eine Zeile markieren, werden die entsprechenden Werte in den Feldern angezeigt und können bearbeitet werden.
⇨ Tutorial 1, "Regeln für Kombi-WGR" auf Seite B-146
⇨ Tutorial 1, "Warengruppen kombinieren" auf Seite B-154

**Ausgangswarengruppen**
*   **Warengruppe 1, 2**: Erste und zweite Warengruppe, die miteinander kombiniert sind. Hier sind alle Warengruppenebenen erlaubt.

**Kombinationswarengruppen**
*   **Warengruppe**: Kombi-WGR, nach deren Regeln die Warengruppe 1 und Warengruppe 2 kombiniert werden sollen. Die möglichen Kombi-WGR müssen im Dialog WGR angelegt sein.
    ⇨ "WGR" auf Seite B-575
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für statistische Auswertungen.
*   **Gültig für Rabattfindung**: Sie können angeben, ob die Kombi-WGR bei der Berechnung des Rabattes berücksichtigt werden soll.
    *   ☐ Die Kombi-WGR wird nicht bei der Berechnung des Preises berücksichtigt.
    *   ☑ Die Kombi-WGR wird bei der Preis- und Rabattfindung berücksichtigt. Die Checkbox **Kombi-Rabatt nur auf Hauptposition bilden** wird freigeschaltet.
*   **Gültig für Statistik**: Sie können angeben, ob die Kombi-WGR in der Statistik berücksichtigt werden soll.
    *   ☐ Die Kombi-WGR wird nicht in der Statistik berücksichtigt.
    *   ☑ Die Kombi-WGR wird in der Statistik berücksichtigt. Die Checkbox **Kombi-Statistik nur auf Hauptposition bilden** wird freigeschaltet.
*   **Kombi-Rabatt nur auf Hauptposition bilden**: Diese Checkbox ist nur freigeschaltet, wenn die Checkbox **Gültig für Rabattfindung** aktiviert wurde.
    *   ☐ Der gesamte Umsatz des Floats und der Bearbeitung wird zur Rabattfindung herangezogen.
    *   ☑ Nur die Hauptposition wird zur Rabattfindung herangezogen.
*   **Kombi-Statistik nur auf Hauptposition bilden**: Diese Checkbox ist nur freigeschaltet, wenn die Checkbox **Gültig für Statistik** aktiviert wurde.
    *   ☐ Der gesamte Umsatz des Floats und der Bearbeitung wird auf die Kombi-Warengruppe gebucht.
    *   ☑ Sie können in der Auswertung unterscheiden, wie viel Float mit und ohne Bearbeitung produziert wurde. Der Umsatz für die Bearbeitung selbst wird jedoch separat verbucht.

**Beispiel Kombiwarengruppe: 100 + 400 = 401**
| Produkt | WGR | Ergebnis Kombi-WGR |
| :--- | :--- | :--- |
| Float | 100 | 401 |
| Bearbeitung | 400 | 401 oder 400 |

**Übersicht**
In der Übersicht werden die angelegten Kombi-WGR aufgelistet.

#### Top-WGR

**Stammdaten > Produkte > Allgemein > Top-WGR**

In diesem Dialog legen Sie Top-Warengruppen (Top-WGR) an. In der Umsatzstatistik können Sie Auswertungen für diese Top-Warengruppen erstellen.

*   **Bezeichnung**: Name der Top-Warengruppe. Im Dialog WGR können Sie die gewünschte Warengruppe zuordnen.
    ⇨ "WGR" auf Seite B-575
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für statistische Auswertungen.

#### Varianten

**Stammdaten > Produkte > Allgemein > Varianten**

In diesem Dialog hinterlegen Sie die Farben, die Sie für die Definition von Produktvarianten verwenden können.
⇨ "Produktvarianten" auf Seite B-652

*   **Sprache**: Auswahl der Sprache, wenn Sie mit der Mehrsprachigkeit arbeiten. Verwenden Sie in allen Sprachen dieselben Schlüssel. Die Bezeichnung kann übersetzt werden.
*   **Variante**: Interne Nummer der Farbe. Diese Nummer benötigen Sie für die Zuordnung der Farbe zur Produktvariante.
*   **Bezeichnung**: Name der Farbe.
*   **Fremdschlüssel**: Bei Dorma-Artikeln der Dorma-Farbschlüssel. Der Fremdschlüssel kann für die Kommunikation mit anderen Programmen verwendet werden, z. B. für die Übergabe an die Produktion.
*   **Farbauswahl**: Öffnet den Dialog Farbe, um die Farbe festzulegen, in der z. B. die Sprossen in der Positionserfassung angezeigt werden. Die Farbe wird nicht an die Produktion übergeben.
*   **Vorschau**: Anzeige der gewählten Farbe.
*   **Sonderfarbe**: Im Auftrag kann bei bestimmten Produkten eine Sonderfarbe verwendet werden, z. B. beim Siebdruck.
    *   ☐ Die Farbe wird nicht als Sonderfarbe verwendet.
    *   ☑ Bei dieser Einstellung kann im Auftrag angegeben werden, welche Farbe verwendet werden soll.
    **Beispiel**: In einem Auftrag soll für einen Kunden ein Siebdruck mit einem bestimmten Motiv erfasst werden, z. B. ein Formel 1-Fahrzeug. Für diesen Fall muss eine Variante mit dem Kennzeichen **Sonderfarbe** für das Produkt Siebdruck angelegt sein. In der Positionserfassung wählen Sie dann für die Bearbeitung Siebdruck diese Produktvariante aus. Dadurch wird ein weiteres Feld angezeigt, in dem Sie den Namen des Motivs angegeben können. Dieser Name wird an die Produktion übergeben.
*   **Gesperrt**: Eine Variante kann für die Erfassung in der Produktverwaltung und in den Dokumenten gesperrt werden, wenn sie nicht mehr benötigt wird.
    *   ☐ Die Variante kann zugewiesen werden.
    *   ☑ Die Variante ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie Produkten und in Dokumenten zugewiesen ist, wird sie jedoch weiterhin angezeigt.

#### Sprossentypen

**Stammdaten > Produkte > Allgemein > Sprossentypen**

In diesem Dialog definieren Sie die Sprossentypen. Jeder Sprosse wird in der Produktverwaltung ein Sprossentyp zugeordnet.
⇨ "Konstruktionstyp" auf Seite B-608

> **Info: Neue Sprossentypen**
> Wenn Sie mit A+W Production arbeiten, müssen Sie neue Sprossentypen mit Ihrem Service-Mitarbeiter der A+W Software GmbH absprechen.

*   **Typ**: Interne Nummer. Diese Nummer muss mit der Nummer in der Produktionssoftware übereinstimmen.
*   **Bezeichnung**: Name des Sprossentyps.
*   **Randstopfenmaß**: Wert für das Randstopfenmaß in mm. Das Randstopfenmaß wird bei der Preisberechnung der Sprossenkonstruktion ausgewertet.
    ⇨ Verkauf, "Gitter" auf Seite C-510
*   **Kennz. Durchgang**: Angabe zur Verbindung mit anderen Sprossen:
    *   **0 - keine**: Das Kennzeichen ist nicht gesetzt, Sprossen des Typs können beliebig verarbeitet werden.
    *   **1 - waagerecht**: Waagerechte Sprossen des Typs müssen durchgängig sein.
    *   **2 - senkrecht**: Senkrechte Sprossen des Typs müssen durchgängig sein.
    *   **3 - waagerecht + senkrecht**: Waagerechte und senkrechte Sprossen des Typs müssen durchgängig sein.
    *   **6 - überlappend**: Waagerechte und senkrechte Sprossen des Typs können sich überlappen.
    *   **7 - längste Sprosse**: Die längste Sprosse des Typs muss durchgängig sein.
    ⇨ Tutorial 1, "Konstruktionstypen der Sprossen" auf Seite B-164
*   **Frästiefe**: Tiefe des Einschnitts im Abstandhalter.
*   **Spezialkreuzung**: Bei einigen Sprossentypen sind Spezialkreuze für die Verbindung erforderlich.
    *   ☐ Für den Sprossentyp wird kein Spezialkreuz verwendet.
    *   ☑ Für den Sprossentyp muss ein Spezialkreuz verwendet werden. Zusätzlich muss die Breite angegeben werden. Bei dieser Einstellung müssen das Kennzeichen für den Durchgang und die Fräßtiefe auf 0 (keine) stehen.
*   **Breite Spezialkreuz, 0=Sprossenbreite**: Breite des Spezialkreuzes im mm. Der Wert 0 zeigt an, dass die Breite des Spezialkreuzes sich nach der Sprossenbreite richtet.

#### Reklamationsverursacher

**Stammdaten > Produkte > Allgemein > Reklamationsverursacher**

In diesem Dialog hinterlegen Sie die Verursacher einer Reklamation. Die Werte können beim Erfassen einer Reklamation ausgewählt werden. Sie werden durch das Modul **Reklamationsstatistik** ausgewertet.

*   **Bezeichnung**: Name des Verursachers, z. B. Produktion, Auftragserfassung, Versand. Die Bezeichnung soll sich deutlich vom Reklamationsgrund unterscheiden.
    ⇨ "Reklamationsgrund" auf Seite B-584
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Finanzbuchhaltung oder für statistische Auswertungen.
*   **Gesperrt**: Ein Reklamationsverursacher kann für die Erfassung in den Dokumenten gesperrt werden, wenn er nicht mehr benötigt wird.
    *   ☐ Der Reklamationsverursacher kann zugewiesen werden.
    *   ☑ Der Reklamationsverursacher ist gesperrt und kann nicht mehr zugewiesen werden. Wenn er in Dokumenten zugewiesen ist, wird er jedoch weiterhin angezeigt.

#### Reklamationsgrund

**Stammdaten > Produkte > Allgemein > Reklamationsgrund**

In diesem Dialog hinterlegen Sie Gründe, die zu einer Reklamation geführt haben.
⇨ "Reklamationsverursacher" auf Seite B-583

*   **Bezeichnung**: Name für den Reklamationsgrund, z. B. Materialfehler, Produktionsfehler, Bruch.
*   **Kombi-WGR**: Kombi-WGR für die Auswertung. Über Kombi-WGR können die Stückzahlen ausgewertet werden, die aufgrund von Reklamationen produziert wurden. In der Reklamationsstatistik im Modul Statistik wird auch der entgangene Umsatz ausgewertet.
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Finanzbuchhaltung oder für statistische Auswertungen.
*   **Gesperrt**: Ein Reklamationsgrund kann für die Erfassung in den Dokumenten gesperrt werden, wenn er nicht mehr benötigt wird.
    *   ☐ Der Reklamationsgrund kann zugewiesen werden.
    *   ☑ Der Reklamationsgrund ist gesperrt und kann nicht mehr zugewiesen werden. Wenn er in Dokumenten zugewiesen ist, wird er jedoch weiterhin angezeigt.

#### Struktur

**Stammdaten > Produkte > Allgemein > Struktur**

In diesem Dialog werden die möglichen Strukturverläufe der Gläser angezeigt. Sie können die Einträge bearbeiten, jedoch nicht um weitere Verläufe ergänzen.

*   **Schlüssel**: Der Schlüssel (ID) ist von A+W Business vorgegeben und darf nicht verändert werden.
*   **Kurzbez.**: Einstellige alphanumerische Kurzbezeichnung, die geändert werden kann.
    **Beispiel**
    S = senkrecht oder V = vertikal
    W = waagrecht oder H = horizontal
*   **Bezeichnung**: Eindeutiger Name für den Strukturverlauf.

#### Strukturseite

**Stammdaten > Produkte > Allgemein > Strukturseite**

In diesem Dialog werden die möglichen Strukturseiten angezeigt. Sie können die Einträge bearbeiten und ergänzen, um bei Mehrfach-ISO oder VSG alle Seiten angeben zu können. Dabei hat jede Scheibe im ISO oder VSG zwei Seiten, die jeweils innen oder außen liegen.
⇨ Tutorial 1, "Strukturen und Beschichtungen" auf Seite B-162

*   **Ebene**: Die Nummern der Ebenen (Seiten im ISO-Aufbau) dürfen nicht verändert werden. Wenn Sie weitere Ebenen anlegen, wählen Sie fortlaufenden Nummern nach demselben Prinzip.
*   **Kurzbez.**: Einstellige alphanumerische Kurzbezeichnung für die Innen- und die Außenseite. Sie können sie ändern.
*   **Bezeichnung**: Eindeutiger Name der Ebene.

#### Beschichtungsseite

**Stammdaten > Produkte > Allgemein > Beschichtungsseite**

In diesem Dialog werden die möglichen Beschichtungsseiten angezeigt. Sie können die Einträge bearbeiten und ergänzen, um bei mehrfach ISO alle Ebenen angeben zu können. Dabei hat jede Scheibe im ISO zwei Seiten, die jeweils innen oder außen liegen.
⇨ Tutorial 1, "Strukturen und Beschichtungen" auf Seite B-162

*   **Ebene**: Die Nummern der Ebenen dürfen nicht verändert werden. Wenn Sie weitere Ebenen anlegen, wählen Sie fortlaufende Nummern nach demselben Prinzip.
*   **Kurzbez.**: Einstellige alphanumerische Kurzbezeichnung für die Innen- und die Außenseite. Sie können sie ändern.
*   **Bezeichnung**: Eindeutiger Name der Ebene.

#### Beschichtungsart

**Stammdaten > Produkte > Allgemein > Beschichtungsart**

In diesem Dialog werden die möglichen Beschichtungsarten angezeigt. Sie können die Einträge bearbeiten und ergänzen.
⇨Tutorial 1, "Strukturen und Beschichtungen" auf Seite B-162

*   **Schlüssel**: Der Schlüssel ist von A+W Business vorgegeben und darf nicht verändert werden.
*   **Kurzbez.**: Einstellige alphanumerische Kurzbezeichnung.
    **Beispiel**
    N = nicht beschichtet oder O = ohne
*   **Bezeichnung**: Eindeutiger Name der Beschichtungsart.

#### Glasartgruppen

**Stammdaten > Produkte > Allgemein > Glasartgruppen**

In diesem Dialog hinterlegen Sie die Glasartgruppen. Glasartgruppen benötigen Sie, wenn Sie mit A+W Production arbeiten. Die Glasartgruppen von A+W Production entsprechen den Produktarten von A+W Business.

**Beispiel**
1 = Float
2 = Isolierglas
3 = ...

Jedem Glasprodukt kann in der Produktverwaltung über das Register **A+W Production** eine Glasart und eine Glasartgruppe zugeordnet werden. Die Definition von Glasartgruppen dient in A+W Production zur Auswertung in Reports und in der Statistik. Für den Produktionslauf haben die Glasartgruppen keine Bedeutung.
⇨ "Glasarten" auf Seite B-644

*   **Bezeichnung**: Name der Glasartgruppe, z. B. Float, ESG, VSG.
*   **Schlüssel**: 1- bis 7-stellige Nummer der Glasartgruppe.

#### Gütetext

**Stammdaten > Produkte > Allgemein > Gütetext**

Gütetexte werden abhängig vom ISO-Aufbau und Landeskennzeichen der Lieferadresse in den Rahmentext eingefügt.

> **Voraussetzung**
> Der Dialog kann nur geöffnet werden, wenn in den **Firmendaten > Register Dokumente** die entsprechende Funktion ausgewählt ist.
> ⇨ "Produktkennzeichnung" auf Seite B-946

Im Dialog **Gütetext** finden Sie folgende Register:
*   Gütetext - Grundeinstellungen
*   Gütetext - Restriktionen

##### Gütetext - Grundeinstellungen

**Stammdaten > Produkte > Allgemein > Gütetext > Register Grundeinstellungen**

In diesem Register hinterlegen Sie die (landesspezifischen) Gütetexte, die in die Rahmentexte eingefügt werden sollen.
⇨Tutorial 2, "Textarten" auf Seite B-469

**Produktauswahl**
*   **Glas**: Glasartikel, für den ein Gütetext definiert ist.
*   **Gas**: Gas in der ISO-Scheibe.

**Werte**
*   **Priorität**: Über die Priorität legen Sie fest, welcher Gütetext genommen wird, falls in einer ISO-Einheit unterschiedliche Gläser enthalten sind, für die jeweils ein Gütetext erfasst ist.
*   **Land**: Die Gütetextanforderungen können sich von Land zu Land unterscheiden. Mit Hilfe des Landeskennzeichens können Sie für ein Glas unterschiedliche Texte pro Land definieren.
*   **Text**: Gütetext, der in den Rahmen gedruckt wird.

##### Gütetext - Restriktionen

**Stammdaten > Produkte > Allgemein > Gütetext > Register Restriktionen**

In diesem Register können Sie die automatische Verwendung des Gütetextes einschränken. Über eine Regel legen Sie fest, bei welchen Produktarten oder Produktgruppen der Gütetext nicht verwendet wird.
Die Felder im Bereiche **Produktauswahl** sind zum Register Grundeinstellungen beschrieben.
⇨ "Gütetext - Grundeinstellungen" auf Seite B-590

**Gültigkeitsbereich**
*   **Regel**: Die verfügbaren Regeln sind vom Programm vorgegeben.
*   **Parameter 1 - 4**: Die Anzahl der änderbaren Parameter hängt von der ausgewählten Regel ab.

**Restriktionen**
In der Übersicht werden für das ausgewählte Glas alle Regeln mit den zugehörigen Parametern aufgelistet.

#### Leistungserklärung Verwaltung

**Stammdaten > Produkte > Allgemein > Leistungserklärung Verwaltung**

In diesem Dialog verwalten Sie die Vorlagen für die Leistungserklärungen. Mit der Kombination von Nummer, Bezeichnung und Sprache haben Sie die Möglichkeit, eine Leistungserklärung in verschiedenen Sprachen mit derselben Nummer zu registrieren.
Zur Erstellung von Leistungserklärungen können die technischen Text in allen erforderlichen Sprachen hinterlegt werden.
⇨ "Technische Werte" auf Seite B-1063
Der Versand von Leistungserklärungen kann pro Kunde und Produkt aktiviert werden.

**Leistungserklärung**
*   **Nummer**: Nummer der Leistungserklärung.
*   **Bezeichnung**: Name der Leistungserklärung. Er sollte eindeutig und sprechend sein.

**Dateianhang**
*   **Sprache**: Sprache, in der die Leistungserklärung abgefasst ist.
*   **Link**: Pfad, in dem die Leistungserklärungen abgelegt sind. Standardmäßig liegen die Leistungserklärungen in demselben Verzeichnis, in dem die Datei-Anhänge abgelegt sind. Dieses Verzeichnis legen Sie in den Firmendaten fest.
    ⇨ "Dateianhänge" auf Seite B-946
*   **[Hinzufügen], [Entfernen]**: Über diese Schaltflächen stellen Sie eine sprachliche Version der Leistungserklärungen zur Verfügung oder entfernen sie aus der Auswahl.

**Übersicht**
In der Übersicht sind alle Leistungserklärungen aufgeführt, die den Produkten oder Kunden zugeordnet werden können.

#### Austauschgruppen

**Stammdaten > Produkte > Allgemein > Austauschgruppen**

In diesem Dialog legen Sie die Austauschgruppen fest. Diesen Gruppen müssen Sie die Produkte zuordnen, die für den Austausch zugelassen sind.
⇨ "Austauschzuordnung" auf Seite B-594
Mit diesen Definitionen legen Sie fest, dass in ISO und/oder VSG nur Gläser, Abstandhalter und Folien eingebaut werden können, die für diese Produkte vorgesehen oder geeignet sind.
Die Funktion müssen Sie in den Firmendaten aktivieren.
⇨ "Produktaustauschregeln für Stücklistenaustausch verwenden" auf Seite B-958
In den Stammdaten der Produkte mit Stückliste müssen Sie die gültige Gruppe angeben:
⇨ "Produktverwaltung – Stückliste" auf Seite B-625

*   **Nummer**: Nummer der Austauschgruppe.
*   **Bezeichnung**: Bezeichnung der Austauschgruppe.

#### Austauschzuordnung

**Stammdaten > Produkte > Allgemein > Austauschzuordnung**

In diesem Dialog ordnen Sie die Produkte einer Austauschgruppe zu. Damit legen Sie fest, welche Produkte für den Austausch verwendet werden dürfen.
In den Stammdaten der Produkte mit Stückliste können Sie die Gruppe mit den zulässigen Produkten angeben.
⇨ "Produktverwaltung - Stückliste" auf Seite B-625
Mit diesen Definitionen legen Sie fest, dass in ISO und/oder VSG nur Gläser, Abstandhalter und Folien eingebaut werden können, die für diese Produkte vorgesehen oder geeignet sind.
Die Funktion müssen Sie in den Firmendaten aktivieren.
⇨ "Produktaustauschregeln für Stücklistenaustausch verwenden" auf Seite B-958

**Neuanlage**
*   **Gruppe**: Bezeichnung der Austauschgruppe. Das Feld ist nur freigeschaltet, wenn Sie einer Gruppe ein Produkt zuordnen. Neue Austauschgruppen legen Sie im Dialog **Austauschgruppen** an.
    ⇨ "Austauschgruppen" auf Seite B-593
*   **Produkt**: Produkt, das der Austauschgruppe zugeordnet ist.

**Produktzuordnung**
In der Übersicht werden alle Zuordnungen angezeigt. Um eine Zuordnung zu ändern, müssen Sie die ungültige Zuordnung löschen und eine neue anlegen.

#### Klassifikatoren – Produkt

**Stammdaten > Produkte > Allgemein > Klassifikatoren > Produkte**
**Stammdaten > Marktpartner > Allgemein > Klassifikatoren > Produkte**

In diesem Register hinterlegen Sie Bezeichnungen für Produkt-Klassifikatoren. Der Dialog ist ausführlich zu Markpartnern beschrieben.
⇨ "Klassifikatoren" auf Seite B-764
Neben der Bezeichnung und einer Bemerkung müssen Sie zu jedem Klassifikator festlegen, welcher Wert ihm zugewiesen werden kann.
⇨ “Produktverwaltung - Anlagen/Klassifikatoren" auf Seite B-634

---

### Produktverwaltung

**Stammdaten > Produkte > Artikel > Artikel**

In A+W Business können Sie Ihre firmeneigene Produktstruktur abbilden. Sie sind frei in der Vergabe sowohl der Artikelnummer (bis zu 8 Stellen) als auch eines alphanumerischen Codes (Matchcode mit bis zu 15 Stellen).

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menüs in der Produktverwaltung" auf Seite B-596
*   "Produktverwaltung" auf Seite B-598
*   "Technische Parameter" auf Seite B-637
*   "Technische Parameter kopieren" auf Seite B-639
*   "Produktänderung" auf Seite B-640
*   "Produktkennzeichen Verwaltung" auf Seite B-641
*   "Glasarten" auf Seite B-644

#### Menüs in der Produktverwaltung

**Stammdaten > Produkte > Artikel > Artikel**

Über die Menüs der Produktverwaltung können Sie die Standardeinstellung des Dialoges bestimmen und andere Dialoge öffnen, ohne die Produktverwaltung zu schließen.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menü Optionen" auf Seite B-596
*   "Menü Funktionen" auf Seite B-597

##### Menü Optionen

**Stammdaten > Produkte > Artikel > Artikel > Menü Optionen**

Über dieses Menü können Sie die Standardeinstellungen des Dialogs festlegen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen. Folgende Einträge werden angezeigt:
*   **Fehlermeldungen A+W Production-Übergabe gesammelt ausgeben**: Übertragungsfehler bei der Übergabe der Produktionsdaten werden gesammelt in einer Meldung angezeigt.

##### Menü Funktionen

**Stammdaten > Produkte > Artikel > Artikel > Menü Funktionen**

Über dieses Menü können Sie weitere Dialoge öffnen, ohne den Dialog zu schließen. Das Menü ist in folgende Gruppen gegliedert:
*   "Gruppe Technische Parameter" auf Seite B-597
*   "Gruppe Preisverwaltung, Gruppe VK-Relevant, Gruppe EK-Relevant" auf Seite B-597
*   "Gruppe Druckkennzeichen" auf Seite B-597
*   "Gruppe A + W Production" auf Seite B-598
*   "Gruppe Ändern/Löschen" auf Seite B-598
*   "Gruppe CE" auf Seite B-598

**Gruppe Technische Parameter**
*   **Technische Parameter allgemein**: Öffnet den Dialog **Technische Parameter**, um technische Parameter auszulesen oder zu ändern.
    ⇨ "Technische Parameter" auf Seite B-637
*   **Technische Parameter Isolierglas**: Öffnet den Dialog **Technische Parameter**, um technische Parameter für ein ausgewähltes ISO-Glas auszulesen oder zu ändern.
    ⇨ "Technische Parameter" auf Seite B-637
*   **Technische Parameter kopieren**: Öffnet den Dialog **Technische Parameter**, um technische Parameter für ein ausgewähltes ISO-Glas zu kopieren.
    ⇨ "Technische Parameter kopieren" auf Seite B-639

**Gruppe Preisverwaltung, Gruppe VK-Relevant, Gruppe EK-Relevant**
*   **Aufruf Preisverwaltung VK, ΕΚ**: Öffnet die Preisverwaltung, in der der Verkaufs- oder der Einkaufspreis für das gewählte Produkt geändert werden kann.
    ⇨ "Preisverwaltung" auf Seite B-723
*   **Setzen für alle Stücklistenelemente**: Aktiviert das entsprechende Preiskennzeichen für alle Stücklisten-Komponenten.
    ⇨ "Produktverwaltung - Stückliste" auf Seite B-625
*   **Löschen für alle Stücklistenelemente**: Deaktiviert das entsprechende Preiskennzeichen für alle Stücklisten-Komponenten.

**Gruppe Druckkennzeichen**
*   **Setzen für alle Stücklistenelemente**: Aktiviert das Druckkennzeichen für alle Stücklisten-Komponenten.
*   **Löschen für alle Stücklistenelemente**: Deaktiviert das Druckkennzeichen für alle Stücklisten-Komponenten.

**Gruppe A + W Production**
*   **Selektierte Produkte an A+W Production übergeben**: Sendet die Daten des ausgewählten Produktes an A+W Production.
*   **Alle Stammdaten an A + W Production übergeben**: Sendet alle Glasartengruppen, Glasarten, Jumbos, Tische und Tischzuordnungen an A+W Production.
*   **A + W Production Stammdaten einlesen**: übernimmt die Stammdaten von A+W Production.

**Gruppe Ändern/Löschen**
*   **Selektierte Produkte ändern**: Öffnet den Dialog **Produktänderung**, in dem Sie die automatischen Zuschläge für das gewählte Produkt aktivieren oder deaktivieren können.
    ⇨ “Produktänderung" auf Seite B-640
*   **Selektierte Produkte löschen**: Löscht alle Produkte, die in der Übersicht aufgelistet sind.

**Gruppe CE**
*   **CE-Stammdaten importieren**: Diese Funktion ist nur freigeschaltet, wenn die entsprechenden Dateien zum Import bereitliegen. In der Regel werden die Daten bei der Installation und Konfiguration von A+W Business importiert.

#### Produktverwaltung

**Stammdaten > Produkte > Artikel > Artikel**

In diesem Dialog verwalten Sie Ihre Produkte, z. B. Einfachglas, ISO, VSG, ESG, Modelle, Sprossen, Bearbeitungen, Stückartikel wie Türgriffe, usw.
Im Dialog **Produktverwaltung** finden Sie folgende Register:
*   Produktverwaltung - Produkt
*   Produktverwaltung - Fertigung
*   Produktverwaltung - Preis/Zuschlag
*   Produktverwaltung – Lager/Einkauf
*   Produktverwaltung - Modelle/Bearbeitungen
*   Produktverwaltung – Stückliste
*   Produktverwaltung - Texte
*   Produktverwaltung – Sprachen
*   Produktverwaltung - A+W Production
*   Produktverwaltung – Anlagen/Klassifikatoren
*   Produktverwaltung – Sprossen
    ⇨ Tutorial 1, "Produktdaten" auf Seite B-135

##### Produktverwaltung – Produkt

**Stammdaten > Produkte > Artikel > Artikel > Register Produkt**

In diesem Dialog können Sie Ihre firmeneigenen Produkte anlegen und bearbeiten. Sie können die Artikelnummer (bis zu 8 Stellen) und den alphanumerischen Matchcode frei wählen. Die Artikelnummer kann nach dem Speichern neuer Produktdaten nicht mehr geändert werden.
⇨Tutorial 1, "Produkt anlegen" auf Seite B-184

**Artikel**
*   **Nummer**: Anzeige der Artikelnummer (Produktnummer). Wenn Sie neue Produktdaten anlegen, können Sie sich über die Lupe die freien Nummern anzeigen lassen.
    ⇨ "Freie Nummern / Bereiche" auf Seite B-800
*   **Matchcode**: Der Matchcode dient als Suchkriterium. Er kann bis zu 15 alphanumerische Zeichen enthalten.
*   **EAN**: EAN-Code bzw. GTIN-Code. In den USA kann das Feld für den UPC-Code verwendet werden.
*   **Bezeichnung (1 bis 3)**: Name und kurze Beschreibung des Produkts. Die Bezeichnung wird in der Positionserfassung angezeigt und beim Formulardruck ausgewertet.
    *   Bei Einzelscheiben, die in eine ISO-Einheit eingebaut werden, wird nur die erste Bezeichnung ausgelesen.
    *   Für die Bezeichnung 1 können Sie Variablen (Platzhalter) verwenden, um die Gültigkeitsdauer von Sonderrabatten bzw. Teuerungszuschlägen (Produktzuordnung Zuschläge) mit auszuweisen.
        ⇨Tutorial 2, "Variablen" auf Seite B-473
    *   Für die Bezeichnung 3 können Sie bei der Produktart Bearbeitungen Variablen (mit Formeln) verwenden. Im Dokument wird dieser Text vom System mit den Werten der Bearbeitungsparameter gefüllt.
        ⇨ Tutorial 2, "Verfügbare Variablen (Platzhalter)" auf Seite B-533
*   **[Formel]**: Öffnet den Dialog **Parameter-Ersetzung**, in dem Sie die zulässigen Parameter auswählen können. Achten Sie auf die Schreibweise, wenn Sie das Feld für Formeln nutzen, damit A+W Business den Text korrekt interpretieren kann.
    **Beispiele:**
    | Bezeichnung 3 im Dialog Produktverwaltung | Beschreibung im Dialog Positionserfassung |
    | :--- | :--- |
    | `<%> Kanten *<§>* mit Gehrung 45° poliert (<=> Ifm)` | `2 Kanten *2/3* mit Gehrung 45° poliert (2,45 Ifm)` |
    | `Sägen von <%> Kanten *<§>*` | `Sägen von 3 Kanten *2/3/4*` |
    | `<%> Lochbohrung(en) mit d = <$> mm` | `2 Lochbohrungen mit d = 20 mm` |
    | `<%> Bohrung(en) x/y/D in mm *<§>*` | `2 Bohrungen x/y/D in mm *100,100, 25-200,200,16*` |
    | `<%> x <$> mm Rundecke *<§>*` | `4 x 15 mm Rundecke *1/2/3/4*` |
    | `<$> Eckausschnitte/<%> Stück/*<§>*` | `100 x 75 Eckausschnitte/2 Stück/3/4*` |
    | `<%> Kante(n) *<$>* mit <$> mm Facette` | `2 Kante(n) *1/4* mit 20,0 mm Facette` |
    ⇨ Verkauf, "Parameter-Ersetzung" auf Seite C-603
*   **Kurzinfo**: Kurzinfo für den Etikettendruck (maximal 20 Zeichen), z. B. ISO 2 x FL4 für Isolierglas 2 x Float 4 mm oder FL4 für Floatglas 4 mm.
*   **Artikelinfo**: Feld für zusätzliche produktspezifische Informationen (ohne Zeichenlimitierung). Die Info kann in der Positionserfassung angezeigt werden.
*   **Anzeige**: Der Text aus dem Feld **Artikelinfo** kann beim Erfassen einer Position angezeigt werden.
    *   ☐ Der Text wird nicht automatisch angezeigt.
    *   ☑ Beim Erfassen des Produkts wird automatisch der Dialog **Artikel-Info** geöffnet, in dem der Aufbau der Stückliste und die Preise geprüft werden können.
*   **Anzeige in Stückliste**: Der Text aus dem Feld **Artikelinfo** kann in der Stückliste angezeigt werden, z. B. beim Austausch.
    *   ☐ Der Text wird nicht angezeigt, wenn das Produkt in einer Stückliste verwendet wird.
    *   ☑ Wenn die Checkbox **Anzeige** aktiviert ist, wird der Text in der Positionserfassung nur angezeigt, wenn das Produkt als Hauptprodukt erfasst wird.
    *   ☑ Der Text wird auch dann angezeigt, wenn das Produkt eine Stücklisten-Komponente ist.
*   **[Icon Info]**: Öffnet den Dialog **Artikel-Info**, um Details zum Produkt zu prüfen.
    ⇨ Verkauf, "Artikel-Informationen" auf Seite C-616
*   **[Icon Varianten]**: Öffnet den Dialog **Produktvarianten**, um Varianten zum Produkt zu prüfen oder anzulegen.
    ⇨ "Varianten" auf Seite B-580

**Eigenschaften**
*   **Produktart, Produktgruppe**: Jedem Produkt werden eine Produktart und eine Produktgruppe zugewiesen. Sie dienen als Ordnungskriterium bei der Suche und können in Auswertungen und zur Preisfindung bei Modellzuschlägen herangezogen werden.
    ⇨ "Produktarten" auf Seite B-573
    ⇨ "Produktgruppen" auf Seite B-574
    **Beispiele:**
    | Produktart | Produktgruppe | Produkt |
    | :--- | :--- | :--- |
    | Einfachglas | Einfachglas | Float 6 mm |
    | | Ornamentglas | Ornm. Altd. Glatt 4 mm, Ornm. Kathedral weiß 4 mm |
    | Bearbeitungen | Rundecken | Rundecke fein, Rundecke grob |
    | | Randausschnitt | Randausschnitt - 100 x 200 mm ESG |
    | ESG | ESG | ESG klar 12 mm |
    | | Ganzglastür | ESG Tür weiß |
    | ISO | ISO | CLIMALIT Standard 2 x 4 mm Float |
*   **WGR**: Jede der drei Warengruppenebenen kann dem Produkt zugewiesen werden. Wenn Sie z. B. zwischen ISO und ISO mit Modellen unterscheiden wollen, müssen Sie dem Modell eine WGR zuordnen. Zur Unterscheidung legen Sie dann für jede Auswertung eine Kombi-WGR an. Wenn Sie keine differenzierte Auswertung benötigen, tragen Sie den Wert 0 ein. Das Modell wird dann automatisch der Warengruppe des Hauptprodukts zugeordnet, also dem ISO oder dem Einfachglas.
    *   Tutorial 1, "Kombi-WGR" auf Seite B-145
    *   Softwarereferenz, "Kombi-WGR" auf Seite B-577
*   **WGR-Statistik**: In der Regel wird dieselbe WGR eingetragen wie im Feld WGR. Die WGR-Statistik bietet die Möglichkeit, für den Rabatt- und Statistikbereich unterschiedliche Warengruppenstrukturen aufzubauen.

**Einheiten / Restriktionen**
*   **Dicke / Sprossendicke**: Bei Gläsern die Glasdicke, bei Sprossen die Sprossendicke in mm.
*   **Gewicht**: Gewicht des Glases pro Mengeneinheit. Im Auftrag dient das Gewicht zur Berechnung eines Zuschlags, z. B. für den Transport bei besonders schweren Positionen.
    **Beispiel**: 1 mm Float wiegt 2,5 kg pro qm. 5 mm Float wiegen 5 x 2,5 kg = 12,5 kg pro qm.
*   **Breite / Höhe min.**: Mindestmaße für Breite und Höhe für die Positionserfassung. Die Werte werden während der Positionserfassung geprüft. Bei Unterschreitung wird eine Meldung angezeigt. Der Auftrag kann dann abgelehnt, mit einem anderen Produkt oder evtl. mit einem entsprechenden Zuschlag gefertigt werden, z. B. für Handzuschnitt.
*   **Fläche / Seitenverhältnis max.**: Höchstmaße für Fläche und Seitenverhältnis für die Positionserfassung. Seitenverhältnis 1:6 bedeutet, dass z. B. bei einer Breite von 600 mm die Höhe höchstens 3600 mm betragen darf. Die Werte werden bei der Positionserfassung geprüft. Bei Überschreitung wird in einer Meldung ein Ausweichartikel vorgeschlagen. Dieser kann dann abgelehnt oder akzeptiert werden. Wenn der Ausweichartikel abgelehnt wird, kann der Auftrag nicht gefertigt werden.
    ⇨ "Ausweichartikel" auf Seite B-604
    Im Register **Preis/Zuschlag** kann ein Zuschlag angegeben werden, der bei Überschreitung der Maße erhoben wird. Die Werte für die Fläche und Seitenverhältnis sollten sich an den entsprechenden Werten im Register **Preis/Zuschlag** orientieren.
    ⇨ "Produktverwaltung - Preis/Zuschlag" auf Seite B-611
*   **Breite / Höhe Standard**: Die eingetragenen Werte werden bei der Auftragserfassung vorgeschlagen. Sie können im Auftrag überschrieben werden.
*   **Mengeneinheit**: Die Mengeneinheit (Maßeinheit) legt fest, auf welcher Basis das Produkt im Auftrag erfasst und der Preis berechnet wird.
    **Beispiele:**
    | Einheit | Beschreibung |
    | :--- | :--- |
    | qm | Auftragserfassung durch Menge, Breite und Höhe. |
    | Stk | Auftragserfassung durch Menge, die Felder für Breite und Höhe sind gesperrt. |
    | lfm | Auftragserfassung als laufende Meter (Menge und Meter). Der Wert für die Länge wird in das Feld Höhe in m (Meter) eingetragen. |
    ⇨ "Preis- und Mengeneinheit" auf Seite B-711
*   **Sperrkennzeichen**: Für das Sperrkennzeichen stehen folgende Einträge zur Wahl:
    *   **Nicht gesperrt**: Das Produkt kann im Auftrag erfasst werden.
    *   **Gesperrt**: Das Produkt wird in der Produktsuche nicht angezeigt und kann im Auftrag nicht erfasst werden. Wenn die Produktnummer in der Positionserfassung eingegeben wird, wird eine entsprechende Meldung wird angezeigt.
    *   **Repliziert**: Wenn die Stammdaten nur in der Master-Datenbank (DB) gepflegt werden, können die Daten durch Replikation aktualisiert werden. Stammdaten mit dem Kennzeichen repliziert können in der Slave-DB nicht bearbeitet werden.

**Ausweichartikel / Fremdschlüssel**
*   **Ausweichartikel**: Der Ausweichartikel wird in der Auftragserfassung automatisch vorgeschlagen, wenn beispielsweise bestimmte Restriktionen überschritten wurden. Eine entsprechende Meldung wird dann angezeigt.
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Produktion oder die Finanzbuchhaltung.
*   **Fremdschlüssel Statistik**: Fremdschlüssel für den Datenaustausch mit einer externen Software für statistische Auswertungen.

**Artikelskizze**
*   **Dateiname**: Dateinamen der Grafik, die dem Produkt zugeordnet ist. Diese grafische Darstellung des Produkts kann im Dokument nur gedruckt werden, wenn die Checkbox **Druck auf Formular** aktiviert ist. Dieses Bild gibt nicht das Modell oder die eingebauten Sprossen wieder. Es ist daher nur für seltene Strukturgläser sinnvoll. Der Pfad wird in den **Firmendaten > Register System** angegeben.
    ⇨ "Pfad zu Produktbildern" auf Seite B-992
*   **Druck auf Formular**: Die Artikelskizze kann in den Formularen gedruckt werden.
    *   ☐ Die Skizze wird nicht in den Formularen gedruckt.
    *   ☑ Die Skizze wird in den Formularen gedruckt.

##### Produktverwaltung – Fertigung

**Stammdaten > Produkte > Artikel > Artikel > Register Fertigung**

In diesem Register legen Sie Parameter für die Fertigung fest, z. B. die Strukturseite oder die Verwendung in einer Stückliste.

**Shaping+Nesting - Parameter**
*   **Kantenqualität**: Die Kantenqualität muss dem Produkt zugewiesen werden, damit in der Produktion die richtige Kantenbearbeitung ausgeführt wird. Neben den Standard-Qualitäten können weitere (individuelle) Qualitäten ausgewählt werden, die der Produktion mit derselben Nummer bekannt sein müssen.

**Parameter Stücklisten**
*   **Stückliste nicht relevant für Fertigung**: Die Stückliste kann an die Produktion übergeben werden.
    *   ☑ Die Stückliste wird an die Produktion übergeben. Wählen Sie diese Einstellung, wenn der gesamte Produktaufbau selbst gefertigt wird. Sie können dann beim Erfassen eines Auftrags die Stückliste modifizieren, z. B. eine Scheibe austauschen.
    *   ☐ Die Stückliste wird nicht an die Produktion übergeben. Wählen Sie diese Einstellung, wenn Sie z. B. ein VSG nicht selbst produzieren. Das VSG ist dann ein Bestellartikel. Im Register Lager/Einkauf muss die Beschaffungsart **Bestellung** eingestellt werden.
        ⇨ "Beschaffungsart" auf Seite B-619
*   **Für ISO geeignet**: Ein Produkt kann für einen ISO-Aufbau ungeeignet sein.
    *   ☐ Das Produkt sollte nicht für ISO-Scheiben verwendet werden.
    *   ☑ Das Produkt kann in ISO-Scheiben verwendet werden.
*   **Strukturebene drehbar**: Bei Ornamentgläsern muss angegeben sein, ob die Strukturseite nach innen und außen eingebaut werden kann. Diese Einstellung gilt nicht für beschichtete Gläser.
    *   ☐ Wenn das Glas innen oder außen angebracht wird, ist in der Positionserfassung die Schaltfläche **Strukturebene** freigeschaltet. Dies gilt für Ornamentgläser. Für beschichtete Gläser gibt es in der Positionserfassung eigene Schaltflächen.
    *   ☐ Die Strukturebene kann nicht geändert werden. Das Glas muss immer auf der Standard-Ebene eingebaut werden, die im Bereich **Struktur** festgelegt ist.
    *   ☑ Das Glas kann beliebig eingebaut werden. In der Positionserfassung wird im Register **Stückliste** die Standard-Ebene angezeigt und kann geändert werden.
        *   Tutorial 1, "Strukturverlauf" auf Seite B-162
        *   "Struktur, Beschichtung" auf Seite B-609
*   **Wird in Stückliste gedruckt**: Das Produkt in der Stückliste kann im Formular gedruckt wird.
    *   ☐ Das Produkt wird nicht in der Stückliste gedruckt.
    *   ☑ Das Produkt wird im Druck als Stücklisten-Komponente ausgewiesen.

**Standard-Werte für abweichende Mengen**
Wenn Sie mit kaufmännischen Übermengen arbeiten, können Sie zu jedem Produkt angeben, wie viel Prozent der tatsächlich angegebenen Menge als Übermenge produziert werden darf. Das gilt entsprechend für die Angabe der Untermenge. In den Kundendaten muss festgelegt sein, ob der Kunde abweichende Mengen zulässt.

*   **Untermenge, Übermenge**: Prozentwert, z. B. 10 %. Die produzierte Menge darf dann 10 % unter oder über der im Auftrag erfassten Menge liegen. Diese Werte können kundenbezogen abweichend eingestellt werden.
    ⇨ “Übermengen" auf Seite B-859

**Abstandhalterkennzeichen**
Bei Produkten der Produktgruppe **Abstandhalter** können Sie weitere Kennzeichen festlegen. Das Abstandhalterkennzeichen aus den Varianten übersteuert das Kennzeichen aus den Produktstammdaten.

*   **Frei**: Zurzeit nicht genutzt.
*   **Verbundtyp**: Typ des Randverbunds, z. B. UV-Randverbund. Die Angabe wird von A+W Production vorgegeben.
*   **Rahmentyp**: Nummer des Rahmentyps, z. B. für Edelstahl, TPS, ALU. Die Nummer ist von A+W Production vorgegeben.
*   **Farbe**: Die Farbe wird von A+W Production vorgegeben.

**Parameter Fertigung**
*   **AW-Broke**: Fremdschlüssel, der an AWBroke und A+W CAD Designer (Shapes) übergeben wird. Insgesamt stehen elf Fremdschlüssel zur Verfügung, die teilweise fest vorgegeben sind.
    Für die bekannten Glasarten sind folgende Kennzeichen definiert:
    *   G01: Floatglas
    *   G02: ESG
    *   G03: VSG
    *   G04: Gussglas
    *   G05: Drahtglas
    *   G06: ISO
    *   G07: Ganzglasanlage
    *   G53: VSG-Folie
    *   G99: Metateil
    **Beispiel**: `G028000` - Dies ist ein ESG mit der Produktnummer 8000.
    Der vollständige Schlüssel besteht jeweils aus dem Buchstaben (= Kennzeichen), dem numerischen Anteil der Produktnummer und einem Punkt. Damit können z. B. Bearbeitungen für einzelne Glasarten getrennt von der Standard-Bearbeitung definiert werden. Fremdschlüssel für Farben werden an den Anfang des Glasfremdschlüssels gestellt.
    **Beispiele:**
    *   `GF10.028000`: ESG, die zu F10 gehörenden Farbe, Produktnummer 8000.
    *   `KGF15.02111`: Polierung auf ESG mit der zu F15 gehörenden Farbe.
*   **Schlüssel Optimierung**: Der Schlüssel wird zur Klassifizierung an A+W Production übergeben. Sie können eine abweichende Produktnummer (Schlüssel) eingeben, die für die Buchungen im kombinierten Lagerführungsmodus genutzt wird.
    ⇨ "Optimierung" auf Seite B-881
    ⇨ Lagerwirtschaft, "Lagerbuchungen bei kombinierter Lagerführung" auf Seite G-41
*   **Konstruktionstyp**: Die Felder sind nur bei Sprossen oder Bleiverglasung freigeschaltet. Sie können den jeweiligen Konstruktionstyp auswählen. Der Wert wird an A+W Production übergeben. Im ersten Feld tragen Sie den Konstruktionstyp, im zweiten Feld den Sprossentyp ein.
    ⇨ Tutorial 1, "Konstruktionstypen der Sprossen" auf Seite B-164
    ⇨ "Sprossentypen" auf Seite B-581
*   **Maßzuschlag Breite, Höhe**: Kennzeichen für den Zuschlag oder Abzug für Bearbeitungen. Die möglichen Zu- und Abschläge sind im Dialog **Maßzuschlag** hinterlegt.
    ⇨ "Maßzuschlag" auf Seite B-650
    Der Maßzuschlag gleicht den Materialverlust aus, der bei den unterschiedlichen Bearbeitungen entsteht. Der Maßzuschlag wird beim Zuschnitt berücksichtigt.
    **Beispiel**: Durch Polieren aller vier Kanten reduziert sich ein Float von 1000 x 1000 mm auf die Maße 998 x 998 mm. Als Maßzuschlag werden 2 mm angegeben. Die Scheibe wird mit den Maßen 1002 x 1002 mm zugeschnitten.

**Struktur, Beschichtung**
*   **Seite**: Bei Ornamentgläsern und bei beschichteten Gläsern wird angegeben, auf welcher Seite (Ebene) die Struktur oder die Beschichtung liegen soll. Die Angabe kann im Auftrag überschrieben werden.
    **Beispiel**: Die Strukturebene eines Ornamentglases liegt z. B. standardmäßig außen. Wird ausdrücklich gewünscht, dass sie innen liegen soll, so wird in den meisten Fällen ein sogenannter Strukturinnenzuschlag erhoben. Bei beschichtetem Glas liegt die Struktur durch die Produktion bedingt standardmäßig innen.
    ⇨Tutorial 1, "Strukturen und Beschichtungen" auf Seite B-162
*   **Verlauf**: Bei Ornamentgläsern ist der (Struktur-)Verlauf angegeben. Diese Angabe wird für den Zuschnitt benötigt.
    ⇨ "Struktur" auf Seite B-585
*   **Art**: Die Beschichtung muss oben liegen, um Beschädigungen durch die weitertransportierenden Rollen beim Zuschnitt zu vermeiden. Dies gilt insbesondere für weiche Beschichtungen. Bei harten Beschichtungen kann das Glas auch anders herum aufgelegt werden.

**Druck**
*   **Modellskizze, Sprossenskizze**: Im Formular können schematische oder maßstäbliche Skizzen für Modelle oder Sprossenkonstruktionen gedruckt werden. Die Einstellungen für den Druck können Sie in der Produktverwaltung, in der Positionserfassung und in der Formularverwaltung festlegen. In der Produktverwaltung können Sie den Druck zulassen oder unterbinden. Das Zusammenspiel der Einstellungen ist im Tutorial beschrieben.
    ⇨ Tutorial 2, "Skizzendruck" auf Seite B-486
*   **Senkbohrung**: Sie können mehrere Senkbohrungen mit unterschiedlichen Werten anlegen, z. B. als Standard-Einstellungen für verschiedene Glasarten oder als Bearbeitungsprodukt.
    *   **Typ**: Der Typ gibt an, ob die Senkbohrung innen und/oder außen liegt.
    *   **Winkel**: Winkel der Senkung. Er wird senkrecht zur Glasebene angegeben. Ein Winkel von 0° entspricht der geraden Schnittkante.
    *   **Erfassungsart**: Die Erfassungsart gibt an, welche Größe im Auftrag für die Senkbohrung angegeben werden muss.

##### Produktverwaltung – Preis/Zuschlag

**Stammdaten > Produkte > Artikel > Artikel > Register Preis/Zuschlag**

In diesem Register ordnen Sie die Zuschläge zu, die automatisch zu dem Produkt berechnet werden sollen.
Die Felder im Bereich **Artikel** sind zum Register **Produkt** beschrieben:
⇨ "Produktverwaltung - Produkt" auf Seite B-600

**Zuschläge/Rabatte anwenden**
In diesem Feld sind die automatischen Zuschläge aufgelistet.
*   ☐ Der Zuschlag wird nicht berechnet.
*   ☑ Der Zuschlag wird berechnet.
    ⇨ Tutorial 1, "Funktion der automatischen Zuschläge" auf Seite B-333
    ⇨ "Produktzuordnung Zuschläge" auf Seite B-1043
*   **Steuer**: Standardmäßig wird jedem Produkt das Steuerkennzeichen 1 zugeordnet. Sie können ein anderes auswählen. In einigen Ländern können auch mehrere Steuersätze zugeordnet werden, z. B. in Nord-Amerika. Wenn Sie keine Steuer aktiviert haben, wird für das Produkt keine Steuer berechnet, z. B. für das Produkt Anzahlung. Die Steuersätze selbst werden im Dialog **Steuer** gepflegt.
    ⇨"Steuer" auf Seite B-916

**Kostenrechnung**
*   **Kostenart, Kostenstelle**: Für die Kostenrechnung können Sie jedem Produkt eine Kostenart und eine Kostenstelle zuweisen. Die Daten können über externe Berichte ausgewertet werden. Die Einstellungen können in der Auftragserfassung überschrieben werden.
    *   "Kostenart" auf Seite B-925
    *   "Kostenstellen" auf Seite B-926

**Preis-Parameter**
*   **Preisdarstellung**: Der Preis eines Produktes kann im Formular unterschiedlich ausgewiesen werden:
    *   **Implizit**: Der Netto-Preis der Hauptposition beinhaltet alle Preise der Stücklisten-Komponenten, also auch die Modell- und Austauschzuschläge und die Bearbeitungen.
    *   **Explizit**: Die Preise der Stücklisten-Komponenten werden einzeln ausgewiesen.
    *   **Implizit in Preis pro ME**: Die Preise der Stücklisten-Komponenten werden umgerechnet auf die Preiseinheit des Hauptproduktes. Dieser Gesamtpreis der Preiseinheit wird im Dokument ausgewiesen, aber nur dann, wenn alle Stücklisten-Komponenten einer Position die gleiche Darstellungsart zugewiesen wurde.
*   **Übernahme Hauptpos.**: Wenn das Produkt in eine Stückliste übernommen wird, kann sich die Berechnung und Darstellung der Preise und Rabatte nach den Angaben richten, die zum Produkt der Hauptposition hinterlegt sind. Folgende Einstellungen sind möglich:
    *   **Keine Übernahme**: Die Preiseinstellungen werden nicht aus der Hauptposition übernommen.
    *   **Rabatt + Preisschlüssel**: Rabatt und Preisschlüssel sollen aus der Hauptposition übernommen werden.
    *   **Rabatt**: Nur der Rabatt soll aus der Hauptposition übernommen werden.
    *   **Preisschlüssel**: Nur der Preisschlüssel soll aus der Hauptposition übernommen werden.
    *   **Keine Übernahme (Netto b. Ind.Pr.HptPos.)**: Bei kundenindividuellen Preisen in netto sollen die Einstellungen aus der Hauptposition nicht übernommen werden.
    *   **Rabatt + Preisschlüssel (Netto b. Ind.Pr.HptPos.)**: Bei kundenindividuellen Preisen in netto sollen der Rabatt und der Preisschlüssel übernommen werden.
    *   **Rabatt (Netto b. Ind.Pr.HptPos.)**: Bei kundenindividuellen Preisen in netto soll nur der Rabatt übernommen werden.
    *   **Preisschlüssel (Netto b. Ind.Pr.HptPos.)**: Bei kundenindividuellen Preisen in netto soll nur der Preisschlüssel aus der Hauptposition soll übernommen werden.
    *   **Rabatt + Preisschlüssel (auch falls Rabatt vorh.)**: Rabatt und Preisschlüssel aus der Hauptposition sollen auch dann übernommen werden, wenn im Stücklisten-Produkt ein Rabatt angegeben ist, z. B. beim Austausch eines Glases.
    *   **Rabatt (auch falls Rabatt vorh.)**: Der Rabatt aus der Hauptposition soll auch dann übernommen werden, wenn im Stücklisten-Produkt ein Rabatt angegeben ist, z. B. beim Austausch eines Glases.
    *   **Preisschlüssel (auch falls Rabatt vorh.)**: Der Preisschlüssel aus der Hauptposition soll auch dann übernommen werden, wenn im Stücklisten-Produkt ein Rabatt angegeben ist, z. B. beim Austausch eines Glases.
    Zur Übernahme von Rabatten siehe auch:
    ⇨ "Rabattverwaltung - Austauschrabatte" auf Seite B-821
    > **Info: Einstellungen zur Preisfindung in den Firmendaten**
    > Im Dialog **Firmendaten > Register Preisberechnung** werden übergreifende Einstellungen festgelegt, die die Einstellungen in den Produktstammdaten z. T. überschreiben können.
*   **Preistabelle VK/EK**: Nummern der Preistabellen, die zur Berechnung es Verkaufspreises und des Einkaufspreises herangezogen werden. Die Produkte und die dazugehörigen Preise werden getrennt angelegt. In der Regel sind Produktnummer und Nummer der Preistabelle gleich. Eine Unterscheidung ist nur dann sinnvoll, wenn viele unterschiedliche Produkte denselben Preis haben.
    *   Tutorial 1, "Preistabellen" auf Seite B-233
    *   **[Preistabelle]**: Öffnet den Dialog zur Bearbeitung der Preise.
        ⇨ "Preise" auf Seite B-725
*   **Grundprodukt**: Nummer der Preistabelle, die als Berechnungsgrundlage dient, wenn BEIDE Gläser in einem ISO ausgetauscht werden. Wenn eine Preistabelle angegeben ist, wird in der Auftragserfassung automatisch eine Meldung angezeigt, die abfragt, ob tatsächlich auf die Grundtabelle zurückgegriffen werden soll. Wird kein Glas oder nur ein Glas ausgetauscht, so wird auf den Eintrag im Feld **Preistabelle** zurückgegriffen.
*   **Tab. Austauschzuschl.**: Nummer der Tabelle für Austauschzuschläge. Jeder Isolierglastabelle kann ein anderer Austauschzuschlag zugeordnet werden.
    *   ⇨ Tutorial 1, "Funktion des Austauschzuschlags" auf Seite B-296
    *   ⇨ "Austauschzuschläge" auf Seite B-677
*   **Mindermengenzuschl.**: Nummer des Mindermengenzuschlags. Bei Gläsern kann ein Zuschlag angegeben werden, der immer dann erhoben wird, wenn im Auftrag eine bestimmte Menge (Fläche) unterschritten wird. Der Mindermengenzuschlag muss als Produktzuordnung Zuschlag angelegt sein.
    *   ⇨Tutorial 1, "Funktion der automatischen Zuschläge" auf Seite B-333
    *   ⇨ "Produktzuordnung Zuschläge" auf Seite B-1043
*   **Sonstiger Zuschlag**: Sonstige Zuschläge können aus unterschiedlichen Gründen erhoben werden, z. B. ein Zuschlag für eine Kantenlänge größer 3760 mm, da diese Länge schwerer zu bearbeiten ist.
    *   ⇨ Tutorial 1, "Funktion der Sonstigen Zuschläge" auf Seite B-314
    *   ⇨ "Sonstige Zuschläge" auf Seite B-675
*   **Zuschlagsart**: Zuschlagsarten geben an, auf welcher Basis der jeweilige Zuschlag berechnet werden soll:
    *   **akt. Bearbeitung**: Für die markierte Komponente in der Stückliste.
    *   **alle vorherigen Bearbeitungen**: Für alle Bearbeitungen, die vor der markierten Komponente in der Stückliste aufgeführt werden.
    *   **alle vorherigen Positionen**: Für alle Komponenten, die vor der markierten Komponente in der Stückliste aufgeführt werden.
    *   **Basisposition**: Für die oberste Position (Produkt) in der Stückliste, der ebenfalls ein Zuschlag zugewiesen sein kann.
    *   **Basisposition ohne sonstige Zuschläge**: Für die oberste Position in der Stückliste, ohne den Zuschlag, der dem Produkt zugewiesen sein kann.
    *   **Basisposition + Bearbeitungen**: Für die oberste Position in der Stückliste und die zugehörigen Bearbeitungen.
    *   **Basisposition + Modell**: Für die oberste Position in der Stückliste und das zugehörige Modell.
    *   **Basispreis**: Für den Preis der obersten Position in der Stückliste.
    *   **Vater + dessen Gläser**: Für die oberste Position einer Baugruppe (Vater) und der Gläser dieser Baugruppe.
    *   **Vater + dessen vorh. Bearbeitung**: Für die oberste Position einer Baugruppe (Vater) und die Bearbeitung, die an diese Komponente angehängt ist.
    *   **vorher. Stckl. m. gl. Vater**: (Vorherige Stückliste mit gleichem Vater). Alle Komponenten der Baugruppe.
    *   **vorherige Bearbeitung**: Alle Bearbeitungen, die vor der Komponente aufgeführt sind, zu der der Zuschlag festgelegt wurde.
    Alle Zuschlagsarten können sowohl additiv als auch nicht additiv berechnet werden. Die Alternative nicht additiv bezieht sich nur auf prozentuale Zuschläge. Der Einstellung entsprechend wird ein Wert gebildet, der als Grundlage zur Berechnung des prozentualen Zuschlages dient.
    ⇨Tutorial 1, "Berechnungen nach Zuschlagsarten" auf Seite B-319
*   **Maßrundung Breite / Höhe**: In Deutschland basiert die Preisberechnung auf einer 30er-Rundung. Dies bedeutet, dass zur Berechnung der nächste durch 30 teilbare Wert für die Kantenlänge zugrunde gelegt wird. In Frankreich wird mit einer 10er-Rundung gerechnet.
    **Beispiel**: Rundung 30: Bei einem Glas von 1000 x 1000 mm wird die Fläche 1,04 (= 1020 x 1020) berechnet.
*   **Fläche max.**: Höchstmaß für die Fläche, für die der reguläre Preis berechnet wird. Der Wert wird bei der Positionserfassung geprüft. Bei Überschreitung wird der angegebene **Sonstige Zuschlag** (Übergrößenzuschlag) berechnet. Der Wert für die Fläche und für das Seitenverhältnis (im nachfolgenden Feld) sollte sich an den entsprechenden Werten im Register **Produkt** orientieren.
    ⇨ "Fläche / Seitenverhältnis max." auf Seite B-603
*   **Seitenverhältnis max.**: Höchstmaß für das Seitenverhältnis. Der Wert wird im Verhältnis von 1 : x angegeben. 1: 6 bedeutet, dass bei einer Breite von 600 mm die Höhe höchstens 3600 mm betragen darf. Bei Überschreitung wird der angegebene **Sonstige Zuschlag** berechnet.
*   **Mittlerer Verschnitt**: Dieser Wert wird bei der Berechnung des EK-Preises für Glas, für Gas (Verlust) und bei der Berechnung der reservierten Lagermenge, berücksichtigt.
    **Beispiel: Verschnitt = 5 %, EK = 8,00 €/qm**
    | Scheibe | EK |
    | :--- | :--- |
    | 1000 x 1000 mm | 8,00 € |
    | **Scheibe** | **Verschnitt** | **Berechnete Fläche** | **EK** |
    | 1000 x 1000 mm | 0,05 qm | 1,05 qm | 8,40 € |
    ⇨Lagerwirtschaft, "Einkaufspreis und Durchschnitts-EK" auf Seite G-52
*   **Bearbeitungsindex**: Der Bearbeitungsindex bewertet den Aufwand und die Schwierigkeit bei der Bearbeitung des Produkts. Das Feld ist nur bei Glasprodukten freigeschaltet. Für den Preis kann der Bearbeitungsindex als Grenztyp eingegeben werden.
    ⇨ Tutorial 1, "Grenztypen für Staffelungen" auf Seite B-254
*   **Preisrelevant VK, EK**: Das Produkt kann bei der Berechnung des Preises für den Verkauf und/oder den Einkauf berücksichtigt werden. Bei Produkten mit einer Stückliste bezieht sich diese Checkbox auf die Hauptposition.
    *   ☐ Das Produkt wird im Auftrag nicht bei der Preisberechnung des VK und/ oder des EK berücksichtigt. Diese Einstellung können Sie verwenden, wenn das Produkt als Stücklisten-Komponente verwendet werden soll und der Preis dann über das Hauptprodukt ermittelt wird, z. B. Folie im VSG.
    *   ☑ Für die Preisberechnung wird auf die zugehörige Preistabelle für VK und/ oder EK zurückgegriffen. Für Gläser in ISO-Einheiten, die im Auftrag ausgetauscht werden, hat diese Angabe keine Bedeutung, da die Preise dann nach den hinterlegten Austauschpreisen berechnet werden.
        ⇨ Tutorial 1, "Kennzeichen zur Preisberechnung" auf Seite B-170
*   **Rabattfähig, Skontofähig**: Angabe, ob im Auftrag ein Rabatt oder Skonto zur Preisberechnung zugelassen ist. Beide Einstellungen können im Auftrag überschrieben werden.
    *   ☐ Für die Preisberechnung wird im Auftrag kein Rabatt berücksichtig, bzw. kann kein Skonto eingeräumt werden. Selbst wenn für eine Warengruppe ein Rabatt angelegt wurde, ist es an dieser Stelle möglich, ihn nicht zu gewähren. Dasselbe gilt für die Skontofähigkeit.
    *   ☑ Rabatt und/oder Skonto sind im Auftrag möglich.
*   **ISO-Aufbau Preis**: Für flexible Isolierglasaufbauten bis 3-fach Isolierglas kann eine Preistabellenzuordnung definiert werden. Im Verwaltungsprogramm (**Stammdaten > Preise > ISO Preise**) kann dann für einen bestimmten Produktaufbau (Glas, Abstandhalter und Gas) eine Zuordnung auf einzelne Preistabellen erfolgen.
    *   ☐ Es erfolgt keine Zuordnung zu dieser Preistabelle und der Preis wird normal ermittelt.
    *   ☑ Es wird der Preis aus dieser Preistabelle verwendet.

##### Produktverwaltung – Lager/Einkauf

**Stammdaten > Produkte > Artikel > Artikel > Register Lager/Einkauf**

In diesem Register legen Sie die Parameter für den Einkauf und die Lagerführung des Produktes fest.

**CPIP-Daten**
Die Felder in diesem Bereich werden nur angezeigt, wenn in den Firmendaten die CPIP-Bildung aktiviert ist. Damit die Daten korrekt eingegeben und geprüft werden können, müssen bei der Installation und Konfiguration von A+W Business die entsprechenden Dateien importiert worden sein.
⇨ "CPIP-Bildung" auf Seite B-966

*   **CE-relevant**: Die CPIP-Daten können unabhängig vom CE-Kennzeichen gekennzeichnet werden.
    *   ☐ Der CPIP-Code hat für die CE-Kennzeichnung keine Bedeutung.
    *   ☑ Der CPIP-Code ist Bestandteil der CE-Kennzeichnung.
*   **Zertifizierung**: Zertifizierung, die für das Produkt zutrifft. Die Zertifizierungen müssen in den Stammdaten zur CE-Kennzeichnung hinterlegt sein. Folgende Werte stehen zur Wahl:
    *   **Selbsterklärt**:
        *   **Alle Produkttypen**: Der CPIP-Code kann gebildet werden, die CE-relevanten Komponenten dürfen nicht gelöscht werden.
        *   **Einfachglas, VSG**: Durch Tauschen oder Hinzufügen CE-relevanter Komponenten wird der CPIP-Code entfernt.
        *   **ISO**: Nach einem Austausch von CE-relevanten Komponenten wird die Suche nach dem CPIP-Code neu gestartet. Wenn die getauschten Komponenten nicht durch die ISO-CPIP-Suche abgefragt werden, wird der CPIP-Code entfernt.
    *   **Zertifiziert, Zertifiziert mit Maßrestriktion**:
        *   **Alle Produkttypen**: Der CPIP-Code muss gebildet werden, die CE-relevanten Komponenten dürfen nicht gelöscht werden.
        *   **Einfachglas, VSG**: Tauschen oder Hinzufügen CE-relevanter Komponenten ist nicht zulässig.
        *   **ISO**: Wenn kein CPIP-Code gefunden wurde, können die Eingaben nicht gespeichert werden.
    ⇨ “CE-Kennzeichen" auf Seite B-1101
*   **Typ**: Auswahl des Produkttyps.
*   **CPIP-Code**: CPIP-Code für das Produkt. Während der Eingabe wird der Code entsprechend der Einstellung im Feld **Zertifizierung** geprüft.
    ⇨"CPIP-Code" auf Seite B-1101

**SAP Produkt Identifikation**
*   **Materialtyp**: Nummer des Materialtyps, der in SAP für dieses Produkt angegeben ist.
*   **Produktcode**: Produktnummer, die in SAP für dieses Produkt angegeben ist.
*   **Statistikcode**: Nummer der Auswertung, die in SAP für dieses Produkt verwendet wird.

**Parameter Bestellung**
*   **Maximale Breite, Maximale Höhe Bestellung**: Die Werte geben die Höchstmaße der Glasplatte für den Einkauf an. Wenn diese Werte im Auftrag überschritten werden, kann die Position weder in Eigenfertigung erzeugt noch bei einem externen Lieferanten bestellt werden. Die Höchstmaße für die Lagerführung können unter diesen Werten liegen. Diese Maße werden im Bereich **Parameter Lagerführung** angegeben.

**Produktkennzeichen**
*   **Beschaffungsart**: Die Beschaffungsart legt fest, wie das Produkt für den Auftrag beschafft wird:
    *   **Produktion**: Die Auftragsposition wird selbst produziert. Wenn ein Hauptartikel mit dieser Beschaffungsart gekennzeichnet ist, können dessen Stücklisten-Komponenten als Lagerartikel oder als Bestellartikel definiert werden.
        ⇨Tutorial 1, "Beschaffungsart" auf Seite B-173
    *   **Zuschnitt**: Das Glas für die Auftragsposition wird aus Lagerplatten zugeschnitten. Die Daten werden an die Produktion übergeben.
    *   **Lagerentnahme**: Das Produkt wird als Lagerartikel mit seinen genauen Abmessungen oder als Stückartikel im Lager geführt. Bei der Auftragserfassung wird die erfasste Menge reserviert.
    *   **Bearbeitung**: Die Bearbeitungen für eine Auftragsposition werden an die Produktion übergeben.
    *   **Kundeneigenes Glas**: Das Produkt wird vom Kunden angeliefert und für die Produktion seiner Aufträge verwendet.
    *   **Bestellung**: Nur das betreffende Produkt wird bestellt, ohne den Inhalt der Stückliste zu beachten. Besteht z. B. ein VSG aus einem Float, einer Folie und einem ESG und ist nur das ESG als Bestellung gekennzeichnet, so wird nur das ESG beim Lieferanten bestellt. Das VSG wird in Eigenfertigung produziert.
    *   **Bestellung (komplett)**: Das Produkt wird inklusive aller Bearbeitungen, die im Auftrag in der Stückliste erfasst wurden, bestellt. Besteht z. B. ein VSG aus einem Float 5 mm, einer Folie und einem ESG 5 mm, so wird das VSG als Ganzes bestellt. Beachten Sie hierzu die Abgrenzung zum Kennzeichen **Bestellung**.
    *   **Lagerzugang durch Produktion**: Das Produkt soll nur in Produktionsaufträgen verwendet werden, um das Lager zu füllen. Die produzierten Positionen werden dem Lager zugebucht.
        ⇨ Tutorial, "Produktionsaufträge" auf Seite E-130
*   **Lagerbuchungsart**: Die Lagerbuchungsart legt fest, wie ein Produkt als Lagerartikel in der Lagerverwaltung geführt wird:
    *   **Maßabhängig**: Wählen Sie diese Einstellung, wenn Lagermaße als Stückartikel geführt werden sollen. Die Einstellung ist nur für Glas sinnvoll. Die Mengeneinheit im Register **Produkt** setzen Sie trotzdem auf **qm**, damit die Fläche berechnet wird.
    *   **Nicht maßabhängig**: Wählen Sie diese Einstellung, für alle Lagerartikel, die in ihrer eigentlichen Mengeneinheit geführt werden sollen, z. B. Stückartikel, Beschläge. Wählen Sie diese Einstellung auch für Gläser, die in qm geführt werden sollen.
    *   **Kombiniert**: Wählen Sie diese Einstellung, wenn Sie mit Rückmeldungen aus der Produktion arbeiten. Die Einstellung ist nur für Glas sinnvoll. Vergessen Sie nicht, dass Sie dazu ein Dummy-Lagermaß ohne Maße anlegen müssen.
    ⇨Tutorial, "Wie soll das Lager geführt werden" auf Seite G-17
    Die Einstellung **ohne** wird in diesem Zusammenhang nicht benutzt.
*   **Automatischer Zuschnitt**: Dieses Kennzeichen wird an A+W Production übergeben.
    *   ☐ A+W Production fügt die Scheibe der Liste der Sonderzuschnitte zu. Diese Scheibe wird dann nicht von der Maschine, sondern von Hand zugeschnitten.
    *   ☑ A+W Production leitet die Scheiben an die Schneidmaschine weiter und optimiert gleichzeitig den Zuschnitt.
*   **Keine Verfügbarkeitsprüfung**: Für jedes Produkt kann im Dialog **Lagerinfo** geprüft werden, ob der aktuelle Bestand für die anstehenden Aufträge ausreicht. Wenn Sie die Verfügbarkeitsprüfung auf die Produkte beschränken, für die im Lager tatsächlich Bestände gepflegt werden, erhöhen Sie die Performance des Systems.
    *   ☐ Für das Produkt wird eine Verfügbarkeitsprüfung durchgeführt.
    *   ☑ Die Verfügbarkeit wird für das Produkt nicht geprüft. Das Produkt wird im Dialog **Lagerinfo** nicht angezeigt. Diese Einstellung ist dann sinnvoll, wenn Sie ein Produkt zwar im Lager haben, aber nicht als Lagerartikel führen.
*   **Technische Artikelnummer**: Pro Glasart-Dicke-Kombination kann bei der Beschaffungsart **Zuschnitt** eine alphanumerische technische Artikelnummer angegeben werden. Diese Nummer wird in der Regel von A+W Production vorgegeben.
*   **Abweichende Produktkennzeichen**: Öffnet den Dialog **Produktkennzeichen Verwaltung**, um ein anderes Produktkennzeichen auszuwählen, z. B. aus einem anderen AV-Bereich.
    ⇨ "Produktkennzeichen Verwaltung" auf Seite B-641

**Parameter Lagerführung**
*   **Maximale Breite, Maximale Höhe Lager**: Höchstmaße für die Lagerplatten, die im Lager geführt werden können. Alle Auftragspositionen innerhalb der festgelegten Maße können aus dem Lagerbestand gefertigt werden. Zwischen den Parametern für die Bestellung und denjenigen für die Lagerführung muss unterschieden werden. Auftragspositionen, deren Maße zwischen denen der Lagerführung und denen der Bestellung liegen, können bei einem Lieferanten bestellt werden. Überschreiten die Maße jedoch die Parameter **Bestellung**, so kann der betreffende Artikel weder gefertigt noch bei einem Lieferanten bestellt werden.

**Produktkennzeichnung**
*   **CE Kennzeichnung**: Sie können ein CE-Kennzeichen für das Produkt (mit seinem Standard-Aufbau) eintragen. Das CE-Kennzeichen wird in den Auftrag übernommen und kann in den Formularen gedruckt werden. Bei der Produktionsübergabe kann es an A+W Production übergeben werden.
    > **Info: CE-Kennzeichnung bei mitgeliefertem Glas**
    > Bei der Bestellung von Lohnhärten wird die CE-Kennzeichnung für das Glas aus den Stammdaten ausgelesen. Der Besteller muss die CE-Kennzeichnung des Basisglases an seinen Lieferanten (Lohnhärter) weitergeben. Nur so kann dieser die CE-Konformität ebenfalls bescheinigen.

##### Produktverwaltung – Modelle/Bearbeitungen

**Stammdaten > Produkte > Artikel > Artikel > Register Modelle/Bearbeitungen**

In diesem Register legen Sie die Daten für die Modelle und Bearbeitungen fest, die im Verkauf einer Scheibe zugeordnet werden.

> **Info: Produktart und Produktgruppe für Modelle**
> A+W Business unterscheidet Standardmodelle und das Modell für Stufen-Isolierglas. Dementsprechend müssen Sie auch die Produktgruppe definieren und die Modell-Nummer. Standardmodelle verwenden die Modell-Nr. 1 – 99, das Modell für Stufen-Isolierglas hat die Nummer 999.

Eine ausführliche Beschreibung der Daten, die Sie in diesem Register erfassen können, finden Sie im Part **Verkauf**:
*   ⇨ Verkauf, "Positionen – Bearbeitungen" auf Seite C-479
*   ⇨ Verkauf, "Positionen - Stufung" auf Seite C-498
*   ⇨ Verkauf, "Positionen - Gebogenes Glas" auf Seite C-499
*   ⇨ Verkauf, "Positionen – Bleiverglasungen" auf Seite C-501
*   ⇨ Verkauf, "Positionen – Modell-Template" auf Seite C-502

**Stückliste**
Bearbeitungen können an einzelnen Komponenten der Stückliste ausgeführt werden. Angaben zum Modell betreffen immer das Hauptprodukt. In der Ansicht wird das Modell schematisch angezeigt. Die Legende bezeichnet die Felder, in denen die Maße eingegeben werden.

**Bearbeitungen**
*   **Schaltflächen**: Mit den Schaltflächen wählen Sie eine Produktgruppe aus, z. B. Modelle, Bearbeitungen, gebogenes Glas oder Bleiverglasung. Wenn der Produktgruppe verschiedene Produkte zugewiesen sind, können Sie das gewünschte Produkt im Dialog **Auswahl** markieren und übernehmen.
*   **Artikel**: Produktnummer und Bezeichnung aus den Stammdaten.
*   **Formel**: Auswahl und Anzeige der Formel für den Bearbeitungstext.

**Modell**
*   **Symbole**: Über diese Schaltflächen können Sie ein Modell auswählen.
*   **Artikel**: Die Produktnummer des Modells wird aus den Stammdaten übernommen.
*   **Modell**: Die Modellnummer wird aus den Stammdaten übernommen.
*   **Bezeichnung**: Die Bezeichnung des Modells wird aus den Stammdaten übernommen.

**Parameter**
*   **W, H**: Zu jedem Modell werden nur die Felder freigeschaltet, die zur Produktion des Modells notwendig sind. Die Bezeichnungen für die Kanten werden in der Ansicht gezeigt.
*   **Restriktionen**: In diesem Bereich finden Sie Angaben zu den Restriktionen. Beispiel: H1>0 bedeutet, dass die Kante H1 nicht 0 sein darf.
*   **S+N Datei**: Wenn Sie häufiger ein bestimmtes Modell mit identischen Maßen erfassen, können Sie es als S+N-Datei speichern. In späteren Aufträgen können Sie diese Datei über die Schaltfläche [Ordner] dann auswählen und der Auftragsposition zuordnen, ohne die Details neu eingeben zu müssen. Wenn Sie das Modell 99 ausgewählt haben, können Sie auch ein S+N-Template laden und zuordnen.

**Preise**
*   **Jahrgang/Schlüssel**: Preisjahrgang und -schlüssel für den Modellzuschlag werden aus den Stammdaten übernommen. Sie können geändert werden.
*   **Preis/PE**: Preis und Preiseinheit für den Modellzuschlag aus den Stammdaten. Sie können geändert werden.
*   **Rabatt**: Rabatt für den Modellzuschlag aus den Stammdaten. Er kann geändert werden.
*   **Netto**: Der Nettobetrag für den Modellzuschlag wird automatisch angezeigt.

**Skizzendruck**
Sie können auswählen, wie das Modell im Druck wiedergegeben werden soll:
*   **Kein Druck**: Die Skizze wird nicht auf den Formularen gedruckt.
*   **Modell (maßstäblich)**: Bei dieser Einstellung werden maßstabsgetreue Modellskizzen gedruckt.
*   **Modell (schematisch)**: Bei dieser Einstellung werden die Standardskizzen gedruckt. Sie geben lediglich das Schema des Modells wieder.

##### Produktverwaltung – Stückliste

**Stammdaten > Produkte > Artikel > Artikel > Register Stückliste**

In diesem Register wird die Stückliste ISO- oder VSG-Scheiben abgebildet. Zusätzlich werden Informationen zu den Stücklisten-Komponenten angegeben.
⇨ Tutorial 1, "Stücklistenaufbau bearbeiten" auf Seite B-187
⇨ Tutorial 1, "Produktionsstücklistenauflösung festlegen" auf Seite B-192

**Stückliste**
In der Übersicht werden alle Stücklisten-Komponenten aufgeführt. Die Ebene gibt wieder, an welches Produkt die Komponente angehängt wurde. Wenn Sie eine Komponente markieren, werden deren Details in den zugehörigen Feldern angezeigt. Für die oberste Ebene (Hauptprodukt) bleiben die Felder leer.

**Produktionsstücklistenauflösung**
In der Übersicht werden alle Bearbeitungen angezeigt, die am Produkt ausgeführt werden können. Mit der Markierung der Checkboxen legen Sie fest, ob die Bearbeitung am Hauptprodukt oder an der Stücklisten-Komponente ausgeführt wird. Wenn zu den Stücklisten-Komponenten keine Checkboxen markiert sind, werden die Bearbeitungen am Hauptprodukt ausgeführt.
**Beispiel**: In einem VSG haben Sie die Bearbeitungen für Kanten an den Stücklisten-Komponenten aktiviert. Die Kanten werden also vor dem Verbund bearbeitet. Wenn zusätzlich ein Logo angebracht werden soll, so wird dies am Hauptprodukt ausgeführt, also an der VSG-Scheibe.
Die Zuweisung kann in der Auftragserfassung überschrieben werden.
Siehe dazu auch die Einstellungen für die Übernahme bei Austauschgläsern in den Firmendaten.
⇨ "Prod.-Stkl.-Auflösung bei Austausch beibehalten" auf Seite B-955

**Stücklistenartikel**
Die Felder in diesem Bereich werden freigeschaltet, wenn in der Übersicht zur Stückliste eine Komponente markiert ist. Die Felder bleiben gesperrt, wenn Sie die oberste Ebene (Hauptprodukt) markieren.

*   **Artikelnummer, Bezeichnung**: Jede Komponente einer Stückliste ist als Produkt mit einer eigenen Produktnummer und Bezeichnung angelegt.
*   **Menge/Breite/Höhe**: Die Menge bezieht sich auf Artikel, z. B. 3 Beschläge mitliefern. In den Feldern **Breite** und **Höhe** steht standardmäßig eine Null. Sie können die Maße z. B. bei Standard-Türen (ESG) angeben. Diese Maße können im Auftrag überschrieben werden.
*   **Abw. WGR, WGR-Statistik**: Die Warengruppe einer Stücklisten-Komponente kann von der der Hauptposition abweichen. Sie können dann z. B. eine Kombinationswarengruppe auswählen, um Komponenten gemeinsam auszuwerten.
    ⇨ Tutorial 1, "Kombi-WGR" auf Seite B-145
*   **Strukturebene, Strukturverlauf, Beschichtungsseite**: Die Angaben gelten jeweils für die markierte Stücklisten-Komponente. Diese Felder sind zum Register **Fertigung** beschrieben.
    ⇨ “Produktverwaltung - Fertigung" auf Seite B-605
*   **Lieferant, Name**: Die Stücklisten-Komponente wird standardmäßig bei dem eingetragenen Lieferanten bestellt. Die Einstellung kann im Auftrag, in der Position und im Bestellpool geändert werden.
    *   "Lieferantenkartei" auf Seite B-866
    *   Einkauf, "Bestellungen" auf Seite D-43
*   **Beschaffungsart**: Die Angabe gilt für die markierte Stücklisten-Komponente. Die Beschaffungsart ist zum Register **Lager/Einkauf** beschrieben.
    ⇨ "Produktverwaltung – Lager/Einkauf" auf Seite B-617
*   **Preisrelevant VK, Preisrelevant EK**: Die Angaben gelten jeweils für die markierte Stücklisten-Komponente. Diese beiden Checkboxen sind zum Register **Preis/Zuschlag** beschrieben.
    ⇨ "Produktverwaltung - Preis/Zuschlag" auf Seite B-611
*   **Wird gedruckt**: Sie können für jede Komponente festlegen, ob sie im Formulardruck in der Stückliste aufgeführt werden soll.
    *   ☐ Die Komponente nicht wird in der Stückliste auf dem Formular gedruckt.
    *   ☑ Die Komponente wird in der Stückliste auf dem Formular gedruckt.
    ⇨ Tutorial 2, "Formularverwaltung" auf Seite B-480
*   **Gruppe für Stücklistenaustausch**: Auswahl der gültigen Austauschgruppe. Mit der Auswahl legen Sie fest, dass nur die Produkte eingebaut werden können, die der angegeben Austauschgruppe zugeordnet sind. Wenn keine Austauschgruppe angegeben ist, können alle Produkte ausgetauscht werden.
    ⇨ "Austauschzuordnung" auf Seite B-594

##### Produktverwaltung – Texte

**Stammdaten > Produkte > Artikel > Artikel > Register Texte**

In diesem Register ordnen Sie einen Text zu, der im Auftrag angezeigt werden kann. Ein Rahmentext kann an die Produktion übergeben werden.
⇨Tutorial 2, "Textarten" auf Seite B-469
⇨ "Texte" auf Seite B-1059

Die Felder im Bereich **Artikel** sind zum Register **Produkt** beschrieben.
⇨ "Produktverwaltung - Produkt" auf Seite B-600

**Standardtexte**
Der zugewiesene Standardtext muss ein produktbezogener Text sein. Dieser wird auf dem Formular nur im Positionsbereich im Zusammenhang mit dem betreffenden Produkt gedruckt. In der Positionserfassung wird im Zeilenkopf der Positionsanzeige ein Symbol für einen zugeordneten Text angezeigt.
Über das Textkennzeichen wird gesteuert, in welchen Dokumenten/Formularen der Text gedruckt wird.
⇨Tutorial 2, "Textkennzeichen und Standardtexte" auf Seite B-471
⇨ "Textkennzeichen" auf Seite B-1058

**Rahmentext**
Rahmentexte werden in die Abstandhalter (SZR, Rahmen) der Isolierglasscheiben gedruckt. Der Text muss in Dialog **Texte** angelegt sein.
⇨Tutorial 2, "Rahmentexte" auf Seite B-470
⇨ "Texte" auf Seite B-1059
Es ist möglich, für jede ISO-Einheit einen speziellen Rahmentext zu hinterlegen. Die Textnummer kann frei vergeben werden.

##### Produktverwaltung – Sprachen

**Stammdaten > Produkte > Artikel > Artikel > Register Sprachen**

In diesem Register tragen Sie für jedes Produkt die entsprechende fremdsprachliche Bezeichnung ein, wenn Sie mit dem Modul Mehrsprachigkeit arbeiten. Die entsprechende Bezeichnung wird über das Sprachkennzeichen des Kunden ausgewählt und im Formular gedruckt.
⇨ "Partnerverwaltung - Adresse" auf Seite B-771

##### Produktverwaltung – A+W Production

**Stammdaten > Produkte > Artikel > Artikel > Register A+W Production**

In diesem Register definieren Sie die Stammdaten, die an die Produktion übergeben werden können. Dieses Register ist nur freigeschaltet, wenn Sie mit A+W Production arbeiten und in den Firmendaten die zugehörige Verbindung eingerichtet haben. Über den Stammdatenabgleich werden die Daten aus diesem Register an A+W Production übertragen.

> **Info: A+W Production-Daten ändern**
> Die Stammdaten werden bei der Installation von A+W Business eingerichtet und an A+W Production übertragen. Setzen Sie sich mit Ihrem Service-Mitarbeiter der A+W Software GmbH in Verbindung, wenn Sie nachträglich Werte ändern müssen.

