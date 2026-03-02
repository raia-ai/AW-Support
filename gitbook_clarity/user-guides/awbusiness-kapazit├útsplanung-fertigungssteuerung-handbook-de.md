---
description: A+W Business Pro Kapazitätsplanung Referenz
---

# awbusiness-kapazitãtsplanung-fertigungssteuerung-handbook-de

## Softwarereferenz Verwaltung

***

### Historientabelle für Fertigmeldungen füllen

Fertigmeldungen können in die Historie geschrieben werden.

* ☐ Fertigmeldungen werden nicht in die Historie geschrieben.
* ☑ Die Fertigmeldungen werden in die Historie geschrieben. Zusätzlich werden Arbeitsgänge protokolliert, die die durch eine Buchung fertiggemeldet sind. STSD-Rückmeldungen werden protokolliert, wenn keine Buchung in die Kapazitätsplanung erfolgt.
* Die Historie kann im Modul Statistik ausgewertet und ausgedruckt werden.

### Automatische Lieferterminsuche nach Tour

Bei Engpässen kann automatisch nach einem neuen Liefertermin gesucht werden.

* ☑ Der nächstmögliche Termin wird als Liefertermin gewählt, unabhängig davon, ob es ein Tourentag ist oder nicht. Dies ist die Standard-Einstellung.
* ☐ Der neue Liefertermin wird nach den Tourentagen des Kunden gesucht.

### Auftrag nicht splitten

Große Aufträge müssen in kleinere Positionen aufgeteilt werden, wenn der Arbeitsgang nicht für eine Position insgesamt an einem Tag erledigt werden kann.

* ☑ Die Aufträge können bei der automatischen Einlastung gesplittet werden. Dies ist die Standard-Einstellung.
* ☐ Die Aufträge können nur manuell gesplittet werden. Bei der automatischen Einlastung großer Aufträge wird eine Meldung angezeigt, so dass Sie eingreifen können.

### Verkürzte Einlastprüfung bei gleichem Aufbau

In einem Auftrag können Positionen mit gleichem Stücklistenaufbau enthalten sein, die sich nur durch die Maße unterscheiden.

* ☐ Bei jeder Position wird der gesamte Stücklistenaufbau geprüft.
* ☑ Bei gleichem Stücklistenaufbau wird von der Einlastung der vorigen Position ausgegangen, ohne die Stückliste neu zu prüfen. Dies ist die Standard-Einstellung.

### Zum Liefertermin einlasten

Bei der automatischen Einlastung werden Aufträge standardmäßig zum Liefertermin eingelastet. Nur wenn keine Kapazitäten frei sind, wird nach einem neuen Liefertermin gesucht.

* ☑ Aufträge werden mit Lieferterminsuche eingelastet. Dies ist die Standard-Einstellung.
* ☐ Die Aufträge werden ohne Suche nach einem alternativen Liefertermin eingelastet, unabhängig davon, ob Kapazitäten frei sind oder nicht.

### Automatische Fertigmeldung berechneter Aufträge

Zurzeit nicht genutzt.

### Produktionsübergabe (OrderXML) mit Planungsdaten

Für die Übergabe an die Produktion können die ermittelten Daten aus der Kapazitätsplanung in die OrderXML-Datei geschrieben werden.

* ☑ Die Daten aus der Kapazitätsplanung werden nicht in die OrderXML-Datei geschrieben.
* ☐ Die Maschinenzuordnung, Produktionsdatum und -schicht, Zeitkosten werden in die Übergabedatei geschrieben.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3101_

### Schichtwechseltabelle verwenden

Wenn Sie mit mehr als einer Schicht arbeiten, können Sie festlegen, wann die Einlastung von einer Schicht zur nächsten wechselt.

* ☐ Die Schichtwechseltabelle wird nicht verwendet.
* ☑ Die Schichtwechseltabelle wird verwendet. Wenn noch keine Schichtwechsel festgelegt sind, wird der Dialog Einstellungen Schichten geöffnet. ⇨ "Einstellungen Schichten" auf Seite H-3102

### Produktgruppen ohne Statusänderung

Sie können die Erhöhung des Positionsstatus (Auftragsstatus) durch Fertigmeldungen für Produktgruppen unterdrücken. Markieren Sie dazu die gewünschten Einträge in der Liste.

### AV-Bereiche ohne Einlastung

⇨ Sie können festlegen, dass in bestimmte AV-Bereiche nicht automatisch eingelastet wird. Das bedeutet, dass Aufträge für die markierten AV-Bereiche nur manuell eingelastet werden können.

### Einstellungen Schichten

**Stammdaten > Firma > Firmendaten > Register Kapa-Planung > Schaltfläche Einstellungen neben Checkbox Schichtwechseltabelle verwenden**

**Abbildung H-128: Stammdaten – Einstellungen Schichten**

\[Image of "Einstellungen Schichten" dialog]

* **Allgemein**
  * Schichtenzahl: 3
  * Abgleichmodus: 0
* **Optionen**
  * Beim Speichern Zeitentabelle korrigieren
* **Schichtwechselzeiten**
  * Schicht 1 > Schicht 2: 12/00/00
  * Schicht 2 > Schicht 3: 16/00/00
* **Schichtsperrzeiten**
  *
    1. Schicht: 08/00/00
  *
    2. Schicht: 10/00/00
  *
    3. Schicht: 14/00/00

In diesem Dialog legen Sie die Schichtwechsel und Sperrzeiten fest, in denen z. B. kein Auftrag eingelastet werden kann.

> **Voraussetzungen** Sie müssen Administratorrechte haben, um den Dialog zu öffnen. Zusätzlich muss in den Firmendaten die Checkbox Schichtwechseltabelle verwenden markiert sein. ⇨ "Schichtwechseltabelle verwenden" auf Seite H-3102

***

### _H-3102_ _A+W Business Pro Kapazitätsplanung_

#### Allgemein

Die Einstellungen in diesem Bereich werden aus den Firmendaten übernommen. ⇨ "A+W Business-Kapazitätsplanung" auf Seite H-3099

**Schichtzahl** Anzahl der Schichten.

**Abgleichmodus** Modus, nach dem nach Aggregaten gesucht wird:

* **0 = Automatisch:** Das Programm sucht automatisch nach der kosten- und zeitgünstigsten Maschine und lastet die Aufträge dort ein. Dies ist die Standard-Einstellung.
* **1 = Semi-automatisch:** Das Programm bietet die alternativen Maschinen zur Auswahl an. Wenn der Liefertermin nicht eingehalten werden kann, müssen Sie eingreifen.
* **3 = Manuell:** Mit dieser Einstellung müssen Sie bei jedem möglichen Wechsel (Maschine, Schicht usw.) manuell eingreifen. Alternative Maschinen können nur bei der manuellen Ein- oder Umlastung ausgewählt werden.

#### Optionen

**Beim Speichern Zeitentabellen korrigieren** Wenn Sie die Werte geändert haben, können die Zeiten der eingelasteten Aufträge überrechnet werden.

* ☐ Die neuen Zeiten verändern die aktuell eingelasteten Aufträge nicht.
* ☑ Die neuen Zeiten werden sofort übernommen. Alle eingelasteten Aufträge werden neu berechnet.

#### Schichtwechselzeiten

**Schicht 1 > Schicht 2, ...** Angabe, wann der Übergang von einer Schicht zur nächsten Schicht stattfindet. Diese Einstellung ist z. B. wichtig für die Berechnung von Übergangszeiten. Die Anzahl der angezeigten Felder hängt von der Anzahl der Schichten ab, die in den Firmendaten angegeben sind. ⇨ "A+W Business-Kapazitätsplanung" auf Seite H-3099

#### Schichtsperrzeiten

**1., 2., ... Schicht** Angabe, ab wann die jeweilige Schicht für neue Aufträge gesperrt ist.

> **Beispiel: 2. Schicht 10:00** Bis 10 Uhr können Aufträge in die zweite Schicht des aktuellen Tages eingelastet werden. Damit halten Sie sich die 2. Schicht so frei, dass alle eingelasteten Aufträge tatsächlich gefertigt werden können und keine Restmengen entstehen. Aufträge, die nach 10 Uhr eingelastet werden, werden für die 3. Schicht oder den folgenden Tag geplant.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3103_

### Allgemein

**Kapazitätsplanung > Stammdaten > Allgemein**

In diesen Dialogen hinterlegen Sie Daten für die Arbeitsgänge und Maschinen, die in der Produktion zur Verfügung stehen.

In diesem Kapitel finden Sie Informationen zu folgenden Stammdaten:

* "Aggregattypen" auf Seite H-3104
* "Arbeitsarten" auf Seite H-3107
* "Zugeordnete Aggregate" auf Seite H-3110
* "Serienfaktoren" auf Seite H-3111
* "Übergangszeiten" auf Seite H-3112

### Aggregattypen

**Kapazitätsplanung > Stammdaten > Allgemein > Aggregattypen**

**Abbildung H-129: Aggregattypen**

| Nr. | Bezeichnung              | Maß-Check | SZR | Gesamtstärke | Einzelstärke | Gewicht | Scheibenanzahl | Fläche | drehbar | Gas | Kantenschutz | Modell | Sprossen | Anzahl |
| --- | ------------------------ | --------- | --- | ------------ | ------------ | ------- | -------------- | ------ | ------- | --- | ------------ | ------ | -------- | ------ |
| 10  | Zuschnitt / Cutting      | ✔         | ☐   | ☐            | ✔            | ☐       | ☐              | ✔      | ☐       | ☐   | ☐            | ☐      | ☐        | ☐      |
| 20  | Bearbeitung / Processing | ☐         | ☐   | ☐            | ☐            | ✔       | ☐              | ☐      | ☐       | ☑   | ☐            | ☐      | ☐        | ☐      |
| 40  | ESG/TG                   | ☐         | ☐   | ☐            | ☐            | ☐       | ☐              | ✔      | ☐       | ☐   | ☐            | ☐      | ☐        | ☐      |
| 50  | VSG/LG                   | ☐         | ☐   | ☐            | ☐            | ☐       | ☐              | ☐      | ☐       | ☐   | ☐            | ☐      | ☐        | ☐      |
| 80  | ISO/IG                   | ☐         | ☐   | ☐            | ☐            | ☐       | ☐              | ☑      | A       | ☐   | ☐            | ☐      | ☐        | ☐      |
| 85  | Rahmen / Frame           | ☐         | ☐   | ☐            | ☐            | ☐       | ☐              | ☐      | ☐       | ☐   | ☐            | ☐      | ☐        | ☐      |
| 90  | Keine Prüfung / No Check | ☐         | ☐   | ☐            | ☐            | ☐       | ☐              | ☐      | ☐       | ☐   | ☐            | ☐      | ☐        | ☐      |
| 91  | CNC                      | ☐         | ☐   | ☐            | ☐            | ☐       | ☐              | ☐      | ☐       | ☐   | ☐            | ☐      | ☐        | ☐      |

In diesem Dialog definieren Sie die Maschinentypen, die Sie in Ihrer Produktion einsetzen, z. B. Schneidtische, Bohrmaschinen, Schleifmaschinen, ESG-Öfen usw. Sie müssen zuerst die Maschinentypen definieren und festlegen, welche Restriktionen jeweils geprüft werden sollen.

Mit einem Doppelklick in den Zeilenkopf öffnen Sie den Dialog **Zugeordnete Aggregate**. ⇨ "Zugeordnete Aggregate" auf Seite H-3110

***

### _H-3104_ _A+W Business Pro Kapazitätsplanung_

Durch das Aktivieren der Checkboxen werden die entsprechenden Felder im Dialog **Aggregate** freigeschaltet. ⇨ "Aggregate" auf Seite H-3117

> **Achtung bei nachträglicher Aktivierung** Wenn Sie eine Checkbox nachträglich aktivieren, müssen Sie alle Aggregate prüfen, die zu dem geänderten Aggregattyp gehören. Die neu freigeschalteten Felder sind standardmäßig leer. Das kann bei der Prüfung Fehler verursachen.

**Nr.** Frei wählbare Nummer, die als ID für die einzelnen Maschinentypen dient.

**Bezeichnung** Name des Maschinentyps.

> **Einstellungen** Im Folgenden wird jeweils die Funktion der aktivierten Checkbox genannt. Eine ausführliche Beschreibung der Funktion finden Sie im Dialog Aggregate mit der Beschreibung der einzelnen Einstellungen. ⇨ "Aggregate" auf Seite H-3117

**Maschinentyp** Die Auswahl des Maschinentyps steht nur in A+W Business Pro zur Verfügung. Für diese Programmversion sind die Maschinentypen fest vorgegeben. Der Maschinentyp bezieht sich auf die konkreten Maschinen und die zu verwendeten Treiber. Die Auswahl legt fest, welche Maschinentreiber im Dialog Aggregate > Zusatz-Optionen zur Verfügung stehen. Mit diesen Treibern kann A+W Business Pro die Maschinen ansteuert. Im Unterschied zum Aggregattypen kann dieser Typ nicht konfiguriert werden.

**Maß-Check** Die Größenrestriktionen müssen bei diesem Maschinentyp geprüft werden.

**SZR** Die SZR-Restriktionen müssen bei diesem Maschinentyp geprüft werden.

**Gesamtstärke** Die Gesamtdicke einer ISO- oder einer VSG-Einheit muss geprüft werden.

**Einzelstärke** Die Dicke eines einzelnen Einfachglases muss geprüft werden.

**Gewicht** Das Gewicht der Scheibe muss geprüft werden.

**Scheibenanzahl** Die Anzahl der Scheiben eines Produkts (2-fach, 3-fach-ISO oder VSG) muss geprüft werden.

**Fläche** Die Fläche der Scheibe muss geprüft werden.

**Gas** Die Position muss auf Gasfüllung überprüft werden.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3105_

**Kantenschutz** Der Kantenschutz muss bei Isoliergläsern geprüft werden.

**Modell** Die Position muss auf Modelle geprüft werden.

**Sprossen** Die Position muss auf Sprossen geprüft werden.

**Anzahl** In der Position muss die Menge oder der Mengenbereich geprüft werden. Die Definition, um welche Anzahl es sich handelt, ist maschinenabhängig, z. B.

* Bohrmaschine = Anzahl Bohrlöcher
* Schleifmaschine = Anzahl der Kanten

**Seitenverhältnis** Das Seitenverhältnis der Scheibe muss geprüft werden.

**Drehbar** Bei jedem Glas muss geprüft werden, ob es gedreht werden darf.

**Bohrdurchmesser** Der Durchmesser einer Bohrung muss geprüft werden.

**Eckradius** Der Radius von gerundeten Ecken muss geprüft werden.

**Diagonale** Diagonale zwischen den Rollen, z. B. auf dem Förderband vor dem ESG-Ofen, muss geprüft werden.

**Gehrungswinkel** Min. und max. Gehrungswinkel für Facetten muss geprüft werden.

***

### _H-3106_ _A+W Business Pro Kapazitätsplanung_

### Arbeitsarten

**Kapazitätsplanung > Stammdaten > Allgemein > Arbeitsarten**

**Abbildung H-130: Arbeitsarten**

\[Image of a table with columns: Nr., Bezeichnung, Sequenz, Nur Hauptprodukt, AWProd.Nr., % Limit, Manuelle Agg.-Auswahl, Ausweich-Arbeitsart]

In diesem Dialog hinterlegen Sie die Arbeitsarten. Das sind alle Tätigkeiten, für die Zeiten benötigt werden, also z. B. Zuschnitt, manueller Zuschnitt, Kanten säumen, Kanten polieren, VSG sägen, verpacken.

In einem Arbeitsprozess können mehreren Arbeitsarten nacheinander ausgeführt werden, z. B. für die ESG-Fertigung der Zuschnitt und das Härten. Sie müssen also entscheiden, ob Sie die einzelnen Schritte jeweils als eine Arbeitsart anlegen oder den gesamten Arbeitsprozess. Je nach der Organisation in Ihrem Betrieb kann es auch sinnvoll sein, beide Formen zu wählen. ⇨ Tutorial, "Arbeitsarten" auf Seite H-2936

> **Arbeitsarten scannen** Wenn Sie mit einer Betriebsdatenerfassung (BDE) arbeiten, müssen Sie alle Arbeitsarten anlegen, die mit dem Scanner erfasst werden können. Nur dann können Sie auch die Rückmeldungen für den Status auswerten.

#### Menü Funktionen

Über dieses Menü können Sie sich eine Übersicht über die Maschinen anzeigen lassen, die der markierten Arbeitsart zugeordnet sind. ⇨ "Zugeordnete Aggregate" auf Seite H-3110

***

### _A+W Business Pro Kapazitätsplanung_ _H-3107_

**Nr.** Frei wählbare Nummer, die als ID für die einzelnen Arbeitsarten dient. Wir empfehlen, die Nummern in Zehnersprüngen anzugeben, so dass Platz zum Einfügen neuer Arbeitsarten bleibt. Damit können Sie ähnliche Arbeitsarten zusammenhalten. Außerdem sollten die Arbeitsarten in der Reihenfolge nummeriert sein, in der sie im Fertigungsprozess aufeinander folgen.

**Bezeichnung** Name der Arbeitsart. Als Arbeitsart kann auch ein Zuschlag definiert werden, der die Maschinenzeit z. B. beim Zuschneiden von Modellen verlängert.

**Sequenz** Reihenfolge der Bearbeitung. Die Ziffer entscheidet, wann die Bearbeitung ausgeführt wird. Die Sequenz gibt die Priorität (Produktionsreihenfolge) der einzelnen Arbeitsarten innerhalb der Kapazitätsplanung an.

> **Beispiel** Kanten müssen vor dem Lochbohren geschliffen werden. VSG-Vorverbund nach dem Bohren. Daraus folgt, dass die Sequenz für den Kantenschliff kleiner, für den VSG-Vorverbund größer ist als für die Lochbohrung.

