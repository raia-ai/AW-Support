---
description: "A+W Production Feinplanung - Tutorial und Softwarereferenz"
---


# Tutorial: Abstellplätze und -modi

---
## Übung 2: Einen Fächerwagen anlegen

Richten Sie einen Abstellplatz für Fächerwagen ein.

### Aufgabenstellung

- **Gestellart:** Fächerwagen
- **Anzahl Fachnummern:** 99
- **Max. Anzahl Fächerwagen:** 50

### Übung 2: Lösung

Das Ergebnis dieser Aufgabe sieht so aus:

**Screenshot-Beschreibung: Fächerwagen-Konfiguration**

- **Titel:** Fächerwagen
- **Buttons:** Hinzufügen, Entfernen, Umbenennen
- **Name:** Harp Rack(Fächerwagen)
- **Anzahl Fachnummern:** 99
- **Breite:** 200 mm
- **Checkbox:** Zwei Fächer/Nummer (nicht aktiviert)
- **Start = 0**
- **Anzahl der Stellen für Fachnummer:** 2
- **Max. Anzahl Fächerwagen:** 50
- **Überprüfung Anzahl (Zuschnitt):** 0: Fächerwagen
- **Maximale Nutzlast (kg):** 0
- **Leergewicht (kg):** 0
- **Abstand erstes/letztes Fach v. Achsen:** 0 mm
- **Max. Abweichung Schwerpunkt v. Mitte (%):** 0.00

*(Abb. D-21 Abstellplatz)*

---

## Übung 3: Einen festen Abstellplatz anlegen

Richten Sie einen festen Abstellplatz ein.

### Aufgabenstellung

- **Gestellart:** Fester Abstellplatz
- **Abstelltiefe:** 1000 mm
- **Breite:** 2000 mm
- **Max. Anzahl FAPs:** 99

---

## Übung 3: Lösung

Das Ergebnis dieser Aufgabe sieht so aus:

**Screenshot-Beschreibung: Feste Abstellplätze Konfiguration**

- **Titel:** Feste Abstellplätze
- **Buttons:** Hinzufügen, Entfernen, Umbenennen
- **Name:** Fix rack (FAP)
- **Abstelltiefe:** 1000 mm
- **Breite:** 2000 mm
- **Max. Anzahl FAPs:** 99
- **Checkbox:** Überprüfung Anzahl (Zuschnitt) (nicht aktiviert)
- **Maximales Gewicht (kg):** 0

*(Abb. D-22 Fester Abstellplatz)*

### Ergänzende Informationen:
- ⇨ Tutorial, "Böcke (Abstellplätze)" auf Seite D-241
- ⇨ Softwarereferenz, “Abstellplätze" auf Seite D-372

---

# Optimierungsmodi

In diesem Themenblock lernen Sie Optimierungen kennen und erfahren, wie Sie damit in der A+W Production umgehen.

Der Themenblock beinhaltet folgende Schulungseinheiten:
- Überblick
- Unterschiedliche Optimierungs-Modi

## Überblick

### Lernziele
- Die unterschiedlichen Optimierungs-Modi kennenlernen und verstehen.
- Unter welchen Umständen wird welcher Modus verwendet.
- Entsprechende Einstellungen in A+W Production kennenlernen und verstehen.

### Nutzen
Nur wenn Sie die unterschiedlichen Optimierungs-Modi kennen und verstehen, können Sie die A+W Production-Feinplanung auf Ihre Produktion so anpassen, dass diese kostengünstig und zeitsparend arbeitet.

### Definitionen
- **Einheit:** Unter Einheit versteht man zwei oder mehr Scheiben Glas, welche zusammengehören, da sie später in einem Produktverbund zusammengebaut werden, z. B. ISO oder VSG.
- **Gruppe:** Die Gruppe bezieht eine Stückzahl mit ein. Sie gruppiert Einheiten nach bestimmten Kriterien, wie z. B. Kundennummer und Auftragsnummer.
- **Supergruppe:** Supergruppen vereinigen verschiedene Gruppen. Dadurch können beispielsweise drei zusammengehörige Gruppen durch ein gleichartiges Regelwerk behandelt werden. Bsp.: Sortierung auf Gestelle, da alle drei Gruppen (z. B. Aufträge) an den selben Kunden oder das selbe Projekt gehen.

> **Merke**
> Bei der Wahl der Optimierung muss ein Kompromiss gefunden werden zwischen dem besten Optimierungserfolg (geringer Verschnitt) und der besten Produktionsreihenfolge für die Montage.

## Unterschiedliche Optimierungs-Modi

Bei der Wahl der Optimierung muss immer ein Kompromiss gefunden werden zwischen dem besten Optimierungserfolg (geringer Verschnitt) und der besten Produktionsreihenfolge für die Montage.

A+W Production verwendet die folgenden Optimierungsmodi:
- 6.2
- 6.1
- 5.2
- 5.1
- Freie Optimierung

### Optimierungsmodus 6.2 - Feste Reihenfolge

Dieser Optimierungsmodus arbeitet mit einer strikten Reihenfolge. Nichts lässt sich ändern und die Scheiben werden in einer 100% strikten Reihenfolge produziert. In dieser Reihenfolge werden sie zur Produktion freigegeben.

- Die Reihenfolge der Gruppen ist fest.
- Die Reihenfolge der Scheiben innerhalb der Gruppe ist fest.

> **Alternierende Optimierungspositionen für Positionen mit ungleichen Scheiben**
> Positionen mit zwei oder mehr Scheiben einer Glasart, die aber unterschiedliche Geometrien haben, können wie herkömmliche Pärchen abgestellt werden, d.h. auf einen gemeinsamen Stapel und alternierend (Scheibe1, Scheibe3, Scheibe 1, Scheibe3,...). Das gewünschte Verhalten wird nur für A-Böcke verwendet, bei denen der Modus 6.2 (=feste Reihenfolge) eingestellt ist.
> Ein Zusammenlegen von Modellen ist bei diesen Scheiben nur noch mittels A+W Shape Optimizer möglich, nicht mehr über das feinplanungsinterne Zusammenlegen von Modellen!

#### Unter welchen Umständen können Sie diesen Modus verwenden?
- Sie optimieren auf A-Böcke.
- Sie haben einen strengen Produktions- und Lieferplan.
- Sie produzieren entweder nach Kunde oder nach Glasart.
- (Gewöhnlich) haben Sie einen schlechten Verschnitt - das Ergebnis ist jedoch nicht das Hauptkriterium, sondern die Produktion in strikter Sequenz (z. B. Ausrichtung der gesamten Produktion auf Entladereihenfolge des LKW für ein spezifisches Kundenprojekt).
- Sie müssen sicher stellen, dass die großen Scheiben zuerst geschnitten und abgestellt werden, oder Sie benötigen ein zusätzliches Gestell zum Umsortieren.
- Gewöhnlich benötigen Sie eine feste Anzahl an Gestellen (Anzahl an Gruppen = nahezu die Anzahl an physikalischen Gestellen).
- Sie können direkt in Produktions- oder Packmittelreihenfolge optimieren.

Die nachfolgende Grafik zeigt Ihnen sinnbildlich die Auswirkungen dieses Modus:

*(Grafik: Ein Dreieck mit den Ecken "Reihenfolge", "Ausbeute" und "Flexibilität". Ein roter Punkt ist an der Ecke "Reihenfolge" platziert, was anzeigt, dass dieser Modus die Reihenfolge priorisiert.)*

#### Einstellungen in A+W Production
Für eine Optimierung in diesem Modus sind im Programm folgende Einstellungen nötig:
Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Abstellplatz markieren > Einstellungen

**Screenshot-Beschreibung: Einstellungen Abstellplatz für Modus 6.2**
- **Geplanter Optimierungsmodus:** 6/2
- **Optimierungsverhalten:** Gruppen sortiert (6.2)
- **Abstellmodus Gruppen:** nur 1 Gruppe je Stapel

*(Abb. D-23 Optimierungsmodus 6.2)*

#### Ergänzende Informationen:
- ⇨ Tutorial, "Böcke (Abstellplätze)" auf Seite D-241
- ⇨ Softwarereferenz, "Einstellungen-Abstellplatz" auf Seite D-361

### Optimierungsmodus 6.1 - Kunden zusammenhalten
In diesem Optimierungsmodus ist die Reihenfolge innerhalb der Gruppen fest, z. B. nach Abmessungen. Die unterschiedlichen Gruppen können von ihrer Anordnung her verändert werden um das Ergebnis zu verbessern. Ein typisches Kriterium hier wäre:
- Tour | Kunde

Auf diese Weise werden die Kundenpositionen zusammen gefertigt, Sie haben jedoch keinen Einfluss darauf, für welchen Kunde zuerst produziert wird.
- Die Reihenfolge der Gruppen kann verändert werden (X).
- Die Reihenfolge der Scheiben innerhalb der Gruppe ist fest.

#### Unter welchen Umständen wird dieser Modus verwendet?
- Sie optimieren auf A-Böcke.
- Sie haben einen strengen Produktions- und Lieferplan.
- Sie produzieren entweder nach Kunde oder nach Glasart.
- Sie haben einen relativ schlechten Verschnitt (aber besser als mit dem Modus 6.2) - der Verschnitt ist jedoch nicht das Hauptkriterium.
- Sie müssen sicher stellen, dass die großen Scheiben zu erst geschnitten und abgestellt werden, oder Sie benötigen ein zusätzliches Gestell zum Umsortieren.
- Gewöhnlich benötigen Sie eine feste Anzahl an Gestellen (Anzahl an Gruppen = nahezu die Anzahl an physikalischen Gestellen).
- Sie können direkt in Produktions- oder Packmittelreihenfolge optimieren.

Die nachfolgende Grafik zeigt Ihnen sinnbildlich die Auswirkungen dieses Modus:

*(Grafik: Ein Dreieck mit den Ecken "Reihenfolge", "Ausbeute" und "Flexibilität". Ein roter Punkt ist auf der Kante zwischen "Reihenfolge" und "Ausbeute" platziert, was einen Kompromiss zwischen diesen beiden Zielen anzeigt.)*

#### Einstellungen in A+W Production
Für eine Optimierung in diesem Modus sind im Programm folgende Einstellungen nötig:
Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Abstellplatz markieren > Einstellungen

**Screenshot-Beschreibung: Einstellungen Abstellplatz für Modus 6.1**
- **Geplanter Optimierungsmodus:** 6/1
- **Optimierungsverhalten:** Gruppen frei (6.1)

