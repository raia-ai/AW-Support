---
title: "DE_AWProduction_Realtime_Optimizer_3_1"
source: "DE_AWProduction_Realtime_Optimizer_3_1.pdf"
tags: ["A+W", "Realtime Optimizer", "A+W Production", "glass manufacturing", "window production", "software manual", "optimization", "cutting control", "production management", "German"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a German-language user manual for the A+W Realtime Optimizer software, version 3.30. It serves as a tutorial and software reference for end-users in the glass, window, and door manufacturing industries. The manual details the functionalities for production optimization, cutting control, and data management."
long_description: "This comprehensive user manual, written in German, provides detailed instructions for operating the A+W Realtime Optimizer software, a component of the A+W Production suite. The document is structured into a tutorial and a software reference section. The tutorial covers the fundamental concepts, key features, and step-by-step workflows. It explains how to work with the software, including data transfer from upstream systems like A+W Production or in a stand-alone configuration. Key processes such as manual data entry for broken or rush items, creating cutting plans, optimization, and cutting machine control are thoroughly explained. The manual details various types of optimization, including table optimizations and quick optimizations, and how to handle remnants and link production runs. It also describes the integration with other A+W modules like A+W Residual Stock Manager, A+W Pattern Viewer, and A+W PlanEditor to enhance production efficiency. The software reference section, detailed in the table of contents, provides an in-depth look at the user interface, menus, and specific dialogs for tasks like data entry, optimization parameter settings, and cutting management. This guide is essential for operators and production managers using A+W software to optimize material usage, reduce waste, and streamline the cutting process in glass, window, and door manufacturing."
---

# A+W Realtime Optimizer J

---
## A+W Production
A+W - Software for Glass, Windows and Doors

---

## Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version / Datum | Beschreibung |
| :--- | :--- |
| 3.30/01-2023 | Diverse Ergänzungen |
| 3.20/10-2020 | Dialog Tischoptimierung hinzugefügt |
| 3.10/04-2019 | Dialog DynOpt-Einstellungen hinzugefügt |
| 3.02/09-2018 | Felder hinzugefügt |
| 3.01/01-2017 | Produkt- und Firmennamen angepasst |
| 3.00/03-2015 | Komplette Überarbeitung |
| 2.01/07-2013 | Vollständige Überarbeitung der XOPT-ON-Dokumentation und Anpassung auf A+W Realtime Optimizer. |
| 2.00/09-2007 | Komplette Überarbeitung |
| 1.00/03-2003 | Ersterstellung |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen
- Kontakt

**Anmerkungen zu diesem Dokument**

Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Realtime Optimizer gedacht.
Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.
Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von A+W Production.

**Urheberrechte**

© 2023, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.
Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

**Warenzeichen**

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

**Kontakt**

A+W Software GmbH
Siemensstr. 3
D-35463 Fernwald
Germany
+49 641 96620-0
info@a-w.com
http://www.a-w.com

---

## Inhalt

- **Vorspann** (J-3)
  - Revisionsübersicht (J-3)
  - Editorial (J-3)
- **Inhalt** (J-5)
- **Tutorial** (J-9)
  - Grundgedanken (J-11)
  - Leistungsmerkmale (J-12)
  - Arbeiten mit A+W Realtime Optimizer (J-13)
    - Überblick (J-14)
    - Datenübernahme (J-15)
    - Anbindung an A+W Production (J-16)
    - Stammdaten (J-17)
    - Verwendung als stand alone-System (J-17)
    - Optimierungen importieren (J-17)
  - Erfassung (J-19)
    - Überblick (J-20)
    - Bruch, Eilscheiben und Füllaufträge (J-21)
    - Scheiben manuell erfassen (J-22)
    - Manuelle Planerstellung (J-25)
    - Chargen-Editor (J-26)
  - Optimierung (J-27)
    - Überblick (J-28)
    - Tischoptimierungen (J-29)
    - Tischoptimierungen erstellen (J-29)
    - Ergebnis der Tischoptimierung prüfen und bearbeiten (J-31)
    - Tischoptimierung auflösen (J-32)
    - Tischoptimierungen verlinken (J-34)
    - Schnelloptimierung erstellen (J-35)
    - Verlinken von Läufen (J-36)
    - Tischansteuerung (J-37)
  - Zuschnitt (J-38)
    - Überblick (J-39)
    - Läufe zum Zuschnitt auswählen (J-40)
    - Optimierung prüfen und schneiden (J-43)
    - Arbeit unterbrechen und fortsetzen (J-45)
    - Die Zuschnitt-Übersicht (J-46)
    - Schneidstatus zurücksetzen (J-48)
  - Zusammenarbeit mit anderen Modulen (J-49)
    - Überblick (J-50)
    - A+W Residual Stock Manager (J-50)
    - A+W Planning Web (J-50)
    - Oberfläche (J-51)
    - Stammdaten (J-51)
  - A+W Pattern Viewer (J-59)
    - Einstellungen (J-59)
    - Die Oberfläche (J-60)
    - Die Menüleiste (J-60)
    - Informationen zu Scheibe und Verschnitt (J-69)
    - Verlinkte Läufe anzeigen (J-69)
    - Abstellkante anzeigen (J-70)
    - Symbol für Stempel, Logo oder Referenzmarke anzeigen (J-70)
    - Farbauswahl für Auftragspositionen (J-71)
    - Erste und letzte Scheibe markieren (J-71)
    - Bruchscheiben (J-71)
  - A+W PlanEditor (J-72)
  - A+W Continuous Cutting (J-73)
    - Übersicht der geplanten Läufe (J-73)
    - Gruppieren (J-76)
    - Eilgruppen (J-77)
    - Zurücksetzen von Läufen (J-77)
    - Zuschneiden (J-78)
  - A+W Defect Optimizer (J-80)
  - A+W DynOpt Compact (J-81)
    - A+W DynOpt Compact Import (J-81)
    - A+W DynOpt Compact Optimierung (J-81)
    - A+W DynOpt Compact-Lauf erzeugen (J-82)
- **Softwarereferenz** (J-85)
  - Übersicht (J-87)
    - Menüs (J-87)
    - Symbol-Schaltflächen (J-88)
  - Erfassung (J-89)
    - Eilscheiben (J-90)
    - Eilscheiben-Eingabe (J-92)
    - Form-Erfassung (J-94)
    - Modell-Nummer (J-96)
    - Manuelle Planerstellung (J-97)
    - Chargen-Editor (J-100)
  - Optimierung (J-102)
    - Selektieren Sie die zu optimierenden Gläser (J-103)
    - Tischoptimierung in der Variante Standard (J-103)
    - Tischoptimierung in der Variante Produktionstermin (J-106)
    - Tischoptimierung Lauf [Nr] (J-107)
    - Übersicht (J-107)
    - Optimieren (J-110)
    - Erläuterung der Felder im Bereich Optimierungsreihenfolge (J-110)
    - Erläuterung der Schaltflächen im Bereich Rangfolge (J-111)
    - Erläuterung der Felder im Bereich Automatische Zusammenstellung (J-111)
    - Erläuterung der Felder im Bereich Lauf-Parameter (J-112)
    - Erläuterung der Felder im Bereich Tisch (J-112)
    - Erläuterung der Felder im Bereich Optimierungs-Parameter (J-112)
    - Restplattlagerplatten und Lagerplatten (J-113)
    - Parameter (J-115)
    - Anzahl der Lagerplatten (J-118)
    - Zurücksetzen eines Zuschnitt Laufes (J-119)
    - Pausierende Glasarten (J-121)
    - Aktuell geänderte Einstellungen (J-123)
  - Zuschnitt (J-124)
    - Wählen Sie einen Lauf aus (J-125)
    - Lauf [Nummer] - Lauf [Nummer] (J-129)
    - Optimierungsreihenfolge (J-131)
    - Lauf: Nummer (J-132)
    - Auswahl der zu verlinkenden Optimierung (J-136)
    - Optimierungsergebnis (J-137)
    - Bruchpool (J-138)
    - Brucherfassung (J-141)
    - Suchfelder (J-142)
    - Modell-Erfassung (J-143)
    - A+W DynOpt - Editor (J-144)
    - Erläuterung der Schaltflächen (J-145)
  - Einstellungen (J-148)
    - Einstellungen (J-149)
    - Tischoptimierung (J-151)
  - Ansicht (J-152)
  - Import (J-153)
  - Fehlermeldungen (J-154)
  - A+W Residual Stock Manager (J-155)
  - A+W Planning Web (J-155)
  - Lager (J-155)
    - Abstellplatzinformationen (J-157)
  - Gestelle (J-159)
    - Gestelleigenschaften (J-161)
    - Eindeutiger Name zur Identifizierung eines Gestelltyp. (J-161)
  - Glasübersicht (J-163)
    - Wenn Sie auf diese Schaltfläche klicken, wird der Datensatz zur Bearbeitung freigegeben und Sie können Änderungen vornehmen. (J-165)
    - Neuen Datensatz hinzufügen/bearbeiten (J-166)
- **Partindex** (J-169)
- **Index A+W Realtime Optimizer** (J-171)

---
---

## Tutorial

### Grundgedanken

Ein wesentliches Einsparpotential bei der Flachglasverarbeitung ist die optimale Ausnutzung der Lagerplatten beim Zuschnitt. Je weniger Verschnitt oder Restblätter, desto höher die Materialausnutzung und desto geringer die Materialkosten. Die Ansteuerung von Zuschnitttischen mit den optimierten Schnittbildern direkt aus der Optimierung beschleunigt den Arbeitsprozess.

A+W Realtime Optimizer basiert auf diesen beiden Grundgedanken:
- Zuschnittoptimierung für den angeschlossenen Zuschnitttisch.
- Übertragung von Schneidcode an den angeschlossenen Zuschnitttisch.

*Abb. J-1: Zuschnittoptimierung und Tischansteuerung*
