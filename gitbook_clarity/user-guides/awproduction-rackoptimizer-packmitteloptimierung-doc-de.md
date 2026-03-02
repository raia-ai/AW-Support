---
description: "DE_AWProduction_RackOptimizer"
---


# A+W Rack Optimizer

A+W Production
A+W - Software for Glass, Windows and Doors

---
## Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version / Datum | Erläuterung |
| :--- | :--- |
| 1.00 / 03-2007 | Ersterstellung |
| 1.01 / 07-2013 | Layout an CI 2013 angepasst. |
| 1.02 / 01-2017 | Produkt- und Firmennamen angepasst. |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
*   Produktnamen
*   Anmerkungen zu diesem Dokument
*   Urheberrechte
*   Warenzeichen
*   Kontakte

#### Produktnamen

Im Rahmen der strategischen Neuausrichtung wurde das Produktportfolio der A+W Software GmbH neu ausgerichtet. Dabei wurden auch die Produktnamen angepasst. So wird ALCIM in Zukunft A+W Production heißen.

Da im Produktentwicklungszyklus sowohl die alten Produktversionen als auch die neuen Produktversionen angepasst und erweitert wurden, verwenden wir in diesem Dokument ausschließlich die alten Produktnamen - gemeint sind dabei jeweils die alten und die neuen Produktversionen.

#### Anmerkungen zu diesem Dokument

Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Production gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.

Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von A+W Production.

#### Urheberrechte

© 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

#### Warenzeichen

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

#### Kontakte

A+W Software GmbH

Am Pfahlgraben 4-10
D-35415 Pohlheim
+49 6404 2051-0
+49 6404 2051-877
Zentrale@a-w.com
http://www.a-w.com

## Inhalt

*   **Vorspann**
    *   Revisionsübersicht
    *   Editorial
*   **Funktionsprinzip**
    *   Grundgedanke
    *   Allgemeines
    *   Stammdaten
        *   Optimierungsregeln (*.RUL-Datei)
        *   Einstellwerte (*.VAL-Datei)
        *   Parameter
    *   Anzeigen
        *   Packmittelgruppen-Anzeige
        *   Restriktionen
    *   Optimierung ansehen
        *   Ansichten (3D-Ansicht, Draufsicht, Detail-Ansicht)
        *   Modi (Vollbild-Modus, Bearbeitungs-Modus, Experten-Modus)
        *   Zwischenablage
        *   Übersicht der Dialoge
*   **Bedienung**
    *   Übersicht
    *   Packmittelgruppen
    *   PackView
*   **Softwarereferenz**
    *   Menüs
    *   Regeln
    *   Werte
    *   Packmittelgruppen
    *   Packmittelgruppen-Anzeige
        *   Summenzeile
        *   Filterfunktion
        *   Schaltflächen zur Schnellanwahl
        *   Kontext-Menü bei markiertem Eintrag
    *   PackView
        *   Menü-Zeile
        *   Symbol-Schaltflächen
        *   Ansichten
        *   Gestellbezeichnung ändern
        *   Neue Gestell-Eigenschaften
        *   Eigenschaften der Kiste ändern
        *   Eigenschaften Referenz-Einheiten
        *   Info-Zeile am unteren Bildschirmrand
*   **Partindex**

## Funktionsprinzip

### Grundgedanke

Die Packmitteloptimierung erspart Ihnen sowohl aufwändiges Umsortieren als auch das Zwischenlager. Sie richtet den gesamten Produktionsprozess auf die Direktverpackung und die bestmögliche Auslastung der Packmittel (Gestelle und Versandkisten) aus.

In einer Produktion ohne Packmitteloptimierung (PMO) werden alle Einheiten, die aus der Produktion kommen, in einem Zwischenlager abgestellt. Danach müssen die Einheiten auf Transportgestelle verpackt werden, was mit aufwändigen Sortierungen verbunden ist. Meist stehen die Einheiten im Zwischenlager nicht in der Reihenfolge zur Verfügung, wie sie für das Transportgestell benötigt werden. Es kann auch der Fall sein, dass das Transportgestell nach Kundenwünschen beladen werden muss, oder es muss eine bestimmte Tour- bzw. Abladereihenfolge eingehalten werden.

Die Aufgabe der Packmitteloptimierung ist, die gewünschten Auftragspositionen unter Beachtung von Nebenbedingungen so auf Packmittel (Gestelle) zu verplanen, dass der Platzbedarf beim Transport minimal ist und Kundenwünsche beim Gestellaufbau erfüllt werden. Die Strategie bei der Verplanung wird durch Packmittelregeln formuliert. Diese enthalten neben den Angaben zu physikalischen Eigenschaften (wie Höhe, Breite und Gewicht) auch kundenspezifische Parameter für die zu verwendenden Packmittel (wie Anzahl der Stapel nebeneinander und übereinander).

In der Packmittelplanung werden Aufträge in gemeinsam zu verpackende Gruppen (Packmittelgruppen) eingeteilt, z. B. gleicher Liefertermin, gleiche Tour, gleiche Lieferanschrift.

### Allgemeines

Dieses Kapitel gibt Ihnen einen Überblick, wie die Packmitteloptimierung (PMO) aufgebaut ist und wie sie grundsätzlich arbeitet. Die Stammdaten der Packmitteloptimierung sind komplex und es sind umfangreiche Kenntnisse nötig, um die Packmitteloptimierung korrekt zu projektieren.

In der Packmitteloptimierung gibt es zwei getrennt zu behandelnde Bereiche von Vorgaben:

*   Die physikalischen Bedingungen (Gestellregeln), die beim Versand eingehalten werden müssen (Gewicht, Anordnung der Stapel, Abstände, etc.).
*   Die von Endkunden gewünschte Behandlung seiner Auftragspositionen (gruppieren, sortieren, auf spezielle Gestelle stellen, etc.).

Für den Endkunden ist in den meisten Fällen die Abnahmereihenfolge wichtig, in der die produzierten Einheiten von den Versandgestellen abgenommen werden können. Je strenger die Vorgaben für diese Reihenfolge sind, desto weniger Freiheit hat die Packmitteloptimierung bei der Verplanung der Gestelle. Das hat zur Folge, dass die Planungsdichte tendenziell schlechter sein wird.

Häufig wird gewünscht, dass Einheiten gemeinsam abnehmbar sind. So sollen zum Beispiel alle Einheiten eines Auftrags gemeinsam abnehmbar sein. Oder es sollen alle Einheiten einer Position hintereinander entladbar sein. Dabei ist noch nicht gesagt, dass solche gemeinsam abnehmbaren Einheiten auch nahe beieinander auf den Gestellen stehen. Es könnte durchaus sein, dass die Einheiten in verschiedenen Stapeln oder sogar auf verschiedenen Gestellen stehen. Die Optimierung stellt aber immer sicher, dass keine anderen Einheiten zunächst abgenommen werden müssen, um an alle gemeinsam abnehmbaren Gläser heran zu kommen. Je mehr Freiheit die Optimierung bei dieser Verplanung hat, desto besser sind die Planungsdichten auf den Gestellen, desto weniger Gestelle werden benötigt.

Eine Packmittelgruppe kann in Sets (etwa entsprechend der Aufträge) eingeteilt sein. Das bedeutet, dass die in einem Set enthaltenen Positionen entladen werden können, ohne andere Positionen anzufassen. Dabei kann das Set durchaus auf verschiedene Stapel oder Packmittel verteilt sein. Die Abladereihenfolge der Sets kann dabei von der Packmitteloptimierung selber bestimmt oder auch vorgegeben werden. Es gibt auch die Möglichkeit die Sets so zu planen, dass sie unabhängig voneinander in wahlfreier Reihenfolge entladen werden können.

Stapel auf dem Gestell müssen eine baumförmige Struktur haben. Zum Beispiel ein großer Stapel zu Beginn gefolgt von maximal 2 weiteren Stapeln, vor denen wieder maximal 2 Stapel stehen dürfen. Das sieht von oben gesehen so aus (die Gestellrückwand ist grau gezeichnet):

[Image: Top-down view of rack loading, showing a tree-like structure of stacks.]
**Abb. I-1: Gestellbeladung von oben gesehen**

Eine weitere Möglichkeit ist die Strukturierung einzelner Stapel durch Matrizen. Eine Matrix ist ein Aufbau, der es erlaubt, mehrere Einheiten nebeneinander und übereinander gleichzeitig zu platzieren. Dazu ist die Beachtung folgender Eigenschaften nötig:

*   Alle Einheiten einer Reihe, bis auf die oberste Reihe, müssen die gleiche Höhe haben.
*   Alle Einheiten einer Reihe müssen die gleiche Dicke haben.
*   Die Gesamtbreite jeder Reihe muss kleiner oder gleich der Gesamtbreite der unteren Reihe sein.
*   Die Dicke jeder Reihe muss kleiner oder gleich der Dicke der unteren Reihe sein.
*   Jede Reihe steht zentriert auf der unteren Reihe.

Daher können in einem Stapel Einheiten nebeneinander und übereinander stehen. Das können Einheiten aus einer oder auch aus verschiedenen Auftragspositionen sein. Von vorne kann dann ein einzelner Stapel so aussehen:

[Image: Front view of a matrix-loaded stack with items labeled (1/1), (2/1), (3/1) on the bottom row and (1/2), (2/2) on the top row.]
**Abb. I-2: Matrixbeladung: Stapel von vorne gesehen**

Die oberen Stapel stehen dabei immer zentriert auf den unteren.

Mit Matrizen kann man insbesondere erreichen, dass vor zwei Stapeln wieder ein größerer Stapel steht (nicht baumförmig).

[Image: Top-down view of matrix loading, showing a large stack in front of two smaller stacks.]
**Abb. I-3: Matrixbeladung von oben gesehen**

Einheiten aus einer Position werden zunächst grundsätzlich nach Möglichkeit zusammengehalten. Wenn eine Position wegen max. Gewicht oder Gestelltiefe nicht auf ein Gestell passt, wird sie geteilt.

### Stammdaten

Für den Anwender sind im Umgang mit der Packmitteloptimierung zwei Stammdaten-Typen sichtbar:

*   **Optimierungsregeln (*.RUL-Datei):** Die *.RUL-Dateien enthalten allgemeine Einstellungen, Angaben zu physikalischen Gestellen und zugehörige Belegungsregeln. Diese können z. B. je nach Kunde oder Auftrag vergeben werden.
*   **Einstellwerte (*.VAL-Datei):** Die *.VAL-Dateien ermöglichen kundenspezifische Einstellwerte zu den Optimierungsregeln.

Die *.RUL- und *.VAL-Dateien stehen dem Anwender zur Auswahl zur Verfügung. Geringfügige Modifikationen wie z. B. maximale Gestellbeladung können für eine bestimmte Packmittelgruppe vom Anwender durchgeführt werden.

> **Weitere Stammdaten**
> Darüber hinaus gibt es noch Gestellregeln, Verladeregeln und Regelzuweisungen. Diese Regeln werden durch die Firma A+W Software GmbH in Zusammenarbeit mit dem Anwender erarbeitet und gefüllt. Möchten Sie Veränderungen an der in Ihrem Hause implementierten Packmitteloptimierung vornehmen, halten Sie bitte unbedingt Rücksprache mit A+W Software GmbH, da es sonst zu unerwünschten Ergebnissen kommen kann!

#### Optimierungsregeln (*.RUL-Datei)

Die *.RUL-Dateien enthalten die Gestellregeln. In den Gestellregeln wird beschrieben, welche Packmittel mit welcher jeweiligen maximalen Anzahl und mit welchen Vorgaben zur Beladung geplant werden können. Das können Gestelle (A-Bock, L-Bock) oder auch Kisten (in Standard- oder Individualmaßen) sein.
⇨ Softwarereferenz, "Regeln" auf Seite I-71

#### Einstellwerte (*.VAL-Datei)

Die *.VAL-Dateien enthalten die Zuweisungen der kundenspezifischen Packmittelparamtern (*.VAL-Dateien) zu den Gestellregeln. Theoretisch kann für jede *.RUL-Datei eine eigene *.VAL-Datei angelegt werden, es sollte aber der dann notwendige Pflegeaufwand nicht außer Acht gelassen werden.
⇨ Softwarereferenz, "Werte" auf Seite I-73

#### Parameter

Zum Beladen der Gestelle arbeitet die Packmitteloptimierung mit unterschiedlichen Parametern. Im Anschluss finden Sie nähere Erläuterungen zu einzelnen, häufig verwendeten Parametern. Die in Ihrem Hause verwendeten Parameter können aufgrund Ihrer individuellen Anforderungen davon abweichen.

**Name des Parameters: Sets in Stapeln zusammenstellen.**
Erläuterung: Mit diesem Wert legen Sie fest, wie Sets in Stapeln (z. B. Aufträge) zusammen gestellt werden.
Mögliche Werte:
*   0-Nein, freie Optimierung,
*   1-Mono,
*   2-Multi,
*   3-Peripher.

**Mono:**
Im Mono-Modus kann jedes Set entladen werden, ohne Einheiten aus einem anderen Set anzufassen. Alle Sets können in jeder gewünschten Reihenfolge entladen werden. Daher steht in jedem Stapel nur ein Set.

[Image: Diagram of Mono mode, where each stack on a rack contains items from only one Set (e.g., Stack 1 has Set 1, Stack 2 has Set 2).]
**Abb. I-4 & I-5: Gestell 1 & Gestell 2**

**Multi:**
Der Multi-Modus gleicht dem Mono-Modus, jedoch kann jedes Set in maximal einem Stapel mit anderen Sets gemischt stehen. In einem gemischten Stapel steht jedes Set blockweise für sich (getrennt von den anderen Sets).

[Image: Diagram of Multi mode, where a stack can contain multiple Sets, but items of the same set are grouped together block-wise.]
**Abb. I-6 & I-7: Gestell 1 & Gestell 2**

**Peripher:**
Im Peripher-Modus kann jedes Set entladen werden, ohne Einheiten aus anderen Sets anzufassen. Die Reihenfolge der Entladung steht aber fest (entweder durch PMO oder den Anwender). Daher kann es mehr als ein Set pro Stapel geben.

[Image: Diagram of Peripher mode, similar to Mono but with a fixed unloading sequence, allowing more than one set per stack if accessibility is maintained.]
**Abb. I-8 & I-9: Gestell 1 & Gestell 2**

**Frei:**
Im Freien-Modus können Sets und Positionen nicht zusammen entladen werden. Die Aufträge stehen gemischt, um die höchste Packdichte zu erreichen.

[Image: Diagram of Frei (Free) mode, where items from different sets are mixed freely within stacks to achieve maximum packing density.]
**Abb. I-10 & I-11: Gestell 1 & Gestell 2**

**Name des Parameters: Sets bestehen aus.**
Erläuterung: Mit diesem Wert bestimmen Sie, wie Sets gebildet werden. Sie können Sets nach Aufträgen, nach Kommissionen oder aber nach Touren bilden.
Mögliche Werte:
*   1=Auftrag,
*   2=Kommission,
*   3=Tour.

**Name des Parameters: Sets auf Gestellen zusammenhalten?**
Erläuterung: Mit diesem Wert bestimmen Sie, ob und wenn ja, wie die Sets auf den Gestellen zusammen gehalten werden. 0 bedeutet, dass die Sets nicht auf Gestellen zusammen gehalten werden. Bei einer 1 werden die Sets auf einem Gestell zusammen gehalten und bei einer 2 auf maximal zwei Gestellen.
Mögliche Werte:
*   0=nein,
*   1=ein Gestell,
*   2=zwei Gestelle.

**Name des Parameters: Sets sortiert entladen?**
Erläuterung: Mit diesem Wert bestimmen Sie, ob und wenn ja, wie die Sets entladen werden sollen. Standardmäßig ist dieser Eintrag mit 0 vorbelegt. D. h. die Sets werden nicht sortiert.
Mögliche Werte:
*   0=nein,
*   1=Sets aufsteig. ++,
*   2=Set absteig. --.

**Name des Parameters: Maximales Gewicht für alle Gestelltypen**
Erläuterung: Der hier eingetragene Wert kennzeichnet das maximale Gewicht aller Gestelltypen dieser Packmittelgruppe. Der Wert ist in kg anzugeben.

**Name des Parameters: Maximale Anzahl der Stapel aufeinander (Standard=1)**
Der hier eingetragene Wert besagt, wie viele Stapel aufeinander gestellt werden dürfen. Standardmäßig ist der Wert 1 eingetragen. Das bedeutet, dass keine Stapel aufeinander stehen dürfen. Die größtmögliche Anzahl aufeinander stehender Stapel ist 5.

**Name des Parameters: Maximaler Überstand links/rechts (Standard: 100 mm)**
Erläuterung: Dieser Wert kennzeichnet den maximalen Gestellüberstand. Der hier eingetragene Wert wirkt sowohl links als auch rechts. Standardmäßig ist der Wert 100 eingetragen. Das bedeutet, dass der Überstand auf der rechten und auf der linken Gestellseite 100 mm ist. Die größt mögliche Wert ist 1000 (1000 mm).

**Name des Parameters: Maximales Seitenverhältnis für aufrechte Scheiben (Standard = 3.0)**
Erläuterung: Bei diesem Wert handelt es sich um den Minimalwert des Verhältnisses zwischen größeren/kleinerem Scheibenmaß, ab welchem die Scheiben liegend platziert werden. Beispiel: Bei einer Vorgabe von 2 wird die Scheibe 2500/1000 liegend platziert und die Scheibe 1500/1000 stehend. Standardmäßig ist der Wert 3 eingetragen. Der größt mögliche Wert ist 5. Eine 1 bewirkt, dass alle Scheiben auf die längere Seite gedreht werden.

**Name des Parameters: Max. Seitenverhältnis für aufrechte Scheiben beim Aufeinanderstapeln (Std=2.0)**
Erläuterung: Bei diesem Wert handelt es sich um das maximale Seitenverhältnis einer Einheit beim Aufeinanderstapeln, also wenn die Einheit auf einer anderen Einheit steht. Der Parameter wirkt nur dann, wenn er kleiner ist als der Parameter Maximales Seitenverhältnis für aufrechte Scheiben.

### Anzeigen

Die Packmitteloptimierung verfügt über eine eigene Anzeige, die Ihnen die Packmittelgruppen anzeigt, die Sie gebildet haben.

#### Packmittelgruppen-Anzeige

Die Packmittelgruppen-Anzeige öffnen Sie entweder über das Menü **Anzeigen > Packmittelgruppen-Anzeige** oder aber über die Symbol-Schaltfläche.

[Image: Screenshot of the 'Packmittel' icon.]
**Abb. I-12: Symbol-Schaltfläche Packmittelgruppen-Anzeige**

[Image: Screenshot of the 'Packmittelgruppen-Anzeige' window, showing a table with columns like OptiID, PMG_INDEX, Rack_ID, etc.]
**Abb. I-13: Packmittelgruppen-Anzeige**
*   **A**: Register
*   **B**: Tabellenspalte
*   **C**: Tabellenkopf
*   **D**: Schaltflächen zur Schnellanwahl
*   **E**: Summenzeile
*   **F**: Filterfunktion

Die Packmittelgruppen-Anzeige gibt Ihnen einen Überblick zu den bereits gebildeten Packmittelgruppen. Packmittelgruppen können Sie über das Kontext-Menü folgender Anzeigen bilden:
*   Auftrags-Anzeige
*   Bearbeitungs-Anzeige
*   Detail-Anzeige

Über die Register können Sie sich die Packmittelgruppen-Anzeige grob strukturieren. Innerhalb der Register stehen Ihnen zur weiteren Unterteilung Tabellenspalten zur Verfügung. Ferner können Sie sich Filter anlegen, um die Anzeige für bestimmte Situationen noch weiter einzuschränken. Bsp.: Innerhalb der Tabellenspalte Packmittel können Sie nach einzelnen Packmittelgruppen filtern. Über beliebig viele Filterfunktionen haben Sie so die Möglichkeit, die Anzeige Ihren speziellen Bedürfnissen anzupassen.
Informationen zu den Filtern und der Summenzeile finden Sie im Part Grobplanung.
⇨ Grobplanung, "Filter-Definition" auf Seite E-126

