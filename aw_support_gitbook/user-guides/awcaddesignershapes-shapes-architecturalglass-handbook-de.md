---
title: "DE-HB-AWCADDesignerShapes_9"
source: "DE-HB-AWCADDesignerShapes_9.pdf"
tags: ["A+W CAD Designer", "Shapes", "architectural glass", "CAD software", "technical manual", "glass processing", "DXF import", "digitalization", "edge processing", "VSG", "ISO"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a technical manual for A+W CAD Designer (Shapes), detailing the use of various tools for processing architectural glass. It covers editing drawings, handling different glass types like single, VSG, and ISO, and fundamental CAD operations."
long_description: "This manual provides a comprehensive overview of the tools and functions available in A+W CAD Designer (Shapes) for the design and production of architectural glass. It is structured to guide users through various workflows, from basic drawing modifications to complex edge processing and component definitions. Key sections include 'Werkzeuge zur Bearbeitung von Bauglas' (Tools for Processing Architectural Glass), which details tools for distorting contours, creating detail views, hatching surfaces, and adding text. It also covers specialized tools for inserting planar fastenings and processing edges on single glass, laminated safety glass (VSG), and insulated glass units (ISO), including grinding, polishing, mitering, and applying facets. The 'Grundsätzliche Bedienung' (Basic Operation) section explains core functionalities like file management (opening, saving, importing/exporting), object transformation (moving, rotating, scaling), zoom controls, and working with groups. The final section, 'Konkrete Fragestellungen' (Specific Questions), addresses common user workflows, such as importing contour data from formats like DXF and ESG, and digitizing glass shapes using a digitizing table."
---

# Werkzeuge verwenden

---
## Werkzeuge zur Bearbeitung von Bauglas

Bauglas zeichnet sich durch die große Vielfalt an Konturen und Bearbeitungen bei oft geringster Stückzahl aus. Dabei werden gute Zeichnungen benötigt, mit denen besondere Details eindeutig sichtbar sind. Ausschnitte, Innenkonturen und Stufen bei Mehrfachgläsern (ISO, VSG) müssen abgebildet werden. Bei Fassadengläsern müssen besondere Befestigungssysteme berücksichtigt werden. A+W CAD Designer (Shapes) unterstützt die Bauglasproduktion durch verschiedene Werkzeuggruppen:

*   "Ausdruck der Zeichnung bearbeiten" auf Seite A-401
*   "Planar-Befestigung einfügen" auf Seite A-407
*   "Kanten bei Einfachglas bearbeiten" auf Seite A-412
*   "Kanten an VSG/ISO bearbeiten" auf Seite A-419
*   "Kanten definieren" auf Seite A-425
*   "ISO- und VSG-Einheiten definieren" auf Seite A-428

### Ausdruck der Zeichnung bearbeiten

Die folgenden Werkzeuge sind nur in den Ansichten Zeichnung verfügbar.

| Symbol | Kurzname | Beschreibung |
| --- | --- | --- |
| TEXT | TEXT | ⇨ "Segment beschriften" auf Seite A-239 |
| CONSTRCH | CONSTRCH | ⇨ "Kontur verzerren" auf Seite A-402 |
| DETAILVW | DETAILVW | ⇨ "Detail vergrößern" auf Seite A-402 |
| DRILLSD | DRILLSD | ⇨ "Schnittzeichnung einer Senkbohrung einfügen" auf Seite A-403 |
| SETFILL | SETFILL | ⇨ "Fläche schraffieren" auf Seite A-404 |
| SETSTYLE | SETSTYLE | ⇨ "Beschriftung und Segmente formatieren" auf Seite A-404 |
| TEXTSEG | TEXTSEG | ⇨ "Freien Text in Zeichnung einfügen" auf Seite A-405 |
| SEGSTRCH | SEGSTRCH | ⇨ "Kantenabhängige Randeinzüge bei freien Formen" auf Seite A-406 |
| CUTBACK | CUTBACK | ⇨ "Kantenabhängige Randeinzüge bei freien Formen" auf Seite A-406 |

*Tab. A-38 Werkzeuge zum Bearbeiten einer Zeichnung*

Mit diesen Werkzeugen können Sie die Darstellung der Scheiben auf dem Ausdruck verändern, um Details deutlich zu machen.

### Kontur verzerren

Verwenden Sie dieses Werkzeug, um eine Kontur mit einem ungünstigem Verhältnis von Höhe zu Breite so zu verzerren, dass der Ausdruck gut lesbar ist.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie auf ein Segment, das sie verschieben wollen.
3.  Geben Sie im Wertefenster die gewünschte Verzerrung in mm ein. Ein positiver Wert verschiebt die markierte Seite nach außen, ein negativer Wert nach innen. Alternativ können Sie die Seite auch durch erneutes Klicken und Ziehen mit der Maus an die gewünschte Stelle verschieben.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Zeichnung wird neu erstellt. Die Maße bleiben erhalten, die Darstellung ist jetzt nicht mehr maßstäblich.

**Ergänzenden Informationen**
*   "Zeichnung gestalten" auf Seite A-475
*   "Variablen in der Zeichnung verwenden" auf Seite A-486

### Detail vergrößern

Verwenden Sie dieses Werkzeug, um ein Detail in einer Zeichnung vergrößert darzustellen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie mit der linken Maustaste und halten Sie diese gedrückt. Ziehen sie dabei ein kleines Rechteck um den Bereich, den Sie vergrößern wollen. Ziehen Sie das Rechteck immer von links oben nach rechts unten. Lassen Sie die Maustaste los, wenn das Rechteck die gewünschte Größe hat. A+W CAD Designer (Shapes) zeigt den zu vergrößernden Bereich als blaues Rechteck an.
3.  Suchen Sie sich eine Stelle auf der Zeichnung, an der die Vergrößerung angezeigt werden soll.
4.  Klicken Sie mit der linken Maustaste und halten Sie diese gedrückt. Ziehen sie dabei ein großes Rechteck an der Stelle, an der A+W CAD Designer (Shapes) die Vergrößerung anzeigen soll. Ziehen Sie das Rechteck immer von links oben nach rechts unten. Lassen Sie die Maustaste los, wenn das Rechteck die gewünschte Größe hat. A+W CAD Designer (Shapes) zeigt den Bereich als blaues Rechteck an.
5.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) erstellt eine Vergrößerung und fügt sie an der angegebenen Stelle ein.

**Ergänzenden Informationen**
*   "Zeichnung gestalten" auf Seite A-475

### Schnittzeichnung einer Senkbohrung einfügen

Mit diesem Werkzeug können Sie in eine Zeichnung eine vergrößerte Schnittzeichnung einer Senkbohrung einfügen. Dazu ist es erforderlich, dass der Kontur eine Glasdicke angegeben wurde.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie auf eine Bohrung. A+W CAD Designer (Shapes) zeigt die markierte Bohrung rot.
3.  Suchen Sie sich eine Stelle auf der Zeichnung, an der die vergrößerte Schnittdarstellung erstellt werden soll.
4.  Klicken Sie mit der linken Maustaste und halten Sie diese gedrückt. Ziehen sie dabei ein Rechteck an der Stelle auf, an der A+W CAD Designer (Shapes) die Schnittzeichnung anzeigen soll. Ziehen Sie das Rechteck immer von links oben nach rechts unten. Lassen Sie die Maustaste los, wenn das Rechteck die gewünschte Größe hat. A+W CAD Designer (Shapes) zeigt den Bereich als blaues Rechteck an.
5.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) erstellt die Schnittzeichnung und fügt sie an der angegebenen Stelle ein.

**Ergänzenden Informationen**
*   "Zeichnung gestalten" auf Seite A-475
*   Softwarereferenz, "Globale Formdaten" auf Seite A-167
*   Softwarereferenz, "Lokale Formdaten" auf Seite A-186

### Fläche schraffieren

Verwenden Sie dieses Werkzeug, wenn Sie in einer Zeichnung eine Fläche schraffiert darstellen wollen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Blenden Sie den Dialog Striche und Füllungen ein.
3.  Klicken Sie auf ein Segment der Kontur, die Sie schraffieren wollen.
4.  Stellen Sie die Art der gewünschten Schraffur im Dialog Striche und Füllungen ein.
5.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) füllt die Fläche.

**Ergänzenden Informationen**
*   "Zeichnung gestalten" auf Seite A-475
*   Softwarereferenz, "Striche und Füllungen" auf Seite A-207

### Beschriftung und Segmente formatieren

Verwenden Sie dieses Werkzeug, wenn Sie die Darstellung von Text oder das Aussehen von Segmenten in einer Zeichnung ändern wollen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Blenden Sie die Dialoge Striche und Füllungen und Textformat ein.
3.  Klicken Sie auf ein Segment der Kontur, das Sie umgestalten oder auf einen Text, den Sie umformatieren wollen.
4.  Wenn Sie ein Segment markiert haben, dann stellen Sie die Art der gewünschten Darstellung im Dialog Striche und Füllungen ein.
5.  Wenn Sie Text markiert haben, dann stellen Sie die Art der gewünschten Darstellung im Dialog Textformat ein.
6.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) ändert die Darstellung des Segmentes oder des Textes.

**Ergänzenden Informationen**
*   "Zeichnung gestalten" auf Seite A-475
*   Softwarereferenz, "Striche und Füllungen" auf Seite A-207
*   Softwarereferenz, "Textformat" auf Seite A-207

### Freien Text in Zeichnung einfügen

Mit diesem Werkzeug können Sie einen einzeiligen Text an einer beliebigen Stelle in einer Zeichnung einfügen. Solche Texte können z. B. Überschriften oder Bemerkungen sein.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie an eine beliebige Stelle in der Zeichnung. A+W CAD Designer (Shapes) zeigt in der Zeichnung ein kleines blaues Rechteck an.
3.  Geben Sie im Wertefenster den Text ein, der in der Zeichnung erscheinen soll.
4.  Verschieben Sie die blaue Textbox in der Zeichnung mit der Maus an die gewünschte Position.
5.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

**Ergänzenden Informationen**
*   "Zeichnung gestalten" auf Seite A-475

### Seite verzerrt zeichnen

Verwenden Sie dieses Werkzeug, um ein Segment in einer Zeichnung verzerrt darzustellen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie auf ein Segment in die Nähe eines Segmentpunktes. A+W CAD Designer (Shapes) zeigt den Segmentpunkt rot an und legt um die Kontur ein gestricheltes blaues Rechteck.
3.  Klicken und ziehen Sie mit der Maus das blaue Rechteck und verzerren Sie so die Zeichnung. Alternativ dazu können Sie auch im Wertefenster angeben, um wieviel mm der Segmentpunkt verschoben gezeichnet werden soll.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) erstellt eine verzerrte Zeichnung.

**Ergänzenden Informationen**
*   "Zeichnung gestalten" auf Seite A-475
*   "Variablen in der Zeichnung verwenden" auf Seite A-486

### Kantenabhängige Randeinzüge bei freien Formen

Mit diesem Werkzeug können Sie Randeinzüge für den Rahmen pro Kante hinterlegen. Das Werkzeug gibt es in zwei Varianten (einstellbar über die SN.INI): In der ersten Variante besitzt es die Eingabewerte Rahmenbreite und Versiegelungstiefe, in der zweiten Variante Rahmenbreite und Rückschnitt. Die Werte werden an die Treiber für die ISO Linie ausgegeben. Im A+W CAD Designer (Shapes) ist es möglich, über SN.INI Parameter Standardwerte für den Rückschnitt zu hinterlegen. Dieser wird benutzt, wenn keine Deko auf der Kante ist.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Wählen Sie eine Kante aus. Der A+W CAD Designer (Shapes) zeigt die Kante in rot an.
3.  Geben Sie im Wertefenster die entsprechenden Werte an. Die Eingabewerte für Rahmenbreite und Versiegelungstiefe sind wie folgt:
    CutbackMode=1 (sn.ini)
    *   `->|\|<-`: Wert für die Rahmenbreite
    *   `|\|->`: Wert für die Versiegelungstiefe
    Die Eingabewerte für Rahmenbreite und Rückschnitt sind wie folgt:
    CutbackMode=2 (sn.ini)
    *   `->|\|<-`: Wert für die Rahmenbreite
    *   `->|\|___|`: Wert für den Rückschnitt
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

**Ergänzenden Informationen**
*   "Zeichnung gestalten" auf Seite A-475
*   "Variablen in der Zeichnung verwenden" auf Seite A-486

