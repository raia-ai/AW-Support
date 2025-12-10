---
title: "DE_AWProduction_Grobplanung_2.50"
source: "DE_AWProduction_Grobplanung_2.50.pdf"
tags: ["A+W Production", "Grobplanung", "Rough Planning", "Glass Manufacturing", "Window Manufacturing", "Production Planning", "ERP Software", "User Manual", "Software Tutorial", "Software Reference"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a user manual for the 'Grobplanung' (Rough Planning) module of the A+W Production software, version 2.50. It provides a comprehensive tutorial and software reference for production planners in the glass, window, and door manufacturing industries. The guide covers key processes such as creating and managing orders, views, runs (Läufe), and pots (Töpfe) to optimize production workflows."
long_description: "This is a detailed guide for end-users of A+W Production's 'Grobplanung' (Rough Planning) module. The document is split into two main parts: a Tutorial and a Software Reference. The Tutorial section is designed for production preparation managers and offers a step-by-step introduction to the core concepts of rough planning. It explains how to configure views, manage orders from the ERP system in the 'Pool,' group them into 'Pots' (Töpfe) for intermediate storage, and finally combine them into 'Runs' (Läufe) for optimized production. It details various strategies for creating runs based on criteria like glass type, product type, or production date. The Software Reference section provides an in-depth explanation of every dialog, field, context menu, and function within the Grobplanung module. It serves as a comprehensive resource for understanding the specifics of dialogs such as Orders (Aufträge), Runs (Läufe), Positions (Positionen), Operations (Bearbeitungen), and more. The document emphasizes the configuration of views (Ansichten) with custom columns, summaries, and filters to provide users with the exact information they need to make informed planning decisions. It is essential for users responsible for organizing and optimizing the production flow from order entry to final production release."
---

# A+W Grobplanung E

**A+W Production**

A+W - Software for Glass, Windows and Doors

---

---
## Revisionsübersicht

| Part Version / Datum | Beschreibung |
| :--- | :--- |
| 2.50/01-2023 | Vorgang suchen ergänzt. |
| 2.01/01-2017 | Produkt- und Firmennamen angepasst. |
| 2.00/07-2014 | Neuerstellung Tutorial und Softwarereferenz. |
| 1.50/08-2013 | Vollständige Überarbeitung der ALCIM-Dokumentation und Anpassung auf A+W Production. |
| 1.00/03-2006 | Ersterstellung. |

## Editorial

Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen

### Anmerkungen zu diesem Dokument
Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Production gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.

Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von A+W Production.

### Urheberrechte
© 2023, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen
Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

# Tutorial

**A+W Production**

A+W - Software for Glass, Windows and Doors

## Überblick

Das Tutorial zum Prozess der Grobplanung beschäftigt sich mit der Lauf-Bildung in A+W Production. Die Verantwortlichen aus der Arbeitsvorbereitung verschaffen sich in der Grobplanung mit verschiedenen Ansichten einen Überblick und bilden mit verschiedenen Strategien Läufe, die eine optimale Produktion ermöglichen.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

### Vorausgesetzte Kenntnisse
Das Tutorial richtet sich an Teilnehmer, die in A+W Production die Arbeitsvorbereitung verantworten und damit den optimalen Ablauf der Produktion organisieren. Die Teilnehmer müssen das Konzept der Stammdaten in A+W Production kennen.

## Dokumentation

Für das Modul *Grobplanung* stehen folgende Dokumente zur Verfügung:

| Typ | Inhalt |
| :--- | :--- |
| **Handout** | Ausdruck des Tutorials für die Schulung |
| **PDF** | Vollständige Unterlagen<ul><li>Tutorial</li><li>Softwarereferenz</li><li>Index</li></ul> |
| **Online-Hilfe <F1>** | Kontextsensitive Dialog-Hilfe |

### Aufbau des Tutorials
Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

- **Überblick**
  Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
  - Lernziele: Was soll vermittelt werden?
  - Nutzen: Wofür können Sie dieses Wissen einsetzen?
  - Merksätze: Welche Zusammenhänge müssen Sie sich merken?
- **Konzepte**
  Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.
- **Übungen**
  Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen.
- **Querverweise**
  Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf ergänzende Informationen in der Softwarereferenz und in anderen Parts hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.

### Darstellungskonventionen
Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

- ***Kursiv***: sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Töpfe*.
- **Fett**: sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: **Geben Sie den Wert 0 ein.**
- **`>`**: Mit dem sogenannten Brotkrumenpfad ist der Weg kennzeichnet, auf dem Sie einen Dialog öffnen, z. B. *Anzeigen > Füllaufträge > Kontextmenü - Liste > Auftragsübersicht*.
- **`[]`**: Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit `[OK]` speichern Sie die Daten.
- **`<>`**: Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit `<F1>` öffnen Sie die Online-Hilfe.

### Lesehinweis
Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.
Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

## Grobplanung

In diesem Tutorial erfahren Sie, welche Bereiche von A+W Production zur Grobplanung gehören und wie Sie die Grobplanung durchführen.
Mit verschiedenen Ansichten (Ansichts-Dialoge) verschaffen Sie sich einen Überblick und wenden Strategien zur Lauf-Bildung an.

### Prozess der Arbeitsvorbereitung

