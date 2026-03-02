---
description: "A+W Business Pro Capacity Planning Tutorial and Reference"
---


# Tutorial

---
## Kapazitätsplanung

### Produktionslisten

4. Wählen Sie im Menü Start > Suchen, um die Suche zu starten.

*Abb. H-99 Detaillierte Produktionsliste*

- **A** Pakete der Auftragsposition 1
- **B** Auftragsnummer

In dieser Übersicht werden zu jeder Arbeitsart die Unterpositionen jeder Position aufgelistet.

Wenn Sie die Ausgabe an einen Drucker senden, achten Sie darauf, dass Sie ein Querformat benötigen, damit alle Daten dargestellt werden können.

*Abb. H-100 Beispiel Produktionsliste (Seite 1)*

Pro Aggregat und Tag wird eine Seite erstellt.

## Auftrag manuell fertig melden

Beim manuellen Fertigmelden haben Sie folgende Möglichkeiten:
- Aufträge komplett
- Einzelne Auftragspositionen komplett
- Teilmenge einer Auftragsposition

Im nachfolgenden Beispiel wird eine Teilmenge fertig gemeldet.

> **i Scannen**
> Wenn Sie mit einem Scanner arbeiten, prüfen Sie zuerst im Menü Optionen, ob die Erfassung des Barcodes aktiviert ist. Der Cursor steht dann automatisch in dem Feld für den Barcode.

### So melden Sie einen Auftrag an einem Aggregat fertig

1. Wählen Sie Fertigung > Kapazitätsplanung > Fertigmeldung > Manuell.
Der Dialog Manuelle Fertigmeldungen wird geöffnet.
2. Wählen Sie im Menü Funktionen > Einstellungen.

*Abb. H-101 Auswahl der Aggregate*

Eine Beschreibung des Dialogs finden Sie in der Softwarereferenz.
⇨ Softwarereferenz, "Einstellungen für manuelle Fertigmeldungen" auf Seite H-317

3. Wählen Sie die Aggregate aus, zu denen Sie die Fertigmeldungen erfassen wollen, und übernehmen Sie die Auswahl mit [OK].
Sie können mehrere Aggregate markieren.

*Abb. H-102 Manuelle Fertigmeldung*

- **A** Option Fertigmeldung
- **B** Feld für Barcode
- **C** Auftragsnummer
- **D** Positionsnummer
- **E** Fertig zu meldende Stückzahl
- **F** Mengenangabe freischalten
- **G** Auswahl des Aggregats

Eine Beschreibung des Dialogs finden Sie in der Softwarereferenz.
⇨ Softwarereferenz, “Manuelle Fertigmeldung" auf Seite H-314

4. Prüfen Sie, ob die Option Fertigmeldung (A) aktiviert ist.
5. Geben Sie die Auftragsnummer (C) ein oder erfassen Sie den Barcode.
Der Cursor springt in das nächste Feld.
6. Geben Sie im Feld Position von (D) die Positionsnummer ein und drücken Sie die <Tab>-Taste.
Die Position wird eingelesen und die Stückzahl wird angezeigt.
7. Markieren Sie die Checkbox mit Mengenangabe (F).
Wenn Sie den Barcode per Scanner erfasst haben, wird genau 1 Scheibe fertig gemeldet. Sie müssen daher die Checkbox markieren und die Anzahl der fertigen Scheiben manuell eintragen.
Wenn Sie aber die gesamte Position fertig melden wollen, dann markieren Sie die Checkbox Position komplett. Die Mengenangabe entfällt dann.
8. Tragen Sie im Feld Menge (E) die Stückzahl ein, die Sie fertig melden wollen.
9. Markieren Sie im Feld Aggregat-Auswahl (G) das Aggregat, an dem die Stückzahl fertiggestellt wurde.
10. Ergänzen Sie ggf. das Datum und die Schicht.

*Abb. H-103 Angaben zur manuellen Fertigmeldung einer Teilmenge*

- **A** Teilmenge
- **B** Fertig melden

11. Klicken Sie auf [Position fertig melden (F9)].

*Abb. H-104 Teilmenge fertig gemeldet*

Die angegebene Stückzahl wird fertig gemeldet.

## Bruchmeldung manuell erfassen

Sie können Bruchmeldungen nur für Positionen erfassen, die bereits fertig gemeldet wurden. Für die manuelle Bruchmeldung haben Sie folgende Möglichkeiten:

- **Bruchmeldung Eingang:**
Die angegebenen Stückzahlen werden am Eingang des Aggregats als Bruch gemeldet. Sie müssen an der vorherigen Maschine erneut gefertigt werden.
- **Bruchmeldung Ausgang:**
Die angegebenen Stückzahlen werden am Ausgang des Aggregats als Bruch gemeldet. Sie müssen an derselben Maschine erneut gefertigt werden.

### So melden Sie zu einer Position einen Bruch

1. Wählen Sie Fertigung > Kapazitätsplanung > Fertigmeldung > Manuell.
Der Dialog Manuelle Fertigmeldungen wird geöffnet.
2. Wählen Sie im ggf. Menü Funktionen > Einstellungen die Aggregate aus, zu denen Sie die Bruchmeldungen erfassen wollen.

*Abb. H-105 Manuelle Fertigmeldung*

- **A** Option Fertigmeldung
- **B** Auftragsnummer
- **C** Positionsnummer
- **D** Anzahl der fehlerhaften Scheiben
- **E** Mengenangabe freischalten
- **F** Auswahl des Aggregats

Eine Beschreibung des Dialogs finden Sie in der Softwarereferenz.
⇨ Softwarereferenz, "Manuelle Fertigmeldung" auf Seite H-314
3. Tragen Sie die Auftragsnummer (B) ein oder erfassen Sie den Barcode.
Der Cursor springt in das nächste Feld.
4. Geben Sie die Positionsnummer (C) ein und drücken Sie die <Tab>-Taste.
Die Position wird eingelesen und die Stückzahl wird angezeigt.
5. Wählen Sie die Meldungsart (A) aus.
Mit dieser Einstellung entscheiden Sie, ob die fehlerhaften Scheiben am vorigen oder am selben Aggregat erneut gefertigt werden müssen.
6. Tragen Sie im Feld Menge (D) die Stückzahl ein, die Sie fertig melden wollen.
Wenn Sie den Barcode per Scanner erfasst haben, wird genau 1 Scheibe gemeldet.
7. Markieren Sie im Feld Aggregat-Auswahl (G) das Aggregat, an dem der Bruch gemeldet werden soll.
8. Ergänzen Sie ggf. das Datum und die Schicht.
9. Klicken Sie auf [Position fertig melden (F9)].

*Abb. H-106 Bruchmeldung für Teilmenge*

Die Daten werden gespeichert. Die Bestätigung wird unter der Schaltfläche angezeigt.
Wenn die beanstandeten Scheiben neu gefertigt wurden, wird der Positionsstatus hochgesetzt.

> **i Bruchmeldung kann nicht bestätigt werden**
> Wenn die Bruchmeldung nicht bestätigt wird, müssen Sie die Position zuerst fertig melden. Nachdem Sie die Fertigmeldung abgeschlossen haben, können Sie die Bruchmeldung erfassen.

## Fertigungsstand prüfen

Sie können den Fertigungsstand der Aufträge detailliert prüfen und vergessene Fertigmeldungen nachholen. Dazu können Sie sich die Aufträge eines Kunden oder alle Aufträge zu einem bestimmten Liefertermin gesammelt anzeigen lassen.

### So prüfen Sie den Fertigungsstand einzelner Auftragspositionen

1. Wählen Sie Fertigung > Kapazitätsplanung > Fertigungsstand Auftrag.

*Abb. H-107 Fertigungsstand eines Auftrags prüfen*

Eine Beschreibung des Dialogs finden Sie in der Softwarereferenz.
⇨ Softwarereferenz, "Fertigungsstand Auftrag" auf Seite H-323
2. Tragen Sie die Nummer des Auftrags oder des Kunden ein.
Wenn Sie das Lieferdatum eintragen, schränken Sie die Auswahl weiter ein. Oder Sie lassen sich damit alle Aufträge zum angegebenen Datum anzeigen.
3. Wählen Sie im Menü Start > Suchen, um die Daten einzulesen.
Die Auftragsdaten werden eingelesen und im Register Auswahl angezeigt.
Wenn Sie als Auswahlkriterium die Kundennummer gewählt haben, werden alle Aufträge des Kunden angezeigt, auch die bereits gefertigten.
4. Wechseln Sie zum Register Positionen, um den Fertigungsstand der einzelnen Auftragspositionen zu prüfen.

*Abb. H-108 Fertigungsstand der Positionen prüfen*

- **A** Stückzahl der Position
- **B** Fertig gemeldete Teilmenge
- **C** Position komplett fertig melden

5. Prüfen Sie das Datum, zu dem Sie die Position fertig melden wollen.
6. Markieren Sie die Checkbox Fertig melden (C) in der Position, die bereits vollständig gefertigt wurde.
Eine Sicherheitsabfrage wird angezeigt. Wenn Sie die Meldung bestätigt haben, wird die Stückzahl der Position in die Spalte komplett fertig eingetragen.

## Fertigmeldungen nachholen

Ob Aufträge nicht fertig gemeldet wurden, können Sie auch prüfen, indem Sie sich die Restmengen vom Vortag anzeigen lassen.

### So prüfen Sie, ob Restmengen vom Vortag übrig geblieben sind

1. Wählen Sie im Modul Fertigung > Kapazitätsplanung > Leitstand > Menü Funktionen > Restmengen anzeigen.

*Abb. H-109 Restmengen anzeigen und fertig melden*

- **A** Mindeststatus auswählen
- **B** Auftrag komplett fertig melden

Eine Beschreibung des Dialogs finden Sie in der Softwarereferenz.
⇨ Softwarereferenz, “Restmengen anzeigen" auf Seite H-377
2. Wählen Sie den Mindest-Status (A).
Die Aufträge müssen mindestens in die Kapazitätsplanung eingelastet sein. Ein niedrigerer Status ist daher nicht sinnvoll.
3. Markieren Sie die Checkboxen fertig melden (B) aller Aufträge, die nicht fertig gemeldet wurden, aber vollständig gefertigt sind.
4. Klicken Sie auf [OK], um die Daten zu speichern.
Der Status der Aufträge wird umgesetzt. Die fertig gemeldeten Aufträge werden aus der Übersicht gelöscht.

Sie können im Dialog Leitstand (Auftrag) prüfen, ob die Daten korrekt umgesetzt wurden. Alle nachgeholten Fertigmeldungen werden auf das aktuelle Tagesdatum gesetzt.

*Abb. H-110 Nachgeholte Fertigmeldungen*

Eine Beschreibung des Dialogs finden Sie in der Softwarereferenz.
⇨ Softwarereferenz, "Leitstand (Auftrag)" auf Seite H-378

> **i Anzeige fertiger Aufträge**
> Sie können in den Einstellungen zum Leitstand angeben, dass fertig gemeldete Aufträge nicht angezeigt werden sollen. Bei der Wahl dieser Option können Sie die Statusumsetzung nicht wie in dem Beispiel prüfen.

### Übungen

- Melden Sie einen Ihrer Aufträge manuell komplett fertig.
- Melden Sie in einem Ihrer Aufträge eine Position fertig.
- Erfassen Sie zu einer ISO-Scheibe eine Bruchmeldung. Beachten Sie dabei, dass die Position oder der Auftrag zuvor fertig gemeldet sein muss.
- Melden Sie die Restmengen von Vortag fertig. Diese Übung können Sie nur ausführen, wenn Restmengen vorhanden sind.

### Ergänzende Informationen

⇨ Softwarereferenz, "Produktionsbereich" auf Seite H-206
⇨ Softwarereferenz, "Restmengenübertragung" auf Seite H-296
⇨ Softwarereferenz, "Datum" auf Seite H-308
⇨ Softwarereferenz, "Manuelle Fertigmeldung" auf Seite H-314
⇨ Softwarereferenz, "Fertigungsstand Auftrag" auf Seite H-323
⇨ Softwarereferenz, "Übersicht Rückmeldungen" auf Seite H-334
⇨ Softwarereferenz, "Auslastung zu Datum" auf Seite H-367
⇨ Softwarereferenz, "Restmengen anzeigen" auf Seite H-377

## Produktionskosten

### Lernziele

- Maschinen- und Zeitkosten im Auftrag oder Angebot prüfen.

### Nutzen

- Schon vor der Produktion eines Auftrags kann festgestellt werden, ob in der Preisgestaltung die Zeit- und Maschinenkosten im Auftrag ausreichend berücksichtigt sind.

### Merke

**Produktionskosten**
Das sind:
- Lohnkosten pro Einheit
- Maschinenkosten pro Stunde
- Variable Kosten pro Stunde, z. B. für Versicherungen
Diese Kosten werden pro Maschine hinterlegt und bei der Einlastung geprüft.

**Produktionskosten im Angebot**
Um die Produktionskosten für ein Angebot zu ermitteln, muss ein Workflow-Task eingerichtet sein, der die Angebote an die Kapazitätsplanung übergibt.

**Tatsächliche Kosten**
Erst in der Produktion werden die tatsächlichen Kosten ermittelt, denn erst dann ist entschieden, welche Maschinen eingesetzt worden sind. Diese tatsächlichen Kosten werden mit den Rückmeldungen in den Auftrag zurückgeschrieben.

## Zeitkosten

Die Zeitkosten für Aufträge und ggf. für Angebote werden vom Programm errechnet. So können Sie vor der Fertigung prüfen, ob der Auftragswert bei den voraussichtlichen Zeitkosten noch gedeckt ist.

Die Kalkulation der Produktionskosten basiert auf folgenden Vorgaben:
- Maschinenkosten pro Stunde
- Variable Kosten pro Stunde, z. B. Versicherungskosten
- Kosten pro Vorgabezeiteinheit, z. B. Lohnkosten pro Einheit

Diese Kosten werden pro Maschine hinterlegt und bei der Einlastung geprüft.

*Abb. H-111 Zusammensetzung der Kosten für eine Maschine*

- **A** Kostensätze
- **B** Gesamtkosten pro gefertigter Einheit

Die bei der Planung errechneten Werte für eine Auftragsposition und den gesamten Auftrag werden nach der Fertigmeldung erneut berechnet. Sie können sich dann vom ursprünglichen Wert unterscheiden, z. B., weil die Fertigung an einer anderen Maschine ausgeführt wurde als ursprünglich geplant.

Im Dialog Fertigungsstand Auftrag können Sie sich die aktuellen Produktionskosten anzeigen lassen.

*Abb. H-112 Aktuelle Produktionskosten prüfen*

- **A** Geplante Produktionskosten für den gesamten Auftrag
- **B** Bisher tatsächlich angefallene Produktionskosten

## Kostenstellen

Sie können für die Analyse der Produktionskosten eigene Kostenstellen einrichten. Damit können Sie die Kosten über definierbare Zeiträume auswerten.

*Abb. H-113 Kostenstellen für Produktionskosten auswerten*

- **A** Sortierung nach Produktionsbereich - AV-Bereich oder AV-Bereich - Produktionsbereich
- **B** Auswertung der Produktarten, Produktgruppen oder Produkte

In dieser Auswertung werden die Kostenstellen für Produktarten aufgeführt. Sie können die Auswertung nach Kostenstellen oder nach AV-Bereichen sortiert anzeigen lassen.

Die Kostenstellen und die Auswertung können Sie nach den Anforderungen in Ihrem Betrieb einrichten. In den folgenden Beispielen soll die letzte Zeile mit der Auswertung Kostenstelle ESG bearbeitet näher erklärt werden.

> **i Kostenstellen in A+W Business Pro-Stammdaten**
> Die Kostenstellen der Kapazitätsplanung haben keine Verbindung zu den Kostenstellen, die Sie im Modul Stammdaten einrichten.

### Prinzip der Auswertungsspalten

In den Spalten wird jeweils festgelegt, was die Abfrage auswerten soll.

*Abb. H-114 Kostenstellen definieren*

- **A** Hauptproduktart: Nummer der Produktart aus den A+W Business Pro-Stammdaten
- **B** Nr 1, Nr 2: Nummer der Produktgruppe oder Produktart im Feld Typ
- **C** Тур 1, Тур 2:
    - 0 = Keine Vorgabe
    - 1 = Produktart
    - 2 = Produktgruppe
