---
title: "DE-HB-AWEnterprise_19"
source: "DE-HB-AWEnterprise_19.pdf"
tags: ["A+W Enterprise", "Lagerverwaltung", "Versandsteuerung", "Software-Referenz", "Help Cards", "Inventur", "Preiskorrektur", "Systemverwaltung", "Warenwirtschaft", "Logistik"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Dieses Dokument ist ein kombiniertes Software-Referenzhandbuch und Tutorial für die Module A+W Enterprise Lager und Versandsteuerung. Es bietet detaillierte Anleitungen für Lager- und Logistikprozesse."
long_description: "Dieses Dokument dient als umfassende Anleitung für die Module A+W Enterprise Lager (Warehouse) und Versandsteuerung (Shipping Control). Es ist in zwei Hauptteile gegliedert. Der erste Teil, die 'Softwarereferenz', beschreibt spezifische Dialoge und Funktionen wie Bestandsprognosen, das Drucken von Etiketten und Listen sowie administrative Aufgaben wie das Löschen von Protokollen, Preiskorrekturen und Datensicherungen. Der zweite, umfangreichere Teil besteht aus 'Help Cards', die als schrittweise Tutorials für eine Vielzahl von Aufgaben konzipiert sind. Diese 'Help Cards' decken das gesamte Spektrum der Lagerverwaltung ab, einschließlich Stammdatenverwaltung, Buchung von Lagerein- und -ausgängen (für verschiedene Lagertypen wie Fach-, Kisten-, Gestell- und Stapellager), Inventurverwaltung, Bewertung und die Nutzung des Infosystems. Jede 'Help Card' folgt einer einheitlichen Struktur mit Ziel, Voraussetzungen, Zusatzinformationen und einem detaillierten Workflow. Der zweite große Themenblock behandelt die Versandsteuerung und bietet ebenfalls eine Mischung aus Tutorial und Referenz. Er deckt Themen wie Versandmodi, den Versand-Explorer, das Verschieben von Touren und Aufträgen, die Versandvorbereitung (z.B. Fehlmengenkontrolle, Lieferscheindruck), die Gestellverwaltung und die Anbindung an den A+W Logistics Optimizer ab. Das Dokument richtet sich an Anwender, die mit den Lager- und Logistikfunktionen von A+W Enterprise arbeiten."
---

# Teil 1: A+W Enterprise Lager - Softwarereferenz

---
## Rumpfbereich

Die Spalten sind im Kopfbereich beschrieben. Zusätzlich werden folgende Spalten angezeigt:

- **Datum**: Datumsangabe für die Bestandsprognose zu verplanten, bestellten und zu dem Zeitpunkt auf Lager vorhandenen Artikeln.
- **Verplant**: Verplante Artikel aus dem Lager, zu dem entsprechend in der ersten Spalte angezeigten Datum.
- **Bestellt**: Bestellte Artikel für das Lager, zu dem entsprechend in der ersten Spalte angezeigten Datum.
- **Bestand**: Bestand des Artikels auf Lager, zu dem entsprechend in der ersten Spalte angezeigten Datum.

## Druck

Im Druck können Sie Informationen über die Lagerdaten oder Etiketten drucken. Sie können das Seitenlayout für den Listendruck oder die Etiketten frei definieren.

In diesem Abschnitt sind folgende Dialoge erklärt:
- Kistenetiketten drucken
- Listendruck

### Kistenetiketten drucken

**Navigation**: `Druck > Etiketten`

*Abb. F-66: Kistenetiketten drucken*

In diesem Dialog können Sie sich die offenen Druckaufträge für Kistenetiketten anzeigen lassen und drucken.

Mit `<Shift>` + `<F3>` starten Sie den Etikettendruck.

- **Kiste**: Kistennummer.
- **Anzahl**: Stückzahl der Artikel in der Kiste.
- **Artikel**: Artikelnummer.
- **Variante**: Maßvariante des Artikels.
- **Lager**: Lagernummer.
- **Kost.St.**: Bezeichnung der Kostenstelle.
- **Spalte ohne Bezeichnung**: Anzeige für den Etikettendruck:
  - J = Etiketten drucken.
  - N = Keine Etiketten drucken.
- **Anz.**: Anzahl der zu druckenden Etiketten.
- **Erfasst**: Datum, an dem der Kisteneingang erfasst wurde.
- **Gedruckt**: Datum, an dem das Etikett der Kiste zuletzt ausgedruckt wurde.

### Listendruck

**Navigation**: `Druck > Listendruck`

*Abb. F-67: Listendruck*

Der Dialog ist ausführlich an folgender Stelle beschrieben:
- Verkauf, "Listendruck" auf Seite D-1428

## Systemverwaltung

In der Systemverwaltung können Sie die Lagerprotokolle und die Preiskorrekturen der Lagerartikel verwalten.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Lagerprotokoll löschen" auf Seite F-1804
- "Lager-Preiskorrektur" auf Seite F-1805
- "Lagersicherung" auf Seite F-1806

### Lagerprotokoll löschen

**Navigation**: `System > Lagerprotokoll löschen`

*Abb. F-68: Lagerprotokoll löschen*

In diesem Dialog können Sie ein Lagerprotokoll entsprechend der Auswahlkriterien im System löschen.

- **Artikel**: Artikelnummer.
- **Lager**: Lagernummer.
- **Variante**: Maßvariante des Artikels.
- **Farbe**: Farbvariante des Artikels.

### Lager-Preiskorrektur

**Navigation**: `System > Preiskorrektur`

*Abb. F-69: Lager-Preiskorrektur*

In diesem Dialog können Sie den Durchschnittspreis für eingekaufte Lagerartikel korrigieren. Fehlerhafte Preisbuchungen für Lagerartikel verfälschen den Durchschnittspreis in der Statistik und können nur über den Höchstpreis und den Niedrigstpreis korrigiert werden.

- **Artikel**: Artikelnummer.
- **Lager**: Lagernummer.
- **Variante**: Maßvariante des Artikels.
- **Farbe**: Farbvariante des Artikels.
- **Höchstpreis**: Höchster Einkaufspreis der Variante im Lager.
- **Niedrigstpreis**: Niedrigster Einkaufspreis der Variante im Lager.

### Lagersicherung

**Navigation**: `System > Lagersicherung`

*Abb. F-70: Lagersicherung*

> In diesem Dialog wir die Information zur letzten Datensicherung vermerkt. Wenn Sie die Lagerdaten sichern möchten, benötigen Sie eine entsprechende System-Konfiguration. Die Sicherung kann nur ein dafür autorisierte Mitarbeiter ausführen. In der Konfiguration können Sie festlegen, in an welchem Tag die automatisierte Sicherung der Lagertabellen: `wlfach`, `wlgest`, `wlx`, `wlxifo`, `wlxv` gemacht wird.
>
> **Sicherungstag**
> Der Standardwert in der Konfiguration ist der 16. des Monats. Sie können die Sicherung auch für andere Tage festlegen: gültige Einstellungen sind zwischen 1 und 31, wobei 31 immer der letzte Tag im Monat ist und wird automatisch an den Monat angepasst (28(29), 30 oder 31).
>
> Zu dem Zeitpunkt der Sicherung dürfen keine Lagerinventuren und keine fehlerhafte Buchungen offen sein, ansonsten kann die Sicherung nicht durchgeführt werden. Im Erfolgsfall sowie auch im Fehlerfall kann ein zuständige Mitarbeiter per E-Mail über das Ergebnis informiert werden. Bitte sprechen Sie einen A+W Mitarbeiter für die korrekte Systemeinstellung dieser Funktion an.

- **Datum**: Datum der letzten Sicherung.
  - Technische Info: Anzeige-Feld, DB-Info: `wlx_m.savedate`
- **Zeit**: Zeitpunkt der letzten Sicherung.
  - Technische Info: Anzeige-Feld, DB-Info: `wlx_m.savetime`

# Teil 2: A+W Enterprise Lager - Help Cards

## A+W Enterprise Lager

In diesem Kapitel finden Sie folgende Themen:
- Informationen zu den HelpCards
- Stammdatenverwaltung
- Inventurverwaltung
- Bewertung
- Infosystem
- Druck
- System

**Inhaltsverzeichnis:**
- Informationen zu den HelpCards (F-1809)
- Stammdatenverwaltung (F-1810)
  - Lagerraum anlegen (F-1811)
  - Lagerartikel festlegen (F-1812)
- Lagerverwaltung (F-1813)
  - Lagereingang buchen (F-1814)
  - Lagerausgang buchen (F-1815)
  - Fachlagereingang buchen (F-1816)
  - Fachlagerausgang buchen (F-1817)
  - Kistenlagereingang buchen (F-1818)
  - Kistenlagerausgang buchen (F-1819)
  - Einzelblattkistenlager einbuchen (F-1820)
  - Einzelblattkistenlager ausbuchen (F-1821)
  - Gestelllagereingang buchen (F-1822)
  - Gestelle auftragsbezogen ausbuchen (F-1823)
  - Gestelllager Artikel umbuchen (F-1824)
  - Auftragsbezogene Ausgänge buchen (F-1825)
  - Stapellagereingang buchen (F-1826)
  - Änderung im Stapellager buchen (F-1827)
  - Buchungskorrektur buchen (F-1828)
- Inventurverwaltung (F-1829)
  - Inventur im Lager durchführen (F-1830)
- Bewertung (F-1831)
  - Bewertung im Lager vornehmen (F-1832)
- Infosystem (F-1833)
  - Infos zu Artikeln einsehen (F-1834)
  - Lagerhistorie einsehen (F-1835)
  - Aufträge / Bestellungen einsehen (F-1836)
  - Buchungsstatus einsehen (F-1837)
  - Dispositiven Lagerbestand einsehen (F-1838)
  - Bestandsprognose einsehen (F-1839)
- Druck (F-1840)
  - Kistenetiketten drucken (F-1841)
- System (F-1842)
  - Lagerprotokoll löschen (F-1843)
  - Durchschnittspreis korrigieren (F-1844)

## Informationen zu den HelpCards

Die Darstellungen in den Help Cards basieren auf der Auslieferversion A+W Enterprise 2015. Einzelne Schritte in den Workflows können je nach Konfiguration abweichen.

## Stammdatenverwaltung

| Help Card | Themen |
| :--- | :--- |
| Lagerraum anlegen | Ein Lager und alle zugehörigen Stammdaten definieren. |
| Lagerartikel festlegen | Lagerartikel pro Lager verwalten. |

### Lagerraum anlegen (SD 01-001)

#### Ziel der Handlung
Ein Lager und alle zugehörigen Stammdaten definieren.

#### Voraussetzungen
(keine)

#### Zusatzinfo
Die Strukturierung der Lagerstammdaten anhand des Lagers ist wohlüberlegt zu definieren, da nachträgliche Änderungen nur mit hohem Aufwand durchgeführt werden können. Bei Unklarheiten unbedingt Rücksprache mit der A+W Software GmbH halten.

#### Workflow
1.  Menü `Stammdaten > Raum` wählen. Der Dialog `Lagerraumverwaltung` wird geöffnet.
2.  Mindestens die folgenden Stammdaten für das neue Lager eingeben:
    - Lagernummer eingeben.
    - Bezeichnung und Kurzbezeichnung des Lagers eingeben.
    - Mandant (im Haus) wählen.
    - Inventurart wählen.
    - Lagerart wählen.
3.  Definition mit [OK] bestätigen.
    - Nächster Schritt: Lagerartikel festlegen.

### Lagerartikel festlegen (SD 01-002)

#### Ziel der Handlung
Lagerartikel pro Lager verwalten.

#### Voraussetzungen
- Lager ist in den Stammdaten angelegt.
- Artikel mit Varianten ist mit der Beschaffungsart Lager in den Stammdaten angelegt.

#### Zusatzinfo
- Lager anlegen: `A+W Enterprise > LAGER > Stammdaten > Raum`.
- Artikel anlegen: `A+W Enterprise > A+W Enterprise > Stammdaten > Artikel`.

#### Workflow
1.  Menü `Stammdaten > Artikel` wählen. Der Dialog `Artikelstammdaten Lager` wird geöffnet.
2.  Artikel und Lager wählen.
3.  Artikelvariante wählen.
4.  Bestandsgrenze für die Bestellvariante in den Spalten Mindest, Alarm und Maximal eingeben.
5.  Bestandsgrenzen pro Artikelvariante eingeben.
6.  Bei Bedarf, pro Variante eine Bemerkung mit `<F5>` erfassen.
7.  Definitionen der Bestandsgrenzen mit `<Ende>` speichern.

## Lagerverwaltung

| Help Card | Themen |
| :--- | :--- |
| Lagereingang buchen | Artikel im Lagereingang buchen. |
| Lagerausgang buchen | Artikel im Lagerausgang buchen. |
| Fachlagereingang buchen | Artikel im Fachlagereingang buchen. |
| Fachlagerausgang buchen | Artikel im Fachlagerausgang buchen. |
| Kistenlagereingang buchen | Komplette Kiste im Kistenlagereingang buchen. |
| Kistenlagerausgang buchen | Komplette Kiste im Kistenlagerausgang buchen. |
| Einzelblattkistenlager einbuchen | Einzelne Glasblätter in das Einzelblattkistenlager buchen. |
| Einzelblattkistenlager ausbuchen | Einzelblattkiste auflösen und Glasblätter der Einzelblattkiste auf ein anderes Lager buchen. |
| Gestelllagereingang buchen | Artikel auf Gestellen in ein Gestelllager buchen. |
| Gestelle auftragsbezogen ausbuchen | Auftragsbezogene Lagerabgänge im Gestelllager buchen. |
| Gestelllager Artikel umbuchen | Artikelvarianten auf ein neues Gestell bzw. neues Fach umbuchen. |
| Auftragsbezogene Ausgänge buchen | Auftragsbezogene Lagerabgänge buchen. |
| Stapellagereingang buchen | Neue Stapel im Stapellagereingang buchen. |
| Änderung im Stapellager buchen | Artikel auf bestehende Stapel buchen. Stapel auflösen und Artikel aus dem Stapellager buchen. |
| Buchungskorrektur buchen | Buchungen im Lager korrigieren. |

### Lagereingang buchen (LA 01-001)

#### Ziel der Handlung
Artikel im Lagereingang buchen.

#### Voraussetzungen
- Standardlager ist in den Stammdaten angelegt.
- Artikelstammdaten sind vollständig erfasst.
- Je nach Systemkonfiguration müssen die Artikel dem gewählten Haus zugeordnet sein.

#### Zusatzinfo
- Mit `<F5>` aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Ende>` die Eingaben im Fußbereich speichern und in den Rumpfbereich wechseln.
- Buchungen können im Dialog `Buchungskorrektur` korrigiert werden. ⇨ `Buchungskorrektur buchen`

#### Workflow
1.  Menü `Buchung > Eingang` wählen. Dialog `Lagereingang` wird geöffnet.
2.  Artikel und Lager wählen.
3.  Artikelvariante, Artikelmenge und Einkaufspreis pro Stück oder pro Mengeneinheit eingeben. Gesamtpreis der Position wird angezeigt. Detailangaben der Position werden im Fußbereich angezeigt.
4.  Detailinformationen im Fußbereich prüfen.
5.  Schritte 3 und 4 für nächste Artikelvariante wiederholen.
6.  Buchung bestätigen. Artikel werden im Lager eingebucht.

#### Buchung prüfen:
7.  Menü `Infosystem > Buchungsstatus > Ungebucht`: Nicht gebuchte Buchungen.
8.  Menü `Infosystem > Buchungsstatus > Fehler`: Fehlerhafte Buchungen.
9.  Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
10. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
11. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
12. Buchungsdaten prüfen.

### Lagerausgang buchen (LA 01-002)

#### Ziel der Handlung
Artikel im Lagerausgang buchen.

#### Voraussetzungen
- Standardlager ist in den Stammdaten angelegt.
- Artikelstammdaten sind vollständig erfasst.
- Benötigte Menge an Artikeln befindet sich auf Lager.

#### Zusatzinfo
- Mit `<F5>` aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Ende>` die Eingaben im Fußbereich speichern und in den Rumpfbereich wechseln.
- Buchungen können im Dialog `Buchungskorrektur` korrigiert werden. ⇨ `Buchungskorrektur buchen`

#### Workflow
1.  Menü `Buchung > Ausgang` wählen. Dialog `Lagerausgang` wird geöffnet.
2.  Artikel und Lager wählen.
3.  Artikelvariante und Artikelmenge in Stückzahl oder Mengeneinheit eingeben. Gesamtpreis der Position wird angezeigt. Detailangaben der Position werden im Fußbereich angezeigt.
4.  Detailinformationen im Fußbereich prüfen.
5.  Schritte 3 und 4 für nächste Artikelvariante wiederholen.
6.  Buchung bestätigen. Artikel werden vom Lager abgebucht.

#### Buchung prüfen:
7.  Menü `Infosystem > Buchungsstatus > Ungebucht`: Nicht gebuchte Buchungen.
8.  Menü `Infosystem > Buchungsstatus > Fehler`: Fehlerhafte Buchungen.
9.  Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
10. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
11. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
12. Buchungsdaten prüfen.

### Fachlagereingang buchen (LA 01-003)

#### Ziel der Handlung
Artikel im Fachlagereingang buchen.

#### Voraussetzungen
- Fachlager ist in den Stammdaten angelegt.
- Artikelstammdaten sind vollständig erfasst.
- Je nach Systemkonfiguration müssen die Artikel dem gewählten Haus zugeordnet sein.

#### Zusatzinfo
- Mit `<F5>` aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Ende>` die Eingaben im Fußbereich speichern und in den Rumpfbereich wechseln.
- Buchungen können im Dialog `Buchungskorrektur` korrigiert werden. ⇨ `Buchungskorrektur buchen`

#### Workflow
1.  Menü `Buchung > Facheingang` wählen. Dialog `Fachlagereingang` wird geöffnet.
2.  Artikel und Lager wählen.
3.  Artikelvariante, Artikelmenge und Einkaufspreis pro Stück oder pro Mengeneinheit eingeben. Gesamtpreis der Position wird angezeigt. Detailangaben der Position werden im Fußbereich angezeigt.
4.  Detailinformationen im Fußbereich prüfen.
5.  Schritte 3 bis 4 für nächste Artikelvariante wiederholen.
6.  Buchung bestätigen. Artikel werden im Lager eingebucht.

#### Buchung prüfen:
7.  Menü `Infosystem > Buchungsstatus > Ungebucht`: Nicht gebuchte Buchungen.
8.  Menü `Infosystem > Buchungsstatus > Fehler`: Fehlerhafte Buchungen.
9.  Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
10. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
11. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
12. Buchungsdaten prüfen.

### Fachlagerausgang buchen (LA 01-004)

#### Ziel der Handlung
Artikel im Fachlagerausgang buchen.

#### Voraussetzungen
- Fachlager ist in den Stammdaten angelegt.
- Artikelstammdaten sind vollständig erfasst.
- Benötigte Menge an Artikeln befindet sich auf Lager.

#### Zusatzinfo
- Mit `<F5>` aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Ende>` die Eingaben im Fußbereich speichern und in den Rumpfbereich wechseln.
- Buchungen können im Dialog `Buchungskorrektur` korrigiert werden. ⇨ `Buchungskorrektur buchen`

#### Workflow
1.  Menü `Buchung > Fachausgang` wählen. Dialog `Fachlagerausgang` wird geöffnet.
2.  Artikel und Lager wählen.
3.  Artikelvariante und Artikelmenge in Stückzahl oder Mengeneinheit eingeben. Gesamtpreis der Position wird angezeigt. Detailangaben der Position werden im Fußbereich angezeigt.
4.  Detailinformationen im Fußbereich prüfen.
5.  Schritte 3 und 4 für nächste Artikelvariante wiederholen.
6.  Buchung bestätigen. Artikel werden vom Lager abgebucht.

#### Buchung prüfen:
7.  Menü `Infosystem > Buchungsstatus > Ungebucht`: Nicht gebuchte Buchungen.
8.  Menü `Infosystem > Buchungsstatus > Fehler`: Fehlerhafte Buchungen.
9.  Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
10. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
11. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
12. Buchungsdaten prüfen.

### Kistenlagereingang buchen (LA 01-005)

#### Ziel der Handlung
Komplette Kiste im Kistenlagereingang buchen.

#### Voraussetzungen
- Kistenlager ist in den Stammdaten angelegt.
- Artikelstammdaten sind vollständig erfasst.
- Je nach Systemkonfiguration müssen die Artikel dem gewählten Haus zugeordnet sein.

#### Zusatzinfo
- Mit `<F5>` aus einer Spalte in die kistenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Shift>` + `<F8>` aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Ende>` die Eingaben im Fußbereich speichern und in den Rumpfbereich wechseln.

#### Workflow
1.  Menü `Buchung > Kisteneingang` wählen. Dialog `Kistenlagereingang` wird geöffnet.
2.  Artikel und Kistenlager wählen.
3.  Artikelvariante wählen.
4.  Kistenbezeichnung und Verpackungsart eingeben.
5.  Artikelmenge und Artikelpreis des Lieferanten eingeben.
6.  Schritte 3 bis 5 für nächste Kiste wiederholen.
7.  Buchung mit [OK] bestätigen. Kisten werden vom Lager abgebucht.

#### Buchung prüfen:
8.  Menü `Infosystem > Buchungsstatus > Ungebucht`: Nicht gebuchte Buchungen.
9.  Menü `Infosystem > Buchungsstatus > Fehler`: Fehlerhafte Buchungen.
10. Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
11. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
12. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
13. Buchungsdaten prüfen.

### Kistenlagerausgang buchen (LA 01-006)

#### Ziel der Handlung
Komplette Kiste im Kistenlagerausgang buchen.

#### Voraussetzungen
- Kistenlager ist in den Stammdaten angelegt.
- Artikelstammdaten sind vollständig erfasst.
- Benötigte Menge an Artikeln befindet sich auf Lager.

#### Zusatzinfo
- Mit `<F5>` aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Ende>` die Eingaben im Fußbereich speichern und in den Rumpfbereich wechseln.
- Buchungen können im Dialog `Buchungskorrektur` korrigiert werden. ⇨ `Buchungskorrektur buchen`

#### Workflow
1.  Menü `Buchung > Kistenausgang` wählen. Dialog `Kistenlagerausgang` wird geöffnet.
2.  Artikel und Kistenlager wählen.
3.  Kiste mit der entsprechenden Artikelvariante wählen und `<F4>` drücken. Zusatzmenü wird angezeigt.
4.  Menü `Kisten > Kiste abbuchen` wählen. Dialog `Achtung` wird geöffnet.
5.  Abfrage, ob die Kiste aus dem Lager entfernt werden soll mit [Ja] bestätigen.
6.  Schritte 3 bis 5 für nächste Kiste wiederholen.
7.  Buchung mit [OK] bestätigen. Kisten werden vom Lager abgebucht.

#### Buchung prüfen:
8.  Menü `Infosystem > Buchungsstatus > Ungebucht`: Nicht gebuchte Buchungen.
9.  Menü `Infosystem > Buchungsstatus > Fehler`: Fehlerhafte Buchungen.
10. Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
11. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
12. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
13. Buchungsdaten prüfen.

### Einzelblattkistenlager einbuchen (LA 01-007)

#### Ziel der Handlung
Einzelne Glasblätter in das Einzelblattkistenlager buchen.

#### Voraussetzungen
- Einzelblattkistenlager ist in den Stammdaten angelegt.
- Artikelstammdaten sind vollständig erfasst.
- Je nach Systemkonfiguration müssen die Artikel dem gewählten Haus zugeordnet werden.

#### Zusatzinfo
- Mit `<F5>` aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Strg>` + `<E>` die Einzelblattinformationen bearbeiten.
- Buchungen können im Dialog `Buchungskorrektur` korrigiert werden. ⇨ `Buchungskorrektur buchen`

#### Workflow
1.  Menü `Buchung > Kisteneingang` wählen. Dialog `Kistenlagereingang` wird geöffnet.
2.  Artikel und Einzelblattkistenlager wählen.
3.  Artikelvariante wählen.
4.  Kistenbezeichnung eingeben. Cursor wechselt in die Tabelle zur Erfassung der Einzelblätter in die Spalte `Blatt`.
5.  Daten für einzelne Glasscheibe eingeben.
6.  Schritt 5 so oft wiederholen, bis alle Glasscheiben der Kiste erfasst sind.
7.  Variante fertig erfassen.
8.  Buchung mit [OK] bestätigen. Einzelblätter werden ins Einzelblattkistenlager gebucht.

#### Buchung prüfen:
9.  Menü `Infosystem > Buchungsstatus > Ungebucht`: Nicht gebuchte Buchungen.
10. Menü `Infosystem > Buchungsstatus > Fehler`: Fehlerhafte Buchungen.
11. Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
12. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
13. Buchungsdaten prüfen.

#### Weitere Glasscheiben in bestehende Einzelblattkiste einbuchen:
14. Schritte 1 bis 3 wiederholen.
15. Kiste auswählen.
16. Mit `<Strg>` + `<E>` in die Tabelle zur Erfassung der Einzelblätter wechseln.
17. Mit `<F6>` neue Blattnummer anlegen.
18. Schritte 5 bis 13 ausführen.

### Einzelblattkistenlager ausbuchen (LA 01-008)

#### Ziel der Handlung
Einzelblattkiste auflösen und Glasblätter der Einzelblattkiste auf ein anderes Lager buchen.

#### Voraussetzungen
- Einzelblattkistenlager ist in den Stammdaten angelegt.
- Artikelstammdaten sind vollständig erfasst.
- Benötigte Menge an Glasblättern befinden sich auf Lager.

#### Zusatzinfo
- Mit `<F5>` aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Strg>` + `<E>` die Einzelblattinformationen bearbeiten.
- Buchungen können im Dialog `Buchungskorrektur` korrigiert werden. ⇨ `Buchungskorrektur buchen`

#### Workflow
1.  Menü `Buchung > Kistenausgang` wählen. Dialog `Kistenlagerausgang` wird geöffnet.
2.  Artikel und Einzelblattkistenlager wählen.
3.  Variante wählen.
4.  Mit `<Strg>` + `<E>` in die Einzelblattinformationen wechseln.
5.  Mit `<F7>` einzelne Positionen löschen. Ausgewähltes Blatt wird aus der Einzelblattkiste gelöscht. Wenn das letzte verbliebene Blatt der Einzelblattkiste gelöscht wird, wird die Einzelblattkiste automatisch gelöscht.
6.  Mit [OK] führen Sie die Buchung aus.

#### Buchung prüfen:
7.  Menü `Infosystem > Buchungsstatus > Ungebucht`: Nicht gebuchte Buchungen.
8.  Menü `Infosystem > Buchungsstatus > Fehler`: Fehlerhafte Buchungen.
9.  Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
10. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
11. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
12. Buchungsdaten prüfen.

### Gestelllagereingang buchen (LA 01-009)

#### Ziel der Handlung
Artikel auf Gestellen in ein Gestelllager buchen.

#### Voraussetzungen
- Gestelllager ist in den Stammdaten angelegt.
- Artikelstammdaten sind vollständig erfasst.
- Je nach Systemkonfiguration müssen die Artikel dem gewählten Haus zugeordnet werden.
- Fächer müssen als Erfassungsstellen aus dem Produktionssystem an A+W Enterprise übergeben werden.

#### Zusatzinfo
- Buchungen können im Dialog `Buchungskorrektur` korrigiert werden. ⇨ `Buchungskorrektur buchen`

#### Workflow
1.  Menü `Buchung > Gestelleingang` wählen. Dialog `Gestelllagereingang` wird geöffnet.
2.  Entweder Artikel und Gestelllager oder das Gestell wählen.
3.  Artikelvariante wählen.
4.  Gestell wählen oder neues Gestell anlegen.
5.  Fach für das Gestell wählen.
6.  Buchungsmenge der Variante in Mengeneinheit eingeben.
7.  Schritte 3 und 4 für weitere Artikelvarianten wiederholen.
8.  Buchung mit [OK] bestätigen. Artikel werden in das Gestelllager eingebucht.

#### Buchung prüfen:
9.  Menü `Infosystem > Buchungsstatus > Ungebucht`: Nicht gebuchte Buchungen.
10. Menü `Infosystem > Buchungsstatus > Fehler`: Fehlerhafte Buchungen.
11. Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
12. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
13. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
14. Buchungsdaten prüfen.

### Gestelle auftragsbezogen ausbuchen (LA 01-010)

#### Ziel der Handlung
Auftragsbezogene Lagerabgänge im Gestelllager buchen.

#### Voraussetzungen
- Gestelllager ist in den Stammdaten angelegt.
- Artikelstammdaten sind vollständig erfasst.
- Gestell mit den entsprechenden Artikelvarianten befindet sich auf Lager.

#### Zusatzinfo
- Mit `<F2>` zwischen dem Register `Auftragsbezogen` und `Umbuchung` wechseln.
- Mit `<Shift>` + `<F8>` eine Position auflösen und in ein anderes Lager buchen.
- Buchungen können im Dialog `Buchungskorrektur` korrigiert werden. ⇨ `Buchungskorrektur buchen`

#### Workflow
1.  Menü `Buchung > Gestellausgang` wählen. Dialog `Gestelllagerausgang` wird geöffnet.
2.  Entweder Artikel und Gestelllager wählen oder das Gestell.
3.  Register `Auftragsbezogen` wählen.
4.  Variante auf dem Gestell wählen.
5.  Buchungsmenge der Variante in Mengeneinheit eingeben.
6.  Auftragsnummer eingeben.
7.  Positionsnummer im Auftrag eingeben.
8.  Schritte 4 bis 7 für weitere auftragsbezogene Buchungen wiederholen.
9.  Buchung mit [OK] bestätigen. Artikel werden vom Gestelllager abgebucht.

#### Buchung prüfen:
10. Menü `Infosystem > Buchungsstatus > Ungebucht`: Nicht gebuchte Buchungen.
11. Menü `Infosystem > Buchungsstatus > Fehler`: Fehlerhafte Buchungen.
12. Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
13. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
14. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
15. Buchungsdaten prüfen.

### Gestelllager Artikel umbuchen (LA 01-011)

#### Ziel der Handlung
Artikelvarianten auf ein neues Gestell bzw. neues Fach umbuchen.

#### Voraussetzungen
- Gestelllager ist in den Stammdaten angelegt.
- Artikelstammdaten sind vollständig erfasst.
- Gestell mit den entsprechenden Artikelvarianten befindet sich auf Lager.

#### Zusatzinfo
- Mit `<F2>` zwischen dem Register `Auftragsbezogen` und `Umbuchung` wechseln.
- Mit `<Shift>` + `<F8>` eine Position auflösen und in ein anderes Lager buchen.
- Buchungen können im Dialog `Buchungskorrektur` korrigiert werden. ⇨ `Buchungskorrektur buchen`

#### Workflow
1.  Menü `Buchung > Gestellausgang` wählen. Dialog `Gestelllagerausgang` wird geöffnet.
2.  Entweder Artikel und Gestelllager wählen oder das Gestell.
3.  Register `Umbuchung` wählen.
4.  Variante auf dem Gestell wählen.
5.  Buchungsmenge der Variante in Mengeneinheit eingeben.
6.  Neues Gestell eingeben.
7.  Neues Fach eingeben.
8.  Schritte 4 bis 7 für weitere Umbuchungen wiederholen.
9.  Buchung mit [OK] bestätigen. Artikel werden vom Gestelllager abgebucht.

#### Buchung prüfen:
10. Menü `Infosystem > Buchungsstatus > Ungebucht`: Nicht gebuchte Buchungen.
11. Menü `Infosystem > Buchungsstatus > Fehler`: Fehlerhafte Buchungen.
12. Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
13. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
14. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
15. Buchungsdaten prüfen.

### Auftragsbezogene Ausgänge buchen (LA 01-012)

#### Ziel der Handlung
Auftragsbezogene Lagerabgänge manuell buchen.

#### Voraussetzungen
- Bestandsänderung des Artikels im Artikelstamm ist als manuelle Buchung definiert worden.
- Lager ist in den Stammdaten angelegt.
- Artikelstammdaten sind vollständig erfasst.
- Benötigte Menge an Artikeln befinden sich auf Lager.

#### Zusatzinfo
- Mit `<F2>` die Spalte Termin für den Liefertermin der Position anzeigen.
- Mit `<F3>` die Buchung auslösen.
- Buchungen können im Dialog `Buchungskorrektur` korrigiert werden. ⇨ `Buchungskorrektur buchen`

#### Workflow
1.  Menü `Buchung > Ausgang (Auftragsbezogen)` wählen. Dialog `Lagerausgang (Auftragsbezogen)` wird geöffnet.
2.  Auftrag wählen. Positionen des Auftrags werden angezeigt.
3.  Position des Auftrags zum Ausbuchen wählen.
4.  Stückzahl des Artikels eingeben.
5.  Schritt 3 und 4 für weitere auftragsbezogene Buchungen wiederholen.
6.  Buchung mit `<F3>` auslösen. Auftragsbezogene Artikel werden vom Lager abgebucht.

#### Buchung prüfen:
7.  Menü `Infosystem > Buchungsstatus > Ungebucht`: Nicht gebuchte Buchungen.
8.  Menü `Infosystem > Buchungsstatus > Fehler`: Fehlerhafte Buchungen.
9.  Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
10. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
11. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
12. Buchungsdaten prüfen.

### Stapellagereingang buchen (LA 01-013)

#### Ziel der Handlung
Neue Stapel im Stapellagereingang buchen.

#### Voraussetzungen
- Stapellager ist in den Stammdaten angelegt.
- Artikelstammdaten sind vollständig erfasst.
- Je nach Systemkonfiguration müssen die Artikel dem gewählten Haus zugeordnet werden.

#### Zusatzinfo
- Mit `<Shift>` + `<F8>` vom System eine neue Stapelnummer vergeben lassen.
- Mit `<Strg>` + `<F12>` den ausgewählten Stapel einbuchen.
- Buchungen können im Dialog `Buchungskorrektur` korrigiert werden. ⇨ `Buchungskorrektur buchen`

#### Workflow
1.  Menü `Buchung > Stapeleingang` wählen. Dialog `Stapellagereingang` wird geöffnet.
2.  Stapellager und Lieferant wählen.
3.  Mit `<Shift>` + `<F8>` eine neue Stapelnummer anlegen.
4.  Artikelvariante, Artikelmenge und Einkaufspreis pro Stück oder pro Mengeneinheit eingeben. Gesamtpreis der Position wird angezeigt. Detailangaben der Position werden im Fußbereich angezeigt.
5.  Schritte 3 und 4 für nächsten Stapel wiederholen.
6.  Buchung mit `<Ende>` bestätigen. Stapel werden in das Stapellager eingebucht.

#### Buchung prüfen:
7.  Menü `Infosystem > Buchungsstatus > Ungebucht`: Nicht gebuchte Buchungen.
8.  Menü `Infosystem > Buchungsstatus > Fehler`: Fehlerhafte Buchungen.
9.  Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
10. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
11. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
12. Buchungsdaten prüfen.

### Änderung im Stapellager buchen (LA 01-014)

#### Ziel der Handlung
- Artikel auf bestehende Stapel buchen.
- Stapel auflösen und Artikel aus dem Stapellager buchen.

#### Voraussetzungen
- Stapellager ist in den Stammdaten angelegt.
- Artikelstammdaten sind vollständig erfasst.
- Eingangsbuchung für ausgewählte Artikel in Stapeln ist bereits erfolgt.

#### Zusatzinfo
- Mit `<Strg>` + `<F8>` den ausgewählten Stapel auflösen und die Artikel des Stapels auf ein anderes Lager buchen.
- Mit `<Strg>` + `<F12>` den ausgewählten Stapel ausbuchen.
- Buchungen können im Dialog `Buchungskorrektur` korrigiert werden. ⇨ `Buchungskorrektur buchen`

#### Workflow

**Artikel auf bestehenden Stapel buchen:**
1.  Menü `Buchung > Stapeländerung` wählen. Dialog `Stapellageränderung` wird geöffnet.
2.  Filterkriterien eingeben. Vorhandene Stapel werden angezeigt.
3.  Stapel wählen und neue Gesamtmenge im Feld `Anzahl` eingeben.
4.  Buchung mit `<Ende>` bestätigen. Stapel wird auf die eingegebene Menge gesetzt.

**Artikel aus dem Stapellager buchen:**
5.  Schritte 1 bis 2 ausführen.
6.  Stapel wählen und Menge für die Buchung eingeben.
7.  Mit `<Strg>` + `<F8>` Spalte `Ziellager` einblenden.
8.  Neues Lager des Stapels eingeben.
9.  Mit `<Strg>` + `<F12>` Stapel auflösen.
10. Abfrage zur Stapelausbuchung mit [Ja] bestätigen. Artikel des Stapels werden in das Ziellager gebucht.

#### Buchung prüfen:
11. Menü `Infosystem > Buchungsstatus > Ungebucht`: Nicht gebuchte Buchungen.
12. Menü `Infosystem > Buchungsstatus > Fehler`: Fehlerhafte Buchungen.
13. Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
14. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
15. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
16. Buchungsdaten prüfen.

### Buchungskorrektur buchen (LA 01-015)

#### Ziel der Handlung
Buchungen im Lager korrigieren.

#### Voraussetzungen
- Lagerdaten sind durch das Lagerbuchungssystem angelegt worden.

#### Zusatzinfo
- Mit `<F5>` zwischen dem Dialog `Übersicht` und `Detailansicht` der ausgewählten Position wechseln.
- Mit `<Shift>` + `<F12>` für den aktuellen Buchungssatz ein neues Datum eingeben.

#### Workflow
1.  Menü `Buchung > Korrektur` wählen. Dialog `Buchungskorrektur` wird geöffnet.
2.  Filterkriterien eingeben. Trefferliste der Suche wird angezeigt.
3.  Mengen/Anzahl und / oder Preis in den Spalten korrigieren.
4.  Mit `<F5>` die Detailansicht des ausgewählten Datensatzes öffnen.
5.  Buchungskorrektur mit `<Ende>` bestätigen. Menge / Anzahl und / oder der Preis werden korrigiert und gebucht.

#### Buchungen prüfen:
6.  Menü `Infosystem > Buchungsstatus > Ungebucht`: Nicht gebuchte Buchungen.
7.  Menü `Infosystem > Buchungsstatus > Fehler`: Fehlerhafte Buchungen.
8.  Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
9.  Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
10. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
11. Buchungsdaten prüfen.

## Inventurverwaltung

| Help Card | Themen |
| :--- | :--- |
| Inventur im Lager durchführen | Inventur eines Lagers durchführen. |

### Inventur im Lager durchführen (IV 01-001)

#### Ziel der Handlung
Inventur eines Lagers durchführen.

#### Voraussetzungen
- Die Inventur eines Lagers kann nur durchgeführt werden, wenn seit der letzten Inventur mindestens eine Ausgangsbuchung oder eine Eingangsbuchung ausgeführt wurde.

#### Zusatzinfo
- Inventuren für die anderen Lagerarten werden auf die gleiche Weise in folgenden Dialogen durchgeführt: `Inventur > Kistenlager, Fachlager, Stapellager, Gestelllager`.
- Zur Inventur freigeschaltete Lagernummern werden vom System mit einem negativen Vorzeichen gekennzeichnet.
- Eine Inventur ist immer nur für ein Lager möglich (von Lager = bis Lager). Wenn ein Wertebereich eingegeben wird, verzweigt das Programm in den Bewertungsmodus.

#### Workflow
1.  Menü `Inventur > Lager` wählen. Dialog `Inventur` wird geöffnet.
2.  Bereichsgrenzen für Artikel wählen in: `von Artikel`, `bis Artikel`.
3.  In beiden Feldern für die Lagernummer dieselbe Lagernummer eines Lagers wählen.
4.  Abfrage zur Freischaltung der Inventur mit [Ja] bestätigen. Standardlager ist zur Inventur freigeschaltet.
5.  Ist-Bestand beim Bedarf pro Artikel bzw. Artikelvariante korrigieren.
6.  Mit `<Shift>` + `<F8>` Inventur abschließen. Inventur wird abgeschlossen.

#### Inventur auf Abschluss prüfen:
7.  Menü `Infosystem > Buchungsstatus > Inventur`. Dialog `Buchungsstatus` wird geöffnet.
8.  Lagernummern für offene Inventuren werden aufgelistet.

## Bewertung

| Help Card | Themen |
| :--- | :--- |
| Bewertung im Lager vornehmen | Bewertung von Artikelpreisen vornehmen. |

### Bewertung im Lager vornehmen (BW 01-001)

#### Ziel der Handlung
Bewertung von Artikelpreisen vornehmen.

#### Voraussetzungen
- Ausgewähltes Lager darf nicht zur Inventur freigeschaltet sein.
- Die Bewertung eines Lagers kann nur durchgeführt werden, wenn seit der letzten Bewertung mindestens eine Ausgangsbuchung oder eine Eingangsbuchung ausgeführt wurde.

#### Zusatzinfo
- Bewertungen für die anderen Lagerarten werden auf die gleiche Weise in folgenden Dialogen durchgeführt: `Bewertung > Kistenlager, Fachlager, Gestelllager, Stapellager`.
- Eine Bewertung kann nur durchgeführt werden, wenn das betreffende Lager zur Inventur / Bewertung freigeschaltet ist. Zur Bewertung freigeschaltete Lagernummern werden vom System mit einem negativen Vorzeichen gekennzeichnet.

#### Workflow
1.  Menü `Bewertung > Lager` wählen. Dialog `Bewertung` wird geöffnet.
2.  Bereichsgrenzen für Artikel wählen in: `von Artikel`, `bis Artikel`.
3.  In beiden Feldern für die Lagernummer dieselbe Lagernummer eines Lagers wählen.
4.  Abfrage zur Vorbereitung der Bewertung mit [Ja] bestätigen. Artikelvarianten des Standardlagers werden aufgelistet.
5.  Gesamtpreis im Feld `Preis` bei Bedarf korrigieren.
6.  Mit `<Shift>` + `<F8>` Bewertung abschließen. Bewertung wird abgeschlossen.

## Infosystem

| Help Card | Themen |
| :--- | :--- |
| Infos zu Artikeln einsehen | Informationen zu Artikeln des Lagers einsehen. |
| Lagerhistorie einsehen | Informationen zu den Buchungen in der Lagerhistorie einsehen. |
| Aufträge / Bestellungen einsehen | Informationen zu auftrags- und bestellbezogenen Buchungen einsehen. |
| Buchungsstatus einsehen | Nicht gebuchte oder fehlerhafte Buchungen einsehen und korrigieren. Übersicht für alle Lager in Inventur aufrufen. |
| Dispositiven Lagerbestand einsehen | Bestellten, verplanten und verfügbaren Lagerbestand einsehen. |
| Bestandsprognose einsehen | Bestandsprognose für verplante Lagerbestände eines Zeitraums einsehen. |

### Infos zu Artikeln einsehen (IS 01-001)

#### Ziel der Handlung
Informationen zu Artikeln des Lagers einsehen.

#### Voraussetzungen
Lagerdaten zu den ausgewählten Suchkriterien müssen im System vorhanden sein.

#### Zusatzinfo
Informationen zu Artikelvarianten, Fächer, Stapeln und Einzelblättern werden in der gleichen Weise in folgenden Dialogen aufgelistet: `Infosystem > Variante, Fach, Gestell, Stapel, Blatt`.

#### Workflow
1.  Menü `Infosystem > Artikel` wählen. Dialog `Info-Lager-Artikel` wird geöffnet.
2.  Ein oder mehrere Filterkriterien eingeben und mit `<F3>` die Suche starten. Trefferliste wird angezeigt.
3.  Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
4.  Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen. Detailansicht wird geöffnet.

### Lagerhistorie einsehen (IS 01-002)

#### Ziel der Handlung
Informationen zu den Buchungen in der Lagerhistorie einsehen.

#### Voraussetzungen
(keine)

#### Zusatzinfo
(keine)

#### Workflow
1.  Menü `Infosystem > Historie` wählen. Dialog `Info-Lager-Historie` wird geöffnet.
2.  Ein oder mehrere Filterkriterien eingeben und mit `<F3>` die Suche starten. Trefferliste wird angezeigt.
3.  Mit `<F5>` die Detailansicht des ausgewählten Datensatzes öffnen. Detailansicht wird geöffnet.

### Aufträge / Bestellungen einsehen (IS 01-003)

#### Ziel der Handlung
Informationen zu auftrags- und bestellbezogenen Buchungen einsehen.

#### Voraussetzungen
Aufträge / Bestellungen enthalten Lagerartikel.

#### Zusatzinfo
(keine)

#### Workflow
1.  Menü `Infosystem > Aufträge/Bestellungen` wählen. Dialog `Aufträge/Bestellungen` wird geöffnet.
2.  Ein oder mehrere Filterkriterien eingeben und mit `<F3>` die Suche starten. Trefferliste wird angezeigt.
3.  Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen. Detailansicht wird geöffnet.

### Buchungsstatus einsehen (IS 01-004)

#### Ziel der Handlung
- Nicht gebuchte oder fehlerhafte Buchungen einsehen und korrigieren.
- Übersicht für alle Lager in Inventur aufrufen.

#### Voraussetzungen
(keine)

#### Zusatzinfo
Informationen zum Buchungsstatus für fehlerhafte Datensätze und für die Inventur werden in der gleichen Weise in folgenden Dialogen aufgelistet: `Infosystem > Buchungsstatus > Fehler, Inventur`.

#### Workflow
1.  Menü `Infosystem > Buchungsstatus > Ungebucht` wählen. Dialog `Buchungsstatus` für ungebuchte Datensätze wird geöffnet.
2.  Mit `<F5>` die Detailansicht des ausgewählten Datensatzes öffnen. Detailansicht wird angezeigt.
3.  Daten korrigieren.
4.  Mit `<Strg>` + `<F8>` nach der Korrektur der Fehlerursache den Fehlerstatus zurücksetzen.
5.  Mit `<Shift>` + `<F8>` den Lagerbucher aktivieren.
6.  Mit `<Ende>` Korrektur speichern. Korrektur wird gespeichert und der Dialog geschlossen.

### Dispositiven Lagerbestand einsehen (IS 01-005)

#### Ziel der Handlung
Bestellten, verplanten und verfügbaren Lagerbestand einsehen.

#### Voraussetzungen
(keine)

#### Zusatzinfo
(keine)

#### Workflow
1.  Menü `Infosystem > Dispositiver Bestand` wählen. Dialog `Dispositiver Bestand` wird geöffnet.
2.  Filterkriterien im Kopfbereich eingeben und bestätigen. Übersicht des Lagerbestands wird angezeigt.

### Bestandsprognose einsehen (IS 01-006)

#### Ziel der Handlung
Bestandsprognose für verplante Lagerbestände eines Zeitraums einsehen.

#### Voraussetzungen
(keine)

#### Zusatzinfo
(keine)

#### Workflow
1.  Menü `Infosystem > Prognose` wählen. Dialog `Bestandsprognose` wird geöffnet.
2.  Filterkriterien im Kopfbereich eingeben und bestätigen. Übersicht der Bestandsprognose wird angezeigt.
3.  Mit `<F5>` die Auftragsnummer oder Bestellnummer des ausgewählten Datensatzes anzeigen lassen.
4.  Mit `<Shift>` + `<F5>` Grafik vom Bestandsverlauf anzeigen lassen.

## Druck

| Help Card | Themen |
| :--- | :--- |
| Kistenetiketten drucken | Kistenetiketten für offene Druckaufträge drucken. |

### Kistenetiketten drucken (DR 01-001)

#### Ziel der Handlung
Kistenetiketten für offene Druckaufträge drucken.

#### Voraussetzungen
(keine)

#### Zusatzinfo
- Im Lagereingang wird für jede Kiste automatisch ein Druckauftrag zum Etikettendruck angelegt.
- Im Dialog `Kistenetiketten drucken` wird in der Spalte ohne Name angezeigt, ob der Druckauftrag zum Etikettendruck freigeschaltet ist oder nicht.

#### Workflow
1.  Menü `Druck > Etiketten` wählen. Dialog `Kistenetiketten drucken` wird geöffnet.
2.  Wenn ein Kistenetikett nicht gedruckt werden soll, muss mit `<Leertaste>` die Kennzeichnung in der Spalte ohne Namen von J auf N umgestellt werden.
3.  Etikettendruck mit `<Shift>` + `<F3>` bestätigen. Etiketten werden gedruckt.

## System

| Help Card | Themen |
| :--- | :--- |
| Lagerprotokoll löschen | Lagerprotokoll im System löschen. |
| Durchschnittspreis korrigieren | Durchschnittspreis für eingekauften Lagerartikel korrigieren. |

### Lagerprotokoll löschen (SY 01-001)

#### Ziel der Handlung
Lagerprotokoll im System löschen.

#### Voraussetzungen
(keine)

#### Zusatzinfo
Nach dem Löschen des Lagerprotokolls werden die entsprechenden Sätze nicht mehr unter `Infosystem > Historie` angezeigt.

#### Workflow
1.  Menü `System > Lagerprotokoll löschen` wählen. Dialog `Lagerprotokoll löschen` wird geöffnet.
2.  Daten eingeben, zu denen das Lagerprotokoll gelöscht werden soll.
3.  Lagerprotokoll mit `<F3>` löschen. Lagerprotokoll wird gelöscht.

### Durchschnittspreis korrigieren (SY 01-002)

#### Ziel der Handlung
Durchschnittspreis für eingekauften Lagerartikel korrigieren.

#### Voraussetzungen
- Artikel ist auf Lager gebucht.

#### Zusatzinfo
(keine)

#### Workflow
1.  Menü `System > Preiskorrektur` wählen. Dialog `Lager-Preiskorrektur` wird geöffnet.
2.  Artikel, Lager, Variante und Farbe wählen. Höchstpreis und Niedrigstpreis wird angezeigt.
3.  Höchstpreis und / oder Niedrigstpreis korrigieren.
4.  Korrektur mit `<F3>` bestätigen. Höchstpreis und oder Niedrigstpreis des Lagerartikels wird für das ausgewählte Lager korrigiert. Durchschnittspreis des Lagerartikels wird für das ausgewählte Lager ermittelt und korrigiert.

# Teil 3: A+W Enterprise Versandsteuerung

## Revisionsübersicht des Moduls

| Datum | Änderung |
| :--- | :--- |
| 04-2022 | Aktualisierung der Softwarereferenz. |
| 01-2017 | Produkt- und Firmennamen angepasst. |
| 02-2014 | Produktnamen aktualisiert. |
| 01-2013 | Layout an CI 2013 angepasst. |
| 11-2012 | Ersterstellung. |

Zu diesem Modul finden Sie folgende Kapitel:
- Tutorial
- Softwarereferenz

## Tutorial: A+W Enterprise Versandsteuerung

### In diesem Kapitel finden Sie folgende Themen:

- Einführung
- Menü-Übersicht
- Allgemeine Bedienschritte
- Versandmodus
- Versand-Explorer
- Verschieben
- Versand vorbereiten
- Gestelle
- Anbindung des A+W Logistics Optimizer
- Zusatzfunktionen
- Servicefunktion

**Inhaltsverzeichnis:**
- Einführung (G-1849)
- Menü-Übersicht (G-1850)
- Allgemeine Bedienschritte (G-1851)
  - Navigieren im Versand (G-1853)
- Versandmodus (G-1855)
- Versand-Explorer (G-1856)
  - Versandsteuerung ohne Explorer (G-1856)
  - Versandsteuerung mit Explorer (G-1858)
- Verschieben (G-1861)
  - Tour verschieben (G-1863)
  - Auftrag verschieben (G-1864)
  - Position verschieben (G-1865)
- Versand vorbereiten (G-1868)
  - Fehlmengekontrolle durchführen (G-1868)
  - Verpackte Menge korrigieren (G-1869)
  - Lieferscheine (G-1870)
  - Ladefolge bearbeiten (G-1871)
- Gestelle (G-1873)
  - Gestellmeldungen aus A+W Production (G-1873)
  - Gestellrückmeldungen aus A+W Production (G-1874)
- Anbindung des A+W Logistics Optimizer (G-1876)
- Zusatzfunktionen (G-1877)
  - Touren-Übersicht (G-1877)
  - Auftragsinformation in der Versandsteuerung (G-1879)
- Servicefunktion (G-1881)
  - Funktionstest (F-Test) starten (G-1881)
  - Funktionstest (F-Test) stoppen (G-1881)

### Einführung

Das Tutorial zum Modul Versandsteuerung führt Sie in A+W Enterprise - Logistik. Das Tutorial baut auf den Kenntnissen von Glasproduktions- Workflow und Kenntnisse anderen Modulen A+W Enterprises.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.
> Im Weiteren sind die Programm-Schritte nur in bestimmten Reihenfolge sinnvoll. So können z.B., nur Ware auf LKW verladen werden, die auch fertigproduziert sind. So sind die Funktionen ebenfalls von der logistischen Reihenfolge zugänglich sind.

#### Themenblöcke
In diesem Tutorial finden Sie folgende Themenblöcke:
- "Menü-Übersicht" auf Seite G-1850
- "Allgemeine Bedienschritte" auf Seite G-1851
- "Versand-Explorer" auf Seite G-1856
- "Servicefunktion" auf Seite G-1881

#### Vorausgesetzte Kenntnisse
Das Tutorial richtet sich an Anwender, die in A+W Enterprise in dem Logistikbereich tätig und dort mit allen Alltagsaufgaben vertraut sind.

### Menü-Übersicht

Die Versandsteuerung ist ein eigenständiges Modul. So können Sie die Versandsteuerung entweder aus dem A+W Enterprise starten oder das Modul direkt beim Verbindungsaufbau auswählen.

*Abb. G-1: Start von Versandmodul*

Im Modul Versansteuerung finden Sie zwei wichtige Menüs, die über alle Datenebenen hinweg verfügbar sind: `<Shift>` + `<F4>` und `<F4>`.

*Abb. G-2: Menüs <Shift> + <F4> und <F4> im Versand*

Ausführliche Beschreibung entnehmen Sie der Softwarereferenz zur Versandsteuerung:
- Softwarereferenz, "Zusatzmenü" auf Seite G-1900
- Softwarereferenz, "Infomenü" auf Seite G-1903

### Allgemeine Bedienschritte

Die Versandsteuerung in A+W Enterprise stellt die Daten in mehreren Ebenen zusammen:
- zu einem Liefertermin
- zu einer Tour
- zu einem Auftrag
- zu bestimmten Positionen.

In die gewünschte Ebene gelangen Sie mit `<F5>` bzw. über die Schaltfläche [Details]. Zurück in die ursprüngliche Ebene gehen Sie mit `<Ende>`.

Wenn Sie gestellweise Warenauslieferung betreiben werden Sie auch eine Gestellsicht haben.

Im Allgemeinen gibt es vorwiegend folgende Unterscheidung:
- **Die Route** ist eine festgelegte Fahrstrecke, die an bestimmten Tagen befahren wird, z. B. die Route 300 von Frankfurt nach München wird jeweils montags und donnerstags gefahren.
- **Die Tour** ist die zu fahrende Strecke an einem bestimmten Liefertermin, z. B. die Tour auf der Route 300 liefert die Kundenaufträge am Donnerstag, dem 28.04.16 aus.

### Glossar

| Begriff | Erklärung |
| :--- | :--- |
| **Versandmodus/Modus** | Je nach dem welche Vorgänge (Auftrag/Bestellung) und wie im Versand behandelt werden, sind folgende Einstellungen möglich: "Versandmodus" auf Seite G-1855 |
| **Versand-Explorer** | Windows-ähnliche Darstellung aller in der Versandsteuerung verfügbaren Lieferungen: Softwarereferenz, "Versand-Explorer" auf Seite G-1893 |
| **Datenebene** | Oberbegriff für alle Lieferungen, die auf das gewählte Datum fallen: Tourebene, Auftragsebene, Positionsebene. Das Wechsel in jeweils untere Ebene erfolgt mit `<F5>`, der Wechsel in die übergeordnete Ebene erfolgt mit `<Ende>` |
| **Tourebene** | Kumulierte Anzeige aller verfügbaren Lieferungen pro Versandtermin. Softwarereferenz, "Register - TourenInfo" auf Seite G-1907 |
| **Auftragsebene** | Kumulierte Anzeige aller verfügbaren Lieferungen pro Versandtermin und Route. Softwarereferenz, "Register - AuftragsInfo" auf Seite G-1917 |
| **Positionsebene** | Kumulierte Anzeige aller verfügbaren Lieferungen pro Versandtermin, Route und Auftrag bzw. Bestellung. Softwarereferenz, "Register - PositionsInfo I" auf Seite G-1935 |

### Navigieren im Versand

Mit `<F2>` wechseln Sie innerhalb einer Datenebene zwischen den Register der aktuellen Ebene. Die folgenden Ebenen verfügen über mehrere Register:
- Tourenebene
- Auftragsebene
- Positionsebene

Nicht alle Register sind in der jeweiligen Kundenkonfiguration verfügbar. Die Gestell- und Optimierungs-Register werden dynamisch bei der entsprechenden Konfiguration eingeblendet.

Mit `<F5>` wechseln Sie von oberer Datenebene in die tiefere Ebene. Mit `<Ende>` wechseln Sie wieder in die übergeordnete Ebene. Ein Überspringen einer Datenebene ist nicht möglich.

Das Navigieren wird anhand des folgenden Workflows erklärt:

**So gelangen Sie in die Ansicht Positionen:**
1.  Starten Sie das Modul Versandsteuerung.
2.  Geben Sie ein Lieferdatum an. Das Programm prüft, ob zu diesem Datum Touren mit auszuliefernden Aufträgen vorhanden sind. Wenn Sie mit dem Versandexplorer arbeiten, können Sie im Dialogkopf einen Zeitraum von-bis für die gesuchte Liefertermine eingeben. ⇨ Tutorial, "Versand-Explorer" auf Seite G-1856
3.  Über die Schaltfläche [Details] wechseln Sie in die Tourebene.
4.  Wählen Sie eine Tour aus und betätigen Sie die Schaltfläche [Aufträge], um in die Auftragsebene zu wechseln.
5.  Aus der Auftragsebene können Sie über die Schaltfläche [Touren], oder [Explorer] zurück zur Ursprungsebene kehren. Oder... .
6.  Wählen Sie einen Auftrag aus und betätigen Sie die Schaltfläche [Positionen], um in die Positionsebene zu wechseln.
7.  Sie können beliebig die Ansichten wechseln.
8.  Wenn Sie direkt zu einem bestimmten Auftrag gelangen möchten, führen Sie die Anweisungen aus dem folgenden Kapitel aus: ⇨ Tutorial, “Springen zu..." auf Seite G-1854

#### Suchen nach einem Auftrag/nach einer Bestellung

In A+W Enterprise haben Sie die Möglichkeit Ihre Lieferungen (Aufträge bzw. Wareneingänge und -ausgänge) zu suchen.

In Selos (`<F9>`) auf den Vorgangsfelder, wie z. B., Auftrag, Bestellung haben Sie eine erweiterte Suche nach den von Ihnen gewünschten Kriterien. Die erweiterte Suchmöglichkeit ist an vielen aber nicht an allen Stellen im Programm verfügbar. Eine ausführliche Dokumentation können Sie in folgenden Kapiteln nachsehen:
- Verkauf, "Suche Aufträge" auf Seite D-1077
- Verkauf, "Marktpartnersuche" auf Seite D-1091

**So suchen Sie nach einem bestimmten Auftrag**
1.  Starten Sie das Modul Versandsteuerung.
2.  Klicken Sie auf die Schaltfläche [Suchen].
3.  Geben Sie im Feld Auftrag/Bestellung die gewünschte Vorgangsnummer. Wenn Sie die Nummer nicht parat haben, können Sie über erweiterte Selo mit `<F9>` danach suchen.
4.  Lösen Sie die Suche aus.
5.  In dem Dialog Information zu dem Auftrag [Nummer] bekommen Sie den aktuellen Auftragsstatus: ⇨ Softwarereferenz, "Auftragsinfo" auf Seite G-1948
6.  Klicken Sie die Schaltfläche [Springen], lösen Sie nachfolgende Aktion aus.
7.  Sie sind nun in der Positionsebene des ausgewählten Auftrages.

**Springen zu...**
1.  Starten Sie das Modul Versandsteuerung.
2.  Klicken Sie auf die Schaltfläche [Springen].
3.  Im Dialog `Springe zu` können Sie mehrere Auswahlkriterien, wie z. B., Lieferdatum, Haus, Route, Auftrag eingeben. Mindestens ein Suchfeld muss zwingend gefüllt werden. In der Regel ist das `Lieferdatum` mit dem aktuellen Datum vorbelegt ist. Das Lieferdatum kann geändert werden. Bleibt das `Lieferdatum` leer, wird in der Suche trotzdem von heutigem Datum ausgegangen. Beim [Auslösen] wird im Programm ein SQL-Statement mit genau diesen where-Bedienungen ausgeführt. Geben Ihre Kriterien keinen Treffer, erscheint die Meldung "Keine Daten gefunden". Je nach dem, welche Kriterien Sie eingeben, wird das Programm Sie unterschiedlich weiterführen:
    - Bei der Eingabe des Lieferdatums startet TourenInfo.
    - Bei der Eingabe des Lieferdatums und der Route startet Auftragsinfo
    - Bei der Eingabe des Lieferdatums, der Route und der Auftragsnummer startet PositionsInfo.

### Versandmodus

Versandmodus bestimmt die Art und Weise, wie die Vorgänge (Aufträge und Bestellungen, bzw. bestellte Bearbeitungen) in der Versandsteuerung eingebucht werden.

A+W Enterprise unterscheidet folgende Konfigurationen:
- die alte Logik für die Auftrags-Logistik. Diese Option gilt als Standard und muss nicht explizit konfiguriert werden, sofern Sie mit dem Modul Versand arbeiten. ⇨ "VA" auf Seite G-1855
- (1) separat konfigurierbare Möglichkeit, eigene Wareneingänge in der Versandsteuerung zu verwalten. Dabei werden alle Bestellungen im Versand als Einkaufs-Abholung dargestellt. ⇨ "EK1" auf Seite G-1855
- (2) separat konfigurierbare Möglichkeit, eigene Wareneingänge und die Warenausgänge in der Versandsteuerung zu verwalten. es werden alle Bestellungen als EK-Auslieferung und EK-Abholung dargestellt ⇨ "EK2" auf Seite G-1855
- wie (1), es werden jedoch nur die Bestellungen mit bestellten Bearbeitungen in der Versandsteuerung behandelt.
- wie (2), es werden jedoch nur die Bestellungen mit bestellten Bearbeitungen in der Versandsteuerung behandelt.

Unter dem Termin zur Warenlieferungen zum Lieferant, der aus der Produktion gemeldet wird, und der entsprechenden Bestellnummer kann der Vorgang im Versand gefunden werden.

#### VA
Versandmodus VA bezeichnet das Handling von Verkaufsaufträgen in der Versandsteuerung.

#### EK1
Versandmodus EK1 bezeichnet das Handling von Einkaufsvorgängen, genau genommen, Wareneingänge in der Versandsteuerung.

#### EK2
Versandmodus EK2 bezeichnet das Handling von Einkaufsvorgängen, genau genommen, Warenausgängen in der Versandsteuerung.

### Versand-Explorer

#### Lernziele
- Touren zu einem Zeitraum suchen
- Aufträge nach Lieferdatum suchen mit und ohne Versand-Explorer.
- Information über die auszuliefernde Positionen einholen.

#### Nutzen
- Die Nutzung des Explorers in der Versandsteuerung bringt größere Überblick über die gefahrene Routen und deren Auslastung, gibt die Möglichkeit einfach zwischen Lieferterminen zu wechseln.
- Versand-Explorer ist standardmäßig im System konfiguriert werden. Wünschen Sie die Bedienung ohne Explorer, sprechen Sie bitte den zuständigen A+W - Mitarbeiter.

#### Versandsteuerung ohne Explorer

Der wesentliche Unterschied beim Arbeiten mit und ohne Versand-Explorer besteht in der Auswahlfelder (A) und im Datenbereich (B).

*Abb. G-3: Start-Dialog (ohne Explorer)*

- A: Auswahlfelder ohne VS-Explorer
- B: Datenbereich
- C: Verfügbare Schaltflächen

Die Felder `Versand-Modus` (ohne Bezeichnung), `Haus` und `Versandgruppe` (nicht im Bild) sind jeweils nur bei entsprechenden Konfiguration betretbar und änderbar.

> **Versand-Modus**
> Beim Versandmodus kann zwischen Verkaufs- (Aufträge) und Einkaufsvorgänge (Wareneingang und -ausgang) unterschieden werden. Diese Möglichkeit besteht, wenn man mit der verlängerten Werkbank arbeitet. Bitte sprechen Sie bei bestehende Interesse den zuständigen A+W - Mitarbeiter an.
> ⇨ Tutorial, "Menü-Übersicht" auf Seite G-1850

> **Haus-Auswahl**
> Bei der Mehrmandanten-Systemkonfiguration können Sie auch in der Versandsteuerung die Vorgänge für unterschiedliche Produktionshäuser verwalten. Bitte sprechen Sie bei bestehende Interesse den zuständigen A+W Mitarbeiter an.

> **Versandgruppen**
> Wenn die bearbeitende Lieferungen noch weiter differenziert werden sollen, können Sie auch mit vordefinieren Versandgruppen arbeiten. Bitte sprechen Sie bei bestehende Interesse den zuständigen A+W - Mitarbeiter an.
> ⇨ Stammdaten: Softwarereferenz, "Versandgruppen" auf Seite B-269

Für das Arbeiten im Versand werden immer die gültige Daten vorausgesetzt. D. h., zum ausgewählten Liefertermin sind Vorgänge auf die Touren geplant sind.

**So suchen Sie Lieferung (en) zu einem Datum**
1.  Starten Sie das Modul Versandsteuerung.
2.  Geben Sie im Feld `Lieferdatum` das gewünschte Datum ein. Das Feld ist beim Programmstart mit jeweils aktuellem Datum vorbelegt. Das Datum könne Sie ändern. Wenn Sie schnell das heutigen Datum eintippen möchten, geben Sie im Feld einen Punkt [.] ein. Bestätigen mit `<Enter>` Ihre Eingabe
3.  Dialog `Versandsteuerung – TourenInfo` mit der Trefferliste wird geöffnet.
4.  Von hier aus können alle Aktionen gestartet werden, um die Tourdaten zu bearbeiten.
5.  Sie können z.B. Aufträge zur ausgewählte Tour einsehen, indem Sie die Schaltfläche [Aufträge] anklicken. Register `AuftragsInfo` wird geöffnet.
6.  Sie können z. B. Positionen zum ausgewählten Auftrag einsehen, indem Sie die Schaltfläche [Positionen] anklicken. Register `PositionsInfo I` wird geöffnet. Die gewünschte Datenebene erreichen Sie auch per Doppelklick auf Tour oder Auftrag oder mit `<F5>`.
7.  Sie können über jeweilige Schaltfläche ([Touren] oder [Aufträge]) wieder in die vorherige Übersicht zurückkehren.

#### Versandsteuerung mit Explorer

Das Arbeiten mit Versand-Explorer ist seit einige Versionen als Standard eingerichtet worden. In den Auswahlfelder können Sie nach Lieferzeitraum suchen, indem Sie von-bis Lieferdatum eingeben. Wenn Sie in beiden Felder für das gleiche Datum sich entscheiden, starten Sie direkt mit der TourenInfo. Die weitere Arbeit erfolgt so, wie ohne Versand-Explorer.

*Abb. G-4: Start-Dialog mit VS-Explorer*
- A: Auswahlfelder mit VS-Explorer
- B: Datenbereich
- C: Verfügbare Schaltflächen

Die Felder `Versand-Modus` (ohne Bezeichnung), `Haus` und `Versandgruppe` (nicht im Bild) sind jeweils nur bei entsprechenden Konfiguration betretbar und änderbar. Diese Module sind unabhängig vom Versand-Explorer. Die Hinweise darüber findet Sie im Kapitel: ⇨ Tutorial, "Versandsteuerung ohne Explorer" auf Seite G-1856

*Abb. G-5: Versand-Explorer*

In dieser Darstellung sehen Sie auf der linken Dialoghälfte die explorerähnliche Darstellung allen gefundenen Lieferungen für den gewünschten Lieferzeitraum. Auf der rechten Dialoghälfte befindet sich kurze Übersicht zu der Markierung im Explorer. Je nach dem, welches Feld Sie im Explorer mit Maus oder Cursor markieren, wird die Übersicht auf der rechte Seite dynamisch aufgebaut. Z. B., wenn Sie den Auftrag `5002099` markieren (blauer Rahmen im Explorer), werden in der Übersicht alle Positionen dieses Auftrages aufgelistet.

Mit `<Details>` starten Sie die ausführliche Übersicht, z. B. `PositionsInfo I`.

**So bewegen Sie im Versand-Explorer**
1.  Starten Sie das Modul Versandsteuerung.
2.  Geben Sie in den Felder (von)Lieferdatum und bis den gewünschten Zeitraum ein.
3.  Bestätigen Sie die Eingabe mit `<Enter>`. Felder Modus, Haus und Versandgruppe sind im folgenden Kapitel beschrieben: ⇨ Tutorial, "Menü-Übersicht" auf Seite G-1850
4.  Alle Tage mit geplanten Touren werden im Versand-Explorer angezeigt. Per Mausklick markieren Sie einen Liefertermin im Explorer. In der Detailsicht auf der rechten Dialogseite werden die Touren des markierten Tages angezeigt.
5.  Ebene aufklappen: Knoten [+] am gesuchten Tag öffnen. Tour in der Explorersicht markieren und [Details] wählen.
6.  Register `TourenInfo` mit den Touren des gewählten Tages wird geöffnet.
7.  Von hier aus können alle Aktionen gestartet werden, um die Tourdaten zu bearbeiten.
8.  Mit [Explorer] zurück in die Explorersicht springen.
9.  Im Explorer können Sie weitere Ebenen aufklappen: Knoten [+] am gesuchten Tag öffnen.
10. Per Mausklick kann eine Tour oder ein Auftrag markiert werden. Detailsicht passt die Anzeige an.
11. Auf den Auftrags- und die Positionsebenen können alle Aktionen gestartet werden, um die Auftrags- bzw. Positionsdaten zu bearbeiten.

**Weitere Optionen im Versand-Explorer**
1.  Starten Sie den Versand-Explorer.
2.  Markieren Sie im Versand-Explorer den gewünschten Liefertag, Tour oder Auftrag.
3.  Klicken Sie die rechte Maustaste an, um das Kontext-Menü aufzurufen. Sie haben nun folgende Möglichkeiten hier:
    - **Kopieren**: Speichert den zuvor markierten Text oder Feldinhalt in die Zwischenablage.
    - **Einfügen**: Fügt den zuvor kopierten Text oder Feldinhalt an die Cursor-Position ein. Die Optionen Kopieren und Einfügen sind nur bedingt im Versand-Explorer möglich.
    - **Details**: Alternativ-Weg, um die Details zur aktuellen Markierung aufzurufen. Die gleiche Option, wie auch die Schaltfläche [Details].
    - **Route ausschneiden**: Speichert die zuvor markierte Tour komplett mit allen Aufträgen in die Zwischenablage.
    - **Route einfügen**: Fügt die zuvor markierte Tour komplett mit allen Aufträgen an die Cursor-Position ein.
4.  Analog zu `Route ausschneiden` bzw. `Route einfügen` sind auch die Optionen `Auftrag` oder `Position ausschneiden` und `einfügen` verfügbar.

> **Explorer-Optionen Ausschneiden und Einfügen**
> Wenn Sie über das Kontext-Menü des Versand-Explorer die Tour/Auftrag/Position ausschneiden und an einer anderen Stelle einfügen, so wird es dabei eine Verschiebung auf Kundenwunsch durchgeführt, die im Lieferterminänderungs-Protokoll vermerkt wird. Verschiebung über Kontext-Menü ist nicht zu empfehlen, da nur wenige Restriktionen dabei geprüft werden. Die Verschiebung von Touren, Aufträgen und Positionen über das Kontext-Menü löst z. B. keine Statusbuchungen im Auftrag aus. Diese Form der Verschiebung ist nur sinnvoll, wenn nur ein einziger Mitarbeiter mit der Versandplanung beauftragt ist.
> Sie können stattdessen die Funktion Verschieben benutzen:
> ⇨ Tutorial, "Verschieben" auf Seite G-1861

### Verschieben

Bei Verschiebung in der Versandplanung können einzelne (Teil-) Positionen, (Teil-) Aufträge, komplette Gestelle, oder Routen verschoben werden. Die Verschiebung kann aus verschiedenen Gründen erfolgen.

*Abb. G-6: Dialoge zur Dateneingaben bei der Verschiebung*

- A: Auswahldialog bei Verschiebung mehrere Positionen
- B: Eingabefeld bei Verschiebung einer Teilmenge
- C: Angabefeld für die Anmerkung
- D: Auswahl des Verschiebegrundes
- E: Gestellsicht

| Verschiebegrund | Kurzbeschreibung |
| :--- | :--- |
| **Kundenwunsch** | Die Verschiebung auf Kundenwunsch besteht auf jeder Datenebene. Dabei können Sie auf einen neuen Termin, eine neue Route verschoben werden. Sie können eine gesamte Tour, einzelnen Auftrag verschieben, Zum Verschieben der Teil-Positionsmenge verwenden Sie die Funktion: ⇨ Softwarereferenz, "Verschieben mehrerer Pos. - Auswahl" auf Seite G-1946. Die Begründung geben Sie in dem dafür vorgesehenen Feld. Diese Bemerkung wird in das Änderungsprotokoll übernommen: ⇨ Softwarereferenz, "Lieferterminänderungen" auf Seite G-1997 |
| **Rückstand** | Die Verschiebung als Rückstand erfolgt, wenn nicht alle auszuliefernde Menge zur aktuellen Termin zur Verfügung steht. Es besteht die Möglichkeit, die (Teil-) Auftrags- bzw. Positionsmenge manuell als Rückstand auf einen anderen Liefertermin bzw. andere Route zu verschieben, oder die fehlende Menge wird innerhalb der Fehlmengenkontrolle automatisch verschoben. ⇨ "Fehlmengekontrolle durchführen" auf Seite G-1868 |
| **Kundenstorno** | Die Verschiebung als Kundenstorno löst eine Löschung der Auftrags- bzw. Positionsmenge in der Versandsteuerung aus. Beim Stornieren einer Teilmenge wird die Abrufmenge und die geplante Menge um die stornierte Stückzahl verringert. Der Auftrag bzw. die Position bleibt jedoch im Verkauf bestehen und wird unter Umständen der Faktura vorliegen. Die eingetragene Anmerkung ist in der Auftragsstatus zu sehen. Technische Info: DB-Feld: `kaufstat.status=501`, `kaufstat.infotxt` |
| **Betriebsstorno** | Die Verschiebung als Betriebsstorno muss im System explizit konfiguriert werden. Bei dieser Konfiguration wird beim Storno zwischen Kundenstorno und Betriebsstorno unterschieden. Bei Betriebsstorno wird nur die geplante Menge verringert. |
| **Tourenplanung** | Diese Möglichkeit zum Verschieben besteht nur auf der Tourenebene und muss im System separat konfiguriert werden. Dabei werden die Daten analog zum Kundenwunsch behandelt. |

#### Tour verschieben

Die Voraussetzung für eine Verschiebung einer kompletten Tour setzt voraus, dass die neue Tour in den Stammdaten hinterlegt ist und die Anfahrtstage beim neuen Termin berücksichtig wird.

**Lernziele**
- Tour auf ein anderes Lieferdatum verschieben.
- Tour auf eine andere Route verschieben.

**Nutzen**
- Das Verschieben in der Versandsteuerung ist ein wichtiger Teil der logistischen Arbeit. Jede Lieferung muss im System leicht auffindbar sein und alle wichtigen Lieferdaten müssen jederzeit abrufbar sein.
- Beim Verschieben einer gesamt Tour kann diese komplett gesperrt werden.
- Viele Funktionen und die Auswahlfelder sind so konfigurierbar, dass die Aktionen mit wenigen Handgriffen durchgeführt werden können, sprechen Sie dazu bitte den zuständigen A+W - Mitarbeiter an.

**So verschieben Sie eine Tour**
1.  Register `TourenInfo`: Tour markieren > [Verschieben]. Dialog `Verschiebung (Versand)` wird geöffnet.
2.  Begründung für die Verschiebung mit `<Leertaste>` wählen und ggf. eine Anmerkung eintragen.
3.  Feld `Auf Tourtag`: Lieferdatum eintragen. Wenn das neue Datum kein gültiger Routentag ist, kann die Tour nicht verschoben werden. Wenn ein Tourplan erstellt ist: in Feld `Auf Tourtag` `<F9>` drücken und Tour auswählen.
4.  Verschiebung mit [Start] auslösen. Die Tour wird komplett auf das neue Lieferdatum verschoben. Im Register `TourenInfo` wird sie zu dem ursprünglichen Termin nicht mehr angezeigt.
5.  Verschiebung prüfen: Tourensuche mit neuem Lieferdatum starten.
6.  Alternativ: Tour für das gleiche Datum auf andere Route verschieben:
7.  Feld `Auf Tourtag`: Lieferdatum prüfen.
8.  Feld `Route`: neue Route eintragen. Wenn das Lieferdatum kein Routentag ist, kann die Tour nicht verschoben werden.
9.  Verschiebung mit [Start] auslösen. Die Tour wird komplett auf die neue Route verschoben. Wenn das Lieferdatum beibehalten wurde, wird die Tour mit der neuen Routennummer angezeigt.

#### Auftrag verschieben

**Lernziele**
- Auftrag auf ein anderes Lieferdatum verschieben.
- Auftrag auf eine andere Route verschieben.

**Nutzen**
- Das Verschieben in der Versandsteuerung ist ein wichtiger Teil der logistischen Arbeit. In der Regel ergibt sich die Notwendigkeit, einen Auftrag auf Kundenwunsch zu verschieben. Andere Aufträge auf der Tour können weiterhin für den Versand vorbereitet werden.
- Viele Funktionen und die Auswahlfelder sind so konfigurierbar, dass die Aktionen mit wenigen Handgriffen durchgeführt werden können, sprechen Sie dazu bitte den zuständigen A+W - Mitarbeiter an.

**So verschieben Sie einen Auftrag**
1.  Register `TourenInfo` > Auftragsebene öffnen.
2.  Auftrag markieren > [Verschieben]. Dialog `Verschiebung (Versand)` wird geöffnet.
3.  Begründung für die Verschiebung mit `<Leertaste>` wählen und ggf. eine Anmerkung eintragen. Siehe dazu die Zusatzinfo.
4.  Feld `Auf Tourtag`: Lieferdatum ändern.
5.  Feld `Route`: ggf. neue Route eintragen. Wenn ein Tourplan erstellt ist: in Feld `Auf Tourtag` `<F9>` drücken und Tour auswählen.
6.  Verschiebung mit [Start] auslösen. Der Auftrag wird komplett auf das neue Lieferdatum und/oder die neue Tour verschoben.

**Mehrere Aufträge der Tour verschieben:**
1.  Register `Zusatzinfo` > Checkbox `versch` bei allen Aufträgen markieren, die verschoben werden sollen.
2.  Lieferdatum und Route eintragen. Wenn das Lieferdatum kein Routentag ist, kann der Auftrag nicht verschoben werden.
3.  Feld `Mehrere Sätze verschieben`: J (ja) wählen.
4.  Verschiebung mit [Start] auslösen.
5.  Ggf. die Abfrage mit [Ja] beantworten. Die Aufträge werden verschoben.
6.  Verschiebung prüfen: Tourensuche mit neuem Lieferdatum starten.

#### Position verschieben

**Lernziele**
- Position auf ein anderes Lieferdatum verschieben.
- Position auf eine andere Route verschieben.

**Nutzen**
- Die Verschiebung der Versandsteuerung auf Positionsebene hat den Vorteil, dass Teillieferungen möglich sind. Teillieferungen kommen häufig vor, wenn eine Position nicht vollständig fertiggestellt wurde oder Lieferschwierigkeiten beim Zwischenlieferanten bestehen.
- Viele Funktionen und die Auswahlfelder sind so konfigurierbar, dass die Aktionen mit wenigen Handgriffen durchgeführt werden können, sprechen Sie dazu bitte den zuständigen A+W - Mitarbeiter an.

**So verschieben Sie eine Position**
1.  Register `TourenInfo` > Auftragsebene > Positionsebene öffnen.
2.  Position markieren > [Verschieben]. Dialog `Verschiebung (Versand)` wird geöffnet.
3.  Begründung für die Verschiebung mit `<Leertaste>` wählen und ggf. eine Anmerkung eintragen. Siehe dazu die Zusatzinfo.
4.  Feld `Auf Tourtag`: Lieferdatum ändern.
5.  Feld `Route`: Route prüfen.
6.  Gesamte Position auf die neue Tour mit [Start] verschieben. Gesamte Position wird auf die neue Tour verschoben.
7.  Verschiebung prüfen: Tourensuche mit neuem Lieferdatum starten.
8.  Position für das gleiche Datum auf andere Route verschieben:
9.  Feld `Auf Tourtag`: Lieferdatum prüfen.
10. Feld `Route`: Route eintragen. Wenn das Lieferdatum kein Routentag ist, kann die Position nicht verschoben werden.
11. Verschiebung mit [Start] auslösen. Die Position wird komplett auf die neue Route verschoben. Wenn das Lieferdatum beibehalten wurde:
    - Die Position wird mit der Original-Auftragsnummer mit der neuen Routennummer angezeigt.
    - Die Position wird mit der Original-Auftragsnummer in eine bestehende Tour verschoben.
    Verschiebung prüfen: Tourensuche mit neuem Lieferdatum starten.

#### Mehrere Positionen verschieben

**So verschieben Sie mehrere Positionen**
1.  Register `TourenInfo` zum Lieferdatum vom Vortag anzeigen.
2.  Dialog zur Verschiebung mit `<Strg>` + `<E>` öffnen. Dialog `Verschiebung für` wird geöffnet.
3.  Aktuelles Lieferdatum prüfen und auf [Auslösen] klicken. Dialog `Verschiebung (Versand)` wird geöffnet.
4.  Ggf. in Spalte `Verschieben` die Stückzahl eintragen.
5.  Checkboxen in Spalte `Buch.` für die Verschiebung markieren. Die markierten Positionen werden komplett verschoben. Wenn nur Teilmengen angegeben sind, werden die entsprechenden Stückzahlen verschoben.
6.  Dialog für die Verschiebung mit [Auslösen] öffnen. Dialog `Verschiebung (Versand)` wird geöffnet.
7.  Daten für Verschiebung eintragen. Siehe Schritte 3 bis 5 in: "So verschieben Sie eine Position" auf Seite G-1865
8.  Verschiebung mit [Start] auslösen.
9.  Abfragen mit [Ja] beantworten. Markierte Positionen werden auf das neue Lieferdatum verschoben. Die nicht verschobenen Positionen prüfen.
10. Verschiebung prüfen: Tourensuche mit neuem Lieferdatum starten.

### Versand vorbereiten

**Lernziele**
- Fehlmengekontrolle durchführen
- Produzierte Menge prüfen.
- Verfügbare Menge als verpackt buchen.
- Fehlende Menge als Rückstand verschieben

**Nutzen**
- Die Handlungsschritte, die Sie für die Vorbereitung des Versands durchführen, sind Voraussetzung für einen reibungslosen Ablauf der Lieferungen.

Fehlmenge der Position kann unterschiedlich behandelt werden:
- Als Rückstand auf einen anderen Liefertermin verschieben.
- Als (Kunden-)Storno aus dem Auftrag entfernen und Position als komplett buchen.

*Abb. G-7: Fehlmenge in der Versandsteuerung kontrolieren*
- A: Auftragspositionen
- B: Aktionen

#### Fehlmengekontrolle durchführen

**So führen Sie die Fehlmengekontrolle durch**
1.  Register `TourenInfo` > Auftragsebene öffnen.
2.  Auftrag markieren: `<Shift>` + `<F9>`. Dialog `Fehlmengenkontrolle für...` wird geöffnet.
3.  Auftragsdaten prüfen und ggf. korrigieren.
4.  Fehlmengenkontrolle mit [Auslösen] öffnen. Dialog `Versandsteuerung für Fehlmengenkontrolle` wird geöffnet.
5.  Mengen in Spalte `Fertig` prüfen. Wenn fertige Menge nicht identisch mit geplanter Menge ist, Fehlmenge verschieben. Siehe dazu die Zusatzinfo.
   So verschieben Sie mehrere Positionen,
6.  Fertige Menge nach Rücksprache korrigieren.
7.  Korrigierte Mengen mit [Buchen] speichern. Menge für den Rückstand wird in Spalte `Rück.` angezeigt. ⇨ "Verpackte Menge korrigieren" auf Seite G-1869
8.  Fehlmenge mit [Buchen] verschieben. ⇨"So verschieben Sie eine Position" auf Seite G-1865. Register `AuftragsInfo` wird angezeigt. Status des Auftrags ist umgesetzt auf komplett verpackt.

#### Verpackte Menge korrigieren

**So können Sie die verpackte Menge korrigieren**
1.  Register `TourenInfo` > Positionsebene öffnen.
2.  Position für die Buchung der verpackten Menge wählen.
3.  Verpackte Menge in Spalte `Verp.` prüfen. Wenn verpackte Menge nicht identisch mit fertiger Menge ist, aktuellen Stand der Verpackung nachfragen.
4.  Verpackte Menge nach Rücksprache korrigieren: Korrekturmodus mit `<Shift>` + `<F10>` freischalten. Cursor springt in die Spalte `Verp.`
5.  Verpackte Menge in Spalte `Verp.` korrigieren.
6.  Verpackte Mengen buchen. Verpackte Menge wird gebucht. Positionsstatus wird umgesetzt. Die Checkbox `Kmp` wird markiert, wenn die gesamte Positionsmenge komplett fertig gebucht ist.
7.  Schritte 2 bis 3 nach Bedarf für jede Position wiederholen.

**Verpackt gemeldete Menge reduzieren:**
8.  Verpackte Menge in Spalte `Verp.` korrigieren. Dialog `Buchungsprotokoll` wird geöffnet.
9.  Buchungsdaten eingeben.
10. Reduzierung der verpackten Menge mit [Buchen] bestätigen. Verpackt gemeldete Menge wird gebucht. Nicht verpackte Menge wird im Feld `Rück.` angezeigt.
11. Reduzierte Menge auf ein anderes Lieferdatum verschieben. ⇨ "Mehrere Positionen verschieben" auf Seite G-1866
12. Fertig geplante Tour können für weitere Bearbeitung sperren: Tourebene > `<Shift>` + `<F10>`

#### Lieferscheine

**Lernziele**
- Vorab-Lieferschein drucken
- End-Lieferschein drucken

**Nutzen**
- Die Nutzung dieser Funktion setzt voraus, dass der Druck von (Voran-) Lieferscheinen konfiguriert ist.
- Im Weiteren können (Vorab-) Lieferscheinen nur gedruckt werden, wenn die auszuliefernden Menge komplett verpackt gemeldet ist.
- Abhängig von der Konfiguration wird mit dem Lieferscheindruck auch die Rechnung gedruckt. Standardmäßig ist die Übergabe an den Rechnungsdruck nicht konfiguriert

**So erstellen Sie einen (Vorab-) Lieferschein**
1.  Register `TourenInfo` > Auftragsebene öffnen.
2.  Auftrag markieren: `<Strg>` + `<F11>`. Dialog `Vorablieferschein für...` wird geöffnet.
3.  Daten prüfen und ggf. anpassen.
4.  Druck mit [Auslösen] starten. Dialog `Drucken auf...` wird geöffnet.
5.  Drucker und Anzahl der Druckexemplare angeben. In der Regel müssen Sie mindestens 2 Exemplare drucken.
6.  Druck des Vorab-Lieferscheins mit `<Enter>` starten.
7.  Druckabfrage mit [Ja] bestätigen. Die Exemplare des Vorab-Lieferscheins werden gedruckt.

**End-Lieferschein erstellen:**
8.  Auftrag markieren: `<Strg>` + `<F9>`. Dialog `Lieferscheinfreigabe für...` wird geöffnet.
9.  Daten prüfen und ggf. anpassen.
10. Lieferscheinfreigabe mit [Auslösen] buchen. Dialog `Drucken auf` wird geöffnet.
11. Drucker und Anzahl der Druckexemplare angeben.
12. Lieferscheindruck mit `<Enter>` starten. Lieferschein wird gedruckt. Auftragsstatus wird auf gesperrt gesetzt. Je nach Konfiguration wird der Rechnungsdruck angestoßen.

#### Ladefolge bearbeiten

**Voraussetzungen**
- Funktionen für Ladefolge müssen konfiguriert sein.
- Touren werden im Register `TourenInfo` angezeigt.

**Zusatzinfo**
- Nur für gedruckte Ladelisten können Ergänzungsladelisten gedruckt werden.
- Fertig geplante Tour für weitere Bearbeitung sperren: `Tourebene > <Shift> + <F10>`

**Lernziele**
- Ladefolge ändern.
- Ladeliste für eine Tour drucken.
- Ladelisten für alle Touren drucken.
- Ergänzungsladeliste drucken.

**Nutzen**
- Die Nutzung dieser Funktion setzt voraus, dass das System für die Ladelisten vollständig konfiguriert ist.
- Die Ladelisten vereinfachen die LKW-Be- und Entladung.

*Abb. G-8: Fehlmenge in der Versandsteuerung kontrolieren*

**So ändern Sie die Ladeliste-Nummer**
1.  Register `TourenInfo` > Auftragsebene öffnen.
2.  Zum Register `Lieferanschrift` wechseln.
3.  Feld `LF`: Laufende Nummern ändern.
4.  Abfrage beantworten, ob die Nummer auf die anderen Aufträge des Kunden vererbt werden soll. Die laufende Nummer wird bei allen Aufträgen eingefügt, die zu demselben Kunden gehören.

**So drucken Sie eine neue Ladeliste:**
1.  Register `TourenInfo`: `<Strg>` + `<F8>`.
2.  Drucker und Anzahl der Druckexemplare angeben.
3.  Druck mit `<Enter>` starten. Ladeliste wird gedruckt. Der Status der Tour wird auf gesperrt gesetzt.

**So drucken Sie Ladelisten für alle angezeigten Touren:**
1.  Register `TourenInfo`: `<Strg>` + `<F12>`.
2.  Haus (Mandant) und Zeitspanne prüfen und ggf. anpassen.
3.  Eingabe mit `<Enter>` bestätigen.
4.  Drucker und Anzahl der Druckexemplare angeben.
5.  Druck mit `<Enter>` starten. Ladeliste wird gedruckt. Der Status der Tour wird auf gesperrt gesetzt.

**So drucken Sie Ergänzungsladelisten:**
1.  Register `TourenInfo`: `<Strg>` + `<F10>`.
2.  "So drucken Sie Ladelisten für alle angezeigten Touren:" auf Seite G-1872. Ladeliste mit den Ergänzungen zur Original-Ladeliste wird gedruckt.

### Gestelle

*Abb. G-9: Gestaffelten Preis anlegen*

#### Gestellmeldungen aus A+W Production
Wenn durch die Rückmeldung aus A+W Produktion eine Bestellung für die bestellte Bearbeitungen erzeugt wird, so werden im Versand 2 Sätze für diese Bestellung erzeugt (Ausnahme Direktlieferung). Gleichzeitig werden für jede Bestellung zusätzlich Daten in eine neue DB-Tabelle 'lapoolstrukt' geschrieben, so dass die Scheiben aus der Ebene der bestellten Bearbeitung vermerkt sind. Diese werden später nach der Fertigstellung zwischenverpackt gemeldet, um die Vorprodukte an den Lieferanten verschicken zu können.

In der Tabelle sind dann Position und Tupel aus dem Auftrag so wie Position und Tupel der Bestellung vermerkt.

Durch die Zwischenverpackt Meldung der Bestellpositionen werden die Mengen als verfügbar gemeldet.

Diese Daten werden analog zu VK-Seite in die neue Tabelle 'kpossumek' gebucht.

Gestellmeldungen aus BDE können nun auch für Zwischenprodukte generiert werden. Die Auswertung dieser Buchungen wurde jetzt auch für EK-Vorgänge aktiviert. Die Zuordnung der Scheiben erfolgt mit einer zusätzlichen Information über das zugehörige Element (Tupel) der Scheibe in der Stückliste der Bestellposition. Wenn die Daten im Versand (ausreichende Mengen) bei der Gestellmeldungen vorhanden sind, so werden die Gestelle auch sofort fest einer Tour zugeordnet und die zugehörigen EK-Auslieferungssätze werden im Versand verpackt gemeldet.

Alle Funktionalitäten für die Gestelle, die über Untermenü "Gestelle" im Versand aufgelistet sind, sind für EK Vorgänge (Warenausgang-Modus) auch aktiv.

**Ausnahmefall**
Für den Fall, dass ein VSG Verbund extern bestellt wird, gehören zu einer Bestellposition mehrere Einzelscheiben, die auf Gestellen gemeldet werden. Wir bezeichnen ein Gestell symmetrisch belegt, wenn aus den aufgestellten Scheiben eine komplette Bestellposition gebildet werden kann. So werden die per BDE gemeldete Mengen nur dann als verpackt und zugeordnet gemeldet, wenn das Gestell symmetrisch belegt ist. Konnten aus den gemeldeten Glasmengen keine vollständige Bestellpositionen restlos gebildet werden, werden die Mengen nur dem Gestell zugeordnet und müssen dann manuell entsprechend verteilt werden, so dass die Bestellpositionen als komplett verpackt gemeldet werden können und ein Gestell dann zu der Tour auch festgebucht werden kann.

#### Gestellrückmeldungen aus A+W Production
Beim Verpacken oder Versenden eines Gestells erfolgt eine Rückmeldung mit der Gestellbelegung an das ERP-System. Dabei werden üblicherweise alle Scheiben auf dem Gestell gemeldet. Anhand der gebuchten Bearbeitungen der Scheiben auf dem Gestell kann jetzt bestimmt werden, ob eine Gestellrückmeldung für die verlängerte Werkbank erfolgen soll. Mit einem schon vorhandenen Schalter werden nur Scheiben gemeldet, deren Bearbeitung Verpacken oder Versenden bereits gebucht ist. Damit wird verhindert, dass ein Gestell verpackt oder versendet gemeldet wird, wenn sich auf dem Gestell nur Scheiben befinden, deren Bearbeitung Zwischenverpacken oder Zwischenversenden für die verlängerte Werkbank gebucht ist.

Mit einem weiteren Schalter kann beim Verpacken eines Gestells jetzt unterschieden werden, ob die Scheiben auf dem Gestell die Bearbeitung Verpacken oder Zwischenverpacken für die verlängerte Werkbank gebucht haben. Ist die Bearbeitung Verpacken gebucht, erfolgt die Rückmeldung für Verpacken mit den verpackten Scheiben. Ist keine Bearbeitung Verpacken gebucht, aber die Bearbeitung Zwischenverpacken, so erfolgt jetzt eine neue Gestellrückmeldung mit den zwischenverpackten Scheiben.

Entsprechend ist die Logik beim Versenden eines Gestells.

*Abb. G-10: Währungen*

### Anbindung des A+W Logistics Optimizer

#### Auslösende Aktionen
Die folgenden Änderungen wurden implementiert:
- Wird eine Tour optimiert, werden die Gestellzuordnungen für diesen Liefertag und Route auf die Optimierungstour verschoben.
- Wird eine Tour optimiert, wird dies nun im Verschiebeprotokoll eingetragen.
- Wird eine Tour optimiert, wird jetzt zusätzlich die Telefonnummer, die E-Mail, die Kontaktperson und der Erlös der übergebenen Positionen an die Routenoptimierung übergeben.
- Bei der Rückmeldung einer optimierten Route, wird jetzt der Anliefertag und die Fahrtdauer in Tagen in den Versand zurückgemeldet (Wenn Tour mehr als einen Tag unterwegs ist).
- Wird eine Tour aus der Routenoptimierung gelöscht, wird nun im Versand die vorherige Routenzuordnung wiederhergestellt.
- Eine bereits optimierte Tour kann jetzt nicht mehr an die Routenoptimierung übergeben werden. Die Tour muss vorher aus der Routenoptimierung gelöscht werden.
- Das Verschieben im Versand ist für optimierte Touren nicht mehr erlaubt und es kann nichts manuell auf eine optimierte Tour geschoben werden.

### Zusatzfunktionen

#### Touren-Übersicht

**Ziel der Handlung**
- Auslastung der Touren eines Lieferdatums darstellen.
- Auslastung einer Tour an aufeinander folgenden Liefertagen darstellen.

**Voraussetzungen**
(keine)

*Abb. G-11: Dialoge zur Dateneingaben bei der Verschiebung*

*Abb. G-12: Dialoge zur Verschiebung*

#### Workflow
1.  Register `TourenInfo`.
2.  Parameterauswahl mit `<Shift>` + `<F11>` öffnen. Dialog `1. Parameter für Übersicht` wird geöffnet.
3.  Parameter 1 wählen: `Stück, QM, Gewicht`.
4.  Mit `<Enter>` bestätigen. Dialog `2. Parameter für Übersicht` wird geöffnet.
5.  Parameter wählen: `Alle Routen für den aktuellen Tourentag anzeigen`.
6.  Mit `<Enter>` bestätigen. Ist- und Soll-Stückzahlen für die Touren werden dargestellt.

**Auslastung einer Tour anzeigen.**
7.  Parameter 1 wählen und mit `<Enter>` bestätigen. Dialog `2. Parameter für Übersicht` wird geöffnet.
8.  Parameter wählen: `Nächste Tourentage für aktuelle Route anzeigen`.
9.  Mit `<Enter>` bestätigen. Auslastung der Tour an Folgetagen wird dargestellt.

#### Auftragsinformation in der Versandsteuerung

**Ziel der Handlung**
- Informationen zum Auftrag einsehen.
- Informationen des Fertigwarenlagers zum Auftrag einsehen.
- Buchungsprotokoll zum Fertigwarenlager einsehen.

**Voraussetzungen**
- Touren werden im Register `TourenInfo` angezeigt.
- Fertigwarenlager muss konfiguriert sein.

#### Workflow
1.  Register `TourenInfo` > Auftragsebene öffnen.
2.  Auftrag markieren: `<Strg>` + `<K>`. Dialog `Informationen zu Auftrag` wird geöffnet.
3.  Auftragsnummer eingeben
4.  Modus prüfen: `VK-Aus`.
5.  Suche mit [Auslösen] starten. Dialog `Informationen zu Auftrag` wird geöffnet.
6.  Auftragsinfos verlassen: mit [Springen] zurück zum Register `PositionsInfo`.

**Aufträge im Fertigwarenlager einsehen:**
7.  Informationen zum Buchungsprotokoll des Fertigwarenlagers mit [FW Lager] öffnen. Dialog `Fertigwarenlager Buchungsprotokoll` wird geöffnet.

**Buchungen im Fertigwarenlager einsehen:**
8.  Übersicht für das Fertigwarenlager mit [Protokoll] öffnen. Dialog `Fertigwarenlager Übersicht` wird geöffnet.

### Servicefunktion

Führen Sie die nachfolgenden Funktionen nur auf Anforderung durch den Servicemitarbeiter der A+W Software GmbH aus.

In diesem Abschnitt finden Sie Informationen zu folgenden Themen:
- "Funktionstest (F-Test) starten" auf Seite G-1881
- "Funktionstest (F-Test) stoppen" auf Seite G-1881

#### Funktionstest (F-Test) starten
`<Strg> + <F4> > <Shift> + <F12> > <9> > [Nein]`

Mit dieser Tastenfolge starten Sie den Funktionstest. Die Service-Techniker benötigen die Protokollierung der Programmabläufe, um im Problemfall die Fehlerquellen zu finden. Beachten Sie folgende Punkte zum Funktionstest:
- Nur auf Anweisung der Service-Techniker einschalten.
- Nach dem Start wird jede Aktion der Software protokolliert.
- Verbraucht zusätzliche Rechenkapazität und zusätzliche Festspeicherkapazität.
- Kann zusammen mit der Datenbankprotokollierung durchgeführt werden.
- Die Eingabe 9 gibt den Hilfelevel für die Protokollierung an.
- Der darauf folgende Dialog `Output on screen` ist mit [Nein] zu bestätigen, um für die Service-Techniker die Protokoll-Datei zu erzeugen.

#### Funktionstest (F-Test) stoppen
`<Strg> + <F4> > <Shift> + <F12>`

Mit dieser Tastenfolge stoppen Sie den Funktionstest.

## Softwarereferenz: A+W Enterprise Versandsteuerung

### In diesem Kapitel finden Sie folgende Themen:
- Übersicht
- Startfunktionen
- Versand-Explorer
- Versandsteuerung - Menüs
- Touren
- Auftragsebene
- Positionsebene
- Funktionen im Versand
- Storno
- Gestelle
- Drucken

**Inhaltsverzeichnis:**
- Übersicht (G-1887)
- Startfunktionen (G-1888)
  - Programmstart (G-1889)
  - Auftragssuche (G-1891)
  - Marktpartnersuche (G-1892)
- Versand-Explorer (G-1893)
  - Explorer - Baumstruktur (G-1894)
  - Übersicht für die Lieferdatumsebene (G-1895)
  - Übersicht für die Tourenebene (G-1897)
  - Übersicht für die Auftragsebene (G-1898)
  - Übersicht für die Positionsebene (G-1899)
- Versandsteuerung - Menüs (G-1900)
  - Zusatzmenü (G-1900)
  - Infomenü (G-1903)
  - Schaltflächen (G-1905)
- Touren (G-1906)
  - Register - TourenInfo (G-1907)
  - Register - GestellInfo (G-1910)
  - Register - FahrzeugInfo (G-1912)
  - Register - Optimierung (G-1914)
- Auftragsebene (G-1916)
  - Register - AuftragsInfo (G-1917)
  - Register - AuftragsInfo/Gestell (G-1922)
  - Register - Lieferanschrift (G-1924)
  - Register - VersandInfo I (G-1926)
  - Register - VersandInfo II (G-1929)
  - Register - Zusatzinfo (G-1931)
- Positionsebene (G-1934)
  - Register - PositionsInfo I (G-1935)
  - Register - PositionsInfo II (G-1938)
- Funktionen im Versand (G-1940)
  - Suchen (G-1941)
  - Springen (G-1942)
  - Verschieben (G-1944)
  - Verschieben mehrerer Pos. - Auswahl (G-1946)
  - Verschiebung mehrerer Pos. - Aktion (G-1947)
  - Auftragsinfo (G-1948)
  - Informationen zum Auftrag (G-1949)
  - Liefereingang buchen (G-1951)
  - Storno des Liefereingangs (G-1952)
  - Fehlmengenkontrolle - Auswahl (G-1953)
  - Fehlmengenkontrolle - Aktion (G-1955)
  - Buchen auf Transport (G-1957)
  - Transport zurückbuchen (G-1958)
  - Barcode Gestellanzeige (G-1959)
  - Ergebnisse der Gestellplanung (G-1960)
  - Packmittelplanung (G-1961)
  - Lieferanschrift suchen (G-1962)
  - Neue Lieferanschrift (G-1963)
  - Gestellinformationen (G-1964)
  - Toursperre setzen/löschen (G-1965)
  - Alle Touren sperren (G-1966)
  - Transportdaten (G-1967)
  - Lagerkommissionierung (G-1968)
- Storno (G-1969)
  - Lieferscheinstorno (G-1969)
  - Auftragsstorno (G-1970)
  - Wareneingangsstorno (G-1971)
  - Storno des Versandstatus (G-1972)
- Gestelle (G-1973)
  - Gestellzuordnung - Auswahl (G-1974)
  - Gestellzuordnung - Anzeige (G-1975)
  - Gestellauflösung - Auswahl (G-1977)
  - Gestellauflösung - Anzeige (G-1977)
  - Freie Gestelle (Übersicht) (G-1979)
  - Gebuchte Gestelle (Übersicht) (G-1981)
  - Alle Gestelle (Übersicht) (G-1982)
  - Einzelne Gestelle (G-1984)
  - Gestelle zu Auftrag (G-1985)
  - Scheibenzuordnung (G-1987)
  - VK/EK Information (G-1990)
  - VK/EK Info (Global) (G-1992)
  - Versandsteuerung - Übersicht (G-1994)
  - Lieferterminänderungen (G-1997)
  - Versandinformationen (G-1998)
  - Via Details (G-1999)
- Fertigwarenlager (G-2000)
  - Fertigwarenlagerbestand (G-2001)
  - Fertigwarenlager Übersicht (G-2002)
  - Fertigwarenlager Inventur (G-2003)
  - Inventur abschließen (G-2003)
  - Protokoll (G-2004)
- Grafische Tourenübersicht (G-2006)
- Drucken (G-2007)
  - Drucken einer Ladeliste (G-2008)
  - Drucken aller Ladelisten (G-2009)
  - Drucken Ergänzungsladelisten (G-2010)
  - Listendruck (G-2011)
  - Vorablieferschein Druck (G-2012)
  - Lief./Wareneing. Freigabe + Druck (G-2014)
  - Druckformat (G-2015)
- Druckerauswahl (G-2015)

### Übersicht

Alle Ansichten, Dialoge und Funktionen für die Versandsteuerung sind über das Modul `Logistik` erreichbar. Sie können das Modul auch direkt aus dem FixWin starten. In der Standard-Konfiguration starten Sie direkt mit dem Versand-Explorer:
⇨ "Versand-Explorer" auf Seite G-1893

Mit der Versandsteuerung finden, planen, bearbeiten und versenden Sie termingerecht Ihre Lieferaufträge. Die Versandsteuerung ist die Steuerzentrale für das Versandgeschäft und ermöglicht den einfachen und schnellen Zugriff auf alle Lieferaufträge. Sie erstellen z. B. eine Auflistung aller Liefertermine eines Zeitraums oder springen direkt in den gesuchten Lieferauftrag. Für die Übersicht der Versandvorgänge ist jeder Lieferauftrag in die folgenden vier Ebenen eingeteilt:
- Liefertermine
- Touren mit Routen
- Aufträge
- Positionen

Die **Liefertermine** sehen Sie in der ersten Ebene. Ein Liefertermin enthält die zugehörigen Touren oder Routen.

Die **Touren mit den Routen** sehen Sie in der zweiten Ebene. Eine Tour enthält die zugehörigen Aufträge und kann aus einer oder mehreren Routen bestehen. Eine Tour steht für mindestens eine Route, die zu einem bestimmten Liefertermin gefahren wird. Die Route steht für eine festgelegte Fahrstrecke. Die Routen können auf bestimmte Wochentage oder auf bestimmte Zeiten festgelegt werden. In der Tourenebene haben Sie eine Übersicht zu den vorhandenen Versandpapieren.

Die **Aufträge** sehen Sie in der dritten Ebene. Ein Auftrag enthält die zugehörigen Positionen und die Lieferanschrift. In der Auftragsebene haben Sie eine Übersicht zu den vorhandenen Versandpapieren.

Die **Positionen** sehen Sie in der vierten Ebene. Eine Position enthält die zugehörigen Einheiten.

Geöffnete Touren, Aufträge oder Positionen sind für andere Mitarbeiter zur Bearbeitung gesperrt. sie werden dann nur mit Leserecht geöffnet.

### Startfunktionen

In A+W Enterprise haben Sie die Möglichkeit, über verschiedene Suchfunktionen Ihre Liefertermine und Aufträge zu suchen.

Zu diesem Thema finden Sie folgende Informationen:
- "Programmstart" auf Seite G-1889
- "Auftragssuche" auf Seite G-1891
- "Marktpartnersuche" auf Seite G-1892

#### Programmstart
**Navigation**: `Logistik > Versandsteuerung`

*Abb. G-13: Suchmodus*

Sie starten die Versandsteuerung mit der Eingabe der folgenden Kriterien:
- Versandmodus (alle, VK-Ausgang, EK-Warenaus- und -eingang)
- Hausnummer bzw. Mandantennummer
- Liefertermin
- Lieferzeitraum

Über die Felder in der Kopfzeile filtern Sie Ihre Suche und das System listet Ihnen anhand der eingegebenen Daten die Liefertermine auf.

**VK-Aus.** Versandmodus. Standardmäßig werden in der Versandsteuerung nur die auszuliefernden Aufträge behandelt. Bei einer entsprechenden Konfiguration können jedoch auch die Bestellungen, komplett oder nur mit bestellten Bearbeitungen, im Versand - Modul bearbeitet werden. Sprechen Sie einen zuständigen Mitarbeiter von A+W an, falls Sie nähere Informationen darüber benötigen. Wenn die Verkaufs- und Einkaufs-Vorgänge über den Versand abgewickelt werden, können auch alle Aufträge für das gewählte Datum bzw. für den gewählten Zeitraum angezeigt werden, wie z. B., im Versand-Explorer, oder auf einer Datenebene.
Technische Info: Toggle-Feld, DB-Feld: `lapool.vmodus`

**Haus**: Nummer des Hauses oder Mandanten.
Technische Info: Numerisches Feld, DB-Feld: `lapool.hausnr`

**Lieferdatum**: Eingabefeld für das Lieferdatum eines bestimmten Tages.
Technische Info: Datumsfeld, DB-Feld: `lapool.ltplan`

**bis**: Eingabefeld für das Lieferdatum eines bestimmten Zeitraums.
Technische Info: Datumsfeld, DB-Feld: `lapool.ltplan`

> **Lieferdatum**
> Die Eingabe des Zeitraums ist nur möglich, wenn Sie mit dem Versandexplorer arbeiten. Alternativ ist nur ein Lieferdatums-Feld aktiv.
> Wenn Sie in beiden Datumsfelder das gleiche Datum eingeben, startet die Versandsteuerung direkt mit der Tourenebene.

#### Auftragssuche
**Navigation**: `Versandsteuerung > [Suchen] > <F9>`

*Abb. G-14: Auftragssuche*

In der Versandsteuerung besteht die Möglichkeit, an vielen verschiedenen Stellen nach Aufträgen über die erweiterte Suche zu suchen. In den Eingabefeldern des Dialogkopfs geben Sie die Kriterien für die Suche ein. Im unteren Bereich wird die Trefferliste angezeigt. Die Suchergebnisse werden in verschiedenen Registern zusammengefasst.

Die Suchmöglichkeit nach bestimmten Vorgangsarten wurde im gesamten A+W Enterprise mit der Version 6 einheitlich gestaltet.

Ausführliche Dokumentation darüber finden Sie im Part Verkauf.
- Verkauf, "Suche Aufträge" auf Seite D-1077
- Verkauf, "Suche Aufträge - Trefferliste" auf Seite D-1082

#### Marktpartnersuche
**Navigation**: `Versandsteuerung > [Suchen] > <F9> > Feld Kunde > <F9>`

*Abb. G-15: Marktpartner-Suchdialog*

Ausführliche Dokumentation über die Marktpartnersuche finden Sie im Part Verkauf:
- Verkauf, "Marktpartnersuche" auf Seite D-1091

### Versand-Explorer
**Navigation**: `Logistik > Versandsteuerung > Eingabe einer Zeitspanne`

*Abb. G-16: Versandsteuerung – Ansicht Explorer*

- **A** Kopfdaten: Eingabe der Suchkriterien
- **B** Explorer - Baumstruktur
- **C** Detailinformation zu dem ausgewählten Liefertermin
- **D** Detailinformation zu der ausgewählten Route
- **E** Ausgewählte Datenebene

In der Versandsteuerung sehen Sie die Lieferaufträge nach dem Lieferdatum aufgelistet, die anhand der Suchkriterien ermittelt wurden.

**VK-Aus.** VK-Ausgang: ausgewählter Versandmodus.
Technische Info: Toggle-Feld, DB-Feld: `lapool.vmodus`

**Haus** Nummer des Hauses oder Mandanten.
Technische Info: Numerisches Feld, DB-Feld: `lapool.hausnr`

**Lieferdatum** Eingabefeld für das Lieferdatum eines bestimmten Tages.
Technische Info: Datumsfeld, DB-Feld: `lapool.ltplan`

**bis** Eingabefeld für das Lieferdatum eines bestimmten Zeitraums.
Technische Info: Datumsfeld, DB-Feld: `lapool.ltplan`

#### Explorer – Baumstruktur
Zur besseren Übersicht sind die Lieferaufträge in der Explorer-Struktur aufgebaut. Das Arbeiten mit dem Versand-Explorer muss zunächst entsprechend konfiguriert werden. Im Explorer werden die Versanddaten in mehreren Ebenen dargestellt:
- Datumsebene
- Routenebene
- Vorgangsebene
- Positionsebene

Jede Ebene ist mit einem festgelegten Symbol gekennzeichnet. In der rechten Dialoghälfte wird eine kurze Übersicht über die vorhanden Lieferungen angezeigt.

In der Baumstruktur wählen Sie die Ebene aus. Wenn das Ebenen-Feld blau hinterlegt ist, dann ist die Ebene ausgewählt.

In den folgenden vier Ebenen werden Kurzinformationen als Schnellübersicht angezeigt:
- "Übersicht für die Lieferdatumsebene" auf Seite G-1895
- "Übersicht für die Tourenebene" auf Seite G-1897
- "Übersicht für die Auftragsebene" auf Seite G-1898
- "Übersicht für die Positionsebene" auf Seite G-1899

#### Übersicht für die Lieferdatumsebene
**Navigation**: `Logistik > Versandsteuerung > Eingabe einer Zeitspanne, Datum im Explorer`

*Abb. G-17: Datumsebene im Versand-Explorer*

Nach der Liefertermin-Auswahl im Explorer werden in der Übersicht folgende Felder angezeigt:

**Route** Nummer der Route.
Technische Info: Numerisches Feld, DB-Feld: `lapool.routenr`

**Haus** Nummer des Hauses oder Mandanten.
Technische Info: Numerisches Feld, DB-Feld: `lapool.hausnr`

**Typ** Versandmodus: Aufgrund der begrenzten Platzmöglichkeit wird der Name des Feldes (Versandmodus=Typ) sowie auch die Anzeige des Versandmodus weitgehend gekürzt:
- **VK**: VK-Ausgang
- **E1**: EK-Wareneingang
- **E2**: EK-Warenausgang
Technische Info: Alphanumerisches Feld, DB-Feld: `lapool.vmodus`

**Name** Routenbezeichnung aus den A+W Enterprise - Stammdaten.
Technische Info: Anzeigefeld, DB-Feld: `route.routenname`

**Ges.** Gesamte Stückzahl der Position, die für diese Route erfasst ist.
Technische Info: Numerisches Feld, DB-Feld: `lapool.gesstk`

**Abruf** Stückzahl der Position, die der Kunde für den Liefertermin anfordert.
Technische Info: Numerisches Feld, DB-Feld: `lapool.abrufstk`

**Verf.** Verfügbare Stückzahl der Position.
Technische Info: Numerisches Feld, DB-Feld: `lapool.sollstk`

**Verp.** Verpackte Stückzahl der Position.
Technische Info: Numerisches Feld, DB-Feld: `lapool.iststk`

**kmp.** Komplett gemeldete Route. Alle Aufträge sind verpackt.
- ☑ Alle Positionen sind zur Auslieferung bereit.
- ☐ Noch nicht alle Positionen sind zur Auslieferung bereit.
Technische Info: Anzeigefeld

#### Übersicht für die Tourenebene
**Navigation**: `Logistik > Versandsteuerung > Eingabe einer Zeitspanne, Datum im Explorer`

*Abb. G-18: Tourenebene im Versand-Explorer*

Nach der Routen-Auswahl im Explorer werden in der Übersicht folgende Felder angezeigt:

**Auftrag/Bestellung** Auftragsnummer oder Bestellnummer für die geplante Lieferung je nach Versandmodus. Es wird immer nach der Vorgangsart unterschieden: 5=Auftrag, 2=Bestellung
Technische Info: Numerisches Feld, DB-Feld: `lapool.auftrnr`, `lapool.vorgang`

**Kunde** Kundenname bei Aufträgen bzw., Lieferantenname bei Bestellungen für die geplante Lieferung.
Technische Info: Alphanumerisches Feld, DB-Feld: `mp.name`

Die folgenden Felder sind von der vorhergehende Übersicht übernommen:
- **Ges.** (gesamt)
- **Abruf**
- **Verf.** (verfügbar)
- **Verp.** (verpackt)
- **kmp.** (komplett)

#### Übersicht für die Auftragsebene
**Navigation**: `Logistik > Versandsteuerung > Eingabe einer Zeitspanne, Datum im Explorer`

*Abb. G-19: Auftragsebene im Versand-Explorer*

Nach der Auftrags-/Bestellungs-Auswahl im Explorer werden in der Übersicht folgende Felder angezeigt:

**Pos.** Laufende Positionsnummer aus dem Auftrag bzw. der Bestellung.
Technische Info: Numerisches Feld, DB-Feld: `lapool.posnr`

**Artikel** Artikelbezeichnung des zu liefernden Artikels.
Technische Info: Numerisches Feld, DB-Feld: `artikel.artbez1`

Die folgenden Felder werden von der vorhergehende Übersicht übernommen:
- **Ges.** (gesamt)
- **Abruf**
- **Verf.** (verfügbar)
- **Verp.** (verpackt)
- **kmp.** (komplett)

#### Übersicht für die Positionsebene
**Navigation**: `Logistik > Versandsteuerung > Eingabe einer Zeitspanne, Datum im Explorer`

*Abb. G-20: Positionsebene im Versand-Explorer*

Die Übersicht aus der Positionsebene listet alle Auftragspositionen bzw. alle Positionen aus dem Einkaufsvorgang mit den jeweiligen Feldern, wie auf Auftragsebene.

Die Felder sind in den folgenden Kapitel beschrieben:
- "Übersicht für die Lieferdatumsebene" auf Seite G-1895
- "Übersicht für die Auftragsebene" auf Seite G-1898

### Versandsteuerung – Menüs

In der Versandsteuerung stehen Ihnen zusätzliche Funktionen zur Verfügung. Diese sind auf allen verfügbaren Ebenen unter Zusatz- und Infomenüs zusammengefasst. Ein detaillierter Überblick über die beiden Menüs sind in den folgenden Kapiteln beschrieben:
- "Zusatzmenü" auf Seite G-1900
- "Infomenü" auf Seite G-1903
- "Schaltflächen" auf Seite G-1905

#### Zusatzmenü
**Navigation**: `Versandsteuerung – Übersichtsebenen > <F4>`

*Abb. G-21: Zusatzmenü auf der Tourenebene*

Auf allen Ebenen der Versandsteuerung haben Sie zusätzliche Funktionen, die über Zusatzmenü `<F4>` erreichbar sind. Die hier aufgelisteten Funktionen können je nach Konfiguration, Kontex und Datenbestand nur begrenzt oder sogar gar nicht zur Verfügung stehen.
- "Zusatzmenü auf der Tourenebene" auf Seite G-1901
- "Zusatzmenü auf der Auftragsebene" auf Seite G-1902
- "Zusatzmenü auf der Positionsebene" auf Seite G-1902
