---
description: "DE-HB-AWEnterprise_10"
---


# Softwarereferenz: Spezielle Konditionen

---
## Beispiel

| Faktor | Grundpreis | Endpreis |
| :--- | :--- | :--- |
| 100 | 20,00 € | 20,00 € |
| 80 (entspricht einem Rabatt) | 20,00 € | 16,00 € |
| 150 (entspricht einem Aufschlag) | 20,00 € | 30,00 € |

## Artikelfaktoren - Details

**Stammdaten > Konditionen > Spezielle Konditionen > ISO-Einzelscheiben-Konditionen > Artikelfaktoren > `<F2>`**

*[Screenshot of "ISO-Einzelscheiben Artikelfaktoren" dialog window. It shows fields for Konditionsart, Kond.-Branche, Artikel, Faktor, Erfasser, Datum, and Kond. gültig von/bis.]*
**Abb. C-202 ISO-Einzelscheiben Artikelfaktoren - Details**

In diesem Dialog legen Sie den Gültigkeitszeitrahmen für die aktuelle Kondition fest.

`<F2>` Wechsel zur Übersicht.
⇨ "Artikelfaktoren - Übersicht" auf Seite C-899

### Feldbeschreibungen

Die Felder sind zum Dialog ISO-Einzelscheiben Artikelfaktoren – Übersicht beschrieben:
⇨ "Artikelfaktoren - Übersicht" auf Seite C-899

Zusätzlich werden die folgenden Felder angezeigt:

**Erfasser, Erfassungsdatum**
Anzeige des Erfassers und des Erfassungs- oder Änderungsdatums.

**Kondition gültig von ..., bis ...**
Angabe des Datums, ab dem und bis zu dem die Konditionen gültig sind.
*Technische Info: Datumsfeld, DB-Feld: kezartfa.vondat, kezartfa.abdat*

> **Ablauf der Gültigkeit**
> Wenn das Enddatum erreicht ist, werden für die Preisberechnung die allgemeinen Preise und Konditionen herangezogen. Die Artikelfaktoren für ISO-Einzelscheiben müssen Sie neu definieren, wenn Sie weiterhin mit diesen speziellen Konditionen arbeiten wollen.

## ISO-Einzelscheiben-Konditionen – Warengruppenfaktoren

**Stammdaten > Konditionen > Spezielle Konditionen > ISO-Einzelscheiben-Konditionen > Warengruppenfaktoren**

In diesem Dialog legen Sie marktpartner- und warengruppenspezifische Artikelfaktoren für Einzelscheiben fest.

Diese Konditionen gelten nur, wenn Sie dem entsprechenden Artikel in den ISO-Grundpreisen den Typ Einzelscheiben zugewiesen haben.
⇨ "ISO-Grundpreise" auf Seite C-711

Zu diesem Dialog stehen folgende Ansichten zur Verfügung:
*   "Warengruppenfaktoren – Übersicht" auf Seite C-902
*   "Warengruppenfaktoren - Details" auf Seite C-904

### Warengruppenfaktoren – Übersicht

**Stammdaten > Konditionen > Spezielle Konditionen > ISO-Einzelscheiben-Konditionen > Warengruppenfaktoren**

*[Screenshot of "Einzelscheiben-Warengruppenfaktoren" dialog window. It shows a table with columns for Konditionsart, Warengruppe, Bezeichnung, and Faktor.]*
**Abb. C-203 Einzelscheiben-Warengruppenfaktoren – Übersicht**

In dieser Übersicht pflegen Sie die marktpartner- und warengruppenspezifische Artikelfaktoren für Einzelscheiben.

`<F2>` Wechsel zur Detailansicht.
⇨ "Warengruppenfaktoren – Details" auf Seite C-904

### Feldbeschreibungen

> **Kunden und Lieferanten in den Konditionen**
> Kunden und Lieferanten, für die eine Kondition gilt, bezeichnen im Folgenden immer den jeweiligen Konditionsdebitor aus den Marktpartnerstammdaten.

**Konditionsart**
Auswahl, für wen die Konditionen gelten:
*   **Kunde:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für einen bestimmten Kunden.
*   **Lieferant:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für einen bestimmten Lieferanten.
*   **Objekt-Verkauf:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für ein bestimmtes Verkaufsobjekt.
*   **Objekt-Einkauf:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für ein bestimmtes Einkaufsobjekt.
*   **Kond.-Branche:** Die Konditionen gelten für die Berechnung von Preisen für eine bestimmte Marktpartnergruppe. Marktpartner, für die gemeinsame Konditionen gelten sollen, müssen einer Branche zugeordnet sein.
*Technische Info: numerisches Feld, Toggle-Feld, DB-Feld: kezwgrpfa.kondkz*

**(Marktpartner)**
Auswahl des Marktpartners, für den die Konditionen gelten. Je nach Konditionsart können Sie einen Kunden, einen Lieferanten, ein Objekt oder eine Kundengruppe angeben.
*Technische Info: numerisches Feld, DB-Feld: kezwgrpfa.kunr*

**Warengruppe, Bezeichnung**
Auswahl der Warengruppe des eingetauschten Glases, für die der Faktor gilt.
*Technische Info: alphanumerische Felder, DB-Feld: kezwgrpfa.wgrp*

**Faktor %**
Angabe des Faktors. Wenn Sie einen Faktor < 100 % angeben, wird er als Rabatt verwendet und reduziert den Preis. Der Faktor gilt dann, wenn die Einzelscheibe zur angegebenen Warengruppe gehört.
*Technische Info: numerisches Feld, DB-Feld: kezwgrpfa.faktor*

## Warengruppenfaktoren – Details

**Stammdaten > Konditionen > Spezielle Konditionen > ISO-Einzelscheiben-Konditionen > Warengruppenfaktoren > `<F2>`**

### Beispiel

| Faktor | Grundpreis | Endpreis |
| :--- | :--- | :--- |
| 100 | 20,00 € | 20,00 € |
| 80 (entspricht einem Rabatt) | 20,00 € | 16,00 € |
| 150 (entspricht einem Aufschlag) | 20,00 € | 30,00 € |

*[Screenshot of "Einzelscheiben-Warengruppenfaktoren" details dialog window. It shows fields for Konditionsart, Warengruppe, Faktor, Erfasser, and Kond. gültig von/bis.]*
**Abb. C-204 Einzelscheiben-Warengruppenfaktoren – Details**

In diesem Dialog legen Sie den Gültigkeitszeitrahmen für die Konditionen fest.

`<F2>` Wechsel zur Übersicht.
⇨ "Warengruppenfaktoren – Übersicht" auf Seite C-902

### Feldbeschreibungen

Die Felder sind zum Dialog Warengruppenfaktoren – Übersicht beschrieben:
⇨ "Warengruppenfaktoren – Übersicht" auf Seite C-902

Zusätzlich werden die folgenden Felder angezeigt:

**Erfasser, Erfassungsdatum**
Anzeige des Erfassers und des Erfassungs- oder Änderungsdatums.

**Kondition gültig von ..., bis ...**
Angabe des Datums, ab dem und bis zu dem die Konditionen gültig sind.
*Technische Info: Datumsfeld, DB-Feld: kezwgrpfa.vondat, kezwgrpfa.abdat*

> **Ablauf der Gültigkeit**
> Wenn das Enddatum erreicht ist, werden für die Preisberechnung die allgemeinen Preise und Konditionen herangezogen. Die Warengruppenfaktoren für Einzelscheiben müssen Sie neu definieren, wenn Sie weiterhin mit diesen speziellen Konditionen arbeiten wollen.

---

# Spezielle Preise

**Stammdaten > Konditionen > Spezielle Preise**

Über den Menüpunkt Spezielle Preise werden marktpartnerspezifische Preise für verschiedene Artikel angelegt.

Die speziellen Preise übersteuern die Preise aus den Preislisten. Die Konditionen wirken aber dennoch auf die speziellen Preise.
⇨ Tutorial, "Prioritäten der Konditionsermittlung" auf Seite C-646
⇨ "Konditionen" auf Seite C-834

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Artikelpreise" auf Seite C-906
*   "Spezielle Preise für Artikelvarianten" auf Seite C-914
*   "Preise für farbige Artikel" auf Seite C-919
*   "Sprossenpreise" auf Seite C-925
*   "Bearbeitungspreise" auf Seite C-930
*   "ISO-Austauschpreise" auf Seite C-937
*   "Spezielle Preise für ISO-Einzelscheiben" auf Seite C-944
*   "Spezielle ISO-Grundpreise" auf Seite C-949
*   "UV-Abdeckungspreise" auf Seite C-958
*   "Verglasungspreise" auf Seite C-962
*   "Austauschpreise Gussklassen" auf Seite C-966
*   "Spezielle VSG-Austausch-/Zusatzpreise" auf Seite C-970

## Artikelpreise

**Stammdaten > Konditionen > Spezielle Preise > Artikelpreise**

In diesem Dialog legen Sie Artikelpreise für einen Marktpartner, ein Objekt oder eine Branche fest.

In den Detailansichten legen Sie die Bedingungen für die Preisberechnung fest, z. B. Preisstaffeln, Mindestberechnungsmenge, Maßrundung, Zuschläge.

Die marktpartnerspezifischen Artikelpreise haben eine höhere Priorität als die Preise der Artikelvektoren.
⇨ "Artikelvektoren" auf Seite C-700

Zu diesem Dialog stehen folgende Ansichten zur Verfügung:
*   "Artikelpreise – Übersicht" auf Seite C-906
*   "Artikelpreise – Details" auf Seite C-910

### Artikelpreise – Übersicht

**Stammdaten > Konditionen > Spezielle Preise > Artikelpreise**

*[Screenshot of "Artikelpreise" overview dialog window. It shows a table with columns for Artikel, Bezeichnung, ab PLKZ, Preisart, Faktor, Preis 1, and Preistyp.]*
**Abb. C-205 Artikelpreise – Übersicht**

In dieser Übersicht pflegen Sie die Artikelpreise für einen Marktpartner, ein Objekt oder eine Branche.

Die marktpartnerspezifischen Artikelpreise haben eine höhere Priorität als die Preise der Artikelvektoren.
⇨ "Artikelvektoren" auf Seite C-700

### Feldbeschreibungen

`<F2>` Wechsel zur Detailansicht.
⇨ "Artikelpreise - Details" auf Seite C-910

`<F2> <F2>` Wechsel zur Detailansicht mit den Stufen 9 - 20.

> **Kunden und Lieferanten in den Konditionen**
> Kunden und Lieferanten, für die eine Kondition gilt, bezeichnen im Folgenden immer den jeweiligen Konditionsdebitor aus den Marktpartnerstammdaten.

**Konditionsart**
Auswahl, für wen die Konditionen gelten:
*   **Kunde:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für einen bestimmten Kunden.
*   **Lieferant:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für einen bestimmten Lieferanten.
*   **Objekt-Verkauf:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für ein bestimmtes Verkaufsobjekt.
*   **Objekt-Einkauf:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für ein bestimmtes Einkaufsobjekt.
*   **Kond.-Branche:** Die Konditionen gelten für die Berechnung von Preisen für eine bestimmte Marktpartnergruppe. Marktpartner, für die gemeinsame Konditionen gelten sollen, müssen einer Branche zugeordnet sein.
*Technische Info: numerisches Feld, Toggle-Feld, DB-Feld: kuartprs.kondkz*

**Marktpartner**
Auswahl des Marktpartners, für den die Konditionen gelten. Je nach Konditionsart können Sie einen Kunden, einen Lieferanten, ein Objekt oder eine Kundengruppe angeben.
*Technische Info: numerisches Feld, DB-Feld: kuartprs.kunr*

**Artikel**
Auswahl des Artikels, für den der marktpartnerspezifische Artikelpreis gelten soll.
*Technische Info: numerisches Feld, DB-Feld: kuartprs.artnr*

**Ab PLKZ**
Auswahl des Preislistenkennzeichens (PLKZ), ab dem die Preisdaten gelten.
Findet A+W Enterprise im Auftrag für den Artikel keine Preise zum aktuellen PLKZ, wird das numerisch vorausgehende PLKZ ermittelt, zu dem Preisdaten definiert sind.
⇨ Tutorial, "Ab-PLKZ-Logik” auf Seite C-560
*Technische Info: numerisches Feld, DB-Feld: kuartprs.plkz*

**Preisart, Bezeichnung**
Auswahl der Preisart, mit der der Preis ermittelt wird. Bei Preisen, die sich auf eine Grundmenge beziehen, wird die Mengeneinheit aus den Artikelstammdaten ausgewertet. Bei gestaffelten Preisen wird die Grundmenge aus der Auftragsposition mit den Grenzmengen der Preisstufen verglichen. Der Preis wird nach der Preisstufe berechnet, die durch diese Menge erreicht ist:
⇨ Tutorial, "Preisarten" auf Seite C-572
*   **1 - Einzelpreis:** Zur Preisberechnung wird der Preis der Stufe 1 herangezogen.
*   **2 - Staffelstufe:** Zur Preisberechnung wird die Preisstufe ermittelt, die in den Konditionen angegeben ist.
    ⇨ "Tageskonditionen" auf Seite C-835
    ⇨ "Spezielle Konditionen" auf Seite C-849
*   **3 - Mengenstaffel pro Position (GME):** Zur Ermittlung der Preisstufe wird die Menge der Position anhand der Grundmengeneinheit (GME) des Artikels ermittelt. Der Preis wird im Auftrag nach der Preisstufe berechnet, die durch die Gesamtmenge der Position erreicht ist.
    ⇨ "Artikelpreise - Details" auf Seite C-910
*   **4 - Mengenstaffel pro Stück (GME):** Zur Ermittlung der Preisstufe wird die Grundmenge in einem Stück der Position ermittelt.
*   **9 - Stück pro Position:** Zur Preisberechnung wird die jeweilige Stückzahl der einzelnen Positionen ermittelt.
*   **10 - Gesamtmenge pro Auftrag:** Zur Preisberechnung wird die Gesamtmenge aller Positionen im Auftrag ermittelt.
*   **11 - Variantenartig:** Bei dieser Preisart können die Preise abhängig von 2 Maßen gestaffelt werden, z. B. Höhe und Breite. Zur Ermittlung der Preisstufe wird das kleinere Maß mit der ersten Spalte verglichen, das größere mit der zweiten Spalte. Der Preis wird nach der Preisstufe berechnet, bei der die Grenzwerte von beiden Maßen erreicht sind.
*   **12 - Variantenstaffel:** Die Preisart ist sinnvoll für Glastüren. Bei dieser Preisart wird die Breite der Glastür mit dem Wert aus der ersten Spalte verglichen und die Höhe der Glastür mit dem Wert aus der zweiten Spalte. Dabei ist wichtig, dass die Maße aufsteigend eingeben werden, zuerst nach der ersten Spalte und dann nach der zweiten Spalte. Der Preis wird nach der Preisstufe berechnet, bei der die Grenzwerte von beiden Maßen erreicht sind.
> **Variantenstaffel vs. Variantenpreise**
> Für Glastüren mit Standardmaßen werden herkömmlicherweise Variantenpreise hinterlegt und für Glastüren mit Sondermaßen Vektorpreise mit der Preisart Variantenstaffel.
> Wenn Glastüren mit Standardmaßen bestellt werden, werden die Variantenpreise herangezogen. Bei Sondermaßen ermittelt A+W Enterprise die Vektorpreise mit der Preisart Variantenstaffel.

*   **13 - Mengenstaffel/Gebindegröße:** Diese Preisart wird dann verwendet, wenn ein Stückpreis für einen Artikel einen sehr geringen Wert hat, der nicht mit einer Genauigkeit von zwei Nachkommastellen angegeben werden kann. Die Preise können auch nach Mengen bis gestaffelt werden. Je nach Konfiguration können die Mengenangaben Positionsstückzahlen oder Positionsmengen in Grundmengeneinheiten des Artikels sein.
*Technische Info: numerisches Feld, DB-Feld: kuartprs.part*

**Beispiel**
Der Stückpreis für einen Sack mit 1000 Korkblättchen beträgt 2,54 €.
Pro Scheibe werden 5 Blättchen verbraucht. Bei einer Positionsmenge von 15 Scheiben werden 75 Blättchen gebraucht.
Der Positionspreis wird als genauer Stückpreis berechnet und anschließend auf zwei Nachkommastellen gerundet.
75 Stück x 0,00254 € = 0,1905 €, ergibt nach Rundung 0,19 €.

**Faktor %**
Angabe eines Faktors, mit dem der Artikelpreis multipliziert wird. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preisstufen anpassen zu müssen, z. B. für eine Preiserhöhung. Wenn Sie das Feld leer lassen, gilt entsprechend der Konditionshierarchie der Faktor aus den Konditionen.
*Technische Info: numerisches Feld, DB-Feld: kuartprs.faktor*

**Beispiel**

| Faktor | Grundpreis | Endpreis |
| :--- | :--- | :--- |
| 100 | 20,00 € | 20,00 € |
| 80 (entspricht einem Rabatt) | 20,00 € | 16,00 € |
| 150 (entspricht einem Aufschlag) | 20,00 € | 30,00 € |

**Preis 1**
Angabe des Einzelpreises. Dieser Preis wird im Auftrag berechnet, wenn als Preisart Einzelpreis angegeben ist oder wenn die Maße der Auftragsposition die Maß- oder Mengenangaben aller anderen Preisstufen unterschreiten. Das Feld ist gesperrt, wenn als Preisart Mengenstaffel/Gebindegröße angegeben ist, da bei dieser Preisart für jede Preisstufe eine Mengenangabe benötigt wird.
*Technische Info: numerisches Feld, DB-Feld: kuartprs.preis1*

**Preistyp**
Angabe, worauf sich der angegebene Preis bezieht:
*   **WE/GME:** Der Preis wird pro Grundmengeneinheit aus den Artikelstammdaten berechnet, z. B. pro qm.
*   **WE/Stück:** Im Auftrag wird der Preis als fester Betrag pro Stück in der Position berechnet.
*Technische Info: alphanumerisches Feld, Toggle-Feld, DB-Feld: kuartprs.ptyp1*

### Artikelpreise – Details

**Stammdaten > Konditionen > Spezielle Preise > Artikelpreise > `<F2>`**

*[Screenshot of "Artikelpreise - Details" dialog window. It shows header information and a table for price scaling (Stufe, ab Menge, Preis, Preistyp).]*
**Abb. C-206 Artikelpreise – Details**

In diesem Dialog legen Sie die Details für die marktpartnerspezifischen Artikelpreise fest. Zusätzlich können Sie Zuschläge und die Stückpreisrundung angeben.

#### Feldbeschreibungen (Details)

Die Felder im Kopfbereich sind zum Dialog Artikelpreise – Übersicht beschrieben:
⇨ "Artikelpreise - Übersicht" auf Seite C-906

Zusätzlich werden die folgenden Felder angezeigt:

**Mindestberechnung ... ME**
Angabe der Mindestmenge, für die der Preis berechnet wird. Die Mindestmenge wird entsprechend der Grundmengeneinheit im Artikelstamm angegeben, z. B. Fläche in qm. Wenn die Fläche des Glases in der Auftragsposition kleiner ist als die Mindestberechnung, wird der Preis für diese Mindestberechnung berechnet.
⇨ Tutorial, "Preisrelevante Menge" auf Seite C-571
*Technische Info: numerisches Feld, DB-Feld: kuartprs.minber*

**Maßrundung... mm**
Angabe der Maßrundung in mm für die Preisberechnung der Artikel, z. B. 30 mm. Für die Preisberechnung werden die Kantenlängen in der Auftragsposition auf die nächsthöhere Länge in mm aufgerundet, die durch die angegebene Maßrundung teilbar ist.
*Technische Info: numerisches Feld, DB-Feld: kuartprs.massrund*

**Beispiel**
Als Maßrundung ist 30 mm definiert.
Der erfasste ISO-Artikel hat die Maße 1000 x 1000 mm. Die nächste durch 30 mm teilbare Kantenlänge ist 1020 mm.
Der Preis wird aus den Maßen 1020 × 1020 mm = 1,04 qm berechnet.

**Zuschlagsmatrix**
Auswahl einer Zuschlagsmatrix für einen allgemeinen Zuschlag auf den Glaspreis.
⇨ "Zuschlagsmatrizen" auf Seite C-814
*Technische Info: numerisches Feld, DB-Feld: kuartprs.zumatnr*

**Größenzuschl.**
Auswahl eines Größenzuschlags, z. B. Kleinglaszuschlag, Überlängenzuschlag usw. Wenn die Auftragsposition den angegebenen Grenzwert im Zuschlag über- oder unterschreitet, wird der Preis um den Zuschlag erhöht.
⇨ “Größenzuschläge" auf Seite C-819
⇨ Tutorial, "Größenzuschläge" auf Seite C-638
*Technische Info: numerisches Feld, DB-Feld: kuartprs.grosszu*

**Stufenzuschlagsvektor**
Auswahl des Zuschlags für die Stufen bei ISO-Scheiben oder VSG-Gläsern.
⇨ Tutorial, "Stufenzuschläge" auf Seite C-642

**EK-Preis WE**
Zurzeit nicht genutzt.
*Technische Info: numerisches Feld, DB-Feld: kuartprs.ekpreis*

**Min.Kantenl.**
Angabe der Kantenlänge in mm für die Preisberechnung. Diese Größe wird herangezogen, wenn die Höhe oder Breite des Glases in der Auftragsposition kleiner ist als diese Mindestkantenlänge.
*Technische Info: numerisches Feld, DB-Feld: kuartprs.minkant*

**Mindestpreis**
Angabe des Mindestpreises. Dieser Preis wird berechnet, wenn der berechnete Preis in der Auftragsposition niedriger ist als der angegebene Mindestpreis.
*   Mindestpreise für Kopfartikel werden nur bei den Preismethoden ISO-Schweiz, ISO-Aktuell (nur mit der Berechnungsart Vektor), PKZ-VSG, PKZ-ESG, PKZ-Basisglas, PKZ-veredeltes Glas oder PKZ-Preise ausgewertet.
*   Mindestpreise für Stücklistenunterteile werden nur ausgewertet, wenn beim Kopfartikel die Preismethode ISO-Aktuell, PKZ-VSG, PKZ-ESG, PKZ-Basisglas, PKZ-veredeltes Glas oder PKZ-Glastüren gewählt ist und das Unterteil ein Zubehörartikel mit der Preismethode PKZ-Preise allgemein ist.
*Technische Info: numerisches Feld, DB-Feld: kuartprs.minpreis*

**Stufe ab Menge 2 ... bis Menge 2...**
Eingabe der Grenzmenge pro Stufe. Je nach Preisart wird ab Menge oder bis Menge angezeigt. Die Felder sind gesperrt, wenn als Preisart Einzelpreis gewählt ist.
*   **ab Menge:** Der angegebene Preis wird berechnet, wenn im Auftrag die Menge größer oder gleich dem Grenzwert ist.
*   **bis Menge:** Der angegebene Preis wird berechnet, wenn im Auftrag die Menge kleiner oder gleich dem Grenzwert ist.
Der Grenzwert wird je nach Preisart als Stückzahl, als Menge pro Grundmengeneinheit oder als Kantenlänge interpretiert.
Die Mengenfelder bis Stufe 20 erreichen Sie mit `<F2>`. Wenn alle 20 Stufen angelegt sind, können Sie mit `<F2>` weitere Stufen hinterlegen.
*Technische Info: numerische Felder, DB-Felder: kuartprs.me2, kuartprs.me3, ..., kuartprs.me20. kuartptab.mas1*

**(Maß 2)**
Diese Felder sind nur freigeschaltet, wenn als Preisart 11 Variantenartig oder 12 Variantenstaffel gewählt ist. Wenn im Auftrag die Kantenlängen des Artikels größer oder gleich den Grenzwerten sind, gilt der Preis dieser Preisstufe.
*Technische Info: numerische Felder, DB-Felder: kuartprs.mas2_2, kuartprs.mas2_3, ... kuartprs.mas2_20*

**Preis**
Angabe des Preises pro Stufe. Abhängig vom Preistyp wird der Preis pro Stück oder pro Mengeneinheit berechnet. Wenn als Preisart Einzelpreis gewählt ist, wird nur der Preis der Stufe 1 verwendet. Das Feld ist gesperrt, wenn als Preisart Mengenstaffel/Gebindegröße angegeben ist, da bei dieser Preisart für jede Preisstufe eine Mengenangabe benötigt wird.
*Technische Info: numerische Felder, DB-Felder: kuartprs.preis2, kuartprs.preis3, ... kuartprs.preis20*

**Preistyp**
Angabe, worauf sich der angegebene Preis bezieht:
*   **WE/GME:** Der Preis wird pro Grundmengeneinheit aus den Artikelstammdaten berechnet, z. B. pro qm.
*   **WE/Stück:** Im Auftrag wird der Preis als fester Betrag pro Stück in der Position berechnet.
*Technische Info: alphanumerische Felder, Toggle-Felder, DB-Felder: kuartprs.ptyp2, kuartprs.ptyp3, ... kuartprs.ptyp20*

