---
description: "DE-HB-AWCADDesignerShapes_6"
---


# Werkzeuge

---
## Werkzeuge verwenden

> **i Nicht für Schleifzuschläge verwenden!**
> Dieses Werkzeug ist kein Bearbeitungssymbol, um Schleifzuschläge zu realisieren. Seine Aufgabe besteht vielmehr darin, Konturen so zu verändern, dass die tatsächlich gewünschte Kontur mit geringem Aufwand gewonnen wird und somit keine Neukonstruktion erforderlich ist.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Wählen Sie nun mit der linken Maustaste die zu verschiebende Seite an. Die Seite wird anschließend selektiert, d. h., fett rot markiert.
3. Geben Sie den Wert ein, um den die Seite verschoben werden soll. Positiver Wert bedeutet eine Verschiebung nach außen, negativer Wert entspricht einer Verschiebung nach innen.
4. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) verschiebt die Kante.

*Abb. A-174 Kantenverschiebung nach innen oder außen*
*A vorher, B nachher*

Das linke Bild zeigt die Kontur vor der Verschiebung.
Die Seite *I* soll um 10 mm nach außen verschoben werden. Sie brauchen dazu nur die Seite *I* auszuwählen und im Wertefenster 10 mm einzutragen.

### Kontur nach innen oder außen parallel verschieben

Mit diesem Werkzeug können Sie einen beliebigen Schleifzuschlag auf alle Segmente einer Kontur definieren. Die Kontur wird dabei parallel nach innen oder außen verschoben. Eine Parallelverschiebung wird mit dem Symbol P am längsten Segment der Kontur angezeigt. Sie können eine Verschiebung nachträglich ändern oder auch wieder löschen. Eine Verschiebung nach innen wird durch einen negativen Verschiebungswert angezeigt.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie ein Segment der zu verschiebenden Kontur.
3. Geben Sie im Wertefenster die Verschiebung in mm ein. Ein positiver Wert verschiebt die Kontur nach außen, ein negativer nach innen.
4. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Kantenverschiebung wird ausgeführt, die ausgewählte Kontur wird neu berechnet und mit der Verschiebung dargestellt.

*Abb. A-175 Parallelverschiebung*

### Kontur durch Spiegeln an einem Segment verdoppeln

Um den Arbeitsaufwand bei der Erstellung symmetrischer Konturen zu reduzieren, können Sie im Menü Skizze nur eine symmetrische Hälfte entwerfen und diese dann spiegeln. Schließen Sie die symmetrische Hälfte mit einem Geradensegment an der Stelle der Spiegelachse. Diese Gerade können Sie mit dem hier beschriebenen Werkzeug als Spiegelachse verwenden. Dabei werden die bereits erfassten Innenkonturen (inkl. Bohrungen) und Kantenbearbeitungen ebenfalls gespiegelt. Es ist möglich, eine bereits gespiegelte Kontur an einer weiteren Geraden nochmals zu spiegeln.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Klicken Sie das Segment an, das als Spiegelachse dienen soll.
3. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Nun wird die komplette Kontur an der Symmetrieachse gespiegelt.

Wenn Sie eine symmetrische Kontur entwerfen möchten, reicht es aus, einen Teil zu skizzieren:

*Abb. A-176 Spiegelung*
*A ein Viertel erstellen*
*B das Viertel spiegeln*
*C die entstandene Hälfte wieder spiegeln*

### Produktionskonformität herstellen

Mit diesem Werkzeug ist es möglich, eine per DXF eingelesene oder digitalisierte Form in eine Hauptkontur und Ausschnitte zu zerlegen. Dies erlaubt es, die Form mit allen Möglichkeiten zu behandeln, die im A+W CAD Designer (Shapes) für die verschiedenen Fertigungsmethoden von Innenkonturen zur Verfügung stehen. So wird es dadurch z. B. möglich, die Ausschnitte automatisch beim Schneiden wegzulassen und dann auf einem Bearbeitungszentrum zu fertigen.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Klicken Sie die Segmente an, die zu den Ausschnitten gehören.
3. Im Wertefenster können Sie zusätzlich einen Rundungsradius für die Ecken am Übergang zwischen Ausschnitt und Hauptkontur eingeben.
4. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

### Ellipse erstellen

Um den Arbeitsaufwand bei der Erstellung symmetrischer Konturen zu reduzieren, können Sie im Register Geometrie eine Viertelellipse entwerfen und diese dann spiegeln.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Geben Sie im Wertefenster die folgenden Werte ein:
   - < >: Breite der Viertelellipse
   - ^: Höhe der Viertelellipse
3. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Viertelellipse wird platziert.
4. Klicken Sie das Segment an, das als Spiegelachse dienen soll.
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Nun wird die komplette Kontur an der Symmetrieachse gespiegelt.

**Ergänzende Informationen**
⇨ "Kontur durch Spiegeln an einem Segment verdoppeln"

## Unvollständige Konturen schließen

Um eine Kontur zu schließen (z. B. nach einem DXF-Import) stehen Ihnen folgende Werkzeuge zur Verfügung:

*Tab. A-13 Werkzeuge zum Nachbearbeiten von DXF-Importen*

| Symbol | Kurzname | Beschreibung |
| --- | --- | --- |
| | JOINCONT | ⇨ "Kontur schließen, die an mehreren Stellen offen ist" |
| | CLOSECON | ⇨ "Einzelne Lücke in Kontur schließen" |
| | CLCUTOUT | ⇨ "Ausschnitt schließen" |

### Kontur schließen, die an mehreren Stellen offen ist

Verwenden Sie dieses Werkzeug, wenn Ihnen nach einem DXF-Import oder durch unvollständige Erfassung nicht alle Segmente einer Kontur vorliegen, diese aber durch gemeinsame Schnittpunkte verbunden werden können. Sie können mit diesem Werkzeug Segmentketten (Segmentzüge) miteinander verbinden. Die Anfangs- und Endsegmente der Segmentketten müssen einen Schnittpunkt haben.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Klicken Sie auf das erste Segment am Segmentende, in dessen Richtung der Konturverlauf gehen soll. A+W CAD Designer (Shapes) zeigt das Segment rot an.
3. Klicken Sie auf ein oder mehrere weitere Segmente an dem Segmentende, in dessen Richtung der Konturverlauf gehen soll. Achten Sie darauf, dass die jeweils aufeinander folgenden Segmente einen Schnittpunkt bilden können. A+W CAD Designer (Shapes) zeigt die markierten Segmente rot an.
4. Wenn Sie alle markierten Segmente zu einer geschlossenen Kontur verbinden wollen, dann aktivieren Sie die Checkbox Schließen im Wertefenster.
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) verbindet die Segmente dadurch, dass es die Segmente bis zum Schnittpunkt mit dem folgenden Segment verlängert oder kürzt.
6. Wenn nach dem ersten Anwenden dieses Werkzeugs noch nicht alle Lücken geschlossen sind, dann wiederholen Sie die Anwendung dieses Werkzeugs. Wenn sich die letzte Lücke der Kontur mit diesem Werkzeug nicht schließen lässt, dann verwenden Sie dazu folgendes Werkzeug:
   ⇨ "Einzelne Lücke in Kontur schließen"

### Einzelne Lücke in Kontur schließen

Verwenden Sie dieses Werkzeug, um eine einzelne Lücke in einer Kontur zu schließen. Die nicht verbundenen Segmentenden müssen in ihrer Verlängerung einen Schnittpunkt besitzen.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Klicken Sie auf ein Segment der Kontur. A+W CAD Designer (Shapes) zeigt das Segment rot an.
3. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) schließt die Kontur dadurch, dass es Anfangs- und Endsegmente bis zu ihrem Schnittpunkt verlängert.

### Ausschnitt schließen

Nach dem Import von z. B. DXF-Daten kann es vorkommen, dass die Außenkontur vollständig angezeigt wird und Ausschnitte unvollständig (keine geschlossene Kontur). Verwenden Sie dieses Werkzeug, um mit Hilfe der Außenkontur die Lücke der fehlenden Segmente einer Innenkontur (Ausschnitt) zu schließen. Die nicht verbundenen Segmentenden müssen in ihrer Verlängerung einen Schnittpunkt mit der Außenkontur besitzen.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Klicken Sie auf ein Segment der nicht geschlossenen Kontur. A+W CAD Designer (Shapes) zeigt das Segment rot an.
3. Klicken Sie auf ein Segment der Außenkontur.
4. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) verbindet die Segmente dadurch, dass es das fehlende Segment oder die fehlenden Segmente der Innenkontur an der Stelle der Außenkontur ergänzt.

## Werkzeuge zur Vermaßung

Bevor Sie ein Werkzeug zur Vermaßung verwenden, sollten Sie das Symbol des Werkzeuges genau beachten. Das Bild eines Werkzeugs zeigt, welche Punkte und Segmente markiert werden müssen und welche Art von Vermaßung dabei entsteht. Alle Punkte und Segmente, die auf einem Symbole rot gekennzeichnet sind, müssen Sie nach der Auswahl des Werkzeugs markieren.