## Planar-Befestigung einfügen

Für Fassadengläser, die mit dem Befestigungssystem Planar montiert werden, stellt A+W CAD Designer (Shapes) entsprechende Werkzeuge zur Verfügung.

> **Nur im SN4-Modus!**
> Die nachfolgend beschriebenen Werkzeuge funktionieren zur Zeit nur im Kompatibilitätsmodus SN4.

| Symbol | Kurzname | Beschreibung |
| --- | --- | --- |
| PLANAR | PLANAR | ⇨ "Einfache Planar-Bohrung" auf Seite A-407 |
| PLANADIM | PLANADIM | ⇨ "Einfache Planar-Bohrung mit Vermaßung" auf Seite A-408 |
| PAPLANAR | PAPLANAR | ⇨ "Planar mit ESG-Gegenscheibe" auf Seite A-409 |
| PAPLADIM | PAPLADIM | ⇨ "Planar mit ESG-Gegenscheibe mit Vermaßung" auf Seite A-409 |
| PAINTEG | PAINTEG | ⇨ "Integra" auf Seite A-410 |
| PAINTDIM | PAINTDIM | ⇨ "Integra mit Vermaßung" auf Seite A-411 |

*Tab. A-39 Werkzeuge zum Einfügen von Planar-Befestigungen*

Mit diesen Werkzeugen können die erforderlichen Bohrungen und Vermaßungen an Einheiten angebracht werden.

### Einfache Planar-Bohrung

Verwenden Sie dieses Werkzeug, um an Scheiben einer ISO-Einheit die Bohrungen für das Planar-Befestigungssystem anzubringen. Dabei wird eine Senkbohrung an der ersten Scheibe und zylindrische Bohrungen an beliebig vielen weiteren Scheiben angebracht.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie mit der linken Maustaste an der Stelle, wo Sie den Mittelpunkt der Planar-Befestigung grob positionieren möchten, oder geben Sie im Wertefenster in den Feldern x und y die exakten X- und Y-Koordinaten der Position ein. Die Bohrlöcher werden nun vorläufig hellgrau dargestellt. Die Größe der Planar-Bohrungen sind in der Konfiguration festgelegt.
3.  Wählen Sie im linken Eingabefeld, ob die Kontur eine ISO-Einheit, eine Einfachscheibe oder VSG-Einheit ist:
    *   I:I = ISO-Einheit
    *   I = Einfachscheibe oder VSG-Einheit
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Bohrungen werden in die Kontur eingefügt und in der Segmentfarbe dargestellt.

### Einfache Planar-Bohrung mit Vermaßung

Verwenden Sie dieses Werkzeug, um an Scheiben einer ISO-Einheit die Bohrungen für das Planar-Befestigungssystem anzubringen. Dabei wird eine Senkbohrung an der ersten Scheibe und zylindrische Bohrungen an beliebig vielen weiteren Scheiben angebracht. Mit diesem Werkzeug können Sie ein Bohrloch erfassen, dessen Abstand zu zwei Segmenten bekannt ist. Dabei wird jeweils ein senkrechter Abstand vom Segment zum Bohrungszentrum angenommen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie das erste Segment, gegen das Sie das Bohrloch positionieren wollen. Dieses färbt sich rot.
3.  Markieren Sie das zweite Segment, gegen das Sie das Bohrloch positionieren wollen. Dieses färbt sich grün.
4.  Geben Sie den Abstand zum ersten (roten) Segment im Eingabefeld D1 und den Abstand zum zweiten Segment im Eingabefeld D2 ein. Die Größe der Planar-Bohrungen sind in der Konfiguration festgelegt.
5.  Wählen Sie im linken Eingabefeld, ob die Kontur eine ISO-Einheit, eine Einfachscheibe oder VSG-Einheit ist:
    *   I:I = ISO-Einheit
    *   I = Einfachscheibe oder VSG-Einheit
6.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Bohrungen werden in die Kontur eingefügt und in der Segmentfarbe dargestellt.

### Planar mit ESG-Gegenscheibe

Verwenden Sie dieses Werkzeug, um an Scheiben einer ISO-Einheit mit zwei- oder dreischeibigem Giesharz mit ESG-Gegenscheibe die benötigten Bohrungen für das Planar-Befestigungssystem anzubringen. Dabei wird eine Senkbohrung an der ersten Scheibe und zylindrische Bohrungen an beliebig vielen weiteren Scheiben angebracht.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie mit der linken Maustaste an der Stelle, wo Sie den Mittelpunkt der Planar-Befestigung grob positionieren möchten, oder geben Sie im Wertefenster in den Feldern x und y die exakten X- und Y-Koordinaten der Position ein. Die Bohrlöcher werden nun vorläufig hellgrau dargestellt. Die Größe der Planar-Bohrungen sind in der Konfiguration festgelegt.
3.  Wählen Sie im linken Eingabefeld, ob die Kontur eine ISO-Einheit, eine Einfachscheibe oder VSG-Einheit ist:
    *   I:I = ISO-Einheit
    *   I = Einfachscheibe oder VSG-Einheit
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Bohrungen werden in die Kontur eingefügt und in der Segmentfarbe dargestellt.

### Planar mit ESG-Gegenscheibe mit Vermaßung

Verwenden Sie dieses Werkzeug, um an Scheiben einer ISO-Einheit mit zwei- oder dreischeibigem Giesharz mit ESG-Gegenscheibe die benötigten Bohrungen für das Planar-Befestigungssystem anzubringen. Dabei wird eine Senkbohrung an der ersten Scheibe und zylindrische Bohrungen an beliebig vielen weiteren Scheiben angebracht. Mit diesem Werkzeug können Sie ein Bohrloch erfassen, dessen Abstand von zwei Segmenten bekannt ist. Dabei wird jeweils ein senkrechter Abstand vom Segment zum Bohrungszentrum angenommen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie das erste Segment, gegen das Sie das Bohrloch positionieren wollen. Dieses färbt sich rot.
3.  Markieren Sie das zweite Segment, gegen das Sie das Bohrloch positionieren wollen. Dieses färbt sich grün.
4.  Geben Sie den Abstand zum ersten (roten) Segment im Eingabefeld D1 und den Abstand zum zweiten Segment im Eingabefeld D2 ein. Die Größe der Planar-Bohrungen sind in der Konfiguration festgelegt.
5.  Wählen Sie im linken Eingabefeld, ob die Kontur eine ISO-Einheit, eine Einfachscheibe oder VSG-Einheit ist:
    *   I:I = ISO-Einheit
    *   I = Einfachscheibe oder VSG-Einheit
6.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Bohrungen werden in die Kontur eingefügt und in der Segmentfarbe dargestellt.

### Integra

Verwenden Sie dieses Werkzeug, um an Scheiben einer ISO-Einheit mit zwei- oder dreischeibigem Giesharz mit ESG-Gegenscheibe die benötigten Bohrungen für ein verdecktes Planar-Befestigungssystem anzubringen. Dabei wird eine Senkbohrung an der zweiten Scheibe und zylindrische Bohrungen an beliebig vielen weiteren Scheiben angebracht.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie mit der linken Maustaste an der Stelle, wo Sie den Mittelpunkt der Planar-Befestigung grob positionieren möchten, oder geben Sie im Wertefenster in den Feldern x und y die exakten X- und Y-Koordinaten der Position ein. Die Bohrlöcher werden nun vorläufig hellgrau dargestellt. Die Größe der Planar-Bohrungen sind in der Konfiguration festgelegt.
3.  Wählen Sie im linken Eingabefeld, ob die Kontur eine ISO-Einheit, eine Einfachscheibe oder VSG-Einheit ist:
    *   I:I = ISO-Einheit
    *   I = Einfachscheibe oder VSG-Einheit
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Bohrungen werden in die Kontur eingefügt und in der Segmentfarbe dargestellt.

### Integra mit Vermaßung

Verwenden Sie dieses Werkzeug, um an Scheiben einer ISO-Einheit mit zwei- oder dreischeibigem Giesharz mit ESG-Gegenscheibe die benötigten Bohrungen für ein verdecktes Planar-Befestigungssystem anzubringen. Dabei wird eine Senkbohrung an der zweiten Scheibe und zylindrische Bohrungen an beliebig vielen weiteren Scheiben angebracht. Mit diesem Werkzeug können Sie ein Bohrloch erfassen, dessen Abstand von zwei Segmenten bekannt ist. Dabei wird jeweils ein senkrechter Abstand vom Segment zum Bohrungszentrum angenommen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie das erste Segment, gegen das Sie das Bohrloch positionieren wollen. Dieses färbt sich rot.
3.  Markieren Sie das zweite Segment, gegen das Sie das Bohrloch positionieren wollen. Dieses färbt sich grün.
4.  Geben Sie den Abstand zum ersten (roten) Segment im Eingabefeld D1 und den Abstand zum zweiten Segment im Eingabefeld D2 ein. Die Größe der Planar-Bohrungen sind in der Konfiguration festgelegt.
5.  Wählen Sie im linken Eingabefeld, ob die Kontur eine ISO-Einheit, eine Einfachscheibe oder VSG-Einheit ist:
    *   I:I = ISO-Einheit
    *   I = Einfachscheibe oder VSG-Einheit
6.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Die Bohrungen werden in die Kontur eingefügt und in der Segmentfarbe dargestellt.

## Kanten bei Einfachglas bearbeiten

Mit den folgenden Werkzeugen fügen Sie einer Kante eine Bearbeitung zu. Jede Kantenbearbeitung hat einen entsprechenden Bearbeitungszuschlag zur Folge, da die Kontur mit größerer Abmessung geschnitten werden muss, um nach der Bearbeitung das Nennmaß zu haben. Im Menü Kantenbearbeitung wird das entsprechende Symbol an der jeweiligen Kante angezeigt, die Nennmaße bleiben erhalten. In der Ansicht Schneiden wird die Kontur mit den korrigierten (vergrößerten) Maßen angezeigt, die die Kontur nach dem Schneiden und vor dem Kantenbearbeitungsvorgang aufweist.

*   "Kante schleifen" auf Seite A-412
*   "Kante grob justieren" auf Seite A-413
*   "Sonderkante festlegen" auf Seite A-414
*   "Kante polieren" auf Seite A-414
*   "Schnittkante festlegen" auf Seite A-415
*   "Kante säumen" auf Seite A-415
*   "Gehrungskante anbringen" auf Seite A-416
*   "Standardfacette anbringen" auf Seite A-417
*   "Facette mit Neigungswinkel an der Kante anbringen" auf Seite A-417
*   "Sonderfacette anbringen" auf Seite A-418

### Kante schleifen

Mit diesem Werkzeug definieren Sie Segmente einer Kontur als Kante, die fein justiert werden muss. Fein justierte Kanten erhalten einen glasdickenabhängigen Bearbeitungszuschlag. Der Zuschlag ist in der sn.ini eingestellt.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die zu bearbeitende Kante (ein Segment).
3.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Der Bearbeitungszuschlag wird der Kontur zugewiesen und die Bearbeitungskennzeichnung wird an dem Segment angezeigt.

> **Bearbeitung auf angrenzender Segmente übernehmen**
> Bei glatten (tangentialen) Übergängen zwischen dem gewählten und angrenzenden Segmenten wird die jeweilige Kantenbearbeitung automatisch auch an den angrenzenden Segmenten angebracht.
> In der Ansicht Schneiden wird die Kontur mit den korrigierten (vergrößerten) Maßen angezeigt, die die Kontur nach dem Schneiden und vor der Kantenbearbeitung hat.

### Kante grob justieren

Mit diesem Werkzeug definieren Sie Segmente einer Kontur als Kante, die grob justiert werden muss. Grob justierte Kanten erhalten einen glasdickenabhängigen Bearbeitungszuschlag. Der Zuschlag ist in der sn.ini eingestellt.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die zu bearbeitende Kante (ein Segment).
3.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Der Bearbeitungszuschlag wird der Kontur zugewiesen und die Bearbeitungskennzeichnung wird an dem Segment angezeigt.

> **Bearbeitung auf angrenzender Segmente übernehmen**
> Bei glatten (tangentialen) Übergängen zwischen dem gewählten und angrenzenden Segmenten wird die jeweilige Kantenbearbeitung automatisch auch an den angrenzenden Segmenten angebracht.
> In der Ansicht Schneiden wird die Kontur mit den korrigierten (vergrößerten) Maßen angezeigt, die die Kontur nach dem Schneiden und vor der Kantenbearbeitung hat.