Die Schaltflächen zur Schnellanwahl können in den einzelnen Anzeigen unterschiedlich sein. Das hängt davon ab, welche Funktion in welcher Anzeige zur Verfügung steht. Die Schaltflächen aktivieren Sie, indem Sie einen Eintrag markieren. In der Packmittelgruppen-Anzeige haben Sie für einen oder mehrere markierte Einträge schnellen Zugriff auf:
*   **Laufbildung:** Es öffnet sich der Dialog **Lauf-Bildung**.
    ⇨ Grobplanung, "Lauf-Bildung" auf Seite E-86
*   **Glasarten:** Es öffnet sich der Dialog **Glasarten-Anzeige**.
    ⇨ Grobplanung, "Glasarten" auf Seite E-105
*   **Details:** Es öffnet sich der Dialog **Detail-Anzeige**.
    ⇨ Grobplanung, "Details" auf Seite E-108

#### Restriktionen

Über das Kontext-Menü der Packmittelgruppen-Anzeige haben Sie die Möglichkeit, Packmittelgruppen zu bearbeiten. D.h. Sie können Packmittelgruppen verschieben, löschen und ändern. Die einzelnen Funktionen sind jedoch abhängig vom Status der Packmittelgruppe. So ist es z. B. nicht möglich, eine bereits feingeplante Packmittelgruppe zu löschen, da die Feinplanung dann bereits mit den Ergebnissen der Packmittelgruppe gearbeitet hat.

Die folgende Tabelle zeigt Ihnen, welche Packmittelgruppe Sie in welchem Status bearbeiten können.

**Tab. I-1: Status der Packmittelgruppen**

| Status | Erläuterung | PMG ändern | PMG verschieben | PMG löschen | Optimieren | Optimierung ansehen | Optimierung zurücksetzen |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 50 | zur Optimierung freigegeben | Ja / Nein¹ | Ja / Nein¹ | Ja / Nein¹ | Ja | Nein | Ja |
| 75 | wird gerade hintergrundoptimiert | Nein | Nein | Nein | Nein | Nein | Nein |
| 80 | Optimierung fehlerhaft | Ja | Ja | Ja | Ja | Nein | Ja |
| 100 | ist packmitteloptimiert | Ja / Nein | Ja / Nein | Ja / Nein | Ja | Ja | Ja |
| >100 | ist feingeplant | Nein | Nein | Nein | Nein | Ja | Nein |

¹ Felder, die mit Ja / Nein belegt sind, sind entweder bereits zur Optimierung freigegeben oder wurden bereits packmitteloptimiert. Hier wird der Anwendern explizit gefragt, ob er Änderungen vornehmen möchte.

> **Weitere Informationen zur Packmittelgruppen-Anzeige**
> ⇨ Softwarereferenz, "Packmittelgruppen-Anzeige" auf Seite I-79
> ⇨ Konventionen, "Bedienoberfläche" auf Seite A-75
> ⇨ Konventionen, "Schaltflächen" auf Seite A-76

### Optimierung ansehen

Nach Durchführung der Packmitteloptimierung können Sie sich, in einer dreidimensionalen Ansicht, die Ergebnisse als Vorschau anzeigen lassen. Ergebnisse bedeutet: Wie werden die Einheiten auf dem Transportgestell stehen? Sie können in dieser Ansicht die optimierten Gestelle auch mit wenigen Mausklicks umpacken. Die Software zur Visualisierung der Packmittelergebnisse heißt PackView.

[Image: Screenshot of the PackView main interface, showing a 3D view, a top-down view, and a detailed list of items on the rack.]
**Abb. I-14: PackView**
*   **A**: Menü-Zeile
*   **B**: Symbol-Schaltflächen
*   **C**: 3D-Ansicht
*   **D**: Draufsicht
*   **E**: Detail-Ansicht der Einheit
*   **F**: Gewichtsverteilung auf linker und rechter Gestellseite
*   **G**: Gesamtgewicht in kg (Vorder- und Rückseite)
*   **I**: Ausdehnung der Gesamtbeladung auf der aktuellen Gestellseite: Breite, Höhe, Tiefe
*   **J**: Experten-Modus, Einstellräder für Nahsicht.

PackView startet nach einer erfolgreich durchgeführten Optimierung automatisch.

> **Weitere Informationen zur Visualisierung**
> ⇨ Softwarereferenz, "PackView" auf Seite I-85

#### Ansichten

PackView verfügt über folgende Ansichten:
*   3D-Ansicht
*   Draufsicht
*   Detail-Ansicht

In welcher der drei Ansichten Sie sich momentan befinden, sehen Sie an der gelben Umrandung der entsprechenden Ansicht. Mit der Maus können Sie einzelne Einheiten auswählen. Wenn Sie in der 3D-Ansicht eine Einheit auswählen, wird diese Einheit sowohl in der Draufsicht als auch in der Detail-Ansicht in Rot dargestellt. In welcher Ansicht Sie sich auch befinden, eine ausgewählte Einheit wird grundsätzlich auch in den anderen Ansichten in Rot hervorgehoben.

##### 3D-Ansicht

[Image: Screenshot of the PackView 3D view, showing a rack with loaded glass panes. One pane is highlighted.]
**Abb. I-15: 3D-Ansicht**
*   **A**: Aktuelle Gestellseite
*   **B**: Ausgewählte Einheit
*   **C**: Linke, untere Ecke (Bezugspunkt für die Rückseite)

Die 3D-Ansicht ermöglicht Ihnen die dreidimensionale Sicht beider Seiten eines Gestells. Welche Gestellseite angezeigt wird, sehen Sie an der roten Zahl in der linken, oberen Ecke der Ansicht.

Um die Gestellseite zu wechseln, stehen Ihnen folgende Möglichkeiten zur Verfügung:
*   Öffnen Sie im Menü **Ansicht** den Menüpunkt **Seitenansicht wechseln**.
*   Betätigen Sie auf Ihrer Tastatur die `<Leertaste>`.
*   Betätigen Sie die Symbol-Schaltfläche.
    [Image: Icon for switching rack side.]
    **Abb. I-16: Gestellseite wechseln**

Sie können sich ein Gestell aus mehreren Blickwinkeln anzeigen lassen. Diese Blickwinkel werden in PackView als **Kamera-Positionen** bezeichnet. Die oben gezeigte Abbildung (Abb. I-15) stellt die so genannte Ausgangs-Position der Kamera dar. Aus dieser Kamera-Position heraus wird die 3D-Ansicht standardmäßig geöffnet. Um zur nächsten Kamera-Position zu wechseln, stehen Ihnen folgende Möglichkeiten zur Verfügung:
*   Öffnen Sie im Menü **Ansicht** den Menüpunkt **Nächste Kamera-Position** oder **Vorhergehende Kamera-Position**.
*   Aktivieren Sie auf Ihrer Tastatur den Nummernblock über die Taste `<Num>`. Betätigen Sie im Bereich des Nummernblocks die Taste `<+>` oder `<->`.
*   Betätigen Sie die Symbol-Schaltflächen.
    [Image: Icons for next and previous camera position.]
    **Abb. I-17: Kamera-Positionen wechseln**

In der 3D-Ansicht können Sie Einheiten über die Funktion Kopieren verschieben. Das bedeutet, Sie markieren eine Einheit, kopieren sie, verschieben sie an die gewünschte Stelle und fügen sie dort ein. Sie haben auch die Möglichkeit, Einheiten nach dem Kopieren an ihrem Platz zu drehen.

##### Draufsicht

[Image: Screenshot of the PackView top-down view, showing the arrangement of stacks. One item is highlighted in red.]
**Abb. I-18: Draufsicht**
*   **A**: Linke, untere Ecke (Bezugspunkt)
*   **B**: Ausgewählte Einheit

Die Draufsicht zeigt Ihnen das Gestells von oben. Die rote Einheit ist die aktuell ausgewählte Einheit.
Sie können in der Draufsicht, wie auch in der 3D-Ansicht Einheiten über die Funktion **Kopieren** verschieben oder an ihrem Platz drehen.

##### Detail-Ansicht

Die Detail-Ansicht zeigt Ihnen tabellarisch, wie die Auftragspositionen auf den Gestellen stehen. Die in der Tabelle an oberster Position stehende Einheit ist die Einheit, die auf dem Gestell an der Gestellrückwand steht. Die in der Tabelle an letzter Position stehende Einheit ist die auf dem Gestell an vorderster Stelle stehende Einheit, d. h. die Tabelle ist in Beladereihenfolge sortiert.

[Image: Screenshot of the PackView detail view, showing a table with information about each item on the rack.]
**Abb. I-19: Detail-Ansicht**
*   **A**: Tabellenkopf
*   **B**: Tabellenspalte

**Erläuterung des Tabellenkopfes und der Tabellenspalten**

*   **Gestell#:** In diesem Feld wird das für die Packmitteloptimierung aktuelle Gestell mit den für diese Packmitteloptimierung gesamten Gestellen angezeigt. Bsp.: 1/3 bedeutet, dass die Packmittelgruppe insgesamt 3 Gestelle dieses Gestelltyps umfasst und das erste Gestell angezeigt wird. Die aktuelle Gestell#/Gesamtzahl finden Sie im Fenstertitel ganz oben.
*   **Seite:** In diesem Feld steht die Gestellseite, die aktuell angezeigt wird. Mögliche Werte:
    *   1: Folgende Einheiten stehen auf der 1. Gestellseite.
    *   2: Folgende Einheiten stehen auf der 2. Gestellseite.
*   **Stapel:** Dieses Feld steht in direktem Zusammenhang mit dem Feld **Seite** und zeigt Ihnen, in welchem Stapel sich die Einheit dieser Tabellenzeile befindet. Steht in dem Feld eine 1, befindet sich die Einheit im ersten Stapel auf dieser Seite des Gestells. Die Anzahl der Stapel ist abhängig von der Gestellgröße und der Einheitengröße.
    **Beispiel:** Auf der abgebildeten Gestellseite befinden sich insgesamt zwei Stapel.
    [Image: Screenshot showing an item in the first stack highlighted.]
    **Abb. I-20: 1. Stapel, 1. Reihe**
    [Image: Screenshot showing an item in the second stack highlighted.]
    **Abb. I-21: 2. Stapel, 1. Reihe**
    Vor dem zweiten Stapel stehen wiederum Reihen.
    [Image: Screenshot showing an item in the second row of the first stack highlighted.]
    **Abb. I-22: 1. Stapel, 2. Reihe**
    [Image: Screenshot showing an item in the second row of the second stack highlighted.]
    **Abb. I-23: 2. Stapel, 2. Reihe**
