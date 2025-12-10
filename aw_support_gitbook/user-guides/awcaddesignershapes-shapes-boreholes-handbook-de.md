---
title: "DE-HB-AWCADDesignerShapes_7"
source: "DE-HB-AWCADDesignerShapes_7.pdf"
tags: ["A+W CAD Designer", "Shapes", "CAD Software", "User Manual", "Technical Documentation", "Boreholes", "Countersinking", "Corner Editing", "Cutouts", "Surface Treatment"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a segment of the user manual for A+W CAD Designer (Shapes), providing detailed instructions on using various tools for creating and modifying geometric designs. It covers functions for boreholes, countersinks, auxiliary lines, corner modifications, cutouts, and surface treatments, aimed at users in the glass and manufacturing industries."
long_description: "This document serves as a comprehensive guide for the A+W CAD Designer (Shapes) software, focusing on the 'Werkzeuge' (Tools) module. It provides step-by-step instructions for a wide range of design and editing functions essential for creating precise technical drawings, particularly for glass manufacturing. Key topics include creating new boreholes by specifying coordinates, placing multiple boreholes along an arc, and managing borehole dimensions. The manual details various methods for creating countersinks (Senkbohrungen) and step drills (Stufenbohrungen), including conversion from standard boreholes and input via diameter or depth. It explains how to insert and manipulate auxiliary lines (Hilfslinien) to aid in dimensioning and positioning. A significant portion is dedicated to corner editing tools, such as cutting, rounding, chamfering, and tapering corners with precise control over distances and angles. Furthermore, the document covers the creation and placement of complex internal cutouts (Innenkonturen) and macros, including grouping elements and defining reference points for repeatable use. Finally, it addresses surface treatment tools, allowing users to define and apply various finishes like coatings, matting, sandblasting, and various types of printing (color, enamel, silk-screen) to specific areas of a design. The guide is structured to help both novice and experienced users master the functionalities of the A+W CAD Designer software."
---

# Werkzeuge

---
## Werkzeuge verwenden

### Neues Bohrloch durch Eingabe von X- und Y-Abstand zu bestehendem Bohrloch erfassen

Mit dieser Option können Sie ein neues Bohrloch erfassen, indem Sie den X und Y Abstand zu einem bereits vorhandenen Bohrloch eingeben.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie mit der linken Maustaste das vorhandene Bohrloch an, von dem aus das neue Bohrloch platziert werden soll. Sie können entweder den Mittelpunkt oder die Kontur des vorhandenen Bohrloches anklicken. Das ausgewählte Bohrloch wird nun vorläufig in rot dargestellt.
3.  Geben Sie im Wertefenster für x und y den gewünschten Abstand ein. Die Werte, die Sie eingeben, beziehen sich auf den Abstand von Lochmittel- punkt zu Lochmittelpunkt.
4.  Geben Sie im Wertefenster den Durchmesser des Bohrloches an.
5.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Das Bohrloch wird nun erzeugt und in der Segmentfarbe (normal schwarz) endgültig darge- stellt. Der x- und y-Abstand sowie der Durchmesser des Bohrloches wer- den als Text an diesem angebracht.

> **Bohrloch mit und ohne Text möglich!**
> Wenn Sie keinen Text am Bohrloch wünschen, können Sie diesen löschen. Weiterhin ist es möglich, mit dem Textwerkzeug Bohrlochdurchmesser an- geben einen beliebigen Text an das Bohrloch anzubringen. Ein gelöschter Bohrlochdurchmesser kann mit dem Werkzeug Bohrlochdurchmesser an- geben wieder angebracht werden.

### Bohrungen auf einem Bogen mit gleichen Abständen erfassen

Mit dieser Option können Sie gleich große Bohrungen erfassen, die mit gleichen Abständen entlang eines Bogens liegen. Es ist nicht notwendig, jede Bohrung einzeln zu erfassen. Geben Sie die Anzahl der Bohrungen, die Abstände sowie den Durchmesser ein und die Bohrungen werden au- tomatisch gesetzt.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie mit der linken Maustaste auf den Bogen, an dem die Bohrlöcher platziert werden sollen. Der ausgewählte Bogen wird nun vorläufig in rot dargestellt. Der Pfeil zeigt in Richtung der erzeugten Bohrlöcher.
3.  Das Wertefenster zeigt Ihnen die x- und y-Koordinaten sowie den Bogen- radius an. Geben Sie die Größe und Lage der Bohrpunkte an:
    *   Geben Sie im Feld a den Abstand von der Bohrlochmitte bis zum Bogen an.
    *   Geben Sie im Feld / den Bogenabstand (kreisförmig) von Bohrlochmitte zu Bohrlochmitte an.
    *   Geben Sie im Feld n die Anzahl der zu platzierenden Bohrpunkte an.
    *   Geben Sie im Feld o den Durchmesser der Bohrlöcher an.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Bohrlöcher wer- den nun erzeugt und in der Segmentfarbe (normal schwarz) endgültig dar- gestellt. Das 1. Bohrloch liegt dabei um den Bogenabstand / entfernt vom Anfang des angeklickten Bogens.

### Bohrlochdurchmesser angeben

Mit diesem Werkzeug können Sie fehlende (gelöschte) Bohrlochverma- ßungen einfügen. Sie können die Vermaßung (auch wenn sie zwischen- zeitlich geändert wurde) wiederherstellen. Dieses Werkzeug zeigt immer den richtigen Bohrlochdurchmesser an.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Wählen Sie das gewünschte Bohrloch. Diese färbt sich rot.
3.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Vermaßung des Bohrloches wird angezeigt.

### Bohrloch mit Vermaßung erfassen

Mit diesem Werkzeug können Sie ein Bohrloch erfassen, dessen Abstand von zwei Segmenten bekannt ist. Dabei wird jeweils ein senkrechter Ab- stand vom Segment zum Bohrlochmittelpunkt angenommen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Wählen Sie das erste Segment aus, gegen das Sie das Bohrloch positio- nieren wollen. Dieses färbt sich rot.
3.  Wählen Sie das zweite Segment aus, gegen das Sie das Bohrloch positio- nieren wollen. Dieses färbt sich grün.
4.  Geben Sie den Abstand zum ersten (roten) Segment im Eingabefeld D1 und den Abstand zum zweiten Segment im Eingabefeld D2 ein.
5.  Geben Sie im Feld o den Bohrlochdurchmesser ein.
6.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Danach wird das Be- rechnungsverfahren gestartet und das Bohrloch an die richtige Stelle posi- tioniert.

### Bohrungen auf einem Kreisbogen mit gleichem Winkelabstand erfassen

Mit diesem Werkzeug können Sie eine Anzahl gleich großer Bohrungen er- fassen, die auf einem Kreisbogen liegen. Den Kreismittelpunkt geben Sie dabei als Abstand zu zwei Segmenten an.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie nacheinander die beiden Segmente an, zu denen der Mittel- punkt des Kreisbogens vermaßt werden soll. A+W CAD Designer (Shapes) zeigt das erste angeklickte Segment rot, das zweite grün an.
3.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   r: Radius des Kreisbogens.
    *   <: Winkelabstand zwischen den Bohrungen.
    *   n: Anzahl der Bohrungen.
    *   o: Durchmesser der Bohrungen.
    *   d1: senkrechter Abstand des Mittelpunktes vom ersten Segment.
    *   d2: senkrechter Abstand des Mittelpunktes vom zweiten Segment.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) erstellt die angegebenen Bohrungen. Die Lage der Bohrpunkte können Sie noch verändern.
5.  Wählen Sie Neu zeichnen im Menü Ansicht, um eine Auswertung der akti- ven Vermaßung zu erzwingen und um die Skizze von A+W CAD Designer (Shapes) übersichtlicher vermaßen zu lassen.

### Konvertiere Bohrloch zur Senkbohrung

Da das DXF-Format keine Standardbeschreibung von Senklochbohrung kennt, war es bisher nur möglich, Kreise entweder immer als einfache Boh- rung oder immer als Senkbohrung zu importieren (gesteuert über die Kon- figuration). Mit diesem Werkzeug ist es nun gezielt möglich, eine importierte Bohrung zu einer Senklochbohrung zu konvertieren. Das Werk- zeug gibt es in zwei Varianten: bei der ersten Variante wird die Senkung über die Durchmesser der Senkung bestimmt, bei der zweiten Variante wir die Senkung durch die Senktiefe bestimmt. Welche Variante aktiv ist, wird durch die Konfigurationsdatei (Sn.ini) bestimmt.(Schalter DrillholeToCoun- terBoreByDiameter im Abschnitt User, Werte 1 (Standard) bzw. 0 für Ein- gabe über Durchmesser bzw. Tiefe). Dieses Werkzeug steht Ihnen in der Ansicht DXF-Import zur Verfügung.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Wählen Sie die Bohrung(en) aus, die konvertiert werden soll(en).
3.  Geben Sie im Wertefenster die geforderten Werte ein. Je nach Variante sind das:
    *   d: Kernlochdurchmesser.
    *   d1: Durchmesser der oberen Senkung.
    *   d2: Durchmesser der unteren Senkung.
    *   <1 und <2: Flankenwinkel bei d1 und d2 der Senkung
    bzw.
    *   d: Kernlochdurchmesser.
    *   t1: Tiefe der oberen Senkung.
    *   t2: Tiefe der unteren Senkung.
    *   <1 und <2: Flankenwinkel bei d1 und d2 der Senkung
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Bohrung wird nun in der Scheibe angezeigt.

### Senkbohrung mit Einsenkdurchmesser eingeben

Mit diesem Werkzeug geben Sie eine Senkbohrung mit einem beliebigen Flankenwinkel ein. Die Senktiefe errechnet A+W CAD Designer (Shapes) durch die Durchmesser d1 und d2. Dieses Werkzeug steht Ihnen in der An- sicht Innenkonturen und in maschinenspezifischen Ansichten zur Verfü- gung.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie auf die Fläche, auf der Sie die Senkbohrung anbringen wollen.
3.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   x und y: Position der Bohrung.
    *   d: Kernlochdurchmesser.
    *   d1: Durchmesser der Oberseite der Scheibe.
    *   d2: Durchmesser der Unterseite der Scheibe.
    *   <1 und <2: Flankenwinkel bei d1und d2 der Senkung.

> **Bohrung ohne Senkung eingeben!**
> Wenn Sie für d1 oder d2 den selben Wert wie für d eingeben, dann wird an der entsprechenden Stelle keine Senkung vorgenommen. Ein angeschlos- senes Produktionssystem (z. B. ALCIM) erhält aber in der Stückliste die entsprechende Bearbeitung. Verwenden Sie dieses Werkzeug nur, wenn Sie Senkungen benötigen.

4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Bohrung wird nun in der Scheibe angezeigt.

### Senkbohrung mit Einsenktiefe eingeben

