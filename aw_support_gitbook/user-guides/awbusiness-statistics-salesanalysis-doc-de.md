---
description: "DE_AWBusiness_Statistik_4.01"
---


# A+W Statistik

---
## Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version/Datum | Beschreibung |
| :--- | :--- |
| 1.00/03-1998 | Ersterstellung |
| 2.00/08-2000 | Überarbeitung Statistik |
| 3.00/12-2003 | Struktureller Umbau auf Programmstruktur 4.0 |
| 3.01/08-2008 | Rechtschreibkorrekturen |
| 3.02/09-2008 | Abbildungen und Part-Nummer angepasst. |
| 3.03/09-2010 | Layout an Doku-Konzept 2010 angepasst. |
| 3.04/01-2013 | Layout an A+W Business angepasst. |
| 4.00/06-2016 | Vollständige Überarbeitung |
| 4.01/01-2017 | Produkt- und Firmennamen angepasst. |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen
- Kontakte

#### Anmerkungen zu diesem Dokument

Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Business gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Dieses Dokument beschreibt die volle Ausbaustufe von A+W Business.

### Urheberrechte

© 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß des Lizenzvertrages ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung von A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

### Kontakte

**A+W Software GmbH**
Am Pfahlgraben 4-10
D-35415 Pohlheim
Tel: +49 6404 205 10
Fax: +49 6404 205 1877
Email: Zentrale@a-w.com
Web: http://www.a-w.com

## Inhalt

- **Vorspann**
  - Revisionsübersicht
  - Editorial
- **Softwarereferenz**
  - Übersicht
  - Verkaufsstatistiken
    - Auftragsinformation
    - Menü Drucken
    - Auftragsinfo - Optionen
    - Auftragsinfo - Erfasst
    - Auftragsinfo - Produziert
    - Auftragsinfo - Fakturiert
    - Auftragsinfo - Offen
    - Auftragsinfo - Grafik
    - Auswahl
    - Umsatz Verkauf
    - Menü Optionen
    - Menü Superstatistik
    - Umsatz Verkauf - Auswahl
    - Umsatz Verkauf - Restriktionen
    - Umsatz Verkauf - Tabelle
    - Umsatzstatistik - Grafik
    - Umsatz Verkauf - SQL
    - Superstatistik
    - Superstatistik - Export
    - Superstatistik – Import
    - Reklamationsstatistik Verkauf
    - Statistik nach Aufbau
    - Statistik nach Aufbau - Auswahl
    - Statistik nach Aufbau - Tabelle
    - Kunden nach AV-Bereich
  - Einkaufsstatistiken
    - Umsatzstatistik Einkauf
    - Reklamationsstatistik Einkauf
    - Liefertreue
    - Analyse Verbrauch
    - Analyse Verbrauch - Auswahl
    - Analyse Verbrauch – Restriktionen
    - Analyse Verbrauch – Tabelle
  - Provisionsstatistik
  - Intrastat Meldung
- **Partindex**
  - Index Statistik

## Softwarereferenz

## Übersicht

A+W Business verfügt über verschiedene Auswertungsmöglichkeiten. Dabei wird, wie nachfolgend beschrieben, zwischen aktueller Auftragsbestandsauswertung, Umsatz-, Reklamations- und Provisionsstatistik unterschieden.

- "Verkaufsstatistiken" auf Seite F-10
- "Einkaufsstatistiken" auf Seite F-44
- "Provisionsstatistik" auf Seite F-54
- "Intrastat Meldung" auf Seite F-56

> **Systemeinstellungen**
> In den Firmendaten können Sie Details für die Übergabe der Aufträge und Bestellungen in die Statistik festlegen. Eine ausführliche Beschreibung finden Sie im Part Stammdaten.
> 
> Stammdaten, "Firmendaten - Archiv" auf Seite B-948

## Verkaufsstatistiken

Die Statistik in A+W Business ist ein wichtiges Instrument für die Unternehmensanalyse. Sie erhalten Auswertungen über Ihre Kunden, Branchen, Produkte, Geschäftsbereiche, Vertreter, etc. Dazu wählen Sie aus, ob die Daten jahresweise oder monatsweise ausgewertet werden sollen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Auftragsinformation" auf Seite F-10
- "Auswahl" auf Seite F-20
- "Umsatz Verkauf" auf Seite F-21
- "Superstatistik" auf Seite F-32
- "Superstatistik – Export" auf Seite F-34
- "Superstatistik - Import" auf Seite F-35
- "Reklamationsstatistik Verkauf" auf Seite F-36
- "Statistik nach Aufbau" auf Seite F-37
- "Kunden nach AV-Bereich" auf Seite F-42

### Auftragsinformation

**Pfad:** Statistik > Auftragsinfo

In diesem Dialog werten Sie Ihren Auftragsbestand aus. Dabei können Sie zwischen den neuen Aufträgen, den an die Produktion übergebenen Aufträgen und den fakturierten Aufträgen unterscheiden.

In diesem Dialog finden Sie folgende Register:
- "Auftragsinfo – Optionen" auf Seite F-11
- "Auftragsinfo – Erfasst" auf Seite F-15
- "Auftragsinfo - Produziert" auf Seite F-16
- "Auftragsinfo - Fakturiert" auf Seite F-17
- "Auftragsinfo - Offen" auf Seite F-18
- "Auftragsinfo – Grafik" auf Seite F-19

### Menü Drucken

**Pfad:** Statistik > Auftragsinfo

Über dieses Menü starten Sie den Druck der Auswertung auf dem Bildschirm oder dem Drucker:

- **Standard:** Öffnet den Dialog Auswahl, um festzulegen, welche Daten gedruckt werden sollen. (Siehe "Auswahl" auf Seite F-20)
- **Umsatz:** Startet den Druck der Umsatzdaten und der Vergleichdaten des Vorjahres. In der tabellarischen Gegenüberstellung werden die Arbeitstage pro Monat angegeben. Die Aufstellung schließt mit den Werten für den durchschnittlichen Umsatz pro Arbeitstag.

### Auftragsinfo – Optionen

**Pfad:** Statistik > Auftragsinfo > Register Optionen

