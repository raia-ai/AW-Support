---
title: "D-HB-AWBusiness_7"
source: "D-HB-AWBusiness_7.pdf"
tags: ["A+W Business", "Stammdaten", "Software Manual", "Technical Documentation", "Glass Industry", "ERP", "Configuration", "Cost Calculation", "Price Calculation", "iTOE"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a technical manual and tutorial for the A+W Business software, focusing on supplementary information and master data management. It covers topics such as change monitoring, data transfer between A+W Business and A+W Production, various costing and pricing methods, and provides detailed application examples for the iTOE module for importing DXF files."
long_description: "This document serves as a comprehensive guide, specifically 'Tutorial 2' and a software reference for the A+W Business ERP system, tailored for the glass, windows, and doors industry. The first part provides supplementary information and tutorials on advanced master data configurations. Key topics include defining variables for frame texts, an overview of standard leaded glass construction types, and a detailed explanation of the change monitoring system for tracking modifications in customer, supplier, price, and discount data. It outlines the process for transferring master data to the A+W Production system, ensuring data consistency across both platforms, with detailed field mapping tables. The manual delves into various calculation methods, including mixed costing (Mischkalkulation), French pricing for insulating glass, and a comprehensive cost-plus calculation (Kosten- und Aufschlagskalkulation) framework. It explains how to set contribution margin limits and provides a complex example of cost calculation for an insulating glass unit. The second part, 'Anwendungsbeispiele iTOE', offers practical, step-by-step examples for using the iTOE (intelligent T.O.E.) module to import DXF files. These examples cover various scenarios, such as model recognition, importing custom shapes, handling rotated models, processing cutouts (like speaker holes), and managing edge qualities. It clarifies how rules and priorities within the system affect the final imported product data. The final, extensive part of the document is a 'Softwarereferenz' (Software Reference), which acts as a detailed index and guide to the master data ('Stammdaten') structure within A+W Business. It systematically describes the dialogs, fields, and settings across all major modules, including Products, Pricing, Warehouse, Market Partners, Production, Order Processing, and Finance, providing a foundational resource for system configuration and administration."
---

# Tutorial 2: Zusatzinformationen

---
## Variablen für Rahmentexte

| Variable | Bedeutung |
| :--- | :--- |
| `<kp>` | Kundenposition |
| `<no>` | Auftragsnummer/Position |
| `<p1>` | Produktbezeichnung 1 |
| `<p2>` | Scheibenaufbau |
| `<pd>` | Produktionsdatum |
| `<pn>` | Produktnummer |
| `<po>` | Positionsnummer mit führenden Nullen, 3-stellig |
| `<ps>` | Positionsnummer, ohne führende Null oder Leerzeichen |
| `<sn>` | Schlüsselnummer |
| `<vs>` | VSG Bezeichnung |
| `<vsg>` | VSG Kurzbezeichnung |
| `<wh>` | Maße der Position |
| `<kk>` | Bestellübergabe: Kundenkommission |

*Tab. B-29 Variablen für Rahmentexte*

### Beispiel

**Eingabe:** `<c1> <p1> <p2> <wh> <no>`
**Ausgabe:** John+Partner Standard ISO FL4/18/ORN528 540x1030 109384/001

---
*A+W Business Stammdaten*
*B-601*
---

# Zusatzinformationen

## Konstruktionstypen Bleiverglasung

Für die Verarbeitung von Bleiverglasungen sind folgende Konstruktionstypen standardmäßig hinterlegt:

- **Typ 1**: Gothic
- **Typ 2**: Stuart
- **Typ 3**: Diamonds
- **Typ 4**: Cumberland
- **Typ 5**: Hanover
- **Typ 6**: Jacobean
- **Typ 7**: Northumberland
- **Typ 8**: Queen Anne
- **Typ 9**: Queen Caroline
- **Typ 10**: Rectangles
- **Typ 11**: Square Gothic
- **Typ 12**: Diamond Pillar
- **Typ 13**: Westmorland
- **Typ 14**: Windsor

*Abb. B-334 Konstruktionstyp Bleiverglasung*

---
*A+W Business Stammdaten*
*B-602*
---

# Änderungsüberwachung

Änderungen in der Kunden-, Lieferanten-, Preis- und Rabattverwaltung können überwacht werden. Dazu steht in den entsprechenden Dialogen das Menü **Historie** zur Verfügung.

Für alle Datenbank-Tabellen, auf die ein Dialog zugreift, kann festgelegt werden, wie Änderungen überwacht werden sollen. Eine sehr detaillierte Überwachung wird möglich, wenn die betreffenden Tabellen auf der Ebene der Felder überwacht werden.

Die Änderungsüberwachung wird für jeden der genannten Dialoge getrennt eingestellt und aktiviert. In Allgemeinen werden in der Auswertung die Änderungen des aktuell ausgewählten Datensatzes angezeigt. Daneben kann die Auswertung aber auch nach Nummernverwaltern oder für alle Datensätze angezeigt werden.

Sowohl die Einstellungen als auch die Auswertungen beziehen sich immer auf den gerade eingestellten Laufzeit-Modus. Zum Beispiel betrifft das in der Preisverwaltung die Auswertung von Änderungen der Standardpreise, der Kundenpreise, der Kundengruppenpreise usw.

Daneben können die Auswertungen zusätzlich durch verschiedene Filter eingeschränkt werden, z. B. auf einen bestimmten Mitarbeiter oder einen Zeitraum.

### Änderungsüberwachung Verwaltung

**Utilities > System > Änderungsüberwachung Verwaltung**

*(Abbildung B-335 zeigt das Fenster "Änderungsüberwachung Verwaltung". Es hat die Reiter "Allgemeine Einstellungen", "Tabelleneinstellungen", und "Feldeinstellungen". Unter Tabelleneinstellungen sind verschiedene Tabellen wie "Kundenrabatt nach Warengruppe" gelistet, bei denen der Historie-Modus ("keine", "detailliert") eingestellt werden kann. Unter Feldeinstellungen kann für einzelne Felder die Überwachung an- oder ausgeschaltet werden.)*

---
*A+W Business Stammdaten*
*B-603*
---

In diesem Dialog legen Sie fest, welche Änderungen überwacht und dokumentiert werden sollen.

Diese Funktion ist nur freigeschaltet, wenn Sie die entsprechenden Lizenzen erworben haben.

### Menü Initialisierung

Über den Eintrag **Auswertung initialisieren** wird die Auswertung vorbereitet. Danach kann sie über das Menü **Historie > Auswertung** angezeigt oder gedruckt werden.

### Allgemeine Einstellungen

**Sprache**: Sprache, in der die Auswertungen ausgegeben werden.

**Trigger erstellen**: Die Schaltfläche ist nur freigeschaltet, wenn:
- eine Änderungsüberwachung initialisiert wurde.
- die Einstellung für eine Tabelle oder ein Feld bearbeitet wurde.

> **i**
> Die Datenbank-Trigger für die Überwachung müssen neu gebildet werden, wenn die Einstellungen neu festgelegt oder geändert wurden. Dies kann manuell gestartet werden (empfohlen). Es erfolgt automatisch beim Beenden des Dialogs. Dieser Vorgang kann einige Zeit in Anspruch nehmen.

### Tabelleneinstellungen

> **Übergreifende Einstellungen**
> Wenn Sie die Einstellungen zur Überwachung von Änderungen über den Programmbereich **Utilities > System > Änderungsüberwachung Verwaltung** festlegen, gelten sie für alle verfügbaren Tabellen. Sie können die Einstellungen aber auch für den aktuellen Dialog festlegen.

**Name**: Bezeichnung der Tabelle. Sie kann geändert werden. Die Bezeichnungen werden in der Auswertung angezeigt.

Wenn die Überwachung aktiviert ist, werden alle Felder dieser Tabelle im Bereich **Feldbeschreibungen** angezeigt.

**Historie**: In den Komboboxen der Spalte **Historie** stehen folgende Einstellungen zur Wahl:
- **Keine**: Die Änderungen werden nicht überwacht. Mit dieser Einstellung kann keine Auswertung angezeigt werden.
- **Komplett**: Die Änderungen werden für die gesamte Datenbank-Tabelle überwacht. In der Preisverwaltung müssen Sie diese Einstellung für alle Preistabellen wählen, wenn Sie sich auch alte Stände anzeigen lassen möchten.
- **Detailliert**: Die Änderungen werden auch auf Feldebene überwacht.

---
*A+W Business Stammdaten*
*B-604*
---

## Feldeinstellungen

Wenn die Tabelle auf Feldebene überwacht wird, kann eingestellt werden, welche Felder eine Überwachung auslösen.

**Name**: Bezeichnung des Feldes. Sie kann geändert werden. Die Bezeichnungen werden in der Auswertung angezeigt.

**Referenziert auf**: Zum Identifizieren von Änderungen werden die Schlüsselspalten der jeweiligen Tabelle herangezogen. Handelt es sich bei den Schlüsselfeldern um referenzierende Felder, so wird in dieser Spalte die referenzierte Tabelle angegeben.

**Anzeigespalte**: In einer Tabelle, auf die verwiesen wird, kann neben dem Schlüsselwert auch eine Bezeichnung angezeigt werden. Die möglichen Bezeichnungen können aus der Kombobox in dieser Spalte ausgewählt werden. Z. B. verweist das Feld **Preisschlüssel** auf die Datenbank-Tabelle **Preisschlüssel**. Aus dieser Tabelle kann die Preisschlüsselnummer oder die Bezeichnung angezeigt werden.
Wenn neben dem Schlüsselwert keine Bezeichnungen zur Verfügung stehen, ist die Kombobox leer.

**An/aus**: Diese Spalte und die Checkboxen werden nur angezeigt, wenn in den Tabelleneinstellungen in der Spalte **Historie** der Wert **detailliert** ausgewählt ist. In der Auswertung werden nur die Felder angezeigt, die über diese Checkboxen aktiviert sind. Sie können höchstens 80 Felder anzeigen lassen.

**Auswahl**: Über die beiden Schaltflächen zur Auswahl können alle Checkboxen in der Spalte **an/aus** aktiviert oder deaktiviert werden. Die Checkboxen können danach einzeln aktiviert oder deaktiviert werden.

---
*A+W Business Stammdaten*
*B-605*
---

# A+W Production

Produktionsrelevante Daten können an A+W Production übergeben werden. A+W Production verwendet die gleichen Stammdaten wie A+W Business. Änderungen in den Stammdaten müssen an A+W Production übergeben werden. Über die Produktnummer ist sichergestellt, dass beide Programme das gleiche Produkt verwenden. In jedem Produkt wird in A+W Business ein Kennzeichen zur Bearbeitung gesetzt. Dieses erzeugt die sogenannten Produktionsstücklisten für die Übergabe.

## Übergabedatei

Für die Übergabe wird eine ASCII-Datei in das Verzeichnis **AWPOOL** geschrieben. Für diese legen Sie fest, welche Parameter übergeben werden sollen.

**Beispiel**
- Kundenspezifische Logo-Nummer
- Relevante Textkennzeichen
- Kantenschutz pro Auftrag (Aluband, nur ISO)
- Abstandhalter (über den Fremdschlüssel aus der Produktdefinition)
- Kennzeichen für das Gas

## Stammdatentransfer von A+W Business an A+W Production

Wenn das Zusatz-Modul **Stammdatentransfer** installiert ist, können folgende Daten übertragen werden. Ohne das Modul müssen die Daten in beiden Programmen identisch angelegt werden.

**Tab. B-30 Übergabe der Stammdaten aus A+W Business an A+W Production**

| Dialog in A+W Business | Feld | Dialog in A+W Production | Feld |
| :--- | :--- | :--- | :--- |
| **Produktverwaltung** | | | |
| Register Produkt: | Bezeichnung (1 – 3) | Artikelstammdaten: | Bezeichnung |
| | | | Artikeltext (1 – 2) |
| | bei Produktarten: <ul><li>HW</li><li>TVG</li><li>ESG</li><li>ISO</li><li>VSG</li><li>GH</li></ul> | | Checkbox Freigabeteil aktiv |
| | Sprossendicke | | Dicke |

---
*A+W Business Stammdaten*
*B-606*
---

| Dialog in A+W Business | Feld | Dialog in A+W Production | Feld |
| :--- | :--- | :--- | :--- |
| Bei Bearbeitungen | Produktgruppe | Bearbeitungsartikel: | Klasse |
| | Mengeneinheit | | Dauer s/ |
| Kurzinfo und Produktinfo werden nicht übergeben | | | |
| Die Schleifgruppe wird aus A+W Production übernommen | | | |
| Register Fertigung: | Struktur - Verlauf | Glasarten: | Struktur |
| Register Lager/Einkauf: | Beschaffungsart | Artikelstammdaten: | Beschaffungsart |
| | Automatischer Zuschnitt | Glasartikel: | Optimierbar |
| | Technische Artikelnummer | | Artikelcode |
| Register A+W Production: | Glasart | Artikelstammdaten: | Glasart |
| | Schleifgruppe | | Schleifgruppe |
| | Modell | Glasartikel: | Modellbruchrand |
| | Bruchrander (o, u, r, l) | | Bruchrander |
| | Max. Traverenbreite | | Max. Traverenbreite |
| | Min. Abst. X-Z Schnitte | | Mindestabstand X-Z |
| | Reihenf. Opti. | | Opti-Rang |
| | Strukturlage | | Strukturlage |
| | Beschichtungslage | | Schichtlage |
| Die Übergangszeit wird nicht übergeben (Feld leer lassen) | | | |
| **Glasarten** | | | |
| Glasarten | Bezeichnung | Glasarten: | Bezeichnung |
| | Produktgruppe | | Artikeltyp |
| | Glasartgruppe | | Glasartgruppe |
| | Struktur | | Struktur |
| | Beschichtung | | Beschichtung |
| Glasart-Jumbos | Produktgruppe | Artikelstammdaten: | Artikeltyp |
| | Bezeichnung | | Bezeichnung |
| | Breite / Höhe Jumbo | Lagermaße: | Breite / Höhe |
| | Priorität für Opti. | | Preis |
| | Traverenflag: <ul><li>X-Richtung</li><li>Y-Richtung</li><li>wahlweise</li></ul> | | Traveren |

*Tab. B-30 Übergabe der Stammdaten aus A+W Business an A+W Production*

---
*A+W Business Stammdaten*
*B-607*
---

| Dialog in A+W Business | Feld | Dialog in A+W Production | Feld |
| :--- | :--- | :--- | :--- |
| Jumbo-Zuschneidetische | Auflegercode | Lagermaße: | Auflegercode |
| | Anzahl | | Anzahl |
| **Zuschneidetische** | | | |
| Register Werte: | Bezeichnung | Tische: | Beschreibung |
| | Breite / Höhe | | Breite / Höhe |
| | Referenzpunkt | | Referenz |
| | Z-Schnitt | | Z-Schnitt |
| | Brechbeginn | | Brechbeginn |
| | Böcke per Zyklus | | Böcke / Zyklus |
| | Spezial | | Spezial |
| | Rang | | Rang |
| Register Einstellungen: | Autobrechen | Tische: | Autobrechen |
| | Autoaufleger | | Autoaufleger |
| | Formen | | Formen |
| | VSG | | VSG |
| | Entschichten | | Entschichten |
| | Handzuschnitt | | Handzuschnitt |
| | max. Traverenbreite darf | | maximale Traverenbreite |
| Register Schnitte: | Min. Abst. Y-Y Schnitte | Tische: | Min X-X |
| | Min. Abst. X-X Schnitte | | Max X-X |
| | Max. Abst. Y-Y Schnitte | | Min Y-Y |
| | Max. Abst. X-X Schnitte | | |
| Die Werte zum maximalen Verschnitt werden nicht übergeben. | | | |

*Tab. B-30 Übergabe der Stammdaten aus A+W Business an A+W Production*

## Bearbeitungskatalog

Der hinterlegte Bearbeitungskatalog enthält alle Bearbeitungstypen und die erforderlichen Parameter. Er dient als zentrales Bindeglied zwischen den bestehenden Programmen der A+W Software GmbH.

Damit können aus A+W Business die Bearbeitungen inklusive aller dazugehöriger Daten an A+W Production oder per OrderXML übergeben werden.

Um immer wiederkehrende komplizierte Kombinationen von Bearbeitungen schnell erfassen zu können, kann zusätzlich ein von Shaping & Nesting generiertes Bearbeitungsmakro angehängt werden.

---
*A+W Business Stammdaten*
*B-608*
---

### Ergänzende Informationen
⇨ Softwarereferenz, "Produktverwaltung - A+W Production" auf Seite B-737
⇨ Softwarereferenz, "Firmendaten - Produktion" auf Seite B-1126
⇨ Verkauf, "Parameter" auf Seite C-1745

## Mischkalkulation

Für die Preisberechnung von kundenspezifischen Preisen kann statt eines Austauschzuschlages die sogenannte Mischkalkulation angewendet werden. Diese Art der Kalkulation wird in Österreich verwendet.

Dazu werden bis zu drei Produkte herangezogen, bei deren Kombination ein gemischter Preis kalkuliert werden soll. Für die Kalkulation wird angegeben, auf welche (kundenspezifische) Preistabelle dabei zurückgegriffen werden soll.

Die Berechnungsfaktoren für die Mischkalkulation werden in den Firmendaten hinterlegt. Außerdem wird dort festgelegt, ob eine Rabatt- und/oder Individualpreissuche bei der ISO-Mischkalkulation möglich sein soll.

Standardmäßig ist die Suche nach Individualpreisen und nach Rabatten bei der Mischkalkulation ausgeschaltet.

**Beispiel**
- Basispreis 2-fach Isolierglas = 50 % ISO-Preistabelle 1 + 50 % ISO-Preistabelle 2.
- Basispreis 3-fach Isolierglas = 50 % ISO-Preistab. 1 + 80 % ISO-Preistab. 2 + 50 % ISO-Preistab. 3.

Für die erste Scheibe der ISO-Einheit wird der Preis für aus der ISO-Preistabelle 1 und für die zweite Scheibe der ISO-Einheit der Preis aus der ISO-Preistabelle 2 genommen. Bei einem 3-fach Isolierglas wird für die dritte Scheibe der ISO-Einheit der Preis aus der ISO-Preistabelle 3 genommen.

### Ergänzende Informationen
⇨ Softwarereferenz, "Mischkalkulation" auf Seite B-820
⇨ Softwarereferenz, "Mischkalkulationsfaktoren" auf Seite B-1068
⇨ Softwarereferenz, "Rabattsuche bei ISO-Mischkalkulation" auf Seite B-1087
⇨ Softwarereferenz, "Individualpreissuche bei ISO-Mischkalkulation" auf Seite B-1087

---
*A+W Business Stammdaten*
*B-609*
---

# Französische Preisberechnung

Bei der sog. französischen Preisberechnung von ISO setzt sich der Preis für das ISO aus folgenden Komponenten zusammen:
- Basispreis für den Zusammenbau des ISO
- Einzelpreise für die Gläser

Dafür werden in der Regel eigene Schlüssel und Tarife definiert. Die Preise für die jeweiligen Einzelgläser werden in der gewohnten Form definiert. Sie müssen im selben Preisschlüssel liegt wie der ISO-Basispreis. Für das ISO muss die Preiseinheit `<qm+EP>` gewählt werden.

Die Produkte werden in der üblichen Form angelegt. Für die Abstandhalter wird ein Sonstiger Zuschlag angelegt und dem ISO-Preis zugeordnet.

> **i ISO und VSG**
> Bei der frz. Preisberechnung darf in den Firmendaten die Option **Iso und VSG-Einzelpreisberechnung** nicht aktiviert werden.
> ⇨ Softwarereferenz, "ISO + VSG Einzelpreisberechnung" auf Seite B-1088

---
*A+W Business Stammdaten*
*B-610*
---

# Kalkulation

### Lernziele
- Komponenten der Kostenkalkulation.
- Vorgaben für die Eigenkosten-Kalkulation festlegen.
- Kalkulation des Deckungsbeitrags festlegen.

### Nutzen
- Die Höhe der Eigenkosten wird übergreifend eingestellt und in die Kalkulationen des Deckungsbeitrags und der Einkaufspreise einbezogen.
- Der Deckungsbeitrag wird automatisch neu berechnet, wenn im Dokument die Preise bei der Erfassung von Positionen geändert werden.

### Merke

| Begriff | Erklärung |
| :--- | :--- |
| **Herstellkosten** | Die Herstellkosten setzen sich zusammen aus: Material-, Maschinen- und Personalkosten zuzüglich Gemeinkosten. |
| **Gemeinkosten** | Die prozentualen Anteile für die Gemeinkosten legen Sie in den Firmendaten fest. |
| **Kalkulation** | Die Kostenkalkulation wird pro Tarif (Preisjahrgang und -schlüssel) aktiviert: <ul><li>Wenn die Kalkulation in den Tarifen nur für die EK-Preisberechnung aktiviert ist, wird die Kosten- und Aufschlagskalkulation nur bis zum Selbstkostenpreis durchgeführt.</li><li>Wenn auch in den VK-Tarifen die Kalkulation aktiviert ist, geht die Kalkulation weiter bis zum Verkaufspreis.</li></ul> |
| **Teilmaterialkosten** | Die Teilmaterialkosten errechnen sich aus der Menge (inkl. produktbezogenem Verschnitt) und dem Preis pro Mengeneinheit. |
| **Vollmaterialkosten** | Auf die Teilmaterialkosten wird ein Gemeinkostenzuschlag berechnet, der die Beschaffungsart des Produkts berücksichtigt. |
| **Deckungsbeitrag** | Für die Ermittlung des Deckungsbeitrags werden Mindest- und Höchstwerte pro Kunde und Warengruppe gepflegt. Die aktuellen Deckungsbeiträge werden pro Dokument ermittelt und angezeigt. Die Deckungsbeitrags-Analyse ermittelt die Deckungsbeiträge über einen beliebigen Zeitraum. |

---
*A+W Business Stammdaten*
*B-611*
---

## Deckungsbeitrags-Grenzwerte

Deckungsbeiträge werden im Auftrag direkt angezeigt und beziehen sich nur auf die im Auftrag enthaltenen Positionen.

*(Abbildung B-336 zeigt eine Maske im Programm, die den aktuellen Deckungsbeitrag im Auftrag und pro Position darstellt. Felder umfassen Materialkosten, Zeitkosten, Frachtkosten, Gesamtkosten und den jeweiligen Deckungsbeitrag (DB) in absoluten Zahlen und Prozent.)*

Mit Hilfe der Deckungsbeitrags-Analyse kann der Deckungsbeitrag von Auftragspositionen über einen beliebigen Zeitraum untersucht und gedruckt werden. Diese Auswertung wird im Modul **Dokumente** gestartet.

*(Abbildung B-337 zeigt die "Deckungsbeitrags-Analyse" in einer tabellarischen Übersicht. Spalten enthalten Auftragsnummer, Position, Kunde, Produkt, Warengruppe (WGR), Deckungsbeitrag in Prozent (DB%), minimale und maximale DB-Grenzwerte, Positionspreis und EK-Preis.)*

Die minimalen und maximalen Deckungsbeiträge werden im Dialog **Deckungsbeitrags-Grenzen** pro Kunde und Warengruppe gepflegt.

---
*A+W Business Stammdaten*
*B-612*
---

*(Abbildung B-338 zeigt den Dialog "Deckungsbeitrags-Grenzen". Hier können Grenzwerte für den Deckungsbeitrag festgelegt werden. Die relevanten Eingabefelder sind: A) Auswahl Kunde oder Kundengruppe, B) Auswahl Warengruppe, C) Angabe der Grenzwerte (minimaler und maximaler Deckungsbeitrag in Prozent).)*

