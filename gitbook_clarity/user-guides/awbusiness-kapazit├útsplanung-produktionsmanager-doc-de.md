---
description: "D-AWBusiness-HB_33"
---


# Softwarereferenz

---
## Leitstand - Arbeitsarten

**Fertigung > Kapazitätsplanung > Leitstand > Register Arbeitsarten**

*Abb. H-215 Leitstand - Arbeitsarten*

In diesem Register prüfen Sie, welche Arbeitsarten an einem Produktionstermin auf einer Maschine durchgeführt werden sollen.

Das Register ist nur gefüllt, wenn Sie sich Teile oder Vorprozesse haben anzeigen lassen.

### Navigation durch die Register

| Aktion | Register |
| :--- | :--- |
| Klick in Zeilenkopf | Details |

**[Teile]** Wechselt zur Darstellung der Positionen im Register Vorprozesse.

**[Vorprozesse]** Wechselt im Register Vorprozesse zur Darstellung der Vorprozesse.

---

## Übersicht

In der Übersicht werden folgende Daten angezeigt:

- **Nummer**: Nummer der Arbeitsart.
- **Vorgang**: Bezeichnung der Arbeitsart.
- **Artikel**: Bezeichnung des Produkts.
- **Schicht**: Schicht, in der diese Arbeitsart ausgeführt werden soll.
- **Stück**: Positionsmenge.
- **Verschieben**: Nur wenn Sie die Checkbox markiert haben, werden die Änderungen übernommen. Sind die Änderungen mit anderen Arbeitsgängen für diesen Auftrag unvereinbar, wird in einer Fehlermeldung angezeigt, dass ein Verschieben unmöglich ist.
- **Stunden**: Für diese Position reservierte Zeit.

### Verschieben

Die Felder in diesem Bereich sind zum Register Auftrag umlasten erklärt.
⇨"Leitstand - d – Auftrag umlasten" auf Seite H-348

---

## Leitstand - Details

**Fertigung > Kapazitätsplanung > Leitstand > Register Vorprozesse > Klick in Zeilenkopf > Register Details**

*Abb. H-216 Leitstand - Details*

In diesem Register werden detaillierte Informationen pro Schicht und Arbeitsart angezeigt.

### Navigation

| Aktion | Dialog |
| :--- | :--- |
| Doppelklick auf Auftragsnummer | -> Dialog Leitstand (Auftrag) |

---

## Übersicht

In der Übersicht werden folgende Daten angezeigt:

- **Auftrag, Kunde**: Auftragsnummer, Kundennamen aus dem Auftrag.
- **Pos.**: Positionsnummer aus dem Auftrag.
- **SL-ID**: Stücklisten-Identnummer, das ist die Stücklistenebene.
- **UP**: Unterpositionen (Pakete), die beim Einlasten durch Splitten der Position entstanden sind.
- **Produkt/Bearb.**: Produktbezeichnung.
- **Stück**: Positionsmenge.
- **Abmessungen**: Maße der Position.
- **Verschieben**: Nur wenn Sie die Checkbox markiert haben, werden die Änderungen übernommen. Sind die Änderungen mit anderen Arbeitsgängen für diesen Auftrag unvereinbar, wird in einer Fehlermeldung angezeigt, dass ein Verschieben unmöglich ist.
- **Stunden**: Für diese Position reservierte Zeit.

### Verschieben

Die Felder in diesem Bereich sind zum Register Auftrag umlasten erklärt.
"Leitstand - Auftrag umlasten" auf Seite H-348

---

## Leitstand – Schichten

**Fertigung > Kapazitätsplanung > Leitstand > Register Schichten**

*Abb. H-217 Leitstand – Schichten*

In diesem Register prüfen Sie die Belegung der Maschinen pro Schicht.

### Übersicht

In der Übersicht werden folgende Daten angezeigt:

- **Aggregat**: Maschine.
- **Schicht**: Pro Schicht wird eine Zeile angezeigt.
- **Wochentag, Datum**: Verplante Zeit und Schichtzeit in Stunden pro Schicht.

---

## Leitstand – Vorprozesse

**Fertigung > Kapazitätsplanung > Leitstand > Register Auftrag umlasten > [Teile], [Vorprozesse] > Register Vorprozesse**

*Abb. H-218 Leitstand – Vorprozesse*

In diesem Register prüfen Sie, aus welchem Produktionsbereich die Positionen kommen, zu denen Sie sich die aktuellen Daten anzeigen lassen. Die Daten können Sie sich in den Modi Teile und Vorprozesse anzeigen lassen.

### Navigation

| Aktion | Dialog |
| :--- | :--- |
| Klick auf Zeilenkopf | -> Spalte Auftrag wird angezeigt |

**[Im Detail]** Öffnet den Dialog Produktionslisten, in dem Sie prüfen können, mit welchen Aufträgen die vorherigen Maschinen ausgelastet sind.
⇨ "Produktionslisten" auf Seite H-318

**[Teile]** Wechselt zur Darstellung der Positionen.

**[Vorprozesse]** Wechselt zur Darstellung der Vorprozesse.

---

### Auswahl

In diesem Bereich werden die Anzahl und die Fläche der Teile insgesamt und pro Schicht angezeigt.

### Optionen

Sie können im Modus Vorprozesse zusätzliche Informationen anzeigen lassen:

- **Mit Bezeichnung**: In der Spalte Teile wird die Produktbezeichnung angezeigt.
- **Mit Arbeitsart**: In der Spalte vorige Arbeitsart wird die Arbeitsart angezeigt, die zuvor ausgeführt wird.
- **Nach Bereichen**: Wenn für die Vorprozesse mehrere Aggregate zur Verfügung stehen, kann die Anzeige in der Spalte kommt von zwischen Produktionsbereich und Aggregat gewechselt werden.
- **Mit Auftragspositionen**: Die Auftragspositionen werden mit angezeigt.

- [ ] Die Zusatzinformation wird nicht angezeigt.
- [ ] Die Zusatzinformation wird in der Übersicht in einer weiteren Spalte ausgegeben. Die Wahl muss im Menü Start > Ausführen bestätigt werden, um die Anzeige zu aktualisieren.

### Übersicht (Teile / Vorprozesse)

In der Übersicht werden standardmäßig folgende Spalten angezeigt:

- **Arbeitsart**: Bezeichnung der Arbeitsart im Produktionsbereich.
- **Auftrag**: Die Auftragsnummer wird angezeigt, wenn Sie auf den Zeilenkopf klicken. Keine Test-Daten, so bekomme ich diese Spalte nicht angezeigt.
- **Kunde**: Der Kundenname wird angezeigt, wenn Sie im Modus Teile auf den Zeilenkopf klicken. Keine Test-Daten, so bekomme ich diese Spalte nicht angezeigt.
- **Anzahl**: Anzahl der Scheiben in der Schicht.
- **qm**: Gesamtfläche in der Schicht.
- **Teil**: Produktbezeichnung (Modus Teile).
- **Artikel-Nr.**: Produktnummer (Modus Teile).
- **kommt von**: Vorheriger Produktionsbereich (Modus Vorprozesse).

---

## Leitstand – Bestellteile

**Fertigung > Kapazitätsplanung > Leitstand > Register Bestellteile**

*Abb. H-219 Leitstand - Bestellteile*

In diesem Register prüfen Sie, welche Bestellungen (Zukaufartikel) in den Positionen enthalten sind.

### Übersicht

In der Übersicht werden folgende Daten angezeigt:

- **Auftrag, Position**: Auftrags- und Positionsnummer aus dem Auftrag.
- **Teil**: Nummer der Stücklistenebene.
- **(Leere Spalte)**: Serien, zurzeit nicht genutzt.
- **Artikel/Bearbeitung**: Produktbezeichnung des Zukaufartikels.
- **Stück**: Stückzahl, die zugekauft werden muss.
- **Abmessungen**: Maße der Position.
- **Bestellt zum**: Gewünschter Liefertermin durch den Lieferanten.
- **Gel.**: Gelieferte Stückzahl.
- **Schicht**: Schicht, in der die Zukaufartikel benötigt werden.

---

## Leitstand (Aggregat)

**Fertigung > Kapazitätsplanung > Leitstand > Register Aggregate > Doppelklick auf Zeilenkopf**

In diesem Dialog prüfen Sie die Auslastung der Maschinen pro Schicht.

Im Dialog Leitstand (Aggregat) finden Sie folgende Register:

- "Leitstand (Aggregat) – Verschieben I” auf Seite H-362
- "Leitstand (Aggregat) - Belegung" auf Seite H-364
- "Leitstand (Aggregat) – Verschieben II" auf Seite H-366
- Tutorial, "Leitstand - Aggregat" auf Seite H-176

### Menü Funktionen

**Fertigung > Kapazitätsplanung > Leitstand > Register Aggregate > Doppelklick auf Zeilenkopf > Leitstand (Aggregat) > Menü Funktionen**

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Leitstand zu schließen.

Das Menü ist in folgende Gruppen gegliedert:

- "Gruppe Schicht füllen" auf Seite H-360
- "Gruppe Komprimieren" auf Seite H-360
- "Gruppe Grafik" auf Seite H-361

### Gruppe Schicht füllen

- **Rückwärts**: Überrechnet die Schichten. Die Stückzahlen werden in eine vorige Schicht verschoben, wenn dies möglich ist.
- **Vorwärts**: Überrechnet die Schichten. Die Stückzahlen werden in eine nächste Schicht verschoben, wenn dies möglich ist.

### Gruppe Komprimieren

Sie können Lücken füllen, die durch die Voreinstellungen zur prozentualen Auslastung beim Splitten einer Position entstanden sind, oder wenn z. B. ein Auftrag storniert wurde und dadurch Kapazitäten frei geworden sind.

- **Rückwärts**: Überrechnet die Auslastung von angezeigten Datum aus zurück.
- **Vorwärts**: Überrechnet die Auslastung von angezeigten Datum aus in die Zukunft.
⇨ "Schichtfüllung bei Positionssplit" auf Seite H-190
⇨ "Positions-Split" auf Seite H-300

### Gruppe Grafik

- **Produktionsbereich**: Öffnet eine grafische Tagesübersicht zum Produktionsbereich.
- "Grafik" auf Seite H-311

### Menü Optionen

**Fertigung > Kapazitätsplanung > Leitstand > Register Aggregate > Doppelklick auf Zeilenkopf > Leitstand (Aggregat) > Menü Optionen**

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

Die Beschreibung der folgenden Einträge gibt den aktivierten Zustand wieder:

- **Rüstzeit verschieben**: Schaltet die Möglichkeit zum Verschieben die Rüstzeiten frei.
- **Meldungen unterdrücken**: Fehler, die beim Umlasten auf einen anderen Termin oder ein anderes Aggregat auftreten, werden in einer Meldung angezeigt. Diese Meldungen können Sie unterdrücken.

---

## Leitstand (Aggregat) – Verschieben I

**Fertigung > Kapazitätsplanung > Leitstand > Register Aggregate > Doppelklick auf Zeilenkopf > Leitstand (Aggregat) > Register Verschieben I**

*Abb. H-220 Leitstand (Aggregat) - Verschieben I*

In diesem Register prüfen Sie, welche Aufträge und Stückzahlen pro Schicht im aktuellen Aggregat gefertigt werden müssen.

### Navigation durch die Register

| Aktion | Dialog |
| :--- | :--- |
| Doppelklick auf Auftragsnummer | -> Leitstand (Auftrag) |

---

## Übersicht

In der Übersicht werden die Stückzahlen für das gewählte Aggregat angezeigt:

- **Datum**: Produktionsdatum.
- **Schicht**: Schicht, in der die Aufträge gefertigt werden.
- **Auftrag**: Auftragsnummer.
- **Stück**: Stückzahl des Auftrags am aktuellen Aggregat.
- **Fertig**: Anzahl der gefertigten Gläser.
- **Verschieben**:
- **Stunden**:

### Verschieben

- **Neuer Termin**: Fertigungstermin, an den der Auftrag verschoben werden soll.
- **Schicht**: Schicht, in die der Auftrag verschoben werden soll.
- **Aggregat**: Maschine, an die der Auftrag verschoben werden soll.
- **[Belegung]**: Prüft die Auslastung der alternativen Maschine. Der Wert wird in Stunden angezeigt. Er schließt die Zeiten des Auftrags mit ein, den Sie durch einen Klick in den Zeilenkopf markiert haben.
- **[Rückgängig]**: Setzt die Verschiebung zurück auf die ursprünglichen Werte.

---

## Leitstand (Aggregat) – Belegung

**Fertigung > Kapazitätsplanung > Leitstand > Register Aggregate > Doppelklick auf Zeilenkopf > Leitstand (Aggregat) > Register Belegung**

*Abb. H-221 Leitstand (Aggregat) – Belegung*

In diesem Register werden alle Positionen angezeigt, die in dem gewählten Zeitraum gefertigt werden müssen.
⇨Tutorial, "Leitstand - Aggregat" auf Seite H-176

### Auswahl

- **Datum von, bis**: Eingabe des Zeitraums, dessen Belegung Sie prüfen wollen.
- **Aggregat**: Auswahl des Aggregats, zu dem Sie die Auslastung prüfen wollen.

---

## Übersicht

