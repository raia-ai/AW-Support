---
description: "DE-HB-AWCADDesignerBars"
---


# A+W CAD Designer (Bars) Handbuch

**Deutsch**

---
## Editorial

### Revisionsübersicht der Dokumentation

| Datum | Änderung |
| :--- | :--- |
| 10-2024 | Gesamthandbuch für PDF und HTML5-Format aktualisiert. |

### Anmerkungen

Diese Veröffentlichung ist ausschließlich für Endanwender von A+W CAD Designer (Bars) gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.

Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von A+W CAD Designer (Bars).

### Urheberrechte

© 2024, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

### Darstellungskonventionen

Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

| Begriff | Bedeutung |
| :--- | :--- |
| *Kursiv* | sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Preiseigenschaften*. |
| **Fett** | sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: Geben Sie den Wert **5** ein. |
| > | Mit dem sogenannten Brotkrumenpfad ist der Weg gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B. Stammdaten > Preise > ISO-Preise. |
| [ ] | Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit [OK] speichern Sie die Daten. |
| < > | Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit <F1> öffnen Sie die Online-Hilfe. |

### Kontakt

**A+W Software GmbH**
Siemensstr. 3
D-35463 Fernwald
Deutschland

**Tel.:** +49 641 96620 0
**E-Mail:** info@a-w.com
**Web:** http://www.a-w.com

## Inhalt

- **Überblick A**
  - Tutorial A-9
    - Überblick A-12
    - Aufbau des Tutorials A-13
    - A+W CAD Designer (Bars) stellt sich vor A-14
    - Arbeiten mit A+W CAD Designer (Bars) A-16
      - Oberfläche von A+W CAD Designer (Bars) A-16
    - Einstellungen A-75
    - Stammdaten in A+W CAD Designer (Bars) A-85
    - Sprossen A-98
      - Neue Konstruktionen A-99
    - Zuschnitt und Messen A-121
    - Spezialmuster A-127
      - Sondermuster A-127
    - Fassaden A-130
    - Makros A-137
    - Datenaustausch A-166
      - Datenimport A-166
      - Datenexport A-169
    - Konfiguration A-174
    - Anhang - Makrokatalog A-175
  - Softwarereferenz A-187
    - Bedienung von A+W CAD Designer (Bars) A-190
      - Softwarebegriffe A-191
      - Programm beenden A-195
    - Übersicht A-196
    - Umgang mit Dateien A-197
      - Neue Scheibe A-199
      - Übergabedatei importieren A-202
      - Neue Scheibenposition A-204
      - Drucken A-205
      - Listendruck A-206
      - Druckereinrichtung A-207
    - Werkzeuge verwenden A-210
    - Mit Spezialmustern arbeiten A-212
      - Muster Senkrecht-Waagerecht A-213
      - Kundenvorgabe SW-Muster A-216
      - Eingabe Sprossen-Abstände A-219
      - Rautenmuster... A-220
      - Fassadenanlage... A-222
      - Sonne und Sterne A-223
      - Makro auswählen A-225
      - Makro-Parameter A-226
      - Relativer Abstand A-227
    - Messen und Zuschnitt A-228
      - Abstand A-229
      - Zuschnitt-Informationen A-230
    - Die Stammdaten A-232
      - Stammdaten A-233
      - Stammdaten-Editor A-235
      - Passwort A-240
    - Ansicht A-241
      - Vermaßung A-242
      - Maße A-244
      - Sprachauswahl A-245
    - Die Hilfe verwenden A-246
      - Über CAD Designer A-247
  - Help Cards A-249
    - Informationen zu den HelpCards A-251
    - Stammdaten A-252
      - Werkzeuge A-253
      - Fangpunkte A-254
      - Sprossen anlegen A-255
      - Stammdaten schützen A-256
    - Sprossen A-257
      - Eigenschaften der Scheibe A-258
      - Einfaches Sprossenmuster platzieren A-259
      - Sprossen über Werte platzieren A-260
      - Modell mit Sprossen platzieren A-261
      - Freie Sprossenkonstruktion erstellen A-262
    - Spezialmuster A-263
      - Fassadenanlage erstellen A-264
      - Makro laden A-265
      - Ein Makro ändern und speichern A-266
      - Eigenes Makro erstellen A-267
- **Index Z**

## A - Überblick

### Revisionsübersicht des Moduls:

| Datum | Änderung |
| :--- | :--- |
| 01-2017 | Produkt- und Firmennamen angepasst. |
| 03-2013 | Überarbeitung im Rahmen der Produktneuausrichtung |
| 10-2010 | Ersterstellung |

### Zu diesem Modul finden Sie folgende Kapitel

- Tutorial
- Softwarereferenz

## Tutorial

### In diesem Kapitel finden Sie folgende Themen:
- Überblick
- A+W CAD Designer (Bars) stellt sich vor
- Arbeiten mit A+W CAD Designer (Bars)
- Sprossen
- Spezialmuster
- Datenaustausch
- Konfiguration
- Anhang - Makrokatalog

#### Überblick
- Aufbau des Tutorials A-13
- A+W CAD Designer (Bars) stellt sich vor A-14
- Arbeiten mit A+W CAD Designer (Bars) A-16
  - Oberfläche von A+W CAD Designer (Bars) A-16
    - Programm-Präsentation A-17
    - Die Menüleiste A-18
    - Die Symbolleiste A-18
    - Das Wertefenster A-20
    - Die Standard-Sprosse A-21
    - Der Mauszeiger A-21
    - Die Fangpunkte A-22
    - Das Arbeiten mit Fangpunkten A-22
  - Die Werkzeuge A-40
    - Die Werkzeuge verwenden A-40
    - Die Vermaßungswerkzeuge A-74
  - Einstellungen A-75
    - Vermaßungen ein- und ausblenden A-76
    - Vermaßung von Bohrpunkten darstellen A-81
    - Maße eingeben A-82
    - Programmsprache wählen A-84
  - Stammdaten in A+W CAD Designer (Bars) A-85
    - Sprossentypen A-86
    - Sprossenstäbe A-88
    - Wegfallsprossen A-89
    - Stammdaten anlegen A-91
    - Stammdaten schützen A-95
    - Übungen A-96
- Sprossen A-98
  - Neue Konstruktionen A-99
    - Allgemeine Vorgehensweise A-100
    - Form für die Konstruktion festlegen A-100
    - Eigenschaften der Scheibe definieren A-101
    - Sprossen platzieren A-102
    - Gleiche lichte Felder A-103
    - Gleicher Bohrpunktabstand A-104
    - Gleicher Bohrpunktabstand (Bezug auf Scheibe) A-105
    - Gleiche Sprossenlänge A-106
    - Kundendefiniert A-107
  - Sprossen tauschen A-109
  - Demos und Übungen A-110
- Zuschnitt und Messen A-121
  - Zuschnittinformationen anzeigen A-122
  - Zuschnitt am Anfang und am Ende der Sprosse A-123
  - Abstände oder Längen messen A-126
- Spezialmuster A-127
  - Sondermuster A-127
    - Sondermuster erstellen A-128
- Fassaden A-130
  - Fassadenanlage A-131
  - Abmessungen der einzelnen Scheiben angeben A-131
  - Demos und Übungen A-132
    - Trainerdemo: Fassadenanlagen erläutern A-132
    - Übung 1: Erstellen einer Fassadenanlage A-132
    - Übung 2: Nachbildung einer Fassadenanlage A-134
- Makros A-137
  - Allgemein A-138
  - Makro laden A-138
  - Demos und Übungen A-139
    - Trainerdemo: Vorhandene Makros erläutern A-139
    - Trainerdemo: Ein vorhandenes Makros ändern A-139
    - Trainerdemo: Eigene Makros erstellen A-139
    - Übung 1: Platzieren Sie das Makro York3H1S auf einer Scheibe A-140
    - Übung 2: Änderungen am Makro York3H1S auf der Scheibe vornehmen A-142
    - Übung 3: Änderungen am Makro York3H1S vornehmen und das Makro unter einem anderen Namen speichern A-144
    - Übung 4: Erstellen eines eigenen Makros A-145
    - Übung 5: Makro erstellen und mittels Referenzpunkt platzieren A-153
- Datenaustausch A-166
  - Datenimport A-166
    - Übergabedateien A-167
    - Dateien importieren - Neu A-167
  - Datenexport A-169
    - Konstruktionen und Übergabedateien A-169
    - Drucker einrichten A-169
    - Konstruktionen drucken A-171
    - Übergabedatei drucken A-171
  - Bild exportieren A-173
  - Nachrichten senden A-174
- Konfiguration A-174
- Anhang - Makrokatalog A-175

### Überblick

Die Schulung zum Produkt A+W CAD Designer (Bars) ist für Mitarbeiter konzipiert, die sich mit der Erstellung einfacher und komplexer Sprossenkonstruktionen beschäftigen. Die Teilnehmer lernen, Stammdaten anzulegen und Sprossenkonstruktionen zu erstellen.

Für häufig vorkommende Konstruktionen lernen die Teilnehmer das Erstellen und den Umgang mit Makros. Mit Hilfe dieser Makros können sich Anwender in einfacher Weise einen Motiv-Katalog erstellen.

#### Themenblöcke
In diesem Tutorial finden Sie folgende Themenblöcke:
- A+W CAD Designer (Bars) stellt sich vor
- Arbeiten mit A+W CAD Designer (Bars)
- Einstellungen
- Stammdaten in A+W CAD Designer (Bars)
- Sprossen
- Zuschnitt und Messen
- Spezialmuster
- Datenaustausch
- Konfiguration
- Anhang - Makrokatalog

> **Vorausgesetzte Kenntnisse**
> EDV-Grundkenntnisse bzw. Windows-Kenntnisse werden bei den Anwendung von A+W CAD Designer (Bars) vorausgesetzt.

### Aufbau des Tutorials

Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

- **Überblick**: Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
  - Lernziele: Was soll vermittelt werden?
  - Nutzen: Wofür können Sie dieses Wissen einsetzen?
  - Merksätze: Welche Zusammenhänge müssen Sie sich merken?
- **Konzepte**: Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.
- **Übungen**:
  - Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen und Lösungsvorschlägen.
  - Die Übungen helfen Ihnen A+W CAD Designer (Bars) zu verstehen und anwenden zu lernen.
- **Querverweisteil**: Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf entsprechende Beschreibungen in der Softwarereferenz hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.
- **Lesehinweis**: Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen. Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

Im Praxisteil jeder Schulungseinheit werden die Softwarereferenz und der Übungsteil über Querverweise systematisch einbezogen. Dadurch entsteht ein roter Faden durch die gesamte Dokumentation.

## A+W CAD Designer (Bars) stellt sich vor

Originelle Architektur und individueller Geschmack finden immer mehr auch Ausdruck in ausgefallenen Sprossenkonstruktionen. Die Häufung der Sonderkonstruktionen macht den Einsatz eines leistungsfähigen Konstruktionsprogramms erforderlich, das auch in der Lage ist, sofort ein Bild der gewünschten Sprossenanordnung auf dem Bildschirm, über einen Drucker oder Plotter in Originalgröße auszugeben.

A+W CAD Designer (Bars) ist ein Sprossenkonstruktionsprogramm mit grafischer Oberfläche, die es ermöglicht, die Mehrzahl gebräuchlicher Sprossentypen beliebig auf Rechteck- oder Modellscheiben anzuordnen. Es können Sprossen mit unterschiedlichen Breiten in eine Konstruktion eingesetzt werden, außerdem ist es möglich, verschiedene Sprossentypen innerhalb eines Sprossenbildes zu verwenden. A+W CAD Designer (Bars) ermöglicht Konstruktionen mit geraden Sprossen, Bogensprossen und Sprossen unter freiem Winkel.

Zu beachten sind jedoch die landesüblichen Spezifikationen. So gibt es in Deutschland überwiegend Dreh- und Kippfenster nach innen. In Amerika hingegen kommen überwiegend Schiebefenster bzw. Kurbelfenster nach außen zum Einsatz.