**Erfasser, Erfassungsdatum**
Anzeige des Erfassers und des Erfassungs- oder Änderungsdatums.

**Kondition gültig von ..., bis ...**
Angabe des Datums, ab dem und bis zu dem die Konditionen gültig sind.
*Technische Info: Datumsfeld, DB-Feld: kuartprs.vondat, kuartprs.abdat*

> **Ablauf der Gültigkeit**
> Wenn das Enddatum erreicht ist, werden für die Preisberechnung die allgemeinen Preise und Konditionen herangezogen. Die Staffelrabatte müssen Sie neu definieren, wenn Sie weiterhin mit diesen Konditionen arbeiten wollen.

## Spezielle Preise für Artikelvarianten

**Stammdaten > Konditionen > Spezielle Preise > Variantenpreise**

In diesem Dialog legen Sie Preise für Artikelvarianten an, die für einen Marktpartner, ein Objekt oder eine Branche gelten.

In der Detailansicht legen Sie die Bedingungen für die Preisberechnung fest, z. B. Rabattstaffeln, Maßrundung.

Die marktpartnerspezifischen Variantenpreise haben eine höhere Priorität als die allgemeinen Variantenpreise.
⇨ "Artikelvektoren" auf Seite C-749

Zu diesem Dialog stehen folgende Ansichten zur Verfügung:
*   "Spezielle Variantenpreise – Übersicht" auf Seite C-914
*   "Spezielle Variantenpreise - Details" auf Seite C-917

### Spezielle Variantenpreise – Übersicht

**Stammdaten > Konditionen > Spezielle Preise > Variantenpreise**

*[Screenshot of "Spezielle Variantenpreise" overview dialog window. It shows a table with columns for Artikel, Bezeichnung, ab PLKZ, Var., Preisart, Faktor, etc.]*
**Abb. C-207 Spezielle Variantenpreise – Übersicht**

In dieser Übersicht pflegen Sie Preise für Artikelvarianten, die für einen Marktpartner, ein Objekt oder eine Branche gelten.

Die marktpartnerspezifischen Variantenpreise haben eine höhere Priorität als die allgemeinen Variantenpreise.
"Artikelvektoren" auf Seite C-749

`<F2>` Wechsel zur Detailansicht.
⇨ "Spezielle Variantenpreise - Details" auf Seite C-917

### Feldbeschreibungen

> **Kunden und Lieferanten in den Konditionen**
> Kunden und Lieferanten, für die eine Kondition gilt, bezeichnen im Folgenden immer den jeweiligen Konditionsdebitor aus den Marktpartnerstammdaten.

**Konditionsart**
Auswahl, für wen die Konditionen gelten:
*   **Kunde:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für einen bestimmten Kunden.
*   **Lieferant:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für einen bestimmten Lieferanten.
*   **Objekt-Verkauf:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für ein bestimmtes Verkaufsobjekt.
*   **Objekt-Einkauf:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für ein bestimmtes Einkaufsobjekt.
*   **Kond.-Branche:** Die Konditionen gelten für die Berechnung von Preisen für eine bestimmte Marktpartnergruppe. Marktpartner, für die gemeinsame Konditionen gelten sollen, müssen einer Branche zugeordnet sein.
*Technische Info: numerisches Feld, Toggle-Feld, DB-Feld: spezvarprs.kondkz*

**(Marktpartner)**
Auswahl des Marktpartners, für den die Konditionen gelten. Je nach Konditionsart können Sie einen Kunden, einen Lieferanten, ein Objekt oder eine Kundengruppe angeben.
*Technische Info: numerisches Feld, DB-Feld: spezvarprs.kondnr*

**Artikel, Bezeichnung**
Auswahl des Artikels, für den der marktpartnerspezifische Variantenpreis gilt. Der Artikel muss in den Artikelstammdaten als Artikel mit Maß- oder Größenvariante definiert sein.
*Technische Info: numerisches Feld, DB-Feld: spezvarprs.artnr*

**Ab PLKZ**
Auswahl des Preislistenkennzeichens (PLKZ), ab dem die Preisdaten gelten sollen.
Findet A+W Enterprise im Auftrag für den Artikel keine Preise zum aktuellen PLKZ, wird das numerisch vorausgehende PLKZ ermittelt, zu dem Preisdaten definiert sind.
⇨ Tutorial, "Ab-PLKZ-Logik" auf Seite C-560
*Technische Info: numerisches Feld, DB-Feld: spezvarprs.plkz*

**Variante**
Auswahl der Artikelvariante, für die der Preis gilt.
*Technische Info: numerisches Feld, DB-Feld: spezvarprs.varnr*

**Preisart, Bezeichnung**
Auswahl der Preisart.
Bei Preisen, die sich auf eine Grundmenge beziehen, wird die Mengeneinheit aus den Artikelstammdaten ausgewertet.
Bei gestaffelten Preisen wird die Grundmenge aus der Auftragsposition mit den Grenzmengen der Preisstufen verglichen. Der Preis wird nach der Preisstufe ermittelt, die durch diese Menge erreicht ist:
*   **9 - Stück pro Position:** Zur Ermittlung der Preisstufe wird die Stückzahl der Position verwendet.
*   **13 - Mengenstaffel/Gebindegröße:** Diese Preisart wird dann verwendet, wenn ein Preis für einen Artikel einen sehr geringen Wert hat, der nicht mit einer Genauigkeit von zwei Nachkommastellen dargestellt werden kann.
*Technische Info: numerisches Feld, DB-Feld: spezvarprs.part*

**Beispiel**
Artikel mit Stückpreis von 0,0254 Euro: bei Menge 100 = 2,54 WE/Stück.
Der Stückpreis für einen Sack mit 1000 Korkblättchen beträgt 25,40 €.
Pro Scheibe werden 5 Blättchen verbraucht.
Bei einer Positionsmenge von 15 Scheiben werden 75 Blättchen gebraucht.
Der Positionspreis wird als genauer Stückpreis berechnet und anschließend auf zwei Nachkommastellen gerundet.
*   Berechnung: 75 Stück x 0,0254 € = 1,905 €
*   nach Rundung = 1,91 €

**Faktor %**
Angabe eines Faktors, mit dem der Variantenpreis multipliziert wird. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preisstufen anpassen zu müssen, z. B. für eine Preiserhöhung. Wenn Sie das Feld leer lassen, gilt entsprechend der Konditionshierarchie der Faktor aus den Konditionen.
*Technische Info: numerisches Feld, DB-Feld: spezvarprs.faktor*

**Beispiel**

| Faktor | Grundpreis | Endpreis |
| :--- | :--- | :--- |
| 100 | 20,00 € | 20,00 € |
| 80 (entspricht einem Rabatt) | 20,00 € | 16,00 € |
| 150 (entspricht einem Aufschlag) | 20,00 € | 30,00 € |

**Preis 1**
Angabe des Einzelpreises. Dieser Preis wird im Auftrag berechnet, wenn als Preisart Stück pro Position angegeben ist und wenn die Menge des Artikels die Mengenangaben aller anderen Preisstufen unterschreitet. Das Feld ist gesperrt, wenn als Preisart Mengenstaffel/Gebindegröße angegeben ist, da bei dieser Preisart für jede Preisstufe eine Mengenangabe benötigt wird.
*Technische Info: numerisches Feld, DB-Feld: spezvarprs.preis1*

**Preistyp**
Angabe, worauf sich der angegebene Preis bezieht:
*   **WE/Stück:** Im Auftrag wird der Preis als fester Betrag pro Stück in der Position berechnet.
*   **WE/GME:** Der Preis wird pro Grundmengeneinheit aus den Artikelstammdaten berechnet, z. B. pro qm.
*Technische Info: alphanumerisches Feld, Toggle-Feld, DB-Feld: spezvarprs.preistyp1*

### Spezielle Variantenpreise – Details

**Stammdaten > Konditionen > Spezielle Preise > Variantenpreise > `<F2>`**

*[Screenshot of "Spezielle Variantenpreise - Details" dialog window. It shows fields for setting up scaled prices (bis Menge, Preis, Preistyp).]*
**Abb. C-208 Spezielle Variantenpreise – Details**

In diesem Dialog legen Sie die Staffelpreise und einen Wert für die Maßrundung für Varianten fest.

`<F2>` Wechsel zur Übersicht.
⇨ "Spezielle Variantenpreise – Übersicht" auf Seite C-914

#### Feldbeschreibungen (Details)

Die Felder im Kopfbereich sind zum Dialog Variantenpreise – Übersicht beschrieben:
⇨ "Spezielle Variantenpreise – Übersicht" auf Seite C-914

Zusätzlich werden die folgenden Felder angezeigt:

**Maßrundung... mm**
Angabe der Maßrundung in mm für die Preisberechnung des Artikels, z. B. 30 mm. Für die Preisberechnung werden die Kantenlängen in der Auftragsposition auf die nächsthöhere Länge in mm aufgerundet, die durch die angegebene Maßrundung teilbar ist.
*Technische Info: numerisches Feld, DB-Feld: spezvarprs.massrund*

**Beispiel**
Als Maßrundung ist 30 mm definiert.
Der erfasste ISO-Artikel hat die Maße 1000 x 1000 mm. Die nächste durch 30 mm teilbare Kantenlänge ist 1020 mm.
Der Preis wird aus den Maßen 1020 × 1020 mm = 1,04 qm berechnet.

**Ab Menge ..., bis Menge ...**
Eingabe der Grenzmenge pro Stufe. Je nach Preisart wird ab Menge oder bis Menge angezeigt.
*   **ab Menge:** Der angegebene Preis wird berechnet, wenn im Auftrag die Menge größer oder gleich dem Grenzwert ist.
*   **bis Menge:** Der angegebene Preis wird berechnet, wenn im Auftrag die Menge kleiner oder gleich dem Grenzwert ist.
Der Grenzwert wird je nach Preisart als Stückzahl, als Menge pro Grundmengeneinheit oder als Kantenlänge interpretiert.
*Technische Info: numerische Felder, DB-Felder: spezvarprs.anz2, spezvarprs.anz..., spezvarprs.anz5*

**Preis**
Angabe des Preises pro Stufe. Abhängig vom Preistyp wird der Preis pro Stück oder pro Mengeneinheit berechnet.
*Technische Info: numerische Felder, DB-Felder: spezvarprs.preis2, spezvarprs.preis3, ... spezvarprs.preis5*

**Preistyp**
Angabe, worauf sich der angegebene Preis bezieht:
*   **WE/Stück:** Im Auftrag wird der Preis als fester Betrag pro Stück in der Position berechnet.
*   **WE/GME:** Der Preis wird pro Grundmengeneinheit aus den Artikelstammdaten berechnet, z. B. pro qm.
Wenn als Preisart Mengenstaffel/Gebindegröße angegeben ist, müssen Sie Preisstufen angeben.
*Technische Info: alphanumerische Felder, Toggle-Felder, DB-Felder: spezvarprs.preistyp2, spezvarprs.preistyp3, ... spezvarprs.preistyp5*

**Erfasser, Erfassungsdatum**
Anzeige des Erfassers und des Erfassungs- oder Änderungsdatums.

**Kondition gültig von ..., bis ...**
Angabe des Datums, ab dem und bis zu dem die Konditionen gültig sind.
*Technische Info: Datumsfeld, DB-Feld: spezvarprs.vondat, spezvarprs.abdat*

> **Ablauf der Gültigkeit**
> Wenn das Enddatum erreicht ist, werden für die Preisberechnung die allgemeinen Preise und Konditionen herangezogen. Die marktpartnerspezifischen Variantenpreise müssen Sie neu definieren, wenn Sie weiterhin mit diesen Konditionen arbeiten wollen.

## Preise für farbige Artikel

**Stammdaten > Konditionen > Spezielle Preise > Farbige Artikel**

In diesem Dialog können Sie sich alle marktpartnerspezifischen Preise zu einem Farbartikel anzeigen lassen.

Der Artikel muss in den Artikelstammdaten als farbiger Artikel definiert sein.

In der Detailansicht legen Sie die Bedingungen für die Preisberechnung fest, z. B. Preisstaffeln, Mindestberechnungsmenge, Maßrundung.

Zu diesem Dialog stehen folgende Ansichten zur Verfügung:
*   "Preise für farbige Artikel – Übersicht" auf Seite C-919
*   "Preise für farbige Artikel - Details" auf Seite C-922

### Preise für farbige Artikel – Übersicht

**Stammdaten > Konditionen > Spezielle Preise > Farbige Artikel**

*[Screenshot of "Preise für farbige Artikel" overview dialog window. It shows a table with columns for Artikel, ab PLKZ, Farbe, Preisart, Preistyp, and Preis 1.]*
**Abb. C-209 Preise für farbige Artikel – Übersicht**

In dieser Übersicht pflegen Sie die marktpartnerspezifischen Preise für farbige Artikel. Diese Preise für farbige Artikel haben eine höhere Priorität als die allgemeinen Preise für farbige Artikel.
⇨ "PKZ-Preise für farbige Artikel" auf Seite C-784

Der Artikel muss in den Artikelstammdaten als farbiger Artikel definiert sein.

`<F2>` Wechsel zur Detailansicht.
⇨ "Preise für farbige Artikel – Details" auf Seite C-922

### Feldbeschreibungen

> **Kunden und Lieferanten in den Konditionen**
> Kunden und Lieferanten, für die eine Kondition gilt, bezeichnen im Folgenden immer den jeweiligen Konditionsdebitor aus den Marktpartnerstammdaten.

**Konditionsart**
Auswahl, für wen die Konditionen gelten:
*   **Kunde:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für einen bestimmten Kunden.
*   **Lieferant:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für einen bestimmten Lieferanten.
*   **Objekt-Verkauf:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für ein bestimmtes Verkaufsobjekt.
*   **Objekt-Einkauf:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für ein bestimmtes Einkaufsobjekt.
*   **Kond.-Branche:** Die Konditionen gelten für die Berechnung von Preisen für eine bestimmte Marktpartnergruppe. Marktpartner, für die gemeinsame Konditionen gelten sollen, müssen einer Branche zugeordnet sein.
*Technische Info: numerisches Feld, Toggle-Feld, DB-Feld: kufarbprs.kondkz*

**Marktpartner**
Auswahl des Marktpartners, für den die Konditionen gelten. Je nach Konditionsart können Sie einen Kunden, einen Lieferanten, ein Objekt oder eine Kundengruppe angeben.
*Technische Info: numerisches Feld, DB-Feld: kufarbprs.kunr*

**Artikel, Bezeichnung**
Auswahl des Farbartikels, für den der marktpartnerspezifische Preis gilt.
*Technische Info: numerisches Feld, DB-Feld: kufarbprs.artnr*

**Ab PLKZ**
Auswahl des Preislistenkennzeichens (PLKZ), ab dem die Preisdaten gelten.
Findet A+W Enterprise im Auftrag für den Artikel keine Preise zum aktuellen PLKZ, wird das numerisch vorausgehende PLKZ ermittelt, zu dem Preisdaten definiert sind.
⇨ Tutorial, "Ab-PLKZ-Logik" auf Seite C-560
*Technische Info: numerisches Feld, DB-Feld: kufarbprs.plkz*

**Farbe**
Auswahl der Farbvariante, für die der Preis gilt.
*Technische Info: numerisches Feld, DB-Feld: kufarbprs.farbnr*

**Preisart, Bezeichnung**
Auswahl der Preisart, mit der der Preis ermittelt wird.
Bei Preisen, die sich auf eine Grundmenge beziehen, wird die Mengeneinheit aus den Artikelstammdaten ausgewertet.
Bei gestaffelten Preisen wird die Grundmenge aus der Auftragsposition mit den Grenzmengen der Preisstufen verglichen. Der Preis wird nach der Preisstufe berechnet, die durch diese Menge erreicht ist:
⇨ Tutorial, "Preisarten" auf Seite C-572
*   **1 - Einzelpreis:** Zur Preisberechnung wird der Preis der Stufe 1 herangezogen.
*   **2 - Staffelstufe:** Zur Preisberechnung wird die Preisstufe ermittelt, die in den Konditionen angegeben ist.
    ⇨ "Tageskonditionen" auf Seite C-835
    ⇨ "Spezielle Konditionen" auf Seite C-849
*   **3 - Mengenstaffel pro Position (GME):** Zur Ermittlung der Preisstufe wird die Menge der Position anhand der Grundmengeneinheit (GME) des Artikels ermittelt. Der Preis wird im Auftrag nach der Preisstufe berechnet, die durch die Gesamtmenge der Position erreicht ist.
    ⇨ "Artikelpreise - Details" auf Seite C-910
*   **4 - Mengenstaffel pro Stück (GME):** Zur Ermittlung der Preisstufe wird die Grundmenge in einem Stück der Position ermittelt.
*   **13 - Mengenstaffel/Gebindegröße:** Diese Preisart wird dann verwendet, wenn ein Preis für einen Artikel einen sehr geringen Wert hat, der nicht mit einer Genauigkeit von zwei Nachkommastellen dargestellt werden kann.
*Technische Info: numerisches Feld, DB-Feld: kufarbprs.part*

**Beispiel**
Artikel mit Stückpreis von 0,0254 Euro: bei Menge 100 = 2,54 WE/Stück.
Der Stückpreis für einen Sack mit 1000 Korkblättchen beträgt 25,40 €.
Pro Scheibe werden 5 Blättchen verbraucht.
Bei einer Positionsmenge von 15 Scheiben werden 75 Blättchen gebraucht.
Der Positionspreis wird als genauer Stückpreis berechnet und anschließend auf zwei Nachkommastellen gerundet.
*   Berechnung: 75 Stück x 0,0254 € = 1,905 €
*   nach Rundung = 1,91 €.

**Preistyp**
Angabe, worauf sich der angegebene Preis bezieht:
*   **WE/Stück:** Im Auftrag wird der Preis als fester Betrag pro Stück in der Position berechnet.
*   **WE/GME:** Der Preis wird pro Grundmengeneinheit des Farbartikels berechnet.
*Technische Info: alphanumerisches Feld, Toggle-Feld, DB-Feld: kufarbprs.ptyp*

**Preis 1**
Angabe des Einzelpreises. Dieser Preis wird berechnet, wenn als Preisart Einzelpreis definiert ist oder wenn die Maße der Auftragsposition die Maß- oder Mengenangaben aller anderen Preisstufen unterschreiten. Das Feld ist bei der Preisart Mengenstaffel/Gebindegröße gesperrt.
*Technische Info: numerisches Feld, DB-Feld: kufarbprs.peis1*

### Preise für farbige Artikel – Details

**Stammdaten > Konditionen > Spezielle Preise > Farbige Artikel > `<F2>`**

*[Screenshot of "Preise für farbige Artikel - Details" dialog window. It shows header information and up to 10 price scale steps (Stufe bis Menge, Preis).]*
**Abb. C-210 Preise für farbige Artikel – Details**

In diesem Dialog legen Sie die Bedingungen für die Berechnung von marktpartnerspezifischen Preisen eines Farbartikels fest, z. B. Mindestberechnungsflächen, Maßrundungen und Staffelpreise.

`<F2>` Wechsel zur Übersicht.
⇨ "Preise für farbige Artikel – Übersicht" auf Seite C-919

#### Feldbeschreibungen (Details)

Die Felder im Kopfbereich sind zum Dialog Preise für farbige Artikel – Übersicht beschrieben:
⇨ "Preise für farbige Artikel – Übersicht" auf Seite C-919

Zusätzlich werden die folgenden Felder angezeigt:

**Maßrundung... mm**
Angabe der Maßrundung in mm für die Preisberechnung des Artikels, z. B. 30 mm. Für die Preisberechnung werden die Kantenlängen in der Auftragsposition auf die nächsthöhere Länge in mm aufgerundet, die durch die angegebene Maßrundung teilbar ist.
*Technische Info: numerisches Feld, DB-Feld: kufarbprs.massrund*

**Beispiel**
Als Maßrundung ist 30 mm definiert.
Der erfasste ISO-Artikel hat die Maße 1000 × 1000 mm. Die nächste durch 30 mm teilbare Kantenlänge ist 1020 mm.
Der Preis wird aus den Maßen 1020 × 1020 mm = 1,04 qm berechnet.

**Mindestberechnung ... Einheiten**
Angabe der Mindestmenge, die berechnet wird. Ausschlaggebend ist die Mengeneinheit aus den Artikelstammdaten. Wenn die Menge in der Auftragsposition kleiner ist als der angegebene Wert, wird diese Mindestberechnungsmenge berechnet.
⇨ Tutorial, "Preisrelevante Menge" auf Seite C-571
*Technische Info: numerisches Feld, DB-Feld: kufarbprs.minber*

**Faktor %**
Angabe eines Faktors, mit dem der marktpartnerspezifische Artikelpreis multipliziert wird. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preisstufen anpassen zu müssen, z. B. für eine Preiserhöhung oder einen Rabatt. Wenn Sie das Feld leer lassen, gilt entsprechend der Konditionshierarchie der Faktor aus den Konditionen.
*Technische Info: numerisches Feld, DB-Feld: kufarbprs.faktor*

**Beispiel**

| Faktor | Grundpreis | Endpreis |
| :--- | :--- | :--- |
| 100 | 20,00 € | 20,00 € |
| 80 (entspricht einem Rabatt) | 20,00 € | 16,00 € |
| 150 (entspricht einem Aufschlag) | 20,00 € | 30,00 € |

**Stufe ab Menge 2 ... 10, bis Menge 2 ... 10**
Eingabe der Grenzmenge pro Stufe. Je nach Preisart wird ab Menge oder bis Menge angezeigt. Die Felder sind gesperrt, wenn als Preisart Einzelpreis gewählt ist.
*   **ab Menge:** Der angegebene Preis wird berechnet, wenn im Auftrag die Menge größer oder gleich dem Grenzwert ist.
*   **bis Menge:** Der angegebene Preis wird berechnet, wenn im Auftrag die Menge kleiner oder gleich dem Grenzwert ist.
Der Grenzwert wird je nach Preisart als Stückzahl, als Menge pro Grundmengeneinheit oder als Kantenlänge interpretiert.
*Technische Info: numerische Felder, DB-Felder: kufarbprs.me2, kufarbprs.me3, ... kufarbprs.me10*

**Preis**
Angabe des Einzelpreises. Dieser Preis wird berechnet, wenn als Preisart Einzelpreis definiert ist oder wenn die Maße der Auftragsposition die Maß- oder Mengenangaben aller anderen Preisstufen unterschreiten. Das Feld ist bei der Preisart Mengenstaffel/Gebindegröße gesperrt.
*Technische Info: numerisches Feld, DB-Feld: kufarbprs.peis1*
*Technische Info: numerische Felder, DB-Felder: kufarbprs.preis2, kufarbprs.preis3, ... kufarbprs.preis10*

**Erfasser, Erfassungsdatum**
Anzeige des Erfassers und des Erfassungs- oder Änderungsdatums.

**Kondition gültig von ..., bis ...**
Angabe des Datums, ab dem und bis zu dem die Konditionen gültig sind.
*Technische Info: Datumsfeld, DB-Feld: kufarbprs.vondat, kufarbprs.abdat*

> **Ablauf der Gültigkeit**
> Wenn das Enddatum erreicht ist, werden für die Preisberechnung die allgemeinen Preise und Konditionen herangezogen. Die marktpartnerspezifischen Variantenpreise müssen Sie neu definieren, wenn Sie weiterhin mit diesen Konditionen arbeiten wollen.

## Sprossenpreise

**Stammdaten > Konditionen > Spezielle Preise > Sprossenpreise**

In diesem Dialog legen Sie marktpartnerspezifische Sprossenpreise fest. In der Detailansicht legen Sie die Bedingungen für die Preisberechnung fest, z. B. Mindestlaufmeter, Mindestfeldanzahl.

Diese Sprossenpreise haben eine höhere Priorität als die Sprossenpreise aus den Sprossenpreisklassen.
⇨ "Sprossenpreisklassen" auf Seite C-703

Zu diesem Dialog stehen folgende Ansichten zur Verfügung:
*   "Sprossenpreise – Übersicht" auf Seite C-925
*   "Sprossenpreise – Details" auf Seite C-928

### Sprossenpreise – Übersicht

**Stammdaten > Konditionen > Spezielle Preise > Sprossenpreise**

*[Screenshot of "Sprossenpreise" overview dialog window. It shows a table with columns for Artikel, ab PLKZ, Berechnungsart, Laufmeter, Kreuz, Rand, and Felder.]*
**Abb. C-211 Sprossenpreise – Übersicht**

In dieser Übersicht pflegen Sie die marktpartnerspezifischen Sprossenpreise. Diese Sprossenpreise haben eine höhere Priorität als die Sprossenpreise aus den Sprossenpreisklassen.
⇨ "Sprossenpreisklassen" auf Seite C-703

`<F2>` Wechsel zur Detailansicht.
⇨ "Sprossenpreise - Details" auf Seite C-928

### Feldbeschreibungen (Überblick)