### Sonderkante festlegen

Mit diesem Werkzeug definieren Sie Segmente einer Kontur als Kante, die einer Sonderbearbeitung unterzogen werden muss. Bei Sonderkanten zeigt A+W CAD Designer (Shapes) einen Dialog an, in dem Sonderkanten ausgewählt werden können. Die Texte und Zuschläge von Sonderkanten können auf der Initialisierungsdatei (sn.ini) individuell eingestellt werden.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die zu bearbeitende Kante (ein Segment).
3.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) zeigt den Dialog Kante auswählen an.
4.  Wählen Sie eine Kantenbearbeitung aus und betätigen Sie <ENTER> oder [OK]. Der Bearbeitungszuschlag wird der Kontur zugewiesen und die Bearbeitungskennzeichnung wird an dem Segment angezeigt.

> **Bearbeitung auf angrenzender Segmente übernehmen**
> Bei glatten (tangentialen) Übergängen zwischen dem gewählten und angrenzenden Segmenten wird die jeweilige Kantenbearbeitung automatisch auch an den angrenzenden Segmenten angebracht.
> In der Ansicht Schneiden wird die Kontur mit den korrigierten (vergrößerten) Maßen angezeigt, die die Kontur nach dem Schneiden und vor der Kantenbearbeitung hat.

**Ergänzende Informationen**
*   Softwarereferenz, "Kante auswählen" auf Seite A-205

### Kante polieren

Mit diesem Werkzeug definieren Sie Segmente einer Kontur als Kante, die poliert werden muss. Zu polierende Kanten erhalten einen glasdickenabhängigen Bearbeitungszuschlag. Der Zuschlag ist in der sn.ini eingestellt.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die zu bearbeitende Kante (ein Segment).
3.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Der Bearbeitungszuschlag wird der Kontur zugewiesen und die Bearbeitungskennzeichnung wird an dem Segment angezeigt.

> **Bearbeitung auf angrenzender Segmente übernehmen**
> Bei glatten (tangentialen) Übergängen zwischen dem gewählten und angrenzenden Segmenten wird die jeweilige Kantenbearbeitung automatisch auch an den angrenzenden Segmenten angebracht.
> In der Ansicht Schneiden wird die Kontur mit den korrigierten (vergrößerten) Maßen angezeigt, die die Kontur nach dem Schneiden und vor der Kantenbearbeitung hat.

### Schnittkante festlegen

Mit diesem Werkzeug definieren Sie Segmente einer Kontur als Schnittkante. Schnittkanten erhalten keinen Bearbeitungszuschlag.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die zu bearbeitende Kante (ein Segment).
3.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Der Bearbeitungszuschlag wird der Kontur zugewiesen und die Bearbeitungskennzeichnung wird an dem Segment angezeigt.

> **Bearbeitung auf angrenzender Segmente übernehmen**
> Bei glatten (tangentialen) Übergängen zwischen dem gewählten und angrenzenden Segmenten wird die jeweilige Kantenbearbeitung automatisch auch an den angrenzenden Segmenten angebracht.

### Kante säumen

Mit diesem Werkzeug definieren Sie Segmente einer Kontur als Kante, die gesäumt werden muss.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die zu bearbeitende Kante (ein Segment).
3.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. Der Bearbeitungszuschlag wird der Kontur zugewiesen und die Bearbeitungskennzeichnung wird an dem Segment angezeigt.

> **Bearbeitung auf angrenzender Segmente übernehmen**
> Bei glatten (tangentialen) Übergängen zwischen dem gewählten und angrenzenden Segmenten wird die jeweilige Kantenbearbeitung automatisch auch an den angrenzenden Segmenten angebracht.

### Gehrungskante anbringen

Verwenden Sie dieses Werkzeug, wenn Sie an die Kante eines Floats oder ESGs eine Gehrungskante anbringen wollen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie auf das Segment, an das Sie eine Gehrung anbringen wollen. A+W CAD Designer (Shapes) färbt das Segment rot.
3.  Geben Sie im Wertefenster folgende Werte an:
    *   `< =`: Gehrungswinkel, Neigung des Winkels gegen die Oberseite oder Unterseite der Scheibe.
    *   `^ =`: Markieren Sie diese Checkbox, damit der Gehrungswinkel in Bezug zur Oberseite der Scheibe angebracht wird.
    *   `v =`: Markieren Sie diese Checkbox, damit der Gehrungswinkel in Bezug zur Unterseite der Scheibe angebracht wird.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) zeigt eine Kennung an den Segmenten an, die mit einer Gehrung versehen wurden.

> **Bearbeitung auf angrenzender Segmente übernehmen**
> Bei glatten (tangentialen) Übergängen zwischen dem gewählten und angrenzenden Segmenten wird die jeweilige Kantenbearbeitung automatisch auch an den angrenzenden Segmenten angebracht.

### Standardfacette anbringen

Mit diesem Werkzeug definieren Sie Segmente einer Scheibe, an denen eine Standard-Facette angebracht werden soll.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die Kante (ein Segment), an das eine Facette angebracht werden soll. A+W CAD Designer (Shapes) zeigt die Kante rot an.
3.  Geben Sie im Wertefenster folgende Einstellungen ein:
    *   `t=`: Breite der Facette mm.
    *   `^=`: Markieren Sie diese Checkbox, wenn die Oberseite des Glases facettiert werden soll.
    *   `v=`: Markieren Sie diese Checkbox, wenn die Unterseite des Glases facettiert werden soll.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) kennzeichnet die Kante mit dem entsprechenden Symbol.

> **Bearbeitung auf angrenzender Segmente übernehmen**
> Bei glatten (tangentialen) Übergängen zwischen dem gewählten und angrenzenden Segmenten wird die jeweilige Kantenbearbeitung automatisch auch an den angrenzenden Segmenten angebracht.

### Facette mit Neigungswinkel an der Kante anbringen

Verwenden Sie dieses Werkzeug, wenn Sie an die Kante eines Floats oder ESGs eine Facette mit einem betimmten Neigungswinkel anbringen wollen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Klicken Sie auf das Segment, an das Sie eine Facette anbringen wollen. A+W CAD Designer (Shapes) färbt das Segment rot.
3.  Geben Sie im Wertefenster folgende Werte an:
    *   `<`: Facettenwinkel, Neigung des Winkels gegen die Horizontale (Glasoberfläche).
    *   `t`: Breite der Facette
    *   `^`: Markieren Sie diese Checkbox, wenn die Oberseite des Glases facettiert werden soll.
    *   `v`: Markieren Sie diese Checkbox, wenn die Unterseite des Glases facettiert werden soll.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) zeigt eine Kennung an den Segmenten an, die mit einer Facette versehen wurden.

> **Bearbeitung auf angrenzender Segmente übernehmen**
> Bei glatten (tangentialen) Übergängen zwischen dem gewählten und angrenzenden Segmenten wird die jeweilige Kantenbearbeitung automatisch auch an den angrenzenden Segmenten angebracht.

### Sonderfacette anbringen

Mit diesem Werkzeug definieren Sie Segmente einer Scheibe, an denen eine Sonderfacette angebracht werden soll. Bei Sonderfacetten können Sie außer der Breite der Facette auch die Höhe des Restglases eingeben.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die Kante (ein Segment), an das eine Facette angebracht werden soll. A+W CAD Designer (Shapes) zeigt die Kante rot an.
3.  Geben Sie im Wertefenster folgende Einstellungen ein:
    *   r: Höhe des Restglases in mm.
    *   t: Breite der Facette mm.
    *   ^: Markieren Sie diese Checkbox, wenn die Oberseite des Glases facettiert werden soll.
    *   v: Markieren Sie diese Checkbox, wenn die Unterseite des Glases facettiert werden soll.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) kennzeichnet die Kante mit dem entsprechenden Symbol.

> **Bearbeitung auf angrenzender Segmente übernehmen**
> Bei glatten (tangentialen) Übergängen zwischen dem gewählten und angrenzenden Segmenten wird die jeweilige Kantenbearbeitung automatisch auch an den angrenzenden Segmenten angebracht.

## Kanten an VSG/ISO bearbeiten

Zur Bearbeitung von Kanten beim ISO/VSG stehen Ihnen folgende Werkzeuge zur Verfügung:

| Symbol | Kurzname | Beschreibung |
| --- | --- | --- |
| ESPELCAM | ESPELCAM | ⇨ "Sonderkante VSG festlegen" auf Seite A-419 |
| EDGELSTP | EDGELSTP | ⇨ "VSG-Stufe anbringen" auf Seite A-420 |
| EDGEISTP | EDGEISTP | ⇨ "ISO-Stufe anbringen" auf Seite A-421 |
| EDGERSTP | EDGERSTP | ⇨ "Bearbeite Kante mit VSG-Vorverbund oder ISO-Stufe" auf Seite A-422 |
| EDGEBLKG | EDGEBLKG | "VSG-Kante blockschleifen" auf Seite A-422 |
| EMITRLAM | EMITRLAM | ⇨ "Gehrung auf VSG anbringen" auf Seite A-423 |
| EDGESLAM | EDGESLAM | "VSG säumen" auf Seite A-424 |
| EDGEPLAM | EDGEPLAM | ⇨ "VSG polieren" auf Seite A-424 |

*Tab. A-40 Werkzeuge zum Bearbeiten von Kanten bei VSG/ISO*

### Sonderkante VSG festlegen

Mit diesem Werkzeug definieren Sie Segmente der Kontur einer VSG-Scheibe als Kante, die einer Sonderbearbeitung unterzogen werden muss. Bei Sonderkanten zeigt A+W CAD Designer (Shapes) einen Dialog an, in dem Sonderkanten ausgewählt werden können. Die Texte und Zuschläge von Sonderkanten können auf der Initialisierungsdatei (sn.ini) individuell eingestellt werden.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die zu bearbeitende Kante (ein Segment).
3.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) zeigt den Dialog Kante auswählen an.
4.  Wählen Sie eine Kantenbearbeitung aus und betätigen Sie <ENTER> oder [OK]. Der Bearbeitungszuschlag ist nun definiert und die Bearbeitungskennzeichnung wird an dem Segment angezeigt.

> **Bearbeitung auf angrenzende Segmente übernehmen**
> Bei glatten (tangentialen) Übergängen zwischen dem gewählten und angrenzenden Segmenten wird die jeweilige Kantenbearbeitung automatisch auch an den angrenzenden Segmenten angebracht.
> In der Ansicht Kantenbearbeitung der nächsttieferen Stufe werden die Teilscheiben mit dem Zuschlag angezeigt. Zusätzlich wird die Form in der Ansicht Schneiden auf der aktuellen Stufe (VSG-Zuschnitt) mit den korrigierten (vergrößerten) Maßen angezeigt.

**Ergänzende Informationen**
*   Softwarereferenz, "Kante auswählen" auf Seite A-205

### VSG-Stufe anbringen

Mit diesem Werkzeug definieren Sie Segmente einer VSG-Kontur als Kante, deren einzelne Scheiben abgestuft werden müssen. Dieses Werkzeug wird in der Ansicht Geometrie verwendet.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die abzustufende Kante (ein Segment). A+W CAD Designer (Shapes) zeigt die Kante rot an. Im Wertefenster erscheint für jede Scheibe der Einheit ein Feld für ein Abzugsmaß.
3.  Geben Sie im Wertefenster ein, um wie viele mm die Kante gekürzt werden soll. Die geforderten Maße beziehen sich für jede Scheibe auf das ursprüngliche Maß:
    *   d1: Wert in mm, um den die erste Scheibe der Einheit gekürzt werden soll.
    *   d2: Wert in mm, um den die zweite Scheibe der Einheit gekürzt werden soll.
    *   d3: Wert in mm, um den die dritte Scheibe der Einheit gekürzt werden soll.
    *   evtl. weitere Maße für weitere Einheiten.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) kennzeichnet die Kante mit dem entsprechenden Symbol.

> **Bearbeitung auf angrenzender Segmente übernehmen**
> Bei glatten (tangentialen) Übergängen zwischen dem gewählten und angrenzenden Segmenten wird die jeweilige Kantenbearbeitung automatisch auch an den angrenzenden Segmenten angebracht.

### ISO-Stufe anbringen