*   **Gestellbeschreibung:** Der Inhalt des Feldes kommt aus den PMO-Stammdaten und zeigt Ihnen den dort vergebenen Namen für das Gestell.
*   **Anzahl:** In diesem Feld sehen Sie, wie viele einzelne Einheiten sich insgesamt auf der aktuellen Seite des Gestells befinden.
*   **Reihe:** In diesem Feld sehen Sie, wie viele Stapel voreinander stehen.
*   **Gestell-ID:** In diesem Feld sehen Sie die aktuell angezeigte Gestell-ID.
*   **Fläche [m2]:** In diesem Feld sehen Sie, wie viele Quadratmeter Einheiten sich auf der betreffenden Seite des Gestells befinden.
*   **Vert. Stapel:** In diesem Feld sehen Sie, wie viele vertikale Stapel übereinander stehen.
*   **Typ:** In diesem Feld können Sie sehen, um welchen Abstellplatztyp es sich handelt. Mögliche Werte: A = A-Bock, L = L-Bock, Box = Kiste.
*   **Gewicht [kg]:** In diesem Feld sehen Sie, wie viele Kilogramm Glas sich auf der betreffenden Seite des Gestells befinden.
*   **Anzahl:** In diesem Feld sehen Sie, wie viele Einheiten eine Position hat und welche Einheit die aktuelle ist. Beispiel: 1/2 bedeutet, dass die Position 2 Einheiten hat und die betreffende Zeile eine davon auflistet.
*   **PM-Gruppe:** Dieses Feld zeigt Ihnen die Packmittelhauptgruppe und die Packmittelgruppe.
*   **Auftrags-Nr.:** Dieses Feld zeigt Ihnen die vom Auftragsbearbeitungssystem übergebene Auftrags-Nr. des Kunden.
*   **Positions-Nr.:** Dieses Feld bezieht sich auf das Feld Auftrags-Nr. und zeigt Ihnen die entsprechende Positions-Nr. zu der Auftrags-Nr.
*   **Größe [mm]:** Dieses Feld zeigt Ihnen die Abmessungen der aktuellen Einheitenposition in mm.
*   **Gewicht [kg]:** Dieses Feld zeigt Ihnen das Gewicht der aktuellen Einheitenposition in kg.
*   **Produktions-Linie:** Dieses Feld zeigt Ihnen, auf welcher Produktions-Linie die jeweilige Einheitenposition gefertigt wird.

Für spezielle Anforderungen ist die Anzahl und der Inhalt der gezeigten Spalten konfigurierbar. Nähere Information hierzu erhalten Sie von der A+W Software GmbH.

#### Modi

In PackView können Sie in drei unterschiedlichen Modi arbeiten. In Abhängigkeit von dem jeweiligen Modus stehen Ihnen unterschiedliche Werkzeuge zur Verfügung.
*   Vollbild-Modus
*   Bearbeitungs-Modus
*   Experten-Modus

##### Vollbild-Modus

PackView befindet sich nach dem Start im Vollbild-Modus. Sie können mit der Maus eine Scheibe markieren, indem Sie entweder in der 3D-Ansicht oder der Draufsicht eine Einheit anklicken oder aber eine Position aus der Detail-Ansicht wählen. Die ausgewählte Einheit wird sowohl in der 3D-Ansicht als auch der Draufsicht in roter Farbe dargestellt. In der Detailansicht befindet sich ein roter Rahmen um die ausgewählte Einheit.

[Image: Screenshot of PackView in Vollbild-Modus (Fullscreen Mode).]
**Abb. I-24: Vollbild-Modus**

Im Vollbild-Modus haben Sie Zugriff auf die unterschiedlichen Kamera-Positionen. Durch Betätigen der jeweiligen Schaltfläche schwenkt das Gestell in der 3D-Ansicht um 45° in die entsprechende Richtung. Sie haben so die Möglichkeit, sich das Gestell aus verschiedenen Blickwinkeln anzusehen, um z.B. freien Gestellplatz besser beurteilen zu können.

> **Modus**
> In welchem Modus Sie sich befinden (Vollbild/Bearbeiten), wird Ihnen im Programm am Ende der Titelleiste in eckigen Klammern angezeigt. Beispiel: `[Vollbild]`.

##### Bearbeitungs-Modus

PackView befindet sich nach dem Start im Vollbild-Modus. In den Bearbeitungs-Modus gelangen Sie entweder über das Menü **Bearbeiten > Bearbeiten**, über die Funktionstaste `<F3>` oder aber über die Symbol-Schaltfläche.

[Image: Icon for toggling edit mode.]
**Abb. I-25: Symbol-Schaltfläche Bearbeiten ein/aus**

Sie können mit der Maus eine Scheibe markieren. Die ausgewählte Einheit wird sowohl in der 3D-Ansicht als auch der Draufsicht in grüner Farbe dargestellt. In der Detailansicht befindet sich ein grüner Rahmen um die ausgewählte Einheit.

PackView wählt automatisch immer Teilstapel aus, die auch tatsächlich bewegt werden können. Wenn Sie eine Einheit in der Mitte eines Stapels auswählen, fügt PackView automatisch alle davor stehenden Einheiten in die Auswahl ein.

[Image: Screenshot of PackView in Bearbeitungs-Modus (Edit Mode) with items highlighted in green.]
**Abb. I-26: Bearbeitungs-Modus**

Im Bearbeitungs-Modus haben Sie Zugriff auf die unterschiedlichen Kamera-Positionen und können einzelne Einheiten oder auch ganze Stapel auf dem Gestell z.B. schrittweise verschieben oder links- bzw. rechtsbündig ausrichten.

> **Modus**
> In welchem Modus Sie sich befinden, wird Ihnen im Programm am Ende der Titelleiste in eckigen Klammern angezeigt. Beispiel: `[Bearbeiten]`.

##### Experten-Modus

PackView befindet sich nach dem Start im Normal-Modus. In den Experten-Modus gelangen Sie entweder über das Menü **Ansicht > Experten-Modus ein/aus**, oder über die Symbol-Schaltfläche.

[Image: Icon for toggling expert mode.]
**Abb. I-27: Symbol-Schaltfläche Experten-Modus ein/aus**

Den Experten-Modus können Sie sowohl im Vollbild- als auch im Bearbeitungs-Modus zuschalten.

[Image: Screenshot of PackView in Experten-Modus (Expert Mode) showing additional rotation and zoom controls.]
**Abb. I-28: Experten-Modus**

Neben den bereits genannten Funktionalitäten haben Sie im Experten-Modus noch die Möglichkeit, das Gestell zu zoomen und auf der X- bzw. Y-Achse zu rotieren.
*   **Zoom:** Platzieren Sie den Mauszeiger mittig auf dem Zoom-Rad, drücken die linke Maustaste und halten sie gedrückt. Drehen Sie das Rad nach oben, wird das Gestell verkleinert, drehen Sie das Rad nach unten, vergrößern Sie das Gestell.
*   **Rotieren (Y-Achse):** Platzieren Sie den Mauszeiger auf dem Y-Rotations-Rad. Drehen nach rechts bewegt das Gestell nach rechts, drehen nach links bewegt es nach links.
*   **Rotieren (X-Achse):** Platzieren Sie den Mauszeiger auf dem X-Rotations-Rad. Drehen nach oben kippt das Gestell nach oben, drehen nach unten kippt es nach unten.

Wenn Sie sich im Experten-Modus befinden, haben Sie auch die Möglichkeit, das Gestell frei zu rotieren. Das freie Rotieren aktivieren Sie entweder über das Menü **Ansicht > Freies Rotieren** oder über die Symbol-Schaltfläche.

[Image: Icon for free rotation.]
**Abb. I-29: Symbol-Schaltfläche Freies Rotieren**

Ihr Mauszeiger ändert sich dann. Platzieren Sie den Mauszeiger auf dem Gestell, drücken Sie die linke Maustaste und halten Sie diese gedrückt. Anschließend können Sie das Gestell nach links oder rechts beliebig drehen oder nach oben bzw. unten kippen. Mit Druck auf das Mausrad können Sie das Gestell nach links und rechts verschieben.

#### Zwischenablage

Wenn Sie eine oder auch mehrere Einheiten ausgeschnitten haben, werden diese nach dem Ausschneiden automatisch in die Zwischenablage gestellt.

Beispiel: Sie markieren im Bearbeitungs-Modus eine Einheit.
[Image: Screenshot showing an item selected for cutting.]
**Abb. I-31: Zwischenablage**

Anschließend betätigen Sie die Schaltfläche zum Ausschneiden der Einheit.
[Image: Icon for cutting an item.]
**Abb. I-32: Schaltfläche zum Ausschneiden der Einheit**

PackView zeigt Ihnen dann das Gestell ohne die Einheit. Die Detail-Ansicht zeigt Ihnen die Inhalte der Zwischenablage, in diesem Fall die soeben ausgeschnittene Einheit.

[Image: Screenshot showing the rack after cutting the item, and the clipboard view with the cut item.]
**Abb. I-33: Zwischenablage**

Durch Betätigen der Schaltfläche **Zwischenablage** können Sie die Detail-Ansicht zwischen der Anzeige der Zwischenablage und der Gestellbelegung umschalten.

Bei Feldern, die in der Detail-Ansicht mit einem `-` versehen sind, können Sie die Sortierung ändern. Wenn Sie den Mauszeiger auf einem solchen Feld platzieren und die linke Maustaste betätigen, ändert sich das Symbol von `-` nach `▲` (aufsteigend). Betätigen Sie die linke Maustaste erneut, wechselt das Symbol von `▲` auf `▼` (absteigend). Zum Ausschalten der Sortierung, betätigen Sie die rechte Maustaste. Sie können mehrere Spalten in dieser Weise anklicken. Die Sortierung erfolgt dann zunächst nach der zuerst angeklickten Spalte, dann nach der nächsten, etc. Die Ziffer zeigt diese Rangfolge an.

