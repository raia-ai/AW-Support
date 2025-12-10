---
title: "DE-HB-AWCADDesignerShapes_5"
source: "DE-HB-AWCADDesignerShapes_5.pdf"
tags: ["A+W CAD Designer", "Shapes", "CAD Software", "Benutzerhandbuch", "Software-Referenz", "Konturerfassung", "Digitalisierung", "Vermaßung", "Werkzeuge"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for A+W CAD Designer (Shapes). It details the functions available in the \"Ansichten\" (Views), \"Fenster\" (Window), and \"Hilfe\" (Help) menus, providing instructions on how to manipulate the display, manage dimensions, and access help resources. A significant portion of the manual is dedicated to the \"Werkzeuge\" (Tools) section, offering a comprehensive overview and detailed instructions for contour capturing, dimensioning, editing contours, and other specialized functions for glass, window, and door design."
long_description: "This is a comprehensive software reference manual for the German-language version of A+W CAD Designer (Shapes), a specialized CAD program for the glass, window, and door industry. The document is structured into several key chapters. The \"Ansichten\" (Views) chapter explains how to alter the appearance of the design screen, manage the visibility of elements, and control dimensioning display options. The \"Fenster\" (Window) and \"Hilfe\" (Help) chapters cover window management for multiple open files and how to use the built-in help system. The largest and most detailed chapter, \"Werkzeuge\" (Tools), serves as a complete guide to all available tools. It is broken down into functional groups, including tools for contour capturing (via digitizing tables, virtual digitizing from photos, or importing files), creating and dimensioning sketches, smoothing and modifying contours, and specialized tools for corner processing, inner contours, surface treatments, and technology-specific settings (e.g., cutting paths). The manual provides step-by-step instructions, explains parameters in dialog boxes, and includes illustrations to clarify complex operations. It is intended for users who need to create, edit, and prepare complex shapes for production."
---

# Softwarereferenz

# Ansichten

Hier sind alle Funktionen versammelt, die das Aussehen des A+W CAD Designer (Shapes) Bildschirms oder die Sichtbarkeit von bestimmten Elementen verändern.

Dieses Menü enthält außerdem Funktionen, mit denen die Darstellung der gezeigten Informationen verändert werden kann. So können Sie z. B. umschalten zwischen der Maßdarstellung in Zoll (inch) oder mm, oder Sie können die momentane Zeichnung nach einer neuen Vermaßung auf den aktuellen Stand bringen.

Das Menü Ansicht beinhaltet folgende Funktionen:

Folgende Optionen stehen unter Transformieren zur Verfügung:

- **Vermaßungen anzeigen**:
  Die Funktion Vermaßungen anzeigen bietet beim Anklicken folgende Optionen:
  - alle Vermaßungen anzeigen
  - Vermaßungen aus dieser Ansicht anzeigen
  - nur wichtige Vermaßungen anzeigen
  - keine Vermaßungen anzeigen

  Da die erste und letzte Funktion sich selbst erklären, werden hier nur die zweite und dritte Option beschrieben.

  - **Vermaßungen aus dieser Ansicht anzeigen**
    Hier werden nur die Vermaßungen angezeigt, welche in der aktuellen Ansicht erstellt wurden. So sieht man z. B. in der Ansicht Kantenbearbeitung nur die dort erstellten Texte. In der Ansicht Innenkonturen würden dementsprechend nur die Vermaßungen zwischen den Konturen dargestellt. Hier fehlen dann z. B. die Maße aus der Ansicht Skizze, was das Arbeiten bei vielen zu vermaßenden Innenkonturen übersichtlicher macht.
  - **nur wichtige Vermaßungen anzeigen**
    In dieser Funktion werden die Vermaßungen weggelassen, die selbstverständlich sind, jedoch bei der Vermaßung erforderlich waren. Solche selbstverständlichen Vermaßungen sind z. B. Parallelitäts- oder Rechtwinkligkeitsangaben zwischen Konturen oder Segmenten sowie Abstandsvermaßungen zwischen zwei Konturen, die den Wert 0 besitzen (notwendige Angabe, wenn man zwei Konturen aufeinander ausrichten möchte, etwa bei Randausschnitten). Ebenso wird von mehreren Maßen, die den gleichen Wert haben, nur eines angezeigt.

- **Vermaßungen prüfen**:
  Diese Funktion steht in allen Ansichten zur Verfügung, in denen Konturen positioniert werden können (z. B. Innenkonturen). Mit dieser Funktion können Sie prüfen, ob die angegebenen Maße für die positionierten Konturen ausreichend, widersprüchlich oder eindeutig sind. A+W CAD Designer (Shapes) prüft auch, ob zyklische Vermaßung vorliegt und warnt entsprechend. Fehlerhafte Maße werden eingefärbt angezeigt.

> **Wartezeiten vermeiden!**
> Verwenden Sie diese Funktion, wenn Sie umfangreiche Vermaßungen eingegeben haben und bevor Sie in eine andere Ansicht wechseln. So vermeiden Sie lange Wartezeiten, in denen A+W CAD Designer (Shapes) versucht, mathematische Konflikte zu lösen.

- **Auswahl anzeigen**:
  Diese Funktion stellt die auf der Zeichenfläche markierten Objekte in der optimalen Größe dar. Damit können Sie sich ein kleines Segment in der maximalen Größe ansehen und dieses bearbeiten, z. B. um in der Ansicht Revision einen Punkt zu verschieben.
  ⇨ Werkzeuge, "Kontur glätten" auf Seite A-240
  Ist kein Segment ausgewählt, so werden alle Objekte der Zeichenfläche zusammengefasst und in der maximalen Größe dargestellt.

- **Alles anzeigen**:
  Diese Funktion stellt Ihre Zeichnung(en) in der optimalen Größe auf der Zeichenfläche dar. Das ist von Nutzen, wenn Sie Ihre Ansicht schon mehrfach vergrößert oder verkleinert haben und zur Gesamtansicht zurückkehren möchten.

- **Neu zeichnen**:
  Mit dieser Funktion veranlassen Sie A+W CAD Designer (Shapes), die Zeichenfläche neu aufzubauen. Dabei werden alle bisher eingegebenen Vermaßungen ausgewertet und die Konturen entsprechend angepasst und platziert. In der Ansicht Skizze erhalten Sie über diesen Menüpunkt Informationen, ob Ihre Kontur schon ausreichend vermaßt ist.
  ⇨ Werkzeuge, "Skizze erstellen und vermaßen" auf Seite A-236

- **Stückliste aktualisieren**:
  Wenn Sie in einer SN-Datei mit Stückliste weitere Konturen (z. B. Bohrlöcher) zufügen, dann aktualisiert A+W CAD Designer (Shapes) die Stückliste nur bei Bedarf. Verwenden Sie diese Funktion, wenn Sie eine aktuelle Stückliste der Datei benötigen. Diese Funktion wird automatisch durchgeführt, wenn Sie die Datei speichern oder zu einer angeschlossenen Auftragsbearbeitung zurückkehren.

- **Innenkonturen**:
  Mit dieser Funktion können Sie die Darstellung der Innenkonturen ein- oder ausschalten.

- **Ecken beim Schneiden ausführen**:
  Mit dieser Funktion können Sie pro Form die Ausführung von Eckenrundungen und Eckabschnitten im Zuschnitt unterdrücken. Wird ein Glas bestellt und Eckenrundungen/Eckabschnitte werden danach intern auf dem Produkt gefertigt, so wird dies bei der Erzeugung von SN-Dateien berücksichtigt. In diesem Fall wird unter Umständen die Schneideansicht zur Bestimmung der Geometrie des Bestellteils genutzt. Daher werden in diesem Fall Eckenrundungen und Eckabschnitte im Zuschnitt nicht ausgeführt. Bei der Erzeugung von SN-Dateien aus OrderXML wird diese Information in der SN-Datei hinterlegt.

- **Einstellungen**:
  In diesem Menüpunkt können Sie Einstellungen, die sich während eines Programmlaufs mehrfach ändern können, vornehmen. Grundeinstellungen, die sich während der Arbeit mit A+W CAD Designer (Shapes) nicht ändern, werden in der Konfigurationsdatei sn.ini fest eingestellt. Alle außer dem letzten Menüpunkt enthalten weitere Untermenüpunkte.
  ⇨ Werkzeuge, "Maßeinheit auswählen" auf Seite A-523
  ⇨ Werkzeuge, "Kritische Stellen anzeigen" auf Seite A-524
  ⇨ Werkzeuge, "Messpunkte anzeigen" auf Seite A-525
  ⇨ Werkzeuge, "Segmente erfassen" auf Seite A-526
  ⇨ Werkzeuge, "Kritische Stellen anzeigen" auf Seite A-524

- **Werkzeuge**:
  Mit den Einträgen im Untermenü Werkzeuge können Sie die verschiedenen Werkzeugdialoge ein- und ausblenden.
  ⇨ "Werkzeugleiste" auf Seite A-204

---
## Werkzeugleiste

**Ansicht > Werkzeuge > Werkzeugleiste**

*Abb. A-156 Werkzeugleiste*

Die Werkzeugleiste enthält die am häufigsten benötigten Funktionen aus den Menüs Datei und Bearbeiten sowie die Zoomwerkzeuge und den Aufruf der Programminformation.

## Werkzeuge

**Ansicht > Werkzeuge > Werkzeuge**

*Abb. A-157 Werkzeuge*

Je nach dem, in welcher Ansicht Sie sich befinden, zeigt A+W CAD Designer (Shapes) die jeweils sinnvollen (und konfigurierten) Werkzeuge an. Die Beschreibung der Werkzeuge finden Sie unter:

**Ergänzende Informationen**
⇨ Werkzeuge, "Werkzeuge zur Konturerfassung" auf Seite A-219
⇨ Werkzeuge, "Werkzeuge verwenden" auf Seite A-218

## Kante auswählen

**Ansicht Kantenbearbeitung > Werkzeug Sonderkante > Klicken auf ein Segment > [OK]**

*Abb. A-158 Kante auswählen*

Wenn Ihre Installation so eingerichtet ist, dass Sie verschiedene Sonderkanten zur Verfügung haben, dann können Sie mit diesem Dialog festlegen, mit welcher Sonderkante das markierte Segment einer Kontur versehen werden soll.

## Wertefenster

**Ansicht > Werkzeuge > Werte-Fenster**

*Abb. A-159 Wertefenster*

Im Wertefenster geben Sie Bearbeitungsparameter ein. A+W CAD Designer (Shapes) zeigt Ihnen hier Informationen zum markierten Segment, Punkt, Maß oder Bearbeitung an. Werte in roten Feldern können Sie ändern. Schwarze Felder dienen zur Information.

> **Werkzeugdialoge verschieben**
> Werkzeugdialoge können Sie nach Bedarf ein- und ausblenden. Sie können sie an beliebige Stellen am Bildschirm verschieben oder in die Benutzeroberfläche integrieren. Um diese Dialoge in die Benutzeroberfläche zu integrieren, schieben Sie diese an einen Rand der Benutzeroberfläche. Manche Dialoge passen besser an den Rand, andere nach oben oder unten.

**Ergänzende Informationen**
⇨ Tutorial, "Wertefenster (D)" auf Seite A-25

## Textformat

**Ansicht > Werkzeuge > Text-Formatierung**

*Abb. A-160 Textformat*

In den Druckdarstellungen der verschiedenen Ansichten können Sie die Texte auf dem Ausdruck formatieren. Dazu stehen Ihnen die in diesem Dialog angezeigten Formatierungsmöglichkeiten zur Verfügung:

- Schriftart
- Schriftgröße
- Schriftfarbe
- Schriftschnitt fett
- Schriftschnitt kursiv
- Schriftschnitt unterstrichen
- Skalierungstyp für Schrift
  Hier stellen Sie ein, ob Sie eine feste Schriftgröße (Typografische Schriftgröße z. B. 12 Punkt) oder eine an die Größe der Zeichnung angepasste Schriftgröße verwenden wollen (die Schriftgröße wird mit der Zeichnung skaliert).

## Striche und Füllungen

**Ansicht > Werkzeuge > Segment-Formatierungen**

*Abb. A-161 Striche und Füllungen*

In den Druckdarstellungen der verschiedenen Ansichten können Sie die Linien auf dem Ausdruck formatieren. Dazu stehen Ihnen die in diesem Dialog angezeigten Formatierungsmöglichkeiten zur Verfügung:

- Strichstärke
- Strichstil (durchgezogen, gestrichelt, gepunktet)
- Farbe des Strichs
- Schraffur (bei einer Fläche)
- Farbe der Schraffur (bei einer Fläche)

## Statusleiste

**Ansicht > Werkzeuge > Statusleiste**

*Abb. A-162 Statusleiste*

In der Statusleiste zeigt A+W CAD Designer (Shapes) Informationen zum ausgewählten Werkzeug oder Informationen zum Programmzustand an.

## BOM Info

**Ansicht > Werkzeuge > Stücklisteninfofenster**

*Abb. A-163 BOM Info*

In diesem Dialog zeigt A+W CAD Designer (Shapes) Informationen zum Produktaufbau (Stückliste) an. Diese Informationen kann A+W CAD Designer (Shapes) nur dann anzeigen, wenn die aktuelle Datei über einen Stücklistenaufbau verfügt. Informationen zur Stückliste finden Sie in der Dokumentation der Auftragsbearbeitung. Für die einzelnen Gläser werden die lokalen Formdaten angezeigt und können verändert werden.

**Ergänzende Informationen**
"Lokale Formdaten" auf Seite A-186

# Fenster

Die Funktionen in diesem Menü sind von Bedeutung, wenn Sie mehrere Dateien gleichzeitig geöffnet haben. Mit den Einträgen in diesem Menü wählen Sie eine Datei zur Bearbeitung aus oder lassen sich alle geöffneten Dateien anzeigen. Folgende Funktionen stehen zur Auswahl:

Folgende Optionen stehen unter Transformieren zur Verfügung:

- **Überlappend**:
  Wählen Sie diese Funktion, um alle geöffneten Dateien überlappend hintereinanderliegend anzuzeigen.
- **Horizontal teilen**:
  Wählen Sie diese Funktion, um alle geöffneten Dateien untereinander anzuzeigen.
- **Vertikal teilen**:
  Wählen Sie diese Funktion, um alle geöffneten Dateien nebeneinander anzuzeigen.
- **Symbole anordnen**:
  Wählen Sie diese Funktion, um alle geöffneten Dateien nebeneinander anzuzeigen.
- **Liste mit Dateinamen**:
  Hier zeigt A+W CAD Designer (Shapes) die Namen aller Dateien an, die momentan geöffnet sind. Klicken Sie auf die Datei, die im Vordergrund angezeigt und bearbeitet werden soll.

# Die Hilfe verwenden

In diesem Menü finden Sie Hilfen und allgemeine Informationen zu A+W CAD Designer (Shapes).

- **Inhalt**:
  Damit starten Sie die Onlinehilfe.
- **Hilfe zum Objekt**:
  Damit verändern Sie zunächst sie Anzeige des Pfeils (Zeigewerkzeug). Klicken Sie mit dem Zeiger dann auf ein Werkzeug. A+W CAD Designer (Shapes) startet die Onlinehilfe an der Stelle, an der das entsprechende Werkzeug beschrieben ist.
- **Über A+W CAD Designer (Shapes)**:
  ⇨ “Über A+W CAD Designer (Shapes)" auf Seite A-211.

## Über A+W CAD Designer (Shapes)

**? > Über CAD Designer (Shapes) ...**

*Abb. A-164 CAD Designer 5*

In dieser Dialogbox wird die aktuelle Programmversion angezeigt.

**Schaltflächen**

- **OK**: Damit gelangen zu Ihrer aktuellen A+W CAD Designer (Shapes) Sitzung zurück.
- **Systeminfo**: Damit starten Sie den Dialog mit den Systeminformationen ihres Betriebssystems. Informationen dazu entnehmen Sie bitte der Dokumentation ihres Betriebssystems.

---

# Werkzeuge

## In diesem Kapitel finden Sie folgende Themen:

- ⇨ Übersicht
- ⇨ Werkzeuge verwenden
- ⇨ Grundsätzliche Bedienung
- ⇨ Konkrete Fragestellungen

---

### Übersicht
- **Erklärung der Werkzeuge**: A-217
- **Bedienung allgemein**: A-217
- **Arbeiten mit konkreten Fragestellungen**: A-217

### Werkzeuge verwenden: A-218

### Werkzeuge zur Konturerfassung
- **Digitalisieren mit dem Digitalisiertisch**: A-220
  - **Punktweise digitalisieren**: A-221
  - **Digitalisieren mit dem Rad**: A-221
  - **Digitalisieren beenden**: A-221
  - **Innenkonturen digitalisieren**: A-222
  - **Bohrlöcher digitalisieren**: A-222
  - **Kritische Stellen**: A-222
- **Modelle und Vorlagen digitalisieren**: A-223
- **Virtuell digitalisieren**: A-234
- **Kontur importieren**: A-235
- **Skizze erstellen und vermaßen**: A-236
- **Kontur glätten**: A-240
- **Kontur verändern**: A-249
- **Unvollständige Konturen schließen**: A-255

### Werkzeuge zur Vermaßung
- **Verschiedene Werkzeuge – ähnliche Vermaßungen**: A-257
- **Reihenfolge der Markierung**: A-257
- **Eigenschaften von Vermaßungen**: A-258
- **Segmente vermaßen**: A-260
- **Winkel vermaßen**: A-276
- **Kreise und Bögen vermaßen**: A-283
- **Automatisch vermaßen**: A-296
- **Bohrlöcher erfassen und vermaßen**: A-299
- **Hilfslinien einfügen**: A-309

### Werkzeuge zur Eckenbearbeitung
- **Radien und Fasen**: A-312
- **Zuspitzen**: A-312
- **Ecke abschneiden**: A-312
- **Ecken runden oder zuspitzen**: A-320

### Werkzeuge zur Bearbeitung von Innenkonturen
- **Ausschnitte als eigene Datei**: A-326
- **Ausschnitte und Bohrungen zuschneiden**: A-326
- **Ausschnittmakros**: A-326
- **Segment symmetrisch teilen**: A-331
- **Ausschnitte anbringen**: A-334

### Werkzeuge für Oberflächen
- **Oberflächenbearbeitungen anbringen**: A-344
- **Flächenentschichtungen anbringen**: A-354
- **Rillenschlifflinien eingeben**: A-356
- **Eine Linie auf dem Modell platzieren**: A-357

### Werkzeuge für Technologien
- **Hilfsschnitte einfügen**: A-359
- **Schneidweg an Ecken festlegen**: A-369
- **Schneidtischansteuerung vorbereiten**: A-372
- **Kontur ausrichten und umschreibendes Rechteck ermitteln**: A-375
- **Kontur vervielfachen**: A-378
- **Spezielle Werkzeuge für Modelle**: A-379
- **Randentschichtungen verbinden**: A-381

### Werkzeuge zur Bearbeitung von Autoglas
- **Startpunkte setzen**: A-382
- **Schneid- und Brechpfade definieren**: A-389
- **Achsen, Anschläge und Sauger positionieren**: A-393
- **Messpunkte setzen**: A-399

### Werkzeuge zur Bearbeitung von Bauglas
- **Ausdruck der Zeichnung bearbeiten**: A-401
- **Planar-Befestigung einfügen**: A-407
- **Kanten bei Einfachglas bearbeiten**: A-412
- **Kanten an VSG/ISO bearbeiten**: A-419
- **Kanten definieren**: A-425
- **ISO- und VSG-Einheiten definieren**: A-428

### Grundsätzliche Bedienung
- **Gummiband**: A-429
- **Zoom (Lupe)**: A-430
- **Das Zeige-Werkzeug (Pfeil)**: A-432
- **Mit Dateien arbeiten**: A-434
- **Allgemeine Funktionen**: A-438
  - **Rückgängig machen oder wieder herstellen**: A-438
  - **Auswählen, Kopieren und Löschen**: A-438
  - **Segmente und Konturen transformieren**: A-439
  - **Mit Gruppen arbeiten**: A-442

### Konkrete Fragestellungen
- **Wie werden Konturen erfasst**: A-446
  - **Kontur-Daten importieren und ergänzen**: A-446
  - **Scheibe als Kontur digitalisieren**: A-449
    - **Digitalisieren mit dem Digitalisiertisch**: A-449
    - **Virtuell digitalisieren**: A-455
  - **Nachbearbeiten in CAD Designer**: A-456
  - **Scheibe als Skizze erfassen**: A-461
  - **Tür mit Ausschnitten und Bohrungen versehen**: A-469
  - **Komplexe Kontur erstellen**: A-476
  - **Mit Modellen arbeiten**: A-480
  - **Mit Variablen arbeiten**: A-482
- **Wie werden Scheiben bearbeitet**: A-488
  - **Zuschnitt vorbereiten**: A-488
  - **Kantenbearbeitung festlegen**: A-490
  - **Ecken bearbeiten**: A-490
- **Wie wird mit Bauglas gearbeitet**: A-491
  - **VSG und ISO**: A-491
- **Wie werden Zeichnungen gedruckt**: A-493
  - **Zeichnung in Worddatei drucken**: A-493
- **Wie ist die Zusammenarbeit mit anderen Programmen**: A-495
  - **Zusammenarbeit mit A+W Enterprise**: A-495
    - **Kopplung über AWBroke**: A-495
    - **Kopplung über SNAuto**: A-503
    - **Verarbeitbare Produkttypen**: A-504
    - **Wichtige Einschränkungen**: A-505
  - **Zusammenarbeit mit A+W Business**: A-508
    - **Modell erfassen und SN-Datei erzeugen**: A-509
    - **Fertige SN-Datei an die Position anhängen**: A-510
    - **Template-Datei verwenden und endgültig vermaßen**: A-510
  - **Zusammenarbeit mit A+W Production**: A-516
- **Über CNC-Dateien**: A-516
- **Über DXF-Dateien**: A-517
  - **Standard DXF**: A-517
  - **CAMDXF**: A-518
- **Über CAMXML-Dateien**: A-519
- **Datenexport**: A-519
- **Darstellung der Zeichnung ändern**: A-523
  - **Anzeige erweitern**: A-524
  - **Segmenterfassung für Experten**: A-526

---
## Übersicht

Das Kapitel Werkzeuge gliedert sich in folgende Teile:

### Erklärung der Werkzeuge
Im diesem Teil finden Sie Erklärungen zum Arbeiten mit den Werkzeugen, die Ihnen A+W CAD Designer (Shapes) zur Verfügung stellt:
- Werkzeuge, "Werkzeuge verwenden" auf Seite A-218

> **Nicht jede Installation hat alle Werkzeuge!**
> In diesem Kapitel sind alle Werkzeuge beschrieben, die zum Zeitpunkt der Veröffentlichung zur Verfügung standen. Verschiedene Werkzeuge stehen nur bei kundenspezifischer Installation oder separater Lizenzierung zur Verfügung. Daher kann es sein, dass in Ihrer Installation nicht alle Werkzeuge verfügbar sind.

### Bedienung allgemein
In diesem Teil erfahren Sie Schritt für Schritt, wie Sie mit A+W CAD Designer (Shapes) grundsätzlich arbeiten. Wenn Sie das erste Mal das Programm starten, sollten Sie zuerst diese grundlegenden Informationen beachten:
- Werkzeuge, "Grundsätzliche Bedienung" auf Seite A-429

### Arbeiten mit konkreten Fragestellungen
- "Wie werden Konturen erfasst" auf Seite A-446
- "Wie werden Scheiben bearbeitet" auf Seite A-488
- "Wie wird mit Bauglas gearbeitet" auf Seite A-491
- "Wie werden Zeichnungen gedruckt" auf Seite A-493
- "Wie ist die Zusammenarbeit mit anderen Programmen" auf Seite A-495

## Werkzeuge verwenden

In diesem Kapitel finden Sie die Beschreibung aller Werkzeuge, die in A+W CAD Designer (Shapes) verfügbar sind.

> **Nicht jede Installation verfügt über alle Werkzeuge!**
> Ihre konkrete Installation kann mit weniger Werkzeugen ausgestattet sein. Wenn Sie ein spezielles Werkzeug vermissen aber benötigen, wenden Sie sich an A+W.

Die Werkzeuge sind hinsichtlich der Aufgabenstellung, für die sie benötigt werden, zusammengefasst. Die folgende Liste zeigt die Gruppen, in die die Werkzeuge zusammengefasst sind:

### Werkzeuge zur Konturerfassung
- ⇨ "Digitalisieren mit dem Digitalisiertisch" auf Seite A-220
- ⇨ "Modelle und Vorlagen digitalisieren" auf Seite A-223
- ⇨ "Skizze erstellen und vermaßen" auf Seite A-236
- ⇨ "Kontur glätten" auf Seite A-240
- ⇨ "Kontur verändern" auf Seite A-249
- ⇨ "Unvollständige Konturen schließen" auf Seite A-255
- ⇨ "Reihenfolge der Markierung" auf Seite A-257
- ⇨ "Eigenschaften von Vermaßungen" auf Seite A-258

### Werkzeuge zur Vermaßung
- ⇨ "Segmente vermaßen" auf Seite A-260
- ⇨ "Winkel vermaßen" auf Seite A-276
- ⇨ "Kreise und Bögen vermaßen" auf Seite A-283
- ⇨ "Automatisch vermaßen" auf Seite A-296
- ⇨ "Bohrlöcher erfassen und vermaßen" auf Seite A-299
- ⇨ "Hilfslinien einfügen" auf Seite A-309
- ⇨ "Radien und Fasen" auf Seite A-312
- ⇨ "Zuspitzen" auf Seite A-312

### Werkzeuge zur Eckenbearbeitung
- ⇨ "Ecke abschneiden" auf Seite A-312
- ⇨ "Ecken runden oder zuspitzen" auf Seite A-320

### Werkzeuge zur Bearbeitung von Innenkonturen
- ⇨ "Ausschnitte als eigene Datei" auf Seite A-326
- ⇨ "Ausschnitte und Bohrungen zuschneiden" auf Seite A-326
- ⇨ "Ausschnittmakros" auf Seite A-326
- ⇨ "Segment symmetrisch teilen" auf Seite A-331
- ⇨ "Ausschnitte anbringen" auf Seite A-334

### Werkzeuge für Oberflächen
- ⇨ "Oberflächenbearbeitungen anbringen" auf Seite A-344
- ⇨ "Flächenentschichtungen anbringen" auf Seite A-354
- ⇨ "Rillenschlifflinien eingeben" auf Seite A-356

### Werkzeuge für Technologien
- ⇨ "Hilfsschnitte einfügen" auf Seite A-359
- ⇨ "Schneidweg an Ecken festlegen" auf Seite A-369
- ⇨ "Schneidtischansteuerung vorbereiten" auf Seite A-372
- ⇨ "Kontur ausrichten und umschreibendes Rechteck ermitteln" auf Seite A-375
- ⇨ "Kontur vervielfachen" auf Seite A-378
- ⇨ "Spezielle Werkzeuge für Modelle" auf Seite A-379
- ⇨ "Randentschichtungen verbinden" auf Seite A-381

### Werkzeuge zur Bearbeitung von Autoglas
- ⇨ "Startpunkte setzen" auf Seite A-382
- ⇨ "Schneid- und Brechpfade definieren" auf Seite A-389
- ⇨ "Achsen, Anschläge und Sauger positionieren" auf Seite A-393
- ⇨ "Messpunkte setzen" auf Seite A-399

### Werkzeuge zur Bearbeitung von Bauglas
- ⇨ "Ausdruck der Zeichnung bearbeiten" auf Seite A-401
- ⇨ "Planar-Befestigung einfügen" auf Seite A-407
- ⇨ "Kanten bei Einfachglas bearbeiten" auf Seite A-412
- ⇨ "Kanten an VSG/ISO bearbeiten" auf Seite A-419
- ⇨ "Kanten definieren" auf Seite A-425
- ⇨ "ISO- und VSG-Einheiten definieren" auf Seite A-428

## Werkzeuge zur Konturerfassung

Für die Konturerfassung bietet A+W CAD Designer (Shapes) grundsätzlich folgende Wege an:

- **Digitalisieren einer Kontur** (eine Geometrie mit dem Digitalisiertisch oder vom Foto digitalisieren)
  - ⇨ "Digitalisieren mit dem Digitalisiertisch" auf Seite A-220
  - ⇨ "Virtuell digitalisieren" auf Seite A-234
- **Import einer Kontur** (z. B. DXF, IGES, CAMXML, ...)
  - ⇨ "Kontur importieren" auf Seite A-235
- **Erstellen und vermaßen einer Skizze**
  - ⇨ "Skizze erstellen und vermaßen" auf Seite A-236

### Digitalisieren mit dem Digitalisiertisch
Je nach Funktionsumfang Ihres Digitalisiertisches können verschiedene Digitalisierungsverfahren angewendet werden. Standardfunktion ist das punktweise Digitalisieren, das von jedem Digitalisiertisch unterstützt wird. Dabei gibt es verschiedene Verfahren, z. B. Digitalisieren mit einer Lupe. Die zweite und einfachste Möglichkeit ist das digitalisieren mit dem Rad (oder Stift). Diese Möglichkeit wird nicht von jedem Digitalisiertisch unterstützt. Digitalisiert wird im A+W CAD Designer (Shapes) in der Ansicht Punkte.

**Ergänzende Informationen**
- ⇨ "Scheibe als Kontur digitalisieren" auf Seite A-449
- ⇨ "Digitalisieren mit dem Digitalisiertisch" auf Seite A-220

#### Punktweise digitalisieren
Wenn Sie punktweise digitalisieren, dann müssen Sie nach dem Setzen der Punkte diese in A+W CAD Designer (Shapes) mit Ausgleichsbögen oder -geraden verbinden. Wenn Sie das Modul Streamingmode besitzen, dann kann das Setzen der Ausgleichsbögen oder -geraden entfallen. Sie können dann direkt nach dem Digitalisieren in die Ansicht Geometrie wechseln. A+W CAD Designer (Shapes) verbindet die Punkte automatisch zu einer Geometrie. Dieses Verfahren setzt voraus, dass Sie genügend Punkte gesetzt haben. Nur mit entsprechend vielen Punkten kann A+W CAD Designer (Shapes) entscheiden, ob es sich bei den Punkten um einen Bogen oder einer Geraden handelt.

Wenn Sie manuell Ausgleichsbögen bzw. -geraden setzen, dann müssen Sie folgende Regeln einhalten:
- Um ein Ausgleichsegment zu setzen müssen Sie prüfen, über welche Punkte sich ein bestimmtes Segment erstreckt. Dies bedeutet, dass eine unbestimmte Anzahl an Punkten eine Gerade bzw. einen Radius beschreiben. Dadurch ist es möglich, dass eine Kante der Kontur aus mehreren Bogensegmenten oder Geradesegmenten bestehen kann. Sind Sie sicher, welches Ausgleichsegment (Ausgleichswerkzeug) Sie benötigen, dann markieren Sie mit dem entsprechenden Werkzeug den ersten Punkt des zu setzenden Segmentes und danach den letzten Punkt dieses Segmentes.
- Um den ersten Ausgleichsbogen bzw. -gerade zu setzen, müssen Sie den ersten digitalisierten Punkt mit dem entsprechenden Werkzeug markieren und in die selbe Richtung weiter arbeiten, wie digitalisiert wurde.
- Bei einem Segmentwechsel (von einem Bogen in den nächsten oder in eine Gerade bzw. umgekehrt) müssen Sie zwischen den beiden Ausgleichssegmenten ein Punkt zur Übergangsberechnung frei lassen.
- Beim Setzen von den Ausgleichsegmenten müssen Sie die Segmente in der Digitalisier-Reihenfolge eingeben. Es ist nicht erlaubt, erst alle Geraden und danach alle Bögen zu setzen oder umgekehrt.

#### Digitalisieren mit dem Rad
Das Digitalisieren mit dem Rad ist die einfachste Art zu digitalisieren, da hier die Punkte von Digitalisiertisch automatisch an A+W CAD Designer (Shapes) gesendet werden. Diese Punkte müssen Sie nicht mit Ausgleichssegmenten in der Ansicht Punkte verbinden. Das Verbinden der Punkte zu einer Skizze erfolgt dadurch, dass Sie nach dem Digitalisieren des letzten Punktes in A+W CAD Designer (Shapes) in die Ansicht Geometrie wechseln.

#### Digitalisieren beenden
Damit A+W CAD Designer (Shapes) weiß, dass eine Kontur fertig digitalisiert ist, müssen Sie als Letztes den zuerst digitalisierten Punkt noch einmal digitalisieren. Dabei wird das Werkzeug für das Digitalisieren automatisch abgewählt. Wenn Sie diesen Punkt nicht exakt treffen, dann können Sie das Werkzeug auch per Hand mit <ESC> abwählen. Das manuelle Abwählen sollten Sie nur verwenden, wenn die Automatik nicht funktioniert hat.

> **Automatik soll korrekte Erfassung sicherstellen!**
> Wenn die Automatik nicht funktioniert besteht die Gefahr, dass die Form beim Digitalisieren verrutscht ist oder bei der Digitalisiereinheit Messprobleme bestehen.

### Innenkonturen digitalisieren
Innenkonturen werden immer nach der Außengeometrie digitalisiert. Dies bedeutet, dass erst die Außengeometrie wie oben beschrieben digitalisiert werden muss. Das Digitalisier-Werkzeug muss zunächst abgewählt sein. Wenn Sie das Digitalisierwerkzeug erneut starten, dann wird dem A+W CAD Designer (Shapes) damit mitgeteilt, dass es sich um eine neue Geometrie handelt.

> **Kontur nicht verschieben!**
> Beachten Sie dabei, dass die Außenkontur vor dem Digitalisieren der Innenkontur nicht verschoben wird, da sonst die Innenkontur ihre richtige Lage verliert.

Handelt es sich um eine normale Innenkontur (keine Bohrung), dann wird die Innenkontur nach dem Digitalisieren wie eine Außengeometrie bearbeitet.

### Bohrlöcher digitalisieren
Bohrlöcher werden immer nach der Außengeometrie digitalisiert. Wollen Sie Bohrlöcher digitalisieren, dann gibt es dafür 2 Methoden:
- Bei der ersten Methode werden 4 Punkte des Kreismantels als Fadenkreuz digitalisiert, d. h., es müssen immer die beiden gegenüberliegenden Punkte nacheinander digitalisiert werden.
- Die zweite Methode verlangt mehrere digitalisierte Punkte auf dem Kreismantel. Die Punkte müssen in Reihenfolge nacheinander gesetzt werden. Damit eine richtige Bestimmung des Bohrdurchmessers durchgeführt werden kann, muss mindestens ein Viertel des Bohrungskreises digitalisiert werden.

**Ergänzende Informationen**
⇨ "Bohrlöcher digitalisieren" auf Seite A-452

### Kritische Stellen
Wenn Sie eine Kontur digitalisiert haben, dann können Sie sich auf der Kontur kritischen Stellen anzeigen lassen. Kritische Stellen sind Punkte an denen kein tangentialer Übergang zwischen einer Geraden und einem Bogen bzw. zwischen 2 Bögen vorhanden ist. Diese kritischen Stellen führen zu unsauberen Kanten, wenn diese von einer Bearbeitungsmaschine bearbeitet werden sollen. Daher können Sie diese kritischen Stellen glätten.
⇨ "Kritische Stellen erkennen und glätten" auf Seite A-457

### Modelle und Vorlagen digitalisieren
Um Konturen mit einem Digitalisiertisch zu erfassen, stehen Ihnen folgende Werkzeuge zur Verfügung:

| Symbol | Kurzname | Beschreibung |
| :--- | :--- | :--- |
| 