---
title: "DE_AWBusiness_Stammdaten_9_1"
source: "DE_AWBusiness_Stammdaten_9_1.pdf"
tags: ["A+W Business", "Stammdaten", "Master Data", "ERP", "Glass Industry", "Windows", "Doors", "Software Tutorial", "Kundendaten", "Produktdaten"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a tutorial and reference guide for the master data module (Stammdaten) of A+W Business, an ERP software for the glass, windows, and doors industry. It covers the creation and management of customer, supplier, product, and financial data."
long_description: "This document serves as a comprehensive guide to the 'Stammdaten' (Master Data) module within the A+W Business software suite. It is intended for end-users responsible for setting up and maintaining the foundational data of the ERP system. The guide is structured into a preface, two tutorials, and a software reference section. The first tutorial, which is the main focus of this document, provides a step-by-step introduction to creating and managing core data entities. This includes detailed instructions on handling market partners (customers, suppliers), address data, order and invoicing rules, employee and branch information, text management, and financial settings like credit limits, calendars, and payment terms. It uses a combination of conceptual explanations, procedural guides, screenshots, and diagrams to facilitate understanding. The document explains the logical connections between different data types and their impact on business processes such as sales, purchasing, and production planning. It also covers the setup of basic tables, the use of classifiers for data segmentation, and the configuration of pricing, discounts, and charges."
---

# A+W Stammdaten B

**A+W - Software for Glass, Windows and Doors**

---
## Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part | Version/Datum | Beschreibung |
| :--- | :--- | :--- |
| Vorspann | 9.00/04-2020 | Überarbeitung der Firmendaten. Neu: Bruchgründe, Produktklassifikatoren, Länder Kalender, ITOE-Regeln, Lieferantenkartei-Bedingungen, Gründe Lieferterminverschiebung, Statusverwaltung pro Mitarbeitergruppe, Dateianhangs-Bemerkungen, Technische Werte (für Leistungserklärung), B2B-Preisimport. |
| | 8.31/05-2018 | Überarbeitung der Firmendaten – Archivierungsmodus. |
| | 8.30/07-2017 | Dialoge Motive, Modellkantenqualitäten, Beschlagszuordnung neu. |
| | 8.21/02-2017 | Rechtschreibkorrekturen. |
| | 8.20/01-2017 | Dialoge Lagerdefintion und Firmendaten aktualisiert. Dialoge Austauschgruppen und Austauschzuordnung neu. Produkt- und Firmennamen angepasst. |
| | 8.12/10-2016 | Rechtschreib- und Layout-Korrekturen. |
| | 8.11/06-2016 | Ergänzung Softwarereferenz (zu Sonstigen Zuschlägen, Erfassungsstellen). |
| | 8.10/08-2013 | Überarbeitung des Kapitels B2B. |
| | 8.00/06-2013 | Vollständige Überarbeitung der ALFAK-Dokumentation und Anpassung auf A+W Business. |
| | 7.00/12-2012 | Vollständige Überarbeitung; Layout an neue Cl angepasst. |
| | 6.01/09-2010 | Layout an Doku-Konzept 2010 angepasst. |
| | 6.00/09-2008 | Neue Kapitel: Änderungshistorie, Änderungsüberwachung, Kreditlimit-Snapshot, Deckungsbeitrags-Grenzwerte. |
| | 5.01/08-2008 | Abbildungen aktualisiert. |
| | 5.00/07-2007 | Kapitel Funktionsprinzip und Bedienung neu (Anpassung an das neue Dokumentationskonzept). Überarbeitung des Kapitels Firmendaten (Softwarereferenz). |
| | 4.00/06-2005 | Überarbeitung der Basisdaten. |
| | 3.00/12-2003 | Struktureller Umbau auf Programmstruktur 4.0. |
| | 2.00/04-2001 | Überarbeitung Basisdaten, Produkte, Partner. |
| | 1.00/03-1998 | Ersterstellung. |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen
- Kontakte

**Anmerkungen zu diesem Dokument**

Diese Veröffentlichung ist ausschließlich für Endanwender von `A+W Business` gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Dieses Dokument beschreibt die volle Ausbaustufe der Stammdaten.

**Urheberrechte**

© 2020, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.
Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

**Warenzeichen**

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

### Kontakte

**A+W Software GmbH**
Am Pfahlgraben 4-10
D-35415 Pohlheim
- **Tel:** +49 6404 2051 0
- **Fax:** +49 6404 2051 877
- **Email:** aw.zentrale@a-w.com
- **Web:** http://www.a-w.com

---

# Tutorial 1

## Überblick

Das Tutorial zum Modul Stammdaten beschäftigt sich mit den Basis- und Stammdaten in `A+W Business`.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

### Schulung der Stammdaten

Die Schulung der Stammdaten ist Teil der Basisschulung des Programms `A+W Business`. Zusammen mit der Schulung zur Einführung bildet sie die Grundlage für alle weiteren Schulungen, die sich mit den Themen Verkauf, Einkauf, Lagerwirtschaft, Fertigung und Kapazitätsplanung befassen.

Das Tutorial 1 wird ergänzt durch das Tutorial 2, in dem Sie die Grundzüge der Auftragserfassung und der Dokumentenverarbeitung kennenlernen. Dieser zweite Teil baut auf diesen Kenntnissen des Tutorials 1 auf und zeigt im Überblick, wie Sie mit den Stammdaten für Partner, Produkte und Preise einen einfachen Auftrag erfassen können.

Zusätzlich werden im Tutorial 2 weitere Einstellungen für die internen Prozesse in `A+W Business` beschrieben.

> **Technische Voraussetzungen**
> Für die Schulung und für das Selbststudium wird eine vollständig eingerichtete Installation von `A+W Business` mit einer zugehörigen Datenbank vorausgesetzt.

### Zielgruppe und vorausgesetzte Kenntnisse

Die Tutorials 1 und 2 richtet sich an Teilnehmer, die in `A+W Business` die Stammdaten einrichten und pflegen. Sie müssen die Fachterminologie der Flachglasbranche beherrschen und grundlegende kaufmännische Kenntnisse haben.

Die Teilnehmer müssen die Elemente der Bedienoberfläche in `A+W Business` kennen und die allgemeine Bedienung beherrschen.

**Ergänzende Informationen**
- Überblick, "Standard-Menüs" auf Seite A-53
- Überblick, "Standard-Schaltflächen" auf Seite A-54
- Verkauf, "Bedienelemente in der Positionserfassung" auf Seite C-61
- Verkauf, "Bedienelemente im Dokumentenkopf" auf Seite C-41

### Themenblöcke

In Tutorial 1 finden Sie folgende Themenblöcke:
- Grundgedanken
- Kundendaten
- Lieferantendaten
- Produktdaten
- Stammdaten für Preise
- Zuschläge
- Rabatte
- Zusatzinformationen zur Firma

Das Tutorial 1 wird im Tutorial 2 durch folgende Themenblöcke ergänzt:
- Dokumente
- Einstellungen zur Faktura
- Text- und Dokumentendruck
- Zusatzinformationen

> **Reihenfolge der Lerneinheiten**
> Die Lerneinheiten der Tutorials sind so aufeinander abgestimmt, dass sie jeweils auf den Kenntnissen der vorausgehenden Einheit aufbauen. Diese Reihenfolge entspricht daher nicht der Reihenfolge, in der die jeweiligen Dialoge im Menü `Stammdaten` aufgeführt werden.

### Dokumentation

Für das Modul Stammdaten stehen folgende Dokumente zur Verfügung:

| Typ | Inhalt |
| :-- | :--- |
| **Handout** | Ausdruck des Tutorials für die Schulung |
| **PDF** | Vollständige Unterlagen<br>- Tutorial<br>- Softwarereferenz<br>- Index |
| **Online-Hilfe `<F1>`** | Kontextsensitive Hilfe |

### Aufbau des Tutorials

Die Tutorials bestehen aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

- **Überblick**: Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
    - Lernziele: Was soll vermittelt werden?
    - Nutzen: Wofür können Sie dieses Wissen einsetzen?
    - Merksätze: Welche Zusammenhänge müssen Sie sich merken?
- **Konzepte**: Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.
- **Übungen**: Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen. Die Übungen bauen aufeinander auf. Sie sollten daher entsprechend der Aufgabenstellung ausgeführt werden.
- **Querverweise**: Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf ergänzende Informationen in der Softwarereferenz und in anderen Parts hinweisen.

**Lesehinweis**
Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.
Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

### Darstellungskonventionen

Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

| Stil | Bedeutung |
| :--- | :--- |
| *Kursiv* | sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog `Produktarten`. |
| **Fett** | sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: **Geben Sie den Wert 0 ein.** |
| **>** | Mit dem sogenannten Brotkrumenpfad ist der Weg kennzeichnet, auf dem Sie einen Dialog öffnen, z. B. `Stammdaten` > `Allgemein` > `Kalender`. |
| **[]** | Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit `[OK]` speichern Sie die Daten. |
| **<>** | Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit `<F1>` öffnen Sie die Online-Hilfe. |

> **Dialogbeschreibungen**
> In den Lerneinheiten sind die besprochenen Dialoge nur so weit beschrieben, wie es für das Verständnis der Einheit notwendig ist. In der Softwarereferenz sind jedoch alle Elemente (Felder, Checkboxen usw.) der Dialoge ausführlich beschrieben, so dass zusätzliche Informationen dort zu finden sind.

### Menü-Übersicht

In diesem Abschnitt finden Sie eine kurze Übersicht über die Programmbereiche und Dialoge, die zum Thema Stammdaten gehören.

Über das Menü `Stammdaten` wählen Sie den Dialog aus, in dem Sie Daten erfassen, ändern oder prüfen wollen. Die folgende Übersicht gibt Ihnen eine erste Orientierung. Eine ausführliche Beschreibung der Dialoge finden Sie in der Softwarereferenz.

**Allgemein**
In diesem Bereich finden Sie allgemeine Vorgabe, z. B. die verfügbaren Sprachen, Arbeitstage und Basisnummernkreise.

**Produkte**
Das Menü `Produkte` ist in drei Untermenüs gegliedert:
- **Allgemein**: In diesem Bereich richten Sie die allgemeinen Daten für die Produktdefinition ein, z. B. Produktarten, Warengruppen, Strukturseiten, Varianten.
- **Artikel**: In diesem Bereich richten Sie die Stammdaten der Produkte ein, z. B. Produkte, Maßzuschläge und Varianten.
- **GGA**: Das Zusatz-Modul für Ganzglas-Anlagen ist nur kundenspezifisch freigeschaltet.
(Siehe "Produktdaten" auf Seite B-133)

**Preise**
In diesem Bereich richten Sie die Stammdaten der Preise ein, z. B. Tarife, Preise, Preiseinheiten, Preisgruppen und Zuschläge.
(Siehe "Stammdaten für Preise" auf Seite B-211)

**Lager**
In diesem Bereich richten Sie die Stammdaten für die Lagerverwaltung ein. Der Bereich ist im Part Lagerwirtschaft beschrieben.

**Marktpartner**
Das Menü `Marktpartner` ist in drei Untermenüs gegliedert:
- **Allgemein**: In diesem Bereich richten Sie die allgemeinen Daten zu den Marktpartnern ein, z. B. Gruppen, Branchen, Objekte, Klassifikatoren.
- **Kunde**: In diesem Bereich richten Sie die kundenbezogenen Daten ein, z. B. Adresse, Filialen, Lieferanschriften, Routen, Zahlungskonditionen und partnerspezifische Rundungen.
- **Lieferant**: In diesem Bereich richten Sie die lieferantenbezogenen Daten ein, z. B. Adresse, partnerspezifische Rundungen und Lieferantennachweise.
(Siehe "Kundendaten" auf Seite B-35)

**Versand**
In diesem Bereich richten Sie die Stammdaten für den Versand ein. Der Bereich ist im Part Fertigung beschrieben.

**Fertigung**
In diesem Bereich richten Sie die Stammdaten für die Produktion ein. Der Bereich ist im Part Fertigung beschrieben.

**Auftrag**
In diesem Bereich richten Sie die Stammdaten für Dokumente ein, z. B. Statuszuordnungen, Rundungen, Nummernkreise, Grenzmengen.
(Siehe Tutorial 2, "Dokumente" auf Seite B-407)

**Finanzen**
In diesem Bereich richten Sie die Stammdaten für Zahlungen und Rechnungen ein, z. B. Steuersätze und Erlöskonten.

**Firma**
In diesem Bereich richten Sie die Stammdaten Ihrer Firma ein, z. B. Mitarbeiter und AV-Bereiche. Außerdem legen Sie in den Firmendaten die Details zur Dokumentenerfassung, zu Datenübertragungen und Preisberechnungen fest.

**Texte**
In diesem Bereich richten Sie die Standardtexte für die Dokumente und die Textkennzeichen ein. Dazu gehören feste und variable Texte für aktuelle Mitteilungen, z. B. zu Ferienzeiten.
(Siehe Tutorial 2, "Text- und Dokumentendruck" auf Seite B-460)

**Formulare**
In diesem Bereich richten Sie die Details für den Druck von Dokumenten (Formularen) ein, z. B. Kopf- und Fußzeilen, Druckaufträge und Optionen für den Rechnungs- und Skizzendruck.
(Siehe Tutorial 2, "Formulare" auf Seite B-472)

**CEKAL**
In diesem Bereich richten Sie die Stammdaten für die Verwaltung der CEKAL-Texte ein. Diese Angaben werden nur in Frankreich und den Benelux-Staaten benötigt.

**CE Kennzeichen**
In diesem Bereich richten Sie die Details für die CE-Kennzeichnung ein.

**B2B**
In diesem Bereich richten Sie die Details für den Datenaustausch ein.

### Grundgedanken

Die Organisation und Pflege der Stammdaten ist die Basis von `A+W Business` und seinen Modulen. Die hinterlegten Daten werden in alle Bereiche des Systems übernommen. Alle Geschäftsbereiche greifen auf die gleichen Stammdaten zu, z. B. Kunden, Produkte, Preise, Status, Währungen.

Über die Stammdaten bestehen Bezüge zu allen Modulen von `A+W Business`. Sie schaffen die Grundlage zur Abwicklung Ihrer Geschäftsvorfälle, z. B. der Kundenaufträge. Über Schnittstellen können die Stammdaten auch an andere Programme übergeben werden.

Die Funktionen von `A+W Business` sind durch eine Reihe von Verknüpfungen zwischen den Stammdaten organisiert. Dazu gehören diejenigen, mit denen Sie die Geschäftsabläufe in Ihrem Unternehmen abbilden und die firmenspezifischen Standardeinstellungen (Defaults), die als Vorbelegung vorgeschlagen werden. Sie können, wie alle Defaults, in einem Dokument überschrieben werden.

> **Stammdaten ändern**
> Änderungen einiger Stammdaten greifen tief in die Funktionalität von `A+W Business` ein. Im Einzelnen werden Sie darauf aufmerksam gemacht, welche Daten nicht ohne Rücksprache bearbeitet werden sollten.

### Von den Stammdaten zum Auftrag

In dieser vereinfachten Darstellung sehen Sie die Abhängigkeiten von Stammdaten untereinander. Firmenweite Einstellungen haben wesentlichen Einfluss auf die weitere Verarbeitung von Aufträgen, auf Preisberechnungen, Abrechnungen, Auswertungen usw.

In den folgenden Einheiten werden Ihnen zunächst Informationen zu der Gestaltung von Marktpartnern, Produkten und Preisen finden. Daran anschließend werden die wichtigsten Einstellungen zu Dokumenten vorgestellt. Die firmenweiten Einstellungen werden dazu jeweils genannt.

### Aufträge in A+W Business

Alle kaufmännischen Vorgänge in `A+W Business` basieren auf den Stammdaten. Wenn Sie einen Auftrag erfassen, müssen (mindestens) folgende Daten eingetragen werden:
- **Auftragskopf**
    - Name und Anschrift des Kunden
    - Lieferbedingungen und -termin
    - Zahlungsbedingungen
- **Auftragspositionen**
    - Produkt und Produktaufbau, z. B. Glas, ISO, Sprossen
    - Maße und Bearbeitungen, z. B. Modellformen, Ausschnitte
    - Preise und Rabatte
    - Zuschläge, z. B. für den Transport

Wenn die notwendigen Daten im Auftrag erfasst sind, müssen die Positionen produziert, verpackt und geliefert werden. Eventuell müssen für die Produktion zusätzliche Artikel eingekauft werden, die Sie nicht auf Lager halten. Aus dem Auftrag heraus entstehen also weitere Geschäftsabläufe, die so weit wie möglich automatisiert sind:
- Druck von weiteren Dokumenten, z. B. Auftragsbestätigung, Lieferschein, Rechnung
- Bestellung durch den Einkauf
- Abruf der Lagerartikel für die Produktion
- Übergabe der Auftragsdaten an die Produktion
- Rückmeldung aus der Produktion, wenn der Auftrag fertig und versandbereit ist
- Auslieferung
- Prüfung der Zahlungen vom Kunden
- Übergabe von Rechnungen an die Finanzbuchhaltung

Diese Abläufe werden in den Parts Verkauf, Einkauf, Lagerverwaltung und zur Fertigung behandelt.

Im Tutorial zu den Stammdaten lernen Sie, wie Sie die Daten der Marktpartner, Produkte und zu Preisen, Zuschlägen und Rabatten anlegen und pflegen. Im zweiten Teil der Schulung lernen Sie, wie diese Daten in Dokumenten getestet und wie die Abläufe gesteuert werden können.

### Stammdaten anlegen

Wenn Sie Ihre Stammdaten ganz neu anlegen, sollten Sie sich an die nachfolgende Empfehlung halten. Sie vermeiden damit, auf Daten zugreifen zu müssen, die noch nicht hinterlegt sind.

Aus der Kundenverwaltung heraus können Sie gleichzeitig auch viele Basisdaten anlegen und sich so an den aktuellen Erfordernissen für Ihre Kundenstammdaten orientieren.

> **Hinweis**
> Wenn Sie Basis- oder Stammdaten angelegt oder geändert haben, sollten Sie diese zunächst testen. Sie können so feststellen, ob das Resultat Ihren Vorstellungen entspricht, bevor Sie die neuen Daten tatsächlich einsetzen.

Folgende Reihenfolge wird zur Erfassung der Stammdaten empfohlen:
1.  **Kundendaten**
    Legen Sie zumindest die Kundendaten zur Adresse und zur Kommunikation an. Spezielle Preis- und Rabattvereinbarungen können Sie später bei Bedarf ergänzen.
2.  **Warengruppen**
    Entwerfen Sie zunächst das Warengruppenkonzept. Sie benötigen dieses zum Anlegen der Produkte.
    Die Warengruppen können auch aus der Produktverwaltung heraus angelegt werden.
3.  **Produkte**
    Gleichzeitig mit einem Produkt können Sie auch die Preise, Zuschläge und Rabatte anlegen. Sie können die Preise aber auch nach den Produkten anlegen und in der Produktdefinition nachträglich zuordnen.
    Wenn Sie neue Produkte und Preise angelegt haben, sollten Sie in der Angebots- bzw. Auftragserfassung testen, ob die Preise nach Ihren Vorstellungen berechnet werden. Sie verringern damit den eventuell nötigen Aufwand, nachträglich Stammdaten korrigieren zu müssen.
4.  **Preise**
    Wenn Sie Preise, Zuschläge und Rabatte angelegt haben, können Sie diese den Produkten zuordnen. Wenn bereits Sonstige Zuschläge vorhanden sind, können Sie diese den Preisen zuordnen.
5.  **Sonderrabatte/Teuerungszuschläge**
    Legen Sie die Rabatte oder Zuschläge an, die unabhängig von Preisen und Marktpartnern gültig sein sollen.
    Wenn Sie Sonderrabatte und Teuerungszuschläge angelegt haben, sollten Sie unbedingt in der Auftragserfassung testen, ob diese nach Ihren Vorstellungen eingefügt und berechnet werden.

### Basistabellen

In den verschiedenen Dialogen zum Erfassen von Stammdaten stehen Komboboxen mit Auswahllisten zur Verfügung, die die Eingabe von Daten erleichtern. Die Einträge in diesen Listen sind in aller Regel in sogenannten Basistabellen hinterlegt und können bearbeitet werden.

**Basistabelle erweitern**

Das Anlegen von Daten in diesen einfachen Tabellen wird beispielhaft für Lieferantengruppen beschrieben.

**So hinterlegen Sie eine neue Lieferantengruppe**
1.  Wählen Sie `Stammdaten` > `Marktpartner` > `Allgemein` > `Lieferantengruppen`.
2.  Wählen Sie im Menü `Start` > `Neu`, um in den Erfassungs-Modus zu wechseln.
3.  Tragen Sie mindestens den Namen der Lieferantengruppe ein.
    Achten Sie darauf, dass der Name sich auf die Besonderheit der Gruppe bezieht, z. B. **Zubehörhändler**.
4.  Wählen Sie im Menü `Start` > `Speichern`, um die Daten zu speichern.
    Die Lieferantengruppe wird gespeichert und steht zur Auswahl in den Dialogen zur Verfügung, in denen Gruppen zugewiesen werden können.

#### Sperren

In fast allen diesen Dialogen können Einträge für die weitere Verwendung gesperrt werden.

*   `Fremdschlüssel` können zur Datenübergabe an andere Programme verwendet werden.
*   Gesperrte Einträge werden nicht mehr zur Auswahl angeboten. Wenn sie vor der Sperrung aber schon zugewiesen waren, werden sie weiterhin angezeigt.

#### Löschen

Daten können nur dann gelöscht werden, wenn sie nirgends eingesetzt wurden, d. h., wenn sie nicht referenziert sind. Wenn referenzierte Daten nicht mehr verwendet werden sollen, müssen sie gesperrt werden.

Wenn Sie in den Übungen Testdaten anlegen, die nicht wirklich verwendet werden sollen, können Sie diese Daten allerdings sofort wieder löschen.

> **Ergänzende Informationen**
> Überblick, "Standard-Schaltflächen" auf Seite A-54

## Kundendaten

In diesem Themenblock lernen Sie, wie Sie die Stammdaten für Kunden einrichten.

Dazu gehören folgende Lerneinheiten:
- "Marktpartner" auf Seite B-36
- "Adressdaten" auf Seite B-41
- "Auftrag und Kundenrechnung" auf Seite B-53
- "Mitarbeiter und Filialen" auf Seite B-60
- "Texte" auf Seite B-67
- "Klassifikatoren" auf Seite B-73
- "Finanzen und Saldo" auf Seite B-80
- "Vertreter" auf Seite B-110
- "Produktion" auf Seite B-114
- "Ergänzende Daten für Partner" auf Seite B-119

Die Daten für Kunden und Lieferanten unterscheiden sich nur geringfügig. In dieser Lerneinheit gelten die Erklärungen und Handlungsschritte daher in den meisten Fällen auch für Lieferanten.

### Marktpartner

**Lernziele**
- Unterschied der Stammdaten für Marktpartner, Kunden und Lieferanten kennenlernen.
- Basistabellen für Marktpartner ergänzen.

**Nutzen**
- Partnerdaten dienen zur schnellen Erfassung von Aufträgen und Bestellungen, ohne die Daten jeweils vollständig eingeben zu müssen.
- Die Einträge in den Basistabellen werden in den komplexeren Dialogen mit einander verknüpft, um bestimmte Funktionen zu erfüllen, z. B. das Landeskürzel für die Auswahl der Formularsprache.

**Merke**

- **Marktpartner**: In `A+W Business` wird zwischen Kunden, Lieferanten und sonstigen Partnern unterschieden:
    - **Kunden** sind all diejenigen, zu denen Aufträge erstellt werden und die von Ihnen mit Produkten beliefert werden.
    - **Lieferanten** sind alle diejenigen, bei denen Sie Produkte bestellen, die im eigenen Unternehmen nicht selbst hergestellt werden.
    - **Partner** sind all diejenigen, die weder Kunden noch Lieferant sind, z. B. der Getränkeservice, der Steuerberater. Zu diesen Partnern können in `A+W Business` keine Dokumente erfasst werden. Partner aus diesem Bereich können nachträglich in die Stammdaten für Kunden oder Lieferanten kopiert werden.
- **Partnerstammdaten**: In den Partnerstammdaten werden alle Informationen hinterlegt, die zum Erfassen eines Auftrags oder einer Bestellung (Dokumente) notwendig sind. Diese Daten werden automatisch in den Dokumentenkopf übernommen und können pro Dokument überschrieben werden. Solche Änderungen werden nicht in die Stammdaten des jeweiligen Partners zurückgeschrieben.
- **Basistabellen**: Basistabellen werden als einfache Dialoge dargestellt. Sie sind in den Untermenüs des Moduls Stammdaten thematisch gruppiert.
- **Checkbox Sperren**: Einträge in den Basistabellen können gesperrt werden. Gesperrte Einträge werden nicht mehr zur Auswahl angeboten. Wenn sie vor der Sperrung aber schon zugewiesen waren, werden sie weiterhin angezeigt.
- **Datenexport**: Die Daten zu Marktpartnern können Sie für jeden Mandanten einzeln verwalten. Mit der integrierten Export-Funktion können Sie Partnerdaten exportieren, z. B. um Serienbriefe zu erstellen.

#### Einführung in das Thema Marktpartner

In der Partnerverwaltung werden nicht nur die Adressen zu den Marktpartnern hinterlegt sondern auch Parameter, die die Angebots- und Auftragserfassung erleichtern, z. B. Tourenzuordnungen, abweichende Rundungen, Mitarbeiter und Filialen, Zahlungsbedingungen, Objekte.

Die Abbildung zeigt das Zusammenspiel von Basisdaten für die Definition und Pflege der Partnerstammdaten. Damit Partnerdaten vollständig angelegt und gepflegt werden können, müssen die Basisdaten hinterlegt sein, z. B. Anreden, Rabatte, Rundungen.

#### Dialog Partnerverwaltung

Die Daten zu Kunden und Lieferanten werden in `A+W Business` als Partnerstammdaten im Dialog `Partnerverwaltung` hinterlegt. Diese Stammdaten werden in den Dokumenten herangezogen und können bei Bedarf überschrieben werden. Änderungen aus den Dokumenten werden nicht in die Stammdaten zurückgeschrieben.

Zu den Stammdaten der Kunden gehören neben den Adress- und Kommunikationsdaten auch Daten zu Finanzen und Kreditwürdigkeit und spezifische Produktionsdaten. Über das Ordner-Symbol können Sie in die jeweilige Basistabelle wechseln, um die Daten zu ergänzen.

Weitere Besonderheiten zu den Lieferanten lernen Sie in der entsprechenden Lerneinheit kennen.

> **Datenschutz beachten**
> Personenbezogene Daten unterliegen dem Datenschutz. Achten Sie daher darauf, dass diese Daten durch entsprechende Zugriffsrechte vor Missbrauch geschützt sind.

#### Stammdatendialoge für Marktpartner

Im Menü `Marktpartner` finden Sie die Untermenüs `Allgemein`, `Kunde` und `Lieferant`, in denen Sie die allgemeinen und die partnerspezifischen Daten hinterlegen. Alle diese Dialoge sind ausführlich in der Softwarereferenz beschrieben.
(Siehe Softwarereferenz, "Marktpartner" auf Seite B-743)

Damit Sie die Kunden- und Lieferantendaten vollständig anlegen können, müssen folgende Basisdaten hinterlegt sein.

| Pfad > Dialog | Bedeutung |
| :--- | :--- |
| `Marktpartner > Allgemein > Anreden` | Neben den üblichen Anreden wie Herr, Frau und Firma können Sie auch andere Bezeichnungen hinterlegen, z. B., um ausländische Partner korrekt anzusprechen. |
| `Marktpartner > Allgemein > Titel` | Als Titel werden in `A+W Business` vor allem die Stellungen der Ansprechpartner verstanden, also z. B. Produktionsleiter, Geschäftsführer. |
| `Versand > Lieferbedingungen` | Die Lieferbedingungen beziehen sich auf das Transportmittel, mit dem ausgeliefert werden soll, z. B. Bahn, Spediteur. |
| `Versand > Touren` | In den Touren legen Sie neben dem Tag, an dem die Tour regelmäßig gefahren wird, auch die Lieferpauschale fest, die zur Berechnung der Frachtkosten herangezogen wird. Wichtig ist, dass Sie auch eine Tour für die Abholung und für den Transport mit einer Spedition anlegen - sofern Sie mit Speditionen zusammenarbeiten. |
| `Finanzen > Steuer` | Dies sind die unterschiedlichen Steuersätze, die Sie in den Aufträgen Ihrer Kunden berechnen. Sie können sowohl die inländischen als auch ausländischen Steuersätze hinterlegen und jedem einzelnen Kunden den passenden Steuersatz zuweisen. |
| `Finanzen > Zahlungs-bedingungen` | Die Zahlungsbedingungen werden zur Berechnung des Zahlungsziels und des Skontobetrags herangezogen. |
| `Finanzen > Banken` | Dies sind Bankverbindungen, über die Sie die Geschäfte mit Ihren Kunden oder Lieferanten abwickeln. Wenn Sie die Angaben vollständig eingetragen haben, können Sie in den Partnerstammdaten die IBAN errechnen lassen. |
| `Finanzen > Währung` | Sie können die unterschiedlichen Währungen und dazu die Wechselkurse hinterlegen, wenn Sie mit mehreren Währungen arbeiten. Für den Euro-Raum selbst brauchen Sie keine Angaben zu machen. |
| `Finanzen > Zahlungswege` | Sie können die Zahlungsformen hinterlegen, die von Ihrem Unternehmen akzeptiert werden. Diese Angaben können auch an die Finanzbuchhaltung (FiBu) übergeben werden. |

Neben den Daten, die in den Dialogen im Menü `Marktpartner` hinterlegt sind, können weitere Daten aus folgenden Dialogen bei der Definition von Kunden und Lieferanten herangezogen werden:
- **Preise**: Jahrgang, Schlüssel, Tarif und Preis
- **Zuschläge**: Sonstige Zuschläge, Austauschzuschläge, Modellzuschläge
- **Finanzen**: Steuer, Kostenart, Kostenstellen

> **Beschreibung von Dialogen in weiteren Parts**
> Einige dieser Dialoge werden ausführlich in anderen Parts beschrieben. Diese Dialoge werden im Tutorial der Stammdaten nicht erläutert.

### Adressdaten

**Lernziele**
- Dialog `Partnerverwaltung` erarbeiten.
- Kundengruppen anlegen und zuweisen.
- Touren und Lieferbedingungen anlegen und zuweisen.

**Nutzen**
- Stammdaten von Kunden werden zentral eingegeben und gepflegt. Sie stehen damit immer aktuell für neue Aufträge zur Verfügung.
- Die Adressdaten werden für die Lieferung und Rechnung verwendet. Abweichende Anschriften können jeweils eingegeben werden.

**Merke**
- **Partnerverwaltung**: Im Dialog `Partnerverwaltung` hinterlegen Sie die Stammdaten eines jeden Kunden, die genau für diesen einen Partner gelten.
- **Anschrift**: Zu jedem Marktpartner wird eine Hauptanschrift angegeben, die in aller Regel für die Lieferung und die Rechnung herangezogen wird.
- **Branche**: Branchen stehen in der Statistik als zusätzliches Auswertungs- und Sortierkriterium zur Verfügung.
- **Sprache**: Dokumente werden in den Formularen gedruckt, die der Sprache des Kunden entsprechen.
- **Gruppen**: Kunden können einer Kundengruppen zugeordnet werden, z. B., um Rabatte oder Preise gemeinsam zu pflegen.
- **Tour**: Touren bilden die Grundlage für die Versandplanung und -steuerung. Aus der Lieferdauer und dem Liefertermin wird der Versandtag berechnet.

#### Vorgaben für Adressen

Im Register `Adresse` erfassen Sie die Daten zur Adresse, Kommunikation und zur Lieferung. Die Einstellungen in diesem Register werden in den folgenden Abschnitten ausführlich erläutert.

**Branchen**
Jedem Kunden und Lieferanten können Sie eine Branche zuordnen, z. B. Glashandel, Fensterbau, Schreiner. Wenn ein neuer Kunde einer Branche angehört, die bisher nicht angelegt war, können Sie über das Ordner-Symbol in den Dialog `Branchen` wechseln, um die neue Branche einzutragen.
Die Branche steht in der Statistik als zusätzliches Auswertungs- und Sortierkriterium zur Verfügung.

**Sprache**
Jedem Kunden weisen Sie die Sprache zu, in der die Dokumente im Formular gedruckt werden sollen. Dem Kennzeichen entsprechend werden dann die jeweiligen Formulare ausgewählt.
Wenn Sie weitere Sprachen anlegen, sollten Sie jeweils auch die Preis- und Mengeneinheiten übersetzen.

**Gruppen**
Marktpartnern können in Gruppen zusammengefasst werden. Jeder Kunde kann einer Kundengruppe zugeordnet werden, jeder Lieferant einer Lieferantengruppe.
Wenn Sie z. B. Rabatte oder Preise für eine Gruppe festlegen, gelten diese Konditionen für alle Mitglieder der Gruppe. Damit vereinfachen Sie die Pflege der Konditionen.
Bei der Erfassung eines Dokuments können die Vorbelegungen überschrieben werden, die über die zugewiesene Gruppe in den jeweiligen Feldern angezeigt werden.

**Beispiele für die Verwendung von Gruppen**

- **Kundengruppe**:
    - Deckungsbeitrags-Grenzwerte
    - Preise
    - Rabatte
    - Rundungen
    - Zuschläge
    - als Sortierkriterium in der Kunden-Umsatzstatistik
- **Lieferantengruppe**:
    - Preise
    - Rabatte
    - Rundungen
    - Zuschläge
    - als Sortierkriterium in der Lieferanten-Umsatzstatistik

Die Gruppen für die Marktpartner legen Sie unter `Marktpartner` > `Allgemein` > `Partnergruppen`, `Kundengruppen`, `Lieferantengruppen` an. Gehen Sie dabei so vor, wie in der Einheit `Basistabelle erweitern` beschrieben.

Wenn Sie die Gruppen angelegt haben, können Sie diese in der `Partnerverwaltung` > Register `Adresse` dem Kunden oder Lieferanten zuordnen.

Bei der Berechnung von Aufträgen (oder Bestellungen) werden die Konditionen in folgender Reihenfolge berücksichtig:
- Angaben aus dem Dokument
- Definitionen aus den Partnerstammdaten
- Gruppenspezifische Konditionen

Wenn keine Vereinbarungen gefunden werden, gelten die allgemeinen Preise, Zuschläge und Rundungen.

**Abweichende Kunden-/Lieferantengruppen**
Wenn ein Kunde bei bestimmten Warengruppen andere Konditionen erhalten soll, kann er einer abweichenden Kundengruppe zugeordnet werden.

> **Beispiel**
> Sie haben u. a. die Kundengruppen `Produzenten` und `Händler` angelegt.
> Der Kunde A gehört zur Kundengruppe `Händler`. Wenn für diesen Kunden ein Auftrag mit einer Position aus der Warengruppe `Wärmeschutz-ISO` erfasst wird, sollen jedoch die Bedingungen der Kundengruppe `Produzent` gelten.
> Solche Ausnahmen legen Sie im Dialog `Abweichende Kundengruppen` fest.

Ein Kunde kann einer abweichenden Kundengruppe auch dann zugeordnet werden, wenn er keiner (normalen) Kundengruppe zugeordnet ist. Die Konditionen der abweichenden Kundengruppe beziehen sich nur auf die angegebene Warengruppe. Alle anderen Konditionen, die für den Kunden gelten, bleiben unverändert bestehen.
Auf die gleiche Weise können Sie auch abweichende Zuordnungen zu Lieferantengruppen festlegen.
Wenn Sie die Partnergruppen sehr feingliedrig angelegt haben, können Sie für die einzelnen Marktpartner mehrere Abweichungen definieren. So kann z. B. ein Lieferant zur Gruppe `Händler` gehören, wenn Sie bei ihm Beschläge bestellen, und zur Gruppe `Produzent`, wenn Sie ESG-Scheiben bestellen.

**Touren und Lieferbedingungen**
Im Zusammenspiel mit den Kundendaten und den Auftragsterminen bilden die Touren die Grundlage für die Versandplanung und -steuerung. Aus der Lieferdauer und dem Liefertermin wird der Versandtag berechnet, an dem die Lieferung an den Fahrer ausgegeben werden muss.
Die Lieferdauer ist in einer separaten Einheit beschrieben.

Pro Tour werden in den Stammdaten die Wochentage festgelegt, an denen sie gefahren wird. So kann eine Tour z. B. von Frankfurt nach Karlsruhe so eingerichtet sein, dass sie montags und donnerstags gefahren wird. Mit dieser Tour sollen alle Kunden beliefert werden, die auf dieser Strecke im Umkreis von 50 km liegen.

Dazu können Sie außerdem Frachtkosten angeben, über die im Auftrag geprüft werden kann, ob sich die Auslieferung eines einzelnen Auftrags lohnt. Die Art der Auslieferung stellen Sie als Lieferbedingung ein, z. B. `Lkw` oder `Spedition`.

Für Ihre ortsansässigen Kunden legen Sie außerdem eine Tour `Abholung` an, zu der jedoch keine Frachtkosten berechnet werden dürfen.

Jedem Kunden werden eine passende Tour und eine Rangfolgenummer zugewiesen. Die Rangfolge legen Sie im Register `Auftrag` fest.

Die Rangfolgenummer bestimmt die Reihenfolge, in der die Kunden pro Tour beliefert werden.

> **Beispiel**
> Kunde A und Kunde B werden mit Tour Süd beliefert. Kunde A hat die Tourrangfolge 1, Kunde B hat die Tourrangfolge 2.
> Kunde A wird also vor Kunde B beliefert.

Diese Einstellungen aus den Stammdaten werden in den Auftrag übernommen. Die Vorbelegung kann pro Auftrag geändert werden. Dabei wird automatisch geprüft, ob der eingegebene Liefertermin mit den Tourentagen des Kunden übereinstimmt. Bei einer Abweichung wird eine entsprechende Meldung ausgegeben. Abweichende Daten können gespeichert werden. Sie werden in der Tourenplanung übernommen.

**Zolltouren**
Für den grenzüberschreitenden Verkehr hinterlegen Sie Touren unter `Stammdaten` > `Versand` > `Zolltouren`. Sie können Grenzübergänge angeben oder den Namen der Tour. Die Zolltouren werden für die Versandplanung benötigt. Sie können in den Partnerstammdaten nicht zugewiesen werden.
Die Touren und Tourenplanung werden ausführlich im Part Fertigung beschrieben.

#### Tour definieren

Sie können die hinterlegten Touren modifizieren oder durch neue Touren ergänzen. Wenn z. B. die Frachtkosten berechnet werden sollen, müssen Sie pro Tour die Kilometerpauschale eintragen.

**So legen Sie eine Tour an**
1.  Wählen Sie im Menü `Stammdaten` > `Versand` > `Touren`.
2.  Wählen Sie im Menü `Start` > `Neu`, um in den Erfassungs-Modus zu wechseln.
3.  Geben Sie die Nummer und Bezeichnung ein. Beide können frei gewählt werden.
4.  Aktivieren Sie die Checkboxen für die Tage, an denen die Tour regelmäßig gefahren wird. Die Angaben werden in der Auftragserfassung mit dem eingetragenen Liefertermin verglichen. Eine Meldung macht Sie darauf aufmerksam, wenn Termin und Tourentag nicht übereinstimmen.
5.  Verschieben Sie die Ansicht nach rechts (scrollen), um weitere Details festzulegen. Sie können dazu auch mit der `<Tab>`-Taste durch die Felder springen.
6.  Verschieben Sie die Ansicht noch weiter nach rechts, um z. B. die Frachtkosten pro Kilometer einzugeben.
    > **Bei Abholung keine Anlieferung berechnen**
    > Sie müssen für die Tour `Abholung`, für die keine Anlieferpauschale berechnet werden darf, die Checkbox `ohne Liefer. Pausch.` aktivieren.
7.  Wählen Sie im Menü `Start` > `Speichern`, um die Daten zu speichern. Die Daten werden gespeichert.
8.  Wiederholen Sie ggf. die Schritte 2 bis 7 für weitere Touren.

Sie müssen nicht sämtliche Daten eintragen. Wenn Sie z. B. nicht in Schichten arbeiten oder keinen eigenen Versand haben, können Sie die entsprechenden Felder überspringen.

#### Partnerstammdaten anlegen

Die Dialoge zum Erfassen von Kunden-, Lieferanten- und Partnerdaten unterscheiden sich nur unwesentlich voneinander und sind daher zu einer Beschreibung zusammengefasst. In der folgenden Handlungsanleitung wird der Dialog `Partnerverwaltung` für Kunden geöffnet. Die Handlungsschritte gelten in gleicher Weise für Lieferanten und Partner.

> **Potenzielle Kunden oder Lieferanten**
> Sie können Daten zunächst als allgemeinen Marktpartner erfassen. Über die Kopierfunktion können die Daten nachträglich als Kunde oder Lieferant gespeichert werden.

Im Dialog `Partnerverwaltung` können Sie sich die freien Nummern anzeigen lassen, indem Sie auf die `[Lupe]` neben dem Eingabefeld für die Nummer klicken. Ein entsprechender Dialog steht auch beim Anlegen von Produktdaten zur Verfügung.

**So legen Sie Kundendaten an**
1.  Wählen Sie im Menü `Stammdaten` > `Marktpartner` > `Kunde` > `Kunden`. Der Dialog `Partnerverwaltung` wird mit dem Register `Adresse` geöffnet.
2.  Wählen Sie im Menü `Start` > `Neu`, um in den Erfassungs-Modus zu wechseln.
3.  Wählen Sie ggf. den Mandanten aus, wenn in Ihrer Firma mehrere Mandanten angelegt sind.
4Geben Sie in den Pflichtfeldern die Nummer und den Matchcode ein. Sie können die Nummern Ihrer Kunden, Lieferanten und sonstigen Geschäftspartner frei wählen, jedoch darf jede Nummer nur einmal vergeben werden. Sie können sich die freien Nummern anzeigen lassen, indem Sie auf die `[Lupe]` klicken.
5.  Geben Sie die Daten für die Anschrift ein. Wenn Sie die gewünschten Daten noch nicht in der Kombobox finden, können mit einem Klick auf das Ordner-Symbol den entsprechenden Dialog öffnen und die Daten ergänzen.
6.  Geben Sie die Daten für die Verbindungen zur Kommunikation ein.
7.  Wählen Sie die Haupttour (Tour 1), eine Ersatztour (Tour 2) und die Lieferbedingung aus. Wenn Sie mit dem neuen Kunden in einer anderen Sprache kommunizieren, so wählen Sie diese Sprache aus. In den Dokumenten wird der entsprechende Sprachenschlüssel angezogen, so dass z. B. die Bezeichnungen für Produkte in der eingestellten Sprache gedruckt werden. Die Beschreibungen zur Mehrsprachigkeit finden Sie in der Softwarereferenz.
8.  Wählen Sie im Menü `Start` > `Speichern`, um die Daten zu speichern.

Damit haben Sie die wichtigsten Daten zur Identifikation des Kunden erfasst. Sie können jetzt im Register `Auftrag` die Daten für die Rechnung ergänzen.

### Auftrag und Kundenrechnung

**Lernziele**
- Auftragspriorität festlegen.
- Einstellungen für Rechnungen, Monatsrechnung, Sammelrechnung kennenlernen.
- Einstellung für Teillieferung und Teilfakturierung kennenlernen.

**Nutzen**
- Vorgaben aus den Kundenstammdaten werden in Auftrag übernommen und müssen nicht immer wieder neu erfasst werden.
- Die meisten Vorgaben aus den Stammdaten können im Auftrag angepasst werden.

**Merke**
- **Priorität**: Die Auftragspriorität gibt an, mit welcher Dringlichkeit ein Auftrag gefertigt werden soll. Sie wird an die Kapazitätsplanung und damit an die Produktion übergeben.
- **Rechnung**: Für jeden Kunden legen Sie die Vorgaben für die Rechnungen fest:
    - Standardrundungen
    - Rechnungsmindestwert
    - Ausgabe der Rechnung (einzeln, gesammelt)
- **Standardrundungen**: Für die Preisberechnung wird die Fläche des Glases gerundet. Diese Rundung gilt nicht für die Produktion.
- **Rechnungsform**: Sammelrechnungen, Monatsrechnungen oder Teilrechnungen können nur erstellt werden, wenn diese Formen in den Kundenstammdaten zugelassen sind.

#### Vorgaben für Aufträge

Im Register `Auftrag` legen Sie Details für die Rechnungen und die Lieferung fest. Die Angaben zur Rechnung und zur Priorität können im Auftrag geändert werden. Diese Vorgaben werden im Folgenden ausführlich beschrieben.

**Auftragspriorität**
Die Auftragspriorität gibt an, mit welcher Dringlichkeit ein Auftrag gefertigt werden soll. Sie wird an die Kapazitätsplanung und damit an die Produktion übergeben.
- **Eilt**: Die Aufträge werden mit oberster Priorität gefertigt.
- **Normal**: Die Aufträge werden in den üblichen Ablauf eingeordnet.
- **Zugabe**: Der Auftrag soll so gefertigt werden, dass er Reste und Restplatten verbraucht, die beim Zuschnitt anderer Aufträge entstehen.
- **Abruf**: Die Aufträge werden auf Abruf gefertigt.

#### Vorgaben für die Rechnung

Für jeden Kunden legen Sie die Vorgaben für die Rechnungen fest:
- Standardrundungen
- Rechnungsmindestwert
- Ausgabe der Rechnung (einzeln, gesammelt)

**Standardrundungen**
Für die Preisberechnung wird die Fläche des Glases gerundet. In Deutschland basiert die Preisberechnung auf einer 30er-Maßrundung. Dies bedeutet, dass zur Berechnung der nächste durch 30 teilbare Wert zugrunde gelegt wird. Daraus ergibt sich bei einem Glas von 1000 mm x 1000 mm für die Preisberechnung die Fläche 1,04 qm (= 1020 x 1020). In Frankreich wird z. B. mit einer 10er-Maßrundung gerechnet.
Diese Rundung gilt nicht für die Produktion.

Die Maßrundung aus den Partnerdaten kann durch andere Vorgaben übersteuert werden. Dabei sucht `A+W Business` in folgender Reihenfolge nach den Angaben: Individualpreise > Rabatte > Preise > Partnerstammdaten. Die Preisfindung wird ausführlich im Part Verkauf geschult.

**Zuschlag für Rechnungsstellung**
Der Zuschlag zur Rechnungsstellung muss als `Sonstiger Zuschlag` angelegt werden. Diese Zuschläge lernen Sie in der gleichnamigen Einheit kennen.
- **Für 1. Rechnung im Monat**: Jeweils für die erste Rechnung im Monat wird der Zuschlag erhoben. Auf alle weiteren Rechnungen im laufenden Monat entfällt dann der Zuschlag.
- **Für jede Rechnung**: Der Rechnungsstellungszuschlag wird für jede Rechnung erhoben.

**Mindestauftragswert**
Pro Auftrag kann ein Mindestwert festgelegt werden. Die Differenz zum Mindestauftragswert kann im Auftrag auf zwei Arten ausgewiesen werden:
- **Als separate Position**: Liegt der Auftragswert unter dem vereinbarten Mindestauftragswert, wird automatisch die Zuschlagsposition `Mindestauftragswert` hinzugefügt, die den Differenzbetrag ausweist.
- **Auf alle Positionen umgerechnet**: Die Differenz wird auf alle Positionen umgelegt.

Zur Berechnung stehen zwei Möglichkeiten zur Verfügung:
- Sie legen einen Zuschlag fest, der im Auftrag herangezogen wird, wenn der Mindestwert nicht erreicht wird.
- Im Auftrag wird automatisch der Mindestwert berechnet, wenn der Auftragswert unter der festgelegten Grenze liegt.

**Monatsrechnung**
Rechnungen können einzeln, gesammelt oder als Monatsrechnung gedruckt und versendet werden, z. B. im monatlichen oder 2-wöchentlichen Turnus. Die Aufträge dieses Kunden erhalten bei Lieferscheindruck automatisch das Kennzeichen `Monatsrechnung`, anhand dessen Sie diese bei Fälligkeit zur Fakturierung selektieren können.
Dazu müssen in den Firmendaten im Register `Druck` den entsprechenden Druckpunkt und Statuspunkt eintragen sein.

**Sammelrechnung**
Wenn ein Kunde keine Einzelrechnungen wünscht, erhalten alle seine Aufträge das Kennzeichen für Sammelrechnungen. Über dieses Kennzeichen können Sie die fälligen Rechnungen selektieren.

Folgende Kriterien müssen in allen Aufträgen des jeweiligen Kunden übereinstimmen, damit alle Aufträge eines Kunden beim Druck in einer Sammelrechnung zusammengefasst werden können:
- Kundennummer
- Kennzeichen Sammelrechnungsdruck im Auftrag
- Zahlungsbedingungen und Fälligkeitsdatum
- Währung
- Mehrwertsteuer-Kennzeichen 1 und 2
- Automatische Zuschläge: Zuschlag für Rechnungsstellung.
- AV-Bereich
- Rechnungsadresse (Name 1)
- Liefertermin

Sobald sich bei einem Auftrag eines dieser Kriterien unterscheidet, wird der Sammelrechnungsdruck bei diesem Auftrag unterbrochen. Dieser Auftrag und alle Aufträge, die ihm im Nummernverwalter nachfolgen, erhalten dann automatisch eine neue Rechnungsnummer. In diesem Fall werden also zwei Rechnungen gedruckt. Wenn weitere Unterschiede auftreten, wird eine weitere Rechnungsnummer vergeben.

**Teillieferung, Teilfakturierung**
Sind für einen Kunden Teillieferungen vereinbart, müssen Sie entscheiden, ob die Teillieferung mit oder ohne Teilfakturierung erfolgen soll.
Bei der Teilfakturierung erhält der Kunde zu jeder Teillieferung eine Teilrechnung. Der Teilrechnungsbetrag und die -menge werden von dem Originalauftrag abgezogen.
Ist die Teilfakturierung nicht zugelassen, ist der Originalauftrag für die Fakturierung so lange gesperrt, bis die letzte Teillieferung erfolgt ist.

> **Teillieferung im Auftrag**
> Sie können aus einem Auftrag nur dann eine Teillieferung erzeugen, wenn in den Stammdaten des Kunden die Checkbox `Teillieferung` markiert ist.

#### Einstellungen für den Kundenauftrag bearbeiten

Die folgende Handlungsanleitung baut auf den Schritten auf, die in der vorigen Einheit beschrieben wurden.

**So ergänzen Sie die Daten für Kundendokumente**
1.  Wählen Sie im Menü `Stammdaten` > `Marktpartner` > `Kunde` > `Kunden` > Register `Auftrag`.
2.  Prüfen Sie, ob die Werte für die Maßrundung korrekt angegeben sind.
3.  Legen Sie den Modus für die Rechnungsstellung fest.
4.  Markieren Sie die Schaltflächen für den Faxversand und den Mailversand von Dokumenten. Die Funktion kann für folgende Dokumente getrennt aktiviert werden:
    - Auftragsbestätigung (AB)
    - Angebot (An)
    - Rechnung (Re)
    - Gutschrift (Gu)
    Achten Sie darauf, dass Sie dazu auch die entsprechenden Faxnummern und die E-Mail-Adressen im Register `Adresse` hinterlegen.
5.  Legen Sie fest, ob für den Kunden Teillieferungen und Teilfakturierungen möglich sind.
6.  Prüfen Sie, ob die Nummer für die Tourrangfolge und die Priorität richtig eingestellt sind.
7.  Wählen Sie im Menü `Start` > `Speichern`, um die Daten zu speichern.

Die Daten werden gespeichert. Sie können jetzt zu diesem Kunden Filialen und Mitarbeiter hinzufügen.

### Mitarbeiter und Filialen

**Lernziele**
- Filialen als zusätzliche Lieferanschriften verwenden.
- Vorgänge kennenlernen.

**Nutzen**
- Filialen dienen als weitere Lieferanschriften, wenn der Kunde z. B. mehrere Lagerorte hat. Im Auftrag kann jeweils die gültige Lieferanschrift ausgewählt werden.
- Zusätzliche Angaben zu Mitarbeitern dienen der Kontaktpflege, so dass zuständige Personen direkt angesprochen werden können.

**Merke**
- **Filialen**: Für die Filialen Ihrer Marktpartner werden die gleichen Daten hinterlegt, wie für den Hauptsitz.
- **Mitarbeiter**: Die Daten zu Mitarbeitern Ihres Kunden dienen zur Information.
- **Vorgang**: Über Vorgänge können Sie bestimmte Kontakte mit dem Kunden verfolgen.

#### Filialen des Kunden

Für die Filialen Ihrer Marktpartner werden die gleichen Daten hinterlegt, wie für den Hauptsitz. Die Daten des Hauptsitzes werden als Vorbelegung in den entsprechenden Feldern angezeigt und können angepasst werden.

**Standard-Lieferanschrift als Filiale anlegen**
Neben der Firmenanschrift können Sie weitere Anschriften für die Lieferungen und für die Rechnungen angeben. Diese Anschriften werden als Filialen erfasst. Für die Filiale muss dann im Register `Adresse` im Bereich `Anschrift` die Checkbox `Standard` aktiviert werden, wenn diese Filiale die Standardlieferanschrift ist.

#### Mitarbeiter des Kunden

Die Namen der Mitarbeiter Ihres Kunden können Sie zur Information hinterlegen. Als zusätzliche Informationen können Sie Angaben zur Abteilung, in der er arbeitet, seiner Funktion, und seine Durchwahl ergänzen. Sie können kennzeichnen, ob der Mitarbeiter alleiniger Ansprechpartner bei Fragen zum Auftrag und/oder zum Vertrieb ist. Diese Angaben können für Auswertungen über die ODBC-Schnittstelle herangezogen werden.

#### Vorgang

Über sogenannte Vorgänge können Sie z. B. verfolgen, wann und welcher Mitarbeiter des Kunden angerufen hat, um Infomaterial zu erhalten. Dazu dokumentieren Sie auch, wann und durch wen der Vorgang verfolgt und abgeschlossen wurde.

#### Filialen hinzufügen

Wählen Sie die Nummer für die Filiale so, dass aus ihr die Verbindung zum Hauptsitz erkennbar ist, z. B. 10000 für den Kunden, 10100, 10200, ... für die Filialen.

**So legen Sie eine Filiale an**
1.  Wählen Sie im Menü `Stammdaten` > `Marktpartner` > `Kunde` > `Kunden`. Der Dialog `Partnerverwaltung` wird geöffnet.
2.  Suchen Sie den Datensatz des gewünschten Partners.
3.  Wählen Sie im Menü `Funktionen` > `Gruppe Details` > `Filiale`.
4.  Tragen Sie mindestens die Adress- und Kommunikationsdaten ein. Weitere Daten können Sie in den Registern ergänzen, so wie in der Handlungssequenz zum Anlegen der Kundendaten beschrieben.
5.  Wählen Sie im Menü `Start` > `Speichern`, um die Daten zu speichern. Die Daten werden gespeichert. Im Register `Adresse` sind die Checkbox `Standard` und die Schaltfläche `[zurück zur Hauptfirma]` freigeschaltet.
6.  Passen Sie die Daten der Filiale an, z. B. die Touren. Beachten Sie folgende Einstellungen:
    - Aktivieren Sie die Checkbox `Standard`, wenn diese Filiale die Standardanschrift für Lieferungen ist.
    - Aktivieren Sie die Checkbox `eigenständige Filiale`, wenn diese Filiale eigene Aufträge vergeben kann.
7.  Wählen Sie im Menü `Start` > `Speichern`, um die Daten zu speichern. Die Daten werden gespeichert.
8.  Klicken Sie auf die Schaltfläche `[zurück zur Hauptfirma]`, um den Dialog zu schließen. Die Daten der Hauptfirma werden wieder angezeigt.

#### Mitarbeiter hinzufügen

Mit den Daten zu Mitarbeitern Ihrer Marktpartner können Sie auch angeben, für welchen Bereich dieser Mitarbeiter zuständig ist. Diese Angabe wird lediglich als Information hinterlegt.

**So legen Sie die Mitarbeiterdaten eines Marktpartners an**
1.  Wählen Sie im Menü `Stammdaten` > `Marktpartner` > `Kunde` > `Kunden`. Der Dialog `Partnerverwaltung` wird geöffnet.
2.  Suchen Sie den Datensatz des gewünschten Partners.
3.  Wählen Sie im Menü `Funktionen` > `Gruppe Details` > `Mitarbeiter`.
4QRCode 2:
Wenn bereits Mitarbeiter des Kunden eingetragen sind, werden deren Daten angezeigt.
4.  Klicken Sie auf `[Neu]`, um die Felder freizuschalten. Wenn bereits Mitarbeiter des Kunden eingetragen sind, können Sie die Daten überschreiben.
5.  Tragen Sie mindestens den Namen und die Telefonnummer ein.
6.  Ergänzen Sie weitere Angaben, sofern diese für die Kommunikation mit dem Mitarbeiter wichtig sind, z. B. die Funktion des Mitarbeiters. Damit haben Sie die wesentlichen Daten eingetragen.
7.  Klicken Sie auf `[Neu]`, um die Daten zu speichern. Die Daten werden gespeichert. Sie können jetzt Daten von weiteren Mitarbeitern anlegen, indem Sie die Schritte 5 bis 7 wiederholen.
8.  Klicken Sie auf `[Ende]`, um den Dialog zu schließen. Der Dialog `Partnerverwaltung` wird wieder im Vordergrund angezeigt. Im Register `Mitarb./Filiale/Vorg.` werden alle Mitarbeiter aufgelistet.

### Texte

**Lernziele**
- Kundenspezifische Texte eintragen.
- Textkennzeichen kennenlernen.

**Nutzen**
- Texte dienen der Information über bestimmte Sachverhalte, z. B. über Sonderwünsche bei der Produktion.

**Merke**
- **Kundenspezifische Texte**: Texte, die nur für einen einzigen Kunden gelten, können Sie in den Kundenstammdaten eingeben und automatisch im Dokument einfügen lassen.
- **Allgemeine Texte**: Häufig verwendete Texte können Sie als allgemeine Texte hinterlegen und über die Kundenstammdaten automatisch im Dokument einfügen lassen.
- **Textkennzeichen**: Über die Textkennzeichen können Sie steuern, in welchen Dokumenten die Texte gedruckt werden sollen, z. B. in Auftragsbestätigungen, in Lieferscheinen.

#### Texte und Textkennzeichen

Immer wiederkehrende Texte können Sie hinterlegen und automatisch z. B. im Dokument einfügen lassen. Bei diesen Texten wird zwischen System-, Standard- und Rahmentexten unterschieden.

Standardtexte werden anhand von Textkennzeichen unterschieden, z. B. das Textkennzeichen `O` für Angebote, `P` für Produktion, `L` für Lieferschein. Die Textkennzeichen können Sie nach den Erfordernissen in Ihrem Betrieb hinterlegen.

> **Beispiele**
> - **Info-Texte (Textkennzeichen I)**: Diese Texte sollen in allen Dokumenten gedruckt werden, z. B. die Ankündigung von Betriebsferien.
> - **Lieferscheinspezifische Texte (Textkennzeichen L)**: Diese Texte sollen nur auf den Lieferscheinen gedruckt werden, z. B. die Reklamationsfrist.
> - **Angebotstexte (Textkennzeichen O)**: Diese Texte sollen nur auf Angeboten gedruckt werden, z. B. Gültigkeitsdauer des Angebots.

Die Textkennzeichen dienen nicht nur der Gruppierung Ihrer Standardtexte. Über die Textkennzeichen können auch Sie steuern, wann die Texte gedruckt werden sollen.

> **Beispiel**
> Produktionstexte (Textkennzeichen P) sollen auf dem Lieferschein nicht gedruckt werden. Pro Formular legen Sie in der Formularverwaltung fest, welche Textkennzeichen nicht gedruckt werden sollen.

Für jede ISO-Einheit können spezielle Rahmentexte hinterlegt und dem Produkt zugeordnet werden.

In den Stammdaten der Partner und der Produkte können Texte hinterlegt werden, die immer in die Dokumente übernommen werden. Dies können entweder Standardtexte sein oder der Text wird nur für den Partner oder das Produkt eingetragen.

> **Ausführliche Beschreibung der Texte**
> Die Texte sind ausführlich im Tutorial 2 beschrieben.
> (Siehe Tutorial 2, "Texte" auf Seite B-461)

#### Text in Kundenstammdaten erfassen

In diesem Beispiel wird ein Text in den Kundenstammdaten beschrieben. Auf die gleiche Weise können Sie Texte für Lieferanten oder Produkte erfassen.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
- "So ordnen Sie einen Standardtext zu" auf Seite B-69
- "So tragen Sie einen kundenspezifischen Text ein" auf Seite B-71

> **Schriftart und -größe**
> Die Einstellungen für die Schriftart und die Schriftgröße gelten nur für die Anzeige auf dem Bildschirm. Sie werden nicht in den Druck übernommen.

**So ordnen Sie einen Standardtext zu**
1.  Wählen Sie im Menü `Stammdaten` > `Marktpartner` > `Kunde` > `Kunden` > Register `Texte`.
2.  Klicken Sie Symbolschaltfläche, um die Eingabefelder freizuschalten.
3.  Geben Sie die Nummer des gewünschten Standardtextes ein oder wählen Sie ihn über die Lupe aus. Wenn Sie die Textnummer direkt eintragen, müssen Sie mit der `<Tab>`-Taste ins nächste Feld springen, damit der Text eingelesen wird.
4.  Wählen Sie im Menü `Start` > `Speichern`, um die Daten zu speichern. Der Standardtext wird dem Textkennzeichen entsprechend auf die jeweiligen Formulare gedruckt oder an die Produktion übergeben. Auf die gleiche Weise tragen Sie einen Rahmentext ein.

**So tragen Sie einen kundenspezifischen Text ein**
1.  Wählen Sie im Menü `Stammdaten` > `Marktpartner` > `Kunde` > `Kunden` > Register `Texte`.
2.  Klicken Sie Symbolschaltfläche, um die Eingabefelder freizuschalten.
3.  Wählen Sie das Textkennzeichen aus, z. B. `I` Informationstexte. Das Textkennzeichen entscheidet, wie der Text verwendet wird. Wenn der Text z. B. an die Produktion übergeben werden soll, müssen Sie das Kennzeichen `P` wählen. Wenn Sie kein Textkennzeichen eingeben, wird der Text nicht übergeben. Lassen Sie im Feld Nummer die `0` stehen.
4.  Schreiben Sie den gewünschten Text in das Eingabefeld.
5.  Wählen Sie im Menü `Start` > `Speichern`, um die Daten zu speichern. Die Daten werden gespeichert und dem Textkennzeichen entsprechend nur für diesen Kunden verwendet. Auf die gleiche Weise können Sie Texte für einzelne Lieferanten, Partner oder Produkte erstellen.

### Klassifikatoren

**Lernziele**
- Klassifikatoren anlegen.
- Klassifikatorenwerte zuweisen.

**Nutzen**
- Klassifikatoren dienen als Filter für zusätzliche Auswertungen, z. B. Umsatz.

**Merke**
- **Klassifikatoren**: Klassifikatoren werden für alle Marktpartner gemeinsam oder jeweils für Kunden, Lieferanten oder Partner angelegt.
- **Klassifikatorenwerte**: Klassifikatorenwerte können numerisch, alphanumerisch oder als Datum eingetragen werden.

#### Klassifikator und Klassifikatorenwert

Klassifikatoren legen Sie an, um sie als Filter für zusätzliche Auswertungen zu nutzen, z. B. Umsatz, Geburtstag, Hobbys. Dazu definieren Sie, ob der Wert numerisch, alphanumerisch oder als Datum eingetragen wird. Nicht mehr benötigte Klassifikatoren können Sie löschen.

Um mit Klassifikatoren zu arbeiten, sind zwei Schritte erforderlich:
- Sie legen einen Klassifikator an. In der Klassifikatorendefinition legen Sie fest, wie der Klassifikator heißt und mit welchen Werten er belegt werden kann.
- Sie weisen einen Klassifikatorenwert zu.

#### Klassifikator anlegen

Klassifikatoren für Kunden, Lieferanten oder Partner können Sie auch aus der jeweiligen Partnerverwaltung heraus anlegen.

**So legen Sie einen Klassifikator an**
1.  Wählen Sie `Stammdaten` > `Marktpartner` > `Kunde` > `Kunden` > Menü `Funktionen` > `Gruppe Klassifikatoren` > `Klassifikatorendefinition`.
Im Register `Gemeinsam` hinterlegte Klassifikatoren gelten für alle Marktpartner. In den drei weiteren Registern legen Sie die Klassifikatoren an, die nur für die jeweilige Gruppe gelten.
2.  Wählen Sie das gewünschte Register, z. B. `Gemeinsam`. In diesem Register legen Sie einen Klassifikator an, der für alle Marktpartner gilt.
3.  Klicken Sie auf `[Neu]`, um die nächste Zeile freizuschalten.
4.  Tragen Sie die Werte ein:
    - Im Feld `Bezeichnung` z. B. **Umsatz Gruppen**.
    - Im Feld `Bemerkung` z. B. **ABC Klassifizierung**.
5.  Markieren Sie eine der Checkboxen, um zu definieren, ob der Wert numerisch, alphanumerisch oder als Datum eingetragen werden muss. Diese Angabe bestimmt, in welcher Form Sie die Klassifikatorenwerte in der Partnerverwaltung eingeben dürfen und wie sie ausgewertet werden.
6.  Klicken Sie auf `[Neu]`, um die Daten zu speichern. Die Daten werden gespeichert. Alle Klassifikatoren im Register `Gemeinsam` werden bei allen Marktpartnern in der Partnerverwaltung im Register `Klassifikatoren` angezeigt. Alle anderen Klassifikatoren werden nur bei den entsprechenden Marktpartnern angezeigt.

#### Klassifikatorenwert zuweisen

In der Klassifikatorendefinition legen Sie fest, welche Art von Werten ein Klassifikator annehmen kann. Von dieser Definition ist abhängig, wie Sie den Wert zuweisen.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
- "So ordnen Sie einen alphanumerischen Wert zu" auf Seite B-76
- "So ordnen Sie einen numerischen Wert zu" auf Seite B-78

**So ordnen Sie einen alphanumerischen Wert zu**
1.  Wählen Sie im Menü `Stammdaten` > `Marktpartner` > `Kunde` > `Kunden` > Register `Klassifikatoren`.
2.  Markieren Sie einen Klassifikator mit dem Kennzeichen `A` (alphanumerisch). Die gesamte Zeile wird markiert.
3.  Wählen Sie im Menü `Funktionen` > `Gruppe Klassifikatoren` > `Klassifikatorenwerte`. Sie können auch doppelt in das Feld `Wert` des markierten Klassifikators klicken. Der Dialog `Klassifikatoren Wertzuordnung` wird geöffnet.
4.  Klicken Sie auf `[Neu]`, um die nächste Zeile freizuschalten. Die nächste Zeile wird freigeschaltet.
5.  Tragen Sie den neuen Wert ein, z. B. **Region Süd 1** für einen alphanumerischen Klassifikator für Umsatz.
6.  Klicken Sie auf `[OK]`, um die Daten zu speichern. Die Daten werden gespeichert. Sie können weitere Klassifikatoren anlegen, indem Sie die Schritte 4 bis 6 wiederholen. Diese Klassifikatorenwerte werden nicht automatisch für den aktuellen Partner übernommen.
7.  Markieren Sie die Zeile mit dem Wert und klicken Sie auf `[Übernahme]`, um dem Partner diesen Wert zuzuweisen. Der Dialog `Klassifikatoren Wertzuordnung` wird geschlossen und der Dialog `Partnerverwaltung` wird wieder im Vordergrund angezeigt.
8.  Wählen Sie im Menü `Start` > `Speichern`, um die Daten zu speichern. Die Werte werden gespeichert. Sie können jetzt zur Auswertung herangezogen werden.

**So ordnen Sie einen numerischen Wert zu**
1.  Wählen Sie im Menü `Stammdaten` > `Marktpartner` > `Kunde` > `Kunden` > Register `Klassifikatoren`.
2.  Setzen Sie im Bereich `Klassifikatoren` den Cursor in das Feld `Wert` eines Eintrags mit dem Kennzeichen `N` (numerisch) oder `D` (Datum).
3.  Wählen Sie im Kontextmenü `Einfügen`. Das Kontextmenü öffnen Sie mit der rechten Maustaste.
4.  Tragen Sie die Werte entsprechend der Vorgabe ein:
    - **N** (numerisch), z. B. **600000** (Umsatz)
    - **D** (Datum), z. B. **23.02.2012** (Geschenk zum Geburtstag des Abteilungsleiters)
    Mit `<Tab>` können Sie in die nächste Zeile wechseln, um einen weiteren Wert einzutragen.
5.  Wählen Sie im Menü `Start` > `Speichern`, um die Daten zu speichern. Die Daten werden gespeichert.

### Übungen

Die Übungen bauen auf einander auf. Sie werden daher die Daten, die Sie zu Übungszwecken anlegen, immer wieder benötigen. Kennzeichnen Sie diese Daten so, dass sie schnell erkannt werden können, z. B. mit dem Zusatz `Schulung` oder `Demo`.
- Legen Sie mindestens einen neuen Kunden an.
- Legen Sie Touren für Ihren Landkreis, für Abholung und eine Spedition an.
- Legen Sie die Kundengruppe `Schulung` an.
- Ordnen Sie jeweils Ihren Kunden einer Gruppe zu.
- Ordnen Sie den Kunden einer anderen Kundengruppe zu, wenn für ihn ein Auftrag zu ESG erfasst wird.
- Standardrundung
- Modus der Rechnungsstellung
- Teillieferung und Teilrechnung erlaubt
- Hinterlegen Sie eine abweichende Rechnungsanschrift.
- Definieren Sie eine der Anschriften als Standard-Lieferanschrift.
- Erfassen Sie für Ihren Schulungskunden einen Text, der nur für ihn gilt und nur auf Produktionspapiere gedruckt wird.
- Legen Sie drei Klassifikatoren mit unterschiedlichen Eigenschaften (numerisch, alphanumerisch, Datum) an.
- Weisen Sie Ihrem Schulungskunden für jeden der Klassifikatoren einen Wert zu.

> **Demo-Daten sperren**
> Wenn Sie die Übungsaufgaben im tatsächlichen Betrieb machen, sollten Sie die Demo-Daten für die Verwendung sperren, sobald Sie Ihre Tests durchgeführt haben.

## Finanzen und Saldo

**Lernziele**
- Bedingungen für Rechnungen und die Zahlungen kennenlernen.
- Kalender und Zahlungstagverschiebung einrichten.
- Prüfung des Kreditlimits einstellen.

**Nutzen**
- Kundenrechnungen werden nach den Vorgaben aus den Kundenstammdaten erstellt.
- Saldo und Kreditlimit werden in der Auftragserfassung angezeigt, so dass die aktuellen Aufträge und offenen Posten berücksichtigt werden können.

**Merke**
- **Fälligkeit**: Fälligkeiten werden automatisch errechnet. Dazu geben Sie den gewünschten Modus an und legen die Daten für die Rechnungslegung fest.
- **Zahlungsziel**: Das Belegdatum und der Tag der Rechnungslegung ergeben das erste Bezugsdatum. Dieses dient als Basis zur Berechnung des Zahlungsziels.
- **Zahlungstagverschiebung**: Damit während der Betriebsferien des Kunden keine Rechnungen fällig werden, kann der entsprechende Zeitraum im Kundenkalender angegeben werden.
- **Zahlungsbedingung**: Jede Zahlungsbedingung kann mehrere Stufen von Zahlungszielen und Prozentsätzen für das Skonto berücksichtigen.
- **Kontonummer**: Die Kundennummer wird als Hauptkonto verwendet und an die FiBu übergeben. Als Hauptdebitor, an den die Rechnungen und Gutschriften gesendet werden, kann die Kundennummer einer Filiale des Kunden verwendet werden.
- **Kreditlimit**: Für jeden Kunden kann ein Wert für das versicherte Kreditlimit und ein Wert für ein internes (unversichertes) Kreditlimit angegeben werden. Das Kreditlimit kann automatisch bei der Erfassung neuer Aufträge geprüft werden.
- **Steuern**: Nur die Steuern können berechnet werden, die als Steuersatz hinterlegt und dem Kunden zugewiesen sind.
- **Währungen**: Preise können in unterschiedlichen Währungen gepflegt werden. Dabei können Aufträgen in Landeswährung (Eigenwährung) oder Fremdwährung erfasst werden. Für statistische Vergleiche wird immer die Landeswährung herangezogen. Die Währungsbeträge werden dazu von `A+W Business` umgerechnet.

### Vorgaben für die Zahlung

Für jeden Kunden legen Sie die Vorgaben für die Rechnungen im Register `Finanzen` fest.

Die Bankdaten des Kunden hinterlegen Sie, z. B, um diese für Gutschriften oder den Belegdruck zu verwenden.

Zu den Kundenrechnungen geben Sie an:
- Modus der Fälligkeitsberechnung
- Angabe des Tags der Rechnungslegung
- Zahlungsbedingung
- Gültiger Steuersatz: Dabei ist es möglich, bis zu 5 verschiedene Steuersätze zu aktivieren.

Die Steuersätze selbst werden unter `Finanzen` > `Steuer` hinterlegt. Zusätzlich können Sie in den Firmendaten noch angeben, ob die Steuer pro Position oder pro Stücklisten-Komponente berechnet werden soll. Diese Angabe gilt dann für alle Kunden. Die Einstellungen in den Firmendaten sind in der Softwarereferenz beschrieben.

### Fälligkeitsberechnung

Fälligkeiten werden automatisch errechnet. Dazu geben Sie den gewünschten Modus an und legen die Daten für die Rechnungslegung fest:
- Tag der Rechnungslegung, z. B., wenn nicht das Rechnungsdatum ausschlaggebend ist.
- Zahlungsziel (Bruttotage)
- Zahlungstage

| Modus | Text |
| :--- | :--- |
| 0 | 1. Bezugsdatum |
| 1 | 1. Bezugsdatum + Bruttotage |
| 2 | 1. Bezugsdatum + Bruttotage + Rundung auf 1. Zahlungstag oder Monatsende |
| 3 | 1. Bezugsdatum + Bruttotage + Rundung auf den 15. oder Monatsende |
| 4 | 1. Bezugsdatum + Bruttotage + Rundung auf den 10., den 20. oder Monatsende |
| 5 | 1. Bezugsdatum wird auf das Monatsende gerundet + Bruttotage (0/30/60/90). Das errechnete Zahlungsziel wird immer auf das Monatsende gerundet. **Achtung**: Bei Kennzeichen 5 und 6 muss der Wert im Feld Bruttotage durch 30 teilbar sein. 30 Tage = 1 Monat, 60 Tage = 2 Monate, 90 Tage = 3 Monate, um die das erste Bezugsdatum erhöht wird. |
| 6 | 1. Bezugsdatum wird auf das Monatsende gerundet + Bruttotage (0/30/60/90) + Zahlungstag |
| 7 | 1. Bezugsdatum + Bruttotage + Rundung auf 1., 2. oder 3. Zahlungstag |
| 8 | 1. Bezugsdatum + Bruttotage + Rundung auf 1. oder 3. Zahlungstag in Abhängigkeit vom 2. Zahlungstag |
| 11 | Fälligkeitsdatum = Lieferdatum + Zahlungsziel |

Beispiele für die Berechnung von Fälligkeiten finden Sie im Part Verkauf.
(Siehe Verkauf, "Fälligkeitsberechnung" auf Seite C-209)

### Rechnungslegung

Das Belegdatum und der Tag der Rechnungslegung ergeben das erste Bezugsdatum. Dieses dient als Basis zur Berechnung des Zahlungsziels.
- **Tag der Rechnungslegung = 0**: Das 1. Bezugsdatum ist gleich Belegdatum.
- **Tag der Rechnungslegung ≠ 0**: Das Belegdatum wird auf den Tag der Rechnungslegung gerundet und ergibt das erste Bezugsdatum.

**Beispiele**

| Belegdatum | RLT | 1. Bezugsdatum | Anmerkung |
| :--- | :-: | :--- | :--- |
| 13.03. | 0 | 13.03. | 1. Bezugsdatum = Belegdatum |
| 13.03. | 25 | 25.03. | Das Belegdatum wird auf den 25. des gleichen Monats gerundet. |
| 27.03. | 25 | 25.04. | Der Tag der Rechnungslegung ist kleiner als das Belegdatum, aus diesem Grund wird das Belegdatum auf den 25. des Folgemonats gerundet. |

*RLT = Rechnungslegungstag*

### Zahlungstagverschiebung

Sie können für die Berechnung des Zahlungstags eine Verschiebung festlegen, z. B. damit keine Rechnungen während der Betriebsferien des Kunden fällig werden. Den Zeitraum für die Verschiebung stellen Sie im Kundenkalender ein.
Die Berechnung bezieht sich auf die Einträge im Kundenkalender. Die Art der Verschiebung gilt unabhängig von den Tagen aus dem Kundenkalender.
(Siehe "Kundenkalender bearbeiten" auf Seite B-103)

| Option | Art der Verschiebung |
| :--- | :--- |
| 0 | Keine Verschiebung |
| 1 | **Hälftige Aufteilung** - Fälligkeitsdaten werden hälftig aufgeteilt: Eine Hälfte des Betrags wird in einem bestimmten Zeitbereich vor dem ursprünglichen Fälligkeitsdatum fällig. Die andere Hälfte wird in einem bestimmten Zeitbereich nach dem ursprünglichen Fälligkeitsdatum fällig. |
| 2 | **Verschiebung um einen Zeitbereich** - Fälligkeitsdaten werden um einen bestimmten Zeitbereich in die Zukunft verschoben. |
| 3 | Entspricht Option 2 plus Zuschlag. Bei der Wahl dieser Option muss ein entsprechender Zuschlag angelegt sein. |

#### Beispiele

**Ausgangssituation:**
- Rechnungsbetrag: 300 Euro
- Rechnungsdatum: 10.07.
- Kunde akzeptiert keine Fälligkeiten im Monat August (01.08. - 31.08.)

**Beispiel 1**
Zahlungsziel 30 Tage = Fälligkeitsdatum 10.08.
- **Option 1: Hälftige Aufteilung**
    - Fälligkeitsdatum 1: 10.07. = 150 €
    - Fälligkeitsdatum 2: 10.09. = 150 €
    - Der Rechnungsbetrag wird je zur Hälfte vor und nach den Betriebsferien fällig.
- **Option 2: Verschiebung um einen Zeitbereich**
    - Fälligkeitsdatum: 10.09. = 300 €
    - Der gesamte Rechnungsbetrag wird nach den Betriebsferien fällig.
- **Option 3: Entspricht Option 2 + Zuschlag**
    - Fälligkeitsdatum: 10.09. = 303 € (300 € + 1%)
    - Der gesamte Rechnungsbetrag wird nach den Betriebsferien fällig. Zusätzlich wird ein Zuschlag erhoben.

**Beispiel 2**
Zahlungsziele 30, 60 Tage
- Fälligkeitsdatum 1: 10.08. = 150 €
- Fälligkeitsdatum 2: 10.09. = 150 €
    - **Option 1: Hälftige Aufteilung**
        - Fälligkeitsdatum 1: 10.07. = 75 €
        - Fälligkeitsdatum 2: 10.09. = 225 €
        - Zum 1. Fälligkeitsdatum sind 150 € fällig. Dieser Betrag wird hälftig aufgeteilt, so dass zum vorgezogenen 1. Fälligkeitsdatum 75 € fällig werden. Die restlichen 75 € werden zum 2. Fälligkeitsdatum fällig, so dass zu diesem Datum 150 € + 75 € fällig sind.
    - **Option 2: Verschiebung um einen Zeitbereich**
        - Fälligkeitsdatum: 10.09. = 300 €
        - Zum 1. Fälligkeitsdatum sind 150 € fällig. Dieser Betrag wird zum 2. Fälligkeitsdatum fällig, so dass zu diesem Datum 300 € fällig sind.
    - **Option 3: Entspricht Option 2 + Zuschlag**
        - Fälligkeitsdatum: 10.09. = 303 € (300 € + 1%)
        - Der gesamte Rechnungsbetrag wird zum 2. Fälligkeitsdatum verschoben. Zusätzlich wird ein Zuschlag berechnet.

**Beispiel 3**
Zahlungsziele 30, 60, 90 Tage
- Fälligkeitsdatum 1: 10.08. = 100 €
- Fälligkeitsdatum 2: 10.09. = 100 €
- Fälligkeitsdatum 3: 10.10. = 100 €
    - **Option 1: Hälftige Aufteilung**
        - Fälligkeitsdatum 1: 10.07. = 50 €
        - Fälligkeitsdatum 2: 10.09. = 150 €
        - Fälligkeitsdatum 3: 10.10. = 100 €
        - In diesem Beispiel ist nur das 1. Fälligkeitsdatum betroffen, an dem 100 € fällig wären. Dieser Betrag wird aufgeteilt, so dass die erste Hälfte (50 €) vor dem ursprünglichen Datum fällig wird. Die zweite Hälfte wird am 2. Fälligkeitsdatum zusammen mit dem ursprünglichen (Drittel-)Betrag fällig (50 €+100 €).
    - **Option 2: Verschiebung um einen Zeitbereich**
        - Fälligkeitsdatum 1: 10.09. = 200 €
        - Fälligkeitsdatum 2: 10.10. = 100 €
        - In diesem Beispiel wird der Betrag zum 1. Fälligkeitsdatum auf das 2. Fälligkeitsdatum verschoben.
    - **Option 3: Entspricht Option 2 + Zuschlag**
        - Fälligkeitsdatum 1: 10.09. = 201 € (200 € + 1%)
        - Fälligkeitsdatum 2: 10.10. = 100 € (100 €)
        - In diesem Beispiel wird der Betrag zum 1. Fälligkeitsdatum auf das 2. Fälligkeitsdatum verschoben und ein Zuschlag auf die verschobene Summe erhoben.

Der Kundenkalender ist in einer separaten Einheit beschrieben.
(Siehe "Kundenkalender bearbeiten" auf Seite B-103)

### Kalender

Um Dokumente erfassen zu können, muss im allgemeinen Kalender das aktuelle Kalenderjahr angelegt sein. Damit die Termine in der Auftragserfassung berechnet werden können, z. B. Liefertermine, müssen die täglichen Arbeitszeiten hinterlegt werden. Für diese Berechnungen müssen Wochenenden und Feiertage (ohne Arbeitsstunden) eingetragen werden.

Dazu können Sie auch Betriebsferien eintragen, indem Sie die Tagesarbeitszeit im Zeitraum der Ferien auf null setzen. Bei der Berechnung von Lieferterminen werden diese Tage berücksichtigt.

Auf dem allgemeinen Kalender baut der Kundenkalender auf. Dieser dient vor allem dazu, die Tage für die Zahlungsverschiebung pro Kunden zu hinterlegen.

### Zahlungsbedingungen

Die Zahlungsbedingungen eines jeden Kunden geben Sie in den Kundenstammdaten im Register `Finanzen` an. Im Auftragskopf werden die Zahlungsbedingungen aus den Kundendaten eingelesen und können überschrieben werden. Die Vorgaben zu den Berechnungen des Skontos legen Sie im Dialog `Zahlungsbedingungen` fest.

Sie können in einer Zahlungsbedingung mehrere Stufen einrichten, nämlich in vollständigen Sätzen mit bis zu fünf Zahlungszielen und drei Prozentsätzen für das Skonto. Daneben können Sie beliebig viele Bedingungen anlegen, die nur das Skonto berücksichtigen.

> **Beispiel**
> 
> | Skonto | Satz 1 | Tage 1 | Satz 2 | Tage 2 | Ziel 1 |
> | :--- | :--- | :--- | :--- | :--- | :--- |
| | 3,00% | 10 | 1,5% | 20 | 30 |
>
> In diesem Beispiel sehen Sie, dass der Kunde in den ersten 10 Tagen 3 % Skonto abziehen kann, in den nächsten 10 Tagen aber nur noch 1,5 %. Nach 30 Tagen ist die Rechnung ohne jegliche Abzüge fällig.

### Zahlungswege, Bonität

Zahlungswege und Bonität dienen der Information. Die Einträge werden in einfachen Basistabellen hinterlegt. Sie können beliebig erweitert werden.

### Hauptkonto oder abweichende Rechnungsanschrift

Sie können die Kundennummer des Hauptdebitors (Filiale) eintragen, an den die Rechnungen und Gutschriften gesendet werden. Voraussetzung hierfür ist, dass dieser als Filiale des Kunden angelegt ist. Das Hauptkonto entspricht also der Kundennummer des Hauptdebitors. Wenn das Feld leer bleibt, wird automatisch die Nummer des aktuellen Kunden als Hauptkonto verwendet.

### Banken

Für den Zahlungsverkehr mit Ihren Kunden und Lieferanten hinterlegen Sie die Bankdaten.

Die Bank weisen Sie den Partnern in der Partnerverwaltung im Register `Finanzen` zu. In der Partnerverwaltung können Sie die IBAN errechnen lassen, wenn mindestens folgende Daten für die Bank hinterlegt sind: BLZ, Länderkennzeichen und Kontonummer (in den Kundenstammdaten). Diese Funktion starten Sie in der Partnerverwaltung über das Menü `Funktionen`.

> **Bank der Firma und Mandanten**
> Die Bankverbindungen für Ihre Firma und Ihre Mandanten hinterlegen Sie im Menü `Stammdaten` > `Firma` > `Banken`. Dabei greifen Sie ebenfalls auf die Bankdaten zu, die unter `Finanzen` angelegt sind.

### Kreditlimit für Kunden

Sie können für jeden Kunden zwei unterschiedliche Werte für ein Kreditlimit festlegen und automatisch bei der Erfassung neuer Aufträge prüfen lassen. Das Kreditlimit 2 kann als hausinternes, nicht versichertes Kreditlimit genutzt werden.

Für die Prüfung des Kreditlimits müssen Sie folgende Entscheidungen treffen:
- **Das Kreditlimit pro Kunde in den Kundendaten bestimmen.**
    - **Kreditlimit 1**: Bei diesem Wert geben Sie das versicherte Kreditlimit an.
    - **Kreditlimit 2**: Bei diesem Wert geben Sie ein internes (unversichertes) Kreditlimit an, das Sie aufgrund der Bonität des Kunden gewähren.
- **Reaktion bei Überschreitung des Kreditlimits festlegen:**
    - In der Regel wird der Status erhöht. Wenn das Kreditlimit überschritten wird, werden neue Aufträge auf einen definierten Status gesetzt und für die Bearbeitung gesperrt. Dieser Status kann manuell zurückgesetzt werden, um die Aufträge zur Bearbeitung freizugeben.
    - Ein neuer Auftrag kann erfasst und gespeichert werden. Eine Meldung macht aber auf den Umstand aufmerksam, dass damit das Kreditlimit überschritten wird. Es liegt dann in Ihrer Entscheidung, den Auftrag weiter zu bearbeiten oder abzulehnen.

#### Art der Prüfung

In der Partnerverwaltung stellen Sie die entsprechenden Kennzeichen für jeden Kunden bzw. für jede Filiale individuell ein.
- Keine Prüfung
- Limit 1 + Meldung Limit 2
- Limit 2 + Meldung Limit 1
- Prüfung von Limit 1
- Prüfung von Limit 1 und 2
- Prüfung von Limit 2
- Vorauskasse

Wenn Sie mit Filialen arbeiten, kann das Kreditlimit auf zwei Ebenen geprüft werden:
- Das Kreditlimit der Filiale selbst wird geprüft.
- Das Kreditlimit des Hauptkunden wird geprüft:
    - Prüfung über das Filialkennzeichen
    - Prüfung über den Eintrag im Feld `Hauptkonto`: Das Kreditlimit der Filiale wird ignoriert.

#### Anzeige des aktuellen Auftragsvolumens

Im Auftragskopf wird der Betrag des Kreditlimits zusammen mit den offenen Posten angezeigt. Damit können Sie in jedem einzelnen Auftrag prüfen und ggf. mit dem Kunden absprechen, ob ein neuer Auftrag erfasst werden kann. In diesem Bereich werden die Daten jeweils nach der Übergabe an die FiBu und nach deren Rückmeldung aktualisiert.

#### Keine Prüfung

Wenn das Kreditlimit nicht geprüft wird, werden die aktuellen Beträge lediglich angezeigt. Bei der Überschreitung des Kreditlimits und bei Vorauskasse können die Aufträge grundsätzlich weiter bearbeitet werden. Angebote können unabhängig vom Kreditlimit und von möglichen Sperren erfasst werden.

#### Rückmeldung von Offenen Posten

Im Zusammenspiel mit einem Programm zur Finanzbuchhaltung (FiBu), das offene Posten zurückmeldet, erhalten Sie einen aussagekräftigen Überblick über den aktuellen Finanzstatus eines Kunden. Wenn Sie ohne OP-Rückmeldung arbeiten, werden bei der Prüfung des Kreditlimits bzw. des Saldos alle Aufträge berücksichtigt, die noch nicht an die FiBu übergeben wurden.

Wenn in den Firmendaten die Funktion `Einzel-OP-Rückmeldung` aktiviert ist, kann in der Auftragserfassung und der Kundenverwaltung eine OP-Abfrage für den jeweiligen Kunden gestartet werden. Dabei werden alle offenen Rechnungen angezeigt.

Kunden, deren Saldo seit dem letzten Einlesen der offenen Posten ausgeglichen wurde, werden mit dem Saldo 0 in der Kundenverwaltung aktualisiert.

#### Überschreitung des Kreditlimits

Über die Firmendaten und die Statuszuordnung legen Sie fest, wie `A+W Business` bei der Überschreitung des Kreditlimits reagieren soll:
- Über die Statuszuordnung ist ein Sperrstatus festgelegt, nach dem keine weitere Erfassung möglich ist.
- Der Status wird nur erhöht, wenn die Option `Status erhöhen, wenn Kreditlimit überschritten` in den Firmendaten aktiviert ist.

In der Kombination dieser beiden Einstellungen können keine neuen Aufträge erfasst werden, wenn das Kreditlimit erreicht oder überschritten wird.

Die Meldung `Kreditlimit ist überschritten, Kunde ist gesperrt!` wird auch vor dem Kopieren des Dokuments angezeigt. Der Kopiervorgang wird nicht durchgeführt. Das Kreditlimit wird auch dann geprüft, wenn in einem erfassten und gespeicherten Auftrag ein anderer Kunde eingetragen wird.

Wenn ein neuer Auftrag bearbeitet werden soll, obwohl das Kreditlimit überschritten ist, muss der Auftragsstatus manuell heruntergesetzt werden. Nach der manuellen Statusumsetzung wird der Status für diesen Auftrag nicht mehr automatisch hochgesetzt. Die Statusumsetzung ist ausführlich im Part Verkauf beschrieben.

Aufträge können vom Kunden über die EDI-Schnittstelle (elektronisch) übergeben werden. Wenn ein Auftrag dabei das Kreditlimit überschreitet, erhält es den Status `Auftrag gesperrt wegen Kreditlimit`. Er wird trotz des Sperrstatus in die Kapazitätsplanung eingelastet. Dieser Auftrag muss manuell freigegeben werden, indem der Status heruntergesetzt wird. Danach wird er automatisch an die Produktion übergeben.

Die Funktionen der Statuserhöhung lernen Sie ausführlich in einer separaten Einheit kennen.
(Siehe Tutorial 2, "Statusverwaltung" auf Seite B-419)

#### Ablauf der Prüfung

1. Auftragskopf wird erfasst.
2. Prüfung aktiviert?
   - Nein: Gehe zu Schritt 7 (Auftrag erfassen).
   - Ja: Weiter zu Schritt 3.
3. Limit überschritten?
   - Nein: Gehe zu Schritt 7 (Auftrag erfassen).
   - Ja: Weiter zu Schritt 4.
4. Status umsetzen.
5. Sperre aktiv?
   - Nein: Eine Meldung wird angezeigt. Gehe zu Schritt 7 (Auftrag erfassen).
   - Ja: Weiter zu Schritt 6.
6. Status manuell zurücksetzen?
   - Nein: Auftrag nicht speichern.
   - Ja: Weiter zu Schritt 7.
7. Auftrag erfassen.
8. Rechnung an FiBu übergeben, auf OP-Rückmeldung warten.

Die manuelle Umsetzung des Status kann unterbunden werden, z. B. durch entsprechende Einstellungen in den Mitarbeiterrechten.

#### Kreditlimit-Analyse

In der Kreditlimit-Analyse können Sie über einen beliebigen Zeitraum die Entwicklung von bestimmten Finanzdaten eines oder mehrerer Kunden oder Kundengruppen auswerten.

Im Einzelnen werden dabei das Kreditlimit, der Betrag der offenen Posten, das Obligo, Saldo 1, Saldo 2 und die Auftragsbestände betrachtet.

Dabei gilt folgende Hierarchie:
1. Nicht gelieferte Aufträge
2. Gelieferte und noch nicht fakturierte Aufträge
3. Fakturierte, aber noch nicht an die FiBu übergebene Aufträge
4. Summe aus den Beständen 1 bis 3

Der Kreditlimit-Snapshot wird über einen täglich laufenden Task erzeugt, der die Finanzdaten auswertet. Wenn Sie diese Funktion nutzen wollen, wenden Sie sich bitte an Ihren Service-Mitarbeiter bei der A+W Software GmbH.

### Währungen

Für Ihre Kunden können die Preise in den Aufträgen in der Fremdwährung ausgewiesen werden, die Sie ihm zugewiesen haben. Dazu müssen die Währungen und die entsprechenden Wechselkurse hinterlegt und gepflegt werden.

Zum Erfassen von Aufträgen kann `A+W Business` auf der Basis von zwei verschiedenen Währungseinstellungen arbeiten:
- **Landeswährung (Eigenwährung)**: Die Währung im Land Ihres Hauptsitzes. In Europa ist dies in der Regel der Euro.
- **Fremdwährung**: Die von der Landeswährung abweichende Währung, in der z. B. im Auftrag die Preise für ausländische Kunden ausgewiesen werden.

Für statistische Vergleiche wird immer die Landeswährung herangezogen. Die Währungsbeträge werden dazu von `A+W Business` umgerechnet.

Für die Pflege der Preise und für die Berechnungen in den Aufträgen ergeben sich folgende Möglichkeiten:
- Die Preislisten und Aufträge werden in der Landeswährung geführt.
- Die Preislisten werden in der Landeswährung geführt, für ausländische Kunden können die Beträge in den Aufträgen wahlweise in Landes- oder Fremdwährung angezeigt werden. Dazu müssen die Wechselkurse für die Fremdwährungen hinterlegt und gepflegt werden.
- Die Preislisten werden in Fremdwährung geführt, in den Aufträgen können die Beträge wahlweise in Landes- oder Fremdwährung angezeigt werden. Für interne Zwecke wird der Wechselkurs hinterlegt.

In den Firmendaten legen Sie fest, welche Währung die Grundlage für Berechnungen ist und mit welcher Währung die Aufträge erfasst werden.

Wenn Sie mit Preislisten in einer anderen als der Landeswährung arbeiten, dann wählen Sie für die Anzeige der Preise in der Auftragserfassung die Einstellung `Euro`.

#### Preisberechnung bei Fremdwährungen

Sie können in `A+W Business` die Preise für den Einkauf und für den Verkauf pflegen, auch wenn diese in unterschiedlichen Währungen anfallen.

Die Berechnung von Preisen kann bei Fremdwährungen zu unterschiedlichen Ergebnissen führen, wenn Mengenpreise auf unterschiedlichen Ebenen ermittelt werden. Diese Einstellung legen Sie in den Firmendaten fest.

Wenn der Fremdwährungsbetrag auf der Basis der Stückliste und der Menge gebildet werden soll, können die Beträge auf folgende Arten errechnet werden.

- **Der Positionspreis wird aus dem Positionspreis in Landeswährung gebildet:**
    | Berechnung | Formel | Ergebnis |
    | :--- | :--- | :--- |
    | LW Preis/PE | x Faktor | = FW Preis/PE |
    | LW Bruttostückpreis | x Faktor | = FW Bruttostückpreis |
    | LW Nettostückpreis | x Faktor | = FW Nettostückpreis |
    | **LW Positionspreis** | **x Faktor** | **= FW Positionspreis** |
- **Der Positionspreis wird aus dem Nettostückpreis in Fremdwährung gebildet:**
    | Berechnung | Formel | Ergebnis |
    | :--- | :--- | :--- |
    | LW Preis/PE | x Faktor | = FW Preis/PE |
    | LW Bruttostückpreis | x Faktor | = FW Bruttostückpreis |
    | LW Nettostückpreis | x Faktor | = FW Nettostückpreis |
    | **FW Nettostückpreis** | **x Menge** | **= FW Positionspreis** |

*Legende: LW = Landeswährung, FW = Fremdwährung, PE = Preiseinheit*

### Skonto

`A+W Business` unterscheidet drei Berechnungsarten für das Skonto, die in den folgenden Beispielen dargestellt sind.

- **Auf Bruttobetrag:**
    | Berechnung | Berechnung/Basis | Wert |
    | :--- | :--- | :--- |
    | Netto 100,00 | 100,00 | 100,00 |
    | MwSt. 19% | | 19,00 |
    | Brutto | 119,00 | 119,00 |
    | Skonto 2% | | 2,38 |

- **Auf Nettobetrag (brutto vermindert um Skonto):**
    | Berechnung | Berechnung/Basis | Wert |
    | :--- | :--- | :--- |
    | Netto 100,00 | 100,00 | |
    | Skonto 2% | 2,00 | 98,00 |
    | MwSt. 19% | 98,00 | 18,62 |
    | Brutto | | 116,62 |

- **Auf Nettobetrag:**
    | Berechnung | Berechnung/Basis | Wert |
    | :--- | :--- | :--- |
    | Netto 100,00 | 100,00 | 100,00 |
    | Skonto 2% | | 2,00 |
    | MwSt. 19% | 98,00 | 18,62 |
    | Brutto | | 118,62 |

### Einstellungen in den Firmendaten

Wenn der Status bei der Überschreitung des Kreditlimits umgesetzt werden soll, muss in den Firmendaten im Register `Parameter` die Checkbox `Status erhöhen, wenn Kreditlimit überschritten` markiert sein.

In der Statuszuordnung muss zusätzlich festgelegt werden, ob die Auftragserfassung bei der Statuserhöhung gesperrt werden soll. Die Statuszuordnungen sind in einer separaten Einheit beschrieben.
(Siehe Tutorial 2, "Statusverwaltung" auf Seite B-419)

### Offene Posten

Für die Rückmeldung der offenen Posten (OP) müssen Sie in den Firmendaten neben dem eingesetzten FiBu-Programm auch die Einstellungen für die Aktualisierung prüfen.

### Finanzdaten des Kunden bearbeiten

Die folgende Handlungsanleitung baut auf den Schritten auf, die in der vorigen Einheit beschrieben wurden.

**So bearbeiten Sie die Daten für die Rechnungsstellung**
1.  Wählen Sie im Menü `Stammdaten` > `Marktpartner` > `Kunde` > `Kunden` > Register `Finanzen`.
2.  Prüfen Sie die Einstellung des Sperrkennzeichens. Wenn Sie die neuen Partnerdaten sofort verwenden wollen, müssen Sie die Einstellung `nicht gesperrt` wählen. Sie sollten die Daten dann sperren, wenn z. B. Preis- und Zahlungsvereinbarungen mit dem neuen Partner noch nicht abgeschlossen sind. In diesem Fall können noch keine Dokumente, d. h. Aufträge oder Bestellungen, für ihn erfasst werden.
3.  Legen Sie die Einstellungen für die Fälligkeiten fest, die Sie mit diesem Partner vereinbart haben.