Die Grenzwerte legen Sie pro Kunde oder Kundengruppe (A) fest. Die Analyse bezieht sich jeweils auf eine Warengruppe (B), wobei Sie alle drei Ebenen (WGR, WOG, WHG) wählen können.

Für jede Kombination von (A) und (B) können Sie prozentualen Werte (C) für die Deckungsobergrenze und die Deckungsuntergrenze festlegen. Damit können Sie z. B. leichter prüfen, ob der Deckungsbeitrag für den Kunden oder die Kundengruppe im gewünschten Rahmen liegt.

Da jede Kalkulation von Preisen im einzelnen Auftrag überschrieben werden kann, können ein Höchst- und ein Mindestbetrag für Deckungsbeiträge hinterlegt werden. Damit werden grobe Fehlkalkulationen bei der manuellen Preisgestaltung im Auftrag verhindert, z. B. ein Verkaufspreis unter den Selbstkosten.

---
*A+W Business Stammdaten*
*B-613*
---

*(Abbildung B-339 zeigt einen Ausschnitt aus den Firmendaten, Register "Kalkulation". Hier werden Standardwerte für den Deckungsbeitrag festgelegt. A markiert den "Mindestbeitrag für Deckungsbeiträge" und B den "Höchstbeitrag für Deckungsbeiträge".)*

Für alle nicht explizit definierten Kombinationen von Kunden und WGR gelten die Standardwerte, die in den Firmendaten im Register **Kalkulation** festgelegt sind.

---
*A+W Business Stammdaten*
*B-614*
---

## Kosten- und Aufschlagskalkulation

Mit der Kosten-/Aufschlagskalkulation wird der Preis pro Preiseinheit ermittelt. Dazu werden die Anteile der Selbstkosten aus den Firmendaten berücksichtigt.

### Herstellungskosten

Auf der Basis von Material-, Maschinen- und Personalkosten werden Herstellkosten ermittelt. Zuzüglich der Gemeinkostenzuschläge für Material und Sondereinzelkosten ergeben sich daraus die Vollherstellkosten.

Zu den Materialgemeinkosten zählen die Beschaffungsarten:
- Bestellung
- Lagerentnahme
- Produktion

Auf diese werden Gemeinkosten für Verwaltung und Vertrieb aufgeschlagen. Zuzüglich einer prozentualen Gewinnerwartung ergibt sich daraus der Verkaufspreis.

Zu den Gemeinkosten zählen:
- **Lohnnebenkosten**: z. B. Kosten für Sozialversicherungen.
- **Vertriebsgemeinkosten**: Kosten, die den Produkten nicht im Einzelnen zugeordnet werden können, z. B. Provisionen.
- **Verwaltungsgemeinkosten**: z. B. Kosten für Büro, Energie, Verwaltungsmitarbeiter usw.
- **Gewinnspanne**

Die prozentualen Anteile für die Gemeinkosten legen Sie in den Firmendaten fest.

---
*A+W Business Stammdaten*
*B-615*
---

*(Abbildung B-340 zeigt die Firmendaten zur Kostenkalkulation. A markiert die prozentualen Zuschläge für die Materialkosten je nach Beschaffungsart. B markiert die prozentualen Zuschläge für Gemeinkosten wie Lohnnebenkosten, Vertriebs- und Verwaltungsgemeinkosten sowie die Gewinnspanne.)*

Diese prozentualen Aufschläge (A, B) beziehen sich auf die Einkaufspreise (netto).

Die Kostenkalkulation wird pro Tarif (Preisjahrgang und -schlüssel) aktiviert.

*(Abbildung B-341 zeigt die Tarifzuordnung. Hier kann pro Tarif die Kostenkalkulation für EK-Tarife (A) und VK-Tarife (B) aktiviert werden.)*

---
*A+W Business Stammdaten*
*B-616*
---

Wenn die Kalkulation in den Tarifen nur für die EK-Preisberechnung aktiviert ist, wird die Kosten- und Aufschlagskalkulation nur bis zum Selbstkostenpreis durchgeführt. Wenn auch in den VK-Tarifen die Kalkulation aktiviert ist, geht die Kalkulation weiter bis zum Verkaufspreis.

Im Dokument und in den Positionen können Sie sich die Kalkulationen für den aktuellen Auftrag anzeigen lassen.

*(Abbildung B-342 zeigt zwei Übersichten zur Kalkulation. A zeigt die Kalkulation für eine Position, B zeigt die detaillierte Kalkulation für die Stücklisten-Komponenten dieser Position.)*

In diesen Beispielen sehen Sie die Kalkulation für eine Position (A). In der Positionserfassung kann die Kalkulation für die Stückliste (B) geprüft werden. Preise, die implizit in einem Produkt enthalten sind, werden dabei nicht angezeigt.

Die Kalkulation kann pro Position angepasst werden, z. B. um bestimmte Nebenkosten mit einem abweichenden Prozentsatz zu kalkulieren oder um Sonderkosten zu berücksichtigen.

---
*A+W Business Stammdaten*
*B-617*
---

*(Abbildung B-343 zeigt die Detailansicht der Kostenkalkulation für eine Position. Hier können Gemeinkosten und Sonderzuschläge (A), die Gewinnerwartung (B) angepasst und Sonderkosten (C) eingegeben werden.)*

Die Kostenkalkulation kann pro Position auch um Sonderzuschläge erweitert werden. Wenn diese Zuschläge als negativer Wert angegeben werden, entspricht das einem Sonderrabatt für diese eine Position.

> **i Maschinen- und Personalkosten aus der Produktion**
> Die Anteile aus Maschinen- und Personalkosten werden über die zugehörigen Basisdaten aus der Kapazitätsplanung errechnet. Diese Kostenfaktoren stehen daher nur zur Verfügung, wenn die A+W Business-Kapazitätsplanung freigeschaltet ist und wenn Rückmeldungen zu den tatsächlichen Kosten aus der Produktion vorliegen.

---
*A+W Business Stammdaten*
*B-618*
---

## Kalkulation der Eigenkosten festlegen

Für die Kalkulation der Eigenkosten für Isolierglas legen Sie pro Abstandhalter den durchschnittlichen Verbrauch von Hilfsstoffen wie Butyl, Thiokol usw. fest. Ein ausführliches Beispiel finden Sie in einer separaten Einheit.
⇨ "Komplexbeispiel: Kalkulation ISO" auf Seite B-621

> **i Voraussetzung**
> Die Verbrauchsartikel, die im Bereich Stücklistenprodukt eingetragen werden sollen, müssen als Produkte angelegt sein.

**So legen Sie Vorgaben für die Kalkulation der Eigenkosten fest**

1. Wählen Sie im Menü **Stammdaten > Produkte > Artikel > EK-Kalkulation**.
Der Dialog *Kalkulationsvorgaben* wird geöffnet.
⇨ Softwarereferenz, "EK-Kalkulation" auf Seite B-765

2. Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.

*(Abbildung B-344 zeigt den Dialog "EK-Kalkulation" im Neuanlage-Modus. Die Felder sind: A - Angaben für Abstandhalter (SZR), B - Rückschnitt, C - Gasmenge, D - Angaben für Produkte aus Stückliste.)*

⇨ Softwarereferenz, "EK-Kalkulation" auf Seite B-765

3. Geben Sie die Artikelnummer des Abstandhalters (A) ein, dem der Verbrauch an Gas, Trockenmittel oder Randverbund zugeordnet werden soll.

---
*A+W Business Stammdaten*
*B-619*
---

Detaillierte Beispiele finden Sie in der nachfolgenden Einheit.

4. Tragen Sie die gewünschten Werte in die Felder ein:
    - **Rückschnitt (einfach)** in mm (B)
    - **Entspannte Menge für Gas** in Liter (C)

5. Wechseln Sie zum Register **Stückliste**.

6. Markieren Sie im Bereich **Stückliste** eine Zeile mit der Artikelnummer 0.

7. Tragen Sie im Bereich **Stücklistenprodukt (D)** die Produktnummer, den Verbrauch des Artikels und dessen Bezugseinheit ein.
Die Einträge werden im Bereich **Stückliste** angezeigt.

8. Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
Die Daten werden gespeichert.

> **i Rückschnitt**
> Mit dem **Rückschnitt (einfach)** ist der Abstand von der Glasaußenkante bis zum Alurahmen außen gemeint. Er ist wichtig für den Bieger der Alurahmen.
> Beträgt das Glasmaß z. B. 1000 x 1000 mm, der **Rückschnitt (einfach)** 5 mm, so beträgt das Rahmenmaß 990 x 990 mm.

---
*A+W Business Stammdaten*
*B-620*
---

# Komplexbeispiel: Kalkulation ISO

In diesem Beispiel wird gezeigt, wie die Eigenkalkulation (EK) einer Isolierglas-Einheit bei Eigenfertigung eingerichtet und im Auftrag angezeigt wird.

Die Kalkulation wird in folgenden Einheiten dargestellt:
- Berechnung der Scheiben
- Berechnung des Rahmens
- Berechnung für das Gas
- Berechnung der Verbrauchsmaterialien

Bei der Beispielberechnung wurde auf Rundungen, Rabatte und Zuschläge verzichtet, damit die Kalkulation einfach nachzuvollziehen ist.

## Anzeige in der Positionserfassung

*(Abbildung B-345 zeigt die Positionserfassung in einem Auftrag. Die Stückliste eines Isolierglases wird mit den Einzelkomponenten und deren Preisen angezeigt. Die Ziffern 1 bis 6 verweisen auf die verschiedenen Preis-Komponenten.)*

Die EK-Preise einer Auftragsposition können über das Menü **Ansicht** angezeigt werden. Die im Beispiel angezeigten Werte sind in der folgenden Berechnung enthalten:

| Legende | Produkt | | Preis |
| :--- | :--- | :--- | :--- |
| 1 | 1. Scheibe | + | 8,57 |
| 2 | 2. Scheibe | + | 10,91 |
| 3 | Verbrauchsmaterialien | + | 3,68 |
| 4 | Rahmen | + | 1,60 |
| 5 | Gas | + | 0,12 |
| 6 | **Stückkosten** | **=** | **24,88** |

*Tab. B-31 Berechnung des Einkaufspreises*

Die Kalkulation der Nummern 1 - 5 wird im Folgenden detailliert dargestellt.

---
*A+W Business Stammdaten*
*B-621*
---

## Berechnung der Scheiben

Bei der Berechnung der Scheiben werden der Einkaufpreis aus der zugeordneten Preistabelle, der Verschnitt und die Rundung berücksichtigt. Im gezeigten Beispiel ist keine Rundung der Fläche definiert.

### Erste Scheibe

Der EK-Preis aus der Preistabelle wird mit der Fläche multipliziert. In diesem Beispiel ist die Höhe x Breite = 1 qm. Zum errechneten Wert wird ein Betrag für den Verschnitt addiert.

| | EK |
| :--- | :--- |
| EK | x (Fläche + Verschnitt) |
| 8,24 | x (1 + 4/100) |
| **8,57** | |

*Tab. B-32 EK-Berechnung der ersten Scheibe*

Verschnitt und Preistabelle werden in den Stammdaten festgelegt.

### Verschnitt

In den Produktstammdaten werden im Register **Preis/Zuschlag** die Preistabellen für den VK und den EK zugeordnet und der mittlere Verschnitt definiert.