Sie sollten bei der Zuordnung der Ziffern mindestens in 10er-Schritten, besser noch in 50er oder 100er-Schritten arbeiten, damit Sie genug Spielraum für neue Arbeitsarten haben.

**Nur Hauptprodukt** Einige Arbeitsarten sind nur beim Hauptprodukt sinnvoll, jedoch nicht für die Stücklistenelemente.

* ☑ Diese Arbeitsart kann sowohl beim Hauptprodukt als auch bei den Stücklisten-Komponenten angewendet werden.
* ☐ Diese Arbeitsart gilt nur für das Hauptprodukt, z. B. ist der Versand für Stücklisten-Komponenten nicht möglich.

**AWProd.Nr** Artikelnummer aus A+W Production. Arbeitsarten, die Bestandteil eines Auftrages bei einem Glasproduzenten sind, jedoch im Auftrag selbst nicht extra spezifiziert werden, benötigen eine A+W Production-Artikelnummer, z. B. Zuschnitt. Für diese Artikelnummer muss in A+W Business Pro ein Produkt der Produktart/Produktgruppe Bearbeitungen mit derselben Nummer angelegt werden.

***

### _H-3108_ _A+W Business Pro Kapazitätsplanung_

**% Limit** Die Kapazitätsplanung lastet standardmäßig einen Auftrag so ein, dass dieser zeitnah zum Liefertermin gefertigt wird. Bei großen Aufträgen kann dies zu Problemen führen. Der Prozentwert legt fest, wie groß der Anteil eines Auftrags an der Tageskapazität sein darf. Größere Aufträge werden dann über mehrere Tage verteilt.

> **Beispiel** Sie erhalten einen großen Auftrag am 17. Juli. Der Liefertermin ist der 22. September.
>
> Die Kapazitätsplanung würde diesen Auftrag so einplanen, dass er kurz vor Liefertermin gefertigt würde. Damit wäre aber die Produktion für z. B. vier komplette Tage durch diesen Auftrag blockiert. Andere Aufträge könnten in dieser Zeit nicht mehr eingelastet werden.
>
> Da Sie aber Zeit haben, den Auftrag verteilt über den gesamten Zeitraum bis zum Liefertermin zu fertigen, können Sie hier eintragen, dass die Arbeitsart pro Auftragsposition nur z. B. 10% der Tageskapazität beanspruchen darf.

Dieser Wert wird nur berücksichtig, wenn Sie die Option Pos. Control aktivieren. Diese Option finden Sie in folgenden Dialogen:

* "Einlasten NV" auf Seite H-3198
* "Einlasten Auftrag" auf Seite H-3204
* "Aggregate Ausfall" auf Seite H-3218

**Manuelle Aggregatauswahl** Wenn Sie mehrere Maschinen haben, die die gleiche Arbeitsart ausführen können, legen Sie eine Maschine mit Priorität 9 in den Vorgabezeiten fest, damit sie standardmäßig ausgewählt wird. Wenn diese Maschine an einem Tag ausgelastet ist, kann auf eine der anderen Maschinen zugegriffen werden.

* ☑ Der Auftrag wird automatisch einer anderen Maschine zugeordnet. Wenn dabei jedoch der Produktionstag gewechselt wird, müssen Sie manuell eingreifen.
* ☐ Wenn die Kapazität einer Maschine überschritten wird, müssen Sie manuell eine andere Maschine auswählen. Die möglichen Ausweichmaschinen werden in einem Dialog angezeigt.

**Ausweich-Arbeitsart** Sie können einer Arbeitsart eine Ausweich-Arbeitsart zuzuordnen, z. B. für das Bohren von Sondergrößen.

> **Beispiel** Sie haben die beiden Arbeitsarten Bohren und Sondergrößen bohren. In der Arbeitsart Bohren wird die Ausweicharbeitsart Sondergrößen bohren eingetragen.
>
> Der Standard-Bohrmaschine wird die Arbeitsart Bohren zugewiesen. Diese kann jedoch nur beschränkte Bohrdurchmesser bohren. Wenn diese Abmessungen überschritten werden, dann prüft die Kapazitätsplanung, ob eine Ausweich-Arbeitsart eingetragen ist. Wenn ja, sucht das Programm nach einer zugeordneten Maschine.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3109_

### Zugeordnete Aggregate

**Kapazitätsplanung > Stammdaten > Allgemein > Arbeitsarten > Menü Funktionen > Zugeordnete Aggregate**

**Abbildung H-131: Zugeordnete Aggregate**

\[Image of "Zugeordnete Aggregate" dialog for "Arbeitsart: Bohrungen / Drillings"]

| Aggregat              | Bemerkung                     | Prio |
| --------------------- | ----------------------------- | ---- |
| CNC-Maschine          | 0 - Basiszeit                 | 8    |
| Bohrungen / Drillings | 0 - Basiszeit / 0 - Basictime | 9    |

In diesem Dialog werden die Maschinen aufgelistet, die einem Aggregattyp oder einer Arbeitsart zugeordnet sind. Im Infobereich des Dialogs wird angezeigt, aus welchem Dialog heraus Sie die Übersicht geöffnet haben.

**Aggregat** Name der Maschine, die zugeordnet ist.

**Bemerkung** In dieser Spalte wird bei Arbeitsarten angezeigt, ob die Arbeitsart für die zugeordnete Maschine als Basiszeit oder als Zeitzuschlag ausgewertet wird.

**Prio** Priorität, mit der das Aggregat beim Einlasten automatisch ausgewählt wird.

* **9:** höchste Priorität (Standard-Maschine). Diese Maschinen werden immer zuerst ausgelastet.
* **8 bis 1:** absteigende Priorität. Diese Maschinen werden je nach Auslastung ausgewählt.
* **0:** niedrigste Prioritäten. Diese Maschinen werden nur dann eingesetzt, wenn alle anderen (gleichartigen) Maschinen ausgelastet sind.
* **-1:** zur manuellen Einlastung. Diese Maschinen werden von der automatischen Einlastung nur bei Engpässen ausgewählt.
* **-2:** nur zur manuellen Einlastung. Diese Maschinen werden nie von der automatischen Einlastung ausgewählt. Die Maschine kann nur manuell ausgewählt werden.
* **-3:** wird nur bei der Rückmeldung vom Produktionssystem ausgewählt, wenn dort umgelastet wurde. Bei Umlasten in der Kapazitätsplanung werden nur noch Aggregate mit Prio > -3 angezeigt.

***

### _H-3110_ _A+W Business Pro Kapazitätsplanung_

### Serienfaktoren

**Kapazitätsplanung > Stammdaten > Allgemein > Serienfaktoren**

**Abbildung H-132: Serienfaktoren**

\[Image of "Serienfaktoren" dialog]

* **Identifikation**
  * Nummer: 1
  * Bezeichnung: Tabelle 1
* **Serientabellen**
  * ab Stück: 10, Faktor: 0,900
  * ab Stück: 50, Faktor: 0,700
* **Tabelle** (Overview)
  * Nummer: 1, Bezeichnung: Tabelle 1

In diesem Dialog legen Sie fest, bei welchen Stückzahlen die geplanten Zeiten reduziert werden, z. B., weil das Rüsten beim Schleifen oder Bohren entfällt.

Die Nummer der Serientabelle ordnen Sie der Maschine im Dialog **Aggregate** zu. ⇨ "Serientabelle" auf Seite H-3122

#### Identifikation

**Nummer** Die Nummer wird automatisch vergeben, wenn Sie eine neue Serientabelle anlegen.

**Bezeichnung** Name der Serientabelle. Geben Sie einen sprechenden Namen ein, wenn Sie mehrere Tabellen anlegen, z. B. für Bohren oder Schleifen.

#### Serientabellen

**Ab Stück** Menge, ab der ein Faktor berücksichtigt werden soll.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3111_

**Faktor** Faktor, mit dem die Basiszeit für den Arbeitsgang multipliziert wird.

> **Beispiel**

| Ab Stück | Faktor pro Stück | Zeit an der Maschine       |
| -------- | ---------------- | -------------------------- |
| 1        | 1                | 0,10 Std                   |
| 10       | 0,9              | 10 x 0,9 x 0,1 = 0,90 Std. |
| 50       | 0,7              | 50 x 0,7 x 0,1 = 3,50 Std. |

#### Tabelle

In der Übersicht sind alle Serientabellen aufgeführt, die Sie eingerichtet haben.

### Übergangszeiten

**Kapazitätsplanung > Stammdaten > Allgemein > Übergangszeiten**

**Abbildung H-133: Übergangszeiten**

| Auftragspriorität | von Arbeitsart                        | nach Arbeitsart                    | Zeit in Schichten | Inkl. arbeitsfreie Tage |
| ----------------- | ------------------------------------- | ---------------------------------- | ----------------- | ----------------------- |
| 0 - Normal        | 0001 - Zuschnitt / Cutting            | 0100 - Kantenbearbeitungen / Ed... | 1                 | ☐                       |
| 0 - Normal        | 0001 - Zuschnitt / Cutting            | 0107 - Facette / Facet             | 1                 | ☐                       |
| 0 - Normal        | 0400 - ESG-Fertigung / TG temperin... | 9900 - Versand / Shipping          | 3                 | ☐                       |

In diesem Dialog geben Sie die Zeit in Schichten ein, die benötigt wird, um von einer Arbeitsart zur anderen zu wechseln. Zum Beispiel müssen nach dem ESG-Ofen die Scheiben erst abkühlen, bevor die nächste Arbeitsart beginnen kann. ⇨ Tutorial, "Übergangsmatrix und Übergangszeiten" auf Seite H-2977

> **Übergangszeiten bearbeiten** Die Komboboxen in den Tabellenfeldern sind nur freigeschaltet, wenn Sie eine neue Übergangzeit festlegen. Sie können die zugeordneten Arbeitsarten einer Übergangszeit nach dem Speichern nicht ändern. Wenn Sie eine Zuordnung ändern wollen, müssen Sie sie neu anlegen und anschließend die ungültige Zuordnung löschen.

***

### _H-3112_ _A+W Business Pro Kapazitätsplanung_

**Auftragspriorität** Auftragspriorität, bei der die Übergangzeit berücksichtigt werden soll. Sie können zwischen folgenden Prioritäten wählen:

* **Normal:** Die Übergangzeit gilt für alle Aufträge, in denen keine besondere Priorität angegeben ist. Dies ist die Standard-Einstellung.
* **Eilt:** Die angegebene Übergangzeit gilt für Eilaufträge. Wenn Übergangszeiten für Eilaufträge verkürzt werden können, dann muss für die entsprechende Kombination von Arbeitsarten eine abweichende Übergangszeit hinterlegt werden.
* **Zugabe:** Diese Priorität bedeutet, dass der Auftrag so gefertigt werden soll, dass er Reste und Restplatten verbraucht, die beim Zuschnitt anderer Aufträge entstehen.
* **Abruf:** Die Übergangzeit gilt nur für Aufträge, die auf Abruf gefertigt werden.

> **Auftragspriorität berücksichtigen** Wenn außer der Auftragspriorität Normal auch z. B. die Priorität Eilt berücksichtigt werden soll, dann muss für die jeweilige Kombination von Arbeitsarten eine eigene Übergangszeit eingerichtet sein. Dies gilt für alle Übergangszeiten, die für Eilaufträge auch verkürzt werden können.

**Von Arbeitsart** Ausgangs-Arbeitsart, z. B. Polieren.

**Nach Arbeitsart** Folge-Arbeitsart, z. B. Bohren. Wenn Sie \<k.A.> auswählen, gilt die Übergangzeit für alle Folge-Arbeitsarten.

**Zeit in Schichten** In diesem Feld tragen Sie die Anzahl der Schichten ein, die für den Wechsel von einer Arbeitsart zur anderen benötigt werden:

* 0 = Der Folgevorgang kann in der gleichen Schicht stattfinden.
* 1 = Der Folgevorgang findet frühestens in der nächsten Schicht statt.
* 2 = Der Folgevorgang findet frühestens in der übernächsten Schicht statt.

> **Beispiel** Sie arbeiten in Ihrem Betrieb regulär in 3 Schichten, im Heat-Soak-Test z. B. jedoch in nur einer Schicht à 12 Stunden. Wenn Sie erreichen möchten, dass die Folge-Arbeitsart generell erst am nächsten Tag beginnt, dann müssen Sie in diesem Feld den Wert 3 eintragen. Damit berechnet die Kapazitätsplanung den Termin für die Folge-Arbeitsart automatisch für den nächsten Tag.

**Inkl. arbeitsfreie Tage** Bei der Berechnung können die arbeitsfreien Tage berücksichtigt werden.

* ☐ Arbeitsfreie Tage werden nicht berücksichtigt.
* ☑ Arbeitsfreien Tage werden berücksichtigt. Das bedeutet, dass ein ESG, das am Freitag aus dem Ofen kommt, ganz regulär am Montag weiter verarbeitet werden kann, da das Wochenende schon länger ist als die Übergangzeit.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3113_

## Organisation

**Kapazitätsplanung > Stammdaten > Organisation**

In diesen Dialogen legen Sie fest, wie die Kapazitätsplanung organisiert ist, z. B. die Produktionsbereiche, Maschinen, Schichtzeiten.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:

* "Produktionsbereich" auf Seite H-3115
* "Aggregate" auf Seite H-3117
* "Kalender" auf Seite H-3127
* "Übergangsmatrix” auf Seite H-3134
* "Besondere technische Restriktionen" auf Seite H-3136
* "Orga Übersicht" auf Seite H-3139

***

### _H-3114_ _A+W Business Pro Kapazitätsplanung_

### Produktionsbereich

**Kapazitätsplanung > Stammdaten > Organisation > Produktionsbereich**

**Abbildung H-134: Produktionsbereiche**

| Nr. | Produktionsbereich                  | Max. Einheit/Std | Min. Verweiltage | AV-Fremdschlüssel | Status Rückmeldung                             |
| --- | ----------------------------------- | ---------------- | ---------------- | ----------------- | ---------------------------------------------- |
| 5   | Wareneingang / Goods Receipt        | 0                | 0.0              | Alle              | 0460 - BDE Zuschnitt fertig/Cutting completed  |
| 10  | Zuschnitt / Cutting                 | 0                | 0.0              | Alle              | 0465 - BDE Schleiferei fertig/Grinding complet |
| 20  | Kantenbearbeitung / Edge Processing | 0                | 0.0              | Alle              | 0470 - BDE Bohren fertig/Drilling completed    |
| 25  | CNC Bearbeitungen / CNC Processings | 0                | 0.0              | Alle              | 0000 -                                         |
| 30  | Bohren/Drilling                     | 0                | 0.0              | Alle              | 0485 - BDE ESG fertig/TEMP completed           |
| 40  | ESG Fertigung / TG Production       | 0                | 0.0              | Alle              | 0490 - BDE VSG fertig/LAMI completed           |
| 50  | VSG Fertigung / LG Production       | 0                | 0.0              | Alle              | 0510 - BDE ISO fertig/IG completed             |
| 80  | ISO Fertigung/IG Production         | 0                | 0.0              | Alle              | 0000 -                                         |

In diesem Dialog definieren Sie die Produktionsbereiche, z. B. Zuschnitt, Schleiferei, Bohren. Gleichzeitig legen Sie fest, welcher Status vom jeweiligen Produktionsbereich gemeldet wird, wenn die Position fertig gemeldet wurde. ⇨ Tutorial, "Produktionsbereiche (Arbeitszentren)" auf Seite H-2938

**Nr.** Frei wählbare Nummer, die als ID für die einzelnen Produktionsbereiche dient. Die Nummerierung stellt keine Hierarchie dar.

> **Der Produktionsbereich \<k.A.>** Der Produktionsbereich Nr. 0 (Null) mit der Beschreibung \<k.A.> muss einmal als Standard-Produktionsbereich definiert werden. Nachdem dieser Eintrag gespeichert wurde, wird er in diesem Dialog nicht mehr angezeigt. Prüfen Sie, ob dieser Eintrag besteht, in dem Sie ihn neu anlegen. Eine Fehlermeldung zeigt an, wenn dieser Datensatz schon angelegt ist.

**Produktionsbereich** Name des Produktionsbereiches.

**Max. Einheit/Std** Angabe, wie viele Einheiten (Stück) im Produktionsbereich pro Stunde höchstens gearbeitet werden können. Wenn Sie z. B. 6 Schleifmaschinen haben, aber nur drei Werker, die an diesen Maschinen arbeiten können, können Sie die Gesamtkapazität nur für drei Maschinen berechnen.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3115_

**Min. Verweiltage** Anzahl der Tage, die ein Stück einer Position im Produktionsbereich verweilt:

* 0 = keine Verweilzeit
* 0,1 = eine Schicht
* 1 = ein Tag, z. B. Eingang in den Produktionsbereich heute, Ausgang morgen. Weitere Zeiten werden als Übergangszeiten definiert. ⇨ "Übergangszeiten" auf Seite H-3112 ⇨ "Übergangsmatrix" auf Seite H-3134

**AV-Fremdschlüssel** Fremdschlüssel des AV-Bereichs, dem der Produktionsbereich zugeordnet ist. Die Fremdschlüssel sind in den Stammdaten hinterlegt.

**Status Rückmeldung** Der Status in der Kapazitätsplanung und im Auftrag kann automatisiert über die Rückmeldung aus der Betriebsdatenerfassung (BDE) von A+W Production umgesetzt werden. Mit der Einstellung legen Sie fest, von welcher Erfassungsstelle die Rückmeldung gesendet wird. Der Status der Positionen und des Auftrags kann im Dialog Statusrückmeldungen geprüft werden. ⇨ Verkauf, "Übersicht Statusrückmeldung" auf Seite C-1860

***

### _H-3116_ _A+W Business Pro Kapazitätsplanung_

### Aggregate

**Kapazitätsplanung > Stammdaten > Organisation > Aggregate**

Alle genutzten Maschinen werden mit den technischen Restriktionen und den Betriebskosten angelegt, die für die Planung und Berechnung der Kosten notwendig sind.

