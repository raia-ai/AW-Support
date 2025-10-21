title: "DE-HB-AW_iShape"
source: "DE-HB-AW_iShape.pdf"
tags: ["A+W iShape", "Handbuch", "Software", "Glass", "Windows", "Doors", "Digitalisierung", "Schablonen", "CAD", "XTREAM"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This is the German user manual (Handbuch) for A+W iShape, a software solution for digitizing non-rectangular glass, window, and door templates (shapes). It explains how to use a smartphone camera with L-shaped reference objects to capture templates, process them in the iShape app, and then import the data into the A+W CAD Designer for further processing and manufacturing."
long_description: "This document serves as a comprehensive user guide for the A+W iShape software system. A+W iShape is designed to simplify and accelerate the process of digitizing physical templates (Schablonen) for non-rectangular glass, windows, and doors. The system uses a smartphone app in conjunction with physical, L-shaped reference objects equipped with QR codes. Users photograph the template with these reference objects placed on it. The app then processes the image, corrects for distortions, and generates a digital contour of the shape. This manual details the entire workflow, from the initial setup and requirements to best practices for taking photos, including proper lighting, background, and focus. It covers the functionalities of the iShape mobile app, such as the gallery for managing images, processing steps, and exporting data. Furthermore, it explains how to import the generated `.ishape` files into the A+W CAD Designer (Shapes) software for post-processing. This includes tools for smoothing curves, connecting segments, adjusting corners, and manually creating edges to finalize the design for production on CNC machines. The manual also provides details on configuring the XTREAM algorithm for contour smoothing. It is intended for end-users of the A+W iShape system."
---

# A+W iShape Handbuch

## Editorial

### Revisionsübersicht der Dokumentation

| Datum | Änderung |
| :--- | :--- |
| 08-2023 | Aktualisierung des Kapitels XTREAM |
| 06-2022 | App-Freigabe in der Version 2.0 |
| 03-2021 | Ersterstellung |

### Anmerkungen

Diese Veröffentlichung ist ausschließlich für Endanwender von A+W iShape gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Diese Dokumentation beschreibt die volle Ausbaustufe von A+W iShape.

### Urheberrechte

© 2024, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß des Lizenzvertrages ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung von A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

### Darstellungskonventionen

Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

| Stil | Bedeutung |
| :--- | :--- |
| *Kursiv* | sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Töpfe*. |
| **Fett** | sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: Geben Sie den Wert **0** ein. |
| > | Mit dem sogenannten Brotkrumenpfad ist der Weg gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B. *Anzeigen > Füllaufträge > Kontextmenü - Liste > Auftragsübersicht*. |
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

---

# A. Überblick

### Revisionsübersicht des Moduls

| Datum | Änderung |
| :--- | :--- |
| 08-2023 | Aktualisierung des Kapitels XTREAM |
| 06-2022 | App-Freigabe in der Version 2.0 |
| 03-2021 | Ersterstellung |

**Zu diesem Modul finden Sie folgende Kapitel**
⇨ Tutorial

## Tutorial

### In diesem Kapitel finden Sie folgende Themen:

*   Dokumentation
*   Grundlagen
*   Muster - Bilder
*   Die Applikation
*   iShape-Dateien im A+W CAD Designer

### Dokumentation

A+W iShape bietet eine einfache und flexible Lösung, um die digitale Daten aus Modellschablonen (nicht rechteckigen Scheiben) zu generieren. Die Digitalisierung von Scheiben erfolgt mit Hilfe einer Kamera.

Die Schablone wird mit den L-förmigen Referenzobjekten bestückt und anschließend mit einer High-End-Smartphone-Kamera fotografiert. Die Referenzobjekte, hochwertige Präzisions-Stücke aus Metall, werden auf die Schablone gelegt oder an ihr befestigt. Sie dienen dazu, eventuelle Verzerrungen beim Fotografieren zu korrigieren. Die Objekte sind zusätzlich mit einem QR-Code ausgestattet, der eine automatische Erkennung der Objekte ermöglicht und damit eine weitere Konfiguration erübrigt.

Das Besondere: Im Gegensatz zu älteren Lösungen ist keine Kalibrierung der verwendeten Kamera erforderlich! A+W iShape funktioniert mit jeder guten Smartphone-Kamera. Nachdem das Foto gemacht und das Bild bearbeitet wird, kann das erkannte Modell direkt auf dem Smartphone kontrolliert und weitergegeben werden.

Die Weiterbearbeitung der Dateien erfolgt im A+W CAD Designer (Shapes): hier können Maschinendaten oder DXF-Dateien erzeugt werden. Der gesamte Erfassungsprozess dauert nur wenige Minuten.

Diese Beschreibung zum A+W iShape zeigt Ihnen, wie Sie das Modul verwenden können und auf was Sie bei der Arbeit mit der Kamera achten müssen.

#### Voraussetzungen

Das Modul A+W iShape setzt die Nutzung (Installation) der aktuellen A+W CAD Designer (Shapes) Version voraus. Auch die Anwender-Kenntnisse des A+W CAD Designer (Shapes) sind von Vorteil. Das Installieren und Konfigurieren von A+W iShape soll bereits erfolgt sein.

### Grundlagen

Die Entstehung der A+W iShape basiert sich auf der Besonderheit in der Produktion: Glasverarbeiter erhalten zur Herstellung einer nicht rechteckigen Glasscheibe (Shape, Freie Form) von ihren Kunden oft eine Handzeichnung oder eine Holz-, Spanplatten- oder Kartonschablone. Diese Scheiben können mit A+W iShape in ihrer Form erkannt und digitalisiert werden.

Die erzeugte Serie von Punkten (Kontur) wird anschließend im A+W CAD Designer (Shapes) geöffnet und kann mit Hilfe der im A+W CAD Designer (Shapes) vorhandenen Werkzeuge korrigiert werden. Damit wird letztendlich die finale Kontur entsprechend den Wünschen der Anwender erzeugt. Beispielsweise können hier Ecken abgerundet werden oder die Kontur an bestimmten Kanten auch um vorgegebene Distanzen verlängert werden. All dies baut auf bekannten Funktionalitäten des A+W CAD Designer (Shapes) auf, so dass hier auf die entsprechende Dokumentation verwiesen wird. Anschließend können diese Dateien in der Produktion auf CNC-Maschinen verwendet werden.

**Ergänzende Information**
In den folgenden Kapiteln wird beschrieben und anhand einigen Bilder gezeigt, welchen Anforderungen die aufgenommenen Bilder entsprechen müssen, um die Modelle möglichst einfach und schnell zu digitalisieren.

*   "Verwendung der Lineale" auf Seite A-14
*   “Anforderungen an Bilder" auf Seite A-20
*   "Befestigung" auf Seite A-27
*   "Muster - Bilder" auf Seite A-31

### Verwendung der Lineale

Um die Modell-Konturen zu erkennen, werden in A+W iShape verschiedene Lineale verwendet. Dabei handelt sind um winkelförmige Lineale mit einem QR-Code. Dieser QR-Code wird auch DMC (Data Matrix Code) genannt.

Im Folgenden erhalten Sie die Beschreibung und die richtige Verwendung der Lineale:

*   "Lineal - Größen" auf Seite A-14
*   "Anzahl an Linealen" auf Seite A-15
*   "Lineal - Abstand zur Kante" auf Seite A-16
*   "Lineal - Platzierung" auf Seite A-17
*   "Das Lineal als Dreieck nutzen" auf Seite A-18
*   "Freilegen der Lineale" auf Seite A-19

#### Lineal - Größen
Es gibt drei verschiedene Lineal-Größen für A+W iShape:

*   Größe L (DIN A3)
*   Größe M (DIN A4)
*   Größe S (DIN A5)

Die Lineale können beliebig kombiniert werden. Der DMC muss dabei klar erkennbar sein. Zu beachten wäre unter anderem, dass je größer das Bild ist, desto weiter ist die Entfernung von der Kamera und somit die QR-Codes von den kleineren Linealen schlecht erkennbar wären.

Zu beachten ist unter anderem, dass der QR-Code von den kleinen Linealen auf großen Modellen schlecht erkennbar ist. Daher sollten die Lineale der Größe S eher auf kleinen Modellen genutzt werden.

#### Anzahl an Linealen
Die Anzahl an verwendeten Linealen hängt von der Modellgröße ab. Je größer das Modell ist, umso wichtiger ist es, genügend Lineale auf dem Modell zu platzieren. D.h., sechs Lineale für ein großes Modell sind genug, während ein Lineal niemals ausreichend ist. Auch drei Lineale reichen selten aus, eventuell nur bei sehr kleinen Modellen.

Die Anzahl der Lineale richtet sich auch nach der Anzahl der Ecken im Model.

#### Lineal - Abstand zur Kante
Das Lineal (L-förmiges Werkzeug) wird auf das Modell mit einem Abstand von ca. 0,5 cm (1/4 Inch) zur Kante gelegt.

#### Lineal - Platzierung
Die Lineale werden entlang der Kontur platziert. Auch alle Ecken der Schablone müssen mit den Linealen abgedeckt werden. Die äußersten Referenzpunkte der Lineale bilden zusammen die konvexe Hülle. Bei der Lineal-Platzierung sollte darauf geachtet werden, dass diese maximal ist.

#### Das Lineal als Dreieck nutzen
Die Kanten des Lineals bilden ein Dreieck, deren gesamte Oberfläche sich innerhalb des Modells befinden muss. Der Inhalt des aufgespannten Dreiecks wird als Orientierung genutzt, welche Farbe das Modell hat. Die Lineale sollten so gelegt werden, dass sich keine Beschriftungen, Sticker oder Ähnliches innerhalb dieses Dreiecks befinden. Dies könnte die Farbgebung verfälschen.

#### Freilegen der Lineale
Alle Lineale werden so platziert, dass die Seiten der Lineale weder ineinander, noch überlappend greifen.

### Anforderungen an Bilder
Um die Bilder in A+W iShape zu überführen, müssen folgende Punkte beachtet werden:

*   "Bildeigenschaften" auf Seite A-21
*   "Bildfokus" auf Seite A-22
*   "Bildhintergrund" auf Seite A-23
*   "Bildkontrast" auf Seite A-24
*   "Bildausleuchtung" auf Seite A-25
*   "Bildqualität" auf Seite A-26

#### Bildeigenschaften
Im Bild sollten das gesamte Modell und nur etwas von dem Hintergrund deutlich sichtbar sein. Es ist zu vermeiden, zu viel Hintergrund aufzunehmen oder Teile vom Modell abzuschneiden. Auf keinen Fall dürfen die Referenzpunkte oder der Datenmatrix-Code auf dem Lineal abgeschnitten werden.

#### Bildfokus
Um den Fokus der Kamera voll auszunutzen, kann ein einfaches, flaches Objekt in der Mitte der Vorlage positioniert werden.

#### Bildhintergrund
Das Bild sollte mit einem möglichst homogenen Hintergrund gemacht werden. Der helle, z. B. graue Hintergrund für eine Bildaufnahme ist am Besten. Heterogene Hintergründe (z.B. Teppichboden, Steine) sind ungeeignet.

#### Bildkontrast
Zwischen dem Modell und dem Hintergrund sollte es genügend Kontrast geben. Vermeiden Sie helle Modelle vor hellen Hintergründen. Bei hellen Modellen wird ein dunkler Hintergrund wie schwarzer Stoff oder Filz empfohlen. Dies stellt einen optimalen Kontrast sicher und vermeidet ungewollte Schattenwürfe des Modells.

#### Bildausleuchtung
Das Bild sollte weder zu hell (überbelichtet) noch zu dunkel (unterbelichtet) sein. Vermeiden Sie Schatten oder Spiegelungen (Reflexionen) auf dem Bild.

#### Bildqualität
Versuchen Sie, nicht zu wackeln, während Sie das Bild aufnehmen und warten Sie (wenn nötig) bis die Kamera fokussiert hat. Bei einem verwackelten Bild kann der Datenmatrix-Code nicht gelesen werden.

### Befestigung
Um Bilder von den benötigten Schablonen und den darauf befindlichen Linealen machen zu können, müssen sowohl die Schablonen als auch die Lineale oft befestigt werden.

In den folgenden Kapiteln wird beschrieben, was Sie dabei beachten müssen:
*   "Befestigungsmaterial" auf Seite A-28
*   "Aufstellung der Schablonen" auf Seite A-30

#### Befestigungsmaterial
Zur Befestigung der Lineale an den Schablonen können Pinn-Nadeln verwendet werden. Bitte beachten Sie, dass es sich um Pinn-Nadeln mit flachem Kopf handeln muss. Bei flachköpfigen Pinn-Nadel muss auch auf die Auswahl der Farbe für die Pinn-Nadeln geachtet werden: weiße oder sehr helle Nadeln können als Markierungspunkte der Linealen erkannt werden und so den Konfidenz-Wert möglicherweise verfälschen. Wenn Sie Pinn-Nadeln verwenden, müssen dafür Löcher in die Lineale gebohrt werden. Bitte achten Sie darauf, die Löcher nur zwischen die weißen Punkte zu setzen.

Im Weiteren dürfen weder Lineale noch Schablonen-Ränder überklebt werden. Klebebandstreifen können jedoch als eine alternative Befestigungsart verwendet werden, wenn sie doppelseitig kleben und auf der Rückseite der Lineale oder Schablonen befestigt werden.

#### Aufstellung der Schablonen
Um die Schablonen ordnungsgemäß zu fotografieren, müssen diese in der Regel gut platziert bzw. aufgestellt werden. Gute Möglichkeiten die Schablonen zu platzieren kann eine Wand bieten. Sie können die Schablonen an der Wand anlehnen, eine Art Aufstellkante herrichten oder diverse Hilfsmittel für die Aufstellung benutzen, z. B. Schrauben. Die Aufstellung der Schablone ist einfacher, wenn die Grundfläche leicht geneigt ist.

### Muster - Bilder
Im Folgenden sind einige Muster-Bilder aufgeführt. Bei diesen Musterbeispielen handelt es sich um verschiedene Schablonen und mögliche L-Platzierungen, die sehr gute Ergebnisse liefern.

---

### Die Applikation
Die A+W iShape-App wurde in der Version 2.0 sowie in der App-Darstellung als auch in der Bedienung überarbeitet. Die Neuerungen können Sie dieser Dokumentation entnehmen. Im Grunde kann die Applikation intuitiv bedient werden. Die Arbeit mit A+W iShape setzt jedoch das allgemeine Wissen eines Smartphones voraus.

In den folgenden Abschnitten werden die einzelnen Bedien- und Anzeigeelemente erklärt:
*   "Anzeigeelemente" auf Seite A-34
*   "Bedienung" auf Seite A-35
*   "App - Aktivierung" auf Seite A-36
*   "Galerie" auf Seite A-37
*   "Verarbeitete Bilder" auf Seite A-40

> **App-Ausrichtung**
> Die App ist in der Bedienung permanent auf Hochformat gestellt. Lediglich in der Zoom-Funktion kann die Anzeige auf Querformat gedreht werden.
> ⇨ "Kontur- Vollbild und Zoom" auf Seite A-51

#### Anzeigeelemente
In der folgenden Tabelle sind alle Symbole beschrieben, die in der Applikation durchgehend verwendet werden:

| Symbol | Name | Bedeutung |
| :--- | :--- | :--- |
| 🖼️ | Galerie | Dieses Symbol signalisiert die Galerie-Ansicht. ⇨ "Galerie" auf Seite A-37 |
| 📷 | Kamera | Über dieses Symbol starten Sie die Aufnahme mit der Kamera. ⇨ "Bild-Aufnahme" auf Seite A-48 |
| 📥 | Bild-Import | Über dieses Symbol starten Sie die Bilder-Freigabe aus der Kamera-Ansicht. ⇨ "Bilder-Import" auf Seite A-49 |
| ⚡ | Kamera-Blitz | Über dieses Symbol schalten Sie den Blitz für die Kamera an und aus. ⇨ "Bild-Aufnahme" auf Seite A-48 |
| ⚙️ | Einstellungen | Über das Zahnrad-Symbol gelangen Sie zu den App-Einstellungen. ⇨ "Einstellungen" auf Seite A-52 |
| < | Zurück | Über dieses Symbol kehren Sie zurück zur vorherigen Seite. |
| ☑️ | Checkbox-Markierung | Über das Checkbox-Symbol wählen Sie ein oder mehrere Bilder bzw. Dateien und können weitere Aktion ausführen, z. B. exportieren oder löschen. |
| 📤 | Freigeben für... | Über dieses Symbol können Sie die Bilder oder Dateien exportieren. ⇨ "Bilder-Import" auf Seite A-49 |
| 🗑️ | Mülleimer | Über dieses Symbol können Sie markierte Bilder löschen. ⇨ "Bilder löschen" auf Seite A-43 |
| 🔎+ | Ansicht vergrößern | Über dieses Symbol können Sie die Bildansicht vergrößern. ⇨ "Kontur- Vollbild und Zoom" auf Seite A-51 |
| 🔎- | Ansicht verkleinern | Über dieses Symbol können Sie die Bildansicht wieder verkleinern. ⇨ "Kontur- Vollbild und Zoom" auf Seite A-51 |

Diese Symbole können abhängig vom Kontext in folgender Darstellung erscheinen:
*   **blau**: aktiv = Tippen löst eine entsprechende Aktion aus,
*   **grau**: inaktiv = Die Aktion ist aktuell nicht verfügbar.

#### Bedienung
In diesem Kapitel wird die Schrittreihenfolge beschrieben, wie Sie mit der A+W iShape - App arbeiten können. Diese Beschreibung setzt voraus, dass die App bereits erworben und auf einem Smartphone installiert ist.

**Diesen Ablauf sieht die App vor:**
1.  Bereiten Sie Ihre Schablone vor, die Sie über die App verarbeiten möchten.
2.  Platzieren Sie zur Erkennung notwendige Lineale auf der Schablone. Beachten Sie dabei die Anforderungen, die im folgenden Kapitel beschrieben sind: ⇨ "Verwendung der Lineale" auf Seite A-14
3.  Bereiten Sie die Schablone mit den Linealen zur Bild-Aufnahme vor: ⇨ "Anforderungen an Bilder" auf Seite A-20
4.  Fotografieren Sie die vorbereitete Schablone oder führen Sie die Schritte 5-6 durch.
5.  Starten Sie die App
6.  Wählen Sie über die App die Möglichkeit zur Bildaufnahme ([Kamera]-Symbol) aus: ⇨ "Bild-Aufnahme" auf Seite A-48
7.  Benutzen Sie die App-Galerie für die Übersicht und Verarbeitung der Bilder: ⇨ "Galerie" auf Seite A-37
8.  Lassen Sie so die Bilder in der App verarbeiten: ⇨ "Bild verarbeiten" auf Seite A-44
9.  Überprüfen Sie die Konfidenz der erkannten Schablone. Sie können vorangehende Schritte beliebig wiederholen, bis Sie das gewünschte Ergebnis erzielen: ⇨ "Schablonen - Konfidenz" auf Seite A-46
10. Geben Sie die bearbeitete Bild-Datei frei, um diese anschließend in A+W CAD Designer (Shapes) zu bearbeiten: ⇨ "Konturanzeige" auf Seite A-50, ⇨ "iShape-Dateien im A+W CAD Designer" auf Seite A-58
11. Arbeiten Sie alle Schablonen auf diese Art und Weise ab.
12. Schließen Sie die App.

#### App - Aktivierung
In der neuen App-Version kommt es beim erstmaligen App-Start zu einer Aktivierungs-Aufforderung. Beim Erwerben der App wird Ihnen ein QR-Code zugestellt, den Sie zur Aktivierung scannen müssen. Nach der erfolgreichen Aktivierung kann die Applikation verwendet werden.

#### Galerie
Die App startet mit einer Galerie, die in folgende Bereiche aufgeteilt ist:
*   Nicht verarbeitet
*   Verarbeitet.

Zuerst sind die beiden Bereiche leer. Um die Bilder in der App zu verarbeiten, müssen diese in der App zur Verfügung gestellt werden. Sie können die zu verarbeitenden Schablonen mit dem Smartphone fotografieren oder über die Smartphone-Import Funktion bereits aufgenommene Bilder hochladen. Diese Möglichkeiten sind in den folgenden Kapiteln beschrieben:
*   "Bild-Aufnahme" auf Seite A-48
*   "Bilder-Import" auf Seite A-49

Die neuen hochgeladenen Bilder werden im Register **Nicht verarbeitet** aufgelistet. Durch einfaches Tippen auf das vorhandene Bild können Sie dieses weiterbearbeiten.

Verarbeitete Bilder sind im entsprechenden Bereich gelistet. Mit dem Tippen auf **[Verarbeitet]** wechseln Sie in die entsprechende Ansicht.

**Nicht verarbeitete Bilder**
In dem Bereich **Nicht verarbeitet** werden die Bilder aufgelistet, die nun zur Verarbeitung anstehen. Mit dem einfachen Tippen auf das gewünschte Bild geben Sie dieses weiter zur Verarbeitung. Sie werden zur weiteren Seite geführt. Mit einem Tippen und Halten markieren Sie das gewünschte Bild und haben so die Möglichkeit, die Bilder zu löschen.

**Verarbeitete Bilder**
Im Bereich **Verarbeitet** bekommen Sie eine Übersicht über alle zuletzt verarbeiteten Bilder angezeigt. Sofern Sie die Bilder verarbeitet haben, erscheint im Bereich Verarbeitet die entsprechende Übersicht.

In der neuen App-Version erhalten Sie für jedes verarbeitete Bild die erreichte Konfidenz über die Schablonen-Erkennung, die mithilfe eines farblichen Ring-Diagramms dargestellt wird.

| Symbol | Name | Bedeutung |
| :--- | :--- | :--- |
| 🟢 | Grüner Ring | Dieses Symbol signalisiert die Modellerkennung im Bereich 80 bis 100%. Der Prozentsatz in der Mitte des Symbols gibt die Konfidenz an. |
| 🟡 | Gelber Ring | Dieses Symbol signalisiert die Modellerkennung im Bereich 60 bis 80%. Der Prozentsatz in der Mitte des Symbols gibt die Konfidenz an. |
| 🔴 | Roter Ring | Dieses Symbol signalisiert die Modellerkennung im Bereich 10 bis 60%. Der Prozentsatz in der Mitte des Symbols gibt die Konfidenz an. |
| 🔴 ! | Roter Ring mit Ausrufezeichen | Dieses Symbol signalisiert, dass die Modellerkennung unter 10% liegt bzw. nicht durchgeführt werden konnte. |

Mit einem längeren Tippen auf die gewünschten Datei/-en markieren Sie diese und haben so die Möglichkeit, die Datei/-en zu löschen.

#### Bilder löschen
In den beiden Bereichen der Galerie können Sie die aufgelistete Bilder jederzeit entfernen.

Zum Löschen können Sie die bestehende Datei zur Seite wischen. Dabei wird genau ein Bild aus der App entfernt.

Um mehrere Bilder gleichzeitig zu löschen, tippen Sie ein Bild an und halten Sie mit dem Finger kurz an. Es werden links von den Bildnamen Checkboxen angezeigt. Aktivieren Sie diese Checkboxen für alle Bilder, die gelöscht werden sollen. Anschließend verwenden Sie das Mülleimer-Symbol. Dabei werden alle markierte Bilder aus der App gelöscht.

Tippen Sie das Symbol [x] an, um den aktuellen Dialog zu schließen und zur App zurückzukehren.

> **Bilder löschen**
> Wenn Sie die Bilder in der App löschen, werden sie auch im Dateiexplorer Ihres Smartphons gelöscht!

#### Bild verarbeiten
Die Auswahl eines Bildes in der Galerie führt Sie zur weiteren Seite, in der Sie folgende Möglichkeiten haben:
*   Das ausgewählte Bild verarbeiten (Schaltfläche [Verarbeiten]),
*   Zur Galerie zurückkehren (Symbol [<]),
*   Das ausgewählte Bild freigeben (Symbol [Freigeben für]).

#### Lineal - Auswahl
Um die Schablone möglichst schnell verarbeiten zu können, benötigt die App die Angabe der Anzahl an Linealen. Wischen Sie mit dem Finger hoch oder runter, um die passende Angabe zu treffen. Bestätigen Sie Ihre Auswahl. Alternativ können Sie die Verarbeitung abbrechen, um zum vorherigen Schirm zurückzukehren. Nach der Bestätigung der Anzahl an Linealen wird das aktuelle Bild in der A+W iShape - App verarbeitet.

#### Schablonen - Konfidenz
Eine Rückmeldung über die mögliche Ursache, wie die Schablonen-Erkennung ausgefallen ist, erhalten Sie durch die entsprechenden Hinweise. Diese Information wird Ihnen direkt nach der Bild-Verarbeitung angezeigt, oder wenn Sie alternativ auf das bereits verarbeitete Bild in der Galerie tippen.

In der dazugehörigen Detail-Ansicht bekommen Sie folgende Information:
*   **Die Bilddarstellung**. Mit Tippen auf das Vergrößerungs-Symbol können Sie das Bild vergrößern, mit Doppel-Tippen können Sie das Bild zoomen.
*   **Der Dateiname** und das Datum der letzten Verarbeitung.
*   **Konfidenzwert** als Ring-Diagramm mit dem Prozentsatz.
*   **Angabe der Lineale** (z.B. L 6/6 bedeutet, dass 6 von 6 Linealen erkannt wurden).
*   **Kontur-Schalter** (grüne Linie auf der Schablone) zum An-und Ausschalten,
*   **Liste mit Hinweisen**. Für weitere Hinweise, falls diese vorhanden sind, scrollen Sie das Bild nach oben.
*   Über das **[Export]**-Symbol können Sie das Bild freigeben.

**Mögliche Hinweise:**
*   Ein oder mehrere L-Referenzobjekte wurde(n) nicht erkannt. Machen Sie ein Foto mit allen L-Referenzobjekten im Fokus.
*   Die Schablone ist nicht vertikal zentriert. Bewegen Sie die Kamera nach unten/oben.
*   Die Schablone ist nicht horizontal zentriert. Bewegen Sie die Kamera nach rechts/links.
*   Bewegen Sie die Kamera weiter von der Schablone weg.
*   Nehmen Sie ein Bild mit einer zentrierten Perspektive auf.
*   Verwenden Sie mehr L-Referenzobjekte.
*   Bewegen Sie die L-Referenzobjekte näher an die Kontur heran oder decken Sie mehr Schablonenfläche mit den L-Referenzobjekten ab.
*   Versuchen Sie eine symmetrischere Anordnung der L-Referenzobjekte um die Bildmitte herum

Zum Verlassen, bzw., zum Zurückkehren zum vorherigen Bildschirm tippen Sie bitte [<].

#### Bild-Aufnahme
Über das [Kamera] - Symbol nehmen Sie das Bild auf. Positionieren Sie die Kamera richtig. Beachten Sie dabei die Anforderungen an Bilder und die richtige Verwendung der Lineale.

Mit dem Tippen auf das Aufnahme Symbol wird der Bildaufnahme-Prozess ausgelöst. Sobald das Bild von der Kamera aufgenommen wurde, werden Sie auf die nächste Seite weitergeleitet. Die Weiterführung zur nächsten Seite erfolgt, nur sofern die Einstellung- **Mehrere Bilder** deaktiviert ist. Ansonsten können Sie mehrere Bilder hintereinander machen, ohne dass Sie weitergeleitet werden. Diese Einstellung ist in der aktuellen App-Version Standard.

Über das [Blitz] - Symbol kann optional der Kamera-Blitz angeschaltet werden, falls es zu dunkel ist. Zu beachten ist, dass der Blitz auch für Reflexionen sorgen kann.

Über das [Öffnen] - Symbol können Sie ein bereits vorhandenes Bild in die App importieren.

Über das [<] - Symbol kehren Sie zur vorherigen Seite zurück.

#### Bilder-Import
Über den Bild - Import können Sie vorhandene Bilder in die A+W iShape - App übernehmen. Hier öffnet sich der standardmäßige Datei-Explorer Ihres Smartphones. Im oberen Bildschirm-Bereich haben Sie die Standard-Funktionen Ihres Smartphones zur Verfügung, wie z. B.: Speicherort-Auswahl, Suche, Ansichtsänderung.

Durch ein Tippen auf das Bild, wählen Sie dieses aus, um es in die A+W iShape - App zu importieren. Wenn Sie in Ihrem Smartphone eine Mehrfachauswahl betätigen können, soll hier beachtet werden, dass eine solche Mehrfach-Auswahl in A+W iShape nicht unterstützt wird, es wird immer nur ein Bild importiert.

#### Konturanzeige
Wenn Sie die Option **Kontur an** in den Einstellungen angestellt haben, wird das verarbeitete Modell mit einer leuchtenden Linie umrandet. Dabei können Sie das Ergebnis der Verarbeitung visuell überprüfen. Diese Option können Sie auch jeder Zeit ein- oder ausblenden.

#### Kontur- Vollbild und Zoom
In dieser Ansicht haben Sie die Möglichkeit, das Bild im Vollbild-Modus darzustellen. Tippen Sie dafür auf [Großansicht/an]-Symbol. Zum Vollbild-Modus auszuschalten, tippen Sie auf [Großansicht/aus]-Symbol.

In der Bild-Verarbeitung sowie im Vollbild-Modus können Sie die Bilder auch ranzoomen. Tippen Sie zweifach auf das Bild oder berühren Sie das Display mit zwei Fingern, und ziehen Sie die Finger auseinander, um den Bildbereich zu vergrößern. So vergrößern Sie das Bild bzw. den Bildausschnitt wie gewünscht. Im Vollbildmodus kann das Smartphone außerdem im Querformat verwendet werden.

Zum Verkleinern ziehen Sie die beiden Finger wieder zusammen oder tippen Sie erneut zweifach.

#### Einstellungen
Über das Zahnrad-Symbol gelangen Sie zur Seite mit der Einstellungen. Hier können Sie folgende Einstellungen vornehmen:

*   **Anzahl der L-Referenzobjekte**: Voreinstellung für die Anzahl der Lineale, die standardmäßig vor der Bildverarbeitung vorgeschlagen werden. Dieser Wert kann vor jeder Bildverarbeitung bei Bedarf geändert werden.
*   **Vorschaubild der Kamera**: Vorschauanzeige in der Kamera. Hier legen Sie fest, auf wie viel Prozent die Vorschau begrenzt wird. Standardmäßig liegt der Wert bei 70%.
*   **Mehrere Bilder: an/aus**: Das Einschalten der Mehrfach-Aufnahme. Ist der Modus der Mehrfach-Aufnahme aktiviert, können mehrere Bilder hintereinander aufgenommen werden. Alle aufgenommenen Bilder werden in der Galerie gespeichert und können nachträglich verarbeitet werden.
*   **Kontur an/aus**: Voreinstellung für die Konturanzeige. Standardmäßig ist der Regler aktiv und die Kontur wird angezeigt.
*   **Verarbeitungsrückmeldungen an/aus**: Diese Einstellung deaktiviert jegliches Feedback außer der Anzahl an Linealen. Es werden kein Konfidenzwert und keine Hinweise mehr angezeigt.
*   **Sprache**: Ändern Sie die App-Sprache. Als Standard wird die Sprache gewählt, die Sie auf Ihren Smartphone festgelegt haben.
*   **Information**: Zeigt Informationen über die App-Installation an (Gerätekennung, Gerätename, App Version, Digitizing Version).
*   **Hilfe**: Bietet Kontaktinformationen zu A+W Software GmbH und Copyright-Infos.
*   **Logdateien**: Ermöglicht das Weiterleiten von Logdateien, z.B. per E-Mail.

> **Änderungen in den Einstellungen**
> Die geänderten Einstellungen sind in der App sofort aktiv. D.h., wenn Sie z.B., Sprache ändern, schaltet die App sofort nach dem Speichern auf die entsprechende Sprache um.

---

### iShape-Dateien im A+W CAD Designer

In A+W iShape digitalisierte Dateien können weiter in A+W CAD Designer (Shapes) bearbeitet werden. Im Folgenden sind einige grundlegende Schritte beschrieben:
*   "iShape-Datei öffnen" auf Seite A-59
*   "iShape-Datei bearbeiten" auf Seite A-60
*   "Glättung" auf Seite A-61
*   "Manuelle Erstellung der Kanten" auf Seite A-68
*   "Sichtbarkeit des Hintergrundbildes" auf Seite A-70
*   "Anpassung von XTREAM" auf Seite A-72

#### iShape-Datei öffnen
Eine Datei mit der Dateiendung `.ishape` kann im A+W CAD Designer (Shapes) entweder über den entsprechenden Menüaufruf *Datei > Öffnen* oder direkt über das markierte Icon geöffnet werden.

Daraufhin startet der Windows-Standarddialog *Öffnen*. Um die `.ISHAPE` öffnen zu können, klappen Sie das Feld für den Dateityp auf und wählen Sie File (*.ISHAPE) aus. Anschließend kann die ISHAPE-Datei geöffnet werden.

#### iShape-Datei bearbeiten
**Werkzeuge für die Nachbearbeitung**
Für die A+W iShape - Modell-Nachbearbeitung werden in A+W CAD Designer (Shapes) folgende Werkzeuge gebraucht:

| Symbol | Name | Beschreibung |
| :--- | :--- | :--- |
|  JOIN | JOIN | Zwei Segmente verbinden (Punkt zwischen Segmenten auswählen). |
| SPLIT | SPLIT | Ein Segment in zwei Segmente teilen (Segment auswählen, Punkt setzen). |
| RNDEDGE | RNDEDGE | Runden eines Segments (Segment zwischen Segmenten auswählen). |
| DESIGNC | DESIGNC | Verschieben eines Segments nach innen/außen mit Anpassung der Ecken. |
| MSEGORTH | MSEGORTH | Verschiebung eines Punktes senkrecht zum Segment (kann mit den Tasten + und - justiert werden). |
| MSEGTANG | MSEGTANG | Verschiebung eines Punktes tangential zum Segment (kann mit den Tasten + und - justiert werden). |
| DIGLINE | DIGLINE | Erstellen der besten Linie aus digitalisierten Punkten. |
| DIGARC | DIGARC | Erstellen der besten Kurve aus digitalisierten Punkten. |

> **A+W CAD Designer (Shapes) Konfiguration**
> Wenn nicht alle Werkzeuge auf der Oberfläche im A+W CAD Designer (Shapes) enthalten sind, müssen diese in der sn.ini ergänzt werden.

#### Glättung
Um die iShape-Datei in A+W CAD Designer (Shapes) zu bearbeiten, werden einige Schritte notwendig. Die Vorgehensweise und die dazu benötigten Werkzeuge werden anhand der Glättung einer Form erklärt.
*   **Mehrere Segmente verbinden**: Mit dem Werkzeug **JOIN** wählt man einen Punkt aus, dessen anliegende Segmente verbunden werden sollen. Dieser Schritt muss unter Umständen mehrfach wiederholt werden.
*   **Runde Ecken auflösen**: Um die Rundung einer Ecke aufzulösen, wählt man das Werkzeug **RNDEDGE** und grenzt das Segment der Ecke ein. Setzt man den Wert auf 0, wird die Ecke scharf. Das Ganze funktioniert auch umgekehrt, falls man die Rundung vergrößern möchte, indem man einen größeren Wert eingibt.
*   **Kurven korrigieren: Möglichkeit 1**: Liegt die Kontur nicht genau entlang der Kante, kann sie korrigiert werden. Zuvor wird das Segment mit dem **SPLIT**-Werkzeug in zwei Segmente unterteilt. Das Werkzeug **DESIGNC** verschiebt das markierte Segment parallel und passt die umliegenden Segmente an. Je nachdem, ob man einen positiven oder negativen Wert eingibt, verschiebt sich das Segment nach außen bzw. innen.
*   **Kurven korrigieren: Möglichkeit 2**: Eine andere Möglichkeit, Kurven zu bearbeiten, bieten die Werkzeuge **MSEGORTH** und **MSEGTANG**. Damit lassen sich Punkte entweder senkrecht oder tangential zum ursprünglichen Segment verschieben. Hat man einen Wert festgelegt, lässt sich die Verschiebung noch über die Tasten + und - justieren.
*   **Manuelle Erstellung der Kanten**: Es ist auch möglich, die Kanten manuell zu erstellen. Dazu werden die Werkzeuge **DIGLINE** und **DIGARC** benötigt. Diese erstellen die beste Linie oder den besten Bogen entlang der markierten Punkten. Dazu markiert man den Start- und den Endpunkt.

#### Sichtbarkeit des Hintergrundbildes
Über den Menüpfad *Ansicht > Einstellungen > Background image > Opacity* kann die Sichtbarkeit des Hintergrundbildes eingestellt werden (20% - 100%).

Die Menüeinträge können für einen schnelleren Zugriff auch dem Kontextmenü hinzugefügt werden. Dazu werden dem Abschnitt `[PopUp]` der `SN.ini` die Einträge `MenuID` und `AdditionalTextForXXXXX` hinzugefügt.

**Beispiel:**
```ini
[PopUp]
MenuID = 32925
MenuID = 32928
AdditionalTextFor32925 = Opacity
AdditionalTextFor32928 = Opacity
```
Die Menükennungen sind 32924 - 32928 für die Einträge 20% - 100% in 20%-Schritten.

Zudem wurde der `SN.INI` ein neuer Parameter hinzugefügt:
```ini
[Digi]
BackgroundImageOpacity = 0.2
; Mögliche Werte: 0.0 - 1.0
```
Dieser Wert wird beim Start von A+W CAD Designer (Shapes) verwendet.

#### Anpassung von XTREAM
XTREAM ist der Algorithmus, der zur Kantenglättung verwendet wird. Das Standardverfahren eignet sich insbesondere für glatte Formen und wurde durch eine verbesserte Eckerkennung aufgewertet. Das Verfahren lässt sich in der `SN.INI`-Datei durch verschiedene Parameter manipulieren.

> **Anpassungen in sn.ini**
> Die Einstellungen in der Konfigurationsdatei sn.ini sollte nur informativ wahrgenommen werden und nur vom Systemadministrator bewusst umgestellt werden.

**Wichtige Schalter für XTREAM in `sn.ini`:**
```ini
[XTREAM]
AccuracyForToolAngZero = 0.1 mm
CAPTURERADIUS = 1.125
CloseOpenShapes = 1
DEFAULTBORDER = 10.
DigiWheelForCheckpointsRadius = 6.35
DigiWheelRadius = 6.35
MAXCORNERANGLE = 25.
MAXRADIUS = 10000.
MINDIGIDIST = 0.75
MINIINTERIORRADIUS = 125.
NORMACCURACY = 1.25
SegmentInfo = 0
ForceTangentAngleZero = 0
ShowPointsForSelection = 1
LineLimit = 0.5
PointsPerInterval = -1
IntervalLength = -1
IShapeDoModel = 0
FINDCORNERS = 1
```
*   Das Setzen des Parameters `CloseOpenShapes` auf 1 erzwingt, dass die gefundene Kontur geschlossen wird. Dies ist wichtig für den späteren Import der SN/DXF-Datei in A+W Business / A+W Enterprise.
*   Durch Veränderung des Parameters `NORMACCURACY` kann die Genauigkeit der Glättung angegeben werden. Ein Wert rund um 1 hat sich bisher als gute Einstellung bewährt.
*   Das Setzen des Parameters `IShapeDoModel` aktiviert das Glättungsverfahren Modell XTREAM.