*(Abbildung B-346 zeigt die Produktstammdaten für "Float 4 mm" im Register "Preis/Zuschlag". Das Feld "Mittlerer Verschnitt" ist auf 4% eingestellt.)*

---
*A+W Business Stammdaten*
*B-622*
---

### Preis

In der Preistabelle wird der Einkaufspreis hinterlegt, den Sie mit Ihrem Lieferanten vereinbart haben.

*(Abbildung B-347 zeigt die Preistabelle für "Float 4 mm". Für den Schlüssel "Festmaße" ist ein Preis von 8,240 pro qm hinterlegt.)*

### Zweite Scheibe

Die Berechnung der zweiten Scheibe basiert ebenfalls auf den Stammdaten. Die Werte können sich von der ersten Scheibe unterscheiden.

| | EK |
| :--- | :--- |
| EK | x (Fläche + Verschnitt) |
| 10,20 | x (1 + 7/100) |
| **10,91** | |

*Tab. B-33 Berechnung der zweiten Scheibe*

Verschnitt und Preis werden so wie bei der ersten Scheibe in den Stammdaten festgelegt.

## Berechnung des Rahmens

In diesem Beispiel beträgt die Kantenlänge genau 1000 mm. Die Gesamtlänge des Rahmens beträgt also 4 m.

| | EK |
| :--- | :--- |
| EK Rahmen | x effektive Lfm |
| 0,40 | x 4 |
| **1,60 \*** | |

\* Nr. 4 der Tabelle "Berechnung des Einkaufspreises" auf Seite B-621

*Tab. B-34 Berechnung des Rahmens*

Der Preis wird ebenfalls als Einzelpreis in den Stammdaten festgelegt.
In der Preistabelle wird der Einkaufspreis pro Preiseinheit hinterlegt, den Sie mit Ihrem Lieferanten vereinbart haben. In diesem Beispiel ist das 0,40/lfm.

---
*A+W Business Stammdaten*
*B-623*
---

## Berechnung für das Gas

Zur Berechnung des Gases wird die hinterlegte Gasmenge mit der Dicke des Scheibenzwischenraums multipliziert.

| m³ | x | SZR/Entspannte Menge Gas | x | EK Gas (1 + Verschnitt/100) | EK |
| :--- | :-: | :--- | :-: | :--- | :--- |
| 1 | x | 12/21000 | x | 215,90/(1 + 0/100)* | **0,12\*\*** |

\* In diesem Beispiel wird ohne Verschnitt für das Gas gerechnet.
\*\* Nr. 5 der Tabelle “Berechnung des Einkaufspreises" auf Seite B-621

*Tab. B-35 Berechnung des Gases*

### Kalkulationsgrundlage

Unter **Stammdaten > Produkte > Artikel > EK Kalkulation** wird die entspannte Menge des Gases (ohne Druck, ohne Kühlung) pro Kubikmeter angegeben.

*(Abbildung B-348 zeigt den Dialog "EK-Kalkulation" für Wärmedämmgas. Das Feld "Entspannte Menge" ist auf 21000,0000 eingestellt.)*

Der Preis wird ebenfalls als Einzelpreis in den Stammdaten festgelegt.
In der Preistabelle wird der Einkaufspreis pro Preiseinheit hinterlegt, den Sie mit Ihrem Lieferanten vereinbart haben.

---
*A+W Business Stammdaten*
*B-624*
---

## Berechnung der Verbrauchsmaterialien

Zusätzlich zu Scheiben, Rahmen und Gasfüllung können Verbrauchsmaterialien angegeben werden, die bei der Produktion der ISO-Einheit benötigt werden.

| | EK |
| :--- | :--- |
| EK Butyl | 2,2 |
| EK Thiokol | + 0,028696 |
| EK Trockenmittel | + 1,4484 |
| | **3,68\*** |

\* Nr. 3 der Tabelle "Berechnung des Einkaufspreises" auf Seite B-621

*Tab. B-36 Berechnung der Verbrauchsmaterialien*

In den folgenden Abschnitten ist dargestellt, wie die drei Einzelbeträge errechnet wurden.

### Berechnung für das Butyl

| EK Butyl | x | tatsächliche Laufmeter | x | Verbrauch pro Einheit | EK |
| :--- | :-: | :--- | :-: | :--- | :--- |
| 100 | x | 4 | x | 0,0055 | **2,20** |

*Tab. B-37 Berechnung des Butyls*

Zur Berechnung des Verbrauchs ist die Menge pro Einheit festgelegt. In diesem Beispiel werden 0,0055 kg pro laufendem Meter (Rahmen) berechnet.
Der Preis wird ebenfalls als Einzelpreis in den Stammdaten festgelegt.
In der Preistabelle wird der Einkaufspreis pro Preiseinheit hinterlegt, den Sie mit Ihrem Lieferanten vereinbart haben.

### Berechnung für das Thiokol

| EK Thiokol | x | effektive Lfm | x | Verbrauch pro Einheit | EK |
| :--- | :-: | :--- | :-: | :--- | :--- |
| 1,17 | x | 4 | x | 0,0422 | **0,028696** |

*Tab. B-38 Berechnung des Thiokols*

Zur Berechnung des Verbrauchs ist die Menge pro Einheit festgelegt. In diesem Beispiel werden 0,0422 Liter pro laufendem Meter (Rahmen) berechnet.
In der Preistabelle wird der Einkaufspreis pro Preiseinheit als Einzelpreis hinterlegt.

---
*A+W Business Stammdaten*
*B-625*
---

### Berechnung der Trockenmittel

| EK Trockenmittel | x | effektive lfm | x | Verbrauch pro Einheit | EK |
| :--- | :-: | :--- | :-: | :--- | :--- |
| 8,50 | x | 4 | x | 0,0426 | **1,4484** |

*Tab. B-39 Berechnung des Trockenmittels*

Zur Berechnung des Verbrauchs ist die Menge pro Einheit festgelegt. In diesem Beispiel werden 0,0426 kg pro laufendem Meter (Rahmen) berechnet.
In der Preistabelle wird der Einkaufspreis pro Preiseinheit als Einzelpreis hinterlegt.

### Ergänzende Informationen
⇨ Tutorial 2, "Kalkulation der Eigenkosten festlegen" auf Seite B-619
⇨ Softwarereferenz, "Einkauf" auf Seite B-1096
⇨ Softwarereferenz, "Firmendaten - Kalkulation" auf Seite B-1120

---
*A+W Business Stammdaten*
*B-626*
---

# B: A+W Business Stammdaten - Anwendungsbeispiele iTOE

---
*(Titelblatt)*
*A+W Software for Glass, Windows & Doors*
*Anwendungsbeispiele iTOE*
---

## In diesem Kapitel finden Sie folgende Themen:
- **Überblick** ... B-629

---
*A+W Business Stammdaten*
*B-628*
---

# Überblick

In diesem Part finden Sie Anwendungsbeispiele für die iTOE in A+W Business.

Dazu gehören folgende Lerneinheiten:
- Modellerkennung ohne iTOE beim Einlesen einer DXF-Datei
- Import eines Modells, das nicht im Modellkatalog enthalten ist ohne iTOE beim Einlesen einer DXF-Datei
- Modellerkennung beim Einlesen einer DXF-Datei mit gedrehtem Modell
- Einlesen einer DXF-Datei mit Durchsprechöffnung
- Wie verhält sich die iTOE beim DXF-Import, wenn man die Kantenqualität bei Bearbeitungen vorgibt
- DXF-Import auf eine Position, die bereits eine Bearbeitung hat
- Auf welcher Stücklistenebene wird eine Bearbeitung importiert, wenn man keine Kantenqualität vorgibt
- Auf welcher Stücklistenebene wird eine Bearbeitung importiert, wenn man eine Kantenqualität vorgibt
- Auf welcher Stücklistenebene wird eine Bearbeitung importiert, wenn man eine Kantenqualität vorgibt (Modell 99)
- Die Prioritäten der Regeln beim Produktabgleich

> **i Voraussetzung**
> Das linzenzpflichtige iTOE-Modul setzt das Datenbanksystem Microsoft SQL Server voraus. Wenden Sie sich an die A+W Software GmbH, wenn Sie das Modul einsetzen wollen.

---
*A+W Business Stammdaten*
*B-629*
---

## Modellerkennung ohne iTOE beim Einlesen einer DXF-Datei

1. Wir erfassen eine Position, hier Float 6 mm.
2. Wir wechseln in die Lasche **3. Modelle/Bearbeitungen**.
3. Im Bereich **Bearbeitung** aktivieren wir die Symbol-Schaltfläche für Modelle.
4. Im Feld **Modell** geben wir die **99** für freie Formen ein.
5. Im Bereich **S+N-Datei** aktivieren wir die Checkbox und klicken am Ende des Feldes auf das Ordner-Symbol.
   
   *(Screenshot der Positionserfassung, die oben genannten Felder sind markiert.)*

6. Es öffnet sich der Dialog **Shaping+Nesting - Datei auswählen**.
7. Wir wählen die gewünschte Datei aus und klicken auf [Öffnen].
8. Es öffnet sich der Dialog **DXF Import** mit einer Vorschau des zu importierenden Modells. Wir klicken auf die Schaltfläche [Modell importieren].

---
*A+W Business Stammdaten*
*B-630*
---

*(Screenshot des DXF Import Dialogs mit der Vorschau einer fünfeckigen Form.)*

9. Handelt es sich bei dem zu importierenden Modell um ein Modell, welches im A+W Modellkatalog enthalten ist (in unserem Beispiel ist das Modell 95) erscheint die Frage **Soll auf das Modell: 95 gewechselt werden?** Wir beantworten die Frage mit [Ja].
   
   *(Screenshot der Bestätigungsabfrage.)*

10. Die DXF-Datei wird importiert und A+W Business gleicht alle Modellparameter entsprechend der DXF-Datei an. Im Feld **Modell** steht jetzt nicht mehr die von uns eingegebene 99 sondern die Nummer 95, auf die gewechselt wurde.

---
*A+W Business Stammdaten*
*B-631*
---

*(Screenshot der Positionserfassung nach dem Import. Das Modell ist jetzt 95, und die Parameter sind ausgefüllt. Die Skizze zeigt das importierte Modell.)*

## Import eines Modells, das nicht im Modellkatalog enthalten ist ohne iTOE beim Einlesen einer DXF-Datei

1. Wir erfassen eine Position, hier Float 6 mm.
2. Wir wechseln in die Lasche **3. Modelle/Bearbeitungen**.
3. Im Bereich **Bearbeitung** aktivieren wir die Symbol-Schaltfläche für Modelle.
4. Im Feld **Modell** geben wir die **99** für freie Formen ein.
5. Im Bereich **S+N-Datei** aktivieren wir die Checkbox und klicken am Ende des Feldes auf das Ordner-Symbol.

*(Screenshot der leeren Modellerfassung.)*

---
*A+W Business Stammdaten*
*B-632*
---

6. Es öffnet sich der Dialog **Shaping+Nesting - Datei auswählen**.
7. Wir wählen die gewünschte Datei aus und klicken auf [Öffnen].
8. Es öffnet sich der Dialog **DXF Import** mit einer Vorschau des zu importierenden Modells. Wir klicken auf die Schaltfläche [Modell importieren].

   *(Screenshot des DXF Import Dialogs mit der Vorschau eines Achtecks.)*

9. Bei diesem zu importierenden Modell handelt es sich nicht um ein Modell, welches im A+W Modellkatalog enthalten ist.
10. Die DXF-Datei wird importiert und A+W Business gleicht alle Modellparameter entsprechend der DXF-Datei an. Im Feld **Modell** bleibt die Modellnummer 99 stehen, mit allen Konsequenzen für die Preisberechnung und auch sonstige Bearbeitungen, die theoretisch in solch einer DXF-Datei enthalten sein könnten.

---
*A+W Business Stammdaten*
*B-633*
---

*(Screenshot der Positionserfassung nach dem Import. Das Modell ist 99 geblieben, die Skizze zeigt das importierte Achteck und die Bemaßungen.)*

## Modellerkennung beim Einlesen einer DXF-Datei mit gedrehtem Modell

1. Wir erfassen eine Position, hier Float 6 mm.
2. Wir wechseln in die Lasche **3. Modelle/Bearbeitungen**.
3. Im Bereich **Bearbeitung** aktivieren wir die Symbol-Schaltfläche für Modelle.
4. Im Feld **Modell** geben wir die **99** für freie Formen ein.
5. Im Bereich **S+N-Datei** aktivieren wir die Checkbox und klicken am Ende des Feldes auf das Ordner-Symbol.
6. Es öffnet sich der Dialog **Shaping+Nesting - Datei auswählen**.
7. Wir wählen die gewünschte Datei aus und klicken auf [Öffnen].
8. Es öffnet sich der Dialog **DXF Import** mit einer Vorschau des zu importierenden Modells. Wir klicken auf die Schaltfläche [Modell importieren].

---
*A+W Business Stammdaten*
*B-634*
---

*(Screenshot des DXF Import Dialogs mit einem gedrehten Modell (Rundbogen).)*

9. Bei diesem Modell handelt es sich um das Modell 74, das um 90 Grad gedreht ist. Da das Modell gedreht ist, erscheint nicht die Abfrage, ob auf das Modell 74 gewechselt werden soll.
10. Die DXF-Datei wird importiert und A+W Business gleicht alle Modellparameter entsprechend der DXF-Datei an. Da es sich um ein gedrehtes Modell handelt, findet kein Wechsel auf das Modell 74 statt.

*(Screenshot der Positionserfassung nach dem Import. Modell 99 ist aktiv, die Skizze zeigt das gedrehte Rundbogen-Modell.)*

---
*A+W Business Stammdaten*
*B-635*
---

> **i Modellrotation**
> Die Modellrotation von Standardmodellen muss beim Einsatz der iTOE grundsätzlich deaktiviert werden, da die Bearbeitungsparametrisierung X/Y Koordinate und Bezugspunkt nicht angepasst werden und somit zu einer Falschberechnung führen.

> **i Lösung für gedrehte Modelle**
> Momentan empfehlen wir als Lösung für gedrehte Modelle, die Drehung in der SN-Datei (Transformieren > Drehen um 90°) vorzunehmen und dort abzuspeichern.

## Einlesen einer DXF-Datei mit Durchsprechöffnung

1. Wir erfassen eine Position, hier VSG, welches aus zwei ESG und einer Folie besteht.
2. Wir wechseln in die Lasche **3. Modelle/Bearbeitungen**.
3. Im Bereich **Bearbeitung** aktivieren wir die Symbol-Schaltfläche für Modelle.
4. Im Feld **Modell** geben wir die **99** für freie Formen ein.
5. Im Bereich **S+N-Datei** aktivieren wir die Checkbox und klicken am Ende des Feldes auf das Ordner-Symbol.
6. Es öffnet sich der Dialog **Shaping+Nesting - Datei auswählen**.
7. Wir wählen die gewünschte Datei aus und klicken auf [Öffnen].
8. Es öffnet sich der Dialog **DXF Import** mit einer Vorschau des zu importierenden Modells. Wir klicken auf die Schaltfläche [Modell importieren].

   *(Screenshot des DXF Import Dialogs mit einer Türform mit einer kreisrunden Öffnung.)*

9. Wir klicken auf die Schaltfläche [Bearbeitung konfigurieren].

---
*A+W Business Stammdaten*
*B-636*
---

10. Der Wert **Grenze** ist der Durchmesser, wann eine Öffnung als Bohrloch erkannt wird. Im Beispiel oben ist der Wert 100. Da das große Bohrloch aber einen Wert von 200 hat, wird es (weil der Grenzwert darunter liegt) nicht als solches erkannt.
11. Im Feld **Kante** befinden sich die verschiedenen Kantenqualitäten, die die Bohrlöcher haben sollen. Wir importieren die Form mit der Kantenqualität **Schleifen**.

    *(Screenshot der DXF-Import-Konfiguration, der die Felder "Grenze" und "Kante" zeigt.)*

12. Wir klicken auf die Schaltfläche [Form importieren].
13. Bei diesem Modell handelt es sich um das Modell 0, daher erscheint die Abfrage, ob auf das Modell 0 gewechselt werden soll. Wir beantworten die Frage mit [Ja]. Das Modell wird importiert.
14. Es öffnet sich der Dialog **Produktabgleich**. Es wurden alle Bohrungen erkannt. Wir klicken auf [OK].

    *(Screenshot des Produktabgleich-Dialogs, der die erkannten CAD-Bearbeitungen (Saumen, Bohrungen) und die zugeordneten Produkte anzeigt.)*

15. Die Stückliste sieht wie folgt aus: Die Bohrungen wurden auf der höchsten Stücklistenebene angehängt, d. h. direkt am VSG.

---
*A+W Business Stammdaten*
*B-637*
---

*(Screenshot der Stückliste, die das VSG-Produkt mit den angehängten Bohrungen und der Durchsprechöffnung zeigt.)*

## Wie verhält sich die iTOE beim DXF-Import, wenn man die Kantenqualität bei Bearbeitungen vorgibt

