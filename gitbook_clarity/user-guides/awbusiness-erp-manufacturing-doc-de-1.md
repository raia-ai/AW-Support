---
description: "A+W Business Fertigung Software Reference Manual"
---


---
## Softwarereferenz Gestelle

> **Einheitlicher Kunde**
> Achten Sie darauf, dass Sie zum Druck nur Gestelle aktivieren, die an einen einzigen Kunden oder Lieferanten gegangen sind. Markieren Sie die Zeile mit einem Doppelklick in die erste Zelle. Für jeden Kunden wird eine Mahnung gedruckt.

### Auswahl

**Kunde von, bis**
Sie können eine einzelne Kundennummer eingeben oder eine Spanne von Nummern. Der Name des ersten und des letzten Kunden wird angezeigt.

**Auswärtig .. - .. Tage**
Sie können nach Gestellen suchen, die seit einer bestimmten Anzahl von Tagen außer Haus sind, z. B. 30 - 60 Tage.

**Mahnstatus**
Sie können die Anzeige auf die Gestelle einschränken, die bereits angemahnt wurden. Wenn Sie die Suche nicht auf eine bestimmte Mahnstufe einschränken, werden alle Gestelle angezeigt.

> **Mahnstatus zurücksetzen**
> Wenn Sie in diesem Register den Mahnstatus zurücksetzen, wird bei allen in der Übersicht angezeigten Gestellen der Mahnstatus auf Null gesetzt. Wenn Sie den Mahnstatus für einzelne Gestelle zurücksetzen wollen, müssen Sie entweder nur das entsprechende Gestell in die Übersicht holen oder den Dialog Mahnstatus zurücksetzen im Auswahlmodus starten.
>
> ⇨ "Mahnstatus zurücksetzen" auf Seite E-259

### Optionen

**Wiederholungsdruck**
Den Wiederholungsdruck müssen Sie dann starten, wenn Sie eine Mahnung erneut drucken wollen.
- Die Mahnung wird zum ersten Mal gedruckt.
- Die Mahnung wird erneut gedruckt.

**(Versandart)**
Die Mahnung kann auf verschiedene Arten versendet werden.
- **Postversand:** Die Mahnung wird per Post versendet. Das Dokument wird ausgedruckt.
- **Faxversand:** Die Mahnung wird per Fax versendet.
- **Mail:** Die Mahnung wird per Mail versendet.

### Mahntexte

**Kopf, Fuß**
Sie können für die Kopf- und Fußzeilen der Mahnung unterschiedliche Texte auswählen. Alternativ zu den hinterlegten Texten können Sie auch in beiden Feldern einen eigenen Text schreiben.

## Auswärtige Gestelle

In der Übersicht werden alle Gestelle angezeigt, die den Auswahlkriterien entsprechen.

- **Nummer:** Gestellnummer.
- **Art:** Gestellart.
- **Kunde:** Name des Kunden, an den das Gestell ausgeliefert wurde.
- **Faxnummer:** Faxnummer des Kunden.
- **Mail:** Mail-Adresse des Kunden.
- **Mahnstatus:** Nur bei bereits gemahnten Gestellen wird ein Mahnstatus angezeigt.
- **Ausgabedatum:** Datum, zu dem das Gestell ausgebucht wurde.
- **Tage ausw.:** Anzahl der Tage seit dem Ausgabedatum.
- **Latten, Räder, Wagen:** Anzahl der Latten, Räder und Wagen, die zum Gestell gehören.
- **Gesperrt:** Das Gestell ist für weitere Buchungen gesperrt.
- **Verloren:** Das Gestell ist nicht im Bestand, sein Verbleib kann nicht geklärt werden.
- **Stationär:** Das Gestell wird nur stationär verwendet.

## Gestellverwaltung

**Fertigung > Gestellverwaltung**

Sie können die Verpackung von produzierten Aufträgen auf Gestellen planen und steuern. Dazu stehen im Menü Gestellverwaltung folgende Dialoge zur Verfügung.

- Gestellarten
- Gestelle
- Kundenkommissionen

In diesem Abschnitt finden Sie Informationen zu folgenden Dialogen des Programmbereichs:

- "Gestellarten" auf Seite E-254
- "Gestelle" auf Seite E-238
- "Gestellübersicht" auf Seite E-256
- "Übersicht Partner" auf Seite E-257
- "Mahnstatus zurücksetzen" auf Seite E-259
- "Gestell umbuchen" auf Seite E-258
- "Kundenkommissionen" auf Seite E-264

## Gestellarten

**Fertigung > Gestellverwaltung > Gestellarten**

*Abb. E-122 Gestellarten*

In diesem Dialog können Sie unterschiedliche Gestellarten anlegen. Die Gestellarten werden den Gestellen zugewiesen. Sie dienen zur Organisation von Gestellen gleicher Machart.

### Gestellart

**Bezeichnung**
Name der Gestellart.

**Bemerkung**
Anmerkung zur Gestellart, z. B. Verwendung nicht außer Haus.

**Max. Breite / Max. Höhe**
Größte zulässige Breite und Höhe der Scheiben, die das Gestell aufnehmen kann.

**Eigengewicht / Max. Gew.**
Eigengewicht der Gestellart und Höchstgewicht im beladenen Zustand. Die Differenz ergibt die zulässige Beladung.

**Gestellwert**
Als Wert des Gestells können Sie z. B. den Anschaffungspreis angeben, oder den Verleihwert.

**Gestelltyp**
Typ des Gestells, z. B. A-Gestell oder Fächerwagen.

### Standard bei Neuanlage

**Anzahl Spannlatten**
Die Angabe der Spannlatten dient dazu, bei der Rückgabe des Gestells dessen Vollständigkeit zu prüfen.

**Anzahl Räder**
Die Angabe der Räder dient dazu, bei der Rückgabe des Gestells dessen Vollständigkeit zu prüfen.

**Anzahl Wagen**
Die Angabe der Wagen dient dazu, bei der Rückgabe des Gestells dessen Vollständigkeit zu prüfen.

**Stationär**
Gestelle können sowohl zum Transport von Gläsern dienen, als auch als Abstellplatz.
- Das Gestell kann frei verwendet werden, z. B. auch für Lieferungen außer Haus.
- Das Gestell hat einen festen Standort. Es kann nicht für Lieferungen verwendet werden.

### Tabelle

In der Übersicht werden alle Gestellarten aufgelistet, die den Suchkriterien entsprechen.

- **Bezeichnung:** Name der Gestellart.
- **Bemerkung:** Bemerkung zur besonderen Verwendung, Größe usw.
- **Max. Breite, max. Höhe:** Höchste zulässige Größe der Scheiben.
- **Eigengewicht:** Gewicht ohne Beladung.
- **Max. Gewicht:** Höchstgewicht im beladenen Zustand.
- **Wert:** Anschaffungs- oder Verleihwert.
- **Latten, Räder, Wagen:** Anzahl der Spannlatten, Räder und Wagen.
- **Stat.:** Angabe, ob das Gestell stationär verwendet wird.

## Gestellübersicht

**Fertigung > Gestellverwaltung > Gestelle > Register Gestelle > Schaltfläche am Feld Nummer**

*Abb. E-123 Gestellübersicht*

In diesem Dialog prüfen Sie die Gestellnummern, wenn Sie ein neues Gestell anlegen möchten.

### Gestelle

**Gesamt**
Anzahl der angelegten Gestellnummern.

**Verfügbar**
Anzahl der verfügbaren Gestelle.

### Auswahl

- **Gestellnummer:** Nummer des Gestells.
- **Gestellart:** Art des Gestells.
- **Kundennummer, Name:** Nummer und Name des Kunden.
- **Ausgabedatum:** Datum, zu dem das Gestell außer Haus gebucht wurde.

## Übersicht Partner

**Fertigung > Gestellverwaltung > Gestelle > Register Historie > [Ordner]**

*Abb. E-124 Gestelle - Übersicht Partner*