Mit diesem Werkzeug geben Sie eine Senkbohrung mit einem beliebigen Flankenwinkel ein. Die Durchmesser der Senkung errechnet A+W CAD Designer (Shapes) durch die Einsenktiefe t1 und t2. Dieses Werkzeug steht Ihnen in der Ansicht Innenkonturen und in maschinenspezifischen Ansichten zur Verfügung.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie auf die Fläche, auf der Sie die Senkbohrung anbringen wollen.
3.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   x und y: Position der Bohrung.
    *   d: Kernlochdurchmesser.
    *   t1: Einsenktiefe an der Oberseite der Scheibe.
    *   t2: Einsenktiefe an der Unterseite der Scheibe.
    *   <1 und <2: Flankenwinkel bei t1und t2 der Senkung.

> **Bohrung ohne Senkung eingeben!**
> Wenn Sie für t1 oder t2 keinen Wert eingeben, dann wird an der entspre- chenden Stelle keine Senkung vorgenommen. Ein angeschlossenes Pro- duktionssystem (z. B. ALCIM) erhält aber in der Stückliste die entsprechende Bearbeitung. Verwenden Sie dieses Werkzeug nur, wenn Sie Senkungen benötigen.

4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Bohrung wird nun in der Scheibe angezeigt.

### Senkbohrung mit Einsenkdurchmesser und Segmentabständen erfassen

Mit diesem Werkzeug geben Sie eine Senkbohrung mit einem beliebigen Flankenwinkel ein. Die Bohrung vermaßen Sie gegen zwei Segmente. Die Senktiefe errechnet A+W CAD Designer (Shapes) aus den Durchmessern d1 und d2. Dieses Werkzeug steht Ihnen in der Ansicht Innenkonturen und in maschinenspezifischen Ansichten zur Verfügung.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie nacheinander auf die beiden Segmente, gegen die Ihre Boh- rung vermaßt werden soll. A+W CAD Designer (Shapes) zeigt das erste Segment rot, das zweite grün an.
3.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   D1 und D2: Senkrechter Abstand in mm vom ersten zum zweiten mar- kierten Segment.
    *   d: Kernlochdurchmesser.
    *   d1: Durchmesser an der Oberseite der Scheibe.
    *   d2: Durchmesser an der Unterseite der Scheibe.
    *   <1 und <2: Flankenwinkel bei d1und d2 der Senkung.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Bohrung wird nun in der Scheibe angezeigt.

### Senkbohrung mit Einsenktiefe und Segmentabständen erfassen

Mit diesem Werkzeug geben Sie eine Senkbohrung mit einem beliebigen Flankenwinkel ein. Die Bohrung vermaßen Sie gegen zwei Segmente. Die Durchmesser der Senkung errechnet A+W CAD Designer (Shapes) durch die Einsenktiefen t1 und t2. Dieses Werkzeug steht Ihnen in der Ansicht In- nenkonturen und in maschinenspezifischen Ansichten zur Verfügung.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie nacheinander auf die beiden Segmente, gegen die Ihre Boh- rung vermaßt werden soll. A+W CAD Designer (Shapes) zeigt das erste Segment rot, das zweite grün an.
3.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   D1 und D2: Senkrechter Abstand in mm vom ersten zum zweiten mar- kierten Segment.
    *   d: Kernlochdurchmesser.
    *   t1: Einsenktiefe an der Oberseite der Scheibe.
    *   t2: Einsenktiefe an der Unterseite der Scheibe.
    *   <1 und <2: Flankenwinkel bei t1und t2 der Senkung.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Bohrung wird nun in der Scheibe angezeigt.

### Stufenbohrung eingeben

Mit diesem Werkzeug geben Sie eine Stufenbohrung im VSG-Umfeld (VSG-SN-Dateien) ein. Dabei handelt es sich um Bohrungen, die auf den unterschiedlichen Scheiben einer mehrstufigen Einheit unterschiedliche Durchmesser haben. Die sogenannte Sackbohrung ist ein Sonderfall der Stufenbohrung, bei dem die Bohrungsdurchmesser ab einer der Scheiben in der Einheit 0 sind. Sie wird wie eine Stufenbohrung behandelt. Die Boh- rungsdurchmesser auf den ungebohrten Scheiben werden auf 0 gesetzt.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie mit der linken Maustaste an der Stelle, wo Sie den Mittelpunkt des Bohrloches grob positionieren möchten, oder geben Sie im Wertefens- ter in den Feldern x und y die exakten X- und Y-Koordinaten der Position ein. Das Bohrloch wird nun vorläufig hellgrau dargestellt.
3.  Geben Sie im Wertefenster die jeweiligen Durchmesser des Bohrloches an.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Das von Ihnen aus- gewählte Bohrloch wird nun erzeugt und in der Segmentfarbe (normal schwarz) endgültig dargestellt. Der bzw. die Durchmesser des Bohrloches wird als Text angebracht.

### Stufenbohrung mit Lagevermaßung eingeben

Mit diesem Werkzeug geben Sie eine Stufenbohrung und deren Positionie- rung im VSG-Umfeld (VSG-SN-Dateien) ein. Dabei handelt es sich um Bohrungen, die auf den unterschiedlichen Scheiben einer mehrstufigen Einheit unterschiedliche Durchmesser haben. Die sogenannte Sackboh- rung ist ein Sonderfall der Stufenbohrung, bei dem die Bohrungsdurchmes- ser ab einer der Scheiben in der Einheit 0 sind. Sie wird wie eine Stufenbohrung behandelt. Die Bohrungsdurchmesser auf den ungebohr- ten Scheiben werden auf 0 gesetzt.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die beiden Segmente der Form, zu der die Stufenbohrung ausgerichtet werden soll. Es öffnet sich das Wertefenster.
3.  Geben Sie im Wertefenster die gewünschten Abstände D1 und D2 der Stu- fenbohrung zu Segment 1 und 2 an.
4.  Geben Sie für jedes Glas im Aufbau den Durchmesser des Bohrloches an.
5.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Das von Ihnen aus- gewählte Bohrloch wird nun erzeugt und mit den entsprechenden Maßen dargestellt. Der bzw. die Durchmesser des Bohrloches wird als Text ange- bracht.

## Hilfslinien einfügen

Um Hilfslinien einzufügen, stehen Ihnen folgende Funktionen zur Verfügung:

**Tab. A-20 Werkzeuge zum Setzen von Hilfslinien**

| Symbol | Kurzname | Beschreibung |
| :--- | :--- | :--- |
| 41 | CUTCORNR | "Neue Hilfslinie erfassen" auf Seite A-309 |
| D1 D2 | DIMAUXLN | "Hilfslinie zwischen zwei Segmenten mit Abstand zum Segmentende erstellen" auf Seite A-310 |
| | DIMREFLN | "Hilfslinie zwischen zwei Punkten erstellen" auf Seite A-310 |
| | REFLINE | "Referenzlinie für einige Segmente erfassen" auf Seite A-311 |

Erstellen und verwenden Sie Hilfslinien, um Positionen und Winkel zu bestim- men, die mit den vorhanden Segmenten nicht oder nur schwer zu vermaßen sind. Gegen Hilfslinien können Sie dann z. B. Bohrlöcher vermaßen.

### Neue Hilfslinie erfassen

Mit diesem Werkzeug können Sie Hilfslinien eingeben. Sie sind nicht an die Konturpunkte der zu entwerfenden Kontur gebunden. Sie können beliebig viele Hilfslinien einzeln oder auch aneinandergekettet der Zeichnung hin- zufügen. Es ist auch möglich, Hilfslinien in die Kontur mit einzubauen. So erhalten Sie geschlossene Konturen. Sie können z. B. die spätere Kontur an diesen Hilfslinien ausrichten oder Texte daran positionieren.

> **Hilfslinien sind für die Bearbeitung ohne Bedeutung!**
> Die Hilfslinien bleiben bei jedem maschinellen Bearbeitungsvorgang unbe- rücksichtigt.

1.  Positionieren Sie einen neuen Startpunkt an die Stelle, von der aus Sie Ihre Hilfslinie zeichnen möchten.
    Wenn Sie keinen Startpunkt setzen, wird die Hilfslinie vom letzten Punkt aus weiter gezeichnet.
2.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
3.  Erstellen Sie eine Hilfslinie wie eine Gerade:

> **Ergänzende Informationen**
> *   "Neuen Startpunkt erfassen" auf Seite A-236
> *   "Neue Gerade durch Werteeingabe erfassen" auf Seite A-238

### Hilfslinie zwischen zwei Segmenten mit Abstand zum Segmentende erstellen

Verwenden Sie dieses Werkzeug, wenn Sie eine Hilfslinie zwischen zwei Segmenten benötigen, die zu Segmentpunkten einen bekannten Abstand hat.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie nacheinander die Segmente an, zwischen denen die Hilfslinie erstellt werden soll. Klicken Sie dabei in die Nähe des Segmentpunktes, dessen Abstand zur Hilfslinie bekannt ist. A+W CAD Designer (Shapes) zeigt die angeklickten Segmente als rote Pfeile an. Der Pfeil beginnt an dem Segmentpunkt, in dessen Nähe Sie geklickt haben. Vom Pfeilanfang aus wird der Abstand zur Hilfslinie gerechnet.
3.  Geben Sie im Wertefenster die gewünschten Abstände D1 und D2 der Hilfslinie zu Segment 1 und 2 an.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. SA+W CAD Designer (Shapes)N erstellt die Hilfslinie.

### Hilfslinie zwischen zwei Punkten erstellen

Verwenden Sie dieses Werkzeug, wenn Sie eine Hilfslinien zwischen zwei Punkten benötigen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie nacheinander die Punkte an, zwischen denen die Hilfslinie er- stellt werden soll. Klicken Sie dazu auf ein Segment in die Nähe des ge- wünschten Punktes. Den ersten Punkt zeigt A+W CAD Designer (Shapes) rot, den zweiten grün an.
3.  Bestätigen Sie Ihre Auswahl. Betätigen Sie dazu <ENTER> oder [OK]. A+W CAD Designer (Shapes) erstellt die Hilfslinie.

### Referenzlinie für einige Segmente erfassen

Mit diesem Werkzeug können Sie eine an einem Segment oder Segment- zug befestigte Referenzlinie erzeugen. Es wird die Sekante der beteiligten Segmente gebildet und dann bis an den Rand der Kontur nach außen ver- schoben. Gegenüber einer Referenzlinie können alle Vermaßungswerk- zeuge angewandt werden. Wenn sich die Lage der Kontur in nachfolgenden Ansichten ändert, wird die Referenzlinie und daran ange- brachte Vermaßungen mit geändert. Diese Referenzlinie wird bei einem Export von Maschinendaten (z. B. CNC) nicht exportiert, sondern stellt le- diglich eine Hilfslinie in der Konstruktion und Vermaßung dar.

Praktisch ist eine Referenzlinie vor allem dann, wenn Sie unregelmäßige Konturen so behandeln wollen, als ob es Dreiecke oder Trapeze wären. Die gewünschten Seiten konstruieren Sie dann aus den Kontursegmenten mit Hilfe von Referenzlinie.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Ein Segment auf der Kontur auswählen. Dieses färbt sich danach rot ein.
3.  Wählen Sie weitere Segmente aus. Diese färben sich ebenfalls rot ein. Sie können nur Segmente auswählen, die an dem zuvor gewählten direkt an- grenzen.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Danach wird das Be- rechnungsverfahren gestartet, die Referenzlinie berechnet und als gestri- chelte Linie (Hilfslinie) auf der Zeichenfläche dargestellt.

