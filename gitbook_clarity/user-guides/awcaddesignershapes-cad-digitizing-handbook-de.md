---
description: "DE-HB-AWCADDesignerShapes_10"
---


- **Digitizing Contours**: Detailed procedures for digitizing both outer and inner contours, including complex shapes and drill holes, using a digitizing table. It explains how to handle post-processing tasks like smoothing critical points and aligning contours.
- **Virtual Digitizing**: Instructions on how to digitize a contour from a digital photograph (*.jpg) using the Virtual Digitizing (VD) add-on software.
- **Sketching and Dimensioning**: A walkthrough of creating a complex shape as a dimensioned sketch. This covers drawing lines, applying various types of dimensions, adding radii, and ensuring the sketch is fully constrained.
- **Advanced Examples**: Practical, multi-page examples are provided, such as creating a door with various cutouts and drill holes, and constructing a complex keyhole shape by creating, connecting, and mirroring sub-contours.
- **Working with Models and Variables**: Guidance on creating parametric models using variables. This includes defining formulas and using conditional logic (via `sign()` function) to create dynamic drawings that can, for example, exaggerate small features for better visibility on printouts.
- **Processing and Production**: Information on preparing shapes for production, including specifying break-off edges, defining edge processing qualities (polishing, grinding), and handling corners.
- **Working with Laminated/Insulated Glass (VSG/ISO)**: Instructions on how to work with multi-pane units, either by aligning individual panes or by using a bill of materials (BOM) structure.
- **Printing and Collaboration**: How to print drawings, including exporting to Microsoft Word using templates and placeholders. It also provides a detailed overview of the software's integration with other systems like A+W Enterprise and A+W Business, explaining the data exchange workflows, key structures for articles, and the technical setup for collaboration."
---

# Werkzeuge
## Konkrete Fragestellungen

### 5. Erfassen Sie den ersten Punkt erneut.
Wenn A+W CAD Designer (Shapes) nicht automatisch erkennt, dass die Kontur jetzt vollständig erfasst ist, dann betätigen Sie `<Esc>`.

### 6. Erfassen Sie, falls erforderlich, die zugehörige Innenkontur.

### 7. Wenn Sie die Kontur vollständig erfasst haben, dann wechseln Sie in die Ansicht Geometrie.
A+W CAD Designer (Shapes) führt eine Interpolation der Punkte zu Geraden und Radien durch. Wenn Sie mit dem Ergebnis nicht zufrieden sind, haben Sie folgende Möglichkeiten:
- Wiederholen Sie das Digitalisieren der Kontur und erfassen Sie an den Stellen, an denen A+W CAD Designer (Shapes) die Kontur nicht richtig erkannt hat, deutlich mehr Punkte.
- Erfassen Sie die benötigten Ausgleichsbögen und Ausgleichsgeraden manuell:

Je nach Digitalisierung sind jetzt noch runde Ecken vorhanden, die Sie zu-spitzen oder kritische Stellen, die Sie beseitigen können.

### Weiterführende Arbeiten
- "Zwischen zwei Segmenten abrunden oder zuspitzen" auf Seite A-321
- "Kritische Stellen erkennen und glätten" auf Seite A-457
- "Kontur ausrichten" auf Seite A-460

### Ergänzende Informationen
- "Ausgleichsbögen und Ausgleichsgeraden manuell setzen" auf Seite A-456
- "Innenkontur digitalisieren" auf Seite A-451
- "Mit Modellen arbeiten" auf Seite A-480

### Innenkontur digitalisieren
Hier finden Sie Informationen zum Digitalisieren komplexer Innenkonturen. Das Digitalisieren von Bohrlöchern finden Sie unter:

Erfassen Sie immer zuerst die Außenkontur und wählen Sie das Digitalisierwerkzeug ab, bevor sie mit der Digitalisierung einer Innenkontur beginnen. Wenn nach dem Erfassen einer Außenkontur Punkte innerhalb dieser Kontur gesendet werden, dann erkennt A+W CAD Designer (Shapes) automatisch, dass es sich um eine Innenkontur handelt.

1.  Wechseln Sie in die Ansicht Punkte.
2.  Stellen Sie sicher, dass das Werkzeug zum Erfassen der Außenkontur abgewählt wurde. Wenn Sie `<Esc>` betätigen, wird das Werkzeug abgewählt.
3.  Innenkonturen werden mit den selben Werkzeugen digitalisiert wie Außenkonturen.

[Image: Three icons representing different digitizing tools.]

*A+W CAD Designer (Shapes) Überblick*
*A-451*
---
## Konkrete Fragestellungen
### Werkzeuge

Markieren Sie das gewünschte Werkzeug zum Digitalisieren der Innenkontur.

Nach dem Digitalisieren einer Innenkontur mit dem Digitalisierrad erkennt A+W CAD Designer (Shapes) automatisch, dass der Raddurchmesser nach Außen verschoben werden muss.

### Ergänzende Informationen
- "Bohrlöcher digitalisieren" auf Seite A-452
- "Außenkontur mit dem Rad digitalisieren" auf Seite A-449
- "Außenkontur mit Stift oder Lupe digitalisieren" auf Seite A-450

### Bohrlöcher digitalisieren
Bohrlöcher werden immer nach der Außengeometrie digitalisiert. Bohrlöcher können auf Grund ihrer Größe normalerweise nicht mit dem Rad digitalisiert werden.

1.  Wechseln Sie in die Ansicht Punkte.
2.  Stellen Sie sicher, dass das Werkzeug zum Erfassen der Außenkontur abgewählt wurde. Wenn Sie `<Esc>` betätigen, wird das Werkzeug abgewählt.
3.  Markieren Sie das Werkzeug zum Digitalisieren der Bohrung.
    [Image: Two icons for digitizing drill holes.]
4.  Digitalisieren Sie Punkte auf dem Kreismantel der Bohrung. Dazu bietet Ihnen A+W CAD Designer (Shapes) zwei Methoden:
    -   **Kreismantel als Fadenkreuz digitalisieren**
        Digitalisieren Sie vier Punkte des Kreismantels als Fadenkreuz. Digitalisieren Sie dabei immer die beiden gegenüberliegenden Punkte nacheinander (z. B. oben – unten, links – rechts).
    -   **Kreismantel als Viertelkreis digitalisieren**
        Digitalisieren Sie mehrere Punkte auf dem Kreismantel in einer Richtung nacheinander. Damit A+W CAD Designer (Shapes) eine richtige Bestimmung des Bohrdurchmessers durchführt, müssen Sie mindestens ein Viertel des Bohrungskreises digitalisieren.
5.  Betätigen Sie `<Esc>`, wenn Sie die erforderliche Menge von Punkten digitalisiert haben.
6.  Wählen Sie das Werkzeug zum Erkennen der Bohrung. Je nach dem, wie Sie den Kreismantel digitalisiert haben, stellt A+W CAD Designer (Shapes) zwei verschiedene Werkzeuge zur Verfügung:

Der Kreismantel wurde als Fadenkreuz digitalisiert:

[Image: Icon for recognizing a crosshair-digitized circle.]

*A-452*
*A+W CAD Designer (Shapes) Überblick*
---
## Werkzeuge
### Konkrete Fragestellungen

Wählen Sie das angezeigte Werkzeug.
Markieren Sie den ersten digitalisierten Punkt, danach den letzten digitalisierten Punkt.

*A+W CAD Designer (Shapes) Überblick*
*A-453*
---
## Konkrete Fragestellungen
### Werkzeuge

Der Kreismantel wurde als Viertelkreis digitalisiert:
[Image: Icon for recognizing a quarter-circle digitized circle.]

Wählen Sie das angezeigte Werkzeug.
Markieren Sie den ersten digitalisierten Punkt, danach den letzten digitalisierten Punkt.

7.  Betätigen Sie [OK]. A+W CAD Designer (Shapes) berechnet den Durchmesser des Bohrlochs und zeigt diesen an. Den angegebenen Durchmesser können Sie in der Ansicht Geometrie bei Bedarf korrigieren.

> **Wenn nur Bohrmittelpunkt und Maße der Bohrung vorhanden sind!**
> Wenn Sie die Bohrung nicht digitalisieren können, weil nur der Mittelpunkt und der Durchmesser bekannt ist, dann können Sie statt das Bohrloch zu digitalisieren ein Bohrloch in der Ansicht Innenkonturen erfassen.

### Ergänzende Informationen
- "Bohrloch von einem digitalisierten Fadenkreuz erfassen" auf Seite A-230
- "Optimales Bohrloch durch Auswahl von digitalisierten Punkten erfassen" auf Seite A-229

*A-454*
*A+W CAD Designer (Shapes) Überblick*
---
# Werkzeuge
## Konkrete Fragestellungen

### Virtuell digitalisieren
Wenn die Zusatz-Software Virtual Digitizing (VD) an Ihrem Arbeitsplatz installiert und A+W CAD Designer (Shapes) entsprechend konfiguriert wurde, dann können Sie Modelle ohne Digitalisiertisch digitalisieren. Gehen Sie dabei wie nachfolgend beschrieben vor.
Details zum Arbeiten mit der Software VD entnehmen Sie bitte dem Handbuch des Herstellers.

Die nachfolgende Beschreibung setzt voraus, dass Sie ein Modell und ein Referenzmaß erstellt haben und die benötigte Kontur mit einer kalibrierten Kamera aufgenommen haben. Das Bild liegt als *.jpg-Datei in einem Verzeichnis.

### Foto einer Kontur digitalisieren
1.  Starten Sie A+W CAD Designer (Shapes).
2.  Wählen Sie im Menü Datei den Eintrag Öffnen. A+W CAD Designer (Shapes) öffnet den Dialog Öffnen.
3.  Wechseln Sie in das Verzeichnis, in dem das Bild liegt.
4.  Wählen Sie als Dateityp File (*.JPG). A+W CAD Designer (Shapes) zeigt Ihnen alle Dateien dieses Typs im gewählten Verzeichnis an.
5.  Klicken Sie auf die gewünschte Datei und bestätigen Sie mit [Öffnen]. A+W CAD Designer (Shapes) startet das Programm Virtual Digitizing (VD) und öffnet dort das ausgewählte Bild.
6.  Korrigieren Sie das Bild mit der Kalibrationsdatei der Kamera, mit der das Bild aufgenommen wurde.
    > **Handbuch der Software Virtual Digitizing beachten!**
    > Details zu den hier beschriebenen Arbeitsschritten finden Sie im Handbuch Virtual Digitizing.
7.  Setzen Sie die Referenzpunkte.
8.  Umranden Sie die Kontur (z. B. mit dem magnetischen Lasso).
9.  Lassen Sie VD Punkte der Kontur finden.
10. Korrigieren oder ergänzen Sie Punkte auf der Kontur.
11. Senden Sie die Konturpunkte nach A+W CAD Designer (Shapes). Wählen Sie dazu die entsprechende Funktion in VD.
    A+W CAD Designer (Shapes) erstellt eine leere Datei und importiert die Punkte der Kontur aus VD in die Ansicht Punkte.

### Ergänzende Informationen
- Softwarereferenz, "Öffnen" auf Seite A-163

*A+W CAD Designer (Shapes) Überblick*
*A-455*
---
# Konkrete Fragestellungen
## Werkzeuge

### Nachbearbeiten in CAD Designer
Nach dem Digitalisieren oder Importieren von Konturen sind diese noch nicht zur Weiterverarbeitung mit diversen Maschinen optimiert. Nachfolgend finden Sie folgende Korrekturarbeiten beschrieben:
- Ausgleichsbögen und Ausgleichsgeraden manuell setzen
- Kritische Stellen erkennen und glätten
- Kontur ausrichten

### Ausgleichsbögen und Ausgleichsgeraden manuell setzen
Die folgende Beschreibung setzt voraus, dass Sie in der Ansicht Punkte eine Kontur digitalisiert haben und das Digitalisierwerkzeug jetzt abgewählt ist.

> **Startpunkt beim Digitalisieren**
> Wenn Sie Ausgleichsbögen und Ausgleichsgeraden manuell setzen, dann müssen Sie damit an dem Punkt beginnen, der zuerst digitalisiert wurde (Startpunkt). Merken Sie sich daher den entsprechenden Punkt in der Ansicht Punkte. Wenn Sie an einem anderen Punkt mit den Ausgleichsbögen oder -geraden beginnen, kann es zu Fehlern im Programm kommen.

Gehen Sie wie folgt vor, um in die digitalisierten Punkte einer Kontur die gewünschten Ausgleichsbögen und -geraden zu legen.

