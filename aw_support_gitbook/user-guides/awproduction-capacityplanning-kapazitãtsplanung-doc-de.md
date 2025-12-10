---
title: "DE_AWProduction_Kapazitaetsplanung_4_1"
source: "DE_AWProduction_Kapazitaetsplanung_4_1.pdf"
tags: ["A+W Production", "Capacity Planning", "Kapazitätsplanung", "ERP Software", "Glass Manufacturing", "Window Manufacturing", "Production Scheduling", "Software Manual", "Tutorial", "German"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a user manual for the A+W Production Capacity Planning (Kapazitätsplanung) module, version 4.50. It serves as a guide for planning production processes and optimizing the use of machinery capacity in the glass, window, and door manufacturing industry. The manual is provided in German."
long_description: "This comprehensive manual details the functionality of the A+W Production Capacity Planning (Kapazitätsplanung) module. It is intended for end-users, production planners, and administrators responsible for organizing the optimal flow of production. The document is divided into several key sections. The 'Vorspann' (Preface) includes revision history, editorial notes, copyright information, and contact details. The 'Tutorial' section provides a step-by-step guide to using the module, covering fundamentals like appointment optimization and scheduling, as well as practical applications such as using the production monitor, handling loading and rescheduling, campaign planning for specific jobs, and managing capacity reservations. It also explains how to set up the master data for capacity planning, including shifts, cost calculations, and transition times. The 'Softwarereferenz' (Software Reference), outlined in the table of contents, offers a detailed reference for all software features, dialogs, and settings, including the production monitor, scheduling functions, campaign and reservation management, and master data configuration for times, shifts, machines, and costs. The document emphasizes practical use with examples, screenshots, and step-by-step instructions to ensure users can effectively manage production deadlines, utilize machinery efficiently, and respond flexibly to unforeseen events."
---

# A+W Kapazitätsplanung

**A+W Production**

*A+W - Software for Glass, Windows and Doors*

---

---
## Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version / Datum | Beschreibung |
| :--- | :--- |
| 4.50 / 01-2023 | Arbeitsplan exportieren hinzugefügt. |
| 4.00 / 11-2017 | Vollständige Überarbeitung. |
| 3.01 / 01-2017 | Produkt- und Firmennamen angepasst. |
| 3.00 / 08-2013 | Ersterstellung des Tutorials und vollständige Überarbeitung der Softwarereferenz. |
| 2.00 / 04-2008 | Überarbeitung. |
| 1.20 / 11-2007 | Namensänderung (AWCapacity/Kapazitätsplanung). |
| 1.10 / 2007 | Änderung Kapitel Arbeitsplan. |
| 1.00 / 2007 | Ersterstellung |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
*   Anmerkungen zu diesem Dokument
*   Urheberrechte
*   Warenzeichen
*   Kontakte

#### Anmerkungen zu diesem Dokument
Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Production gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Dieses Dokument beschreibt die volle Ausbaustufe der Stammdaten.

#### Urheberrechte
© 2023, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

#### Warenzeichen
Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

#### Kontakte
**A+W Software GmbH**
Am Pfahlgraben 4-10
D-35415 Pohlheim
*   Tel: +49 6404 2051-0
*   Fax: +49 6404 2051-877
*   Email: aw.zentrale@a-w.com
*   Web: http://www.a-w.com

---

## Inhalt

*   **Vorspann**
    *   Revisionsübersicht
    *   Editorial
*   **Inhalt**
*   **Tutorial**
    *   Überblick
        *   Dokumentation
        *   Aufbau des Tutorials
        *   Darstellungskonventionen
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
*   **Softwarereferenz**
    *   Überblick
    *   Produktionsmonitor
        *   Einlastung
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
            *   Arbeitsplan – Details
            *   Arbeitsplan – Übersicht
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
            *   Kampagnen – Einzeltermine
            *   Kampagnen – Wöchentliche Termine
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
*   **Partindex**

---

## Tutorial

### Überblick

Das Tutorial zum Modul *Kapazitätsplanung* beschäftigt sich mit der Planung Ihres Produktionsablaufs und der optimalen Nutzung der Kapazität Ihres Maschinenparks. Ziele der Kapazitätsplanung sind die Liefertermine einzuhalten, den Maschinenpark effizient zu nutzen und flexibel auf unvorhersehbare Ereignisse reagieren zu können. Eine optimale Kapazitätsplanung stellt immer einen Kompromiss zwischen größtmöglicher Effizienz und größtmöglicher Flexibilität dar.

In diesem Tutorial ist beschrieben, wie Sie manuell in die Planung eingreifen können und wie die Stammdaten für die Kapazitätsplanung eingerichtet werden.

Das Tutorial umfasst folgende Themenblöcke:
*   "Grundlagen" auf Seite E-14
*   "Planung und Einlastung" auf Seite E-21
*   "Stammdaten der Kapazitätsplanung" auf Seite E-68

#### Vorausgesetzte Kenntnisse
Das Tutorial richtet sich an Mitarbeiter, die in *A+W Production* die Arbeitsvorbereitung verantworten und damit den optimalen Ablauf der Produktion organisieren. Die Mitarbeiter müssen die Maschinenzuordnung (MZO) und das Konzept der Stammdaten in *A+W Production* kennen. Außerdem sind Kenntnisse der Grob- und Feinplanung hilfreich.

> **Stammdaten vor Zugriff schützen**
> Die Stammdaten von *A+W Production* und insbesondere von *A+W Capacity Planner* sind hochsensible Daten. Unkontrollierte oder unbeabsichtigte Eingriffe und Änderungen können die gesamte Produktion stilllegen. Richten Sie daher die jeweiligen Arbeitsplätze so ein, dass nur die Administratoren oder Mitarbeiter mit entsprechenden Funktionen Zugriff auf die Stammdaten haben.

> **Datensicherung**
> Erstellen Sie eine vollständige Datensicherung der Stammdaten bevor Sie mit der Bearbeitung der Stammdaten beginnen. Das Backup-Tool finden Sie unter:
> `C:\Programme (x86)\A+W\Techsoft\Tools\AWSplicer\AWSplicer.exe`.
> Verschieben Sie das gespeicherte Backup aus Ihrem User-Verzeichnis in ein Verzeichnis, auf das auch der Support Zugriff hat.
> Besprechen Sie die anstehenden Änderungen vorab mit Ihrem Projektierer bei der A+W Software GmbH.

### Dokumentation

Für das Modul *Kapazitätsplanung* stehen folgende Dokumente zur Verfügung:

| Format | Umfang |
| :--- | :--- |
| PDF | Vollständige Unterlagen<br>• Tutorial<br>• Softwarereferenz<br>• Index |
| Online-Hilfe `<F1>` | Dialog-Hilfe |

### Aufbau des Tutorials
Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

**Überblick**
Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
*   Lernziele: Was soll vermittelt werden?
*   Nutzen: Wofür können Sie dieses Wissen einsetzen?
*   Merksätze: Welche Zusammenhänge müssen Sie sich merken?

**Konzepte**
Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.

**Übungen**
Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen.

### Darstellungskonventionen

Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

| Begriff | Bedeutung |
| :--- | :--- |
| *Kursiv* | sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Kampagnenplanung*. |
| **Fett** | sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: Geben Sie den Wert **0** ein. |
| `>` | Mit dem sogenannten Brotkrumenpfad ist der Weg gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B. *Stammdaten > Kapazitätsplanung > Kampagnenplanung > Kampagne hinzufügen*. |
| `[]` | Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit `[OK]` speichern Sie die Daten. |
| `< >` | Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit `<F1>` öffnen Sie die Online-Hilfe. |

#### Lesehinweis
Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.

Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

## Grundlagen

*A+W Capacity Planner* ist so ausgelegt, dass auch für Produkte mit ungewöhnlich tiefen Stücklisten meist gleich mehrere sichere Pfade von der Starttechnologie bis zum Versand gefunden werden. Die Kapazitätsplanung greift dazu auf die Arbeitsgänge zu, die die Scheiben vom Zuschnitt bis zur Auslieferung durchlaufen.

### Stammdaten der Maschinenzuordnung
Die Maschinenzuordnung (MZO) stellt die Verbindung zwischen Arbeitsgängen und Maschinen dar und bildet die Bewertung nach Vorzugsmaschinen ab. Damit für die zu fertigenden Scheiben gültige Maschinen gefunden werden, müssen die Maschinen präzise beschrieben sein. In der Maschinenzuordnung wird dazu zwischen physikalischen Restriktionen und logischen Maschinen mit zusätzlichen Restriktionen, Kostensätzen und Übergangszeiten unterschieden.

Da die Schritte zum Einrichten der Kapazitätsplanung auf den logischen Maschinen beruhen, muss der Maschinenpark vollständig beschrieben sein. Die Informationen dazu finden Sie im Part *Maschinenzuordnung*.

### Stammdaten der Kapazitätsplanung
Für die Terminbestimmung werden Schichtpläne, Übergangszeiten und Zeiten für die Bearbeitungsdauer benötigt.

*   Damit sich zum Test der Daten ein einfaches Bild für die Auslastung ergibt, empfiehlt es sich, die Bearbeitungsdauern pauschal in Sekunde pro Stück anzugeben, z. B. 1 - 5 Minuten pro Scheibe je nach Maschine.
*   Für die Übergangszeiten soll der optimale und realistische Produktionsdurchlauf beschrieben werden.
    Die Angabe der Zeiten in ganzen Schichten sorgt für eine einfache und vorhersagbare Terminbestimmung. An Maschinen, die auch unbeaufsichtigt arbeiten können, kann die Übergangszeit (Verweildauer) in Stunden angegeben werden, z. B. Heatsoak, Autoklav oder Aushärten von Silikonversiegelungen. Achten Sie bei den Übergängen darauf, dass Sie im Betrieb den Platz benötigen, um die Glasmenge einer Schicht abzustellen.
*   Aus den Zeiten für die Bearbeitungsdauer können die Engpässe für die Einlastung bestimmt werden.

### Einlastungsregeln
Die Einlastungsregeln werden als Konfigurationsparameter für *A+W Capacity Planner* festgelegt. Sie beeinflussen das Programmverhalten, die Meldungskultur und die möglichen Benutzerreaktionen. Dies betrifft z. B.:
*   Dürfen Liefertermine verschoben werden.
*   Wann ist der früheste Produktionsbeginn für einen eingelasteten Auftrag.
*   Wie werden Angebote eingelastet und müssen sie wieder storniert werden.
*   Wie werden Eilaufträge durchgeschleust.
*   Ab welcher Stückzahl müssen Positionen gesplittet werden.

### Terminoptimierung

Die Terminoptimierung beginnt mit dem letzten Betriebsmittel am oder vor dem Liefertermin: dem Verladen. Mit Blick auf den Produktionsmonitor kann die Terminoptimierung wie folgt dargestellt werden.

