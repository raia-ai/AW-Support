---
title: "DE_AWBusiness_Lagerwirtschaft_6_1"
source: "DE_AWBusiness_Lagerwirtschaft_6_1.pdf"
tags: ["A+W Business", "Lagerwirtschaft", "Warehouse Management", "Software Documentation", "Tutorial", "Inventory Management", "Stammdaten", "ERP", "Glass Industry", "Windows and Doors"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a tutorial for the 'Lagerwirtschaft' (Warehouse Management) module of the A+W Business software. It covers the fundamental concepts of warehouse administration, including master data setup, inventory management, order processing for stock items, and performing physical inventory counts. The guide is intended for end-users who manage stock within the A+W Business environment."
long_description: "This is a comprehensive German-language tutorial for the A+W Business 'Lagerwirtschaft' (Warehouse Management) module, version 6.1. The document is designed to guide end-users through the core functionalities of managing inventory within the A+W software, which is specialized for the glass, windows, and doors industry. It begins with an introduction, revision history, and editorial notes. The main tutorial section is structured into several thematic blocks: 'Grundgedanken zum Lager' (Basic Concepts of the Warehouse), 'Stammdaten' (Master Data), 'Lagerwirtschaft' (Warehouse Management), 'Lagerartikel in Dokumenten' (Stock Items in Documents), and 'Inventur' (Inventory/Stock-taking). The 'Stammdaten' section details how to define warehouses, storage locations, categories, and product-specific settings. It explains the differences between various inventory management methods (e.g., by area, by piece, combined). The 'Lagerwirtschaft' section covers practical operations like stock movements (receipts, issues), inquiries, and automated ordering. The tutorial also explains how stock items are handled in sales and production documents, including reservations and automatic booking. Finally, it provides a step-by-step guide for conducting both periodic and initial physical inventories. The document includes a software reference section and a detailed table of contents."
---

# A+W Lagerwirtschaft
**A+W Business**
A+W - Software for Glass, Windows and Doors

---

---
## Vorspann
In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version/Datum | Beschreibung |
| :--- | :--- |
| 6.1/04-2020 | Neu: Lagerverwaltung > Kritischer Lagerbestand. |
| 6.0/10-2019 | Einstellungen Kistenmanagement in separaten Part übertragen und aus Part Lagerwirtschaft gelöscht. |
| 5.2/08-2019 | Einstellungen zur Inventurlisten und zum Druck von Kistenetiketten neu. |
| 5.10/01-2017 | Inventur überarbeitet, Dialog Lagerbewertung neu. |
| 5.00/08-2013 | Vollständige Überarbeitung der ALFAK-Dokumentation und Anpassung auf A+W Business. |
| 4.12/01-2013 | Layout an CI 2013 angepasst. |
| 4.11/02-2012 | Korrekturen |
| 4.10/11-2010 | Aktualisierung und Umstellung auf Doku-Konzept 2010 |
| 4.00/08-2009 | Vollständige Überarbeitung |
| 3.02/09-2008 | Abbildungen und Part-Nummer angepasst. |
| 3.01/08-2008 | Rechtschreibkorrekturen |
| 3.00/12-2003 | Struktureller Umbau auf Programmstruktur 4.0 |
| 2.00/08-2000 | Überarbeitung Lager |
| 1.00/03-1998 | Ersterstellung |

### Editorial
Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen
- Kontakte

### Anmerkungen zu diesem Dokument
Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Business gedacht.
Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.
Dieses Dokument beschreibt die volle Ausbaustufe von A+W Business.

### Urheberrechte
© 2020, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.
Die Dokumentation darf nur gemäß des Lizenzvertrages ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung von A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen
Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

### Kontakte
**A+W Software GmbH**
Am Pfahlgraben 4-10
D-35415 Pohlheim
- **Tel:** +49 6404 2051 0
- **Fax:** +49 6404 2051 877
- **Email:** aw.zentrale@a-w.com
- **Web:** http://www.a-w.com

## Inhalt

- **Vorspann** (G-3)
- **Revisionsübersicht** (G-3)
- **Editorial** (G-3)
- **Tutorial** (G-9)
    - **Übersicht** (G-11)
    - **Dokumentation** (G-12)
        - Aufbau des Tutorials (G-12)
        - Darstellungskonventionen (G-13)
    - **Menü-Übersicht** (G-14)
    - **Grundgedanken zum Lager** (G-16)
    - **Stammdaten** (G-19)
        - **Lager** (G-20)
            - Lagerdefinition (G-21)
            - Lagerkategorien (G-22)
            - Lagerebenen festlegen (G-22)
            - Lagerort definieren (G-24)
            - Lagerkategorien festlegen (G-27)
            - Übungen (G-28)
        - **Firmendaten** (G-29)
            - Lagerführungsmodus und Reservierung (G-30)
            - Firmendaten prüfen (G-31)
        - **Status** (G-34)
            - Statusänderungen durch Zu- und Abgänge (G-35)
            - Statuszuordnungen prüfen (G-35)
        - **Produktdefinition** (G-38)
            - Produkt (G-39)
            - Produkte als Lagerartikel (G-40)
            - Lagermaße (G-42)
            - Produktstammdaten prüfen (G-44)
            - Lagermaß anlegen (G-48)
            - Übungen (G-50)
        - **Preise** (G-51)
            - Einkaufspreis und Durchschnitts-EK (G-52)
            - Einstellung für EK-Ermittlung prüfen (G-57)
            - Preise prüfen (G-58)
            - Übungen (G-60)
        - **Lagerführung auf Stücklistenebene** (G-61)
            - Reservierung und Buchung für Stücklisten-Komponenten (G-62)
            - Einstellung prüfen (G-64)
            - Produkte prüfen (G-65)
    - **Lagerwirtschaft** (G-67)
        - **Lagerverwaltung** (G-68)
            - Elemente im Dialog Lagerverwaltung (G-69)
            - Lagerartikel (G-70)
            - Lager-Hauptartikel (G-70)
            - Mindestmengen (G-71)
            - Preise (G-72)
            - Lagerartikel anlegen (G-74)
            - Übungen (G-77)
        - **Lagerbuchung** (G-78)
            - Lagerbewegungen (G-79)
            - Buchungsarten (G-79)
            - Ab- und Zubuchung (G-80)
            - Ab- oder Zugang manuell erfassen (G-81)
            - Lagerort ändern (G-85)
            - Übungen (G-87)
        - **Abfragen** (G-88)
            - Lagerabfrage (G-89)
            - Buchungsjournal anzeigen (G-90)
            - Reservierte Lagerartikel drucken (G-92)
            - Lagerstatistik anzeigen (G-94)
            - Übungen (G-96)
        - **Lagerinformationen** (G-97)
            - Lagersuche (G-98)
            - Bestand (G-98)
            - Lagerinfo und zukünftiger Lagerbestand (G-99)
            - Bestände in der Lagersuche anzeigen (G-102)
            - Übungen (G-106)
        - **Lagerbestellung (automatisch)** (G-107)
            - Bestellvorschläge (G-108)
            - Lagerbestellung an den Einkauf übergeben (G-109)
            - Preise vor der Übergabe vergleichen (G-114)
            - Übungen (G-116)
    - **Lagerartikel in Dokumenten** (G-117)
        - **Auftragserfassung von Lagerartikeln** (G-118)
            - Reservierung und Buchung von Lagerartikeln (G-119)
            - Lagerartikel für Position suchen (G-120)
            - Buchungen prüfen (G-124)
            - Übungen (G-126)
        - **Manuelle Lagerbestellung** (G-127)
            - Lagerbestellung manuell erfassen (G-128)
            - Übungen (G-130)
        - **Produktionsaufträge** (G-131)
            - Lagerartikel im Produktionsauftrag (G-132)
            - Manuelle Erfassung durch Kopieren (G-133)
            - Einstellungen in der Lieferantenkartei (G-134)
            - Bestellmenge nach Bestandsprüfung (G-135)
            - Lagerzugang durch Produktionsauftrag (G-140)
    - **Inventur** (G-141)
        - **Periodische Inventur** (G-142)
            - Bestandaufnahme (G-143)
            - Inventurliste erstellen (G-145)
            - Sollbestand ermitteln (G-150)
            - Inventurwerte erfassen (G-152)
            - Inventur abschließen (G-154)
            - Nachtragsinventur anhängen (G-156)
            - Übungen (G-157)
        - **Erstinventur** (G-158)
            - Ablauf für die Erstinventur (G-159)
            - Erstinventur durchführen (G-160)
            - Übungen (G-162)
- **Softwarereferenz** (G-163)
    - **Übersicht** (G-165)
    - **Inventur** (G-166)
        - **Inventurliste** (G-167)
        - **Listendruck** (G-171)
        - **Sollbestand** (G-173)
    - **Inventurverwaltung** (G-175)
        - Menüs in der Inventurverwaltung (G-175)
            - Menü Optionen (G-175)
            - Menü Funktionen (G-176)
        - Verwaltung (G-176)
        - Gehe zu Artikel (G-179)
        - Wertberichtigung (G-179)
    - **Inventurabschluss** (G-180)
        - Menüs im Inventurabschluss (G-180)
            - Menü Optionen (G-180)
            - Menü Funktionen (G-180)
        - Abschluss (G-181)
        - Inventurliste wählen (G-183)
    - **Lagerverwaltung** (G-184)
        - Menüs in der Lageverwaltung (G-184)
            - Menü Funktionen (G-184)
            - Menü Optionen (G-185)
            - Menü Druck (G-185)
        - Lagerverwaltung (G-185)
            - Lagerverwaltung - Lagerartikel (G-186)
            - Lagerverwaltung – Preise (G-190)
            - Lagerverwaltung - Zusatz (G-193)
    - **Lagerbewegung** (G-195)
        - Menü Optionen (G-195)
        - Lagerbewegung (G-195)
            - Lagerbewegung - Abgang, Zugang (G-196)
            - Lagerbewegung - Umbuchung (G-198)
            - Lagerbewegung - Blattanzahl (G-199)
            - Lagerbewegung - Aufbruch (G-200)
        - Bemerkung (Lagerbewegung) (G-201)
    - **Abfragen** (G-202)
        - Buchungsjournal (G-202)
        - Lagerhistorie (G-204)
            - Lagerhistorie – Auswahl (G-205)
            - Lagerhistorie - Tabelle (G-208)
        - Lagerstatistik (G-209)
            - Lagerstatistik - Produkte (G-210)
            - Lagerstatistik - Statistik (G-212)
            - Lagerstatistik – FIFO/LIFO (G-214)
        - Reservierte Lagerartikel (G-215)
    - **Suche** (G-217)
        - Lagersuche - Lagersuche (G-217)
        - Lagersuche - Zukünftiger Lagerbestand (G-218)
    - **Lagerbestellung** (G-220)
        - Menüs im Bestellpool (G-220)
            - Menü Funktionen (G-220)
            - Menü Optionen (G-221)
        - Lagerbestellung (G-223)
    - **Lagerbewertung** (G-226)
        - Lagerbewertung (G-227)
            - Menü Optionen (G-227)
            - Lagerbewertung – Selektion (G-228)
            - Lagerbewertung - Bewertung (G-230)
- **Partindex** (G-233)
    - **Index Lagerwirtschaft** (G-235)

---

## Tutorial

### Übersicht
Das Tutorial zum Modul Lagerwirtschaft beschäftigt sich mit den Grundlagen der Lagerverwaltung in A+W Business. Das Tutorial baut auf den Kenntnissen zu den Stammdaten, zum Einkauf und zum Verkauf auf.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

#### Themenblöcke
In diesem Tutorial finden Sie folgende Themenblöcke:
- Grundgedanken zum Lager
- Stammdaten
- Lagerwirtschaft
- Lagerartikel in Dokumenten
- Inventur

#### Vorausgesetzte Kenntnisse
Das Tutorial richtet sich an Teilnehmer, die in A+W Business den Lagerbestand verwalten. Die Teilnehmer müssen das Konzept der Stammdaten, den Verkauf und den Einkauf in A+W Business kennen.

> **Kistenverwaltung im Lager**
> Die Einstellungen zum Kistenmanagement sind in dem separaten Part Kistenmanagement beschrieben.

### Dokumentation
Für das Modul Lagerwirtschaft stehen folgende Dokumente zur Verfügung:

| Format | Umfang |
| :--- | :--- |
| **Handout** | Ausdruck des Tutorials für die Schulung |
| **PDF** | Vollständige Unterlagen<ul><li>Tutorial</li><li>Softwarereferenz</li><li>Index</li></ul> |
| **Online-Hilfe `<F1>`** | Kontextsensitive Dialog-Hilfe der A+W Business-Softwarereferenz und Tutorials. |

### Aufbau des Tutorials
Das Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

- **Überblick**: Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
    - Lernziele: Was soll vermittelt werden?
    - Nutzen: Wofür können Sie dieses Wissen einsetzen?
    - Merksätze: Welche Zusammenhänge müssen Sie sich merken?
- **Konzepte**: Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.
- **Übungen**: Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen und Lösungsvorschlägen.
- **Querverweise**: Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf ergänzende Informationen in der Softwarereferenz und in anderen Parts hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.

#### Lesehinweis
Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.
Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

### Darstellungskonventionen
Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

| Konvention | Bedeutung |
| :--- | :--- |
| *Kursiv* | sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Lagerinfo*. |
| **Fett** | sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: Geben Sie den Wert **0** ein. |
| **>** | Mit dem sogenannten Brotkrumenpfad ist der Weg kennzeichnet, auf dem Sie einen Dialog öffnen, z. B. *Lagerwirtschaft > Inventur > Abschluss*. |
| **[ ]** | Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit **[OK]** speichern Sie die Daten. |
| **< >** | Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit **`<F1>`** öffnen Sie die Online-Hilfe. |

### Menü-Übersicht
In diesem Abschnitt finden Sie eine kurze Übersicht über die Programmbereiche, die in den Themenblöcken dieser Schulung angesprochen werden.

*(Abb. G-1 zeigt das Hauptfenster des Moduls Lagerwirtschaft, das in die Bereiche Inventur, Lagerverwaltung, Lagerbewegung, Abfragen, Suche, Lagerbestellung und Lagerbewertung unterteilt ist.)*

#### Inventur
In diesem Bereich bereiten Sie die Inventur vor, tragen die gezählten Werte ein und schließen die Inventur ab.
- "Inventur" auf Seite G-141
- Softwarereferenz, "Inventur" auf Seite G-166

#### Lagerverwaltung
In diesem Dialog erfassen und pflegen Sie die Daten für Lagerartikel.
- "Lagerverwaltung" auf Seite G-68
- Softwarereferenz, "Lagerverwaltung" auf Seite G-184

#### Lagerbewegung
In diesem Dialog buchen Sie Warenzugänge und Warenabgänge, Änderungen von Lagerorten und den Aufbruch von Kisten.
- "Lagerbuchung" auf Seite G-78
- Softwarereferenz, “Lagerbewegung" auf Seite G-195

#### Abfragen
In diesem Bereich lassen Sie sich die Lagerhistorie, Auswertungen und Reservierungen anzeigen.
- "Abfragen" auf Seite G-88
- Softwarereferenz, "Abfragen" auf Seite G-202

#### Suche
In diesem Dialog prüfen Sie die Verfügbarkeit von Produkten in einem bestimmten Zeitraum.
- "Lagerinformationen" auf Seite G-97
- Softwarereferenz, "Suche" auf Seite G-217

#### Lagerbestellung
In diesem Dialog übergeben Sie Bestellungen zu Lagerartikeln an den Einkauf.
- "Lagerbestellung an den Einkauf übergeben" auf Seite G-109
- Softwarereferenz, "Lagerbestellung" auf Seite G-220

#### Ergänzende Informationen
- Überblick, "Elemente des Programmfensters" auf Seite A-52
- Verkauf, "Dialog Dokumentenverwaltung" auf Seite C-40

### Grundgedanken zum Lager
Im Modul *Lagerwirtschaft* von A+W Business können Sie Bandmaße, Lagermaße, Restblätter, Kisten, Ganzglastüren, Beschläge, Rahmenteile und Zubehör wie Spiegelaufhängungen, Dichtungsbänder usw. verwalten.
Dabei ist es möglich, die Lagerorganisation Ihres Unternehmens im Programm abzubilden. Sie definieren Standorte, Gänge, Regale bis hin zu den einzelnen Fächern und legen fest, welche Stück-, Quadrat- oder Laufmeterartikel sich an welchem Lagerort befinden.

*(Abb. G-2 zeigt ein Flussdiagramm der Lagerwirtschaft. Ein Auftrag führt zu einem Lagerartikelbedarf. Dieser wird aus dem Lagerbestand gedeckt oder löst eine Reservierung/Disposition aus. Eine Unterdeckung führt zu einer Bestellung (Einkauf). Der Wareneingang vom Lieferant führt zu einer Zugangsbuchung im Lager. Der Lagerartikel wird für den Auftrag abgebucht, was zu Lieferschein und Rechnung führt. Alle Vorgänge können ausgewertet werden.)*

Alle kaufmännischen Vorgänge in A+W Business basieren auf den Stammdaten. Nur wenn diese korrekt gepflegt sind, kann die Verwaltung des Lagers problemlos abgewickelt werden. Zusammen mit dem Verkauf und dem Einkauf ergeben sich folgende Abläufe:

- **Auftrag:** In einem Auftrag fixieren Sie die Bestellung Ihres Kunden. Dabei erfassen Sie Positionen, die nach den Angaben des Kunden gefertigt werden müssen.
- **Übergabe Produktion:** An die Produktion werden die Auftragspositionen übergeben, die gefertigt werden müssen. Die benötigten Materialien werden reserviert und beim Druck von Lieferschein oder Rechnung ausgebucht. Gleichzeitig wird der verfügbare Lagerbestand aktualisiert.
- **Lagerbestellung:** Wenn der Mindestbestand von Lagerartikeln unterschritten wird, müssen diese Lagerartikel als Lagerbestellung erfasst werden.
- **Lagerzugang:** Mit der Erfassung des Wareneingangs wird der Lagerbestand der Lagerartikel aktualisiert. Artikel, die nicht als Lagerartikel geführt werden, können nicht als Lagerbestand geführt werden.
- **Inventur:** Mit der Inventur bereinigen Sie die Bestandszahlen in A+W Business.

#### Handlungsablauf bei der Lagerverwaltung
Üblicherweise pflegen Sie den Lagerbestand durch folgende Aktivitäten:
- Stammdaten einrichten
- Lagerartikel erfassen (Erstinventur)
- Warenein- und -ausgänge buchen (automatisch, manuell)
- Abfragen zu Umschlagshäufigkeit, Preisen, Beständen usw.
- Lagerbestellung erfassen, prüfen, senden
- Inventur durchführen:
    - Inventurliste erstellen, Nachtragsinventur anhängen
    - Sollbestand ermitteln
    - Zähllisten drucken
    - Gezählte Werte erfassen
    - Inventur abschließen

#### Wie soll das Lager geführt werden
Allen Produkten, die im Verkauf erfasst werden, wird ein Kennzeichen zugeordnet, das die Art der Beschaffung festlegt. Gläser, die im Lager geführt werden, haben neben dem Kennzeichen (Beschaffungsart) *Lagerentnahme* ein Kennzeichen (Lagerbuchungsart) für die Art, wie ihr Lagerbestand berechnet wird. Diese beiden Kennzeichen werden in der Themenblock Stammdaten beschrieben.

Bevor Sie Ihr Lager in A+W Business einrichten, müssen Sie entscheiden, auf welcher Basis die Bestände geführt werden sollen: als Fläche (qm) oder in Stückzahlen. Als dritte Möglichkeit steht die kombinierte Lagerführung zur Verfügung, wobei der maßabhängige Lagermodus mit den Rückmeldungen aus der Optimierung kombiniert wird, so dass neben den Lagermaßen auch die zugeschnittenen Bandmaße automatisch ausgebucht werden können.

Diese unterschiedlichen Möglichkeiten wirken sich folgendermaßen aus:

| Modus (Lagerkennzeichen) | Bedeutung, Beispiel | Nachteil |
| :--- | :--- | :--- |
| **qm = Fläche:** (nicht maßabhängig) | pro Glas wird die Fläche ermittelt: <ul><li>Float 4 => 10.500 qm</li><li>Float 5 => 11.070 qm</li><li>Float 6 => x qm</li></ul> | <ul><li>keine Info über die Anzahl der Lagermaße</li><li>keine Info darüber, wie viele Bandmaße verschnitten wurden</li></ul> |
| **Stück:** (maßabhängig) | pro Bandmaß und Lagermaß wird die Stückzahl ermittelt: <ul><li>Float 4: 3210/6000 (3 Stück), 800/1200 (3 Stück), x/x (n Stück)</li><li>Float 5: 3210/6000 (3 Stück), 800/1200 (3 Stück), x/x (n Stück)</li></ul> | <ul><li>keine Info über verschnittene Band- und Lagermaße</li><li>Bandmaße müssen manuell ausgebucht werden</li></ul> |
| **Stück inkl. Rückmeldungen:** (kombiniert) | Kombination aus maßabhängigen Lagermaßen und Rückmeldungen. Die verschnittenen Bandmaße und die Lagermaße werden automatisch ausgebucht. Bestand der Stückzahlen wird aktualisiert. | (Für diesen Modus müssen A+W Optimizer-Rückmeldungen möglich sein.) |

Nach der Entscheidung zum Modus ordnen Sie das entsprechende Lagerkennzeichen pro Glasprodukt zu und legen in den Firmendaten den Lagerführungsmodus fest. Diese Einstellungen sind in der Themenblock Stammdaten detailliert beschrieben.
- "Lagerführungsmodus und Reservierung" auf Seite G-30

### Stammdaten
In diesem Themenblock lernen Sie, wie Sie die Stammdaten für die Verwaltung des Lagers pflegen.
Dazu gehören folgende Lerneinheiten:
- "Lager" auf Seite G-20
- "Firmendaten" auf Seite G-29
- "Status" auf Seite G-34
- "Produktdefinition" auf Seite G-38
- "Preise" auf Seite G-51

#### Lager

**Lernziele**
- Lagerebenen benennen.
- Lagerort definieren.
- Lagerkategorien festlegen.

**Nutzen**
- Mit Lagerorten können Sie (gleiche) Materialien an unterschiedlichen Orten verwalten.
- Auswertungen können sich auf bestimmte Lagerorte oder Lagerartikel beziehen, die an unterschiedlichen Orten gelagert sind.

**Merke**

| Begriff | Beschreibung |
| :--- | :--- |
| **Ebenen** | Vier Differenzierungsebenen bezeichnen z. B. unterschiedliche Lagerhäuser, Gänge, Regale und Fächer. |
| **Lagerorte** | Die Kombinationen der verschiedenen Differenzierungsebenen bilden die Lagerorte. |
| **Lagerkategorien** | Mit Lagerkategorien können Sie die Suche und Auswertung auf bestimmte Produkte einschränken, die an unterschiedlichen Orten gelagert werden. |
| **Voreinstellungen** | Keine |

##### Lagerdefinition
Für die Darstellung Ihres Lagers legen Sie folgende Einstellungen fest:
- Namen der Lagerebenen
- Lagerebenen
- Lagerorte
Die Bezeichnung der einzelnen Ebenen können Sie an die Erfordernisse im Unternehmen anpassen. Diese Möglichkeit sollten Sie auch dann nutzen, wenn Sie nur mit einer Ebene arbeiten.

**Lagerort**
Zur Definition von Lagerorten können Sie bis zu vier Differenzierungsebenen festlegen und damit z. B. Lagerhäuser, Gänge, Regale und Fächer unterscheiden. Die Lagerorte werden in der Lagerverwaltung und bei der Inventur herangezogen.

*(Abb. G-3 zeigt eine hierarchische Lagerstruktur: Haus 1 -> Gang A/Gang B -> Regal 1/2/m/n -> Fach 1-6.)*

**Lagerebene**
Pro Ebene können Sie verschiedene Namen festlegen, z. B. auf der Ebene 1 die Lagerhäuser an unterschiedlichen Standorten, auf Ebene 2 die Gänge A bis F usw.

> **Mindestens einen Lagerort definieren**
> Sie müssen auch dann einen Lagerort definieren, wenn Sie Ihr Lager nicht weiter unterteilt haben. In diesem Fall legen Sie nur die Ebene 1 fest und definieren dann im Lagerort alle weiteren Ebenen als `<k.A.>`.

**Lagerkategorien**
Über Lagerkategorien haben Sie ein weiteres Suchkriterium für die Lagerverwaltung. Wenn Sie z. B. gleiches Material an verschiedenen Lagerorten verwalten, können Sie die Lagerkategorie dazu verwenden, das Material gemeinsam auszuwerten. Dazu sollten Sie alle Lagerorte definiert haben, an denen das Material tatsächlich vorgehalten wird.
Die definierten Lagerkategorien ordnen Sie im Dialog *Lagerverwaltung* den Produkten zu.

##### Lagerebenen festlegen
In dieser Einheit lernen Sie, wie Sie die Lagerebenen an die Erfordernisse in Ihrem Unternehmen anpassen.
Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
- "So legen Sie Ihre verschiedenen Lagerebenen fest" auf Seite G-22
- "So benennen Sie die Lagerebenen" auf Seite G-24

**So legen Sie Ihre verschiedenen Lagerebenen fest**
Die folgenden Schritte sind für alle Lagerebenen gleich. In diesem Beispiel wird eine Lagerebene 1 für Fertigprodukte angelegt.

1.  Wählen Sie im Menü *Stammdaten > Lager > Ebene 1*. Der Dialog *Ebene 1* wird geöffnet.
    - Stammdaten, "Ebene 1 bis 4" auf Seite B-736
2.  Wählen Sie im Menü *Start > Neu*, um in den Erfassungs-Modus zu wechseln.
    *(Abb. G-4 zeigt eine leere Zeile im Dialog "Ebene 1" zur Eingabe einer neuen Lagerebene.)*
3.  Geben Sie eine Bezeichnung für die Lagerebene ein, z. B. **Ortsnamen**, **Zuschnitt** usw.
4.  Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern. Die Daten werden gespeichert.
5.  Wiederholen die Schritte 1 bis 4 für alle Ebenen, die Sie in Ihrem Lager unterscheiden möchten. Öffnen Sie dazu auch die Dialoge zu den Lagerebenen 2 bis 4 und verfahren Sie auf die gleiche Weise.

**So benennen Sie die Lagerebenen**
1.  Wählen Sie im Menü *Stammdaten > Lager > Lagerdefinition*. Der Dialog *Lagerdefinition* wird geöffnet.
    - Stammdaten, "Lagerdefinition" auf Seite B-737
2.  Wählen Sie im Menü *Definition > Ebenen*.
    *(Abb. G-5 zeigt den Dialog "Lagerebenen", in dem die Namen für Ebene 1 bis 4 definiert werden, z.B. Stock, Corridor, Shelf, Tray.)*
3.  Legen Sie die Namen der Lagerebenen fest, z. B. **Lagerhaus** für die Ebene 1.
4.  Klicken Sie auf **[OK]**, um die Namen zu speichern. Der Dialog wird geschlossen. Die Änderungen werden in den Dialog *Lagerdefinition* übernommen.
5.  Schließen Sie den Dialog *Lagerdefinition* oder definieren Sie nun die Lagerorte.

##### Lagerort definieren
In dieser Einheit lernen Sie, wie Sie in A+W Business die Lagerorte einrichten.
Sie müssen auch dann einen Lagerort definieren, wenn Sie Ihr Lager nicht weiter unterteilt haben. In diesem Fall legen Sie nur die Ebene 1 fest und definieren dann für den Lagerort alle weiteren Ebenen als `<k.A.>`. Beachten Sie, dass auch ein Lagerort mit der Definition `<k.A.>` für alle Ebenen als Lagerort bebucht werden kann.

> **Tipp**
> Sie können bestimmte Materialien von einer Lagerhalle in den Produktionsbereich verlagern. Dazu werden die Lagerorte umgebucht. Für diesen Fall ist es sinnvoll, Lagerorte so präzise (kleinteilig) wie möglich zu definieren, z. B. bei den Fächern.

**So definieren Sie einen Lagerort**
1.  Wählen Sie im Menü *Stammdaten > Lager > Lagerdefinition*.
    *(Abb. G-6 zeigt den Dialog "Lagerdefinition", der aus zwei Hauptbereichen besteht: A) Auswahl der Bezeichnungen für die Ebenen (Stock, Corridor etc.) und B) eine Liste der bereits definierten Lagerorte.)*
    - Stammdaten, "Lagerdefinition" auf Seite B-737
    In diesem Modus können Sie die definierten Lagerorte (A) ändern, indem Sie die Bezeichnungen der Ebenen ändern. Wenn Sie den Erfassungsmodus gewählt haben, werden die Felder der Tabelle gesperrt.