*(Abb. D-24 Optimierungsmodus 6.1)*

#### Ergänzende Informationen:
- ⇨ Tutorial, "Böcke (Abstellplätze)" auf Seite D-241
- ⇨ Softwarereferenz, "Einstellungen-Abstellplatz" auf Seite D-361

### Optimierungsmodus 5.2 - Standard
Dieser Optimierungsmodus ist der Standard-Modus der Feinplanung. Der Gruppierungs- und Sortierungsschlüssel enthält nur die Gruppen-Nr. Das bedeutet, dass jede Position innerhalb der Gruppe ihre eigene Positions-Nr. besitzt und so eindeutig identifiziert werden kann. Daher müssen die Teile innerhalb der Gruppe keine feste Reihenfolge einhalten, sondern können frei optimiert werden.
- Die Reihenfolge der Gruppen ist fest.
- Die Reihenfolge der Scheiben innerhalb der Gruppe kann verändert werden. Nur Einheiten (z. B. für ISO) werden zusammengehalten (X).

#### Unter welchen Umständen wird dieser Modus verwendet?
- Wenn der Modus 5.1 nicht verwendet wird.
- In kombinierten Gruppierungs-/Sortierungsschlüssel nicht die beiden Eigenschaften AUFTRAGSNUMMER und POSITIONSNUMMER verwendet wird.

Die nachfolgende Grafik zeigt Ihnen sinnbildlich die Auswirkungen dieses Modus:

*(Grafik: Ein Dreieck mit den Ecken "Reihenfolge", "Ausbeute" und "Flexibilität". Ein roter Punkt ist auf der Kante zwischen "Reihenfolge" und "Flexibilität" platziert, was einen Kompromiss zwischen diesen beiden Zielen anzeigt.)*

#### Einstellungen in A+W Production
Für eine Optimierung in diesem Modus sind im Programm folgende Einstellungen nötig:
Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Abstellplatz markieren > Einstellungen

**Screenshot-Beschreibung: Einstellungen Abstellplatz für Modus 5.2**
- **Geplanter Optimierungsmodus:** 5/2
- **Optimierungsverhalten:** Standard

*(Abb. D-25 Optimierungsmodus 5.2)*

#### Ergänzende Informationen:
- ⇨ Tutorial, "Böcke (Abstellplätze)" auf Seite D-241
- ⇨ Softwarereferenz, "Einstellungen-Abstellplatz" auf Seite D-361

### Optimierungsmodus 5.1 - ISO auf Fächerwagen oder viele A-Böcke
Der Gruppierungs- und Sortierungsschlüssel enthält nur die Gruppen-Nr. Das bedeutet, dass jede Position innerhalb der Gruppe seine eigene Positions-Nr. besitzt und so eindeutig identifiziert werden kann. Daher müssen die Teile innerhalb der Gruppe keine feste Reihenfolge einhalten, sondern können optimiert werden. Dies ist soweit identisch zum Optimierungsmodus 5.2.
- Die Reihenfolge der Gruppen kann verändert werden (X).
- Die Reihenfolge der Scheiben innerhalb der Gruppe kann verändert werden.
- Nur Einheiten (z. B. für ISO) werden zusammengehalten (X).

#### Unter welchen Umständen wird dieser Modus verwendet?
- Sie optimieren auf Fächerwagen und benötigen zusätzlich einige A-Böcke.
- Sie werden einen guten Verschnitt haben.
- Vor der Auslieferung werden Sie viel umsortieren müssen - dies erfordert eine große Anzahl an physikalischen Gestellen.

Die nachfolgende Grafik zeigt Ihnen sinnbildlich die Auswirkungen dieses Modus:

*(Grafik: Ein Dreieck mit den Ecken "Reihenfolge", "Ausbeute" und "Flexibilität". Ein roter Punkt ist auf der Kante zwischen "Ausbeute" und "Flexibilität" platziert.)*

#### Einstellungen in A+W Production
Für eine Optimierung in diesem Modus sind im Programm folgende Einstellungen nötig:
Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Abstellplatz markieren > Einstellungen

**Screenshot-Beschreibung: Einstellungen Abstellplatz für Modus 5.1**
- **Geplanter Optimierungsmodus:** 5/1
- **Optimierungsverhalten:** Alles frei (5.1)

*(Abb. D-26 Optimierungsmodus 5.1)*

#### Ergänzende Informationen:
- ⇨ Tutorial, "Böcke (Abstellplätze)" auf Seite D-241
- ⇨ Softwarereferenz, "Einstellungen-Abstellplatz" auf Seite D-361

### Optimierungsmodus Freie Optimierung - Scheiben auf Fächerwagen
Freie Optimierung ist die Standardoptimierung für Scheiben auf Fächerwagen. Bei der Freien Optimierung können, ebenso wie für den Handzuschnitt, verschiedene Glasarten/-dicken auf einem Abstellplatz abgestellt werden (verschiedene Stapel).
- Alles ist frei

#### Unter welchen Umständen wird dieser Modus verwendet?
- Sie optimieren auf Fächerwagen (und benötigen zusätzlich einige A-Böcke für besondere Gläser z. B. für große Scheiben).
- Sie werden einen sehr guten Verschnitt haben - der Verschnitt ist der wichtigste Parameter.
- Sie werden viel umsortieren müssen - dies erfordert eine große Anzahl an physikalischen Gestellen.

Die nachfolgende Grafik zeigt Ihnen sinnbildlich die Auswirkungen dieses Modus:

*(Grafik: Ein Dreieck mit den Ecken "Reihenfolge", "Ausbeute" und "Flexibilität". Ein roter Punkt ist an der Ecke "Ausbeute" platziert, was anzeigt, dass dieser Modus die Ausbeute priorisiert.)*

#### Einstellungen in A+W Production
Für eine Optimierung in diesem Modus sind im Programm folgende Einstellungen nötig:
Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Abstellplatz markieren > Einstellungen

**Screenshot-Beschreibung: Einstellungen Abstellplatz für Freie Optimierung**
- **Optimierungsverhalten:** Alles frei (5.1)
- **Abstellmodus:** Zusammen, Kompakt, alternierend (für Fächerwagen)

*(Abb. D-27 Optimierungsmodus Freie Optimierung)*

Sie sehen, es besteht eine Wechselwirkung zwischen Gruppierung und Sortierung, Ergebnis und der Anzahl an Gestellen. Je restriktiver Sie Gruppieren und Sortieren je mehr Einschränkungen haben Sie bezüglich der Optimierung und dem Ergebnis.
Allerdings sind die Gruppierungen und Sortierungen nicht das einzig Wichtige für die Gestellzuweisung und Produktionsorganisation. Der Umgang mit Scheiben verschiedener Größe, Glasarten, Modellen, usw. ist ebenso wichtig wie die Abstellen auf den Gestellen.

### Doppel-Optimierung
Bei der Freien Optimierung kann eine Doppel-Optimierung, d. h. für unterschiedliche Glasarten eine Optimierung mit identischem Schneidplan, durchgeführt werden.
Der Vorteil dieser Art der Optimierung liegt darin, dass die Scheiben einer Einheit trotz Freier Optimierung geordnet abgelegt werden können. Die Scheiben einer Doppel-Optimierung können mit anderen Doppel- oder Freien Optimierungen auf einem Abstellplatz abgelegt werden.

> **Doppel-Optimierung**
> Eine Doppel-Optimierung kann nur für Abstellplätze mit dem Modus **Einheit** eingestellt werden.

---

## Demos und Übungen

In diesem Abschnitt sehen Sie, wie die Optimierung arbeitet.

### Komplexübung: Verschiedene Feinplanungsergebnisse gemeinsam mit dem Trainer vergleichen:
Es wird der Ablauf der Optimierung gezeigt und erläutert.
Folgender Dialog wird unter diesem Aspekt erklärt:
- Dialog Feinplanung für Lauf

#### Schritt 1: Testaufträge erfassen
Erfassen Sie gemeinsam mit dem Trainer zwei Testaufträge, welche verschiedene Produktaufbauten beinhalten. Die Stückzahlen der Positionen sollten jeweils zwischen 20 - 100 Stk. liegen. Es sollten mindestens ISO mit ESG erfasst werden, zusätzlich Float-Einzelscheiben und ESG-Einzelscheiben (über die Positionen und Aufträge verteilt). Es sollten Modelle, große Scheiben und kleinere Scheiben vorhanden sein.

Lasten Sie die Aufträge ein. Bilden Sie mit diesen beiden Testaufträgen und ggf. bereits im System vorhandenen Test- / Trainingsaufträgen einen Lauf (oder mehrere Läufe, je nach Anzahl an Testaufträgen).

Geben Sie den Lauf / die Läufe in die Feinplanung. Schauen Sie sich unter Registerkarte 2 (Bockbelegung) das Ergebnis der Abstellplatzzuweisung durch die Feinplanung an. Klicken Sie nun auf die Schaltfläche Optimierung und sehen sich im A+W Plan Editor die Ergebnisse auf dem Schneidplan an. Was fällt Ihnen auf? Welche Daten können Sie erkennen und wie können Sie die Abstellplatzzuweisung auf dem Schneidplan lesen? Besprechen Sie die Ergebnisse mit Ihrem Trainer.

#### Schritt 2: Wechseln Sie die Organisation
Schließen Sie den Plan Editor und wählen Sie nun unter Registerkarte 5 (Organisation) eine andere Master-Orga aus und führen Sie die Berechnung der Abstellplatzzuweisung neu durch. Betätigen Sie dazu die Schaltfläche Wiederholen. Wechseln Sie nun wieder in Registerkarte 2 (Bockbelegung). Vergleichen Sie die Ergebnisse mit der ersten Abstellplatzzuweisung. Welche Unterschiede erkennen Sie? Besprechen Sie die Ergebnisse mit Ihrem Trainer.

#### Schritt 3: Optimieren Sie den Lauf erneut
Optimieren Sie den Lauf erneut und öffnen den Schneidplan (Plan Editor). Welche Unterschiede erkennen Sie? Besprechen Sie die Ergebnisse mit Ihrem Trainer.

Wechseln Sie in Registerkarte 5 und verändern Sie erneut die Master-Orga, in dem Sie Ihre eigene Orga aus (welche Sie vorher gemeinsam mit dem Trainer definiert haben). Vergleichen Sie die Ergebnisse.

