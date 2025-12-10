---
title: "D-AWProduction-HB_7"
source: "D-AWProduction-HB_7.pdf"
tags: ["A+W Production", "Kapazitätsplanung", "Formeleditor", "Software-Referenz", "Produktionsmonitor", "Einlastung", "Schichtplanung", "Maschinensteuerung", "Umlastung", "Tutorial"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a detailed software reference manual for A+W Production, focusing on capacity planning (Kapazitätsplanung) and the formula editor (Formeleditor). It provides step-by-step instructions and descriptions for various modules, including production monitoring, filtering, shift management, and machine configuration."
long_description: "This comprehensive technical document serves as a software reference for the A+W Production system, specifically covering the modules for Capacity Planning (Kapazitätsplanung) and the Formula Editor (Formeleditor). The manual is structured to guide users through the software's functionalities, from basic operations to advanced configurations. It details processes such as \"Einlastung\" (loading/scheduling), managing custom filters in the production monitor, creating and adjusting machine shifts, and configuring machine properties like bottleneck status and display types. The guide explains how to handle work plans, view details and overviews, and perform \"Umlastung\" (rescheduling) of production tasks. It also covers the management of campaigns and reservations, allowing users to allocate machine capacity for specific jobs or customers. A significant portion is dedicated to the setup of master data for time calculations, including standard times (Vorgabezeiten), transition times (Übergangszeiten), and shift schedules. The document concludes with a deep dive into the A+W Formula Editor, explaining its syntax, elements, and application in creating complex rules and conditions for production and data handling. It is intended for system administrators and advanced users responsible for configuring and maintaining the A+W Production environment."
---

# A+W Production Kapazitätsplanung - Softwarereferenz

---
## Filter – Eigene Filter

*Pfad: Anzeigen > Produktionsmonitor > [Ansicht filtern] > Eigene Filter*

[Image: Dialog "Bitte wählen Sie einen Auftrag/Lauf aus – Eigene Filter"]
*Abb. E-87 Bitte wählen Sie einen Auftrag/Lauf aus – Eigene Filter*

In diesem Register werden die selbst definierten Filter angezeigt.

- **[Neu]** Öffnet den Dialog Neuen Filter erstellen, in dem Sie eigene Filter definieren können.
- **[OK]** Speichert die Daten.
- **[Verwerfen]** Schließt den Dialog, ohne die Daten zu speichern.

## Neuen Filter erstellen

*Pfad: Anzeigen > Produktionsmonitor > [Ansicht filtern] > Register Eigene Filter > [Neu]*

[Image: Dialog "Neuen Filter erstellen"]
*Abb. E-88 Neuen Filter erstellen*

In diesem Dialog können Sie eigene Filter für die Suche im Produktionsmonitor erstellen. Sie erstellen die Filter in der Datenbanksprache SQL.

> **i Eigene Filter erstellen**
> Bitte wenden Sie sich an den Kundenservice der A+W Software GmbH, wenn Sie spezielle Filter zur Suche im Produktionsmonitor brauchen.

- **Name**: Name für den Filter.
- **Beschreibung**: Beschreibung für den Filter.
- **SQL**: Definition des Filters in SQL.
- **[OK]**: Speichert die Daten.
- **[Verwerfen]**: Schließt den Dialog, ohne die Daten zu speichern.

## Maschine (Name)

*Pfad: Anzeigen > Produktionsmonitor > Maschine > Kontextmenü > Eigenschaften*

[Image: Dialog "Maschine (Name)"]
*Abb. E-89 Maschine (Name)*

In diesem Dialog ändern Sie die Eigenschaften der Maschine im Produktionsmonitor.

- **[Kategorien]** Sortiert die Elemente nach Kategorien.
- **[Alphabetisch]** Sortiert die Elemente alphabetisch.
- **[Eigenschaften]** Zur Zeit nicht genutzt.

### Eigenschaften der Maschine

- **ID:** Identifikationsnummer der Maschine.
- **Erfassungsstelle:** Identifikationsnummer der Erfassungsstelle.
- **Name:** Name der Maschine.
- **Engpass:** Auswahl, ob die Maschine ein Engpassbetriebsmittel ist. Engpassbetriebsmittel werden im Produktionsmonitor in der Liste der Maschinen in roter Schrift angezeigt.
- **Anzeigeart:** Auswahl, in welcher Einheit die Schichtinfo den Status Fertig anzeigt. Zur Auswahl stehen:
    - Prozent
    - Menge
    - Fläche
    - Gewicht
    - Laufmeter
    - Bearbeitung
- **Gruppe:** Maschinengruppe, zu der die Maschine gehört.
- **Leistung pro Anzeigeart ändern:** Angabe der Einheit, in der die Leistung der Maschine angezeigt wird.

### Misc

- **Logische Maschinen anzeigen:** Auswahl, ob im Produktionsmonitor zur markierten Maschine auch die logischen Maschinen angezeigt werden, z. B. zur Maschine Drilling (Bohrmaschine).

- **[OK]** Speichert die Daten.
- **[Verwerfen]** Schließt den Dialog, ohne die Daten zu speichern.

## Schichten für Maschine anpassen

*Pfad: Anzeigen > Produktionsmonitor > Maschine > Kontextmenü > Schichteigenschaften*

[Image: Dialog "Schichten für Maschine anpassen"]
*Abb. E-90 Schichten für Maschine anpassen*

In diesem Dialog können Sie die Arbeitsschichten für die jeweilige Maschine bezogen auf Wochentage anpassen.

- **Wochentage**: Angabe, für welche Wochentage die Änderung der Arbeitsschicht gilt.
    - ☐ Die Arbeitsschicht wird für diesen Wochentag nicht geändert.
    - ☑ Die Arbeitsschicht wird für diesen Wochentag geändert.
- **Schichtnummer**: Angabe der Schichtnummer.
- **Kapazität**: Angabe der Schichtkapazität an den markierten Wochentagen.
- **[OK]** Speichert die Daten.
- **[Verwerfen]** Schließt den Dialog, ohne die Daten zu speichern.

## Schichteigenschaften

*Pfad: Anzeigen > Produktionsmonitor > Anzeige der Schichten > Kontextmenü > Schichteigenschaften*

[Image: Dialog "Schichteigenschaften"]
*Abb. E-91 Schichteigenschaften*

In diesem Dialog können Sie die Eigenschaften einer Arbeitsschicht bezogen auf eine Maschine anzeigen lassen.

- **[Kategorien]** Sortiert die Elemente nach Kategorien.
- **[Alphabetisch]** Sortiert die Elemente alphabetisch.
- **[Eigenschaften]** Zur Zeit nicht genutzt.

### Eigenschaften der Schicht

- **Datum:** Datum der markierten Arbeitsschicht.
- **Schichtnummer:** Nummer der markierten Arbeitsschicht.
- **Start, Ende:** Start- und Endezeit aus den Stammdaten der markierten Arbeitsschicht.
- **Kapazität:** Zeit in Stunden, die in der Arbeitsschicht zur Verfügung stehen. Sie können die Kapazität einer Arbeitsschicht ändern. Die verkleinerte Kapazität wird im Produktionsmonitor schraffiert angezeigt.
- **Kommentar:** Bemerkung zu den manuellen Änderungen der aktuellen Arbeitsschicht.
- **Status:** Status einer Arbeitsschicht. Im Auswahlmenü wählen Sie unter folgenden Optionen:
    - **Aktiv:** Die Arbeitsschicht ist für die jeweilige Maschine verfügbar.
    - **Deaktiviert:** Die Arbeitsschicht ist für die jeweilige Maschine nicht verfügbar. Die Schicht wird im Produktionsmonitor mit einem X markiert. (⇨ "Anzeige der Arbeitsschichten" auf Seite E-563)
    - **Aktiv für Eilaufträge:** Die Arbeitsschicht steht für die jeweilige Maschine ausschließlich für Eilaufträge zur Verfügung. Die Arbeitsschicht wird im Produktionsmonitor mit einem ! markiert.
- **Engpass:** Auswahl, ob die Arbeitsschicht ein Engpass ist. Ein Engpassbetriebsmittel kann nicht über seine Kapazität hinaus bebucht werden.

- **[OK]** Speichert die Daten.
- **[Verwerfen]** Schließt den Dialog, ohne die Daten zu speichern.

## Reservierungsanzeige

*Pfad: Anzeigen > Produktionsmonitor > Schicht > Kontextmenü > Reservierung anzeigen*

[Image: Dialog "Übersicht - Reservierungen"]
*Abb. E-92 Übersicht - Reservierungen*

In diesem Dialog werden alle Reservierungen der aktuellen Schicht angezeigt. Abgelaufene oder abgesagte Reservierungen sollten Sie löschen.

⇨ Tutorial, "So löschen Sie eine Reservierung" auf Seite E-472

## Arbeitsplan aus Produktionsmonitor

*Pfad: Anzeigen > Produktionsmonitor > Schicht > Kontextmenü > Arbeitsplan*

In diesem Dialog können Sie sich einen Überblick zu einer bestimmten Arbeitsschicht verschaffen.

Der Dialog enthält folgende Register:
- "Arbeitsplan - Details" auf Seite E-578
- "Arbeitsplan - Übersicht" auf Seite E-579

### Kontextmenü

Über das Kontextmenü zu den Läufen können Sie andere Dialoge öffnen, um sich Details zum gewählten Lauf anzeigen zu lassen.

Über das Kontextmenü zu den Spalten können Sie folgende Einträge wählen:

| Eintrag | Funktion |
| :--- | :--- |
| **Umsortieren** | Spalte aufsteigend oder absteigend sortieren. Wirkt sich auf die ersten drei Spalten aus. |
| **Formatieren** | Format oder Einheit auswählen, z. B. Datumsformate oder Längen-Einheiten. |
| **Einfügen** | Öffnet die Auswahl für Spalten, die in den verschiedenen Kategorien eingefügt werden können. |
| **Entfernen** | Löscht die markierte Spalte. |
| **Definition anzeigen** | Öffnet den Dialog Spaltendefinition, in dem Details zur jeweiligen Spalte angezeigt werden. |

### Schaltflächen

Die Funktionen der Schaltflächen sind ausführlich im Part Grobplanung beschrieben.

## Arbeitsplan – Details

*Pfad: Anzeigen > Produktionsmonitor > Schicht > Kontextmenü > Arbeitsplan > Details*

[Image: Dialog "Arbeitsplan: Selektion aus Produktionsmonitor – Details"]
*Abb. E-93 Arbeitsplan: Selektion aus Produktionsmonitor – Details*

In diesem Register können Sie sich einen Überblick zu den geplanten Läufen in einer bestimmten Arbeitsschicht verschaffen. Sie können für die markierten Einträge Glasarten prüfen, Details prüfen und Läufe starten. Diese Funktionen sind ausführlich im Part Grobplanung beschrieben.

### Spalten

Über das Kontextmenü können Sie die Spalten auswählen, um sich die gewünschten Informationen anzeigen zu lassen, z. B.:
- **Lauf:** Angabe des Laufs.
- **Auftrag:** Auftragsnummer.
- **Pos (int Pos):** Nummer der internen Position.
- **Teile-Nr:** Teilenummer.
- **Sequenz:** Sequenznummer der Bearbeitung.
- **Bearbnr:** Artikelnummer der Bearbeitung.
- **MZO-Maschine:** Nummer der Maschine, auf der die Bearbeitung durchgeführt wird.

### Summenzeile

In der Summenzeile können Sie sich verschiedene Summen anzeigen lassen, z. B.:
- **Menge Soll Gesamt:** Gesamtmenge und Menge in den markierten Läufen.
- **Dauer gesamt:** Gesamte Bearbeitungsdauer der markierten Läufe in Stunden.

### Filter

- **[Filter hinzufügen]** Fügt einen Filter ein.
- **Dropdown-Menü** Auswahl eines Filters:
    - **Klick:** Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
    - **Rechtsklick:** Öffnet einen Dialog, um den aktuellen Filter zu bearbeiten.

## Arbeitsplan – Übersicht

*Pfad: Anzeigen > Produktionsmonitor > Schicht > Kontextmenü > Arbeitsplan > Übersicht*

[Image: Dialog "Arbeitsplan: Selektion aus Produktionsmonitor – Übersicht"]
*Abb. E-94 Arbeitsplan: Selektion aus Produktionsmonitor – Übersicht*

In diesem Register können Sie sich einen Überblick zu den Bearbeitungstypen verschaffen, die in der gewählten Arbeitsschicht an einer Maschine ausgeführt werden.

Die Anzeige der Spalten können Sie auf die gleiche Weise einrichten, wie im Register Details.

## Einlastung

*Pfad: Anzeigen > Einlastung*

[Image: Dialog "Einlastung"]
*Abb. E-95 Einlastung*

In diesem Dialog prüfen Sie Aufträge, die als XML-Daten aus A+W Business oder A+W Enterprise importiert werden. Mit Öffnen des Dialogs werden die Aufträge automatisch importiert. Nach dem Import wird im Feld Status die aktuelle Uhrzeit angezeigt.

Wenn in A+W Production ein automatischer Import der Aufträge eingerichtet ist, müssen Sie den Dialog Einlastung nicht öffnen. Der Datenimport läuft dann als Hintergrundprozess. Sie können den Prozess der Einlastung über den A+W Service Monitor verfolgen.

## Stücklistenkonfiguration

*Pfad: Stammdaten > Einlastung > Stücklistenkonfiguration*

[Image: Dialog "Stücklistenkonfiguration"]
*Abb. E-96 Stücklistenkonfiguration*

In diesem Dialog können Sie die Stücklistenkonfiguration analysieren.

> **i Keine Änderungen der Stücklistenkonfiguration**
> Änderungen im Dialog Stücklistenkonfiguration bedeuten einen tiefen Eingriff in die Struktur von A+W Production. Ändern Sie die Stücklistenkonfiguration auf keinen Fall. Bei Fragen wenden Sie sich bitte an den Kundenservice der A+W Software GmbH.

## Aktion

*Pfad: Stammdaten > Einlastung > Stücklistenkonfiguration > [Neu], [Ändern]*

[Image: Dialog "Stücklistenkonfiguration – Aktion"]
*Abb. E-97 Stücklistenkonfiguration – Aktion*

In diesem Dialog können Sie die einzelnen Aktionen zur Stücklistenmanipulation analysieren. Jede Aktion besteht aus mindestens einer Bedingung, bei deren Zutreffen die hinterlegte Funktion ausgeführt wird.

> **i Keine Änderungen der Stücklistenkonfiguration**
> Änderungen im Dialog Stücklistenkonfiguration bedeuten einen tiefen Eingriff in die Struktur von A+W Production. Ändern Sie die Stücklistenkonfiguration auf keinen Fall. Bei Fragen wenden Sie sich bitte an den Kundenservice der A+W Software GmbH.

## Umlastung

*Pfad: Anzeige > Produktionsmonitor > Doppelklick auf Schicht > > Kontextmenü > Arbeitsplan > Umlastung*
*Pfad: Anzeige > Aufträge > Kontextmenü > Bearbeitungen > Kontextmenü > Arbeitsplan > Umlastung*
*Pfad: Anzeige > Läufe > Kontextmenü > Bearbeitungen > Kontextmenü > Arbeitsplan > Umlastung*

[Image: Dialog "Umlastung"]
*Abb. E-98 Umlastung*

In diesem Dialog können Sie Bearbeitungen aus Aufträgen oder Läufen auf andere Termine und Maschinen umlasten.

⇨ Tutorial, "Umlastungen" auf Seite E-448

### 1. Wählen Sie umzulastende Bearbeitungen aus

Liste der Bearbeitungen, die umgelastet werden können.

- **Auftrag:** Liste der Bearbeitungen, sortiert nach Datum und Maschinen.
- **Position:** Positions-Nummer der jeweiligen Bearbeitung.
- **Produktionstermin:** Bisheriger Termin, an dem die Bearbeitung durchgeführt werden soll.
- **Schicht:** Bisherige Arbeitsschicht, in der die Bearbeitung durchgeführt werden soll.
- **Geschützt:** Anzeige, ob der Termin geschützt ist.
- **Arbeitsgang:** Arbeitsgang, mit dem die Bearbeitung durchgeführt wird.
- **Logische Maschine:** Logische Maschine, die für die Bearbeitung verwendet wird.
- **Menge:** Teilemenge, die bei der Bearbeitung hergestellt wird.
- **Maschine:** Maschine, auf der die Bearbeitung durchgeführt wird.
- **Teilenummer:** Nummer der Stücklistenkomponente.
- **Sequenz:** Sequenz der Bearbeitung.
- **BearbNr:** Bearbeitungs-Nummer der Bearbeitung.
- **Bestell-Information:** Angabe, ob Bestellteile enthalten sind.

**Einlastung erzwingen** Sie können die Einlastung auf einen bestimmten Termin erzwingen.
- Die Termin-Umlastung wird nicht erzwungen.
- Die Termin-Umlastung wird erzwungen. Mit dieser Einstellung werden die Kapazitätsgrenzen von Engpassbetriebsmitteln nicht berücksichtigt. Daher werden die Arbeitsschichten ggf. überbucht.

**Erlaube Eilraster** Sie können für die Umlastung festlegen, dass die Übergangszeiten vom Typ Eil verwendet werden.
- Die Termin-Umlastung wird mit den normalen Übergangszeiten berechnet.
- Die Termin-Umlastung wird mit den Eil-Übergangszeiten berechnet.

**Kombobox (Schutz)** Auswahl, ob Termine vor Umlastungen geschützt sind. In der Regel setzen Sie den Schutz nach einer erfolgreichen Umlastung.
- **Geschützte Bearbeitungstermine beibehalten:** Geschützte Bearbeitungstermine werden nicht umgelastet.
- **Umlastungsziele schützen:** Die nach der Umlastung berechneten neuen Termine werden vor weiteren Umlastungen geschützt.
- **Alle Bearbeitungstermine schützen:** Alle Bearbeitungstermin der markierten Läufe werden geschützt.
- **Bearbeitungsschutz aufheben:** Der Schutz für alle Bearbeitungstermine der markierten Läufe wird aufgehoben.

**Begründung** Wenn Sie für die Umlastung auch einen Termin in der Vergangenheit zulassen wollen, müssen Sie eine Begründung eingeben. Damit wird die entsprechende Checkbox freigeschaltet.
⇨ "Erlaube Zieltermine in der Vergangenheit" auf Seite E-585

**Tage für automatische Lieferterminverschiebung** Angabe, um wie viele Tage der Liefertermin verschoben werden darf.

> **i Umlasten und Versandtermin**
> Der Versandtermin ist bei der Umlastung geschützt, um die Anforderungen des ERP-Systems zu erfüllen. Der Versandtermin bleibt bestehen, solange Sie ihn nicht explizit umlasten.
> Halten Sie Rücksprache mit dem Auftragserfasser, falls Sie einen Versandtermin verändern wollen.

**Als Chefauftrag umlasten** Sie können die Bearbeitung mit oberster Priorität umlasten.
- Die Bearbeitung wird mit der normalen Priorität umgelastet.
- Die Bearbeitung wird mit oberster Priorität umgelastet. Die Aufträge werden mit den minimalen Übergangszeiten eingelastet. Dabei können auch die Zeiten von Kampagnen genutzt werden. Verwenden Sie diese Einstellung nur in Notfällen.

**Ignoriere Wareneingangstermine** Manche Bearbeitungen sind davon abhängig, dass zugekaufte Teile angeliefert sein müssen, z. B. die Fertigung einer ISO-Scheibe mit einem ESG, das nicht selbst produziert wird.
- Für die Fertigung wird ein Wareneingang erwartet. Der Wareneingang wird vor der Umlastung geprüft.
- Der Wareneingang wird vor der Umlastung nicht geprüft.

**Lieferterminverschiebungen zurückmelden** Die Umlastung einer Position kann den Liefertermin betreffen.
- Bei einer Lieferterminverschiebung für eine Position wird der Liefertermin aus dem Auftragskopf zurückgemeldet.
- Eine Lieferterminverschiebung einer Position wird an den Auftrag zurückgemeldet. Der Liefertermin im Auftragskopf wird angepasst. Das ist jedoch nur möglich, wenn die Daten online übertragen werden.

**Erlaube Zieltermine in der Vergangenheit** Sie können bei der Umlastung auch Termine in der Vergangenheit zulassen. Die Checkbox ist nur freigeschaltet, wenn Sie eine Begründung eingegeben haben.
- Termine werden nicht in die Vergangenheit verschoben.
- Die Bearbeitung kann auch in die Vergangenheit verschoben werden. Dazu müssen Sie eine Begründung eingeben.
⇨ "Begründung" auf Seite E-584

### 2. Wählen Sie Datum, Schicht und Maschine aus

In diesem Bereich werden die Maschinen und die jeweils zugehörigen Arbeitsschichten pro Arbeitstag angezeigt.

- **[Ansicht aktualisieren]** Aktualisiert die Liste.
- **[Gegebene Anzahl von Tagen zurück]** Verschiebt den Zeitraum der angezeigten Arbeitsschichten um die Anzahl der Tage in die Vergangenheit, die im Feld Tage angegeben ist.
- **Starttermin** Angabe des Starttermins, von dem an der Zeitraum angezeigt werden soll.
- **Tage** Angabe, um wie viele Tage die Anzeige der Arbeitsschichten mit den Schaltflächen jeweils vor- oder zurückgestellt werden soll.
- **[Gegebene Anzahl von Tagen vor]** Verschiebt den Zeitraum der angezeigten Arbeitsschichten um die Anzahl der Tage in die Zukunft, die im Feld Tage angegeben ist.

### 3. Umlastung ausführen

**Zum Start der Umlastung den Modus auswählen** Auswahl, in welchem Modus die Umlastung erfolgt:
- **Komplette Stückliste umlasten:** Die komplette Stückliste, zu der die Bearbeitung gehört, wird umgelastet.
- **Nur markierte Bearbeitung:** Nur die markierte Bearbeitung wird umgelastet.
- **Markierte und alle folgende Bearbeitungen:** Die markierte und alle nachfolgenden Bearbeitungen der Stückliste werden umgelastet.
- **Markierte und alle vorherigen Bearbeitungen:** Die markierte und alle vorherigen Bearbeitungen der Stückliste werden umgelastet.
- **Unbedingte Terminzuweisung für markierte Bearbeitung:** Die markierte Bearbeitung wird auf den ausgewählten Termin der gewählten Maschine umgelastet. Die Plausibilität wird nicht geprüft und die Maschinenkapazitäten werden dabei nicht berücksichtigt.

- **[Umlasten]** Startet die Umlastung mit den gewählten Parametern. Die Schaltfläche ist nur freigeschaltet, wenn ein Umlastungsmodus ausgewählt ist.
- **[Schließen]** Schließt den Dialog, ohne die Daten zu speichern.

## Maschinenumlastung

*Pfad: Aufträge > Kontextmenü > Arbeitsplan > Maschinenumlastung*
*Pfad: Läufe > Kontextmenü > Maschinenumlastung*

[Image: Dialog "Maschinenumlastung"]
*Abb. E-99 Maschinenumlastung*

In diesem Dialog können Sie Bearbeitungen aus Aufträgen oder Läufen auf andere Logische Maschinen umlasten. Bei der Maschinenumlastung wird die Bearbeitungsdauer nicht neu berechnet. Die Kosten und Einlastungsregeln werden nicht geprüft.
Eine Umlastung über diesen Dialog ist daher nur sinnvoll, wenn Sie auf eine identische Logische Maschine umlasten können.

- **Logische Routen**: Maschinen und logische Maschinen, von denen aus eine Bearbeitung umgelastet werden soll.
- **Umlastungsalternativen**: Anzeige und Auswahl der möglichen Alternativen zu der markierten logischen Maschine.
- **[Übernehmen]** Speichert die Daten.
- **[Schließen]** Schließt den Dialog, ohne die Daten zu speichern.

## Nachbearbeitung Einlastung

*Pfad: Stammdaten > Nachbearbeitung Einlastung*

[Image: Dialog "Nachbearbeitung Einlastung"]
*Abb. E-100 Nachbearbeitung Einlastung*

In diesem Dialog können Sie Aufträge, die nicht erfolgreich eingelastet wurden, nachbearbeiten und erneut einlasten.
⇨ Tutorial, "Eingelastete Aufträge nachbearbeiten" auf Seite E-453

- **[Bearbeiten]** Öffnet den Dialog Fehlerhafte Aufträge, in dem Sie auf Probleme bei der Einlastung reagieren können.
⇨ "Fehlerhafte Aufträge" auf Seite E-591
- **[Aktualisieren]** Aktualisiert die Ansicht mit aktuellen Daten.

### Übersicht Aufträge

Die Anzeige der Spalten hängt von der Option ab, die im Feld **Nachbearbeitung von ...** gewählt ist.

- **Auftrag:** Die Auftragsnummer wird angezeigt, wenn die Option undefinierten Artikeln gewählt ist.
- **Artikel-Nr., Artikelbez.:** Nummer und Bezeichnung des Artikels, der nicht definiert ist, werden angezeigt, wenn die Option undefinierten Artikeln oder undefinierten Bearbeitungen gewählt ist.
- **Produktionsartikelnummer, Produktionsartikel:** Nummer und Bezeichnung des Produktionsartikels, der nicht definiert ist, werden angezeigt, wenn die Option undefinierten Produktionsartikel/Dicke-Kombinationen gewählt ist.
- **Dicke:** Die Dicke in mm wird angezeigt, wenn die Option undefinierten Produktionsartikel/Dicke-Kombinationen gewählt ist.
- **Meldung:** Der Text der Rückmeldung wird angezeigt, wenn die Option Rückmeldungsprobleme gewählt ist.
- **Status:** Der Status der Aufträge wird angezeigt, wenn die Option fehlerhafter Auftragsdaten gewählt ist.
- **Anzahl Aufträge:** Die Anzahl der Aufträge mit gleichem Status wird angezeigt, wenn die Option fehlerhafter Auftragsdaten gewählt ist.
- **Zeitstempel der Importdatei:** Datum und Uhrzeit, zu denen der Auftrag eingelastet wurde.
- **Pos.:** Die Nummer der Auftragsposition wird angezeigt, wenn die Option Änderungen verplanter Aufträge gewählt ist.
- **PosRef.:** Die Referenznummer der Auftragsposition wird angezeigt, wenn die Option Änderungen verplanter Aufträge gewählt ist.
- **Packmittelgruppe:** Die Packmittelgruppe, die dem Lauf zugeordnet ist, wird angezeigt, wenn die Option Änderungen verplanter Aufträge gewählt ist.
- **Anzahl Pos.:** Die Anzahl der zum Lauf gehörenden Positionen wird angezeigt, wenn die Option Änderungen verplanter Aufträge gewählt ist.
- **Änderungstext:** Die Anmerkung aus dem ERP-System wird angezeigt, wenn die Option Änderungen verplanter Aufträge gewählt ist. Dazu muss die Anmerkung mit übergeben worden sein.

### Nachbearbeitung von

Mit der Wahl der Option legen Sie fest, nach welchen Kriterien die Aufträge in der Liste angezeigt werden sollen. In der Klammer steht jeweils, wie viele Aufträge mit dem Kriterium vorhanden sind.
Bei undefinierten Artikeln, Dicken-Kombinationen und/oder Bearbeitungen können Sie den Auftrag mit einem Doppelklick öffnen und korrigieren.

- **Undefinierten Artikeln (n Aufträge):** Aufträge mit undefinierten Artikeln.
- **Undefinierten Produktionsartikel-/Dicke-Kombinationen (n Aufträge):** Aufträge mit undefinierten Produktionsartikel-Kombinationen und undefinierten Dicke-Kombinationen.
- **Undefinierten Bearbeitungen (n Aufträge):** Aufträge mit undefinierten Bearbeitungen.
- **Rückmeldeproblemen (n Aufträge):** Aufträge mit Rückmeldeproblemen. Rückmeldeprobleme können bei der Datenübergabe zwischen einem ERP-System und A+W Production entstehen.
⇨ "Asynchrone Verarbeitung" auf Seite E-591
- **Änderungen verplanter Aufträge (n Aufträge):** Aufträge, die nach der Einlastung geändert wurden.
⇨ "Änderung bereits verplanter Aufträge" auf Seite E-593
- **Fehlerhafter Auftragsdaten (n Aufträge):** Aufträge mit fehlerhaften Auftragsdaten.
⇨ "Fehlerhafte Aufträge" auf Seite E-591
- **Aufträgen mit Hinweisstatus (n Aufträge):** Aufträge mit einem Hinweisstatus.

### Anzeigen nach

Mit der Wahl der Option legen Sie fest, wie die Aufträge in der Liste sortiert werden.
- **Auftragsnummer:** Sortierung nach Auftragsnummern.
- **Nachbearbeitungsursache:** Sortierung nach Nachbearbeitungsursachen.

### Detailanzeige für Läufe und Packmittelgruppen

Das Feld wird angezeigt, wenn die Option Änderungen verplanter Aufträge gewählt ist.
- **Lauf:** Nummer des Laufs.
- **Laufstatus:** Status des Laufs.
- **Packmittelgruppe:** Packmittelgruppe, die dem Lauf zugeordnet ist.

## Fehlerhafte Aufträge

*Pfad: Stammdaten > Nachbearbeitung Einlastung > Option Fehlerhafter Auftragsdaten > [Bearbeiten]*

[Image: Dialog "Fehlerhafte Aufträge"]
*Abb. E-101 Fehlerhafte Aufträge*

In diesem Dialog können Sie wählen, wie nicht eingelastete Aufträge verarbeitet werden sollen.
⇨ Tutorial, "Eingelastete Aufträge nachbearbeiten" auf Seite E-453

Dazu können Sie zwischen folgenden Optionen wählen:

- **Erneute Datenübernahme:** Markierte Aufträge werden erneut eingelastet. Verwenden Sie diese Option z. B. bei Fehlern in den Stammdaten, z. B. wenn A+W Production keine Arbeitsschicht für den Auftrag gefunden hat. Wenn Sie den Fehler behoben haben, können Sie den Auftrag einlasten, ohne eine erneute Datenübertragung vom ERP-System anzufragen.
- **Einlastung erzwingen. Die freie Kapazität an Engpassbetriebsmitteln wird in diesem Fall nicht berücksichtigt.:** Der Auftrag wird erneut eingelastet. Dabei wird die Kapazität der Maschine nicht berücksichtigt. Daher werden die Arbeitsschichten ggf. überbucht. Wenn eine Kapazität überschritten ist, kann es zu Terminverschiebungen bei anderen Aufträgen kommen.
- **Einlastung ignorieren. Die Produktionstermine werden ermittelt ohne Rücksicht auf Übergangszeiten, Kapazitätsgrenzen und Kampagnentermine. Gültige Arbeitspläne müssen Sie mittels manueller Umlastung erstellen.**
- **Löschung der fehlerhaften Aufträge. Die Aufträge können dann mit diesem System NICHT verplant werden. Rücksprache mit Auftragserfassung erforderlich!:** Die Aufträge werden aus A+W Production gelöscht. Die Aufträge müssen im ERP-System korrigiert und erneut übertragen werden.
- **Ermittelten Liefertermin bestätigen:** Übernahme des neuen Liefertermins, den A+W Production für die gewählten Aufträge vorschlägt. Die Aufträge werden zu den neuen Liefertermin-Bedingungen eingelastet und der ermittelte Liefertermin wird an das ERP-System zurück gemeldet. Ändern Sie Liefertermine nur nach Absprache mit der Auftragserfassung.

## Asynchrone Verarbeitung

*Pfad: Stammdaten > Nachbearbeitung Einlastung > Option Rückmeldungsprobleme > [Bearbeiten]*

[Image: Dialog "Asynchrone Verarbeitung"]
*Abb. E-102 Asynchrone Verarbeitung*

In diesem Dialog können Sie wählen, wie Aufträge mit Problemen bei der Rückmeldung verarbeitet werden sollen.

Dazu können Sie zwischen folgenden Optionen wählen:
- **Erneuten Versuch starten:** Markierte Aufträge werden erneut eingelastet. Verwenden Sie diese Option z. B. bei Fehlern während der Datenübertragung.
- **Position stornieren:** Die Position wird storniert. Der restliche Auftrag wird eingelastet. Bei dieser Option sollten Sie Rücksprache mit dem Auftraggeber halten, damit die Daten erneut übertragen werden.
- **Fehler ignorieren:** Die Produktionstermine werden ermittelt. Die Position wird übernommen, die Rückmeldung wird jedoch nicht geschrieben. Deshalb dürfen Sie diese Option nur auswählen, wenn Sie absolut sicher sind, dass Sie den Fehler ignorieren können.

## Änderung bereits verplanter Aufträge

*Pfad: Stammdaten > Nachbearbeitung Einlastung > [Bearbeiten]*

[Image: Dialog "Änderung bereits verplanter Aufträge"]
*Abb. E-103 Änderung bereits verplanter Aufträge*

In diesem Dialog können Sie wählen, wie eingelastete Aufträge behandelt werden sollen, zu denen Änderungen übertragen wurden.

Dazu können Sie zwischen folgenden Optionen wählen.

- **Neue Position erzeugen: Storno der bisherigen Position und Übernahme der Änderung als neue Position in den Pool.:** Der Auftrag wird mit einer neuen Positionsnummer erneut eingelastet.
- **Erneut versuchen: Übernahme der Änderung in den Pool. Lösen Sie zuvor die betroffenen Läufe/PMO-Mastergruppen auf.:** Lösen Sie die betroffenen Läufe zunächst auf und wählen Sie anschließend diese Option. Der Auftrag wird erneut eingelastet.
- **Änderung ignorieren: Löschung der Änderung. Die bisherige Position bleibt unverändert.:** Die Änderung wird gelöscht und die ursprünglichen Daten beibehalten.
- **(nicht empfohlen): Übernahme der Änderung in die bisherigen Läufe. Stellen Sie zuvor sicher, dass die Änderung nicht produktionsrelevant ist.:** Zur Zeit nicht genutzt.

- **[Änderung analysieren]** Zur Zeit nicht genutzt.

## Positionssplit

*Pfad: Anzeigen > Aufträge > Kontextmenü > Positionen splitten*

[Image: Dialog "Positionssplit"]
*Abb. E-104 Positionssplit*

In diesem Dialog können Sie Positionen aus Aufträgen aufsplitten. Wenn bei einer großen Position die Bearbeitungsdauer der langsamsten Maschine die konfigurierte Schwelle überschreitet, wird diese Position im Rahmen der Einlastung durch A+W Capacity Planner gesplittet. In der Regel werden die Positionen automatisch gesplittet, so dass die Terminfindung auch bei großen Positionen mit optimaler Geschwindigkeit abläuft.

Der Positionssplit ist im Part Grobplanung - Tutorial beschrieben.

### Markierte Positionen

In der Liste werden die Positionen angezeigt, die Sie im Dialog Bearbeitungen ausgewählt haben.

- **Auftrag:** Auftrag, den Sie zum Splitten ausgewählt haben.
- **Pos.:** Nummer der Auftragsposition.
- **UPos.:** Nummer der Unterpositionen im Auftrag.
- **Menge:** Anzahl der Scheiben in der Position.

- **[Entfernen]** Löscht die markierte Position.

### Splitting-Optionen

Mit der Wahl der Option legen Sie fest, wie die Positionen geteilt werden:

- **Je Position in ... Positionen aufteilen:** Angabe, in wie viele neue Positionen aufgeteilt wird. Das Feld zur Angabe der Anzahl wird freigeschaltet.
- **Positionen mit maximal ... Scheiben erzeugen:** Angabe, wie viele Scheiben eine neue Position maximal enthalten darf. Das Feld zur Angabe der Anzahl wird freigeschaltet.
- **Je Pos. eine Pos. mit ... Scheiben erzeugen:** Angabe der Scheibenanzahl, für die jeweils eine neue Position erzeugt wird. Das Feld zur Angabe der Anzahl wird freigeschaltet.
- **Teilung gemäß PMO Ergebnis:** Angabe, dass die Positionen passend zur Packmitteloptimierung gesplittet werden.

### Neue Positionen

In der Liste werden die gesplitteten Positionen als Unterpositionen angezeigt.

- **Auftrag:** Auftragsnummer.
- **Pos.:** Nummer der Auftragsposition.
- **UPos.:** Nummer der Unterpositionen im Auftrag.
- **Neue Position:** Nummer der neuen Position nach dem Split. Die Nummerierung wird pro gesplitteter Auftragsposition gezählt.
- **Menge:** Anzahl der Scheiben in der neuen Position.

- **[Splitten]** Splittet die markierte Position. Die neuen Positionen werden erst gespeichert, wenn sie mit [Übernehmen] bestätigt sind.
- **[Übernehmen]** Speichert die neuen Positionen. Diese Aktion kann nicht rückgängig gemacht werden.
- **[Verwerfen]** Stellt die ursprüngliche Position wieder her. Anschließend können Sie die Position mit anderen Vorgaben splitten.
- **[Schließen]** Schließt den Dialog, ohne die Daten zu speichern.

# Kampagnen und Reservierungen

Für bestimmte Arbeitsgänge und/oder Aufträge können Sie Kampagnen einrichten und Kapazitäten reservieren.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Kampagnen" auf Seite E-597
- "Abgelaufene Reservierungen" auf Seite E-601
- "Reservierungen" auf Seite E-603
- "Reservierung für Maschine" auf Seite E-606
- "Kunde auswählen" auf Seite E-606
- "Objekt auswählen" auf Seite E-608

## Kampagnen

*Pfad: Stammdaten > Kapazitätsplanung > Kampagnenplanung*

In diesem Dialog können Sie Kampagnen als Einzeltermine oder wöchentliche Termine definieren. Mit Kampagnen können Sie für bestimmte Arbeitsgänge Kapazitäten einplanen, z. B. für Siebdruck für jeden Wochentag eine andere Farbe.

> **i Voraussetzung**
> Nur die Bearbeitungen werden in Kampagnenterminen eingelastet, die als Kampagnen-Bearbeitungen definiert sind.

⇨ Tutorial, "Kampagnenplanung" auf Seite E-455

Der Dialog **Kampagnen** enthält folgende Register:
- "Kampagnen – Einzeltermine" auf Seite E-598
- "Kampagnen – Wöchentliche Termine” auf Seite E-600

## Kampagnen – Einzeltermine

*Pfad: Stammdaten > Kapazitätsplanung > Kampagnenplanung > Register Einzeltermine*

[Image: Dialog "Kampagnen - Einzeltermine"]
*Abb. E-105 Kampagnen - Einzeltermine*

In diesem Register verwalten Sie Einzelkampagnen. Mit Einzelkampagnen führen Sie Kampagnen durch, die einmalig anfallen.

⇨ Tutorial, "Kampagnenplanung" auf Seite E-455

- **Arbeitsgang**: Arbeitsgänge, die Sie in der Maschinenzuordnung erzeugt haben. Ein Arbeitsgang ist in der Liste hellgrau hinterlegt, wenn er zu einer Kampagne hinzugefügt ist.

- **Kampagnen**: Kampagnenfähige Arbeitsgänge, die Sie hinzugefügt haben. Wenn Sie in der Liste Kampagnen einen Arbeitsgang markieren, werden in den Registern **Einzeltermine** oder **Wöchentliche Termine** die zugehörigen Termine angezeigt.
    - ☐ Die Kampagne ist nicht aktiv.
    - ☑ Die Kampagne ist aktiv.

- **[Zuordnen]** Verschiebt ein markiertes Element auf die andere Seite.

### Einzeltermine

- **Kalender**: Auswahl eines Datums für eine Kampagne.
- **Schichten**: Verfügbare Arbeitsschichten am gewählten Datum.
    > **i Anzeige der Schichten**
    > Nur die aktiven Schichtpläne werden angezeigt. Aktivieren Sie ggf. die Schichtpläne, die für die Kampagne benötigt werden.
- **Einzeltermine**: Anzeige der Kampagnen für das markierte Datum.
    - **Datum:** Termine, zu denen Sie Kampagnen erzeugt haben.
    - **Schicht:** Arbeitsschicht, in der die jeweilige Kampagne durchgeführt wird.
    > **i Kampagnen löschen**
    > Wenn Sie kurzfristig Kampagnen löschen, hat das Auswirkungen auf die Produktion. Bearbeitungen werden z. B. nicht durchgeführt oder Produktionstermine ändern sich.
    > Bitte wenden Sie sich an den Kundenservice der A+W Software GmbH, wenn Sie Kampagnen löschen wollen und zu diesem Zeitpunkt bereits Aufträge eingelastet sind.

- **Hinzufügen für die nächsten**: Angabe, für welchen Zeitraum die Kampagne angelegt wird. Mit der Wahl der Option legen Sie fest, ob die Dauer des Termins in Tagen oder Wochen angegeben wird.
- **[Kampagne hinzufügen]** Fügt eine Kampagne hinzu. Dazu müssen folgende Elemente markiert sein:
    - ein kampagnenfähiger Arbeitsgang
    - ein Termin
    - eine Schicht
- **[Löschen]** Löscht die markierte Kampagne.
- **[OK]** Speichert die Daten.
- **[Abbrechen]** Schließt den Dialog, ohne die Daten zu speichern.

## Kampagnen – Wöchentliche Termine

*Pfad: Stammdaten > Kapazitätsplanung > Kampagnenplanung > Register Wöchentliche Termine*

[Image: Dialog "Kampagnentage - Wöchentliche Termine"]
*Abb. E-106 Kampagnentage - Wöchentliche Termine*

In diesem Register verwalten Sie Serienkampagnen. Mit Serienkampagnen führen Sie regelmäßig wiederkehrende Kampagnen durch.

⇨ Tutorial, "Kampagnen anlegen und verwalten" auf Seite E-458
Eine Beschreibung der Felder im Dialog Kampagnen finden Sie hier:
⇨ "Kampagnen - Einzeltermine" auf Seite E-598

### Wöchentliche Termine

Anzeige der Kampagnen für den markierten Wochentag.
- **Wochentag:** Arbeitstage, zu denen Sie Kampagnen erzeugt haben.
- **Schicht:** Arbeitsschicht, in der die jeweilige Kampagne durchgeführt wird.

## Abgelaufene Reservierungen

*Pfad: Stammdaten > Kapazitätsplanung > Reservierungen*

[Image: Dialog "Abgelaufene Reservierungen"]
*Abb. E-107 Abgelaufene Reservierungen*

In diesem Dialog werden abgelaufene Reservierungen angezeigt. Der Dialog wird automatisch geöffnet, wenn Sie den Dialog Reservierungen öffnen und abgelaufene Reservierungen vorhanden sind.

### Liste

- **Maschine:** Maschine, auf der Kapazität reserviert wurde.
- **Kunde:** Kunde, für den Kapazität reserviert wurde.
- **Objekt:** Objekt, für das Kapazität reserviert wurde.
- **Woche:** Kalenderwoche, in der Kapazität reserviert wurde.
- **Jahr:** Jahr, für das Kapazität reserviert wurde.
- **Datum:** Datum, an dem die Reservierung beginnt.
- **Schicht:** Arbeitsschicht, für die Kapazität reserviert wurde.
- **Prozent:** Kapazität in Prozent, die auf der Maschine reserviert wurde.
- **Verbraucht:** Angabe in Prozent, wie viel von der Reservierung bereits verbraucht wurde.
- **Ablauf:** Datum, an dem die Reservierung endet.

- **[Löschen]** Löscht die markierte Reservierung.
- **[OK]** Speichert die Daten und wechselt zum Fenster **Reservierungen**.

## Reservierungen

*Pfad: Stammdaten > Kapazitätsplanung > Reservierungen*

[Image: Dialog "Reservierungen"]
*Abb. E-108 Reservierungen*

In diesem Dialog verwalten Sie Reservierungen von Maschinenkapazitäten. Reservierungen sind nur auf den einzelnen Maschinen möglich, die als Engpassbetriebsmittel definiert sind. Sie sind zeitlich begrenzt. Ein Engpassbetriebsmittel kann nicht über seine Kapazität hinaus bebucht werden.

Die Reservierungen werden entweder für spezifische Kunden oder Bauprojekte angelegt.

Im Produktionsmonitor werden die reservierten Zeiten in den jeweiligen Arbeitsschichten gekennzeichnet.

⇨ Tutorial, "Reservierungen" auf Seite E-466

> **i Reservierungen für einzelne Aufträge**
> Reservierungen von Zeiten für einzelne Aufträge müssen vom ERP-System erfasst und übertragen werden. Die als Reservierungsauftrag gekennzeichneten und zur Produktion freigegebenen Aufträge reservieren auf allen für die Produktion benötigten Maschinen entsprechende Zeiten.

### Reservierungen

> **i Reservierungen in Schichten, Tagen oder Wochen**
> In der Regel werden Kapazitäten wochenweise reserviert. Je nach Einstellung unter Stammdaten > Konfiguration > A+W Production > Kapazitätsplanung > Art der Reservierung können für die Reservierung aber auch Tage oder Arbeitsschichten angegeben werden. Wenn Sie die Einstellung ändern, gehen die alten Reservierungen verloren.

- **Maschine**: Auswahl der Maschine, deren Reservierungen angezeigt werden. In der Auswahl-Liste sind alle Maschinen angezeigt, die als Engpassbetriebsmittel definiert sind.
- **Starttermin**: Beginn des Reservierungszeitraums. Standardmäßig wird der aktuelle Kalendertag angezeigt.
- **Tage**: Angabe, wie viele Tage in der Vorschau angezeigt werden.

### Schichtreservierungen

Im Bereich Schichtreservierungen werden die Reservierungen ab dem ausgewählten Datum grafisch dargestellt.

- **Frei**: Freie Kapazität der Maschine.
- **Reserviert**: Reservierte Kapazität der Maschine.
- **Benutzt**: Tatsächlich benutzter Anteil der Reservierung.

### Reservierungen pro Kunde

Ist im Bereich Schichtreservierungen ein Tag markiert, wird eine Übersicht mit allen Reservierungen angezeigt.

- **Kunde:** Kunde, für den Kapazitäten reserviert sind.
- **Objekt:** Objekt, für das Kapazitäten reserviert sind.
- **Reservierung:** Reservierte Maschinen-Kapazitäten in Prozent.
- **Benutzt:** Tatsächlich benutzter Anteil der Reservierung in Prozent.
- **Ablaufdatum:** Datum, an dem die Reservierung endet.
- **Datum:** Datum, an dem die Reservierung erfasst wurde.
- **Schicht:** Arbeitsschicht, für die die Reservierung gilt.

- **[Neu]** Öffnet den Dialog zum Reservieren von Maschinen-Kapazitäten. ⇨ "Reservierung für Maschine" auf Seite E-606
- **[Löschen]** Löscht die markierte Reservierung.
- **[OK]** Speichert die Daten.
- **[Ende]** Bricht die Bearbeitung ab und schließt den Dialog.

## Reservierung für Maschine

*Pfad: Stammdaten > Kapazitätsplanung > Reservierungen > [Neu]*

[Image: Dialog "Reservierung für Kunde oder Objekt"]
*Abb. E-109 Reservierung für Kunde oder Objekt*

In diesem Dialog reservieren Sie Maschinen-Kapazitäten für einen bestimmten Kunden oder ein Objekt.

> **i Reservierungen in Schichten, Tagen oder Wochen**
> In der Regel werden Kapazitäten wochenweise reserviert. Je nach Einstellung unter Stammdaten > Konfiguration > A+W Production > Kapazitätsplanung > Art der Reservierung können für die Reservierung aber auch Tage oder Arbeitsschichten angegeben werden. Wenn Sie die Einstellung ändern, gehen die alten Reservierungen verloren.

- **Kunde**: Kunde, für den Maschinen-Kapazität reserviert wird. Die [Lupe] öffnet den Dialog **Kunde auswählen**. ⇨ "Kunde auswählen" auf Seite E-606
- **Objekt**: Objekt, für das Maschinen-Kapazität reserviert wird. Die [Lupe] öffnet den Dialog **Objekt auswählen**. ⇨ "Objekt auswählen" auf Seite E-608
- **Datum**: Beginn des Reservierungszeitraums.
- **Schicht**: Arbeitsschicht, in der die Maschine reserviert ist.
- **Ablaufdatum**: Ende des Reservierungszeitraums.
- **Reservierung in %**: Maschinen-Kapazität in Prozent, die reserviert werden soll. Sie können die Reservierung als Betrag eingeben oder indem Sie den Balken im Feld darüber mit der Maus aufziehen.
- **[OK]** Speichert die Daten.
- **[Schließen]** Schließt den Dialog, ohne die Daten zu speichern.

## Kunde auswählen

*Pfad: Stammdaten > Kapazitätsplanung > Reservierungen > [Neu] > Kunde*

[Image: Dialog "Kunde auswählen"]
*Abb. E-110 Kunde auswählen*

In diesem Dialog wählen Sie den Kunden, für den Sie Maschinen-Kapazitäten reservieren wollen.

### Übersicht

- **ID:** Kundennummer.
- **Name:** Name des Kunden.
- **Matchcode:** Matchcode, der dem Kunden zugewiesen wurde.

- **Matchcode**: Angabe des Matchcodes für die Kundensuche.
- **Name**: Angabe des Namens für die Kundensuche.
- **Anzahl**: Anzahl der Kunden, die in der Übersicht angezeigt werden.
- **[Suchen]**: startet die Suche, wenn Sie im Filterkriterium die Wild Card % eingesetzt haben.
- **[OK]**: Übernimmt den markierten Kunden in den Dialog **Reservierung für Maschine**.
- **[Schließen]**: Schließt den Dialog, ohne die Daten zu übernehmen.

## Objekt auswählen

*Pfad: Stammdaten > Kapazitätsplanung > Reservierungen > [Neu] > Objekt*

[Image: Dialog "Objekt auswählen"]
*Abb. E-111 Objekt auswählen*

In diesem Dialog wählen Sie ein Objekt, für das eine Reservierung vorgenommen wird.

### Übersicht

- **ID:** Identifikationsnummer des Objekts.
- **Beschreibung:** Name des Objekts.

- **Name**: Angabe des Namens für die Objektsuche.
- **Anzahl**: Anzahl der Objekte, die in der Übersicht angezeigt werden.
- **[Suchen]**: startet die Suche, wenn Sie im Filterkriterium die Wild Card % eingesetzt haben.
- **[OK]**: Übernimmt das markierte Objekt in den Dialog **Reservierung für Maschine**.
- **[Schließen]**: Schließt den Dialog, ohne die Daten zu übernehmen.

# Bearbeitungen

Die Bearbeitungen beschreiben die Arbeitsschritte zur Fertigung der Teile. Die Bearbeitungserzeugung stellt sicher, dass für jedes Stücklistenteil beschrieben wird, wie es in der Produktion entsteht. Diese Information ist für A+W Capacity Planner unabdingbar und auch sonst ist es sinnvoll, z.B. auf Papieren die ganze Entstehung der Produkte zu sehen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Bearbeitungserzeugung" auf Seite E-610
- "Existierende Bedingung hinzufügen" auf Seite E-612

## Bearbeitungserzeugung

*Pfad: Stammdaten > Kapazitätsplanung > Bearbeitungserzeugung*

[Image: Dialog "Bearbeitungserzeugung"]
*Abb. E-112 Bearbeitungserzeugung*

In diesem Dialog ordnen Sie den Teiletypen jeweils die Bearbeitungsartikel zu, die in den Stammdaten hinterlegt sind. Diese Zuordnung ist z. B. dann notwendig, wenn Ihr ERP-System diese Bearbeitungen nicht übergibt.

Anhand der Zuordnungen können Arbeitsgänge ermittelt werden. Diese Angaben werden für die Produktionsplanung und Kostenermittlung benötigt.

Bei der Bearbeitungserzeugung werden für die Teile der Stückliste den Teiletypen und den Beschaffungsarten entsprechende Bearbeitungen erzeugt. Die Bearbeitungen beschreiben die Entstehung der Teile. Damit die Kapazitätsplanung arbeiten kann, müssen mindestens für alle Lagerentnahmen, Bestell- und Zuschnittsteile und Zusammenbaubearbeitungen, wie VSG und ISO, Bearbeitungen definiert sein.

Beachten Sie zusätzliche Bearbeitungen wie Verpacken und Versenden, sofern dies nicht von Ihrem ERP-System übergeben werden.

⇨ Tutorial, "Bearbeitungen erzeugen" auf Seite E-477

### Bearbeitungserzeugung

- **Bearbeitungen**: Produktionsrelevante Bearbeitungstypen und zugeordnete Bearbeitungsartikel.
- **Teiletypen**: Teiletypen mit zugeordneten Bearbeitungsartikeln.
- **[Zuordnen]**: Ordnet einen markierten Bearbeitungsartikel dem markierten Teiletyp zu.

### Details

Informationen zum markierten Bearbeitungstyp oder Bearbeitungsartikel.

- **Artikelnummer:** Artikelnummer des markierten Bearbeitungsartikels.
- **Bearbeitungstyp:**
    - Bei markiertem Bearbeitungsartikel: Zugeordneter Bearbeitungstyp.
    - Bei markiertem Bearbeitungstyp: ID des Bearbeitungstyps.
- **Beschaffungsart:** Beschaffungsart des Bearbeitungstyps.
- **Klasse:** Bearbeitungsklasse des markierten Bearbeitungsartikels, z. B. **Säumen**.
- **Name:** Name des markierten Elements.
- **Sequenz/Sequenznummer:** Sequenznummer des markierten Elements. Je höher eine Sequenznummer ist, desto später wird die Bearbeitung am Glas durchgeführt.
    - Ist für einen Bearbeitungsartikel eine Sequenz angegeben, wird diese berücksichtigt.
    - Ist für einen Bearbeitungsartikel keine Sequenz angegeben, wird die Sequenz des Bearbeitungstyps verwendet.
    Für alle erzeugenden Bearbeitungen kann die Sequenz 100 gesetzt werden, z. B. für Isolieren, Vorspannen oder Verpacken. Für alle anderen Bearbeitungen muss die Sequenz entsprechend aufsteigend sein, z. B. für Säumen und Bohren.
> **i Sequenz und Sequenznummer**
> Die Sequenz steuert die Reihenfolge der Bearbeitungen und ist damit produktionsrelevant. Wenden Sie sich an den Kundenservice der A+W Software GmbH, wenn Sie Sequenzen ändern möchten.
- **Teiletyp:** Nummer des Teiletyps, z. B. 2 für Handelsglas. Der Teiletyp wird durch die A+W Software GmbH festgelegt. Im Feld darunter wird die Beschreibung zum markierten Element angezeigt.

- **[Kategorien]** Sortiert die Elemente nach Kategorien.
- **[Alphabetisch]** Sortiert die Elemente alphabetisch.
- **[Eigenschaften]** Zur Zeit nicht genutzt.

### Bedingungen

Formeln, die dem Bearbeitungsartikel zugeordnet sind, der im Bereich Teiletypen markiert ist.

> **i Formeln und Bedingungen**
> Formeln beeinflussen die Eigenschaften und planungstechnischen Auswirkungen von Bearbeitungstypen und Teiletypen unter Umständen massiv. Sie müssen verstehen, welche Auswirkungen die hinterlegte Formel hat. Zum Thema Formeln und Restriktionen in A+W Production gibt es ein separates Handbuch.

- **[Neu]** Öffnet den Dialog **Existierende Bedingung hinzufügen**, um dem Bearbeitungsartikel eine Formel zuzuordnen.
- **[Löschen]** Löscht die markierte Formel im Feld **Bedingungen**.
- **[OK]** Speichert die Daten.

## Existierende Bedingung hinzufügen

*Pfad: Stammdaten > Kapazitätsplanung > Bearbeitungserzeugung > [Neu Drop-down-Menü] > Existierende Bedingung hinzufügen, Standardbedingung hinzufügen*

[Image: Dialog "Existierende Bedingung hinzufügen"]
*Abb. E-113 Existierende Bedingung hinzufügen*

In diesem Dialog wählen Sie die Bedingung aus, die Sie im Dialog **Bearbeitungserzeugung** einer Bearbeitung zuordnen wollen.

- **[OK]** Übernimmt eine markierte Formel in den Dialog **Bearbeitungserzeugung**.
- **[Schließen]** Schließt den Dialog, ohne eine Bedingung in den Dialog **Bearbeitungserzeugung** zu übernehmen.

# Stammdaten für Zeiten

Für alle Bearbeitungen müssen Zeiten hinterlegt werden, aus denen die Dauer pro Bearbeitungsposition errechnet werden kann.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Vorgabezeiten" auf Seite E-614
- "Vorgabezeitformel" auf Seite E-616
- "Elemente hinzufügen" auf Seite E-620
- "Tabelle, Vektor (Name)" auf Seite E-621
- "Eingabehilfe für Vektoren" auf Seite E-622
- "Formel auswählen" auf Seite E-624
- "Erfassung eines Formelelements" auf Seite E-624
- "Benutzerdefinierte Tabellenelemente" auf Seite E-626
- "Grenzwert auswählen" auf Seite E-626
- "Zeitformeltest" auf Seite E-627
- "Eigenschaften des Formelobjekts" auf Seite E-629
- "Formel (Name)" auf Seite E-630
- "Verlauf der Formelauswertung" auf Seite E-631
- "Übergangszeiten” auf Seite E-632

## Vorgabezeiten

*Pfad: Stammdaten > Kapazitätsplanung > Vorgabezeiten*

[Image: Dialog "Vorgabezeiten"]
*Abb. E-114 Vorgabezeiten*

In diesem Dialog verwalten Sie die Berechnungsformeln für die Bearbeitungen an einer der logischen Maschinen. Mit einer Formel definieren Sie, wie die Dauer eines Arbeitsgangs berechnet wird. Basis der Berechnung ist z. B. die jeweilige Fläche oder Kantenlänge in der einzelnen Auftragsposition.

⇨ Tutorial, "Vorgabezeiten" auf Seite E-518

Für die Erstellung von Formeln stehen zwei verschiedene Editoren zur Verfügung. Eine ausführliche Beschreibung der Editoren finden Sie im Part Formeleditor.

In der Zeile **0 – Alle Maschinen** können Sie Formelelemente als Vorlagen für alle Maschinen definieren.

### Vorgabezeitformeln

In der Übersicht sind alle in A+W Production definierten Maschinen angezeigt. Diese Daten werden aus der Maschinenzuordnung eingelesen und können nicht bearbeitet werden.

- **Nr.:** Nummer der logischen Maschine.
- **Log.:** Logische ID der logischen Maschine.
- **Maschine:** Name der Maschine.
- **Log. Maschine:** Name der logischen Maschine.
- **Engpass:** Anzeige, ob die Maschine als Engpass definiert ist.
- **Einzel:** Anzeige, ob die Maschine Bearbeitungsketten bildet. Wenn keine Bearbeitungsketten gebildet werden sollen, werden die Bearbeitungen einzeln abgehandelt, d. h. eine nach der anderen in separaten Arbeitsschritten verplant. Diese Einstellung ist z. B. für Siebdruck, Flächenbearbeitungen usw. wichtig. Für Bohren, Schleifen usw. sollte die Checkbox nicht markiert sein, da für diese Bearbeitungen Bearbeitungsketten sinnvoll sind.
- **Manuell:** Anzeige, ob die Maschine manuell bedient wird. Manuelle Maschinen werden nicht in die automatische Maschinenumlastung einbezogen. Sie sind außerdem für den automatischen Positionssplit gesperrt.
- **Typ:** Maschinentyp der zugehörigen Maschine.
- **Id:** Nummer der Logischen Maschine. Diese ID ist für den technischen Support wichtig.

- **[Bearbeiten]** Öffnet den Dialog **Vorgabezeitformel**, um die Vorgabezeitformel zu bearbeiten. ⇨ "Vorgabezeitformel" auf Seite E-616
> **i Bereits vorhandene Vorgabezeitformel**
> Wenn Sie auf Bearbeiten klicken und bereits eine formelbasierte Vorgabezeitformel zugeordnet ist, wird eine Meldung angezeigt. Wenden Sie sich an den Kundenservice der A+W Software GmbH, wenn Sie die Vorgabezeit ändern wollen.
- **[Löschen]** Löscht den markierten Eintrag.
- **[Ende]** Schließt den Dialog, ohne die Daten zu übernehmen.

## Vorgabezeitformel

*Pfad: Stammdaten > Kapazitätsplanung > Vorgabezeiten > [Bearbeiten]*

[Image: Dialog "Vorgabezeitformel – Beispiel der Auswahlmöglichkeiten"]
*Abb. E-115 Vorgabezeitformel – Beispiel der Auswahlmöglichkeiten*

In diesem Dialog bearbeiten Sie die Taktzeiten einer logischen Maschine.

> **i Vorgabezeitformel ändern**
> Ändern oder erstellen Sie Vorgabezeitformeln nur in Rücksprache mit dem Kundenservice der A+W Software GmbH.
>
> Komplexe Vorgabezeitformeln stellen einen tiefgreifenden Eingriff in A+W Production dar und sollen nur vom Kundenservice der A+W Software GmbH vorgenommen werden. Eine Vorgabezeitformel gilt z. B. dann als komplex, wenn sie zwei und mehr Faktoren/Vektoren enthält.

⇨ Tutorial, "Vorgabezeitformeln anlegen und verwalten" auf Seite E-530

### Vorgabezeitformel

Liste der Elemente, die zur Formel gehören.

**Basiszeit**: Angabe der Basiszeit für die Vorgabezeitformel in Sekunden. Wenn die Berechnung mit der Ermittlung aus einer Formel beginnt, legen Sie als Startwert 0 fest, z. B. die Berechnung einer Fläche bevor der erste Siebdruck aufgetragen wird.

Sie können folgende Zeitzuschläge für die Berechnung definieren:
- **Faktor 'Gas':** Zuschlag für das Befüllen von ISO mit Gas.
- **Faktor 'Sprossen':** Zuschlag in Abhängigkeit von der Anzahl der Sprossen.
- **Modellfaktor:** Zuschlag in Abhängigkeit vom gewählten Modell.
- **Faktor 'Große Scheibe', Faktor 'Kleine Scheibe':** Zuschlag in Abhängigkeit von der Größe der Scheiben. Dazu geben Sie auch die Maße der Scheibe an.
- **Faktor 'ESG':** Zuschlag, mit dem Sie die Handhabung von ESG berücksichtigen.
- **Faktor 'VSG':** Zuschlag, mit dem Sie die Handhabung von VSG berücksichtigen.
- **Faktor 'mindestens Dreifach-ISO':** Zuschlag, mit dem Sie die Handhabung von ISO berücksichtigen.
- **Beschichtungsfaktor:** Zuschlag, mit dem Sie die Handhabung von beschichteten Scheiben berücksichtigen.
- **Vektor 'Gewicht -> Faktor':** Zuschlag in Abhängigkeit vom Gewicht der Scheiben.
- **Vektor 'Länge -> Faktor':** Zuschlag in Abhängigkeit von der zu bearbeitenden Kantenlänge.
- **Vektor 'Anzahl -> Faktor':** Zuschlag in Abhängigkeit von der Anzahl der zu bearbeitenden Scheiben.
- **Vektor 'Dicke -> Faktor':** Zuschlag in Abhängigkeit von der Dicke der Scheiben.
- **Vektor 'Fläche -> Faktor':** Zuschlag in Abhängigkeit von der zu bearbeitenden Fläche.
- **Vektor 'Kantenmatrix -> Faktor':** Zuschlag in Abhängigkeit von der Kantenmatrix der Scheiben.
- **'Freies' Element 1 - 10:** Freie Elemente für weitere Zeitzuschläge.

**+ Wert, + Vektor, + Tabelle**: Auswahl der Rechenoperation für einen konstanten Wert, einen Vektor oder eine Tabelle:

| Einstellung | Bedeutung |
| --- | --- |
| **+ Tabelle** | Der Wert aus der Tabelle wird zum Zwischenergebnis addiert. |
| **+ b * Wert** | Die Basiszeit wird mit dem Wert multipliziert. Das Ergebnis der Multiplikation wird zum Zwischenergebnis addiert. |
| **+ Wert** | Der Wert wird zum Zwischenergebnis addiert. |
| **\* (1 + Wert)** | Der Wert wird zu 1 addiert und das Ergebnis mit dem Zwischenergebnis aus der vorausgehenden Zeile multipliziert. |
| **\* Vektor** | Das Ergebnis der vorausgehenden Zeile wird mit dem Wert des Vektors multipliziert. |
*Tab. E-5 Mögliche Einstellungen für die Vorgabezeitformel*

> **i Berechnungsreihenfolge**
> Bei der Berechnung müssen Sie die Operatorrangfolge der Mathematik berücksichtigen: Multiplikation und Division werden vor Addition und Subtraktion gerechnet – es sei denn, Klammern geben die Reihenfolge vor.
> Außerdem müssen Sie die Reihenfolge der Zeilen beachten, wenn eine Berechnung auf dem Ergebnis der vorausgehenden Zeile aufbauen soll.

**[...]** Öffnet den Dialog **Vektor (Name)**, in dem Sie die Eigenschaften des Vektors bearbeiten.
⇨ "Tabelle, Vektor (Name)" auf Seite E-621

**[Verschieben]** Verschiebt ein markiertes Element in der Vorgabezeitformel. Die Reihenfolge der Faktoren ist wichtig, wenn Sie die Option **Faktor multipliziert mit Zwischensumme** wählen.

**Multiplikation des Formelergebnisses mit der Bearbeitungsmenge pro Teil**: Sie können das Formelergebnis mit der Bearbeitungsmenge pro Teil multiplizieren lassen.
- ☐ Das Formelergebnis wird nicht mit der Bearbeitungsmenge pro Teil multipliziert.
- ☑ Das Formelergebnis wird mit der Bearbeitungsmenge pro Teil multipliziert.

**Eigene Formel**: Anzeige der zugewiesenen Formel.

- **[Lupe]**: Öffnet den Dialog **Formel auswählen**, in dem Sie hinterlegte Formeln auswählen. ⇨ "Formel auswählen" auf Seite E-624
- **[X]**: Entfernt die Formel aus dem Feld **Eigene Formel**.
- **[Formeleditor]**: Öffnet den Dialog **Erfassung eines Formelelements**, in dem Sie eine Formel anlegen können. Zum Thema **Formel-Editor** gibt es ein separates Handbuch. ⇨ "Erfassung eines Formelelements" auf Seite E-624
- **Formeltest**: Öffnet den Dialog **Zeitformeltest**, mit dem Sie Formeln zur Zeitberechnung prüfen. ⇨ "Zeitformeltest" auf Seite E-627
- **[Neu]**: Öffnet den Dialog **Elemente hinzufügen**, in dem Sie Elemente auswählen können. ⇨ "Elemente hinzufügen" auf Seite E-620
- **[OK]**: Speichert die Daten.
- **[Ende]**: Schließt den Dialog, ohne die Daten zu übernehmen.

## Elemente hinzufügen

*Pfad: Stammdaten > Kapazitätsplanung > Vorgabezeiten > [Bearbeiten] > [Neu]*

[Image: Dialog "Elemente hinzufügen"]
*Abb. E-116 Elemente hinzufügen*

In diesem Dialog können Sie Elemente für Zeitzuschläge in den Dialog **Vorgabezeitformel** übernehmen.

⇨ Tutorial, "Vorgabezeitformeln anlegen und verwalten" auf Seite E-530

- **[Löschen]** Löscht den markierten Eintrag.
- **[OK]** Übernimmt den markierten Eintrag in den Dialog **Vorgabezeitformel**.
- **[Ende]** Schließt den Dialog, ohne die Daten zu übernehmen.

## Tabelle, Vektor (Name)

*Pfad: Stammdaten > Kapazitätsplanung > Vorgabezeiten > logische Maschine markieren > [Bearbeiten] > Element einfügen > [...] *

[Image: Dialoge für "Werterfassung - Tabellarische Erfassung" und "Matrixdarstellung"]
*Abb. E-117 Werterfassung - Tabellarische Erfassung, Matrixdarstellung*

In diesem Dialog bearbeiten Sie die Eigenschaften eines Zeitzuschlags. Sie können die Werte je nach Typ in der tabellarischen Erfassung bearbeiten.

⇨ Tutorial, "Vorgabezeitformeln anlegen und verwalten" auf Seite E-530

- **Spalten**: Die Anzeige der Spalten hängt von dem Formelelement ab, zu dem der Dialog geöffnet ist, z. B. Dicke, Gewicht, Höhe und Breite.
    > **Beispiel Dicke**
    > Wenn Sie für die Dicke in der Tabelle die Werte 4,00 mm, 8,00 mm und 10,00 mm angeben, gelten die zugewiesenen Faktoren jeweils für die Dicken 4,00 bis 7,99 mm, 8,00 bis 9,99 mm, usw.
- **Wert**: Faktor pro Dicke, Gewicht, Länge, Anzahl, Fläche oder Kantenmatrix.
- **[Eingabehilfe]**: Öffnet den Dialog **Eingabehilfe für Vektoren**. ⇨ "Eingabehilfe für Vektoren" auf Seite E-622
- **[OK]**: Übernimmt den markierten Eintrag in den Dialog **Vorgabezeitformel**.
- **[Schließen]**: Schließt den Dialog, ohne die Daten zu übernehmen.

## Eingabehilfe für Vektoren

*Pfad: Stammdaten > Kapazitätsplanung > Vorgabezeiten > logische Maschine markieren > Bearbeiten > [...] > Vektor einfügen > [Eingabehilfe]*

[Image: Dialog "Eingabehilfe für Vektoren"]
*Abb. E-118 Eingabehilfe für Vektoren*

In diesem Dialog können Sie die Tabelle im Dialog **Vektor ...** automatisch ausfüllen lassen, indem Sie Werte vorgeben.

⇨ Tutorial, "Vorgabezeitformeln anlegen und verwalten" auf Seite E-530

### Vorgabewerte

In diesem Bereich geben Sie die Grenzwerte für die Berechnung der Tabelle ein.

- **Startwert**: Startwert, mit dem die Tabelle beginnt. Der Startwert entspricht der Tabellen-Spalte Dicke, Gewicht, Länge, Anzahl, Fläche oder Kantenmatrix im Dialog **Faktor/Vektor (Name)**. Geben Sie zum Beispiel bei dem Vektor 'Länge -> Faktor' als Startwert die Länge von 100 mm an, um die Berechnung bei 100 mm zu beginnen.
- **Endwert**: Endwert, mit dem die Tabelle schließt. Der Endwert entspricht der Tabellen-Spalte Dicke, Gewicht, Länge, Anzahl, Fläche oder Kantenmatrix im Dialog **Faktor/Vektor (Name)**. Geben Sie zum Beispiel bei dem Vektor 'Länge -> Faktor' als Endwert die Länge von 2000 mm an, um die Berechnung bei 2000 mm zu beenden.
- **Schrittgröße**: Größe, mit der die Grenzwerte zwischen Start- und Endwert angelegt werden. Die Schrittgröße entspricht der Tabellen-Spalte Dicke, Gewicht, Länge, Anzahl, Fläche, oder Kantenmatrix im Dialog **Faktor/Vektor (Name)**. Geben Sie zum Beispiel bei dem Vektor 'Länge -> Faktor' als Schrittgröße 100 mm an. Damit bekommt der Vektor alle 100 mm einen anderen Wert zugeordnet, z. B. 100,00 bis 199,00 mm, 200,00 bis 299,99 mm, usw.

### Werte

In diesem Bereich geben Sie die Werte für die Berechnung der Zeitzuschläge pro Grenzwert ein.

- **Startwert**: Wert, mit dem der Zeitzuschlag für den kleinsten der angegebenen Grenzwerte berechnet wird. Der Startwert entspricht der Tabellen-Spalte **Faktor** im Dialog **Vektor ...**. Geben Sie zum Beispiel bei dem Vektor 'Länge -> Faktor' als Startwert 1 an. Damit wird dem Vektor bei einer Länge zwischen 100 mm und 199,99 mm der Wert 1 zugeordnet.
- **Schrittgröße**: Wert, um den der Berechnungswert pro Grenzwert erhöht wird. Die Schrittgröße entspricht der Tabellen-Spalte **Faktor** im Dialog **Vektor ...**. Geben Sie zum Beispiel bei dem Vektor 'Länge -> Faktor' als Schrittgröße 2 an. Damit wird der Wert des Vektors alle 100 mm um den Wert 2 erhöht, z. B. die Werte 1, 3, 5, usw.

- **[OK]** Speichert die Daten.
- **[Schließen]** Schließt den Dialog, ohne die Daten zu speichern.

## Formel auswählen

*Pfad: Stammdaten > Kapazitätsplanung > Vorgabezeiten > Bearbeiten > Eigene Formel*

[Image: Dialog "Formel auswählen"]
*Abb. E-119 Formel auswählen*

In diesem Dialog können Sie definierte Formeln auswählen und im Dialog **Vorgabezeitformel** einfügen.

⇨ Tutorial, "Vorgabezeitformeln anlegen und verwalten" auf Seite E-530

> **i Eigene Formeln**
> Zusätzliche Formeln beeinflussen das Verhalten und die Eigenschaften von Vorgabezeitformeln unter Umständen massiv. Bitte wenden Sie sich an den Kundenservice der A+W Software GmbH, falls Sie eigene Formeln benötigen oder bestehende Formeln ändern wollen.

- **ID**: Identifikationsnummer der Formel.
- **Formel**: Name der Formel.
- **Beschreibung**: Beschreibung der Formel.
- **Sprache**: Auswahl der Sprache, in der die Formeln geschrieben sind. Wählen Sie z. B. English, werden nur Formeln angezeigt, die in dieser Sprache definiert sind.
- **Text**: Formelsuche über den Namen.
- **[OK]**: Speichert die Daten.
- **[Verwerfen]**: Schließt den Dialog, ohne die Daten zu speichern.

## Erfassung eines Formelelements

*Pfad: Stammdaten > Kapazitätsplanung > Vorgabezeiten > [Bearbeiten] > [Formeleditor], [Neu]*

[Image: Dialog "Erfassung eines Formelelements"]
*Abb. E-120 Zeitformel - Element erfassen*

In diesem Dialog können Sie ein eigenes Element zur Berechnung einer Zeitformel erfassen.

⇨ Tutorial, "Editor für Formelelemente" auf Seite E-525

- **Name**: Name, der in der Auswahl der Formelelemente angezeigt wird.
- **Elementtyp**: Auswahl des Elementtyps.
    - **Festes Element:** Ausdrücke ohne Benutzereingabe, z. B. Langkante. Diese Einstellung sollten Sie nicht mehr für neue Definitionen verwenden. Sie ist durch **Freies Element** abgelöst worden.
    - **Bedingung:** Ausdrücke mit einer Benutzereingabe, die verwendet wird, wenn die Bedingung wahr ist.
    - **Freies Element:** Ausdrücke, bei denen das Ergebnis mit der Benutzereingabe gewichtet wird, z. B. Sekunden pro Schleifmeter.
    - **Schwellenwert:** Ausdrücke, bei denen der Schwellenwert für die Bedingung einstellbar ist, ohne die Formeldefinition zu verändern, z. B. Mengenzuschlag ab Benutzereingabe.
    - **Vektor:** Ausdrücke, bei denen eine Tabelle mit Wertepaaren aus Mindestwerten und zu verwendenden Koeffizienten gepflegt wird.
- **Beschriftung**: Bezeichnung, die im Dialog **Vorgabezeitformel** angezeigt wird.
- **Definition**: Formel für die Berechnung bei den Elementtypen **Festes Element**, **Bedingung** und **Freies Element**.
- **Eingabeformat**: Format der Maßeinheit für die Elementtypen **Schwellenwert** und **Vektor**:
    - **Einheitenlos:** Keine Maßeinheit.
    - **Dicke, Länge:** Millimeter, inch.
    - **Fläche:** Quadratmeter, square foot.
Mit der Einstellung wird gewährleistet, dass die Eingaben für die Parameter in der Einheit interpretiert werden, die in A+W Production konfiguriert ist.
- **Beschriftung**: Bezeichnung, die im Dialog **Vorgabezeitformel** vor dem Berechnungswert angezeigt wird, z. B. **sec.** bei einem Zeitwert.
- **Definition**: Anzeige der Formel für einen unabhängigen Parameter, der bei einem Vektor oder Schwellenwert ausgewählt ist.

## Benutzerdefinierte Tabellenelemente

*Pfad: Stammdaten > Kapazitätsplanung > Vorgabezeiten > [Bearbeiten] > [Neu] > <Neue Tabelle ...>*

[Image: Dialog "Benutzerdefinierte Tabellenelemente"]
*Abb. E-121 Benutzerdefinierte Tabellenelemente*

In diesem Dialog definieren Sie ein neues Tabellenelement für Vorgabezeitformeln.

⇨ Tutorial, "Struktur von Vorgabezeitformeln" auf Seite E-520

### Eigenschaften

- **Name**: Name des Tabellenelements.
- **Typ**: Typ des Formelelements. Für **Neue Tabelle** stehen folgende Optionen zur Wahl:
    - Vektor (eindimensional)
    - Tabelle (zweidimensional)
    - Würfel (dreidimensional)
- **Wert 1, Wert 2, Wert 3**: Öffnet den Dialog **Grenzwert auswählen**, in dem Sie einen Wert auswählen. Die Anzahl der Felder ist vom gewählten Tabellentyp abhängig. ⇨ "Grenzwert auswählen" auf Seite E-626
- **Beschreibung**: Beschreibung für die Tabellenelemente.
- **[Löschen]**: Löscht das markierte Element.
- **[Speichern]**: Speichert die Daten.
- **[Neu]**: Erstellt ein neues Tabellenelement.
- **[Schließen]**: Schließt den Dialog, ohne die Daten zu speichern.

## Grenzwert auswählen

*Pfad: Stammdaten > Kapazitätsplanung > Vorgabezeiten > [Bearbeiten] > [Neu] > <Neue Tabelle ...> auswählen*

[Image: Dialog "Grenzwert auswählen"]
*Abb. E-122 Grenzwerte für Tabellenelemente*

In diesem Dialog können Sie Grenzwerte für ein neues Tabellenelement auswählen. Das Tabellenelement wird für die Formel zur Berechnung von Vorgabezeiten eingesetzt.

⇨ "Benutzerdefinierte Tabellenelemente" auf Seite E-626

- **[OK]**: Übernimmt die Daten.
- **[Schließen]**: Schließt den Dialog, ohne die Daten zu übernehmen.

## Zeitformeltest

*Pfad: Stammdaten > Kapazitätsplanung > Vorgabezeiten > [Bearbeiten] > [Formeltest]*

[Image: Dialog "Zeitformeltest"]
*Abb. E-123 Zeitformeltest*

In diesem Dialog können Sie Formeln zur Zeitberechnung prüfen lassen. Der Test betrifft immer das markierte Element im Dialog **Vorgabezeitformel**. Wenn die gesamte Vorgabezeitformel getestet werden soll, müssen Sie den Eintrag **Basic Time** markieren.

⇨ Tutorial, "Zeitformel testen" auf Seite E-537

### Formelobjekt

- **Formelobjekt (Name)**: Grafische Darstellung der Formelobjekte. Mit einem Doppelklick öffnen Sie einen Dialog, in dem Sie Werte für den Test eingeben können, z. B. die Scheibenmaße. ⇨ "Eigenschaften des Formelobjekts" auf Seite E-629
- **[Neu]**: Speichert ein neues Formelobjekt.
- **[Laden]**: Lädt ein gespeichertes Formelobjekt.
- **[Speichern]**: Speichert das geänderte Formelobjekt.
- **[Hinzufügen]**: Fügt ein Element unter dem markierten Element ein.
- **[Löschen]**: Löscht das markierte Element.

### Diagnosewerkzeuge

- **Formel anzeigen**: Sie können sich die Syntax der Formel anzeigen lassen.
    - ☐ Die Syntax der Formel wird nicht angezeigt.
    - ☑ Öffnet den Dialog **(Formelname)**, in dem die Syntax der Formel angezeigt wird und kopiert werden kann. ⇨ "Formel (Name)" auf Seite E-630
- **Auswertung protokollieren**: Sie können ein Protokoll der Formel-Auswertung erstellen lassen.
    - ☐ Es wird kein Protokoll erstellt.
    - ☑ Die Auswertung der Formel wird im Dialog **Verlauf der Formelauswertung** angezeigt. ⇨ "Verlauf der Formelauswertung" auf Seite E-631
- **Ergebnis**: Ergebnis der Zeitberechnung in Sekunden. Ein Pfeil nach oben oder nach unten zeigt an, ob das Ergebnis der Vorgabezeitformel höher oder niedriger als die Basiszeit ist.
- **[Auswerten]**: Startet die Auswertung der Formel. Die Auswertung beginnt immer am markierten Formelobjekt. Haben Sie kein Element ausgewählt, beginnt die Auswertung am Kopfteil. Das Ergebnis der Auswertung wird im Feld **Ergebnis** angezeigt. Wenn Sie die Checkbox **Auswertung protokollieren** markiert haben, wird der Dialog **Verlauf der Formelauswertung** geöffnet. ⇨ "Verlauf der Formelauswertung" auf Seite E-631
- **[Schließen]**: Schließt den Dialog, ohne die Daten zu speichern.

## Eigenschaften des Formelobjekts

*Pfad: Stammdaten > Kapazitätsplanung > Vorgabezeiten > Bearbeiten > Formeltest > Doppelklick auf das Formelobjekt*

[Image: Dialog "Zeitformeltest – Eigenschaften des Formelobjekts"]
*Abb. E-124 Zeitformeltest – Eigenschaften des Formelobjekts*

In diesem Dialog geben Sie die Daten für den Formeltest ein, z. B. eine Scheibe mit der Dicke 4 mm und einer Breite von 2.500 mm. In diesem Dialog werden Längen und Dicken in der Einheit Mikrometer (µm) angegeben.

⇨ Tutorial, "Zeitformel-Objekte" auf Seite E-529

### Eigenschaften des Formelobjekts

- **Name**: Name des Formelobjekts.
- **Typ**: Auswahl der Option **Teil** oder **Bearbeitung**.

### Übersicht

- **Eigenschaft:** Zugeordnete Eigenschaft. In der Auswahl-Liste stehen alle Faktoren zur Verfügung, die Sie zur Vorgabezeitformel hinzugefügt haben und deren Eigenschaften bearbeitet werden können.
- **Wert:** Wert für die jeweilige Testberechnung. Bei Längen- und Dicken-Angaben in Mikrometer.
- **[Hinzufügen]** Fügt ein neues Element in der Liste **Eigenschaft** ein. Die Anzeige der Eigenschaften ist abhängig von den Elementen, die in die Vorgabezeitformel eingefügt sind.
- **[Löschen]** Löscht das markierte Element.
- **[Schließen]** Schließt den Dialog, ohne die Daten zu speichern.

## Formel (Name)

*Pfad: Stammdaten > Kapazitätsplanung > Vorgabezeiten > [Bearbeiten] > [Formeltest] > Checkbox Formel anzeigen aktivieren*

[Image: Dialog "Formel-Syntax"]
*Abb. E-125 Formel-Syntax*

In diesem Dialog wird die Formel in der natürlichen Syntax angezeigt, um Fehler in einer Vorgabezeitformel zu finden.

⇨ Tutorial, "Vorgabezeitformeln anlegen und verwalten" auf Seite E-530

- **[Kopieren]** Kopiert die Formel, um sie z. B. in einen Editor einzufügen.
- **[Schließen]** Schließt den Dialog, ohne die Daten zu speichern.

## Verlauf der Formelauswertung

*Pfad: Stammdaten > Kapazitätsplanung > Vorgabezeiten > [Bearbeiten] > [Formeltest] > Checkbox Auswertung protokollieren aktivieren > [Auswerten]*

[Image: Dialog "Verlauf der Formelauswertung"]
*Abb. E-126 Verlauf der Formelauswertung*

In diesem Dialog wird das Protokoll der Formelauswertung angezeigt. Diese Auswertung wird vom Support der A+W Software GmbH benötigt, um eine Formelberechnung zu analysieren.

⇨ Tutorial, "Vorgabezeitformeln anlegen und verwalten" auf Seite E-530

- **[Schließen]** Schließt den Dialog.

## Übergangszeiten

*Pfad: Stammdaten > Kapazitätsplanung > Übergangszeiten*

[Image: Dialog "Übergangszeiten"]
*Abb. E-127 Übergangszeiten*

In diesem Dialog legen Sie Übergangszeiten zwischen (logischen) Maschinen fest. Sie können Übergangszeiten für den optimalen Übergang und für beschleunigte Übergänge definieren. Mit der Angabe von minimalen und maximalen Zeiten legen Sie eine Spanne fest, in der der Übergang stattfinden kann. Bei der Planung wird immer der Übergang vom Ende einer Schicht aus betrachtet.

⇨ Tutorial, "Übergangszeiten" auf Seite E-505

Die Übergangszeiten werden hierarchisch abgearbeitet.
- **Maschine x -> Maschine y** beschreibt den expliziten Übergang zwischen zwei Maschinen.
- **Maschine x -> Alle Maschinen** beschreibt den Übergang am Ausgang von Maschine x.
- **Alle Maschinen -> Maschine x** beschreibt den Übergang am Eingang von Maschine x.
- **Alle Maschinen -> Alle Maschinen** beschreibt den allgemeinen Übergang und wird zuletzt ausgewertet.

⇨ Tutorial, “Übergangszeiten" auf Seite E-505

> **i Übergangszeiten in Schichten**
> In der Regel werden Übergangszeiten in Schichten definiert. Nur in Ausnahmefällen verwenden Sie die Dauer in Stunden und Minuten, z. B. bei Trocknungszeiten.

### Maschinen

- **Maschine 1:** Logische Maschine, von der aus der Übergang stattfindet. Mit einem Doppelklick in ein Feld öffnen Sie den Dialog zur Auswahl einer logischen Maschine.
- **Maschine 2:** Logische Maschine, zu der der Übergang stattfindet. Mit einem Doppelklick in ein Feld öffnen Sie den Dialog zur Auswahl einer logischen Maschine.
- **Typ:** Art der Übergangszeit:
    - **Normal:** Normale Übergangszeit. Sie beschreibt den optimalen Durchgang durch die Produktion, d. h. ohne Ausfälle von Personal oder Maschinen, Bruch usw.
    - **Eil:** Reduzierte Übergangszeit für Eilaufträge, z. B. ohne Verweilzeiten. Mit dieser Zeit erhöhen sich die (virtuellen) Kosten. Diese Übergangszeiten werden automatisch für Aufträge verwendet, die im ERP-System die Priorität **Eil** haben. Diese Aufträge verwenden auch die für Eilaufträge reservierten Arbeitsschichten.
    - **Minimal:** Reduzierte Übergangszeit für Chef-Aufträge. Diese Einstellung dürfen Sie nur verwenden, wenn eine weitere Reduktion technisch überhaupt möglich ist. In der Regel wird diese Einstellung nur verwendet, wenn eine Mindestzeit eingehalten werden muss, z. B. nach dem Autoklav. Nur die Übergangszeit aus der Spalte **Übergangszeit 'h:m'** wird verwendet.
    - **Verboten:** Maschine 2 darf nicht nach Maschine 1 angesteuert werden. Mit dieser Einstellung können Sie z. B. abbilden, dass eine Maschine nicht ohne innerbetrieblichen Transport erreichbar ist.
- **Übergangszeit 'h:m':** Minimale Übergangszeit in Stunden und Minuten. Diese Einstellung wird dann verwendet, wenn die Zeit auch über arbeitsfreie Tage gerechnet wird. Sie können die minimale Übergangszeit und die maximale Übergangszeit in gemischten Einheiten angeben, z. B. eine optimale Übergangszeit von 2 Stunden und eine maximale Übergangszeit von 2 Schichten.
- **Schichten:** Minimale Übergangszeit in Schichten.
- **Maximale Übergangszeit 'h:m':** Maximale Übergangszeit in Stunden und Minuten. Hierbei muss ein Wert eingetragen werden, der mindestens ein Wochenende beschreibt, da die Maschine sonst ggf. am Freitag nicht verwendet wird.
- **Maximale Schichten:** Maximale Übergangszeit in Schichten. Der Wert der maximalen Übergangszeit wird zur minimalen Übergangszeit addiert. So ergibt sich z. B. aus einer minimalen Übergangszeit von 1 Schicht und einer maximalen Übergangszeit von 3 Schichten eine Übergangszeit von 1 bis 4 Schichten. Sie können die minimale Übergangszeit und die maximale Übergangszeit in gemischten Einheiten angeben, z. B. eine minimale Übergangszeit von 2 Stunden und eine maximale Übergangszeit von 2 Schichten.

**Beispiel**

| Übergangstyp | Schichten | Maximale Schichten | Spanne in Schichten |
| --- | --- | --- | --- |
| Normal | 2 | 2 | 4 |
| | 2 | 1 | 3 |
| Eil | 1 | | 1 |
| Minimal | 1 | | 1 |

> **i Tipp**
> Wählen Sie für den Übergang zur letzten Bearbeitung, z. B. Verpacken oder Versand, die größte Übergangszeit, die möglich ist. Damit haben Sie in kritischen Situationen größere Flexibilität.

- **[Neu]** Schaltet eine neue Zeile frei, um eine Übergangszeit zu definieren.
- **[Löschen]** Löscht den markierten Eintrag.
- **[OK]** Übernimmt den markierten Eintrag in den Dialog **Vorgabezeitformel**.
- **[Ende]** Schließt den Dialog, ohne die Daten zu speichern.

# Stammdaten der Schichten

Neben den Vorgabe- und Übergangszeiten können auch Schichten definiert werden, in denen die Arbeitszeiten in der Produktion pro Tag definiert werden können.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Schichten" auf Seite E-636
- "Schichtkalender" auf Seite E-637
- "Schichtplan" auf Seite E-637
- "Schichtregel" auf Seite E-639
- "Schichtgruppe" auf Seite E-641
- "Maschine" auf Seite E-643

## Schichten

*Pfad: Stammdaten > Kapazitätsplanung > Schichten*

Zum Dialog **Schichten** finden Sie folgende Kapitel:
- "Schichtkalender" auf Seite E-637
- "Schichtplan" auf Seite E-637
- "Schichtregel" auf Seite E-639
- "Schichtgruppe" auf Seite E-641
- "Maschine" auf Seite E-643

[Image: Dialog "Schichten"]
*Abb. E-128 Schichten*

In diesem Dialog verwalten Sie die Schichtpläne.

> **i Schichten ändern**
> Änderungen an Schichtplänen stellen einen tiefen Eingriff in die Kapazitätsplanung dar. Prüfen Sie im Produktionsmonitor, ob Änderungen korrekt in Arbeitsschichten umgesetzt sind.
> Bereits eingelastete Aufträge werden nicht automatisch umgelastet. Ändern Sie Schichtpläne daher so, dass sie erst zu einem Zeitpunkt zur Verfügung stehen, zu dem aktuell noch keine Aufträge eingelastet sind.
> Für kurzfristige Änderungen stehen verschiedene Funktionen im Produktionsmonitor zur Verfügung.
> Bei Fragen wenden Sie sich an den Kundenservice der A+W Software GmbH.

⇨ Tutorial, "Schichten" auf Seite E-481

### Schichteditor

Im Bereich **Schichteditor** werden der Kalender und die Schichtpläne angezeigt. Über das Kontextmenü oder die Schaltflächen können Sie die verschiedenen Ansichten für die Definition der Schichtpläne öffnen:
- Schichtkalender
- Schichtplan
- Schichtregel
- Schichtgruppe
- Maschine

- **[Neu]** Öffnet die Ansicht **Schichtkalender**, um einen neuen Kalender zu definieren.
- **[Löschen]** Löscht den markierten Eintrag.
- **[Übernehmen]** Speichert die Daten.
- **[Ende]** Schließt den Dialog, ohne die Daten zu speichern.

## Schichtkalender

*Pfad: Stammdaten > Kapazitätsplanung > Schichten > Kalender*

[Image: Dialog "Schichten - Kalender"]
*Abb. E-129 Schichten - Kalender*

In dieser Sicht des Dialogs definieren Sie die arbeitsfreien Tage.

⇨ Tutorial, "Arbeitsfreie Tage anlegen" auf Seite E-484

- **Schichtkalender**: Angabe der arbeitsfreien Tage, zum Beispiel Feiertage.
- **Tag**: Datum des arbeitsfreien Tags.
- **Kommentar**: Bezeichnung des arbeitsfreien Tags, zum Beispiel Weihnachten.
- **[Neu]**: Fügt im Schichtkalender eine neue Zeile ein, um einen arbeitsfreien Tag zu definieren. Über die Auswahl-Liste erstellen Sie einen neuen Schichtplan.
- **[Löschen]**: Löscht den markierten Tag aus dem Schichtkalender.
- **[Übernehmen]**: Speichert die Daten.
- **[Ende]**: Schließt den Dialog, ohne die Daten zu speichern.

## Schichtplan

*Pfad: Stammdaten > Kapazitätsplanung > Schichten > Schichtplan*

[Image: Dialog "Schichten, Schichtplan"]
*Abb. E-130 Schichten, Schichtplan*

In dieser Sicht des Dialogs verwalten Sie die Schichtpläne, mit denen Sie die Arbeitsschichten definieren.

⇨ Tutorial, "Schichtplan erstellen" auf Seite E-487

### Schichtplan

In diesem Bereich erstellen und verwalten Sie einen Schichtplan, z. B. einen Zwei-Schicht-Plan oder einen Drei-Schicht-Plan.

- **ID**: ID des Schichtplans.
- **Name**: Frei wählbarer Name des Schichtplans.
- **Aktiv**: Sie können festlegen, ob der Schichtplan für die Planung von wöchentlichen Kampagnen verwendet werden kann.
    - ☐ Der Schichtplan steht nicht für Wöchentliche Termine zur Verfügung. Er kann im Dialog Kampagnen nicht ausgewählt werden.
    - ☑ Der Schichtplan steht für Wöchentliche Termine zur Verfügung.
- **Gültig ab**: Angabe des Datums, ab dem der Schichtplan gültig ist. Damit können Sie den Schichtplan einrichten, ohne dass die Arbeitsschicht sofort zur Verfügung steht, z. B. für Sonderschichten an einem Wochenende.

### Schichten generieren

Mit der Wahl der Option legen Sie fest, welcher Kalender für den Schichtplan verwendet wird:
- **Eigenen Kalender verwenden:** Verwendet den Kalender, den Sie im Schichtkalender definiert haben.
- **Kalender aus ERP-System übernehmen:** Importiert einen Kalender aus einem ERP-System, z. B. aus A+W Business.

- **Von ..., bis ...**: Angabe des Start- und Enddatums. Arbeitsschichten nach diesem Schichtplan werden im Produktionsmonitor nur für den angegebenen Zeitraum erzeugt.
- **[Erzeugen]**: Erzeugt im Produktionsmonitor eine Arbeitsschicht mit den neuen Daten, die Sie eingegeben haben. Die Schaltfläche wird erst freigeschaltet, wenn Sie eine Schichtregel und eine Schichtgruppe mit Maschinen zugewiesen haben.
- **[Neu]**: Legt einen neuen Schichtplan an. Mit der Auswahl-Liste erstellen Sie eine neue Schichtregel.
- **[Löschen]**: Löscht einen markierten Schichtplan.
- **[Übernehmen]**: Speichert die Daten.
- **[Ende]**: Schließt den Dialog, ohne die Daten zu speichern.

## Schichtregel

*Pfad: Stammdaten > Kapazitätsplanung > Schichten > Schichtregel*

[Image: Dialog "Schichten – Schichtregel"]
*Abb. E-131 Schichten – Schichtregel*

In dieser Sicht des Dialogs verwalten Sie die Schichtregeln eines Schichtplans.

⇨ Tutorial, "Schichtregel erstellen" auf Seite E-490

### Schichtregel

Schichtregeln gelten jeweils für einen einzelnen Schichtplan. Sie können jeder Schichtregel eine Schichtgruppe zuordnen.

- **Name**: Frei wählbaren Namen der Schichtregel, z. B. *Frühschicht normal*.
- **Schichtbeginn, Schichtende**: Angabe der Uhrzeit, zu der die Arbeitsschicht beginnt und endet.
- **Kapazität**: Anzeige der Kapazität der Arbeitsschicht in Stunden. Sie wird aus dem Schichtbeginn und dem Schichtende berechnet.
- **Schichtnummer**: Eingabe der Schichtnummer.
- **Tage**: Angabe der Wochentage, an denen die Arbeitsschicht gefahren werden kann.
    - ☐ Die Arbeitsschicht wird nicht erzeugt.
    - ☑ Die Arbeitsschicht kann im Produktionsmonitor erzeugt werden.

### Schichten generieren

Mit der Wahl der Option legen Sie fest, welcher Kalender für den Schichtplan verwendet wird:
- **Eigenen Kalender verwenden:** Verwendet den Kalender, den Sie im Schichtkalender definiert haben.
- **Kalender aus ERP-System übernehmen:** Importiert einen Kalender aus einem ERP-System, z. B. aus A+W Business.

- **Von ..., bis ...**: Angabe des Start- und Enddatums. Arbeitsschichten nach diesem Schichtplan werden im Produktionsmonitor nur für den angegebenen Zeitraum erzeugt.
- **[Löschen]**: Löscht die markierte Schichtregel mit allen zugeordneten Maschinen. Damit werden die zugehörigen Arbeitsschichten aus dem Produktionsmonitor gelöscht.
- **[Erzeugen]**: Erzeugt im Produktionsmonitor Arbeitsschichten mit den neuen Daten, die Sie eingegeben haben. Die Schaltfläche wird erst freigeschaltet, wenn Sie eine Schichtgruppe mit Maschinen zugewiesen haben.
- **[Neu]**: Erstellt eine neue Schichtregel. Die Auswahl-Liste wird derzeit nicht verwendet.
- **[Löschen]**: Löscht eine markierte Schichtregel.
- **[Übernehmen]**: Speichert die Daten.
- **[Ende]**: Schließt den Dialog, ohne die Daten zu speichern.

## Schichtgruppe

*Pfad: Stammdaten > Kapazitätsplanung > Schichten > Schichtgruppe*

[Image: Dialog "Schichten - Schichtgruppe bearbeiten"]
*Abb. E-132 Schichten - Schichtgruppe bearbeiten*

In dieser Sicht des Dialogs ordnen Sie einer Schichtgruppe die Erfassungsstellen zu. Pro Schichtregel kann jeweils eine Schichtgruppe erstellt werden.

⇨ Tutorial, "Schichtgruppe erstellen" auf Seite E-495

### Schichtgruppe bearbeiten

- **Name der Schichtgruppe**: Name der Schichtgruppe, der die Erfassungsstellen zugeordnet sind.
- **Erfassungsstellennummer**: Nummer der Erfassungsstelle.
- **Name**: Name der Erfassungsstelle.
- **Schichtgruppe**: Schichtgruppe, die der Erfassungsstelle für den aktuellen Schichtplan zugeordnet ist. Sie können eine andere Schichtgruppe auswählen.
- **[Neu]**: Erstellt eine neue Schichtgruppe. Jeder Schichtregel kann nur eine Schichtgruppe zugeordnet werden.
- **[Löschen]**: Löscht eine markierte Schichtgruppe.
- **[Übernehmen]** Speichert die Daten.
- **[Ende]** Schließt den Dialog, ohne die Daten zu speichern.

## Maschine

*Pfad: Stammdaten > Kapazitätsplanung > Schichten > Schichtgruppe > Maschine*

[Image: Dialog "Schichten – Maschine"]
*Abb. E-133 Schichten – Maschine*

In dieser Sicht des Dialogs weisen Sie einer Erfassungsstelle die logischen Maschinen zu.

⇨ Tutorial, "Schichtgruppe erstellen" auf Seite E-495

### Erfassungsstelle

Eigenschaften der markierten Erfassungsstelle und die logischen Maschinen, die der Erfassungsstelle zugeordnet sind.

- **Nummer**: ID der Maschine.
- **Name**: Name der Maschine.
- **Barcode**: Barcode der Maschine.
- **Maschinen**: Logische Maschinen, die der Erfassungsstelle zugeordnet sind.

- **[Löschen]**: Löscht die markierte logische Maschine.
- **[Übernehmen]**: Speichert die Daten.
- **[Ende]**: Schließt den Dialog, ohne die Daten zu speichern.

# Maschinen und Kosten

Maschinen können zur Gruppen zusammengefasst werden, um die verfügbaren Zeiten besser zu verplanen. Außerdem werden an den Maschinen die Kosten hinterlegt.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Kostenkalkulation" auf Seite E-646
- "Maschinengruppen" auf Seite E-647
- "Lastverteilung" auf Seite E-649

## Kostenkalkulation

*Pfad: Stammdaten > Kapazitätsplanung > Kostenkalkulation*

[Image: Dialog "Kostenkalkulation"]
*Abb. E-134 Kostenkalkulation*

In diesem Dialog legen Sie Kosten fest, die an logischen Maschinen anfallen.

Wenn Ihre PPS- und ERP-Systeme vollständig eingerichtet sind, werden die Kosten an das ERP-System zurückgemeldet, z. B. an A+W Enterprise oder A+W Business.

⇨ Tutorial, "Kostenkalkulation" auf Seite E-500

### Kosten

In der Übersicht werden alle definierten Maschinen angezeigt.

- **Maschine:** Nummer und Name der physikalischen Maschine, für die Kosten definiert sind. Mit einem Doppelklick öffnen Sie einen Dialog zur Auswahl einer Maschine.
- **Log. Maschine:** Zugeordnete logische Maschine, zu der die Kosten definiert sind. Mit einem Doppelklick öffnen Sie einen Dialog zur Auswahl einer logischen Maschine.
- **Lohnkosten:** Lohnkosten der logischen Maschine in der Landeswährung.
- **Maschinenkosten:** Maschinenkosten für die logische Maschine in der Landeswährung.
- **Sonstige Kosten:** Sonstige Kosten der logischen Maschine in der Landeswährung. Mit diesen Kosten können Sie z. B. berücksichtigen, dass an einer Maschine zusätzliche Schutzkleidung notwendig ist und kostentechnisch berücksichtigt werden muss.
- **Kommentar:** Kommentare zur logischen Maschine.

- **[Neu]** Schaltet eine neue Zeile frei, um weitere Maschinenkosten anzulegen.
- **[Löschen]** Löscht den markierten Eintrag.
- **[OK]** Übernimmt den markierten Eintrag in den Dialog **Vorgabezeitformel**.
- **[Ende]** Schließt den Dialog, ohne die Daten zu speichern.

## Maschinengruppen

*Pfad: Stammdaten > Kapazitätsplanung > Maschinengruppen*

[Image: Dialog "Maschinengruppen"]
*Abb. E-135 Maschinengruppen*

In diesem Dialog können Sie Maschinen zu Gruppen zusammenfassen und eine Anzahl von Personen zuordnen. Damit gilt eine festgelegte Kapazität für die gesamte Maschinengruppe, z. B. für Arbeitsbereiche wie Zuschnitt, ISO oder Versand.

Das Zusammenfassen zu einer Maschinengruppe funktioniert nur, wenn die Schichtpläne aller Maschinen in der Gruppe übereinstimmen.

Wenn eine Maschine zu einer Maschinengruppe hinzugefügt wird, wird sie automatisch zu einem Engpassbetriebsmittel. Die Überlasteinstellungen der logischen Maschine werden dabei an die Überlasteinstellungen aller logischen Maschinen in der Gruppe angepasst.

⇨ Tutorial, "Maschinengruppen" auf Seite E-544

### Maschinengruppen

- **Gruppe**: Liste der definierten Maschinengruppen.
- **Personen**: Anzahl der Personen, die in der jeweiligen Maschinengruppe tätig sind.

### Maschinen für Gruppe

Im Feld auf der linken Seite sind die logischen Maschinen angezeigt, die zu einer markierten Maschinengruppe hinzugefügt werden können. Auf der rechten Seite sind die logischen Maschinen angezeigt, die zur Maschinengruppe hinzugefügt sind.

- **[Zuordnen]** Verschiebt ein markiertes Element auf die andere Seite.
- **[Neu]** Öffnet einen Dialog, um eine neue Maschinengruppe anzulegen.
- **[Löschen]** Löscht den markierten Eintrag.
- **[OK]** Speichert die Daten.
- **[Ende]** Schließt den Dialog, ohne die Daten zu speichern.

## Lastverteilung

*Pfad: Stammdaten > Kapazitätsplanung > Lastverteilung*

[Image: Dialog "Lastverteilung"]
*Abb. E-136 Lastverteilung*

In diesem Dialog definieren Sie den prozentualen Anteil der logischen Maschinen an der Kapazität der physikalischen Maschine. Sind zu einer Maschine zwei logische Maschinen definiert, können Sie die 100% Last der Maschine auf die logischen Maschinen aufteilen, z. B. zu jeweils 50%.

Lastverteilung nutzen Sie, um zu gewährleisten, dass eine Maschine eine garantierte Mindestkapazität für Spezialaufgaben freihält, z. B. für den Modellzuschnitt. Wenn die freigehaltene Kapazität nicht für Modelle genutzt wird, können auch Rechtecke bearbeitet werden. Diese Lastverteilung ist nur bei Maschinen möglich und sinnvoll, die als Engpassbetriebsmittel definiert sind.

⇨ Tutorial, "Lastverteilung" auf Seite E-550

### Lastverteilung

- **Physikalische Maschinen**: Auswahl der Maschinen, um die Lastverteilung zu bearbeiten.
- **Prüfung aktivieren**: Die Lastverteilung ist gesperrt, um versehentliche Änderungen zu verhindern.
    - ☐ Die Lastverteilung der logischen Maschinen in der Liste kann nicht bearbeitet werden.
    - ☑ Die Lastverteilung der logischen Maschinen in der Liste kann bearbeitet werden.
- **[OK]** Speichert die Daten.
- **[Abbrechen]** Schließt den Dialog, ohne die Daten zu speichern.

# A+W Formeleditor

[Image: A+W Production title page with a puzzle piece graphic]

## Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version / Datum | Beschreibung |
| :--- | :--- |
| 1.02 / 01-2017 | Produkt- und Firmennamen angepasst. |
| 1.01 / 07-2013 | Vollständige Überarbeitung der ALCIM-Dokumentation und Anpassung auf A+W Production. |
| 1.00 / 01-2004 | Ersterstellung |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen

#### Anmerkungen zu diesem Dokument

Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Production gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.

Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von A+W Production.

#### Urheberrechte

© 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

#### Warenzeichen

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

# Tutorial: Der Formeleditor

Den Formeleditor finden Sie in A+W Production in den folgenden Bereichen:
- Organisation
- Maschinenzuordnung
- Etiketten/Skizzen/Biegertexte

Den Formeleditor gibt es in verschiedenen Stufen. Je komplexer die Formel aufgebaut ist, je höher ist die Stufe.

Die Dokumentation zum Formeleditor wurde deshalb wie folgt unterteilt:
- "Elemente des Formeleditors: Stufe I" auf Seite F-9
- "Elemente des Formeleditors: Stufe II" auf Seite F-15
- "Elemente des Formeleditors: Stufe III" auf Seite F-19

## Ziele des Formeleditors

- **Im Bereich der Organisation** ist das Ziel des Formeleditors das Erstellen von Bedingungen zur Trennung von beliebigen Eigenschaften eines Produktes auf die dafür vorgesehenen Abstellplätze.
- **Im Bereich der MZO** ist es das Ziel, Bedingungen zur Lokalisierung von Maschinen in Abhängigkeit der Bearbeitung und Eigenschaften eines Produktes zu erstellen.
- **Das Ziel des Formeleditors im Bereich Etiketten** ist das Erstellen von Bedingungen zur Auswahl des notwendigen Etikettenlayouts in Bezug auf die Produkteigenschaften.

## Elemente des Formeleditors: Stufe I

Im Formeleditor gibt es die folgenden Elemente:
- "Formel" auf Seite F-10
- "Vergleich" auf Seite F-11
- "Bedingung" auf Seite F-11
- "Menge" auf Seite F-14
- "Zuweisung" auf Seite F-15

### Formel

In der einfachsten Form besteht eine Formel aus einem Ausdruck, in dem die erlaubten Eigenschaften der Objekte (Properties), Konstanten, andere Formeln sowie einige Operatoren vorkommen können. Die möglichen Operatoren sind die Grundrechenarten +, -, * und / nebst Klammern. Darüber hinaus gibt es noch die String-Operatoren:

- **@LEFT**: Syntax `STRING @LEFT ANZAHL = STRING`
- **@RIGHT**: Syntax `STRING @RIGHT ANZAHL = STRING`
- **@MID**: Syntax `STRING @MID INDEX = STRING`; der Index ist 0-basiert

Alle diese Operatoren dürfen nahezu beliebig gemischt werden. Die Formel wirkt genau auf ein Teil.

[Image: Formel-Editor dialog]
*Abb. F-1 Formel-Editor*

**Beispiele:**
`$TEILETYP`
`$MENGE * ($DICKE+1000)`
`($BEARB1TEXT @MID $TEILETYP) @RIGHT ($DICKE/1000)`