Mit diesem Werkzeug definieren Sie Segmente einer ISO-Kontur als Kante, deren einzelne Scheiben abgestuft werden müssen. Dieses Werkzeug wird in der Ansicht Geometrie verwendet.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die abzustufende Kante (ein Segment). A+W CAD Designer (Shapes) zeigt die Kante rot an. Im Wertefenster erscheint für jede Scheibe der Einheit ein Feld für ein Abzugsmaß.
3.  Geben Sie im Wertefenster ein, um wie viele mm die Kante gekürzt werden soll. Die geforderten Maße beziehen sich für jede Scheibe auf das ursprüngliche Maß:
    *   d1: Wert in mm, um den die erste Scheibe der Einheit gekürzt werden soll
    *   d2: Wert in mm, um den die zweite Scheibe der Einheit gekürzt werden soll
    *   d3: Wert in mm, um den die dritte Scheibe der Einheit gekürzt werden soll
    *   evtl. weitere Maße für weitere Einheiten
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) kennzeichnet die Kante mit dem entsprechenden Symbol.

> **Bearbeitung auf angrenzender Segmente übernehmen**
> Bei glatten (tangentialen) Übergängen zwischen dem gewählten und angrenzenden Segmenten wird die jeweilige Kantenbearbeitung automatisch auch an den angrenzenden Segmenten angebracht.

### Bearbeite Kante mit VSG-Vorverbund oder ISO-Stufe

In manchen Fällen kann es sinnvoll sein, neben dem senkrechten Wert die Einzugstiefe in einer anderen Richtung anzugeben. Dies ist z. B. relevant, wenn bei Modell 1 oder 2 die obere schräge Kante eingezogen werden soll. Hier kann es vorkommen, dass der Anwender bevorzugt den Einzug entlang der Nachbarkante übergibt, d. h. die senkrechte Verschiebung der Kante. Ausgewählt wird aktiv die zu verschiebende Kante und passiv eine zusätzliche Referenzkante. Die Auswahl der zweiten Kante ist optional. Dieses Werkzeug wird in der Ansicht Geometrie verwendet.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die zu verschiebende Kante. A+W CAD Designer (Shapes) zeigt die Kante rot an. Im Wertefenster erscheint für jede Scheibe der Einheit ein Feld für ein Einzug.
3.  Geben Sie im Wertefenster ein, um wie viele mm die Kante gekürzt werden soll. Die geforderten Maße beziehen sich für jede Scheibe auf das ursprüngliche Maß:
    *   d1: Wert in mm, um den die erste Scheibe der Einheit gekürzt werden soll
    *   d2: Wert in mm, um den die zweite Scheibe der Einheit gekürzt werden soll
    *   d3: Wert in mm, um den die dritte Scheibe der Einheit gekürzt werden soll
    *   evtl. weitere Maße für weitere Einheiten
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) kennzeichnet die Kante mit dem entsprechenden Symbol.
5.  Markieren Sie die zweite zu verschiebende Kante. A+W CAD Designer (Shapes) zeigt die Kante rot an. Im Wertefenster erscheint für jede Scheibe der Einheit ein Feld für ein Einzug.
6.  Die weitere Vorgehensweise ist identisch mit der oben aufgeführten.

### VSG-Kante blockschleifen

Mit diesem Werkzeug definieren Sie Segmente einer VSG-Kontur als Kante, die geschliffen werden muss.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die zu schleifende Kante (ein Segment). A+W CAD Designer (Shapes) zeigt die Kante rot an.
3.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) kennzeichnet die Kante mit dem entsprechenden Symbol.

> **Bearbeitung auf angrenzender Segmente übernehmen**
> Bei glatten (tangentialen) Übergängen zwischen dem gewählten und angrenzenden Segmenten wird die jeweilige Kantenbearbeitung automatisch auch an den angrenzenden Segmenten angebracht.
>
> In der Ansicht Kantenbearbeitung der nächsttieferen Stufe werden die Teilscheiben mit dem Zuschlag angezeigt. Zusätzlich wird die Form in der Ansicht Schneiden auf der aktuellen Stufe (VSG-Zuschnitt) mit den korrigierten (vergrößerten) Maßen angezeigt.

### Gehrung auf VSG anbringen

Mit diesem Werkzeug definieren Sie Segmente einer VSG-Kontur, die als Gehrung ausgeführt werden müssen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie die Kante (ein Segment), an das eine Gehrung angebracht werden soll. A+W CAD Designer (Shapes) zeigt die Kante rot an.
3.  Geben Sie im Wertefenster folgende Einstellungen ein:
    *   `<`: Neigungswinkel in Grad, den die Gehrung gegen die Vertikale hat.
    *   `^`: Markieren Sie diese Checkbox, wenn die Oberseite des Glases gekürzt werden soll.
    *   `v`: Markieren Sie diese Checkbox, wenn die Unterseite des Glases gekürzt werden soll.
4.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) kennzeichnet die Kante mit dem entsprechenden Symbol.

> **Bearbeitung auf angrenzender Segmente übernehmen**
> Bei glatten (tangentialen) Übergängen zwischen dem gewählten und angrenzenden Segmenten wird die jeweilige Kantenbearbeitung automatisch auch an den angrenzenden Segmenten angebracht.

### VSG säumen

Verwenden Sie dieses Werkzeug, um eine VSG-Kante zu säumen.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie ein oder nacheinander mehrere Segmente, die gesäumt werden sollen. A+W CAD Designer (Shapes) zeigt die markierten Segmente rot an.
3.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) kennzeichnet die Segmente mit dem entsprechenden Symbol.

> **Bearbeitung auf angrenzender Segmente übernehmen**
> Bei glatten (tangentialen) Übergängen zwischen dem gewählten und angrenzenden Segmenten wird die jeweilige Kantenbearbeitung automatisch auch an den angrenzenden Segmenten angebracht.

### VSG polieren

Verwenden Sie dieses Werkzeug, um eine VSG-Kante zu polieren.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie ein oder nacheinander mehrere Segmente, die poliert werden sollen. A+W CAD Designer (Shapes) zeigt die markierten Segmente rot an.
3.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) kennzeichnet die Segmente mit dem entsprechenden Symbol.

> **Bearbeitung auf angrenzender Segmente übernehmen**
> Bei glatten (tangentialen) Übergängen zwischen dem gewählten und angrenzenden Segmenten wird die jeweilige Kantenbearbeitung automatisch auch an den angrenzenden Segmenten angebracht.

## Kanten definieren

Diese Werkzeuge werden bei der Zusammenarbeit mit der A+W Enterprise TAB verwendet.

| Symbol | Kurzname | Beschreibung |
| --- | --- | --- |
| EDGCLSTD | EDGCLSTD | "Kante als Standardkante definieren" auf Seite A-425 |
| EDGCLSPE | EDGCLSPE | "Kante als Modell-Sonderkante definieren" auf Seite A-425 |
| EDGCLOUT | EDGCLOUT | "Kante als äußere Modellkante definieren" auf Seite A-426 |
| EDGCLINN | EDGCLINN | "Kante als innere Modellkante definieren" auf Seite A-426 |

*Tab. A-41 Werkzeuge zum Definieren von Kanten*

### Kante als Standardkante definieren

Um Kantenbearbeitungen für verschiedene Kantenarten zu unterscheiden, können Sie Kanten als Standardkante, Spezialkante, Modellkante außen oder Modellkante innen definieren.

Verwenden Sie dieses Werkzeug, um eine Kante als Standardkante zu definieren.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie ein oder mehrere Segmente, die als Standardkante definiert werden sollen. A+W CAD Designer (Shapes) zeigt die markierten Segmente rot an.
3.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) kennzeichnet die Segmente mit dem entsprechenden Symbol.

### Kante als Modell-Sonderkante definieren

Um Kantenbearbeitungen für verschiedene Kantenarten zu unterscheiden, können Sie Kanten als Standardkante, Spezialkante, Modellkante außen oder Modellkante innen definieren.
Verwenden Sie dieses Werkzeug, um eine Kante als Spezialkante zu definieren.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie ein oder mehrere Segmente, die als Spezialkante definiert werden sollen. A+W CAD Designer (Shapes) zeigt die markierten Segmente rot an.
3.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) kennzeichnet die Segmente mit dem entsprechenden Symbol.

### Kante als äußere Modellkante definieren

Um Kantenbearbeitungen für verschiedene Kantenarten zu unterscheiden, können Sie Kanten als Standardkante, Spezialkante, Modellkante außen oder Modellkante innen definieren.

Verwenden Sie dieses Werkzeug, um eine Kante als äußere Modellkante zu definieren.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie ein oder mehrere Segmente, die als äußere Modellkante definiert werden sollen. A+W CAD Designer (Shapes) zeigt die markierten Segmente rot an.
3.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) kennzeichnet die Segmente mit dem entsprechenden Symbol.

### Kante als innere Modellkante definieren

Um Kantenbearbeitungen für verschiedene Kantenarten zu unterscheiden, können Sie Kanten als Standardkante, Spezialkante, Modellkante außen oder Modellkante innen definieren.

Verwenden Sie dieses Werkzeug, um eine Kante als innere Modellkante zu definieren.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie ein oder mehrere Segmente, die als innere Modellkante definiert werden sollen. A+W CAD Designer (Shapes) zeigt die markierten Segmente rot an.
3.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK]. A+W CAD Designer (Shapes) kennzeichnet die Segmente mit dem entsprechenden Symbol.

## ISO- und VSG-Einheiten definieren

Zum Definieren von ISO- und VSG-Einheiten stehen Ihnen folgende Werkzeuge zur Verfügung:

| Symbol | Kurzname | Beschreibung |
| --- | --- | --- |
| 1+2 | PACLAYER | ⇨ "Scheibenfolgen für Einheiten definieren" auf Seite A-428 |

*Tab. A-42 Werkzeug zum Definieren von ISO- und VSG-Einheiten*

### Scheibenfolgen für Einheiten definieren

Mit diesem Werkzeug können Sie Scheibenreihenfolgen bei Einheiten festlegen. Dabei wird einer Außenkontur eine oder mehrere Scheibennummern zugeordnet.

⇨ Werkzeuge, "Einheiten mit Stückliste bearbeiten" auf Seite A-492

Am Bildschirm wird ein entsprechender Text in der Mitte der Kontur angezeigt.

1.  Wählen Sie das Werkzeug aus. Klicken Sie dazu auf das entsprechende Symbol.
2.  Markieren Sie ein Segment der zu bestimmenden Kontur. Dabei muss es sich um eine Außenkontur handeln und es dürfen noch keine Einheiten definiert worden sein. Das Segment färbt sich rot.
3.  Geben Sie im Wertefenster die Scheibenreihenfolge ein. Markieren Sie dazu die entsprechenden Checkboxen.
4.  Geben Sie im Wertefenster unter D die Versiegelungstiefe ein.
5.  Bestätigen Sie Ihre Eingabe mit <ENTER> oder [OK].

# Grundsätzliche Bedienung

Für jede Funktion aus einem Menü (z. B. Bearbeiten, Transformieren) müssen Sie die betreffende Kontur vorher auswählen. Für Funktionen im Menü Bearbeiten müssen Sie die zu bearbeitende Kontur (oder nur einzelne Segmente) vorher auswählen.

Wenn Sie ein Werkzeug aus der Werkzeugleiste verwenden wollen, verfahren Sie bei der Anwahl umgekehrt. Zuerst wählen Sie das gewünschte Werkzeug an und dann klicken Sie eine geeignete Stelle in der Zeichenfläche an, um das Werkzeug anzuwenden.

> **Funktionen ausführen und Werkzeuge anwenden**
> Beachten Sie bitte die unterschiedliche Vorgehensweise bei Werkzeugen und Funktionen aus den Menüs! Erst Werkzeug dann Objekt anwählen aber erst Objekt und dann Funktion auswählen.

Werkzeuge können ihre Bearbeitung direkt an der gewünschten Stelle ausführen. Bei Funktionen aus den Menüs wie Bearbeiten, Transformieren usw. muss sowohl der Gegenstand (Segment, Kontur) der Operation als auch die Aktion selber (wie weit verschoben oder gedreht wird usw.) bestimmt werden. Das erste Symbol auf jeder Werkzeugleiste ist immer der Mauszeiger. Seine Anwahl beendet die vorher gewählte Funktion bzw. bricht diese ab. Mit dem Mauszeiger ist die Auswahl von Konturelementen (etwa für Bearbeiten, Transformieren) möglich.