### Verschiedene Werkzeuge — ähnliche Vermaßungen

Für ähnliche Vermaßungen gibt es jeweils ein eigenes Werkzeug:

*Abb. A-177 Vermaßungswerkzeuge*
**A** Wenn ein roter Punkt direkt an einem roten Segment liegt, dann muss der Punkt des zu markierenden Segmentes angeklickt werden und auch das Segment selbst.
**B** Wenn auf dem Symbol die zu markierenden Punkte und Segmente so dargestellt, dass kein zu markierender Punkt an einem zu markierenden Segment liegt, dann müssen Sie dies auch bei der Verwendung des Werkzeuges beachten.

### Reihenfolge der Markierung

Damit ein Werkzeug das richtige Ergebnis liefert, müssen Sie beachten, welcher Punkt, welches Segment oder welche Kontur (z. B. Bohrung) Sie als erstes und als zweites anklicken.

### Punkte

Bei Werkzeugen die mehr als eine Markierung fordern, müssen Sie zuerst den zu vermaßenden Punkt (der sich nach Maßangabe verändern soll) und danach den Punkt, von dem aus die Vermaßung entstehen soll (der fest bleibt) markieren. In der Regel müssen Sie bei den Werkzeugen, die einen bestimmten Abstand definieren, 2 Punkte markieren. Das zusätzlich zu markierende Segment dient dabei als Bezugskante. Diese Bezugskante bestimmt, wie sich die bildlich dargestellte Vermaßung in Bezug zur Bezugskante ausrichten soll:

**Beispiel:** Sie möchten das angezeigte Werkzeug benutzen. Das Werkzeug zeigt 2 rote Punkte und ein rotes Segment. Dies bedeutet, dass Sie einen Abstand zwischen 2 Punkten definieren können. Der Abstand zwischen den Punkten wird nicht direkt gemessen, sondern ein Segment als Bezugskante angegeben. Der Abstand der Punkte wird als Abstand der Lote der Punkte auf das Segment angegeben. Die Maßhilfslinie richtet A+W CAD Designer (Shapes) parallel an diesem Segment (Bezugskante) aus. Markieren sie als erstes den gesuchten Punkt und danach den Bezugspunkt (von dem aus Sie das Maß erzeugen wollen). Markieren Sie als drittes das Bezugssegment.

> **i Nur auf bereits vermaßte Punkte weitere Maße beziehen!**
> Der 2. Punkt (Bezugspunkt) muss schon definiert sein, damit A+W CAD Designer (Shapes) auch einen Zusammenhang zur Gesamtgeometrie herstellen kann.

### Bohrungen

Achten Sie bei Kettenvermaßungen von Bohrungen darauf, welche Bohrung Sie zuerst anklicken und welche als zweites. Möchten Sie den Abstand einer Bohrung zu einer anderen Bohrungen definieren, dann müssen Sie zuerst die zu positionierende Bohrung anklicken und danach die bereits vermaßte Bohrung. Eine falsche Reihenfolge führt zu unerwarteten Ergebnissen.

### Modelle

Damit A+W CAD Designer (Shapes) Modelle mit Bögen in der Ansicht Skizze ohne Probleme berechnen kann, sollten Sie beim Zeichnen und Vermaßen folgendes beachten:
- Zeichnen Sie Modelle mit Bögen in der Ansicht Skizze schon annähernd so, wie die Geometrie später aussehen soll. Dabei sind die Maßstabsrelationen nicht wichtig.
- Vermaßung Sie die Skizze in der Reihenfolge, wie Sie die Skizze erstellt haben. Entscheiden Sie, ob Sie im oder gegen den Uhrzeigersinn vermaßen wollen und vermaßen Sie die Punkte dann reihum.

### Hilfslinien

Bei komplexen Konturen kann die Vermaßung schwierig sein. Durch Hilfslinien, auf die sich die Vermaßung beziehen kann, vereinfacht A+W CAD Designer (Shapes) die Vermaßung.

### Eigenschaften von Vermaßungen

Die Werkzeuge zur Vermaßung wurden für verschiedene Anforderungen entwickelt. Folgende Unterschiede gibt es:
- Werkzeuge zur Vermaßung von Konturen in der Ansicht Skizze. Damit können Sie Werte zur Konturberechnung vorgeben.
- Werkzeuge zur Positionierung fertiger Konturen. Damit können Sie fertig berechnete Konturen gegeneinander vermaßen (z. B. Ausschnitte oder Bohrungen).
- Werkzeuge zur Anzeige von Maßen. Damit können Sie anzeigen, welches Maß besteht.

Einige Werkzeuge können sowohl zur Konturvermaßung als auch zur Positionierung von Konturen verwendet werden.

Im Wertefenster stehen die Optionen aktiv, messend und fix zur Verfügung.

> **i Die Lage der zuerst angewählten Kontur ändert sich!**
> Wenn Sie Konturen zueinander vermaßen, dann ändert sich die Lage der zuerst angewählten Kontur (rot = aktiv).

### Kennzeichnung der Werkzeuge

In den nachfolgenden Übersichtstabellen werden die Werkzeuge zur Vermaßung wie folgt gekennzeichnet:

*Tab. A-14 Legende zur Werkzeugkennzeichnung*

| Kennzeichen | Bedeutung |
| --- | --- |
| **K** | Dieses Werkzeug können Sie zur Berechnung einer Kontur in der Ansicht Skizze verwenden. |
| **P** | Dieses Werkzeug können Sie zur Positionierung von Konturen gegeneinander verwenden (in den Technologieansichten und der Ansicht Innenkonturen). |
| **KP** | Dieses Werkzeug können Sie zur Berechnung und zur Positionierung von Konturen verwenden. |
| **M** | Dieses Werkzeug können Sie nur messend verwenden. |

An den Symbolen der Werkzeuge können Sie diese Unterscheidung nicht erkennen. Die Kennzeichnung ist nur in dieser Dokumentation enthalten. Je nach aktueller Ansicht stehen nur die jeweils brauchbaren Werkzeuge zur Verfügung.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

## Segmente vermaßen

Um Segmente zu vermaßen, stehen Ihnen folgende Werkzeuge zur Verfügung:

*Tab. A-15 Werkzeuge zum Vermaßen von Segmenten*

| Symbol | Kurzname | Beschreibung |
| --- | --- | --- |
| | DSTPTPT | ⇨ "Abstand zwischen den Endpunkten von zwei Segmenten vermaßen" |
| | DST2PT | ⇨ "Abstand zwischen zwei Punkten vermaßen" |
| | PRJPTSG | ⇨ "Abstand zwischen einem Punkt und einem Strecken-Endpunkt parallel zu einer Strecke vermaßen" |
| | DSTPTSG | "Abstand zwischen einem Punkt und einer Strecke vermaßen" |
| | PRJ2PTSG | ⇨ "Abstand zwischen zwei Punkten parallel zu einer Strecke vermaßen" |
| | DST2PTSG | "Abstand zwischen zwei Punkten senkrecht zu einer Strecke vermaßen" |
| | PRJPTISY | "Vertikalen Abstand zwischen einem Punkt und einem Schnittpunkt vermaßen" |
| | PRJPTISX | ⇨ "Horizontalen Abstand zwischen einem Punkt und einem Schnittpunkt vermaßen" |
| | PRJPTIS | ⇨ "Abstand zwischen einem Punkt und einem Schnittpunkt parallel zu einer Geraden vermaßen" |
| | DSTPTPTY | "Vertikalen Abstand zwischen zwei Punkten vermaßen" |
| | DSTPTPTX | ⇨ "Horizontalen Abstand zwischen zwei Punkten vermaßen" |
| | DSTPTIS | "Abstand zwischen einem Punkt und einem Schnittpunkt senkrecht zu einer Geraden vermaßen" |
| | LINELEN | ⇨ "Länge einer Geraden vermaßen" |
| | COORREL | ⇨ "X- und Y-Koordinaten eines Segment-Endpunktes relativ zu einem anderen vermaßen" |
| | COORABS | ⇨ "X- und Y-Koordinaten eines Segment-Endpunktes vermaßen" |
| | DIMCORNR | ⇨ "Abstand zur abgeschnittenen Ecke ermitteln" |

### Abstand zwischen den Endpunkten von zwei Segmenten vermaßen

Hiermit bestimmen Sie die Distanz zwischen zwei Konturpunkten, die nicht direkt über ein Segment miteinander verbunden sind.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie die zu vermaßenden Konturpunkte in beliebiger Reihenfolge. Der erste angewählte Punkt färbt sich rot, der zweite grün.
3. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
4. Bei einer aktiven Vermaßung geben Sie die Entfernung im Wertefenster unter D ein.
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Vermaßung wird zwischen den gewählten Punkten angezeigt. Nach mehreren Vermaßungen kann die Skizze unübersichtlich werden.
6. Wählen Sie Neu zeichnen im Menü Ansicht, um eine Auswertung der aktiven Vermaßung zu erzwingen und um die Skizze von A+W CAD Designer (Shapes) übersichtlicher vermaßen zu lassen.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Abstand zwischen zwei Punkten vermaßen