Nehmen nun auch Änderungen an den Einstellungen bezüglich Gruppierung und Sortierung und Abstellmodus vor. Schauen Sie sich die neuen Ergebnisse in der Abstellplatzzuweisung und der Optimierung / dem Schneidplan an. Welche Unterschiede erkennen Sie? Besprechen Sie die Ergebnisse mit Ihrem Trainer.

#### Schritt 4: Orga erweitern
Erweitern Sie Ihre eigene Orga, bspw. um einen zusätzlichen Glastyp oder trennen Sie Modelle-groß von Modelle-klein.
Wiederholen Sie nun Übungsschritt 3 erneut und so oft wie nötig mit verschiedenen Einstellungen und vergleichen Sie jeweils die Ergebnisse.

---

# Orgas

In diesem Themenblock lernen Sie die unterschiedlichen Organisationsformen kennen und erfahren, wie Sie damit in der A+W Production umgehen.

Der Themenblock beinhaltet folgende Schulungseinheiten:
- Organisationsformen
- Produktionsreihenfolge
- A+W Standard-Orgas
- Abstellplatzorganisation

## Organisationsformen

### Lernziele
- Organisationsformen kennenlernen und verstehen.
- Die Auswirkungen der Orgas verstehen.
- Orgas einrichten können.

### Nutzen
Um Läufe korrekt planen zu können, müssen Sie die unterschiedlichen Formen von Organisationen verstehen. Nur dann ist es möglich, die Auswirkungen auf die realen Produktionsabläufe nachvollziehen und vorab planen zu können.

### Definitionen
- **Orga:** Eine Orga ist nichts anderes als ein datentechnisches Regelwerk zur Abbildung der Produktion.
- **Orga-Gruppe:** Die Orga-Gruppe ist ein Strukturelement einer Orga zur genaueren Definition von Regeln und Bedingungen bspw. für unterschiedliche Glasarten (ESG, VSG, ISO) oder um innerhalb einer Glasart (ISO) zwischen der Behandlung von Rechtecken und Modellen zu unterscheiden.

> **Merke**
> - **Verschiedene Orgas:** In Abhängigkeit von der Struktur des Unternehmens können verschiedene Orgas definiert werden.
> - **Orga-Gruppen/Bocktypen:** Eine Orga besteht aus ein oder mehreren Orga-Gruppen, die wiederum aus ein oder mehreren Bocktypen bestehen.
> - **Produktionsreihenfolge:** Die Produktionsreihenfolge innerhalb einer Orga ergibt sich durch die Reihenfolge der Orga-Gruppen.

### Allgemein
Um einen Lauf korrekt und effizient planen zu können, stehen Ihnen in der A+W Production sogenannte Orgas zur Verfügung. Eine Orga ist nichts anderes als ein datentechnisches Regelwerk zur Abbildung der Produktion (bezüglich Produktionswegen, Prozessketten und Laufwegen und Gestellverwaltung). In Abhängigkeit von der Struktur des Unternehmens können beliebig viele Orgas (ESG-Orga, ISO-Orga, Bearbeitungs-Orga, etc.) definiert werden. Die unterschiedlichen Orgas organisieren die Abstellplätze jeweils vor den Produktionsschritten (ISO-Linie, Ofen, etc.).

### Baumstruktur
Um die gewünschte Produktionsreihenfolge erzeugen zu können, wird jedem Lauf von der A+W Production eine sogenannte Master-Orga zugewiesen. Eine Master-Orga ist eine Gruppe von Orgas und besteht aus einer oder auch aus mehreren Orgas. Dabei ist es durchaus möglich, dass in einem Betrieb mehrerer dieser Master-Orgas vorhanden sind. In diesem Fall wird dem Lauf die Master-Orga zugewiesen, die auf die Produktmischung des Laufes am ehesten zutrifft.

Eine Master-Orga muss immer genau eine Standard-Orga (Verwendung) enthalten. Von allen anderen Typen darf eine Master-Orga maximal eine Orga enthalten. Eine Orga besteht aus einer oder mehrerer Orga-Gruppen, die wiederum aus einem oder mehreren Bocktypen bestehen. An den Orga-Gruppen und an den Bocktypen kann man hinterlegen, wie die gewünschte Produktionsreihenfolge aussehen soll.

*(Diagramm: Eine Baumstruktur wird gezeigt, beginnend mit "Master Orga", die sich in "Orga 1" und "Orga 2" verzweigt. "Orga 2" verzweigt sich weiter in "Orga-Gruppe 1", "Orga-Gruppe 2" und "Orga-Gruppe 3". "Orga-Gruppe 2" enthält "Bocktyp 1" und "Bocktyp 2", die jeweils Bedingungen haben.)*

*(Abb. D-28 Beispiel aus der Praxis)*

### Master-Orga
Jede Master-Orga enthält eine Standardverwendungs-Orga. Zusätzlich können für jeden Lostyp noch Verwendungs- und Produktions-Orgas erstellt werden.

Wenn nun ein Teil einer Orga zugewiesen werden soll, wird erst überprüft, ob eine Produktions-Orga für den entsprechenden Lostyp (im folgenden Beispiel 300) vorhanden ist. Wenn keine Produktions-Orga gefunden wird, wird nach einer Standardproduktions-Orga gesucht. Auch die gibt es in unserem Beispiel nicht. D. h. dem Teil wird keine Produktions-Orga zugewiesen. Als nächstes wird die dem Lostyp zugeordnete Verwendungs-Orga gesucht. Falls keine gefunden wird, bekommt das Teil die Standardverwendungs-Orga. Hier ist aber die entsprechende Verwendungs-Orga (300) vorhanden und wird dem Teil zugewiesen.

*(Abb. D-29 Master-Orga Beispiel 1)*
**Diagramm-Beschreibung:**
- A: Master-Orga
- B: Standardverwendungs-Orga (blau)
- C: Produktions-Orga (gelb) für Lostyp 700
- D: Verwendungs-Orga (blau) für Lostyp 700
- E: Teil mit Lostyp 300
- **Logik:** Für Teil E (Lostyp 300) wird die Verwendungs-Orga (300) gefunden. Für einen Teil mit Lostyp 700 würden sowohl Produktions-Orga C als auch Verwendungs-Orga D gefunden.

Für das Teil mit dem Lostyp 700 wird sowohl eine Produktions- als auch eine Verwendungs-Orga gefunden. Es wird also zwei verschiedenen Orgas mit unterschiedlichen Bocktypen (Verwendungs- und Produktionsbock) zugeordnet.

Man kann auch eine Standardproduktions-Orga definieren, die allen Teilen zugewiesen wird, für die keine dem Lostyp entsprechende Standardproduktions-Orga gefunden wird. Im Gegensatz zu der Verwendungs-Orga muss in der Produktions-Orga aber kein Auffang-Abstellplatz für alle Teile, die die Bedingungen keines anderen Abstellplatzes der Orga erfüllen, erstellt werden. Wenn für ein Teil in der Produktions-Orga kein passender Abstellplatz gefunden wird, wird die Zuweisung zu einer Produktions-Orga einfach ignoriert. Das bedeutet, wenn man für bestimmte Lostypen Produktions-Orga zuweisen will, sollte man in dieser Orga einen Auffangabstellplatz erstellen, um zu verhindern, dass die Zuweisung bei einzelnen Teilen einfach ignoriert wird.

*(Abb. D-30 Master-Orga Beispiel 2)*

Die entsprechenden Einstellungen werden im Dialog Orga gemacht:
**Stammdaten > Feinplanung > Orga**

*(Abb. D-31 Master-Orga)*

#### So erstellen Sie eine Master-Orga
1. Wählen Sie in der Menü **Stammdaten > Feinplanung > Orga**.
2. Betätigen Sie die Schaltfläche [Neu]. Es öffnet sich der Dialog **Master-Orga**.
3. Im Feld **Name der Master-Orga** geben Sie einen Namen für die Master-Orga ein.
4. Aktivieren oder deaktivieren Sie die Checkbox **XOPT zusammen abstellen**.
5. Aktivieren oder deaktivieren Sie die Checkbox **Schnell-Orga**.
6. Wählen Sie aus der Kombobox **Fertigungsgruppen** die entsprechende Gruppe.
7. Wählen Sie aus der Kombobox **Pseudoserien** die entsprechende Serie.
8. Wenn es sich um Pseudoserien handelt, tragen Sie im Feld **Mindestmenge** einen entsprechenden Mindestwert ein.
9. Falls Sie Ihr System durch ein speziell angepasstes Script erweitert oder angepasst haben, können Sie dieses Script im Feld **Verwendetes Script** auswählen.
10. Mittels der Schaltfläche **Auffüller** können Sie definierte Auffüllbedingungen auswählen.
11. Erfassen Sie das Feld **Quasi-Teile**. Um sich alle vorhandenen Quasi-Teile anzeigen zu lassen, betätigen Sie die Schaltfläche [...].
12. Aktivieren oder deaktivieren Sie die Checkbox **Verwende Füller**. Bei aktivierter Checkbox müssen die Felder **Start Füller** und **Ende Füller** erfasst werden!
13. Aktivieren oder deaktivieren Sie die Checkbox **Verwende Restblätter**. Bei aktivierter Checkbox müssen die Felder **Start Restblatt** und **Ende Restblatt** erfasst werden!
14. Aktivieren oder deaktivieren Sie die Checkbox **Doppeloptis zusammen**.
15. Aktivieren oder deaktivieren Sie die Checkbox **Verwende Bruchscheiben**. Bei aktivierter Checkbox müssen die Felder **Start Bruch** und **Ende Bruch** erfasst werden!
16. Betätigen Sie die Schaltfläche **Ok**. Die neu angelegte Master-Orga erscheint automatisch im Orga-Dialog.

#### So fügen Sie einer Master-Orga eine vorhandene, neue Orga hinzu
1. Wählen Sie in der Menü **Stammdaten > Feinplanung > Orga**. Das Register **Master-Orga** zeigt alle vorhandenen Master-Orgas.
2. Markieren Sie die Master-Orga, der Sie eine neue Orga hinzufügen möchten.
3. Im Fenster rechts unten sind alle angelegten Orgas enthalten. Markieren Sie die Orga, die Sie der Master-Orga hinzufügen möchten.
4. Betätigen Sie die Schaltfläche [Neu]. Unter der Master-Orga erscheint die neue Orga.