2.  Wählen Sie im Menü *Start > Neu*, um in den Erfassungs-Modus zu wechseln.
    *(Abb. G-7 zeigt denselben Dialog im Erfassungsmodus. Die Felder zur Auswahl der Lagerebenen (A) und Parameter (B) sind aktiv, während die Tabelle darunter gesperrt ist.)*
3.  Wählen Sie auf jeder Ebene (A) einen Eintrag aus.
4.  Legen Sie ggf. einen der Parameter (B) fest, wenn der Lagerort besonders gekennzeichnet werden soll, z. B. als *Standardlager*. Wenn Sie als Lagerart den Eintrag *Hegla* ausgewählt haben, können Sie den Lagerort für den der Wareneingang der Hegla-Lieferungen festlegen.
5.  Wählen Sie im Menü *Start > Speichern*, um den Lagerort zu speichern. Die Daten werden gespeichert.
6.  Wiederholen Sie die Schritte 2 bis 5 für alle Lagerorte, die Sie zur Verwaltung Ihres Lagers benötigen.

##### Lagerkategorien festlegen
In dieser Einheit lernen Sie, wie Sie die Lagerkategorien festlegen, die Sie den Lagerartikeln zuordnen wollen.

**So legen Sie eine Lagerkategorie fest**
1.  Wählen Sie im Menü *Stammdaten > Lager > Kategorie*.
    *(Abb. G-8 zeigt den Dialog "Lagerkategorie" mit Einträgen wie Floatglas, Ornament, VSG/LG.)*
    - Stammdaten, "Lagerkategorien" auf Seite B-739