In diesem Dialog finden Sie folgende Register:

* "Aggregate - Allgemein" auf Seite H-3118
* "Aggregate - Restriktionen" auf Seite H-3124

Die Felder für die Definition von Restriktionen werden im Dialog **Aggregattypen** freigeschaltet. ⇨ "Aggregattypen" auf Seite H-3104

> **Achtung bei nachträglicher Aktivierung von Prüfungen** Wenn Sie bei einem Aggregattyp eine Checkbox nachträglich aktivieren, müssen Sie alle Aggregate prüfen, die zu dem geänderten Aggregattyp gehören. Die neu freigeschalteten Felder sind standardmäßig leer. Das kann bei der Prüfung Fehler verursachen.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3117_

#### Aggregate – Allgemein

**Kapazitätsplanung > Stammdaten > Organisation > Aggregate > Register Allgemein**

**Abbildung H-135: Aggregate - Allgemein**

\[Image of the "Aggregate - Allgemein" dialog for a cutting machine]

In diesem Register legen Sie die Maschinen (Aggregate) an, die Sie nutzen und die für die Kapazitätsplanung relevant sind. Sie sollten auch ein Aggregat Versand anlegen, damit die Zeiten dafür geplant werden können. ⇨ Tutorial, "Aggregattypen und Aggregate" auf Seite H-2932

**Aggregat**

**Nr./Bezeichnung** Nummer (ID) und Beschreibung können frei gewählt werden. Wir empfehlen, ähnliche Maschinen in Nummernkreisen zu gruppieren, z. B. Schneidtische 100-199, Bohrmaschinen 400-499 usw.

**Typ** Aggregat-Typ, zu dem die Maschine gehört. Durch die Zuweisung werden die Felder für die Restriktionsprüfungen freigeschaltet. ⇨ "Aggregattypen" auf Seite H-3104

**Produktionsbereich** Produktionsbereich, in dem die Maschine steht. ⇨ "Produktionsbereich" auf Seite H-3115

***

### _H-3118_ _A+W Business Pro Kapazitätsplanung_

**Optionen**

**Scheiben drehbar** Angabe, ob die Scheiben auf der Maschine gedreht werden können.

* ☐ Die Scheiben können nicht gedreht werden.
* ☑ Die Scheiben können gedreht werden.

**Kantenschutz möglich** Angabe, ob auf der Maschine Kantenschutz angebracht werden kann.

* ☐ Kantenschutz kann nicht angebracht werden.
* ☑ Kantenschutz kann angebracht werden.

**Autobrechen** Angabe, ob der Zuschneidetisch über eine automatische Brechvorrichtung verfügt.

* ☐ Der Tisch hat keine automatische Brechvorrichtung.
* ☑ Die Scheiben können automatisch gebrochen werden.

**Modelle möglich** Angabe, ob auf der Maschine Modelle (nicht-rechteckige Scheiben) gefertigt werden können.

* ☐ Modelle sind nicht möglich.
* ☑ Modelle sind möglich.

**Sprossen möglich** Angabe, ob auf der Maschine Sprossen gefertigt werden können.

* ☐ Sprossen sind nicht möglich.
* ☑ Sprossen sind möglich.

**VSG** Angabe, ob auf den Zuschneidetisch auch VSG geschnitten werden kann.

* ☐ Der Tisch kann keine VSG-Scheiben schneiden.
* ☑ Der Tisch kann VSG-Scheiben schneiden.

**Gasfüllung möglich** Angabe, ob auf der Maschine Gasfüllungen möglich sind.

* ☐ Gasfüllungen sind nicht möglich.
* ☑ Gasfüllungen sind möglich.

**Autoaufleger** Angabe, ob der Zuschneidetisch über einen automatischen Aufleger verfügt.

* ☐ Der Tisch hat keinen automatische Aufleger.
* ☑ Der Tisch hat einen automatischen Aufleger. In diesem Fall muss für jede Lagerplatte, die auf diesem Tisch zugeschnitten wird, ein Auflegercode vergeben werden.

**Entschichten** Angabe, ob auf der Maschine Scheiben randentschichtet werden können.

* ☐ Randentschichtungen sind nicht möglich.
* ☑ Randentschichtungen sind möglich.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3119_

**Zuschnitt Tisch**

Auswahl der Nummer von Zuschnitt-Tischen. Diese Einstellung wird bei A+W Business Pro nicht angezeigt.

**Zusatz-Optionen**

Diese Einstellungen gelten nur für A+W Business Pro.

**Ausgabeverzeichnis** Auswahl des Speicherorts für Ausgabedatei.

**Maschinencode** Auswahl des Maschinencodes. Die Maschinencodes sind im gleichnamigen Dialog hinterlegt. Wenn der gesuchte Code fehlt können Sie ihn in diesem Dialog anlegen.

**ISO-Treiber, ISO-Sektion** Die Felder werden gefüllt, wenn der Maschinencode für eine ISO-Linie ausgewählt ist.

**Schlüsselwort** Schlüsselwort, mit dem das Aggregat im System eindeutig identifiziert wird. Das Feld wird nach Auswahl des Maschinencodes automatisch gefüllt.

**Kostenfaktor Z-Schnitt** Angabe zur Preiserhöhung von Z-Schnitten. Der Faktor 1 bedeutet, dass der Preis für den Schnitt nicht erhöht wird. Faktor 1,5 erhöht den Preis um die Hälfte.

**Z-Schnitt** Die Angabe bestimmt die Lage der Z-Schnitte im Schneidemodus.

* **(\<k.A.>):** Keine Angaben.
* **oben:** Normalerweise ist es günstiger, die Z-Schnitte nach oben, also weg von der Arbeitsbreite zu legen, damit einzelne Schnitte zunächst über die ganze Breite gebrochen und gleich abgestellt werden können. Weisen darüber liegende Scheiben Z-Schnitte auf, ist dann bereits Platz auf dem Brechtisch, um die Scheibe zum Brechen des Z-Schnitts zu drehen.
* **unten:** Der Startpunkt liegt oben
* **beliebig:** Der Startpunkt kann beliebig gewählt werden.

**Referenzpunkt** Auswahl des Referenzpunkts für den Schneidmodus. Der Referenzpunkt des Tisches bezeichnet den Punkt mit den Koordinaten 0/0, von dem aus der Schneidmodus aufgebaut ist. Er ist wichtig, um Modelle korrekt zu schneiden.

> **Referenzpunkt vs. Ruheposition des Schneidkopfes** Der Referenzpunkt muss nicht mit der Ruheposition des Schneidkopfes übereinstimmen. Bei Bystronic gibt es z. B. gespiegelte Tische, deren Referenzpunkt links vorne ist, während der Schneidkopf rechts vorne in Ruheposition steht. Bei manchen Tischen kann dies als Parameter eingestellt werden.

***

### _H-3120_ _A+W Business Pro Kapazitätsplanung_

**Schneidmodus** Angabe, in welcher Reihenfolge die Schnitte ausgeführt werden:

* **1 - XYZW:** Der erste Schnitt verläuft senkrecht zum unteren Plattenrand. Danach folgen der Y-Schnitt und der Z-Schnitt. Die weitere Reihenfolge ist wahlweise.
* _2 - XYZ:_\* Wie 1. Nach dem Z-Schnitt folgt ein beliebiger anderer Schnitt.
* **3 - XYZZZ:** Der erste Schnitt verläuft senkrecht zum unteren Plattenrand. Danach folgen der Y-Schnitt und anschließend die Z-Schnitte.
* **4 - XYZZ:** Wie 3. Jedoch sind nur zwei Z-Schnitte möglich.

**Abbildung H-136: XYZ-Schnitte auf der Lagerplatte** \[Image showing X, Y, and Z cuts on a glass plate]

**Brechstart** Auswahl des Brechstarts. Der Brechbeginn richtet sich nach den räumlichen Bedingungen im Betrieb und bestimmt die Lager der Restplatte sowie in gewissem Maße die Zuschnittsreihenfolge (erste zu brechende Scheibe oben oder unten).

**Werte**

**Einheiten pro Stunde** Der Wert in diesem Feld hängt davon ab, in welcher Arbeitseinheit die Kapazitätsplanung für diese Maschine die Kapazität berechnen soll, ob in Mannstunden oder Maschinenstunden. Standardmäßig wird 1 eingetragen. ⇨ Tutorial, "Arbeitseinheiten" auf Seite H-2950

**Lohnkosten pro Einheit** Die einzutragenden Personalkosten hängen davon ab, in welcher Arbeitseinheit die Kapazitätsplanung für diese Maschine die Kapazität berechnen soll, z. B. in Mannstunden oder Maschinenstunden. Sie finden eine ausführliche Erläuterung zu diesem Thema unter: ⇨ Tutorial, "Arbeitseinheit = Mannstunde" auf Seite H-2951

**Maschinenkosten pro Stunde** Maschinenkosten pro Stunde, z. B. für Wartung, Reparatur, Verbrauchsmittel.

**Variable Kosten pro Stunde** Sonstige Kosten, die weder zu Lohn- noch zu Maschinenkosten zählen, können in die Produktionskosten eingerechnet werden, z. B. Versicherung. Den Gesamtbetrag der Versicherung Sie müssen pro Stunde umrechnen.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3121_

**Kosten pro Einheit** Berechnete Gesamtkosten pro Einheit für diese Maschine. Sie bilden die Grundlage für die Kostenkalkulation. Die Kosten werden auf Basis von Personal-, Maschinen- und variablen Kosten und der Arbeitseinheit pro Stunde berechnet.

> **Beispiel** Personalkosten/Stunde + Maschinenkosten/Stunde dividiert durch Einheiten/Stunde + Variable Kosten/Stunde dividiert durch Einheiten/Stunde = Kosten/Einheit

**Erfassungsstelle** Nummer der Erfassungsstelle (Maschine) in A+W Production, auf die sich das Aggregat bezieht. Die Nummern müssen in A+W Business Pro und A+W Production identisch sein. Wenn Sie mit der BDE (Scanner) arbeiten, muss die Nummer der Erfassungsstelle gescannt werden.

**Leistung pro Stunde** Durchschnittliche Soll-Vorgaben (Erfahrungswerte oder Information des Maschinen-Herstellers) in Mengeneinheiten. Diese Angabe nutzen Sie, wenn Sie z. B. alle Stammdaten bis auf die Vorgabezeiten erfasst haben und vorab in die Kapazitätsplanung einlasten möchten, um die Kapazität in Ihrer Produktion in etwa abschätzen zu können. Damit können Sie den Zeitraum überbrücken, bis alle Vorgabezeiten erfasst sind.

**Serientabelle** Auswahl der Serientabelle, in der die speziellen Zeiten für Serien definiert sind. ⇨ "Serienfaktoren" auf Seite H-3111

**Default-Rückschnitt** Maße für den Rückschnitt pro Kante in mm. Der Rückschnitt beschreibt den einfachen Abstand zwischen Glasaußenkante und Rahmeninnenkante. Dieses Feld ist nur freigeschaltet, wenn im Bereich Optionen die Checkbox Entschichten aktiviert ist.

**Sperre**

**Aggregat gesperrt** Das Aggregat kann für die Planung gesperrt werden.

* ☐ Das Aggregat ist nicht gesperrt.
* ☑ Das Aggregat ist gesperrt und kann nicht in die Planung einbezogen werden. Diese Einstellung wählen Sie z. B., wenn eine neue Maschine zunächst getestet werden soll, bevor sie tatsächlich eingesetzt wird. Wenn Sie eine Maschine wegen einer notwendigen Wartung vorübergehend sperren wollen, wählen Sie den Dialog **Aggregat Ausfall**: ⇨ "Aggregate Ausfall" auf Seite H-3218

**Sperrformel** Über eine Sperrformel können Sie weitere Restriktionen hinterlegen, die mit den Standard-Mitteln nicht zu erreichen sind.

***

### _H-3122_ _A+W Business Pro Kapazitätsplanung_

> **Beispiel** Auf einem Aggregat dürfen nur Modelle, sehr kleine und sehr große Scheiben gefertigt werden, da diese Maschine sehr langsam ist.
>
> Alle Rechteckscheiben mit einer Breite >200 und <2600 sowie einer Höhe >300 und <3600 dürfen nicht auf dieser Maschine geschnitten werden.
>
> Diese Restriktion kann nur über eine Formel angegeben werden. Falls Sie Formeln einsetzen wollen, wenden Sie sich an Ihren Service-Mitarbeiter bei der A+W Software GmbH.

**Zus. Arbeitsart bei gekoppelten Maschinen** Zurzeit nicht genutzt.

**Tabelle**

In der Übersicht werden je nach Auswahlkriterien die Maschinen aufgeführt, die der Kapazitätsplanung zur Verfügung stehen.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3123_

#### Aggregate – Restriktionen

**Kapazitätsplanung > Stammdaten > Organisation > Aggregate > Register Restriktionen**

**Abbildung H-137: Aggregate - Technische Restriktionen**

\[Image of the "Aggregate - Restriktionen" dialog]

In diesem Register hinterlegen Sie Mindest- und Höchstwerte für die Restriktionsprüfungen. Geben Sie jeweils 0 bis 9999 ein, wenn alle Werte zugelassen sind.

Die Felder für die Definition von Restriktionen werden im Dialog **Aggregattypen** freigeschaltet. ⇨ "Aggregattypen" auf Seite H-3104

Wenn die technischen Restriktionen für eine Maschine bei gleichen Arbeitsarten verschieden sind, definieren Sie diese Restriktionen im Dialog **Besondere technische Restriktionen**. Die Kapazitätsplanung prüft den Eintrag im Dialog **Besondere technische Restriktionen** zuerst. ⇨ "Besondere technische Restriktionen" auf Seite H-3136

Die Felder im Bereich **Aggregat** sind zum Register **Allgemein** beschrieben. ⇨ "Aggregate - Allgemein" auf Seite H-3118

***

### _H-3124_ _A+W Business Pro Kapazitätsplanung_

**Arbeitsarten / Zeitzuschläge**

In diesem Bereich werden alle Arbeitsarten aufgelistet, für die Vorgabezeiten an dieser Maschine definiert sind. ⇨ "Vorgabezeiten (Dialog)" auf Seite H-3141

**Technische Restriktionen**

Die Felder für die Definition von Restriktionen werden im Dialog **Aggregattypen** freigeschaltet. ⇨ "Aggregattypen" auf Seite H-3104

Geben Sie **0** oder **9999** ein, wenn alle Werte zugelassen sind.

**Breite, Höhe** Min. und max. Scheibenmaße für diese Maschine.

**SZR** Min. und max. SZR für diese Maschine.

**Gesamtstärke** Min. und max. Gesamtdicke für ISO und VSG.

**Glasstärke** Min. und max. Dicke von Einfachglas.

**Diagonale** Diagonale zwischen den Rollen, z. B. auf dem Förderband vor dem ESG-Ofen.

**Scheibenanzahl** Maximale Anzahl der Scheiben für eine VSG- bzw. ISO-Einheit, z. B. 3 auf einer ISO-Linie.

**Fläche in qm** Min. und max. Fläche für diese Maschine.

**Gehrungswinkel** Min. und max. Gehrungswinkel für Facetten.

**Anzahl** Min. und max. Stückzahl der Auftragsposition. In der Position muss die Menge oder der Mengenbereich geprüft werden. Die Definition, um welche Anzahl es sich handelt, ist maschinenabhängig, z. B.

* Bohrmaschine = Anzahl Bohrlöcher
* Schleifmaschine = Anzahl der Kanten

**Bohrdurchmesser** Min. und max. Abmessung für diese Maschine.

**Rundeck-Radius** Min. und max. Abmessung für diese Maschine.

**Seitenverhältnis** Maximales Seitenverhältnis für diese Maschine.

> **Beispiel** Sie geben den Wert 5 ein. Dies entspricht einem max. Seitenverhältnis von 1:5. Wenn eine Seite z. B. 500 mm lang ist, dann darf die andere Seitenlänge max. 2500 mm betragen.

**Gewicht bis kg** Maximales Gewicht einer Einheit.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3125_

**Abstände zwischen Schnitten**

Bei Schneidtischen mit einer automatischen Brechanlage müssen Sie die Höchst- und Mindestabstände zwischen den Schnitten einstellen. Diese Abstände müssen eingehalten werden, damit die Anlage die Schreiben noch brechen kann.

**Min. Abs. X-X mit Y** Minimaler Abstand zwischen X-X-Schnitten wenn auch Y-Schnitte ausgeführt werden.

**Min. Abs. X-X ohne Y** Minimaler Abstand zwischen X-X-Schnitten wenn keine Y-Schnitte ausgeführt werden.

**Max. Abs. X-X** Maximaler Abstand zwischen X-X-Schnitten.

**Min. Abs. Y-Y mit Z** Minimaler Abstand zwischen Y-Y-Schnitten wenn auch Z-Schnitte ausgeführt werden. Bei Schneidetischen mit mehreren Y-Schneidköpfen entspricht der Minimalabstand der Entfernung der Schneidrädchen zweier unmittelbar gegeneinander geschobener Schneidköpfe, z. B. Bystronic XYZVA = 300 mm.

**Min. Abs. Y-Y ohne Z** Minimaler Abstand zwischen Y-Y-Schnitten wenn keine Z-Schnitte ausgeführt werden.

**Max. Abs. Y-Y** Maximaler Abstand zwischen Y-Y-Schnitten.

**Min. Restbreite** Minimale Breite am Rand der Platte.

**Min. Abs. X-Z** Minimaler Abstand zwischen X und Z-Schnitten.

**Min. Abs. Z-Z** Minimaler Abstand zwischen Z-Schnitten.

**Toleranz für Min. Abs. X-X, Y-Y** Sie können einstellen, dass die minimalen Abstände der X-X-Schnitte und/oder Y-Y-Schnitte ignoriert werden, wenn eine Scheibe die Restriktionen verletzt.

* ☑ Die Mindestabstände werden eingehalten.
* ☐ Die Mindestabstände werden ignoriert.