### Sprossenaufteilung

A+W CAD Designer (Bars) stellt eine Automatik für die häufigsten Sprossenaufteilungen wie etwa gleiche lichte Felder zur Verfügung. Daneben können auch komplett freie Konstruktionen bequem mit Hilfe von Hilfspunkten erstellt werden. Diese Hilfspunkte können, wie in CAD-Programmen üblich, aus einer Reihe von geometrischen Operationen (z. B. Schnittpunkt oder Abstand) erzeugt werden. Darüber hinaus können einzelne Sprossen oder auch Sprossengruppen auf vielfältige Weise manipuliert werden (verschieben, drehen, spiegeln etc). Details lassen sich mit Hilfe von Ausschnittvergrößerungen sichtbar machen.

### Sprossenabgleich

Der Abgleich der Sprossen erfolgt auf einer Arbeitsfläche, auf der Scheiben beliebig zueinander angeordnet und dargestellt werden können. Gleichzeitig können Sie die Sprossenaufteilung der Fassadenfläche anpassen. D.h. der optisch einwandfreie Verlauf von Sprossen kann über alle Scheiben einer Fassade fortgesetzt werden.

### Ausgabe

Zur Ausgabe wird eine maßstabgetreue Zeichnung gedruckt, die auch die Liste der zu schneidenden Profile enthält. Diese Zeichnung enthält außerdem alle relevanten Informationen für die Sprossenkreuzungen, wie z. B. den Fräswinkel. Alle Produktionspapiere sind frei gestaltbar und können auf dem Monitor oder als Ausdruck ausgegeben werden. Die Ausgabe kann auch über einen Plotter im Maßstab 1:1 erfolgen.

### Makros

Bei häufig vorkommenden Konstruktionen finden sogenannte Makros ihren Einsatz. Die Makros werden auf einfache Art und Weise erstellt. Bei ihrer Anwendung müssen dann lediglich noch die für die Konstruktion zwingend erforderlichen Maße eingegeben werden. Mit Hilfe dieser Makros können sich Anwender in einfacher Weise einen Motiv-Katalog erstellen.

### Vermaßung

Die Vermaßung der fertigen Konstruktion kann den individuellen Produktionsanforderungen angepasst werden. So ist es z. B. möglich, die Bohrpunktinformation sowohl in Bezug auf die Innenkante als auch in Bezug auf die Außenkante des Rahmens zu erstellen.

### Weitere Details

Die integrierte Datenschnittstelle ermöglicht Ihnen einen reibungslosen Datenimport. Weiterhin können NC-Codes für diverse Maschinen (z. B. Hegla Sprossensäge, Rottler & Rüdiger-Säge und Montagezentrum) erzeugt werden.

## Arbeiten mit A+W CAD Designer (Bars)

In diesem Themenblock lernen Sie die Oberfläche von und den Umgang mit A+W CAD Designer (Bars) kennen.

### Oberfläche von A+W CAD Designer (Bars)

> **Lernziele**
> - Oberfläche von A+W CAD Designer (Bars) kennenlernen
> - Fangpunkte kennenlernen und verstehen
> - Die Werkzeuge kennenlernen und verstehen
> - Inhalte des Wertefensters verstehen
> - Unterschiedliche Darstellung der Mauszeiger kennenlernen

> **Nutzen**
> Das Arbeiten in A+W CAD Designer (Bars) ist nur dann sinnvoll möglich, wenn Sie die zur Verfügung gestellten Werkzeuge anwenden können. Je besser Sie die Werkzeuge von A+W CAD Designer (Bars) kennen um so effizienter können Sie arbeiten.

> **Definitionen**
> **Symbolleiste**: ist die waagerechte Leiste mit kleinen, bebilderten Schaltflächen.
> **Werkzeuge**: helfen Ihnen bei der Konstruktion von Sprossenbildern.
> **Wertefenster**: Abhängig von der Auswahl erhalten Sie Informationen zu verbauten Materialien bzw. deren Anzahl.
> **Konstruktionsbereich**: In diesem Bereich erstellen Sie die Sprossenkonstruktion.
> **Fangpunkte**: helfen Ihnen beim Platzieren von Sprossen.

> **Merke**
> **Symbolleiste, Werkzeuge, Wertefenster und Fangpunkte**: können mit der Maus an jede x-beliebige Stelle verschoben werden.
> **Fangpunkte**: Die Funktionen können über das Menü Ansicht beliebig ein- und ausgeblendet werden.
> **Unterschiedliche Mauszeiger**: Abhängig von dem, was Sie tun, ändert sich in A+W CAD Designer (Bars) das Aussehen des Mauszeigers.

### Programm-Präsentation

Wenn Sie A+W CAD Designer (Bars) gestartet haben, stellt sich das Programm wie folgt dar:

Im oberen Bereich befinden sich jeweils von links nach rechts die Menüleiste (A), die Symbolleiste (B) sowie die definierte Standard-Sprosse (C). Unter der Standard-Sprosse finden Sie die Werkzeuge (D) und das Wertefenster (E). Am rechten Bildschirmrand befinden sich die Fangpunkte (G). Die große Fläche in der Mitte ist der Konstruktionsbereich (F).

- **A** Menüleiste
- **B** Symbolleiste
- **C** Eingestellte Standard-Sprosse
- **D** Werkzeuge
- **E** Wertefenster
- **F** Konstruktionsbereich
- **G** Fangpunkte

> **Elemente verschieben**
> Mit Ausnahme der Menüleiste können Sie alle Elemente mit der Maus anfassen und beliebig verschieben. Dadurch können Sie den Konstruktionsbereich variabel gestalten.

### Die Menüleiste

Die Menüleiste beinhaltet die für den Anwender wichtigsten Funktionen. Die einzelnen Menüs können per Mausklick geöffnet werden. Einige Menüpunkte können mit Hilfe von Tastenkombinationen direkt geöffnet werden.
`Datei Bearbeiten Makro Info Stammdaten Ansicht Hilfe`

### Die Symbolleiste

Die Funktion, die mit einer Symbolschaltfläche ausgeführt werden kann, steht Ihnen auch über die Menüs zur Verfügung. In A+W CAD Designer (Bars) gibt es folgende Symbolschaltflächen:

#### Erläuterung der einzelnen Symbole

| Symbol | Erläuterung |
| :--- | :--- |
| Neue Konstruktion | Neue Konstruktion (Scheibe, Makro, Fassadenanlage). Wenn Sie diese Symbol-Schaltfläche betätigen, erstellen Sie eine neue Datei. Befindet sich noch eine Konstruktion auf Ihrer Arbeitsfläche werden Sie gefragt, ob Sie diese speichern möchten. Anschließend wird die Arbeitsfäche geleert. |
| Öffnen | Öffnen einer Konstruktion. Wenn Sie diese Symbol-Schaltfläche betätigen, können Sie eine Datei öffnen. Es erscheint der Dialog Datei öffnen.... |
| Speichern | Speichern einer Konstruktion. Wenn Sie diese Symbol-Schaltfläche betätigen, können Sie eine Datei speichern. |
| Drucken | Drucken einer Konstruktion. Wenn Sie diese Symbol-Schaltfläche betätigen, können Sie eine Konstruktion drucken. Bitte beachten Sie, dass der gewünschte Drucker eingerichtet ist. |
| Importieren | Importieren einer Übergabedatei. Wenn Sie diese Symbol-Schaltfläche betätigen, importieren Sie Dateien, die von übergeordneten Systemen an A+W CAD Designer (Bars) übergeben werden. |
| Übergabedatei drucken | Drucken einer Übergabedatei. Wenn Sie diese Symbol-Schaltfläche betätigen, können Sie eine vom übergeordneten System übergebene Datei drucken. Bitte beachten Sie, dass der gewünschte Drucker eingerichtet ist. |
| Ausschnitt vergrößern | Ausschnitt vergrößern. Es stehen zwei Varianten zur Verfügung: Pro Mausklick wird die Konstruktion um 10% vergrößert. Bei gehaltener Maustaste wird ein gewählter Bereich vergrößert. |
| Ausschnitt verkleinern | Ausschnitt verkleinern. Pro Mausklick wird die Konstruktion um 10% verkleinert. |
| Alles | Alles. Die Konstruktion wird so vergrößert oder verkleienert, dass sie komplett dargestellt werden kann. |
| Rückgängig | Rückgängigmachen der letzten Aktion. |
| Wiederherstellen | Wiederherstellen der letzten rückgängig gemachten Aktion. |
| Hilfe | Hilfe aufrufen. |
| Stammdaten | Stammdaten öffnen. Wenn Sie diese Symbol-Schaltfläche betätigen, öffnet sich der Dialog Stammdaten. |

> **Symbolleiste verschieben**
> Sie können die Symbolleiste mit der Maus anfassen und an einer anderen Stelle platzieren.

### Das Wertefenster

Die Inhalte des Wertefensters ändern sich je nach Auswahl. Haben Sie innerhalb einer Konstruktion eine Sprosse oder ein Segment ausgewählt, zeigt Ihnen A+W CAD Designer (Bars) den entsprechenden Artikel, die Breite, die Farbe sowie die durchgehende Sprosse. Das Feld ID erscheint nur bei einer A+W Business-Anbindung und wird dann automatisch gefüllt.

| Titel | Wert |
| :--- | :--- |
| Sprossenartikel | 004a |
| Sprossenbreite | 26.00 |
| Frästiefe | 6.50 |
| Sprossenfarbe | Gold |
| Durchgang | Senkrecht |
| Sprossenlänge | 778.00 |

> **Werte für Vermaßung**
> Haben Sie die Vermaßung aktiviert, können Sie diese anklicken und der Wert erscheint ebenfalls im Wertefenster. Etwaige Änderungen an den Vermaßungen können im Wertefenster bequem vorgenommen werden.

Betätigen Sie die Schaltfläche [Mengen], zeigt Ihnen A+W CAD Designer (Bars) die Anzahl der Konstruktionsmerkmale. Diese Merkmale sind relevant für die Preisfindung.

| Titel | Wert |
| :--- | :--- |
| Randstopfen | 11 |
| Kreuz | 1 |
| Feld | 15 |
| L-Verbindung | 1 |
| T-Verbindung | 2 |
| X-Verbindung | 2 |
| Bogen 90° | 1 |
| Bogen 180° | 1 |
| 3-Sonne | 2 |
| Mond 1 | 1 |

### Die Standard-Sprosse

Bei der Sprosse, die Sie hier sehen, handelt es sich um die sogenannte Standard-Sprosse. D. h. solange Sie keine andere Sprosse wählen, werden Konstruktionen mit dieser Sprosse erstellt. Diese Sprosse wird bei jedem Programm-Start aktiviert. Sie können die Sprosse jederzeit temporär wechseln, indem Sie aus der Kombobox eine andere Sprosse wählen.

Welche Sprosse als Standard-Sprosse definiert ist, legen Sie im Dialog Stammdaten-Editor fest.

### Der Mauszeiger

In Abhängigkeit von dem, was Sie gerade tun, kann der Mauszeiger von A+W CAD Designer (Bars) sein Aussehen verändern. Im Anschluss haben wir die unterschiedlichen Mauszeiger aufgelistet:

- Im normalen Arbeitsbetrieb sieht der Mauszeiger sieht wie folgt aus: (Normaler Pfeil-Cursor)
- Sie können mit ihm einzelne Elemente markieren bzw. Werkzeuge und Fangpunkte aktivieren.
- Wenn Sie mit Fangpunkten arbeiten und den Mauszeiger auf einem solchen Fangpunkt platzieren, ändert er sein Aussehen zu einem Fadenkreuz.
- Das Fadenkreuz erleichtert Ihnen das Arbeiten. Immer, wenn sich der Mauszeiger zu dem Fadenkreuz ändert, haben Sie den Fangpunkt quasi getroffen.
- Zum Ändern der durchgehenden Sprosse, ändert der Mauszeiger sein Aussehen wie folgt: (Kreuz mit Pfeilen)
- Zum Verlängern von Sprossen, ändert der Mauszeiger sein Aussehen wie folgt: (T-förmiger Cursor)