> **Kunden und Lieferanten in den Konditionen**
> Kunden und Lieferanten, für die eine Kondition gilt, bezeichnen im Folgenden immer den jeweiligen Konditionsdebitor aus den Marktpartnerstammdaten.

**Konditionsart**
Auswahl, für wen die Konditionen gelten:
*   **Kunde:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für einen bestimmten Kunden.
*   **Lieferant:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für einen bestimmten Lieferanten.
*   **Objekt-Verkauf:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für ein bestimmtes Verkaufsobjekt.
*   **Objekt-Einkauf:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für ein bestimmtes Einkaufsobjekt.
*   **Kond.-Branche:** Die Konditionen gelten für die Berechnung von Preisen für eine bestimmte Marktpartnergruppe. Marktpartner, für die gemeinsame Konditionen gelten sollen, müssen einer Branche zugeordnet sein.
*Technische Info: numerisches Feld, Toggle-Feld, DB-Feld: kuspropr.kondkz*

**Marktpartner**
Auswahl des Marktpartners, für den die Konditionen gelten. Je nach Konditionsart können Sie einen Kunden, einen Lieferanten, ein Objekt oder eine Kundengruppe angeben.
*Technische Info: numerisches Feld, DB-Feld: kuspropr.kunr*

**Artikel, Bezeichnung**
Auswahl des Sprossenartikels, für den der marktpartnerspezifische Preis gilt.
*Technische Info: numerisches Feld, DB-Feld: kuspropr.artnr*

**Ab PLKZ**
Auswahl des Preislistenkennzeichens (PLKZ) des Positionsartikels, ab dem die Sprossenpreisdaten gelten. Findet A+W Enterprise im Auftrag für den Artikel keine Preise zum aktuellen PLKZ, wird das numerisch vorausgehende PLKZ ermittelt, zu dem Preisdaten definiert sind.
⇨ Tutorial, "Ab-PLKZ-Logik" auf Seite C-560
*Technische Info: numerisches Feld, DB-Feld: kuspropr.plkz*

**Berechnungsart, Bezeichnung**
Auswahl der Berechnungsart, nach der die Sprossenpreise berechnet werden:
*   **1 - Felder:** Der Preis wird pro Feld berechnet.
*   **2 - LM+K+R:** Der Preis wird pro laufendem Meter, pro Kreuz und pro Randanschluss berechnet.
*   **3 - LM:** Der Preis wird pro laufendem Meter berechnet.
*   **4 - LM+K:** Der Preis wird pro laufendem Meter und pro Kreuz berechnet.
*   **5 - LM+R:** Der Preis wird pro laufendem Meter und pro Randanschluss berechnet.
*   **6 - K:** Der Preis wird pro Kreuz berechnet.
*   **7 - K+R:** Der Preis wird pro Kreuz und pro Randanschluss berechnet.
*   **8 - R:** Der Preis wird pro Randanschluss berechnet.
*   **9 - Spezial:** Diese Form der Berechnung ist kundenindividuell konfiguriert.
*   **10 - Prozent:** Der Preis wird prozentual aus dem Grundpreis des Kopfartikels berechnet. Der Prozentsatz wird in der Detailansicht im Feld Prozent angegeben.
*   **11 - qm-Preis:** Der Preis wird pro Quadratmeter des Glases berechnet. Der Preis wird in der Detailansicht im Feld Qm-Preis angegeben.
*   **12 - Feld+LM:** Der Preis wird pro Feld und pro laufendem Meter berechnet.
*   **13 - Stück:** Für den Sprossenaufbau wird ein Gesamtpreis berechnet. Der Preis wird in der Detailansicht im Feld Stückpreis angegeben.
*   **14 - K oder LM:** Der Preis wird pro Kreuz oder pro laufendem Meter berechnet.
    *   Wenn sich im Sprossenaufbau Kreuzungspunkte ergeben, werden die Sprossen nach Anzahl der Kreuze berechnet.
    *   Wenn keine Kreuzungspunkte vorhanden sind, werden die Sprossen nach laufenden Metern berechnet.
*   **15 - Feld+K+R:** Der Preis wird pro Feld, pro Kreuz und pro Randanschluss berechnet.
Wenn in den Konditionen eine andere Berechnungsart angegeben ist, gelten die Preise aus den Konditionen.
*Technische Info: numerisches Feld, alphanumerisches Feld, DB-Feld: kuspropr.berart*

**Laufmeter**
Angabe des Preises pro laufendem Meter. Der Preis wird bei den Berechnungsarten LM, LM+K+R, LM+K, LM+R, Feld+LM und Spezial ausgewertet. Im Auftrag wird der Preis aus der Gesamtlänge der Sprossen berechnet.
*Technische Info: numerisches Feld, DB-Feld: kuspropr.plm*

**Kreuz**
Angabe des Preises pro Kreuzungspunkt. Der Preis wird bei den Berechnungsarten K, K+R, LM+K, LM+K+R, K oder LM, Feld+K+R und Spezial ausgewertet. Im Auftrag wird der Preis nach der Anzahl der Kreuzungspunkte berechnet. Wenn in einer Scheibe 2 verschiedene Sprossenartikel eingebaut werden, wird der Preis mit dem Kreuzpreis der ersten Sprosse ermittelt.
*Technische Info: numerisches Feld, DB-Feld: kuspropr.pkr*

**Rand**
Angabe des Preises pro Randanschluss. Der Preis wird bei den Berechnungsarten R, LM+K+R, LM+R, K+R, Feld+K+R und Spezial ausgewertet. Im Auftrag wird der Preis aus der Anzahl der Randanschlüsse berechnet.
*Technische Info: numerisches Feld, DB-Feld: kuspropr.pra*

**Felder**
Angabe des Preises pro Feld. Der Preis wird bei den Berechnungsarten Felder, Feld+LM, Feld+K+R und Spezial ausgewertet. Im Auftrag wird der Preis nach der Anzahl der Felder berechnet. Wenn in einer Scheibe 2 verschiedene Sprossenartikel eingebaut werden, wird der Preis mit dem Feldpreis der ersten Sprosse ermittelt.
*Technische Info: numerisches Feld, DB-Feld: kuspropr.pfe*

### Sprossenpreise – Details

**Stammdaten > Konditionen > Spezielle Preise > Sprossenpreise > `<F2>`**

*[Screenshot of "Sprossenpreise - Details" dialog window. It shows detailed price fields for Laufmeter, Kreuz, Rand, Felder, Prozent, Qm-Preis, Stückpreis, etc.]*
**Abb. C-212 Sprossenpreise – Details**

In diesem Dialog legen Sie die Bedingungen für die Berechnung von Sprossenpreisen fest, z. B für die Berechnungsart Prozent oder Spezial.

`<F2>` Wechsel zur Übersicht.
⇨ "Sprossenpreise – Übersicht" auf Seite C-925

#### Feldbeschreibungen (Details)

Die Felder im Kopfbereich sind zum Dialog Sprossenpreise – Übersicht beschrieben:
⇨ "Sprossenpreise – Übersicht" auf Seite C-925

Zusätzlich werden die folgenden Felder angezeigt:

**Felder2**
Angabe des Preises pro Feld, wenn im Sprossenaufbau keine Kreuzungspunkte vorhanden sind. Der Preis wird bei der Berechnungsart 9 - Spezial ausgewertet.
*Technische Info: numerisches Feld, DB-Feld: kuspropr.pfe2*

**Prozent**
Angabe des Prozentsatzes. Der Preis wird bei den Berechnungsarten Prozent und Spezial ausgewertet. Im Auftrag wird der Preis aus dem Stückpreis des Kopfartikels inklusive aller Bearbeitungen berechnet.
*Technische Info: numerisches Feld, DB-Feld: kuspropr.prozent*

**Qm-Preis**
Angabe des Quadratmeterpreises. Der Preis wird bei der Berechnungsart qm-Preis ausgewertet. Im Auftrag wird der Preis aus der Anzahl der Quadratmeter der ISO-Einheit berechnet.
*Technische Info: numerisches Feld, DB-Feld: kuspropr.qmpreis*

**Stückpreis**
Angabe des Stückpreises. Der Preis wird bei der Berechnungsart Stück ausgewertet. Im Auftrag wird der Stückpreis für den Sprossenaufbau insgesamt berechnet.
*Technische Info: numerisches Feld, DB-Feld: kuspropr.stckpreis*

**Mindestlaufmeter ... m**
Angabe der Sprossenlänge in Meter, für die der Preis mindestens berechnet wird. Der Preis wird bei der Berechnungsart LM ausgewertet. Im Auftrag wird der Preis für diese Sprossenlänge berechnet, wenn die tatsächliche Sprossenlänge insgesamt kleiner ist als dieser Wert. Wenn Sie die Mindestlaufmeter-Berechnung auf Sprossenteilstücke über die Umgebungsvariable MINBER_AUF_TEILSPROSSE entsprechend konfigurieren, wird dieser Wert für jede einzelne Sprosse ausgewertet.
*Technische Info: numerisches Feld, DB-Feld: kuspropr.minlm*

**Mindestfeldanzahl ... Stück**
Angabe der Sprossenfelder, für die der Preis mindestens berechnet wird. Der Preis wird bei den Berechnungsarten Feld ausgewertet. Im Auftrag wird der Preis für diese Anzahl von Feldern berechnet, wenn die tatsächliche Feldanzahl kleiner ist als der eingetragene Wert.
*Technische Info: numerisches Feld, DB-Feld: kuspropr.minfeld*

**Erfasser, Erfassungsdatum**
Anzeige des Erfassers und des Erfassungs- oder Änderungsdatums.

**Kondition gültig von ..., bis...**
Angabe des Datums, ab dem und bis zu dem die Konditionen gültig sind.
*Technische Info: Datumsfeld, DB-Feld: kuspropr.vondat, kuspropr.abdat*

> **Ablauf der Gültigkeit**
> Wenn das Enddatum erreicht ist, werden für die Preisberechnung die allgemeinen Preise und Konditionen herangezogen. Die marktpartnerspezifischen Sprossenpreise müssen Sie neu definieren, wenn Sie weiterhin mit diesen Konditionen arbeiten wollen.

## Bearbeitungspreise

**Stammdaten > Konditionen > Spezielle Preise > Bearbeitungspreise**

In diesem Dialog legen Sie Bearbeitungspreise für Marktpartner, Objekte oder Branchen an. In der Detailansicht legen Sie die Bedingungen für die Preisberechnung fest, z. B. Preisstaffeln, Mindestberechnungsmenge, Zuschläge.

Diese Bearbeitungspreise haben eine höhere Priorität als die Preise aus den Bearbeitungsvektoren.
⇨ "Bearbeitungsvektoren" auf Seite C-760

Zu diesem Dialog stehen folgende Ansichten zur Verfügung:
*   "Bearbeitungspreise – Übersicht" auf Seite C-930
*   "Bearbeitungspreise - Details" auf Seite C-934

### Bearbeitungspreise – Übersicht

**Stammdaten > Konditionen > Spezielle Preise > Bearbeitungspreise**

*[Screenshot of "Bearbeitungspreise" overview dialog window. It shows a table with columns for Artikel, ab PLKZ, bis Dicke, ab Menge, Berechnungsart, Preistyp, and Preis 1.]*
**Abb. C-213 Bearbeitungspreise – Übersicht**

In dieser Übersicht pflegen Sie die marktpartnerspezifischen Bearbeitungspreise.

`<F2>` Wechsel zur Detailansicht.
⇨ "Bearbeitungspreise - Details" auf Seite C-934

### Feldbeschreibungen

> **Kunden und Lieferanten in den Konditionen**
> Kunden und Lieferanten, für die eine Kondition gilt, bezeichnen im Folgenden immer den jeweiligen Konditionsdebitor aus den Marktpartnerstammdaten.

**Konditionsart**
Auswahl, für wen die Konditionen gelten:
*   **Kunde:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für einen bestimmten Kunden.
*   **Lieferant:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für einen bestimmten Lieferanten.
*   **Objekt-Verkauf:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für ein bestimmtes Verkaufsobjekt.
*   **Objekt-Einkauf:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für ein bestimmtes Einkaufsobjekt.
*   **Kond.-Branche:** Die Konditionen gelten für die Berechnung von Preisen für eine bestimmte Marktpartnergruppe. Marktpartner, für die gemeinsame Konditionen gelten sollen, müssen einer Branche zugeordnet sein.
*Technische Info: numerisches Feld, Toggle-Feld, DB-Feld: kubeapr.kondkz*

**(Marktpartner)**
Auswahl des Marktpartners, für den die Konditionen gelten. Je nach Konditionsart können Sie einen Kunden, einen Lieferanten, ein Objekt oder eine Kundengruppe angeben.
*Technische Info: numerisches Feld, DB-Feld: kubeapr.kunr*

**Artikel**
Auswahl des Artikels, für den die marktpartnerspezifischen Bearbeitungspreise gelten.
*Technische Info: numerisches Feld, DB-Feld: kubeapr.artnr*

> **Vektorbezogene Bearbeitungspreise**
> Wenn Sie die marktpartnerspezifischen Bearbeitungspreise pro Bearbeitungsvektor hinterlegen, kann Ihr System dafür explizit konfiguriert werden. In solcher Konfiguration müssen Sie im Feld Artikel die Nummer des Bearbeitungsvektors manuell eingeben. Bei Interesse wenden Sie sich bitte an den Mitarbeiter der A+W Software GmbH.

**Ab PLKZ**
Auswahl des Preislistenkennzeichens (PLKZ), ab dem die Preisdaten gelten.
Findet A+W Enterprise im Auftrag für den Artikel keine Preise zum aktuellen PLKZ, wird das numerisch vorausgehende PLKZ ermittelt, zu dem Preisdaten definiert sind.
⇨ Tutorial, "Ab-PLKZ-Logik" auf Seite C-560
*Technische Info: numerisches Feld, DB-Feld: kubeapr.plkz*

**Bis Dicke**
Angabe der Dicke in Millimetern, bis zu der die Preisangaben gelten. Die Dicke bezieht sich auf den Artikel, an dem die Bearbeitung in der Stückliste angebracht ist.
*Technische Info: numerische Feld, DB-Feld: kubeapr.dicke*

**Ab Menge**
Eingabe der Grenzmenge, ab der die Preisangaben berücksichtigt werden. Für die Mengen bis zum Erreichen der Grenzmenge gilt der allgemeine Bearbeitungspreis. Die Menge bezieht sich auf die Grundmengeneinheit (GME), die dem Bearbeitungsartikel in den Stammdaten zugewiesen ist, z. B. Fläche, Stück, Länge.
*Technische Info: numerische Feld, DB-Feld: kubeapr.menge*

**Berechnungsart**
Auswahl der Berechnungsart, nach der die Bearbeitungspreise gestaffelt werden:
*   **Stufe 1:** Der Preis aus dem Feld Stufe 1 wird als Bearbeitungspreis herangezogen.
*   **Fläche:** Der Preis wird nach der Fläche des Glases (nach Maßrundung, ohne Mindestberechnung) gestaffelt. Wenn die Fläche größer oder gleich der angegebenen Grenzmenge ist, wird der entsprechende Staffelpreis als Bearbeitungspreis herangezogen.
*   **Längere Kante:** Der Preis wird nach der längsten Kante (nach Maßrundung) gestaffelt. Wenn die längste Kante größer oder gleich der angegebenen Grenzmenge ist, wird der entsprechende Staffelpreis als Bearbeitungspreis herangezogen.
*   **Umfang:** Der Preis wird nach dem Umfang des Glases (nach Maßrundung) gestaffelt. Wenn der Umfang größer oder gleich der angegebenen Grenzmenge ist, wird der entsprechende Staffelpreis als Bearbeitungspreis herangezogen.
*   **Staffelstufe:** Der Preis der Preisstufe, die in den Konditionen angegeben ist, wird als Bearbeitungspreis herangezogen.
*   **Fläche/Position:** Der Preis wird nach der Fläche des Glases (nach Maßrundung, ohne Mindestberechnung) pro Position gestaffelt. Dazu wird die Fläche des Glases nach der Maßrundung berechnet und mit der Stückzahl aus der Position multipliziert. Wenn die berechnete Gesamtfläche größer oder gleich der angegebenen Grenzmenge ist, wird der entsprechende Staffelpreis als Bearbeitungspreis herangezogen.
*   **2 Kanten:** Der Preis wird abhängig von den zwei Kantenlängen gestaffelt. Die zwei Kantenlängen werden mit den hinterlegten Grenzwerten verglichen. Dabei wird die kürzere Kante mit dem kleineren Grenzmaß und die längere Kante mit dem größeren Grenzmaß aus dem Bearbeitungsvektor verglichen. Wenn eine der beiden Kantenlängen in einer höheren Preisstufe liegt als die andere, wird der Staffelpreis der entsprechend höheren Preisstufe als Bearbeitungspreis herangezogen.
*   **Stück/Position:** Der Preis wird nach der Anzahl der Scheiben pro Position gestaffelt. Wenn die Gesamtstückzahl der Position größer oder gleich der angegebenen Grenzmenge ist, wird der entsprechende Staffelpreis als Bearbeitungspreis herangezogen.
*Technische Info: alphanumerisches Feld, Toggle-Feld, DB-Feld: kubeapr.berart*

**Preistyp**
Angabe, worauf sich der angegebene Preis bezieht:
*   **WE/Stück:** Im Auftrag wird der Preis als fester Betrag pro Stück in der Position berechnet.
*   **WE/GME:** Der Preis wird pro Grundmengeneinheit berechnet, die in den Artikelstammdaten hinterlegt ist, z. B. pro Stück, lfm (laufendem Meter).
*   **Prozent:** Der Preis wird prozentual aus dem Glasgrundpreis errechnet.
*   **WE/qm:** Der Preis wird pro Quadratmeter berechnet.
*   **WE/lm:** Der Preis wird pro laufendem Meter berechnet.
*Technische Info: alphanumerisches Feld, Toggle-Feld, DB-Feld: kubeapr.ptyp*

**Preis 1**
Angabe des Einzelpreises. Dieser Preis wird im Auftrag herangezogen, wenn keine Staffelung definiert ist oder wenn die Maße des Artikels die Mengenangaben der definierten Preisstufen unterschreiten. In der Detailansicht kann dazu eine Mindestberechnungsmenge angegeben werden.
*Technische Info: numerisches Feld, DB-Feld: kubeapr.preis1*

### Bearbeitungspreise – Details

**Stammdaten > Konditionen > Spezielle Preise > Bearbeitungspreise > `<F2>`**

*[Screenshot of "Bearbeitungspreise - Details" dialog window. It shows header information and a table for price scaling (Stufe, ab Menge, Preis).]*
**Abb. C-214 Bearbeitungspreise – Details**

In diesem Dialog legen Sie Bedingungen für die Berechnung von marktpartnerspezifischen Bearbeitungspreisen fest. Zusätzlich können Sie Staffelpreise für den gewählten Bearbeitungsartikel angeben.

`<F2>` Wechsel zur Übersicht.
⇨ "Bearbeitungspreise – Übersicht" auf Seite C-930

#### Feldbeschreibungen (Details)

Die Felder im Kopfbereich sind zum Dialog Bearbeitungspreise – Übersicht beschrieben:
⇨ "Bearbeitungspreise – Übersicht" auf Seite C-930

Zusätzlich werden die folgenden Felder angezeigt:

**Zuschlagsmatrix**
Auswahl einer Zuschlagsmatrix für einen allgemeinen Zuschlag auf den Bearbeitungspreis.
⇨ "Zuschlagsmatrizen" auf Seite C-814
Sie können auch eine Zuschlagsmatrix der Art Glasgrundpreis zuordnen. Damit wird der Zuschlag nicht auf den Bearbeitungspreis erhoben, sondern auf den Glaspreis.
*Technische Info: numerisches Feld, DB-Feld: kubeapr.zumatnr*

**Mindestberechnung ... GME**
Angabe der Menge in Grundmengeneinheiten, die mindestens berechnet wird. Die Grundmengeneinheit wird aus den Artikelstammdaten ermittelt. Wenn die preisrelevante Menge in der Auftragsposition kleiner ist als die definierte Mindestmenge, wird der Preis für diese Mindestmenge berechnet.
⇨ Tutorial, "Preisrelevante Menge" auf Seite C-571
*Technische Info: numerisches Feld, DB-Feld: kubeapr.minber*

**Faktor...%**
Angabe eines Faktors, mit dem der marktpartnerspezifische Bearbeitungspreis multipliziert wird. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preisstufen anpassen zu müssen, z. B. für eine Preiserhöhung oder einen marktpartnerspezifischen Rabatt. Wenn Sie das Feld leer lassen, gilt entsprechend der Konditionshierarchie der Faktor aus den Konditionen.
*Technische Info: numerisches Feld, DB-Feld: kubeapr.faktor*

**Beispiel**

| Faktor | Grundpreis | Endpreis |
| :--- | :--- | :--- |
| 100 | 20,00 € | 20,00 € |
| 80 (entspricht einem Rabatt) | 20,00 € | 16,00 € |
| 150 (entspricht einem Aufschlag) | 20,00 € | 30,00 € |

**Stufe ab Menge**
Eingabe der Grenzmenge pro Stufe. Die Felder werden für alle Berechnungsarten außer 2 Kanten angezeigt. Der Grenzwert wird je nach Berechnungsart als Stückzahl, als Fläche oder als Kantenlänge interpretiert. Der angegebene Preis wird herangezogen, wenn im Auftrag die Menge größer oder gleich dem Grenzwert ist.
*Technische Info: numerische Felder, DB-Felder: kubeapr.me2, kubeapr.me3, ..., kubeapr.me10*

**Stufe bis Menge**
Eingabe der Grenzmengen pro Stufe. Die Felder werden nur für die Berechnungsart 2 Kanten angezeigt. Pro Stufe müssen Sie zwei Grenzmengen für die beiden Kanten angeben. Der angegebene Preis wird herangezogen, wenn im Auftrag die Menge kleiner oder gleich der angegebenen Grenzwerte ist.
*Technische Info: numerische Felder, DB-Felder: kubeapr.me1, kubeapr.mas2_1, kubeapr.me2, kubeapr.mas2_2, ... kubeapr.me10, kubeapr.mas2_10*

**(Maße)**
Angabe des Grenzwerts in mm pro Stufe. Diese Felder sind nur freigeschaltet, wenn als Berechnungsart 11 Variantenartig oder 12 Variantenstaffel gewählt ist. Wenn im Auftrag die Kantenlängen des Artikels größer oder gleich den Grenzwerten sind, gilt der Preis dieser Preisstufe.
*Technische Info: numerische Felder, DB-Felder: kubeapr.mas2_1, kubeapr.mas2_2, ... kubeapr.mas2_10*

**Preis**
Angabe des Preises pro Preisstufe. Wenn Berechnungsart Stufe 1 gewählt ist, wird nur der Preis aus dem Feld Stufe 1 verwendet.
*Technische Info: numerische Felder, DB-Felder: kubeapr.preis2, kubeapr.preis3, ... kubeapr.preis10*

**Erfasser, Erfassungsdatum**
Anzeige des Erfassers und des Erfassungs- oder Änderungsdatums.

**Kondition gültig von ..., bis ...**
Angabe des Datums, ab dem und bis zu dem die Konditionen gültig sind.
*Technische Info: Datumsfeld, DB-Feld: kubeapr.vondat, kubeapr.abdat*

> **Ablauf der Gültigkeit**
> Wenn das Enddatum erreicht ist, werden für die Preisberechnung die allgemeinen Preise und Konditionen herangezogen. Die marktpartnerspezifischen Bearbeitungspreise müssen Sie neu definieren, wenn Sie weiterhin mit diesen Konditionen arbeiten wollen.

## ISO-Austauschpreise

**Stammdaten > Konditionen > Spezielle Preise > ISO-Austauschpreise**

In diesem Dialog legen Sie ISO-Austauschpreise für Marktpartner, Objekte oder Branchen an. In der Detailansicht legen Sie die Bedingungen für die Preisberechnung fest, z. B. Mindestberechnungsmenge, Maßrundung, Kleinglaszuschläge und Überlängenzuschläge.

Diese Austauschpreise haben eine höhere Priorität als die allgemeinen Austauschpreise.
⇨ “ESG/VSG/Sonder Austauschpreise" auf Seite C-737

Zu diesem Dialog stehen folgende Ansichten zur Verfügung:
*   "ISO-Austauschpreise – Übersicht" auf Seite C-937
*   "ISO-Austauschpreise - Details" auf Seite C-940

### ISO-Austauschpreise – Übersicht

**Stammdaten > Konditionen > Spezielle Preise > ISO-Austauschpreise**

*[Screenshot of "Austauschpreise" overview dialog window. It shows a table with columns for Artikel, Austauschliste, ab PLKZ, ab Stück, Faktor, and Preis 1.]*
**Abb. C-215 Austauschpreise – Übersicht**

