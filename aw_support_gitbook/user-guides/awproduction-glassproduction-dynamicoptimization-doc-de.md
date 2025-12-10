---
title: "DE_AWProduction_DynOpt_1.00"
source: "DE_AWProduction_DynOpt_1.00.pdf"
tags: ["A+W DynOpt", "Glass Production", "Dynamic Optimization", "Production Planning", "Software Tutorial", "ERP", "Cutting Optimization", "German"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A German-language tutorial for A+W DynOpt, a software module for dynamic optimization in glass production. The document explains the concept, problem statement, and practical application of the software, including how to manage production runs, handle exceptions like broken lites, and use the A+W DynOpt Editor for process control."
long_description: "This document is a comprehensive tutorial for A+W DynOpt, a software solution designed for the dynamic optimization of production processes in the glass, window, and door industries. Written in German, it targets production planners and supervisors responsible for optimizing workflow. The tutorial begins with an overview of dynamic optimization, contrasting it with standard methods and highlighting its benefits in handling smaller batch sizes and increased product variety. It details the system's components, including the A+W Realtime Optimizer and its integration with cutting tables, buffer systems, and the A+W Production Cockpit. The guide explains key concepts like the 'dynamic timeline,' buffer management, and handling of remnants and broken lites. A significant portion is dedicated to practical instructions on using the A+W DynOpt Editor to import, prioritize, and manage production runs, including a step-by-step guide for prioritizing rush orders. The document aims to empower users to leverage A+W DynOpt for improved material yield, increased flexibility, and a more efficient production flow."
---

# A+W DynOpt

**A+W - Software for Glass, Windows and Doors**

---

---
## Vorspann N

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Version / Datum | Beschreibung |
| :--- | :--- |
| 1.00 / 03-2016 | Ersterstellung |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen
- Kontakte

#### Anmerkungen zu diesem Dokument
Diese Veröffentlichung ist ausschließlich für Endanwender von *A+W DynOpt* gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.

Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von *A+W Production*.

#### Urheberrechte
© 2016, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen
Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

### Kontakte
**A+W Software GmbH**

Am Pfahlgraben 4 - 10
D-35415 Pohlheim
Germany

📞 +49 6404 2051 0
📠 +49 6404 2051 877
📧 Zentrale@a-w.com
🌐 http://www.a-w.com

---

## Inhalt

- **Vorspann** (N-3)
  - Revisionsübersicht (N-3)
  - Editorial (N-3)
- **Tutorial** (J-7)
  - Überblick (J-9)
  - Dynamische Optimierung (J-10)
    - Leistungsbeschreibung (J-11)
    - Problemstellung (J-14)
    - Optimierung mit A+W DynOpt (J-17)
    - Dynamischer Zeitstrahl (J-19)
    - Puffersystem (J-21)
    - Pufferbelegung (J-22)
    - Zusammenarbeit mit Panorama (J-23)
  - Mit A+W DynOpt arbeiten (J-25)
    - A+W DynOpt Editor (J-27)
    - Eilscheiben in zwei Schritten priorisieren (J-29)
    - A+W DynOpt Editor bedienen (J-33)
- **Partindex** (N-35)
  - Index (N-37)

---

## Tutorial J

### Überblick

In diesem Dokument finden Sie Informationen zum Konzept der dynamischen Optimierung. Daran schließend finden Sie Informationen zu den manuellen Eingriffen, mit Sie die Optimierung starten und bearbeiten.

In diesem Tutorial finden Sie folgende Informationen:
- "Dynamische Optimierung" auf Seite J-10
- "Mit A+W DynOpt arbeiten" auf Seite J-25

#### Vorausgesetzte Kenntnisse
Das Tutorial richtet sich an Teilnehmer, die in *A+W Production* die Arbeitsvorbereitung verantworten und damit den optimalen Ablauf der Produktion organisieren. Die Teilnehmer müssen das Konzept der Stammdaten und Einlastung in *A+W Production* kennen.

#### Darstellungskonventionen
Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

- *Kursiv*: sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Kampagnenplanung*.
- **Fett**: sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: Geben Sie den Wert **0** ein.
- **>**: Mit dem sogenannten Brotkrumenpfad ist der Weg gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B. *Stammdaten > Kapazitätsplanung > Kampagnenplanung > Kampagne hinzufügen*.
- **[]**: Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit [OK] speichern Sie die Daten.
- **<>**: Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit <F1> öffnen Sie die Online-Hilfe.

#### Lesehinweis
Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.

### Dynamische Optimierung

Das Tutorial zum Modul *A+W DynOpt* beschäftigt sich mit der Optimierung des Produktionsablaufs von der Planung der Lose bis zum fertigen Produkt.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Leistungsbeschreibung" auf Seite J-11
- "Problemstellung" auf Seite J-14
- "Optimierung mit A+W DynOpt" auf Seite J-17
- "Zusammenarbeit mit Panorama" auf Seite J-23

#### Leistungsbeschreibung
Ein wesentliches Einsparpotential bei der Flachglasverarbeitung ist die optimale Ausnutzung der Lagerplatten beim Zuschnitt.
- Mit dem innovativen Optimierungsalgorithmus und der intelligenten und modernen Maschinen- und Lageranbindung ist es möglich, alternierend verschiedene Glasarten aufzulegen und zu schneiden.
- Mit dem Einsatz eines Zwischenpuffers kann dynamisch optimiert, geschnitten und in den Zwischenpuffer einsortiert werden.
- Die Ansteuerung von Schneidtischen mit den optimierten Schnittbildern direkt aus der Optimierung beschleunigt zudem den Arbeitsprozess.

*A+W DynOpt* ist ein komplexer Systemverbund aus verschiedenen Hardware- und Softwarekomponenten:
- Schneidtisch(e)
- Lager- und Restplattenlager
- Zwischenpuffer und Sortiersystem
- *A+W Production* zur Arbeitsvorbereitung
- *A+W Realtime Optimizer* zur Online-Optimierung am Tisch
- Panorama und Produktionsansicht in *A+W Production Cockpit* zur Gesamtsteuerung und Visualisierung des Systems.