#### Übersicht der Dialoge

Die Übersicht zeigt Ihnen alle Dialoge, die Sie zur vollständigen Nutzung der Packmitteloptimierung benötigen. Die Verweise führen Sie in das Kapitel Softwarereferenz des Stammdatenbereichs. Dort finden Sie detaillierte Informationen zu den Dialogen mit ihren Feldern und Schaltflächen.

**Menü Stammdaten**

| Menü-Eintrag | Untermenü | Dialog/Funktion |
| :--- | :--- | :--- |
| PMO | Regeln | ⇨ Softwarereferenz, "Packmittelgruppen" auf Seite I-76 |
| | Werte | ⇨ Softwarereferenz, "Werte" auf Seite I-73 |
| Anzeigen | Packmittelgruppen-Anzeige | ⇨ Softwarereferenz, "Packmittelgruppen-Anzeige" auf Seite I-79 |

## Bedienung

### Übersicht

In dem Kapitel Bedienung wird Ihnen gezeigt, wie Sie mit der Packmitteloptimierung arbeiten.
Es gibt Handlungsanweisungen zu folgenden Themen:
*   Packmittelgruppen
*   PackView

### Packmittelgruppen

In diesem Kapitel wird erläutert, wie Sie mit Packmittelgruppen umgehen.

| Thema | Handlungsanweisung |
| :--- | :--- |
| Packmittelgruppen | ⇨ "So bilden Sie Packmittelgruppen" auf Seite I-41 |
| | ⇨ "So starten Sie die Optimierung für eine Packmittelgruppe" auf Seite I-42 |
| | ⇨ "So nehmen Sie Änderungen an den Parametern einer bestehenden Packmittelgruppe vor" auf Seite I-42 |

**So bilden Sie Packmittelgruppen**

Die Vorgehensweise zum Bilden von Packmittelgruppen ist für alle Anzeigen (Aufträge, Bearbeitungen, etc.) gleich. Wir erläutern die Vorgehensweise deshalb nur einmal am Beispiel der Anzeige Aufträge.
1.  Öffnen Sie die Anzeige **Aufträge** entweder über das Menü **Anzeigen > Aufträge** oder über die entsprechende Schaltfläche.
    ⇨ Konventionen, “Pool-Anzeige" auf Seite A-78
2.  Selektieren Sie den bzw. die Aufträge, mit denen Sie eine Packmittelgruppe bilden möchten.
3.  Öffnen Sie das Kontext-Menü und wählen Sie **Packmittelgruppe bilden**.
4.  Es öffnet sich der Dialog **Packmittelgruppen**.
5.  Geben Sie im Feld **Packmittelhauptgruppe** den Namen für die Packmittelhauptgruppe an.
    ⇨ Softwarereferenz, “Packmittelhauptgruppe" auf Seite I-76
6.  Geben Sie im Feld **Packmittelgruppe** den Namen für die Packmittelgruppe an.
    ⇨ Softwarereferenz, "Packmittelgruppe" auf Seite I-77
7.  Wählen Sie aus der Kombobox **Packmittelregel** die entsprechende Regel aus.
    ⇨ Softwarereferenz, "Packmittelregel" auf Seite I-77
8.  Geben Sie im Feld **Beschreibung** eine weitere Bezeichnung für die Packmittelgruppe an.
    ⇨ Softwarereferenz, "Beschreibung" auf Seite I-77
9.  Aktivieren oder deaktivieren Sie die Checkbox **Positionen von Optimierung ausschließen**.
    ⇨ Softwarereferenz, "Positionen von Optimierung ausschließen" auf Seite I-77
10. Aktivieren oder deaktivieren Sie die Checkbox **Mehrere Produktionslinien zusammenfassen**.
    ⇨ Softwarereferenz, "Mehrere Produktionslinien zusammenpacken" auf Seite I-77
11. Ändern Sie bei Bedarf die VAL-Einstellungen.
12. Betätigen Sie die Schaltfläche [OK].
13. Der bzw. die selektierten Aufträge werden aus der Anzeige **Aufträge** entfernt. Sie finden den bzw. die Aufträge unter der soeben vergebenen Packmittelhauptgruppe in der Anzeige **Packmittel**.

**So starten Sie die Optimierung für eine Packmittelgruppe**

1.  Öffnen Sie die Anzeige **Packmittel** entweder über das Menü **Anzeigen > Packmittel** oder über die entsprechende Schaltfläche.
    ⇨ Konventionen, "Packmittelgruppen-Anzeige" auf Seite A-78
2.  Selektieren Sie den bzw. die Packmittelgruppe, die Sie optimieren möchten.
3.  Öffnen Sie das Kontext-Menü und wählen Sie **PMG optimieren**.
4.  Die Optimierung wird gestartet.

**So nehmen Sie Änderungen an den Parametern einer bestehenden Packmittelgruppe vor**

1.  Öffnen Sie die Anzeige **Packmittel** entweder über das Menü **Anzeigen > Packmittel** oder über die entsprechende Schaltfläche.
    ⇨ Konventionen, “Packmittelgruppen-Anzeige" auf Seite A-78
2.  Selektieren Sie den bzw. die Packmittelgruppe, an der Sie Änderungen vornehmen möchten.
3.  Öffnen Sie das Kontext-Menü und wählen Sie **PMG verwalten > Parameter ändern**.
4.  Es öffnet sich der Dialog **Packmittelgruppen**. Änderungen, die Sie zu diesem Zeitpunkt vornehmen können, beziehen sich auf die Felder:
    *   Packmittelregel
    *   Beschreibung
    *   Positionen von Optimierung ausschließen
    *   Mehrere Produktionslinien zusammenpacken
    *   VAL.
5.  Wählen Sie aus der Kombobox **Packmittelregel** die entsprechende Regel aus.
    ⇨ Softwarereferenz, "Packmittelregel" auf Seite I-77

> **Weitere Informationen zu Packmittelgruppen**
> ⇨ Funktionsprinzip, "Packmittelgruppen-Anzeige" auf Seite I-19
> ⇨ Softwarereferenz, "Packmittelgruppen" auf Seite I-76

### PackView

In diesem Kapitel wird erläutert, wie Sie mit PackView umgehen.

| Thema | Handlungsanweisung |
| :--- | :--- |
| PackView | ⇨ "So wählen Sie das nächste/vorherige Gestell zur Anzeige aus" auf Seite I-43 |
| | ⇨ "So wählen Sie ein beliebiges Gestell zur Anzeige aus" auf Seite I-43 |
| | ⇨ "So verschieben Sie eine oder wenige Einheiten" auf Seite I-44 |
| | ⇨ "So verschieben Sie einen ganzen Stapel" auf Seite I-46 |
| | ⇨ "So arbeiten Sie mit der Zwischenablage" auf Seite I-49 |
| | ⇨ "So arbeiten Sie mit mehreren Stapeln in der Zwischenablage" auf Seite I-54 |

**So wählen Sie das nächste/vorherige Gestell zur Anzeige aus**

In der Regel werden durch die Packmitteloptimierung mehrere Gestelle beladen. PackView startet nach erfolgreich durchgeführter Optimierung automatisch mit dem ersten Gestell. Zum Anzeigen der weiteren Gestelle gehen Sie wie folgt vor:
1.  Wählen Sie im Menü **Ansicht > Zeige nächstes Gestell**, verwenden Sie die entsprechende Symbol-Schaltfläche oder die Tasten `<BildAuf>` bzw. `<Bild-Ab>`.
    ⇨ Softwarereferenz, "Zeige nächstes Gestell" auf Seite I-89
    ⇨ Softwarereferenz, "Zeige vorheriges Gestell" auf Seite I-89
    Auf diese Art und Weise können Sie sich Gestell für Gestell anzeigen lassen.

**So wählen Sie ein beliebiges Gestell zur Anzeige aus**

1.  Wählen Sie entweder im Menü **Ansicht > Gestell zur Anzeige auswählen**, verwenden Sie die entsprechende Symbol-Schaltfläche oder die Tasten `<BildAuf>` bzw. `<BildAb>`.
    ⇨ Softwarereferenz, "Gestell zur Anzeige auswählen ." auf Seite 1-89
2.  Es öffnet sich der Dialog **Eingabe**. Im Feld **Gestell ID eingeben** können Sie die gewünschte Gestellnummer eingeben.
3.  Nach Betätigen der Schaltfläche [OK] wird das entsprechende Gestell angezeigt.

**So verschieben Sie eine oder wenige Einheiten**

1.  Aktivieren Sie den Bearbeitungs-Modus über das Menü **Bearbeiten > Bearbeiten**, über die Funktionstaste `<F3>` oder aber über die Symbol-Schaltfläche.
    ⇨ Softwarereferenz, "Bearbeiten ein/aus" auf Seite I-91
2.  Markieren Sie die Einheit(en), die Sie verschieben möchten. Die Einheit(en) bekommt einen grünen Rahmen. Es bekommen automatisch weitere Einheiten einen grünen Rahmen, die mit bewegt werden müssen. Durch weitere Klicks können weitere Einheiten hinzugenommen oder bereits gewählte Einheiten abgewählt werden.
    [Image: Screenshot showing an item selected in edit mode, highlighted in green.]
    **Abb. I-34: Einheit markieren**
3.  Kopieren Sie die Einheit(en) entweder über das Menü **Bearbeiten > Kopieren**, über die Symbol-Schaltfläche oder über die Tastatur (`<Strg>+<C>`).
    ⇨ Softwarereferenz, "Einheit Kopieren" auf Seite I-92
    Die Einheit wird komplett in grüner Farbe dargestellt.
    [Image: Screenshot showing the entire selected stack highlighted in green.]
    **Abb. I-35: Einheit kopieren, markieren**
4.  Verschieben Sie die Einheit an die gewünschte Stelle mithilfe der Richtungstasten oder über die Symbol-Schaltfläche.
    ⇨ Softwarereferenz, "Einheit nach links bewegen" auf Seite I-92
    ⇨ Softwarereferenz, "Einheit nach rechts bewegen" auf Seite I-92
    [Image: Screenshot showing the copied item being moved to a new position.]
    **Abb. I-36: Einheit verschieben**