#### So erstellen Sie eine neue Orga
1. Wählen Sie in der Menü **Stammdaten > Feinplanung > Orga**.
2. Öffnen Sie das Register **Produktionsreihenfolge**.
*(Abb. D-32 Register Produktionsreihenfolge)*
3. Betätigen Sie die Schaltfläche [Neu]. Unter der letzten Orga erscheint die neue Orga. Diese trägt zunächst den Namen `unknown / ...`.
4. Markieren Sie diese Orga und betätigen Sie die Schaltfläche [Einstellungen]. Es öffnet sich der Dialog **Orga**.
*(Abb. D-33 Orga Einstellungen)*
5. Ändern Sie im Feld **Name der Orga-Form** den Namen von `unknown` in einen sprechenden Namen.
6. Wählen Sie aus der Kombobox **Typ** den entsprechenden Orga-Typ.
7. Aktivieren Sie die entsprechende Checkbox im Bereich **Abstellmodus**.
8. Füllen Sie gegebenenfalls die Felder im Bereich **Kein Teilen von ... bei Bockbelegung von mehr als** aus.
9. Betätigen Sie die Schaltfläche [OK] um den Dialog zu verlassen.

#### So fügen Sie einer Orga eine neue Orga-Gruppe hinzu
1. Wählen Sie in der Menü **Stammdaten > Feinplanung > Orga**.
2. Öffnen Sie das Register **Produktionsreihenfolge**.
3. Markieren Sie die Orga, der Sie eine neue Orga-Gruppe hinzufügen möchten und betätigen Sie die Schaltfläche [Neu]. Unter der markierten Orga erscheint die neue Orga-Gruppe mit dem Namen `noname`.
4. Markieren Sie die Orga-Gruppe mit dem Namen `noname` und betätigen Sie die Schaltfläche [Einstellungen]. Es öffnet sich der Dialog **Orga-Gruppen**.
5. Vergeben Sie im Feld **Namen** einen sprechenden Namen für die Orga-Gruppe.
6. Wählen Sie aus der Kombobox **Bildung der Gruppen** die entsprechende Gruppierung.
7. Aktivieren oder deaktivieren Sie die Checkbox **Sortierung der Gruppen**.
8. Wählen Sie aus der Kombobox **Sortierung in den Gruppen** die entsprechende Sortierung.
9. Betätigen Sie die Schaltfläche [OK] um den Dialog zu verlassen.

**Ergänzende Informationen**
- ⇨ Tutorial, "Orgas" auf Seite D-296
- ⇨ Softwarereferenz, "Orga" auf Seite D-357
- ⇨ Softwarereferenz, "Orga-Gruppen" auf Seite D-359

#### So legen Sie Gruppierungen und Sortierungen für einen Abstellplatz an
1. Wählen Sie in der Menü **Stammdaten > Feinplanung > Orga**.
2. Öffnen Sie das Register **Produktionsreihenfolge**.
3. Markieren Sie die Orga-Gruppe, für die der Abstellplatz angelegt werden soll und betätigen Sie die Schaltfläche [Neu]. Es wird automatisch ein Abstellplatz mit dem Namen `unknown` angelegt.
4. Markieren Sie den Abstellplatz mit dem Namen `unknown` und betätigen Sie die Schaltfläche [Einstellungen]. Es öffnet sich der Dialog **Einstellungen-Abstellplatz**.
*(Abb. D-34 Einstellungen - Abstellplatz)*
5. Vergeben Sie im Feld **Name** anstelle von `unknown` einen sprechenden Namen für den Abstellplatz.
6. Wählen Sie aus der Kombobox **Bildung der Gruppen** nach welchem Regelwerk die Gruppen gebildet werden sollen (bspw. nach Kunden-Nr. und Auftrags-Nr.).
7. Aktivieren oder deaktivieren Sie die Checkbox **Sortierung der Gruppen**.
8. Wählen Sie aus der Kombobox **Abstellmodus Gruppen** das Abstellverhalten der Gruppen je Stapel.
9. Wählen Sie aus der Kombobox **Optimierungsverhalten**, ob die Reihenfolge der Gruppen sortiert sein soll (Supergruppen), umsortiert sein soll, oder ob alles unsortiert sein soll.
10. Aktivieren oder deaktivieren Sie die Checkbox **Auffang-Abstellplatz**. Jede Orga sollte ein Auffang-Gestell enthalten.
11. Handelt es sich bei dem Abstellplatz um einen **Verwendungsbock**, nehmen Sie im Register **Verwendung** folgende Einstellungen vor:
    - Erfassen Sie die Felder **Von Bis**.
    - Aktivieren Sie die entsprechende Checkbox im Bereich **Abstellmodus**.
    - Aktivieren oder deaktivieren Sie die Checkbox **Zyklische Optimierung**.
    - Erfassen Sie das Feld **Max. Anzahl Gruppen**.
    - Erfassen Sie das Feld **Zyklusgröße**.
    - Aktivieren Sie die entsprechende Checkbox im Bereich **Abstellplatz-Typ**.
12. Handelt es sich bei dem Abstellplatz um einen **Produktionsbock**, nehmen Sie im Register **Produktion** folgende Einstellungen vor:
    - Erfassen Sie die Felder **Von Bis**.
    - Aktivieren oder deaktivieren Sie die Checkbox **Erzeuge Produktionsböcke**.
    - Erfassen Sie das Feld **Max. Anzahl Gruppen**.
    - Aktivieren Sie die entsprechende Checkbox im Bereich **Abstellplatz-Typ**.
13. Betätigen Sie die Schaltfläche [OK] um den Dialog zu verlassen.

### Bruch-Orga
Mit Hilfe der Bruch-Orga können Sie Bruchscheiben nach beliebigen Kriterien auf Böcken abstellen. Die Bruch-Orga prüft automatisch anhand programminterner Bedingungen die Eigenschaften der Bruchscheibe (des Basisglases, d. h. des Floats). Bruch-Orgas definieren Sie, wie die anderen Orga-Formen auch, im Dialog Orga.

### Prüfreihenfolge
In einer Orga werden Abstellplätze angelegt, für die Bedingungen definiert werden. Diese Bedingungen legen die Zuordnung einer Scheibe zu einem bestimmten Abstellplatztyp fest. Die Reihenfolge der Abstellplatztypen wird in der Regel so angeordnet, dass mit den restriktivsten Bedingungen begonnen wird und die Scheiben durch die Prüfreihenfolge der Abstellplatztypen wie durch einen Filter laufen.

*(Abb. D-35 Bedingung des Abstellplatzes: Ein Diagramm zeigt, wie ein "Teil" sequenziell durch die Abstellplatztypen 1 bis 5 geprüft wird.)*

Zuerst werden die Spezialfälle überprüft. So wäre es zum Beispiel möglich, dem in der Prüfreihenfolge an erster Stelle stehenden Abstellplatztyp die Bedingung `Bin Modell` zuzuweisen. Alle Modellscheiben würden sofort diesem Abstellplatztyp zugewiesen. Der zweite Abstellplatztyp würde mit der Bedingung `Kleine Scheiben` alle Scheiben bis zu einer einstellbaren Größe abfangen, etc. Je weiter hinten in der Prüfreihenfolge ein Abstellplatztyp steht, desto schwächer werden die Bedingungen.

Wird für ein Teil in einer Verwendungs-Orga kein Abstellplatztyp gefunden, wird es dem Auffang-Abstellplatz zugeordnet. Ein Auffang-Abstellplatz zeichnet sich dadurch aus, dass er entweder keine Bedingungen hat und somit stets am Ende der Prüfreihenfolge stehen sollte, oder aber das Kennzeichen `Auffang-Abstellplatz` gesetzt ist. Jede Orga-Gruppe darf maximal einen solchen Auffang-Abstellplatz haben, wobei er für die Verwendungs-Orga zwingend vorgeschrieben ist.

#### So ändern Sie die Prüfreihenfolge
1. Wählen Sie in der Menü-Leiste **Stammdaten > Feinplanung > Orga**.
2. Öffnen Sie das Register **Prüfreihenfolge**.
3. Markieren Sie im Bereich der **Orgas** die Orga, für die die Prüfreihenfolge geändert werden soll.
4. Markieren Sie im Bereich der **Abstellplätze** den Abstellplatz, dessen Reihenfolge geändert werden soll.
5. Verschieben Sie die Prüfreihenfolge des markierten Abstellplatzes mit Hilfe der Schaltflächen [Anfang], [Hoch], [Runter] oder [Ende] so lange, bis sich der Abstellplatz an der gewünschten Position befindet.

*(Abb. D-36 Prüfreihenfolge)*

### Orga-Typ und Los-Typ
Jedes Teil bzw. jede Bearbeitung hat seinen Teiletyp bzw. Bearbeitungstyp (Basisglas, VSG, etc.) und seine Beschaffungsart (Bestellt, Zuschnitt, etc.). Abhängig von diesen beiden Eigenschaften wird das Teil bzw. die Bearbeitung einem bestimmten Lostyp zugewiesen. Dadurch können Teile mit unterschiedlichen Bearbeitungstypen ein und dem selben Lostyp zugeordnet und gemeinsam behandelt werden, z.B. bei der Zuweisung von Abstellplätzen.

Darüber hinaus hat jede Orga einen bestimmten Orga-Typ. Mit diesem Orga-Typ wird festgelegt, welche Teile der Orga zugewiesen werden. Idealerweise definieren und filtern Sie nach Unterschieden und Ähnlichkeiten:
- Modelle?, Rechtecke?
- Höhe?, Gewicht?

Produktionslose werden für unterschiedliche Teiletypen und verschiedene Glasarten im Zuschnitt gebildet.

### Verwendungs- und Produktions-Orgas
Neben dem Orga-Typ ist eine weitere Eigenschaft der Orgas die Unterscheidung in Produktions-Orgas und Verwendungs-Orgas. Eine Verwendungs-Orga muss erstellt werden, eine Produktions-Orga kann zusätzlich erstellt werden. Jedes Teil bekommt also eine Verwendungs-Orga und kann bei Bedarf eine zusätzliche Produktions-Orga erhalten.

Für den gleichen Bearbeitungsprozess wird bei einer Verwendungs-Orga immer ein Verwendungsbock eingerichtet. Zusätzlich ist die Einrichtung eines Produktionsbocks möglich. Bei einer Produktions-Orga kann nur ein Produktionsbock erzeugt werden.

