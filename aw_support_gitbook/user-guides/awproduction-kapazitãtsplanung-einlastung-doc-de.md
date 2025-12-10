---
title: "DE_AWProduction_Kapazitaetsplanung_4_4"
source: "DE_AWProduction_Kapazitaetsplanung_4_4.pdf"
tags: ["A+W Production", "Kapazitätsplanung", "Software-Referenz", "Einlastung", "Produktionsmonitor", "Umlastung", "Kampagnenplanung", "ERP", "Stückliste", "Maschinensteuerung"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for the \"Einlastung\" (scheduling/loading) module of the A+W Production Kapazitätsplanung software. It provides detailed descriptions of dialogs, settings, and functions related to production monitoring, capacity planning, order management, and machine scheduling. Key features covered include filtering and displaying machines, adjusting shift properties, managing backlogs, and rescheduling orders."
long_description: "This comprehensive software reference manual details the functionalities of the A+-W Production Capacity Planning (Kapazitätsplanung) software, specifically focusing on the \"Einlastung\" (scheduling/loading) and related modules. The guide is intended for users and administrators responsible for managing production schedules and machine capacities. It covers a wide range of topics, starting with the \"Produktionsmonitor\" which provides a visual overview of machine loads and order statuses. The document explains how to interpret color-coded statuses for backlogs, configure machine and shift properties, and manage work shifts. It elaborates on various settings to customize the display, such as colors for different states (e.g., planned, overloaded, completed), and how to filter views by orders, runs, or custom criteria. A significant portion is dedicated to \"Umlastung\" (rescheduling), detailing the process of moving operations to different times or machines, handling constraints like bottlenecks, and managing dependencies. The manual also covers advanced topics like campaign planning (\"Kampagnenplanung\") for grouping specific work processes, and capacity reservation for customers or projects. Furthermore, it explains how to handle post-processing tasks for orders that failed to schedule correctly, manage bill of materials (BOM) configurations, and split large order positions."
---

# Softwarereferenz Einlastung

Über das Kontextmenü stehen folgende Informationen zur Verfügung:

- **Eigenschaften:**
  Öffnet einen Dialog, in dem Sie die Anzeige der Maschineneigenschaften ändern können.
  ⇨ "Maschine (Name)" auf Seite E-161
- **Schichteigenschaften:**
  Öffnet einen Dialog, in dem Sie Schichtzeiten der Maschine anpassen können.
  ⇨ "Schichten für Maschine anpassen" auf Seite E-163
- **Logische Maschinen anzeigen:**
  Mit diesem Eintrag kann die Darstellung der logischen Maschinen aktiviert und deaktiviert werden. Bislang musste man dazu den entsprechenden Schalter im Stammdaten-Dialog ändern. Bei Verwendung des Kontextmenüs wird nicht der in den Stammdaten hinterlegte Wert geändert, es wird nur die Anzeige angepasst, so dass die Änderung nur temporär ist.
  ⇨ "Misc" auf Seite E-162

---
### Status der Planung

Die Farben der Punkte zeigen die Rückstände an:

- **Grün:** Keine Rückstände.
- **Gelb:** Rückstände, die mit der freien Kapazität noch am aktuellen Tag aufgeholt werden können.
- **Rot:** Rückstände, die nicht mehr am aktuellen Tag aufgeholt werden können.

### Anzeige der Arbeitsschichten

Im Tooltipp zu einer Arbeitsschicht wird eine Kurzinformation zum Status angezeigt.

Über das Kontextmenü stehen folgende Informationen zur Verfügung:

- **Arbeitsplan:**
  Öffnet den Dialog Arbeitsplan: Selektion aus A+W Production Monitor mit dem Überblick über die Läufe und Aufträge der Maschine und Schicht.
  ⇨ "Arbeitsplan aus Produktionsmonitor" auf Seite E-167
- **Löschen:**
  Löscht eine markierte Arbeitsschicht aus dem Produktionsmonitor.
- **Schichteigenschaften:**
  Öffnet den Dialog Schichteigenschaften, um die Eigenschaften einer Schicht zu ändern.
  ⇨ "Schichteigenschaften" auf Seite E-164
- **Reservierungen anzeigen:**
  Öffnet den Dialog Reservierungsanzeige, um die Reservierungen einer Schicht zu prüfen.
  ⇨ "Reservierungsanzeige" auf Seite E-166

**Schraffiert** Die Dauer der Arbeitsschicht ist herabgesetzt.

**X** Die Arbeitsschicht ist deaktiviert.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-151*

# Einlastung Softwarereferenz

**!** Die Arbeitsschicht ist auf *Aktiv für Eilaufträge* gesetzt und steht damit nur für Eilaufträge zur Verfügung.

**?** In der Arbeitsschicht sind undefinierte Bearbeitungen eingelastet.

**Rahmen** Die Arbeitsschicht ist als Engpass definiert.
⇨ "Schichteigenschaften" auf Seite E-164

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-152*

# Angezeigte Maschinen

**Anzeigen > Produktionsmonitor > [Ausgewählte Maschinen]**

*Abb. E-85 Angezeigte Maschinen*

In diesem Dialog wählen Sie die Maschinen aus, die im Dialog Produktionsmonitor angezeigt werden. Dabei können Sie auch die Reihenfolge festlegen. Maschinen, die als Engpassbetriebsmittel definiert sind, werden in der Liste in roter Schrift angezeigt. Ein Engpassbetriebsmittel kann nicht über seine Kapazität hinaus bebucht werden.

**Checkbox** Angabe, ob eine Maschine im Dialog Produktionsmonitor angezeigt wird.
- ☐ Die Maschine wird nicht angezeigt.
- ☑ Die Maschine wird angezeigt.

**[Pfeil nach oben], [Pfeil nach unten]** Verschiebt die markierte Maschine um eine Stelle nach oben oder nach unten.

**[OK]** Speichert und übernimmt die Auswahl und schließt den Dialog.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-153*

# Einstellungen

**Anzeigen > Produktionsmonitor > [Einstellungen]**

*Abb. E-86 Einstellungen – Felder nach Kategorien angezeigt*

In diesem Dialog können Sie die Anzeige im Dialog Produktionsmonitor einstellen, z. B. ob Maschinengruppen und Rückstände angezeigt werden. Außerdem können Sie die Anzeige der Farben für Arbeitsschichten, Engpässe oder Überlasten festlegen.

**[Kategorien]** Sortiert die Elemente nach Kategorien.

**[Alphabetisch]** Sortiert die Elemente alphabetisch.

**[Eigenschaften]** Zur Zeit nicht genutzt.

### Andere Einstellungen

- **Anzahl an Tagen vor Startdatum:**
  Angabe, wie viele Tage vor dem aktuellen Startdatum angezeigt werden.
- **Behandlung von Maschinengruppen:**
  Angabe, ob Maschinengruppen angezeigt werden.
- **Behandlung von Rückständen:**
  Angabe, ob Rückstände angezeigt werden.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-154*

## Darstellung

- **Abgearbeitet:**
  Farbe, in der abgearbeitete Aufträge angezeigt werden.
- **Aktualisierungszeit:**
  Angabe des Intervalls in Sekunden, in dem die Anzeige im Dialog Produktionsmonitor aktualisiert wird.
- **Ausgewählte Schichten:**
  Farbe, in der die ausgewählte Arbeitsschicht angezeigt wird.
- **Auslastung in Grafik anzeigen:**
  Angabe, ob die Auslastung als Text angezeigt wird.
- **Automatische Aktualisierung:**
  Angabe, ob die Anzeige automatisch aktualisiert wird.
- **Eingelastet:**
  Farbe, in der eingelastete Aufträge angezeigt werden.
- **Engpass:**
  Farbe, in der Engpässe angezeigt werden.
- **Engpassfarbe:**
  Schriftfarbe für Engpassbetriebsmittel.
- **Farbe für Hinweissymbole:**
  Farbe, in der Hinweissymbole in den Arbeitsschichten angezeigt werden.
- **Freie Reservierungszeit:**
  Farbe, in der unbebuchte Reservierungen angezeigt werden.
- **Intensität des 3D-Effekts:**
  Auswahl, in welcher Intensität der 3D-Effekt angezeigt wird.
- **Schicht:**
  Farbe, in der Arbeitsschichten angezeigt werden.
- **Stunden anzeigen:**
  Angabe, ob ein Stunden-Raster hinter die Schichten gelegt wird.
- **Überlast:**
  Farbe, in der eine Überlast angezeigt wird.
- **Verplant:**
  Farbe, in der verplante Arbeitsschichten angezeigt werden.
- **Verplante Arbeitsgänge:**
  Farbe, in der verplante Arbeitsgänge angezeigt werden.
- **Zeit anzeigen:**
  Angabe, ob ein Zeitraster angezeigt wird.
- **Zeitfarbe:**
  Farbe, in der die Zeit angezeigt wird.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-155*

## Detaildarstellung

- **Arbeitsgänge mit fertigen Vorprodukten:**
  Angabe, ob Arbeitsgänge mit fertigen Vorprodukten angezeigt werden.
- **Intensität des 3D-Effekts:**
  Angabe der Intensität des 3D-Effekts für grafische Elemente im Produktionsmonitor.
- **Produktionsfreigabe (mengenbasiert):**
  Farbe, in der mengenbasierte Produktionsfreigaben angezeigt werden.
- **Produktionsfreigabe (zeitbasiert):**
  Farbe, in der zeitbasierte Produktionsfreigaben angezeigt werden.
- **Stati anzeigen:**
  Auswahl, ob neben der Maschine der Status für Rückstände angezeigt wird.
- **Unverplant (mengenbasiert):**
  Farbe, in der unverplante Arbeitsschichten angezeigt werden. Die Anzeige ist mengenbasiert.
- **Unverplant (zeitbasiert):**
  Farbe, in der unverplante Arbeitsschichten angezeigt werden. Die Anzeige ist zeitbasiert.
- **Verplant (mengenbasiert):**
  Farbe, in der verplante Arbeitsschichten angezeigt werden. Die Anzeige ist mengenbasiert.
- **Verplant (zeitbasiert):**
  Farbe, in der verplante Arbeitsschichten angezeigt werden. Die Anzeige ist zeitbasiert.
- **Vorprodukte fertig (mengenbasiert):**
  Farbe, in der fertige Vorprodukte angezeigt werden. Die Anzeige ist mengenbasiert.
- **Vorprodukte fertig (zeitbasiert):**
  Farbe, in der fertige Vorprodukte angezeigt werden. Die Anzeige ist zeitbasiert.

**[OK]** Speichert und übernimmt die Auswahl und schließt den Dialog.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-156*

# Bitte wählen Sie einen Auftrag / Lauf aus (Filtern)

**Anzeigen > Produktionsmonitor > [Ansicht filtern]**

In diesem Dialog können Sie Aufträge, Läufe und selbst erstellte Filter auswählen, nach denen die Ansicht im Produktionsmonitor gefiltert werden soll.

Der Dialog enthält folgende Register:
- "Filter - Aufträge" auf Seite E-157
- "Filter - Läufe" auf Seite E-158
- "Filter - Eigene Filter" auf Seite E-159

### Filter - Aufträge

**Anzeigen > Produktionsmonitor > [Ansicht filtern] > Aufträge**

*Abb. E-87 Bitte wählen Sie einen Auftrag/Lauf aus - Aufträge*

In diesem Register sind die definierten Aufträge angezeigt. Sie können jeweils einen Auftrag auswählen. Die Anzeige im Produktionsmonitor wird auf den gewählten Auftrag eingeschränkt.

**Auftragsnummer** Auftragsnummer, nach der gefiltert werden soll.

**Kunde** Kundenname, nach dem gefiltert werden soll. Die Liste der Aufträge wird auf den Kunden eingeschränkt.

**Anzahl der Sätze** Angabe, wie viele Aufträge in der Liste angezeigt werden.

**[OK]** Speichert die Daten.

**[Verwerfen]** Schließt den Dialog, ohne die Daten zu speichern.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-157*

### Filter - Läufe

**Anzeigen > Produktionsmonitor > [Ansicht filtern] > Läufe**

*Abb. E-88 Bitte wählen Sie einen Auftrag/Lauf aus - Läufe*

In diesem Register sind die definierten Läufe angezeigt. Sie können jeweils einen Lauf auswählen. Die Anzeige im Produktionsmonitor wird auf den gewählten Lauf eingeschränkt.

**Laufnummer** Laufnummer, nach der gefiltert werden soll.

**Laufbeschreibung** Laufbeschreibung, nach der gefiltert werden soll. Die Liste der Läufe wird auf den Lauf eingeschränkt.

**Anzahl der Sätze** Angabe, wie viele Läufe in der Liste angezeigt werden.

**[OK]** Speichert die Daten.

**[Verwerfen]** Schließt den Dialog, ohne die Daten zu speichern.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-158*

### Filter - Eigene Filter

**Anzeigen > Produktionsmonitor > [Ansicht filtern] > Eigene Filter**

*Abb. E-89 Bitte wählen Sie einen Auftrag/Lauf aus - Eigene Filter*

In diesem Register werden die selbst definierten Filter angezeigt.

**[Neu]** Öffnet den Dialog *Neuen Filter erstellen*, in dem Sie eigene Filter definieren können.

**[OK]** Speichert die Daten.

**[Verwerfen]** Schließt den Dialog, ohne die Daten zu speichern.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-159*

# Neuen Filter erstellen

**Anzeigen > Produktionsmonitor > [Ansicht filtern] > Register Eigene Filter > [Neu]**

*Abb. E-90 Neuen Filter erstellen*

In diesem Dialog können Sie eigene Filter für die Suche im Produktionsmonitor erstellen. Sie erstellen die Filter in der Datenbanksprache SQL.

> **i Eigene Filter erstellen**
> Bitte wenden Sie sich an den Kundenservice der A+W Software GmbH, wenn Sie spezielle Filter zur Suche im Produktionsmonitor brauchen.

**Name** Name für den Filter.

**Beschreibung** Beschreibung für den Filter.

**SQL** Definition des Filters in SQL.

**[OK]** Speichert die Daten.

**[Verwerfen]** Schließt den Dialog, ohne die Daten zu speichern.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-160*

# Maschine (Name)

**Anzeigen > Produktionsmonitor > Maschine > Kontextmenü > Eigenschaften**

*Abb. E-91 Maschine (Name)*

In diesem Dialog ändern Sie die Eigenschaften der Maschine im Produktionsmonitor.

**[Kategorien]** Sortiert die Elemente nach Kategorien.

**[Alphabetisch]** Sortiert die Elemente alphabetisch.

**[Eigenschaften]** Zur Zeit nicht genutzt.

### Eigenschaften der Maschine

- **ID:** Identifikationsnummer der Maschine.
- **Erfassungsstelle:** Identifikationsnummer der Erfassungsstelle.
- **Name:** Name der Maschine.
- **Engpass:** Auswahl, ob die Maschine ein Engpassbetriebsmittel ist. Engpassbetriebsmittel werden im Produktionsmonitor in der Liste der Maschinen in roter Schrift angezeigt.
- **Anzeigeart:** Auswahl, in welcher Einheit die Schichtinfo den Status *Fertig* anzeigt. Zur Auswahl stehen:
    - Prozent
    - Menge
    - Fläche
    - Gewicht
    - Laufmeter
    - Bearbeitung

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-161*

- **Gruppe:** Maschinengruppe, zu der die Maschine gehört.
- **Leistung pro Anzeigeart ändern:** Angabe der Einheit, in der die Leistung der Maschine angezeigt wird.

### Misc

- **Logische Maschinen anzeigen:** Auswahl, ob im Produktionsmonitor zur markierten Maschine auch die logischen Maschinen angezeigt werden, z. B. zur Maschine Drilling (Bohrmaschine).

**[OK]** Speichert die Daten.

**[Verwerfen]** Schließt den Dialog, ohne die Daten zu speichern.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-162*

# Schichten für Maschine anpassen

**Anzeigen > Produktionsmonitor > Maschine > Kontextmenü > Schichteigenschaften**

*Abb. E-92 Schichten für Maschine anpassen*

In diesem Dialog können Sie die Arbeitsschichten für die jeweilige Maschine bezogen auf Wochentage anpassen.

**Wochentage** Angabe, für welche Wochentage die Änderung der Arbeitsschicht gilt.
- ☐ Die Arbeitsschicht wird für diesen Wochentag nicht geändert.
- ☑ Die Arbeitsschicht wird für diesen Wochentag geändert.

**Schichtnummer** Angabe der Schichtnummer.

**Kapazität** Angabe der Schichtkapazität an den markierten Wochentagen.

**[OK]** Speichert die Daten.

**[Verwerfen]** Schließt den Dialog, ohne die Daten zu speichern.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-163*

# Schichteigenschaften

**Anzeigen > Produktionsmonitor > Anzeige der Schichten > Kontextmenü > Schichteigenschaften**

*Abb. E-93 Schichteigenschaften*

In diesem Dialog können Sie die Eigenschaften einer Arbeitsschicht bezogen auf eine Maschine anzeigen lassen.

**[Kategorien]** Sortiert die Elemente nach Kategorien.

**[Alphabetisch]** Sortiert die Elemente alphabetisch.

**[Eigenschaften]** Zur Zeit nicht genutzt.

### Eigenschaften der Schicht

- **Datum:** Datum der markierten Arbeitsschicht.
- **Schichtnummer:** Nummer der markierten Arbeitsschicht.
- **Start, Ende:** Start- und Endezeit aus den Stammdaten der markierten Arbeitsschicht.
- **Kapazität:** Zeit in Stunden, die in der Arbeitsschicht zur Verfügung stehen. Sie können die Kapazität einer Arbeitsschicht ändern. Die verkleinerte Kapazität wird im Produktionsmonitor schraffiert angezeigt.
- **Kommentar:** Bemerkung zu den manuellen Änderungen der aktuellen Arbeitsschicht.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-164*

- **Status:** Status einer Arbeitsschicht. Im Auswahlmenü wählen Sie unter folgenden Optionen:
    - **Aktiv:** Die Arbeitsschicht ist für die jeweilige Maschine verfügbar.
    - **Deaktiviert:** Die Arbeitsschicht ist für die jeweilige Maschine nicht verfügbar. Die Schicht wird im Produktionsmonitor mit einem X markiert.
      ⇨ "Anzeige der Arbeitsschichten" auf Seite E-151
    - **Aktiv für Eilaufträge:** Die Arbeitsschicht steht für die jeweilige Maschine ausschließlich für Eilaufträge zur Verfügung. Die Arbeitsschicht wird im Produktionsmonitor mit einem ! markiert.
- **Engpass:** Auswahl, ob die Arbeitsschicht ein Engpass ist. Ein Engpassbetriebsmittel kann nicht über seine Kapazität hinaus bebucht werden.

**[OK]** Speichert die Daten.

**[Verwerfen]** Schließt den Dialog, ohne die Daten zu speichern.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-165*

# Reservierungsanzeige

**Anzeigen > Produktionsmonitor > Schicht > Kontextmenü > Reservierung anzeigen**

*Abb. E-94 Übersicht - Reservierungen*

In diesem Dialog werden alle Reservierungen der aktuellen Schicht angezeigt. Abgelaufene oder abgesagte Reservierungen sollten Sie löschen.

⇨ Tutorial, "So löschen Sie eine Reservierung" auf Seite E-60

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-166*

# Arbeitsplan aus Produktionsmonitor

**Anzeigen > Produktionsmonitor > Schicht > Kontextmenü > Arbeitsplan**

In diesem Dialog können Sie sich einen Überblick zu einer bestimmten Arbeitsschicht verschaffen.

Der Dialog enthält folgende Register:
- "Arbeitsplan - Details" auf Seite E-168
- "Arbeitsplan - Übersicht" auf Seite E-170

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

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-167*

# Arbeitsplan – Details

**Anzeigen > Produktionsmonitor > Schicht > Kontextmenü > Arbeitsplan > Details**

*Abb. E-95 Arbeitsplan: Selektion aus Produktionsmonitor – Details*

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

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-168*

### Summenzeile

In der Summenzeile können Sie sich verschiedene Summen anzeigen lassen, z. B.:

- **Menge Soll Gesamt:**
  Gesamtmenge und Menge in den markierten Läufen.
- **Dauer gesamt:**
  Gesamte Bearbeitungsdauer der markierten Läufe in Stunden.

### Filter

**[Filter hinzufügen]** Fügt einen Filter ein.

**Dropdown-Menü** Auswahl eines Filters:
- **Klick:** Öffnet das Dropdown-Menü, aus dem Sie einen Filter wählen.
- **Rechtsklick:** Öffnet einen Dialog, um den aktuellen Filter zu bearbeiten.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-169*

# Arbeitsplan – Übersicht

**Anzeigen > Produktionsmonitor > Schicht > Kontextmenü > Arbeitsplan > Übersicht**

*Abb. E-96 Arbeitsplan: Selektion aus Produktionsmonitor – Übersicht*

In diesem Register können Sie sich einen Überblick zu den Bearbeitungstypen verschaffen, die in der gewählten Arbeitsschicht an einer Maschine ausgeführt werden.

Die Anzeige der Spalten können Sie auf die gleiche Weise einrichten, wie im Register Details.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-170*

# Einlastung

**Anzeigen > Einlastung**

*Abb. E-97 Einlastung*

In diesem Dialog prüfen Sie Aufträge, die als XML-Daten aus A+W Business oder A+W Enterprise importiert werden. Mit Öffnen des Dialogs werden die Aufträge automatisch importiert. Nach dem Import wird im Feld **Status** die aktuelle Uhrzeit angezeigt.

Wenn in A+W Production ein automatischer Import der Aufträge eingerichtet ist, müssen Sie den Dialog Einlastung nicht öffnen. Der Datenimport läuft dann als Hintergrundprozess. Sie können den Prozess der Einlastung über den A+W Service Monitor verfolgen.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-171*

# Stücklistenkonfiguration

**Stammdaten > Einlastung > Stücklistenkonfiguration**

*Abb. E-98 Stücklistenkonfiguration*

In diesem Dialog können Sie die Stücklistenkonfiguration analysieren.

> **i Keine Änderungen der Stücklistenkonfiguration**
> Änderungen im Dialog Stücklistenkonfiguration bedeuten einen tiefen Eingriff in die Struktur von A+W Production. Ändern Sie die Stücklistenkonfiguration auf keinen Fall. Bei Fragen wenden Sie sich bitte an den Kundenservice der A+W Software GmbH.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-172*

# Aktion

**Stammdaten > Einlastung > Stücklistenkonfiguration > [Neu], [Ändern]**

*Abb. E-99 Stücklistenkonfiguration – Aktion*

In diesem Dialog können Sie die einzelnen Aktionen zur Stücklistenmanipulation analysieren. Jede Aktion besteht aus mindestens einer Bedingung, bei deren Zutreffen die hinterlegte Funktion ausgeführt wird.

> **i Keine Änderungen der Stücklistenkonfiguration**
> Änderungen im Dialog Stücklistenkonfiguration bedeuten einen tiefen Eingriff in die Struktur von A+W Production. Ändern Sie die Stücklistenkonfiguration auf keinen Fall. Bei Fragen wenden Sie sich bitte an den Kundenservice der A+W Software GmbH.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-173*

# Umlastung

- **Anzeige > Produktionsmonitor > Doppelklick auf Schicht > > Kontextmenü > Arbeitsplan > Umlastung**
- **Anzeige > Aufträge > Kontextmenü > Bearbeitungen > Kontextmenü > Arbeitsplan > Umlastung**
- **Anzeige > Läufe > Kontextmenü > Bearbeitungen > Kontextmenü > Arbeitsplan > Umlastung**

*Abb. E-100 Umlastung*

In diesem Dialog können Sie Bearbeitungen aus Aufträgen oder Läufen auf andere Termine und Maschinen umlasten.

⇨ Tutorial, "Umlastungen" auf Seite E-37

### 1. Wählen Sie umzulastende Bearbeitungen aus

Liste der Bearbeitungen, die umgelastet werden können.
- **Auftrag:**
  Liste der Bearbeitungen, sortiert nach Datum und Maschinen.
- **Position:**
  Positions-Nummer der jeweiligen Bearbeitung.
- **Produktionstermin:**
  Bisheriger Termin, an dem die Bearbeitung durchgeführt werden soll.
- **Schicht:**
  Bisherige Arbeitsschicht, in der die Bearbeitung durchgeführt werden soll.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-174*

- **Geschützt:**
  Anzeige, ob der Termin geschützt ist.
- **Arbeitsgang:**
  Arbeitsgang, mit dem die Bearbeitung durchgeführt wird.
- **Logische Maschine:**
  Logische Maschine, die für die Bearbeitung verwendet wird.
- **Menge:**
  Teilemenge, die bei der Bearbeitung hergestellt wird.
- **Maschine:**
  Maschine, auf der die Bearbeitung durchgeführt wird.
- **Teilenummer:**
  Nummer der Stücklistenkomponente.
- **Sequenz:**
  Sequenz der Bearbeitung.
- **BearbNr:**
  Bearbeitungs-Nummer der Bearbeitung.
- **Bestell-Information:**
  Angabe, ob Bestellteile enthalten sind.

**Einlastung erzwingen** Sie können die Einlastung auf einen bestimmten Termin erzwingen.
- ☐ Die Termin-Umlastung wird nicht erzwungen.
- ☑ Die Termin-Umlastung wird erzwungen. Mit dieser Einstellung werden die Kapazitätsgrenzen von Engpassbetriebsmitteln nicht berücksichtigt. Daher werden die Arbeitsschichten ggf. überbucht.

**Erlaube Eilraster** Sie können für die Umlastung festlegen, dass die Übergangszeiten vom Typ Eil verwendet werden.
- ☐ Die Termin-Umlastung wird mit den normalen Übergangszeiten berechnet.
- ☑ Die Termin-Umlastung wird mit den Eil-Übergangszeiten berechnet.

**Kombobox (Schutz)** Auswahl, ob Termine vor Umlastungen geschützt sind. In der Regel setzen Sie den Schutz nach einer erfolgreichen Umlastung.
- **Geschützte Bearbeitungstermine beibehalten:**
  Geschützte Bearbeitungstermine werden nicht umgelastet.
- **Umlastungsziele schützen:**
  Die nach der Umlastung berechneten neuen Termine werden vor weiteren Umlastungen geschützt.
- **Alle Bearbeitungstermine schützen:**
  Alle Bearbeitungstermin der markierten Läufe werden geschützt.
- **Bearbeitungsschutz aufheben:**
  Der Schutz für alle Bearbeitungstermine der markierten Läufe wird aufgehoben.

**Begründung** Wenn Sie für die Umlastung auch einen Termin in der Vergangenheit zulassen wollen, müssen Sie eine Begründung eingeben. Damit wird die entsprechende Checkbox freigeschaltet.
⇨ "Erlaube Zieltermine in der Vergangenheit" auf Seite E-176

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-175*

**Tage für automatische Lieferterminverschiebung** Angabe, um wie viele Tage der Liefertermin verschoben werden darf.

> **i Umlasten und Versandtermin**
> Der Versandtermin ist bei der Umlastung geschützt, um die Anforderungen des ERP-Systems zu erfüllen. Der Versandtermin bleibt bestehen, solange Sie ihn nicht explizit umlasten.
> Halten Sie Rücksprache mit dem Auftragserfasser, falls Sie einen Versandtermin verändern wollen.

**Als Chefauftrag umlasten** Sie können die Bearbeitung mit oberster Priorität umlasten.
- ☐ Die Bearbeitung wird mit der normalen Priorität umgelastet.
- ☑ Die Bearbeitung wird mit oberster Priorität umgelastet. Die Aufträge werden mit den minimalen Übergangszeiten eingelastet. Dabei können auch die Zeiten von Kampagnen genutzt werden. Verwenden Sie diese Einstellung nur in Notfällen.

**Ignoriere Wareneingangstermine** Manche Bearbeitungen sind davon abhängig, dass zugekaufte Teile angeliefert sein müssen, z. B. die Fertigung einer ISO-Scheibe mit einem ESG, das nicht selbst produziert wird.
- ☐ Für die Fertigung wird ein Wareneingang erwartet. Der Wareneingang wird vor der Umlastung geprüft.
- ☑ Der Wareneingang wird vor der Umlastung nicht geprüft.

**Lieferterminverschiebungen zurückmelden** Die Umlastung einer Position kann den Liefertermin betreffen.
- ☐ Bei einer Lieferterminverschiebung für eine Position wird der Liefertermin aus dem Auftragskopf zurückgemeldet.
- ☑ Eine Lieferterminverschiebung einer Position wird an den Auftrag zurückgemeldet. Der Liefertermin im Auftragskopf wird angepasst. Das ist jedoch nur möglich, wenn die Daten online übertragen werden.

**Erlaube Zieltermine in der Vergangenheit** Sie können bei der Umlastung auch Termine in der Vergangenheit zulassen. Die Checkbox ist nur freigeschaltet, wenn Sie eine Begründung eingegeben haben.
- ☐ Termine werden nicht in die Vergangenheit verschoben.
- ☑ Die Bearbeitung kann auch in die Vergangenheit verschoben werden. Dazu müssen Sie eine Begründung eingeben.
⇨ "Begründung" auf Seite E-175

### 2. Wählen Sie Datum, Schicht und Maschine aus

In diesem Bereich werden die Maschinen und die jeweils zugehörigen Arbeitsschichten pro Arbeitstag angezeigt.

**[Ansicht aktualisieren]** Aktualisiert die Liste.

**[Gegebene Anzahl von Tagen zurück]** Verschiebt den Zeitraum der angezeigten Arbeitsschichten um die Anzahl der Tage in die Vergangenheit, die im Feld Tage angegeben ist.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-176*

**Starttermin** Angabe des Starttermins, von dem an der Zeitraum angezeigt werden soll.

**Tage** Angabe, um wie viele Tage die Anzeige der Arbeitsschichten mit den Schaltflächen jeweils vor- oder zurückgestellt werden soll.

**[Gegebene Anzahl von Tagen vor]** Verschiebt den Zeitraum der angezeigten Arbeitsschichten um die Anzahl der Tage in die Zukunft, die im Feld Tage angegeben ist.

### 3. Umlastung ausführen

**Zum Start der Umlastung den Modus auswählen** Auswahl, in welchem Modus die Umlastung erfolgt:
- **Komplette Stückliste umlasten:**
  Die komplette Stückliste, zu der die Bearbeitung gehört, wird umgelastet.
- **Nur markierte Bearbeitung:**
  Nur die markierte Bearbeitung wird umgelastet.
- **Markierte und alle folgende Bearbeitungen:**
  Die markierte und alle nachfolgenden Bearbeitungen der Stückliste werden umgelastet.
- **Markierte und alle vorherigen Bearbeitungen:**
  Die markierte und alle vorherigen Bearbeitungen der Stückliste werden umgelastet.
- **Unbedingte Terminzuweisung für markierte Bearbeitung:**
  Die markierte Bearbeitung wird auf den ausgewählten Termin der gewählten Maschine umgelastet. Die Plausibilität wird nicht geprüft und die Maschinenkapazitäten werden dabei nicht berücksichtigt.

**[Umlasten]** Startet die Umlastung mit den gewählten Parametern. Die Schaltfläche ist nur freigeschaltet, wenn ein Umlastungsmodus ausgewählt ist.

**[Schließen]** Schließt den Dialog, ohne die Daten zu speichern.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-177*

# Maschinenumlastung

- **Aufträge > Kontextmenü > Arbeitsplan > Maschinenumlastung**
- **Läufe > Kontextmenü > Maschinenumlastung**

*Abb. E-101 Maschinenumlastung*

In diesem Dialog können Sie Bearbeitungen aus Aufträgen oder Läufen auf andere Logische Maschinen umlasten. Bei der Maschinenumlastung wird die Bearbeitungsdauer nicht neu berechnet. Die Kosten und Einlastungsregeln werden nicht geprüft.
Eine Umlastung über diesen Dialog ist daher nur sinnvoll, wenn Sie auf eine identische Logische Maschine umlasten können.

**Logische Routen** Maschinen und logische Maschinen, von denen aus eine Bearbeitung umgelastet werden soll.

**Umlastungsalternativen** Anzeige und Auswahl der möglichen Alternativen zu der markierten logischen Maschine.

**[Übernehmen]** Speichert die Daten.

**[Schließen]** Schließt den Dialog, ohne die Daten zu speichern.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-178*

# Nachbearbeitung Einlastung

**Stammdaten > Nachbearbeitung Einlastung**

*Abb. E-102 Nachbearbeitung Einlastung*

In diesem Dialog können Sie Aufträge, die nicht erfolgreich eingelastet wurden, nachbearbeiten und erneut einlasten.
⇨ Tutorial, "Eingelastete Aufträge nachbearbeiten" auf Seite E-42

**[Bearbeiten]** Öffnet den Dialog *Fehlerhafte Aufträge*, in dem Sie auf Probleme bei der Einlastung reagieren können.
⇨ "Fehlerhafte Aufträge" auf Seite E-182

**[Aktualisieren]** Aktualisiert die Ansicht mit aktuellen Daten.

### Übersicht Aufträge

Die Anzeige der Spalten hängt von der Option ab, die im Feld *Nachbearbeitung von...* gewählt ist.
- **Auftrag:** Die Auftragsnummer wird angezeigt, wenn die Option *undefinierten Artikeln* gewählt ist.
- **Artikel-Nr., Artikelbez.:** Nummer und Bezeichnung des Artikels, der nicht definiert ist, werden angezeigt, wenn die Option *undefinierten Artikeln* oder *undefinierten Bearbeitungen* gewählt ist.
- **Produktionsartikelnummer, Produktionsartikel:** Nummer und Bezeichnung des Produktionsartikels, der nicht definiert ist.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-179*

werden angezeigt, wenn die Option *undefinierten Produktionsartikel/Dicke-Kombinationen* gewählt ist.
- **Dicke:** Die Dicke in mm wird angezeigt, wenn die Option *undefinierten Produktionsartikel/Dicke-Kombinationen* gewählt ist.
- **Meldung:** Der Text der Rückmeldung wird angezeigt, wenn die Option *Rückmeldungsprobleme* gewählt ist.
- **Status:** Der Status der Aufträge wird angezeigt, wenn die Option *fehlerhafter Auftragsdaten* gewählt ist.
- **Anzahl Aufträge:** Die Anzahl der Aufträge mit gleichem Status wird angezeigt, wenn die Option *fehlerhafter Auftragsdaten* gewählt ist.
- **Zeitstempel der Importdatei:** Datum und Uhrzeit, zu denen der Auftrag eingelastet wurde.
- **Pos.:** Die Nummer der Auftragsposition wird angezeigt, wenn die Option *Änderungen verplanter Aufträge* gewählt ist.
- **PosRef.:** Die Referenznummer der Auftragsposition wird angezeigt, wenn die Option *Änderungen verplanter Aufträge* gewählt ist.
- **Packmittelgruppe:** Die Packmittelgruppe, die dem Lauf zugeordnet ist, wird angezeigt, wenn die Option *Änderungen verplanter Aufträge* gewählt ist.
- **Anzahl Pos.:** Die Anzahl der zum Lauf gehörenden Positionen wird angezeigt, wenn die Option *Änderungen verplanter Aufträge* gewählt ist.
- **Änderungstext:** Die Anmerkung aus dem ERP-System wird angezeigt, wenn die Option *Änderungen verplanter Aufträge* gewählt ist. Dazu muss die Anmerkung mit übergeben worden sein.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-180*

### Nachbearbeitung von

Mit der Wahl der Option legen Sie fest, nach welchen Kriterien die Aufträge in der Liste angezeigt werden sollen. In der Klammer steht jeweils, wie viele Aufträge mit dem Kriterium vorhanden sind.
Bei undefinierten Artikeln, Dicken-Kombinationen und/oder Bearbeitungen können Sie den Auftrag mit einem Doppelklick öffnen und korrigieren.

- **Undefinierten Artikeln (n Aufträge):** Aufträge mit undefinierten Artikeln.
- **Undefinierten Produktionsartikel-/Dicke-Kombinationen (n Aufträge):** Aufträge mit undefinierten Produktionsartikel-Kombinationen und undefinierten Dicke-Kombinationen.
- **Undefinierten Bearbeitungen (n Aufträge):** Aufträge mit undefinierten Bearbeitungen.
- **Rückmeldeproblemen (n Aufträge):** Aufträge mit Rückmeldeproblemen. Rückmeldeprobleme können bei der Datenübergabe zwischen einem ERP-System und A+W Production entstehen.
  ⇨ "Asynchrone Verarbeitung" auf Seite E-183
- **Änderungen verplanter Aufträge (n Aufträge):** Aufträge, die nach der Einlastung geändert wurden.
  ⇨ "Änderung bereits verplanter Aufträge" auf Seite E-184
- **Fehlerhafter Auftragsdaten (n Aufträge):** Aufträge mit fehlerhaften Auftragsdaten.
  ⇨ "Fehlerhafte Aufträge" auf Seite E-182
- **Aufträgen mit Hinweisstatus (n Aufträge):** Aufträge mit einem Hinweisstatus.

### Anzeigen nach

Mit der Wahl der Option legen Sie fest, wie die Aufträge in der Liste sortiert werden.

- **Auftragsnummer:** Sortierung nach Auftragsnummern.
- **Nachbearbeitungsursache:** Sortierung nach Nachbearbeitungsursachen.

### Detailanzeige für Läufe und Packmittelgruppen

Das Feld wird angezeigt, wenn die Option *Änderungen verplanter Aufträge* gewählt ist.

- **Lauf:** Nummer des Laufs.
- **Laufstatus:** Status des Laufs.
- **Packmittelgruppe:** Packmittelgruppe, die dem Lauf zugeordnet ist.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-181*

# Fehlerhafte Aufträge

**Stammdaten > Nachbearbeitung Einlastung > Option Fehlerhafter Auftragsdaten > [Bearbeiten]**

*Abb. E-103 Fehlerhafte Aufträge*

In diesem Dialog können Sie wählen, wie nicht eingelastete Aufträge verarbeitet werden sollen.

⇨ Tutorial, "Eingelastete Aufträge nachbearbeiten" auf Seite E-42

Dazu können Sie zwischen folgenden Optionen wählen:

- **Erneute Datenübernahme:**
  Markierte Aufträge werden erneut eingelastet. Verwenden Sie diese Option z. B. bei Fehlern in den Stammdaten, z. B. wenn A+W Production keine Arbeitsschicht für den Auftrag gefunden hat.
  Wenn Sie den Fehler behoben haben, können Sie den Auftrag einlasten, ohne eine erneute Datenübertragung vom ERP-System anzufragen.
- **Einlastung erzwingen. Die freie Kapazität an Engpassbetriebsmitteln wird in diesem Fall nicht berücksichtigt.:**
  Der Auftrag wird erneut eingelastet. Dabei wird die Kapazität der Maschine nicht berücksichtigt. Daher werden die Arbeitsschichten ggf. überbucht.
  Wenn eine Kapazität überschritten ist, kann es zu Terminverschiebungen bei anderen Aufträgen kommen.
- **Einlastung ignorieren. Die Produktionstermine werden ermittelt ohne Rücksicht auf Übergangszeiten, Kapazitätsgrenzen und Kampagnentermine. Gültige Arbeitspläne müssen Sie mittels manueller Umlastung erstellen.**
- **Löschung der fehlerhaften Aufträge. Die Aufträge können dann mit diesem System NICHT verplant werden. Rücksprache mit Auftragserfassung erforderlich!:**
  Die Aufträge werden aus A+W Production gelöscht. Die Aufträge müssen im ERP-System korrigiert und erneut übertragen werden.
- **Ermittelten Liefertermin bestätigen:**
  Übernahme des neuen Liefertermins, den A+W Production für die gewähl-

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-182*

ten Aufträge vorschlägt. Die Aufträge werden zu den neuen Liefertermin-Bedingungen eingelastet und der ermittelte Liefertermin wird an das ERP-System zurück gemeldet.
Ändern Sie Liefertermine nur nach Absprache mit der Auftragserfassung.

# Asynchrone Verarbeitung

**Stammdaten > Nachbearbeitung Einlastung > Option Rückmeldungsprobleme > [Bearbeiten]**

*Abb. E-104 Asynchrone Verarbeitung*

In diesem Dialog können Sie wählen, wie Aufträge mit Problemen bei der Rückmeldung verarbeitet werden sollen.

Dazu können Sie zwischen folgenden Optionen wählen:

- **Erneuten Versuch starten:**
  Markierte Aufträge werden erneut eingelastet. Verwenden Sie diese Option z. B. bei Fehlern während der Datenübertragung.
- **Position stornieren:**
  Die Position wird storniert. Der restliche Auftrag wird eingelastet. Bei dieser Option sollten Sie Rücksprache mit dem Auftraggeber halten, damit die Daten erneut übertragen werden.
- **Fehler ignorieren:**
  Die Produktionstermine werden ermittelt. Die Position wird übernommen, die Rückmeldung wird jedoch nicht geschrieben. Deshalb dürfen Sie diese Option nur auswählen, wenn Sie absolut sicher sind, dass Sie den Fehler ignorieren können.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-183*

# Änderung bereits verplanter Aufträge

**Stammdaten > Nachbearbeitung Einlastung > [Bearbeiten]**

*Abb. E-105 Änderung bereits verplanter Aufträge*

In diesem Dialog können Sie wählen, wie eingelastete Aufträge behandelt werden sollen, zu denen Änderungen übertragen wurden.

Dazu können Sie zwischen folgenden Optionen wählen:
- **Neue Position erzeugen: Storno der bisherigen Position und Übernahme der Änderung als neue Position in den Pool.:**
  Der Auftrag wird mit einer neuen Positionsnummer erneut eingelastet.
- **Erneut versuchen: Übernahme der Änderung in den Pool. Lösen Sie zuvor die betroffenen Läufe/PMO-Mastergruppen auf.:**
  Lösen Sie die betroffenen Läufe zunächst auf und wählen Sie anschließend diese Option. Der Auftrag wird erneut eingelastet.
- **Änderung ignorieren: Löschung der Änderung. Die bisherige Position bleibt unverändert.:**
  Die Änderung wird gelöscht und die ursprünglichen Daten beibehalten.
- **(nicht empfohlen): Übernahme der Änderung in die bisherigen Läufe. Stellen Sie zuvor sicher, dass die Änderung nicht produktionsrelevant ist.:**
  Zur Zeit nicht genutzt.

**[Änderung analysieren]** Zur Zeit nicht genutzt.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-184*

# Positionssplit

**Anzeigen > Aufträge > Kontextmenü > Positionen splitten**

*Abb. E-106 Positionssplit*

In diesem Dialog können Sie Positionen aus Aufträgen aufsplitten. Wenn bei einer großen Position die Bearbeitungsdauer der langsamsten Maschine die konfigurierte Schwelle überschreitet, wird diese Position im Rahmen der Einlastung durch A+W Capacity Planner gesplittet. In der Regel werden die Positionen automatisch gesplittet, so dass die Terminfindung auch bei großen Positionen mit optimaler Geschwindigkeit abläuft.

Der Positionssplit ist im Part Grobplanung - Tutorial beschrieben.

### Markierte Positionen

In der Liste werden die Positionen angezeigt, die Sie im Dialog *Bearbeitungen* ausgewählt haben.

- **Auftrag:** Auftrag, den Sie zum Splitten ausgewählt haben.
- **Pos.:** Nummer der Auftragsposition.
- **UPos.:** Nummer der Unterpositionen im Auftrag.
- **Menge:** Anzahl der Scheiben in der Position.

**[Entfernen]** Löscht die markierte Position.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-185*

### Splitting-Optionen

Mit der Wahl der Option legen Sie fest, wie die Positionen geteilt werden:
- **Je Position in ... Positionen aufteilen:**
  Angabe, in wie viele neue Positionen aufgeteilt wird. Das Feld zur Angabe der Anzahl wird freigeschaltet.
- **Positionen mit maximal ... Scheiben erzeugen:**
  Angabe, wie viele Scheiben eine neue Position maximal enthalten darf. Das Feld zur Angabe der Anzahl wird freigeschaltet.
- **Je Pos. eine Pos. mit ... Scheiben erzeugen:**
  Angabe der Scheibenanzahl, für die jeweils eine neue Position erzeugt wird. Das Feld zur Angabe der Anzahl wird freigeschaltet.
- **Teilung gemäß PMO Ergebnis:**
  Angabe, dass die Positionen passend zur Packmitteloptimierung gesplittet werden.

### Neue Positionen

In der Liste werden die gesplitteten Positionen als Unterpositionen angezeigt:
- **Auftrag:** Auftragsnummer.
- **Pos.:** Nummer der Auftragsposition.
- **UPos.:** Nummer der Unterpositionen im Auftrag.
- **Neue Position:** Nummer der neuen Position nach dem Split. Die Nummerierung wird pro gesplitteter Auftragsposition gezählt.
- **Menge:** Anzahl der Scheiben in der neuen Position.

**[Splitten]** Splittet die markierte Position. Die neuen Positionen werden erst gespeichert, wenn sie mit [Übernehmen] bestätigt sind.

**[Übernehmen]** Speichert die neuen Positionen. Diese Aktion kann nicht rückgängig gemacht werden.

**[Verwerfen]** Stellt die ursprüngliche Position wieder her. Anschließend können Sie die Position mit anderen Vorgaben splitten.

**[Schließen]** Schließt den Dialog, ohne die Daten zu speichern.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-186*

# Kampagnen und Reservierungen

Für bestimmte Arbeitsgänge und/oder Aufträge können Sie Kampagnen einrichten und Kapazitäten reservieren.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Kampagnen" auf Seite E-188
- "Abgelaufene Reservierungen" auf Seite E-192
- "Reservierungen" auf Seite E-194
- "Reservierung für Maschine" auf Seite E-197
- "Kunde auswählen" auf Seite E-198
- "Objekt auswählen" auf Seite E-199

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-187*

# Kampagnen

**Stammdaten > Kapazitätsplanung > Kampagnenplanung**

In diesem Dialog können Sie Kampagnen als Einzeltermine oder wöchentliche Termine definieren. Mit Kampagnen können Sie für bestimmte Arbeitsgänge Kapazitäten einplanen, z. B. für Siebdruck für jeden Wochentag eine andere Farbe.

> **i Voraussetzung**
> Nur die Bearbeitungen werden in Kampagnenterminen eingelastet, die als Kampagnen-Bearbeitungen definiert sind.

⇨ Tutorial, "Kampagnenplanung" auf Seite E-44

Der Dialog Kampagnen enthält folgende Register:
- "Kampagnen – Einzeltermine" auf Seite E-189
- "Kampagnen – Wöchentliche Termine" auf Seite E-191

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-188*

## Kampagnen – Einzeltermine

**Stammdaten > Kapazitätsplanung > Kampagnenplanung > Register Einzeltermine**

*Abb. E-107 Kampagnen - Einzeltermine*

In diesem Register verwalten Sie Einzelkampagnen. Mit Einzelkampagnen führen Sie Kampagnen durch, die einmalig anfallen.

⇨ Tutorial, "Kampagnenplanung" auf Seite E-44

**Arbeitsgang** Arbeitsgänge, die Sie in der Maschinenzuordnung erzeugt haben. Ein Arbeitsgang ist in der Liste hellgrau hinterlegt, wenn er zu einer Kampagne hinzugefügt ist.

**Kampagnen** Kampagnenfähige Arbeitsgänge, die Sie hinzugefügt haben. Wenn Sie in der Liste Kampagnen einen Arbeitsgang markieren, werden in den Registern *Einzeltermine* oder *Wöchentliche Termine* die zugehörigen Termine angezeigt.
- ☐ Die Kampagne ist nicht aktiv.
- ☑ Die Kampagne ist aktiv.

**[Zuordnen]** Verschiebt ein markiertes Element auf die andere Seite.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-189*

### Einzeltermine

**Kalender** Auswahl eines Datums für eine Kampagne.

**Schichten** Verfügbare Arbeitsschichten am gewählten Datum.

> **i Anzeige der Schichten**
> Nur die aktiven Schichtpläne werden angezeigt. Aktivieren Sie ggf. die Schichtpläne, die für die Kampagne benötigt werden.

**Einzeltermine** Anzeige der Kampagnen für das markierte Datum.
- **Datum:** Termine, zu denen Sie Kampagnen erzeugt haben.
- **Schicht:** Arbeitsschicht, in der die jeweilige Kampagne durchgeführt wird.

> **i Kampagnen löschen**
> Wenn Sie kurzfristig Kampagnen löschen, hat das Auswirkungen auf die Produktion. Bearbeitungen werden z. B. nicht durchgeführt oder Produktionstermine ändern sich.
> Bitte wenden Sie sich an den Kundenservice der A+W Software GmbH, wenn Sie Kampagnen löschen wollen und zu diesem Zeitpunkt bereits Aufträge eingelastet sind.

**Hinzufügen für die nächsten** Angabe, für welchen Zeitraum die Kampagne angelegt wird.
Mit der Wahl der Option legen Sie fest, ob die Dauer des Termins in Tagen oder Wochen angegeben wird.

**[Kampagne hinzufügen]** Fügt eine Kampagne hinzu. Dazu müssen folgende Elemente markiert sein:
- ein kampagnenfähiger Arbeitsgang
- ein Termin
- eine Schicht

**[Löschen]** Löscht die markierte Kampagne.

**[OK]** Speichert die Daten.

**[Abbrechen]** Schließt den Dialog, ohne die Daten zu speichern.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-190*

## Kampagnen – Wöchentliche Termine

**Stammdaten > Kapazitätsplanung > Kampagnenplanung > Register Wöchentliche Termine**

*Abb. E-108 Kampagnentage – Wöchentliche Termine*

In diesem Register verwalten Sie Serienkampagnen. Mit Serienkampagnen führen Sie regelmäßig wiederkehrende Kampagnen durch.

⇨ Tutorial, "Kampagnen anlegen und verwalten" auf Seite E-47

Eine Beschreibung der Felder im Dialog Kampagnen finden Sie hier:
⇨ "Kampagnen – Einzeltermine" auf Seite E-189

**Wöchentliche Termine** Anzeige der Kampagnen für den markierten Wochentag.
- **Wochentag:** Arbeitstage, zu denen Sie Kampagnen erzeugt haben.
- **Schicht:** Arbeitsschicht, in der die jeweilige Kampagne durchgeführt wird.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-191*

# Abgelaufene Reservierungen

**Stammdaten > Kapazitätsplanung > Reservierungen**

*Abb. E-109 Abgelaufene Reservierungen*

In diesem Dialog werden abgelaufene Reservierungen angezeigt. Der Dialog wird automatisch geöffnet, wenn Sie den Dialog *Reservierungen* öffnen und abgelaufene Reservierungen vorhanden sind.

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

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-192*

**[Löschen]** Löscht die markierte Reservierung.

**[OK]** Speichert die Daten und wechselt zum Fenster *Reservierungen*.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-193*

# Reservierungen

**Stammdaten > Kapazitätsplanung > Reservierungen**

*Abb. E-110 Reservierungen*

In diesem Dialog verwalten Sie Reservierungen von Maschinenkapazitäten. Reservierungen sind nur auf den einzelnen Maschinen möglich, die als Engpassbetriebsmittel definiert sind. Sie sind zeitlich begrenzt. Ein Engpassbetriebsmittel kann nicht über seine Kapazität hinaus bebucht werden.

Die Reservierungen werden entweder für spezifische Kunden oder Bauprojekte angelegt.

Im Produktionsmonitor werden die reservierten Zeiten in den jeweiligen Arbeitsschichten gekennzeichnet.

⇨ Tutorial, "Reservierungen" auf Seite E-54

> **i Reservierungen für einzelne Aufträge**
> Reservierungen von Zeiten für einzelne Aufträge müssen vom ERP-System erfasst und übertragen werden. Die als Reservierungsauftrag gekennzeichneten und zur Produktion freigegebenen Aufträge reservieren auf allen für die Produktion benötigten Maschinen entsprechende Zeiten.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-194*

## Reservierungen

> **i Reservierungen in Schichten, Tagen oder Wochen**
> In der Regel werden Kapazitäten wochenweise reserviert. Je nach Einstellung unter Stammdaten > Konfiguration > A+W Production > Kapazitätsplanung > Art der Reservierung können für die Reservierung aber auch Tage oder Arbeitsschichten angegeben werden. Wenn Sie die Einstellung ändern, gehen die alten Reservierungen verloren.

**Maschine** Auswahl der Maschine, deren Reservierungen angezeigt werden. In der Auswahl-Liste sind alle Maschinen angezeigt, die als Engpassbetriebsmittel definiert sind.

**Starttermin** Beginn des Reservierungszeitraums. Standardmäßig wird der aktuelle Kalendertag angezeigt.

**Tage** Angabe, wie viele Tage in der Vorschau angezeigt werden.

### Schichtreservierungen

Im Bereich Schichtreservierungen werden die Reservierungen ab dem ausgewählten Datum grafisch dargestellt.

**Frei** Freie Kapazität der Maschine.

**Reserviert** Reservierte Kapazität der Maschine.

**Benutzt** Tatsächlich benutzter Anteil der Reservierung.

### Reservierungen pro Kunde

Ist im Bereich Schichtreservierungen ein Tag markiert, wird eine Übersicht mit allen Reservierungen angezeigt.

- **Kunde:** Kunde, für den Kapazitäten reserviert sind.
- **Objekt:** Objekt, für das Kapazitäten reserviert sind.
- **Reservierung:** Reservierte Maschinen-Kapazitäten in Prozent.
- **Benutzt:** Tatsächlich benutzter Anteil der Reservierung in Prozent.
- **Ablaufdatum:** Datum, an dem die Reservierung endet.
- **Datum:** Datum, an dem die Reservierung erfasst wurde.
- **Schicht:** Arbeitsschicht, für die die Reservierung gilt.

**[Neu]** Öffnet den Dialog zum Reservieren von Maschinen-Kapazitäten.
⇨ "Reservierung für Maschine" auf Seite E-197

**[Löschen]** Löscht die markierte Reservierung.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-195*

**[OK]** Speichert die Daten.

**[Ende]** Bricht die Bearbeitung ab und schließt den Dialog.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-196*

# Reservierung für Maschine

**Stammdaten > Kapazitätsplanung > Reservierungen > [Neu]**

*Abb. E-111 Reservierung für Kunde oder Objekt*

In diesem Dialog reservieren Sie Maschinen-Kapazitäten für einen bestimmten Kunden oder ein Objekt.

> **i Reservierungen in Schichten, Tagen oder Wochen**
> In der Regel werden Kapazitäten wochenweise reserviert. Je nach Einstellung unter Stammdaten > Konfiguration > A+W Production > Kapazitätsplanung > Art der Reservierung können für die Reservierung aber auch Tage oder Arbeitsschichten angegeben werden. Wenn Sie die Einstellung ändern, gehen die alten Reservierungen verloren.

**Kunde** Kunde, für den Maschinen-Kapazität reserviert wird. Die [Lupe] öffnet den Dialog Kunde auswählen.
⇨ “Kunde auswählen" auf Seite E-198

**Objekt** Objekt, für das Maschinen-Kapazität reserviert wird. Die [Lupe] öffnet den Dialog Objekt auswählen.
⇨ "Objekt auswählen" auf Seite E-199

**Datum** Beginn des Reservierungszeitraums.

**Schicht** Arbeitsschicht, in der die Maschine reserviert ist.

**Ablaufdatum** Ende des Reservierungszeitraums.

**Reservierung in %** Maschinen-Kapazität in Prozent, die reserviert werden soll.
Sie können die Reservierung als Betrag eingeben oder indem Sie den Balken im Feld darüber mit der Maus aufziehen.

**[OK]** Speichert die Daten.

**[Schließen]** Schließt den Dialog, ohne die Daten zu speichern.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-197*

# Kunde auswählen

**Stammdaten > Kapazitätsplanung > Reservierungen > [Neu] > Kunde**

*Abb. E-112 Kunde auswählen*

In diesem Dialog wählen Sie den Kunden, für den Sie Maschinen-Kapazitäten reservieren wollen.

### Übersicht

- **ID:** Kundennummer.
- **Name:** Name des Kunden.
- **Matchcode:** Matchcode, der dem Kunden zugewiesen wurde.

**Matchcode** Angabe des Matchcodes für die Kundensuche.

**Name** Angabe des Namens für die Kundensuche.

**Anzahl** Anzahl der Kunden, die in der Übersicht angezeigt werden.

**[Suchen]** startet die Suche, wenn Sie im Filterkriterium die Wild Card % eingesetzt haben.

**[OK]** Übernimmt den markierten Kunden in den Dialog *Reservierung für Maschine*.

**[Schließen]** Schließt den Dialog, ohne die Daten zu übernehmen.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-198*

# Objekt auswählen

**Stammdaten > Kapazitätsplanung > Reservierungen > [Neu] > Objekt**

*Abb. E-113 Objekt auswählen*

In diesem Dialog wählen Sie ein Objekt, für das eine Reservierung vorgenommen wird.

### Übersicht

- **ID:** Identifikationsnummer des Objekts.
- **Beschreibung:** Name des Objekts.

**Name** Angabe des Namens für die Objektsuche.

**Anzahl** Anzahl der Objekte, die in der Übersicht angezeigt werden.

**[Suchen]** startet die Suche, wenn Sie im Filterkriterium die Wild Card % eingesetzt haben.

**[OK]** Übernimmt das markierte Objekt in den Dialog *Reservierung für Maschine*.

**[Schließen]** Schließt den Dialog, ohne die Daten zu übernehmen.

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-199*

# Bearbeitungen

Die Bearbeitungen beschreiben die Arbeitsschritte zur Fertigung der Teile. Die Bearbeitungserzeugung stellt sicher, dass für jedes Stücklistenteil beschrieben wird, wie es in der Produktion entsteht. Diese Information ist für A+W Capacity Planner unabdingbar und auch sonst ist es sinnvoll, z.B. auf Papieren die ganze Entstehung der Produkte zu sehen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Bearbeitungserzeugung" auf Seite E-201
- "Existierende Bedingung hinzufügen" auf Seite E-204

---
*4.50/01-2023, A+W Production Kapazitätsplanung, E-200*
