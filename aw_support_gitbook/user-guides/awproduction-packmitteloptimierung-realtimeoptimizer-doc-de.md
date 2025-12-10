---
title: "D-AWProduction-HB_12"
source: "D-AWProduction-HB_12.pdf"
tags: ["A+W Production", "Packmitteloptimierung", "Realtime Optimizer", "Software Reference", "Tutorial", "Glass Cutting", "Optimization", "Zuschnitt", "PackView", "A+W Software"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical manual for A+W's production software, detailing the Packmitteloptimierung (Packaging Optimization) module in PackView and the A+W Realtime Optimizer for cutting optimization. It includes software references and tutorials."
long_description: "This document serves as a comprehensive technical guide for two key components of the A+W Production software suite: Packmitteloptimierung and A+W Realtime Optimizer. The first section is a software reference for the 'Packmitteloptimierung' (Packaging Optimization) module, accessible through PackView. It details the various menu functions, buttons, and views for manipulating and organizing packaging units (scheiben) on racks (gestelle). This includes functions for rotation, alignment, viewing properties, and managing racks and crates. The second, more extensive part of the document focuses on the A+W Realtime Optimizer, a powerful tool for optimizing glass cutting processes. This section is divided into a tutorial and a software reference. The tutorial covers fundamental concepts, data transfer from upstream systems, manual data entry for urgent or broken items, creating and managing cutting optimizations (Tischoptimierungen), and controlling the cutting table (Zuschnitt). It also explains how the Realtime Optimizer interacts with other A+W modules like Pattern Viewer, Residual Stock Manager, and PlanEditor to create a seamless production workflow. The software reference provides an exhaustive description of every dialog, menu, button, and parameter within the Realtime Optimizer, making it an essential resource for operators and system administrators."
---

# A+W Production Packmitteloptimierung

---
## Softwarereferenz - Menüs

### Rotiere Einheit gegen den Uhrzeigersinn
[ICON]
Diese Schaltfläche ist nur aktiv, wenn Sie sich im Bearbeitungs-Modus befinden und zuvor eine Scheibe markiert wurde. Sie können dann die markierte Scheibe um 90 Grad gegen den Uhrzeigersinn drehen. Klicken Sie anschließend auf Schaltfläche Einfügen, wird die Scheibe an dieser Stelle eingefügt.

### Einheit nach links ausrichten
[ICON]
Diese Schaltfläche ist nur aktiv, wenn Sie sich im Bearbeitungs-Modus befinden und zuvor eine Scheibe markiert wurde. Sie können dann die markierte Scheibe zur linken Seite des Stapels hin ausrichten. Klicken Sie anschließend auf Schaltfläche Einfügen, wird die Scheibe an dieser Stelle eingefügt.

### Einheit zur Mitte ausrichten
[ICON]
Diese Schaltfläche ist nur aktiv, wenn Sie sich im Bearbeitungs-Modus befinden und zuvor eine Scheibe markiert wurde. Sie können dann die markierte Scheibe zur Mitte des Stapels hin ausrichten. Klicken Sie anschließend auf Schaltfläche Einfügen, wird die Scheibe an dieser Stelle eingefügt.

### Einheit nach rechts ausrichten
[ICON]
Diese Schaltfläche ist nur aktiv, wenn Sie sich im Bearbeitungs-Modus befinden und zuvor eine Scheibe markiert wurde. Sie können dann die markierte Scheibe zur rechten Seite des Stapels hin ausrichten. Klicken Sie anschließend auf Schaltfläche Einfügen, wird die Scheibe an dieser Stelle eingefügt.

### Experten-Modus
[ICON]
Schaltet den Experten-Modus ein bzw. aus.

### Freie Rotation der Gestellansicht
[ICON]
Schaltet freie Rotation ein/aus. Die Symbol-Schaltfläche steht in direktem Zusammenhang mit der Symbol-Schaltfläche für den Experten-Modus. Sie ist nur dann aktiv, wenn der Experten-Modus eingeschaltet ist. Wenn Sie diese Symbol-Schaltfläche betätigen, ändert sich der Mauszeiger und Sie können das Gestell zur Sichtung frei drehen. Bei eingeschalteter Rotation, ist die Symbol-Schaltfläche hellgrau unterlegt und der Mauszeiger ändert sich in das Symbol: [ICON]

> Durch einen entsprechenden Schubs können Sie das Gestell dabei in eine fortlaufende Drehung versetzen. Diese können Sie durch einen Klick auf [ICON] beenden.

### Bemaßungs-Werkzeug
[ICON]
Schaltet Bemaßungs-Werkzeug ein/aus. Wenn Sie diese Symbol-Schaltfläche betätigen, ändert sich der Mauszeiger und Sie können verschiedene Abstände vermessen. Die Messergebnisse werden am unteren Bildschirmrand eingeblendet. Bei eingeschalteter Bemaßung, ist die Symbol-Schaltfläche hellgrau unterlegt und der Mauszeiger ändert sich in das Symbol: [ICON]

### Eigenschaften der Einheit
[ICON]
Eigenschaften der Einheit ein-/ausblenden. Wenn Sie diese Symbol-Schaltfläche betätigen, öffnet sich der Dialog Eigenschaft Einheit.
⇨ Softwarereferenz, "Eigenschaften Referenz-Einheiten" auf Seite 1-1054

### 3D-Ansicht
[ICON]
Schaltet die 3D-Ansicht ein/aus. Wenn Sie diese Symbol-Schaltfläche betätigen, aktivieren bzw. deaktivieren Sie die 3D-Ansicht. Bei aktivierter 3D-Ansicht ist die Symbol-Schaltfläche hellgrau unterlegt.

### Draufsicht
[ICON]
Schaltet die Draufsicht ein/aus. Wenn Sie diese Symbol-Schaltfläche betätigen, aktivieren bzw. deaktivieren Sie die Draufsicht. Bei aktivierter Draufsicht ist die Symbol-Schaltfläche hellgrau unterlegt.

### Kanten-Ansicht
[ICON]
Schaltet die Kanten-Ansicht ein/aus. Wenn Sie diese Symbol-Schaltfläche betätigen, aktivieren bzw. deaktivieren Sie die Draufsicht. Bei aktivierter Draufsicht ist die Symbol-Schaltfläche hellgrau unterlegt.

### Detail-Ansicht
[ICON]
Schaltet die Detail-Ansicht ein/aus. Wenn Sie diese Symbol-Schaltfläche betätigen, aktivieren bzw. deaktivieren Sie die Detail-Ansicht. Bei aktivierter Detail-Ansicht ist die Symbol-Schaltfläche hellgrau unterlegt. Die Detail-Ansicht und die Zwischenablage können gleichzeitig angezeigt werden.

### Zwischenablage
[ICON]
Schaltet die Detail-Ansicht zwischen der Gestellbelegung und der Zwischenablage hin und her. Haben Sie Einheiten in die Zwischenablage kopiert, können Sie sich beim Aktivieren dieser Symbol-Schaltfläche den bzw. die Inhalte der Zwischenablage anzeigen lassen. Die Zwischenablage und die Detail-Ansicht können gleichzeitig angezeigt werden.

### Ansichten
PackView verfügt über folgende Ansichten:
*   3D-Ansicht
*   Draufsicht
*   Detail-Ansicht

Nähere Erläuterungen zu den Ansichten finden Sie im Tutorial:
⇨ Tutorial, "Ansichten" auf Seite I-980

### Gestellbezeichnung ändern
**Pfad:** PackView > Bearbeiten ein > Menü Bearbeiten > Gestellbezeichnung ändern ...

*Abb. 1-85: Eingabe*

In diesem Dialog können Sie die Gestellbezeichnung ändern. Es sind lediglich die Felder freigegeben, die zum Ändern der Gestellbezeichnung notwendig sind. Auf die anderen Felder haben Sie an dieser Stelle keinen Zugriff.

**Technische Info:** Datenbanktabelle: PMO_RACKS

#### Erläuterung der Felder
**Gruppe** Die Kombobox ist mit dem Eintrag -Aktuell- vorbelegt und kann nicht geändert werden. In der darunter liegenden Kombobox sehen Sie den Namen der Gestellbezeichnung. Sie können mit der Maus in das Feld klicken und den Namen überschreiben. Wenn Sie den Dialog mit der Schaltfläche [OK] verlassen, wird der Name in der Tabelle geändert.

> **Kundenindividuelle Einstellungen**
> In Abhängigkeit von der jeweiligen Installation (Einstellungen in Ihrem Hause) können Sie in der Kombobox Gruppe die gewünschte Gestellgruppe auswählen. Innerhalb der Gestellgruppe dann das entsprechende Gestell. Das ist immer dann möglich, wenn aus einer großen Anzahl von Gestellen oder Kisten gewählt werden soll. Das Verhalten wird dann von der A+W Software GmbH entsprechend konfiguriert.

**Weitere Informationen zu Neue Gestellbezeichnung ändern**
⇨ Konventionen, "Bedienoberfläche" auf Seite A-77
⇨ Konventionen, "Schaltflächen" auf Seite A-78

### Neue Gestell-Eigenschaften
**Pfad:** PackView > Bearbeiten ein > Menü Bearbeiten > Neues Gestell einfügen ...

*Abb. I-86: Neue Gestell-Eigenschaften*

In diesem Dialog haben Sie die Möglichkeit, ein neues Gestell hinzuzufügen.

**Technische Info:** Datenbanktabelle: PMO_RACKS

#### Erläuterung der Felder im Bereich Abmessungen
**Breite** In diesem Feld geben Sie Breite (in mm) des Gestells ein, das Sie hinzufügen möchten.
**Technische Info:** Eingabe zwingend, Numerisch, Datenbankfeld: WIDTH

**Höhe** In diesem Feld geben Sie Höhe (in mm) des Gestells ein, das Sie hinzufügen möchten.
**Technische Info:** Eingabe zwingend, Numerisch, Datenbankfeld: HEIGHT

**Tiefe** In diesem Feld geben Sie Tiefe (in mm) des Gestells ein, das Sie hinzufügen möchten.
**Technische Info:** Eingabe zwingend, Numerisch, Datenbankfeld: DEPTH

#### Erläuterung des Feldes im Bereich Vor Gestell# einfügen
**Kombobox** Die Kombobox enthält die Anzahl der Gestelle der jeweiligen Packmittelgruppe. D.h. wenn eine Packmittelgruppe fünf Gestelle beinhaltet, dann sind in der Kombobox die Zahlen 1, 2, 3, 4 und 5 aufgeführt. Sie haben so die Möglichkeit zu bestimmen, vor welchem dieser fünf Gestelle das neue Gestell eingefügt werden soll.

#### Erläuterung der Felder im Bereich Typ
**1 Seite (Typ L)** Aktivieren Sie diese Radiotaste, wenn es sich bei dem einzufügenden Gestell um ein L-Gestell handelt.

**2 Seiten (Typ A)** Aktivieren Sie diese Radiotaste, wenn es sich bei dem einzufügenden Gestell um ein A-Gestell handelt.

**Kiste** Aktivieren Sie diese Radiotaste, wenn es sich bei dem einzufügenden Gestell um eine nach Maß zu bauende Kiste handelt.

#### Erläuterung der Felder im Bereich Bezeichnung ID
**Gruppe** Die Kombobox ist mit dem Eintrag -Aktuell- vorbelegt und kann nicht geändert werden. In der darunter liegenden Kombobox sehen Sie den Namen der Gestellbezeichnung. Sie können mit der Maus in das Feld klicken und den Namen überschreiben. Wenn Sie den Dialog mit der Schaltfläche [OK] verlassen, wird der Name in der Tabelle geändert.

> **Kundenindividuelle Einstellungen**
> In Abhängigkeit von der jeweiligen Installation (Einstellungen in Ihrem Hause) können Sie in der Kombobox Gruppe die gewünschte Gestellgruppe auswählen. Innerhalb der Gestellgruppe dann das entsprechende Gestell. Das ist immer dann sinnvoll, wenn aus einer großen Anzahl von Gestellen oder Kisten gewählt werden soll. Das Verhalten wird dann von der A+W Software GmbH konfiguriert.

**Weitere Informationen zu Neue Gestell-Eigenschaften**
⇨ Konventionen, "Bedienoberfläche" auf Seite A-77
⇨ Konventionen, "Schaltflächen" auf Seite A-78

### Eigenschaften der Kiste ändern
**Pfad:** PackView > Bearbeiten ein > Menü Bearbeiten > Eigenschaften der Kiste ändern ...

*Abb. 1-87: Neue Gestell-Eigenschaften*

Der Menüpunkt Eigenschaften der Kiste ändern ... ist nur dann aktiv, wenn es sich bei dem selektierten Gestell um eine Kiste handelt. Sie haben dann die Möglichkeit, die vorhandenen Eigenschaften der Kiste zu ändern.

**Technische Info:** Datenbanktabelle: PMO_RACKS

#### Erläuterung der Felder im Bereich Abmessungen
**Breite Zuschlag** In diesem Feld geben Sie Breite (in mm) des Zuschlags der Kiste ein, um die die Kiste größer als die Ladung sein soll. Damit bleibt Platz für Füllmaterial zum Sichern der Ladung in der Kiste.

**Höhe Zuschlag** In diesem Feld geben Sie Höhe (in mm) des Zuschlags der Kiste ein, um die die Kiste größer als die Ladung sein soll. Damit bleibt Platz für Füllmaterial zum Sichern der Ladung in der Kiste.

**Tiefe Zuschlag** In diesem Feld geben Sie Tiefe (in mm) des Zuschlags der Kiste ein, um die die Kiste größer als die Ladung sein soll. Damit bleibt Platz für Füllmaterial zum Sichern der Ladung in der Kiste.

#### Erläuterung der Felder im Bereich Bezeichnung ID
**Gruppe** Die Kombobox ist mit dem Eintrag -Aktuell- vorbelegt und kann nicht geändert werden. In der darunter liegenden Kombobox sehen Sie den Namen der Gestellbezeichnung. Sie können mit der Maus in das Feld klicken und den Namen überschreiben. Wenn Sie den Dialog mit der Schaltfläche [OK] verlassen, wird der Name in der Tabelle geändert.

> **Kundenindividuelle Einstellungen**
> In Abhängigkeit von der jeweiligen Installation (Einstellungen in Ihrem Hause) können Sie in der Kombobox Gruppe die gewünschte Gestellgruppe auswählen. Innerhalb der Gestellgruppe dann das entsprechende Gestell. Das ist immer dann sinnvoll, wenn aus einer großen Anzahl von Gestellen oder Kisten gewählt werden soll. Das Verhalten wird dann von der A+W Software GmbH konfiguriert.

**Weitere Informationen zu Eigenschaft der Kiste ändern**
⇨ Tutorial, "Optimierung ansehen" auf Seite 1-979
⇨ Konventionen, "Bedienoberfläche" auf Seite A-77
⇨ Konventionen, "Schaltflächen" auf Seite A-78

### Eigenschaften Referenz-Einheiten
**Pfad:** PackView > Menü Ansicht > Eigenschaften Einheit

*Abb. 1-88: Eingeschaften Referenz-Einheiten*

Der Dialog gibt Ihnen Informationen zu der ausgewählten Scheibe. Es werden folgende Werte erläutert:

*   **Los/Sequenz:** Zeigt Ihnen die nach der Feinplanung für die Packmitteloptimierung ermittelte Losnummer sowie die Reihenfolge (Sequenz) der Scheibe innerhalb des Loses.
*   **Auftrag/Position:** Zeigt Ihnen die Auftrags-Nummer und die Positions-Nummer innerhalb des Auftrags. Bsp.: 639478/20 bedeutet: Auftrags-Nr.: 639478 und Positions-Nr.: 20.
*   **Breite x Höhe x Tiefe:** Zeigt Ihnen die Breite, die Höhe und die Dicke der Scheibe in mm.
*   **Gewicht:** Zeigt Ihnen das Gewicht der Scheibe in kg.
*   **Position (X, Y, Z):** Zeigt Ihnen die Koordinaten der Scheibe auf dem Gestell.

**Beispiel:**
*Abb. 1-89: Dialog: SQL-Analyse*

Die markierte Einheit hat die Koordinaten: 822.00, 51.00, 471.00. Das bedeutet, sie steht auf der X-Achse bei 822 mm (vom Bezugspunkt aus gesehen), 51 mm von der Gestellrückwand weg in einer Höhe von 471 mm.

### Info-Zeile am unteren Bildschirmrand
*Abb. 1-90: Info-Zeile am unteren Bildschirmrand*

Die Info-Zeile am unteren Bildschirmrand liefert Ihnen Informationen zu den Abmessungen und den Gewichten der jeweiligen Gestellseite. Mit der Info-Zeile sind Sie zu jeder Zeit über Maße und Gewichte der aktuell angezeigten Gestellseite auf dem Laufenden. Wechseln Sie zur anderen Gestellseite, ändert sich die Anzeige entsprechend.

Die Info-Zeile ist in drei Bereiche unterteilt:
*   Bereich A
*   Bereich B
*   Bereich C

#### Bereich A
Der Bereich A informiert Sie über die Ausdehnung der Einheiten pro Gestellseite.

*Abb. I-91: Ausdehnung*

Für die oben gezeigte Grafik bedeutet das: Das Gestell ist in einer Länge von 1136 mm, einer Höhe von 1270 mm und in einer Tiefe von 168 mm mit Einheiten bepackt.

> **Ausdehnung**
> Bei der Ausdehnung handelt es sich um die komplette Ausdehnung pro Gestellseite. D. h. auch Zwischenräume und Füllmaterial werden mit eingerechnet und angezeigt.

Werte werden in diesem Bereich nur angezeigt, wenn das Bemaßungs-Werkzeug nicht aktiv ist. Wurde das Bemaßungs-Werkzeug aktiviert, ist dieser Bereich leer bis ein Messergebnis angezeigt wird.

Zum Aktivieren des Bemaßungs-Werkzeuges stehen Ihnen folgende drei Möglichkeiten zur Verfügung:
*   Über das Menü: Ansicht > Bemaßungs-Werkzeug.
*   Durch Betätigen der Funktionstaste F4.
*   Durch Betätigen der Symbolschaltfläche. [ICON]
⇨ Softwarereferenz, “Symbol-Schaltflächen" auf Seite I-1045

| Menü |
| :--- |
| Tab. I-10 |

#### Bereich B
Der Bereich B informiert Sie über die Gewichtsverteilung in kg pro Gestell und pro Seite.

*Abb. 1-92: Gewicht in kg*

Für die oben gezeigte Grafik bedeutet das: Das Gestell hat ein Gesamtgewicht von 383 kg. Die Werte in den Klammern zeigen Ihnen die Gewichte pro Gestellseite. D.h. 183 kg für Gestellseite 1 und 200 kg für Gestellseite 2.

#### Bereich C
Der Bereich C informiert Sie über die Lastverteilung in % für die rechte und linke Seite des Gestells.

*Abb. 1-93: Gewicht in %*

Für die oben gezeigte Grafik bedeutet das: 51% der Last sind links und 49% rechts. Der Prozentwert berücksichtigt auch den Beitrag von weiter außen stehenden Einheiten im Verhältnis zu innen stehenden. Das kann zu deutlichen Unterschieden in der Lastverteilung führen (wie etwa 30 % zu 70%).

# A+W Realtime Optimizer

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
*   Anmerkungen zu diesem Dokument
*   Urheberrechte
*   Warenzeichen

#### Anmerkungen zu diesem Dokument
Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Realtime Optimizer gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.

Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von A+W Production.

#### Urheberrechte
© 2023, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

#### Warenzeichen
Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

## Tutorial

### Grundgedanken
Ein wesentliches Einsparpotential bei der Flachglasverarbeitung ist die optimale Ausnutzung der Lagerplatten beim Zuschnitt. Je weniger Verschnitt oder Restblätter, desto höher die Materialausnutzung und desto geringer die Materialkosten. Die Ansteuerung von Zuschnitttischen mit den optimierten Schnittbildern direkt aus der Optimierung beschleunigt den Arbeitsprozess.

A+W Realtime Optimizer basiert auf diesen beiden Grundgedanken:
*   Zuschnittoptimierung für den angeschlossenen Zuschnitttisch.
*   Übertragung von Schneidcode an den angeschlossenen Zuschnitttisch.

*Abb. J-1: Zuschnittoptimierung und Tischansteuerung*

### Leistungsmerkmale
A+W Realtime Optimizer unterstützt die genannten Grundgedanken mit folgenden Leistungsmerkmalen:
*   A+W Realtime Optimizer steuert Ihren Zuschnitt mit optimierten Feinplanungsdaten.
*   In ein Restblatt können automatisch Eil-, Bruch- oder Füllscheiben nachoptimiert werden.
*   Die Ansteuerung der Schneidtische erfolgt hauptsächlich online über die Kommunikationsprotokolle, die von den Tischherstellern unterstützt werden.
*   Eilscheiben, Bruchscheiben und Füller werden direkt am Zuschnitt optimiert.
*   Es besteht die Möglichkeit, bereits vorhandene Optimierungen für eine Tischoptimierung zu prüfen, aufzulösen und nochmals neu zusammenzufassen. Dabei können gemeinsam mit Bruch-, Füll- und Eilscheiben Optimierungen größerer Mengen erzeugt werden. Vorgegebene Reihenfolgen auf A-Böcken bleiben dabei erhalten.
*   A+W Production bietet bereits bei der Feinplanung die Möglichkeit, den Zuschnitt für jeden Lauf auf den geplanten Schneidtisch zu optimieren.
*   A+W Realtime Optimizer wird speziell für einen Schneidtisch konfiguriert und kann die für diesen Schneidtisch vorgeplanten und bereits optimierten Läufe mit dem Schneidcode an den Schneidtisch übertragen.
*   Wenn der erforderliche Maschinencode an den Schneidtisch übermittelt wurde, dann kann das Brechbild mit XTV angezeigt werden.

### Arbeiten mit A+W Realtime Optimizer
In diesem Themenblock lernen Sie die Arbeitsweise des A+W Realtime Optimizer kennen.
Der Themenblock beinhaltet folgende Schulungseinheiten:
*   Datenübernahme
    *   Anbindung an A+W Production
    *   Verwendung als stand alone-System

#### Überblick
**Lernziele**
*   Die Datenübernahme kennenlernen und verstehen.
*   Die Anbindung an A+W Production kennenlernen und verstehen.
*   Die Verwendung als stand alone-System kennenlernen und verstehen.

**Nutzen**
Zum optimalen Arbeiten mit dem A+W Realtime Optimizer müssen die Daten korrekt übernommen werden.

**Definitionen**
*   **Vorsysteme**: Liefern Aufträge (Läufe), in denen Stammdaten und Zuschnittoptimierungen enthalten sind.
*   **Stand-alone Variante**: Hier erfolgt die Datenübernahme mithilfe von save-Dateien, die in einem bestimmten Verzeichnis zur Verfügung gestellt werden.
*   **Restelager**: Mit einem Restelager-Magazin werden Restplatten am Zuschnitttisch verwaltet.

**Merke**
*   **A+W Realtime Optimizer**: Kann an alle gängigen Zuschnitttische angepasst werden.
*   **Stand-alone Variante**: Der A+W Realtime Optimizer kann auch stand-alone eingesetzt werden.
*   **Anbindung**: Die Datenübernahme wird im Rahmen der Installation von A+W Mitarbeitern konfiguriert.

#### Datenübernahme
Je nach dem, welches Vorsystem verwendet wird, erfolgt die Datenübernahme aus dem Vorsystem voll- oder halbautomatisch. Vorsysteme liefern an A+W Realtime Optimizer Aufträge (Läufe), in denen Stammdaten und Zuschnittoptimierungen enthalten sind.

*Abb. J-2: Übersicht der Arbeiten mit A+W Realtime Optimizer, die in kursiver Schrift dargestellten Arbeiten kommen nur bei stand alone-Systemen zum Einsatz*

Die vielfältigen Konfigurationsmöglichkeiten erlauben folgende Einsatzmöglichkeiten des A+W Realtime Optimizer:
*   Eingebettet in eine A+W Production oder A+W Business Pro-Umgebung.
*   Anpassung an alle gängigen Zuschnitttische.
*   Anbindung an ein Restelager.
*   Einsatz als stand alone-System.

Die Konfiguration und Installation für die verschiedenen Einsatzmöglichkeiten wird von A+W-Mitarbeitern durchgeführt.

Mögliche Vorsysteme sind:
*   A+W Production
*   A+W Business Pro

> **Anbindung an ein Vorsystem**
> Welches Vorsystem bei Ihnen eingesetzt wird und die Art und Weise, wie Daten übernommen werden, wird im Rahmen der Installation von A+W-Mitarbeitern konfiguriert.

*Abb. J-3: Datenübernahme in A+W Realtime Optimizer*

Wenn A+W Realtime Optimizer mit A+W Production zusammenarbeitet, dann verwendet A+W Realtime Optimizer die A+W Production-Datenbank mit. Kommt ein anderes Vorsystem zum Einsatz, dann benötigt A+W Realtime Optimizer eine leere A+W Production-Datenbank. Stammdaten und Optimierungen, die in den Läufen des Vorsystems enthalten sind, werden von A+W Realtime Optimizer in die leere A+W Production-Datenbank übernommen. Dabei werden die Daten geprüft.

Daten, die bei der Übernahme einen Fehler verursacht haben, werden abgewiesen. Im erstellten Fehlerprotokoll können Sie nachvollziehen, welche Datensätze warum abgewiesen wurden. Diese Daten können Sie dann nachbearbeiten.

##### Anbindung an A+W Production
Bei der Anbindung von A+W Realtime Optimizer an ein bestehendes A+W Production-System erfolgt ein vollautomatischer Datenaustausch. Stammdaten, Läufe, Bruch, Eil- und Füllaufträge werden direkt aus der A+W Production-Datenbank genommen. Darüber hinaus werden Statusmeldungen für die einzelnen Läufe in die Datenbank zurückgeschrieben.

##### Stammdaten
Wenn bei der Konfiguration der Zugang zu den Stammdaten freigegeben wurde, dann können diese eingesehen und bearbeitet werden.
Zu den Stammdaten zählen:
*   Artikel
*   Glasarten
*   Tische
*   Optimierungsparameter
*   Lagerplatten
Beschrieben sind diese Stammdaten und das Arbeiten damit im Part Feinplanung des Anwenderhandbuches A+W Production.

##### Verwendung als stand alone-System
A+W Realtime Optimizer wird bei der Installation mit einer leeren A+W Production-Datenbank eingerichtet. Diese Datenbank wird beim Import von Läufen nach und nach mit Stammdaten gefüllt.

Beim stand alone-System erfolgt die Datenübernahme mit Hilfe von save-Dateien, die A+W Realtime Optimizer in einem bestimmten Verzeichnis zur Verfügung gestellt werden müssen. Die save-Dateien müssen eine definierte Struktur einhalten und werden üblicherweise im Arbeitsverzeichnis ...\Xopton\import\work\\*save.\\* bereit gestellt. Eingelesene Daten werden aus dem Arbeitsverzeichnis entfernt und in ein Archivverzeichnis verschoben.

##### Optimierungen importieren
Die Funktion Optimierungen importieren ist nur bei A+W Realtime Optimizer stand alone-Versionen erforderlich und möglich.
A+W Realtime Optimizer kann nur dann einen Zuschnitttisch mit Zuschnittdaten versorgen oder Tischoptimierungen erstellen, wenn Läufe aus einem vorgelagerten System zur Verfügung gestellt werden. Wenn solche Läufe bereitgestellt werden, dann kann A+W Realtime Optimizer diese zur Weiterbearbeitung importieren.

Folgende Arbeitsschritte können Sie im Rahmen der Importierung von Läufen durchführen:
*   Import einschalten.
*   Import ausschalten.
*   Auf Fehlermeldungen reagieren.

**Import einschalten**
1.  Öffnen Sie den Dialog Import. Wählen Sie dazu im Menü Ansicht > Import.
2.  Um den Import zu starten, betätigen Sie die Schaltfläche [Start].
    A+W Realtime Optimizer prüft, ob im Arbeitsverzeichnis Importdateien vorliegen. Werden solche Dateien gefunden, so werden diese Daten in die Datenbank importiert und die Importdateien werden ins Archiv-Verzeichnis verschoben.
    Importierte Läufe werden in den Dialogen Wählen Sie einen Lauf aus und Selektieren Sie die zu optimierenden Gläser zur Weiterbearbeitung zur Verfügung gestellt.
    Die Schaltfläche [Start] wechselt die Darstellung auf [Stop].
3.  Schließen Sie den Dialog. Betätigen Sie dazu die Schaltfläche [Schließen].
    A+W Realtime Optimizer überwacht das Arbeitsverzeichnis so lange, bis die Importfunktion ausgeschaltet wird.
    Wenn während des Imports Fehler auftreten, dann werden diese protokolliert und die entsprechenden Läufe nicht importiert. Fehler können manuell nachbearbeitet werden.

**Import ausschalten**
1.  Öffnen Sie den Dialog Import. Solange der Import eingeschaltet ist, befindet sich der Dialog in minimierter Darstellung links unten im A+W Realtime Optimizer-Dialog.
2.  Um den Import zu beenden, betätigen Sie die Schaltfläche [Stopp].
    Neu ins Arbeitsverzeichnis gespeicherte Importdateien verbleiben dort unbearbeitet.
    Die Schaltfläche [Stopp] wechselt die Darstellung auf [Start].
3.  Schließen Sie den Dialog. Betätigen Sie dazu die Schaltfläche [Schließen].

**Auf Fehlermeldungen reagieren**
Wenn während des Imports Fehler auftreten, dann werden diese protokolliert und die entsprechenden Läufe nicht importiert.

Der Import wird nur dann gestoppt, wenn Datenverlust droht. Dies ist z. B. dann der Fall, wenn eine bereits vorhandene Optimierung überschrieben werden soll. Je nach Konfiguration erscheint eine entsprechende Fehlermeldung.

1.  Beantworten Sie die Frage im Fehlermeldungs-Dialog xopt-on.
    Wählen Sie dazu die entsprechende Schaltfläche [Ja] oder [Nein].
    Der Datenimport wird fortgesetzt.
2.  Öffnen Sie den Dialog Fehlermeldungen. Wählen Sie dazu im Menü Ansicht > Fehlermeldungen.
3.  Prüfen Sie die Fehlermeldungen und reagieren Sie entsprechend.

**Ergänzende Informationen**
⇨ "Auf Fehlermeldungen reagieren" auf Seite J-1072
⇨ Softwarereferenz, “Fehlermeldungen" auf Seite J-1206

### Erfassung
In diesem Abschnitt wird Ihnen gezeigt, wie Sie mit der Erfassung umgehen.
Der Themenblock beinhaltet folgende Schulungseinheiten:
*   Bruch, Eilscheiben und Füllaufträge
*   Manuelle Planerstellung
*   Chargen-Editor

#### Überblick
**Lernziele**
*   Bruchscheiben und den Umgang damit kennen lernen und verstehen.
*   Eilscheiben und den Umgang damit kennen lernen und verstehen.
*   Füllaufträge und den Umgang damit kennen lernen und verstehen.

**Nutzen**
Unter Verwendung von Bruch-, Eilscheiben und Füllaufträgen können Sie den Verschnitt erheblich verbessern.

**Definitionen**
*   **Bruchscheibe**: Eine Scheibe, die beim Zuschnitt kaputt gegangen ist.
*   **Eilscheibe**: Eine Scheibe, die schnell geschnitten werden muss.
*   **Füllauftrag**: Dienen dazu, Kapazitäten und Material effizient auszunutzen.

**Merke**
*   **Bruchscheiben**: Können manuell mit dem A+W Realtime Optimizer oder an einer anderen Stelle einer vernetzten Produktion erfasst werden.
*   **Eilscheiben**: Werden mit dem A+W Realtime Optimizer angelegt und in der Datenbank gespeichert.
*   **Füllaufträge**: Können nur verwendet werden, wenn der A+W Realtime Optimizer mit einem A+W Production -System verwendet wird.

#### Bruch, Eilscheiben und Füllaufträge
Bruch kann manuell mit A+W Realtime Optimizer oder an einer anderen Stelle einer vernetzten Produktion erfasst werden. Je nach Konfiguration werden Bruchscheiben direkt im Bruchpool von A+W Realtime Optimizer angezeigt. Bei nächster Gelegenheit werden Bruchscheiben automatisch auf das Restblatt optimiert oder manuell (je nach Konfiguration) in eine Tischoptimierung integriert.

Eilscheiben werden mit A+W Realtime Optimizer angelegt und in der Datenbank gespeichert. Eilscheiben können ebenfalls bei der nächsten Tischoptimierung, die eine passenden Glasart und Dicke verwendet, in die Optimierung integriert werden.

Füllaufträge können nur verwendet werden, wenn A+W Realtime Optimizer mit einem A+W Production-System verwendet wird. Füllaufträge werden dann direkt aus der A+W Production-Datenbank entnommen.

*Abb. J-4: Datenerfassung und -verarbeitung in A+W Realtime Optimizer*

#### Scheiben manuell erfassen
Zusätzlich zu den Läufen aus einem Vorsystem, können in A+W Realtime Optimizer Scheiben erfasst, in Tischoptimierungen eingebracht und zum Schneidtisch übertragen werden.

Mit folgende Arbeitsschritten können Sie unterschiedliche Scheiben manuell erfassen oder wieder löschen:
*   Eilscheiben erfassen.
*   Eilscheiben bearbeiten.
*   Eilscheiben löschen.
*   Bruchscheiben erfassen.
*   Bruchscheiben löschen.

##### Eilscheiben erfassen
1.  Öffnen Sie dein Dialog Eilscheiben. Wählen Sie dazu im Menü Erfassung > Eilscheiben. Im Dialog Eilscheiben werden alle erfassten und noch nicht in einer Optimierung verwendeten Eilscheiben angezeigt.
2.  Öffnen Sie den Dialog Eilscheibeneingabe. Betätigen Sie dazu die Schaltfläche [Hinzufügen].
3.  Wählen Sie im Feld Glasart die Glasart, für die Sie Eilscheiben erfassen wollen. Wenn für die Glasart mehrere Dicken möglich sind, dann geben Sie im Feld Dicke die Dicke an, die Sie benötigen.
4.  Geben Sie im Feld Bock ein, auf welchen Abstellplatz die Eilscheiben nach dem Zuschnitt gestellt werden. Je nach Arbeitsorganisation kann dieses Feld auch leer bleiben.
5.  Geben Sie im Feld Menge ein, wieviele Scheiben Sie erfassen wollen.
6.  Wählen Sie im Feld Modell-Nr. die entsprechende Nummer, wenn Sie Modellscheiben erfassen wollen.
    Wenn Sie Modellscheiben erfassen wollen, können Sie die Form der Modellscheiben bearbeiten. Betätigen Sie dazu die Schaltfläche [^]. Es ist auch möglich für Eilscheiben eine freie Form zu hinterlegen. Geben Sie dazu die Modelnummer 99 ein. Wählen Sie anschließend aus dem Katalog-Verzeichnis die entsprechende SN-Datei aus (diese muss vorher separat via CAD Designer Shapes erfasst und als Block-Ind-Datei exportiert worden sein).
7.  Geben Sie in den Feldern Breite und Höhe die Maße der Scheiben ein, die Sie erfassen wollen. Wenn Sie eine Modellscheibe erfasst haben, dann werden in diesen Feldern automatisch die Maße des umschreibenden Rechtecks angezeigt.
8.  Speichern Sie die Eilscheibeneingabe. Betätigen Sie dazu die Schaltfläche [OK].
    Die erfassten Daten werden gespeichert und in der Liste angezeigt.
9.  Erfassen Sie weitere Scheiben oder schließen Sie den Dialog.
    Um weitere Scheiben zu erfassen, wiederholen Sie die Arbeitsschritte ab Schritt 2.
    Um den Dialog zu schließen, betätigen Sie die Schaltfläche [Beenden].

##### Eilscheiben bearbeiten
1.  Öffnen Sie den Dialog Eilscheiben-Eingabe. Wählen Sie dazu im Menü Erfassung > Eilscheiben. Im Dialog Eilscheiben werden alle erfassten und noch nicht in einer Optimierung verwendeten Eilscheiben angezeigt.
2.  Markieren Sie die Zeile in der Liste der Eilscheiben, die Sie bearbeiten möchten.
3.  Betätigen Sie die Schaltfläche [Bearbeiten]. Es öffnet sich der Dialog Eilscheiben-Eingabe. Die Felder enthalten die Werte der Eilscheibe, die Sie ändern möchten.
4.  Nehmen Sie die Änderungen vor und verlassen Sie den Dialog mit der Schaltfläche [OK].

##### Eilscheiben löschen
1.  Öffnen Sie den Dialog Eilscheiben-Eingabe. Wählen Sie dazu im Menü Erfassung > Eilscheiben. Im Dialog Eilscheiben werden alle erfassten und noch nicht in einer Optimierung verwendeten Eilscheiben angezeigt.
2.  Markieren Sie eine Zeile in der Liste der Eilscheiben.
3.  Betätigen Sie die Schaltfläche [Löschen]. Die markierte Eilscheibe wird gelöscht.
4.  Schließen Sie den Dialog. Betätigen Sie dazu die Schaltfläche [OK].

##### Bruchscheiben erfassen
Wenn Sie am Zuschnitttisch mit A+W Production Terminal (XTV) arbeiten, dann kann Bruch direkt am Tisch erfasst werden und wird automatisch an A+W Realtime Optimizer übertragen. Bruch kann aber auch manuell erfasst werden:
1.  Öffnen Sie den Dialog Brucherfassung. Wählen Sie dazu im Menü Zuschnitt > Bruchpool > [Hinzufügen].
2.  Geben Sie im Bereich Teile-ID die Auftragsnummer, Positionsnummer und Unterpositionsnummer an, zu der die zu Bruch gegangenen Scheiben gehören.
3.  Wenn Sie mit der BDE arbeiten, können Sie einen Bruchgrund angeben. Wählen Sie dazu den entsprechenden Eintrag in der Kombobox Bruchgrund.
4.  Speichern Sie die Eingaben. Betätigen Sie dazu die Schaltfläche [Speichern].

##### Bruchscheiben löschen
1.  Öffnen Sie dein Dialog Bruchpool. Wählen Sie dazu im Menü Zuschnitt > Bruchpool. Im Dialog Bruchpool werden alle erfassten und noch nicht in einer Optimierung verwendeten Bruchscheiben angezeigt.
2.  Markieren Sie eine oder mehrere Zeilen in der Liste der Bruchscheiben.
3.  Betätigen Sie die Schaltfläche [Löschen]. Die markierten Bruchscheiben werden gelöscht.
4.  Schließen Sie den Dialog. Betätigen Sie dazu die Schaltfläche [Schließen].

> **Bruchscheiben buchen**
> Über die Schaltfläche [Buchen F5] werden die Bruchscheiben wieder der Produktion zugeführt. Haben Sie versehentlich Scheiben zu Bruch gemeldet, können Sie diese ebenfalls über die Schaltfläche als Gut melden.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Modell-Erfassung" auf Seite J-1196
⇨ Softwarereferenz, "Eilscheiben" auf Seite J-1144
⇨ Softwarereferenz, "Bruchpool" auf Seite J-1192
⇨ Softwarereferenz, “Brucherfassung" auf Seite J-1194

#### Manuelle Planerstellung
Mit dieser Option haben Sie die Möglichkeit, einen rein manuellen Plan zu erstellen und als Tischoptimierung in der Datenbank zu speichern. Der manuelle Plan kann nach der Erstellung erneut editiert und geändert werden. Dies geschieht mithilfe des Moduls A+W PlanEditor. Nähere Erläuterungen zu diesem Modul finden Sie in der entsprechenden Dokumentation. Es ist keine Barcode-Information für den manuellen Plan verfügbar.

##### So erstellen Sie einen neuen Plan
1.  Wählen Sie dazu im Menü Eingabe > Manueller Plan. Es öffnet sich der Dialog Manuelle Planerstellung für Tisch ....
2.  Wählen Sie im Bereich Glasarten die Glasart aus, für die Sie einen neuen Plan erstellen möchten.
3.  Wählen Sie auf der linken Seite im Bereich Lagerplatten das Lagermaß aus, welches für das manuelle Schnittbild als Grundlage verwendet werden soll.
4.  Definieren Sie ggf. im Bereich Restplatten die Höhe und Breite, welche als Restplatte angelegt werden soll.
5.  Klicken Sie auf die Symbol-Schaltfläche [Neu]. Es öffnet sich der A+W PlanEditor.
6.  Über das Kontext-Menü können Sie nun die gewünschten Scheiben erfassen. Wählen Sie dazu die Option Einfügen und erfassen Sie anschließend die gewünschten Scheibendaten.
7.  Über Datei > Speichern unter, können Sie den Scheidplan als Datei speichern.
8.  Mittels Ausgabe > AWC erfolgt die Übergabe an den Zuschnitt.

##### So editieren Sie einen manuellen Plan
1.  Um einen manuell erfassten Schneidplan zu ändern, wählen Sie im Menü Eingabe > Manuellen Plan. Es öffnet sich der Dialog Manuelle Planerstellung für Tisch .... Im unteren Bereich Plan erscheint der im Vorfeld manuell erfasste Plan.
2.  Mittels der Schaltfläche [Editieren] öffnen Sie den vorher erstellten Plan und können diesen editieren.
3.  Vergessen Sie nicht, die Änderungen zu speichern oder mittels Ausgabe > AWC die Daten zum Schneiden freizugeben.

##### So wählen Sie einen manuell erfassten Plan zum Zuschnitt aus
1.  Einen manuell erfassten Plan können Sie nur via Zuschnitt direkt zuschneiden.
2.  Über die Schaltfläche [Schneiden] können Sie alle optimierten und für den Zuschnitt vorbereiteten Läufe auswählen.
3.  Der manuell erstellte Plan erscheint in der Liste der verfügbaren Läufe mit einer Laufnummer >15000 und hat die Zusatzinformation PlanEdit.
4.  Wählen Sie den Lauf aus und bereiten Sie ihn für den Zuschnitt vor (Schaltfläche [Optionen]) oder schneiden Sie ihn direkt (Schaltfläche [Zuschnitt]).

**Ergänzende Informationen**
⇨ Softwarereferenz, "Manuelle Planerstellung" auf Seite J-1151

#### Chargen-Editor
Über diesen Dialog haben Sie die Möglichkeit, eine Chargen-Nummer zu hinterlegen. Mit Hilfe der aktivierten Checkbox können Sie die eingegebene Chargen Nummer auf die nachfolgenden Lagerplatten der gleichen Glasart/Dicke vererben. Die letzte Chargen Nummer wird pro Glasart/Dicke/Lagerplatte gespeichert. Mit diesem Wert wird bei dem nächsten Aufruf des Editors das Eingabefeld wieder vorbelegt. Die Zuweisung wirkt immer auf das ausgewählte Lagermaß (und bei Vererbung auf die darunterliegenden).

Es ist auch möglich, über diesen Editor eine gesetze Charge wieder zu löschen (inklusive Vererbung).

Läuft der Zuschnittsprozess auf eine Lagerplatte ohne Chargenzuordnung, so muss der Mitarbeiter am Brechtisch zunächst eine Chargen-Nummer eingeben. Hierzu erscheint wieder der Dialog Chargen-Editor mit einer entsprechenden Info im A+W Production Terminal (XTV). Die eingegebene Chargen Nummer wird beim Weiterschalten des A+W Production Terminal (XTV) für alle Scheiben des jeweiligen Lagerblattes verbucht.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Chargen-Editor" auf Seite J-1154

### Optimierung
In diesem Abschnitt wird Ihnen gezeigt, wie Sie mit der Optimierung umgehen.
Der Themenblock beinhaltet folgende Schulungseinheiten:
*   Tischoptimierungen
*   Schnelloptimierung erstellen
*   Verlinken von Läufen
*   Tischansteuerung

#### Überblick
**Lernziele**
*   Tischoptimierungen kennenlernen und verstehen.
*   Schnelloptimierungen kennenlernen und verstehen.
*   Das Verlinken von Restplatten kennenlernen und verstehen.
*   Tischansteuerung kennenlernen und verstehen.

**Nutzen**
Je effizienter die Optimierung arbeiten kann, umso höher ist die Ausbeute. Das spart Geld.

**Definitionen**
*   **Tischoptimierungen**: Sind Optimierungen, die mit A+W Realtime Optimizer erzeugt werden.
*   **Schnelloptimierung**: Platten, die noch nicht an den Tisch gesandt wurden, können komplett aufgelöst und neu optimiert werden.

**Merke**
*   **Lauf**: Ein Lauf ist eine Zusammenstellungen von Gläsern aus einem oder mehreren Aufträgen, welche in der Optimierung und Produktion gemeinsam betrachtet und produziert werden sollen (bspw. gleiche Tour, gleicher Kunde, gleiche Glasarten, gleiche Produktionstermine). Die Optimierungen von vorgelagerten Systemen liegen in Form von Läufen vor.
*   **Los**: Ein Teil / eine Glasart eines Laufes, welcher unter gleichen Bedingungen zur gleichen Zeit in der Produktion bearbeitet / geschnitten werden soll (bspw. alles Float 4 eines Laufes).
*   **Tischansteuerung**: Bei der Installation wird festgelegt, welcher Zuschnitttisch mit einem A+W Realtime Optimizer angesteuert werden.
*   **Bruchscheiben**: Können entweder in der Nachoptimierung am Ende eines zu schneidenden Laufes geschnitten werden oder landen im Bruchpool und können zusammen mit dem nächsten Lauf geschnitten werden.

#### Tischoptimierungen
Tischoptimierungen sind Optimierungen, die mit A+W Realtime Optimizer erzeugt werden. Vorgelagerte Systeme liefern bereits fertige Optimierungen, die mit A+W Realtime Optimizer aufgelöst und neu zusammengestellt werden können. Dabei können so viele Läufe zusammengefasst werden, wie Platz für die benötigten Abstellplätze am Zuschnitttisch in einer Produktion vorhanden ist.

Bei der Erstellung von Tischoptimierungen können Sie Restblätter auf dem Zuschnitttisch berücksichtigen, unterschiedliche Lagerplatten verwenden oder ein Restelager nutzen. Bruch, Eilscheiben oder Füllaufträge können ausgeschlossen oder mit einbezogen werden.

Erstellte Tischoptimierungen werden in der Datenbank abgespeichert und bei Bedarf zum Zuschnitt aufgerufen.

##### Tischoptimierungen erstellen
Zum Erstellen neuer Tischoptimierungen müssen folgende Arbeitsschritte durchgeführt werden:
*   Glasart und Lauf für eine Tischoptimierung auswählen.
*   Tischoptimierung erstellen.

**Glasart und Lauf für eine Tischoptimierung auswählen**
1.  Öffnen Sie den Dialog Selektieren Sie die zu optimierenden Gläser. Wählen Sie dazu Optimierung > Tischoptimierung.
2.  Wählen Sie in der Liste Glasart die Glasart aus, für die Sie eine Optimierung erstellen wollen. In der Liste Glasart wird ihnen angezeigt, ob für eine Glasart im A+W Realtime Optimizer besondere Aufträge (Bruchscheiben, Eilscheiben, etc.) existieren.
    Wenn Sie eine Glasart wählen, für die Bruchscheiben oder Eilaufträge existieren, so werden diese Bruchscheiben oder Eilaufträge automatisch (wenn konfiguriert) in die zu erstellende Tischoptimierung integriert.
    Wenn Ihr System für die Zusammenarbeit mit einem Restelager-Magazin konfiguriert wurde, dann wird in dieser Liste angezeigt, ob für die entsprechende Glasart ein Restplatte verfügbar ist.
    In der Liste Verfügbare Optimierungen werden alle Läufe angezeigt, in denen Optimierungen für die in der Liste Glasart gewählte Glasart und Dicke enthalten sind.
3.  Markieren Sie die Checkbox Erlaube Handzuschnitt, wenn Sie auch die Glasarten anzeigen wollen, die nur für den Handzuschnitt vorgesehen sind.
4.  Wählen Sie in der Liste Verfügbare Optimierungen die Läufe aus, die Sie zu einer Tischoptimierung zusammenfassen wollen.

> **Nur Bruch- und Eilscheiben auswählen**
> Wenn für die gewählte Glasart Bruch- oder Eilscheiben vorhanden sind, dann können Sie diese Scheiben ohne einen weiteren Lauf optimieren. Wählen Sie in diesem Fall keinen Lauf aus der Liste aus.
>
> Wenn sie einen Lauf markiert haben, aber keinen Lauf wählen wollen, dann wechseln Sie die gewählte Glasart. Bei erneuter Auswahl der gewünschten Glasart ist kein Lauf markiert.

5.  Klicken Sie auf [Auswählen], wenn Sie die ausgewählten Läufe zu einer Tischoptimierung zusammenstellen wollen.
    Der Dialog wird geschlossen. Der Dialog Tischoptimierung öffnet sich mit dem Register Optimieren und zeigt die gewählten Läufe an.

**Tischoptimierung erstellen**
1.  Stellen Sie sicher, dass mit dem vorherigen Arbeitsschritt So wählen Sie Läufe für eine Tischoptimierung aus Läufe für die Tischoptimierung ausgewählt wurden.
    Der Dialog Tischoptimierung wird mit dem Register Optimieren angezeigt.
2.  Wählen Sie die erforderlichen Optimierungsparameter.
3.  Wählen Sie die erforderlichen Parameter im Register Lagerplatten.
4.  Wählen Sie die erforderlichen Parameter im Register Füller.
5.  Um die Optimierung zu erstellen, wechseln Sie wieder in das Register Optimieren und betätigen Sie die Schaltfläche [Optimieren].
    Die Berechnung der Optimierung startet, der Dialog wird ausgeblendet und die Berechnung läuft im Hintergrund. So lange die Berechnung läuft, können Sie weitere Arbeiten mit A+W Realtime Optimizer durchführen.
    Sobald das Ergebnis der Optimierung vorliegt, wird der Dialog automatisch wieder eingeblendet. Das Optimierungsergebnis wird im Register Übersicht angezeigt.
6.  Um die Optimierung abzuspeichern, betätigen Sie die Schaltfläche [Speichern].
    Die Optimierung steht jetzt im Dialog Wählen Sie einen Lauf aus zur Auswahl bereit und kann an den Schneidtisch übertragen werden.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Selektieren Sie die zu optimierenden Gläser" auf Seite J-1157
⇨ Softwarereferenz, “Optimieren" auf Seite J-1164
⇨ Softwarereferenz, "Restplatten und Lagerplatten" auf Seite J-1166
⇨ "Läufe zum Zuschnitt auswählen" auf Seite J-1094

#### Ergebnis der Tischoptimierung prüfen und bearbeiten
Tischoptimierungen, die noch nicht zum Schneidtisch übertragen wurden, können jederzeit geprüft werden. Sollen Tischoptimierungen geändert oder um Bruch-, Eil- oder Füllscheiben ergänzt werden oder sollen ganze Läufe zugefügt oder daraus gelöscht werden, so muss die gesamte Optimierung aufgelöst und neu erstellt werden.

Folgende Arbeitsschritte können beim Erstellen einer Tischoptimierung durchgeführt werden:
*   Andere Lagerplatten für die Optimierung wählen.
*   Restblatt der vorherigen Optimierung verwenden.
*   Füllaufträge zur Optimierung zufügen.

Sobald eine Tischoptimierung gespeichert wurde, können keine Änderungen mehr durchgeführt werden.

##### Andere Lagerplatten für die Optimierung wählen
1.  Wählen Sie im Dialog Tischoptimierung das Register Lagerplatten.
    In der rechten Liste werden alle Lagerplatten angezeigt, die in den Stammdaten für die Glasart und Dicke des Laufes definiert wurden und dem Schneidtisch zur Verfügung stehen.
2.  Markieren Sie die Lagerplatten, die A+W Realtime Optimizer für die Zuschnittoptimierung verwenden kann.
    Während der Optimierung prüft A+W Realtime Optimizer, mit wievielen Platten welcher Größe das beste Optimierungsergebnis erzielt wird.
3.  Um die Optimierung zu erstellen, wechseln Sie in das Register Optimieren und betätigen Sie die Schaltfläche [Start].
4.  Um die Optimierung abzuspeichern, betätigen Sie die Schaltfläche [Speichern].

##### Restblatt der vorherigen Optimierung verwenden
1.  Wählen Sie im Dialog Tischoptimierung das Register Lagerplatten.
    Wenn auf dem Schneidtisch noch ein Restblatt der gleichen Glasart und Dicke liegt, wie in der angezeigten Optimierung, dann können Sie dieses Restblatt in die Tischoptimierung integrieren.
2.  Geben Sie die Höhe und Breite des Restblatts auf dem Schneidtisch im Bereich Restblatt ein.
3.  Um die Optimierung zu erstellen, wechseln Sie in das Register Optimieren und betätigen Sie die Schaltfläche [Start].
4.  Um die Optimierung abzuspeichern, betätigen Sie die Schaltfläche [Speichern].

##### Füllaufträge zur Optimierung zufügen
1.  Wählen Sie im Dialog Tischoptimierung das Register Füller.
    In der rechten Liste werden alle Füllaufträge angezeigt, die für die Glasart des Laufes definiert wurden.
2.  Markieren Sie die Füllaufträge, die Sie in die Tischoptimierung integrieren wollen.
    Idealer Weise werden Füllaufträge so verwendet, dass möglichst geringer Verschnitt oder Restblätter entstehen.
3.  Um die Optimierung zu erstellen, wechseln Sie in das Register Optimieren und betätigen Sie die Schaltfläche [Optimieren].
4.  Wiederholen Sie das Zufügen oder Entfernen von Füllaufträgen so lange, bis das für Sie optimale Ergebnis ermittelt wurde.
5.  Um die Optimierung abzuspeichern, betätigen Sie die Schaltfläche [Speichern].

**Ergänzende Informationen**
⇨ "Tischoptimierung auflösen" auf Seite J-1086

#### Tischoptimierung auflösen
Tischoptimierungen können nur dann aufgelöst werden, wenn sie nach dem Erstellen gespeichert wurden. Solange der Dialog Tischoptimierung noch mit einer Tischoptimierung geöffnet ist, und diese Optimierung nicht gespeichert wurde, kann die Optimierung durch betätigen der Schaltfläche Abbrechen verworfen werden.

Wenn Sie eine Tischoptimierung auflösen, dann werden die enthaltenen Läufe wieder in die Laufliste gestellt. Evtl. enthaltene Bruch-, Eil- oder Füllscheiben stehen in den entsprechenden Pools (Sammelbehälter) für neue Optimierungen wieder zur Verfügung.

Optimierungen, deren Zuschnitt bereits begonnen und dann abgebrochen wurde, können ebenfalls aufgelöst werden. Läufe, bei denen bereits Scheiben geschnittenen wurden, werden zurückgesetzt und so behandelt, als ob noch kein Zuschnitt erfolgt wäre.

##### Erstellte und gespeicherte Tischoptimierungen auflösen
1.  Öffnen Sie den Dialog Zurücksetzen eines Zuschnitt Laufes.
    Wählen Sie dazu im Menü Optimierung > Zurücksetzen.
    Im Dialog Zurücksetzen eines Zuschnitt Laufes wird eine Liste aller Läufe angezeigt, für die Sie Statusänderungen vornehmen können. Die Liste erscheint nach Laufnummern sortiert. Tischoptimierungen werden als Lauf im Nummernbereich ab 15000 (konfigurierbar) angezeigt.
2.  Wählen Sie die Tischoptimierung, die Sie auflösen wollen. Markieren Sie dazu im Nummernbereich ab 15000 den entsprechenden Lauf. Sie können mehrere Tischoptimierungen markieren und gleichzeitig auflösen.
3.  Um die Tischoptimierung aufzulösen, betätigen Sie die Schaltfläche [OK]. Es erscheint eine Sicherheitsabfrage.
4.  Bestätigen Sie die Sicherheitsabfrage. Wählen Sie dazu die Schaltfläche [Ja].
    Die Läufe und Scheiben der gewählten Tischoptimierung stehen wieder für neue Tischoptimierungen zur Verfügung. Wurden in der Tischoptimierung Remasterplatten verwendet, so stehen diese nach der Auflösung der Optimierung wieder zur Verfügung.

**Ergänzende Informationen**
⇨ "Tischoptimierungen erstellen" auf Seite J-1083

#### Tischoptimierungen verlinken
Zur Verbesserung des Verschnitts haben Sie die Möglichkeit, Tischoptimierungen miteinander zu verlinken. Sie können nur Tischoptimierungen der gleichen Glasart miteinander verlinken. D. h., die Tischoptimierungen müssen vorhanden sein.

Zum Verlinken von Tischoptimierungen müssen folgende Arbeitsschritte durchgeführt werden:
*   Glasart und Lauf für eine Tischoptimierung auswählen.
*   Tischoptimierung erstellen.

##### Tischoptimierungen verlinken
1.  Öffnen Sie den Dialog Selektieren Sie die zu optimierenden Gläser. Wählen Sie dazu Optimierung > Tischoptimierung.
2.  Wählen Sie in der Liste Glasart die Glasart aus, für die Sie eine Optimierung erstellen wollen. In der Liste Glasart wird ihnen angezeigt, ob für eine Glasart im A+W Realtime Optimizer besondere Aufträge (Bruchscheiben, Eilscheiben, etc.) existieren.
    Wenn Sie eine Glasart wählen, für die Bruchscheiben oder Eilaufträge existieren, so werden diese Bruchscheiben oder Eilaufträge automatisch (wenn konfiguriert) in die zu erstellende Tischoptimierung integriert.
    Wenn Ihr System für die Zusammenarbeit mit einem Restelager-Magazin konfiguriert wurde, dann wird in dieser Liste angezeigt, ob für die entsprechende Glasart ein Restplatte verfügbar ist.
    In der Liste Verfügbare Optimierungen werden alle Läufe angezeigt, in denen Optimierungen für die in der Liste Glasart gewählte Glasart und Dicke enthalten sind.
3.  Markieren Sie die Checkbox Erlaube Handzuschnitt, wenn Sie auch die Glasarten anzeigen wollen, die nur für den Handzuschnitt vorgesehen sind.
4.  Wählen Sie in der Liste Verfügbare Optimierungen die Läufe aus, die Sie zu einer Tischoptimierung zusammenfassen wollen.

**Ergänzende Informationen**
⇨ "Tischoptimierungen verlinken" auf Seite J-1088

#### Schnelloptimierung erstellen
Bereits optimierte Platten / Muster (durch A+W Production oder via Tischoptimierung in A+W Realtime Optimizer), welche aber noch nicht an den Tisch gesandt wurden, können komplett aufgelöst und neu optimiert werden. Dadurch werden beispielsweise Eilscheiben oder Bruchscheiben mit hinein-optimiert und es entsteht ein komplett neues Schnittmuster für die neu optimierten Platten.

Zum Erstellen einer Schnelloptimierung müssen folgende Arbeitsschritte durchgeführt werden:
*   Tischoptimierung erstellen.
*   Tischoptimierung wurde begonnen zu schneiden.

Entsteht beim Zuschnitt Bruch, kann dieser zeitnah und bequem über die sogenannte Schnelloptimierung nachgeschnitten werden.

*Abb. J-5: Zuschnitt-Übersicht*

Über das Kontextmenü können Sie die Optimierung ab dem nächst möglichen Muster auflösen und neu optimieren.

Im Beispiel Abb. J-5 (Zuschnitt-Übersicht) wurden die Muster / Platten 1 und 2 an den Tisch gesandt und geschnitten. Die Platten / Muster 3-6 können mittels Rechtsklick aufgelöst und neu optimiert werden (Schnell-Optimierung).

*Abb. J-6: Kontextmenü - Optimierung 15002 Los 1 ab Muster 3 auflösen und neu optimieren.*

Nachdem die Meldung bestätigt wurde, werden die noch zu schneidenden Platten zunächst entfernt. Im Anschluss werden die zu Bruch gegangenen Scheiben inklusive der noch zu schneidenden Platten neu optimiert.

**Ergänzende Informationen**
⇨ "Die Zuschnitt-Übersicht" auf Seite J-1100

#### Verlinken von Läufen
Mit dem Verlinken von Läufen hat A+W die Möglichkeit geschafften, Restplatten zu vermeiden. In der Vergangenheit mussten solche Restplatten manuell zusammengelegt werden. Dies ist jetzt nicht mehr notwendig.

Das Verlinken findet während des Zuschnittprozesses statt und wird mit diesem synchronisiert.

Im Dialog Lauf: # kann im Bereich Restblatt-Verwaltung die Option zum Verlinken von Läufen aktiviert werden.

Nachdem der Zuschnitt gestartet wurde, wird nach dem Senden des 1. Musters eines Loses, das geschnitten wird, in der Datenbank beginnend mit dem Folgelauf nach einem passenden Los dieser Glasart für diesen Tisch gesucht und die entsprechenden Daten geladen.

Das Folgelos muss den Status Freigegeben besitzen. Das Laden geschieht im Hintergrund, damit der Zuschnitt am Tisch weiterlaufen kann. Ist das vorletzte Blatt (konfigurierbar) einer Glasart geschnitten, erhält der Benutzer optional eine Abfrage, mit welchem Lauf und Los das Restblatt verlinkt werden soll. Der Benutzer hat dann die Möglichkeit, das Verlinken abzubrechen oder eben ein entsprechendes Los auszuwählen.

Wird das Verlinken bestätigt, werden Bruch- und Eilscheiben dieser Glasart geladen und mit der Priorität 0 zu der Folgeoptimierung hinzugefügt. Das Restblatt des zur Zeit geschnittenen Loses wird zu der Folgeoptimierung als Startblatt hinzugefügt. Anschließend wird die Optimierung gestartet. Nach dem Optimieren wird die Folgeoptimierung mit der Ursprungsoptimierung verbunden, so dass das Restblatt der Ursprungsoptimierung mit den Scheiben des 1. Blatts der Folgeoptimierung aufgefüllt wird. Alle weiteren Muster der Folgeoptimierung werden in der gerade geschnittenen Optimierung aufgelöst. Anschließend wird neuer Schneidcode erstellt und übertragen.

Das 1. Muster der Folgeoptimierung wird als Geschnitten markiert. Die Folgeoptimierung wird mit dem vorhandenen Mechanismus aus der Tischoptimierung zunächst als Tischoptimierung abgespeichert und dann mit der Lauf- und Losnummer der ursprünglichen Folgeoptimierung versehen. Der Status der Folgeoptimierung wird auf Begonnen gesetzt.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Auswahl der zu verlinkenden Optimierung" auf Seite J-1190

#### Tischansteuerung
A+W Realtime Optimizer arbeitet als Leitstand für einen Zuschnitttisch.

> **Parameter des angeschlossenen Tischs**
> Bei der Installation wird festgelegt, welche Zuschnitttische mit einem A+W Realtime Optimizer angesteuert werden. Entsprechend werden die Parameter bei der Installation hinterlegt. Die Optimierungen werden mit den eingestellten Parametern von A+W Production oder A+W Realtime Optimizer erstellt.

Bei der Tischansteuerung wird Schneidcode generiert und für die Ansteuerung des Zuschnitttischs seriell an den Tisch übertragen oder in einem vereinbarten Verzeichnis bereitgestellt. Je nach angeschlossenem Tisch und technischer Lösung zur Tischansteuerung wird der Schneidcode mit einem weiteren Programm an den Tisch übertragen oder von der Software des Tischherstellers aus dem vereinbarten Verzeichnis abgerufen.

*Abb. J-7: Datenerfassung und -verarbeitung in A+W Realtime Optimizer*

Sobald der Schneidcode für eine Lagerplatte an den Tisch geschickt wurde, behandelt A+W Realtime Optimizer die Lagerplatte als abgearbeitet. Wird die Übertragung von Schneidcode für mehrere Platten eines Laufes unterbrochen, so kann die Arbeit an dieser Stelle wieder fortgesetzt werden.

In Zusammenarbeit mit XTV wird Bruch am Tisch direkt an A+W Realtime Optimizer zurückgemeldet. Ist der Schneidcode der letzten Lagerplatte einer Glasart (eines Loses) noch nicht an den Zuschnitttisch übertragen, so kann der Bruch automatisch nachoptimiert und mit der letzten Lagerplatte des Loses zugeschnitten werden.

### Zuschnitt
In diesem Abschnitt wird Ihnen gezeigt, wie Sie mit dem Zuschnitt umgehen.
Der Themenblock beinhaltet folgende Schulungseinheiten:
*   Läufe zum Zuschnitt auswählen
*   Optimierung prüfen und schneiden
*   Arbeit unterbrechen und fortsetzen
*   Die Zuschnitt-Übersicht

#### Überblick
**Lernziele**
*   Die Abläufe im Zuschnitt kennenlernen und verstehen.

**Nutzen**
Das Arbeiten mit dem A+W Realtime Optimizer ist nur dann sinnvoll möglich, wenn Sie die Abläufe kennen.

**Definition**
*   **Panorama**: Konfigurierbarer Programmteil für die Ansteuerung von komplexen Maschinen oder Maschinenverbünden (Schneidanlagen).

**Merke**
*   **Laufnummer 1000-9999**: Stammen aus einem vorgelagerten System.
*   **Laufnummer ab 15000**: Diese Läufe enthalten Tischoptimierungen, die mit dem A+W Realtime Optimizer erstellt wurden. Der Nummernkreis ist konfigurierbar.
*   **Panorama**: Die Administration im Panorama ist passwort-geschützt.

#### Läufe zum Zuschnitt auswählen
Die Optimierungen liegen in Form von Läufen vor. Wählen Sie die Läufe aus, in denen die Optimierungen enthalten sind, die Sie auf dem Schneidtisch zuschneiden wollen.

##### Läufe zum Zuschnitt auswählen
1.  Öffnen Sie den Dialog Wählen Sie einen Lauf aus. Wählen Sie dazu im Menü Zuschnitt > Schneide Optimierung.
2.  Wählen Sie einen Lauf aus. Markieren Sie dazu in der Liste Läufe einen Eintrag. In der Liste Optimierungen werden die Optimierungen angezeigt, die für diesen Lauf existieren.
    > **Nummern der Läufe**
    > Läufe mit den Nummern 1000-9999 stammen aus einem vorgelagerten System und enthalten eine oder mehrere Optimierungen. Läufe ab Nummer 15000 enthalten Tischoptimierungen, die mit A+W Realtime Optimizer erstellt wurden.
3.  Wählen Sie eine oder alle Optimierungen aus. Wenn keine Optimierung markiert wird, gelten alle Optimierungen als ausgewählt. Es kann konfiguriert werden, ob einzelne Optimierungen gewählt werden dürfen.
    > **Nummern der Optimierungen**
    > Die Optimierungen sind Losweise (je Glasart) angelegt und je Lauf fortlaufend durchnummeriert.
4.  Betätigen Sie [OK]. Die gewählten Optimierungen werden zum Zuschnitt ausgewählt und im Dialog Lauf [Nummer -] - Lauf [Nummer] angezeigt.
5.  Schließen Sie den Dialog. Betätigen Sie dazu die Schaltfläche [OK].
6.  Starten Sie den Zuschnitt. Betätigen Sie dazu die Schaltfläche [START].

##### Geschnittene Läufe erneut schneiden
Wenn alle Platten einer Optimierung geschnitten wurden, wird der ganze Lauf in den Status Produziert gesetzt. Dieser Status kann in den Status Freigegeben zurückgesetzt und der ganze Lauf erneut zugeschnitten werden.
1.  Öffnen Sie den Dialog Zurücksetzen eines Zuschnitt Laufes. Wählen Sie dazu im Menü Optimierung > Zurücksetzen.
    Im Dialog Zurücksetzen eines Zuschnitt Laufes wird eine Liste aller Läufe angezeigt, für die Sie Statusänderungen vornehmen können. Die Liste erscheint nach Laufnummern sortiert. Vollständig geschnittene Läufe werden mit dem Status Produziert angezeigt.
2.  Wählen Sie die den Lauf, den Sie vom Status Produziert in den Status Freigegeben zurücksetzen wollen. Sie können mehrere Läufe markieren und gleichzeitig zurücksetzen.
3.  Um den Lauf zurückzusetzen, betätigen Sie die Schaltfläche [OK]. Der Lauf steht als fertige Optimierung für einen erneuten Zuschnitt zur Verfügung.

##### Muster überspringen
Wenn Sie für eine Platte Muster überspringen wählen, dann wird für diese Platte kein Schneidcode erzeugt und kein Brechbild angezeigt.
1.  Öffnen Sie den Dialog Restblatt Behandlung. Betätigen Sie dazu die Schaltfläche [Optionen] im Dialog Lauf: [Nr.] - Lauf: [Nr.] des Laufes, den Sie bearbeiten wollen.
2.  Markieren Sie in der Liste Optimierungen die Glasart, von der einzelne Lagerplatten nochmals geschnitten werden sollen. In der Liste Platten werden alle zu der markierten Glasart gehörigen Platten des Laufes angezeigt. In der Spalte Status sehen Sie den Status jeder einzelnen Lagerplatte. Sie können nur solche Platten überspringen, die nicht im Status Geschnitten sind.
3.  Klicken Sie mit der rechten Maustaste auf die Platte, die Sie beim Zuschnitt überspringen wollen. Es erscheint ein Kontext-Menü mit den Einträgen Muster überspringen und Kein Schneidcode senden.
4.  Wählen Sie Muster überspringen um für diese Platte keinen Schneidcode zu erzeugen und kein Brechbild anzuzeigen.
5.  Schließen Sie den Dialog. Betätigen Sie dazu die Schaltfläche [OK].

##### Erzeugung von Schneidcode unterdrücken
Wenn Sie für eine Platte Kein Schneidcode senden wählen, dann wird für diese Platte kein Schneidcode erzeugt aber in A+W Production Terminal (XTV) ein Brechbild angezeigt.
1.  Öffnen Sie den Dialog Restblatt Behandlung. Betätigen Sie dazu die Schaltfläche [Optionen] im Dialog Lauf: [Nr.] - Lauf: [Nr.] des Laufes, den Sie bearbeiten wollen.
2.  Markieren Sie in der Liste Optimierungen die Glasart, von der einzelne Lagerplatten nochmals geschnitten werden sollen. In der Liste Platten werden alle zu der markierten Glasart gehörigen Platten des Laufes angezeigt. In der Spalte Status sehen Sie den Status jeder einzelnen Lagerplatte. Sie können nur bei solchen Platten keinen Schneidcode senden, die nicht im Status Geschnitten sind.
3.  Klicken Sie mit der rechten Maustaste auf die Platte, die Sie beim Zuschnitt überspringen wollen. Es erscheint ein Kontext-Menü mit den Einträgen Muster überspringen und Kein Schneidcode senden.
4.  Wählen Sie Kein Schneidcode senden um für diese Platte keinen Schneidcode zu erzeugen, aber in A+W Production Terminal (XTV) ein Brechbild anzuzeigen.
5.  Schließen Sie den Dialog. Betätigen Sie dazu die Schaltfläche [OK].

**Ergänzende Informationen**
⇨ Softwarereferenz, "Lauf: Nummer" auf Seite J-1186
⇨ Softwarereferenz, "Wählen Sie einen Lauf aus" auf Seite J-1179

#### Optimierung prüfen und schneiden
Wenn Sie Optimierungen zum Zuschnitt ausgewählt haben, können Sie einige Prüfungen vornehmen und dann die Optimierungen zum Schneidtisch übertragen.

Folgende Arbeitsschritte sind in diesem Kapitel erklärt:
*   Vorgesehene Zuschnittreihenfolge anzeigen.
*   Restblätter überprüfen.
*   Zuschnittbeginn festlegen und Zuschnitt starten.

Die nachfolgenden Beschreibungen setzen voraus, dass Sie den vorherigen Arbeitsschritt Läufe zum Zuschnitt auswählen durchgeführt haben und der Dialog Lauf [Nummer] - Lauf [Nummer] angezeigt wird.

##### Vorgesehene Zuschnittreihenfolge anzeigen
1.  Betätigen Sie die Schaltfläche [Reihenfolge]. Der Dialog Zuschnittreihenfolge wird angezeigt.
    > **Reihenfolge bei mehreren Losen**
    > Wurden mehrere Lose zum Zuschnitt ausgewählt, so werden die Zuschnittplatten so sortiert, wie das A+W Realtime Optimizer konfiguriert wurde. Z. B. können alle Restblätter am Ende des gesamten Laufes geschnitten werden oder jeweils am Ende einer Glasart. A+W Realtime Optimizer kann auch so konfiguriert werden, dass Lagerplatten alternierend (z. B.: beschichtet - unbeschichtet) geschnitten werden.
2.  Betätigen Sie [OK], um den Dialog zu schließen.

##### Restblätter überprüfen
1.  Betätigen Sie die Schaltfläche [Restblätter]. Der Dialog Restblatt Behandlung wird angezeigt.
2.  Prüfen Sie die angezeigten Werte.
3.  Ändern Sie den Status für einzelne Platten oder die Einstellungen für den Umgang mit Bruchscheiben, falls erforderlich.
4.  Wenn an Ihrem Arbeitsplatz das Softwaremodul PlanEdit installiert ist, dann können Sie die durch Betätigen der Schaltfläche Muster bearbeiten das Schneidmuster für die markierte Platte anzeigen.
5.  Betätigen Sie [OK], um den Dialog zu schließen.

##### Zuschnittbeginn festlegen und Zuschnitt starten
1.  Markieren Sie in der Liste Optimierungen das Los, ab dem der Zuschnitt erfolgen soll.
2.  Markieren Sie in der Liste Muster die Lagerplatte, ab der der Zuschnitt erfolgen soll.
3.  Betätigen Sie die Schaltfläche [START].
    Für die angezeigten Optimierungen wird der Schneidcode erzeugt und für den angeschlossenen Schneidtisch bereitgestellt.
    Die Beschriftung und Funktion der Schaltfläche ändert sich zu [STOP].
    Wenn A+W Realtime Optimizer mit einem A+W Production Terminal (XTV) zusammenarbeitet, dann kann die Brechbildanzeige des A+W Production Terminal (XTV) jetzt mit den Tasten [Stopp] und [<<] gesteuert werden.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Lauf: Nummer" auf Seite J-1186
⇨ Softwarereferenz, "Lauf [Nummer] - Lauf [Nummer]" auf Seite J-1183

#### Arbeit unterbrechen und fortsetzen
Eine Optimierung, deren Lagerplatten nach und nach am Zuschnitttisch geschnitten werden, kann auf Grund technischer Störungen oder Arbeitsende unterbrochen werden. A+W Realtime Optimizer registriert, an welcher Stelle die Arbeit unterbrochen wurde und bietet die Möglichkeit, an der Unterbrechungsstelle die Arbeit fortzusetzen.

Nachfolgend finden Sie folgende Arbeitsschritte erklärt:
*   Zuschnitt innerhalb einer Optimierung unterbrechen.
*   Einen unterbrochenen Zuschnitt einer Optimierung fortsetzen.

##### Zuschnitt innerhalb einer Optimierung unterbrechen
1.  Sie befinden sich in dem Dialog Zuschnitt-Übersicht ein.
2.  Betätigen Sie die Schaltfläche [STOPP].
3.  Schließen Sie den Dialog.

##### Einen unterbrochenen Zuschnitt einer Optimierung fortsetzen
A+W Realtime Optimizer merkt sich, wenn eine begonnene Optimierung nicht zu Ende zugeschnitten wurde.
1.  Wählen Sie im Menü Zuschnitt > Schneide Optimierung, um eine Optimierung zum Zuschnitt auszuwählen.
    Es erscheint eine Sicherheitsabfrage. Es wird angegeben, welcher Lauf nicht zu Ende geführt wurde und abgefragt, ob dieser Lauf weiter ausgeführt werden soll.
2.  Um den unterbrochenen Lauf anzuzeigen, wählen Sie [Ja].
    A+W Realtime Optimizer zeigt den Lauf im Dialog Lauf [Nummer] - Lauf [Nummer] an, der abgebrochen wurde.
    Wenn Sie die Sicherheitsabfrage mit Nein beantworten, dann wird die unterbrochene Optimierung auf den Status Begonnen gesetzt. Bereits übertragene Zuschnittsmuster behalten den Status Geschnitten. Der Dialog Wählen Sie einen Lauf aus wird angezeigt.
3.  Um den unterbrochenen Zuschnitt fortzusetzen, wählen Sie [Start].
    Der Schneidcode der bereits geschnittenen Scheiben wird nicht erneut zum Schneidtisch übertragen.

#### Die Zuschnitt-Übersicht
Die Zuschnitt-Übersicht zeigt Ihnen, was als nächstes zugeschnitten werden soll.

*Abb. J-8: Zuschnitt-Übersicht*
A Menü, B Plattenanzeige, C Scheibenanzeige

Das Menü (A) auf der linken Seite des Dialogs können Sie ein- und ausblenden, indem Sie die entsprechendeSymbol-Schaltfläche anklicken. Darüber hinaus können Sie die einzelnen Einträge (Zuschnitt, Panorama, Administration) auf- und zuklappen.

Über die Optionen im Eintrag Zuschnitt können Sie sich die Anzeige konfigurieren.

*Abb. J-9: Plattenanzeige*

Die Plattenanzeige (B) können Sie proTisch konfigurieren. Über die Checkboxen können Sie bequem einstellen, welche Felder in der Tabelle angezeigt werden sollen und welche nicht.

Soll die Plattengrafik gespiegelt werden, aktivieren Sie im Bereich Plattengrafik die gewünschte Achse.

Gleiches gilt für die Scheibenanzeige (C). Auch hier können Sie die gewünschten Optionen zur Anzeige ein- und ausblenden:

*Abb. J-10: Scheibenanzeige*

Der Punkt Modell im Eintrag Panorama visualisiert das Modell, das zur Maschinenansteuerung im A+W Realtime Optimizer hinterlegt ist.

Der Bereich Administration ist passwortgeschützt. Hier nehmen Sie allgemeine Einstellungen vor.

Durch Klicken auf die Symbol-Schaltfläche [Start] starten Sie den Zuschnitt. Um den Zuschnitt zu stoppen, klicken Sie auf die Symbol-Schaltfläche [Stopp].

#### Schneidstatus zurücksetzen
Wenn ein Lauf oder einzelne Lagerplatten bereits den Status Geschnitten erhalten haben, aber noch einmal geschnitten werden sollen, dann kann der Schneidstatus zurückgesetzt und das Schneiden wiederholt werden.

Mit folgenden Arbeitsschritten können Sie mit den Schneidstatus zurücksetzen:
*   Geschnittene Platten erneut schneiden.
*   Geschnittene Läufe erneut schneiden.

Wenn eine Optimierung als ganzes zurückgesetzt wurde, aber nur einzelne Lagerplatten erneut geschnitten werden sollen, dann können Sie mit folgenden Arbeitsschritten Teile einer Optimierung vom erneuten Zuschnitt ausschließen:
*   Muster überspringen.
*   Erzeugung von Schneidcode unterdrücken.

##### Geschnittene Platten erneut schneiden
Einzelne Platten oder ganze Läufe können erneut geschnitten werden, solange die Läufe noch im Zugriff von A+W Realtime Optimizer sind. Der Zuschnitt für den entsprechenden Lauf muss gewählt und im Dialog Lauf: [Nr.] - Lauf: [Nr.] angezeigt werden.
1.  Öffnen Sie den Dialog Restblatt Behandlung. Betätigen Sie dazu die Schaltfläche [Restblätter] im Dialog Lauf: [Nr.] - Lauf: [Nr.] des entsprechenden Laufes.
2.  Markieren Sie in der Liste Optimierungen die Glasart, für die eine Lagerplatte erneut geschnitten werden soll.
    In der Liste Platten werden alle zu der markierten Glasart gehörigen Platten des Laufes angezeigt. In der Spalte Status sehen Sie den Status jeder einzelnen Lagerplatte.
    ⇨ Softwarereferenz, "Lauf: Nummer" auf Seite J-1186
3.  Klicken Sie mit der rechten Maustaste auf die Platte, die Sie vom Status Geschnitten zurücksetzen und erneut schneiden wollen.
    Es erscheint ein Kontext-Menü mit dem Eintrag Geschnitten.
4.  Wählen Sie Geschnitten um die Platte zurückzusetzen.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Lauf: Nummer" auf Seite J-1186

### Zusammenarbeit mit anderen Modulen
**Lernziele**
*   Die Zusammenarbeit mit dem A+W Residual Stock Manager kennenlernen und verstehen.
*   Die Zusammenarbeit mit dem A+W Pattern Viewer kennenlernen und verstehen.
*   Die Zusammenarbeit mit dem A+W PlanEditor kennenlernen und verstehen.
*   Die Zusammenarbeit mit dem A+W Continuous Cutting kennenlernen und verstehen
*   Die Zusammenarbeit mit dem A+W Defect Optimizer kennenlernen und verstehen.

**Nutzen**
Die Leistungsfähigkeit des A+W Realtime Optimizer kann durch die Anbindung anderer Module erhöht werden.

**Definitionen**
*   **A+W Residual Stock Manager**: Das Restelager-Magazin verwaltet Restplatten am Zuschnitttisch.
*   **A+W Pattern Viewer**: Stellt die Brechbildanzeige am Zuschnitttisch zur Verfügung.
*   **A+W PlanEditor**: Zeigt die Daten von zu schneidenden Mustern in tabellarischer und in grafischer Form an.
*   **A+W Continuous Cutting**: Steuert vom Büro aus, was geschnitten wird, so dass die Bediener automatisch wissen, was zu tun ist.
*   **A+W Defect Optimizer**: Ist die intelligente Fehlerstellenoptimierung.
*   **A+W DynOpt Compact**: A+W Einstiegslösung im Bereich Dynamische Optimierung.

**Merke**
*   **Konfiguration**: Der A+W Realtime Optimizer muss zur Zusammenarbeit mit den anderen Modulen entsprechend konfiguriert werden.

#### Überblick
A+W Realtime Optimizer kann zur Zusammenarbeit mit unterschiedlichen Modulen konfiguriert werden. Informationen zur Anbindung verschiedener Vorsysteme wurden in dem vorherigen Kapitel bereits gegeben.

Wenn A+W Realtime Optimizer entsprechend konfiguriert wurde, kann es mit folgenden Modulen zusammenarbeiten:
*   A+W Residual Stock Manager
*   A+W Pattern Viewer
*   A+W PlanEditor
*   A+W Continuous Cutting
*   A+W Defect Optimizer
*   A+W DynOpt Compact

#### A+W Residual Stock Manager
Bei diesem Modul handelt es sich um ein Restelager-Magazin, in dem Restplatten am Zuschnitttisch verwaltet werden. Bleibt beim Zuschnitt eine Restplatte übrig, so wird dieses nicht verworfen sondern im A+W Residual Stock Manager zwischengespeichert. Informationen über Glasart, Dicke und Abmessungen der Restplatten werden in einem Verwaltungsprogramm (A+W Planning Web) erfasst und gespeichert. A+W Realtime Optimizer kann mit dem A+W Planning Web zusammenarbeiten. Dabei werden Daten über die Restplatten ausgetauscht. Restplatten können anschließend vom A+W Realtime Optimizer in Tischoptimierungen integriert werden. Wird eine Optimierung geschnitten, kann die Restplatte durch eine Platte aus dem Restelager ersetzt werden (ohne Neuoptimierung).

Sobald eine Restplatte in eine Optimierung eingeplant ist, informiert A+W Realtime Optimizer das A+W Planning Web über diesen Status. Die Restplatte kann dann nicht mehr für andere Zuschnitte verwendet werden.

Wird ein Tisch mit Schneidcode angesteuert, der für eine Resteplatte optimiert wurde, so steuert der Schneidcode das Restelager-Magazin an und die benötigte Restplatte wird zum Zuschnitt auf den Tisch aufgelegt.

##### A+W Planning Web
In diesem Modul nehmen Sie die Konfiguration für den A+W Residual Stock Manager vor.

> **A+W Planning Web-Konfiguration**
> Die Standard-Konfiguration wird bei der Installation durch A+W-Mitarbeiter vorgenommen. Wir erläutern in dieser Dokumentation, wie Sie Lager, Abstellplätze und Gestelle im A+W Planning Web anlegen.

##### Oberfläche
Wenn Sie das A+W Planning Web gestartet haben, erscheint folgende Ansicht:

*Abb. J-11: Oberfläche A+W Planning Web*

Im Anschluss wählen Sie den Eintrag Lager aus. Sie befinden sich im Bereich Aufträge.

*Abb. J-12: Bereich: Aufträge*

##### Stammdaten
In diesem Bereich befinden sich die Einstellungen für die Stammdaten. Dazu zählen:
*   Lager
*   Abstellplätze
*   Gestelle
*   Gruppen

**Lager**
Über die Symbol-Schaltflächen Lager können Sie sich die entsprechenden Inhalte anzeigen lassen.

*Abb. J-13: Bereich: Stammdaten*

In diesem Bereich werden Ihnen alle in Ihrem Hause angelegten Lager angezeigt.
Es stehen Ihnen folgende Möglichkeiten zur Verfügung:
*   Den Namen eines bestehenden Lagers ändern
*   Ein neues Lager hinzufügen
*   Ein bestehendes Lager löschen

**So ändern Sie den Namen eines bestehenden Lagers**
1.  Klicken Sie mit der Maus in das Feld Bezeichnung. Das Feld wird zur Bearbeitung freigegeben.
2.  Ändern Sie den Namen und verlassen Sie das Feld.
3.  Das Feld bekommt oben links in der Ecke ein kleines rotes Dreieck. Das Dreieck signalisiert, dass es Änderungen gibt, die noch nicht gespeichert wurden. Es wird so lange angezeigt, bis Sie auf die Schaltfläche [Speichern] klicken.
4.  Klicken Sie auf die Schaltfläche [Speichern], um die Angaben zu speichern.
5.  Das kleine rote Dreieck ist nicht mehr da.

**So fügen Sie ein neues Lager hinzu**
1.  Klicken Sie auf die Schaltfläche [Hinzufügen]. Es wird eine neue Zeile oben in der Tabelle eingefügt.
2.  Im Feld ID wird die nächst mögliche Nummer automatisch vorgeschlagen. Sie können diese Nummer überschreiben.
3.  Geben Sie im Feld Bezeichnung den Namen für das Lager ein und verlassen Sie das Feld.
4.  Das Feld bekommt oben links in der Ecke ein kleines rotes Dreieck. Das Dreieck signalisiert, dass es Änderungen gibt, die noch nicht gespeichert wurden. Es wird so lange angezeigt, bis Sie auf die Schaltfläche [Speichern] klicken.
5.  Klicken Sie auf die Schaltfläche [Speichern], um die Angaben zu speichern.
6.  Das kleine rote Dreieck ist nicht mehr da.

**So löschen Sie ein Lager**
1.  Klicken Sie in die Zeile mit dem entsprechenden Lager.
2.  Klicken Sie auf die Schaltfläche [Löschen].
3.  Das Lager wird gelöscht. Vorsicht: Es erscheint keine Sicherheitsabfrage.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Lager" auf Seite J-1207

**Abstellplätze**
Abstellplätze sind Plätze oder Bereiche, auf denen Scheiben abgestellt werden können.
Um einem Lager weitere Abstellplätze hinzufügen, bestehende Abstellplätze zu ändern oder zu löschen, klicken Sie in dem Eintrag für das entsprechende Lager auf die Schaltfläche [Bearbeiten]. Im Anschluss werden Ihnen alle Abstellplätze angezeigt, die für das Lager angelegt sind.

*Abb. J-14: Bereich: Abstellplatzinformationen*

Es stehen Ihnen folgende Möglichkeiten zur Verfügung:
*   Einen neuen Abstellplatz hinzufügen
*   Einen bestehenden Abstellplatz löschen
*   Änderungen an einem bestehenden Abstellplatz vornehmen

**So fügen Sie einen neuen Abstellplatz hinzu**
1.  Klicken Sie auf die Schaltfläche [Hinzufügen]. Es wird eine neue Zeile oben in der Tabelle eingefügt.
2.  Im Feld ID wird die nächst mögliche Nummer automatisch vorgeschlagen. Sie können diese Nummer überschreiben.
3.  Geben Sie im Feld Bezeichnung den Namen für den Abstellplatz ein.
4.  Wählen Sie aus der Kombobox Lagertyp den entsprechenden Typ aus (Lagerplatz/Lagereingang).
5.  Wählen Sie aus der Kombobox Zuordnungsstatus den entsprechenden Status aus.
6.  Klicken Sie auf die Schaltfläche [Speichern], um die Angaben zu speichern.

**So löschen Sie einen Abstellplatz**
1.  Klicken Sie in die Zeile mit dem entsprechenden Abstellplatz.
2.  Klicken Sie auf die Schaltfläche [Löschen].
3.  Der Abstellplatz wird gelöscht. Vorsicht: Es erscheint keine Sicherheitsabfrage.

**So nehmen Sie Änderungen an einem Abstellplatz vor**
1.  Klicken Sie in das Feld mit dem entsprechenden Eintrag.
2.  Überschreiben Sie den Eintrag oder wählen Sie aus der Kombobox den gewünschten Eintrag aus.
3.  Klicken Sie auf die Schaltfläche [Speichern], um die Angaben zu speichern.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Abstellplatzinformationen" auf Seite J-1209

**Gestelle**
In diesem Bereich werden Ihnen die für einen Abstellplatz angelegten Gestelle angezeigt.

*Abb. J-15: Stammdaten: Gestelle*

Es stehen Ihnen folgende Möglichkeiten zur Verfügung:
*   Ein neues Gestell hinzufügen
*   Ein bestehendes Gestell löschen
*   Änderungen an einem bestehenden Gestell vornehmen

**So fügen Sie ein neues Gestell hinzu**
1.  Klicken Sie auf die Schaltfläche [Hinzufügen]. Es wird eine neue Zeile oben in der Tabelle eingefügt.
2.  Im Feld ID wird die nächst mögliche Nummer automatisch vorgeschlagen. Sie können diese Nummer überschreiben.
3.  Im Feld Bezeichnung vergeben Sie einen eindeutigen Namen zur Identifizierung eines Gestelltyp.
4.  Wählen Sie aus der Kombobox Zuordnungsstatus den entsprechenden Status aus.
    ⇨A+W Realtime Optimizer: Softwarereferenz, "Zuordnungsstatus" auf Seite J-1211
5.  Wählen Sie aus der Kombobox Eigenschaft den entsprechenden Typ aus.
6.  Klicken Sie auf die Schaltfläche [Speichern], um die Angaben zu speichern.

**So löschen Sie ein bestehendes Gestell**
1.  Klicken Sie in die Zeile mit dem entsprechenden Gestell.
2.  Klicken Sie auf die Schaltfläche [Löschen].
3.  Das Gestell wird gelöscht. Vorsicht: Es erscheint keine Sicherheitsabfrage.

**So nehmen Sie Änderungen an einem Gestell vor**
1.  Klicken Sie in das Feld mit dem entsprechenden Eintrag.
2.  Überschreiben Sie den Eintrag oder wählen Sie aus der Kombobox den gewünschten Eintrag aus.
3.  Klicken Sie auf die Schaltfläche [Speichern], um die Angaben zu speichern.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Gestelle" auf Seite J-1211

**Gestelleigenschaften**
In diesem Bereich werden Ihnen die Eigenschaften der unterschiedlichen Gestelltypen angezeigt. Als Eigenschaft ist hier der Gestelltyp zu verstehen (A-Bock, L-Bock, Fächerwagen, etc.).

*Abb. J-16: Stammdaten: Gestelleigenschaften*

Es stehen Ihnen folgende Möglichkeiten zur Verfügung:
*   Eine neue Gestelleigenschaft hinzufügen
*   Eine bestehende Gestelleigenschaft löschen
*   Änderungen an einer bestehenden Gestelleigenschaft vornehmen

**So fügen Sie eine neue Gestelleigenschaft hinzu**
1.  Klicken Sie auf die Schaltfläche [Hinzufügen]. Es wird eine neue Zeile oben in der Tabelle eingefügt.
2.  Im Feld Bezeichnung vergeben Sie einen eindeutigen Namen zur Identifizierung eines Gestelltyp.
3.  Geben Sie im Feld Zugangsart wählen Sie aus der Kombobox die entsprechende Art aus.
    ⇨ A+W Realtime Optimizer: Softwarereferenz, "Zugangsart" auf Seite J-1213
4.  Wählen Sie aus der Kombobox Lagertyp den entsprechenden Typ aus (Lagerplatz/Lagereingang).
5.  Wählen Sie aus der Kombobox Zuordnungsstatus den entsprechenden Status aus.
6.  Klicken Sie auf die Schaltfläche [Speichern], um die Angaben zu speichern.

**So löschen Sie eine bestehende Gestelleigenschaft**
1.  Klicken Sie in die Zeile mit der entsprechenden Eigenschaft.
2.  Klicken Sie auf die Schaltfläche [Löschen].
3.  Die Gestelleigenschaft wird gelöscht. Vorsicht: Es erscheint keine Sicherheitsabfrage.

**So nehmen Sie Änderungen an einer Gestelleigenschaft vor**
1.  Klicken Sie in das Feld mit dem entsprechenden Eintrag.
2.  Überschreiben Sie den Eintrag oder wählen Sie aus der Kombobox den gewünschten Eintrag aus.
3.  Klicken Sie auf die Schaltfläche [Speichern], um die Angaben zu speichern.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Gestelleigenschaften" auf Seite J-1213

**Übersicht**
In diesem Bereich werden Ihnen alle Restblätter angezeigt, die eingelagert wurden.

*Abb. J-17: Übersicht: Eingelagerte Restblätter*

Die Daten können in der Ansicht editiert werden, z. B. die Größe der eingelagerten Restscheibe. Über die Filterfunktionen, die Ihnen im Tabellenkopf jedes Feldes zur Verfügung stehen, können Sie die Ergebnisse der Anzeige einschränken.

Es stehen Ihnen folgende Möglichkeiten zur Verfügung:
*   Änderungen an einem eingelagerten Rest vornehmen
*   Einen neuen Rest hinzufügen
*   Einen bestehenden Rest löschen

**So nehmen Sie Änderungen an einem eingelagerten Rest vor**
1.  Klicken Sie in dem Eintrag den Sie ändern möchten auf die Schaltfläche [Bearbeiten]. Es öffnet sich der Dialog Hinzufügen/Bearbeiten.
2.  Nehmen Sie die gewünschten Änderungen vor.
3.  Klicken Sie auf die Schaltfläche [Anwenden], um die Angaben zu speichern.

**So fügen Sie einen neuen Rest hinzu**
1.  Klicken Sie auf die Schaltfläche [Neuen Datensatz hinzufügen]. Es öffnet sich der Dialog Hinzufügen/Bearbeiten.
2.  Im Feld Lager wählen Sie aus der Kombobox das entsprechende Lager aus.
3.  Im Feld Abstellplatzinformationen wählen Sie aus der Kombobox den Abstellplatz aus, auf dem der Rest steht.
4.  Im Feld Gestell wählen Sie aus der Kombobox das entsprechende Gestell aus, auf dem der Rest steht.
5.  Im Feld Gruppe wählen Sie aus der Kombobox die entsprechende Gruppe aus.
6.  Im Feld Glastyp wählen Sie aus der Kombobox aus, um welchen Glastyp es sich bei dem Rest handelt.
7.  In den Feldern Breite und Höhe geben Sie die Abmessungen des Restes ein.
8.  Im Feld Info können Sie eine zusätzliche Information zu dem Rest hinterlegen.
9.  Im Feld Zuordnungsstatus wählen Sie aus der Kombobox den entsprechenden aus.
    ⇨ Softwarereferenz, "Zuordnungsstatus" auf Seite J-1216
10. Im Feld Datum geben Sie ein, wann der Rest eingelagert wurde.
11. Klicken Sie auf die Schaltfläche [Anwenden], um die Angaben zu speichern.

**So löschen Sie einen eingelagerten Rest**
1.  Klicken Sie in die Zeile mit der entsprechenden Eigenschaft.
2.  Klicken Sie auf die Schaltfläche [Löschen].
3.  Der eingelagerte Rest wird gelöscht. Vorsicht: Es erscheint keine Sicherheitsabfrage.

> **Restelager-Platten und Restblätter nicht gleichzeitig möglich!**
> Wenn Sie für eine Optimierung Platten aus dem Restelager verwenden wollen, dann wird ein zuvor eingetragenes Restblatt ignoriert. A+W Realtime Optimizer zeigt dann eine entsprechende Meldung an.

##### Restelager-Platten bei der Optimierung verwenden
1.  Wählen Sie im Dialog Tischoptimierung das Register Restelagerplatten.
    In der rechten Liste werden alle Platten angezeigt, die im A+W Residual Stock Manager für die Glasart und Dicke des Laufes vorhanden sind und dem Schneidtisch zur Verfügung stehen.
2.  Markieren Sie die Restelager-Platte, die A+W Realtime Optimizer für die Zuschnittoptimierung verwenden soll.
    Sie können bis zu zehn Restelager-Platte in eine Optimierung integrieren.
3.  Um die Optimierung zu erstellen, wechseln Sie in das Register Optimieren und betätigen Sie die Schaltfläche [Optimieren].
    Anschließend wird die Restelager-Platte im Programm, das die Restelager-Platten verwaltet, für diesen Lauf reserviert und kann von keinem anderen Lauf mehr verwendet werden.
4.  Um die Optimierung abzuspeichern, betätigen Sie die Schaltfläche [Speichern].

**Ergänzende Informationen**
⇨ Softwarereferenz, "Restplatten und Lagerplatten" auf Seite J-1166

##### Etiketten drucken
Das Drucken der entsprechenden Etiketten ist ebenfalls aus der Übersicht heraus möglich. Dazu klicken Sie in dem Eintrag auf die Schaltfläche [Drucken].

> **Etiketten drucken**
> Zum Drucken der Etiketten muss der entsprechende Drucker eingerichtet sein.

#### A+W Pattern Viewer
Der A+W Pattern Viewer stellt eine Brechbildanzeige am Zuschnitttisch zur Verfügung, mit der, je nach Konfiguration, auch Bruch erfasst werden kann. Der A+W Realtime Optimizer gibt die Informationen an den A+W Pattern Viewer, wenn Schneidcode für den angeschlossenen Tisch erstellt wurde. Der A+W Pattern Viewer kann darauf hin das zur jeweiligen Optimierung gehörende Brechbild anzeigen. Die Darstellung entspricht dem zu schneidenden Lagermaß bzw. Restblatt und enthält alle wichtigen Informationen über die Optimierung, den Artikel und die einzelnen Scheiben. Wird mit A+W Pattern Viewer Bruch erfasst, so gibt das Modul eine entsprechende Information an den A+W Realtime Optimizer.

##### Einstellungen
Über das A+W Logo erreichen Sie die Einstellungen:

*Abb. J-18: Menü*

Der Eintrag **Sprache** enthält alle Sprachen, in denen das Modul verfügbar ist. Die Sprache kann zur Laufzeit umgeschaltet werden.

Die Bereiche **Anwendung registrieren** und **Bruchgründe** werden von A+W-Mitarbeitern benötigt, um das Modul in Ihrem Haus entsprechend Ihren Anforderungen zu konfigurieren. Wir gehen daher nicht weiter auf diese Bereiche ein.

Im Bereich **Über** wird Ihnen die Versionsnummer des Moduls angezeigt.

Über die Schaltfläche **Zurück** gelangen Sie wieder in die Brechbildanzeige.

##### Die Oberfläche
*Abb. J-19: Zurück zur Brechbildanzeige*

*Abb. J-20: Die Brechbildanzeige*

##### Die Menüleiste
Die Menüleiste im A+W Pattern Viewer beinhaltet die Einträge:
*   Ansicht
*   Maße

**Ansicht**
Klicken Sie auf Ansicht, öffnet sich die Menüleiste:

*Abb. J-21: Menüleiste - komplett*

Die Menüleiste ist in einzelne Bereiche unterteilt:
*   Brechbild
*   Zoom
*   Eingabetyp
*   Ansicht konfigurieren
*   Tooltipp
*   Validierung

Direkt unterhalb der Menüleiste befindet sich der Informationsbereich. Dieser enthält weiterreichende Informationen zu dem aktuellen Muster.

*Abb. J-22: Menüleiste - Informationsbereich*

Ganz links wird Ihnen die Lauf-, Los- und Musternummer angezeigt. Im Beispiel oben heißt das:
*   Laufnummer: 2689
*   Losnummer: 3
*   Musternummer: 3

Als nächstes wird Ihnen die Nummer des aktuellen Muster und die Gesamtanzahl der Muster angezeigt. Im Beispiel oben Muster Nummer 3 von insgesamt 5. Dann wird Ihnen die Glasart angezeigt. Im Beispiel oben Star S 4 mm 4.00. Im Anschluss folgt die Breite x Höhe der verwendeten Lagerplatte. Rechts außen wird das Optimierungsergebnis für das aktuelle Muster angezeigt.

**Brechbild**
In diesem Bereich können Sie die Art der Anzeige durch Klicken auf die entsprechende Schaltfläche auswählen. Es gibt zwei Möglichkeiten:
*   Brechbild
*   JSON

Bei Ihrer täglichen Arbeit werden Sie die Einstellung Brechbild verwenden. Beim Auftreten von Problemen können Sie dann in die Einstellung JSON wechseln, über das Kontextmenü den Inhalt kopieren und diesen anschließend einem A+W-Mitarbeiter für eine detaillierte Analyse zur Verfügung stellen.

**Zoom**
In diesem Bereich befinden sich die Einstellungen für die Größendarstellung des Brechbildes und dem Informationsbereich direkt unterhalb der Menüleiste.
Brechbild:

*Abb. J-23: Zoom Brechbild*

Die Kombobox enthält die Werte 0 bis 4. Die im Anschluss folgende Grafik soll die unterschiedlichen Einstellungen verdeutlichen:

*Abb. J-24: Unterschiedlichen Schnitte*

*   **0:** Es wird das komplette Brechbild einer Platte angezeigt:
    *Abb. J-25: Brechbild - komplett*
*   **1:** Es werden die einzelnen X-Schnitte angezeigt. Ein X-Schnitt (üblicherweise der Traverenschnitt) verläuft parallel zum linken bzw. rechten Plattenrand (-schnitt) bzw. senkrecht zum unteren Plattenrand. Dieser Schnitt teilt die Lagerplatte in Teile bzw. Traveren. Über die Pfeiltasten rechts und links können Sie die einzelnen Traveren weiter bzw. zurück schalten.
    *Abb. J-26: Brechbild - Travere*
*   **2:** Es werden die einzelnen Y-Schnitte angezeigt (von unten nach oben). Ein Y-Schnitt verläuft parallel zum oberen bzw. unteren Plattenrand (-schnitt). Dieser Schnitt teilt eine Travere in obere und untere Abschnitte. Über die Pfeiltasten rechts und links können Sie die einzelnen Schnitte weiter bzw. zurück schalten.
    *Abb. J-27: Brechbild - Y-Schnitt*
*   **3:** Es werden die einzelnen Z-Schnitte angezeigt (von links nach rechts). Ein Z-Schnitt verläuft wieder parallel zu einem linken bzw. rechten Plattenrand (-schnitt) und/oder einem X-Schnitt. Er unterteilt die durch Y-Schnitte gebildeten Abschnitte. Über die Pfeiltasten rechts und links können Sie die einzelnen Schnitte weiter bzw. zurück schalten.
    *Abb. J-28: Brechbild - Z-Schnitt*
*   **4:** Es werden die einzelnen W-Schnitte angezeigt (von unten nach oben). Ein W-Schnitt verläuft parallel zu einem Y-Schnitt und befindet sich zwischen einem X-Schnitt (bzw. linkem oder rechten Plattenrand (-schnitt)) und einem Z-Schnitt. Über die Pfeiltasten rechts und links können Sie die einzelnen Schnitte weiter bzw. zurück schalten.
    *Abb. J-29: Brechbild - W-Schnitt*

**Schriftgröße**
Über die Kombobox können Sie steuern, in welcher Größe der Informationsbereich direkt unterhalb der Menüleiste dargestellt wird.
Es stehen die Werte klein, mittel und groß zur Verfügung:
*   **Klein:**
    *Abb. J-30: Schriftgröße klein*
*   **Mittel:**
    *Abb. J-31: Schriftgröße mittel*
*   **Groß:**
    *Abb. J-32: Schriftgröße groß*

**Eingabetyp**
In diesem Bereich befindet sich der Eintrag Einzelscheibe. In diesem Modus arbeiten automatisierte Betriebe. Es wird jede Scheibe einzeln zur Abarbeitung vorgegeben. Der entsprechende Modus wird bei Einrichtung des A+W Pattern Viewer von A+W Mitarbeitern eingestellt.

**Ansicht konfigurieren**
In diesem Bereich befinden sich verschiedene Eigenschaften, mit deren Hilfe Sie sich die Brechbildanzeige nach Ihren Bedürfnissen einstellen können.

*   **Koordinaten:**
    *Abb. J-33: Koordinaten*
    Über diese Schaltfläche aktivieren bzw. deaktivieren Sie die Anzeige der Koordinaten:
    A: Koordinaten deaktiviert, B: Koordinaten aktiviert
*   **Maße:**
    *Abb. J-34: Maße*
    Über diese Schaltfläche aktivieren bzw. deaktivieren Sie die Anzeige der Abmessungen der Scheibe:
    A: Maße deaktiviert, B: Maße aktiviert
*   **Gestellnummer:**
    *Abb. J-35: Gestellnummer*
    Über diese Schaltfläche aktivieren bzw. deaktivieren Sie die Anzeige der Gestellnummer:
    A: Gestellnummer deaktiviert, B: Gestellnummer aktiviert
*   **Brechreihenfolge:**
    *Abb. J-36: Brechreihenfolge*
    Über diese Schaltfläche aktivieren bzw. deaktivieren Sie die Anzeige der Brechreihenfolge. Die Scheibe mit der kleinsten Nummer wird zuerst gebrochen:
    A: Brechreihenfolge deaktiviert, B: Brechreihenfolge aktiviert
*   **Zweite Glasart oder Laufnummer:**
    *Abb. J-37: Zweite Glasart oder Laufnummer*
    Über diese Schaltfläche aktivieren bzw. deaktivieren Sie die Anzeige der zweiten Glasart oder der Laufnummer. Im Beispiel unten wird die Laufnummer angezeigt:
    A: Laufnummer deaktiviert, B: Laufnummer aktiviert
*   **Barcode:**
    *Abb. J-38: Barcode*
    Über diese Schaltfläche aktivieren bzw. deaktivieren Sie die Anzeige des Barcodes:
    A: Barcode deaktiviert, B: Barcode aktiviert
*   **Zusatztexte:**
    *Abb. J-39: Zusatztexte*
    Über diese Schaltfläche aktivieren bzw. deaktivieren Sie die Anzeige der Zusatztexte. Zusatztexte können im Kopf- und im Fußbereich angezeigt werden. Ist ein Kopftext konfiguriert, ändert sich die Hintergrundfarbe von blau auf lachs. Ist ein Fußtext konfiguriert, ändert sich die Hintergrundfarbe von rot auf gelb. Entsprechende Texte werden von A+W Mitarbeitern bei der Installation nach Ihren Wünschen eingerichtet:
    A: Kopfbereich ohne Zusatztext, B: Kopfbereich mit Zusatztext
    A: Fußbereich ohne Zusatztext, B: Fußbereich mit Zusatztext
*   **Travere drehen:**
    *Abb. J-40: Travere drehen*
    Über diese Schaltfläche ist es möglich, Traveren automatisch um 90° zu drehen, wenn das Größenverhältnis der Travere besser zum Bildschirm passt, um eine größere Darstellung zu erzielen:
    A: Travere nicht gedreht, B: Travere gedreht

**Tooltipp**
In diesem Bereich befindet sich eine Kombobox, mit deren Hilfe Sie die Anzeigedauer für einen Tooltipp einstellen können. Sie können von einer bis zu acht Sekunden wählen.
*Abb. J-41: Anzeigedauer Tooltipp*

**Validierung**
In diesem Bereich befindet sich die Schaltfläche über die Sie die Arbeitsrichtung wechseln können.
A: Normal, B: Umkehren

Normalerweise liegt die Platte so auf dem Tisch, dass Sie auf der linken Seite anfangen zu brechen. Die Brechbildanzeige schalten Sie dann zum nächsten Muster weiter, indem Sie auf den rechten Pfeil klicken.

Es gibt aber auch Konstellationen, wo die Platte so auf dem Tisch liegt, dass Sie auf der rechten Seite anfangen zu brechen. Damit Sie dann ebenfalls den rechten Pfeil zum Umschalten auf das nächste Muster verwenden können, aktvieren Sie die Schaltfläche [umkehren].

##### Informationen zu Scheibe und Verschnitt
Wenn Sie die Maus auf einer Scheibe oder auf einem leeren Bereich platzieren, werden Ihnen die entsprechenden Informationen angezeigt:

*Abb. J-42: Informationen zu Scheibe und Verschnitt*
A: Scheibeninformation, B: Verschnittinformation

> **Informationen**
> Die angezeigten Informationen sind abhängig vom Kunden und der Konfiguration. Sie werden bei der Installation von A+W-Mitarbeitern entsprechend eingerichtet. Wenn Sie Änderungen an Ihrer Konfiguration wünschen (z. B. der Name des Kunden soll angezeigt werde), kontaktieren Sie bitte einen A+W-Mitarbeiter.

##### Verlinkte Läufe anzeigen
Das blaue Dreieck an der oberen Kante im A+W Pattern Viewer zeigt an, wo der verlinkte Lauf beginnt:
*Abb. J-43: Beginn des verlinkten Laufes*

##### Abstellkante anzeigen
Wurde bei einer freien Form in der SN-Datei eine Markierung für die Abstellkante hinterlegt (z. B. in der Auftragserfassung mit iTOE), wird diese Kante im A+W Pattern Viewer durch einen gelben Pfeil angezeigt:
*Abb. J-44: Abstellkante für freie Formen*

##### Symbol für Stempel, Logo oder Referenzmarke anzeigen
Der A+W Pattern Viewer bietet auch die Möglichkeit, ein Bild an der Stelle eines Stempels oder eines Logos zu zeigen.
> **Symbole**
> Die Symbole sind abhängig vom Kunden und der Konfiguration. Sie werden bei der Installation von A+W-Mitarbeitern entsprechend eingerichtet. Wenn Sie Änderungen an Ihrer Konfiguration wünschen (z. B. Logo oder Stempel anzeigen), kontaktieren Sie bitte einen A+W-Mitarbeiter.

##### Farbauswahl für Auftragspositionen
Der A+W Pattern Viewer bietet auch die Möglichkeit, Glas in einer benutzerdefinierten Farbe einzufärben. Es stehen verschiedene Farben zur Auswahl.
> **Farben**
> Die Auswahl der Farben basiert auf den Wünschen der einzelnen Kunden. Sie werden bei der Installation von A+W-Mitarbeitern entsprechend eingerichtet. Wenn Sie Änderungen an Ihrer Konfiguration wünschen (z. B. Logo oder Stempel anzeigen), kontaktieren Sie bitte einen A+W-Mitarbeiter.

##### Erste und letzte Scheibe markieren
Der A+W Pattern Viewer bietet die Möglichkeit, die ersten und letzten Scheiben auf einem Abstellplatz entsprechend zu markieren.
> **Ersten und letzten Scheibe markieren**
> Ob die ersten und letzten Scheiben auf einem Abstellplatz markiert werden, basiert auf den Wünschen der einzelnen Kunden. Das wird bei der Installation von A+W-Mitarbeitern entsprechend eingerichtet. Wenn Sie Änderungen an Ihrer Konfiguration wünschen, kontaktieren Sie bitte einen A+W-Mitarbeiter.

##### Maße
Klicken Sie auf Maße, öffnet sich der Bereich Einheitensystem:
*Abb. J-45: Menü Maße*

Im Eintrag **Einheitensystem** können Sie wählen zwischen:
*   Metrisch
*   Imperial

Die darunter liegende Kombobox ist abhängig von der Auswahl des Einheitensystems. Haben Sie Metrisch gewählt, können Sie über die Kombobox Nachkommastellen entscheiden, wie viele Nachkommastellen (bis zu drei) Sie sich anzeigen lassen. Haben Sie Imperial gewählt, können Sie über die Kombobox Genauigkeit diese auswählen (1/16, 1/32, 1/64, 1/128, 1/256).

##### Bruchscheiben
Im A+W Pattern Viewer können Sie Scheiben als Bruch markieren, indem Sie in der Brechbildanzeige die entsprechende Scheibe markieren. Es erscheint eine Auswahl mit allen angelegten Bruchgründen. Wählen Sie den entsprechenden Bruchgrund aus. Die Auswahl wird geschlossen und die ausgewählte Scheibe entsprechend gekennzeichnet.

#### A+W PlanEditor
Der A+W PlanEditor zeigt die Daten von zu schneidenden Mustern in tabellarischer und in grafischer Form an. Die Ergebnisanzeige zeigt übersichtlich die statistische Auswertung der vorhandenen Muster. Sie erhalten einen schnellen Überblick über die zu produzierenden Scheiben, Lagermaße, Restblätter, Verschnitt, usw.

Der grafische Editor zeigt, je nach Konfiguration, die zu schneidenden Muster an und stellt eine Reihe von Bearbeitungsmöglichkeiten zur Verfügung. Sie können Muster anlegen, verändern, Scheiben zufügen, speichern und drucken.

Wenn der A+W PlanEditor an Ihrem Arbeitsplatz installiert ist, dann können Sie nach Erstellung einer Tischoptimierung durch Doppelklick auf die optimierte Zuschnittplatte den A+W PlanEditor starten. Dieser zeigt dann das Schneidmuster der Zuschnittplatte an. Veränderungen, die Sie mit dem A+W PlanEditor an einem solchen Muster vornehmen, werden in den A+W Realtime Optimizer übernommen.

**Ergänzende Informationen**
⇨ Weitere Informationen zu dem A+W PlanEditor finden Sie in der entsprechenden Dokumentation.

#### A+W Continuous Cutting
Läuft der A+W Realtime Optimizer am Schneidtisch im Modus Kontinuierlicher Zuschnitt wird vor dem Start des Zuschnitts eine Übersicht der für diesen Tisch geplanten Läufe angezeigt. Hier besteht auch noch die Möglichkeit, einen Lauf wieder zurückzusetzen. Fahren Sie mit dem Zuschnitt fort, wird die erste Gruppe in den Zuschnitt geladen und der Zuschnitt gestartet. Ist eine Eilgruppe vorhanden, wird diese zuerst geladen und die darauffolgende Gruppe angehängt. Wenn der letzte Lauf der aktuellen Gruppe fast fertig zugeschnitten ist, wird die nächste Gruppe automatisch in den Zuschnitt geladen. So werden nach und nach alle geplanten Läufe entsprechend der in der Planung vorgenommenen Einstellungen automatisch abgearbeitet.

##### Übersicht der geplanten Läufe
In der Planungsansicht werden alle in A+W Production optimierten und zum Zuschnitt freigegebenen Läufe und ihre Eigenschaften angezeigt. Hier können Sie nun auswählen, welche Läufe am Schneidtisch, für den sie optimiert wurden, zugeschnitten werden sollen. Dabei kann die Reihenfolge festgesetzt und verschiedene Einstellungen vorgenommen werden. Für bereits geplante Läufe können Änderungen vorgenommen werden, vorausgesetzt der Zuschnitt wurde noch nicht begonnen.

Klicken Sie im A+W Realtime Optimizer auf Zuschnitt > Kontinuierliches Schneiden ... erscheint eine Liste mit den freigegebenen Losen:

*Abb. J-46: Freigegebene Lose*

Über die Kombobox Schneidtische können Sie bei Bedarf die Anzeige einschränken. Klicken Sie dann unten rechts auf die Schaltfläche [Planung F5], öffnet sich die Planungsansicht:

*Abb. J-47: Planungsansicht*

##### Erläuterung der Felder
**Filter**
Für eine bessere Übersicht können Filter angewendet werden, um die angezeigten Läufe beispielsweise nach Glasart zu filtern.
Die entsprechenden Einstellungen befinden sich in A+W Production > Konfiguration > Parameter > A+W Production > Kontinuierliches Schneiden > AUW_CONTINUOUS_CUTTING > Filter.

*Abb. J-48: Filtereinstellungen*

Um einen neuen Filter anzulegen oder aber um Änderungen an einem bestehenden Filter vorzunehmen, klicken Sie bitte auf die drei Punkte. Es öffnet sich der Dialog.

*Abb. J-49: Neuen Filter anlegen oder bestehenden Filter ändern*

Um Änderungen an einem bestehenden Filter vorzunehmen, markieren Sie den entsprechenden Filter und klicken auf die Schaltfläche [Bearbeiten]. Um einen neuen Filter anzulegen, klicken Sie auf die Schaltfläche [Neu]. Es öffnet sich der Dialog Filter anlegen/bearbeiten:

*Abb. J-50: Bestehenden Filter bearbeiten*

Geben Sie dem Filter einen aussagekräftigen Namen und achten Sie auf den korrekten Syntax des Filters. Sie können einen festen Filter definieren, z. B. pool_teile.glasart = 1004 oder einen Filter mit bis zu zwei Platzhaltern, z. B. pool_teile.glasart = [TTV1NUM]. Bei Filtern mit Platzhalter geben Sie später den gewünschten Wert selbst ein.

**Produktionstermin**
Wird hier eine Zeitspanne angegeben, werden nur Läufe angezeigt, deren Produktionstermin in dieser Zeitspanne liegt.

**Nachoptimierung**
Hier wird der Modus für die Nachoptimierung und die Menge an Bruchscheiben, ab der dieser ausgelöst werden soll, festgelegt.

**Eiloptimierung**
Hier legen Sie fest, ob für den Lauf eine Eiloptimierung durchgeführt werden soll, wenn eine bestimmte Menge an Bruchscheiben erreicht wurde.

**Restplattenverwaltung**
Hier legen Sie fest, ob und in welchem Modus das Restblatt verlinkt werden soll.

**Restblatt bearbeiten**
Hier legen Sie fest, ob das Restblatt bearbeitet werden kann und ab welcher Länge.

**Gruppieren**
Mehrere Läufe lassen sich zu einer Gruppe zusammenfassen. Läufe derselben Gruppe werden im A+W Realtime Optimizer am Schneidtisch zusammen an den Zuschnitt geschickt. Wurde für eine Gruppe der Zuschnitt begonnen, darf kein Lauf dieser Gruppe verändert werden. Ein Lauf muss einer Gruppe zugeordnet sein, um für den Zuschnitt freigegeben werden zu können.

**So erstellen Sie eine Gruppe für einen Lauf**
1.  Wählen Sie den entsprechenden Tisch aus.
2.  Markieren Sie die gewünschten Läufe.
3.  Betätigen Sie die Schaltfläche [Gruppieren].
4.  Betätigen Sie die Schaltfläche [Freigabe].
5.  Die Gruppe wird erstellt und hinter die bereits freigegebenen Läufe gehängt.

**So verschieben Sie eine Gruppe für einen Lauf**
Freigegebene und noch nicht begonnene Läufe können in der Reihenfolge geändert werden.
1.  Wählen Sie entsprechende Gruppe aus.
2.  Verschieben Sie die ausgewählte Gruppe mit den Pfeiltasten an die gewünschte Stelle.
3.  Betätigen Sie die Schaltfläche [Freigabe].
4.  Die Gruppe wird an die gewünschte Stelle verschoben.

**So lösen Sie eine Gruppe auf**
1.  Markieren Sie die gewünschten Lose einer Gruppe.
2.  Betätigen Sie die Schaltfläche [Zurücksetzen].
3.  Betätigen Sie die Schaltfläche [Freigabe].
4.  Die Gruppe wird aufgelöst.

**Eilgruppen**
Eilgruppen beinhalten Läufe, die bevorzugt behandelt werden.

**So erstellen Sie eine Eilgruppe**
1.  Wählen Sie die gewünschten Läufe aus.
2.  Betätigen Sie die Schaltfläche [Eilgruppe].
3.  Betätigen Sie die Schaltfläche [Freigabe]. Sollte die Eilgruppe nicht an der gewünschten Stelle stehen, können Sie diese (solange der Zuschnitt noch nicht begonnen hat) mit Hilfe der Pfeiltasten an die gewünschte Stelle verschieben.

**Zurücksetzen von Läufen**
Bereits geplante Läufe und Einstellungen können wieder zurückgesetzt werden, sodass sie nicht automatisch zugeschnitten werden.

##### Zuschneiden
Klicken Sie im A+W Realtime Optimizer Menü auf Einstellungen > Zuschnitt. Es öffnet sich der Dialog:

*Abb. J-51: Automatischer Zuschnitt*

Wählen Sie aus der Kombobox Automatisch und klicken Sie auf [OK]. Öffnen Sie nun den Zuschnitt über die Symbol-Schaltfläche in der Menüleiste.

Sie sehen eine Übersicht über den geplanten Zuschnitt.

*Abb. J-52: Geplanter Zuschnitt*

Über die Schaltfläche [Optionen] können Sie (wenn nötig) den Status der Läufe zurücksetzen.

Klicken Sie auf die Schaltfläche [Start] um mit dem Zuschnitt zu beginnen. Die Optimierungen der ersten Gruppe werden an den Zuschnitt übergeben.

*Abb. J-53: Zuschnitt-Übersicht*

Wenn das letzte Muster der Gruppe an den Schneidtisch gesendet und zugeschnitten wurde, wird die nächste Gruppe automatisch in den Zuschnitt geladen.

#### A+W Defect Optimizer
... die intelligente Fehlerstellenoptimierung!

In Verbindung mit z. B. einem Qualitätsscanner der Firma Viprotron werden die Lagerplatten gescannt und etwaige Fehler bzw. Fehlerstellen (Defekte) noch vor dem Beginn des Zuschnitts erkannt und visualisiert. Je früher die Fehlerstellen im Prozess erkannt werden, um so geringer sind die anfallenden Kosten.

Die Fehlerstellen werden in der Optimierung für die Neu- und Restrukturierung des Schnittbildes berücksichtigt. Gibt es einzuhaltende Reihenfolgen, werden diese selbstverständlich berücksichtigt.
Selbst auf Restplatten werden die Fehlerstellen gespeichert und können so später ohne erneute Kontrolle wiederverwendet werden.

Lassen sich Defekte durch die Optimierung nicht vermeiden (z. B. Anzahl und Größe der Scheiben auf dem Muster), so versucht die Optimierung kleine und somit kostengünstigere Gläser auf die Defekte zu legen.

Gläser, die auf Defekten liegen, werden automatisch als Bruch gemeldet und nachgeschnitten.

> **Voraussetzung**
> Für den Einsatz des A+W Defect Optimizers ist das Produktionssystem A+W Production sowie der A+W Realtime Optimizer Voraussetzung.

**Ergänzende Informationen**
⇨ Weitere Informationen zu dem A+W Defect Optimizer finden Sie in der entsprechenden Dokumentation.

#### A+W DynOpt Compact
A+W DynOpt Compact ist die clevere Einstiegslösung von A+W im Bereich Dynamische Optimierung.

Das System baut auf dem A+W Realtime Optimizer auf und lädt die Läufe, welche voroptimiert vom vorgelagerten Produktionssystem A+W Production gesendet werden. Diese Läufe werden komplett aufgelöst und systematisch und dynamisch neu optimiert. Dieses Verfahren verbessert den Verschnitt erheblich und reduziert die Anzahl an zu speichernden Restplatten.

Sie können A+W DynOpt Compact daher auch als automatischen A+W Realtime Optimizer sehen.

A+W DynOpt Compact arbeitet mit folgenden zwei Modulen:
*   A+W DynOpt Compact Import
*   A+W DynOpt Compact Optimierung

##### A+W DynOpt Compact Import
Beim Import werden die für A+W DynOpt Compact freigegebenen Läufe in so genannte Cluster umgewandelt. Bei einem Cluster handelt es sich um eine, zunächst beliebige Produktionseinheit, also z. B. um ein Gestell, eine Gruppe von Gestellen oder auch um einzelne Scheibe.

##### A+W DynOpt Compact Optimierung
Nach dem Import wird, anhand des verfügbaren Platzes, die Abarbeitungsreihenfolge der Cluster erzeugt. Diese entspricht weitgehend der Produktionsreihenfolge, wobei in besonderen Fällen Cluster vorgezogen werden können, damit der Verschnitt verbessert wird. Sie können sowohl Fächerwagen als auch A-Böcke oder beide Gestelle zusammen verweden.

Etwa die Hälfte der berechneten Cluster werden zu primären Clustern, der Rest wird zu sekundären Clustern. Die primären Cluster bekommen die Priorität 1 und werden in der aktuellen Optimierung komplett optimiert. Die sekundären Cluster dienen als Füller und die Optimierung entscheidet selbst, ob diese benötigt werden oder nicht.

**Beispiel:**
Verfügbarer Platz: 6. Der Platz für ein Fächerwagen entspricht 1, der Platz für ein A-Bock entspricht 0,5 (gerechnet in Fächerwagen, d. h. 1 Fächerwagen = 2 A-Böcke.

Wenn etwa genauso viele Fächerwagen wie A-Böcke zur Verfügung stehen und die Verteilung auf die Cluster übertragen wird, dann gilt: 4 Fächerwagen plus 4x0,5 A-Böcke = 6. Jeweils die Hälfte der Anzahlen ergibt je zwei primäre und zwei sekundäre Fächerwagen und A-Böcke.

| | Eingelesen | Verwendet | Primär | Sekundär |
| :--- | :--- | :--- | :--- | :--- |
| Fächerwagen | 16 | 4 | 2 | 2 |
| A-Bock | 17 | 4 | 2 | 2 |
*Tab. J-1: Beispiel*

Bei der Ermittlung der Timeline werden folgende Bedingungen eingehalten:
*   Die primäre Sortierung der Cluster ist die Produktionsreihenfolge.
*   Solange Cluster des aktuellen Laufs den verfügbaren Platz füllen können, werden keine Cluster des nachfolgenden Laufs zur Erstellung der Timeline verwendet.
*   Falls man in den sekundären Clustern eine Glasart hat, die in den primären Clustern nicht vorkommt, so gibt es zwei Möglichkeiten:
    *   Besteht der Cluster auch aus Scheiben einer Glasart, zu denen es auch primäre Scheiben gibt, so werden nur diese optimiert. Die Scheiben der Glasart, die in den primären Clustern nicht vorkommt, werden dann optimiert, wenn der Cluster primär wird.
    *   Besteht der Cluster komplett aus Scheiben einer Glasart, die in den primären Clustern nicht vorkommt, wo wird innerhalb des aktuellen Laufes nach einem alternativen Cluster gesucht, der (zumindest teilweise) aus Scheiben einer primären Glasart besteht. Falls man einen solchen findet, werden die Cluster getauscht, ansonsten wird der aktuelle Cluster nicht mit optimiert.

In jedem A+W DynOpt Compact-Schritt werden alle primären und alle sekundären Cluster zusammen der Optimierung zur Verfügung gestellt. Die primären Scheiben werden stets von der Optimierung verwendet, die sekundären Scheiben nur bei Bedarf. Nach einem solchen Schritt sind alle primären Cluster gefüllt und können durch sekundäre und in manchen Fällen auch neue Cluster ersetzt werden. Eine Abarbeitung von mehreren Clustern sieht wie folgt aus:

##### A+W DynOpt Compact-Lauf erzeugen
A+W DynOpt Compact-Läufe können auf zwei Arten erstellt werden.
*   Bilden von A+W DynOpt Compact-Läufen aus der Cluster-Ansicht.
*   Bilden eines A+W DynOpt Compact-Laufes aus dem Zuschnitt heraus.

**Bilden von A+W DynOpt Compact-Läufen aus der Cluster-Ansicht**
1.  Öffnen Sie den Dialog Cluster-Ansicht. Wählen Sie dazu Zuschnitt > A+W DynOpt Compact.
2.  Markieren Sie im linken Bereich den bzw. die Läufe, mit denen Sie einen A+W DynOpt Compact-Lauf erzeugen möchten.
3.  Öffnen Sie für diese Auswahl das Kontext-Menü und wählen Sie A+W DynOpt Compact-Lauf erzeugen.
4.  Nachdem die A+W DynOpt Compact-Läufe gebildet wurden, erscheinen diese im linken, oberen Bereich des Dialogs. Sie sind jetzt mit einem +-Zeichen versehen. Wenn Sie die Baumstruktur aufklappen, können Sie sich die Abstellplatzdaten zu den Läufen ansehen.

**Bilden eines A+W DynOpt Compact-Laufes aus dem Zuschnitt heraus**
1.  Öffnen Sie den Dialog Wählen Sie einen Lauf aus. Wählen Sie dazu entweder Zuschnitt > Schneide Optimierung oder betätigen Sie die entsprechende Symbol-Schaltfläche.
2.  Markieren Sie im Bereich der Läufe den Lauf, mit dem Sie einen A+W DynOpt Compact-Lauf erzeugen möchten.
3.  Öffnen Sie für diese Auswahl das Kontext-Menü und wählen Sie A+W DynOpt Compact für Lauf XXXX erzeugen.
4.  Nachdem der A+W DynOpt Compact Lauf gebildet wurde, erscheint dieser im linken, oberen Bereich des Dialogs und ist mit Cut&Go gekennzeichnet. Markieren Sie den Lauf im linken Bereich, erhalten Sie im Bereich der Optimierungen entsprechende Informationen dazu.

> **Voraussetzung**
> Für den Einsatz von A+W DynOpt Compact ist das Produktionssystem A+W Production sowie der A+W Realtime Optimizer Voraussetzung.

**Ergänzende Informationen**
⇨ Weitere Informationen zu dem A+W DynOpt Compact finden Sie in der entsprechenden Dokumentation.

## Softwarereferenz

### Übersicht
Im nachfolgenden Kapitel werden alle Dialoge beschrieben, die im A+W Realtime Optimizer insgesamt zur Verfügung stehen. Je nach Programmvariante sind manche Dialoge oder Felder in den Dialogen nicht zu sehen. Folgende Varianten sind möglich:
*   In die A+W Production-Umgebung eingebetteter A+W Realtime Optimizer.
*   In die A+W Production-Umgebung eingebetteter A+W Realtime Optimizer im Einsatz mit einem Remaster-Magazin.
*   A+W Realtime Optimizer-Stand alone.

Bei der Beschreibung des jeweiligen Dialogs ist angegeben, wenn eine Information nur für eine bestimmte Variante gilt.

### Menüs
Nach dem Start von Realtime Optimizer erscheinen folgende Menüs:

*Abb. J-54: Menü des A+W Realtime Optimizer*

In den Menüs befinden sich Funktionen, Untermenüs und Dialog-Aufrufe. In der nachfolgenden Tabelle werden die Funktionen kurz beschrieben und die Untermenüs und Dialogaufrufe genannt. Die Beschreibung der Dialoge in den nachfolgenden Kapiteln erfolgt nach Menü sortiert.

### Symbol-Schaltflächen
Einige Dialoge können direkt über Symbol-Schaltflächen aufgerufen werden:

| Icon | Dialog/Funktion |
| :--- | :--- |
| [Eilscheiben] | Öffnet den Dialog "Eilscheiben" auf Seite J-1144 |
| [Optimierung] | Öffnet den Dialog "Selektieren Sie die zu optimierenden Gläser" auf Seite J-1157 |
| [Zuschnitt] | Öffnet den Dialog "Wählen Sie einen Lauf aus" auf Seite J-1179 |
| [Bruchpool] | Öffnet den Dialog "Bruchpool" auf Seite J-1192 |
| [Fehler] | Öffnet den Dialog “Fehlermeldungen" auf Seite J-1206 |
| [Info] | Öffnet den Dialog mit Informationen zum A+W Realtime Optimizer. |

*Tab. J-2: Symbol-Schaltflächen und ihre Funktion*

