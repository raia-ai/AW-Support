---
description: "D-HB-AWBusiness_20"
---


# Übersichten und Referenzen zu Positionen

---
## Glaskleber

Zur Berechnung des Klebers wählen Sie den zu verwendenden Kleber aus.

**Kanten Breite, Höhe**: Zur Berechnung des verbrauchten Klebers geben Sie die Breite und Höhe der Kanten ein, die verklebt werden.

## Teillieferungen

> Dokumente > Auftrag > Teillieferung

In diesem Dialog können Sie Teillieferungen erstellen und sich eine Übersicht über den Auftragsstatus der Teillieferungen anzeigen lassen.
Der Dialog Teillieferungen ist für Auftrag und Bestellung gleich. Er wird in dieser Anleitung am Beispiel Auftrag beschrieben.

> **Voraussetzungen**
> Teillieferungen können nur ausgelöst werden, wenn diese Funktion in den Kundenstammdaten und in den Kopfdaten des Auftrags aktiviert ist. Wenn zusätzlich eine Teilrechnung gestellt werden soll, muss auch diese Option in den Kundenstammdaten und den Kopfdaten aktiviert sein.
> Eine Teillieferung kann nur ausgelöst werden, wenn mindestens ein Stück einer Auftragsposition aus der Produktion als fertig produziert gemeldet ist. In den Firmenstammdaten wird festgelegt, bei welchem Status eine Position als fertig produziert gilt.

In diesem Dialog finden Sie folgende Register:
- "Teillieferungen – Pro Fertigmeldung / Wareneingang" auf Seite C-1902
- "Teillieferungen – Pro Gestell" auf Seite C-1905

### Teillieferungen – Pro Fertigmeldung / Wareneingang

> Dokumente > Auftrag > Teillieferung > Register pro Fertigmeldung / Wareneingang

*Abb. C-330 Teillieferung - pro Fertigmeldung / Wareneingang*

In diesem Register können Sie Teillieferungen zu Aufträgen des gewählten Nummernverwalters erstellen.

#### Selektion

**Nummernverwalter**: Auswahl des gewünschten Nummernverwalters.

#### Dokumente

In der Übersicht werden alle Dokumente des gewählten Nummernverwalters angezeigt.
Die Dokumente werden in roter oder grüner Schrift angezeigt. In grüner Schrift werden Aufträge und Bestellungen angezeigt, die komplett ausgeliefert sind. Zusätzlich ist die Checkbox in der Spalte Komplett markiert.
In roter Schrift werden Aufträge angezeigt, die noch nicht komplett ausgeliefert sind.

- **Auftrag**: Auftragsnummer.
- **Kunde, Name**: Nummer und Name des Marktpartners aus dem Auftrag.
- **Status**: Status des Auftrags.
- **Fertig %**: Anteil der Positionen, die als fertig produziert gemeldet sind. Der Anteil richtet sich nach der Gesamtstückzahl und wird in Prozent angezeigt.
- **Teillieferfähig %**: Anteil der Positionen, die teilgeliefert werden können. Der Anteil richtet sich nach der Gesamtstückzahl und wird in Prozent angezeigt. Wenn noch keine Positionen des Auftrags teilgeliefert sind, entspricht der Anteil Teillieferfähig % dem Anteil Fertig %.

> **Beispiel**
> Ein Auftrag hat 10 Auftragspositionen, von denen 6 als fertig produziert gemeldet sind. Es wurden noch keine Teillieferungen ausgelöst.
> Der Anteil Fertig % und der Anteil Teillieferfähig % beträgt jeweils 60%.
> Von dem Auftrag werden 2 Auftragspositionen teilgeliefert.
> Der Anteil Fertig % beträgt noch immer 60%, der Anteil Teillieferfähig % jedoch nur noch 40%, da 2 Positionen bereits teilgeliefert wurden und somit nur noch 4 Positionen für die Teillieferung bereitstehen.

- **Komplett**: Die Checkbox ist markiert, wenn der Auftrag komplett ausgeliefert ist.

> **Aufträge manuell als komplett melden**
> Sie können noch nicht fertiggemeldete Aufträge manuell als komplett melden, indem Sie in der Tabellenspalte Komplett die Checkbox aktivieren. Der Dokumentenstatus des markierten Auftrags wird geändert.

#### Positionen

In der Übersicht werden die Positionen des markierten Auftrags aus der Übersicht Dokumente angezeigt.

- **Pos.**: Nummer der Auftragsposition.
- **Status**: Status der Auftragsposition.
- **Fertig %**: Anteil der Positionen, die als fertig produziert gemeldet sind. Der Anteil richtet sich nach der Gesamtstückzahl und wird in Prozent angezeigt.
- **Teillieferfähig %**: Anteil der Positionen, die teilgeliefert werden können. Der Anteil richtet sich nach der fertiggemeldeten Menge und wird in Prozent angezeigt.
- **Menge (original)**: Menge der Auftragsposition.
- **Menge (teilgeliefert)**: Menge, die aus der Position teilgeliefert wurde.
- **Menge (fertig)**: Menge der fertiggemeldeten Auftragsposition.
- **Teilliefermenge**: Menge, zu der eine Teillieferung erstellt werden soll.

Sie können in die Tabellenspalte Teillieferung eintragen, wie viel Stück der fertiggemeldeten Menge teilgeliefert werden sollen.

#### Ziel

**Nummernverwalter**: Das Dokument kann in einen anderen Nummernverwalter gestellt werden, den Sie in der Kombobox wählen können.

**AV-Bereich**: Das Dokument kann einem anderen AV-Bereich zugeordnet werden.
- ☐ Das Dokument wird keinem anderen AV-Bereich zugeordnet.
- ☑ Das Dokument wird dem gewählten AV-Bereich zugeordnet. Die Kombobox zur Auswahl des AV-Bereichs wird freigeschaltet.

### Teillieferungen – Pro Gestell

> Dokumente > Auftrag > Teillieferung > Register pro Gestell

*Abb. C-331 Teillieferung - pro Gestell*

In diesem Register können Sie Teillieferungen zu Auftragspositionen erstellen, die auf ein Gestell gebucht sind. Sie können sich die Auftragspositionen auf einem Gestell nach Nummernverwalter oder nach Kunde anzeigen lassen.

#### Selektion

Mit der Wahl der Option können Sie die Suche auf einen bestimmten Nummernverwalter oder Kunden einschränken.

- **Nummernverwalter**: Auswahl eines Nummernverwalters.
- **Kunde**: Nummer und Name des Kunden.

**Liefertermin von, bis**: Lieferzeitraum der Aufträge, nach denen gesucht werden soll.

**Status von, bis**: Statusnummernbereich der Aufträge, nach denen gesucht werden soll.

#### Gestell - Aufträge

In dieser Übersicht wird angezeigt, von welchen Aufträgen einzelne oder alle Auftragspositionen auf ein Gestell gebucht sind.

- **Gestell**: Gestellnummer, auf die die Auftragsposition gebucht ist.
- **Auftrag**: Auftragsnummer.
- **Kunde, Name**: Nummer und Name des Marktpartners aus dem Auftrag.
- **Liefertermin**: Liefertermin aus dem Auftrag.
- **Status**: Status des Auftrags.
- **Teillieferfähig %**: Anteil der Positionen, die teilgeliefert werden können. Der Anteil richtet sich nach der Gesamtstückzahl und wird in Prozent angezeigt.
- **Teilgeliefert %**: Anteil der Positionen, die bereits teilgeliefert sind. Der Anteil richtet sich nach der Gesamtstückzahl und wird in Prozent angezeigt.

Sie können eine Teillieferung für ein Gestell erstellen, wenn Sie mit Doppelklick den Zeilenkopf des Auftrags für die Teillieferung auswählen. Der ausgewählte Auftrag wird mit einem roten X im Zeilenkopf markiert. Nach Erstellen einer Teillieferung wird der Dialog Formulardruck-/Etikettendruck geöffnet.
⇨ "Formular-/Etikettendruck" auf Seite C-1926

#### Gestell - Positionen

In der Übersicht werden die Positionen des Auftrags angezeigt, der in der Übersicht Gestell-Aufträge markiert ist.

- **Pos.**: Nummer der Auftragsposition.
- **Status**: Status der Auftragsposition.
- **Produkt**: Produktnummer und -bezeichnung.
- **Breite, Höhe**: Maße der Position.
- **Menge (original)**: Menge der Auftragsposition.
- **Menge (auf Gestell)**: Menge der Auftragsposition auf dem Gestell.
- **Menge (teilgeliefert)**: Menge, die aus der Position bereits teilgeliefert ist.

#### Ziel

**Nummernverwalter**: Die erstellten Teillieferungen können in einen anderen Nummernverwalter gestellt werden. Wenn Sie einen neuen Namen eintragen, wird der Nummernverwalter angelegt. Standardmäßig ist der Nummernverwalter ausgewählt, in dem die Aufträge stehen.

**Lieferdatum**: Sie können ein Lieferdatum für die Teillieferung festlegen.
- ☐ Das Lieferdatum wird aus den Kundenstammdaten oder dem Auftrag übernommen.
- ☑ Sie können das Lieferdatum eintragen. Das Feld zur Eingabe wird freigeschaltet.

**LKW**: Sie können einen Lkw für die Teillieferung wählen.
- ☐ Der Lkw wird aus den Kundenstammdaten oder dem Auftrag übernommen.
- ☑ Sie können einen Lkw wählen. Die Kombobox zur Auswahl wird freigeschaltet.

**Tour**: Sie können eine Tour für die Teillieferung wählen.
- ☐ Die Tour wird aus den Kundenstammdaten oder dem Auftrag übernommen.
- ☑ Sie können eine Tour wählen. Die Kombobox zur Auswahl wird freigeschaltet.

**Fahrer**: Sie können einen Fahrer für die Teillieferung wählen.
- ☐ Der Fahrer wird aus den Kundenstammdaten oder dem Auftrag übernommen.
- ☑ Sie können einen Fahrer wählen. Die Kombobox zur Auswahl wird freigeschaltet.

## Makros

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Aufbau > Gruppe Makro

Produktaufbauten können als Makro(befehl) gespeichert werden und stehen dann ohne weitere Eingaben bei der Erfassung zur Verfügung.
Die Dialoge zum Speichern und Verwalten von Makros sind für alle Dokumentenarten gleich. Sie werden in dieser Anleitung am Beispiel Auftrag beschrieben.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Makro sichern" auf Seite C-1908
- "Makro ändern" auf Seite C-1909
- "Makro suchen" auf Seite C-1911
- "Makro kopieren" auf Seite C-1912

### Makro sichern

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Aufbau > Gruppe Makro > Sichern, Löschen

*Abb. C-332 Makro sichern (löschen)*

In diesem Dialog können Sie ein Produkt mit einer komplizierten Stückliste als Makro sichern.
⇨ Tutorial, "Makro speichern" auf Seite C-1420

#### Definition

**Makroname**: Name des neuen Makros, der zur Auswahl in der Positionserfassung angezeigt wird.

**Exakte Suche**: Die Suche nach Makros kann Preise berücksichtigen. Die Checkbox wird nur angezeigt, wenn die Einstellung zur Makro-Preissuche in den Firmendaten aktiviert ist.
- ☐ Das Makro kann ohne den exakten Preis übernommen werden.
- ☑ Das Makro kann mit dem exakten Preis übernommen werden.
⇨ Stammdaten, "Firmendaten - Preisberechnung" auf Seite B-1085

Mit der Wahl der Option legen Sie fest, wie das Makro gespeichert wird:
- **Kundenbezogen**: Das neue Makro wird kundenbezogen gespeichert. Er wird dann nur zur Auswahl angeboten, wenn ein Auftrag für den gewählten Kunden erfasst wird. Das Feld Nummer wird freigeschaltet.
- **Allgemein**: Das neue Makro wird so gespeichert, dass er für alle Kunden zur Auswahl angeboten wird. Das Feld Nummer wird gesperrt.

#### Kunde

**Nummer**: Dieses Feld ist nur freigeschaltet, wenn die Option Kundenbezogen markiert ist. Die Kundennummer kann eingegeben oder über die Lupe ausgewählt werden.

**Name**: Der Kundenname wird aus den Stammdaten übernommen, wenn eine Kundennummer eingetragen ist.

### Makro ändern

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Aufbau > Gruppe Makro > Ändern

*Abb. C-333 Makro ändern*

Über diesen Dialog können Sie gespeicherte Makros bearbeiten.
⇨ Tutorial, "Makros ändern" auf Seite C-1423

#### Auswahl

Die Felder in diesem Bereich sind nur freigeschaltet, wenn der Auswahl-Modus aktiviert ist.

- **Alle Makros**: Die Auswahl wird auf alle gespeicherten Makros ausgedehnt.
- **Kundenbezogene Makros**: Die Auswahl wird auf kundenbezogenen Makros eingeschränkt. Die Felder von und bis werden freigeschaltet.

**Von... bis**: Eingabefelder zum Einschränken der Suche nach kundenbezogenen Makros. Die Suche der Makros beschränkt sich auf die Nummernfolge zwischen den eingegebenen Kundennummern. Diese Felder sind nur freigeschaltet, wenn die Option kundenbezogene Makros markiert ist.

#### Preisänderung

Die Felder in diesem Bereich sind nur freigeschaltet, wenn Makros angezeigt werden.

**Wert**: Betrag, um den der Preis des markierten Makros geändert werden soll.
Mit der Wahl der Option legen Sie fest, wie der Preis geändert werden soll:
- **Absolut** und ein Wert, z. B. 5 oder -5, wenn der Preis um 5 Euro erhöht oder vermindert werden soll.
- **Prozentual** und ein Wert, z. B. 2 oder -2, wenn der Preis um 2 Prozent erhöht oder vermindert werden soll.

#### Rundung

Die Rundung in allen markierten Makros wird auf die ausgewählte Rundungsart gesetzt.

#### Makros

Liste aller Makros, die den Auswahlkriterien entsprechen. Zur Änderung können mehrere Einträge markiert werden (Mehrfachmarkierung).

### Makro suchen

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Aufbau > Gruppe Makro > Suchen

*Abb. C-334 Makro suchen*

In diesem Dialog suchen Sie nach bestimmten Makros. Die Felder sind in den beiden Registern gleich. Die Wahl des Registers schränkt die Suche ein.
⇨ Tutorial, "Makros" auf Seite C-1418

#### Makros

**Name**: Name des Makros, das gesucht werden soll. Das Ergebnis der Suche wird in der Übersicht aufgelistet (Trefferliste).

#### Aufbau

Der Aufbau des Produktes wird angezeigt, wenn in der Trefferliste ein Makro markiert ist.

### Makro kopieren

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Aufbau > Gruppe Makro > Kopieren

*Abb. C-335 Makro kopieren*

In diesem Dialog kopieren Sie ein kundenbezogenes Makro, z. B. zu den Filialen des Kunden oder zu einem anderen Kunden.
⇨ Tutorial, "Makros kopieren" auf Seite C-1426

#### Quelle

**Kunde**: Nummer des Kunden, dessen Makro(s) kopiert werden soll(en).

#### Ziel

Mit der Wahl der Option legen Sie fest, wohin die Makros kopiert werden sollen:

- **Kunde**: Nummer des Kunden, zu dem Makro(s) kopiert werden sollen.
- **Filialen**: Mit dieser Option werden die Filialen des Kunden angezeigt. Wenn mehrere Filialen aufgelistet werden, können diejenigen ausgewählt werden, zu denen das Makro kopiert werden soll.
- **Hauptktn.**: Mit dieser Option werden die Makros einer Filiale zum Hauptkunden kopiert.

#### Optionen

Mit der Wahl der Option legen Sie fest, ob vorhandene Makros gelöscht oder überschrieben werden sollen:

- **Vorhandene Makros im Ziel updaten**: Die neuen Makros werden hinzugefügt. Wenn bereits Makros für den Zielkunden gespeichert sind, bleiben diese unverändert erhalten.
- **Alle Makros im Ziel zuvor löschen**: Vor dem Kopieren werden alle Makros beim Zielkunden gelöscht. Nach dem Kopieren stehen für den Zielkunden nur die neuen Makros zur Verfügung.

## Nummernverwalter

> Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > NV Angebot, NV Auftrag, NV Gutschrift, NV Anfrage, NV Bestellung

Der Dialog Nummernverwalter ist für alle Dokumentenarten gleich. Er wird in dieser Anleitung am Beispiel Auftrag beschrieben.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite C-1914
- "Nummernverwalter" auf Seite C-1917
- "Nummernverwalter kopieren" auf Seite C-1920

### Menü Funktionen

> Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > NV Angebot, NV Auftrag, NV Gutschrift, NV Anfrage, NV Bestellung

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Nummernverwalter zu schließen.
Das Menü ist in folgende Gruppen gegliedert:
- Gruppe Bearbeiten
- Gruppe Dokument
- Gruppe Dokumentenkopie
- Gruppe Übersicht
- Gruppe Export
- Gruppe Produktion
- Gruppe Routenoptimierung

#### Gruppe Bearbeiten

- **Kopieren nach**: Öffnet den Dialog Nummernverwalter Kopieren, um Dokumente in einem Nummernverwalter zu selektieren und diese dann in einen neuen Nummernverwalter zu kopieren.
    - ⇨ Tutorial, "Nummernverwalter kopieren" auf Seite C-1446
    - ⇨ "Nummernverwalter kopieren" auf Seite C-1920
- **Überschreiben**: Leert den gesamten Nummernverwalter. Der Modus wechselt automatisch zu Anlegen.
- **Statusänderung**: Öffnet den Dialog Statusänderung, um den Status manuell umzusetzen und den Nummernverwalter zu ändern.
    - ⇨ "Statusänderung" auf Seite C-1836
- **Kennzeichenänderung**: Öffnet den Dialog Bestellkennzeichen ändern, um die Beschaffungsart zu ändern.
    - ⇨ "Bestellkennzeichen ändern" auf Seite C-1921

#### Gruppe Dokument

- **Dokument anzeigen**: Öffnet den Dialog Dokumentenansicht als Vorschau auf das Dokument.
    - ⇨ "Dokument anzeigen" auf Seite C-1829