2.  Wählen Sie im Menü *Start > Neu*, um in den Erfassungs-Modus zu wechseln.
3.  Geben Sie für die Lagerkategorie eine ID ein, z. B. Ziffern oder Bezeichnungen wie **Rohmaterial**, **Produktion**.
4.  Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern. Die Daten werden gespeichert.

##### Übungen
- Benennen Sie alle vier Lagerebenen um.
- Legen Sie vier unterschiedliche Lagerorte an, von denen mindestens einer für Rohmaterial vorgesehen ist.

**Ergänzende Informationen im Part Stammdaten**
- Stammdaten, "Ebene 1 bis 4" auf Seite B-736
- Stammdaten, "Lagerdefinition" auf Seite B-737
- Stammdaten, "Lagerkategorien" auf Seite B-739

#### Firmendaten

**Lernziele**
- Einstellungen für die Reservierung (Lagerführungsmodus) kennenlernen.
- Einstellungen für die Ermittlung des Einkaufspreises kennenlernen.
- Zeitraum für die Lagervorschau festlegen.

**Nutzen**
- Reservierungen wirken sich auf den Lagerbestand aus. Der Bestand kann schon mit der Reservierung aktualisiert werden, so dass reservierte Mengen nicht mehr frei verfügbar sind.
- In der Lagervorschau werden der aktuelle Bestand und die reservierten Mengen für einen Zeitraum angezeigt, den Sie selbst festlegen.
- Der Einkaufspreis von Lagerartikeln kann automatisch aktualisiert werden. Dabei wird entweder der durchschnittliche EK berechnet oder der zuletzt erfasste.