Wie Sie das Werkzeug anwenden, wird im Bereich Die Werkzeuge detailliert erklärt.

**Ergänzende Informationen**
- "Die Werkzeuge verwenden" auf Seite A-40
- "Ändert den Sprossendurchgang" auf Seite A-59
- "Verlängert eine Sprosse" auf Seite A-60

### Die Fangpunkte

In A+W CAD Designer (Bars) haben Sie die Möglichkeit, Hilfspunkte sogenannte Fangpunkte auf der Konstruktion zu platzieren. Diese Fangpunkte können beliebig eingefügt werden und helfen Ihnen, Segmente (Sprossen, Bögen, etc.) korrekt zu platzieren. Steht Ihr Mauszeiger auf der Scheibe und Sie betätigen die rechte Maustaste, setzt A+W CAD Designer (Bars) automatisch jeweils in den Ecken und in der Mitte der Fläche einen Fangpunkt. Diese automatisch gesetzten Fangpunkte werden in grüner Farbe dargestellt. Fangpunkte, die Sie manuell platzieren, werden in roter Farbe dargestellt.

#### Das Arbeiten mit Fangpunkten

Die folgende Tabelle gibt Ihnen eine Überblick zu den Fangpunkten, die Ihnen in A+W CAD Designer (Bars) zur Verfügung stehen.

| Symbol | Erläuterung |
| :--- | :--- |
| Lösche | Löscht einen Fangpunkt. "Löscht einen Fangpunkt" auf Seite A-39 |
| Lösche alle | Löscht alle Fangpunkte. "Löscht alle Fangpunkt" auf Seite A-39 |
| Einteilung | Eingabe der Anzahl der Intervall-Teilungen für Objekt, Distanz und Parallel. "Erzeugt Fangpunkt(e)" auf Seite A-24 |
| Schnittpunkt | Erzeugt Fangpunkte in allen Schnittpunkten zweier Objekte. "Erzeugt Fangpunkt in Schnittpunkt" auf Seite A-25 |
| Relativ | Erzeugt einen Fangpunkt relativ zu einem beliebigen Punkt. "Erzeugt einen relativen Fangpunkt" auf Seite A-25 |
| Objekt | Erzeugt Fangpunkte auf Sprosse, Rahmen oder Scheibenrand. "Erzeugt Fangpunkte auf Objekten" auf Seite A-26 |
| Rechteck | Erzeugt vier Fangpunkte auf den Ecken eines durch zwei Mausklicks beschriebenen Rechtecks. "Erzeugt vier Fangpunkte auf den Ecken eines Rechtecks" auf Seite A-27 |
| Flucht | Erzeugt Fangpunkte in allen Schnittpunkten mit anderen Sprossen. "Erzeugt Fangpunkte in Kreuzungen" auf Seite A-28 |
| Distanz | Erzeugt Fangpunkte auf einer Geraden. "Anzahl Fangpunkte von (Startpunkt) bis (Endpunkt) erzeugen" auf Seite A-29 |
| Bogenlänge I | Erzeugt in wählbarer Entfernung einen Fangpunkt auf einem Bogen. "Anzahl Fangpunkte von (Startpunkt) bis (Endpunkt) erzeugen" auf Seite A-29 |
| Mittelpunkt I | Erzeugt Fangpunkte in möglichen Mittelpunkten von Kreisen (2 Punkte). "Platziere Fangpunkt in möglichem Mittelpunkt" auf Seite A-30 |
| Parallel | Erzeugt Fangpunkte parallel versetzt zu einer Geraden. "Erzeugt Fangpunkte parallel zu einer Geraden" auf Seite A-33 |
| Bogenlänge II | Erzeugt einen Fangpunkt in wählbarer Entfernung entlang des Bogens. "Platziere Fangpunkt in wählbarer Entfernung entlang eines Bogens" auf Seite A-34 |
| Mittelpunkt II | Erzeugt Fangpunkte im Mittelpunkt eines Kreises (3 Punkte). "Erzeugt Fangpunkt im Mittelpunkt eines Kreises (3 Punkte)" auf Seite A-35 |
| Richtung | Erzeugt Fangpunkte vom Bezugspunkt aus unter einem einstellbaren Winkel. "Erzeugt Fangpunkte unter einstellbarem Winkel" auf Seite A-37 |
| Vektor | Erzeugt einen Fangpunkt auf einer Geraden im wählbaren Abstand vom Startpunkt. "Erzeugt einen Fangpunkt auf einer Geraden mit wählbarem Abstand vom Startpunkt" auf Seite A-38 |

#### Beispiele zu Fangpunkten

Nachfolgend finden Sie zu jedem Fangpunkt ein Beispiel, in dem die Vorgehensweise erläutert wird.

**Erzeugt Fangpunkt(e)**
Mit diesem Werkzeug haben Sie die Möglichkeit, Fangpunkte durch die Eingabe von Intervallen zu setzen.
1. Wählen Sie das Werkzeug aus. Es öffnet sich der Dialog Eingabe-Intervalle für Fangpunkte.
2. Geben Sie die Anzahl der Intervalle (Bereiche zwischen den Fangpunkten) ein, z. B. 3.
3. Es werden vier Fangpunkte werden gesetzt.

**Erzeugt Fangpunkt in Schnittpunkt**
Mit diesem Werkzeug haben Sie die Möglichkeit, Fangpunkte in den Schnittpunkten von Sprossen zu setzen.
1. Wählen Sie das Werkzeug aus.
2. Klicken Sie die erste Sprosse an, z. B. die Horizontale.
3. Klicken Sie die zweite Sprosse an, z. B. die Vertikale.
4. Der Fangpunkt wird in dem Schnittpunkt der beiden ausgewählten Sprossen gesetzt.

**Erzeugt einen relativen Fangpunkt**
Mit diesem Werkzeug haben Sie die Möglichkeit, einen Fangpunkt relativ zu einem bestimmten Punkt zu setzen.
1. Wählen Sie das Werkzeug aus.
2. Klicken Sie den Bezugspunkt an, z. B. Schnittpunkt beider Sprossen.
3. Es öffnet sich der Dialog Eingabe - Relativer Abstand.
4. Geben Sie im Feld dx den horizontalen Abstand zum Bezugspunkt an, z. B. 80 mm.
5. Geben Sie im Feld dy den vertikalen Abstand zum Bezugspunkt an, z. B. 40 mm.
6. Betätigen Sie die Schaltfläche [OK] um den Dialog zu verlassen.
7. Der Fangpunkt wird gemäß den eingegebenen Koordinaten gesetzt.

**Erzeugt Fangpunkte auf Objekten**
Mit dem Begriff Objekte können Sprossen, Rahmen oder der Scheibenrand gemeint sein.
1. Wählen Sie das Werkzeug aus.
2. Klicken Sie das Objekt an, auf dem die Fangpunkte platziert werden sollen, z. B. die horizontale Sprosse.
3. Die Fangpunkte werden auf der Sprosse platziert.

> **Anzahl der Fangpunkte**
> Die Anzahl der Fangpunkte, die Sie platzieren, können Sie im Werkzeug Anzahl ? einstellen.

**Erzeugt vier Fangpunkte auf den Ecken eines Rechtecks**
Mit diesem Werkzeug haben Sie die Möglichkeit, in einem Kreuz vier Fangpunkte zu setzen. Sie müssen lediglich zwei Fangpunkte angeben und A+W CAD Designer (Bars) setzt die beiden fehlenden automatisch.
1. Wählen Sie das Werkzeug aus.
2. Klicken Sie den ersten Fangpunkt an.
3. Klicken Sie den zweiten Fangpunkt an.
4. Die beiden fehlenden Fangpunkte werden platziert.

**Erzeugt Fangpunkte in Kreuzungen**
Mit diesem Werkzeug haben Sie die Möglichkeit, Fangpunkte in Kreuzungen zu setzen.
1. Wählen Sie das Werkzeug aus.
2. Klicken Sie das Objekt an, auf dem die Fangpunkte platziert werden sollen, z. B. die horizontale Sprosse.
3. Der Fangpunkt wird in der Kreuzung platziert.

**Anzahl Fangpunkte von (Startpunkt) bis (Endpunkt) erzeugen**
Mit diesem Werkzeug haben Sie die Möglichkeit, eine gewünschte Anzahl von Fangpunkten auf einer Sprosse zu setzen. Sie geben lediglich den Start- und Endpunkt an und A+W CAD Designer (Bars) platziert die Fangpunkte automatisch.
1. Wählen Sie das Werkzeug aus.
2. Klicken Sie auf dem Objekt den Startpunkt an, z. B. die horizontale Sprosse.
3. Klicken Sie auf dem Objekt den Endpunkt an.
4. Die Fangpunkte werden auf der Sprosse platziert.

> **Anzahl der Fangpunkte**
> Die Anzahl der Fangpunkte, die Sie platzieren, können Sie im Werkzeug Anzahl ? einstellen.

**Platziere Fangpunkte entlang eines Bogens**
Mit diesem Werkzeug haben Sie die Möglichkeit, einen Fangpunkt in einer frei wählbaren Entfernung (Radius) auf einem Bogen zu platzieren.
1. Wählen Sie das Werkzeug aus.
2. Klicken Sie den Mittelpunkt des Bogens an.
3. Klicken Sie einen Punkt auf dem Bogen an. Es öffnet sich der Dialog Eingabe: Bogen-Segmentlänge. Geben Sie -45 ein. Schließen Sie den Dialog mit der Schaltfläche [OK].
4. Der Fangpunkt wird entsprechend platziert.

> **Fangpunkte setzen**
> Wie Sie auf dem Werkzeug-Symbol erkennen können, wird der Fangpunkt im Uhrzeigersinn gesetzt. Durch die Eingabe der negativen 45 wurde der Fangpunkt entgegen des Uhrzeigersinns gesetzt.

**Platziere Fangpunkt in möglichem Mittelpunkt**
Mit diesem Werkzeug haben Sie die Möglichkeit, einen Fangpunkt als Mittelpunkt eines Kreises zu platzieren.
1. Wählen Sie das Werkzeug aus.
2. Klicken Sie den ersten Punkt auf dem Bogen an.
3. Klicken Sie den zweiten Punkt auf dem Bogen an. Es öffnet sich der Dialog Eingabe: Radius. Geben Sie 200 ein. Schließen Sie den Dialog mit der Schaltfläche [OK].
4. Die Fangpunkte werden entsprechend platziert.
Durch diese Eingabe war es A+W CAD Designer (Bars) möglich, zwei Fangpunkte zu setzen. Zur Verdeutlichung haben wir in der folgenden Grafik die entsprechenden Kreise eingezeichnet. Wir erinnern uns, als Radius 200 eingegeben zu haben.

**Erzeugt Fangpunkte parallel zu einer Geraden**
Mit diesem Werkzeug haben Sie die Möglichkeit, Fangpunkte parallel zu einer Sprosse zu platzieren.
1. Wählen Sie das Werkzeug aus.
2. Klicken Sie den Startpunkt des Objektes an, zu dem die Fangpunkte parallel platziert werden sollen, z. B. die horizontale Sprosse.
3. Klicken Sie den Endpunkt des Objektes an, zu dem die Fangpunkte parallel platziert werden sollen. Es öffnet sich der Dialog Eingabe: Paralleler Abstand. Geben Sie 100 ein. Schließen Sie den Dialog mit [OK].
4. Die Fangpunkte werden platziert.