**Beispiel:**

*   A Selektion der Segmente
*   B Erzeugte Referenzlinie

*Abb. A-194 Segment Kennlinie*

## Werkzeuge zur Eckenbearbeitung

Für den Zuschnitt ist es vorteilhaft, wenn große Schnitte und keine oder nur große Radien gefahren werden müssen.

### Radien und Fasen

Kleine Radien oder Fasen an den Ecken einer Scheibe können zugeschnitten oder nachträglich geschliffen werden. Nachträglich angebrachte Radien und Fasen werden als kaufmännische Radien und Fasen bezeichnet. Diese Werk- zeuge stehen ab der Ansicht Geometrie zur Verfügung.

### Zuspitzen

In manchen Fällen (z. B. zur Modellekenung) ist es sinnvoll, Ecken zuzuspit- zen. Wenn z. B. eine digitalisierte oder importierte Kontur bereits Rundungen oder Fasen an den Ecken hat, werden diese Ecken für den Zuschnitt zuge- spitzt benötigt. Auch dafür stellt A+W CAD Designer (Shapes) geeignete Werkzeuge zur Verfügung.

### Ecke abschneiden

Um Ecken abzuschneiden, stehen Ihnen folgende Funktionen zur Verfügung:

**Tab. A-21 Werkzeuge zum Abschneiden von Ecken**

| Symbol | Kurzname | Beschreibung |
| :--- | :--- | :--- |
| D | CUTCORNR | "Ecke abschneiden" auf Seite A-313 |
| D2 D1 | CUTCRNR2 | "Ecke mit verschiedenen Abständen abschneiden" auf Seite A-314 |
| D D | CUTEDGE | "Ecke durch Auswahl von zwei Segmenten abschnei- den" auf Seite A-314 |
| D2 D1 | CUTEDG2 | "Ecke mit verschiedenen Abständen durch Auswahl von zwei Segmenten abschneiden" auf Seite A-315 |
| | CUTCRNRW | "Ecke mit senkrechtem Abstand abschneiden" auf Seite A-316 |
| | CUTEDGW | "Ecke mit senkrechtem Abstand durch Auswahl von zwei Segmenten abschneiden" auf Seite A-317 |
| | CUTCUR90 | "Ecke auf beliebigen Winkel abschneiden" auf Seite A-317 |
| | CHAMEDGE | "Ecke durch Eckabschnitt ersetzen" auf Seite A-318 |
| | WCHAM | "Symmetrischen Eckabschnitt als Stücklistenelement einfügen" auf Seite A-318 |
| | ASYMCHAM | "Asymmetrischen Eckabschnitt als Stücklistenele- ment einfügen" auf Seite A-319 |

### Ecke abschneiden

Mit diesem Werkzeug können Sie Ecken nachträglich abschneiden. Sie können also eine Kontur überwiegend aus Geradensegmenten erstellen, diese vermaßen und dann die Ecken abschneiden.

Ebenso notwendig ist dieses Werkzeug bei kleinen Ecken, die aufgrund der Glasart oder Glasstärke nicht geschnitten bzw. gebrochen werden kön- nen oder sollen und demzufolge auf dieses Maß geschliffen werden müs- sen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Wählen Sie den abzurundenden Eckpunkt aus. Dieser färbt sich rot.
3.  Geben Sie im Wertefenster den Abstand D ein, um den jedes angrenzende Segment gekürzt werden soll.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Ecke wird abge- schnitten und gestrichelt dargestellt.

**Beispiel:**

*Abb. A-195 Ecke abschneiden*

Diese Ecke existiert nur beim Skizzieren und Vermaßen der Länge.

### Ecke mit verschiedenen Abständen abschneiden

Mit diesem Werkzeug können Sie Ecken nachträglich abschneiden. Sie können eine Kontur aus Geradensegmenten erstellen, diese vermaßen und dann die Ecken abschneiden.

Hilfreich ist dieses Werkzeug bei kleinen Rundecken, die aufgrund der Glasart oder der Glasstärke nicht geschnitten bzw. gebrochen werden kön- nen oder sollen. Solche Rundecken werden geschliffen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Wählen Sie den abzuschneidenden Eckpunkt aus. Dieser färbt sich rot.
3.  Geben Sie im Wertefenster die Abstände D1 und D2 ein, um die die an- grenzenden Segmente gekürzt werden sollen.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Ecke wird abge- schnitten und gestrichelt dargestellt.

### Ecke durch Auswahl von zwei Segmenten abschneiden

Mit diesem Werkzeug können Sie an eine Ecke eine Fase anbringen. Nach der Anwahl von zwei Segmenten geben Sie einen Abstand ein. Dieser Ab- stand bezieht sich auf beide gewählte Segmente (oder ihre Verlängerung zur gebildeten Ecke).

Im Gegensatz zum Werkzeug Ecke abschneiden können Sie über mehrere Segmente hinweg arbeiten.

Wenn dieses Werkzeug an zwei Segmenten angewendet wird, die über ein drittes oder viertes Segment miteinander verbunden sind, so werden diese dazwischenliegenden Segmente gelöscht und die selektierten Segmente werden soweit verlängert, bis der vorgegebene Abschnitt angesetzt wer- den kann.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die beiden Segmente in der Nähe des Eckpunktes. Die Seg- mente werden als Pfeile dargestellt.
3.  Geben Sie im Wertefenster den Abstand D ein. Der Abstand bezieht sich auf die von den beiden gewählten Segmenten (oder ihrer Verlängerung) gebildeten Ecke.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die beiden Segmen- te werden entsprechend gekürzt und durch ein weiteres Segment (Fase) miteinander verbunden.

**Beispiel:**

*Abb. A-196 Ecke abschneiden (Fase)*

D: Abstand, um den die Segmente gekürzt werden.

> **Kontur sichtbar machen!**
> Wenn Sie nach der Bearbeitung eines der beteiligten Segmente auswäh- len, wird die ursprüngliche Kontur sichtbar.

> **Ergänzende Informationen**
> "Ecke abschneiden" auf Seite A-313

### Ecke mit verschiedenen Abständen durch Auswahl von zwei Segmenten abschneiden

Mit diesem Werkzeug können Sie Ecken nachträglich abschneiden. Sie können eine Kontur aus Geradensegmenten erstellen, diese vermaßen und dann die Ecken abschneiden.

Im Gegensatz zum Werkzeug Ecke mit verschiedenen Abständen ab- schneiden können Sie über mehrere Segmente hinweg arbeiten.

Wenn dieses Werkzeug an zwei Segmenten angewendet wird, die über ein drittes oder viertes Segment miteinander verbunden sind, so werden diese dazwischenliegenden Segmente gelöscht und die selektierten Segmente werden soweit verlängert, bis der vorgegebene Abschnitt angesetzt wer- den kann.

Hilfreich ist dieses Werkzeug bei kleinen Rundecken, die aufgrund der Glasart oder der Glasstärke nicht geschnitten bzw. gebrochen werden kön- nen oder sollen. Solche Rundecken werden geschliffen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die beiden Segmente, an denen die Ecke abgeschnitten werden soll. Klicken Sie dazu die Segmente in der Hälfte an, in deren Rich- tung die Ecke abgeschnitten werden soll. Diese färben sich rot und die Pfeile zeigen zur Ecke, die abgeschnitten werden soll.
3.  Geben Sie im Wertefenster die Abstände D1 und D2 ein. Um die angege- benen Werte werden die Segmente gekürzt.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Ecke wird abge- schnitten und gestrichelt dargestellt.

> **Ergänzende Informationen**
> "Ecke mit verschiedenen Abständen abschneiden" auf Seite A-314

### Ecke mit senkrechtem Abstand abschneiden

Mit diesem Werkzeug können Sie Ecken nachträglich abschneiden, indem Sie einen senkrechten Abstand zur gewünschten Ecke eingeben. Sie kön- nen eine Ecke aus Geradensegmenten erstellen, diese vermaßen und dann die Ecken abschneiden.

Hilfreich ist dieses Werkzeug bei kleinen Rundecken, die aufgrund der Glasart oder der Glasstärke nicht geschnitten bzw. gebrochen werden kön- nen oder sollen. Solche Rundecken werden geschliffen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie den abzuschneidenden Eckpunkt. Dieser färbt sich rot.
3.  Geben Sie im Wertefenster den senkrechten Abstand D ein, den die Ecke zur abgeschnittenen Kante haben soll.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Ecke wird abge- schnitten und gestrichelt dargestellt.

### Ecke mit senkrechtem Abstand durch Auswahl von zwei Segmenten abschneiden

Mit diesem Werkzeug können Sie Ecken nachträglich abschneiden, indem Sie einen senkrechten Abstand zu den Segmenten eingeben. Sie können eine Ecke aus Geradensegmenten erstellen, diese vermaßen und an- schließend die Ecke abschneiden.

Hilfreich ist dieses Werkzeug bei kleinen Rundecken, die aufgrund der Glasart oder der Glasstärke nicht geschnitten bzw. gebrochen werden kön- nen oder sollen. Solche Rundecken werden geschliffen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die beiden Segmente, zwischen denen die Ecke als gleich- schenkliges Dreieck abgeschnitten werden soll. Klicken Sie dazu die Seg- mente in der Hälfte an, in deren Richtung die Ecke abgeschnitten werden soll. Die Segmente färben sich rot und zeigen als Pfeile auf die Ecke.
3.  Geben Sie im Wertefenster den senkrechten Abstand D ein, um den die Segmente gekürzt werden sollen.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Ecke wird abge- schnitten und gestrichelt dargestellt.

### Ecke auf beliebigen Winkel abschneiden

Mit diesem Werkzeug können Sie Ecken nachträglich abschneiden. Sie können eine Kontur aus Geradensegmenten erstellen, diese vermaßen und anschließend die Ecken abschneiden.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie das Segment, dessen Ecke gekürzt und mit einem Win- kel versehen werden soll. Das Segment färbt sich rot.
3.  Geben Sie im Wertefenster den Abstand D zur Ecke und den Winkel <1 ein.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Das markierte Seg- ment wird um den eingegebenen Wert gekürzt. Am neuen Ende des Seg- mentes wird im angegebenen Winkel eine Gerade zum zweiten Segment der Ecke gelegt.

### Ecke durch Eckabschnitt ersetzen

Das Werkzeug dient zum Entfernen von Eckausschnitten. Mit ihm können Sie einen Eckausschnitt durch ein Geradensegment ersetzen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie das Segment, wo die Gerade beginnen soll. Das Seg- ment färbt sich rot mit einer Pfeilspitze, die in Richung Ecke zeigt.
3.  Markieren Sie das Segment, wo die Gerade enden soll. Das Segment färbt sich rot mit einer Pfeilspitze, die in Richung Ecke zeigt.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Segmentkette zwischen den Spitzen der Selektionspfeile wird durch ein Geradensegment ersetzt.