**Merke**

| Begriff | Beschreibung |
| :--- | :--- |
| **Lagerführungsmodus** | Der Lagerführungsmodus in der Firmentabelle legt fest, wie Reservierungen den Lagerbestand beeinflussen. |
| **Lagerkennzeichen** | Das Lagerkennzeichen legt fest, ob die Bestände eines Lagerartikels als Fläche (qm) oder in Stückzahlen gewertet werden. |
| **Reservierung** | Zur Fertigung einer Auftragsposition werden die benötigten Mengen reserviert. Die Mengen werden in den Beständen gekennzeichnet oder ausgebucht. |
| **Voreinstellungen** | Keine |

##### Lagerführungsmodus und Reservierung
Wenn im Auftrag ein Produkt mit der Beschaffungsart *Lagerentnahme* erfasst wird, wird die entsprechende Menge (plus Verschnitt bei Festmaßen) des Lagerartikels als reserviert gekennzeichnet. Die Reservierung kann wahlweise manuell aus dem aktuellen Bestand ausgebucht werden oder automatisch, wenn der Lieferschein oder die Rechnung gedruckt wird.

- **Reservierung ohne Bestandsaktualisierung:** Die Menge wird als reserviert gekennzeichnet, vom Bestand jedoch noch nicht ausgebucht. Die Abbuchung muss manuell durchgeführt werden.
- **Reservierung mit Bestandsaktualisierung:** Die reservierte Menge wird mit dem Druck des Lieferscheins oder der Rechnung aus dem aktuellen Bestand ausgebucht. Dabei bestimmt die Statuszuordnung, welches Formular die Buchung anstößt.
- **Lagerabbuchung vor Formularausdruck durchführen:** Lagerartikel können abgebucht werden, bevor der Formulardruck ausgeführt wird. Falls bei der Lagerabbuchung ein Problem auftritt, wird der Auftrag nicht gedruckt.