- **D** Priorität (Reihenfolge der Abfrage)
- **E** Produkte, die von der Auswertung ausgeschlossen sind

Mit der Kombination der Spalten Nr und Typ stellen Sie ein, was in der Stückliste gesucht werden soll.

**Beispiel: Auswertung von ESG bearbeitet**

| HPA | Nr 1 | Nr 2 | Typ 1 | Typ 2 | Priorität |
| :-- | :--- | :--- | :---- | :---- | :-------- |
| 2   | 20   | 0    | 1     | 0     | 19        |

- **Hauptprodukt:** ESG
- **Produktart:** Bearbeitungen
- **Typ 1:** Produktart

In diesem Beispiel sehen Sie, dass im Hauptprodukt der Produktart ESG (2) nach dem Typ1 (also Produktart) mit der Nummer 20 (Bearbeitungen) gesucht werden soll. Das bedeutet, dass in diese Kostenstelle nur ESG mit Bearbeitungen einfließen soll.

Bevor Sie mit dem Anlegen von Kostenstellen beginnen, sollten Sie sich überlegen, in welcher Reihenfolge die Kostenstellen abgefragt werden sollen. Diese Reihenfolge wird in der Spalte Priorität festgelegt.

**Beispiel ESG**
Sie fragen erst ab, ob es sich um ein ESG mit Bearbeitung handelt (Kostenstelle Nr. 7 mit Prio 19).
Wenn dies nicht der Fall ist, kommt die Folge-Abfrage, also Prio 20.
Das ESG, das nicht bearbeitet ist, fließt automatisch in die Kostenstelle ESG (Kostenstelle Nr. 6 mit Prio 20).

In der Spalte Ausschluss können Sie ein Produkt von der Regel ausschließen, indem Sie die Produktnummer eintragen. Die Produktnummer muss in Klammern stehen.

**Beispiel**
Alle ESG-Scheiben werden gesäumt. Deshalb möchten Sie nicht, dass die gesäumten ESG-Scheiben in die Kostenstelle ESG mit Bearbeitung einfließen.
Dies können Sie ausschließen, indem Sie die Produktnummer für Säumen eintragen.

Eine ausführliche Beschreibung zur Definition der Spalten finden Sie im Part Fertigung. Dort wird die Definition der Vorschauspalten beschrieben, die nach demselben Prinzip festgelegt werden.
⇨ Fertigung, "Prinzip der Vorschauspalten" auf Seite E-161

### Kostenkalkulation im Auftrag

Die Materialpreise werden in A+W Business Pro aufgrund der Einkaufspreise kalkuliert. Daneben können aber auch die Zeit- und Maschinenkosten im Auftrag eingesehen werden.

Diese Kosten werden pro Auftrag in der Kapazitätsplanung während der Einlastung ermittelt und im Auftrag angezeigt.

Die Material- und Zeitkosten werden im Auftragskopf im Register Summen angezeigt.

*Abb. H-115 Kostenkalkulation: Auftrag – Register Summen*

Die Kosten werden im Auftragskopf über das Menü Funktionen > Gruppe Kalkulation > Kosten- und Aufschlagskalkulation angezeigt.

*Abb. H-116 Kostenkalkulation im Auftrag*

### Kostenkalkulation für Angebote

Angebote können mit einem eigenen Workflow-Task an die Kapazitätsplanung übergeben werden, um die Kosten zu berechnen. Mit dieser Funktion können die Kosten im Angebotskopf und in der Positionserfassung genauso angezeigt werden wie im Auftrag. Die Angebote werden dabei nicht in die Kapazitätsplanung eingelastet und nicht an die Produktion übergeben.

### Übungen

- Prüfen Sie in den Aufträgen, die Sie an die Kapazitätsplanung übergeben haben, ob die Maschinenkosten angezeigt werden.
- Wenn Kosten fehlen: Prüfen Sie, ob Sie in den Aggregaten die Kosten eingetragen haben. Holen Sie dies ggf. nach und lasten Sie die Aufträge erneut ein. Prüfen Sie dann, ob die Kosten angezeigt werden.

### Ergänzende Informationen

⇨ Softwarereferenz, "Konten" auf Seite H-277
⇨ Softwarereferenz, "Kostenstellen-Definitionen" auf Seite H-279

## Leitstand

### Lernziele

- Navigation im Dialog Leitstand.
- Auslastung der Maschinen prüfen.
- Aufträge oder Auftragspositionen umlasten.

### Nutzen

- Im Dialog Leitstand erhalten Sie einen Überblick über die Auslastung der Aggregate.
- Über diesen Dialog können Sie alle Programme zum Prüfen und Umlasten der Aufträge erreichen.

### Merke

**Leitstand**
Vom Dialog Leitstand aus können Sie alle Dialoge zum Prüfen und Umlasten aufrufen.

### Konzept des Leitstands

Im Dialog Leitstand erhalten Sie eine Übersicht über die verplanten Stunden pro Aggregat und können im Bedarfsfall Termine verschieben.

*Abb. H-117 Planzeiten im Leitstand*

- **A** Verplante Zeit für Zuschnitt
- **B** Aggregate, an denen die Zeit verplant ist.
- **C** Aufträge, die an den Aggregaten gearbeitet werden sollen.

In diesem Beispiel sehen Sie die Auslastung des Produktionsbereichs Zuschnitt (A) für eine Woche. Die Detaildaten für die einzelnen Aggregate des Produktionsbereichs Zuschnitt (B) und die Aufträge (C), die an einem bestimmten Aggregat beteiligt sind, können Sie sich ebenfalls im Dialog Leitstand anzeigen lassen.

Über den Dialog Leitstand können Sie alle Programme zum Prüfen und Umlasten der Aufträge erreichen. Dies sind im Einzelnen folgende Dialoge:

- **Über Menü Funktionen:**
    - Auftrag auswählen > Leitstand (Auftrag)
    - Restmengen anzeigen > Restmengen
    - Grafik > Grafische Darstellung der Auslastung
    - Auslastung > Auslastung zum Datum
- **Über Leitstand > Register Vorprozesse:**
    - [im Detail] > Produktionslisten
- **Über Leitstand (Auftrag) > Menü Funktionen:**
    - Übersicht Rückmeldungen
    - Einlasten > Einlasten Auftrag
    - Manuelle Vorgabe > Fertigungsstand Auftrag

Im Dialog Leitstand navigieren Sie auf folgende Weise:

| Register | Aktion | Register / Dialog |
| :--- | :--- | :--- |
| **Bereiche** | Doppelklick auf Zeilenkopf | -> Aggregate (alle Aggregate) |
| | Doppelklick auf Produktionsbereich | -> Aggregate (nur Aggregate im Produktionsbereich) |
| **Aggregate** | Doppelklick auf Aggregat | -> Aufträge |
| | Doppelklick auf Detaildaten | -> Auftrag umlasten |
| **Aufträge** | Doppelklick in Zeilenkopf | -> Leitstand (Aggregat) |
| | Doppelklick auf Nummer | -> Leitstand (Auftrag) |
| | Doppelklick auf Detaildaten | -> Position umlasten |
| **Auftrag umlasten** | Klick in Zeilenkopf | -> Position umlasten |
| | Klick auf [neu] oder [Vorprozesse] | -> Vorprozesse |
| **Position umlasten** | Kontext-Menü auf Vorgang (rechte Maustaste) | -> Rüstzeit löschen / Rüstzeit hinzufügen |
| **Arbeitsarten** | Klick in Zeilenkopf | -> Details |
| **Details** | Doppelklick auf Nummer | -> Leitstand (Auftrag) |
| **Vorprozesse** | Klick auf [im Detail] | -> Produktionslisten |

### Leitstand – Auftrag

Um die Einlastung eines einzelnen Auftrags zu prüfen, steht der Dialog Leitstand (Auftrag) zur Verfügung.
Sie erreichen den Dialog über Leitstand > Menü Funktionen > Auftrag auswählen.

*Abb. H-118 Leitstand für einzelnen Auftrag*

- **A** Liefertermin
- **B** Versandtag

In diesem Beispiel sehen Sie, wie die Terminierung vom Liefertermin aus rückwärts gerechnet wird: Ein Tag vor dem Liefertermin muss der Auftrag den Produktionsbereich Versand erreichen und verpackt werden. Alle anderen Arbeiten finden unter Berücksichtigung der Produktions- und Übergangszeiten entsprechend früher statt.

Im Dialog Leitstand – Auftrag navigieren Sie auf folgende Weise:

| Register | Aktion | Register / Dialog |
| :--- | :--- | :--- |
| **Aggregate** | Doppelklick auf Aggregat | -> Verschieben II |
| | Doppelklick auf Datum | -> Detail |
| **Detail** | Klick auf Zellenkopf | -> Arbeitsarten |

### Leitstand – Aggregat

Um die Auslastung eines einzelnen Aggregats zu prüfen, steht der Dialog Leitstand - Auftrag zur Verfügung.
Sie erreichen den Dialog über Leitstand > Register Aggregat > Doppelklick in Zeilenkopf.

*Abb. H-119 Leitstand für einzelnes Aggregat*

- **A** Aggregat
- **B** Benötigte Stunden

In diesem Beispiel sehen Sie die Aufträge mit den Stückzahlen und den benötigten Zeiten an dem ausgewählten Aggregat. Der angezeigte Zeitraum entspricht der Anzeige im Dialog Leitstand, vom dem aus Sie diesen Dialog geöffnet haben.

Im nächsten Register können Sie sich die Zeiten detailliert anzeigen lassen. Dazu können Sie den angezeigten Zeitraum dann so ändern, dass Sie die Auslastung z. B. nur noch für einen Tag sehen.

Die durch ein Splitting erzeugten Pakete werden einzeln aufgeführt. Um eine Einlastung zu verschieben, können Sie mit einem Doppelklick auf die Auftragsnummer in den Dialog Leitstand (Auftrag) wechseln.

### Einlastung für einzelnen Auftrag verschieben

Sie möchten prüfen, ob der Versand für einen Auftrag verschoben werden kann, z. B., weil sich die Lieferung der Bestellteile verzögert.

In diesem Beispiel soll die Auslieferung eines Auftrags um mehrere Tage verschoben werden. Das bedeutet, dass sowohl der Liefertermin als auch die Einlastung geändert werden sollen.

#### So prüfen Sie die Einlastung eines Auftrags

1. Wählen Sie Modul Fertigung > Kapazitätsplanung > Leitstand > Menü Funktionen > Auftrag auswählen.
Der Dialog Leitstand - Auftrag wird geöffnet.
2. Tragen Sie die Auftragsnummer ein.
3. Wählen Sie im Menü Start > Suchen, um die Daten einzulesen.

*Abb. H-120 Plandaten des aktuellen Auftrags*

- **A** Aktueller Liefertermin
- **B** Versand: Fertigstellung ein Tag vor Liefertermin

Eine Beschreibung des Dialogs finden Sie in der Softwarereferenz.
⇨ Softwarereferenz, "Leitstand (Dialog)" auf Seite H-342
4. Tragen Sie im Feld Liefertermin den neuen Termin ein (B).
5. Klicken Sie auf [Ändern].
Die Anzeige wird erst beim nächsten Öffnen des Dialogs aktualisiert.
6. Wählen Sie im Menü Funktionen > Einlasten.

*Abb. H-121 Auftrag zum neuen Liefertermin einlasten*

Eine Beschreibung des Dialogs finden Sie in der Softwarereferenz.
⇨ Softwarereferenz, "Einlasten Auftrag" auf Seite H-289
Der Auftrag wird mit dem neuen Liefertermin angezeigt. Er ist aber noch nicht zu diesem Termin eingelastet. Dies können Sie prüfen, indem Sie über die Schaltfläche [Ergebnis] den Dialog Einlastungsergebnis öffnen.

*Abb. H-122 Alte Einlastung*

Sie sehen in diesem Beispiel, dass der Versand zum alten Termin angezeigt wird. Wenn Sie den Dialog geschlossen haben, wird die Einlastung fortgesetzt.
7. Wählen Sie im Menü Start > Ausführen, um den Auftrag erneut einzulasten.
Die Einlastung beginnt. Je nach Einstellung müssen Sie den Liefertermin für die einzelnen Positionen bestätigen. Nach der erfolgreichen Einlastung können Sie sich das Ergebnis erneut anzeigen lassen.

*Abb. H-123 Neue Einlastung*

Sie sehen in diesem Beispiel, dass der Versand zum neuen Termin angezeigt wird. Alle Arbeitsschritte an den vorgelagerten Aggregaten sind entsprechend verschoben.
8. Wechseln Sie zum Dialog Leitstand (Auftrag) zurück.
Um die Anzeige zu aktualisieren, müssen Sie den Auftrag neu einlesen.
9. Wählen Sie dazu im Menü Start > Filter, um in den Such-Modus zu wechseln.
10. Tragen Sie die Auftragsnummer wieder ein und starten Sie die Suche, um den Auftrag einzulesen.

*Abb. H-124 Geänderte Plandaten des Auftrags*

- **A** Neuer Liefertermin
- **B** Versand: Fertigstellung ein Tag vor Liefertermin

### Aggregat ändern

Sie können die Einlastung von Auftragspositionen auf ein anderes Aggregat verschieben, z. B. von der ISO-Linie I auf die ISO-Linie II.

#### So lasten Sie eine Auftragsposition auf ein anderes Aggregat um

1. Wählen Sie im Modul Fertigung > Kapazitätsplanung > Leitstand > Menü Funktionen > Auftrag auswählen.
Der Dialog Leitstand (Auftrag) wird geöffnet.
2. Tragen Sie die Auftragsnummer ein und starten Sie die Suche.
Die Auftragsdaten werden eingelesen.

*Abb. H-125 Plandaten des aktuellen Auftrags*

3. Klicken Sie doppelt auf das Aggregat, um den Leitstand für das Aggregat zu öffnen.
Der Dialog Leitstand (Aggregat) wird mit dem Register Verschieben II angezeigt.
4. Markieren Sie die Checkbox der Position, die an ein anderes Aggregat verschoben werden soll.
5. Wählen Sie im Bereich Verschieben ein anderes Aggregat aus.
Zusätzlich können Sie einen neuen Termin und/oder eine andere Schicht eintragen.
6. Über [Belegung] können Sie prüfen, ob die Verschiebung sinnvoll ist.

*Abb. H-126 Verschiebung prüfen*

7. Wählen Sie im Menü Start > Ausführen, um die Aktion zu starten.
Die Einlastung wird verschoben. Die Änderung wird nach dem Neustart des Dialogs angezeigt.

### Übungen

- **Navigation im Leitstand üben:**
Ausgangspunkt für die folgenden Übungen ist immer der Leitstand. Schließen Sie den aufgerufenen Dialog, um die nächste Übung auszuführen.
    - Lassen Sie sich die Aggregate zu einem Produktionsbereich anzeigen.
    - Wechseln Sie zum Dialog Leitstand (Aggregat).
    - Wechseln Sie zum Dialog Leitstand (Auftrag).
    - Lassen Sie sich die Daten im Register Im Detail anzeigen.

> **i Tipp zur Navigationsübung**
> Drucken Sie sich die Übersicht über die Navigation aus. Sie finden diese auch in der Softwarereferenz.
> ⇨ "Navigation durch die Register und Dialoge" auf Seite H-323

- Wechseln Sie aus dem Leitstand zu einem Auftrag und prüfen Sie die Einlastung.
- Verschieben Sie den Liefertermin eines Auftrags um eine Woche. Was müssen Sie noch tun? Wann werden Sie die neuen Termine angezeigt?
- Lasten Sie einen Auftrag mit 10 großen ISO-Scheiben so ein, dass nur eine Einheit pro Tag produziert wird (Positionssplit und Produktionstermin festlegen).

### Ergänzende Informationen

⇨ Softwarereferenz, “Leitstand (Dialog)" auf Seite H-342
⇨ Softwarereferenz, "Leitstand (Aggregat)" auf Seite H-360
⇨ Softwarereferenz, "Leitstand (Auftrag)" auf Seite H-378
⇨ Softwarereferenz, "Fertigungsstand Auftrag" auf Seite H-323
⇨ Softwarereferenz, "Produktions-Zeiten ändern" auf Seite H-335

# Softwarereferenz

## Übersicht

A+W Business Pro Capacity Planning gliedert sich in zwei Bereiche:
- Verwaltung der Kapazitätsplanung
- Planung und Überwachung der Kapazitäten