1. Wir erfassen eine Position, hier ESG 8 mm.
2. Wir wechseln in die Lasche **3. Modelle/Bearbeitungen**.
3. Im Bereich **Bearbeitung** aktivieren wir die Symbol-Schaltfläche für Modelle.
4. Im Feld **Modell** geben wir die **99** für freie Formen ein.
5. Im Bereich **S+N-Datei** aktivieren wir die Checkbox und klicken am Ende des Feldes auf das Ordner-Symbol.
6. Wir wählen die gewünschte Datei aus und klicken auf [Öffnen].
7. Es öffnet sich der Dialog **DXF Import** mit einer Vorschau des zu importierenden Modells. Es handelt sich um eine Tür mit zwei kleinen Löchern und einem größeren Loch (Durchsprechöffnung) in der Mitte.

   *(Screenshot des DXF Import Dialogs, der eine Türform mit drei Öffnungen zeigt.)*

8. Wir klicken auf die Schaltfläche [Bearbeitung konfigurieren]. Da hier zunächst keine Kantenqualität angegeben ist, werden in der Vorschau nur zwei kleine Kreise (Lochbohrungen) und ein großer Kreis (Durchsprechöffnung) dargestellt.

---
*A+W Business Stammdaten*
*B-638*
---

*(Screenshot des Konfigurationsdialogs. Die Kantenqualität ist "None". Die Vorschau zeigt nur die Umrisse der Löcher.)*

9. Ändern wir die Kantenqualität in **Polieren**, wird diese in der Vorschau mit zwei x (xx) dargestellt.

   *(Screenshot des Konfigurationsdialogs. Kantenqualität ist jetzt "Polishing". Die Vorschau zeigt die kleinen Löcher mit "xx", was die polierte Kante symbolisiert.)*

10. Das große Loch in der Mitte wird nicht mit zwei x dargestellt, da das Loch einen größeren Durchmesser hat als das **Limit**, für das ein Loch als Lochbohrung erkannt wird (100 mm). Ändern wir den Wert von 100 auf 150, wird auch das große Loch entsprechend dargestellt. Es hat die zwei x für die Kantenqualität Polieren und das Fadenkreuz für die Lochbohrung.

---
*A+W Business Stammdaten*
*B-639*
---

*(Screenshot des Konfigurationsdialogs. Das Limit für Bohrlöcher wurde auf 150 erhöht. Die Vorschau zeigt nun alle drei Löcher mit "xx" (poliert) und Fadenkreuz.)*

11. Wir ändern jetzt das Limit wieder zurück auf 100, damit das große Loch als Durchsprechöffnung erkannt wird.
12. Wenn die Kantenqualität von dem großen Loch ebenfalls **Poliert** sein soll, muss diese Einstellung im Bereich **Allgemeine Bearbeitung** vorgenommen werden.

    *(Screenshot des Konfigurationsdialogs. Das Limit ist wieder 100. Im Bereich "Additional Processing" -> "Edge" ist "Polishing" ausgewählt. Die Vorschau zeigt nun das große Loch ebenfalls als poliert.)*

13. Wir klicken auf die Schaltfläche [Form importieren].

---
*A+W Business Stammdaten*
*B-640*
---

14. Bei diesem Modell handelt es sich um das Modell 0, daher erscheint die Abfrage, ob auf das Modell 0 gewechselt werden soll. Wir beantworten die Frage mit [Ja]. Das Modell wird importiert.
15. Es öffnet sich der Dialog **Produktabgleich**.
    
    *(Screenshot des Produktabgleich-Dialogs.)*

16. Für die Durchsprechöffnung klicken wir im Bereich **Regel bearbeiten** auf die drei Punkte. Es öffnet sich der Dialog **Produkt Zuordnung**. Die Regel, die markiert ist, ist die Regel, die gefunden wurde. Da der Bearbeitungstyp **Durchsprechöffnung** und die Kantenqualität **Polieren** sind erfüllt, entsteht daraus das Produkt 9941 (Durchsprechöffnung mit polierten Kanten).
    
    *(Screenshot des "Produkt Zuordnung"-Dialogs. Die Regel für "Durchsprechöffnung" mit Kantenqualität "Polieren" und Priorität 5 wird zu Produkt 9941.)*

17. Schauen wir uns die andere Regel an, dann sehen wir, dass es sich bei dieser Regel um die allgemeine Regel handelt. Diese Regel bezieht sich ausschließlich auf den Bearbeitungstyp Durchsprechöffnung, der dann zum Produkt 941 wird. Hierbei handelt es sich also um eine Durchsprechöffnung ohne Kantenqualität. Diese Regel hat außerdem die Priorität 10 wohingegen die Regel 2 die Priorität 5 hat.

---
*A+W Business Stammdaten*
*B-641*
---

*(Screenshot des "Produkt Zuordnung"-Dialogs für die allgemeine Regel ohne Kantenqualität. Priorität ist 10.)*

18. Wir ändern jetzt in der gefunden Regel die Priorität von 5 auf 11. Die Regel, die die Kantenqualität nicht berücksichtigt und auf das allgemeine Produkt 941 verweist, hat die Priorität 10. Diese liegt also vor der Priorität 11. Wir klicken auf [OK], der Dialog wird geschlossen und wir befinden uns wieder im Dialog **Produktabgleich**. Dort sehen wir, dass die Durchsprechöffnung (nach Änderung der Priorität) zu Produkt 941 (Durchsprechöffnung ohne polierte Kanten) wurde. Das heißt, obwohl im DXF-Import die Kantenqualität übergeben wurde, übersteuert die gefundene Regel diese Einstellungen!
    
    *(Screenshot des Produktabgleich-Dialogs nach der Prioritätsänderung. Die Durchsprechöffnung wird jetzt zu Produkt 941 (ohne polierte Kanten) zugeordnet.)*

19. Wir klicken auf [OK], der Dialog wird geschlossen und wir befinden uns wieder in der Positionserfassung. Wie an der Skizze zu erkennen ist, fehlen bei der Durchsprechöffnung die beiden x. Das zeigt an, dass es hier keine Kantenqualität (aufgrund geänderter Priorität) gibt. Bei den beiden Lochbohrungen sind die xx vorhanden. Hätte die Importregel für die beiden Lochbohrungen ebenfalls auf ein Produkt verwiesen, das die Kantenqualität Polieren nicht eingestellt hat, wären die beiden x auch nicht da.

---
*A+W Business Stammdaten*
*B-642*
---

*(Screenshot der Skizze in der Positionserfassung. Die große Öffnung hat keine 'xx', die kleinen haben 'xx'.)*

> **i Regeln beachten**
> Wenn man eine Unterscheidung (poliert, geschliffen, etc.) machen möchte, gerade bei größeren Ausschnitten und es existieren dafür verschiedene Artikel, dann ist es auf jeden Fall wichtig, dass die Kantenqualität beim Import bei den Regeln berücksichtigt wird. Die Priorität muss so eingestellt sein, dass diese Regeln eine niedrigere Priorität (niedrigere Zahl in der Priorität heißt, dass diese angewendet wird) haben als die allgemeine Regel. Nur so kann gesteuert werden, dass wirklich im A+W Business ankommt, ob die Kantenqualität z. B. poliert oder geschliffen ist. Was in der DXF-Datei angegeben ist, ist nicht zwangsläufig das, was importiert wird. Der Import hängt von den eingestellten Regeln ab.

---
*A+W Business Stammdaten*
*B-643*
---

## DXF-Import auf eine Position, die bereits eine Bearbeitung hat

1. Es existiert folgende Ausgangssituation (ab A+W Business Version 13.4.1993): Template mit zwei Löcher und einer Durchsprechöffnung (noch nicht zu sehen).
   
   *(Screenshot einer Stückliste mit einem VSG und mehreren Bearbeitungen, inklusive einer Skizze.)*

2. Wir markieren in der Stückliste den Eintrag **8000/Rechteck**, öffnen das Kontextmenü und wählen **Komponente löschen**.
   
   *(Screenshot der Stückliste nach dem Löschen des Rechtecks.)*

3. Im Bereich **Bearbeitung** aktivieren wir die Symbol-Schaltfläche für Modelle.
4. Im Feld **Modell** geben wir die **99** für freie Formen ein.
5. Im Bereich **S+N-Datei** aktivieren wir die Checkbox und klicken am Ende des Feldes auf das Ordner-Symbol.
6. Wir wählen die gewünschte Datei aus und klicken auf [Öffnen].
7. Es öffnet sich der Dialog **DXF Import** mit einer Vorschau des zu importierenden Modells. Es handelt sich um eine Tür mit zwei kleinen Löchern und einem größeren Loch (Durchsprechöffnung) in der Mitte. Wir klicken auf die Schaltfläche [Bearbeitung konfigurieren].

---
*A+W Business Stammdaten*
*B-644*
---

*(Screenshot des DXF-Import Konfigurationsdialogs.)*

8. Wir ändern das Limit von 100 auf 300, damit das obere Loch als Lochbohrung erkannt wird und klicken auf die Schaltfläche [Form importieren].
9. Bei diesem Modell handelt es sich um das Modell 0, daher erscheint die Abfrage, ob auf das Modell 0 gewechselt werden soll. Wir beantworten die Frage mit [Ja]. Das Modell wird importiert.
10. Es öffnet sich der Dialog **Produktabgleich**.
    
    *(Screenshot des Produktabgleich-Dialogs, der alle erkannten Bohrungen zeigt.)*

11. Wir bestätigen die Angaben mit [OK].
12. Die Stückliste und die Skizze werden entsprechend angepasst.

---
*A+W Business Stammdaten*
*B-645*
---

*(Screenshot der aktualisierten Stückliste und Skizze mit allen importierten und ursprünglichen Bearbeitungen.)*

> **i Ab A+W Business Version 13.4.1993**
> Das oben gezeigte Verfahren gilt für alle Bearbeitungen, außer Kantenbearbeitungen (polieren, schleifen, etc.). Auch für solche, die manuell erfasst worden sind. Das bedeutet, es wird immer zuerst die DXF-Datei importiert. Sollen manuelle Bearbeitungen hinzugefügt werden, müssen diese im Anschluss gemacht werden.

## Auf welcher Stücklistenebene wird eine Bearbeitung importiert, wenn man keine Kantenqualität vorgibt

1. Es handelt sich um ein VSG, welches aus zwei ESG besteht.
   
   *(Screenshot der VSG-Stückliste.)*

2. Im Bereich **Bearbeitung** aktivieren wir die Symbol-Schaltfläche für Modelle.
3. Im Feld **Modell** geben wir die **99** für freie Formen ein.
4. Im Bereich **S+N-Datei** aktivieren wir die Checkbox und klicken am Ende des Feldes auf das Ordner-Symbol.
5. Wir wählen die gewünschte Datei aus und klicken auf [Öffnen].
6. Es öffnet sich der Dialog **DXF Import** mit einer Vorschau des zu importierenden Modells. Es handelt sich um einen Halbkreis mit sechs kleinen Löchern und einem bogenförmigen Ausschnitt. Wir klicken auf die Schaltfläche [Bearbeitung konfigurieren].

---
*A+W Business Stammdaten*
*B-646*
---

*(Screenshot des DXF-Import Konfigurationsdialogs für das Halbkreis-Modell.)*

7. Die Bohrlöcher sowie der bogenförmige Ausschnitt bekommen keine Kantenqualität vorgegeben. Wir klicken auf die Schaltfläche [Form importieren].
8. Bei diesem Modell handelt es sich um das Modell 62, daher erscheint die Abfrage, ob auf das Modell 62 gewechselt werden soll. Wir beantworten die Frage mit [Ja]. Das Modell wird importiert.
9. Es öffnet sich der Dialog **Produktabgleich**. Wir sehen, dass für alle Bearbeitungen eine Produktnummer gefunden wurde. Wir klicken auf [OK].

   *(Screenshot des Produktabgleich-Dialogs, der die erkannten Bearbeitungen (Saumen, Ausschnitt, Bohrungen) anzeigt.)*

10. Es folgt der Hinweis [2671]: Bei allen Modellen mit einer Kantenanzahl ungleich 4 muss die Breiten- oder Höhenzuordnung manuell eingetragen werden! Den bestätigen wir mit [OK].
11. Wir wechseln in das Register **Stückliste**, das sich nach dem Import wie folgt darstellt:

    *(Screenshot der komplexen Stückliste nach dem Import. Die Bearbeitungen sind auf verschiedenen Ebenen angehängt.)*

---
*A+W Business Stammdaten*
*B-647*
---

## Auf welcher Stücklistenebene wird eine Bearbeitung importiert, wenn man eine Kantenqualität vorgibt

1. In den nächsten Schritten wiederholen wir den oben gezeigten Ablauf, jedoch geben wir diesmal eine Kantenqualität sowohl für die Bohrungen als auch für den bogenförmigen Kantenausschnitt vor.
2. Im Bereich **Bearbeitung** aktivieren wir die Symbol-Schaltfläche für Modelle.
3. Im Feld **Modell** geben wir die **99** für freie Formen ein.
4. Im Bereich **S+N-Datei** aktivieren wir die Checkbox und klicken am Ende des Feldes auf das Ordner-Symbol.
5. Wir wählen die gewünschte Datei aus und klicken auf [Öffnen].
6. Es öffnet sich der Dialog **DXF Import** mit einer Vorschau des zu importierenden Modells. Wir klicken auf die Schaltfläche [Bearbeitung konfigurieren].

   *(Screenshot des DXF-Import Konfigurationsdialogs.)*

7. Für die Bohrungen wählen wir als Kantenqualität **Geschliffen**. Ebenso für den bogenförmigen Kantenausschnitt. Wir klicken auf die Schaltfläche [Form importieren].

---
*A+W Business Stammdaten*
*B-648*
---

*(Screenshot des DXF-Import Konfigurationsdialogs mit eingestellter Kantenqualität "Grinding".)*

8. Bei diesem Modell handelt es sich um das Modell 62, daher erscheint die Abfrage, ob auf das Modell 62 gewechselt werden soll. Wir beantworten die Frage mit [Ja]. Das Modell wird importiert.
9. Es öffnet sich der Dialog **Produktabgleich**. Wir sehen, dass für alle Bearbeitungen eine Produktnummer gefunden wurde. Wir klicken auf [OK].

   *(Screenshot des Produktabgleich-Dialogs.)*

10. Es folgt der Hinweis [2671]: Bei allen Modellen mit einer Kantenanzahl ungleich 4 muss die Breiten- oder Höhenzuordnung manuell eingetragen werden! Den bestätigen wir mit [OK].
11. Wir wechseln in das Register **Stückliste**, das sich nach dem Import wie folgt darstellt: Die Bohrungen befinden sich wieder am Hauptprodukt, obwohl wir eine Kantenqualität hinzugefügt haben. Das bedeutet, Bohrungen verhalten sich immer gleich. Sie kommen immer an das Hauptprodukt, egal, ob eine Kantenqualität vorgegeben ist oder nicht.

    *(Screenshot der Stückliste nach Import. Bohrungen sind am Hauptprodukt angehängt.)*

---
*A+W Business Stammdaten*
*B-649*
---

12. Anders verhält sich der bogenförmige Kantenausschnitt. Dieser ist jetzt zweimal vorhanden und zwar jeweils direkt am ESG. Gibt man eine Kantenqualität bei Ausschnitten vor, dann kommt die Bearbeitung immer auf die zweit unterste Stücklistenebene (auf das zweit unterste Glas).

    *(Screenshot der Stückliste, der zeigt, dass der Kantenausschnitt ("Curved cut") jetzt zweimal, jeweils unter den einzelnen Gläsern (ESG), vorhanden ist.)*

## Auf welcher Stücklistenebene wird eine Bearbeitung importiert, wenn man eine Kantenqualität vorgibt (Modell 99)

1. In den nächsten Schritten wiederholen wir den oben gezeigten Ablauf, jedoch geben wir diesmal eine Kantenqualität sowohl für die Bohrungen als auch für den bogenförmigen Kantenausschnitt vor und wir wechseln nicht auf das vorgeschlagene Modell 62 sonder bleiben bei Modell 99.
2. Im Bereich **Bearbeitung** aktivieren wir die Symbol-Schaltfläche für Modelle.
3. Im Feld **Modell** geben wir die **99** für freie Formen ein.
4. Im Bereich **S+N-Datei** aktivieren wir die Checkbox und klicken am Ende des Feldes auf das Ordner-Symbol.
5. Wir wählen die gewünschte Datei aus und klicken auf [Öffnen].
6. Es öffnet sich der Dialog **DXF Import** mit einer Vorschau des zu importierenden Modells. Wir klicken auf die Schaltfläche [Bearbeitung konfigurieren].

    *(Screenshot des DXF-Import Konfigurationsdialogs.)*

7. Für die Bohrungen wählen wir als Kantenqualität **Geschliffen**. Ebenso für den bogenförmigen Kantenausschnitt. Wir klicken auf die Schaltfläche [Form importieren].

---
*A+W Business Stammdaten*
*B-650*
---

*(Screenshot des DXF-Import Konfigurationsdialogs mit eingestellter Kantenqualität "Grinding".)*

8. Bei diesem Modell handelt es sich um das Modell 62, daher erscheint die Abfrage, ob auf das Modell 62 gewechselt werden soll. Wir beantworten die Frage mit [Nein]. Das Modell wird importiert.
9. Es öffnet sich der Dialog **Produktabgleich**. Wir sehen, dass für alle Bearbeitungen eine Produktnummer gefunden wurde. Wir klicken auf [OK].

   *(Screenshot des Produktabgleich-Dialogs.)*

10. Die Stückliste sieht jetzt wie folgt aus. Die Lochbohrungen befinden sich direkt am Hauptprodukt und der bogenförmige Kantenausschnitt befindet sich wieder auf dem zweit untersten Glas.

    *(Screenshot der Stückliste, die die Verteilung der Bearbeitungen zeigt: Bohrungen am Hauptprodukt (Modell 99), Ausschnitt am untergeordneten Glas.)*