Diese Einstellungen werden in der Anzeige von Bestandsmengen im Dialog *Lagerinfo* (Lagervorschau) und bei den automatischen Bestellvorschlägen sichtbar, die beim Erreichen von Mindestmengen angestoßen werden können.

##### Firmendaten prüfen
In dieser Einheit lernen Sie, wie Sie die Vorgaben zur Bewertung des Lagers und zum Lagerführungsmodus einstellen.

**So prüfen Sie die Einstellungen für das Lager**
1.  Wählen Sie im Menü *Stammdaten > Firma > Firmendaten*.
    - Stammdaten, "Firmendaten" auf Seite B-918
2.  Wechseln Sie zum Register *Parameter* und prüfen Sie die Einstellungen für die virtuellen Positionsnummern.
    *(Abb. G-9 zeigt das Register "Parameter" in den Firmendaten. Die Option "Virtuelle Positionsnummern verwenden" ist hervorgehoben.)*
    - **Virtuelle Positionsnummern für den Wareneingang von Kisten:** Die virtuelle Positionsnummer wird benötigt, damit der Wareneingang von Kistenpositionen mit einer Stückzahl > 1 korrekt verbucht werden kann. Der Wareneingang von Kisten ist im Part Kistenmanagement beschrieben. Auf das Kennzeichen wird daher in dieser Schulung nur hingewiesen.
3.  Wechseln Sie zum Register *Lager / EK / EDI*.
    *(Abb. G-10 zeigt das Register "Lager / EK / EDI" mit drei markierten Bereichen: A) Einstellungen zur Ermittlung des Einkaufspreises, B) Einstellung zur Aktualisierung des Lagerbestands (Lagerführungsmodus), C) Anzahl der Vorschautage für den Dialog Lagerinfo.)*
    Die Einstellungen zur Ermittlung des Einkaufspreises lernen Sie in der Einheit *Preise* kennen.
    - "Einkaufspreis und Durchschnitts-EK" auf Seite G-52
4.  Wählen Sie die Einstellungen für Lagerbestellungen (A) aus:
    - **Abstandhalter bei Sprossen mitbestellen:** Aktivieren Sie diese Checkbox, wenn in einer Stückliste die Abstandhalter zusammen mit den Sprossen bestellt werden sollen, deren Beschaffungsart auf *Bestellung* gesetzt ist.
    - **ISO als Bestellartikel (Bearb. können Eigenfertigung sein):** Aktivieren Sie diese Checkbox, wenn die ISO-Einheit ohne die Bearbeitungen bestellt werden soll. Die Bearbeitung wird dann in der eigenen Produktion durchgeführt.
    - **Pos. ohne Lagerkennz. im WE anzeigen bei Lagerbestellung:** Aktivieren Sie diese Checkbox, wenn in Lagerbestellungen Positionen ohne Lagerkennzeichen im Wareneingang in roter Schrift angezeigt werden sollen.
5.  Wählen Sie im Bereich *Lagerführungsmodus* (B) die Funktionen aus, die bei der Aktualisierung des Lagerbestands berücksichtigt werden sollen.
    - **Reservierung ohne Bestandsaktualisierung:** Aktivieren Sie diese Option, wenn reservierte Mengen nicht aus dem aktuellen Bestand ausgebucht werden sollen. Die Abbuchungen müssen Sie dann zum gegebenen Zeitpunkt manuell durchführen. Bei der Auftragserfassung wird der aktuelle Bestand daher nicht angezeigt.
    - **Reservierung mit Bestandsaktualisierung:** Diese Option ist standardmäßig aktiviert, damit reservierte Mengen mit dem Druck des Lieferscheins bzw. der Rechnung aus dem aktuellen Bestand ausgebucht werden.
    - **Lagerführung auf Stücklistenebene:** Aktivieren Sie diese Checkbox, wenn Produkte im Lager auch dann geführt werden sollen, wenn sie Bestandteile einer Stückliste sind.
    - **Lagerabbuchung vor Formularausdruck durchführen:** Aktivieren Sie diese Checkbox, wenn Lagerartikel abgebucht werden sollen, bevor der Formulardruck ausgeführt wird. Falls bei der Lagerabbuchung ein Problem auftritt, wird der Auftrag aus den zu druckenden Dokumenten entfernt, also nicht gedruckt.
6.  Tragen Sie die Anzahl der Werktage (C) ein. Die Anzahl der Werktage wird für die Vorschau im Dialog *Lagerinfo* ausgewertet. Sie gibt an, über welchen Zeitraum in die Zukunft die zukünftigen Lagerbestände angezeigt werden.
7.  Wählen Sie im Menü *Start > Speichern*, um Änderungen zu speichern. Die Daten werden gespeichert. Nach Änderungen der Firmendaten sollten Sie A+W Business neu starten.

> **Statuszuordnung für Lagerabbuchung**
> Wenn Sie die Option *Lagerabbuchung vor Formulardruck durchführen* aktiviert haben, sollten Sie die Statuszuordnung für die Lagerabbuchung prüfen. Die Mindest-, Vergabe- und Sperrstatus müssen so organisiert sein, dass die Lagerabbuchung vor dem Druck ausgeführt werden kann. Wenn die Statuszuordnung die Umkehrung der Reihenfolge nicht zulässt, wird unter Umständen die Lagerabbuchung nicht durchgeführt.
> Die Statuszuordnungen lernen Sie in der nächsten Einheit kennen.

#### Status

**Lernziele**
- Statusänderungen durch Warenzugang und Warenabgang kennenlernen.
- Relevante Statuspunkte und -zuordnungen prüfen.

**Nutzen**
- Mit der Statuszuordnung schaffen Sie die Voraussetzungen für die automatische Statusumsetzung in Dokumenten und für die Lagerbuchungen.

**Merke**