1.  Identifizieren Sie den Startpunkt, mit dem das Digitalisieren begonnen wurde.
2.  Wählen Sie das geeignete Werkzeug aus (Ausgleichsbogen oder Ausgleichsgerade).
    [Image: Two icons, one for setting an arc and one for setting a straight line.]
3.  Klicken Sie damit auf den Startpunkt. A+W CAD Designer (Shapes) färbt den Punkt rot.
4.  Suchen Sie in der Richtung, in der Sie die Kontur digitalisiert haben, nach dem Punkt, bis zu dem der Ausgleichsbogen oder die Ausgleichsgerade gelegt werden soll, und klicken Sie auf diesen Punkt. A+W CAD Designer (Shapes) färbt den Punkt grün, alle Punkte davor färbt A+W CAD Designer (Shapes) rot.
5.  Betätigen Sie [OK].
6.  Lassen Sie zwischen zwei Bögen einen Punkt (zwei Zwischenräume) frei. Lassen Sie zwischen einer Geraden und einem Bogen einen Zwischenraum frei. A+W CAD Designer (Shapes) benötigt diesen Zwischenraum, um einen Ausgleich zwischen den Segmenten zu berechnen.
7.  Wählen Sie das geeignete Werkzeug aus (Ausgleichsbogen oder Ausgleichsgerade) und klicken Sie damit auf den nächsten verwendbaren Punkt (nach einem freigelassenen Punkt oder nach einem Zwischenraum).

*A-456*
*A+W CAD Designer (Shapes) Überblick*
---
# Werkzeuge
## Konkrete Fragestellungen

> **Werkzeug wechseln!**
> Wenn Sie nach einem Bogen eine Gerade legen wollen (oder umgekehrt), dann müssen Sie das Werkzeug wechseln. A+W CAD Designer (Shapes) verwendet zur Berechnung intern jeweils andere Algorithmen.

> **In Reihenfolge arbeiten!**
> Arbeiten Sie in fortlaufender Reihenfolge, auch wenn Sie dazu mehrfach die Werkzeuge wechseln müssen. A+W CAD Designer (Shapes) berechnet falsche Ergebnisse, wenn Sie zuerst alle Geraden und dann dazwischen alle Bögen legen.

8.  Wiederholen Sie die Schritte 3 bis 6 so lange, bis Sie den letzten Punkt erreicht haben. Diesen müssen Sie frei lassen, wenn er zwischen zwei Bögen liegt.
9.  Wechseln Sie in die Ansicht Geometrie. A+W CAD Designer (Shapes) berechnet die Segmente und zeigt die berechnete Kontur an.

Je nach dem, wie Sie die Ausgleichsbögen und -geraden gelegt haben, sind jetzt noch runde Ecken vorhanden, die Sie zuspitzen oder kritische Stellen, die Sie beseitigen können.

### Weiterführende Arbeiten
- "Optimale Gerade durch Auswahl von digitalisierten Punkten erfassen" auf Seite A-231
- "Optimalen Bogen durch Auswahl von digitalisierten Punkten erfassen" auf Seite A-232
- "Zwischen zwei Segmenten abrunden oder zuspitzen" auf Seite A-321
- "Kritische Stellen erkennen und glätten" auf Seite A-457
- "Kontur ausrichten" auf Seite A-460

### Kritische Stellen erkennen und glätten
Kritische Stellen sind Segmente oder Punkte in einer Kontur, die so nicht hergestellt oder bearbeitet werden können. Kritische Stellen sind Punkte an denen kein tangentialer Übergang (0°) zwischen einer Geraden und einem Bogen oder zwischen 2 Bögen vorhanden ist. Diese kritischen Stellen führen zu unsauberen Kanten, wenn diese von einer Bearbeitungsmaschine bearbeitet werden sollen oder verzögern den Zuschnitt. Was als kritische Stelle gilt, kann in der sn.ini festgelegt werden.

Mit den Werkzeugen zum glätten der Kontur können Sie den kritischen Punkt so lange zu verschieben, bis ein tangentialer Winkel von 0° bzw. annähernd 0° erreicht wird. Dabei kommt es zu einer minimalen Vergrößerung bzw. Verkleinerung der Kontur an dieser Stelle.

1.  Wechseln Sie in die Ansicht Geometrie.
2.  Aktivieren Sie im Menü Ansicht > Einstellungen > Kritische Stellen anzeigen den Punkt Markiere kritische Stellen in Geometrie und Revision.
    A+W CAD Designer (Shapes) zeigt jetzt auf der Kontur die kritischen Stellen mit blauen Pfeilen an.

*A+W CAD Designer (Shapes) Überblick*
*A-457*
---
## Konkrete Fragestellungen
### Werkzeuge

3. Klicken Sie mit dem Zeiger auf ein Segment an einer kritischen Stelle. A+W CAD Designer (Shapes) markiert das Segment rot und numeriert die Enden mit 1 und 2. Im Wertefenster zeigt A+W CAD Designer (Shapes) verschiedene Informationen zu dem Segment und den Winkeln in den Punkten 1 und 2 an.
4. Klicken Sie auf das Werkzeug, mit dem Sie den Punkt an der kritischen Stelle verschieben wollen.

   [Image: Three tool icons for moving points to smooth contours.]
   
   Der Pfeil zeigt das Werkzeugsymbol an.
5. Klicken Sie mit dem Werkzeug auf den kritischen Punkt, den Sie beseitigen wollen. A+W CAD Designer (Shapes) zeigt im Wertefenster die Schrittweite D an.
   Wenn Sie das Werkzeug *Punkt in beliebiger Richtung verschieben* gewählt haben, dann können Sie den markierten Punkt mit der Maus und gedrückter linker Maustaste verschieben. A+W CAD Designer (Shapes) zeigt dabei im Wertefenster fortlaufend die erreichten Ergebnisse an. Die nächsten Schritte entfallen bei diesem Werkzeug.
6. Ändern Sie, falls gewünscht, die Schrittweite. Die Schrittweite ist der Abstand, mit dem A+W CAD Designer (Shapes) den markierten Punkt immer wieder verschiebt, bis der kleinste mögliche tangentiale Winkel erreicht ist. Nach jeder Schrittweite berechnet A+W CAD Designer (Shapes) das erreichte Ergebnis.

> **Aufwand gering halten**
> Um ein optimales Ergebnis zu erreichen, versucht A+W CAD Designer (Shapes) auch die zu dem gewählten Punkt benachbarten Punkte mit zu glätten. Wenn Sie mehrere Kritische Punkte glätten müssen, ist es daher ratsam, mit dem Punkt in der Mitte zu beginnen. Damit können Sie Arbeit einsparen.

7. Betätigen Sie [OK]. A+W CAD Designer (Shapes) ermittelt die Position des Punktes in der angegebenen Richtung, bei der der Übergangswinkel zwischen den benachbarten Segmenten minimal ist. Den neuen Verlauf der Segmente zeigt A+W CAD Designer (Shapes) blau an. Im Wertefenster zeigt A+W CAD Designer (Shapes) das Ergebnis der Verschiebung an.
8. Prüfen Sie die angezeigten Ergebnisse im Wertefenster:

| Anzeige | Bedeutung |
| :--- | :--- |
| e | |
| d | Direkter Abstand zwischen dem alten und dem neuen Punkt. |
| d= | Abstand des neuen Punktes vom alten Punkt in tangentialer Richtung des Segmentes (Konturlinie) am alten Punkt. |

**Tab. A-45: Wertefenster zur Punktverschiebung**

*A-458*
*A+W CAD Designer (Shapes) Überblick*
---
## Werkzeuge
### Konkrete Fragestellungen