Mit diesem Werkzeug können Sie die Distanz zwischen zwei Konturpunkten eingeben. Dabei kann es sich um zwei beliebige Endpunkte von Segmenten handeln.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie die zu vermaßenden Konturpunkte in beliebiger Reihenfolge. Der erste angewählte Punkt färbt sich rot, der zweite Punkt grün.
3. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
4. Bei einer aktiven Vermaßung geben Sie die Entfernung im Wertefenster unter D ein.
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Vermaßung wird anschließend zwischen an den gewählten Punkten angezeigt. Nach mehreren Vermaßungen kann die Skizze unübersichtlich werden.
6. Wählen Sie Neu zeichnen im Menü Ansicht, um eine Auswertung der aktiven Vermaßung zu erzwingen und um die Skizze von A+W CAD Designer (Shapes) übersichtlicher vermaßen zu lassen.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Abstand zwischen einem Punkt und einem Strecken-Endpunkt parallel zu einer Strecke vermaßen

Dieses Werkzeug können Sie in der Ansicht Skizze zur Vermaßung einer Kontur nutzen. Wenn Sie in der Ansicht Innenkonturen sind, ermöglicht Ihnen dieses Werkzeug, zwei Konturen zueinander zu positionieren.

Mit diesem Werkzeug können Sie die zu einer Strecke parallele Entfernung eines Konturpunktes zu einem der beiden Strecken-Endpunkte angeben. Die Strecke muss in der dem 2. Konturpunkt entgegengesetzten Hälfte angewählt werden. Bei einer Anwahl in der angrenzenden Hälfte wird der 2. Konturpunkt wieder abgewählt.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Wählen Sie den 1. Punkt aus. Dieser färbt sich rot.
3. Wählen Sie den Endpunkt eines Segmentes aus. Dieser färbt sich grün.
4. Wählen Sie das Segment aus, auf dem Sie den Punkt gewählt haben. Markieren Sie das Segment in der dem zuvor angewählten Punkt entgegengesetzten Hälfte. Die Strecke färbt sich hellgrau.
5. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
6. Bei einer aktiven Vermaßung geben Sie anschließend die entsprechende (auf die Strecke projizierte) Entfernung zwischen dem freien Konturpunkt und dem Strecken-Endpunkt im Wertefenster unter P ein.
7. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Das von Ihnen eingegebene Maß wird in die Zeichnung übernommen.

**Beispiel:**
*Abb. A-178 Abstand zwischen einem Punkt und einem Strecken-Endpunkt parallel zu einer Strecke vermaßen*
*A Beispiel in der Ansicht Skizze*
*B Beispiel in der Ansicht Innenkontur*

**In der Ansicht Skizze:**
Die Vermaßung der Strecke C – A projiziert auf g (400 mm) soll nachvollzogen werden.
- Werkzeug anklicken.
- Konturpunkt A anwählen.
- Strecken-Endpunkt C wählen.
- Strecke g wählen, auf die die Entfernung C - A projiziert werden soll.

**In der Ansicht Innenkonturen:**
Die Konturpunkte sind durch Großbuchstaben, die Strecken sind durch Kleinbuchstaben gekennzeichnet. Der freie Konturpunkt ist in diesem Fall A, die Bezugsstrecke ist b, der Strecken-Endpunkt B und die zu der Bezugsstrecke parallele Entfernung ist die Länge a (=300mm).

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Abstand zwischen einem Punkt und einer Strecke vermaßen

Mit diesem Werkzeug definieren Sie die senkrechte Entfernung von einem beliebigen Konturpunkt zu einer Konturgeraden oder Hilfslinie. In der Ansicht Skizze können Sie dieses Werkzeug zur Vermaßung einer Kontur nutzen. In der Ansicht Innenkonturen ermöglicht Ihnen dieses Werkzeug, zwei Konturen zueinander zu positionieren.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie den Punkt einer Figur. Dieser färbt sich rot.
3. Wählen Sie ein Segment aus. Dieses färbt sich grün.
4. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
5. Bei einer aktiven Vermaßung geben Sie im Wertefenster unter D den Abstand des Punktes zum Segment ein.
6. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Das von Ihnen eingegebene Maß wird in die Zeichnung übernommen.

**Beispiel:**
*Abb. A-179 Abstand Punkt - Segment*
- **C:** Konturpunkt
- **a:** Geradensegment
- **500:** zu vermaßende senkrechte Entfernung

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Abstand zwischen zwei Punkten parallel zu einer Strecke vermaßen

Dieses Werkzeug ermöglicht Ihnen, die zu einer Strecke parallele Entfernung zweier Konturpunkte anzugeben. In der Ansicht Skizze können Sie dieses Werkzug zur Vermaßung einer Kontur nutzen. Wenn Sie in der Ansicht Innenkonturen sind, ermöglicht Ihnen dieses Werkzeug, zwei Konturen zueinander zu positionieren.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Wählen Sie den 1. Punkt aus. Dieser färbt sich rot.
3. Wählen Sie den 2. Punkt aus. Dieser färbt sich grün.
4. Wählen Sie die Bezugsstrecke (gerades Segment) aus. Dieses Segment färbt sich hellgrau.
5. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
6. Bei einer aktiven Vermaßung geben Sie im Wertefenster unter P die auf die Strecke projizierte Entfernung zwischen den Konturpunkten ein.
7. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Das von Ihnen eingegebene Maß wird in die Zeichnung übernommen.

**Beispiel:**
*Abb. A-180 Abstand zwischen zwei Punkten parallel zu einer Strecke*

**Vermaßung der Länge x = 400:**
- Werkzeug anklicken.
- Konturpunkte A und B markieren.
- Gerade c wählen, auf die die Entfernung bezogen wird.
- Länge 400 im Wertefenster unter P eingeben.
- Eingabe bestätigen (<ENTER> oder [OK])

### Abstand zwischen zwei Punkten senkrecht zu einer Strecke vermaßen

Dieses Werkzeug ermöglicht es Ihnen, die zu einer Strecke senkrechte Entfernung zweier Konturpunkte anzugeben. Die freien Konturpunkte dürfen nicht über ein Segment miteinander verbunden sein. In der Ansicht Skizze können Sie dieses Werkzug zur Vermaßung einer Kontur nutzen. Wenn Sie in der Ansicht Innenkonturen sind, ermöglicht Ihnen dieses Werkzeug, zwei Konturen zueinander zu positionieren.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Wählen Sie den 1. Punkt einer Figur aus. Dieser färbt sich rot.
3. Wählen Sie den 2. Punkt einer Figur aus. Dieser färbt sich grün.
4. Wählen Sie das zu den 2 Punkten senkrechte Segment aus. Dieses färbt sich hellgrau.
5. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
6. Bei einer aktiven Vermaßung geben Sie im Wertefenster die auf die Strecke senkrechte Entfernung D zwischen den beiden Konturpunkten an.
7. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Das von Ihnen eingegebene Maß wird in die Zeichnung übernommen.

**Beispiel:**
*Abb. A-181 Abstand zwischen zwei Punkten*
*A in der Ansicht Skizze*
*B in der Ansicht Innenkontur*

**In der Ansicht Skizze:**
Sie können die zur Basis c senkrechte Entfernung zwischen den beiden Konturpunkten A und B eingeben:
- Werkzeug anklicken
- Konturpunkte A und B markieren
- Basisgerade c markieren.
- Entfernung 400 im Wertefenster eingeben
- Eingabe bestätigen (<ENTER> oder [OK])

**In der Ansicht Innenkonturen:**
Sie können die zur Strecke f rechtwinklige Entfernung zwischen den Konturpunkten A und B durch die Werteingabe von 200 bestimmen.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Vertikalen Abstand zwischen einem Punkt und einem Schnittpunkt vermaßen

Dieses Werkzeug ermöglicht Ihnen, die Entfernung eines Punktes zu einem Segment in Richtung der Y-Achse anzugeben. Dabei müssen Sie darauf achten, dass von dem Punkt aus in Richtung der Y-Achse tatsächlich ein Schnittpunkt mit dem Segment existiert. Dieses Werkzeug kann in der Ansicht Skizze nicht benutzt werden. In anderen Ansichten ist es dazu gedacht, Konturen gegeneinander zu positionieren.