In diesem Dialog prüfen Sie, welche Gestelle bei einem bestimmten Marktpartner stehen oder gestanden haben.

### Auswärtig

In diesen Feldern werden die Summen angezeigt:

- **Gestelle:** Anzahl der Gestelle, die zurzeit bei diesem Partner sind.
- **Latten:** Anzahl der Latten, die zurzeit beim Partner sind.
- **Räder:** Anzahl der Räder, die zurzeit beim Partner sind.
- **Wagen:** Anzahl der Wagen, die zurzeit beim Partner sind.

### Gestelle

- **Gestellnr.:** Nummer des angelegten Gestells.
- **Gestellart:** Art des Gestells.
- **Ausgabe:** Datum, zu dem das Gestell außer Haus gebucht wurde.
- **Rückgabe:** Datum, zu dem der Gestelleingang gebucht wurde.
- **Latten, Räder, Wagen:** Anzahl der Latten, Räder oder Wagen, die zu dem Gestell gehören.

## Gestell umbuchen

**Fertigung > Gestellverwaltung > Gestelle > Menü Funktionen > Gruppe Ausführen > Gestell umbuchen**

*Abb. E-125 Gestell umbuchen*

In diesem Dialog buchen Sie ein Gestell von einem Partner auf einen anderen um.

### Auswärtige Gestelle

In der Übersicht werden alle Gestelle angezeigt, die zurzeit außer Haus sind.
- **Nummer:** Nummer des angelegten Gestells.
- **Gestellart:** Art des Gestells.
- **Kunde:** Nummer des Kunden.
- **Ausgabe:** Datum, zu dem das Gestell außer Haus gebucht wurde.

### Gestell

**Nummer**
Nummer des markierten Gestells

**Art**
Gestellart des markierten Gestells

### Umbuchen

**Von**
Nummer und Name des Partners, auf den das auswärtige Gestell gebucht ist.

**Nach**
Sie können die Nummer des neuen Partners eintragen oder über die Suche auswählen.

## Mahnstatus zurücksetzen

**Fertigung > Gestellverwaltung > Gestelle > Menü Funktionen > Gruppe Ausführen > Mahnstatus zurücksetzen**

*Abb. E-126 Mahnstatus zurücksetzen*

In diesem Dialog setzen Sie den Mahnstatus für einzelne Gestelle zurück.

## Gestellbelegung

**Fertigung > Gestellverwaltung > Gestelle > Register Gestelle > Menü Funktionen > Gruppe Ausführen > Gestellbelegung**

In diesem Dialog können Sie die Zuordnung von Auftragspositionen zu Gestellen festlegen.

> **Voraussetzung**
> Sie können eine Zuordnung nur festlegen, wenn Sie Gestelle angelegt haben und die Gestelle verfügbar sind. Gestelle können Sie in der Gestellverwaltung im Register Gestelle anlegen.

In diesem Dialog finden Sie folgende Register:
- "Gestellbelegung - Nach Auftrag" auf Seite E-260
- "Gestellbelegung – Nach Gestell" auf Seite E-262

## Gestellbelegung – Nach Auftrag

**Fertigung > Gestellverwaltung > Gestelle > Menü Funktionen > Gruppe Ausführen > Gestellbelegung > Register Nach Auftrag**

*Abb. E-127 Gestellbelegung – Nach Auftrag*

In diesem Register ordnen Sie den einzelnen Positionen eines Auftrags die Gestelle zu. Sie können zusätzlich festlegen, welche Menge einer Position auf dem Gestell abgestellt werden soll. Sie können mehrere Positionen demselben Gestell zuordnen.

### Auswahl

**Auftrag**
Nummer des Auftrags.

**Kunde**
Nummer und Name des Kunden. Die Felder werden gefüllt, wenn Sie die Auftragsnummer eintragen.

**[Zuordnungen entfernen]**
Löscht alle Zuordnungen der Auftragspositionen zu den Gestellen aus der Übersicht. Wenn Sie nur eine Auftragsposition aus der Zuordnung löschen wollen, müssen Sie im Menü Start auf [Löschen] klicken.

### Übersicht

In der Übersicht werden alle Positionen des ausgewählten Auftrags mit den Zuordnungen zu den Gestellen angezeigt. Sie können Zuordnungen zu einem Gestell bearbeiten oder neue Zuordnungen erstellen. Nur die Felder Gestell, Suche und Scheiben auf Gestell können bearbeitet werden, die anderen Felder werden automatisch gefüllt.

- **Pos:** Nummer der Auftragsposition.
- **Bezeichnung:** Bezeichnung des Glases.
- **Breite, Höhe:** Maße der Position.
- **Positionsmenge:** Stückzahl der Position.
- **Gewicht pro Stück:** Gewicht eines Stücks der Position.
- **Noch nicht abgestellt:** Stückzahl der Position, die noch keinem Gestell zugeordnet ist.
- **Gestell:** Nummer des Gestells, dem die Position zugeordnet werden soll.
- **Max. Höhe, Max Breite:** Höchste zulässige Maße der Scheiben. Die Felder werden automatisch gefüllt, wenn eine Gestellnummer eintragen ist.
- **Max. Gewicht:** Höchstgewicht im beladenen Zustand. Das Feld wird automatisch gefüllt, wenn eine Gestellnummer eintragen ist.
- **Suche:** Öffnet den Dialog Gestellübersicht, in dem Sie ein Gestell wählen können. Die Maße und das Gewicht des gewählten Gestells werden in der Tabelle übernommen. Das Feld Scheiben auf Gestell wird standardmäßig mit der Stückzahl aus dem Feld Positionsmenge gefüllt.
- **Scheiben auf Gestell:** Stückzahl der Scheiben, die dem gewählten Gestell zugeordnet werden sollen. Wenn Sie dem Gestell weniger Scheiben zuordnen als die Gesamtstückzahl der Position, wird automatisch eine neue Zeile mit der Differenzstückzahl der Position angezeigt. Sie können diese Stückzahl einem anderen Gestell zuordnen.

**Gesamt**
Gesamtstückzahl der Auftragspositionen.

**Rest**
Gesamtstückzahl der Positionen, die keinem Gestell zugeordnet sind.

**Auf Gestell**
Gesamtstückzahl der Positionen, die einem Gestell zugeordnet sind.

## Gestellbelegung – Nach Gestell

**Fertigung > Gestellverwaltung > Gestelle > Menü Funktionen > Gruppe Ausführen > Gestellbelegung > Register Nach Gestell**

*Abb. E-128 Gestellbelegung – Nach Gestell*

In diesem Register ordnen Sie einem Gestell einzelne Positionen eines Auftrags zu. Sie können zusätzlich festlegen, welche Menge einer Position auf dem Gestell abgestellt werden soll.

### Auswahl

**Gestell/Gestellart**
Nummer und Art des Gestells. Sie können nur die Nummer des Gestells angeben, dem Positionen zugeordnet werden sollen. Das Feld Gestellart wird gefüllt.

**Max. Breite/Höhe/Gewicht**
Höchste zulässige Maße der Scheiben und Höchstgewicht des beladenen Gestells. Die Felder werden gefüllt, wenn Sie eine Gestellnummer eintragen.

**[Gestell leeren]**
Löscht alle Zuordnungen der Auftragspositionen zu dem markierten Gestell aus der Übersicht. Wenn Sie nur eine Auftragsposition aus der Zuordnung löschen wollen, müssen Sie im Menü Start auf [Löschen] klicken.

### Übersicht

In der Übersicht werden alle Positionen angezeigt, die dem ausgewählten Gestell zugeordnet sind. Sie können die Zuordnungen bearbeiten oder Positionen neu zuordnen. Nur die Felder Auftrag, Pos und Scheiben auf Gestell können bearbeitet werden, die anderen Felder werden automatisch gefüllt.

