---
title: "D-AWProduction-HB_1"
source: "D-AWProduction-HB_1.pdf"
tags: ["A+W Production", "Software Manual", "Glass Manufacturing", "Window Production", "Door Production", "ERP", "PPS", "Production Planning", "Capacity Planning", "Barcode Manager"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a comprehensive handbook for the A+W Production software, a production planning and control system designed for the glass, windows, and doors industry. It provides an overview of the software's modules, functionalities, and user conventions."
long_description: "The A+W Production Handbook is a detailed user manual for the comprehensive production planning and control software developed by A+W. The software is tailored for manufacturers in the glass, windows, and doors sectors. This handbook serves as a complete guide for end-users, covering the full scope of the A+W Production suite. The document is structured into several parts, each designated by a letter (A, C, D, E, etc.), which correspond to different modules and functionalities of the software. Key topics include an general overview (Überblick), rough planning (Grobplanung), fine planning (Feinplanung), capacity planning (Kapazitätsplanung), a formula editor (Formeleditor), machine assignment (Maschinenzuordnung), barcode management (Barcode Manager), optimization systems (Packmitteloptimierung, Realtime Optimizer), and production terminals (Production Terminal). The manual begins with a preface containing revision history, copyright information, and contact details. It then provides a highly detailed table of contents. Each major section includes tutorials, software reference guides, and explanations of system conventions. The document is intended to help users understand the system architecture, from basic modules to advanced add-ons, and effectively utilize the software for planning, controlling, and monitoring their entire production process."
---

# A+W Handbuch

**Deutsch**

---
## A+W Production

**A+W - Software for Glass, Windows and Doors**

---

## Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Gesamt-Handbuch Version / Datum | Beschreibung |
| :--- | :--- |
| 4.00/06-2023 | Vollständige Überarbeitung |
| 3.00/03-2016 | Optimierung vollständig überarbeitet. |
| 2.00/08-2013 | Dokumentation an CI 2013 angepasst. Überarbeitung der Parts Grobplanung, MZO, Kapazitätsplanung |
| 1.00/01-2002 | Ersterstellung |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
*   Anmerkungen zu diesem Dokument
*   Urheberrechte
*   Warenzeichen
*   Kontakt

#### Anmerkungen zu diesem Dokument

Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Production gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Dieses Dokument beschreibt die volle Ausbaustufe von A+W Production.

#### Urheberrechte

© 2023, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß des Lizenzvertrages ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung von A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

#### Warenzeichen

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

#### Kontakt

**A+W Software GmbH**
Siemensstr. 3
D-35463 Fernwald
Germany
*   +49 641 96620 0
*   info@a-w.com
*   http://www.a-w.com

---

## Inhalt

*   **Vorspann**
    *   Revisionsübersicht
    *   Editorial
*   **Überblick (A)**
    *   Revisionsübersicht
    *   Editorial
    *   Tutorial
        *   Überblick
        *   Dokumentation
        *   Aufbau des Tutorials
        *   Darstellungskonventionen
        *   Produktportfolio der A+W Software GmbH
        *   A+W Production stellt sich vor
    *   Basismodul A+W Production
        *   Einlastung
        *   Einlastung allgemein
        *   Grobplanung
        *   Grobplanung allgemein
        *   Läufe bilden
        *   Feinplanung
        *   Feinplanung allgemein
        *   Ablauf der Feinplanung
        *   Gruppierungen und Sortierungen
        *   Abstellplatz- und Stapellogik
        *   Optimierungs-Modi
        *   Organisationsformen
        *   Orga-Typ und Los-Typ
        *   Maschinenzuordnung
        *   Bestandteile der Maschinenzuordnung
        *   Maschinen in der Maschinenzuordnung
        *   Arbeitsgänge in der Maschinenzuordnung
        *   Arbeitsgangzuordnung
        *   Bearbeitungstypen in der Maschinenzuordnung
        *   Bearbeitungsartikel in der Maschinenzuordnung
    *   A+W Production Ausbaumodule
        *   Kapazitätsplanung
        *   A+W Capacity Planner
        *   Optimierungssysteme
        *   Realtime Optimizer
        *   Sequence Optimizer
        *   Shape Optimizer
        *   Rack Optimizer
        *   DynOpt
        *   Furnace Optimizer
        *   Barcode Manager
        *   Allgemein
        *   Scanner
        *   Anzeige- und Leitrechnersysteme
        *   Production Terminal
        *   Statistiksysteme
        *   A+W Discovery
        *   Production Cockpit
    *   Konventionen
        *   Bedienoberfläche
        *   Dialoge
        *   Schaltflächen
        *   Dokumentation
        *   Aufbau des Handbuchs
        *   Online-Hilfe
        *   Hilfethemen
        *   Register Inhalt
        *   Register Index
        *   Register Suchen
        *   Hilfetext nicht gefunden
*   **Grobplanung (C)**
    *   Revisionsübersicht
    *   Editorial
    *   Tutorial
    *   Überblick
    *   Dokumentation
        *   Aufbau des Tutorials
        *   Darstellungskonventionen
    *   Grobplanung
        *   Prozess der Arbeitsvorbereitung
        *   Ansichten
        *   Ansichten in der Grobplanung
        *   Konfigurieren von und arbeiten mit Ansichten
        *   Übungen: Konfigurieren von und arbeiten mit Ansichten
    *   Aufträge / Pool
        *   Aufträge in der Grobplanung
        *   Töpfe
        *   Töpfe in der Grobplanung
        *   Läufe und Laufstrategien
        *   Läufe in der Grobplanung
        *   Positionen
        *   Positionen in der Grobplanung
        *   Vorgang suchen
    *   Softwarereferenz
        *   Grobplanung
        *   Aufträge in der Grobplanung
        *   Aufträge
        *   Auftragsübersicht
        *   Füllaufträge
        *   Übermengen-Editor
        *   Änderung der Beschaffungsart
        *   Töpfe in der Grobplanung
        *   Töpfe
        *   Reservierungsaufträge-Topf
        *   Bestellteile-Topf
        *   Topf-Bildung
        *   Topfbezeichnung ändern
        *   Läufe in der Grobplanung
        *   Läufe
        *   Lauf-Bildung
        *   Sonderglas-Lauf bilden
        *   Laufbezeichnung ändern
        *   Freigabe Lauf (Name): AUW – Wiederholung
        *   Positionen in der Grobplanung
        *   Positionen
        *   Auftrag zu Positionen hinzufügen
        *   Positionssplit
        *   Felddefinition
        *   Export/Import Positionsansicht
        *   Bearbeitungen in der Grobplanung
        *   Bearbeitungen
        *   Vorgabezeiten ändern
        *   Glasarten, Details, BDE und Lose
        *   Glasarten
        *   Details
        *   BDE
        *   Lose
        *   Übergreifende Dialoge
        *   Arbeitsplan
        *   Eigenschaften von (Register)
        *   Spaltendefinition
        *   (Filter Name)
        *   Filter-Definition
        *   Dokumentenverknüpfungen
        *   Entschichtungsflächen
        *   Übergreifende Kontextmenüs
*   **Feinplanung (D)**
    *   Revisionsübersicht
    *   Editorial
    *   Tutorial
        *   Dokumentations-Hinweise
        *   Wichtige Hinweise
        *   Dokumentation
    *   Überblick Feinplanung
        *   Ablauf der A+W Production
        *   Begriffe der A+W Production
    *   Gruppierungen und Sortierungen
        *   Überblick
        *   Einführung
        *   Gruppierung
        *   Sortierung
        *   Zusatz-Sortierung
        *   Sonderteile
        *   Demos und Übungen
    *   Abstellplätze und -modi
        *   Überblick
        *   Abstellplätze
        *   Logische Abstellplätze
        *   Abstellregeln
        *   Vordefinierte Abstellmodi für A-Böcke
        *   Robot-Böcke
        *   Abstellmodi für Fächerwagen
        *   Abstellmodi für feste Abstellplätze
        *   Standard-Einstellungen in der Konfiguration
        *   Einstellungen in den Stammdaten
        *   Demos und Übungen
    *   Optimierungsmodi
        *   Überblick
        *   Unterschiedliche Optimierungs-Modi
        *   Demos und Übungen
    *   Orgas
        *   Organisationsformen
        *   Allgemein
        *   Baumstruktur
        *   Master-Orga
        *   Bruch-Orga
        *   Prüfreihenfolge
        *   Orga-Typ und Los-Typ
        *   Globale Einstellungen
        *   Demos und Übungen
    *   Produktionsreihenfolge
        *   Allgemein
        *   Gruppierungsschlüssel der Orga-Gruppen
        *   A+W Standard-Orgas
        *   Abstellplatzorganisation
        *   Demos und Übungen
    *   Softwarereferenz
        *   Übersicht
        *   Organisationen
        *   Register Master-Orga
        *   Register Produktionsreihenfolge
        *   Register Prüfreihenfolge
        *   Master-Orga
        *   Orga
        *   Orga-Gruppen
        *   Einstellungen-Abstellplatz
        *   Voreinstellungen
        *   Gruppierung und Sortierung
        *   Gruppierung/Sortierung - Dialog
        *   Register Editor-Gruppierungen
        *   Register Editor-Sortierung
        *   Register Zusatz-Sortierungen
        *   Erzeugung einer Zusatz-Sortierung
        *   Abstellplätze
        *   Abstellplätze
        *   Lose
        *   Lostypen und Bearbeitungen
        *   Register Lostypen
        *   Register Bearbeitungen
        *   Register Abhängige Bearbeitungen
        *   Läufe feinplanen
        *   Feinplanung für Lauf
        *   Register Glasarten
        *   Register Bockbelegung
        *   Register Ergebnisse
        *   Register Spezial
        *   Register Freie Optimierung
        *   Register Teilmengen
        *   Register Orga
        *   Register Orga-Optionen
        *   Register Optionen
        *   Register Auswahl Lagermaß
        *   Ändern der minimalen Anzahl A-Böcke
        *   Reihenfolge der Maschinen
*   **Kapazitaetsplanung (E)**
    *   Revisionsübersicht
    *   Editorial
    *   Tutorial
    *   Überblick
        *   Dokumentation
    *   Grundlagen
        *   Terminoptimierung
        *   Terminfindung
    *   Planung und Einlastung
        *   Produktionsmonitor
        *   Tagesaktuelle Anpassungen der Arbeitsschichten
        *   Produktionsmonitor einrichten
        *   Arbeitsplan exportieren
    *   Einlastung und Umlastung
        *   Aufträge einlasten
        *   Umlastungen
        *   Bearbeitungen umlasten
        *   Fehlerhafte Einlastung
        *   Eingelastete Aufträge nachbearbeiten
    *   Kampagnenplanung
        *   Definition der Kampagnen
        *   Kampagnen in der Terminfindung
        *   Kampagnen anlegen und verwalten
        *   Übungen zu Kampagnen
    *   Reservierungen
        *   Reservierung von Kapazitäten
        *   Reservierungen anlegen und verwalten
        *   Übungen zu Reservierungen
    *   Bearbeitungserzeugung
        *   Bearbeitungserzeugung für die Einlastung
        *   Bearbeitungen erzeugen
    *   Stammdaten der Kapazitätsplanung
    *   Schichten
        *   Schichtpläne
        *   Arbeitsfreie Tage anlegen
        *   Schichtplan erstellen
        *   Schichtregel erstellen
        *   Schichtgruppe erstellen
        *   Übungen
    *   Kostenkalkulation
        *   Definition der Kostenkalkulation
        *   Kosten anlegen und verwalten
        *   Übungen
    *   Übergangszeiten
        *   Übergangszeiten in Schichten oder Stunden
        *   Definition von Übergangszeiten
        *   Übergangszeiten anlegen und verwalten
        *   Übungen
    *   Vorgabezeiten
        *   Definition der Vorgabezeiten
        *   Struktur von Vorgabezeitformeln
        *   Berechnung von Zeitzuschlägen
        *   Editor für Formelelemente
        *   Beispiel - Vorgabezeit für die logische Maschine Zuschnitt
        *   Zeitformel-Objekte
        *   Vorgabezeitformeln anlegen und verwalten
        *   Zeitformel testen
        *   Übungen
    *   Maschinengruppen
        *   Definition der Maschinengruppen
        *   Maschinengruppen anlegen und verwalten
        *   Übungen
    *   Lastverteilung
        *   Definition der Lastverteilung
        *   Lastverteilung einrichten und bearbeiten
        *   Übungen
    *   Softwarereferenz
        *   Überblick
        *   Einlastung
        *   Produktionsmonitor
        *   Angezeigte Maschinen
        *   Einstellungen
        *   Bitte wählen Sie einen Auftrag / Lauf aus (Filtern)
        *   Filter - Aufträge
        *   Filter - Läufe
        *   Filter - Eigene Filter
        *   Neuen Filter erstellen
        *   Maschine (Name)
        *   Schichten für Maschine anpassen
        *   Schichteigenschaften
        *   Reservierungsanzeige
        *   Arbeitsplan aus Produktionsmonitor
        *   Arbeitsplan - Details
        *   Arbeitsplan - Übersicht
        *   Einlastung
        *   Stücklistenkonfiguration
        *   Aktion
        *   Umlastung
        *   Maschinenumlastung
        *   Nachbearbeitung Einlastung
        *   Fehlerhafte Aufträge
        *   Asynchrone Verarbeitung
        *   Änderung bereits verplanter Aufträge
        *   Positionssplit
        *   Kampagnen und Reservierungen
        *   Kampagnen
        *   Kampagnen - Einzeltermine
        *   Kampagnen - Wöchentliche Termine
        *   Abgelaufene Reservierungen
        *   Reservierungen
        *   Reservierung für Maschine
        *   Kunde auswählen
        *   Objekt auswählen
        *   Bearbeitungen
        *   Bearbeitungserzeugung
        *   Existierende Bedingung hinzufügen
        *   Stammdaten für Zeiten
        *   Vorgabezeiten
        *   Vorgabezeitformel
        *   Elemente hinzufügen
        *   Tabelle, Vektor (Name)
        *   Eingabehilfe für Vektoren
        *   Formel auswählen
        *   Erfassung eines Formelelements
        *   Benutzerdefinierte Tabellenelemente
        *   Grenzwert auswählen
        *   Zeitformeltest
        *   Eigenschaften des Formelobjekts
        *   Formel (Name)
        *   Verlauf der Formelauswertung
        *   Übergangszeiten
        *   Stammdaten der Schichten
        *   Schichten
        *   Schichtkalender
        *   Schichtplan
        *   Schichtregel
        *   Schichtgruppe
        *   Maschine
        *   Maschinen und Kosten
        *   Kostenkalkulation
        *   Maschinengruppen
        *   Lastverteilung
*   **Formeleditor (F)**
    *   Revisionsübersicht
    *   Editorial
    *   Tutorial
    *   Der Formeleditor
        *   Ziele des Formeleditors
        *   Elemente des Formeleditors: Stufe I
        *   Elemente des Formeleditors: Stufe II
        *   Elemente des Formeleditors: Stufe III
    *   Notation Formula.dll
        *   Syntax
        *   Ergebnisprüfung
        *   Bedingungen für Abstellplätze
        *   Bedingungen für Orga-Gruppen
        *   Modus für Gruppenbildung
        *   Bedingungen für Fertigungsabschnitte
        *   Weitere Beispiele
        *   Übersicht der betroffenen Dialoge
    *   Softwarereferenz
        *   Formel-Editor
        *   Auswahl Bedingungen
        *   Bedingungen - Erzeuger
        *   Bedingung
        *   Name der Bedingung
        *   Info
        *   Invertieren
        *   Übergebene Menge
        *   Eingabe Zahlenwert
        *   Auswahl Mengen
        *   Mengen - Erzeuger
        *   Name der Menge
        *   Info
        *   Auswahl Formeln
        *   Formel - Editor
        *   Auswahl Zuweisung
        *   Zuweisung - Editor
*   **Maschinenzuordnung (G)**
    *   Revisionsübersicht
    *   Editorial
    *   Tutorial
    *   Überblick
    *   Grundlagen
    *   Maschinenzuordnung
        *   Maschinen
        *   Maschinen in der Maschinenzuordnung
        *   Maschinen anlegen und verwalten
        *   Restriktionen von Maschinen anlegen und bearbeiten
        *   Übungen zu Maschinen
    *   Logische Maschinen
        *   Logische Maschinen in der Maschinenzuordnung
        *   Logische Maschinen anlegen und verwalten
        *   Übungen zu logischen Maschinen
    *   Arbeitsgänge
        *   Arbeitsgänge in der Maschinenzuordnung
        *   Arbeitsgänge anlegen und verwalten
        *   Übungen zu Arbeitsgängen
    *   Arbeitsgangzuordnung
        *   Angepasste Arbeitsgangzuordnung
        *   Arbeitsgänge und logische Maschinen zuordnen
        *   Übungen zur Arbeitsgangzuordnung
    *   Bedingungen, Formeln, Restriktionen
        *   Bedingungen und Formeln in der Maschinenzuordnung
    *   Bearbeitungstypen und Bearbeitungsartikel
        *   Bearbeitungstypen in der Maschinenzuordnung
        *   Bearbeitungsartikel in der Maschinenzuordnung
    *   Softwarereferenz
        *   Maschinenzuordnung
        *   MZO-Editor
        *   Spaltendefinition
*   **Barcode Manager (H)**
    *   Vorspann
    *   Tutorial
    *   Grundgedanken
    *   Buchungselemente
    *   Buchungsorte
    *   Datenerfassung
    *   Buchungsbeispiele
    *   Production Terminals
    *   Bruchmanagement
    *   Statistik, Reporting und Monitoring
    *   Statistik: A+W Discovery
    *   Softwarereferenz
*   **Packmitteloptimierung (I)**
    *   Revisionsübersicht
    *   Editorial
    *   Tutorial
    *   Grundgedanke
    *   Allgemeines
    *   Stammdaten
    *   Anzeigen
    *   Optimierung ansehen
    *   Softwarereferenz
*   **A+W Realtime Optimizer (J)**
    *   Revisionsübersicht
    *   Editorial
    *   Tutorial
    *   Grundgedanken
    *   Arbeiten mit A+W Realtime Optimizer
    *   Optimierung
    *   Zuschnitt
    *   Zusammenarbeit mit anderen Modulen
    *   Softwarereferenz
*   **A+W Production Terminal (L)**
    *   Revisionsübersicht
    *   Editorial
    *   Tutorial
    *   Überblick
    *   Dokumentation
    *   Production Terminal Systeme
    *   Überblick A+W Production Terminal IG
    *   Überblick A+W Production Terminal Manual Cutting
    *   Überblick A+W Production Terminal Georgian Bars
    *   Überblick A+W Production Terminal Order
    *   Überblick A+W Production Terminal Processing
    *   Überblick A+W Production Terminal TG
    *   Überblick A+W Production Terminal LG
    *   Überblick A+W Production Terminal Edit
    *   Softwarereferenz
*   **A+W Production Index (Z)**

---

# A. Überblick

## Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version / Datum | Beschreibung |
| :--- | :--- |
| 2.03/02-2017 | Screenshots aktualisiert. |
| 2.02/01-2017 | Produkt- und Firmennamen angepasst. |
| 2.01/08-2013 | Vollständige Überarbeitung der ALCIM-Dokumentation und Anpassung auf A+W Production |
| 2.00/11-2012 | Überarbeitungen |
| 1.00/03-2003 | Ersterstellung |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
*   Anmerkungen zu diesem Dokument
*   Urheberrechte
*   Warenzeichen

#### Anmerkungen zu diesem Dokument

Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Production gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.

Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von A+W Production.

#### Urheberrechte

© 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

#### Warenzeichen

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

## Inhalt des Überblicks

*   Revisionsübersicht
*   Editorial
*   **Tutorial (A-7)**
    *   Überblick
    *   Dokumentation
        *   Aufbau des Tutorials
        *   Darstellungskonventionen
    *   Produktportfolio der A+W Software GmbH
    *   A+W Production stellt sich vor
    *   Basismodul A+W Production
        *   Einlastung
        *   Grobplanung
        *   Feinplanung
        *   Maschinenzuordnung
    *   A+W Production Ausbaumodule
        *   Kapazitätsplanung
        *   A+W Capacity Planner
        *   Optimierungssysteme
        *   Barcode Manager
        *   Anzeige- und Leitrechnersysteme
        *   Statistiksysteme
*   **Konventionen (A-75)**
    *   Bedienoberfläche
    *   Dokumentation
*   **Partindex (A-87)**
    *   Index

## Tutorial

### Überblick

Die Zielgruppe der Schulung zum Produkt A+W Production sind ISO-, ESG- oder VSG-Produzenten sowie Bearbeitungs- und Veredelungsunternehmen welche sich einen Überblick über die Leistungen und die Prozesse in und mit A+W Production verschaffen wollen.

Ziel dieses Systemüberblickes ist es, Ihnen einen grundlegenden Überblick über die Leistungen und Möglichkeiten von A+W Production zu geben. Alle hier beschriebenen Inhalte und Module werden in separaten Schulungen und Tutorials tiefer und ausführlicher behandelt.

Ein gutes Verständnis für die Systemarchitektur und den modularen Aufbau von A+W Production sind die Grundvoraussetzung für die Handhabung und Bedienung der einzelnen Bereiche und den hierfür notwendigen Wissenserwerb.

#### Themenblöcke

In diesem Tutorial finden Sie folgende Themenblöcke:
*   A+W Production stellt sich vor
*   Basismodul A+W Production
*   A+W Production Ausbaumodule

> **Vorausgesetzte Kenntnisse**
> EDV-Grundkenntnisse bzw. Windows-Kenntnisse werden bei den Anwendung von A+W Production vorausgesetzt.

### Dokumentation

Für die Schulung zu A+W Production - Einführung stehen folgende Unterlagen zur Verfügung:

| Format | Inhalt |
| :--- | :--- |
| HTML | Tutorial und Softwarereferenz |
| Handout | Ausdruck Schulungsunterlage für die Teilnehmer |
| PDF | Vollständige Unterlagen, Tutorial, Softwarereferenz |
| Online-Hilfe <F1> | Kontextsensitive Dialog-Hilfe der A+W Production-Softwarereferenz |

#### Aufbau des Tutorials

Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

*   **Überblick**: Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
    *   Lernziele: Was soll vermittelt werden?
    *   Nutzen: Wofür können Sie dieses Wissen einsetzen?
    *   Merksätze: Welche Zusammenhänge müssen Sie sich merken?
*   **Konzepte**: Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.
*   **Übungen**:
    *   Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen und Lösungsvorschlägen.
    *   Die Übungen helfen Ihnen A+W Production zu verstehen und anwenden zu lernen.
*   **Querverweisteil**: Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf entsprechende Beschreibungen in der Softwarereferenz hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.
*   **Lesehinweis**: Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen. Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

#### Darstellungskonventionen

Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

| Stil | Bedeutung |
| :--- | :--- |
| *Kursiv* | sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Muster senkrecht/waagerecht*. |
| **Fett** | sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B. geben Sie den Wert **0** ein. |
| > | Mit dem sogenannten Brotkrumenpfad ist der Weg gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B. Datei > Importieren > Übergabedatei. |
| [] | Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B. mit [OK] speichern Sie die Daten. |
| <> | Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B. mit <F1> öffnen Sie die Online-Hilfe. |

### Produktportfolio der A+W Software GmbH

In dieser Abbildung wird A+W Production als Produktionsplanungs- und Steuerungs-System im Anschluss an das ERP-System im gesamten Unternehmensprozess dargestellt.

**Systemkomponenten:**

*   **ERP (Enterprise Resource Planning)**
    *   **ERP Solution:**
        *   A+W Enterprise
        *   A+W Business
        *   Module: Verkauf, Einkauf, Lager, Versand, Statistik, eCommerce
*   **PPS (Production Planning and Control)**
    *   **PPS Solution:**
        *   A+W Production
        *   Module: Kapazitätsplanung, Produktionsplanung (Grob- und Feinplanung), Verschnittoptimierung
*   **Maschinen-steuerung**
    *   **Control Units:**
        *   Production Terminal
        *   Realtime Optimizer
        *   Rack Optimizer
        *   DynOpt
        *   Monitoring
        *   Controlling
        *   Barcoding
*   **Maschinen**
    *   Zuschnittslinie
    *   ISO Linie
    *   VSG Linie

*   **CAD Konstruktion**
    *   A+W CAD Designer (Bars) (Shapes + Bars)

**(Abb. A-1 A+W Software GmbH Produktfolio)**

### A+W Production stellt sich vor

Steigende Anforderungen an die Produktion erfordern immer leistungsfähigere Planungs- und Steuerungsapplikationen.

A+W Production ist die Produktions-Planungs- und Steuerungs-Software aus dem Hause A+W Software GmbH. Die modulare Architektur erlaubt die optimale Anpassung an Ihre Anforderungen. Welche der angebotenen Lösungen in welcher Ausbaustufe für Ihr Unternehmen in Frage kommt, wird in Gesprächen mit Ihnen eingehend analysiert.

A+W Production stellt Ihnen einen Vielzahl an modernen Methoden und Werkzeugen zur Verfügung, mit welchen Sie Ihre komplette Produktion planen, steuern, überwachen und auswerten können - von der Einlastung der Auftragsdaten bis hin zur Erzeugung von NC-Code und Buchung von BDE-Daten. Zusätzlich zu diesen standardisierten Prozessen, können Sie direkt und dynamisch in die Produktion eingreifen um bspw. wichtige Eilaufträge einzusteuern oder Engpässe zu beseitigen. So haben Sie stets die volle Kontrolle über alle produktionsrelevanten Ressourcen und Daten - Maschinen, Kosten, Zeiten und Kapazitäten.

Sowohl durch die Vernetzung mit Maschinen und anderen Softwaremodulen aus dem Hause A+W Software GmbH als auch durch die Prozessvisualisierung und -steuerung mittels Production Terminals an den Arbeitsstationen wird ein hohes Maß an Qualität erreicht.

Die Software ist zur Zeit in 12 Sprachen weltweit im Einsatz.

Um die modulare Struktur von A+W Production abbilden zu können, wurde die Software in zwei Kategorien unterteilt:
*   Basissystem
*   Ausbaumodule

**Das Basissystem umfasst die Bereiche:**
*   Einlastung
*   Grobplanung
*   Feinplanung
*   Maschinenzuordnung

**Darüber hinaus stehen folgende Ausbaumodule zur Verfügung:**
*   Kapazitätsplanung
*   Optimierungssysteme
    *   Realtime Optimizer
    *   Sequence Optimizer
    *   Shape Optimizer
    *   Rack Optimizer
    *   DynOpt
    *   Furnace Optimizer
*   Barcode Manager
*   Anzeige- und Leitrechnersysteme
    *   Production Terminal
*   Statistiksysteme
    *   A+W Discovery
    *   Production Cockpit

#### Prozessablauf mit A+W Production

**(Abb. A-2 Prozessablauf A+W Production)**

Der Prozessablauf ist wie folgt visualisiert:

1.  **ERP Auftragserfassung**: Startpunkt des Prozesses.
2.  **Auftrags-Prüfung**: Aufträge werden geprüft. Bei Fehlern geht eine Info an die Auftragserfassung.
3.  **Auftrags-Analyse**: Bei OK werden die Aufträge analysiert und gehen in den **Auftrags-Pool** innerhalb der **Produktions-Planung**.
4.  **Produktions-Planung**:
    *   **Auftrags-Pool**: Enthält ungeplante Aufträge (z.B. Auftrag 1, 2, 3, 4).
    *   **Grobgeplante Läufe**: Aufträge werden zu Läufen zusammengefasst (Lauf 1, 2, 3, 4) und durchlaufen eine Qualitätskontrolle.
    *   **Feingeplante Läufe**: Nach der Kontrolle werden die Läufe feingeplant.
    *   **Job Release**: Die feingeplanten Läufe werden freigegeben.
5.  **Freigegebene Läufe**: Werden an die Produktion übergeben. Parallel kann ein **CAD Designer** eingesetzt werden.
6.  **Produktionsschritte**:
    *   **Zuschnitt**: Einsatz von **Realtime Optimizer**.
    *   **Glas-Bearbeitung**: Einsatz von **Production Terminals**.
    *   **Glas-Bearbeitung ESG/VSG**: Einsatz von **Production Terminal IN/OUT**.
    *   **Glas-Bearbeitung ISO-Linie**.
    *   **Versandbereich**: Einsatz von **Barcode Manager**.
7.  **Datenbank**: Alle Produktionsdaten, Monitoring-Informationen und AWDiscovery-Analysen werden in einer zentralen Datenbank gespeichert und für die Produktionsplanung und -überwachung genutzt.

---

## Basismodul A+W Production

In diesem Themenblock lernen Sie, wie Sie mit dem Basismodul arbeiten.
Der Themenblock beinhaltet folgende Schulungseinheiten:
*   Einlastung
*   Grobplanung
*   Feinplanung
*   Maschinenzuordnung

### Einlastung

In diesem Themenblock lernen Sie die Funktionsweise des Einlastungsprozesses von A+W Production kennen.

**Lernziele**
*   Die Arbeitsweise der Einlastung kennenlernen
*   Über beteiligte Module, Prozesse und Abläufe informiert sein.

**Nutzen**
Nur wenn Sie die Arbeitsweise kennen und verstehen, können Sie die nachgelagerten Prozesse verstehen und entsprechend ausrichten.

**Definitionen**
*   **Items4ALCIM**: Modulname des Einlastungsdienstes. Wird als Begriff häufig synonym verwendet.

> **Merke: Dienst**
> Die Einlastung ist ein Windows-Dienst und kann aktiv und interaktiv laufen. Aktiv wird er durch den Benutzer gesteuert oder interaktiv läuft er als Hintergrundprozess. Es ist möglich, mehrere Einlastungsprozesse parallel laufen zu lassen.

#### Einlastung allgemein

Mittels des Einlastungsprozesses (Windowsdienst) werden die Auftragsdaten aus dem ERP-System aktiv in die Produktionsdatenbank geschrieben.

Die Daten können auf zwei Wegen zwischen den Systemen übertragen werden:
*   **Direkter Datenimport**: Durch direkten Zugriff auf eine A+W Enterprise-Datenbank.
*   **Mittels einer XML-basierten Standard-Schnittstelle** (z. B. aus A+W Business).

Die Prozessabläufe und beteiligten Module werden in folgenden Schaubildern dargestellt:

**(Abb. A-3 Zusammenspiel A+W Enterprise und A+W Production & Abb. A-4 Zusammenspiel A+W Business und A+W Production)**

**Prozessschritte der Einlastung:**

Im Verlauf der Einlastung werden folgende Prozessschritte je Auftragsposition ausgeführt:
1.  Was? - Stammdaten
2.  Wo? - Maschinenzuordnung
3.  Wie lange? - Kapazitätsplanung
4.  Wann? - Kapazitätsplanung
5.  Erstellung der SN-Dateien
6.  Füllen der sogenannten "Pool_"-Tabellen
7.  Laden und Ausführen von Kundenanpassungen
8.  Geometrieberechnung
9.  BDE-Initialisierung
10. Rückmeldung ERP-System (über WebService)

Nach dem Einlesen der letzten Position werden die Auftragsdaten gespeichert. Die eingelesenen Aufträge finden Sie nun in der sogenannten Pool-Anzeige (erster Schritt im Prozess der Grobplanung).

Die ausgeführten Prozessschritte sind davon abhängen, wie das System konfiguriert ist und welche Zusatzmodule eingerichtet sind. Das bedeutet, wenn Sie ohne die Kapazitätsplanung arbeiten, werden die Schritte 3 und 4 nicht ausgeführt.

### Grobplanung

In diesem Themenblock lernen Sie die Grobplanung von A+W Production kennen.

**Lernziele**
*   Die unterschiedlichen Anzeigen kennenlernen

**Nutzen**
Ziel und Nutzen der Grobplanung im Rahmen der Arbeitsvorbereitung verstehen. Nur wenn Sie die Arbeitsweise der Grobplanung kennen und versehen, können Sie Läufe effizient bilden und verwalten.

**Definitionen**

*   **Grobplanung**: Der Prozess der Grobplanung und die dazu zur Verfügung gestellten Anzeigen und Werkzeuge dienen einer effizienten Auftragsvorbereitung (Laufplanung und -verwaltung). Abhängig von produktionsrelevanten Faktoren wie bspw. Maschinen und Auftragsdaten können Läufe immer völlig unterschiedlich sein und flexibel verwaltet werden.
*   **Pool**: Nach dem Einlasten der Aufträge, finden Sie diese in der sog. Pool-Anzeige. Diese zeigt alle unverplanten Produkte und Zwischenprodukte (Auftragsvorbereitung).
*   **Topf**: Sie können vor der Laufbildung Produkte bzw. einzelne Positionen zusammenfassen um sich einen generellen Überblick der Mengen zu verschaffen. Die Topf-Anzeige zeigt alle vorgruppierten Produkte und einzelne Positionen (Freigabeteile).
*   **Lauf**: Läufe sind das Ergebnis der Grobplanung. Sie können zur Produktion freigegeben oder auch wieder aufgelöst werden. Die Lauf-Anzeige zeigt alle grobgeplanten Aufträge und einzelne Positionen (Freigabeteile).
*   **Freigabeteil**: Unter Freigabeteilen sind explizit für die Produktion zu planende Teile zu verstehen. Nicht-Freigabeteile werden implizit zur Produktion eingeplant, was z. B. für Gläser gilt, die zugeschnitten werden. Freigabeteile werden in den A+W Production-Anzeigen explizit angezeigt.
*   **Stückliste**: Listet alle Komponenten hierarchisch und beschreibt exakt deren Abhängigkeiten (Oberteil / Unterteil) inklusive Bearbeitungen.
*   **Bearbeitung**: Arbeitsschritte an einem Glas/Produkt, z. B. Zuschnitt, Härten, Versand.

> **Merke: Anzeigen**
> Die verschiedenen Anzeigen von A+W Production filtern Informationen aus verschiedenen Datenbankeinträgen. Das Anzeigesystem ist flexibel an die Bedürfnisse des Planers anpassbar.

#### Grobplanung allgemein

Die Grobplanung ist ein Prozess in der Arbeitsvorbereitung, in welchem Sie sich einen Gesamtüberblick über die zu produzierenden Aufträge verschaffen, und sie dann in geeignete Läufe zur Produktion einteilen. Das Besondere an der Grobplanung ist dabei, dass die mengenorientierte Betrachtung der zu produzierenden Aufträge und Positionen nach beliebigen Kriterien möglich ist. Das geschieht durch die verschieden konfigurierbaren Anzeigen.

**Übersicht der Anzeigen:**

*   **Pool-Anzeige**: Zeigt alle unverplanten Aufträge, Produkte und Zwischenprodukte.
*   **Topf-Anzeige**: Zeigt alle vorgruppierten Aufträge, Produkte und Zwischenprodukte.
*   **Lauf-Anzeige**: Zeigt alle grobgeplanten Aufträge, Produkte und Zwischenprodukte.
*   **Detail-Anzeige**: Zeigt alle Freigabeteile und deren besondere Merkmale (z. B. Sprossen, Modelle, ...).
*   **Bearbeitungs-Anzeige**: Zeigt alle Teile und deren Bearbeitungen.
*   **Glasarten-Anzeige**: Zeigt alle Teile inklusive der Basisgläser, jedoch ohne Kopfteil sowie Glaskombinationen für ISO.
*   **Füllauftrag-Anzeige**: Zeigt alle Freigabeteile.
*   **Positions-Anzeige**: Zeigt die Stücklistenstruktur an und dient als Editor.
*   **Auftragsübersicht**: Zeigt die komplette Stücklistenstruktur.
*   **BDE-Anzeige**: Zeigt Status und Historie von Aufträgen, Produkten und Zwischenprodukten.
*   **Produktionslos-Anzeige**: Zeigt Ergebnisdaten der Feinplanung.

Mit Hilfe des Ansichtenkonzeptes können Sie so, vor dem Start der Feinplanung, Läufe jederzeit flexibel erstellen und ändern.

#### Die Auftrags-Anzeige (Pool)

Nach dem Import der Auftragsdaten werden alle fehlerfrei übernommenen Daten in einen Pool gestellt. Die Auftrags-Anzeige stellt den unverplanten Auftragsbestand dar und ermöglicht eine liefertermin-, tour- oder kundenorientierte Planung.

#### Die Auftragsübersicht

In dieser Anzeige bekommen Sie eine übersichtliche Gliederung und Darstellung der kompletten Stücklistenstruktur. Die Anzeige kann konfiguriert werden.

#### Die Topf-Anzeige

Aufträge, Produkte und Zwischenprodukte (Freigabeteile) können zu Töpfen zusammengefasst werden. Töpfe dienen als Hilfsmittel zur Voreinteilung, müssen aber nicht zwingend verwendet werden.

#### Die Positions-Anzeige

In dieser Ansicht werden die Auftragsdaten für eine Auswahl angezeigt. Die Positions-Anzeige ist auch geeignet, um für eine Auswahl (z. B. einen Lauf) die darin enthaltenen Aufträge zu ermitteln.

#### Die Glasarten-Anzeige

In der Glasarten-Anzeige werden die Bestandteile der Produkte dargestellt. Daher eignet sich die Glasarten-Anzeige besonders für die Zusammenstellung von Läufen und Töpfen für den Zuschnitt.

#### Die Detail-Anzeige

Die Detail-Anzeige entspricht der Auftrags-Anzeige, arbeitet aber mit einer beliebig selektierten Menge.

#### Die Bearbeitungs-Anzeige

Die Bearbeitungs-Anzeige gibt Ihnen einen Überblick über die Teile und deren Bearbeitung.

#### Die Füllauftrag-Anzeige

Die Füllauftrag-Anzeige entspricht der Auftrags-Anzeige, zeigt Ihnen jedoch nur die Aufträge, die Sie zuvor als Füllaufträge gekennzeichnet haben.

#### Die Lauf-Anzeige

Die Lauf-Anzeige gibt Ihnen einen Überblick über die vorhandenen Läufe und deren Status (grobgeplant, feingeplant, in Produktion, usw.). Läufe sind das Ergebnis der Grobplanung.

#### Läufe bilden

Läufe können Sie aus folgenden Anzeigen heraus bilden:
*   Auftrags-Anzeige
*   Topf-Anzeige
*   Füllauftrag-Anzeige
*   Detail-Anzeige
*   Bearbeitungs-Anzeige
*   Glasarten-Anzeige

**Bildung von Läufen**
Im Allgemeinen erfolgt der Planungsprozess in verschiedenen Stufen. Zuerst wird aufgrund der Hauptkriterien getrennt, dann das Ergebnis überprüft: Menge, Ausbeute, Restplatten Lagermaße, Anzahl benötigter Gestelle.

Läufe können bspw. nach folgenden Kriterien gebildet werden:
*   **Nach der Glasart**: Dicke Gläser haben in der Regel größere Abmessungen und sind teuerer und schwerer.
*   **Nach Produktart**: In komplexen Produktionen werden unterschiedliche Glasarten (z. B. ISO, VSG und ESG) separiert.
*   **Nach Bearbeitung**: Bestimmte Bearbeitungen erfordern eine lange Vorlaufzeit oder sind teuer.
*   **Nach Produktionsdatum**: Mit der Kapazitätsplanung wird das Produktionsdatum ermittelt.
*   **Nach Auftrag oder Position**: Das Programm verfolgt den Arbeitsfortschritt auf Teileebene.

**Allgemeine Regeln**
Ein Lauf muss Sinn machen: Er sollte eine angemessene Größe (ca. 2 Arbeitsstunden) haben. Die Größe sollte für ein gutes Ergebnis veränderbar sein. Sie sollten Spezialprodukte nicht isolieren (mischen Sie diese zu den Standardläufen und stellen Sie sie auf separate Gestelle).

### Feinplanung

In diesem Themenblock lernen Sie die Feinplanung kennen.

**Lernziele**
*   Ziele und Rahmenbedingungen der Feinplanung kennenlernen
*   Unterschiedliche Optimierungsmodi kennenlernen
*   Unterschiedliche Organisationsformen kennenlernen

**Nutzen**
Die Feinplanung beinhaltet verschiedene Module und Funktionen, die Ihre Produktion zielgerichtet in Produktionssequenz und Verschnittoptimierung ausrichten. Die Aufgabe der Feinplanung ist es, die Produktionsreihenfolge für die Inhalte der Läufe zu ermitteln.

**Definitionen**
*   **Gruppierung**: Erfolgt nach unterschiedlichen und eindeutigen Werten für eine Eigenschaft, z. B. nach Kundennummer, Glasart.
*   **Sortierung**: Erfolgt nach Eigenschaften, die einen fortlaufenden Wert innerhalb der gegebenen Gruppe annehmen (z. B. Glasdicke oder Größe).
*   **Physikalischer Abstellplatz**: Gestell (A-Bock, L-Bock, Fester Abstellplatz)
*   **Logischer Abstellplatz**: Auf einem physikalischen Abstellplatz können Sie mehrere logische Abstellplätze (Glasstapel) nebeneinander haben.
*   **Orga**: Abbildung Ihrer Produktion in Sequenz und Laufwegen über definierte Regeln und Filter.

> **Merke: Trennung von Glasarten**
> stellt sicher, dass unterschiedliche Glasarten in einem Stapel nicht vermischt werden und erstellt je Glasart einen separaten Stapel auf einem physikalischen oder logischen Abstellplatz.

#### Feinplanung allgemein

Laufwege durch die Produktion können verschiedene Bearbeitungsprozesse beinhalten.

**Ablauf der Feinplanung**
Die Feinplanung ist der zweite Schritt der Arbeitsvorbereitung und beginnt nach Abschluss der Grobplanung. Aufgabe der Feinplanung ist es, für die in den Läufen enthaltenen Teile die Produktionsreihenfolge zu erstellen, um die Abstellplätze zu definieren (Anzahl und Zuordnung).

Die Produktionsreihenfolge kann sich durch folgende Kriterien ergeben:
*   Durch die Vorgaben des Kunden (z. B. Entladereihenfolge bei Lieferung),
*   durch die Ergebnisse einer Gestell- und Packmitteloptimierung (Rack Optimizer) oder
*   durch fertigungstechnische Restriktionen

Die Feinplanung läuft in verschiedenen Schritten ab. Alle dazu notwendigen Prozesse werden im Hintergrund abgearbeitet. Das Spannungsfeld der Feinplanung liegt zwischen **Reihenfolge**, **Verschnitt** und **Flexibilität**.

#### Gruppierungen und Sortierungen

Die Gruppierungen und Sortierungen dienen dazu, den verschiedenen Abstellplätzen die gewünschte Produktionsreihenfolge zuzuweisen. Die Optimierung berechnet unter Berücksichtigung von Gruppierung und Sortierung den bestmöglichen Verschnitt unter Einhaltung der definierten Produktionssequenz.

#### Abstellplatz- und Stapellogik

In der Feinplanung haben Sie verschiedene Kriterien zur Verfügung, um Scheiben auf Abstellplätze zu stellen. Dies verbessert die Durchlaufzeiten und vermeidet unnötiges Umsortieren, Bruch und Suchen von Gläsern.

A+W Production bietet Ihnen verschiedene Standardorganisationen an, basierend auf über 40 Jahren Erfahrung:
*   Speziell ausgerichtete Organisationen für A-Böcke
*   Speziell ausgerichtete Organisationen für Fächerwagen
*   Speziell ausgerichtete Organisationen für Einheiten (ISO, VSG)
*   Speziell ausgerichtete Organisationen für mehrstufige Produktionsformen
*   Speziell ausgerichtete Organisationen für Los-basierte Produktionsformen

#### Abstellmodi für A-Böcke

*   **Abstellmodus Glas**: Eine Glasart pro Abstellplatz.
*   **Abstellmodus Einheit**: Jede Einheit auf einem logischen Abstellplatz.
*   **Abstellmodus Produktion**: Verschiedene Glasarten auf einer logischen Abstellplatznummer mit mehreren Stapeln.
*   **Abstellmodus VABGLA**: Pro Glasart ein logischer Abstellplatz mit jeweils einem Stapel.

#### Abstellmodi für Fächerwagen

*   **Zusammen**: Scheibe und Gegenscheibe(n) immer zusammen auf einen Fächerwagen.
*   **Glas**: Scheiben immer getrennt weggestellt.

#### Optimierungs-Modi

In A+W Production können Sie folgende Optimierungsmodi einstellen:
*   XOPTS 6.2
*   XOPTS 6.1
*   XOPTS 5.2
*   XOPTS 5.1
*   XOPT

*   **Optimierungsmodus XOPTS 6.2 - Feste Reihenfolge**: Arbeitet mit einer strikten Reihenfolge der Gruppen und der Gläser innerhalb der Gruppen.
*   **Optimierungsmodus XOPTS 6.1 - Kunden zusammenhalten**: Reihenfolge der Gläser innerhalb der Gruppen ist fest. Die Gruppen können in ihrer Anordnung verändert werden, um das Ergebnis zu verbessern.
*   **Optimierungsmodus XOPTS 5.2 - Standard**: Standard-Modus der Feinplanung. Teile innerhalb der Gruppen können frei optimiert werden.
*   **Optimierungsmodus XOPTS 5.1 - ISO auf Fächerwagen oder viele A-Böcke**: Frei optimiert, lediglich Einheiten (z.B. ISO) werden zusammengehalten.
*   **Optimierungsmodus XOPT - Scheiben auf Fächerwagen**: Standardoptimierung für Scheiben auf Fächerwagen.

#### Organisationsformen

Um einen Lauf korrekt und effizient planen zu können, stehen Ihnen sogenannte Orgas zur Verfügung. Eine Orga ist nichts anderes als ein datentechnisches Regelwerk zur Abbildung der Produktion.

#### Orga-Typ und Los-Typ

Jedes Teil bzw. jede Bearbeitung hat seinen Teiletyp bzw. Bearbeitungstyp (Basisglas, VSG, etc.) und seine Beschaffungsart (Bestellt, Zuschnitt, etc.). Abhängig von diesen Eigenschaften wird das Teil einem bestimmten Lostyp zugewiesen. Produktionslose werden für unterschiedliche Teiletypen und verschiedene Glasarten im Zuschnitt gebildet.

### Maschinenzuordnung

In diesem Themenblock lernen Sie die Maschinenzuordnung kennen.

**Lernziele**
*   Die Maschinenzuordnung kennenlernen

**Nutzen**
Mit Maschinen wird der physikalische Maschinenpark abgebildet. Somit bilden Maschinen die Basis, um die Produktion zu steuern.

**Definitionen**

*   **Maschinen**: Bilden physikalische Maschinen im Maschinenpark ab.
*   **Logische Maschine**: Datentechnische Beschreibung eines Teils einer Maschine oder eines Betriebszustandes.
*   **Maschinentypen**: Definieren, um welchen Typ einer Maschine es sich handelt (z.B. Zuschnitt, Rahmenbieger).
*   **Arbeitsgänge**: Bringen Eigenschaften des Bearbeitungstyps mit denen eines Werkstücks zusammen.
*   **Bearbeitungstypen**: Beschreiben die technische Form einer Bearbeitung.
*   **Bearbeitungsartikel**: Definieren Bearbeitungstypen genauer.

> **Merke: Arbeitsgangzuordnung**
> Mit der Arbeitsgangzuordnung hat der Anwender die Möglichkeit in den Produktionsprozess einzugreifen. Die Arbeitsgangzuordnung verbindet logische Maschinen mit Arbeitsgängen.

#### Bestandteile der Maschinenzuordnung

Maschinen werden durch einen Maschinentyp, Eigenschaften und Restriktionen definiert. Eine Maschine ist mit einer logischen Maschine verknüpft, welche wiederum mit einem Arbeitsgang verbunden ist. Der Arbeitsgang wird durch einen Bearbeitungstyp oder -artikel definiert. All dies wird durch die Arbeitsgangzuordnung gesteuert.

#### Maschinen in der Maschinenzuordnung

Im Register *Maschinen* sind alle physikalischen Maschinen gelistet. Sie ordnen jeder Maschine einen Maschinentyp zu.

#### Arbeitsgänge in der Maschinenzuordnung

Ein Arbeitsgang wird durch einen hinterlegten Bearbeitungstyp, einen Bearbeitungsartikel, eine Artikelgruppe und/oder eine zusätzliche Bedingung definiert.

#### Arbeitsgangzuordnung

Hier ordnen Sie logische Maschinen den Arbeitsgängen zu. Unter jedem Arbeitsgang kann die Reihenfolge, und damit die Priorität der logischen Maschinen, individuell festgelegt werden.

> **Beispiel: Arbeitsgangzuordnung**
> Sie haben in Ihrer Produktion eine Rechteckschleifmaschine und ein CNC-Center.
> *   Ein Arbeitsgang *Rechteckschleifen* wird der Rechteckschleifmaschine mit höchster Priorität zugeordnet.
> *   Ein Arbeitsgang *Modellschleifen* wird dem CNC-Center zugeordnet.
> *   Das CNC-Center ist auch dem Arbeitsgang *Rechteckschleifen* zugeordnet, aber mit geringerer Priorität.
> So wird das Schleifen von Rechtecken auf der kostengünstigeren Maschine durchgeführt. Bei Engpässen wird auf das CNC-Center ausgewichen.

#### Bearbeitungstypen in der Maschinenzuordnung

Mit einem Bearbeitungstyp wird beschrieben, um welche technische Form der Bearbeitung es sich handelt (z.B. Zuschnitt, Montage, Schleifen).

#### Bearbeitungsartikel in der Maschinenzuordnung

Bearbeitungsartikel referenzieren auf Bearbeitungstypen und können diese genauer beschreiben (z.B. Facetten-Schleifen, Gehrungs-Schleifen).

---

## A+W Production Ausbaumodule

In diesem Themenblock lernen Sie die Ausbau- und Zusatzmodule von A+W Production kennen.

Der Themenblock beinhaltet folgende Schulungseinheiten:
*   **Kapazitätsplanung**
    *   A+W Capacity Planner
*   **Optimierungssysteme**
    *   Realtime Optimizer
    *   Sequence Optimizer
    *   Shape Optimizer
    *   Rack Optimizer
    *   DynOpt
    *   Furnace Optimizer
*   **Barcode Manager**
*   **Anzeige- und Leitrechnersysteme**
    *   Production Terminal
*   **Statistiksysteme**
    *   A+W Discovery
    *   Production Cockpit

### Kapazitätsplanung

**Lernziele**
*   Die Kapazitätsplanung kennenlernen.
*   Über Bedienungsprinzipien und Möglichkeiten informiert sein.
*   Den Prozessfluss und die Interaktion mit den anderen Modulen kennenlernen.

**Nutzen**
Mit Hilfe der Kapazitätsplanung können Sie gegenüber Ihren Kunden schnell Auskunft geben über generelle Möglichkeiten, Produktionsauslastung und Kosten.

**Definitionen**
*   **Übergangszeiten**: Ruhephasen für das Glas zwischen Arbeitsgängen (z.B. Autoklavprozess).
*   **Kapazität**: Definierte Zeitspanne, in der eine Maschine zur Verfügung steht.
*   **Auslastung**: Zeitspanne innerhalb der Gesamtkapazität, für die bereits Arbeit eingelastet ist.
*   **Reservierung**: Zeitspanne für besondere Aufträge.
*   **Kampagne**: Zeitspanne, in der die Maschine nur einen bestimmten Arbeitsgang ausführt.
*   **Maschine**: Physikalische Maschine.

> **Merke: Modus**
> Wenn bei der Rückwärtsterminierung der Produktionsstart in der Vergangenheit liegt oder der Liefertermin nicht gehalten werden kann, wird auf Eilraster umgeschaltet und eine neue Berechnung durchgeführt.

> **Merke: Produktionsmonitor**
> Über diesen können Sie direkt die entsprechende Maschine und deren Einstellungen (z. B. Kapazitäten) und darauf eingelastete Auftragsdaten bearbeiten.

#### A+W Capacity Planner

Der A+W Capacity Planner dient zur Verplanung der vorhandenen Produktionskapazitäten im direkten Abgleich zu den für den Auftragsbestand bereits reservierten Kapazitäten. Dies ermöglicht ein frühzeitiges Erkennen von Produktionsengpässen. Die Planung erfolgt auf Basis von Produktionsauslastungen je Maschine. Die Basis bilden hinterlegte Stammdaten (Zeiten, Schichtpläne, Kosten).

*   **Produktionsmonitor**: Bietet eine detaillierte Kapazitätsübersicht.
    *   Zeigt grafisch: Arbeitsrückstand, Schichten, Arbeitsauslastung, Überlast, Arbeitsfortschritt, Reservierungen.
*   **Kampagneneditor**: Zur Verwaltung von Kampagnenterminen für ausgewählte Arbeitsgänge.
*   **Schichteditor**: Zum Anlegen und Konfigurieren von Schichten, Schichtplänen und Schichtregeln.
*   **Grafisch orientierte Terminumlastung**: Editor, um einzelne oder Gruppen von Bearbeitungen auf alternative Maschinen und Schichten umzulasten.

### Optimierungssysteme

**Nutzen**
Optimierungssysteme helfen Ihnen, Ihre Produktion besser auszulasten und Verschnitt zu minimieren. Das spart Zeit und Geld.

**Definitionen**
*   **A+W Realtime Optimizer**: Online-Zuschnitt-Leitrechner, um nach erfolgter Optimierung in Fertigungsläufe einzugreifen.
*   **A+W Sequence Optimizer**: Optimiert den Verschnitt einzelner Glasarten unter Berücksichtigung der Sortierreihenfolge.
*   **A+W Shape Optimizer**: Legt Modelle aus unterschiedlichen Positionen flächensparend innerhalb eines Rechtecks zusammen.
*   **A+W Rack Optimizer**: Ermöglicht die Direktverpackung von Scheiben auf Versandgestelle und optimiert die Belegung.
*   **A+W DynOpt**: Dynamisches Optimierungs- und Zuschnittkontrollsystem, das bei Einhaltung von Fertigungssequenzen mit dem höchsten Ertrag optimiert.
*   **A+W Furnace Optimizer**: Ermittelt die optimale Belegung des Ofenbetts.

#### Realtime Optimizer

Der A+W Realtime Optimizer ist ein Leitrechner zur Verbesserung der Glasausbeute und der Prozesse im Zuschnitt. Er erlaubt das automatische Verlinken gleicher Glasarten aus verschiedenen Läufen und das direkte Schneiden von Bruchscheiben.
*   **Tischoptimierungen**: Können direkt am Zuschnitttisch erzeugt werden.
*   **Tischansteuerung**: Arbeitet als Leitstand für einen Zuschnitttisch.
*   **Stammdaten**: Können direkt am Zuschnitt eingesehen und angepasst werden.

#### Sequence Optimizer

Der A+W Sequence Optimizer optimiert den Verschnitt einzelner Glasarten der feingeplanten Produktionsläufe unter Berücksichtigung der Sortierreihenfolgen, Eilscheiben und Füllpositionen.

#### Shape Optimizer

Der A+W Shape Optimizer ermöglicht eine erweiterte Modelloptimierung, indem er Modelle aus unterschiedlichen Positionen flächensparend innerhalb eines Rechtecks zusammenschachtelt.

#### Rack Optimizer

Der A+W Rack Optimizer ermöglicht die Direktverpackung der Scheiben in der Produktion auf Versandgestelle. Die Sequenz der Scheiben wird entsprechend der Gestellzuweisung durch den gesamten Produktionsprozess vererbt.

#### DynOpt

A+W DynOpt ist ein dynamisches Optimierungs- und Zuschnitt-Kontrollsystem. Es ermöglicht die gleichzeitige Steuerung mehrerer Zuschnitttische und Isolierglaslinien und sorgt für einen kontinuierlichen Glasfluss.

#### Furnace Optimizer

Durch den A+W Furnace Optimizer wird unter Berücksichtigung gegebener Randbedingungen, eine optimale Belegung des Ofenbetts ermittelt.

### Barcode Manager

**Lernziele**
*   Den A+W Barcode Manager kennenlernen und verstehen.

**Nutzen**
Der A+W Barcode Manager liefert Ihnen einen Überblick zum Produktionsfortschritt, d. h. was befindet sich wo. Sie können dynamisch in den Produktionsprozess eingreifen und diesen beeinflussen.

**Definitionen**
*   **Einheiten**: Anhand von Etiketten können Scheiben/Einheiten überall verfolgt werden.
*   **Gestelle**: Sind ebenfalls mit Etiketten versehen.
*   **Erfassungsstellen**: Stellen in der Produktion, an denen Scheiben/Einheiten gescannt werden.

#### Allgemein

Der A+W Barcode Manager erfasst den Produktionsfluss an wichtigen Stellen (Erfassungsstellen) mit Hilfe von Barcodes, Scannern, Leitrechnern usw. Die Erfassungsstellen haben einen zentralen Stellenwert. Eine Maschine kann in mehrere Erfassungsstellen aufgeteilt sein (z.B. ISO-Linie: Eingang, Maschine, Ausgang).

#### Scanner

In der BDE kommen verschieden Scannertypen zum Einsatz:
*   **Online-Scanner**: Übertragen Scandaten direkt an das System; bei Verbindungsabbruch gehen Daten verloren.
*   **Offline-Scanner**: Verfügen über Speicher und übertragen die Daten bei Verbindung mit dem System.

### Anzeige- und Leitrechnersysteme

**Nutzen**
Mittels der A+W Leitrechner bekommen Sie an jeder Arbeitsstation genau die Information angezeigt, die Sie brauchen. Weiterhin können Sie direkt Produktionsprozesse anstoßen, NC-Codes generieren und Produktionsbuchungen (BDE) vornehmen.

**Definitionen**
*   **A+W Production Terminals**: Leitrechnersystem zur Anzeige und Steuerung des Arbeitsvorrates an bestimmten Stellen innerhalb der Produktion.
*   **A+W Production Cockpit**: Online-Monitoring und Controlling-System. Visualisiert Ihnen stets die aktuellen Produktionsdaten.

#### Production Terminal

Production Terminals sind interaktive Anzeige- und Leitrechnersysteme im Produktionsbereich. Es gibt sie in folgenden Varianten:
*   **Manual Cutting**: Visualisiert am Handzuschnitttisch den Arbeitsplan.
*   **Order**: Dient zur auftrags- oder laufbasierten Bearbeitung von Daten von einem zentralen Punkt aus.
*   **Processing**: Kommt an Bearbeitungsmaschinen zum Einsatz und steuert diese an.
*   **IG-In**: Visualisiert den Arbeitsvorrat am Einlauf der Isolierglaslinie.
*   **IG-Assembly**: Visualisiert die technischen Daten jeder zu fertigenden Einheit vor der Rahmensetzstation.
*   **IG-Out**: Visualisiert am Auslauf der Isolierglaslinie die technischen und versandorientierten Daten.
*   **TG-In**: Anzeigesystem am Ofeneinlauf, zeigt die Belegung des Ofenbettes.
*   **TG-Out**: Anzeigesystem am Ofenauslauf.

**Ziel der Production Terminals**
*   Geplante Jobs/Lose werden auf Arbeitsplätze verteilt.
*   Durchgeführte Arbeiten werden gebucht.
*   Abweichungen werden erfasst.
*   Produktionsfortschritt wird angezeigt.
*   Nachläufer (wegen Bruch) werden automatisch generiert.
*   Gesammelte Daten werden für Auswertungen genutzt.

### Statistiksysteme

**Nutzen**
Statistiksysteme helfen Ihnen, Ihre Produktionsdaten quantitativ aufzubereiten und dienen Ihnen somit zur besseren Beurteilung.

**Definitionen**
*   **OLAP**: Online Analytical Processing. OLAP-Würfel werden häufig zur Analyse komplexer Unternehmensdatenbeständen eingesetzt.
*   **A+W Discovery**: Modernes Business Intelligence System von A+W. Als Auswertungsoberfläche dient Microsoft Excel (ab Version 2010).
*   **A+W Production Cockpit**: Online Produktionsbenchmarking. Zeigt den aktuellen Nutzungsgrad, Status der Maschinen, Produktivität und weitere Kennzahlen in Echtzeit.

#### A+W Discovery

A+W Discovery ist das Business Intelligence System aus dem Hause A+W. Es unterstützt die Konvertierung, Integration und Analyse von heterogenen Daten aus multiplen Quellen. Durch OLAP-Technologie werden schnelle Datenzugriffe und komplexe Berechnungen ermöglicht.

#### Production Cockpit

Mit dem A+W Production Cockpit erhalten Sie einen transparenten Überblick über den aktuellen Status der Fertigung. Gegliedert nach Teilbereichen (Zuschnitt, Isolierglaslinien, etc.) zeigt das Programm Kennzahlen in Echtzeit.

---

## Konventionen

### Bedienoberfläche

Dieses Kapitel gibt Ihnen einen Überblick über die Bedienelemente, die Sie in der Software finden.

#### Dialoge

Dieses Kapitel gibt Ihnen einen Überblick über die Softwarebegriffe, die in diesem Handbuch zur Beschreibung eines Dialoges verwendet werden.

| Begriff | Beschreibung |
| :--- | :--- |
| **Register** | Zur besseren Übersicht teilen Register den Dialog nach unterschiedlichen Themen. |
| **Schaltfläche** | Z.B. [OK], [Abbrechen]. |
| **Schnelltaste/Hot-Key** | Tastenkombinationen, z.B. <Alt> + unterstrichener Buchstabe. |
| **Optionsschalter** | (Radio button) Erlauben die Auswahl von nur einer Option. |
| **Kombobox** | Dropdown-Listen mit zur Auswahl stehenden Optionen. |
| **Checkbox** | Erlauben das getrennte Aktivieren/Deaktivieren von Optionen. |
| **Feld** | Eingabefeld für Werte. |
| **Titelleiste** | Oberste Leiste eines Fensters. |
| **Menüleiste/Menüpunkt** | Menüstruktur (Datei, Bearbeiten, ...). |
| **Symbolleiste** | Leiste mit Icons für schnellen Zugriff. |
| **Dialog öffnen** | Eine Schaltfläche mit `...` öffnet einen weiteren Dialog. |
| **Tabellen-/Spaltenüberschrift** | Kopfzeile einer Tabelle. |

#### Schaltflächen

*   **[...]**: Öffnet einen zugehörigen Dialog.
*   **Abbrechen**: Schließt den Dialog ohne Änderungen zu speichern.
*   **Ändern**: Ermöglicht das Bearbeiten eines markierten Datensatzes.
*   **Aktualisieren**: Lädt den Inhalt des geöffneten Dialogs neu.
*   **BDE-Anzeige**: Öffnet den Dialog BDE-Anzeige.
*   **Datenübernahme**: Startet die Datenübernahme in A+W Production.
*   **Drucken**: Öffnet einen Dialog für Druckeinstellungen.
*   **Einfügen**: Fügt einen kopierten Datensatz ein.
*   **Filtern**: Ermöglicht das Erstellen neuer Filter in den Anzeigen.
*   **Kopieren**: Kopiert einen markierten Datensatz in die Zwischenablage.
*   **Lauf-Anzeige**: Öffnet den Dialog Lauf-Anzeige.
*   **Löschen**: Löscht den markierten Datensatz.
    > **Löschen**: Das Löschen erfolgt teilweise ohne Rückfrage des Systems. Mit [Abbrechen] schließen Sie den Dialog, das Löschen wird nicht ausgeführt. Bestätigen Sie den Dialog jedoch mit [OK], wird die Auswahl unwiderruflich gelöscht!
*   **Manuelle Nachbearbeitung**: Öffnet den Dialog Manuelle Nachbearbeitung.
*   **Neu**: Erfasst einen neuen Datensatz.
*   **OK**: Übernimmt alle vorgenommenen Eingaben, speichert sie und schließt den Dialog.
*   **Hilfe (?)**: Öffnet das Online-Hilfesystem.
*   **Packmittelgruppen-Anzeige**: Öffnet den Dialog Packmittelgruppen-Anzeige.
*   **Pool-Anzeige**: Öffnet den Dialog Pool-Anzeige.
*   **Schließen**: Schließt den Dialog.
*   **Speichern**: Übernimmt Eingaben in die Datenbank.
*   **Suchen**: Öffnet den Dialog Suchen.
*   **Topf-Anzeige**: Öffnet den Dialog Topf-Anzeige.
*   **Verwerfen**: Verwirft alle vorgenommenen Eingaben (nicht speichern).

### Dokumentation

#### Aufbau des Handbuchs

Die Dokumentation ist in Parts unterteilt (A-Z). Der erste Part ist grundsätzlich der Part Überblick (A). Die letzten Parts sind Index (Y) und Glossar (Z). Die dazwischen liegenden Parts stehen jeweils für die unterschiedlichen Themenbereiche.

| Part | Inhalt |
| :--- | :--- |
| **A Überblick** | Vermittelt einen Überblick zum Aufbau des Handbuchs und erläutert Softwarebegriffe. |
| **C Grobplanung** | Erläutert Einstellungen und Durchführung der Grobplanung. |
| **D Feinplanung** | Beschreibt die notwendigen Einstellungen für die Produktion und die Feinplanung. |
| **E Kapazitaetsplanung** | Erläutert die Arbeitsweise und Einstellungen der Kapazitätsplanung. |
| **F Formeleditor** | Beschreibt, wie mit dem Formeleditor Bedingungen erstellt werden. |
| **G Maschinenzuordnung** | Erläutert die Arbeitsweise und Einstellungen der Maschinenzuordnung. |
| **H Barcode Manager** | Bietet Informationen zur Betriebsdatenerfassung (BDE). |
| **I Packmitteloptimierung** | Erläutert die Arbeitsweise und Einstellungen der Packmitteloptimierung. |
| **J A+W Realtime Optimizer** | Beschreibt die Nutzung des Moduls XOPT-ON zur Optimierung des Zuschnitts. |
| **L A+W Production Terminal** | Beschreibt die Nutzung der Leitrechner-Technologie. |

#### Online-Hilfe

Die A+W Production Online-Hilfe kann auf unterschiedliche Weise geöffnet werden:
*   Menü **Hilfe**
*   Schaltfläche **[Hilfe]**
*   Taste **<F1>**

Die Online-Hilfe wird zu den meisten Dialogen kontext-sensitiv geöffnet.

*   **Hilfethemen**: Die Hilfe ist in Themen strukturiert, die über eine Baumansicht zugänglich sind.
*   **Blättern**: Mit den Pfeilschaltflächen kann zum nächsten/vorherigen Thema geblättert werden.
*   **Register Inhalt**: Zeigt die Module/Kataloge in Form von Büchern an.
*   **Register Index**: Ermöglicht die Suche nach Hauptthemen.
*   **Register Suchen**: Ermöglicht eine Volltextsuche.
*   **Hilfetext nicht gefunden**: Wenn kein kontextspezifisches Thema existiert, wird die Startseite der Hilfe angezeigt.
