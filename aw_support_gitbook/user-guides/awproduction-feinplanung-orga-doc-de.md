---
title: "DE_AWProduction_Feinplanung_3_3"
source: "DE_AWProduction_Feinplanung_3_3.pdf"
tags: ["A+W Production", "Feinplanung", "Orga", "Abstellplatz", "Produktionsreihenfolge", "Software-Tutorial", "Technical Manual", "Glass Production", "ERP", "MES"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a technical tutorial and software reference guide for the 'Orgas' (Organizations) module within the A+W Production Feinplanung (Fine Planning) software. It details the configuration of production sequences, storage locations, and organizational groups for optimizing glass manufacturing processes."
long_description: "This comprehensive document serves as both a tutorial and a software reference manual for the A+W Production Feinplanung (Fine Planning) system, focusing specifically on the configuration of 'Orgas' (Organizations). The document is divided into two main sections. The first section is a tutorial that provides practical, step-by-step guidance on setting up various organizational structures, such as 'A-Böcke Versand' (A-Racks for Shipping) and 'Fächerwagen' (Harp Racks). It explains key concepts including size classifications for glass panes, defining production sequences, grouping and sorting criteria, and managing number ranges for different storage types. This section includes illustrative screenshots of the software's user interface and practical exercises to guide the user. The second section is a detailed software reference that systematically describes all dialogs, fields, and settings available in the Feinplanung module. It covers the creation and management of Master-Orgas, Production Sequences, Check Sequences (Prüfreihenfolge), Storage Locations (Abstellplätze), and the rules for Grouping and Sorting. This reference part is intended for administrators and advanced users who need a deep understanding of the system's capabilities to configure and optimize production logistics, material flow, and resource utilization in a glass processing environment."
---

# Tutorial

---
## Orgas

### Einstellungen in A+W Production

Die nachfolgenden Dialoge zeigen Ihnen die entsprechenden Einstellungen in A+W Production für ISO-Kleine Einheiten.

**Einstellungen der Orga-Gruppe:**

*Abb. F-41: Einstellungen der Orga-Gruppe*

**Einstellungen Abstellplatz:**

*Abb. F-42: Einstellungen Abstellplatz*

> ### Ergänzende Informationen
>
> *   ⇨ Softwarereferenz, "Orga-Gruppen" auf Seite F-133
> *   ⇨ Softwarereferenz, “Einstellungen-Abstellplatz" auf Seite F-135

## A-Böcke Versand

Die Orga A-Böcke Versand liefert eine versandorientierte Produktionsreihenfolge, bei der vor der Linie im Wechsel von mehreren A-Böcken abgegriffen wird.

Die Einteilung der Abstellplatzgruppen basiert auf Größenklassen, innerhalb derer nach Kunde sortiert wird. Die Idee hierbei ist, eine Produktionsreihenfolge zu erreichen, die innerhalb gewisser Größenschwankungen global von groß nach klein läuft, wobei in jeder Größenklasse die Kundenaufträge zusammen gehalten und am Ende der Linie direkt auf Versandgestelle separiert werden.

Die Orga benötigt Abstellplätze vor und hinter der Linie und liefert eine verpackungsgerechte Produktionsreihenfolge. Hinter der Linie müssen Gestelle je Kunde bereitgestellt werden.

*   Es werden ausschließlich A-Böcke verwendet (Tiefe 200, Breite 2000).
*   Abstellmodus ist Glas.

### Größenklassen

Um Scheiben in Größenklassen einzuteilen, arbeitet diese Orga mit 2 Schwellwerten (im Diagramm S1 und S2).

*Abb. F-43: Größenklassen*

Da in der Orga immer zuerst die kleine Kante gesucht und geprüft wird, ist nur der Teil unterhalb der Diagonalen (im Diagramm) von Bedeutung. Die Größenklassen sind wie folgt definiert:

*   **Größenklasse 1:** kleine Kante > Gr_Schwelle_2
*   **Größenklasse 2:**
    *   kleine Kante > Gr_Schwelle_1 und
    *   große Kante ≤ Gr_Schwelle_2
*   **Größenklasse 3:**
    *   kleine Kante > Gr_Schwelle_1 und
    *   große Kante ≤ Gr_Schwelle_1
*   **Größenklasse 4:**
    *   kleine Kante < Gr_Schwelle_1 und
    *   große Kante > Gr_Schwelle_2
*   **Größenklasse 5:**
    *   Kleine Kante < Gr_Schwelle_1 und
    *   große Kante > Gr_Schwelle_1
*   **Größenklasse 6:**
    *   Kleine Kante < Gr_Schwelle_1 und
    *   große Kante < Gr_Schwelle_1

### Produktionsreihenfolge

Nach dieser Größenrasterung werden Abstellplatzgruppen definiert und die Produktionsreihenfolge nach dem Schema 1`2`3`4`5`6 gebildet, also von groß nach klein. Innerhalb dieser Größenklassen wie nachfolgend angegeben:

*   **ISO Größenklasse 1**
    *   Serie
    *   Normale ISO
    *   ISO-Besonderheiten (Stufe, Modell, 3-fach, Sprossen)
*   **ISO Größenklasse 2**
    *   Serie
    *   Normale ISO
    *   Stufen-ISO
    *   3-fach-ISO
    *   ISO-Modellscheiben
    *   ISO-Scheiben mit Sprossen
*   **ISO Größenklasse 3**
    *   Wie Größenklasse 2
*   **ISO Größenklasse 4**
    *   Wie Größenklasse 2
*   **ISO Größenklasse 5**
    *   Wie Größenklasse 2
*   **ISO Größenklasse 6**
    *   Serie
    *   Normale ISO
    *   ISO-Besonderheiten (Stufe, Modell, 3-fach, Sprossen)

Bei den größten und kleinsten Scheiben werden also alle Besonderheiten zusammengefasst.

### Gruppierung und Sortierung

Die Gruppierung an der Abstellplatzgruppe (Größenklasse) ist:
`Kunde + Artikel + SprossenKZ + Modell + Stufen`

Ein gegebener Kunde ist i.A. im Wechsel von den Gestellen einer Größenklasse abzunehmen. Die (Produkt-) Artikelnummer sorgt dafür, dass gleiche Glasaufbauten zusammenhängend in der Produktionsreihenfolge bleiben (i.d.R. gleicher Bock).

Ansonsten kommen Stufen vor Modellen, Modelle vor Sprossen. Serien stehen positionsweise separat, werden aber in Produktionsreihenfolge beigemischt. Alle anderen A-Böcke enthalten mehrere Kunden und Aufträge hintereinander.

### Nummernkreise

Die zu produzierenden Scheiben werden durch die Orga auf Abstellplätze verteilt. Folgende Abstellplätze und Nummernkreise sind dafür in der Orga hinterlegt:

**Tab. F-4: Nummernkreise der Produktionsorga A-Böcke Versand**

| Orgagruppe | Abstellplatz | Nummernkreis von | Nummernkreis bis |
| :--- | :--- | :--- | :--- |
| Auffänger | Auffänger | 10000 | 10999 |
| ESG - bearbeitet | bearbeitet-- große Scheiben | 8921 | 8950 |
| ESG - bearbeitet | bearbeitet- kleine Scheiben | 8901 | 8920 |
| ESG - bearbeitet | bearbeitet | 8501 | 8899 |
| ESG - bearbeitet | bearbeitet - Serien | 8951 | 8999 |
| ESG - gesäumt | gesäumt - große Scheiben | 8421 | 8450 |
| ESG - gesäumt | gesäumt | 8001 | 8399 |
| ESG - gesäumt | gesäumt - kleine Scheiben | 8401 | 8420 |
| ESG - gesäumt | gesäumt - Serien | 8451 | 8499 |
| Einfachglas | kleine Scheiben | 7901 | 7920 |
| Einfachglas | große Scheiben | 7921 | 7950 |
| Einfachglas | Einfach | 7501 | 7899 |
| Einfachglas | Serien | 7951 | 7999 |
| Einfachglas - geschliffen | geschliffen - kleine Scheiben | 7401 | 7420 |
| Einfachglas - geschliffen | Einfach - geschliffen | 7001 | 7399 |
| Einfachglas - geschliffen | geschliffen große Scheiben | 7421 | 7450 |
| Einfachglas - geschliffen | geschliffen - Serien | 7451 | 7499 |
| ISO Grkl 1 | ISO normal Grkl 1 | 1001 | 1499 |
| ISO Grkl 1 | ISO Besonderheiten Grkl 1 | 1801 | 1899 |
| ISO Grkl 1 | Iso Serie - Grkl 1 | 1951 | 1999 |
| ISO Grkl 2 | Iso Serie - Grkl 2 | 2951 | 2999 |
| ISO Grkl 2 | ISO normal Grkl 2 | 2001 | 2499 |
| ISO Grkl 2 | ISO Sprosse Grkl 2 | 2601 | 2699 |
| ISO Grkl 2 | ISO Modell Grkl 2 | 2501 | 2599 |
| ISO Grkl 2 | ISO 3-fach Grkl 2 | 2701 | 2799 |
| ISO Grkl 2 | ISO Stufe Grkl 2 | 2801 | 2899 |
| ISO Grkl 3 | ISO normal Grkl 3 | 3001 | 3499 |
| ISO Grkl 3 | ISO Stufe Grkl 3 | 3801 | 3899 |
| ISO Grkl 3 | ISO 3-fach Grkl 3 | 3701 | 3799 |
| ISO Grkl 3 | ISO Modell Grkl 3 | 3501 | 3599 |
| ISO Grkl 3 | Iso Serie - Grkl 3 | 3951 | 3999 |
| ISO Grkl 3 | ISO Sprosse Grkl 3 | 3601 | 3699 |
| ISO Grkl 4 | ISO Sprosse Grkl 4 | 4601 | 4699 |
| ISO Grkl 4 | ISO normal Grkl 4 | 4001 | 4499 |
| ISO Grkl 4 | ISO Stufe Grkl 4 | 4801 | 4899 |
| ISO Grkl 4 | ISO 3-fach Grkl 4 | 4701 | 4799 |
| ISO Grkl 4 | ISO Modell Grkl 4 | 4501 | 4599 |
| ISO Grkl 4 | Iso - Serie - Grkl 4 | 4951 | 4999 |
| ISO Grkl 5 | ISO normal Grkl 5 | 5001 | 5499 |
| ISO Grkl 5 | Iso Serie - Grkl 5 | 5951 | 5999 |
| ISO Grkl 5 | ISO 3-fach Grkl 5 | 5701 | 5799 |
| ISO Grkl 5 | ISO Modell Grkl 5 | 5501 | 5599 |
| ISO Grkl 5 | ISO Sprosse Grkl 5 | 5601 | 5699 |
| ISO Grkl 5 | ISO Stufe Grkl 5 | 5801 | 5899 |
| ISO Grkl 6 | Iso - Serie - Grkl 6 | 6951 | 6999 |
| ISO Grkl 6 | ISO normal Grkl 6 | 6001 | 6499 |
| ISO Grkl 6 | ISO Besonderheiten Grkl 6 | 6801 | 6899 |
| VSG | VSG | 9001 | 9899 |
| VSG | VSG - kleine Scheiben | 9901 | 9920 |
| VSG | VSG - große Scheiben | 9921 | 9950 |
| VSG | VSG - Serien | 9951 | 9990 |

Die Orga A-Böcke Versand optimiert direkt ausgerichtet auf Verpacken und Versand. Sie benötigen dadurch zwar mehr Gestelle am Linienende (pro Kunde / Auftrag) die Abstelllogik der Gläser ist aber einfacher.

### Einstellungen in A+W Production für ISO-Serie-Größenklasse 1

Die nachfolgenden Dialoge zeigen Ihnen die entsprechenden Einstellungen in A+W Production für ISO-Serie-Größenklasse 1.

**Einstellungen der Orga-Gruppe:**

*Abb. F-44: Einstellungen der Orga-Gruppe*

**Einstellungen Abstellplatz:**

*Abb. F-45: Einstellungen Abstellplatz*

> ### Ergänzende Informationen
>
> *   ⇨ Softwarereferenz, “Orga-Gruppen" auf Seite F-133
> *   ⇨ Softwarereferenz, "Einstellungen-Abstellplatz" auf Seite F-135

## Fächerwagen ohne Auffüllen

Die Orga Fächerwagen entspricht im Aufbau und der Abstellplatzvergabe weitgehend der Orga A-Böcke, es werden aber Fächerwagen für die Hauptabstellplätze genommen.

Dadurch wird meist ein erheblich besserer Verschnitt gewährleistet. Große und kleine Einheiten sowie Serien werden auf A-Böcke herausgezogen.

Ein wichtiger Unterschied zur Orga A-Böcke liegt darin, dass die Produktionsreihenfolge stets versandgerecht ist. Zwar wird mit der Orga Fächerwagen ebenfalls ein Bock nach dem anderen vor der Linie abgearbeitet, doch können auf Fächerwagen alle benötigten Glasarten zusammengestellt und auf Versandreihenfolge gebracht werden.

### Produktionsreihenfolge

Die verwendeten Abstellplatzgruppen sind (in Produktionsreihenfolge):

*   Normale ISO-Scheiben
*   ISO-Modellscheiben
*   ISO-Modellscheiben mit Sprossen
*   ISO-Scheiben mit Sprossen
*   Stufen-ISO
*   3-fach ISO

Um eine teilweise Direktverpackung zu ermöglichen, sind die Abstellplatzgruppen jeweils von groß nach klein unterteilt (in Produktionsreihenfolge):

*   **Serien:** A-Bock, (Serienflag gesetzt oder Stück ≥10)
*   **Große Einheiten:** A-Bock, Bedingung große Einheit, Voreinstellung:
    *   große Kante > 2100 oder
    *   kleine Kante > 1600)
*   **Normale Einheiten:** Fächerwagen
*   **Kleine Einheiten:** A-Bock, Bedingung kleine Einheit, Voreinstellung:
    *   kleine Kante < 300 oder
    *   große Kante < 500)

### Gruppierung und Sortierung

Die Fächerwagen haben 60 einzeln nummerierte Fächer. Die Sortierung auf den Fächerwagen ist `Kunde+Auftrag+Position`, während die A-Böcke nach `Kunde+Auftrag` gruppiert sind.

Die zu einem Produktaufbau gehörigen Scheiben werden nebeneinander in die Fächerwagen gesetzt. Handzuschnitte und Zukaufsgläser müssen zusortiert werden.

In jeder der Abstellplatzgruppen (in Produktionsreihenfolge) können am Ende schwach belegte Fächerwagen mit nur wenigen Scheiben auftreten. Beispielsweise ergibt sich in der Abstellplatzgruppe Modellsprossen ein Wagen mit nur zwei Einheiten, wenn der Produktionslauf nicht mehr an Modellsprossen enthält. Dieser Effekt wird in der Orga Aufgefüllte Fächerwagen vermieden.

### Optimierung

Wenn in einem Optimierungslauf nur Scheiben für Fächerwagen enthalten sind, erfolgt die Optimierung als freie Optimierung (XOPT). Sobald A-Bock-Scheiben in der Optimierung enthalten sind, erfolgt die Optimierung als Sequenz-Optimierung. Dabei werden aber die Scheiben auf Fächerwagen ohne jegliche Restriktion optimiert, das entspricht in der Wirkung einer freien Optimierung.

> **Fächerwagen nicht aufgefüllt!**
>
> Bei dieser Organisation ist wichtig, dass Fächerwagen nicht aufgefüllt werden.
>
> D. h. ein Fächerwagen wird nicht optimal ausgenutzt. Es kann passieren, dass einige Fächer frei bleiben, da die Positionen nicht gesplittet werden. Passt eine Auftragsposition nicht mehr in die restlichen Fächer des Fächerwagens, wird eine neue Fächerwagennummer vergeben!
>
> Die Sortierung auf dem Fächerwagen wird vorab durch die Gruppierung (bzw. Sortierung), welche an der Abstellplatzorganisation hängt, bestimmt.

### Nummernkreise

Die zu produzierenden Scheiben werden durch die Orga auf Abstellplätze verteilt. Folgende Abstellplätze und Nummernkreise sind dafür in der Orga hinterlegt:

**Tab. F-5: Nummernkreise der Produktionsorga Fächerwagen ohne Auffüllen**

| Orgagruppe | Abstellplatz | Nummernkreis von | Nummernkreis bis |
| :--- | :--- | :--- | :--- |
| Auffänger | Auffänger | 10000 | 10999 |
| ESG - bearbeitet | bearbeitet - große Scheiben | 8921 | 8950 |
| ESG - bearbeitet | bearbeitet - kleine Scheiben | 8901 | 8920 |
| ESG - bearbeitet | bearbeitet | 8500 | 8899 |
| ESG - bearbeitet | bearbeitet - Serien | 8951 | 8999 |
| ESG - gesäumt | gesäumt - Serien | 8451 | 8499 |
| ESG - gesäumt | gesäumt - große Scheiben | 8421 | 8450 |
| ESG - gesäumt | gesäumt - kleine Scheiben | 8401 | 8420 |
| ESG - gesäumt | Gesäumt | 8000 | 8399 |
| Einfachglas | Serien | 7951 | 7999 |
| Einfachglas | kleine Scheiben | 7901 | 7920 |
| Einfachglas | Einfach | 7500 | 7899 |
| Einfachglas | große Scheiben | 7921 | 7950 |
| Einfachglas - geschliffen | geschliffen - große Scheiben | 7421 | 7450 |
| Einfachglas - geschliffen | geschliffen - kleine Scheiben | 7401 | 7420 |
| Einfachglas - geschliffen | Einfach - geschliffen | 7000 | 7399 |
| Einfachglas - geschliffen | geschliffen - Serien | 7451 | 7499 |
| Iso | Iso | 100 | 1899 |
| Iso | Iso - kleine Einheiten | 1901 | 1920 |
| Iso | Iso - große Einheiten | 1921 | 1950 |
| Iso | Iso - Serien | 1951 | 1999 |
| Iso - Dreifach | Iso - Dreifach | 6000 | 6899 |
| Iso - Dreifach | Iso - Dreifach - große Einheiten | 6921 | 6950 |
| Iso - Dreifach | Iso - Dreifach - Serien | 6951 | 6999 |
| Iso - Dreifach | Iso - Dreifach - kleine Einheiten | 6901 | 6920 |
| Iso - Modelle | Iso - Modelle - kleine Einheiten | 2901 | 2920 |
| Iso - Modelle | Iso - Modelle | 2000 | 2899 |
| Iso - Modelle | Iso - Modelle - große Einheiten | 2921 | 2940 |
| Iso - Modelle | Iso - Modelle - Serien | 2951 | 2999 |
| Iso - Modelle | Iso - Modelle - nicht versiegelt | 2941 | 2950 |
| Iso - Modelle - Sprossen | Iso - Modelle - Sprossen - groß | 3921 | 3950 |
| Iso - Modelle - Sprossen | Iso - Modelle - Sprossen | 3000 | 3899 |
| Iso - Modelle - Sprossen | Iso - Modelle - Sprossen - klein | 3901 | 3920 |
| Iso - Modelle - Sprossen | Iso - Modelle - Sprossen - Serien | 3951 | 3999 |
| Iso - Sprossen | Iso - Sprossen - Serien | 4951 | 4999 |
| Iso - Sprossen | Iso - Sprossen - große Einheiten | 4921 | 4950 |
| Iso - Sprossen | Iso - Sprossen - kleine Einheiten | 4901 | 4920 |
| Iso - Sprossen | Iso - Sprosse | 4000 | 4899 |
| Iso - Stufe | Iso - Stufe - kleine Einheiten | 5901 | 5920 |
| Iso - Stufe | Iso - Stufe - große Einheiten | 5921 | 5950 |
| Iso - Stufe | Iso - Stufe - Serien | 5951 | 5999 |
| Iso - Stufe | Iso - Stufe | 5000 | 5899 |
| VSG | VSG - Serien | 9951 | 9990 |
| VSG | VSG - große Scheiben | 9921 | 9950 |
| VSG | VSG - kleine Scheiben | 9901 | 9920 |
| VSG | VSG | 9000 | 9899 |

Die Orga Fächerwagen optimiert versandorientiert und entspricht im Aufbau und der Abstellplatzvergabe weitgehend der Orga A-Böcke, es werden aber Fächerwagen für die Hauptabstellplätze verwendet.

### Einstellungen in A+W Production für ISO Modelle

Die nachfolgenden Dialoge zeigen Ihnen die entsprechenden Einstellungen in A+W Production für ISO Modelle.

**Einstellungen der Orga-Gruppe:**

*Abb. F-46: Einstellungen der Orga-Gruppe*

**Einstellungen Abstellplatz:**

*Abb. F-47: Einstellungen Abstellplatz*

> ### Ergänzende Informationen
>
> *   ⇨ Softwarereferenz, "Orga-Gruppen" auf Seite F-133
> *   ⇨ Softwarereferenz, “Einstellungen-Abstellplatz" auf Seite F-135

## Aufgefüllte Fächerwagen

Die Orga Aufgefüllte Fächerwagen vermeidet schwach gefüllte Fächerwagen und zieht alle Fächerwagen in Produktionsreihenfolge zusammen. Zuerst werden alle Fächerwagen abgearbeitet, anschließend kommen die Spezialitäten auf A-Böcke.

### Produktionsreihenfolge

Die Abstellplatzgruppen in Produktionsreihenfolge sind:

**Tab. F-6: Produktionsreihenfolge**

| Beschreibung | Abstellplatz-Typ |
| :--- | :--- |
| Normale ISO (nach Produkttyp sortiert) | Fächerwagen |
| ISO groß, klein, Serie | A-Böcke |
| ISO Modelle groß, klein, Serie | A-Böcke |
| ISO Modellsprossen groß, klein, Serie | A-Böcke |
| ISO Sprossen groß, klein, Serie | A-Böcke |
| ISO Stufen groß, klein, Serie | A-Böcke |
| ISO 3-fach groß, klein, Serie | A-Böcke |

Bis auf frei gehaltene Fächer zum Zusortieren von Zukaufsgläsern und Handzuschnitten, werden die Fächerwägen lückenlos gefüllt und enthalten alle Scheiben normaler Größe - also auch Sprossen, Modelle usw.

Große und kleine Einheiten sowie Serien sind herausgezogen und werden am Ende produziert.

### Gruppierung und Sortierung

Serien stehen positionsweise getrennt. Alle anderen A-Böcke enthalten eine Gruppierung nach `Kunde+Auftrag`, mit mehreren Aufträgen je Bock, und sind in der Positionsreihenfolge frei.

Die Orga enthält eine interne Gruppierung nach Produkteigenschaften. Die Belegungsreihenfolge der Fächerwagen und somit die Produktionsreihenfolge kann aber durch Vorgabe einer globalen Gruppierung und Sortierung übersteuert werden.

*   Gruppierung = Keine
*   Sortierung = Keine

Mit dieser globalen Einstellung erfolgt die Belegung der Fächerwagen gruppiert nach folgenden Produkteigenschaften:

Modelle, Modellsprossen, Sprossen, Stufen, 3-fach Aufbauten und normale ISO.

Diese werden jeweils zusammenhängend abgestellt und produziert.

Mit der folgenden Einstellung werden Kundenaufträge - unabhängig von Produkteigenschaften - zusammen gehalten:

*   Gruppierung = Kunde+Auftrag
*   Sortierung = Keine

Dabei wechseln Modelle, Sprossen, 3-fach entsprechend des Auftragsmixes ab; innerhalb eines Auftrags ist nach Produkteigenschaften gruppiert.

Die Fächerwagen haben 60 einzeln nummerierte Fächer.

Abstellmodus ist Einheit - die zu einem Produktaufbau gehörigen Scheiben werden nebeneinander in die Fächerwagen gestellt. Handzuschnitte und Zukaufsgläser müssen zusortiert werden.

### Optimierung

Diese Organisation basiert i.A. auch auf Sequenz - siehe Organisation Fächerwagen ohne Auffüllen - jedoch wird hier aufgefüllt, d. h. die Fächerwagen werden komplett gefüllt, auch wenn eine Auftragsposition gesplittet wird.

### Nummernkreise

Die zu produzierenden Scheiben werden durch die Orga auf Abstellplätze verteilt. Folgende Abstellplätze und Nummernkreise sind dafür in der Orga hinterlegt:

**Tab. F-7: Nummernkreise der Produktionsorga Aufgefüllte Fächerwagen**

| Orgagruppe | Abstellplatz | Nummernkreis von | Nummernkreis bis |
| :--- | :--- | :--- | :--- |
| Auffänger | Auffänger | 10000 | 10999 |
| ESG - bearbeitet | bearbeitet - Serien | 8951 | 8999 |
| ESG - bearbeitet | bearbeitet - große Scheiben | 8921 | 8950 |
| ESG - bearbeitet | bearbeitet - kleine Scheiben | 8901 | 8920 |
| ESG - bearbeitet | bearbeitet | 8500 | 8899 |
| ESG - gesäumt | gesäumt - große Scheiben | 8421 | 8450 |
| ESG - gesäumt | gesäumt - kleine Scheiben | 8401 | 8420 |
| ESG - gesäumt | gesäumt | 8000 | 8399 |
| ESG - gesäumt | gesäumt - Serien | 8451 | 8499 |
| Einfachglas | Einfach | 7500 | 7899 |
| Einfachglas | Serien | 7951 | 7999 |
| Einfachglas | große Scheiben | 7921 | 7950 |
| Einfachglas | kleine Scheiben | 7901 | 7920 |
| Einfachglas - geschliffen | geschliffen - Serien | 7451 | 7499 |
| Einfachglas - geschliffen | geschliffen - große Scheiben | 7421 | 7450 |
| Einfachglas - geschliffen | geschliffen - kleine Scheiben | 7401 | 7420 |
| Einfachglas - geschliffen | Einfach - geschliffen | 7000 | 7399 |
| Fächerwage aufgefüllt | Fächerwagen alles | 11000 | 50999 |
| Iso | Iso - kleine Einheiten | 1901 | 1920 |
| Iso | Iso - Serien | 1951 | 1999 |
| Iso | Iso - große Einheiten | 1921 | 1950 |
| Iso - Dreifach | Iso - Dreifach - kleine Einheiten | 6901 | 6920 |
| Iso - Dreifach | Iso - Dreifach - große Einheit | 6921 | 6950 |
| Iso - Dreifach | Iso - Dreifach - Serien | 6951 | 6999 |
| Iso - Modelle | Iso - Modelle - große Einheiten | 2921 | 2940 |
| Iso - Modelle | Iso - Modelle - kleine Einheiten | 2901 | 2920 |
| Iso - Modelle | Iso - Modelle - Serien | 2951 | 2999 |
| Iso - Modelle | Iso - Modelle - nicht versiege | 2941 | 2950 |
| Iso - Modelle - Sprossen | Iso - Modelle - Sprossen - groß | 3921 | 3950 |
| Iso - Modelle - Sprossen | Iso - Modelle - Sprossen - Serien | 3951 | 3999 |
| Iso - Modelle - Sprossen | Iso - Modelle - Sprossen - klein | 3901 | 3920 |
| Iso - Sprossen | Iso - Sprossen - kleine Einheiten | 4901 | 4920 |
| Iso - Sprossen | Iso - Sprossen - Serien | 4951 | 4999 |
| Iso - Sprossen | Iso - Sprossen - große Einheiten | 4921 | 4950 |
| Iso - Stufe | Iso - Stufe - Serien | 5951 | 5999 |
| Iso - Stufe | Iso - Stufe - kleine Einheiten | 5901 | 5920 |
| Iso - Stufe | Iso - Stufe - große Einheiten | 5921 | 5950 |
| VSG | VSG - große Scheiben | 9921 | 9950 |
| VSG | VSG - Serien | 9951 | 9990 |
| VSG | VSG | 9000 | 9899 |
| VSG | VSG- kleine Scheiben | 9901 | 9920 |

Die Orga Aufgefüllte Fächerwagen optimiert die Gläser produktionsorientiert nach Produkteigenschaften auf Fächerwagen und A-Böcke. Sie benötigen zwar mehr Gestelle, haben aber eine bessere Versandausrichtung der Produktion, da die Gläser nach Kunde und Auftragsnummer gruppiert werden.

### Einstellungen in A+W Production für ISO Dreifach Große Einheiten

Die nachfolgenden Dialoge zeigen Ihnen die entsprechenden Einstellungen in A+W Production für ISO Dreifach Große Einheiten.

**Einstellungen der Orga-Gruppe:**

*Abb. F-48: Einstellungen der Orga-Gruppe*

**Einstellungen Abstellplatz:**

*Abb. F-49: Einstellungen Abstellplatz*

> ### Ergänzende Informationen
>
> *   ⇨ Softwarereferenz, “Orga-Gruppen" auf Seite F-133
> *   ⇨ Softwarereferenz, “Einstellungen-Abstellplatz" auf Seite F-135

## Demos und Übungen

In diesem Abschnitt erfahren Sie, wie Sie eine Orga in der A+W Production anlegen.

### Trainerdemo: Stammdaten erläutern

Es werden die Stammdaten der A+W Production gezeigt und erläutert. Folgender Dialog wird unter diesem Aspekt erklärt:

*   Dialog Orga, mit den Registern
    *   Master-Orga
    *   Produktionsreihenfolge
    *   Prüfreihenfolge

### Übung 1: Eine Master-Orga anlegen

Erstellen Sie eine Master-Orga gemäß den unten aufgeführten Spezifikationen.

**Aufgabenstellung**
Erfassen Sie einen Testauftrag und lasten Sie diesen gemeinsam mit dem Trainer ein, um die Auswirkungen zu sehen. Der Testauftrag hat folgende Rahmenbedingungen zu erfüllen:

*   Name der Orga: `Neue Trainings-Orga`.
*   Fertigungsgruppen: Nach `Kundennummer+Auftragsnummer`
*   Name der Orga-Form: `Neue Training`
*   Typ der Orga-Form: Standard
*   Abstellmodus: Einheit
*   Name der Orga-Gruppe: `Auffang-Abstellplatz`
*   Einstellungen Abstellplatz: A-Bock, Supergruppenbildung: `+Kundennummer+Auftragsnummer`, keine Sortierung in den Gruppen, vollständige Gruppen werden gemeinsam abgestellt, Optimierungsverhalten 5.1, Abstellmodus Einheit.

**Übung 1: Lösung**
Die einzelnen Schritte dieser Aufgabe werden in folgenden Dialogen vorgenommen:

*   Dialog Orga
*   Dialog Master-Orga
*   Dialog Einstellungen - Abstellplatz

#### Master-Orga anlegen

1.  Öffnen Sie den Dialog Orga über das Menü `Stammdaten > Feinplanung`.
2.  Betätigen Sie die Schaltfläche `[Neu]`. Es öffnet sich der Dialog Master-Orga.
3.  Geben Sie im Feld Name der Master-Orga `Neue Trainings-Orga` ein.
4.  Öffnen Sie die Kombobox `Fertigungsgruppen` und wählen Sie `+Kundennummer-Auftragsnummer` aus.
5.  Betätigen Sie die Schaltfläche `[OK]`. Der Dialog wird geschlossen und Sie befinden sich wieder im Dialog Orga.
6.  Die neue Orga steht jetzt in der Übersicht.

#### Produktionsreihenfolge anlegen

1.  Öffnen Sie das Register Produktionsreihenfolge.
2.  Betätigen Sie die Schaltfläche `[Neu]`. Es wird der Eintrag `unknon/Standard` hinzugefügt.
3.  Betätigen Sie die Schaltfläche `[Einstellungen]`. Es öffnet sich der Dialog Orga.
4.  Geben Sie im Feld `Name der Orga-Form` `Neues Training` ein.
5.  Im Bereich `Abstellmodus` aktivieren Sie `Einheit`.
6.  Betätigen Sie die Schaltfläche `[OK]`. Der Dialog wird geschlossen und Sie befinden sich wieder im Register Produktionsreihenfolge.

#### Orga-Gruppe anlegen

1.  Markieren Sie die soeben angelegte Orga-Form `Neues Training` und betätigen Sie die Schaltfläche `[Neu]`. Es wird der Eintrag `noname` hinzugefügt.
2.  Betätigen Sie die Schaltfläche `[Einstellungen]`. Es öffnet sich der Dialog `Orga-Gruppen`.
3.  Geben Sie im Feld `Name` `Auffang Abstellplatz` ein.
4.  Im Bereich `Bildung der Gruppen` wählen Sie `Kundennummer`.
5.  Aktivieren Sie die Checkbox `Sortierung der Gruppen`.
6.  Betätigen Sie die Schaltfläche `[OK]`. Der Dialog wird geschlossen und Sie befinden sich wieder im Register Produktionsreihenfolge.

#### Abstellplatz anlegen

1.  Markieren Sie die soeben angelegte Orga-Gruppe `Auffang Abstellplatz` und betätigen Sie die Schaltfläche `[Neu]`. Es wird der Eintrag `unknown` hinzugefügt.
2.  Betätigen Sie die Schaltfläche `[Einstellungen]`. Es öffnet sich der Dialog `Einstellungen-Abstellplatz`.
3.  Geben Sie im Feld `Name` `A-Bock` ein.
4.  Im Bereich `Bildung der Gruppen` wählen Sie `+Kundennummer+Auftragsnummer`.
5.  Aus der Kombobox `Sortierung in den Gruppen` wählen Sie `Keine`.
6.  Im Bereich `Abstellmodus Gruppen` wählen Sie `vollständige Gruppen gemeinsam` und im Bereich `Optimierungsverhalten 5.1`.
7.  Aktivieren Sie die Checkbox `Auffang-Abstellplatz`.

> ### Ergänzende Informationen
>
> *   ⇨ Softwarereferenz, "Orga" auf Seite F-131
> *   ⇨ Softwarereferenz, “Orga-Gruppen" auf Seite F-133
> *   ⇨ Softwarereferenz, “Einstellungen-Abstellplatz" auf Seite F-135

# Softwarereferenz

## Übersicht

Menü `Stammdaten > Feinplanung` öffnen

Im Menü `Feinplanung` befinden sich folgende Programmpunkte:

*   **Voreinstellungen:**
    Diesen Menüpunkt benötigen Sie, wenn keine Einstellungen für Orga, Gruppierung und Sortierung in der Orga sowie Sortierung auf dem Abstellplatz vorgenommen wurden.
    *   ⇨ "Voreinstellungen" auf Seite F-139
*   **Orga:**
    Über diesen Menüpunkt richten Sie die Orgas ein. Sie definieren die Produktionsreihenfolge sowie die Prüfreihenfolge.
    *   ⇨ Softwarereferenz, "Register Master-Orga" auf Seite F-120
    *   ⇨ Softwarereferenz, "Register Produktionsreihenfolge" auf Seite F-122
    *   ⇨ Softwarereferenz, "Register Prüfreihenfolge" auf Seite F-124
*   **Gruppierung:**
    Über diesen Menüpunkt richten Sie Gruppierungen und Sortierungen ein.
    *   ⇨ Softwarereferenz, “Gruppierung/Sortierung - Dialog” auf Seite F-140
*   **Abstellplätze:**
    Mit diesem Menüpunkt richten Sie die Abstellplätze ein.
    *   ⇨ Softwarereferenz, "Abstellplätze" auf Seite F-146
*   **Bearbeitungen:**
    Mit diesem Menüpunkt können Sie neue Bearbeitungen anlegen oder existierende Bearbeitungen ändern.
*   **Lostypen**
    Über diesen Menüpunkt legen Sie Lostypen an und weisen Bearbeitungen zu.
    *   ⇨ Softwarereferenz, "Lostypen und Bearbeitungen" auf Seite F-151

> **Dialoge können von unterschiedlichen Stellen aus geöffnet werden**
> Bitte beachten Sie, dass Funktionen und Dialoge auf verschiedenen Wegen geöffnet werden können. In dieser Anleitung werden die entsprechenden Dialoge nur einmal beschrieben.
> Der Weg, wie einzelne Dialoge aufgerufen werden, ist bei den nachfolgenden Dialogbeschreibungen nochmals angegeben. Bestehen mehrere alternative Wege einen Dialog aufzurufen, so sind diese ebenfalls angegeben.

## Organisationen

**Stammdaten > Feinplanung > Orga**

In diesem Bereich erfassen bzw. ändern Sie Master-Orgas, Orgas und Orga-Gruppen. Darüber hinaus nehmen Einstellungen an der Produktionsreihenfolge sowie der Prüfreihenfolge vor. Detaillierte Informationen entnehmen Sie den Erläuterungen der einzelnen Register.

Der Dialog ist in folgende Register unterteilt:

*   "Register Master-Orga" auf Seite F-120
*   "Register Produktionsreihenfolge" auf Seite F-122
*   "Register Prüfreihenfolge" auf Seite F-124
*   "Voreinstellungen" auf Seite F-139

### Register Master-Orga

**Stammdaten > Feinplanung > Orga**

*Abb. F-46: Orga-Dialog, Register Master-Orga*

Im Register `Master-Orga` legen Sie neue Master-Orgas an oder nehmen Änderungen an bestehenden Master-Orgas vor. Die erstellten Master-Orgas weisen Sie dann später bei der Feinplanung einem Lauf zu. Im linken Fenster werden alle bereits definierten Master-Orgas in Baumstruktur dargestellt. Mit einem Klick auf das Pluszeichen, öffnen Sie die Master-Orga und sehen, welche Orga der Master-Orga zugeordnet ist. Im rechten Fenster sehen Sie alle definierten Orgas.

Die in dem rechten Fenster angezeigten Symbole haben folgende Bedeutung:

*Abb. F-47: Erläuterung der Symbole für Orgas*

| Symbol | Bedeutung |
| :--- | :--- |
| `S` (rot) | Standardorga / Verwendung |
| `S` (schwarz) | Standardorga / Produktion |
| `X` (blau) | Nicht-Standardorga / Produktion |
| `X` (schwarz) | Nicht-Standardorga / Verwendung |

#### Erläuterung der Schaltflächen

*   **Neu:** Betätigen Sie diese Schaltfläche, öffnet sich der Dialog Master-Orga, in dem Sie eine neue Master-Orga anlegen können. Zum Anlegen einer neuen Master-Orga, müssen Sie im linken Fenster den in der Baumstruktur an erster Stelle stehenden Eintrag `Master-Orga` markiert haben.
*   **Löschen:** Betätigen Sie diese Schaltfläche, wird die im linken Fenster markierte Master-Orga gelöscht. Haben Sie eine Orga markiert, wird die Orga gelöscht.
    > **Löschen ohne Sicherheitsabfrage**
    > Sollten Sie versehentlich etwas gelöscht haben, verlassen Sie den Orga-Dialog über die Schaltfläche `[Abbrechen]`. Wenn Sie ihn das nächste Mal öffnen, sind die Daten wieder vorhanden.
*   **Einstellungen:** Betätigen Sie diese Schaltfläche, öffnet sich der Dialog Master-Orga für die im linken Fenster ausgewählte Master-Orga.

> #### Weitere Informationen zum Register Master-Orga
>
> *   ⇨ Tutorial, "Master-Orga" auf Seite F-71
> *   ⇨ Überblick, "Schaltflächen" auf Seite A-78

### Register Produktionsreihenfolge

**Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge**

*Abb. F-48: Register Produktionsreihenfolge*

Das Register `Produktionsreihenfolge` zeigt Ihnen die Reihenfolge der Orga-Gruppen in der Orga.

#### Erläuterung der Schaltflächen

*   **Bedingung:** Diese Schaltfläche ist nur für Orga-Gruppen und Abstellplätze aktiv, da Sie nur für diese beiden Bedingungen definieren können. Betätigen Sie diese Schaltfläche, wenn Sie eine Orga-Gruppe markiert haben, öffnet sich der Dialog `Auswahl Bedingungen`. Sie definieren an dieser Stelle eine Bedingung für die Orga-Gruppe. Betätigen Sie diese Schaltfläche, wenn Sie einen Abstellplatz markiert haben, öffnet sich ebenfalls der Dialog `Auswahl Bedingungen`. Sie definieren an dieser Stelle eine Bedingung für den Abstellplatz. Die Bedingung für einen Abstellplatz wird optisch durch ein `?` angezeigt.
*   **Neu:** Betätigen Sie diese Schaltfläche, können Sie entweder eine neue Orga, eine neue Orga-Gruppe oder einen neuen Abstellplatz anlegen. Das hängt davon ab, welchen Eintrag Sie markiert haben. Haben Sie Orga markiert und betätigen Sie die Schaltfläche `[Neu]`, wird unterhalb der letzten Orga-Form eine neue Orga (z.B. `MZO ISO groß`) angehängt. Diese neue Orga erscheint zunächst mit dem Namen `unknown`. Markieren Sie dann diese neue angelegte Orga und betätigen Sie die Schaltfläche `[Einstellungen]`. Es öffnet sich der Dialog `Orga`, in dem Sie dann die entsprechenden Einstellungen zur Orga vornehmen können. Haben Sie eine Orga markiert und betätigen Sie die Schaltfläche `[Neu]`, wird innerhalb der markierten Orga an letzter Stelle eine neue Orga-Gruppe angehängt. Diese neue Orga-Gruppe erscheint zunächst mit dem Namen `noname`. Markieren Sie dann diese neue angelegte Orga-Gruppe und betätigen Sie die Schaltfläche `[Einstellungen]`. Es öffnet sich der Dialog `Orga-Gruppe`, in dem Sie dann die entsprechenden Einstellungen zur Orga-Gruppe vornehmen können. Haben Sie eine Orga-Gruppe markiert und betätigen Sie die Schaltfläche `[Neu]`, wird innerhalb der markierten Orga-Gruppe an letzter Stelle eine neuer Abstellplatz angehängt. Dieser neue Abstellplatz erscheint zunächst mit dem Namen `unknown`. Markieren Sie dann diesen neu angelegten Abstellplatz und betätigen Sie die Schaltfläche `[Einstellungen]`. Es öffnet sich der Dialog `Einstellungen - Abstellplatz`, in dem Sie dann die entsprechenden Einstellungen zu dem Abstellplatz vornehmen können.
*   **Ausschneiden:** Betätigen Sie diese Schaltfläche, wird der markierte Datensatz ausgeschnitten und in die Zwischenablage gelegt. Sie können ihn dann einer anderen Orga über die Schaltfläche `[Einfügen]` zufügen. Sollten Sie versehentlich einen falschen Datensatz ausgeschnitten haben, erfolgt beim Verlassen des Dialoges noch einmal eine Sicherheitsabfrage, ob die Änderungen ignoriert werden sollen. Beantworten Sie diese Abfrage mit `[Ja]`, ist der ausgeschnittene Datensatz beim nächsten Öffnen wieder vorhanden.
*   **Kopieren:** Betätigen Sie diese Schaltfläche, wird der markierte Datensatz in die Zwischenablage kopiert. Sie können ihn dann einer anderen Orga über die Schaltfläche `[Einfügen]` zufügen.
*   **Einfügen:** Betätigen Sie diese Schaltfläche, wird der kopierte oder ausgeschnittene Datensatz aus der Zwischenablage eingefügt.
*   **Löschen:** Betätigen Sie diese Schaltfläche, wird der markierte Datensatz gelöscht. Sollte der Datensatz, den Sie löschen möchten, noch von einem A+W Production-Prozess verwendet werden, erscheint eine entsprechende Sicherheitsabfrage. Sollten Sie versehentlich einen falschen Datensatz gelöscht haben, erfolgt beim Verlassen des Dialoges noch einmal eine Sicherheitsabfrage, ob die Änderungen ignoriert werden sollen. Beantworten Sie diese Abfrage mit `[Ja]`, ist der gelöschte Datensatz beim nächsten Öffnen wieder vorhanden.
*   **Einstellungen:** Betätigen Sie diese Schaltfläche, öffnet sich in Abhängigkeit des Eintrags, den Sie markiert haben, der entsprechende Dialog.
    *   Softwarereferenz, "Orga" auf Seite F-131
    *   Softwarereferenz, “Orga-Gruppen" auf Seite F-133
    *   Softwarereferenz, “Einstellungen-Abstellplatz" auf Seite F-135
    *   Formeleditor, "Auswahl Bedingungen" auf Seite F-44
*   **Export Orga:** Betätigen Sie diese Schaltfläche, wird die markierte Orga exportiert.

> #### Weitere Informationen zur Produktionsreihenfolge
>
> *   ⇨ Tutorial, "Produktionsreihenfolge" auf Seite F-81
> *   ⇨ Überblick, "Schaltflächen" auf Seite A-78

### Register Prüfreihenfolge

**Stammdaten > Feinplanung > Orga > Register Prüfreihenfolge**

*Abb. F-49: Orga Dialog, Register Prüfreihenfolge*

Dieser Dialog zeigt Ihnen die Prüfreihenfolge aller Abstellplätze einer Orga. Das bedeutet, hier wird festgelegt, in welcher Reihenfolge geprüft wird, ob eine Scheibe einem entsprechenden Abstellplatz zugewiesen wird (hinter den Namen der Abstellplätze stehen implizit die von Ihnen entsprechend zugewiesenen Bedingungen. Somit definieren Sie implizit die Reihenfolge, in der die Bedingungen abgefragt werden. Innerhalb eines Abstellplatzes sind alle zugewiesenen Bedingungen - maximal 7 pro Abstellplatz - UND-verknüpft).

Im rechten Fenster werden die Abstellplätze der im linken Fenster markierten Orga angezeigt. Ein `*` vor dem Namen kennzeichnet den Auffang-Abstellplatz der Orga (dieser sollte immer am Ende dieser Liste stehen). Um aus einem Abstellplatz einen Auffang-Abstellplatz zu machen, markieren Sie den gewünschten Abstellplatz durch einen Doppelklick. Bitte denken Sie daran, dass es für eine Orga immer nur einen Auffang-Abstellplatz geben kann. D.h. wenn es für eine Orga bereits einen Auffang-Abstellplatz gibt und Sie markieren einen anderen Abstellplatz durch einen Doppelklick, wird der zuerst vorhandene Abstellplatz wieder als normaler Abstellplatz (ohne `*`) gekennzeichnet.

Die Abstellplätze zeigen von oben nach unten die Reihenfolge an, nach der die Scheiben bestimmten Abstellplätzen zugewiesen werden. Eine Scheibe durchläuft, entsprechend der eingestellten Prüfreihenfolge, solange die Abstellplätze, bis sie auf einen Abstellplatz treffen, dessen Bedingungen sie erfüllt. Diesem wird sie dann zugewiesen. Die Spalten `Von` und `Bis` kennzeichnen den Nummernkreis der Abstellplätze. Sie können durch einen Klick in die entsprechende Spalte den Nummernkreis direkt in diesem Dialog editieren.

#### Erläuterung der Schaltflächen

*   **Anfang:** Betätigen Sie diese Schaltfläche, verschiebt sich die markierte Scheibe an den Anfang, d.h. an die erste Stelle.
*   **Hoch:** Betätigen Sie diese Schaltfläche, verschiebt sich die markierte Scheibe um eine Position nach oben.
*   **Runter:** Betätigen Sie diese Schaltfläche, verschiebt sich die markierte Scheibe um eine Position nach unten.
*   **Ende:** Betätigen Sie diese Schaltfläche, verschiebt sich die markierte Scheibe an das Ende, d.h. an die letzte Stelle.

> #### Weitere Informationen zur Prüfreihenfolge
>
> *   ⇨ Tutorial, "Prüfreihenfolge" auf Seite F-76
> *   ⇨ Überblick, "Schaltflächen" auf Seite A-78

## Master-Orga

**Pfade:**
*   `Stammdaten > Feinplanung > Orga > Register Master-Orga > [Neu]`
*   `Stammdaten > Feinplanung > Orga > Register Master-Orga > Master-Orga markieren > [Einstellungen]`

*Abb. F-50: Master-Orga erfassen*

Im Dialog Master-Orga können Sie entweder eine neue Master-Orga anlegen oder Einstellungen zu einer bestehenden Master-Orga ändern. Das Anlegen der Master-Orga gliedert sich in zwei Teile. Im ersten Schritt erfassen Sie die Master-Orga mit den entsprechenden Einstellungen und im zweiten Schritt legen Sie fest, aus welchen Orgas die Master-Orga bestehen soll. Weitere Erläuterungen finden Sie in den entsprechenden Feldern.

Technische Info: Datenbanktabelle: `FEIN_MASTERORGA`

### Erläuterung der Felder

*   **Name der Master-Orga:** In diesem Feld geben Sie den Namen für die Master-Orga ein. Der Name der Master-Orga wird in allen Anzeigen, die mit der Orga zu tun haben, verwendet und angezeigt.
    *   Technische Info: Pflichtfeld, Alphanumerisch, 32stellig, Datenbankfeld: `NAME`

*   **XOPT zusammen abstellen:** In der Feinplanung können aus den Optimierungen bestimmte Scheiben herausgeholt und mittels XOPT optimiert werden.
    *   `☑` XOPT - Optimierungen werden trotz verschiedener Glasart/-dicke gemeinsam in einem Stapel auf einem A-Bock abgestellt.
    *   `☐` Freie Optimierungen werden auf A-Böcken getrennt abgestellt.
    *   Technische Info: Datenbankfeld: `TOGETHER`

*   **Kombobox:** Die Checkbox steuert, um welchen Typ es sich bei der Master-Orga handelt:
    *   **Standard:** Es wird die normale Master-Orga verwendet.
    *   **Schnellorga:** Es wird eine Schnell-Orga durchlaufen, ohne dass die Anzeigen der Feinplanung erscheinen. Für Läufe, in denen Zuschnitt enthalten ist und die eine als Schnell-Orga gekennzeichnete Master-Orga durchlaufen, wird der Zuschnitt stets als Handzuschnitt behandelt.
    *   **Phys. Gestellbelegung:** Das System erzeugt automatisch eine sinnvolle Belegung der physikalischen Gestelle unter Beachtung der dafür angelegten Regeln und Zwangsbedingungen (Gewicht, Größe, etc.). Hierzu wird im Rahmen der Feinplanung zusätzlich der Stack Optimizer gestartet.
    *   Technische Info: Datenbankfeld: `QUICKORGA`

*   **Pärchenbildung verboten:** Diese Checkbox kommt bei 3-fach Isolierglas zum Einsatz. Die Einheiten bestehen meist aus einer unbeschichteten und zwei beschichteten Scheiben, wobei die beschichteten Scheiben die 1. und 3. Scheibe sind. Die Schichten werden zum SZR eingebaut, so dass eine der beiden Scheiben vor der Linie gedreht werden müsste. Um diese Scheibe bereits im Zuschnitt gedreht auf den Bock zu stellen, soll die Feinplanung die Scheiben daher auf verschiedene Stapel abstellen. Damit die beiden Stapel identische, passende Reihenfolgen haben, muss in diesem Nummernkreis mit fester Reihenfolge optimiert werden.
    *   `☑` Die Bildung von Pärchen ist verboten.
    *   `☐` Die Bildung von Pärchen ist erlaubt.
    *   Technische Info: Datenbankfeld: `PAIRFORBIDDEN`

*   **Maximale Anzahl Abstellplätze in Optimierung:** In diesem Feld können Sie angeben, wie viele Stapel gleichzeitig von der Optimierung verwendet werden dürfen.

*   **Fertigungsgruppen:** Die Kombobox enthält alle in dem Register Gruppierungen des Dialogs Gruppierung/Sortierung angelegten Werte. Wenn Sie von den vorhandenen Gruppierungen in diesem Feld eine auswählen, werden innerhalb der Feinplanung Fertigungsgruppen entsprechend des ausgewählten Wertes gebildet (als Vorbelegung - das kann man später an den Einstellungen der Orga ändern und auch in der Feinplanung (Optimierung) selbst). Die ausgewählten Werte beziehen sich auf die Basisteile des Laufs.
    *   Technische Info: Datenbankfeld: `ID_GROUP`

*   **Pseudoserien:** Über die Pseudoserien haben Sie in der Feinplanung die Möglichkeit, Positionen mit gleichem Aufbau zu sogenannten Pseudoserien zusammen zu fassen. Die in der Kombobox enthaltenen Werte kommen aus dem Register Gruppierungen des Dialogs `Gruppierung/Sortierung`. Wählen Sie aus der Kombobox den Wert aus, der auf die Pseudoserien angewendet werden soll.
    Normaler Weise dürfen auf festen Abstellplätzen nur kurzzeitig einzelne Scheiben (einzelne Positionen, welche jeweils nur 1 Scheibe enthalten) zwischengelagert / abgestellt werden, um bspw. auf Nachläufer zu warten. Mittels der Pseudo-Serie kann man nun identische Positionen (Einzelscheiben) als Serie zusammenfassen und diese dürfen nun auch ausnahmsweise gemeinsam auf einen festen Abstellplatz abgestellt werden. Die Pseudo-Serie hat noch einen 2. Sinn: Eine Serie (Stückzahl >100, aber das definiert jeder Kunde anders) kann prozesstechnisch anders durch die Produktion laufen - andere Laufwege, andere Behandlung. Mittels der Pseudo-Serie kann ich einzelne Positionen als "Serie" markieren und diese als Serien behandeln (bekommen dann auch intern das Serien-Flag).
    *   Technische Info: Datenbankfeld: `ID_PSEUDOGROUP`

*   **Mindestmenge:** Das Feld bezieht sich auf das Feld `Pseudoserien` und gibt an, ab welcher Mindestmenge Pseudoserien erzeugt werden. Liegt der Wert darunter, wird keine Pseudoserie gebildet.
    *   Technische Info: Datenbankfeld: `PSEUDOSCHWELLE`

*   **Freigabe:** Bei der Freigabe des mit dieser Master-Orga feingeplanten Laufes wird das hier angezeigte Skript (`*.bas` / `*.bat`-Datei) verwendet. Betätigen Sie die Schaltfläche `[Freigabe]`, öffnet sich der Dialog `Auswahl Skript`. In diesem Dialog sind alle im Programm angelegten Skripte enthalten. Die Skripte werden im A+W Production-Verzeichnis in einem separaten Ordner abgelegt (Ordnername: Scripts).
    *   Technische Info: Datenbankfeld: `SKRIPT`

*   **Auffüller:** Dieses Feld dient dazu, Scheiben mit einer größeren Dicke als vom Kunden bestellt zu optimieren. Diese Scheiben dienen dann als sogenannte Füller. Voraussetzung dafür ist jedoch, dass die Scheiben auf jeden Fall in ein ISO eingebaut werden. Darüber hinaus muss das ISO die in diesem Feld stehende Bedingung erfüllen. Betätigen Sie die Schaltfläche `[Auffüller]`, öffnet sich der Formeleditor. Dort können Sie aus den definierten Formeln die gewünschte auswählen. Nachdem Sie den Dialog geschlossen haben, wird Ihnen der Name der Formel im Feld dahinter angezeigt.
    *   Technische Info: Datenbankfeld: `ID_FILLERCONDITION`

*   **Quasiteile:** Dieses Feld ermöglicht Ihnen die Abbildung von Quasiteilen. Quasiteile sind Teile, die ihre Losbildungs- und Abstellplatzinformationen von ihren Unterteilen übernehmen und nicht nur fest vom Lostyp der Teile und Bearbeitungen abhängig zu machen. Nun kann über eine Bedingung an der Master-Orga noch gezielter bestimmt werden, für welche Teile eines Lostyps dies erlaubt ist. Betätigen Sie die Schaltfläche `[Quasiteile]`, öffnet sich der Formeleditor. Dort können Sie aus den definierten Formeln die gewünschte auswählen. Nachdem Sie den Dialog geschlossen haben, wird Ihnen der Name der Formel im Feld dahinter angezeigt.
    *   Technische Info: Datenbankfeld: `ID_QUASICONDITION`

*   **Bereich unten:** Bei diesem Bereich handelt es sich um die Verwendung von Sonderteilen (Füller, Restblätter, Bruchscheiben und Eilscheiben). Sie müssen erst in der Liste das gewünschte Sonderteil markieren und können anschließend rechts daneben die entsprechenden Abstellplatz-Nummer vergeben.

*   **Verwende Füller:** Das Feld bezieht sich auf vorhandene Füllaufträge. Füllaufträge können von der Feinplanung nur dann verwendet werden, wenn in der ausgewählten Master-Orga diese Checkbox aktiviert ist.
    *   `☑` Die Füller werden im Zuschnitt auf beliebige Böcke gestellt, deren Nummernkreis durch `Start Füller` und `Ende Füller` gegeben ist. Dabei wird jeder Position genau eine Bocknummer zugewiesen.
    *   `☐` Es werden keine Füller verwendet.
    *   Technische Info: Datenbankfeld: `USEFUELLER`

*   **Start Füller:** Dieses Feld bezieht sich auf den Abstellplatz-Nummernkreis der verwendeten Füllaufträge. Sie geben hier die kleinste Abstellplatz-Nummer an, auf der Füllaufträge abgestellt werden können.
    *   Technische Info: Datenbankfeld: `FUELLERSTART`

*   **Ende Füller:** Dieses Feld bezieht sich auf den Abstellplatz-Nummernkreis der verwendeten Füllaufträge. Sie geben hier die höchste Abstellplatz-Nummer an, auf der Füllaufträge abgestellt werden können.
    *   Technische Info: Datenbankfeld: `FUELLERENDE`

*   **Verwende Restblätter:** Das Feld bezieht sich auf Scheiben, die auf aufgelösten Restblättern vorangegangener Feinplanungen lagen.
    *   `☑` Die ausgewählte Master-Orga verwendet Restblätter. Die Restscheiben werden im Zuschnitt auf beliebige Böcke gestellt, deren Nummernkreis durch `Start Restblatt` und `Ende Restblatt` gegeben ist. Dabei wird jeder Position genau eine Bocknummer zugewiesen.
    *   `☐` Es werden keine Restblätter verwendet.
    *   Technische Info: Datenbankfeld: `USERESTBLATT`

*   **Start Restblatt:** Dieses Feld bezieht sich auf den Abstellplatz-Nummernkreis der verwendeten Restblätter. Sie geben hier die kleinste Abstellplatz-Nummer an, auf der Restblätter abgestellt werden können.
    *   Technische Info: Datenbankfeld: `RESTBLATTSTART`

*   **Ende Restblatt:** Dieses Feld bezieht sich auf den Abstellplatz-Nummernkreis der verwendeten Restblätter. Sie geben hier die höchste Abstellplatz-Nummer an, auf der Restblätter abgestellt werden können.
    *   Technische Info: Datenbankfeld: `RESTBLATTENDE`

*   **Verwende Bruchscheiben:** Das Feld bezieht sich auf vorhandene Bruchscheiben.
    *   `☑` Die ausgewählte Master-Orga verwendet vorhandene Bruchscheiben. Die Bruchscheiben werden im Zuschnitt auf beliebige Böcke gestellt, deren Nummernkreis durch `Start Bruch` und `Ende Bruch` gegeben ist. Dabei wird jeder Position genau eine Bocknummer zugewiesen.
    *   `☐` Es werden keine Bruchscheiben verwendet.
    *   Technische Info: Datenbankfeld: `USEBRUCH`

*   **Start Bruch:** Dieses Feld bezieht sich auf den Abstellplatz-Nummernkreis der verwendeten Bruchscheiben. Sie geben hier die kleinste Abstellplatz-Nummer an, auf der Bruchscheiben abgestellt werden können.
    *   Technische Info: Datenbankfeld: `BRUCHSTART`

*   **Ende Bruch:** Dieses Feld bezieht sich auf den Abstellplatz-Nummernkreis der verwendeten Bruchscheiben. Sie geben hier die höchste Abstellplatz-Nummer an, auf der Bruchscheiben abgestellt werden können.
    *   Technische Info: Datenbankfeld: `BRUCHENDE`

*   **Verwende Eilscheiben:** Das Feld bezieht sich auf vorhandene Eilscheiben.
    *   `☑` Die ausgewählte Master-Orga verwendet vorhandene Eilscheiben.
    *   `☐` Es werden keine Eilscheiben verwendet.
    *   Technische Info: Datenbankfeld: `USEBRUCH`

> #### Weitere Informationen zur Master-Orga
>
> *   ⇨ Tutorial, "Master-Orga" auf Seite F-71
> *   ⇨ Tutorial, "Sonderteile" auf Seite F-30
> *   ⇨ Überblick, "Schaltflächen" auf Seite A-78

## Orga

**Pfad:** `Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Orga markieren > [Einstellungen]`

*Abb. F-51: Orga Einstellungen*

In diesem Dialog legen Sie neue Orgas an oder nehmen Änderungen an bestehenden Orgas vor. Weitere Erläuterungen finden Sie in den entsprechenden Feldern.

Technische Info: Datenbanktabelle: `FEIN_ORGA`

### Erläuterung der Felder

*   **Name der Orga-Form:** In diesem Feld geben Sie den Namen der Orga an.
    *   Technische Info: Datenbankfeld: `NAME`

*   **Typ:** In dieser Kombobox wählen Sie den Orga-Typ. Orga-Typen sind `Standard`, `Packmittel` und alle im System enthaltenen Lostypen mit Ausnahme des Zuschnitts. Um in diesem Feld einen Lostyp auswählen zu können, muss dieser bereits definiert sein! Die Definition nehmen Sie im Dialog `Lostypen` vor.
    *   Technische Info: Datenbankfeld: `LOSTYP`

*   **Produktion:** Die Checkbox steuert, ob es sich bei der Orga um eine Produktions- oder um eine Verwendungs-Orga handelt.
    *   `☑` Bei der Orga handelt es sich um eine Produktions-Orga
    *   `☐` Bei der Orga handelt es sich um eine Verwendungs-Orga.
    *   Technische Info: Datenbankfeld: `PRODUKTION`

*   **Abstellmodus:** Über die Optionen nehmen Sie die Voreinstellung des Abstellplatzmodus auf A-Böcken innerhalb der Orga vor. Die hier vorgenommenen Einstellungen können in der Orga jederzeit noch überschrieben werden. Der Standard-Wert für den Abstellmodus ist `Einheit`. Mögliche Werte:
    *   Glas
    *   Einheit
    *   Produktion
    *   VABGLA
    *   Technische Info: Datenbankfeld: `BELEGUNGSMODE`

*   **Kein Teilen von ... bei Bockbelegung von mehr als ... Prozent:** Mögliche Werte:
    *   **Gruppen:** Sollte eine Gruppe von Scheiben auf einen Abstellplatz gestellt werden, diese Gruppe aber wegen der Bocktiefe nicht mehr komplett auf den Abstellplatz passen, so wird die Gruppe nicht geteilt und ein Teil dort abgestellt, falls der Abstellplatz bereits zu mehr als X Prozent belegt ist, bevor begonnen wird, die Gruppe auf dem Abstellplatz abzustapeln.
        *   Technische Info: Datenbankfeld: `USETIEFE_GRUPPE`
    *   **Einheiten:** Sollte eine Gruppe geteilt auf einem Abstellplatz abgestellt werden, so kann diese Teilung genau innerhalb einer Einheit stattfinden. Auch hier wird das Teilen der Einheit verhindert, falls der Abstellplatz bereits zu mehr als X Prozent belegt ist. Damit eine Einheit gesplittet werden kann, muss auf jeden Fall die Gruppe gesplittet werden, daher sollte der Wert für die Gruppen stets größer als der für die Einheiten sein.
        *   Technische Info: Datenbankfeld: `USETIEFE_EINHEIT`

> #### Weitere Informationen zur Orga
>
> *   ⇨ Tutorial, "Orgas" auf Seite F-68
> *   ⇨ Überblick, "Schaltflächen" auf Seite A-78

## Orga-Gruppen

**Pfad:** `Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Orga-Gruppe > [Einstellungen]`

*Abb. F-52: Einstellungen Orga-Gruppen*

In diesem Dialog nehmen Sie die Einstellungen zu bereits vorhandenen oder aber auch neuen Orga-Gruppen vor. Das bedeutet, Sie vergeben oder ändern den Namen der Orga-Gruppe und weisen der Orga-Gruppe sogenannten Gruppierungen und/oder Sortierungen zu. Weitere Erläuterungen finden Sie in den entsprechenden Feldern.

Technische Info: Datenbanktabelle: `FEIN_ORGAGRUPPE`

### Erläuterung der Felder

*   **Name:** In diesem Feld geben Sie den Namen für die Orga-Gruppe ein.
    *   Technische Info: Datenbankfeld: `NAME`

*   **DynOpt Einstellung:** Diese Checkbox müssen Sie aktivieren, wenn die Orga-Gruppe für A+W DynOpt gedacht sind. D. h., Scheiben, die für A+W DynOpt gedacht sind, können nur in einer Orga-Gruppe landen, die dieses Kennzeichen trägt.
    *   Technische Info: Datenbankfeld: `DYNOPT`

*   **Bildung der Gruppen:** Das Feld steuert, ob für die jeweilige Orga-Gruppe, eine Gruppenbildung erfolgen soll. Die Kombobox enthält alle bereits definierten Gruppierungen, unter denen Sie die entsprechende auswählen können. Die Gruppierungen werden in den Stammdaten angelegt. Wählen Sie aus der Kombobox die entsprechende Gruppierung.
    *   Technische Info: Datenbankfeld: `GROUPINDEX`

*   **Sortierung der Gruppen:** Die Checkbox ist in Zusammenhang mit dem Feld `Bildung der Gruppen` zu sehen und steuert, ob eine Sortierung der dort gewählten Gruppe erfolgen soll.
    *   `☑` Es erfolgt eine Sortierung der Gruppen.
    *   `☐` Es erfolgt keine Sortierung der Gruppen.
    *   Technische Info: Datenbankfeld: `HASGSORT`

*   **Sortierung in den Gruppen:** Die Kombobox steuert, ob für die im Feld `Bildung der Gruppen` getroffene Auswahl eine Sortierung innerhalb der entsprechenden Gruppe stattfinden soll. Es gibt die folgenden Sortierungswerte:
    *   **Keine** = Es erfolgt keine Sortierung in den Gruppen.
    *   **Global** = Die Angaben aus den Voreinstellungen werden übernommen.
    *   **Selbst definierte Sortierungen.**
    *   Technische Info: Datenbankfeld: `SUBSORTINDEX`

> **Einstellungen bei Orga-Gruppen**
> Wenn Orga-Gruppen mit Gruppierung und Sortierung definiert wurden, muss für den Abstellplatz keine Gruppierung/Sortierung eingestellt werden, da dies von der Orga-Gruppe übernommen wird. Wenn für den Abstellplatz Einstellungen vorgenommen werden, überschreiben diese die Gruppierung/Sortierung der Orga.

> #### Weitere Informationen zu Orga-Gruppen
>
> *   ⇨ Tutorial, "Orgas" auf Seite F-68
> *   ⇨ Tutorial, "Produktionsreihenfolge" auf Seite F-81
> *   ⇨ Überblick, "Schaltflächen" auf Seite A-78

## Einstellungen-Abstellplatz

**Pfad:** `Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Einstellungen > Register [Verwendung]`

*Abb. F-53: Einstellungen - Abstellplatz*

In diesem Dialog nehmen Sie die Zuweisung von Namen und Nummernkreisen zu den Abstellplätzen vor. Es ist darauf zu achten, dass die Namen und Nummernkreise mit dem Abstellplatz-Typ (A-Bock, Fächerwagen, etc.) korrespondieren. Darüber hinaus werden die Gruppierungen und Sortierungen sowie die Abstellmodi zugewiesen.

Technische Info: Datenbanktabelle: `FEIN_BOCKTYP`

### Erläuterung der Felder

*   **Name:** In diesem Feld geben Sie den Namen für die Abstellplatz-Typ ein.
    *   Technische Info: Pflichtfeld, Alphanumerisch, 32stellig, Datenbankfeld: `NAME`

*   **Bildung der Gruppen:** Das Feld steuert, ob für den jeweilige Abstellplatz-Typ, eine Gruppenbildung erfolgen soll. Die Kombobox enthält alle bereits definierten Gruppierungen, unter denen Sie die entsprechende auswählen können. Die Gruppierungen werden in den Stammdaten angelegt. Wählen Sie aus der Kombobox die entsprechende Gruppierung.
    *   Technische Info: Datenbankfeld: `GROUPINDEX`

*   **Sortierung in den Gruppen:** Die Kombobox steuert, ob für die im Feld `Bildung der Gruppen` getroffene Auswahl eine Sortierung innerhalb der entsprechenden Gruppe stattfinden soll. Es gibt die folgenden Sortierungs-Werte:
    *   **Keine** = Es erfolgt keine Sortierung in den Gruppen.
    *   **Global** = Die Angaben aus den Voreinstellungen werden übernommen.
    *   **Selbst definierte Sortierungen.**
    *   Technische Info: Datenbankfeld: `SUBSORTINDEX`

*   **Invertierung überprüfen:** Bei Bearbeitungen, die über die Lostypen-Einstellung `Nicht verwenden`, `Nur Eigenschaften` oder `Verwende Unterteil` innerhalb der Feinplanung aus der Stückliste entfernt werden, kann über die dafür zuständige logische Maschine hinterlegt werden, ob durch diesen Bearbeitungsschritt die Reihenfolge auf A-Böcken invertiert werden muss. In den Nummernkreisen der Feinplanung kann dann eingestellt werden, ob das Kennzeichen der logischen Maschine verwendet werden soll. Ist dies der Fall und zwischen dem zu produzierenden Schritt und dem verwendeten Schritt befindet sich eine ungerade Anzahl an Bearbeitungen, die obiges Kennzeichen haben, so wird auf A-Böcken die Reihenfolge innerhalb der Stapel invertiert. Dazu werden Scheiben mit unterschiedlichen Invertierungsverhalten auf separate Stapel gestellt. Für den Zuschnitt bedeutet dies, dass auch die Brechreihenfolge entsprechend angepasst wird.
    *   Technische Info: Datenbankfeld: `INVERT_SEQUENCE`

*   **Abstellmodus Gruppen:** Das Feld wird nur dann ausgewertet, wenn der Optimierungs-Modus 6.1 oder 5.1 verwendet wird. Die Kombobox steuert in diesem Fall, wie Gruppen abgestellt werden. Wählen Sie aus der Kombobox den entsprechende Abstellmodus. Mögliche Werte:
    *   nur 1 Gruppe je Stapel.
    *   vollständige Gruppen gemeinsam.
    *   feste Reihenfolge.
    *   nur 1 aufgeteilte Gruppe je Stapel.
    *   alternierend.
    *   Technische Info: Datenbankfeld: `BELEGMODE`

*   **Optimierungsverhalten:** Die Kombobox ist in Zusammenhang mit dem Feld `Bildung der Gruppen` zu sehen. Bitte wählen Sie aus der Kombobox, wie Sie optimieren möchten. Mögliche Werte:
    *   Gruppen frei (6.1).
    *   Gruppen sortiert (6.2).
    *   Alles frei (5.1).

    > **Optimierungs-Modus verwenden**
    > Die Optimierungs-Modi 6.1 und 6.2 werden nur dann verwendet, wenn Auftrags-Nummer und Positions-Nummer im Gruppierungs- und Sortierungsschlüssel enthalten sind. Sind diese nicht enthalten, wird der Optimierungs-Modus 5.2 verwendet.

*   **Auffang-Abstellplatz:** Diese Checkbox steuert den Auffang-Abstellplatz. Als Auffang-Abstellplatz wird der Abstellplatz markiert, auf dem die Teile eines Laufes landen, die keinem anderen Abstellplatz zugewiesen werden konnten, da sie keine der für die anderen Abstellplätze definierten Bedingungen erfüllen.
    *   `☑` Bei dem Abstellplatz handelt es sich um den Auffang-Abstellplatz der Orga.
    *   `☐` Bei diesem Abstellplatz handelt es sich nicht um einen Auffang-Abstellplatz der Orga.
    *   Technische Info: Datenbankfeld: `AUFFAENGER`

*   **Von / Bis:** Für jeden Bocktyp wird mindestens ein Nummernkreis erfasst, der beschreibt, in welchem Bereich die Bocknummern für diesen Bocktyp liegen dürfen. Verwendungsbocktypen können darüber hinaus sogar zwei Nummernkreise haben, falls für diese auch ein Produktionsbock vergeben wird. Weder innerhalb einer Orga noch innerhalb einer Master-Orga darf es vorkommen, dass die darin enthaltenen Nummernkreise sich überlappen (das lässt das Programm auch nicht zu und wird Sie mit entsprechenden Fehlermeldungen darauf hinweisen). Für die Master-Orgas ist dabei zu beachten, dass diese noch zusätzlich Nummernkreise für diverse Spezialitäten (Bruch, Füller, Rest) beinhalten können.
    *   Technische Info: Datenbankfeld: `MINIMUM`
    *   Technische Info: Datenbankfeld: `MAXIMUM`

*   **Max. Anzahl Gruppen:** Dieses Feld bezieht sich auf die maximale Anzahl von Gruppen, die auf dem Abstellplatz stehen dürfen. Sollen beliebig viele Gruppen abgestellt werden können, so muss hier der Wert `0` eingetragen werden.
    *   Technische Info: Datenbankfeld: `MAXNUMBER`

*   **Nächsten Schritt trennen:** Ist die Checkbox aktiviert, wird bei A-Böcken auch auf die Losbildung des nächsten Schrittes geschaut, wenn überprüft wird, was zusammen abgestellt werden kann.

*   **Freie Optimierung (nur für A-Bock):** Mit dieser Checkbox können Sie für jeden Nummernkreis einstellen, ob alle A-Böcke dieses Nummernkreises die Freie Optimierung automatisch verwenden sollen.

*   **Abstellmodus:** Die in diesem Bereich aufgeführten Werte sind in Zusammenhang mit dem Feld `Abstellplatz-Typ` zu sehen. Wenn Sie im Feld `Abstellplatz-Typ` die Radiotaste `A-Bock` aktiviert haben, erscheinen die Werte:
    *   **Global:** Der in der Orga hinterlegte Modus wird verwendet.
    *   **Glas:** Jede Glasart erhält eine eigenen Nummer und wird auf einem eigenen Abstellplatz abgestellt.
    *   **Einheit:** Die jeweils zusammengehörigen Gläser einer Einheit (VSG, ISO) werden gemeinsam auf einem Abstellplatz mit einer gemeinsamen Abstellplatznummer abgestellt. Unterschiedliche Glasarten werden dabei automatisch vom System getrennt und in verschiedenen Stapeln nebeneinander abgestellt.
    *   **Produktion:** Mehrere Glasarten werden gemeinsam, in nach Glasart getrennten Stapeln, auf einem Abstellplatz abgestellt. Aus diesen verschiedenen Stapeln können verschiedene Produkte / Kombinationen gefertigt werden.
    *   **VABGLA:** Es gibt pro Glastyp einen logischen Abstellplatz mit jeweils einem Stapel. Der Unterschied zum Modus `Glas` ergibt sich bezüglich dem Splitten von Gruppen bei Erreichen der Maximalbeladung des Abstellplatzes. Genaueres entnehmen Sie bitte der Beschreibung der Modi im Tutorial.

    Wenn Sie im Feld Abstellplatz-Typen die Radiotaste `Fächerwagen` aktiviert haben, erscheinen die Werte:
    *   **Zusammen:** Scheibe und Gegenscheibe(n) werden immer zusammen auf einen Fächerwagen gestellt.
    *   **Glas:** Die Scheiben werden immer getrennt weggestellt.
    *   **Kompakt:** Es werden nur Scheiben auf einen Fächerwagen gestellt, die ein gemeinsames Kennzeichen haben. Dieses Kennzeichen kann, je nach Konfiguration, entweder das Feld `XOPT_TISCH.CUTGO` oder das Feld `POOL_TEILE.SONDERKZ3` sein.

    Wenn Sie im Feld Abstellplatz-Typen die Radiotaste `Feste Abstellplätze` aktiviert haben, ist der Bereich Abstellmodus nicht aktiv.
    *   Technische Info: Datenbankfeld: `BELEGMODE`

*   **Abstellplatz-Typ:** Die Optionen steuern, um welchen Abstellplatz-Typ es sich handelt. Mögliche Werte:
    *   A-Bock
    *   Fächerwagen
    *   Feste Abstellplätze
    Die darunter liegende Kombobox bezieht sich immer auf den aktivierten Abstellplatz-Typ. Sollte es z.B. bei einem A-Bock mehrere Ausführungen geben, können Sie auf diese dann in der Kombobox zugreifen.
    *   Technische Info: Datenbankfeld: `TYPE`

### Erläuterung der Schaltflächen

*   **Abstellplätze:** Wählen Sie diese Schaltfläche, um den Dialog `Abstellplätze` zu öffnen.

> #### Weitere Informationen zum Register Verwendung
>
> *   ⇨ Tutorial, "Abstellplätze" auf Seite F-38
> *   ⇨ Tutorial, “Gruppierungsschlüssel der Orga-Gruppen" auf Seite F-82
> *   ⇨ Überblick, "Schaltflächen" auf Seite A-78

## Voreinstellungen

**Pfad:** `Stammdaten > Feinplanung > Voreinstellung`

*Abb. F-54: Voreinstellungen*

Die hier vorhandenen Einstellungen werden immer dann verwendet, wenn keine Einstellungen für Orga, Gruppierung und Sortierung in der Orga sowie Sortierung auf dem Abstellplatz vorgenommen wurden. Es wird empfohlen, hier Einstellungen vorzunehmen, da sonst beim Starten der Feinplanung eine Fehlermeldung erscheint.

### Erläuterung der Felder

*   **Verarbeitungsreihenfolge:** In dieser Kombobox können Sie unter den vorhandenen Sortierungen die entsprechende auswählen. Die Sortierungen werden in den Stammdaten angelegt und steuern an dieser Stelle, nach welchen Kriterien die Scheiben verarbeitet werden.
*   **Orga:** In dieser Kombobox können Sie unter den vorhandenen Master-Orgas die entsprechende auswählen. Die Master-Orgas werden in den Stammdaten angelegt und steuern, mit welcher Master-Orga der Lauf die Feinplanung durchläuft.
*   **Gruppenbildung:** In dieser Kombobox können Sie unter den vorhandenen Gruppierungen die entsprechende auswählen. Die Gruppierungen werden in den Stammdaten angelegt und steuern, anhand welcher Kriterien eine Gruppenbildung stattfinden soll.
*   **Sortierung auf Abstellplatz:** In dieser Kombobox können Sie unter den vorhandenen Sortierungen die entsprechende auswählen. Die Sortierungen werden in den Stammdaten angelegt und steuern, anhand welcher Kriterien Scheiben sortiert werden sollen.

> #### Weitere Informationen zu den Voreinstellungen
>
> *   ⇨ Tutorial, "Globale Einstellungen" auf Seite F-79
> *   ⇨ Überblick, "Schaltflächen" auf Seite A-78

## Gruppierung und Sortierung

Die Einstellungen, die Sie im Bereich `Gruppierung/Sortierung` vornehmen, haben die Aufgabe, die Scheiben auf den Abstellplätzen zu gruppieren und zu sortieren. Die Scheiben werden in Gruppen zusammengefasst und innerhalb der Gruppen sortiert. Es ist weiterhin möglich, die Abfolge der Gruppen zu bestimmen.

### Gruppierung/Sortierung - Dialog

Der Dialog ist in drei Register unterteilt:
*   Register Editor-Gruppierungen
*   Register Editor-Sortierung
*   Register Zusatz-Sortierungen

> #### Weitere Informationen zu Gruppierung und Sortierung
>
> *   ⇨ Tutorial, "Gruppierungen und Sortierungen" auf Seite F-21
> *   ⇨ Überblick, "Schaltflächen" auf Seite A-78

### Register Editor-Gruppierungen

**Pfad:** `Stammdaten > Feinplanung > Gruppierung > Register Editor - Gruppierung`

*Abb. F-55: Gruppierung/Sortierung-Dialog, Register Gruppierung*

In diesem Dialog stellen Sie neue Gruppierungen zusammen oder nehmen Änderungen an bestehenden Gruppierungen vor. Die im Register `Editor-Gruppierungen` vorhandenen Einträge finden in folgenden Bereichen Verwendung:

*   Softwarereferenz, “Einstellungen-Abstellplatz" auf Seite F-135
*   Softwarereferenz, "Orga-Gruppen" auf Seite F-133
*   Softwarereferenz, “Master-Orga" auf Seite F-126
*   Softwarereferenz, “Voreinstellungen" auf Seite F-139

Technische Info: Datenbanktabelle: `SORTING`

#### Erläuterung der Felder

**Linkes Fenster:** Das Fenster zeigt Ihnen alle angelegten Gruppierungen bzw. Sortierungen. Die einzelnen Gruppierungen/Sortierungen sind in einer Baumstruktur angelegt, so dass Sie sich die Eigenschaften, aus denen die Gruppierungen/Sortierungen bestehen, durch Aufklappen des Baumes anzeigen lassen können. Bsp.: Die Gruppierung `+Artikelnummer+Abstellbreite` beinhaltet die Eigenschaften `Artikelnummer` und `Abstellbreite`. Das Plus- oder Minus-Zeichen vor den jeweiligen Eigenschaften zeigt Ihnen die Sortier-Richtung der Eigenschaft. Bsp.: `+Artikelnummer` bedeutet, dass die Sortier-Richtung innerhalb der Artikelnummer aufsteigend ist. `-Artikelnummer` bedeutet, dass die Sortier-Richtung innerhalb der Artikelnummer absteigend ist.

#### Felder im Bereich Sortier-Richtung

*   **Aufsteigend:** Das Feld ist nur aktiv, wenn Sie eine Eigenschaft der Gruppierung/Sortierung markiert haben. Aktivieren Sie die Radiotaste `Aufsteigend`, bedeutet dies, dass die Sortier-Richtung der markierten Eigenschaft aufsteigend ist. Optisch wird die Eigenschaft noch durch das Plus-Zeichen vor der Eigenschaft gekennzeichnet.
*   **Absteigend:** Das Feld ist nur aktiv, wenn Sie eine Eigenschaft der Gruppierung/Sortierung markiert haben. Aktivieren Sie die Radiotaste `Absteigend`, bedeutet dies, dass die Sortier-Richtung der markierten Eigenschaft absteigend ist. Optisch wird die Eigenschaft noch durch das Minus-Zeichen vor der Eigenschaft gekennzeichnet.

#### Erläuterung der Schaltflächen im Bereich Sortier-Richtung

*   **Entfernen:** Das Betätigen dieser Schaltfläche führt entweder zum Löschen der markierten Eigenschaft der Gruppierung/Sortierung oder zum Löschen der kompletten Gruppierung/Sortierung. Das hängt davon ab, was Sie markiert haben. Haben Sie eine Eigenschaft der Gruppierung/Sortierung markiert, wird nur die Eigenschaft gelöscht. Ist jedoch die Gruppierung/Sortierung markiert, wird die komplette Gruppierung/Sortierung gelöscht.
*   **Hinzufügen:** Diese Schaltfläche steht in Zusammenhang mit dem rechten Fenster. Die Eigenschaft bzw. Formel, die im rechten Fenster markiert ist, wird durch das Betätigen der Schaltfläche `[Hinzufügen]` entweder als ganze Gruppierung/Sortierung oder als Eigenschaft in die Gruppierung/Sortierung eingefügt. Das hängt davon ab, was Sie markiert haben. Haben Sie eine Gruppierung/Sortierung markiert, wird die Eigenschaft bzw. Formel der markierten Gruppierung/Sortierung hinzugefügt. Haben Sie den in der linken Liste an oberster Stelle stehenden Eintrag (im Register `Editor-Gruppierungen` ist das der Eintrag `Gruppierungen`, im Register `Editor-Sortierung` ist das der Eintrag `Sortierung`) markiert, wird eine neue Gruppierung/Sortierung angelegt.

#### Erläuterung der Optionen

*   **Eigenschaft:** Ist die Radiotaste `Eigenschaft` aktiv, sehen Sie im rechten Fenster alle vorhanden Eigenschaften.
*   **Formel:** Ist die Radiotaste `Formel` aktiv, sehen Sie im rechten Fenster alle vorhanden Formeln.

#### Erläuterung der Schaltfläche

*   **Formeln:** Betätigen Sie diese Schaltfläche, öffnet sich der Dialog `Auswahl Formeln`. Sie können entweder eine bereits bestehende Formel ändern oder aber eine neue Formel erstellen. Nähere Erläuterungen finden Sie in der Dokumentation Formel-Editor.

> #### Weitere Informationen zu Gruppierungen
>
> *   ⇨ Tutorial, "Gruppierungen und Sortierungen" auf Seite F-21
> *   ⇨ Überblick, "Schaltflächen" auf Seite A-78

### Register Editor-Sortierung

**Pfad:** `Stammdaten > Feinplanung > Gruppierung > Register Editor - Sortierungen`

*Abb. F-56: Gruppierung/Sortierung-Dialog, Register Sortierung*

In diesem Dialog stellen Sie neue Sortierungen zusammen oder nehmen Änderungen an bestehenden Sortierungen vor.

Der Inhalt des Registers `Editor-Sortierung` ist mit dem des Registers `Editor-Gruppierungen` bis auf die nachstehend aufgeführte Schaltfläche identisch und wird deshalb an dieser Stelle nicht mehr erläutert. Die entsprechenden Informationen finden Sie unter dem Register `Editor-Gruppierung`.

Technische Info: Datenbanktabelle: `SORTING`

#### Erläuterung der Schaltfläche

*   **Zusatzsortierung:** Betätigen Sie diese Schaltfläche, öffnet sich für die markierte Sortierung der Dialog `Zusatz-Sortierungen`.

> #### Weitere Informationen zu Sortierungen
>
> *   ⇨ Tutorial, "Gruppierungen und Sortierungen" auf Seite F-21
> *   ⇨ Überblick, "Schaltflächen" auf Seite A-78

### Register Zusatz-Sortierungen

**Pfad:** `Stammdaten > Feinplanung > Gruppierung > Register Zusatz - Sortierungen`

*Abb. F-57: Gruppierung/Sortierung-Dialog, Register Zusatz-Sortierungen*

Dieser Dialog gibt Ihnen einen Überblick zu den vorhandenen Zusatz-Sortierungen. Die Zusatz-Sortierungen legen Sie im Dialog `Erzeugung einer Zusatz-Sortierung` an.

Technische Info: Datenbanktabelle:

#### Erläuterung der Felder

*   **Schlüssel:** Die Tabellenspalte `Schlüssel` zeigt, auf welchen Schlüssel die Zusatz-Sortierung angewendet wird.
*   **Wert:** In diesem Feld steht der Wert der Zusatz-Sortierung.
*   **Zusatzsortierung:** Das Feld zeigt Ihnen die komplette Sortierung an, auf die der Schlüssel wirkt.

> #### Weitere Informationen zu Zusatz-Sortierungen
>
> *   ⇨ Tutorial, "Zusatz-Sortierung" auf Seite F-28
> *   ⇨ Überblick, "Schaltflächen" auf Seite A-78

### Erzeugung einer Zusatz-Sortierung

**Pfad:** `Stammdaten > Feinplanung > Gruppierung > Register Editor - Sortierungen > [Erzeuge Zusatz-Sortierungen]`

*Abb. F-58: Erzeugung einer Zusatz-Sortierung*

Sortierungen können noch durch zusätzliche Sortierungen ergänzt werden. Dazu muss lediglich eine Zusatz-Sortierung erzeugt werden, der die Kombination Sortierungsschlüssel-Wert zugewiesen ist. Wenn nun eine Sortierung mit dem gegebenen Sortierungsschlüssel endet, so wird die Gruppe, deren Elemente alle den gegebenen Wert für den Sortierungsschlüssel haben, durch die zusätzliche Sortierung in weitere Gruppen aufgeteilt.

**Beispiel:** Auf einem Abstellplatz sind die Positionen nach `TOUR+KUNDENNUMMER+` sortiert. Wenn es nun eine Zusatzsortierung `KLEINMASS+` gibt mit `KUNDENNUMMER=4711`, so wird nur für den Kunden 4711 eine erweiterte Sortierung durchgeführt. Bei allen anderen Kunden ist die Reihenfolge beliebig. Selbstverständlich ist es möglich, verschiedenen Kunden verschiedene Zusatzsortierungen zuzuweisen.

Technische Info: Datenbanktabelle: `MORESORTING`

#### Erläuterung der Felder

*   **Wert:** In diesem Feld geben Sie den Wert für die Zusatz-Sortierung an. Die Optionen `Ziffer`, `Dicke`, `Text`, `Länge` und `SZR` steuern, um welchen Wert es sich handelt. Die Zusatz-Sortierungen sehen Sie im Register `Zusatz-Sortierung`.

#### Erläuterung der Schaltfläche

*   **Wert nicht prüfen:** Betätigen Sie diese Schaltfläche, wird, unabhängig des letzten Sortierungs-Schlüssels, die Zusatz-Sortierung verwendet.

> #### Weitere Informationen zur Erzeugung einer Zusatz-Sortierung
>
> *   ⇨ Tutorial, "Zusatz-Sortierung" auf Seite F-28
> *   ⇨ Überblick, "Schaltflächen" auf Seite A-78

## Abstellplätze

Der Dialog ist in drei Bereiche unterteilt:
*   A-Böcke
*   Fächerwagen
*   Feste Abstellplätze

### Abstellplätze Dialog

**Pfade:**
*   `Stammdaten > Feinplanung > Abstellplätze`
*   `Stammdaten > Feinplanung > Orga > Register Produktionsreihenfolge > Abstellplatz der Orga-Gruppe markieren > Schaltfläche [Einstellungen]`

*Abb. F-59: Abstellplätze*

In diesem Dialog definieren Sie die in Ihrem Betrieb vorhandenen Abstellplätze oder nehmen Änderungen an vorhandenen Abstellplätzen vor. Die hier definierten Abstellplätze werden von folgenden Bereichen der Feinplanung verwendet:

*   Softwarereferenz, “Einstellungen-Abstellplatz" auf Seite F-135
*   Softwarereferenz, “Register Orga" auf Seite F-182

(Hinweis: Die Details der Felder aus dem Dialog in Abb. F-59 sind in den vorherigen Abschnitten, insbesondere in "Einstellungen-Abstellplatz", beschrieben.)