> **i Vermaßung auf Koordinatensystem vermeiden!**
> Wenn Sie mit diesem Werkzeug vermaßen, dann müssen Sie sicher sein, dass die Kontur später nicht mehr gedreht wird. Maße, die sich auf das Koordinatensystem beziehen verändern die Kontur beim drehen, weil das Koordinatensystem (Bezugssystem) nicht mitgedreht wird. Vermaßen Sie mit anderen Werkzeugen, denn die Kontur später noch gedreht werden soll.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie den Punkt einer Kontur. Dieser färbt sich rot.
3. Markieren Sie ein Segment, das mit diesem Punkt einen Schnittpunkt in Richtung der Y-Achse hat. Dieses färbt sich grün.
4. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
5. Bei einer aktiven Vermaßung geben Sie im Wertefenster die auf die Strecke projizierte Entfernung P zwischen dem Konturpunkt und dem Segmentschnittpunkt ein.
6. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Das von Ihnen eingegebene Maß wird in die Zeichnung übernommen.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Horizontalen Abstand zwischen einem Punkt und einem Schnittpunkt vermaßen

Dieses Werkzeug ermöglicht Ihnen, die Entfernung eines Punktes zu einem Segment in Richtung der X-Achse anzugeben. Dabei müssen Sie darauf achten, dass von dem Punkt aus in Richtung der X-Achse tatsächlich ein Schnittpunkt mit dem Segment existiert. Dieses Werkzeug kann in der Ansicht Skizze nicht benutzt werden. In anderen Ansichten ist es dazu gedacht, Konturen gegeneinander zu positionieren.

> **i Vermaßung auf Koordinatensystem vermeiden!**
> Wenn Sie mit diesem Werkzeug vermaßen, dann müssen Sie sicher sein, dass die Kontur später nicht mehr gedreht wird. Maße, die sich auf das Koordinatensystem beziehen verändern die Kontur beim drehen, weil das Koordinatensystem (Bezugssystem) nicht mitgedreht wird. Vermaßen Sie mit anderen Werkzeugen, denn die Kontur später noch gedreht werden soll.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie den zu vermaßenden Punkt. Dieser färbt sich rot.
3. Markieren Sie ein Segment, das mit diesem Punkt in horizontaler Richtung einen Schnittpunkt hat. Dieses färbt sich grün.
4. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
5. Bei einer aktiven Vermaßung geben Sie im Wertefenster die auf die Strecke projizierte Entfernung P zwischen dem Konturpunkt und dem Segmentschnittpunkt in Richtung der X-Achse ein.
6. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Das von Ihnen eingegebene Maß wird in die Zeichnung übernommen.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Abstand zwischen einem Punkt und einem Schnittpunkt parallel zu einer Geraden vermaßen

Dieses Werkzeug ermöglicht Ihnen, den Abstand eines Punktes zu dem Schnittpunkt eines Segment in Richtung einer Geraden anzugeben. Dabei müssen Sie darauf achten, dass der Punkt mit dem Segment in Richtung der Geraden tatsächlich einen Schnittpunkt besitzt. Dieses Werkzeug kann in der Ansicht Skizze nicht benutzt werden. In anderen Ansichten ist es dazu gedacht, Konturen gegeneinander zu positionieren.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie den Punkt einer Figur. Dieser färbt sich rot.
3. Markieren Sie ein Segment, das mit diesem Punkt in Richtung eines Referenzsegmentes einen Schnittpunkt hat. Dieses färbt sich grün.
4. Markieren Sie das Referenzsegment, in dessen Richtung sich der zu bestimmende Abstand beziehen soll. Dieses Segment färbt sich hellgrau.
5. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
6. Bei einer aktiven Vermaßung geben Sie im Wertefenster die auf die Strecke projizierte Entfernung P zwischen dem Konturpunkt und dem Segmentschnittpunkt in Richtung des Referenzsegmentes ein.
7. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Das von Ihnen eingegebene Maß wird in die Zeichnung übernommen.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Vertikalen Abstand zwischen zwei Punkten vermaßen

Mit diesem Werkzeug können Sie die Distanz zwischen zwei Konturpunkten in Richtung der Y-Achse eingeben. Dabei kann es sich um zwei beliebige Endpunkte von Segmenten handeln.

> **i Vermaßung auf Koordinatensystem vermeiden!**
> Wenn Sie mit diesem Werkzeug vermaßen, dann müssen Sie sicher sein, dass die Kontur später nicht mehr gedreht wird. Maße, die sich auf das Koordinatensystem beziehen verändern die Kontur beim drehen, weil das Koordinatensystem (Bezugssystem) nicht mitgedreht wird. Vermaßen Sie mit anderen Werkzeugen, denn die Kontur später noch gedreht werden soll.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie die zu vermaßenden Konturpunkte in beliebiger Reihenfolge. Der erste angewählte Punkt färbt sich rot, der zweite grün.
3. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
4. Bei einer aktiven Vermaßung geben Sie im Wertefenster die Entfernung D ein.
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Vermaßung wird zwischen an den gewählten Punkten angezeigt.
6. Wählen Sie Neu zeichnen im Menü Ansicht, um eine Auswertung der aktiven Vermaßung zu erzwingen und um die Skizze von A+W CAD Designer (Shapes) übersichtlicher vermaßen zu lassen.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Horizontalen Abstand zwischen zwei Punkten vermaßen

Mit diesem Werkzeug können Sie die Distanz zwischen zwei Konturpunkten in Richtung der X-Achse eingeben. Dabei kann es sich um zwei beliebige Endpunkte von Segmenten handeln.

> **i Vermaßung auf Koordinatensystem vermeiden!**
> Wenn Sie mit diesem Werkzeug vermaßen, dann müssen Sie sicher sein, dass die Kontur später nicht mehr gedreht wird. Maße, die sich auf das Koordinatensystem beziehen verändern die Kontur beim drehen, weil das Koordinatensystem (Bezugssystem) nicht mitgedreht wird. Vermaßen Sie mit anderen Werkzeugen, denn die Kontur später noch gedreht werden soll.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie die zu vermaßenden Konturpunkte in beliebiger Reihenfolge. Der erste angewählte Punkt färbt sich rot, der zweite grün.
3. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
4. Bei einer aktiven Vermaßung geben Sie im Wertefenster die Entfernung D ein.
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Vermaßung wird zwischen an den gewählten Punkten angezeigt.
6. Wählen Sie Neu zeichnen im Menü Ansicht, um eine Auswertung der aktiven Vermaßung zu erzwingen und um die Skizze von A+W CAD Designer (Shapes) übersichtlicher vermaßen zu lassen.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Abstand zwischen einem Punkt und einem Schnittpunkt senkrecht zu einer Geraden vermaßen

Dieses Werkzeug ermöglicht Ihnen, den Abstand eines Punktes zum Schnittpunkt mit einem Segment senkrecht zu einer Geraden (Referenzsegment) anzugeben. Dabei müssen Sie darauf achten, dass der Punkt mit dem Segment in senkrechter Richtung mit einer Geraden tatsächlich einen Schnittpunkt besitzt. Dieses Werkzeug kann in der Ansicht Skizze nicht benutzt werden. In anderen Ansichten ist es dazu gedacht, Konturen gegeneinander zu positionieren.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie den Punkt einer Figur. Dieser färbt sich rot.
3. Markieren Sie ein Segment, das mit diesem Punkt in senkrechter Richtung zu einem Referenzsegment einen Schnittpunkt hat. Dieses färbt sich grün.
4. Markieren Sie das Referenzsegment, auf dessen Senkrechte sich der zu bestimmende Abstand beziehen soll. Dieses Segment färbt sich hellgrau.
5. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
6. Bei einer aktiven Vermaßung geben Sie im Wertefenster die auf die Strecke projizierte Entfernung P zwischen dem Konturpunkt und dem Segmentschnittpunkt in senkrechter Richtung zum Referenzsegment ein.
7. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Das von Ihnen eingegebene Maß wird in die Zeichnung übernommen.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Länge einer Geraden vermaßen

Mit diesem Vermaßungswerkzeug können Sie die exakte Länge eines Geradensegmentes von seinem Startpunkt bis zu seinem Endpunkt bestimmen.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie das zu vermaßende Geradensegment.
3. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
4. Bei einer aktiven Vermaßung geben Sie im Wertefenster die Streckenlänge D ein.
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].
6. Wählen Sie Neu zeichnen im Menü Ansicht, um eine Auswertung der aktiven Vermaßung zu erzwingen und um die Skizze von A+W CAD Designer (Shapes) übersichtlicher vermaßen zu lassen.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### X- und Y-Koordinaten eines Segment-Endpunktes relativ zu einem anderen vermaßen

Mit diesem Werkzeug können Sie Relativkoordinaten eines Konturpunktes angeben. Relativkoordinaten sind Entfernungen in X- und Y-Richtung, die sich auf einen zuvor gewählten Konturpunkt beziehen.

> **i Vermaßung auf Koordinatensystem vermeiden!**
> Wenn Sie mit diesem Werkzeug vermaßen, dann müssen Sie sicher sein, dass die Kontur später nicht mehr gedreht wird. Maße, die sich auf das Koordinatensystem beziehen verändern die Kontur beim drehen, weil das Koordinatensystem (Bezugssystem) nicht mitgedreht wird. Vermaßen Sie mit anderen Werkzeugen, denn die Kontur später noch gedreht werden soll.

