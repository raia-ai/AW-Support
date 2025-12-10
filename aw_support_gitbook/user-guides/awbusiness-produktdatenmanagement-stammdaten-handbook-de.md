---
title: "A+W Business Stammdaten - Tutorial 1: Produktdaten, Preise, Lager"
source: "D-HB-AWBusiness_3.pdf"
tags: ["A+W Business", "ERP-Software", "Produktdatenmanagement", "Stammdaten", "Warengruppen", "Preisverwaltung", "Stücklisten", "Lagerverwaltung", "Fertigungssteuerung", "Glasindustrie"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Dieses Tutorial bietet eine umfassende Anleitung zur Verwaltung von Produktdaten im A+W Business ERP-System. Es behandelt die Erstellung und Organisation von Produkten, Produktarten, Warengruppen und Stücklisten sowie die Konfiguration von Fertigungs- und Preisparametern."
long_description: "Dieses Dokument ist ein detailliertes Tutorial zur Stammdatenverwaltung innerhalb der A+W Business Software, das sich primär an Anwender in der Glasindustrie richtet. Es führt schrittweise durch die Konfiguration von Produktdaten, die für den gesamten Geschäftsprozess von der Auftragserfassung über die Fertigung bis zur Preisberechnung grundlegend sind. Das Tutorial beginnt mit der Definition von Produkten, Produktarten, Produktgruppen und Warengruppen, einschließlich ihrer hierarchischen Organisation und deren Bedeutung für die Preis- und Rabattfindung. Es werden Konzepte wie Kombi- und Top-Warengruppen erläutert, die für Auswertungen und Statistiken relevant sind. Ein weiterer Schwerpunkt liegt auf der Erstellung und Verwaltung von Stücklisten für komplexe Produkte wie Isolierglaseinheiten. Dabei werden die Preis- und Produktionsrelevanz von Komponenten sowie Vererbungsmechanismen für Maße und Zuschläge erklärt. Das Dokument beschreibt zudem die Konfiguration von fertigungsrelevanten Daten, wie Maßzuschläge, Strukturen, Beschichtungen und Sprossenkonstruktionen. Es wird detailliert auf die verschiedenen Preis- und Mengeneinheiten sowie deren Anwendung eingegangen. Die Verwaltung von Preisen wird in einem eigenen Kapitel behandelt, das die Definition von Preislisten, Preisjahrgängen, Preisschlüsseln und Tarifen umfasst. Verschiedene Preismethoden wie Einzelpreisberechnung, ISO-Preise mit Austauschzuschlägen und die Berücksichtigung von Mindestmengen werden vorgestellt. Schließlich behandelt das Tutorial die Lagerverwaltung, einschließlich der Unterscheidung zwischen Lagermaßen und Lagerartikeln, der Definition von Beschaffungsarten und der Verwaltung von Produktvarianten wie Farben."
---

# Tutorial 1: Produkt

---
## Lernziele
- Nutzen der Produkte kennenlernen.
- Produktarten, Produktgruppen kennenlernen.
- Produktorganisation in Warengruppen kennenlernen.
- Funktion der Kombi- und Top-Warengruppen kennenlernen.

## Nutzen
- Produkte bilden die Basis für Auftrags- und Bestellpositionen und für die Berechnung von Preisen im Verkauf und im Einkauf.
- Über die Produktstammdaten wird die gesamte Produktstruktur abgebildet.

## Merke

| Begriff | Erklärung |
| :--- | :--- |
| **Produkt** | Produkte sind die Grundlagen der Preis- und Kostenkalkulation, der Disposition, der Material- und Zeitwirtschaft, für technische Prüfungen usw. |
| **Produktarten** | Produktarten bilden die Basis für Produkte. Unter Produktarten sind nicht nur Gläser oder Glasarten, sondern auch Modelle, Bearbeitungen, Zuschläge usw. zu verstehen, die im Auftrag wie ein Produkt erfasst werden. |
| **Produktgruppen** | Die Produktarten werden wiederum in Produktgruppen unterteilt. Produktarten und -gruppen fassen die Produkte für die Produktionsübergabe und für programminterne Zwecke zusammen. |
| **Warengruppen** | Alle Produkte werden einer Warengruppe zugeordnet. Die Warengruppen und Kombinationen von Warengruppen haben eine zentrale Bedeutung bei der Preisfindung, z. B. um Rabatte und Zuschläge zu berechnen. Warengruppen bilden folgende Hierarchie:<ul><li>WHG: Warenhauptgruppe</li><li>WOG: Warenobergruppe</li><li>WGR: Warengruppe</li></ul> |
| **Kombi-WGR** | Warengruppen können miteinander kombiniert werden. Diese Warengruppen-Kombinationen (Kombi-WGR) dienen zur Rabattfindung und Auswertung. |
| **Top-Warengruppen** | Top-Warengruppen werden bei der Erstellung von Umsatzstatistiken ausgewertet. |
| **Mengeneinheit** | Zu jedem Produkt wird hinterlegt, welche Maßangaben zu seiner konkreten Beschreibung notwendig sind. Im Allgemeinen geschieht dies über die Mengeneinheit. |

---
*A+W Business Stammdaten*
*B-201*
---

## Produktarten und Produktgruppen
Produktarten bilden die Basis für Produkte. Unter Produktarten sind nicht nur Gläser oder Glasarten, sondern auch Modelle, Bearbeitungen, Zuschläge usw. zu verstehen, die im Auftrag wie ein Produkt erfasst werden.

Die Produktarten werden wiederum in Produktgruppen unterteilt. Produktarten und -gruppen fassen die Produkte für die Produktionsübergabe und für programminterne Zwecke zusammen, z.B. für die Vorauswahl bei der Erfassung von Auftragspositionen.

**Abb. B-75: Produktarten, Produktgruppen**

| Produktart | Produktgruppen | Produkt |
| :--- | :--- | :--- |
| Einfachglas | Einfachglas, Ornamentglas | Float 6 mm, Orn. Ald. Glastt 4 mm, Orn. Kathed. weiß 4 mm |
| ISO | ISO, 3-fach ISO | CLIMALIT Standard 2x4, CLIMASOL silber 53/39 |
| ESG | ESG, Ganzglastür | ESG klar 12 mm, ESG Tür weiß |
| Modelle | Modelle, Stufung | Standard-Modell 1 – 135, Modell 999 |
| Abstandhalter | Alu, Stahl, TPS | 12 mm, 16 mm |
| Leistungen | Anzahlung, Zuschläge, UV-Randverbund | Anzahlung, Eilzuschlag |
| Bearbeitungen | Rundecken, Randausschnitt | Rundecke fein, Rundecke grob, Randausch. 100x200 mm |

Jedes Produkt wird einer Produktgruppe und damit einer Produktart zugeordnet.

---
*B-202*
*A+W Business Stammdaten*
---

### Produktorganisation: Beispiel Abstandhalter
In diesem Beispiel sehen Sie, dass der Produktart **Abstandhalter** verschiedene Produktgruppen zugeordnet sind. In der Produktgruppe **Alu** sind die Abstandhalter mit unterschiedlichen Maßen zusammengefasst.

**Abb. B-76: Produktorganisation: Beispiel Abstandhalter**

*   **A: Produktarten**
    *   Tabelle zeigt verschiedene Produktarten wie "Abstandhalter", "Bearbeitungen", "Einfachglas", "ESG" etc. mit einem Schlüssel.

*   **B: Produktgruppen der Produktart Abstandhalter**
    *   Tabelle zeigt, dass zur Produktart "Abstandhalter" die Produktgruppen "Abstandhalter", "Alu", "Stahl", "Thermix", "TPS" gehören.

*   **C: Produkte der Produktgruppe ALU**
    *   Tabelle listet spezifische Produkte der Gruppe "Alu" auf, z.B. "ALUSTEG 6" (6 mm ALU Profil), "ALUSTEG 8" (8 mm ALU Profil) usw.

> **Neue Produktarten oder Produktgruppen**
> Die Produktarten sind fest in A+W Business vorgegeben. Die Produktgruppen können zwar geändert oder angelegt werden, greifen im System aber nicht. Wenn Sie weitere Produktarten und Produktgruppen benötigen, wenden Sie sich bitte an die A+W Software GmbH.

---
*A+W Business Stammdaten*
*B-203*
---

## Warengruppen
Grundsätzlich werden alle Produkte einer Warengruppe zugeordnet. Die Warengruppen und Kombinationen von Warengruppen haben eine zentrale Bedeutung bei der Preisfindung, z. B. um Rabatte und Zuschläge zu berechnen. Für die Umsatzstatistik können Sie zusätzlich Top-Warengruppen anlegen.

### Warengruppen 0xx
Jede Warengruppe wird mit einer 3-stelligen alphanumerischen Nummer gekennzeichnet, die die Hierarchie-Ebene anzeigt.

**Abb. B-77: Hierarchischer Aufbau der Warengruppen**
Die Abbildung zeigt eine Baumstruktur der Warengruppen:
- **A: WHG (Warenhauptgruppe)**: z.B. `1**` (Isolierglas), `2**` (Sicherheits-Isolierglas)
- **B: WOG (Warenobergruppe)**: z.B. `21*` (durchbruchhemmend) unter `2**`
- **C: WGR (Warengruppe)**: z.B. `210` (B1 31 mm Iso.) unter `21*`
- **D: WHG mit alphanumerischer Nummer**: z.B. `A**` (Antikgläser)

Die Warenhauptgruppe 0**, Warenobergruppe 00* und Warengruppe 000 sind fest angelegt. Alle anderen Warengruppen können Sie nach eigenen Regeln nummerieren.

- Die **Warenhauptgruppe (WHG)** dient zur Rabattvergabe und zu statistischen Auswertungen. Beispiel: WHG 1**. Wenn mehr als 10 WHG (0** bis 9**) benötigt werden, können Sie auch Buchstaben zur Nummerierung verwenden, z. B. A**.
- Die **Warenobergruppe (WOG)** dient zur Rabattvergabe und zu statistischen Auswertungen. Beispiel: WOG 10*.
- Die **Warengruppe (WGR)** dient zur Rabattvergabe, Produktorganisation und Statistik. Nur dieser Ebene kann ein Produkt zugeordnet werden. Beispiel: WGR 105.

---
*B-204*
*A+W Business Stammdaten*
---

> **Tipp zur Zuordnung der Warengruppen**
> Der Warengruppe 000 werden in der Regel nur Modelle zugeordnet. So kann in der Statistik z. B. der Modellumsatz automatisch dem Umsatz des Hauptproduktes zugeordnet werden.
> Sprossen und Bearbeitungen haben in der Regel eigene Warengruppen.

### Hierarchie der Warengruppen bei der Auswertung
Um in der Umsatzstatistik weitere Differenzierungen zu erhalten, können Sie Top-Warengruppen und Kombinationen von Warengruppen angelegen, z. B. für die verschiedenen ISO-Gläser mit Modellen. Daneben werden Modelle den Einfachgläsern oder den ISO-Gläsern usw. zugeordnet und mit diesen zusammen ausgewertet.

- **Top-Warengruppe (Top-WGR)**, z. B. Sprossen.
  - Relevant für Statistikauswertung.
- **Warenhauptgruppe (WHG)**, z. B. 1**.
  - Relevant für Rabattvergabe und Statistikauswertung.
- **Warenobergruppe (WOG)**, z. B. 10*.
  - Relevant für Rabattvergabe und Statistikauswertung.
- **Warengruppe (WGR)**, z. B. 105.
  - Relevant für Rabattvergabe. Nur die Warengruppe kann einem Produkt zugeordnet werden.

Wie die Warengruppen im Einzelnen für die Statistik ausgewertet werden, ist im Part Statistik beschrieben.

### Kombi-WGR
Warengruppen können miteinander kombiniert werden. Diese Warengruppen-Kombinationen (Kombi-WGR) dienen zur Rabattfindung und Auswertung, z. B. um den Umsatz von ISO-Einheiten in den verschiedenen Aufbauten darzustellen.

**Beispiele**
Kombi-WGR für die Umsatzstatistik bieten sich für folgende Auswertungen an:
- ISO (ohne alles)
- ISO mit Modell
- ISO mit Sprossen
- ISO mit Modell und Sprossen
- VSG mit Bearbeitung
- VSG mit Modell und Bearbeitung

Jede Kombination von Warengruppen ergibt eine sogenannte Kombi-WGR. Diese wird jedoch nicht automatisch durch die Kombination erzeugt, sondern muss zuvor angelegt werden wie jede andere WGR auch.

Jede Kombination kann nur einmal angegeben werden, selbst dann, wenn Sie eine andere Nummer für die Kombi-WGR wählen.

---
*A+W Business Stammdaten*
*B-205*
---

**Abb. B-78: Definition der Kombi-Warengruppen**
Die Abbildung zeigt das Einstellungsfenster für Kombi-Warengruppen.
- **A**: Felder zur Auswahl der zu kombinierenden Warengruppen (Warengruppe 1 und Warengruppe 2).
- **B**: Eine Tabelle, die bestehende Kombinationen auflistet, inklusive der resultierenden Kombi-WGR Nummer.
- **C**: Checkboxen zur Angabe der Verwendung der Kombination (z.B. `gültig für Rabattfindung`, `gültig für Statistik`).

Bei der Definition einer Kombi-WGR können Sie unterscheiden, ob die Kombination für die Rabattfindung oder für die Statistik gelten soll. Zusätzlich können Sie festlegen, ob z. B. bei der Suche nach einem Rabattsatz nur das Hauptprodukt ausgewertet werden soll oder alle Produkte der Stückliste.

### Regeln für Kombi-WGR
Bei der Bildung von Kombi-WGR müssen Sie bestimmte Regeln einhalten. An Beispielen sind folgende Regeln erklärt:
- Kombi-Regeln für die Nummernvergabe
- Kombi-Regeln bei Folgebearbeitungen
- WGR-Kombinationen mit kompletter Stückliste bilden

#### Kombi-Regeln für die Nummernvergabe
In der Regel vergeben Sie eine eindeutige Nummer für eine Kombi-WGR. Die Nummernvergabe kann auch mit Platzhaltern gesteuert werden, so dass die Produkte automatisch zugeordnet werden. Als Platzhalter werden die Symbole `<` für links und `>` für rechts eingesetzt.

---
*B-206*
*A+W Business Stammdaten*
---

**Abb. B-79: Beispiel für Kombi-Warengruppe**
Dieses Beispiel zeigt eine Kombination, die im System konfiguriert wird.
- **A**: Definition der Kombi-WGR: WGR `1**` (Isolierglas) wird mit WGR `9*` (Aufwand ISO) zu Kombi-WGR `19>` kombiniert. Das Symbol `>` bedeutet, dass die 3. Stelle der WGR `19*` angesprochen wird.
- **B**: Gültigkeit: Die Kombination gilt für Rabatte und Statistik.
- **C**: Statistik-Einstellung: Die Statistik soll nur für die Hauptposition angewendet werden.
- **D**: Beispielhafter Bruch-Artikel: Der Artikel `AW ISO Prod./Bruchersatz` mit der WGR-Nummer `190` wird als Beispiel für einen Aufwandsartikel gezeigt.

In diesem Beispiel sehen Sie die Kombination von WGR 1** und WGR 9* zu Kombi-WGR 19> (A). Das Symbol > bedeutet, dass die 3. Stelle der WGR 19* angesprochen werden soll.

Bei der Kombination einer ISO-Einheit (WGR 1**) mit Bruch (D) soll ein Rabatt (B) berücksichtigt werden. Da für Bruch vermutlich kein Rabatt definiert ist, wird also nur für die ISO-Einheit der Rabatt berechnet. Daher erübrigt sich die Markierung der Checkbox für die Hauptposition. Die Kombination (ISO und Bruch) soll statistisch ausgewertet werden und dabei in die Statistik für ISO (C) einfließen.

---
*A+W Business Stammdaten*
*B-207*
---

#### Beispiele für unterschiedliche Kombinationen

**Tab. B-2: Regeln der Kombi-WGR (Beispiele)**

| | WGR 1 | WGR 2 | Kombi-WGR | Erklärung |
| :--- | :--- | :--- | :--- | :--- |
| **Definition** | 10* | 81* | 1G< | Die letzte Zahl der WGR 1 wird zugewiesen. |
| **Beispiel** | 101 | 814 | 1G1 | Die letzte Zahl der WGR 1 ist die Zahl 1, daher 1G1. |
| **WGR** | 100-109 | 811-815 | 1G0-1G9 | Die möglichen Warengruppen-Kombinationen 1G0-1G9 müssen als WGR angelegt sein. |
| **Definition** | 10* | 81* | 1G> | Die letzte Zahl der WGR 2 wird zugewiesen. |
| **Beispiel** | 101 | 814 | 1G4 | Die letzte Zahl der WGR 2 ist die Zahl 4, daher 1G4. |
| **WGR** | 100-109 | 811-815 | 1G1-1G5 | Die möglichen Warengruppen-Kombinationen 1G0-1G5 müssen als WGR angelegt sein. |
| **Definition** | 22* | 766 | 966 | Feste Vorgabe. |
| **Beispiel** | 224 | 766 | 966 | Die Kombi-WGR ist hier immer 966. |
| **WGR** | 220-229 | 766 | 966 | Die Warengruppen-Kombination 966 muss als WGR angelegt sein. |
| **Definition** | 3** | 19* | 4<< | Die 2. und 3. Zahl der WGR 1 wird zugewiesen. |
| **Beispiel** | 376 | 195 | 476 | Die letzten Zahlen der WGR 1 sind 7 und 6, daher 476. |
| **WGR** | 300-387 | 190-199 | 400-487 | Die möglichen Warengruppen-Kombinationen 400 - 487 müssen als WGR angelegt sein. |
| **Definition** | 3** | 19* | 4>> | Die letzten beiden Zahlen der WGR 2 werden zugewiesen. |
| **Beispiel** | 376 | 195 | 495 | Die letzten Zahlen der WGR 2 sind 9 und 5, daher 495. |
| **WGR** | 300-387 | 190-199 | 400-499 | Die möglichen Warengruppen-Kombinationen 400-499 müssen als WGR angelegt sein. |

#### Erläuterung zu den Beispielen
Für das erste der aufgeführten Beispiele gilt:
- WGR 10* enthält die WGR 100–109, 10A-10Z, 10a-10z, z. B. für ISO-Einheiten.
- WGR 81* enthält die WGR 810–815, z. B. für Sprossen.

Damit in der Statistik die ISO-Einheiten mit Sprossen ausgewertet werden können, soll die WGR 10* mit WGR 81* kombiniert werden. Das Resultat ist eine Kombi-WGR mit der Nummer 1G<.

Das Symbol < steht für Warengruppe 1. Es steht an 3. Stelle und bezieht sich daher auf die 3. Stelle der WGR 1.

---
*B-208*
*A+W Business Stammdaten*
---

Für die Kombination WGR 101 und 814 bedeutet 1G< gleich 1G1. Das heißt, dass die Auswertung der Kombination in WGR 1G1 einfließt.

In gleicher Weise sind die weiteren Beispiele gebildet.

Die Regel kann auch auf die zweite und sogar die erste Stelle angewendet werden. Dies erzeugt jedoch eine Vielzahl an möglichen Kombinationen und ist daher fehlerträchtig.

Wichtig ist, dass Sie alle Warengruppen anlegen, die durch eine Kombi-WGR möglich sind. Für das erste Beispiel sind dies die WGR 1G0 bis 1G9.

#### Kombi-Regeln bei Folgebearbeitungen
Bei der Produktion von Auftragspositionen können mehrere Arbeitsschritte erfasst sein, z. B. ein Isolierglas mit Sprossen und Modell.

Wenn alle Komponenten einer solchen Stückliste in eine Warengruppen-Kombination einfließen sollen, gelten folgende Kombinationsregeln:

**Tab. B-3: Kombi-Regeln bei Folgebearbeitungen (Beispiele)**

| | WGR 1 | WGR 2 | Kombi-WGR | Erklärung |
| :--- | :--- | :--- | :--- | :--- |
| **Definition** | 12* | 5** | A2A | Grundsätzlich gilt die WGR A2A. |
| **Beispiel** | 121 (ISO) | 502 (Sprossen) | A2A | Aus ISO + Sprosse wird A2A. |
| **Definition** | A2A | 5** | A2A | Grundsätzlich gilt die WGR A2A. |
| **Beispiel** | A2A (ISO + Sprosse) | 540 (Modell) | A2A | Aus ISO + Sprosse + Modell wird A2A. |

Wenn keine entsprechende Folgekombination (A2A + 5** = A2A) definiert ist, wird die Ursprungs-WGR der Bearbeitung genommen (540).

#### WGR-Kombinationen mit kompletter Stückliste bilden
Um Kombi-Warengruppen mit vollständiger Stückliste abzubilden, müssen Sie in den Firmendaten festlegen, ob bei einer Kombi-WGR die gesamte Stückliste auf Rabatte geprüft werden soll. Diese Einstellung gilt dann für alle Kombi-WGR.
⇨ Softwarereferenz, "WGR-Kombinationen mit kompletter Stückliste bilden" auf Seite B-1087

---
*A+W Business Stammdaten*
*B-209*
---

#### Kombinationsbeispiele für Warengruppen mit Stückliste

**WGR Bezeichnung (Beispiele)**
- **100** Float 4 mm
- **101** Float 4 mm, Kanten poliert
- **102** Float 4 mm, Lochbohrung
- **103** Float 4 mm, Kanten poliert und Lochbohrung
- **400** Facetten
- **600** Kanten polieren
- **800** Lochbohrung

**Tabelle der Kombinationen**
| WGR 1 + WGR 2 | Kombi-WGR | Bezeichnung |
| :--- | :--- | :--- |
| 100 + 600 | 101 | Float 4 mm, Kanten poliert |
| 100 + 800 | 102 | Float 4 mm, Lochbohrung |
| 101 + 800 | 103 | Float 4 mm, Kanten poliert und Lochbohrung |
| 102 + 600 | 103 | Float 4 mm, Kanten poliert und Lochbohrung |

Abhängig von den Einstellungen in den Firmendaten wird entweder die für das Produkt gültige Warengruppenkombination herangezogen oder es wird alles aus der Stückliste in die letzte in der Position gefundene Kombination gebucht.

**Tabelle: Auswirkung der Checkbox "WGR-Kombinationen mit kompletter Stückliste bilden"**

| Produkt | WGR 1 + WGR 2 | Checkbox WGR-Kombinationen mit kompletter Stückliste bilden (Firmendaten) |
| :--- | :--- | :--- |
| | | **[ ] (deaktiviert)** | **[✔] (aktiviert)** |
| Float 4 mm | 100 | 101 | 103 |
| + Kanten poliert | 600 | | |
| + Facetten | 400 | - | 400 | 103 |
| + Lochbohrung | 800 | 101 | 103 | 103 |

Im Beispiel sehen Sie, welche Warengruppen bebucht werden, wenn in den Firmendaten die Checkbox WGR-Kombinationen mit kompletter Stückliste bilden aktiviert oder deaktiviert ist.

---
*B-210*
*A+W Business Stammdaten*
---

## Top-WGR
Jede beliebige Warengruppe (WGR) kann einer Top-WGR zugeordnet werden. Diese dienen in der Umsatzstatistik zur gesonderten Auswertung.

> **Beispiel**
> Eine Top-WGR für Sprossen ist sinnvoll, wenn in der Statistik alle Sprossen über Kombi-WGR in die verschiedenen ISO-Gläser einfließen. Sie können damit pro Standard-ISO oder pro Wärmeschutz-ISO sehen, was an Sprossen produziert wurde. Die Sprossen oder die ISO-Einheiten allein können Sie aber nur über die Top-WGR auswerten.
>
> Wenn Sie allen Warengruppen, die Sprossen beinhalten, die Top-WGR Sprossen zuordnen, erhalten Sie in der Umsatzstatistik eine Gesamtübersicht über alle Sprossenproduktionen.

Top-WGR werden nicht als Warengruppen angelegt, sondern in einer Basistabelle.

> **Top-WGR zuordnen**
> Nur Warengruppen der dritten Ebene können einer Top-Warengruppe zugeordnet werden.

## Maß- und Mengeneinheiten
Neben der strukturellen Beschreibung eines Produktes (Stückliste) sind für die Berechnung des Preises Mengeneinheiten notwendig, auf die sich der Preis bezieht. Die jeweils gültige Einheit muss pro Produkt festgelegt sein. Die Einheiten sind fest vorgeben.

In den Stammdaten wird zu jedem Produkt hinterlegt, welche Maßangaben zu seiner konkreten Beschreibung notwendig sind. Im Allgemeinen geschieht dies über die Mengeneinheit:

- **Stück:**
  Die Mengeneinheit Stück wird z. B. für Artikel wie Handgriffe, Noppen usw. eingesetzt.
- **Volumen:**
  Die Mengeneinheit Liter wird für Gas eingesetzt. Im Auftrag wird die Stückzahl (= Literangabe) abgefragt.
- **Zeit:**
  Die Mengeneinheit Stunden wird für besondere Leistungen oder Bearbeitungen eingesetzt. Im Auftrag wird die Stückzahl (= Anzahl der Stunden) pro Position abgefragt.
- **Laufmeter:**
  Die Mengeneinheit Laufmeter wird für die Länge (je Meter) von Sprossen, Kantenbearbeitungen usw. eingesetzt. Im Auftrag werden die Stückzahl und die Länge pro Position abgefragt.
- **Fläche:**
  Die Mengeneinheit Fläche bezeichnet die Gesamtfläche in qm (Breite x Höhe) von Gläsern oder Scheiben. Im Auftrag werden die Stückzahl, die Breite und die Höhe der Position abgefragt.

---
*A+W Business Stammdaten*
*B-211*
---

### Maßberechnung
Zur Berechnung bei Maßen können Formeln und Variablen eingesetzt werden. Folgende Variablen haben bereits eine feste Bedeutung und können nicht verändert werden:
- **$1** = Breite
- **$2** = Höhe
- **$3** = SZR1 (Scheibenzwischenraum 1) oder Tiefe
- **$4** = SZR2 (Scheibenzwischenraum 2, für 3-fach-ISO)

> **Verfügbare Variablen**
> Im Tutorial 2 finden Sie eine Übersicht über die verfügbaren Variablen und Platzhalter, die in Formeln eingesetzt werden können.
> ⇨ Tutorial 2, "Verfügbare Variablen (Platzhalter)" auf Seite B-599

Die Maße werden für die Preisberechnung gerundet. In Deutschland basiert die Preisberechnung für Glas auf einer 30er-Rundung. Dies bedeutet, dass zur Berechnung der nächste durch 30 teilbare Wert zugrunde gelegt wird.

> **Beispiel**
> **Rundung 30:**
> Bei einem Glas von 1000 x 1000 mm wird der Preis für die Fläche 1,04 qm (= 1020 x 1020 mm) berechnet.
> Die Scheibe wird aber auf das Maß 1000 x 1000 mm zugeschnitten.

In anderen Ländern gelten andere Maßrundungen, z. B. in Frankreich die 10er-Rundung.

Maßrundungen werden in folgenden Bereichen angegeben:
- **Produkt**
  ⇨ Softwarereferenz, "Produktverwaltung - Preis/Zuschlag" auf Seite B-717
- **Preisliste**
  ⇨ Softwarereferenz, "Preisverwaltung" auf Seite B-836
- **Stammdaten der Kunden und der Lieferanten**
  ⇨ Softwarereferenz, "Partnerverwaltung - Auftrag" auf Seite B-892

Wenn A+W Business in mehreren Bereichen Angaben zur Maßrundung findet, gilt folgende Hierarchie: Partner > Produkte > Preise > Rabatte > Individualpreise. Die Eintragung in den Individualpreisen gilt vor allen anderen.

---
*B-212*
*A+W Business Stammdaten*
---

## Warengruppen anlegen
Warengruppen (WGR) dienen der übersichtlichen Strukturierung der Produkte, zur schnellen Erfassung von Artikeln, zur Zuordnung von Rabatten und Zuschlägen und zur Auswertung in der Statistik. Außerdem werden Budgetierung, Provisionierung und Erlöskontenberechnung auf Basis der Warengruppen durchgeführt.

Sinnvoll sind auch Warengruppen, die ausschließlich für die Statistik angelegt werden.

> **WHG, WOG oder WGR anlegen**
> Warenhauptgruppe (X**), Warenobergruppe (XX*) und Warengruppe (XXX) werden auf die gleiche Weise angelegt.

### So legen Sie eine Warengruppe an
1.  Wählen Sie im Menü **Stammdaten > Produkte > Allgemein > WGR**.
    Der Dialog **Warengruppen** wird geöffnet.
    ⇨ Softwarereferenz, "WGR" auf Seite B-680
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.

    **Abb. B-80: Felder für neue Warengruppe freigeschaltet**
    Die Abbildung zeigt das Fenster "Warengruppen". Links ist die Baumstruktur der Warengruppen (A) sichtbar. Rechts sind die Felder für die Eingabe einer neuen Warengruppe freigeschaltet, darunter die Nummer (B) und die Bezeichnung (C).

3.  Geben Sie die Nummer (B) und die Bezeichnung (C) der Warengruppe ein.
4.  Lassen Sie die Felder **Vorlauftage** und **Sonderzuschlag** frei. Sie können diese später füllen.
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die neue Warengruppe wird gespeichert.
6.  Markieren Sie ggf. ein Symbol (A), wenn die neue Warengruppe nicht das Bitmap der übergeordneten Warengruppe behalten soll.
7.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.

---
*A+W Business Stammdamten*
*B-213*
---

## Warengruppen kombinieren
Beim Anlegen von Kombi-Warengruppen können Platzhalter für die Nummernvergabe verwendet werden. Lesen Sie die Beispiele für die Kombi-Regeln gut durch, bevor Sie eine Kombi-Warengruppe angelegen.
⇨ "Regeln für Kombi-WGR" auf Seite B-206

> **Reihenfolge beim Anlegen von Kombi-WGR**
> Jede Kombination von Warengruppen ergibt eine sogenannte Kombi-WGR. Diese wird jedoch nicht automatisch durch die Kombination erzeugt, sondern muss zuvor angelegt werden. Legen Sie also zunächst die Warengruppen an, die durch Kombi-WGR entstehen können. Nur dann können Sie in den folgenden Handlungsschritten die Kombi-WGR auswählen.

### So kombinieren Sie Warengruppen
1.  Wählen Sie im Menü **Stammdaten > Produkte > Allgemein > Kombi-WGR**.
    Der Dialog **Kombi-WGR** wird geöffnet.
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.

---
*B-214*
*A+W Business Stammdaten*
---

**Abb. B-81: Felder für neue Kombi-WGR freigeschaltet**
Die Abbildung zeigt das Dialogfenster zur Erstellung von Kombi-Warengruppen.
- **A**: Auswahlfeld für WGR 1 (Hauptprodukt)
- **B**: Auswahlfeld für WGR 2 (Stücklisten-Komponente)
- **C**: Eingabefeld für die Nummer der neuen Kombi-WGR
- **D**: Checkboxen für die Anwendungseinstellungen (z.B. "gültig für Statistik")

Die freigeschalteten Felder sind mit den Werten der markierten Kombi-WGR vorbelegt.
⇨ Softwarereferenz, "Kombi-WGR" auf Seite B-682

3.  Wählen Sie Warengruppen 1 (A) und 2 (B) aus.
4.  Geben Sie die Nummer der Kombi-WGR (C) ein.
    Beachten Sie dabei die Regeln für die Platzhalter, sofern Sie diese verwenden wollen. Die Kombi-WGR wird nicht automatisch angelegt, wenn Sie eine neue Nummer eintragen. Sie müssen diese neue Kombi-WGR anschließend im Dialog WGR anlegen.
5.  Markieren Sie die gewünschten Checkboxen (D) für die Gültigkeit der Kombi-Warengruppe.
    Die Checkboxen für die Verarbeitung von Kombi-Rabatten werden freigeschaltet, wenn Sie die Checkboxen für die Gültigkeit markiert haben.
6.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.

---
*A+W Business Stammdaten*
*B-215*
---

> **Einstellungen für Kombi-WGR prüfen**
> Beachten Sie auch die Einstellungen für Kombi-Warengruppen in den Firmendaten.
>
> ⇨ Softwarereferenz, "WGR-Kombi für Rabatte nur gültig falls Rabatt vorhanden" auf Seite B-1087
> ⇨ Softwarereferenz, “WGR-Kombinationen mit kompletter Stückliste bilden" auf Seite B-1087

## Top-WGR anlegen und zuordnen
Für die Zuordnung einer Top-WGR führen Sie folgende Handlungen aus:
- Top-WGR anlegen.
- WGR zuordnen.

### So richten Sie eine Top-WGR für die Auswertung ein
1.  Wählen Sie im Menü **Stammdaten > Produkte > Allgemein > Top-WGR**.
    Der Dialog **Top-WGR** wird geöffnet.
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    Die nächste Zeile wird freigeschaltet.
3.  Tragen Sie die Bezeichnung ein.

    **Abb. B-82: Top-WGR anlegen**
    Die Abbildung zeigt den einfachen Dialog zum Anlegen einer Top-WGR mit Feldern für Nummer, Bezeichnung und Fremdschlüssel.

    ⇨ Softwarereferenz, "Top-WGR" auf Seite B-684
4.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.
5.  Schließen Sie den Dialog **Top-WGR**.
6.  Wechseln Sie zum Menü **Stammdaten > Produkte > Allgemein > WGR**.

---
*B-216*
*A+W Business Stammdaten*
---

Der Dialog **Warengruppen** wird geöffnet.
⇨ Softwarereferenz, "WGR" auf Seite B-680
7.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.

    **Abb. B-83: Top-WGR zuordnen**
    Die Abbildung zeigt das Fenster "Warengruppen".
    - **A Warengruppe**: Eine spezifische Warengruppe (z.B. "Wärme-ISO m. echten Sprossen") ist in der Baumansicht markiert.
    - **B Top-WGR**: Im rechten Detailbereich ist eine Checkbox für eine Top-Warengruppe (z.B. "TOP WGR 01 = Sprossen") aktiviert, um die Zuordnung vorzunehmen.

8.  Markieren Sie die WGR (A), die Sie der Top-WGR zuordnen wollen.
9.  Markieren Sie die Checkbox der Top-Warengruppe (B), die Sie zuordnen wollen.
10. Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.

---
*A+W Business Stammdaten*
*B-217*
---

## Übungen
- Legen Sie eine Warengruppe für die Schulung an.
- Legen Sie eine Kombi-WGR an, die für alle Bearbeitungen am VSG gilt. Beachten Sie dabei:
  - Sie müssen die Kombi-WGR als Warengruppe anlegen.
  - Sie müssen die Regel für die Kombi-WGR festlegen.

---
*B-218*
*A+W Business Stammdaten*
---

# iTOE
Mithilfe des iTOE-Moduls erfolgt eine Synchronisation der Bearbeitungen zwischen dem A+W CAD Designer (Shapes) und dem A+W Business.

Beim Import der DXF-Dateien aus dem A+W CAD Designer (Shapes) erfolgt eine sofortige Übernahme der Bearbeitungen in die Auftragserfassung. Der Vorteil der iTOE liegt darin, dass somit keine doppelten Eingaben der Bearbeitungen mehr nötig sind.

> **Voraussetzung**
> Das lizenzpflichtige iTOE-Modul setzt das Datenbanksystem Microsoft SQL Server 2016 voraus. Wenden Sie sich an die A+W Software GmbH, wenn Sie das Modul einsetzen wollen.

Zu Beginn sind nicht unbedingt Stammdaten erforderlich, da das Modul selbstlernend arbeitet. Die Stammdaten bestehen aus Regeln, mit denen festgelegt wird, welcher Artikel beim Abgleich in die Stückliste übertragen werden soll. Nach jedem Import werden die Artikel, die keiner Regel entsprechen, angezeigt und können dort während des Abgleichs angelegt und auch geändert werden.

## Regeln anlegen
Die Regeln können entweder zu Beginn in dem Dialog iTOE Regeln angelegt werden oder aber während des Imports definiert werden. Die Regeln werden in der Reihenfolge der vorgegebenen Priorität abgearbeitet.

---
*A+W Business Stammdaten*
*B-219*
---

## iTOE Regeln
Den Dialog zum Anlegen der Regeln erreichen Sie über:
**Stammdaten > Produkte > Artikel > iTOE-Regeln**

**Abb. B-84: iTOE Regeln**
Die Abbildung zeigt den Dialog "iTOE Regeln". Hier können Regeln für den Produktabgleich zwischen CAD und ERP definiert werden. Man kann Bearbeitungstypen, Prioritäten, Produktarten und diverse geometrische Parameter (Abstand, Länge, Tiefe, Radien) festlegen, um diese automatisch einem Produkt in A+W Business zuzuordnen.

Eine detaillierte Beschreibung zu den Feldern dieses Dialoges finden Sie unter:
⇨ Softwarereferenz, "iTOE Regeln" auf Seite B-778

## Produktabgleich
In der Bearbeitungserfassung kann der Produktabgleich entweder durch einen DXF-Datei Import oder durch die Schaltfläche [iTOE] in der Symbolleiste gestartet werden. Haben Sie die Änderungen an der Glas-Einheit im A+W CAD Designer (Shapes) durchgeführt, übernehmen Sie die geänderten Daten über den Menüpunkt **Datei > Speichern mit Datei** oder **Datei > Speichern ohne Datei**.

**Speichern mit Datei** bedeutet, dass eine SN-Datei (iTOE-Datei) in der Stückliste angelegt werden soll. Beim **Speichern ohne Datei** wird keine Datei angelegt.

Wird eine iTOE-Datei angelegt, fügt der Produktabgleich selbstständig einen Modellsatz ein (sollte dieser noch nicht vorhanden sein) und verknüpft die entstandene iTOE-Datei. Die iTOE-Dateien erkennen Sie am Dateinamen in der Form `XXXX_TOE.SN`. Wobei die vorangestellte Nummer aus den Nummernkreisen der SN-Dateien bestimmt wird.

Sobald die Änderungen übernommen wurden, zeigt A+W Business das Ergebnis der Regelprüfung in einem Dialog an.

---
*B-220*
*A+W Business Stammdaten*
---

**Abb. B-85: Ergebnis des Produktabgleichs**
Die Abbildung zeigt den "Produktabgleich"-Dialog. In einer Tabelle werden CAD-Bearbeitungen (z.B. Bohrungen, Innenausschnitte) mit ihren Eigenschaften aufgelistet. Für jede Bearbeitung wird das gefundene Produkt aus A+W Business gemäß den iTOE-Regeln angezeigt. Zeilen ohne gefundenes Produkt sind dunkel hinterlegt.

Ist für jede Bearbeitung ein Produkt gefunden worden, wird dies so wie im Beispiel oben angezeigt. Sollte für eine Bearbeitung keine Regel zutreffen, so ist dies an der dunkel hinterlegten Zeile zu erkennen und daran, dass die Artikelnummer (Feld Produkt) fehlt. Sie können jetzt über die Schaltfläche **[...]** im Feld **Regel bearbeiten/Regel einfügen** direkt in den Dialog **iTOE Regeln** wechseln und dort die passende Regel anlegen. Sie können auch bereits angelegte Regeln über diese Schaltfläche verändern. Nachdem der Dialog **iTOE Regeln** beendet wird, erfolgt immer ein neuer Abgleich und die gerade gemachten Änderungen am Regelwerk zeigen sofort ihre Auswirkungen.

Bestätigen Sie das Ergebnis des Produktabgleichs, wird in der Bearbeitungserfassung die komplette Stückliste erzeugt und mit den jeweiligen Preisen versehen. Änderungen, die jetzt in der Bearbeitungserfassung durchgeführt werden, gleicht das System mit der iTOE-Datei ab.

> **Eigenschaft von CAD-Bearbeitung**
> Änderungen von Eigenschaften, die nicht Bestandteil des A+W-Bearbeitungstypenkatalogs sind, gehen beim Abgleich verloren, z. B. eine Bohrloch-Reihe mit Serienvermaßung: Die Serienvermaßung wird gelöscht, sobald eine der beteiligten Bohrungen in der Bearbeitungserfassung geändert wird. Solche Änderungen müssen im A+W CAD Designer durchgeführt werden.

### Restriktionen und Konfiguration
Bei Bearbeitungen, die eine Kantenqualität haben (Bohrungen, Ausschnitte) ist beim DXF-Import immer die Kantenqualität im Import-Dialog zu definieren, die iTOE-Regel muss die Kantenqualität berücksichtigen und dann das Produkt auswählen, welches der Kantenqualität entspricht. Im A+W Business wird die Kantenqualität nicht im Auftrag gespeichert, sondern kommt immer aus dem Basisprodukt. Wird keine Qualität definiert, dann wird immer die der Stammdatenbearbeitung genutzt.

---
*A+W Business Stammdaten*
*B-221*
---

# Fertigung

## Lernziele
- Beschaffungsart zuweisen.
- Produktspezifische Standard-Einstellungen für die Produktion zuweisen.

## Nutzen
- Produkte werden mit produktionstechnischen Vorgaben in den Auftrag übernommen. Diese Angaben können im Dokument überschrieben werden.

## Merke

| Begriff | Erklärung |
| :--- | :--- |
| **Beschaffungsart** | Über dieses Kennzeichen erkennt A+W Business, wie eine Auftragsposition beschafft werden soll.<br>- Alle Produkte, die nicht fertig aus dem Lagerbestand entnommen werden können, müssen an die Produktion übergeben werden, damit sie angefertigt werden.<br>- Produkte, die nicht gefertigt und nicht aus dem Lager entnommen werden können, müssen bestellt werden. |
| **Maßzuschlag** | Ein Maßzuschlag gleicht den Materialverlust aus, der bei den unterschiedlichen Bearbeitungen entsteht. |
| **Maßabzug** | Ein Maßabzug wird gebraucht, wenn das Glas für einen Bilderrahmen zugeschnitten werden soll. |
| **Struktur** | Strukturen können einen Verlauf haben, der beim Zuschnitt berücksichtigt werden muss. Die möglichen Richtungen sind in einer Basistabelle hinterlegt und müssen den Ornamentgläsern zugewiesen werden. |
| **Ebenen für Struktur und Beschichtung** | Für die Produktion von ISO-Einheiten muss angegeben werden, wie ein Glas in die Einheit eingebaut werden soll. Bei einem 3-fach-ISO ergeben sich z. B. sechs Ebenen. Diese werden immer von außen nach innen gezählt. |
| **Sprossenkonstruktionen** | Sprossen können in Bezug auf die Felder oder auf die Bohrpunkte symmetrisch oder asymmetrisch erfasst werden. |
| **Sprossentypen** | Sprossen werden zu Typen zusammengefasst, die sich nach bestimmten Kriterien unterscheiden, z. B. welche Sprosse bei einem Kreuz durchgängig sein soll. |

---
*B-222*
*A+W Business Stammdaten*
---

## Vorgaben für die Fertigung
Abhängig von der Produktart und Produktgruppe sind unterschiedliche Angaben für die Übergabe an die Produktion erforderlich. Die entsprechenden Felder sind jeweils freigeschaltet.

**Abb. B-86: Produktverwaltung - Fertigung**
Die Abbildung zeigt das Register "Fertigung" in der Produktverwaltung. Wichtige Felder sind:
- **A Kantenqualität**: Auswahl der Kantenbearbeitung.
- **B Einstellungen für die Stückliste**: z.B. ob die Stückliste für die Fertigung relevant ist.
- **C Abweichende Mengen für Lagerartikel**: Einstellungen für Über-/Untermengen.
- **D Kennzeichen für Abstandhalter**: Definition von Verbundtyp, Rahmentyp etc.
- **E Skizzendruck bei Modellen oder Sprossen**: Steuerung des Drucks von Skizzen.
- **F Angaben zur Struktur und zur Beschichtung**: Definition von Verlauf und Beschichtungsseite.
- **G Maßzuschläge**: Eingabe von Zuschlägen für Breite und Höhe.

Bei einem komplexen Produkt kann die Stückliste mit an die Produktion (B) übergeben werden. Wenn das Produkt jedoch komplett eingekauft wird, ist die Stückliste nicht relevant für die Produktion. Bei einfachen (Glas-)Produkten muss angegeben werden, ob sie in der Stückliste verwendet werden dürfen. Wenn in einem Produkt Bearbeitungen der Kanten enthalten sind, muss die Kantenqualität (A) zugewiesen werden, damit in der Produktion die richtige Kantenbearbeitung ausgeführt wird.

Wenn im Produkt Sprossen oder Modellformen angegeben sind, kann der Druck einer Skizze (E) unterbunden werden. Der Skizzendruck ist ausführlich in einer separaten Einheit beschrieben.
⇨ Tutorial 2, "Skizzendruck" auf Seite B-552

---
*A+W Business Stammdaten*
*B-223*
---

## Maßzuschläge und -abzüge
Beim Zuschnitt muss in einigen Fällen ein Maßzu- oder Maßabschlag berücksichtigt werden.
- Ein **Maßzuschlag** gleicht den Materialverlust aus, der bei den unterschiedlichen Bearbeitungen entsteht.
- Ein **Maßabzug** wird gebraucht, wenn das Glas für einen Bilderrahmen zugeschnitten werden soll.

> **Beispiel**
> Durch Polieren aller vier Kanten reduziert sich ein Float von 1000 x 1000 mm auf die Maße 998 x 998 mm.
> Als Maßzuschlag müssen 2 mm zugegeben werden. Dieser Wert wird der zugeordneten Tabelle entnommen, wobei die Dicke des Glases berücksichtigt wird.

Die Maßzuschläge und -abzüge werden in Zugabe- oder Abzugstabellen zusammengefasst. Pro Tabellen können unterschiedliche Werte für den Zuschlag oder Abzug angegeben werden, der die jeweilige Dicke der Gläser berücksichtigt. Die Maßzuschläge werden den Produkten der Produktart Bearbeitung zugewiesen.

**Abb. B-87: Maßzugaben und Maßabzüge**
Die Abbildung zeigt:
- **A Zuschlagstabelle**: Ein Dialog zur Definition einer Maßzuschlagstabelle mit einer Nummer und Bezeichnung.
- **B Werte pro Glasdicke**: Eine Tabelle innerhalb des Dialogs, die den Zuschlagswert in Abhängigkeit von der Glasdicke ("bis Dicke") festlegt (z.B. für Dicke bis 4mm ein Wert von 1).
- **C Produkt Kanten-Bearbeitung**: Ein Ausschnitt aus der Produktverwaltung, wo dem Produkt "Kante(n) gesäumt" eine Maßzuschlagstabelle für Breite und Höhe zugewiesen wird.

---
*B-224*
*A+W Business Stammdaten*
---

## Strukturen und Beschichtungen
Für die Produktion müssen Strukturen, Verläufe, Beschichtungsarten und -ebenen angegeben werden. Diese können sowohl in der Produktverwaltung als auch im Auftrag ausgewählt werden.

### Strukturverlauf
Der Verlauf einer Struktur muss bei Ornamentgläsern für den Zuschnitt und den Einbau angegeben werden. Der Eintrag wird in der Produktverwaltung dem Glas zugewiesen.

**Abb. B-88: Strukturverlauf**
- **A**: Zeigt ein Ornamentglas mit senkrechtem Strukturverlauf.
- **B**: Zeigt ein Ornamentglas mit waagerechtem Strukturverlauf.

Der Verlauf kann folgende Werte annehmen:
- **Kein:**
  Dies gilt für alle Floatgläser.
- **Senkrecht, waagerecht:**
  Die Struktur verläuft senkrecht (A) bzw. waagerecht (B).
- **Beliebig:**
  Ornamentgläser, bei denen die Struktur keinen eindeutigen Verlauf hat, können in beiden Richtungen verwendet werden.

### Beschichtungsart
Beschichtungen werden in verschiedenen Härtegraden aufgebracht. Die Härte wird angegeben, damit beim Zuschnitt und bei Bearbeitungen die geeigneten Werkzeuge, z. B. Bohrer, eingesetzt werden. Die Bezeichnung kann frei gewählt werden, z. B. weich, hart, ohne.

---
*A+W Business Stammdaten*
*B-225*
---

## Ebenen für die Struktur- und Beschichtungsseite
Um genau angeben zu können, wie ein Glas in die ISO-Einheit eingebaut werden soll, definieren Sie die verschiedenen Ebenen innerhalb eines ISO-Aufbaus. Die Sichtweise ist dabei immer von außen (Ebene 1) nach innen (Ebene 2).

**Abb. B-89: Einbau-Ebenen für Struktur- und Beschichtungsseite**
Die Abbildung zeigt ein 4-fach-ISO-Glas mit 8 Ebenen, die von außen (1) nach innen (8) nummeriert sind. Die Sonne symbolisiert die Außenseite.

## Schnitte
Für den Zuschnitt müssen Sie außerdem festlegen, wie die Schnitte verlaufen sollen. Spielt der Strukturverlauf bei einem Auftrag keine Rolle, kann diese Angabe entfallen, um den Verschnitt möglichst gering zu halten.

**Abb. B-90: XYZ-Schnitte auf der Lagerplatte**
Die Abbildung zeigt eine Lagerplatte, auf der X-, Y- und Z-Schnitte dargestellt sind, um verschiedene Schnittorientierungen zu visualisieren.

---
*B-226*
*A+W Business Stammdaten*
---

## Sprossen
Sprossen können unterschiedlichen Typen angehören, z. B. glasteilende Sprossen, aufgesetzte Sprossen, Sprossen im Scheibenzwischenraum (SZR). In A+W Business werden in der Regel Sprossen für den SZR angelegt und nach Konstruktionstypen unterteilt.

Alle Sprossen, Verbindungsstücke und Randstopfen müssen als Produkt angelegt sein, damit sie im Auftrag erfasst werden können.

### Konstruktionstypen der Sprossen
Für die Bearbeitung von Scheiben mit mehreren Feldern wird neben den Randstopfen auch die Art der Verbindung der Sprossen angegeben. Die folgenden Konstruktionstypen sind standardmäßig hinterlegt:

| Icon | Beschreibung |
| :--- | :--- |
| 