In der Übersicht werden alle Auftragspositionen aufgelistet, die im gewählten Zeitraum gefertigt werden müssen.

- **Datum**: Produktionsdatum.
- **Schicht**: Schicht, in der die Position gefertigt wird.
- **Auftrag, Pos**: Auftrags- und Positionsnummer aus dem Auftrag.
- **Produkt**: Produktbezeichnung.
- **Glasmaß**: Maße der Position.
- **Teil**: Produktname der Stücklisten-Komponente.
- **Arbeitsart**: Arbeitsart im Produktionsbereich.
- **Stück**: Stückzahl der Position.
- **Zeit**: Geplante Zeit.
- **Kunde**: Kundenname aus dem Auftrag.

---

## Leitstand (Aggregat) – Verschieben II

**Fertigung > Kapazitätsplanung > Leitstand > Register Aggregate > Doppelklick auf Zeilenkopf > > Leitstand (Aggregat) > Register Verschieben II**

*Abb. H-222 Leitstand (Aggregat) – Verschieben II*

In diesem Register werden alle Sichten im gewählten Zeitraum angezeigt. Eine Zelle ist farbig hinterlegt, wenn bei der Einlastung ein Problem besteht.

### [Übersicht]

In der Übersicht werden alle Schichten für den gewählten Zeitraum aufgelistet.

- **Datum**: Produktionsdatum.
- **Schicht**: Schicht, in der die Stückzahlen gefertigt werden.
- **Stück**: Stückzahl der Position.
- **Stunden**: Benötigte Zeit. Wenn Probleme beim Einlasten entstanden sind, wird das Feld rot eingefärbt.

---

### Verschieben

Die Felder in diesem Bereich sind zum Register Verschieben I erklärt.
⇨ "Leitstand (Aggregat) - Verschieben I" auf Seite H-362

## Auslastung zu Datum

**Fertigung > Kapazitätsplanung > Leitstand > Register Aggregate > Menü Funktionen > Gruppe Anzeige > Auslastung**

In diesem Dialog lassen Sie sich eine Übersicht über die zu produzierenden Mengen für einen vorgegebenen Zeitraum anzeigen. Die Übersicht kann wahlweise nach Produktionsbereichen, Aggregaten oder Aggregat-Typen ausgegeben werden.

Die Daten werden angezeigt, wenn Sie die Filterung im Menü Start > Ausführen gestartet haben.

In diesem Kapitel finden Sie folgende Informationen:

- "Menü Werk" auf Seite H-368
- "Menü Anzeige" auf Seite H-368
- "Auslastung zu Datum (Anzeigezeitraum)" auf Seite H-369
- "Auslastung zu Datum – Auswahl" auf Seite H-371
- "Auslastung zu Datum – Details" auf Seite H-372
- "Auslastung - Grafik" auf Seite H-373
- "Auslastung – Druck" auf Seite H-374

---

## Menü Werk

**Fertigung > Kapazitätsplanung > Leitstand > Register Aggregate> Menü Funktionen > Gruppe Anzeige > Auslastung > Menü Werk**

Über dieses Menü legen Sie fest, ob die Kapazität eines einzelnen Werks oder die aller Werke berücksichtigt werden sollen.

- **Alle**: Alle definierten Produktionsbereiche werden angezeigt.
- **Werk 1**: Nur die Produktionsbereiche mit Eintrag 0 und 1 werden angezeigt.
- **Werk 2**: Nur die Produktionsbereiche mit Eintrag 0 und 2 werden angezeigt.
- **Werk 3**: Nur die Produktionsbereiche mit Eintrag 0 und 3 werden angezeigt.

Das Werk bezieht sich auf den Schlüssel, der Firmendaten für einen Mandanten eingetragen ist.

Die Mandanten werden dann im Dialog Produktionsbereiche zugeordnet.

## Menü Anzeige

**Fertigung > Kapazitätsplanung > Leitstand > Register Aggregate > Menü Funktionen > Gruppe Anzeige > Auslastung > Menü Anzeige**

- **Anzeige Status**: Über dieses Menü können Sie den Auftragsstatus festlegen, bis zu dem Aufträge angezeigt werden sollen.
⇨ "Anzeigestatus" auf Seite H-375

---

## Auslastung zu Datum (Anzeigezeitraum)

**Fertigung > Kapazitätsplanung > Leitstand > Register Aggregate > Menü Funktionen > Gruppe Anzeige > Auslastung**

*Abb. H-223 Auslastung zu Datum – Zeitraum auswählen*

In diesem Dialog prüfen Sie die Kriterien für die Anzeige der Auslastung fest. Das Ergebnis können Sie sich als Grafik oder als Liste anzeigen lassen.

⇨ "Auslastung - Grafik" auf Seite H-373
⇨ "Auslastung - Druck" auf Seite H-374

### Auswertungszeitraum

**Von, bis** Zeitraum, für den Sie eine Übersicht erhalten möchten.

### Optionen

**Umsatz anzeigen** Diese Checkbox ist nur freigeschaltet, wenn Sie im Bereich Übersicht über die Option Aggregat gewählt haben.

- Der Umsatz wird nicht angezeigt.
- Der Umsatz für das gewählte Aggregat wird angezeigt.

---

### Übersicht über

Mit der Wahl der Optionen filtern Sie die Anzeige.

- **Produktionsbereich**: Sie können die Übersicht auf einen bestimmten Produktionsbereich einschränken (<k.A.> = alle).
- **Aggregattypen**: Sie können die Übersicht auf einen bestimmten Aggregattyp einschränken.
- **Aggregat**: Sie können die Übersicht auf ein bestimmtes Aggregat einschränken. Bei dieser Option können Sie die Checkbox Umsatz anzeigen aktivieren.
- **Alle Aggregate nach Produktionsbereich**: Mit dieser Option werden alle Aggregate sortiert nach Produktionsbereichen angezeigt.

### Übersicht

In der Übersicht werden folgende Daten angezeigt:

- **Datum, Produktionsbereiche/Aggregate**: Die Auslastung wird pro Datum und Produktionsbereich oder Aggregat angezeigt.
- **Stück**: Gesamtstückzahl.
- **Fläche**: Gesamtfläche.
- **Umfang**: Gesamte Kantenlänge.
- **Zeit**: Verplante Zeit.
- **Kosten**: Zeitkosten.
- **Umsatz**: Umsatz pro Aggregat. Diese Spalte wird nur angezeigt, wenn Sie die Option Aggregat gewählt und die Checkbox Umsatz anzeigen markiert haben.

---

## Auslastung zu Datum – Auswahl

**Fertigung > Kapazitätsplanung > Leitstand > Register Aggregate > Menü Funktionen > Gruppe Anzeige > Auslastung > Auswertungszeitraum anzeigen > Klick in Zeilenkopf > Register Auswahl**

*Abb. H-224 Auslastung zu Datum – Produktionsbereich/Aggregat auswählen*

In diesem Dialog prüfen Sie die Auslastung in einem bestimmten Zeitraum.

### Auswertung - Datum

- **Von, bis**: Zeitraum, für den Sie eine Übersicht erhalten möchten.
- **Nur Schicht**: Angabe der Schicht, deren Auslastung angezeigt werden soll. Das Feld ist nur im Auswahl-Modus freigeschaltet.
- **Schichten-Info**: Die Checkbox ist nur im Auswahl-Modus freigeschaltet.
  - Die Auswahl soll nicht auf eine bestimmte Schichten eingegrenzt werden. Nach dem Filtern werden in der Übersicht alle Schichten angezeigt.
  - Die Auswahl soll auf die Schicht eingegrenzt werden, die im Feld Nur Schicht angegeben ist.

### Übersicht

Mit der Wahl der Option legen Sie die Filterung der Anzeige fest:

- **Alle Produktionsbereiche**: Die Auslastung aller Produktionsbereiche im eingestellten Zeitraum wird angezeigt.
- **Alle Aggregate**: Die Auslastung aller Aggregate im eingestellten Zeitraum wird angezeigt.
- **Nur zu Produktionsbereich**: Die Auslastung zu einem bestimmten Produktionsbereich wird angezeigt. Das Feld für die Auswahl des Produktionsbereichs wird freigeschaltet.

**Gruppierung Detailübersicht** Mit der Wahl der Option legen Sie die Gruppierung im Register Details fest. Die Felder sind nur freigeschaltet, wenn Daten angezeigt werden.
- **Auftrag, Kunde**: Die Auslastung wird pro Auftrag und Kunde angezeigt.
- **Produkt**: Die Auslastung wird pro Produkt angezeigt.

### Auslastung

In der Übersicht wird die Trefferliste angezeigt.

---

## Auslastung zu Datum – Details

**Fertigung > Kapazitätsplanung > Leitstand > Register Aggregate > Menü Funktionen > Gruppe Anzeige > Auslastung > Auswertungszeitraum anzeigen > Klick in Zeilenkopf > Register Details**

*Abb. H-225 Auslastung zu Datum – Details zum Produktionsbereich/Aggregat*

In diesem Dialog prüfen Sie die Details der Auslastung.

### Navigation durch die Register

| Aktion | Dialog |
| :--- | :--- |
| Klick auf Zeilenkopf | -> Fertigungsstand Auftrag |

---

### Details

Die Anzeige der Spalten und Daten richtet sich nach den Auswahlkriterien. Die Listen sind nach der Option gruppiert, die im Register Auswahl markiert ist.

**Produktionsbereich** Anzeige des Produktionsbereichs, in dem die Maschinen stehen oder die Arbeiten ausgeführt werden.

**Nummernverwalter** Auswahl des Nummernverwalters, in den die angezeigten Aufträge gestellt werden sollen.

**[NV füllen]** Stellt alle angezeigten Aufträge in den angegebenen Nummernverwalter.

## Auslastung – Grafik

**Fertigung > Kapazitätsplanung > Leitstand > Register Aggregate > Menü Funktionen > Gruppe Anzeige > Auslastung > Auswertungszeitraum anzeigen > Klick in Zeilenkopf > Auslastung zu Datum – Auswahl > Menü Funktionen > Gruppe Auslastung > Grafik anzeigen**

*Abb. H-226 Auslastung zu Datum – Grafik*

Die grafische Darstellung zeigt die Auslastung je nach den Auswahlkriterien im Dialog Auslastung zu Datum.

---

## Auslastung – Druck

**Fertigung > Kapazitätsplanung > Leitstand > Register Aggregate > Menü Funktionen > Gruppe Anzeige > Auslastung > Auswertungszeitraum anzeigen > Menü Druck**

Sie können das Ergebnis aus dem Dialog Auslastung zu Datum ausdrucken. Bei der Wahl zum Druck können Sie den dargestellten Zeitraum auf 8 oder 12 Tage einschränken.
⇨ "Auslastung - Druck" auf Seite H-374

*Abb. H-227 Druck*

Sie können das Ergebnis aus dem Dialog Auslastung zu Datum ausdrucken. Bei der Wahl zum Druck können Sie den dargestellten Zeitraum auf 8 oder 12 Tage einschränken. Achten Sie bei 12 Tagen darauf, in Ihren Druckeinstellungen das Querformat zu wählen.

Dargestellt ist eine Tagesübersicht über die zu produzierenden Einheiten pro Maschine und Produktionsbereich. Zusätzlich wird der Soll-Wert angegeben.

---

## Anzeigestatus

**Fertigung > Kapazitätsplanung > Leitstand > Register Aggregate > Menü Funktionen > Gruppe Anzeige > Auslastung > Menü Anzeige > Gruppe Optionen > Anzeige Status**

*Abb. H-228 Anzeigestatus festlegen*

In diesem Dialog schränken Sie die Anzeige der Aufträge auf einen Höchststatus ein. Angezeigt werden nur die Aufträge, deren Status kleiner als der eingetragenen Status ist.

## Einstellungen zum Leitstand

**Fertigung > Kapazitätsplanung > Leitstand > Menü Funktionen > Einstellungen**

*Abb. H-229 Einstellungen zum Dialog Leitstand*

In diesem Dialog legen Sie fest, welche Daten im Dialog Leitstand angezeigt werden sollen.

Die geänderten Einstellungen müssen Sie mit [OK] bestätigen. Der Dialog Leitstand muss neu geöffnet werden, damit die Daten neu eingelesen werden.

---

### Nur diese Produktionsbereiche

Sie können die Anzeige auf einen bestimmten Produktionsbereich oder mehrere Produktionsbereiche einschränken. Wenn Sie keinen Eintrag markiert haben, werden alle Produktionsbereiche angezeigt.

### Auswahlkriterien

**Nur die noch nicht fertig gemeldeten Einträge anzeigen** Sie können einstellen, dass nur die nicht gefertigten Positionen angezeigt werden.

- Mit dieser Einstellung werden gefertigte und noch nicht gefertigte Positionen angezeigt.
- Mit dieser Einstellung werden nur die Positionen angezeigt, die noch gefertigt werden müssen.

**AV-Bereich** Sie können die Anzeige auf einen bestimmten AV-Bereich einschränken. Die Kombobox zur Wahl des AV-Bereichs wird freigeschaltet.

**Von Status, Bis Status** Sie können die Anzeige nach Auftragsstatus einschränken. Wenn Sie in beiden Feldern denselben Status auswählen, werden nur Aufträge mit diesem einen Status angezeigt.