**Toleranz für Max. Abs. X-X, Y-Y** Sie können einstellen, dass die maximalen Abstände der X-X-Schnitte und/oder Y-Y-Schnitte ignoriert werden, wenn eine Scheibe die Restriktionen verletzt.

* ☑ Die Maximalabstände werden eingehalten.
* ☐ Die Maximalabstände werden ignoriert.

> **Toleranz kann zu Problemen führen** Standardmäßig werden Scheiben, die die Restriktionen verletzen, nicht optimiert. Wenn Sie die Toleranz aktivieren, werden die markierten Restriktionen ignoriert und die Scheibe durchläuft die Optimierung. Wählen Sie eine Toleranz nur nach Rücksprache mit der A+W Software GmbH aus. Eine Änderung kann zu Fehlproduktionen oder Stillständen in der Produktion führen.

***

### _H-3126_ _A+W Business Pro Kapazitätsplanung_

### Kalender

**Kapazitätsplanung > Stammdaten > Organisation > Kalender**

In diesem Dialog legen Sie die Arbeitstage und Schichtzeiten fest. Die Daten können nur gespeichert werden, wenn mindestens eine Schicht angelegt ist. Die Anzahl der Schichten wird in den Firmendaten festgelegt. ⇨ "Voreinstellungen Firmendaten" auf Seite H-3098

Wenn keine Kalender in der Kapazitätsplanung angelegt sind, benutzt die Kapazitätsplanung den A+W Business Pro-Standard-Kalender.

Standardmäßig geht die Kapazitätsplanung von einer Schicht aus. Wenn Sie jedoch in Ihrem Betrieb mit mehr als einer Schicht arbeiten, müssen Sie als ersten Schritt die Anzahl der Schichten festlegen. Erst dann legen Sie Kalender für Maschinen mit abweichenden Schichten und Schichtzeiten an.

> **Beispiel** Der Kalender lässt maximal 6 Schichten pro Tag zu. Daraus resultieren bei gleichmäßiger Verteilung der Stunden maximal 4 Stunden pro Schicht. Die Verteilung der Anzahl der Stunden pro Schicht ist jedoch variabel, z. B. 5, 3, 5, 3, 5, 3 oder 4, 2, 6, 6, 3, 3. Mit diesen Beispielen soll verdeutlicht werden, dass Sie nicht an eine gleichmäßige Verteilung gebunden sind. Bei 4 Schichten können Sie bei gleichmäßiger Verteilung pro Schicht maximal 6 Stunden eintragen. Die Gesamtzeit der Stunden x Schichten pro Tag darf logischerweise 24 Stunden nicht überschreiten.

> **Kalender ändern** Wenn Sie einen Kalender bearbeitet oder angelegt haben, müssen Sie A+W Business Pro neu starten, damit die Daten beim Einlasten zur Verfügung stehen.

In diesem Dialog finden Sie folgende Register:

* "Kalender - Auswahl" auf Seite H-3129
* "Kalender - Kalender" auf Seite H-3131

***

### _A+W Business Pro Kapazitätsplanung_ _H-3127_

#### Menü Funktionen

**Kapazitätsplanung > Stammdaten > Organisation > Kalender > Menü Funktionen**

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Kalender zu schließen.

Folgende Einträge werden angezeigt:

* **Kopieren:** Öffnet den Dialog Kalender kopieren, um einen Kalender zu übertragen, z. B. in ein neues Jahr. ⇨ "Kalender kopieren" auf Seite H-3133
* **Schichtzeiten:** Öffnet den Dialog Einstellung Schichten, in dem Sie den Schichtübergang und die Sperrzeiten festlegen können. ⇨ "Einstellungen Schichten" auf Seite H-3102 Sie müssen Administratorrechte haben, um den Dialog zu öffnen. Zusätzlich muss in den Firmendaten die Checkbox Schichtwechseltabelle verwenden markiert sein. ⇨ "Schichtwechseltabelle verwenden" auf Seite H-3102

***

### _H-3128_ _A+W Business Pro Kapazitätsplanung_

#### Kalender – Auswahl

**Kapazitätsplanung > Stammdaten > Organisation > Kalender > Register Auswahl**

**Abbildung H-138: Kalender - Auswahl** \[Image of the Calendar selection dialog showing modes for "Arbeitsart/Aggregat" and "Produktionsbereich/Mandant"]

In diesem Register legen Sie Kalender für Arbeitsarten, Aggregate, Produktionsbereiche oder Mandanten an. Wenn Sie für einen Produktionsbereich oder ein Aggregat keinen eigenen Kalender anlegen, gilt der allgemeine Kalender. ⇨ Tutorial, "Kalender anpassen" auf Seite H-2957

**Identifikation**

Die Beschriftung der beiden Auswahlfelder richtet sich nach dem gewählten Modus.

**Arbeitsart, Aggregat** Arbeitsart und Maschine, für die der Kalender gilt.

**Produktionsbereich, Mandant** Produktionsbereich und Mandant, für die der Kalender gilt.

**Jahr** Jahr, für das der Kalender bearbeitet oder angelegt werden sollen.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3129_

**Modus**

Mit der Wahl der Option legen Sie fest, wofür Sie den Kalender anlegen wollen. Die Felder sind nur im Auswahlmodus freigeschaltet.

* **Arbeitsart, Aggregat:** Mit dieser Einstellung legen Sie einen Kalender für die Arbeitsart und/oder die Maschine an.
* **Produktionsbereich/Mandant:** Mit dieser Einstellung legen Sie einen Kalender für den Produktionsbereich und/oder den Mandanten an. Um einen allgemeinen Kalender anzulegen, wählen Sie diese Option und tragen den Produktionsbereich \<k. A.> und für den Mandanten alle ein.

**Kalender-Tabellen**

In der Übersicht werden alle Kalender angezeigt, die den Auswahlkriterien entsprechen. Wenn Sie die Auswahl nur nach dem Modus Arbeitsart oder Produktionsbereich eingegrenzt haben, werden alle Kalender angezeigt.

***

### _H-3130_ _A+W Business Pro Kapazitätsplanung_

#### Kalender – Kalender

**Kapazitätsplanung > Stammdaten > Organisation > Kalender Aggregat > Register Kalender**

**Abbildung H-139: Kalender - Kalender** \[Image of the calendar setup dialog showing weekdays with hours per shift and a monthly calendar view]

In diesem Register legen Sie die Arbeitszeit pro Schicht fest. Die Anzahl der Schichten wird in den Firmendaten angegeben. ⇨ "Voreinstellungen Firmendaten" auf Seite H-3098

**Arbeitswoche**

**Montag - Sonntag** Wenn Sie die Schichtzeit eines Wochentags ändern wollen, dann müssen Sie die entsprechende Checkbox aktivieren und die neue Stundenzahl eintragen. Die Änderung gilt nur für das angezeigte Datum. Sie müssen die neue Schichtzeit ggf. auf das Jahr oder die Kalenderwoche übertragen.

**Stunden pro Schicht** Anzahl der verfügbaren Stunden pro Wochentag und Schicht.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3131_

> **Zusätzliche Schicht einrichten** Wenn Sie eine zusätzliche Schicht für ein Aggregat oder einen Produktionsbereich einrichten, müssen Sie alle Schichtzeiten neu eintragen. Es reicht nicht, nur die Stunden der neuen Schicht anzugeben, weil bei der Übertragung auf das Jahr (oder die Woche) die leeren Felder ebenfalls übernommen werden. Damit sind die alten Schichtzeiten gelöscht.

**Schichten in Kalender übernehmen**

**\[Auf Jahr übertragen]** Überträgt die Änderungen auf alle entsprechenden Wochentage des Jahres. Nur die Schichtzeiten der Wochentage werden übertragen, bei denen die Checkbox markiert ist.

**\[Auf KW übertragen]** Überträgt die Änderungen auf alle Tage der Kalenderwoche.

**Kalenderwoche**

**Gehe zu** Auswahl der Kalenderwoche.

**\[Zur aktuellen KW]** Wechselt die Darstellung im Bereich **Arbeitswoche**, um die Schichtzeiten für die aktuelle Kalenderwoche zu bearbeiten.

**Kalender**

In der Übersicht werden die ausgewählten Tage der Arbeitswoche mit den jeweiligen Schichtzeiten angezeigt.

***

### _H-3132_ _A+W Business Pro Kapazitätsplanung_

### Kalender kopieren

**Kapazitätsplanung > Stammdaten > Organisation > Kalender > Menü Funktionen > Kopieren**

**Abbildung H-140: Kalender kopieren** \[Image of the "Kalender kopieren" dialog]

In diesem Dialog kopieren Sie den Kalender eines Aggregats oder eines Produktionsbereichs, z. B. um ihn auf ein anderes Aggregat zu übertragen.

#### Kalender Auswahl Quelle

Die Beschriftung der beiden Auswahlfelder richtet sich nach dem gewählten Modus.

**Arbeitsart, Aggregat** Arbeitsart und Maschine, für die der Kalender angelegt ist.

**Produktionsbereich, Mandant** Produktionsbereich und Mandant, für die der Kalender angelegt ist.

**Jahr** Jahr, für das der Kalender angelegt ist.

#### Kalender Auswahl Ziel

**Arbeitsart, Aggregat** Arbeitsart und Aggregat, auf die der Kalender übertragen werden soll.

**Produktionsbereich, Mandant** Produktionsbereich und Mandant, auf die der Kalender übertragen werden soll.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3133_

### Übergangsmatrix

**Kapazitätsplanung > Stammdaten > Organisation > Übergangsmatrix**

**Abbildung H-141: Übergangs-Matrix**

| Auftragspriorität | von Produktionsbereich            | nach Produktionsbereich              | Übergangszeit |
| ----------------- | --------------------------------- | ------------------------------------ | ------------- |
| Normal            | 0010 - Zuschnitt / Cutting        | 0020 - Bearbeitung / Processing      | 0             |
| Normal            | 0040 - ESG Fertigung / TG Prod... | 0080 - ISO Fertigung / IG Production | 2             |
| Normal            | 0040 - ESG Fertigung / TG Prod... | 0900 - Versand / Shipping            | F(500)        |

In diesem Dialog tragen Sie ein, wie lange es dauert, bis die Position von einem Produktionsbereich in den nächsten gelangt. Die Zeiten können Sie je nach Auftragspriorität unterschiedlich gestalten.

> **Beispiel** Der Übergang vom Produktionsbereich Zuschnitt in den Produktionsbereich Bearbeitung kann normalerweise in der gleichen Schicht erfolgen. Der Übergang vom Produktionsbereich ESG in den Produktionsbereich ISO-Fertigung benötigt mehrere Schichten bzw. 1 Tag.

⇨ Tutorial, “Übergangsmatrix und Übergangszeiten" auf Seite H-2977

**Auftragspriorität** Auswahl, bei welcher Auftragspriorität die Übergangszeit berücksichtig werden soll. Sie können zwischen folgenden Prioritäten wählen:

* **Normal:** Die Übergangszeit gilt für alle Aufträge, in denen keine besondere Priorität angegeben ist. Dies ist die Standard-Einstellung.
* **Eilt:** Die angegebene Übergangszeit gilt für Eilaufträge. Wenn Übergangszeiten für Eilaufträge verkürzt werden können, dann muss für die entsprechende Kombination von Produktionsbereichen eine abweichende Übergangszeit hinterlegt werden.
* **Zugabe:** Diese Priorität bedeutet, dass der Auftrag so gefertigt werden soll, dass er Reste und Restplatten verbraucht, die beim Zuschnitt anderer Aufträge entstehen.

***

### _H-3134_ _A+W Business Pro Kapazitätsplanung_

* **Abruf:** Die Übergangzeit gilt nur für Aufträge, die auf Abruf gefertigt werden.

> **Auftragspriorität berücksichtigen** Wenn außer der Auftragspriorität Normal auch z. B. die Priorität Eilt berücksichtigt werden soll, dann muss für die jeweilige Kombination von Produktionsbereichen eine eigene Übergangszeit eingerichtet sein. Dies gilt für alle Übergangszeiten, die für Eilaufträge auch verkürzt werden können.

**Von Produktionsbereich** Produktionsbereich, aus dem die Position kommt.

**Nach Produktionsbereich** Folge-Produktionsbereich, in den die Position wechselt.

**Übergangszeit** Zeit, die ein Glas zum Wechsel in den nächsten Produktionsbereich braucht. Die Werte werden in Tagen eingegeben:

* 0 = gleicher Tag bzw. gleiche Schicht
* 0,01 bis 0,99 = Folgeschichten
* 1 = Folgender Tag

#### Beispiele für die Berechnung des Übergangs

**Tab. H-4: Übergangszeiten in Tagen**

| Anz. Schichten | 1/Anzahl Stunden | Gleiche Schicht | Nächste Schicht | z.B. | Übernächste S. | z.B. | Über-Über-nächste S. | z.B. | Über-Über-Über-nächste S. | z.B. |
| -------------- | ---------------- | --------------- | --------------- | ---- | -------------- | ---- | -------------------- | ---- | ------------------------- | ---- |
| **4**          | 1/4=0,25         | 0               | 0,1-0,24        | 0,2  | 0,26-0,49      | 0,4  | 0,51-0,74            | 0,6  | 0,76-1                    | 1    |
| Übergang:      |                  | S1-Mo           | S2-Mo           |      | S3-Mo          |      | S4-Mo                |      | S1-Di                     |      |
| Übergang:      |                  | S2-Mo           | S3-Mo           |      | S4-Mo          |      | S1-Di                |      | S2-Di                     |      |
| **3**          | 1/3=0,33         | 0               | 0,1-0,3         | 0,2  | 0,4-0,6        | 0,5  | 0,7-1                | 1    | -                         | -    |
| Übergang:      |                  | S1-Mo           | S2-Mo           |      | S3-Mo          |      | S1-Di                |      | -                         | -    |
| Übergang:      |                  | S2-Mo           | S3-Mo           |      | S1-Di          |      | S2-Di                |      | -                         | -    |
| **2**          | 1/2=0,5          | 0               | 0,1-0,49        | 0,3  | 0,51-0,1       | 1    | -                    | -    | -                         | -    |
| Übergang:      |                  | S1-Mo           | S2-Mo           |      | S1-Di          |      | -                    | -    | -                         | -    |
| Übergang:      |                  | S2-Mo           | S1-Di           |      | S2-Di          |      | -                    | -    | -                         | -    |

> **Flexible Übergangszeit** Sie können statt eines festen Wertes auch eine Formel eintragen, wenn die Übergangszeit von unterschiedlichen Parametern abhängt, z. B. von der Dicke. Mit einem Rechtsklick in das Feld wird der Dialog **Formelsuche** geöffnet. Wenn Sie mit Formeln arbeiten wollen, lassen Sie sich von Ihrem Service-Mitarbeiter bei der A+W Software GmbH unterstützen.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3135_

### Besondere technische Restriktionen

**Kapazitätsplanung > Stammdaten > Organisation > Besondere technische Restriktionen**

**Abbildung H-142: Besondere technische Restriktionen** \[Image of the "Bes. techn. Restriktionen" dialog]

In diesem Dialog geben Sie Restriktionen für Aggregate an, die sich auf bestimmte Arbeitsarten beziehen. Wenn auf einer Maschine unterschiedliche Arbeitsarten ausgeführt werden können, z. B. Lochbohren und Eckausschnitt, können Sie pro Arbeitsart unterschiedliche Prüfwerte angeben. Wenn die Kapazitätsplanung keine Definition für die Arbeitsart findet, werden die allgemeinen technischen Restriktionen für diese Maschine geprüft. ⇨ "Aggregate - Restriktionen" auf Seite H-3124

Die verfügbaren Parameter sind abhängig von den Einstellungen im Dialog **Aggregattypen**. ⇨ "Aggregattypen" auf Seite H-3104

#### Menü Funktionen

Über dieses Menü können Sie die Werte aus dem Standard-Aggregat übertragen. Bereits eingetragene Werte werden ohne Abfrage überschrieben. ⇨ "Aggregate – Restriktionen" auf Seite H-3124

#### Identifikation

**Arbeitsart** Arbeitsart, für die die Restriktionen gelten.

***

### _H-3136_ _A+W Business Pro Kapazitätsplanung_

**Aggregat** Maschine, für die die Restriktionen gelten, wenn die entsprechende Arbeitsart ausgeführt wird.

#### Technische Restriktionen (Minimal/Maximal)

Geben Sie 0 oder 9999 ein, wenn alle Werte zugelassen sind.

**Breite, Höhe** Min. und max. Maße für diese Maschine.

**SZR** Min. und max. SZR für diese Maschine.

**Gesamtstärke** Min. und max. Gesamtdicke für ISO und VSG für diese Maschine.

**Glasstärke** Min. und max. Dicke von Einfachglas.

**Anzahl** Min. und max. Stückzahl der Auftragsposition. In der Position muss die Menge oder der Mengenbereich geprüft werden. Die Definition, um welche Anzahl es sich handelt, ist maschinenabhängig, z. B.

* Bohrmaschine = Anzahl Bohrlöcher
* Schleifmaschine = Anzahl der Kanten

**Bohrdurchmesser** Min. und max. Abmessung für diese Maschine.

**Rundeck-Radius** Min. und max. Abmessung für diese Maschine.

**Fläche in qm** Min. und max. Fläche für diese Maschine.

**Diagonale** Diagonale zwischen den Rollen, z. B. auf dem Förderband vor dem ESG-Ofen.

**Gehrungswinkel** Min. und max. Gehrungswinkel für Facetten.

#### Sonstige technische Restriktionen

Geben Sie 9999 ein, wenn alle Werte zugelassen sind.

**Serien-Tabelle** Nummer der Serientabelle, die bei der Produktion von Serien herangezogen wird. ⇨ Softwarereferenz, "Serienfaktoren" auf Seite H-3111

**Max. Scheibenanzahl** Maximale Anzahl an Scheiben, die für eine VSG- bzw. ISO-Einheit auf dieser Maschine erlaubt sind.