Innerhalb einer Verwendungs-Orga sind die Bedingungen für die Verteilung der Scheiben auf Verwendungs- und Produktionsböcke gleich. Die Zuordnung eines Artikels für den gleichen Bearbeitungsprozess zu einer Verwendungs- und einer Produktions-Orga erlaubt innerhalb der Gruppierung und Sortierung eine Verteilung der Scheiben auf Verwendungs- und Produktionsböcke nach jeweils unterschiedlichen Bedingungen. So können z.B. die Scheiben auf den Verwendungsböcken nach ihrer Größe sortiert und nach der Produktion (z.B. bei ESG nach den Öfen) auf die Produktionsböcke nach der Verwendung im ISO oder dem Versand verteilt werden.

Wenn einem Teil für eine bestimmte Bearbeitung eine Produktions-Orga zugeordnet wird, werden die Gruppierungen und Sortierungen auf den Abstellplätzen der Verwendungs-Orga ignoriert. Das Teil wird nach den Gruppierungen und Sortierungen des Produktionsbocks der Produktions-Orga auf die Abstellplätze hinter dem Bearbeitungsprozess verteilt.

**Ergänzende Informationen**
- ⇨ Softwarereferenz, "Produktion" auf Seite D-357

### Globale Einstellungen
Die globalen Einstellungen stehen in Zusammenhang mit den Werten, die Sie in den unten genannten Dialogen und Felder ausgewählt haben:
- **Dialog Orga-Gruppen:**
  - Felder: Bildung der Gruppen, Sortierung in den Gruppen.
- **Dialog Einstellungen-Abstellplatz:**
  - Felder: Bildung der Gruppen, Sortierung in den Gruppen.

> **Angaben in den Voreinstellungen**
> Wurden bei den oben genannten Dialogen aus den Komboboxen der entsprechenden Felder der Wert `Keine` explizit ausgewählt, so werden die Werte der globalen Einstellungen verwendet. Hier sollten Angaben gemacht werden, da beim Starten der A+W Production sonst Fehlermeldungen kommen.

**Ergänzende Informationen**
- ⇨ Softwarereferenz, "Voreinstellungen" auf Seite D-365
- ⇨ Softwarereferenz, "Orga-Gruppen" auf Seite D-359
- ⇨ Softwarereferenz, "Einstellungen-Abstellplatz" auf Seite D-361
- ⇨ Tutorial, “A+W Standard-Orgas" auf Seite D-312

### Demos und Übungen
Öffnen Sie die Stammdaten der Feinplanung. Schauen Sie sich gemeinsam mit dem Trainer bereits vordefinierte Orgas an und analysieren Sie den Aufbau (Baustruktur, verschiedene Abstellplätze, Zuweisung von Bedingungen). Was fällt Ihnen auf? Besprechen Sie die Struktur gemeinsam mit Ihrem Trainer.

---

# Produktionsreihenfolge

### Lernziele
- Die Produktionsreihenfolge kennenlernen und verstehen.
- Die Auswirkungen der Produktionsreihenfolge verstehen.

### Nutzen
Durch die Kenntnisse der Einstellungsmöglichkeiten an den Orga-Gruppen bezüglich Gruppierung und Sortierung können Sie die reale Produktionsreihenfolge von Läufen und einzelnen Gläsern definieren und jederzeit flexibel ändern.

### Definitionen
- **Gruppierungsschlüssel:** Über den Gruppierungsschlüssels in einer Orga-Gruppe haben Sie die Möglichkeit, eine Produktionsreihenfolge zu bestimmen, ohne für die Abstellplätze eine Gruppierung/Sortierung festzulegen.

> **Merke**
> - **Ohne Gruppierung:** Wenn in der Orga-Gruppe keine Gruppenbildung angegeben ist, richtet sich die Produktionsreihenfolge nach der Reihenfolge der Abstellplätze in der Orga-Gruppe.
> - **Mit Gruppierung:** Wenn in der Orga-Gruppe z. B. nach Kunde gruppiert wird, so ergibt sich die Produktionsreihenfolge nicht länger einfach durch die Abfolge der Abstellplätze in der Orga-Gruppe. Das Hauptkriterium ist nun die Eigenschaft Kunde der Teile.

### Allgemein
Die Produktionsreihenfolge innerhalb einer Orga ergibt sich durch die Reihenfolge der Orga-Gruppen. Innerhalb dieser in der Regel durch die Reihenfolge der Bocktypen. Die Reihenfolge innerhalb der Bocktypen wird durch Gruppierungs- und Sortierungsschlüssel hinterlegt.

Damit man nicht die gleiche Sortierung bei jedem Bocktyp innerhalb einer Orga-Gruppe anlegen muss, kann man eine Sortierung in der Orga-Gruppe hinterlegen. Diese wird an die in der Orga-Gruppe enthaltenen Bocktypen vererbt und kann dort ergänzt werden. Gleiches gilt für die Gruppierung.

Allerdings hat die Gruppierung in der Orga-Gruppe noch einen entscheidenden Einfluss auf die Produktionsreihenfolge. Wenn z. B. in der Orga-Gruppe nach `Tour` gruppiert wird, so ergibt sich die Produktionsreihenfolge nicht länger einfach durch die Reihenfolge der Bocktypen in der Orga-Gruppe. Das Hauptkriterium ist nun die Eigenschaft `Tour` der Teile. Das bedeutet, dass zunächst alle Teile der Tour A produziert werden, danach die der Tour B usw. Für eine gegebene Tour wiederum ist allerdings die Reihenfolge der Bocktypen innerhalb der Orga-Gruppe entscheidend.

### Gruppierungsschlüssel der Orga-Gruppen
Das Anlegen eines Gruppierungsschlüssels in einer Orga-Gruppe hat einen entscheidenden Einfluss auf die Produktionsreihenfolge. Er bietet die Möglichkeit, eine Produktionsreihenfolge zu bestimmen, ohne für die Abstellplätze eine Gruppierung/Sortierung festzulegen.

#### Ohne Gruppierung
Wenn in der Orga-Gruppe keine Gruppenbildung angegeben ist, richtet sich die Produktionsreihenfolge nach der Reihenfolge der Abstellplätze in der Orga-Gruppe (z. B. kleine Scheiben, Sprossen, usw.).

*(Abb. D-37 Produktionsreihenfolge ohne Gruppierung in der Orga-Gruppe)*
*(Diagramm: Zeigt zwei Abstellplatztypen A und B. Eine Orga-Gruppe füllt diese sequenziell, erst A, dann B.)*

#### Mit Gruppierung
Wenn in der Orga-Gruppe z. B. nach Kunde gruppiert wird, so ergibt sich die Produktionsreihenfolge nicht länger einfach durch die Abfolge der Abstellplätze in der Orga-Gruppe. Das Hauptkriterium ist nun die Eigenschaft `Kunde` der Teile. Im Beispiel würde dies bedeuten, dass zunächst alle Teile des Kunden A produziert werden, danach die des Kunden B usw. Für einen Kunden richtet sich die Abfolge der Produktion allerdings wieder nach der Reihenfolge der Abstellplätze in der Orga-Gruppe.
Innerhalb der Gruppen ist die Reihenfolge der Teile frei, d. h. es gibt keine Einschränkung bei der Optimierung (XOPTS 5.2).

*(Abb. D-38 Produktionsreihenfolge mit Gruppierung in der Orga-Gruppe)*
*(Diagramm: Zeigt, wie eine Orga-Gruppe zuerst alle Plätze für Kunde A füllt, dann alle für Kunde B.)*

> **Bestimmung der Produktionsreihenfolge durch den Gruppierungsschlüssel**
> Damit die Produktionsreihenfolge durch den Gruppierungsschlüssel der Orga-Gruppe bestimmt werden kann, darf bei den Abstellplätzen keine Sortierung mit Auftrags- und Positions-Nr. eingestellt sein. Dies würde dazu führen, dass die Optimierung nach XOPTS 6.1 durchgeführt und der Gruppierungsschlüssel der Orga-Gruppe ignoriert wird.

---

# A+W Standard-Orgas

### Lernziele
- Unterschiedliche Standard-Orgas kennenlernen und verstehen.
- Entsprechende Einstellungen in A+W Production nachvollziehen können.

### Nutzen
Die Standard-Orgas haben den Vorteil, dass sie bereits vollständig angelegt sind und Sie diese gleich nutzen können. Das spart Ihnen Zeit und minimiert das Fehlerrisiko beim Einrichten.

### Definitionen
- **Standard-Orga:** Fertig eingerichtete Orgas von A+W.

> **Merke bei Änderungen**
> Wir raten Ihnen, die gewünschte Standard-Orga zu kopieren und die kopierte Version dann zu ändern. So bleibt Ihnen das Original immer erhalten und Sie minimieren das Fehlerrisiko.

## Abstellplatzorganisation

Für die Organisation der Glasproduktion mit A+W Production stehen bereits verschiedene Regelwerke, so genannte Standard-Orgas zur Auswahl. Jede Orga sortiert und gruppiert die zu produzierenden Scheiben nach anderen Gesichtspunkten und optimiert die Produktion hinsichtlich unterschiedlicher Anforderungen.
Die folgende Tabelle gibt eine Übersicht über die verfügbaren Orgas und deren Eigenschaften. Die Reihenfolge ist von produktionsorientierten Orgas hin zu versandorientierten Orgas.

| Name | Beschreibung |
| :--- | :--- |
| **A-Böcke SZR** | Diese Orga ist sinnvoll bei einem Bieger, der starke SZR-Restriktionen aufweist und keinen Puffer zum Vorproduzieren und Sortieren der Rahmen hat. Die Orga bietet keine Versandorientierung. |
| **A-Böcke** | Diese Orga liefert eine moderat versandorientierte Produktionsreihenfolge nach Kunde und Auftrag, allerdings mit der Restriktion, dass vor der Linie stets nur von wenigen Böcken abgearbeitet wird. Der Grad der Versandausrichtung kann durch Setzen der globalen Einstellungen für Gruppierung und Sortierung gesteuert werden. Die Orga ist darauf ausgelegt, dass nach der ISO-Produktion umgepackt wird. |
| **A-Böcke Versand** | Diese Orga liefert eine versandorientierte Produktionsreihenfolge, bei der vor der Linie im Wechsel von mehreren A-Böcken abgegriffen wird. Die Orga benötigt Abstellplätze vor und hinter der Linie und liefert eine verpackungsgerechte Produktionsreihenfolge. Hinter der Linie müssen Gestelle je Kunde bereitgestellt werden. |
| **Fächerwagen** | Diese Orga entspricht im Aufbau und der Abstellplatzvergabe weitgehend der Orga A-Böcke, es werden aber Fächerwagen für die Hauptabstellplätze genommen, wodurch i.d.R. ein erheblich besserer Verschnitt gewährleistet ist. Große und kleine Einheiten sowie Serien werden auf A-Böcke herausgezogen. Abweichend zur Orga A-Böcke ist die Produktionsreihenfolge stets versandgerecht. Zwar wird mit der Orga Fächerwagen ebenfalls ein Bock nach dem anderen vor der Linie abgearbeitet, doch können auf Fächerwagen alle benötigten Glasarten zusammengestellt und auf Versandreihenfolge gebracht werden. |
| **Aufgefüllte Fächerwagen** | Diese Orga vermeidet schwach gefüllte Fächerwagen und zieht alle Fächerwagen in Produktionsreihenfolge zusammen. Zuerst werden alle Fächerwagen abgearbeitet, anschließend kommen die Spezialitäten auf A-Böcken. |