---
*A+W Business Stammdaten*
*B-651*
---

## Die Prioritäten der Regeln beim Produktabgleich

Wir importieren ein Einfachglas 4mm mit zwei Lochbohrungen Durchmesser 20 mm, deren Kantenqualität poliert ist.

*(Screenshot des Produktabgleich-Dialogs für eine Bohrung. Die gefundene Regel ist "93005 Lochbohrung poliert".)*

1. Wir klicken auf die drei Punkte im Bereich **Regel bearbeiten/einfügen**. Es öffnet sich der Dialog **Produkt Zuordnung**.
   
   *(Screenshot des Produkt Zuordnung-Dialogs für Bohrungen mit Kantenqualität Polieren.)*

2. Für den Bearbeitungstyp **Bohrungen** gibt es vier verschiedene Regeln. Dabei ist die zweite Regel mit dem Durchmesser 0-21 die, die gefunden wurde. Alle Regeln haben unterschiedliche Prioritäten:

   *(Vier Screenshots zeigen die vier verschiedenen Regeln für Bohrungen: 1. Säumen, Prio 51; 2. Polieren, Prio 99; 3. Geschlitzt, Prio 50; 4. Allgemein, Prio 9999.)*

---
*A+W Business Stammdaten*
*B-652*
---

Die Regeln werden anhand der eingestellten **Priorität** (in der aufsteigenden Reihenfolge angefangen mit 0) geprüft und sind vom Datentyp integer (nach oben offen).

3. Die erste Regel hat die Priorität 51 und wird auf die Kantenqualität **Säumen** sowie den Durchmesser 0-21 geprüft. Da unsere Lochbohrung die Kantenqualität **poliert** hat, wird diese Regel nicht gewählt.
4. Die dritte Regel hat die Priorität 50 und wird auf den Durchmesser 21-40 geprüft. Da unsere Lochbohrung einen Durchmesser von 20 hat, wird diese Regel nicht gewählt.
5. Die zweite Regel hat die Priorität 99 und wird auf die Kantenqualität **Polieren** sowie den Durchmesser 0-20 geprüft. Diese Angaben entsprechen den Angaben unserer Lochbohrung und somit wird diese Regel gewählt.
6. Die vierte Regel hat die Priorität 9999 und wird auf den Durchmesser 21-40 geprüft. Diese Regel wird nicht mehr geprüft, da die zweite Regel bereits einen Treffer erzielte.

---
*A+W Business Stammdaten*
*B-653*
---

## Produktzuordnung über Formel

Es gibt Regeln, die sich nicht mit den Standardparametern abbilden lassen können. Hier kommen dann Formeln, sogenannte Customizingformeln zum Einsatz. Die Formeln müssen im Vorfeld definiert werden.
⇨ Softwarereferenz, "Formeln" auf Seite B-1173

Sollten Sie Formeln benötigen oder eine Formel anpassen müssen, wenden Sie sich bitte an Ihren Ansprechpartner bei A+W.

Die folgenden Bilder dienen als Beispiel für solche Formeln:

Im Beispiel unten wird dem Bearbeitungstyp **1010 - Polieren** die Formel **0016-Formel iTOE gerade Modellkanten** zugewiesen. Sie wirkt auf die Produktart **Einfachglas** und wird zu dem Produkt **90100**.

*(Abbildung B-349 zeigt den Dialog "Produkt Zuordnung", in dem eine Regel mit einer Customizing-Formel definiert wird.)*

Im nächsten Beispiel wird dem Bearbeitungstyp **1010 - Polieren** die Formel **0017-Formel iTOE ungerade Modellkanten** zugewiesen. Sie wirkt auf die Produktart **Einfachglas** und wird zu dem Produkt **90050**.

---
*A+W Business Stammdaten*
*B-654*
---

*(Abbildung B-350 zeigt den Dialog "Produkt Zuordnung" mit der Formel 0017, die ungerade Modellkanten zu dem Produkt 90050 (Kanten feingeschliffen) zuordnet.)*

---
*A+W Business Stammdaten*
*B-655*
---
*(Leere Seite)*
---
*A+W Business Stammdaten*
*B-656*
---

# B: A+W Business Stammdaten - Softwarereferenz

---
*(Titelblatt)*
*A+W Software for Glass, Windows & Doors*
*Softwarereferenz*
---

## In diesem Kapitel finden Sie folgende Themen:
- Übersicht
- Allgemein
- Produkte
  - Produktverwaltung
  - Artikel
  - Preise
  - Preisverwaltung
- Lager
- Marktpartner
  - Allgemein
  - Partnerverwaltung
  - Kunde
  - Lieferant
- Versand
- Fertigung
- Auftrag
- Finanzen
  - Firma
  - Texte
  - Formulare
- CEKAL
- CE-Kennzeichen
- B2B

### Inhaltsverzeichnis

- **Übersicht** ... B-667
- **Allgemein** ... B-668
  - Sprachen ... B-668
  - Preis-/Mengeneinheit für Mehrsprachigkeit ... B-669
  - Monate ... B-670
  - Tage ... B-670
  - Landeskürzel ... B-671
  - Kalender ... B-672
  - Länder Kalender ... B-674
  - Basisnummernkreise ... B-675
- **Produkte** ... B-677
  - Allgemein ... B-677
  - Produktarten ... B-678
  - Produktgruppen ... B-679
  - WGR ... B-680
  - Kombi-WGR ... B-682
  - Top-WGR ... B-684
  - Varianten ... B-685
  - Sprossentypen ... B-687
  - Reklamationsverursacher ... B-689
  - Reklamationsgrund ... B-690
  - Struktur ... B-691
  - Strukturseite ... B-692

---
*A+W Business Stammdaten*
*B-658*
---

- Beschichtungsseite ... B-693
- Beschichtungsart ... B-694
- Glasartgruppen ... B-695
- Gütetext ... B-696
  - Gütetext - Grundeinstellungen ... B-696
  - Gütetext - Restriktionen ... B-697
- Leistungserklärung Verwaltung ... B-698
- Austauschgruppen ... B-699
- Austauschzuordnung ... B-700
- Klassifikatoren - Produkt ... B-701
- Produktverwaltung ... B-702
  - Menüs in der Produktverwaltung ... B-702
  - Menü Optionen ... B-702
  - Menü Funktionen ... B-703
  - Produktverwaltung ... B-705
  - Produktverwaltung - Produkt ... B-706
  - Produktverwaltung – Fertigung ... B-711
  - Produktverwaltung - Preis/Zuschlag ... B-717
  - Produktverwaltung - Lager/Einkauf ... B-723
  - Produktverwaltung - Modelle/Bearbeitungen ... B-728
  - Produktverwaltung - Stückliste ... B-731
  - Produktverwaltung - Texte ... B-734
  - Produktverwaltung - Sprachen ... B-736
  - Produktverwaltung - A+W Production ... B-737
  - Produktverwaltung - Anlagen/Klassifikatoren ... B-741
  - Produktverwaltung - Sprossen ... B-743
- Technische Parameter ... B-744
- Technische Parameter kopieren ... B-746
- Produktänderung ... B-747
- Produktkennzeichen Verwaltung ... B-748
  - Produktkennzeichen Verwaltung - Editieren ... B-748
  - Produktkennzeichen Verwaltung - Kopieren ... B-750
- Glasarten ... B-752
- Artikel ... B-753
- Lagermaße ... B-753
  - Menü Funktionen ... B-753
  - Lagermaße - Produkt ... B-754
  - Lagermaße - Tabelle ... B-757
- Maßzuschlag ... B-758
  - Maßzuschlag - Maßzuschläge ... B-758
  - Maßzuschlag - Tabelle ... B-759
- Produktvarianten ... B-760
  - Menü Funktionen ... B-760
  - Produktvarianten - Varianten ... B-760
  - Produktvarianten - Tabelle ... B-763
- Varianten kopieren ... B-764
- EK-Kalkulation ... B-765
- Abstandhalterrestriktionen ... B-767
- Template Editor ... B-769
- ISO-Aufbau ... B-770
- Bearbeitungsrestriktionen ... B-772
- Motive ... B-774
- Modellkantenqualitäten ... B-775

---
*A+W Business Stammdaten*
*B-659*
---

- Beschlagszuordnung ... B-776
- ITOE Regeln ... B-778
- **Preise** ... B-780
  - Preisjahrgang ... B-781
  - Preisschlüssel ... B-782
  - Tarife ... B-783
  - Sonstige Zuschläge ... B-785
  - Austauschzuschläge ... B-788
    - Menü Funktionen ... B-789
    - Austauschzuschläge - Tabelle ... B-790
    - Austauschzuschläge - Allgemein, nach Dicke, nach Produkt ... B-792
    - Austauschzuschläge - Kunden-, Lieferantenpreise ... B-794
    - Auswahl - Austauschzuschlag ... B-795
  - Austauschpreise kopieren ... B-795
    - Austauschpreise kopieren - Quelle, Ziel ... B-796
    - Austauschpreise kopieren - Preisänderung ... B-798
  - Preise pro Austauschartikel komplett kopieren ... B-799
    - Preise pro Austauschartikel komplett kopieren - Quelle, Ziel ... B-799
    - Preise pro Austauschartikel komplett kopieren - Preisänderung ... B-801
  - Austauschpreise löschen ... B-802
  - Austauschpreise ändern ... B-803
    - Austauschpreise ändern - Preisart ... B-803
    - Austauschpreise ändern - Preisänderung ... B-805
  - Preisgruppen ... B-806
  - Preisgruppenzuordnung ... B-807
  - Preisgruppenzuordnung kopieren ... B-808
  - Gruppenzuschläge ... B-809
  - Gruppenzuschläge kopieren ... B-812
    - Gruppenzuschläge kopieren - Quelle, Ziel ... B-813
    - Gruppenzuschläge kopieren - Preisänderung ... B-815
  - Gruppenzuschläge löschen ... B-816
  - Gruppenzuschläge ändern ... B-817
    - Gruppenzuschläge ändern - Preisart ... B-817
    - Gruppenzuschläge ändern – Preisänderung ... B-819
  - Mischkalkulation ... B-820
  - Modellbearbeitungszuschläge ... B-821
  - Zuschläge kopieren ... B-823
  - Preis- und Mengeneinheit ... B-824
  - Versicherungspreise ... B-826
    - Versicherungspreise - Reparaturverglasung ... B-827
    - Versicherungspreise - Notverglasung ... B-829
    - Versicherungspreise - Auf-/Abschläge ... B-830
    - Versicherungspreise - Zusatzleistungen ... B-832
  - Sprossenpreiselemente ... B-833
  - ISO Preise ... B-834
- **Preisverwaltung** ... B-836
  - Menüs in der Preisverwaltung ... B-836
  - Menü Optionen ... B-836
  - Menü Funktionen ... B-837
  - Menü Historie ... B-837

---
*A+W Business Stammdaten*
*B-660*
---

- Preise ... B-839
  - Preise – Preisauswahl ... B-840
  - Preise – Matrix ... B-843
  - Preise – Vektor ... B-845
  - Preise – Einzelpreis ... B-846
  - Preise – Modell ... B-847
  - Preise – Sprossen ... B-848
  - Preise – Würfel ... B-849
  - Preise – Preisformel ... B-850
- Preise ändern ... B-851
- Preise kopieren ... B-853
- Preise löschen ... B-856
- Preismatrizenimport ... B-857
- Preismatrix importieren ... B-858
- Preismatrix exportieren ... B-859
- Änderungshistorie ... B-861
- **Lager** ... B-863
  - Verpackung ... B-863
  - Ebene 1 bis 4 ... B-864
  - Lagerdefinition ... B-865
  - Lagerebenen ... B-866
  - Lagerkategorien ... B-867
  - Lagerort für Aggregate ... B-868
  - Suche Aggregate ... B-869
  - Buchart ... B-870
- **Marktpartner** ... B-871
  - Allgemein ... B-872
    - Partnergruppen ... B-873
    - Kundengruppen ... B-874
    - Lieferantengruppen ... B-875
    - Vorgänge ... B-876
    - Anreden ... B-877
    - Titel (Funktion) ... B-877
    - Branchen ... B-878
    - Objekte ... B-879
    - Provinz ... B-880
  - Partner ... B-881
  - Klassifikatoren ... B-881
    - Klassifikatoren – Marktpartner Gemeinsam, Kunden, Lieferanten ... B-882
    - Klassifikatoren – Produkt ... B-883
  - Partnerverwaltung ... B-884
    - Menüs in der Partnerverwaltung ... B-884
    - Menü Funktionen ... B-885
    - Menü Optionen ... B-886
    - Menü Druck ... B-886

---
*A+W Business Stammdaten*
*B-661*
---

- Partnerverwaltung ... B-887
  - Partnerverwaltung – Adresse ... B-888
  - Partnerverwaltung – Auftrag ... B-892
  - Partnerverwaltung – Mitarbeiter/Filiale/Vorgänge ... B-899
  - Partnerverwaltung – Texte ... B-900
  - Partnerverwaltung – Klassifikatoren ... B-902
  - Partnerverwaltung – Finanzen ... B-904
  - Partnerverwaltung – Saldo ... B-909
  - Partnerverwaltung – Vertrieb ... B-913
  - Partnerverwaltung – Produktion ... B-915
  - Partnerverwaltung – Anlage ... B-918
- Freie Nummern / Bereiche ... B-919
- Telekommunikationsdaten ... B-920
- Rechnungsstellungszuschlag/Mindestwert pro AV-Bereich ... B-921
- Tourrangfolge ... B-922
- Textsuche ... B-923
- Umsatz / AV-Bereich ... B-924
- Filiale ... B-924
- Mitarbeiter ... B-925
- Vorgangsverwaltung ... B-927
- Mitarbeiter-Klassifikatoren ... B-928
- Klassifikatoren Wertzuordnung ... B-929
- OP-Abfrage ... B-930
- Stammdaten kopieren ... B-931
- Partneränderung ... B-931
- Konditionen ... B-932
- **Kunde** ... B-933
  - Rabattverwaltung (Kunden, Lieferanten) ... B-934
    - Menü Funktionen ... B-934
    - Rabattverwaltung – Rabattübersicht ... B-935
    - Rabattverwaltung – Abweichungen ... B-937
    - Rabattverwaltung – Staffelrabatte ... B-939
    - Rabattverwaltung – Austauschrabatte ... B-940
    - Rabattverwaltung – Tabelle ... B-941
  - Rabatte kopieren, ändern ... B-942
    - Rabatte kopieren ... B-942
    - Rabatte ändern ... B-944
  - Rabatte löschen ... B-946
  - Parameter (Kunden, Lieferanten) ... B-947
  - Kundenindividuelle Produkte ... B-949
  - Lieferdauer (Kunde, Lieferant) ... B-951
  - Objekte (Kunde, Lieferant) ... B-952
    - Menüs in der Objekt-/Abrechnungsverwaltung ... B-953
    - Abrechnungen – Abrechnungen ... B-954
    - Abrechnungen – Rahmenauftrag ... B-959
    - Abrechnungen – Zugeordnete Aufträge ... B-960
    - Abrechnungen – Zugeordnete Bestellungen ... B-961
    - Abrechnungen – Summen ... B-962
    - Abrechnungen – Veranschlagte Mengen ... B-963
    - Abrechnungen – Tabelle ... B-964
  - Objekte – Dokumente ... B-965
  - Stundenforderung ... B-966
  - Einkaufsforderung ... B-967

---
*A+W Business Stammdaten*
*B-662*
---

- Forderungsberechnung ... B-968
- Forderungs-Historie ... B-969
- Rundung (Kunde, Lieferant) ... B-970
- Rundung Kunden-, Lieferantengruppen ... B-971
- Logoposition ... B-972
- Abweichende Kunden-, Lieferantengruppen ... B-974
- Kreditlimit-Analyse ... B-975
- Deckungsbeitrags-Grenzwerte ... B-978
- Übermengen ... B-980
- Kalender (Kunde) ... B-982
- Kalenderdaten übertragen ... B-984
- **Lieferant** ... B-985
  - Lieferant ... B-986
  - Lieferantenkartei ... B-987
    - Lieferantenkartei – Produkte ... B-988
    - Lieferantenkartei – Warengruppen ... B-991
    - Lieferantenkartei – Bedingungen ... B-992
  - Nachweis ... B-993
- **Versand** ... B-994
  - Lieferbedingungen ... B-994
  - Touren ... B-995
  - Lkw ... B-998
  - Fahrer ... B-999
  - Zolltouren ... B-1000
  - Zollnummern ... B-1001
- **Fertigung** ... B-1003
  - Optimierung ... B-1003
  - Erfassungsstellen Produktion ... B-1004
  - Glasart-Jumbos-Tische ... B-1007
  - Zuschneidetische ... B-1009
  - Arbeitsgänge ... B-1013
  - Bruchgründe ... B-1014
- **Auftrag** ... B-1015
  - Rundung ... B-1015
  - Rundungspunkte ... B-1017
  - Rundungszuordnung ... B-1018
  - Statusverwaltung ... B-1020
  - Statuspunkte ... B-1021
  - Statuszuordnung ... B-1022
  - Geschäftsart ... B-1024
  - Grenzmengen ... B-1025
  - Priorität ... B-1026
  - Nummernkreise ... B-1028
    - Menü Funktionen ... B-1028
    - Nummernkreise – Dokumente ... B-1028
    - Nummernkreise – Produktion ... B-1031
    - Nummernkreise – FiBu ... B-1032
  - Nummernkreise – Tabelle ... B-1033
  - Sperrkennzeichen ... B-1034
  - Dokumententyp ... B-1036
  - Kategorien ... B-1038
  - Gründe Lieferterminverschiebung ... B-1039