5.  Ist die Einheit an der Stelle angekommen, wo sie neu platziert werden soll, fügen Sie sie dort entweder über das Menü **Bearbeiten > Einfügen** oder aber über die Symbol-Schaltfläche ein.
    ⇨ Softwarereferenz, "Einheit Einfügen" auf Seite I-92
    [Image: Screenshot showing the item placed in its new position.]
    **Abb. I-37: Einheit einfügen**

**So verschieben Sie einen ganzen Stapel**

1.  Aktivieren Sie den Bearbeitungs-Modus.
    ⇨ Softwarereferenz, "Bearbeiten ein/aus" auf Seite I-91
2.  Markieren Sie die Einheit des Stapels, die der Gestellrückwand am nähesten steht und die Sie verschieben möchten. Die Einheit und alle davor stehenden Einheiten bekommen einen grünen Rahmen.
    [Image: Screenshot showing a full stack selected for moving.]
    **Abb. I-38: Stapel markieren**
3.  Kopieren Sie den Stapel entweder über das Menü **Bearbeiten > Kopieren**, oder aber über die Symbol-Schaltfläche.
    ⇨ Softwarereferenz, "Einheit Kopieren" auf Seite I-92
    Der Stapel wird komplett in grüner Farbe dargestellt. Alle markierten Einheiten verschwinden aus der Detail-Ansicht.
    [Image: Screenshot showing the stack removed from the detail view and highlighted green in the 3D view.]
    **Abb. I-39: Stapel kopieren**
4.  Verschieben Sie den Stapel an die gewünschte Stelle mithilfe der Richtungstasten oder über die Symbol-Schaltfläche.
    [Image: Screenshot showing the copied stack being moved.]
    **Abb. I-40: Stapel verschieben**
5.  Ist der Stapel an der Stelle angekommen, wo er neu platziert werden soll, fügen Sie ihn dort wieder ein.
    ⇨ Softwarereferenz, "Einheit Einfügen" auf Seite I-92
    [Image: Screenshot showing the stack pasted into its new position.]
    **Abb. I-41: Stapel einfügen**

**So arbeiten Sie mit der Zwischenablage**

Wenn Sie viele Einheiten, etwa aus verschiedenen Stapeln, auf einer anderen Gestellseite platzieren möchten oder gar auf einem anderen Gestell, geht dies gut über die Zwischenablage. Dabei können Sie auch bequem die Reihenfolge der Einheiten nach Größe, Auftragsnummer etc. sortieren, um den neuen Stapel Ihren Wünschen entsprechend aufzubauen.
1.  Aktivieren Sie den Bearbeitungs-Modus.
2.  Markieren Sie die Einheit(en), die Sie verschieben möchten.
3.  Schneiden Sie die Einheit(en)/Stapel aus.
    ⇨ Softwarereferenz, "Einheit Ausschneiden" auf Seite I-92
    Die Einheit(en)/Stapel verschwindet sowohl aus der 3D-Ansicht als auch aus der Draufsicht. Im Bereich der Detail-Ansicht bekommen Sie automatisch den Inhalt der Zwischenablage angezeigt.
    [Image: Screenshot showing the clipboard view after cutting items.]
    **Abb. I-44: Zwischenablage ein- und ausblenden**
4.  Wechseln Sie zu der gewünschten Gestellseite bzw. dem gewünschten Gestell.
5.  Lassen Sie sich den Inhalt der Zwischenablage anzeigen und sortieren Sie ihn bei Bedarf.
    ⇨ Funktionsprinzip, "Zwischenablage" auf Seite I-35
6.  Klicken Sie anschließend auf die Symbol-Schaltfläche [Einfügen]. Der Mauszeiger ändert sich zu einem Fadenkreuz.
    [Image: Screenshot showing the crosshair cursor for pasting.]
    **Abb. I-47: Einheit einfügen**
7.  Bewegen Sie das Fadenkreuz an die Stelle, wo die Einheit(en)/Stapel eingefügt werden soll(en).
8.  Betätigen Sie anschließend die linke Maustaste. Die Einheit(en)/Stapel wird - sofern physikalisch möglich - an dieser Stelle eingefügt. Sollte es nicht möglich sein, wird die Einheit kurzzeitig in oranger Farbe angezeigt, aber nicht platziert.
9.  Nach dem Einfügen wird die Zwischenablage geleert.

**So arbeiten Sie mit mehreren Stapeln in der Zwischenablage**

1.  Aktivieren Sie den Bearbeitungs-Modus.
2.  Markieren Sie die letzte Einheit des ersten Stapels, den Sie verschieben möchten.
3.  Schneiden Sie den Stapel aus. Er wird in die Zwischenablage verschoben.
4.  Wechseln Sie zum nächsten Gestell und markieren Sie den nächsten Stapel.
5.  Schneiden Sie diesen Stapel ebenfalls aus. Er wird der Zwischenablage hinzugefügt.
6.  Wiederholen Sie dies für alle gewünschten Stapel.
7.  Wechseln Sie zu dem gewünschten Zielgestell.
8.  Sortieren Sie die Einheiten in der Zwischenablage nach Ihren Wünschen (z.B. nach Breite).
9.  Fügen Sie die Einheiten nacheinander aus der Zwischenablage auf dem neuen Gestell ein. Sie können die Einheiten präzise ausrichten (z.B. linksbündig).
    > **Tastatur**
    > `<Strg>+<V>` fügt die nächste Einheit aus der Zwischenablage vor die zuletzt eingefügte ein.
10. Arbeiten Sie so weiter, bis alle Einheiten aus der Zwischenablage auf dem Gestell platziert sind.

> **Weitere Informationen zu PackView**
> ⇨ Funktionsprinzip, "Optimierung ansehen" auf Seite I-22
> ⇨ Softwarereferenz, "PackView" auf Seite I-85

## Softwarereferenz

### Menüs

Die nachfolgenden Tabellen geben eine Übersicht der Dialoge und Funktionen in den Menüs.

**Übersicht der Dialoge im Menü Stammdaten**

| Menü-Eintrag | Dialog/Funktion |
| :--- | :--- |
| PMO > Regeln | ⇨ Kapitel "Regeln" auf Seite I-71 |
| PMO > Werte | ⇨ Kapitel "Werte" auf Seite I-73 |

**Übersicht der Dialoge im Kontext-Menü (Anzeigen: Aufträge, Bearbeitungen, Details)**

| Menü-Eintrag | Dialog/Funktion |
| :--- | :--- |
| Kontext-Menü > Packmittelgruppe bilden | ⇨ Kapitel "Packmittelgruppen" auf Seite I-76 |

**Übersicht der Dialoge im Kontext-Menü (Anzeige: Packmittelgruppe)**

| Menü-Eintrag | Dialog/Funktion |
| :--- | :--- |
| Kontext-Menü > Packmittelgruppe verschieben | ⇨ Kapitel "PMG verschieben" auf Seite I-82 |
| Kontext-Menü > Packmittelgruppe optimieren | ⇨ Kapitel "PMG optimieren" auf Seite I-82 |
| Kontext-Menü > Packmittelgruppe optimieren im Hintergrund | ⇨ Kapitel "PMG optimieren im Hintergrund" auf Seite I-83 |
| Kontext-Menü > Packmittelgruppe verwalten | ⇨ Kapitel "PMG verwalten" auf Seite I-83 |
| Kontext-Menü > Optimierung ansehen | ⇨ Softwarereferenz, "PackView" auf Seite I-85 |

**Übersicht der Dialoge im Menü Anzeigen**

| Menü-Eintrag | Dialog/Funktion |
| :--- | :--- |
| Packmittelgruppen-Anzeige | ⇨ Kapitel "Packmittelgruppen-Anzeige" auf Seite I-79 |

### Regeln

**Stammdaten > PMO > Regeln**

[Image: Screenshot of the PMO-Regeln dialog.]
**Abb. I-69: Packmittelgruppen, Regeln**

In diesem Dialog erfassen Sie neue Optimierungsregeln oder ändern bestehende Regeln ab.
**Technische Info:** Datenbanktabelle: `PMO_MASTER_RULES`

**Erläuterung der Schaltfläche**
*   **.RUL-Dateien laden:** Wenn Sie diese Schaltfläche betätigen, werden die `*.RUL`-Dateien aus dem entsprechenden Verzeichnis geladen. Sind bereits `*.RUL`-Dateien in der Anzeige zu sehen, werden Sie darauf aufmerksam gemacht, dass alle aktuellen Datensätze verloren gehen.

**Erläuterung der Tabellenspalten**
*   **RUL-Datei:** Name der zur Zeit geladenen `*.RUL`-Dateien.
*   **Bezeichnung:** Bezeichnung der `*.RUL`-Datei.
*   **VAL_FILE:** Zeigt, welche `*.VAL`-Datei der `*.RUL`-Datei zugeordnet ist.

**Erläuterung der Felder**
*   **.RUL-Datei:** Dateiname der RUL-Datei. Über [...] öffnet sich der Dialog **Öffnen**. (Datenbankfeld: FILE)
*   **Bezeichnung:** Bezeichnung der `*.RUL`-Datei. (Datenbankfeld: NAME)
*   **Beschreibung:** Beschreibender Text zur `*.RUL`-Datei. (Datenbankfeld: DESCRIPTION)
*   **.VAL-Datei:** Zugehörige `*.VAL`-Datei. Über [...] kann eine andere `*.VAL`-Datei zugeordnet werden. (Datenbankfeld: VAL_FILE)

> **Weitere Informationen zu Regeln**
> ⇨ Funktionsprinzip, "Optimierungsregeln (*.RUL-Datei)" auf Seite I-13
> ⇨ Konventionen, "Schaltflächen" auf Seite A-76

### Werte

**Stammdaten > PMO > Werte**

[Image: Screenshot of the PMO-Werte dialog.]
**Abb. I-70: Packmittelgruppen, Werte**

In diesem Dialog erfassen Sie die kundenspezifischen Werte oder nehmen Änderungen an bestehenden Werten vor.
**Technische Info:** Datenbanktabelle: `PMO_MASTER_VALUES`

**Erläuterung der Schaltflächen**
*   **.VAL-Dateien laden:** Wenn Sie diese Schaltfläche betätigen, werden die `*.VAL`-Dateien (Regel) aus dem entsprechenden Verzeichnis geladen.