### Neben den Zeiten noch anzeigen

Standardmäßig werden nur die am Tag verfügbaren Stunden pro Maschine angezeigt. Sie können diese Angaben um folgende Details erweitern:

- **Stück**: Stückzahlen aller Schichten und Aufträge.
- **qm**: Gesamtfläche aller Schichten und Aufträge.
- **Lfm**: Gesamtkantenlänge aller Schichten und Aufträge.
- **in %**: prozentuale Auslastung aller Schichten.
  - Die Information wird nicht angezeigt.
  - Die Information wird in den Registern Aggregate und Aufträge angezeigt.

---

## Restmengen anzeigen

**Fertigung > Kapazitätsplanung > Leitstand > Menü Funktionen > Restmengen anzeigen**

*Abb. H-230 Restmengen anzeigen und fertig melden*

In diesem Dialog prüfen Sie, welche Aufträge noch nicht fertig gemeldet sind und holen dies ggf. nach.

**Anzeige ab Status** Sie können die Anzeige der offenen Aufträge auf einen Mindeststatus einschränken, damit z. B. keine Aufträge angezeigt werden, die schon begonnen wurden.

### Übersicht

In der Übersicht werden alle Aufträge angezeigt, die bis zum aktuellen Datum nicht gefertigt wurden. Wenn Sie die Checkbox markieren, wird der entsprechende Auftrag zum aktuellen Datum fertig gemeldet, sobald Sie mit [OK] bestätigt haben.

---

## Leitstand (Auftrag)

**Fertigung > Kapazitätsplanung > Leitstand > Menü Funktionen > Auftrag auswählen**

In diesem Dialog prüfen Sie die einzelnen Aggregate, die ein Auftrag bei der Produktion bis zum Versand durchläuft, um die Einlastung an den "kritischen" Aggregaten zu verschieben.

Im Dialog **Leitstand - Auftrag** finden Sie folgende Register:

- "Leitstand (Auftrag) – Aggregate" auf Seite H-381
- "Leitstand (Auftrag) – Detail" auf Seite H-383
- "Leitstand (Auftrag) – Arbeitsarten" auf Seite H-385
- "Leitstand (Auftrag) – Bestellteile" auf Seite H-387
- "Leitstand (Auftrag) – Verschieben I" auf Seite H-388
- "Leitstand (Auftrag) – Verschieben II" auf Seite H-389
- "Leitstand (Auftrag) – Belegung" auf Seite H-391
- Tutorial, "Leitstand - Auftrag" auf Seite H-175

### Navigation durch die Register und Dialoge

Die folgende Übersicht zeigt Ihnen, wie Sie sich die Daten anzeigen lassen.

| Register | Aktion | Register / Dialog |
| :--- | :--- | :--- |
| Aggregate | Doppelklick auf Aggregat | -> Verschieben II |
| | Doppelklick auf Datum | Detail |
| Detail | Klick auf Zellenkopf | -> Arbeitsarten |

### Menü Funktionen

**Fertigung > Kapazitätsplanung > Leitstand > Menü Funktionen > Auftrag auswählen > Menü Funktionen**

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Leitstand zu schließen.

Das Menü ist in folgende Gruppen gegliedert:

- "Gruppe Dokument" auf Seite H-378
- "Gruppe Grafik" auf Seite H-379
- "Gruppe Produktion" auf Seite H-379

#### Gruppe Dokument

- **Dokument anzeigen**: Öffnet die Ansicht des Dokuments.
- **Historie**: Öffnet den Dialog Historie, in dem Sie den Verlauf der Statusumsetzungen prüfen können.
  - Verkauf, "Historie" auf Seite C-564
- **Statusänderung**: Öffnet den gleichnamigen Dialog, in dem Sie den Status des Auftrags umsetzen können.
  - Verkauf, "Statusänderung" auf Seite C-566

#### Gruppe Grafik

- **Produktionsbereich**: Öffnet die grafische Darstellung Produktionsbereiche / Wochenübersicht zum Vergleich der fertigen und offenen Mengen.
- **Auftrag**: Öffnet die grafische Darstellung Auftragsinfo / Wochenübersicht zum Vergleich der fertigen und offenen Mengen.

Diese Grafiken entsprechen der Darstellung Grafik-Bereiche.
- "Grafik-Bereiche" auf Seite H-272

#### Gruppe Produktion

- **Übersicht Rückmeldungen**: Öffnet den Dialog Übersicht Rückmeldungen, um den aktuellen Stand der Produktion pro Auftragsposition zu prüfen.
  - "Übersicht Rückmeldungen" auf Seite H-334
- **Einlasten**: Öffnet den Dialog Einlasten Auftrag, um die Einlastung des aktuellen Auftrags zu ändern.
  - "Einlasten Auftrag" auf Seite H-289
- **Manuelle Vorgabe**: Öffnet den Dialog Fertigungsstand Auftrag, in dem Sie den Fertigungsstand des Auftrags prüfen können.
  - “Fertigungsstand Auftrag" auf Seite H-323

### Menü Optionen

**Fertigung > Kapazitätsplanung > Leitstand > Menü Funktionen > Auftrag auswählen > Menü Optionen**

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

Die Beschreibung der folgenden Einträge gibt den aktivierten Zustand wieder:

- **Verweilzeit prüfen**: Vor dem Verschieben wird geprüft, ob die Übergangszeiten eine Verschiebung zulassen. Diese Einstellung sollten Sie übernehmen, wenn Sie wissen, dass der Übergang längere Übergangszeiten benötigt, z. B. bei der ESG-Produktion. Diese Prüfung sollten Sie nur dann unterdrücken, wenn der Übergang von einem Produktionsbereich in den nächsten keine längeren Übergangszeiten erfordert.
- **Verweiltage ignorieren**: Ignoriert die Verweiltag beim Umlasten.
- **Rüstzeit verschieben**: Wenn diese Option aktiviert ist, werden die Schaltflächen im Register Verschieben II gesperrt.

---

#### Rüstzeitkontrolle:

Wenn die Rüstzeit zu mehreren Arbeitsarten eingerichtet ist, die für eine Auftragsposition ausgeführt werden, dann soll diese Zeit nur einmal pro Position berechnet werden.

#### Meldungen unterdrücken:

Fehler, die beim Umlasten auf einen anderen Termin oder ein anderes Aggregat auftreten, werden in einer Meldung angezeigt. Diese Meldungen können Sie unterdrücken.

## Leitstand (Auftrag) – Aggregate

**Fertigung > Kapazitätsplanung > Leitstand > Menü Funktionen > Auftrag auswählen > Register Aggregate**

*Abb. H-231 Leitstand (Auftrag) - Aggregate*

In diesem Register prüfen Sie, wie die Maschinen ausgelastet sind, an denen der Auftrag gefertigt werden muss. Wenn Sie den Dialog aus dem Leitstand heraus geöffnet haben, werden die Daten des aktuellen Auftrags angezeigt. Sie können jedoch über den Suchmodus einen anderen Auftrag anzeigen lassen oder die Anzeige auf eine bestimmte Position einschränken.

Wenn der Auftrag manuell komplett fertig gemeldet wurde, werden alle bis dahin noch nicht gemeldeten Werte auf den Tag verschoben, an dem fertig gemeldet wurde. Die Werte sind dann in grüner Schrift angezeigt.

---

### Auftrag

- **Nummer, Kunde**: Nummer und Kundenname aus dem Auftrag.
- **Nur Position**: Nummer der Position, die geändert werden soll. Das Feld ist im Auswahlmodus freigeschaltet. Sie können dann die Positionsnummer angeben, wenn Sie nur eine Auftragsposition anzeigen lassen wollen. Wenn Sie eine Null (0) eintragen, werden alle Positionen angezeigt.
- **Liefertermin**: Liefertermin aus dem Auftrag. Sie können den Termin ändern und mit [Ändern] bestätigen.
  - Tutorial, “Einlastung für einzelnen Auftrag verschieben" auf Seite H-177
- **[Ändern]**: Bestätigt den neuen Termin.
- **AV-Bereich**: AV-Bereich, aus dem der Auftrag stammt.
- **Produktion von - bis**: Anzeige des Zeitraums, in dem der Auftrag produziert wird.

### Übersicht

- **Aggregat**: Aggregate, an denen der Auftrag produziert wird.
- **Wochentag, Datum**: Pro Wochentag wird die Auslastung mit der verplanten und der verplanbaren Zeit (alle Schichten) pro Maschine angezeigt.
  - Verplante und verplanbare Zeit (alle Schichten).
  - Offene und gefertigte Anzahl aller Scheiben in Stk.
  - Gesamt Fläche in qm.
  - Kantenlänge aller Scheiben.
  - Auslastung in Prozent.
- Alle Angaben außer der Zeit können in den Einstellungen zum Leitstand zu- oder abgewählt werden.
  - "Einstellungen zum Leitstand" auf Seite H-375

---

## Leitstand (Auftrag) – Detail

**Fertigung > Kapazitätsplanung > Leitstand > Menü Funktionen > Auftrag auswählen > Register Detail**

*Abb. H-232 Leitstand (Auftrag) – Detail*

In diesem Register können Sie Stückzahlen manuell verschieben oder fertig melden. Über den Feldern wird das Aggregat angezeigt, zu dem die Daten abgefragt wurden.

Wenn Sie eine Position insgesamt verschoben haben, wird sie aus der Anzeige gelöscht.

### Übersicht

In der Übersicht werden die Stückzahlen des aktuellen Auftrags für das gewählte Aggregat angezeigt. Folgende Spalten werden angezeigt:

- **Schicht**: Aktuelle Schicht.
- **Stück**: Stückzahl des Auftrags am aktuellen Aggregat.
- **Fertig**: Anzahl der gefertigten Gläser.
- **Verschieben**: Nur wenn Sie die Checkbox markiert haben, werden die Änderungen übernommen. Sind die Änderungen mit anderen Arbeitsgängen für diesen Auftrag unvereinbar, wird in einer Fehlermeldung angezeigt, dass ein Verschieben unmöglich ist.
- **Stunden**: Für die angezeigte Stückzahl verplante Zeit.

**[Belegung / Tag]** Aktualisiert die Anzeige im nachfolgenden Feld.

### Verschieben

- **Neuer Termin**: Fertigungstermin, an den der Auftrag verschoben werden soll.
- **Schicht**: Schicht, in die der Auftrag verschoben werden soll.
- **Aggregat**: Maschine, an die der Auftrag verschoben werden soll. Das Feld wird freigeschaltet, wenn Sie die Checkbox verschieben markiert und mit [OK] bestätigt haben.
- **[Belegung]**: Prüft die Auslastung der alternativen Maschine. Der Wert wird in Stunden angezeigt. Er schließt die Zeiten des Auftrags mit ein.
- **[Rückgängig]**: Setzt die Verschiebung zurück auf die ursprünglichen Werte.

---

## Leitstand (Auftrag) – Arbeitsarten

**Fertigung > Kapazitätsplanung > Leitstand > Menü Funktionen > Auftrag auswählen > Register Arbeitsarten**

*Abb. H-233 Leitstand (Auftrag) – Arbeitsarten*

In diesem Register prüfen Sie, welche Arbeitsarten an einem Produktionstermin auf einer Maschine durchgeführt werden sollen.

Wenn Sie eine Position insgesamt auf ein anderes Datum verschoben haben, wird sie aus der Anzeige gelöscht.

**[Alle], [Keine]** Markiert alle Checkboxen in der Spalte verschieben oder entfernt die Markierungen.

> **Rüstzeiten bearbeiten**
> Über das Kontextmenü (rechte Maustaste) auf eine Position können Sie Rüstzeiten hinzufügen oder löschen. Dazu muss die Rüstzeit als Arbeitsart mit einer Basiszeit angelegt sein.

---

## Übersicht

In der Übersicht werden folgende Daten angezeigt:

- **Schicht**: Schicht, in der die Position gefertigt werden soll.
- **Pos.**: Positionsnummer aus dem Auftrag.
- **SL-ID**: Stücklisten-Identnummer, das ist die Stücklistenebene.
- **UP**: Unterpositionen (Pakete), die beim Einlasten durch Splitten der Position entstanden sind.
- **Vorgang**: Arbeitsart.
- **Produkt/Bearb.**: Produktbezeichnung.
- **Stück**: Positionsmenge.
- **Fertig**: Anzahl der gefertigten Scheiben.
- **Abmessungen**: Maße der Position.
- **Verschieben**: Nur wenn Sie die Checkbox markiert haben, werden die Änderungen übernommen. Sind die Änderungen mit anderen Arbeitsgängen für diesen Auftrag unvereinbar, wird in einer Fehlermeldung angezeigt, dass ein Verschieben unmöglich ist.
  > Diese Meldung kann über das Menü Optionen ausgeschaltet sein!
- **Stunden**: Für diese Position reservierte Zeit.

### Einlastung ändern

Die Felder im Bereich Verschieben sind zum Register Detail erklärt.

⇨ "Leitstand (Auftrag) - Detail" auf Seite H-383

---

## Leitstand (Auftrag) – Bestellteile

**Fertigung > Kapazitätsplanung > Leitstand > Menü Funktionen > Auftrag auswählen > Register Bestellteile**

