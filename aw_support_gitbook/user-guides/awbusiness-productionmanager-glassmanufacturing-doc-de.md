---
title: "DE_AWBusiness_ProductionManager_2.21"
source: "DE_AWBusiness_ProductionManager_2.21.pdf"
tags: ["A+W Business Pro", "Production Manager", "Software Manual", "Glass Manufacturing", "Window Production", "ERP", "MES", "Tutorial", "Software Reference", "German"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a comprehensive German-language user manual for the A+W Business Pro Production Manager software, version 2.21. It serves as a guide for end-users in the glass, window, and door manufacturing industries. The manual is divided into a tutorial, master data management, and a detailed software reference section, covering both standard and expert modes of operation."
long_description: "This is the official user manual for the A+W Business Pro Production Manager software, version 2.21, as of January 2017. The document is intended for end-users and provides a complete guide to managing production planning and execution within the A+W software ecosystem for glass, window, and door manufacturers. The manual begins with a preface (Vorspann) containing a revision history, copyright information, and contact details for A+W Software GmbH. The core of the document is split into two main parts: a Tutorial and a Software Reference. The Tutorial section introduces the fundamental concepts of the Production Manager, explains the user interface, and provides step-by-step guidance on using both the simplified 'Standardmodus' (Wizard) and the detailed 'Expertenmodus'. It covers key processes such as creating production runs (Laufbildung), fine-tuning, optimization, managing breakages, and generating outputs like reports and cutting codes. The Stammdaten (Master Data) section explains how to configure essential data such as storage locations (Abstellplätze), criteria, and sorting keys, which are foundational for the production process. The Softwarereferenz section offers an in-depth reference for every dialog, field, and function within the software, providing detailed explanations for both standard and expert modes, including order selection, run management, optimization, and output settings. The manual concludes with an index for quick reference."
---

# A+W Produktionsmanager

---
## A+W Business Pro
A+W - Software for Glass, Windows and Doors

---

## Vorspann
In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version/Datum | Beschreibung |
| :--- | :--- |
| 1.00/07-2013 | Ersterstellung. |
| 2.00/07-2014 | Anpassung: Layout, Struktur und Texte der Help Cards. |
| 2.10/02-2015 | Überarbeitung. |
| 2.20/04-2016 | Bruchscheiben ergänzt. |
| 2.21/01-2017 | Produkt- und Firmennamen angepasst. |

### Editorial
Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen
- Kontakte

#### Anmerkungen zu diesem Dokument
Diese Veröffentlichung ist ausschließlich für Endanwender von *A+W Business Pro* gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Dieses Dokument beschreibt die volle Ausbaustufe der Stammdaten.

### Urheberrechte
© 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen
Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

### Kontakte
**A+W Software GmbH**

Am Pfahlgraben 4 - 10
D-35415 Pohlheim
Germany

📞 +49 6404 2051 0
📠 +6404 2051 877
Zentrale@a-w.com
http://www.a-w.com

---

## Tutorial
A+W Business Pro

### Überblick

> **i**
>
> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
>
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

Das Tutorial zum Modul *Produktionsmanager* beschäftigt sich mit den Grundlagen der Produktionslösung in *A+W Business Pro*. Das Tutorial baut auf den Kenntnissen zu den Stammdaten und zum Nummernverwalter auf.

#### Themenblöcke
In diesem Tutorial finden Sie folgende Themenblöcke:
- Grundgedanken zum Produktionsmanager
- Standardmodus
- Expertenmodus

#### Vorausgesetzte Kenntnisse
Das Tutorial richtet sich an Teilnehmer, die in *A+W Business Pro* Aufträge zur Produktion vorbereiten. Die Teilnehmer müssen das Konzept der Stammdaten und des Nummernverwalters kennen.

### Dokumentation
Für das Modul *Production Manager* stehen folgende Dokumente zur Verfügung:

| Typ | Inhalt |
| :--- | :--- |
| **Handout** | Ausdruck des Tutorials für die Schulung |
| **PDF** | Vollständige Unterlagen<br>- Tutorial<br>- Softwarereferenz<br>- Index |
| **Online-Hilfe `<F1>`** | Kontextsensitive Dialog-Hilfe der A+W Business-Softwarereferenzen und Tutorials der Basisversion |

#### Aufbau des Tutorials
Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

- **Überblick**
  Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
  - Lernziele: Was soll vermittelt werden?
  - Nutzen: Wofür können Sie dieses Wissen einsetzen?
  - Merksätze: Welche Zusammenhänge müssen Sie sich merken?

- **Konzepte**
  Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.

- **Übungen**
  Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen und Lösungsvorschlägen.

- **Querverweise**
  Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf ergänzende Informationen in der Softwarereferenz und in anderen Parts hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.

#### Lesehinweis
Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.

Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

### Darstellungskonventionen
Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

| Stil | Bedeutung |
| :--- | :--- |
| *Kursiv* | sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Nummernverwalter*. |
| **Fett** | sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: Geben Sie den Wert **0** ein. |
| > | Mit dem sogenannten Brotkrumenpfad ist der Weg kennzeichnet, auf dem Sie einen Dialog öffnen, z. B. *Fertigung > Produktion > Produktionsübergabe*. |
| [ ] | Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit [OK] speichern Sie die Daten. |
| `< >` | Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit `<F1>` öffnen Sie die Online-Hilfe. |

### Grundgedanken zum Produktionsmanager
Aufgabe des Produktionsmanageres ist es, Sie im Planungs- und Vorbereitungsprozess für die Produktion zu unterstützen - von der Laufbildung bis hin zum Druck von Produktionspapieren und dem Erzeugen vom Maschinencode.

Der Prozessablauf stellt sich wie folgt dar:
