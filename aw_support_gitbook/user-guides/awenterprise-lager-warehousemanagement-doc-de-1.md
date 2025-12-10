---
title: "DE_AWEnterprise_Lager_HelpCards"
source: "DE_AWEnterprise_Lager_HelpCards.pdf"
tags: ["A+W Enterprise", "Lager", "Warehouse Management", "Inventory Management", "ERP", "Help Cards", "User Guide", "Stammdaten", "Glass Software", "Windows and Doors"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides a series of 'Help Cards' for the A+W Enterprise Lager (Warehouse) module. It offers step-by-step instructions for various warehouse management tasks, including master data setup, goods receipt and issue, inventory control, and system administration."
long_description: "This is a comprehensive user guide for the A+W Lager module within the A+W Enterprise software suite, specifically for version 2015. The guide is structured as a collection of 'Help Cards,' each dedicated to a specific function or workflow. It covers all major aspects of warehouse management. The main sections include: Stammdatenverwaltung (Master Data Management) for setting up warehouses and articles; Lagerverwaltung (Warehouse Management) for daily operations like goods receipt, goods issue, and handling different storage types (e.g., bin locations, crates, racks); Inventurverwaltung (Inventory Management) for performing stocktakes; Bewertung (Valuation) for article pricing; and an Infosystem for retrieving data and generating reports. Each help card clearly outlines the goal, prerequisites, additional information, and a detailed, numbered workflow to guide the user through the software's interface. This document is essential for users who manage inventory, process stock movements, and administer the A+W Lager system."
---

# A+W Lager: Help Cards für A+W Enterprise

Die Darstellungen in den Help Cards basieren auf der Auslieferversion A+W Enterprise 2015. Einzelne Schritte in den Workflows können je nach Konfiguration abweichen.

---
## Inhaltsverzeichnis

### Stammdatenverwaltung
| Help Card | Themen |
|---|---|
| Lagerraum anlegen | Ein Lager und alle zugehörigen Stammdaten definieren. |
| Lagerartikel festlegen | Lagerartikel pro Lager verwalten. |

### Lagerverwaltung
| Help Card | Themen |
|---|---|
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

### Inventurverwaltung
| Help Card | Themen |
|---|---|
| Inventur im Lager durchführen | Inventur eines Lagers durchführen. |

### Bewertung
| Help Card | Themen |
|---|---|
| Bewertung im Lager vornehmen | Bewertung von Artikelpreisen vornehmen. |

### Infosystem
| Help Card | Themen |
|---|---|
| Infos zu Artikeln einsehen | Informationen zu Artikeln des Lagers einsehen. |
| Lagerhistorie einsehen | Informationen zu den Buchungen in der Lagerhistorie einsehen. |
| Aufträge / Bestellungen einsehen | Informationen zu auftrags- und bestellbezogenen Buchungen einsehen. |
| Buchungsstatus einsehen | Nicht gebuchte oder fehlerhafte Buchungen einsehen und korrigieren. Übersicht für alle Lager in Inventur aufrufen. |
| Dispositiven Lagerbestand einsehen | Bestellten, verplanten und verfügbaren Lagerbestand einsehen. |
| Bestandsprognose einsehen | Bestandsprognose für verplante Lagerbestände eines Zeitraums einsehen. |

### Druck
| Help Card | Themen |
|---|---|
| Kistenetiketten drucken | Kistenetiketten für offene Druckaufträge drucken. |

### System
| Help Card | Themen |
|---|---|
| Lagerprotokoll löschen | Lagerprotokoll im System löschen. |
| Durchschnittspreis korrigieren | Durchschnittspreis für eingekauften Lagerartikel korrigieren. |

---

## Stammdatenverwaltung

### Lagerraum anlegen (SD 01-001)

**Ziel der Handlung**
Ein Lager und alle zugehörigen Stammdaten definieren.

**Voraussetzungen**
(Keine)

**Zusatzinfo**
Die Strukturierung der Lagerstammdaten anhand des Lagers ist wohlüberlegt zu definieren, da nachträgliche Änderungen nur mit hohem Aufwand durchgeführt werden können. Bei Unklarheiten unbedingt Rücksprache mit der A+W Software GmbH halten.

**Workflow**
1.  Menü `Stammdaten > Raum` wählen.
    Dialog `Lagerraumverwaltung` wird geöffnet.
2.  Mindestens die folgenden Stammdaten für das neue Lager eingeben:
    *   Lagernummer eingeben.
    *   Bezeichnung und Kurzbezeichnung des Lagers eingeben.
    *   Mandant (im Haus) wählen.
    *   Inventurart wählen.
    *   Lagerart wählen.
3.  Definition mit [OK] bestätigen.

**Nächster Schritt:** Lagerartikel festlegen.

### Lagerartikel festlegen (SD 01-002)

**Ziel der Handlung**
Lagerartikel pro Lager verwalten.

**Voraussetzungen**
*   Lager ist in den Stammdaten angelegt.
*   Artikel mit Varianten ist mit der Beschaffungsart Lager in den Stammdaten angelegt.

**Zusatzinfo**
*   Lager anlegen: `A+W Enterprise > LAGER > Stammdaten > Raum`.
*   Artikel anlegen: `A+W Enterprise > A+W Enterprise > Stammdaten > Artikel`.

**Workflow**
1.  Menü `Stammdaten > Artikel` wählen.
    Dialog `Artikelstammdaten Lager` wird geöffnet.
2.  Artikel und Lager wählen.
3.  Artikelvariante wählen.
4.  Bestandsgrenze für die Bestellvariante in den Spalten `Mindest`, `Alarm` und `Maximal` eingeben.
5.  Bestandsgrenzen pro Artikelvariante eingeben.
6.  Bei Bedarf, pro Variante eine Bemerkung mit `<F5>` erfassen.
7.  Definitionen der Bestandsgrenzen mit `<Ende>` speichern.

---

## Lagerverwaltung

### Lagereingang buchen (LA 01-001)

**Ziel der Handlung**
Artikel im Lagereingang buchen.

**Voraussetzungen**
*   Standardlager ist in den Stammdaten angelegt.
*   Artikelstammdaten sind vollständig erfasst.
*   Je nach Systemkonfiguration müssen die Artikel dem gewählten Haus zugeordnet sein.

**Zusatzinfo**
*   Mit `<F5>` aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
*   Mit `<Ende>` die Eingaben im Fußbereich speichern und in den Rumpfbereich wechseln.
*   Buchungen können im Dialog `Buchungskorrektur` korrigiert werden.
    ⇨ Buchungskorrektur buchen

**Workflow**
1.  Menü `Buchung > Eingang` wählen. Dialog `Lagereingang` wird geöffnet.
2.  Artikel und Lager wählen.
3.  Artikelvariante, Artikelmenge und Einkaufspreis pro Stück oder pro Mengeneinheit eingeben. Gesamtpreis der Position wird angezeigt. Detailangaben der Position werden im Fußbereich angezeigt.
4.  Detailinformationen im Fußbereich prüfen.
5.  Schritte 3 und 4 für nächste Artikelvariante wiederholen.
6.  Buchung bestätigen. Artikel werden im Lager eingebucht.

**Buchung prüfen:**
7.  Menü `Infosystem > Buchungsstatus > Ungebucht: Nicht gebuchte Buchungen`.
8.  Menü `Infosystem > Buchungsstatus > Fehler: Fehlerhafte Buchungen`.
9.  Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
10. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
11. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
12. Buchungsdaten prüfen.

### Lagerausgang buchen (LA 01-002)

**Ziel der Handlung**
Artikel im Lagerausgang buchen.

**Voraussetzungen**
*   Standardlager ist in den Stammdaten angelegt.
*   Artikelstammdaten sind vollständig erfasst.
*   Benötigte Menge an Artikeln befindet sich auf Lager.

**Zusatzinfo**
*   Mit `<F5>` aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
*   Mit `<Ende>` die Eingaben im Fußbereich speichern und in den Rumpfbereich wechseln.
*   Buchungen können im Dialog `Buchungskorrektur` korrigiert werden.
    ⇨ Buchungskorrektur buchen

**Workflow**
1.  Menü `Buchung > Ausgang` wählen. Dialog `Lagerausgang` wird geöffnet.
2.  Artikel und Lager wählen.
3.  Artikelvariante und Artikelmenge in Stückzahl oder Mengeneinheit eingeben. Gesamtpreis der Position wird angezeigt. Detailangaben der Position werden im Fußbereich angezeigt.
4.  Detailinformationen im Fußbereich prüfen.
5.  Schritte 3 und 4 für nächste Artikelvariante wiederholen.
6.  Buchung bestätigen. Artikel werden vom Lager abgebucht.

**Buchung prüfen:**
7.  Menü `Infosystem > Buchungsstatus > Ungebucht: Nicht gebuchte Buchungen`.
8.  Menü `Infosystem > Buchungsstatus > Fehler: Fehlerhafte Buchungen`.
9.  Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
10. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
11. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
12. Buchungsdaten prüfen.

### Fachlagereingang buchen (LA 01-003)

**Ziel der Handlung**
Artikel im Fachlagereingang buchen.

**Voraussetzungen**
*   Fachlager ist in den Stammdaten angelegt.
*   Artikelstammdaten sind vollständig erfasst.
*   Je nach Systemkonfiguration müssen die Artikel dem gewählten Haus zugeordnet sein.

**Zusatzinfo**
*   Mit `<F5>` aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
*   Mit `<Ende>` die Eingaben im Fußbereich speichern und in den Rumpfbereich wechseln.
*   Buchungen können im Dialog `Buchungskorrektur` korrigiert werden.
    ⇨ Buchungskorrektur buchen

**Workflow**
1.  Menü `Buchung > Facheingang` wählen. Dialog `Fachlagereingang` wird geöffnet.
2.  Artikel und Lager wählen.
3.  Artikelvariante, Artikelmenge und Einkaufspreis pro Stück oder pro Mengeneinheit eingeben. Gesamtpreis der Position wird angezeigt. Detailangaben der Position werden im Fußbereich angezeigt.
4.  Detailinformationen im Fußbereich prüfen.
5.  Schritte 3 bis 4 für nächste Artikelvariante wiederholen.
6.  Buchung bestätigen. Artikel werden im Lager eingebucht.

**Buchung prüfen:**
7.  Menü `Infosystem > Buchungsstatus > Ungebucht: Nicht gebuchte Buchungen`.
8.  Menü `Infosystem > Buchungsstatus > Fehler: Fehlerhafte Buchungen`.
9.  Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
10. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
11. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
12. Buchungsdaten prüfen.

### Fachlagerausgang buchen (LA 01-004)

**Ziel der Handlung**
Artikel im Fachlagerausgang buchen.

**Voraussetzungen**
*   Fachlager ist in den Stammdaten angelegt.
*   Artikelstammdaten sind vollständig erfasst.
*   Benötigte Menge an Artikeln befindet sich auf Lager.

**Zusatzinfo**
*   Mit `<F5>` aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
*   Mit `<Ende>` die Eingaben im Fußbereich speichern und in den Rumpfbereich wechseln.
*   Buchungen können im Dialog `Buchungskorrektur` korrigiert werden.
    ⇨ Buchungskorrektur buchen

**Workflow**
1.  Menü `Buchung > Fachausgang` wählen. Dialog `Fachlagerausgang` wird geöffnet.
2.  Artikel und Lager wählen.
3.  Artikelvariante und Artikelmenge in Stückzahl oder Mengeneinheit eingeben. Gesamtpreis der Position wird angezeigt. Detailangaben der Position werden im Fußbereich angezeigt.
4.  Detailinformationen im Fußbereich prüfen.
5.  Schritte 3 und 4 für nächste Artikelvariante wiederholen.
6.  Buchung bestätigen. Artikel werden vom Lager abgebucht.

**Buchung prüfen:**
7.  Menü `Infosystem > Buchungsstatus > Ungebucht: Nicht gebuchte Buchungen`.
8.  Menü `Infosystem > Buchungsstatus > Fehler: Fehlerhafte Buchungen`.
9.  Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
10. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
11. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
12. Buchungsdaten prüfen.

### Kistenlagereingang buchen (LA 01-005)

**Ziel der Handlung**
Komplette Kiste im Kistenlagereingang buchen.

**Voraussetzungen**
*   Kistenlager ist in den Stammdaten angelegt.
*   Artikelstammdaten sind vollständig erfasst.
*   Je nach Systemkonfiguration müssen die Artikel dem gewählten Haus zugeordnet sein.

**Zusatzinfo**
*   Mit `<F5>` aus einer Spalte in die kistenbezogenen Angaben im Fußbereich wechseln.
*   Mit `<Shift>` + `<F8>` aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
*   Mit `<Ende>` die Eingaben im Fußbereich speichern und in den Rumpfbereich wechseln.

**Workflow**
1.  Menü `Buchung > Kisteneingang` wählen. Dialog `Kistenlagereingang` wird geöffnet.
2.  Artikel und Kistenlager wählen.
3.  Artikelvariante wählen.
4.  Kistenbezeichnung und Verpackungsart eingeben.
5.  Artikelmenge und Artikelpreis des Lieferanten eingeben.
6.  Schritte 3 bis 5 für nächste Kiste wiederholen.
7.  Buchung mit [OK] bestätigen. Kisten werden vom Lager abgebucht.

**Buchung prüfen:**
8.  Menü `Infosystem > Buchungsstatus > Ungebucht: Nicht gebuchte Buchungen`.
9.  Menü `Infosystem > Buchungsstatus > Fehler: Fehlerhafte Buchungen`.
10. Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
11. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
12. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
13. Buchungsdaten prüfen.

### Kistenlagerausgang buchen (LA 01-006)

**Ziel der Handlung**
Komplette Kiste im Kistenlagerausgang buchen.

**Voraussetzungen**
*   Kistenlager ist in den Stammdaten angelegt.
*   Artikelstammdaten sind vollständig erfasst.
*   Benötigte Menge an Artikeln befindet sich auf Lager.

**Zusatzinfo**
*   Mit `<F5>` aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
*   Mit `<Ende>` die Eingaben im Fußbereich speichern und in den Rumpfbereich wechseln.
*   Buchungen können im Dialog `Buchungskorrektur` korrigiert werden.
    ⇨ Buchungskorrektur buchen

**Workflow**
1.  Menü `Buchung > Kistenausgang` wählen. Dialog `Kistenlagerausgang` wird geöffnet.
2.  Artikel und Kistenlager wählen.
3.  Kiste mit der entsprechenden Artikelvariante wählen und `<F4>` drücken. Zusatzmenü wird angezeigt.
4.  Menü `Kisten > Kiste abbuchen` wählen. Dialog `Achtung` wird geöffnet.
5.  Abfrage, ob die Kiste aus dem Lager entfernt werden soll mit [Ja] bestätigen.
6.  Schritte 3 bis 5 für nächste Kiste wiederholen.
7.  Buchung mit [OK] bestätigen. Kisten werden vom Lager abgebucht.

**Buchung prüfen:**
8.  Menü `Infosystem > Buchungsstatus > Ungebucht: Nicht gebuchte Buchungen`.
9.  Menü `Infosystem > Buchungsstatus > Fehler: Fehlerhafte Buchungen`.
10. Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
11. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
12. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
13. Buchungsdaten prüfen.

### Einzelblattkistenlager einbuchen (LA 01-007)

**Ziel der Handlung**
Einzelne Glasblätter in das Einzelblattkistenlager buchen.

**Voraussetzungen**
*   Einzelblattkistenlager ist in den Stammdaten angelegt.
*   Artikelstammdaten sind vollständig erfasst.
*   Je nach Systemkonfiguration müssen die Artikel dem gewählten Haus zugeordnet werden.

**Zusatzinfo**
*   Mit `<F5>` aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
*   Mit `<Strg>` + `<E>` die Einzelblattinformationen bearbeiten.
*   Buchungen können im Dialog `Buchungskorrektur` korrigiert werden.
    ⇨ Buchungskorrektur buchen

**Workflow**
1.  Menü `Buchung > Kisteneingang` wählen. Dialog `Kistenlagereingang` wird geöffnet.
2.  Artikel und Einzelblattkistenlager wählen.
3.  Artikelvariante wählen.
4.  Kistenbezeichnung eingeben. Cursor wechselt in die Tabelle zur Erfassung der Einzelblätter in die Spalte `Blatt`.
5.  Daten für einzelne Glasscheibe eingeben.
6.  Schritt 5 so oft wiederholen, bis alle Glasscheiben der Kiste erfasst sind.
7.  Variante fertig erfassen.
8.  Buchung mit [OK] bestätigen. Einzelblätter werden ins Einzelblattkistenlager gebucht.

**Buchung prüfen:**
9.  Menü `Infosystem > Buchungsstatus > Ungebucht: Nicht gebuchte Buchungen`.
10. Menü `Infosystem > Buchungsstatus > Fehler: Fehlerhafte Buchungen`.
11. Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
12. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
13. Buchungsdaten prüfen.

**Weitere Glasscheiben in bestehende Einzelblattkiste einbuchen:**
14. Schritte 1 bis 3 wiederholen.
15. Kiste auswählen.
16. Mit `<Strg>` + `<E>` in die Tabelle zur Erfassung der Einzelblätter wechseln.
17. Mit `<F6>` neue Blattnummer anlegen.
18. Schritte 5 bis 13 ausführen.

### Einzelblattkistenlager ausbuchen (LA 01-008)

**Ziel der Handlung**
Einzelblattkiste auflösen und Glasblätter der Einzelblattkiste auf ein anderes Lager buchen.

**Voraussetzungen**
*   Einzelblattkistenlager ist in den Stammdaten angelegt.
*   Artikelstammdaten sind vollständig erfasst.
*   Benötigte Menge an Glasblättern befinden sich auf Lager.

**Zusatzinfo**
*   Mit `<F5>` aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
*   Mit `<Strg>` + `<E>` die Einzelblattinformationen bearbeiten.
*   Buchungen können im Dialog `Buchungskorrektur` korrigiert werden.
    ⇨ Buchungskorrektur buchen

**Workflow**
1.  Menü `Buchung > Kistenausgang` wählen. Dialog `Kistenlagerausgang` wird geöffnet.
2.  Artikel und Einzelblattkistenlager wählen.
3.  Variante wählen.
4.  Mit `<Strg>` + `<E>` in die Einzelblattinformationen wechseln.
5.  Mit `<F7>` einzelne Positionen löschen. Ausgewähltes Blatt wird aus der Einzelblattkiste gelöscht. Wenn das letzte verbliebene Blatt der Einzelblattkiste gelöscht wird, wird die Einzelblattkiste automatisch gelöscht.
6.  Mit [OK] führen Sie die Buchung aus.

**Buchung prüfen:**
7.  Menü `Infosystem > Buchungsstatus > Ungebucht: Nicht gebuchte Buchungen`.
8.  Menü `Infosystem > Buchungsstatus > Fehler: Fehlerhafte Buchungen`.
9.  Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
10. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
11. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
12. Buchungsdaten prüfen.

### Gestelllagereingang buchen (LA 01-009)

**Ziel der Handlung**
Artikel auf Gestellen in ein Gestelllager buchen.

**Voraussetzungen**
*   Gestelllager ist in den Stammdaten angelegt.
*   Artikelstammdaten sind vollständig erfasst.
*   Je nach Systemkonfiguration müssen die Artikel dem gewählten Haus zugeordnet werden.
*   Fächer müssen als Erfassungsstellen aus dem Produktionssystem an A+W Enterprise übergeben werden.

**Zusatzinfo**
*   Buchungen können im Dialog `Buchungskorrektur` korrigiert werden.
    ⇨ Buchungskorrektur buchen

**Workflow**
1.  Menü `Buchung > Gestelleingang` wählen. Dialog `Gestelllagereingang` wird geöffnet.
2.  Entweder Artikel und Gestelllager oder das Gestell wählen.
3.  Artikelvariante wählen.
4.  Gestell wählen oder neues Gestell anlegen.
5.  Fach für das Gestell wählen.
6.  Buchungsmenge der Variante in Mengeneinheit eingeben.
7.  Schritte 3 und 4 für weitere Artikelvarianten wiederholen.
8.  Buchung mit [OK] bestätigen. Artikel werden in das Gestelllager eingebucht.

**Buchung prüfen:**
9.  Menü `Infosystem > Buchungsstatus > Ungebucht: Nicht gebuchte Buchungen`.
10. Menü `Infosystem > Buchungsstatus > Fehler: Fehlerhafte Buchungen`.
11. Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
12. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
13. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
14. Buchungsdaten prüfen.

### Gestelle auftragsbezogen ausbuchen (LA 01-010)

**Ziel der Handlung**
Auftragsbezogene Lagerabgänge im Gestelllager buchen.

**Voraussetzungen**
*   Gestelllager ist in den Stammdaten angelegt.
*   Artikelstammdaten sind vollständig erfasst.
*   Gestell mit den entsprechenden Artikelvarianten befindet sich auf Lager.

**Zusatzinfo**
*   Mit `<F2>` zwischen dem Register `Auftragsbezogen` und `Umbuchung` wechseln.
*   Mit `<Shift>` + `<F8>` eine Position auflösen und in ein anderes Lager buchen.
*   Buchungen können im Dialog `Buchungskorrektur` korrigiert werden.
    ⇨ Buchungskorrektur buchen

**Workflow**
1.  Menü `Buchung > Gestellausgang` wählen. Dialog `Gestelllagerausgang` wird geöffnet.
2.  Entweder Artikel und Gestelllager wählen oder das Gestell.
3.  Register `Auftragsbezogen` wählen.
4.  Variante auf dem Gestell wählen.
5.  Buchungsmenge der Variante in Mengeneinheit eingeben.
6.  Auftragsnummer eingeben.
7.  Positionsnummer im Auftrag eingeben.
8.  Schritte 4 bis 7 für weitere auftragsbezogene Buchungen wiederholen.
9.  Buchung mit [OK] bestätigen. Artikel werden vom Gestelllager abgebucht.

**Buchung prüfen:**
10. Menü `Infosystem > Buchungsstatus > Ungebucht: Nicht gebuchte Buchungen`.
11. Menü `Infosystem > Buchungsstatus > Fehler: Fehlerhafte Buchungen`.
12. Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
13. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
14. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
15. Buchungsdaten prüfen.

### Gestelllager Artikel umbuchen (LA 01-011)

**Ziel der Handlung**
Artikelvarianten auf ein neues Gestell bzw. neues Fach umbuchen.

**Voraussetzungen**
*   Gestelllager ist in den Stammdaten angelegt.
*   Artikelstammdaten sind vollständig erfasst.
*   Gestell mit den entsprechenden Artikelvarianten befindet sich auf Lager.

**Zusatzinfo**
*   Mit `<F2>` zwischen dem Register `Auftragsbezogen` und `Umbuchung` wechseln.
*   Mit `<Shift>` + `<F8>` eine Position auflösen und in ein anderes Lager buchen.
*   Buchungen können im Dialog `Buchungskorrektur` korrigiert werden.
    ⇨ Buchungskorrektur buchen

**Workflow**
1.  Menü `Buchung > Gestellausgang` wählen. Dialog `Gestelllagerausgang` wird geöffnet.
2.  Entweder Artikel und Gestelllager wählen oder das Gestell.
3.  Register `Umbuchung` wählen.
4.  Variante auf dem Gestell wählen.
5.  Buchungsmenge der Variante in Mengeneinheit eingeben.
6.  Neues Gestell eingeben.
7.  Neues Fach eingeben.
8.  Schritte 4 bis 7 für weitere Umbuchungen wiederholen.
9.  Buchung mit [OK] bestätigen. Artikel werden vom Gestelllager abgebucht.

**Buchung prüfen:**
10. Menü `Infosystem > Buchungsstatus > Ungebucht: Nicht gebuchte Buchungen`.
11. Menü `Infosystem > Buchungsstatus > Fehler: Fehlerhafte Buchungen`.
12. Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
13. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
14. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
15. Buchungsdaten prüfen.

### Auftragsbezogene Ausgänge buchen (LA 01-012)

**Ziel der Handlung**
Auftragsbezogene Lagerabgänge manuell buchen.

**Voraussetzungen**
*   Bestandsänderung des Artikels im Artikelstamm ist als manuelle Buchung definiert worden.
*   Lager ist in den Stammdaten angelegt.
*   Artikelstammdaten sind vollständig erfasst.
*   Benötigte Menge an Artikeln befinden sich auf Lager.

**Zusatzinfo**
*   Mit `<F2>` die Spalte `Termin` für den Liefertermin der Position anzeigen.
*   Mit `<F3>` die Buchung auslösen.
*   Buchungen können im Dialog `Buchungskorrektur` korrigiert werden.
    ⇨ Buchungskorrektur buchen

**Workflow**
1.  Menü `Buchung > Ausgang (Auftragsbezogen)` wählen. Dialog `Lagerausgang (Auftragsbezogen)` wird geöffnet.
2.  Auftrag wählen. Positionen des Auftrags werden angezeigt.
3.  Position des Auftrags zum Ausbuchen wählen.
4.  Stückzahl des Artikels eingeben.
5.  Schritt 3 und 4 für weitere auftragsbezogene Buchungen wiederholen.
6.  Buchung mit `<F3>` auslösen. Auftragsbezogene Artikel werden vom Lager abgebucht.

**Buchung prüfen:**
7.  Menü `Infosystem > Buchungsstatus > Ungebucht: Nicht gebuchte Buchungen`.
8.  Menü `Infosystem > Buchungsstatus > Fehler: Fehlerhafte Buchungen`.
9.  Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
10. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
11. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
12. Buchungsdaten prüfen.

### Stapellagereingang buchen (LA 01-013)

**Ziel der Handlung**
Neue Stapel im Stapellagereingang buchen.

**Voraussetzungen**
*   Stapellager ist in den Stammdaten angelegt.
*   Artikelstammdaten sind vollständig erfasst.
*   Je nach Systemkonfiguration müssen die Artikel dem gewählten Haus zugeordnet werden.

**Zusatzinfo**
*   Mit `<Shift>` + `<F8>` vom System eine neue Stapelnummer vergeben lassen.
*   Mit `<Strg>` + `<F12>` den ausgewählten Stapel einbuchen.
*   Buchungen können im Dialog `Buchungskorrektur` korrigiert werden.
    ⇨ Buchungskorrektur buchen

**Workflow**
1.  Menü `Buchung > Stapeleingang` wählen. Dialog `Stapellagereingang` wird geöffnet.
2.  Stapellager und Lieferant wählen.
3.  Mit `<Shift>` + `<F8>` eine neue Stapelnummer anlegen.
4.  Artikelvariante, Artikelmenge und Einkaufspreis pro Stück oder pro Mengeneinheit eingeben. Gesamtpreis der Position wird angezeigt. Detailangaben der Position werden im Fußbereich angezeigt.
5.  Schritte 3 und 4 für nächsten Stapel wiederholen.
6.  Buchung mit `<Ende>` bestätigen. Stapel werden in das Stapellager eingebucht.

**Buchung prüfen:**
7.  Menü `Infosystem > Buchungsstatus > Ungebucht: Nicht gebuchte Buchungen`.
8.  Menü `Infosystem > Buchungsstatus > Fehler: Fehlerhafte Buchungen`.
9.  Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
10. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
11. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
12. Buchungsdaten prüfen.

### Änderung im Stapellager buchen (LA 01-014)

**Ziel der Handlung**
*   Artikel auf bestehende Stapel buchen.
*   Stapel auflösen und Artikel aus dem Stapellager buchen.

**Voraussetzungen**
*   Stapellager ist in den Stammdaten angelegt.
*   Artikelstammdaten sind vollständig erfasst.
*   Eingangsbuchung für ausgewählte Artikel in Stapeln ist bereits erfolgt.

**Zusatzinfo**
*   Mit `<Strg>` + `<F8>` den ausgewählten Stapel auflösen und die Artikel des Stapels auf ein anderes Lager buchen.
*   Mit `<Strg>` + `<F12>` den ausgewählten Stapel ausbuchen.
*   Buchungen können im Dialog `Buchungskorrektur` korrigiert werden.
    ⇨ Buchungskorrektur buchen

**Workflow**
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

**Buchung prüfen:**
11. Menü `Infosystem > Buchungsstatus > Ungebucht: Nicht gebuchte Buchungen`.
12. Menü `Infosystem > Buchungsstatus > Fehler: Fehlerhafte Buchungen`.
13. Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
14. Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
15. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
16. Buchungsdaten prüfen.

### Buchungskorrektur buchen (LA 01-015)

**Ziel der Handlung**
Buchungen im Lager korrigieren.

**Voraussetzungen**
*   Lagerdaten sind durch das Lagerbuchungssystem angelegt worden.

**Zusatzinfo**
*   Mit `<F5>` zwischen dem Dialog `Übersicht` und `Detailansicht` der ausgewählten Position wechseln.
*   Mit `<Shift>` + `<F12>` für den aktuellen Buchungssatz ein neues Datum eingeben.

**Workflow**
1.  Menü `Buchung > Korrektur` wählen. Dialog `Buchungskorrektur` wird geöffnet.
2.  Filterkriterien eingeben. Trefferliste der Suche wird angezeigt.
3.  Mengen / Anzahl und / oder Preis in den Spalten korrigieren.
4.  Mit `<F5>` die Detailansicht des ausgewählten Datensatzes öffnen.
5.  Buchungskorrektur mit `<Ende>` bestätigen. Menge / Anzahl und / oder der Preis werden korrigiert und gebucht.

**Buchungen prüfen:**
6.  Menü `Infosystem > Buchungsstatus > Ungebucht: Nicht gebuchte Buchungen`.
7.  Menü `Infosystem > Buchungsstatus > Fehler: Fehlerhafte Buchungen`.
8.  Menü `Infosystem > Historie > Filterkriterium eingeben > <F3>`.
9.  Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
10. Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen.
11. Buchungsdaten prüfen.

---

## Inventurverwaltung

### Inventur im Lager durchführen (IV 01-001)

**Ziel der Handlung**
Inventur eines Lagers durchführen.

**Voraussetzungen**
*   Die Inventur eines Lagers kann nur durchgeführt werden, wenn seit der letzten Inventur mindestens eine Ausgangsbuchung oder eine Eingangsbuchung ausgeführt wurde.

**Zusatzinfo**
*   Inventuren für die anderen Lagerarten werden auf die gleiche Weise in folgenden Dialogen durchgeführt: `Inventur > Kistenlager, Fachlager, Stapellager, Gestelllager`.
*   Zur Inventur freigeschaltete Lagernummern werden vom System mit einem negativen Vorzeichen gekennzeichnet.
*   Eine Inventur ist immer nur für ein Lager möglich (von Lager = bis Lager). Wenn ein Wertebereich eingegeben wird, verzweigt das Programm in den Bewertungsmodus.

**Workflow**
1.  Menü `Inventur > Lager` wählen. Dialog `Inventur` wird geöffnet.
2.  Bereichsgrenzen für Artikel wählen in: `von Artikel`, `bis Artikel`.
3.  In beiden Feldern für die Lagernummer dieselbe Lagernummer eines Lagers wählen.
4.  Abfrage zur Freischaltung der Inventur mit [Ja] bestätigen. Standardlager ist zur Inventur freigeschaltet.
5.  Ist-Bestand beim Bedarf pro Artikel bzw. Artikelvariante korrigieren.
6.  Mit `<Shift>` + `<F8>` Inventur abschließen. Inventur wird abgeschlossen.

**Inventur auf Abschluss prüfen:**
7.  Menü `Infosystem > Buchungsstatus > Inventur`. Dialog `Buchungsstatus` wird geöffnet.
8.  Lagernummern für offene Inventuren werden aufgelistet.

---

## Bewertung

### Bewertung im Lager vornehmen (BW 01-001)

**Ziel der Handlung**
Bewertung von Artikelpreisen vornehmen.

**Voraussetzungen**
*   Ausgewähltes Lager darf nicht zur Inventur freigeschaltet sein.
*   Die Bewertung eines Lagers kann nur durchgeführt werden, wenn seit der letzten Bewertung mindestens eine Ausgangsbuchung oder eine Eingangsbuchung ausgeführt wurde.

**Zusatzinfo**
*   Bewertungen für die anderen Lagerarten werden auf die gleiche Weise in folgenden Dialogen durchgeführt: `Bewertung > Kistenlager, Fachlager, Gestelllager, Stapellager`.
*   Eine Bewertung kann nur durchgeführt werden, wenn das betreffende Lager zur Inventur / Bewertung freigeschaltet ist. Zur Bewertung freigeschaltete Lagernummern werden vom System mit einem negativen Vorzeichen gekennzeichnet.

**Workflow**
1.  Menü `Bewertung > Lager` wählen. Dialog `Bewertung` wird geöffnet.
2.  Bereichsgrenzen für Artikel wählen in: `von Artikel`, `bis Artikel`.
3.  In beiden Feldern für die Lagernummer dieselbe Lagernummer eines Lagers wählen.
4.  Abfrage zur Vorbereitung der Bewertung mit [Ja] bestätigen. Artikelvarianten des Standardlagers werden aufgelistet.
5.  Gesamtpreis im Feld `Preis` bei Bedarf korrigieren.
6.  Mit `<Shift>` + `<F8>` Bewertung abschließen. Bewertung wird abgeschlossen.

---

## Infosystem

### Infos zu Artikeln einsehen (IS 01-001)

**Ziel der Handlung**
Informationen zu Artikeln des Lagers einsehen.

**Voraussetzungen**
*   Lagerdaten zu den ausgewählten Suchkriterien müssen im System vorhanden sein.

**Zusatzinfo**
Informationen zu Artikelvarianten, Fächer, Stapeln und Einzelblättern werden in der gleichen Weise in folgenden Dialogen aufgelistet: `Infosystem > Variante, Fach, Gestell, Stapel, Blatt`.

**Workflow**
1.  Menü `Infosystem > Artikel` wählen. Dialog `Info-Lager-Artikel` wird geöffnet.
2.  Ein oder mehrere Filterkriterien eingeben und mit `<F3>` die Suche starten. Trefferliste wird angezeigt.
3.  Mit `<F2>` gegebenenfalls weitere Informationen anzeigen lassen.
4.  Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen. Detailansicht wird geöffnet.

### Lagerhistorie einsehen (IS 01-002)

**Ziel der Handlung**
Informationen zu den Buchungen in der Lagerhistorie einsehen.

**Voraussetzungen**
(Keine)

**Zusatzinfo**
(Keine)

**Workflow**
1.  Menü `Infosystem > Historie` wählen. Dialog `Info-Lager-Historie` wird geöffnet.
2.  Ein oder mehrere Filterkriterien eingeben und mit `<F3>` die Suche starten. Trefferliste wird angezeigt.
3.  Mit `<F5>` die Detailansicht des ausgewählten Datensatzes öffnen. Detailansicht wird geöffnet.

### Aufträge / Bestellungen einsehen (IS 01-003)

**Ziel der Handlung**
Informationen zu auftrags- und bestellbezogenen Buchungen einsehen.

**Voraussetzungen**
*   Aufträge / Bestellungen enthalten Lagerartikel.

**Zusatzinfo**
(Keine)

**Workflow**
1.  Menü `Infosystem > Aufträge/Bestellungen` wählen. Dialog `Aufträge/Bestellungen` wird geöffnet.
2.  Ein oder mehrere Filterkriterien eingeben und mit `<F3>` die Suche starten. Trefferliste wird angezeigt.
3.  Mit `<F5>` die Detailansicht des ausgewählten Datensatzes der Trefferliste öffnen. Detailansicht wird geöffnet.

### Buchungsstatus einsehen (IS 01-004)

**Ziel der Handlung**
*   Nicht gebuchte oder fehlerhafte Buchungen einsehen und korrigieren.
*   Übersicht für alle Lager in Inventur aufrufen.

**Voraussetzungen**
(Keine)

**Zusatzinfo**
Informationen zum Buchungsstatus für fehlerhafte Datensätze und für die Inventur werden in der gleichen Weise in folgenden Dialogen aufgelistet: `Infosystem > Buchungsstatus > Fehler`, `Inventur`.

**Workflow**
1.  Menü `Infosystem > Buchungsstatus > Ungebucht` wählen. Dialog `Buchungsstatus` für ungebuchte Datensätze wird geöffnet.
2.  Mit `<F5>` die Detailansicht des ausgewählten Datensatzes öffnen. Detailansicht wird angezeigt.
3.  Daten korrigieren.
4.  Mit `<Strg>` + `<F8>` nach der Korrektur der Fehlerursache den Fehlerstatus zurücksetzen.
5.  Mit `<Shift>` + `<F8>` den Lagerbucher aktivieren.
6.  Mit `<Ende>` Korrektur speichern. Korrektur wird gespeichert und der Dialog geschlossen.

### Dispositiven Lagerbestand einsehen (IS 01-005)

**Ziel der Handlung**
Bestellten, verplanten und verfügbaren Lagerbestand einsehen.

**Voraussetzungen**
(Keine)

**Zusatzinfo**
(Keine)

**Workflow**
1.  Menü `Infosystem > Dispositiver Bestand` wählen. Dialog `Dispositiver Bestand` wird geöffnet.
2.  Filterkriterien im Kopfbereich eingeben und bestätigen. Übersicht des Lagerbestands wird angezeigt.

### Bestandsprognose einsehen (IS 01-006)

**Ziel der Handlung**
Bestandsprognose für verplante Lagerbestände eines Zeitraums einsehen.

**Voraussetzungen**
(Keine)

**Zusatzinfo**
(Keine)

**Workflow**
1.  Menü `Infosystem > Prognose` wählen. Dialog `Bestandsprognose` wird geöffnet.
2.  Filterkriterien im Kopfbereich eingeben und bestätigen. Übersicht der Bestandsprognose wird angezeigt.
3.  Mit `<F5>` die Auftragsnummer oder Bestellnummer des ausgewählten Datensatzes anzeigen lassen.
4.  Mit `<Shift>` + `<F5>` Grafik vom Bestandsverlauf anzeigen lassen.

---

## Druck

### Kistenetiketten drucken (DR 01-001)

**Ziel der Handlung**
Kistenetiketten für offene Druckaufträge drucken.

**Voraussetzungen**
(Keine)

**Zusatzinfo**
*   Im Lagereingang wird für jede Kiste automatisch ein Druckauftrag zum Etikettendruck angelegt.
*   Im Dialog `Kistenetiketten drucken` wird in der Spalte `ohne Name` angezeigt, ob der Druckauftrag zum Etikettendruck freigeschaltet ist oder nicht.

**Workflow**
1.  Menü `Druck > Etiketten` wählen. Dialog `Kistenetiketten drucken` wird geöffnet.
2.  Wenn ein Kistenetikett nicht gedruckt werden soll, muss mit `<Leertaste>` die Kennzeichnung in der Spalte `ohne Namen` von `J` auf `N` umgestellt werden.
3.  Etikettendruck mit `<Shift>` + `<F3>` bestätigen. Etiketten werden gedruckt.

---

## System

### Lagerprotokoll löschen (SY 01-001)

**Ziel der Handlung**
Lagerprotokoll im System löschen.

**Voraussetzungen**
(Keine)

**Zusatzinfo**
Nach dem Löschen des Lagerprotokolls werden die entsprechenden Sätze nicht mehr unter `Infosystem > Historie` angezeigt.

**Workflow**
1.  Menü `System > Lagerprotokoll löschen` wählen. Dialog `Lagerprotokoll löschen` wird geöffnet.
2.  Daten eingeben, zu denen das Lagerprotokoll gelöscht werden soll.
3.  Lagerprotokoll mit `<F3>` löschen. Lagerprotokoll wird gelöscht.