*Abb. H-234 Leitstand (Auftrag) – Bestellteile*

In diesem Register prüfen Sie, welche Bestellungen für die Produktion benötigt werden.

### Übersicht

In der Übersicht werden folgende Daten angezeigt:

- **Position**: Positionsnummer aus dem Auftrag.
- **Artikel**: Produktbezeichnung des Bestellteils.
- **Stück**: Stückzahl, die zugekauft werden muss.
- **Abmessungen**: Maße der Position.
- **Bestellt zum**: Gewünschter Liefertermin durch den Lieferanten.
- **Gel.**: Gelieferte Stückzahl.
- **Wird benötigt an, Datum, Schicht**: In diesen drei Spalten wird angezeigt, wann die Bestellteile wo benötigt werden.

---

## Leitstand (Auftrag) – Verschieben I

**Fertigung > Kapazitätsplanung > Leitstand > Menü Funktionen > Auftrag auswählen > Register Verschieben I**

*Abb. H-235 Leitstand (Auftrag) – Verschieben II*

In diesem Register planen und bearbeiten Sie die Belegung der Maschinen mit Serien. Diese Funktion wird zurzeit nicht genutzt.

### Auftrag

In diesem Bereich werden die Auftragsnummer und der Name des Kunden angezeigt.

### Verschieben um volle Tage

**Anzahl Tage** Anzahl der Tage, um die die Produktion der Serie verschoben werden soll.

**Nur von Datum** Ausgangsdatum, vom der aus die oben angegebenen vollen Tage gezählt werden sollen.

---

## Leitstand (Auftrag) – Verschieben II

**Fertigung > Kapazitätsplanung > Leitstand > Menü Funktionen > Auftrag auswählen > Register Verschieben II**

*Abb. H-236 Leitstand Auftrag - Verschieben II*

In diesem Register verschieben Sie die Positionen oder Aufträge auf andere Termine, Schichten oder Maschinen.

Wenn Sie eine Position insgesamt verschoben haben, wird sie aus der Anzeige gelöscht.

### Übersicht

In der Übersicht werden die Stückzahlen des aktuellen Auftrags für das gewählte Aggregat angezeigt. Folgende Spalten werden angezeigt:

- **Datum**: Geplantes Produktionsdatum.
- **Schicht**: Aktuelle Schicht.
- **Stück**: Stückzahl des Auftrags am aktuellen Aggregat.
- **Fertig**: Anzahl der gefertigten Gläser.
- **Verschieben**: Nur wenn Sie die Checkbox markiert haben, werden die Änderungen übernommen. Sind die Änderungen mit anderen Arbeitsgängen für diesen Auftrag unvereinbar, wird in einer Fehlermeldung angezeigt, dass ein Verschieben unmöglich ist.
- **Stunden**: Für die angezeigte Stückzahl verplante Zeit.

> **Bereiche gesperrt**
> Die Bereiche Schicht füllen und Komprimieren können über das Menü Optionen > Rüstzeit verschieben gesperrt werden.

### Schicht füllen

Sie können die Schichtzeiten überrechnen lassen, um Lücken in einer Schicht mit den passenden Stückzahlen der vorigen oder folgenden Schicht aufzufüllen.

- **[Rückwärts]** Überrechnet die Schichten. Die Stückzahlen werden in eine vorige Schicht verschoben, wenn dies möglich ist.
- **[Vorwärts]** Überrechnet die Schichten. Die Stückzahlen werden in die nächste Schicht verschoben, wenn dies möglich ist.

### Komprimieren

Sie können die Auslastung des Aggregats neu berechnen lassen. Damit können Sie Lücken füllen, die durch die Voreinstellungen zur prozentualen Auslastung beim Splitten einer Position entstanden sind, oder wenn z. B. ein Auftrag storniert wurde und dadurch Kapazitäten frei geworden sind.

- "Schichtfüllung bei Positionssplit" auf Seite H-190
- "Positions-Split" auf Seite H-300

- **[Rückwärts]** Überrechnet die Auslastung von angezeigten Datum aus zurück.
- **[Vorwärts]** Überrechnet die Auslastung von angezeigten Datum aus in die Zukunft.

### Verschieben

Die Felder im Bereich Verschieben sind zum Register Detail erklärt.
⇨ "Leitstand (Auftrag) - Detail" auf Seite H-383

---

## Leitstand (Auftrag) – Belegung

**Fertigung > Kapazitätsplanung > Leitstand > Menü Funktionen > Auftrag auswählen > Register Belegung**

*Abb. H-237 Leitstand (Auftrag) – Belegung*

In diesem Register prüfen Sie, welche Auftragspositionen neben den aktuellen an der jeweiligen Maschine gefertigt werden sollen. Grün hinterlegt sind die Auftragspositionen, zu denen Sie die Anzeige gestartet haben.

### Auswahl

- **Datum von, bis**: Zeitraum, den Sie prüfen wollen.
- **Aggregat**: Aggregat, zu dem Sie die eingelasteten Aufträge prüfen wollen.

### Übersicht

In der Übersicht werden alle Auftragspositionen aufgelistet, die im gewählten Zeitraum gefertigt werden müssen.

- **Datum**: Produktionsdatum.
- **Schicht**: Schicht, in der die Position gefertigt wird.
- **Auftrag, Pos**: Auftrags- und Positionsnummer.
- **Produkt**: Produktbezeichnung.
- **Glasmaß**: Maße der Position.
- **Teil**: Produktname der Stücklisten-Komponente.
- **Arbeitsart**: Arbeitsart im Produktionsbereich.
- **Stück**: Stückzahl der Position.
- **Zeit**: Geplante Zeit.
- **Kunde**: Kundenname aus dem Auftrag.

---

## Verschieben nicht möglich

**Fertigung > Kapazitätsplanung > Leitstand > Verschieben**

*Abb. H-238 Verschieben nicht möglich*

In diesem Dialog prüfen Sie, warum die beabsichtigte Verschiebung eines Auftrags nicht möglich ist. Sie können die Anzeige dieser Meldung unterdrücken.

---
---

# A+W Produktionsmanager

## Tutorial

### Überblick

Das Tutorial zum Modul Produktionsmanager beschäftigt sich mit den Grundlagen der Produktionslösung in A+W Business Pro. Das Tutorial baut auf den Kenntnissen zu den Stammdaten und zum Nummernverwalter auf.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

#### Themenblöcke

- Standardmodus
- Expertenmodus

#### Vorausgesetzte Kenntnisse

Das Tutorial richtet sich an Teilnehmer, die in A+W Business Pro Aufträge zur Produktion vorbereiten. Die Teilnehmer müssen das Konzept der Stammdaten und des Nummernverwalters kennen.

---

### Dokumentation

Für das Modul Production Manager stehen folgende Dokumente zur Verfügung:

- **Handout PDF**: Ausdruck des Tutorials für die Schulung
- **Vollständige Unterlagen**:
  - Tutorial
  - Softwarereferenz
  - Index
- **Online-Hilfe <F1>**: Kontextsensitive Dialog-Hilfe der A+W Business-Softwarereferenzen und Tutorials der Basisversion

### Aufbau des Tutorials

Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

- **Überblick**: Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
  - **Lernziele**: Was soll vermittelt werden?
  - **Nutzen**: Wofür können Sie dieses Wissen einsetzen?
  - **Merksätze**: Welche Zusammenhänge müssen Sie sich merken?
- **Konzepte**: Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.
- **Übungen**: Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen und Lösungsvorschlägen.
- **Querverweise**: Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf ergänzende Informationen in der Softwarereferenz und in anderen Parts hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.

> **Lesehinweis**
> Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.
> Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

---

### Darstellungskonventionen

Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

| Format | Bedeutung |
| :--- | :--- |
| *Kursiv* | sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Nummernverwalter*. |
| **Fett** | sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: Geben Sie den Wert **0** ein. |
| `>` | Mit dem sogenannten Brotkrumenpfad ist der Weg kennzeichnet, auf dem Sie einen Dialog öffnen, z. B. `Fertigung > Produktion > Produktionsübergabe`. |
| `[]` | Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit **[OK]** speichern Sie die Daten. |
| `< >` | Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit **<F1>** öffnen Sie die Online-Hilfe. |

---

### Grundgedanken zum Produktionsmanager

Aufgabe des Produktionsmanageres ist es, Sie im Planungs- und Vorbereitungsprozess für die Produktion zu unterstützen - von der Laufbildung bis hin zum Druck von Produktionspapieren und dem Erzeugen vom Maschinencode.

Der Prozessablauf stellt sich wie folgt dar:
**Auftrags- / Teileselektion -> Laufbildung -> Abstellplatzorganisation -> Optimierung -> Freigabe**
*Abb. I-1 Standardprozess für Produktionslösung*

Die Aufträge werden automatisiert über einen vordefinierten Status oder manuell durch den Anwender für die interne Kapazitätsplanung freigegeben. In diesem Zuge wird eine Tabelle mit allen erforderlichen Daten gefüllt. Auf diese Daten greift dann der Production Manager zu.

Der Prozess wird in einem einzigen Dialog abgebildet, so dass für den Anwender ein Hin- und Herspringen nicht nötig ist.

Das Modul befindet sich im Bereich `Fertigung > Produktion`.

*Abb. I-2 Der Produktionsmanager im Menü von A+W Business*

---

### Die Oberfläche

Der Production Manager kann auf zwei unterschiedliche Weisen bedient werden:

- Standardmodus
- Expertenmodus

#### Standardmodus

In diesem Modus kann das Programm über eine vereinfachte Benutzerführung, den sogenannten Wizard bedient werden.

Mittels des Wizards ist es möglich, den Gesamtprozess (Laufbildung, Optimierungen, etc.) mit wenigen Eingaben zu durchlaufen. Es werden am Ende des Prozesses die Optimierungsergebnisse angezeigt und Sie können entscheiden, ob Sie den Lauf und Optimierungsergebnisse akzeptieren.

Den Standardmodus aktivieren Sie, indem Sie die entsprechende Symbol-Schaltfläche betätigen.
*Standardmodus*
⇨ "Standardmodus" auf Seite 1-13

#### Expertenmodus

In diesem Modus werden die einzelnen Schritte (Laufbildung, Optimierungen, etc.) vom Benutzer manuell ausgeführt. Sie können so sehr detailliert und selektiv Einfluss nehmen auf die einzelnen Prozessschritte der Laufbildung und -verarbeitung.

Den Expertenmodus aktivieren Sie, indem Sie die entsprechende Symbol-Schaltfläche betätigen.
*Expertenmodus*
⇨ "Expertenmodus" auf Seite 1-13

---

## Standardmodus

In diesem Themenblock lernen Sie, wie Sie den Umgang mit dem Production Manager im Standardmodus.

Dazu gehören folgende Lerneinheiten:

- "Standardmodus starten" auf Seite 1-16
- "Lauf bilden" auf Seite 1-17
- "Lauf feinplanen" auf Seite I-17
- "Ausgaben" auf Seite I-18
- "Ergebnisse" auf Seite I-19
- "Lagerplatten und Optimierungsparameter" auf Seite 1-21

---

### Überblick

**Lernziele**
- Standardmodus (Wizard) kennenlernen und verstehen

**Nutzen**
- Mit dem Wizard können Sie den Gesamtprozess mit nur wenigen Mausklicks durchlaufen. Das spart Zeit und minimiert das Fehlerrisiko.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| Standardmodus | Der Produktionsmanager wird immer im Standardmodus geöffnet. |
| Abstellplatzorganisation | Wird mit der Standard-Organisation aus den Stammdaten vorbelegt. Es kann eine andere gewählt werden. |
| Abstellplatztiefe | Durch die Veränderung dieses Wertes hat man Einfluss auf das Optimierungsergebnis. |
| Variante | Die durchgeführten Varianten bleiben erhalten. Sie können sich so für die beste Variante entscheiden. |

---

### Standardmodus starten

Der Produktionsmanager wird beim Starten im Standardmodus geöffnet. Aus dem Expertenmodus heraus können Sie in den Standardmodus wechseln, indem Sie die entsprechende Symbol-Schaltfläche betätigen. In diesem Modus präsentiert sich das Programm wie folgt:

*Abb. 1-3 Hauptdialog - Standardmodus*

Im Standardmodus kann das Programm über eine vereinfachte Benutzerführung (Wizard) bedient werden.

Mittels des Wizards ist es möglich, den Gesamtprozess (Laufbildung, Optimierung, etc.) mit wenigen Eingaben zu starten. Es werden am Ende des Prozesses die Optimierungsergebnisse angezeigt und Sie können entscheiden, ob Sie den Lauf und Optimierungsergebnisse so akzeptieren (speichern) oder mit anderen Einstellungen wiederholen, um ein besseres Ergebnis zu erzielen.

---

### Lauf bilden

Im ersten Schritt wählen Sie einen Nummernverwalter (NV) aus. Alle Aufträge, welche in diesem NV enthalten sind, werden in einem Lauf zusammengefasst.

Im Nummernverwalter fassen Sie diejenigen Aufträge zusammen, die später im Produktionsmanager in einem Lauf verarbeitet werden sollen.

*Abb. 1-4 Bereich Laufbildung*