**Platziere Fangpunkt in wählbarer Entfernung entlang eines Bogens**
Mit diesem Werkzeug haben Sie die Möglichkeit, einen Fangpunkt in einem definierten Abstand entlang eines Bogens zu platzieren.
1. Wählen Sie das Werkzeug aus.
2. Klicken Sie den Mittelpunkt des Kreises an.
3. Klicken Sie einen Punkt auf dem Bogen an. Es öffnet sich der Dialog Eingabe: Bogenlänge. Geben Sie 100 ein. Schließen Sie den Dialog mit der Schaltfläche [OK].
4. Der Fangpunkt wird platziert.
Zur Verdeutlichung haben wir in der folgenden Grafik den entsprechenden Kreis eingezeichnet. Wir erinnern uns, als Bogenlänge 100 eingegeben zu haben.

**Erzeugt Fangpunkt im Mittelpunkt eines Kreises (3 Punkte)**
Mit diesem Werkzeug haben Sie die Möglichkeit, einen Fangpunkt in den Mittelpunkt eines durch drei Punkte definierten Bogens zu platzieren.
1. Wählen Sie das Werkzeug aus.
2. Klicken Sie den ersten Punkt auf dem Bogen an.
3. Klicken Sie den zweiten Punkt auf dem Bogen an.
4. Klicken Sie den dritten Punkt auf dem Bogen an.
5. Der Fangpunkt wird platziert.
Zur Verdeutlichung haben wir in der folgenden Grafik den entsprechenden Kreis eingezeichnet.

**Erzeugt Fangpunkte unter einstellbarem Winkel**
Mit diesem Werkzeug haben Sie die Möglichkeit, Fangpunkte in einem definierten Winkel zu platzieren.
1. Wählen Sie das Werkzeug aus.
2. Klicken Sie den Bezugspunkt an. Es öffnet sich der Dialog Eingabe: Richtung Winkel (Grad). Geben Sie ein, wie viel Grad der Winkel haben soll, z. B. 45°. Es öffnet sich ein zweiter Dialog Eingabe: Richtung Länge (in mm), z. B. 200.
3. Die Fangpunkte werden entsprechend gesetzt.

> **Anzahl der Fangpunkte**
> Die Anzahl der Fangpunkte, die Sie platzieren, können Sie im Werkzeug Anzahl ? einstellen.

**Erzeugt einen Fangpunkt auf einer Geraden mit wählbarem Abstand vom Startpunkt**
Mit diesem Werkzeug haben Sie die Möglichkeit, einen Fangpunkt auf einer Geraden zu platzieren.
1. Wählen Sie das Werkzeug aus.
2. Klicken Sie den Bezugspunkt an.
3. Klicken Sie einen Punkt in der gewünschten Richtung an. Es öffnet sich der Dialog Eingabe: Abstand. Geben Sie den Abstand ein, z. B. 200.
4. Der Fangpunkt wird entsprechend gesetzt.

**Löscht einen Fangpunkt**
Mit diesem Werkzeug haben Sie die Möglichkeit, einen einzelnen Fangpunkt durch anklicken zu löschen.
1. Wählen Sie das Werkzeug aus.
2. Klicken Sie den Fangpunkt an, den Sie löschen möchten (zweiter von links).
3. Der Fangpunkt wird gelöscht.

**Löscht alle Fangpunkt**
Mit diesem Werkzeug haben Sie die Möglichkeit, alle Fangpunkt mit einem Klick zu löschen.
1. Wählen Sie das Werkzeug aus.
2. Die Fangpunkte werden alle gelöscht.

### Die Werkzeuge

A+W CAD Designer (Bars) verfügt über eine Reihe von Werkzeugen, deren Funktion Ihnen das Arbeiten erleichtern. Die Werkzeuge stehen Ihnen auch über die Menüs zur Verfügung.

#### Die Werkzeuge verwenden

Die folgende Tabelle gibt Ihnen eine Überblick zu den Werkzeugen, die Ihnen in A+W CAD Designer (Bars) zur Verfügung stehen.

| Symbol | Erläuterung |
| :--- | :--- |
| Element auswählen | Element auswählen. |
| Gerade Sprosse | Erzeugt eine gerade Sprosse zwischen zwei Fangpunkten. "Erzeugt eine gerade Sprosse zwischen zwei Fangpunkten" auf Seite A-42 |
| Horizontale Sprosse | Erzeugt eine gerade (horizontale) Sprosse zwischen zwei Fangpunkten. "Erzeugt eine horizontale Sprosse" auf Seite A-43 |
| Vertikale Sprosse | Erzeugt eine gerade (vertikale) Sprosse zwischen zwei Fangpunkten. "Erzeugt eine vertikale Sprosse" auf Seite A-44 |
| Sprosse mit Winkel | Erzeugt eine gerade Sprosse zwischen zwei Fangpunkten unter Eingabe des Winkels. "Erzeugt eine gerade Sprosse mit zwei Mausklicks unter Angabe des Winkels" auf Seite A-45 |
| Gebogene Sprosse | Erzeugt eine gebogene Sprosse zwischen drei Fangpunkten. "Erzeugt eine gebogene Sprosse mit drei Mausklicks" auf Seite A-47 |
| Sprossenkreis | Erzeugt einen Sprossenkreis zwischen zwei Fangpunkten. "Erzeugt einen Sprossenkreis mit zwei Mausklicks" auf Seite A-49 |
| Sonne | Erzeugt eine Sonne in einem lichten Feld. "Erzeugt eine Sonne in einem lichten Feld" auf Seite A-51 |
| Halbmond | Erzeugt einen Halbmond. "Erzeugt einen Halbmond" auf Seite A-54 |
| Bogen | Erzeugt einen Bogen in einem lichten Feld. "Erzeugt einen Bogen in einem lichten Feld" auf Seite A-56 |
| Durchgang ändern | Für eine 90° Kreuzung wird die Durchgangsrichtung geändert. "Ändert den Sprossendurchgang" auf Seite A-59 |
| Verlängern | Sprosse wird bis auf wählbares Objekt verlängert. "Verlängert eine Sprosse" auf Seite A-60 |
| Teilen | Teilt alle Sprossen. "Alle Sprossen teilen" auf Seite A-64 |
| Verbinden | Verbindet alle Sprossen. "Alle Sprossen verbinden" auf Seite A-65 |
| Löschen/Erzeugen | Setzt oder löscht eine Sprosse in einem lichten Feld. "Löscht oder erzeugt eine Sprosse in einem lichten Feld" auf Seite A-66 |
| Neue Scheibe | Erzeugt eine neue Scheibe. Nachdem Sie das Werkzeug aktiviert haben, klicken Sie auf die Scheibe und es öffnet sich der Dialog. Softwarereferenz, "Neue Scheibe" auf Seite A-199 |
| Makro | Erzeugt aus Makro Sprossen-Aufteilung in der Scheibe. |
| SW-Muster | Öffnet den Dialog zur Eingabe von senkrechten und waagerechten Sprossen. |
| Mengen | Zeigt die entsprechenden Mengen im Wertebereich an. |
| YT-Zuschnitt | Ändert den YT-Zuschnitt. "YT-Zuschnitt ändern" auf Seite A-68 |

Abgesehen von den Werkzeugen, die Ihnen über die Symbole zur Verfügung stehen, gibt es in A+W CAD Designer (Bars) noch die folgenden Werkzeuge (Menü Bearbeiten):
- **Drehen**: "Eine Sprosse drehen" auf Seite A-69
- **Spiegeln**: "Eine Sprosse spiegeln" auf Seite A-71
- **Bewegen**: "Eine Sprosse bewegen" auf Seite A-73

#### Beispiele zu den Werkzeugen

Nachfolgend finden Sie zu jedem Werkzeug ein Beispiel, in dem die Vorgehensweise erläutert wird.

**Erzeugt eine gerade Sprosse zwischen zwei Fangpunkten**
Mit diesem Werkzeug haben Sie die Möglichkeit, eine gerade Sprosse in einem freien Winkel zu platzieren. Zum Starten der Sprosse dient ein Fangpunkt. Die Länge der Sprosse definiert sich durch den von Ihnen gewählten Endpunkt.
1. Setzen Sie entsprechende Fangpunkte.
2. Wählen Sie das Werkzeug aus.
3. Klicken Sie den Start(fang)punkt der Geraden an.
4. Klicken Sie den End(fang)punkt der Geraden an.
5. Die Sprosse wird gesetzt.

**Erzeugt eine horizontale Sprosse**
Mit diesem Werkzeug haben Sie die Möglichkeit, eine horizontale Sprosse zu platzieren. Zum Starten der Sprosse dient ein Fangpunkt. Die Länge der Sprosse definiert sich durch den von Ihnen gewählten Endpunkt.
1. Setzen Sie entsprechende Fangpunkte.
2. Wählen Sie das Werkzeug aus.
3. Klicken Sie den Start(fang)punkt der Geraden an.
4. Klicken Sie den Endpunkt der Geraden an.
5. Die Sprosse wird gesetzt.

**Erzeugt eine vertikale Sprosse**
Mit diesem Werkzeug haben Sie die Möglichkeit, eine vertikal Sprosse zu platzieren. Zum Starten der Sprosse dient ein Fangpunkt. Die Länge der Sprosse definiert sich durch den von Ihnen gewählten Endpunkt.
1. Setzen Sie entsprechende Fangpunkte.
2. Wählen Sie das Werkzeug aus.
3. Klicken Sie den Start(fang)punkt der Geraden an.
4. Klicken Sie den Endpunkt der Geraden an.
5. Die Sprosse wird gesetzt.

**Erzeugt eine gerade Sprosse mit zwei Mausklicks unter Angabe des Winkels**
Mit diesem Werkzeug haben Sie die Möglichkeit, eine gerade Sprosse unter Angabe eines frei definierbaren Winkels zu platzieren.
1. Setzen Sie entsprechende Fangpunkte.
2. Wählen Sie das Werkzeug aus.
3. Klicken Sie den Start(fang) punkt der Geraden an.
4. Klicken Sie den Endpunkt der Geraden an. Der Endpunkt dient gleichzeitig als Sprossenlänge.
5. Es öffnet sich der Dialog Eingabe: Winkel. Geben Sie den gewünschten Winkel ein, z. B. -45.
6. Die Sprosse wird gesetzt.

> **Negative Werte**
> Wie Sie auf dem Werkzeug-Symbol erkennen können, wird die Sprosse entgegen des Uhrzeigersinns gesetzt. Durch die Eingabe der negativen 45 wird das Setzen der Sprosse im Uhrzeigersinn erreicht.

**Erzeugt eine gebogene Sprosse mit drei Mausklicks**
Bei diesem Werkzeug stehen Ihnen zwei unterschiedliche Vorgehensweisen zur Verfügung:
1. Sie klicken erst den Mittelpunkt des Bogens an, dann den Anfangs- und anschließend den Endpunkt. Oder
2. Sie klicken erst den Anfangspunkt des Bogens an, dann den Endpunkt und anschließend einen beliebigen Punkt auf dem Bogen.
Wir erläutern die unter 1. beschriebene Vorgehensweise:
1. Setzen Sie entsprechende Fangpunkte.
2. Wählen Sie das Werkzeug aus.
3. Klicken Sie den Mittelpunkt des Kreises an.
4. Klicken Sie den Startpunkt des Kreises an.
5. Klicken Sie den Endpunkt des Kreises an.
6. Die Sprosse wird gesetzt.

**Erzeugt einen Sprossenkreis mit zwei Mausklicks**
Den Sprossenkreis definieren Sie durch den Mittelpunkt des Kreises und einen beliebigen Punkt auf dem Kreis.
1. Setzen Sie entsprechende Fangpunkte.
2. Wählen Sie das Werkzeug aus.
3. Klicken Sie den Mittelpunkt des Kreises an.
4. Klicken Sie den beliebigen (Fang)punkt auf dem Kreis an.
5. Der Sprossenkreis wird gesetzt.