### Symmetrischen Eckabschnitt als Stücklistenelement einfügen

Mit diesem Werkzeug fügen Sie einen symmetrischen Eckabschnitt ein, bei dem die Ecke in den Geometriedaten erhalten bleibt. Verwenden Sie dieses Werkzeug, wenn z. B. die automatische Modellerkennung das Mo- dell noch erkennen soll, die Ecke aber später abgeschnitten (gefast) wird.

Diesen Eckabschnitt kann A+W CAD Designer (Shapes) als Artikel der Stückliste (als Bearbeitung) an eine angeschlossene Auftragsbearbeitung geben.

Dieses Werkzeug steht Ihnen in der Ansicht Kantenbearbeitung zur Verfü- gung.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie auf den Eckpunkt, der abgeschnitten werden soll. A+W CAD Designer (Shapes) zeigt den Punkt rot an.
3.  Geben Sie im Wertefenster an, um wieviel mm beide an die Ecke angren- zenden Segmente gekürzt werden sollen.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) zeigt zunächst nur das Symbol # in der betroffenen Ecke an. Wenn Sie in die Ansicht Endprodukt wechseln, dann zeigt A+W CAD Designer (Shapes) die Ecke abgeschnitten an.

### Asymmetrischen Eckabschnitt als Stücklistenelement einfügen

Mit diesem Werkzeug fügen Sie einen asymmetrischen Eckabschnitt ein, bei dem die Ecke in den Geometriedaten erhalten bleibt. Verwenden Sie dieses Werkzeug, wenn z. B. die automatische Modellerkennung das Mo- dell noch erkennen soll, die Ecke aber später gefast (abgeschnitten) wird.

Diesen Eckabschnitt kann A+W CAD Designer (Shapes) als Artikel der Stückliste (als Bearbeitung) an eine angeschlossene Auftragsbearbeitung zurückgeben.

Dieses Werkzeug steht Ihnen in der Ansicht Kantenbearbeitung zur Verfü- gung.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie auf das erste Segment in die Nähe der Ecke, die abgeschnitten werden soll. A+W CAD Designer (Shapes) zeigt das Segment rot an.
3.  Klicken Sie auf das zweite Segment in die Nähe der Ecke, die abgeschnit- ten werden soll. A+W CAD Designer (Shapes) zeigt das Segment grün an.
4.  Geben Sie im Wertefenster bei D1 an, um wieviel mm das erste (rote) Seg- ment von der Ecke aus gekürzt werden soll.
5.  Geben Sie im Wertefenster bei D2 an, um wieviel mm das zweite (grüne) Segment von der Ecke aus gekürzt werden soll.
6.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) zeigt zunächst nur das Symbol # in der betroffenen Ecke an. Wenn Sie in die Ansicht Endprodukt wechseln, dann zeigt A+W CAD Designer (Shapes) die Ecke abgeschnitten an.

## Ecken runden oder zuspitzen

Zum Runden oder Zuspitzen von Ecken stehen Ihnen folgende Werkzeuge zur Verfügung:

**Tab. A-22 Werkzeuge zum Runden und Zuspitzen von Ecken**

| Symbol | Kurzname | Beschreibung |
| :--- | :--- | :--- |
| | RNDCORNER | "Ecke runden" auf Seite A-320 |
| | ROUNDEDGE | "Zwischen zwei Segmenten abrunden oder zuspit- zen" auf Seite A-321 |
| | RNDALL | "Alle Ecken der Kontur mit einem einheitlichen Radi- us versehen" auf Seite A-322 |
| | SHRPCRNR | "Ecke zuspitzen" auf Seite A-322 |
| | DESIGNC | "Ecke durch Zugabe oder Abnahme bei Segmenten modellieren" auf Seite A-323 |
| | WRND | "Rundecke als Stücklistenelement einfügen" auf Seite A-325 |

### Ecke runden

Mit diesem Werkzeug können Sie zwei Segmente, die eine Ecke bilden, über einen beidseitig tangential angelegten Bogen verbinden (mit einem Radius versehen). Wenn Sie im Wertefenster keinen Radius eingeben, dann verlängert A+W CAD Designer (Shapes) die beiden Segmente und spitzt die Ecke zu.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die Ecke einer Kontur, die gerundet werden soll.
3.  Geben Sie den Radius des Bogens im Wertefenster ein.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

### Zwischen zwei Segmenten abrunden oder zuspitzen

Mit diesem Werkzeug können Sie zwei beliebige Segmente über einen beidseitig tangential angelegten Bogen verbinden. Der Radius wird von Ih- nen im Wertefenster erfragt. Wenn Sie keinen Radius eingeben, d. h. das Eingabefeld bleibt leer, dann verlängert A+W CAD Designer (Shapes) die beiden markierten Segmente und spitzt die Ecke zu.

Im Gegensatz zum Werkzeug Ecke runden können Sie hier über mehrere Segmente hinweg arbeiten.

Wenn dieses Werkzeug auf zwei angrenzende Segmente angewendet wird, dann kann man von einer Eckenrundung sprechen. Wenn dieses Werkzeug an zwei Segmenten angewendet wird, die über ein drittes oder viertes Segment miteinander verbunden sind, so werden diese dazwi- schenliegenden Segmente gelöscht und die selektierten Segmente wer- den soweit verlängert, bis die vorgegebene Rundung tangential angesetzt werden kann.

**Beispiel:**

*A zu verbindende SegmenteB Resultat*
*Abb. A-197 Abrundung zwischen 2 Segmenten, die über weitere Segmente ver- bunden sind*

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Wählen Sie die beiden Segmente aus, zwischen denen die Eckenrundung erfolgen soll. Klicken Sie dazu die Segmente in der Hälfte an, in deren Richtung die Ecke abgeschnitten werden soll. Die Segmente färben sich rot und zeigen als Pfeile auf die Ecke.
3.  Geben Sie den Radius des Bogens im Wertefenster ein.

> **Segmente durch optimalen Radius ersetzen!**
> Wenn Sie mit einem Radius mehrere Segmente ersetzen wollen, aber im Wertefenster keinen Radius vorgeben (das Feld leer lassen), dann errech- net A+W CAD Designer (Shapes) einen Radius, der sich an die zu erset- zenden Punkte optimal annähert. Damit können Sie z. B. eine beschädigte Rundecke wieder herstellen.

4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

> **Ergänzende Informationen**
> "Ecke runden" auf Seite A-320

### Alle Ecken der Kontur mit einem einheitlichen Radius versehen

Verwenden Sie dieses Werkzeug, wenn Sie alle Ecken einer Kontur mit dem selben Radius abrunden wollen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie auf ein Segment der Kontur.
3.  Geben Sie im Wertefenster den Radius ein, den die Ecken erhalten sollen.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) rundet alle Ecken (Innen- und Außenecken) der Kontur mit dem angegebenen Radius ab.

### Ecke zuspitzen

Verwenden Sie dieses Werkzeug, um z. B. im Zuschnitt (Ansicht Schnei- den) kleine Radien als Ecken zuzuschneiden und erst bei einer späteren Bearbeitung abzurunden.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die beiden Segmente, zwischen denen die Zuspitzung erfol- gen soll. Klicken Sie dazu die Segmente in der Hälfte an, in deren Richtung zugespitzt werden soll. Die Segmente färben sich rot und zeigen als Pfeile auf die Ecke.
3.  Geben Sie im Wertefenster ein, wie weit nach dem Segmentende die ur- sprüngliche Kontur noch erhalten bleiben soll, bevor das neue Ecksegment tangential beginnen und eine Ecke bilden soll. Geben Sie jeweils einen Wert für den Abstand vom ersten und vom zweiten gewählten Segment an.
    Wenn Sie jeweils 0 eingeben, dann schließt A+W CAD Designer (Shapes) die Ecke direkt an das Ende der markierten Segmente an.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) zeigt die Kontur mit Ecke an.

### Ecke durch Zugabe oder Abnahme bei Segmenten modellieren

Mit diesem Werkzeug können Sie Ecken und Bögen verändern. Sie kön- nen Ecken vergrößern (herausziehen) oder stutzen. Besonders nützlich ist diese Funktion beim Modellieren von digitalisierten Konturen oder abgewi- ckelten 3D-Zeichnungen im Autoglasbereich. Dieses Werkzeug beinhaltet ein Glättungsverfahren, so dass, je nach Notwendigkeit, automatisch Kon- turpunkte hinzugefügt werden oder wegfallen (d. h., die Anzahl der Seg- mente kann sich verändern).

Dieses Werkzeug verschiebt den Teil der Kontur, der zwischen den mar- kierten Segmenten liegt, um den eingegebenen Wert. Damit wird ein Punkt oder ein (kleiner) Konturteil nach außen oder innen (parallel) verschoben. Die markierten Segmentzüge links und rechts von diesem Bereich werden für einen sanften An- und Abstieg zu diesem Bereich genutzt. Je länger diese markierten Segmentzüge sind, desto sanfter (knickfreier) ist der An- und Abstieg.

Wenn Sie nach Anwendung dieses Werkzeuges ein an der Glättung betei- ligtes Segment auswählen, werden alle an der Glättung beteiligten Seg- mente und die alte Konturform angezeigt. Im Wertefenster sehen Sie die Abweichung der neuen Kurvenform, die Sie auch noch nachträglich ändern können.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Wählen Sie das erste Segment in der Segmenthälfte an, in deren Richtung die Ecke liegt. Nach dem Anklicken des Segmentes wird dieses mit einem Pfeil markiert, der zur Ecke zeigen.
3.  Wählen Sie mindestens ein weiteres Segment aus. Sie benötigen mindes- tens zwei Markierungspfeile, die zueinander zeigen, um den zu modellie- renden Bereich zu bestimmen. Einen besseren Übergang erreichen Sie, wenn Sie alle Segmente markieren, die in den zu modellierenden Bereich fallen.

**Beispiel:**

*Abb. A-198 Modellierte Segmente*

*   A ausgewähltes Segment
*   B an der Änderung beteiligte Segmente
*   C alter Bogen
*   D Modellierung 1
*   E Modellierung 2

*   **Modellierung 1**
    In diesem Fall wird die Verschiebung nach außen nur an den beiden markierten Segmenten durchgeführt. d. h., die gesamte Ecke inklusive den markierten Segmenten wird an der Spitze um den von Ihnen einge- gebenen Wert nach außen oder innen (negativer Wert) verschoben, der Ausgleich findet dabei nur an den markierten Segmenten statt.
*   **Modellierung 2**
    In diesem Fall wird die Rundung um den von Ihnen eingegebenen Wert nach außen oder innen verschoben und die Verschiebung über alle markierten Segmente ausgeglichen.

4.  Geben Sie im Wertefenster den Wert D für die Streckung oder Kürzung der Ecke ein, sobald Sie zwei zueinander zeigende Markierungspfeile festge- legt haben. Positive Werteingaben bedeuten Vergrößerungen, negative Werteingaben haben Eckenverschiebungen nach innen zur Folge.
5.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Kontur wird nun neu berechnet und gezeichnet.