*(Tab. D-1)*

### A-Böcke SZR
Diese Orga ist für Isolierglas-produzierende Betriebe sinnvoll bei denen der Bieger starke SZR-Restriktionen aufweist und keinen Puffer zum Vorproduzieren und Sortieren der Rahmen hat. Die Orga A-Böcke SZR bildet eine nach SZR gruppierte Produktionsreihenfolge ab, bei der vor der Linie ein A-Bock nach dem anderen abgearbeitet wird.

- Die Orga bietet keine Versandorientierung.
- Es werden ausschließlich A-Böcke verwendet (Tiefe 200 mm, Breite 2000 mm).
- Abstellmodus ist **Einheit** (die Scheiben einer Einheit stehen auf demselben Abstellplatz auf verschiedenen Stapeln).

#### Produktionsreihenfolge
Die Produktionsreihenfolge bildet sich aus folgenden optimierten Abstellplatzgruppen (in Produktionsreihenfolge):
- Normale ISO-Scheiben
- ISO-Modellscheiben
- ISO-Scheiben mit Sprossen
- ISO-Modellscheiben mit Sprossen
- Stufen-ISO
- 3-fach ISO

Jede dieser Gruppen besteht aus 5 SZR-Abstellplatzgruppen, die in der Produktionsreihenfolge nacheinander abgewickelt werden. Die SZR-Gruppen sind durch einstellbare Schwellwerte getrennt:
- **SZR-Gruppe 1:** > SZR-Schwelle1
- **SZR-Gruppe 2:** > SZR-Schwelle2
- **SZR-Gruppe 3:** > SZR-Schwelle3
- **SZR-Gruppe 4:** > SZR-Schwelle4
- **SZR-Gruppe 5:**

Die Schwellwerte sind wie folgt voreingestellt und können angepasst werden:
- SZR-Schwelle1 = 10 mm
- SZR-Schwelle2 = 12 mm
- SZR-Schwelle3 = 16 mm
- SZR-Schwelle4 = 18 mm

Innerhalb jeder SZR-Abstellplatzgruppe gibt es in Produktionsreihenfolge folgende Abstellplätze (klein nach groß, da hinter der Linie umgepackt werden muss):
- Serien (Serienflag gesetzt oder Stück ≥ 10)
- Kleine Einheiten (Bedingung: kleine Kante < 300 oder große Kante < 500)
- Normale Einheiten
- Große Einheiten (Bedingung: große Kante > 2100 oder kleine Kante > 1600)

Innerhalb jedes Abstellplatzes ist die Produktionsreihenfolge nach Kunden und Auftrag gruppiert. Die Positionsreihenfolge innerhalb eines Auftrags ist frei. Für Scheiben, die nicht in die oben genannten Abstellplatzgruppen passen, sind Auffang-Abstellplätze vorhanden, die aber nicht weiter optimiert sind (ESG-Scheiben, VSG-Scheiben, Nicht zugeordnete Einheiten).

#### Optimierung
Optimierungstechnisch kann bei dieser Orga ein XOPTS ab Modus 5/1 angewendet werden. Je größer die Restriktionen auf einem A-Bock innerhalb eines Abstellplatzes sind, desto größer kann der Optimierungsverschnitt ausfallen. Der Nachteil liegt darin, dass es sehr viele Abstellplätze geben kann und der Sortieraufwand nach der Produktion hoch ist.

#### Nummernkreise
Die zu produzierenden Scheiben werden durch die Orga auf Abstellplätze verteilt. Die folgende Tabelle zeigt die hinterlegten Abstellplätze und Nummernkreise.

*(Die vollständige Tabelle erstreckt sich über die Seiten D-316 bis D-320 des Originaldokuments. Hier ist ein zusammengefasster Auszug.)*

| Orgagruppe | Abstellplatz | Nummernkreis von | bis |
| :--- | :--- | :--- | :--- |
| Auffänger | Auffänger | 10000 | 10999 |
| ESG - bearbeitet | bearbeitet - Serien | 8951 | 8999 |
| ESG - bearbeitet | bearbeitet - große Scheiben | 8921 | 8950 |
| ESG - gesäumt | Gesäumt - große Scheiben | 8421 | 8450 |
| Einfachglas | große Scheiben | 7921 | 7950 |
| Einfachglas - geschliffen | geschliffen - große Scheiben | 7421 | 7450 |
| Iso - Dreifach | Iso - Dreifach - große Einheiten | 6921 | 6950 |
| Iso - Modell-Sprossen-szrgr1 | Iso-1 - Mod-Spross - klein | 1311 | 1320 |
| ... | ... | ... | ... |
| VSG | VSG - große Scheiben | 9921 | 9950 |
| VSG | VSG - kleine Scheiben | 9901 | 9920 |

*(Tab. D-2 Nummernkreise der Produktionsorga A-Böcke SZR)*

Die Orga A-Böcke SZR optimiert auf Einheiten. Sie ist einfach zu handhaben, verursacht aber ggf. einen höheren Sortieraufwand nach der Linie.

*(Grafik: Darstellung einer Produktionslinie mit A-Böcken davor und dahinter.)*

#### Einstellungen in A+W Production für ISO-SZRGR1
- **Einstellungen der Orga-Gruppe:**
  - Name: Iso-szrgr1
  - Bildung der Gruppen: Keine
  - Sortierung in den Gruppen: Keine
  - *(Abb. D-39)*
- **Einstellungen Abstellplatz:**
  - Name: Iso-1-series/HQ
  - Verwendung: Von 1151, Bis 1199
  - Bildung der Gruppen: +KUNDENNUMM+AUFTRAGSI
  - Abstellmodus Gruppen: nur 1 Gruppe je Stapel
  - Optimierungsverhalten: Gruppen frei (6.1)
  - Geplanter Optimierungsmodus: 6/1
  - *(Abb. D-40)*

---

### ISO-A-Böcke
Die Orga A-Böcke liefert eine moderat versandorientierte Produktionsreihenfolge nach Kunde und Auftrag. Es besteht die Einschränkung, dass vor der Linie immer nur von wenigen Böcken abgearbeitet wird. Der Grad der Versandausrichtung kann durch Setzen der globalen Einstellungen für Gruppierung und Sortierung gesteuert werden. Die Orga ist darauf ausgelegt, dass nach der ISO-Produktion umgepackt wird.

- Es werden ausschließlich A-Böcke verwendet (Tiefe 200, Breite 2000).
- Der Abstellmodus ist **Einheit**.

#### Produktionsreihenfolge
Die Reihenfolge bildet sich aus Abstellplatzgruppen wie:
- Normale ISO-Scheiben
- ISO-Modellscheiben
- ISO-Modellscheiben mit Sprossen
- ISO-Scheiben mit Sprossen
- Stufen-ISO
- 3-fach ISO

Diese Gruppen sind unterteilt nach: Serien, Kleine Einheiten, Normale Einheiten, Große Einheiten. Wegen des Umpackens geht die Reihenfolge von klein nach groß.

#### Gruppierung und Sortierung
Die Gruppierung richtet sich nach der globalen Voreinstellung.
- **Voreinstellung:**
  - Gruppierung = Kunde+Auftrag
  - Sortierung = Keine
- **Änderung der Einstellung (bei wenig Platz):**
  - Gruppierung = Artikel+Kunde+Auftrag
  - Sortierung = Keine

#### Nummernkreise
Die folgende Tabelle zeigt die hinterlegten Abstellplätze und Nummernkreise.

*(Die vollständige Tabelle erstreckt sich über die Seiten D-324 und D-325.)*

| Orgagruppe | Abstellplatz | Nummernkreis von | bis |
| :--- | :--- | :--- | :--- |
| Auffänger | Auffänger | 10000 | 10999 |
| ESG - bearbeitet | bearbeitet | 8501 | 8899 |
| Iso | Iso | 1001 | 1899 |
| Iso | Iso - kleine Einheiten | 1901 | 1920 |
| Iso - Dreifach | Iso - Dreifach | 6001 | 6899 |
| Iso - Modelle | Iso-Modelle | 2001 | 2899 |
| Iso - Modelle - Sprossen | Iso-Modell-Sprossen | 3001 | 3899 |
| Iso - Sprossen | Iso-Sprosse | 4001 | 4899 |
| Iso - Stufe | Iso - Stufe | 5001 | 5899 |
| VSG | VSG | 9001 | 9899 |

*(Tab. D-3 Nummernkreise der Produktionsorga A-Böcke)*

Die Orga A-Böcke optimiert stärker versandorientiert. Sie müssen am Linienausgang weniger nachsortieren und benötigen daher weniger Platz für Gestelle.

#### Einstellungen in A+W Production für ISO-Kleine Einheiten
- **Einstellungen der Orga-Gruppe:**
  - Name: Iso
  - Bildung der Gruppen: Keine
  - Sortierung in den Gruppen: Keine
  - *(Abb. D-41)*
- **Einstellungen Abstellplatz:**
  - Name: IG-small sheets
  - Verwendung: Von 1901, Bis 1920
  - Bildung der Gruppen: Global
  - Sortierung in den Gruppen: Global
  - Abstellmodus Gruppen: nur 1 aufgeteilte Gruppe je Stapel
  - Optimierungsverhalten: Gruppen sortiert (6.2)
  - Geplanter Optimierungsmodus: 5/2
  - *(Abb. D-42)*

---

### A-Böcke Versand
Die Orga A-Böcke Versand liefert eine versandorientierte Produktionsreihenfolge, bei der vor der Linie im Wechsel von mehreren A-Böcken abgegriffen wird. Die Einteilung basiert auf Größenklassen, innerhalb derer nach Kunde sortiert wird. Die Idee ist, eine Produktionsreihenfolge von groß nach klein zu erreichen, wobei Kundenaufträge zusammengehalten werden.