In dieser Übersicht pflegen Sie die Austauschpreise für ESG, VSG und Float-Gläser, die in eine ISO-Scheibe eingebaut werden sollen. Diese Preise gelten jeweils für einen Marktpartner, ein Objekt oder eine Branche. Diese Austauschpreise haben eine höhere Priorität als die allgemeinen Austauschpreise.

`<F2>` Wechsel zur Detailansicht.
⇨ "ISO-Austauschpreise - Details" auf Seite C-940

### Feldbeschreibungen

> **Kunden und Lieferanten in den Konditionen**
> Kunden und Lieferanten, für die eine Kondition gilt, bezeichnen im Folgenden immer den jeweiligen Konditionsdebitor aus den Marktpartnerstammdaten.

**Konditionsart**
Auswahl, für wen die Konditionen gelten:
*   **Kunde:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für einen bestimmten Kunden.
*   **Lieferant:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für einen bestimmten Lieferanten.
*   **Objekt-Verkauf:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für ein bestimmtes Verkaufsobjekt.
*   **Objekt-Einkauf:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für ein bestimmtes Einkaufsobjekt.
*   **Kond.-Branche:** Die Konditionen gelten für die Berechnung von Preisen für eine bestimmte Marktpartnergruppe. Marktpartner, für die gemeinsame Konditionen gelten sollen, müssen einer Branche zugeordnet sein.
*Technische Info: numerisches Feld, Toggle-Feld, DB-Feld: kuaustpr.kondkz*

**Marktpartner**
Auswahl des Marktpartners, für den die Konditionen gelten. Je nach Konditionsart können Sie einen Kunden, einen Lieferanten, ein Objekt oder eine Kundengruppe angeben.
*Technische Info: numerisches Feld, DB-Feld: kuaustpr.kunr*

**Artikel, Bezeichnung**
Auswahl des Austauschglases, für den die marktpartnerspezifischen Austauschpreise gelten.
*Technische Info: numerisches Feld, DB-Feld: kuaustpr.artnr*

**Austauschliste, Bezeichnung**
Auswahl der Austauschliste, für die die marktpartnerspezifischen Austauschpreise gelten.
*Technische Info: alphanumerische Felder, DB-Feld: kuaustpr.atinr*

**Ab PLKZ**
Auswahl des Preislistenkennzeichens (PLKZ), ab dem die Preisdaten gelten.
Findet A+W Enterprise im Auftrag für den Artikel keine Preise zum aktuellen PLKZ, wird das numerisch vorausgehende PLKZ ermittelt, zu dem Preisdaten definiert sind.
⇨ Tutorial, "Ab-PLKZ-Logik" auf Seite C-560
*Technische Info: numerisches Feld, DB-Feld: kuaustpr.plkz*

**Ab Stück**
Grenzmenge in Stück, ab der die Preisinformationen gelten. Die Daten aus diesem Dialog werden dann für die Preisberechnung herangezogen, wenn die Anzahl der Scheiben in der Position im Vorgang bei der Positionserfassung größer oder gleich der angegebenen Stückzahl ist.
*Technische Info: numerisches Feld, DB-Feld: kuaustpr.stueckzahl*

**Faktor %**
Angabe eines Faktors, mit dem der marktpartnerspezifische Austauschpreis multipliziert wird. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für eine Preiserhöhung oder einen Rabatt. Wenn Sie das Feld leer lassen, gilt entsprechend der Konditionshierarchie der Faktor aus den Konditionen.
*Technische Info: numerisches Feld, DB-Feld: kuaustpr.faktor*

**Beispiel**

| Faktor | Grundpreis | Endpreis |
| :--- | :--- | :--- |
| 100 | 20,00 € | 20,00 € |
| 80 (entspricht einem Rabatt) | 20,00 € | 16,00 € |
| 150 (entspricht einem Aufschlag) | 20,00 € | 30,00 € |

**Preis 1**
Angabe des Einzelpreises für das Austauschglas, der ab der angegebenen Stückzahl gilt. Wenn im Auftrag die Menge nicht erreicht ist, werden die allgemeinen Austauschpreise und Konditionen herangezogen.
*Technische Info: numerisches Feld, DB-Feld: kuaustpr.preis1*

### ISO-Austauschpreise – Details

**Stammdaten > Konditionen > Spezielle Preise > ISO-Austauschpreise > `<F2>`**

*[Screenshot of "Austauschpreise - Details" dialog window. It shows fields for Mindestberechnung, Maßrundung, Kleinglaszuschläge, Überlängenzuschläge and scaled pricing.]*
**Abb. C-216 Austauschpreise – Details**

In diesem Dialog legen Sie Bedingungen für die Berechnung von ISO-Austauschpreisen fest, z. B. Preisstaffeln, Mindestberechnungsflächen, Maßrundungen, Zuschläge.

`<F2>` Wechsel zur Übersicht.
⇨ "ISO-Austauschpreise - Übersicht" auf Seite C-937

#### Feldbeschreibungen (Details)

Die Felder im Kopfbereich sind zum Dialog Austauschpreise – Übersicht beschrieben:
⇨ “ISO-Austauschpreise - Übersicht" auf Seite C-937

Zusätzlich werden die folgenden Felder angezeigt:

**Mindestberechnung ... ME**
Angabe der Mindestmenge, für die der Preis berechnet wird. Die Mindestmenge wird entsprechend der Grundmengeneinheit im Artikelstamm angegeben, z. B. Fläche in qm. Wenn die Fläche des Glases in der Auftragsposition kleiner ist als die Mindestberechnung, wird der Preis für diese Mindestberechnung berechnet. Abhängig von der Konfiguration kann die Berechnung des Austauschpreises auf den Kopfartikel oder auf den Austauschartikel bezogen sein.
*   Wenn die Variable `MINBER_AUSTAUSCH_OHNE_MAX` aktiv ist, wird für Artikel mit der Preismethode ISO-Aktuell nur die Mindestberechnungseinheit ausgewertet.
*   Wenn die Variable `MINBER_AUSTAUSCH_OHNE_MAX` nicht aktiv ist, wird für Artikel mit der Preismethode ISO-Aktuell die Mindestberechnung von Grundartikel und Austauschartikel herangezogen und die größere der beiden Berechnungen ausgewertet.

Unabhängig von dieser Einstellung wird immer der höhere Preis berechnet.
⇨ Tutorial, "Preisrelevante Menge" auf Seite C-571
*Technische Info: numerisches Feld, DB-Feld: kuaustpr.minber*

**Maßrundung**
Angabe der Maßrundung in mm für die Preisberechnung des Artikels, z. B. 30 mm. Für die Preisberechnung werden die Höhe und die Breite der Auftragsposition auf die nächsthöhere Länge in mm aufgerundet, die durch die angegebene Maßrundung teilbar ist.
*Technische Info: numerisches Feld, DB-Feld: kuaustpr.massrund*

**Beispiel**
Als Maßrundung ist 30 mm definiert.
Der erfasste ISO-Artikel hat die Maße 1000 × 1000 mm. Die nächste durch 30 mm teilbare Kantenlänge ist 1020 mm.
Der Preis wird aus den Maßen 1020 × 1020 mm = 1,04 qm berechnet.

**Berechnungsart**
Auswahl der Berechnungsart, nach der die Austauschpreise gestaffelt werden:
*   **Fläche:** Der Preis wird nach der Fläche des Glases (nach Maßrundung, ohne Mindestberechnung) gestaffelt. Wenn die Fläche größer oder gleich der angegebenen Grenzmenge ist, wird der Staffelpreis als Austauschpreis herangezogen.
*   **1 Kante:** Der Preis wird nach der Länge der Kante (nach Maßrundung) gestaffelt. Wenn die längste Kante größer oder gleich der angegebenen Grenzmenge ist, wird der Staffelpreis als Austauschpreis herangezogen.
*   **2 Kanten:** Der Preis wird abhängig von den zwei Kantenlängen gestaffelt. Die zwei Kantenlängen werden mit den hinterlegten Grenzwerten verglichen. Dabei wird die kürzere Kante mit dem 1. Maß und die längere Kante mit dem 2. Maß verglichen. Standardmäßig wird der Austauschpreis der jeweiligen Stufe nur herangezogen, wenn beide Maße die Grenzwerte überschreiten. Wenn die Variable `ISOAUST_2KANTEN_BIS` aktiv ist, wird der Austauschpreis auch herangezogen, wenn nur ein Grenzmaß überschritten ist.
*   **Matrix:** Der Preis wird nach der zugeordneten Matrix gestaffelt. Die Matrix ordnen Sie im Feld Matrix zu. Standardmäßig wird als Austauschpreis ein Mischpreis aus (Glasgrundpreis + Matrixpreis) / 2 - Glasgrundpreis berechnet. Wenn die Variable `ISOAUST_KEINE_MISCHMATRIX` mit dem Wert ON aktiv ist, wird der Staffelpreis aus der entsprechenden Matrix direkt als Austauschpreis herangezogen.
*   **Prozent:** Der Preis wird nach der Fläche des Glases (nach Maßrundung, ohne Mindestberechnung) gestaffelt. Wenn die Fläche größer oder gleich der angegebenen Grenzmenge ist, wird der Staffelpreis als Austauschpreis herangezogen. Der Preis wird prozentual aus dem Grundpreis des Kopfartikels errechnet und addiert.
*Technische Info: alphanumerisches Feld, Toggle-Feld, DB-Feld: kuaustpr.berechart*

**Matrix**
Angabe der Matrix, die zur Berechnung herangezogen wird. Das Feld wird nur angezeigt, wenn Sie als Berechnungsart Matrix angegeben haben. Die Felder für die Maßstufen und die Staffelpreise sind dann gesperrt.
*Technische Info: numerisches Feld, DB-Feld: kuaustpr.matrix*

**Abmessungen**
**Ab...** Angabe der Grenzwerte für Staffelpreise. Der Preis einer Stufe gilt so lange, bis der nächsthöhere Wert erreicht ist. Je nach der gewählten Berechnungsart müssen Sie die Werte in folgenden Maßeinheiten eingeben:
*   **Fläche:** Anzahl der Quadratmeter, ab denen der zugeordnete Preis herangezogen wird.
*   **Kante:** Anzahl der Millimeter, ab denen der zugeordnete Preis berechnet wird.
*   **Prozent:** Anzahl der Fläche in Prozent, ab der der zugeordnete Preis berechnet wird.
*   **Matrix:** Die Preise werden nach der zugeordneten Matrix berechnet. Die Felder für die Grenzwerte und die Preise sind gesperrt.
*Technische Info: numerische Felder, DB-Felder: kuaustpr.grenz21, kuaustpr.grenz31, kuaustpr.grenz41, kuaustpr.grenz51*

**Preis 2-5**
Angabe des Preises für die jeweilige Maßstufe. Der Preis gilt so lange, bis der nächsthöhere Wert erreicht ist.
*Technische Info: numerische Felder, DB-Felder: kuaustpr.preis2, kuaustpr.preis3, ... kuaustpr.preis5*

**Kleinglaszuschläge**
**Bis ... qm** Angabe von Grenzwerten für Preiszuschläge. Der Preis wird auf den Preis des Austauschglases aufgeschlagen, wenn die erfasste Fläche kleiner ist als der angegebene Wert, z. B. bis 0,5 qm. Dieser Zuschlag ist z. B. sinnvoll, wenn die Gläser zu klein sind, um sie mit der Maschine zu bearbeiten.
*Technische Info: numerische Felder, DB-Felder: kuaustpr.kleinme1, ... kuaustpr.kleinme4*

**(Wert)**
Angabe des Zuschlags, der aufgeschlagen wird, wenn die Fläche des Austauschglases kleiner ist als der angegebene Grenzwert.
*Technische Info: numerische Felder, DB-Felder: kuaustpr.kleinzu1, ... kuaustpr.kleinzu4*

**(Zuschlagstyp)**
Angabe, worauf sich der angegebene Zuschlag bezieht:
*   **WE/qm:** Der Zuschlag wird pro qm erhoben, z. B. ist bis 0,5 qm ein Preiszuschlag von 10 € pro qm fällig.
*   **Prozent:** Der Zuschlag wird prozentual auf den Preis des Austauschglases aufgeschlagen, z. B. ist bis 0,5 qm ein Preiszuschlag von 10% fällig.
*Technische Info: alphanumerische Felder, Toggle-Felder, DB-Felder: kuaustpr.kleinptyp1, ... kuaustpr.kleinptyp4*

**Überlängenzuschläge**
**Ab ... mm** Angabe von Grenzwerten für prozentuale Preiszuschläge. Der Zuschlag wird prozentual auf den Preis des Austauschglases aufgeschlagen, wenn das erfasste Maß einschließlich Maßrundung größer oder gleich dem angegebenen Maß ist, z. B. ab 2200 mm. Die Angabe bezieht sich unabhängig von der Berechnungsart immer auf die längere Kante.
Wenn die Umgebungsvariable `ISO_UELZUSCHLAG_NUR_AUSTAUSCH` aktiv ist, wird der Überlängenzuschlag für die Preismethode ISO-Aktuell nur auf die Austauschpreise und nicht auf den Grundpreis aufgeschlagen.
*Technische Info: numerische Felder, DB-Felder: kuaustpr.uelme1, kuaustpr.uelme2*

**(Wert) %**
Angabe des Prozentsatzes, der aufgeschlagen wird, wenn eine Kantenlänge des Austauschartikels länger ist als der angegebene Grenzwert.
*Technische Info: numerische Felder, DB-Felder: kuaustpr.uelzu1, kuaustpr.uelzu2*

**Erfasser, Erfassungsdatum**
Anzeige des Erfassers und des Erfassungs- oder Änderungsdatums.

**Kondition gültig von ..., bis ...**
Angabe des Datums, ab dem und bis zu dem die Konditionen gültig sind.
*Technische Info: Datumsfeld, DB-Feld: kuaustpr.vondat, kuaustpr.abdat*

> **Ablauf der Gültigkeit**
> Wenn das Enddatum erreicht ist, werden für die Preisberechnung die allgemeinen Preise und Konditionen herangezogen. Die marktpartnerspezifischen Austauschpreise müssen Sie neu definieren, wenn Sie weiterhin mit diesen Konditionen arbeiten wollen.

## Spezielle Preise für ISO-Einzelscheiben

**Stammdaten > Konditionen > Spezielle Preise > ISO-Einzelscheiben**

In diesem Dialog legen Sie die marktpartnerspezifischen Preise für die Einzelscheiben an, die in ISO-Artikel verbaut werden. Als Einzelscheiben gelten die Festmaßartikel, die sich in der ersten Ebene der Stückliste unterhalb des ISO-Artikels befinden. Die Preise für Einzelscheiben werden herangezogen, wenn dem Artikel in den ISO-Grundpreisen der Berechnungstyp Einzelscheiben zugeordnet ist.
⇨ "Preise für ISO-Einzelscheiben" auf Seite C-717

In der Detailansicht legen Sie die Bedingungen für die Preisberechnung fest, z. B. Preisstaffeln, Mindestberechnungspreis, Zuschläge.

Diese Preise haben eine höhere Priorität als die allgemeinen ISO-Einzelscheiben-Preise.

Zu diesem Dialog stehen folgende Ansichten zur Verfügung:
*   "Spezielle Preise für ISO-Einzelscheiben – Übersicht" auf Seite C-944
*   "Spezielle Preise für ISO-Einzelscheiben – Details" auf Seite C-947

### Spezielle Preise für ISO-Einzelscheiben – Übersicht

**Stammdaten > Konditionen > Spezielle Preise > ISO-Einzelscheiben**

*[Screenshot of "Einzelscheiben für ISO-Artikel" overview dialog window. It shows a table with columns for Artikel, Bezeichnung, ab PLKZ, Preisart, Preistyp, Faktor, and Preis 1.]*
**Abb. C-217 Einzelscheiben für ISO-Artikel - Übersicht**

In dieser Übersicht pflegen Sie die marktpartnerspezifischen Preise für Einzelscheiben, die in ISO-Artikeln verbaut werden. Als Einzelscheiben gelten die Festmaßartikel, die sich in der ersten Ebene der Stückliste unterhalb des ISO-Artikels befinden.

`<F2>` Wechsel zur Detailansicht.
⇨ "Spezielle Preise für ISO-Einzelscheiben – Details" auf Seite C-947

### Feldbeschreibungen

> **Kunden und Lieferanten in den Konditionen**
> Kunden und Lieferanten, für die eine Kondition gilt, bezeichnen im Folgenden immer den jeweiligen Konditionsdebitor aus den Marktpartnerstammdaten.

**Konditionsart**
Auswahl, für wen die Konditionen gelten:
*   **Kunde:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für einen bestimmten Kunden.
*   **Lieferant:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für einen bestimmten Lieferanten.
*   **Objekt-Verkauf:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für ein bestimmtes Verkaufsobjekt.
*   **Objekt-Einkauf:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für ein bestimmtes Einkaufsobjekt.
*   **Kond.-Branche:** Die Konditionen gelten für die Berechnung von Preisen für eine bestimmte Marktpartnergruppe. Marktpartner, für die gemeinsame Konditionen gelten sollen, müssen einer Branche zugeordnet sein.
*Technische Info: numerisches Feld, Toggle-Feld, DB-Feld: spezeinz.kondkz*

**Marktpartner**
Auswahl des Marktpartners, für den die Konditionen gelten. Je nach Konditionsart können Sie einen Kunden, einen Lieferanten, ein Objekt oder eine Kundengruppe angeben.
*Technische Info: numerisches Feld, DB-Feld: spezeinz.kondnr*

**Artikel, Bezeichnung**
Auswahl des Glasartikels, für den die marktpartnerspezifischen Preise gelten.
*Technische Info: numerisches Feld, DB-Feld: spezeinz.artnr*

**Ab PLKZ**
Auswahl des Preislistenkennzeichens (PLKZ), ab dem die Preisdaten gelten.
Findet A+W Enterprise im Auftrag für den Artikel keine Preise zum aktuellen PLKZ, wird das numerisch vorausgehende PLKZ ermittelt, zu dem Preisdaten definiert sind.
⇨ Tutorial, "Ab-PLKZ-Logik" auf Seite C-560
*Technische Info: numerisches Feld, DB-Feld: spezeinz.plkz*

**Preisart**
Auswahl der Preisart, die bestimmt, aus welcher Preisstufe der Preis ermittelt wird:
*   **1 - Einzelpreis:** Zur Preisberechnung wird der Preis der Stufe 1 herangezogen.
*   **3 - Mengenstaffel pro Position (GME):** Zur Ermittlung der Preisstufe wird die Menge der Position anhand der Grundmengeneinheit (GME) des Artikels ermittelt. Der Preis wird nach der Preisstufe berechnet, die durch die Gesamtmenge der Position erreicht ist.
*   **4 - Mengenstaffel pro Stück (GME):** Zur Ermittlung der Preisstufe wird die Grundmenge in einem Stück der Position ermittelt. Zur Preisberechnung wird der Preis mit der Stückzahl multipliziert.
*Technische Info: numerisches Feld, DB-Feld: spezeinz.part*

**Preistyp**
Angabe, worauf sich der angegebene Preis bezieht:
*   **WE/GME:** Der Preis wird pro Grundmengeneinheit aus den Artikelstammdaten berechnet, z. B. pro qm.
*   **WE/Stück:** Im Auftrag wird der Preis als fester Betrag pro Stück in der Position berechnet.
*Technische Info: alphanumerisches Feld, Toggle-Feld DB-Feld: spezeinz.ptyp*

**Faktor**
Angabe eines marktpartnerspezifischen Faktors, mit dem der Preis multipliziert wird. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für eine Preiserhöhung oder einen Rabatt. Wenn Sie das Feld leer lassen, gilt entsprechend der Konditionshierarchie der Faktor aus den Konditionen.
*Technische Info: numerisches Feld, DB-Feld: spezeinz.faktor*

**Beispiel**

| Faktor | Grundpreis | Endpreis |
| :--- | :--- | :--- |
| 100 | 20,00 € | 20,00 € |
| 80 (entspricht einem Rabatt) | 20,00 € | 16,00 € |
| 150 (entspricht einem Aufschlag) | 20,00 € | 30,00 € |

**Preis 1**
Angabe des Grundpreises für die Einzelscheibe. Wenn als Preisart 1 - Einzelpreis gewählt ist, wird zur Preisberechnung ausschließlich der Preis aus diesem Feld verwendet.
*Technische Info: numerisches Feld, DB-Feld: spezeinz.preis1*

### Spezielle Preise für ISO-Einzelscheiben – Details

**Stammdaten > Konditionen > Spezielle Preise > ISO-Einzelscheiben > `<F2>`**

*[Screenshot of "Einzelscheiben für ISO-Artikel - Details" dialog window. It shows header information and fields for setting up price scales.]*
**Abb. C-218 Einzelscheiben für ISO-Artikel - Details**

In diesem Dialog legen Sie die Bedingungen für die Berechnung von marktpartnerspezifischen Preisen für die Einzelscheibe fest, z. B. die gestaffelten Preise.

Die Preise für Einzelscheiben werden herangezogen, wenn dem Artikel in den ISO-Grundpreisen der Berechnungstyp Einzelscheiben zugeordnet ist.

`<F2>` Wechsel zur Übersicht.
⇨ "Spezielle Preise für ISO-Einzelscheiben – Übersicht" auf Seite C-944

#### Feldbeschreibungen (Details)

Die Felder im Kopfbereich sind zum Dialog ISO-Einzelscheiben – Übersicht beschrieben:
⇨ "Spezielle Preise für ISO-Einzelscheiben – Übersicht" auf Seite C-944

Zusätzlich werden die folgenden Felder angezeigt:

**Zuschlagsmatrix**
Auswahl der Zuschlagsmatrix für einen allgemeinen Zuschlag auf die einzelne Scheibe. In der Auftragserfassung wird der Preis der Einzelscheibe inklusive dieses Zuschlags angezeigt.
⇨ "Zuschlagsmatrizen" auf Seite C-814
*Technische Info: numerisches Feld, DB-Feld: spezeinz.zumatnr*

**Mindestpreis**
Angabe des Mindestpreises für die Einzelscheibe. Dieser Preis wird berechnet, wenn der berechnete Preis in der Auftragsposition niedriger ist als der angegebene Mindestpreis. Der Mindestpreis für Kopfartikel mit der Preismethode ISO-Aktuell kann nach den Mindestpreisen für Einzelscheiben ausgewertet werden. Dazu werden der ISO-Grundpreis des Artikels aus der Summe der Einzelscheiben und der ISO-Mindestpreis aus der Summe der Mindestpreise für die Einzelscheiben ermittelt. Wenn der Preis des ISO-Artikels einschließlich der definierten Zuschläge und des Faktors kleiner ist als der Mindestpreis, wird der Mindestpreis berechnet. Diese Berechnung kann für Einkaufs- und Verkaufspreise herangezogen werden.
*Technische Info: numerisches Feld, DB-Feld: spezeinz.minpreis*

**Stufe ab Menge**
Angabe der Menge, ab der der Preis der Stufe berechnet wird. Wenn im Auftrag die Menge in Mengeneinheiten (qm) größer oder gleich dem angegebenen Wert ist, wird der zugeordnete Preis berechnet. Die Preise für Stufen werden nur zur Preisberechnung bei den Preisarten 3 - Mengenstaffel pro Position (GME) oder 4 - Mengenstaffel pro Stück (GME) herangezogen.
*Technische Info: numerisches Feld, DB-Felder: spezeinz.me2, spezeinz.me3, ..., spezeinz.me10*

**Preis für Stufe**
Angabe des Preises, der für die Stufe berechnet wird.
*   Bei der Preisart 1 - Einzelpreis wird nur der Preis für die Stufe 1 verwendet.
*   Bei der Preisart 3 - Mengenstaffel pro Position (GME) oder 4 - Mengenstaffel pro Stück (GME) werden die Preise aus der zugehörigen Preisstufe ermittelt.
*Technische Info: numerisches Feld, DB-Felder: spezeinz.preis2, spezeinz.preis3 ... spezeinz.preis10*

**Erfasser, Erfassungsdatum**
Anzeige des Erfassers und des Erfassungs- oder Änderungsdatums.

**Kondition gültig von ..., bis ...**
Angabe des Datums, ab dem und bis zu dem die Konditionen gültig sind.
*Technische Info: Datumsfeld, DB-Feld: spezeinz.vondat, spezeinz.abdat*

> **Ablauf der Gültigkeit**
> Wenn das Enddatum erreicht ist, werden für die Preisberechnung die allgemeinen Preise und Konditionen herangezogen. Die marktpartnerspezifischen Preise für Einzelscheiben müssen Sie neu definieren, wenn Sie weiterhin mit diesen Konditionen arbeiten wollen.

## Spezielle ISO-Grundpreise

**Stammdaten > Konditionen > Spezielle Preise > ISO-Grundpreise**

In diesem Dialog ordnen Sie den ISO-Artikeln spezielle Preismatrizen, Preisvektoren oder Preise für Einzelgläser zu. Diese Zuordnung gilt nur für den ausgewählten Marktpartner.