## Gummiband

Das Gummiband erscheint als blaue Linie am Bildschirm und kann zum Messen und zum Zeichnen eingesetzt werden.

### Messen mit dem Gummiband

1.  Positionieren Sie die Spitze de Zeigewerkzeugs an die Stelle, an der Sie die Messung starten wollen.
2.  Drücken Sie die linke Maustaste und ziehen Sie gleichzeitig mit der Maus entlang der Stecke, die Sie messen wollen.
3.  Lassen Sie die linke Maustaste am Endpunkt los. A+W CAD Designer (Shapes) erzeugt am Anfang und am Ende der Strecke ein blaues X und zeigt die Messergebnisse im Wertefenster an.

**Ergänzende Informationen**
*   "Neue Gerade durch Gummiband erfassen" auf Seite A-237
*   "Neuen Bogen durch Gummiband erfassen" auf Seite A-238

## Zoom (Lupe)

In der Werkzeugleiste befinden sich zwei Lupensymbole, eine mit einem Plus- und eine mit einem Minuszeichen. Durch Klick darauf wird der sichtbare Ausschnitt vergrößert (+) oder verkleinert (-).

Um die Zeichnung in unterschiedlicher Größe anzuzeigen haben Sie folgende Möglichkeiten:

*   Optimale Größe anzeigen
*   Schrittweise verkleinern
*   Schrittweise vergrößern
*   Bereich vergrößern

### Optimale Größe anzeigen

Optimale Größe anzeigen bedeutet, dass A+W CAD Designer (Shapes) alle Objekte einer Zeichnung anzeigt und dabei den ganzen Platz einer Seite ausnutzt.

1.  Bewegen Sie den Mauszeiger über die Lupe mit dem [+].
2.  Betätigen Sie gleichzeitig die linke und die rechte Maustaste. A+W CAD Designer (Shapes) zeigt alle Objekte in der optimalen Größe an.

### Segment in optimale Größe anzeigen

1.  Markieren Sie das Segment, das Sie in optimaler Größe anzeigen wollen. Klicken Sie dazu auf das Segment. A+W CAD Designer (Shapes) zeigt das markierte Segment rot an.
2.  Bewegen Sie den Mauszeiger über die Lupe mit dem (-).
3.  Betätigen Sie gleichzeitig die linke und die rechte Maustaste. A+W CAD Designer (Shapes) zeigt das markierte Segment auf den ganzen Bildschirmbereich vergrößert an.

> **Alle markierten Segmente werden vergrößert!**
> Sie können auch mehrere Segmente wählen, um diese optimal zu vergrößern.

### Ansicht schrittweise verkleinern

1.  Klicken Sie auf die Lupe mit dem [–]. A+W CAD Designer (Shapes) verkleinert die Darstellung der Objekte. Als Mittelpunkt verwendet A+W CAD Designer (Shapes) die Mitte der Zeichenfläche. Beachten Sie, dass A+W CAD Designer (Shapes) auch die Beschriftung der Lineale am Seitenrand anpasst.

Wenn Sie die Zeichnung an einer bestimmte Stelle schrittweise verkleinern wollen, dann gehen Sie wie folgt vor:

2.  Klicken Sie auf die Lupe mit dem [-] und halten Sie die Maustaste gedrückt.
3.  Ziehen Sie das Lupensymbol mit gedrückter Maustaste an die Stelle, die der Mittelpunkt der Verkleinerung sein soll.
4.  Lassen Sie die Maustaste los. A+W CAD Designer (Shapes) verkleinert die Ansicht um eine Stufe.
5.  Wiederholen Sie den beschriebenen Schritt, bis die Zeichnung die gewünschte Größe hat.

### Ansicht schrittweise vergrößern

1.  Klicken Sie auf die Lupe mit dem [+]. A+W CAD Designer (Shapes) vergrößert die Darstellung der Objekte. Als Mittelpunkt verwendet A+W CAD Designer (Shapes) die Mitte der Zeichenfläche. Beachten Sie, dass A+W CAD Designer (Shapes) auch die Beschriftung der Lineale am Seitenrand anpasst.

Wenn Sie eine bestimmte Stelle der Zeichnung schrittweise vergrößern wollen, dann gehen Sie wie folgt vor:

2.  Klicken Sie auf die Lupe mit dem [+] und halten Sie die Taste gedrückt.
3.  Ziehen Sie das Lupensymbol mit gedrückter Maustaste an die Stelle, die der Mittelpunkt der Vergrößerung sein soll.
4.  Lassen Sie die Maustaste los. A+W CAD Designer (Shapes) vergrößert die Ansicht um eine Stufe.
5.  Wiederholen Sie den beschriebenen Schritt, bis die Zeichnung die gewünschte Größe hat.

### Ausschnitt vergrößern

Ausschnitt vergrößern ist eine Funktion, die Sie permanent einschalten können.

1.  Klicken Sie mit dem Mauszeiger auf den kleinen Pfeil neben der [+]-Lupe. A+W CAD Designer (Shapes) zeigt einen Menüpunkt an.
    (Image shows a dropdown menu with the option "Ausschnitt vergrößern")
    *Abb. A-211 Ausschnitt vergrößern*
2.  Markieren Sie Ausschnitt vergrößern. Diese Funktion ist jetzt so lange aktiv, bis Sie die Markierung durch erneutes Anklicken wieder entfernen.
    Wenn Sie nicht permanent Ausschnitte vergrößern wollen, dann können Sie vorübergehend auch bei gedrückter <Strg> Ausschnitte vergrößern.
3.  Bewegen Sie den Mauszeiger an die linke obere Ecke des Ausschnitts, den Sie vergrößern wollen, und klicken Sie mit der linken Maustaste. Halten Sie die Maustaste gedrückt.
4.  Ziehen Sie den Mauszeiger an die rechte untere Ecke des Ausschnitts, den Sie vergrößern wollen, und lassen Sie die Maustaste los. A+W CAD Designer (Shapes) vergrößert den markierten Bereich. Beachten Sie, dass A+W CAD Designer (Shapes) auch die Beschriftung der Lineale am Seitenrand anpasst.

## Das Zeige-Werkzeug (Pfeil)

Der Zeiger dient im allgemeinen dazu, bestimmte Zeichnungselemente auszuwählen, um diese in irgendeiner Weise zu verändern, zu löschen oder um ihre genauen Daten zu erfahren. Sie können Zeichnungssegmente, Konturpunkte, Maßangaben und geometrische Beziehungen in der Zeichnung damit auswählen.

> **Auswahl aufheben**
> Ein zweites Anklicken des Zeigers hebt die Auswahl auf.

Mit dem Pfeil können Sie folgende Funktionen ausführen:

*   "Ein Segment oder mehrere Segment auswählen" auf Seite A-432
*   "Geometrische Beziehungen anzeigen" auf Seite A-433
*   "Maßangaben anzeigen und ändern" auf Seite A-433
*   "Dekorationen anzeigen und ändern" auf Seite A-433

### Ein Segment oder mehrere Segment auswählen

1.  Klicken Sie mit dem Zeige-Werkzeug auf ein Segment. Das gewählte Segment wird fett dargestellt und sein Anfangs- und Endpunkt mit der Ziffer 1 und 2 versehen. Im Wertefenster zeigt A+W CAD Designer (Shapes) alle aktuellen Daten des Segmentes an. Zum Anfangspunkt (1) gehören die Koordinaten x1 und y1, zum Endpunkt (2) die Koordinaten x2 und y2. Die Überganswinkel zu den angrenzenden Segmenten werden mit den Symbolen <1 und <2 (für 1. und 2. Punkt) angezeigt.
2.  Lassen Sie die Maus auf dem zuerst markierten Segment stehen und klicken Sie mit der linken Maustaste erneut oder betätigen Sie < + >. Mit jedem weiteren linken Mausklick (oder < + >) markiert A+W CAD Designer (Shapes) das nächste Segment im Uhrzeigersinn. Mit jedem rechten Mausklick (oder < - >) wählen Sie in entgegengesetzter Richtung das nächste Segment an. Sie müssen hierbei lediglich darauf achten, die Maus nicht zu verschieben.

Wenn das angewählte Segment durch eine Werkzeugbedienung wie Abrunden, Punktverschieben, Hilfsschnitt usw. entstanden ist, dann werden im Wertefenster die Parameter zur Änderung oder Bestätigung angezeigt.

### Geometrische Beziehungen anzeigen

Da geometrische Beziehungen wie z. B. Parallelität oder Rechtwinkligkeit immer zwischen zwei Segmenten bestehen, diese Beziehungen aber an nur einem Segment gekennzeichnet werden können, kann man das dazugehörige zweite Segment auf den ersten Blick nicht erkennen.

1.  Klicken Sie mit der linken Maustaste auf eine Kennzeichnung (z. B. Sympol für Parallelität). A+W CAD Designer (Shapes) zeigt die beiden (zu dieser Beziehung) gehörenden Segmente und die dazugehörige Kennzeichnung fett an.

### Maßangaben anzeigen und ändern

1.  Klicken Sie eine beliebige Vermaßung an. A+W CAD Designer (Shapes) markiert die angeklickte Vermaßung und das zugehörige Segment. Das Maß erscheint im Wertefenster und kann dort geändert werden.
2.  Ändern Sie, je nach Erfordernis, die jeweiligen Maßangaben.

### Dekorationen anzeigen und ändern

Dekorationen (Beschriftungen (Texte) und Maße, die angezeigt werden und keine aktive Vermaßung sind), die auf einzelnen Segmenten angebracht sind, können Sie inspizieren und ändern.

1.  Klicken Sie mit dem Zeige-Werkzeug auf die jeweilige Dekoration (z. B. Parallelverschiebung (P) oder Skalierung (S)).
2.  Ändern Sie die Angaben der Kontur, wie z. B. Glaszuschläge bei Kantenbearbeitungen (X, XX, etc.).

## Mit Dateien arbeiten

Zum Arbeiten mit Dateien stehen Ihnen folgende Funktionen zur Verfügung:

*   "Datei öffnen" auf Seite A-434
*   "Datei speichern" auf Seite A-434
*   "Dateien importieren" auf Seite A-435
*   "Konturen aus BLOCK.IND importieren" auf Seite A-436
*   "CAD Designer-Zeichnung exportieren" auf Seite A-436
*   "Zeichnung drucken" auf Seite A-437

### Datei öffnen

Mit dieser Funktion laden Sie eine bereits bestehende Kontur, die in einer *.sn Datei auf dem Datenträger abgelegt ist, in den Arbeitsspeicher.

1.  Wählen Sie `Datei > Öffnen`.
2.  Geben Sie einen Dateinamen ein:
    *   Geben Sie den Dateinamen im Feld `Dateiname` ein (mit oder ohne Dateierweiterung) oder
    *   wählen Sie mit der Maus eine Datei aus.
    *   Im Eingabefeld `Dateityp` können Sie den Dateityp einstellen. A+W CAD Designer (Shapes) lässt als Dateierweiterung verschiedene Grafikformate zu.
    *   Mit der Kombobox `Suchen in` können Sie das gewünschte Verzeichnis wechseln.
3.  Bestätigen Sie ihre Auswahl mit <ENTER> oder [OK]. Die ausgewählte Kontur wird geladen und auf dem Bildschirm dargestellt. Der entsprechende Dateiname wird in der Titelzeile des Programms angezeigt.

Wenn Sie den Dialog ohne eine Aktion verlassen möchten, betätigen Sie [ABBRECHEN]. Sie gelangen nun zu A+W CAD Designer (Shapes) zurück und können Ihre zuvor begonnen Arbeit fortsetzen.

> **Verfügbare Sprachen**
> Die Sprache der Dialogbox ist abhängig von der auf Ihrem Computer installierten Windows Version.
> Es können mehrere Zeichnungen gleichzeitig geöffnet sein.

### Datei speichern

Mit dieser Dialogbox geben Sie einen Dateinamen ein, unter dem Sie die Datei abspeichern möchten. Es ist nicht nötig eine Dateierweiterung anzugeben, da sie vom Programm selbst vergeben wird. Wenn Sie einen bereits bestehenden Dateinamen ausgewählt haben, werden Sie anschließend gefragt, ob Sie diese Datei überschreiben wollen.