- Es werden ausschließlich A-Böcke verwendet (Tiefe 200, Breite 2000).
- Abstellmodus ist **Glas**.

#### Größenklassen
Die Orga arbeitet mit 2 Schwellwerten (S1, S2), um Scheiben in 6 Größenklassen einzuteilen, wobei immer zuerst die kleine Kante geprüft wird.

- **Größenklasse 1:** kleine Kante > Gr_Schwelle_2
- **Größenklasse 2:** kleine Kante > Gr_Schwelle_1 und große Kante ≤ Gr_Schwelle_2
- ... und so weiter für die Klassen 3-6.

#### Produktionsreihenfolge
Die Reihenfolge wird nach dem Schema 1'2'3'4'5'6 (groß nach klein) gebildet. Innerhalb der Größenklassen:
- **ISO Größenklasse 1:** Serie, Normale ISO, ISO-Besonderheiten
- **ISO Größenklasse 2:** Serie, Normale ISO, Stufen-ISO, 3-fach-ISO, etc.
- ... und so weiter.

#### Gruppierung und Sortierung
Die Gruppierung an der Abstellplatzgruppe ist: `Kunde + Artikel + SprossenKZ + Modell + Stufen`. Ein gegebener Kunde ist i.A. im Wechsel von den Gestellen einer Größenklasse abzunehmen.

#### Nummernkreise

*(Die vollständige Tabelle erstreckt sich über die Seiten D-330 und D-331.)*

| Orgagruppe | Abstellplatz | Nummernkreis von | bis |
| :--- | :--- | :--- | :--- |
| Auffänger | Auffänger | 10000 | 10999 |
| ESG - bearbeitet | bearbeitet-- große Scheiben | 8921 | 8950 |
| ISO Grkl 1 | ISO normal Grkl 1 | 1001 | 1499 |
| ISO Grkl 2 | ISO normal Grkl 2 | 2001 | 2499 |
| ... | ... | ... | ... |
| VSG | VSG | 9001 | 9899 |

*(Tab. D-4 Nummernkreise der Produktionsorga A-Böcke Versand)*

Die Orga A-Böcke Versand optimiert direkt auf Verpacken und Versand. Sie benötigen mehr Gestelle am Linienende, aber die Abstelllogik ist einfacher.

---

### Fächerwagen ohne Auffüllen
Diese Orga entspricht weitgehend der Orga A-Böcke, es werden aber Fächerwagen für die Hauptabstellplätze genommen, was zu besserem Verschnitt führt. Große/kleine Einheiten und Serien werden auf A-Böcke herausgezogen. Die Produktionsreihenfolge ist stets versandgerecht.

#### Produktionsreihenfolge
Die Abstellplatzgruppen sind:
- Normale ISO-Scheiben
- ISO-Modellscheiben
- ... etc.
Die Abstellplatzgruppen sind von groß nach klein unterteilt (Serien A-Bock, Große Einheiten A-Bock, Normale Einheiten Fächerwagen, Kleine Einheiten A-Bock).

#### Gruppierung und Sortierung
Die Fächerwagen haben 60 einzeln nummerierte Fächer. Die Sortierung auf den Fächerwagen ist `Kunde+Auftrag+Position`, während die A-Böcke nach `Kunde+Auftrag` gruppiert sind.

> **Fächerwagen nicht aufgefüllt!**
> Bei dieser Organisation ist wichtig, dass Fächerwagen nicht aufgefüllt werden. D. h. ein Fächerwagen wird nicht optimal ausgenutzt. Passt eine Auftragsposition nicht mehr in die restlichen Fächer, wird eine neue Fächerwagennummer vergeben.

#### Nummernkreise

*(Die vollständige Tabelle erstreckt sich über die Seiten D-335 und D-336.)*

| Orgagruppe | Abstellplatz | Nummernkreis von | bis |
| :--- | :--- | :--- | :--- |
| Auffänger | Auffänger | 10000 | 10999 |
| Iso | Iso | 100 | 1899 |
| Iso - Modelle | Iso - Modelle | 2000 | 2899 |
| ... | ... | ... | ... |
| VSG | VSG | 9000 | 9899 |

*(Tab. D-5 Nummernkreise der Produktionsorga Fächerwagen ohne Auffüllen)*

---

### Aufgefüllte Fächerwagen
Diese Orga vermeidet schwach gefüllte Fächerwagen und zieht alle Fächerwagen in Produktionsreihenfolge zusammen. Zuerst werden alle Fächerwagen abgearbeitet, dann die Spezialitäten auf A-Böcke.

#### Produktionsreihenfolge
- Normale ISO (nach Produkttyp sortiert): Fächerwagen
- ISO groß, klein, Serie: A-Böcke
- ISO Modelle groß, klein, Serie: A-Böcke
- ... und so weiter.

Bis auf frei gehaltene Fächer zum Zusortieren werden die Fächerwägen lückenlos gefüllt.

#### Gruppierung und Sortierung
Eine globale Einstellung `Gruppierung = Keine`, `Sortierung = Keine` führt zur Belegung nach Produkteigenschaften (Modelle, Sprossen, Stufen, etc.).
Eine Einstellung `Gruppierung = Kunde+Auftrag` hält Kundenaufträge zusammen.

#### Optimierung
Diese Organisation basiert i.A. auch auf Sequenz-Optimierung, jedoch wird hier aufgefüllt, d. h. die Fächerwagen werden komplett gefüllt, auch wenn eine Auftragsposition gesplittet wird.

#### Nummernkreise

*(Die vollständige Tabelle erstreckt sich über die Seiten D-339 und D-340.)*

| Orgagruppe | Abstellplatz | Nummernkreis von | bis |
| :--- | :--- | :--- | :--- |
| Fächerwage aufgefüllt | Fächerwagen alles | 11000 | 50999 |
| Auffänger | Auffänger | 10000 | 10999 |
| ... | ... | ... | ... |
| VSG | VSG | 9000 | 9899 |

*(Tab. D-7 Nummernkreise der Produktionsorga Aufgefüllte Fächerwagen)*

---

## Demos und Übungen

### Trainerdemo: Stammdaten erläutern
Es werden die Stammdaten der A+W Production gezeigt und erläutert. Folgender Dialog wird unter diesem Aspekt erklärt:
- Dialog Orga, mit den Registern
  - Master-Orga
  - Produktionsreihenfolge
  - Prüfreihenfolge

### Übung 1: Eine Master-Orga anlegen
Erstellen Sie eine Master-Orga gemäß den unten aufgeführten Spezifikationen.

#### Aufgabenstellung
- **Name der Orga:** Neue Trainings-Orga
- **Fertigungsgruppen:** Nach Kundennummer+Auftragsnummer
- **Name der Orga-Form:** Neue Training
- **Typ der Orga-Form:** Standard
- **Abstellmodus:** Einheit
- **Name der Orga-Gruppe:** Auffang-Abstellplatz
- **Einstellungen Abstellplatz:** A-Bock, Supergruppenbildung: +Kundennummer+Auftragsnummer, keine Sortierung in den Gruppen, vollständige Gruppen werden gemeinsam abgestellt, Optimierungsverhalten 5.1, Abstellmodus Einheit.

#### Übung 1: Lösung
- **Master-Orga anlegen**
  1. Öffnen Sie den Dialog Orga über das Menü **Stammdaten > Feinplanung**.
  2. Betätigen Sie die Schaltfläche [Neu]. Es öffnet sich der Dialog Master-Orga.
  3. Geben Sie im Feld **Name der Master-Orga** `Neue Trainings-Orga` ein.
  4. Öffnen Sie die Kombobox **Fertigungsgruppen** und wählen Sie `+Kundennummer-Auftragsnummer` aus.
  5. Betätigen Sie die Schaltfläche [OK].
- **Produktionsreihenfolge anlegen**
  1. Öffnen Sie das Register Produktionsreihenfolge.
  2. Betätigen Sie [Neu].
  3. Betätigen Sie [Einstellungen].
  4. Geben Sie im Feld **Name der Orga-Form** `Neues Training` ein.
  5. Im Bereich **Abstellmodus** aktivieren Sie `Einheit`.
  6. Betätigen Sie [OK].
- **Orga-Gruppe anlegen**
  1. Markieren Sie die Orga-Form `Neues Training` und betätigen Sie [Neu].
  2. Betätigen Sie [Einstellungen].
  3. Geben Sie im Feld **Name** `Auffang Abstellplatz` ein.
  4. Im Bereich **Bildung der Gruppen** wählen Sie `Kundennummer`.
  5. Aktivieren Sie die Checkbox **Sortierung der Gruppen**.
  6. Betätigen Sie [OK].
- **Abstellplatz anlegen**
  1. Markieren Sie die Orga-Gruppe `Auffang Abstellplatz` und betätigen Sie [Neu].
  2. Betätigen Sie [Einstellungen].
  3. Geben Sie im Feld **Name** `A-Bock` ein.
  4. Im Bereich **Bildung der Gruppen** wählen Sie `+Kundennummer+Auftragsnummer`.
  5. Aus der Kombobox **Sortierung in den Gruppen** wählen Sie `Keine`.
  6. Im Bereich **Abstellmodus Gruppen** wählen Sie `vollständige Gruppen gemeinsam` und im Bereich **Optimierungsverhalten** `5.1`.
  7. Aktivieren Sie die Checkbox **Auffang-Abstellplatz**.

**Ergänzende Informationen**
- ⇨ Softwarereferenz, "Orga" auf Seite D-357
- ⇨ Softwarereferenz, "Orga-Gruppen" auf Seite D-359
- ⇨ Softwarereferenz, “Einstellungen-Abstellplatz" auf Seite D-361

---
---

# Softwarereferenz: A+W Production Feinplanung

## Übersicht
Menü **Stammdaten > Feinplanung** öffnen