> **Segmente vor dem Modellieren teilen**
> Bei Ecken, die aus sehr wenigen Segmenten bestehen, kann es notwendig sein, vor dem Modellieren ein oder zwei Segmente zu splitten, d. h., ein Segment in mehrere Segmente aufzuteilen, indem Sie nachträglich zu- sätzliche Konturpunkte hinzufügen, bzw. einfügen.

> **Ergänzende Informationen**
> "Segment in zwei Segmente teilen" auf Seite A-246

### Rundecke als Stücklistenelement einfügen

Mit diesem Werkzeug bestimmen Sie eine zu produzierende Rundecke (z. B. gemäß der Skizze Ihres Kunden). Die Rundkante wird zunächst als kleiner Kreis dargestellt und dann in den Technologie-Ansichten (Schnei- den, Schleifen, ...) entsprechend gerundet gezeichnet. Mit den Rundungs- daten wird die Kontur an die Fertigungsmaschinen übertragen.

Diesen Eckabschnitt kann A+W CAD Designer (Shapes) als Artikel der Stückliste (als Bearbeitung) an eine angeschlossene Auftragsbearbeitung zurückgeben.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die Ecke einer Kontur, die eine die Rundecke erhalten soll. Die Ecke färbt sich rot.
3.  Geben Sie im Wertefenster den Radius r für die Rundung ein.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

## Werkzeuge zur Bearbeitung von Innenkonturen

Ausschnitte und Bohrungen sind Innenkonturen und werden daher meist in der entsprechenden Ansicht eingefügt. Je nach Größe und Vorlage können Ausschnitte und Bohrungen aber auch schon bei der Digitalisierung von Mo- dellen oder bei der Erstellung einer Skizze erfasst werden.

### Ausschnitte als eigene Datei

Sie können mit A+W CAD Designer (Shapes) einfache (Rechtecke und Bö- gen) oder komplexe Ausschnitte an Scheiben anbringen. Komplexe Aus- schnitte können Sie zuvor als eigene Geometrie zeichnen und als Datei speichern oder in einer aktuellen Datei erstellen. Wenn Sie die Ausschnitte in einer eigenen Datei speichern, dann können Sie diese Ausschnitte immer wie- der verwenden. Die Geometrien für Ausschnitte können Sie in gleicher Weise wie eine normale Außengeometrie (es muss eine geschlossene Kontur sein) erstellen. Die Ausschnitte, die Sie in einer eigenen Datei gespeichert haben, können Sie in die entsprechende SN-Datei laden.

### Ausschnitte und Bohrungen zuschneiden

Innenkonturen (Ausschnitte und Bohrungen) und Randausschnitte werden nur dann geschnitten, wenn diese auch in der Ansicht Schneiden zu sehen sind. In der Regel werden A+W CAD Designer (Shapes)-Arbeitsplätze (je nach Absprache mit dem Kunden) so konfiguriert, dass Innenkonturenen in der Ansicht Schneiden ausgeblendet werden. Sie haben jedoch die Möglich- keit, die Innenkonturen in der Ansicht Schneiden einzublenden. Randaus- schnitte können über diesen Weg nicht automatisch ausgeblendet werden. Sie können diese Randausschnitte jedoch manuell entfernen.

### Ausschnittmakros

Ein Ausschnittmakro ist eine Datei, die eine Gruppe von Ausschnitten und Bohrungen enthält. Diese Bearbeitungen sind z. B. notwendig, um einen be- stimmten Beschlag am Glas zu befestigen. Typischerweise handelt es sich um einen Ausschnitt, evtl. mit einer oder mehreren Bohrungen. Es können auch nur Bohrungen vorliegen. Diese Datei kann später in andere Dateien (die z. B. eine Glastür beschreiben) eingefügt werden (auch mehrfach). Wird das Makro über das SN-API eingefügt (z. B. durch das A+W Business) so müssen die Bearbeitungen zwingend gruppiert und mit einem Referenzpunkt versehen werden. Beim Einfügen wird dann gegen diesen Referenzpunkt vermaßt.

Die folgenden Schritte sind zum Erstellen eines Ausschnittmakros notwendig:

*   Erzeugung der Formen und Bohrungen
*   Gruppieren und Erzeugen des Referenzpunktes

### Erzeugung der Formen und Bohrungen

Die Formen werden entweder aus DXF-Daten übernommen, die z. B. vom Be- schlaghersteller angeboten werden. Falls solche Daten nicht verfügbar sind, sind die Ausschnitte in der Ansicht Skizze zu zeichnen. Häufig (bei Randaus- schnitten) handelt es sich um symmetrische Ausschnitte. Hier ist es von Vorteil nur eine Hälfte zu zeichnen und in der Ansicht Geometrie die Form aufzuklap- pen. Die Bohrungen sollten in der Ansicht Innenkonturen hinzugefügt und ver- maßt werden.

### Gruppieren und Erzeugen des Referenzpunktes

Durch das Gruppieren werden die Ausschnitte und Bohrungen zu einer Ein- heit zusammen gefasst, die sich durch eine Operation an einer Außengeome- trie anbringen lässt. Desweiteren ändern bei Verschiebungen und Drehungen alle Teile ihre Positionen synchron, d. h. ihre gegenseitigen Lagebeziehungen bleiben in jeden Fall erhalten.

Das Gruppieren sollte in der Ansicht Innenkonturen vorgenommen werden. Mit dem Maus werden alle Bohrlöcher und jeweils ein Segment des Aus- schnitts (falls vorhanden) markiert.

Dann wird über das Menü Transformieren > Gruppieren ausgewählt. Es er- scheint ein Wertefenster, in dem weitere Optionen angegeben werden kön- nen. Das betrifft die Ränder des Gruppierungsrechtecks, und die Lage des Referenzpunktes.

Der Referenzpunkt ist (erst einmal) ein Eckpunkt des Gruppierungsrechtecks. Beim Einfügen über das A+W Business wird dieser Punkt auf eine Kante der Außengeometrie gelegt. Zusätzlich wird ein weiterer Abstand zu einem End- punkt dieses Segmentes angegeben. Damit ist Lage des Referenzpunktes beim Einfügen eindeutig bestimmt. Dann wird evtl. das Gruppierungsrechteck so gedreht, dass die Kante, an der der Referenzpunkt liegt, mit der Außenkan- te zusammenfällt. Falls dann das Gruppierungsrechteck außerhalb der Glas- kontur liegt, wird es zusätzlich noch gespiegelt. Dadurch muss für Bearbeitungen, die in zwei gespiegelten Varianten vorliegen können, nur ein Makro erstellt werden.

Beim Gruppieren ist also folgendermaßen vorzugehen:
Wählen Sie eine Kante des Gruppierungsrechtecks, an der die Bearbeitungen an der Außenkante angebracht werden. (...) . Einer der beiden Eckpunkte wird als Referenzpunkt ausgewählt. Der Abstand des Gruppierungsrechtecks an dieser Kante wird so gewählt, dass Bearbeitungen beim Einfügen richtig lie- gen: bei einem Ausschnitt wird der Rand daher i. a. die Breite 0 haben. Falls das Makro nur Bohrungen enthält, ist der Rand der Abstand der Bohrlöcher von der Außengeometrie (also Abstand der Bohrlochzentren von der Außen- geometrie minus Bohrradius).

### Rundungen an ein Makro anbringen

Mit diesem Werkzeug kann an einem Makro ein Radius angegeben werden, um Ecken zu runden. Dies ist beispielsweise erforderlich, um eingehende oder ausgehende Rundungen (Glaskante -> Makro-Ausschnitt -> Glaskante) zu definieren. Wird das Makro dann im ERP-System an der entsprechenden Glaskante / Glasecke platziert, so werden die Ecken des Makros entspre- chend der Angaben im A+W CAD Designer (Shapes) gerundet.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die erste Ecke der Kontur, die eine Rundecke erhalten soll. Die Ecke färbt sich rot.
3.  Geben Sie im Wertefenster den Radius r für die Rundung ein.
4.  Markieren Sie die zweite Ecke der Kontur, die eine Rundecke erhalten soll. Die Ecke färbt sich ebenfalls rot.
5.  Geben Sie im Wertefenster den Radius r für die Rundung ein.
6.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) zeigt das Symbol # in der betroffenen Ecke an.
7.  Die Strecke zwischen der ersten und der zweiten Ecke der Kontur läuft pa- rallel zur Außenkontur der Scheibe.

> **Erst runden dann gruppieren**
> Wir empfehlen, die Ecken erst zu runden und dann die Kontur zu gruppie- ren.

> **Bei Kanten-Makros und Eck-Makros immer verwenden**
> Wir empfehlen dieses Werkzeug bei Eck- und Kantenmakros immer zu ver- wenden und ggf. den Rundungsradius auf 0 zu setzen.
> Durch die Verwendung des Werkzeugs ist klar definiert, wo später das Ma- kro an der Glaskante platziert werden soll bzw. kann. Dies hilft bei genauen Auswahl von notwendigen und nicht notwendigen Maßangaben, welche im ERP-System angezeigt werden sollen (SN-Live Anzeige).
>
> "Maßangaben löschen" auf Seite A-330

### Maßangaben löschen

Dieses Werkzeug dient dazu, Maßangaben gezielt zu löschen. Typischerwei- se werden in der Zeichnungs-Darstellung nur die wichtigen Maße angezeigt und an SN Live übergeben. Doch auch diese Angaben können schon zu viel sein. Mit diesem Werkzeug wird vermieden, dass SN Live beim Platzieren ei- nes Makros zu viele Vermaßungen anzeigt. D. h., die Angaben werden aus- geblendet und nicht an SN Live übergeben.

1.  Wechseln Sie in die Ansicht Endprodukt und wählen Sie die Darstellung Zeichnung.
2.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol. Es werden jetzt alle Maße eingeblendet, welche tatsächlich in SN Live, auf Ausdrucken oder in der grafischen Anzeige der A+W Production Terminals angezeigt werden.
3.  Klicken Sie die Maßangabe an, die gelöscht werden soll. Diese färbt sich rot.
4.  Drücken Sie die <Entf>-Taste. Die Maßangabe wird gelöscht.
5.  Wiederholen Sie diesen Schritt, bis alle nicht gewünschten Maßangaben gelöscht sind.

### Form löschen

Mit diesem Werkzeug können Sie eine Kontur vollständig löschen. Das Werk- zeug löscht alle Segmente. Bei parametrischen Formen mit variabler Seg- mentzahl stellt die Verwendung dieses Werkzeugs sicher, dass immer alle Segmente gelöscht werden.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie ein Segment der zu löschenden Kontur. Das Segment färbt sich rot.
3.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Kontur, zu der das Segment gehört, wird vollständig gelöscht.

## Segment symmetrisch teilen

### Symmetrische Makros gruppieren