> **Datei unter neuem Namen speichern!**
> Häufig wird eine Zeichnung geladen, um darauf aufbauend eine neue, andere Kontur zu entwerfen. Um die Gefahr des Datenverlustes der ursprünglichen Datei durch Überschreiben mit der geänderten Datei zu vermeiden, ist es ratsam, noch vor dem Bearbeiten der geladenen Datei diese unter dem neuen Namen zu speichern. A+W CAD Designer (Shapes) merkt sich das Verzeichnis, unter dem zuletzt abgespeichert wurde. Dieses kann vom Verzeichnis, das zum Öffnen von Dateien benutzt wird, verschieden sein. Dadurch wird die Gefahr eines unabsichtlichen Überschreibens einer (z. B. als Vorlage gedachten) Kontur beim Speichern (der produktionsfertig vermaßten Kontur) verringert.

1.  Wählen Sie `Datei > Speichern unter`. A+W CAD Designer (Shapes) zeigt den Dialog `Globale Formdaten` an.
2.  Füllen Sie die für Sie relevanten Felder aus.
3.  Betätigen Sie [OK]. A+W CAD Designer (Shapes) zeigt den Dialog `Speichern unter` an.
4.  Geben Sie einen Dateinamen an:
    *   Geben Sie den Dateinamen im Feld `Dateiname` ein (mit oder ohne Dateierweiterung) oder
    *   wählen Sie mit der Maus einen Dateinamen aus.
    *   Mit der Kombobox `Speichern` können Sie das gewünschte Verzeichnis wechseln.
5.  Bestätigen Sie Ihre Auswahl mit <ENTER> oder [OK]. Die Datei wird gespeichert.

Wenn Sie den Dialog ohne eine Aktion verlassen möchten, betätigen Sie [ABBRECHEN]. Sie gelangen nun zu A+W CAD Designer (Shapes) zurück und können Ihre zuvor begonnen Arbeit fortsetzen.

### Dateien importieren

Nachfolgend wird beispielhaft das Importieren einer ESG-Datei beschrieben. Diese Beschreibung gilt auch für andere Importformate.

1.  Öffnen Sie das Menü `Daten > Importieren > ESG...`
    Es erscheint ein Eingabedialog.
2.  Geben Sie das Verzeichnis an, in dem nach Dateien mit der Endung .ESG gesucht werden soll.
    Nach der Pfadangabe werden alle ESG-Dateien (wenn vorhanden) aufgelistet.
3.  Wählen Sie die gewünschte Datei oder geben Sie den Dateinamen ein.
4.  Bestätigen Sie die Eingabe oder Auswahl. Betätigen Sie dazu [OK] oder <Enter>.

Die gewählte ESG-Kontur wird nun in Ihr aktuelles Objekt eingefügt. Dabei schaltet A+W CAD Designer (Shapes) ggf. auf die Ansicht Skizze um.

### Konturen aus BLOCK.IND importieren

1.  Öffnen Sie das Menü `Datei > Importieren > BLOCK.IND`.
    Es erscheint ein Dialog, in dem A+W CAD Designer (Shapes) den Inhalt der Datenbank BLOCK.IND anzeigt. Konturen, die mit A+W CAD Designer (Shapes) exportiert wurden, besitzen die Endung .sn und tragen dahinter die Bezeichnung der Ansicht, aus der sie exportiert wurden. Andere Konturen (aus S/N 2.XX) können beliebige 30 Zeichen lange Namen haben.
2.  Wählen Sie die gewünschte Kontur aus.
    Einmaliges Anklicken eines Namens zeigt den Zusatztext im unteren Teil der Auswahlbox an. Durch Eingabe der ersten Zeichen eines Namens im Eingabefeld am oberen Rand der Box rollt die Anzeige auf diejenigen Konturen, deren Namen mit den eingegebenen Zeichen beginnen.
3.  Wählen Sie, ob Sie Außenkonturen (shaping) oder Innenkonturen (nesting) importieren wollen. Markieren Sie dazu die entsprechende Checkbox im Dialog.
4.  Importieren Sie die ausgewählte Kontur mit Doppelklick oder mit <Enter>.

### CAD Designer-Zeichnung exportieren

1.  Öffnen Sie das Menü `Datei > Exportieren`.
    Die verfügbaren Exportformate werden angezeigt.
2.  Wählen Sie eines der angegebenen Formate.
    Die A+W CAD Designer (Shapes)-Zeichnung wird in das ausgewählten Format umgewandelt und unter mit dem Namen der Zeichnung und der formatspezifischen Dateiendung im aktuellen Arbeitsverzeichnis (Festplatte, Diskette oder Server) gespeichert. Das Original A+W CAD Designer (Shapes)-Objekt bleibt erhalten.

> **Erst speichern, dann exportieren!**
> Sollten Sie eine zu exportierende Zeichnung noch nicht als Datei gesichert oder zwischenzeitlich verändert haben, so öffnet sich zuerst der Dialog zum Speichern. Wenn Ihre aktuelle Datei als A+W CAD Designer (Shapes)-Objekt gesichert ist, wird sie automatisch exportiert.

### Zeichnung drucken

1.  Rufen Sie zunächst `Datei > Vorschau` auf, wenn Sie vor dem Druck prüfen wollen, was gedruckt wird.
2.  Stellen Sie im Dialog `Seitenansicht` oder `Drucken` die Anzahl Kopien und das gewünschte Formular ein.
3.  Wählen Sie aus, ob Sie die Zeichnung vollständig, in einem bestimmten Maßstab oder einen Ausschnitt in einem Rahmen drucken wollen.
4.  Wenn Sie einen bestimmten Drucker auswählen wollen, dann betätigen Sie [Drucker]. A+W CAD Designer (Shapes) zeigt den Dialog zur Auswahl des Druckers an.
    *   Wählen Sie den gewünschten Drucker aus. und bestätigen Sie die Auswahl mit [OK].
    *   Betätigen Sie [OK]. A+W CAD Designer (Shapes) kehrt zum vorherigen Dialog zurück.
5.  Betätigen Sie [OK] um den Ausdruck zu starten.

**Ergänzende Informationen**
*   "Datei speichern" auf Seite A-434
*   Softwarereferenz, "Öffnen" auf Seite A-163
*   Softwarereferenz, "Globale Formdaten" auf Seite A-167
*   Softwarereferenz, "Datei auswählen..." auf Seite A-172
*   Softwarereferenz, "Seitenansicht Dialog..." auf Seite A-178
*   Softwarereferenz, "Speichern unter" auf Seite A-170
*   Softwarereferenz, “Datei speichern unter (exportieren)" auf Seite A-175

## Allgemeine Funktionen

In diesem Abschnitt sind folgende Funktionen zusammengefasst:

*   Werkzeuge, “Rückgängig machen oder wieder herstellen" auf Seite A-438
*   Werkzeuge, "Auswählen, Kopieren und Löschen" auf Seite A-438
*   Werkzeuge, "Segmente und Konturen transformieren" auf Seite A-439
*   Werkzeuge, "Mit Gruppen arbeiten" auf Seite A-442

### Rückgängig machen oder wieder herstellen

#### Bearbeitung Rückgängig machen

1.  Öffnen Sie das Menü `Bearbeiten`.
2.  Wählen Sie die Option `Rückgängig`.

Oder

1.  Drücken Sie `<Strg>` oder `<Ctrl>` (Steuerungs- oder Control-Taste) und halten Sie diese Taste gedrückt.
2.  Betätigen Sie `<Z>`. Mit jedem Betätigen dieser Taste wird die bisher letzte Aktion widerrufen.

Oder

1.  Drücken Sie `<Alt>` und halten Sie diese gedrückt.
2.  Betätigen Sie `<->` (die Rückschritt-Taste). Mit jedem Betätigen dieser Taste wird die bisher letzte Aktion widerrufen.

#### Letzte Bearbeitungsstände wieder herstellen

1.  Öffnen Sie das Menü `Bearbeiten`.
2.  Wählen Sie die Option `Wiederherstellen` an.

Oder

1.  Drücken Sie `<Strg>` oder `<Ctrl>` oder `<Alt>` (Steuerungs-, Control- oder Alternativ-Taste) und halten Sie diese gedrückt.
2.  Betätigen Sie `<R>`. Mit jedem Betätigen der Taste R wird die bisher zuletzt widerrufene Aktion wieder hergestellt.

### Auswählen, Kopieren und Löschen

#### Ganze Kontur auswählen

1.  Markieren Sie ein Segment oder eine Gruppe von Segmenten einer Kontur.
2.  Öffnen Sie das Menü `Bearbeiten`.
3.  Wählen Sie die Option `Kontur auswählen`.
    Die ganze Kontur färbt sich und ist ausgewählt.

Oder

1.  Markieren Sie ein Segment oder eine Gruppe von Segmenten, der Kontur, die Sie auswählen wollen.
2.  Betätigen Sie `<CTRL>` + `<A>`.
    Die ganze Kontur färbt sich und ist ausgewählt.

#### Auswahl kopieren, ausschneiden, einfügen oder löschen

1.  Markieren Sie ein Segment oder eine Gruppe von Segmenten.
2.  Öffnen Sie das Menü `Bearbeiten`.
3.  Wählen Sie die Option `Kopieren` oder `Ausschneiden` oder `Einfügen` oder `Löschen`. Die gewählte Option wird an den markierten Segmenten durchgeführt.

## Segmente und Konturen transformieren

Mit `transformieren` sind bei A+W CAD Designer (Shapes) folgende Funktionen gemeint:

*   "Kontur verschieben" auf Seite A-439
*   "Kontur frei drehen" auf Seite A-440
*   "Objekt um 90° im Uhrzeigersinn drehen" auf Seite A-440
*   "Kontur wie in einer anderen Ansicht positionieren" auf Seite A-440
*   "Objekt horizontal spiegeln" auf Seite A-440
*   "Objekt vertikal spiegeln" auf Seite A-441
*   "Objekt skalieren" auf Seite A-441
*   "Objekt strecken" auf Seite A-441

### Kontur verschieben

1.  Aktivieren Sie den Pfeil (Zeigewerkzeug). Klicken Sie dazu auf das entsprechende Symbol.
2.  Wählen Sie mit der Maus ein Segment des zu verschiebenden Objektes aus.
3.  Öffnen Sie das Menü `Transformieren` und wählen Sie die Option `Verschieben`. Es wird nun automatisch um das zu verschiebende Objekt ein rechteckiger Rahmen gelegt und das komplette Objekt wird markiert.
4.  Klicken Sie mit der linken Maustaste an beliebiger Stelle auf der Zeichenfläche und halten Sie die Maustaste gedrückt.
5.  Ziehen Sie die Maus bei gedrückter Maustaste um die gewünschte Verschiebungslänge in die gewünschte Richtung (hierbei wird ein Gummiband angezeigt).
6.  Lassen Sie die Maustaste an der gewünschten Stelle los. Das Objekt wird um die Länge des Gummibandes in die entsprechende Richtung verschoben und neu gezeichnet. Die Länge der Verschiebung kann auch während der Mausbetätigung im Wertefenster abgelesen werden.

### Kontur frei drehen

1.  Aktivieren Sie den Pfeil (Zeigewerkzeug). Klicken Sie dazu auf das entsprechende Symbol.
2.  Wählen Sie mit der Maus ein Segment des zu drehenden Objektes aus.
3.  Öffnen Sie das Menü `Transformieren` und wählen Sie die Option `Drehen`. Es wird nun automatisch um das zu drehende Objekt ein rechteckiger Rahmen gelegt und das komplette Objekt wird markiert.
4.  Klicken Sie mit der linken Maustaste an beliebiger Stelle auf dem Zeichenbrett und lassen Sie diese gedrückt.
5.  Ziehen Sie die Maus bei gedrückter Maustaste um den gewünschten Drehwinkel (Winkel wird im Wertefenster angezeigt) um das Objekt herum. Hierbei wird in Form eines Gummibandes ein Hebel vom Zentrum des gerahmten Objektes zum Mauszeiger angedeutet.
6.  Wenn Sie den gewünschten Drehwinkel erreicht haben, dann lassen Sie die Maustaste los. Das Objekt wird in gedrehter Lage neu dargestellt.

### Objekt um 90° im Uhrzeigersinn drehen

1.  Aktivieren Sie den Pfeil (Zeigewerkzeug). Klicken Sie dazu auf das entsprechende Symbol.
2.  Wählen Sie mit der Maus ein Segment des zu drehenden Objektes aus.
3.  Öffnen Sie das Menü `Transformieren` und wählen Sie die Option `Drehen um 90°`. Das gesamte Objekt wird um 90° im Uhrzeigersinn gedreht.