- **Finanzen** ... B-1040

---
*A+W Business Stammdaten*
*B-663*
---

- Steuer ... B-1040
- Zahlungsbedingungen ... B-1042
- Bonität ... B-1043
- Banken ... B-1044
- Währung ... B-1045
- Erlöskonten ... B-1047
- Erlöskonten kopieren ... B-1049
- Kostenart ... B-1050
- Kostenstellen ... B-1051
- Zahlungswege ... B-1052
- Brasilianische Steuer ... B-1053
- **Firma** ... B-1054
  - Firmendaten ... B-1055
    - Firmendaten – Mandant ... B-1056
    - Firmendaten – Steuer ... B-1058
    - Firmendaten – FiBu ... B-1061
    - Firmendaten – Dokumente ... B-1066
    - Firmendaten – Parameter ... B-1073
    - Firmendaten – Preisberechnung ... B-1085
    - Firmendaten – Lager/EK/EDI ... B-1096
    - Firmendaten – Archiv ... B-1104
    - Firmendaten – Tagesabschluss ... B-1111
    - Firmendaten – System ... B-1113
    - Firmendaten – Kalkulation ... B-1120
    - Firmendaten – Druck ... B-1122
    - Firmendaten – Produktion ... B-1126
    - Firmendaten – Versand ... B-1134
    - Firmendaten – Kapa-Planung ... B-1138
    - Firmendaten – Sonstiges ... B-1145
  - Portugiesische Zertifizierung ... B-1147
  - Mitarbeiter ... B-1149
    - Mitarbeiter – Mitarbeiter ... B-1149
    - Mitarbeiter – Spezifikation ... B-1151
    - Mitarbeiter – Einstellungen ... B-1153
  - Mitarbeitergruppen ... B-1155
  - Mitarbeiterrechte ... B-1156
  - Rechte kopieren ... B-1158
  - Statusverwaltung pro Mitarbeitergruppe ... B-1159
  - AV-Bereiche ... B-1160
  - AD-Bereiche ... B-1161
  - Vertreterprovision ... B-1163
  - Vertreter – Provisionssätze kopieren ... B-1166
  - Banken ... B-1167
  - Filialen ... B-1169
  - Buchungsperioden ... B-1170
  - Produktzuordnung Zuschläge ... B-1171
  - Formeln ... B-1173
  - Schnittstellen-Dienst ... B-1175
    - Schnittstellen-Dienst – Einstellungen A+W Production-Formate ... B-1175
    - Schnittstellen-Dienst – Einstellungen weitere Formate ... B-1181
    - Schnittstellen-Dienst – Optionen ... B-1184
  - Customizing ... B-1186
  - Datencontainer ... B-1187

---
*A+W Business Stammdaten*
*B-664*
---

- **Texte** ... B-1188
  - Textkennzeichen ... B-1188
  - Texte ... B-1189
  - Systemtexte ... B-1191
  - Mahntexte ... B-1192
  - Dateianhangs-Typen ... B-1193
  - Dateianhangs-Bemerkungen ... B-1194
  - Technische Werte ... B-1194
- **Formulare** ... B-1195
  - Formularverwaltung ... B-1195
    - Formularverwaltung – Formular ... B-1196
    - Formularverwaltung – Kopf-/Fußtexte ... B-1199
    - Formularverwaltung – Texte ... B-1200
    - Formularverwaltung – Optionen 1 ... B-1201
    - Formularverwaltung – Optionen 2 ... B-1205
    - Formularverwaltung – Optionen 3 ... B-1208
    - Formularverwaltung – Skizzendruck ... B-1210
    - Formularverwaltung – Customizing ... B-1212
  - Auftragsformulare ... B-1213
  - Druckaufträge ... B-1214
  - Crystal Reports ... B-1220
  - Zuordnung ... B-1221
- **CEKAL** ... B-1222
  - Klassen ... B-1223
  - Zuordnung ... B-1224
  - Ergebnisse ... B-1225
  - Textzuordnung ... B-1227
  - Restriktionen ... B-1229
  - Produkttexte ... B-1231
- **CE-Kennzeichen** ... B-1233
  - CPIP-Code ... B-1233
  - Maßrestriktionen ... B-1234
  - ISO-Suchdaten ... B-1235
  - Einstellungen ... B-1236
- **B2B** ... B-1237
  - Produkte (Kunde, Lieferant) ... B-1237
    - Menü Funktionen ... B-1237
    - Produkte – Stückliste ... B-1238
    - Produkte – Parameter ... B-1240
    - Produkte – Tabelle ... B-1241
    - Produkte – Modelle/Bearbeitungen ... B-1242
    - Produkte – Sprossen ... B-1243
    - Produkte – Anlagen ... B-1244
  - Kopieren von Fremdartikeln ... B-1245
  - SZR (Kunde, Lieferant) ... B-1246
  - Gas (Kunde, Lieferant) ... B-1247
  - Touren (Kunde, Lieferant) ... B-1248
  - Kunde, Lieferant ... B-1249
    - Menü Funktionen ... B-1249
    - Kunde, Lieferant – Auswahl ... B-1249
    - Kunde, Lieferant – Parameter ... B-1251
    - Kunde, Lieferant – Tabelle ... B-1254
  - Dokumentenexport ... B-1255

---
*A+W Business Stammdaten*
*B-665*
---

- SN-Datei-Regeln ... B-1258
- Artikelimport ... B-1259

---
*A+W Business Stammdaten*
*B-666*
---

# Übersicht

Im Modul **Stammdaten** werden alle Daten zu A+W Business eingerichtet und gepflegt, die übergreifend von allen Modulen genutzt werden.

Die Stammdaten sind in folgende Menüs gegliedert:
- "Allgemein" auf Seite B-668
- "Produkte" auf Seite B-677
- "Preise" auf Seite B-780
- "Lager" auf Seite B-863
- "Marktpartner" auf Seite B-871
- "Versand" auf Seite B-994
- "Fertigung" auf Seite B-1003
- "Auftrag" auf Seite B-1015
- "Finanzen" auf Seite B-1040
- "Firma" auf Seite B-1054
- "Texte" auf Seite B-1188
- "Formulare" auf Seite B-1195
- "CEKAL" auf Seite B-1222
- "CE-Kennzeichen" auf Seite B-1233
- "B2B" auf Seite B-1237

> **i Schaltflächen in den Dialogen**
> Die Standard-Schaltflächen und -menüs sind ausführlich im Part **Übersicht** und in den Tutorials beschrieben. Auf sie wird daher in der Beschreibung der Dialoge nicht eingegangen.

---
*A+W Business Stammdaten*
*B-667*
---

# Allgemein

**Stammdaten > Allgemein**

In diesem Programmbereich sind allgemeine Daten hinterlegt.

Im Menü **Allgemein** finden Sie folgende Einträge:
- "Sprachen" auf Seite B-668
- "Monate" auf Seite B-670
- "Tage" auf Seite B-670
- "Landeskürzel" auf Seite B-671
- "Kalender" auf Seite B-672
- "Basisnummernkreise" auf Seite B-675

## Sprachen

**Stammdaten > Allgemein > Sprachen**

### Zu Dialogbeschreibung:
⇨ Preis-/Mengeneinheit für Mehrsprachigkeit

*(Abbildung B-351 zeigt den Dialog "Sprachen" mit einer Liste von Sprachen, ihrer internen Nummer, Bezeichnung, Fremdschlüssel und internationalem Kennzeichen.)*

In diesem Dialog tragen Sie alle Sprachen ein, in denen Sie mit Ihren Kunden in schriftlicher Form korrespondieren. An erster Stelle steht immer Ihre Korrespondenzsprache. Sie können diese nicht nachträglich ändern.

Dieser Dialog steht nur mit dem Modul Mehrsprachigkeit zur Verfügung.

### Menü Funktionen

Über dieses Menü können Sie den Dialog **Anlage Preis-/Mengeneinheit für Mehrsprachigkeit** öffnen, um die Bezeichnungen für Preis- und Mengeneinheiten in eine neu angelegte Sprache zu kopieren.
⇨ "Preis-/Mengeneinheit für Mehrsprachigkeit" auf Seite B-669

---
*A+W Business Stammdaten*
*B-668*
---

**Bezeichnung**: Name der Sprache.

**Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Produktion oder die Finanzbuchhaltung.

## Preis-/Mengeneinheit für Mehrsprachigkeit

**Stammdaten > Allgemein > Sprachen > Menü Funktionen > Einheiten kopieren**

*(Abbildung B-352 zeigt den Dialog "Anlage Preis-/Mengeneinheit für Mehrsprachigkeit" mit den Feldern Quellsprache und Zielsprache.)*

In diesem Dialog kopieren Sie die Bezeichnungen für Preis- und Mengeneinheiten in eine neu angelegte Sprache, wenn Sie das Modul Mehrsprachigkeit einsetzen. Anschließend müssen Sie diese Bezeichnungen in die neue Sprache übersetzen.

### Preis-/Mengeneinheit

**Quellsprache**: Standardmäßig wird die Basissprache vorgeschlagen. Sie können jede andere Sprache auswählen, in der die Preis- und Mengeneinheiten vorhanden sind.

**Zielsprache**: Zielsprache, in die die Preis- und Mengeneinheiten kopiert werden sollen.
Im Dialog **Preis/Menge** müssen anschließend Sie die Bezeichnungen in dem entsprechenden Sprachregister übersetzen.
⇨ "Preis- und Mengeneinheit" auf Seite B-824

---
*A+W Business Stammdaten*
*B-669*
---

## Monate

**Stammdaten > Allgemein > Monate**

*(Abbildung B-353 zeigt eine Liste der Monate mit Nummer, Bezeichnung und Fremdschlüssel.)*

Die Monatsnamen sind standardmäßig mit der Basissprache vorbelegt und sollten nicht geändert werden.

**Bezeichnung**: Name des Monats.
**Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für statistische Auswertungen.

## Tage

**Stammdaten > Allgemein > Tage**

*(Abbildung B-354 zeigt eine Liste der Wochentage mit Nummer, Bezeichnung und Fremdschlüssel.)*

Die Tagesnamen sind standardmäßig mit der Basissprache vorbelegt und sollten nicht geändert werden.

**Bezeichnung**: Name des Wochentags.
**Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für statistische Auswertungen.

---
*A+W Business Stammdaten*
*B-670*
---

## Landeskürzel

**Stammdaten > Allgemein > Landeskürzel**

*(Abbildung B-355 zeigt den Dialog "Landeskürzel" mit einer Liste von Ländern, ihrem Kürzel, Bezeichnung, MwSt-Rundung, Fremdschlüssel und internationalem Kennzeichen.)*

In diesem Dialog verwalten Sie die internationalen Landeskürzel und ordnen die Standardrundung für die Steuer zu.

**Landeskürzel**: Landeskürzel, z. B. D = Deutschland, F = Frankreich, USA = United States of America.
Das Kürzel weisen Sie im Dialog **Partnerverwaltung** Ihren Kunden und Lieferanten zu, damit die Texte in der Sprache des Partners angezeigt und gedruckt werden, z. B. die Mengeneinheiten.
⇨ "(Land, Provinz)" auf Seite B-889

**Bezeichnung**: Name des Landes, z. B. Deutschland, Frankreich.

**Rundung Mwst**: Sie können für jedes Land festlegen, auf welchen Wert die Mehrwertsteuer gerundet werden soll. Zum Beispiel bedeutet 1, dass auf den nächsten Wert auf- oder abgerundet wird, bei 5 wird auf die nächste 5 auf- oder abgerundet.
⇨ Tutorial 2, "Rundungen" auf Seite B-515
⇨ "Rundung (Kunde, Lieferant)" auf Seite B-970
⇨ "Rundung" auf Seite B-1015

**Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für statistische Auswertungen.

**Gesperrt**: Ein Landeskürzel kann für die Erfassung in der Partnerverwaltung und in den Dokumenten gesperrt werden, wenn es nicht mehr benötigt wird.
- ☐ Das Landeskürzel kann zugewiesen werden.
- ☑ Das Landeskürzel ist gesperrt und kann nicht mehr zugewiesen werden. Wenn es Partnern und in Dokumenten zugewiesen ist, wird es jedoch weiterhin angezeigt.

**Internationales Kennzeichen**: Zweistelliges internationales Landeskürzel, z. B. DE = Deutschland, FR = Frankreich, US = United States of America.

---
*A+W Business Stammdaten*
*B-671*
---

## Kalender

**Stammdaten > Allgemein > Kalender**

*(Abbildung B-356 zeigt den Kalenderdialog. Links ist die Arbeitswoche mit Stunden pro Wochentag definierbar. Rechts eine Übersicht der Tage der ausgewählten Kalenderwoche mit den Arbeitsstunden. Unten sind Schaltflächen zur Jahres- und KW-Auswahl sowie zum Übertragen von Einstellungen.)*

In diesem Dialog pflegen Sie die Feiertage und die täglichen Arbeitsstunden in Ihrem Unternehmen. Wenn im Feld **Stunden** ein Wert größer 0 steht, gilt dieser als Arbeitstag. Wenn Sie einen Tag als Feiertag definieren möchten, müssen Sie den Wert 0 eintragen.
⇨ Tutorial 1, "Allgemeinen Kalender anlegen" auf Seite B-163

### Arbeitswoche

**Wochentag**: Anzahl der regulären Arbeitsstunden für jeden Wochentag. Die Feiertage müssen Sie auf 0 (Stunden) setzen.
- ☐ Der Wochentag wird nicht in die Arbeitswoche aufgenommen.
- ☑ Der Wochentag wird in die Arbeitswoche aufgenommen.

### Auswahl

**Jahr, KW**: Auswahl des Jahres und der Kalenderwoche, um die entsprechende Kalenderwoche in der Übersicht anzuzeigen.

**[Auf Jahr übertragen]**: Überträgt die Änderungen auf alle entsprechenden Wochentage des gesamten Kalenderjahrs. Die Feiertage müssen Sie danach auf 0 setzen.

**[Auf KW übertragen]**: Überträgt die Änderungen auf alle Tage der aktuellen Kalenderwoche. Die entsprechenden Wochentage des restlichen Kalenderjahrs bleiben unverändert.

**[Zur aktuellen KW]**: Mit dieser Schaltfläche lassen Sie sich die aktuelle Kalenderwoche anzeigen.

---
*A+W Business Stammdaten*
*B-672*
---

### Übersicht

In der Übersicht werden alle Kalenderwochen des aktuellen Kalenderjahrs mit den Tagesarbeitszeiten angezeigt. Die Wochenenden sind in roter Schrift dargestellt.

---
*A+W Business Stammdaten*
*B-673*
---

## Länder Kalender

**Stammdaten > Allgemein > Länder Kalender**

*(Abbildung B-357 zeigt den Dialog "Länder Kalender". Man kann eine Provinz und ein Jahr auswählen. In einer Tabelle werden Kalender für verschiedene Provinzen/Jahre gelistet. In der Hauptansicht ("Übersicht") kann man für jeden Tag des Jahres festlegen, ob es ein Feiertag ist.)*

In diesem Dialog pflegen Sie die Feiertage in den Ländern und Provinzen, in denen die Unternehmen angesiedelt sind, mit denen Sie arbeiten.

### Identifikation

**Provinz**: Auswahl der Provinz, für die der Feiertagskalender gilt. Die Provinzen sind unter **Marktpartner > Allgemein** hinterlegt.
⇨ "Provinz" auf Seite B-880

**Jahr**: Auswahl des Jahres, in dem die Feiertage gelten.

**Land**: Auswahl des Landes, zu dem die Provinz gehört. Die Länder sind unter **Stammdaten > Allgemein** hinterlegt.
⇨ "Landeskürzel" auf Seite B-671

### Tabelle

In der Tabelle werden alle Kalender zu den Provinzen angezeigt, für die besondere Feiertage gelten.

### Übersicht

In der Übersicht werden alle Kalenderwochen des aktuellen Kalenderjahrs mit den Tagesarbeitszeiten angezeigt. Die Wochenenden sind in roter Schrift dargestellt.

---
*A+W Business Stammdaten*
*B-674*
---

## Basisnummernkreise

**Stammdaten > Allgemein > Basisnummernkreise**

*(Abbildung B-358 zeigt eine Liste von Stammdatentabellen, wie "Anreden", "Banken", "Branchen", etc., und zeigt für jede Tabelle die "Letzte Nummer" und "Höchste Nummer" an, die vergeben werden kann.)*

In diesem Dialog wird angezeigt, wie viele Datensätze Sie in der jeweiligen Stammdatentabelle anlegen können und wie viele Nummern bereits vergeben sind. Die Start- und Endnummern sind in der Regel fest vorgegeben und müssen nicht angepasst werden.

Diese Nummern können pro Datenbank (DB) gepflegt werden. D. h., dass sich die Nummernkreise der Master-DB und der Slave-DBs unterscheiden können. Diese Einstellungen werden nicht repliziert.

In den aufgeführten Stammdatendialogen ist die Anzahl der möglichen Datensätze auf die höchste Nummer begrenzt. Wenn weitere Datensätze angelegt werden sollen, müssen Sie die höchste Nummer erhöhen.

> **i Nummernkreise für Dokumente**
> Nummernkreise für die Dokumente legen Sie im Programmbereich **Auftrag** fest.
> ⇨ "Nummernkreise" auf Seite B-1028