Im Menü Feinplanung befinden sich folgende Programmpunkte:
- **Voreinstellungen:** Diesen Menüpunkt benötigen Sie, wenn keine Einstellungen für Orga, Gruppierung und Sortierung vorgenommen wurden. (⇨ "Voreinstellungen" auf Seite D-365)
- **Orga:** Über diesen Menüpunkt richten Sie die Orgas ein. Sie definieren die Produktionsreihenfolge sowie die Prüfreihenfolge. (⇨ Register Master-Orga, Produktionsreihenfolge, Prüfreihenfolge)
- **Gruppierung:** Über diesen Menüpunkt richten Sie Gruppierungen und Sortierungen ein. (⇨ “Gruppierung/Sortierung - Dialog" auf Seite D-366)
- **Abstellplätze:** Mit diesem Menüpunkt richten Sie die Abstellplätze ein. (⇨ "Abstellplätze" auf Seite D-372)
- **Bearbeitungen:** Anlegen oder Ändern von Bearbeitungen.
- **Lostypen:** Anlegen von Lostypen und Zuweisung von Bearbeitungen. (⇨ "Lostypen und Bearbeitungen" auf Seite D-376)

> Dialoge können von unterschiedlichen Stellen aus geöffnet werden. Bitte beachten Sie, dass Funktionen und Dialoge auf verschiedenen Wegen geöffnet werden können.

## Organisationen
**Stammdaten > Feinplanung > Orga**

In diesem Bereich erfassen bzw. ändern Sie Master-Orgas, Orgas und Orga-Gruppen sowie Einstellungen an der Produktionsreihenfolge und Prüfreihenfolge.

### Register Master-Orga
Im Register **Master-Orga** legen Sie neue Master-Orgas an oder nehmen Änderungen an bestehenden vor. Die erstellten Master-Orgas weisen Sie dann später bei der Feinplanung einem Lauf zu.
- **Linkes Fenster:** Zeigt alle definierten Master-Orgas in Baumstruktur.
- **Rechtes Fenster:** Zeigt alle definierten Orgas. Die Symbole haben folgende Bedeutung:
  - **S:** Standardorga / Verwendung
  - **S (fett):** Standardorga / Produktion
  - **X:** Nicht-Standardorga / Produktion
  - **X (kursiv):** Nicht-Standardorga / Verwendung
*(Abb. D-49 Erläuterung der Symbole für Orgas)*

**Schaltflächen:**
- **Neu:** Öffnet den Dialog Master-Orga zum Anlegen einer neuen Master-Orga.
- **Löschen:** Löscht die markierte Master-Orga oder Orga.
- **Einstellungen:** Öffnet den Dialog Master-Orga für die ausgewählte Master-Orga.

### Register Produktionsreihenfolge
Zeigt die Reihenfolge der Orga-Gruppen in der Orga.

**Schaltflächen:**
- **Bedingung:** Definiert eine Bedingung für die markierte Orga-Gruppe oder den Abstellplatz.
- **Neu:** Legt eine neue Orga, Orga-Gruppe oder einen neuen Abstellplatz an, je nach Markierung.
- **Ausschneiden / Kopieren / Einfügen:** Bearbeiten der Orga-Struktur.
- **Löschen:** Löscht den markierten Datensatz.
- **Einstellungen:** Öffnet den entsprechenden Dialog für den markierten Eintrag (Orga, Orga-Gruppe, Abstellplatz).
- **Export Orga:** Exportiert die markierte Orga.

### Register Prüfreihenfolge
Zeigt die Prüfreihenfolge aller Abstellplätze einer Orga. Hier wird festgelegt, in welcher Reihenfolge geprüft wird, ob eine Scheibe einem Abstellplatz zugewiesen wird. Ein `*` vor dem Namen kennzeichnet den Auffang-Abstellplatz.

**Schaltflächen:**
- **Anfang / Hoch / Runter / Ende:** Verschieben des markierten Abstellplatzes in der Prüfreihenfolge.

### Dialog: Master-Orga
*(Stammdaten > Feinplanung > Orga > Register Master-Orga > [Neu] oder [Einstellungen])*

Hier legen Sie eine neue Master-Orga an oder ändern eine bestehende.

**Felder:**
- **Name der Master-Orga:** Name für die Master-Orga.
- **XOPT zusammen abstellen:** Steuert, ob Optimierungen trotz verschiedener Glasart/-dicke gemeinsam auf einem A-Bock abgestellt werden.
- **Kombobox (Standard / Schnellorga / Phys. Gestellbelegung):** Steuert den Typ der Master-Orga.
- **Pärchenbildung verboten:** Verhindert die Pärchenbildung, z.B. für 3-fach Isolierglas.
- **Maximale Anzahl Abstellplätze in Optimierung:** Begrenzt die Anzahl der Stapel, die die Optimierung gleichzeitig verwenden darf.
- **Fertigungsgruppen:** Globale Vorbelegung für die Bildung von Fertigungsgruppen.
- **Pseudoserien / Mindestmenge:** Fasst Positionen mit gleichem Aufbau zu Pseudoserien zusammen.
- **Freigabe (verwende Skript):** Verwendet ein Skript bei der Freigabe des Laufs.
- **Auffüller / Quasiteile:** Ermöglicht die Abbildung von Füllern und Quasiteilen über Formeln.
- **Sonderteile (Verwende Füller, Restblätter, Bruchscheiben, Eilscheiben):** Aktiviert die Verwendung von Sonderteilen und definiert deren Abstellplatz-Nummernkreise (Start/Ende).

### Dialog: Orga
*(Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Orga markieren > [Einstellungen])*

**Felder:**
- **Name der Orga-Form:** Name der Orga.
- **Typ:** Orga-Typ (Standard, Packmittel oder ein definierter Lostyp).
- **Produktion:** Checkbox, ob es sich um eine Produktions- oder Verwendungs-Orga handelt.
- **Abstellmodus:** Voreinstellung des Abstellmodus (Glas, Einheit, Produktion, VABGLA).
- **Kein Teilen von ... bei Bockbelegung von mehr als ... Prozent:** Verhindert das Splitten von Gruppen oder Einheiten, wenn der Bock bereits zu einem bestimmten Prozentsatz belegt ist.

### Dialog: Orga-Gruppen
*(Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Orga-Gruppe > [Einstellungen])*

**Felder:**
- **Name:** Name der Orga-Gruppe.
- **DynOpt Einstellung:** Aktivieren, wenn die Orga-Gruppe für A+W DynOpt gedacht ist.
- **Bildung der Gruppen:** Steuert, ob eine Gruppenbildung erfolgen soll, und wählt die entsprechende Gruppierung aus.
- **Sortierung der Gruppen:** Steuert, ob eine Sortierung der gewählten Gruppe erfolgen soll.
- **Sortierung in den Gruppen:** Steuert die Sortierung innerhalb der Gruppen (Keine, Global, Selbst definierte).

### Dialog: Einstellungen-Abstellplatz
*(Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Einstellungen > Register [Verwendung])*

Hier werden Namen, Nummernkreise, Gruppierungen und Abstellmodi für Abstellplätze zugewiesen.

**Felder:**
- **Name:** Name für den Abstellplatz-Typ.
- **Bildung der Gruppen:** Gruppierungsregel für diesen Abstellplatz.
- **Sortierung in den Gruppen:** Sortierregel innerhalb der Gruppen.
- **Invertierung überprüfen:** Steuert, ob die Reihenfolge auf A-Böcken bei bestimmten Bearbeitungsschritten invertiert werden muss.
- **Abstellmodus Gruppen:** Steuert, wie Gruppen abgestellt werden (z.B. `nur 1 Gruppe je Stapel`).
- **Optimierungsverhalten:** Wählt den Optimierungs-Modus (6.1, 6.2, 5.1).
- **Auffang-Abstellplatz:** Markiert diesen Platz als Auffangplatz für nicht zugeordnete Teile.
- **Von / Bis:** Nummernkreis für die Bocknummern dieses Typs.
- **Max. Anzahl Gruppen:** Maximale Anzahl von Gruppen auf diesem Platz.
- **Abstellmodus:** Spezifischer Abstellmodus für den gewählten Abstellplatz-Typ (z.B. Global, Glas, Einheit).
- **Abstellplatz-Typ:** Wählt den Typ aus (A-Bock, Fächerwagen, Feste Abstellplätze).

### Dialog: Voreinstellungen
*(Stammdaten > Feinplanung > Voreinstellung)*

Diese globalen Einstellungen werden verwendet, wenn in den Orgas keine spezifischen Einstellungen vorgenommen wurden.
- **Verarbeitungsreihenfolge:** Globale Sortierregel für die Verarbeitung der Scheiben.
- **Orga:** Globale Master-Orga, die standardmäßig verwendet wird.
- **Gruppenbildung:** Globale Regel zur Gruppenbildung.
- **Sortierung auf Abstellplatz:** Globale Regel zur Sortierung der Scheiben.

### Dialog: Gruppierung/Sortierung
*(Stammdaten > Feinplanung > Gruppierung)*

Dieser Dialog hat drei Register, um Gruppierungen und Sortierungen zu erstellen und zu bearbeiten.
- **Register Editor-Gruppierungen / Editor-Sortierung:** Hier werden neue Gruppierungen/Sortierungen aus den verfügbaren Eigenschaften und Formeln zusammengestellt.
- **Register Zusatz-Sortierungen:** Zeigt erstellte Zusatz-Sortierungen an, die greifen, wenn ein bestimmter Schlüssel (z.B. KUNDENNUMMER) einen bestimmten Wert annimmt.

### Dialog: Abstellplätze
*(Stammdaten > Feinplanung > Abstellplätze)*

Dieser Dialog dient der Definition der physikalischen Abstellplätze, die im Betrieb vorhanden sind. Er ist in drei Bereiche unterteilt:

**Bereich A-Böcke:**
- **Abstelltiefe / Breite:** Dimensionen des A-Bocks.
- **Max. Abstellplätze/Bock:** Anzahl der Stapel pro Bock (1, 2, oder 4).
- **L-Bock / Robot:** Spezielle Bocktypen.
- **Max. Anzahl A-Böcke:** Maximale Anzahl für die Bildung von Opti-Gruppen.
- **Maximales Gewicht (kg):** Gewichtsbegrenzung.

**Bereich Fächerwagen:**
- **Anzahl Fachnummer:** Anzahl der Fächer.
- **Breite:** Breite der Fächer.
- **Zwei Fächer/Nummer:** Zwei Fächer teilen sich eine Nummer.
- **Anzahl der Stellen für Fachnummer:** Reservierte Stellen in der Abstellplatznummer.
- **Max. Anzahl Fächerwagen:** Maximale Anzahl für Opti-Gruppen.
- **Maximale Nutzlast (kg) / Leergewicht (kg):** Gewichtsangaben.

**Bereich Feste Abstellplätze:**
- **Abstelltiefe / Breite:** Dimensionen.
- **Max. Anzahl FAPs:** Maximale Anzahl für Opti-Gruppen.
- **Maximales Gewicht (kg):** Gewichtsbegrenzung.

