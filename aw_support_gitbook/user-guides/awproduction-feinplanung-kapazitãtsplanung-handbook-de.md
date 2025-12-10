---
title: "A+W Production Feinplanung und Kapazitätsplanung"
source: "DE_HB_AWProduction_5.pdf"
tags: ["A+W Production", "Feinplanung", "Kapazitätsplanung", "Software-Referenz", "Produktionsplanung", "ERP", "Glasfertigung", "Tutorial", "Stammdaten"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A detailed software reference and tutorial for the A+W Production modules Feinplanung (Detailed Planning) and Kapazitätsplanung (Capacity Planning). It covers master data setup, configuration, and operational procedures."
long_description: "This document serves as a comprehensive guide to the A+W Production software, focusing on the Feinplanung (Detailed Planning) and Kapazitätsplanung (Capacity Planning) modules. The first part is a software reference for Feinplanung, detailing the configuration of storage places (Abstellplätze), batch types (Lostypen), and the various parameters within the detailed planning dialogs for production runs (Läufe). It explains fields, settings, and technical database information for optimizing cutting processes, managing special parts like fillers and remnants, and configuring organizational parameters. The second part is a tutorial for Kapazitätsplanung, designed for production planners. It provides an overview of capacity planning principles, including master data setup for machines, shifts, and lead times. It explains how to use the production monitor to manage and adjust production schedules, handle faulty schedules, create campaigns for specific work processes, and reserve capacity for specific customers or projects. The tutorial includes step-by-step instructions with screenshots to guide users through common tasks."
---

# Softwarereferenz

---
## Abstellplätze

**Technische Info: Datenbankfeld: DIGITSFACH**

**Max. Anzahl Fächerwagen**
Die maximale Anzahl an Fächerwagen ist für die Bildung von Opti-Gruppen wichtig. Wenn eine Glasart die maximal erlaubte Anzahl erreicht, so wird für alle Optimierungen die aktuelle Opti-Gruppe geschlossen und eine neue begonnen. Diese kann dann zugeschnitten werden, wenn wieder Wagen frei sind.

**Überprüfung Anzahl (Zuschnitt)**
Die Checkbox bezieht sich auf den im Feld Max. Anzahl Fächerwagen stehenden Wert und prüft diesen gegebenenfalls.
Der im Feld Max. Anzahl Fächerwagen stehende Wert wird geprüft. Wird er überschritten, erfolgt eine entsprechende Fehlermeldung. Die Feinplanung kann dann weder optimiert noch gespeichert werden.
Es erfolgt keine Überprüfung der Anzahl.

**Sortjet**
Arbeiten Sie in Ihrem Hause mit einem Sortjet, müssen Sie diese Checkbox aktivieren.
Technische Info: Datenbankfeld: SORTJET

**Maximale Nutzlast (kg)**
Erlaubtes Nutzgewicht des Abstellplatzes in Kilogramm. Ist dieses Gewicht erreicht, so wird ein neuer Abstellplatz angefangen. 0 bedeutet hier, dass es keine Gewichtsbegrenzung gibt. Ist 0 angegeben, wird die Zahl der auf dem Fächerwagen abzulegenden Scheiben nur durch die Anzahl der Fächer begrenzt.
Technische Info: Datenbankfeld: GEWICHT

**Leergewicht (kg)**
Das Leergewicht des Abstellplatzes in Kilogramm.
Technische Info: Datenbankfeld: LEERGEWICHT

**Abstand erstes/letztes Fach v. Achsen**
Hier geben Sie den Abstand zwischen Außenkante und Achse (links/rechts) ein.
Technische Info: Datenbankfeld: ABSTAND_FACH_ACHSE

**Max. Abweichung Schwerpunkt v. Mitte (%)**
Hier geben Sie die erlaubte Abweichung von der Schwerpunktmitte aus in Prozent ein (+/-).
Technische Info: Datenbankfeld: ABWEICHUNG_SP

### Erläuterung der Felder im Bereich Feste Abstellplätze

**Kombobox**
Die Kombobox unterhalb der Schaltflächen [Hinzufügen], [Entfernen] und [Umbenennen] enthält alle im System angelegten Festen Abstellplätze.

**Abstelltiefe**
In diesem Feld geben Sie die Abstelltiefe in mm an. Bsp.: 1200 mm bedeutet, dass der Stapel, der abgestellt wird, bis zu 1200 mm tief sein darf. Bitte beachten Sie, dass Abstelltiefen ab 20 m automatisch als unendliche große Abstelltiefen behandelt werden.
Technische Info: Datenbankfeld: TIEFE

*A+W Production Feinplanung*
*D-401*

---

## Abstellplätze

*D-402*

**Softwarereferenz**

**Breite**
Dieses Feld kennzeichnet die Gesamtbreite des Abstellplatzes in mm. Bsp. 2000 mm bedeutet, dass der Abstellplatz eine Breite von 2000 mm hat, auf der Scheiben abgestellt werden können.
Technische Info: Datenbankfeld: BREITE

**Max. Anzahl FAPs**
Die maximale Anzahl an Festen Abstellplätzen ist für die Bildung von Opti-Gruppen wichtig. Wenn eine Glasart die maximal erlaubte Anzahl erreicht, so wird für alle Optimierungen die aktuelle Opti-Gruppe geschlossen und eine neue begonnen. Diese kann dann zugeschnitten werden, wenn wieder Abstellplätze frei sind.

**Überprüfung Anzahl (Zuschnitt)**
Die Checkbox bezieht sich auf den im Feld Max. Anzahl FAPs stehenden Wert und prüft dieses gegebenenfalls.
Der im Feld FAPs stehenden Wert wird geprüft. Wird er überschritten, erfolgt eine entsprechende Fehlermeldung. Der feingeplante Lauf kann dann weder optimiert noch können die Ergebnisse gespeichert werden.
Es erfolgt keine Überprüfung der Anzahl.

**Maximales Gewicht (kg)**
Maximales Gewicht aller Scheiben auf dem Festen Abstellplatz. Ist dieses Gewicht erreicht, so wird ein neuer Abstellplatz angefangen. O bedeutet hier, dass es keine Gewichtsbegrenzung gibt.
Technische Info: Datenbankfeld: GEWICHT

**Weitere Informationen zu Abstellplätzen**
⇨ Tutorial, "Abstellplätze" auf Seite D-289
⇨ Überblick, "Schaltflächen" auf Seite A-92

*A+W Production Feinplanung*

---

## Lose

**Softwarereferenz**

In dem Dialog Lostypen und Bearbeitungen nehmen Sie die Einstellungen bezüglich der Losbildung für einen Lostyp vor. Dem Lostyp werden anschließend noch Bearbeitungen oder abhängige Bearbeitungen zugeordnet.

### Lostypen und Bearbeitungen

Der Dialog ist in drei Register unterteilt:
- Register Lostypen
- Register Bearbeitungen
- Register Abhängige Bearbeitungen

### Register Lostypen

**Stammdaten > Feinplanung > Lostypen**