Randausschnitte sind häufig symmetrisch und werden bzgl. ihrer Symmetrie- linien vermaßt. Dabei wird folgendermaßen vorgegangen: Die Gruppierung wird erzeugt wie oben beschrieben. Nun gibt es zusätzlich die Möglichkeit, ein Segment des Gruppierungsrechtecks zu halbieren und die Referenz auf die- sen Punkt zu setzten. Dazu wird das Werkzeug SPLITSYM verwendet.

Nach Auswahl des Werkzeugs wird das entsprechende Segment des Grup- pierungsrechtecks selektiert und mit [OK] bestätigt. Danach ist das Segment in zwei gleich lange Teile zerlegt.

Mit dem Werkzeug PLACEREF lässt sich nun einer der beiden Teile als Refe- renzsegment auswählen.

Der Endpunkt, in dessen Nähe geklickt wurde, wird dabei der Referenzpunkt.

Rein technisch kann diese Datei nun über das SN-API eingefügt werden. Für einen ansprechenden Skizzendruck in der Ansicht Endprodukt ist das Hinzu- fügen einer Symmetrielinie sinnvoll. Auf diese Linien können sich dann die Vermaßungen, die beim Einfügen entstehen, beziehen. Dazu splittet man nicht nur die eine Seite des Gruppierungsrechtecks, sonder auch die gegen- überliegende. Dann verwendet man das Tool DIMREFLN, um zwischen den beiden neu entstandenen Endpunkten eine Hilfslinie zu erzeugen.

Beim Einfügen werden die Vermaßungen dann später auf diese Hilfslinie be- zogen.

Es sollte dann in der SN.ini die Einstellung ShowTARGETPRODUCTAtta- chedSegments = 1 gewählt werden, so dass die Hilfslinie und damit auch die Vermaßung in der Ansicht Endprodukt sichtbar sind. Hinweis: Zur Vereinfa- chung der Selektion kann es sinnvoll sein, den Rand des Gruppierungsrecht- ecks erst ungleich Null zu wählen. Dann werden die Manipulationen vorgenommen, später wird der Rand zurück gesetzt.

## Ausschnitte anbringen

Die Werkzeuge zum Anbringen von Ausschnitten gibt es in zwei Varianten:

*   Mit der einen Variante wird der Ausschnitt lediglich an die entsprechende Stelle gelegt. Damit kann der Ausschnitt als Stücklistenelement gehand- habt werden. Ein zu Grunde liegendes Modell wird in seiner Modellgeome- trie nicht verändert, das Modell kann erkannt werden, auch wenn es zusätzliche Ausschnitte enthält.
*   Mit der anderen Variante wird der Ausschnitt mit der Kontur verschmolzen. Die automatische Modellerkennung würde scheitern.

Die Werkzeuge zur Bearbeitung von Ausschnitten stehen üblicherweise in der Ansicht Innenkonturen zur Verfügung. Folgende Werkzeuge stehen zur Verfü- gung:

**Tab. A-23 Werkzeuge zur Bearbeitung der Oberfläche**

| Symbol | Kurzname | Beschreibung |
| :--- | :--- | :--- |
| | PLACEREC | "Komplexe Ausschnitte positionieren" auf Seite A-335 |
| | PLACEGRP | "Gruppierung positionieren" auf Seite A-336 |
| 1/2 | SPLITSYM | "Segment halbieren" auf Seite A-337 |
| | PLACEREF | "Referenzsegment zum Einfügen von Ausschnitten setzen" auf Seite A-337 |
| | MELTCUTO | "Konturen verschmelzen" auf Seite A-338 |
| | BOCUTPRO | "Rechteckigen Randausschnitt als Stücklistenele- ment anbringen" auf Seite A-338 |
| | BOCUTOUT | "Randausschnitt anbringen und mit Kontur ver- schmelzen" auf Seite A-339 |
| 2 | JOINEDGE | "Randausschnitt entfernen und Form schließen" auf Seite A-339 |
| d2 | COCUTPRO | "Eckausschnitt als Stücklistenelement anbringen" auf Seite A-340 |
| | COCUTOUT | "Eckausschnitt anbringen und mit Kontur verschmel- zen" auf Seite A-341 |
| | ARCUTPRO | "Bogenförmigen Randausschnitt als Stücklistenele- ment anbringen" auf Seite A-342 |
| | ARCUTOUT | "Bogenförmigen Randausschnitt anbringen und mit Kontur verschmelzen" auf Seite A-343 |

Über den Schalter ShowProfileCutout = 1 werden Ausschnitte auch im Profil dargestellt.

### Komplexe Ausschnitte positionieren

Komplexe Ausschnitte, die aus mehreren Geraden und Kreisbögen beste- hen (z. B. für Pendeltürbeschläge), können Sie als eigene SN-Dateien er- stellen und später einfügen und ausrichten.

Mit diesem Werkzeug positionieren Sie einen Ausschnitt im benötigten Ab- stand an der richtigen Kante und in der benötigten Ausrichtung. Das Werk- zeug steht in der Ansicht Innenkonturen zur Verfügung. Der ausschnitt wird immer im Innern der Kontur angebracht.

1.  Fügen Sie den Ausschnitt, den Sie in Ihrer Kontur positionieren wollen, in Ihre SN-Datei ein.

> **Verwenden Sie Gruppierungsrechtecke!**
> Wenn Sie mit mehreren Innenkonturen arbeiten, die eine Einheit bilden (z. B. ein Ausschnitt und eine Bohrung, die zum selben Beschlag gehören), dann sollten Sie diese gruppieren. Gruppierte Innenkonturen haben ein umschließendes Gruppierungsrechteck, mit dem sie gemeinsam an einer Außenkontur ausgerichtet werden können.
> Nur gruppierte Ausschnitte haben eine gemeinsame Richtung und können so gemeinsam ausgerichtet (vermaßt) werden. Eine Gruppe können Sie auch gegen eine andere Gruppe austauschen und dabei die Vermaßung beibehalten.

2.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
3.  Markieren Sie ein Segment des Ausschnitts. Wählen Sie das Segment am Ausschnitt, das Sie an einem Segment ihrer Scheibe ausrichten wollen. Klicken Sie dazu in die Nähe des Segment-Endpunktes, in dessen Rich- tung der Ausschnitt ausgerichtet werden soll. A+W CAD Designer (Sha- pes) ändert die Darstellung des Segmentes in einen roten Pfeil.
4.  Markieren Sie das Segment der Scheibe, an das Sie den Ausschnitt posi- tionieren wollen. Klicken Sie in die Nähe des Segment-Endpunktes, in des- sen Richtung der Ausschnitt ausgerichtet werden soll. A+W CAD Designer (Shapes) ändert die Darstellung des Segmentes in einen grünen Pfeil. Der Ausschnitt wird später so gedreht oder gespiegelt, dass die beiden Pfeile in die selbe Richtung zeigen.
5.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   D1: Paralleler Abstand zwischen den beiden markierten Segmenten.
    *   D2: Abstand des Segment-Endpunktes am Ausschnitt zum Nachbar- segment des ausgewählten Segmentes der Außenkontur.
    *   R1: Radius in Pfeilrichtung, mit dem der Ausschnitt an die Außenkante angeschlossen wird.
    *   R2: Radius gegen Pfeilrichtung, mit dem der Ausschnitt an die Außen- kante angeschlossen wird.
    *   X >> K: Überlappende Ausschnitt-Kontur an Konturkante abschneiden: Wenn Sie den Ausschnitt so an der Kontur ausrichten, dass der Aus- schnitt die Konturkante überragt, dann schneidet A+W CAD Designer (Shapes) den Ausschnitt an der Konturkante automatisch ab.
6.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) berechnet die neue Position des Ausschnitts und zeigt sie an.
    Wenn der Ausschnitt über die Kontur der Scheibe ragt, dann passt A+W CAD Designer (Shapes) den Ausschnitt automatisch so an die Kontur an, dass der Ausschnitt an der Überlappung gekürzt wird.

### Gruppierung positionieren

Mit diesem Werkzeug positionieren Sie eine Gruppierung im benötigten Abstand an der richtigen Kante und in der benötigten Ausrichtung. Das Werkzeug steht in der Ansicht Innenkonturen zur Verfügung. Der Aus- schnitt wird immer im Inneren der Kontur angebracht.

1.  Fügen Sie den Ausschnitt, den Sie in Ihrer Kontur positionieren wollen, in Ihre SN-Datei ein.
2.  Markieren Sie ein Segment des Ausschnitts. Wählen Sie das Segment am Ausschnitt, das Sie an einem Segment ihrer Scheibe ausrichten wollen. Klicken Sie dazu in die Nähe des Segment-Endpunktes, in dessen Rich- tung der Ausschnitt ausgerichtet werden soll. A+W CAD Designer (Sha- pes) ändert die Darstellung des Segmentes in einen roten Pfeil.
3.  Markieren Sie das Segment der Scheibe, an das Sie den Ausschnitt posi- tionieren wollen. Klicken Sie in die Nähe des Segment-Endpunktes, in des- sen Richtung der Ausschnitt ausgerichtet werden soll. A+W CAD Designer (Shapes) ändert die Darstellung des Segmentes in einen grünen Pfeil. Der Ausschnitt wird später so gedreht oder gespiegelt, dass die beiden Pfeile in die selbe Richtung zeigen.
4.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   D1: Paralleler Abstand zwischen den beiden markierten Segmenten.
    *   D2: Abstand des Segment-Endpunktes am Ausschnitt zum Nachbar- segment des ausgewählten Segmentes der Außenkontur.
    *   R1: Radius in Pfeilrichtung, mit dem der Ausschnitt an die Außenkante angeschlossen wird.
    *   R2: Radius gegen Pfeilrichtung, mit dem der Ausschnitt an die Außen- kante angeschlossen wird.
    *   X >> K: Überlappende Ausschnitt-Kontur an Konturkante abschneiden: Wenn Sie den Ausschnitt so an der Kontur ausrichten, dass der Aus- schnitt die Konturkante überragt, dann schneidet A+W CAD Designer (Shapes) den Ausschnitt an der Konturkante automatisch ab.
5.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) berechnet die neue Position des Ausschnitts und zeigt sie an.

Wenn der Ausschnitt über die Kontur der Scheibe ragt, dann passt A+W CAD Designer (Shapes) den Ausschnitt automatisch so an die Kontur an, dass der Ausschnitt an der Überlappung gekürzt wird.

### Segment halbieren

Mit diesem Werkzeug lässt sich ein Segment halbieren. Das Werkzeug kann auf ein Segment der Ausschnittkontur angewendet werden oder auch auf eine Kante des Gruppierungsrechtecks. Eins der neu entstandenen Segmente kann dann mit dem Werkzeug PLACEREC ausgewählt werden, so dass Vermaßungen bezüglich des neu entstandenen Punktes erzeugt werden. Dies ist insbesondere für symmetrische Ausschnitte (Vermaßung bezüglich der Symmetrieachse) wünschenswert.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Wählen Sie das Segment aus, dass Sie halbieren möchten. Dieses färbt sich rot ein und wird fett auf der Zeichenfläche dargestellt.
3.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) berechnet die Halbierung des Segments und zeigt sie mit einem Punkt an.

