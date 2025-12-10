---
title: "DE_HB_AWProduction_3"
source: "DE_HB_AWProduction_3.pdf"
tags: ["A+W Production", "Grobplanung", "Feinplanung", "Softwarereferenz", "Benutzerhandbuch", "Felddefinition", "Export/Import", "Bearbeitungen", "Kontextmenü", "Help Cards"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference and help guide for the A+W Production software, focusing on the 'Grobplanung' (Rough Planning) and 'Feinplanung' (Detailed Planning) modules. It covers topics like field definitions, data import/export, editing processes, and provides step-by-step 'Help Cards' for common workflows."
long_description: "This document serves as a comprehensive technical reference and user guide for A+W Production, a software solution for glass, windows, and doors manufacturing. It is divided into several key sections. The 'Softwarereferenz' part details the functionalities within the 'Grobplanung' (Rough Planning) module, explaining dialogs for field definitions, position views, and various processing steps. It provides detailed descriptions of UI elements, context menus, and database fields for managing orders, batches, and glass types. The document then transitions to 'Übergreifende Dialoge' (General Dialogs), covering features common across the application, such as register properties, column definitions, and filter creation. The second major part of the document consists of 'Help Cards,' which offer practical, step-by-step instructions for performing specific tasks like creating, merging, and archiving production runs ('Läufe'). It concludes with an introduction to the 'Feinplanung' (Detailed Planning) module, outlining its core concepts, such as grouping, sorting, and optimization modes, to prepare users for more advanced production scheduling. The guide is intended for trained users and system administrators, providing both conceptual explanations and actionable workflows."
---

# Softwarereferenz: Positionen in der Grobplanung

---
## Felddefinition

**Navigation:**
Positionen > Kontextmenü – Datenbankspalten > Einfügen > Felddefinitionen > Editieren

*(Abb. C-40 Felddefinition)*

Im Dialog **Felddefinition** können Sie die Definitionen der jeweiligen Felder bearbeiten.

### Menü-Gruppe
Auswahl der Menü-Gruppe, der das Feld zugeordnet wird.

### Menü-Eintrag
Auswahl einer Beschreibung für die gewählte Menü-Gruppe.

### Spaltenüberschrift
Angabe des Spaltennamens. Wenn Sie keine Spaltenüberschrift angeben, wird der Eintrag aus dem Feld Menü-Eintrag als Spaltenüberschrift übernommen.

### Beschreibung
Angabe der Feldbeschreibung. Wenn Sie keine Beschreibung angeben, wird der Eintrag aus dem Feld Menü-Eintrag als Beschreibung übernommen.

### Format
Angabe des Format des Feldes, z. B. ob es sich um Datums-, Längen-, oder Flächenangaben handelt.

### Datenbankfeld
Angabe der Datenbanktabelle und des entsprechenden Feldes, auf das die neue Abfrage bzw. Spalte zugreift.

### Optionen
Sie können wählen, nach welchen Kriterien die angezeigten Daten sortiert werden:
- **Sortierung aufsteigend:** Die angezeigten Daten werden aufsteigend sortiert.
- **Sortierreihenfolge absteigend:** Die angezeigten Daten werden absteigend sortiert.
- **Kumulieren:** Die angezeigten Daten werden kumuliert.

### Anzeigeoptionen
Sie haben verschiedene Optionen, wie die Felder angezeigt werden sollen:

**Gleiche Inhalte in Folgezeilen ausblenden**
Wenn aufeinanderfolgende Felder gleiche Inhalte haben, können Sie diese in Folgezeilen ausblenden.
- Gleiche Inhalte werden in Folgezeilen angezeigt.
- Gleiche Inhalte werden in Folgezeilen ausgeblendet.

**Wert änderbar (nur Positionsanzeige)**
Angabe, ob die Werte in den jeweiligen Feldern geändert werden können.
- Die Werte können nicht geändert werden.
- Die Werte können geändert werden.

**Aufklappkriterium (nur Teileanzeige)**
Auswahl, ob es ein Aufklappkriterium gibt.
- Es gibt kein Aufklappkriterium.
- Es gibt ein Aufklappkriterium.

**[Speichern]**
Speichert den Menüeintrag.

**[Löschen]**
Löscht den gesamten Menüeintrag.

**[Schließen]**
Schließt den Dialog.

## Export/Import Positionsansicht

**Navigation:**
- Positionen > Navigation > Kontextmenü > Ansicht exportieren
- Positionen > Navigation > Kontextmenü > Ansicht importieren

*(Abb. C-41 Export/Import Positionsansicht)*

Im Dialog **Export/Import Positionsansicht** können Sie geänderte oder neue erstellte Ansichten des Dialogs Positionen importieren oder exportieren. Sie wählen dabei, ob der Export bzw. Import global oder lokal durchgeführt wird.
⇨ "Positionen" auf Seite C-195

### Ansichtentyp

**Nur global**
Speichert die neue Ansicht systemweit, für alle Anwender.

**Nur lokal**
Speichert die neue Ansicht nur für den aktuell angemeldeten Anwender.

**[OK]**
Speichert die Daten.

**[Abbrechen]**
Schließt den Dialog, ohne die Daten zu speichern.

# Bearbeitungen in der Grobplanung

In diesem Kapitel finden Sie Informationen zu allen Dialogen, mit denen Sie sich zu Bearbeitungen einen Überblick verschaffen. Sie können Bearbeitungen überwachen und Vorgabezeiten ändern.

Das Kapitel enthält folgende Themen:
- "Bearbeitungen" auf Seite C-205
- "Vorgabezeiten ändern" auf Seite C-208

## Bearbeitungen

**Navigation:**
- Anzeigen > Aufträge > Kontextmenü > Bearbeitungen
- Anzeigen > Töpfe > Kontextmenü > Bearbeitungen
- Anzeigen > Läufe > Kontextmenü > Bearbeitungen
- Anzeigen > Füllaufträge > Kontextmenü > Bearbeitungen
- Glasarten > Kontextmenü > Bearbeitungen
- Details > Kontextmenü > Bearbeitungen
- BDE > Kontextmenü > Bearbeitungen
- Lose > Kontextmenü > Bearbeitungen

*(Abb. C-42 Bearbeitungen (Beispiel))*

Im Dialog **Bearbeitungen** haben Sie eine Übersicht über die Bearbeitungen in den Aufträgen.
Sie können die Register und Spalten im Dialog Bearbeitungen nach Ihren Bedürfnissen anpassen, sodass genau die Informationen angezeigt werden, die Sie benötigen.
Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.

Der Dialog **Bearbeitungen** enthält z. B. folgende Spalten:

- **Termin:** Termin, an dem die Bearbeitung durchgeführt wird.
- **Schicht:** Schicht, in der die Bearbeitung durchgeführt wird.
- **Sequenz:** Sequenznummer der Bearbeitung.
- **Typ:** Nummer des Bearbeitungstyps.
- **ArtikNr:** Artikelnummer.
- **Bezeichnung:** Bezeichnung der Bearbeitung.
- **MZO-Maschine:** Maschine, auf der die Bearbeitung durchgeführt wird.
- **Menge:** Anzahl der zu fertigenden Teile bzw. durchzuführenden Bearbeitungen.
- **Erfassungsstelle:** Erfassungsstelle der zugewiesenen Maschine.
- **Dauer gesamt:** Gesamte Bearbeitungsdauer der markierten Aufträge bzw. Positionen. Einheit: Stunden.

> **Datenbank-Informationen von Spalten**
> Mit einem Rechtsklick auf eine Spalte und der Option **Definition anzeigen** öffnen Sie den Dialog **Spaltendefinition**. Im Dialog Spaltendefinition finden Sie die jeweiligen Datenbank-Informationen einer Spalte.
> ⇨ "Spaltendefinition" auf Seite C-229

### Summenzeile
- **Dauer gesamt:** Gesamte Bearbeitungsdauer der markierten Aufträge bzw. Positionen. Einheit: Stunden.
- **Summe Stück:** Summe der Teile in den markierten Aufträgen bzw. Positionen.

### Filter
**[Filter hinzufügen]** Fügt einen Filter ein.

**Dropdown-Menü**
Sie haben im Dropdown-Menü des Filters folgende Optionen:
- **Klick:** Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
- **Rechtsklick:** Öffnet den Dialog **(Filter Name)**. Mit der Schaltfläche **Verwalten** gelangen Sie in den Dialog **Filter-Definition**, in dem Sie den jeweiligen Filter bearbeiten.
  ⇨ "Filter-Definition" auf Seite C-231

### Kontextmenüs
In folgenden Bereichen des Dialogs Bearbeitungen werden Kontextmenüs angeboten:
- Register
- Spalten
- Liste
- Summenzeile
- Filter

Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen, sind im Kapitel Übergreifende Kontextmenüs gelistet.
⇨ "Übergreifende Kontextmenüs" auf Seite C-236

| Gruppe | Pfad | Bemerkung |
| --- | --- | --- |
| Liste | Status setzen | Öffnet den Dialog **Status setzen**, in dem Sie den Status der Glasart wählen:<ul><li>in Produktion</li><li>produziert</li><li>versandfertig</li><li>ausgeliefert</li></ul> |
| | Arbeitsplan > Maschinen-Umlastung | Öffnet den Dialog **Umlastung** zur Maschinenumlastung.<br>⇨ Kapazitätsplanung: Softwarereferenz, "Maschinenumlastung" auf Seite E-618<br>Die Ergebnisse der Maschinenzuordnung im Rahmen der Einlastung werden überschrieben. |
| | Arbeitsplan > Terminumlastung | Öffnet den Dialog **Umlastung** zur Terminumlastung.<br>⇨ Kapazitätsplanung: Softwarereferenz, "Umlastung" auf Seite E-613<br>Die Ergebnisse der Maschinenzuordnung im Rahmen der Einlastung werden überschrieben. |
| | Arbeitsplan > Vorgabezeiten ändern | Öffnet den Dialog **Vorgabezeiten ändern**, in dem Sie Vorgabezeiten ändern können.<br>⇨ "Vorgabezeiten ändern" auf Seite C-208<br>Die Ergebnisse der Kapazitätsplanung im Rahmen der Einlastung werden überschrieben. |
| | Arbeitsplan > Bearbeitungs-Termin schützen | Schützt den Bearbeitungstermin für die markierten Bearbeitungen.<br>Die Ergebnisse der Kapazitätsplanung im Rahmen der Einlastung werden überschrieben. |
| | Arbeitsplan > Bearbeitungs-Termin Schutz aufheben | Hebt den Bearbeitungstermin-Schutz für die markierten Bearbeitungen auf.<br>Die Ergebnisse der Kapazitätsplanung im Rahmen der Einlastung werden überschrieben. |

### Schaltflächen
- **[Lauf]** Bildet aus den markierten Aufträgen, Positionen oder Teilen einen Lauf.
- **[Glasarten]** Zeigt die Glasarten der markierten Aufträge an.
- **[Details]** Zeigt die Details der markierten Aufträge an.

## Vorgabezeiten ändern

**Navigation:**
Bearbeitungen > Kontextmenü > Arbeitsplan > Vorgabezeiten ändern

*(Abb. C-43 Vorgabezeiten ändern)*

Im Dialog **Vorgabezeiten ändern** können Sie Vorgabezeiten für Bearbeitungen ändern.

> **Vorgabezeiten ändern**
> Die errechneten Vorgabezeiten des A+W Capacity Planner werden für die jeweilige Auswahl überschrieben, wenn Sie im Dialog Vorgabezeiten ändern einen Wert festlegen.
> Die hinterlegten Vorgabezeitformeln in den Stammdaten der Kapazitätsplanung sind von dieser Änderung nicht betroffen.

- **Faktor:** Der Faktor, um den die Vorgabezeit verändert werden soll.
- **[OK]:** Speichert die Daten.
- **[Abbrechen]:** Schließt den Dialog, ohne die Daten zu speichern.

# Glasarten, Details, BDE und Lose

In diesem Kapitel finden Sie Informationen zu allen Dialogen, mit denen Sie sich zu Glasarten, Details, BDE und Losen einen Überblick verschaffen.

Das Kapitel enthält folgende Themen:
- "Glasarten" auf Seite C-210
- "Details" auf Seite C-213
- "BDE" auf Seite C-217
- "Lose" auf Seite C-221

## Glasarten

**Navigation:**
- Anzeigen > Aufträge > Kontextmenü > Glasarten
- Anzeigen > Töpfe > Kontextmenü > Glasarten
- Anzeigen > Läufe > Kontextmenü > Glasarten
- Anzeigen > Füllaufträge > Kontextmenü > Glasarten
- Bearbeitungen > Kontextmenü > Glasarten
- Details > Kontextmenü > Glasarten
- Lose > Kontextmenü > Glasarten
- BDE > Kontextmenü > Glasarten

*(Abb. C-44 Glasarten - Typen (Beispiel))*

Mit dem Dialog **Glasarten** können Sie sich in einer Übersicht die enthaltenen Glasarten ausgewählter Aufträge bzw. Positionen anzeigen lassen und einen Lauf bilden. Dieser erscheint dann im Dialog **Läufe**.

Sie können die Register und Spalten im Dialog Glasarten nach Ihren Bedürfnissen anpassen, sodass genau die Informationen angezeigt werden, die Sie benötigen. Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.

Das Register **Typen** enthält z. B. folgende Spalten:
- **Lauf:** Nummer des Laufs.
- **Glasart:** Bezeichnung der Glasart, die im Auftrag bzw. der Position enthalten ist.
- **Dicke:** Dicke der Scheiben.
- **Menge:** Anzahl der jeweiligen Glasart.
- **im ISO:** Anzahl der Scheiben, die für ISO verwendet werden.
- **im ESG:** Anzahl der Scheiben, die für ESG verwendet werden.
- **im VSG:** Anzahl der Scheiben, die für VSG verwendet werden.

> **Datenbank-Informationen von Spalten**
> Mit einem Rechtsklick auf eine Spalte und der Option **Definition anzeigen** öffnen Sie den Dialog **Spaltendefinition**. Im Dialog Spaltendefinition finden Sie die jeweiligen Datenbank-Informationen einer Spalte.
> ⇨ "Spaltendefinition" auf Seite C-229

### Summenzeile
- **Stück:** Anzahl der Scheiben in den markierten Aufträgen bzw. Positionen.
- **Dauer gesamt:** Gesamte Bearbeitungsdauer der markierten Aufträge bzw. Positionen. Einheit: Stunden.
- **Fläche:** Gesamtfläche aller markierten Aufträge bzw. Positionen. Einheit: Quadratmeter.

### Filter
**[Filter hinzufügen]** Fügt einen Filter ein.

**Dropdown-Menü:** Sie haben im Dropdown-Menü des Filters folgende Optionen:
- **Klick:** Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
- **Rechtsklick:** Öffnet den Dialog **(Filter Name)**. Mit der Schaltfläche **Verwalten** gelangen Sie in den Dialog **Filter-Definition**, in dem Sie den jeweiligen Filter bearbeiten.
  ⇨ "Filter-Definition" auf Seite C-231

### Kontextmenüs
In folgenden Bereichen des Dialogs **Glasarten** werden Kontextmenüs angeboten:
- Register
- Spalten
- Liste
- Summenzeile
- Filter

Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen, sind im Kapitel Übergreifende Kontextmenüs gelistet.
⇨ "Übergreifende Kontextmenüs" auf Seite C-236

| Gruppe | Pfad | Bemerkung |
| --- | --- | --- |
| Liste | Sonderglas > Hinzufügen | Öffnet den Dialog **Sonderglas-Lauf bilden**. ⇨ "Sonderglas-Lauf bilden" auf Seite C-189 |
| | Sonderglas > Entfernen | Derzeit nicht genutzt. |
| | Status setzen | Öffnet den Dialog **Status setzen**, in dem Sie den Status der Glasart wählen: <ul><li>in Produktion</li><li>produziert</li><li>versandfertig</li><li>ausgeliefert</li></ul> |
| | Freie Formen | Öffnet den **A+W CAD Designer (Shapes)** zur Nachbearbeitung der Modell-Daten. |
| | Maschinen-Umlastung | Öffnet den Dialog **Maschinenumlastung** aus der Kapazitätsplanung. ⇨ Kapazitätsplanung: Softwarereferenz, "Maschinenumlastung" auf Seite E-618. Die Ergebnisse der Maschinenzuordnung im Rahmen der Einlastung werden überschrieben. |

### Schaltflächen
- **[Lauf]:** Bildet aus den markierten Aufträgen, Positionen oder Teilen einen Lauf.
- **[Glasarten]:** Zeigt die Glasarten der markierten Aufträge bzw. Positionen an.
- **[Details]:** Zeigt die Details der markierten Aufträge bzw. Positionen an.

## Details

**Navigation:**
- Anzeigen > Aufträge > Details
- Anzeigen > Töpfe > Kontextmenü > Details
- Anzeigen > Läufe > Kontextmenü > Details
- Anzeigen > Füllaufträge > Kontextmenü > Details
- Glasarten > Kontextmenü > Details
- Bearbeitungen > Kontextmenü > Details
- BDE > Kontextmenü > Details
- Lose > Kontextmenü > Details

*(Abb. C-45 Details (Beispiel))*

Mit dem Dialog **Details** können Sie sich Details zu ausgewählten Aufträgen, Positionen, Teilen, Läufen oder Töpfen anzeigen lassen. Sie können den Dialog **Details** aus jeder Ansicht in der Grobplanung öffnen.

Sie können die Register und Spalten im Dialog **Details** nach Ihren Bedürfnissen anpassen, sodass genau die Informationen angezeigt werden, die Sie benötigen. Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.

Der Dialog **Details** enthält z. B. folgende Spalten:
- **SN Info:** Zeigt den Modellstatus und die damit verbundene Geometrieberechnung im Rahmen der Einlastung. Folgende Anzeigen sind möglich:
    - 0: Status ok.
    - Nummer: Es liegt ein Fehler vor.
- **Storno:** Angabe, ob der Auftrag im ERP-System storniert wurde.
- **Auftrag:** Nummer des Auftrags.
- **Lauf:** Nummer des Laufs.
- **Liefertermin:** Liefertermin des Auftrags.
- **Produktionstermin:** Produktionstermin des Auftrags, der Position, der Einheit oder des Teils.
- **Summe ISO:** Anzahl der ISO-Scheiben, die der Auftrag enthält.
- **Summe [teil] mattiert:** Anzahl der Scheiben, die mattiert oder teilmattiert werden.
- **Summe VSG:** Anzahl der VSG-Scheiben im Auftrag bzw. in der Position.
- **Summe ESG:** Anzahl der ESG-Scheiben im Auftrag bzw. in der Position.
- **Summe Sprossen:** Anzahl der Sprossen im Auftrag.
- **Summe Modelle:** Anzahl der Modelle im Auftrag.
- **Summe 3-Fach-ISO:** Anzahl der 3-fach-ISO-Scheiben im Auftrag.
- **Summe Stufen:** Anzahl der Stufen-ISO oder Stufen-VSG im Auftrag.

> **Datenbank-Informationen von Spalten**
> Mit einem Rechtsklick auf eine Spalte und der Option **Definition anzeigen** öffnen Sie den Dialog **Spaltendefinition**. Im Dialog **Spaltendefinition** finden Sie die jeweiligen Datenbank-Informationen einer Spalte.
> ⇨ "Spaltendefinition" auf Seite C-229

### Summenzeile
- **Summe Stück:** Summe der Teile in den markierten Aufträgen bzw. Positionen.
- **Modelle:** Anzahl der in den markierten Aufträgen bzw. Positionen enthaltenen Modelle.
- **Fläche Mod:** Gesamtfläche der Modelle in den markierten Aufträgen bzw. Positionen. Einheit: Quadratmeter.

### Filter
- **[Filter hinzufügen]:** Fügt einen Filter ein.
- **Dropdown-Menü:** Sie haben im Dropdown-Menü des Filters folgende Optionen:
    - **Klick:** Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
    - **Rechtsklick:** Öffnet den Dialog **(Filter Name)**. Mit der Schaltfläche **Verwalten** gelangen Sie in den Dialog **Filter-Definition**, in dem Sie den jeweiligen Filter bearbeiten.
      ⇨ "Filter-Definition" auf Seite C-231

### Kontextmenüs
In folgenden Bereichen des Dialogs **Details** werden Kontextmenüs angeboten:
- Register
- Spalten
- Liste
- Summenzeile
- Filter

Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen, sind im Kapitel Übergreifende Kontextmenüs gelistet.
⇨ "Übergreifende Kontextmenüs" auf Seite C-236

| Gruppe | Pfad | Bemerkung |
| --- | --- | --- |
| Liste | Zurück in den Pool | Gibt die ausgewählten Aufträge zurück in den Dialog **Aufträge**. ⇨ "Aufträge" auf Seite C-156 |
| | Status setzen | Öffnet den Dialog **Status setzen**, in dem Sie den Status des Laufs wählen: <ul><li>in Produktion</li><li>produziert</li><li>versandfertig</li><li>ausgeliefert</li></ul> |
| | Arbeitsplan > Maschinen-Umlastung | Öffnet den Dialog **Umlastung** zur Maschinenumlastung. ⇨ Kapazitätsplanung: Softwarereferenz, “Maschinenumlastung" auf Seite E-618. Die Ergebnisse der Maschinenzuordnung im Rahmen der Einlastung werden überschrieben. |
| | Arbeitsplan > Maschinen-Zuordnung | Führt die Maschinenzuordnung für markierte Aufträge bzw. Positionen erneut durch. Die Ergebnisse der Maschinenzuordnung im Rahmen der Einlastung werden überschrieben. |
| | Arbeitsplan > Arbeitsplan neu berechnen | Zur Zeit nicht genutzt |
| | Sprossen-Druck | Startet den Druck von Produktionspapieren für die Sprossenproduktion bzw. -bearbeitung. |
| | Vorgabezeiten ändern | Öffnet den Dialog **Vorgabezeiten ändern**, in dem Sie Vorgabezeiten ändern können. ⇨ "Vorgabezeiten ändern" auf Seite C-208. Die Ergebnisse der Kapazitätsplanung im Rahmen der Einlastung werden überschrieben. |

### Schaltflächen
- **[Lauf]:** Bildet aus den markierten Aufträgen, Positionen oder Teilen einen Lauf.
- **[Glasarten]:** Zeigt die Glasarten der markierten Aufträge bzw. Positionen an.
- **[Details]:** Zeigt die Details der markierten Aufträge bzw. Positionen an.

## BDE

**Navigation:**
- Anzeigen > Aufträge > Kontextmenü > Bearbeitungen > Kontextmenü > BDE
- Anzeigen > Töpfe > Kontextmenü > Bearbeitungen > Kontextmenü > BDE
- Anzeigen > Läufe > Kontextmenü > BDE
- Glasarten > Kontextmenü > BDE
- Details > Kontextmenü > BDE

*(Abb. C-46 BDE - Produkt (Beispiel))*

Im Dialog **BDE** bekommen Sie einen Überblick über Informationen, die sich auf die Betriebsdatenerfassung beziehen.
Sie können die Aufträge nach unterschiedlichen Kriterien sortieren und bearbeiten. Folgende Bestandteile des Dialogs BDE können Sie frei konfigurieren:
- Register
- Spalten
- Summenzeile
- Filter

Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.

Das Register **Produkt** enthält z. B. folgende Spalten:
- **Auftrag:** Nummer des Auftrags.
- **Pos (int Pos):** Interne Positionsnummer aus der Auftragserfassung.
- **Teile-Nr.:** Teilenummer des jeweiligen Teils.
- **Artikelbezeichnung:** Bezeichnung des jeweiligen Artikels.
- **Etikett-Nr.:** Etikettnummer des jeweiligen Teils.

> **Datenbank-Informationen von Spalten**
> Mit einem Rechtsklick auf eine Spalte und der Option **Definition anzeigen** öffnen Sie den Dialog **Spaltendefinition**. Im Dialog **Spaltendefinition** finden Sie die jeweiligen Datenbank-Informationen einer Spalte.
> ⇨ "Spaltendefinition" auf Seite C-229

### Summenzeile
In der Summenzeile können Sie sich verschiedene Summen anzeigen lassen, Sie bekommen z. B. folgende Informationen angezeigt:
- **Dauer gesamt:** Gesamte Bearbeitungsdauer der markierten Aufträge bzw. Positionen. Einheit: Stunden.
- **Summe Stück:** Summe der Teile in den markierten Aufträgen bzw. Positionen.

### Filter
**[Filter hinzufügen]** Fügt einen Filter ein.

**Dropdown-Menü** Sie haben im Dropdown-Menü des Filters folgende Optionen:
- **Klick:** Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
- **Rechtsklick:** Öffnet den Dialog **(Filter Name)**. Mit der Schaltfläche **Verwalten** gelangen Sie in den Dialog **Filter-Definition**, in dem Sie den jeweiligen Filter bearbeiten.
  ⇨ "Filter-Definition" auf Seite C-231

### Kontextmenüs
In folgenden Bereichen des Dialogs BDE werden Kontextmenüs angeboten:
- Register
- Spalten
- Liste
- Summenzeile
- Filter

Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen, sind im Kapitel Übergreifende Kontextmenüs gelistet.
⇨ "Übergreifende Kontextmenüs" auf Seite C-236

| Gruppe | Pfad | Bemerkung |
| --- | --- | --- |
| Liste | Zurück in den Pool | Gibt die ausgewählten Aufträge bzw. Positionen zurück in den Dialog **Aufträge**. |
| | Status setzen | Öffnet den Dialog **Status setzen**, in dem Sie den Status des Laufs wählen:<ul><li>in Produktion</li><li>produziert</li><li>versandfertig</li><li>ausgeliefert</li></ul> |
| | Arbeitsplan > Maschinen-Umlastung | Öffnet den Dialog **Umlastung** zur Maschinenumlastung. ⇨ Kapazitätsplanung: Softwarereferenz, "Maschinenumlastung" auf Seite E-618. Die Ergebnisse der Maschinenzuordnung im Rahmen der Einlastung werden überschrieben. |
| | Arbeitsplan > Maschinen-Zuordnung | Führt die Maschinenzuordnung für markierte Aufträge bzw. Positionen erneut durch. Die Ergebnisse der Maschinenzuordnung im Rahmen der Einlastung werden überschrieben. |
| | Arbeitsplan > Arbeitsplan neu berechnen | Zur Zeit nicht genutzt. |
| | Vorgabezeiten ändern | Öffnet den Dialog **Vorgabezeiten ändern**, in dem Sie Vorgabezeiten ändern können. ⇨ "Vorgabezeiten ändern" auf Seite C-208. Die Ergebnisse der Kapazitätsplanung im Rahmen der Einlastung werden überschrieben. |

### Schaltflächen
- **[Lauf]:** Zur Zeit nicht aktiv.
- **[Glasarten]:** Zeigt die Glasarten der markierten Aufträge bzw. Positionen an.
- **[Details]:** Zeigt die Details der markierten Aufträge bzw. Positionen an.

## Lose

**Navigation:**
- Anzeigen > Läufe > Kontextmenü > Lose
- Details > Kontextmenü > Lose

*(Abb. C-47 Lose - Zuschnitt (Beispiel))*

Im Dialog **Lose** bekommen Sie einen Überblick über die erstellten Lose der ausgewählten Läufe.

Sie können die Lose nach unterschiedlichen Kriterien sortieren und bearbeiten. Die Steuerung des Dialogs **Lose** erfolgt vorrangig über Kontextmenüs. Folgende Bestandteile des Dialogs **Lose** können Sie frei konfigurieren:
- Register
- Spalten
- Summenzeile
- Filter

Das Register **Zuschnitt** enthält z. B. folgende Spalten:
- **Lostyp:** Gibt den Typ des Loses an.
- **Los:** Bezeichnung des Loses.
- **Bock:** Gestell, auf das das Los geplant wird.
- **Glasart:** Nummer der Glasart.
- **Glasart-Bez.:** Bezeichnung der Glasart des Loses.
- **Stück:** Anzahl der Positionen bzw. Teile im Los.

> **Datenbank-Informationen von Spalten**
> Mit einem Rechtsklick auf eine Spalte und der Option **Definition anzeigen** öffnen Sie den Dialog **Spaltendefinition**. Im Dialog **Spaltendefinition** finden Sie die jeweiligen Datenbank-Informationen einer Spalte.
> ⇨ "Spaltendefinition" auf Seite C-229

### Summenzeile
In der Summenzeile können Sie sich verschiedene Summen anzeigen lassen, Sie bekommen z. B. folgende Informationen angezeigt:
- **Dauer gesamt:** Gesamte Bearbeitungsdauer der markierten Aufträge bzw. Positionen. Einheit: Stunden.
- **Stück:** Anzahl der Einzelscheiben oder Stückartikel in den markierten Aufträgen bzw. Positionen.

### Filter
- **[Filter hinzufügen]:** Fügt einen Filter ein.
- **Dropdown-Menü:** Sie haben im Dropdown-Menü des Filters folgende Optionen:
    - **Klick:** Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
    - **Rechtsklick:** Öffnet den Dialog **(Filter Name)**. Mit der Schaltfläche **Verwalten** gelangen Sie in den Dialog **Filter-Definition**, in dem Sie den jeweiligen Filter bearbeiten.
      ⇨ "Filter-Definition" auf Seite C-231

### Kontextmenüs
In folgenden Bereichen des Dialogs **Lose** werden Kontextmenüs angeboten:
- Register
- Spalten
- Liste
- Summenzeile
- Filter

Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen, sind im Kapitel Übergreifende Kontextmenüs gelistet.
⇨ "Übergreifende Kontextmenüs" auf Seite C-236

| Gruppe | Pfad | Bemerkung |
| --- | --- | --- |
| Liste | Status setzen | Öffnet den Dialog **Status setzen**, in dem Sie den Status des Laufs wählen: <ul><li>in Produktion</li><li>produziert</li><li>versandfertig</li><li>ausgeliefert</li></ul> |

### Schaltflächen
- **[Lauf]:** Zur Zeit nicht aktiv.
- **[Glasarten]:** Zeigt die Glasarten der markierten Lose an.
- **[Details]:** Zeigt die Details der markierten Lose an.

# Übergreifende Dialoge

In diesem Kapitel finden Sie Informationen zu allen Dialogen, die Sie übergreifend in der gesamten Arbeitsvorbereitung finden. Sie können Eigenschaften von Dialogen bearbeiten, Dokumentenverknüpfungen verwalten und Entschichtungsflächen bearbeiten.

Das Kapitel enthält folgende Themen:
- "Eigenschaften von (Register)" auf Seite C-228
- "Spaltendefinition" auf Seite C-229
- "(Filter Name)" auf Seite C-230
- "Filter-Definition" auf Seite C-231
- "Dokumentenverknüpfungen" auf Seite C-233
- "Entschichtungsflächen" auf Seite C-234

## Arbeitsplan

**Navigation:**
Produktionsmonitor > Kontextmenü – Schicht > Arbeitsplan

*(Abb. C-48 Arbeitsplan (Beispiel))*

Mit dem Dialog **Arbeitsplan** können Sie sich aus dem Produktionsmonitor heraus einen Überblick verschaffen. Der Arbeitsplan zeigt die geplanten Läufe auf einer Maschine, bzw. in einer Schicht.

Sie können die Register und Spalten im Dialog Arbeitsplan nach Ihren Bedürfnissen anpassen, sodass genau die Informationen angezeigt werden, die Sie benötigen. Die Steuerung des Dialogs erfolgt zum größten Teil über Kontextmenüs.

Das Register **Details** enthält z. B. folgende Spalten:
- **Lauf:** Angabe des Laufs.
- **Auftrag:** Angabe des Auftrags.
- **Pos (int Pos):** Angabe der Positionsnummer.
- **Teile-Nr:** Angabe der Teilenummer.
- **Sequenz:** Sequenznummer der Bearbeitung.
- **Bearbnr:** Nummer der Bearbeitung.
- **MZO-Maschine:** Logische Maschine, auf der die Bearbeitung durchgeführt wird.

> **Datenbank-Informationen von Spalten**
> Mit einem Rechtsklick auf eine Spalte und der Option **Definition anzeigen** öffnen Sie den Dialog **Spaltendefinition**. Im Dialog **Spaltendefinition** finden Sie die jeweiligen Datenbank-Informationen einer Spalte.
> ⇨ "Spaltendefinition" auf Seite C-229

### Summenzeile
In der Summenzeile können Sie sich verschiedene Summen anzeigen lassen, Sie bekommen z. B. folgende Informationen angezeigt:
- **Summe Stück:** Summe der Teile in den markierten Aufträgen bzw. Positionen.
- **Dauer gesamt:** Gesamte Bearbeitungsdauer der markierten Aufträge bzw. Positionen. Einheit: Stunden.

### Filter
- **[Filter hinzufügen]:** Fügt einen Filter ein.
- **Dropdown-Menü:** Sie haben im Dropdown-Menü des Filters folgende Optionen:
    - **Klick:** Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
    - **Rechtsklick:** Öffnet den Dialog **(Filter Name)**. Mit der Schaltfläche **Verwalten** gelangen Sie in den Dialog **Filter-Definition**, in dem Sie den jeweiligen Filter bearbeiten.
      ⇨ "Filter-Definition" auf Seite C-231

### Kontextmenüs
In folgenden Bereichen des Dialogs **Arbeitsplan** werden Kontextmenüs angeboten:
- Register
- Spalten
- Liste
- Summenzeile
- Filter

Kontextmenüs, die im gesamten Bereich der Arbeitsvorbereitung vorkommen, sind im Kapitel Übergreifende Kontextmenüs gelistet.
⇨ "Übergreifende Kontextmenüs" auf Seite C-236

| Gruppe | Pfad | Bemerkung |
| --- | --- | --- |
| Liste | Status setzen | Öffnet den Dialog **Status setzen**, in dem Sie den Status des Laufs wählen:<ul><li>in Produktion</li><li>produziert</li><li>versandfertig</li><li>ausgeliefert</li></ul> |
| | Arbeitsplan > Maschinen-Umlastung | Öffnet den Dialog **Umlastung** zur Maschinenumlastung.<br>⇨ Kapazitätsplanung: Softwarereferenz, "Maschinenumlastung" auf Seite E-618<br>Die Ergebnisse der Maschinenzuordnung im Rahmen der Einlastung werden überschrieben. |
| | Arbeitsplan > Terminumlastung | Öffnet den Dialog **Umlastung** zur Terminumlastung.<br>⇨ Kapazitätsplanung: Softwarereferenz, "Maschinenumlastung" auf Seite E-618<br>Die Ergebnisse der Maschinenzuordnung im Rahmen der Einlastung werden überschrieben. |
| | Arbeitsplan > Vorgabezeiten ändern | Öffnet den Dialog **Vorgabezeiten ändern**, in dem Sie Vorgabezeiten ändern können.<br>⇨ "Vorgabezeiten ändern" auf Seite C-208<br>Die Ergebnisse der Kapazitätsplanung im Rahmen der Einlastung werden überschrieben. |
| | Arbeitsplan > Bearbeitungs-Termin schützen | Schützt den Bearbeitungstermin für die markierten Bearbeitungen. Die Ergebnisse der Kapazitätsplanung im Rahmen der Einlastung werden überschrieben. |
| | Arbeitsplan > Bearbeitungs-Termin Schutz aufheben | Hebt den Bearbeitungstermin-Schutz für die markierten Bearbeitungen auf. Die Ergebnisse der Kapazitätsplanung im Rahmen der Einlastung werden überschrieben. |
| | Fertigmelden | Die Läufe, Aufträge oder Positionen werden auf den Status **Fertig** gesetzt. |

### Schaltflächen
- **[Lauf]:** Bildet aus den markierten Läufen, Aufträgen oder Positionen einen Lauf.
- **[Glasarten]:** Zeigt die Glasarten der markierten Läufe, Aufträge oder Positionen an.
- **[Details]:** Zeigt die Details der markierten Läufe, Aufträge oder Positionen an.

> **Daten exportieren**
> Über **Anzeigen > Exportieren** können Sie die Daten in eine CSV-Datei exportieren.

## Eigenschaften von (Register)

**Navigation:**
- Anzeigen > Aufträge > Kontextmenü – Register > Einfügen
- Anzeigen > Aufträge > Kontextmenü – Register > Eigenschaften

*(Abb. C-49 Eigenschaften von (Register))*

Im Dialog **Eigenschaften von (Register)** können Sie neue Register anlegen oder bestehende Register ändern.

- **Registertext:** Titel des Registers.
- **Beschreibung:** Beschreibung des Registers.
- **Systemweite Anzeige:** Checkbox mit folgenden Funktionen:
    - ☐ Das Register wird nur in diesem Dialog angezeigt.
    - ☑ Das Register wird systemweit angezeigt.
- **[OK]:** Speichert die Daten.
- **[Abbrechen]:** Schließt den Dialog, ohne die Daten zu speichern.

## Spaltendefinition

**Navigation:**
- Anzeigen > Aufträge > Kontextmenü – Spalten > Definition anzeigen
- Anzeigen > Töpfe > Kontextmenü – Spalten > Definition anzeigen
- Anzeigen > Läufe > Kontextmenü – Spalten > Definition anzeigen
- Auftragsübersicht > Kontextmenü – Spalten > Definition anzeigen
- Glasarten > Kontextmenü – Spalten > Definition anzeigen
- Bearbeitungen > Kontextmenü – Spalten > Definition anzeigen
- Lose > Kontextmenü - Spalten > Definition anzeigen
- BDE > Kontextmenü – Spalten > Definition anzeigen
- Details > Kontextmenü – Spalten > Definition anzeigen

*(Abb. C-50 Spaltendefinition)*

Im Dialog **Spaltendefinition** werden die Eigenschaften einer Spalte angezeigt.

- **Titel:** Name der Spalte.
- **Format:** Format der Spalte, z. B. das Datums-Format.
- **Menü:** Gibt an, in welchem Bereich des Kontextmenüs die jeweilige Auswahl hinterlegt ist.
- **SQL-Def.:** Name der Datenbank-Tabelle und des Datenbank-Felds. Diese werden ausführlich in der A+W Datenbank-Dokumentation beschrieben.
- **SQL-Definition Teile:** Name der Datenbank-Tabelle und des Datenbank-Felds, wenn Sie im Dialog **Auftragsübersicht** die Anzeige-Option **Teile** gewählt haben. Die Datenbanktabellen und -felder sind ausführlich in der A+W Datenbank-Dokumentation beschrieben.
- **SQL-Definition Bearbeitungen:** Name der Datenbank-Tabelle und des Datenbank-Felds, wenn Sie im Dialog **Auftragsübersicht** die Anzeige-Option **Bearbeitungen** gewählt haben. Die Datenbanktabellen und -felder sind ausführlich in der A+W Datenbank-Dokumentation beschrieben.
- **[OK]:** Schließt den Dialog.

## (Filter Name)

**Navigation:**
Anzeigen > Aufträge > Kontextmenü – Filter

*(Abb. C-51 (Filter Name))*

Im Dialog **(Filter Name)** gelangen Sie zur Filter-Definition und Sie können Filter löschen.

- **Verwalten:** Öffnet den Dialog **Filter-Definition**, in dem Sie Filter bearbeiten.
  ⇨ "Filter-Definition" auf Seite C-231
- **Entfernen:** Löscht den ausgewählten Filter.
- **[OK]:** Schließt den Dialog.
- **[Abbrechen]:** Schließt den Dialog, ohne die Daten zu speichern.

## Filter-Definition

**Navigation:**
Anzeigen > Aufträge > Kontextmenü – Filter > (Filter Name) > [Verwalten]

*(Abb. C-52 Filter-Definition)*

Im Dialog **Filter-Definition** können Sie Filter definieren und bearbeiten.

- **Definierte Filter:** Liste der definierten Filter.
- **Name:** Bezeichnung des jeweiligen Filters.
- **Beschreibung:** Beschreibung des jeweiligen Filters.
- **SQL-Bedingung:** Hinterlegte Formel bzw. Bedingung mit Referenz auf die entsprechenden Datenbanktabellen und -felder.
- **Standard-Parameter:** Angabe eines Standard-Werts, z. B. ein Standard-Datum, auf das zurückgegriffen wird, wenn die entsprechenden Datenbanktabellen bzw. -felder keinen Wert ermitteln.
- **Zulässig für Ansicht:** Auswahl, in welchem Dialog der Filter zur Verfügung steht. Zur Auswahl stehen:
    - Pool-Ansicht
    - Topf-Ansicht
    - Lauf-Ansicht
    - Füllauftrags-Ansicht
    - Details
    - Vorauswahl BDE-Ansicht
    - Bestellteile-Topf
    - Glasarten-Ansicht
    - Produktionslos-Ansicht
    - Bearbeitungs-Ansicht
    - BDE
    - Packmittel
    - Bruchstatistik
    - Produktionsstatistik
    - Produktionsübersicht
- **Speichern:** Speichert die Daten.
- **Löschen:** Löscht den markierten Filter.
- **Exportieren:** Öffnet den Dialog **Speichern unter**, in dem Sie den jeweiligen Filter speichern können.
- **Importieren:** Öffnet den Dialog **Öffnen**, in dem Sie Filter zum Importieren auswählen.
- **[Schließen]:** Schließt den Dialog, ohne die Daten zu speichern.

## Dokumentenverknüpfungen

**Navigation:**
- Anzeigen > Aufträge > Kontextmenü > Zugehörige Dokumente
- Anzeigen > Töpfe > Kontextmenü > Zugehörige Dokumente
- Anzeigen > Läufe > Kontextmenü > Zugehörige Dokumente
- Anzeigen > Füllaufträge > Kontextmenü > Zugehörige Dokumente
- Glasarten > Kontextmenü > Zugehörige Dokumente
- Bearbeitungen > Kontextmenü > Zugehörige Dokumente
- BDE > Kontextmenü > Zugehörige Dokumente
- Lose > Kontextmenü > Zugehörige Dokumente

*(Abb. C-53 Dokumentenverknüpfungen)*

Im Dialog **Dokumentenverknüpfungen** können Sie Aufträge mit Dokumenten, wie z. B. speziellen Lieferbedingungen, verknüpfen und sehen, mit welchen Dokumenten ein Auftrag bzw. eine Position verknüpft ist.

- **Auftrag:** Ausgewählte Aufträge.
- **Position:** Anzahl der Positionen pro Auftrag.
- **Typ:** Typ des verknüpften Dokuments. Sie geben den Dokumententyp mit einer frei wählbaren Zahl an. Sie legen auch fest, welcher Dokumententyp einer Zahl zugeordnet ist, z. B 3 für Textdokumente.
- **Dokument:** Pfad des verknüpften Dokuments.
- **[Öffnen]:** Öffnet ein angehängtes Dokument.
- **[Löschen]:** Löscht die Dokumentenverknüpfung.
- **[Neu]:** Erstellt eine neue Dokumentenverknüpfung.
- **[Ändern]:** Öffnet den Dialog **Dokumentenverknüpfung (Auftragsnummer)**, um die Daten zu ändern.
- **[Schließen]:** Schließt den Dialog.

## Entschichtungsflächen

**Navigation:**
- Anzeigen > Aufträge > Kontextmenü > Nacherfassung > Entschichtung
- Anzeigen > Töpfe > Kontextmenü > Nacherfassung > Entschichtung
- Anzeigen > Läufe > Kontextmenü > Nacherfassung > Entschichtung
- Anzeigen > Füllauftr. > Kontextmenü > Nacherfassung > Entschichtung
- Details > Kontextmenü > Nacherfassung > Entschichtung
- BDE > Kontextmenü > Nacherfassung > Entschichtung

*(Abb. C-54 Entschichtungsflächen)*

Im Dialog **Entschichtungsflächen** können Sie nachträglich die Flächen angeben, die entschichtet werden sollen.

### Kopfzeile
In der Kopfzeile werden folgende Informationen zur jeweiligen Position angezeigt:
- Auftrag
- Position
- Unterposition
- Teilenummer
- Glasart
- Modell

### Navigationsfenster
Im Navigationsfenster bekommen Sie die markierten Entschichtungsflächen angezeigt.

### Navigation
1. Abstand der Entschichtungsfläche von Ecke 1. Einheit: Millimeter.
2. Abstand der Entschichtungsfläche von Ecke 2. Einheit: Millimeter.
- **[Pfeil nach links]:** Ändert die Lage der Ecken 1 und 2 auf der Scheibe.
- **[Pfeil nach rechts]:** Ändert die Lage der Ecken 1 und 2 auf der Scheibe.

### Schaltflächen
- **[OK]:** Speichert die Daten.
- **[Abbrechen]:** Schließt den Dialog, ohne die Daten zu speichern.

# Übergreifende Kontextmenüs

In diesem Kapitel finden Sie Informationen zu allen Kontextmenüs, die übergreifend im gesamten Bereich der Arbeitsvorbereitung vorkommen.
Die Kontextmenüs finden Sie in folgenden Dialogbereichen:
- Register
- Spalten
- Liste
- Summenzeile
- Filter

| Gruppe | Pfad | Bemerkung |
| --- | --- | --- |
| **Register** | Speicherautomatik | Änderungen am Register werden automatisch gespeichert. |
| | Speichern | Manuelles Speichern von Änderungen am Register. |
| | Einfügen | Öffnet den Dialog **Eigenschaften von (Register)**. ⇨ "Eigenschaften von (Register)" auf Seite C-228 |
| | Löschen | Löscht das markierte Register. |
| | Eigenschaften | Öffnet den Dialog **Eigenschaften von (Register)**, in dem Sie die Eigenschaften des Registers ändern. ⇨ "Eigenschaften von (Register)" auf Seite C-228 |
| | Import | Öffnet den Dialog **Importieren** eines Registers. |
| | Export | Öffnet den Dialog **Exportieren** eines Registers. |
| **Spalten** | Umsortieren | Spalte aufsteigend oder absteigend sortieren. Wirkt sich auf die ersten drei Spalten im Dialog aus. |
| | Formatieren | Format oder Einheit für die Spalten auswählen, z. B. Datumsformate oder Längen-Einheiten. |
| | Einfügen | Fügt eine neue Spalte ein. Verschiedene Kategorien stehen zur Verfügung. |
| | Einfügen > Felddefinitionen > Editieren | Öffnet den Dialog **Felddefinition**, in dem Sie Abfragen auf Datenbank-Tabellen und -Felder formulieren können. Diese Abfragen können Sie dann z. B. teile-, positions- oder auftragsbezogen als Spalte einfügen. ⇨ "Felddefinition" auf Seite C-201 |
| | Einfügen > Felddefinitionen > Importieren | Öffnet den Dialog **Importieren von Felddefinitionen**. |
| | Einfügen > Felddefinitionen > Exportieren | Öffnet den Dialog **Exportieren von Felddefinitionen**. |
| | Entfernen | Löscht die markierte Spalte. |
| | Ändern | Derzeit nicht genutzt. |
| | Definition anzeigen | Öffnet den Dialog **Spaltendefinition**, in dem Details zur jeweiligen Spalte angezeigt werden. ⇨ "Spaltendefinition" auf Seite C-229 |
| **Liste** | Lauf bilden | Öffnet den Dialog **Lauf-Bildung**. ⇨ "Lauf-Bildung" auf Seite C-187 |
| | Topf bilden | Öffnet den Dialog **Topf-Bildung**. ⇨ "Topf-Bildung" auf Seite C-180 |
| | Füllauftrag | Ändert den ausgewählten Auftrag zu einem Füllauftrag. ⇨ "Füllaufträge" auf Seite C-162 |
| | Packmittelgruppe bilden | Öffnet den Dialog **Packmittelgruppen**. |
| | Automatisch Packmittelgruppen bilden | Bildet automatisch Packmittelgruppen. |
| | Auftragsübersicht | Öffnet den Dialog **Auftragsübersicht**. ⇨ "Auftragsübersicht" auf Seite C-159 |
| | Positionen | Öffnet den Dialog **Positionen**. ⇨ "Positionen" auf Seite C-195 |
| | Glasarten | Öffnet den Dialog **Glasarten**. ⇨ "Glasarten" auf Seite C-210 |
| | Bearbeitungen | Öffnet den Dialog **Bearbeitungen**. ⇨ "Bearbeitungen" auf Seite C-205 |
| | Lose | Öffnet den Dialog **Lose**. ⇨ "Lose" auf Seite C-221 |
| | BDE | Öffnet den Dialog **BDE**. ⇨ "BDE" auf Seite C-217 |
| | Details | Öffnet den Dialog **Details**. ⇨ "Details" auf Seite C-213 |
| | Nacherfassung > Entschichtung | Öffnet den Dialog **Entschichtungsflächen**. ⇨ "Entschichtungsflächen" auf Seite C-234 |
| | Nacherfassung > Sprossen | Öffnet den **A+W CAD Designer (Shapes)** zur Nacherfassung von Sprossen. |
| | Nacherfassung > Freie Formen | Öffnet den **A+W CAD Designer (Bars)** zur Nachbearbeitung der Modell-Daten. |
| | Nacherfassung > Übermengen | Öffnet den Dialog **Übermengen-Editor** zur Nacherfassung von kaufmännischen und produktionstechnischen Übermengen. ⇨ “Übermengen-Editor" auf Seite C-165 |
| | Arbeitsplan > Maschinen-Umlastung | Öffnet den Dialog **Umlastung** zur Maschinenumlastung. ⇨ Kapazitätsplanung: Softwarereferenz, "Maschinenumlastung" auf Seite E-618. Die Ergebnisse der Maschinenzuordnung im Rahmen der Einlastung werden überschrieben. |
| | Arbeitsplan > Maschinen-Zuordnung | Führt die Maschinenzuordnung für markierte Aufträge bzw. Positionen erneut durch. Die Ergebnisse der Maschinenzuordnung im Rahmen der Einlastung werden überschrieben. |
| | Arbeitsplan > Arbeitsplan neu berechnen | Zur Zeit nicht genutzt. |
| | Positionen splitten | Öffnet den Dialog **Positionssplit**. ⇨ "Positionssplit" auf Seite C-199 |
| | Beschaffungsart ändern | Öffnet den Dialog **Änderung der Beschaffungsart**. ⇨ "Änderung der Beschaffungsart" auf Seite C-167. Die Option funktioniert ausschließlich bei ESG und VSG. |
| | Zugehörige Dokumente | Öffnet den Dialog **Dokumentenverknüpfungen**. ⇨ "Dokumentenverknüpfungen" auf Seite C-233 |
| **Summenzeile** | Umsortieren | Zur Zeit nicht genutzt. |
| | Formatieren | Format oder Einheit für die Spalten auswählen, z. B. Datumsformate oder Längen-Einheiten. |
| | Einfügen | Fügt ein neues Feld in die Summenzeile ein. Verschiedene Kategorien stehen zur Verfügung. |
| | Einfügen > Felddefinitionen > Editieren | Öffnet den Dialog **Felddefinition**, in dem Sie Abfragen auf Datenbank-Tabellen und -Felder formulieren können. Diese Abfragen können Sie dann z. B. teile-, positions- oder auftragsbezogen einfügen. ⇨"Felddefinition" auf Seite C-201 |
| | Einfügen > Felddefinitionen > Importieren | Öffnet den Dialog **Importieren von Felddefinitionen**. |
| | Einfügen > Felddefinitionen > Exportieren | Öffnet den Dialog **Exportieren von Felddefinitionen**. |
| **Filter** | | Öffnet den Dialog **(Filter Name)**. Mit der Schaltfläche **[Verwalten]** gelangen Sie zum Dialog **Filter-Definition**, in dem Sie Filter bearbeiten können. ⇨"Filter-Definition" auf Seite C-231 |

# Help Cards

## Informationen zu den Help Cards

Die Darstellungen in den Help Cards basieren auf der Auslieferversion A+W Production. Einzelne Schritte in den Workflows können je nach Konfiguration abweichen.

### In diesem Kapitel finden Sie folgende Themen:
- Informationen zu den Help Cards (C-243)
- Läufe (C-244)
    - Läufe bilden (C-245)
    - Läufe ergänzen (C-246)
    - Läufe zusammenfügen (C-247)
    - Läufe auflösen (C-248)
    - Aufträge aus Läufen entfernen (C-249)
    - Läufe archivieren oder löschen (C-250)
- Ansichten (C-251)
    - Spalte oder Summenzeile hinzufügen (C-252)

## Läufe

| Help Card | Themen |
| :--- | :--- |
| Läufe bilden | Sie erstellen einen Lauf. |
| Läufe ergänzen | Sie fügen einem bestehenden Lauf einen Auftrag hinzu. |
| Läufe zusammenfügen | Sie fügen zwei Läufe zu einem zusammen. |
| Läufe auflösen | Sie lösen einen Lauf auf. |
| Aufträge aus Läufen entfernen | Sie entfernen einen Auftrag aus einem Lauf. |
| Läufe archivieren oder löschen | Sie archivieren einen produzierten Lauf. |

### Läufe bilden (GP 01-001)

**Ziel der Handlung:** Sie erstellen einen Lauf.

**Workflow:**
1. Öffnen Sie die Ansicht, in der Sie einen Lauf erstellen möchten, z. B. **Anzeigen > Aufträge**.
2. Markieren Sie die gewünschten Aufträge oder Positionen, öffnen Sie das Kontext-Menü und wählen Sie **Lauf bilden**. Der Dialog **Lauf-Bildung** wird geöffnet.
3. A+W Production legt im Feld **Lauf** automatisch eine neue Laufnummer an.
4. Geben Sie im Feld **Bezeichnung** eine Bezeichnung für den Lauf ein.
5. Wählen Sie im Kalender-Feld **Produktionstermin** den Produktionsstart. **Hinweis:** Wenn Sie mit Kapazitätsplanung arbeiten, können Sie die Läufe auch aus dem Produktionsmonitor heraus bilden.
6. Wählen Sie nun den Produktionsstarttermin und die Produktionsschicht aus. Wenn Sie mit Kapazitätsplanung arbeiten, sollten Sie hier den durch die Kapazitätsplanung errechneten frühesten Starttermin und die entsprechende Schicht eintragen.
7. Mit der Checkbox **Auftrag zusammenhalten** bewirken Sie, dass alle verfügbaren Teile und Positionen in den Lauf gepackt werden, auch wenn Sie nur 1 Teil oder 1 Position ausgewählt haben. Sie vermeiden dadurch, etwas zu vergessen.
8. Klicken Sie auf **[OK]**, um die Daten zu speichern.
9. Der Lauf wurde gebildet und ist in der Ansicht **Läufe** gelistet.

### Läufe ergänzen (GP 01-002)

**Ziel der Handlung:** Sie fügen einem bestehenden Lauf einen Auftrag hinzu.

**Voraussetzungen:** Der Lauf muss angelegt sein.

**Workflow:**
1. Öffnen Sie die Ansicht, aus der heraus Sie einen Lauf ergänzen möchten, z. B. **Anzeigen > Aufträge**.
2. Markieren Sie den gewünschten Auftrag, öffnen Sie das Kontext-Menü und wählen Sie **Lauf bilden**. Der Dialog **Lauf-Bildung** wird geöffnet.
3. Wählen Sie einen bestehenden Lauf im Dropdown-Menü um den Auftrag / die Positionen einem Lauf hinzuzufügen.
4. Durch den bestehenden Lauf ist der Produktionsstarttermin bereits vordefiniert. Falls sich durch das Hinzufügen der neuen Aufträge / Positionen der Starttermin ändert, wählen Sie hier den neuen Starttermin aus (bitte ggf. die errechneten Termine der Kapazitätsplanung beachten).
5. Mit der Checkbox **Auftrag zusammenhalten** bewirken Sie, dass alle verfügbaren Teile und Positionen in den Lauf gepackt werden, auch wenn Sie nur 1 Teil oder 1 Position ausgewählt haben. Sie vermeiden dadurch, etwas zu vergessen.
6. Klicken Sie auf **[OK]**, um die Daten zu speichern.
7. Der Lauf wurde aktualisiert und ist in der Ansicht **Läufe** gelistet.

### Läufe zusammenfügen (GP 01-003)

**Ziel der Handlung:** Sie fügen zwei Läufe zu einem zusammen.

**Voraussetzungen:** Beide Läufe müssen angelegt sein.

**Workflow:**
1. Öffnen Sie die Ansicht **Läufe**.
2. Markieren Sie die Läufe, die Sie zu einem Lauf zusammen fassen möchten.
3. Öffnen Sie das Kontext-Menü und wählen Sie **Lauf bilden**. Der Dialog **Lauf-Bildung** wird geöffnet.
4. A+W Production legt im Feld **Lauf** automatisch eine neue Laufnummer an.
5. Geben Sie im Feld **Bezeichnung** eine Bezeichnung für den Lauf ein.
6. Durch die bestehenden Läufe ist der Produktionsstarttermin bereits vordefiniert. Falls sich durch das Zusammenfügen der Läufe der Starttermin ändert, wählen Sie hier den neuen Starttermin aus (bitte ggf. die errechneten Termine der Kapazitätsplanung beachten).
7. Mit der Checkbox **Auftrag zusammenhalten** bewirken Sie, dass alle verfügbaren Teile und Positionen in den Lauf gepackt werden, auch wenn Sie nur 1 Teil oder 1 Position ausgewählt haben. Sie vermeiden dadurch, etwas zu vergessen.
8. Klicken Sie auf **[OK]**, um die Daten zu speichern.
9. Der Lauf wurde gebildet, ist in der Ansicht **Läufe** gelistet und hat die beiden ursprünglichen Läufe ersetzt.

### Läufe auflösen (GP01-004)

**Ziel der Handlung:** Sie lösen einen Lauf auf.

**Voraussetzungen:** Der Lauf muss angelegt sein.

**Zusatzinfo:** Sie können nur solche Läufe auflösen, deren Status **grobgeplant** ist.

**Workflow:**
1. Öffnen Sie die Ansicht **Läufe**.
2. Markieren Sie den Lauf, aus dem Sie den Auftrag löschen möchten.
3. Öffnen Sie das Kontext-Menü und wählen Sie **Details**.
4. Es öffnet sich die Ansicht **Detail** für den entsprechenden Lauf. In ihr werden die verschiedenen Aufträge angezeigt.
5. Markieren Sie den Auftrag, den Sie aus dem Lauf entfernen möchten.
6. Öffnen Sie das Kontext-Menü und wählen Sie **Zurück in den Pool**.
7. Der markierte Auftrag wird zurück in den Pool (Ansicht **Aufträge**) geschrieben.
8. Der Lauf bleibt mit den noch darin enthaltenen Aufträgen / Positionen bestehen.

### Aufträge aus Läufen entfernen (GP 01-005)

**Ziel der Handlung:** Sie entfernen einen Auftrag aus einem Lauf.

**Voraussetzungen:** Der Lauf muss mehrere Aufträge enthalten.

**Zusatzinfo:** Sie können nur solche Läufe bearbeiten, deren Status **grobgeplant** ist.

**Workflow:**
1. Öffnen Sie die Ansicht **Läufe**.
2. Markieren Sie den Lauf, aus dem Sie den Auftrag löschen möchten.
3. Öffnen Sie das Kontext-Menü und wählen Sie **Details**.
4. Es öffnet sich die Ansicht **Detail** für den entsprechenden Lauf. In ihr werden die verschiedenen Aufträge angezeigt.
5. Markieren Sie den Auftrag, den Sie aus dem Lauf entfernen möchten.
6. Öffnen Sie das Kontext-Menü und wählen Sie **Zurück in den Pool**.
7. Der markierte Auftrag wird zurück in den Pool (Ansicht **Aufträge**) geschrieben.
8. Der Lauf bleibt mit den noch darin enthaltenen Aufträgen / Positionen bestehen.

### Läufe archivieren oder löschen (GP 01-006)

**Ziel der Handlung:** Sie archivieren einen produzierten Lauf.

**Zusatzinfo:**
- Nachdem der Lauf archiviert wurde, hat er den Status **archivierbar**.
- Ob ein Lauf tatsächlich archiviert wird oder stattdessen gelöscht werden soll, kann in der Systemkonfiguration definiert werden.
- Zum Archivieren eines Laufes ist eine Archivdatenbank und ein Prozess (ALCIM Server) notwendig. Dieser Prozess kann manuell gestartet werden oder ist als Automatismus im Hintergrund konfiguriert.

**Workflow:**
1. Öffnen Sie die Ansicht **Läufe**.
2. Markieren Sie den Lauf, den Sie archivieren oder löschen möchten.
3. Öffnen Sie das Kontext-Menü und wählen Sie **Lauf verwalten > Lauf archivieren**.
4. Es folgt eine Sicherheits-Abfrage ob Sie den Lauf wirklich archivieren möchten.
5. Klicken Sie auf **[OK]** um den Lauf zu archivieren.
Anschließend hat der Lauf den Status **archivierbar**.

## Ansichten

| Help Card | Themen |
| :--- | :--- |
| Spalte oder Summenzeile hinzufügen | Sie definieren eine neue Spalte oder Summenzeile. |

### Spalte oder Summenzeile hinzufügen (GP 02-001)

**Ziel der Handlung:** Sie definieren eine neue Spalte oder Summenzeile.

**Workflow:**
1. Öffnen Sie die Ansicht, in der Sie eine Spalte oder eine Summenzeile definieren möchten, z. B. **Anzeigen > Aufträge**.
2. Öffnen Sie das Kontextmenü einer Spalte oder Summenzeile.
3. Klicken Sie im Kontextmenü auf **Einfügen > Felddefinitionen > Editieren**. Der Dialog **Felddefinition** wird geöffnet.
4. Wählen Sie im Feld **Menü-Gruppe**, welcher Gruppe im Kontextmenü die Spalte oder die Summenzeile zugeordnet wird, z. B. **Teile kumuliert**.
5. Geben Sie im Feld **Menü-Eintrag** einen Namen für die Spalte oder der Summenzeile ein, z. B. **Fertige Teile**.
6. Geben Sie im Feld **Spaltenüberschrift** den Namen der Spalte oder die Summenzeile ein, mit der die Spalte oder Summenzeile im Dialog angezeigt wird, z. B. **Fertige Teile_alle**.
7. Geben Sie in der Zeile **Beschreibung** eine Beschreibung für die Spalte oder die Summenzeile ein, z. B. **Zeigt alle fertigen Teile an**.
8. Wählen Sie mit der Schaltfläche **Format**, das Format für die Spalte oder Summenzeile, z. B. **Text**.
9. Mit der Schaltfläche **Auswahl öffnen** können Sie entweder einen neuen SQL-Ausdruck eingeben oder auf eine Tabelle und ein Feld der Grobplanung Datenbank filtern.
10. Wählen Sie die Anzeigeoptionen für die Spalte oder die Summenzeile, z. B. ob die Sortierung der Daten aufsteigend oder absteigend erfolgen soll.
11. Klicken Sie auf **[Speichern]**, um die Änderungen zu übernehmen.
12. Klicken Sie auf **[Schließen]**, um den Dialog zu schließen. Die neue Spalte oder Summenzeile **Fertige Teile** ist jetzt im Kontextmenü verfügbar.

# A+W Production Feinplanung

## Revisionsübersicht des Moduls
- **01-2023:** Komplette Überarbeitung.
- **01-2017:** Produkt- und Firmennamen angepasst, Felder ergänzt.
- **07-2013:** Vollständige Überarbeitung der ALCIM-Dokumentation und Anpassung auf A+W Production.
- **11-2012:** Komplette Überarbeitung.
- **09-2007:** Ersterstellung.

**Zu diesem Modul finden Sie folgende Kapitel:**
- Tutorial
- Softwarereferenz

## Tutorial

### In diesem Kapitel finden Sie folgende Themen:
- Dokumentations-Hinweise
- Überblick Feinplanung
- Gruppierungen und Sortierungen
- Abstellplätze und -modi
- Optimierungsmodi

| Thema | Seite |
| :--- | :--- |
| **Dokumentations-Hinweise** | D-258 |
| Wichtige Hinweise | D-258 |
| Aufbau des Tutorials | D-259 |
| **Überblick Feinplanung** | D-260 |
| Ablauf der A+W Production | D-261 |
| Begriffe der A+W Production | D-263 |
| Lostyp | D-263 |
| Lose | D-264 |
| Böcke (Abstellplätze) | D-264 |
| Läufe | D-265 |
| Teilebaum | D-270 |
| Organisation (Orga) | D-271 |
| **Gruppierungen und Sortierungen** | D-272 |
| Überblick | D-273 |
| Einführung | D-274 |
| Gruppierung | D-275 |
| Sortierung | D-276 |
| Zusatz-Sortierung | D-279 |
| Sonderteile | D-281 |
| Demos und Übungen | D-285 |
| **Abstellplätze und -modi** | D-287 |
| Überblick | D-288 |
| Abstellplätze | D-289 |
| Logische Abstellplätze | D-289 |
| Abstellregeln | D-290 |
| Vordefinierte Abstellmodi für A-Böcke | D-292 |
| Robot-Böcke | D-298 |
| Abstellmodi für Fächerwagen | D-298 |
| Abstellmodi für feste Abstellplätze | D-298 |
| Standard-Einstellungen in der Konfiguration | D-299 |
| Einstellungen in den Stammdaten | D-300 |
| Demos und Übungen | D-303 |
| **Optimierungsmodi** | D-306 |
| Überblick | D-307 |
| Unterschiedliche Optimierungs-Modi | D-308 |
| **Orgas** | D-319 |
| Organisationsformen | D-320 |
| Produktionsreihenfolge | D-333 |
| A+W Standard-Orgas | D-336 |
| Abstellplatzorganisation | D-337 |
| Demos und Übungen | D-366 |

## Dokumentations-Hinweise

Das Tutorial zum Modul **Feinplanung** beschäftigt sich mit den Grundlagen des gesamten Produktionsprozesses. Angefangen vom Zuschnitt über die unterschiedlichen Produktions-Linien bis hin zu den Versandgestellen. Es baut auf den Kenntnissen der Grobplanung auf.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

### Themenblöcke
Zur Schulung des Moduls Feinplanung gehören folgende Themenblöcke:
- Gruppierungen und Sortierungen
- Abstellplätze und -modi
- Optimierungsmodi
- Orgas

### Wichtige Hinweise
Diese Dokumentation ist als Unterstützung für den täglichen Arbeitsbetrieb und als Schulungsunterlage für eine begleitete Softwareschulung durch einen zertifizierten A+W Trainer zu verstehen. Sie dient nicht dem Selbststudium und kann keine 100%ig fehlerfreie Anwendung gewährleisten, da die Komplexität nicht von der Software sondern von den realen Arbeitsprozessen abhängt. Die **Feinplanung** definiert die gesamten Organisations- und Produktionsabläufe in Ihrer Produktion. Sie kann daher entsprechend Ihren Anforderungen sehr komplex ausfallen und wird ausschließlich in Begleitung durch einen erfahrenen A+W-Mitarbeiter erstellt und gemeinsam mit Ihnen eingerichtet. Möchten Sie Änderungen an den Einstellungen vornehmen, wenden Sie sich vorher bitte unbedingt an A+W, da es sonst zu unerwünschten Ergebnissen kommen kann!
Der Anwender muss Kenntnisse in der Anwendung von physischen Prozessabläufen in der Glasproduktion und -organisation haben.

### Aufbau des Tutorials
Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

- **Überblick:** Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
    - Lernziele: Was soll vermittelt werden?
    - Nutzen: Wofür können Sie dieses Wissen einsetzen?
    - Merksätze: Welche Zusammenhänge müssen Sie sich merken?
- **Konzepte:** Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.
- **Übungen:** Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen und Lösungsvorschlägen.
- **Querverweisteil:** Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf entsprechende Beschreibungen in der Softwarereferenz hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.

### Lesehinweis
Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.
Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.
Im Praxisteil jeder Schulungseinheit werden die Softwarereferenz und der Übungsteil über Querverweise systematisch einbezogen. Dadurch entsteht ein roter Faden durch die gesamte Dokumentation.

## Überblick Feinplanung

Das für die Produktion benötigte Glas wird in der Regel aus Lagerplatten auf den Schneidtischen zugeschnitten. Häufig gibt es in einem Unternehmen mehrere automatische Schneidtische sowie mindestens einen Schneidtisch für Handzuschnitt oder aber auch für Modelle.

Die Scheiben werden nach dem Zuschnitt, in Abhängigkeit von ihrem nächsten Bearbeitungsschritt, auf Abstellplätzen (z. B. A-Böcke) abgestellt und mit dem Abstellplatz zu ihrer nächsten Bearbeitung bewegt.

Innerhalb eines Arbeitsbereiches (bspw. Zuschnitt) oder einer Prozesskette (bspw. Zuschnitt > VSG-Linie) kann die Verweil- und Bearbeitungsdauer sehr unterschiedlich sein. Dies ist unter anderem davon abhängig wie viel Platz in diesem Bereich für Gestelle zur Verfügung steht um die Gläser abzustellen, wie kompliziert die Abstelllogik ist und wie weit die Laufwege sind. Diese Fragen sind für die Feinplanung maßgeblich. Wenn z. B. hinter dem Zuschnitt wenig Platz für Gestelle ist, muss diese Situation durch eine gute Optimierung und Sequenz der Scheiben ausgeglichen werden, so dass möglichst wenige Gestelle benötigt werden und wenig umsortiert werden muss.

Für die Montage an der ISO-Linie müssen die einzelnen Scheiben der Einheit möglichst nahe beieinander stehen. Sie müssen nicht unbedingt auf einem Gestell stehen. Das bedeutet, dass, je nach Optimierung, beim Zuschnitt vor der Linie umsortiert werden muss.

> **Optimierungsergebnis**
> Die Optimierung mit dem geringsten Verschnitt kann nicht immer oberstes Ziel der A+W Production sein. Beispielsweise wenn sie dazu führt, dass sich der Sortieraufwand vor der Montage unverhältnismäßig erhöht.

Ein wichtiges Kriterium für Feinplanungsergebnisse und die Verweil- und Bearbeitungsdauer ist die Laufgröße und -zusammenstellung. Es sind verschiedene Aspekte zu berücksichtigen:
- Ist die Anzahl der Scheiben im Lauf zu klein oder sind nur sehr große Scheiben vorhanden, dann ist der Verschnitt zu groß. Die Lagermaße können nicht effektiv geschnitten werden, es bleibt ein zu großer Rest.
- Ist der Lauf dagegen zu groß, d. h. er enthält sehr viele Scheiben, dann ist die Produktionszeit für den Lauf sehr hoch und die Gestelle bleiben lange belegt. Gestelle können erst wieder verwendet werden, wenn die Produktion des Laufes abgeschlossen ist.

### Ablauf der A+W Production
Die Feinplanung setzt genau dort an, wo die Grobplanung endet. Das Ergebnis der Grobplanung sind die Läufe. Läufe enthalten die zu produzierenden Teile. Aufgabe der Feinplanung ist es, für die in den Läufen enthaltenen Teile die Produktionsreihenfolge zu erstellen.

Die Produktionsreihenfolge kann sich durch folgende Kriterien ergeben:
- Durch die Vorgaben des Kunden,
- durch die Ergebnisse einer Packmitteloptimierung (PMO) oder
- durch fertigungstechnische Restriktionen.

Die Feinplanung läuft in verschiedenen Schritten ab. Alle dazu notwendigen Prozesse (Daten aus der Datenbank laden, etc.) werden in A+W Production im Hintergrund abgearbeitet und sind für den Benutzer nicht sichtbar. Die Schritte bauen wie folgt aufeinander auf:
1. Im ersten Schritt werden die Daten aus der Datenbank geladen.
2. Ist dies geschehen, erstellt die Feinplanung anhand der Teile und Bearbeitungen die entsprechende Stückliste.
3. Nachdem die Stückliste erstellt ist, weist die Feinplanung die Teile den zur Verfügung stehenden Orgas und Abstellplatztypen zu.
4. Anschließend erfolgen die Gruppierungen und Sortierungen innerhalb der Orga-Gruppen und auf den Abstellplätzen.
5. Im nächsten Schritt behandelt die Feinplanung das Abstellen der Scheiben auf den Abstellplätzen.
6. Dann erfolgt die Bildung der Produktionslose.
7. Im letzten Schritt beschäftigt sich die Feinplanung mit den sogenannten Sonderteilen (Restscheiben, Füllaufträge, Bruch, etc.).

Damit die für jeden Produktionsschritt gewünschte Reihenfolge auch möglich ist, müssen die Vorprodukte auf den Abstellplätzen vor diesem Produktionsschritt in einer passenden Reihenfolge stehen. Die Belegung der Abstellplätze unmittelbar nach dem jeweiligen Produktionsschritt ist das Ergebnis der Produktionsreihenfolge.

Die nachfolgende Grafik (Dreieck aus Reihenfolge, Flexibilität, Ausbeute) zeigt Ihnen sinnbildlich die Auswirkungen der verschiedenen Einstellmöglichkeiten in der A+W Production. Sie können lediglich einen Punkt auf den Linien des Dreiecks definieren. Diesen Punkt können Sie bewegen, indem Sie mithilfe der A+W Production die Produktionseinstellungen verändern.

Sie können genau an einem Eckpunkt arbeiten und die anderen beiden außer Acht lassen. Sie können sich aber auch auf einer Seite bewegen - genau in der Mitte der beiden angrenzenden Ecken, ohne Berücksichtigung des dritten Eckpunktes. Eine Produktion unter Berücksichtigung aller drei Eckpunkte gleichzeitig ist nicht möglich.
- Sie können mit einer strikten Reihenfolge (an einem Eckpunkt) arbeiten - dies geht zu Lasten der Flexibilität und liefert ein schlechtes Ergebnis.
- Sie können mit einer Kombination von Reihenfolge und unbedingte Ausbeute (auf einer Seite) arbeiten - sind dann aber nicht mehr flexibel.

Wir werden dieses Schema innerhalb der Dokumentation immer wieder verwenden.
**Ergänzende Informationen:** ⇨ Tutorial, "Begriffe der A+W Production" auf Seite D-263

### Begriffe der A+W Production
Innerhalb der A+W Production werden folgende Begriffe verwendet:
- Lostyp
- Lose (Verwendungslos, Produktionslos)
- Böcke (Abstellplätze) (Verwendungsbock, Produktionsbock)
- Läufe
- Teilebaum
- Organisation (Orga)

#### Lostyp
Der Lostyp wird durch die Eigenschaften **Bearbeitungstyp** und **Beschaffungsart** gebildet.

*(Abb. D-1 Schematische Darstellung der Lostypen Zuschnitt und Lagerentnahme)*

#### Lose
Ein Los ist eine Anzahl an Scheiben, welche innerhalb eines Zeitraums unter den gleichen Bedingungen auf den gleichen Maschinen verwendet oder produziert werden. Ein Los enthält eine Anzahl von Scheiben eines **Lostyps**. In der A+W Production gibt es zwei Arten von Lostypen:
- **Verwendungslos:** Scheiben eines Verwendungsloses werden zur Fertigung von in Läufen befindlichen Scheiben benötigt. Alle in diesem Los enthaltenen Scheiben haben den gleichen Lostyp.
- **Produktionslos:** Scheiben eines Produktionsloses werden im dazugehörigen Lauf produziert. Alle Scheiben darin haben den gleichen Lostyp. Scheiben eines Produktionsloses werden auf den gleichen Maschinen produziert. Scheiben für eine andere Maschine kommen in ein anderes Los vom gleichen Typ. Ferner können Produktionslose noch nach weiteren Kriterien getrennt werden. So wäre es zum Beispiel denkbar, die Produktion für ISO-Einheiten nach dem Scheibenzwischenraum (SZR) zu trennen. Dadurch würden mehrere Produktionslose gebildet, von denen jedes nur Scheiben für einen bestimmten Scheibenzwischenraum enthält.

**Ergänzende Informationen:** ⇨ Abb. D-2 auf Seite D-265 (Übersicht Produktions- und Verwendungsbock)

#### Böcke (Abstellplätze)
Teile eines Laufes können nach dem Zuschnitt unterschiedlich bearbeitet werden. Dazu werden die Teile auf **Böcke** (Abstellplätze) für die nächste Bearbeitung gestellt. Sie gehören immer einem **Verwendungslos** an, d. h. es sind Scheiben, die zur Produktion benötigt werden. Deshalb müssen sie auf den Verwendungsböcken so stehen, dass für den nächsten Bearbeitungsprozess die gewünschte Produktionsreihenfolge eingehalten werden kann.

Die A+W Production unterscheidet zwischen:
- **Verwendungsbock:** Teile eines Laufes können nach dem Zuschnitt unterschiedlich bearbeitet werden. Dazu werden die Teile auf einen Verwendungsbock (Abstellplatz) für die nächste Bearbeitung gestellt. Sie gehören immer einem Verwendungslos an, d. h. es sind Scheiben, die zur Produktion benötigt werden. Deshalb müssen sie auf den Verwendungsböcken so stehen, dass für den nächsten Bearbeitungsprozess die gewünschte Produktionsreihenfolge eingehalten werden kann.
- **Produktionsbock:** Auf dem Produktionsbock werden Scheiben unmittelbar nach ihrer Produktion abgestellt. Sie stehen auf dem Bock in der Reihenfolge, in der sie aus der Produktion kamen. Es handelt sich dabei stets um Scheiben in einem Produktionslos. Produktionsböcke müssen in der A+W Production nicht zwingend verwendet werden, man kann die Scheiben nach der Produktion auch direkt auf einen Verwendungsbock für die nächste Bearbeitung stellen.

> **Produktions- und Verwendungsböcke**
> In der A+W Production kann für jeden Bearbeitungsschritt eine unterschiedliche Gruppierung/Sortierung verwendet werden. Es ist nicht möglich, einem Produktionsbock einfach eine andere Nummer zu geben und ihn als Verwendungsbock für den nächsten Bearbeitungsschritt zu nehmen. Wenn Scheiben direkt nach der Bearbeitung statt auf einem Produktionsbock auf einen Verwendungsbock gestellt werden, müssen sie so angeordnet werden, dass die Produktionsreihenfolge des nächsten Bearbeitungsschritts eingehalten werden kann.

**Ergänzende Informationen:** ⇨ Softwarereferenz, "Einstellungen-Abstellplatz" auf Seite D-387

#### Läufe
Läufe enthalten eine Menge von Auftragspositionen, die gemeinsam für die Produktion frei gegeben und gemeinsam produziert werden.

**Läufe archivieren**
Läufe, die Sie nicht mehr im Produktionssystem benötigen, können archiviert werden. In der Anzeige **Läufe** können Sie über das Kontextmenü (Lauf verwalten > Lauf archivieren) den ausgewählten Lauf bzw. die ausgewählten Läufe auf archivierbar setzen. Archivierte Läufe erhalten dann den Laufstatus 2000.

Es gibt 2 Arten der Archivierung:
- **Manuelle Archivierung:** Die Einstellungen befinden sich im Parameter-Administrator unter: `Parameter > A+W Production > Allgemein > ALCIM Server > Automatische Laufarchivierung`. Der Eintrag für die manuelle Archivierung ist die `0`.
- **Automatische Archivierung:** Neben der manuellen Archivierung gibt es 3 weitere Archivierungsmodi, die sich auf die Laufstati **produziert (700)**, **verpackt (800)** und **versendet (900)** beziehen. Diese Laufstati werden automatisch vom AlcimBooking gesetzt, sobald alle Kopfteile in dem Lauf die Bearbeitungen für produziert, verpackt oder versendet erhalten haben.

**So archivieren Sie einen Lauf (manuell):**
1. Öffnen Sie die Ansicht **Läufe**.
2. Markieren Sie den Lauf, den Sie archivieren oder löschen möchten.
3. Öffnen Sie das Kontext-Menü und wählen Sie **Lauf verwalten > Lauf archivieren**.
4. Es folgt eine Sicherheits-Abfrage, ob Sie den Lauf wirklich archivieren möchten.
5. Klicken Sie auf **[OK]** um den Lauf zu archivieren.
6. Anschließend hat der Lauf den Status **archivierbar**.

**Archivierungsmethode**
In diesem Bereich wählen Sie, mit welcher Archivierungsmethode gearbeitet werden soll.
Die Einstellungen befinden sich im Parameter-Administrator unter: `Parameter > A+W Production > Allgemein > ALCIM Server > Archivierungsmethode`.
- **0: Standard-Archivierungsmethode:** Arbeitet nur aufgrund des Status eines Laufes.
- **1: Erweiterte Prüfung der Läufe:** Berücksichtigt zusätzlich Flags der Aufträge, um zu prüfen, ob ein Auftrag archiviert werden kann. Diese Methode ist weniger restriktiv.

**Funktionsweise Standard Archivierungsmethode (0):**
Wenn der AlcimServer einen Lauf (z.B. Lauf 1000 mit Status 900) verarbeitet, prüft er alle Aufträge in diesem Lauf. Anschließend prüft er, in welchen anderen Läufen diese Aufträge enthalten sind und ob diese Läufe ebenfalls einen archivierbaren Status haben. Wenn ein Auftrag in einem anderen Lauf mit einem nicht-archivierbaren Status (z.B. 700, produziert) enthalten ist, kann der ursprüngliche Lauf (1000) nicht archiviert werden.

**Funktionsweise Erweiterte Archivierungsmethode (1):**
Diese Methode ermöglicht die Archivierung von Aufträgen, die als abgeschlossen gelten, auch wenn sie in einem anderen Lauf mit einem niedrigeren Status (aber >= 700) enthalten sind. Es werden zusätzliche Datensätze analysiert, um zu bestimmen, ob ein Teil eines Auftrags archivierbar ist. Dies erlaubt es, mehr Läufe zu archivieren.

#### Teilebaum
Der Teilebaum beschreibt den Aufbau und die Produktionsschritte für ein Produkt. Das fertige Produkt (ISO) bildet dabei den Kopf des Teilebaums, seine zur Produktion benötigten Unterteile (ESG und A+W Therm) werden im Teilebaum darunter angeordnet, deren Unterteile (Float) wiederum darunter. Dies wird solange fortgesetzt, bis die Basisteile (in der Regel Float) erreicht sind. Im Teilebaum befinden sich nicht nur Teile, sondern auch deren Bearbeitungen.
*(Abb. D-5 Teilebaum)*

#### Organisation (Orga)
Um einen Lauf korrekt und effizient planen zu können, stehen Ihnen in A+W Production sogenannte Orgas zur Verfügung. Eine Orga ist nichts anderes als ein datentechnisches Regelwerk zur Abbildung der Produktion. In Abhängigkeit von der Struktur des Unternehmens können beliebig viele Orgas (ESG-Orga, ISO-Orga, Bearbeitungs-Orga, etc.) definiert werden. Die unterschiedlichen Orgas organisieren die Abstellplätze jeweils vor den Produktionsschritten (ISO-Linie, Ofen, etc.).
*(Abb. D-6 Schematische Darstellung der Organisation)*

## Gruppierungen und Sortierungen

In diesem Themenblock lernen Sie die unterschiedlichen Gruppierungen und Sortierungen kennen und erfahren, wie Sie damit in der A+W Production umgehen.
Der Themenblock beinhaltet folgende Schulungseinheiten:
- Einführung
- Gruppierung
- Sortierung
- Zusatz-Sortierung
- Demos und Übungen

### Überblick
- **Lernziele:** Gruppierungen, Sortierungen und deren Auswirkungen kennenlernen und verstehen.
- **Nutzen:** Über Gruppierungen und Sortierungen wird das Abstellen der Scheiben in der gewünschten Reihenfolge organisiert. Ohne diese müssten Scheiben vor jedem Produktionsschritt neu sortiert werden.
- **Definitionen:**
    - **Gruppierung:** Erfolgt nach unterschiedlichen und eindeutigen Werten für eine Eigenschaft (z. B. Kundennummer, Glasdicke).
    - **Sortierung:** Erfolgt nach Eigenschaften, die einen fortlaufenden Wert annehmen.
    - **Abstellplatz/Bock:** Gestell (A-Bock, Fächerwagen, Fester Abstellplatz).
- **Merke:** Gruppierungen oder Sortierungen werden durch eine beliebige Kombination aus Eigenschaften und Formeln gebildet.

### Einführung
Die Gruppierungen und Sortierungen dienen dazu, den verschiedenen Abstellplätzen die gewünschte Produktionsreihenfolge zuzuweisen. Gruppierungen können auch verwendet werden, um Scheiben vom gleichen Lostyp auf verschiedene Produktionslose zu verteilen.
A+W Production erlaubt es, Gruppierungskriterien zu definieren und zu entscheiden, ob die Gruppierung in einer gewissen Reihenfolge (sortierte Gruppen) sein soll und ob die Inhalte der Gruppen sortiert sein sollen (Sortierung innerhalb der Gruppe).
Die Optimierung berechnet unter Berücksichtigung von Gruppierung und Sortierung den bestmöglichen Verschnitt.
*(Abb. D-7 Gruppierung und Sortierung)*

### Gruppierung
Gruppiert wird nach unterschiedlichen und eindeutigen Werten für eine Eigenschaft wie z.B. nach Kundennummer, Glasdicke/-farbe, Modelltyp. Jede Gruppe enthält ausschließlich Elemente, die die Eigenschaften des Gruppierungsschlüssels enthalten. Gruppen müssen während des Laufs durch die Produktion zusammengehalten werden.

Die Einstellungen werden im Dialog **Gruppierung/Sortierung** gemacht:
**Stammdaten > Feinplanung > Gruppierung**

**So legen Sie eine neue Gruppierung an:**
1. Wählen Sie im Menü **Stammdaten > Feinplanung > Gruppierung**. Der Dialog **Gruppierung/Sortierung** wird geöffnet.
2. Markieren Sie im linken Bereich den Eintrag **Gruppierungen**.
3. Über die Checkboxen **Eigenschaft** und **Formel** bestimmen Sie die Art der Gruppierung.
4. Wählen Sie die entsprechende Eigenschaft oder Formel aus.
5. Betätigen Sie die Schaltfläche **[Hinzufügen]**.
6. Der Eintrag wird der Liste auf der linken Seite am Ende hinzugefügt. Die erstellte Gruppierung kann nun für Einstellungen in den Orgas genutzt werden.

### Sortierung
Sortiert werden kann nach Eigenschaften, die einen fortlaufenden Wert annehmen (z.B. nach Größe). Sortiert wird innerhalb der gegebenen Gruppen. Die Sortierungen können noch bei Bedarf durch Werte im letzten Teil des Sortierungsschlüssels verfeinert werden.
*(Abb. D-9 Gruppierung und Sortierung)*

> **Supergruppen:**
> Die Optimierung verwendet den Begriff Supergruppe. Eine Supergruppe kann sich aus Scheiben zusammensetzen, die alle identisch bzgl. des Gruppierungsschlüssel oder des kombinierten Gruppierungs-/Sortierungsschlüssel sind. Die Scheiben innerhalb einer Gruppe können, müssen aber nicht sortiert sein.

**So legen Sie eine neue Sortierung an:**
1. Wählen Sie im Menü **Stammdaten > Feinplanung > Gruppierung**. Wechseln Sie in das Register **Gruppierung**.
2. Markieren Sie im linken Bereich den Eintrag **Sortierung**.
3. Über die Checkboxen **Eigenschaft** und **Formel** bestimmen Sie die Art der Sortierung.
4. Wählen Sie die entsprechende Eigenschaft oder Formel aus.
5. Betätigen Sie die Schaltfläche **[Hinzufügen]**.
6. Der Eintrag wird der Liste auf der linken Seite am Ende hinzugefügt.

**So fügen Sie einer bestehenden Sortierung eine Eigenschaft hinzu:**
1. Wählen Sie **Stammdaten > Feinplanung > Gruppierung > Editor-Sortierung**.
2. Aktivieren Sie die Radiotaste **Eigenschaften**.
3. Markieren Sie im rechten Fenster die gewünschte Eigenschaft.
4. Markieren Sie im linken Fenster die Sortierung, der die Eigenschaft hinzugefügt werden soll.
5. Betätigen Sie die Schaltfläche **[Hinzufügen]**.

**Einen neuen Modus für die Gruppenbildung erstellen (Beispiel):**
Erstellung einer Gruppierung nach Anzahl der Scheiben pro Kunde, sortiert nach der größten Anzahl an Scheiben.
1. Gehen Sie zu **Stammdaten > Feinplanung > Gruppierung**.
2. Aktivieren Sie die Radiotaste **Formel** und klicken Sie auf **[Formeln ...]**.
3. Klicken Sie auf **[Neue Formel ...]**, um den **Formel Editor** zu öffnen.
4. Geben Sie einen Namen ein (z.B. "Menge der Scheiben pro Kunde").
5. Suchen Sie die Formel `#Menge#` und fügen Sie sie hinzu.
6. Klicken Sie auf **[Menge] > [Neue Menge ...]** um den **Mengen - Erzeuger** zu öffnen.
7. Erstellen Sie eine neue Menge mit einem Namen.
8. Wählen Sie **Menge > Übergebene Menge**, um alle Positionen des Laufs zu berücksichtigen.
9. Fügen Sie die Eigenschaft **KUNDENNUMMER** als Formel hinzu, um nach Kunde zu filtern.
10. Schließen Sie alle Dialoge mit **[OK]**.
11. Im Dialog **Gruppierung/Sortierung** markieren Sie die neue Formel und klicken auf **[Hinzufügen]**.
12. Die neue Gruppierung ist nun im Dialog **Orga-Gruppen und Einstellungen – Abstellplatz** verfügbar.

### Zusatz-Sortierung
Die Zusatz-Sortierungen können nur auf die Sortierungen angewendet werden, um vorhandene Sortierungen in Abhängigkeit des Werts des letzten Elements zu ergänzen. Zum Beispiel kann eine Sortierung nach Tour, Kunde und `xxxxx` gewünscht sein, wobei `xxxxx` für jeden Kunden anders definiert wird.

**So erstellen Sie eine Zusatz-Sortierung (Beispiel):**
1. Wählen Sie **Stammdaten > Feinplanung > Gruppierung > Editor-Sortierung**.
2. Aktivieren Sie die Radiotaste **Eigenschaften**.
3. Markieren Sie im linken Fenster die Sortierung, für die die Zusatz-Sortierung erstellt werden soll (z.B. `+Auftragsnummer+Positionsnummer`).
4. Markieren Sie im rechten Fenster die Eigenschaft für die Zusatz-Sortierung (z.B. `Kundennummer`).
5. Betätigen Sie **[Erzeuge Zusatzsortierung]**.
6. Geben Sie den Wert für das Sortierungselement ein (z.B. `11` für Kundennummer 11).
7. Aktivieren Sie die Radiotaste **Ziffer** und klicken Sie auf **[Ok]**.
8. Öffnen Sie das Register **Zusatz-Sortierungen**. Die erstellte Zusatz-Sortierung wird angezeigt.

### Sonderteile
Für Sonderteile gibt es keine Gruppierung oder Sortierung. Es gibt folgende Sonderteile:
- **Füllaufträge:** Scheiben, die nicht fest einem Lauf zugeordnet sind und zur Verschnittoptimierung verwendet werden. Sie liegen in der Tabelle `POOL_TEILE` mit Laufnummer `10003`.
- **Restscheiben:** Scheiben der letzten Platte bei hohem Verschnitt, die mit Laufnummer `10005` in die Tabelle `FEIN_TEILE` zurückgesetzt werden.
- **Bruchscheiben:** Gebuchte Bruchscheiben, die mit Laufnummer `10000` in die Tabelle `FEIN_TEILE` zurückgeschrieben werden.
- **Eilscheiben:** Schnell erfasste Scheiben, die der Produktion zugeführt werden, ohne über die normale Auftragsbearbeitung zu laufen. Sie werden mit Laufnummer `10002` in die Tabelle `FEIN_TEILE` geschrieben.

> **Anzeigen von Sonderteilen**
> Damit Füllaufträge, Restblätter oder Bruchscheiben im Register **Spezial** des Dialogs **Feinplanung für Lauf** angezeigt werden, müssen im Dialog **Master-Orga** die jeweiligen Bereiche (Verwende Füller, Verwende Restblätter, Verwende Bruchscheiben) aktiviert und die entsprechenden Abstellplätze angegeben sein. Änderungen an diesen Einstellungen sollten nur in Absprache mit A+W erfolgen.

### Demos und Übungen
- **Trainerdemo:** Gruppierungen und Sortierungen erläutern.
- **Übung 1:** Eine neue Gruppierung hinzufügen (Eigenschaft: Kundennummer).
- **Übung 2:** Einer Gruppierung eine weitere hinzufügen (Eigenschaft: Auftragsnummer zu Kundennummer).
- **Übung 3:** Eine neue Sortierung hinzufügen (Eigenschaft: Positionsnummer).
- **Übung 4:** Einer Sortierung eine weitere hinzufügen (Eigenschaft: Gross_Mass zu Positionsnummer).

## Abstellplätze und -modi

In diesem Themenblock lernen Sie die unterschiedlichen Abstellplätze sowie die verschiedenen Abstellmodi kennen und erfahren, wie Sie damit in der A+W Production umgehen.

### Überblick
- **Lernziele:** Abstellplätze und Abstellmodi sowie deren Auswirkungen verstehen.
- **Nutzen:** Eine gut organisierte Produktion durch verstandene Abstellmodi spart Zeit, Platz und Geld.
- **Definitionen:**
    - **Physikalischer Abstellplatz:** Gestell (A-Bock, L-Bock, Fester Abstellplatz).
    - **Logischer Abstellplatz:** Besteht aus einem oder mehreren Stapeln von Glas und definiert, wie diese zusammengehören. Ein logischer Abstellplatz ist ein Bereich auf einem physikalischen Abstellplatz.

### Abstellplätze
Dieser Abschnitt beschäftigt sich mit den logischen Abstellplätzen sowie den entsprechenden Abstellmodi.

> **Abstellplätze**
> Wir weisen darauf hin, dass wir ausschließlich von Abstellplätzen reden, da wir nicht wissen, ob der Kunde physikalische oder logische Gestelle verwendet.

#### Logische Abstellplätze
Ein logischer Abstellplatz besteht aus einem oder mehreren Stapeln von Glas und definiert, wie diese Stapel zusammen gehören (bspw. um daraus ISO oder VSG zu produzieren). Abhängig ist dies vom gewählten Stapelmodus. Ein logischer Abstellplatz ist einfach ein Bereich auf einem physikalischen Abstellplatz mit Nummer, auf welchen die zusammengehörigen Glasstapel gestellt werden.

#### Abstellregeln
- Unterschiedliche Glasarten werden immer getrennt.
- Die angegebene Abstelltiefe darf nicht überschritten werden.
- In der Regel kommen große Scheiben zuerst auf den Abstellplatz.
- Durch die Verwendung von Abstellmodi können Sie bestimmen, wie das System Einheiten und Gruppen auf den physikalischen und logischen Abstellplätzen abstellt.

**Regeln:**
- **Eine Gruppe pro Stapel:** Jede Gruppe kommt in einen Stapel.
- **Komplette Gruppe können zusammen abgestellt werden:** Verschiedene, komplette Gruppen kommen in einen Stapel.
- **Gruppen werden geteilt:** Das Teilen von Gruppen ist erlaubt (z.B. bei Erreichen des Maximalgewichts).

#### Vordefinierte Abstellmodi für A-Böcke
Auf A-Böcken kann nach vier verschiedenen Verfahren abgestellt werden:
- **Abstellmodus Glas:** Eine Glasart pro Abstellplatz. Jeder Stapel bekommt eine eigene Abstellplatznummer. Erfordert mehr Abstellplätze.
- **Abstellmodus Einheit:** Jede Einheit (bspw. Gläser für ISO oder VSG) steht auf einem logischen Abstellplatz. Jede Glasart ist auf einem anderen Stapel, aber jede Einheit hat ihre eigene Nummer. Benötigt weniger physikalische Gestelle als Modus Glas.
- **Abstellmodus Produktion:** Verschiedene Glasarten können auf einem logischen Abstellplatz in mehreren Stapeln kombiniert werden. Benötigt weniger physikalische Gestelle, aber zusätzliche Kontrollmechanismen.
- **Abstellmodus VABGLA:** Pro Glasart gibt es einen logischen Abstellplatz mit jeweils einem Stapel. Sehr komplex.

#### Robot-Böcke
Robot-Böcke sind A-Böcke mit unendlicher Abstelltiefe und einer maximalen Anzahl von 1 Gruppe pro Abstellplatz. Auf ihnen landen nur Scheiben mit gleichen Eigenschaften.

#### Abstellmodi für Fächerwagen
- **Zusammen:** Scheibe und Gegenscheibe(n) werden immer zusammen auf einen Fächerwagen gestellt.
- **Glas:** Scheiben werden immer getrennt weggestellt.

#### Abstellmodi für feste Abstellplätze
Dienen als Zwischenlager hinter dem Zuschnitt. Es wird so lange auf diesen Abstellplätzen abgestellt, bis er voll ist. Dann muss für die Produktion umsortiert werden.

### Standard-Einstellungen in der Konfiguration
Je mehr Abstellplätze zur Verfügung stehen, desto größer die Flexibilität und besser das Optimierungsergebnis. In der Konfiguration (**Stammdaten > Konfiguration > A+W Production > Feinplanung**) können diverse Einstellungen vorgenommen werden, z.B. die Mindestanzahl an Gestellen.
*(Abb. D-18 Minimale Anzahl an Abstellplätzen)*

### Einstellungen in den Stammdaten
In den Stammdaten (**Stammdaten > Feinplanung > Abstellplätze**) können Sie bestimmte Gestellarten anlegen und verwalten.
- **Abstelltiefe:** Maximale Tiefe des Glasstapels auf dem Gestell.
- **Breite:** Gesamte Breite des Gestells.
- **Max. Abstellplätze/Bock:** Wie viele logische Abstellplätze auf einem physikalischen Gestell sind.
- **Maximales Gewicht:** Maximales Gewicht aller Scheiben auf dem Gestell.

**So richten Sie eine neue A-Bock-Art ein:**
1. Wählen Sie im Menü **Stammdaten > Feinplanung > Abstellplätze**.
2. Betätigen Sie die Schaltfläche **[Hinzufügen]** im Bereich der A-Böcke. Es öffnet sich der Dialog Feinplanung.