**Gewicht bis kg** Maximales Gewicht.

**Max. Seitenverhältnis** Maximales Seitenverhältnis für diese Maschine.

> **Beispiel** Der Wert 5 entspricht einem max. Seitenverhältnis von 1:5. Wenn eine Kantenlänge der Scheibe z. B. 500 mm beträgt, dann darf die andere Kante max. 2500 mm lang sein.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3137_

#### Technische Restriktionen (Optionen)

**Modelle möglich** Angabe, ob auf der aktuellen Maschine Modelle gefertigt werden können.

* ☐ Modelle sind nicht möglich.
* ☑ Modelle sind möglich.

**Sprossen möglich** Angabe, ob auf der aktuellen Maschine Sprossen gefertigt werden können.

* ☐ Sprossen sind nicht möglich.
* ☑ Sprossen sind möglich.

**Gasfüllung möglich** Angabe, ob auf der aktuellen Maschine Gasfüllungen möglich sind.

* ☐ Gasfüllungen sind nicht möglich.
* ☑ Gasfüllungen sind möglich.

**Scheiben drehbar** Angabe, ob die Scheiben auf der aktuellen Maschine gedreht werden können.

* ☐ Scheiben können nicht gedreht werden.
* ☑ Scheiben können gedreht werden.

**Kantenschutz möglich** Angabe, ob auf der aktuellen Maschine Kantenschutz angebracht werden kann.

* ☐ Kantenschutz kann nicht angebracht werden.
* ☑ Kantenschutz kann angebracht werden.

#### Übersicht Sonder-Restriktionen

In der Übersicht sind die Arbeitsarten und Maschinen aufgeführt, für die besondere Restriktionen hinterlegt sind.

***

### _H-3138_ _A+W Business Pro Kapazitätsplanung_

### Orga Übersicht

**Kapazitätsplanung > Stammdaten > Organisation > Orga Übersicht**

**Abbildung H-143: Orga Übersicht** \[Image of the "Orga Übersicht" dialog, showing a hierarchical view of Produktionsbereich -> Aggregat -> Arbeitsart -> Zuschläge]

In diesem Dialog prüfen Sie, welche Maschinen und Arbeitsarten den Produktionsbereichen zugeordnet sind.

#### Auswahl

**Mandant** Mandant, dem der Produktionsbereich zugeordnet ist.

**Produktionsbereich** Produktionsbereich, dem die Aggregate zugeordnet sind.

#### Auflösungstiefe

Mit der Wahl der Option filtern Sie die Anzeige in der Übersicht.

#### Ansicht

Die Spalten in der Übersicht sind abhängig von der Auflösungstiefe.

* **Produktionsbereich:** Produktionsbereich, dem das Aggregat (die Maschine) zugeordnet ist.
* **Aggregat:** Aggregate, die dem jeweiligen Produktionsbereich zugeordnet sind.
* **Arbeitsart:** Arbeitsarten, die dem jeweiligen Aggregat zugeordnet sind.
* **Zuschläge:** Typ der Vorgabezeit, die für die jeweilige Arbeitsart zur Berechnung herangezogen werden.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3139_

## Vorgabezeiten

**Kapazitätsplanung > Stammdaten > Vorgabezeiten**

In diesem Programmbereich finden Sie die Dialoge, in denen die Vorgaben für die Zeitberechnung hinterlegt sind.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:

* "Vorgabezeiten (Dialog)" auf Seite H-3141
* "Vorgabezeiten ändern" auf Seite H-3149
* "Vorgabezeiten kopieren" auf Seite H-3149
* "Sonderzeiten" auf Seite H-3150
* "Besondere Prioritäten" auf Seite H-3151

***

### _H-3140_ _A+W Business Pro Kapazitätsplanung_

### Vorgabezeiten (Dialog)

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten**

In diesem Dialog tragen Sie die für Ihre Maschinen ermittelten Zeitwerte pro Arbeitsart und Maschine ein. Ob der Zeitwert abhängig von laufenden Metern, Quadratmetern oder Stück berechnet wird, hängt von der Maschine ab.

In diesem Dialog finden Sie folgende Register:

* "Vorgabezeiten – Zeitauswahl" auf Seite H-3142
* "Vorgabezeiten – Matrix" auf Seite H-3145
* "Vorgabezeiten – Vektor" auf Seite H-3147
* "Vorgabezeiten – Würfel" auf Seite H-3148

#### Eintrag von Zeitwerten in Stunden

Die Zeiten werden nicht in Minuten, sondern in Stunden hinterlegt. Das heißt, dass Sie die gemessenen Minuten in Stunden umrechnen müssen:

| Minuten | Zeiteintrag in Std. |
| ------- | ------------------- |
| 60      | 1                   |
| 30      | 0,5                 |
| 15      | 0,25                |
| 7,5     | 0,125               |
| 3,75    | 0,0625              |
| 1,875   | 0,03125             |

#### Menü Funktionen

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten**

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Vorgabezeiten zu schließen. Folgende Einträge werden angezeigt:

* **Ändern:** Öffnet den gleichnamigen Dialog, um die Vorgabezeiten um einen Faktor zu erhöhen oder zu reduzieren. ⇨ "Vorgabezeiten ändern" auf Seite H-3149
* **Kopieren:** Öffnet den gleichnamigen Dialog, um die Vorgabezeiten aus der Standard-Maschine zu kopieren. ⇨ "Vorgabezeiten kopieren" auf Seite H-3149

***

### _A+W Business Pro Kapazitätsplanung_ _H-3141_

#### Vorgabezeiten – Zeitauswahl

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten > Register Zeitauswahl**

**Abbildung H-144: Vorgabezeiten – Tabellenauswahl** \[Image of the "Vorgabezeiten - Zeitauswahl" dialog]

In diesem Register legen Sie den Typ der Berechnung und die Priorität fest. ⇨ Tutorial, "Vorgabezeiten" auf Seite H-2967

**Identifikation**

**Arbeitsart** Arbeitsart, für die die Vorgabezeit gilt.

**Aggregat** Maschine, an der die Arbeitsart die Vorgabezeit benötigt.

***

### _H-3142_ _A+W Business Pro Kapazitätsplanung_

**Typ** Typ der Vorgabezeit:

* **0 - Basiszeit:** Gestoppte Zeit für einen Arbeitsgang. ⇨ "Eintrag von Zeitwerten in Stunden" auf Seite H-3141
* **1 - Zeitzuschlag:** Ein Zeitzuschlag wird für Arbeitsarten benötigt, die mehr Aufwand erfordern, z. B. für das Zuschneiden von Modellen.
* **2 - Alternativer Vorgang:** Diese Vorgabezeit wird nur herangezogen, wenn für die Arbeitsart eine alternative Arbeitsart existiert. In diesem Fall müssen Sie im Feld **Altern. Masch.-Nr.** die alternative Maschinennummer eintragen.
* **3 - Alternative ohne Stückliste:** Als VSG-Produzent ist Ihr VSG-Artikel standardmäßig mit einer Stückliste hinterlegt. Soll aber z. B. eine VSG-Scheibe manchmal nicht produziert, sondern direkt aus einem VSG-Bandmaß geschnitten werden, dann darf die Stückliste nicht berücksichtigt werden. Für die Arbeitsart VSG schneiden würden Sie Alternative ohne Stückliste wählen. In diesem Fall müssen Sie im Feld **Altern. Masch.-Nr.** die alternative Maschinennummer eintragen.
* **4 - Vorgang ignorieren:** Für einen Eckausschnitt müssen z. B. 3 Arbeitsgänge gemacht werden: 1. Bohren (von Eckloch), 2. Zuschnitt und 3. Schleifen. Die CNC-Maschine kann alles in einem, d. h., dort wird nur die Lochbohrung berücksichtigt. Die beiden anderen Arbeitsarten werden ignoriert. Sie müssen also nur der Arbeitsart Bohren eine Vorgabezeit zuweisen, die den gesamten Vorgang umfasst. Den anderen beiden Arbeitsarten weisen Sie auf dieser Maschine dann den Wert **Vorgang ignorieren** zu.

**Priorität** Wenn mehrere Maschinen für eine Arbeitsart zur Verfügung stehen, müssen Sie festlegen, welche Maschine zuerst auf freie Kapazitäten geprüft werden soll und welche z. B. nur manuell ausgewählt werden kann. Wenn zwei Maschinen die gleiche Priorität haben, dann prüft die Kapazitätsplanung die Kosten, die pro Maschine definiert sind. In diesem Fall wird automatisch die günstigere Maschine ausgewählt. Wenn keine Kosten pro Maschine hinterlegt sind, kann das Programm keine günstigste Maschine finden. In diesem Fall muss die Priorität bei gleichen Maschinen eindeutig sein.

* **9:** höchste Priorität (Standard-Maschine). Diese Maschinen werden immer zuerst ausgelastet.
* **8 bis 1:** absteigende Prioritäten. Diese Maschinen werden je nach Auslastung ausgewählt.
* **0:** niedrigste Priorität. Diese Maschinen werden nur dann eingesetzt, wenn alle anderen (gleichartigen) Maschinen ausgelastet sind.
* **-1:** zur manuellen Einlastung. Diese Maschinen werden von der automatischen Einlastung nur bei Engpässen ausgewählt.
* **-2, -3:** nur zur manuellen Einlastung. Diese Maschinen werden nie von der automatischen Einlastung ausgewählt.

**Alternative Masch.-Nr.** In diesem Feld muss die Maschinen-Nummer aus A+W Production eingetragen werden, wenn im Feld **Typ** der Wert **Alternativer Vorgang** oder **Alternative ohne Stückliste** ausgewählt ist.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3143_

**Gruppieren nach**

Mit der Wahl der Option legen Sie fest, wie die Darstellung in der Übersicht gruppiert sein soll. Die Felder sind nur im Auswahlmodus freigeschaltet.

* **Arbeitsart:** Zu jeder Arbeitsart werden die zugeordneten Aggregate angezeigt.
* **Aggregat:** Zu jedem Aggregat werden die Arbeitsarten mit den definierten Zeiten angezeigt.

**Sonstige Zuschläge**

**Tabelle** Verweis auf Zuschlagstabelle, z. B. für Übergrößen. Diese Zuschlagstabellen sind im Dialog **Sonderzeiten** angelegt. ⇨ "Sonderzeiten" auf Seite H-3150

**Einzelzeit**

**Zeit** Gemessene Zeit für die Arbeitsgänge am gewählten Aggregat.

**Zeiteinheit** Einheit, auf die sich die gemessene Zeit bezieht, z. B. auf Stück, auf Quadratmeter, auf Laufmeter usw.

**Mindestzeit** Zeit, die für eine Position mindestens berechnet wird, wenn die benötigte Zeit darunter liegt.

**Übersicht**

In der Übersicht sind alle Vorgabezeiten mit den zugeordneten Arbeitsarten aufgeführt. Mit einem Doppelklick auf Zuordnungen können werden die zugeordneten Produkte, Produktarten, Produktgruppen und/oder Warengruppen angezeigt. Die Gruppierung legen Sie im Auswahlmodus fest.

***

### _H-3144_ _A+W Business Pro Kapazitätsplanung_

#### Vorgabezeiten – Matrix

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten > Register Matrix**

**Abbildung H-145: Vorgabezeiten – Matrix** \[Image of the "Vorgabezeiten - Matrix" dialog with two dimensions: Dicke/Thickness and Laufmeter/Linear meter]

In diesem Register legen Sie Vorgabezeiten fest, die nach zwei Grenztypen gestaffelt sind. ⇨ Tutorial, "Vorgabezeiten" auf Seite H-2967

**Grenztyp1, Grenztyp2** Der Grenztyp legt die Maßeinheit für die Staffelung der Zeit fest. Sie können z. B. Dicke und Fläche wählen. Das Eingabefeld für den Grenzwert wird freigeschaltet, wenn Sie eine neue Spalte/Zeile einfügen. Der Grenzwert bezieht sich auf den Grenztyp. ⇨ Stammdaten, "Grenzmengen" auf Seite B-1025

**Spezifikation**

**Zeiteinheit** Die Einheit bezieht sich auf den Grenzwert. Der Grenzwert kann sich z. B. auf Stück, auf Quadratmeter, auf Laufmeter usw. beziehen.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3145_

**Dreiecksform** Sie können in einer Matrix oder in einem Würfel die Zeiten so erfassen, dass die angegebenen Grenzwerte vertauscht werden dürfen, z. B. Höhe und Breite.

* ☐ Die Grenztypen dürfen nicht vertauscht werden. In diesem Fall müssen Sie in allen Feldern pro Spalte/Zeile eine Zeit eintragen. Wählen Sie diese Einstellung für Gläser, bei denen es wichtig ist, in welcher Richtung sie geschnitten werden.
* ☑ Die Grenztypen dürfen vertauscht werden. Damit müssen Sie die Zeit nur in jeweils einer der Kombinationen der Grenztypen eintragen.

**Mindestangaben**

Die Mindestangaben werden bei der Einlastung geprüft. Bei Unterschreitung der Werte wird eine Meldung angezeigt und/oder ein Zuschlag erhoben.

**Mindestzeit** Sie können angeben, wie viel Zeit für eine Position mindestens berechnet wird.

**Übersicht**

In der Übersicht geben Sie in jedem Feld pro Zeile und Spalte die Zeit ein, die bei dieser Kombination von Grenztypen für die Arbeitsart benötigt wird.

***

### _H-3146_ _A+W Business Pro Kapazitätsplanung_

#### Vorgabezeiten – Vektor

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten > Register Vektor**

**Abbildung H-146: Vorgabezeiten – Vektor** \[Image of the "Vorgabezeiten - Vektor" dialog, showing a one-dimensional list based on qm/sqm]

In diesem Register hinterlegen Sie Vorgabezeiten, die nach einem Grenztyp gestaffelt sind, z. B. nach Dicke. Die Felder sind zum Register Matrix beschrieben. ⇨ "Vorgabezeiten - Matrix" auf Seite H-3145

***

### _A+W Business Pro Kapazitätsplanung_ _H-3147_

#### Vorgabezeiten – Würfel

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten > Register Würfel**

**Abbildung H-147: Vorgabezeiten – Würfel** \[Image of the "Vorgabezeiten - Würfel" dialog, showing three dimensions: Breite/Width, Höhe/Height, and Dicke/Thickness]

In diesem Register hinterlegen Sie Vorgabezeiten, die nach drei Grenztypen gestaffelt sind, z. B. nach Höhe, Breite und Dicke. Die Felder sind zum Register Matrix beschrieben. ⇨ "Vorgabezeiten - Matrix" auf Seite H-3145

***

### _H-3148_ _A+W Business Pro Kapazitätsplanung_

### Vorgabezeiten ändern

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten > Menü Funktionen > Ändern**

**Abbildung H-148: Vorgabezeiten ändern** \[Image of "Vorgabezeiten ändern" dialog with Aggregat, Arbeitsart, and Faktor fields]

In diesem Dialog können Sie die Vorgabezeiten für ein Aggregat oder eine Arbeitsart ändern. Wenn Sie z. B. den Faktor 1,5 eintragen, werden alle Zeiten der ausgewählten Kombination von Aggregat und Arbeitsart um die Hälfte erhöht. Der Faktor 0,5 würde die Zeiten auf die Hälfte reduzieren.

### Vorgabezeiten kopieren

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten > Menü Funktionen > Kopieren**

**Abbildung H-149: Vorgabezeiten kopieren** \[Image of "Vorgabezeiten kopieren" dialog with source and target Aggregat/Arbeitsart and a Faktor field]

In diesem Dialog können Sie Vorgabezeiten von einer Maschine und Arbeitsart kopieren, um sie auf eine andere Maschine und Arbeitsart zu übertragen. Sie können dabei Werte um einen Faktor erhöhen oder vermindern. Wenn Sie z. B. den Faktor 1,5 eintragen, werden alle Zeiten der ausgewählten Kombination von Aggregat und Arbeitsart um die Hälfte erhöht. Der Faktor 0,5 würde die Zeiten auf die Hälfte reduzieren.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3149_

### Sonderzeiten

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Sonderzeiten**

**Abbildung H-150: Sonderzeiten** \[Image of the "Sonderzeiten" dialog for defining time surcharges]

In diesem Dialog definieren Sie Zeitzuschläge für besonders aufwendige Bearbeitungen, z. B. für Sondergrößen. Die Zeitschläge können Sie im Dialog **Vorgabezeiten** im Bereich **Sonstige Zuschläge** zuweisen. Sonderzeiten, die nach den gleichen Kriterien angelegt sind, können in Gruppen (Tabellen) zusammengefasst werden. ⇨ Tutorial, "Sonderzeiten" auf Seite H-2970

Eine weitere Möglichkeit der Definition von Zeitzuschlägen in Form von Faktoren besteht über die Zuordnungsdialoge. ⇨ "Vorgabezeiten (Dialog)" auf Seite H-3141 ⇨ "Zuordnen" auf Seite H-3153

#### Zeitzuschlag für

**Nummer** Benutzerdefinierte Nummer (ID) der Tabelle.

**Bezeichnung** Name der Tabelle, z. B. Übergrößen.

#### Zuschläge (Übersicht)

In der Übersicht werden alle definierten Zuschläge aufgeführt.

***

### _H-3150_ _A+W Business Pro Kapazitätsplanung_

#### Zuschläge

In der Übersicht werden die Staffelungen des Zeitzuschlags angezeigt, der im Register **Tabelle** markiert ist.

* **Bis Grenze1, 2:** Wert pro Grenztyp, bis zu dem der Zuschlag berechnet werden soll.
* **Grenztyp 1, 2:** Grenztyp, auf den sich der Grenzwert bezieht, z. B. die Kantenlänge für die Berechnung von Übergrößen. ⇨ Stammdaten, “Grenzmengen" auf Seite B-1025
* **Zuschlag:** Höhe des Zuschlags. Der Wert bezieht sich auf die Zuschlagseinheit.
* **Zuschlagseinheit:** Einheit, mit der der Zuschlag berechnet werden soll.
* **Zuschlagsart:** Basis, auf die der Zuschlag bezogen wird.