- **Auftrag:** Nummer des Auftrags.
- **Pos:** Nummer der Auftragsposition.
- **Bezeichnung:** Bezeichnung des Glases.
- **Maße:** Maße der Position.
- **Kunde:** Nummer des Kunden.
- **Maximal abstellbar:** Stückzahl der Position, die noch keinem Gestell zugeordnet ist.
- **Gewicht:** Gewicht der Stückzahl einer Position, die einem Gestell zugeordnet ist.
- **Scheiben auf Gestell:** Stückzahl der Scheiben, die dem gewählten Gestell zugeordnet werden sollen.

**Gesamt**
Gesamtstückzahl der Auftragspositionen.

**(Gewicht) Auf Gestell**
Gesamtgewicht der Positionen, die dem Gestell zugeordnet sind.

**Auf Gestell**
Gesamtstückzahl der Positionen, die dem Gestell zugeordnet sind.

## Kundenkommissionen

**Fertigung > Gestellverwaltung > Kundenkommissionen**

Mit der Kundenkommission werden weitere Details für den Versand festgelegt.

In diesem Dialog finden Sie folgende Register:
- "Kundenkommissionen - Kommission" auf Seite E-264
- "Kundenkommissionen - Abladestelle" auf Seite E-265
- "Kundenkommissionen – Zuordnung" auf Seite E-266

### Kundenkommissionen – Kommission

**Fertigung > Gestellverwaltung > Kundenkommissionen > Register Kommission**

*Abb. E-129 Kundenkommissionen – Kommission*

In diesem Register legen Sie die Standard-Kommission des Kunden fest. Dadurch können Sie im Auftrag bei der Positionserfassung die gewünschte Kommission auswählen.

⇨ Softwarereferenz, "Kommission" auf Seite C-454

### Kundenkommissionen – Abladestelle

**Fertigung > Gestellverwaltung > Kundenkommissionen > Register Abladestelle**

*Abb. E-130 Kundenkommissionen - Abladestelle*

In diesem Register geben Sie an, welche Abladestellen beim Kunden in der Regel angefahren werden.

### Kundenkommissionen – Zuordnung

**Fertigung > Gestellverwaltung > Kundenkommissionen > Register Zuordnung**

*Abb. E-131 Kundenkommissionen – Zuordnung*

In diesem Register ordnen Sie die Kommissionen den Abladestellen zu.

## Terminübersicht

**Fertigung > Terminübersicht > Terminübersicht**

In der Terminübersicht können Sie sich anzeigen lassen, was in einem bestimmten Zeitraum produziert werden muss und welche Materialien dazu benötigt werden.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menüs in der Terminübersicht" auf Seite E-267
- "Terminübersicht (Dialog)" auf Seite E-268
- "Exportieren" auf Seite E-275

### Menüs in der Terminübersicht

Über die Menüs im Dialog Terminübersicht können Sie die Standardeinstellung des Dialoges festlegen und andere Dialoge öffnen, ohne die Terminübersicht zu schließen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite E-267
- "Menü Optionen" auf Seite E-268

#### Menü Funktionen

**Fertigung > Terminübersicht > Terminübersicht > Menü Funktionen**

Im Register Tabelle können Sie über dieses Menü andere Dialoge öffnen, ohne die Terminübersicht zu schließen.

**Gruppe Dokument**
- **Historie:** Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des markierten Dokuments. Eine ausführliche Beschreibung finden Sie im Part Verkauf.
  ⇨ Verkauf, "Historie" auf Seite C-550
- **Anzeigen:** Öffnet den Dialog Dokumentenansicht zu einer Vorschau auf das Dokument. Eine ausführliche Beschreibung finden Sie im Part Verkauf.
  ⇨ Verkauf, "Reklamationen" auf Seite C-585

**Gruppe Auswahl**
- **Exportieren:** Öffnet den Dialog Export, in dem Sie auswählen können, welche Daten in eine Exportdatei geschrieben werden sollen.
  ⇨ "Exportieren" auf Seite E-275

#### Menü Optionen

**Fertigung > Terminübersicht > Terminübersicht > Menü Optionen**

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellungen werden nicht zurückgesetzt, wenn Sie den Dialog schließen. Folgende Einträge werden angezeigt:

- **Automatischer Seitenvorschub aktiv:** Im Druck wird nach jedem Datum und Auftrag ein Seitenumbruch eingefügt.
- **Archiv:** Das Archiv wird herangezogen, z. B. um Vergleichszeiträume des Vorjahrs auszuwerten.

### Terminübersicht (Dialog)

**Fertigung > Terminübersicht > Terminübersicht**

In der Terminübersicht wird angezeigt, welche Mengen in einem bestimmten Zeitraum produziert werden müssen und welche Materialien dazu benötigt werden. Die Auswertungen können gedruckt oder exportiert werden.

In diesem Dialog finden Sie folgende Register:
- "Terminübersicht - Auswahl" auf Seite E-269
- "Terminübersicht - Tabelle" auf Seite E-274

#### Terminübersicht – Auswahl

**Fertigung > Terminübersicht > Terminübersicht > Register Auswahl**

*Abb. E-132 Terminübersicht - Auswahl*

Im diesem Register legen Sie die Kriterien für die Aufträge fest, die im Register Tabelle angezeigt werden sollen.
⇨ "Terminübersicht - Tabelle" auf Seite E-274

**Quelle**
Mit der Wahl der Option legen Sie fest, wie Sie nach Aufträgen suchen wollen:
- **Nummer:** Sie können sich einen einzelnen Auftrag anzeigen lassen. Die Felder für die Eingabe der Auftragsnummer und den Auswertungszeitraum werden freigeschaltet.
- **Nummernverwalter:** Sie können sich die Aufträge eines Nummernverwalters anzeigen lassen. Das Feld für die Auswahl des Nummernverwalters wird freigeschaltet.

> **Material pro Auftrag**
> Wenn Sie einen einzelnen Auftrag auswählen, können Sie sich über den Auswertungsmodus und die Auflösungstiefe eine Liste aller Materialien erstellen, die in dem gewählten Auftrag verbraucht werden.

**Mandant**
Wenn Sie mit Mandanten arbeiten, können Sie die Auswahl auf einen bestimmten einschränken.

**AV-Bereich**
Wenn Sie mit AV-Bereichen arbeiten, können Sie die Auswahl auf einen bestimmten einschränken.

**Auswertungsmodus**
Mit der Wahl der Option legen Sie fest, wie die Aufträge ausgewertet werden sollen:
- **Produktionsbereich:** Die Felder in Bereich Produktionsbereich werden freigeschaltet, so dass Sie den gewünschten Bereich wählen können.
- **Warengruppen:** Die Felder in Bereich Auswahl Warengruppe werden freigeschaltet, so dass Sie eine WGR wählen können.
- **Produkt:** Die Felder in Bereich Auswahl Produkt werden freigeschaltet, so dass Sie ein Produkt wählen können.

**Auswertungszeitraum**
Die Felder in diesem Bereich sind nur freigeschaltet, wenn Sie im Bereich Quelle die Option Nummer gewählt haben und das Feld leer lassen. Sie können sich dann alle Aufträge eines bestimmten Zeitraums anzeigen lassen.
- **Nach Liefertermin:** Der eingegebene Zeitraum bezieht sich auf den Liefertermin.
- **Nach Produktionstermin:** Der eingegebene Zeitraum bezieht sich auf den Produktionstermin.
- **Von, bis:** Zeitraum, der ausgewertet werden soll. Wenn Sie in beiden Feldern dasselbe Datum eingeben, wird nur ein Tag ausgewertet.

**Produktionsbereiche**
Mit der Wahl der Option legen Sie fest, welchen Produktionsbereich Sie betrachten wollen. Die Felder sind nur freigeschaltet, wenn Sie den Auswertungsmodus nach Produktionsbereich gewählt haben.
- **Isolierglas:** Nur Aufträge mit ISO-Positionen werden angezeigt.
- **VSG:** Nur Aufträge mit VSG-Positionen werden angezeigt.
- **ESG:** Nur Aufträge mit ESG-Positionen werden angezeigt.
- **EFG:** Nur die Aufträge werden angezeigt, in denen Einfachglas (EFG) erfasst ist. Dies gilt auch für Einfachglas, das in ISO verarbeitet wird.
- **Zuschnitt:** Alle Aufträge werden angezeigt, in denen Glas zugeschnitten werden soll.
- **ISO Hilfsstoffe:** Alle Aufträge werden angezeigt, in denen ISO-Hilfsstoffe erfasst sind.
- **Alles:** Alle Aufträge werden angezeigt.