**Erläuterung der Tabellenspalten**
*   **.VAL-Datei:** Name der zur Zeit geladenen `*.VAL`-Dateien.
*   **Parameter:** Der Packmittelparameter der `*.VAL`-Datei.
*   **Bezeichnung:** Die Bezeichnung der `*.VAL`-Datei.
*   **Mindestwert:** Der Mindestwert des Parameters.
*   **Maximalwert:** Der Maximalwert des Parameters.
*   **Wertetyp:** Der Wertetyp des Parameters.

**Erläuterung der Felder**
*   **.VAL-Datei:** Zeigt die `*.VAL`-Datei an. Über [...] können Sie eine `*.VAL`-Datei auswählen. (Datenbankfeld: FILE)
*   **Nummer des Packmittelparameters:** Hier geben Sie die Nummer des Parameters ein. Es gibt die folgenden 9 Packmittelparameter:
    1.  Sets in Stapeln zusammenhalten (0-nein, 1-mono, 2-multi, 3-peripher).
    2.  Sets bestehen aus (1-Auftrag, 2-Kommission, 3-Tour).
    3.  Sets auf Gestellen zusammen halten? (0-nein, 1-ein Gestell, 2-zwei Gestelle).
    4.  Sets sortiert entladen? (0-nein, 1-Sets aufsteigend ++, 2-Sets absteigend --).
    5.  Maximales Gewicht für alle Gestelltypen.
    6.  Maximale Anzahl der Stapel aufeinander (Standard=1).
    7.  Maximaler Überstand links/rechts (Standard: 100mm).
    8.  Maximales Stimmenverhältnis für aufrechte Scheiben (Standard=3.0).
    9.  Max. Seitenverhältnis für aufrechte Scheiben beim Aufeinanderstapeln (Std.=2.0).
    Nähere Erläuterungen finden Sie im Funktionsprinzip.
*   **Bezeichnung:** Geben Sie die Bezeichnung der `*.VAL`-Datei ein. (Datenbankfeld: NAME)
*   **Beschreibung:** Geben Sie einen beschreibenden Text zur `*.VAL`-Datei ein. (Datenbankfeld: DESCRIPTION)
*   **Mindestwert:** Mindestwert des aktuellen Parameters. (Datenbankfeld: VALUE_MIN)
*   **Maximalwert:** Maximalwert des aktuellen Parameters. (Datenbankfeld: VALUE_MAX)

> **Weitere Informationen zu Einstellwerten**
> ⇨ Funktionsprinzip, "Einstellwerte (*.VAL-Datei)" auf Seite I-13
> ⇨ Konventionen, "Schaltflächen" auf Seite A-76

### Packmittelgruppen

**Aufträge > Kontext-Menü > Packmittelgruppen bilden**
(auch erreichbar über Bearbeitungs-Anzeige und Detail-Anzeige)

[Image: Screenshot of the Packmittelgruppen dialog.]
**Abb. I-71: Packmittelgruppen bilden**

In diesem Dialog nehmen Sie die Einstellungen vor, mit denen die Packmittelgruppe gebildet werden soll.
**Technische Info:** Datenbanktabelle: `PMO_GROUPS`

**Erläuterung der Felder und Schaltflächen**
*   **Packmittelhauptgruppe:** Wählen Sie eine bestehende Hauptgruppe aus oder erfassen Sie eine neue. (Datenbankfeld: PMO_MASTERGROUP)
*   **Packmittelgruppe:** Wählen Sie eine bestehende Gruppe aus oder erfassen Sie eine neue. (Datenbankfeld: PMO_GROUP)
*   **Packmittelregel:** Ordnen Sie die gewünschte Packmittelregel zu. Die Regeln werden im Dialog **Regeln** hinterlegt. (Datenbankfeld: RUL_FILE)
*   **Beschreibung:** Optionale Erläuterung zur Packmittelgruppe. (Datenbankfeld: GROUP_INFO)
*   **Positionen von Optimierung ausschließen (Checkbox):** Aktivieren, um selektierte Positionen nicht für Gestelle zu optimieren (sie gehen in die "grüne Kiste"). Sinnvoll für sehr große Scheiben. (Datenbankfeld: KEEP_SET_TOGETHER)
*   **Mehrere Produktionslinien zusammenpacken (Checkbox):** Erlaubt, Einheiten von verschiedenen Produktionslinien auf demselben Gestell zu planen. (Datenbankfeld: LINE_PACK_TOGETHER)

**Erläuterung der Tabellenspalten**
*   **Wert:** Hier können Sie die Werte aus der VAL-Datei einmalig für diese Optimierung ändern.
*   **Beschreibung:** Zeigt die Beschreibung des Parameters an.
*   **Wertetyp:** Zeigt den Wertetyp des Parameters an.

> **Weitere Informationen zu Packmittelgruppen**
> ⇨ Konventionen, "Schaltflächen" auf Seite A-76
> ⇨ Funktionsprinzip, "Optimierungsregeln (*.RUL-Datei)" auf Seite I-13
> ⇨ Funktionsprinzip, "Einstellwerte (*.VAL-Datei)" auf Seite I-13

### Packmittelgruppen-Anzeige

**Anzeigen > Packmittelgruppen-Anzeige**

[Image: Screenshot of the Packmittelgruppen-Anzeige window.]
**Abb. I-73: Packmittelgruppen-Anzeige**

Die Anzeige gibt einen Überblick zu den gebildeten Packmittelgruppen. Die Inhalte und Sortierungen bestimmen Sie über die Kontext-Menüs, die sich je nach Position des Mauszeigers (auf Registern, Tabellenkopf, Datensatz) unterscheiden.

#### Summenzeile

Mithilfe der Summenzeile können Sie sich einen zahlenmäßigen Überblick über markierte Einträge verschaffen.

#### Filterfunktion

Über die Filterfunktion haben Sie die Möglichkeit, die aktuelle Anzeige nach beliebigen Kriterien zu filtern.

#### Schaltflächen zur Schnellanwahl

Im rechten, unteren Bereich der Anzeige befinden sich Schaltflächen für schnellen Zugriff auf Funktionen. Ein oder mehrere Datensätze müssen markiert sein.
*   **Laufbildung (F6):** Öffnet den Dialog zur Lauf-Bildung. (⇨ Grobplanung, "Lauf-Bildung" auf Seite E-86)
*   **Glasarten (F7):** Öffnet die Glasarten-Anzeige für den Datensatz. (⇨ Grobplanung, "Glasarten" auf Seite E-105)
*   **Details (F8):** Öffnet die Detail-Anzeige für den Datensatz. (⇨ Grobplanung, "Details" auf Seite E-108)

> **Weitere Informationen zur Packmittelgruppen-Anzeige**
> ⇨ Bedienung, "Packmittelgruppen" auf Seite I-41
> ⇨ Konventionen, "Bedienoberfläche" auf Seite A-75
> ⇨ Konventionen, "Schaltflächen" auf Seite A-76

### Kontext-Menü bei markiertem Eintrag

**Anzeigen > Packmittelgruppen > Datensatz markieren > rechte Maustaste**

[Image: Screenshot of the context menu for a selected entry in the Packmittelgruppen-Anzeige.]
**Abb. I-77: Kontext-Menü bei markiertem Datensatz**

Das Kontext-Menü bei einem markierten Datensatz verfügt über folgende Menüpunkte:
*   **PMG verschieben:** Öffnet die Anzeige **Packmittelgruppen**, um eine oder mehrere Packmittelgruppen zu verschieben.
*   **PMG optimieren:** Startet die Optimierung für die selektierte(n) Packmittelgruppe(n).
*   **PMG optimieren im Hintergrund:** Startet die Optimierung auf dem AlcimServer (falls installiert).
*   **PMG verwalten:**
    *   **Parameter ändern:** Öffnet die Anzeige **Packmittelgruppen**, um Regel und Beschreibung zu ändern.
    *   **Optimierung rücksetzen:** Setzt eine bereits durchgeführte Optimierung zurück.
    *   **PMG löschen:** Löscht die selektierte Packmittelgruppe(n). Die Funktion ist statusabhängig.
*   **PMG ansehen:** Öffnet PackView mit dem Vorschlag des bepackten Transportgestells.
*   **Positions-Anzeige:** Öffnet für einen markierten Datensatz die Anzeige **Positionen**.
*   **Teile-Anzeige:** Öffnet für einen markierten Datensatz die Anzeige **Teile**.
*   **Glasarten-Anzeige:** Öffnet für einen markierten Datensatz die Anzeige **Glasarten**.
*   **Bearbeitungs-Anzeige:** Öffnet für einen markierten Datensatz die Anzeige **Bearbeitungen**.
*   **Detail-Anzeige:** Öffnet für einen markierten Datensatz die Anzeige **Details**.
*   **Auftrag suchen:** Öffnet den Dialog **Suchen von Aufträgen**.

### PackView

PackView startet nach einer erfolgreich durchgeführten Optimierung automatisch.

[Image: Screenshot of the PackView main interface.]
**Abb. I-78: PackView**

PackView zeigt Ihnen die Ergebnisse der Packmitteloptimierung. Das Programm teilt sich in:
*   Menü-Zeile (A)
*   Symbol-Schaltflächen (B)
*   Ansichten (C, D, E)
*   Info-Zeile am unteren Bildschirmrand (F, G, H)

#### Menü-Zeile

**Das Menü `Datei`**

| Symbol | Menü-Eintrag | Erläuterung |
| :--- | :--- | :--- |
| [Öffnen Icon] | Öffnen | Öffnet gespeicherte oder exportierte Dateien (`.out`). |
| | Schließen | Schließt die aktuelle Anzeige. |
| | Automatische Sicherung | Sichert den aktuellen Zwischenstand als `AutoSave.out`. |
| | Drucker-Setup | Öffnet den Dialog zur Druckereinrichtung. |
| | Druck-Vorschau | Zeigt eine Vorschau des Ausdrucks. |
| | Drucken | Startet den Ausdruck. |
| | Beenden | Schließt das Programm PackView. |

**Das Menü `Bearbeiten`**