| Begriff | Beschreibung |
| :--- | :--- |
| **Status** | Der Status legt fest, wann die Bestandswerte aktualisiert werden. |
| **Voreinstellungen** | Keine |

##### Statusänderungen durch Zu- und Abgänge
Warenab- und Warenzugänge können den Status von Dokumenten verändern und mit der Statusveränderung zu Bestandsänderungen im Lager führen. Wenn die Statuspunkte und Statuszuordnungen entsprechend definiert sind, gilt dies auch für Teillieferungen.
Wenn Sie in den Firmendaten die Option *Lagerabbuchung vor Formulardruck durchführen* aktiviert haben, müssen der Mindest-, Vergabe- und Sperrstatus so organisiert sein, dass die Lagerabbuchung vor dem Druck ausgeführt werden kann. Wenn die Statuszuordnung die Umkehrung der Reihenfolge nicht zulässt, wird unter Umständen die Lagerabbuchung nicht durchgeführt.

##### Statuszuordnungen prüfen
In dieser Einheit lernen Sie, wie Sie die Statuszuordnung prüfen und ggf. ändern.
Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
- "So prüfen Sie die Statusverwaltung" auf Seite G-35
- "So prüfen Sie die Statuszuordnung" auf Seite G-36

**So prüfen Sie die Statusverwaltung**
1.  Wählen Sie im Menü *Stammdaten > Auftrag > Statusverwaltung*.
    *(Abb. G-11 zeigt eine Liste von Anwenderstatus. A) "Wareneingang gebucht" (Status für Lagereingang) und B) "Warenabgang gebucht" (Status für Lagerabgang) sind hervorgehoben.)*
    - Stammdaten, "Statusverwaltung" auf Seite B-885
2.  Prüfen Sie, ob der Anwenderstatus für den Lagereingang und für den Lagerabgang vorhanden ist. Legen Sie diese ggf. an.
3.  Wählen Sie dazu im Menü *Start > Neu*, um in den Erfassungs-Modus zu wechseln. Eine neue Zeile wird freigeschaltet.
4.  Geben Sie die Nummer und die Bezeichnung ein.
5.  Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern. Die Daten werden gespeichert.
6.  Wiederholen Sie die Schritte 3 bis 5, wenn Sie einen weiteren Anwenderstatus anlegen wollen.
7.  Prüfen Sie als Nächstes die Statuszuordnungen.

**So prüfen Sie die Statuszuordnung**
1.  Wählen Sie im Menü *Stammdaten > Auftrag > Statuszuordnung*.
    *(Abb. G-12 zeigt den Dialog "Statuszuordnung". Der Statuspunkt "072 - Warenabgang Lager" ist ausgewählt und seine Zuordnungen (Dokumententyp, Anwenderstatus, Mindeststatus, Sperrstatus) werden angezeigt.)*
    - Stammdaten, "Statuszuordnung" auf Seite B-887
2.  Prüfen Sie, ob die Statuszuordnungen von Lagereingang und Lagerabgang für die Dokumententypen *Auftrag* und *Bestellung* festgelegt sind:
    - **Warenabgang Lager:** Status *Lieferschein gedruckt* oder *Rechnung gedruckt*
    - **Wareneingang Lager:** Status *Wareneingang gebucht*
    
    Für Wareneingänge und Teilwareneingänge müssen folgende Zuordnungen festgelegt sein:
    - AB-Lieferant teilweise/Auftrag
    - AB-Lieferant komplett/Auftrag
    - Wareneingang teilweise/Auftrag
    - Wareneingang komplett/Auftrag
    - Wareneingang teilweise/Bestellung
    - Wareneingang komplett/Bestellung
    - AB-Lieferant teilweise/Bestellung
    - AB-Lieferant komplett/Bestellung
3.  Legen Sie die fehlenden Zuordnungen an und korrigieren Sie die vorhandenen ggf.
4.  Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern. Die Daten werden gespeichert.

#### Produktdefinition

**Lernziele**
- Unterschied zwischen Lagermaß und Lagerartikel kennenlernen.
- Zusammenspiel von Produkt, Lagerartikel und Lagermaß kennenlernen.
- Produkt und Lagerkennzeichen kennenlernen.
- Einstellungen im Hauptprodukt und in der Stückliste unterscheiden.

**Nutzen**
- Wenn Sie die Produkte korrekt anlegen, können die Berechnungen und die Reservierung von Stück und Flächen durchgeführt werden.
- Die jeweils aktuelle Anzeige des Bestands inklusive der Reservierungen erleichtert den Einkauf.

**Merke**

| Begriff | Beschreibung |
| :--- | :--- |
| **Produkte** | Die Produkte aus den Stammdaten dienen zur Erfassung und Preisfindung in Dokumenten. Sie werden nicht automatisch als Lagerbestand geführt, sondern nur aufgrund zusätzlicher Einstellungen und Definitionen. |
| **Lagerartikel** | Alle Produkte, die im Lager mit Bestandsmengen geführt werden, müssen auch als Lagerartikel angelegt sein. |
| **Bandmaß** | Platte, wie sie vom Hersteller geliefert wird. Aus ihr werden die Gläser für den Verkauf zugeschnitten. |
| **Lagerplatte** | Tatsächlich im Lager befindliches Glas mit bestimmtem Maß, z. B. Float 4 mm in 1200 x 1800 mm oder 3500 x 5100 mm. Lagerplatten mit definierten Maßen werden als auch Lagermaß bezeichnet. Lagerplatten können als Ganzes (1200 x 1800) verarbeitet werden. Aus ihnen können aber auch Gläser zugeschnitten werden, z. B. 600 x 900 aus der Platte 1200 x 1800 oder aus der Platte 3210 x 5100. |
| **Lagermaß (Festmaß)** | Die als Lagermaß festgelegten Gläser werden ohne Zuschnitt verkauft. Ihnen sind eigene Preistabellen (Lagermaßtabelle) zugeordnet. Ein maßabhängiger Lagerartikel ist immer auch ein Lagermaß. |
| **Lagerkennzeichen (Lagerbuchungsart)** | Das Lagerkennzeichen legt fest, ob die Bestände eines Lagerartikels als Fläche (qm) oder in Stückzahlen gewertet werden. |
| **Beschaffungsart** | Das Kennzeichen legt fest, wie ein Produkt standardmäßig beschafft wird, z. B. durch Zuschnitt, Lagerentnahme, Produktion, Bestellung. |
| **Voreinstellungen** | Keine |

##### Produkt
Produkte werden in den Auftragspositionen mit konkreten Maßen erfasst und von dort in die Produktion übergeben. In der Produktion werden die Gläser für die Auftragsposition aus Lagerplatten geschnitten oder aus dem Bestand der Lagermaße entnommen.
Für die Bestandspflege im Lager ist dabei wichtig, wie viel Material verbraucht wird. Dieser Verbrauch schließt den Verschnitt mit ein. Die errechnete Fläche oder Stückzahl wird nach der Auftragserfassung im Lager reserviert.

*(Abb. G-13 veranschaulicht die Beziehung zwischen Verkauf, Lagerbestand und Preis. Ein Verkaufsauftrag (z.B. Float 4, 400x600mm) kann entweder aus einem Zuschnitt einer Lagerplatte (Verbrauch=Fläche+Verschnitt) oder aus einem vordefinierten Lagermaß (Verbrauch=Stück) bedient werden. Entsprechend wird der Preis entweder als Festmaß pro qm oder als Lagermaß pro Stück berechnet.)*

##### Produkte als Lagerartikel
Alle Produkte, die im Lager mit Bestandsmengen geführt werden, müssen auch als Lagerartikel angelegt sein.
Die Bestände von Lagerartikeln können im Lager unterschiedlich geführt werden, nämlich unter Berücksichtigung der Maße oder der Stückzahlen. Mit dem Kennzeichen zur Lagerbuchungsart legen Sie eine dieser Möglichkeiten fest. Diese Zusammenhänge sind in den Grundgedanken zur Lagerverwaltung dargestellt:
- "Wie soll das Lager geführt werden" auf Seite G-17