In der Detailansicht legen Sie die Bedingungen für die Preisberechnung fest, z. B. Mindestkantenlänge, Maßrundung, Mindestberechnung und verschiedene Zuschläge.

Diese marktpartnerspezifischen Preise haben eine höhere Priorität als die allgemeinen ISO-Grundpreise.
⇨ "ISO-Grundpreise" auf Seite C-711

Zu diesem Dialog stehen folgende Ansichten zur Verfügung:
*   "Spezielle ISO-Grundpreise – Übersicht" auf Seite C-949
*   "Spezielle ISO-Grundpreise – Details" auf Seite C-952
*   "Spezielle ISO-Grundpreise – Austauschlisten" auf Seite C-956

### Spezielle ISO-Grundpreise – Übersicht

**Stammdaten > Konditionen > Spezielle Preise > ISO-Grundpreise**

*[Screenshot of "ISO - Grundpreise" overview dialog window. It shows a table for assigning a Typ (Vektor or Matrix) to an ISO article.]*
**Abb. C-219 ISO-Grundpreise – Übersicht**

In dieser Übersicht pflegen Sie die Zuordnungen von marktpartnerspezifischen Preisen zu ISO-Artikeln. Diese marktpartnerspezifischen Preise haben eine höhere Priorität als die allgemeinen ISO-Grundpreise.

`<F2>` Wechsel zur Detailansicht.
⇨ "Spezielle ISO-Grundpreise - Details" auf Seite C-952

`<F2> <F2>` Wechsel zur Detailansicht für Austauschlisten.
⇨ "Spezielle ISO-Grundpreise - Austauschlisten" auf Seite C-956

### Feldbeschreibungen

> **Kunden und Lieferanten in den Konditionen**
> Kunden und Lieferanten, für die eine Kondition gilt, bezeichnen im Folgenden immer den jeweiligen Konditionsdebitor aus den Marktpartnerstammdaten.

**Konditionsart**
Auswahl, für wen die Konditionen gelten:
*   **Kunde:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für einen bestimmten Kunden.
*   **Lieferant:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für einen bestimmten Lieferanten.
*   **Objekt-Verkauf:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für ein bestimmtes Verkaufsobjekt.
*   **Objekt-Einkauf:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für ein bestimmtes Einkaufsobjekt.
*   **Kond.-Branche:** Die Konditionen gelten für die Berechnung von Preisen für eine bestimmte Marktpartnergruppe. Marktpartner, für die gemeinsame Konditionen gelten sollen, müssen einer Branche zugeordnet sein.
*Technische Info: numerisches Feld, Toggle-Feld, DB-Feld: spezpisomat.kondkz*

**(Marktpartner)**
Auswahl des Marktpartners, für den die Konditionen gelten. Je nach Konditionsart können Sie einen Kunden, einen Lieferanten, ein Objekt oder eine Kundengruppe angeben.
*Technische Info: numerisches Feld, DB-Feld: spezpisomat.kondnr*

**Artikel**
Auswahl des ISO-Artikels, für den die marktpartnerspezifischen Preise gelten.
*Technische Info: numerisches Feld, DB-Feld: spezpisomat.artnr*

**Ab PLKZ**
Auswahl des Preislistenkennzeichens (PLKZ), ab dem die Preisdaten gelten. Findet A+W Enterprise im Auftrag für den Artikel keine Preise zum aktuellen PLKZ, wird das numerisch vorausgehende PLKZ ermittelt, zu dem Preisdaten definiert sind.
⇨ Tutorial, "Ab-PLKZ-Logik" auf Seite C-560
*Technische Info: numerisches Feld, DB-Feld: spezpisomat.vpkz*

**Typ**
Auswahl des Typs, nach dem der ISO-Artikel berechnet wird:
*   **Matrix:** Der Preis für den ISO-Artikel wird aus der zugeordneten Preismatrix berechnet. Dazu müssen Sie die Nummer der Preismatrix auswählen. Dies ist die Standardmethode für ISO.
*   **Vektor:** Der Preis für den ISO-Artikel wird aus dem zugeordneten Vektor berechnet. Dazu müssen Sie die Nummer des Preisvektors auswählen.
*   **Einzelscheiben:** Der Preis für den ISO-Artikel wird aus den Einzelpreisen der Gläser ermittelt, aus denen sich die ISO-Scheibe zusammensetzt. Die Preise für Einzelscheiben werden im Dialog Einzelscheiben für ISO-Artikel erfasst. Dies gilt auch für Austauschgläser.
    ⇨ "Preise für ISO-Einzelscheiben" auf Seite C-717
*Technische Info: alphanumerisches Feld, Toggle-Feld, DB-Feld: spezpisomat.matvek*

**Matrix, Bezeichnung**
Auswahl der Preismatrix für den ISO-Artikel. Das Feld ist nur freigeschaltet, wenn der Typ Matrix gewählt ist. Die Preise selbst legen Sie im Dialog Matrix-Editor an.
⇨ "Matrix-Editor" auf Seite C-722
*Technische Info: numerisches Feld, DB-Feld: spezpisomat.matnr*

**Vektor, Bezeichnung**
Auswahl des Vektors für den ISO-Artikel. Das Feld ist nur freigeschaltet, wenn der Typ Vektor gewählt ist. Die Preise selbst legen Sie im Dialog Artikelvektoren an.
⇨ "Artikelvektoren" auf Seite C-700
*Technische Info: numerisches Feld, DB-Feld: spezpisomat.veknr*

### Spezielle ISO-Grundpreise – Details

**Stammdaten > Konditionen > Spezielle Preise > ISO-Grundpreise > `<F2>`**

*[Screenshot of "ISO - Grundpreise - Details" dialog window. It shows various fields for calculation conditions like Mindestkantenlänge, Mindestberechnung, Maßrundung, and various surcharges.]*
**Abb. C-220 ISO-Grundpreise – Details**

In diesem Dialog legen Sie die Bedingungen für die Berechnung von marktpartnerspezifischen Grundpreisen fest, z. B. Zuschläge und Austauschlisten.

`<F2>` Wechsel zur Detailansicht für Austauschlisten.
⇨ "Spezielle ISO-Grundpreise – Austauschlisten" auf Seite C-956

`<F2> <F2>` Wechsel zur Übersicht.
⇨ "Spezielle ISO-Grundpreise – Übersicht" auf Seite C-949

#### Feldbeschreibungen (Details)

Die Felder im Kopfbereich sind zum Dialog ISO-Grundpreise – Übersicht beschrieben:
⇨ "Spezielle ISO-Grundpreise – Übersicht" auf Seite C-949

Zusätzlich werden die folgenden Felder angezeigt:

**Mindestkantenlänge ... mm**
Angabe der Kantenlänge in mm. Diese Größe wird bei der Preisberechnung herangezogen, wenn die Höhe oder Breite des Glases in der Auftragsposition kleiner ist als diese Mindestkantenlänge.
⇨ Tutorial, "Preisrelevante Menge" auf Seite C-571
*Technische Info: numerisches Feld, DB-Feld: spezpisomat.minkan*

**Mindestberechnung... qm**
Angabe der Fläche in qm. Diese Größe wird bei der Preisberechnung herangezogen, wenn die Fläche des Glases in der Auftragsposition kleiner ist als diese Mindestberechnungsfläche. Bei Modellen wird als preisrelevante Fläche das umschriebene Rechteck der ISO-Einheit herangezogen.
⇨ Tutorial, "Preisrelevante Menge" auf Seite C-571
*Technische Info: numerisches Feld, DB-Feld: spezpisomat.minbereh*

**Maßrundung in mm**
Angabe der Maßrundung in mm für die Preisberechnung der Glasfläche. Für die Preisberechnung werden die Kantenlängen in der Auftragsposition auf die nächsthöhere Länge in mm aufgerundet, die durch die angegebene Maßrundung teilbar ist. Ist die Mindestkantenlänge eines Glases nicht erreicht, wird diese zunächst herangezogen. Die Maßrundung wird anschließend berechnet.
⇨ Tutorial, "Preisrelevante Menge" auf Seite C-571
*Technische Info: numerisches Feld, DB-Feld: spezpisomat.massrd*

**Beispiel**
Als Maßrundung ist 30 mm definiert.
Der erfasste ISO-Artikel hat die Maße 1000 x 1000 mm. Die nächste durch 30 mm teilbare Kantenlänge ist 1020 mm.
Der Preis wird aus den Maßen 1020 × 1020 mm = 1,04 qm berechnet.

**Zuschlagsmatrix**
Auswahl der Zuschlagsmatrix für einen allgemeinen Zuschlag:
*   Bei der Preisberechnung nach einer Matrix wird der Zuschlag auf die ISO-Einheit erhoben.
*   Bei der Preisberechnung nach Einzelscheiben wird der Zuschlag auf jede Einzelscheibe erhoben.
In der Auftragserfassung wird der Preis inklusive dieses Zuschlags angezeigt.
⇨ "Zuschlagsmatrizen" auf Seite C-814
⇨ Tutorial, "Zuschlagsmatrix" auf Seite C-636
*Technische Info: numerisches Feld, DB-Feld: spezpisomat.zumatnr*

**Zuschlag**
Angabe des Preiszuschlags, der immer hinzugerechnet wird, z. B. für ISO mit Thermoscheibe. Im nachfolgenden Feld geben Sie den Zuschlagstyp an.
*Technische Info: numerisches Feld, alphanumerisches Toggle-Feld, DB-Feld: spezpisomat.zuschl*

**Zuschlagstyp**
Angabe, worauf sich der angegebene Zuschlag bezieht:
*   **WE/qm:** Der Zuschlag wird auf den ISO-Grundpreis aufgeschlagen und mit der preisrelevanten Menge in Quadratmeter multipliziert.
*   **Prozent:** Der Zuschlag wird prozentual auf den ISO-Grundpreis aufgeschlagen.
*Technische Info: numerisches Feld, alphanumerisches Toggle-Feld, DB-Feld: spezpisomat.zutyp*

**Zuschlagsrundung ..., auf ...**
Angabe, wie der errechnete Zuschlag gerundet wird:
*   **Auf:** Der Preis wird auf den Hundertstelwert in Währungseinheiten aufgerundet, der im folgenden Feld eingetragen wird.
*   **Ab:** Der Preis wird auf den Hundertstelwert in Währungseinheiten abgerundet, der im folgenden Feld eingetragen wird.
*   **Kau:** Der Preis wird kaufmännisch auf den Hundertstelwert auf- oder abgerundet, der im folgenden Feld eingetragen wird.
*Technische Info: alphanumerisches Toggle-Feld, DB-Felder: spezpisomat.zurdtyp*

**Auf**
Angabe des Werts, auf den gerundet wird, z. B. auf 1, 10, 100.
*Technische Info: numerisches Feld, DB-Feld: spezpisomat.zurund*

**Beispiel**

| Rundung | Wert | von | auf |
| :--- | :--- | :--- | :--- |
| Auf 10 | 4,32 € | 4,40 € | aufgerundet |
| | 4,78 € | 4,80 € | |
| Ab 10 | 4,32 € | 4,30 € | abgerundet |
| | 4,78 € | 4,70 € | |
| Kau 10 | 4,32 € | 4,30 € | abgerundet |
| | 4,78 € | 4,80 € | aufgerundet |
| Kau 100 | 4,32 € | 4,00 € | abgerundet |
| | 4,78 € | 5,00 € | aufgerundet |

**SZR-Zuschlagsvektor**
Auswahl eines Zuschlags für den Abstandhalter im Scheibenzwischenraum (SZR).
⇨ "SZR-Zuschläge" auf Seite C-743
Die Angabe wird ignoriert, wenn in den Auftragskonditionen oder in den Konditionen für den jeweiligen Marktpartner festgelegt ist, dass kein SZR-Zuschlag berechnet wird.
⇨ "Spezielle Allgemeine Konditionen" auf Seite C-850
*Technische Info: numerisches Feld, DB-Feld: spezpisomat.szrzutab*

**Kunstverglasungszuschlag**
Angabe eines Zuschlags für Kunstverglasungen. Dieser Zuschlag wird dann berechnet, wenn in die Stückliste der ISO-Scheibe ein Glas mit dem Artikeltyp Kunstverglasung eingetauscht ist. Der Zuschlag wird nur berechnet, wenn die Kunstverglasung als Austauschglas mit Austausch-Kennzeichen in dem ISO-Artikel eingehängt ist.
*Technische Info: numerisches Feld, DB-Feld: spezpisomat.kunver*

**Stufenzuschlag**
Angabe eines marktpartnerspezifischen Stufenzuschlags. Dieser Zuschlag wird berechnet, wenn in die Stückliste der ISO-Scheibe eine Stufung mit dem Artikeltyp Stufe mit Stufendifferenzmaßen eingehängt ist.
*Technische Info: numerisches Feld, DB-Feld: spezpisomat.stufe*

**Stufenzuschlagstyp**
Angabe, worauf sich der angegebene Zuschlag bezieht:
*   **WE/St ne:** Der Stufenzuschlag wird nach Berechnung des Faktors als fester Nettobetrag pro Stufe aufgeschlagen.
*   **WE/St br:** Der Stufenzuschlag wird vor Berechnung des Faktors als fester Bruttobetrag pro Stufe aufgeschlagen.
*   **Prozent:** Der Stufenzuschlag wird prozentual auf den Glasmengeneinheitspreis und die Austauschpreise aufgeschlagen.
*   **%/Stück:** Der Stufenzuschlag wird pro Stufe prozentual auf den Glasmengeneinheitspreis und die Austauschpreise aufgeschlagen.
*Technische Info: alphanumerisches Toggle-Feld, DB-Feld: spezpisomat.stuftyp*

**Größenzuschläge**
Angabe eines Größenzuschlags. Der Zuschlag wird in der Auftragsposition auf den Glasgrundpreis aufgeschlagen. Wenn dem ISO-Artikel die Preismethode ISO-Aktuell zugeordnet ist und die Umgebungsvariablen `ISO_GROSSZU_AUF_AUSTAUSCH` und/oder `GROSSZU_AUF_SZR` entsprechend konfiguriert sind, wird der Zuschlag zusätzlich auf den Austausch- und/oder SZR-Preis aufgeschlagen.
⇨ “Größenzuschläge" auf Seite C-819
⇨ Tutorial, "Größenzuschläge" auf Seite C-638
*Technische Info: numerisches Feld, DB-Feld: spezpisomat.grosszu*

**Erfasser, Erfassungsdatum**
Anzeige des Erfassers und des Erfassungs- oder Änderungsdatums.

**Kondition gültig von ..., bis ...**
Angabe des Datums, ab dem und bis zu dem die Konditionen gültig sind.
*Technische Info: Datumsfeld, DB-Feld: spezpisomat.vondat, spezpisomat.abdat*

> **Ablauf der Gültigkeit**
> Wenn das Enddatum erreicht ist, werden für die Preisberechnung die allgemeinen Preise und Konditionen herangezogen. Die marktpartnerspezifischen Grundpreise für ISO-Scheiben müssen Sie neu definieren, wenn Sie weiterhin mit diesen Konditionen arbeiten wollen.

### Spezielle ISO-Grundpreise – Austauschlisten

**Stammdaten > Konditionen > Spezielle Preise > ISO-Grundpreise > `<F2>` > `<F2>`**

*[Screenshot of "ISO-Grundpreise - Austauschpreise" dialog window. It shows fields to assign exchange lists for Gussglas, Sonderglas, VSG, ESG, and for Außenscheibe, Mittelscheibe, Innenscheibe.]*
**Abb. C-221 ISO-Grundpreise – Austauschpreise**

In diesen Feldern ordnen Sie dem ISO-Artikel Austauschlisten zu. Diese Listen werden immer dann zur Preisberechnung herangezogen, wenn in der Auftragsposition ein Glas der ISO-Scheibe getauscht wird.
⇨ "Austausch-/Zusatzlisten" auf Seite C-699

`<F2>` Wechsel zur Übersicht.
⇨ "Spezielle ISO-Grundpreise – Übersicht" auf Seite C-949

`<F2> <F2>` Wechsel zur Detailansicht.
⇨ "Spezielle ISO-Grundpreise - Details" auf Seite C-952

#### Feldbeschreibungen (Austauschlisten)

Die Felder im Kopfbereich sind zum Dialog ISO-Grundpreise – Übersicht beschrieben:
⇨ "Spezielle ISO-Grundpreise – Details" auf Seite C-952

Zusätzlich werden die folgenden Felder angezeigt:

**Außenscheibe, Mittelscheibe, Innenscheibe**
Sie können die Austauschlisten abhängig von der Einbauposition angeben, in der die Austauschscheibe in die ISO-Einheit eingebaut ist.

**Gussglas**
Wenn in der Auftragsposition ein Gussglas in die Stückliste der ISO-Scheibe eingetauscht wird, wird der Austauschpreis aus der zugeordneten Austauschliste berechnet.
*Technische Info: numerische Felder, DB-Felder: spezpisomat.gussatph, spezpisomat.kalpkz, spezpisomat.gussatpb*

**Sonderglas**
Wenn in der Auftragsposition ein Sonderglas in die Stückliste der ISO-Scheibe eingetauscht wird, wird der Austauschpreis aus der zugeordneten Austauschliste berechnet.
*Technische Info: numerische Felder, DB-Felder: spezpisomat.sonatph, spezpisomat.prsrdtp, spezpisomat.sonatpb*

**VSG**
Wenn in der Auftragsposition ein VSG in die Stückliste der ISO-Scheibe eingetauscht wird, wird der Austauschpreis aus der zugeordneten Austauschliste berechnet.
*Technische Info: numerische Felder, DB-Felder: spezpisomat.vsgatph, spezpisomat.prsrd, spezpisomat.vsgatpb*

**ESG**
Wenn in der Auftragsposition ein ESG in die Stückliste der ISO-Scheibe eingetauscht wird, wird der Austauschpreis aus der zugeordneten Austauschliste berechnet.
*Technische Info: numerische Felder, DB-Felder: spezpisomat.esgatph, spezpisomat.minprstp, spezpisomat.esgatpb*

**Erfasser, Erfassungsdatum**
Anzeige des Erfassers und des Erfassungs- oder Änderungsdatums.

**Kondition gültig von ..., bis ...**
Angabe des Datums, ab dem und bis zu dem die Konditionen gültig sind.
*Technische Info: Datumsfeld, DB-Feld: spezpisomat.vondat, spezpisomat.abdat*

> **Ablauf der Gültigkeit**
> Wenn das Enddatum erreicht ist, werden für die Preisberechnung die allgemeinen Preise und Konditionen herangezogen. Die marktpartnerspezifischen Preise für UV-Abdeckungen müssen Sie neu definieren, wenn Sie weiterhin mit diesen Konditionen arbeiten wollen.

## UV-Abdeckungspreise

**Stammdaten > Konditionen > Spezielle Preise > UV-Abdeckungspreise**

In diesem Dialog legen Sie marktpartnerspezifische Preise für UV-Abdeckungen an. In der Detailansicht legen Sie weitere Staffelpreise an.

Diese Preise haben eine höhere Priorität als die allgemeinen Preise für UV-Abdeckungen.
⇨ “UV-Abdeckung" auf Seite C-745

Zu diesem Dialog stehen folgende Ansichten zur Verfügung:
*   "UV-Abdeckungspreise – Übersicht" auf Seite C-958
*   "UV-Abdeckungspreise – Details" auf Seite C-960

### UV-Abdeckungspreise – Übersicht

**Stammdaten > Konditionen > Spezielle Preise > UV-Abdeckungspreise**

*[Screenshot of "UV-Abdeckungen - Übersicht" dialog window. It shows a table with columns for Artikel, ab PLKZ, and up to 5 price tiers (Staffel1-5).]*
**Abb. C-222 UV-Abdeckungen – Übersicht**

In dieser Übersicht pflegen Sie die marktpartnerspezifischen Preise für UV-Abdeckungen. Diese Preise haben eine höhere Priorität als die allgemeinen Preise für UV-Abdeckungen.

`<F2>` Wechsel zur Detailansicht.
⇨ "UV-Abdeckungspreise - Details" auf Seite C-960

### Feldbeschreibungen

> **Kunden und Lieferanten in den Konditionen**
> Kunden und Lieferanten, für die eine Kondition gilt, bezeichnen im Folgenden immer den jeweiligen Konditionsdebitor aus den Marktpartnerstammdaten.

**Konditionsart**
Auswahl, für wen die Konditionen gelten:
*   **Kunde:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für einen bestimmten Kunden.
*   **Lieferant:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für einen bestimmten Lieferanten.
*   **Objekt-Verkauf:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für ein bestimmtes Verkaufsobjekt.
*   **Objekt-Einkauf:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für ein bestimmtes Einkaufsobjekt.
*   **Kond.-Branche:** Die Konditionen gelten für die Berechnung von Preisen für eine bestimmte Marktpartnergruppe. Marktpartner, für die gemeinsame Konditionen gelten sollen, müssen einer Branche zugeordnet sein.
*Technische Info: numerisches Feld, Toggle-Feld, DB-Feld: kupuvab.kondkz*

**(Marktpartner)**
Auswahl des Marktpartners, für den die Konditionen gelten. Je nach Konditionsart können Sie einen Kunden, einen Lieferanten, ein Objekt oder eine Kundengruppe angeben.
*Technische Info: numerisches Feld, DB-Feld: kupuvab.kunr*

**Artikel**
Angabe des Artikels vom Artikeltyp UV-Abdeckung, für den die Preise gelten.
*Technische Info: numerische Felder, DB-Felder: kupuvab.artnr*

**Ab PLKZ**
Auswahl des Preislistenkennzeichens (PLKZ), ab dem die Preisdaten gelten.
Findet A+W Enterprise im Auftrag für den Artikel keine Preise zum aktuellen PLKZ, wird das numerisch vorausgehende PLKZ ermittelt, zu dem Preisdaten definiert sind.
⇨ Tutorial, "Ab-PLKZ-Logik" auf Seite C-560
*Technische Info: numerische Felder, DB-Felder: kupuvab.plkz*

**Staffel 1-10 (Preis)**
Angabe der Staffelpreise. Der Preis gilt pro Mengeneinheit der UV-Abdeckung. In der Detailansicht geben Sie die Grenzwerte für die Maße an. Der Preis gilt so lange, bis der nächsthöhere Grenzwert erreicht ist.
⇨ "UV-Abdeckungspreise - Details" auf Seite C-960
*Technische Info: numerische Felder, DB-Felder: kupuvab.preis1, kupuvab.preis2, ... kupuvab.preis10*

### UV-Abdeckungspreise – Details

**Stammdaten > Konditionen > Spezielle Preise > UV-Abdeckungspreise > `<F2>`**

*[Screenshot of "UV-Abdeckungen - Details" dialog window. It shows a list of price tiers defined by 'bis Breite' and 'Preis'.]*
**Abb. C-223 UV-Abdeckungen – Details**

In diesem Dialog legen Sie die marktpartnerspezifischen Grenzwerte für die Preisstaffeln fest.

`<F2>` Wechsel zur Übersicht.
⇨ "UV-Abdeckungspreise - Übersicht" auf Seite C-958

#### Feldbeschreibungen (Details)

Die Felder im Kopfbereich sind zum Dialog UV-Abdeckungen – Übersicht beschrieben:
⇨ "UV-Abdeckungspreise - Übersicht" auf Seite C-958

Zusätzlich werden die folgenden Felder angezeigt:

**Breite bis ... mm**
Angabe der Breite der UV-Abdeckung, bis zu der der Preis gilt.
*Technische Info: numerische Felder, DB-Felder: kupuvab.bis1, kupuvab.bis2, ..., kupuvab.bis9*

**Preis**
Angabe der Staffelpreise. Der Preis gilt pro Mengeneinheit der UV-Abdeckung. Der Preis gilt so lange, bis der nächsthöhere Grenzwert erreicht ist, der in den Feldern Breite bis ... mm angegeben ist.
*Technische Info: numerische Felder, DB-Felder: kupuvab.preis2, ..., kupuvab.preis10*

**Erfasser, Erfassungsdatum**
Anzeige des Erfassers und des Erfassungs- oder Änderungsdatums.

**Kondition gültig von ..., bis ...**
Angabe des Datums, ab dem und bis zu dem die Konditionen gültig sind.
*Technische Info: Datumsfeld, DB-Feld: kupuvab.vondat, kupuvab.abdat*

> **Ablauf der Gültigkeit**
> Wenn das Enddatum erreicht ist, werden für die Preisberechnung die allgemeinen Preise und Konditionen herangezogen. Die marktpartnerspezifischen Preise für UV-Abdeckungen müssen Sie neu definieren, wenn Sie weiterhin mit diesen Konditionen arbeiten wollen.

## Verglasungspreise

**Stammdaten > Konditionen > Spezielle Preise > Verglasungspreise**

In diesem Dialog legen Sie marktpartnerspezifische Preise für Verglasung und Versiegelung an. In der Detailansicht legen Sie zusätzlich einen Mindestberechnungspreis an.