---
*A+W Business Stammdaten*
*B-675*
---

### Übersicht

**Tabelle**: Namen der Stammdatentabellen, zu denen Nummernkreise geführt werden.

**Letzte Nummer**: Nummer des Datensatzes, die in diesem Nummernkreis zuletzt vergeben wurde.

**Höchste Nummer**: Höchste Nummer, die in diesem Nummernkreis vergeben werden kann.

---
*A+W Business Stammdaten*
*B-676*
---

# Produkte

**Stammdaten > Produkte**

In diesem Programmbereich definieren Sie die allgemeinen Daten für die Verwaltung von Produkten und die Produktstammdaten.

Im Menü **Produkte** finden Sie folgende Einträge:
- "Allgemein" auf Seite B-677
- "Artikel" auf Seite B-753

## Allgemein

**Stammdaten > Produkte > Allgemein**

In diesem Programmbereich sind die allgemeinen Daten zu den Produkten hinterlegt.

Im Menü **Allgemein** finden Sie folgende Einträge:
- "Produktarten" auf Seite B-678
- "Produktgruppen" auf Seite B-679
- "WGR" auf Seite B-680
- "Kombi-WGR" auf Seite B-682
- "Top-WGR" auf Seite B-684
- "Varianten" auf Seite B-685
- "Sprossentypen" auf Seite B-687
- "Reklamationsverursacher" auf Seite B-689
- "Reklamationsgrund" auf Seite B-690
- "Struktur" auf Seite B-691
- "Strukturseite" auf Seite B-692
- "Beschichtungsseite" auf Seite B-693
- "Beschichtungsart" auf Seite B-694
- "Glasartgruppen" auf Seite B-695
- "Gütetext" auf Seite B-696
- "Leistungserklärung Verwaltung" auf Seite B-698
- "Austauschgruppen" auf Seite B-699
- "Austauschzuordnung" auf Seite B-700
- "Klassifikatoren - Produkt" auf Seite B-701

---
*A+W Business Stammdaten*
*B-677*
---

## Produktarten

**Stammdaten > Produkte > Allgemein > Produktarten**

*(Abbildung B-359 zeigt den Dialog "Produktarten" mit einer Liste vordefinierter Produktarten wie Einfachglas, ESG, VSG, Isolierglas etc.)*

In diesem Dialog werden die Produktarten angezeigt, die in A+W Business zur Verfügung stehen. Sie können diese nicht umbenennen oder ergänzen.
⇨ Tutorial 1, "Produktarten und Produktgruppen" auf Seite B-202

**Bezeichnung**: Name der Produktart.

**Schlüssel**: Schlüsselnummer (ID), mit der die Produktart im System eindeutig identifiziert wird.

**Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Produktion.

**Gesperrt**: Eine Produktart kann für die Erfassung in der Produktverwaltung und in den Dokumenten gesperrt werden, wenn sie nicht mehr benötigt wird.
- ☐ Die Produktart kann zugewiesen werden.
- ☑ Die Produktart ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie Produkten und in Dokumenten zugewiesen ist, wird sie jedoch weiterhin angezeigt.

> **i Produktarten erweitern**
> Wenn Sie weitere Produktarten benötigen, sprechen Sie Ihren Service-Mitarbeiter bei der A+W Software GmbH an.

---
*A+W Business Stammdaten*
*B-678*
---

## Produktgruppen

**Stammdaten > Produkte > Allgemein > Produktgruppen**

*(Abbildung B-360 zeigt den Dialog "Produktgruppen", in dem verschiedene Produktgruppen (z.B. Abstandhalter, Artikel, Bearbeitungen) aufgelistet sind. Für jede Gruppe werden Produktart, Bezeichnung, Schlüssel und Fremdschlüssel angezeigt.)*

In diesem Dialog pflegen Sie die Produktgruppen, mit denen Sie in A+W Business arbeiten. Den Namen einer neuen Produktgruppe können Sie frei wählen. Anschließend ordnen Sie die Produktart zu.
⇨ Tutorial 1, "Produktarten und Produktgruppen" auf Seite B-202

**Produktart**: Produktart, die einer Produktgruppe zugeordnet ist.

**Bezeichnung**: Name der Produktgruppe.

**Schlüssel**: Schlüsselnummer, über die die Produktgruppe in System eindeutig identifiziert wird.

**Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Produktion.

**Schlüssel A+W Production**: Fremdschlüssel, der für den Datenaustausch mit A+W Production genutzt wird. Dieser Schlüssel muss auch in A+W Production bei der entsprechenden Produktgruppe hinterlegt sein.

**Gesperrt**: Eine Produktgruppe kann für die Erfassung in der Produktverwaltung und in den Dokumenten gesperrt werden, wenn sie nicht mehr benötigt wird.
- ☐ Die Produktgruppe kann zugewiesen werden.
- ☑ Die Produktgruppe ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie Produkten und in Dokumenten zugewiesen ist, wird sie jedoch weiterhin angezeigt.

---
*A+W Business Stammdaten*
*B-679*
---

## WGR

**Stammdaten > Produkte > Allgemein > WGR**

*(Abbildung B-361 zeigt den Dialog "Warengruppen". Links ist eine Baumstruktur der Warengruppen (WHG, WOG, WGR) zu sehen. Rechts werden die Details der ausgewählten Warengruppe angezeigt, wie Nummer, Bezeichnung, Vorlauftage, etc.)*

In diesem Dialog verwalten Sie die Warengruppen, mit denen Sie in A+W Business arbeiten. Die Warengruppen werden in drei Ebenen klassifiziert:
- Warenhauptgruppe (WHG)
- Warenobergruppe (WOG)
- Warengruppe (WGR)

Die Abkürzung wird WGR auch für Warengruppen im Allgemeinen verwendet.

Die WHG 0\*\*, WOG 00\* und WGR 000 sind fest angelegt.

Der Warengruppe 000 werden in der Regel nur Modelle zugeordnet. So kann in der Statistik z. B. der Modellumsatz automatisch dem Umsatz des Hauptproduktes zugeordnet werden.

Sprossen und Bearbeitungen haben in der Regel eine eigene Warengruppe.
⇨ Tutorial 1, "Warengruppen" auf Seite B-204

> **i Kombi-Warengruppen**
> Wenn Sie mit Kombi-Warengruppen arbeiten möchten, müssen Sie diese wie jede andere WGR anlegen. Im Dialog **Kombi-WGR** können Sie dann die gewünschten Warengruppen kombinieren und zuordnen.
> ⇨ "Kombi-WGR" auf Seite B-682

---
*A+W Business Stammdaten*
*B-680*
---

### Warengruppe

**Nummer**: Nummer der WGR. Sie können je nach Ebene bis zu 3 Stellen alphanumerisch angeben, z. B. 1AT.

**Vorlauftage**: Vorlauftage für die Berechnung des Versandtags. Dies gilt nur für Bestellartikel.
Der Wert gibt an, wie viele Tage ein Bestellartikel im Voraus beim Lieferanten bestellt werden muss, damit der Artikel rechtzeitig zur Produktion bereitsteht.

**Bezeichnung**: Eindeutiger Name der WGR.

**Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Produktion oder die Finanzbuchhaltung.
Mit Hilfe eines Fremdschlüssels können Preise nach Warengruppen berechnet werden. Im Dialog zur Preisdefinition können Sie ihn für den Grenztyp **WGR Fremdkey** einsetzen.
⇨ "Preise" auf Seite B-839

> **i Exakte Grenzmenge für WGR-Fremdkey**
> Um eine exakte Grenzmenge für den WGR-Fremdkey zu haben, steht die Grenzmenge **140 WGR Fremdkey exakt** zur Verfügung. Die entsprechende Funktion kann in den Firmendaten aktiviert werden.
> ⇨ "WGR-Fremdkey als nicht exakte Grenzmenge berechnen" auf Seite B-1094

### Kosten und Aufschlagskalkulation

**Sonderzuschlag**: Prozentualer Zuschlag für eine Warengruppe. Dieser Sonderzuschlag wird bei der Berechnung der Selbstkosten berücksichtigt und entsprechend ausgewiesen.

**Steuercode**: Zur Steuerberechnung können die Daten an den Avalara Web-Service übergeben werden. Für die korrekte Steuerberechnung müssen sogenannte Steuercodes zu jeder Warengruppe eingetragen werden. Während der Übergabe wird für jede Position der Steuercode anhand der Kombi-Warengruppe des Hauptproduktes ermittelt und an Avalara übergeben.
Die Zugangsdaten müssen in den Firmendaten eingerichtet werden.
⇨ "Firmendaten - Steuer" auf Seite B-1058

**Bitmap**: Piktogramme, die einer WGR zugeordnet werden können. So können Sie die Produktart oder -gruppe schnell erkennen.

**Top-Warengruppen**: Top-Warengruppen aus dem Dialog Top-WGR. Sie können eine Warengruppe nur auf Warengruppenebene (WGR), nicht auf Warenhaupt- oder Warenobergruppenebene einer Top-Warengruppe zuordnen.
- ☐ Die Warengruppe ist nicht zugeordnet.
- ☑ Die Warengruppe ist der Top-WGR zugeordnet.
⇨ Tutorial 1, "Top-WGR" auf Seite B-211
⇨ "Top-WGR" auf Seite B-684

---
*A+W Business Stammdaten*
*B-681*
---

## Kombi-WGR

**Stammdaten > Produkte > Allgemein > Kombi-WGR**

*(Abbildung B-362 zeigt den Dialog "WGR-Kombinationen". In einer Tabelle werden Kombinationen aus zwei Ausgangswarengruppen (Warengruppe 1, Warengruppe 2) einer Kombinationswarengruppe zugeordnet. Es gibt Checkboxen für "gültig für Rabattfindung" und "gültig für Statistik".)*

In diesem Dialog legen Sie Kombi-Warengruppen (Kombi-WGR) an. Wenn Sie in der Übersicht eine Zeile markieren, werden die entsprechenden Werte in den Feldern angezeigt und können bearbeitet werden.
⇨ Tutorial 1, "Regeln für Kombi-WGR" auf Seite B-206
⇨ Tutorial 1, "Warengruppen kombinieren" auf Seite B-214

### Ausgangswarengruppen

**Warengruppe 1, 2**: Erste und zweite Warengruppe, die miteinander kombiniert sind. Hier sind alle Warengruppenebenen erlaubt.

### Kombinationswarengruppen

**Warengruppe**: Kombi-WGR, nach deren Regeln die Warengruppe 1 und Warengruppe 2 kombiniert werden sollen.
Die möglichen Kombi-WGR müssen im Dialog WGR angelegt sein.
⇨ "WGR" auf Seite B-680

**Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für statistische Auswertungen.

---
*A+W Business Stammdaten*
*B-682*
---

**Gültig für Rabattfindung**: Sie können angeben, ob die Kombi-WGR bei der Berechnung des Rabattes berücksichtigt werden soll.
- ☐ Die Kombi-WGR wird nicht bei der Berechnung des Preises berücksichtigt.
- ☑ Die Kombi-WGR wird bei der Preis- und Rabattfindung berücksichtigt. Die Checkbox **Kombi-Rabatt nur auf Hauptposition bilden** wird freigeschaltet.

**Gültig für Statistik**: Sie können angeben, ob die Kombi-WGR in der Statistik berücksichtigt werden soll.
- ☐ Die Kombi-WGR wird nicht in der Statistik berücksichtigt.
- ☑ Die Kombi-WGR wird in der Statistik berücksichtigt. Die Checkbox **Kombi-Statistik nur auf Hauptposition bilden** wird freigeschaltet.

**Kombi-Rabatt nur auf Hauptposition bilden**: Diese Checkbox ist nur freigeschaltet, wenn die Checkbox **Gültig für Rabattfindung** aktiviert wurde.
- ☐ Der gesamte Umsatz des Floats und der Bearbeitung wird zur Rabattfindung herangezogen.
- ☑ Nur die Hauptposition wird zur Rabattfindung herangezogen.

**Beispiel Kombiwarengruppe: 100 + 400 = 401**

| Produkt | WGR | Ergebnis Kombi-WGR |
| :--- | :--- | :--- |
| | | ☐ | ☑ |
| Float | 100 | 401 | 401 |
| Bearbeitung | 400 | 401 | 400 |

**Kombi-Statistik nur auf Hauptposition bilden**: Diese Checkbox ist nur freigeschaltet, wenn die Checkbox **Gültig für Statistik** aktiviert wurde.
- ☐ Der gesamte Umsatz des Floats und der Bearbeitung wird auf die Kombi-Warengruppe gebucht.
- ☑ Sie können in der Auswertung unterscheiden, wie viel Float mit und ohne Bearbeitung produziert wurde. Der Umsatz für die Bearbeitung selbst wird jedoch separat verbucht.

### Übersicht

In der Übersicht werden die angelegten Kombi-WGR aufgelistet.

---
*A+W Business Stammdaten*
*B-683*
---

## Top-WGR

**Stammdaten > Produkte > Allgemein > Top-WGR**

*(Abbildung B-363 zeigt den Dialog "Top-WGR" mit einer Liste von Top-Warengruppen, die eine Nummer, Bezeichnung und einen Fremdschlüssel haben.)*

In diesem Dialog legen Sie Top-Warengruppen (Top-WGR) an. In der Umsatzstatistik können Sie Auswertungen für diese Top-Warengruppen erstellen.

**Bezeichnung**: Name der Top-Warengruppe. Im Dialog WGR können Sie die gewünschte Warengruppe zuordnen.
⇨ "WGR" auf Seite B-680

**Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für statistische Auswertungen.

---
*A+W Business Stammdaten*
*B-684*
---

## Varianten

**Stammdaten > Produkte > Allgemein > Varianten**

*(Abbildung B-364 zeigt den Dialog "Varianten", in dem Farben für Produktvarianten definiert werden. Die Liste enthält Spalten für Variante, Bezeichnung, Fremdschlüssel, Farbauswahl, Vorschau und Optionen wie Sonderfarbe und Gesperrt.)*

In diesem Dialog hinterlegen Sie die Farben, die Sie für die Definition von Produktvarianten verwenden können.
⇨ "Produktvarianten" auf Seite B-760

**Sprache**: Auswahl der Sprache, wenn Sie mit der Mehrsprachigkeit arbeiten. Verwenden Sie in allen Sprachen dieselben Schlüssel. Die Bezeichnung kann übersetzt werden.

**Variante**: Interne Nummer der Farbe. Diese Nummer benötigen Sie für die Zuordnung der Farbe zur Produktvariante.

**Bezeichnung**: Name der Farbe.

**Fremdschlüssel**: Bei Dorma-Artikeln der Dorma-Farbschlüssel. Der Fremdschlüssel kann für die Kommunikation mit anderen Programmen verwendet werden, z. B. für die Übergabe an die Produktion.

**Farbauswahl**: Öffnet den Dialog **Farbe**, um die Farbe festzulegen, in der z. B. die Sprossen in der Positionserfassung angezeigt werden. Die Farbe wird nicht an die Produktion übergeben.

**Vorschau**: Anzeige der gewählten Farbe.

---
*A+W Business Stammdaten*
*B-685*
---

**Sonderfarbe**: Im Auftrag kann bei bestimmten Produkten eine Sonderfarbe verwendet werden, z. B. beim Siebdruck.
- ☐ Die Farbe wird nicht als Sonderfarbe verwendet.
- ☑ Bei dieser Einstellung kann im Auftrag angegeben werden, welche Farbe verwendet werden soll.

**Beispiel**
In einem Auftrag soll für einen Kunden ein Siebdruck mit einem bestimmten Motiv erfasst werden, z. B. ein Formel 1-Fahrzeug.
Für diesen Fall muss eine Variante mit dem Kennzeichen **Sonderfarbe** für das Produkt Siebdruck angelegt sein. In der Positionserfassung wählen Sie dann für die Bearbeitung Siebdruck diese Produktvariante aus. Dadurch wird ein weiteres Feld angezeigt, in dem Sie den Namen des Motivs angegeben können. Dieser Name wird an die Produktion übergeben.

**Gesperrt**: Eine Variante kann für die Erfassung in der Produktverwaltung und in den Dokumenten gesperrt werden, wenn sie nicht mehr benötigt wird.
- ☐ Die Variante kann zugewiesen werden.
- ☑ Die Variante ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie Produkten und in Dokumenten zugewiesen ist, wird sie jedoch weiterhin angezeigt.

---
*A+W Business Stammdaten*
*B-686*
---

## Sprossentypen

**Stammdaten > Produkte > Allgemein > Sprossentypen**

*(Abbildung B-365 zeigt den Dialog "Sprossentypen" mit einer Liste definierter Typen. Spalten umfassen Typ, Bezeichnung, Randstopfenmaß, Kennz. Durchgang, Frästiefe, etc.)*

In diesem Dialog definieren Sie die Sprossentypen. Jeder Sprosse wird in der Produktverwaltung ein Sprossentyp zugeordnet.
⇨ "Konstruktionstyp" auf Seite B-714

> **i Neue Sprossentypen**
> Wenn Sie mit A+W Production arbeiten, müssen Sie neue Sprossentypen mit Ihrem Service-Mitarbeiter der A+W Software GmbH absprechen.

**Typ**: Interne Nummer. Diese Nummer muss mit der Nummer in der Produktionssoftware übereinstimmen.

**Bezeichnung**: Name des Sprossentyps.

**Randstopfenmaß**: Wert für das Randstopfenmaß in mm. Das Randstopfenmaß wird bei der Preisberechnung der Sprossenkonstruktion ausgewertet.
⇨ Verkauf, "Gitter" auf Seite C-1777