Die zugehörigen Dialoge finden Sie in den Modulen Kapazitätsplanung und Fertigung.

In dieser Softwarereferenz sind die Dialoge aus den beiden Modulen in folgenden Abschnitten beschrieben:
- "Verwaltung" auf Seite H-188
- "Kapazitätsplanung" auf Seite H-281

## Verwaltung

Um mit A+W Business Pro Capacity Planning arbeiten zu können, müssen die Stammdaten eingerichtet werden. Diese Daten bilden die Grundlage für alle weiteren Zuordnungen, Zeitplanungen und Auswertungen.

In diesem Kapitel finden Sie Informationen zu folgenden Stammdaten:
- "Voreinstellungen Firmendaten" auf Seite H-189
- "Allgemein" auf Seite H-195
- "Organisation" auf Seite H-205
- "Vorgabezeiten" auf Seite H-229

Neben der Beschreibung der Stammdaten finden Sie Informationen zu folgenden Themen:
- "Zuordnen" auf Seite H-242
- "Sperren" auf Seite H-259
- "Übersichten" auf Seite H-270
- "Einlastung" auf Seite H-282
- "Produktionsmeldungen" auf Seite H-307
- "Leitstand" auf Seite H-341

### Voreinstellungen Firmendaten

**Stammdaten > Firma > Firmendaten > Register Kapa-Planung**

*Abb. H-127 Firmendaten – Kapa-Planung*

Im Modul Stammdaten legen Sie die Grundeinstellungen für A+W Business Pro Capacity Planning fest. Diese Einstellungen beziehen sich vor allem auf die automatische Einlastung. Sie können bei einer manuellen Einlastung überschrieben werden.

> **i Einstellungen ändern**
> Wenn Sie die Einstellungen in den Firmendaten und in den Stammdaten der Kapazitätsplanung geändert haben, müssen Sie A+W Business Pro neu starten, damit die Daten neu eingelesen werden.

#### Kapazitätsplanung

**Version** Bei der Wahl des Programms zur Kapazitätsplanung müssen Sie darauf achten, wie Sie Rückmeldungen aus der Produktion empfangen. Wenn Sie mit A+W Business Pro Capacity Planning arbeiten wollen, müssen Sie den Eintrag A+W Business Kapazitätsplanung auswählen.
Mit dieser Einstellung können Sie die Online-Meldungen nicht nutzen.

**Fehlermeldung aus autom. Kapazitätsplanung**
Mit der Wahl der Option legen Sie fest, an wen Fehlermeldungen gesendet werden.
- **An Auftragserfasser:**
Mit dieser Einstellung werden die Fehlermeldungen an den Mitarbeiter gesendet, der den jeweiligen Auftrag erfasst hat. Solche Fehlermeldungen beziehen sich in aller Regel auf Termine, die nicht eingehalten werden können, weil nicht genügend Kapazitäten zur Verfügung stehen. Dies ist die Standard-Einstellung.
- **An Mitarbeiter:**
Mit dieser Einstellung wird das Feld für die Auswahl eines Mitarbeiters freigeschaltet. Wählen Sie diese Option, wenn nur ein einziger Mitarbeiter die Aufträge bearbeitet, die nicht problemlos eingelastet werden konnten.

> **i Aufträge automatisch einlasten**
> In der Regel werden die Aufträge durch einen Workflow-Task automatisch in festgelegten Intervallen in die Kapazitätsplanung eingelastet. Diese Funktion ist im Tutorial beschrieben.

#### A+W Business-Kapazitätsplanung

**Schichtenzahl** Anzahl der Schichten, in denen Sie arbeiten. Die Schichtzeiten legen Sie im Modul Kapazitätsplanung im Dialog Kalender fest.
⇨"Kalender" auf Seite H-217

**Fertigungsterminmodus** Angabe, ob Sie mit offenen oder geschlossenen Kapazitäten arbeiten wollen.
- **Automatisch Normalkapazität:**
Die Aufträge werden entsprechend der zur Verfügung stehenden Schichtzeiten eingelastet. Die Überbuchung ist nicht möglich. Dies ist die Standard-Einstellung (geschlossene Kapazitäten).
- **Automatisch volle Tage:**
Bei dieser Einstellung werden die Angaben im Kalender für die Anzahl Schichten und Stunden ignoriert. Die Einlastung geht dann von einem Arbeitstag mit 24 Stunden aus (offene Kapazitäten). Dies gilt jedoch nur für reguläre Arbeitstage, nicht für Feiertage.
- **Nur Aggregatwechsel:**
Bei ausgelasteten Kapazitäten soll automatisch nur nach einem anderen Aggregat gesucht werden. Wenn das ebenfalls ausgelastet ist, wird die Einlastung unterbrochen und Sie müssen manuell eingreifen.
- **Einlasten ohne Kontrolle:**
Diese Einstellung entspricht der offenen Schicht. Das heißt z. B., dass trotz der Schichtzeit von 8 Std. auch 16 Std. eingelastet werden können. Dabei wird keine Meldung ausgegeben, wenn ein Tag voll ausgelastet ist.

**Schichtfüllung bei Positionssplit** Große Positionen können auf mehrere Aggregate, Schichten oder Tage verteilt werden. Dazu geben Sie an, zu wie viel Prozent die Schicht(en) eines Aggregats durch das Splitting gefüllt werden dürfen, um Platz für andere Aufträge zu behalten.

**Aggregatabgleich** Wenn Sie mit mehreren Maschinen arbeiten, die dieselben Arbeitsarten ausführen können, kann die Planung diese Maschinen auf unterschiedliche Weise berücksichtigen:
- **Automatisch:**
Das Programm sucht automatisch nach der kosten- und zeitgünstigsten Maschine und lastet die Aufträge dort ein. Dies ist die Standard-Einstellung.
- **Semi-automatisch:**
Das Programm bietet die alternativen Maschinen zur Auswahl an. Wenn der Liefertermin nicht eingehalten werden kann, müssen Sie eingreifen.
- **Manuell:**
Mit dieser Option müssen Sie bei jedem möglichen Wechsel (Maschine, Schicht usw.) manuell eingreifen. Alternative Maschinen können nur bei der manuellen Ein- oder Umlastung ausgewählt werden.

**Einlastpriorität** Die Prioritäten aus dem Auftrag können beim Einlasten berücksichtigt werden:
- **Standard:**
Die Kapazitäten der benötigten Aggregate werden geprüft und die Aufträge werden entsprechend der eingetragenen Priorität eingelastet.
- **Niedrige Priorität:**
Standardmäßig werden alle Aufträge mit niedriger Priorität eingelastet.
- **Geänderte Priorität in Auftrag übernehmen:**
Wenn die Priorität beim Einlasten geändert wird, soll sie automatisch in den Auftrag zurückgeschrieben werden.

**Max. Verschiebung bei autom. Lieferterminbestimmung (Tage)** Sie können festlegen, wie viele Tage in die Zukunft der Liefertermin automatisch verschoben werden darf.

**Einlastung von Bestellpositionen (Nur Hauptprodukte)** Mit der A+W Business Kapazitätsplanung können Bestellpositionen aus dem Hauptartikel eingelastet werden.
- Bestellpositionen werden nicht eingelastet.
- Die Bestellpositionen werden eingelastet. Die Zeitkosten für die Positionen können bestimmt werden.

**Einlastung von Lagerpositionen (Nur Hauptprodukte)** Mit der A+W Business Kapazitätsplanung können Lagerpositionen aus dem Hauptartikel eingelastet werden.
- Lagerpositionen werden nicht eingelastet.
- Die Lagerpositionen werden eingelastet. Die Zeitkosten für die Positionen können bestimmt werden.

**Einlastung von manuell erfassten Leistungspositionen (Nur Hauptprodukte)** Mit der A+W Business Kapazitätsplanung können manuell erfasste Leistungspositionen aus dem Hauptartikel eingelastet werden.
- Manuell erfasste Leistungspositionen werden nicht eingelastet.
- Die manuell erfassten Leistungspositionen werden eingelastet. Die Zeitkosten für die Positionen können bestimmt werden.

**Historientabelle für Fertigmeldungen füllen** Fertigmeldungen können in die Historie geschrieben werden.
- Fertigmeldungen werden nicht in die Historie geschrieben.
- Die Fertigmeldungen werden in die Historie geschrieben. Zusätzlich werden Arbeitsgänge protokolliert, die die durch eine Buchung fertiggemeldet sind. STSD-Rückmeldungen werden protokolliert, wenn keine Buchung in die Kapazitätsplanung erfolgt.
Die Historie kann im Modul Statistik ausgewertet und ausgedruckt werden.

**Automatische Lieferterminsuche nach Tour** Bei Engpässen kann automatisch nach einem neuen Liefertermin gesucht werden.
- Der nächstmögliche Termin wird als Liefertermin gewählt, unabhängig davon, ob es ein Tourentag ist oder nicht. Dies ist die Standard-Einstellung.
- Der neue Liefertermin wird nach den Tourentagen des Kunden gesucht.

**Auftrag nicht splitten** Große Aufträge müssen in kleinere Positionen aufgeteilt werden, wenn der Arbeitsgang nicht für eine Position insgesamt an einem Tag erledigt werden kann.
- Die Aufträge können bei der automatischen Einlastung gesplittet werden. Dies ist die Standard-Einstellung.
- Die Aufträge können nur manuell gesplittet werden. Bei der automatischen Einlastung großer Aufträge wird eine Meldung angezeigt, so dass Sie eingreifen können.

**Verkürzte Einlastprüfung bei gleichem Aufbau** In einem Auftrag können Positionen mit gleichem Stücklistenaufbau enthalten sein, die sich nur durch die Maße unterscheiden.
- Bei jeder Position wird der gesamte Stücklistenaufbau geprüft.
- Bei gleichem Stücklistenaufbau wird von der Einlastung der vorigen Position ausgegangen, ohne die Stückliste neu zu prüfen. Dies ist die Standard-Einstellung.

**Zum Liefertermin einlasten** Bei der automatischen Einlastung werden Aufträge standardmäßig zum Liefertermin eingelastet. Nur wenn keine Kapazitäten frei sind, wird nach einem neuen Liefertermin gesucht.
- Aufträge werden mit Lieferterminsuche eingelastet. Dies ist die Standard-Einstellung.
- Die Aufträge werden ohne Suche nach einem alternativen Liefertermin eingelastet, unabhängig davon, ob Kapazitäten frei sind oder nicht.

**Automatische Fertigmeldung berechneter Aufträge** Zurzeit nicht genutzt.

**Produktionsübergabe (OrderXML) mit Planungsdaten** Für die Übergabe an die Produktion können die ermittelten Daten aus der Kapazitätsplanung in die OrderXML-Datei geschrieben werden.
- Die Daten aus der Kapazitätsplanung werden nicht in die OrderXML-Datei geschrieben.
- Die Maschinenzuordnung, Produktionsdatum und -schicht, Zeitkosten werden in die Übergabedatei geschrieben.

**Schichtwechseltabelle verwenden** Wenn Sie mit mehr als einer Schicht arbeiten, können Sie festlegen, wann die Einlastung von einer Schicht zur nächsten wechselt.
- Die Schichtwechseltabelle wird nicht verwendet.
- Die Schichtwechseltabelle wird verwendet. Wenn noch keine Schichtwechsel festgelegt sind, wird der Dialog Einstellungen Schichten geöffnet.
⇨ "Einstellungen Schichten" auf Seite H-193

**Produktgruppen ohne Statusänderung**
Sie können die Erhöhung des Positionsstatus (Auftragsstatus) durch Fertigmeldungen für Produktgruppen unterdrücken. Markieren Sie dazu die gewünschten Einträge in der Liste.

**AV-Bereiche ohne Einlastung**
⇨ Sie können festlegen, dass in bestimmte AV-Bereiche nicht automatisch eingelastet wird. Das bedeutet, dass Aufträge für die markierten AV-Bereiche nur manuell eingelastet werden können.

### Einstellungen Schichten

**Stammdaten > Firma > Firmendaten > Register Kapa-Planung > Schaltfläche Einstellungen neben Checkbox Schichtwechseltabelle verwenden**

*Abb. H-128 Stammdaten – Einstellungen Schichten*

In diesem Dialog legen Sie die Schichtwechsel und Sperrzeiten fest, in denen z. B. kein Auftrag eingelastet werden kann.

> **Voraussetzungen**
> Sie müssen Administratorrechte haben, um den Dialog zu öffnen. Zusätzlich muss in den Firmendaten die Checkbox Schichtwechseltabelle verwenden markiert sein.
> ⇨ "Schichtwechseltabelle verwenden" auf Seite H-193

#### Allgemein

Die Einstellungen in diesem Bereich werden aus den Firmendaten übernommen.
⇨ "A+W Business-Kapazitätsplanung" auf Seite H-190

**Schichtzahl** Anzahl der Schichten.

**Abgleichmodus** Modus, nach dem nach Aggregaten gesucht wird:
- **0 = Automatisch:**
Das Programm sucht automatisch nach der kosten- und zeitgünstigsten Maschine und lastet die Aufträge dort ein. Dies ist die Standard-Einstellung.
- **1 = Semi-automatisch:**
Das Programm bietet die alternativen Maschinen zur Auswahl an. Wenn der Liefertermin nicht eingehalten werden kann, müssen Sie eingreifen.
- **3 = Manuell:**
Mit dieser Einstellung müssen Sie bei jedem möglichen Wechsel (Maschine, Schicht usw.) manuell eingreifen. Alternative Maschinen können nur bei der manuellen Ein- oder Umlastung ausgewählt werden.

#### Optionen

**Beim Speichern Zeitentabellen korrigieren** Wenn Sie die Werte geändert haben, können die Zeiten der eingelasteten Aufträge überrechnet werden.
- Die neuen Zeiten verändern die aktuell eingelasteten Aufträge nicht.
- Die neuen Zeiten werden sofort übernommen. Alle eingelasteten Aufträge werden neu berechnet.

#### Schichtwechselzeiten

**Schicht 1 > Schicht 2, ...** Angabe, wann der Übergang von einer Schicht zur nächsten Schicht stattfindet. Diese Einstellung ist z. B. wichtig für die Berechnung von Übergangszeiten. Die Anzahl der angezeigten Felder hängt von der Anzahl der Schichten ab, die in den Firmendaten angegeben sind.
⇨ "A+W Business-Kapazitätsplanung" auf Seite H-190

#### Schichtsperrzeiten

**1., 2., ... Schicht** Angabe, ab wann die jeweilige Schicht für neue Aufträge gesperrt ist.

> **Beispiel: 2. Schicht 10:00**
> Bis 10 Uhr können Aufträge in die zweite Schicht des aktuellen Tages eingelastet werden. Damit halten Sie sich die 2. Schicht so frei, dass alle eingelasteten Aufträge tatsächlich gefertigt werden können und keine Restmengen entstehen.
> Aufträge, die nach 10 Uhr eingelastet werden, werden für die 3. Schicht oder den folgenden Tag geplant.

### Allgemein

**Kapazitätsplanung > Stammdaten > Allgemein**

In diesen Dialogen hinterlegen Sie Daten für die Arbeitsgänge und Maschinen, die in der Produktion zur Verfügung stehen.

In diesem Kapitel finden Sie Informationen zu folgenden Stammdaten:
- "Aggregattypen" auf Seite H-195
- "Arbeitsarten" auf Seite H-198
- "Zugeordnete Aggregate" auf Seite H-201
- "Serienfaktoren" auf Seite H-202
- "Übergangszeiten" auf Seite H-203

#### Aggregattypen

**Kapazitätsplanung > Stammdaten > Allgemein > Aggregattypen**

*Abb. H-129 Aggregattypen*

In diesem Dialog definieren Sie die Maschinentypen, die Sie in Ihrer Produktion einsetzen, z. B. Schneidtische, Bohrmaschinen, Schleifmaschinen, ESG-Öfen usw. Sie müssen zuerst die Maschinentypen definieren und festlegen, welche Restriktionen jeweils geprüft werden sollen.

Mit einem Doppelklick in den Zeilenkopf öffnen Sie den Dialog Zugeordnete Aggregate.
⇨ "Zugeordnete Aggregate" auf Seite H-201

Durch das Aktivieren der Checkboxen werden die entsprechenden Felder im Dialog Aggregate freigeschaltet.
⇨ "Aggregate" auf Seite H-207