### Referenzsegment zum Einfügen von Ausschnitten setzen

Mit diesem Werkzeug markieren Sie ein Segment des Gruppierungsrecht- ecks als Referenzsegment. Das Werkzeug steht in der Ansicht Innenkon- turen zur Verfügung. Um den Ausschnitt oder das Ausschnittmakro per SN- API einfügen zu können, ist es notwendig, eine Gruppierung zu erzeugen.

1.  Wählen Sie das Werkzeug aus.
2.  Wählen Sie das Segment aus, das als Referenzsegment dienen soll. Kli- cken Sie in die Nähe des Endpunkts des Segments, der später positioniert werden soll. A+W CAD Designer (Shapes) färbt das Segment rot, der Pfeil zeigt auf den Referenzpunkt.
3.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) markiert das Segment nun mit einem Pfeil.

### Konturen verschmelzen

Verwenden Sie dieses Werkzeug, wenn Sie zwei Konturen miteinander verschmelzen wollen. Dies ist nützlich, wenn Sie z. B. einen Ausschnitt, der als eigene Kontur (z. B. aus der Stückliste) vorliegt, mit einer anderen Kon- tur (Scheibe) verbinden wollen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Ermitteln Sie die beiden Segmente der beiden Konturen, die übereinander liegen und verschmolzen werden sollen.
3.  Klicken Sie auf das erste Segment. A+W CAD Designer (Shapes) färbt das Segment rot.
4.  Klicken Sie auf das zweite Segment. A+W CAD Designer (Shapes) färbt das Segment grün.
5.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) ändert den Konturverlauf der Hauptkontur. Der Ausschnitt wird in die Hauptkontur integriert.

### Rechteckigen Randausschnitt als Stücklistenelement anbringen

Verwenden Sie dieses Werkzeug, wenn Sie einen rechteckigen Randaus- schnitt anbringen wollen, der in der Stückliste aufgeführt werden soll.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie das Segment, an dem Sie den Ausschnitt anbringen wollen. Klicken Sie in die Nähe des Segmentendes, von dem aus Sie den Aus- schnitt vermaßen wollen. A+W CAD Designer (Shapes) zeigt das Segment als roten Pfeil an. Die folgenden Maßangaben werden von der Pfeilspitze aus gerechnet.
3.  Geben Sie im Wertefenster folgende Werte an:
    *   D: Abstand von der Pfeilspitze, bei dem der Ausschnitt beginnt.
    *   W: Größe des Ausschnitts in Richtung des angeklickten Segmentes.
    *   H: Größe des Ausschnitts senkrecht zum angeklickten Segment.
    *   R1: Übergangsradius der Ecke in Pfeilrichtung.
    *   R2: Übergangsradius der Ecke gegen Pfeilrichtung.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) zeigt den definierten Ausschnitt mit ununterbrochenem Randsegment an. In der Ansicht Endprodukt können Sie die endgültige Kontur sehen.

### Randausschnitt anbringen und mit Kontur verschmelzen

Verwenden Sie dieses Werkzeug, wenn Sie einen rechteckigen Randaus- schnitt anbringen wollen, der mit der Kontur verschmelzen soll.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie das Segment, an dem Sie den Ausschnitt anbringen wollen. Klicken Sie dazu in die Nähe des Segmentendes, von dem aus Sie den Ausschnitt vermaßen wollen. A+W CAD Designer (Shapes) zeigt das Seg- ment als roten Pfeil an. Die folgenden Maßangaben werden von der Pfeil- spitze aus gerechnet.
3.  Geben Sie im Wertefenster folgende Werte an:
    *   D: Abstand von der Pfeilspitze zum Anfang des Ausschnitts.
    *   W: Größe des Ausschnitts in Richtung des markierten Segmentes.
    *   H: Größe des Ausschnitts senkrecht zum markierten Segment.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) zeigt den Ausschnitt mit neuen Randsegmenten an.

### Randausschnitt entfernen und Form schließen

Das Werkzeug dient zum Entfernen von Randausschnitten. Mit ihm kön- nen Sie einen in die Geometrie integrierten Randausschnitt durch ein Ge- radensegment ersetzen bzw. anschließende Randsegmente verlängern.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie das Segment, an dem der Randausschnitt beginnt. Das Segment färbt sich rot mit einer Pfeilspitze, die in Richung Ausschnitt zeigt.
3.  Markieren Sie das Segment, auf den der Randausschnitt trifft. Das Seg- ment färbt sich rot mit einer Pfeilspitze, die in Richung Ausschnitt zeigt.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Segmentkette zwischen den Spitzen der Selektionspfeile wird durch ein Geradensegment ersetzt bzw. das Randsegment wird verlängert.
5.  Die Form wird geschlossen.

### Eckausschnitt als Stücklistenelement anbringen

Verwenden Sie dieses Werkzeug, wenn Sie einen viereckigen Eckaussch- nitt anbringen wollen, der in der Stückliste aufgeführt werden soll.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie das erste Segment, an dem der Eckausschnitt angebracht werden soll. Klicken Sie dazu in die Nähe des Segmentendes, in der der Ausschnitt angebracht werden soll. A+W CAD Designer (Shapes) zeigt das Segment als roten Pfeil an. Die folgenden Maßangaben werden von der Pfeilspitze aus gerechnet.
3.  Markieren Sie das zweite Segment, an dem der Eckausschnitt angebracht werden soll. Klicken Sie dazu in die Nähe des Segmentendes, in der der Ausschnitt angebracht werden soll. A+W CAD Designer (Shapes) zeigt das Segment als grünen Pfeil an. Die folgenden Maßangaben werden von der Pfeilspitze aus gerechnet.
4.  Geben Sie im Wertefenster folgende Werte an:
    *   d1=: Abstand von der Pfeilspitze des ersten Segmentes zum Anfang des Ausschnitts.
    *   =: Markieren Sie diese Checkbox, wenn A+W CAD Designer (Shapes) den Ausschnitt parallel zum ersten Segment anbringen soll.
    *   +: Markieren Sie diese Checkbox, wenn A+W CAD Designer (Shapes) den Ausschnitt senkrecht zum ersten Segment anbringen soll.
    *   d2=: Abstand von der Pfeilspitze des zweiten Segmentes, bei dem der Ausschnitt beginnt.
    *   =: Markieren Sie diese Checkbox, wenn A+W CAD Designer (Shapes) den Ausschnitt parallel zum zweiten Segment anbringen soll.
    *   +: Markieren Sie diese Checkbox, wenn A+W CAD Designer (Shapes) den Ausschnitt senkrecht zum zweiten Segment anbringen soll.
    *   R1: Übergangsradius der Ecke auf dem ersten Segment.
    *   R2: Übergangsradius der Ecke auf dem zweiten Segment.
5.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) zeigt den Ausschnitt mit ununterbrochenem Randsegment an. In der Ansicht Endprodukt können Sie die endgültige Kontur sehen.

### Eckausschnitt anbringen und mit Kontur verschmelzen

Verwenden Sie dieses Werkzeug, wenn Sie einen viereckigen Eckaussch- nitt anbringen wollen, der mit der Kontur verschmelzen soll.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie das erste Segment, an dem der Eckausschnitt angebracht werden soll. Klicken Sie dazu in die Nähe des Segmentendes, in der der Ausschnitt angebracht werden soll. A+W CAD Designer (Shapes) zeigt das Segment als roten Pfeil an. Die folgenden Maßangaben werden von der Pfeilspitze aus gerechnet.
3.  Markieren Sie das zweite Segment, an dem der Eckausschnitt angebracht werden soll. Klicken Sie dazu in die Nähe des Segmentendes, in der der Ausschnitt angebracht werden soll. A+W CAD Designer (Shapes) zeigt das Segment als grünen Pfeil an. Die folgenden Maßangaben werden von der Pfeilspitze aus gerechnet.
4.  Geben Sie im Wertefenster folgende Werte an:
    *   d1=: Abstand von der Pfeilspitze des ersten Segmentes zum Anfang des Ausschnitts.
    *   =: Markieren Sie diese Checkbox, wenn A+W CAD Designer (Shapes) den Ausschnitt parallel zum ersten Segment anbringen soll.
    *   +: Markieren Sie diese Checkbox, wenn A+W CAD Designer (Shapes) den Ausschnitt senkrecht zum ersten Segment anbringen soll.
    *   d2=: Abstand von der Pfeilspitze des zweiten Segmentes, bei dem der Ausschnitt beginnt.
    *   =: Markieren Sie diese Checkbox, wenn A+W CAD Designer (Shapes) den Ausschnitt parallel zum zweiten Segment anbringen soll.
    *   +: Markieren Sie diese Checkbox, wenn A+W CAD Designer (Shapes) den Ausschnitt senkrecht zum zweiten Segment anbringen soll.
5.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) zeigt den Ausschnitt mit neuen Randsegmenten an.

### Bogenförmigen Randausschnitt als Stücklistenelement anbringen

Verwenden Sie dieses Werkzeug, wenn Sie einen bogenförmigen Rand- ausschnitt anbringen wollen, der in der Stückliste aufgeführt werden soll.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie das Segment, an dem Sie den Ausschnitt anbringen wollen. Klicken Sie dazu in die Nähe des Segmentendes, von dem aus Sie den Ausschnitt vermaßen wollen. A+W CAD Designer (Shapes) zeigt das Seg- ment als roten Pfeil an. Die folgenden Maßangaben werden von der Pfeil- spitze aus gerechnet.
3.  Geben Sie im Wertefenster folgende Werte an:
    *   D=: Abstand von der Pfeilspitze des Segmentes zum Anfang des Aus- schnitts.
    *   W=: Länge des Bogenausschnitts (Sehnenlänge).
    *   R=: Radius des Bogenausschnitts.
    *   R1=: Übergangsradius der Ecke in Pfeilrichtung.
    *   R2=: Übergangsradius der Ecke gegen Pfeilrichtung.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) zeigt den Ausschnitt mit ununterbrochenem Randsegment an. In der Ansicht Endprodukt können Sie die endgültige Kontur sehen.

### Bogenförmigen Randausschnitt anbringen und mit Kontur verschmelzen

Verwenden Sie dieses Werkzeug, wenn Sie einen bogenförmigen Rand- ausschnitt anbringen wollen, der mit der Kontur verschmelzen soll.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie das Segment, an dem Sie den Ausschnitt anbringen wollen. Klicken Sie dazu in die Nähe des Segmentendes, von dem aus Sie den Ausschnitt vermaßen wollen. A+W CAD Designer (Shapes) zeigt das Seg- ment als roten Pfeil an. Die folgenden Maßangaben werden von der Pfeil- spitze aus gerechnet.
3.  Geben Sie im Wertefenster folgende Werte an:
    *   d=: Abstand von der Pfeilspitze des Segmentes zum Anfang des Aus- schnitts.
    *   w=: Länge des Bogenausschnitts (Sehnenlänge).
    *   r=: Radius des Bogenausschnitts.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) zeigt den Ausschnitt mit neuen Randsegmenten an.