Diese Preise haben eine höhere Priorität als die allgemeinen Verglasungspreise.
⇨ "PKZ-Verglasungspreise" auf Seite C-797

> **Voraussetzung**
> Die Preise für Verglasung und/oder Versiegelung können nur berechnet werden, wenn ein Artikel in die Stückliste eingehängt ist, für den im Artikelstamm der Artikeltyp 520 Verglasung oder 525 Montage und die Preismethode PKZ-Verglasung definiert ist.

Zu diesem Dialog stehen folgende Ansichten zur Verfügung:
*   "Verglasungspreise – Übersicht" auf Seite C-962
*   "Verglasungspreise – Details" auf Seite C-964

### Verglasungspreise – Übersicht

**Stammdaten > Konditionen > Spezielle Preise > Verglasungspreise**

*[Screenshot of "Verglasung - Übersicht" dialog window. It shows a table with columns for Artikel, ab PLKZ, Berechnungstyp, Versiegelung Preis/lm, Verglasungspreise Preis/qm.]*
**Abb. C-224 Verglasung - Übersicht**

In dieser Übersicht pflegen Sie die marktpartnerspezifischen Preise für Verglasung und Versiegelung. In der Detailansicht können Sie zusätzlich einen Mindestberechnungspreis angeben.

`<F2>` Wechsel zur Detailansicht.
⇨ "Verglasungspreise - Details" auf Seite C-964

### Feldbeschreibungen

> **Kunden und Lieferanten in den Konditionen**
> Kunden und Lieferanten, für die eine Kondition gilt, bezeichnen im Folgenden immer den jeweiligen Konditionsdebitor aus den Marktpartnerstammdaten.

**Konditionsart**
Auswahl, für wen die Konditionen gelten:
*   **Kunde:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für einen bestimmten Kunden.
*   **Lieferant:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für einen bestimmten Lieferanten.
*   **Objekt-Verkauf:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für ein bestimmtes Verkaufsobjekt.
*   **Objekt-Einkauf:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für ein bestimmtes Einkaufsobjekt.
*   **Kond.-Branche:** Die Konditionen gelten für die Berechnung von Preisen für eine bestimmte Marktpartnergruppe. Marktpartner, für die gemeinsame Konditionen gelten sollen, müssen einer Branche zugeordnet sein.
*Technische Info: numerisches Feld, Toggle-Feld, DB-Feld: kuverglas.kondkz*

**(Marktpartner)**
Auswahl des Marktpartners, für den die Konditionen gelten. Je nach Konditionsart können Sie einen Kunden, einen Lieferanten, ein Objekt oder eine Kundengruppe angeben.
*Technische Info: numerisches Feld, DB-Feld: kuverglas.kunr*

**Artikel**
Auswahl des Verglasungsartikels, für den der marktpartnerspezifische Preis gilt.
*Technische Info: numerisches Feld, DB-Feld: kuverglas.artnr*

**Ab PLKZ**
Auswahl des Preislistenkennzeichens (PLKZ), ab dem die Preisdaten gelten.
Findet A+W Enterprise im Auftrag für den Artikel keine Preise zum aktuellen PLKZ, wird das numerisch vorausgehende PLKZ ermittelt, zu dem Preisdaten definiert sind.
⇨ Tutorial, "Ab-PLKZ-Logik" auf Seite C-560
*Technische Info: numerisches Feld, DB-Feld: kuverglas.pkz*

**Berechnungstyp**
Auswahl des Berechnungstyps. Dieser Typ legt fest, wie die Preise berechnet werden:
*   **verglasen:** Die Verglasung wird nach der Fläche der Scheibe berechnet.
*   **versiegeln:** Die Versiegelung wird nach dem Umfang der Scheibe berechnet.
*   **verglasen + versiegeln:** Verglasung und Versiegelung werden berechnet.
*Technische Info: alphanumerisches Feld, Toggle-Feld, DB-Feld: kuverglas.typ*

#### Versiegelung

**Preis/lm**
Angabe des Preises pro Laufmeter.
*Technische Info: numerisches Feld, DB-Feld: kuverglas.vklmpreis*

#### Verglasung

**Preis/qm**
Angabe des Preises pro Quadratmeter.
*Technische Info: numerisches Feld, DB-Feld: kuverglas.vkqmpreis*

### Verglasungspreise – Details

**Stammdaten > Konditionen > Spezielle Preise > Verglasungspreise > `<F2>`**

*[Screenshot of "Verglasung - Details" dialog window. It shows fields for setting minimum prices for sealing (Versiegelung) and glazing (Verglasung).]*
**Abb. C-225 Verglasung - Details**

In diesem Dialog legen Sie die marktpartnerspezifischen Mindestpreise für Verglasung und Versiegelung fest.

`<F2>` Wechsel zur Übersicht.
⇨ "Verglasungspreise – Übersicht" auf Seite C-962

#### Feldbeschreibungen (Details)

Die Felder im Kopfbereich sind zum Dialog Verglasung – Übersicht beschrieben:
⇨ "Verglasungspreise – Übersicht" auf Seite C-962

Zusätzlich werden die folgenden Felder angezeigt:

#### Versiegelung

**Mindestpreis**
Angabe des Mindestpreises für die Versiegelung. Dieser Preis wird berechnet, wenn der berechnete Preis in der Auftragsposition niedriger ist als der angegebene Mindestpreis.
*   Mindestpreise für Kopfartikel werden nur bei den Preismethoden ISO-Schweiz, ISO-Aktuell (nur mit der Berechnungsart Vektor), PKZ-VSG, PKZ-ESG, PKZ-Basisglas, PKZ-veredeltes Glas oder PKZ-Preise ausgewertet.
*   Mindestpreise für Stücklistenunterteile werden nur ausgewertet, wenn beim Kopfartikel die Preismethode ISO-Aktuell, PKZ-VSG, PKZ-ESG, PKZ-Basisglas, PKZ-veredeltes Glas oder PKZ-Glastüren gewählt ist und das Unterteil ein Zubehörartikel mit der Preismethode PKZ-Preise allgemein ist.
Der Preis wird für die Berechnungstypen `versiegeln` und `verglasen + versiegeln` herangezogen.
*Technische Info: numerisches Feld, DB-Feld: kuverglas.vkminversieg*

#### Verglasung

**Mindestpreis**
Angabe des Mindestpreises für die Verglasung. Dieser Preis wird berechnet, wenn der berechnete Preis in der Auftragsposition niedriger ist als der angegebene Mindestpreis.
*   Mindestpreise für Kopfartikel werden nur bei den Preismethoden ISO-Schweiz, ISO-Aktuell (nur mit der Berechnungsart Vektor), PKZ-VSG, PKZ-ESG, PKZ-Basisglas, PKZ-veredeltes Glas oder PKZ-Preise ausgewertet.
*   Mindestpreise für Stücklistenunterteile werden nur ausgewertet, wenn beim Kopfartikel die Preismethode ISO-Aktuell, PKZ-VSG, PKZ-ESG, PKZ-Basisglas, PKZ-veredeltes Glas oder PKZ-Glastüren gewählt ist und das Unterteil ein Zubehörartikel mit der Preismethode PKZ-Preise allgemein ist.
Der Preis wird für die Berechnungstypen `verglasen` und `verglasen + versiegeln` herangezogen.
*Technische Info: numerisches Feld, DB-Feld: kuverglas.vkminpreis*

**Erfasser, Erfassungsdatum**
Anzeige des Erfassers und des Erfassungs- oder Änderungsdatums.

**Kondition gültig von ..., bis ...**
Angabe des Datums, ab dem und bis zu dem die Konditionen gültig sind.
*Technische Info: Datumsfeld, DB-Feld: kuverglas.vondat, kuverglas.abdat*

> **Ablauf der Gültigkeit**
> Wenn das Enddatum erreicht ist, werden für die Preisberechnung die allgemeinen Preise und Konditionen herangezogen. Die marktpartnerspezifischen Preise für Verglasungen müssen Sie neu definieren, wenn Sie weiterhin mit diesen Konditionen arbeiten wollen.

## Austauschpreise Gussklassen

**Stammdaten > Konditionen > Spezielle Preise > Austauschpreise Gussklassen**

In diesem Dialog legen Sie marktpartnerspezifische Austauschpreise für Gussklassen fest. In der Detailansicht legen Sie die Bedingungen für die Preisberechnung fest, z. B. Mindestberechnungsmenge, Faktor.

Diese Preise haben eine höhere Priorität als die allgemeinen Austauschpreise für Gussglas.
⇨ "Gussglas-Austauschpreise" auf Seite C-735

Zu diesem Dialog stehen folgende Ansichten zur Verfügung:
*   "Austauschpreise Gussklassen – Übersicht" auf Seite C-966
*   "Austauschpreise Gussklassen - Details" auf Seite C-968

### Austauschpreise Gussklassen – Übersicht

**Stammdaten > Konditionen > Spezielle Preise > Austauschpreise Gussklassen**

*[Screenshot of "Austauschpreise Gussklassen - Übersicht" dialog window. It shows a table with columns for Austauschliste, Gussklasse, ab PLKZ, Faktor, Preis, and Preistyp.]*
**Abb. C-226 Austauschpreise Gussklassen – Übersicht**

In dieser Übersicht pflegen Sie die marktpartnerspezifischen Austauschpreise für Gussklassen. Zusätzlich können Sie einen Faktor angeben.

`<F2>` Wechsel zur Detailansicht.
⇨ "Austauschpreise Gussklassen - Details" auf Seite C-968

### Feldbeschreibungen

> **Kunden und Lieferanten in den Konditionen**
> Kunden und Lieferanten, für die eine Kondition gilt, bezeichnen im Folgenden immer den jeweiligen Konditionsdebitor aus den Marktpartnerstammdaten.

**Konditionsart**
Auswahl, für wen die Konditionen gelten:
*   **Kunde:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für einen bestimmten Kunden.
*   **Lieferant:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für einen bestimmten Lieferanten.
*   **Objekt-Verkauf:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für ein bestimmtes Verkaufsobjekt.
*   **Objekt-Einkauf:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für ein bestimmtes Einkaufsobjekt.
*   **Kond.-Branche:** Die Konditionen gelten für die Berechnung von Preisen für eine bestimmte Marktpartnergruppe. Marktpartner, für die gemeinsame Konditionen gelten sollen, müssen einer Branche zugeordnet sein.
*Technische Info: numerisches Feld, Toggle-Feld, DB-Feld: spezpgssat.kondkz*

**(Marktpartner)**
Auswahl des Marktpartners, für den die Konditionen gelten. Je nach Konditionsart können Sie einen Kunden, einen Lieferanten, ein Objekt oder eine Kundengruppe angeben.
*Technische Info: numerisches Feld, DB-Feld: spezpgssat.kondnr*

**Austauschliste, Bezeichnung**
Auswahl der Austauschliste für die Zuordnung von marktpartnerspezifischen Austauschpreisen.
*Technische Info: numerisches Feld, DB-Feld: spezpgssat.atlnr*

**Gussklasse**
Angabe der Gussglas-Klasse (Preisgruppe) für die Austauschliste. Die Gläser werden den Gussglas-Klassen im Dialog Gussglas-Austausch zugeordnet.
⇨ "Gussglas-Austauschpreise" auf Seite C-735
*Technische Info: alphanumerisches Feld, DB-Feld: spezpgssat.klasse*

**Ab PLKZ**
Auswahl des Preislistenkennzeichens (PLKZ), ab dem die Preisdaten gelten.
Findet A+W Enterprise im Auftrag für den Artikel keine Preise zum aktuellen PLKZ, wird das numerisch vorausgehende PLKZ ermittelt, zu dem Preisdaten definiert sind.
⇨ Tutorial, "Ab-PLKZ-Logik" auf Seite C-560
*Technische Info: numerisches Feld, DB-Feld: spezpgssat.plkz*

**Faktor**
Angabe eines Faktors, mit dem der Austauschpreis multipliziert wird. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für eine Preiserhöhung oder einen Rabatt. Wenn Sie das Feld leer lassen, gilt entsprechend der Konditionshierarchie der Faktor aus den Konditionen.
*Technische Info: numerisches Feld, DB-Feld: spezpgssat.faktor*

**Beispiel**

| Faktor | Grundpreis | Endpreis |
| :--- | :--- | :--- |
| 100 | 20,00 € | 20,00 € |
| 80 (entspricht einem Rabatt) | 20,00 € | 16,00 € |
| 150 (entspricht einem Aufschlag) | 20,00 € | 30,00 € |

**Preis**
Angabe des Preises für die jeweilige Gussklasse. Damit übersteuern Sie den Preis aus der Gussklasse für den aktuellen Marktpartner.
*Technische Info: numerisches Feld, DB-Feld: spezpgssat.preis*

**Preistyp**
Angabe, worauf sich der angegebene Preis bezieht:
*   **WE/qm:** Der Preis wird pro Quadratmeter berechnet.
*   **Prozent:** Der Preis wird prozentual aus dem Grundpreis des Kopfartikels einschließlich des Teuerungszuschlags errechnet.
*Technische Info: alphanumerisches Feld, Toggle-Feld, DB-Feld: spezpgssat.preistyp*

### Austauschpreise Gussklassen – Details

**Stammdaten > Konditionen > Spezielle Preise > Austauschpreise Gussklassen > `<F2>`**

*[Screenshot of "Austauschpreise Gussklassen - Details" dialog window. It shows fields for setting a minimum calculation area (Mindestberechnung) for the exchange article.]*
**Abb. C-227 Austauschpreise Gussklassen – Details**

In diesem Dialog legen Sie den marktpartnerspezifischen Mindestberechnungspreis für den Austauschartikel fest.

`<F2>` Wechsel zur Übersicht.
⇨ "Austauschpreise Gussklassen – Übersicht" auf Seite C-966

#### Feldbeschreibungen (Details)

Die Felder im Kopfbereich sind zum Dialog Austauschpreise Gussklassen – Übersicht beschrieben:
⇨ "Austauschpreise Gussklassen – Übersicht" auf Seite C-966

Zusätzlich werden die folgenden Felder angezeigt:

**Mindestberechnung ...qm**
Angabe der Mindestfläche in qm, für die der Preis berechnet wird. Wenn die Fläche des Austauschglases in der Auftragsposition kleiner ist als die Mindestberechnungsfläche, wird der Preis für diese Fläche berechnet.
⇨ Tutorial, "Preisrelevante Menge" auf Seite C-571
*Technische Info: numerisches Feld, DB-Feld: spezpgssat.minber*

**Erfasser, Erfassungsdatum**
Anzeige des Erfassers und des Erfassungs- oder Änderungsdatums.

**Kondition gültig von ..., bis ...**
Angabe des Datums, ab dem und bis zu dem die Konditionen gültig sind.
*Technische Info: Datumsfeld, DB-Feld: spezpgssat.vondat, spezpgssat.abdat*

> **Ablauf der Gültigkeit**
> Wenn das Enddatum erreicht ist, werden für die Preisberechnung die allgemeinen Preise und Konditionen herangezogen. Die marktpartnerspezifischen Austauschpreise für Gussklassen müssen Sie neu definieren, wenn Sie weiterhin mit diesen Konditionen arbeiten wollen.

## Spezielle VSG-Austausch-/Zusatzpreise

**Stammdaten > Konditionen > Spezielle Preise > VSG-Austausch-/Zusatzpreise**

In diesem Dialog legen Sie marktpartnerspezifische Austauschpreise für Gläser und Folien an, die in VSG-Artikel eingetauscht oder zusätzlich eingebaut werden. In der Detailansicht legen Sie die Bedingungen für die Preisberechnung fest, z. B. Staffelpreise, Mindestberechnungsmenge, Maßrundung, Größenzuschläge.

Diese Preise haben eine höhere Priorität als die allgemeinen VSG-Austauschpreise.
⇨ "VSG-Austausch-/Zusatzpreise – Übersicht" auf Seite C-779

Zu diesem Dialog stehen folgende Ansichten zur Verfügung:
*   "Spezielle VSG-Austausch-/Zusatzpreise – Übersicht" auf Seite C-971
*   "Spezielle VSG-Austausch-/Zusatzpreise – Details" auf Seite C-974

### Spezielle VSG-Austausch-/Zusatzpreise – Übersicht

**Stammdaten > Konditionen > Spezielle Preise > VSG-Austausch-/Zusatzpreise**

*[Screenshot of "VSG-Austausch-/Zusatzpreise - Übersicht" dialog window. It shows a table with columns for Artikel, Liste, ab PLKZ, Berechnungsart, Faktor, and Preis 1.]*
**Abb. C-228 VSG-Austausch-/Zusatzpreise – Übersicht**

In dieser Übersicht pflegen Sie marktpartnerspezifische Austauschpreise für Gläser und Folien, die in VSG-Artikel eingetauscht oder zusätzlich eingebaut werden. Diese Preise haben eine höhere Priorität als die allgemeinen VSG-Austauschpreise.

`<F2>` Wechsel zur Detailansicht.
⇨ "Spezielle VSG-Austausch-/Zusatzpreise – Details" auf Seite C-974

### Feldbeschreibungen

> **Kunden und Lieferanten in den Konditionen**
> Kunden und Lieferanten, für die eine Kondition gilt, bezeichnen im Folgenden immer den jeweiligen Konditionsdebitor aus den Marktpartnerstammdaten.

**Konditionsart**
Auswahl, für wen die Konditionen gelten:
*   **Kunde:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für einen bestimmten Kunden.
*   **Lieferant:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für einen bestimmten Lieferanten.
*   **Objekt-Verkauf:** Die Konditionen gelten für die Berechnung von Verkaufspreisen für ein bestimmtes Verkaufsobjekt.
*   **Objekt-Einkauf:** Die Konditionen gelten für die Berechnung von Einkaufspreisen für ein bestimmtes Einkaufsobjekt.
*   **Kond.-Branche:** Die Konditionen gelten für die Berechnung von Preisen für eine bestimmte Marktpartnergruppe. Marktpartner, für die gemeinsame Konditionen gelten sollen, müssen einer Branche zugeordnet sein.
*Technische Info: numerisches Feld, Toggle-Feld, DB-Feld: spezvsgaust.kondkz*

**(Marktpartner)**
Auswahl des Marktpartners, für den die Konditionen gelten. Je nach Konditionsart können Sie einen Kunden, einen Lieferanten, ein Objekt oder eine Kundengruppe angeben.
*Technische Info: numerisches Feld, DB-Feld: spezvsgaust.kondnr*

**Artikel, Bezeichnung**
Auswahl des VSG-Artikels, für den die marktpartnerspezifischen VSG-Austausch-/Zusatzpreise gelten.

**Liste**
Auswahl der Austauschliste, in der Sie die Preise festlegen. Das Kennzeichen der Austauschliste wird im Dialog Austausch-/Zusatzlisten angelegt.
⇨ "Austausch-/Zusatzlisten" auf Seite C-699
*Technische Info: numerisches Feld, DB-Feld: spezvsgaust.artnr*

**ab PLKZ**
Auswahl des Preislistenkennzeichens (PLKZ), für das die Preisdaten gelten. Das Preislistenkennzeichen wird im Dialog Preislistenkennzeichen angelegt.
⇨ "Preislisten (PLKZ)" auf Seite C-696
*Technische Info: numerisches Feld, DB-Feld: spezvsgaust.plkz*

**Berechnungsart**
Auswahl der Berechnungsart, nach der die Austauschpreise berechnet werden:
*   **Fläche:** Der Preis wird nach der Fläche des Glases (nach Maßrundung, ohne Mindestberechnung) gestaffelt. Wenn die Fläche größer oder gleich der angegebenen Grenzmenge ist, wird der Staffelpreis als Austauschpreis herangezogen.
*   **1 Kante:** Der Preis wird nach der Länge der Kante (nach Maßrundung) gestaffelt. Wenn die längste Kante größer oder gleich der angegebenen Grenzmenge ist, wird der Staffelpreis als Austauschpreis herangezogen.
*   **2 Kanten:** Der Preis wird abhängig von den zwei Kantenlängen gestaffelt. Die zwei Kantenlängen werden mit den hinterlegten Grenzwerten verglichen. Dabei wird die kürzere Kante mit dem 1. Maß und die längere Kante mit dem 2. Maß verglichen. Standardmäßig wird der Austauschpreis der jeweiligen Stufe nur herangezogen, wenn beide Maße die Grenzwerte überschreiten. Wenn die Variable `ISOAUST_2KANTEN_BIS` aktiv ist, wird der Austauschpreis auch herangezogen, wenn nur ein Grenzmaß überschritten ist.
*   **Matrix:** Der Preis wird nach der zugeordneten Matrix gestaffelt. Die Matrix ordnen Sie im Feld Matrix zu. Standardmäßig wird als Austauschpreis ein Mischpreis aus (Glasgrundpreis + Matrixpreis) / 2 - Glasgrundpreis berechnet. Wenn die Variable `ISOAUST_KEINE_MISCHMATRIX` mit dem Wert ON aktiv ist, wird der Staffelpreis aus der entsprechenden Matrix direkt als Austauschpreis herangezogen.
*   **Prozent:** Der Preis wird nach der Fläche des Glases (nach Maßrundung, ohne Mindestberechnung) gestaffelt. Wenn die Fläche größer oder gleich der angegebenen Grenzmenge ist, wird der Staffelpreis als Austauschpreis herangezogen. Der Preis wird prozentual aus dem Grundpreis des Kopfartikels errechnet und addiert.
*Technische Info: alphanumerisches Feld, Toggle-Feld, DB-Feld: spezvsgaust.berechart*

**Faktor**
Angabe eines Faktors, mit dem der Austauschpreis multipliziert wird. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für eine Preiserhöhung oder einen Rabatt. Wenn Sie das Feld leer lassen, gilt entsprechend der Konditionshierarchie der Faktor aus den Konditionen.
*Technische Info: numerisches Feld, DB-Feld: spezvsgaust.faktor*

**Beispiel**

| Faktor | Grundpreis | Endpreis |
| :--- | :--- | :--- |
| 100 | 20,00 € | 20,00 € |
| 80 (entspricht einem Rabatt) | 20,00 € | 16,00 € |
| 150 (entspricht einem Aufschlag) | 20,00 € | 30,00 € |

**Preis 1**
Angabe des Einzelpreises. Gestaffelte Preise geben Sie in der Detailansicht ein.
⇨ “Spezielle VSG-Austausch-/Zusatzpreise – Details" auf Seite C-974
*Technische Info: numerisches Feld, DB-Feld: spezvsgaust.preis1*

### Spezielle VSG-Austausch-/Zusatzpreise – Details

**Stammdaten > Konditionen > Spezielle Preise > VSG-Austausch-/Zusatzpreise > `<F2>`**

*[Screenshot of "VSG-Austausch-/Zusatzpreise - Details" dialog window. It shows fields for Mindestberechnung, Maßrundung, Größenzuschläge, and scaled pricing based on 'Abmessungen'.]*
**Abb. C-229 VSG-Austausch-/Zusatzpreise – Details**

In diesem Dialog legen Sie Bedingungen für die Preisberechnung fest, z. B. Preisstaffeln, Mindestberechnungsmenge, Maßrundung, Zuschläge.

`<F2>` Wechsel zur Übersicht.
⇨ "Spezielle VSG-Austausch-/Zusatzpreise – Übersicht" auf Seite C-971

#### Feldbeschreibungen (Details)

Die Felder im Kopfbereich sind zum Dialog VSG-Austausch-/Zusatzpreise – Übersicht beschrieben:
⇨ "Spezielle VSG-Austausch-/Zusatzpreise – Übersicht" auf Seite C-971

Zusätzlich werden die folgenden Felder angezeigt:

**Mindestberechnung ... ME**
Angabe der Mindestmenge, für die der Preis berechnet wird. Die Mindestmenge wird entsprechend der Grundmengeneinheit im Artikelstamm angegeben, z. B. Fläche in qm. Wenn die Fläche des Glases in der Auftragsposition kleiner ist als die Mindestberechnung, wird der Preis für diese Mindestberechnung berechnet.
Abhängig von der Konfiguration kann die Berechnung des Austauschpreises auf den Kopfartikel oder auf den Austauschartikel bezogen sein.
*   Wenn die Variable `MINBER_AUSTAUSCH_OHNE_MAX` aktiv ist, wird für Artikel mit der Preismethode ISO-Aktuell nur die Mindestberechnungseinheit ausgewertet.
*   Wenn die Variable `MINBER_AUSTAUSCH_OHNE_MAX` nicht aktiv ist, wird für Artikel mit der Preismethode ISO-Aktuell die Mindestberechnung von Grundartikel und Austauschartikel herangezogen und die größere der beiden Berechnungen ausgewertet.
Unabhängig von dieser Einstellung wird immer der höhere Preis berechnet.
⇨ Tutorial, "Preisrelevante Menge" auf Seite C-571
*Technische Info: numerisches Feld, DB-Feld: spezvsgaust.minber*