> **i Achtung bei nachträglicher Aktivierung**
> Wenn Sie eine Checkbox nachträglich aktivieren, müssen Sie alle Aggregate prüfen, die zu dem geänderten Aggregattyp gehören. Die neu freigeschalteten Felder sind standardmäßig leer. Das kann bei der Prüfung Fehler verursachen.

**Nr.** Frei wählbare Nummer, die als ID für die einzelnen Maschinentypen dient.

**Bezeichnung** Name des Maschinentyps.

> **i Einstellungen**
> Im Folgenden wird jeweils die Funktion der aktivierten Checkbox genannt. Eine ausführliche Beschreibung der Funktion finden Sie im Dialog Aggregate mit der Beschreibung der einzelnen Einstellungen.
> ⇨ "Aggregate" auf Seite H-207

**Maschinentyp** Die Auswahl des Maschinentyps steht nur in A+W Business Pro zur Verfügung. Für diese Programmversion sind die Maschinentypen fest vorgegeben. Der Maschinentyp bezieht sich auf die konkreten Maschinen und die zu verwendeten Treiber.
Die Auswahl legt fest, welche Maschinentreiber im Dialog Aggregate > Zusatz-Optionen zur Verfügung stehen. Mit diesen Treibern kann A+W Business Pro die Maschinen ansteuert.
Im Unterschied zum Aggregattypen kann dieser Typ nicht konfiguriert werden.

**Maß-Check** Die Größenrestriktionen müssen bei diesem Maschinentyp geprüft werden.

**SZR** Die SZR-Restriktionen müssen bei diesem Maschinentyp geprüft werden.

**Gesamtstärke** Die Gesamtdicke einer ISO- oder einer VSG-Einheit muss geprüft werden.

**Einzelstärke** Die Dicke eines einzelnen Einfachglases muss geprüft werden.

**Gewicht** Das Gewicht der Scheibe muss geprüft werden.

**Scheibenanzahl** Die Anzahl der Scheiben eines Produkts (2-fach, 3-fach-ISO oder VSG) muss geprüft werden.

**Fläche** Die Fläche der Scheibe muss geprüft werden.

**Gas** Die Position muss auf Gasfüllung überprüft werden.

**Kantenschutz** Der Kantenschutz muss bei Isoliergläsern geprüft werden.

**Modell** Die Position muss auf Modelle geprüft werden.

**Sprossen** Die Position muss auf Sprossen geprüft werden.

**Anzahl** In der Position muss die Menge oder der Mengenbereich geprüft werden.
Die Definition, um welche Anzahl es sich handelt, ist maschinenabhängig, z. B.
- Bohrmaschine = Anzahl Bohrlöcher
- Schleifmaschine = Anzahl der Kanten

**Seitenverhältnis** Das Seitenverhältnis der Scheibe muss geprüft werden.

**Drehbar** Bei jedem Glas muss geprüft werden, ob es gedreht werden darf.

**Bohrdurchmesser** Der Durchmesser einer Bohrung muss geprüft werden.

**Eckradius** Der Radius von gerundeten Ecken muss geprüft werden.

**Diagonale** Diagonale zwischen den Rollen, z. B. auf dem Förderband vor dem ESG-Ofen, muss geprüft werden.

**Gehrungswinkel** Min. und max. Gehrungswinkel für Facetten muss geprüft werden.

#### Arbeitsarten

**Kapazitätsplanung > Stammdaten > Allgemein > Arbeitsarten**

*Abb. H-130 Arbeitsarten*

In diesem Dialog hinterlegen Sie die Arbeitsarten. Das sind alle Tätigkeiten, für die Zeiten benötigt werden, also z. B. Zuschnitt, manueller Zuschnitt, Kanten säumen, Kanten polieren, VSG sägen, verpacken.

In einem Arbeitsprozess können mehreren Arbeitsarten nacheinander ausgeführt werden, z. B. für die ESG-Fertigung der Zuschnitt und das Härten. Sie müssen also entscheiden, ob Sie die einzelnen Schritte jeweils als eine Arbeitsart anlegen oder den gesamten Arbeitsprozess. Je nach der Organisation in Ihrem Betrieb kann es auch sinnvoll sein, beide Formen zu wählen.
⇨Tutorial, "Arbeitsarten" auf Seite H-30

> **i Arbeitsarten scannen**
> Wenn Sie mit einer Betriebsdatenerfassung (BDE) arbeiten, müssen Sie alle Arbeitsarten anlegen, die mit dem Scanner erfasst werden können. Nur dann können Sie auch die Rückmeldungen für den Status auswerten.

**Menü Funktionen**
Über dieses Menü können Sie sich eine Übersicht über die Maschinen anzeigen lassen, die der markierten Arbeitsart zugeordnet sind.
⇨ "Zugeordnete Aggregate" auf Seite H-201

**Nr.** Frei wählbare Nummer, die als ID für die einzelnen Arbeitsarten dient. Wir empfehlen, die Nummern in Zehnersprüngen anzugeben, so dass Platz zum Einfügen neuer Arbeitsarten bleibt. Damit können Sie ähnliche Arbeitsarten zusammenhalten. Außerdem sollten die Arbeitsarten in der Reihenfolge nummeriert sein, in der sie im Fertigungsprozess aufeinander folgen.

**Bezeichnung** Name der Arbeitsart. Als Arbeitsart kann auch ein Zuschlag definiert werden, der die Maschinenzeit z. B. beim Zuschneiden von Modellen verlängert.

**Sequenz** Reihenfolge der Bearbeitung. Die Ziffer entscheidet, wann die Bearbeitung ausgeführt wird. Die Sequenz gibt die Priorität (Produktionsreihenfolge) der einzelnen Arbeitsarten innerhalb der Kapazitätsplanung an.

> **Beispiel**
> Kanten müssen vor dem Lochbohren geschliffen werden.
> VSG-Vorverbund nach dem Bohren.
> Daraus folgt, dass die Sequenz für den Kantenschliff kleiner, für den VSG-Vorverbund größer ist als für die Lochbohrung.

Sie sollten bei der Zuordnung der Ziffern mindestens in 10er-Schritten, besser noch in 50er oder 100er-Schritten arbeiten, damit Sie genug Spielraum für neue Arbeitsarten haben.

**Nur Hauptprodukt** Einige Arbeitsarten sind nur beim Hauptprodukt sinnvoll, jedoch nicht für die Stücklistenelemente.
- Diese Arbeitsart kann sowohl beim Hauptprodukt als auch bei den Stücklisten-Komponenten angewendet werden.
- Diese Arbeitsart gilt nur für das Hauptprodukt, z. B. ist der Versand für Stücklisten-Komponenten nicht möglich.

**AWProd.Nr** Artikelnummer aus A+W Production. Arbeitsarten, die Bestandteil eines Auftrages bei einem Glasproduzenten sind, jedoch im Auftrag selbst nicht extra spezifiziert werden, benötigen eine A+W Production-Artikelnummer, z. B. Zuschnitt.
Für diese Artikelnummer muss in A+W Business Pro ein Produkt der Produktart/Produktgruppe Bearbeitungen mit derselben Nummer angelegt werden.

**% Limit** Die Kapazitätsplanung lastet standardmäßig einen Auftrag so ein, dass dieser zeitnah zum Liefertermin gefertigt wird. Bei großen Aufträgen kann dies zu Problemen führen. Der Prozentwert legt fest, wie groß der Anteil eines Auftrags an der Tageskapazität sein darf. Größere Aufträge werden dann über mehrere Tage verteilt.

> **Beispiel**
> Sie erhalten einen großen Auftrag am 17. Juli.
> Der Liefertermin ist der 22. September.
> Die Kapazitätsplanung würde diesen Auftrag so einplanen, dass er kurz vor Liefertermin gefertigt würde. Damit wäre aber die Produktion für z. B. vier komplette Tage durch diesen Auftrag blockiert. Andere Aufträge könnten in dieser Zeit nicht mehr eingelastet werden.
> Da Sie aber Zeit haben, den Auftrag verteilt über den gesamten Zeitraum bis zum Liefertermin zu fertigen, können Sie hier eintragen, dass die Arbeitsart pro Auftragsposition nur z. B. 10% der Tageskapazität beanspruchen darf.

Dieser Wert wird nur berücksichtig, wenn Sie die Option Pos. Control aktivieren. Diese Option finden Sie in folgenden Dialogen:
- "Einlasten NV" auf Seite H-283
- "Einlasten Auftrag" auf Seite H-289
- "Aggregate Ausfall" auf Seite H-303

**Manuelle Aggregatauswahl** Wenn Sie mehrere Maschinen haben, die die gleiche Arbeitsart ausführen können, legen Sie eine Maschine mit Priorität 9 in den Vorgabezeiten fest, damit sie standardmäßig ausgewählt wird. Wenn diese Maschine an einem Tag ausgelastet ist, kann auf eine der anderen Maschinen zugegriffen werden.
- Der Auftrag wird automatisch einer anderen Maschine zugeordnet. Wenn dabei jedoch der Produktionstag gewechselt wird, müssen Sie manuell eingreifen.
- Wenn die Kapazität einer Maschine überschritten wird, müssen Sie manuell eine andere Maschine auswählen. Die möglichen Ausweichmaschinen werden in einem Dialog angezeigt.

**Ausweich-Arbeitsart** Sie können einer Arbeitsart eine Ausweich-Arbeitsart zuzuordnen, z. B. für das Bohren von Sondergrößen.

> **Beispiel**
> Sie haben die beiden Arbeitsarten Bohren und Sondergrößen bohren.
> In der Arbeitsart Bohren wird die Ausweicharbeitsart Sondergrößen bohren eingetragen.
> Der Standard-Bohrmaschine wird die Arbeitsart Bohren zugewiesen. Diese kann jedoch nur beschränkte Bohrdurchmesser bohren. Wenn diese Abmessungen überschritten werden, dann prüft die Kapazitätsplanung, ob eine Ausweich-Arbeitsart eingetragen ist.
> Wenn ja, sucht das Programm nach einer zugeordneten Maschine.

#### Zugeordnete Aggregate

**Kapazitätsplanung > Stammdaten > Allgemein > Arbeitsarten > Menü Funktionen > Zugeordnete Aggregate**

*Abb. H-131 Zugeordnete Aggregate*

In diesem Dialog werden die Maschinen aufgelistet, die einem Aggregattyp oder einer Arbeitsart zugeordnet sind. Im Infobereich des Dialogs wird angezeigt, aus welchem Dialog heraus Sie die Übersicht geöffnet haben.

**Aggregat** Name der Maschine, die zugeordnet ist.

**Bemerkung** In dieser Spalte wird bei Arbeitsarten angezeigt, ob die Arbeitsart für die zugeordnete Maschine als Basiszeit oder als Zeitzuschlag ausgewertet wird.

**Prio** Priorität, mit der das Aggregat beim Einlasten automatisch ausgewählt wird.
- **9:** höchste Priorität (Standard-Maschine). Diese Maschinen werden immer zuerst ausgelastet.
- **8 bis 1:** absteigende Priorität. Diese Maschinen werden je nach Auslastung ausgewählt.
- **0:** niedrigste Prioritäten. Diese Maschinen werden nur dann eingesetzt, wenn alle anderen (gleichartigen) Maschinen ausgelastet sind.
- **-1:** zur manuellen Einlastung. Diese Maschinen werden von der automatischen Einlastung nur bei Engpässen ausgewählt.
- **-2:** nur zur manuellen Einlastung. Diese Maschinen werden nie von der automatischen Einlastung ausgewählt. Die Maschine kann nur manuell ausgewählt werden.
- **-3:** wird nur bei der Rückmeldung vom Produktionssystem ausgewählt, wenn dort umgelastet wurde. Bei Umlasten in der Kapazitätsplanung werden nur noch Aggregate mit Prio > -3 angezeigt.

#### Serienfaktoren

**Kapazitätsplanung > Stammdaten > Allgemein > Serienfaktoren**

*Abb. H-132 Serienfaktoren*

In diesem Dialog legen Sie fest, bei welchen Stückzahlen die geplanten Zeiten reduziert werden, z. B., weil das Rüsten beim Schleifen oder Bohren entfällt.

Die Nummer der Serientabelle ordnen Sie der Maschine im Dialog Aggregate zu.
"Serientabelle" auf Seite H-212

**Identifikation**
**Nummer** Die Nummer wird automatisch vergeben, wenn Sie eine neue Serientabelle anlegen.
**Bezeichnung** Name der Serientabelle. Geben Sie einen sprechenden Namen ein, wenn Sie mehrere Tabellen anlegen, z. B. für Bohren oder Schleifen.

**Serientabellen**
**Ab Stück** Menge, ab der ein Faktor berücksichtigt werden soll.

**Faktor** Faktor, mit dem die Basiszeit für den Arbeitsgang multipliziert wird.

> **Beispiel**
> 
> | Ab Stück | Faktor pro Stück | Zeit an der Maschine |
> | :--- | :--- | :--- |
> | 1 | 1 | 0,10 Std. |
> | 10 | 0,9 | 10 x 0,9 x 0,1 = 0,90 Std. |
> | 50 | 0,7 | 50 x 0,7 x 0,1 = 3,50 Std. |

**Tabelle**
In der Übersicht sind alle Serientabellen aufgeführt, die Sie eingerichtet haben.

#### Übergangszeiten

**Kapazitätsplanung > Stammdaten > Allgemein > Übergangszeiten**

*Abb. H-133 Übergangszeiten*

In diesem Dialog geben Sie die Zeit in Schichten ein, die benötigt wird, um von einer Arbeitsart zur anderen zu wechseln. Zum Beispiel müssen nach dem ESG-Ofen die Scheiben erst abkühlen, bevor die nächste Arbeitsart beginnen kann.
⇨ Tutorial, "Übergangsmatrix und Übergangszeiten" auf Seite H-72

> **i Übergangszeiten bearbeiten**
> Die Komboboxen in den Tabellenfeldern sind nur freigeschaltet, wenn Sie eine neue Übergangzeit festlegen. Sie können die zugeordneten Arbeitsarten einer Übergangszeit nach dem Speichern nicht ändern. Wenn Sie eine Zuordnung ändern wollen, müssen Sie sie neu anlegen und anschließend die ungültige Zuordnung löschen.

**Auftragspriorität** Auftragspriorität, bei der die Übergangzeit berücksichtigt werden soll. Sie können zwischen folgenden Prioritäten wählen:
- **Normal:**
Die Übergangzeit gilt für alle Aufträge, in denen keine besondere Priorität angegeben ist. Dies ist die Standard-Einstellung.
- **Eilt:**
Die angegebene Übergangzeit gilt für Eilaufträge. Wenn Übergangszeiten für Eilaufträge verkürzt werden können, dann muss für die entsprechende Kombination von Arbeitsarten eine abweichende Übergangszeit hinterlegt werden.
- **Zugabe:**
Diese Priorität bedeutet, dass der Auftrag so gefertigt werden soll, dass er Reste und Restplatten verbraucht, die beim Zuschnitt anderer Aufträge entstehen.
- **Abruf:**
Die Übergangzeit gilt nur für Aufträge, die auf Abruf gefertigt werden.

> **i Auftragspriorität berücksichtigen**
> Wenn außer der Auftragspriorität Normal auch z. B. die Priorität Eilt berücksichtigt werden soll, dann muss für die jeweilige Kombination von Arbeitsarten eine eigene Übergangszeit eingerichtet sein. Dies gilt für alle Übergangszeiten, die für Eilaufträge auch verkürzt werden können.

**Von Arbeitsart** Ausgangs-Arbeitsart, z. B. Polieren.

**Nach Arbeitsart** Folge-Arbeitsart, z. B. Bohren. Wenn Sie <k.A.> auswählen, gilt die Übergangzeit für alle Folge-Arbeitsarten.

**Zeit in Schichten** In diesem Feld tragen Sie die Anzahl der Schichten ein, die für den Wechsel von einer Arbeitsart zur anderen benötigt werden:
- **0** = Der Folgevorgang kann in der gleichen Schicht stattfinden.
- **1** = Der Folgevorgang findet frühestens in der nächsten Schicht statt.
- **2** = Der Folgevorgang findet frühestens in der übernächsten Schicht statt.

> **Beispiel**
> Sie arbeiten in Ihrem Betrieb regulär in 3 Schichten, im Heat-Soak-Test z. B. jedoch in nur einer Schicht à 12 Stunden.
> Wenn Sie erreichen möchten, dass die Folge-Arbeitsart generell erst am nächsten Tag beginnt, dann müssen Sie in diesem Feld den Wert 3 eintragen. Damit berechnet die Kapazitätsplanung den Termin für die Folge-Arbeitsart automatisch für den nächsten Tag.