Die Lauf-Nummer wird automatisch vom System vergeben und kann nicht geändert werden. Im Feld Status wird Ihnen der Status des Laufs angezeigt. Im Beispiel oben ist der Status Feingeplant, d. h. der Lauf hat die Feinplanung durchlaufen. Im Feld Beschreibung sehen Sie den Namen des Nummernverwalters, den Benutzer sowie das Datum der Laufbildung.

Der Bereich Laufinhalt wird erst nach der Laufbildung gefüllt. Sie sehen dann, wie viele ISO, VSG, ESG und bearbeitete Gläser der Lauf enthält.

### Lauf feinplanen

Im zweiten Schritt nehmen Sie die Einstellungen für die Feinplanung und Optimierung vor. D. h. Sie wählen mittels der Kombobox eine vordefinierte Abstellplatzorganisation aus. Nun können Sie noch die Tiefe des Abstellplatzes einstellen.

Die Verwaltung der Abstellplatzorganisationen und Abstellplatztiefe nehmen Sie in den Stammdaten vor (Stammdaten > Fertigung > Abstellplatzorganisation).

*Abb. 1-5 Bereich Feinplanung*

Wenn man für die Abstellpatztiefe einen Bereich einstellt (z. B. 80-120 %), dann definiert das Feld Anzahl Varianten wie viele Varianten durch das Klicken auf die Symbol-Schaltfläche [Ausführen] entstehen. Beispiel:

- Abstellplatztiefe: 80 - 120%
- Anzahl Varianten: 5
- Feinplanung mit 80, 90, 100 110 und 120% Gestelltiefe.

### Ausgaben

Über diesen Bereich werden alle Ausgaben, unabhängig davon, ob es sich um Ausgaben auf Papier oder in Dateiform handelt, eingestellt. Die Kombobox bietet Ihnen folgende Auswahlen:

- **Keine**: Es finden keine Ausgaben statt.
- **Alle**: Es werden folgende Medien ausgegeben:
  - Produktionslisten für den Lauf
  - Etiketten für den Lauf
  - Maschinenansteuerung für den Lauf
  - Standardlisten für die Optimierung (Rahmenbieger, ISO-Linie)
  - Schneidpläne für die Optimierung
  - Zuschnittetiketten für die Optimierung
  - Maschinenansteuerung für die Optimierung (Zuschnitttisch)
- **Auswahl**: Hier können Sie manuell die unter Punkt Alle aufgelisteten Medien aktivieren.

*Abb. 1-6 Bereich Speichern*

---

### Ergebnisse

Im Bereich **Optimierungen** werden Ihnen die möglichen Optimierungen angezeigt. Die Tabelle enthält erst dann Daten, wenn der Lauf gebildet und die Feinplanung durchlaufen wurde. Sie können wählen, welchen Glasarten Sie in welcher Reihenfolge optimieren möchten oder auch einzelne Glasarten auf Handzuschnitt setzen:

*Abb. 1-7 Bereich Optimierungen*

Nachdem Sie die Symbol-Schaltfläche [Ausführen] betätigt haben, wird der vorgeschlagene Lauf erst grobgeplant und dann feingeplant. Anschließend werden nacheinander die Optimierungen der einzelnen Gläser in der angezeigten Reihenfolge durchgeführt.

Nachdem Sie alle Optimierungen durchgeführt haben, können Sie diese über die Symbol-Schaltfläche [Speichern] speichern. Die gebildeten Läufe und durchgeführten Optimierungen werden in der Datenbank gespeichert.

> **Ausgaben werden angestoßen**
> Wenn Sie die Schaltfläche [Speichern] betätigen, werden ebenfalls alle aktivierten Ausgaben mit angestoßen inkl. Übergabe der Daten an die entsprechenden Maschinen.

#### Erläuterung der Felder im Bereich Gesamtergebnis

Im Bereich **Gesamtergebnis** werden Ihnen die verschiedenen Optimierungsvarianten angezeigt. Mittels verschiedener Einstellungen (bspw. Abstellplatztiefe, oder welche Glasart als erste optimiert wird), können Sie verschiedene Ergebnisse in der Optimierung erzeugen / berechnen (verschiedene Varianten). Aus diesen Varianten können Sie dann im nächsten Schritt die Beste auswählen und speichern. So werden die Ausgaben (Papiere und Maschinencodes) nur für diese ausgewählte Variante erzeugt. Die Tabelle enthält erst dann Daten, wenn der Lauf gebildet und die Feinplanung und die Optimierung durchlaufen wurde:

*Abb. 1-8 Bereich Gesamtergebnis*

Das Feld **Variante** zeigt Ihnen, wie oft Sie die Feinplanung und die Optimierung durchlaufen haben. Mit jedem Klick auf die Symbol-Schaltfläche [Ausführen] wird eine weitere Variante erzeugt und dort gelistet. Die einzelnen Varianten bleiben Ihnen erhalten, so dass Sie sich schlussendlich für die beste Variante entscheiden können.

Im Feld **Abstellplatzorganisation** wird Ihnen die verwendete Abstellplatzorganisation angezeigt. Es handelt sich dabei um die Abstellplatzorganisation, die Sie im Bereich Feinplanung und Optimierung ausgewählt haben (der Wert kommt aus den Stammdaten: Fertigung > Abstellplatzorganisation).

Bei dem Feld **Faktor** handelt es sich um den Faktor der Abstellplatztiefe, den Sie im Bereich Feinplanung eingestellt haben.

Werden die Gläser in Fächerwagen gestellt, wird Ihnen im Feld **Anzahl Fächerwagen** angezeigt, wie viele Fächerwagen nötig sind, um alle Gläser des Laufs abzustellen. Kommen die Gläser auf A-Böcke, sehen Sie im Feld **Anzahl A-Böcke**, wie viele A-Böcke dazu nötig sind.

Im Feld **Ergebnis** wird Ihnen das Gesamtergebnis der Variante in % angezeigt und das Feld **Verschnitt** zeigt Ihnen den Gesamt-Verschnitt der Variante in Euro.

*Abb. 1-9 Bereich Optimierung je Variante*

Das Feld **Optimierung** zeigt Ihnen pro Variante die entsprechenden Optimierungen.

Im Feld **Glasart** werden Ihnen die im Lauf enthaltenen Glasarten angezeigt. Die Ziffer davor zeigt Ihnen die Reihenfolge in der Optimierung. Anschließend sehen Sie den Schneidtisch, auf dem das Glas geschnitten wird, gefolgt von der Laufnummer. Im Feld **Stückzahl** wird Ihnen je Glasart die Stückzahl angezeigt und im nächsten Feld die Fläche in Quadratmetern.

Im Feld **Ergebnis** wird Ihnen das Ergebnis der Optimierung für die jeweilige Glasart angezeigt. Zunächst sehen Sie das Ergebnis in %. Dahinter wird Ihnen in Klammern angezeigt, wie viele Muster und wie viele Lagerplatten die Optimierung benötigt sowie die verbleibende Restblattenlänge. Sollte der Produktionsmanager eine Glasart automatisch auf Handzuschnitt setzen, liegt das daran, dass die in den Stammdaten eingestellte Mindestfläche für die Optimierung nicht erreicht wird.

Anschließend wird Ihnen der Verschnitt in Euro angezeigt.

---

### Lagerplatten und Optimierungsparameter

Am rechten Bildschirmrand befinden sich zwei weitere Register, die bei Bedarf aufgeklappt werden können:

- Register Lagerplatten
- Register Optimierungsparameter

> **Register Lagerplatten und Optimierungsparameter**
> Nachdem Sie die Feinplanung und die Optimierung für einen Lauf durchlaufen haben, sind auch die Register Lagerplatten und Optimierungsparameter gefüllt.

Klicken Sie mit der Maus das Register **Lagerplatten** an, wird dieses geöffnet:
*Abb. I-10 Register Lagerplatten, am rechten Bildschirmrand*

Dieses Register liefert Ihnen alle Informationen zu den Lagerplatten der entsprechenden Glasart. Die hier angezeigten Werte werden im Modul Lager verwaltet.

Klicken Sie mit der Maus das Register **Optimierungsparameter** an, wird dieses geöffnet:
*Abb. I-11 Register Optimierungsparameter, am rechten Bildschirmrand*

Dieses Register liefert Ihnen alle Informationen zu der Optimierung der entsprechenden Glasart. Die hier angezeigten Werte kommen aus den Stammdaten (Artikel > Artikel).

Im Bereich **Allgemeine Einstellungen** können Sie zwischen folgenden Optimierungsmodi wählen:

- **XOPT**: Bei dieser Variante erfolgt die Optimierung chaotisch. D. h, die Reihenfolge der Scheiben nach der Optimierung ist nicht wichtig, die Scheiben einer Position müssen nicht zusammengehalten werden. Dadurch erzielt man zwar ein besseren Verschnitt, es müssen allerdings vor der ISO-Produktion alle Scheiben auf den A-Böcken umsortiert werden.
- **XOPT-S**: Dies ist der Standard-Modus für ISO-Betriebe. Hier wird die in der Abstellplatzorganisation vorgegebene Reihenfolge der Scheiben auf den Abstellplätzen eingehalten. Eine Synchronoptimierung der Scheiben ist möglich, damit Scheibe und Gegenscheibe auf der ISO-Linie zusammenpassen. Die Scheiben einer Auftragsposition stehen nach der Optimierung immer zusammen auf einem A-Gestell, d. h. die Position wird nicht gesplittet.

> **Register Lagerplatten und Optimierungsparameter**
> Nachdem Sie die Feinplanung und die Optimierung für einen Lauf durchlaufen haben, sind auch die Register Lagerplatten und Optimierungsparameter gefüllt.

### Informationen

In diesem Bereich haben Sie die Möglickeit, einen Auftrag über dessen Nummer gezielt zu suchen. Öffnen Sie hierzu das Menü Informationen und dann den Eintrag Auftrag suchen. Geben Sie die Auftragsnummer ein, die entsprechenden Daten werden angezeigt.

**So finden Sie Aufträge**

1.  Öffnen Sie im Menü den Eintrag Informationen.
2.  Betätigen Sie die Symbol-Schaltfläche [Auftrag]. Es öffnet sich die Auftragssuche.
3.  Geben Sie im Feld Auftragsnummer die gewünschte Nummer ein.
4.  Betätigen Sie die Symbol-Schaltfläche [Filter].

**Ergänzende Informationen**
⇨ Softwarereferenz, "Auftragssuche" auf Seite 1-143

---

## Expertenmodus

In diesem Themenblock lernen Sie den Umgang mit dem Produktionsmanager im Expertenmodus.

Dazu gehören folgende Lerneinheiten:

- "Überblick" auf Seite 1-24
- "Auftragsselektion" auf Seite 1-26

---

### Überblick

**Lernziele**

- Die Ansicht kennenlernen
- Wie werden die Daten geladen.
- Die Inhalte der Anzeigen übersichtlich aufbereiten.

**Nutzen**

- Im Expertenmodus führen Sie die einzelnen Schritte wie Läufe bilden, optimieren, etc. selber durch. Somit haben Sie die Möglichkeit über verschiedene Varianten zum bestmöglichen Ergebnis zu gelangen.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| Expertenmodus | In den Expertenmodus muss explizit umgeschaltet werden. |

---

### Expertenmodus starten

Den Expertenmodus starten Sie, indem Sie die entsprechende Symbol-Schalftläche betätigen. Er ist unter anderem für die mehrstufige Produktion von Gläsern gedacht. Sie nehmen alle notwendigen Schritte, wie z. B. die Zusammenstellung der einzelnen Läufe selbst vor. Sie können so Läufe bspw. aus verschiedenen Aufträgen und basierend auf spezifischen Bearbeitungsschritten zusammenstellen, oder aber aus verschiedenen Läufen eine gemeinsame Optimierung starten. In diesem Modus präsentiert sich das Programm wie folgt:

*Abb. I-12 Hauptdialog, Expertenmodus*

Der Production Manager besteht aus dem Hauptdialog mit verschiedenen Registern. Folgende Hauptregister stehen zur Verfügung:

- Auftragsselektion
- Laufübersicht
- Optimierungsmanager
- Optimierungsübersicht
- Ausgabe

Neben den Hauptregistern gibt es noch Register, die während der Laufzeit eingeblendet werden. Dazu zählt z. B. die Detailansicht, die Sie aus dem Register Laufansicht öffnen können. Diese Ansicht erscheint dann rechts neben dem Register Laufansicht.

---

### Auftragsselektion

In der Auftragsselektion können Sie über verschiedene Selektionskriterien Stücklistenteile einer Auftragsposition zu einem Lauf zusammenfassen. Sie dienen dazu, die Menge der Aufträge/Auftragspositionen/Stücklistenteile einzuschränken, die für die Laufbildung herangezogen werden sollen. Wird ein Auftrag selektiert, werden alle Positionen des Aufrags selektiert. Sie können jedoch einzelne Positionen an- und abwählen. Wählen Sie im Bereich Positionen eine Position aus, wird im Bereich Aufträge der entsprechende Auftrag ausgewählt.

Der Dialog ist in mehrere Bereiche eingeteilt. Rechts oben befindet sich die Liste der zu optimierenden Gläser. Hierüber können Sie sehen, wie groß der Lauf wird. Im unteren Bereich werden Ihnen Auftrags- und Positionsdaten zur Selektion angezeigt.