- Der X-Wert gibt die waagerechte Entfernung (X-Richtung) zwischen den beiden gewählten Punkten an.
  - positiver Wert: Abstand nach rechts
  - negativer Wert: Abstand nach links
- Der Y-Wert gibt die senkrechte Entfernung (Y-Richtung) zwischen den beiden gewählten Punkten an.
  - positiver Wert: Abstand nach oben
  - negativer Wert: Abstand nach unten

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie den Punkt, dessen Koordinaten sie festlegen wollen. Dieser färbt sich rot.
3. Markieren Sie den Punkt, der als Referenzpunkt dienen soll. Dieser färbt sich grün.
4. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
5. Bei einer aktiven Vermaßung geben Sie im Wertefenster den waagerechten (X-Wert) und den senkrechten (Y-Wert) Abstand zwischen den gewählten Konturpunkten ein.
6. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### X- und Y-Koordinaten eines Segment-Endpunktes vermaßen

Mit diesem Werkzeug können Sie Absolutkoordinaten eines Konturpunktes bestimmen. Absolutkoordinaten sind Entfernungen in X- und Y-Richtung, die sich auf den Ursprung (Nullpunkt) des Koordinatenkreuzes beziehen.

Ein X-Wert gibt die waagerechte Entfernung eines Punktes vom Ursprung an. Liegt der Punkt rechts vom Nullpunkt, so ist der Wert positiv, liegt er links davon, so ist der Wert negativ und muss mit einem Minus eingegeben werden.

Der Y-Wert eines Punktes gibt die senkrechte Entfernung vom Ursprung an. Liegt der Konturpunkt oberhalb des Ursprungs, so ist er positiv, liegt er unterhalb des Nullpunktes, so ist der Wert negativ und muss mit einem Minus eingegeben werden.

> **i Vermaßung auf Koordinatensystem vermeiden!**
> Wenn Sie mit diesem Werkzeug vermaßen, dann müssen Sie sicher sein, dass die Kontur später nicht mehr gedreht wird. Maße, die sich auf das Koordinatensystem beziehen verändern die Kontur beim drehen, weil das Koordinatensystem (Bezugssystem) nicht mitgedreht wird. Vermaßen Sie mit anderen Werkzeugen, denn die Kontur später noch gedreht werden soll.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie den Konturpunkt, dessen Koordinaten Sie bestimmen möchten. Dieser färbt sich rot.
3. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
4. Bei einer aktiven Vermaßung geben Sie im Wertefenster die waagerechte Entfernung (X-Wert) und die senkrechte Entfernung (Y-Wert) des gewählten Konturpunktes vom Nullpunkt ein.
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

**Beispiel:**
*Abb. A-182 X- und Y-Koordinaten*
*A Koordinatenkreuz*

Auf der Benutzeroberfläche sehen Sie eine Markierung (Kreuzchen) am Nullpunkt.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"
⇨ Werkzeuge, "X- und Y-Koordinaten eines Segment-Endpunktes relativ zu einem anderen vermaßen"

### Abstand zur abgeschnittenen Ecke ermitteln

Verwenden Sie dieses Werkzeug, um zu ermitteln, welchen Abstand ein Segmentende zum Eckpunkt einer abgeschnittenen Ecke hat.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Klicken Sie auf das erste Segment. Klicken Sie an dem Segmentende, in dessen Richtung der Abstand ermittelt werden soll. A+W CAD Designer (Shapes) zeigt das Segment rot an.
3. Klicken Sie auf das zweite Segment, mit dem das erste Segment eine Ecke bilden kann. Klicken Sie an dem Segmentende, in dessen Richtung die Ecke liegt. A+W CAD Designer (Shapes) zeigt das Segment grün an.
4. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) ermittelt den Abstand der Ecke zum zuerst angeklickten Segment und zeigt ihn an.

## Winkel vermaßen

Um Winkel zu vermaßen, stehen Ihnen folgende Werkzeuge zur Verfügung:

*Tab. A-16 Werkzeuge zum Vermaßen von Winkeln*

| Symbol | Kurzname | Beschreibung |
| --- | --- | --- |
| | ANGARC | ⇨ "Öffnungswinkel eines Bogens vermaßen" |
| | TANGSGSG | ⇨ "Segment glatt anschließen" |
| | SGANGSG | ⇨ "Innenwinkel zwischen zwei angrenzenden Segmenten vermaßen" |
| | ANGSGSG | ⇨ "Innenwinkel zwischen zwei Segmenten vermaßen" |
| | PARALLEL | ⇨ "Zwei Segmente parallel zueinander vermaßen" |
| | ORTHOGON | ⇨ "Zwei Segmente senkrecht zueinander vermaßen" |

### Öffnungswinkel eines Bogens vermaßen

Mit diesem Werkzeug bestimmen Sie den Öffnungswinkel eines Kreisbogens, bzw. den Winkel, der von dem Kreisbogen eingeschlossen wird.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Wählen Sie das zu vermaßende Kreissegment aus.
3. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
4. Bei einer aktiven Vermaßung geben Sie in dem Wertefenster den Winkel in Grad ein.
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Der Eingabewert wird in die Zeichnung übernommen.

**Beispiel:**
*Abb. A-183 Öffnungswinkel eines Bogens*

**Vermaßungsvorschlag der Bogenvermaßung:**
- Länge der unteren Geraden vermaßen (1000 mm).
- Werkzeug Öffnungswinkel eines Bogens vermaßen anklicken.
- Kreisbogen anwählen.
- Öffnungswinkel angeben (120°).
- Eingabe bestätigen.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Segment glatt anschließen

Mit diesem Werkzeug können Sie einen tangentialen Übergang zwischen zwei Segmenten bestimmen. D. h., das weiterführende Segment beginnt mit dergleichen Steigung, mit der das andere Segment abschließt. Die Steigungsdifferenz ist also im gemeinsamen Konturpunkt gleich Null.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Wählen Sie die zwei Segmente aus, die tangential ineinander übergehen sollen. Das erste färbt sich rot, das zweite grün.
3. Vergeben Sie dem Übergang, falls gewünscht, eine Eigenschaft (aktiv, messend, fixiert).
4. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Der von Ihnen ausgewählte tangentiale Übergang wird berechnet und auf der Zeichenfläche dargestellt.

> **i Nachträgliche Kantenbearbeitung anbringen**
> Wenn Sie nachträglich Kantenbearbeitungen (oder eine gewöhnliche Kantenverschiebung) an einem Segment anbringen, welches tangential angrenzende Segmente hat, so werden diese auf alle tangential anschließenden Segmente übertragen.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Innenwinkel zwischen zwei angrenzenden Segmenten vermaßen

Mit diesem Werkzeug bestimmen Sie den Winkel, der von zwei (sich berührenden) Segmenten eingeschlossen wird.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie die beiden Segmente, die den zu bestimmenden Winkel einschließen, in beliebiger Reihenfolge mit der Maus. Die erste ausgewählte Seite wird das aktive Segment und die zweite Seite das passive Segment. Das aktive Segment trägt dabei nach der Eingabe das Winkelsymbol.
3. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
4. Bei einer aktiven Vermaßung geben Sie im Wertefenster den Winkel in Grad ein.
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Der Winkel wird nun in der Zeichnung angezeigt.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Innenwinkel zwischen zwei Segmenten vermaßen

Dieses Werkzeug ermöglicht es Ihnen, den Innenwinkel zwischen zwei beliebigen Segmenten, deren Endpunkte sich nicht berühren, zu bestimmen. Mit diesem Werkzeug können Sie Innenwinkel auch ausrichten:

Wenn Sie eine Kontur erstellt und fertig vermaßt haben, können Sie im Menü Innenkonturen diese Kontur anzeigen. Hier können Sie fehlende Winkelangaben zwischen beliebigen Seiten, die sich aus den gegebenen Maßangaben errechnen lassen, anzeigen lassen. Beachten Sie, dass Sie in diesem Fall keine Formänderung der Kontur vornehmen können, also den errechneten Winkel nicht verändern können. Diese Möglichkeit kann auch in anderen Ansichten (wie Geometrie) zur Verfügung stehen.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie das erstes Segment mit der Maus.
3. Markieren Sie das zweite Segment mit der Maus.
4. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Der Winkel zwischen den gewählten Seiten wird nun an der ersten Seite angezeigt.

**Beispiel:**
*Abb. A-184 Innenwinkel zwischen zwei Segmenten vermaßen (1)*

Wenn Sie diese Kontur skizziert und vollständig vermaßt haben (z. B. die Seiten a, b, c, d und einen rechten Winkel), können Sie sich noch den Winkel a zwischen den Seiten a und b, anzeigen lassen:
- Werkzeug anklicken.
- Segment a markieren.
- Segment b markieren.
- Eingabe bestätigen (<ENTER> oder [OK])
- Eventuell im Menü Ansicht die Option Neu zeichnen wählen. Der entsprechende Winkel wird am zuerst gewählten Segment angezeigt.