### Besondere Prioritäten

**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Besondere Prioritäten**

**Abbildung H-151: Besondere Prioritäten** \[Image of the "Bes. Prioritäten" dialog showing rules for setting machine priorities based on criteria like customer, thickness, etc.]

In diesem Dialog tragen Sie pro Maschine und Arbeitsart die Prioritäten nach zusätzlichen Kriterien ein, z. B. nach Warengruppen, pro Dicke, pro Kunde. Wenn in den Feldern null (0) steht, gilt die besondere Priorität übergreifend, z. B. für den gewählten Kunden oder bei der angegebenen Anzahl.

Dies ist beispielsweise in folgenden Fällen sinnvoll:

* Wenn für eine Arbeitsart mehrere gleichartige Maschinen zur Verfügung stehen.
* Wenn Kunden spezielle Bearbeitungen wünschen, die nur auf speziellen Maschinen ausgeführt werden sollen oder können.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3151_

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

* **9:** höchste Priorität (Standard-Maschine). Diese Maschinen werden immer zuerst ausgelastet.
* **8 bis 1:** absteigende Prioritäten. Diese Maschinen werden je nach Auslastung ausgewählt.
* **0:** niedrigste Priorität. Diese Maschinen werden nur dann eingesetzt, wenn alle anderen (gleichartigen) Maschinen ausgelastet sind.
* **-1:** zur manuellen Einlastung. Diese Maschinen werden von der automatischen Einlastung nur bei Engpässen ausgewählt.
* **-2, -3:** nur zur manuellen Einlastung. Diese Maschinen werden nie von der automatischen Einlastung ausgewählt.

***

### _H-3152_ _A+W Business Pro Kapazitätsplanung_

## Zuordnen

**Kapazitätsplanung > Stammdaten > Zuordnen**

In diesen Dialogen ordnen Sie die Basisprodukte von A+W Business Pro (Einfachglas, VSG, ESG, Bearbeitungen, Modelle, Sprossen usw.) den Arbeitsarten zu.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:

* "Produktarten" auf Seite H-3154
* "WGR" auf Seite H-3156
* "Produktgruppe" auf Seite H-3157
* "Produkte" auf Seite H-3158
* "Kombi-Produktart" auf Seite H-3159
* "Sonderzuordnung 1" auf Seite H-3161
* "Sonderzuordnung 2" auf Seite H-3163
* "Sonderzuordnung 3" auf Seite H-3165
* "Sonderzuordnung 4" auf Seite H-3167
* "Kombi-Produktgruppe" auf Seite H-3169
* "Lagerartikel" auf Seite H-3171

***

### _A+W Business Pro Kapazitätsplanung_ _H-3153_

### Produktarten

**Kapazitätsplanung > Zuordnen > Produktarten**

**Abbildung H-152: Produktarten** \[Image of the "Produktarten" dialog, showing assignment of "Arbeitsarten" to a "Produktart"]

In diesem Dialog ordnen Sie den A+W Business Pro-Produktarten die Arbeitsarten in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für die jeweilige Produktart ausgeführt werden. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll. ⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-3012

#### Identifikation

**Produktart** Produktart, der Arbeitsarten zugeordnet sind.

#### Arbeitsarten

In der Übersicht werden die zugeordneten Arbeitsarten angezeigt.

**#** Nummer der Reihenfolge.

**Arbeitsart** Produktnummer und Bezeichnung der Arbeitsart. Wenn Sie \<k.A.> eintragen, wird die Produktart ignoriert. Das ist z. B. für die Produktart Leistungen sinnvoll.

***

### _H-3154_ _A+W Business Pro Kapazitätsplanung_

**Faktor** Die bei der Einlastung berechnete Zeit wird mit diesem Faktor multipliziert.

* 0 oder 1: Die Zeit wird nicht erhöht oder vermindert.
* \>1: Ein Faktor von z. B. 1,5 entspricht einer Zeiterhöhung von 50%.

#### Schaltflächen

**\[Neu], \[Löschen]** Mit diesen Schaltflächen schalten Sie eine neue Zeile frei oder löschen einen markierten Eintrag.

**Pfeilschaltflächen** Mit diesen Schaltflächen können Sie die Reihenfolge der Arbeitsarten ändern. Für die Produktart ESG könnte die Zuordnung z. B. wie folgt aussehen:

* Glas waschen
* Kontrolle
* ESG fertigen
* Verpacken verarbeitetes ESG
* Verladen

#### Übersicht Zuordnungen

In der Übersicht werden die Produktarten angezeigt, denen Arbeitsarten zugeordnet sind.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3155_

### WGR

**Kapazitätsplanung > Zuordnen > WGR**

**Abbildung H-153: Warengruppen** \[Image of the "WGR" (Warengruppen) dialog, similar to the "Produktarten" dialog]

In diesem Dialog ordnen Sie den A+W Business Pro-Warengruppen die Arbeitsarten in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für die jeweilige Warengruppe ausgeführt werden. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll. ⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-3012

#### Identifikation

**Warengruppe** Warengruppe, der Arbeitsarten zugeordnet sind.

#### Arbeitsarten

Die Felder und Schaltflächen in diesem Bereich sind zum Dialog **Produktarten** beschrieben. ⇨ "Produktarten" auf Seite H-3154

#### Übersicht Zuordnungen

In der Übersicht werden die Warengruppen angezeigt, denen Arbeitsarten zugeordnet sind.

***

### _H-3156_ _A+W Business Pro Kapazitätsplanung_

### Produktgruppe

**Kapazitätsplanung > Zuordnen > Produktgruppe**

**Abbildung H-154: Produktgruppen** \[Image of the "Produktgruppe" dialog, similar to the "Produktarten" dialog]

In diesem Dialog ordnen Sie den A+W Business Pro-Produktgruppen die Arbeitsarten in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für die jeweilige Produktgruppe ausgeführt werden. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll. ⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-3012

#### Identifikation

**Produktgruppe** Produktgruppe, der Arbeitsarten zugeordnet sind.

#### Arbeitsarten

Die Felder und Schaltflächen in diesem Bereich sind zum Dialog **Produktarten** beschrieben. ⇨ "Produktarten" auf Seite H-3154

#### Übersicht Zuordnungen

In der Übersicht werden die Produktgruppen angezeigt, denen Arbeitsarten zugeordnet sind.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3157_

### Produkte

**Kapazitätsplanung > Zuordnen > Produkte**

**Abbildung H-155: Produkte** \[Image of the "Produkte" dialog, similar to the "Produktarten" dialog]

In diesem Dialog ordnen Sie den A+W Business Pro-Produkten die Arbeitsarten aus der Kapazitätsplanung in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für das jeweilige Produkt ausgeführt werden. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll. ⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-3012

#### Identifikation

**Produkt** Produkt, dem Arbeitsarten zugeordnet sind.

#### Arbeitsarten

Die Felder und Schaltflächen sind zum Dialog **Produktarten** beschrieben. ⇨ "Produktarten" auf Seite H-3154

#### Übersicht Zuordnungen

In der Übersicht werden die Produkte angezeigt, denen Arbeitsarten zugeordnet sind.

***

### _H-3158_ _A+W Business Pro Kapazitätsplanung_

### Kombi-Produktart

**Kapazitätsplanung > Zuordnen > Kombi-Produktart**

**Abbildung H-156: Kombi-Produktarten** \[Image of the "Kombi-Produktart" dialog]

In diesem Dialog ordnen Sie den A+W Business Pro-Produkten, die Bestandteil einer Stückliste sind oder als Bearbeitung auf eine Produktgruppe wirken, die Arbeitsarten in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für die jeweilige Produktart ausgeführt werden. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll. ⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-3012

#### Identifikation

**Produkt** Produkt, dem als Stücklistenelement von z. B. VSG, ESG usw. eine andere Arbeitsart zugeordnet ist, als diejenige, die standardmäßig für das Hauptprodukt gilt.

**Als Teil von, Wirkt auf** Wenn die Float-Scheibe Teil einer Stückliste ist, kann sich die Produktionsreihenfolge oder die Arbeitsart ändern. Tragen Sie dann die entsprechende Produktart ein, z. B. ESG.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3159_

#### Arbeitsarten

Die Felder und Schaltflächen in diesem Bereich sind zum Dialog **Produktarten** beschrieben. ⇨ "Produktarten" auf Seite H-3154

#### Übersicht Zuordnungen

In der Übersicht werden die Kombi-Produktarten angezeigt, denen Arbeitsarten zugeordnet sind.

***

### _H-3160_ _A+W Business Pro Kapazitätsplanung_

### Sonderzuordnung 1

**Kapazitätsplanung > Zuordnen > Sonderzuordnung 1**

**Abbildung H-157: Sonderzuordnung 1 - Bearbeitungen** \[Image of the "Sonderzuordnung 1" dialog for assigning work types to a combination of a processing type and a follow-up processing type]

In diesem Dialog ordnen Sie einem A+W Business Pro-Bearbeitungsprodukt und der Folgebearbeitung die Arbeitsarten in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für dieses Produkt ausgeführt werden. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll. ⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-3012

#### Identifikation

**Bearbeitung** Bearbeitung, der Arbeitsarten zugeordnet sind.

**Folgebearbeitung** Folgebearbeitung, der Arbeitsarten zugeordnet sind.

#### Arbeitsarten

Die Felder und Schaltflächen in diesem Bereich sind zum Dialog **Produktarten** beschrieben. ⇨ "Produktarten" auf Seite H-3154

***

### _A+W Business Pro Kapazitätsplanung_ _H-3161_

#### Übersicht Zuordnungen

In der Übersicht werden die Bearbeitungen und Folgebearbeitung angezeigt, denen Arbeitsarten zugeordnet sind.

***

### _H-3162_ _A+W Business Pro Kapazitätsplanung_

### Sonderzuordnung 2

**Kapazitätsplanung > Zuordnen > Sonderzuordnung 2**

**Abbildung H-158: Sonderzuordnung 2 – Bearbeitungen an Modellen** \[Image of the "Sonderzuordnung 2" dialog, showing assignment of work types based on processing, model, and edge number]

In diesem Dialog ordnen Sie einer Bearbeitung an Modellscheiben und der Folgebearbeitung die Arbeitsarten in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für dieses Produkt ausgeführt werden. Sie können zu jeder Arbeitsart pro Kante einen Zeitfaktor angeben, der bei der Planung berechnet werden soll.

> **Beispiel** An einer Scheibe mit Rundbogen soll die Kantenbearbeitung an geraden Kanten auf der Standard-Schleifmaschine ausgeführt werden, die Kantenbearbeitung für den Rundbogen muss auf einer anderen Maschine gemacht werden.

⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-3012

#### Identifikation

**Bearbeitung** Bearbeitung, der Arbeitsarten zugeordnet sind.

**Modell** Modell, dem Arbeitsarten zugeordnet sind.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3163_

**Bis Stück** Stückzahl, wenn die Zuordnung der Arbeitsarten von der Anzahl der Scheiben abhängig ist, z. B. große Stückzahlen auf CNC-Maschinen. Geben Sie **9999** ein, wenn die Stückzahl nicht geprüft werden soll.

**Abbildung H-159: Kennzeichnung von Ecken und Kanten des gewählten Modells** \[Image of a shape with numbered edges and corners]

#### Arbeitsarten mit Kantenzuordnung

In der Übersicht werden die zugeordneten Arbeitsarten angezeigt. Die Anzahl der Kanten richtet sich nach dem gewählten Modell. Die Schaltflächen sind zum Dialog **Produktarten** beschrieben. ⇨ "Produktarten" auf Seite H-3154

**#** Nummer der Reihenfolge.

**Arbeitsart** Nummer und Bezeichnung der Arbeitsart. Wenn Sie \<k.A.> eintragen, wird die Bearbeitung ignoriert.

**Faktor** Die bei der Einlastung berechnete Zeit wird mit diesem Faktor multipliziert.

* 0 oder 1: Die Zeit wird nicht erhöht oder vermindert.
* \>1: Ein Faktor von z. B. 1,5 entspricht einer Zeiterhöhung von 50%.

**1 - n (Kante)** Angabe, für welche Kante der Faktor gilt. Die Anzahl der zur Verfügung stehenden Felder richtet sich nach der Anzahl der Kanten und Ecken des Modells. In der Modellskizze sind die Kanten mit roten Ziffern gekennzeichnet.

* ☐ Der Faktor wird für diese Kante nicht berechnet.
* ☑ Der Faktor wird berechnet.

#### Übersicht Zuordnungen

In der Übersicht werden die Bearbeitungen an Modellen angezeigt, denen Arbeitsarten zugeordnet sind.

***

### _H-3164_ _A+W Business Pro Kapazitätsplanung_

### Sonderzuordnung 3

**Kapazitätsplanung > Zuordnen > Sonderzuordnung 3**

**Abbildung H-160: Sonderzuordnung 3 – Kantenbearbeitung (Rechteckscheiben)** \[Image of the "Sonderzuordnung 3" dialog for edge processing on rectangular panes, with edge assignments]

In diesem Dialog ordnen Sie den Kantenbearbeitungen an Rechteckscheiben die Reihenfolge zu, in der sie ausgeführt werden.

> **Beispiel** Wenn bei einer Rechteckscheibe alle Kanten poliert werden sollen, werden standardmäßig gleichzeitig die Kanten 1 und 3 poliert und danach 2 und 4 (oder umgekehrt). Können auf einer Maschine 2 gegenüberliegende Kanten gleichzeitig poliert, gesäumt usw. werden, dann müssen Sie hierfür die Arbeitsart pro Kanten 1 + 3 und 2 + 4 zuordnen.

⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-3012

#### Identifikation

**Bearbeitung** Bearbeitung, der Arbeitsarten zugeordnet sind.

**Kanten 1 - 4** Angabe, für welche Kanten die Zuordnung gilt.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3165_

* ☐ Diese Kante wird nicht bearbeitet.
* ☑ Diese Kante wird bearbeitet.

**Abbildung H-161: Kennzeichnung von Ecken und Kanten für die Berechnung des Faktors** \[Image showing a rectangle with numbered edges 1-4]

#### Arbeitsarten mit Kantenzuordnung

In der Übersicht werden die zugeordneten Arbeitsarten angezeigt. Pro Kante kann ein Faktor festgelegt werden. Die Schaltflächen sind zum Dialog **Produktarten** beschrieben. ⇨ "Produktarten" auf Seite H-3154

**#** Nummer der Reihenfolge.

**Arbeitsart** Nummer und Bezeichnung der Arbeitsart. Wenn Sie `<k.A.>` eintragen, wird die Bearbeitung ignoriert.

**Faktor** Die bei der Einlastung berechnete Zeit wird mit diesem Faktor multipliziert.

* 0 oder 1: Die Zeit wird nicht erhöht oder vermindert.
* \>1: Ein Faktor von z. B. 1,5 entspricht einer Zeiterhöhung von 50%.

**1 - 4 (Kanten)** Angabe, für welche Kanten der Faktor gilt. In der Modellskizze sind die Kanten mit roten Ziffern gekennzeichnet.

* ☐ Der Faktor wird für diese Kante nicht berechnet.
* ☑ Der Faktor wird berechnet.

#### Übersicht Zuordnungen

In der Übersicht werden die Bearbeitungen angezeigt, denen Arbeitsarten zugeordnet sind.

***

### _H-3166_ _A+W Business Pro Kapazitätsplanung_

### Sonderzuordnung 4

**Kapazitätsplanung > Zuordnen > Sonderzuordnung 4**

**Abbildung H-162: Sonderzuordnung 4** \[Image of "Sonderzuordnung 4" dialog, assigning work types based on product, follow-up processing, and model]

In diesem Dialog ordnen Sie einem Produkt abhängig von einer Folgebearbeitung und einem Modell andere Arbeitsarten zu. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll. ⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-3012

#### Identifikation

**Produkt** Produkt, dem Arbeitsarten zugeordnet sind.

**Folgebearbeitung** Folgebearbeitung, der Arbeitsarten zugeordnet sind.

**Modell** Modell, für das die Zuordnung gilt.

**Abbildung H-163: Kennzeichnung von Ecken und Kanten für die Berechnung des Faktors** \[Image of a shape with numbered edges]

***

### _A+W Business Pro Kapazitätsplanung_ _H-3167_

#### Arbeitsarten mit Kantenzuordnung

In der Übersicht werden die zugeordneten Arbeitsarten angezeigt. Die Anzahl der Felder für die Kanten ist von der Wahl des Modells abhängig. Die Schaltflächen sind zum Dialog **Produktarten** beschrieben. ⇨ "Produktarten" auf Seite H-3154

**#** Nummer der Reihenfolge.

**Arbeitsart** Nummer und Bezeichnung der Arbeitsart. Wenn Sie `<k.A.>` eintragen, wird die Bearbeitung ignoriert.

**Faktor** Die bei der Einlastung berechnete Zeit wird mit diesem Faktor multipliziert.

* 0 oder 1: Die Zeit wird nicht erhöht oder vermindert.
* \>1: Ein Faktor von z. B. 1,5 entspricht einer Zeiterhöhung von 50%.

**1 - n (Kanten)** Angabe, für welche Kanten der Faktor gilt. Die Anzahl der zur Verfügung stehenden Felder richtet sich nach der Anzahl der Kanten des Modells. In der Modellskizze sind die Kanten mit roten Ziffern gekennzeichnet.

* ☐ Der Faktor wird für diese Kante nicht berechnet.
* ☑ Der Faktor wird berechnet.

#### Übersicht Zuordnungen

In der Übersicht werden die Bearbeitungen angezeigt, denen Arbeitsarten zugeordnet sind.

***

### _H-3168_ _A+W Business Pro Kapazitätsplanung_

### Kombi-Produktgruppe

**Kapazitätsplanung > Zuordnen > Kombi-Produktgruppe**