| Anzeige | Bedeutung |
| :--- | :--- |
| e | |
| d+ | Abstand des neuen Punktes vom alten Punkt senkrecht zur Tangente des Segmentes (Konturlinie) am alten Punkt. |
| D | Angabe, um wie viele mm der Punkt verschoben wird. Positiver Wert: Verschiebung nach außen. Negativer Wert: Verschiebung nach innen. |
| 1)( | Segment 1 ist mit dem angegebenen Radius nach innen gekrümmt. |
| 2() | Segment 2 ist mit dem angegebenen Radius nach außen gekrümmt. |
| <1 | Erreichter Übergangswinkel am Punkt 1 (vor dem kritischen Punkt). |
| <C | Erreichter Übergangswinkel am kritischen Punkt. |
| <2 | Erreichter Übergangswinkel am Punkt 2 (nach dem kritischen Punkt). |
| --1-- | Wählen Sie diese Checkbox, wenn der Übergang am Punkt 1 tangential verlaufen soll. |
| --C-- | Wählen Sie diese Checkbox, wenn der Übergang am kritischen Punkt tangential verlaufen soll. |
| --2-- | Wählen Sie diese Checkbox, wenn der Übergang am Punkt 2 tangential verlaufen soll. |
| \|>( | Wählen Sie diese Checkbox, wenn A+W CAD Designer (Shapes) beim Glätten Geraden in einen Kreisbogen wandeln darf. |

**Tab. A-45: Wertefenster zur Punktverschiebung**

9. Wenn Sie mit dem neuen Verlauf der Segmente einverstanden sind, bestätigen Sie mit [OK]. Die kritische Stelle ist beseitigt. Setzen Sie die Arbeit bei Schritt 17 fort.
   Wenn Sie mit dem neuen Verlauf der Segmente nicht zufrieden sind, fahren Sie mit den folgenden Punkten fort.
10. Betätigen Sie `<Esc>`. A+W CAD Designer (Shapes) deaktiviert das gewählte Werkzeug und verwirft das erzielte Ergebnis.
11. Wählen Sie das jeweils andere Werkzeug (Punkt entlang der Kontur verschieben oder Punkt senkrecht zur Kontur verschieben) und wiederholen Sie Schritt 5 bis Schritt 8.
12. Wenn Sie mit dem neuen Verlauf der Segmente einverstanden sind, bestätigen Sie mit [OK]. Die kritische Stelle ist beseitigt.
   Wenn Sie mit dem neuen Verlauf der Segmente nicht zufrieden sind, dann kann es daran liegen, dass die an den kritischen Punkt angrenzenden Segmente zu groß sind. Fahren Sie mit den folgenden Arbeitsschritten fort oder versuchen Sie, den Verlauf angrenzender Segmente zu korrigieren.
13. Betätigen Sie `<Esc>`. A+W CAD Designer (Shapes) deaktiviert das gewählte Werkzeug und verwirft das erzielte Ergebnis.
14. Klicken Sie auf das Werkzeug Segment in zwei Segmente teilen.

*A+W CAD Designer (Shapes) Überblick*
*A-459*
---
## Konkrete Fragestellungen
### Werkzeuge

[Icon for splitting a segment]

15. Setzen Sie den neuen Punkt an eine geeignete Stelle. Teilen Sie, falls erforderlich, auch das zweite angrenzende Segment.
16. Wiederholen Sie die Schritte 4 bis 11.
17. Betätigen Sie [OK], um das Ergebnis zu akzeptieren. A+W CAD Designer (Shapes) zeigt die neue Kontur an.
18. Wenn Sie den ursprünglichen Verlauf der Kontur nochmals sehen wollen, betätigen Sie im Menü Bearbeiten den Eintrag Aktion auswählen.

### Ergänzende Informationen
- "Segment in zwei Segmente teilen" auf Seite A-246
- "Punkt entlang der Kontur verschieben" auf Seite A-240
- "Punkt in beliebiger Richtung verschieben" auf Seite A-243
- "Punkt senkrecht zur Kontur verschieben" auf Seite A-244

### Kontur ausrichten
Damit eine Kontur optimal durch die Produktion laufen kann, wird eine Standkante benötigt.
1. Wenn die digitalisierte Kontur keine geeignete Standkante besitzt, dann ermitteln Sie das kleinste umschreibende Rechteck als geeignete Kontur für die Produktion.
   [Icon for calculating bounding box]
2. Wenn die Kontur eine geeignete Kante besitzt, diese aber nicht waagerecht ausgerichtet ist, dann drehen Sie die Kontur in die richtige Position.
   [Icon for rotating the contour]

### Ergänzende Informationen
- "Minimale Breite und Höhe des umschreibenden Rechtecks berechnen" auf Seite A-376
- "Scheibe zur X-Richtung ausrichten" auf Seite A-375

*A-460*
*A+W CAD Designer (Shapes) Überblick*
---
# Werkzeuge
## Konkrete Fragestellungen

### Scheibe als Skizze erfassen
Nachfolgend finden Sie die Beschreibung aller Arbeitsschritte, die zum Erfassen einer Kontur als Skizze mit Vermaßung erforderlich sind. Um die Arbeitsschritte anschaulicher zu machen, werden die Arbeitsschritte anhand eines Beispiels erklärt. Die folgende Kontur soll erfasst und vermaßt werden:

**Zeichnung Endprodukt**
[Image of a dimensioned shape to be created.]
*Abb. A-212 Beispiel zur Konturerfassung mit Skizze*

Nachfolgend finden Sie folgende Arbeitsschritte beschrieben, mit denen Sie eine Kontur als Skizze erfassen können:
- Skizze erstellen
- Skizze vermaßen
- Kontur drehen und Radien einfügen
- Zeichnung vermaßen

### Skizze erstellen
1.  Öffnen Sie eine neue Datei und wechseln Sie in die Ansicht Skizze. A+W CAD Designer (Shapes) setzt den Startpunkt in einer neuen Datei unten links.
2.  Entscheiden Sie, auf welche Kante der Skizze sich die meisten Maße beziehen. Prüfen Sie dazu ggf. die vorliegende Handskizze.
3.  Setzen Sie den Startpunkt an eine geeignete Stelle (evtl. an den Anfang der Bezugskante). Verwenden Sie dazu das angezeigte Werkzeug.
    [Icon for setting the starting point]

*A+W CAD Designer (Shapes) Überblick*
*A-461*
---
## Konkrete Fragestellungen
### Werkzeuge

4. Ziehen Sie die benötigten Linie. Wählen Sie dazu das angezeigte Werkzeug und klicken Sie in ungefähr an die Stelle, an der die Kante enden soll.
   [Icon for drawing a line]

5. Ziehen Sie auch für die Radien zunächst Linien. Dies erleichtert die Vermaßung. Die Radien können Sie am Ende in der Ansicht Geometrie als Eckrundungen ergänzen.

6. Wiederholen Sie den vorherigen Schritt für alle Kanten, die eine benötigte Kontur hat. Arbeiten Sie dabei zusammenhängend in eine Richtung, auch wenn Sie das Werkzeug wechseln und an einer Geraden einen Radius anschließen. Klicken Sie bei der letzten Linie auf den Startpunkt, um die Kontur zu schließen. Die Beispielform sieht nach diesen Schritten wie folgt aus:

   [Image of the shape with straight lines only]
   *Abb. A-213 Beispiel nach dem Ziehen der Linien*

> **Skizze braucht nur ungefähr zu stimmen!**
> Beim Erstellen der Skizze ist es ausreichend, wenn die Skizze ungefähr so aussieht, wie die Scheibe später aussehen soll. Wichtig ist, dass Sie alle Kanten erfasst haben und die Kontur geschlossen ist.

7. Wählen Sie das Werkzeug ab und vermaßen Sie die Skizze.

### Ergänzende Informationen
- "Neuen Startpunkt erfassen" auf Seite A-236
- "Neue Gerade durch Werteeingabe erfassen" auf Seite A-238
- "Neuen Bogen durch Gummiband erfassen" auf Seite A-238

*A-462*
*A+W CAD Designer (Shapes) Überblick*
---
# Werkzeuge
## Konkrete Fragestellungen

### Skizze vermaßen
Zum Vermaßen einer Skizze stehen viele unterschiedliche Werkzeuge zur Verfügung. Nachfolgend sind diejenigen genannt, die zum Vermaßen der Beispielform benötigt werden. Einen Überblick über die Vermaßungswerkzeuge finden Sie unter:
- "Werkzeuge zur Vermaßung" auf Seite A-257
- "Segmente vermaßen" auf Seite A-260
- "Winkel vermaßen" auf Seite A-276
- "Kreise und Bögen vermaßen" auf Seite A-283
- "Automatisch vermaßen" auf Seite A-296

Um eine Skizze vollständig zu vermaßen brauchen Sie folgende Anzahl von Vermaßungen:
`3 * Anzahl der Kreisbögen + 2 * Anzahl der Geraden - 3 = Anzahl der benötigten Konturvermaßungen`

1.  Beginnen Sie mit der Vermaßung der Bezugskante. Wählen Sie dazu das angezeigte Werkzeug, klicken Sie auf das entsprechende Segment und geben Sie das Maß (444,20) ein.
    [Icon for dimensioning a segment length]

> **Maßangaben später formatieren**
> Wenn Sie in der Zeichnung eine bestimmte Vermaßung sehen wollen, und bestimmte Maße nicht benötigen, dann können Sie diese Darstellung nach der Vermaßung der Skizze erfassen.

2.  Vermaßen Sie den nächsten Punkt nach der Bezugskante. Im Beispiel wurde der Punkt gegen den Uhrzeigersinn gewählt. Geben Sie zunächst den senkrechten Abstand zur Bezugskante an. Wählen Sie dazu das angezeigte Werkzeug und geben Sie den erforderlichen Wert ein (71,7).
    [Icon for vertical dimensioning from a point to a line]

3.  Geben Sie jetzt den waagerechten Abstand zur Bezugskante an. Wählen Sie dazu das angezeigte Werkzeug und geben Sie den erforderlichen Wert ein (48,4).
    [Icon for horizontal dimensioning from a point to a line]

Die Kontur im Beispiel sollte jetzt so aussehen (vergrößert):

*A+W CAD Designer (Shapes) Überblick*
*A-463*
---
## Konkrete Fragestellungen
### Werkzeuge

[Image of a partially dimensioned sketch.]
*Abb. A-214 Beispiel nach den ersten Maßangaben*

4. Vermaßen Sie den nächsten Punkt in der begonnenen Richtung.
   [Image: Two tool icons for dimensioning a point relative to a segment.]
   Verwenden Sie dazu die beiden bereits eingesetzten Werkzeuge oder alternativ die beiden angezeigten. Der Unterschied der Werkzeuge liegt darin, dass der Bezugspunkt einmal auf dem Bezugssegment liegen muss und das andere Mal nicht auf dem Bezugssegment liegen darf.

> **Maße können jederzeit kontrolliert werden!**
> Wenn Sie feststellen wollen, wie ein Punkt vermaßt wurde, dann wählen Sie den Zeiger und klicken Sie auf das Maß, das Sie interessiert. A+W CAD Designer (Shapes) markiert die Punkte und das Segment farbig, die zur Vermaßung herangezogen wurden.

5. Vermaßen Sie den nächsten und alle weiteren Punkte in der begonnenen Richtung mit den beschriebenen Werkzeugen.
   Nach vollständiger Vermaßung sollte die Kontur im Beispiel wie folgt aussehen:

*A-464*
*A+W CAD Designer (Shapes) Überblick*
---
# Werkzeuge
## Konkrete Fragestellungen

[Image of the fully dimensioned sketch.]
*Abb. A-215 Beispiel nach der Vermaßung*

6. Betätigen Sie `<Strg> + <D>` um zu Prüfen, ob Sie bereits ausreichend vermaßt haben. A+W CAD Designer (Shapes) markiert die Segmente rot, die geometrisch berechnet werden können und zeigt in der Mitte eine kleine rote Zahl an. Diese Zahl gibt an, wie viele Maße noch fehlen. Hat die Zahl ein negatives Vorzeichen, so ist die Kontur überbestimmt und enthält möglicherweise widersprüchliche Maßangaben.
7. Wenn A+W CAD Designer (Shapes) die Kontur vollständig geometrisch berechnen kann, dann können Sie die fehlenden Radien einfügen.

*A+W CAD Designer (Shapes) Überblick*
*A-465*
---
## Konkrete Fragestellungen
### Werkzeuge

### Kontur drehen und Radien einfügen
1.  Wechseln Sie in die Ansicht Geometrie. In dieser Ansicht sieht die Beispielform jetzt so aus:

    [Image of the dimensioned geometry in the geometry view.]
    *Abb. A-216 Beispiel in der Ansicht Geometrie*

    A+W CAD Designer (Shapes) dreht die Kontur automatisch auf die lange untere Seite, um diese als Standkante zu verwenden.
2.  Richten Sie die Kante, die Ihre Bezugskante ist, waagerecht aus. Verwenden Sie dazu das angezeigte Werkzeug.
    [Icon for aligning an edge horizontally.]
3.  Fügen Sie die fehlenden Radien ein verwenden Sie dazu eines der angezeigten Werkzeuge.
    [Image: Two icons for adding radii to corners.]

Damit ist die gewünschte Kontur erfasst und Sie können, falls erforderlich, noch Bohrungen setzen oder Kantenbearbeitungen anbringen.

*A-466*
*A+W CAD Designer (Shapes) Überblick*
---
# Werkzeuge
## Konkrete Fragestellungen

### Zeichnung vermaßen
1.  Wechseln Sie in die Ansicht Innenkonturen oder Endprodukt.
    Innerhalb dieser Ansichten (und auch in anderen Ansichten) können Sie die Darstellung am Bildschirm über zwei Register am unteren Zeichnungsrand zwischen S&N und Zeichnung umschalten. In der Darstellung Zeichnung zeigt
    [Icon for toggling between S&N and Drawing view.]
    die Kontur und Vermaßung so an, wie sie auf dem Ausdruck aussehen wird.
2.  Wählen Sie, in welcher Darstellung (S&N oder Zeichnung) Sie Maßergänzungen oder Änderungen durchführen wollen.

> **Änderungen werden nur von S&N nach Zeichnung übernommen!**
> Änderungen, die Sie in der Darstellung S&N vornehmen, werden automatisch in die Darstellung Zeichnung übernommen. Umgekehrt werden Änderungen in der Darstellung Zeichnung nicht in die Darstellung S&N übernommen. Die Darstellung Zeichnung ist eine Vorschau auf den Ausdruck.

3.  Wählen Sie ein geeignetes Vermaßungswerkzeug und wenden Sie es an:
4.  Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).

> **Erst vermaßen, dann Ecken runden!**
> Wenn Sie auf Ecken vermaßen wollen, die eine Rundung erhalten haben, dann fehlt der Eckpunkt als Bezugspunkt. In solchen Fällen können Sie zuerst auf die Ecke vermaßen und anschließend die Ecke runden. A+W CAD Designer (Shapes) behält dann die Lage der ursprünglichen Ecke bei.

5.  Wechseln Sie in die Darstellung Zeichnung und entfernen Sie nicht gewünschte Vermaßungen. Die Skizze sollte am Ende wie folgt aussehen:

*A+W CAD Designer (Shapes) Überblick*
*A-467*
---
## Konkrete Fragestellungen
### Werkzeuge

**Zeichnung Endprodukt**
[Image of the final product drawing with rounded corners and dimensions.]
*Abb. A-217 Beispiel nach Eckrundung*

> **Die Zeichnungsansicht Endprodukt wird in A+W Business TAB verwendet!**
> Wenn Sie mit einer A+W Business TAB zusammenarbeiten, dann wird die Darstellung Zeichnung im Register Endprodukt als Vorschau für die Templates verwendet.
>
> "Zusammenarbeit mit A+W Business" auf Seite A-508

*A-468*
*A+W CAD Designer (Shapes) Überblick*
---
# Werkzeuge
## Konkrete Fragestellungen

### Tür mit Ausschnitten und Bohrungen versehen
Nachfolgend finden Sie die Beschreibung aller Arbeitsschritte, die Sie zum Erstellen einer Tür mit Randausschnitten benötigen. Um die Arbeitsschritte anschaulicher zu machen, werden die Arbeitsschritte anhand des folgenden Beispiels erklärt.

[Image of a dimensioned drawing of a door with cutouts and drill holes.]
*Abb. A-218 Beispiel: Tür mit Ausschnitten*

Folgende Arbeitsschritte müssen Sie durchführen, um eine Tür mit Ausschnitten zu erfassen:
- Ausschnitte erstellen
- Tür erstellen und Ausschnitte positionieren
- Zeichnung gestalten

*A-W CAD Designer (Shapes) Überblick*
*A-469*
---
## Konkrete Fragestellungen
### Werkzeuge

### Ausschnitte erstellen
Erstellen Sie die Ausschnitte, die sie häufig benötigen, in einer separaten Datei. So können Sie den selben Ausschnitt immer wieder bei verschiedenen anderen Konturen einsetzen.
1. Öffnen Sie eine neue Datei und wechseln Sie in die Ansicht Skizze.
2. Setzen Sie den Startpunkt an eine geeignete Stelle und zeichnen Sie den Ausschnitt.

> **Nur halben Ausschnitt zeichnen!**
> Wenn der benötigte Ausschnitt eine Symmetrieachse hat, dann kann es von Vorteil sein, wenn Sie nur eine Hälfte des Ausschnitts erstellen und diese Hälfte dann spiegeln. Die Symmetrieachse können Sie zur Vermaßung nutzen.

3. Vermaßen Sie den Ausschnitt oder die Hälfte vollständig.

[Image of a dimensioned half-cutout.]
*Abb. A-219 Beispiel: Halber Ausschnitt*

> **Verwendete Maßkanten beachten!**
> Wenn Sie einen Ausschnitt erstellen, dann soll dieser später in einer Kontur positioniert werden und eine Kante entfällt (sonst entsteht kein Ausschnitt sondern eine Innenkontur). Achten Sie beim Vermaßen darauf, so zu vermaßen, dass die entsprechende Kante entfallen kann und der Ausschnitt dennoch vollständig vermaßt ist.

4. Wechseln Sie in die Ansicht Geometrie. A+W CAD Designer (Shapes) zeigt den Ausschnitt (oder die Hälfte) maßstabsgerecht an.
5. Wenn Sie nur eine Hälfte des Ausschnitts erstellt haben, dann spiegeln Sie die Kontur an der entsprechenden Kante.
6. Wechseln Sie in die Ansicht Innenkonturen.
7. Wenn zu dem erstellten Ausschnitt immer auch eine Bohrung gehört, dann ergänzen Sie die Bohrung und vermaßen Sie diese. Wenn Sie den Ausschnitt als Hälfte erstellt und gespiegelt haben, dann können Sie die Symmetrieachse als Bezug für die Vermaßung der Bohrung verwenden.

*A-470*
*A+W CAD Designer (Shapes) Überblick*
---
## Werkzeuge
### Konkrete Fragestellungen

8. Betätigen Sie `<Strg> + <D>`, damit A+W CAD Designer (Shapes) die Anzeige mit den gültigen Maßen aktualisiert.
9. Ergänzen Sie ggf. Maße, die Sie in der endgültigen Zeichnungsansicht sehen wollen und definieren Sie diese als messend.

[Image: Drawing of a complete cutout with a drill hole, fully dimensioned.]
*Abb. A-220 Beispiel: Ganzer Ausschnitt mit Bohrung*

10. Vervielfachen Sie den Ausschnitt so oft, wie Sie ihn normalerweise in einer Kontur benötigen. Damit müssen Sie nur einen Import durchführen und haben gleich die benötigte Anzahl Ausschnitte.
    - Wechseln Sie dazu in die Ansicht Geometrie.
    - Kopieren Sie den Ausschnitt.
    - Wechseln Sie in die Ansicht Innenkonturen.
    - Setzen und vermaßen Sie das Bohrloch (falls erforderlich).

> **In der Kopie fehlt die Symmetrieachse!**
> Wenn Sie den ersten Ausschnitt über das Spiegeln einer Hälfte erstellt haben, dann hatten Sie eine Mittellinie als Bezug zum Vermaßen. Diese Mittellinie fehlt in der Kopie.

11. Bereiten Sie die Darstellung der Ausschnitte in der Endprodukt-Zeichnung vor. Wechseln Sie dazu in die Ansicht Endprodukt in die Darstellung Zeichnung. Entfernen Sie dort die Maße, die Sie in der Zeichnung nicht benötigen.
    Wenn Sie mehrere identische Ausschnitte haben, reicht es oft aus, nur einen Ausschnitt ausreichend vermaßt darzustellen.

*A+W CAD Designer (Shapes) Überblick*
*A-471*
---
## Konkrete Fragestellungen
### Werkzeuge

[Image of two cutouts with drill holes, prepared as a final drawing.]
*Abb. A-221 Beispiel 2: Ausschnitte mit Bohrung als Zeichnung*

12. Speichern Sie die Datei mit einem Namen und zugehörigen Informationen, mit dem Sie auf den Inhalt schließen können.

### Tür erstellen und Ausschnitte positionieren
1.  Erstellen Sie die Grundform der Tür als Skizze oder wählen Sie diese aus dem Modellkatalog.
2.  Wechseln Sie in die Ansicht Innenkonturen.
3.  Setzen und vermaßen Sie, falls erforderlich, die Bohrungen für den Türgriff.
    Im Beispiel wurde in die Tür noch eine Senkbohrung angebracht, um die Möglichkeit einer Schnittdarstellung in der Zeichnung zu zeigen. Wenn Sie das Beispiel nachvollziehen wollen, dann setzen Sie auf die Tür ebenfalls eine Senkbohrung.
4.  Importieren Sie die Ausschnitte. Wählen Sie dazu Datei > Einfügen.

*A-472*
*A+W CAD Designer (Shapes) Überblick*
---
## Werkzeuge
### Konkrete Fragestellungen

5. Schieben Sie die Ausschnitte in die Nähe der Position, an die sie vermaßt werden sollen. A+W CAD Designer (Shapes) verschiebt die Ausschnitte samt zugehöriger Bohrung (falls vorhanden).
6. Vermaßen Sie jeden Ausschnitt an die Position der Türkante, an der er benötigt wird.

**Innenkonturen**
[Image of the door with cutouts and drill holes positioned and dimensioned within the door's contour.]
*Abb. A-222 Beispiel: Tür mit Ausschnitten und Bohrungen*

Im Beispiel wurde in die Tür noch ein weiterer Ausschnitt angebracht. Damit wird gezeigt, wie ein Ausschnitt mit einer Hilfslinie versehen wird, um den Ausschnitt durch Vermaßen der Hilfslinie zu positionieren.

7. Wechseln Sie in die Ansicht Skizze und erstellen und vermaßen Sie ein Rechteck, das Sie als Ausschnitt verwenden wollen.

*A+W CAD Designer (Shapes) Überblick*
*A-473*
---
## Konkrete Fragestellungen
### Werkzeuge

[Image: Skizze des Ausschnitts (Sketch of the cutout)]
*Abb. A-223 Beispiel: Skizze des Ausschnitts*

8.  Wechseln Sie in die Ansicht Geometrie und runden Sie die beiden rechten Ecken ab.

[Image: Vermaßter und abgerundeter Ausschnitt (Dimensioned and rounded cutout)]
*Abb. A-224 Beispiel 2: Vermaßter und abgerundeter Ausschnitt*

9.  Erstellen Sie eine Hilfslinie.
10. Wechseln Sie in die Ansicht Innenkonturen und verschieben Sie die Hilfslinie zum Ausschnitt.
11. Vermaßen Sie den Ausschnitt bezogen auf die Hilfslinie. Vermaßen Sie so, dass die Hilfslinie den Ausschnitt symmetrisch teilt. Vermaßen Sie die Hilfslinie parallel zum oberen oder unteren Rand.

*A-474*
*A+W CAD Designer (Shapes) Überblick*
---
## Werkzeuge
### Konkrete Fragestellungen

[Image: Vermaßter und abgerundeter Ausschnitt (Dimensioned and rounded cutout with helper line)]
*Abb. A-225 Beispiel: Vermaßter und abgerundeter Ausschnitt*

12. Verschieben Sie die Hilfslinie zur gewünschten Position an der Tür. A+W CAD Designer (Shapes) verschiebt den ganzen Ausschnitt. Wenn A+W CAD Designer (Shapes) nicht den ganzen Ausschnitt verschiebt, dann liegt ein Fehler in der Vermaßung vor.
13. Vermaßen Sie den Ausschnitt an die gewünschte Position an der Tür. Dabei können Sie die Vermaßung auf die Hilfslinie beziehen.
14. Ergänzen Sie die Kantenqualitäten, falls erforderlich. Wechseln Sie dazu in die Ansicht Kantenbearbeitung.

### Zeichnung gestalten
Im Zeichnungsausdruck benötigen Sie oftmals nicht alle Maße, die zur exakten geometrischen Bestimmung der Kontur erforderlich sind. Manchmal benötigen Sie auch andere Maßangaben. Die Zeichnung können Sie nach Ihren Bedürfnissen gestalten.
1. Wechseln Sie in die Ansicht Endprodukt und wählen Sie die Darstellung Zeichnung.
2. Vergrößern Sie den Bereich um einen kleinen Ausschnitt.
3. Fügen Sie eine Schnittzeichnung der Senkbohrung hinzu.
4. Schraffieren Sie die Schnittflächen der Schnittzeichnung.
5. Ergänzen Sie Beschriftungen, falls erforderlich.

*A+W CAD Designer (Shapes) Überblick*
*A-475*
---
## Konkrete Fragestellungen
### Werkzeuge

### Komplexe Kontur erstellen
Einige schwierige Konturen lassen sich dadurch einfach erstellen, dass Sie Teile dieser Kontur erstellen und diese dann verbinden und spiegeln.
Nachfolgend finden Sie die Beschreibung aller Arbeitsschritte, die Sie zum Erstellen einer komplexen Kontur benötigen. Um die Arbeitsschritte anschaulicher zu machen, werden die Arbeitsschritte anhand des folgenden Beispiels erklärt.

**Zeichnung Endprodukt**
[Image of a complex keyhole-shaped contour.]
*Abb. A-226 Beispiel: Komplexe Kontur*

Folgende Arbeitsschritte müssen Sie durchführen, um eine Tür mit Ausschnitten zu erfassen:
- Konturteile erstellen
- Konturen verbinden und spiegeln

*A-476*
*A+W CAD Designer (Shapes) Überblick*
---
## Werkzeuge
### Konkrete Fragestellungen

### Konturteile erstellen
Erstellen Sie nur Teile einer Kontur, wenn es einfacher ist, solche Teile zu vermaßen als die ganze Kontur zu vermaßen. Im gezeigten Beispiel ist es einfacher, folgende Teile zu erstellen als die ganze Kontur:
- Ein Viertelkreis
- Ein Viereck mit 3 rechten Winkeln und einem Bogen
- Ein Viereck mit 2 rechten Winkeln

1. Erstellen und Vermaßen Sie den Viertelkreis. Wechseln Sie dazu in die Ansicht Skizze.
2. Erstellen Sie ein Geradensegment (Radius), ein Bogensegment (Viertelkreis-Bogen) und wieder ein Geradensegment (Radius).
3. Vermaßen Sie die Winkel und den Radius.

> **Kreise als Viertelkreise erstellen!**
> Wenn Sie Kreisformen benötigen, dann können Sie diese am einfachsten aus dem Modellkatalog übernehmen. Wenn Sie Kreise selbst konstruieren wollen, dann geht dies mit A+W CAD Designer (Shapes) am Besten über Viertelkreise.

[Image of a dimensioned quarter circle.]
*Abb. A-227 Beispiel: Viertelkreis*

4. Erstellen und vermaßen Sie das Viereck mit 3 rechten Winkeln und einem Bogen. Erstellen Sie dazu drei Geradensegmente und ein Bogensegment und vermaßen Sie diese.

[Image of a dimensioned shape with three right angles and one arc.]
*Abb. A-228 Beispiel: Viereck mit 3 rechten Winkeln*

5. Erstellen und vermaßen Sie das Viereck mit 2 rechten Winkeln. Erstellen Sie dazu vier Geraden und vermaßen Sie diese.

*A+W CAD Designer (Shapes) Überblick*
*A-477*
---
## Konkrete Fragestellungen
### Werkzeuge

[Image of a dimensioned trapezoid with two right angles.]
*Abb. A-229 Beispiel: Viereck mit 2 rechten Winkeln*

### Ergänzende Informationen
- "Skizze erstellen und vermaßen" auf Seite A-236
- "Segmente vermaßen" auf Seite A-260
- "Kreise und Bögen vermaßen" auf Seite A-283

### Konturen verbinden und spiegeln
1.  Wechseln Sie in die Ansicht Geometrie und stellen Sie die Teile der Kontur so zueinander, wie Sie diese verbinden wollen.
2.  Löschen Sie die Segmente der Teilformen, die durch das Verbinden der Kontur entfallen werden.

[Image showing the individual parts of the keyhole shape ready to be connected.]
*Abb. A-230 Beispiel: Konturen verbinden*

*A-478*
*A+W CAD Designer (Shapes) Überblick*
---
## Werkzeuge
### Konkrete Fragestellungen

> **Erst Segmente verbinden und dann weitere Segmente löschen!**
> Löschen Sie die nicht mehr benötigten Segmente von 2 Teilformen. Verbinden Sie diese, bevor Sie weitere Segmente löschen, die beim Verbinden mit der nächsten Teilform überflüssig werden.

3.  Verbinden Sie die ersten beiden Teilformen.
4.  Wiederholen Sie die Schritte 2 und 3 mit der dritten Teilform (Segmente löschen und Teilformen verbinden).
5.  Spiegeln Sie die neu erstellte Kontur an einem der Segmente der Symmetrieachse. Als Mittellinie, auf die Sie vermaßen können, bleibt immer die Linie stehen, die Sie als Spiegelachse gewählt haben.

> **Fehlende Maße!**
> Durch das Verbinden von Teilformen und das Spiegeln der Kontur sind eine Reihe von Maßen entfallen. A+W CAD Designer (Shapes) kann die Kontur darstellen, weil die Ausgangsformen ausreichend vermaßt waren. In der Darstellung für die Fertigung der Kontur müssen Sie jetzt die benötigten Maße noch eintragen.

6.  Gestalten Sie die Vermaßungen der Zeichnung.

### Ergänzende Informationen
- "Zwei offene Teilfiguren zu einer geschlossenen verbinden" auf Seite A-249
- "Kontur durch Spiegeln an einem Segment verdoppeln" auf Seite A-252
- "Ausdruck der Zeichnung bearbeiten" auf Seite A-401

*A+W CAD Designer (Shapes) Überblick*
*A-479*
---
## Konkrete Fragestellungen
### Werkzeuge

### Mit Modellen arbeiten
Um mit Modellen zu arbeiten, können Sie eigene Modelle definieren oder den Modellkatalog von A+W oder einen anderen Modellkatalog nutzen. Alle Modelle haben die Eigenschaft, dass ihre grundsätzliche Kontur festgelegt, die konkreten Maße aber noch variabel sind. Die Geometrie von Modellen wird daher mit Variablen beschrieben.

Zum Arbeiten mit Modellen finden Sie nachfolgend folgende Arbeiten beschrieben:
- Modell erstellen
- Modell verwenden

### Modell erstellen
1. Zeichnen Sie das Modell in der Ansicht Skizze.

> **Besonderheiten der Geometrie verdeutlichen!**
> Wenn das Modell Kanten hat, die nicht parallel zu gegenüberliegenden oder rechtwinklig zu benachbarten Kanten verlaufen, dann stellen Sie dies in der Skizze deutlich dar. Dadurch entstehen zwar verzerrte Skizzen, Sie haben aber später kein Problem zu entscheiden, wie das Vorzeichen bei der Vermaßung gewählt werden muss.

2. Vermaßen Sie die Skizze. Verwenden Sie zum Vermaßen nur solche Werkzeuge, deren Bezugskante eine der Kanten ist, zwischen denen der rechte Winkel liegt.

| Abbildung | Beschreibung |
| :--- | :--- |
| **A** [Icon] | A: Abstand zwischen einem Punkt und einem Schnittpunkt senkrecht zu einer Geraden vermaßen |
| **B** [Icon] | B: Abstand zwischen einem Punkt und einer Strecke vermaßen |

*Abb. A-231 Abstandswerkzeuge zur Modellvermaßung*

Verwenden Sie, je nach Erfordernis, die unter A und B angegebenen Werkzeuge zur Vermaßung.

| Abbildung | Beschreibung |
| :--- | :--- |
| **C** [Icon] | C: Horizontalen Abstand zwischen zwei Punkten vermaßen |
| **D** [Icon] | D: Vertikalen Abstand zwischen zwei Punkten vermaßen |

*Abb. A-232 Für Modelle ungeeignete Vermaßungswerkzeuge*

Vermeiden Sie die Vermaßung mit Werkzeugen ohne Bezugskante (C und D). Diese Werkzeuge erzeugen implizit Vermaßungen von anderen Typen, deren Verhalten bei beliebigen Kombinationen der Variablenwerte nicht vorhersagbar ist.

*A-480*
*A+W CAD Designer (Shapes) Überblick*
---
## Werkzeuge
### Konkrete Fragestellungen

3.  Benutzen Sie für Längen oder Winkel, die in der Zeichnung keinen festen Wert haben, Variablen. Geben Sie einfache Formeln, Variablen oder Funktion direkt im Wertefenster ein.

> **Namen der Variablen vereinbaren!**
> Wenn Sie variable Maße für Modelle mit Geschäftspartnern (Zulieferer, Hersteller oder Händler) austauschen, dann müssen Sie die Namen der Variablen in den Modellskizzen mit dem Geschäftspartner vereinbaren. Nur so ist ein eindeutiger und reibungsloser Datenaustausch möglich. Verwenden Sie dann nur die Variablennamen, die in der entsprechenden Vereinbarung festgelegt wurden.

4.  Geben Sie die Werte für die Variablen erst ein, wenn beim Neuzeichnen der Variablendialog angezeigt wird.

| Icon | Werkzeug | Beschreibung |
| :--- | :--- | :--- |
| E | [Icon] | E: Kontur durch Segment ausrichten |
| F | [Icon: Text] | F: Segment beschriften |

5.  Kennzeichnen Sie die Kante, die parallel zur X-Achse ausgerichtet werden soll.
6.  Nummerieren Sie, falls erforderlich, die Kanten entsprechend der Vereinbarung mit Ihrem Geschäftspartner. Geben Sie dabei nur die Zahl ein, keine führenden oder abschließenden Leerzeichen.

### Ergänzende Informationen
- Softwarereferenz, "Variablen bearbeiten" auf Seite A-188
- Tutorial, "Wertefenster (D)" auf Seite A-25
- "Segment beschriften" auf Seite A-239
- "Kontur durch Segment ausrichten" auf Seite A-376

### Modell verwenden
Wenn Sie Geometrien, die Sie in ähnlicher Form immer wieder benötigen, als Modell abgespeichert haben, dann können Sie eine konkret benötigte Kontur sehr schnell erstellen.

1.  Öffnen Sie die Datei, die das Modell enthält.
2.  Rufen Sie den Dialog Variablen bearbeiten auf.
    Betätigen Sie dazu `<Alt> + <E>`.
3.  Geben Sie für die Variablen die konkret benötigten Werte ein und bestätigen Sie Ihre Eingabe mit [Übernehmen]. A+W CAD Designer (Shapes) stellt die Kontur mit den neuen Werten der Variablen dar.
4.  Speichern Sie die Datei unter einem neuen Namen.

### Ergänzende Informationen
- Softwarereferenz, "Variablen bearbeiten" auf Seite A-188
- Softwarereferenz, “Speichern unter" auf Seite A-170

*A+W CAD Designer (Shapes) Überblick*
*A-481*
---
## Konkrete Fragestellungen
### Werkzeuge

### Mit Variablen arbeiten
Mit Variablen können Sie Modelle erstellen.
Ein weiteres Anwendungsgebiet ist die variable Gestaltung von Ansichten in A+W CAD Designer (Shapes). Je nach Größenverhältnis kann es z. B. sein, dass Kanten auf einem Ausdruck parallel oder rechtwinklig aussehen, tatsächlich aber eine geringe Abweichung davon haben. Mit Hilfe von Variablen können Sie Bedingungen formulieren, die eine Zeichnung verzerren, um Geometrien zu verdeutlichen. Folgende Arbeiten sind nachfolgend beschrieben:
- Bedingungen formulieren
- Variablen in der Zeichnung verwenden

#### Ergänzende Informationen
- "Mit Modellen arbeiten" auf Seite A-480

### Bedingungen formulieren
A+W CAD Designer (Shapes) unterstützt außer Variablen auch arithmetische Ausdrücke in Variablen.

Logische Fallunterscheidungen müssen Sie mit arithmetischen Mitteln formulieren. Eine wesentliche Rolle spielt hierbei die Signum-Funktion `sign(x)`. `sign(x)` hat folgende Eigenschaften:
- `sign(x) = 1`, wenn x ≥ 0
- `sign(x) = -1`, wenn x < 0
- `sign(x) - sign(-x) = 2`, wenn x > 0
- `sign(x) - sign(-x) = 0`, wenn x = 0
- `sign(x) - sign(-x) = -2`, wenn x < 0

Mithilfe der Signum-Funktion lassen sich die folgenden arithmetischen Isolationsausdrücke bilden (ein Isolationsausdruck ist ein Ausdruck, der den Wert 1 hat, wenn eine Bedingung erfüllt ist, und den Wert 0, wenn sie nicht erfüllt ist):

| Bedingung | Isolationsausdruck |
| :--- | :--- |
| x < y | 0.5\*(1-sign(x-y)) |
| x ≤ y | 0.5\*(1+sign(y-x)) |
| x > y | 0.5\*(1-sign(y-x)) |
| x ≥ y | 0.5\*(1+sign(x-y)) |
| x = y | 0.5\*(sign(y-x)+sign(x-y)) |
| x ≠ y | 1 - 0.5\*(sign(y-x)+sign(x-y)) |

**Tab. A-46: Isolationsausdrücke**

Damit gilt für `f(y-x) = (sign(y-x)-sign(-(y-x))/2`:
- `= 1`, wenn y > x

*A-482*
*A+W CAD Designer (Shapes) Überblick*
---
## Werkzeuge
### Konkrete Fragestellungen

- `= 0`, wenn y = x
- `= -1`, wenn y < x

Damit haben Sie alle Fallunterscheidungen, die Sie benötigen.

1.  Erstellen Sie in der Ansicht Skizze ein Modell mit Variablen. Die weitere Beschreibung orientiert sich an dem nachfolgend gezeigten Beispiel.

[Image: A drawing of a shape with dimensions represented by variables like H, W, D1, H1, etc.]
*Abb. A-233 Beispiel: Modell mit Variablen als Skizze*

Die Variablen D1, D2, H, H1, W und W1 sind Variablen, die eingegeben werden müssen (manuell oder mit einer Übergabedatei).

In diesem Beispiel können folgende Situationen auftreten:
- Das Verhältnis von Höhe zu Breite (H zu W) ist für eine maßstäbliche Zeichnung ungünstig. Dies ist z. B. dann der Fall, wenn H > 4 * W. Dann sollte die Zeichnung nicht mehr maßstäblich dargestellt, aber richtig beschriftet werden.
- Das Verhältnis von D2 zu H oder D1 zu H oder H1 zu H ist so klein, dass es auf der Zeichnung schlecht zu sehen ist und daher übertrieben dargestellt werden soll. Dies ist z. B. dann der Fall, wenn das Verhältnis D2...

*A+W CAD Designer (Shapes) Überblick*
*A-483*
---
## Konkrete Fragestellungen
### Werkzeuge

- ...zu H kleiner ist als 1:10 und wenn das Verhältnis D1 oder H1 zu H kleiner ist als 1:20.
- Die Gesamthöhe und die Gesamtbreite der Kontur wird durch große Werte für D1 oder D2 so stark beeinflusst, dass D1 und D2 bei der Ermittlung der Größenverhältnisse berücksichtigt werden müssen.

2.  Wechseln Sie in die Ansicht Geometrie. A+W CAD Designer (Shapes) zeigt den Dialog Variablen bearbeiten an. Geben Sie dort die im Beispiel angegebenen Werte ein.
3.  Ermitteln Sie die Gesamthöhe und Gesamtbreite der Kontur. Erstellen Sie dazu die Variablen `_HTot` und `_WTot`. Verwenden Sie dazu die Funktion `max(x1;x2;...;xn)`.
    - `_HTot = max(H;H-D2)`
    - `_WTot = max(W;W-D1)`
    Verwenden Sie H-D2 und W-D1, weil D1 und D2, wenn sie negative Werte haben, die Höhe und Breite vergrößern.
4.  Ermitteln Sie das Größenverhältnis der Kontur und prüfen Sie, ob es das Verhältnis 1:4 unterschreitet. Wenn das Verhältnis kleiner ist, dann berechnen Sie die zum Verhältnis 1:4 fehlende Strecke. Erstellen Sie dazu folgende Variablen:
    - `_HzuW = _HTot / _WTot`
    - `__fGr4zu1 = 0.5*(1-sign(4-_HzuW))`
      Dieser Isolationsausdruck = 1, wenn Höhe zu Breite > 4.
    - `_DStreck = __fGr4zu1*(_HTot/4-_WTot)`
      `_DStreck` wird später bei der Erstellung der Zeichnung benötigt. Eine Streckung findet nur statt, wenn das Verhältnis Höhe zu Breite größer als 4 ist. Dann wird um den Betrag gestreckt, der an diesem Verhältnis fehlt (`_HTot/4 - _WTot`). Beachten Sie dabei die Berechnungsvorschrift Punkt vor Strich (`(_HTot/4) - _WTot`).

> **Namenskonvention für Variablen beachten!**
> Zur besseren Übersicht wurden in diesem Beispiel folgende Regeln für die Variablennamen eingehalten: Variablen, deren Name mit einem Unterstrich beginnen, sind Variablen, die im Wertefenster eingegeben werden. Variablen, die mit zwei Unterstrichen beginnen, werden zur Berechnung von Zwischenschritten (z. B. Isolationsausdrücke) verwendet.

5.  Ermitteln Sie die Größe der vertikalen Schräglage und prüfen Sie ob das Verhältnis 1:10 unterschritten wird. Wenn das Verhältnis kleiner ist, dann berechnen Sie die zum Verhältnis 1:10 fehlende Strecke. Erstellen Sie dazu folgende Variablen:
    - `_fD2 = 0.5*(sign(D2)-sign(-D2))`
      `_fD2` ist 0, wenn D2 = 0. Wenn D2 > oder < 0, dann muss übertrieben werden, bis das Verhältnis 1:10 erreicht ist.
    - `__VerschD2 = max(H/10-abs(D2);0 mm)`
      Die Kante ist ja bereits um D2 abgeschrägt. Die fehlende Schräge ist demnach H/10-D2. Da D2 auch ein negatives Vorzeichen haben kann, muss der Absolutbetrag von D2 genommen werden: `H/10-abs(D2)`. Ist

*A-484*
*A+W CAD Designer (Shapes) Überblick*
---
## Werkzeuge
### Konkrete Fragestellungen

nun D2 bereits größer als H/10, so ist dieser Ausdruck negativ. In diesem Fall lieferte der Ausdruck den Wert 0 mm, so dass keine Übertreibung angewendet wird.
- `_SchrD2 = (-1)*_fD2*_VerschD2`
  Das Vorzeichen der Übertreibung ist negativ, weil D2 in der Richtung nach innen positiv ist.

6.  Ermitteln Sie die Größe der horizontale Schräglage für D1 und prüfen Sie, ob das Verhältnis 1:20 unterschritten wird. Wenn das Verhältnis kleiner ist, dann berechnen Sie die zum Verhältnis 1:20 fehlende Strecke. Erstellen Sie dazu, analog zum vorherigen Schritt, folgende Variablen:
    - `_fD1 = 0.5*(sign(D1)-sign(-D1))`
    - `VerschD1 = max(H/20-abs(D1);0 mm)`
    - `SchrD1 = (-1)*__fD1*__VerschD1`

7.  Ermitteln Sie die Größe der horizontale Schräglage für H1 und prüfen Sie, ob das Verhältnis 1:20 unterschritten wird. Wenn das Verhältnis kleiner ist, dann berechnen Sie die zum Verhältnis 1:20 fehlende Strecke. Erstellen Sie dazu, analog zum vorherigen Schritt, folgende Variablen:
    - `__fH1 = 0.5*(1+sign(H/20-H1))`
      Berücksichtigen Sie hierbei, dass H1 nicht 0 oder negativ sein kann. Daher reicht der Isolationsausdruck für H1 ≤ H/20.
    - `VerschH1 = H/20-H1`
      Berücksichtigen Sie hierbei, dass H1 nicht 0 oder negativ sein kann. Daher entfällt die max-Funktion.
    - `_SchrH1 = (-1)*__fH1*__VerschH1`

Jetzt sollten sie folgende Variablen in A+W CAD Designer (Shapes) definiert haben:
[Image: Screenshot of the 'A+W Shaping & Nesting-Variablen bearbeiten' dialog, showing a list of defined variables and their expressions.]
*Abb. A-234 Beispiel: Variablen für die Übertreibung von Maßen*

8.  Schließen Sie den Dialog und richten Sie die die Kontur senkrecht zur oberen Kante aus.

*A+W CAD Designer (Shapes) Überblick*
*A-485*
---
## Konkrete Fragestellungen
### Ergänzende Informationen
- "Kontur verzerren" auf Seite A-402

### Werkzeuge
#### Variablen in der Zeichnung verwenden
Die nachfolgende Beschreibung setzt voraus, dass Sie die in den vorhergehenden Arbeitsschritten beschriebenen Variablen definiert haben.

1.  Wechseln Sie in der Ansicht Endprodukt in das Register Zeichnung. A+W CAD Designer (Shapes) zeigt die erstellte Kontur maßstäblich an. Die Maße D1 und D2 im Beispiel sind kaum zu erkennen.
2.  Wählen Sie das angezeigte Werkzeug und klicken Sie auf die rechte Kante der Kontur.
    [Icon for distorting a contour]
3.  Geben Sie im Wertefenster die Variable `_DStreck` ein und betätigen Sie [OK]. A+W CAD Designer (Shapes) verändert die Darstellung der Kontur.

> **Reihenfolge der Werkzeuge beachten!**
> Es ist wichtig, dass Sie beim Anwenden der Werkzeuge die richtige Reihenfolge einhalten. Wenden Sie zuerst das Werkzeug *Kontur verzerren* an allen erforderlichen Stellen an. Wenden Sie erst danach das Werkzeug *Kantenabhängige Randeinzüge bei freien Formen* an. Beachten Sie bei der Anwendung von *Kantenabhängige Randeinzüge bei freien Formen*, dass sich die einzelnen Anwendungen überlagern, wenn sie sich auf die gleiche Ecke beziehen.

4.  Wählen Sie das angezeigte Werkzeug und klicken Sie auf die Kante, deren Schräglage Sie verändern wollen.
    [Icon for modifying the slant of an edge]
    Klicken Sie in die Nähe des Punktes, den Sie verschieben wollen.
5.  Geben Sie im Wertefenster die Variable ein, mit der die Schräglage der Kante verzerrt werden soll und betätigen Sie [OK]. A+W CAD Designer (Shapes) verändert die Darstellung der Kontur.
    - Wenn Sie die untere Kante markiert haben, geben Sie die Variable `_SchrD2` ein.
    - Wenn Sie die linke Kante markiert haben, geben Sie die Variable `_SchrD1` ein.
    - Wenn Sie die schräge Kante oben links markiert haben, geben Sie die Variable `_SchrH1` ein.

Die nachfolgende Abbildung zeigt die Zeichnung mit und ohne Übertreibungen:

*A-486*
*A+W CAD Designer (Shapes) Überblick*
---
## Werkzeuge
### Konkrete Fragestellungen

[Image: Side-by-side comparison of the same drawing, one without exaggeration and one with exaggerated small features.]
*Abb. A-235 Beispiel: Zeichnung mit und ohne Übertreibung*

6.  Wenn Ihnen die Vermaßunge von A+W CAD Designer (Shapes) nicht gefallen und Sie andere Maße benötigen, wechseln Sie in der Ansicht Endprodukt in das Register S&N. Geben Sie dort die benötigten Maße mit der Option `messend` im Wertefenster ein.
    Wechseln Sie anschließend wieder in das Register Zeichnung und löschen Sie nicht benötigte Maße.

### Ergänzende Informationen
- Tutorial, "Wertefenster (D)" auf Seite A-25
- "Kantenabhängige Randeinzüge bei freien Formen" auf Seite A-406
- "Kontur verzerren" auf Seite A-402

*A+W CAD Designer (Shapes) Überblick*
*A-487*
---
## Konkrete Fragestellungen
### Werkzeuge

### Wie werden Scheiben bearbeitet
Wenn Sie eine Scheibe in ihrer Kontur vollständig beschrieben haben, dann können Sie Informationen zur Bearbeitung (Schneiden, Brechen, Bohren, Schleifen, etc.) im A+W CAD Designer (Shapes) angeben. Nachfolgend finden Sie Beschreibungen zu folgenden Themen:
- Zuschnitt vorbereiten
- Kantenbearbeitung festlegen
- Ecken bearbeiten

### Zuschnitt vorbereiten
Beim Zuschnitt einer Kontur müssen Sie einige Randbedingungen beachten. A+W CAD Designer (Shapes) unterstützt Sie bei der Lösung folgender Probleme:

**Radien sind zu klein zum Zuschneiden**
- "Ecke zuspitzen" auf Seite A-322

**Bruchstücke sind zu groß**
- "Hilfsschnitt durch Fortsetzung eines Segmentes erfassen" auf Seite A-359
- "Hilfsschnitt durch Verlängerung eines Segmentes erfassen" auf Seite A-361
- "Hilfsschnitt erfassen, um den Bruchrand zu teilen" auf Seite A-362
- "Hilfsschnitt erfassen, um zwei Konturen zu trennen" auf Seite A-364

### Bruchränder vorgeben
1.  Wechseln Sie in die Ansicht Zuschnitt.
    A+W CAD Designer (Shapes) zeigt um die Kontur ein Rechteck mit gestrichelten Linien an. Dieses entsteht durch die in der sn.ini hinterlegten Maße, die beim Zuschnitt als Bruchrand (Abstand zur Kontur in Abhängigkeit von der Glasstärke) eingehalten werden sollen.
2.  Prüfen Sie, ob die Maßangaben der Bruchränder korrekt sind. Klicken Sie dazu auf das gestrichelte Rechteck oder auf das angezeigte Werkzeug.
    [Icon for editing break-off edges]
    A+W CAD Designer (Shapes) zeigt im Wertefenster an, welche Bruchränder eingehalten wurden.
    Wenn in der Zeichnung mehrere Zuschnitte enthalten sind, dann müssen Sie nach dem Auswählen des Werkzeugs noch das gewünschte Rechteck anklicken.
3.  Prüfen Sie die angezeigten Ergebnisse im Wertefenster:

*A-488*
*A+W CAD Designer (Shapes) Überblick*
---
## Werkzeuge
### Konkrete Fragestellungen

| Anzeig | Bedeutung |
| :--- | :--- |
| e | |
| <> | Breite des Primitivs (Kontur plus Bruchrand links und rechts) |
| ^= | Höhe des Primitivs (Kontur plus Bruchrand oben und unten) |
| <= | linker Bruchrand |
| >= | rechter Bruchrand |
| ^= | oberer Bruchrand |
| v= | unterer Bruchrand |

**Tab. A-47: Wertefenster für Bruchränder**

4.  Passen Sie die Bruchränder an, falls erforderlich. Klicken Sie dazu zunächst auf das Symbol rechts neben dem Wert, den Sie ändern wollen. A+W CAD Designer (Shapes) ändert die Anzeige des Wertes auf rot und gibt das Feld zur manuellen Eingabe frei. Geben Sie jetzt den gewünschten Wert ein und betätigen Sie [OK].
5.  Wenn Sie die Größe des Primitivs nicht über die Bruchränder sondern die Bruchränder über die Maße des Primitivs bestimmen wollen, dann wählen Sie das angezeigte Werkzeug.
    [Icon for editing primitive size]
6.  Prüfen und ändern Sie ggf. die angezeigten Werte im Wertefenster:

| Anzeig | Bedeutung |
| :--- | :--- |
| e | |
| <> | Breite des Primitivs (Kontur plus Bruchrand links und rechts) |
| ^= | Höhe des Primitivs (Kontur plus Bruchrand oben und unten) |
| <=> | Breitenänderung auf beide Bruchränder aufteilen |
| < | Breitenänderung nur am linken Bruchrand anpassen |
| > | Breitenänderung nur am rechten Bruchrand anpassen |
| D = | Dicke der Scheibe |
| ^=v | Höhenänderung auf beide Bruchränder aufteilen |
| ^ | Höhenänderung nur am oberen Bruchrand anpassen |
| v | Höhenänderung nur am unteren Bruchrand anpassen |

**Tab. A-48: Wertefenster für Primitiv**

7.  Geben Sie, falls erforderlich, neue Maße für das Primitiv ein.

*A+W CAD Designer (Shapes) Überblick*
*A-489*
---
## Konkrete Fragestellungen
### Werkzeuge

8.  Wählen Sie, wie A+W CAD Designer (Shapes) die Maßänderung auf die bestehenden Bruchränder aufteilen soll und betätigen Sie [OK].

> **Schneidlinie**
> Am Schneidtisch geschnitten wird später das umschließende Rechteck (gestrichelte Linie) und die volle schwarze Konturlinie.

### Ergänzende Informationen
- "Breite und Höhe des zu schneidenden umschreibenden Rechtecks eingeben" auf Seite A-372
- "Bruchränder für zu schneidendes Modell erfassen" auf Seite A-373

### Kantenbearbeitung festlegen
Bei der Kantenbearbeitung unterscheidet A+W CAD Designer (Shapes) Kantenarten und Kantenqualitäten.

Mit Kantenarten können Sie unterscheiden, ob eine Kante als Standardkante, Modellkante oder Spezialkante definiert werden soll. Entsprechend unterschiedlich können Sie die Kostenkalkulation in einem angeschlossenen Auftragserfassungssystem gestalten.

#### Kanten definieren
- "Kante als Standardkante definieren" auf Seite A-425
- "Kante als äußere Modellkante definieren" auf Seite A-426
- "Kante als innere Modellkante definieren" auf Seite A-426
- "Kante als Modell-Sonderkante definieren" auf Seite A-425

Mit Kantenqualitäten legen Sie fest, wie einzelne oder alle Kanten einer Scheibe bearbeitet werden sollen (z. B. Schleifen, Polieren, etc.). Dazu stehen Ihnen eine Vielzahl von Bearbeitungen zur Verfügung:
- "Kanten bei Einfachglas bearbeiten" auf Seite A-412
- "Kanten an VSG/ISO bearbeiten" auf Seite A-419

### Ecken bearbeiten
Ecken können Sie abrunden oder fasen (abschneiden). Rundecken und Fasen können Sie als normale Bearbeitung oder als sogenannte kaufmännische Rundecke oder Fase anbringen.

Die kaufmännische Rundecke oder Fase gibt A+W CAD Designer (Shapes) über AWBroke als Element der Stückliste an die Auftragserfassung zurück. In der Bearbeitung unterscheiden sich die kaufmännischen Rundecken und Fasen nicht von denen, die keine Stücklisteninformation besitzen.

Weitere Informationen zu den Eckbearbeitungen finden Sie unter:
- "Schneidweg an Ecken festlegen" auf Seite A-369

*A-490*
*A+W CAD Designer (Shapes) Überblick*
---
# Werkzeuge
## Konkrete Fragestellungen

### Wie wird mit Bauglas gearbeitet
Die hier beschriebenen Arbeiten setzen voraus, dass Sie den allgemeinen Umgang mit A+W CAD Designer (Shapes) beherrschen und mit den Arbeiten zur Erfassung von Konturen grundsätzlich vertraut sind. Zu folgenden Themen finden Sie hier eine Beschreibung:
- "VSG und ISO" auf Seite A-491

### VSG und ISO
VSG- und ISO-Einheiten bestehen aus mehreren Scheiben, die zu einer Einheit gehören. Verschiedene Bearbeitungen, die auf der Einheit vorgenommen werden, haben unterschiedlichen Auswirkungen auf die einzelnen Scheiben. Dazu zählen z. B.:

Grundsätzlich bietet Ihnen A+W CAD Designer (Shapes) zwei Wege an, um Scheiben als Einheit zu definieren und entsprechend zu behandeln:
- Scheiben aufeinander ausrichten
- Einheiten mit Stückliste bearbeiten

#### Ergänzende Informationen
- Werkzeuge, "Planar-Befestigung einfügen" auf Seite A-407
- Werkzeuge, "Kanten an VSG/ISO bearbeiten" auf Seite A-419

### Scheiben aufeinander ausrichten
Bei dieser Arbeitsweise erstellen Sie die einzelnen Scheiben einer Einheit nebeneinander in einer Datei. In der Ansicht Einheit richten Sie die Scheiben aufeinander aus und bilden so die Einheit.

1.  Erstellen Sie eine Kontur.
2.  Wechseln Sie in die Ansicht Geometrie.
3.  Markieren und kopieren Sie die Kontur.
4.  Wechseln Sie in die Ansicht Kantenbearbeitung.
5.  Vergeben Sie den Konturen Nummern.

> **Bearbeitungen werden erst nach einer Nummerierung übernommen!**
> Erst wenn Sie den Konturen Nummern vergeben haben, können Sie die Einheit und die einzelnen Scheiben getrennt bearbeiten. A+W CAD Designer (Shapes) fügt dann die Bearbeitungen, die Sie in der Ansicht Einheit verwenden, nicht mehr in den Ansichten Bohren und Bearbeiten ein.

6.  Wechseln Sie in die Ansicht Einheit.
7.  Hinterlegen Sie für jede Scheibe die benötigten Konturdaten.
8.  Legen Sie die beiden Scheiben übereinander und richten Sie diese aufeinander aus. Verwenden Sie dazu die Vermaßungswerkzeuge.
9.  Fügen Sie in der Ansicht Einheit die Bearbeitungen ein, die für die Einheit als ganzes gilt.

*A+W CAD Designer (Shapes) Überblick*
*A-491*
---
## Konkrete Fragestellungen
### Werkzeuge

10. Fügen Sie in den anderen Ansichten (Innenkonturen, Kantenbearbeitung) die Bearbeitungen ein, die nur für eine Einheit gelten.

### Ergänzende Informationen
- "Wie werden Konturen erfasst" auf Seite A-446
- "Auswahl kopieren, ausschneiden, einfügen oder löschen" auf Seite A-439
- "Segmente vermaßen" auf Seite A-260
- Softwarereferenz, "Lokale Formdaten" auf Seite A-186

### Einheiten mit Stückliste bearbeiten
Ab der Version 5.x kann A+W CAD Designer (Shapes) mit Stücklisten arbeiten. Dies bedeutet, dass Einheiten als Ober- und Unterteile in verschiedenen Stufen (Layern) dargestellt und bearbeitet werden können.

1. Öffnen Sie eine Datei, die einen Stücklisten-Aufbau enthält.

> **Daten mit Stücklistenaufbau von Vorsystemen**
> Dateien mit Stücklistenaufbau werden bei der Zusammenarbeit mit einer Auftragserfassung von A+W Enterpise oder A+W Business an A+W CAD Designer (Shapes) übergeben.

2. Wechseln Sie in die Ansicht Geometrie und wählen Sie das Register Stufe 0.
3. Vergeben Sie der Kontur in der Stufe 0 die Nummer 0.

> **Weitere Nummern vergibt CAD Designer automatisch!**
> Vergeben Sie nur der obersten Stufe die Nummer 0. Alle weiteren Nummern im Aufbau der Einheit vergibt A+W CAD Designer (Shapes) automatisch selbst.

4. Fügen Sie Bearbeitungen, die für die ganze Einheit gelten, in der Stufe 0 der jeweiligen Ansicht (Bohren, Kantenbearbeitung, ...) ein.

### Ergänzende Informationen
- "Über CAMXML-Dateien" auf Seite A-519
- "Zusammenarbeit mit A+W Enterprise" auf Seite A-495
- "Zusammenarbeit mit A+W Business" auf Seite A-508
- "Scheibenfolgen für Einheiten definieren" auf Seite A-428

*A-492*
*A+W CAD Designer (Shapes) Überblick*
---
## Werkzeuge
### Konkrete Fragestellungen

### Wie werden Zeichnungen gedruckt
Als Zeichnung wird die Ausgabe der Kontur auf dem Drucker bezeichnet. Sie können für verschiedene Ansichten (Kantenbearbeitung, Endprodukt, ...) jeweils eine andere Zeichnung definieren. Je nach dem, aus welcher Ansicht Sie dann eine Zeichnung drucken, wird die jeweils zugehörige Zeichnung gedruckt.

Welche Zeichnung (Ansicht Kantenbearbeitung oder Ansicht Endprodukt) ein angeschlossenes Auftragserfassungssystem (A+W Enterpise oder A+W Business) verwendet, kann bei der Konfiguration des Auftragserfassungssystems festgelegt werden.

Bei der Zusammenarbeit mit A+W Enterpise wird dies in der SNAuto.ini bzw. der AWBroke.ini festgelegt.

Bei der Zusammenarbeit mit A+W Business wird dies in der Konfiguration eingestellt.

Zur Gestaltung von Zeichnungen in CAD Designer stehen Ihnen eine Reihe von Funktionen und Beschreibungen zur Verfügung:
- Werkzeuge, "Darstellung der Zeichnung ändern" auf Seite A-523
- Werkzeuge, "Ausdruck der Zeichnung bearbeiten" auf Seite A-401
- Softwarereferenz, "Textformat" auf Seite A-207
- Softwarereferenz, "Striche und Füllungen" auf Seite A-207

### Zeichnung in Worddatei drucken
A+W CAD Designer (Shapes) bietet die Möglichkeit, Zeichnungen und Beschriftungen in eine Worddatei zu exportieren. Dazu müssen Sie zuerst eine Vorlagedatei in Word erstellen. Wenn Sie eine solche Vorlagedatei in das Verzeichnis `Wordform` der A+W CAD Designer (Shapes)-Installation legen, dann steht diese Vorlage im Druckdialog von A+W CAD Designer (Shapes) zur Verfügung.
- Softwarereferenz, "Drucken Dialog..." auf Seite A-176

Um Informationen aus A+W CAD Designer (Shapes) in Word zu verwenden, stellt A+W CAD Designer (Shapes) die Informationen einer Zeichnung mit Platzhaltern zur Verfügung. Platzhalter sind z. B.:

| Information | Platzhalter |
| :--- | :--- |
| Dateiname | SN_FILE |
| Bearbeiter | SN_CLERK |
| Position der Grafik | SN_DRAWING |
| ... | |

**Tab. A-49 Beispiele für Platzhalter**

Die verfügbaren Platzhalter und deren Bedeutung können Sie sich ausdrucken.

*A+W CAD Designer (Shapes) Überblick*
*A-493*
---
## Konkrete Fragestellungen
### Werkzeuge

Wenn Sie eine Zeichnung über Word ausdrucken, dann wird die Zeichnung in der Auflösung in Word eingebunden, wie in der sn.ini angegeben. Ein Ausdruck über Word erreich nicht die grafische Qualität wie ein Ausdruck direkt aus A+W CAD Designer (Shapes).

Um Zeichnungen in Worddateien auszudrucken, müssen Sie folgende Arbeitsschritte durchführen:

### Wordvorlage erstellen
1. Erstellen Sie eine Worddatei mit den verfügbaren Platzhaltern. Verwenden Sie dazu im Druckdialog das Formular `<SNW>`.
2. Öffnen und gestalten Sie die Word-Datei mit den Platzhaltern nach Ihren Vorstellungen:
   - Löschen Sie die Platzhalter, die Sie nicht benötigen.
   - Setzen Sie den Platzhalter für die Grafik (SN_Drawing) in einen Grafikrahmen.
   - Ändern Sie Schriftarten.
   - Fügen Sie Texte hinzu.
   - Gestalten Sie das Layout.
   - ...
3. Speichern Sie die Datei unter dem gewünschten Namen und legen Sie die Datei in das Verzeichnis `Wordform` der A+W CAD Designer (Shapes)-Installation.
4. Wechseln Sie in A+W CAD Designer (Shapes) und dort in die gewünschte Ansicht. Wählen Sie im Druckdialog die erstellte Vorlagedatei und starten Sie den Ausdruck.
5. Prüfen Sie, ob das Ergebnis Ihren Vorstellungen entspricht und ändern Sie ggf. die Vorlage.

### Ergänzende Informationen
- Softwarereferenz, "Drucken Dialog..." auf Seite A-176

*A-494*
*A+W CAD Designer (Shapes) Überblick*
---
# Werkzeuge
## Konkrete Fragestellungen

### Wie ist die Zusammenarbeit mit anderen Programmen
A+W CAD Designer (Shapes) können Sie an ein kaufmännisches System (Auftragserfassung) oder eine Produktionssteuerung ankoppeln. Dabei werden Informationen zu einem Produkt aus der Auftragserfassung übernommen, in A+W CAD Designer (Shapes) ergänzt und an das angekoppelte System zurückgegeben. Nachfolgend finden Sie folgenden Arbeiten beschrieben:
- Zusammenarbeit mit A+W Enterprise
- Zusammenarbeit mit A+W Business
- Datenexport

### Zusammenarbeit mit A+W Enterprise
Wenn Sie mit A+W Enterpise arbeiten, dann können Sie direkt bei der Auftragserfassung für jede Auftragsposition eine Datei anlegen. Diese Arbeitsweise bezeichnet A+W Enterpise als Technische Auftragsbearbeitung (TAB). Voraussetzung für diese Zusammenarbeit zwischen A+W Enterpise und A+W CAD Designer (Shapes) ist eine vollständig ausgefüllte Konvertierungstabelle für die Artikelnummern. A+W CAD Designer (Shapes) benötigt jeden Artikel in einer A+W CAD Designer (Shapes)-eigenen Bezeichnung. Diese Bezeichnung wird in A+W Enterpise SN-Schlüssel genannt.

Die TAB mit A+W Enterpise in Zusammenarbeit mit A+W CAD Designer (Shapes) ermöglicht das Erzeugen von SN-Dateien aus der A+W Enterpise-Stückliste. Der Auftragserfasser kann mit A+W CAD Designer (Shapes) komplexe Produkte in der Stückliste vollständig beschreiben. Die Datei wird im Hintergrund erzeugt. Die in A+W CAD Designer (Shapes) ergänzte und jetzt vollständige Stückliste wird an A+W Enterpise zurückgegeben.

Technisch stehen Ihnen 2 Wege zur Verfügung:
- Kopplung über AWBroke
- Kopplung über SNAuto

### Kopplung über AWBroke
(Vordergrund- oder Online-TAB)

Wenn Sie aus A+W Enterpise heraus A+W CAD Designer (Shapes) starten wollen, dann muss die Stückliste mit den A+W Enterpise-Artikelnummern in eine Stückliste mit A+W CAD Designer (Shapes)-Artikelnummern umgesetzt werden. Diese Aufgabe übernimmt AWBroke. Die Tabelle, in der die A+W Enterpise-Artikelnummern und die zugehörigen A+W CAD Designer (Shapes)-Artikelnummern aufgelistet sind, können Sie in den A+W Enterpise-Stammdaten pflegen.

Um die Stücklisten-Informationen austauschen zu können wurde eine Stücklistenbeschreibungssprache (SL) entwickelt. Eine Datei, in der eine Stückliste in SL beschrieben ist, heißt SL-Skript. Solche Dateien haben die Erweiterung `.sl`.

Bei der TAB ist A+W Enterpise das Master-System und initiiert die Kopplung mit A+W CAD Designer (Shapes) wie nachfolgend dargestellt:

*A+W CAD Designer (Shapes) Überblick*
*A-495*
---
## Konkrete Fragestellungen
### Werkzeuge

[Workflow diagram showing the interaction between A+W Enterprise, AWBroke, and CAD Designer.]

**Legende zur Abbildung A-236: CAD Designer - A+W Enterprise mit AWBroke**
- **A**: Zuordnungstabelle pflegen
- **B**: Position erfassen mit Vorgabe-Stückliste
- **C**: Aufruf von CAD Designer über AWBroke
- **D**: Zuordnungsdaten lesen
- **E**: Vorgabe-Stückliste konvertieren
- **F**: CAD Designer starten
- **G**: Zurück zur Auftragsbearbeitung
- **H**: Ergebnis-Stückliste konvertieren
- **I**: SN-Datei speichern

Die Verbindung zwischen UNIX und MS Windows kann über ein mit Samba gemountetes Laufwerk oder mit ftp erfolgen.

### Arbeitsweise der Kopplung
Die Kopplung von A+W Enterpise mit A+W CAD Designer (Shapes) erfolgt über Betriebssystemgrenzen hinweg, da ALCIB auf UNIX läuft und AWBroke und A+W CAD Designer (Shapes) Anwendungen auf MS Windows sind.

**Artikelnummern (A)** Nach der Konfiguration von A+W Enterpise für die TAB mit A+W CAD Designer (Shapes) müssen Sie in den A+W Enterpise-Stammdaten eine Tabelle anlegen und pflegen. In dieser Tabelle werden die Artikelnummern von A+W Enterpise und die entsprechende Artikelnummer für A+W CAD Designer (Shapes) eingetragen. Die Artikelnummern für alle Standardgläser können Sie automatisch per Knopfdruck erzeugen. Artikelnummern für Bearbeitungen müssen Sie manuell pflegen.
- Werkzeuge, “A+W Enterprise-Stammdaten" auf Seite A-498

*A-496*
*A+W CAD Designer (Shapes) Überblick*
---
## Werkzeuge
### Konkrete Fragestellungen

**Position erfassen (B)** Erfassen Sie die Positionsdaten eines Auftrags in A+W Enterpise wie gewohnt. Wählen Sie in einer Auftragsposition einen Artikel aus.

**CAD Designer aufrufen (C)** Falls die Position mit A+W CAD Designer (Shapes) erfasst oder weiterbearbeitet werden soll, dann betätigen Sie im Mengenfeld der Position die Tastenkombination `<Ctrl> + <E>` oder klicken Sie auf die Symbolschaltfläche ShapingNesting. Als Reaktion auf den Tastendruck legt A+W Enterpise für die Position eine Vorgabe-Stückliste an und ruft AWBroke auf.

**Stückliste konvertieren und CAD Designer starten (D, E, F)** A+W Enterpise konvertiert die Vorgabestückliste mit Hilfe der Zuordnungstabelle. Diese Zuordnung befindet sich in der Tabelle snkey in der A+W Enterpise-Datenbank. AWBroke greift auf die Vorgabestückliste zu. Dann startet AWBroke A+W CAD Designer (Shapes) und übergibt die Daten der zuvor in A+W Enterpise ausgewählten Glasscheibe.

**Position bearbeiten und zurückgeben (G, H, I)** Nutzen Sie die Möglichkeiten von A+W CAD Designer (Shapes) zur vollständigen grafischen Beschreibung der Position (z. B. Vermaßung, Bohrungen, Kantenbearbeitungen). Wenn Sie die Position vollständig beschrieben haben, wählen Sie den Menüpunkt Zurück zur Auftragsbearbeitung.
A+W CAD Designer (Shapes) speichert die Produktbeschreibung jeweils in einer Datei. Diese Dateien sind positionspezifisch und gehören zu den Auftragsdaten. Die Datei bekommt ihren Namen aus dem Nummernkreis contour.mfo. Der Name wird in A+W Enterpise vergeben und ist schon in der Vorgabestückliste enthalten. A+W CAD Designer (Shapes) aktiviert AWBroke und stößt die Rückgabe der Ergebnisstückliste an. AWBroke greift mittels ODBC auf die INFORMIX-Datenbank zu und liest die Konvertierungstabelle.
AWBroke interpretiert die von A+W CAD Designer (Shapes) zur Verfügung gestellten Daten und schreibt die Ergebnisstückliste. Die Ergebnisstückliste wird als .sl-Datei im eingerichteten Verzeichnis auf dem UNIX-Rechner gespeichert. AWBroke tauscht die A+W CAD Designer (Shapes)-Artikelnummern (z. B. für die zugefügten Bearbeitungen) gegen die A+W Enterpise-Artikelnummern aus.
A+W Enterpise befindet sich seit dem Aufruf von A+W CAD Designer (Shapes) in einer Warteschleife. Sobald die Datei mit der Ergebnis-Stückliste da ist, werden die aktualisierten Auftragsdaten erzeugt und der Benutzer kann die Erfassung der Position in A+W Enterpise fortsetzen. Wenn Sie für weitere Auftragspositionen in A+W Enterpise wieder eine SN-Datei anlegen, dann werden für den mit A+W CAD Designer (Shapes) wieder die selben Dateinamen für die Vorgabestückliste und die Rückgabestückliste (SL-Dateien) verwendet. Die vorherigen Kommunikationsdateien (SL-Dateien) werden also überschrieben.

### Koppelbare Produkttypen
Die TAB mit A+W Enterpise, AWBroke und A+W CAD Designer (Shapes) ist nur für die hier aufgelisteten Produkttypen (Gläser und Bearbeitungen) verfügbar. Nicht aufgelistete Glasarten oder Bearbeitungen können mit der TAB auch nicht erfasst werden.

*A+W CAD Designer (Shapes) Überblick*
*A-497*
---
## Konkrete Fragestellungen
### Werkzeuge

#### Glasartikel
Die TAB mit A+W Enterpise, AWBroke und A+W CAD Designer (Shapes) kann diese Glasarten behandeln:
- Float-Gläser, unbearbeitet (Artikel 11xxxx).
- Float-Gläser, bearbeitetet (Artikel 15xxxx).
- ESG-Gläser (Artikel 30xxxx und 35xxxx) mit darunter liegendem einfachen Float (Artikel 11xxxx) oder bearbeitetem Float (Artikel 15xxxx).
- VSG aus Float oder ESG, bestehend aus den zuvor genannten Gläsern, jedoch kein Zuschnitt-VSG (Artikel 40xxxx).
- ISO-Einheiten, bestehend aus den zuvor genannten Gläsern, jedoch kein Stufen-ISO (Artikel 50xxxx).

#### Bearbeitungen (Artikel 90xxxx)
Die TAB mit A+W Enterpise, AWBroke und A+W CAD Designer (Shapes) kann diese Bearbeitungen behandeln:
- Zylindrische (normale) Bohrungen
- Senkbohrungen
- Gesäumte, geschliffene und polierte Kanten
- Definierbare Sonderkanten. Diese Sonderkanten sind nicht parametrisierbar. Es stehen 15 unterschiedliche Sonderkanten zur Verfügung.
- Symmetrische Eckabschnitte (Fasen), auch mit Kantenbearbeitung
- Rundecken, auch mit Kantenbearbeitung

### A+W Enterprise-Stammdaten
In den A+W Enterpise-Stammdaten muss für jeden Artikel ein so genannter A+W CAD Designer (Shapes)-Schlüssel hinterlegt sein, damit eine Vorgabe-Stückliste für A+W CAD Designer (Shapes) konvertiert werden kann.

Im A+W Enterpise wird die A+W CAD Designer (Shapes)-Schlüsselzuordnung unter Stammdaten > Schlüssel > Produktschlüssel > Shaping/Nesting-Artikel festgelegt.

> **Eindeutige CAD Designer-Artikelnummern**
> A+W CAD Designer (Shapes)-Schlüssel (hier die CAD Designer-Artikelnummern) sind eindeutig und enden immer mit einem Punkt `< . >`.

Die A+W CAD Designer (Shapes)-Schlüssel sind wie folgt aufgebaut:

#### Gläser
- Glasschlüssel beginnen mit G
- Es folgen 2 Ziffern für die Kategorie:
    - G01 für Float
    - G02 für ESG
    - G03, G08, G09 für VSG
    - G06 für ISO
- Es folgt eine beliebige Zahl (z. B. die A+W Enterpise-Artikelnummer):
  G02300008., ESG Float 8mm

*A-498*
*A+W CAD Designer (Shapes) Überblick*
---
## Werkzeuge
### Konkrete Fragestellungen

- Der Glasschlüssel kann abgekürzt werden:
  G02.ESG.

*A+W CAD Designer (Shapes) Überblick*
*A-499*
---
## Konkrete Fragestellungen
### Werkzeuge

#### Bearbeitungen

**Kantenqualitäten**
- Kantenschlüssel beginnen mit K
- Differenzierung nach Außenkante, Innenkante, Modellaußenkante und Modellinnenkante
- Der Kantenschlüssel kann eingeschoben werden:
  KG02300008.109., Polierte Außenkante auf ESG Float 8 mm
- Der Kantenschlüssel kann abgekürzt werden:
  KG02.109., Polierte Außenkante auf ESG

**Bohrlöcher**
- Bohrlochschlüssel beginnen mit D
- Es folgt eine 3-stellige Typkennung:
    - 101 = Standardbohrung
    - 102 = Senkbohrung beidseitig
    - 103 = Senkbohrung oben
    - 104 Senkbohrung unten
- Es folgen zwei 5-stellige Zahlengruppen für die Grenzwerte des Durchmessers in Zehntelmillimeter:
  D1010200005000.
- Der Bohrlochschlüssel kann nach dem Typ abgekürzt werden:
  D101.
- In den Bohrlochschlüssel kann ein Glasschlüssel eingeschoben werden:
  DG02300008.1010200005000.:
  Bohrung von 20 bis 50 mm auf ESG Float 8 mm
- Der Glasschlüssel kann abgekürzt werden:
  DG02.1010200005000.:
  Bohrung von 20 bis 50 mm auf ESG

**Ausschnitte**
- Ausschnittschlüssel beginnen mit A
- Dann folgt eine Ziffer, die die Ausschnittart festlegt:
    - 1 = Randausschnitt
    - 2 = Eckausschnitt
    - 3 = Innenausschnitt;
- Es folgen 4 beliebige Ziffern
- Dann folgen zwei 5-stellige Zahlen, die die Ausdehnung in x- und y-Richtung angeben:
  A100010010000080., Randausschnitt (Typ 1) mit x=100 mm, y=80 mm
- In den Schlüssel können Glas- und Kantenschlüssel eingeschoben werden:
  AKG02.109.100010010000080. für Randausschnitt (Typ 1) auf ESG mit polierten Kanten, Ausdehnung x=100 mm, y=80 mm

*A-500*
*A+W CAD Designer (Shapes) Überblick*