**Erzeugt eine Sonne in einem lichten Feld**
Sie können ein Strahlenmuster mit einer definierten Anzahl von Strahlen erstellen. Die einzelnen Strahlen können auf vier unterschiedliche Weisen platziert werden. Wir erläutern zunächst die Platzierung von fünf Strahlen in gleichem Winkel.
1. Erstellen Sie die Scheibe.
2. Wählen Sie das Werkzeug aus.
3. Klicken Sie die Scheibe (lichtes Feld) an, in der das Strahlenmuster platziert werden soll. Es öffnet sich der Dialog Sonne und Sterne. Aktivieren Sie die Radiotaste Gleiche Winkel. Wählen Sie aus der Kombobox Anzahl der Strahlen 5. Schließen Sie den Dialog mit der Schaltfläche [OK].
4. Das Strahlenmuster wird platziert.
5. Hätten Sie im Schritt 3 statt der Radiotaste Gleiche Winkel die Radiotaste Strahlen in die Ecken aktiviert und als Zuschnittmethode Zuschnitt in Ecke gewählt, wäre das Ergebnis wie folgt: (anderes Muster).
6. Hätten Sie im Schritt 3 statt der Radiotaste Gleiche Winkel die Radiotaste Strahlen in die Ecken aktiviert und als Zuschnittmethode Zuschnitt auf senkrechten Rahmen gewählt, wäre das Ergebnis wie folgt: (anderes Muster).
7. Hätten Sie im Schritt 3 statt der Radiotaste Gleiche Winkel die Radiotaste Strahlen in die Ecken aktiviert und als Zuschnittmethode Zuschnitt auf waagerechten Rahmen gewählt, wäre das Ergebnis wie folgt: (anderes Muster).

**Erzeugt einen Halbmond**
Dieses Werkzeug kommt dort zum Einsatz, wo ein Strahlenmuster platziert wurde. Dort, wo sich die Strahlen der Sonne treffen, können Sie einen Halbkreis einsetzen.
1. Erstellen Sie die Scheibe mit dem Strahlenmuster.
2. Wählen Sie das Werkzeug aus.
3. Bewegen Sie den Mauszeiger zu der Stelle, wo der Halbmond eingefügt werden soll. An der entsprechenden Stelle ändert der Mauszeiger sein Aussehen zu einem Halbkreis.
4. An der gewünschten Stelle angekommen, drücken Sie die linke Maustaste. Im Wertefenster können Sie die notwendigen Einstellungen vornehmen:
   - **Radius**: Wählen Sie den entsprechenden Wert aus.
   - **Orientierung**: Bezieht sich auf die Ausrichtung des Strahlenmusters. Sie können wählen, wie der Halbmond verlaufen soll (von unten nach oben, von oben nach unten, von rechts nach links, von links nach rechts).

**Erzeugt einen Bogen in einem lichten Feld**
1. Erstellen Sie die Scheibe.
2. Wählen Sie das Werkzeug aus.
3. Klicken Sie die Scheibe (lichtes Feld) an, in der der Bogen platziert werden soll.
4. Im Wertefenster können Sie die notwendigen Einstellungen vornehmen.
   - **Modus**: Schneidet senkrechten Rahmen, Trifft Ecke, Schneidet waagerechten Rahmen, Hat Radius von unten gemessen, Hat Radius von oben gemessen.
   - **Radius**: Kann genutzt werden, wenn im Feld Modus die Einstellung 'Hat Radius von ...' gewählt wurde.
   - **Orientierung**: Legt fest, wie der Sprossenbogen verlaufen soll.
Für die folgende Grafik wurden die Einstellungen *Schneidet senkrechten Rahmen* und *Von unten nach oben* gewählt.

**Ändert den Sprossendurchgang**
Mit diesem Werkzeug haben Sie die Möglichkeit, die durchgehende Sprosse zu ändern.
1. Ausgangssituation. Die senkrechte Sprosse ist die Durchgehende.
2. Wählen Sie das Werkzeug aus.
3. Klicken Sie die Sprossenkreuzung an.
4. Der Sprossendurchgang wird geändert. Die waagerechte Sprosse geht durch.

**Verlängert eine Sprosse**
Mit diesem Werkzeug haben Sie die Möglichkeit, eine Sprosse zu verlängern oder abzuschneiden.
1. Eine Sprosse soll verlängert werden.
2. Wählen Sie das Werkzeug aus.
3. Klicken Sie die Sprosse an die verlängert werden soll. Die Sprosse wird in roter Farbe dargestellt.
4. Klicken Sie das Objekt an, auf das die Sprosse verlängert werden soll.
5. Die Sprosse wird verlängert.
6. Oder, wenn Sie eine Sprosse schneiden möchten: Wählen Sie das Werkzeug aus.
7. Klicken Sie die Sprosse an, die abgeschnitten werden soll. Die Sprosse wird in roter Farbe dargestellt.
8. Klicken Sie das Objekt an der Stelle an, an der die Sprosse geschnitten werden soll.
9. Die Sprosse wird geschnitten.

**Alle Sprossen teilen**
Mit einem Mausklick alle Sprossen zu teilen.
1. Ausgangssituation: Die beiden senkrechten Sprossen sind durchgehend.
2. Wählen Sie das Werkzeug aus. Die Sprossen werden geteilt.

**Alle Sprossen verbinden**
Mit einem Mausklick alle Sprossen zu verbinden.
1. Ausgangssituation: Alle Sprossen sind geteilt.
2. Wählen Sie das Werkzeug aus. Die Sprossen werden verbunden.

**Löscht oder erzeugt eine Sprosse in einem lichten Feld**
1. Ausgangssituation: Vollständiges Gitter.
2. Wählen Sie das Werkzeug aus und platzieren Sie den Mauszeiger auf der Sprosse, die entfernt werden soll.
3. Klicken Sie die linke Sprosse an.
4. Die Sprosse wird entfernt und die Sprossendurchgänge werden angepasst.
5. Bewegen Sie den Mauszeiger an die Stelle, an der die Sprosse gelöscht wurde, ändert er sein Aussehen und Sie können durch Betätigen der linken Maustaste die gelöschte Sprosse wieder setzen.

**YT-Zuschnitt ändern**
Bei einem Sprossenkreuz und zusätzlich auftreffenden Y-Sprossen den Zuschnitt für die Y-Sprossen bestimmen.
1. Ausgangssituation: Werkzeug ist nicht aktiv. Alle Sprossen werden symmetrisch geschnitten.
2. Aktivieren Sie das Werkzeug aus. Das Sprossenkreuz wird normal berechnet und nur die beiden Y-Teile auf das Kreuz geschnitten.

**Eine Sprosse drehen**
(Bearbeiten > Drehen) Mit drei Mausklicks eine Sprosse gedreht zu duplizieren.
1. Ausgangssituation: Die zu drehende Sprosse ist markiert.
2. Wählen Sie den Menüpunkt aus. Klicken Sie den Rotationsmittelpunkt an.
3. Klicken Sie den ersten Bezugspunkt für die Rotation an.
4. Klicken Sie den zweiten Bezugspunkt für die Rotation an.
5. Die Sprosse wird dupliziert gedreht.

**Eine Sprosse spiegeln**
(Bearbeiten > Spiegeln) Mit zwei Mausklicks eine Sprosse horizontal oder vertikal zu spiegeln.
1. Ausgangssituation: Die zu spiegelnde Sprosse ist markiert.
2. Wählen Sie den Menüpunkt aus. Klicken Sie den ersten Punkt auf der Spiegelgeraden an.
3. Klicken Sie den zweiten Punkt auf der Spiegelgeraden an.
4. Die Sprosse wird dupliziert gespiegelt.

**Eine Sprosse bewegen**
(Bearbeiten > Bewegen) Eine markierte Sprosse zu verschieben.
1. Ausgangssituation: Die zu bewegende Sprosse ist markiert.
2. Wählen Sie den Menüpunkt aus. Drücken Sie die linke Maustaste und halten Sie diese gedrückt. Bewegen Sie die Sprosse.

### Die Vermaßungswerkzeuge

A+W CAD Designer (Bars) verfügt über zwei Vermaßungswerkzeuge. Sie können zwischen der Vermaßung von absoluten und relativen Bohrpunkten hin und her schalten und festlegen, ob die Scheibe oder der Rahmen der Bezugspunkt sein soll.

- **Vermaßungsdarstellung von:**
  - Absoluten Bohrpunkten
  - Relativen Bohrpunkten

- **Werkzeug 1 (absolut/relativ):**
  - **Deaktiviert**: Vermaßung der absoluten Bohrpunkte.
  - **Aktiviert**: Vermaßung der relativen Bohrpunkte.
- **Werkzeug 2 (Rahmen/Scheibe):**
  - **Deaktiviert**: Vermaßung mit Bezug auf den Rahmen.
  - **Aktiviert**: Vermaßung mit Bezug auf die Scheibe.

> **Checkbox Vermaßung aktivieren**
> Um die Symbol-Schaltflächen benutzen zu können, müssen Sie die Checkbox Vermaßung im Dialog Einstellungen... aktivieren.

**Weitere Informationen zu den Vermaßungswerkzeugen**
- "Vermaßung von Bohrpunkten darstellen" auf Seite A-81
- Softwarereferenz, "Vermaßung" auf Seite A-242

## Einstellungen

> **Lernziele**
> - Vermaßung in A+W CAD Designer (Bars) kennenlernen und verstehen
> - Nummerieren der Sprossen verstehen
> - Unterschied zwischen der Vermaßung von absoluten und relativen Bohrpunkten verstehen
> - Unterschied bei der Vermaßung von Bohrpunkten in Bezug auf Rahmen und Scheibe verstehen
> - Maßsysteme kennenlernen
> - Programm in einer anderen Sprache starten

> **Nutzen**
> Um A+W CAD Designer (Bars) effizient bedienen zu können ist es wichtig, die Einstellungen korrekt vorzunehmen. Für mehrsprachig-arbeitende Unternehmen kann A+W CAD Designer (Bars) während der Laufzeit auf eine andere Sprache gestellt werden.

> **Merke**
> - **Vermaßung**: Die Vermaßung von Sprossen-Konstruktionen kann aktiviert oder deaktiviert werden.
> - **Maßsystem**: A+W CAD Designer (Bars) kann mm oder Inch darstellen.
> - **Sprache zur Laufzeit umstellen**: Die Programm-Sprache kann zur Laufzeit umgestellt werden.
> - **Ziffern, Fräspunkte und Pfeile**: Die Darstellung kann nur erfolgen, wenn die Checkbox Vermaßung aktiv ist!

### Vermaßungen ein- und ausblenden

Sie können entscheiden, ob und wie eine Vermaßung erfolgen soll.

**So aktivieren Sie die Vermaßung**
1. Wählen Sie im Menü **Ansicht > Einstellungen**. Der Dialog **Einstellungen...** wird geöffnet.
2. Aktivieren Sie die Checkbox **Vermaßung**.

**So erfolgt eine Vermaßung mit Pfeilen**
1. Öffnen Sie den Dialog **Einstellungen...**.
2. Aktivieren Sie die Checkbox **Vermaßung**.
3. Aktivieren Sie die Checkbox **Pfeile**.

**So werden die Sprossen mit Ziffern versehen**
1. Öffnen Sie den Dialog **Einstellungen...**.
2. Aktivieren Sie die Checkbox **Vermaßung**.
3. Aktivieren Sie die Checkbox **Ziffern an Sprossen**.
Gleiche Sprossen erhalten dann den gleichen Buchstaben.

**So können Sie sich Fräspunkte anzeigen lassen**
1. Öffnen Sie den Dialog **Einstellungen...**.
2. Aktivieren Sie die Checkbox **Vermaßung**.
3. Aktivieren Sie die Checkbox **Fräspunkte**.

### Vermaßung von Bohrpunkten darstellen

Das Programm unterscheidet zwischen der Vermaßungsdarstellung von:
- Absoluten Bohrpunkten
- Relativen Bohrpunkten

Die Vermaßungsdarstellung der Bohrpunkte ist immer in Zusammenhang mit der Einstellung des Bereiches **Bezug auf** zu sehen (Rahmen oder Scheibe).