**Inkl. arbeitsfreie Tage** Bei der Berechnung können die arbeitsfreien Tage berücksichtigt werden.
- Arbeitsfreie Tage werden nicht berücksichtigt.
- Arbeitsfreien Tage werden berücksichtigt. Das bedeutet, dass ein ESG, das am Freitag aus dem Ofen kommt, ganz regulär am Montag weiter verarbeitet werden kann, da das Wochenende schon länger ist als die Übergangzeit.

## Organisation

**Kapazitätsplanung > Stammdaten > Organisation**

In diesen Dialogen legen Sie fest, wie die Kapazitätsplanung organisiert ist, z. B. die Produktionsbereiche, Maschinen, Schichtzeiten.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Produktionsbereich" auf Seite H-206
- "Aggregate" auf Seite H-207
- "Kalender" auf Seite H-217
- "Übergangsmatrix” auf Seite H-222
- "Besondere technische Restriktionen" auf Seite H-225
- "Orga Übersicht" auf Seite H-228

### Produktionsbereich

**Kapazitätsplanung > Stammdaten > Organisation > Produktionsbereich**

*Abb. H-134 Produktionsbereiche*

In diesem Dialog definieren Sie die Produktionsbereiche, z. B. Zuschnitt, Schleiferei, Bohren. Gleichzeitig legen Sie fest, welcher Status vom jeweiligen Produktionsbereich gemeldet wird, wenn die Position fertig gemeldet wurde.
⇨ Tutorial, “Produktionsbereiche (Arbeitszentren)" auf Seite H-32

**Nr.** Frei wählbare Nummer, die als ID für die einzelnen Produktionsbereiche dient. Die Nummerierung stellt keine Hierarchie dar.

> **i Der Produktionsbereich <k.A.>**
> Der Produktionsbereich Nr. 0 (Null) mit der Beschreibung <k.A.> muss einmal als Standard-Produktionsbereich definiert werden. Nachdem dieser Eintrag gespeichert wurde, wird er in diesem Dialog nicht mehr angezeigt. Prüfen Sie, ob dieser Eintrag besteht, in dem Sie ihn neu anlegen. Eine Fehlermeldung zeigt an, wenn dieser Datensatz schon angelegt ist.

**Produktionsbereich** Name des Produktionsbereiches.

**Max. Einheit/Std** Angabe, wie viele Einheiten (Stück) im Produktionsbereich pro Stunde höchstens gearbeitet werden können.
Wenn Sie z. B. 6 Schleifmaschinen haben, aber nur drei Werker, die an diesen Maschinen arbeiten können, können Sie die Gesamtkapazität nur für drei Maschinen berechnen.

**Min. Verweiltage** Anzahl der Tage, die ein Stück einer Position im Produktionsbereich verweilt:
- 0 = keine Verweilzeit
- 0,1 = eine Schicht
- 1 = ein Tag, z. B. Eingang in den Produktionsbereich heute, Ausgang morgen.

Weitere Zeiten werden als Übergangszeiten definiert.
⇨ "Übergangszeiten" auf Seite H-203
⇨ "Übergangsmatrix” auf Seite H-222

**AV-Fremdschlüssel** Fremdschlüssel des AV-Bereichs, dem der Produktionsbereich zugeordnet ist. Die Fremdschlüssel sind in den Stammdaten hinterlegt.

**Status Rückmeldung** Der Status in der Kapazitätsplanung und im Auftrag kann automatisiert über die Rückmeldung aus der Betriebsdatenerfassung (BDE) von A+W Production umgesetzt werden. Mit der Einstellung legen Sie fest, von welcher Erfassungsstelle die Rückmeldung gesendet wird.
Der Status der Positionen und des Auftrags kann im Dialog Statusrückmeldungen geprüft werden.
⇨ Verkauf, "Übersicht Statusrückmeldung" auf Seite C-590

### Aggregate

**Kapazitätsplanung > Stammdaten > Organisation > Aggregate**

Alle genutzten Maschinen werden mit den technischen Restriktionen und den Betriebskosten angelegt, die für die Planung und Berechnung der Kosten notwendig sind.

In diesem Dialog finden Sie folgende Register:
- "Aggregate - Allgemein" auf Seite H-208
- "Aggregate - Restriktionen" auf Seite H-214

Die Felder für die Definition von Restriktionen werden im Dialog Aggregat-typen freigeschaltet.
⇨ "Aggregattypen" auf Seite H-195

> **i Achtung bei nachträglicher Aktivierung von Prüfungen**
> Wenn Sie bei einem Aggregattyp eine Checkbox nachträglich aktivieren, müssen Sie alle Aggregate prüfen, die zu dem geänderten Aggregattyp gehören. Die neu freigeschalteten Felder sind standardmäßig leer. Das kann bei der Prüfung Fehler verursachen.

#### Aggregate – Allgemein

**Kapazitätsplanung > Stammdaten > Organisation > Aggregate > Register Allgemein**

*Abb. H-135 Aggregate - Allgemein*

In diesem Register legen Sie die Maschinen (Aggregate) an, die Sie nutzen und die für die Kapazitätsplanung relevant sind. Sie sollten auch ein Aggregat Versand anlegen, damit die Zeiten dafür geplant werden können.
⇨Tutorial, "Aggregattypen und Aggregate" auf Seite H-26

**Aggregat**
**Nr./Bezeichnung** Nummer (ID) und Beschreibung können frei gewählt werden. Wir empfehlen, ähnliche Maschinen in Nummernkreisen zu gruppieren, z. B. Schneidtische 100-199, Bohrmaschinen 400-499 usw.

**Typ** Aggregat-Typ, zu dem die Maschine gehört. Durch die Zuweisung werden die Felder für die Restriktionsprüfungen freigeschaltet.
⇨ "Aggregattypen" auf Seite H-195

**Produktionsbereich** Produktionsbereich, in dem die Maschine steht.
⇨ "Produktionsbereich" auf Seite H-206

**Optionen**
**Scheiben drehbar** Angabe, ob die Scheiben auf der Maschine gedreht werden können.
- Die Scheiben können nicht gedreht werden.
- Die Scheiben können gedreht werden.

**Kantenschutz möglich** Angabe, ob auf der Maschine Kantenschutz angebracht werden kann.
- Kantenschutz kann nicht angebracht werden.
- Kantenschutz kann angebracht werden.

**Autobrechen** Angabe, ob der Zuschneidetisch über eine automatische Brechvorrichtung verfügt.
- Der Tisch hat keine automatische Brechvorrichtung.
- Die Scheiben können automatisch gebrochen werden.

**Modelle möglich** Angabe, ob auf der Maschine Modelle (nicht-rechteckige Scheiben) gefertigt werden können.
- Modelle sind nicht möglich.
- Modelle sind möglich.

**Sprossen möglich** Angabe, ob auf der Maschine Sprossen gefertigt werden können.
- Sprossen sind nicht möglich.
- Sprossen sind möglich.

**VSG** Angabe, ob auf den Zuschneidetisch auch VSG geschnitten werden kann.
- Der Tisch kann keine VSG-Scheiben schneiden.
- Der Tisch kann VSG-Scheiben schneiden.

**Gasfüllung möglich** Angabe, ob auf der Maschine Gasfüllungen möglich sind.
- Gasfüllungen sind nicht möglich.
- Gasfüllungen sind möglich.

**Autoaufleger** Angabe, ob der Zuschneidetisch über einen automatischen Aufleger verfügt.
- Der Tisch hat keinen automatische Aufleger.
- Der Tisch hat einen automatischen Aufleger. In diesem Fall muss für jede Lagerplatte, die auf diesem Tisch zugeschnitten wird, ein Auflegercode vergeben werden.

**Entschichten** Angabe, ob auf der Maschine Scheiben randentschichtet werden können.
- Randentschichtungen sind nicht möglich.
- Randentschichtungen sind möglich.

**Zuschnitt Tisch**
Auswahl der Nummer von Zuschnitt-Tischen. Diese Einstellung wird bei A+W Business Pro nicht angezeigt.

**Zusatz-Optionen**
Diese Einstellungen gelten nur für A+W Business Pro.

**Ausgabeverzeichnis** Auswahl des Speicherorts für Ausgabedatei.

**Maschinencode** Auswahl des Maschinencodes. Die Maschinencodes sind im gleichnamigen Dialog hinterlegt. Wenn der gesuchte Code fehlt können Sie ihn in diesem Dialog anlegen.

**ISO-Treiber, ISO-Sektion** Die Felder werden gefüllt, wenn der Maschinencode für eine ISO-Linie ausgewählt ist.

**Schlüsselwort** Schlüsselwort, mit dem das Aggregat im System eindeutig identifiziert wird. Das Feld wird nach Auswahl des Maschinencodes automatisch gefüllt.
So?

**Kostenfaktor Z-Schnitt** Angabe zur Preiserhöhung von Z-Schnitten. Der Faktor 1 bedeutet, dass der Preis für den Schnitt nicht erhöht wird. Faktor 1,5 erhöht den Preis um die Hälfte.

**Z-Schnitt** Die Angabe bestimmt die Lage der Z-Schnitte im Schneidemodus.
- **(<k.A.>):** Keine Angaben.
- **oben:** Normalerweise ist es günstiger, die Z-Schnitte nach oben, also weg von der Arbeitsbreite zu legen, damit einzelne Schnitte zunächst über die ganze Breite gebrochen und gleich abgestellt werden können. Weisen darüber liegende Scheiben Z-Schnitte auf, ist dann bereits Platz auf dem Brechtisch, um die Scheibe zum Brechen des Z-Schnitts zu drehen.
- **unten:** Der Startpunkt liegt oben
- **beliebig:** Der Startpunkt kann beliebig gewählt werden.

**Referenzpunkt** Auswahl des Referenzpunkts für den Schneidmodus. Der Referenzpunkt des Tisches bezeichnet den Punkt mit den Koordinaten 0/0, von dem aus der Schneidmodus aufgebaut ist. Er ist wichtig, um Modelle korrekt zu schneiden.

> **i Referenzpunkt vs. Ruheposition des Schneidkopfes**
> Der Referenzpunkt muss nicht mit der Ruheposition des Schneidkopfes übereinstimmen. Bei Bystronic gibt es z. B. gespiegelte Tische, deren Referenzpunkt links vorne ist, während der Schneidkopf rechts vorne in Ruheposition steht. Bei manchen Tischen kann dies als Parameter eingestellt werden.

**Schneidmodus** Angabe, in welcher Reihenfolge die Schnitte ausgeführt werden:
- **1 - XYZW:** Der erste Schnitt verläuft senkrecht zum unteren Plattenrand. Danach folgen der Y-Schnitt und der Z-Schnitt. Die weitere Reihenfolge ist wahlweise.
- **2 - ΧΥΖ*:** Wie 1. Nach dem Z-Schnitt folgt ein beliebiger anderer Schnitt.
- **3 - XYZZZ** Der erste Schnitt verläuft senkrecht zum unteren Plattenrand. Danach folgen der Y-Schnitt und anschließend die Z-Schnitte.
- **4 - ΧΥΖΖ:** Wie 3. Jedoch sind nur zwei Z-Schnitte möglich.

*Abb. H-136 XYZ-Schnitte auf der Lagerplatte*

**Brechstart** Auswahl des Brechstarts. Der Brechbeginn richtet sich nach den räumlichen Bedingungen im Betrieb und bestimmt die Lager der Restplatte sowie in gewissem Maße die Zuschnittsreihenfolge (erste zu brechende Scheibe oben oder unten).

**Werte**
**Einheiten pro Stunde** Der Wert in diesem Feld hängt davon ab, in welcher Arbeitseinheit die Kapazitätsplanung für diese Maschine die Kapazität berechnen soll, ob in Mannstunden oder Maschinenstunden. Standardmäßig wird 1 eingetragen.
⇨Tutorial, "Arbeitseinheiten" auf Seite H-45

**Lohnkosten pro Einheit** Die einzutragenden Personalkosten hängen davon ab, in welcher Arbeitseinheit die Kapazitätsplanung für diese Maschine die Kapazität berechnen soll, z. B. in Mannstunden oder Maschinenstunden. Sie finden eine ausführliche Erläuterung zu diesem Thema unter:
⇨ Tutorial, "Arbeitseinheit = Mannstunde" auf Seite H-46

**Maschinenkosten pro Stunde** Maschinenkosten pro Stunde, z. B. für Wartung, Reparatur, Verbrauchsmittel.

**Variable Kosten pro Stunde** Sonstige Kosten, die weder zu Lohn- noch zu Maschinenkosten zählen, können in die Produktionskosten eingerechnet werden, z. B. Versicherung. Den Gesamtbetrag der Versicherung Sie müssen pro Stunde umrechnen.

**Kosten pro Einheit** Berechnete Gesamtkosten pro Einheit für diese Maschine. Sie bilden die Grundlage für die Kostenkalkulation. Die Kosten werden auf Basis von Personal-, Maschinen- und variablen Kosten und der Arbeitseinheit pro Stunde berechnet.

> **Beispiel**
> Personalkosten/Stunde
> + Maschinenkosten/Stunde dividiert durch Einheiten/Stunde
> + Variable Kosten/Stunde dividiert durch Einheiten/Stunde
> = Kosten/Einheit

**Erfassungsstelle** Nummer der Erfassungsstelle (Maschine) in A+W Production, auf die sich das Aggregat bezieht. Die Nummern müssen in A+W Business Pro und A+W Production identisch sein. Wenn Sie mit der BDE (Scanner) arbeiten, muss die Nummer der Erfassungsstelle gescannt werden.

**Leistung pro Stunde** Durchschnittliche Soll-Vorgaben (Erfahrungswerte oder Information des Maschinen-Herstellers) in Mengeneinheiten.
Diese Angabe nutzen Sie, wenn Sie z. B. alle Stammdaten bis auf die Vorgabezeiten erfasst haben und vorab in die Kapazitätsplanung einlasten möchten, um die Kapazität in Ihrer Produktion in etwa abschätzen zu können. Damit können Sie den Zeitraum überbrücken, bis alle Vorgabezeiten erfasst sind.

**Serientabelle** Auswahl der Serientabelle, in der die speziellen Zeiten für Serien definiert sind.
⇨ "Serienfaktoren" auf Seite H-202

**Default-Rückschnitt** Maße für den Rückschnitt pro Kante in mm. Der Rückschnitt beschreibt den einfachen Abstand zwischen Glasaußenkante und Rahmeninnenkante. Dieses Feld ist nur freigeschaltet, wenn im Bereich Optionen die Checkbox Entschichten aktiviert ist.

**Sperre**
**Aggregat gesperrt** Das Aggregat kann für die Planung gesperrt werden.
- Das Aggregat ist nicht gesperrt.
- Das Aggregat ist gesperrt und kann nicht in die Planung einbezogen werden. Diese Einstellung wählen Sie z. B., wenn eine neue Maschine zunächst getestet werden soll, bevor sie tatsächlich eingesetzt wird.
Wenn Sie eine Maschine wegen einer notwendigen Wartung vorübergehend sperren wollen, wählen Sie den Dialog Aggregat Ausfall:
⇨ "Aggregate Ausfall" auf Seite H-303

**Sperrformel** Über eine Sperrformel können Sie weitere Restriktionen hinterlegen, die mit den Standard-Mitteln nicht zu erreichen sind.

> **Beispiel**
> Auf einem Aggregat dürfen nur Modelle, sehr kleine und sehr große Scheiben gefertigt werden, da diese Maschine sehr langsam ist.
> Alle Rechteckscheiben mit einer Breite >200 und <2600 sowie einer Höhe >300 und <3600 dürfen nicht auf dieser Maschine geschnitten werden.
> Diese Restriktion kann nur über eine Formel angegeben werden. Falls Sie Formeln einsetzen wollen, wenden Sie sich an Ihren Service-Mitarbeiter bei der A+W Software GmbH.

**Zus. Arbeitsart bei gekoppelten Maschinen** Zurzeit nicht genutzt.

**Tabelle**
In der Übersicht werden je nach Auswahlkriterien die Maschinen aufgeführt, die der Kapazitätsplanung zur Verfügung stehen.

#### Aggregate – Restriktionen