**Kennz. Durchgang**: Angabe zur Verbindung mit anderen Sprossen:
- **0 - keine**: Das Kennzeichen ist nicht gesetzt, Sprossen des Typs können beliebig verarbeitet werden.
- **1 - waagerecht**: Waagerechte Sprossen des Typs müssen durchgängig sein.
- **2 - senkrecht**: Senkrechte Sprossen des Typs müssen durchgängig sein.
- **3 - waagerecht + senkrecht**: Waagerechte und senkrechte Sprossen des Typs müssen durchgängig sein.

---
*A+W Business Stammdaten*
*B-687*
---

- **6 - überlappend**: Waagerechte und senkrechte Sprossen des Typs können sich überlappen.
- **7 - längste Sprosse**: Die längste Sprosse des Typs muss durchgängig sein.
⇨ Tutorial 1, "Konstruktionstypen der Sprossen" auf Seite B-227

**Frästiefe**: Tiefe des Einschnitts im Abstandhalter.

**Spezialkreuzung**: Bei einigen Sprossentypen sind Spezialkreuze für die Verbindung erforderlich.
- ☐ Für den Sprossentyp wird kein Spezialkreuz verwendet.
- ☑ Für den Sprossentyp muss ein Spezialkreuz verwendet werden. Zusätzlich muss die Breite angegeben werden. Bei dieser Einstellung müssen das Kennzeichen für den Durchgang und die Fräßtiefe auf 0 (keine) stehen.

**Breite Spezialkreuz, 0=Sprossenbreite**: Breite des Spezialkreuzes im mm. Der Wert 0 zeigt an, dass die Breite des Spezialkreuzes sich nach der Sprossenbreite richtet.

---
*A+W Business Stammdaten*
*B-688*
---

## Reklamationsverursacher

**Stammdaten > Produkte > Allgemein > Reklamationsverursacher**

*(Abbildung B-366 zeigt den Dialog "Reklamationsverursacher" mit einer Liste von möglichen Verursachern wie "Büro", "Produktion", "Fahrer".)*

In diesem Dialog hinterlegen Sie die Verursacher einer Reklamation. Die Werte können beim Erfassen einer Reklamation ausgewählt werden. Sie werden durch das Modul **Reklamationsstatistik** ausgewertet.

**Bezeichnung**: Name des Verursachers, z. B. Produktion, Auftragserfassung, Versand. Die Bezeichnung soll sich deutlich vom Reklamationsgrund unterscheiden.
⇨ "Reklamationsgrund" auf Seite B-690

**Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Finanzbuchhaltung oder für statistische Auswertungen.

**Gesperrt**: Ein Reklamationsverursacher kann für die Erfassung in den Dokumenten gesperrt werden, wenn er nicht mehr benötigt wird.
- ☐ Der Reklamationsverursacher kann zugewiesen werden.
- ☑ Der Reklamationsverursacher ist gesperrt und kann nicht mehr zugewiesen werden. Wenn er in Dokumenten zugewiesen ist, wird er jedoch weiterhin angezeigt.

---
*A+W Business Stammdaten*
*B-689*
---

## Reklamationsgrund

**Stammdaten > Produkte > Allgemein > Reklamationsgrund**

*(Abbildung B-367 zeigt den Dialog "Reklamationsgrund" mit einer Liste von Gründen wie "Produktionsfehler", "Materialfehler", "Bruch".)*

In diesem Dialog hinterlegen Sie die Gründe, die zu einer Reklamation geführt haben.
⇨ "Reklamationsverursacher" auf Seite B-689

**Bezeichnung**: Name für den Reklamationsgrund, z. B. Materialfehler, Produktionsfehler, Bruch.

**Kombi-WGR**: Kombi-WGR für die Auswertung. Über Kombi-WGR können die Stückzahlen ausgewertet werden, die aufgrund von Reklamationen produziert wurden.
In der Reklamationsstatistik im Modul **Statistik** wird auch der entgangene Umsatz ausgewertet.

**Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Finanzbuchhaltung oder für statistische Auswertungen.

**Gesperrt**: Ein Reklamationsgrund kann für die Erfassung in den Dokumenten gesperrt werden, wenn er nicht mehr benötigt wird.
- ☐ Der Reklamationsgrund kann zugewiesen werden.
- ☑ Der Reklamationsgrund ist gesperrt und kann nicht mehr zugewiesen werden. Wenn er in Dokumenten zugewiesen ist, wird er jedoch weiterhin angezeigt.

---
*A+W Business Stammdaten*
*B-690*
---

## Struktur

**Stammdaten > Produkte > Allgemein > Struktur**

*(Abbildung B-368 zeigt den Dialog "Struktur", der die möglichen Strukturverläufe von Gläsern definiert: keiner, senkrecht, waagerecht, beliebig.)*

In diesem Dialog werden die möglichen Strukturverläufe der Gläser angezeigt. Sie können die Einträge bearbeiten, jedoch nicht um weitere Verläufe ergänzen.

**Schlüssel**: Der Schlüssel (ID) ist von A+W Business vorgegeben und darf nicht verändert werden.

**Kurzbez.**: Einstellige alphanumerische Kurzbezeichnung, die geändert werden kann.

**Beispiel**
- S = senkrecht oder V = vertikal
- W = waagrecht oder H = horizontal

**Bezeichnung**: Eindeutiger Name für den Strukturverlauf.

---
*A+W Business Stammdaten*
*B-691*
---

## Strukturseite

**Stammdaten > Produkte > Allgemein > Strukturseite**

*(Abbildung B-369 zeigt den Dialog "Strukturseite" mit einer Liste der Ebenen (Seiten im ISO-Aufbau), z.B. Ebene 1, Ebene 2, etc.)*

In diesem Dialog werden die möglichen Strukturseiten angezeigt. Sie können die Einträge bearbeiten und ergänzen, um bei Mehrfach-ISO oder VSG alle Seiten angeben zu können. Dabei hat jede Scheibe im ISO oder VSG zwei Seiten, die jeweils innen oder außen liegen.
⇨ Tutorial 1, "Strukturen und Beschichtungen" auf Seite B-225

**Ebene**: Die Nummern der Ebenen (Seiten im ISO-Aufbau) dürfen nicht verändert werden. Wenn Sie weitere Ebenen anlegen, wählen Sie fortlaufenden Nummern nach demselben Prinzip.

**Kurzbez.**: Einstellige alphanumerische Kurzbezeichnung für die Innen- und die Außenseite. Sie können sie ändern.

**Bezeichnung**: Eindeutiger Name der Ebene.

---
*A+W Business Stammdaten*
*B-692*
---

## Beschichtungsseite

**Stammdaten > Produkte > Allgemein > Beschichtungsseite**

*(Abbildung B-370 zeigt den Dialog "Beschichtungsseite", der identisch zum Dialog "Strukturseite" aussieht und die Ebenen (Seiten im ISO-Aufbau) auflistet.)*

In diesem Dialog werden die möglichen Beschichtungsseiten angezeigt. Sie können die Einträge bearbeiten und ergänzen, um bei mehrfach ISO alle Ebenen angeben zu können. Dabei hat jede Scheibe im ISO zwei Seiten, die jeweils innen oder außen liegen.
⇨ Tutorial 1, "Strukturen und Beschichtungen" auf Seite B-225

**Ebene**: Die Nummern der Ebenen dürfen nicht verändert werden. Wenn Sie weitere Ebenen anlegen, wählen Sie fortlaufende Nummern nach demselben Prinzip.

**Kurzbez.**: Einstellige alphanumerische Kurzbezeichnung für die Innen- und die Außenseite. Sie können sie ändern.

**Bezeichnung**: Eindeutiger Name der Ebene.

---
*A+W Business Stammdaten*
*B-693*
---

## Beschichtungsart

**Stammdaten > Produkte > Allgemein > Beschichtungsart**

*(Abbildung B-371 zeigt den Dialog "Beschichtungsart" mit den Optionen "nicht beschichtet", "beschichtet", "weich beschichtet", "hart beschichtet".)*

In diesem Dialog werden die möglichen Beschichtungsarten angezeigt. Sie können die Einträge bearbeiten und ergänzen.
⇨ Tutorial 1, "Strukturen und Beschichtungen" auf Seite B-225

**Schlüssel**: Der Schlüssel ist von A+W Business vorgegeben und darf nicht verändert werden.

**Kurzbez.**: Einstellige alphanumerische Kurzbezeichnung.

**Beispiel**
N = nicht beschichtet oder O = ohne

**Bezeichnung**: Eindeutiger Name der Beschichtungsart.

---
*A+W Business Stammdaten*
*B-694*
---

## Glasartgruppen

**Stammdaten > Produkte > Allgemein > Glasartgruppen**

*(Abbildung B-372 zeigt den Dialog "Glasartgruppen" mit einer Liste von Gruppen wie Floatglas, Isolierglas, ESG, VSG etc. mit zugehörigem Schlüssel.)*

In diesem Dialog hinterlegen Sie die Glasartgruppen. Glasartgruppen benötigen Sie, wenn Sie mit A+W Production arbeiten. Die Glasartgruppen von A+W Production entsprechen den Produktarten von A+W Business.

**Beispiel**
- 1 = Float
- 2 = Isolierglas
- 3 = ...

Jedem Glasprodukt kann in der Produktverwaltung über das Register **A+W Production** eine Glasart und eine Glasartgruppe zugeordnet werden. Die Definition von Glasartgruppen dient in A+W Production zur Auswertung in Reports und in der Statistik. Für den Produktionslauf haben die Glasartgruppen keine Bedeutung.
⇨ "Glasarten" auf Seite B-752

**Bezeichnung**: Name der Glasartgruppe, z. B. Float, ESG, VSG.

**Schlüssel**: 1- bis 7-stellige Nummer der Glasartgruppe.

---
*A+W Business Stammdaten*
*B-695*
---

## Gütetext

**Stammdaten > Produkte > Allgemein > Gütetext**

Gütetexte werden abhängig vom ISO-Aufbau und Landeskennzeichen der Lieferadresse in den Rahmentext eingefügt.

> **i Voraussetzung**
> Der Dialog kann nur geöffnet werden, wenn in den **Firmendaten > Register Dokumente** die entsprechende Funktion ausgewählt ist.
> ⇨ "Produktkennzeichnung" auf Seite B-1071

Im Dialog **Gütetext** finden Sie folgende Register:
- Gütetext – Grundeinstellungen
- Gütetext – Restriktionen

### Gütetext – Grundeinstellungen

**Stammdaten > Produkte > Allgemein > Gütetext > Register Grundeinstellungen**

*(Abbildung B-373 zeigt den Gütetext-Dialog. Man kann ein Glas und ein Gas auswählen und dann für eine bestimmte Priorität und ein Land einen spezifischen Text definieren.)*

In diesem Register hinterlegen Sie die (landesspezifischen) Gütetexte, die in die Rahmentexte eingefügt werden sollen.
⇨ Tutorial 2, "Textarten" auf Seite B-535

#### Produktauswahl

**Glas**: Glasartikel, für den ein Gütetext definiert ist.
**Gas**: Gas in der ISO-Scheibe.

---
*A+W Business Stammdaten*
*B-696*
---

#### Werte

**Priorität**: Über die Priorität legen Sie fest, welcher Gütetext genommen wird, falls in einer ISO-Einheit unterschiedliche Gläser enthalten sind, für die jeweils ein Gütetext erfasst ist.

**Land**: Die Gütetextanforderungen können sich von Land zu Land unterscheiden. Mit Hilfe des Landeskennzeichens können Sie für ein Glas unterschiedliche Texte pro Land definieren.

**Text**: Gütetext, der in den Rahmen gedruckt wird.

### Gütetext – Restriktionen

**Stammdaten > Produkte > Allgemein > Gütetext > Register Restriktionen**

*(Abbildung B-374 zeigt das Register "Restriktionen". Hier können Regeln definiert werden, die die Verwendung des Gütetextes einschränken, z.B. "Produktgruppe [PGS1] darf nicht vorhanden sein".)*

In diesem Register können Sie die automatische Verwendung des Gütetextes einschränken. Über eine Regel legen Sie fest, bei welchen Produktarten oder Produktgruppen der Gütetext nicht verwendet wird.

Die Felder im Bereiche **Produktauswahl** sind zum Register **Grundeinstellungen** beschrieben.
⇨ "Gütetext - Grundeinstellungen" auf Seite B-696

#### Gültigkeitsbereich

**Regel**: Die verfügbaren Regeln sind vom Programm vorgegeben.

**Parameter 1 - 4**: Die Anzahl der änderbaren Parameter hängt von der ausgewählten Regel ab.

---
*A+W Business Stammdaten*
*B-697*
---

### Restriktionen

In der Übersicht werden für das ausgewählte Glas alle Regeln mit den zugehörigen Parametern aufgelistet.

## Leistungserklärung Verwaltung

**Stammdaten > Produkte > Allgemein > Leistungserklärung Verwaltung**

*(Abbildung B-375 zeigt den Dialog "Leistungserklärung Verwaltung". Hier werden Leistungserklärungen mit Nummer und Bezeichnung verwaltet. Man kann sprachspezifische Dateianhänge (Links) hinzufügen.)*

In diesem Dialog verwalten Sie die Vorlagen für die Leistungserklärungen. Mit der Kombination von **Nummer**, **Bezeichnung** und **Sprache** haben Sie die Möglichkeit, eine Leistungserklärung in verschiedenen Sprachen mit derselben Nummer zu registrieren.

Zur Erstellung von Leistungserklärungen können die technischen Text in allen erforderlichen Sprachen hinterlegt werden.
⇨ "Technische Werte" auf Seite B-1194

Der Versand von Leistungserklärungen kann pro Kunde und Produkt aktiviert werden.

### Leistungserklärung

**Nummer**: Nummer der Leistungserklärung.
**Bezeichnung**: Name der Leistungserklärung. Er sollte eindeutig und sprechend sein.

---
*A+W Business Stammdaten*
*B-698*
---

### Dateianhang

**Sprache**: Sprache, in der die Leistungserklärung abgefasst ist.

**Link**: Pfad, in dem die Leistungserklärungen abgelegt sind. Standardmäßig liegen die Leistungserklärungen in demselben Verzeichnis, in dem die Dateianhänge abgelegt sind. Dieses Verzeichnis legen Sie in den Firmendaten fest.
⇨ "Dateianhänge" auf Seite B-1071

**[Hinzufügen]**, **[Entfernen]**: Über diese Schaltflächen stellen Sie eine sprachliche Version der Leistungserklärungen zur Verfügung oder entfernen sie aus der Auswahl.

### Übersicht

In der Übersicht sind alle Leistungserklärungen aufgeführt, die den Produkten oder Kunden zugeordnet werden können.

## Austauschgruppen

**Stammdaten > Produkte > Allgemein > Austauschgruppen**

*(Abbildung B-376 zeigt den Dialog "Austauschgruppen" mit einer Liste von Gruppen, die eine Nummer und eine Bezeichnung haben, z.B. "100 Float", "400 Tempered Glass".)*

In diesem Dialog legen Sie die Austauschgruppen fest. Diesen Gruppen müssen Sie die Produkte zuordnen, die für den Austausch zugelassen sind.
⇨ "Austauschzuordnung" auf Seite B-700

Mit diesen Definitionen legen Sie fest, dass in ISO und/oder VSG nur Gläser, Abstandhalter und Folien eingebaut werden können, die für diese Produkte vorgesehen oder geeignet sind.

Die Funktion müssen Sie in den Firmendaten aktivieren.
⇨ "Produktaustauschregeln für Stücklistenaustausch verwenden" auf Seite B-1083

In den Stammdaten der Produkte mit Stückliste müssen Sie die gültige Gruppe angeben:
⇨ "Produktverwaltung - Stückliste" auf Seite B-731

**Nummer**: Nummer der Austauschgruppe.
**Bezeichnung**: Bezeichnung der Austauschgruppe.

---
*A+W Business Stammdaten*
*B-699*
---

## Austauschzuordnung

**Stammdaten > Produkte > Allgemein > Austauschzuordnung**

*(Abbildung B-377 zeigt den Dialog "Austauschzuordnung". Hier wird einem Produkt eine Austauschgruppe zugeordnet. Eine Tabelle listet bestehende Zuordnungen auf.)*

In diesem Dialog ordnen Sie die Produkte einer Austauschgruppe zu. Damit legen Sie fest, welche Produkte für den Austausch verwendet werden dürfen.

In den Stammdaten der Produkte mit Stückliste können Sie die Gruppe mit den zulässigen Produkten angeben.
⇨ "Produktverwaltung - Stückliste" auf Seite B-731

Mit diesen Definitionen legen Sie fest, dass in ISO und/oder VSG nur Gläser, Abstandhalter und Folien eingebaut werden können, die für diese Produkte vorgesehen oder geeignet sind.

Die Funktion müssen Sie in den Firmendaten aktivieren.
⇨ "Produktaustauschregeln für Stücklistenaustausch verwenden" auf Seite B-1083

### Neuanlage

**Gruppe**: Bezeichnung der Austauschgruppe. Das Feld ist nur freigeschaltet, wenn Sie einer Gruppe ein Produkt zuordnen. Neue Austauschgruppen legen Sie im Dialog **Austauschgruppen** an.
⇨ "Austauschgruppen" auf Seite B-699

**Produkt**: Produkt, das der Austauschgruppe zugeordnet ist.

---
*A+W Business Stammdaten*
*B-700*
---