**Ergänzende Informationen**
⇨ "Innenwinkel zwischen zwei Segmenten ausrichten"

### Innenwinkel zwischen zwei Segmenten ausrichten

Wenn Sie eine Außenkontur und mindestens eine Innenkontur definiert haben (es können auch mehrere Außenkonturen und keine Innenkontur sein), so können Sie diese Konturen mit diesem Werkzeug zueinander positionieren. Mit diesem Werkzeug können Sie Innenwinkel auch vermaßen:

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie ein Segment einer Kontur mit der Maus. Die Kontur, die dieses Segment enthält, wird sich später entsprechend der eingegebenen Vermaßung bewegen.
3. Markieren Sie ein Segment einer zweiten Kontur mit der Maus. Diese Kontur stellt für die Vermaßung die Bezugsgröße dar und ändert ihre Lage nicht.
4. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
5. Bei einer aktiven Vermaßung geben Sie im Wertefenster den Winkel in Grad ein.
6. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].
7. Wählen Sie Neu zeichnen im Menü Ansicht, um eine Auswertung der aktiven Vermaßung zu erzwingen und um die Skizze von A+W CAD Designer (Shapes) übersichtlicher vermaßen zu lassen.

**Beispiel:**
*Abb. A-185 Innenwinkel zwischen zwei Segmenten vermaßen (2)*

Wenn Sie in der Ansicht Skizze eine Außenkontur (Rechteck), und eine Innenkontur (Dreieck) erstellt haben, dann können Sie diese Konturen in der Ansicht Innenkonturen zueinander positionieren:
- Abstand eines Punktes vermaßen (Abstand des Dreiecks in X- und Y-Richtung von der Außenkontur).
- Werkzeug anklicken.
- Unteres Segment des Dreiecks markieren.
- Basissegment des Rechtecks markieren.
- Winkel angeben (20°).
- Eingabe bestätigen (<ENTER> oder [OK]).

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"
⇨ "Abstand zwischen einem Punkt und einer Strecke vermaßen"
⇨ "Innenwinkel zwischen zwei Segmenten vermaßen"

### Zwei Segmente parallel zueinander vermaßen

Mit diesem Werkzeug können Sie zwischen zwei Segmenten, in welcher Lage sie auch immer gezeichnet wurden, eine Parallelitätsbeziehung aufstellen. In der Ansicht Skizze können Sie dieses Werkzug zur Vermaßung einer Kontur nutzen. In der Ansicht Innenkonturen ermöglicht Ihnen dieses Werkzeug, zwei Konturen zueinander zu positionieren.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Wählen Sie das 1. Segment aus. Dieses färbt sich rot.
3. Wählen Sie nun das zu dem 1. Segment parallele Segment aus. Dieses färbt sich grün.
4. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].
6. Wenn Sie sich in der Ansicht Innenkonturen befinden, können Sie sich durch einen Klick auf den Befehl Neu zeichnen im Menü Ansicht die aktuelle Zeichnungslage anzeigen lassen.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Zwei Segmente senkrecht zueinander vermaßen

Hiermit können Sie eine rechtwinklige Beziehung zwischen zwei Segmenten aufstellen. Diese zwei Segmente dürfen sich, müssen sich aber nicht berühren. In der Ansicht Skizze können Sie dieses Werkzug zur Vermaßung einer Kontur nutzen. In der Ansicht Innenkonturen ermöglicht Ihnen dieses Werkzeug, zwei Konturen zueinander zu positionieren.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Wählen Sie das 1. Segment aus. Dieses färbt sich rot.
3. Wählen Sie das zu dem 1. Segment senkrechte Segment aus. Dieses färbt sich grün.
4. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

**Beispiel:**
*Abb. A-186 Vermaße zwei Segmente senkrecht zueinander*

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

## Kreise und Bögen vermaßen

Zur Vermaßung von Kreisen und Bögen stehen Ihnen folgende Funktionen zur Verfügung:

*Tab. A-17 Werkzeuge zum Vermaßen von Kreisen und Bögen*

| Symbol | Kurzname | Beschreibung |
| --- | --- | --- |
| | DSTPTCNT | ⇨ "Abstand zwischen einem Endpunkt und dem Zentrum eines Bogens bestimmen" |
| | DSTSGCNT | ⇨ "Abstand zwischen einer Geraden und einem Bogenmittelpunkt vermaßen" |
| | DSTSGARC | ⇨ "Abstand zwischen einer Strecke und einem Bogenumfang vermaßen" |
| | DSTARCAC | ⇨ "Abstand der Scheitelpunkte zweier Kreise vermaßen" |
| | DSTCTARC | ⇨ "Abstand des Mittelpunktes eines Kreises zum Scheitelpunkt eines anderen vermaßen" (ab Version 3.11) |
| | DSTCTCT | ⇨ "Abstand der Mittelpunkte zweier Kreise vermaßen" |
| | CEILARC | ⇨ "Bogenhöhe vermaßen" |
| | PRJSGCNT | ⇨ "Parallelen Abstand zwischen einem Bogenmittelpunkt und dem Endpunkt vermaßen" |
| | RADARC | ⇨ "Radius eines Bogens vermaßen" |
| | SECNTARC | ⇨ "Sekantenlänge eines Bogens vermaßen" |
| | ARCLEN | ⇨ "Länge eines Bogens vermaßen" (ab Version 3.12) |
| | TANG2ARC | ⇨ "Glatten Übergang zwischen zwei Bögen mit gleichem Radius vermaßen" |

### Abstand zwischen einem Endpunkt und dem Zentrum eines Bogens bestimmen

Mit diesem Werkzeug bestimmen Sie die Entfernung zwischen dem Mittelpunkt eines Kreisbogens und einem beliebigen Konturpunkt, der nicht direkt mit dem Kreisbogen verbunden ist (sonst würde man den Radius bestimmen).

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie den Kreisbogen, dessen Zentrum Sie vermaßen möchten. Dieser färbt sich rot.
3. Wählen Sie den freien Konturpunkt. Dieser wird grün dargestellt.
4. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
5. Bei einer aktiven Vermaßung geben Sie im Wertefenster die Entfernung zwischen dem Kreisbogenzentrum und dem gewählten Konturpunkt ein.
6. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Das von Ihnen eingegebene Maß wird in die Zeichnung übernommen.

**Beispiel:**
*Abb. A-187 Abstand: Endpunkt - Zentrum eines Bogens bestimmen*

**Vermaßungsvorschlag mit 8 Maßen:**
- 2 x Länge einer Geraden vermaßen. Seite a: 250 mm, Seite c: 200 mm.
- 1 x Zwei Segmente parallel zueinander vermaßen, Seite a und c.
- 2 x Abstand zwischen einem Punkt und einer Strecke vermaßen. Länge des Lotes vom Konturpunkt E auf die Gerade a = 500 mm und Länge des Lotes vom Konturpunkt B auf die Verlängerung der Geraden a: Eingabe: 250 mm.
- 2 x Abstand zwischen einem Punkt und einem Strecken-Endpunkt parallel zu einer Strecke vermaßen. Entfernung des Punktes B von C in Richtung von a = 100 mm und Entfernung des Punktes B von A in Richtung der Geraden c = 150 mm.
- 1 x Abstand zwischen einem Endpunkt und dem Zentrum eines Bogens bestimmen. Distanz zwischen dem Mittelpunkt des Kreisbogens und dem Punkt B = 300 mm.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Abstand zwischen einer Geraden und einem Bogenmittelpunkt vermaßen

Mit diesem Werkzeug bestimmen Sie die Länge des Lotes vom Mittelpunkt eines Kreisbogens zu einem Geradensegment. D. h., man denkt sich eine Hilfsgerade, die vom Kreismittelpunkt ausgeht und senkrecht auf eine bestimmte Gerade fällt. Diese Länge der Hilfsgeraden wird mit diesem Werkzeug bestimmt.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Wählen Sie nacheinander in beliebiger Reihenfolge das Geradensegment und den gewünschten Kreisbogen an. Das erste angewählte Segment färbt sich rot und das zweite Segment grün.
3. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
4. Bei einer aktiven Vermaßung geben Sie die den Abstand zwischen der Geraden und dem Kreisbogenmittelpunkt ein.
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Das von Ihnen eingegebene Maß wird in die Zeichnung übernommen.

**Beispiel:**
*Abb. A-188 Abstand zwischen einer Geraden und einem Bogenmittelpunkt*

**Vermaßungsvorschlag: es sind 6 Maßangaben erforderlich:**
- 3 x Länge einer Geraden vermaßen. Längenangaben der drei Geradensegmente: 850 mm, 400 mm und 300 mm.
- 2 x Zwei Segmente senkrecht zueinander vermaßen.
- 1 x Abstand zwischen einer Geraden und einem Bogenmittelpunkt vermaßen. Rechtwinklige Distanz zwischen Kreisbogenmittelpunkt und der linken Geraden = 200 mm.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Abstand zwischen einer Strecke und einem Bogenumfang vermaßen