**Beschaffungsart**
Jedem Produkt ist eine Beschaffungsart zugeordnet, z. B.:
- *Lagerentnahme* (für Lagerartikel)
- *Zuschnitt* (für Gläser, die zugeschnitten werden sollen)
- *Produktion* (für Scheiben, die zusammengesetzt werden, z. B. ISO, VSG)
- *Bestellung* (für Produkte, die nicht im Lager gehalten werden)
Bei der Erstinventur werden die Lagerartikel aufgrund der Beschaffungsart *Lagerentnahme* und des Lagerkennzeichens (qm oder Stück) automatisch erstellt.

**Lagerbuchungsart (Lagerkennzeichen)**
Jedem Produkt wird in den Stammdaten eine der folgenden Lagerbuchungsarten zugeordnet:
- **Maßabhängig:** pro Produkt mehrere Lagerartikel (Glas in verschiedenen Abmessungen), Lagerbuchungsart = *Stück*. Produkte mit diesem Kennzeichen werden als Stückartikel im Lager geführt. Dies sind in der Regel Gläser mit festen Maßen. Jedes Lagermaß ist dann ein eigener Stückartikel. Im Bestand wird die Gesamtfläche dieser Lagermaße nicht bewertet, sondern z. B. 6 Stück des Lagermaßes Float 4 in der Größe 600 x 800 mm.
- **Nicht maßabhängig:** pro Produkt ein Lagerartikel ohne Maße, Lagerbuchungsart = *qm*. Produkte mit diesem Kennzeichen werden im Lager in der Mengeneinheit des Produkts geführt, z. B. Scharniere, Griffe als Stückartikel, Gläser in Quadratmetern. Die Gesamtfläche eines Glases kann dann aus beliebig vielen Platten und Resten bestehen. Bandmaße müssen dann manuell ausgebucht werden.
- **Kombiniert:** Lagerbuchung = *Stück oder qm*. Produkte mit diesem Kennzeichen werden sowohl als qm- als auch als Stückartikel geführt. Diese Einstellung ist nur sinnvoll, wenn die Lagerführung Rückmeldungen von A+W Optimizer auswertet. Aus diesen Rückmeldungen wird ersichtlich, welche Bandmaße verschnitten wurden. Das Kennzeichen wird verwendet, um sowohl Bandmaße als auch Lagermaße im Lager automatisch zu führen.

**Lagerbuchungen bei kombinierter Lagerführung**
Der kombinierte Lagerführungsmodus erlaubt die Lagerführung für Zuschnitts- und für Festmaße sowohl auf Quadratmeter- als auch auf Stückbasis. Bei einer A+W Optimizer-Rückmeldung ist es dann möglich, Bandmaße, die verschnitten wurden, aus dem Lager automatisch auszubuchen (anstatt nur die qm-Menge).

Für die Reservierung wird ein qm-Lagerartikel mit Abmessung 0 x 0 mm genutzt, der als eine Art Zwischenspeicher dient:
- Die Menge wird auf dem qm-Artikel reserviert.
- Mit der Rückmeldung aus der Produktion wird diese Reservierung storniert.
- Die Menge wird auf das Bandmaß umgebucht.
- Mit dem Druck des Lieferscheins wird die Menge ausgebucht. Damit reduziert sich die Stückzahl der Bandmaße. Der verbleibende Rest wird in den qm-Bestand übernommen.

**Ausnahme:**
Wird der Lieferschein vor der A+W Optimizer-Rückmeldung gedruckt, so werden zunächst die entsprechenden Quadratmeter ausgebucht (Dummy-Buchung). Wenn danach die A+W Optimizer-Rückmeldung kommt, wird diese qm-Buchung korrigiert und die entsprechenden Bandmaße ausgebucht. Für die Dummy-Buchung muss in der Produktverwaltung im Register *Fertigung* ggf. eine abweichende Produktnummer im Feld *Schlüssel Optimierung* angegeben werden.

##### Lagermaße
Gläser mit festen Größen können als Lagermaße und/oder Kisten definiert werden. Neben den Lagermaßen müssen Sie auch Lagerartikel anlegen. Lagerartikel werden für die Bestandsführung herangezogen. Wenn Sie ein Lagermaß in den Stammdaten angelegt haben, bietet A+W Business die Möglichkeit, sofort in die Lagerverwaltung zu wechseln. Wie Sie den Lagerartikel anlegen, lernen Sie im Themenblock *Lagerwirtschaft*.

*(Abb. G-14 zeigt das Zusammenspiel zwischen der Produktverwaltung (Stammdaten) und der Lagerverwaltung. In der Produktverwaltung (A) werden für ein Produkt (B) verschiedene Lagermaße (C) definiert. Dies führt zur Erstellung von zugehörigen Lagerartikeln in der Lagerverwaltung (D), wo dann auch Preistabellen (E) und der EK (F) zugeordnet werden.)*

Jedem Lagermaß kann eine eigene Preistabelle zugeordnet werden. Wenn Sie mit dem Lagerkennzeichen maßabhängig arbeiten, müssen Sie für alle Lagermaße auch Lagerartikel angelegen.

> **Lagermaß Kiste im Dialog Lagermaße anlegen**
> Das Lagermaß *Kiste* ist für Lagerbuchungen zwingend erforderlich. Für die Erfassung einer Kiste als Auftrags- oder Bestellposition muss daher ein Lagerartikel/-maß *Kiste* angelegt sein. Eine ausführliche Beschreibung finden Sie im Part Kistenmanagement.

**Lagermaße vs. Lagerartikel**
Lagermaße legen Sie in den Stammdaten für alle Produkte an, die Sie in Ihrem Lager in festen Größen verwalten, z. B. für das Produkt Float 4 die Größen 600 x 800 mm, 1200 x 1800 mm, 2400 x 2800 mm usw. Diese Lagermaße dienen jedoch nicht zur Bestandsführung, sondern zur Preisgestaltung.

Allen Lagermaßen können Sie eine eigene Preistabelle zuordnen und so z. B. Preise mit und ohne Zuschnitt unterscheiden. In der Regel verwenden Sie für die Lagermaße auch die qm-Preise. Außerdem können Sie auch Lagermaße anlegen, die nur bestellt werden. Jedem Lagermaß kann eine eigene Warengruppe zugeordnet werden.

Die Lagermaße, die in den Stammdaten angelegt sind, müssen auch in der Lagerverwaltung anlegt sein, wenn sie auch als Lagerartikel (mit Bestand) geführt werden sollen. Dazu bietet A+W Business den schnellen Wechsel aus den Stammdaten in die Lagerwirtschaft.

| Stammdaten | Lagerverwaltung |
| :--- | :--- |
| **Produkt:** Float 4 mm | |
| **Lagermaß:** | **Lagerartikel:** |
| 600 x 800 mm | 600 x 800 mm |
| 1200 x 1800 mm | 1200 x 1800 mm |
| 2400 x 2800 mm | 2400 x 2800 mm |
*(Abb. G-15: Produkt, Lagermaß und Lagerartikel)*

**Sonderfall Lagerentnahme - nicht maßabhängig**
Die Lagermaßtabelle (Stammdaten) hat - bis auf einen Sonderfall - keine Verknüpfung zum Lager, sondern wird nur zur Abbildung der preislichen Abweichungen und für statistische Zwecke genutzt.

Der Sonderfall betrifft Lagerartikel mit dem Kennzeichen *nicht maßabhängig*, für die ein Lagermaß in der Lagermaßtabelle angelegt wurde.
Für diese nicht maßabhängigen Lagerartikel wird kein Verschnitt reserviert und es findet keine Übergabe an die Produktion statt, wenn in der Lagermaßtabelle der Produkte diese Abmessung vorhanden ist.

**Beispiel: Reservierung mit/ohne Verschnitt**