**Kapazitätsplanung > Stammdaten > Organisation > Aggregate > Register Restriktionen**

*Abb. H-137 Aggregate - Technische Restriktionen*

In diesem Register hinterlegen Sie Mindest- und Höchstwerte für die Restriktionsprüfungen. Geben Sie jeweils 0 bis 9999 ein, wenn alle Werte zugelassen sind.

Die Felder für die Definition von Restriktionen werden im Dialog Aggregattypen freigeschaltet.
⇨ "Aggregattypen" auf Seite H-195

Wenn die technischen Restriktionen für eine Maschine bei gleichen Arbeitsarten verschieden sind, definieren Sie diese Restriktionen im Dialog Besondere technische Restriktionen. Die Kapazitätsplanung prüft den Eintrag im Dialog Besondere technische Restriktionen zuerst.
⇨ "Besondere technische Restriktionen" auf Seite H-225

Die Felder im Bereich Aggregat sind zum Register Allgemein beschrieben.
⇨ "Aggregate - Allgemein" auf Seite H-208

**Arbeitsarten / Zeitzuschläge**
In diesem Bereich werden alle Arbeitsarten aufgelistet, für die Vorgabezeiten an dieser Maschine definiert sind.
⇨ "Vorgabezeiten (Dialog)" auf Seite H-230

**Technische Restriktionen**
Die Felder für die Definition von Restriktionen werden im Dialog Aggregat-typen freigeschaltet.
⇨ "Aggregattypen" auf Seite H-195
Geben Sie 0 oder 9999 ein, wenn alle Werte zugelassen sind.

**Breite, Höhe** Min. und max. Scheibenmaße für diese Maschine.
**SZR** Min. und max. SZR für diese Maschine.
**Gesamtstärke** Min. und max. Gesamtdicke für ISO und VSG.
**Glasstärke** Min. und max. Dicke von Einfachglas.
**Diagonale** Diagonale zwischen den Rollen, z. B. auf dem Förderband vor dem ESG-Ofen.
**Scheibenanzahl** Maximale Anzahl der Scheiben für eine VSG- bzw. ISO-Einheit, z. B. 3 auf einer ISO-Linie.
**Fläche in qm** Min. und max. Fläche für diese Maschine.
**Gehrungswinkel** Min. und max. Gehrungswinkel für Facetten.
**Anzahl** Min. und max. Stückzahl der Auftragsposition. In der Position muss die Menge oder der Mengenbereich geprüft werden. Die Definition, um welche Anzahl es sich handelt, ist maschinenabhängig, z. B.
- Bohrmaschine = Anzahl Bohrlöcher
- Schleifmaschine = Anzahl der Kanten

**Bohrdurchmesser** Min. und max. Abmessung für diese Maschine.
**Rundeck-Radius** Min. und max. Abmessung für diese Maschine.
**Seitenverhältnis** Maximales Seitenverhältnis für diese Maschine.

> **Beispiel**
> Sie geben den Wert 5 ein. Dies entspricht einem max. Seitenverhältnis von 1:5. Wenn eine Seite z. B. 500 mm lang ist, dann darf die andere Seitenlänge max. 2500 mm betragen.

**Gewicht bis kg** Maximales Gewicht einer Einheit.

**Abstände zwischen Schnitten**
Bei Schneidtischen mit einer automatischen Brechanlage müssen Sie die Höchst- und Mindestabstände zwischen den Schnitten einstellen. Diese Abstände müssen eingehalten werden, damit die Anlage die Schreiben noch brechen kann.

**Min. Abs. X-X mit Y** Minimaler Abstand zwischen X-X-Schnitten wenn auch Y-Schnitte ausgeführt werden.
**Min. Abs. X-X ohne Y** Minimaler Abstand zwischen X-X-Schnitten wenn keine Y-Schnitte ausgeführt werden.
**Max. Abs. X-X** Maximaler Abstand zwischen X-X-Schnitten.
**Min. Abs. Y-Y mit Z** Minimaler Abstand zwischen Y-Y-Schnitten wenn auch Z-Schnitte ausgeführt werden.
Bei Schneidetischen mit mehreren Y-Schneidköpfen entspricht der Minimalabstand der Entfernung der Schneidrädchen zweier unmittelbar gegeneinander geschobener Schneidköpfe, z. B. Bystronic XYZVA = 300 mm.
**Min. Abs. Y-Y ohne Z** Minimaler Abstand zwischen Y-Y-Schnitten wenn keine Z-Schnitte ausgeführt werden.
**Max. Abs. Y-Y** Maximaler Abstand zwischen Y-Y-Schnitten.
**Min. Restbreite** Minimale Breite am Rand der Platte.
**Min. Abs. X-Z** Minimaler Abstand zwischen X und Z-Schnitten.
**Min. Abs. Z-Z** Minimaler Abstand zwischen Z-Schnitten.

**Toleranz für Min. Abs. X-X, Y-Y** Sie können einstellen, dass die minimalen Abstände der X-X-Schnitte und/oder Y-Y-Schnitte ignoriert werden, wenn eine Scheibe die Restriktionen verletzt.
- Die Mindestabstände werden eingehalten.
- Die Mindestabstände werden ignoriert.
so?

**Toleranz für Max. Abs. X-X, Y-Y** Sie können einstellen, dass die maximalen Abstände der X-X-Schnitte und/oder Y-Y-Schnitte ignoriert werden, wenn eine Scheibe die Restriktionen verletzt.
- Die Maximalabstände werden eingehalten.
- Die Maximalabstände werden ignoriert.
so?

> **i Toleranz kann zu Problemen führen**
> Standardmäßig werden Scheiben, die die Restriktionen verletzen, nicht optimiert. Wenn Sie die Toleranz aktivieren, werden die markierten Restriktionen ignoriert und die Scheibe durchläuft die Optimierung.

Wählen Sie eine Toleranz nur nach Rücksprache mit der A+W Software GmbH aus. Eine Änderung kann zu Fehlproduktionen oder Stillständen in der Produktion führen.

### Kalender

**Kapazitätsplanung > Stammdaten > Organisation > Kalender**

In diesem Dialog legen Sie die Arbeitstage und Schichtzeiten fest. Die Daten können nur gespeichert werden, wenn mindestens eine Schicht angelegt ist. Die Anzahl der Schichten wird in den Firmendaten festgelegt.
⇨ "Voreinstellungen Firmendaten" auf Seite H-189

Wenn keine Kalender in der Kapazitätsplanung angelegt sind, benutzt die Kapazitätsplanung den A+W Business Pro-Standard-Kalender.

Standardmäßig geht die Kapazitätsplanung von einer Schicht aus. Wenn Sie jedoch in Ihrem Betrieb mit mehr als einer Schicht arbeiten, müssen Sie als ersten Schritt die Anzahl der Schichten festlegen. Erst dann legen Sie Kalender für Maschinen mit abweichenden Schichten und Schichtzeiten an.

> **Beispiel**
> Der Kalender lässt maximal 6 Schichten pro Tag zu. Daraus resultieren bei gleichmäßiger Verteilung der Stunden maximal 4 Stunden pro Schicht. Die Verteilung der Anzahl der Stunden pro Schicht ist jedoch variabel, z. B. 5, 3, 5, 3, 5, 3 oder 4, 2, 6, 6, 3, 3.
> Mit diesen Beispielen soll verdeutlicht werden, dass Sie nicht an eine gleichmäßige Verteilung gebunden sind.
> Bei 4 Schichten können Sie bei gleichmäßiger Verteilung pro Schicht maximal 6 Stunden eintragen.
> Die Gesamtzeit der Stunden x Schichten pro Tag darf logischerweise 24 Stunden nicht überschreiten.

> **i Kalender ändern**
> Wenn Sie einen Kalender bearbeitet oder angelegt haben, müssen Sie A+W Business Pro neu starten, damit die Daten beim Einlasten zur Verfügung stehen.

In diesem Dialog finden Sie folgende Register:
- "Kalender - Auswahl" auf Seite H-218
- "Kalender - Kalender" auf Seite H-220

#### Menü Funktionen

**Kapazitätsplanung > Stammdaten > Organisation > Kalender > Menü Funktionen**

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Kalender zu schließen.

Folgende Einträge werden angezeigt:
- **Kopieren:**
Öffnet den Dialog Kalender kopieren, um einen Kalender zu übertragen, z. B. in ein neues Jahr.
⇨ "Kalender kopieren" auf Seite H-221
- **Schichtzeiten:**
Öffnet den Dialog Einstellung Schichten, in dem Sie den Schichtübergang und die Sperrzeiten festlegen können.
⇨ "Einstellungen Schichten" auf Seite H-193
Sie müssen Administratorrechte haben, um den Dialog zu öffnen. Zusätzlich muss in den Firmendaten die Checkbox Schichtwechseltabelle verwenden markiert sein.
⇨ "Schichtwechseltabelle verwenden" auf Seite H-193

#### Kalender – Auswahl

**Kapazitätsplanung > Stammdaten > Organisation > Kalender > Register Auswahl**

*Abb. H-138 Kalender - Auswahl*

In diesem Register legen Sie Kalender für Arbeitsarten, Aggregate, Produktionsbereiche oder Mandanten an.

Wenn Sie für einen Produktionsbereich oder ein Aggregat keinen eigenen Kalender anlegen, gilt der allgemeine Kalender.
⇨Tutorial, "Kalender anpassen" auf Seite H-52

**Identifikation**
Die Beschriftung der beiden Auswahlfelder richtet sich nach dem gewählten Modus.

**Arbeitsart, Aggregat** Arbeitsart und Maschine, für die der Kalender gilt.
**Produktionsbereich, Mandant** Produktionsbereich und Mandant, für die der Kalender gilt.
**Jahr** Jahr, für das der Kalender bearbeitet oder angelegt werden sollen.

**Modus**
Mit der Wahl der Option legen Sie fest, wofür Sie den Kalender anlegen wollen. Die Felder sind nur im Auswahlmodus freigeschaltet.
- **Arbeitsart, Aggregat:**
Mit dieser Einstellung legen Sie einen Kalender für die Arbeitsart und/oder die Maschine an.
- **Produktionsbereich/Mandant:**
Mit dieser Einstellung legen Sie einen Kalender für den Produktionsbereich und/oder den Mandanten an.
Um einen allgemeinen Kalender anzulegen, wählen Sie diese Option und tragen den Produktionsbereich <k. A.> und für den Mandanten alle ein.

**Kalender-Tabellen** In der Übersicht werden alle Kalender angezeigt, die den Auswahlkriterien entsprechen. Wenn Sie die Auswahl nur nach dem Modus Arbeitsart oder Produktionsbereich eingegrenzt haben, werden alle Kalender angezeigt.

#### Kalender – Kalender

**Kapazitätsplanung > Stammdaten > Organisation > Kalender Aggregat > Register Kalender**

*Abb. H-139 Kalender - Kalender*

In diesem Register legen Sie die Arbeitszeit pro Schicht fest. Die Anzahl der Schichten wird in den Firmendaten angegeben.
⇨ "Voreinstellungen Firmendaten" auf Seite H-189

**Arbeitswoche**
**Montag - Sonntag** Wenn Sie die Schichtzeit eines Wochentags ändern wollen, dann müssen Sie die entsprechende Checkbox aktivieren und die neue Stundenzahl eintragen. Die Änderung gilt nur für das angezeigte Datum. Sie müssen die neue Schichtzeit ggf. auf das Jahr oder die Kalenderwoche übertragen.
**Stunden pro Schicht** Anzahl der verfügbaren Stunden pro Wochentag und Schicht.

> **i Zusätzliche Schicht einrichten**
> Wenn Sie eine zusätzliche Schicht für ein Aggregat oder einen Produktionsbereich einrichten, müssen Sie alle Schichtzeiten neu eintragen.
> Es reicht nicht, nur die Stunden der neuen Schicht anzugeben, weil bei der Übertragung auf das Jahr (oder die Woche) die leeren Felder ebenfalls übernommen werden. Damit sind die alten Schichtzeiten gelöscht.

**Schichten in Kalender übernehmen**
**[Auf Jahr übertragen]** Überträgt die Änderungen auf alle entsprechenden Wochentage des Jahres.
Nur die Schichtzeiten der Wochentage werden übertragen, bei denen die Checkbox markiert ist.
**[Auf KW übertragen]** Überträgt die Änderungen auf alle Tage der Kalenderwoche.

**Kalenderwoche**
**Gehe zu** Auswahl der Kalenderwoche.
**[Zur aktuellen KW]** Wechselt die Darstellung im Bereich Arbeitswoche, um die Schichtzeiten für die aktuelle Kalenderwoche zu bearbeiten.

**Kalender**
In der Übersicht werden die ausgewählten Tage der Arbeitswoche mit den jeweiligen Schichtzeiten angezeigt.

### Kalender kopieren

**Kapazitätsplanung > Stammdaten > Organisation > Kalender > Menü Funktionen > Kopieren**

*Abb. H-140 Kalender kopieren*

In diesem Dialog kopieren Sie den Kalender eines Aggregats oder eines Produktionsbereichs, z. B. um ihn auf ein anderes Aggregat zu übertragen.

**Kalender Auswahl Quelle**
Die Beschriftung der beiden Auswahlfelder richtet sich nach dem gewählten Modus.
**Arbeitsart, Aggregat** Arbeitsart und Maschine, für die der Kalender angelegt ist.
**Produktionsbereich, Mandant** Produktionsbereich und Mandant, für die der Kalender angelegt ist.
**Jahr** Jahr, für das der Kalender angelegt ist.

**Kalender Auswahl Ziel**
**Arbeitsart, Aggregat** Arbeitsart und Aggregat, auf die der Kalender übertragen werden soll.
**Produktionsbereich, Mandant** Produktionsbereich und Mandant, auf die der Kalender übertragen werden soll.

### Übergangsmatrix

**Kapazitätsplanung > Stammdaten > Organisation > Übergangsmatrix**

*Abb. H-141 Übergangs-Matrix*

In diesem Dialog tragen Sie ein, wie lange es dauert, bis die Position von einem Produktionsbereich in den nächsten gelangt. Die Zeiten können Sie je nach Auftragspriorität unterschiedlich gestalten.

> **Beispiel**
> Der Übergang vom Produktionsbereich Zuschnitt in den Produktionsbereich Bearbeitung kann normalerweise in der gleichen Schicht erfolgen.
> Der Übergang vom Produktionsbereich ESG in den Produktionsbereich ISO-Fertigung benötigt mehrere Schichten bzw. 1 Tag.
> ⇨Tutorial, “Übergangsmatrix und Übergangszeiten" auf Seite H-72

**Auftragspriorität** Auswahl, bei welcher Auftragspriorität die Übergangszeit berücksichtig werden soll. Sie können zwischen folgenden Prioritäten wählen:
- **Normal:** Die Übergangszeit gilt für alle Aufträge, in denen keine besondere Priorität angegeben ist. Dies ist die Standard-Einstellung.
- **Eilt:** Die angegebene Übergangszeit gilt für Eilaufträge. Wenn Übergangszeiten für Eilaufträge verkürzt werden können, dann muss für die entsprechende Kombination von Produktionsbereichen eine abweichende Übergangszeit hinterlegt werden.
- **Zugabe:** Diese Priorität bedeutet, dass der Auftrag so gefertigt werden soll, dass er Reste und Restplatten verbraucht, die beim Zuschnitt anderer Aufträge entstehen.
- **Abruf:** Die Übergangzeit gilt nur für Aufträge, die auf Abruf gefertigt werden.

> **i Auftragspriorität berücksichtigen**
> Wenn außer der Auftragspriorität Normal auch z. B. die Priorität Eilt berücksichtigt werden soll, dann muss für die jeweilige Kombination von Produktionsbereichen eine eigene Übergangszeit eingerichtet sein. Dies gilt für alle Übergangszeiten, die für Eilaufträge auch verkürzt werden können.

**Von Produktionsbereich** Produktionsbereich, aus dem die Position kommt.

**Nach Produktionsbereich** Folge-Produktionsbereich, in den die Position wechselt.

**Übergangszeit** Zeit, die ein Glas zum Wechsel in den nächsten Produktionsbereich braucht. Die Werte werden in Tagen eingegeben:
- 0 = gleicher Tag bzw. gleiche Schicht
- 0,01 bis 0,99 = Folgeschichten
- 1 = Folgender Tag

#### Beispiele für die Berechnung des Übergangs

