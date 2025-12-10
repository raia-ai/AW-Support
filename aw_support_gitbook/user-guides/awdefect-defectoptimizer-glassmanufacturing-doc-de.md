---
title: "DE-AWDefect_Optimizer_Kurzbeschreibung"
source: "DE-AWDefect_Optimizer_Kurzbeschreibung.pdf"
tags: ["A+W Software", "Defect Optimizer", "Glass Manufacturing", "Window Production", "ERP", "Cutting Optimization", "Quality Control", "Viprotron", "Hegla", "German"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A short product description in German for the A+W Defect Optimizer software. This software integrates with glass cutting lines to detect and optimize around defects in jumbo glass sheets, reducing waste and improving quality."
long_description: "This document is a short description ('Kurzbeschreibung') in German for the A+W Defect Optimizer, a software solution for the glass, window, and door manufacturing industry. It details how the software works in conjunction with quality scanners (like Viprotron) and cutting lines (like Hegla) to identify defects on jumbo glass plates before the cutting process begins. The software then re-optimizes the cutting pattern in real-time to avoid these defects, either by repositioning the required glass panes or by placing smaller, less costly panes over the defective areas. The manual outlines the process flow from defect detection to re-optimization, explains the benefits such as cost reduction and quality improvement, and details system prerequisites. It serves as an introductory guide for end-users to understand the functionality and value of the A+W Defect Optimizer."
---

# A+W Defect Optimizer Kurzbeschreibung

---
## Editorial

### Revisionsübersicht der Dokumentation

| Datum | Erstellung |
| :--- | :--- |
| 10-2014 | Ersterstellung. |

### Anmerkungen

Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Defect Optimizer gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.

Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von A+W Defect Optimizer.

### Urheberrechte

© 2014, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

## Darstellungskonventionen

Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

| Stil | Bedeutung |
| :--- | :--- |
| *Kursiv* | sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Preiseigenschaften*. |
| **Fett** | sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: Geben Sie den Wert **5** ein. |
| > | Mit dem sogenannten Brotkrumenpfad ist der Weg gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B. *Stammdaten > Preise > ISO-Preise*. |
| [] | Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit [OK] speichern Sie die Daten. |
| < > | Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit <F1> öffnen Sie die Online-Hilfe. |

## Kontakt

**A+W Software GmbH**
Siemensstr. 3
D-35463 Fernwald
Deutschland

**Tel.:** +49 641 96620 0
**E-Mail:** info@a-w.com
**Web:** http://www.a-w.com

## Inhalt

- Tutorial
- A+W Defect Optimizer stellt sich vor
- Intelligente Fehlerstellenoptimierung
    - Ihr Nutzen
- Prozessablauf
    - Erkennung der Fehlerstellen
    - Verarbeitung der Fehlerstellen
    - Die Online-Analyse

## Tutorial

In diesem Kapitel finden Sie folgende Themen:
- A+W Defect Optimizer stellt sich vor
- Intelligente Fehlerstellenoptimierung
- Prozessablauf

### A+W Defect Optimizer stellt sich vor

Statistisch hat jede zweite Jumbo-Scheibe einen Defekt. Allerdings werden Einschlüsse und Fehler auf Lager- und Restplatten häufig erst sehr spät bzw. zu spät erkannt - bspw. bei der Qualitätskontrolle vor bzw. nach dem Iso-Zusammenbau oder im schlimmsten Fall erst beim Kunden.

In diesem Fällen hatten Sie bereits erhebliche Kosten mit der Produktion (und dem Versand) der Scheibe. Und nun investieren Sie erneut um eine Scheibe nach zu produzieren und ggf. neu an den Kunden zu versenden.

Warum die Fehler nicht schon vor dem Zuschnitt erkennen und in der Optimierung berücksichtigen?

#### Voraussetzungen für den Einsatz des A+W Defect Optimizer

Um den A+W Defect Optimizer in Ihrem Hause einsetzen zu können, sind folgende Voraussetzungen nötig:

- Der A+W Realtime Optimizer (online Zuschnitt-Leitrechner) ab Version 12.3 muss vorhanden und installiert sein.
- Ein Inspektionssystem, das die entsprechenden Daten verlässlich meldet, wenn die Lagerplatte in die Maschine läuft (z. B. Qualtiätsscanner von Viprotron).

### Intelligente Fehlerstellenoptimierung

In Verbindung mit z. B. einem Qualitätsscanner der Firma Viprotron werden die Lagerplatten gescannt und etwaige Fehler bzw. Fehlerstellen (Defekte) noch vor dem Beginn des Zuschnitts erkannt und visualisiert. Je früher die Fehlerstellen im Prozess erkannt werden, um so geringer sind die anfallenden Kosten.

Die Fehlerstellen werden in der Optimierung für die Neu- und Restrukturierung des Schnittbildes berücksichtigt. Gibt es einzuhaltende Reihenfolgen, werden diese selbstverständlich berücksichtigt.
Selbst auf Restplatten werden die Fehlerstellen gespeichert und können so später ohne erneute Kontrolle wiederverwendet werden.

Lassen sich Defekte durch die Optimierung nicht vermeiden (z. B. Anzahl und Größe der Scheiben auf dem Muster), so versucht die Optimierung kleine und somit kostengünstigere Gläser auf die Defekte zu legen.

Gläser, die auf Defekten liegen, werden automatisch als Bruch gemeldet und nachgeschnitten.

#### Ihr Nutzen

... durch den Einsatz des A+W Defect Optimizer lässt sich zusammenfassen in:

- Qualitätssteigerung durch Fehlervermeidung
- Deutliche Kostensenkung durch Früherkennung der Fehlerstellen vor dem Zuschnittprozess und Restrukturierung des Optimierungsprozesses (mittels A+W Realtime Optimizer und z. B. Viprotron Qualitätsscannern)
- Vermeidung von Bearbeitungen auf bereits fehlerhaften Scheiben
- Auswahl von geeigneten Lieferanten durch Qualitätskontrollen
- Steigerung der Liefertermin-Treue

### Prozessablauf

Nachfolgend erhalten Sie einen Überblick zum Prozessablauf. In unserem Beispiel kommen folgende Komponenten zum Einsatz:

- Aufleger der Firma Hegla (Compact Loader)
- Automatische Schneidanlage der Firma Hegla (Optimax)
- Jumbo Controller der Firma Viprotron
- A+W Realtime Optimizer
- A+W Defect Optimizer

#### Erkennung der Fehlerstellen

Im ersten Schritt werden die von der Optimierung ermittelten Schneidcodes an den Zuschnitttisch gesendet.

*Abb. A-1: Schneidcode wird an den Zuschnitttisch gesendet*

Anschließend kommt vom Zuschnitttisch die entsprechende Platten-Anforderung an das Lager.

*Abb. A-2: Lagerplatten werden angefordert*

Die erste Lagerplatte wird aufgelegt und fährt durch den Jumbo Controller.

*Abb. A-3: Erkennung von Fehlerstellen*

Der Jumbo Controller findet die Fehlerstellen und meldet die entsprechenden Koordinaten an den A+W Defect Optimizer.

*Abb. A-4*

Aufgrund der zurückgemeldeten Daten erstellt der A+W Realtime Optimizer den neuen Schneidcode und übermittelt diesen an den Zuschnitttisch.

### Verarbeitung der Fehlerstellen

Vorhandene Fehlerstellen werden Ihnen wie folgt angezeigt:

*Abb. 2: Fehlerstellen auf dem Schneidmuster*

Nach der erneuten Optimierung durch den A+W Defect Optimizer sieht das Schneidmuster wie folgt aus:

*Abb. 3: Neues Schneidmuster*

### Die Online-Analyse

> **Rote Kreise um die Fehlerstellen**
> Die roten Kreise um die Fehlerstellen sollen diese nur deutlich machen, sie sind zur Laufzeit nicht vorhanden!

Der A+W Defect Optimizer analysiert die Daten der Inspektion für jede einzelne Lagerplatte während des Transports und Ausrichtens der Tafel am Schneidtisch.

*Abb. 4: Fehlerstellen*

Das System erkennt automatisch die betroffenen Scheiben und markiert diese entsprechend in der Brechbildanzeige:

*Abb. 5: Brechbildanzeige*

### Fehlerklassen

Die Fehler werden nach Größe und Typ in zwei Klassen unterteilt. In der einen Klasse befinden sich die Fehler, die auf dem Scheibenrand sind. Diese Fehler werden toleriert, die Scheibe wird nicht als Bruch markiert.
Die anderen Fehler liegen im sichtbaren Bereich einer Scheibe. Diese wird zu Bruch gemeldet.

Die Grenzen dieser Klassen werden in Abstimmung mit den Kunden festgelegt.

> **Bruchscheiben verwenden**
> Sollte eine als Bruch markierte Scheibe verwendet werden können (Fehler konnte z. B. durch Reinigen behoben werden), können Sie diese mit einem Klick als gut melden!