**Restriktionen**
Sie können die Auswertung zusätzlich auf eine der angezeigten Nebenbedingungen einschränken. Die Checkboxen Modellzuschnitt bis Bearbeitungen sind nur freigeschaltet, wenn Sie den Auswertungsmodus nach Produktionsbereich gewählt haben.

- **Modellzuschnitt:** Sie können die Auswertung auf Modelle einschränken.
  - Die Auswertung ist nicht auf Modelle eingeschränkt.
  - In der Auswertung werden nur Positionen mit Modell angezeigt.
- **Sprossenproduktion:** Sie können die Auswertung auf Sprossenkonstruktionen einschränken.
  - Die Auswertung ist nicht auf Sprossen eingeschränkt.
  - In der Auswertung werden nur Positionen mit Sprossenkonstruktionen angezeigt.
- **Stufung:** Sie können die Auswertung auf Stufungen einschränken.
  - Die Auswertung ist nicht auf Stufungen eingeschränkt.
  - In der Auswertung werden nur Positionen mit Stufungen angezeigt.
- **Bearbeitungen:** Sie können die Auswertung auf Bearbeitungen einschränken.
  - Die Auswertung ist nicht auf Bearbeitungen eingeschränkt.
  - In der Auswertung werden nur Positionen mit Bearbeitungen angezeigt.
- **Eigenfertigung:** Sie können die Auswertung auf Eigenfertigungen einschränken. Als Eigenfertigungen gelten Aufträge mit den Beschaffungsarten Zuschnitt, Produktion, Bearbeitung.
  - Die Auswertung ist nicht auf Eigenfertigungen eingeschränkt.
  - In der Auswertung werden nur Positionen mit Eigenfertigungen angezeigt.
- **Lager:** Sie können die Auswertung auf Lagerartikel einschränken.
  - Die Auswertung ist nicht auf Lagerartikel eingeschränkt.
  - In der Auswertung werden nur Positionen mit Lagerartikeln angezeigt.
- **Einkauf:** Sie können die Auswertung auf Zukaufartikel einschränken.
  - Die Auswertung ist nicht auf Zukaufartikel eingeschränkt.
  - In der Auswertung werden nur Positionen mit Zukaufartikeln angezeigt.

**Auswahl Statusbereich**
Mit der Eingrenzung auf einen Status können Sie z. B. Angebote oder Aufträge auswählen, die noch nicht an die Produktion übergeben wurden.

**Von, Bis**
In den Komboboxen werden alle Statuspunkte angezeigt, die in den Stammdaten definiert sind.

**Auswahl Warengruppe**
Mit der Wahl der Option legen Sie fest, welche Warengruppe Sie betrachten wollen. Die Felder sind nur freigeschaltet, wenn Sie den Auswertungsmodus nach Warengruppen gewählt haben.
- **WGR:** Alle Aufträge mit Produkten aus einer bestimmten Warengruppe werden betrachtet. Das Feld zur Auswahl der Warengruppe wird freigeschaltet. Sie können die WGR aus jeder der drei Ebenen der Warengruppen auswählen. Wenn Sie das Feld frei lassen, werden alle Warengruppen angezeigt.
- **WGR-Statistik:** Das Feld zur Auswahl der Statistik-Warengruppe wird freigeschaltet. Sie können eine Warengruppe (WGR), Warenobergruppe (WOG) oder Warenhauptgruppe (WHG) auswählen. Die Auswertung selbst zeigt jedoch immer nur die WHG. Wenn für Ihre Übersicht auch Warengruppen (WGR) oder Warenobergruppen (WOG) wichtig sind, können Sie zum Dialog Kapazitätsübersicht wechseln.
  ⇨ "Kapazitätsübersicht" auf Seite E-276

**Kombinations-Warengruppe**
Die Auswertung kann Kombinations-Warengruppen (Kombi-WGR) einbeziehen.
- Die Original-WGR der Produkte werden angezeigt.
- Die Kombi-WGR werden angezeigt.

> **Beispiel:**
> - Float 4 = WGR 100
> - Lochbohrung = WGR 801
> - Float 4 mit Lochbohrung (Kombination 100 und 801) = Kombi-WGR 860
>
> - Die Auswertung auf WGR-Ebene zeigt die WGR 100 und 801 an.
> - Die WGR 860 wird angezeigt.

**Auswahl Produkt**
Sie können die Auswertung auf Aufträge einschränken, in denen ein bestimmtes Produkt erfasst ist. Die Felder sind nur freigeschaltet, wenn Sie den Auswertungsmodus nach Produkt gewählt haben.
- **Produktart:** Sie können die Auswertung auf eine Produktart einschränken, z. B. auf die Produktart Artikel, um zu prüfen, welches Zubehör für die Produktion bestellt werden muss.
- **Produktgruppe:** Eine Produktgruppe können Sie nur auswählen, nachdem Sie eine Produktart gewählt haben.
- **Produkt:** Sie können die Auswertung auf ein ganz bestimmtes Produkt einschränken.

**Auflösungstiefe**
Die Auflösungstiefe bestimmt, wie detailliert die Aufträge dargestellt werden. Sie können mehrere Checkboxen markieren.
- **Pro Datum:** Die Aufträge können pro Liefertermin angezeigt werden. Diese Einstellung ist dann sinnvoll, wenn Sie sich z. B. einen Überblick über die Produkte verschaffen wollen, die in der nächsten Woche produziert werden sollen.
  - Der Liefertermin wird nicht herangezogen.
  - Die Aufträge werden nach Lieferterminen gruppiert.
- **Pro Auftrag:** Die Auswertung betrachtet jeden Auftrag einzeln. Diese Einstellung ist z. B. dann sinnvoll, wenn Sie einen Produktionsbereich ausgewählt haben.
  - Einzelne Aufträge werden nicht dargestellt.
  - Die Anzeige wird nach Aufträgen gruppiert.
- **Pro Position:** Die Auswertung betrachtet jede einzelne Position der Aufträge. Die Checkbox ist nur freigeschaltet, wenn die Checkbox pro Auftrag markiert ist. Diese Einstellung ist z. B. dann sinnvoll, wenn Sie Aufträge mit vielen Positionen und großen Stückzahlen auswerten.
  - Einzelne Positionen werden nicht dargestellt.
  - In der Anzeige werden für jeden Auftrag die Positionen angezeigt.
- **Pro Kunde:** Die Aufträge können pro Kunde angezeigt werden. Diese Einstellung ist z. B. dann sinnvoll, wenn Sie die Aufträge eines Kunden auswerten wollen.
  - Einzelne Kunden werden nicht dargestellt.
  - Die Aufträge werden nach Kunden gruppiert.
- **Zwischensumme pro ME:** Sie können Sie jeweils eine Zwischensumme anzeigen lassen.
  - Die Zwischensumme wird nicht angezeigt.
  - Pro Auftrag wird die Zwischensumme für die Mengeneinheiten angezeigt, die in den Positionen erfasst sind.

**Berechnung Gas**
- **Gasberechnung individuell:** Sie können die Anzeige der Mengeneinheit von Gas ändern. Wenn z. B. das Produkt Gas in den Produktstammdaten mit der Mengeneinheit kg angelegt ist, können Sie verbrauchte Menge in Liter anzeigen lassen.
  - Die Gasberechnung wird nicht umgerechnet.
  - Die Gasberechnung wird auf die neue Mengeneinheit umgerechnet.
- **Mengeneinheit:** Angabe der neuen Mengeneinheit. Die Menge wird nur umgerechnet, wenn die Checkbox Gasberechnung individuell aktiviert ist.

#### Terminübersicht – Tabelle