- **Historie**: Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des Dokuments.
    - "Historie" auf Seite C-1834
- **Dokumentendaten**: Öffnet den Dialog Dokumente, um ggf. die Termine und den Status in Aufträgen und Bestellungen zu korrigieren.
    - ⇨ "Dokumentendaten" auf Seite C-2030
- **Dokumentenerfassung**: Öffnet das markierte Dokument.
    - ⇨ "Dokument - Kopfdaten" auf Seite C-1687

#### Gruppe Dokumentenkopie

- **Dokumente kopieren**: Öffnet den Dialog Dokumente kopieren, um ein Dokument in den gleichen oder anderen Dokumententyp zu kopieren.
    - ⇨ Tutorial, "Dokumente kopieren" auf Seite C-1505
    - ⇨ "Dokumente kopieren" auf Seite C-1813
- **Teillieferung**: Öffnet den Dialog Dokumente kopieren im Modus Teillieferung, um eine Teillieferung zu erfassen.
    - ⇨ Tutorial, "Teillieferungen" auf Seite C-1517
- **Reklamation**: Öffnet den Dialog Dokumente kopieren im Modus Reklamation, um eine Reklamation zu erfassen.
    - ⇨ Tutorial, "Reklamationen" auf Seite C-1544
- **Anzahlung**: Öffnet den Dialog Dokumente kopieren im Modus Anzahlung, um eine Anzahlung zu erfassen.
    - ⇨ Tutorial, "Anzahlungen" auf Seite C-1535

#### Gruppe Übersicht

- **Artikel-Info**: Öffnet einen Dialog mit detaillierten Informationen zum Produkt, um Preise und Verfügbarkeit zu prüfen.
    - ⇨ "Artikel-Informationen" auf Seite C-1887
- **Teillieferungsübersicht**: Öffnet die Liste der Teillieferungen zum aktuellen Auftrag.
    - ⇨ "Teillieferungsübersicht" auf Seite C-1841
- **Anzahlungsübersicht**: Öffnet die Liste der geleisteten Anzahlungen zum aktuellen Auftrag.
    - ⇨ "Anzahlungsübersicht" auf Seite C-1844

#### Gruppe Export

- **Xternal Dateien erstellen**: Erstellt für alle Bestellungen im Nummernverwalter eine Xternal Datei. Die Funktion ist nur kundenspezifisch freigeschaltet.

#### Gruppe Produktion

- **Produktionsübersicht**: Öffnet den Dialog Übersicht Statusrückmeldungen zum markierten Auftrag. Die Funktion ist gesperrt, wenn Sie im aktuellen Dokument keine Positionen enthalten sind, die an die Produktion übergeben werden sollen.
    - ⇨ "Übersicht Statusrückmeldung" auf Seite C-1860

#### Gruppe Routenoptimierung

Diese Gruppe ist nur freigeschaltet, wenn auf Ihrem System auch A+W Logistics Optimizer installiert ist.

**Nummernverwalter übergeben**: Übergibt Aufträge aus dem Nummernverwalter im Modus Lieferung. Die Auftragsnummern werden an den Logistic Service gesendet, der die erforderlichen Daten aus der Datenbank liest.

### Nummernverwalter Dialog

> Dokumente > Auftrag > NV Auftrag

Der Dialog Nummernverwalter und die zugehörigen Menüs sind für alle Dokumentenarten und Module gleich. Er wird in dieser Anleitung am Beispiel Auftrag beschrieben.

*Abb. C-336 Nummernverwalter*

In diesem Dialog können Sie Nummernverwalter anlegen und verwalten.
⇨ Tutorial, "Nummernverwalter" auf Seite C-1440

#### Identifikation

**Mitarbeiter**: Name des Mitarbeiters, der sich in A+W Business angemeldet hat.

**Nummernverwalter**: Name des ausgewählten Nummernverwalters. Das Feld ist freigeschaltet, wenn Sie einen neuen Nummernverwalter anlegen.
⇨ Tutorial, "Nummernverwalter" auf Seite C-1440

**Auftrag, Statusbereich von bis**: Sie können Dokumente innerhalb einer Folge von Nummern oder von Statusnummern auswählen.

#### Auswahl

In der Liste werden alle angelegten Nummernverwalter angezeigt. Der ausgewählte Nummernverwalter wird im Feld Nummernverwalter angezeigt.

#### Optionen

**Anzeige**: Sie können die Anzeige von Tabellenspalten in der Übersicht ausblenden.
Mit der Wahl des Eintrags **Komplett** werden alle Kopfdaten des Dokumentes angezeigt, bei **Lieferung** werden nur die für die Lieferung relevanten Daten angezeigt.

**Sortierung**: Mit dieser Schaltfläche öffnen Sie den Dialog Nummernverwalter-Sortierung, in dem Sie die Sortierung der Listeneinträge ändern können.
⇨ "Nummernverwalter - Sortierung" auf Seite C-1919

#### Zugriff auf

**Mandant**: Beim Anlegen können den Mandanten auswählen, für den der Nummernverwalter gelten soll.

**Datenbank**: Datenbanken, aus der die Dokumente angezeigt werden, z. B. ein Archiv.

#### Dokumente

In diesem Bereich werden alle Dokumente des ausgewählten Nummernverwalters aufgelistet, die den eingegebenen Kriterien entsprechen.

> **Benutzerdefinierte Spalte einfügen**
> In der Übersicht der Dokumente können benutzerdefinierte Spalten eingefügt werden, die über das Customizing mit beliebigen Daten gefüllt werden können. Wenn Sie sich an Ihren Ansprechpartner bei der A+W Software GmbH, wenn Sie solche Spalten einfügen wollen.

### Nummernverwalter – Sortierung

> Dokumente > Auftrag > NV Auftrag > [Sortierung]

*Abb. C-337 Sortierung*

In diesem Dialog legen Sie fest, wie die Dokumente im Nummernverwalter sortiert werden sollen.
Mögliche Sortierungen sind:
- Kunde/Lieferant + Dokumentennummer
- Kunde/Lieferant + Lieferanschrift + Dokumentennummer
- Matchcode + Dokumentennummer
- Kunde/Lieferant + Lieferschein + Auftrag
- Tournummer + Kunde/Lieferant
- Lieferdatum + Kunde/Lieferant
- Kunde/Lieferant + Bestelltext 1
- Reihenfolge laut Routenoptimierung

> Sammelrechnung, Zahlungsbedingung, Währung und Steuersatz 1+2 werden zusätzlich berücksichtigt, um eine optimale Sortierung für den Sammeldruck zu erreichen.

### Nummernverwalter kopieren

> Dokumente > Auftrag > NV Auftrag > Menü Funktionen > Gruppe Bearbeiten > Kopieren nach

*Abb. C-338 Kopieren*

In diesem Dialog kopieren Sie Auftragsnummern, um sie in einen anderen Nummernverwalter zu stellen, z. B. aus dem Nummernverwalter für die Produktion in den Nummernverwalter für den Lieferscheindruck oder zur Weiterbearbeitung von einem Mitarbeiter zu einem anderen.
⇨ Tutorial, "Nummernverwalter kopieren" auf Seite C-1446

#### Dokument

In diesem Bereich wird angezeigt, zu welcher Dokumentenart der Nummernverwalter gehört.

**Typ**: Dokumententyp der Quelle

#### Quelle, Ziel

**Mitarbeiter**: Auswahl des Mitarbeiters, der für den Nummernverwalter zuständig ist.

**Nummernverwalter**: Auswahl des Nummernverwalters, den Sie kopieren möchten.

### Bestellkennzeichen ändern

> Dokumente > Auftrag > NV Auftrag > Menü Funktionen > Gruppe Bearbeiten > Kennzeichenänderung

*Abb. C-339 Bestellkennzeichen ändern*

In diesem Dialog ändern Sie das Bestellkennzeichen aller Dokumente, die sich in dem aktuellen Nummernverwalter befinden. Dabei ändern Sie die Beschaffungsart und/oder den Lieferanten.
⇨ Tutorial, "Bestellung" auf Seite C-1557

#### Modus

Mit der Wahl der Option legen Sie fest, für welche Positionsebene das Kennzeichen geändert werden soll:
- **Ändern auf Positionsebene**: Das Kennzeichen wird für das Hauptprodukt der Auftragsposition umgesetzt.
- **Ändern auf Stücklistenebene**: Das Kennzeichen wird an den Stücklisten-Komponenten umgesetzt.
- **Alle Gläser bestellen**: Alle Gläser der Aufträge erhalten dasselbe Bestellkennzeichen.

#### Lieferant für alle Glas-Bestellartikel

**Lieferant ändern**: Für die gewählte Option (Ebene) kann der Lieferant geändert werden.
- ☐ Der Lieferant wird nicht geändert. Die Felder des Bereichs sind gesperrt.
- ☑ Der Lieferant wird geändert. Die Felder des Bereichs sind freigeschaltet. Der Name des gewählten Lieferanten wird aus den Stammdaten übernommen.
Beachten Sie dazu die Auswahl der Option im Bereich Modus.

> **Alle Dokumente werden geändert**
> Beachten Sie, dass immer alle Dokumente des Nummernverwalters geändert werden.

#### Ändern auf Dokumentenebene

**Bestellung direkt an den Kunden**: Die Bestellung kann vom Lieferanten direkt an den Kunden ausgeliefert werden.
- ☐ Die Bestellung wird nicht direkt an den Kunden geliefert.
- ☑ Die Bestellung wird direkt an den Kunden geliefert. Diese Einstellung kann sinnvoll sein, wenn die Bestellung nicht für die Fertigung benötigt wird.
Damit wird im Auftrag die Checkbox Direktanlieferung durch den Lieferanten ebenfalls aktiviert. Bei der Bestellübergabe wird dann als abweichende Lieferanschrift die Kundenanschrift eingefügt.
⇨ "Direktanlieferung durch den Lieferanten" auf Seite C-1694

#### Beschaffungsart

**Beschaffungsart ändern**: Für die gewählte Option (Ebene) kann die Beschaffungsart geändert werden.
- ☐ Die Beschaffungsart wird nicht geändert. Die Felder des Bereichs sind gesperrt.
- ☑ Die Beschaffungsart wird geändert. Die Felder des Bereichs sind freigeschaltet.

**Von, nach**: Auswahl der Beschaffungsart, die geändert werden soll und der neuen Beschaffungsart. Die Felder sind nur freigeschaltet, wenn die Checkbox Beschaffungsart ändern markiert ist.

**Nur für Produkt**: Die Änderung der Beschaffungsart kann auf ein einzelnes Produkt eingeschränkt werden. Die Bezeichnung des gewählten Produkts wird aus den Stammdaten übernommen.
Beachten Sie dazu die Auswahl der Option im Bereich Modus.

## Druck

> Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Druck Angebot, Auftrag, Gutschrift, Anfrage, Bestellung

Der Dialog Formular-/Etikettendruck und die zugehörigen Menüs sind für alle Dokumentenarten gleich. Er wird in dieser Anleitung am Beispiel Auftrag beschrieben.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menüs im Formular-/Etikettendruck" auf Seite C-1923
- "Vermaßte Skizze drucken" auf Seite C-1936
- "Formular-/Etikettendruck" auf Seite C-1926
- Touren/Fahrer Zuordnung

### Menüs im Formular-/Etikettendruck

> Dokumente > Auftrag > Auftrag auswählen > Menü Start > Gruppe Druck > Allgemeiner Formulardruck
> Dokumente > Auftrag > Druck Auftrag

Über die Menüs des Druckdialogs können Sie die Standardeinstellung des Dialoges festlegen und Funktionen für den Druck auswählen.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite C-1923
- "Menü Optionen" auf Seite C-1924

#### Menü Funktionen

> Dokumente > Auftrag > Auftrag auswählen > Menü Start > Gruppe Druck > Allgemeiner Formulardruck > Menü Funktionen
> Dokumente > Auftrag > Druck Auftrag > Menü Funktionen

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Formular- und Etikettendruck zu schließen.
Das Menü ist in folgende Gruppen gegliedert:
- Gruppe Allgemeine
- Gruppe Rechnungsdruck
- Gruppe Druck Server

##### Gruppe Allgemeine

- **Touren/Fahrer Zuordnung**: Öffnet den Dialog Touren/Fahrer Zuordnung, in dem Sie der Lieferung einen bestimmten Fahrer zuordnen können. Diese Funktion ist nur beim Druck von Lieferscheinen freigeschaltet.
    - ⇨ "Touren/Fahrer Zuordnung" auf Seite C-1939
- **Dokument anzeigen**: Öffnet den Dialog Dokumentenansicht als Vorschau auf das Dokument.
    - ⇨ "Dokument anzeigen" auf Seite C-1829
- **Vermaßte Skizze drucken**: Öffnet den Dialog Vermaßte Skizze drucken, um eine maßstäbliche Skizze im DIN-A4 Format zu drucken.
    - ⇨ "Vermaßte Skizze drucken" auf Seite C-1936
- **Dokumentendaten**: Öffnet den Dialog Dokumente, um ggf. die Termine und den Status in Aufträgen und Bestellungen zu korrigieren.
    - ⇨ "Dokumentendaten" auf Seite C-2030
- **Artikel Info**: Öffnet einen Dialog mit detaillierten Informationen zum Produkt, um Preise und Verfügbarkeit zu prüfen.
    - "Artikel-Informationen" auf Seite C-1887

##### Gruppe Rechnungsdruck

- **Storno von Rechnungs-/Lieferscheinnummern**: Diese Option ist nur freigeschaltet, wenn in den Firmendaten die Checkboxen für die Nummernvergabe aktiviert sind.
    - ⇨ Stammdaten, “Nummernvergabe pro Seite bei" auf Seite B-1068

##### Gruppe Druck Server

**Druck Server Monitor starten**: Öffnet den Dialog Druckaufträge, in dem eine Liste der aktuellen Druckaufträge angezeigt wird, die zum Drucker-Server gesendet wurden.
⇨ Tutorial, "Druckauftrag" auf Seite C-1455

#### Menü Optionen

> Dokumente > Auftrag > Auftrag auswählen > Menü Start > Gruppe Druck > Allgemeiner Formulardruck > Menü Optionen
> Dokumente > Auftrag > Druck Auftrag > Menü Optionen

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

> **Aktivierte Optionen nach dem Öffnen des Dialogs**
> Bitte beachten Sie, dass geänderte Optionen erst beim nächsten Öffnen des Dialogs wirksam werden.
> Wenn durch eine aktivierte Option eine Prüfung gestartet wurde, kann sich das Öffnen eines Dokuments verzögern. Der Grad der Verzögerung hängt von der Leistungsfähigkeit des Rechners ab.
> Die folgenden Beschreibungen stellen die aktivierte Option dar.

Das Menü ist in folgende Gruppen gegliedert:
- Gruppe Meldungen
- Gruppe Druckoptionen
- Gruppe Druckmodi

##### Gruppe Meldungen

- **Verarbeitungsende melden**: Wenn der Druckauftrag verarbeitet wurde, d. h. an den Drucker oder Server übergeben wurde, wird eine Meldung angezeigt.

##### Gruppe Druckoptionen