*Abb. I-13 Selektionskriterien*

Bei der Selektion können Sie wählen zwischen dem Nummernverwalter und dem Arbeitsgang. Innerhalb des Arbeitsganges können Sie zusätzlich auf das Produktionsdatum filtern.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Auftragsselektion" auf Seite 1-105

---

### Aufträge auswählen

In dieser Einheit lernen Sie, wie Sie Aufträge für den Produktionsmanager auswählen.

Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:

- So selektieren Sie Aufträge über den Nummernverwalter
- So selektieren Sie Aufträge über den Arbeitsgang
- So finden Sie Aufträge

**■ So selektieren Sie Aufträge über den Nummernverwalter**

1.  Klicken Sie auf die Symbol-Schaltfläche [Filter]. Die Felder werden zur Bearbeitung freigegeben.
2.  Aktivieren Sie die Radiotaste Nummernverwalter.
3.  Öffnen Sie die Kombobox.
4.  Wählen Sie einen entsprechenden NV aus.
5.  Betätigen Sie die Symbol-Schaltfläche [Suchen].
6.  Die Daten werden geladen.

**■ So selektieren Sie Aufträge über den Arbeitsgang**

1.  Klicken Sie auf die Symbol-Schaltfläche [Filter]. Die Felder werden zur Bearbeitung freigegeben.
2.  Aktivieren Sie die Radiotaste Arbeitsgang.
3.  Öffnen Sie die Kombobox.
4.  Wählen Sie einen entsprechenden Arbeitsgang aus.
    Wenn nötig, verwenden Sie die Datumsfelder von und bis, um die Auswahl einzugrenzen. Diese Felder stehen in Zusammenhang mit der Auswahl, die Sie im Feld Arbeitgang getroffen haben. Sie haben hier die Möglichkeit, den Arbeitsgang mit einem Datum einzugrenzen. Dieses Datum bezieht sich dann auf das Produktionsdatum. Bsp.: Arbeitsgang Bohren, Produktionsdatum 15.06.2013 bis 20.06.2013. Haben Sie als Arbeitsgang Versand gewählt, ist das eingegebene Datum das Versanddatum.
5.  Betätigen Sie die Symbol-Schaltfläche [Suchen].
    Die Daten werden geladen.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Auftragsselektion" auf Seite 1-105

---

### Die Bereiche Aufträge und Positionen

In diesen Bereichen werden Ihnen die Daten gemäß den Einstellungen im Bereich Selektionskriterien angezeigt. Der Bereich Aufträge gibt Ihnen einen Überblick zu den Aufträgen mit Auftragsnummer, Kundennummer, etc.

Die Inhalte des Bereichs Positionen sind abhängig von den Selektionskriterien. Um dies zu verdeutlichen, zeigen wir Ihnen im Anschluss zwei Beispiele. Wir verwenden immer den selben Auftrag, jedoch lassen wir uns diesen in Bezug auf unterschiedliche Arbeitsgänge anzeigen.

Wählen wir als Selektion den Eintrag **ISO-Fertigen**, werden folgende Daten angezeigt:
*Abb. I-14 Arbeitsgang ISO-Fertigen*

Im Bereiche Aufträge werden Ihnen alle Aufträge angezeigt, welche Positionen enthalten die gesäumt werden müssen (oder eben gebohrt). Wir wählen den Auftrag 20143 aus.

Im Bereich Positionen werden nun die einzelnen Positionen des Auftrags 20143 markiert, welche gesäumt werden müssen. Dabei ist zu beachten, dass alle Auftragspositionen eines Auftrages selektiert und in der Auswahlliste gesperrt sind, sobald Sie im Bereich Aufträge einen Auftrag auswählen und markieren.

Hier könnten wir nun einzelne Positionen auswählen und diese für einen eigenen Lauf berücksichtigen. Dazu müssen Sie im Bereich Aufträge zunächst die Markierung des Auftrags aufheben, und dann die relevanten Auftragspositionen im Bereich Positionen einzeln markieren (selektieren).

Wählen wir als Selektion den Eintrag **Zuschneiden**, werden folgende Daten angezeigt:
*Abb. I-15 Arbeitsgang Zuschneiden*

Im Bereich Positionen sehen Sie jetzt alle einzelnen Gläser, die zugeschnitten werden müssen.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Auftragsselektion" auf Seite 1-105

---

### Daten gruppieren

Es kann unter Umständen vorkommen, dass eine große Anzahl von Daten angezeigt wird. Um dennoch den Überblick zu behalten, haben Sie Möglichkeit, die Daten zu gruppieren und innerhalb der Gruppierung zu sortieren. Das Gruppieren von Daten ist für die Bereiche Aufträge und Positionen identisch. Um doppelte Beschreibungen zu vermeiden, wird die Vorgehensweise am Beispiel der Aufträge erläutert.

Die Gruppierungen nehmen Sie im Tabellenkopf vor:
*Abb. I-16 Daten gruppieren*

Über die Symbol-Schaltfläche [Spaltenauswahl] öffnen Sie ein Fenster, das alle Spalten enthält, nach denen gruppiert werden kann. Die folgende Grafik zeigt eine kleine Auswahl der Spalten.
*Abb. I-17 Spaltenauswahl*

### Daten sortieren

Um Daten innerhalb einer Gruppierung auf- oder absteigend zu sortieren, stehen Ihnen die Pfeile am Ende der Spalte zur Verfügung:

- `▲` sortiert die Daten aufsteigend
- `▼` sortiert die Daten absteigend.

Ist am Ende der Spalte kein Pfeil, erfolgt keine Sortierung.

Die Gruppierungen nehmen Sie in folgendem Bereich vor:
*Abb. I-18 Daten gruppieren*

---

### Daten übersichtlich darstellen

In dieser Einheit lernen Sie, wie Sie angezeigten Daten durch Gruppieren übersichtlich darstellen können.

Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:

- So gruppieren Sie Aufträge
- Weitere Gruppierungen hinzufügen
- So speichern Sie eine Gruppierung
- So entfernen Sie eine Gruppierung

**So gruppieren Sie Aufträge**

1.  Klicken Sie die Symbol-Schaltfläche [Spaltenauswahl] an. Es öffnet sich ein Auswahl-Dialog.
2.  Klicken Sie das gewünschte Feld (z. B. Kundennummer) mit der linken Maustaste an und halten Sie die Maustaste gedrückt.
3.  Mit gedrückter Maustaste ziehen Sie das Feld an die gewünschte Stelle im Tabellenkopf.
4.  An der entsprechenden Stelle angekommen, lassen Sie die Maustaste los.

*Abb. I-19 Daten nach Kundennummer gruppiert*

**■ Weitere Gruppierungen hinzufügen**

1.  Klicken Sie die Symbol-Schaltfläche [Spaltenauswahl] an. Es öffnet sich ein Auswahl-Dialog.
2.  Klicken Sie das gewünschte Feld (z. B. Erfassungsdatum) mit der linken Maustaste an und halten Sie die Maustaste gedrückt.
3.  Mit gedrückter Maustaste ziehen Sie das Feld an die gewünschte Stelle im Tabellenkopf.
4.  An der entsprechenden Stelle angekommen, lassen Sie die Maustaste los.

*Abb. I-20 Daten nach Kundennummer und Erfassungsdatum gruppiert*

**■ So speichern Sie eine Gruppierung**
Nachdem Sie die Gruppierung(en) erstellt haben, können Sie diese speichern.

1.  Betätigen Sie die Symbol-Schaltfläche [Speichern]. Es öffnet sich der Dialog Ansicht speichern.
2.  Geben Sie im Feld Name der Ansicht den entsprechenden Namen ein.
3.  Klicken Sie auf die Schaltfläche [OK]. Der Dialog wird geschlossen und der Name wird Ihnen rechts im Tabellenkopf angezeigt.

**■ So entfernen Sie eine Gruppierung**

1.  Wählen Sie die Gruppierung aus, die gelöscht werden soll.
2.  Klicken Sie auf die Symbol-Schaltfläche [X]. Die ausgewählte Gruppierung wird entfernt.

> **Gruppierungen löschen**
> Das Löschen von Gruppierungen erfolgt ohne Sicherheitsabfrage. Nachdem Sie die Symbol-Schaltfläche [X] betätigt haben, wird die Gruppierung gelöscht!

---

### Produkt

Am rechten Bildschirmrand befindet sich ein weiteres Register, das bei Bedarf aufgeklappt werden kann:
- Register Produkt

Klicken Sie mit der Maus das Register Produkt an, wird dieses geöffnet:
*Abb. I-21 Register Produkt, am rechten Bildschirmrand*

Dieses Register liefert Ihnen detaillierte Informationen zu der ausgewählten Position inklusive der Modellparameter und einer grafischen Vorschau mit Vermaßung.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Produkt" auf Seite I-111

### Informationen

Dieser Bereich ist identisch mit den gleichnamigen Bereichen im Standardmodus und wird an dieser Stelle nicht noch einmal erläutert.
⇨ "Informationen" auf Seite 1-22

---

### Bruchscheiben

Wenn bei der Produktion Scheiben mit Mängeln auftreten, können Sie diese zur Nachproduktion erfassen.

Klicken Sie mit der Maus auf die Symbol-Schaltfläche [Bruchscheiben], wird das Register Bruchpositionen geöffnet:
*Abb. I-22 Register Bruchpositionen*

Dieses Register zeigt Ihnen alle vorhandenen Bruchscheiben und liefert Ihnen detaillierte Informationen zu den noch zu verplanenenden Bruchscheiben. Um Inhalte zu filtern, stehen Ihnen die bereits oben erwähnten Gruppierungsmöglichkeiten zur Verfügung.

Sie haben an dieser Stelle folgende Möglichkeiten:
- Bruch erfassen
- Bruch löschen
- Einen Bruchlauf bilden

#### Bruch erfassen

Über diesen Dialog können Sie Bruchscheiben erfassen. Öffnen Sie im Register Bruchpositionen das Kontextmenü und anschließend den Eintrag Bruch erfassen. Es öffnet sich der gleichnamige Dialog.
*Abb. I-23 Bruch erfassen*

Über die Eingabe der Auftrags- und Positionsnummer und anschließendes Klicken auf die Symbol-Schaltfläche [Suchen] können Sie sich alle Stücklistenteile zu der eingegebenen Auftrags- und Positionsnummer anzeigen lassen.

Anschließend markieren Sie die Stücklistenteile, die als Bruch erfasst werden sollen und geben im Feld Menge die gewünschte Stückzahl ein.

#### Einen Bruchlauf bilden

Über diesen Dialog können Sie einen Bruchlauf bilden. Markieren Sie im Register Bruchpositionen die gewünschte Auftragsnummer, öffnen Sie das Kontextmenü und anschließend den Eintrag Neuen Bruchlauf erzeugen. Es öffnet sich der Dialog Neuen Lauf erstellen.
*Abb. I-24 Bruchlauf bilden*

Dieser Dialog wird im folgenden Kapitel detailliert beschrieben:
⇨ "Allgemein" auf Seite 1-39

---

### Mit Bruch arbeiten

In dieser Einheit lernen Sie, wie Sie mit Bruch umgehen.

Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
- So erfassen Sie Bruchscheiben
- So löschen Sie Bruchscheiben
- So erzeugen Sie einen neuen Bruchlauf

**■ So erfassen Sie Bruchscheiben**

1.  Klicken Sie die Symbol-Schaltfläche [Bruchscheiben] an. Es öffnet sich der Dialog Bruchpositionen.
2.  Geben Sie im Feld Auftrag die entsprechende Auftragsnummer ein.
3.  Geben Sie im Feld Position die entsprechende Positionsnummer ein.
4.  Klicken Sie auf die Symbol-Schaltfläche [Suchen]. In der Liste werden Ihnen die gewünschten Daten angezeigt.
5.  Selektieren Sie mit der Maus die Scheibe, die nachproduziert werden soll.
6.  Geben Sie im Feld Stückzahl die Menge ein, die nochproduziert werden soll.
7.  Wählen Sie aus der Kombobox Grund den Bruchgrund aus.
8.  Wählen Sie aus der Kombobox Stelle den Ort aus, an dem der Bruch passiert ist.
9.  Klicken Sie auf die Schaltfläche [Speichern], um die Daten zu speichern. Der Dialog ist wieder leer.
10. Klicken Sie auf die Schaltfläche [Schließen], um den Dialog zu schließen. Sie befinden sich wieder im Register Bruchscheiben.

**■ So löschen Sie Bruchscheiben**

1.  Klicken Sie die Symbol-Schaltfläche [Bruchscheiben] an. Es öffnet sich der Dialog Bruchpositionen.
2.  Markieren Sie die Position, die gelöscht werden soll.
3.  Öffnen Sie das Kontextmenü.
4.  Wählen Sie Bruch löschen. Es erfolgt eine Sicherheitsabfrage. Wenn Sie diese bestätigen, wird die ausgewählte Position gelöscht.

**■ So erzeugen Sie einen neuen Bruchlauf**