Dieses Werkzeug eignet sich, um die Entfernung zwischen einer beliebigen Geraden und der parallelen Tangente (angelegte Gerade mit derselben Steigung wie die Funktion) eines Kreisbogens zu bestimmen.
⇨ "Abstand zwischen einer Strecke und einem Bogenumfang vermaßen"

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Wählen Sie nacheinander in beliebiger Reihenfolge das Geradensegment und den gewünschten Kreisbogen an. Das erste angewählte Segment färbt sich rot und das zweite Segment grün.
3. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
4. Bei einer aktiven Vermaßung geben Sie im Wertefenster die Entfernung D zwischen dem angeklickten Geradensegment und der nicht sichtbaren Tangente des gewählten Kreisbogens ein.
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Das von Ihnen eingegebene Maß wird in die Zeichnung übernommen.

*Abb. A-189 Abstand zwischen einer Strecke und einem Bogenumfang vermaßen*
*A beliebige Geraden*
*B parallele Tangenten*

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Abstand der Scheitelpunkte zweier Kreise vermaßen

Mit diesem Werkzeug bestimmen Sie die Entfernung vom Scheitelpunkt eines Kreisbogensegments zum Scheitelpunkt eines anderen Kreisbogensegments. Dies ist die Summe dem Abstand der Mittelpunkte und den beiden Radien.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Klicken Sie nacheinander die Kreisbogensegmente mit der Maus an. Das zuerst angewählte Kreisbogensegment färbt sich rot, das zweite grün.
3. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
4. Bei einer aktiven Vermaßung geben Sie im Wertefenster den Abstand ein.
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Abstand des Mittelpunktes eines Kreises zum Scheitelpunkt eines anderen vermaßen

Mit diesem Werkzeug bestimmen Sie die Entfernung vom Scheitelpunkt eines Kreisbogensegmentes zum Mittelpunkt eines anderen Kreisbogensegmentes.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Klicken Sie nacheinander das Kreisbogensegment, dessen Kreismittelpunkt Sie für die Vermaßung verwenden möchten und dann das Kreisbogensegment, dessen Scheitelpunkt für die Vermaßung verwendet werden soll mit der Maus an. Das erste angewählte Kreisbogensegment färbt sich rot und das zweite grün.
3. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
4. Bei einer aktiven Vermaßung geben Sie im Wertefenster den Abstand ein.
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Abstand der Mittelpunkte zweier Kreise vermaßen

Mit diesem Werkzeug bestimmen Sie die Entfernung vom Mittelpunkt eines Kreisbogensegmentes zum Mittelpunkt eines anderen Kreisbogensegmentes.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Klicken Sie nacheinander die Kreisbogensegmente mit der Maus an. Das erste angewählte Kreisbogensegment färbt sich rot und das zweite grün.
3. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
4. Bei einer aktiven Vermaßung geben Sie im Wertefenster den Abstand ein.
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Bogenhöhe vermaßen

Mit diesem Werkzeug können Sie die Bogenhöhe eines Kreisbogensegmentes bestimmen. Unter der Bogenhöhe versteht man die maximale Entfernung des Kreisbogensegmentes von der Bogensehne, die sich aus der Verbindung der beiden Kreisbogenendpunkte ergibt.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie den zu vermaßenden Kreisbogen. Im Wertefenster wird ein Vorgabewert für die Bogenhöhe angezeigt.
3. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
4. Bei einer aktiven Vermaßung geben Sie unter D die Bogenhöhe ein.
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

**Beispiel:**
*Abb. A-190 Vermaße Bogenhöhe*

**Vermaßungsvorschlag:**
- Geradensegment anklicken und Länge eingeben: 1000 mm.
- Bogensegment anklicken und Bogenhöhe angeben: 288,675 mm.
oder:
- Bogensegment anklicken und Bogenhöhe angeben: 288,675 mm.
- Bogensegment anklicken und Sekantenlänge angeben: 1000 mm.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ "Radius eines Bogens vermaßen"
⇨ Tutorial, "Wertefenster (D)"

### Parallelen Abstand zwischen einem Bogenmittelpunkt und dem Endpunkt vermaßen

Stellen Sie sich ein Lot vom Mittelpunkt eines Kreisbogens auf ein Geradensegment vor. Den Abstand zwischen dem Schnittpunkt des Lotes mit der Geraden und einem Konturpunkt der Geraden können Sie mit diesem Symbol bestimmen.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Wählen Sie zuerst das Kreisbogensegment an, dessen Bogenmittelpunkt Sie vermaßen möchten. Dieses färbt sich rot.
3. Wählen Sie danach den Endpunkt einer Strecke an. Dieser färbt sich grün.
4. Markieren Sie zuletzt die Strecke, zu der parallel vermaßt wird. Diese erscheint hellgrau.
5. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
6. Bei einer aktiven Vermaßung geben Sie die zu der markierten Strecke parallele Entfernung zwischen dem Bogenmittelpunkt des angewählten Kreisbogensegmentes und dem gewählten Strecken-Endpunkt im Wertefenster ein.
7. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Das von Ihnen eingegebene Maß wird in die Zeichnung übernommen.

**Beispiel:**
*Abb. A-191 Parallelen Abstand zwischen einem Bogenmittelpunkt und dem Endpunkt vermaßen*

**Vermaßungsvorschlag: 6 Maßangaben werden benötigt:**
- 3 x Länge einer Geraden vermaßen. Längenangaben der drei Geradensegmente: 600, 200 und 400 mm.
- 1 x Innenwinkel zwischen zwei angrenzenden Segmenten vermaßen. Winkelangabe 120°.
- 1 x Abstand zwischen einer Geraden und einem Bogenmittelpunkt vermaßen. Rechtwinklige Distanz zwischen Kreisbogenmittelpunkt und der linken Geraden: 225 mm.
- 1 x Parallelen Abstand zwischen einem Bogenmittelpunkt und dem Endpunkt vermaßen. Entfernung zwischen dem oberen linken Konturpunkt und dem Lot des Kreisbogenmittelpunktes auf die linke Gerade: 325 mm.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Radius eines Bogens vermaßen

Mit diesem Werkzeug können Sie den Radius eines Kreisbogens eingeben.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie den zu vermaßenden Kreisbogen. Dieser färbt sich rot.
3. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
4. Bei einer aktiven Vermaßung geben Sie im Wertefenster bei R den Radius ein.
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Sekantenlänge eines Bogens vermaßen

Hiermit bestimmen Sie die Sekantenlänge eines Bogens, also die Entfernung zwischen den beiden Endpunkten eines Kreisbogensegmentes. Man spricht auch von der Bogensehne.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie den zu vermaßenden Kreisbogen.
3. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
4. Bei einer aktiven Vermaßung geben Sie im Wertefenster bei S die Sekantenlänge ein.
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

**Beispiel:**
*Abb. A-192 Sekantenlänge eines Bogens vermaßen*

**Vermaßungsvorschlag Sekantenlänge:**
- Die Länge a = 500 mm ist die Sekantenlänge
- Strecke b = 250 mm ist die Bogenhöhe.

**Ergänzende Informationen**
⇨ "Bogenhöhe vermaßen"
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Länge eines Bogens vermaßen

Mit diesem Vermaßungswerkzeug lässt sich die exakte Länge eines Bogensegmentes von seinem Startpunkt bis zu seinem Endpunkt bestimmen.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Klicken Sie das zu vermaßende Bogensegment mit der Maus an. Das ausgewählte Bogensegment wird nun vorläufig in rot dargestellt.
3. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
4. Bei einer aktiven Vermaßung geben Sie im Wertefenster die Bogenlänge ein.
5. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

### Glatten Übergang zwischen zwei Bögen mit gleichem Radius vermaßen

Einen glatten Übergang zwischen zwei Bögen zu bestimmen bedeutet, dass die Winkeländerung in dem gemeinsamen Endpunkt zwischen den Bögen gleich Null wird. Diese Option ist dann sinnvoll, wenn ein Kreisbogen mit einer Winkelöffnung größer als 180° erstellt werden muss. Da nämlich ein Kreisbogen bei der Konstruktion einen maximalen Öffnungswinkel von 180° aufweisen kann, muss ein Kreis größerer Winkelöffnung aus zwei solchen Segmenten aufgebaut sein. Diese beiden Segmente verbindet man mit diesem Werkzeug, welches eine Tangentenbeziehung zwischen den beiden Bögen aufstellt und ebenso die Radien auf einen Wert setzt.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie die beiden gleichzusetzenden Bögen. Der erste färbt sich rot, der zweite grün.
3. Vergeben Sie dem Maß eine Eigenschaft (aktiv, messend, fixiert).
4. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Der von Ihnen ausgewählte tangentiale Übergang wird in die Zeichnung übernommen.

**Beispiel:**
*Abb. A-193 Glatter Übergang zwischen zwei Bögen*