- **Inchzeichen drucken**: Wenn Sie mit den Maßen in Inch arbeiten, sollten Sie diese Option aktivieren, damit das Zeichen für Inch (") gedruckt wird.
    - ⇨ Stammdaten, "Maßsystem" auf Seite B-1113
- **Faxnummer im Druckjobname**: Wenn Sie Dokumente per Fax senden, kann die Faxnummer im Namen des Druckauftrags angezeigt werden. Damit können Sie die Druckaufträge besser überwachen. Diese Option gilt für Druck über einen Drucker-Server.
- **E-Mail im Druckjobname**: Wenn Sie Dokumente per Mail senden, kann die E-Mail-Adresse des Marktpartners im Namen des Druckauftrags angezeigt werden. Damit können Sie die Druckaufträge besser überwachen. Diese Option gilt für Druck über einen Drucker-Server.
- **Steuerkorrektur bei Sammelrechnung (Wiederholungsdruck)**: Wenn der Steuersatz in den einzelnen Aufträgen unterschiedlich ist, wird die Steuer im Wiederholungsdruck neu berechnet.
- **Lieferscheindruck mit fertig gemeldeter Menge**: Diese Option ist nur freigeschaltet, wenn zum markierten Dokument eine Rückmeldung aus der Produktion vorliegt.

##### Gruppe Druckmodi

> Dokumente > Auftrag > Druck Auftrag > Gruppe Druckmodi

Mit der Wahl des Druckmodus legen Sie fest, welche Formulare zur Auswahl angeboten werden. Den Druckmodus können Sie auch im Dialog selbst auswählen.
"Druckmodus" auf Seite C-1929

### Formular-/Etikettendruck

> Dokumente > Auftrag > Auftrag auswählen > Menü Start > Gruppe Druck > Allgemeiner Formulardruck
> Dokumente > Auftrag > Druck Auftrag

**Zu Dialogbeschreibung:**
⇨ "Touren/Fahrer Zuordnung" auf Seite C-1939

Der Dialog Formular-/Etikettendruck ist für alle Dokumente gleich. Er wird in dieser Anleitung am Beispiel Auftrag beschrieben. Dokumente werden in vorgegebene Formulare gedruckt und können auf einem Drucker oder auf dem Bildschirm ausgegeben werden.
⇨ Tutorial, "Druck" auf Seite C-1450

> **Einträge in der Gruppe Druck**
> Standardmäßig wird in der Gruppe Druck nur der Eintrag Allgemeiner Formulardruck angezeigt. Sie können eigene Voreinstellungen für den Druck definieren. Diese werden dann ebenfalls zur Auswahl angeboten.
> ⇨ Stammdaten, "Druckaufträge" auf Seite B-1214

In diesem Dialog finden Sie folgende Register:
- "Formular-/Etikettendruck - Formulare" auf Seite C-1927
- "Formular-/Etikettendruck - Etiketten" auf Seite C-1933
- "Formular-/Etikettendruck – Dokumentenexport" auf Seite C-1935

#### Formular-/Etikettendruck – Formulare

> Dokumente > Auftrag > Auftrag auswählen > Menü Start > Gruppe Druck > Allgemeiner Formulardruck > Register Formulare
> Dokumente > Auftrag > Druck Auftrag > Register Formulare

*Abb. C-340 Formular-/Etikettendruck – Formulare*

In diesem Register legen Sie die Optionen für den Druck von Dokumenten fest. In der Formularverwaltung kann angegeben werden, wie viele Exemplare gedruckt werden sollen.
⇨ Stammdaten, "Formularverwaltung - Optionen 1" auf Seite B-1201

##### Selektion nach

**Mitarbeiter**: Name des Mitarbeiters, der sich in A+W Business angemeldet hat.

**Nummernverwalter**: Beim Druck über den Dialog Nummernverwalter können Sie den Nummernverwalter auswählen, in dem die Dokumente für den Druck bereitgestellt sind. Die Dokumente des gewählten Nummernverwalters werden in der Übersicht im Bereich Dokumente angezeigt. Alle weiteren Einstellungen gelten dann für alle Dokumente des Nummernverwalters.
⇨ Tutorial, "Nummernverwalter" auf Seite C-1440
⇨ "Nummernverwalter" auf Seite C-1914

##### Formularauswahl

**Formular**: Zur Auswahl werden die Formulare angeboten, die für den gewählten Druckpunkt zur Verfügung stehen. Das Formular wird automatisch geändert, wenn Sie eine der Checkboxen im Bereich **Sonderdruck** markieren.
⇨ Tutorial, "Formular- und Etikettendruck" auf Seite C-1451
⇨ Stammdaten, "Formularverwaltung" auf Seite B-1195

**Status**: Der Status der Dokumente wird automatisch auf den Status umgesetzt, der dem gewählten Formular zugeordnet ist.
⇨ Stammdaten, "Statusverwaltung" auf Seite B-1020

##### Nummernkreise

**(Präfix)**: Wenn Sie für Ihre AV-Bereiche unterschiedliche Nummernkreise eingerichtet haben, können Sie festlegen, dass die Dokumentennummern aus den zugehörigen Nummernkreisen gezogen werden. Die Felder sind abhängig von der gewählten Einstellung für Lieferscheine (Präfix) und Rechnungen freigeschaltet.
- **0-Vorg. Mandant + Bereich**: Die Felder Mandant und Bereich sind freigeschaltet.
- **1-Doku. Mandant + Bereich**: Der Mandant und der Bereich werden aus dem Dokument übernommen.
- **2-Doku. Mandant + Vorg. Bereich**: Der Mandant wird aus dem Dokument übernommen. Das Feld Bereich ist freigeschaltet.
⇨ Stammdaten, "Funktion der Nummernkreise" auf Seite B-507
⇨ Stammdaten, "Nummernkreise" auf Seite B-1028

**Mandant**: Mandant, aus dessen Nummernkreis die Dokumentennummer gezogen wird.

**Bereich**: Bereich, aus dessen Nummernkreis die Dokumentennummer gezogen wird.

##### Details

**Datenbank**: Wenn Sie mit mehreren Datenbanken arbeiten, müssen Sie die Datenbank auswählen.

**Druckdatum**: Anzeige des aktuellen Tagesdatums (Systemdatum). Es kann nur bei Rechnungen geändert werden, bei denen das Rechnungsdatum die Zahlungsfristen bestimmt.

##### Ausgabe auf

Mit der Wahl der Option legen Sie fest, wie die Dokumente ausgegeben werden.

- **Drucker**: Die Dokumente werden direkt an den Drucker übergeben und gedruckt. Wenn keine anderen Einstellungen im Bereich Sonderdruck aktiviert sind, werden Dokumente auf Papier gedruckt. Diese Einstellung sollten Sie dann wählen, wenn Sie Dokumente für den Post- oder Faxversand fertig machen möchten. Wenn Sie im Bereich Sonderdruck eine oder mehrere Checkboxen aktivieren, werden aus dem Nummernverwalter die entsprechenden Dokumente ausgefiltert.
- **Bildschirm**: Ein einzelnes Dokument wird auf dem Bildschirm angezeigt und kann geprüft werden. Es kann aus dieser Anzeige heraus gedruckt werden. Auch die Ausgabe auf den Bildschirm gilt als Druck, nach dem Sie weitere Drucke nur starten können, wenn Sie im Bereich Sonderdruck die Checkbox Wiederholungsdruck markiert haben. Auch wenn Sie die Checkbox Sammeldruck markiert haben, wird nur das Dokument angezeigt, das in der Übersicht markiert ist.
- **Datei**: Alle aufgelisteten Dokumente werden als Dateien gespeichert und können dann elektronisch (per Datenaustausch) weitergegeben werden.
- **Server**: Die Dokumente werden auf dem Drucker-Server gespeichert und von dort automatisch weiter verarbeitet. Die Option Server ist nur freigeschaltet, wenn mit dem Print-Server gearbeitet wird.

> **Vor dem Druck Bildschirmausgabe erzeugen**
> Wenn Sie Dokumente mit maßstäblichen Skizzen drucken möchten, sollten Sie sich das Dokument zunächst auf dem Bildschirm anzeigen lassen. Sie können dann prüfen, ob z. B. die Beschriftung und die Maße korrekt dargestellt werden. Wenn Korrekturen im Skizzendruck notwendig sind, können Sie die Skizzen über den S+N-Editor bearbeiten.

##### Druckmodus

Die Auswahl aus dieser Kombobox steht auch über das Menü Druckmodi zur Verfügung. Der Druckmodus bestimmt, welche Art von Formular gedruckt wird. Die Auswahl gilt jeweils für alle Dokumente, die in der Übersicht aufgelistet sind. Über den Druckmodus werden die zugeordneten Formulare im gleichnamigen Feld zur Auswahl angeboten.

- **Auftrag**: Mit dieser Auswahl werden Auftragsbestätigungen gedruckt.
- **Fertigungsschein**: Mit dieser Auswahl werden Fertigungsscheine gedruckt.
- **Lieferschein**: Mit dieser Auswahl werden Lieferscheine und Teillieferscheine gedruckt.
- **Rechnung**: Mit dieser Auswahl werden Anzahlungsrechnungen, Rechnungen und Teilrechnungen gedruckt.
- **Sonstige**: Mit dieser Auswahl können spezielle Ausgaben erzeugt werden, z. B. Rechnungen für ein Daten-Management-System (DMS).
- **Gutschrift**: Mit dieser Auswahl werden Gutschriften gedruckt. Es steht Ihnen in diesem Bereich die zusätzliche Auswahl Sonstige zur Verfügung. Mit dieser Einstellung wird keine Rechnungsnummer vergeben.

##### Formularsprache

In diesem Feld wird die Sprache angezeigt, in der die Dokumente gedruckt werden. Die Anzeige ist nur vorhanden, wenn mit Mehrsprachigkeit gearbeitet wird.

##### Sonderdruck

Über diese Checkboxen legen Sie die Kriterien fest, nach denen Dokumente aus dem Nummernverwalter gefiltert werden. Dokumente, auf die die Kriterien nicht zutreffen, werden nicht gedruckt. Zusätzlich geben Sie damit an, wie die Dokumente gesendet werden sollen.

**Wiederholungsdruck**: In der Regel kann ein Dokument nur einmal gedruckt werden. Sie können jedoch beliebig viele Wiederholungsdrucke starten. Ob Sie einen Wiederholungsdruck starten müssen oder nicht, können Sie am Status des Dokuments erkennen, der in der Übersicht in der gleichnamigen Spalte angezeigt wird.
- ☐ Das Dokument wird zum ersten Mal gedruckt. Bei Lieferscheinen, Fertigungsscheinen und Rechnungen wird automatisch eine Dokumentennummer erzeugt, z. B. die Rechnungsnummer.
- ☑ Das Dokument wird als Wiederholungsdruck ausgegeben und erhält keine neue Nummer.

**Dokumentenarchivierung**: Die Dokumente können an ein externes Archiv übergeben werden.
- ☐ Die gedruckten Dokumente werden nicht extern archiviert.
- ☑ Die Dokumente werden an das externe Archiv übergeben.

**Sammelausdruck**: Als Sammeldruck können alle Dokumente für einen Kunden ausgegeben werden, die im Nummernverwalter aufgelistet sind. Dazu muss in den Stammdaten und/oder im Dokument das Kennzeichen für den Sammeldruck aktiviert sein.
- ☐ Die Dokumente der angezeigten Liste werden einzeln gedruckt.
- ☑ Die Dokumente im gewählten Nummernverwalter werden als Sammeldruck ausgegeben. Die Kombobox wird freigeschaltet. Zum Filtern der Dokumente stehen folgende Kriterien zur Wahl:
    - **Immer**: Diese Einstellung überschreibt die Einstellung zum Sammeldruck aus den Stammdaten.
    - **Pro Bestelltext 1**: Alle Dokumente für einen Kunden werden nach dem Bestelltext 1 gefiltert und zusammengefasst. Wenn z. B. für einen Kunden 10 Aufträge vorhanden sind, von denen fünf den gleichen Bestelltext 1 haben, werden sechs Auftragsbestätigungen gedruckt.
    - **Pro Lieferadresse**: Alle Dokumente mit derselben Lieferanschrift werden zusammengefasst.
    - **Standard**: Alle Dokumente mit demselben Kunden/Lieferanten werden zusammengefasst, wenn das Kennzeichen für den Sammeldruck gesetzt ist.
        - ⇨Tutorial, "Sammelrechnungsdruck" auf Seite C-1287
        - ⇨ "Teillieferung, Teilfaktura, Sammelrechnung" auf Seite C-1697

> **Rechnungen für den Sammeldruck sortieren**
> Die Sammelrechnungen werden beim Druck nicht nach Kriterien sortiert. Sie müssen die Rechnungen vor dem Druck im Nummernverwalter so sortieren, dass der Sammelrechnungsdruck sinnvoll ausgeführt wird.
> ⇨ "Sortierung" auf Seite C-1918

**Einschränkung**: Mit der Wahl der Option legen Sie fest, ob bestimmte Dokumente vor dem Druck herausgefiltert werden:
- **Alle Dokumente**: Der Betrag der Dokumente wird nicht geprüft.
- **Betrag ungleich 0**: Alle Dokumente mit einem positiven oder negativen Betrag werden gedruckt, z. B. Rechnungen mit einem negativen Betrag, die als Gutschriften gewertet werden.
- **Betrag größer 0**: Alle Dokumente mit einem Betrag über null werden gedruckt.
- **Alle Dokumente mit Positionen**: Alle Dokumente mit Positionen werden gedruckt, der Ausdruck von Dokumenten ohne Positionen wird unterdrückt.

**Faxversand**: Die Dokumente können direkt als Fax versendet werden. Dazu muss in den Stammdaten das Kennzeichen für den Versand per Fax aktiviert sein. Diese Einstellung kann im einzelnen Dokument geändert werden.
- ☐ Die Dokumente sollen nicht automatisch per Fax versendet werden.
- ☑ Die Dokumente werden automatisch als Fax versendet, sofern eine Faxnummer hinterlegt ist. Dokumenten ohne Faxnummer werden nicht gedruckt und nicht gesendet.
⇨ Stammdaten, “Verbindungen" auf Seite B-890

> **Faxnummer muss angegeben sein**
> Für den Versand als Fax muss für den Adressaten eine Faxnummer hinterlegt sein. Bedenken Sie, dass beim Faxversand die Skizzen ggf. nicht korrekt gedruckt werden können.

**Faxversand an Vertreter**: Die Dokumente können automatisch an den zuständigen Vertreter gesendet werden. Dazu muss der Vertreter im Dokumentenkopf angegeben sein. Wenn für den Vertreter keine Faxnummer hinterlegt ist, wird das Dokument nicht gedruckt und gesendet.
- ☐ Die Dokumente werden nicht an den Vertreter gesendet.
- ☑ Die Dokumente werden an den angegebenen Vertreter gesendet.
⇨ "Vertreter" auf Seite C-1664

> **Faxversand wahlweise an den Kunden oder den Vertreter**
> Sie können für den Versand der Dokumente nur eine der beiden Checkboxen markieren. Wollen Sie die Dokumente sowohl an den Kunden als auch an den Vertreter senden, so müssen Sie den Druck mit der geänderten Einstellung ein zweites Mal starten.

**Mail**: Die Dokumente können als PDF-Datei per E-Mail an den Kunden oder den zuständigen Vertreter gesendet werden. Dazu muss in den Stammdaten das Kennzeichen für den Versand per E-Mail aktiviert sein. Diese Einstellung kann im einzelnen Dokument geändert werden.
- ☐ Die Dokumente sollen nicht automatisch per E-Mail gesendet werden.
- ☑ Alle Dokumente werden automatisch als E-Mail gesendet, sofern eine E-Mail-Adresse hinterlegt ist. Die Checkbox Interaktion und die Optionen an Kunde und an Vertreter werden freigeschaltet. Dokumenten ohne E-Mail-Adresse werden nicht gedruckt und nicht gesendet.
    - **an Kunde**: Die Dokumente werden per E-Mail an den Kunden gesendet.
    - **an Vertreter**: Die Dokumente werden per E-Mail an den Vertreter gesendet.
⇨ Stammdaten, "Dokumentenversand" auf Seite B-893
⇨ "Fax, Mail" auf Seite C-1689

> **E-Mail-Adresse muss angegeben sein**
> Für den Versand als E-Mail muss für den Adressaten eine E-Mail-Adresse hinterlegt sein. Bedenken Sie, dass beim E-Mail-Versand die Skizzen ggf. nicht korrekt gedruckt werden können.
> Sie können für den Versand der Dokumente nur eine der beiden Optionen markieren. Wollen Sie die Dokumente sowohl an den Kunden als auch an den Vertreter senden, so müssen Sie die Checkbox Interaktion markieren und die zweite E-Mail-Adresse manuell eingeben.

**Interaktion**: Dokumente können direkt als E-Mail versendet werden oder Sie können eine Anmerkung dazu schreiben.
- ☐ Die Dokumente werden direkt per E-Mail an den Kunden oder den Vertreter gesendet.
- ☑ Vor dem Versand wird der Browser-Dialog geöffnet und Sie können zusätzliche Anmerkungen oder eine zweite E-Mail-Adresse hinzufügen. Danach müssen Sie den Versand manuell starten.

**Nur Postversand**: Die Informationen für den Dokumentenversand werden aus den Stammdaten des Kunden/Lieferanten übernommen und können im Dokumentenkopf geändert werden.
- ☐ Alle Dokumente werden gedruckt.
- ☑ Aus dem Nummernverwalter werden alle Dokumente herausgefiltert, bei denen weder das Kennzeichen für den Fax- noch für den Mail-Versand gesetzt ist.
⇨ Stammdaten, “Partnerverwaltung - Auftrag" auf Seite B-892
⇨ "Fax, Mail" auf Seite C-1689

##### Dokumente

In der Übersicht werden alle Dokumente aufgelistet, die sich in dem gewählten Nummernverwalter befinden. Wenn Sie den Druckdialog über die Dokumentenverwaltung geöffnet haben, wird nur das aktuelle Dokument angezeigt.
⇨ "Nummernverwalter" auf Seite C-1914

#### Formular-/Etikettendruck – Etiketten

> Dokumente > Auftrag > Auftrag auswählen > Menü Start > Gruppe Druck > Allgemeiner Formulardruck > Register Etiketten
> Dokumente > Auftrag > Druck Auftrag > Register Etiketten

*Abb. C-341 Formular-/Etikettendruck – Etiketten*

In diesem Register legen Sie die Optionen für den Druck von Etiketten fest.

##### Selektion nach, Details, Ausgabe auf, Dokumente

Diese Felder sind ausführlich zum Register Formulare beschrieben.
"Formular-/Etikettendruck - Formulare" auf Seite C-1927

##### Etikettenauswahl

**Etikett**: Etiketten können direkt aus A+W Business heraus gedruckt werden, wenn der Etikettendruck nicht über die Produktion gesteuert wird.
⇨ "Produktionsetiketten" auf Seite C-1708
⇨ "Etikettenparameter" auf Seite C-1708

**Status**: Der Status der Dokumente wird automatisch auf den Status umgesetzt, der dem gewählten Formular zugeordnet ist.

##### Druckmodus

Mit der Wahl der Option legen Sie fest, wie viele Etiketten gedruckt werden müssen:
- **Pro Einheit**: Für jede Bestelleinheit wird ein Etikett gedruckt. Beispielsweise wird für ein 3-fach ISO ein Etikett gedruckt, bei 5 Einheiten also 5 Etiketten.
- **Pro Position**: Für jede Position wird nur ein Etikett gedruckt, z. B. für 5 ISO-Einheiten nur ein Etikett.
- **Pro Auftrag**: Für den gesamten Auftrag wird nur ein Etikett gedruckt, unabhängig davon, wie viele Positionen und wie viele Stücke der Auftrag umfasst.
- **Nach Dokumenteneinstellung**: Der Druck richtet sich nach den Angaben aus dem Dokument. Mit dieser Einstellung können Sie für gemischte Aufträge genau die Etiketten drucken, die pro Position oder Scheibe erforderlich sind.
⇨ "Etikettenparameter" auf Seite C-1708

##### Sonderdruck

**Wiederholungsdruck**: Wenn für den Etikettendruck ein Sperrstatus eingerichtet ist, muss der Wiederholungsdruck gesondert gekennzeichnet werden.
- ☐ Die Etiketten werden im regulären Druck gedruckt.
- ☑ Der Druck für die Etiketten soll wiederholt werden.

**Nicht optimierte Gläser**: Von Hand zugeschnittene Gläser sind nicht durch die Optimierung gelaufen und müssen gekennzeichnet werden, z. B. bei Modellen.
- ☐ Der Zuschnitt wurde über XOpt gesteuert.
- ✔ Für diese Position sollen Etiketten ausgedruckt werden.

#### Formular-/Etikettendruck – Dokumentenexport

> Dokumente > Auftrag > Auftrag auswählen > Menü Start > Gruppe Druck > Allgemeiner Formulardruck > Register Dokumentenexport
> Dokumente > Auftrag > Druck Auftrag > Register Dokumentenexport

*Abb. C-342 Formular-/Etikettendruck – Dokumentenexport*

In diesem Register können Sie den Export von Dokumenten prüfen.

##### Dokumentenexport-Pool

In der Übersicht werden alle Dokumente aufgelistet, die übergeben werden sollen.

**[Löschen]**: Die Schaltfläche ist nur freigeschaltet, wenn ein Fehler bei der Übertragung festgestellt wurde. Mit dieser Schaltfläche löschen Sie einen Eintrag aus dem Übertragungspool.

**[Aktivieren]**: Die Schaltfläche ist nur freigeschaltet, wenn ein Fehler bei der Übertragung festgestellt wurde. Wenn ein Fehler festgestellt wurde, können Sie die Daten korrigieren und erneut zur Übertragung übergeben. Sie lösen die Übertragung mit [Aktivieren] aus.

**[Abfragen]**: Mit dieser Schaltfläche aktualisieren Sie die Anzeige, um den Übertragungsstatus zu prüfen.

### Vermaßte Skizze drucken

> Dokumente > Auftrag > Auftrag auswählen > Menü Start > Gruppe Druck > Vermaßte Skizze drucken
> Dokumente > Auftrag > NV Auftrag > Menü Druck > Gruppe NV Druck > Vermaßte Skizze drucken

*Abb. C-343 Vermaßte Skizze drucken*

In diesem Dialog können Sie eine maßstäbliche Skizze im Format DIN A4 drucken.
⇨ Tutorial, "Druck von Skizzen" auf Seite C-1456

> **Voraussetzung**
> Um vermaßte Skizzen zu drucken, muss die Funktion in den Firmendaten aktiviert sein.
> ⇨ Stammdaten, "Firmendaten - Druck" auf Seite B-1122

**Nummernverwalter**: Auswahl des Nummernverwalters. In der Übersicht im Bereich Dokumente werden nur die Positionen angezeigt, in denen der Skizzendruck von Modellen oder Sprossen auf maßstäblich gesetzt ist. Wenn Sie den Druck für ein einzelnes Dokument starten, ist diese Anzeige ohne Bedeutung.

#### Formularauswahl

**Formular**: Zur Auswahl werden die Formulare angeboten, die für den Skizzendruck zur Verfügung stehen. Das Formular wird automatisch geändert, wenn Sie eine der Checkboxen im Bereich **Sonderdruck** markieren.

#### Ausgabe auf

Mit der Wahl der Option legen Sie fest, wie die Dokumente ausgegeben werden.

- **Drucker**: Die Dokumente werden direkt an den Drucker übergeben und gedruckt. Wenn keine anderen Einstellungen im Bereich Sonderdruck aktiviert sind, werden Dokumente auf Papier gedruckt. Diese Einstellung sollten Sie dann wählen, wenn Sie Dokumente für den Post- oder Faxversand fertig machen möchten. Wenn Sie im Bereich Sonderdruck eine oder mehrere Checkboxen aktivieren, werden aus dem Nummernverwalter die entsprechenden Dokumente ausgefiltert.
- **Bildschirm**: Ein einzelnes Dokument wird auf dem Bildschirm angezeigt und kann geprüft werden.

> **Vor dem Druck Bildschirmausgabe erzeugen**
> Sie sollten sich das Dokument zunächst auf dem Bildschirm anzeigen lassen. Sie können dann prüfen, ob z. B. die Beschriftung und die Maße korrekt dargestellt werden. Wenn Korrekturen im Skizzendruck notwendig sind, können Sie die Skizzen über den S+N-Editor bearbeiten.

#### Druckmodus

Mit der Wahl der Option legen Sie fest, wie der Druck gesendet wird:
- **Ausdruck**: Der Druck wird an einen Drucker gesendet.
- **Fax**: Der Druck wird an ein Faxgerät gesendet.
- **Mail**: Der Druck wird als PDF-Datei ausgegeben und kann per E-Mail gesendet werden. Für diese Einstellung muss im Auftrag der Versand der Auftragsbestätigung als Mail aktiviert sein.
⇨ "Fax, Mail" auf Seite C-1689

#### Optionen

- **Um Rechteckscheiben mit Bearbeitungen erweitern**: In der Regel werden Rechteckscheiben nur angezeigt, wenn in ihnen Sprossen enthalten sind.
    - ☐ Rechteckscheiben werden nicht angezeigt, wenn in ihnen keine Sprossen enthalten sind.
    - ☑ Rechteckscheiben mit Bearbeitungen werden auch angezeigt.
- **Auswahl auf EFG, ESG und VSG beschränken**: Die Anzeige der Positionen kann auf Einfachglas, ESG und VSG eingeschränkt werden.
    - ☐ Die Anzeige der Positionen wird nicht weiter eingeschränkt.
    - ☑ Die Anzeige der Positionen wird auf EFG, ESG und VSG eingeschränkt.
- **Um Ganzglastüranlagen erweitern**: Positionen mit Ganzglastüren werden in der Regel nicht angezeigt.
    - ☐ Ganzglastüren werden nicht angezeigt.
    - ☑ Positionen mit Ganzglastüren werden angezeigt.
- **Sprossenzuschnittsliste ausgeben**: Details zu den Sprossen können zusätzlich gedruckt werden.
    - ☐ Nur die Sprossenskizze wird gedruckt.
    - ☑ Längen und Zuschnittsinfos der einzelnen Sprossenstäbe werden in eine Detailliste gedruckt. Damit können die Sprossen anhand des Ausdrucks gefertigt werden.
- **Template Variablennamen nicht anzeigen**: Variablennamen aus einem SN-Template können ausgeblendet werden.
    - ☐ Variablennamen werden angezeigt, z. B. Scheibenbreite.
    - ☑ Variablennamen werden nicht angezeigt.

#### Sonderdruck

- **Erweitert**: Hierbei können Sie die Funktion Erweiterte Modellskizze auswählen, um maßstäbliche Skizzen von Modellen und Sprossen auf ein separates Blatt zu drucken.
- **Produktskizze**: Produktbild aus den Produktstammdaten. Es kann nur gedruckt werden, wenn in der Produktverwaltung die Checkbox Druck auf Formular aktiviert ist. Das Produktbild gibt das Produkt selbst wieder. Es zeigt weder das Modell noch die eingebauten Sprossen. Es ist daher nur für seltene Strukturgläser sinnvoll.
    - ⇨ Stammdaten, "Artikelskizze" auf Seite B-711

#### Dokumente

In diesem Bereich werden alle Dokumente des Nummernverwalters aufgelistet, in denen Positionen mit Sprossen oder Modellen erfasst sind.
- Mit den oberen Schaltflächen können Sie alle Positionen markieren oder alle Markierungen entfernen.
- Mit den unteren Schaltflächen können Sie die Positionen markieren, in denen Sprossen oder Modelle enthalten sind.

### Touren/Fahrer Zuordnung

> Dokumente > Auftrag > Druck Auftrag > Menü Funktionen > Gruppe Allgemein > Touren/Fahrer Zuordnung

*Abb. C-344 Touren/Fahrer Zuordnung*

In diesem Dialog können Sie sich die Touren zu Lieferscheinen anzeigen lassen, die zum Datum des markierten Auftrags gefahren werden.
Die Funktion ist nur freigeschaltet, wenn der Druckmodus Lieferschein eingestellt ist.
Sie können den Touren jeweils einen Fahrer zuordnen, so dass der Name des Fahrers auf den Lieferscheinen gedruckt wird.

## Übergabe Bestellungen

> Dokumente > Auftrag > Bestellübergabe

Bestellungen aus den Aufträgen können direkt an die Lieferanten übergeben werden.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Bestellübergabe" auf Seite C-1940
- "Lieferant und Liefertermin ändern" auf Seite C-1949
- "Markierungsoptionen" auf Seite C-1950
- "Preisvergleich" auf Seite C-1951
- "Erweiterte Einstellungen" auf Seite C-1953
- "Stücklistenübersicht" auf Seite C-1957

### Bestellübergabe

> Dokumente > Auftrag > Bestellübergabe

Mit der Bestellübergabe werden die Produkte aus den Aufträgen herausgefiltert, die bestellt werden müssen.
⇨ Tutorial, "Bestellübergabe" auf Seite C-1558

> **Voraussetzung**
> Nur wenn die Lieferantenkartei korrekt geführt ist, können Bestellungen zu Aufträgen direkt erzeugt werden.
> ⇨ Stammdaten, "Lieferantenkartei" auf Seite B-987

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite C-1940
- "Menü Optionen" auf Seite C-1941
- "Bestellübergabe - Bestellnummern" auf Seite C-1943
- "Bestellübergabe - Bestellpool" auf Seite C-1946

#### Menü Funktionen

> Dokumente > Auftrag > Bestellübergabe > Menü Funktionen

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Bestellübergabe zu schließen. Folgende Einträge werden angezeigt:

- **Lieferant/Liefertermine ändern**: Öffnet den Dialog Lieferant und Liefertermin ändern.
    - "Lieferant und Liefertermin ändern" auf Seite C-1949
- **Markierungsoptionen**: Öffnet den Dialog Markierungsoptionen.
    - ⇨ "Markierungsoptionen" auf Seite C-1950
- **Lieferantenpreise**: Öffnet den Dialog Preisvergleich.
    - ⇨ "Preisvergleich" auf Seite C-1951

#### Menü Optionen

> Dokumente > Auftrag > Bestellübergabe > Menü Optionen

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

> **Aktivierte Optionen nach dem Öffnen des Dialogs**
> Bitte beachten Sie, dass geänderte Optionen erst beim nächsten Öffnen des Dialogs wirksam werden. Wenn durch eine aktivierte Option eine Prüfung gestartet wurde, kann sich das Öffnen eines Dokuments verzögern. Der Grad der Verzögerung hängt von der Leistungsfähigkeit des Rechners ab. Die folgenden Beschreibungen stellen die aktivierte Option dar.

Das Menü ist in folgende Gruppen gegliedert:
- Gruppe Übergabe
- Gruppe Liefertermin
- Gruppe Produktbezeichnung
- Gruppe Sonstige
- Gruppe Erweitert

##### Gruppe Übergabe

- **Auftragsbezogene Übergabe**: Die Bestellungen werden pro Auftrag übergeben. Wenn diese Option nicht aktiviert ist, können Sammelbestellungen erzeugt werden.
- **Bestellnummer = Auftragsnummer**: Diese Option ist nur freigeschaltet, wenn die Option Auftragsbezogene Übergabe aktiviert ist.
- **Bestellpool pro Mitarbeiter**: Pro Mitarbeiter kann ein eigener Bestellpool angelegt werden.

##### Gruppe Liefertermin

- **Lieferterminprüfung**: Der Liefertermin wird automatisch geprüft. Ändern Sie einen Liefertermin, der nicht an einem Tourentag liegt, wird eine entsprechende Meldung angezeigt.
- **Lieferantentour berücksichtigen**: Wenn die Bestellung auf einen Liefertermin fällt, der nicht an einem Tourentag liegt, wird eine entsprechende Meldung angezeigt. Dazu müssen die Lieferantentouren in den Stammdaten hinterlegt werden.
    - ⇨ Stammdaten, "Touren" auf Seite B-995
- **Lieferantentour ignorieren bei Direktanlieferung**: Wenn die Bestellung direkt zum Kunden geliefert wird, können Lieferantentouren ignoriert werden.
- **Vorlauftage mit Kombiwarengruppen ermitteln**: Wenn in den Kombiwarengruppen Vorlauftage hinterlegt sind, sollen diese zur Berechnung des Liefertermins herangezogen werden.
    - ⇨ Stammdaten, "Vorlauftage" auf Seite B-681

##### Gruppe Produktbezeichnung

- **Produktbezeichnung aus Lieferantenkartei**: Die Bezeichnung der bestellten Produkte wird aus der Lieferantenkartei übernommen.
- **Produktbezeichnung aus Basisdaten (interne Best.)**: Für interne Bestellungen wird die Bezeichnung der bestellten Produkte aus den Produktstammdaten übernommen.

##### Gruppe Sonstige

- **Keine Kostenrückschreibung**: Die Kosten werden nicht in die EK-Preise des Auftrags zurückgeschrieben.
- **Maßzuschläge berücksichtigen**: Bei der Bestellung sollen die Maßzuschläge mit übergeben werden.
- **Rückschnitt vom Abstandhaltermaß abziehen**: Der Rückschnitt von Abstandhaltern wird in der Breite und Höhe der Bestellung abgezogen, jedoch nur, wenn keine Sprossen mitbestellt werden. Im Fall von unterschiedlichen Modellkanten wird der Rückschnitt vom Abstandhaltermaß immer abgezogen.
- **Druckkennzeichen für Bearbeitungen immer setzen**: In der Bestellung sollen Bearbeitungen immer gedruckt werden. Wenn die Option deaktiviert ist, werden die Druckkennzeichen unverändert aus dem Auftrag in die Bestellung übernommen.
- **Statistikwarengruppe aus dem Auftrag**: Die Angabe zur Statistikwarengruppe wird aus dem Auftrag übernommen, wenn für Auftrag und Bestellung unterschiedliche Statistikwarengruppen definiert sind.
- **Geschäftsart aus dem Auftrag**: Die Geschäftsart wird aus dem Auftrag übernommen, wenn für Auftrag und Bestellung unterschiedliche Geschäftsarten definiert sind.
- **AV-Bereich aus dem Auftrag**: Der AV-Bereich wird aus dem Auftrag übernommen, wenn für Auftrag und Bestellung unterschiedliche AV-Bereiche definiert sind.
- **Fachberater = Erfasser bei Neuanlage**: In der Bestellung wird automatisch der Name des Mitarbeiters eingetragen, der sich in A+W Business angemeldet hat.
- **Statusänderung erfragen**: Die Abfrage zur Änderung des Status wird angezeigt.
- **Wiederholte Übergabe nur bis Sperrstatus**: Bestellungen können mehrfach übergeben werden, allerdings nur, bis der Sperrstatus erreicht ist.
- **Autom. Zuschl.-Kennz. aus Produkten einlesen**: Die Zuschlagskennzeichen immer wieder aus dem Artikelstamm einlesen.

##### Gruppe Erweitert

- **Einstellungen**: Öffnet den Dialog Erweiterte Einstellungen, um Angaben zum Druck von Texten und Dateianhängen festzulegen.
    - ⇨ "Erweiterte Einstellungen" auf Seite C-1953

### Bestellübergabe – Bestellnummern

> Dokumente > Auftrag > Bestellübergabe > Register Bestellnummern

*Abb. C-345 Bestellübergabe - Bestellnummern*

In diesem Register wählen Sie den Übergabe-Modus aus. Die sofort an den Einkauf übergebenen Bestellungen können Sie sich im Dialog Bestellungen anzeigen lassen.
⇨ Tutorial, "Bestellübergabe" auf Seite C-1558

#### Modus

Mit der Wahl der Option legen Sie die Form der Übergabe von Bestellpositionen fest:
- **Pool füllen**: Mit dieser Option werden die Auftragspositionen mit Bestellteilen im Register Bestellpool angezeigt und können vor der Übergabe geprüft werden.
- **Sofort bestellen**: Mit dieser Option werden die Daten sofort an den Standard-Lieferanten übergeben. Diese Option ist dann sinnvoll, wenn Sie zuvor keine Preise oder Liefertermine prüfen möchten und die Lieferantenkartei entsprechend gepflegt ist.
- **Sofort anfragen**: Die Bestellungen werden zur Anfrage an die Standard-Lieferanten übergeben.

#### Selektion nach Nummernverwalter

**Name**: Auswahl des Nummernverwalters, in dem die Aufträge zusammengefasst sind, die übergeben werden sollen.

#### Dokumente

- **Auftragsnummer**: Auftragsnummer aus dem Auftragskopf
- **Bestellnummer(n)**: Wenn Aufträge bereits übergeben wurden, werden die Bestellnummern angezeigt.
- **Kundennummer, Kunde**: Kundennummer und Kundenname aus dem Auftragskopf bzw. den Stammdaten.
- **Status**: Aktueller Status des Auftrags. Bei neuen Aufträgen ist das in der Regel der Mindest-Status, z. B. Dokument gedruckt.
- **Datum Erfassung**: Datum, an dem der Auftrag erstellt wurde.
- **Datum Auslieferung**: Datum, an dem der Auftrag ausgeliefert wird.
- **Datum AB**: Datum, an dem die Auftragsbestätigung gedruckt wurde.
- **Sperr-KZ**: Ggf. Sperr-Kennzeichen des Auftrags.

#### Ziel-Nummernverwalter

**Mitarbeiter**: Name des Mitarbeiters, in dessen Nummernverwalter die erzeugten Bestellungen gestellt werden sollen.

**Name**: Nummernverwalters, in den die Bestellungen gestellt werden sollen. Wenn Sie einen neuen Namen eintragen, wird ein neuer Nummernverwalter angelegt.
⇨ Tutorial, "Nummernverwalter" auf Seite C-1440
"Nummernverwalter" auf Seite C-1914

#### Ziel-Nummernkreis

**Mandant**: Mandant, aus dessen AV-Bereich die Bestellnummern genommen werden sollen. Die Wahl des Mandanten steuert die Anzeige im Feld AV-Bereich.

**AV-Bereich**: Standard-AV-Bereich, der in den Stammdaten des Produkts hinterlegt ist. Sie können einen anderen AV-Bereich auswählen. Wenn die Auswahl der AV-Bereiche nicht eingeschränkt werden soll, müssen Sie den Eintrag <k.A.> wählen.

### Bestellübergabe – Bestellpool

> Dokumente > Auftrag > Bestellübergabe > Register Bestellpool

*Abb. C-346 Bestellübergabe - Bestellpool*

In diesem Register können Sie die Positionen prüfen und ggf. die Daten ergänzen, bevor Sie die Bestellung übergeben. Wenn Sie den Bestellpool nicht über das Register Bestellnummern gefüllt haben, können Sie Aufträge mit Bestellpositionen über die Schaltflächen nach Lieferant, Produkt und/oder Liefertermin zusammenstellen.
Die übergebenen Bestellungen können Sie sich im Dialog Bestellungen anzeigen lassen.
⇨ "Bestellung im Bestellpool ändern" auf Seite C-1568

- **Lieferant**: Im Auswahlmodus können Sie Bestellpositionen für einen bestimmten Lieferanten zusammenstellen. ⇨ "Markierungsoptionen" auf Seite C-1950
- **Produkt**: Im Auswahlmodus können Sie Bestellpositionen für ein bestimmtes Produkt zusammenstellen.
- **Liefertermin**: Im Auswahlmodus können Sie Bestellpositionen für einen bestimmten Liefertermin zusammenstellen.
- **Auftrag**: Im Auswahlmodus können Sie Bestellpositionen für eine Abfolge von Auftragsnummern zusammenstellen.

#### Bestellpool

Mit den Schaltflächen können Sie alle Positionen automatisch markieren, die an einen bestimmten Lieferanten gesendet werden sollen, oder alle Markierungen entfernen.
Über das Menü Funktionen können Sie Filter einstellen, anhand derer die Positionen automatisch markiert werden.
⇨ "Markierungsoptionen" auf Seite C-1950

> **Positionen markieren**
> Nur die markierten Positionen werden übergeben. Bei langen Listen können Sie die Positionen insgesamt aus- oder abwählen, indem Sie auf die entsprechenden Schaltflächen klicken.

**Übergabe an**: Bestellungen können wahlweise direkt an die Lieferanten übergeben oder als Bestellanfrage gesendet werden.
- **Bestellung**: Mit dieser Option werden Bestellungen erzeugt. Bestellungen an denselben Lieferanten können zu Sammelbestellungen zusammengefasst werden. Dazu muss die Option Auftragsbezogene Übergabe deaktiviert sein und die Bestellpositionen müssen in der richtigen Reihenfolge aufgeführt sein.
- **Bestellanfrage**: Mit dieser Option werden Bestellanfragen erzeugt, um z. B. Liefertermine oder Preise zu erfragen.

#### Übersicht

In der Übersicht werden die Daten zu den Bestellpositionen angezeigt. Diese können bearbeitet werden. Zur Wahl eines alternativen Lieferanten können Sie sich einen Preisvergleich anzeigen lassen.

- **Auftrag, Pos.**: Nummer des Auftrags und der Position, zu der die Bestellung erzeugt werden soll.
- **Int. Kunde**: Name des internen Kunden. Die Spalte wird nur angezeigt, wenn im Bestellpool Dokumente für interne Aufträge vorhanden sind. ⇨ Tutorial, "Interne Aufträge" auf Seite C-1562
- **Lieferant**: Der Lieferant wird aus der Lieferantenkartei oder dem Auftrag übernommen. Wenn kein Lieferant eingetragen ist oder wenn Ihnen Lieferschwierigkeiten Ihres Standard-Lieferanten bekannt sind, können Sie den Namen ändern. ⇨ "Lieferant und Liefertermin ändern" auf Seite C-1949
- **Artikel, Farbe**: Nummer und ggf. Variante des Produkts, das bestellt werden soll.
- **Menge**: Menge, die bestellt werden soll.
- **Breite, Höhe**: Maße der Scheibe, die bestellt werden soll.
- **Anlief.-Term. bei Kunde**: Der Liefertermin wird aus dem Auftrag übernommen. Lieferschwierigkeiten werden farblich gekennzeichnet und Sie können den Termin dann ändern.
- **Anlief.-Term. d. Lieferant**: Der Liefertermin des Lieferanten wird aus den Angaben in der Lieferantenkartei errechnet. Lieferschwierigkeiten werden farblich gekennzeichnet und Sie können den Termin dann ändern.
- **Übergeben an**: Die Bestell- oder Anfragenummern werden nach der Übergabe angezeigt.
- **Stkl.-Anz.**: Mit einem Klick in die entsprechende Zelle können Sie sich die Stückliste anzeigen lassen. In der Spalte sind die Zeilen mit Produkten gekennzeichnet, die komplett mit allen Stücklistenelementen bestellt werden.
- **Kritischer Lagerbestand erreicht am**: Datum, an dem die Menge erreicht wird, ab der Lagerbestand keine termingerechte Produktion mehr sicherstellen kann. Die entsprechend Lagerbestellung muss manuell angestoßen werden.

**Position für**: Die aufgelisteten Positionen sind farblich gekennzeichnet.

#### Ziel-Nummernverwalter, Nummernkreise

Diese Felder sind zum Register Bestellnummer beschrieben.
⇨ "Bestellübergabe - Bestellnummern" auf Seite C-1943

### Lieferant und Liefertermin ändern

> Dokumente > Auftrag > Bestellübergabe > Register Bestellpool > Doppelklick auf Position

*Abb. C-347 Lieferant und Liefertermin ändern*

In diesem Dialog können Sie den Lieferanten und die Liefertermine für die Bestellungen zu einem bestimmten Auftrag ändern.
Die Checkboxen werden automatisch markiert, wenn Sie im zugehörigen Feld eine Änderung eingetragen haben.

**Lieferant / Matchcode**: Nummer des aktuellen Lieferanten. Über die Lieferantennummer oder den Matchcode können Sie einen anderen Lieferanten angeben.

**Anliefertermin bei Kunde**: Aktueller Liefertermin beim Kunden. Zum Ändern können Sie das Datum überschreiben oder aus dem Kalender auswählen.

**Anliefertermin durch Lieferant**: Aktueller Liefertermin für den Lieferanten. Zum Ändern können Sie das Datum überschreiben oder aus dem Kalender auswählen. Wenn Sie den Termin über den Kalender auswählen, werden die Tourentage hervorgehoben.

**Statt internem Auftrag reguläre Bestellung erzeugen**: Sie können interne Aufträge in Bestellungen an einen Lieferanten umwandeln, ohne den Lieferanten auswählen zu müssen.
- ☐ Interne Bestellungen bleiben erhalten, sofern Sie keinen externen Lieferanten ausgewählt haben.
- ☑ Die interne Bestellung wird automatisch in eine reguläre Bestellung umgewandelt. Als Lieferant wird automatisch der Standard-Lieferant für den Artikel eingesetzt.

### Markierungsoptionen

> Dokumente > Auftrag > Bestellübergabe > Register Bestellpool > Menü Funktionen > Markierungsoptionen

*Abb. C-348 Markierungsoptionen*

In diesem Dialog stellen Sie Kriterien ein, nach denen die Bestellungen gefiltert und markiert werden, um sie dann zu bestellen. Die Felder werden freigeschaltet, wenn die zugehörige Checkbox markiert ist.

#### Markierungsoptionen

- **Auftragsnummer von, bis**: Alle Positionen werden markiert, deren Auftragsnummern im angegebenen Bereich liegen.
- **Lieferant**: Alle Positionen werden markiert, die bei einem bestimmten Lieferanten bestellt werden.
- **Liefertermin**: Alle Positionen werden markiert, die zum angegebenen Termin geliefert werden sollen.
- **Produkt**: Alle Positionen werden markiert, die das angegebene Produkt betreffen.
- **Produktionstermin**: Alle Positionen werden markiert, die zu einem bestimmten Termin produziert werden sollen.
- **Warengruppe**: Alle Positionen werden markiert, die die angegebene Warengruppe betreffen.
- **Int. Kunde**: Alle internen Bestellungen für einen internen Kunden werden markiert.

### Preisvergleich

> Dokumente > Auftrag > Bestellübergabe > Register Bestellpool > Menü Funktionen > Lieferantenpreise

*Abb. C-349 Lieferanten - Preisvergleich*

In diesem Dialog lassen Sie sich anzeigen, welche Lieferanten die Produkte zu welchen Preisen und Terminen liefern können.
Die Checkbox des Standard-Lieferanten ist automatisch markiert.
Wenn Sie einen anderen Lieferanten auswählen, werden die entsprechenden Angaben im Dialog Bestellübergabe im Register Bestellpool aktualisiert.
⇨ "Bestellübergabe - Bestellpool" auf Seite C-1946

> **Die Zeile muss mit einem X markiert sein**
> Sie können den Preisvergleich nur starten, wenn Sie im Register Bestellpool die entsprechende Zeile markiert haben und ein X im Zeilenkopf angezeigt ist. Die einfache Markierung einer Zeile reicht nicht aus.

#### Lieferanten - Positionspreise

In der Übersicht werden die ausgewählten Aufträge angezeigt. Die aufgelisteten Positionen sind farblich gekennzeichnet:
- **Default-Lieferant**: In roter Schrift ist der Standard-Lieferant dargestellt.
- **!!! -> rechtzeit. Liefertermin gefaehrdet**: Mit drei Ausrufungszeichen sind die Einträge dargestellt, bei denen der Liefertermin gefährdet ist.
- **preisguenstigster Lieferant**: In grüner Schrift sind die Einträge des preisgünstigsten Lieferanten dargestellt.
- **Default- und preisguenstigster Lieferant**: In blauer Schrift sind die Einträge des Standard-Lieferanten dargestellt, die gleichzeitig die preisgünstigsten sind.

### Erweiterte Einstellungen

> Dokumente > Auftrag > Bestellübergabe > Menü Optionen > Gruppe Erweitert > Einstellungen

In diesem Dialog legen Sie Einstellungen für die Bestellübergabe fest.
In diesem Dialog finden Sie folgende Register:
- "Erweiterte Einstellungen – Allgemein" auf Seite C-1954
- "Erweiterte Einstellungen – Sortierung" auf Seite C-1955

#### Erweiterte Einstellungen – Allgemein

> Dokumente > Auftrag > Bestellübergabe > Menü Optionen > Gruppe Erweitert > Einstellungen > Register Allgemein

*Abb. C-350 Erweiterte Einstellungen – Allgemein*

In diesem Register können Sie bestimmen, welche Texte nicht in die Bestellung übernommen werden sollen.

##### Textfilter

**1.-6.**: Textkennzeichen der Texte, die nicht in die Bestellung übernommen werden sollen, z. B. L für Lieferscheintexte.
⇨ Stammdaten, "Textkennzeichen" auf Seite B-1188

##### Kommissionstext ersetzen

**Die Kommission nicht aus dem Auftrag übernehmen**: Sie können festlegen, ob die Kommissionstexte in die Bestellung übernommen werden sollen.
- ☐ Kommissionstexte aus dem Auftragskopf werden in die Bestellung übernommen.
- ☑ Kommissionstexte aus dem Auftragskopf werden nicht in die Bestellung übernommen. Das Feld für die Formel ist freigeschaltet, um einen anderen Text einzutragen.

##### Text für interne Bestellung

**Nr.**: Für interne Bestellungen können Sie eigene Texte hinterlegen. Mit der Textnummer bestimmen Sie, welcher Text übergeben werden soll.
⇨ Tutorial, "Text erfassen" auf Seite C-1308

##### SZR Bestellung

Wenn ein SZR aus einer Auftragsposition bestellt wird, wird die gewählte Produktgruppe mitbestellt, z. B. Sprossen.

##### In die Bestellung übertragbare Dateianhänge

In der Übersicht werden alle Typen von Dateianhängen aufgelistet. Nur die Dateianhänge werden mit der Bestellung übertragen, die zum markierten Typ gehören.

#### Erweiterte Einstellungen – Sortierung

> Dokumente > Auftrag > Bestellübergabe > Menü Optionen > Gruppe Erweitert > Einstellungen > Register Sortierung

*Abb. C-351 Erweiterte Einstellungen – Sortierung*

In diesem Register legen Sie fest, wie die Angaben im Bestellpool sortiert sein sollen.

##### Sortierung nach

Mit der Wahl der Option legen Sie die Sortierung auf dem Bestellschein fest:
- **Nach Auftrag - Lieferant - Position**: Die Positionen werden pro Auftrag nach Lieferanten aufgelistet.
- **Nach Auftrag - Position - Lieferant**: Die Lieferanten werden pro Auftrag nach Positionen aufgelistet.
- **Bestelloptimiert nach Lieferant**: Die Bestellungen werden nach AB-Nummer und Lieferanten sortiert.
- **Benutzerdefiniert**: Die Felder Verfügbare Sortierkriterien und Ausgewählte Kriterien und Reihenfolge werden freigeschaltet, so dass Sie die Kriterien auswählen und sortieren können.

##### NV-Sortierung beibehalten

Die Sortierung kann aus dem jeweiligen Nummernverwalter übernommen werden.
- ☐ Die Sortierung des Nummernverwalters wird nicht berücksichtigt.
- ☑ Die Sortierung richtet sich nach den Einstellungen im Nummernverwalter.

##### Verfügbare Sortierkriterien

In diesem Feld werden die möglichen Sortierkriterien aufgelistet. Das Feld ist nur freigeschaltet, wenn die Option Benutzerdefiniert gewählt wurde.

##### Ausgewählte Sortierkriterien und Reihenfolge

Aus dem Feld Verfügbare Sortierkriterien werden ausgewählte Sortierkriterien in dieses Feld verschoben. Zusätzlich kann die Reihenfolge bearbeitet werden. Das Feld ist nur freigeschaltet, wenn die Option Benutzerdefiniert gewählt wurde.

### Stücklistenübersicht

> Dokumente > Auftrag > Bestellübergabe > Register Bestellpool > Klick auf Spalte Stkl.Anz.

*Abb. C-352 Stücklistenübersicht*

In diesem Dialog lassen Sie sich die Stückliste der Bestellposition anzeigen.

## Auftrag

Über das Menü **Auftrag** erreichen Sie sich folgende Programmpunkte:

- **NV Auftrag**: Die Funktion des Nummernverwalters ist für alle Dokumente gleich. Sie wird am Beispiel Auftrag beschrieben. ⇨ "Nummernverwalter" auf Seite C-1914
- **Auftrag**: Die Erfassung von Dokumenten ist für alle Dokumentenarten gleich. Sie wird am Beispiel Auftrag beschrieben. ⇨ "Dokument - Kopfdaten" auf Seite C-1687
- **Teillieferung**: Öffnet den Dialog Teillieferung, in dem der Auftragsstatus der Dokumente angezeigt wird. ⇨ "Teillieferungen" auf Seite C-1901
- **Druck Auftrag**: Der Formular- und Etikettendruck ist für alle Dokumente gleich. Er wird am Beispiel Auftrag beschrieben. "Druck" auf Seite C-1923
- **FiBu-Übergabe**: Die FiBu-Übergabe ist für Aufträge und Gutschriften gleich. Sie wird am Beispiel Auftrag beschrieben. ⇨ "FiBu-Übergabe” auf Seite C-1967
- **Import/Export von Zahlungen**: Dieser Dialog steht nur für den brasilianischen Zahlungsverkehr zur Verfügung. ⇨ "Import/Export von Zahlungen" auf Seite C-1973
- **Journal**: Der Journaldruck ist für alle Dokumente gleich. Er wird am Beispiel Auftrag beschrieben. ⇨ "Journal" auf Seite C-2018
- **Anzahlungen Aufträge**: Der Anzahlungsdruck ist für Aufträge und Gutschriften gleich. Er wird am Beispiel Auftrag beschrieben. ⇨ "Anzahlungen" auf Seite C-1961
- **Bestellübergabe**: Wenn in den Auftragspositionen Bestellungen enthalten sind, können diese direkt bestellt oder in einen Bestellpool übergeben werden. ⇨ "Übergabe Bestellungen" auf Seite C-1940
- **Übergabe Archiv**: Die Archivübergabe ist für alle Dokumente gleich. Sie wird am Beispiel Auftrag beschrieben. ⇨ "Übergabe Archiv" auf Seite C-1974
- **Suche**: Der Suchdialog ist für alle Dokumente gleich. Er wird am Beispiel Auftrag beschrieben. ⇨ "Dokument suchen" auf Seite C-1803
- **Import**: Mit dieser Funktion werden elektronische Kunden-Aufträge importiert. ⇨ "Import" auf Seite C-1976
- **Bankbelege**: Die Bankbelege sind für Aufträge und Gutschriften gleich. Sie werden am Beispiel Auftrag beschrieben. ⇨ "Bankbelege" auf Seite C-1962
- **Überrechnen**: Öffnet den Dialog Neuberechnung von Dokumenten, um Preisänderungen in den Stammdaten in das ausgewählte Dokument zu übernehmen. ⇨ "Überrechnen" auf Seite C-1964
- **Objektabrechnung**: Die folgenden Einträge sind abhängig von dem Modus der Objektverwaltung, der in den Firmendaten eingestellt ist.
    - **Nummernverwalter**: Öffnet den Nummernverwalter für die Objekt-/Abrechnungsverwaltung. "Nummernverwalter" auf Seite C-1917
    - **Abrechnung**: Öffnet den Dialog Objekte, um objektbezogene Abrechnungen zu erstellen. ⇨ "Abrechnung" auf Seite C-1981
    - **Formulare**: Öffnet den Formular-/Etikettendruck für die Objekt-/Abrechnungsverwaltung. "Formular-/Etikettendruck" auf Seite C-1926
    - **Stunden**: Öffnet den Dialog Einkauf, um eine Stundenforderung zu erfassen. ⇨ "Stundenforderung" auf Seite C-1993
    - **Einkauf**: Öffnet den Dialog Einkauf, um eine Einkaufsforderung zu erfassen. ⇨ "Einkaufsforderung" auf Seite C-1994
- **TPS Faktura**: Öffnet den Dialog TPS Faktura. Dieser Eintrag ist nur kundenspezifisch freigeschaltet.
- **Schnellanfrage**: Öffnet den Dialog Schnellanfrage, um eine (telefonische) Kundenanfrage aufzunehmen, ohne den aktuellen Auftrag zu schließen. ⇨ "Schnellanfrage" auf Seite C-1871
- **Garantiebelege**: Dieser Dialog ist nur kundenspezifisch freigeschaltet.
- **SAFT-PT-Export**: Öffnet den Dialog SAFT-PT Export. Dieser Eintrag ist für den portugiesischen Markt freigeschaltet. ⇨ “SAFT-PT Export" auf Seite C-1966
- **Auswertungen**:
    - **Preisänderung**: Öffnet den Dialog Preisänderungsreport, um alle Aufträge anzuzeigen, die von Preisänderungen betroffen sind. ⇨ "Preisänderung (Report)" auf Seite C-1998
    - **Null-Preisreport**: Öffnet den Dialog Null-Preisreport, um alle Auftragspositionen ohne Preis anzuzeigen. ⇨ "Null-Preisreport" auf Seite C-2000
    - **Deckungsbeitrags-Analyse**: Öffnet den Dialog Deckungsbeitrags-Analyse, um die Deckungsbeiträge von Aufträgen anzuzeigen. ⇨ "Deckungsbeitrags-Analyse" auf Seite C-2002
    - **Kalkulatorische Frachtkosten**: Öffnet den Dialog Kalkulatorische Frachtkosten, um Fracht- und Speditionskosten zu erfassen. "Kalkulatorische Frachtkosten" auf Seite C-2006
- **Interne Kontrolle**
    - **Gutschriftgründe**: Öffnet den Dialog Gutschriftgründe, um eine Auswertung zu Gutschriftgründen zu erstellen. ⇨ "Gutschriftgründe" auf Seite C-2011
    - **Verspätete Lieferung/Lieferung ohne Berechnung**: Öffnet einen Dialog, um eine Auswertung zu verspäteten Lieferungen oder Lieferungen ohne Preise zu erstellen. ⇨ "Verspätete Lieferung/Lieferung ohne Berechnung" auf Seite C-2014

### Anzahlungen

> Dokument > Auftrag > Anzahlungen Aufträge

*Abb. C-353 Anzahlungsdruck*

In diesem Dialog lassen Sie sich Listen der erfassten Anzahlungsrechnungen erstellen. Der Dialog ist für Aufträge und Gutschriften gleich.
⇨ Tutorial, "Anzahlungen" auf Seite C-1535

#### Auswahl

**Nummernverwalter**: Auswahl des Nummernverwalters, in dem die Anzahlungen gesammelt wurden.

**Seitenumbruch beim Wechsel von**
Für den Druck kann ein Seitenumbruch festgelegt werden:
- Das Anzahlungsdatum ist ausschlaggebend.
- Die Zahlungsart ist ausschlaggebend.
- ☐ Der Seitenumbruch wird nicht beim Anzahlungsdatum / bei der Zahlungsart eingefügt.
- ☑ Der Seitenumbruch wird eingefügt.

**Anzahlungsdatum**: Bei Druck kann

#### Dokumente

In der Übersicht werden alle Dokumente aus dem gewählten Nummernverwalter angezeigt. Die Liste wird über die Druckfunktion erstellt.

### Bankbelege

> Dokumente > Auftrag, Gutschrift > Bankbelege

*Abb. C-354 Bankbelege - Wechseldruck*

In diesem Dialog können Sie Überweisungsträger für Ihre Kunden drucken.

#### Menü Optionen

- **LGF Modus aktiv**: Diese Funktion ist nur kundenspezifisch freigeschaltet.

#### Menü Funktionen

- **Historie**: Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des Dokuments.
    - ⇨ "Historie" auf Seite C-1834

#### Identifikation

**Mandant**: Mandant, für den die Überweisung verbucht werden muss.
⇨ Stammdaten, "Firmendaten - Mandant" auf Seite B-1056

**Bereich**: Wenn Sie mit AV-Bereichen als eigene Profit-Center arbeiten, können den AV-Bereich auswählen, zu dem die Überweisung gehört.

**Mitarbeiter**: Name des Mitarbeiters, der sich in A+W Business angemeldet hat.

**Nummernverwalter**: Auswahl des Nummernverwalters, in dem die Rechnungen gesammelt sind.

**Einzeldruck**: Die Überweisungen können gesammelt gedruckt werden.
- ☐ Die Überweisungen werden gemeinsam auf einen Datenträger gedruckt. Diese Einstellung ist nur sinnvoll, wenn alle Rechnungen für denselben Kunden gelten.
- ☑ Die Überweisungen werden einzeln auf jeweils einen eigenen Datenträger gedruckt.

#### Modifikation

In diesem Bereich werden Details des Dokuments angezeigt.

**Rechnung**: Rechnungsnummer des markieren Dokuments.

**Rechnungsdatum, Nettobetrag**: Rechnungsdatum und Nettobetrag des markieren Dokuments.

**KZ Fälligkeitsberechnung**: Kennzeichen für die Fälligkeit aus dem Auftrag.
⇨ Tutorial, "Fälligkeitsberechnung" auf Seite C-1469

**Zahltage**: Die Zahltage werden im Auftrag angegeben.

**Valuta-Datum**: Das Datum der Wertstellung wird aus den Angaben zur Fälligkeit errechnet.

**Bruttotage**: Die Bruttotage werden aus den Angaben zur Fälligkeit und den Zahltagen errechnet.

**Betrag Fakturieren**: Anzeige Netto-Rechnungsbetrag. Er kann geändert werden. Die Änderungen gelten nur für das markierte Dokument. Mit der Pfeil-Schaltfläche kann die Änderung zurückgesetzt werden.

#### Übersicht

Aus dem gewählten Nummernverwalter werden nur die Dokumente mit einer Rechnungsnummer angezeigt.
Im Zeilenkopf wird ein rotes X angezeigt, wenn der Sperrstatus des Dokumentes überschritten ist.

### Überrechnen

> Dokumente > Auftrag > Überrechnen

*Abb. C-355 Überrechnen – Neuberechnung von Dokumenten*

In diesem Dialog können Sie die Auftragssummen neu berechnen lassen, z. B. Mehrwertsteuer, Zuschläge, Flächen. Die Kosten der Fußzuschläge werden nur überrechnet, wenn die Überrechnung im Modus EK gestartet wird.

#### Dokumente

Mit der Wahl der Option geben Sie an, welche Dokumente aufgelistet werden sollen. Gleichzeitig wird die Wahl eines Nummernverwalters in der gleichnamigen Kombobox entsprechend eingeschränkt.

#### Optionen

Die Checkboxen in diesem Bereich sind in Abhängigkeit des Modus zur Neuberechnung freigeschaltet bzw. gesperrt.

**Preis auf Null setzen**: Die Checkbox ist nur freigeschaltet, wenn der Modus Komplette Berechnung markiert ist.
- ☐ Die Preise in den Dokumenten werden nicht auf null gesetzt.
- ☑ Die Preise werden auf null gesetzt.
- **Mwst %-Satz neu einlesen**: Der Mwst-Steuersatz kann nach einer Änderung für alle Dokumente neu eingelesen werden. Die Checkbox ist nur freigeschaltet, wenn der Modus Komplette Berechnung oder Mwstberechnung markiert ist.
    - ☐ Der Mwst-Satz wird nicht neu eingelesen.
    - ☑ Der Mwst-Satz wird neu eingelesen. Anschließend wird die Mehrwert-Steuer neu berechnet.
- **Manuelle Preisvorgaben löschen**: Die Checkbox ist nur freigeschaltet, wenn der Modus Komplette Berechnung markiert ist.
    - ☐ Die manuellen Preise werden nicht gelöscht.
    - ☑ Die manuellen Preise werden gelöscht. Zur Neuberechnung werden die Preise aus den Stammdaten herangezogen.
- **Warengruppen neu einlesen**: Die Checkbox ist nur freigeschaltet, wenn der Modus Komplette Berechnung oder Kombi-WGR bilden markiert ist.
    - ☐ Die Warengruppen werden nicht neu eingelesen.
    - ☑ Die Warengruppen werden neu eingelesen.
- **Autom. Zuschl.-Kennz. aus Produkten einlesen**: Aus den Stammdaten der Produkte können automatische Zuschläge übergeben werden.
    - ☐ Die Kennzeichen für automatische Zuschläge aus den Stammdaten der Produkte werden nicht berücksichtigt.
    - ☑ Die Kennzeichen für automatische Zuschläge aus den Stammdaten der Produkte werden neu eingelesen.
- **Fixierte Sonderrabatte/-zuschläge überrechnen**: Die Checkbox ist nur freigeschaltet, wenn entweder der Modus Komplette Berechnung oder der Modus Sonderrabatte/-zuschläge berech. markiert ist. Sie steuert, ob die fixierten Sonderrabatte bzw. -zuschläge überrechnet werden oder nicht.
    - ☐ Die fixierten Zuschläge werden nicht angepasst.
    - ☑ Die fixierten Zuschläge werden zwangsweise überrechnet.
    - Stammdaten: Tutorial 1, "Automatische Zuschläge fixieren" auf Seite B-402

#### Modus

Mit der Wahl der Option geben Sie an, welche Daten neu berechnet bzw. neu eingelesen werden sollen. Im Bereich Optionen werden die zugehörigen Checkboxen freigeschaltet.

#### Selektion nach

- **Nummernverwalter**: Die Dokumente des gewählten Nummernverwalters sollen neu berechnet werden. Das Feld Nummernverwalter wird freigeschaltet.
- **SQL-Befehl**: Zur Auswahl der Dokumente wird ein SQL-Befehl eingegeben. Das Eingabefeld wird freigeschaltet.

**Mitarbeiter**: Name des Mitarbeiters, der sich in A+W Business angemeldet hat.
**Nummernverwalter**: Sie können den Nummernverwalter auswählen, in dem sich die zu überrechnenden Dokumente befinden. Die Auswahl wird durch die Wahl der Option im Bereich Dokumente eingeschränkt. Das Feld ist gesperrt, wenn im Bereich Selektion nach die Option SQL-Befehl markiert ist.

**Eingabefeld, [Ausführen]**: Das Eingabefeld für den SQL-Befehl ist nur freigeschaltet, wenn im Bereich Selektion nach die Option SQL-Befehl markiert ist.

#### Dokumente

In der Übersicht werden alle Dokumente aufgelistet, für die die Neuberechnung durchgeführt werden soll.

### TPS Faktura

> Dokumente > Auftrag > TPS Faktura

Dieser Dialog ist nur kundenspezifisch freigeschaltet.

### Garantiebelege

> Dokumente > Auftrag > Garantiebelege

Dieser Dialog wird nur kundenspezifisch genutzt.

### SAFT-PT Export

> Dokumente > Auftrag > SAFT-PT Export

*Abb. C-356 SAFT-PT Export*

In diesem Dialog legen Sie den Zeitraum fest, aus dem zertifizierte Rechnungen und Gutschriften für den portugiesischen Markt in eine XML-Datei exportiert werden sollen.

## Übergabe, Im-/Export von Dokumenten

Die Übergabe, der Import, der Export und die zugehörigen Menüs sind für Aufträge, Gutschriften und Bestellungen gleich. Die Dialoge werden in dieser Anleitung am Beispiel Auftrag beschrieben.

Zum diesem Thema finden Sie Informationen zu folgenden Themen:
- "FiBu-Übergabe" auf Seite C-1967
- "Sollstellung FiBu" auf Seite C-1970
- "Einstellungen FiBu-Übergabe" auf Seite C-1972
- "Import/Export von Zahlungen" auf Seite C-1973
- "Übergabe Archiv” auf Seite C-1974
- "Import" auf Seite C-1976
- "Fremddokumentenverwaltung" auf Seite C-1980

### FiBu-Übergabe

> Dokumente > Auftrag, Gutschrift, Bestellung > FiBu-Übergabe

Sie können Rechnungen, Gutschriften und Bestellungen an ein externes Programm zur Finanzbuchhaltung (FiBu) übergeben.

Zum Thema FiBu-Übergabe finden Sie folgende Informationen:
- "Menü Funktionen" auf Seite C-1968
- "Menü Optionen" auf Seite C-1968
- "Sollstellung FiBu" auf Seite C-1970
- "Einstellungen FiBu-Übergabe" auf Seite C-1972
- "Import/Export von Zahlungen" auf Seite C-1973

#### Menü Funktionen

> Dokumente > Auftrag, Gutschrift, Bestellung > FiBu-Übergabe > Menü Funktionen

Über dieses Menü können Sie andere Dialoge öffnen, ohne die FiBu-Übergabe zu schließen. Folgende Einträge werden angezeigt:
- **Historie**: Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des Dokuments.
    - ⇨ "Historie" auf Seite C-1834
- **Produkt Export**: Dieser Eintrag ist nur in Verbindung mit FiBu-Programm Prodaja freigeschaltet. Die Produktstammdaten werden in eine ASCII-Datei exportiert.
- **Einstellungen**: Öffnet den Dialog Einstellungen FiBu-Übergabe, um zu den Dokumenten im Nummernverwalter Details für die Übergabe festzulegen.
    - ⇨ "Einstellungen FiBu-Übergabe" auf Seite C-1972

#### Menü Optionen

> Dokumente > Auftrag, Gutschrift, Bestellung > FiBu-Übergabe > Menü Optionen

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

> **Aktivierte Optionen nach dem Öffnen des Dialogs**
> Bitte beachten Sie, dass geänderte Optionen erst beim nächsten Öffnen des Dialogs wirksam werden. Wenn durch eine aktivierte Option eine Prüfung gestartet wurde, kann sich das Öffnen eines Dokuments verzögern. Der Grad der Verzögerung hängt von der Leistungsfähigkeit des Rechners ab. Die folgenden Beschreibungen stellen die aktivierte Option dar.

Das Menü ist in folgende Gruppen gegliedert:
- "Gruppe Kosten" auf Seite C-1968
- "Gruppe Kunden" auf Seite C-1969
- "Gruppe Sonstige" auf Seite C-1969

##### Gruppe Kosten

- **Übergabe Kostenrechnung**: Anzeige, ob die Kostenrechnung in den Firmendaten aktiviert wurde. Die Funktion kann über diesen Eintrag nicht aktiviert oder deaktiviert werden.
    - ⇨ Stammdaten, "Kostenrechnung aktiv" auf Seite B-1063
- **Nur Rechnungen mit Wert > 0**: Nur die Rechnungen sollen an die FiBu übergeben werden, deren Rechnungssummer größer als Null ist.
- **Nur Buchungen mit Wert > 0**: Erlöskonten mit dem Betrag 0 sollen nicht an die FiBu übergeben werden.
- **Steuerkennzeichen separat verarbeiten**: Zur Ermittlung des korrekten Erlöskontos werden die Positionen und Stücklisten-Komponenten gemäß dem Steuerkennzeichen auf die Warengruppen gruppiert.
- **FiBu in Altwährung**: Die Funktion wird nur benötigt, wenn ein Kunde der gemeinsamen Währung Euro beitritt.
- **Fremdschlüssel als Währungskennzeichen übergeben**: Wenn Sie mit mehreren Währungen arbeiten und in den Stammdaten den Währungen den Fremdschlüssel Ihrer FiBu zugeordnet haben, können Sie diesen Fremdschlüssel an die FiBu übergeben. Die Währung wird dann anhand des Fremdschlüssels identifiziert.
    - ⇨ Stammdaten, "Währung" auf Seite B-1045

##### Gruppe Kunden

- **Kundenübergabe deaktiviert**: Der Kundenname wird nicht übergeben.
- **Kundenkonto anstatt Kundennummer übergeben**: Wenn in den Kundendaten ein Debitorenkonto hinterlegt ist, wird dieses anstelle der Kundennummer übergeben.
    - ⇨ Stammdaten, "Partnerverwaltung - Finanzen" auf Seite B-904

##### Gruppe Sonstige

- **Automatische Sortierung aktiv (Kunde/Rechnung/Auftrag)**: Die Daten werden zur Übergabe pro Kunde, Rechnung und/oder Auftrag automatisch sortiert. Wenn die Sortierung nicht aktiviert ist, wird die Sortierung aus dem Nummernverwalter übernommen.
- **Ausgabedatei überschreiben**: Diese Funktion wird nur benötigt, wenn die FiBu nicht mit Nummernkreisen sondern mit festen Dateinamen arbeitet. Die Ausgabedatei aus der vorigen Übertragung wird überschrieben. Wenn die Funktion ausgeschaltet ist, werden in der Ausgabedatei die neuen Daten hinzugefügt. Die Datei wird dabei immer größer.
- **OEM Konvertierung aktiv**: Für die FiBu-Übergabe kann die Konvertierung von Sonderzeichen aktiviert werden, z. B. ä in ae. Die OEM Konvertierung kann in den Firmendaten gesperrt werden.
    - ⇨ Stammdaten, "OEM/ANSI Konvertierung deaktivieren" auf Seite B-1102

### Sollstellung FiBu

> Dokumente > Auftrag, Gutschrift, Bestellung > FiBu-Übergabe

*Abb. C-357 FiBu-Übergabe – Sollstellung FiBu*

In diesem Dialog geben Sie an, welche Rechnungen/Gutschriften an die FiBu (Finanzbuchhaltung) übergeben werden sollen. Der Dialog ist für alle FiBu-Programme gleich aufgebaut. In der Titelzeile wird jeweils der Name der FiBu angezeigt.
⇨ Tutorial, "Finanzbuchhaltung (FiBu)" auf Seite C-1616

#### Identifikation

**Mandant**: Mandant, für den die Rechnungen übergeben werden.
**Bereich**: AV-Bereich, zu dem die Dokumente gehören.
**Mitarbeiter**: Mitarbeiter, der sich in A+W Business angemeldet hat.
**Nummernverwalter**: Nummernverwalter, in dem sich die zu übergebenden Rechnungen bzw. Gutschriften befinden.
Vor der FiBu-Übergabe prüft das Programm, ob mindestens ein Dokument im Nummernverwalter eine Rechnungsnummer enthält und den notwendigen Status für die Übergabe hat. Nur dann wird eine Laufnummer vergeben.

**Kontrollsumme**: Wenn die Dokumente an die FiBu übergeben wurden, wird als Kontrollsumme die Gesamtsumme der übergebenen Beträge angezeigt.
**Lauf**: Wenn die Dokumente an die FiBu übergeben wurden, wird die Nummer des Übergabelaufs angezeigt. Diese wird in aufsteigender Folge automatisch aus dem Nummernkreis genommen, der für den Mandanten und/oder AV-Bereich definiert ist.
⇨ Stammdaten, "Nummernkreise - FiBu" auf Seite B-1032

#### Ausgabe

**Debitor/Kreditor**: Pfad und Datei, in die die Daten geschrieben werden. Die Angaben werden aus den Firmendaten übernommen.
⇨ Stammdaten, "Pfad und Dateiname" auf Seite B-1062

**Rechnung/Gutschrift**: Pfad und Datei, in die die Daten geschrieben werden. Die Angaben werden aus den Firmendaten übernommen.

**Buchungsdatum**: Als Buchungsdatum wird das Systemdatum angezeigt. Es kann überschrieben werden.

**Periode**: Angabe der Buchungsperiode, zu der die Rechnungen und Gutschriften gehören.
⇨ Stammdaten, "Buchungsperioden" auf Seite B-1170

**Aktueller Auftrag**: Nummer des Auftrags, der aktuell an die FiBu übergeben wird.

**Position**: Nummer der Auftragsposition, die aktuell an die FiBu übergeben wird.

**Gesamt - Aufträge**: Anzahl der Dokumente, die an die FiBu übergeben wurden.

**Positionen**: Anzahl der Positionen, die an die FiBu übergeben wurden.

#### Übersicht

In der Übersicht werden alle Dokumente angezeigt, die sich im aktuellen Nummernverwalter befinden. Nur wenn Sie Rechnungen und Gutschriften über denselben Nummernverwalter übergeben, werden beide Dokumentenarten aufgelistet.

**Ergänzende Informationen**
⇨ Stammdaten, "Finanzen und Saldo" auf Seite B-141
⇨ Stammdaten, "Firmendaten - FiBu" auf Seite B-1061
⇨ Tutorial, "Finanzbuchhaltung (FiBu)" auf Seite C-1616

### Einstellungen FiBu-Übergabe

> Dokumente > Auftrag, Gutschrift, Bestellung > FiBu-Übergabe > Menü Funktionen > Einstellungen

*Abb. C-358 Einstellungen FiBu-Übergabe*

In diesem Dialog können Sie Details für die FiBu-Übergabe festlegen.

**Klassifikator 1, 2**: Zur Auswahl werden alle Klassifikatoren angeboten, die übergreifend für alle Marktpartner gelten. Wenn in den Stammdaten Klassifikatoren mit zusätzlichen Kundeninformationen hinterlegt sind, können diese an die FiBu übergeben werden, z. B. kundenindividuelles Forderungskonto, Kundentyp.
⇨ Stammdaten, "Klassifikator anlegen" auf Seite B-135
⇨ Stammdaten, "Klassifikatoren" auf Seite B-881

**Defaultkonto Erlöse, Skonto, Rundungsdifferenzen**: Diese Felder werden nur für die FiBu Golden Soft ausgewertet. Sie lesen den Wert des Feldes Cuenta aus.

**Steuerkennzeichen alt, neu**: Diese Angabe wird nur benötigt, wenn Dokumenten nach einer Änderung des Steuersatzes an die FiBu übergeben werden.

**Geschäftsart für Anzahlungen**: Die Geschäftsart aus dem Auftrag kann überschrieben werden.

### Import/Export von Zahlungen

> Dokumente > Auftrag > Import/Export von Zahlungen

*Abb. C-359 Import/Export von Zahlungen*

In diesem Dialog wickeln Sie den brasilianischen Zahlungsverkehr über die Bank ab. Mit dem Export werden die Rechnungen (Zahlungsinformationen) an die Bank übertragen. Mit dem Import werden Rückmeldungen über geleistete Zahlungen importiert.

Für den Import/Export von Zahlungsinformationen müssen folgende Voraussetzungen erfüllt sein:
- Für den Zahlungsverkehr müssen pro Bank eigene Customizing-Formeln für den Import und den Export angelegt sein.
- Jeder Bank müssen diese Formeln zugeordnet sein: Stammdaten > Finanzen > Banken.
- Pro Währung muss das internationale Währungskennzeichen als Fremdschlüssel eingetragen sein: Stammdaten > Finanzen > Währungen.
- In den Firmendaten müssen folgende Einstellungen aktiviert sein:
    - Register Parameter: Brasilianische Steuer und Import/Export von Zahlungen
    - Register NFE: Steuernummer der Firma (Feld CNPU).

### Übergabe Archiv

> Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Übergabe Archiv

*Abb. C-360 Übergabe Archiv – Verkauf*

In diesem Dialog können Sie Dokumente manuell an das Archiv übergeben.

#### Identifikation

**Mandant**: Mandant, dessen Dokumente archiviert werden sollen.
**Mitarbeiter**: Mitarbeiter, der sich in A+W Business angemeldet hat.
**Nummernverwalter**: Nummernverwalter, in dem sich die zu archivierenden Dokumente befinden.

#### Dokumente

In den Feldern wird die Anzahl der Datensätze angezeigt, die übergeben wurden.

**Provisionsstatistik**: Dokumente können gesondert an die Provisionsstatistik übergeben werden.
- ☐ Die Dokumente werden nicht an die Provisionsstatistik übergeben.
- ☑ Die Dokumente werden an die Provisionsstatistik übergeben.
- **Umsatzstatistik**: Standardmäßig werden die Dokumente an die Umsatzstatistik übergeben.
    - ☐ Die Dokumente werden nicht an die Umsatzstatistik übergeben.
    - ☑ Die Dokumente werden an die Umsatzstatistik übergeben.
- **Archiv**: Standardmäßig werden die Dokumente an das aktuelle Archiv übergeben. Mit der Übergabe sollten die Dokumente aus der Hauptdatenbank gelöscht werden.
    - ☐ Die Dokumente werden nicht an das Archiv übergeben.
    - ☑ Die Dokumente werden an das Archiv übergeben.
- **Löschen**: Nach der Übergabe an das Archiv sollten die Dokumente aus der Hauptdatenbank gelöscht werden.
    - ☐ Die Dokumente werden nicht aus der Hauptdatenbank gelöscht.
    - ☑ Die Dokumente werden aus der Hauptdatenbank gelöscht.
    - ⇨Stammdaten, "Firmendaten - Archiv" auf Seite B-1104

#### Vorgaben

**Statistikjahr**: Sie können angeben, an welches Statistikjahr die Dokumente übergeben werden sollen. Wenn nichts eintragen ist, wird das Datum des Dokuments herangezogen.

**Statistikmonat**: Sie können angeben, an welchen Statistikmonat die Dokumente übergeben werden sollen. Wenn nichts eintragen ist, wird das Datum des Dokuments herangezogen.

**Leere Vertreterprovisionierung übergeben**: In der Regel werden nur Dokumente zur Provisionsberechnung übergeben, in denen eine Provision > 0 enthalten ist.
- ☐ Alle Dokumente werden an die Provisionierung übergeben.
- ☑ Die Dokumente werden auch dann an die Provisionierung übergeben, wenn keine Provision enthalten ist.

**Negative Verbuchung**: Wenn ein Dokument z. B. an den falschen Statistikmonat übergeben wurde, kann man dies rückgängig gemacht werden.
- ☐ Alle ausgewählten Dokumente werden an die Statistik und das Archiv übergeben, die in den Feldern eingetragen sind.
- ☑ Die Dokumente werden aus der falschen Statistik oder dem falschen Archiv zurückgeholt. Sie müssen dann an die richtige Statistik oder das richtige Archiv übergeben werden.

#### Dokumente

In der Übersicht sind alle Dokumente aufgelistet, die sich im gewählten Nummernverwalter befinden.

### Import

> Dokumente > Auftrag > Import

Der Dialog **Import** ist für Auftrag, Angebot und Gutschrift gleich. Er wird in dieser Anleitung am Beispiel Auftrag beschrieben.

*Abb. C-361 Import*

In diesem Dialog können Sie importierte Dokumente aus dem Import-Verzeichnis in den zugehörigen Nummernverwalter stellen.
⇨ Tutorial, "Import von Dokumenten" auf Seite C-1639

Über die Checkbox **Automatisch aktualisieren alle X Sekunden** wird die Tabelle mit den Dokumenten aktualisiert. Die untere Grenze des Intervalls beträgt 5 Sekunden. Die Schaltfläche **Dateien einlesen** startet einen erneuten Import.

Per Doppelklick auf ein Dokument wird ein neuer Dialog angezeigt, in dem alle Daten des ausgewählten Dokumentes bearbeitet werden können. Per Rechtsklick auf ein Dokument erscheint ein Kontextmenü über welches zusätzlich zur Anzeige des Dokumentes auch eine evtl. nicht mehr gültige Sperre aufgehoben werden kann. Für das Aufheben dieser Sperre ist ein Sub-Recht des Import Dialoges erforderlich. Sind keine Rechte angelegt, so ist die Aufhebung der Sperre für jeden Anwender möglich.

In dem Menü Optionen ist einstellbar, ob der Fortschritt über den Import auf dem Dialog angezeigt wird oder nicht. Ist der Fortschritt ausgeblendet, so wird er automatisch beim Start einer Aktion dargestellt. Über die Schaltfläche [Fortschritt ausblenden] kann er erneut ausgeblendet werden.

> **Customizing Funktion zum Einlagern der Dateien**
> Das Programm lagert entweder beim Start des Import-Dialoges oder beim Betätigen der Schaltfläche [Dateien einlesen] die Fremddokumente in den Puffertabellen ein. Diese Funktionalität kann auch über einen Workflow per Customizing ausgeführt werden. Wenn Sie diese Funktion nutzen wollen, wenden Sie sich bitte an Ihren Service-Mitarbeiter bei der A+W Software GmbH.

**Auswahl der Fremddokumente**
Die Auswahl der einzelnen Dokumente zum Import erfolgt direkt in der Tabelle durch entsprechendes Markieren. Die drei Schaltflächen oberhalb der Tabelle können verwendet werden, um alle oder keine Dokumente auszuwählen. Die dritte Schaltfläche startet einen Auswahldialog in den bestimmten Kriterien zur Auswahl eingegeben werden können.

*Abb. C-362 Markierungsoptionen*

**Mehrbenutzer-Betrieb**
Sobald ein anderer Benutzer ein Dokument zum Import ausgewählt hat, wird dieses in der eigenen Ansicht mit einem Icon markiert und kann nicht mehr ausgewählt werden.
Auf diese Weise wird verhindert, dass ein Dokument an mehreren Stellen importiert und somit dupliziert wird. Der Mitarbeiter, der momentan ein Dokument bearbeitet und ausgewählt hat, wird mit seinem Namen in der Tabelle angezeigt.
Alle auftretenden Ereignisse werden in der unteren Hälfte des Dialoges in einer Tabelle als Fortschritt dargestellt. Über das Menü Optionen sind die Meldungstypen (Info, Warnung und Fehler) des Fortschritts einzeln auswählbar. Auch, ob beim Start die Dateien in die Puffertabellen übertragen werden, kann hier eingestellt werden. Ist dies deaktiviert, kann die Übertragung über die Schaltfläche [Dateien einlesen] gestartet werden.

### Fehlende Referenzen

> Dokumente > Auftrag > Import > Register Fehlende Referenzen

*Abb. C-363 Import - Fehlende Referenzen*

Es wird automatisch geprüft, ob für die ausgewählten Dokumente alle Artikel in den B2B Artikel-Referenzen angelegt wurden. Sind alle Referenzen vorhanden und korrekt angelegt wird dieses Register nicht aktiv. Fehlt eine Referenz, wird diese in der Tabelle angezeigt.

Durch einen Doppelklick wechselt das Programm in den Verwaltungsdialog der Artikel-Referenzen, startet dessen Neu-Modus und belegt die bekannten Datenfelder (Fremdartikelnummer/Kunde) bereits vor. Sie müssen dann nur die fehlenden Daten ergänzen und speichern. Sobald der Dialog geschlossen und Sie sich wieder in diesem Register befinden, erfolgt eine erneute Prüfung der Referenzen.
⇨ Stammdaten: Softwarereferenz, "Produkte - Stückliste" auf Seite B-1238

Dokumente, die aufgrund von fehlerhaften Daten nicht importiert werden konnten, können Sie über den Dialog Fremddokumentenverwaltung öffnen und korrigieren.
⇨ "Fremddokumentenverwaltung" auf Seite C-1980

### Dokumente erstellen

> Dokumente > Auftrag > Import > Register Dokumente erstellen

*Abb. C-364 Import - Dokumente erstellen*

Sind alle Referenzartikel vorhanden, können Sie in das Register 3. Dokumente erstellen wechseln. Es erscheint eine Darstellung des aktuell ausgewählten Nummernverwalters mit den darin befindlichen Dokumenten. Sie können nun den Nummernverwalter auswählen, in den die Dokumente importiert werden sollen, oder durch Eingabe eines neuen Namens einen neuen Nummernverwalter erzeugen.

Über die Felder im Bereich Parameter können Sie den Mandant und den AV-Bereich vorgegeben. Durch Klicken auf [OK] bzw. durch drücken der <Enter> - Taste wird der Import gestartet. Sofern keine Vorgabe der Dokumentennummer definiert wurde, wird der Nummernkreis des angegebenen Mandanten und AV-Bereichs verwendet.

Nach erfolgreichem Import erscheinen die importierten Dokumente in der Übersicht des Nummernverwalters.

### Fremddokumentenverwaltung

> Dokumente > Auftrag > Import > Doppelklick auf Dokument > Fremddokumentenverwaltung

Der Dialog Fremddokumentenverwaltung ist für Auftrag, Angebot und Gutschrift gleich. Er wird in dieser Anleitung am Beispiel Auftrag beschrieben.

*Abb. C-365 Import - Fremddokumentenverwaltung*

In diesem Dialog werden Details zum Import der Fremddokumente angezeigt. Die Einstellungen müssen i. d. R. nicht bearbeitet werden.
Die importierten Dokumente werden den hinterlegten Import-Regeln entsprechend eingelesen und in neue Aufträge geschrieben.
⇨ Tutorial, "Import von Dokumenten" auf Seite C-1639

## Objektabrechnung

> Dokumente > Auftrag > Objektabrechnung

Die Dialoge für die Abrechnung von Objekten stehen nur zur Verfügung, wenn in den Firmendaten die entsprechende Objektverwaltung aktiviert ist und die Objekte angelegt und zugewiesen sind.
⇨ Stammdaten, "Firmendaten - Dokumente" auf Seite B-1066
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Abrechnung" auf Seite C-1981
- "Objekte - Dokumente" auf Seite C-1992
- "Stundenforderung" auf Seite C-1993
- "Einkaufsforderung" auf Seite C-1994
- "Forderungsberechnung" auf Seite C-1995
- "Forderungs-Historie" auf Seite C-1997

### Abrechnung

> Dokumente > Auftrag > Objektabrechnung > Abrechnung

**Zu Dialogbeschreibung:**
- ⇨ Objekte - Dokumente
- ⇨ Stundenforderung
- ⇨ Einkaufsforderung
- ⇨ Forderungsberechnung
- ⇨ Forderungs-Historie

Je nach der Objektverwaltung, die in den Firmendaten aktiviert wurde, werden im Dialog Abrechnungen unterschiedliche Register angezeigt. In den folgenden Beschreibungen wird daher darauf hingewiesen, in welcher der Objektverwaltungen die Register und Felder freigeschaltet sind.
⇨ Tutorial 2, "Objekt-/Abrechnungsverwaltung" auf Seite B-568

> **Dialog für Kunden- und Lieferantendaten**
> Der Dialog Objekte ist für Kunden und Lieferanten identisch aufgebaut. Er wird in dieser Anleitung am Beispiel Auftrag beschrieben.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite C-1982
- "Menü Druck" auf Seite C-1982
- “Objekte – Abrechnungen” auf Seite C-1983
- "Objekte - Rahmenauftrag" auf Seite C-1986
- "Objekte - Zugeordnete Aufträge" auf Seite C-1987
- "Objekte - Zugeordnete Bestellungen" auf Seite C-1988
- "Objekte - Summen" auf Seite C-1989
- "Objekte - Veranschlagte Mengen" auf Seite C-1990
- "Objekte - Tabelle" auf Seite C-1991

#### Menü Funktionen

> Dokumente > Auftrag > Objektabrechnung > Abrechnung > Menü Funktionen

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Abrechnungsverwaltung zu schließen. Die Funktionen sind je nach aktiviertem Modus der Objektverwaltung freigeschaltet.
Folgende Einträge werden angezeigt:
- **Stundenforderungen hinzufügen**: Öffnet den Dialog Stundenforderung, in dem Sie z. B. Beträge für Monteurstunden erfassen können (nur Abrechnungsverwaltung). ⇨ "Stundenforderung" auf Seite C-1993
- **Einkaufsforderungen hinzufügen**: Öffnet den Dialog Einkaufsforderung, in dem Sie z. B. Beträge für Montagematerial erfassen können (nur Abrechnungsverwaltung). ⇨ "Einkaufsforderung" auf Seite C-1994
- **Forderungsrechnung erstellen**: Öffnet den Dialog Forderungsberechnung, in dem Sie Forderungsrechnungen erstellen und prüfen können. ⇨ "Forderungsberechnung" auf Seite C-1995

#### Menü Druck

> Dokumente > Auftrag > Objektabrechnung > Abrechnung > Menü Druck

Über dieses Menü können Sie Übersichten zu den Abrechnungen erzeugen. Die Einträge sind nur freigeschaltet, wenn Sie den Modus **Abrechnungsverwaltung** aktiviert haben.
Das Menü ist in folgende Gruppen gegliedert:
- Gruppe Bildschirm, Gruppe Drucker
- Gruppe Status Report
- Gruppe Auflistung

##### Gruppe Bildschirm, Gruppe Drucker

- **Druck nach WGR**: Im Druck werden die Positionen nach Warengruppen sortiert.
- **Druck nach Produkt**: Im Druck werden die Positionen nach Produkten sortiert.
- **Bildschirm**: Ein einzelnes Dokument wird auf dem Bildschirm angezeigt und kann geprüft werden.
- **Drucker**: Die Dokumente werden direkt an den Drucker übergeben und gedruckt.

##### Gruppe Status Report

- **Status Report**: Erstellt eine Liste aller Abrechnungsprojekte mit den aktuellen Forderungssummen und dem aktuellen Saldo.

##### Gruppe Auflistung

- **Auflistung**: Erstelle eine Übersicht zu den veranschlagten Summen und den aufgelaufenen Kosten für das markierte Abrechnungsprojekt.
    - **Bildschirm**: Ein einzelnes Dokument wird auf dem Bildschirm angezeigt und kann geprüft werden.
    - **Drucker**: Die Dokumente werden direkt an den Drucker übergeben und gedruckt.

### Objekte - Abrechnungen

> Dokumente > Auftrag > Objektabrechnung > Abrechnung > Register Abrechnungen

*Abb. C-366 Objekte - Abrechnungen*

In diesem Register fügen Sie zusätzliche Angaben zu einem Objekt ein, z. B. eine abweichende Lieferanschrift und abweichende Zahlungsbedingungen.

#### Auswahl

**Angebot**: Nummern des Angebots, sofern ein Angebot erfasst wurde.
**Kundenauftr. Nr**: Nummern des Auftrags, den der Kunde gesendet hat.
**Einfügedatum**: Datum, an dem Sie die Nummer hinterlegt haben.
**Objekt, Abrechnung**: Nummer des Objekts oder der Abrechnung, die zum Rahmenauftrag erfasst wurde.
**[Dokumente/Info]**: Öffnet eine Übersicht über die Aufträge, die zu dem gewählten Objekt erfasst worden sind (nur Standard Objektverwaltung). ⇨ "Objekte - Dokumente" auf Seite C-1992
**Kunde**: Kunde, der an diesem Objekt beteiligt ist. Bei Erfassen eines Dokuments werden nur die Objekte angezeigt, die dem Kunden in den Stammdaten zugeordnet sind.
**Rahmenauftrag**: Nummer des Rahmenauftrags, zu dem die Abrechnung erfasst wird (nur Objektverwaltung + Abrechnungsverwaltung).

#### Modalitäten

Dieser Bereich wird nur angezeigt, wenn in den Firmendaten die Erweiterte Objektverwaltung aktiviert ist.
⇨ "Erweiterte Objektverwaltung" auf Seite B-956

**Gültig von, bis**: Anfangs- und Enddatum des Zeitraums, in dem das Objekt in einem Dokument erfasst werden kann.
**Vertreter**: Vertreter, der für den Marktpartner zuständig ist. Die Umsätze werden dann zu Berechnung seiner Provision herangezogen.
**Zahlungsbedingung**: Zahlungsbedingungen, wenn diese von denen in der Partnerverwaltung oder im Dokument abweichen. Die Einstellung wird in das Dokument zurückgeschrieben, wenn das Objekt zugeordnet wird.
**Nettoumsatz, Qm, Stück**: Für jedes Kundenobjekt können Sie Höchstwerte angeben, die für den jeweiligen Kunden gelten. Beim Schließen der Auftragserfassung wird eine Übersicht über die bereits erfassten Aufträge und die aufgelaufenen Summen angezeigt.

#### Definition

**Anrede**: Anrede, die in den Dokumenten gedruckt werden soll, z. B. Firma.
**Name 1-3**: In den drei Feldern können Sie neben dem Namen auch Zusätze eintragen, z. B. Firmengruppe.
**Straße**: Straße, in der der Sitz des Kunden ist.
**Provinz / Land**: Provinz und Landeskürzel, die in Dokumenten zur korrekten Bezeichnung der Anschrift gedruckt werden sollen. Das Feld Provinz ist für USA und Kanada vorgesehen.
**PLZ / Ort**: Postleitzahl und Ort.
**Abrechnung**: Datum oder Nummer der Abrechnung.
**Telefon**: Telefonnummer eines Ansprechpartners für das Objekt, z. B. des Bauleiters.
**Mitarbeiter**: Mitarbeiter, der den Partner betreut.
**Status**: Status, in dem sich das Objekt befindet:
- **Aktuell**: Zu diesem Objekt können Dokumente erfasst werden.
- **Komplett**: Das Objekt ist abgeschlossen. Zu diesem Objekt können keine Dokumente mehr erfasst werden. Der Status wird automatisch gesetzt, wenn die vereinbarten Höchstwerte erreicht sind. Er kann vorzeitig manuell gesetzt werden.
**Entfernung**: Entfernung in Kilometer, die pro Tour berechnet werden, d. h. die einfache Entfernung zum Kunden. Dieser Wert wird zusammen mit der Kilometerpauschale aus der zugewiesenen Tour zur Berechnung der Frachtkosten herangezogen.

**Übernahme in Auftrag**: Die Felder im Bereich Definition können in den Auftrag übernommen werden.
- ☐ Die Felder werden nicht in den Auftrag übernommen.
- ☑ Die Felder werden in den Auftrag übernommen.

**Info, Memo**: Zusätzliche Information.

### Objekte – Rahmenauftrag

> Dokumente > Auftrag > Objektabrechnung > Abrechnung > Register Rahmenauftrag

*Abb. C-367 Objekte - Rahmenauftrag*

Dieses Register wird nur angezeigt, wenn die Funktion **Abrechnungsverwaltung mit zugeordneten Aufträgen** aktiviert ist. Die Positionen und Mengen des Rahmenauftrags werden angezeigt.
⇨ Tutorial 2, "Rahmenauftrag abrechnen" auf Seite B-582

Über das Kontextmenü (rechte Maustaste) können Sie den Dialog **Forderungs-Historie** öffnen, um sich eine Übersicht über Forderungen anzeigen lassen.
⇨ "Forderungs-Historie" auf Seite C-1997

#### Summen

In diesem Bereich werden der Gesamt-VK und der Gesamt-EK für den Rahmenauftrag angezeigt.
Zusätzlich werden der bereits berechnete Betrag und der Prozentsatz angezeigt, den dieser Betrag von Gesamt-VK ausmacht.
Diese beiden Werte werden mit jeder weiteren Abrechnung aktualisiert. Sie geben jedoch nicht wieder, ob der Betrag bereits gezahlt wurde.

### Objekte - Zugeordnete Aufträge

> Dokumente > Auftrag > Objektabrechnung > Abrechnung > Register Zugeordnete Aufträge

*Abb. C-368 Objekte - Zugeordnete Aufträge*

In diesem Register lassen Sie sich die zugeordneten Aufträge und Gutschriften anzeigen. Das Register ist nur freigeschaltet, wenn die **Abrechnungsverwaltung mit zugeordneten Aufträgen** oder die **Standard Objektverwaltung + Abrechnungsverwaltung mit zugeordneten Aufträgen** aktiviert ist.

> **Zugeordnete Dokumente**
> Bei der Standard-Objektverwaltung können Sie sich die Aufträge und Bestellungen anzeigen lassen, indem Sie im Register Abrechnung auf die Schaltfläche [Dokumente/Info] klicken.

### Objekte - Zugeordnete Bestellungen

> Dokumente > Auftrag > Objektabrechnung > Abrechnung > Register Zugeordnete Bestellungen

*Abb. C-369 Objekte - Zugeordnete Bestellungen*

In diesem Register lassen Sie sich die zugeordneten Bestellungen anzeigen. Das Register ist nur freigeschaltet, wenn die **Abrechnungsverwaltung mit zugeordneten Aufträgen** oder die **Standard Objektverwaltung + Abrechnungsverwaltung mit zugeordneten Aufträgen** aktiviert ist.
Das Register wird nicht angezeigt, wenn die **Erweiterte Objektverwaltung** aktiviert ist.

**Auftragsbezogene Bestellungen**: Umschaltung der Anzeige.
- ☐ Die manuell erfassten Bestellungen zum Objekt werden angezeigt.
- ☑ Die referenzierten Bestellungen zum Objekt werden angezeigt.

### Objekte – Summen

> Dokumente > Auftrag > Objektabrechnung > Abrechnung > Register Summen

*Abb. C-370 Objekte - Summen*

In diesem Register werden die Summen angezeigt, die bisher für das gewählte Objekt aufgelaufen sind. Das Register ist nur freigeschaltet, wenn die **Erweiterte Objektverwaltung** aktiviert ist.
Die Summen werden in roter Schrift dargestellt, wenn die veranschlagten Mengen erreicht oder überschritten sind.
⇨ "Objekte - Veranschlagte Mengen" auf Seite C-1990

#### Produkte, Warengruppen

In den Übersichten werden die aktuellen Werte für Produkte und/oder Warengruppen angezeigt.

### Objekte – Veranschlagte Mengen

> Dokumente > Auftrag > Objektabrechnung > Abrechnung > Register Veranschlagte Mengen

*Abb. C-371 Objekte - Veranschlagte Mengen*

In diesem Register hinterlegen Sie zu einem Objekt Angaben zur geplanten Menge. Diese Angaben werden bei der Berechnung der Summen herangezogen. Das Register ist nur freigeschaltet, wenn die **Erweiterte Objektverwaltung** aktiviert ist.

#### Übersicht

In der Übersicht werden alle Produkte bzw. Warengruppen aufgelistet, zu denen Sie veranschlagte Mengen eingegeben haben.

#### Auswahl

Mit der Wahl der Option legen Sie fest, wofür Sie die Mengen veranschlagt haben:
- **Produkt**: Wenn Sie eine Produktnummer eingegeben haben, wird die Produktbezeichnung angezeigt.
- **WGR**: Wenn Sie die Nummer einer Warengruppe eingegeben haben, wird deren Bezeichnung angezeigt. Sie können nur eine WGR auswählen. Die Auswahl einer WOB oder WHG ist nicht möglich.

**Veran. Qm**: Glasfläche, die maximal verbaut werden darf.
**Veran. Stück**: Stückzahl der Gläser, Scheiben oder Artikel, die höchstens verbaut werden darf.
**Veran. Umsatz**: Netto-Höchstbetrag, der für das Objekt erreicht werden darf. Beim Schließen der Auftragserfassung wird eine Übersicht über die bereits erfassten Aufträge und die aufgelaufenen Summen angezeigt. Die Werte werden im Register Summen zur Berechnung herangezogen.

#### Schaltflächen

Über die Schaltflächen können Sie einen Eintrag hinzufügen oder löschen. Beim Hinzufügen werden die Felder für die veranschlagten Mengen freigeschaltet. Achten Sie darauf, dass Sie die richtige Option (Produkt, WGR) gewählt haben, bevor Sie eine neue Zeile einfügen.

### Objekte - Tabelle

> Dokumente > Auftrag > Objektabrechnung > Abrechnung > Register Tabelle

*Abb. C-372 Objekte - Tabelle*

In diesem Register werden je nach Objektverwaltung alle Objekte oder Abrechnungen angezeigt, die den Auswahlkriterien entsprechen. Wenn Sie keine Kriterien angegeben haben, werden alle Objekte angezeigt.

### Objekte – Dokumente

> Dokumente > Auftrag > Objektabrechnung > Abrechnung > Register Abrechnungen > [Dokumente/Info]

*Abb. C-373 Objekte - Dokumente*

In diesem Dialog werden alle Dokumente aufgelistet, die dem aktuellen Objekt zugeordnet sind. Der Dialog steht nur in der **Standard-Objektverwaltung** zur Verfügung.
Der Dialog wird auch angezeigt, wenn die Positionserfassung geschlossen wird. Dann werden jedoch nur die Aufträge aufgelistet, die für den aktuellen Kunden zu dem Objekt erfasst wurden.

### Stundenforderung

> Dokumente > Auftrag > Objektabrechnung > Abrechnung > Menü Funktionen > Stundenforderungen hinzufügen

*Abb. C-374 Stundenforderung hinzufügen*

In diesem Dialog hinterlegen Sie den Betrag, der für Zusatzleistungen erbracht wurde, z. B. für Montage-Arbeiten. Der Betrag wird dem ausgewählten Projekt zugeordnet.
Die Funktion ist nur freigeschaltet, wenn Sie den Modus **Abrechnungsverwaltung mit zugeordneten Aufträgen** aktiviert haben.

**Abrechnungsnummer**: Nummer der Abrechnung, zu der die Stundenforderung hinzugefügt werden soll.
**Wert**: Betrag der Stundenforderung.

### Einkaufsforderung

> Dokumente > Auftrag > Objektabrechnung > Abrechnung > Menü Funktionen > Einkaufsforderungen hinzufügen

*Abb. C-375 Einkaufsforderung hinzufügen*

In diesem Dialog hinterlegen Sie den Betrag, der für Zusatzkäufe erbracht wurde, z. B. für Montagematerial. Der Betrag wird dem ausgewählten Projekt zugeordnet.
Die Funktion ist nur freigeschaltet, wenn Sie den Modus **Abrechnungsverwaltung mit zugeordneten Aufträgen** aktiviert haben.

**Abrechn.Nr.**: Nummer der Abrechnung, zu der die Einkaufsforderung hinzugefügt werden soll.
**Wert**: Betrag der Einkaufsforderung.

### Forderungsberechnung

> Dokumente > Auftrag > Objektabrechnung > Abrechnung > Menü Funktionen > Forderungsrechnung erstellen

Dieser Dialog wird je nach aktivierter Objektverwaltung unterschiedlich angezeigt:
- "Abrechnungsverwaltung + Zugeordnete Aufträge" auf Seite C-1995
- "Abrechnungsverwaltung" auf Seite C-1996

#### Abrechnungsverwaltung + Zugeordnete Aufträge

*Abb. C-376 Abrechnungsverwaltung mit zugeordneten Aufträgen – Forderungsrechnung*

In diesem Dialog wird angezeigt, welche Summen bereits durch Forderungsrechnungen abgedeckt sind. Zu den verbliebenen Mengen können Sie dann weitere Forderungsrechnungen erstellen, indem Sie in der Spalte `zu ber. Menge` den gewünschten Wert eingeben.

Über den eingegebenen Wert wird ein Dokument vom Typ **Forderung** erstellt, das Sie in der Dokumentenverwaltung für Aufträge öffnen und bearbeiten können. Die Nummer des neuen Dokuments können Sie sich in der Forderungshistorie anzeigen lassen.
⇨ "Forderungs-Historie" auf Seite C-1997

Der Dialog wird auch angezeigt, wenn die **Standard Objektverwaltung + Zugeordnete Aufträge** aktiviert ist.

#### Abrechnungsverwaltung

*Abb. C-377 Abrechnungsverwaltung - Forderungsrechnung*

In diesem Dialog können Sie die Forderungen erfassen, die zu einem Abrechnungsobjekt entstanden sind. Der Dialog ist nur kundenspezifisch freigeschaltet.

### Forderungs-Historie

> Dokumente > Auftrag > Objektabrechnung > Abrechnung > Register Rahmenauftrag > Kontextmenü auf eine der angezeigten Positionen

*Abb. C-378 Objekte - Forderungs-Historie*

In diesem Dialog wird angezeigt, welche Summen bereits durch Forderungsrechnungen abgedeckt sind.
Je nach der Wahl des Eintrags im Kontextmenü werden folgende Details angezeigt:
- **Forderungshistorie nach Dokumenten**: Alle Dokumente zum Rahmenauftrag werden angezeigt.
- **Forderungshistorie nach Positionen**: Nur die Dokumente zur aktuellen Position werden angezeigt.

## Auswertungen

> Dokumente > Auftrag > Auswertungen

In diesem Bereich finden Sie Dialoge, über die Sie verschiedene Auswertungen erstellen können.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Preisänderung (Report)" auf Seite C-1998
- "Null-Preisreport" auf Seite C-2000
- "Deckungsbeitrags-Analyse" auf Seite C-2002
- "Kalkulatorische Frachtkosten" auf Seite C-2006

### Preisänderung (Report)

> Dokumente > Auftrag > Auswertungen > Preisänderung

*Abb. C-379 Preisänderungsreport*

In diesem Dialog können Sie sich eine Übersicht über die Preisänderungen für Aufträge und Angebote anzeigen oder drucken lassen.

#### Auswahl

**Datum von, Datum bis**: Sie können die Auswertung auf einen beliebigen Zeitraum.
**Auftragsnummer von, Auftragsnummer bis**: Sie können die Auswertung auf eine Spanne von Auftragsnummern einschränken.
**Kunde von, Kunde bis**: Sie können die Auswertung auf eine Spanne von Kundennummern einschränken.
**Aufträge, Angebote**: Sie können die Auswertung auf Aufträge oder Angebote einschränken.
**Archive mit einbeziehen**: Außerdem können Sie die Archive in die Auswertung einbeziehen.
- ☐ Die Auswertung zieht archivierte Dokumente nicht mit ein.
- ☑ Die Auswertung sucht auch in den Archiven nach entsprechenden Dokumenten. Beachten Sie dabei, dass die Auswertung u. U. sehr lange dauert.

#### Preise

Mit der Wahl der Option legen Sie fest, nach welchen Preisänderungen gesucht werden soll:
- **Alle geänderten**: Alle Aufträge mit geänderten Preisen sollen angezeigt werden.
- **Nur geänderte, die niedriger sind**: Nur Aufträge mit niedrigeren Preisen sollen angezeigt werden.
- **Nur geänderte, die höher sind**: Nur Aufträge mit höheren Preisen sollen angezeigt werden.

#### Preisänderungen

In der Übersicht werden alle Dokumente angezeigt, die den Filterbedingungen entsprechen.

### Null-Preisreport

> Dokumente > Auftrag > Auswertungen > Null-Preisreport

*Abb. C-380 Null-Preisreport*

In diesem Dialog können Sie sich Übersichten zu kostenlosen Auftragspositionen anzeigen lassen. Zum Anzeigen der Übersicht wählen Sie jeweils einen Nummernverwalter aus.

#### Kostenlose Auftragspositionen

- **Handelsvertreter**: Name des zuständigen Vertreters.
- **Bearbeiter**: Name des Bearbeiters, der den Auftrag erfasst hat.
- **Auftrag**: Auftragsnummer. Wenn in einem Auftrag mehrere Positionen ohne Berechnung aufgeführt sind, wird die Auftragsnummer mehrfach aufgelistet.
- **Position**: Positionsnummer aus dem Auftrag.
- **Status**: Auftragsstatus.
- **AB Datum**: Datum der zugehörigen Auftragsbestätigung.
- **Lieferdatum**: Lieferdatum aus dem Auftragskopf.
- **Rechnung**: Rechnungsnummer. Das Feld bleibt leer, wenn noch keine Rechnung erstellt wurde.