**Fertigung > Terminübersicht > Terminübersicht > Register Tabelle**

*Abb. E-133 Terminübersicht - Tabelle*

Im diesem Register werden alle Aufträge angezeigt, die den Kriterien entsprechen, die Sie im Register Auswahl festgelegt haben.
⇨ "Terminübersicht - Auswahl" auf Seite E-269

**Ergebnis**
In der Übersicht wird die Auswertung angezeigt. Die Darstellung der Spalten hängt von den gewählten Kriterien ab. Sie können sich jeden Auftrag über das Menü Funktionen > Dokument > Anzeigen in der Dokumentenansicht anzeigen lassen.

**Summen**
In der Übersicht werden die Gesamtsummen über alle Aufträge im Bereich Ergebnis angezeigt.

## Exportieren

**Fertigung > Terminübersicht > Terminübersicht > Menü Funktionen > Gruppe Auswahl > Exportieren**

*Abb. E-134 Export der Terminübersicht*

Mit der Funktion Exportieren haben Sie die Möglichkeit, die Daten für weitere Auswertungen in eine ASCII-Datei zu exportieren.

### Pfad/Dateiname

In diesem Feld tragen Sie den Pfad und den Dateinamen für die Übergabedatei ein. Schreiben Sie als Format ASC oder TXT.
Im Feld Exportiert wird nach dem Export angezeigt, wie viele Datensätze in die Datei geschrieben wurden.

### Export-Felder

In diesem Bereich sind die Felder angezeigt, aus denen Daten exportiert werden können. Das jeweilige Kennzeichen für das Darstellungsformat wird zur Information angezeigt.

## Kapazitätsübersicht

**Fertigung > Terminübersicht > Kapazitätsübersicht**

*Abb. E-135 Kapazitätsübersicht*

In diesem Dialog können Sie sich pro Liefertermin eine Vorschau auf die Kapazitäten anzeigen lassen, die für die Produktion von bestimmten Warengruppen benötigt werden.

> **Keine Verbindung zur Kapazitätsplanung**
> Die Kapazitätsübersicht steht nicht in Verbindung mit der A+W Business-Kapazitätsplanung und verarbeitet keine Rückmeldungen aus der Produktion.

### Auflösung nach

Mit der Wahl der Option legen Sie die Auflösungstiefe fest. Dazu können Sie zusätzlich einzelne Warengruppen auswählen.

- **Warenhauptgruppe:** Nur Warenhauptgruppen (WHG) werden ausgewertet.
- **Warenobergruppe:** Innerhalb der WHG wird nach Warenobergruppen (WOG) differenziert.
- **Warengruppe:** Innerhalb der WOG wird nach Warengruppen (WGR) differenziert.

### Warengruppen

**Alle**
Sie können einzelne Warengruppen auswählen. Die Auswahl ist abhängig von der gewählten Auflösung.
- Einzelne Warengruppen sollen ausgewertet werden. Die Felder zur Auswahl sind freigeschaltet. Sie können eine Anfangs- und eine Endnummer eingeben. Wenn Sie zusätzlich die Stücklisten mit auswerten, werden deren Warengruppen durch die eingestellte Auswahl nicht ausgeblendet.
- Alle Warengruppen sollen ausgewertet werden.

**Mit Stückl.**
Bei der Auswertung können die Stücklisten mit einbezogen werden.
- Die Stücklisten werden nicht ausgewertet. Das bedeutet z. B., dass das für die Produktion von ISO benötigte Float nicht berücksichtigt wird.
- Die Stücklisten werden mit ausgewertet. Diese Einstellung ist z. B. sinnvoll, wenn Sie wissen wollen, wie viele Rahmen oder Sprossen erfasst sind.

### Auftragsstatus

**Von, bis**
Sie können die Auswertung auf den Status der Aufträge eingrenzen. Um eine Vorschau zu erhalten, ist es sinnvoll, den Status bis vor Produktionsübergabe einzustellen.

### Lieferdatum

**Von, bis**
Sie können die Auswertung auf Aufträge eingrenzen, die in einem bestimmten Zeitraum geliefert werden müssen.

### Übersicht

In der Übersicht werden pro Datum alle WHG, WOG oder WGR aufgelistet, die den Auswahlkriterien entsprechen.

- **Lieferdatum:** Lieferdatum innerhalb des gewählten Zeitraums. Nach dem letzten Eintrag zum angezeigten Datum wird eine Summenzeile eingefügt, in der die Werte in blauer Schrift angezeigt sind.
- **WHG, WOG, WGR:** Nummer der Warengruppe. Die Anzeige richtet sich nach der Wahl der Auflösung.
- **Bezeichnung:** Bezeichnung der Warengruppe.
- **Anzahl:** Stückzahl aller Auftragspositionen, die zu der Warengruppe gehören.
- **Fläche:** Gesamtfläche aller Auftragspositionen, die zu der Warengruppe gehören.
- **Gewicht:** Gesamtgewicht aller Auftragspositionen, die zu der Warengruppe gehören.
- **Betrag netto:** Verkaufswert aller Auftragspositionen, die zu der Warengruppe gehören.

Im unteren Bereich der Übersicht werden die Gesamtsummen der angezeigten Warengruppe angezeigt.

## Fertigungsvorschau

**Fertigung > Terminübersicht > Fertigungsvorschau**

Pro Liefertermin können Sie zu den Produktarten Isolierglas, Einfachglas, ESG und VSG die Summe der Glasflächen anzeigen lassen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Fertigungsvorschau (Dialog)" auf Seite E-279
- "Definition Vorschauspalten" auf Seite E-280
- "GA-Ausschluss bei Fertigungsvorschau" auf Seite E-281

### Menü Optionen

**Fertigung > Terminübersicht > Fertigungsvorschau**

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Fertigungsvorschau zu schließen. Folgende Einträge werden angezeigt:

**Gruppe Anzeige**
- **Spaltendefinition:** Öffnet den Dialog Definition Vorschauspalten, in dem Sie festlegen können, welche Spalten angezeigt werden.
  ⇨ "Definition Vorschauspalten" auf Seite E-280
- **Geschäftsarten ausblenden:** Öffnet den Dialog GA-Ausschluss, in dem Sie festlegen können, welche Geschäftsarten nicht angezeigt werden sollen.
  ⇨ "GA-Ausschluss bei Fertigungsvorschau" auf Seite E-281

**Gruppe Termin**
Über dieses Menü können Sie auswählen, auf welchen Termin sich die Vorschau beziehen soll:
- **Nach Liefertermin:** Die Vorschau bezieht sich auf den Liefertermin.
- **Nach Produktionsende:** Die Vorschau bezieht sich auf das Produktionsende.

### Fertigungsvorschau (Dialog)

**Fertigung > Terminübersicht > Fertigungsvorschau**

*Abb. E-136 Fertigungsvorschau*

In diesem Dialog können Sie sich eine Vorschau auf die Mengen einzelner Produkte oder Produktarten anzeigen lassen. In den verschiedenen Registern werden die Vorschaudaten für die jeweilige Glasart angezeigt.

Die Spalten können pro Arbeitsplatz individuell eingestellt werden.
⇨ Tutorial, "Fertigungsvorschau" auf Seite E-161

Die Fertigungsvorschau analysiert alle Aufträge nach quantitativen Gesichtspunkten und informiert über die zukünftige Auslastung nach Produktarten und Produktgruppen. Für die Auswertung werden alle aktuellen Aufträge mit Versandtag größer gleich dem aktuellen Tagesdatum herangezogen. Die Auswertungskriterien sind jeweils eine Kombination von Produktart und Produktgruppe.

Das Auswertungsergebnis wird jeweils in einer Datenbanktabelle gespeichert und beim Aufruf des Dialogs sofort angezeigt. Die Anzeige kann manuell aktualisiert werden. Das letzte Aktualisierungsdatum wird mit Stunde und Minute angezeigt.

### Definition Vorschauspalten

**Fertigung > Terminübersicht > Fertigungsvorschau > Menü Optionen > Gruppe Anzeige > Spaltendefinition**

