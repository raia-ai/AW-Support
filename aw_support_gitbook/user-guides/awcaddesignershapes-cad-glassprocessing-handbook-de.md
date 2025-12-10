---
title: "DE-HB-AWCADDesignerShapes_8"
source: "DE-HB-AWCADDesignerShapes_8.pdf"
tags: ["CAD", "A+W CAD Designer", "Glass Processing", "Technical Manual", "Werkzeuge", "Hilfsschnitte", "Schneidwege", "Autoglas", "Flächenentschichtung", "Software Manual"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a chapter from the A+W CAD Designer (Shapes) user manual, focusing on the various tools available within the software. It provides step-by-step instructions for using tools related to surface modifications, technological cuts, autoglass processing, and quality control."
long_description: "This document serves as a detailed guide to the 'Werkzeuge' (Tools) section of the A+W CAD Designer (Shapes) software. It is intended for users who design and prepare glass shapes for manufacturing. The guide covers a wide array of functionalities, organized into logical sections. It begins with tools for placing surface elements like recessed grips, applications, motifs, stamps, and logos. It then moves to more technical processes such as applying surface delayering ('Flächenentschichtungen') and creating V-groove lines ('Rillenschlifflinien'). A significant portion is dedicated to 'Werkzeuge für Technologien' (Tools for Technologies), which includes instructions for inserting various types of auxiliary cuts ('Hilfsschnitte') to aid in the glass breaking process. The manual also details how to define cutting paths at corners and prepare cutting table controls. Specialized sections for autoglass production cover positioning axes, stops, and suction cups, as well as defining cutting/breaking paths and setting start points for different machines. Finally, it explains how to set measurement points for quality control. Each tool description includes its purpose, an icon, step-by-step usage instructions, and relevant parameters."
---

# Werkzeuge verwenden

---
## Eine Griffmulde auf der Oberfläche platzieren

[Icon]

Mit diesem Werkzeug können Sie auf einem zuvor definierten rechteckigen Bereich eine Griffmulde platzieren.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie den rechteckigen Bereich. Dieser wird in roter Farbe dargestellt und das Wertefenster öffnet sich.
3.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   `^=`: Markieren Sie diese Checkbox, wenn die Griffmulde auf die Oberseite des Glases gemacht werden soll.
    *   `v=`: Markieren Sie diese Checkbox, wenn die Griffmulde auf die Unterseite des Glases gemacht werden soll.
    *   `^v`: Markieren Sie diese Checkbox, wenn die Griffmulde auf die Oberseite und die Unterseite des Glases gemacht werden soll.
4.  Bestätigen Sie Ihre Eingabe mit `<ENTER>` oder [OK].

**Ergänzende Informationen**
⇨ "Rechteckigen Bereich positionieren" auf Seite A-345

## Eine Applikation auf der Oberfläche platzieren

[Icon]

Mit diesem Werkzeug können Sie einem zuvor definierten rechteckigen Bereich eine Applikation zuweisen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie den rechteckigen Bereich. Dieser wird in roter Farbe dargestellt und das Wertefenster öffnet sich.
3.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   `^=`: Markieren Sie diese Checkbox, wenn die Applikation auf die Oberseite des Glases gemacht werden soll.
    *   `v=`: Markieren Sie diese Checkbox, wenn die Applikation auf die Unterseite des Glases gemacht werden soll.
    *   `^v`: Markieren Sie diese Checkbox, wenn die Applikation auf die Oberseite und die Unterseite des Glases gemacht werden soll.
4.  Bestätigen Sie Ihre Eingabe mit `<ENTER>` oder [OK].

---

**Ergänzende Informationen**
⇨ "Rechteckigen Bereich positionieren" auf Seite A-345

## Ein Motiv auf der Oberfläche platzieren

[Icon]

Mit diesem Werkzeug können Sie ein Motiv auf der Oberfläche platzieren.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol. Es öffnet sich der Dialog Öffnen... .
2.  Wählen Sie das Motiv aus, das eingefügt werden soll.
3.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   `<->`: Breite des Motivs
    *   `|<->|`: Höhe des Motivs
    *   `%`: Größe des Motivs in %
    *   `mm`: Größe des Motivs in mm
    *   `x`: x-Position des Motiv-Mittelpunktes
    *   `y`: y-Position des Motiv-Mittelpunktes
    *   `^=`: Markieren Sie diese Checkbox, wenn das Motiv auf der Oberseite des Glases platziert werden soll.
    *   `v=`: Markieren Sie diese Checkbox, wenn das Motiv auf die Unterseite des Glases platziert werden soll.
    *   `^v`: Markieren Sie diese Checkbox, wenn das Motiv auf der Oberseite und der Unterseite des Glases platziert werden soll.
4.  Bestätigen Sie Ihre Eingabe mit `<ENTER>` oder [OK].

> **Format für Motive**
> Das Motiv kann entweder in Form eines Bildes (EMF-Format) oder als externe CAD-Daten (DXF-Format) eingelesen werden.

## Einen Stempel auf der Oberfläche platzieren

[Icon]

Mit diesem Werkzeug können Sie einen Stempel auf der Oberfläche platzieren.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Positionieren Sie den Stempel auf der Oberfläche.
3.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   `#=`: Nummer des Stempels
    *   `^=`: Markieren Sie diese Checkbox, wenn der Stempel auf der Oberseite des Glases platziert werden soll.
    *   `v=`: Markieren Sie diese Checkbox, wenn der Stempel auf die Unterseite des Glases platziert werden soll.
    *   `^v`: Markieren Sie diese Checkbox, wenn der Stempel auf der Oberseite und der Unterseite des Glases platziert werden soll.
4.  Bestätigen Sie Ihre Eingabe mit `<ENTER>` oder [OK].

> **Farbliche Darstellung konfigurieren**
> Für die farbliche Darstellung von Stempeln können Sie eine Standardfarbe hinterlegen. Zusätzlich wird bei der Farbe die Stempelnummer berücksichtigt. Für mehrere Nummernbereiche kann eine abweichende Farbe hinterlegt werden.

## Ein Logo auf der Oberfläche platzieren

[Icon]

Mit diesem Werkzeug können Sie ein Logo auf der Oberfläche platzieren.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Positionieren Sie das Logo auf der Oberfläche.
3.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   `#=`: Nummer des Logos
    *   `^=`: Markieren Sie diese Checkbox, wenn das Logo auf der Oberseite des Glases platziert werden soll.
    *   `v=`: Markieren Sie diese Checkbox, wenn das Logo auf die Unterseite des Glases platziert werden soll.
    *   `^v`: Markieren Sie diese Checkbox, wenn das Logo auf der Oberseite und der Unterseite des Glases platziert werden soll.
4.  Bestätigen Sie Ihre Eingabe mit `<ENTER>` oder [OK].

> **Farbliche Darstellung konfigurieren**
> Für die farbliche Darstellung von Logos können Sie eine Standardfarbe hinterlegen. Zusätzlich wird bei der Farbe die Logonummer berücksichtigt. Für mehrere Nummernbereiche kann eine abweichende Farbe hinterlegt werden.

## Flächenentschichtungen anbringen

Die Vorgehensweise zum Anbringen von Flächenentschichtungen erfolgt in zwei Schritten:
1.  Erzeugen Sie auf dem Glas an einem oder mehreren Segmenten der Außenform einen Randbereich
2.  Markieren Sie diesen Bereich als Flächenentschichtung

Die Werkzeuge zur Flächenentschichtung finden Sie in der Ansicht Innenkonturen. Folgende Werkzeuge stehen zur Verfügung:

| Symbol | Kurzname | Beschreibung |
| :--- | :--- | :--- |
| [Icon] | STRIPE | ⇨ Werkzeuge, "Randbereich an der Außenform erzeugen" auf Seite A-354 |
| [Icon] | STRIPPIN | ⇨ Werkzeuge, "Flächenentschichtung zuweisen" auf Seite A-355 |
*Tab. A-25 Werkzeuge zur Flächenentschichtung*

### Randbereich an der Außenform erzeugen

[Icon]

Mit diesem Werkzeug erzeugen Sie für die Flächenentschichtung einen Randbereich (z. B. Abkleben, Sandstrahlen, etc.) auf dem Glas. Sie können ein oder mehrere Segmente wählen. Der Bereich definiert sich durch die Breite des Streifens und die Ausformung des Streifens am Ende: tangentiale Fortführung, rechtwinkeliger Abschluss oder Abschluss durch Rundung. Dieser Schritt ist notwendig, um anschließend den Bereich als Flächenentschichtung zu markieren.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie den bzw. die Segmente für die Flächenentschichtung.
3.  Geben Sie im Wertefenster folgende Werte an:
    *   `|<x>|`: Breite des Streifens
    *   `|<>|`: Abstand des Streifens von der Kante
    *   `()`: Ausrundung am Anfangspunkt
    *   `_`: Tangentiale Fortführung am Anfangspunkt
    *   `|_`: Senkrechter Abschluss am Anfangspunkt
    *   `()`: Ausrundung am Endpunkt
    *   `_`: Tangentiale Fortführung am Endpunkt
    *   `|_`: Senkrechter Abschluss am Endpunkt
4.  Bestätigen Sie Ihre Eingabe mit `<ENTER>` oder [OK].

### Flächenentschichtung zuweisen

[Icon]

Mit diesem Werkzeug können Sie einem zuvor definierten Randbereich eine Entschichtung zuweisen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie den Randbereich.
3.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   `^=`: Markieren Sie diese Checkbox, wenn die Oberseite des Glases entschichtet werden soll.
    *   `v=`: Markieren Sie diese Checkbox, wenn die Unterseite des Glases entschichtet werden soll.
    *   `^v`: Markieren Sie diese Checkbox, wenn die Oberseite und die Unterseite des Glases entschichtet werden soll.
4.  Bestätigen Sie Ihre Eingabe mit `<ENTER>` oder [OK].

**Ergänzende Informationen**
⇨ "Randbereich an der Außenform erzeugen" auf Seite A-354

## Rillenschlifflinien eingeben

Die Vorgehensweise zum Eingeben von Rillenschlifflinien erfolgt in zwei Schritten:
1.  Erzeugen Sie auf dem Glas eine Linie mit parametrisierbarer Länge
2.  Kennzeichnen Sie diese Linie als Rillenschliff

Die Werkzeuge für Rillenschliffe finden Sie in der Ansicht Innenkonturen. Folgende Werkzeuge stehen zur Verfügung:

| Symbol | Kurzname | Beschreibung |
| :--- | :--- | :--- |
| [Icon] | SINGLINE | ⇨ Werkzeuge, "Eine Linie für Rillenschliff auf der Oberfläche erzeugen" auf Seite A-356 |
| [Icon] | PLACELIN | ⇨ Werkzeuge, "Linie auf Modell platzieren" auf Seite A-357 |
| [Icon] | SURGROOV | ⇨ Werkzeuge, "Eine Linie als Rillenschliff kennzeichnen" auf Seite A-358 |
*Tab. A-26 Werkzeuge für Rillenschliff*

### Eine Linie für Rillenschliff auf der Oberfläche erzeugen

[Icon]

Mit diesem Werkzeug können Sie eine Linie mit parametrischer Länge erzeugen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie die Stelle an, wo die Linie eingefügt werden soll. Mit gedrückter linker Maustaste können Sie die Linie beliebig verschieben. Die Linie wird standardmäßig mit einer Länge von 100 mm angelegt.
3.  Im Wertefenster können Sie den Wert ändern. Sie können auch einen variablen Ausdruck hinterlegen (z. B. H-10). Dann wird sich bei Veränderung der Variablen die Länge des Segments automatisch anpassen.
4.  Bestätigen Sie Ihre Eingabe mit `<ENTER>` oder [OK].

## Eine Linie auf dem Modell platzieren

### Linie auf Modell platzieren

[Icon]

Mit diesem Werkzeug verschieben Sie eine zuvor platzierte Linie auf dem Modell.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die Linie. Diese färbt sich rot ein.
3.  Markieren Sie das Segment, welches als Referenzsegment dient. A+W CAD Designer (Shapes) ändert die Darstellung des Segmentes in einen grünen Pfeil.
4.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   D1: Paralleler Abstand zwischen den beiden markierten Segmenten.
    *   D2: Abstand des Segment-Endpunktes am Ausschnitt zum Nachbarsegment des ausgewählten Segmentes der Außenkontur.
5.  Bestätigen Sie Ihre Eingabe mit `<ENTER>` oder [OK].
6.  Die Linie wird an die gewünschte Stelle verschoben.

### Eine Linie als Rillenschliff kennzeichnen

[Icon]

Mit diesem Werkzeug können Sie eine zuvor platzierte Linie als Rillenschliff kennzeichnen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie die Linie an, die Sie als Rillenschliff kennzeichnen möchten.
3.  Geben Sie im Wertefenster die geforderten Werte ein:
    *   `|<->|`: Höhe des Rillenschliffs
    *   `#=`:
    *   `^=`: Markieren Sie diese Checkbox, wenn sich der Rillenschliff auf der Oberseite des Glases befindet.
    *   `v=`: Markieren Sie diese Checkbox, wenn sich der Rillenschliff auf der Unterseite des Glases befindet.
    *   `^v`: Markieren Sie diese Checkbox, wenn sich der Rillenschliff auf der Oberseite und der Unterseite des Glases befindet.
4.  Bestätigen Sie Ihre Eingabe mit `<ENTER>` oder [OK].

**Ergänzende Informationen**
⇨ "Eine Linie für Rillenschliff auf der Oberfläche erzeugen" auf Seite A-356

## Werkzeuge für Technologien

Je nach dem, welche Konturen Sie schneiden wollen und welche Maschinen Sie einsetzen, bietet A+W CAD Designer (Shapes) eine Reihe von Werkzeugen zur optimalen Maschinenansteuerung. Solche Werkzeuge werden in den Technologieansichten bereitgestellt.

### Hilfsschnitte einfügen

Um Hilfsschnitte einzufügen, stehen Ihnen folgende Werkzeuge zur Verfügung:

| Symbol | Kurzname | Beschreibung |
| :--- | :--- | :--- |
| [Icon] | AUXCTANG | ⇨ "Hilfsschnitt durch Fortsetzung eines Segmentes erfassen" auf Seite A-359 |
| [Icon] | AUXCINTR | ⇨ "Hilfsschnitt durch Verlängerung eines Segmentes erfassen" auf Seite A-361 |
| [Icon] | AUXCORTH | ⇨ "Hilfsschnitt erfassen, um den Bruchrand zu teilen" auf Seite A-362 |
| [Icon] | AUXCPARA | "Hilfsschnitt erfassen, um zwei Konturen zu trennen" auf Seite A-364 |
| [Icon] | CUTRAIL | ⇨ "Neuen tangentialen Einfahrweg für eine Schlepprad-Schneidmaschine eingeben" auf Seite A-365 |
| [Icon] | AUXLOOP | ⇨ "Neuen schleifenförmigen Hilfsschnitt eingeben" auf Seite A-365 |
| [Icon] | AUXCINTC | "Zwei Hilfsschnitte miteinander verbinden" auf Seite A-366 |
| [Icon] | AUXCPERP | ⇨ "Hilfsschnitt senkrecht zur Kontur erzeugen" auf Seite A-366 |
| [Icon] | SATELLIT | "Satellit für freies Brechen" auf Seite A-367 |
*Tab. A-27 Werkzeuge zum Setzen von Hilfsschnitten*

#### Hilfsschnitt durch Fortsetzung eines Segmentes erfassen

[Icon]

Mit diesem Werkzeug bestimmen Sie einen Hilfsschnitt, der tangential zu dem gewählten Segment bis hin zum Glasrand fortgesetzt wird. Der Hilfsschnitt führt von der Kontur bis zum Glasprimitiv (aus dem die Kontur geschnitten wird). Der Hilfsschnitt endet um einen bestimmten Wert vor dem Segment und vor dem Rand. Dieser Wert wurde bei der Installation in der sn.ini eingestellt.

Wenn Sie Konturen ändern (d. h., der Glasrand oder die Lage der Kontur ändert sich), nachdem Sie den Hilfsschnitt eingegeben haben, so behält der Hilfsschnitt selbständig seine zuvor eingestellten Abstände und Ausrichtung bei.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Wählen Sie das Segment an, von dem der Hilfsschnitt ausgehen und in gleicher Steigung weitergeführt werden soll. Das angewählte Segment wird rot markiert dargestellt.
3.  Wählen Sie nun den Rand des Glasprimitives an, in dessen Richtung der Hilfsschnitt weitergeführt werden soll. Die Konturpunkte des gewählten Randes werden grün markiert hervorgehoben.
4.  Bestätigen Sie Ihre Eingabe mit `<ENTER>` oder [OK].

**Beispiel:**