*Tab. H-4 Übergangszeiten in Tagen*

| Anz. Schichten | 1/Anzahl Stunden | Gleiche Schicht | Nächste Schicht | z.B. | Übernächste S. | z.B. | Über-Über-nächste S. | z.B. | Über-Über-Über-nächste S. | z.B. |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 4 | 1/4=0,25 | 0 | 0,1-0,24 | 0,2 | 0,26-0,49 | 0,4 | 0,51-0,74 | 0,6 | 0,76-1 | 1 |
| Übergang: | S1-Mo | S2-Mo | | S3-Mo | | S4-Mo | | S1-Di | |
| Übergang: | S2-Mo | S3-Mo | | S4-Mo | | S1-Di | | S2-Di | |
| 3 | 1/3=0,33 | 0 | 0,1-0,3 | 0,2 | 0,4-0,6 | 0,5 | 0,7-1 | 1 | - | - |
| Übergang: | S1-Mo | S2-Mo | | S3-Mo | | S1-Di | | - | |
| Übergang: | S2-Mo | S3-Mo | | S1-Di | | S2-Di | | - | |
| 2 | 1/2=0,5 | 0 | 0,1-0,49 | 0,3 | 0,51-1 | 1 | - | - | - | - |
| Übergang: | S1-Mo | S2-Mo | | S1-Di | | - | | - | |
| Übergang: | S2-Mo | S1-Di | | S2-Di | | - | | - | |

> **i Flexible Übergangszeit**
> Sie können statt eines festen Wertes auch eine Formel eintragen, wenn die Übergangszeit von unterschiedlichen Parametern abhängt, z. B. von der Dicke. Mit einem Rechtsklick in das Feld wird der Dialog Formelsuche geöffnet.
> Wenn Sie mit Formeln arbeiten wollen, lassen Sie sich von Ihrem Service-Mitarbeiter bei der A+W Software GmbH unterstützen.

### Besondere technische Restriktionen

**Kapazitätsplanung > Stammdaten > Organisation > Besondere technische Restriktionen**

*Abb. H-142 Besondere technische Restriktionen*

In diesem Dialog geben Sie Restriktionen für Aggregate an, die sich auf bestimmte Arbeitsarten beziehen.

Wenn auf einer Maschine unterschiedliche Arbeitsarten ausgeführt werden können, z. B. Lochbohren und Eckausschnitt, können Sie pro Arbeitsart unterschiedliche Prüfwerte angeben. Wenn die Kapazitätsplanung keine Definition für die Arbeitsart findet, werden die allgemeinen technischen Restriktionen für diese Maschine geprüft.
⇨ "Aggregate - Restriktionen" auf Seite H-214

Die verfügbaren Parameter sind abhängig von den Einstellungen im Dialog Aggregattypen.
⇨ "Aggregattypen" auf Seite H-195

**Menü Funktionen**
Über dieses Menü können Sie die Werte aus dem Standard-Aggregat übertragen. Bereits eingetragene Werte werden ohne Abfrage überschrieben.
⇨ "Aggregate - Restriktionen" auf Seite H-214

**Identifikation**
**Arbeitsart** Arbeitsart, für die die Restriktionen gelten.
**Aggregat** Maschine, für die die Restriktionen gelten, wenn die entsprechende Arbeitsart ausgeführt wird.

**Technische Restriktionen (Minimal/Maximal)**
Geben Sie 0 oder 9999 ein, wenn alle Werte zugelassen sind.

**Breite, Höhe** Min. und max. Maße für diese Maschine.
**SZR** Min. und max. SZR für diese Maschine.
**Gesamtstärke** Min. und max. Gesamtdicke für ISO und VSG für diese Maschine.
**Glasstärke** Min. und max. Dicke von Einfachglas.
**Anzahl** Min. und max. Stückzahl der Auftragsposition. In der Position muss die Menge oder der Mengenbereich geprüft werden. Die Definition, um welche Anzahl es sich handelt, ist maschinenabhängig, z. B.
- Bohrmaschine = Anzahl Bohrlöcher
- Schleifmaschine = Anzahl der Kanten

**Bohrdurchmesser** Min. und max. Abmessung für diese Maschine.
**Rundeck-Radius** Min. und max. Abmessung für diese Maschine.
**Fläche in qm** Min. und max. Fläche für diese Maschine.
**Diagonale** Diagonale zwischen den Rollen, z. B. auf dem Förderband vor dem ESG-Ofen.
**Gehrungswinkel** Min. und max. Gehrungswinkel für Facetten.

**Sonstige technische Restriktionen**
Geben Sie 9999 ein, wenn alle Werte zugelassen sind.

**Serien-Tabelle** Nummer der Serientabelle, die bei der Produktion von Serien herangezogen wird.
⇨ Softwarereferenz, "Serienfaktoren" auf Seite H-202

**Max. Scheibenanzahl** Maximale Anzahl an Scheiben, die für eine VSG- bzw. ISO-Einheit auf dieser Maschine erlaubt sind.

**Gewicht bis kg** Maximales Gewicht.

**Max. Seitenverhältnis** Maximales Seitenverhältnis für diese Maschine.

> **Beispiel**
> Der Wert 5 entspricht einem max. Seitenverhältnis von 1:5.
> Wenn eine Kantenlänge der Scheibe z. B. 500 mm beträgt, dann darf die andere Kante max. 2500 mm lang sein.

**Technische Restriktionen (Optionen)**

**Modelle möglich** Angabe, ob auf der aktuellen Maschine Modelle gefertigt werden können.
- Modelle sind nicht möglich.
- Modelle sind möglich.

**Sprossen möglich** Angabe, ob auf der aktuellen Maschine Sprossen gefertigt werden können.
- Sprossen sind nicht möglich.
- Sprossen sind möglich.

**Gasfüllung möglich** Angabe, ob auf der aktuellen Maschine Gasfüllungen möglich sind.
- Gasfüllungen sind nicht möglich.
- Gasfüllungen sind möglich.

**Scheiben drehbar** Angabe, ob die Scheiben auf der aktuellen Maschine gedreht werden können.
- Scheiben können nicht gedreht werden.
- Scheiben können gedreht werden.

**Kantenschutz möglich** Angabe, ob auf der aktuellen Maschine Kantenschutz angebracht werden kann.
- Kantenschutz kann nicht angebracht werden.
- Kantenschutz kann angebracht werden.

**Übersicht Sonder-Restriktionen**
In der Übersicht sind die Arbeitsarten und Maschinen aufgeführt, für die besondere Restriktionen hinterlegt sind.

### Orga Übersicht

**Kapazitätsplanung > Stammdaten > Organisation > Orga Übersicht**

*Abb. H-143 Orga Übersicht*

In diesem Dialog prüfen Sie, welche Maschinen und Arbeitsarten den Produktionsbereichen zugeordnet sind.

**Auswahl**
**Mandant** Mandant, dem der Produktionsbereich zugeordnet ist.
**Produktionsbereich** Produktionsbereich, dem die Aggregate zugeordnet sind.

**Auflösungstiefe**
Mit der Wahl der Option filtern Sie die Anzeige in der Übersicht.

**Ansicht**
Die Spalten in der Übersicht sind abhängig von der Auflösungstiefe.
- **Produktionsbereich:** Produktionsbereich, dem das Aggregat (die Maschine) zugeordnet ist.
- **Aggregat:** Aggregate, die dem jeweiligen Produktionsbereich zugeordnet sind.
- **Arbeitsart:** Arbeitsarten, die dem jeweiligen Aggregat zugeordnet sind.
- **Zuschläge:** Typ der Vorgabezeit, die für die jeweilige Arbeitsart zur Berechnung herangezogen werden.

## Vorgabezeiten

**Kapazitätsplanung > Stammdaten > Vorgabezeiten**

In diesem Programmbereich finden Sie die Dialoge, in denen die Vorgaben für die Zeitberechnung hinterlegt sind.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Vorgabezeiten (Dialog)" auf Seite H-230
- "Vorgabezeiten ändern" auf Seite H-238
- "Vorgabezeiten kopieren" auf Seite H-238
- "Sonderzeiten" auf Seite H-239
- "Besondere Prioritäten" auf Seite H-240

### Vorgabezeiten (Dialog)

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten**

In diesem Dialog tragen Sie die für Ihre Maschinen ermittelten Zeitwerte pro Arbeitsart und Maschine ein. Ob der Zeitwert abhängig von laufenden Metern, Quadratmetern oder Stück berechnet wird, hängt von der Maschine ab.

In diesem Dialog finden Sie folgende Register:
- "Vorgabezeiten – Zeitauswahl" auf Seite H-231
- "Vorgabezeiten - Matrix" auf Seite H-234
- "Vorgabezeiten – Vektor" auf Seite H-236
- "Vorgabezeiten – Würfel" auf Seite H-237

#### Eintrag von Zeitwerten in Stunden

Die Zeiten werden nicht in Minuten, sondern in Stunden hinterlegt. Das heißt, dass Sie die gemessenen Minuten in Stunden umrechnen müssen:

| Minuten | Zeiteintrag in Std. |
| :--- | :--- |
| 60 | 1 |
| 30 | 0,5 |
| 15 | 0,25 |
| 7,5 | 0,125 |
| 3,75 | 0,0625 |
| 1,875 | 0,03125 |

#### Menü Funktionen

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten**
Über dieses Menü können Sie andere Dialoge öffnen, ohne die Vorgabezeiten zu schließen. Folgende Einträge werden angezeigt:
- **Ändern:**
Öffnet den gleichnamigen Dialog, um die Vorgabezeiten um einen Faktor zu erhöhen oder zu reduzieren.
⇨ "Vorgabezeiten ändern" auf Seite H-238
- **Kopieren:**
Öffnet den gleichnamigen Dialog, um die Vorgabezeiten aus der Standard-Maschine zu kopieren.
⇨ "Vorgabezeiten kopieren" auf Seite H-238

#### Vorgabezeiten – Zeitauswahl

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten > Register Zeitauswahl**

*Abb. H-144 Vorgabezeiten – Tabellenauswahl*

In diesem Register legen Sie den Typ der Berechnung und die Priorität fest.
⇨ Tutorial, "Vorgabezeiten" auf Seite H-62

**Identifikation**
**Arbeitsart** Arbeitsart, für die die Vorgabezeit gilt.
**Aggregat** Maschine, an der die Arbeitsart die Vorgabezeit benötigt.
**Typ** Typ der Vorgabezeit:
- **0 - Basiszeit:**
Gestoppte Zeit für einen Arbeitsgang.
⇨ "Eintrag von Zeitwerten in Stunden" auf Seite H-230
- **1 - Zeitzuschlag:**
Ein Zeitzuschlag wird für Arbeitsarten benötigt, die mehr Aufwand erfordern, z. B. für das Zuschneiden von Modellen.
- **2 - Alternativer Vorgang:**
Diese Vorgabezeit wird nur herangezogen, wenn für die Arbeitsart eine alternative Arbeitsart existiert. In diesem Fall müssen Sie im Feld Altern. Masch.-Nr. die alternative Maschinennummer eintragen.
- **3 - Alternative ohne Stückliste:**
Als VSG-Produzent ist Ihr VSG-Artikel standardmäßig mit einer Stückliste hinterlegt. Soll aber z. B. eine VSG-Scheibe manchmal nicht produziert, sondern direkt aus einem VSG-Bandmaß geschnitten werden, dann darf die Stückliste nicht berücksichtigt werden. Für die Arbeitsart VSG schneiden würden Sie Alternative ohne Stückliste wählen. In diesem Fall müssen Sie im Feld Altern. Masch.-Nr. die alternative Maschinennummer eintragen.
- **4 - Vorgang ignorieren:**
Für einen Eckausschnitt müssen z. B. 3 Arbeitsgänge gemacht werden: 1. Bohren (von Eckloch), 2. Zuschnitt und 3. Schleifen.
Die CNC-Maschine kann alles in einem, d. h., dort wird nur die Lochbohrung berücksichtigt. Die beiden anderen Arbeitsarten werden ignoriert. Sie müssen also nur der Arbeitsart Bohren eine Vorgabezeit zuweisen, die den gesamten Vorgang umfasst. Den anderen beiden Arbeitsarten weisen Sie auf dieser Maschine dann den Wert Vorgang ignorieren zu.

**Priorität** Wenn mehrere Maschinen für eine Arbeitsart zur Verfügung stehen, müssen Sie festlegen, welche Maschine zuerst auf freie Kapazitäten geprüft werden soll und welche z. B. nur manuell ausgewählt werden kann.
Wenn zwei Maschinen die gleiche Priorität haben, dann prüft die Kapazitätsplanung die Kosten, die pro Maschine definiert sind. In diesem Fall wird automatisch die günstigere Maschine ausgewählt.
Wenn keine Kosten pro Maschine hinterlegt sind, kann das Programm keine günstigste Maschine finden. In diesem Fall muss die Priorität bei gleichen Maschinen eindeutig sein.
- **9:** höchste Priorität (Standard-Maschine). Diese Maschinen werden immer zuerst ausgelastet.
- **8 bis 1:** absteigende Prioritäten. Diese Maschinen werden je nach Auslastung ausgewählt.
- **0:** niedrigste Priorität. Diese Maschinen werden nur dann eingesetzt, wenn alle anderen (gleichartigen) Maschinen ausgelastet sind.
- **-1:** zur manuellen Einlastung. Diese Maschinen werden von der automatischen Einlastung nur bei Engpässen ausgewählt.
- **-2, -3:** nur zur manuellen Einlastung. Diese Maschinen werden nie von der automatischen Einlastung ausgewählt.

**Alternative Masch.-Nr.** In diesem Feld muss die Maschinen-Nummer aus A+W Production eingetragen werden, wenn im Feld Typ der Wert Alternativer Vorgang oder Alternative ohne Stückliste ausgewählt ist.

**Gruppieren nach**
Mit der Wahl der Option legen Sie fest, wie die Darstellung in der Übersicht gruppiert sein soll. Die Felder sind nur im Auswahlmodus freigeschaltet.
- **Arbeitsart:** Zu jeder Arbeitsart werden die zugeordneten Aggregate angezeigt.
- **Aggregat:** Zu jedem Aggregat werden die Arbeitsarten mit den definierten Zeiten angezeigt.

**Sonstige Zuschläge**
**Tabelle** Verweis auf Zuschlagstabelle, z. B. für Übergrößen. Diese Zuschlagstabellen sind im Dialog Sonderzeiten angelegt.
⇨ "Sonderzeiten" auf Seite H-239

**Einzelzeit**
**Zeit** Gemessene Zeit für die Arbeitsgänge am gewählten Aggregat.
**Zeiteinheit** Einheit, auf die sich die gemessene Zeit bezieht, z. B. auf Stück, auf Quadratmeter, auf Laufmeter usw.
**Mindestzeit** Zeit, die für eine Position mindestens berechnet wird, wenn die benötigte Zeit darunter liegt.

**Übersicht**
In der Übersicht sind alle Vorgabezeiten mit den zugeordneten Arbeitsarten aufgeführt. Mit einem Doppelklick auf Zuordnungen können werden die zugeordneten Produkte, Produktarten, Produktgruppen und/oder Warengruppen angezeigt.
Die Gruppierung legen Sie im Auswahlmodus fest.

#### Vorgabezeiten – Matrix

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten > Register Matrix**

*Abb. H-145 Vorgabezeiten – Matrix*

In diesem Register legen Sie Vorgabezeiten fest, die nach zwei Grenztypen gestaffelt sind.
⇨ Tutorial, "Vorgabezeiten" auf Seite H-62

**Grenztyp1, Grenztyp2** Der Grenztyp legt die Maßeinheit für die Staffelung der Zeit fest. Sie können z. B. Dicke und Fläche wählen.
Das Eingabefeld für den Grenzwert wird freigeschaltet, wenn Sie eine neue Spalte/Zeile einfügen. Der Grenzwert bezieht sich auf den Grenztyp.
⇨ Stammdaten, "Grenzmengen" auf Seite B-901

**Spezifikation**
**Zeiteinheit** Die Einheit bezieht sich auf den Grenzwert. Der Grenzwert kann sich z. B. auf Stück, auf Quadratmeter, auf Laufmeter usw. beziehen.
**Dreiecksform** Sie können in einer Matrix oder in einem Würfel die Zeiten so erfassen, dass die angegebenen Grenzwerte vertauscht werden dürfen, z. B. Höhe und Breite.
- Die Grenztypen dürfen nicht vertauscht werden. In diesem Fall müssen Sie in allen Feldern pro Spalte/Zeile eine Zeit eintragen. Wählen Sie diese Einstellung für Gläser, bei denen es wichtig ist, in welcher Richtung sie geschnitten werden.
- Die Grenztypen dürfen vertauscht werden. Damit müssen Sie die Zeit nur in jeweils einer der Kombinationen der Grenztypen eintragen.

