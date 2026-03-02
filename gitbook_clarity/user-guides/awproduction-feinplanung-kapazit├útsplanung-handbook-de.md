---
description: "A+W Production Feinplanung und Kapazitätsplanung"
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