1.  Klicken Sie die Symbol-Schaltfläche [Bruchscheiben] an. Es öffnet sich der Dialog Bruchpositionen.
2.  Markieren Sie die Auftragsnummer, mit der Sie den Bruchlauf bilden möchten.
3.  Öffnen Sie das Kontextmenü.
4.  Wählen Sie Neuen Bruchlauf erzeugen. Es öffnet sich der Dialog Neuen Lauf erstellen.
5.  Geben Sie im Feld Bezeichnung die gewünschten Bezeichnung für den Bruchlauf ein.
6.  Wählen Sie aus der Kombobox Abstellplatzorganisation die gewünschte Organisation aus.
7.  Geben Sie im Feld Faktor für Abstellplatztiefe den gewünschten Faktor an.
8.  Bei Bedarf aktivieren Sie die Checkbox Unbegrenzte Abstellplatztiefe.
9.  Über die darunter liegenden Checkboxen steuern Sie, wie mit dem Lauf verfahren werden soll. Aktivieren Sie die gewünschte(n) Checkbox(en).
10. Klicken Sie auf die Schaltfläche [OK]. Die markierte Auftragsnummer verschwindet aus dem Register Bruchpositionen.

**Ergänzende Informationen**
- ⇨ Softwarereferenz, “Bruchpositionen" auf Seite I-113
- ⇨ Softwarereferenz, "Bruch erfassen" auf Seite I-116
- ⇨ Softwarereferenz, “Neuen Lauf erstellen" auf Seite 1-117

---

### Läufe verwalten

**Lernziele**
- Lernen, wie Sie einen Lauf erstellen.
- Wie werden die Daten geladen.
- Die Inhalte der Anzeigen übersichtlich aufbereiten.

**Nutzen**
- Wenn Sie Ihre Läufe optimal zusammenstellen, haben Sie einen geringeren Verschnitt.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| Laufnummer | Die Laufnummer wird vom System vergeben. |
| Abstellplatzorganisation | Kann nach der Laufbildung noch geändert werden. |
| Abstellplatztiefe | Durch die Veränderung der Abstellplatztiefe haben Sie Einfluss auf das Optimierungsergebnis. |

---

### Allgemein

Bei der Bildung von Läufen gehen alle selektierten und nicht anderweitig verplanten Teile in den Lauf.

Läufe werden entweder mit Hilfe des Nummerverwalters oder aber pro Arbeitsgang im Register Auftragsselektion gebildet (Kontextmenü Neuen Lauf erstellen). Es erscheint folgender Dialog:

*Abb. 1-25 Neuen Lauf erstellen*

#### Erläuterung der Felder

Als **Laufnummer** wird vom Programm die nächst höhere Nummer vergeben. Im Feld **Bezeichnung** können Sie detaillierte Beschreibung zum Lauf hinterlegen. Anschließend wählen Sie aus der Kombobox **Abstellplatzorganisation** die gewünschte Organisationsform aus. Die Kombobox enthält alle in Ihrem Haus angelegten Abstellplatzorganisationen.

Bei dem **Faktor für Abstellplatztiefe** handelt es sich um den Faktor für die im Lauf zu verwendende Gestelltiefe in Prozent. Der Wert für die Abstellplatztiefe kommt aus dem Stammdaten (`Fertigung > Logische Abstellplätze`). Über den Faktor können Sie den Wert temporär verändern. 100% bedeutet, dass der in den Stammdaten hinterlegte Wert verwendet wird. 90% bedeutet, dass die in den Stammdaten hinterlegte Tiefe nur zu 90% genutzt wird, d. h. es gehen weniger Scheiben auf den Abstellplatz. Eine Korrektur des Wertes nach oben führt zu einer Überbeladung.

Aktivieren Sie die Checkbox **Unbegrenzte Abstellplatztiefe** überschreiben Sie jegliche Werte aus den Stammdaten.

Über die Checkboxen im Bereich **Aktionen nach Lauferstellung** steuern Sie, wie mit dem Lauf verfahren wird.
Aktivieren Sie die Checkbox **Feinplanung**, erfolgt nach der Laufbildung automatisch die Feinplanung. Die Checkbox **Optimierungsmanager** können Sie nur aktivieren, wenn die Checkox Feinplanung aktiv ist. Dann öffnet sich nach der Laufbildung und der Feinplanung das Register Optimierungsmanager. Es wird jedoch keine Optimierung erzeugt! Die Checkbox **Kompletter Handzuschnitt** können Sie ebenfalls nur aktivieren, wenn die Checkbox Feinplanung aktiv ist. Dann werden nach der Laufbildung und der Feinplanung alle Scheiben auf Handzuschnitt gesetzt.
Die Checkbox **Ausgabe** ist nur aktiv, wenn die Checkboxen Feinplanung und Kompletter Handzuschnitt aktiv sind. Dann wird nach der Laufbildung, der Feinplanung und dem Handzuschnitt direkt in das Register Ausgabe gewechselt.

#### Der Lauf wurde gebildet ...

Nachdem der Lauf gebildet wurde, hat er den Status *Grobgeplant*. Die gebildeten Läufe finden Sie im Register **Laufübersicht**.

Mit grobgeplanten Läufen können Sie folgendes tun:

- Die bei der Laufbildung zugewiesene Abstellplatzorganisation kann geändert werden.
- Sie können weitere Teile diesem Lauf hinzufügen.
- Sie können Teile aus dem Lauf löschen.
- Sie können den Lauf auflösen.
- Sie können den Lauf an die Feinplanung übergeben.

*Abb. I-26 Hauptdialog, Expertenmodus, Laufübersicht*

Der Dialog ist in mehrere Bereiche eingeteilt. Im oberen Bereich befinden sich die Selektionskriterien. Im unteren Bereich werden Ihnen die existierenden Läufe angezeigt.

---

#### Informationen und Filtereinstellungen

*Abb. I-27 Selektionskriterien für Läufe*

Über das Feld **Laufnummer** können Sie sich gezielt Läufe nach deren Nummer anzeigen lassen. Das setzt voraus, dass Sie die Nummer des Laufes, den Sie sich anzeigen lassen wollen, kennen. Die Felder dienen auch dazu, die angezeigten Läufe zu limitieren, um den Überblick zu behalten.

Über die Felder **Erstelldatum** können Sie sich die Läufe nach dem Datum anzeigen lassen, an dem sie erstellt wurden.

Mit hilfe der Komboboxen **Status** können Sie sich die Läufe nach deren Status anzeigen lassen. Folgende Status sind möglich:

- **Grobgeplant**: Für diese Läufe ist noch keine Abstellplatzvergabe erfolgt.
- **Feingeplant**: Für diese Läufe erfolgte eine Abstellplatzvergabe.
- **Teiloptimiert**: Einige Glasarten dieser Läufe wurden bereits optimiert.
- **Optimiert**: Alle Glasarten dieser Läufe wurden bereits optimiert.
- **Teilfertig**: Wird zur Zeit noch nicht ausgewertet.
- **Fertig**: Alle Teile, die zu diesen Läufen gehören, sind fertig.

Über das Feld **Bezeichnung** können Sie sich die Läufe nach deren Bezeichnung anzeigen lassen. Diese Bezeichnung haben Sie beim Erstellen eines Laufes im Dialog Neuen Lauf erstellen vergeben.

#### Informationen und Filtereinstellungen im Bereich Läufe

In der Spalte **Laufnummer** wird Ihnen die Laufnummer angezeigt, die Sie im Register Laufübersicht selektiert haben. Anschließend sehen Sie das Datum, an dem der Lauf erstellt wurde. In der Spalte **Bezeichnung** wird Ihnen die Laufbezeichnung angezeigt, die Sie beim Erstellen des Laufes angegeben haben. Dann folgt die Abstellplatzorganisation, die Sie bei der Laufbildung gewählt haben sowie der Laufstatus. Die Felder **ISO, VSG, ESG und Glas** zeigen Ihnen die im Lauf enthaltenen Mengen der jeweiligen Art.

Einträge, die in diesem Bereich hellgrau dargestellt werden, wurden bereits an den Optimierungsmanager übergeben. Klicken Sie einen solchen Eintrag an, erscheint eine entsprechende Meldung am Bildschirm. Sie können sich für diese Einträge die Detailansicht und die Feinplanungsergebnisse anzeigen lassen sowie die Ausgabe (Maschinen, Reports, etc.) starten.

Es kann unter Umständen vorkommen, dass eine große Anzahl von Daten angezeigt wird. Um dennoch den Überblick zu behalten, haben Sie Möglichkeit, die Daten zu gruppieren und innerhalb der Gruppierung zu sortieren.

Die Vorgehensweise wurde bereits im Register Auftragsselektion erläutert und wird an dieser Stelle nicht noch einmal beschrieben.
⇨ "Daten gruppieren" auf Seite 1-30

**Ergänzende Informationen**
- ⇨ Softwarereferenz, "Neuen Lauf erstellen" auf Seite I-117
- ⇨ "Läufe über bestimmte Kriterien auswählen" auf Seite 1-43

---

### Läufe über bestimmte Kriterien auswählen

In dieser Einheit lernen Sie, wie Sie Läufe zur Produktion auswählen.

Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:

- So selektieren Sie Läufe über die Laufnummer
- So selektieren Sie Läufe über das Erstelldatum
- So selektieren Sie Läufe über die Bezeichnung

#### So selektieren Sie Läufe über die Laufnummer

1.  Klicken Sie auf die Symbol-Schaltfläche [Filter]. Die Felder werden zur Bearbeitung freigegeben.
2.  Tragen Sie im Feld **von** die kleinste Laufnummer ein und im Feld **bis** die größte Laufnummer. Wenn Sie in beiden Feldern dieselbe Nummer eintragen, wird nur dieser eine Lauf angezeigt.
3.  Klicken Sie auf die Symbol-Schaltfläche [Suchen].
4.  Die Daten werden geladen.

#### So selektieren Sie Läufe über das Erstelldatum

1.  Klicken Sie auf die Symbol-Schaltfläche [Filter]. Die Felder werden zur Bearbeitung freigegeben.
2.  Tragen Sie in den Feldern **von** bis das entsprechende Erstelldatum ein. Wenn Sie in beiden Feldern dasselbe Datum eintragen, werden nur die Läufe angezeigt, die an diesem Tag erstellt wurden.
3.  Klicken Sie auf die Symbol-Schaltfläche [Suchen].
4D. Die Daten werden geladen.

#### So selektieren Sie Läufe über den Status

1.  Klicken Sie auf die Symbol-Schaltfläche [Filter]. Die Felder werden zur Bearbeitung freigegeben.
2.  Tragen Sie in den Feldern **von** bis die entsprechenden Kriterien aus.
3.  Klicken Sie auf die Symbol-Schaltfläche [Suchen].
4.  Die Daten werden geladen.

#### So selektieren Sie Läufe über die Bezeichnung

1.  Klicken Sie auf die Symbol-Schaltfläche [Filter]. Die Felder werden zur Bearbeitung freigegeben.
2.  Tragen Sie in den Felder **Bezeichnung** den entsprechenden Text ein.
3.  Klicken Sie auf die Symbol-Schaltfläche [Suchen].
4.  Die Daten werden geladen.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Neuen Lauf erstellen" auf Seite I-117

---

### Detailansicht für Läufe

Über das Kontextmenü haben Sie die Möglichkeit, sich Läufe im Detail anzusehen. Der entsprechende Lauf wird dann in einem separaten Register angezeigt.

Im nachfolgenden Beispiel öffnen wir für den Lauf 1379 die Detailansicht. Dazu wird der Lauf in der Laufübersicht selektiert.

Anschließend können Sie über das Kontextmenü den Eintrag Detailansicht wählen.

Der Lauf wird mit allen seinen Bestandteilen in einem separaten Register angezeigt. Dieser Dialog ist ebenfalls in verschiedene Bereiche unterteilt:

*Abb. I-28 Detailansicht für Lauf 1379*

#### Informationen im Bereich Feinplanung:
*Abb. I-29 Bereich Feinplanung*

In diesem Bereich werden Ihnen die Daten angezeigt, die Sie bei der Bildung des Laufes eingegeben oder ausgewählt haben.

Sie sehen die Laufbezeichnung, die Sie an dieser Stelle noch ändern können. Ebenso können Sie die Abstellplatzorganisation noch ändern, indem Sie die Kombobox öffnen und eine andere Organisationsform zuweisen. Die Felder Erstelldatum und Status können nicht geändert werden. Das Erstelldatum zeigt Ihnen, wann der Lauf erstellt wurde und das Feld Status zeigt Ihnen, in welchem Status sich der Lauf befindet. An dieser Stelle können Sie auch den Faktor für die Abstellplatztiefe noch ändern bzw. dem Abstellplatz eine unbegrenzte Tiefe zuweisen.

#### Informationen im Bereich Optimierungsartikel:
*Abb. I-30 Bereich Optimierungsartikel*

Hier sehen Sie, um welche Glasart es sich handelt, die zu optimierende Menge sowie die Quadratmeter pro Glasart und die entsprechende Quadratmeterzahl im Verhältnis zur Gesamtfläche des Laufes.

**Beispiel:**
Der Lauf hat eine zu optimierende Gesamtfläche von 67,86 m². Der Artikel 104 A+W Float 4 mm hat eine Fläche von 16,35 m². Diese 16,35 m² sind 24,10 % von der Gesamtfläche.