| Symbol | Menü-Eintrag | Erläuterung |
| :--- | :--- | :--- |
| [Bearbeiten Icon] | Bearbeiten F3 | Schaltet den Bearbeitungs-Modus ein/aus. |
| | Gestellbezeichnung ändern ... | Öffnet Dialog zum Ändern der Gestellbezeichnung. |
| | Neues Gestell einfügen ... | Öffnet Dialog zum Einfügen eines neuen Gestells. |
| | Eigenschaften der Kiste ändern ... | Öffnet Dialog zum Ändern der Kisteneigenschaften. |
| [Rückgängig Icon] | Rückgängig | Macht die letzte Aktion rückgängig. |
| [Wiederholen Icon] | Wiederholen | Wiederholt die letzte rückgängig gemachte Aktion. |
| [Kopieren Icon] | Kopieren | Markiert die ausgewählte Einheit zum Verschieben. |
| [Ausschneiden Icon] | Ausschneiden | Entfernt die Einheit und legt sie in die Zwischenablage. |
| [Einfügen Icon] | Einfügen | Fügt den Inhalt der Zwischenablage ein. |
| [Zur grünen Kiste Icon] | Zur grünen Kiste hinzufügen | Entfernt die Einheit und überträgt sie in die grüne Kiste. |
| [Uhrzeigersinn Icon] | Rotiere Einheit im Uhrzeigersinn | Rotiert die markierte Einheit um 90 Grad im Uhrzeigersinn. |
| [Gegen-Uhrzeigersinn Icon] | Rotiere Einheit gegen Uhrzeigersinn | Rotiert die markierte Einheit um 90 Grad gegen den Uhrzeigersinn. |
| [Rechts bewegen Icon] | Einheit nach rechts bewegen | Bewegt die markierte Einheit nach rechts. |
| [Links bewegen Icon] | Einheit nach links bewegen | Bewegt die markierte Einheit nach links. |
| | Präzises bewegen | Bewegt die Einheit um 1,0 mm in die gewählte Richtung. |
| [Ausrichten Icons] | Ausrichten | Richtet die Einheit links, mittig oder rechts im Stapel aus. |

**Das Menü `Ansicht`**

| Symbol | Menü-Eintrag | Erläuterung |
| :--- | :--- | :--- |
| [3D Icon] | 3D-Anzeige | Schaltet die 3D-Anzeige ein/aus. |
| [Draufsicht Icon] | Draufsicht | Schaltet die Draufsicht ein/aus. |
| [Detail Icon] | Detail-Anzeige | Schaltet die Detail-Anzeige ein/aus. |
| [Zwischenablage Icon] | Zwischenablage anzeigen | Schaltet zwischen Gestellbelegung und Zwischenablage um. |
| [Nächstes Gestell Icon] | Zeige nächstes Gestell | Zeigt das nächste Gestell der Packmittelgruppe. |
| [Vorheriges Gestell Icon] | Zeige vorheriges Gestell | Zeigt das vorherige Gestell. |
| [Gestell auswählen Icon] | Gestell zur Anzeige auswählen ... | Öffnet Dialog zur Auswahl eines Gestells per ID. |
| [Nächste Kamera Icon] | Nächste Kamera-Position | Wechselt zur nächsten Kameraposition (45° Drehung). |
| [Vorherige Kamera Icon] | Vorhergehende Kamera-Position | Wechselt zur vorherigen Kameraposition. |
| [Ausgangskamera Icon] | Ausgangs-Kamera-Position | Setzt die Kamera auf die Standard-Einstellung zurück. |
| [Seitenansicht Icon] | Seitenansicht wechseln | Wechselt zwischen den Seiten eines A-Bocks. |
| [Experten-Modus Icon] | Experten-Modus ein/aus | Schaltet den Experten-Modus ein/aus. |
| [Freie Rotation Icon] | Freies Rotieren | Schaltet die freie Rotation der Gestellansicht ein/aus. |
| | Zeige, warum Einheit nicht platziert wird | |
| [Bemaßung Icon] | Bemaßungs-Werkzeug | Schaltet das Werkzeug zum Vermessen von Abständen ein/aus. |
| [Eigenschaften Icon] | Eigenschaften Einheit | Blendet den Dialog "Eigenschaft Einheit" ein/aus. |

#### Symbol-Schaltflächen

Eine detaillierte Beschreibung der meisten Schaltflächen finden Sie in den Tabellen zum Menü `Bearbeiten` und `Ansicht`.

#### Ansichten

PackView verfügt über eine 3D-Ansicht, Draufsicht und Detail-Ansicht.
⇨ Funktionsprinzip, "Ansichten" auf Seite I-23

#### Gestellbezeichnung ändern

**PackView > Bearbeiten ein > Menü Bearbeiten > Gestellbezeichnung ändern ...**

[Image: Screenshot of the "Gestellbezeichnung ändern" dialog.]
**Abb. I-81: Eingabe**

In diesem Dialog können Sie die Gestellbezeichnung ändern. Nur die relevanten Felder sind freigegeben.
**Technische Info:** Datenbanktabelle: `PMO_RACKS`

**Erläuterung der Felder**
*   **Gruppe:** Die Kombobox ist mit "-Aktuell-" vorbelegt. Darunter sehen Sie den Namen der Gestellbezeichnung, den Sie überschreiben können.
> **Kundenindividuelle Einstellungen**
> Je nach Installation können Sie hier auch andere Gestellgruppen auswählen, um aus einer größeren Anzahl von Gestellen zu wählen.

#### Neue Gestell-Eigenschaften

**PackView > Bearbeiten ein > Menü Bearbeiten > Neues Gestell einfügen ...**

[Image: Screenshot of the "Neue Gestell-Eigenschaften" dialog.]
**Abb. I-82: Neue Gestell-Eigenschaften**

In diesem Dialog haben Sie die Möglichkeit, ein neues Gestell hinzuzufügen.
**Technische Info:** Datenbanktabelle: `PMO_RACKS`

*   **Abmessungen:** Geben Sie Breite, Höhe und Tiefe in mm ein.
*   **Vor Gestell# einfügen:** Bestimmen Sie, vor welchem Gestell das neue Gestell eingefügt wird.
*   **Typ:** Wählen Sie den Gestelltyp (L-Gestell, A-Gestell, Kiste).

#### Eigenschaften der Kiste ändern

**PackView > Bearbeiten ein > Menü Bearbeiten > Eigenschaften der Kiste ändern ...**

[Image: Screenshot of the "Eigenschaften der Kiste ändern" dialog.]
**Abb. I-83: Neue Gestell-Eigenschaften**

Dieser Menüpunkt ist nur aktiv, wenn das selektierte Gestell eine Kiste ist.

*   **Abmessungen (Zuschlag):** Geben Sie Breite-, Höhe- und Tiefe-Zuschläge in mm ein. Damit bleibt Platz für Füllmaterial.
*   **Bezeichnung ID:** Ändern Sie den Namen der Kiste.

#### Eigenschaften Referenz-Einheiten

**PackView > Menü Ansicht > Eigenschaften Einheit**

[Image: Screenshot of the "Eigenschaften Referenz-Einheiten" dialog.]
**Abb. I-84: Eingeschaften Referenz-Einheiten**

Der Dialog gibt Ihnen Informationen zu der ausgewählten Scheibe.
*   **Los/Sequenz:** Zeigt Losnummer und Reihenfolge der Scheibe.
*   **Auftrag/Position:** Zeigt Auftrags- und Positionsnummer. Bsp.: 639478/20.
*   **Breite x Höhe x Tiefe:** Zeigt die Abmessungen in mm.
*   **Gewicht:** Zeigt das Gewicht in kg.
*   **Position (X, Y, Z):** Zeigt die Koordinaten der Scheibe auf dem Gestell.
    Beispiel: Die Koordinate `822.00, 51.00, 471.00` bedeutet, die Scheibe steht auf der X-Achse bei 822 mm, 51 mm von der Gestellrückwand weg, in einer Höhe von 471 mm.

#### Info-Zeile am unteren Bildschirmrand

[Image: Screenshot of the info bar at the bottom of the PackView window.]
**Abb. I-86: Info-Zeile am unteren Bildschirmrand**

Die Info-Zeile liefert Informationen zu Abmessungen und Gewichten der aktuellen Gestellseite. Sie ist in drei Bereiche unterteilt:
*   **Bereich A (Ausdehnung):** Informiert über die Ausdehnung der Einheiten pro Gestellseite (Länge, Höhe, Tiefe). Z.B. `1136, 1270, 168`.
*   **Bereich B (Gewicht in kg):** Informiert über die Gewichtsverteilung. Z.B. `383 (183+200) Kg` bedeutet 383 kg Gesamtgewicht, davon 183 kg auf Seite 1 und 200 kg auf Seite 2.
*   **Bereich C (Gewicht in %):** Informiert über die Lastverteilung in % für die linke und rechte Seite des Gestells. Z.B. `51% 49%`.

### Index Packmitteloptimierung

*   **A**
    *   Anzahl (Detail-Ansicht): I-29
    *   Anzeigen (Kontext-Menü): I-82
    *   Auftrags-Nr. (Detail-Ansicht): I-29
*   **B**
    *   Breite (Gestell hinzufügen): I-96, I-97
    *   Breite Zuschlag (Kiste hinzufügen): I-98
*   **D**
    *   Detail-Ansicht (Spalten): I-26 - I-30
*   **F**
    *   Filterfunktion: I-80
    *   Fläche (Detail-Ansicht): I-29
*   **G**
    *   Gestell hinzufügen: I-96, I-97
    *   Gestell#: I-26
    *   Gestellbezeichnung ändern: I-95, I-97, I-98
    *   Gestell-ID: I-29
    *   Gewicht: I-29
    *   Größe: I-29, I-30
*   **H**
    *   Höhe (Gestell hinzufügen): I-96
    *   Höhe Zuschlag (Kiste hinzufügen): I-98
*   **K**
    *   Kiste hinzufügen: I-98
*   **P**
    *   Packmittelgruppe: I-77
    *   Packmittelgruppen (Dialog): I-76 - I-77
    *   Packmittelhauptgruppe: I-76
    *   Packmittelregel: I-77
    *   PackView: I-85 - I-101
    *   PM-Gruppe (Detail-Ansicht): I-29
