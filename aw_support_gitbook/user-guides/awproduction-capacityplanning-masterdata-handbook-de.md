---
title: "DE_HB_AWProduction_6"
source: "DE_HB_AWProduction_6.pdf"
tags: ["capacity planning", "A+W Production", "master data", "shift planning", "reservations", "production scheduling", "cost calculation", "Vorgabezeiten", "Schichtpläne", "ERP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A comprehensive tutorial and software reference for the A+W Production Capacity Planning module. This document provides step-by-step instructions for managing reservations, process generation, and configuring essential master data such as shifts, costs, and machine parameters."
long_description: "This document serves as a detailed guide for the A+W Production Capacity Planning (Kapazitätsplanung) software. It is divided into a tutorial section and a software reference section. The tutorial provides practical exercises and instructions on key functionalities, including creating and managing reservations for customers and objects, generating production processes for scheduling, and handling various master data configurations. Key master data topics covered in-depth are: creating and managing shifts and shift plans (Schichten), defining cost calculations (Kostenkalkulation) for labor and machines, setting up transition times (Übergangszeiten) between production steps, configuring default processing times (Vorgabezeiten) using complex formulas, organizing machine groups (Maschinengruppen), and managing load distribution (Lastverteilung) for bottleneck resources. The software reference section provides a systematic overview of the user interface, detailing dialogs, fields, and functions for production monitoring, scheduling, and master data maintenance. The document is intended for administrators and advanced users responsible for setting up and maintaining the capacity planning environment in A+W Production."
---

# Tutorial: Planung und Einlastung

---
## Übungen zu Reservierungen

*   Legen Sie für einen Kunden oder ein Objekt eine Reservierung für mehrere Tage und Schichten an.
*   Erfassen Sie einen Testauftrag für einen Kunden oder ein Objekt mit einem Liefertermin am Ende der zwei Wochen.
*   Lasten Sie den Auftrag ein.
*   Prüfen Sie die Ergebnisse.
*   Legen Sie eine neue Reservierung an und erfassen Sie einen neuen Auftrag, der die reservierten Kapazitäten übersteigt.
*   Lasten Sie den Auftrag ein und prüfen Sie die Ergebnisse.
*   Bearbeiten Sie Reservierungen.

### Ergänzende Informationen
⇨ Softwarereferenz, "Reservierungen" auf Seite E-634

---
## Bearbeitungserzeugung

### Lernziele
*   Was ist die Bearbeitungserzeugung?
*   Wie werden Bearbeitungen erzeugt und in der Stückliste ergänzt?

### Nutzen
Das PPS-System benötigt für die Kalkulation der einzelnen Produktionstermine und Produktionskosten eine detailliertere Stückliste, in der alle Arbeitsschritte enthalten sind. Diese werden im Rahmen der Einlastung durch die Bearbeitungserzeugung erstellt.

### Merke
| Begriff | Definition |
| :--- | :--- |
| **Bearbeitungen** | Bearbeitungen definieren den Bedarf bearbeitet zu werden, z. B. Säumen. |
| **Arbeitsgänge** | Arbeitsgänge definieren die Art und Weise, wie der Bedarf der Bearbeitung erfüllt werden soll, z. B. eine spezielle Art des Säumens. |

> **Voraussetzung**
> Die Bearbeitungserzeugung kann nur durch die Zuordnung von Bearbeitungsartikeln zu Teiletypen durchgeführt werden. Wie Sie Bearbeitungstypen, Bearbeitungsartikel und Teiletypen anlegen, wird im Part Stammdaten beschrieben.
> Bitte sprechen Sie Änderungen in der Bearbeitungserzeugung mit dem Kundenservice der A+W Software GmbH ab, da solche Änderungen produktionsrelevant sind.

### Bearbeitungserzeugung für die Einlastung

Die Stückliste des ERP-Systems enthält das zu fertigende Endprodukt mit seinen Unterteilen und die preisrelevanten Bearbeitungen, z. B. das Säumen der Kanten. Andere Produktionsschritte sind in dieser Stückliste nur implizit enthalten, z. B. der Zuschnitt.

A+W Capacity Planner benötigt für die Kalkulation der einzelnen Produktionstermine und Produktionskosten eine detailliertere Stückliste mit allen Arbeitsschritten, für die ein Aufwand an Zeit oder Kosten notwendig ist. Daher werden im Rahmen der Einlastung produktionsrelevante Arbeitsschritte in der Produktionsstückliste ergänzt. Die Bearbeitungserzeugung stellt damit sicher, dass für jedes Stücklistenteil beschrieben wird, wie es in der Produktion entsteht.

*(Abbildung E-17: Screenshot des Dialogs 'Bearbeitungserzeugung' mit zwei Hauptbereichen: links 'Bearbeitungen' und rechts 'Teiletypen'.)*

**A** Bearbeitungen mit den zugeordneten Bearbeitungsartikeln
**B** Teiletypen mit zugeordneten Bearbeitungen

Damit die Bearbeitungen für die Teile der Stückliste erzeugt werden können, müssen diese Bearbeitungen an den entsprechenden Teiletypen erlaubt sein. Indem Sie die Bearbeitung (A) einem Teiletyp (B) zuordnen, kann die Produktionsstückliste so erzeugt werden, dass alle zeit- und kostenrelevanten Berechnungen durchgeführt werden können.

Daher müssen für die Kapazitätsplanung mindestens für alle Lagerentnahmen, Bestell- und Zuschnittsteile und für den Zusammenbau von VSG und ISO Bearbeitungen definiert sein.

### Bearbeitungen erzeugen

In dieser Lerneinheit erfahren Sie, wie Sie die Stückliste um produktionsrelevante Bearbeitungsschritte ergänzen.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So ergänzen Sie eine Bearbeitung" auf Seite E-504
*   "So entfernen Sie eine Bearbeitung aus der Bearbeitungserzeugung" auf Seite E-505

#### So ergänzen Sie eine Bearbeitung

> **Bearbeitungen ergänzen**
> Bei der Ergänzung von Bearbeitungen sind Änderungen gesetzt, sobald sie im Dialog eingetragen sind. Sie können nicht rückgängig gemacht werden.
> Bitte wenden Sie sich an den Kundenservice der A+W Software GmbH, wenn Sie Bearbeitungen ändern wollen.

1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Bearbeitungserzeugung**.
    *(Screenshot des Dialogs 'Bearbeitungserzeugung')*
2.  Markieren Sie im Feld **Bearbeitungen** den Bearbeitungsartikel, den Sie einem Teiletyp zuordnen wollen.
3.  Markieren Sie im Feld **Teiletypen** einen Teiletyp, dem Sie den Bearbeitungsartikel zuordnen wollen.
4.  Klicken Sie auf den Pfeil nach rechts.
    Der Bearbeitungsartikel wird dem Artikeltyp zugeordnet.
5.  Klicken Sie auf **[OK]**, um die Daten zu speichern.
    Die Zuordnung wird gespeichert.

#### So entfernen Sie eine Bearbeitung aus der Bearbeitungserzeugung

> **Bearbeitungen ergänzen**
> Bei der Ergänzung von Bearbeitungen sind Änderungen gesetzt, sobald sie im Dialog eingetragen sind. Diese können nicht rückgängig gemacht werden.
> Bitte wenden Sie sich an den Kundenservice der A+W Software GmbH, wenn Sie Bearbeitungen ändern wollen.

1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Bearbeitungserzeugung**.
    *(Screenshot des Dialogs 'Bearbeitungserzeugung')*
2.  Markieren Sie im Feld **Teiletypen** den Bearbeitungsartikel, der entfernt werden soll.
3.  Klicken Sie auf den Pfeil nach links.
    Die Zuordnung wird vom Artikeltyp entfernt.
4.  Klicken Sie auf **[OK]**, um die Daten zu speichern.
    Die Änderung wird gespeichert.

---
## Stammdaten der Kapazitätsplanung

Um mit A+W Capacity Planner arbeiten zu können, müssen die Stammdaten für die Kapazitätsplanung eingerichtet sein. Diese Stammdaten bilden zusammen mit den Stammdaten der Maschinenzuordnung (MZO) und den Stammdaten der Artikel die Grundlage für die Einlastung der Aufträge und die Verplanung durch A+W Capacity Planner.

Bevor Sie die Stammdaten der Kapazitätsplanung einrichten oder bearbeiten, müssen die Maschinen und Arbeitsgänge vollständig beschrieben sein. Informationen zu diesem Thema finden Sie im Part Maschinenzuordnung.

> **Stammdaten vor Zugriff schützen**
> Die Stammdaten von AWP und insbesondere von A+W Capacity Planner sind hochsensible Daten. Unkontrollierte oder unbeabsichtigte Eingriffe und Änderungen können die gesamte Produktion stilllegen.
> Richten Sie daher die jeweiligen Arbeitsplätze so ein, dass nur die Administratoren oder Mitarbeiter mit entsprechenden Funktionen Zugriff auf die Stammdaten haben.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Schichten" auf Seite E-508
*   "Kostenkalkulation" auf Seite E-527
*   "Übergangszeiten" auf Seite E-532
*   "Vorgabezeiten" auf Seite E-545
*   "Maschinengruppen" auf Seite E-570
*   "Lastverteilung" auf Seite E-576

> **Datensicherung**
> Erstellen Sie eine vollständige Datensicherung der Stammdaten bevor Sie mit der Bearbeitung der Stammdaten beginnen. Das Backup-Tool finden Sie unter:
> `C:\Programme (x86)\A+W\Techsoft\Tools\AWSplicer\AWSplicer.exe`.
> Verschieben Sie das gespeicherte Backup aus Ihrem User-Verzeichnis in ein Verzeichnis, auf das auch der Support Zugriff hat.
> Besprechen Sie die anstehenden Änderung vorab mit Ihrem Projektierer bei der A+W Software GmbH.

### Schichten

#### Lernziele
*   Wozu dient der Kalender?
*   Was sind Schichten?
*   Welche Angaben werden für eine Schicht benötigt?
*   Wie werden Schichten angelegt, bearbeitet oder gelöscht?

#### Nutzen
Mit Schichten definieren Sie, in welchem Zeitrahmen an bestimmten Maschinen gearbeitet wird.

#### Merke

| Begriff | Definition |
| :--- | :--- |
| **Kalender** | Mit dem Kalender definieren Sie arbeitsfreie Tage, z. B. gesetzliche Feiertage oder Betriebsferien. |
| **Arbeitsschicht** | Arbeitsschichten werden im Produktionsmonitor angezeigt. Eine Arbeitsschicht wird als Schichtplan mit Schichtregeln und Schichtgruppen definiert. |
| **Schichtplan** | Im Schichtplan ist mit Schichtregeln und Schichtgruppen definiert: <ul><li>In wie vielen Schichten wird gearbeitet.</li><li>An welchen Tagen steht die Schicht zur Verfügung.</li><li>Für welche Maschinen gelten die Regeln.</li></ul> |
| **Schichtregel** | Mit einer Schichtregel definieren Sie Einzelheiten einer Schicht, z. B. die Schichtdauer. Zu jeder Schichtregel kann nur eine Schichtgruppe definiert werden. Alle Schichtregeln eines Schichtplans müssen dieselbe Schichtgruppe haben. |
| **Schichtgruppe** | In einer Schichtgruppe sind die Maschinen angegeben, die in der Schicht arbeiten. Alle Schichtregeln einer Schicht müssen dieselben Maschinengruppen haben. |

### Schichtpläne

Mit Schichtplänen definieren Sie Arbeitsschichten, die im Produktionsmonitor angezeigt werden. Im Schichtplan legen Sie fest, in welchem Zeitrahmen die Betriebsmittel in Ihrer Produktion arbeiten. Eine einzelne Arbeitsschicht kann im Produktionsmonitor geändert oder gelöscht werden, ohne dass die Änderung in den Schichtplan übernommen wird.

*(Abbildung E-18: Screenshot des Dialogs 'Schichten'.)*
*   **A** Kalender
*   **B** Schichtplan
*   **C** Schichtregel
*   **D** Schichtregel mit zugewiesenen Maschinen
*   **E** Schichtplan ist verfügbar
*   **F** Daten für den Produktionsmonitor erzeugen

Eine allgemeine Grundlage bildet der Kalender (A), in dem Sie die arbeitsfreien Tage festlegen, z. B. die öffentlichen Feiertage oder Betriebsferien.

Die Schichten definieren Sie in A+W Production durch einen Schichtplan (B) mit Schichtregeln (C) und Schichtgruppen (D).

*   Mit dem Schichtplan (B) definieren Sie die Rahmenbedingungen. Sie erstellen z. B. einen Schichtplan Zwei-Schicht, in dem Sie dann den Zwei-Schicht-Betrieb definieren. Im Schichtplan Zwei-Schicht legen Sie fest, ob dieser aktiv ist, ab wann und wie lange er gültig ist und ob Sie den eigenen Schichtkalender verwenden, oder ob der Schichtkalender aus dem ERP-System importiert werden soll.
*   Zu jedem Schichtplan gehört mindestens eine Schichtregel (C), mit der Sie festlegen, an welchen Tagen und zu welchen Uhrzeiten gearbeitet wird, z. B. im Zwei-Schicht-Betrieb von Montag bis Freitag, jeweils von 6 Uhr bis 14 Uhr in der Frühschicht und von 14 Uhr bis 22 Uhr in der Spätschicht.
*   Die Schichtregel gilt für eine Schichtgruppe (D), in der Sie definieren, welche Maschinen in welchen Schichten arbeiten. So können Sie z. B. festlegen, dass einer Ihrer Schneidetische immer nur in der Frühschicht aktiv ist, oder dass das CNC-Center auch samstags in Betrieb ist. Jeder Schichtregel kann nur eine Schichtgruppe hinzugefügt werden. Wenn Sie mehrere Schichtregeln verwenden, müssen alle dieselbe Schichtgruppe erhalten.

Mit den Schichtregeln können Sie die Planung so einrichten, dass z. B. die Maschinen, an denen Engpässe entstehen können, in mehreren Schichten arbeiten, alle anderen aber nur in einer Schicht.

Jeder Schichtplan kann zunächst unabhängig von der Kapazitätsplanung definiert werden. Damit können Sie Schichtpläne anlegen, die Sie nur zu bestimmten Zeiten aktivieren (E), z. B. für Sonderschichten.

Außerdem kann jeder Schichtplan nur begrenzt gültig sein. So können Sie z. B. für ein geplantes Bauprojekt einen Schichtplan anlegen, der nur für die Zeit gültig ist, in der die Scheiben geliefert werden müssen. Damit werden diese Zeiten außerhalb der Gültigkeit nicht in die Planung einbezogen.

Wenn Sie einen Schichtplan anlegen oder ändern, wird die Schicht nur dann als Arbeitsschicht in den Produktionsmonitor übernommen, wenn sie mit (F) explizit erzeugt wird. Die neuen Arbeitsschichten werden bei der Einlastung in A+W Capacity Planner für die neuen Aufträge berücksichtigt, die bereits eingelasteten Aufträge bleiben davon unberührt.

Eine Übersicht über die Arbeitsschichten und deren Auslastung können Sie sich im Dialog Produktionsmonitor anzeigen lassen.
⇨ Softwarereferenz, “Einlastung" auf Seite E-587

### Arbeitsfreie Tage anlegen

In dieser Lerneinheit lernen Sie, wie Sie arbeitsfreie Tage anlegen, bearbeiten oder löschen.

> **Kalender einrichten**
> Sie müssen den Kalender einrichten, bevor Sie Schichtpläne definieren. Die arbeitsfreien Tage werden nur für neue Schichten berücksichtigt.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So legen Sie arbeitsfreie Tage an" auf Seite E-511
*   "So bearbeiten Sie arbeitsfreie Tage" auf Seite E-512
*   "So löschen Sie arbeitsfreie Tage" auf Seite E-513

#### So legen Sie arbeitsfreie Tage an
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Schichten**.
    *(Screenshot des Schichteditors mit markiertem Kalender (A) und der Liste der arbeitsfreien Tage (B).)*
2.  Markieren Sie im Feld **Schichteditor** den Eintrag **Kalender (A)**.
3.  Klicken Sie auf **[Neu]**.
    Im Bereich **Schichtkalender** wird eine neue Zeile eingefügt.
4.  Tragen Sie in den Feldern **Tag** und **Kommentar** die Daten ein, z. B. einen nationalen Feiertag.
5.  Klicken Sie auf **[Übernehmen]**.
    Die Daten werden gespeichert. Beim Anlegen von neuen Schichten werden die arbeitsfreien Tage übersprungen.

#### So bearbeiten Sie arbeitsfreie Tage
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Schichten**.
2.  Markieren Sie im Bereich **Schichteditor** den Eintrag **Kalender**.
    *(Screenshot des Schichteditors.)*
3.  Markieren Sie im Feld **Schichtkalender** das Datum, das Sie bearbeiten wollen.
4.  Ändern Sie die Werte.
5.  Klicken Sie auf **[Übernehmen]**.
    Die Daten werden gespeichert.

#### So löschen Sie arbeitsfreie Tage
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Schichten**.
2.  Markieren Sie im Bereich **Schichteditor** den Eintrag **Kalender**.
3.  Markieren Sie im Bereich **Kalender** in der ersten Spalte den Tag, den Sie löschen wollen.
    *(Screenshot des Schichteditors mit markiertem Eintrag.)*
4.  Klicken Sie auf **[Löschen]**.
    Der Tag mit dem Pfeil in der ersten Spalte wird gelöscht.
5.  Klicken Sie auf **[Übernehmen]**.
    Die Daten werden gespeichert.

### Schichtplan erstellen

In dieser Lerneinheit lernen Sie, wie Sie Schichtpläne anlegen, bearbeiten oder löschen.
Eine neue Arbeitsschicht kann erst erzeugt werden, wenn zu dem neuen Schichtplan mindestens eine Schichtregel und eine Schichtgruppe mit Maschinen angelegt sind.

> **Daten übernehmen**
> Wenn Sie einen Schichtplan, eine Schichtregel oder eine Schichtgruppe erstellen oder ändern, müssen Sie auf [Erzeugen] klicken, damit die geänderten Schichtdaten im Produktionsmonitor erzeugt wird.
> Wenn die geänderte Schicht nicht erzeugt wird, plant A+W Production die Produktion mit den alten Schichtdaten.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So erstellen Sie einen Schichtplan" auf Seite E-515
*   "So bearbeiten Sie einen Schichtplan" auf Seite E-516
*   "So löschen Sie einen Schichtplan" auf Seite E-517

#### So erstellen Sie einen Schichtplan
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Schichten**.
2.  Markieren Sie im Bereich **Schichteditor** den Eintrag **Kalender**.
    *(Screenshot, der das Kontextmenü (A) und die Schaltfläche (B) zum Erstellen eines neuen Schichtplans zeigt.)*
3.  Öffnen Sie mit einem Rechtsklick auf den Kalender das Kontextmenü (A) und wählen den Eintrag **Neuer Schichtplan**.
    Alternativ können Sie die Auswahl-Liste (B) auf der Schaltfläche [Neu] öffnen und **Neuer Schichtplan** wählen.
    *(Screenshot des leeren Schichtplan-Dialogs)*
4.  Tragen Sie im Bereich **Schichtplan** im Feld **Name** eine Bezeichnung ein, z. B. Zwei-Schicht normal.
5.  Klicken Sie auf **[Übernehmen]**.
    Die Daten werden gespeichert. Der neue Schichtplan wird im Schichteditor angezeigt.
    Als nächstes müssen Sie die Schichtregeln einrichten und die Maschinen zuordnen. Erst danach wird die Schaltfläche [Erzeugen] freigeschaltet.
    ⇨ "Schichtregel erstellen" auf Seite E-517

#### So bearbeiten Sie einen Schichtplan
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Schichten**.
2.  Markieren Sie im Bereich **Schichteditor** den Schichtplan, den Sie bearbeiten wollen.
    *(Screenshot des ausgefüllten Schichtplan-Dialogs)*
3.  Bearbeiten Sie die Werte des Schichtplans.
    Ein typischer Anwendungsfall ist die Verlängerung eines Schichtplans.
4.  Prüfen Sie, ob die Checkbox **Aktiv** markiert ist, damit der Schichtplan in der Kapazitätsplanung verwendet werden kann.
5.  Klicken Sie auf **[Übernehmen]**.
    Die Daten werden gespeichert.
6.  Klicken Sie auf **[Erzeugen]**, damit die Schicht mit den geänderten Daten im Produktionsmonitor erzeugt wird.

#### So löschen Sie einen Schichtplan
> **Schichtplan löschen**
> Wenn Sie einen Schichtplan löschen, werden die zugehörige Schichtregel und die zugehörige Schichtgruppe mit gelöscht! Im Produktionsmonitor wird die gelöschte Schicht weiterhin angezeigt. Um sie aus dem Produktionsmonitor zu löschen, müssen Sie erst die eingelasteten Bearbeitungen umlasten.

1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Schichten**.
2.  Markieren Sie im Bereich **Schichteditor** den Schichtplan, den Sie löschen wollen.
3.  Klicken Sie auf **[Löschen]**.
    Der Schichtplan wird aus dem Schichteditor gelöscht.
4.  Klicken Sie auf **[Übernehmen]**.
    Die Daten werden gespeichert.

### Schichtregel erstellen

In dieser Lerneinheit lernen Sie, wie Sie Schichtregeln anlegen, bearbeiten oder löschen.

> **Daten übernehmen**
> Wenn Sie einen Schichtplan, eine Schichtregel oder eine Schichtgruppe erstellen oder ändern, müssen Sie auf [Erzeugen] klicken, damit die geänderte Schicht im Produktionsmonitor erzeugt wird.
> Wenn die geänderte Schicht nicht erzeugt wird, plant A+W Production die Produktion mit den alten Schichtdaten.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So erstellen Sie eine Schichtregel" auf Seite E-518
*   "So bearbeiten Sie eine Schichtregel" auf Seite E-520
*   "So löschen Sie eine Schichtregel" auf Seite E-521

#### So erstellen Sie eine Schichtregel
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Schichten**.
2.  Markieren Sie den Schichtplan, dem Sie die Schichtregel zuordnen wollen.
    *(Screenshot, der das Kontextmenü (A) und die Schaltfläche (B) zum Erstellen einer neuen Schichtregel zeigt.)*
3.  Öffnen Sie zu dem Schichtplan das Kontextmenü (A) und wählen den Eintrag **Neue Schichtregel**.
    Alternativ können Sie die Auswahl-Liste (B) auf der Schaltfläche [Neu] öffnen und **Neue Schichtregel** wählen.
    *(Screenshot des leeren Schichtregel-Dialogs.)*
4.  Geben Sie einen Namen (A) und eine Schichtnummer (C) ein, z. B. Frühschicht und Nummer 1.
5.  Wählen Sie die Uhrzeit für Schichtbeginn und Schichtende (B), z. B. Beginn 6 Uhr und Ende 14 Uhr.
6.  Markieren Sie die Wochentage, an denen in der Schicht gearbeitet werden soll, z. B. Mo-Fr für eine Fünf-Tage-Arbeitswoche.
7.  Wählen Sie, ob Sie den eigenen Kalender verwenden wollen (D), oder ob der Kalender aus dem ERP-System importiert werden soll, z. B. aus A+W Enterprise.
    Den Gültigkeitszeitraum müssen Sie nur festlegen, wenn Sie eine Sonderschicht einrichten.
8.  Klicken Sie auf **[Übernehmen]**.
    Die Daten werden gespeichert. Der neue Schichtplan wird im Schichteditor angezeigt.
    Als nächstes müssen Sie die Schichtgruppen einrichten und die Maschinen zuordnen. Erst danach wird die Schaltfläche [Erzeugen] freigeschaltet.
    ⇨ "Schichtgruppe erstellen" auf Seite E-522

#### So bearbeiten Sie eine Schichtregel
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Schichten**.
2.  Markieren Sie die Schichtregel, die Sie bearbeiten wollen.
    *(Screenshot des Schichtregel-Dialogs mit Bearbeitungsoptionen.)*
3.  Ändern Sie im Bereich **Schichtregel** die Werte.
    Eine typische Änderung ist, einen Schichtplan zu verlängern. Dazu ändern Sie den Zeitraum (A). Die Felder für den Zeitraum sind nur freigeschaltet, wenn mindestens eine Schichtgruppe zugeordnet ist.
4.  Klicken Sie auf **[Übernehmen] (B)**.
    Die Daten werden gespeichert.
5.  Klicken Sie auf **[Erzeugen] (C)**, damit die Schicht mit den geänderten Daten im Produktionsmonitor erzeugt wird.
    Die Arbeitsschicht wird mit den geänderten Daten im Produktionsmonitor angezeigt.

#### So löschen Sie eine Schichtregel
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Schichten**.
    Bevor Sie eine Schichtregel löschen, sollten Sie die Gültigkeit einschränken. Damit werden die Arbeitsschichten im Produktionsmonitor nicht mehr angezeigt und können nicht mehr bebucht werden.
2.  Markieren Sie die Schichtregel, die Sie löschen wollen.
    *(Screenshot des Schichtregel-Dialogs mit Löschoptionen.)*
3.  Klicken Sie auf **[Löschen] (A)**.
    Die Schichtregel wird aus dem Editor gelöscht.
4.  Klicken Sie auf **[Löschen] (B)**.
    Die Arbeitsschicht wird aus dem Produktionsmonitor gelöscht.

> **Schicht löschen**
> Sie können eine Arbeitsschicht im Produktionsmonitor löschen. Dabei wird nur die einzelne Arbeitsschicht gelöscht. Wenn Sie die Arbeitsschichten löschen wollen, indem Sie die Schichtregel löschen, sollten Sie zunächst die Arbeitsschichten im Produktionsmonitor prüfen. Unter Umständen müssen Sie noch eingelastete Aufträge verschieben.

### Schichtgruppe erstellen

In dieser Lerneinheit lernen Sie, wie Sie Schichtgruppen anlegen, bearbeiten oder löschen.

> **Daten übernehmen**
> Wenn Sie einen Schichtplan, eine Schichtregel oder eine Schichtgruppe erstellen oder ändern, müssen Sie auf [Erzeugen] klicken, damit die geänderte Schicht im Produktionsmonitor erzeugt wird.
> Wenn die geänderte Schicht nicht erzeugt wird, plant A+W Production die Produktion mit den alten Schichtdaten.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So erstellen Sie eine Schichtgruppe" auf Seite E-522
*   "So bearbeiten Sie eine Schichtgruppe" auf Seite E-525
*   "So löschen Sie eine Schichtgruppe" auf Seite E-526

#### So erstellen Sie eine Schichtgruppe
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Schichten**.
2.  Markieren Sie im Bereich **Schichteditor** die Schichtregel, der Sie die Schichtgruppe zuordnen wollen.
    *(Screenshot zeigt das Kontextmenü (A) und die Schaltfläche (B) zum Erstellen einer neuen Schichtgruppe.)*
3.  Öffnen Sie zu der Schichtregel das Kontextmenü (A) und wählen Sie den Eintrag **Neue Schichtgruppe**.
    Alternativ dazu können Sie die Auswahl-Liste (B) auf der Schaltfläche [Neu] öffnen und **Neue Schichtgruppe** wählen.
    *(Screenshot des Dialogs 'Schichtgruppe bearbeiten'.)*
4.  Wählen Sie im Feld **Name (A)** eine Schichtgruppe aus oder tragen Sie einen Namen ein.
    Im Bereich **Schichtgruppe bearbeiten** werden die verfügbaren Maschinen gelistet.
5.  Klicken Sie auf **[Übernehmen]**, um die Daten zu speichern.
6.  Wählen Sie bei allen Maschinen, die Sie der neuen Schichtgruppe zuweisen wollen, in der Spalte **Schichtgruppe (B)** die Schichtgruppe aus.
    *(Screenshot zeigt die Zuweisung von Maschinen zu einer Schichtgruppe.)*
7.  Weisen Sie auf diese Weise jede Maschine einer Schichtgruppe zu.
8.  Klicken Sie auf **[Übernehmen]**.
    Die Daten werden gespeichert. Die neue Schichtgruppe wird im Schichteditor mit allen zugeordneten Maschinen angezeigt.
    *(Screenshot des Schichteditors mit der neuen Schichtgruppe.)*
    Nachdem Sie den Schichtplan vollständig definiert haben, können Sie die Schicht im Produktionsmonitor erzeugen. Dazu gehen Sie folgendermaßen vor:
9.  Markieren Sie den neuen Schichtplan im Schichteditor.
    Der Bereich **Schichtplan** wird angezeigt.
10. Markieren Sie die Checkbox **Aktiv** und tragen Sie das Datum ein, ab dem der Schichtplan gültig ist.
11. Klicken Sie auf **[Erzeugen]**.
    Damit wird die Schicht erzeugt und steht für die Kapazitätsplanung ab dem Gültigkeitsdatum und ggf. für den angegebenen Zeitraum zur Verfügung.

#### So bearbeiten Sie eine Schichtgruppe
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Schichten**.
2.  Markieren Sie im Bereich **Schichteditor** die Schichtgruppe, die Sie bearbeiten wollen.
    *(Screenshot des Dialogs 'Schichtgruppe bearbeiten'.)*
3.  Ändern Sie im Bereich **Schichtgruppe bearbeiten** die Daten, z. B.:
    *   Maschinen anderen Schichtgruppen zuweisen.
        Die Änderung der Zuordnung einer Maschine zu einer Maschinengruppe ist ein typischer Anwendungsfall, um mit einer Maschine in einen anderen Schichtbetrieb zu wechseln.
    *   Namen einer Schichtgruppe ändern.
4.  Klicken Sie auf **[Übernehmen]**, um die Daten zu speichern.
    Die Daten werden gespeichert.
5.  Markieren Sie die aktuelle Schichtregel.
    Der Bereich **Schichtregel** wird mit den aktuellen Daten angezeigt.
6.  Prüfen Sie die Daten und passen Sie ggf. die Einstellungen an, z. B. den Gültigkeitszeitraum.
    Nachdem Sie den Schichtplan bearbeitet haben, können Sie die geänderte Schicht im Produktionsmonitor erzeugen. Dazu gehen Sie folgendermaßen vor:
7.  Klicken Sie auf **[Erzeugen]**.
    Diesen Schritt müssen Sie für alle Schichten ausführen.

#### So löschen Sie eine Schichtgruppe
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Schichten**.
2.  Markieren Sie im Bereich **Schichteditor** die Schichtgruppe, die Sie löschen wollen.
3.  Klicken Sie auf **[Löschen]**.
    Die Schichtgruppe wird gelöscht.
4.  Klicken Sie auf **[Übernehmen]**, um die Daten zu speichern.
    Die Daten werden gespeichert.

### Übungen
Legen Sie die Daten so an, dass sie in allen nachfolgenden Übungen zur Verfügung stehen. Wenn auf diese Weise die Daten für die Kapazitätsplanung vollständig sind, können Sie die Planung für eigene Aufträge im Produktionsmonitor testen.
*   Planen Sie Ihre Produktion auf dem Papier. An welchen Tagen soll in welchen Schichten gearbeitet werden und welche Maschinen werden in welcher Schicht verwendet?
*   Übertragen Sie Ihre Ergebnisse in A+W Production, indem Sie die Schichten definieren.
*   Prüfen Sie Ihre Ergebnisse im Produktionsmonitor.
    ⇨ Softwarereferenz, "Einlastung" auf Seite E-587
*   Ändern Sie für eine Maschine den Schichtplan, z. B. von einem Zwei-Schicht-Plan in einen Drei-Schicht-Plan.
*   Verlängern Sie einen bestehenden Schichtplan.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Schichten" auf Seite E-671

---
### Kostenkalkulation

#### Lernziele
*   Was ist die Kostenkalkulation in der Kapazitätsplanung?
*   Wie werden Kosten für logische Maschinen angelegt, bearbeitet oder gelöscht?
*   Welche Daten werden bei der Kostenkalkulation zwischen A+W Production und dem ERP-System ausgetauscht?

#### Nutzen
*   Mit der Kostenkalkulation kann eine Kostenoptimierung erreicht werden. Zusammen mit den Übergangszeiten werden bei der Einlastung zunächst die billigeren Maschinen ausgelastet.
*   Durch die Aufschlüsselung und Rückmeldung der Kosten werden folgende Vorteile ermöglicht:
    *   Exakte Kostenkalkulation bei Angebots- und Auftragserfassung im ERP-System.
    *   Einlastung auf kostengünstigere Betriebsmittel.
    *   Statistische Auswertungen basierend auf Kosten.

#### Merke
*   Mit der Kostenkalkulation können Sie Personalkosten, Maschinenkosten und sonstige Kosten ermitteln.
*   Lohn- und Maschinenkosten werden pro Maschine in A+W Capacity Planner hinterlegt.
*   Materialkosten werden im ERP-System hinterlegt und berechnet.

### Definition der Kostenkalkulation

Für logische Maschinen können Sie die Kosten angeben, die bei der Produktion entstehen. Wird ein Auftrag oder ein Angebot eingelastet, meldet A+W Production die Kosten an das ERP-System zurück. Damit kann der Auftragserfasser die Produktionskosten anfragen, die bei der Produktion entstehen. Die Materialkosten werden im ERP-System hinterlegt und berechnet.

*(Abbildung: Screenshot des Dialogs 'Kostenkalkulation'.)*
*   **A** Physikalische Maschine
*   **B** Zugeordnete logische Maschine

Sie geben die Kosten pro Stunde und logischer Maschine ein. Damit können Sie die Kosten einer physikalischen Maschine unterschiedlich gewichten, je nachdem, welche logische Maschine angesprochen ist. Pro logischer Maschine geben Sie Maschinenkosten, Lohnkosten und sonstige Kosten separat an.

> **Beispiel**
> Auf Ihrer einseitigen Schleifmaschine können unterschiedliche Kantenbearbeitungen ausgeführt werden, z. B. Schleifen, Polieren und Gehren. Sie wird insbesondere für Modelle verwendet, wobei die Gehrung auch für Rechtecke gemacht wird.
>
> Die unterschiedlichen Arbeitsgänge sind nicht nur als unterschiedliche Bearbeitungen angelegt, sondern auch als unterschiedliche logische Maschinen.
>
> Die Maschinenwerkzeuge für die möglichen Bearbeitungen haben unterschiedliche Kosten für die Werkzeugstandzeit und für die Wiederbeschaffung. Diese Unterschiede bilden Sie über die Kosten der logischen Maschinen ab, die zu der physikalischen Maschine definiert sind.
>
> Gleichzeitig können Sie die unterschiedlichen Geschwindigkeiten bei der Bearbeitung in verschiedenen Vorgabezeiten berücksichtigen.

### Kosten anlegen und verwalten

In dieser Lerneinheit erfahren Sie, wie Sie Kosten für logische Maschinen anlegen, bearbeiten oder löschen.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So legen Sie Kosten für eine logische Maschine an" auf Seite E-529
*   "So bearbeiten Sie Kosten für eine logische Maschine" auf Seite E-530
*   "So löschen Sie Kosten für eine logische Maschine" auf Seite E-531

#### So legen Sie Kosten für eine logische Maschine an
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Kostenkalkulation**.
    Der Dialog **Kostenkalkulation** wird geöffnet.
2.  Klicken Sie auf **[Neu]**.
    In der Liste wird eine Zeile mit der Maschine -1 eingefügt.
    *(Screenshot des Dialogs 'Kostenkalkulation' mit einer neuen leeren Zeile.)*
3.  Klicken Sie doppelt auf das Feld **-1 (A)**.
    Der Dialog **Bitte wählen Sie eine Maschine aus** wird geöffnet.
4.  Übernehmen Sie die gewünschte Maschine mit einem Doppelklick.
5.  Klicken Sie doppelt auf das leere Feld **Log. Maschine**.
    Der Dialog **Bitte wählen Sie eine Technologie aus** wird geöffnet. In der Liste sind alle logischen Maschinen aufgeführt, die zur ausgewählten Maschine definiert sind.
6.  Übernehmen Sie die gewünschte logische Maschine mit einem Doppelklick.
7.  Geben Sie die Lohnkosten pro Stunde für einen Werker ein.
    Wenn für den Arbeitsgang zwei Personen erforderlich sind, müssen Sie die doppelten Kosten eintragen.
8.  Wiederholen Sie Schritt 7 für die Felder **Maschinenkosten** und **Sonstige Kosten (B)**.
    Sie können einen Kommentar eintragen, z. B. um die Lohnkosten zu erklären.
9.  Klicken Sie auf **[OK]**.
    Die Daten werden gespeichert und der Dialog wird geschlossen.

#### So bearbeiten Sie Kosten für eine logische Maschine
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Kostenkalkulation**.
    *(Screenshot des Dialogs 'Kostenkalkulation' mit ausgefüllten Werten.)*
2.  Ändern Sie den Wert des jeweiligen Felds, z. B. **Sonstige Kosten**.
3.  Wiederholen Sie Schritt 2 für alle Kosten, deren Werte nicht mehr aktuell sind.
4.  Klicken Sie auf **[OK]**.
    Die Daten werden gespeichert und der Dialog wird geschlossen.

#### So löschen Sie Kosten für eine logische Maschine
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Kostenkalkulation**.
2.  Markieren Sie die Zeile, die Sie löschen wollen.
3.  Klicken Sie auf **[Löschen]**.
    Der Eintrag wird aus der Liste gelöscht.
    Falls Sie den Eintrag versehentlich gelöscht haben, brechen Sie den Vorgang mit [Ende] ab.
4.  Klicken Sie auf **[OK]**.
    Die Daten werden gespeichert und der Dialog wird geschlossen.

### Übungen
Legen Sie die Daten so an, dass sie in allen nachfolgenden Übungen zur Verfügung stehen. Wenn auf diese Weise die Daten für die Kapazitätsplanung vollständig sind, können Sie die Planung für eigene Aufträge im Produktionsmonitor testen.
*   Wählen Sie Ihre Maschine aus und erarbeiten Sie die Kosten für die zugehörigen logischen Maschinen:
    *   Welche Lohnkosten, welche Maschinenkosten und welche sonstigen Kosten fallen jeweils bei der logischen Maschine an.
*   Legen Sie die Kosten für die logische Maschine im Dialog **Kostenkalkulation** an.
*   Erfassen Sie einen Testauftrag oder ein Testangebot und lasten Sie diese auf dieser Maschine ein. Prüfen Sie die zurückgemeldeten Preise.
*   Bearbeiten Sie die Kosten der logischen Maschinen im Dialog **Kostenkalkulation**.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Kostenkalkulation" auf Seite E-683

---
### Übergangszeiten

#### Lernziele
*   Was sind Übergangszeiten?
*   Wie werden Übergangszeiten angelegt, bearbeitet oder gelöscht?

#### Nutzen
Übergangszeiten bilden die zeitliche Bewegung der Scheiben durch die Produktion ab.

#### Merke

| Begriff | Definition |
| :--- | :--- |
| **Übergangszeit** | Eine Übergangszeit beschreibt die Spanne zwischen den Endzeitpunkten aufeinanderfolgender Bearbeitungen. Wenn zwei aufeinanderfolgende Arbeitsgänge auf derselben Maschine gearbeitet werden, entstehen keine Übergangszeiten, z. B. Bohren und Waschen. Übergangszeiten werden ausschließlich zu logischen Maschinen definiert. |
| **Übergangstyp** | Übergangszeiten werden als drei verschiedene Typen definiert: Normal, Eilübergang, minimaler Übergang. |
| **Normaler Übergang** | Normale Übergänge beschreiben den optimalen Produktionsablauf, d. h., ohne Ausfälle von Personal oder Maschinen, Bruch usw. |
| **Eilübergang** | Eilübergänge beschreiben beschleunigte Durchläufe, z. B., indem die Verweilzeiten verkürzt werden. Diese Übergangszeiten erhöhen jedoch die Kosten. |
| **Minimaler Übergang** | Minimale Übergänge sind die teuersten Übergangszeiten. |
| **Übergangszeit 0** | Bearbeitungen, die direkt aufeinanderfolgen, haben keine Übergangszeiten, z. B. Rahmenbiegen - ISO-Linie - ISO versiegeln. Bei diesen Bearbeitungen sind alle drei Typen von Übergangszeiten identisch. |
| **Expliziter Übergang** | Als expliziten Übergang definieren Sie den Übergang von Maschine x zu Maschine y. |
| **Hierarchische Auswertung** | Die hinterlegten Übergangszeiten werden in folgender Reihenfolge ausgewertet: <ul><li>Maschine x -> Maschine y.</li><li>Maschine x -> Alle Maschinen.</li><li>Alle Maschinen -> Maschine x.</li><li>Alle Maschinen -> Alle Maschinen.</li></ul> |
| **Verweilzeiten** | Verweilzeiten bezeichnen Zeiten, die ohne eigentliche Bearbeitung verlaufen, z. B. zur Scheibensortierung, Wartezeit auf Nachläufer, Trocknungszeiten. Notwendige Verweilzeiten können nicht beschleunigt werden, z. B. die Zeiten für Heat Soak. Verweilzeiten werden mit in die Übergangszeiten eingerechnet. |
| **Rüstzeit** | Rüstzeiten werden mit in die Übergangszeiten eingerechnet. |
| **Kundenhandlingzeit** | Damit ist die Zeit gemeint, die zum Verladen der verpackten Ware benötigt wird. In der Regel wird dafür ein Arbeitstag angesetzt. Für die Beladung eines Containers können aber auch mehrere Tage benötigt werden. Diese Zeit wird nicht in die Terminoptimierung eingerechnet und daher auch nicht als Übergangszeit definiert. Sie wird im ERP-System in den Stammdaten des Kunden hinterlegt. |

### Übergangszeiten in Schichten oder Stunden

Mit Übergangszeiten definieren Sie die Zeit zwischen zwei Bearbeitungen oder zwei (logischen) Maschinen. Diese Zeiten variieren je nachdem, von welcher Maschine eine Scheibe kommt und zu welcher Maschine sie geht.

Die einfachste Form der Übergangszeit ist die Zeit für den Weg, die eine Scheibe von einer (logischen) Maschine zur nächsten benötigt, z. B. der Übergang vom Zuschnitt zur nächsten Bearbeitung. Diese Zeiten werden als optimale Übergänge mit dem Typ Normal definiert. Wenn der Übergang beschleunigt werden kann, wird zusätzlich die Zeit mit dem Typ Eil und/oder Minimal angelegt.
⇨ "Übergangstypen" auf Seite E-539

*(Abbildung E-19: Rückwärtskalkulation mit normalen Übergangszeiten, zeigt den Ablauf einer Scheibe durch verschiedene Stationen über mehrere Tage und Schichten.)*
*   **A** Alternative - mit oder ohne Beschichtung
*   **B** Übergangszeit innerhalb einer Schicht
*   **C** Übergang von 2 Schichten

In diesem Beispiel sehen Sie den optimalen Ablauf mit den normalen Übergangszeiten für eine ISO-Scheibe mit einer beschichteten Scheibe. Wenn in dem ISO nur eine Scheibe beschichtet (A) wird, teilt sich der Zuschnitt auf zwei Schichten auf, damit die zu beschichtende Scheibe früher geschnitten wird. Da Rahmenbieger - ISO-Linie - ISO versiegeln (B) immer direkt hintereinander ausgeführt werden, fallen diese Bearbeitungen in derselben Schicht an.

Der Übergang wird jeweils vom Ende einer Schicht aus betrachtet. Der Übergang von Verpacken zum Versiegeln (C) ist z. B. mit 2 Schichten angegeben. Damit bleibt genug Spielraum innerhalb der Schicht, in der die Bearbeitung anfällt.

Jeder Übergang in eine andere Schicht erzeugt virtuelle Kosten, die um so höher ausfallen, je weiter der Übergang vom optimalen Übergang abweicht. Die Übergänge müssen also auch unter diesem Gesichtspunkt so optimal wie möglich gestaltet werden.

#### Übergangszeiten in Schichten
Maximale Übergangszeiten werden nur für normale Übergänge ausgewertet. Die anderen Übergänge werden als minimal automatisch aufgefüllt. Falls es einen Eintrag vom Typ Minimal gibt, sind schnellere Übergänge verboten. Für Eil-Übergänge genügt die Angabe der Mindestanzahl Schichten.

*(Abbildung E-20: Übergänge in Schichten, zeigt optimale, Eil- und minimale Übergangszeiten grafisch.)*
*   **A** Optimale und maximale Übergangszeit
*   **B** Eil-Übergangszeit
*   **C** Minimale Übergangszeit

In diesem Beispiel ist die normale Übergangszeit (A) auf fünf Schichten festgelegt, die maximal auf sieben erweitert werden können. Der Eil-Übergang (B) ist mit drei Schichten definiert. Das Programm kann damit automatisch auch vier Schichten berechnen.

Mit dem minimalen Übergang von genau einer Schicht (C) ist der Übergang in derselben Schicht automatisch verboten. Der Übergang von zwei Schichten wird ebenfalls automatisch mit berechnet.

Das bedeutet, dass Sie nur vier Angaben festlegen müssen: Normal mit 5 + 2, Eil mit 3 Schichten und Minimal mit 1 Schicht. Damit können sieben mögliche Schichtübergänge berechnet werden.

#### Übergangszeiten in Stunden
Die Übergangszeit in Stunden bezieht sich nicht auf Arbeitszeit, sondern auf die Kalenderzeit und wird auch so bei den virtuellen Kosten bewertet. Das Programm legt die Übergangszeiten in Stunden in aller Regel in die Arbeitszeit.
Bearbeitungstermine beziehen sich immer auf das Schichtende. Bei einer Übergangszeit von 00:00 Stunden gehen die Scheiben unmittelbar auf die nächste Maschine über, d. h. werden in derselben Schicht weiterbearbeitet.
Wenn Sie die Übergangszeit in Stunden angeben, müssen Sie eine maximale Zeit angeben. Die Wahl der maximalen Zeit bestimmt, ob Wochenenden in die Planung einbezogen werden.

> **Jede Zeitangabe bedeutet einen Wechsel der Schicht**
> Mit der ersten Minute, die Sie als Übergangszeit in Stunden angeben, wird in die nächste Schicht gewechselt.

*(Abbildung E-21: Übergänge in Stunden, zeigt Übergänge von 0h, in die nächste Schicht, zum nächsten Tag und über das Wochenende.)*
*   **A** Übergangszeit = 0
*   **B** Übergangszeit in die nächste Schicht
*   **C** Übergangszeit zum nächsten Tag
*   **D** Übergangszeit zum Wochenende

Die Schichtzeiten der unterschiedlichen Maschinen können unterschiedlich lang sein, z. B. kann der ESG-Ofen mit einer Schichtzeit von 6 Std. angegeben sein, die ISO-Linie hat dagegen 8 Std.
Wenn Sie mit solchen flatternden Schichtenden arbeiten, darf die Zeit nicht mit 8 Std. angegeben werden. Um diese Problematik zu umgehen, können Sie einfach 6 Std. (B) angeben.
Von Freitag 22 h bis Montag 14 h brauchen Sie eine Übergangszeit von mindestens 64 Std (D) für den optimalen Übergang. Nur mit dieser Übergangszeit lohnt sich das Stehenlassen des Glases über das Wochenende.
An diesem Beispiel sehen Sie, dass die Definition von Übergangszeiten in Schichten sehr viel einfacher ist als der Übergang in Stunden.

#### Schichtwechsel – Sonderfall
Die Schleifmaschine im folgenden Beispiel arbeitet in einer einzigen Schicht. Außerdem arbeitet sie sehr langsam. Wenn sie am Morgen bestückt wird, könnten die Scheiben am Schichtende zur nachfolgenden Maschine übergehen.
Die Übergangszeiten sind daher mit den folgenden Angaben definiert:
*   Normal = 0 Schicht
*   Max. = 1 Schicht
*   Eil = 1 Schicht
*   Min. = 0 Schicht

*(Abbildung E-22: Schichtwechsel in Bezug auf Maschine)*

Die Übergangszeit von 1 Schicht bezieht sich auf die Schichten der Schleifmaschine. Daraus folgt, dass der Übergang in die nächste Schicht unabhängig vom Übergangstyp immer für den folgenden Tag berechnet wird.
In diesem Fall ist es notwendig, die Übergangszeiten für die Schleifmaschine in Stunden zu definieren:
*   Normal = 0 Std.
*   Max. = 8 Std.
*   Eil = 4 Std.
*   Min. = 4 Std.

*(Abbildung E-23: Übergang in Stunden)*

Als Ergebnis dieser Einstellungen führt der maximale Übergang zum Ende der nachfolgenden Schicht auf der Folgemaschine. Die Zeiten für den Eilübergang und den minimalen Übergang führen in die Mitte der nachfolgenden Schicht.

### Definition von Übergangszeiten

Für die einzelnen logischen Maschinen legen Sie jeweils Übergangszeiten von allen Typen mit den entsprechenden Zeitangaben in Schichten an. In Ausnahmefällen können Sie auch Zeitdauern mit der Angabe in Stunden verwenden, z. B. für Trocknungszeiten.

Daneben gibt es eine Reihe von produktionsbedingten Übergangszeiten, die nicht beschleunigt werden können, z. B. für Heat Soak oder Trocknungszeiten nach dem Siebdruck.

Für den Fall, dass ein Übergang nicht zu einem Maschinenwechsel führt und kein expliziter Übergang zwischen zwei logischen Maschinen definiert ist, wird ein automatischer Übergang mit Übergangszeit 0 verwendet. Dadurch wird gewährleistet, dass unnötige Maschinenübergänge auch dann vermieden werden, wenn keine expliziten Übergänge definiert sind.
⇨ "Erstellung der Maschinenwege" auf Seite E-455

*(Abbildung E-24: Screenshot des Dialogs 'Übergangszeiten'.)*
*   **A** Station, von der die Scheibe kommt
*   **B** Station, zu der die Scheibe geht
*   **C** Art des Übergangs
*   **D** Normale Übergangszeit in Stunden
*   **E** Normale Übergangszeit in Schichten
*   **F** Maximale Übergangszeit in Stunden, Schichten

Übergangszeiten werden in der Regel in Schichten (E) definiert, können in Ausnahmefällen aber auch in Stunden (D) angegeben werden. In den Übergangszeiten müssen Handlings- und Rüstzeiten berücksichtigt werden.

*   Übergangszeiten in Schichten definieren Sie in ganzen Schichten.
*   Übergangszeiten in Stunden definieren Sie in Blöcken von vier oder acht Stunden. Das ist den Schichten Ihrer Produktion angepasst und übersichtlich. Die Übergangszeiten laufen auch über die arbeitsfreie Zeit, z. B. für das Aushärten von Silikonversiegelung übers Wochenende.

Die Übergangszeiten werden hierarchisch abgearbeitet. Dabei gilt:
*   **Maschine x -> Maschine y** beschreibt den expliziten Übergang zwischen zwei Maschinen.
*   **Maschine x -> Alle Maschinen** beschreibt den Übergang am Ausgang von Maschine x.
*   **Alle Maschinen -> Maschine x** beschreibt den Übergang am Eingang von Maschine x.
*   **Alle Maschinen -> Alle Maschinen** beschreibt den allgemeinen Übergang und wird zuletzt ausgewertet, wenn keine andere Übergangszeit gefunden wurde.

### Übergangstypen
Um die Übergangszeiten korrekt anlegen zu können, müssen Sie den optimalen Durchlauf Ihrer Produktion kennen. Das bedeutet, dass Sie genau wissen müssen, wie lange es dauert, bis die nachfolgende Bearbeitung ausgeführt werden kann. Ausgehend vom normalen (optimalen) Übergang können Sie dann bestimmen, um welche Zeit ein Übergang verkürzt werden kann.

Die verschiedenen Typen von Übergangszeiten werden folgendermaßen eingesetzt:
*   Im Typ **Normal** durchlaufen Scheiben die Produktion in der regulären Zeit, die dafür eingeplant wurde. Diese Zeiten gelten für den optimalen Produktionsablauf, d. h. ohne Ausfälle von Personal oder Maschinen, Bruch usw.
*   Im Typ **Eil** wird die Produktion einzelner Scheiben beschleunigt, z. B., indem die Verweilzeiten verkürzt werden. Diese Übergangszeiten erhöhen jedoch die Kosten.
*   Im Typ **Minimal** werden die sogenannten Chef-Aufträge durch die Produktion geführt. Dabei werden nur die Übergangszeiten berücksichtigt, die unabdingbar für die Produktion sind, z. B. Verweilzeiten im VSG-Autoklav, Trocknung von Verklebungen. Minimale Übergänge sind die teuersten Übergangszeiten.
*   Mit dem Typ **Verboten** wird ein Übergang von oder zu einer Maschine gesperrt, z. B. weil innerbetriebliche Transportwege erforderlich sind.

> **Beispiel**
> Bei einer Schleif-Bohrstraße kann mit der Einstellung **Verboten** z. B. erreicht werden, dass nur solche Scheiben auf die Bohrstation gelangen, die vorher auf der Schleifstation waren. Dazu würden Sie folgende Übergänge einrichten:
> *   Verboten: Alle Maschinen -> Bohrstation
> *   Normal: Schleifstation -> Bohrstation

### Vorbereitung der Definition von Übergangszeiten

Um die Übergangszeiten für Ihre Produktion zu ermitteln, können Sie zunächst eine Matrix erstellen. Die Matrix hilft, die Übergangszeiten zwischen den logischen Maschinen zu visualisieren.
Unterscheiden Sie zwischen der Zeit beim Weggang und der Zeit bei Ankunft:
*   Der Weggang nach dem Arbeitsprozess kann z. B. bedeuten, dass eine Scheibe nach einer Bearbeitung darauf wartet umgepackt zu werden.
*   Die Ankunft am Eingang kann sich z. B. auf Vorarbeiten beziehen.

*(Abbildung E-25: Beispiel-Matrix für Übergangszeiten)*
**Legende:**
*   **Zahl:** Übergangszeit in Stunden
*   **Grün:** Übergangszeit bei Weggang
*   **Rot:** Übergangszeit bei Ankunft

In diesem Beispiel sehen Sie, dass z. B. das Glas im Heat Soak immer acht Stunden verweilt. Daher beträgt die Übergangszeit vom Heat Soak zu allen anderen Arbeitsstationen immer 16 Stunden. Die so ermittelten Zeiten Ihrer Produktion rechnen Sie in Schichten um.

Eine solche Matrix zeigt, dass Sie nur wenige Übergangszeiten zwischen den Arbeitsstationen definieren müssen. Alle anderen können Sie mit der Einstellung **Von allen Maschinen -> Maschine X** oder **Von Maschine X -> alle anderen Maschinen** definieren.

Die Erstellung der Matrix und das Umsetzen im Dialog führen Sie am besten gemeinsam mit dem Service der A+W Software GmbH durch.

### Übergangszeiten anlegen und verwalten
In dieser Lerneinheit lernen Sie, wie Sie Übergangszeiten anlegen, bearbeiten oder löschen. Denken Sie daran, dass in den Übergangszeiten auch Rüstzeiten und Handlingszeiten berücksichtigt werden müssen.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So legen Sie eine Übergangszeit an" auf Seite E-541
*   "So bearbeiten Sie eine Übergangszeit auf Seite E-543
*   "So löschen Sie eine Übergangszeit" auf Seite E-543

> **Voraussetzung**
> Um Übergangszeiten anzulegen, müssen die entsprechenden logischen Maschinen in der Maschinenzuordnung definiert sein.

#### So legen Sie eine Übergangszeit an
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Übergangszeiten**.
2.  Klicken Sie auf **[Neu]**.
    *(Screenshot des Dialogs 'Übergangszeiten' mit einer neuen Zeile.)*
    In der Liste der Maschinen wird oben eine neue Zeile eingefügt.
3.  Klicken Sie doppelt in das Feld **(B)**, um den Dialog zur Auswahl der Maschine zu öffnen.
4.  Übernehmen Sie die gewünschte Maschine mit einem Doppelklick.
5.  Wiederholen Sie den Schritt für die Maschine **(C)**, zu der Sie den Übergang festlegen.
    Nutzen Sie auch die Möglichkeiten **Alle Maschinen** auf Maschine X und Maschine X auf **Alle Maschinen**.
6.  Wählen Sie den Typ **(D)** für die Übergangszeit aus und tragen Sie die zugehörige Zeit **(E)** ein.
    Verwenden Sie bevorzugt Schichten. In Ausnahmefällen können Sie auch Zeitdauern verwenden, z. B. Trockungszeiten.
7.  Tragen Sie die maximale Übergangszeit **(F)** ein.
    Damit erlauben Sie dem System, die Übergangszeit maximal zu dehnen. Verwenden Sie auch hier entweder Stunden oder Schichten.

> **Tipp**
> Wählen Sie für den Übergang zur letzten Bearbeitung, z. B. Verpacken oder Versand, die größte Übergangszeit, die möglich ist. Damit haben Sie in kritischen Situationen größere Flexibilität.

8.  Wiederholen Sie die Schritte 2 bis 7 für den nächsten Übergangstyp **(D)** derselben Maschinenkombination.
9.  Klicken Sie auf **[OK]**, um die Daten zu speichern.
    Damit haben Sie die Übergangszeiten in den verschiedenen Übergangstypen für einen Übergang angelegt.

#### So bearbeiten Sie eine Übergangszeit
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Übergangszeiten**.
2.  Korrigieren Sie die Übergangszeiten für die gewünschten Maschinen.
    Sie aktivieren die Felder mit einem Doppelklick.
3.  Ergänzen Sie ggf. eine Maschinenkombination, indem Sie die Daten für einen anderen Übergangstyp anlegen.
    Folgen Sie dazu der Beschreibung in der Handlungssequenz zum Anlegen der Übergangszeiten.
4.  Klicken Sie auf **[OK]**, um die Änderungen zu speichern.
    Damit haben Sie die Übergangszeiten geändert.

#### So löschen Sie eine Übergangszeit
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Übergangszeiten**.
2.  Markieren Sie in der ersten Spalte die Übergangszeit, die Sie löschen wollen.
    Die gesamte Zeile der Übergangszeit wird markiert.
    *(Screenshot des Dialogs 'Übergangszeiten' mit markierter Zeile.)*
3.  Klicken Sie auf **[Löschen]**.
    Die Übergangszeit wird aus der Liste gelöscht.
    Falls Sie eine Übergangszeit versehentlich aus der Liste gelöscht haben, klicken Sie auf [Ende].
    Wenn Sie die Meldung mit [Nein] bestätigen, wird der Dialog geschlossen, ohne die Änderung zu speichern. Die Übergangszeit steht wieder in der Liste, wenn Sie den Dialog erneut öffnen.
4.  Klicken Sie auf **[OK]**, um den Dialog zu schließen.
    Die Änderungen werden in die Datenbank übernommen.

### Übungen
Legen Sie die Daten so an, dass sie in allen nachfolgenden Übungen zur Verfügung stehen. Wenn auf diese Weise die Daten für die Kapazitätsplanung vollständig sind, können Sie die Planung für eigene Aufträge im Produktionsmonitor testen.
*   Legen Sie gemeinsam mit dem Trainer eine neue Maschine in der Maschinenzuordnung vollständig an, die Sie deutlich als Test-Maschine für die Kapazitätsplanung kennzeichnen.
*   Definieren Sie die Übergangszeiten für diese Maschine im Eil- und Normalraster.
*   Legen Sie Übergangszeiten zwischen zwei Maschinen für alle Typen von Übergangszeiten an, die für die Übergänge erforderlich sind.
*   Verändern Sie die Übergangszeiten.
*   Prüfen Sie die Ergebnisse mit einem Testauftrag im Produktionsmonitor.

**Ergänzende Informationen**
⇨ Softwarereferenz, “Übergangszeiten" auf Seite E-667

---
### Vorgabezeiten

#### Lernziele
*   Was sind Vorgabezeiten?
*   Wie werden Vorgabezeiten angelegt, bearbeitet oder gelöscht?
*   Aus welchen Elementen bestehen Vorgabezeiten?
*   Wie fließen die Elemente in Vorgabezeiten ein?
*   Wie funktioniert der Formeltest?

#### Nutzen
Mit Vorgabezeiten definieren Sie, wie lange ein Arbeitsschritt auf einer Maschine für eine Scheibe dauert. Zusammen mit den Übergangszeiten werden damit die Zeiten durch die Produktionsstationen berechnet.

#### Merke

| Begriff | Definition |
| :--- | :--- |
| **Vorgabezeit = Bearbeitungsdauer** | Mit der Vorgabezeit legen Sie fest, wie lange ein Arbeitsgang auf einer spezifischen Maschine dauert. Die Bearbeitungsdauer wird anhand von Formeln berechnet. Vorgabezeiten werden in der Maschinenzuordnung (MZO) als Bearbeitungsdauer bezeichnet. |
| **Logische Maschinen** | Vorgabezeiten werden zu den logischen Maschinen erstellt. |
| **Vorgabezeiten** | Die Vorgabezeiten werden zur Kapazitätsplanung und zur Kostenkalkulation herangezogen. |
| **Formel** | Vorgabezeiten können mit Formeln berechnet werden, um verschiedene Einflussgrößen zu berücksichtigen, z. B. Fläche, Laufmeter, Stückzahl, Dicke. Komplexe Vorgabezeiten hinterlegen Sie als Formel in der Maschinenzuordnung. |
| **Element** | Eine Zeile in einer Vorgabezeitformel, z. B. eine Dickenabhängigkeit, der Zeitanteil für die Fertigung eines Ausschnitts an einem Bearbeitungszentrum oder ein Zeitzuschlag für schwere Scheiben. Elemente können separat erfasst und getestet werden. Es gibt feste Elemente, bedingte Ausdrücke, Schwellenwerte, gewichtete Ausdrücke (freie Elemente) und Vektoren. Als benutzerdefinierte Elemente lassen sich zusätzlich Tabellen und dreidimensionale Abhängigkeiten (Würfel) verarbeiten. |

### Definition der Vorgabezeiten

Mit einer Vorgabezeit definieren Sie, wie die Dauer eines Arbeitsgangs an einer logischen Maschine berechnet wird. Basis der Berechnung ist dabei z. B. die jeweilige Fläche oder Kantenlänge in der einzelnen Auftragsposition.

*(Abbildung E-26: Screenshot des Dialogs 'Vorgabezeiten'.)*

In diesem Dialog sind die logischen Maschinen aufgelistet, über die Bearbeitungen gesteuert werden. Vorgabezeiten werden in A+W Production mit Vorgabezeitformeln festgelegt. Die Vorgabezeitformeln definieren Sie im Dialog Vorgabezeitformel.

> **Vorgabezeiten**
> Die Vorgabezeiten werden in der Maschinenzuordnung (MZO) als Bearbeitungsdauer bezeichnet. Da die Vorgabezeiten an den logischen Maschinen festgemacht werden, können Sie auch in der Maschinenordnung Formeln für Vorgabezeiten hinterlegen. Sie tun dies im MZO-Editor > Register Logische Maschine > Feld Bearbeitungsdauer.
> Diese Formeln aus der MZO können nicht im Dialog Vorgabezeiten geändert werden.

⇨ "Struktur von Vorgabezeitformeln" auf Seite E-547

### Struktur von Vorgabezeitformeln

Jede Vorgabezeitformel basiert auf einer Basiszeit, die in Sekunden angegeben ist. Vorgabezeitformeln können mit vorgegebenen Elementen definiert werden. Daneben können Sie auch eigene Elemente erstellen und in der Formel verwenden.

*(Abbildung E-27: Screenshot des Dialogs 'Vorgabezeitformel'.)*
*   **A** Elemente der Vorgabezeitformel
*   **B** Basiszeit in Sekunden
*   **C** Auswahl der Rechenoperation
*   **D** Reihenfolge der Elemente sortieren
*   **E** Multiplikator für die Bearbeitungsmenge

Mit jeder Zeile ist ein Zeitzuschlag angegeben, der entweder als Formel berechnet oder als Wert aus einer Tabelle ermittelt wird.

Sie können in einer Vorgabezeitformel mehrere unterschiedliche Elemente (A) verwenden. Dazu wählen Sie jeweils das gewünschte Element aus, geben einen Wert in Sekunden an und legen fest, wie der Wert in der Rechenoperation verwendet werden soll (C). Wichtig ist dabei, dass die Reihenfolge (D) korrekt sortiert ist. Das gilt insbesondere dann, wenn die nächste Rechenoperation auf dem Zwischenergebnis der vorausgegangenen Operation aufbaut.

Die Basiszeit gilt dabei als Startwert. Alle weiteren Elemente der Formel sind daher Zuschläge auf den Startwert. Wenn Sie keine Basiszeit eintragen, bauen alle Berechnungen auf dem Ergebnis des ersten Eintrags (A) auf.

Standardmäßig werden verschiedene Element zur Auswahl angeboten, die auch durch eigene Definitionen ergänzt werden können:
⇨ "Editor für Formelelemente" auf Seite E-552

#### Beispiel Gas und Modell
| Schritt | Formel | Ergebnis |
| :--- | :--- | :--- |
| Basiszeit | | 23 s |
| Faktor für Größe | | 23 * Größenfaktor |
| Faktor für Gas | | Zwischenergebnis * Gasfaktor |
| Konstante für Modell | | Zwischenergebnis + Modellkonstante |

Mit dieser Vorgabezeitformel können Sie Zeiten für Scheiben mit Gasfüllung und für Modelle berechnen. Wenn Sie aber VSG berechnen wollen, muss die Formel folgendermaßen aufgebaut werden:

#### Beispiel VSG, Größe und Gas
| Schritt | Formel | Ergebnis |
| :--- | :--- | :--- |
| Basiszeit | | 23 s |
| Faktor VSG | | + VSG-Faktor |
| Faktor für Größe | | Zwischenergebnis 1 * Größenfaktor |
| Faktor für Gas | | Zwischenergebnis 2 + (23* Gasfaktor) |

⇨ "Mögliche Einstellungen für die Vorgabezeitformel" auf Seite E-551

#### Feste Elemente
Festen Elementen wird kein Wert zugewiesen, sondern lediglich angegeben, wie sich die Elemente auf die Vorgabezeitformel auswirken. Zur Berechnung werden die tatsächlichen Werte des Glases herangezogen. So wird z. B. für das Feste Element 'Dicke' bei einer 4.00 mm dicken Scheibe der Wert 4 ermittelt. Bei dem Festen Element 'Menge' wird die Anzahl der Scheiben und bei einem Festen Element 'Fläche' wird die Fläche der Scheiben ermittelt.

Mit der Auswahl der Rechenoperation geben Sie im Dialog Vorgabezeitformeln an, wie der ermittelte Wert in der Vorgabezeitformel verwendet wird.

#### Faktoren
Mit einem Faktor können Sie einen Zeitzuschlag festlegen, der immer dann berechnet wird, wenn die Voraussetzung für die Anwendung des Faktors erfüllt ist.

> **Beispiel**
> Mit dem Faktor Wert für 'Große Scheibe' legen Sie einen Zuschlag auf die Basiszeit fest, der immer für Übergrößen berechnet wird. Ab wann eine Scheibe als Übergröße gilt, geben Sie zu dem Faktor an.

Mit der Auswahl der Rechenoperation geben Sie im Dialog Vorgabezeitformeln an, wie der ermittelte Wert in der Vorgabezeitformel verwendet wird.

#### Vektoren - Tabellen und Würfel
Vektoren ermöglichen eine exakte Planung der Vorgabezeiten in Abhängigkeit von den Werkstückeigenschaften. Mit Vektoren können Sie die Vorgabezeit z. B. auf die Glasdicke, die zu bearbeitende Fläche, die Beschaffenheit der Kanten und das Verhältnis von Breite zu Höhe einer Scheibe abstimmen.

*(Abbildung E-28: Vektor 'Dicke -> Wert' - Zeitzuschläge abhängig von der Scheibendicke)*

Unterschiedliche Dicken von Scheiben berücksichtigen Sie z. B. mit dem Vektor 'Dicke → Wert'. Damit legen Sie Zeitzuschläge abhängig von der Dicke einer Scheibe fest.

Wenn Sie den Wert im Vektor 'Dicke → Wert' als Tabelle festlegen, können Sie den Wert des Vektors staffeln, z. B. von 4.00 mm - 5.99 mm Dicke gilt der Wert 0.1, für 6.00 mm - 7.99 mm der Wert 0.2 usw.

Mit der Auswahl der Rechenoperation geben Sie im Dialog Vorgabezeitformeln an, wie Vektoren in der Vorgabezeitformel verwendet werden.

#### Eingabehilfe für Vektoren
Vektoren werden im Dialog Vektor (Name) als Tabelle definiert. Diese Tabelle enthält pro Grenzwert (Staffelstufe) einen Zuschlagswert. Zum Anlegen einer solchen Tabelle stehen zwei Vorgehensweisen zur Verfügung:
*   Sie geben die Werte einzeln in die Tabelle ein. Dabei legen Sie z. B. mehrere Stufen von Dicken, Längen oder Gewichten fest und weisen diesen jeweils einen Wert zu.
*   Sie lassen sich die Staffelstufen und die gestaffelten Werte berechnen.

*(Abbildung E-29: Eingabehilfe für Vektoren – Resultat)*

Für diese Berechnung legen Sie einen Anfangs- und einen Endwert fest, z. B. 4.00 - 20.00 mm für die Dicke. Wenn Sie als Schrittgröße 2.00 mm angeben, wird zwischen dem Anfangs- und dem Endwert alle 2.00 mm eine Stufe eingefügt.

Wenn Sie als Startwert für den Zuschlag 0.1 und als Schrittgröße 0.1 angeben, gilt für die erste Stufe der Wert 0.1, für alle weiteren Stufen wird dieser Wert jeweils um 0.1 erhöht.

Für die Tabelle ergibt sich daraus: Scheiben mit einer Dicke von 4,00 - 5,99 mm haben den Wert 0.1, von 6.00 mm - 8.00 mm den Wert 0.2 usw.

#### Berechnung von Zeitzuschlägen
Im einfachsten Fall besteht eine Vorgabezeitformel lediglich aus einer Basiszeit. Sie können z. B. für eine logische Maschine eine Basiszeit von 30 Sekunden angeben. Damit ist festgelegt, dass jeder beliebige Arbeitsgang an dieser logischen Maschine 30 Sekunden dauert.
In der Praxis ist die Dauer eines Arbeitsgangs jedoch von verschiedenen Einflüssen abhängig, z. B. von der Dicke einer Scheibe oder von der Kantenlänge, die bearbeitet werden muss. Je dicker eine Scheibe und je länger die zu bearbeitende Kantenlänge, desto mehr Zeit nimmt ein Arbeitsgang in Anspruch.

Um diese Abhängigkeiten zu berücksichtigen, können Sie Zeitaufschläge festlegen. In der Vorgabezeitformel stehen dazu feste Elemente und/oder Vektoren zur Verfügung.

Für die Vorgabezeitformel stehen folgende Elemente zur Wahl:
*   Basiszeit oder Startwert.
*   Zeitzuschlag als festes Element, z. B. die Glasdicke.
*   Zeitzuschlag als fester Wert, z. B. für große Scheiben.
*   Zeitzuschlag als Vektor, z. B. Staffelung nach Gewicht.
*   Zeitzuschlag als Tabelle für Matrix, z. B. Kantenlänge.
Basiszeit und Zeitzuschläge werden in Sekunden angegeben.

#### Reihenfolge der Berechnungen
Bei der Berechnung müssen Sie die Operatorrangfolge der Mathematik berücksichtigen: Multiplikation und Division werden vor Addition und Subtraktion gerechnet - es sei denn, Klammern geben die Reihenfolge vor.

**Beispiel**
| Formel | Ergebnis | Erklärung |
| :--- | :--- | :--- |
| `1 + 2 * 4` | `= 9` | Multiplikation zuerst |
| `(1 + 2) * 4` | `= 12` | Klammer zuerst |
| `1 + (2 * 4)` | `= 9` | |
| `4 * (1 + 2)` | `= 12` | |
| `6 + (9 / 3)` | `= 9` | |
| `(6 + 9) / 3` | `= 5` | |

Zur Berechnung der Zeitzuschläge stehen folgende Einstellungen zur Wahl:

| Einstellung | Bedeutung |
| :--- | :--- |
| **+ Tabelle** | Der Wert aus der Tabelle wird zum Zwischenergebnis addiert. |
| **+ b * Wert** | Die Basiszeit wird mit dem Wert multipliziert. Das Ergebnis der Multiplikation wird zum Zwischenergebnis addiert. |
| **+ Wert** | Der Wert wird zum Zwischenergebnis addiert. |
| *** (1 + Wert)** | Der Wert wird zu 1 addiert und das Ergebnis mit dem Zwischenergebnis aus der vorausgehenden Zeile multipliziert. |
| *** Vektor** | Das Ergebnis der vorausgehenden Zeile wird mit dem Wert des Vektors multipliziert. |

*(Tabelle E-1: Mögliche Einstellungen für die Vorgabezeitformel)*

Wenn die Berechnung mit der Ermittlung aus einer Formel beginnt, legen Sie als Startwert 0 fest, z. B. für die Berechnung einer Fläche, bevor der erste Siebdruck aufgetragen wird.

Wenn die Berechnung auf dem Ergebnis der vorausgehenden Zeile basiert, ist die Reihenfolge der Einträge wichtig.

### Editor für Formelelemente
Für die Definition eigener Formelelemente steht ein Editor zur Verfügung, in dem Sie eigene Formeln anlegen oder eine vordefinierte Formel auswählen können.

*(Abbildung E-30: Screenshot des Dialogs 'Zeitformelelement erfassen'.)*
*   **A** Name des Formelelements
*   **B** Auswahl des Typs
*   **C** Beschriftung
*   **D** Berechnungsformel
*   **E** Eingabeformat
*   **F** Unabhängiger Parameter

Dem Formelelement geben Sie einen Namen (A), der in der Auswahl der Formelelemente angezeigt wird, und eine Beschriftung (C), die im Dialog Vorgabezeitformel angezeigt wird. Die zweite Beschriftung wird vor dem Berechnungswert angezeigt.

Die unterschiedlichen Elementtypen (B) verwenden Sie für folgende Berechnungen:
*   **Festes Element:** Ausdrücke ohne Benutzereingabe, z. B. Langkante. Diese Einstellung sollten Sie nicht mehr für neue Definitionen verwenden. Sie ist durch **Freies Element** abgelöst worden.
*   **Bedingung:** Ausdrücke mit einer Benutzereingabe, die verwendet wird, wenn die Bedingung wahr ist.
*   **Freies Element:** Ausdrücke, bei denen das Ergebnis mit der Benutzereingabe gewichtet wird, z. B. Sekunden pro Schleifmeter.
*   **Schwellenwert:** Ausdrücke, bei denen der Schwellenwert für die Bedingung einstellbar ist, ohne die Formeldefinition zu verändern, z. B. Mengenzuschlag ab Benutzereingabe.
*   **Vektor:** Ausdrücke, bei denen eine Tabelle mit Wertepaaren aus Mindestwerten und zu verwendenden Koeffizienten gepflegt wird.

Die eigentliche Formeldefinition (D) des Elements können Sie als Formel schreiben oder eine vordefinierte Formel auswählen und anpassen. Bei Vektoren können Sie die Definition nicht ändern, daher ist das Feld ausgeblendet.

### Beispiel – Vorgabezeit für die logische Maschine Zuschnitt
Aus einer Produktionsstatistik haben Sie die Flächenabhängigkeit Ihres Zuschnitts ermittelt. Außerdem wissen Sie, dass die Rundbogenmodelle im Schnitt 20 Sekunden länger dauern und der Tisch 10% mehr Zeit fürs Randentschichten von ISO-Komponenten benötigt.

Um schnell auf Produktionsveränderungen reagieren zu können, wollen Sie die komplette Vorgabezeitformel mit einem Steuerparameter auf schneller oder langsamer einstellen können.

*(Abbildung E-31: Beispiel - Vorgabezeitformel für Zuschnitt)*

| Zeile | Definition | Erklärung |
| :--- | :--- | :--- |
| **Basiszeit** | 0.95 | Der Steuerparameter steht auf 95% der Vorgabezeit, also auf schneller. |
| **Randentschichtung** | `* (1 + 0.1)` | Der Zuschlag wird nur bei einer beschichteten Scheibe für ISO berechnet. |
| **Zuschnittfläche** | `* Vektor` | Das Ergebnis wird mit den Zeiten für die Scheibenfläche multipliziert. |
| **Rundbogenmodell** | `+ 20` | Bei einem Modell mit Rundbogen werden 20 Sekunden aufgeschlagen. |
*(Tabelle E-2: Beispiel - Bedingungen der Berechnung)*

Die eigentlichen Zeiten werden in dem Vektor für die Zuschnittsfläche gepflegt, z. B.:
| Fläche (qm) | Wert (s) | Erklärung |
| :--- | :--- | :--- |
| 0.1 | 70 | bis 0.099 qm werden 70 Sekunden gerechnet |
| 0.5 | 45 | für 0.1 - 0.499 qm werden 45 Sekunden gerechnet |
| 1.0 | 60 | für 0.5 - 0.999 qm werden 60 Sekunden gerechnet |
| 2.0 | 150 | für 1.0 - 1.999 qm werden 150 Sekunden gerechnet |
| 3.0 | 210 | für 1.999 - 2.999 qm werden 210 Sekunden gerechnet |

In diesem Beispiel sehen Sie, dass für die ganz kleinen und für die großen Scheiben mehr Zeit für den Zuschnitt benötigt wird. Damit entfällt ein weiterer Größenzuschlag für den Zuschnitt. Für Flächenbearbeitungen kann ein solcher Zuschlag aber durchaus notwendig sein und muss dann an der entsprechenden logischen Maschine definiert werden.

#### Bedingung: Modell mit Rundbogen
Die Bedingung soll nur dann die Benutzereingabe als Ergebnis liefern, wenn sie wahr ist.

**Definition (Beispiel)**
`IF (($Parts_MODELL_NR >= 60 AND $Parts_MODELL_NR <= 81) OR ($Parts_MODELL_NR >= 113 AND $Parts_MODELL_NR <= 118) OR ($Parts_MODELL_NR >= 123 AND $Parts_MODELL_NR <= 125) OR ($Parts_MODELL_NR >= 133 AND $Parts_MODELL_NR <= 199)) THEN 20 END`

> **Längenangabe in der Formel**
> Beachten Sie, dass die Längenwerte in einer Formel in µm angegeben werden müssen.

#### Bedingung: Schwellenwert
Bei mehr als 11 Stück soll die Vorgabezeit 10 % kleiner sein.

**Definition (Beispiel)**
`IF ($Parts_MENGE > 11) THEN - 0.1 END`

#### Bedingung: Vektor für Modellzuschnitt
Vektoren können von Einheiten abhängig sein oder auch nicht lineare Sachverhalte darstellen. Falls Ihnen z. B. der einfache Zuschlag für Modelle mit Rundbögen nicht präzise genug ist, definieren Sie einen Vektor, mit dessen Hilfe Sie die benötigten Koeffizienten einfach und sehr präzise abfragen können.

Im Dialog zur Erfassung eines Formelelements legen Sie dazu ein neues Element mit dem Elementtyp Vektor an. Für einen gültigen Vektor wählen Sie eine Formel für den unabhängigen Parameter, z. B. `AWF_ShapeNumber`.

*(Abbildung E-32: Vektor für modellabhängige Zeitzuschläge)*
*   **A** Vektor mit unabhängigem Parameter
*   **B** Tabelle für Modellnummern

Die Tabelle erlaubt die modellabhängige Abstufung der Zuschläge. Der Eintrag der linken Spalte gibt immer den Startwert des Gültigkeitsbereichs an. Es ist gute Praxis, ein Wertepaar für 0 zu definieren, damit der Wertebereich vollständig beschrieben ist.

### Zeitformel-Objekte

Sie können die Stückliste oder Teile der Stückliste als Formelobjekte abbilden, um die Kette der Bearbeitungen darzustellen. Diese Darstellung dient dazu, die Abhängigkeiten der Bearbeitungen in der Vorgabezeitformel zu testen, z. B. um zu prüfen, wie die Bearbeitung davon abhängt, was in der Gegenscheibe gemacht wird. Formelobjekte werden zum Testen von Formeln mit logischen Mengen verwendet.

Formelobjekte sind immer auf eine bestimmte Vorgabezeitformel bezogen. Sie können nicht übergreifend verwendet werden. Sie speichern die Formelobjekte dann, wenn Sie einen Nachweis führen wollen, dass die Formel korrekt angewendet wird.

*(Abbildung E-33: Stücklistenbaum aus der Sicht der einzelnen Bearbeitungen)*
*   **A** Gesamtes Objekt speichern
*   **B** Objekt löschen
*   **C** Objekt hinzufügen
*   **D** Markiertes Objekt löschen
*   **E** Objekte

In diesem Beispiel sehen Sie die Bearbeitungsstückliste einer ISO-Scheibe. Beim Hinzufügen werden die Formelobjekte (E) nummeriert. Mit einem Doppelklick können Sie jedes Formelobjekt öffnen und umbenennen, z. B. das erste Objekt in ISO. Das ist sinnvoll, um die Struktur zu verdeutlichen. Beim Hinzufügen (C) wird unter dem markierten Objekt ein neues Objekt angelegt. Beim Löschen (D) wird das markierte Objekt mit allen Unterebenen gelöscht.

> **Gespeichertes Objekt zum Testen laden**
> Ein gespeichertes Formelobjekt kann nur für die Formel verwendet werden, zu der es angelegt wurde, z. B. um die Berechnung nach Änderungen in der Vorgabezeitformel zu testen. Daher ist es sinnvoll, beim Speichern einen sprechenden Namen zu vergeben.

Ein Beispiel für ein Formelobjekt finden Sie zum Test der Vorgabezeitformel.
⇨ "So testen Sie die Berechnung der Zeitformel" auf Seite E-564

### Vorgabezeitformeln anlegen und verwalten

In dieser Lerneinheit erfahren Sie, wie Sie Vorgabezeitformeln anlegen, bearbeiten oder löschen.

In der ersten Zeile im Dialog **Vorgabezeitformeln** können Sie Formelelemente als Vorlagen für alle Maschinen definieren. Wenn Sie für die Maschine 0 eine Zeitformel definieren, wird diese zwar in der Datenbank gespeichert, die Formel wird jedoch nicht verwendet, da der Maschine 0 in der MZO keine Bearbeitung zugewiesen ist.

> **Voraussetzung**
> Vorgabezeitformeln werden zu den logischen Maschinen definiert, die einen bestimmten Arbeitsgang ausführen. Daher müssen die entsprechenden logischen Maschinen in der Maschinenzuordnung definiert sein.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So definieren Sie eine Vorgabezeitformel" auf Seite E-558
*   "So erstellen Sie einen Vektor mit der Eingabehilfe" auf Seite E-561
*   "So löschen Sie eine Vorgabezeitformel" auf Seite E-562

> **Komplexität von Vorgabezeitformeln**
> A+W Production bietet die Möglichkeit, Vorgabezeitformeln beliebig komplex zu definieren. Somit lassen sich alle erdenklichen Sonderfälle abdecken.
> Halten Sie Vorgabezeitformeln so einfach wie möglich. Sollte in Ihrer Produktion der Einsatz einer komplexen Vorgabezeitformel nötig sein, setzen Sie sich bitte mit dem Kundenservice der A+W Software GmbH in Verbindung.

#### So definieren Sie eine Vorgabezeitformel
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Vorgabezeiten**.
    *(Screenshot des Dialogs 'Vorgabezeiten'.)*
2.  Markieren Sie die logische Maschine, für die Sie eine Vorgabezeitformel erstellen wollen.
3.  Klicken Sie auf **[Bearbeiten]**.
    Der Dialog **Vorgabezeitformel** wird geöffnet.
    Wenn für die logische Maschine bereits in der Maschinenzuordnung eine Formel zur Bearbeitungsdauer hinterlegt wurde, wird eine Warnmeldung angezeigt. Wenn Sie den Vorgang fortsetzen, wird die in der Maschinenzuordnung hinterlegte Formel überschrieben.
    *(Screenshot des Dialogs 'Vorgabezeitformel'.)*
4.  Geben Sie die Basiszeit (A) in Sekunden ein.
    Sie können entweder eine vordefinierte Formel hinzufügen (E) und die Daten speichern oder eine Formel mit Formelelementen aufbauen. In den folgenden Schritten wird der Aufbau mit Formelelementen gezeigt.
5.  Klicken Sie auf **[Neu] (D)**, um ein Element auszuwählen.
    *(Screenshot des Dialogs 'Elemente hinzufügen'.)*
6.  Wählen Sie das Element aus, z. B. einen Vektor, und übernehmen Sie die Auswahl mit **[OK]**.
    Das ausgewählte Element wird im Dialog **Vorgabezeitformel** unter der Basiszeit eingefügt.
    *(Screenshot des Dialogs 'Vorgabezeitformel' mit hinzugefügtem Element.)*
7.  Klicken Sie auf **[...] (A)**, um den Dialog zur Eingabe der Werte zu öffnen.
    Wenn Sie einen Vektor anlegen, können Sie die Grenzwerte und die Zeitwerte manuell oder über die Eingabehilfe eintragen.
    ⇨ "So erstellen Sie einen Vektor mit der Eingabehilfe" auf Seite E-561
8.  Wählen Sie den Operator (B) für die Berechnung aus.
9.  Wiederholen Sie die Schritte 5 - 8, um weitere Elemente hinzuzufügen.
10. Prüfen Sie die Reihenfolge der Formelelemente.
    Die Reihenfolge ist für die Berechnung wichtig, wenn sich der Zuschlag auf die Zwischensumme des vorausgehenden Elements bezieht.
11. Klicken Sie auf **[OK]**, um die Daten zu übernehmen.
    Der Dialog wird geschlossen. Damit haben Sie eine Vorgabezeitformel zusammengestellt. Sie können die Berechnung prüfen und mit einem Formel-Objekt eine Berechnung mit Beispielgrößen starten.
    *   "Zeitformel testen" auf Seite E-563
    *   "Zeitformel-Objekte" auf Seite E-556

#### So erstellen Sie einen Vektor mit der Eingabehilfe
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Vorgabezeiten > Vorgabezeitformel**.
2.  Geben Sie die Basiszeit in Sekunden ein.
3.  Klicken Sie auf **[Neu]** und wählen Sie ein Element aus, z. B. **Vektor 'Dicke -> Wert'**.
    *(Screenshot des leeren Vektor-Dialogs.)*
4.  Klicken Sie auf **[Eingabehilfe]**.
    *(Screenshot des Dialogs 'Eingabehilfe für Vektoren'.)*
    Zunächst geben Sie die Grenzwerte für die Staffelung (A) und dann die Werte für den Faktor (B) ein. Aus diesen Angaben wird die Tabelle erstellt.
5.  Geben Sie den Startwert und den Endwert ein, z. B. **4.00** und **20.00**.
    Diese Werte legen die kleinste und die größte Dicke fest.
6.  Geben Sie die Schrittgröße ein, z. B. **2.00**.
    Dieser Wert legt fest, in welchen Schritten die Grenzwerte für die Staffelung zwischen dem Startwert und dem Endwert berechnet werden.
7.  Geben Sie die den Startwert und die Schrittgröße für den Faktor ein, z. B **0.1**.
    Dieser Wert legt fest, um welche Größe der Faktor pro Grenzwert erhöht wird. Damit haben Sie alle notwendigen Werte eingetragen.
8.  Klicken Sie auf **[OK]**, um die Berechnung der Tabelle zu starten.
    Der Dialog **Eingabehilfe für Vektoren** wird geschlossen. Die Tabellen wird berechnet und in den Dialog 'Vektor-> Dicke' übernommen.
    Sie können die Daten korrigieren und ergänzen.
    *(Screenshot des Vektor-Dialogs mit berechneter Tabelle.)*
9.  Klicken Sie auf **[OK]**, um die Daten zu speichern.
    Der Dialog **Vektor 'Dicke -> Wert'** wird geschlossen. Die angelegte Staffelung wird in die Vorgabezeitformel übernommen.

#### So löschen Sie eine Vorgabezeitformel
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Vorgabezeiten > Vorgabezeitformel**.
2.  Markieren Sie das Element, das Sie löschen wollen.
3.  Klicken Sie auf **[Löschen]**.
4.  Wiederholen Sie die Schritte 2 und 3, bis alle Elemente in der Liste entfernt sind, die nicht mehr benötigt werden.
5.  Setzen Sie die Basiszeit auf den Wert Null.
6.  Klicken Sie auf **[OK]**, um die Daten zu speichern.
    Der Dialog wird geschlossen.
    Um eine Vorgabezeitformel insgesamt zu löschen, markieren Sie die Vorgabezeit im Dialog **Vorgabezeiten** und klicken Sie auf **[Löschen]**.

### Zeitformel testen
Im Dialog **Zeitformeltest** können Sie Formeln testen und damit die eingegebenen Werte und Berechnungseinstellungen prüfen. Sie können entweder die Formel testen, die Sie aktuell im Dialog **Vorgabezeitformel** bearbeiten, oder Sie laden eine gespeicherte Formel in den Dialog, um diese zu testen.
Der Formeltest gibt ein Ergebnis aus, das die Zeit des jeweiligen Arbeitsganges in Sekunden angibt.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So testen Sie die Zeitformel" auf Seite E-563
*   "So testen Sie die Berechnung der Zeitformel" auf Seite E-564
*   "So erstellen Sie eine Kopie der Zeitformelsyntax" auf Seite E-568

Daneben können Sie Formelobjekte definieren, die Sie zum Testen aller Formeln verwenden können. Dort geben Sie den konkreten Fall an, in dem Sie die Formel testen wollen, also z. B. die Dicke und die Breite einer Scheibe. Damit haben Sie immer die gleichen Vorgaben für den Test. Diese Funktion ist in einer separaten Einheit beschrieben.
⇨ "Zeitformel-Objekte" auf Seite E-556

#### So testen Sie die Zeitformel
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Vorgabezeiten > Vorgabezeitformel**.
    *(Screenshot des Dialogs 'Vorgabezeitformel'.)*
2.  Markieren Sie das Formelelement, das Sie testen wollen.
    Wenn Sie die gesamte Vorgabzeitformel testen wollen, müssen Sie das Element **Basic Time** markieren. Sie können aber auch jedes Element einzeln testen, indem Sie es markieren und die nachfolgenden Schritte ausführen.
3.  Klicken Sie auf **[Formeltest]**.
    *(Screenshot des Dialogs 'Zeitformeltest'.)*
4.  Klicken Sie auf **[Auswerten] (B)**.
    Das Berechnungsergebnis (A) wird angezeigt. Sie können die Formel ggf. weiter bearbeiten und korrigieren.
5.  Klicken Sie auf **[OK]**, um die Daten zu speichern.
    Um die Formel mit Scheibendaten zu testen, können Sie für den Test ein Formelobjekt anlegen und Werte eingeben.

#### So testen Sie die Berechnung der Zeitformel
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Vorgabezeiten > Vorgabezeitformel**.
    Der Dialog **Vorgabezeitformel** wird geöffnet.
2.  Klicken Sie auf **[Formeltest]**.
    *(Screenshot des Dialogs 'Zeitformeltest'.)*
3.  Klicken Sie doppelt auf das Formelobjekt (A), um den Dialog zur Eingabe der Eigenschaften zu öffnen.
    *(Screenshot des Dialogs 'Eigenschaften des Formelobjekts'.)*
4.  Geben Sie einen Namen (A) ein und wählen Sie den Typ (B) aus, z. B. Teil.
5.  Klicken Sie auf **[Hinzufügen]**.
    Die Felder in der Spalte **Eigenschaften** werden mit den Elementen vorbelegt, die in der aktuellen Vorgabezeitformel enthalten sind.
    *(Screenshot des Dialogs 'Eigenschaften des Formelobjekts' mit hinzugefügten Eigenschaften.)*
6.  Geben Sie zu jeder Eigenschaft die entsprechenden Werte ein, z. B. die Maße für Höhe und Breite.
    Beachten Sie, dass Sie die Maße in Mikrometer (µm) eingeben müssen.
7.  Klicken Sie auf **[Schließen]**, um die Daten zu speichern und den Dialog zu schließen.
    Der Dialog **Formeltest** wird wieder im Vordergrund angezeigt.
    *(Screenshot des Dialogs 'Zeitformeltest' mit Ergebnis.)*
8.  Markieren Sie das Formelobjekt, für das die Berechnung gestartet werden soll.
9.  Klicken Sie auf **[Formeltest]**.
    Das Ergebnis der Berechnung mit den eingegebenen Werten wird angezeigt. Wenn die Berechnung nicht Ihren Vorstellungen entspricht, können Sie die berechneten Werte prüfen.

#### So erstellen Sie eine Kopie der Zeitformelsyntax
1.  Testen Sie die Zeitformel wie in der vorausgehenden Handlungssequenz angegeben.
    *(Screenshot des Dialogs 'Zeitformeltest'.)*
2.  Aktivieren Sie die Checkbox **Formel anzeigen (A)**.
    *(Screenshot des Dialogs 'CAP_TF_... ' mit natürlicher und nativer Syntax.)*
    In diesem Dialog können Sie die Syntax der kompletten Formel prüfen. Um die Syntax mit Unterstützung durch den A+W-Service zu korrigieren, kopieren Sie die Syntax und senden Sie den Text an A+W.

### Übungen
*   Wählen Sie eine logische Maschine Ihrer Test-Maschinen und planen Sie auf dem Papier die Vorgabezeiten für diese logische Maschine:
    *   Welche Scheiben werden auf der logischen Maschine bearbeitet?
    *   Welche Faktoren benötigen Sie, um die Vorgabezeiten für diese Scheiben zu definieren?
    *   Wie sollen diese Faktoren in die Vorgabezeitformel einfließen?
*   Stellen Sie die Vorgabezeitformel mit den benötigten Elementen zusammen.
*   Erfassen Sie für den Eintrag 0 - Alle Maschinen verschiedene Formelelemente, z. B. einen eigenen Vektor, eine Tabelle, einen Schwellenwert.
*   Legen Sie zu einer Formel ein Formelobjekt an und testen Sie die Vorgabezeitformel, um zu prüfen, ob das Ergebnis Ihren Erwartungen entspricht.

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Vorgabezeiten" auf Seite E-646
*   ⇨ Softwarereferenz, "Vorgabezeitformel" auf Seite E-648
*   ⇨ Softwarereferenz, "Tabelle, Vektor (Name)" auf Seite E-653
*   ⇨ Softwarereferenz, "Eingabehilfe für Vektoren" auf Seite E-654
*   ⇨ Softwarereferenz, "Erfassung eines Formelelements" auf Seite E-657

---
### Maschinengruppen

#### Lernziele
*   Was sind Maschinengruppen in der Kapazitätsplanung?
*   Wie werden Maschinengruppen erstellt, bearbeitet oder gelöscht?

#### Nutzen
Mit Maschinengruppen fassen Sie Maschinen eines Bereichs zusammen und steuern über die Mitarbeiteranzahl die Kapazität der Gruppe.

#### Merke

| Begriff | Definition |
| :--- | :--- |
| **Maschinengruppen** | Mit Maschinengruppen fassen Sie Maschinen von Bereichen zusammen, z. B. Zuschnitt oder Kantenbearbeitung. |
| **Personen** | Sie weisen Maschinengruppen jeweils eine Personenanzahl zu und legen damit die Kapazität der jeweiligen Maschinengruppe fest. |
| **Schichten** | Bei Maschinen einer Maschinengruppe müssen die Schichten übereinstimmen. |
| **Engpassbetriebsmittel** | Ein Engpassbetriebsmittel kann nicht über seine Kapazität hinaus bebucht werden. Maschinen werden zu einem Engpassbetriebsmittel, wenn sie einer Maschinengruppe zugewiesen werden. |

> **Voraussetzung**
> Bei allen Maschinen, die zu einer Maschinengruppe hinzugefügt werden, müssen die Schichten übereinstimmen. Dies umfasst die Start- und die Endzeit der Schichten.

### Definition der Maschinengruppen
Sie können Maschinen zu Gruppen zusammenfassen. Maschinengruppen sind für Maschinen des gleichen Bereichs sinnvoll. So könnten Sie z. B. eine Maschinengruppe **Zuschnitt** erstellen, der Sie alle Maschinen des Zuschnitts zuordnen. Eine festgelegte Kapazität gilt dann für die gesamte Maschinengruppe, also z. B. für den Zuschnitt.

Sie können nur Maschinen zu einer Gruppe zusammenfassen, deren Schichten übereinstimmen, die also zur gleichen Zeit verfügbar sind. Maschinen, die Sie zu einer Maschinengruppe hinzufügen, werden automatisch zu einem Engpassbetriebsmittel.

*(Abbildung E-34: Screenshot des Dialogs 'Maschinengruppen'.)*
*   **A** Maschinengruppe
*   **B** Verfügbare Maschinen
*   **C** Anzahl der Personen in der Gruppe
*   **D** Zugeordnete Maschinen

Den Maschinengruppen müssen Sie jeweils eine Anzahl von Personen (C) zuordnen. A+W Production geht grundsätzlich davon aus, dass an jeder Maschine eine Person arbeitet. Wenn Sie die Anzahl der Mitarbeiter in der Gruppe reduzieren, verringert sich die verfügbare Zeit pro Maschine.

> **Beispiel**
> In der Maschinengruppe Zuschnitt mit vier Maschinen werden vier Personen angenommen.
> Wenn die 4 Mitarbeiter 40 Stunden pro Woche arbeiten, sind 4 x 40 = 160 Arbeitsstunden pro Woche verfügbar.
> Bei 3 Mitarbeitern sind nur noch 3 x 40 = 120 Arbeitsstunden pro Woche verfügbar.

### Maschinengruppen anlegen und verwalten
In dieser Lerneinheit erfahren Sie, wie Sie Maschinengruppen anlegen, bearbeiten oder löschen.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So legen Sie eine Maschinengruppe an" auf Seite E-572
*   "So bearbeiten Sie eine Maschinengruppe" auf Seite E-574
*   "So löschen Sie eine Maschinengruppe" auf Seite E-575

#### So legen Sie eine Maschinengruppe an
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Maschinengruppen**.
2.  Klicken Sie auf **[Neu]**.
    *(Screenshot des Dialogs 'Neue Maschinengruppe'.)*
3.  Geben Sie einen Namen für die Maschinengruppe ein, z. B. Zuschnitt.
4.  Klicken Sie auf **[OK]**.
    Im Feld **Maschinengruppen** wird die neue Maschinengruppe angezeigt.
5.  Markieren Sie die neue Maschinengruppe.
    In der Liste **Maschinen für Gruppe** werden alle verfügbaren Maschinen angezeigt.
6.  Markieren Sie die Maschine, die Sie zu der Gruppe hinzufügen wollen, z. B. 180 Schneidetisch 8.
7.  Klicken Sie auf den Pfeil nach rechts und bestätigen Sie die Meldung.
    Die Maschine wurde zur Gruppe hinzugefügt.
8.  Wiederholen Sie die Schritte 5 bis 7, um weitere Maschinen hinzuzufügen.
9.  Klicken Sie im Feld **Maschinengruppen** doppelt in die Spalte **Personen**.
10. Geben Sie die Anzahl der Personen ein, die in dieser Maschinengruppe arbeiten.
11. Klicken Sie auf **[OK]**, um die Daten zu speichern.
    Der Dialog wird geschlossen. Damit haben Sie die Maschinengruppe angelegt.

#### So bearbeiten Sie eine Maschinengruppe
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Maschinengruppen**.
2.  Markieren Sie im Feld **Maschinengruppen** die Maschinengruppe, die Sie bearbeiten wollen.
    In der Liste **Maschinen für Gruppe** werden auf der rechten Seite alle Maschinen angezeigt, die der Gruppe zugeordnet sind. Auf der linken Seite werden die verfügbaren Maschinen angezeigt.
3.  Markieren Sie eine Maschine, die Sie aus der Gruppe entfernen oder zur Gruppe hinzufügen wollen.
4.  Klicken Sie auf den Pfeil nach links oder den Pfeil nach rechts, um eine Maschine aus der Gruppe zu entfernen oder um sie zur Gruppe hinzuzufügen.
5.  Wiederholen Sie die Schritte 3 bis 4, um weitere Maschinen aus der Gruppe zu entfernen oder zur Gruppe hinzuzufügen.
6.  Korrigieren Sie im Feld **Maschinengruppen** die Anzahl der Personen.
7.  Klicken Sie auf **[OK]**, um die Daten zu speichern.
    Die Änderungen werden gespeichert und der Dialog wird geschlossen.

#### So löschen Sie eine Maschinengruppe
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Maschinengruppen**.
2.  Markieren Sie im Feld **Maschinengruppen** die Maschinengruppe, die Sie löschen wollen.
3.  Klicken Sie auf **[Löschen]**.
    Die Maschinengruppe wird aus der Liste entfernt. Damit ändern Sie die verfügbare Kapazität für die Einlastung.
4.  Klicken Sie auf **[OK]**, um die Daten zu speichern.
    Die Änderungen werden gespeichert und der Dialog wird geschlossen.

### Übungen
Legen Sie die Daten so an, dass sie in allen nachfolgenden Übungen zur Verfügung stehen. Wenn auf diese Weise die Daten für die Kapazitätsplanung vollständig sind, können Sie die Planung für eigene Aufträge im Produktionsmonitor testen.
*   Erarbeiten Sie, welche Maschinen Sie zu Gruppen zusammenfassen wollen.
*   Erstellen Sie mindestens eine Maschinengruppe im Dialog **Maschinengruppen**.
*   Bearbeiten Sie Ihre Maschinengruppe.
*   Löschen Sie eine Ihrer Maschinengruppen.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Maschinengruppen" auf Seite E-685

---
### Lastverteilung

#### Lernziele
*   Was ist die Lastverteilung in der Kapazitätsplanung?
*   Wie wird eine Lastverteilung erstellt, bearbeitet oder gelöscht?

#### Nutzen
Die Lastverteilung ist bei Maschinen mit einer Spezialqualifikation sinnvoll. Wenn diese Qualifikation nicht abgerufen wird, wird die Maschine für die Standardbearbeitung genutzt.

#### Merke

| Begriff | Definition |
| :--- | :--- |
| **Physikalische Maschine** | Sie können eine Lastverteilung nur für eine Maschine einrichten, die als Engpassbetriebsmittel definiert ist. Sie können z. B. auf der Maschine 30% für Modelle freihalten, die aber für Rechtecke verwendet werden dürfen, wenn keine Modelle eingelastet sind. |
| **Logische Maschinen** | Die Lastverteilung wird unter den logischen Maschinen vorgenommen, die zu derselben physikalischen Maschine definiert sind. Damit können Sie die Lastverteilung eines CNC-Centers mit z. B. den drei logischen Maschinen Sonderkanten, Ausschnitte und Bohrungen prozentual aufteilen. Diese Lastverteilung wird bei der Einlastung berücksichtigt. |
| **Engpassbetriebsmittel** | Ein Engpassbetriebsmittel kann nicht über seine Kapazität hinaus bebucht werden. |

### Definition der Lastverteilung
Die Lastverteilung wird unter den logischen Maschinen festgelegt, die zu derselben physikalischen Maschine definiert sind. Damit legen Sie den prozentualen Anteil der logischen Maschinen an der Gesamtkapazität der physikalischen Maschine fest.

Lastverteilung nutzen Sie, um zu gewährleisten, dass eine Maschine eine garantierte Mindestkapazität für Spezialaufgaben freihält, z. B. für den Modellzuschnitt. Wenn die freigehaltene Kapazität nicht für Modelle genutzt wird, können auch Rechtecke bearbeitet werden. Diese Lastverteilung ist nur bei Maschinen möglich und sinnvoll, die als Engpassbetriebsmittel definiert sind.

*(Abbildung E-35: Screenshot des Dialogs 'Lastverteilung'.)*
*   **A** Physikalische Maschine
*   **B** Bearbeitung freischalten
*   **C** Logische Maschinen
*   **D** Anteile an der Gesamtkapazität

Sie teilen die Kapazität einer Maschine auf, indem Sie den zugehörigen logischen Maschinen (C) prozentuale Anteile (D) zuordnen.

> **Beispiel**
> Eine Maschine kann Formen bearbeiten, also Rechtecke und Modelle. Damit diese Spezialqualifikation nicht von den einfacheren Rechtecken belegt wird, halten Sie z. B. 30% für Modelle frei. Diese Lastverteilung wird bei der Einlastung berücksichtigt.
> Wenn diese 30% aber nicht für Modelle gebraucht werden, können auch Rechtecke bearbeitet werden.

### Lastverteilung einrichten und bearbeiten
In dieser Lerneinheit erfahren Sie, wie Sie Lastverteilungen einrichten, bearbeiten oder löschen.

> **Voraussetzung**
> Sie können eine Lastverteilung nur für eine Maschine einrichten, die als Engpassbetriebsmittel definiert ist.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So richten Sie eine Lastverteilung ein" auf Seite E-578
*   "So bearbeiten Sie eine Lastverteilung" auf Seite E-580
*   "So löschen Sie eine Lastverteilung" auf Seite E-581

#### So richten Sie eine Lastverteilung ein
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Lastverteilung**.
2.  Wählen Sie die Maschine (A) aus, deren Kapazität Sie aufteilen wollen.
    In der Auswahl-Liste sind nur die Maschinen freigeschaltet, die als Engpassbetriebsmittel definiert sind.
    Die zugehörigen logischen Maschinen werden in der Liste angezeigt.
3.  Aktivieren Sie die Checkbox **Prüfung aktivieren (B)**, um die Felder freizuschalten.
    Die Felder der logischen Maschinen werden freigeschaltet. Ist noch keine Lastverteilung angegeben, steht in der rechten Spalte **unbegrenzt**.
4.  Klicken Sie doppelt in die rechte Spalte.
5.  Geben Sie den Prozentwert für die Kapazität ein.
6.  Wiederholen Sie die Schritte 4 bis 5, um bei allen logischen Maschinen den Anteil an der Gesamtkapazität der physikalischen Maschine einzurichten.
7.  Deaktivieren Sie die Checkbox **Prüfung aktivieren**, um versehentliche Änderungen zu verhindern.
8.  Klicken Sie auf **[OK]**, um die Daten zu speichern und den Dialog **Lastverteilung** zu schließen.
    Die Daten werden gespeichert und der Dialog wird geschlossen.

#### So bearbeiten Sie eine Lastverteilung
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Lastverteilung**.
2.  Wählen Sie die Maschine (A), deren Lastverteilung Sie bearbeiten wollen.
    In der Auswahl-Liste sind nur die Maschinen freigeschaltet, die als Engpassbetriebsmittel definiert sind.
3.  Aktivieren Sie ggf. die Checkbox **Prüfung aktivieren (B)**.
4.  Ändern Sie bei allen logischen Maschinen den Prozentwert für die Kapazität.
5.  Deaktivieren Sie ggf. die Checkbox **Prüfung aktivieren**.
6.  Klicken Sie auf **[OK]**, um die Daten zu speichern.
    Die Änderungen werden gespeichert und der Dialog wird geschlossen.

#### So löschen Sie eine Lastverteilung
1.  Wählen Sie **Stammdaten > Kapazitätsplanung > Lastverteilung**.
2.  Wählen Sie im Feld **Physikalische Maschinen** die Maschine, deren Lastverteilung Sie löschen wollen.
    Die zugehörigen logischen Maschinen werden in der Liste angezeigt.
3.  Aktivieren Sie die Checkbox **Prüfung aktivieren**.
    Die Felder werden freigeschaltet.
4.  Ändern Sie bei allen logischen Maschinen den Prozentwert für die Kapazität auf **000%**.
    In den Feldern wird **unbegrenzt** angezeigt.
5.  Deaktivieren Sie ggf. die Checkbox **Prüfung aktivieren**.
6.  Klicken Sie auf **[OK]**, um die Daten zu speichern.
    Die Änderungen werden gespeichert und der Dialog wird geschlossen. Damit haben Sie die Lastverteilung für die Maschine gelöscht.

### Übungen
Legen Sie die Daten so an, dass sie in allen nachfolgenden Übungen zur Verfügung stehen. Wenn auf diese Weise die Daten für die Kapazitätsplanung vollständig sind, können Sie die Planung für eigene Aufträge im Produktionsmonitor testen.
*   Prüfen Sie, bei welchen Ihrer Maschinen eine Lastverteilung sinnvoll ist.
*   Legen Sie ggf. zuvor weitere logische Maschinen zu Ihren Test-Maschinen an.
*   Richten Sie mindestens eine Lastverteilung ein.
*   Bearbeiten Sie eine Lastverteilung.
*   Löschen Sie eine Lastverteilung.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Lastverteilung" auf Seite E-687

# A+W Production Kapazitätsplanung Softwarereferenz

## In diesem Kapitel finden Sie folgende Themen:
*   ⇨ Überblick
*   ⇨ Einlastung
*   ⇨ Kampagnen und Reservierungen
*   ⇨ Bearbeitungen
*   ⇨ Stammdaten für Zeiten
*   ⇨ Stammdaten der Schichten
*   ⇨ Maschinen und Kosten

| Thema | Seite |
| :--- | :--- |
| **Überblick** | **E-586** |
| **Einlastung** | **E-587** |
| Produktionsmonitor | E-588 |
| Angezeigte Maschinen | E-592 |
| Einstellungen | E-593 |
| Bitte wählen Sie einen Auftrag / Lauf aus (Filtern) | E-596 |
| Filter - Aufträge | E-596 |
| Filter - Läufe | E-597 |
| Filter - Eigene Filter | E-598 |
| Neuen Filter erstellen | E-599 |
| Maschine (Name) | E-600 |
| Schichten für Maschine anpassen | E-602 |
| Schichteigenschaften | E-603 |
| Reservierungsanzeige | E-605 |
| Arbeitsplan aus Produktionsmonitor | E-606 |
| Arbeitsplan - Details | E-607 |
| Arbeitsplan - Übersicht | E-609 |
| Einlastung | E-610 |
| Stücklistenkonfiguration | E-611 |
| Aktion | E-612 |
| Umlastung | E-613 |
| Maschinenumlastung | E-618 |
| Nachbearbeitung Einlastung | E-619 |
| Fehlerhafte Aufträge | E-622 |
| Asynchrone Verarbeitung | E-623 |
| Änderung bereits verplanter Aufträge | E-624 |
| Positionssplit | E-625 |
| **Kampagnen und Reservierungen** | **E-627** |
| Kampagnen | E-628 |
| Kampagnen - Einzeltermine | E-629 |
| Kampagnen - Wöchentliche Termine | E-631 |
| Abgelaufene Reservierungen | E-632 |
| Reservierungen | E-634 |
| Reservierung für Maschine | E-637 |
| Kunde auswählen | E-638 |
| Objekt auswählen | E-639 |
| **Bearbeitungen** | **E-640** |
| Bearbeitungserzeugung | E-641 |
| Existierende Bedingung hinzufügen | E-644 |
| **Stammdaten für Zeiten** | **E-645** |
| Vorgabezeiten | E-646 |
| Vorgabezeitformel | E-648 |
| Elemente hinzufügen | E-652 |
| Tabelle, Vektor (Name) | E-653 |
| Eingabehilfe für Vektoren | E-654 |
| Formel auswählen | E-656 |
| Erfassung eines Formelelements | E-657 |
| Benutzerdefinierte Tabellenelemente | E-659 |
| Grenzwert auswählen | E-660 |
| Zeitformeltest | E-661 |
| Eigenschaften des Formelobjekts | E-663 |
| Formel (Name) | E-665 |
| Verlauf der Formelauswertung | E-666 |
| Übergangszeiten | E-667 |
| **Stammdaten der Schichten** | **E-670** |
| Schichten | E-671 |
| Schichtkalender | E-673 |
| Schichtplan | E-674 |
| Schichtregel | E-676 |
| Schichtgruppe | E-678 |
| Maschine | E-680 |
| **Maschinen und Kosten** | **E-682** |
| Kostenkalkulation | E-683 |
| Maschinengruppen | E-685 |
| Lastverteilung | E-687 |

## Überblick

Für die Planung und Organisation der Kapazitäten Ihrer Produktion steht der Dialog **Produktionsmonitor** zur Verfügung. In diesem werden die Arbeitsschichten pro Maschine angezeigt.

Die Aufträge werden positionsweise eingelastet, wobei die Einlastung pro Position erfolgreich sein muss. Wenn eine Auftragsposition nicht erfolgreich eingelastet werden kann, wird der gesamte Auftrag nicht eingelastet.

Damit die Berechnungen im Produktionsmonitor korrekt ablaufen, müssen die Stammdaten der Kapazitätsplanung eingerichtet werden. Die Beschreibung der Dialoge ist zu Themengruppen zusammengefasst. Sie folgt nicht der Anordnung der Dialoge in der Softwarereferenz.

## Einlastung

Der Produktionsmonitor ist der zentrale Kapazitäts- und Auftrags-Leitstand und der Einstiegspunkt für die Arbeitsvorbereitung, z. B. Laufbildung, Umlastung.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Produktionsmonitor" auf Seite E-588
*   "Angezeigte Maschinen" auf Seite E-592
*   "Einstellungen" auf Seite E-593
*   "Bitte wählen Sie einen Auftrag / Lauf aus (Filtern)" auf Seite E-596
*   "Neuen Filter erstellen" auf Seite E-599
*   "Maschine (Name)" auf Seite E-600
*   "Schichten für Maschine anpassen" auf Seite E-602
*   "Schichteigenschaften" auf Seite E-603
*   "Reservierungsanzeige" auf Seite E-605
*   "Arbeitsplan aus Produktionsmonitor" auf Seite E-606
*   "Einlastung" auf Seite E-610
*   "Stücklistenkonfiguration" auf Seite E-611
*   "Aktion" auf Seite E-612
*   "Umlastung" auf Seite E-613
*   "Maschinenumlastung" auf Seite E-618
*   "Nachbearbeitung Einlastung" auf Seite E-619
*   "Fehlerhafte Aufträge" auf Seite E-622
*   "Asynchrone Verarbeitung" auf Seite E-623
*   "Änderung bereits verplanter Aufträge" auf Seite E-624
*   "Positionssplit" auf Seite E-625

### Produktionsmonitor
**Anzeigen > Produktionsmonitor**
**Detailanzeige > Kontextmenü > Produktionsmonitor**

*(Abbildung E-36: Screenshot des Produktionsmonitors.)*

In diesem Dialog werden die aktuelle Planung der Produktion und die kapazitive Auslastung der Maschinen pro Arbeitsschicht angezeigt. Damit ist der Produktionsmonitor der zentrale Kapazitäts- und Auftrags-Leitstand und der Einstiegspunkt für die Arbeitsvorbereitung, z. B. Laufbildung, Umlastung.
⇨ Tutorial, "Produktionsmonitor" auf Seite E-460

#### Schaltflächen

| Symbol | Funktion | Beschreibung |
| :--- | :--- | :--- |
| *(Symbol)* | **Ausgewählte Maschinen** | ⇨ "Angezeigte Maschinen" auf Seite E-592 |
| *(Symbol)* | **Einstellungen** | ⇨ "Einstellungen" auf Seite E-593 |
| *(Symbol)* | **Anzeigeart für alle Maschinen ändern** | Auswahl der Anzeige für alle Maschinen: <ul><li>Zeit</li><li>Menge</li><li>Fläche</li><li>Gewicht</li></ul> |
| *(Symbol)* | **Anzeige ändern (Schicht, Tag, Woche)** | Ändert die Anzeige. Die Maschinenkapazität wird entweder pro Arbeitsschicht, Tag oder Woche angezeigt. |
| *(Symbol)* | **Ansicht umschalten** | Schaltet die Ansicht um. <ul><li>**Hauptansicht:** Alle Schichten im angegebenen Zeitraum werden angezeigt.</li><li>**Detailansicht:** Nur die Schichten des angegebenen Tags werden angezeigt.</li></ul> |
| *(Symbol)* | **Vergrößern, Verkleinern** | Vergrößert, verkleinert die Darstellung der Arbeitsschichten. |
| *(Symbol)* | **Ansicht aktualisieren** | Aktualisiert die Ansicht. |
| *(Pfeile)* | **Gegebene Anzahl von Tagen zurück, vor** | Verschiebt den angezeigten Zeitraum um die Anzahl der Tage vor oder zurück, die im Feld **Tage** angegeben ist. |
| *(Filter)* | **Ansicht filtern, Filter entfernen** | ⇨ "Bitte wählen Sie einen Auftrag / Lauf aus (Filtern)" auf Seite E-596 |

**Starttermin:** Öffnet den Kalender, um den Starttag für die Anzeige der Arbeitsschichten auswählen.

**Tage:** Angabe, um wie viele Tage die Anzeige mit den Schaltflächen jeweils vor- oder zurückgestellt werden soll.

**Eingabefeld Filter:** Eingabe des Filterkriteriums, die Anzeige nach Aufträgen oder Läufen zu filtern.

> **Darstellung**
> Die Darstellung kann individuell angepasst werden. Dies betrifft z. B. die Farben, ein Zeitraster, Statusinformationen usw.
> ⇨ "Einstellungen" auf Seite E-593

#### Arbeitsschichten
Im Produktionsmonitor werden die Arbeitsschichten aller ausgewählten Maschinen angezeigt. Maschinen, die als Engpassbetriebsmittel definiert sind, werden in roter Schrift angezeigt. Ein Engpassbetriebsmittel kann nicht über seine Kapazität hinaus bebucht werden.

Über das Kontextmenü stehen folgende Informationen zur Verfügung:
*   **Eigenschaften:** Öffnet einen Dialog, in dem Sie die Anzeige der Maschineneigenschaften ändern können.
    ⇨ "Maschine (Name)" auf Seite E-600
*   **Schichteigenschaften:** Öffnet einen Dialog, in dem Sie Schichtzeiten der Maschine anpassen können.
    ⇨ "Schichten für Maschine anpassen" auf Seite E-602
*   **Logische Maschinen anzeigen:** Mit diesem Eintrag kann die Darstellung der logischen Maschinen aktiviert und deaktiviert werden. Bislang musste man dazu den entsprechenden Schalter im Stammdaten-Dialog ändern. Bei Verwendung des Kontextmenüs wird nicht der in den Stammdaten hinterlegte Wert geändert, es wird nur die Anzeige angepasst, so dass die Änderung nur temporär ist.
    ⇨ "Misc" auf Seite E-601

#### Status der Planung
Die Farben der Punkte zeigen die Rückstände an:
*   **Grün:** Keine Rückstände.
*   **Gelb:** Rückstände, die mit der freien Kapazität noch am aktuellen Tag aufgeholt werden können.
*   **Rot:** Rückstände, die nicht mehr am aktuellen Tag aufgeholt werden können.

#### Anzeige der Arbeitsschichten
Im Tooltipp zu einer Arbeitsschicht wird eine Kurzinformation zum Status angezeigt.
Über das Kontextmenü stehen folgende Informationen zur Verfügung:
*   **Arbeitsplan:** Öffnet den Dialog Arbeitsplan: Selektion aus A+W Production Monitor mit dem Überblick über die Läufe und Aufträge der Maschine und Schicht.
    ⇨ "Arbeitsplan aus Produktionsmonitor" auf Seite E-606
*   **Löschen:** Löscht eine markierte Arbeitsschicht aus dem Produktionsmonitor.
*   **Schichteigenschaften:** Öffnet den Dialog Schichteigenschaften, um die Eigenschaften einer Schicht zu ändern.
    ⇨ "Schichteigenschaften" auf Seite E-603
*   **Reservierungen anzeigen:** Öffnet den Dialog Reservierungsanzeige, um die Reservierungen einer Schicht zu prüfen.
    ⇨ "Reservierungsanzeige" auf Seite E-605

**Schraffiert:** Die Dauer der Arbeitsschicht ist herabgesetzt.
**X:** Die Arbeitsschicht ist deaktiviert.
**!** Die Arbeitsschicht ist auf **Aktiv für Eilaufträge** gesetzt und steht damit nur für Eilaufträge zur Verfügung.
**?** In der Arbeitsschicht sind undefinierte Bearbeitungen eingelastet.
**Rahmen:** Die Arbeitsschicht ist als Engpass definiert.
⇨ "Schichteigenschaften" auf Seite E-603

### Angezeigte Maschinen
**Anzeigen > Produktionsmonitor > [Ausgewählte Maschinen]**

*(Abbildung E-37: Screenshot des Dialogs 'Angezeigte Maschinen'.)*

In diesem Dialog wählen Sie die Maschinen aus, die im Dialog **Produktionsmonitor** angezeigt werden. Dabei können Sie auch die Reihenfolge festlegen. Maschinen, die als Engpassbetriebsmittel definiert sind, werden in der Liste in roter Schrift angezeigt. Ein Engpassbetriebsmittel kann nicht über seine Kapazität hinaus bebucht werden.

**Checkbox:** Angabe, ob eine Maschine im Dialog **Produktionsmonitor** angezeigt wird.
*   ☐ Die Maschine wird nicht angezeigt.
*   ☑ Die Maschine wird angezeigt.

**[Pfeil nach oben], [Pfeil nach unten]:** Verschiebt die markierte Maschine um eine Stelle nach oben oder nach unten.

**[OK]:** Speichert und übernimmt die Auswahl und schließt den Dialog.

### Einstellungen
**Anzeigen > Produktionsmonitor > [Einstellungen]**

*(Abbildung E-38: Screenshot des Dialogs 'Einstellungen' – Felder nach Kategorien angezeigt.)*

In diesem Dialog können Sie die Anzeige im Dialog **Produktionsmonitor** einstellen, z. B. ob Maschinengruppen und Rückstände angezeigt werden. Außerdem können Sie die Anzeige der Farben für Arbeitsschichten, Engpässe oder Überlasten festlegen.

**[Kategorien]:** Sortiert die Elemente nach Kategorien.
**[Alphabetisch]:** Sortiert die Elemente alphabetisch.
**[Eigenschaften]:** Zur Zeit nicht genutzt.

#### Andere Einstellungen
*   **Anzahl an Tagen vor Startdatum:** Angabe, wie viele Tage vor dem aktuellen Startdatum angezeigt werden.
*   **Behandlung von Maschinengruppen:** Angabe, ob Maschinengruppen angezeigt werden.
*   **Behandlung von Rückständen:** Angabe, ob Rückstände angezeigt werden.

#### Darstellung
*   **Abgearbeitet:** Farbe, in der abgearbeitete Aufträge angezeigt werden.
*   **Aktualisierungszeit:** Angabe des Intervalls in Sekunden, in dem die Anzeige im Dialog Produktionsmonitor aktualisiert wird.
*   **Ausgewählte Schichten:** Farbe, in der die ausgewählte Arbeitsschicht angezeigt wird.
*   **Auslastung in Grafik anzeigen:** Angabe, ob die Auslastung als Text angezeigt wird.
*   **Automatische Aktualisierung:** Angabe, ob die Anzeige automatisch aktualisiert wird.
*   **Eingelastet:** Farbe, in der eingelastete Aufträge angezeigt werden.
*   **Engpass:** Farbe, in der Engpässe angezeigt werden.
*   **Engpassfarbe:** Schriftfarbe für Engpassbetriebsmittel.
*   **Farbe für Hinweissymbole:** Farbe, in der Hinweissymbole in den Arbeitsschichten angezeigt werden.
*   **Freie Reservierungszeit:** Farbe, in der unbebuchte Reservierungen angezeigt werden.
*   **Intensität des 3D-Effekts:** Auswahl, in welcher Intensität der 3D-Effekt angezeigt wird.
*   **Schicht:** Farbe, in der Arbeitsschichten angezeigt werden.
*   **Stunden anzeigen:** Angabe, ob ein Stunden-Raster hinter die Schichten gelegt wird.
*   **Überlast:** Farbe, in der eine Überlast angezeigt wird.
*   **Verplant:** Farbe, in der verplante Arbeitsschichten angezeigt werden.
*   **Verplante Arbeitsgänge:** Farbe, in der verplante Arbeitsgänge angezeigt werden.
*   **Zeit anzeigen:** Angabe, ob ein Zeitraster angezeigt wird.
*   **Zeitfarbe:** Farbe, in der die Zeit angezeigt wird.

#### Detaildarstellung
*   **Arbeitsgänge mit fertigen Vorprodukten:** Angabe, ob Arbeitsgänge mit fertigen Vorprodukten angezeigt werden.
*   **Intensität des 3D-Effekts:** Angabe der Intensität des 3D-Effekts für grafische Elemente im Produktionsmonitor.
*   **Produktionsfreigabe (mengenbasiert):** Farbe, in der mengenbasierte Produktionsfreigaben angezeigt werden.
*   **Produktionsfreigabe (zeitbasiert):** Farbe, in der zeitbasierte Produktionsfreigaben angezeigt werden.
*   **Stati anzeigen:** Auswahl, ob neben der Maschine der Status für Rückstände angezeigt wird.
*   **Unverplant (mengenbasiert):** Farbe, in der unverplante Arbeitsschichten angezeigt werden. Die Anzeige ist mengenbasiert.
*   **Unverplant (zeitbasiert):** Farbe, in der unverplante Arbeitsschichten angezeigt werden. Die Anzeige ist zeitbasiert.
*   **Verplant (mengenbasiert):** Farbe, in der verplante Arbeitsschichten angezeigt werden. Die Anzeige ist mengenbasiert.
*   **Verplant (zeitbasiert):** Farbe, in der verplante Arbeitsschichten angezeigt werden. Die Anzeige ist zeitbasiert.
*   **Vorprodukte fertig (mengenbasiert):** Farbe, in der fertige Vorprodukte angezeigt werden. Die Anzeige ist mengenbasiert.
*   **Vorprodukte fertig (zeitbasiert):** Farbe, in der fertige Vorprodukte angezeigt werden. Die Anzeige ist zeitbasiert.

**[OK]:** Speichert und übernimmt die Auswahl und schließt den Dialog.

### Bitte wählen Sie einen Auftrag / Lauf aus (Filtern)
**Anzeigen > Produktionsmonitor > [Ansicht filtern]**

In diesem Dialog können Sie Aufträge, Läufe und selbst erstellte Filter auswählen, nach denen die Ansicht im Produktionsmonitor gefiltert werden soll.
Der Dialog enthält folgende Register:
*   "Filter - Aufträge" auf Seite E-596
*   "Filter - Läufe" auf Seite E-597
*   "Filter - Eigene Filter" auf Seite E-598

#### Filter - Aufträge
**Anzeigen > Produktionsmonitor > [Ansicht filtern] > Aufträge**

*(Abbildung E-39: Screenshot des Dialogs 'Bitte wählen Sie einen Auftrag/Lauf aus – Aufträge'.)*

Im diesem Register sind die definierten Aufträge angezeigt. Sie können jeweils einen Auftrag auswählen. Die Anzeige im Produktionsmonitor wird auf den gewählten Auftrag eingeschränkt.

*   **Auftragsnummer:** Auftragsnummer, nach der gefiltert werden soll.
*   **Kunde:** Kundenname, nach dem gefiltert werden soll. Die Liste der Aufträge wird auf den Kunden eingeschränkt.
*   **Anzahl der Sätze:** Angabe, wie viele Aufträge in der Liste angezeigt werden.
*   **[OK]:** Speichert die Daten.
*   **[Verwerfen]:** Schließt den Dialog, ohne die Daten zu speichern.

#### Filter - Läufe
**Anzeigen > Produktionsmonitor > [Ansicht filtern] > Läufe**

*(Abbildung E-40: Screenshot des Dialogs 'Bitte wählen Sie einen Auftrag/Lauf aus – Läufe'.)*

In diesem Register sind die definierten Läufe angezeigt. Sie können jeweils einen Lauf auswählen. Die Anzeige im Produktionsmonitor wird auf den gewählten Lauf eingeschränkt.

*   **Laufnummer:** Laufnummer, nach der gefiltert werden soll.
*   **Laufbeschreibung:** Laufbeschreibung, nach der gefiltert werden soll. Die Liste der Läufe wird auf den Lauf eingeschränkt.
*   **Anzahl der Sätze:** Angabe, wie viele Läufe in der Liste angezeigt werden.
*   **[OK]:** Speichert die Daten.
*   **[Verwerfen]:** Schließt den Dialog, ohne die Daten zu speichern.

#### Filter – Eigene Filter
**Anzeigen > Produktionsmonitor > [Ansicht filtern] > Eigene Filter**

*(Abbildung E-41: Screenshot des Dialogs 'Bitte wählen Sie einen Auftrag/Lauf aus – Eigene Filter'.)*

In diesem Register werden die selbst definierten Filter angezeigt.

*   **[Neu]:** Öffnet den Dialog **Neuen Filter erstellen**, in dem Sie eigene Filter definieren können.
*   **[OK]:** Speichert die Daten.
*   **[Verwerfen]:** Schließt den Dialog, ohne die Daten zu speichern.

### Neuen Filter erstellen
**Anzeigen > Produktionsmonitor > [Ansicht filtern] > Register Eigene Filter > [Neu]**

*(Abbildung E-42: Screenshot des Dialogs 'Neuen Filter erstellen'.)*

In diesem Dialog können Sie eigene Filter für die Suche im Produktionsmonitor erstellen. Sie erstellen die Filter in der Datenbanksprache SQL.

> **Eigene Filter erstellen**
> Bitte wenden Sie sich an den Kundenservice der A+W Software GmbH, wenn Sie spezielle Filter zur Suche im Produktionsmonitor brauchen.

*   **Name:** Name für den Filter.
*   **Beschreibung:** Beschreibung für den Filter.
*   **SQL:** Definition des Filters in SQL.
*   **[OK]:** Speichert die Daten.
*   **[Verwerfen]:** Schließt den Dialog, ohne die Daten zu speichern.

### Maschine (Name)
**Anzeigen > Produktionsmonitor > Maschine > Kontextmenü > Eigenschaften**

*(Abbildung E-43: Screenshot des Dialogs 'Maschine (Name)'.)*

In diesem Dialog ändern Sie die Eigenschaften der Maschine im Produktionsmonitor.

*   **[Kategorien]:** Sortiert die Elemente nach Kategorien.
*   **[Alphabetisch]:** Sortiert die Elemente alphabetisch.
*   **[Eigenschaften]:** Zur Zeit nicht genutzt.

#### Eigenschaften der Maschine
*   **ID:** Identifikationsnummer der Maschine.
*   **Erfassungsstelle:** Identifikationsnummer der Erfassungsstelle.
*   **Name:** Name der Maschine.
*   **Engpass:** Auswahl, ob die Maschine ein Engpassbetriebsmittel ist. Engpassbetriebsmittel werden im Produktionsmonitor in der Liste der Maschinen in roter Schrift angezeigt.
*   **Anzeigeart:** Auswahl, in welcher Einheit die Schichtinfo den Status **Fertig** anzeigt. Zur Auswahl stehen:
    *   Prozent
    *   Menge
    *   Fläche
    *   Gewicht
    *   Laufmeter
    *   Bearbeitung
