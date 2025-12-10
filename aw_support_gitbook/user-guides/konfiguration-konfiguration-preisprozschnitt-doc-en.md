---
title: "Konfiguration_Preis_pro_Z-Schnitt"
source: "Konfiguration_Preis_pro_Z-Schnitt.docx"
tags: ["A+W Production", "Konfiguration", "Preis pro Z-Schnitt", "Lagerplatte", "Z-Schnitte", "MZO-Editor", "Feinplanung", "Tischoptimierung", "Maschinen", "Zuschnitt"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Diese Anleitung beschreibt, wie Sie in A+W Production Preise so konfigurieren, dass Z‑Schnitte gezielt reduziert werden. Sie zeigt zwei Stellhebel: den Preis pro m² für Lagerplatten sowie die Kosten pro Z‑Schnitt am Zuschnittstisch. Schrittweise wird erklärt, wo die Einstellungen in den Stammdaten (Artikel/Glasartikel, Maschinen/Tische, MZO‑Editor) zu finden sind und wie Werte angepasst werden. Abschließend erhalten Sie Empfehlungen, wie Sie die Parameter je nach Glasart und Prioritäten (Verschnitt vs. Zuschnittsdauer) sinnvoll wählen."
long_description: "Dieses Dokument führt durch die Konfiguration von Preisparametern in A+W Production mit dem Ziel, die Anzahl der Z‑Schnitte bei der Optimierung zu verringern. Z‑Schnitte entstehen typischerweise bei Komplexität im Zuschnitt und können die Bearbeitungszeit erhöhen sowie den Materialfluss beeinflussen. Durch eine geeignete Gewichtung von Preis und Kosten in der Optimierung lässt sich das Ergebnis in Richtung weniger Z‑Schnitte steuern, ohne die grundsätzlichen Rahmenbedingungen der Produktion zu verändern.

Zwei Parameter sind dafür zentral: Erstens der Preis pro Quadratmeter einer Lagerplatte, der im Kontext der Artikel- bzw. Glasartikelstammdaten gepflegt wird. Ein höherer Preis führt dazu, dass der Optimierer den Materialeinsatz stärker gewichtet. Zweitens die Kosten pro Z‑Schnitt am jeweiligen Zuschnittstisch. Erhöht man diese Kosten, wird ein Z‑Schnitt in der Optimierung ‚teurer‘ und folglich seltener gewählt – sofern dies mit den restlichen Restriktionen und Zielgrößen vereinbar ist.

Die Anleitung beschreibt Schritt für Schritt, wie Sie zum gewünschten Einstellungsdialog navigieren: Für Lagerplattenpreise über Stammdaten > Artikel > (Glas-)Artikel bis hin zu den Lagermaßen, in denen der Preis je Maß angepasst wird. Für die Z‑Schnitt‑Kosten gelangen Sie über Stammdaten > Maschinen > Tische zum entsprechenden Tisch oder alternativ über Stammdaten > MZO > MZO‑Editor in die Eigenschaften des Tisches. Anschließend passen Sie die Felder ‚Preis‘ (pro Lagerplatte) bzw. ‚Kosten pro Z‑Schnitt‘ an.

Im Anschluss finden Sie Empfehlungen zur Parametrierung in unterschiedlichen Szenarien. Bei teuren Glasarten, bei denen die Reduktion von Verschnitt gegenüber einer minimalen Zuschnittsdauer wichtiger ist, kann es sinnvoll sein, den Preis pro Lagerplatte zu erhöhen. Zudem lohnt es sich, mit den Kosten pro Z‑Schnitt zu experimentieren und die Ergebnisse im Mittel zu betrachten. Einzelne Optimierungsläufe können ohne sichtbare Wirkung bleiben; über mehrere Läufe hinweg sollte jedoch eine Reduktion der Z‑Schnitt‑Anzahl erkennbar sein. Die vorgenommenen Einstellungen wirken sowohl in der Feinplanung als auch in der Tischoptimierung.

Dieses Dokument dient als praxisnaher Leitfaden für Einrichter und Produktionsplaner, die die Optimierungsergebnisse gezielt beeinflussen möchten – transparent, reproduzierbar und innerhalb der vorgesehenen Konfigurationsmöglichkeiten von A+W Production."
---
## Z-Schnitte reduzieren über Preise

## Einstellen der Preise pro Lagerplatte

**Schritte**

1. Der Preis pro m² einer Lagerplatte kann folgendermaßen im A+W Production geändert werden:
2. Über Stammdaten > Artikel > Artikel oder Glasartikel
3. Dann öffnet sich eine Maske, in der alle Artikel aufgeführt sind.
4. Rechts gibt es den Button
5. In der neuen Maske wird der zugehörige Glasartikel ausgewählt. Hier kann es aber mehrere Lagerplatten-maße geben. Für jedes Maß gibt es eine Zeile:
6. Auf den Button Lagermaße gehen.
7. Jetzt öffnen sich die gespeicherten Parameter zu dem Lagermaß:
8. Oben auf
9. gehen, damit man hier den Wert im Feld Preis ändern kann.

## Ändern des Preises pro Z-Schnitt

**Methode 1: Über Stammdaten > Maschinen > Tische**

1. Um die Preise pro Z-Schnitt am Zuschnittstisch zu ändern gehen Sie über Stammdaten > Maschinen > Tische und wählen den gewünschten Tisch aus:
2. Oben wieder auf Ändern gehen, dann kann das Feld Kosten pro Z-Schnitt angepasst werden.

**Alternative: Über Stammdaten > MZO > MZO-Editor**

1. Hier den entsprechenden Tisch auswählen und auf Bearbeiten gehen.
2. Im Drop-Down Eigenschaften des Tisches (Aufklappen) in der Zeile Kosten pro Z-Schnitt den gewünschten Wert eintragen:

## Empfehlung

- Erhöhen Sie bei teuren Glasarten, bei denen der Verschnitt wichtiger ist als die Zuschnittsdauer, den Preis pro Lagerplatte.
- Spielen Sie mit den Kosten pro Z-Schnitt, bis Ihnen das gemittelte Ergebnis sinnvoll erscheint. Bei einzelnen Optimierungen kann es durchaus vorkommen, dass der Preis pro Z-Schnitt keine Auswirkung hat. Im Mittel jedoch sollte die Anzahl der Z-Schnitte reduziert werden.
- Die so gemachten Einstellungen gelten sowohl für die Feinplanung als auch für die Tischoptimierung.