| Produkt | Lagerartikel |
| :--- | :--- |
| | **ohne Lagermaß in Lagermaßtabelle** | **mit Lagermaß in Lagermaßtabelle** |
| Float 4 mm | nicht maßabhängig 500 x 500 mm | nicht maßabhängig 500 x 500 mm |
| Verschnitt 10% | | |
| Auftragsmenge 500 x 500 mm | | |
| **Reservierte Menge** | **0,275 qm** | **0,25 qm** |

##### Produktstammdaten prüfen
Die Produkte aus den Stammdaten dienen in Dokumenten als Basis für die Erfassung von Positionen. In der Produktion werden die Gläser für die Auftragsposition aus Lagerplatten geschnitten oder aus dem Bestand der Lagermaße entnommen.
In dieser Einheit lernen Sie, wie Sie die Produktdaten so einrichten, dass die Lagerbestände und Preise korrekt berechnet werden.

**So prüfen Sie die Stammdaten eines Produkts**
1.  Wählen Sie im Menü *Stammdaten > Produkte > Artikel > Artikel*. Der Dialog *Produktverwaltung* wird geöffnet.
    - Stammdaten, "Produktverwaltung" auf Seite B-590
2.  Suchen Sie das Produkt, das Sie im Lager führen wollen, und prüfen Sie die Mengeneinheit.
    *(Abb. G-16 zeigt das Register "Produkt" der Produktverwaltung. Feld A, "Mengeneinheit", ist hervorgehoben.)*
    Die Mengeneinheit muss so gewählt sein, dass der Lagerbestand sinnvoll ermittelt werden kann, z. B. für Scharniere **Stück**, für Glas **qm**.
3.  Wechseln Sie zum Register *Preis/Zuschlag* und prüfen Sie die Einstellungen.
    *(Abb. G-17 zeigt das Register "Preis/Zuschlag". Hervorgehoben sind: A) Preistabelle VK/EK, B) Mittlerer Verschnitt, C) Checkboxen "Preisrelevant VK" und "Preisrelevant EK".)*
    - Sind die Preistabellen (A), der Verschnitt (B) und die Checkboxen *Preisrelevant* (C) für VK/EK richtig aktiviert.
    - Die Checkbox *Preisrelevant EK* muss markiert sein, damit der Einkaufspreis ermittelt werden kann.
4.  Wechseln Sie zum Register *Lager/Einkauf* und prüfen Sie die Einstellung.
    *(Abb. G-18 zeigt das Register "Lager/Einkauf". Hervorgehoben sind: A) Lagerbuchungsart, B) Verfügbarkeitsprüfung, C) Maximale Maße für die Bestellung der Lagerplatte.)*
    Für Lagerartikel können Sie folgende Lagerbuchungsarten (A) auswählen:
    - **Maßabhängig:** Wählen Sie diese Einstellung, wenn Lagermaße als Stückartikel geführt werden sollen. Die Einstellung ist nur für Glas sinnvoll. Die Mengeneinheit im Register *Produkt* setzen Sie trotzdem auf **qm**, damit die Fläche berechnet wird.
    - **Nicht maßabhängig:** Wählen Sie diese Einstellung, für alle Lagerartikel, die in ihrer eigentlichen Mengeneinheit geführt werden sollen, z. B. Stückartikel, Beschläge. Wählen Sie diese Einstellung auch für Gläser, die in **qm** geführt werden sollen.
    - **Kombiniert:** Wählen Sie diese Einstellung, wenn Sie mit Rückmeldungen von A+W Optimizer arbeiten. Die Einstellung ist nur für Glas sinnvoll. Beachten Sie, dass Sie dazu ein Dummy-Lagermaß in **qm** aber ohne Maße anlegen müssen.
5.  Legen Sie fest, ob für die Verfügbarkeit (B) des Produkts geprüft werden soll. Wenn der Lagerartikel nicht in der Lagervorschau berücksichtigt werden muss, ist eine Verfügbarkeitsprüfung nicht erforderlich.
6.  Wenn im aktuellen Produkt Stücklisten-Komponenten enthalten sind, wechseln Sie zum Register *Stückliste*.

> **Lagerführung auf Stücklistenebene**
> Wenn Sie in den Firmendaten die Option *Lagerführung auf Stücklistenebene* gewählt haben, müssen Sie die Beschaffungsart für die entsprechenden Stücklisten-Komponenten setzen.
> Diese Form der Lagerführung lernen Sie in der Einheit *Lagerführung auf Stücklistenebene* kennen.

7.  Markieren Sie die jeweilige Stücklisten-Komponente und wählen Sie die Beschaffungsart (A) aus, wenn diese von der Definition in den Stammdaten der Komponente abweichen soll.
    *(Abb. G-19 zeigt das Register "Stücklisten-Komponenten". Hervorgehoben sind A) das Feld "Beschaffungsart" und B) die Checkbox "Preisrelevant EK".)*
    Wenn die Beschaffungsart für das Hauptprodukt auf *Produktion* gesetzt ist, können die Stücklisten-Komponenten gleichzeitig als Lagerartikel geführt werden. Wenn Sie einen solches Hauptprodukt im Auftrag erfassen, werden in der Lagerinfo alle Stücklisten-Komponenten auf *reserviert* gesetzt.
8.  Wählen Sie im Menü *Start > Speichern*, um die Änderungen zu speichern. Die Daten werden gespeichert.

##### Lagermaß anlegen
In dieser Einheit lernen Sie, wie Sie die Lagermaße zu den Produkten anlegen, um die Preisberechnung differenzieren zu können.

**So legen Sie Lagermaße in den Stammdaten an**
1.  Wählen Sie im Menü *Stammdaten > Produkt > Artikel > Lagermaße*. Der Dialog *Lagermaße* wird geöffnet.
    - Stammdaten, "Lagermaße" auf Seite B-637
2.  Wählen Sie im Menü *Start > Neu* und legen Sie das Lagermaß an.
    *(Abb. G-20 zeigt den Dialog zum Anlegen von Lagermaßen. Hervorgehoben sind: A) Maße der Platte, B) Preistabellen für VK/EK, C) Checkbox für Preisermittlung im Lager.)*
    Falls Sie in der Lagerverwaltung bereits einen entsprechenden Lagerartikel definiert haben sollten, tragen Sie die gleichen Werte für Breite und Höhe (A) ein.
3.  Sie können zusätzlich folgende abweichende Angaben einstellen:
    - Preisschlüssel für den Verkauf und den Einkauf (B).
    - Bezeichnung und Kurzbezeichnung (Matchcode), um z. B. den Lagerartikel besser identifizieren zu können.
    - Beschaffungsart, z. B. bei Lagerartikeln *Lagerentnahme*.
4.  Markieren Sie die Checkbox *EK Suche Lager* (C), wenn das Lagermaß in die Preisermittlung einbezogen werden soll. In der Einheit *Preise* lernen Sie, welche Einstellungen für die unterschiedlichen Formen der Berechnung notwendig sind.
    - "Einkaufspreis und Durchschnitts-EK" auf Seite G-52
5.  Wählen Sie im Menü *Start > Speichern*, um die Daten zu speichern. Die Daten werden gespeichert. Anschließend wird die Abfrage angezeigt, ob Sie dieses Lagermaß auch als Lagerartikel anlegen möchten.
6.  Wählen Sie **[Ja]**, wenn das Lagermaß auch als Lagerartikel verwaltet werden soll. Der Dialog *Lagerverwaltung* wird geöffnet. Die Handlungsschritte zum Anlegen eines Lagerartikels sind in einer separaten Einheit beschrieben.
    - "Lagerartikel anlegen" auf Seite G-74

##### Übungen
- Legen Sie zu einigen Ihrer Produkte Lagermaße an.
- Achten Sie darauf, dass diese Lagermaße auch als Lagerartikel angelegt sind.

**Ergänzende Informationen**
- "Lagermaße" auf Seite G-42
- "Lagerführungsmodus und Reservierung" auf Seite G-30
- Stammdaten, "Produkt anlegen" auf Seite B-182
- Stammdaten, "Produktverwaltung" auf Seite B-590
- Stammdaten, "Lagermaße" auf Seite B-637
- Stammdaten, "Firmendaten - Lager/EK/EDI" auf Seite B-957