**Maßrundung... mm**
Angabe der Maßrundung in mm für die Preisberechnung des Artikels, z B. 30 mm. Für die Preisberechnung werden die Höhe und die Breite der Auftragsposition auf die nächsthöhere Länge in mm aufgerundet, die durch die angegebene Maßrundung teilbar ist.
*Technische Info: numerisches Feld, DB-Feld: spezvsgaust.massrund*

**Beispiel**
Als Maßrundung ist 30 mm definiert.
Der erfasste ISO-Artikel hat die Maße 1000 × 1000 mm. Die nächste durch 30 mm teilbare Kantenlänge ist 1020 mm.
Der Preis wird aus den Maßen 1020 × 1020 mm = 1,04 qm berechnet.

**Größenzuschläge**
Auswahl eines Größenzuschlags. Das kann ein Kleinglaszuschlag, ein Überlängenzuschlag und/oder Übergrößenzuschlag sein. Wenn der Artikel diese Größe über- oder unterschreitet, wird der Zuschlag auf den Glaspreis aufgeschlagen.
⇨ "Größenzuschläge" auf Seite C-819
*Technische Info: numerisches Feld, DB-Feld: spezvsgaust.grosszu*

**Abmessungen**
**Ab...** Angabe der Grenzwerte für Staffelpreise. Der Preis einer Stufe gilt so lange, bis der nächsthöhere Wert erreicht ist. Je nach der gewählten Berechnungsart müssen Sie die Werte in folgenden Maßeinheiten eingeben:
*   **Fläche:** Anzahl der Quadratmeter, ab denen der zugeordnete Preis herangezogen wird.
*   **Kante:** Anzahl der Millimeter, ab denen der zugeordnete Preis berechnet wird.
*   **Prozent:** Anzahl der Fläche in Prozent, ab der der zugeordnete Preis berechnet wird.
*   **Matrix:** Die Preise werden nach der zugeordneten Matrix berechnet. Die Felder für die Grenzwerte und die Preise sind gesperrt.
*Technische Info: numerische Felder, DB-Felder: spezvsgaust.grenz21, spezvsgaust.grenz22, spezvsgaust.grenz31, spezvsgaust.grenz32, spezvsgaust.grenz41, spezvsgaust.grenz42, spezvsgaust.grenz51, spezvsgaust.grenz52*

**Preis**
Angabe des Preises für die jeweilige Maßstufe. Der Preis gilt so lange, bis der nächsthöhere Wert erreicht ist.
*Technische Info: numerische Felder, DB-Felder: spezvsgaust.preis2, spezvsgaust.preis3, ... spezvsgaust.preis5*

**Erfasser, Erfassungsdatum**
Anzeige des Erfassers und des Erfassungs- oder Änderungsdatums.

**Kondition gültig von ..., bis ...**
Angabe des Datums, ab dem und bis zu dem die Konditionen gültig sind.
*Technische Info: Datumsfeld, DB-Feld: spezvsgaust.vondat, spezvsgaust.abdat*

> **Ablauf der Gültigkeit**
> Wenn das Enddatum erreicht ist, werden für die Preisberechnung die allgemeinen Preise und Konditionen herangezogen. Die marktpartnerspezifischen Austausch- und Zusatzpreise für VSG müssen Sie neu definieren, wenn Sie weiterhin mit diesen Konditionen arbeiten wollen.

---

# D. A+W Enterprise Verkauf

## Revisionsübersicht des Moduls

| Datum | Änderung |
| :--- | :--- |
| 05-2023 | Ersterstellung des Tutorials, Aktualisierung der Softwarereferenz |
| 02-2020 | Vollständige Überarbeitung |
| 01-2017 | Produkt- und Firmennamen angepasst. |
| 07-2013 | Vollständige Überarbeitung und Anpassung an neues CI |
| 01-2010 | Kleinere Korrekturen/Identifier |
| 01-2008 | Preisberechnung |
| 02-2007 | Zusammenführung Verkauf/Einkauf |
| 12-2006 | Änderung Part Verkauf |
| 02-2006 | Ersterstellung |

**Zu diesem Modul finden Sie folgende Kapitel:**
⇨ Tutorial
⇨ Softwarereferenz

---

# A+W Enterprise Verkauf: Tutorial

## In diesem Kapitel finden Sie folgende Themen:

*   ⇨ Einführung
*   ⇨ Allgemeine Bedienung und Tastenkürzel
*   ⇨ Übersicht im Menü Verkauf
*   ⇨ Angebote
*   ⇨ Aufträge
*   ⇨ Lieferscheine
*   ⇨ Rechnungen
*   ⇨ Gutschriften
*   ⇨ Auftragsfreischaltung
*   ⇨ Druck
*   ⇨ Übersicht-Funktionen im Verkauf
*   ⇨ Wiedervorlagen
*   ⇨ Modifikations-Funktionen im Verkauf

### Inhaltsverzeichnis

*   **Einführung** D-982
*   **Allgemeine Bedienung und Tastenkürzel** D-983
    *   Bedienung im Auftrag D-983
    *   Tastenkürzel D-984
    *   Glossar D-985
    *   Vorgänge suchen D-986
*   **Übersicht im Menü Verkauf** D-988
*   **Angebote** D-989
*   **Aufträge** D-991
    *   Auftrags-Kopf- und Fußbereich D-992
    *   Auftrag neu erfassen D-992
    *   Auftrag mit Bezug erfassen D-996
    *   Auftrag mit Kommissionen D-997
    *   Adressen im Auftrag D-999
    *   Texte und Floskeln erfassen D-1000
    *   Zusatz-Dokumente im Auftrag D-1001
    *   Auftragserfassung abschließen D-1002
    *   Auftragsänderung/Korrektur durchführen D-1003
*   **Positionserfassung** D-1006
    *   Neue Positionen anlegen D-1007
    *   Positionen erfassen (nach Produktart) D-1013
    *   Stückliste bearbeiten D-1016
    *   Sprossenerfassung D-1024
    *   Stufenerfassung D-1028
    *   iTOE - Erfassung und Nachbearbeitung D-1031
    *   Produktaustausch D-1035
*   **Preislose Erfassung** D-1038
    *   Preiskalkulation D-1038
    *   Preislose Erfassung D-1038
*   **Lieferscheine** D-1041
*   **Rechnungen** D-1042
*   **Gutschriften** D-1043
*   **Auftragsfreischaltung** D-1044
*   **Druck** D-1046
    *   Listendruck D-1048
*   **Übersicht-Funktionen im Verkauf** D-1049
    *   Übersicht D-1049
    *   Auftragsinformation D-1049
    *   Hintergrund-Kontrollen D-1050
*   **Wiedervorlagen** D-1051
*   **Modifikations-Funktionen im Verkauf** D-1054
    *   Vorgangsänderung D-1055

## Einführung

Das Tutorial zum Modul Verkauf beschäftigt sich mit der Arbeit in der Verkaufsabteilung, deren Handlungsschritte in A+W Enterprise abgebildet sind. Das Tutorial baut auf den Kenntnissen zu den Artikel-Stammdaten und allgemeinen kaufmännischen Grundlagen auf.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

### Vorausgesetzte Kenntnisse

Das Tutorial richtet sich an Anwender, die im Bereich Verkauf tätig sind, täglichen Kontakt zu eigenen Kunden und Lieferanten haben und eine zentrale Stelle in A+W Enterprise für alle Betriebsabläufe bilden.

Die Teilnehmer müssen das Konzept des Verkaufs und die Bedienelemente kennen, mit denen Funktionen aufgerufen und gestartet werden. Die Grundlagen der Bedienung sind im Part Überblick beschrieben.
⇨ Überblick, "" auf Seite A-52

### Ziel des Tutorials

*   Überblick über die Funktionen im Verkauf verschaffen.
*   Bedienschritte für ausgewählte Themen kennenlernen.

### Aufbau des Tutorials

Das Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

**Überblick**
Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
*   Lernziele: Was soll vermittelt werden?
*   Nutzen: Wofür können Sie dieses Wissen einsetzen?
*   Merksätze: Welche Zusammenhänge müssen Sie sich merken?

**Konzepte**
Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.

## Allgemeine Bedienung und Tastenkürzel

A+W Enterprise lässt sich im Allgemeinen sowohl über die Tastatur als auch mit Mausunterstützung bedienen. Der schnelle Auftragserfasser arbeitet vorwiegend mit den Tasten bzw. mit Tastenkombinationen. Das Verlassen eines Feldes, um sich im Dialog weiter bewegen zu können, erfolgt in der Regel über die Taste [Enter].

In folgenden Kapiteln finden Sie die wichtigsten Abläufe und häufig verwendete Tasten bzw. Tastenkombinationen:
⇨ "Bedienung im Auftrag" auf Seite D-983
⇨ "Tastenkürzel" auf Seite D-984
⇨ "Glossar" auf Seite D-985
⇨ "Vorgänge suchen" auf Seite D-986

### Bedienung im Auftrag

*[Diagram of "Ablaufschema der Vorgangserfassung". Shows flow from Kopfdaten -> Rumpfdaten -> Fußdaten, with options to go back (Pos1/F12) or forward (Ende). Final options are "Auftrag verwerfen" or "Auftrag speichern".]*
**Abb. D-1 Ablaufschema der Vorgangserfassung**

Der Ablauf der Vorgangserfassung unterliegt einem bestimmten Schema. Das Zusammenspiel der Tasten `<Pos1>`/`<F12>` und `<Ende>` bestimmt, wie weit die Vorgangserfassung geht und mit welchem Ergebnis die Erfassung beendet wird.
*   Mit `<Enter>` bewegen Sie sich von Feld zu Feld und wechseln von einer Erfassungsebene zu der anderen, z. B. von der Kopfebene zu der Rumpfebene.
*   Mit `<Pos1>` oder `<F12>` gelangen Sie in den übergeordneten Bereich, bzw. verwerfen den Auftrag.
*   Mit `<Ende>` gelangen Sie in den untergeordneten Bereich, bzw. speichern den Auftrag.

### Tastenkürzel

In der folgenden Tabelle sind die häufigsten und konstante Tasten aufgelistet. Die Tabelle hat an dieser Stelle keinen Anspruch auf Vollständigkeit. In der Regel können Sie innerhalb von einem Dialog diverse andere Tasten und Tastenkombinationen nutzen, die entsprechend erwähnt werden:

| Taste | Erklärung |
| :--- | :--- |
| `<Enter>`/`<Return>` | Damit verlassen Sie ein Feld, bzw. einen Dialog und bestätigen Ihre Eingabe. |
| `<Pos1>` | Damit verlassen Sie ein Feld, bzw. einen Dialog und verwerfen Ihre Eingabe. |
| `<F1>` | Damit starten Sie die Online-Hilfe. |
| `<F2>`/`<Mode>` | Damit wechseln Sie zwischen Mode-Dialogen, sofern diese vorhanden sind. |
| `<F3>`/[Start] | Damit führen Sie eine Aktion aus. |
| `<F4>` | Damit starten Sie das Zusatzmenü. |
| `<F5>` | Damit starten Sie die detaillierte Information zu dem aktuellen Datensatz, sofern diese vorhanden ist. |
| `<F6>` | Damit fügen Sie eine neue Zeile bzw. einen neuen Satz ein. |
| `<F7>` | Damit löschen Sie die Zeile bzw. den Feldinhalt. Je nach Kontext können Sie mit [F7] auch den aktuellen Satz löschen. |
| `<F8>` | Damit springen Sie zu dem ersten Satz in einem Treffermenge-Dialog. Je nach Kontext starten Sie mit [F8] eine Matchcode-Suche. |
| `<F9>` | Damit starten Sie die Suche nach einem Wert. |
| `<F10>` | Damit springen Sie zu dem letzten Satz in einem Treffermenge-Dialog. |
| `<F11>` | Damit können Sie von einem Bereich zu einem anderen springen, sofern die Bereiche festgelegt sind, wie z. B. in der Vorgangserfassung. Auf diese Weise werden etliche Felder im Dialog übersprungen. |
| `<F12>` | Damit bewegen Sie sich in einem Dialog rückwärts. |
| `<Ende>` | Damit verlassen Sie einen Dialog und speichern die Änderungen. |

### Glossar