**Unterschied absolute Bohrpunkte/relative Bohrpunkte mit Bezug auf Rahmen:**
Die Vermaßungsdarstellung der relativen Bohrpunkte nimmt weniger Platz in Anspruch, bietet aber weniger Informationen auf einen Blick. Die sinnvolle Darstellung hängt von der Komplexität Ihrer Arbeit ab.

**Unterschied absolute Bohrpunkte/relative Bohrpunkte mit Bezug auf Scheibe**

### Maße eingeben

Sie haben die Möglichkeit, die Maßeinheit einzustellen. Maße können in folgenden Einheiten dargestellt werden:
- mm
- Zoll (in Brüchen oder Dezimal)

> **Umrechnung von Maßeinheiten**
> A+W CAD Designer (Bars) kann in unterschiedlichen Maßeinheiten arbeiten. Es ist sogar möglich, die eingestellte Maßeinheit während der Laufzeit umzustellen. Vorhandene Stammdaten werden dann umgerechnet!

**So stellen Sie die Maßeinheit ein**
1. Wählen Sie im Menü **Ansicht > Einstellungen** und wechseln zum Register **Maße**.
2. Wählen Sie die gewünschte Maßeinheit:
   - **Maßeingabe in mm**: Aktivieren Sie diese Radiotaste.
   - **Maßeingabe in Zoll (Brüche)**: Aktivieren Sie diese Radiotaste und geben im Feld **Bruch Nenner** den Nenner an (Bsp.: 32 für 1/32).
   - **Maßeingabe in Zoll (dezimal)**: Aktivieren Sie diese Radiotaste und geben im Feld **Genauigkeit (dezimal)** die Anzahl der Nachkommastellen an (Bsp.: 3 für 2,345).

### Programmsprache wählen

A+W CAD Designer (Bars) kann zur Zeit in sieben Sprachen betrieben werden. Die Sprache kann während der Laufzeit umgestellt werden.

**So wählen Sie eine andere Sprache**
1. Wählen Sie im Menü **Ansicht > Einstellungen** und wechseln zum Register **Sprachauswahl**.
2. Wählen Sie aus der Kombobox die gewünschte Sprache aus.
3. Schließen Sie den Dialog über die Schaltfläche [OK].

## Stammdaten in A+W CAD Designer (Bars)

> **Lernziele**
> - Unterschiedliche Sprossentypen kennenlernen
> - Anlegen neuer Sprossen beherrschen
> - Festlegen der Standard-Sprosse beherrschen
> - Den Stammdaten-Bereich mit einem Passwort schützen

> **Nutzen**
> Um mit A+W CAD Designer (Bars) arbeiten zu können, müssen als erstes die Stammdaten (die Sprossen) definiert werden.

> **Definitionen**
> - **Glasteilende Sprosse**: Echte Sprossen, die eine Scheibe in mehrere kleine Scheiben teilen.
> - **Innenliegende Sprosse**: Sprossen, die in den Scheibenzwischenraum eingebaut werden.
> - **Aufgesetzte Sprosse**: Bestehen aus eingebauten Abstandhalterprofilen und sind mit der Oberfläche verbunden.
> - **Wegfallsprosse**: Sprossen(teile), die zur Erstellung einer Konstruktion benötigt und später gelöscht werden.
> - **Randstopfen**: Schließt die Sprosse und dient als Verbindung zum umlaufenden Abstandhalter.
> - **Durchgang**: Festlegung von Sprossendurchgängen, die von außen mittels Übergabedateien übergeben werden.

> **Merke**
> **Konfiguration**: Der Stammdatenbereich kann vom Anwender selbst konfiguriert werden.

### Sprossentypen

Es gibt verschiedene Arten von Sprossen. Grundsätzlich unterscheiden wir zwischen:
- Glasteilenden Sprossen
- Innenliegenden Sprossen
- Aufgesetzten Sprossen

#### Glasteilende Sprossen
Glasteilende Sprossen sind echte Sprossen bei einem Fenster.
- **Vorteile**: Stabilisieren das Element, gute plastische optische Wirkung, bis zu 138 mm Breite machbar.
- **Nachteile**: Erhöhter Wärmeverlust, können nicht sehr schmal gefertigt werden, nicht reinigungsfreundlich.

#### Innenliegende Sprossen
Bei größeren Glasflächen kann die innenliegende Sprosse schnell zur ersten Wahl werden.
- **Vorteile**: Günstige Variante, Scheiben können komplett geputzt werden, geringerer Wärmeverlust.
- **Nachteile**: Plastische optische Wirkung fehlt, kann zu Klappergeräuschen kommen, eignet sich nicht für jeden Luftzwischenraum.

#### Aufgesetzte Sprossen
Geklebte Sprossen sind schmale Holzleisten, die von außen auf die Scheibe geklebt werden.
- **Vorteile**: Sehr schmale Sprossen mit guter plastischer Wirkung, geringerer Wärmeverlust.
- **Nachteile**: Teurer als innenliegende Sprossen, kann zu Klappergeräuschen kommen, nur bis zu einer geringen Breite machbar, nicht reinigungsfreundlich.

#### Sprossenstäbe
Sprossen werden in Form von Stäben geliefert (meist 6000 mm Länge) in Materialien wie:
- Aluminium
- Kunststoff
- Holz

#### Wegfallsprossen
Bei den Wegfallsprossen handelt es sich um Sprossen, die zur Konstruktion eines Bildes benötigt werden und anschließend ganz oder teilweise wieder gelöscht werden.

### Stammdaten anlegen

Bei den Stammdaten von A+W CAD Designer (Bars) handelt es sich ausschließlich um Sprossendaten. Den Stammdaten-Editor öffnen Sie über **Stammdaten > Stammdaten-Editor**.

#### So erfassen Sie eine neue Sprosse
1. Betätigen Sie die Schaltfläche [Hinzufügen]. Es öffnet sich der Dialog **Eingabe neuer Artikel**.
2. Geben Sie die gewünschte Artikel-Nummer ein und betätigen Sie [OK].
3. Das Feld **Name** wird automatisch vor-belegt, kann aber ersetzt werden.
4. Im Feld **Breite** geben Sie die Breite der Sprosse ein.
5. Im Feld **Frästiefe** geben Sie den entsprechenden Wert ein.
6. Das Feld **Offset** dient der Spezialbehandlung von Bohrmaschinen mit Offset-Bemaßung.
7. **Randabzug**: Wert für Kunststoff-Stopfen hinterlegen.
8. **Spezial-Kreuzung** und **Breite-Kreuz**: Wenn die Checkbox Spezial-Kreuzung aktiviert ist, können Sie im Feld Breite-Kreuz einen Wert hinterlegen.
9. Geben Sie im Feld **Stablänge** die Länge des Sprossenstabes ein.
10. Das Feld **T-Zugabe** wird verwendet, wenn eine Sprosse im rechten Winkel auf eine andere Sprosse zugeschnitten wird.
11. Die Radiotasten im Bereich **Durchgang** dienen der Festlegung von Sprossendurchgängen.
12. Checkbox **Doppelter Zuschnitt**: Verdoppelt die Zuschnittmengen für den Sprossentyp.
13. Checkbox **L-Felder mit Abzug**: Die Randstopfen der Sprosse werden nicht mit vermaßt.
14. Feld **Liniennummer**: Für unterschiedliche Fertigungslinien.
15. Weisen Sie der Sprosse einen **Farbcode** zu.
16. Schaltflächen [Start]: Dienen zur Definition der Standard-Sprosse.

### Stammdaten schützen

Das Ändern der Stammdaten kann verheerende Auswirkungen haben. Schützen Sie sie mit einem Passwort.

**So schützen Sie Ihre Stammdaten mit einem Passwort**
1. Öffnen Sie den **Stammdaten-Editor**.
2. Aktivieren Sie die Checkbox **Passwortschutz**.
3. Verlassen Sie den Dialog mit [OK]. Beantworten Sie die Sicherheitsabfrage mit [Ja].
4. Es öffnet sich der Dialog **Passwort**. Geben Sie das Passwort ein.
5. Wiederholen Sie das Passwort.
6. Betätigen Sie [OK].

### Übungen

#### Übung 1: Einen Sprossenartikel anlegen

**Aufgabenstellung**
Legen Sie einen Artikel mit folgenden Spezifikationen an:
- Artikelnummer: **8500**
- Name der Sprosse: **Aufgesetzte Sprosse**
- Farbcode: **RAL 1004**
- Farbname: **Goldgelb**
- Breite: **26 mm**
- Frästiefe: **6,5 mm**
- Randabzug: **3 mm**
- Stablänge: **6000 mm**
- Doppelter Zuschnitt
- Dieser Artikel soll die Standard-Sprosse sein.
- Schützen Sie den Stammdaten-Bereich mit einem Passwort (**1111**).

**Übung 1: Lösung**

**Artikel anlegen**
1. Öffnen Sie den **Stammdaten-Editor**.
2. Betätigen Sie [Hinzufügen]. Geben Sie **8500** ein. Betätigen Sie [OK].
3. Geben Sie im Feld **Name** `Aufgesetzte Sprosse` ein.
4. Betätigen Sie [Start] um die Sprosse als Standard-Sprosse zu definieren.
5. Geben Sie im Feld **Breite** `26 mm` ein.
6. Geben Sie im Feld **Frästiefe** `6,5 mm` ein.
7. Geben Sie im Feld **Randabzug** `3 mm` ein.
8. Geben Sie im Feld **Stablänge** `6000 mm` ein.
9. Aktivieren Sie die Checkbox **Doppelter Zuschnitt**.
10. Betätigen Sie im Bereich Farbcode [Hinzufügen]. Geben Sie **RAL 1004** ein und [OK].
11. Markieren Sie den Eintrag RAL 1004 im Feld Name und überschreiben Sie ihn mit `Goldgelb`.
12. Markieren Sie den Eintrag RAL 1004 und betätigen Sie [Ändere]. Wählen Sie einen Gelbton aus und betätigen Sie [OK].
13. Betätigen Sie [Start], um die Standard-Farbe zuzuweisen.
14. Aktivieren Sie die Checkbox **Passwortschutz**.
15. Betätigen Sie [OK]. Im Dialog **Passwort** geben Sie `1111` ein und wiederholen die Eingabe.
16. Betätigen Sie [OK].

## Sprossen

In diesem Abschnitt wird Ihnen gezeigt, wie Sie eigene Sprossenkonstruktionen erstellen.

### Neue Konstruktionen

> **Lernziele**
> - Vorgehensweise zum Erstellen neuer Sprossenkonstruktionen verstehen
> - Aufteilung von Sprossen kennenlernen und verstehen
> - Sprossen in vorhandenen Konstruktionen austauschen

> **Nutzen**
> Die vom Kunden gewünschten Sprossenkonstruktionen abbilden und umsetzen zu können.

> **Definitionen: Modellparameter**
> - **W(idth)** = Gesamtbreite
> - **H(eight)** = Gesamthöhe
> - **H1, 2, ...** = bei unterschiedlichen Höhen
> - **W1, 2, ...** = bei unterschiedlichen Breiten
> - **R** = Radius
> - **R1, 2, ...** = bei unterschiedlichen Radien
> - **S** = Stichhöhe
> - **<-->** = Gespiegelte Darstellung (0: ohne, 1: horizontal)
> - **@** = Drehwinkel (90, 180, 270 Grad im Uhrzeigersinn)
> - **Rückschnitt**: Breite des Rahmens plus Versiegelungstiefe
> - **SZR**: Abkürzung für Scheibenzwischenraum

#### Allgemeine Vorgehensweise

Das Erstellen von Sprossenkonstruktionen geschieht in drei Schritten:
1. Form für die Konstruktion festlegen
2. Eigenschaften definieren
3. Sprossen platzieren (Waagerecht/senkrecht, frei, Makro)

##### Form für die Konstruktion festlegen