Im Bereich **Aufträge und Positionen** werden Ihnen alle auftragsrelevanten Informationen angezeigt, wie bspw. Auftragsnummer, Kundennummer und Versanddatum.

Im Bereich **Positionen** werden nun die positionsbezogenen Informationen der entsprechenden Aufträge angezeigt, wie bspw. Stückzahl, Modellnummer, Beschaffungsart.

**Ergänzende Informationen**
- ⇨ Softwarereferenz, "Detailansicht" auf Seite 1-121
- ⇨ "Erläuterung der Felder im Bereich Aufträge" auf Seite 1-106
- ⇨ "Erläuterung der Felder im Bereich Positionen" auf Seite I-107

---

### Register Produkt und Zuschnitt

Am rechten Bildschirmrand befinden sich zwei weitere Register, die bei Bedarf aufgeklappt werden können:

- Register Produkt
- Register Zuschnitt

#### Register Produkt

Dieses Register ist identisch mit dem gleichnamigen Register im Bereich Auftragsselektion und wird an dieser Stelle nicht noch einmal erläutert.
⇨ "Produkt" auf Seite 1-33

#### Register Zuschnitt

Klicken Sie mit der Maus das Register Zuschnitt an, wird dieses geöffnet:
*Abb. I-31 Register Zuschnitt, am rechten Bildschirmrand*

Es liefert Ihnen detaillierte Informationen zu der ausgewählten Position inklusive der Modellparameter und einer grafischen Vorschau mit Vermaßung. Die gestrichelte Linie kennzeichnet die Modellbruchränder.

Klicken Sie auf die Schaltfläche [Bearbeiten], öffnet sich der Dialog **Zuschnitt bearbeiten**.
*Abb. I-32 Zuschnitt bearbeiten*

In diesem Dialog können Sie diverse Änderungen vornehmen. Sie können z. B. ein anderes Modell auswählen, die Modellparameter sowie die Modellbruchränder und die zu prozierende Stückzahl ändern. Die Modellbruchränder werden Ihnen durch die gestrichelte Linie angezeigt.

Wenn Sie Änderungen vorgenommen haben, werden Ihnen diese sofort im Bereich Vorschau angezeigt.

> **Zuschnittdaten bearbeiten**
> Bitte bedenken Sie, dass Änderungen, die Sie hier vornehmen, lediglich den Zuschnitt betreffen. Diese Änderungen werden nicht an das Auftragsbearbeitungssystem zurück gemeldet!

#### Das Register Produkt

Das Register Produkt ist identisch mit dem gleichnamigen Register in der Detailansicht für Läufe und wird an dieser Stelle nicht noch einmal erläutert.
⇨ "Register Produkt und Zuschnitt" auf Seite 1-47

**Ergänzende Informationen**
⇨ Softwarereferenz, "Zuschnitt bearbeiten" auf Seite 1-125

---

### Feinplanung

**Lernziele**
- Die Feinplanung kennen lernen und verstehen
- Die Optimierungsmodi kennenlernen und verstehen
- Unter welchen Umständen wird welcher Modus verwendet

**Nutzen**
- Wenn Sie die unterschiedlichen Optimierungsmodi kennen und verstehen, können Sie die Feinplanung auf Ihre Produktion so anpassen, dass diese kostengünstig und zeitsparend arbeitet.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| Variante | Die durchgeführten Optimierungsvarianten bleiben erhalten, so dass Sie die Beste auswählen können. |
| Feinplanung | Aufteilen der Gläser eines Auftrags auf verschiedene Glasstapel und Abstellplätze (Gestelle) nach definierten Kriterien für Gruppierung und Sortierung. |

---

### Ablauf der Feinplanung

Die grobgeplanten Läufe können aus dem Register Laufübersicht an die Feinplanung übergeben werden. Aufgabe der Feinplanung ist es, für die in den Läufen enthaltenen Teile die Produktionsreihenfolge zu erstellen.

Die Produktionsreihenfolge kann sich durch folgende Kriterien ergeben:

- Durch die Vorgaben des Kunden
- durch fertigungstechnische Restriktionen

In diesem Schritt erfolgt auch die aktuell zugewiesene Abstellplatzorganisation. Der Status des Laufes wechselt von Grobgeplant in Feingeplant.

Mit feingeplanten Läufen können Sie folgendes tun:

- Sie können die Feinplanung beliebig oft wiederholen (z. B. wegen geänderter Stammdaten der Abstellplatzorganisation).
- Sie können feingeplante Läufe an den Optimierungsmanager übergeben.
- Sie können den Lauf auflösen.
- Sie können sich die Gestellbelegung anzeigen lassen.

---

### Optimierungsmanager

Feingeplante Läufe können an den Optimierungsmanager übergeben werden. Nachdem Sie die erste Optimierung für einen Lauf durchgeführt und bestätigt haben, ändert sich der Status in Teiloptimiert.

Mit teiloptimierten Läufen können Sie folgendes tun:

- Sie können die Ausgabe für einzelne Optimierungen des Laufs durchführen.
- Sie können mit diesen Läufen alles tun, was mit feingeplanten Läufen auch getan werden kann (außer dem Auflösen des Laufes).

*Abb. I-33 Optimierungsmanager*

In diesem Register werden die Optimierungen der einzelnen Glasarten für die ausgewählten Läufe durchgeführt.

Dieser Dialog ist ebenfalls in verschiedene Bereiche unterteilt.

---

#### Erläuterung der Felder im Bereich Läufe

*Abb. I-34 Bereich Läufe*

In der Spalte **Laufnummer** wird Ihnen die Laufnummer angezeigt, die Sie im Register Laufübersicht selektiert haben. Anschließend sehen Sie das Datum, an dem der Lauf erstellt wurde sowie den Laufstatus. In der Spalte **Bezeichnung** wird Ihnen die Laufbezeichnung angezeigt, die Sie beim Erstellen des Laufes angegeben haben. Dann folgt die Abstellplatzorganisation, die Sie bei der Laufbildung gewählt haben. Die Felder **ISO, VSG, ESG, Glas** zeigen Ihnen die im Lauf enthaltenen Mengen der jeweiligen Art. Bei dem Faktor für Abstellplatztiefe handelt es sich ebenfalls um den Faktor, den Sie bei der Lauferstellung angegeben haben.

#### Erläuterung der Felder im Bereich Glasarten

*Abb. I-35 Bereich Glasarten*

Hier werden Ihnen die einzelnen Glasarten, die im Lauf enthalten sind, angezeigt. Wenn Sie den Eintrag der Glasart aufklappen, erhalten Sie Informationen zu der Stückzahl, der Fläche und dem Lauf.

Da mehrere Läufe in den Optimierungsmanager geladen werden können, sehen Sie hier, aus welchen Läufen die einzelnen Glasarten kommen.

#### Die Bereiche Optimierungen und Gesamtergebnis

Die Felder im Bereich Optimierungen und Gesamtergebnis sind identisch mit den gleichnamigen Bereichen im Standardmodus und werden an dieser Stelle nicht noch einmal erläutert.
⇨ "Ergebnisse" auf Seite 1-19

---

#### Die Register Lagerplatten und Optmierungsparameter

Die am rechten Bildschirmrand liegenden Register Lagerplatten und Optimierungsparameter sind identisch mit den gleichnamigen Registern im Bereich Standardmodus und werden an dieser Stelle nicht noch einmal erläutert.
⇨ "Lagerplatten und Optimierungsparameter" auf Seite 1-21

### Läufe optimieren

In dieser Einheit lernen Sie, wie Sie Läufe optimieren.

Zu dieser Lerneinheit gibt es folgende Handlungsanweisungen:
- So übergeben Sie Läufe an den Optimierungsmanager
- So setzen Sie eine Glasart auf Handzuschnitt
- So starten Sie die Optimierung
- So speichern Sie die Optimierung

**■ So übergeben Sie Läufe an den Optimierungsmanager**

1.  Markieren Sie im Register Laufübersicht den oder die gewünschten Läufe.
2.  Öffnen Sie das Kontextmenü.
3.  Klicken Sie auf den Menü-Eintrag Optimierungsmanager. Das Register Optimierungsmanager wird geöffnet und die Daten werden geladen.

> **Läufe übergeben**
> Sie können nur Läufe an den Optimierungsmanager übergeben, die den Status Feingeplant haben!

**■ So setzen Sie eine Glasart auf Handzuschnitt**

1.  Markieren Sie im Bereich Optimierungen den oder die gewünschten Glasarten.
2.  Öffnen Sie das Kontextmenü.
3.  Klicken Sie auf den Menü-Eintrag Handzuschnitt. Das Häkchen vor der Glasart verschwindet und im Feld Ergebnis erscheint der Eintrag Handzuschnitt.

**■ So starten Sie die Optimierung**

1.  Markieren Sie im Register Optimierungsmanager im Bereich Optimierungen die gewünschte Glasart.
2.  Öffnen Sie das Kontextmenü.
3.  Klicken Sie auf den Menü-Eintrag Optimierung starten. Nachdem die Optimierung durchlaufen wurde, wird der Bereich Gesamtergebnis mit Daten gefüllt.

---

> **Ribbon-Leiste**
> Die Optimierung können Sie auch über die Ribbon-Leiste (Ausführen) starten. Dann entfällt das Öffnen des Kontextmenüs.

**■ So speichern Sie die Optimierung**

1.  Öffnen Sie das Kontextmenü.
2.  Klicken Sie auf den Menü-Eintrag Optimierung speichern. Die Optimierung wird gespeichert.

> **Ribbon-Leiste**
> Das Speichern können Sie auch über die Ribbon-Leiste (Speichern) durchführen. Dann entfällt das Öffnen des Kontextmenüs.

### Temporäre Optimierung

Mit jedem Klick auf die Symbol-Schaltfläche [Ausführen] wird eine neue Optimierung durchgeführt. Diese Vorgehensweise dient dazu, Läufe mit unterschiedlichen Variationen zu optimieren. So können Sie z. B. Glasarten tauschen, Optimierungsparameter oder Lagerplatten ändern. Die durchgeführten Optimierungen werden als Varianten im Bereich Gesamtergebnis angezeigt.

Im Bereich Optimierungen können Sie über das Kontextmenü die Detailansicht öffnen. Diese wird in einem separaten Register angezeigt.

*Abb. I-36 Optimierungsmanager, Detailansicht*

Dieser Dialog ist ebenfalls in verschiedene Bereiche unterteilt.

#### Erläuterung der Felder im Bereich Gestell

*Abb. I-37 Bereich Gestell*

Hier werden Ihnen alle relevanten Informationen zu den Gestellen angezeigt. In der Spalte **Laufnummer** wird Ihnen die Laufnummer angezeigt, die Sie im Register Optimierungsmanager selektiert haben. Anschließend sehen Sie die Gestellnummer sowie den Gestell-Typ, auf dem die Scheiben abgestellt werden und dem logischen Abstellplatz.

#### Erläuterung der Felder im Bereich Läufe

*Abb. I-38 Bereich Läufe*

In der Spalte **Laufnummer** wird Ihnen die Laufnummer angezeigt, die Sie im Register Optimierungsmanager sowie das Datum, an dem der Lauf erstellt wurde.

#### Erläuterung der Felder im Bereich Lagermaße

*Abb. I-39 Bereich Lagermaße*

In der Spalte **Menge** wird Ihnen die benötigte Anzahl an Lagerplatten angezeigt. Die Felder **Höhe** und **Breite** zeigen Ihnen die Abmessungen der verwendeten Lagerplatten. Im Feld **Fläche** sehen Sie die Fläche in Quadratmeter und im Feld **Priorität** die entsprechende Priorität.

#### Erläuterung der Felder im Bereich Muster

*Abb. I-40 Bereich Muster*

In der Spalte **Muster** werden Ihnen die einzelnen Muster aufgelistet. Klicken Sie ein Muster an, wird es auf der rechten Sei im Bereich Schneidplan grafisch angezeigt. Das Feld **Optigruppe** zeigt Ihnen die Optimierungsgruppe. Im Feld **Menge** sehen Sie die Menge bezogen auf das Muster. Die Felder **Höhe** und **Breite** zeigen Ihnen die Abmessungen der verwendeten Lagerplatten.

#### Erläuterung der Felder im Bereich Schneidplan

*Abb. I-41 Bereich Schneidplan*

In diesem Bereich wird Ihnen das bei der Optimierung erzeugte Schneidmuster grafisch dargestellt. Die Darstellung entspricht dem zu schneidenden Lagermaß und enthält alle wichtigen Informationen über die Optimierung, den Artikel und die einzelnen Scheiben.

Bei der oberen Zahl handelt es sich um die Gestell-Nr. (z. B. 7968). Anschließend folgt die Abmessung der Scheibe (z. B. 1200x800). Darunter befindet sich die Auftragsnummer und die dazugehörige Position.

**Ergänzende Informationen**
⇨ "Lagerplatten und Optimierungsparameter" auf Seite 1-21

---

### Optimierung abbrechen

Hier haben Sie die Möglichkeit, eine Optimierung, die gerade durchlaufen wird, durch Klicken auf die Schaltfläche [Abbrechen] zu stoppen.

*Abb. I-42 Optimierung abbrechen*

**Ergänzende Informationen**
⇨ Softwarereferenz, "Optimierung abbrechen" auf Seite 1-132