*Abb. E-137 Spaltendefinition für die Fertigungsvorschau*

In diesem Dialog legen Sie fest, welche Einstellungen firmenübergreifend gelten sollen. Sie brauchen Administratorrechte, um diesen Dialog zu öffnen.

#### Spalten

**Nr.** Der fortlaufende Zähler wird bei der Spalteneingabe gesetzt.

**Bezeichnung** Der Titel für die Spaltenüberschrift ist frei wählbar, z. B. Isolierglas.

**Bezeichnung 2** Der Titel für die Spaltenüberschrift ist frei wählbar, z. B. die Mengeneinheit.

**Typ HP** Die Typauswahl auf Basis des Hauptprodukts:
- 1 = Produktart
- 2 = Produktgruppe

**HP** Das Hauptprodukt entspricht der Schlüsselnummer der in den Artikelstammdaten hinterlegten Produktart oder Produktgruppe.

**Typ 0** Die Typauswahl auf Basis des Hauptprodukts:
- 1 = Produktart
- 2 = Produktgruppe,

**Nr. 0** Die Schlüsselnummer für die Produktart oder die Produktgruppe je nach Typ.

**ST/QM** Darstellung der Mengen (Maßeinheit)
- 1 = Stück
- 2 = Qm

**GR.-Klasse** Die Größenklassen werden durch Von-bis-Werte festgelegt, die sich auf die Maßeinheit beziehen.

### GA-Ausschluss bei Fertigungsvorschau

**Produktion > Fertigungsvorschau > Menü Optionen > Gruppe Anzeige > Geschäftsarten ausblenden**

*Abb. E-138 Ausschluss von Geschäftsarten*

In diesem Dialog legen Sie fest, welche Geschäftsarten nicht angezeigt werden sollen. Sie brauchen Administratorrechte, um diesen Dialog zu öffnen.
Zur Wahl stehen alle Geschäftsarten, die in den Stammdaten > Auftrag hinterlegt sind.

## Zollverwaltung

**Fertigung > Zollverwaltung**

In diesem Bereich können Sie verschiedene Zoll-Listen für den Warenexport erstellen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Zollverwaltungsliste" auf Seite E-282
- "Listennummer zurücksetzen" auf Seite E-286
- "Produktgruppe mit Positionsmenge" auf Seite E-286
- "Zoll-Export" auf Seite E-287
- "Export Artikelstammdaten" auf Seite E-289

### Zollverwaltungsliste

**Fertigung > Zollverwaltung > Zollvw.-Liste**

Für die Zollpapiere können Sie verschiedene Ladelisten erstellen.
In diesem Dialog finden Sie folgende Register:
- "Ladeliste - Nummernverwalter" auf Seite E-283
- "Ladeliste - Zollverwaltungslisten" auf Seite E-285

#### Menü Funktionen

In diesem Menü finden Sie folgende Einträge:
- **Listennummer zurücksetzen:** Öffnet den gleichnamigen Dialog, in dem Sie die zuletzt verwendete Nummer der Zoll-Liste zurücksetzen können.
  ⇨ "Listennummer zurücksetzen" auf Seite E-286
- **Produktgruppe ohne Stkl.-Auflösung:** Öffnet den Dialog Produktgruppe mit Positionsmengen, in dem Sie bestimmte Produkte ausschließen können.
  ⇨ "Produktgruppe mit Positionsmenge" auf Seite E-286

### Ladeliste - Nummernverwalter

**Fertigung > Zollverwaltung > Zollvw.-Liste > Register Nummernverwalter**

*Abb. E-139 Ladeliste - Nummernverwalter*

In diesem Dialog können Sie den Nummernverwalter auswählen, in dem Sie die Aufträge für die Zollverwaltungsliste gesammelt haben.

> **Voraussetzungen**
> Sie können Zollpapiere nur drucken, wenn den Produkten und/oder Warengruppen Zolltarifnummern zugeordnet sind.

#### Identifikation

**Mandant**
Wenn Sie mit unterschiedlichen Mandanten arbeiten, werden diese zur Auswahl angeboten.

**Mitarbeiter**
Name des Mitarbeiters, der sich in A+W Business angemeldet hat.

**Nummernverwalter**
Auswahl des Nummernverwalters, in dem Sie die Aufträge für den Warenexport gesammelt haben.

#### Eingabe

**Zollübergang von, Zollübergang nach**
Auswahl der Grenzübergänge, die der Lkw benutzen wird. Zur Auswahl werden alle Grenzübergänge angeboten, die Sie in den Stammdaten hinterlegt haben. Eine Beschreibung finden Sie im Part Stammdaten.
⇨ Stammdaten, "Zolltouren" auf Seite B-860

**NV Proforma Rechnung**
Auswahl des Nummernverwalters, in dem die Proforma-Rechnungen gesammelt werden.

**Gewichtsfaktor**
Angabe des Gewichtsfaktors, wenn das Bruttogewicht als Bemessungsgrundlage für die Berechnung des Zolls herangezogen wird.

**Liefertermin**
Angabe des Liefertermins, der in die Zollpapiere gedruckt werden soll.

#### Übersicht

In der Übersicht werden alle Aufträge aus dem Nummernverwalter aufgelistet.
- **Auftrag:** Auftragsnummer.
- **Nummer Kunde/Lief., Kunde/Lieferant:** Nummer und Name des Kunden oder Lieferanten.
- **Status:** Auftragsstatus.
- **Lieferschein:** Nummer des Lieferscheins.
- **Datum Lieferung:** Lieferdatum aus dem Auftrag.
- **Stückzahl gesamt:** Stückzahl aller Positionen pro Auftrag.
- **Gewicht gesamt:** Gewicht aller Positionen pro Auftrag.

### Ladeliste – Zollverwaltungslisten

**Fertigung > Zollverwaltung > Zollvw.-Liste > Register Zollverwaltungslisten**

*Abb. E-140 Ladeliste - Zollverwaltungslisten*

In diesem Register können Sie sich die Zollverwaltungslisten anzeigen und drucken lassen.

#### Eingabe

**Zollverwaltungsliste Nr.:**
In diesem Feld wird die Nummer der Zollverwaltungsliste angezeigt. Die Nummer wird automatisch von System vergeben, wenn eine neue Liste erstellt wird. Im Auswahlmodus können Sie sich jede Liste anzeigen lassen, die zuvor erstellt wurde.
Mit der Wahl der Option legen Sie die Art der Liste fest:
- **Zollverwaltungsliste anzeigen:** Mit dieser Option können Sie die erfassten Zollverwaltungslisten anzeigen.
- **Zollverwaltungslistennachweis:** Mit dieser Option können Sie die erfassten Artikel einer Zollverwaltungsliste anzeigen lassen.

### Listennummer zurücksetzen

**Fertigung > Zollverwaltung > Zollvw.-Liste > Menü Funktionen > Listennummer zurücksetzen**

*Abb. E-141 Listennummer zurücksetzen*

In diesem Dialog können Sie die Nummer der Zollverwaltungsliste zurücksetzen.

### Produktgruppe mit Positionsmenge

**Fertigung > Zollverwaltung > Zollvw.-Liste > Menü Funktionen > Produktgruppe ohne Stkl.-Auflösung**

*Abb. E-142 Produktgruppe ohne Stücklisten-Auflösung*

In diesem Dialog können Sie die Produktgruppe auswählen, bei der die Stücklistenmenge nicht berücksichtigt werden soll. Damit wird bei Produktgruppen mit der Produktart Artikel nur die Menge der Position in die Zollverwaltungsliste übernommen.

## Zoll-Export

**Fertigung > Zollverwaltung > Zollexport**

### Menü Funktionen

**Fertigung > Zollverwaltung > Zollexport > Menü Funktionen**

Über dieses Menü können Sie den Dialog öffnen, in dem Sie den Pfad für eine Schnittstellendatei für Stammdaten erstellen können.
⇨ "Export Artikelstammdaten" auf Seite E-289

### Zoll-Export (Dialog)