Die Arbeit beginnt mit der Auswahl einer entsprechenden Form, dem sogenannten Modell. Die mögliche Auswahl hängt vom Umfang des benutzten Modell-Katalogs in Ihrem Hause ab. Der Dialog **Modell-Erfassung** öffnet sich.

- **Parameterübersicht (A)**: Die benötigten Eingaben für das gewählte Modell.
- **Modellvorschau-Fenster (C)**: Zeigt das gewählte Modell maßstäblich an.

##### Eigenschaften der Scheibe definieren

Im nächsten Schritt legen Sie die Eigenschaften fest (Scheibe, Auftrags- und Kundendaten). Der Dialog **Eigenschaften Scheibe** öffnet sich automatisch. Hier legen Sie X- und Y-Position, Auftragsdaten, Kundendaten, etc. fest.

##### Sprossen platzieren

Die Vorgehensweise zum Platzieren von Sprossen ist abhängig von der Komplexität. Für einfache Konstruktionen gibt es den Dialog **Muster: Senkrecht/Waagerecht**.

Bei der Aufteilung der Sprossen unterscheidet A+W CAD Designer (Bars) zwischen:
- Gleiche lichte Felder
- Gleicher Bohrpunktabstand
- Gleicher Bohrpunktabstand (Scheibe)
- Gleiche Sprossenlänge
- Kundenspezifisch

**Beispiel: Gleiche lichte Felder**
Diese Einstellung platziert die Sprossen so, dass alle Felder (waagerecht und senkrecht) gleich groß sind.

**Beispiel: Gleicher Bohrpunktabstand**
Hierbei sind das obere und das untere lichte Feld gleich, das mittlere Feld wird kleiner.

**Beispiel: Gleicher Bohrpunktabstand (Bezug auf Scheibe)**
Ähnlich wie oben, aber die Bohrlöcher werden von der Scheibenhöhe (z.B. 600mm) berechnet.

**Beispiel: Gleiche Sprossenlänge**
Hier haben alle durchgehenden Sprossen die gleiche Länge.

**Beispiel: Kundendefiniert**
Hier können Sie die Position der Sprossen über fixe Werte oder Abstände zwischen den Sprossen definieren.

#### Sprossen tauschen

In A+W CAD Designer (Bars) haben Sie die Möglichkeit, Sprossen in Konstruktionen zu tauschen.

**So tauschen Sie Sprossen aus**
1. Markieren Sie die Sprosse, die getauscht werden soll.
2. Öffnen Sie im Menü **Bearbeiten** den Menüpunkt **Artikel ändern...**.
3. Es öffnet sich der Dialog **Stammdaten**.
4. Wählen Sie die gewünschte Sprosse.
5. Betätigen Sie die Schaltfläche [OK].

### Demos und Übungen

#### Trainerdemo: Modelle erläutern
- Dialog **Modell-Erfassung**: Öffnet sich über die Symbol-Schaltfläche *Neue Scheibe*.

#### Trainerdemo: Eigenschaften der Scheibe definieren
- Dialog **Eigenschaften Scheibe**: Öffnet sich automatisch nach dem Dialog *Modell-Erfassung*.

#### Trainerdemo: Einfaches Sprossenmuster einfügen
- Dialog **Muster Senkrecht Waagerecht**

#### Übung 1: Eine Konstruktion mit Hilfe eines Sprossenmusters erstellen
**Aufgabenstellung:**
Legen Sie eine Sprossenkonstruktion an:
- **Modell-Nummer:** 65 (Höhe: 800 mm, Breite: 600 mm)
- **Eigenschaften der Scheibe:** Rahmenstärke 11 mm, Kunde Albrecht GmbH (Nr. 811), Auftrag 2123, 5 Stück, Baustelle Europaplatz, Isolierglas mit 16 mm Abstandhalter.
- **Muster:** Zwei waagerechte und eine senkrechte Sprosse, senkrechte Sprosse ist durchgängig, gleiche lichte Felder.

**Lösung:**
1. Öffnen Sie den Dialog **Modell-Erfassung**.
2. Wählen Sie Modell-Nummer **065**.
3. Geben Sie Breite **600** und Höhe **800** ein.
4. Füllen Sie den Dialog **Eigenschaften Scheibe** mit den Auftragsdaten.
5. Betätigen Sie die Symbol-Schaltfläche [Neues senkrecht/waagerecht Muster].
6. Geben Sie Anzahl Waagerecht **2** und Anzahl Senkrecht **1** ein.
7. Aktivieren Sie für beide Teilungen die Radiotaste **Gleiche lichte Felder**.
8. Aktivieren Sie bei **Durchgängige Sprossen** die Checkbox **Senkrechte**.
9. Betätigen Sie [OK].

#### Übung 2: Eine freie Sprossenkonstruktion erstellen
Erstellen Sie die gleiche Konstruktion wie in Übung 1, aber frei, ohne das Muster-Werkzeug.

**Lösung:**
1. Erstellen Sie das Modell wie in Übung 1 (Schritt 1-17).
2. Entfernen Sie automatische Fangpunkte (rechte Maustaste auf Scheibe).
3. Setzen Sie über die Fangpunkt-Werkzeuge manuell die benötigten Punkte auf den Rahmen und verbinden Sie diese mit den Sprossen-Werkzeugen.

#### Übung 3: Nachbildung einer Sprossenkonstruktion
**Aufgabenstellung:**
Bilden Sie eine Sprossenkonstruktion nach (Foto):
- Breite: 500 mm, Höhe: 600 mm, Sprosse 12 mm breit.
- Drei waagerechte, zwei senkrechte Sprossen, Sonne mit drei Strahlen.

**Lösung:**
1. Erstellen Sie das Modell (065, 500x600) und füllen die Eigenschaften.
2. Verwenden Sie das Werkzeug **Muster Senkrecht-Waagerecht**.
3. Anzahl Waagerecht: 3, Anzahl Senkrecht: 2.
4. Teilung Waagerecht: **Kundendefiniert**. Teilung Senkrecht: **Gleiche lichte Felder**.
5. Im Dialog **Kundenvorgabe SW-Muster** fügen Sie die drei waagerechten Sprossen mit einem Abstand von 120 (aufsummiert) hinzu.
6. Schneiden Sie die oberen Teile der senkrechten Sprossen ab, sodass Platz für die Sonne entsteht.
7. Fügen Sie mit dem Werkzeug **Sonne** die Sonne mit drei Strahlen im oberen Feld ein.

## Zuschnitt und Messen

> **Lernziele**
> - Informationen zum Zuschnitt kennenlernen und verstehen
> - Strecken vermessen

### Zuschnittinformationen anzeigen

A+W CAD Designer (Bars) liefert auf Knopfdruck alle für den Zuschnitt wichtigen Informationen über **Info > Zuschnitt-Info**.

- **Zuschnitt am Anfang und am Ende der Sprosse**: Die Maßangaben hinter A: (Anfang) und E: (Ende) geben an, wie die Sprosse zugeschnitten wird.
  - **Eine Zahl (z. B. -- 0° --)**: Sprosse wird glatt geschnitten (z.B. bei Stoß auf Rahmen).
  - **Zwei Zahlen (z. B. 45° 0° -45°)**: Sprosse wird von der Mitte der Seite unter den beiden Winkeln geschnitten.
  - **Drei Zahlen (z. B. 56 22 -68)**: Die Sprosse trifft unter dem mittleren Winkel auf eine andere Sprosse.
  - **Zahlen in Klammern (z. B. 68(15,4) - 22(4.1) -56(6,5))**: Mehrere Sprossen treffen in einem Punkt zusammen. Die Zahlen in Klammern geben die Breite des Zuschnitts an.
- **Fräspunkte**: Wird mit dem Buchstaben F: angezeigt, gefolgt von den relativen Fräsmaßen und der Richtung (R für rechts, L für links).

### Abstände oder Längen messen

Das Vermessen geht über zwei Mausklicks mit dem Werkzeug **Info > Messen** oder dem entsprechenden Symbol.

> **Genaues Messen**
> Um möglichst genau die gewünschten Punkte zu treffen, ist es sinnvoll, zuvor Fangpunkte auf die Arbeitsfläche zu setzen.

## Spezialmuster

### Sondermuster

> **Lernziele**
> - Sondermuster kennenlernen und verstehen
> - Eigene Sondermuster erstellen

#### Sondermuster erstellen

Sie können Sondermuster (Rauten oder Rechtecke) automatisch platzieren.
1. Platzieren Sie eine Scheibe.
2. Wählen Sie im Menü **Makro > Spezial Muster > Sondermuster**.
3. Der Dialog **Rauten- bzw. Rechteckmuster...** wird geöffnet.
4. Wählen Sie **Rauten** oder **Rechteck**, geben Sie **Breite** und **Höhe** ein.
5. Steuern Sie die Aufteilung über die Radiotasten (z.B. **Rautensymmetrisch** oder **Sprossensymmetrisch**).

### Fassaden

> **Lernziele**
> - Fassaden kennenlernen und verstehen
> - Eigene Fassade erstellen

#### Fassadenanlage

Mit A+W CAD Designer (Bars) können Sie bis zu vier Scheiben als Fassade positionieren.

**Abmessungen der einzelnen Scheiben angeben**
Über **Makro > Spezial-Muster > Fassadenanlage** öffnet sich der Dialog **Fassadenanlage...**. Hier geben Sie die Abmessungen der einzelnen Scheiben (A, B, C, D) an.

#### Übung 1: Erstellen einer Fassadenanlage
Erstellen Sie eine Fassade mit vier Scheiben unterschiedlicher Größe.

#### Übung 2: Nachbildung einer Fassadenanlage
Bilden Sie eine Fassadenanlage nach einem Foto nach, inklusive Sprossen.

### Makros

> **Lernziele**
> - Sinn und Zweck von Makros verstehen
> - Eigene Makros erstellen und speichern

#### Allgemein

Makros sind Vorlagen, die Sie einmal erstellen und immer wieder verwenden können.

#### Makro laden

Über **Makro > Freies Muster** und Klick auf die Scheibe öffnet sich der Dialog **Makro auswählen**.

#### Demos und Übungen

- **Trainerdemo: Vorhandene Makros erläutern**
- **Trainerdemo: Ein vorhandenes Makros ändern**
- **Trainerdemo: Eigene Makros erstellen**

#### Übung 1: Platzieren Sie das Makro York3H1S auf einer Scheibe
Erstellen Sie eine Scheibe und platzieren Sie das vordefinierte Makro, wobei Parameter wie Rautenbreite und -höhe angepasst werden.

#### Übung 2: Änderungen am Makro York3H1S auf der Scheibe vornehmen
Ändern Sie die platzierte Konstruktion und speichern Sie sie als neue Datei.

#### Übung 3: Änderungen am Makro York3H1S vornehmen und das Makro unter einem anderen Namen speichern
Ändern Sie die Konstruktion und speichern Sie diese als neues Makro.

#### Übung 4: Erstellen eines eigenen Makros
Erstellen Sie eine einfache T-Sprossen-Konstruktion und speichern Sie sie als Makro.

#### Übung 5: Makro erstellen und mittels Referenzpunkt platzieren
Erstellen Sie ein Makro mit einem definierten Referenzpunkt, um es präzise auf verschiedenen Scheiben positionieren zu können.

## Datenaustausch

### Datenimport

> **Lernziele**
> - Das Arbeiten mit Übergabedateien kennenlernen und verstehen
> - Positionen importieren

#### Übergabedateien

Daten werden importiert, wenn A+W CAD Designer (Bars) mit einem übergeordneten System (z. B. A+W Business) eingesetzt wird. Dies geschieht über eine spezielle Schnittstelle (meist Order.XML).

#### Dateien importieren - Neu

**So importieren Sie eine Datei**
1. Wählen Sie im Menü **Datei > Importieren > Übergabedatei**.
2. Der Dialog **Auswahl - Auftrag/Position** wird geöffnet.
3. Markieren Sie eine Position und klicken Sie [OK], um sie zu öffnen, oder [Abgleich] für Fassaden.