## Werkzeuge für Oberflächen

Nachfolgend finden Sie die Werkzeuge, die zur Bearbeitung von Oberflächen zur Verfügung stehen.

### Oberflächenbearbeitungen anbringen

Die Vorgehensweise zum Anbringen von Oberflächenbearbeitungen erfolgt in drei bzw. vier Schritten:

1.  Markieren Sie auf dem Glas einen rechteckigen Bereich für die Bearbei- tung
2.  Positionieren Sie diesen Bereich auf dem Glas
3.  Spezifizieren Sie die Art der Bearbeitung.
4.  Spezifizieren Sie die Ebene bzw. das Teil auf dem die Bearbeitung ausge- führt wird. Wenn ihre SN-Datei keine Stückliste enthält, wird Ihnen bereits in Schritt 3 eine Auswahl Oben/Unten/Beidseitig geboten. Falls sie eine SN-Datei mit Stückliste haben (z. B. für ein VSG oder ISO), geschieht das in einen separaten Schritt über den Menüpunkt Bearbeiten>Stückliste be- arbeiten (Alt+B). (Siehe ....)

Die Werkzeuge zur Bearbeitung von Oberflächen stehen üblicherweise in der Ansicht Innenkonturen zur Verfügung. Folgende Werkzeuge stehen zur Verfü- gung:

**Tab. A-24 Werkzeuge zur Bearbeitung der Oberfläche**

| Symbol | Kurzname | Beschreibung |
| :--- | :--- | :--- |
| | SURFRECT | "Rechteckigen Bereich positionieren" auf Seite A-345 |
| | SURFCOAT | "Oberfläche beschichten" auf Seite A-345 |
| | SURFMASK | "Oberfläche abkleben" auf Seite A-346 |
| | SURFROST | "Oberfläche mattieren" auf Seite A-347 |
| | SURFSAND | "Oberfläche sandstrahlen" auf Seite A-347 |
| | SURCOLOR | "Oberfläche mit Farbdruck versehen" auf Seite A-348 |
| 88 | SURENAML | "Oberfläche emaillieren" auf Seite A-349 |
| 88 | SURFSILK | "Oberfläche mit Siebdruck versehen" auf Seite A-349 |
| | SURPHOTO | "Einen Fotodruck auf der Oberfläche platzieren" auf Seite A-350 |
| | SURFHAND | "Eine Griffmulde auf der Oberfläche platzieren" auf Seite A-351 |
| * | SURFAPPL | "Eine Applikation auf der Oberfläche platzieren" auf Seite A-351 |
| | SURFPICT | "Ein Motiv auf der Oberfläche platzieren" auf Seite A-352 |
| | SURFSTAMP | "Einen Stempel auf der Oberfläche platzieren" auf Seite A-352 |
| | SURFLOGO | "Ein Logo auf der Oberfläche platzieren" auf Seite A-353 |

### Rechteckigen Bereich positionieren

Mit diesem Werkzeug positionieren Sie einen rechteckigen Bereich auf dem Glas. Dieser Schritt ist notwendig, um anschließend eine Oberflä- chenbearbeitung zu platzieren.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Positionieren Sie den Bereich auf dem Glas. Dies braucht nur eine unge- fähre Vorpositionierung zu sein.
3.  Geben Sie im Wertefenster folgende Werte an:
    *   -<->: Breite des Rechtecks
    *   |<->: Höhe des Rechtecks
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].
5.  Im Allgemeinen werden Sie das Rechteck nun noch exakt positionieren. Dazu verwenden Sie die Bemaßungswerkzeuge (z. B. Abstand Punkt/Li- nie).

### Oberfläche beschichten

Mit diesem Werkzeug können Sie einem zuvor definierten rechteckigen Bereich eine Beschichtung zuweisen.

"Rechteckigen Bereich positionieren" auf Seite A-345

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie den rechteckigen Bereich. Dieser wird in roter Farbe darge- stellt und das Wertefenster öffnet sich.
3.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   #: Sieb-/Schichtnummer
    *   Var: RAL-Nummern (Farbnummer)
    *   %: Wert für die Sättigung
    *   ^=: Markieren Sie diese Checkbox, wenn die Oberseite des Glases be- schichtet werden soll.
    *   v=: Markieren Sie diese Checkbox, wenn die Unterseite des Glases be- schichtet werden soll.
    *   ^v: Markieren Sie diese Checkbox, wenn die Oberseite und die Unter- seite des Glases beschichtet werden soll.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

> **Darstellung beschichteter Gläser**
> Die Strichdicke beschichteter Gläser im Profil kann vorgegeben werden, was zu einer markanteren Darstellung der Beschichtung genutzt werden kann.

### Oberfläche abkleben

Dieses Werkzeug dient dazu, eine Kantenbearbeitung an einer Kante mit Randoberflächenbearbeitung einzugeben.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie eine beliebige Kante. Der gesamte Bereich der Oberflächen- bearbeitung wird in roter Farbe dargestellt und das Wertefenster öffnet sich.
3.  Treffen Sie im Wertefenster die folgende Auswahl:
    *   ^=: Markieren Sie diese Checkbox, wenn die Oberseite des Glases ab- geklebt werden soll.
    *   v=: Markieren Sie diese Checkbox, wenn die Unterseite des Glases ab- geklebt werden soll.
    *   ^v: Markieren Sie diese Checkbox, wenn die Oberseite und die Unter- seite des Glases abgeklebt werden soll.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Der abgeklebte Be- reich wird schraffiert dargestellt.

### Oberfläche mattieren

Mit diesem Werkzeug können Sie einem zuvor definierten rechteckigen Bereich eine Mattierung zuweisen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie den rechteckigen Bereich. Dieser wird in roter Farbe darge- stellt und das Wertefenster öffnet sich.
3.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   #: Sieb-/Schichtnummer
    *   Var: RAL-Nummern (Farbnummer)
    *   %: Wert für die Sättigung
    *   ^=: Markieren Sie diese Checkbox, wenn die Oberseite des Glases mattiert werden soll.
    *   v=: Markieren Sie diese Checkbox, wenn die Unterseite des Glases mattiert werden soll.
    *   ^v: Markieren Sie diese Checkbox, wenn die Oberseite und die Unter- seite des Glases mattiert werden soll.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

> **Ergänzende Informationen**
> "Rechteckigen Bereich positionieren" auf Seite A-345

### Oberfläche sandstrahlen

Mit diesem Werkzeug können Sie einem zuvor definierten rechteckigen Bereich eine Sandstrahlung zuweisen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie den rechteckigen Bereich. Dieser wird in roter Farbe darge- stellt und das Wertefenster öffnet sich.
3.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   #: Sieb-/Schichtnummer
    *   Var: RAL-Nummern (Farbnummer)
    *   %: Wert für die Sättigung
    *   ^=: Markieren Sie diese Checkbox, wenn die Oberseite des Glases sandgestrahlt werden soll.
    *   v=: Markieren Sie diese Checkbox, wenn die Unterseite des Glases sandgestrahlt werden soll.
    *   ^v: Markieren Sie diese Checkbox, wenn die Oberseite und die Unter- seite des Glases sandgestrahlt werden soll.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

> **Ergänzende Informationen**
> "Rechteckigen Bereich positionieren" auf Seite A-345

### Oberfläche mit Farbdruck versehen

Mit diesem Werkzeug können Sie einem zuvor definierten rechteckigen Bereich einen Farbdruck zuweisen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie den rechteckigen Bereich. Dieser wird in roter Farbe darge- stellt und das Wertefenster öffnet sich.
3.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   #: Sieb-/Schichtnummer
    *   Var: RAL-Nummern (Farbnummer)
    *   %: Wert für die Sättigung
    *   ^=: Markieren Sie diese Checkbox, wenn der Farbdruck auf die Ober- seite des Glases gemacht werden soll.
    *   v=: Markieren Sie diese Checkbox, wenn der Farbdruck auf die Unter- seite des Glases gemacht werden soll.
    *   ^v: Markieren Sie diese Checkbox, wenn der Farbdruck auf die Ober- seite und die Unterseite des Glases gemacht werden soll.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

> **Ergänzende Informationen**
> "Rechteckigen Bereich positionieren" auf Seite A-345

### Oberfläche emaillieren

Mit diesem Werkzeug können Sie einem zuvor definierten rechteckigen Bereich eine Emaillierung zuweisen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie den rechteckigen Bereich. Dieser wird in roter Farbe darge- stellt und das Wertefenster öffnet sich.
3.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   #: Sieb-/Schichtnummer
    *   Var: RAL-Nummern (Farbnummer)
    *   %: Wert für die Sättigung
    *   ^=: Markieren Sie diese Checkbox, wenn die Oberseite des Glases emailliert werden soll.
    *   v=: Markieren Sie diese Checkbox, wenn die Unterseite des Glases emailliert werden soll.
    *   ^v: Markieren Sie diese Checkbox, wenn die Oberseite und die Unter- seite des Glases emailliert werden soll.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

> **Ergänzende Informationen**
> "Rechteckigen Bereich positionieren" auf Seite A-345

### Oberfläche mit Siebdruck versehen

Mit diesem Werkzeug können Sie einem zuvor definierten rechteckigen Bereich einen Siebdruck zuweisen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie den rechteckigen Bereich. Dieser wird in roter Farbe darge- stellt und das Wertefenster öffnet sich.
3.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   #: Sieb-/Schichtnummer
    *   Var: RAL-Nummern (Farbnummer)
    *   %: Wert für die Sättigung
    *   ^=: Markieren Sie diese Checkbox, wenn der Siebdruck auf die Ober- seite des Glases gemacht werden soll.
    *   v=: Markieren Sie diese Checkbox, wenn der Siebdruck auf die Unter- seite des Glases gemacht werden soll.
    *   ^v: Markieren Sie diese Checkbox, wenn der Siebdruck auf die Ober- seite und die Unterseite des Glases gemacht werden soll.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

> **Ergänzende Informationen**
> "Rechteckigen Bereich positionieren" auf Seite A-345

### Einen Fotodruck auf der Oberfläche platzieren

Mit diesem Werkzeug können Sie einem zuvor definierten rechteckigen Bereich einen Fotodruck zuweisen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie den rechteckigen Bereich. Dieser wird in roter Farbe darge- stellt und das Wertefenster öffnet sich.
3.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   #: Sieb-/Schichtnummer
    *   Var: RAL-Nummern (Farbnummer)
    *   %: Wert für die Sättigung
    *   ^=: Markieren Sie diese Checkbox, wenn der Fotodruck auf die Ober- seite des Glases gemacht werden soll.
    *   v=: Markieren Sie diese Checkbox, wenn der Fotodruck auf die Unter- seite des Glases gemacht werden soll.
    *   ^v: Markieren Sie diese Checkbox, wenn der Fotodruck auf die Ober- seite und die Unterseite des Glases gemacht werden soll.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

> **Ergänzende Informationen**
> "Rechteckigen Bereich positionieren" auf Seite A-345