**Fertigung > Zollverwaltung > Zollexport**

*Abb. E-143 Zoll-Export*

In diesem Dialog können Sie eine Schnittstellendatei schreiben, die von Zoll-Programmen importiert werden kann.

#### Modus

Die Datei kann für verschiedene Schnittstellen angefertigt werden. In der Kombobox sind alle Schnittstellen aufgeführt, für die eine Exportdatei geschrieben werden kann.

#### Identifikation

**Nummernverwalter**
Nur die Aufträge werden in der Übersicht angezeigt, die dem eingestellten Auftragsstatus entsprechen.

**Status von, bis**
Sie können die Anzeige der Aufträge auf einen Status eingrenzen, z. B. auf Lieferschein oder Rechnung gedruckt.

#### Pfad der Ausgabedatei

Angabe des Orts, an dem die Schnittstellendateien gespeichert werden sollen.

#### Mandant

Wenn Sie mit Mandaten arbeiten, können Sie die Schnittstellendatei für jeden Mandanten einzeln erstellen. In diesem Feld tragen Sie den Namen des Mandanten ein.

#### Format der Ausgabedatei

Mit der Wahl der Option legen Sie das Dateiformat fest:
- **ANSI:** Diese Einstellung erzeugt eine reine ASCII-Datei nach dem ANSI-Standard.
- **OEM:** Diese Einstellung erzeugt eine Datei nach dem Format anderer Hersteller, das dem Standard entspricht.

#### Dokumente

In der Übersicht werden alle Aufträge angezeigt, die den Auswahlkriterien entsprechen.
- **Auftragsnummer:** Nummer des Auftrags.
- **Kundennummer, Kunde:** Nummer und Name des Kunden aus dem Auftrag.
- **PLZ, Ort:** Geschäftsort des Kunden.
- **Land:** Land, in dem der Kunde seinen Geschäftssitz hat.
- **Nettobetrag, Nettobetrag FW:** Nettobetrag des Auftrags in Eigen- und in Fremdwährung.
- **Datum Rechnung:** Datum der Rechnung.
- **Status:** Status des Auftrags.
- **Produktnummer:** Nummer des Produkts aus den Stammdaten.
- **Anzahl Produkte:** Menge der Produkte.
- **ISO-Glas, VSG-Glas:** Stückzahl ISO, VSG.

## Export Artikelstammdaten

**Fertigung > Zollverwaltung > Zoll-Export > Menü Funktionen > Stammdaten-Export**

*Abb. E-144 Export von Artikelstammdaten*

In diesem Dialog können Sie die Stammdaten der Produkte oder der Kundenprodukte in eine Schnittstellendatei schreiben. Exportiert werden nur die Daten der Aufträge, die im Dialog Zoll-Export angezeigt werden.

### Pfad Ausgabedatei

In diesem Feld tragen Sie den Pfad ein, unter dem die Schnittstellendatei gespeichert werden soll.

### Export

Mit der Wahl der Option legen Sie fest, wessen Stammdaten exportiert werden sollen.
- **Artikel:** Die Stammdaten der Artikel werden exportiert.
- **Kunden:** Die Stammdaten des Kunden werden exportiert.

## Angebotsoptimierung

**Fertigung > Angebotsoptimierung**

In diesem Bereich können Sie Ihre Angebote probehalber an die Produktion übergeben, um z. B. festzustellen, wie viele Bandmaße für den Zuschnitt benötigt werden. Dies kann bei besonderen Gläsern zur Preisgestaltung berücksichtigt werden.

Die Dialoge sind bereits an anderer Stelle ausführlich beschrieben.

- **Nummernverwalter:** Der Dialog Nummernverwalter ist im Part Verkauf beschreiben.
  ⇨ Verkauf, "Nummernverwalter" auf Seite C-624
- **Übergabe Produktion:** Die Funktion dieses Dialogs entspricht der Übergabe von Aufträgen. Im Unterschied zu den Aufträgen sind die übergebenen Angebote jedoch nicht für die Produktion freigegeben.
  ⇨ "Übergabe Produktion" auf Seite E-170

## Versandsteuerung

**Fertigung > Versandsteuerung**

In diesem Bereich können Sie den Versand organisieren, der nicht über den eigenen Fuhrpark abgewickelt wird. Sie können für Ihre Spediteure verschiedene Versandpapiere und Ladelisten erstellen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Versand (Spedition)" auf Seite E-290
- "Versandaufträge löschen" auf Seite E-297
- "Gestell-Packliste" auf Seite E-298
- "Teillieferung" auf Seite E-299
- "Ladelisten" auf Seite E-301

### Versand (Spedition)

**Fertigung > Versandsteuerung > Versand**

Im Dialog Versand ordnen Sie Aufträge, Gestelle und Lagerorte einander zu.

In diesem Dialog finden Sie folgende Register:
- "Versandsteuerung - Sammeln" auf Seite E-292
- "Versandsteuerung - Versandinfo" auf Seite E-294
- "Versandsteuerung – Verpackung + Transport" auf Seite E-295

#### Menü Funktionen

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Versandsteuerung zu schließen.

**Gruppe Versand**
- **Aufträge gruppieren:** Aufträge können zu Gruppen zusammengefasst werden.
- **Versanddatei erstellen:** Speichert die Versandliste als Datei.
- **Auflösen von Versandaufträgen:** Öffnet den Dialog Versandaufträge löschen, in dem Sie Aufträge aus einem Versandauftrag herausnehmen können.
  ⇨ "Versandaufträge löschen" auf Seite E-297

**Gruppe Drucken**
Über die Schaltflächen öffnen Sie den Dialog Formular-/Etikettendruck im jeweiligen Druckmodus. Folgende Druckmodi stehen zur Wahl:
- Versandetiketten
- Containerliste
- Ladeliste
- Packliste

Eine ausführliche Beschreibung finden Sie im Part Verkauf.
⇨ Verkauf, "Formular-/Etikettendruck" auf Seite C-633

### Versandsteuerung – Sammeln

**Fertigung > Versandsteuerung > Versand**

*Abb. E-145 Versand – Sammeln*

In diesem Register stellen Sie die Aufträge für eine Ladeliste zusammen. Die Aufträge müssen alle für denselben Kunden ausgestellt sein.

> **Auftrag aus der Liste entfernen**
> Wenn Sie versehentlich einen (falschen) Auftrag ausgewählt haben, können Sie diesen über Menü Funktionen > Auflösen von Versandaufträgen aus der Liste entfernen.
>
> ⇨ "Versandaufträge löschen" auf Seite E-297

#### Selektion nach

Mit der Wahl der Option legen Sie fest, nach welchem Kriterium Sie die Aufträge zusammenstellen wollen. Die gleichnamigen Felder werden freigeschaltet.

- **Ident-/Gestellnummer:** Angabe der Identnummer oder der Nummer des Gestells, auf dem die Auftragspositionen abgestellt sind.
- **Auftragsnummer:** Angabe der Auftragsnummer des fertig meldeten Auftrags ein.
- **Lagerort:** Auswahl des Lagerorts, an dem die gefertigten Auftragspositionen abgestellt sind.

#### Ziel

- **Nummernverwalter:** Die gesammelten Aufträge werden automatisch in einen Nummernverwalter kopiert. Wenn Sie einen neuen Namen eintragen, wird der Nummernverwalter angelegt.
- **AV-Bereich:** Wenn Sie mit AV-Bereichen arbeiten, können Sie in diesem Feld den Bereich auswählen, dem die Aufträge zugeordnet sind.

#### Aufträge

In der Übersicht werden alle Aufträge angezeigt, die Sie zusammengestellt haben.
- **Auftrag:** Nummer des Auftrags
- **Pos.:** Nummer der Auftragsposition
- **Menge:** Stückzahl der Position
- **Gewicht:** Gewicht der Position
- **Breite, Höhe:** Breite und Höhe der Scheiben
- **Bezeichnung:** Bezeichnung des Produkts
- **Ident/Gestell:** ID oder Gestellnummer