### Kontur wie in einer anderen Ansicht positionieren

1.  Aktivieren Sie den Pfeil (Zeigewerkzeug). Klicken Sie dazu auf das entsprechende Symbol.
2.  Wählen Sie mit der Maus ein Segment des zu verschiebenden Objektes aus.
3.  Öffnen Sie das Menü `Transformieren` und wählen Sie die Option `positionieren wie in ...`. Die selektierte Kontur erfährt die gleichen Transformationen (verschieben, drehen usw.) wie sie in der ausgewählten Ansicht (wie in ...) für diese Kontur bereits vorgenommen wurde.

### Objekt horizontal spiegeln

1.  Aktivieren Sie den Pfeil (Zeigewerkzeug). Klicken Sie dazu auf das entsprechende Symbol.
2.  Wählen Sie mit der Maus ein Segment des zu spiegelnden Objektes aus.
3.  Öffnen Sie das Menü `Transformieren` und wählen Sie die Option `horizontal spiegeln`. Das gesamte Objekt wird an der horizontalen Achse gespiegelt.

### Objekt vertikal spiegeln

1.  Aktivieren Sie den Pfeil (Zeigewerkzeug). Klicken Sie dazu auf das entsprechende Symbol.
2.  Wählen Sie mit der Maus ein Segment des zu spiegelnden Objektes aus.
3.  Öffnen Sie das Menü `Transformieren` und wählen Sie die Option `vertikal spiegeln`. Das gesamte Objekt wird an der vertikalen Achse gespiegelt.

### Objekt skalieren

1.  Aktivieren Sie den Pfeil (Zeigewerkzeug). Klicken Sie dazu auf das entsprechende Symbol.
2.  Wählen Sie mit der Maus ein Segment des zu skalierenden Objektes aus.
3.  Öffnen Sie das Menü `Transformieren` und wählen Sie die Option `skalieren`. Das gesamte Objekt wird markiert dargestellt.
4.  Geben Sie im Wertefenster die Faktoren ein, um die das Objekt in X- und in Y-Richtung skaliert werden soll.
5.  Klicken Sie [OK] oder betätigen Sie <ENTER>. Die von Ihnen eingegebenen Skalierung wird in die Zeichnung übernommen und die Kontur wird neu dargestellt.

### Objekt strecken

1.  Aktivieren Sie den Pfeil (Zeigewerkzeug). Klicken Sie dazu auf das entsprechende Symbol.
2.  Wählen Sie mit der Maus ein Segment des zu streckenden Objektes aus.
3.  Öffnen Sie das Menü `Transformieren` und wählen Sie die Option `strecken`. Das gesamte Objekt wird markiert dargestellt.
4.  Geben Sie nun im Wertefenster die Längen an, um die das Objekt an jeder Seite in X- und Y-Richtung gestreckt werden soll.
5.  Klicken Sie [OK] oder betätigen Sie <ENTER>. Die von Ihnen eingegebene Streckung wird in die Zeichnung übernommen und die Figur wird neu dargestellt.

## Mit Gruppen arbeiten

Neben der Wahl eines Einzelelementes sind in A+W CAD Designer (Shapes) auch Gruppierungen möglich. Eine Gruppe ist eine Menge von Elementen, die gemeinsam bearbeitet (kopiert, verschoben, gelöscht, ausgerichtet oder ersetzt) werden. Nachfolgend finden Sie folgende Arbeiten beschrieben:

*   "Elemente gruppieren" auf Seite A-442
*   "Elemente einer Gruppe hinzufügen" auf Seite A-443
*   "Gruppierung aufheben" auf Seite A-444
*   "Gruppe ersetzen" auf Seite A-444

### Elemente gruppieren

1.  Markieren Sie mehrere Elemente. Halten Sie dazu die Taste `<Ctrl>` oder `<Strg>` gedrückt und klicken Sie bei gedrückter Taste nacheinander auf die Elemente (Segmente, Bohrungen), die Sie gruppieren wollen. Neu angeklickten Elemente fügt A+W CAD Designer (Shapes) der Gruppe der bereits markierten Objekte hinzu und färbt sie rot. Wenn Sie die Maus nicht bewegen und die linke oder rechte Maustaste betätigen, werden die nächsten oder die vorhergehenden Segmente in der Kette den markierten Segmenten hinzugefügt.
    Bei manchen Werkzeugen ist von vornherein die Auswahl mehrerer Elemente notwendig, dort entfällt das Drücken der Taste. Wenn mehrere Elemente ausgewählt sind, bleibt das Zufügen weiterer Elemente eingeschaltet, auch wenn Sie die Taste loslassen.
    Die Erweiterung der Auswahl bleibt solange erhalten, bis ein anderes Werkzeug angeklickt wird. Ein Klick auf den Pfeil (Zeigewerkzeug) löst eine bestehende Markierung auf.
2.  Wählen Sie im Menü `Transformieren` die Option `Gruppieren`. A+W CAD Designer (Shapes) zeigt im Wertefenster folgende Einstellmöglichkeiten an:

| Option | Bedeutung |
| :--- | :--- |
| `ப` | Mit dieser Einstellung erstellt A+W CAD Designer (Shapes) ein senkrecht stehendes Gruppierungsrechteck. |
| `|_/` | Mit dieser Einstellung erzeugt A+W CAD Designer (Shapes) eine Gruppe, deren Gruppierungsrechteck parallel zu einem der Segmente der gruppierten Konturen ist. Wenn die Konturen gegen die x-Achse gedreht sind, entsteht ein gedrehtes Gruppierungsrechteck. |
| `min` | Mit dieser Einstellung erstellt A+W CAD Designer (Shapes) ein minimales Gruppierungsrechteck |
| `fix` | Wenn Sie eine Gruppe fixieren, dann können Sie dieser Gruppe keine weiteren Elemente (Konturen) zufügen. |
| `RefP` | Hier geben Sie an, welche Seite des Gruppierungsrechtecks die Bezugskante sein soll. Wenn Sie die Gruppe an einem anderen Element ausrichten wollen, dann bezieht sich die Ausrichtung auf die hier angegebene Seite. Folgende Eingaben sind möglich:<br>- 1: untere Kante<br>- 2: rechte Kante<br>- 3: obere Kante<br>- 4: linke Kante<br>⇨ "Komplexe Ausschnitte positionieren" auf Seite A-335 |
| `[>]` | Mit dieser Einstellung erhält die Bezugskante eine Ausrichtung im Uhrzeigersinn. Dies ist von Bedeutung, wenn Sie die Gruppe an einem Segment einer anderen Kontur ausrichten wollen.<br>⇨ "Komplexe Ausschnitte positionieren" auf Seite A-335 |
| `[<]` | Mit dieser Einstellung erhält die Bezugskante eine Ausrichtung gegen den Uhrzeigersinn. Dies ist von Bedeutung, wenn Sie die Gruppe an einem Segment einer anderen Kontur ausrichten wollen.<br>⇨ "Komplexe Ausschnitte positionieren" auf Seite A-335 |
| `<>=` | Hier zeigt A+W CAD Designer (Shapes) die Breite des Gruppierungsrechtecks an. |
| `^v=` | Hier zeigt A+W CAD Designer (Shapes) die Höhe des Gruppierungsrechtecks an. |
| `< =` | Hier können Sie den Abstand der linken Seite des Gruppierungsrechtecks zum ersten Element eingeben. |
| `> =` | Hier können Sie den Abstand der rechten Seite des Gruppierungsrechtecks zum ersten Element eingeben. |
| `^ =` | Hier können Sie den Abstand der oberen Seite des Gruppierungsrechtecks zum ersten Element eingeben. |
| `v =` | Hier können Sie den Abstand der unteren Seite des Gruppierungsrechtecks zum ersten Element eingeben. |

*Tab. A-43 Optionen beim Gruppieren*

3.  Wählen Sie die gewünschten Einstellungen und betätigen Sie [OK]. A+W CAD Designer (Shapes) stellt die Gruppe mit einem umschreibenden Rechteck dar.

### Elemente einer Gruppe hinzufügen

A+W CAD Designer (Shapes) bietet folgende Möglichkeiten, um ein Element einer Gruppe hinzuzufügen:

*   Element in das Gruppierungsrechteck schieben
*   Gruppierung erweitern

> **Gruppe darf nicht fixiert sein!**
> Sie können nur dann Elemente einer Gruppe zufügen, wenn die entsprechende Gruppe nicht fixiert ist.

#### Element in das Gruppierungsrechteck verschieben:

1.  Markieren Sie das Element, das Sie einer Gruppe zufügen wollen.
2.  Verschieben Sie das Element in das Gruppierungsrechteck. A+W CAD Designer (Shapes) fügt neue Elemente im Gruppierungsrechteck automatisch der Gruppe zu.

#### Gruppierung erweitern

1.  Markieren Sie das Gruppierungsrechteck. Klicken Sie dazu auf eine Seite des Gruppierungsrechtecks.
2.  Halten Sie `<Ctrl>` oder `<Strg>` gedrückt und klicken Sie bei gedrückter Taste die Elemente an, die der Gruppe zugefügt werden sollen. Neu angeklickten Segmente (oder Ausschnitte oder Bohrungen) färbt A+W CAD Designer (Shapes) rot.
3.  Wählen Sie im Menü `Transformieren` die Option `Gruppieren`. A+W CAD Designer (Shapes) zeigt im Wertefenster Einstellmöglichkeiten an.
4.  Wählen Sie die gewünschten Einstellungen und betätigen Sie [OK]. A+W CAD Designer (Shapes) stellt die Gruppe mit einem umschreibenden Rechteck dar.

### Gruppierung aufheben

1.  Markieren Sie das Gruppierungsrechteck. Klicken Sie dazu auf eine Seite des Gruppierungsrechtecks.
2.  Betätigen Sie `<Entf>`. A+W CAD Designer (Shapes) entfernt das Gruppierungsrechteck. Alle Elemente, die im Gruppierungsrechteck waren, liegen jetzt wieder ungruppiert vor.

### Gruppe ersetzen

Grundsätzlich sollten Sie, wenn Sie mit Ausschnitten arbeiten, diese Ausschnitte gruppieren und als eigene Datei abspeichern. Wenn Sie dann z. B. an einer Tür einen anderen Ausschnitt benötigen, dann können Sie diesen Ausschnitt samt aller Ausrichtungen und Vermaßungen mit A+W CAD Designer (Shapes) einfach austauschen.

1.  Markieren Sie die Gruppe, die Sie gegen eine andere Gruppe austauschen wollen. Klicken Sie dazu auf eine Seite des Gruppierungsrechtecks. A+W CAD Designer (Shapes) markiert das angeklickte Segment rot.
2.  Wählen Sie im Menü `Transformieren` die Funktion `Gruppe ersetzen`. A+W CAD Designer (Shapes) öffnet den Dialog `Datei zum Einfügen wählen`.
3.  Wählen Sie die Datei aus, mit der Sie die Gruppe ersetzen wollen und betätigen Sie [Öffnen]. A+W CAD Designer (Shapes) öffnet die gewählte Datei und ersetzt damit die markierte Gruppe. Wenn die gewählte Datei eine Gruppe enthält und die ursprüngliche Gruppe gegen ein Segment ausgerichtet war, dann richtet A+W CAD Designer (Shapes) die Gruppe wieder genau so aus, wie die ursprüngliche Gruppe ausgerichtet war.

**Ergänzende Informationen**
*   Softwarereferenz, "Datei zum Einfügen wählen" auf Seite A-166
*   "Ganze Kontur auswählen" auf Seite A-438
*   "Kontur verschieben" auf Seite A-439
*   "Komplexe Ausschnitte positionieren" auf Seite A-335

# Konkrete Fragestellungen

Dieser Bereich befasst sich mit gezielten Fragestellungen unserer Kunden. Die Fragen sind in folgende Blöcke zusammengefasst:

*   Wie werden Konturen erfasst
*   Wie werden Scheiben bearbeitet
*   Wie wird mit Bauglas gearbeitet
*   Wie werden Zeichnungen gedruckt
*   Wie ist die Zusammenarbeit mit anderen Programmen

## Wie werden Konturen erfasst

