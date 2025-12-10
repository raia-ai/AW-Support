---
title: "DE_AWBusiness_Kapazitaetsplanung_4_3"
source: "DE_AWBusiness_Kapazitaetsplanung_4_3.pdf"
tags: ["A+W Business Pro", "Kapazitätsplanung", "Software-Referenz", "Organisation", "Aggregate", "Vorgabezeiten", "Einlastung", "Stammdaten", "Produktionsplanung"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Dieses Dokument ist eine Softwarereferenz für das Modul Kapazitätsplanung in A+W Business Pro. Es beschreibt die Konfiguration von Stammdaten wie Organisation, Aggregate, Kalender, Vorgabezeiten und die Durchführung der Einlastung von Fertigungsaufträgen."
long_description: "Diese Softwarereferenz bietet eine detaillierte Anleitung für das Modul Kapazitätsplanung der Software A+W Business Pro. Das Dokument ist in mehrere Hauptkapitel unterteilt, die den Benutzer durch die Konfiguration und Nutzung der Kapazitätsplanungsfunktionen führen. Im Kapitel 'Organisation' wird die Einrichtung von grundlegenden Organisationseinheiten wie Produktionsbereichen, Maschinen (Aggregaten) und deren technischen Restriktionen sowie Kalendern und Übergangszeiten behandelt. Das Kapitel 'Vorgabezeiten' erklärt, wie Zeitwerte für verschiedene Arbeitsarten und Maschinen definiert werden, unterteilt in Matrix-, Vektor- und Einzelzeit-Formate. Das Kapitel 'Zuordnen' beschreibt, wie Basisprodukte aus A+W Business Pro (z.B. Einfachglas, VSG, ESG) den entsprechenden Arbeitsarten in der Kapazitätsplanung zugeordnet werden. Im Kapitel 'Sperren' wird erläutert, wie Maschinen für bestimmte Produkte, Warengruppen oder Arbeitsgänge gesperrt werden können, um fehlerhafte Planungen zu vermeiden. Schließlich behandeln die Kapitel 'Übersichten' und 'Einlastung' die Analyse der Maschinenauslastung durch verschiedene Statistiken und Grafiken sowie den eigentlichen Prozess der manuellen oder automatischen Einlastung von Fertigungsaufträgen in die Produktion."
---

# Softwarereferenz - Organisation

---
## Min. Verweiltage
Anzahl der Tage, die ein Stück einer Position im Produktionsbereich verweilt:
- **0** = keine Verweilzeit
- **0,1** = eine Schicht
- **1** = ein Tag, z. B. Eingang in den Produktionsbereich heute, Ausgang morgen.

Weitere Zeiten werden als Übergangszeiten definiert.
⇨ "Übergangszeiten" auf Seite H-197
⇨ “Übergangsmatrix" auf Seite H-216

## Mandant
Mandant, dem der Produktionsbereich zugeordnet ist. Die Mandanten sind in den Firmendaten hinterlegt.
⇨ Stammdaten, "Firmendaten - Mandant" auf Seite B-906

## Status Rückmeldungen
Der Status in der Kapazitätsplanung und im Auftrag kann automatisiert über die Rückmeldung aus der Betriebsdatenerfassung (BDE) von A+W Production umgesetzt werden. Mit der Einstellung legen Sie fest, von welcher Erfassungsstelle die Rückmeldung gesendet wird.
Der Status der Positionen und des Auftrags kann im Dialog Statusrückmeldungen geprüft werden.
⇨ Verkauf, "Übersicht Statusrückmeldung" auf Seite C-507

## Aggregate
**Kapazitätsplanung > Stammdaten > Organisation > Aggregate**

Alle genutzten Maschinen werden mit den technischen Restriktionen und den Betriebskosten angelegt, die für die Planung und Berechnung der Kosten notwendig sind.

In diesem Dialog finden Sie folgende Register:
- "Aggregate - Allgemein" auf Seite H-202
- "Aggregate - Restriktionen" auf Seite H-208

Die Felder für die Definition von Restriktionen werden im Dialog Aggregattypen freigeschaltet.
⇨ "Aggregattypen" auf Seite H-189

> **Achtung bei nachträglicher Aktivierung von Prüfungen**
> Wenn Sie bei einem Aggregattyp eine Checkbox nachträglich aktivieren, müssen Sie alle Aggregate prüfen, die zu dem geänderten Aggregattyp gehören. Die neu freigeschalteten Felder sind standardmäßig leer. Das kann bei der Prüfung Fehler verursachen.

## Aggregate - Allgemein
**Kapazitätsplanung > Stammdaten > Organisation > Aggregate > Register Allgemein**

*(Abb. H-135 Aggregate - Allgemein)*

In diesem Register legen Sie die Maschinen (Aggregate) an, die Sie nutzen und die für die Kapazitätsplanung relevant sind. Sie sollten auch ein Aggregat Versand anlegen, damit die Zeiten dafür geplant werden können.
⇨ Tutorial, "Aggregattypen und Aggregate" auf Seite H-25

### Aggregat

**Nr./Bezeichnung**
Nummer (ID) und Beschreibung können frei gewählt werden. Wir empfehlen, ähnliche Maschinen in Nummernkreisen zu gruppieren, z. B. Schneidtische 100-199, Bohrmaschinen 400-499 usw.

**Typ**
Aggregat-Typ, zu dem die Maschine gehört. Durch die Zuweisung werden die Felder für die Restriktionsprüfungen freigeschaltet.
⇨ "Aggregattypen" auf Seite H-189

**Produktionsbereich**
Produktionsbereich, in dem die Maschine steht.
⇨ "Produktionsbereich" auf Seite H-200

### Optionen

**Scheiben drehbar**
Angabe, ob die Scheiben auf der Maschine gedreht werden können.
- [ ] Die Scheiben können nicht gedreht werden.
- [x] Die Scheiben können gedreht werden.

**Kantenschutz möglich**
Angabe, ob auf der Maschine Kantenschutz angebracht werden kann.
- [ ] Kantenschutz kann nicht angebracht werden.
- [x] Kantenschutz kann angebracht werden.

**Autobrechen**
Angabe, ob der Zuschneidetisch über eine automatische Brechvorrichtung verfügt.
- [ ] Der Tisch hat keine automatische Brechvorrichtung.
- [x] Die Scheiben können automatisch gebrochen werden.

**Modelle möglich**
Angabe, ob auf der Maschine Modelle (nicht-rechteckige Scheiben) gefertigt werden können.
- [ ] Modelle sind nicht möglich.
- [x] Modelle sind möglich.

**Sprossen möglich**
Angabe, ob auf der Maschine Sprossen gefertigt werden können.
- [ ] Sprossen sind nicht möglich.
- [x] Sprossen sind möglich.

**VSG**
Angabe, ob auf den Zuschneidetisch auch VSG geschnitten werden kann.
- [ ] Der Tisch kann keine VSG-Scheiben schneiden.
- [x] Der Tisch kann VSG-Scheiben schneiden.

**Gasfüllung möglich**
Angabe, ob auf der Maschine Gasfüllungen möglich sind.
- [ ] Gasfüllungen sind nicht möglich.
- [x] Gasfüllungen sind möglich.

**Autoaufleger**
Angabe, ob der Zuschneidetisch über einen automatischen Aufleger verfügt.
- [ ] Der Tisch hat keinen automatischen Aufleger.
- [x] Der Tisch hat einen automatischen Aufleger. In diesem Fall muss für jede Lagerplatte, die auf diesem Tisch zugeschnitten wird, ein Auflegercode vergeben werden.

**Entschichten**
Angabe, ob auf der Maschine Scheiben randentschichtet werden können.
- [ ] Randentschichtungen sind nicht möglich.
- [x] Randentschichtungen sind möglich.

### Zuschnitt Tisch
Auswahl der Nummer von Zuschnitt-Tischen. Diese Einstellung wird bei A+W Business Pro nicht angezeigt.

### Zusatz-Optionen
Diese Einstellungen gelten nur für A+W Business Pro.

**Ausgabeverzeichnis**
Auswahl des Speicherorts für Ausgabedatei.

**Maschinencode**
Auswahl des Maschinencodes. Die Maschinencodes sind im gleichnamigen Dialog hinterlegt. Wenn der gesuchte Code fehlt können Sie ihn in diesem Dialog anlegen.

**ISO-Treiber, ISO-Sektion**
Die Felder werden gefüllt, wenn der Maschinencode für eine ISO-Linie ausgewählt ist.

### Schlüsselwort

**Z-Schnitt**
Die Angabe bestimmt die Lage der Z-Schnitte im Schneidemodus.
- **(<k.A.>)**: Keine Angaben.
- **oben**: Normalerweise ist es günstiger, die Z-Schnitte nach oben, also weg von der Arbeitsbreite zu legen, damit einzelne Schnitte zunächst über die ganze Breite gebrochen und gleich abgestellt werden können. Weisen darüber liegende Scheiben Z-Schnitte auf, ist dann bereits Platz auf dem Brechtisch, um die Scheibe zum Brechen des Z-Schnitts zu drehen.
- **unten**: Der Startpunkt liegt oben
- **beliebig**: Der Startpunkt kann beliebig gewählt werden.

### Schneidmodus
Angabe, in welcher Reihenfolge die Schnitte ausgeführt werden:
- **1 - XYZW**: Der erste Schnitt verläuft senkrecht zum unteren Plattenrand. Danach folgen der Y-Schnitt und der Z-Schnitt. Die weitere Reihenfolge ist wahlweise.
- **2 - ΧΥΖ***: Wie 1. Nach dem Z-Schnitt folgt ein beliebiger anderer Schnitt.
- **3 - XYZZZ**: Der erste Schnitt verläuft senkrecht zum unteren Plattenrand. Danach folgen der Y-Schnitt und anschließend die Z-Schnitte.
- **4 - ΧΥΖΖ**: Wie 3. Jedoch sind nur zwei Z-Schnitte möglich.

*(Abb. H-136 XYZ-Schnitte auf der Lagerplatte)*

**Kostenfaktor Z-Schnitt**
Angabe zur Preiserhöhung von Z-Schnitten. Der Faktor 1 bedeutet, dass der Preis für den Schnitt nicht erhöht wird, Faktor 1,5 erhöht den Preis um die Hälfte.

**Referenzpunkt**
Auswahl des Referenzpunkt für den Schneidmodus. Der Referenzpunkt des Tisches bezeichnet den Punkt mit den Koordinaten 0/0, von dem aus der Schneidmodus aufgebaut ist. Er ist wichtig, um Modelle korrekt zu schneiden.

> **Referenzpunkt vs. Ruheposition des Schneidkopfes**
> Der Referenzpunkt muss nicht mit der Ruheposition des Schneidkopfes übereinstimmen. Bei Bystronic gibt es z. B. gespiegelte Tische, deren Referenzpunkt links vorne ist, während der Schneidkopf rechts vorne in Ruheposition steht. Bei manchen Tischen kann dies als Parameter eingestellt werden.

**Brechstart**
Auswahl des Brechstarts. Der Brechbeginn richtet sich nach den räumlichen Bedingungen im Betrieb und bestimmt die Lager der Restplatte sowie in gewissem Maße die Zuschnittsreihenfolge (erste zu brechende Scheibe oben oder unten).

### Werte

**Einheiten pro Stunde**
Der Wert in diesem Feld hängt davon ab, in welcher Arbeitseinheit die Kapazitätsplanung für diese Maschine die Kapazität berechnen soll, ob in Mannstunden oder Maschinenstunden. Standardmäßig wird 1 eingetragen.
⇨ Tutorial, "Arbeitseinheiten" auf Seite H-43

**Lohnkosten pro Einheit**
Die einzutragenden Personalkosten hängen davon ab, in welcher Arbeitseinheit die Kapazitätsplanung für diese Maschine die Kapazität berechnen soll, z. B. in Mannstunden oder Maschinenstunden. Sie finden eine ausführliche Erläuterung zu diesem Thema unter:
⇨ Tutorial, "Arbeitseinheit = Mannstunde" auf Seite H-44

**Maschinenkosten**
Maschinenkosten pro Stunde, z. B. für Wartung, Reparatur, Verbrauchsmittel.

**Variable Kosten pro Stunde**
Sonstige Kosten, die weder zu Lohn- noch zu Maschinenkosten zählen, können in die Produktionskosten eingerechnet werden, z. B. Versicherung. Den Gesamtbetrag der Versicherung Sie müssen pro Stunde umrechnen.

**Kosten pro Einheit**
Berechnete Gesamtkosten pro Einheit für diese Maschine. Sie bilden die Grundlage für die Kostenkalkulation. Die Kosten werden auf Basis von Personal-, Maschinen- und variablen Kosten und der Arbeitseinheit pro Stunde berechnet.

> **Beispiel**
> Personalkosten/Stunde
> + Maschinenkosten/Stunde dividiert durch Einheiten/Stunde
> + Variable Kosten/Stunde dividiert durch Einheiten/Stunde
> = Kosten/Einheit

**Erfassungsstelle**
Nummer der Erfassungsstelle (Maschine) in A+W Production, auf die sich das Aggregat bezieht. Die Nummern müssen in A+W Business Pro und A+W Production identisch sein. Wenn Sie mit der BDE (Scanner) arbeiten, muss die Nummer der Erfassungsstelle gescannt werden.

**Leistung pro Stunde**
Durchschnittliche Soll-Vorgaben (Erfahrungswerte oder Information des Maschinen-Herstellers) in Mengeneinheiten. Diese Angabe nutzen Sie, wenn Sie z. B. alle Stammdaten bis auf die Vorgabezeiten erfasst haben und vorab in die Kapazitätsplanung einlasten möchten, um die Kapazität in Ihrer Produktion in etwa abschätzen zu können. Damit können Sie den Zeitraum überbrücken, bis alle Vorgabezeiten erfasst sind.

**Serientabelle**
Auswahl der Serientabelle, in der die speziellen Zeiten für Serien definiert sind.
⇨ "Serienfaktoren" auf Seite H-196

### Sperre

**Gesperrt**
Das Aggregat kann für die Planung gesperrt werden.
- [ ] Das Aggregat ist nicht gesperrt.
- [x] Das Aggregat ist gesperrt und kann nicht in die Planung einbezogen werden. Diese Einstellung wählen Sie z. B., wenn eine neue Maschine zunächst getestet werden soll, bevor sie tatsächlich eingesetzt wird.
Wenn Sie eine Maschine wegen einer notwendigen Wartung vorübergehend sperren wollen, wählen Sie den Dialog Aggregat Ausfall:
⇨ "Aggregate Ausfall" auf Seite H-297

**Sperrformel**
Über eine Sperrformel können Sie weitere Restriktionen hinterlegen, die mit den Standard-Mitteln nicht zu erreichen sind.

> **Beispiel**
> Auf einem Aggregat dürfen nur Modelle, sehr kleine und sehr große Scheiben gefertigt werden, da diese Maschine sehr langsam ist.
> Alle Rechteckscheiben mit einer Breite >200 und <2600 sowie einer Höhe >300 und <3600 dürfen nicht auf dieser Maschine geschnitten werden.
> Diese Restriktion kann nur über eine Formel angegeben werden. Falls Sie Formeln einsetzen wollen, wenden Sie sich an Ihren Service-Mitarbeiter bei der A+W Software GmbH.

**Zus. Arbeitsart bei gekoppelten Maschinen**
Zurzeit nicht genutzt.

### Tabelle
In der Übersicht werden je nach Auswahlkriterien die Maschinen aufgeführt, die der Kapazitätsplanung zur Verfügung stehen.

## Aggregate - Restriktionen
**Kapazitätsplanung > Stammdaten > Organisation > Aggregate > Register Restriktionen**

*(Abb. H-137 Aggregate Technische Restriktionen)*

In diesem Register hinterlegen Sie Mindest- und Höchstwerte für die Restriktionsprüfungen. Geben Sie jeweils 0 bis 9999 ein, wenn alle Werte zugelassen sind.

Die Felder für die Definition von Restriktionen werden im Dialog Aggregattypen freigeschaltet.
⇨ "Aggregattypen" auf Seite H-189

Wenn die technischen Restriktionen für eine Maschine bei gleichen Arbeitsarten verschieden sind, definieren Sie diese Restriktionen im Dialog Besondere technische Restriktionen. Die Kapazitätsplanung prüft den Eintrag im Dialog Besondere technische Restriktionen zuerst.
⇨ "Besondere technische Restriktionen" auf Seite H-219

Die Felder im Bereich Aggregat sind zum Register Allgemein beschrieben.
⇨ "Aggregate - Allgemein" auf Seite H-202

### Arbeitsarten / Zeitzuschläge
In diesem Bereich werden alle Arbeitsarten aufgelistet, für die Vorgabezeiten an dieser Maschine definiert sind.
⇨ "Vorgabezeiten (Dialog)" auf Seite H-224

### Technische Restriktionen
Die Felder für die Definition von Restriktionen werden im Dialog Aggregattypen freigeschaltet.
⇨ "Aggregattypen" auf Seite H-189

Geben Sie **0** oder **9999** ein, wenn alle Werte zugelassen sind.

**Breite, Höhe**
Min. und max. Scheibenmaße für diese Maschine.

**SZR**
Min. und max. SZR für diese Maschine.

**Gesamtstärke**
Min. und max. Gesamtdicke für ISO und VSG.

**Glasstärke**
Min. und max. Dicke von Einfachglas.

**Fläche in qm**
Min. und max. Fläche für diese Maschine.

**Gehrungswinkel**
Min. und max. Gehrungswinkel für Facetten.

**Anzahl**
Min. und max. Stückzahl der Auftragsposition. In der Position muss die Menge oder der Mengenbereich geprüft werden. Die Definition, um welche Anzahl es sich handelt, ist maschinenabhängig, z. B.
- Bohrmaschine = Anzahl Bohrlöcher
- Schleifmaschine = Anzahl der Kanten

**Bohrdurchmesser**
Min. und max. Abmessung für diese Maschine.

**Rundeck-Radius**
Min. und max. Abmessung für diese Maschine.

**Diagonale**
Diagonale zwischen den Rollen, z. B. auf dem Förderband vor dem ESG-Ofen.

**Max. Scheibenanzahl**
Maximale Anzahl der Scheiben für eine VSG- bzw. ISO-Einheit, z. B. 3 auf einer ISO-Linie.

**Max. Seitenverhältnis**
Maximales Seitenverhältnis für diese Maschine.

> **Beispiel**
> Sie geben den Wert 5 ein. Dies entspricht einem max. Seitenverhältnis von 1:5. Wenn eine Seite z. B. 500 mm lang ist, dann darf die andere Seitenlänge max. 2500 mm betragen.

**Gewicht bis kg**
Maximales Gewicht einer Einheit.

### Abstände zwischen Schnitten
Bei Schneidtischen mit einer automatischen Brechanlage müssen Sie die Höchst- und Mindestabstände zwischen den Schnitten einstellen. Diese Abstände müssen eingehalten werden, damit die Anlage die Scheiben noch brechen kann.

**Min. Abst. X-X mit Y**
Minimaler Abstand zwischen X-X-Schnitten wenn auch Y-Schnitte ausgeführt werden.

**Min. Abst. X-X ohne Y**
Minimaler Abstand zwischen X-X-Schnitten wenn keine Y-Schnitte ausgeführt werden.

**Max. Abst. X-X-Schnitte**
Maximaler Abstand zwischen X-X-Schnitten.

**Min. Abst. Y-Y mit Z**
Minimaler Abstand zwischen Y-Y-Schnitten wenn auch Z-Schnitte ausgeführt werden.
Bei Schneidetischen mit mehreren Y-Schneidköpfen entspricht der Minimalabstand der Entfernung der Schneidrädchen zweier unmittelbar gegeneinander geschobener Schneidköpfe, z. B. Bystronic XYZVA = 300 mm.

**Min. Abst. Y-Y ohne Z**
Minimaler Abstand zwischen Y-Y-Schnitten wenn keine Z-Schnitte ausgeführt werden.

**Max. Abst. Y-Y-Schnitte**
Maximaler Abstand zwischen Y-Y-Schnitten.

**Min. Restbreite**
Minimale Breite am Rand der Platte.

**Min. Abst. X-Z-Schnitte**
Minimaler Abstand zwischen X und Z-Schnitten.

**Min. Abst. Z-Z-Schnitte**
Minimaler Abstand zwischen Z-Schnitten.

## Kalender
**Kapazitätsplanung > Stammdaten > Organisation > Kalender**

In diesem Dialog legen Sie die Arbeitstage und Schichtzeiten fest. Die Daten können nur gespeichert werden, wenn mindestens eine Schicht angelegt ist. Die Anzahl der Schichten wird in den Firmendaten festgelegt.
⇨ "Voreinstellungen Firmendaten" auf Seite H-183

Wenn keine Kalender in der Kapazitätsplanung angelegt sind, benutzt die Kapazitätsplanung den A+W Business Pro-Standard-Kalender.

Standardmäßig geht die Kapazitätsplanung von einer Schicht aus. Wenn Sie jedoch in Ihrem Betrieb mit mehr als einer Schicht arbeiten, müssen Sie als ersten Schritt die Anzahl der Schichten festlegen. Erst dann legen Sie Kalender für Maschinen mit abweichenden Schichten und Schichtzeiten an.

> **Beispiel**
> Der Kalender lässt maximal 6 Schichten pro Tag zu. Daraus resultieren bei gleichmäßiger Verteilung der Stunden maximal 4 Stunden pro Schicht. Die Verteilung der Anzahl der Stunden pro Schicht ist jedoch variabel, z. B. 5, 3, 5, 3, 5, 3 oder 4, 2, 6, 6, 3, 3.
> Mit diesen Beispielen soll verdeutlicht werden, dass Sie nicht an eine gleichmäßige Verteilung gebunden sind.
> Bei 4 Schichten können Sie bei gleichmäßiger Verteilung pro Schicht maximal 6 Stunden eintragen.
> Die Gesamtzeit der Stunden x Schichten pro Tag darf logischerweise 24 Stunden nicht überschreiten.

> **Kalender ändern**
> Wenn Sie einen Kalender bearbeitet oder angelegt haben, müssen Sie A+W Business Pro neu starten, damit die Daten beim Einlasten zur Verfügung stehen.

In diesem Dialog finden Sie folgende Register:
- "Kalender - Auswahl" auf Seite H-212
- "Kalender - Kalender" auf Seite H-214

### Menü Funktionen
**Kapazitätsplanung > Stammdaten > Organisation > Kalender Aggregat**

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Kalender zu schließen.

Folgende Einträge werden angezeigt:
- **Kopieren:** Öffnet den Dialog Kalender kopieren, um einen Kalender zu übertragen, z. B. in ein neues Jahr.
⇨ "Kalender kopieren" auf Seite H-215

- **Schichtzeiten:** Öffnet den Dialog Einstellung Schichten, in dem Sie den Schichtübergang und die Sperrzeiten festlegen können.
⇨ "Einstellungen Schichten" auf Seite H-187
Sie müssen Administratorrechte haben, um den Dialog zu öffnen. Zusätzlich muss in den Firmendaten die Checkbox Schichtwechseltabelle verwenden markiert sein.
⇨ "Schichtwechseltabelle verwenden" auf Seite H-186

## Kalender – Auswahl
**Kapazitätsplanung > Stammdaten > Organisation > Kalender Aggregat > Register Auswahl**

*(Abb. H-138 Kalender - Auswahl)*

In diesem Register legen Sie Kalender für Arbeitsarten, Aggregate, Produktionsbereiche oder Mandanten an.
Wenn Sie für einen Produktionsbereich oder ein Aggregat keinen eigenen Kalender anlegen, gilt der allgemeine Kalender.
⇨ Tutorial, "Kalender anpassen" auf Seite H-50

### Identifikation
Die Beschriftung der beiden Auswahlfelder richtet sich nach dem gewählten Modus.

**Arbeitsart, Aggregat**
Arbeitsart und Maschine, für die der Kalender gilt.

**Produktionsbereich, Mandant**
Produktionsbereich und Mandant, für die der Kalender gilt.

**Jahr**
Jahr, für das der Kalender bearbeitet oder angelegt werden sollen.

### Modus
Mit der Wahl der Option legen Sie fest, wofür Sie den Kalender anlegen wollen. Die Felder sind nur im Auswahlmodus freigeschaltet.
- **Arbeitsart, Aggregat:** Mit dieser Einstellung legen Sie einen Kalender für die Arbeitsart und/oder die Maschine an.
- **Produktionsbereich/Mandant:** Mit dieser Einstellung legen Sie einen Kalender für den Produktionsbereich und/oder den Mandanten an. Um einen allgemeinen Kalender anzulegen, wählen Sie diese Option und tragen den Produktionsbereich <k. A.> und für den Mandanten alle ein.

### Kalender-Tabellen
In der Übersicht werden alle Kalender angezeigt, die den Auswahlkriterien entsprechen. Wenn Sie die Auswahl nur nach dem Modus Arbeitsart oder Produktionsbereich eingegrenzt haben, werden alle Kalender angezeigt.

## Kalender – Kalender
**Kapazitätsplanung > Stammdaten > Organisation > Kalender Aggregat > Register Kalender**

*(Abb. H-139 Kalender - Kalender)*

In diesem Register legen Sie die Arbeitszeit pro Schicht fest. Die Anzahl der Schichten wird in den Firmendaten angegeben.
⇨ "Voreinstellungen Firmendaten" auf Seite H-183

### Arbeitswoche

**Montag - Sonntag**
Wenn Sie die Schichtzeit eines Wochentags ändern wollen, dann müssen Sie die entsprechende Checkbox aktivieren und die neue Stundenzahl eintragen. Die Änderung gilt nur für das angezeigte Datum. Sie müssen die neue Schichtzeit ggf. auf das Jahr oder die Kalenderwoche übertragen.

**Stunden pro Schicht**
Anzahl der verfügbaren Stunden pro Wochentag und Schicht.

> **Zusätzliche Schicht einrichten**
> Wenn Sie eine zusätzliche Schicht für ein Aggregat oder einen Produktionsbereich einrichten, müssen Sie alle Schichtzeiten neu eintragen.
> Es reicht nicht, nur die Stunden der neuen Schicht anzugeben, weil bei der Übertragung auf das Jahr (oder die Woche) die leeren Felder ebenfalls übernommen werden. Damit sind die alten Schichtzeiten gelöscht.

### Schichten in Kalender übernehmen
**[Auf Jahr übertragen]**
Überträgt die Änderungen auf alle entsprechenden Wochentage des Jahres. Nur die Schichtzeiten der Wochentage werden übertragen, bei denen die Checkbox markiert ist.

**[Auf KW übertragen]**
Überträgt die Änderungen auf alle Tage der Kalenderwoche.

### Kalenderwoche
**Gehe zu**
Auswahl der Kalenderwoche.

**[Zur aktuellen KW]**
Wechselt die Darstellung im Bereich Arbeitswoche, um die Schichtzeiten für die aktuelle Kalenderwoche zu bearbeiten.

## Kalender kopieren
**Kapazitätsplanung > Stammdaten > Organisation > Kalender > Menü Funktionen > Kopieren**

*(Abb. H-140 Kalender kopieren)*

In diesem Dialog kopieren Sie den Kalender eines Aggregats oder eines Produktionsbereichs, z. B. um ihn auf ein anderes Aggregat zu übertragen.

### Kalender Auswahl Quelle
Die Beschriftung der beiden Auswahlfelder richtet sich nach dem gewählten Modus.

**Arbeitsart, Aggregat**
Arbeitsart und Maschine, für die der Kalender angelegt ist.

**Produktionsbereich, Mandant**
Produktionsbereich und Mandant, für die der Kalender angelegt ist.

**Jahr**
Jahr, für das der Kalender angelegt ist.

### Kalender Auswahl Ziel
**Arbeitsart, Aggregat**
Arbeitsart und Aggregat, auf die der Kalender übertragen werden soll.

**Produktionsbereich, Mandant**
Produktionsbereich und Mandant, auf die der Kalender übertragen werden soll.

## Übergangsmatrix
**Kapazitätsplanung > Stammdaten > Organisation > Übergangsmatrix**

*(Abb. H-141 Übergangs-Matrix)*

In diesem Dialog tragen Sie ein, wie lange es dauert, bis die Position von einem Produktionsbereich in den nächsten gelangt. Die Zeiten können Sie je nach Auftragspriorität unterschiedlich gestalten.

> **Beispiel**
> Der Übergang vom Produktionsbereich Zuschnitt in den Produktionsbereich Bearbeitung kann normalerweise in der gleichen Schicht erfolgen.
> Der Übergang vom Produktionsbereich ESG in den Produktionsbereich ISO-Fertigung benötigt mehrere Schichten bzw. 1 Tag.

⇨ Tutorial, "Übergangsmatrix und Übergangszeiten" auf Seite H-69

**Auftragspriorität**
Auswahl, bei welcher Auftragspriorität die Übergangszeit berücksichtig werden soll. Sie können zwischen folgenden Prioritäten wählen:
- **Normal:** Die Übergangszeit gilt für alle Aufträge, in denen keine besondere Priorität angegeben ist. Dies ist die Standard-Einstellung.
- **Eilt:** Die angegebene Übergangszeit gilt für Eilaufträge. Wenn Übergangszeiten für Eilaufträge verkürzt werden können, dann muss für die entsprechende Kombination von Produktionsbereichen eine abweichende Übergangszeit hinterlegt werden.
- **Zugabe:** Diese Priorität bedeutet, dass der Auftrag so gefertigt werden soll, dass er Reste und Restplatten verbraucht, die beim Zuschnitt anderer Aufträge entstehen.
- **Abruf:** Die Übergangzeit gilt nur für Aufträge, die auf Abruf gefertigt werden.

> **Auftragspriorität berücksichtigen**
> Wenn außer der Auftragspriorität Normal auch z. B. die Priorität Eilt berücksichtigt werden soll, dann muss für die jeweilige Kombination von Produktionsbereichen eine eigene Übergangszeit eingerichtet sein. Dies gilt für alle Übergangszeiten, die für Eilaufträge auch verkürzt werden können.

**Von Produktionsbereich**
Produktionsbereich, aus dem die Position kommt.

**Nach Produktionsbereich**
Folge-Produktionsbereich, in den die Position wechselt.

**Übergangszeit**
Zeit, die ein Glas zum Wechsel in den nächsten Produktionsbereich braucht. Die Werte werden in Tagen eingegeben:
- 0 = gleicher Tag bzw. gleiche Schicht
- 0,01 bis 0,99 = Folgeschichten
- 1 = Folgender Tag

### Beispiele für die Berechnung des Übergangs

| Anz. Schichten | 1/Anzahl Stunden | Gleiche Schicht | Nächste Schicht | z.B. | Übernächste S. | z.B. | Über-Über-nächste S. | z.B. | Über-Über-Über-nächste S. | z.B. |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 4 | 1/4=0,25 | 0 | 0,1-0,24 | 0,2 | 0,26-0,49 | 0,4 | 0,51-0,74 | 0,6 | 0,76-1 | 1 |
| | Übergang: S1-Mo | S2-Mo | | S3-Mo | | S4-Mo | | S1-Di | | |
| | Übergang: S2-Mo | S3-Mo | | S4-Mo | | S1-Di | | S2-Di | | |
| 3 | 1/3=0,33 | 0 | 0,1-0,3 | 0,2 | 0,4-0,6 | 0,5 | 0,7-1 | 1 | | |
| | Übergang: S1-Mo | S2-Mo | | S3-Mo | | S1-Di | | | | |
| | Übergang: S2-Mo | S3-Mo | | S1-Di | | S2-Di | | | | |
| 2 | 1/2=0,5 | 0 | 0,1-0,49 | 0,3 | 0,51-0,1 | 1 | | | | |
| | Übergang: S1-Mo | S2-Mo | | S1-Di | | | | | | |
| | Übergang: S2-Mo | S1-Di | | S2-Di | | | | | | |

*Tab. H-4 Übergangszeiten in Tagen*

> **Flexible Übergangszeit**
> Sie können statt eines festen Wertes auch eine Formel eintragen, wenn die Übergangszeit von unterschiedlichen Parametern abhängt, z. B. von der Dicke. Mit einem Rechtsklick in das Feld wird der Dialog Formelsuche geöffnet.
> Wenn Sie mit Formeln arbeiten wollen, lassen Sie sich von Ihrem Service-Mitarbeiter bei der A+W Software GmbH unterstützen.

## Besondere technische Restriktionen
**Kapazitätsplanung > Stammdaten > Organisation > Besondere technische Restriktionen**

*(Abb. H-142 Besondere technische Restriktionen)*

In diesem Dialog geben Sie Restriktionen für Aggregate an, die sich auf bestimmte Arbeitsarten beziehen.
Wenn auf einer Maschine unterschiedliche Arbeitsarten ausgeführt werden können, z. B. Lochbohren und Eckausschnitt, können Sie pro Arbeitsart unterschiedliche Prüfwerte angeben. Wenn die Kapazitätsplanung keine Definition für die Arbeitsart findet, werden die allgemeinen technischen Restriktionen für diese Maschine geprüft.
⇨ "Aggregate – Restriktionen" auf Seite H-208

Die verfügbaren Parameter sind abhängig von den Einstellungen im Dialog Aggregattypen.
⇨ "Aggregattypen" auf Seite H-189

### Menü Funktionen
Über dieses Menü können Sie die Werte aus dem Standard-Aggregat übertragen. Bereits eingetragene Werte werden ohne Abfrage überschrieben.
⇨ "Aggregate - Restriktionen" auf Seite H-208

### Identifikation
**Arbeitsart**
Arbeitsart, für die die Restriktionen gelten.

**Aggregat**
Maschine, für die die Restriktionen gelten, wenn die entsprechende Arbeitsart ausgeführt wird.

### Technische Restriktionen (Minimal/Maximal)
Geben Sie **0** oder **9999** ein, wenn alle Werte zugelassen sind.

- **Breite, Höhe**: Min. und max. Maße für diese Maschine.
- **SZR**: Min. und max. SZR für diese Maschine.
- **Gesamtstärke**: Min. und max. Gesamtdicke für ISO und VSG für diese Maschine.
- **Glasstärke**: Min. und max. Dicke von Einfachglas.
- **Anzahl**: Min. und max. Stückzahl der Auftragsposition. In der Position muss die Menge oder der Mengenbereich geprüft werden. Die Definition, um welche Anzahl es sich handelt, ist maschinenabhängig, z. B.:
    - Bohrmaschine = Anzahl Bohrlöcher
    - Schleifmaschine = Anzahl der Kanten
- **Bohrdurchmesser**: Min. und max. Abmessung für diese Maschine.
- **Rundeck-Radius**: Min. und max. Abmessung für diese Maschine.
- **Fläche in qm**: Min. und max. Fläche für diese Maschine.
- **Diagonale**: Diagonale zwischen den Rollen, z. B. auf dem Förderband vor dem ESG-Ofen.
- **Gehrungswinkel**: Min. und max. Gehrungswinkel für Facetten.

### Sonstige Technische Restriktionen
Geben Sie **9999** ein, wenn alle Werte zugelassen sind.

- **Serien-Tabelle**: Nummer der Serientabelle, die bei der Produktion von Serien herangezogen wird.
⇨ Softwarereferenz, "Serienfaktoren" auf Seite H-196
- **Max. Scheibenanzahl**: Maximale Anzahl an Scheiben, die für eine VSG- bzw. ISO-Einheit auf dieser Maschine erlaubt sind.
- **Gewicht bis kg**: Maximales Gewicht.
- **Max. Seitenverhältnis**: Maximales Seitenverhältnis für diese Maschine.
  > **Beispiel**
  > Der Wert 5 entspricht einem max. Seitenverhältnis von 1:5.
  > Wenn eine Kantenlänge der Scheibe z. B. 500 mm beträgt, dann darf die andere Kante max. 2500 mm lang sein.

### Technische Restriktionen (Optionen)

**Modelle möglich**
Angabe, ob auf der aktuellen Maschine Modelle gefertigt werden können.
- [ ] Modelle sind nicht möglich.
- [x] Modelle sind möglich.

**Sprossen möglich**
Angabe, ob auf der aktuellen Maschine Sprossen gefertigt werden können.
- [ ] Sprossen sind nicht möglich.
- [x] Sprossen sind möglich.

**Gasfüllung möglich**
Angabe, ob auf der aktuellen Maschine Gasfüllungen möglich sind.
- [ ] Gasfüllungen sind nicht möglich.
- [x] Gasfüllungen sind möglich.

**Scheiben drehbar**
Angabe, ob die Scheiben auf der aktuellen Maschine gedreht werden können.
- [ ] Scheiben können nicht gedreht werden.
- [x] Scheiben können gedreht werden.

**Kantenschutz möglich**
Angabe, ob auf der aktuellen Maschine Kantenschutz angebracht werden kann.
- [ ] Kantenschutz kann nicht angebracht werden.
- [x] Kantenschutz kann angebracht werden.

### Übersicht Sonder-Restriktionen
In der Übersicht sind die Arbeitsarten und Maschinen aufgeführt, für die besondere Restriktionen hinterlegt sind.

## Orga Übersicht
**Kapazitätsplanung > Stammdaten > Organisation > Orga Übersicht**

*(Abb. H-143 Orga Übersicht)*

In diesem Dialog prüfen Sie, welche Maschinen und Arbeitsarten den Produktionsbereichen zugeordnet sind.

### Auswahl
**Mandant**
Mandant, dem der Produktionsbereich zugeordnet ist.

**Produktionsbereich**
Produktionsbereich, dem die Aggregate zugeordnet sind.

### Auflösungstiefe
Mit der Wahl der Option filtern Sie die Anzeige in der Übersicht.

### Ansicht
Die Spalten in der Übersicht sind abhängig von der Auflösungstiefe.
- **Produktionsbereich:** Produktionsbereich, dem das Aggregat (die Maschine) zugeordnet ist.
- **Aggregat:** Aggregate, die dem jeweiligen Produktionsbereich zugeordnet sind.
- **Arbeitsart:** Arbeitsarten, die dem jeweiligen Aggregat zugeordnet sind.
- **Zuschläge:** Typ der Vorgabezeit, die für die jeweilige Arbeitsart zur Berechnung herangezogen werden.

# Vorgabezeiten
**Kapazitätsplanung > Stammdaten > Vorgabezeiten**

In diesem Programmbereich finden Sie die Dialoge, in denen die Vorgaben für die Zeitberechnung hinterlegt sind.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Vorgabezeiten (Dialog)" auf Seite H-224
- "Vorgabezeiten ändern" auf Seite H-233
- "Vorgabezeiten kopieren" auf Seite H-233
- "Sonderzeiten" auf Seite H-234
- "Besondere Prioritäten" auf Seite H-235

## Vorgabezeiten (Dialog)
**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten**

In diesem Dialog tragen Sie die für Ihre Maschinen ermittelten Zeitwerte pro Arbeitsart und Maschine ein. Ob der Zeitwert abhängig von laufenden Metern, Quadratmetern oder Stück berechnet wird, hängt von der Maschine ab.

In diesem Dialog finden Sie folgende Register:
- "Vorgabezeiten - Zeitauswahl" auf Seite H-225
- "Vorgabezeiten - Matrix" auf Seite H-228
- "Vorgabezeiten – Vektor" auf Seite H-230
- "Vorgabezeiten - Einzelzeit" auf Seite H-231
- "Vorgabezeiten – Würfel" auf Seite H-232

### Eintrag von Zeitwerten in Stunden
Die Zeiten werden nicht in Minuten, sondern in Stunden hinterlegt. Das heißt, dass Sie die gemessenen Minuten in Stunden umrechnen müssen:

| Minuten | Zeiteintrag in Std. |
| :--- | :--- |
| 60 | 1 |
| 30 | 0,5 |
| 15 | 0,25 |
| 7,5 | 0,125 |
| 3,75 | 0,0625 |
| 1,875 | 0,03125 |

### Menü Funktionen
**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten**

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Vorgabezeiten zu schließen. Folgende Einträge werden angezeigt:
- **Ändern:** Öffnet den gleichnamigen Dialog, um die Vorgabezeiten um einen Faktor zu erhöhen oder zu reduzieren.
⇨ "Vorgabezeiten ändern" auf Seite H-233
- **Kopieren:** Öffnet den gleichnamigen Dialog, um die Vorgabezeiten aus der Standard-Maschine zu kopieren.
⇨ "Vorgabezeiten kopieren" auf Seite H-233

## Vorgabezeiten – Zeitauswahl
**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten > Register Zeitauswahl**

*(Abb. H-144 Vorgabezeiten - Tabellenauswahl)*

In diesem Register legen Sie den Typ der Berechnung und die Priorität fest.
⇨ Tutorial, "Vorgabezeiten" auf Seite H-60

### Identifikation

**Arbeitsart**
Arbeitsart, für die die Vorgabezeit gilt.

**Aggregat**
Maschine, an der die Arbeitsart die Vorgabezeit benötigt.

### Typ
Typ der Vorgabezeit:
- **0 - Basiszeit:** Gestoppte Zeit für einen Arbeitsgang.
  ⇨ "Eintrag von Zeitwerten in Stunden" auf Seite H-224
- **1 - Zeitzuschlag:** Ein Zeitzuschlag wird für Arbeitsarten benötigt, die mehr Aufwand erfordern, z. B. für das Zuschneiden von Modellen.
- **2 - Alternativer Vorgang:** Diese Vorgabezeit wird nur herangezogen, wenn für die Arbeitsart eine alternative Arbeitsart existiert. In diesem Fall müssen Sie im Feld Altern. Masch.-Nr. die alternative Maschinennummer eintragen.
- **3 - Alternative ohne Stückliste:** Als VSG-Produzent ist Ihr VSG-Artikel standardmäßig mit einer Stückliste hinterlegt. Soll aber z. B. eine VSG-Scheibe manchmal nicht produziert, sondern direkt aus einem VSG-Bandmaß geschnitten werden, dann darf die Stückliste nicht berücksichtigt werden. Für die Arbeitsart VSG schneiden würden Sie Alternative ohne Stückliste wählen. In diesem Fall müssen Sie im Feld Altern. Masch.-Nr. die alternative Maschinennummer eintragen.
- **4 - Vorgang ignorieren:** Für einen Eckausschnitt müssen z. B. 3 Arbeitsgänge gemacht werden: 1. Bohren (von Eckloch), 2. Zuschnitt und 3. Schleifen. Die CNC-Maschine kann alles in einem, d. h., dort wird nur die Lochbohrung berücksichtigt. Die beiden anderen Arbeitsarten werden ignoriert. Sie müssen also nur der Arbeitsart Bohren eine Vorgabezeit zuweisen, die den gesamten Vorgang umfasst. Den anderen beiden Arbeitsarten weisen Sie auf dieser Maschine dann den Wert Vorgang ignorieren zu.

### Priorität
Wenn mehrere Maschinen für eine Arbeitsart zur Verfügung stehen, müssen Sie festlegen, welche Maschine zuerst auf freie Kapazitäten geprüft werden soll und welche z. B. nur manuell ausgewählt werden kann.
Wenn zwei Maschinen die gleiche Priorität haben, dann prüft die Kapazitätsplanung die Kosten, die pro Maschine definiert sind. In diesem Fall wird automatisch die günstigere Maschine ausgewählt.
Wenn keine Kosten pro Maschine hinterlegt sind, kann das Programm keine günstigste Maschine finden. In diesem Fall muss die Priorität bei gleichen Maschinen eindeutig sein.
- **9:** höchste Priorität (Standard-Maschine). Diese Maschinen werden immer zuerst ausgelastet.
- **8 bis 1:** absteigende Prioritäten. Diese Maschinen werden je nach Auslastung ausgewählt.
- **0:** niedrigste Priorität. Diese Maschinen werden nur dann eingesetzt, wenn alle anderen (gleichartigen) Maschinen ausgelastet sind.
- **-1:** zur manuellen Einlastung. Diese Maschinen werden von der automatischen Einlastung nur bei Engpässen ausgewählt.
- **-2, -3:** nur zur manuellen Einlastung. Diese Maschinen werden nie von der automatischen Einlastung ausgewählt.

### Alternative Masch.-Nr.
In diesem Feld muss die Maschinen-Nummer aus A+W Production eingetragen werden, wenn im Feld Typ der Wert Alternativer Vorgang oder Alternative ohne Stückliste ausgewählt ist.

### Gruppiert nach
Mit der Wahl der Option legen Sie fest, wie die Darstellung in der Übersicht gruppiert sein soll. Die Felder sind nur im Auswahlmodus freigeschaltet.
- **Arbeitsart:** Zu jeder Arbeitsart werden die zugeordneten Aggregate angezeigt.
- **Aggregat:** Zu jedem Aggregat werden die Arbeitsarten mit den definierten Zeiten angezeigt.

### Sonstige Zuschläge
**Tabelle**
Verweis auf Zuschlagstabelle, z. B. für Übergrößen. Diese Zuschlagstabellen sind im Dialog Sonderzeiten angelegt.
⇨ "Sonderzeiten" auf Seite H-234

### Übersicht
In der Übersicht sind alle Vorgabezeiten mit den zugeordneten Arbeitsarten aufgeführt. Mit einem Doppelklick auf Zuordnungen können werden die zugeordneten Produkte, Produktarten, Produktgruppen und/oder Warengruppen angezeigt. Die Gruppierung legen Sie im Auswahlmodus fest.

## Vorgabezeiten – Matrix
**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten > Register Matrix**

*(Abb. H-145 Vorgabezeiten – Matrix)*

In diesem Register legen Sie Vorgabezeiten fest, die nach zwei Grenztypen gestaffelt sind.
⇨ Tutorial, "Vorgabezeiten" auf Seite H-60

**Grenztyp1, Grenztyp2**
Der Grenztyp legt die Maßeinheit für die Staffelung der Zeit fest. Sie können z. B. Dicke und Fläche wählen. Das Eingabefeld für den Grenzwert wird freigeschaltet, wenn Sie eine neue Spalte/Zeile einfügen. Der Grenzwert bezieht sich auf den Grenztyp.
⇨ Stammdaten, "Grenzmengen" auf Seite B-879

### Spezifikation
**Zeiteinheit**
Die Einheit bezieht sich auf den Grenzwert. Der Grenzwert kann sich z. B. auf Stück, auf Quadratmeter, auf Laufmeter usw. beziehen.

### Dreiecksform
Sie können in einer Matrix oder in einem Würfel die Zeiten so erfassen, dass die angegebenen Grenzwerte vertauscht werden dürfen, z. B. Höhe und Breite.
- [ ] Die Grenztypen dürfen nicht vertauscht werden. In diesem Fall müssen Sie in allen Feldern pro Spalte/Zeile eine Zeit eintragen. Wählen Sie diese Einstellung für Gläser, bei denen es wichtig ist, in welcher Richtung sie geschnitten werden.
- [x] Die Grenztypen dürfen vertauscht werden. Damit müssen Sie die Zeit nur in jeweils einer der Kombinationen der Grenztypen eintragen.

### Mindestangaben
Die Mindestangaben werden bei der Einlastung geprüft. Bei Unterschreitung der Werte wird eine Meldung angezeigt und/oder ein Zuschlag erhoben.

**Mindestzeit**
Sie können angeben, wie viel Zeit für eine Position mindestens berechnet wird.

### Übersicht
In der Übersicht geben Sie in jedem Feld pro Zeile und Spalte die Zeit ein, die bei dieser Kombination von Grenztypen für die Arbeitsart benötigt wird.

## Vorgabezeiten – Vektor
**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten > Register Vektor**

*(Abb. H-146 Vorgabezeiten – Vektor)*

In diesem Register hinterlegen Sie Vorgabezeiten, die nach einem Grenztyp gestaffelt sind, z. B. nach Dicke.
Die Felder sind zum Register Matrix beschrieben.
⇨ "Vorgabezeiten - Matrix" auf Seite H-228

## Vorgabezeiten – Einzelzeit
**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten > Register Einzelzeit**

*(Abb. H-147 Vorgabezeiten – Einzelzeit)*

In diesem Register hinterlegen Sie Einzelzeiten. In der Regel hinterlegen Sie Einzelzeiten für die Arbeitsgänge. Zu jeder Kombination von Aggregat und Arbeitsart wird eine Zeile angezeigt. Einträge in roter Schrift zeigen an, dass keine Zeiten definiert sind.

### Übersicht
- **Aggregat:** Aggregat, das im Register Zeitauswahl markiert ist.
- **Arbeitsart:** Arbeitsart, zu der am gewählten Aggregat eine Zeit angegeben wird.
- **Zeit:** Gemessene Zeit.
- **Zeiteinheit:** Einheit, auf die sich die gemessene Zeit bezieht, z. B. auf Stück, auf Quadratmeter, auf Laufmeter usw.
- **Mindestzeit:** Zeit, die für eine Position mindestens berechnet wird, wenn die benötigte Zeit darunter liegt.
- **Typ:** Typ der Zeit. Der Typ legt fest, wie die Zeit berechnet werden soll, z. B. als Basiszeit oder Zuschlag.
  ⇨ "Vorgabezeiten - Zeitauswahl" auf Seite H-225

## Vorgabezeiten – Würfel
**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten > Register Würfel**

*(Abb. H-148 Vorgabezeiten – Würfel)*

In diesem Register hinterlegen Sie Vorgabezeiten, die nach drei Grenztypen gestaffelt sind, z. B. nach Höhe, Breite und Dicke.
Die Felder sind zum Register Matrix beschrieben.
⇨ "Vorgabezeiten – Matrix" auf Seite H-228

## Vorgabezeiten ändern
**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten > Menü Funktionen > Ändern**

*(Abb. H-149 Vorgabezeiten ändern)*

In diesem Dialog können Sie die Vorgabezeiten für ein Aggregat oder eine Arbeitsart ändern. Wenn Sie z. B. den Faktor 1,5 eintragen, werden alle Zeiten der ausgewählten Kombination von Aggregat und Arbeitsart um die Hälfte erhöht. Der Faktor 0,5 würde die Zeiten auf die Hälfte reduzieren.

## Vorgabezeiten kopieren
**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Vorgabezeiten > Menü Funktionen > Kopieren**

*(Abb. H-150 Vorgabezeiten kopieren)*

In diesem Dialog können Sie Vorgabezeiten von einer Maschine und Arbeitsart kopieren, um sie auf eine andere Maschine und Arbeitsart zu übertragen. Sie können dabei Werte um einen Faktor erhöhen oder vermindern.

## Sonderzeiten
**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Sonderzeiten**

*(Abb. H-151 Sonderzeiten)*

In diesem Dialog definieren Sie Zeitzuschläge für besonders aufwendige Bearbeitungen, z. B. für Sondergrößen. Die Zeitschläge können Sie im Dialog Vorgabezeiten im Bereich Sonstige Zuschläge zuweisen. Sonderzeiten, die nach den gleichen Kriterien angelegt sind, können in Gruppen (Tabellen) zusammengefasst werden.
⇨ Tutorial, "Sonderzeiten" auf Seite H-63

Eine weitere Möglichkeit der Definition von Zeitzuschlägen in Form von Faktoren besteht über die Zuordnungsdialoge.
⇨ "Vorgabezeiten (Dialog)" auf Seite H-224
⇨ "Zuordnen" auf Seite H-237

### Zeitzuschlag für
**Nummer**
Benutzerdefinierte Nummer (ID) der Tabelle.

**Bezeichnung**
Name der Tabelle, z. B. Übergrößen.

### Zuschläge (Übersicht)
In der Übersicht werden alle definierten Zuschläge aufgeführt.

### Zuschläge
In der Übersicht werden die Staffelungen des Zeitzuschlags angezeigt, der im Register Tabelle markiert ist.
- **Bis Grenze1, 2:** Wert pro Grenztyp, bis zu dem der Zuschlag berechnet werden soll.
- **Grenztyp1, 2:** Grenztyp, auf den sich der Grenzwert bezieht, z. B. die Kantenlänge für die Berechnung von Übergrößen.
  ⇨ Stammdaten, “Grenzmengen" auf Seite B-879
- **Zuschlag:** Höhe des Zuschlags. Der Wert bezieht sich auf die Zuschlagseinheit.
- **Zuschlagseinheit:** Einheit, mit der der Zuschlag berechnet werden soll.
- **Zuschlagsart:** Basis, auf die der Zuschlag bezogen wird.

## Besondere Prioritäten
**Kapazitätsplanung > Stammdaten > Vorgabezeiten > Besondere Prioritäten**

*(Abb. H-152 Besondere Prioritäten)*

In diesem Dialog tragen Sie pro Maschine und Arbeitsart die Prioritäten nach zusätzlichen Kriterien ein, z. B. nach Warengruppen, pro Dicke, pro Kunde. Wenn in den Feldern null (0) steht, gilt die besondere Priorität übergreifend, z. B. für den gewählten Kunden oder bei der angegebenen Anzahl.

Dies ist beispielsweise in folgenden Fällen sinnvoll:
- Wenn für eine Arbeitsart mehrere gleichartige Maschinen zur Verfügung stehen.
- Wenn Kunden spezielle Bearbeitungen wünschen, die nur auf speziellen Maschinen ausgeführt werden sollen oder können.

### Felder
- **Arbeitsart**: Arbeitsart, für die eine Ausnahme definiert ist.
- **Aggregat**: Aggregat, an dem die Arbeitsart ausgeführt wird.
- **Kunde**: Kunde, für den die Priorität gilt.
- **Firma**: Mandant, für den die Priorität gilt.
- **WGR**: Warengruppe, für die die Priorität gilt.
- **Kantenlänge**: Kantenlänge in mm, ab der die Priorität gilt.
- **Dicke >=**: Glasdicke in mm, ab der die Priorität gilt. 0 = Alle Dicken.
- **Anzahl >**: Anzahl, ab der die Priorität gilt, z. B. Anzahl der Bohrungen, der Eckausschnitte.
- **Bohrdurchmesser >=**: Durchmesser einer Bohrung in mm, ab dem die Priorität gilt.
- **Priorität**: Die Ziffern haben folgende Bedeutung:
    - **9**: höchste Priorität (Standard-Maschine). Diese Maschinen werden immer zuerst ausgelastet.
    - **8 bis 1**: absteigende Prioritäten. Diese Maschinen werden je nach Auslastung ausgewählt.
    - **0**: niedrigste Priorität. Diese Maschinen werden nur dann eingesetzt, wenn alle anderen (gleichartigen) Maschinen ausgelastet sind.
    - **-1**: zur manuellen Einlastung. Diese Maschinen werden von der automatischen Einlastung nur bei Engpässen ausgewählt.
    - **-2, -3**: nur zur manuellen Einlastung. Diese Maschinen werden nie von der automatischen Einlastung ausgewählt.

# Zuordnen
**Kapazitätsplanung > Stammdaten > Zuordnen**

In diesen Dialogen ordnen Sie die Basisprodukte von A+W Business Pro (Einfachglas, VSG, ESG, Bearbeitungen, Modelle, Sprossen usw.) den Arbeitsarten zu.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Produktarten" auf Seite H-238
- "WGR" auf Seite H-240
- "Produktgruppe" auf Seite H-241
- "Produkte" auf Seite H-242
- "Kombi-Produktart" auf Seite H-243
- "Sonderzuordnung 1" auf Seite H-244
- "Sonderzuordnung 2" auf Seite H-245
- "Sonderzuordnung 3" auf Seite H-247
- "Sonderzuordnung 4" auf Seite H-249
- "Kombi-Produktgruppe" auf Seite H-251
- "Lagerartikel" auf Seite H-252

## Produktarten
**Kapazitätsplanung > Zuordnen > Produktarten**

*(Abb. H-153 Produktarten)*

In diesem Dialog ordnen Sie den A+W Business Pro-Produktarten die Arbeitsarten in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für die jeweilige Produktart ausgeführt werden. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll.
⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-102

**Produktart**
Produktart, der Arbeitsarten zugeordnet sind.

### Arbeitsarten
In der Übersicht werden die zugeordneten Arbeitsarten angezeigt.

**#**
Nummer der Reihenfolge.

**Arbeitsart**
Produktnummer und Bezeichnung der Arbeitsart. Wenn Sie <k.A.> eintragen, wird die Produktart ignoriert. Das ist z. B. für die Produktart Leistungen sinnvoll.

**Faktor**
Die bei der Einlastung berechnete Zeit wird mit diesem Faktor multipliziert.
- 0 oder 1: Die Zeit wird nicht erhöht oder vermindert.
- >1: Ein Faktor von z. B. 1,5 entspricht einer Zeiterhöhung von 50%.

### Schaltflächen
**[Neu], [Löschen]**
Mit diesen Schaltflächen schalten Sie eine neue Zeile frei oder löschen einen markierten Eintrag.

**Pfeilschaltflächen**
Mit diesen Schaltflächen können Sie die Reihenfolge der Arbeitsarten ändern.
Für die Produktart ESG könnte die Zuordnung z. B. wie folgt aussehen:
- Glas waschen
- Kontrolle
- ESG fertigen
- Verpacken verarbeitetes ESG
- Verladen

### Übersicht Zuordnungen
In der Übersicht werden die Produktarten angezeigt, denen Arbeitsarten zugeordnet sind.

## WGR
**Kapazitätsplanung > Zuordnen > WGR**

*(Abb. H-154 Warengruppen)*

In diesem Dialog ordnen Sie den A+W Business Pro-Warengruppen die Arbeitsarten in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für die jeweilige Warengruppe ausgeführt werden. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll.
⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-102

### Identifikation
**Warengruppe**
Warengruppe, der Arbeitsarten zugeordnet sind.

### Arbeitsarten
Die Felder und Schaltflächen in diesem Bereich sind zum Dialog Produktarten beschrieben.
⇨ "Produktarten" auf Seite H-238

### Übersicht Zuordnungen
In der Übersicht werden die Warengruppen angezeigt, denen Arbeitsarten zugeordnet sind.

## Produktgruppe
**Kapazitätsplanung > Zuordnen > Produktgruppe**

*(Abb. H-155 Produktgruppen)*

In diesem Dialog ordnen Sie den A+W Business Pro-Produktgruppen die Arbeitsarten in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für die jeweilige Produktgruppe ausgeführt werden. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll.
⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-102

### Identifikation
**Produktgruppe**
Produktgruppe, der Arbeitsarten zugeordnet sind.

### Arbeitsarten
Die Felder und Schaltflächen in diesem Bereich sind zum Dialog Produktarten beschrieben.
⇨ "Produktarten" auf Seite H-238

### Übersicht Zuordnungen
In der Übersicht werden die Produktgruppen angezeigt, denen Arbeitsarten zugeordnet sind.

## Produkte
**Kapazitätsplanung > Zuordnen > Produkte**

*(Abb. H-156 Produkte)*

In diesem Dialog ordnen Sie den A+W Business Pro-Produkten die Arbeitsarten aus der Kapazitätsplanung in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für das jeweilige Produkt ausgeführt werden. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll.
⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-102

### Identifikation
**Produkt**
Produkt, dem Arbeitsarten zugeordnet sind.

### Arbeitsarten
Die Felder und Schaltflächen sind zum Dialog Produktarten beschrieben.
⇨ "Produktarten" auf Seite H-238

### Übersicht Zuordnungen
In der Übersicht werden die Produkte angezeigt, denen Arbeitsarten zugeordnet sind.

## Kombi-Produktart
**Kapazitätsplanung > Zuordnen > Kombi-Produktart**

*(Abb. H-157 Kombi-Produktarten)*

In diesem Dialog ordnen Sie den A+W Business Pro-Produkten, die Bestandteil einer Stückliste sind oder als Bearbeitung auf eine Produktgruppe wirken, die Arbeitsarten in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für die jeweilige Produktart ausgeführt werden. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll.
⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-102

### Identifikation
**Produkt**
Produkt, dem als Stücklistenelement von z. B. VSG, ESG usw. eine andere Arbeitsart zugeordnet ist, als diejenige, die standardmäßig für das Hauptprodukt gilt.

**Als Teil von, Wirkt auf**
Wenn die Float-Scheibe Teil einer Stückliste ist, kann sich die Produktionsreihenfolge oder die Arbeitsart ändern. Tragen Sie dann die entsprechende Produktart ein, z. B. ESG.

### Arbeitsarten
Die Felder und Schaltflächen in diesem Bereich sind zum Dialog Produktarten beschrieben.
⇨ "Produktarten" auf Seite H-238

### Übersicht Zuordnungen
In der Übersicht werden die Kombi-Produktarten angezeigt, denen Arbeitsarten zugeordnet sind.

## Sonderzuordnung 1
**Kapazitätsplanung > Zuordnen > Sonderzuordnung 1**

*(Abb. H-158 Sonderzuordnung 1 – Bearbeitungen)*

In diesem Dialog ordnen Sie einem A+W Business Pro-Bearbeitungsprodukt und der Folgebearbeitung die Arbeitsarten in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für dieses Produkt ausgeführt werden. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll.
⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-102

### Identifikation
**Bearbeitung**
Bearbeitung, der Arbeitsarten zugeordnet sind.

**Folgebearbeitung**
Folgebearbeitung, der Arbeitsarten zugeordnet sind.

### Arbeitsarten
Die Felder und Schaltflächen in diesem Bereich sind zum Dialog Produktarten beschrieben.
⇨ "Produktarten" auf Seite H-238

### Übersicht Zuordnungen
In der Übersicht werden die Bearbeitungen und Folgebearbeitung angezeigt, denen Arbeitsarten zugeordnet sind.

## Sonderzuordnung 2
**Kapazitätsplanung > Zuordnen > Sonderzuordnung 2**

*(Abb. H-159 Sonderzuordnung 2 – Bearbeitungen an Modellen)*

In diesem Dialog ordnen Sie einer Bearbeitung an Modellscheiben und der Folgebearbeitung die Arbeitsarten in der Reihenfolge zu, in der sie in der Produktion bzw. im Versand für dieses Produkt ausgeführt werden. Sie können zu jeder Arbeitsart pro Kante einen Zeitfaktor angeben, der bei der Planung berechnet werden soll.

> **Beispiel**
> An einer Scheibe mit Rundbogen soll die Kantenbearbeitung an geraden Kanten auf der Standard-Schleifmaschine ausgeführt werden, die Kantenbearbeitung für den Rundbogen muss auf einer anderen Maschine gemacht werden.

⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-102

### Identifikation
**Bearbeitung**
Bearbeitung, der Arbeitsarten zugeordnet sind.

**Modell**
Modell, dem Arbeitsarten zugeordnet sind.

**Bis Stück**
Stückzahl, wenn die Zuordnung der Arbeitsarten von der Anzahl der Scheiben abhängig ist, z. B. große Stückzahlen auf CNC-Maschinen. Geben Sie **9999** ein, wenn die Stückzahl nicht geprüft werden soll.

*(Abb. H-160 Kennzeichnung von Ecken und Kanten des gewählten Modells)*

### Arbeitsarten
In der Übersicht werden die zugeordneten Arbeitsarten angezeigt. Die Anzahl der Kanten richtet sich nach dem gewählten Modell.
Die Schaltflächen sind zum Dialog Produktarten beschrieben.
⇨ "Produktarten" auf Seite H-238

**#** Nummer der Reihenfolge.

**Arbeitsart** Nummer und Bezeichnung der Arbeitsart. Wenn Sie <k.A.> eintragen, wird die Bearbeitung ignoriert.

**Faktor** Die bei der Einlastung berechnete Zeit wird mit diesem Faktor multipliziert.
- 0 oder 1: Die Zeit wird nicht erhöht oder vermindert.
- >1: Ein Faktor von z. B. 1,5 entspricht einer Zeiterhöhung von 50%.

**1-n (Kante)** Angabe, für welche Kante der Faktor gilt. Die Anzahl der zur Verfügung stehenden Felder richtet sich nach der Anzahl der Kanten und Ecken des Modells. In der Modellskizze sind die Kanten mit roten Ziffern gekennzeichnet.
- [ ] Der Faktor wird für diese Kante nicht berechnet.
- [x] Der Faktor wird berechnet.

## Sonderzuordnung 3
**Kapazitätsplanung > Zuordnen > Sonderzuordnung 3**

*(Abb. H-161 Sonderzuordnung 3 – Kantenbearbeitung (Rechteckscheiben))*

In diesem Dialog ordnen Sie den Kantenbearbeitungen an Rechteckscheiben die Reihenfolge zu, in der sie ausgeführt werden.

> **Beispiel**
> Wenn bei einer Rechteckscheibe alle Kanten poliert werden sollen, werden standardmäßig gleichzeitig die Kanten 1 und 3 poliert und danach 2 und 4 (oder umgekehrt).
> Können auf einer Maschine 2 gegenüberliegende Kanten gleichzeitig poliert, gesäumt usw. werden, dann müssen Sie hierfür die Arbeitsart pro Kanten 1 + 3 und 2 + 4 zuordnen.

⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-102

### Identifikation
**Bearbeitung**
Bearbeitung, der Arbeitsarten zugeordnet sind.

**Kanten 1-4**
Angabe, für welche Kanten die Zuordnung gilt.
- [ ] Diese Kante wird nicht bearbeitet.
- [x] Diese Kante wird bearbeitet.

*(Abb. H-162 Kennzeichnung von Ecken und Kanten für die Berechnung des Faktors)*

### Arbeitsarten
In der Übersicht werden die zugeordneten Arbeitsarten angezeigt. Pro Kante kann ein Faktor festgelegt werden.
Die Schaltflächen sind zum Dialog Produktarten beschrieben.
⇨ "Produktarten" auf Seite H-238

**#** Nummer der Reihenfolge.

**Arbeitsart** Nummer und Bezeichnung der Arbeitsart. Wenn Sie <k.A.> eintragen, wird die Bearbeitung ignoriert.

**Faktor** Die bei der Einlastung berechnete Zeit wird mit diesem Faktor multipliziert.
- 0 oder 1: Die Zeit wird nicht erhöht oder vermindert.
- >1: Ein Faktor von z. B. 1,5 entspricht einer Zeiterhöhung von 50%.

**1-4 (Kanten)** Angabe, für welche Kanten der Faktor gilt. In der Modellskizze sind die Kanten mit roten Ziffern gekennzeichnet.
- [ ] Der Faktor wird für diese Kante nicht berechnet.
- [x] Der Faktor wird berechnet.

### Übersicht Zuordnungen
In der Übersicht werden die Bearbeitungen angezeigt, denen Arbeitsarten zugeordnet sind.

## Sonderzuordnung 4
**Kapazitätsplanung > Zuordnen > Sonderzuordnung 4**

*(Abb. H-163 Sonderzuordnung 4)*

In diesem Dialog ordnen Sie einem Produkt abhängig von einer Folgebearbeitung und einem Modell andere Arbeitsarten zu. Sie können zu jeder Arbeitsart einen Zeitfaktor angeben, der bei der Planung berechnet werden soll.
⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-102

### Identifikation
**Produkt**
Produkt, dem Arbeitsarten zugeordnet sind.

**Folgebearbeitung**
Folgebearbeitung, der Arbeitsarten zugeordnet sind.

**Modell**
Modell, für das die Zuordnung gilt.

*(Abb. H-164 Kennzeichnung von Ecken und Kanten für die Berechnung des Faktors)*

### Arbeitsarten
In der Übersicht werden die zugeordneten Arbeitsarten angezeigt. Die Anzahl der Felder für die Kanten ist von der Wahl des Modells abhängig.
Die Schaltflächen sind zum Dialog Produktarten beschrieben.
⇨ "Produktarten" auf Seite H-238

**#** Nummer der Reihenfolge.

**Arbeitsart** Nummer und Bezeichnung der Arbeitsart. Wenn Sie <k.A.> eintragen, wird die Bearbeitung ignoriert.

**Faktor** Die bei der Einlastung berechnete Zeit wird mit diesem Faktor multipliziert.
- 0 oder 1: Die Zeit wird nicht erhöht oder vermindert.
- >1: Ein Faktor von z. B. 1,5 entspricht einer Zeiterhöhung von 50%.

**1-n (Kanten)** Angabe, für welche Kanten der Faktor gilt. Die Anzahl der zur Verfügung stehenden Felder richtet sich nach der Anzahl der Kanten des Modells. In der Modellskizze sind die Kanten mit roten Ziffern gekennzeichnet.
- [ ] Der Faktor wird für diese Kante nicht berechnet.
- [x] Der Faktor wird berechnet.

### Übersicht Zuordnungen
In der Übersicht werden die Bearbeitungen angezeigt, denen Arbeitsarten zugeordnet sind.

## Kombi-Produktgruppe
**Kapazitätsplanung > Zuordnen > Kombi-Produktgruppe**

*(Abb. H-165 Kombi-Produktgruppen)*

In diesem Dialog ordnen Sie Produkten, die Bestandteil einer Stückliste sind oder als Bearbeitung auf eine Produktgruppe wirken, eine Arbeitsart und einen Zeitfaktor zu.
⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-102

### Identifikation
**Produkt**
Produkt, dem als Stücklistenelement von VSG oder ISO usw. eine andere Arbeitsart zugeordnet ist, als diejenige für das Hauptprodukt.

**Als Teil von/wirkt auf**
Wenn die Float-Scheibe Teil einer Stückliste ist, kann sich die Produktionsreihenfolge oder die Arbeitsart ändern. Tragen Sie dann die entsprechende Produktgruppe ein, z. B. VSG.

### Arbeitsarten
Die Felder und Schaltflächen in diesem Bereich sind zum Dialog Produktarten beschrieben.
⇨ "Produktarten" auf Seite H-238

## Lagerartikel
**Kapazitätsplanung > Zuordnen > Lagerartikel**

*(Abb. H-166 Lagerartikel)*

In diesem Dialog ordnen Sie Lagerartikeln die Arbeitsart Versand zu. Diese Zuordnung nutzen Sie, da die Lagerartikel (Beschaffungsart Lagerentnahme) nicht bearbeitet werden, z. B. bei Handgriffen, die nur verpackt und geliefert werden. Damit erreichen Sie, dass diese Produktgruppen z. B. in den Versand eingelastet und die Kosten und Zeiten kalkuliert werden.
⇨ Tutorial, "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-102

### Übersicht Zuordnungen
Liste der Produkte, denen Arbeitsarten zugeordnet sind.

### Identifikation
**Produktgruppe**
Lagerartikel, der Arbeitsart zugeordnet ist.

### Arbeitsarten
Die Felder und Schaltflächen in diesem Bereich sind zum Dialog Produktarten beschrieben.
⇨ "Produktarten" auf Seite H-238

### Übersicht Zuordnungen
In der Übersicht werden die Produktgruppen der Lagerartikel angezeigt, denen die Arbeitsart zugeordnet ist.

# Sperren
Sie müssen Sperren definieren, um z. B. zu vermeiden, dass bestimmte Arbeiten doppelt durchgeführt werden oder eine Maschine eingeplant wird, die eine Leistung für ein bestimmtes Produkt nicht erbringen kann.
Die Vorgehensweise für das Sperren von Produkten, Produktgruppen oder Warengruppen auf bestimmten Maschinen ist für alle Dialoge ähnlich.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Sperren nach WGR" auf Seite H-255
- "Sperren nach Produktgruppen" auf Seite H-256
- "Sperren nach Produkten" auf Seite H-258
- "Folge-Aggregate überspringen" auf Seite H-259
- "Kundenbezogene Sperren" auf Seite H-260
- "Fertigungsstraße definieren" auf Seite H-262
- "Arbeitsgänge überspringen" auf Seite H-263

## Sperren nach WGR
**Kapazitätsplanung > Sperren > Sperren nach WGR**

*(Abb. H-167 Sperren nach WGR)*

In diesem Dialog sperren Sie bestimmte Warengruppen für eine oder mehrere Maschinen.
⇨ Tutorial, "Sperren" auf Seite H-95

### Identifikation
**Warengruppe**
Warengruppe, für die die Maschine gesperrt ist.

### Aggregate
In der Übersicht werden die zugeordneten Aggregate angezeigt.
- **#** Nummer der Reihenfolge.
- **Aggregat** Nummer und Bezeichnung des Aggregats

### Schaltflächen
**[Neu], [Löschen]** Mit diesen Schaltflächen schalten Sie eine neue Zeile frei oder löschen einen markierten Eintrag.
**Pfeilschaltflächen** Mit diesen Schaltflächen können Sie die Reihenfolge der Arbeitsarten ändern.

### Übersicht Sperren
In der Übersicht werden die Warengruppen angezeigt, für die Sperren definiert wurden.

## Sperren nach Produktgruppen
**Kapazitätsplanung > Sperren > Sperren nach Produktgruppen**

*(Abb. H-168 Sperren nach Produktgruppen)*

In diesem Dialog sperren Sie eine Produktgruppe abhängig von der Arbeitsart für eine oder mehrere Maschinen.
⇨ Tutorial, "Sperren" auf Seite H-95

> **Beispiel**
> Für die Isolierglas-Produktion stehen 2 ISO-Linien zur Verfügung. Der Einbau eines Stahlrahmens in die ISO-Einheit geht jedoch nur auf der ISO-Linie Nr. 2.
> Darum muss die Produktgruppe Isolierglas bei der Arbeitsart Stahlrahmen montieren für die ISO-Linie Nr. 1 gesperrt werden.

### Identifikation
**Produktgruppe**
Produktgruppe, für die die Maschine gesperrt ist.

### Aggregate
Die Schaltflächen sind zum Dialog Sperren nach WGR beschrieben.
⇨ "Sperren nach WGR" auf Seite H-255

- **#** Nummer der Reihenfolge.
- **Arbeitsart** Nummer und Bezeichnung der Arbeitsart.
- **Aggregat** Nummer und Bezeichnung des Aggregats.
- **Total** In der Kombination von Produktgruppe und Arbeitsart kann die Maschine ganz oder teilweise gesperrt werden.
  - [ ] Diese Maschine ist nur für diese Produktgruppe (Hauptprodukt) und diese Arbeitsart gesperrt.
  - [x] Ist die Produktgruppe inklusive der Arbeitsart Bestandteil einer Stückliste, dann wird die Maschine komplett gesperrt, d. h. auch für alle anderen Arbeitsarten, die das Hauptprodukt und dessen Stücklisten-Komponenten betreffen.

### Übersicht Sperren
In der Übersicht werden die Produktgruppen angezeigt, für die Sperren definiert wurden.

## Sperren nach Produkten
**Kapazitätsplanung > Sperren > Sperren nach Produkten**

*(Abb. H-169 Sperren nach Produkten)*

In diesem Dialog sperren Sie ein Produkt abhängig von der Arbeitsart für eine oder mehrere Maschinen.
⇨ Tutorial, "Sperren" auf Seite H-95

### Identifikation
**Produkt**
Produkt, für das die Maschine gesperrt ist.

### Aggregate
Die Felder und Schaltflächen sind zum Dialog Sperren nach Produktgruppen beschrieben.
⇨ "Sperren nach Produktgruppen" auf Seite H-256

### Übersicht Sperren
In der Übersicht werden die Produkte angezeigt, für die Sperren definiert wurden.

## Folge-Aggregate überspringen
**Kapazitätsplanung > Sperren > Folge-Aggregate überspringen**

*(Abb. H-170 Folge-Aggregate überspringen)*

In diesem Dialog sperren Sie eine Maschine abhängig von der Folge-Maschine.

> **Beispiel**
> Wenn die Bohrstraße das Waschen automatisch beinhaltet, dann können Sie das nachfolgende Aggregat Waschmaschine sperren oder überspringen, um doppeltes Waschen zu verhindern.

⇨ Tutorial, "Sperren" auf Seite H-95

### Identifikation
**Aggregat**
Aggregat, für das die Folge-Maschine gesperrt ist.

### Aggregat
Die Felder und Schaltflächen sind zum Dialog Sperren nach Produktgruppen beschrieben.
⇨ "Sperren nach Produktgruppen" auf Seite H-256

## Kundenbezogene Sperren
**Kapazitätsplanung > Sperren > Kundenbezogene Sperren**

*(Abb. H-171 Kundenbezogene Sperren)*

In diesem Dialog sperren Sie Maschinen abhängig von der Kundennummer, vom Produkt oder von der Bearbeitung.

> **Beispiel**
> Besteht ein Kunde z. B. darauf, dass für seine Aufträge eine bestimmte Bohrmaschine nicht benutzt wird, muss diese Bohrmaschine für ihn gesperrt werden.

⇨ Tutorial, "Sperren" auf Seite H-95

### Menü Funktionen
Über dieses Menü können Sie die Sperre eines Kunden auf die gesamte Kundengruppe ausdehnen oder die Sperre aufheben. Folgende Einträge werden angezeigt:
- **Sperre setzen:** Die Sperre wird auf alle Kunden der Kundengruppe ausgedehnt, zu der der angezeigte Kunde gehört. Alle betroffenen Kunden werden in der Übersicht aufgeführt.
- **Sperre aufheben:** Die Sperre wird für alle Kunden der Kundengruppe gelöscht. Die Kunden werden alle aus der Übersicht entfernt.

### Identifikation
**Kunde**
Kunde, für den die Sperre eingerichtet ist.

**Produkt/Bearbeitung**
Produkt oder Bearbeitung, für die die Maschine gesperrt ist.

**Gesperrtes Aggregat**
Maschine, die gesperrt ist.

### Tabelle
In der Übersicht werden alle Kunden angezeigt, für die Sperren definiert sind.
- **Kunden-Nr., Kunde:** Nummer und Name des Kunden.
- **Kundengruppe:** Kundengruppe, zu der der Kunde gehört.
- **Ort:** Hauptsitz des Kunden.
- **Produkt-Nr., Produkt:** Nummer und Bezeichnung des Produkts, für das die Sperre definiert ist.
- **Gesperrtes Aggregat:** Aggregat, das für die Kombination von Kunde und Produkt gesperrt ist.

## Fertigungsstraße definieren
**Kapazitätsplanung > Sperren > Fertigungsstraße definieren**

*(Abb. H-172 Fertigungsstraßen definieren)*

In diesem Dialog sperren Sie eine Maschine abhängig von der vorherigen Maschine.
⇨ Tutorial, "Fertigungsstraße definieren" auf Seite H-98
Die Schaltflächen sind zum Dialog Sperren nach WGR beschrieben.
⇨ "Sperren nach WGR" auf Seite H-255

### Identifikation
**Aggregat**
Aggregat, für das die Folge-Maschine gesperrt ist. Diese Folge-Maschine wird im Bereich Aggregate angegeben.

### Aggregate
In der Übersicht werden die Arbeitsarten und zugeordneten Aggregate angezeigt.
- **#** Nummer der Reihenfolge.
- **Arbeitsart** Nummer und Bezeichnung der Arbeitsart.
- **Aggregat** Nummer und Bezeichnung des Aggregats.
- **Total** Die Maschine kann ganz oder teilweise gesperrt werden.
  - [ ] Die Maschine kann manuell ausgewählt werden.
  - [x] Diese Maschine ist für diese Arbeitsart vollständig gesperrt.

### Übersicht Sperren
In der Übersicht werden die Aggregate mit Sperren angezeigt.

## Arbeitsgänge überspringen
**Kapazitätsplanung > Sperren > Arbeitsgänge überspringen**

*(Abb. H-173 Arbeitsgänge überspringen)*

In diesem Dialog sperren Sie Folgebearbeitungen abhängig von der Maschine.

> **Beispiel**
> Wenn die Bohrstraße das Waschen beinhaltet, dann können Sie den Folge-Arbeitsgang Glas waschen sperren, um doppeltes Waschen zu verhindern.

⇨ Tutorial, "Sperren" auf Seite H-95

### Identifikation
**Aggregat**
Aggregat, an dem die Arbeitsart gesperrt ist.

### Arbeitsarten
In der Übersicht werden die zugeordneten Arbeitsarten angezeigt.
Die Schaltflächen sind zum Dialog Sperren nach WGR beschrieben.
⇨ "Sperren nach WGR" auf Seite H-255

- **#** Nummer der Reihenfolge.
- **Arbeitsart** Nummer und Bezeichnung der Arbeitsart, für das Aggregat gesperrt ist.

### Übersicht Sperren
In der Übersicht werden die Aggregate angezeigt, für die Sperren definiert wurden.

# Übersichten
Mit verschiedenen Tabellen und Grafiken erhalten Sie einen Überblick über die Auslastung an einem bestimmten Datum oder in einen Zeitraum.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Statistik" auf Seite H-266
- "Grafik-Bereiche" auf Seite H-267
- "AV-Bereichsstatistik" auf Seite H-268
- "AV-Bereichsstatistik kurz" auf Seite H-272
- "Konten" auf Seite H-272
- "Kostenstellen-Definitionen" auf Seite H-274

## Statistik
**Kapazitätsplanung > Übersicht > Statistik**

*(Abb. H-174 Statistik)*

In dieser Übersicht können Sie sich alle Aufträgen anzeigen lassen, die innerhalb eines Zeitraumes von einem Aggregat fertig gemeldet wurden.
Die Bildschirm-Anzeige gilt nur für die ausgewählte Maschine. Die Druck-Ausgabe zeigt jedoch alle Maschinen und die Zeitkosten an.

### Selektion
**Von, bis**
Auswertungszeitraum. Wenn Sie in beiden Feldern dasselbe Datum eintragen, wird eine Tagesauswertung erstellt.

**Aggregat**
Maschine, deren Auslastung angezeigt werden soll.

### Belegzeiten
In der Übersicht werden pro Aggregat die Werte für alle fertig gemeldeten Stückzahlen aufgelistet.
- **Arbeitsart**
- **Stück** Fertig gemeldete Stückzahl.
- **Fläche** Fertig gemeldeten Quadratmeter.
- **Umfang** Kantenlänge insgesamt.
- **Zeit** Insgesamt benötigte Zeit.
- **Aggregat** Aggregat, das die Werte gemeldet hat.
- **Summe Zeit** Summe der Zeiten für die ausgewählte Maschine.

## Grafik-Bereiche
**Kapazitätsplanung > Übersicht > Grafik-Bereiche > Legende**

*(Abb. H-175 Grafik-Bereiche - Wochenübersicht)*

In dieser Übersicht lassen Sie sich eine grafische Übersicht über die Auslastung entweder nach Aggregattypen oder nach Produktionsbereichen anzeigen.
Sie können die Anzeige über das Menü Werk auf ein bestimmtes Werk oder einen Mandanten einschränken.
Die Grafik kann aus verschiedenen Dialogen heraus geöffnet werden. Die Anzeige der Daten ist dann entsprechend des Ausgangsdialogs gefiltert, z. B. pro Tagesschicht.

### Zeitraum
**Datum**
Datum, für das die Grafik erstellt werden soll.

**Woche**
Sie können nur den eingetragenen Tag oder die gesamte Woche auswerten.
- [ ] Nur der ausgewählte Tag wird ausgewertet.
- [x] Die Auswertung bezieht die ganze Woche ein (Montag bis Sonntag).

**Aggregattyp, Produktionsbereich**
Mit der Wahl der Option legen Sie fest, worauf sich die Auswertung beziehen soll.

**[Legende]**
Blendet die Legende mit der Bedeutung der Farben in der Grafik ein und aus. Die Einstellung gilt für alle Grafiken.

### Grafik
**Rote Linien**
Die rote Linie zeigt das Ende einer Schicht an.

**Linke Spalte**
Die linke Spalte verändert sich je nach Tages- oder Wochenansicht.
- Tagesansicht: Schichten
- Wochenansicht: Tagesdatum.

## AV-Bereichsstatistik
**Kapazitätsplanung > Übersicht > AV-Bereichsstatistik**

Die AV-Bereichsstatistik ist eine Statistik auf Produktebene für alle fertig gemeldeten Arbeitsarten.

In diesem Dialog finden Sie folgende Register:
- "AV-Bereichsstatistik - Auswahl" auf Seite H-269
- "AV-Bereichsstatistik - Tabelle" auf Seite H-271

## AV-Bereichsstatistik – Auswahl
**Kapazitätsplanung > Übersicht > AV-Bereichsstatistik > Register Auswahl**

*(Abb. H-176 AV-Bereichsstatistik – Auswahl)*

In diesem Register wählen Sie die Kriterien aus, nach denen die Übersicht über Fertigmeldungen erstellt werden soll. Wenn Sie alle Angaben eines Zeitraums anzeigen lassen wollen, dürfen Sie die Suche nicht durch Restriktionen einschränken.

### Auswertungszeitraum
**Von, bis**
Auswertungszeitraum. Wenn Sie in beiden Feldern dasselbe Datum eintragen, wird eine Tagesauswertung erstellt.

### Restriktionen
In diesem Bereich können Sie Auswahl einschränken.

> **Eintrag <k. A.>**
> Wenn eines der Felder nicht berücksichtigt werden soll, müssen Sie den Eintrag vollständig löschen. Der Eintrag <k. A.> bedeutet, dass z. B. die Produktart <k. A.> ausgeschlossen werden soll.
> Wenn Sie Informationen zu allen Produktarten, -gruppen und AV-, Produktionsbereichen anzeigen lassen wollen, müssen Sie alle vier Felder leer lassen.

**Produktart**
Die gewählte Produktart soll nicht angezeigt werden.

**Produktgruppe**
Die gewählte Produktgruppe soll nicht angezeigt werden.

**AV-Bereich**
Der gewählte AV-Bereich soll nicht angezeigt werden.

**Produktionsbereich**
Der gewählte Produktionsbereich soll nicht angezeigt werden.

### Ausgabe / Sortierung
Im linken Feld werden die Ausgabemöglichkeiten angezeigt. Im rechten Feld wird angezeigt, nach welchem Kriterium die Auswertung sortiert werden soll. Die Einstellung wirkt sich auf die Darstellung des Ergebnisses im Register Tabelle aus.
Einen markierten Eintrag verschieben Sie mit den Pfeilschaltflächen in das rechte Feld oder zurück in das linke Feld.

### Übersicht nach
Mit der Wahl der Option legen Sie fest, welche Daten angezeigt werden sollen:
- **Produktart:** Die Auswertung soll sich auf die Produktart beziehen.
- **Produktgruppe:** Die Auswertung soll sich auf die Produktgruppe beziehen.
- **Produkt:** Die Auswertung soll sich auf die Produkte beziehen.

## AV-Bereichsstatistik – Tabelle
**Kapazitätsplanung > Übersicht > AV-Bereichsstatistik > Register Tabelle**

*(Abb. H-177 AV-Bereichsstatistik - Tabelle)*

In diesem Register wird das Ergebnis der Auswertung angezeigt. Sie können mit den entsprechenden Auswahlkriterien z. B. ermitteln, in welchen AV-Bereichen das Glas verbraucht wird.

### Übersicht
Die zweite Spalte wird nur dann gefüllt, wenn nach Produktionsbereich und AV-Bereich sortiert wird, egal in welcher Reihenfolge.
- **Produktionsbereich, AV-Bereich:** Anzeige je nach Wahl des Sortierkriteriums.
- **Produkt, Produktgruppe, Produktart:** Anzeige je nach Wahl des Sortierkriteriums.
- **Vorgang:** In diesem Feld werden die Arbeitsarten angezeigt.
- **Stück:** Produzierte Stückzahlen.
- **Qm:** Produzierte Fläche.
- **Lfm:** Produzierte Laufmeter (Kanten).
- **Kosten ZW:** Ermittelte Zeitkosten.
- **Materialkosten:** Ermittelte Materialkosten.

## AV-Bereichsstatistik kurz
**Kapazitätsplanung > Übersicht > AV-Bereichsstatistik kurz**

In diesem Dialog lassen Sie sich eine verkürzte Liste der Auswertung nach AV-Bereichen anzeigen, die automatisch nach den beiden Kriterien AV-Bereich und Produktionsbereiche sortiert ist.
Die Felder sind zum Dialog AV-Bereichsstatistik beschrieben.
⇨"AV-Bereichsstatistik" auf Seite H-268

## Konten
**Kapazitätsplanung > Übersicht > Konten**

*(Abb. H-178 Konten - Auswahl)*

In diesem Dialog lassen Sie sich anzeigen, auf welche Kostenstellen oder AV-Bereiche bestimmte Produkte, Produktgruppen oder Produktarten gebucht wurden. Die Daten werden aus den Aufträgen ausgelesen. Archivierte Aufträge werden nicht berücksichtigt.

### Menü Kostenstellen
Über dieses Menü können Sie den Dialog Kostenstellen-Definition öffnen, um die Kostenstellen anzulegen oder zu bearbeiten.
⇨ "Kostenstellen-Definitionen" auf Seite H-274

### Auswertungszeitraum Liefertermin
**Von, bis**
Auswertungszeitraum. Wenn Sie in beiden Feldern dasselbe Datum eintragen, wird eine Tagesauswertung erstellt.

### Sortiert nach
Mit der Wahl der Option legen Sie fest, wie die Anzeige sortiert werden soll:
- **Kostenstellen:** Das sind die Kostenstellen, die Sie für die Kapazitätsplanung erstellt haben.
  ⇨ "Kostenstellen-Definitionen" auf Seite H-274
- **AV-Bereiche:** AV-Bereiche aus den A+W Business Pro-Stammdaten.

> **Kostenstellen definieren**
> Neue Kostenstellen definieren Sie auf die gleiche Weise wie die Vorschauspalten im Modul Fertigung.
> ⇨ Tutorial, "Prinzip der Auswertungsspalten" auf Seite H-162

### Übersicht nach
Mit der Wahl der Option legen Sie fest, ob die Auswertung nach Produktart, Produktgruppe oder nach den einzelnen Produkten angezeigt wird.

### Übersicht
In der Übersicht werden folgende Daten angezeigt:
- **Kostenstelle:** Bezeichnung der Kostenstelle. Die Bezeichnungen werden im Dialog Kostenstellen Definition festgelegt.
  ⇨ "Kostenstellen-Definitionen" auf Seite H-274
- **AV-Bereich:** AV-Bereich, dem die Kostenstelle zugeordnet ist.
- **Produktart, Produktgruppe, Produkt:** Die Anzeige der entsprechenden Daten richtet sich nach der Option, die im Register Auswahl gewählt wurde.
- **Stück:** Anzahl der gefertigten Scheiben.
- **Fläche:** Gesamtfläche der gefertigten Scheiben.
- **Materialkosten:** Materialkosten der gefertigten Scheiben.

## Kostenstellen-Definitionen
**Kapazitätsplanung > Übersicht > Konten > Menü Kostenstellen**

*(Abb. H-179 Kostenstellen-Definition)*

In diesem Dialog legen Sie die Kostenstellen für die Auswertung von Produktionsdaten und -kosten an.
Bevor Sie Kostenstellen anlegen, sollten Sie sich überlegen, in welcher Reihenfolge die Kostenstellen abgefragt werden sollen.

> **Beispiel ESG**
> Sie fragen erst ab, ob es sich um ein ESG mit Bearbeitung handelt (Kostenstelle Nr. 7 mit Prio 19).
> Wenn dies nicht der Fall ist, kommt die Folge-Abfrage.
> Das ESG, das nicht bearbeitet ist, fließt in die Kostenstelle ESG (Kostenstelle Nr. 6 mit Prio 20).

> **Kostenstellen definieren**
> Neue Kostenstellen definieren Sie auf die gleiche Weise wie die Vorschauspalten im Modul Fertigung.
> ⇨ Tutorial, "Prinzip der Auswertungsspalten" auf Seite H-162

**Nr.** Nummer der Kostenstelle.

**Bezeichnung** Namen der Kostenstelle.

**HPA** Haupt-Produktart. In diesem Feld tragen Sie ein, für welche Produktart die Auswertung gemacht werden soll.

**Nr 1, Nr 2** Diese Einträge beziehen sich auf die Felder Typ 1 und Typ 2. Hier tragen Sie die entsprechende Nummer der Produktart oder Produktgruppe von Typ 1 oder Typ 2 ein oder 0 für keine Vorgabe.

**Typ 1, Typ 2**
Produktart bzw. Produktgruppe, die Stücklistenelement der Hauptproduktart ist.
- 0 = Keine Vorgabe
- 1 = Produktart
- 2 = Produktgruppe

Sie suchen z. B. nach der Produktart (Typ 1 = 1) Bearbeitung (Nr 1 = 20), die Bestandteil von ESG (HPA = 2) ist.

**Priorität**
Nummer der Reihenfolge, in der die Abfrage der Kostenstellen erfolgen soll.

**Ausschluss**
Sie können ein Produkt von der Regel ausschließen. Die Produktnummer muss in Klammern stehen.

> **Beispiel**
> Alle ESG-Scheiben werden gesäumt. Deshalb möchten Sie nicht, dass gesäumte ESG-Scheiben in die Kostenstelle ESG mit Bearbeitung einfließen.
> Sie schließen dies aus, indem Sie die entsprechende Produktnummer (in Klammern) eintragen.

### Schnittstelle Lisec
Dieser Dialog ist nur freigeschaltet, wenn Sie mit einer entsprechenden Schnittstelle arbeiten.

# Kapazitätsplanung
**Fertigung > Kapazitätsplanung**

Zur Planung der Kapazitäten stehen im Modul Fertigung verschiedene Dialoge zur Verfügung. Damit können Sie in diesem Modul neben der Übergabe von Daten an die Produktion auch den Produktionsfortschritt mit Hilfe der Rückmeldungen prüfen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Einlastung" auf Seite H-277
- "Produktionsmeldungen" auf Seite H-301
- "Leitstand" auf Seite H-335

## Einlastung
Die Zeit- und Materialkosten können nur für Aufträge berechnet werden, die in die Kapazitätsplanung eingelastet werden. Die Aufträge können manuell oder automatisch in definierten Intervallen eingelastet werden.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Nummernverwalter" auf Seite H-277
- "Einlasten NV" auf Seite H-278
- "Kriterien ändern (Modus Terminsuche)" auf Seite H-281
- "Lieferdatum" auf Seite H-283
- "Einlasten Auftrag" auf Seite H-284
- "Einlasten Ergebnis" auf Seite H-289
- "Aggregat-Auswahl bei Engpass" auf Seite H-291
- "Auftragsnummern" auf Seite H-293
- "Positions-Split" auf Seite H-294
- "Positions-Zeiten" auf Seite H-296
- "Aggregate Ausfall" auf Seite H-297
- "Restmengenübertragung" auf Seite H-300
- "Einstellungen Schichten" auf Seite H-187

## Nummernverwalter
**Fertigung > Kapazitätsplanung > Einlastung > Nummernverwalter**

Sie haben die Möglichkeit, mehrere Aufträge manuell gleichzeitig in die Kapazitätsplanung einzulasten. Hierfür werden diese in einem Nummernverwalter gesammelt.

Im Dialog **Einlasten NV** können Sie den Nummernverwalter auswählen und die Aufträge einlasten. Angezeigt werden alle Nummernverwalter, die für Dokumente erstellt wurden.
⇨ "Einlasten NV" auf Seite H-278

Im Dialog Nummernverwalter können Sie sich zu dem Auftrag, den Sie in der Übersicht markiert haben, den Dialog **Übersicht Statusrückmeldungen** öffnen. Der Dialog ist ausführlich im Part Verkauf beschrieben.
⇨ Verkauf, "Übersicht Statusrückmeldung" auf Seite C-507

Der Dialog Nummernverwalter und die zugehörigen Menüs sind für alle Module gleich. Er ist ausführlich im Part Verkauf beschrieben.
⇨ Verkauf, "Nummernverwalter" auf Seite C-551

## Einlasten NV
**Fertigung > Kapazitätsplanung > Einlastung > Einlasten NV**

Über einen Nummernverwalter lasten Sie alle Aufträge manuell ein, die dem Mindeststatus entsprechen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite H-278
- "Menü Optionen" auf Seite H-278
- "Einlasten NV (Dialog)" auf Seite H-279

### Menü Funktionen
**Fertigung > Kapazitätsplanung > Einlastung > Einlasten NV > Menü Funktionen**

Über dieses Menü können Sie sich die Historie zu dem Auftrag anzeigen lassen, den Sie in der Übersicht markiert haben. Die Historie ist ausführlich im Part Verkauf beschrieben.
⇨ Verkauf, "Historie" auf Seite C-486

### Menü Optionen
**Fertigung > Kapazitätsplanung > Einlastung > Einlasten NV > Menü Optionen**

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen und andere Dialoge öffnen, ohne den aktuellen Dialog zu verlassen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen. Folgende Einträge werden angezeigt:

- **Modus Terminsuche:** Öffnet den gleichnamigen Dialog, in dem Sie die Kriterien für die Terminsuche festlegen können.
  ⇨ "Kriterien ändern (Modus Terminsuche)" auf Seite H-281
- **Pos. Control:** Beim Einlasten wird der Anteil des Auftrags an der Tageskapazität geprüft. Der Prozentwert ist im Dialog Arbeitsarten hinterlegt.
  ⇨ "% Limit" auf Seite H-194
- **Alter Verweiltagemodus:** Diese Einstellung ist nur erforderlich, wenn Sie den alten Modus für Verweiltage (= Übergangsmatrix) beibehalten wollen.
- **Check auf Rüstzeit:** Wenn die Rüstzeit zu mehreren Arbeitsarten eingerichtet ist, die für eine Auftragsposition ausgeführt werden, dann soll diese Zeit nur einmal pro Position berechnet werden.

### Einlasten NV (Dialog)
**Fertigung > Kapazitätsplanung > Einlastung > Einlasten NV**

*(Abb. H-180 Einlasten nach Nummernverwalter)*

In diesem Dialog übergeben Sie die Aufträge aus einem Nummernverwalter an die Kapazitätsplanung. Die Übergabe starten Sie mit Menü **Start > Ausführen**.
⇨ Tutorial, "Einlastung der Aufträge" auf Seite H-113

#### Identifikation
- **Mandant**: Auswahl des Mandanten, dessen Aufträge eingelastet werden sollen.
- **Bereich**: Auswahl des AV-Bereichs, dessen Aufträge eingelastet werden sollen.
  ⇨ Stammdaten, "AV-Bereiche" auf Seite B-998
- **Mitarbeiter**: Angemeldeter Mitarbeiter.
- **Nummernverwalter**: Wenn Sie einen Nummernverwalter ausgewählt haben, werden alle Aufträge übergeben, die in diesem Nummernverwalter stehen und den Mindeststatus erreicht haben.

#### Auftragspriorität
Das Feld ist nur freigeschaltet, wenn Sie in den Firmendaten > Register Kapa-Planung > Feld Einlastpriorität die Einstellung **Geänderte Priorität in Auftrag übernehmen** ausgewählt haben.

Die Aufträge werden in der Regel nach der Priorität **Normal** eingelastet. Nur wenn es sich bei den Aufträgen z. B. um Eilaufträge handelt, die mit schnelleren Durchlaufzeiten berechnet werden sollen, müssen Sie die entsprechende Priorität auswählen.
- **Abruf:** Der Auftrag wird erst gefertigt, wenn der Kunde die Positionen abruft.
- **Eilt:** Der Auftrag muss mit oberster Priorität eingelastet werden.
- **Normal:** Der Auftrag wird den Standard-Einstellungen entsprechend eingelastet.
- **Zugabe:** Diese Priorität bedeutet, dass der Auftrag so gefertigt werden soll, dass er Reste und Restplatten verbraucht, die beim Zuschnitt anderer Aufträge entstehen.

> **Auftragspriorität berücksichtigen**
> Wenn außer der Auftragspriorität Normal auch z. B. die Priorität Eilt berücksichtigt werden soll, dann müssen dafür eigene Übergangszeiten eingerichtet sein. Wenn diese nicht eingerichtet sind, wird mit der Priorität Normal eingelastet.
> ⇨ "Übergangszeiten" auf Seite H-197
> ⇨ "Übergangsmatrix” auf Seite H-216

#### Verhalten bei Lieferterminproblemen
Mit der Wahl der Option legen Sie fest, wie beim Einlasten auf Probleme reagiert werden soll:
- **Keine Automatik:** Der Auftrag soll nicht automatisch zum nächsten möglichen Produktionstermin eingelastet werden. Bei dieser Option wird der Dialog **Lieferdatum** geöffnet, in dem Sie die Vorgaben zum Einlasten einstellen.
  ⇨ "Lieferdatum" auf Seite H-283
- **Nächster Liefertermin:** Der Auftrag soll zum nächsten möglichen Liefertermin eingelastet werden. Der neue Liefertermin wird in den Auftrag zurückgeschrieben.
- **Zum Liefertermin einlasten:** Der Auftrag soll zum ursprünglichen Liefertermin eingelastet werden, auch wenn damit die Maschinenkapazitäten überlastet werden. Diese Option können Sie wählen, wenn Sie sicher sind, dass Sie andere eingelastete Aufträge verschieben können.
- **Unendliche Kapazitäten:** Der Auftrag wird unabhängig von den tatsächlichen Kapazitäten eingelassen.

## Kriterien ändern (Modus Terminsuche)
**Fertigung > Kapazitätsplanung > Einlastung > Einlasten NV > Menü Optionen > Modus Terminsuche**
**Fertigung > Kapazitätsplanung > Einlastung > Einlasten Auftrag > Menü Funktionen > Terminsuche**

*(Abb. H-181 Einstellungen für die Terminsuche)*

In diesem Dialog legen Sie die Kriterien für die manuelle Einlastung oder bei Kapazitätsproblemen fest. Die Einstellungen gelten jeweils nur für die aktuelle Einlastung.

### Bestimmung des Fertigungstermins
Mit diesen Einstellungen übersteuern Sie die Standard-Einstellungen aus den Firmendaten. Die übersteuerten Einstellungen gelten nur für die aktuelle Sitzung:
- **Automatisch Normalkapazität:** Die Aufträge werden entsprechend der zur Verfügung stehenden Schichtzeiten eingelastet. Die Überbuchung ist nicht möglich. Dies ist die Standard-Einstellung (geschlossene Kapazitäten).
- **Automatisch "volle Tage":** Bei dieser Einstellung werden die Angaben im Kalender für die Anzahl Schichten und Stunden ignoriert. Die Einlastung geht dann von einem Arbeitstag mit 24 Stunden aus (offene Kapazitäten). Dies gilt jedoch nur für reguläre Arbeitstage, nicht für Feiertage.
- **Nur Aggregatwechsel:** Bei ausgelasteten Kapazitäten soll automatisch nur nach einem anderen Aggregat gesucht werden. Wenn das ebenfalls ausgelastet ist, wird die Einlastung unterbrochen und Sie müssen manuell eingreifen.
- **Einlasten ohne Kontrolle:** Diese Einstellung entspricht der offenen Schicht. Das heißt z. B., dass trotz der Schichtzeit von 8 Std. auch 16 Std. eingelastet werden können. Dabei wird keine Meldung ausgegeben, wenn ein Tag voll ausgelastet ist. Diese Option sollte nur in Ausnahmefällen genutzt werden.

### Modus zum Abgleich der Aggregate
Wenn Sie mit mehreren Maschinen arbeiten, die dieselben Arbeitsarten ausführen können, kann die Planung diese Maschinen auf unterschiedliche Weise berücksichtigen:
- **Automatisch:** Das Programm sucht automatisch nach der kosten- und zeitgünstigsten Maschine und lastet die Aufträge dort ein. Dies ist die Standard-Einstellung.
- **Semi-automatisch:** Das Programm bietet die alternativen Maschinen zur Auswahl an. Wenn der Liefertermin nicht eingehalten werden kann, müssen Sie eingreifen.
- **Manuell:** Mit dieser Option müssen Sie bei jedem möglichen Wechsel (Maschine, Schicht usw.) manuell eingreifen. Alternative Maschinen können nur bei der manuellen Ein- oder Umlastung ausgewählt werden.

### Optionen
**Sperrstunde**
Bei der manuellen Einlastung können Sie angeben, bis zu welcher Uhrzeit Aufträge eingelastet werden dürfen. Die Einstellung wird bis zur nächsten Änderung beibehalten.

> **Beispiel**
> Am Freitag erhalten Sie um 12 Uhr einen neuen Auftrag. Bei der manuellen Einlastung tragen Sie 14 Uhr ein, obwohl die Schicht bis 16 Uhr geht. Damit wird der Auftrag nicht eingelastet, wenn er an diesem Tag nicht mehr gefertigt werden kann. Sie verhindern damit, dass Restmengen von noch nicht begonnenen Aufträgen entstehen, die am folgenden Tag dann umgelastet werden müssen.
> Wenn der Auftrag wegen der Sperrstunde nicht mehr eingelastet werden kann, wird im Dialog Lieferdatum eine entsprechende Meldung angezeigt. Sie müssen dann das Lieferdatum ändern.

Die Sperrzeiten können übergreifend im Dialog **Einstellung Schichten** festgelegt werden.
⇨ "Einstellungen Schichten" auf Seite H-187

**Verkürzte Kontrolle**
Normalerweise prüft die Einlastung für jede Position, an welchem Tag noch Kapazitäten zur Verfügung stehen, um die Position dort einzulasten. In einem Auftrag können jedoch Positionen mit gleichem Stücklistenaufbau enthalten sein, die sich nur durch die Maße unterscheiden.
- [ ] Bei jeder Position wird der gesamte Stücklistenaufbau geprüft.
- [x] Bei gleichem Stücklistenaufbau wird von der Einlastung der vorigen Position ausgegangen, ohne die Stückliste neu zu prüfen. Dies ist die Standard-Einstellung.
Das Programm merkt sich den Starttermin der Produktion der ersten Position, z. B. für die Schleifmaschine. Die Folgeposition setzt genau auf diesem Termin auf, um die Kapazität für diese Maschine zu prüfen und geht, falls die Maschine für diesen Tag ausgelastet ist, auf die vorherige Schicht bzw. den vorherigen Tag. Die nächste Position setzt wiederum auf diesem neuen Termin für die Prüfung der Kapazität auf usw.

**Aufträge nicht splitten**
Wenn ein Auftrag nicht an einem Tag gefertigt werden kann, sollte der Auftrag gesplittet werden.
- [ ] Der Auftrag kann gesplittet werden, so dass sich die Produktion über mehrere Tage verteilt.
- [x] Der Auftrag soll nicht gesplittet werden. Die Terminsuche muss so lange fortgesetzt werden, bis die für den gesamten Auftrag benötigten Kapazitäten frei sind.

## Lieferdatum
**Fertigung > Kapazitätsplanung > Einlastung > Einlasten nach NV, Einlasten nach Auftrag > Einlasten**

*(Abb. H-182 Lieferdatum beim Einlasten)*

In diesem Dialog legen Sie manuell fest, wann oder wie der Auftrag eingelastet werden soll.
Der Dialog wird angezeigt, wenn der Liefertermin aus dem Auftrag nicht eingehalten werden kann, weil die Kapazitätsprüfung keinen zeitgerechten, freien Termin ermitteln konnte. Diese manuellen Einstellungen werden in der Historie dokumentiert.

Folgende Optionen stehen zur Wahl:
- **Automatisch festlegen:** Mit dieser Option wird der nächstmögliche Liefertermin ermittelt und in den Auftrag zurückgeschrieben. Die Tourentage des Kunden werden dabei berücksichtigt. Bei dieser Option wird eine Vorwärtsterminierung durchgeführt.
- **Liefertermin wählen:** Mit dieser Option wählen Sie einen anderen Liefertermin aus. Danach wird erneut geprüft, ob zu dem neuen Liefertermin genügend Kapazitäten verfügbar sind. Dieser Vorgang wird so lange fortgesetzt, bis der Auftrag eingelassen werden kann. Wenn die Einlastung erfolgreich ist, wird das neue Datum in den Auftrag zurückgeschrieben.
- **Zum Liefertermin einlasten:** Mit dieser Option werden die standardmäßigen Vorlaufzeiten ignoriert und das Programm versucht den Auftrag zum Liefertermin einzulasten. Die Suche nach freien Kapazitäten geht jeweils einen Tag zurück bis zum aktuellen Datum. Wenn bis dahin keine Kapazitäten gefunden wurden, wird der Auftrag an diesem Tag eingelastet, unabhängig davon, ob Kapazitäten frei sind oder nicht.
- **Unendliche Kapazität:** Mit dieser Option wird den Auftrag zum Liefertermin eingelastet, unabhängig davon, ob Kapazitäten frei sind oder nicht.
- **Einzel-Vorgabe:** Mit dieser Option kann zunächst manuell der Liefertermin bestimmt werden, danach stoppt das Programm bei jeder Arbeitsart, die im Auftrag enthalten ist. Sie müssen die entsprechenden Maschinen, den Produktionstag und die Schicht manuell festlegen.

**[Ende]** Mit dieser Schaltfläche brechen Sie das Einlasten des aktuellen Auftrages ab. Nachdem Sie eine Sicherheitsabfrage mit [Ja] beantwortet haben, fährt das Programm mit dem nächsten Auftrag des Nummernverwalters fort. Der nicht eingelastete Auftrag muss danach separat eingelastet werden.

## Einlasten Auftrag
**Fertigung > Kapazitätsplanung > Einlastung > Einlasten Auftrag**

In diesem Dialog lasten Sie einen einzelnen Auftrag oder auch eine einzelne Position eines Auftrages manuell in die Kapazitätsplanung ein.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite H-285
- "Menü Optionen" auf Seite H-286
- "Gruppe Einstellungen" auf Seite H-285
- "Einlasten Auftrag (Dialog)" auf Seite H-287

### Menü Funktionen
**Fertigung > Kapazitätsplanung > Einlastung > Einlasten Auftrag**

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Dialog Einlasten Auftrag zu schließen.

#### Gruppe Aktueller Auftrag
- **Einlastungsergebnis:** Öffnet den Dialog Einlastungsergebnis, in dem Sie das Ergebnis der Einlastung prüfen können.
  ⇨ "Einlasten Ergebnis" auf Seite H-289
- **Priorität übernehmen:** Übernimmt die geänderte Priorität und schreibt sie in den Auftrag zurück. Nur wenn Sie die Änderung in den Auftrag zurückschreiben, wird sie bei der Einlastung berücksichtigt.
- **Einlastung löschen:** Löscht den eingelasteten Auftrag aus der Kapazitätsplanung, z. B., um ihn unter geänderten Kriterien erneut einzulasten oder bei Stornierungen. Der Auftrag wird aus der Kapazitätsplanung gelöscht, die reservierten Kapazitäten werden wieder freigegeben.
- **An Produktion übergeben:** Übergibt den Auftrag direkt an die Produktion.
- **Meldungen anzeigen:** Zeigt nach der Einlastung eine Meldung mit verschiedenen Informationen zur Einlastung an. Der Eintrag ist nur freigeschaltet, wenn Sie mit Administratorrechten angemeldet sind.

#### Gruppe Einstellungen
- **Terminsuche:** Öffnet den gleichnamigen Dialog, in dem Sie Kriterien zur Terminsuche festlegen können.
  ⇨ "Kriterien ändern (Modus Terminsuche)" auf Seite H-281
- **Schichtzeiten:** Öffnet den Dialog Einstellung Schichten, in dem Sie den Schichtübergang und die Sperrzeiten festlegen können.
  ⇨ "Einstellungen Schichten" auf Seite H-187
  Sie müssen Administratorrechte haben, um den Dialog zu öffnen. Zusätzlich muss in den Firmendaten die Checkbox Schichtwechseltabelle verwenden markiert sein.
  ⇨ "Schichtwechseltabelle verwenden" auf Seite H-186
- **Schicht wählen:** Schaltet das Feld Schicht frei, um die gewünschte Schicht einzutragen.
- **Restmengenübertragung:** Öffnet den Dialog Restmengen-Übertragung, in dem Sie festlegen können, bis zu welchem Status Aufträge auf Restmengen geprüft werden sollen.
  ⇨ "Restmengenübertragung" auf Seite H-300

### Menü Optionen
**Fertigung > Kapazitätsplanung > Einlastung > Einlasten Auftrag**

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen. Folgende Einträge werden angezeigt:
- **Alter Verweiltagemodus:** Diese Einstellung ist nur erforderlich, wenn Sie den alten Modus für Verweiltage (= Übergangsmatrix) beibehalten wollen
- **Check auf Rüstzeit:** Wenn die Rüstzeit zu mehreren Arbeitsarten eingerichtet ist, die für eine Auftragsposition ausgeführt werden, dann soll diese Zeit nur einmal pro Position berechnet werden.
- **Pos. Control:** Beim Einlasten wird der Anteil des Auftrags an der Tageskapazität geprüft. Der Prozentwert ist im Dialog Arbeitsarten hinterlegt.
  ⇨ "% Limit" auf Seite H-194
- **Sperrstunde für Einlastung berücksichtigen:** Beim Einlasten soll geprüft werden, bis zu welcher Uhrzeit Aufträge in die Schicht eingelastet werden dürfen.
  ⇨ "Einstellungen Schichten" auf Seite H-187

### Einlasten Auftrag (Dialog)
**Fertigung > Kapazitätsplanung > Einlastung > Einlasten Auftrag**

*(Abb. H-183 Auftrag manuell einlasten)*

In diesem Dialog lasten Sie einen einzelnen Auftrag oder auch eine einzelne Position eines Auftrages manuell in die Kapazitätsplanung ein.
⇨ Tutorial, "Einlastung der Aufträge" auf Seite H-113

#### Auftragsinformationen
- **Auftrag**: Eingabe der Auftragsnummer.
- **Kunde**: Anzeige des Kundennamens.
- **Versandtag**: Versandtag aus dem Auftrag. Sie können das Datum überschreiben. Die Änderung wird in den Auftrag zurückgeschrieben. Wenn Sie die Checkbox **Liefertermin beibehalten** markiert haben, können Sie keinen anderen Termin auswählen.
  > **Produktion vorziehen**
  > Um die Terminierung der Produktion vorzuverlegen, müssen Sie erst den Versandtag ändern und anschließend die Checkbox Liefertermin beibehalten markieren.
- **Schicht**: Angabe der Schichtnummer, in der der Auftrag gefertigt werden soll. Das Feld wird über das Menü **Funktionen > Gruppe Einstellungen > Schicht wählen** freigeschaltet.
- **Status**: Aktueller Auftragsstatus.
- **Priorität**: Standardmäßig werden die Aufträge mit der Priorität **Normal** eingelassen. Sie können eine andere Priorität wählen und über das Menü **Funktionen > Gruppe Einstellungen > Priorität übernehmen** in den Auftrag zurückschreiben. Erst danach wird die neue Priorität beim Einlasten berücksichtigt. Folgende Einträge stehen zur Wahl:
    - **Abruf:** Der Auftrag wird erst gefertigt, wenn der Kunde die Positionen abruft.
    - **Eilt:** Der Auftrag muss mit oberster Priorität eingelastet werden.
    - **Normal:** Der Auftrag wird den Standard-Einstellungen entsprechend eingelastet.
    - **Zugabe:** Diese Priorität bedeutet, dass der Auftrag so gefertigt werden soll, dass er Reste und Restplatten verbraucht, die beim Zuschnitt anderer Aufträge entstehen.

> **Auftragspriorität berücksichtigen**
> Wenn außer der Auftragspriorität Normal auch z. B. die Priorität Eilt berücksichtigt werden soll, dann müssen dafür eigene Übergangszeiten eingerichtet sein. Wenn diese nicht eingerichtet sind, wird mit der Priorität Normal eingelastet.
> ⇨ "Übergangszeiten" auf Seite H-197
> ⇨ "Übergangsmatrix" auf Seite H-216

#### Optionen
- **Einzelne Position einlasten**: Sie können aus einem Auftrag einzelne Positionen einlasten.
  - [ ] Alle Positionen des Auftrags werden eingelastet.
  - [x] Das Feld für die Eingabe der Positionsnummer wird freigeschaltet. Nur diese eine Position wird dann eingelastet.
- **Positionsnummer**: Eingabe der Position, die eingelastet werden soll. Das Feld ist nur freigeschaltet, wenn die Checkbox **Einzelne Position einlasten** markiert ist.
- **Auch Priorität -1 verwenden**: Bei der Wahl des Aggregats werden die Prioritäten der Aggregate berücksichtigt. Standardmäßig wird die Verfügbarkeit des Aggregats mit der höchsten Priorität geprüft. Die Priorität -1 wird in aller Regel den Aggregaten für die manuelle Auswahl zugewiesen, z. B. dem Handzuschnitt.
  - [ ] Auf Aggregate mit der Priorität -1 kann nur manuell eingelastet werden.
  - [x] Die Aggregate mit der Priorität -1 werden in die Planung einbezogen.
- **Liefertermin beibehalten**: Wenn die Auslastung der Maschinen den Liefertermin unmöglich macht, kann dieser verschoben werden.
  - [ ] Bei der Einlastung des Auftrags ist eine Verschiebung des Liefertermins zulässig.
  - [x] Der Auftrag soll so eingelastet werden, dass der Liefertermin aus dem Auftrag eingehalten wird. Mit dieser Einstellung können Sie im Feld **Versandtag** keinen anderen Termin auswählen.
- **Frühester Produktionsstart**: Wenn Sie einen Liefertermin haben, der weit in der Zukunft liegt, können Sie festlegen, wann frühestens mit der Produktion begonnen werden soll.

#### Aktuelle Einlastung
In diesem Bereich wird angezeigt, welche Position aktuell eingelastet wird.

#### Artikel/Bearbeitungen
In der Übersicht werden die Produktbezeichnungen und Bearbeitungen der einzelnen Positionen angezeigt.

## Einlasten Ergebnis
**Fertigung > Kapazitätsplanung > Einlastung > Einlasten Auftrag > Menü Funktionen > Einlastungsergebnis**

*(Abb. H-184 Ergebnis der Einlastung)*

In diesem Dialog prüfen Sie, wie der Auftrag eingelastet wurde.

### Arbeitsgänge
In der Übersicht werden die Positionen pro Arbeitsart angezeigt:
- **Pos.:** Positionsnummer aus dem Auftrag.
- **Aggregat:** Bezeichnung der Maschine.
- **Arbeitsart:** Arbeitsart, die an der Maschine ausgeführt wird.
- **Zeit:** Verplante Zeit pro Position und Arbeitsart. In der Summenzeile wird die Gesamtzeit für den Auftrag angezeigt.
- **Stück:** Anzahl der Arbeitsschritte, das wären z. B. 10 Scheiben beim Zuschnitt, aber 4 x 10 Stück bei Rundecken.
- **Datum:** Fertigungsdatum.
- **Schicht:** Schicht, in der die Position eingelastet ist.
- **Kosten:** Kosten pro Arbeitsart und Position. In der Summenzeile werden die Gesamtkosten für den Auftrag angezeigt.

### Ergebnis sortieren
Mit der Wahl der Option legen Sie fest, wie die Darstellung sortiert werden soll:
- **Nach Position:** Pro Positionen werden die Arbeitsarten aufgelistet.
- **Nach Produktionsdatum:** Die Positionen werden nach dem Datum der jeweiligen Arbeitsart aufgelistet.

### Summen
In diesem Bereich werden die Summen für die Zeiten und Kosten angezeigt, die für den eingelasteten Auftrag errechnet wurden.

## Aggregat-Auswahl bei Engpass
**Fertigung > Kapazitätsplanung > Einlastung > Einlasten Auftrag > Einlasten > (Engpass)**

*(Abb. H-185 Engpass bei Einlastung – Aggregat auswählen)*

In diesem Dialog wählen Sie manuell eine andere Maschine aus. Der Dialog wird beim Einlasten automatisch angezeigt, wenn die Standard-Maschine mit der Priorität 9 ausgelastet ist.
⇨ Tutorial, "Kapazitätsprobleme" auf Seite H-119

### Kapazitätsengpass
- **Auftrag, Kunde, Versandtag**: Anzeige der Auftragsnummer, des Kundennamens und des Versandtermins aus dem Auftrag.
- **Pos./Teil/Unterpos.**: Anzeige von Positionsnummer, Ebene der Stückliste und bei gesplitteten Positionen die Nummer der Unterposition, bei denen der Kapazitätsengpass auftritt.
- **Anzahl**: Stückzahl der Position.
- **Produkt, Abmessung**: Produktbezeichnung und Maße der Auftragsposition
- **Arbeitsart**: Arbeitsart, bei der der Engpass auftritt.

### Produktion
- **Datum**: Geplantes Produktionsdatum. Mit den Pfeiltasten können Sie das Datum vor- oder zurückschieben.
- **Schicht**: Geplante Schicht. Mit den Pfeiltasten können Sie die Schicht am selben Tag vor- oder zurückschieben. Wenn Sie nur mit einer Schicht arbeiten, wird das Datum verschoben.

### Mögliche Aggregate
In der Übersicht werden alle Aggregate angezeigt, an denen die Arbeitsart ebenfalls ausgeführt werden kann.
- **Aggregat:** Ausweichmaschinen.
- **Zeit benötigt:** Zeit, die für den Vorgang bei der angezeigten Position und Stückzahl benötigt wird.
- **Zeit reserviert:** Zeit, die auf der angezeigten Maschine bereits für andere Aufträge reserviert ist.
- **Rüstzeit:** Zeit, die zum Einrichten der Maschine benötigt wird, wenn die angezeigten Positionen gefertigt werden sollen.
- **Maximalzeit:** Schichtzeit der Maschine an dem ausgewählten Datum.

### Schaltflächen
- **[Übersicht]**: Öffnet den Dialog **Auftragsnummern**, in dem Sie prüfen können, welche Aufträge bei den aktuellen Vorgaben bereits an der Maschine eingelassen sind.
  ⇨ "Auftragsnummern" auf Seite H-293
- **[Abgleich]**: Zurzeit nicht genutzt.
- **[Positions-Split]**: Öffnet den Dialog **Positions-Split**, in dem Sie die Position in Unterpositionen aufteilen können.
  ⇨ "Positions-Split" auf Seite H-294
- **[Kriterien]**: Öffnet den Dialog **Kriterien ändern**.
  ⇨ "Kriterien ändern (Modus Terminsuche)" auf Seite H-281
- **[Einlasten]**: Lastet die Position zu den eingestellten Bedingungen ein. Je nach Einstellung müssen Sie dabei jede Arbeitsart pro Position einzeln einlasten. Wenn alle Positionen eingelastet sind, wird eine Meldung mit den Änderungen angezeigt.
- **[Vortag einlasten]**: Lastet die Position zu den eingestellten Bedingungen am Vortag ein. Dazu sollten Sie im Feld Schicht zunächst z. B. die letzte Schicht des Vortags auswählen.

## Auftragsnummern
**Fertigung > Kapazitätsplanung > Einlastung > Einlasten Auftrag > Aggregat-Auswahl bei Engpass > [Übersicht]**

*(Abb. H-186 Engpass bei Einlastung – Übersicht über die eingelasteten Aufträge)*

In diesem Dialog prüfen Sie, welche Aufträge zu den eingestellten Bedingungen bereits an der Maschine eingelastet sind.

## Positions-Split
**Fertigung > Kapazitätsplanung > Einlastung > Einlasten Auftrag > Einlasten > Aggregatauswahl bei Engpass > [Positions-Split]**

*(Abb. H-187 Engpass bei Einlastung – Position splitten)*

In diesem Dialog teilen Sie eine Auftragsposition in mehrere Unterpositionen auf.
⇨ Tutorial, "Kapazitätsprobleme" auf Seite H-119

### Positionsinformationen
- **Auftrag, Position**: Auftragsnummer und Nummer und Produktbezeichnung für die Auftragsposition.
- **Produkt, Stückzahl**: Produktnummer und Stückzahl der Auftragsposition.

### Split
In diesem Bereich geben Sie ein, wie die Position aufgeteilt werden soll. Die Teilung der Position in Unterpositionen wird in der Übersicht angezeigt.
Wenn Sie im Bereich **Optionen** die Checkbox **Produktionsdatum vorgeben** markiert haben, werden neben der Stückzahl auch das Datum und die Schicht angezeigt. Die gewünschten Werte können Sie direkt in diese Felder schreiben.

**Anzahl**
Eingabe der Anzahl. Über die nachfolgenden Schaltflächen legen Sie fest, ob die Zahl als Schicht- oder als Stückzahl interpretiert werden soll.

**[Split zurücksetzen]**
Setzt die Aufteilung der Position zurück. Sie können dann andere Möglichkeiten für die Teilung der Position ausprobieren.

**[Anzahl = Schichten]**
Der Wert im Feld **Anzahl** soll sich auf die Schichten beziehen, z. B. 2 Schichten. Die Stückzahl der Position wird gleichmäßig auf die Anzahl der Schichten aufgeteilt. In der Übersicht können Sie die Werte überschreiben.

**[Anzahl = Stück pro Schicht]**
Der Wert im Feld **Anzahl** soll sich auf die Stückzahl pro Schichten beziehen, z. B. 50 Stück pro Schicht.
Wenn Sie keine Angaben zur Anzahl gemacht haben, werden so viele Unterpositionen erzeugt, wie die Vorgaben aus den Firmendaten zulassen, z. B. 50% der Schicht. In der Übersicht können Sie die Werte überschreiben.
⇨ "Schichtfüllung bei Positionssplit" auf Seite H-184

### Optionen
**Max. Arbeitsart bei Datumsvorgabe**
Das Feld ist nur freigeschaltet, wenn die Checkbox **Produktionsdatum vorgeben** aktiviert ist. Es darf nicht leer bleiben.
Sie können beim Positionssplit Produktionstermine vorgeben. In diesem Fall können Sie zusätzlich angeben, ab welcher Arbeitsart diese Termine nicht gelten sollen. Diese Einstellung ist sinnvoll, damit die Unterpositionen z. B. nicht getrennt verpackt und versendet werden.

**Verkürzte Kontrolle**
Normalerweise prüft die Einlastung für jede Position, an welchem Tag noch Kapazitäten zur Verfügung stehen, um die Position dort einzulasten. In einem Auftrag können jedoch Positionen mit gleichem Stücklistenaufbau enthalten sein, die sich nur durch die Maße unterscheiden.
- [ ] Bei jeder Position wird der gesamte Stücklistenaufbau geprüft.
- [x] Bei gleichem Stücklistenaufbau wird von der Einlastung der vorigen Position ausgegangen, ohne die Stückliste neu zu prüfen. Dies ist die Standard-Einstellung.
Das Programm merkt sich den Starttermin der Produktion der ersten Position, z. B. für die Schleifmaschine. Die Folgeposition setzt genau auf diesem Termin auf, um die Kapazität für diese Maschine zu prüfen und geht, falls die Maschine für diesen Tag ausgelastet ist, auf die vorherige Schicht bzw. den vorherigen Tag. Die nächste Position setzt wiederum auf diesem neuen Termin für die Prüfung der Kapazität auf usw.

**Mit Sperren**
Beim Splitten kann die verbleibende Schichtzeit für andere Aufträge gesperrt werden, z. B. damit die Maschine nicht umgerüstet werden muss.
- [ ] Restzeiten in der Schicht oder dem Tag sind nicht für andere Aufträge gesperrt.
- [x] Nur die Unterpositionen, die durch das Splitten entstanden sind, werden gefertigt. Restzeiten werden nicht anders verplant.

**Produktionsdatum vorgeben**
Sie können pro Unterposition ein Datum vorgeben.
- [ ] Das Datum kann nicht vorgegeben werden.
- [x] In der Übersicht werden die Spalten Datum und Schicht angezeigt, im Bereich Optionen das Feld Max. Arbeitsart bei Datumsvorgabe.

### Aktionen
**[OK]** Übernimmt die Daten. Die Einlastung wird mit den neuen Unterpositionen fortgesetzt.

**[Ende]** Bricht die Teilung ab. Der Dialog **Aggregat-Auswahl bei Engpass** wird wieder im Vordergrund angezeigt.

**[Übersicht]** Öffnet den Dialog **Positions-Zeiten**.

## Positions-Zeiten
**Fertigung > Kapazitätsplanung > Einlastung > Einlasten Auftrag > Einlasten > Aggregatauswahl bei Engpass > [Positions-Split] > [Übersicht]**

*(Abb. H-188 Engpass bei Einlastung – Übersicht im Positions-Split)*

In diesem Dialog prüfen Sie die Zeiten, die für die aktuelle Position benötigt werden. In roter Schrift sind die Zeiten angezeigt, für die keine Kapazitäten zur Verfügung stehen.

## Aggregate Ausfall
**Fertigung > Kapazitätsplanung > Einlastung > Aggregate Ausfall**

Aggregate können vorübergehend oder ganz gesperrt werden. Die bereits eingelasteten Aufträge müssen dann umgelastet werden. Die Abfrage zum Umlasten startet, wenn Sie ein Aggregat sperren, an dem bereits Aufträge eingelastet sind. Sie sollten daher zuvor den Modus einstellen.
⇨ "Kriterien ändern (Modus Terminsuche)" auf Seite H-281

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite H-297
- "Menü Optionen" auf Seite H-298
- "Aggregate Ausfall (Dialog)" auf Seite H-299

### Menü Funktionen
**Fertigung > Kapazitätsplanung > Einlastung > Aggregate Ausfall**

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Dialog Aggregate Ausfall zu schließen.

#### Gruppe Terminsuche
- **Kriterien ändern:** Öffnet den gleichnamigen Dialog, in dem Sie Kriterien zur Terminsuche festlegen können.
  ⇨ "Kriterien ändern (Modus Terminsuche)" auf Seite H-281

#### Gruppe Restmengen
- **Übertragen:** Öffnet den Dialog Restmengenübertragung, in dem Sie festlegen können, bis zu welchem Status Aufträge auf Restmengen geprüft werden sollen.
  ⇨ "Restmengenübertragung" auf Seite H-300

#### Gruppe Einlastung
- **Auswahl einlasten:** Öffnet den Dialog Auftrag einlasten, um die markierten Aufträge auf andere Aggregate umzulasten.
  ⇨ "Einlasten Auftrag" auf Seite H-284

#### Gruppe Zeitwirtschaft
- **Schichten:** Öffnet den Dialog Einstellung Schichten, in dem Sie den Schichtübergang und die Sperrzeiten festlegen können.
  ⇨ "Einstellungen Schichten" auf Seite H-187
  Sie müssen Administratorrechte haben, um den Dialog zu öffnen. Zusätzlich muss in den Firmendaten die Checkbox Schichtwechseltabelle verwenden markiert sein.
  ⇨ "Schichtwechseltabelle verwenden" auf Seite H-186

### Menü Optionen
**Fertigung > Kapazitätsplanung > Einlastung > Aggregate Ausfall**

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

#### Gruppe Verweiltage
- **Alten Verweiltagemodus verwenden:** Diese Einstellung ist nur erforderlich, wenn Sie den alten Modus für Verweiltage (= Übergangsmatrix) beibehalten wollen

#### Gruppe Rüstzeit
- **Prüfen:** Wenn die Rüstzeit zu mehreren Arbeitsarten eingerichtet ist, die für eine Auftragsposition ausgeführt werden, dann soll diese Zeit nur einmal pro Position berechnet werden.

#### Gruppe Einlastung
- **Positionskontrolle:** Beim Einlasten wird der Anteil des Auftrags an der Tageskapazität geprüft. Der Prozentwert ist im Dialog Arbeitsarten hinterlegt.
  ⇨ "% Limit" auf Seite H-194
- **Sperrstunde berücksichtigen:** Beim Einlasten soll geprüft werden, bis zu welcher Uhrzeit Aufträge in eine Schicht eingelastet werden dürfen.
  ⇨ "Einstellungen Schichten" auf Seite H-187

### Aggregate Ausfall (Dialog)
**Fertigung > Kapazitätsplanung > Einlastung > Aggregate Ausfall**

*(Abb. H-189 Aggregat-Ausfall)*

In diesem Dialog hinterlegen Sie Ausfallzeiten für Ihre Maschinen, damit die Kapazitätsplanung diese bei der Planung berücksichtigen kann. Solche Ausfallzeiten entstehen z. B. wegen Wartungsarbeiten oder Reparaturen.
⇨ Tutorial, "Sperren" auf Seite H-95

#### Auswahl
- **Aggregat**: Auswahl der Maschine, der Ausfallzeiten zugeordnet werden sollen. Die Ausfallzeiten werden nur in Tagen angegeben, nicht in Schichten.
- **Ausfall von/bis**: Zeitraum, für den diese Maschine vermutlich ausfällt. Wenn Sie die eingegebenen Zeiten speichern, werden die betroffenen Aufträge in der Übersicht angezeigt. Die Aufträge können automatisch auf anderen Maschinen eingelastet werden. Dazu wird eine Abfrage angezeigt, mit der Sie die Verschiebung bestätigen oder ablehnen können.

#### Daten
In der Übersicht werden alle Aggregate aufgeführt, für die Ausfallzeiten eingetragen sind.

#### Betroffene Aufträge
In der Übersicht werden alle Aufträge aufgelistet, die auf dem markierten Aggregat eingelastet sind. In der Spalte **Stunden** wird die Zeit angezeigt, die für den Auftrag auf der gesperrten Maschine reserviert ist.

## Restmengenübertragung
**Fertigung > Kapazitätsplanung > Einlastung > Einlasten Auftrag > Menü Funktionen > Gruppe Einstellungen > Restmengenübertragung**

*(Abb. H-190 Übertragung von Restmengen)*

In diesem Dialog legen Sie den Status fest, bis zu dem der Workflow-Task nach nicht gefertigten Restmengen aus dem Vortag sucht. Berücksichtigt werden nur Aufträge und Positionen, die am Vortag hätten gefertigt werden sollen, aber noch nicht begonnen wurden.
⇨ Tutorial, "Restmengen vom Vortag" auf Seite H-144