**Abbildung H-164: Kombi-Produktgruppen** \[Image of the "Kombi-Produktgruppe" dialog]

In diesem Dialog ordnen Sie Produkten, die Bestandteil einer Stückliste sind oder als Bearbeitung auf eine Produktgruppe wirken, eine Arbeitsart und einen Zeitfaktor zu. ⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-3012

#### Identifikation

**Produkt** Produkt, dem als Stücklistenelement von VSG oder ISO usw. eine andere Arbeitsart zugeordnet ist, als diejenige für das Hauptprodukt.

**Als Teil von/Wirkt auf** Wenn die Float-Scheibe Teil einer Stückliste ist, kann sich die Produktionsreihenfolge oder die Arbeitsart ändern. Tragen Sie dann die entsprechende Produktgruppe ein, z. B. VSG.

#### Arbeitsarten

Die Felder und Schaltflächen in diesem Bereich sind zum Dialog **Produktarten** beschrieben. ⇨ "Produktarten" auf Seite H-3154

***

### _A+W Business Pro Kapazitätsplanung_ _H-3169_

#### Übersicht Zuordnungen

Liste der Produkte, denen Arbeitsarten zugeordnet sind.

***

### _H-3170_ _A+W Business Pro Kapazitätsplanung_

### Lagerartikel

**Kapazitätsplanung > Zuordnen > Lagerartikel**

**Abbildung H-165: Lagerartikel** \[Image of the "Lagerartikel" dialog]

In diesem Dialog ordnen Sie Lagerartikeln die Arbeitsart Versand zu. Diese Zuordnung nutzen Sie, da die Lagerartikel (Beschaffungsart Lagerentnahme) nicht bearbeitet werden, z. B. bei Handgriffen, die nur verpackt und geliefert werden. Damit erreichen Sie, dass diese Produktgruppen z. B. in den Versand eingelastet und die Kosten und Zeiten kalkuliert werden. ⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-3012

#### Identifikation

**Produktgruppe** Lagerartikel, der Arbeitsart zugeordnet ist.

#### Arbeitsarten

Die Felder und Schaltflächen in diesem Bereich sind zum Dialog **Produktarten** beschrieben. ⇨ "Produktarten" auf Seite H-3154

***

### _A+W Business Pro Kapazitätsplanung_ _H-3171_

#### Übersicht Zuordnungen

In der Übersicht werden die Produktgruppen der Lagerartikel angezeigt, denen die Arbeitsart zugeordnet ist.

***

### _H-3172_ _A+W Business Pro Kapazitätsplanung_

## Sperren

Sie müssen Sperren definieren, um z. B. zu vermeiden, dass bestimmte Arbeiten doppelt durchgeführt werden oder eine Maschine eingeplant wird, die eine Leistung für ein bestimmtes Produkt nicht erbringen kann.

Die Vorgehensweise für das Sperren von Produkten, Produktgruppen oder Warengruppen auf bestimmten Maschinen ist für alle Dialoge ähnlich.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:

* "Sperren nach WGR" auf Seite H-3174
* "Sperren nach Produktgruppen" auf Seite H-3175
* "Sperren nach Produkten" auf Seite H-3177
* "Folge-Aggregate überspringen" auf Seite H-3178
* "Kundenbezogene Sperren" auf Seite H-3179
* "Fertigungsstraße definieren" auf Seite H-3181
* "Arbeitsgänge überspringen" auf Seite H-3182

***

### _A+W Business Pro Kapazitätsplanung_ _H-3173_

### Sperren nach WGR

**Kapazitätsplanung > Sperren > Sperren nach WGR**

**Abbildung H-166: Sperren nach WGR** \[Image of the "Sperren nach WGR" dialog]

In diesem Dialog sperren Sie bestimmte Warengruppen für eine oder mehrere Maschinen. ⇨ Tutorial, "Sperren" auf Seite H-3005

#### Identifikation

**Warengruppe** Warengruppe, für die die Maschine gesperrt ist.

#### Aggregate

In der Übersicht werden die zugeordneten Aggregate angezeigt.

**#** Nummer der Reihenfolge.

**Aggregat** Nummer und Bezeichnung des Aggregats.

#### Schaltflächen

**\[Neu], \[Löschen]** Mit diesen Schaltflächen schalten Sie eine neue Zeile frei oder löschen einen markierten Eintrag.

***

### _H-3174_ _A+W Business Pro Kapazitätsplanung_

**Pfeilschaltflächen** Mit diesen Schaltflächen können Sie die Reihenfolge der Arbeitsarten ändern.

#### Übersicht Sperren

In der Übersicht werden die Warengruppen angezeigt, für die Sperren definiert wurden.

### Sperren nach Produktgruppen

**Kapazitätsplanung > Sperren > Sperren nach Produktgruppen**

**Abbildung H-167: Sperren nach Produktgruppen** \[Image of the "Sperren nach Produktgruppen" dialog]

In diesem Dialog sperren Sie eine Produktgruppe abhängig von der Arbeitsart für eine oder mehrere Maschinen. ⇨ Tutorial, "Sperren" auf Seite H-3005

> **Beispiel** Für die Isolierglas-Produktion stehen 2 ISO-Linien zur Verfügung. Der Einbau eines Stahlrahmens in die ISO-Einheit geht jedoch nur auf der ISO-Linie Nr. 2. Darum muss die Produktgruppe Isolierglas bei der Arbeitsart Stahlrahmen montieren für die ISO-Linie Nr. 1 gesperrt werden.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3175_

#### Identifikation

**Produktgruppe** Produktgruppe, für die die Maschine gesperrt ist.

#### Aggregate

Die Schaltflächen sind zum Dialog **Sperren nach WGR** beschrieben. ⇨ "Sperren nach WGR" auf Seite H-3174

**#** Nummer der Reihenfolge.

**Arbeitsart** Nummer und Bezeichnung der Arbeitsart.

**Aggregat** Nummer und Bezeichnung des Aggregats.

**Total** In der Kombination von Produktgruppe und Arbeitsart kann die Maschine ganz oder teilweise gesperrt werden.

* ☑ Diese Maschine ist nur für diese Produktgruppe (Hauptprodukt) und diese Arbeitsart gesperrt.
* ☐ Ist die Produktgruppe inklusive der Arbeitsart Bestandteil einer Stückliste, dann wird die Maschine komplett gesperrt, d. h. auch für alle anderen Arbeitsarten, die das Hauptprodukt und dessen Stücklisten-Komponenten betreffen.

#### Übersicht Sperren

In der Übersicht werden die Produktgruppen angezeigt, für die Sperren definiert wurden.

***

### _H-3176_ _A+W Business Pro Kapazitätsplanung_

### Sperren nach Produkten

**Kapazitätsplanung > Sperren > Sperren nach Produkten**

**Abbildung H-168: Sperren nach Produkten** \[Image of the "Sperren nach Produkten" dialog]

In diesem Dialog sperren Sie ein Produkt abhängig von der Arbeitsart für eine oder mehrere Maschinen. ⇨ Tutorial, "Sperren" auf Seite H-3005

#### Identifikation

**Produkt** Produkt, für das die Maschine gesperrt ist.

#### Aggregate

Die Felder und Schaltflächen sind zum Dialog **Sperren nach Produktgruppen** beschrieben. ⇨ "Sperren nach Produktgruppen" auf Seite H-3175

#### Übersicht Sperren

In der Übersicht werden die Produkte angezeigt, für die Sperren definiert wurden.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3177_

### Folge-Aggregate überspringen

**Kapazitätsplanung > Sperren > Folge-Aggregate überspringen**

**Abbildung H-169: Folge-Aggregate überspringen** \[Image of the "Folge-Aggregate überspringen" dialog]

In diesem Dialog sperren Sie eine Maschine abhängig von der Folge-Maschine.

> **Beispiel** Wenn die Bohrstraße das Waschen automatisch beinhaltet, dann können Sie das nachfolgende Aggregat Waschmaschine sperren oder überspringen, um doppeltes Waschen zu verhindern.

⇨ Tutorial, "Sperren" auf Seite H-3005

#### Identifikation

**Aggregat** Aggregat, für das die Folge-Maschine gesperrt ist.

#### Aggregat

Die Felder und Schaltflächen sind zum Dialog **Sperren nach Produktgruppen** beschrieben. ⇨ "Sperren nach Produktgruppen" auf Seite H-3175

***

### _H-3178_ _A+W Business Pro Kapazitätsplanung_

#### Übersicht Sperren

In der Übersicht werden die Aggregate angezeigt, für die Sperren definiert wurden.

### Kundenbezogene Sperren

**Kapazitätsplanung > Sperren > Kundenbezogene Sperren**

**Abbildung H-170: Kundenbezogene Sperren** \[Image of the "Kundenbezogene Sperren" dialog]

In diesem Dialog sperren Sie Maschinen abhängig von der Kundennummer, vom Produkt oder von der Bearbeitung.

> **Beispiel** Besteht ein Kunde z. B. darauf, dass für seine Aufträge eine bestimmte Bohrmaschine nicht benutzt wird, muss diese Bohrmaschine für ihn gesperrt werden.

⇨ Tutorial, "Sperren" auf Seite H-3005

#### Menü Funktionen

Über dieses Menü können Sie die Sperre eines Kunden auf die gesamte Kundengruppe ausdehnen oder die Sperre aufheben.

Folgende Einträge werden angezeigt:

* **Sperre setzen:** Die Sperre wird auf alle Kunden der Kundengruppe ausgedehnt, zu der der angezeigte Kunde gehört. Alle betroffenen Kunden werden in der Übersicht aufgeführt.
* **Sperre aufheben:** Die Sperre wird für alle Kunden der Kundengruppe gelöscht. Die Kunden werden alle aus der Übersicht entfernt.
* **Vollständig gesperrt:** Die Sperre wird auf alle Registerkarten und Eingabefelder ausgedehnt.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3179_

Des Weiteren sind die Funktionen im Menü nicht aufrufbar. Verfügt ein Mitarbeiter über das Recht **Sperre aufheben** für die Kundenverwaltung, kann dieser für den Kunden das Sperrkennzeichen zurücksetzen oder verändern.

#### Identifikation

**Kunde** Kunde, für den die Sperre eingerichtet ist.

**Produkt/Bearbeitung** Produkt oder Bearbeitung, für die die Maschine gesperrt ist.

**Gesperrtes Aggregat** Maschine, die gesperrt ist.

#### Tabelle

In der Übersicht werden alle Kunden angezeigt, für die Sperren definiert sind.

* **Kunden-Nr., Kunde:** Nummer und Name des Kunden.
* **Kundengruppe:** Kundengruppe, zu der der Kunde gehört.
* **Ort:** Hauptsitz des Kunden.
* **Produkt-Nr., Produkt:** Nummer und Bezeichnung des Produkts, für das die Sperre definiert ist.
* **Gesperrtes Aggregat:** Aggregat, das für die Kombination von Kunde und Produkt gesperrt ist.

***

### _H-3180_ _A+W Business Pro Kapazitätsplanung_

### Fertigungsstraße definieren

**Kapazitätsplanung > Sperren > Fertigungsstraße definieren**

**Abbildung H-171: Fertigungsstraßen definieren** \[Image of the "Fertigungsstraße definieren" dialog]

In diesem Dialog sperren Sie eine Maschine abhängig von der vorherigen Maschine. ⇨ Tutorial, "Fertigungsstraße definieren" auf Seite H-3008

Die Schaltflächen sind zum Dialog **Sperren nach WGR** beschrieben. ⇨ "Sperren nach WGR" auf Seite H-3174

#### Identifikation

**Aggregat** Aggregat, für das die Folge-Maschine gesperrt ist. Diese Folge-Maschine wird im Bereich **Aggregate** angegeben.

#### Aggregate

In der Übersicht werden die Arbeitsarten und zugeordneten Aggregate angezeigt.

**#** Nummer der Reihenfolge.

**Arbeitsart** Nummer und Bezeichnung der Arbeitsart.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3181_

**Aggregat** Nummer und Bezeichnung des Aggregats.

**Total** Die Maschine kann ganz oder teilweise gesperrt werden.

* ☐ Die Maschine kann manuell ausgewählt werden.
* ☑ Diese Maschine ist für diese Arbeitsart vollständig gesperrt.

#### Übersicht Sperren

In der Übersicht werden die Aggregate mit Sperren angezeigt.

### Arbeitsgänge überspringen

**Kapazitätsplanung > Sperren > Arbeitsgänge überspringen**

**Abbildung H-172: Arbeitsgänge überspringen** \[Image of the "Arbeitsgänge überspringen" dialog]

In diesem Dialog sperren Sie Folgebearbeitungen abhängig von der Maschine.

> **Beispiel** Wenn die Bohrstraße das Waschen beinhaltet, dann können Sie den Folge-Arbeitsgang Glas waschen sperren, um doppeltes Waschen zu verhindern.

⇨ Tutorial, "Sperren" auf Seite H-3005

***

### _H-3182_ _A+W Business Pro Kapazitätsplanung_

#### Identifikation

**Aggregat** Aggregat, an dem die Arbeitsart gesperrt ist.

#### Arbeitsarten

In der Übersicht werden die zugeordneten Arbeitsarten angezeigt. Die Schaltflächen sind zum Dialog **Sperren nach WGR** beschrieben. ⇨ "Sperren nach WGR" auf Seite H-3174

**#** Nummer der Reihenfolge.

**Arbeitsart** Nummer und Bezeichnung der Arbeitsart, für das Aggregat gesperrt ist.

#### Übersicht Sperren

In der Übersicht werden die Aggregate angezeigt, für die Sperren definiert wurden.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3183_

## Übersichten

Mit verschiedenen Tabellen und Grafiken erhalten Sie einen Überblick über die Auslastung an einem bestimmten Datum oder in einen Zeitraum.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:

* "Statistik" auf Seite H-3185
* "Grafik-Bereiche" auf Seite H-3186
* "AV-Bereichsstatistik" auf Seite H-3188
* "AV-Bereichsstatistik kurz" auf Seite H-3192
* "Konten" auf Seite H-3192
* "Kostenstellen-Definitionen" auf Seite H-3194

***

### _H-3184_ _A+W Business Pro Kapazitätsplanung_

### Statistik

**Kapazitätsplanung > Übersicht > Statistik**

**Abbildung H-173: Statistik** \[Image of the "Statistik" dialog showing completed jobs for a specific aggregate within a date range]

In dieser Übersicht können Sie sich alle Aufträgen anzeigen lassen, die innerhalb eines Zeitraumes von einem Aggregat fertig gemeldet wurden. Die Bildschirm-Anzeige gilt nur für die ausgewählte Maschine. Die Druck-Ausgabe zeigt jedoch alle Maschinen und die Zeitkosten an.

#### Selektion

**Von, bis** Auswertungszeitraum. Wenn Sie in beiden Feldern dasselbe Datum eintragen, wird eine Tagesauswertung erstellt.

**Aggregat** Maschine, deren Auslastung angezeigt werden soll.

#### Belegzeiten

In der Übersicht werden pro Aggregat die Werte für alle fertig gemeldeten Stückzahlen aufgelistet.

* **..:** Arbeitsart.
* **Stück:** Fertig gemeldete Stückzahl.
* **Fläche:** Fertig gemeldeten Quadratmeter.
* **Umfang:** Kantenlänge insgesamt.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3185_

* **Zeit:** Insgesamt benötigte Zeit.
* **Aggregat:** Aggregat, das die Werte gemeldet hat.

**Summe Zeit** Summe der Zeiten für die ausgewählte Maschine.

### Grafik-Bereiche

**Kapazitätsplanung > Übersicht > Grafik-Bereiche > Legende**

**Abbildung H-174: Grafik-Bereiche - Wochenübersicht** \[Image of a graphical weekly overview of machine load, with a legend for different work types]

In dieser Übersicht lassen Sie sich eine grafische Übersicht über die Auslastung entweder nach Aggregattypen oder nach Produktionsbereichen anzeigen. Sie können die Anzeige über das Menü **Werk** auf ein bestimmtes Werk oder einen Mandanten einschränken. Die Grafik kann aus verschiedenen Dialogen heraus geöffnet werden. Die Anzeige der Daten ist dann entsprechend des Ausgangsdialogs gefiltert, z. B. pro Tagesschicht.

***

### _H-3186_ _A+W Business Pro Kapazitätsplanung_

#### Zeitraum

**(Datum)** Datum, für das die Grafik erstellt werden soll.

**Woche** Sie können nur den eingetragenen Tag oder die gesamte Woche auswerten.

* ☐ Nur der ausgewählte Tag wird ausgewertet.
* ☑ Die Auswertung bezieht die ganze Woche ein (Montag bis Sonntag).

#### Auswahl

**Aggregattyp, Produktionsbereich** Mit der Wahl der Option legen Sie fest, worauf sich die Auswertung beziehen soll.

**\[Legende]** Blendet die Legende mit der Bedeutung der Farben in der Grafik ein und aus. Die Einstellung gilt für alle Grafiken.

#### Grafik

**Rote Linien** Die rote Linie zeigt das Ende einer Schicht an.

**Linke Spalte** Die linke Spalte verändert sich je nach Tages- oder Wochenansicht.

* Tagesansicht: Schichten
* Wochenansicht: Tagesdatum.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3187_

### AV-Bereichsstatistik

**Kapazitätsplanung > Übersicht > AV-Bereichsstatistik**

Die AV-Bereichsstatistik ist eine Statistik auf Produktebene für alle fertig gemeldeten Arbeitsarten.

In diesem Dialog finden Sie folgende Register:

* "AV-Bereichsstatistik - Auswahl" auf Seite H-3189
* "AV-Bereichsstatistik - Tabelle" auf Seite H-3191

***

### _H-3188_ _A+W Business Pro Kapazitätsplanung_

#### AV-Bereichsstatistik – Auswahl

**Kapazitätsplanung > Übersicht > AV-Bereichsstatistik > Register Auswahl**