**Mindestangaben**
Die Mindestangaben werden bei der Einlastung geprüft. Bei Unterschreitung der Werte wird eine Meldung angezeigt und/oder ein Zuschlag erhoben.

**Mindestzeit** Sie können angeben, wie viel Zeit für eine Position mindestens berechnet wird.

**Übersicht**
In der Übersicht geben Sie in jedem Feld pro Zeile und Spalte die Zeit ein, die bei dieser Kombination von Grenztypen für die Arbeitsart benötigt wird.

#### Vorgabezeiten – Vektor

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten > Register Vektor**

*Abb. H-146 Vorgabezeiten – Vektor*

In diesem Register hinterlegen Sie Vorgabezeiten, die nach einem Grenztyp gestaffelt sind, z. B. nach Dicke.
Die Felder sind zum Register Matrix beschrieben.
⇨ "Vorgabezeiten - Matrix" auf Seite H-234

#### Vorgabezeiten – Würfel

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten > Register Würfel**

*Abb. H-147 Vorgabezeiten – Würfel*

In diesem Register hinterlegen Sie Vorgabezeiten, die nach drei Grenztypen gestaffelt sind, z. B. nach Höhe, Breite und Dicke.
Die Felder sind zum Register Matrix beschrieben.
⇨ "Vorgabezeiten - Matrix" auf Seite H-234

### Vorgabezeiten ändern

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten > Menü Funktionen > Ändern**

*Abb. H-148 Vorgabezeiten ändern*

In diesem Dialog können Sie die Vorgabezeiten für ein Aggregat oder eine Arbeitsart ändern. Wenn Sie z. B. den Faktor 1,5 eintragen, werden alle Zeiten der ausgewählten Kombination von Aggregat und Arbeitsart um die Hälfte erhöht. Der Faktor 0,5 würde die Zeiten auf die Hälfte reduzieren.

### Vorgabezeiten kopieren

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten > Menü Funktionen > Kopieren**

*Abb. H-149 Vorgabezeiten kopieren*

In diesem Dialog können Sie Vorgabezeiten von einer Maschine und Arbeitsart kopieren, um sie auf eine andere Maschine und Arbeitsart zu übertragen. Sie können dabei Werte um einen Faktor erhöhen oder vermindern. Wenn Sie z. B. den Faktor 1,5 eintragen, werden alle Zeiten der ausgewählten Kombination von Aggregat und Arbeitsart um die Hälfte erhöht. Der Faktor 0,5 würde die Zeiten auf die Hälfte reduzieren.

### Sonderzeiten

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Sonderzeiten**

*Abb. H-150 Sonderzeiten*

In diesem Dialog definieren Sie Zeitzuschläge für besonders aufwendige Bearbeitungen, z. B. für Sondergrößen. Die Zeitschläge können Sie im Dialog Vorgabezeiten im Bereich Sonstige Zuschläge zuweisen. Sonderzeiten, die nach den gleichen Kriterien angelegt sind, können in Gruppen (Tabellen) zusammengefasst werden.
➡Tutorial, "Sonderzeiten" auf Seite H-65

Eine weitere Möglichkeit der Definition von Zeitzuschlägen in Form von Faktoren besteht über die Zuordnungsdialoge.
⇨ "Vorgabezeiten (Dialog)" auf Seite H-230
⇨ "Zuordnen" auf Seite H-242

**Zeitzuschlag für**
**Nummer** Benutzerdefinierte Nummer (ID) der Tabelle.
**Bezeichnung** Name der Tabelle, z. B. Übergrößen.

**Zuschläge (Übersicht)**
In der Übersicht werden alle definierten Zuschläge aufgeführt.

**Zuschläge**
In der Übersicht werden die Staffelungen des Zeitzuschlags angezeigt, der im Register Tabelle markiert ist.
- **Bis Grenze1, 2:** Wert pro Grenztyp, bis zu dem der Zuschlag berechnet werden soll.
- **Grenztyp 1, 2:** Grenztyp, auf den sich der Grenzwert bezieht, z. B. die Kantenlänge für die Berechnung von Übergrößen.
⇨ Stammdaten, “Grenzmengen" auf Seite B-901
- **Zuschlag:** Höhe des Zuschlags. Der Wert bezieht sich auf die Zuschlagseinheit.
- **Zuschlagseinheit:** Einheit, mit der der Zuschlag berechnet werden soll.
- **Zuschlagsart:** Basis, auf die der Zuschlag bezogen wird.

### Besondere Prioritäten

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Besondere Prioritäten**

*Abb. H-151 Besondere Prioritäten*

In diesem Dialog tragen Sie pro Maschine und Arbeitsart die Prioritäten nach zusätzlichen Kriterien ein, z. B. nach Warengruppen, pro Dicke, pro Kunde.
Wenn in den Feldern null (0) steht, gilt die besondere Priorität übergreifend, z. B. für den gewählten Kunden oder bei der angegebenen Anzahl.

Dies ist beispielsweise in folgenden Fällen sinnvoll:
- Wenn für eine Arbeitsart mehrere gleichartige Maschinen zur Verfügung stehen.
- Wenn Kunden spezielle Bearbeitungen wünschen, die nur auf speziellen Maschinen ausgeführt werden sollen oder können.
**Arbeitsart** Arbeitsart, für die eine Ausnahme definiert ist.
**Aggregat** Aggregat, an dem die Arbeitsart ausgeführt wird.
**Kunde** Kunde, für den die Priorität gilt.
**Firma** Mandant, für den die Priorität gilt.
**WGR** Warengruppe, für die die Priorität gilt.
**Kantenlänge** Kantenlänge in mm, ab der die Priorität gilt.
**Dicke >=** Glasdicke in mm, ab der die Priorität gilt. 0 = Alle Dicken.
**Anzahl >** Anzahl, ab der die Priorität gilt, z. B. Anzahl der Bohrungen, der Eckausschnitte.
**Bohrdurchmesser >=** Durchmesser einer Bohrung in mm, ab dem die Priorität gilt.

**Priorität** Die Ziffern haben folgende Bedeutung:
- **9:** höchste Priorität (Standard-Maschine). Diese Maschinen werden immer zuerst ausgelastet.
- **8 bis 1:** absteigende Prioritäten. Diese Maschinen werden je nach Auslastung ausgewählt.
- **0:** niedrigste Priorität. Diese Maschinen werden nur dann eingesetzt, wenn alle anderen (gleichartigen) Maschinen ausgelastet sind.
- **-1:** zur manuellen Einlastung. Diese Maschinen werden von der automatischen Einlastung nur bei Engpässen ausgewählt.
- **-2, -3:** nur zur manuellen Einlastung. Diese Maschinen werden nie von der automatischen Einlastung ausgewählt.

## Zuordnen

**Kapazitätsplanung > Stammdaten > Zuordnen**

In diesen Dialogen ordnen Sie die Basisprodukte von A+W Business Pro (Einfachglas, VSG, ESG, Bearbeitungen, Modelle, Sprossen usw.) den Arbeitsarten zu.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Produktarten" auf Seite H-243
- "WGR" auf Seite H-245
- "Produktgruppe" auf Seite H-246
- "Produkte" auf Seite H-247
- "Kombi-Produktart" auf Seite H-248
- "Sonderzuordnung 1" auf Seite H-249
- "Sonderzuordnung 2" auf Seite H-250
- "Sonderzuordnung 3" auf Seite H-252
- "Sonderzuordnung 4" auf Seite H-254
- "Kombi-Produktgruppe" auf Seite H-256
- "Lagerartikel" auf Seite H-257

### Produktarten

**Kapazitätsplanung > Zuordnen > Produktarten**

*Abb. H-152 Produktarten*

In diesem Dialog ordnen Sie den A+W Business Pro-Produktarten die Arbeitsarten in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für die jeweilige Produktart ausgeführt werden. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll.
⇨Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-107

**Identifikation**
**Produktart** Produktart, der Arbeitsarten zugeordnet sind.

**Arbeitsarten**
In der Übersicht werden die zugeordneten Arbeitsarten angezeigt.
**#** Nummer der Reihenfolge.
**Arbeitsart** Produktnummer und Bezeichnung der Arbeitsart. Wenn Sie <k.A.> eintragen, wird die Produktart ignoriert. Das ist z. B. für die Produktart Leistungen sinnvoll.
**Faktor** Die bei der Einlastung berechnete Zeit wird mit diesem Faktor multipliziert.
- 0 oder 1: Die Zeit wird nicht erhöht oder vermindert.
- >1: Ein Faktor von z. B. 1,5 entspricht einer Zeiterhöhung von 50%.

**Schaltflächen**
**[Neu], [Löschen]** Mit diesen Schaltflächen schalten Sie eine neue Zeile frei oder löschen einen markierten Eintrag.

**Pfeilschaltflächen** Mit diesen Schaltflächen können Sie die Reihenfolge der Arbeitsarten ändern.
Für die Produktart ESG könnte die Zuordnung z. B. wie folgt aussehen:
- Glas waschen
- Kontrolle
- ESG fertigen
- Verpacken verarbeitetes ESG
- Verladen

**Übersicht Zuordnungen**
In der Übersicht werden die Produktarten angezeigt, denen Arbeitsarten zugeordnet sind.

### WGR

**Kapazitätsplanung > Zuordnen > WGR**

*Abb. H-153 Warengruppen*

In diesem Dialog ordnen Sie den A+W Business Pro-Warengruppen die Arbeitsarten in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für die jeweilige Warengruppe ausgeführt werden. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll.
⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-107

**Identifikation**
**Warengruppe** Warengruppe, der Arbeitsarten zugeordnet sind.

**Arbeitsarten**
Die Felder und Schaltflächen in diesem Bereich sind zum Dialog Produktarten beschrieben.
"Produktarten" auf Seite H-243

**Übersicht Zuordnungen**
In der Übersicht werden die Warengruppen angezeigt, denen Arbeitsarten zugeordnet sind.

### Produktgruppe

**Kapazitätsplanung > Zuordnen > Produktgruppe**

*Abb. H-154 Produktgruppen*

In diesem Dialog ordnen Sie den A+W Business Pro-Produktgruppen die Arbeitsarten in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für die jeweilige Produktgruppe ausgeführt werden. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll.
⇨Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-107

**Identifikation**
**Produktgruppe** Produktgruppe, der Arbeitsarten zugeordnet sind.

**Arbeitsarten**
Die Felder und Schaltflächen in diesem Bereich sind zum Dialog Produktarten beschrieben.
"Produktarten" auf Seite H-243

**Übersicht Zuordnungen**
In der Übersicht werden die Produktgruppen angezeigt, denen Arbeitsarten zugeordnet sind.

### Produkte

**Kapazitätsplanung > Zuordnen > Produkte**

*Abb. H-155 Produkte*

In diesem Dialog ordnen Sie den A+W Business Pro-Produkten die Arbeitsarten aus der Kapazitätsplanung in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für das jeweilige Produkt ausgeführt werden. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll.
⇨Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-107

**Identifikation**
**Produkt** Produkt, dem Arbeitsarten zugeordnet sind.

**Arbeitsarten**
Die Felder und Schaltflächen sind zum Dialog Produktarten beschrieben.
"Produktarten" auf Seite H-243

**Übersicht Zuordnungen**
In der Übersicht werden die Produkte angezeigt, denen Arbeitsarten zugeordnet sind.

### Kombi-Produktart

**Kapazitätsplanung > Zuordnen > Kombi-Produktart**

*Abb. H-156 Kombi-Produktarten*

In diesem Dialog ordnen Sie den A+W Business Pro-Produkten, die Bestandteil einer Stückliste sind oder als Bearbeitung auf eine Produktgruppe wirken, die Arbeitsarten in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für die jeweilige Produktart ausgeführt werden. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll.
⇨Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-107

**Identifikation**
**Produkt** Produkt, dem als Stücklistenelement von z. B. VSG, ESG usw. eine andere Arbeitsart zugeordnet ist, als diejenige, die standardmäßig für das Hauptprodukt gilt.

**Als Teil von, Wirkt auf** Wenn die Float-Scheibe Teil einer Stückliste ist, kann sich die Produktionsreihenfolge oder die Arbeitsart ändern. Tragen Sie dann die entsprechende Produktart ein, z. B. ESG

**Arbeitsarten**
Die Felder und Schaltflächen in diesem Bereich sind zum Dialog Produktarten beschrieben.
"Produktarten" auf Seite H-243

**Übersicht Zuordnungen**
In der Übersicht werden die Kombi-Produktarten angezeigt, denen Arbeitsarten zugeordnet sind.

### Sonderzuordnung 1

**Kapazitätsplanung > Zuordnen > Sonderzuordnung 1**

*Abb. H-157 Sonderzuordnung 1 – Bearbeitungen*

In diesem Dialog ordnen Sie einem A+W Business Pro-Bearbeitungsprodukt und der Folgebearbeitung die Arbeitsarten in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für dieses Produkt ausgeführt werden. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll.
⇨Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-107

**Identifikation**
**Bearbeitung** Bearbeitung, der Arbeitsarten zugeordnet sind.
**Folgebearbeitung** Folgebearbeitung, der Arbeitsarten zugeordnet sind.

**Arbeitsarten**
Die Felder und Schaltflächen in diesem Bereich sind zum Dialog Produktarten beschrieben.
"Produktarten" auf Seite H-243

**Übersicht Zuordnungen**
In der Übersicht werden die Bearbeitungen und Folgebearbeitung angezeigt, denen Arbeitsarten zugeordnet sind.

### Sonderzuordnung 2

**Kapazitätsplanung > Zuordnen > Sonderzuordnung 2**

*Abb. H-158 Sonderzuordnung 2 – Bearbeitungen an Modellen*

In diesem Dialog ordnen Sie einer Bearbeitung an Modellscheiben und der Folgebearbeitung die Arbeitsarten in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für dieses Produkt ausgeführt werden. Sie können zu jeder Arbeitsart pro Kante einen Zeitfaktor angeben, der bei der Planung berechnet werden soll.

> **Beispiel**
> An einer Scheibe mit Rundbogen soll die Kantenbearbeitung an geraden Kanten auf der Standard-Schleifmaschine ausgeführt werden, die Kantenbearbeitung für den Rundbogen muss auf einer anderen Maschine gemacht werden.
> ⇨Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-107

**Identifikation**
**Bearbeitung** Bearbeitung, der Arbeitsarten zugeordnet sind.
**Modell** Modell, dem Arbeitsarten zugeordnet sind.

**Bis Stück** Stückzahl, wenn die Zuordnung der Arbeitsarten von der Anzahl der Scheiben abhängig ist, z. B. große Stückzahlen auf CNC-Maschinen. Geben Sie 9999 ein, wenn die Stückzahl nicht geprüft werden soll.

*Abb. H-159 Kennzeichnung von Ecken und Kanten des gewählten Modells*

**Arbeitsarten mit Kantenzuordnung**
In der Übersicht werden die zugeordneten Arbeitsarten angezeigt. Die Anzahl der Kanten richtet sich nach dem gewählten Modell.
Die Schaltflächen sind zum Dialog Produktarten beschrieben.
"Produktarten" auf Seite H-243

**#** Nummer der Reihenfolge.
**Arbeitsart** Nummer und Bezeichnung der Arbeitsart. Wenn Sie <k.A.> eintragen, wird die Bearbeitung ignoriert.

**Faktor** Die bei der Einlastung berechnete Zeit wird mit diesem Faktor multipliziert.
- 0 oder 1: Die Zeit wird nicht erhöht oder vermindert.
- >1: Ein Faktor von z. B. 1,5 entspricht einer Zeiterhöhung von 50%.

**1-n (Kante)** Angabe, für welche Kante der Faktor gilt. Die Anzahl der zur Verfügung stehenden Felder richtet sich nach der Anzahl der Kanten und Ecken des Modells. In der Modellskizze sind die Kanten mit roten Ziffern gekennzeichnet.
- Der Faktor wird für diese Kante nicht berechnet.
- Der Faktor wird berechnet.
