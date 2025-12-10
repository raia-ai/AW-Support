---
title: "DE_AWProduction_Feinplanung_3_4"
source: "DE_AWProduction_Feinplanung_3_4.pdf"
tags: ["A+W Production", "Feinplanung", "Software Reference", "Glass Manufacturing", "ERP", "Optimization", "Storage Locations", "Batches", "Production Planning", "Technical Documentation"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference manual for the A+W Production Feinplanung (Fine Planning) module. It provides detailed explanations of the settings and parameters for managing storage locations (Abstellplätze), batch types (Lostypen), and the fine-planning of production runs (Läufe)."
long_description: "This comprehensive technical reference guide details the configuration and use of the A+W Production Feinplanung (Fine Planning) software module. It is intended for administrators and advanced users responsible for setting up and managing production planning processes in a glass manufacturing environment. The document is divided into several key sections. The 'Abstellplätze' section covers the setup of various storage locations, including A-racks (A-Böcke), compartment carts (Fächerwagen), and fixed storage locations (Feste Abstellplätze), detailing parameters like depth, width, capacity, and robot control. The 'Lose' section explains the creation and management of batch types, including their properties, grouping rules, and relationships with different processing steps and procurement types. It also covers the automatic generation of dependent processing steps. The 'Läufe feinplanen' section provides an in-depth walkthrough of the fine-planning dialog, which appears after a run has been roughly planned. It explains the various tabs (Register) used to review and modify planning parameters, such as 'Glasarten' (Glass Types), 'Bockbelegung' (Rack Assignment), 'Ergebnisse' (Results), 'Spezial' (for handling remnants, broken sheets, and fillers), 'Orga' (organizational settings), and 'Optionen' (optimization parameters). For many fields, the corresponding database table and field names are provided under 'Technische Info'."
---

---
## Abstellplätze

**Technische Info:** Datenbanktabelle: ABSTELLPLATZ

### Erläuterung der Felder im Bereich A-Böcke

**Kombobox**
Die Kombobox unterhalb der Schaltflächen [Hinzufügen], [Entfernen] und [Umbenennen] enthält die Namen der im System angelegten Abstellplätze für A-Böcke.

**Abstelltiefe**
In diesem Feld geben Sie die Abstelltiefe in mm an. Bsp. 1200 mm bedeutet, dass der Stapel, der abgestellt wird, bis zu 1200 mm tief sein darf. Bitte beachten Sie, dass Abstelltiefen ab 20 m automatisch als unendliche große Abstelltiefen behandelt werden.
**Technische Info:** Datenbankfeld: TIEFE

**Breite**
Dieses Feld kennzeichnet die Gesamtbreite des Abstellplatzes in mm. Bsp. 2000 mm bedeutet, dass der Abstellplatz eine Breite von 2000 mm hat, auf der Scheiben abgestellt werden können.
**Technische Info:** Datenbankfeld: BREITE

**Max. Abstellplätze/Bock**
In diesem Feld geben Sie ein, wie viele Abstellplätze Ihnen pro Bock zur Verfügung stehen. Mögliche Werte:
- 1 = pro Bock steht Ihnen ein Abstellplatz zur Verfügung.
- 2 = pro Bock stehen Ihnen 2 Abstellplätze zur Verfügung.
- 4 = pro Bock stehen Ihnen 4 Abstellplätze zur Verfügung.
**Technische Info:** Datenbankfeld: MAXCOUNT

**L-Bock**
Diese Checkbox muss aktiviert werden, wenn es sich bei dem Abstellplatz um einen L-Bock anstelle eines A-Bocks handelt.

**Robot**
Diese Checkbox muss aktiviert werden, wenn es sich bei dem A-Bock um einen Robot-Bock handelt. Bei einem Robot-Bock handelt es sich um einen Abstellplatz, der durch einen Roboter angesteuert wird. Mögliche Werte:
- 0 = Kein Robot-Bock.
- 1 = Einfach = Robot-Bock, einfach.
- 2 = Gespiegelt = Robot-Bock, gespiegelt.
- 3 = Doppelt=Robot-Bock, doppelt vorhanden, dabei getrennt ansteuerbar.
**Technische Info:** Datenbankfeld: ROBOT

**Anzahl**
Dieses Feld ist nur aktiv, wenn es sich bei dem A-Bock um einen Robot-Bock handelt. Sie haben dann die Möglichkeit zu hinterlegen, wie viele Robot-Böcke im Betrieb vorhanden sind. Ferner können Sie angeben, ob diese Anzahl einfach oder doppelt vorhanden ist, oder ob die Robot-Böcke eigentlich zweifach ausgelegt sind, aber das System bei Auslastung selber entscheidet, welchen Robot-Bock es verwendet. Den mit gegebener Nummer aus der ersten oder zweiten Menge.

**Max. Anzahl A-Böcke**
Die maximale Anzahl an A-Böcken ist für die Bildung von Opti-Gruppen wichtig. Wenn eine Glasart die maximal erlaubte Anzahl erreicht, so wird für alle Optimierungen die aktuelle Opti-Gruppe geschlossen und eine neue begonnen. Diese kann dann zugeschnitten werden, wenn wieder Böcke frei sind.

**Überprüfung Anzahl (Zuschnitt)**
Die Checkbox bezieht sich auf den im Feld **Max. Anzahl A-Böcke** stehenden Wert und prüft diesen gegebenenfalls.

**Sortjet**
Arbeiten Sie in Ihrem Hause mit einem Sortjet, müssen Sie diese Checkbox aktivieren.
**Technische Info:** Datenbankfeld: SORTJET

**Maximales Gewicht (kg)**
Maximales Gewicht aller Scheiben auf dem A-Bock. Ist dieses Gewicht erreicht, so wird ein neuer Abstellplatz angefangen. 0 bedeutet hier, dass es keine Gewichtsbegrenzung gibt.
**Technische Info:** Datenbankfeld: GEWICHT

**ID für Stack-Opti**
Arbeiten Sie in Ihrem Hause mit dem Stack Optimizer, wird hier die ID des verwendeten physikalischen Abstellplatzes hinterlegt. Die möglichen Werte holt sich die Anwendung aus den Konfigurationsdateien des Stack Optimizers.
**Technische Info:** Datenbankfeld: STACK_ID

### Erläuterung der Felder im Bereich Fächerwagen

**Kombobox**
Die Kombobox unterhalb der Schaltflächen [Hinzufügen], [Entfernen] und [Umbenennen] enthält die Namen der im System angelegten Abstellplätze für Fächerwagen.

**Anzahl Fachnummer**
In diesem Feld geben Sie an, wieviel Fachnummern der Wagen hat. Bei einem Fach pro Nummer entspricht die Anzahl der Fachnummern der Anzahl der Fächer des Wagens.
**Technische Info:** Datenbankfeld: FACHANZAHL

**Breite**
Dieses Feld kennzeichnet die Breite der Fächer.
**Technische Info:** Datenbankfeld: BREITE

**Zwei Fächer/Nummer**
Die Checkbox steuert, ob jeweils zwei Fächer eine gemeinsame Fachnummer bekommen. Die Anzahl der Fachnummern ist dann nur noch halb so groß wie die Anzahl der Fächer. D.h., es dürfen auch zwei Scheiben gemeinsam in ein Fach gestellt werden.
**Technische Info:** Datenbankfeld: FACH_PRO_NR

**Start = 0**
Die Checkbox steuert, ob die Zählung der Fachnummern bei 0 oder bei 1 beginnt.
- ☐ Die Zählung der Fachnummern beginnt mit 0.
- ☑ Die Zählung der Fachnummern beginnt mit 1 (Standard).
**Technische Info:** Datenbankfeld: STARTFACH

**Anzahl der Stellen für**
Diese Radiotaste legt fest, wie viele Stellen der Abstellplatznummer für die Fachnummern reserviert werden.
- 2 bedeutet, dass die letzten 2 Stellen reserviert sind.
- 3 bedeutet, dass die letzten 3 Stellen reserviert sind.
- 4 bedeutet, dass die letzten 4 Stellen reserviert sind.
Bei 50 Fachnummern sind das 2 Stellen, ab 100 Fachnummern 3 Stellen usw.
**Technische Info:** Datenbankfeld: DIGITSFACH

**Max. Anzahl Fächerwagen**
Die maximale Anzahl an Fächerwagen ist für die Bildung von Opti-Gruppen wichtig. Wenn eine Glasart die maximal erlaubte Anzahl erreicht, so wird für alle Optimierungen die aktuelle Opti-Gruppe geschlossen und eine neue begonnen. Diese kann dann zugeschnitten werden, wenn wieder Wagen frei sind.

**Überprüfung Anzahl (Zuschnitt)**
Die Checkbox bezieht sich auf den im Feld **Max. Anzahl Fächerwagen** stehenden Wert und prüft diesen gegebenenfalls.
- ☑ Der im Feld **Max. Anzahl Fächerwagen** stehende Wert wird geprüft. Wird er überschritten, erfolgt eine entsprechende Fehlermeldung. Die Feinplanung kann dann weder optimiert noch gespeichert werden.
- ☐ Es erfolgt keine Überprüfung der Anzahl.

**Sortjet**
Arbeiten Sie in Ihrem Hause mit einem Sortjet, müssen Sie diese Checkbox aktivieren.
**Technische Info:** Datenbankfeld: SORTJET

**Maximale Nutzlast (kg)**
Erlaubtes Nutzgewicht des Abstellplatzes in Kilogramm. Ist dieses Gewicht erreicht, so wird ein neuer Abstellplatz angefangen. 0 bedeutet hier, dass es keine Gewichtsbegrenzung gibt. Ist 0 angegeben, wird die Zahl der auf dem Fächerwagen abzulegenden Scheiben nur durch die Anzahl der Fächer begrenzt.
**Technische Info:** Datenbankfeld: GEWICHT

**Leergewicht (kg)**
Das Leergewicht des Abstellplatzes in Kilogramm.
**Technische Info:** Datenbankfeld: LEERGEWICHT

**Abstand erstes/letztes Fach v. Achsen**
Hier geben Sie den Abstand zwischen Außenkante und Achse (links/rechts) ein.
**Technische Info:** Datenbankfeld: ABSTAND_FACH_ACHSE

**Max. Abweichung Schwerpunkt v. Mitte (%)**
Hier geben Sie die erlaubte Abweichung von der Schwerpunktmitte aus in Prozent ein (+/-).
**Technische Info:** Datenbankfeld: ABWEICHUNG_SP

### Erläuterung der Felder im Bereich Feste Abstellplätze

**Kombobox**
Die Kombobox unterhalb der Schaltflächen [Hinzufügen], [Entfernen] und [Umbenennen] enthält alle im System angelegten Festen Abstellplätze.

**Abstelltiefe**
In diesem Feld geben Sie die Abstelltiefe in mm an. Bsp.: 1200 mm bedeutet, dass der Stapel, der abgestellt wird, bis zu 1200 mm tief sein darf. Bitte beachten Sie, dass Abstelltiefen ab 20 m automatisch als unendliche große Abstelltiefen behandelt werden.
**Technische Info:** Datenbankfeld: TIEFE

**Breite**
Dieses Feld kennzeichnet die Gesamtbreite des Abstellplatzes in mm. Bsp. 2000 mm bedeutet, dass der Abstellplatz eine Breite von 2000 mm hat, auf der Scheiben abgestellt werden können.
**Technische Info:** Datenbankfeld: BREITE

**Max. Anzahl FAPs**
Die maximale Anzahl an Festen Abstellplätzen ist für die Bildung von Opti-Gruppen wichtig. Wenn eine Glasart die maximal erlaubte Anzahl erreicht, so wird für alle Optimierungen die aktuelle Opti-Gruppe geschlossen und eine neue begonnen. Diese kann dann zugeschnitten werden, wenn wieder Abstellplätze frei sind.

**Überprüfung Anzahl (Zuschnitt)**
Die Checkbox bezieht sich auf den im Feld **Max. Anzahl FAPs** stehenden Wert und prüft dieses gegebenenfalls.
- ☑ Der im Feld FAPs stehenden Wert wird geprüft. Wird er überschritten, erfolgt eine entsprechende Fehlermeldung. Der feingeplante Lauf kann dann weder optimiert noch können die Ergebnisse gespeichert werden.
- ☐ Es erfolgt keine Überprüfung der Anzahl.

**Maximales Gewicht (kg)**
Maximales Gewicht aller Scheiben auf dem Festen Abstellplatz. Ist dieses Gewicht erreicht, so wird ein neuer Abstellplatz angefangen. O bedeutet hier, dass es keine Gewichtsbegrenzung gibt.
**Technische Info:** Datenbankfeld: GEWICHT

**Weitere Informationen zu Abstellplätzen**
- ⇨ Tutorial, "Abstellplätze" auf Seite F-38
- ⇨ Überblick, "Schaltflächen" auf Seite A-78

## Lose

In dem Dialog **Lostypen und Bearbeitungen** nehmen Sie die Einstellungen bezüglich der Losbildung für einen Lostyp vor. Dem Lostyp werden anschließend noch Bearbeitungen oder abhängige Bearbeitungen zugeordnet.

### Lostypen und Bearbeitungen

Der Dialog ist in drei Register unterteilt:
- Register Lostypen
- Register Bearbeitungen
- Register Abhängige Bearbeitungen

### Register Lostypen

*Stammdaten > Feinplanung > Lostypen*