**Abbildung H-175: AV-Bereichsstatistik – Auswahl** \[Image of the selection criteria for the AV-Bereichsstatistik report]

In diesem Register wählen Sie die Kriterien aus, nach denen die Übersicht über Fertigmeldungen erstellt werden soll. Wenn Sie alle Angaben eines Zeitraums anzeigen lassen wollen, dürfen Sie die Suche nicht durch Restriktionen einschränken.

**Auswertungszeitraum**

**Von, bis** Auswertungszeitraum. Wenn Sie in beiden Feldern dasselbe Datum eintragen, wird eine Tagesauswertung erstellt.

**Restriktionen**

In diesem Bereich können Sie Auswahl einschränken.

> **Eintrag \<k. A.>** Wenn eines der Felder nicht berücksichtigt werden soll, müssen Sie den Eintrag vollständig löschen. Der Eintrag `<k. A.>` bedeutet, dass z. B. die Produktart `<k. A.>` ausgeschlossen werden soll. Wenn Sie Informationen zu allen Produktarten, -gruppen und AV-, Produktionsbereichen anzeigen lassen wollen, müssen Sie alle vier Felder leer lassen.

**Produktart** Die gewählte Produktart soll nicht angezeigt werden.

**Produktgruppe** Die gewählte Produktgruppe soll nicht angezeigt werden.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3189_

**AV-Bereich** Der gewählte AV-Bereich soll nicht angezeigt werden.

**Produktionsbereich** Der gewählte Produktionsbereich soll nicht angezeigt werden.

**Ausgabe / Sortierung**

Im linken Feld werden die Ausgabemöglichkeiten angezeigt. Im rechten Feld wird angezeigt, nach welchem Kriterium die Auswertung sortiert werden soll. Die Einstellung wirkt sich auf die Darstellung des Ergebnisses im Register **Tabelle** aus. Einen markierten Eintrag verschieben Sie mit den Pfeilschaltflächen in das rechte Feld oder zurück in das linke Feld.

**Übersicht nach**

Mit der Wahl der Option legen Sie fest, welche Daten angezeigt werden sollen:

* **Produktart:** Die Auswertung soll sich auf die Produktart beziehen.
* **Produktgruppe:** Die Auswertung soll sich auf die Produktgruppe beziehen.
* **Produkt:** Die Auswertung soll sich auf die Produkte beziehen.

***

### _H-3190_ _A+W Business Pro Kapazitätsplanung_

#### AV-Bereichsstatistik – Tabelle

**Kapazitätsplanung > Übersicht > AV-Bereichsstatistik > Register Tabelle**

**Abbildung H-176: AV-Bereichsstatistik – Tabelle** \[Image of the results table for the AV-Bereichsstatistik report]

In diesem Register wird das Ergebnis der Auswertung angezeigt. Sie können mit den entsprechenden Auswahlkriterien z. B. ermitteln, in welchen AV-Bereichen das Glas verbraucht wird.

**Übersicht**

Die zweite Spalte wird nur dann gefüllt, wenn nach Produktionsbereich und AV-Bereich sortiert wird, egal in welcher Reihenfolge.

* **Produktionsbereich, AV-Bereich:** Anzeige je nach Wahl des Sortierkriteriums.
* **Produkt, Produktgruppe, Produktart:** Anzeige je nach Wahl des Sortierkriteriums.
* **Vorgang:** In diesem Feld werden die Arbeitsarten angezeigt.
* **Stück:** Produzierte Stückzahlen.
* **Qm:** Produzierte Fläche.
* **Lfm:** Produzierte Laufmeter (Kanten).
* **Kosten ZW:** Ermittelte Zeitkosten.
* **Materialkosten:** Ermittelte Materialkosten.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3191_

### AV-Bereichsstatistik kurz

**Kapazitätsplanung > Übersicht > AV-Bereichsstatistik kurz**

In diesem Dialog lassen Sie sich eine verkürzte Liste der Auswertung nach AV-Bereichen anzeigen, die automatisch nach den beiden Kriterien AV-Bereich und Produktionsbereiche sortiert ist. Die Felder sind zum Dialog **AV-Bereichsstatistik** beschrieben. ⇨ "AV-Bereichsstatistik" auf Seite H-3188

### Konten

**Kapazitätsplanung > Übersicht > Konten**

**Abbildung H-177: Konten - Auswahl** \[Image of the "Konten" (Accounts/Cost Centers) selection dialog]

In diesem Dialog lassen Sie sich anzeigen, auf welche Kostenstellen oder AV-Bereiche bestimmte Produkte, Produktgruppen oder Produktarten gebucht wurden. Die Daten werden aus den Aufträgen ausgelesen. Archivierte Aufträge werden nicht berücksichtigt.

#### Menü Kostenstellen

Über dieses Menü können Sie den Dialog **Kostenstellen-Definition** öffnen, um die Kostenstellen anzulegen oder zu bearbeiten. ⇨ "Kostenstellen-Definitionen" auf Seite H-3194

***

### _A+W Business Pro Kapazitätsplanung_ _H-3192_

#### Auswertungszeitraum Liefertermin

**Von, bis** Auswertungszeitraum. Wenn Sie in beiden Feldern dasselbe Datum eintragen, wird eine Tagesauswertung erstellt.

#### Sortierung nach

Mit der Wahl der Option legen Sie fest, wie die Anzeige sortiert werden soll:

* **Kostenstellen:** Das sind die Kostenstellen, die Sie für die Kapazitätsplanung erstellt haben. ⇨ "Kostenstellen-Definitionen" auf Seite H-3194
* **AV-Bereiche:** AV-Bereiche aus den A+W Business Pro-Stammdaten.

> **Kostenstellen definieren** Neue Kostenstellen definieren Sie auf die gleiche Weise wie die Vorschauspalten im Modul Fertigung. ⇨ Tutorial, "Prinzip der Auswertungsspalten" auf Seite H-3073

#### Übersicht nach

Mit der Wahl der Option legen Sie fest, ob die Auswertung nach Produktart, Produktgruppe oder nach den einzelnen Produkten angezeigt wird.

#### Übersicht

In der Übersicht werden folgende Daten angezeigt:

* **Kostenstelle:** Bezeichnung der Kostenstelle. Die Bezeichnungen werden im Dialog **Kostenstellen Definition** festgelegt. ⇨ "Kostenstellen-Definitionen" auf Seite H-3194
* **AV-Bereich:** AV-Bereich, dem die Kostenstelle zugeordnet ist.
* **Produktart, Produktgruppe, Produkt:** Die Anzeige der entsprechenden Daten richtet sich nach der Option, die im Register **Auswahl** gewählt wurde.
* **Stück:** Anzahl der gefertigten Scheiben.
* **Fläche:** Gesamtfläche der gefertigten Scheiben.
* **Materialkosten:** Materialkosten der gefertigten Scheiben.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3193_

### Kostenstellen-Definitionen

**Kapazitätsplanung > Übersicht > Konten > Menü Kostenstellen**

**Abbildung H-178: Kostenstellen-Definition** \[Image of the "Kostenstellen Definition" dialog]

In diesem Dialog legen Sie die Kostenstellen für die Auswertung von Produktionsdaten und -kosten an. Bevor Sie Kostenstellen anlegen, sollten Sie sich überlegen, in welcher Reihenfolge die Kostenstellen abgefragt werden sollen.

> **Beispiel ESG** Sie fragen erst ab, ob es sich um ein ESG mit Bearbeitung handelt (Kostenstelle Nr. 7 mit Prio 19). Wenn dies nicht der Fall ist, kommt die Folge-Abfrage. Das ESG, das nicht bearbeitet ist, fließt in die Kostenstelle ESG (Kostenstelle Nr. 6 mit Prio 20).

> **Kostenstellen definieren** Neue Kostenstellen definieren Sie auf die gleiche Weise wie die Vorschauspalten im Modul Fertigung. ⇨ Tutorial, "Prinzip der Auswertungsspalten" auf Seite H-3073

**Nr.** Nummer der Kostenstelle.

**Bezeichnung** Namen der Kostenstelle.

**HPA** Haupt-Produktart. In diesem Feld tragen Sie ein, für welche Produktart die Auswertung gemacht werden soll.

**Nr 1, Nr 2** Diese Einträge beziehen sich auf die Felder **Typ 1** und **Typ 2**. Hier tragen Sie die entsprechende Nummer der Produktart oder Produktgruppe von Typ 1 oder Typ 2 ein oder 0 für keine Vorgabe.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3194_

**Typ 1, Typ 2** Produktart bzw. Produktgruppe, die Stücklistenelement der Hauptproduktart ist.

* 0 = Keine Vorgabe
* 1 = Produktart
* 2 = Produktgruppe Sie suchen z. B. nach der Produktart (Typ 1 = 1) Bearbeitung (Nr 1 = 20), die Bestandteil von ESG (HPA = 2) ist.

**Priorität** Nummer der Reihenfolge, in der die Abfrage der Kostenstellen erfolgen soll.

**Ausschluß** Sie können ein Produkt von der Regel ausschließen. Die Produktnummer muss in Klammern stehen.

> **Beispiel** Alle ESG-Scheiben werden gesäumt. Deshalb möchten Sie nicht, dass gesäumte ESG-Scheiben in die Kostenstelle ESG mit Bearbeitung einfließen. Sie schließen dies aus, indem Sie die entsprechende Produktnummer (in Klammern) eintragen.

### Schnittstelle Lisec

Dieser Dialog ist nur freigeschaltet, wenn Sie mit einer entsprechenden Schnittstelle arbeiten.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3195_

## Kapazitätsplanung

**Fertigung > Kapazitätsplanung**

Zur Planung der Kapazitäten stehen im Modul Fertigung verschiedene Dialoge zur Verfügung. Damit können Sie in diesem Modul neben der Übergabe von Daten an die Produktion auch den Produktionsfortschritt mit Hilfe der Rückmeldungen prüfen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:

* "Einlastung" auf Seite H-3197
* "Produktionsmeldungen" auf Seite H-3222
* "Leitstand" auf Seite H-3260

***

### _H-3196_ _A+W Business Pro Kapazitätsplanung_

### Einlastung

Die Zeit- und Materialkosten können nur für Aufträge berechnet werden, die in die Kapazitätsplanung eingelastet werden. Die Aufträge können manuell oder automatisch in definierten Intervallen eingelastet werden.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:

* "Nummernverwalter" auf Seite H-3197
* "Einlasten NV" auf Seite H-3198
* "Kriterien ändern (Modus Terminsuche)" auf Seite H-3201
* "Lieferdatum" auf Seite H-3203
* "Einlasten Auftrag" auf Seite H-3204
* "Einlasten Ergebnis" auf Seite H-3209
* "Restmengenübertragung" auf Seite H-3211
* "Aggregat-Auswahl bei Engpass" auf Seite H-3212
* "Auftragsnummern" auf Seite H-3214
* "Positions-Split" auf Seite H-3215
* "Positions-Zeiten" auf Seite H-3217
* "Aggregate Ausfall" auf Seite H-3218

#### Nummernverwalter

**Fertigung > Kapazitätsplanung > Einlastung > Nummernverwalter**

Sie haben die Möglichkeit, mehrere Aufträge manuell gleichzeitig in die Kapazitätsplanung einzulasten. Hierfür werden diese in einem Nummernverwalter gesammelt.

Im Dialog **Einlasten NV** können Sie den Nummernverwalter auswählen und die Aufträge einlasten. Angezeigt werden alle Nummernverwalter, die für Dokumente erstellt wurden. ⇨ "Einlasten NV" auf Seite H-3198

Im Dialog **Nummernverwalter** können Sie sich zu dem Auftrag, den Sie in der Übersicht markiert haben, den Dialog **Übersicht Statusrückmeldungen** öffnen. Der Dialog ist ausführlich im Part **Verkauf** beschrieben. ⇨ Verkauf, "Übersicht Statusrückmeldung" auf Seite C-1860

Der Dialog **Nummernverwalter** und die zugehörigen Menüs sind für alle Module gleich. Er ist ausführlich im Part **Verkauf** beschrieben. ⇨ Verkauf, "Nummernverwalter" auf Seite C-1917

***

### _A+W Business Pro Kapazitätsplanung_ _H-3197_

#### Einlasten NV

**Fertigung > Kapazitätsplanung > Einlastung > Einlasten NV**

Über einen Nummernverwalter lasten Sie alle Aufträge manuell ein, die dem Mindeststatus entsprechen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:

* "Menü Funktionen" auf Seite H-3198
* "Menü Optionen" auf Seite H-3198
* "Einlasten NV (Dialog)" auf Seite H-3199

**Menü Funktionen**

**Fertigung > Kapazitätsplanung > Einlastung > Einlasten NV > Menü Funktionen**

Über dieses Menü können Sie sich die Historie zu dem Auftrag anzeigen lassen, den Sie in der Übersicht markiert haben. Die Historie ist ausführlich im Part **Verkauf** beschrieben. ⇨ Verkauf, "Historie" auf Seite C-1834

**Menü Optionen**

**Fertigung > Kapazitätsplanung > Einlastung > Einlasten NV > Menü Optionen**

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen und andere Dialoge öffnen, ohne den aktuellen Dialog zu verlassen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen. Folgende Einträge werden angezeigt:

* **Modus Terminsuche:** Öffnet den gleichnamigen Dialog, in dem Sie die Kriterien für die Terminsuche festlegen können. ⇨ "Kriterien ändern (Modus Terminsuche)" auf Seite H-3201
* **Positionskontrolle:** Beim Einlasten wird der Anteil des Auftrags an der Tageskapazität geprüft. Der Prozentwert ist im Dialog **Arbeitsarten** hinterlegt. ⇨ "% Limit" auf Seite H-3109
* **Alter Verweiltagemodus:** Diese Einstellung ist nur erforderlich, wenn Sie den alten Modus für Verweiltage (= Übergangsmatrix) beibehalten wollen.
* **Check auf Rüstzeit:** Wenn die Rüstzeit zu mehreren Arbeitsarten eingerichtet ist, die für eine Auftragsposition ausgeführt werden, dann soll diese Zeit nur einmal pro Position berechnet werden.

***

### _H-3198_ _A+W Business Pro Kapazitätsplanung_

#### Einlasten NV (Dialog)

**Fertigung > Kapazitätsplanung > Einlastung > Einlasten NV**

**Abbildung H-179: Einlasten nach Nummernverwalter** \[Image of the "Aufträge einlasten" dialog showing a list of orders from a selected number range manager]

In diesem Dialog übergeben Sie die Aufträge aus einem Nummernverwalter an die Kapazitätsplanung. Die Übergabe starten Sie mit **Menü Start > Ausführen**. ⇨ Tutorial, "Einlastung der Aufträge" auf Seite H-3023

**Identifikation**

**Mandant** Auswahl des Mandanten, dessen Aufträge eingelastet werden sollen.

**Bereich** Auswahl des AV-Bereichs, dessen Aufträge eingelastet werden sollen. ⇨ Stammdaten, "AV-Bereiche" auf Seite B-1160

**Mitarbeiter** Angemeldeter Mitarbeiter.

**Nummernverwalter** Wenn Sie einen Nummernverwalter ausgewählt haben, werden alle Aufträge übergeben, die in diesem Nummernverwalter stehen und den Mindeststatus erreicht haben.

***

### _A+W Business Pro Kapazitätsplanung_ _H-3199_

**Auftragspriorität**

Das Feld ist nur freigeschaltet, wenn Sie in den Firmendaten > Register Kapa-Planung > Feld **Einlastpriorität** die Einstellung **Geänderte Priorität in Auftrag übernehmen** ausgewählt haben. Die Aufträge werden in der Regel nach der Priorität **Normal** eingelastet. Nur wenn es sich bei den Aufträgen z. B. um Eilaufträge handelt, die mit schnelleren Durchlaufzeiten berechnet werden sollen, müssen Sie die entsprechende Priorität auswählen.

* **Abruf:** Der Auftrag wird erst gefertigt, wenn der Kunde die Positionen abruft.
* **Eilt:** Der Auftrag muss mit oberster Priorität eingelastet werden.
* **Normal:** Der Auftrag wird den Standard-Einstellungen entsprechend eingelastet.
* **Zugabe:** Diese Priorität bedeutet, dass der Auftrag so gefertigt werden soll, dass er Reste und Restplatten verbraucht, die beim Zuschnitt anderer Aufträge entstehen.

> **Auftragspriorität berücksichtigen** Wenn außer der Auftragspriorität **Normal** auch z. B. die Priorität **Eilt** berücksichtigt werden soll, dann müssen dafür eigene Übergangszeiten eingerichtet sein. Wenn diese nicht eingerichtet sind, wird mit der Priorität **Normal** eingelastet. ⇨ "Übergangszeiten" auf Seite H-3112 ⇨ "Übergangsmatrix" auf Seite H-3134

**Verhalten bei Lieferterminproblemen**

Mit der Wahl der Option legen Sie fest, wie beim Einlasten auf Probleme reagiert werden soll:

* **Keine Automatik:** Der Auftrag soll nicht automatisch zum nächsten möglichen Produktionstermin eingelastet werden. Bei dieser Option wird der Dialog **Lieferdatum** geöffnet, in dem Sie die Vorgaben zum Einlasten einstellen. ⇨ "Lieferdatum" auf Seite H-3203
* **Nächster Liefertermin:** Der Auftrag soll zum nächsten möglichen Liefertermin eingelastet werden. Der neue Liefertermin wird in den Auftrag zurückgeschrieben.
* **Zum Liefertermin einlasten:** Der Auftrag soll zum ursprünglichen Liefertermin eingelastet werden, auch wenn damit die Maschinenkapazitäten überlastet werden. Diese Option können Sie wählen, wenn Sie sicher sind, dass Sie andere eingelastete Aufträge verschieben können.
* **Unendliche Kapazitäten:** Der Auftrag wird unabhängig von den tatsächlichen Kapazitäten eingelastet.

***

### _H-3200_ _A+W Business Pro Kapazitätsplanung_