Scheiben oder Einheiten (ISO, VSG) werden im A+W CAD Designer (Shapes) als Kontur (Reihe von Segmenten) angezeigt. A+W CAD Designer (Shapes) bietet mehrere Möglichkeiten, eine Kontur zu erfassen:

*   Kontur-Daten importieren und ergänzen
*   Scheibe als Kontur digitalisieren
*   Scheibe als Skizze erfassen
*   Mit Modellen arbeiten
*   Tür mit Ausschnitten und Bohrungen versehen
*   Komplexe Kontur erstellen

Nach der Erfassung einer Kontur können Sie Informationen zu Glasart, Kunde, Glasdicke, Auftragsnummer, etc. erfassen. Den Dialog dazu zeigt Ihnen A+W CAD Designer (Shapes) spätestens beim Speichern automatisch an. Sie können diesen aber auch bei Bedarf aufrufen:
⇨ Softwarereferenz, "Globale Formdaten" auf Seite A-167

### Kontur-Daten importieren und ergänzen

Wenn Sie Scheibengeometrieen in unterschiedlichen Dateiformaten erhalten, dann bietet A+W CAD Designer (Shapes) verschiedene Importfilter an:

| Format | Beschreibung |
| --- | --- |
| **DXF** | Datenaustauschformat aus CAD-Anwendungen. In den Dateien können mehrere Ebenen (Layer) enthalten sein, die Sie beim Import einzeln auswählen können. |
| **ESG** | Austauschformat mit dem A+W-Programm ESG-Kontur. |
| **IGES (2D und 3D)** | Standard-Datenaustauschformat nach IEEE für CAD-Daten. |
| **VDA (2D und 3D)** | Standard-Datenaustauschformat in der deutschen Automobilindustrie für CAD-Daten. |
| **CAM/XML** | Datenaustauschformat zwischen verschiedenen A+W CAD Designer (Shapes)-Versionen ab CAD Designer 5.02. Mit diesem Format können Sie auch Teile der Stückliste austauschen.<br>⇨ Werkzeuge, "Teil einer Stückliste exportieren" auf Seite A-522 |
| **JPG** oder **Virtual Digitizing** | Diese Auswahl steht Ihnen nur dann zur Verfügung, wenn Sie mit Virtual Digitizing arbeiten. Dieses Format ist ein Bildformat. Wenn Sie ein Bild mit diesem Format öffnen, startet automatisch Virtual Digitizing.<br>⇨ Werkzeuge, “Virtuell digitalisieren" auf Seite A-455 |
| **VDP** | Dieses Format steht Ihnen nur dann zur Verfügung, wenn Sie mit virtuellem Digitalisieren arbeiten. Dieses Format ist eine Projektdatei des Programms Virtual Digitizing. Wenn Sie ein Bild mit diesem Format öffnen, startet automatisch Virtual Digitizing.<br>⇨ Werkzeuge, "Virtuell digitalisieren" auf Seite A-455 |

*Tab. A-44 Importformate*

Nach dem Import kann es nötig sein, dass die Konturen noch nachbearbeitet werden müssen, damit A+W CAD Designer (Shapes) die Daten korrekt weiterverarbeiten kann.

Nachfolgend finden Sie folgende Arbeiten beschrieben:

*   Daten importieren
*   Importierte Kontur nachbearbeiten

#### Daten importieren

Am Beispiel von DXF-Daten finden Sie hier die Erklärung des Datenimports. Grundsätzlich werden auch alle anderen Datenformate auf diese Weise importiert. Einzelne Arbeitsschritte können dabei von der folgenden Beschreibung abweichen.

1.  Erstellen Sie eine neue Datei. Betätigen Sie dazu `<Strg>` + `<N>`. A+W CAD Designer (Shapes) zeigt ein neues leeres Blatt an.

> **Daten aus Fremdformaten in eigene Datei importieren!**
> Grundsätzlich ist es auch möglich, DXF-Daten in eine bestehende CAD Designer-Zeichnung zu importieren. A+W empfiehlt, Fremdformate zunächst in eine eigene Datei zu importieren und ggf. zu ergänzen und anschließend die Datei bei Bedarf in andere, bestehende Dateien zu importieren.

2.  Wechseln Sie in die Ansicht `2D Import`.
3.  Wählen Sie im Menü `Datei` den Eintrag `Importieren` und dort die Option `DXF`. A+W CAD Designer (Shapes) zeigt den Dialog `DXF-Datei auswählen` an.
4.  Klicken Sie auf die Datei, die Sie ganz oder teilweise importieren wollen und betätigen Sie [Öffnen]. A+W CAD Designer (Shapes) zeigt den Dialog `Layer-Filter` an.
5.  Wählen Sie die Layer aus, die Sie importieren wollen.
6.  Betätigen Sie [Auswahl anzeigen], um in A+W CAD Designer (Shapes) anzuzeigen, welche Konturdaten die ausgewählten Layer enthalten.
7.  Betätigen Sie [Auswahl importieren], um die ausgewählten Konturdaten in die Datei zu importieren. A+W CAD Designer (Shapes) übernimmt die Geometriedaten (Koordinaten) der ausgewählten Konturen und stellt diese in der Ansicht `2D Import` dar. Konturen (z. B. Außenkonturen), die vollständig erkannt wurden, stellt A+W CAD Designer (Shapes) rot dar. Konturen (z. B. ein Ausschnitt), die noch nicht vollständig im Sinne von A+W CAD Designer (Shapes) sind, stellt A+W CAD Designer (Shapes) schwarz dar.
8.  Bearbeiten Sie die importierte Kontur bei Bedarf nach. A+W CAD Designer (Shapes) zeigt mit türkisfarbenen kleinen Kreuzen an, wenn eine Kontur noch geöffnet ist und nachbearbeitet werden muss.

**Ergänzende Informationen**
*   Softwarereferenz, "Datei auswählen..." auf Seite A-172
*   Softwarereferenz, "Layer-Filter" auf Seite A-174
*   "Importierte Kontur nachbearbeiten" auf Seite A-448

#### Importierte Kontur nachbearbeiten

Die nachfolgende Beschreibung geht davon aus, dass Sie Daten im Register `2D Import` oder `3D Import` importiert haben und diese noch nicht vollständig sind. A+W CAD Designer (Shapes) zeigt alle Konturen, die nicht weiterbearbeitet werden können, mit schwarzer Kontur an. Z. B. können alle geöffnete Konturen von A+W CAD Designer (Shapes) nicht weiterverarbeitet werden.

1.  Prüfen Sie, ob importierten Konturen schwarz angezeigt werden. Die Konturen, die A+W CAD Designer (Shapes) schwarz anzeigt, müssen Sie nachbearbeiten. Rot markierte Konturen hat A+W CAD Designer (Shapes) als vollständige Konturen erkannt.
2.  Wählen Sie das geeignete Werkzeug aus.

Folgende Werkzeuge stehen Ihnen zur Nachbearbeitung importierter Konturen zur Verfügung:

*   **Kontur schließen, die an mehreren Stellen geöffnet ist**
    *   ⇨ "Kontur schließen, die an mehreren Stellen offen ist" auf Seite A-255
*   **Kontur schließen, die nur an einer Stelle geöffnet ist**
    *   ⇨ "Einzelne Lücke in Kontur schließen" auf Seite A-256
*   **Randausschnitt in Kontur einfügen**
    *   "Ausschnitt schließen" auf Seite A-256

## Scheibe als Kontur digitalisieren

Die Arbeiten beim Digitalisieren einer Kontur unterteilen sich in folgende Arbeitsschritte:

*   Digitalisieren mit dem Digitalisiertisch
*   Virtuell digitalisieren
*   Nachbearbeiten in CAD Designer

### Digitalisieren mit dem Digitalisiertisch

Je nach dem, mit welchem Digitalisiertisch Sie arbeiten, können verschiedene Digitalisierverfahren anwenden. Standardfunktion ist das punktweise Digitalisieren, das von jedem Digitalisiertisch unterstützt wird. Dabei können Sie mit einer Lupe oder mit einem Stift digitalisieren. Das Ergebnis ist das selbe. Die zweite und einfachere Möglichkeit ist das Digitalisieren mit dem Digitalisierrad. Diese Möglichkeit wird nicht von jedem Digitalisiertisch unterstützt. Digitalisiert wird im A+W CAD Designer (Shapes) in der Ansicht `Punkte`. Egal wie Sie digitalisieren, die grundsätzliche Vorgehensweise in A+W CAD Designer (Shapes) ist identisch.

Nachfolgend finden Sie folgende Arbeiten beschrieben:

*   Außenkontur mit dem Rad digitalisieren
*   Außenkontur mit Stift oder Lupe digitalisieren
*   Innenkontur digitalisieren
*   Bohrlöcher digitalisieren

#### Außenkontur mit dem Rad digitalisieren

1.  Wechseln Sie in die Ansicht `Punkte`.
2.  Markieren Sie das Digitalisier-Werkzeug.
3.  Gehen Sie zum Digitalisiertisch und beginnen Sie mit dem Digitalisieren der Kontur.
    Setzen Sie das Rad an den Startpunkt und betätigen Sie die Start-Taste. Der Digitalisiertisch sendet jetzt in regelmäßigen Abständen die Positionsdaten des Digitalisierrades an A+W CAD Designer (Shapes). Umfahren Sie die Kontur. Unterbrechen Sie das Senden von Punkten, wenn Sie Störstellen (z. B. durch die Befestigung) erreichen. Setzen Sie nach einer Unterbrechung das Digitalisieren an geeigneten Stellen in der begonnenen Umlaufrichtung fort, bis Sie wieder den Startpunkt erreicht haben. A+W CAD Designer (Shapes) erkennt, dass die Kontur vollständig umfahren ist und deaktiviert das gewählte Werkzeug.
4.  Erfassen Sie, falls erforderlich, die zugehörige Innenkontur.
5.  Wenn Sie die Kontur vollständig erfasst haben, dann wechseln Sie in die Ansicht `Geometrie`. A+W CAD Designer (Shapes) führt eine Interpolation der Punkte zu Geraden und Radien durch.
    A+W CAD Designer (Shapes) korrigiert die Position der Punkte um den Radius des Digitalisierrades. Wenn eine solche Korrektur durchgeführt wurde, dann zeigt A+W CAD Designer (Shapes) an einer Kante ein P an. Wenn Sie auf das P klicken, dann zeigt A+W CAD Designer (Shapes) im Wertefenster an, um welchen Wert die Position der Punkte korrigiert wurden.
    Je nach Digitalisierung sind jetzt noch runde Ecken vorhanden, die Sie zuspitzen, oder kritische Stellen, die Sie beseitigen können.

**Ergänzende Informationen**
*   "Modelle und Vorlagen digitalisieren" auf Seite A-223
*   "Innenkontur digitalisieren" auf Seite A-451

**Weiterführende Arbeiten**
*   "Zwischen zwei Segmenten abrunden oder zuspitzen" auf Seite A-321
*   "Kritische Stellen erkennen und glätten" auf Seite A-457
*   "Kontur ausrichten" auf Seite A-460

#### Außenkontur mit Stift oder Lupe digitalisieren

1.  Wechseln Sie in die Ansicht `Punkte`.
2.  Markieren Sie das gewünschte Werkzeug.
3.  Gehen Sie zum Digitalisiertisch und markieren Sie die Stelle, an der Sie den ersten Punkt erfassen wollen. Dieser Punkt muss am Ende noch einmal digitalisiert werden. A+W CAD Designer (Shapes) erkennt dadurch das Ende der Konturerfassung.

> **Geeigneten Startpunkt wählen!**
> Wenn Sie nach dem Digitalisieren Ausgleichsbögen und -geraden manuell legen wollen, dann müssen Sie mit dem Startpunkt beginnen. Wählen Sie den Startpunkt daher so, dass Sie diesen in der Ansicht `Punkte` eindeutig identifizieren können.

4.  Beginnen Sie mit dem Digitalisieren der Kontur. Setzen Sie den Stift oder die Lupe an den Startpunkt und betätigen Sie die Sende-Taste. Der Digitalisiertisch überträgt den aktuellen Punkt an A+W CAD Designer (Shapes). Erfassen Sie auf diese Weise eine für die Konturerkennung erforderliche Anzahl von Punkten im Uhrzeigersinn. Die digitalisierten Punkte erscheinen nach und nach in der Ansicht `Punkte`. Je mehr Punkte Sie bei Bögen erfassen, desto genauer kann A+W CAD Designer (Shapes) den Bogen später berechnen.