### Versandsteuerung – Versandinfo

**Fertigung > Versandsteuerung > Versand > Register Versandinfo**

*Abb. E-146 Versand - Versandinfo*

In diesem Register geben Sie die Details zu der Ladeliste an, für die Sie die Aufträge zusammengestellt haben.

#### Versandangaben

- **Ladeliste:** Nummer der Ladeliste.
- **LKW:** Sie können einen LKW aus der Liste wählen.
- **Fahrer:** Sie können einen Fahrer aus der Liste wählen.

#### Versandtext

Sie können einen Text aus den hinterlegten Texten auswählen oder einen eigenen Text einfügen. Der Text wird auf der Ladeliste gedruckt.
- **Nummer:** Sie können das Textkennzeichen eingeben oder den gewünschten Text suchen. Den gewählten Text können Sie im Anzeigefeld modifizieren.

### Versandsteuerung – Verpackung + Transport

**Fertigung > Versandsteuerung > Versand > Register Verpackung + Transport**

*Abb. E-147 Versand - Verpackung + Transport*

In diesem Register können Sie einen Zuschlag für die Verpackung und/oder den Transport hinzufügen.

#### Zuschlag

- **Produkt:** Sie können einen Zuschlag auswählen, der allen oder einzelnen Aufträgen in der Übersicht hinzugefügt wird. Über die Suche werden Ihnen alle Produkte der Produktart Leistungen/Zuschläge zur Auswahl angeboten.
- **Menge:** Angabe, wie oft der gewählte Zuschlag berechnet werden soll.
- **Preis/PE, (ME):** Angabe des Betrags pro Mengeneinheit und Auswahl der Mengeneinheit, auf die sich der Betrag bezieht.
- **[Einfügen]:** Mit dieser Schaltfläche übernehmen Sie den Zuschlag in die markierten Aufträge. Wenn kein Auftrag markiert ist, wird der Zuschlag nicht berechnet.

#### Preisdarstellung

Die Zuschläge können einzeln ausgewiesen werden und/oder der Stückliste hinzugefügt werden.

- **Explizit:** Sie können die Art der Preisdarstellung wählen.
  - Der Zuschlag wird in die Auftragspositionen mit eingerechnet (implizit).
  - Der Zuschlag wird als eigene Position ausgewiesen.

#### Einfügemodus

Mit der Wahl der Option legen Sie fest, wo der Zuschlag eingefügt werden soll. Wenn der Zuschlag z. B. für Kantenschutz erhoben wird, ist es sinnvoll, ihn in der Stückliste einzufügen, wenn er für eine Transportversicherung erhoben wird, ist er als eigene Position sinnvoll.
- **In Stückliste:** Der Zuschlag wird in die Stückliste eingefügt. Bei einer impliziten Preisdarstellung wird er in die Komponenten der Stückliste eingerechnet.
- **Als Position:** Der Zuschlag wird im Auftrag als eigene Position eingefügt. Für die Preisdarstellung sollte dann explizit gewählt sein.

#### Versandaufträge

**[Alle], [Keine]:** Mit diesen Schaltflächen markieren Sie alle Aufträge, für die der Zuschlag gelten soll, oder Sie entfernen die Markierung von allen Aufträgen. Wenn kein Auftrag markiert ist, wird der Zuschlag nicht berechnet.

In der Übersicht sind alle Aufträge dargestellt, die Sie im Register Sammeln eingefügt haben.
- **Versand-Nr:** Auftragsnummer für den Versand
- **Kunde/Ort:** Name und Geschäftssitz des Kunden aus dem Auftrag
- **Gewicht:** Gesamtgewicht aller Positionen
- **Netto Wert:** Gesamtwert des Auftrags

### Versandaufträge löschen

**Fertigung > Versandsteuerung > Versand > Menü Funktionen > Auflösen von Versandaufträgen**

*Abb. E-148 Versandaufträge löschen*

In diesem Dialog können Sie einzelne Aufträge aus der Aufstellung im Dialog Versand löschen.

#### Dokument

**Versand-Nr.**
Angabe der Auftragsnummer, aus dem Sie einen Auftrag löschen wollen. Der Name und der Ort des Kunden werden automatisch angezeigt.

#### Zu löschende Dokumente

In der Übersicht sind alle Dokumente aufgeführt, die zu der jeweiligen Versandnummer gehören.
- **Versand-Nr.:** Nummer des Versandauftrags
- **Container:** Nummer des Packmittels
- **Kundenauftrag:** Nummer des Auftrags aus A+W Business
- **Status:** Auftragsstatus

### Gestell-Packliste

**Fertigung > Versandsteuerung > Gestell-Packliste**

#### Menü Funktionen

**Fertigung > Versandsteuerung > Gestell-Packliste > Menü Funktionen**

**Tabelle leeren:** Über dieses Menü löschen Sie alle Einträge aus der Tabellenübersicht.

#### Gestell-Packliste (Dialog)

**Fertigung > Versandsteuerung > Gestell-Packliste**

*Abb. E-149 Gestell-Packliste*

In diesem Dialog prüfen Sie sich die Beladung der Gestelle.

**Selektion**
Mit der Wahl der Option legen Sie die Darstellung in der Übersicht fest.
- **Alle nicht gedruckten:** Nur die Gestelle werden angezeigt, die noch nicht ausgedruckt wurden.
- **Gestell:** Die Beladung eines einzelnen Gestells wird angezeigt.

#### Tabelle

In der Übersicht sind die Gestelle je nach der gewählten Einstellung aufgeführt.
- **Gestell:** Gestellnummer.
- **Einheit:** Einheit, wenn Auftragsposition aus mehreren Einheiten besteht.
- **Auftrag:** Auftragsnummer.
- **Pos.:** Nummer der Position im Auftrag.
- **Menge:** Stückzahl der Position.
- **Breite, Höhe:** Breite und Höhe der Position.
- **Produkt:** Produktnummer der Position.

### Teillieferung

**Fertigung > Versandsteuerung > Teillieferung**

*Abb. E-150 Übersicht - Teillieferungen*

In diesem Dialog können Sie sich anzeigen lassen, welche Aufträge in einem Nummernverwalter noch offene Mengen ausweisen.

#### Identifikation

- **Mandant:** Wenn Sie mit unterschiedlichen Mandanten arbeiten, werden diese zur Auswahl angeboten.
- **Bereich:** Wenn in der Produktion mit verschiedenen Bereichen gearbeitet wird, können Sie denjenigen auswählen, dem die Aufträge zugeordnet sind.
- **Mitarbeiter:** Name des Mitarbeiters, der sich in A+W Business angemeldet hat.
- **Nummernverwalter:** Wenn Sie einen Nummernverwalter ausgewählt haben, werden alle Aufträge aufgelistet, die in diesem Nummernverwalter stehen.

#### Ausgabe auf

Mit der Wahl der Option legen Sie die Ausgabe der Liste fest:
- **Drucker:** Die Liste wird an den Drucker gesendet.
- **Bildschirm:** Die Liste wird auf dem Bildschirm dargestellt.

#### Übersicht

In der Übersicht werden alle Aufträge im gewählten Nummernverwalter angezeigt.
- **Dokument:** Auftragsnummer.
- **Pos:** Positionsnummer aus dem Auftrag.
- **Datum Lieferung:** Lieferdatum.
- **Breite, Höhe:** Breite und Höhe der Position.
- **Produkt Kunde:** Bei Kundenprodukten wird die Referenznummer angezeigt.
- **Produkt Nummer, Produkt Bezeichnung:** Nummer und Bezeichnung des Produkts in A+W Business.
- **Bestelltext/Kundenpos.:** Bestelltext oder Kundenposition aus dem Auftrag.
- **Menge original, Menge geliefert, Menge offen:** Gesamtmenge der Auftragsposition, davon gelieferte bzw. offene Menge.
- **Status Nummer, Status Bezeichnung:** Auftragsstatus.
- **Nummer Kunde, Name Kunde:** Nummer und Name des Kunden.