### Datenexport

> **Lernziele**
> - Drucken und plotten von Konstruktionen
> - Drucken von Übergabedateien
> - Konstruktionen als Grafiken exportieren

#### Konstruktionen und Übergabedateien

Zur Ausgabe wird eine maßstabgetreue Zeichnung gedruckt.

#### Drucker einrichten

Bevor Sie drucken können, müssen Sie unter **Datei > Druckereinrichtung...** bis zu zwei Drucker (Drucker 1 und Drucker 2/Plotter) definieren.

#### Konstruktionen drucken

Über **Datei > Drucken > Konstruktion** können Sie die erstellten Konstruktionen drucken.

#### Übergabedatei drucken

Übergabedateien können als Liste oder als detaillierte Skizze gedruckt werden.

#### Bild exportieren

Über **Datei > Bild exportieren...** können Sie eine Konstruktion als Grafik (JPG, BMP, PNG) speichern.

#### Nachrichten senden

Über **Datei > Nachricht senden** können Sie die aktuelle Konstruktion als E-Mail-Anhang (.awd-Format) versenden.

## Konfiguration

Das Programm wird durch A+W-Mitarbeiter vor Ort konfiguriert. Änderungen an der Konfiguration sollten nur nach Rücksprache mit A+W vorgenommen werden. Der Zugriff erfolgt über **Stammdaten > Konfiguration bearbeiten**.

## Anhang – Makrokatalog

Hier folgt eine Auflistung der mitgelieferten Makros mit Beschreibung und eventuell notwendigen Eingaben.

- **Makro 2S2W**: 2 senkrechte, 2 waagerechte Sprossen.
- **Makro 2S3W**: 2 senkrechte, 3 waagerechte Sprossen. Abstand vom Rand ist anzugeben.
- **Makro 2SX4W**: 3 senkrechte, 4 waagerechte Sprossen.
- **Makro Crowder**: 21 senkrechte, 13 waagerechte Sprossen.
- **Makro Cumbria**: Vier Rauten. Abstand zum Rand, Breite und Höhe der Rauten sind anzugeben.
- **Makro Diamond1**: 5 waagerechte, 3 senkrechte Sprossen mit drei Rauten. Halbe Rautenhöhe/-breite angeben.
- **Makro Dumfries**: 4 waagerechte, 4 senkrechte Sprossen (Rahmen-Optik). Abstand zwischen Sprossen und zum Rand angeben.
- **Makro Durham**: Achteck mit Verbindung zum Rand. Abstand A und B angeben.
- **Makro Galloway**: Form aus Achteck, Halbkreisen und Rechteck. Abstände und Radius angeben.
- **Makro Kent1 bis Kent5**: Verschiedene Anzahlen von Sprossen mit integrierten Rauten. Breite und Höhe der Rauten angeben.
- **Makro Multi**: 8 waagerechte, 5 senkrechte Sprossen mit festem Abstand von 202 mm.
- **Makro NewVersi**: 5 waagerechte, 5 senkrechte Sprossen.
- **Makro QueenAnn**: 5 waagerechte, 3 senkrechte Sprossen mit integrierten Rauten.
- **Makro Sonne/Sonne1**: Sonnenmuster mit Halbkreis/Bogensprosse. Abstand und/oder Radius angeben.
- **Makro York0Add1, York3H1S**: Senkrechte Sprossen mit integrierten Rauten. Breite und Höhe der Raute angeben.

## Softwarereferenz

- **Bedienung von A+W CAD Designer (Bars)**
  - Softwarebegriffe
  - Programm beenden
- **Übersicht**
- **Umgang mit Dateien**
  - Neue Scheibe
  - Übergabedatei importieren
  - Neue Scheibenposition
  - Drucken
- **Werkzeuge verwenden**
- **Mit Spezialmustern arbeiten**
  - Muster Senkrecht-Waagerecht
  - Kundenvorgabe SW-Muster
  - Rautenmuster...
  - Fassadenanlage...
  - Sonne und Sterne
  - Makro auswählen
- **Messen und Zuschnitt**
  - Abstand
  - Zuschnitt-Informationen
- **Die Stammdaten**
  - Stammdaten
  - Stammdaten-Editor
  - Passwort
- **Ansicht**
  - Vermaßung
  - Maße
  - Sprachauswahl
- **Die Hilfe verwenden**
  - Über CAD Designer

(Die folgenden Abschnitte bieten eine detaillierte Referenz zu den oben genannten Punkten, die bereits im Tutorial-Teil behandelt wurden.)

## Help Cards

### Informationen zu den HelpCards

Die Darstellungen in den Help Cards basieren auf der Auslieferversion A+W CAD Designer 2014. Einzelne Schritte in den Workflows können je nach Konfiguration abweichen.

### Stammdaten

| Help Card | Themen |
| :--- | :--- |
| Werkzeuge | Sie erhalten einen Überblick über die Werkzeuge. |
| Fangpunkte | Sie erhalten einen Überblick über die Fangpunkte. |
| Sprossen anlegen | Einen Sprossenartikel anlegen. |
| Stammdaten schützen | Die Stammdaten mit einem Passwort schützen. |

#### Werkzeuge (Bar 01-001)

- **Ziel der Handlung**: Sie erhalten einen Überblick über die Werkzeuge.
- **Workflow**: Eine Übersicht der Werkzeug-Symbole und deren Funktion wird bereitgestellt.

#### Fangpunkte (Bar 01-002)

- **Ziel der Handlung**: Sie erhalten einen Überblick über die Fangpunkte.
- **Workflow**: Eine Übersicht der Fangpunkt-Symbole und deren Funktion wird bereitgestellt.

#### Sprossen anlegen (Bar 01-003)

- **Ziel der Handlung**: Einen Sprossenartikel anlegen.
- **Workflow**:
  1. Öffnen Sie den Dialog **Stammdaten-Editor**.
  2. Klicken Sie auf [Hinzufügen] und geben die Artikel-Nummer ein.
  3. Geben Sie **Breite**, **Frästiefe**, **Randabzug**, **Stablänge** etc. ein.
  4. Legen Sie Durchgänge, Zuschnittoptionen und Farben fest.
  5. Bei Bedarf als Standard-Sprosse mit [Start] definieren.

#### Stammdaten schützen (Bar 01-004)

- **Ziel der Handlung**: Die Stammdaten mit einem Passwort schützen.
- **Workflow**:
  1. Öffnen Sie den **Stammdaten-Editor**.
  2. Aktivieren Sie die Checkbox **Passwortschutz**.
  3. Klicken Sie auf [OK] und dann auf [Ja].
  4. Geben Sie im Dialog **Passwort** das gewünschte Passwort ein und bestätigen es.

### Sprossen

| Help Card | Themen |
| :--- | :--- |
| Eigenschaften der Scheibe | Die Eigenschaften der Scheibe definieren. |
| Einfaches Sprossenmuster | Zwei senkrechte und zwei waagerechte Sprossen platzieren. |
| Sprossen über Werte | Sprossen über feste Werte platzieren. |
| Modell mit Sprossen | Ein Modell mit Sprossen platzieren. |
| Freie Sprossenkonstruktion | Eine freie Sprossenkonstruktion erstellen. |

#### Eigenschaften der Scheibe (Bar 02-001)

- **Ziel der Handlung**: Die Eigenschaften der Scheibe definieren.
- **Workflow**:
  1. Klicken Sie auf die Symbol-Schaltfläche [Neue Scheibe].
  2. Wählen Sie Modell-Nr. und Maße im **Modell-Erfassung**-Dialog.
  3. Im Dialog **Eigenschaften Scheibe** Position, Ausrichtung und Auftragsdaten eintragen.

#### Einfaches Sprossenmuster platzieren (Bar 02-002)

- **Ziel der Handlung**: Zwei senkrechte und zwei waagerechte Sprossen platzieren.
- **Workflow**:
  1. Klicken Sie auf [Neues senkrecht/waagerecht Muster].
  2. Geben Sie die Anzahl der Sprossen ein.
  3. Wählen Sie die Teilungs- und Durchgangsoptionen (z.B. "Gleiche lichte Felder", "Senkrechte" durchgehend).

#### Sprossen über Werte platzieren (Bar 02-003)

- **Ziel der Handlung**: Sprossen über feste Werte platzieren.
- **Workflow**:
  1. Öffnen Sie den Dialog **Muster Senkrecht-Waagerecht**.
  2. Wählen Sie "Kundendefiniert" als Teilungsoption.
  3. Im Dialog **Kundenvorgabe SW-Muster** fügen Sie die Sprossen mit exakten Abständen vom Scheibenrand hinzu.

#### Modell mit Sprossen platzieren (Bar 02-004)

- **Ziel der Handlung**: Ein Modell mit Sprossen platzieren.
- **Workflow**:
  1. Erstellen Sie ein Modell (z.B. Rundbogen 065).
  2. Verwenden Sie das Werkzeug **Muster Senkrecht-Waagerecht**, um Sprossen im Modell zu platzieren.

#### Freie Sprossenkonstruktion erstellen (Bar 02-005)

- **Ziel der Handlung**: Eine freie Sprossenkonstruktion erstellen.
- **Workflow**:
  1. Erstellen Sie ein Modell.
  2. Platzieren Sie ein Grundgitter mit dem Muster-Werkzeug.
  3. Modifizieren Sie das Gitter manuell, indem Sie Teile löschen/schneiden und neue Elemente (z.B. eine "Sonne") hinzufügen.

### Spezialmuster

| Help Card | Themen |
| :--- | :--- |
| Fassadenanlage erstellen | Eine Fassadenanlage platzieren. |
| Makro laden | Ein vorhandenes Makro laden. |
| Ein Makro ändern und speichern | Ein vorhandenes Makro abändern und speichern. |
| Eigenes Makro erstellen | Ein eigenes Makro erstellen. |

#### Fassadenanlage erstellen (Bar 03-001)

- **Ziel der Handlung**: Eine Fassadenanlage platzieren.
- **Workflow**:
  1. Wählen Sie im Menü **Makro > Spezial Muster > Fassadenanlage**.
  2. Geben Sie die Abmessungen für bis zu vier Scheiben ein.
  3. Klicken Sie [OK] und definieren die Eigenschaften der Scheiben.

#### Makro laden (Bar 03-002)

- **Ziel der Handlung**: Ein vorhandenes Makro laden.
- **Workflow**:
  1. Platzieren Sie eine Scheibe.
  2. Klicken Sie auf die Symbol-Schaltfläche [Neues Makro].
  3. Wählen Sie das gewünschte Makro aus der Liste.
  4. Geben Sie ggf. die abgefragten Parameter (z.B. Rautenhöhe) ein.

#### Ein Makro ändern und speichern (Bar 03-003)

- **Ziel der Handlung**: Ein vorhandenes Makro abändern und speichern.
- **Workflow**:
  1. Platzieren Sie ein Makro wie oben beschrieben.
  2. Modifizieren Sie die Konstruktion (z.B. durch Löschen von Sprossen).
  3. Wählen Sie **Datei > Speichern unter...**, um die Konstruktion als neue Datei zu speichern oder **Makro > Speichern** um ein neues Makro zu erstellen.

#### Eigenes Makro erstellen (Bar 03-004)

- **Ziel der Handlung**: Ein eigenes Makro erstellen.
- **Workflow**:
  1. Öffnen Sie über **Makro > Neues Makro** eine leere Makro-Arbeitsfläche.
  2. Erstellen Sie die gewünschte Konstruktion mit Fangpunkten und Werkzeugen.
  3. Definieren Sie Parameter (editierbare Abstände) über den Dialog **Relativer Abstand**.
  4. Speichern Sie die Konstruktion über **Makro > Speichern**.

## Index

(Eine alphabetische Liste aller im Dokument vorkommenden Begriffe mit den entsprechenden Seitenzahlen.)