| Begriff | Erklärung |
| :--- | :--- |
| **Vorgangsart** | Alle kaufmännische Dokumenten werden programmintern in der Datenbank-Tabelle kauf gespeichert. Diese Dokumente werden nach ihrer Art unterschieden. Die Nummer der Vorgangsart wird vom System automatisch vergeben und hat jeweils die feste Zuordnung: <br> - (Lieferanten-) Anfragen (kauf.vorgang=1) <br> - Bestellungen (kauf.vorgang=2) <br> - Wareneingänge (kauf.vorgang=3) <br> - Angebote (kauf.vorgang=4) <br> - Aufträge (kauf.vorgang=5) <br> - Lieferscheine (kauf.vorgang=6) <br> - Rechnungen (kauf.vorgang=7) <br> - EK-Rechnungen(kauf.vorgang=8) <br> - Gutschriften (kauf.vorgang=9) <br> - EK-Gutschriften (kauf.vorgang=10) <br> - Produktsets (kauf.vorgang=14) |
| **Auftragsart** | Man unterscheidet zwischen verschiedenen Arten eines Auftrages. Je nachdem, um welche Auftragsart es sich handelt, werden die Aufträge im System unterschiedlich behandelt: <br> - normal (kauf._kaufart=0) <br> - hausintern (kauf._kaufart=1) <br> - kostenlos (kauf._kaufart=2) <br> - Reservierung (kauf._kaufart=3) <br> - Vorabauftrag (NIU) (kauf._kaufart=4) <br> - Vorabrechnung (NIU) (kauf._kaufart=5) <br> - Vorabgutschrift (NIU (kauf._kaufart=6) <br> - Kalkulationstyp (kauf._kaufart=7) <br> - gruppenintern (kauf._kaufart=8) <br> - Abrufauftrag (kauf._kaufart=9) <br> - Lagerauftrag (kauf._kaufart=10) <br> - Chefauftrag (kauf._kaufart=11) <br> - Ersatzauftrag (kauf._kaufart=12) <br> - Referenz-Preisliste (kauf._kaufart=13) <br> - Vorab-Internetauftrag (kauf._kaufart=14) <br> - Bruchauftrag (kauf._kaufart=15) <br> - Kunden-Stapelauftrag (kauf._kaufart=16) <br> - Lager-Stapelauftrag (kauf._kaufart=17) <br> - Versandauftrag (kauf._kaufart=18) <br> - Gestrech (NIU) (kauf._kaufart=20) <br> - Rücknahmeauftrag (kauf._kaufart=21) |

### Vorgänge suchen

**Lernziele**
*   A+W Enterprise Vorgangssuche kennenlernen.
*   Bedienung im Dialog beherrschen.
*   Tipps und Tricks der Suchfunktion beachten.
*   Nutzen der Funktion erkennen.

**Nutzen**
Die Vorgangssuche ist eine der zentralen Funktionen nicht nur im Verkauf, sondern auch im Gesamtprogramm A+W Enterprise. Die Suche nach einem bestimmten Vorgang anhand weniger bekannter Kriterien ermöglicht die schnelle Erledigung von Aufgaben im täglichen Arbeitsablauf.

**Merke**
*   **Direkte Suche**: Unter diesen Begriff fällt die ältere direkte `<F9>`-Suche nach Vorgangsnummern. Dabei ist nur die Startwert-Nummereingabe möglich. Diese Suchmöglichkeit muss im Bedarfsfall explizit aktiviert werden.
*   **Erweiterte Suche**: Diese Suche ist bereits eine Standardfunktion in A+W Enterprise. Es handelt sich dabei um eine Suchmöglichkeit mit der Eingabe mehrerer Suchkriterien.
    ⇨ "Suche Aufträge" auf Seite D-1077

Es ist möglich, über die Suchfunktion bereits erfasste und gespeicherte Vorgänge (z. B. Angebote oder Aufträge) zu finden. Mit `<F9>` starten Sie aus einem Vorgangsfeld den Such-Dialog, deren Felder im folgenden Kapitel beschrieben sind:
⇨ Verkauf, "Suche Aufträge" auf Seite D-1077

#### So suchen Sie nach einem Auftrag

1.  Öffnen Sie den Dialog Verkauf -> Auftragserfassung.
2.  Starten Sie den Such-Dialog im Feld Auftrag mit `<F9>`. Der Dialog öffnet das erste Register Vorgangs-Schlüssel.
3.  Suchen Sie den Vorgang folgendermaßen:
    *   Geben Sie im Feld Aufträge ab die Vorgangsnummer ein, wenn diese bekannt ist.
    *   Geben Sie weitere Suchkriterien ein (beispielsweise die Fremdnummer des Kunden), wenn Sie die Suche weiter einschränken wollen.
    *   Sie können mit `<F2>` in das Register Positions-Schlüssel wechseln, um dort ebenfalls einige Suchkriterien einzugeben.
    *   Mit `<F3>` starten Sie die Suche.
    *   Oder, wenn Sie noch mit der alten Such-Logik arbeiten, startet der Dialog mit dem Register Direkte Suche.
        *   Geben Sie im Feld Aufträge ab die Vorgangsnummer ein, wenn diese bekannt ist.
        *   Mit `<F3>` starten Sie die Suche.
    *   Oder betätigen Sie `<Strg>` + `<T>`, um die Vorgangs-Recherche zu öffnen.
        *   Geben Sie die Suchkriterien ein (beispielsweise die Fremdnummer des Kunden).
        *   Mit `<F3>` starten Sie die Suche.
    *   Laden Sie den gewünschten Vorgang mit `<F3>` auf den Bildschirm.
    *   Oder betätigen Sie `<F5>`, um nach der Fremdnummer zu suchen.
    *   Oder betätigen Sie `<Shift>` + `<F5>`, um nach der Kommission zu suchen.
4.  Bestätigen Sie die Auswahl mit `<Enter>`.
5.  Falls eine Meldung angezeigt wird, dass der Vorgang nicht gefunden wurde bzw. vom System bearbeitet wird, korrigieren Sie die Suchkriterien oder starten Sie die Suche nach einem kurzen Zeitraum erneut.

> **Vorgangssuche mit `<F8>`**
> Die Such-Möglichkeit mit `<F8>` für Vorgänge wurde in A+W Enterprise angepasst: jeder Anwender kann nun mit `<F8>` im Feld Auftrag seine zuletzt erfassten Vorgänge ansehen. Es ist über eine Umgebungsvariable konfigurierbar, wie viele Tage in die Vergangenheit die Vorgänge als zuletzt erfasste gelten sollen.

## Übersicht im Menü Verkauf

*[Screenshot of the "Verkauf" menu in A+W Enterprise. It lists options from 'a Schnellerfassung' to 'r Vertrieb'.]*
**Abb. D-2 Menü Verkauf**

In diesem Modul finden Sie eine Übersicht über die Funktionen zu kaufmännischen Schritten, die in der Verkaufsabteilung vorkommen. Diese Dokument umfasst folgende Kapitel:
*   Angebote
*   Aufträge
*   Preislose Erfassung
*   Lieferscheine
*   Rechnungen
*   Gutschriften
*   Auftragsfreischaltung
*   Druck
*   Übersicht-Funktionen im Verkauf
*   Wiedervorlagen
*   Modifikations-Funktionen im Verkauf

> **Umfang des Tutorials im Bereich Verkauf**
> Die Anzahl der Funktionen und deren Vielfalt ist im Bereich Verkauf sehr umfangreich. Dieses Tutorial umfasst nur ausgewählte Themen und hat keinen Anspruch auf die Vollständigkeit. Das Tutorial wird ständig überarbeitet.

Viele Funktionen und Handlungsschritte sind in allen bzw. mehreren Vorgangsdialogen nutzbar. Solche Themen werden ausschließlich in dem Kapitel Auftragserfassung beschrieben.

## Angebote

**Lernziele**
*   A+W Enterprise-Funktionen zur Angebotserfassung kennenlernen.
*   Bedienung in der Angebotserfassung, sofern Unterschiede zur Auftragserfassung bestehen, beherrschen.
*   Unterschiede zwischen Angeboten und Aufträgen verstehen.
*   Funktionsnutzen und die Folgen erkennen.

**Nutzen**
Als Angebot wird eine empfangsbedürftige Willenserklärung bezeichnet, die alle vertragswesentlichen Bestandteile umfasst und durch die einem anderen der Vertragsschluss so angetragen wird, dass das Zustandekommen des Vertrages nur noch von dem Einverständnis des Empfängers abhängt. A+W Enterprise bietet daher alle kaufmännische Funktionen, um ein umfangreiches Kundenangebot erstellen zu können.

> **Merke: VOKA**
> Der Zutritt zu dem Dialog Auftragserfassung wird durch das EDV-Modul-Kürzel VOKA gesteuert. Diverse andere Einschränkungen innerhalb der Auftragserfassung erfragen Sie bei einen A+W-Mitarbeiter.

In der Angebotserfassung können Sie aus der Vielzahl der Produkte ein komplettes Angebot ganz nach Kundenwunsch erstellen. Dieses Angebot bekommt eine Angebotsnummer zugeteilt und wird unter dieser Nummer abgespeichert.
⇨ Verkauf, "Angebotserfassung" auf Seite D-1132

Der wesentliche Unterschied zwischen einem Angebot und einem Auftrag liegt darin, dass bei der Erfassung eines Angebots kein Liefertermin erforderlich ist. Auf weitere Unterschiede wird im Kapitel explizit eingegangen.

Wenn Sie in einem Angebot einen Liefertermin eintragen, kann dieser zu einer Wiedervorlage oder zum Löschen des Angebots führen, sofern Sie das im System konfigurieren.
⇨ Verkauf, "Wiedervorlagen" auf Seite D-1051

Eine weitere Vereinfachung im Angebot ist bei der Bearbeitungserfassung gegeben. Möchte Ihr Kunde ein Angebot mit mehr als einer gleichen Bearbeitung am Glas kalkulieren lassen z. B. mit mehreren Bohrungen, so müssen Sie diese Bohrungen im Angebot nicht einzeln vermaßen. Sie tragen nur die gewünschte Menge bei der Bearbeitung ein. Entsteht einschließlich aus diesem Angebot ein Auftrag, wird diese Bearbeitung vervielfacht, um sie einzeln für die Produktion zu vermaßen.

Darüber hinaus erhalten Sie in der Angebotserfassung einen Überblick über die Produktionsauslastung. Diese Funktion bietet Ihnen die Möglichkeit, während der Erfassung bei größeren Angeboten auf die Produktionsfristen zu achten und so die Lieferterminverschiebungen zu vermeiden. Diese Funktion muss im System separat konfigiert werden. Bei Interessen wenden Sie an einen A+W-Mitarbeiter.

Ein Angebot verfügt über einen Ablaufstatus. Das Feld `Angeb. Status` finden Sie im Angebot > Dialogkopf > Register Verschiedenes.
Folgende Auswahlmöglichkeiten stehen zur Verfügung:
*   **offen**
    Dieser Status wird automatisch in einem neuen Angebot gesetzt.
*   **gewonnen**
    Dieser Status wird automatisch in einem Angebot gesetzt, sobald ein Auftrag mit Bezug auf das aktuelle Angebot erstellt wird.
*   **verloren**
    Dieser Status muss manuell in einem neuen Angebot gesetzt werden, wenn der Kunde dem Angebot nicht zustimmt. Sie können das System so konfigurieren, dass solche Angebote nach einem bestimmten Zeitraum gelöscht werden. Weiter Information entnehmen Sie dem folgenden Kapitel:
    ⇨ Verkauf, "Wiedervorlagen" auf Seite D-1051
*   **unentschlossen**
    Dieser Status kann nur manuell gesetzt werden und wird für interne Kundenauswertungen genutzt.

## Aufträge

Mit der Auftragserfassung nehmen Sie die eingehenden Kundenwünsche auf und übergeben diese anschließend dem System zur weiteren Bearbeitung. Die erforderlichen Bearbeitungen werden unter Berücksichtigung des vom Kunden gewünschten Liefertermins disponiert. Die am Lager befindlichen Teile werden für den Auftrag reserviert, während die Zukaufware dem Einkauf zur Bestellung übergeben wird. Anschließend wird ein Auftrag an die Produktion übergeben. Am Ende der Produktionskette steht der Auftrag im Versand zur Auslieferung bereit und kann abgerechnet werden. Der Prozess wird mit den notwendigen Papieren begleitet. Die möglichen Änderungen werden vor der Anpassung auf die Ausführbarkeit geprüft. Auch die gesetzlichen Bestimmungen sind im Programm enthalten.

Der Funktionsbestand ist in der Auftragserfassung sehr umfangreich. Viele Handlungsschritte sind konfigurationsabhängig. Nicht zu letzt haben auch die Stammdaten bestimmte Auswirkungen in der Auftragserfassung. In den folgenden Kapiteln werden sofern wie möglich die Bedien- und Konfigurations-Voraussetzungen explizit beschrieben.

Die Auftragserfassung wird in A+W Enterprise in drei Bereiche untergliedert:
*   Kopfdaten
*   Rumpfdaten
*   Fußdaten

In diesen Bereichen werden die oft verwendeten Funktionen beschrieben. Besonders dokumentationsumfangreiche Funktionen sind in extra Kapiteln zu finden, wie z. B.:
⇨ Verkauf, "iTOE - Erfassung und Nachbearbeitung" auf Seite D-1031
⇨ Verkauf, "Produktaustausch" auf Seite D-1035

In den Kopfdaten werden generelle marktpartnerspezifische Daten erfasst oder aus den Marktpartnerstammdaten ermittelt.
⇨ Verkauf, "Auftrags-Kopf- und Fußbereich" auf Seite D-992

In den Rumpfdaten werden die Positionen eingegeben. Sie beinhalten die Produktinformationen.
⇨ Verkauf, "Positionserfassung" auf Seite D-1006

In den Fußdaten wird die Erfassung des Angebots oder Auftrags abgeschlossen. Die Auftragssumme wird gebildet sowie Rabatte und Zuschläge ermittelt.

Die genauen Feldbeschreibungen der Felder in dem Dialog Auftragserfassung entnehmen Sie bitte dem folgenden Kapitel in der Softwarereferenz:
⇨ Verkauf, "Auftragserfassung" auf Seite D-1134

In diesem Kapitel erfahren Sie, wie Sie Aufträge erfassen. Wenn Sie ein Angebot erfassen möchten, öffnen Sie im Menü Verkauf > Angebotserfassung.

### Auftrags-Kopf- und Fußbereich

**Lernziele**
*   Vielfalt der A+W Enterprise-Funktionen im Auftragsumfeld kennenlernen.
*   Stammdaten-Anhängigkeit und Erfassungs- bzw. Änderung dieser Daten im Auftrag verstehen.
*   Nutzen einiger wichtigen Funktionen erkennen.

**Nutzen**
Die Auftragserfassung ist der Kern des gesamten A+W Enterprise. Die Auftragserfassung bildet die Grundlage von kaufmännischen, produktionsbezogenen und auch rechtlichen Prozessen. Die Funktionen, die global in einem Auftrag gelten, werden dem Auftragskopf zuordnet. Auftragsabschließende Handlungen sind im Fußbereich zusammengefasst.

> **Merke: VOKA**
> Der Zutritt zu dem Dialog Auftragserfassung wird durch EDV-Modul-Kürzel VOKA gesteuert. Diverse andere Einschränkungen innerhalb der Auftragserfassung erfragen Sie bei einen A+W-Mitarbeiter.

Im Kopfbereich legen Sie die Grundlage für einen Auftrag fest. Zunächst wird die Auftragsnummer vom System automatisch vergeben. Die Nummernvergabe erfolgt über so genannte Nummernkreise, die bei der Installation bzw. Konfiguration festgelegt werden. Die Nummern für die Aufträge sind nicht lückenlos: wird ein Auftrag verworfen und bereits ein Folgeauftrag erfasst, so wird die verworfene Nummer nicht erneut verwendet. Diese Logik findet jedoch nicht in der Rechnungs- und Gutschrifterfassung Anwendung.

#### Auftrag neu erfassen

**So erfassen Sie einen Auftrag**
1.  Öffnen Sie den Menüpunkt Verkauf > Auftragserfassung. A+W Enterprise zeigt den ausgewählten Dialog an.
2.  Betätigen Sie `<Enter>` im Feld Auftrag (bzw. Angebot). A+W Enterprise vergibt die nächste freie Vorgangsnummer automatisch und zeigt diese an. Der Cursor springt in das Feld Kunde.
    ⇨ Verkauf, "Auftrag" auf Seite D-1135
3.  Wählen Sie den Kunden folgendermaßen aus:
    *   Geben Sie die Kundennummer ein, wenn diese bekannt ist.
    *   Oder betätigen Sie die Taste `<F9>` für eine Suche nach der Kundennummer oder `<F8>` für eine Matchcode-Suche.
    Der Dialog Marktpartner-Suche öffnet sich. Der Cursor befindet sich im Feld Ab Nummer beim Start mit `<F9>`, oder im Feld Matchcode beim Start mit `<F8>`:
    *   Geben Sie die Suchkriterien ein.
    *   Mit `<F3>` starten Sie die Suche.
    ⇨ Softwarereferenz, "Marktpartnersuche" auf Seite D-1091
    ⇨ Verkauf, "Kunde" auf Seite D-1136
4.  Erfassen Sie den Auftrag mit Bezug auf einen vorhandenen Vorgang, führen Sie nachfolgend beschriebene Schritte aus:
    ⇨ Verkauf, "So erfassen Sie einen neuen Auftrag mit Bezug auf einen bestehenden Angebot oder Auftrag" auf Seite D-996
5.  Gehen Sie mit der Taste `<Enter>` die Felder bis zu Termin durch. Wenn Sie als Erfassungs-Datum ein anderes als Heute () eingeben müssen, verlangt das Programm die doppelte Eingabe.
6.  Erfassen Sie den vom Kunden gewünschten Liefertermin im Feld Termin als KW (Kalenderwoche) oder als ein festes Datum. Die Eingabe des Liefertermins ist nur bei einem Auftrag zwingend. Beachten Sie die Folgen der Liefertermin-Eingabe bei Angeboten:
    ⇨ Verkauf, "Wiedervorlagen” auf Seite D-1051
    Wenn Sie mit dem Tourenplan arbeiten, können Sie auch direkt einen Tourentag auswählen. Um alle Tourentage innerhalb der ausgewählten Lieferwoche anzuzeigen, drücken Sie `<F9>` und wählen Sie den Wunschtermin aus. Diese Funktion ist nur dann möglich, wenn Sie mit dem Tourenplan arbeiten.
    ⇨ Stammdaten, "Tourenplan" auf Seite B-263
    Aufgrund mehreren Kriterien, wie z. B. Kalendereinträge, Route-Fahrtage, Fahrt- und Handlingszeit, errechnet das Programm direkt einen geplanten Liefertermin. Die mögliche Verschiebung durch die Produktion findet erst bei Auftragsübergabe statt.
7.  Ordnen Sie den aktuellen Vorgang einem Objekt zu (optional), um objektspezifische Sondervereinbarungen für diesen Vorgang zu berücksichtigen.
    *   Betätigen Sie `<F9>` im Feld Objekt. Wählen Sie in der Liste das gewünschte Objekt aus.
    Alle objektbezogenen Felder werden aus den Stammdaten ermittelt.
8.  Erfassen Sie Kommissionen (optional), um kommissionsbezogene Texte einzugeben.
    ⇨ Verkauf, "Auftrag mit Kommissionen" auf Seite D-997
9.  Mit einem weiteren `<Enter>` gelangen Sie in die Positionserfassung. Nutzen Sie dafür nachfolgend beschriebene Schritte:
    ⇨ Verkauf, "So erfassen Sie eine Position mit Artikelnummer" auf Seite D-1007

**So beeinflussen Sie die Eilzuschlagsberechnung**
1.  Erfassen Sie einen Auftragskopf bis zum Feld Termin.
2.  Geben Sie im Feld Termin ein naheliegendes Datum ein.
    Sie können in der Systemkonfiguration die Eilfrist bestimmen, d. h. bis zu wie vielen Tage in die Zukunft gelten Aufträge als Eilaufträge.
    Das ausgewählte Datum muss in dem Zeitraum zwischen HEUTE() + Eilfrist liegen.
3.  Wählen Sie im Feld Term. Art den Wert `eilt` aus.
4.  Erfassen Sie den Auftrag bis zum Feld Rabatt im Auftragsfuß.
5.  Wechseln Sie mit `<F2>` in die Rabattübersicht. Wenn Sie einen Eilauftrag-Zuschlag hinterlegt haben, wird dieser automatisch ermittelt.
    Einen Eilauftrag-Zuschlag sollen Sie im Vorfeld unter Stammdaten > Schlüssel > Marktpartner > Vorgangsrabatte > Rabatte definieren.
    Zu beachten ist hier, dass nicht das Feld Eilauftrag im Register Eigenschaften für den Zuschlag ausgewertet wird.
    Sie können auch über das Menü `<F4>` > Preisangaben > Rabatte neu ermitteln alle Rabatte und Zuschläge erneut berechnen lassen.
6.  Erfassen Sie den Auftrag zu Ende.

**So können Sie den Auftrag zwischenspeichern**
Besonders bei größeren Aufträgen mit mehreren Positionen oder bei aufwändigen Erfassungen ist ratsam den betroffenen Auftrag zwischenzuspeichern. Der Vorteil an dieser Stelle ist, sofern ein Problem auftritt, wird bei einem Neustart auf den gesicherten Zustand zurückgegriffen.
1.  Erfassen Sie einen Auftragskopf bis zu der Stelle, an der Ihnen die Sicherung sinnvoll erscheint. Es muss jedoch mindestens eine Position vollständig erfasst werden, damit die Schaltfläche Sichern automatisch aktiviert wird.
    Dabei wird ein Datensatz in der Tabelle `kauf` mit `kauf.still=999` angelegt.
2.  Sie können den Auftrag noch zu einem späteren Zeitpunkt, z. B. nach der Erfassung weiterer Positionen erneut sichern.
    Dabei wird der zuerst gesicherte Datensatz in der Tabelle `kauf` überschrieben.
3.  Sofern ein Auftrag vollständig erfasst und gespeichert wird, wird das `kauf.still=-3` gesetzt und der Auftrag wird dem Hintergrundprozess `intauf` zur weiteren Bearbeitung vorgelegt. Alternativ kann der erfasste Auftrag auch in den Freischaltpool gestellt werden.
4.  Im Falle, dass die Erfassung durch ein technisches Problem abgebrochen wurde, so dass anschließend A+W Enterprise neue gestartet werden muss, bietet das Programm folgende Möglichkeit:
    *   Beim Starten der Auftragserfassung bekommen Sie einen Hinweis, dass noch Vorgänge existieren, deren Erfassung noch nicht abgeschlossen ist.
    *   Sofern Sie diesen Hinweis bestätigen, startet der Übersichts-Dialog der gesicherten Vorgänge:
        *[Screenshot of "Übersicht der gesicherten Vorgänge" dialog window]*
    *   In diesem Dialog werden alle Vorgänge dargestellt, deren Erfassung nicht zu Ende durchgeführt wurde und zu denen jeweils eine Sicherung existiert.
    *   Mit [Abbrechen] schließen Sie diesen Übersichts-Dialog und kehren zum Dialog Auftragserfassung zurück. Sie können noch nicht zu Ende erfasste Vorgänge zu einem späteren Zeitpunkt weiter bearbeiten. Dieser Übersichts-Dialog startet immer beim Betreten der Auftragserfassung, solange noch weitere Vorgänge existieren.
    *   Mit [OK], bzw., vorheriger Vorgangsauswahl, sofern mehrere Vorgänge existieren, starten Sie den Vorgang für die weitere Erfassung. Es wird der zuletzt gesicherte Stand des Vorgangs wiederhergestellt.
    **Einschränkungen**
    Bitte beachten Sie folgende Einschränkungen:
    *   die gesicherte Vorgänge werden maximal 30 Tage im System aufgehoben,
    *   in dem Übersichts-Dialog werden nur die eigene Vorgänge, also nicht die von anderen Benutzer, aufgelistet,
    *   die Funktion Sichern für Angebote, Aufträge, Anfragen und Bestellungen zur Verfügung steht.
5.  Anschließend können Sie den Vorgang weiter erfassen.

#### Auftrag mit Bezug erfassen

Sie können einen neuen Auftrag (oder Angebot) mit Bezug auf ein vorhandenes Angebot oder Auftrag erfassen. Dabei werden die Daten des Bezugsvorgang kopiert und Sie können diese dann in dem neuen Vorgang anpassen bzw. weiter bearbeiten. Als Bezugsvorgang kann ein Auftrag oder ein Angebot jedes beliebigen Kunden genommen werden. In seltenen Fällen kann auch eine Lieferantenanfrage oder eine Bestellung in den Verkaufsvorgang umgewandelt werden. Dabei müssen die Daten des neuen Vorgangs sorgfältig geprüft werden.
⇨ Verkauf, "Vorgangsart für den Bezug vorauswählen" auf Seite D-1136

Beachten Sie, dass Sie anschließend gegebenenfalls einige Informationen, wie z. B. den Liefertermin im Feld Termin sowie die Kommissionstexte anpassen müssen. Gegebenenfalls muss der Vorgang neu kalkuliert werden. Dies gilt vor allem, wenn Sie Vorgänge anderer Kunden in den Auftrag kopieren.

**Ein Auftrag mit Bezug auf Angebot für den selben Kunden erfassen**
Wenn Sie ein Angebot des selben Kunden in einen Auftrag umwandeln möchten, dann können Sie die Angebotsnummer direkt im Feld Bezug eingeben. Die vorhandenen Daten aus dem bestehenden Angebot werden in den Dialog geladen. Diese Vorgehensweise ist jedoch nur dann möglich, wenn das System für den Standard-Bezugsvorgang=Angebot konfiguriert ist.

Das Angebot erhält durch A+W Enterprise automatisch den Angebotsstatus `gewonnen` (Angebot > Register Verschiedenes > Feld Angeb.Status = gewonnen). Diese Information kann bei Bedarf für kundenindividuelle Auswertungen bzw. Statistiken verwendet werden.

**So erfassen Sie einen neuen Auftrag mit Bezug auf einen bestehendes Angebot oder Auftrag**
1.  Starten Sie den Dialog Auftragserfassung. Mit `<Enter>` im Feld Auftrag vergeben Sie eine neue Auftragsnummer.
2.  Geben Sie die gewünschte Kundennummer ein oder wählen Sie diese aus.
3.  Gehen Sie im Feld Bezug folgendermaßen vor:
    *   Wählen Sie mit `<F8>` die Vorgangsart des Vorgang, auf den Bezug genommen wird. Die Standard-Voreinstellung für die Vorgangsart wird in den Systemeinstellungen festgelegt und entsprechend hier angezeigt. Sie können den Standardwert mit `<Enter>` bestätigen.
    *   Oder, um eine andere Vorgangsart auszuwählen, betätigen Sie `<F9>`.
        *   Wählen Sie aus der Liste die Vorgangsart des Bezugsvorgang aus.
        *   Bestätigen Sie die Auswahl mit `<Enter>`.
    *   Als nächstes wird die Kundennummer in das Feld aus dem neuen Auftrag übernommen. Sie können die aktuelle Kundennummer mit `<Enter>` bestätigen.
    *   Um sich auf den Vorgang eines anderen Kunden zu beziehen, geben Sie dessen Kundennummer ein oder öffnen Sie die Marktpartner-Suche mit `<F9>`. Bei Lieferantenanfragen und Bestellungen werden nur die Lieferanten zur Auswahl angezeigt.
    *   Bestätigen Sie die Auswahl mit `<Enter>`.
    *   Nun geben Sie die Vorgangsnummer ein oder suchen Sie alle Vorgänge mit der gewählten Vorgangsart dieses Kunden mit `<F9>`.
    *   Bestätigen Sie die Auswahl und verlassen Sie das Feld Bezug mit `<Enter>`.
    Im Feld Bezug wird die Vorgangsnummer angezeigt.
4.  Die Daten des gewählten Referenzvorgangs können entweder komplett oder auch nur die Kopfdaten in den neuen Vorgang kopiert werden.
5.  Außerdem können einigen Daten neu ermittelt bzw. berechnet werden, z. B.:
    *   **Neukalkulation des zu erfassenden Auftrags:**
        Die Abfrage nach der Neukalkulation wird in einem separaten Dialog gestellt. Diese Abfrage ist immer mit dem Wert `Keine Neukalkulation` vorbelegt. Über eine Systemeinstellung können Sie diese Voreinstellungen selbst bestimmen. Folgende Werte sind zulässig:
        *   0 - Keine Neukalkulation (Standardeinstellung)
        *   1 - VK + EK Preise
        *   2 - VK-Preise
        *   3 - EK-Preise
        So können Sie konfigurieren, welcher Wert bei der Erfassung mit Bezugnahme vorbelegt wird. Darüber hinaus können Sie bestimmen, welcher Wert vorbelegt wird, wenn in dem neuen Vorgang die Neukalkulation im Kopf oder in der Position aufgerufen wird, sofern diese Funktion genutzt wird.
    *   **Rabattermittlung in dem zu erfassenden Auftrag:** Existieren marktpartnerbezogene Rabatte im Vorgang und die Vorgangserfassung mit Bezugnahme ruft einen Marktpartnerwechsel hervor, können Sie entscheiden, ob die Rabatte neu berechnet werden. Durch eine Programmmeldung werden Sie dazu aufgefordert.
6.  Sie können die Auftragserfassung nun fortsetzen, ggf. nutzen Sie dafür die Information, wie sie in den folgenden Kapiteln beschrieben sind:
    ⇨ Verkauf, "So erfassen Sie einen Auftrag" auf Seite D-992
    ⇨ Verkauf, "Neue Positionen anlegen" auf Seite D-1007

#### Auftrag mit Kommissionen

Eine Kommission ist die Gruppierung von bestimmten Positionen eines Auftrags unter einem Titel. Je nachdem, wie das Feld Kommission konfiguriert ist, springt der Cursor nach dem Feld Objekt in das Feld Kommission oder das Feld wird übersprungen und Sie können direkt die erste Position erfassen.
⇨ Verkauf, "Kommis" auf Seite D-1169

**So erfassen Sie einen Kommissionstext**
Hier können Sie einen kommissionsbezogenen Text eingeben, der sowohl auf den Unterlagen als auch auf dem Etikett ausgedruckt werden kann.
1.  Starten Sie die Auftragserfassung und erfassen Sie die Daten im Auftragskopf, wie in folgenden Kapitel beschrieben ist:
    ⇨ Verkauf, "So erfassen Sie einen Auftrag" auf Seite D-992
2.  Geben Sie den Kommissionstext im Feld `Kommis.` ein. Der Text kann über die sichtbare Feldlänge hinausgehen. Nutzen Sie die `<Pfeiltasten>` (links/rechts), um den Text einzusehen.
3.  Bestätigen Sie die Eingabe mit `<Enter>`. Diese Kommission gilt für den gesamten Auftrag. Wenn Sie einen positionsgenauen Kommissionstext erfassen möchten, folgend Sie auf der Positionsebene dem Menüpfad `<F4>` Kommissionen > neue Kommission.
    Der Cursor springt auf die erste Position im Register Allgemein.

**So legen Sie weitere Kommissionstexte an**
Die Kommissionstexte bleiben für die nachfolgenden Positionen so lange unverändert erhalten, bis ein neuer Kommissionstext angelegt wird. Wenn Sie für die nachfolgenden Positionen einen neuen Kommissionstext anlegen möchten, können Sie diesen wie folgt eingeben.
⇨ Verkauf, "Auftragspositionen – Allgemein" auf Seite D-1167
1.  Drücken Sie in der zu ändernden Position im Register Allgemein `<Shift>` + `<F11>`. Der Cursor springt in das Feld Kommis.
2.  Ändern Sie den Kommissionstext wie gewünscht und bestätigen Sie die Eingabe mit `<Enter>`. Der Cursor springt zurück in die Position im Register Allgemein, die Sie gerade bearbeitet haben.

**So ändern Sie Kommissionstexte**
Sie können Kommissionstexte ändern oder korrigieren. Die Änderung bezieht sich auf alle Positionen, für die diese Kommission gültig ist, auch auf alle vorherigen.
1.  Drücken Sie in der zu ändernden Position im Register Allgemein `<Strg>` + `<F11>`.
    Oder rufen Sie mit `<F4>` das Zusatzmenü auf.
    *   Wählen Sie den Punkt Kommissionen.
    *   Wählen Sie den Untermenüpunkt Kommission ändern aus.
    Der Cursor springt in das Feld Kommis.
2.  Ändern Sie den Kommissionstext wie gewünscht und bestätigen Sie die Eingabe mit `<Enter>`. Der Cursor springt zurück in die Position im Register Allgemein, die Sie gerade bearbeitet haben.

### Adressen im Auftrag

Es ist möglich, für den Auftrag eine andere Lieferadresse, als die Adresse die aus den Stammdaten ermittelt wurde, zu erfassen oder auszuwählen. Die Feldbeschreibung zum Dialog Adressen finden Sie in folgendem Kapitel:
⇨ Stammdaten: Softwarereferenz, "Adressen" auf Seite B-140

Der Funktionsumfang für Ermittlung, Erfassung und Übernahme von Adressen in einen Vorgang ist sehr umfangreich. Eine Adressenänderung kann eine Folgenänderung in anderen Bereichen auslösen, wie z. B.:
*   Neuermittlung und Berechnung von Lieferzuschlägen, sowie anderen Rabatten,
*   Änderung der Art der DFÜ, sowie die bestellbezogenen Daten,
*   Erneute Übergabe an die Produktion, sofern es um produktionsrelevante Änderung handelt,
*   Auswirkung auf die Gestellplanung und Versandsteuerung, usw.

Es ist daher unbedingt zu beachten, dass die Änderungen einer bestehenden Adresse sich nicht nur auf einen bestehenden oder neuen Vorgang auswirkt, sondern u.U. auf eine Reihe von Vorgängen.

> **Adresslogik**
> Wenden Sie sich an einen A+W - Mitarbeiter, wenn Sie die Kunden- und Lieferadressen an Ihre Arbeitsweise anpassen und konfigurieren möchten.

**So wählen Sie eine andere Lieferadresse**
Sie können eine abweichende Lieferadresse für diesen Auftrag wählen oder eine neue erfassen.
⇨ Verkauf, "Neue Lieferadresse" auf Seite D-1192
1.  Betätigen Sie im Auftrag `<Strg>` + `<L>`.
    Oder rufen Sie mit `<F4>` das Zusatzmenü auf.
    *   Wählen Sie den Punkt Adressen.
    *   Wählen Sie den Untermenüpunkt Lieferadresse wählen.
    Der Dialog Adressen Suche startet.
2.  Im Such-Dialog können Sie die Suche auf bestimmte Kriterien eingrenzen. Die Dialog-Beschreibung entnehmen Sie folgendem Kapitel:
    ⇨ Verkauf, "Adressen Suche" auf Seite D-1099
3.  Wählen Sie mit der Maus oder den `<Pfeiltasten>` eine Adresse aus der Treffermenge aus und bestätigen Sie die Auswahl mit `<Enter>`.
4.  Schließen Sie den Dialog mit `<Ende>`. A+W Enterprise schließt den Dialog und übernimmt die gewählte Adresse als Lieferadresse in den Auftrag.

**So erfassen Sie eine neue Lieferadresse**
Sie können eine abweichende neue Lieferadresse für den Auftrag erfassen. Die neue Adresse kann als Einmaladresse (gültig nur in diesem Auftrag) oder zur weiteren Verwendung in die Stammdaten übernommen werden.
1.  Wählen Sie mit `<F4>` das Zusatzmenü > Adressen > Neue Lieferadresse auf.
2.  Füllen Sie die Felder für eine neue Adresse aus.
    Sie können eine vorhandene Adresse als Vorlage verwenden. Über die Schaltfläche `<Vorlage>` starten Sie wieder die Adressen-Suche, über die Sie eine neue Adresse zur Vorlage wählen können.
    Verändern Sie die Angaben, sofern nötig ist.
3.  Anschließend können Sie die neue Adresse mit `<F3>` im Marktpartnerstamm hinterlegen lassen. Alternativ wird die neue Adressen nach dem Speichern nur in diesem Auftrag gültig.
4.  Schließen Sie den Dialog mit `<Ende>`. A+W Enterprise schließt den Dialog und übernimmt die gewählte Adresse in den Auftrag als Lieferadresse.

**So löschen Sie eine Lieferadresse**
Sie können die Lieferadresse im Auftrag löschen.
1.  Rufen Sie im Auftrag mit `<F4>` das Zusatzmenü auf.
2.  Wählen Sie den Punkt Adressen.
3.  Wählen Sie den Untermenüpunkt Lieferadresse löschen und bestätigen Sie mit `<Enter>`. A+W Enterprise löscht die Lieferadresse aus dem Auftrag.

### Texte und Floskeln erfassen

Es besteht die Möglichkeit, an verschiedenen Programm-Stellen Texte zu erfassen und einzufügen. In den Regeln erfolgt die Generierung und Ausgabe der Texte automatisch auf Basis der Systemkonfiguration, der Stammdaten und anderer Einstellungen.

**So erfassen Sie Kopftext oder Auftrags-Fußtext**
Mit Hilfe dieses Menüpunktes können Sie in der Auftragserfassung im Zusatzmenü weitere Texte frei eingeben, die in den Kopfdaten oder Fußdaten der kundenseitigen Dokumente ausgedruckt werden.
⇨ Verkauf, "Untermenü Texte" auf Seite D-1070
⇨ Verkauf, "Kopf- und Fußtexte" auf Seite D-1313
1.  Rufen Sie mit `<F4>` das Zusatzmenü auf und wählen Sie den Punkt Texte.
2.  Wählen Sie den Untermenüpunkt Kopftext oder Fußtext aus.