Im obigen Beispiel ist ein Kreisbogen mit einem Öffnungswinkel von 240° und einem Radius von 400 mm konstruiert. Dazu müssen Sie zwei Kreisbögen aneinander reihen (z. B. einen Bogen mit 180° und den anderen mit 60° vermaßen) und mit dem Werkzeug ihre Werte angleichen. Beachten Sie, dass nur für einen Bogen der Radius anzugeben ist.

**Ergänzende Informationen**
⇨ "Eigenschaften von Vermaßungen"
⇨ Tutorial, "Wertefenster (D)"

## Automatisch vermaßen

Zum automatischen Vermaßen stellt Ihnen A+W CAD Designer (Shapes) folgende Funktionen zur Verfügung:

*Tab. A-18 Werkzeuge zum automatischen Vermaßen*

| Symbol | Kurzname | Beschreibung |
| --- | --- | --- |
| | XDIMABS | ⇨ "Automatisch auf Nullpunkt vermaßen" |
| | XDIMREL1 | "Automatisch relativ zueinander vermaßen" |
| | XDIMCONT | ⇨ "Skizze automatisch vermaßen" |
| | XDIMFRME | ⇨ "Segmentlängen und Innenwinkel automatisch vermaßen" |
| | XDIMRELO | "Automatisch auf die linke untere Ecke der Kontur vermaßen" |
| | XDIMDRL | ⇨ "Bohrungen mit Kontur und Referenzpunkt automatisch vermaßen" |

### Automatisch auf Nullpunkt vermaßen

Mit diesem Werkzeug können Sie alle Segmente einer Kontur automatisch vermaßen. Die Vermaßung erfolg in Bezug auf den Nullpunkt. Es werden alle Punkte der Kontur mit X- und Y-Werten angezeigt, bezogen auf den Nullpunkt. Bei Bögen wird der jeweilige Radius angegeben.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie ein Segment der Kontur, die Sie vermaßen möchten. Dieses färbt sich rot.
3. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Vermaßung werden automatisch dargestellt.

### Automatisch relativ zueinander vermaßen

Mit diesem Werkzeug können Sie alle Segmente einer Kontur automatisch relativ zueinander im Uhrzeigersinn vermaßen.

Sie müssen nicht jedes Segment einzeln anwählen sondern Sie markieren lediglich ein Segment der Kontur. Die Vermaßungen werden so gewählt, dass die Kontur ausreichend und korrekt vermaßt ist. Wenn Sie in der Ansicht Skizze eine Kontur mit Hilfe der Segmenterfassung maßstäblich korrekt eingegeben haben, liefert dieses Werkzeug eine passende Vermaßung.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie ein Segment der Kontur, die Sie vermaßen möchten. Dieses färbt sich rot.
3. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Vermaßung der Kontur wird automatisch dargestellt.

### Skizze automatisch vermaßen

Mit diesem Werkzeug können Sie Skizzen automatisch vermaßen. Sie müssen nicht jedes Segment einzeln anwählen sondern Sie markieren lediglich ein Segment der Kontur. Neben den Maßen werden auch Eigenschaften angezeigt, z. B. Rechtwinkligkeit, parallele Segmente, etc. Die Vermaßungen werden so gewählt, dass die Kontur ausreichend und korrekt vermaßt ist. Wenn Sie in der Ansicht Skizze eine Kontur mit Hilfe der Segmenterfassung maßstäblich korrekt eingegeben haben, liefert dieses Werkzeug eine passende Vermaßung.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie ein Segment der Kontur, die Sie vermaßen möchten. Dieses färbt sich rot.
3. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Vermaßung der Kontur wird automatisch dargestellt.

### Segmentlängen und Innenwinkel automatisch vermaßen

Mit diesem Werkzeug können Sie Konturen in Bezug auf Segmentlängen und Innenwinkel automatisch vermaßen. Sie müssen nicht jedes Segment einzeln anwählen sondern Sie selektieren lediglich ein Segment.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie ein beliebiges Segment der Kontur, die Sie vermaßen möchten. Das selektierte Segment färbt sich rot.
3. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Vermaßung der Kontur wird automatisch dargestellt.

### Automatisch auf die linke untere Ecke der Kontur vermaßen

Mit diesem Werkzeug können Sie Konturen in Bezug auf die linke untere Ecke der Kontur automatisch vermaßen. Es werden alle Punkte der Kontur mit X- und Y-Werten, bezogen auf die linke, untere Ecke, angezeigt, jeder Bogen mit seinem Radius.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie ein beliebiges Segment der Kontur, die Sie vermaßen möchten. Das selektierte Segment färbt sich rot.
3. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Vermaßung der Kontur wird automatisch dargestellt.

### Bohrungen mit Kontur und Referenzpunkt automatisch vermaßen

Mit diesem Werkzeug können Sie Bohrungen in Bezug zu einem Referenzpunkt automatisch vermaßen.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Markieren Sie ein Segment der Kontur, in der sich die zu vermaßenden Bohrungen befinden. Das Segment färbt sich rot.
3. Markieren Sie den Referenzpunkt. Dieser färbt sich grün.
4. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Vermaßung der Kontur wird automatisch dargestellt.

## Bohrlöcher erfassen und vermaßen

Um Bohrlöcher zu erfassen und zu vermaßen stehen Ihnen folgende Funktionen zur Verfügung:

*Tab. A-19 Werkzeuge zum Erfassen und Vermaßen von Bohrlöchern*

| Symbol | Kurzname | Beschreibung |
| --- | --- | --- |
| | DRILLHOLE | ⇨ "Neues Bohrloch durch Handeingabe erfassen" |
| | CPDRILL | ⇨ "Neues Bohrloch durch Eingabe von X- und Y-Abstand zu bestehendem Bohrloch erfassen" |
| | DRLSTLEN | ⇨ "Bohrungen auf einem Bogen mit gleichen Abständen erfassen" |
| | DRILLTXT | ⇨ "Bohrlochdurchmesser angeben" |
| | DRILLDIM | ⇨ "Bohrloch mit Vermaßung erfassen" |
| | DRLSTANG | ⇨ "Bohrungen auf einem Kreisbogen mit gleichem Winkelabstand erfassen" |
| | HOLETOCB | ⇨ "Konvertiere Bohrloch zur Senkbohrung" |
| | CNTSINK | ⇨ "Senkbohrung mit Einsenkdurchmesser eingeben" |
| | CNTSINKT | ⇨ "Senkbohrung mit Einsenktiefe eingeben" |
| | CNTSDDIM | ⇨ "Senkbohrung mit Einsenkdurchmesser und Segmentabständen erfassen" |
| | CNTSTDIM | ⇨ "Senkbohrung mit Einsenktiefe und Segmentabständen erfassen" |
| | DRILLSTP | ⇨ "Stufenbohrung eingeben" |
| | DRSTPDIM | ⇨ "Stufenbohrung mit Lagevermaßung eingeben" |

### Neues Bohrloch durch Handeingabe erfassen

Mit dieser Option können Sie in einer fertig vermaßten Kontur ein Bohrloch definieren. Es bestehen zwei Möglichkeiten, die Position des Bohrloches festzulegen: Entweder gibt man bei der Erstellung des Bohrloches die exakten Koordinaten des Lochmittelpunktes an oder man ignoriert diese Koordinaten und bestimmt zunächst lediglich den Bohrlochdurchmesser. Die Innenkontur wird dann in den nächsten Schritten (z. B. zur Außenkontur hin) ausgerichtet.

1. Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2. Klicken Sie mit der linken Maustaste an der Stelle, wo Sie den Mittelpunkt des Bohrloches grob positionieren möchten, oder geben Sie im Wertefenster in den Feldern x und y die exakten X- und Y-Koordinaten der Position ein. Das Bohrloch wird nun vorläufig hellgrau dargestellt.
3. Geben Sie im Wertefenster den Durchmesser des Bohrloches an.
4. Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Das von Ihnen ausgewählte Bohrloch wird nun erzeugt und in der Segmentfarbe (normal schwarz) endgültig dargestellt. Der Durchmesser des Bohrloches wird als Text an diesem angebracht.

> **i Bohrloch mit und ohne Text möglich!**
> Wenn Sie keinen Text am Bohrloch wünschen, können Sie diesen löschen. Weiterhin ist es möglich, mit dem Textwerkzeug Bohrlochdurchmesser angeben einen beliebigen Text an das Bohrloch anzubringen. Ein gelöschter Bohrlochdurchmesser kann mit dem Werkzeug Bohrlochdurchmesser angeben wieder angebracht werden.

**Zum Ausrichten existieren unter anderem folgende Werkzeuge:**
⇨ "Abstand zwischen einem Punkt und einem Strecken-Endpunkt parallel zu einer Strecke vermaßen"
⇨ "Abstand zwischen einem Punkt und einer Strecke vermaßen"
⇨ "Abstand zwischen zwei Punkten parallel zu einer Strecke vermaßen"
⇨ "Abstand zwischen zwei Punkten senkrecht zu einer Strecke vermaßen"

