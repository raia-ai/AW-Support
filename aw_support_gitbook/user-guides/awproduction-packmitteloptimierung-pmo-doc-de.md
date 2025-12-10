---
title: "DE_AWProduction_PMO_2.00"
source: "DE_AWProduction_PMO_2.00.pdf"
tags: ["A+W Production", "Packmitteloptimierung", "PMO", "Software Manual", "Glass Manufacturing", "Window Manufacturing", "Logistics", "Stacking", "Optimization"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A user manual for the A+W Production \"Packmitteloptimierung\" (Packaging Optimization) module, version 2.00. It details the setup, operation, and reference for optimizing the loading of glass, windows, and doors onto transport racks and crates to save space and streamline production logistics."
long_description: "This document is the comprehensive German user manual for the A+W Production \"Packmitteloptimierung\" (PMO), or Packaging Optimization, software module, version 2.00. It is intended for end-users and administrators of the A+W software suite for glass, window, and door manufacturing. The manual is divided into a Tutorial, a Software Reference, and an Index. The Tutorial section explains the fundamental concepts of PMO, which aims to eliminate intermediate storage and complex sorting by planning the direct packing of production units onto transport racks. It covers master data setup (RUL and VAL files), parameter configuration for stacking rules, and how to use the PackView visualization tool. The PackView tool allows users to see a 3D representation of the optimized racks, manipulate units, and manage loading sequences. The Software Reference section provides a detailed breakdown of all menus, dialogs, buttons, and functions within the PMO module, including creating and managing packaging groups, setting rules and values, and using the various display and editing modes in PackView."
---

# A+W Packmitteloptimierung

**A+W - Software for Glass, Windows and Doors**

---
## Vorspann
In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version / Datum | Beschreibung |
| :--- | :--- |
| 2.00 / 01-2023 | Freien Editier-Modus ergänzt. |
| 1.02 / 01-2017 | Produkt- und Firmennamen angepasst. |
| 1.01 / 07-2013 | Vollständige Überarbeitung der ALCIM-Dokumentation und Anpassung auf A+W Production. |
| 1.00 / 03-2007 | Ersterstellung |

### Editorial
Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen
- Kontakte

#### Anmerkungen zu diesem Dokument
Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Production gedacht.
Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.
Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.
Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von A+W Production.

#### Urheberrechte
© 2023, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.
Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

#### Warenzeichen
Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

#### Kontakte
**A+W Software GmbH**
Am Pfahlgraben 4-10
D-35415 Pohlheim
📞 +49 6404 2051-0
📠 +49 6404 2051-877
Zentrale@a-w.com
http://www.a-w.com

## Tutorial

### Grundgedanke
Die Packmitteloptimierung erspart Ihnen sowohl aufwändiges Umsortieren als auch das Zwischenlager. Sie richtet den gesamten Produktionsprozess auf die Direktverpackung und die bestmögliche Auslastung der Packmittel (Gestelle und Versandkisten) aus.

In einer Produktion ohne Packmitteloptimierung (PMO) werden alle Einheiten, die aus der Produktion kommen, in einem Zwischenlager abgestellt. Danach müssen die Einheiten auf Transportgestelle verpackt werden, was mit aufwändigen Sortierungen verbunden ist. Meist stehen die Einheiten im Zwischenlager nicht in der Reihenfolge zur Verfügung, wie sie für das Transportgestell benötigt werden. Es kann auch der Fall sein, dass das Transportgestell nach Kundenwünschen beladen werden muss, oder es muss eine bestimmte Tour- bzw. Abladereihenfolge eingehalten werden.

Die Aufgabe der Packmitteloptimierung ist, die gewünschten Auftragspositionen unter Beachtung von Nebenbedingungen so auf Packmittel (Gestelle) zu verplanen, dass der Platzbedarf beim Transport minimal ist und Kundenwünsche beim Gestellaufbau erfüllt werden. Die Strategie bei der Verplanung wird durch Packmittelregeln formuliert. Diese enthalten neben den Angaben zu physikalischen Eigenschaften (wie Höhe, Breite und Gewicht) auch kundenspezifische Parameter für die zu verwendenden Packmittel (wie Anzahl der Stapel nebeneinander und übereinander).

In der Packmittelplanung werden Aufträge in gemeinsam zu verpackende Gruppen (Packmittelgruppen) eingeteilt, z. B. gleicher Liefertermin, gleiche Tour, gleiche Lieferanschrift.

### Allgemeines
Dieses Kapitel gibt Ihnen einen Überblick, wie die Packmitteloptimierung (PMO) aufgebaut ist und wie sie grundsätzlich arbeitet. Die Stammdaten der Packmitteloptimierung sind komplex und es sind umfangreiche Kenntnisse nötig, um die Packmitteloptimierung korrekt zu projektieren.

In der Packmitteloptimierung gibt es zwei getrennt zu behandelnde Bereiche von Vorgaben:
- Die physikalischen Bedingungen (Gestellregeln), die beim Versand eingehalten werden müssen (Gewicht, Anordnung der Stapel, Abstände, etc.).
- Die von Endkunden gewünschte Behandlung seiner Auftragspositionen (gruppieren, sortieren, auf spezielle Gestelle stellen, etc.).

Für den Endkunden ist in den meisten Fällen die Abnahmereihenfolge wichtig, in der die produzierten Einheiten von den Versandgestellen abgenommen werden können. Je strenger die Vorgaben für diese Reihenfolge sind, desto weniger Freiheit hat die Packmitteloptimierung bei der Verplanung der Gestelle. Das hat zur Folge, dass die Planungsdichte tendenziell schlechter sein wird.

Häufig wird gewünscht, dass Einheiten gemeinsam abnehmbar sind. So sollen zum Beispiel alle Einheiten eines Auftrags gemeinsam abnehmbar sein. Oder es sollen alle Einheiten einer Position hintereinander entladbar sein. Dabei ist noch nicht gesagt, dass solche gemeinsam abnehmbaren Einheiten auch nahe beieinander auf den Gestellen stehen. Es könnte durchaus sein, dass die Einheiten in verschiedenen Stapeln oder sogar auf verschiedenen Gestellen stehen. Die Optimierung stellt aber immer sicher, dass keine anderen Einheiten zunächst abgenommen werden müssen, um an alle gemeinsam abnehmbaren Gläser heran zu kommen. Je mehr Freiheit die Optimierung bei dieser Verplanung hat, desto besser sind die Planungsdichten auf den Gestellen, desto weniger Gestelle werden benötigt.

Eine Packmittelgruppe kann in Sets (etwa entsprechend der Aufträge) eingeteilt sein. Das bedeutet, dass die in einem Set enthaltenen Positionen entladen werden können, ohne andere Positionen anzufassen. Dabei kann das Set durchaus auf verschiedene Stapel oder Packmittel verteilt sein. Die Abladereihenfolge der Sets kann dabei von der Packmitteloptimierung selber bestimmt oder auch vorgegeben werden. Es gibt auch die Möglichkeit die Sets so zu planen, dass sie unabhängig voneinander in wahlfreier Reihenfolge entladen werden können.

Stapel auf dem Gestell müssen eine baumförmige Struktur haben. Zum Beispiel ein großer Stapel zu Beginn gefolgt von maximal 2 weiteren Stapeln, vor denen wieder maximal 2 Stapel stehen dürfen. Das sieht von oben gesehen so aus (die Gestellrückwand ist grau gezeichnet):

**Abb. I-1: Gestellbeladung von oben gesehen**
(Bild zeigt eine schematische Draufsicht auf eine baumförmige Stapelanordnung vor einer Gestellrückwand.)

Eine weitere Möglichkeit ist die Strukturierung einzelner Stapel durch Matrizen. Eine Matrix ist ein Aufbau, der es erlaubt, mehrere Einheiten nebeneinander und übereinander gleichzeitig zu platzieren. Dazu ist die Beachtung folgender Eigenschaften nötig:
- Alle Einheiten einer Reihe, bis auf die oberste Reihe, müssen die gleiche Höhe haben.
- Alle Einheiten einer Reihe müssen die gleiche Dicke haben.
- Die Gesamtbreite jeder Reihe muss kleiner oder gleich der Gesamtbreite der unteren Reihe sein.
- Die Dicke jeder Reihe muss kleiner oder gleich der Dicke der unteren Reihe sein.
- Jede Reihe steht zentriert auf der unteren Reihe.

Daher können in einem Stapel Einheiten nebeneinander und übereinander stehen. Das können Einheiten aus einer oder auch aus verschiedenen Auftragspositionen sein. Von vorne kann dann ein einzelner Stapel so aussehen:

**Abb. I-2: Matrixbeladung: Stapel von vorne gesehen**
(Bild zeigt eine schematische Frontansicht einer Matrixbeladung, bei der kleinere Einheiten (1/2, 2/2) auf größeren Einheiten (1/1, 2/1, 3/1) zentriert platziert sind.)

Die oberen Stapel stehen dabei immer zentriert auf den unteren.

Mit Matrizen kann man insbesondere erreichen, dass vor zwei Stapeln wieder ein größerer Stapel steht (nicht baumförmig).

**Abb. I-3: Matrixbeladung von oben gesehen**
(Bild zeigt eine schematische Draufsicht, bei der ein großer Stapel vor zwei kleineren Stapeln platziert ist.)

Einheiten aus einer Position werden zunächst grundsätzlich nach Möglichkeit zusammengehalten. Wenn eine Position wegen max. Gewicht oder Gestelltiefe nicht auf ein Gestell passt, wird sie geteilt.

### Stammdaten
Für den Anwender sind im Umgang mit der Packmitteloptimierung zwei Stammdaten-Typen sichtbar:
- **Optimierungsregeln (*.RUL-Datei):** Die *.RUL-Dateien enthalten allgemeine Einstellungen, Angaben zu physikalischen Gestellen und zugehörige Belegungsregeln. Diese können z. B. je nach Kunde oder Auftrag vergeben werden.
- **Einstellwerte (*.VAL-Datei):** Die *.VAL-Dateien ermöglichen kundenspezifische Einstellwerte zu den Optimierungsregeln.

Die *.RUL- und *.VAL-Dateien stehen dem Anwender zur Auswahl zur Verfügung. Geringfügige Modifikationen wie z. B. maximale Gestellbeladung können für eine bestimmte Packmittelgruppe vom Anwender durchgeführt werden.

> **Weitere Stammdaten**
> Darüber hinaus gibt es noch Gestellregeln, Verladeregeln und Regelzuweisungen. Diese Regeln werden durch die Firma A+W in Zusammenarbeit mit dem Anwender erarbeitet und gefüllt. Möchten Sie Veränderungen an der in Ihrem Hause implementierten Packmitteloptimierung vornehmen, halten Sie bitte unbedingt Rücksprache mit A+W, da es sonst zu unerwünschten Ergebnissen kommen kann!

#### Optimierungsregeln (*.RUL-Datei)
Die *.RUL-Dateien enthalten die Gestellregeln. In den Gestellregeln wird beschrieben, welche Packmittel mit welcher jeweiligen maximalen Anzahl und mit welchen Vorgaben zur Beladung geplant werden können. Das können Gestelle (A-Bock, L-Bock) oder auch Kisten (in Standard- oder Individualmaßen) sein.
*Siehe Softwarereferenz, "Regeln" auf Seite 1-69*

#### Einstellwerte (*.VAL-Datei)
Die *.VAL-Dateien enthalten die Zuweisungen der kundenspezifischen Packmittelparamtern (*.VAL-Dateien) zu den Gestellregeln. Theoretisch kann für jede *.RUL-Datei eine eigene *.VAL-Datei angelegt werden, es sollte aber der dann notwendige Pflegeaufwand nicht außer Acht gelassen werden.
*Siehe Softwarereferenz, "Werte" auf Seite 1-71*

### Parameter
Zum Beladen der Gestelle arbeitet die Packmitteloptimierung mit unterschiedlichen Parametern. Im Anschluss finden Sie nähere Erläuterungen zu einzelnen, häufig verwendeten Parametern. Die in Ihrem Hause verwendeten Parameter können aufgrund Ihrer individuellen Anforderungen davon abweichen.

**Name des Parameters: Sets in Stapeln zusammenstellen.**
Erläuterung: Mit diesem Wert legen Sie fest, wie Sets in Stapeln (z. B. Aufträge) zusammen gestellt werden.
Mögliche Werte:
- 0-Nein, freie Optimierung,
- 1-Mono,
- 2-Multi,
- 3-Peripher.

- **Mono:** Im Mono-Modus kann jedes Set entladen werden, ohne Einheiten aus einem anderen Set anzufassen. Alle Sets können in jeder gewünschten Reihenfolge entladen werden. Daher steht in jedem Stapel nur ein Set.
  **Abb. I-4 & I-5:** (Bilder zeigen, dass jedes Set auf einem eigenen Stapel oder blockweise getrennt liegt)

- **Multi:** Der Multi-Modus gleicht dem Mono-Modus, jedoch kann jedes Set in maximal einem Stapel mit anderen Sets gemischt stehen. In einem gemischten Stapel steht jedes Set blockweise für sich (getrennt von den anderen Sets).
  **Abb. I-6 & I-7:** (Bilder zeigen, dass Sets auf einem Stapel gemischt sein können, aber immer noch als Blöcke entnehmbar sind)

- **Peripher:** Im Peripher-Modus kann jedes Set entladen werden, ohne Einheiten aus anderen Sets anzufassen. Die Reihenfolge der Entladung steht aber fest (entweder durch PMO oder den Anwender). Daher kann es mehr als ein Set pro Stapel geben.
  **Abb. I-8:** (Bild zeigt, dass mehrere Sets pro Stapel möglich sind, solange die Entladereihenfolge gewahrt bleibt)

- **Frei:** Im Freien-Modus können Sets und Positionen nicht zusammen entladen werden. Die Aufträge stehen gemischt, um die höchste Packdichte zu erreichen.
  **Abb. I-9, I-10 & I-11:** (Bilder zeigen eine gemischte Anordnung verschiedener Sets zur Maximierung der Dichte)

**Name des Parameters: Sets bestehen aus.**
Erläuterung: Mit diesem Wert bestimmen Sie, wie Sets gebildet werden. Sie können Sets nach Aufträgen, nach Kommissionen oder aber nach Touren bilden.
Mögliche Werte:
- 1=Auftrag,
- 2=Kommission,
- 3=Tour.

**Name des Parameters: Sets auf Gestellen zusammenhalten?**
Erläuterung: Mit diesem Wert bestimmen Sie, ob und wenn ja, wie die Sets auf den Gestellen zusammen gehalten werden. 0 bedeutet, dass die Sets nicht auf Gestellen zusammen gehalten werden. Bei einer 1 werden die Sets auf einem Gestell zusammen gehalten und bei einer 2 auf maximal zwei Gestellen.
Mögliche Werte:
- 0=nein,
- 1=ein Gestell,
- 2=zwei Gestelle.

**Name des Parameters: Sets sortiert entladen?**
Erläuterung: Mit diesem Wert bestimmen Sie, ob und wenn ja, wie die Sets entladen werden sollen. Standardmäßig ist dieser Eintrag mit 0 vorbelegt. D. h. die Sets werden nicht sortiert.
Mögliche Werte:
- 0=nein,
- 1=Sets aufsteig. ++,
- 2=Set absteig. --.

**Name des Parameters: Maximales Gewicht für alle Gestelltypen**
Erläuterung: Der hier eingetragene Wert kennzeichnet das maximale Gewicht aller Gestelltypen dieser Packmittelgruppe. Der Wert ist in kg anzugeben.

**Name des Parameters: Maximale Anzahl der Stapel aufeinander (Standard=1)**
Erläuterung: Der hier eingetragene Wert besagt, wie viele Stapel aufeinander gestellt werden dürfen. Standardmäßig ist der Wert 1 eingetragen. Das bedeutet, dass keine Stapel aufeinander stehen dürfen. Die größtmögliche Anzahl aufeinander stehender Stapel ist 5.

**Name des Parameters: Maximaler Überstand links/rechts (Standard: 100 mm)**
Erläuterung: Dieser Wert kennzeichnet den maximalen Gestellüberstand. Der hier eingetragene Wert wirkt sowohl links als auch rechts. Standardmäßig ist der Wert 100 eingetragen. Das bedeutet, dass der Überstand auf der rechten und auf der linken Gestellseite 100 mm ist. Der größt mögliche Wert ist 1000 (1000 mm).

**Name des Parameters: Maximales Seitenverhältnis für aufrechte Scheiben (Standard = 3.0)**
Erläuterung: Bei diesem Wert handelt es sich um den Minimalwert des Verhältnisses zwischen größeren/kleinerem Scheibenmaß, ab welchem die Scheiben liegend platziert werden. Beispiel: Bei einer Vorgabe von 2 wird die Scheibe 2500/1000 liegend platziert und die Scheibe 1500/1000 stehend. Standardmäßig ist der Wert 3 eingetragen. Der größt mögliche Wert ist 5. Eine 1 bewirkt, dass alle Scheiben auf die längere Seite gedreht werden.

**Name des Parameters: Max. Seitenverhältnis für aufrechte Scheiben beim Aufeinanderstapeln (Std=2.0)**
Erläuterung: Bei diesem Wert handelt es sich um das maximale Seitenverhältnis einer Einheit beim Aufeinanderstapeln, also wenn die Einheit auf einer anderen Einheit steht. Der Parameter wirkt nur dann, wenn er kleiner ist als der Parameter Maximales Seitenverhältnis für aufrechte Scheiben.

### Anzeigen
Die Packmitteloptimierung verfügt über eine eigene Anzeige, die Ihnen die Packmittelgruppen anzeigt, die Sie gebildet haben.

#### Packmittelgruppen-Anzeige
Die Packmittelgruppen-Anzeige öffnen Sie entweder über das Menü Anzeigen > Packmittelgruppen-Anzeige oder aber über die Symbol-Schaltfläche.

**Abb. I-12: Symbol-Schaltfläche Packmittelgruppen-Anzeige**

**Abb. I-13: Packmittelgruppen-Anzeige**
(Bild zeigt das Fenster "Packmittelgruppen" mit Registern, Tabellenspalten, Kopfzeile und Schaltflächen.)
- A: Register
- B: Tabellenspalte
- C: Tabellenkopf
- D: Schaltflächen zur Schnellanwahl
- E: Summenzeile
- F: Filterfunktion

Die Packmittelgruppen-Anzeige gibt Ihnen einen Überblick zu den bereits gebildeten Packmittelgruppen. Packmittelgruppen können Sie über das Kontext-Menü folgender Anzeigen bilden:
- Auftrags-Anzeige
- Bearbeitungs-Anzeige
- Detail-Anzeige

Über die Register können Sie sich die Packmittelgruppen-Anzeige grob strukturieren. Innerhalb der Register stehen Ihnen zur weiteren Unterteiltung Tabellenspalten zur Verfügung. Ferner können Sie sich Filter anlegen, um die Anzeige für bestimmte Situationen noch weiter einzuschränken.

Informationen zu den Filtern und der Summenzeile finden Sie im Part Grobplanung.

Die Schaltflächen zur Schnellanwahl können in den einzelnen Anzeigen unterschiedlich sein. In der Packmittelgruppen-Anzeige haben Sie für einen oder mehrere markierte Einträge schnellen Zugriff auf:
- **Laufbildung:** Es öffnet sich der Dialog Lauf-Bildung.
- **Glasarten:** Es öffnet sich der Dialog Glasarten-Anzeige.
- **Details:** Es öffnet sich der Dialog Detail-Anzeige.

#### Restriktionen
Über das Kontext-Menü der Packmittelgruppen-Anzeige haben Sie die Möglichkeit, Packmittelgruppen zu bearbeiten. D.h. Sie können Packmittelgruppen verschieben, löschen und ändern. Die einzelnen Funktionen sind jedoch abhängig vom Status der Packmittelgruppe.

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

#### So bilden Sie Packmittelgruppen
Die Vorgehensweise zum Bilden von Packmittelgruppen ist für alle Anzeigen (Aufträge, Bearbeitungen, etc.) gleich. Wir erläutern die Vorgehensweise deshalb nur einmal am Beispiel der Anzeige Aufträge.
1. Öffnen Sie die Anzeige Aufträge.
2. Selektieren Sie den bzw. die Aufträge, mit denen Sie eine Packmittelgruppe bilden möchten.
3. Öffnen Sie das Kontext-Menü und wählen Sie Packmittelgruppe bilden.
4. Es öffnet sich der Dialog Packmittelgruppen.
5. Geben Sie im Feld Packmittelhauptgruppe den Namen für die Packmittelhauptgruppe an.
6. Geben Sie im Feld Packmittelgruppe den Namen für die Packmittelgruppe an.
7. Wählen Sie aus der Kombobox Packmittelregel die entsprechende Regel aus.
8. Geben Sie im Feld Beschreibung eine weitere Bezeichnung für die Packmittelgruppe an.
9. Aktivieren oder deaktivieren Sie die Checkbox Positionen von Optimierung ausschließen.
10. Aktivieren oder deaktivieren Sie die Checkbox Mehrere Produktionslinien zusammenfassen.
11. Ändern Sie bei Bedarf die VAL-Einstellungen.
12. Betätigen Sie die Schaltfläche [OK].
13. Der bzw. die selektieren Aufträge werden aus der Anzeige Aufträge entfernt und in der Anzeige Packmittel angezeigt.

#### So starten Sie die Optimierung für eine Packmittelgruppe
1. Öffnen Sie die Anzeige Packmittel.
2. Selektieren Sie den bzw. die Packmittelgruppe, die Sie optimieren möchten.
3. Öffnen Sie das Kontext-Menü und wählen Sie PMG optimieren.
4. Die Optimierung wird gestartet.

#### So nehmen Sie Änderungen an den Parametern einer bestehenden Packmittelgruppe vor
1. Öffnen Sie die Anzeige Packmittel.
2. Selektieren Sie den bzw. die Packmittelgruppe, an der Sie Änderungen vornehmen möchten.
3. Öffnen Sie das Kontext-Menü und wählen Sie PMG verwalten > Parameter ändern.
4. Es öffnet sich der Dialog Packmittelgruppen. Änderungen, die Sie zu diesem Zeitpunkt vornehmen können, beziehen sich auf die Felder:
    - Packmittelregel
    - Beschreibung
    - Positionen von Optimierung ausschließen
    - Mehrere Produktionslinien zusammenpacken
    - VAL
5. Wählen Sie aus der Kombobox Packmittelregel die entsprechende Regel aus.

### Optimierung ansehen
Nach Durchführung der Packmitteloptimierung können Sie sich, in einer dreidimensionalen Ansicht, die Ergebnisse als Vorschau anzeigen lassen. Ergebnisse bedeutet: Wie werden die Einheiten auf dem Transportgestell stehen? Sie können in dieser Ansicht die optimierten Gestelle auch mit wenigen Mausklicks umpacken. Die Software zur Visualisierung der Packmittelergebnisse heißt **PackView**.

**Abb. I-14: PackView**
(Bild zeigt die PackView-Benutzeroberfläche mit einer 3D-Ansicht, Draufsicht und Detail-Ansicht eines beladenen Gestells.)
- A: Menü-Zeile
- B: Symbol-Schaltflächen
- C: 3D-Ansicht
- D: Draufsicht
- E: Detail-Ansicht der Einheit
- F: Gewichtsverteilung auf linker und rechter Gestellseite
- G: Gesamtgewicht in kg (Vorder- und Rückseite)
- I: Ausdehnung der Gesamtbeladung auf der aktuellen Gestellseite: Breite, Höhe, Tiefe
- J: Experten-Modus, Einstellräder für Nahsicht.

PackView startet nach einer erfolgreich durchgeführten Optimierung automatisch.

#### Ansichten
PackView verfügt über folgende Ansichten:
- 3D-Ansicht
- Draufsicht
- Detail-Ansicht

In welcher der drei Ansichten Sie sich momentan befinden, sehen Sie an der gelben Umrandung der entsprechenden Ansicht. Mit der Maus können Sie einzelne Einheiten auswählen. Eine ausgewählte Einheit wird grundsätzlich auch in den anderen Ansichten in Rot hervorgehoben.

**3D-Ansicht**
Die 3D-Ansicht ermöglicht Ihnen die dreidimensionale Sicht beider Seiten eines Gestells. Welche Gestellseite angezeigt wird, sehen Sie an der roten Zahl in der linken, oberen Ecke der Ansicht.
Um die Gestellseite zu wechseln, stehen Ihnen folgende Möglichkeiten zur Verfügung:
- Öffnen Sie im Menü Ansicht den Menüpunkt Seitenansicht wechseln.
- Betätigen Sie auf Ihrer Tastatur die `<Leertaste>`.
- Betätigen Sie die Symbol-Schaltfläche.

Sie können sich ein Gestell aus mehreren Blickwinkeln anzeigen lassen (Kamera-Positionen). Um zur nächsten Kamera-Position zu wechseln, stehen Ihnen folgende Möglichkeiten zur Verfügung:
- Öffnen Sie im Menü Ansicht den Menüpunkt Nächste Kamera-Position oder Vorhergehende Kamera-Position.
- Betätigen Sie im Bereich des Nummernblocks die Taste `<+>` oder `<->`.
- Betätigen Sie die Symbol-Schaltflächen.

In der 3D-Ansicht können Sie Einheiten über die Funktion Kopieren verschieben.

**Draufsicht**
Die Draufsicht zeigt Ihnen das Gestell von oben. Die rote Einheit ist die aktuell ausgewählte Einheit. Sie können in der Draufsicht, wie auch in der 3D-Ansicht Einheiten über die Funktion Kopieren verschieben oder an ihrem Platz drehen.

**Detail-Ansicht**
Die Detail-Ansicht zeigt Ihnen tabellarisch, wie die Auftragspositionen auf den Gestellen stehen. Die Tabelle ist in Beladereihenfolge sortiert.
Der Tabellenkopf enthält die Spalten:
- **Gestell#:** unterteilt in Seite, Stapel
- **Gestellbeschreibung:** unterteilt in Anzahl, Reihe
- **Gestell-ID:** unterteilt in Fläche [m²], Vert. Stapel
- **Typ:** unterteilt in Gewicht [kg], Anzahl
- **PM-Gruppe:** unterteilt in Auftrags-Nr.
- **Größe [mm]:** unterteilt in Positions-Nr., Größe [mm], Gewicht [kg], Produktions-Linie

**Erläuterung des Tabellenkopfes und der Tabellenspalten**
- **Gestell#:** Das aktuelle Gestell mit der Gesamtzahl der Gestelle (z.B. 1/3).
- **Seite:** Gestellseite 1 oder 2.
- **Stapel:** Zeigt an, in welchem Stapel sich die Einheit befindet. Die Anzahl der Stapel ist von der Gestell- und Einheitengröße abhängig.
- **Gestellbeschreibung:** Der vergebene Name für das Gestell.
- **Anzahl:** Wie viele einzelne Einheiten sich auf der aktuellen Seite befinden.
- **Reihe:** Wie viele Stapel voreinander stehen.
- **Gestell-ID:** Die ID des aktuell angezeigten Gestells.
- **Fläche [m²]:** Quadratmeter der Einheiten auf der Seite.
- **Vert. Stapel:** Wie viele vertikale Stapel übereinander stehen.
- **Typ:** Abstellplatztyp (A = A-Bock, L = L-Bock, Box = Kiste).
- **Gewicht [kg]:** Gewicht des Glases auf der Seite.
- **Anzahl:** Wie viele Einheiten eine Position hat und welche Einheit die aktuelle ist (z.B. 1/2).
- **PM-Gruppe:** Die Packmittelhauptgruppe und Packmittelgruppe.
- **Auftrags-Nr.:** Auftragsnummer des Kunden.
- **Positions-Nr.:** Positionsnummer zum Auftrag.
- **Größe [mm]:** Abmessungen der Einheit.
- **Gewicht [kg]:** Gewicht der Einheit.
- **Produktions-Linie:** Fertigungslinie der Einheit.

#### Modi
In PackView können Sie in drei unterschiedlichen Modi arbeiten:
- Vollbild-Modus
- Bearbeitungs-Modus
- Experten-Modus

**Vollbild-Modus**
PackView befindet sich nach dem Start im Vollbild-Modus. Sie können mit der Maus eine Scheibe markieren. Die ausgewählte Einheit wird in roter Farbe dargestellt. Im Vollbild-Modus haben Sie Zugriff auf die unterschiedlichen Kamera-Positionen.

> **Modus**
> In welchem Modus Sie sich befinden (Vollbild/Bearbeiten), wird Ihnen im Programm am Ende der Titelleiste in eckigen Klammern angezeigt. Beispiel: [Vollbild].

**Bearbeitungs-Modus**
In den Bearbeitungs-Modus gelangen Sie über das Menü `Bearbeiten > Bearbeiten`, die Taste `<F3>` oder die Symbol-Schaltfläche. Die ausgewählte Einheit wird in grüner Farbe dargestellt. PackView wählt automatisch immer Teilstapel aus, die auch tatsächlich bewegt werden können.

**Experten-Modus**
In den Experten-Modus gelangen Sie über `Ansicht > Experten-Modus ein/aus` oder die Symbol-Schaltfläche. Hier haben Sie zusätzlich die Möglichkeit, das Gestell zu zoomen und auf der X- bzw. Y-Achse zu rotieren oder frei zu rotieren.

**Freier Editier-Modus**
Dieser Modus erlaubt es Ihnen, Scheiben auf einem Gestell umzuorganisieren, ohne dass physikalische Einschränkungen berücksichtigt werden. Sie können z. B. beliebige Scheiben auswählen und erweiterte Bewegungen und Aktionen durchführen.
- Mit `<Strg>` + `<linke Maustaste>` können beliebige Einheiten ausgewählt werden.
- Mit der `ENTER`-Taste kann ein "Locator" (eine Gruppe von Einheiten) erstellt werden.
- Mit den Pfeiltasten Auf/Ab können Scheiben vor- und zurückbewegt werden.
- Mit der `Alt`-Taste kann die Ausrichtung in Bezug auf das Gestell erzwungen werden.
- Scheiben können gedreht werden.
- Eine automatische Gültigkeitsprüfung wird durchgeführt, wenn der Bearbeitungsmodus ausgeschaltet wird. Ungültige Platzierungen werden farblich markiert.

#### Zwischenablage
Wenn Sie eine oder auch mehrere Einheiten ausgeschnitten haben, werden diese nach dem Ausschneiden automatisch in die Zwischenablage gestellt.

**So wählen Sie das nächste/vorherige Gestell zur Anzeige aus**
1. Wählen Sie im Menü `Ansicht > Zeige nächstes Gestell`, verwenden Sie die entsprechende Symbol-Schaltfläche oder die Tasten `<BildAuf>` bzw. `<BildAb>`.

**So wählen Sie ein beliebiges Gestell zur Anzeige aus**
1. Wählen Sie im Menü `Ansicht > Gestell zur Anzeige auswählen...`.
2. Es öffnet sich der Dialog Eingabe. Geben Sie die gewünschte Gestellnummer ein.
3. Nach Betätigen der Schaltfläche [OK] wird das entsprechende Gestell angezeigt.

#### So verschieben Sie eine oder wenige Einheiten
1. Aktivieren Sie den Bearbeitungs-Modus.
2. Markieren Sie die Einheit(en), die Sie verschieben möchten. Sie bekommen einen grünen Rahmen.
3. Kopieren Sie die Einheit(en) über das Menü `Bearbeiten > Kopieren`, die Symbol-Schaltfläche oder `<Strg>+<C>`.
4. Verschieben Sie die Einheit an die gewünschte Stelle mithilfe der Richtungstasten oder der Symbol-Schaltflächen.
5. Ist die Einheit an der neuen Stelle, fügen Sie sie über `Bearbeiten > Einfügen` oder die Symbol-Schaltfläche ein.

#### So verschieben Sie einen ganzen Stapel
1. Aktivieren Sie den Bearbeitungs-Modus.
2. Markieren Sie die Einheit des Stapels, die der Gestellrückwand am nächsten steht. Der gesamte Stapel wird markiert.
3. Kopieren Sie den Stapel.
4. Verschieben Sie den Stapel an die gewünschte Stelle.
5. Fügen Sie den Stapel an der neuen Position ein.

#### So arbeiten Sie mit der Zwischenablage
Wenn Sie viele Einheiten, etwa aus verschiedenen Stapeln, auf einer anderen Gestellseite oder einem anderen Gestell platzieren möchten, geht dies gut über die Zwischenablage.
1. Aktivieren Sie den Bearbeitungs-Modus.
2. Markieren Sie die zu verschiebenden Einheit(en).
3. Schneiden Sie die Einheit(en) über `Bearbeiten > Ausschneiden` oder die Symbol-Schaltfläche aus. Die Einheiten erscheinen in der Zwischenablage.
4. Wechseln Sie zu der gewünschten Gestellseite bzw. dem gewünschten Gestell.
5. Lassen Sie sich den Inhalt der Zwischenablage anzeigen. Sie können die Einheiten hier sortieren (z.B. nach Breite oder Höhe).
6. Klicken Sie auf die Schaltfläche [Einfügen]. Der Mauszeiger ändert sich zu einem Fadenkreuz.
7. Bewegen Sie das Fadenkreuz an die Stelle, wo die Einheit(en) eingefügt werden sollen.
8. Betätigen Sie die linke Maustaste. Die Einheit(en) werden eingefügt.
9. Wiederholen Sie den Vorgang für alle Einheiten in der Zwischenablage.

## Softwarereferenz

### Menüs
Dieser Abschnitt gibt eine Übersicht der Dialoge und Funktionen in den verschiedenen Menüs und Kontext-Menüs.

| Menü-Eintrag | Dialog/Funktion |
| :--- | :--- |
| **PMO (Stammdaten)** | |
| Regeln | Siehe Kapitel "Regeln" |
| Werte | Siehe Kapitel "Werte" |
| **Kontext-Menü (Aufträge, etc.)** | |
| Packmittelgruppe bilden | Siehe Kapitel "Packmittelgruppen" |
| **Kontext-Menü (Packmittelgruppe)** | |
| Packmittelgruppe verschieben | Siehe Kapitel "PMG verschieben" |
| Packmittelgruppe optimieren | Siehe Kapitel "PMG optimieren" |
| Packmittelgruppe optimieren im Hintergrund | Siehe Kapitel "PMG optimieren im Hintergrund" |
| Packmittelgruppe verwalten | Siehe Kapitel "PMG verwalten" |
| Optimierung ansehen | Siehe Softwarereferenz, "PackView" |
| **Menü Anzeigen** | |
| Packmittelgruppen-Anzeige | Siehe Kapitel "Packmittelgruppen-Anzeige" |

### Regeln
**Stammdaten > PMO > Regeln**
In diesem Dialog erfassen Sie neue Optimierungsregeln oder ändern bestehende Regeln ab.
- **.RUL-Dateien laden:** Lädt *.RUL-Dateien aus dem Verzeichnis.
- **Tabellenspalten:** `.RUL-Datei`, `Bezeichnung`, `VAL_FILE`.
- **Felder:** `.RUL-Datei`, `Bezeichnung`, `Beschreibung`, `.VAL-Datei`.

### Werte
**Stammdaten > PMO > Werte**
In diesem Dialog erfassen Sie die kundenspezifischen Werte oder nehmen Änderungen an bestehenden Werten vor.
- **.VAL-Dateien laden:** Lädt *.VAL-Dateien aus dem Verzeichnis.
- **Tabellenspalten:** `.VAL-Datei`, `Parameter`, `Bezeichnung`, `Mindestwert`, `Maximalwert`, `Wertetyp`.
- **Felder:** `Nummer des Packmittelparameters`, `Bezeichnung`, `Beschreibung`, `Mindestwert`, `Maximalwert`.

**Packmittelparameter:**
1.  Sets in Stapeln zusammenhalten (0-nein, 1-mono, 2-multi, 3-peripher)
2.  Sets bestehen aus (1-Auftrag, 2-Kommission, 3-Tour)
3.  Sets auf Gestellen zusammen halten? (0-nein, 1-ein Gestell, 2-zwei Gestelle)
4.  Sets sortiert entladen? (0-nein, 1-aufsteigend, 2-absteigend)
5.  Maximales Gewicht für alle Gestelltypen
6.  Maximale Anzahl der Stapel aufeinander (Standard=1)
7.  Maximaler Überstand links/rechts (Standard: 100mm)
8.  Maximales Seitenverhältnis für aufrechte Scheiben (Standard=3.0)
9.  Max. Seitenverhältnis für aufrechte Scheiben beim Aufeinanderstapeln (Std.=2.0)

### Packmittelgruppen
**Aufträge > Kontext-Menü > Packmittelgruppen bilden**
In diesem Dialog nehmen Sie die Einstellungen vor, mit denen die Packmittelgruppe gebildet werden soll.
- **Packmittelhauptgruppe:** Wählen oder erstellen Sie eine Hauptgruppe.
- **Packmittelgruppe:** Wählen oder erstellen Sie eine Untergruppe.
- **Packmittelregel:** Weisen Sie eine Regel zu.
- **Beschreibung:** Optionale Erläuterung.
- **Positionen von Optimierung ausschließen:** Checkbox, um Positionen von der Optimierung auszunehmen.
- **Mehrere Produktionslinien zusammenpacken:** Checkbox, um Einheiten verschiedener Linien zu mischen.

### Packmittelgruppen-Anzeige
**Anzeigen > Packmittelgruppen-Anzeige**
Diese Anzeige gibt einen Überblick über die gebildeten Packmittelgruppen. Sie besteht aus:
- **Summenzeile:** Zeigt einen zahlenmäßigen Überblick über markierte Einträge.
- **Filterfunktion:** Ermöglicht das Filtern der Anzeige nach Kriterien.
- **Schaltflächen zur Schnellanwahl:** Schneller Zugriff auf Funktionen wie `Laufbildung (F6)`, `Glasarten (F7)`, `Details (F8)`.

### Kontext-Menü bei markiertem Eintrag
Verfügt über folgende Menüpunkte:
- **PMG verschieben:** Öffnet die Anzeige Packmittelgruppen zum Verschieben.
- **PMG optimieren:** Startet die Optimierung für die selektierte(n) Gruppe(n).
- **PMG optimieren im Hintergrund:** Startet die Optimierung auf dem AlcimServer.
- **PMG verwalten:** Untermenü mit:
  - **Parameter ändern:** Ändern der Packmittelregel und Beschreibung.
  - **Optimierung rücksetzen:** Setzt eine durchgeführte Optimierung zurück.
  - **PMG löschen:** Löst die Zuordnung der Aufträge zur Gruppe auf.
- **PMG ansehen:** Öffnet PackView mit dem Ergebnis.
- **Positions-Anzeige / Teile-Anzeige / etc.:** Öffnet die entsprechenden Anzeigen für den Datensatz.
- **Auftrag suchen:** Öffnet den Dialog zum Suchen von Aufträgen.

### PackView
PackView startet nach einer erfolgreich durchgeführten Optimierung automatisch. Es zeigt die Ergebnisse der Packmitteloptimierung.

#### Menü-Zeile
- **Datei:** Öffnen, Schließen, Automatische Sicherung, Drucker-Setup, Druck-Vorschau, Drucken, Beenden.
- **Bearbeiten:** Bearbeiten F3, Gestellbezeichnung ändern, Neues Gestell einfügen, Eigenschaften der Kiste ändern, Rückgängig, Wiederholen, Kopieren, Ausschneiden, Einfügen etc.
- **Ansicht:** 3D-Anzeige, Draufsicht, Detail-Anzeige, Zeige nächstes/vorheriges Gestell, Kamera-Positionen, Experten-Modus etc.

#### Symbol-Schaltflächen
Eine Toolbar mit Icons für den schnellen Zugriff auf die wichtigsten Funktionen wie:
- Datei öffnen
- Gestell zur Anzeige auswählen
- Seitenansicht wechseln
- Zeige vorhergehendes/nächstes Gestell
- Kamera-Positionen wechseln
- Bearbeiten ein/aus
- Rückgängig/Wiederherstellen
- Einheit Kopieren/Ausschneiden/Einfügen
- Einheiten rotieren/ausrichten
- Experten-Modus, Freie Rotation
- Bemaßungs-Werkzeug
- Anzeigen (3D, Draufsicht, Detail, Zwischenablage)

#### Ansichten
PackView verfügt über 3D-Ansicht, Draufsicht und Detail-Ansicht. Details dazu finden sich im Tutorial-Abschnitt.

#### Gestellbezeichnung ändern
**PackView > Bearbeiten ein > Menü Bearbeiten > Gestellbezeichnung ändern ...**
Ermöglicht das Ändern des Namens (Bezeichnung) eines Gestells.

#### Neue Gestell-Eigenschaften
**PackView > Bearbeiten ein > Menü Bearbeiten > Neues Gestell einfügen ...**
Ermöglicht das Hinzufügen eines neuen Gestells mit spezifischen Dimensionen (Breite, Höhe, Tiefe) und Typ (L-Gestell, A-Gestell, Kiste).

#### Eigenschaften der Kiste ändern
**PackView > Bearbeiten ein > Menü Bearbeiten > Eigenschaften der Kiste ändern ...**
Nur aktiv für Kisten. Ermöglicht das Anpassen der Zuschläge (Breite, Höhe, Tiefe) für Füllmaterial.

#### Eigenschaften Referenz-Einheiten
**PackView > Menü Ansicht > Eigenschaften Einheit**
Zeigt detaillierte Informationen zu einer ausgewählten Scheibe an:
- **Los/Sequenz:** Losnummer und Sequenz aus der Feinplanung.
- **Auftrag/Position:** Auftrags- und Positionsnummer.
- **Breite x Höhe x Tiefe:** Abmessungen der Scheibe.
- **Gewicht:** Gewicht der Scheibe.
- **Position (X, Y, Z):** Koordinaten der Scheibe auf dem Gestell.

#### Info-Zeile am unteren Bildschirmrand
Liefert Informationen zu den Abmessungen und Gewichten der jeweiligen Gestellseite.
- **Bereich A (Ausdehnung):** Länge, Höhe und Tiefe der Bepackung.
- **Bereich B (Gewicht in kg):** Gesamtgewicht des Gestells und pro Seite.
- **Bereich C (Gewicht in %):** Lastverteilung links/rechts in Prozent.

## Partindex

### Index Packmitteloptimierung

**A**
- **Anzahl**
  - Detail-Ansicht
- **Anzeigen**
  - Kontext-Menü bei markiertem Eintrag
- **Auftrags-Nr.**
  - Detail-Ansicht

**B**
- **Breite**
  - Gestell hinzufügen
- **Breite Zuschlag**
  - Kiste hinzufügen

**D**
- **Detail-Ansicht**
  - Anzahl, Auftrags-Nr., Fläche, Gestell#, Gestellbezeichnung, Gestell-ID, Gewicht, Größe, PM-Gruppe, Positions-Nr., Produktions-Linie, Reihe, Seite, Stapel, Typ, Vert. Stapel

**F**
- **Filterfunktion**
  - Pool-Anzeige
- **Fläche**
  - Detail-Ansicht
- **Freier Editier-Modus**

**G**
- **Gestell hinzufügen**
  - Breite, Höhe, Tiefe
- **Gestell#**
  - Detail-Ansicht
- **Gestellbezeichnung**
  - Detail-Ansicht
  - Gestellbezeichnung ändern (PackView)
- **Gestell-ID**
  - Detail-Ansicht
- **Gewicht**
  - Detail-Ansicht
- **Größe**
  - Detail-Ansicht

**H**
- **Höhe**
  - Gestell hinzufügen
- **Höhe Zuschlag**
  - Kiste hinzufügen

**K**
- **Kiste hinzufügen**
  - Breite Zuschlag
  - Höhe Zuschlag
  - Tiefe Zuschlag

**P**
- **Packmittelgruppe**
- **Packmittelgruppen**
  - Beschreibung, Packmittelgruppe, Packmittelhauptgruppe, Packmittelregel, Positionen von einer Optimierung ausschließen, Produktionslinien zusammenpacken
- **Packmittelhauptgruppe**
- **Packmittelregel**
- **PackView**
  - Automatische Sicherung, Datei öffnen, Datei schließen, Drucken, Drucker Setup, Druck-Vorschau, Gestellbezeichnung ändern, Menü, Programm Beenden, Symbol-Schaltflächen
- **PM-Gruppe**
  - Detail-Ansicht
- **Pool-Anzeige**

