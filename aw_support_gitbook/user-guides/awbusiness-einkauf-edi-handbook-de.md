---
title: "A+W Business Einkauf - Tutorial und Softwarereferenz"
source: "D-HB-AWBusiness_23.pdf"
tags: ["A+W Business", "Einkauf", "EDI", "openTRANS", "Dokumentenaustausch", "Rechnungskontrolle", "Bestellung", "Tutorial", "Softwareanleitung", "Wareneingang"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Dieses Dokument ist ein umfassendes Handbuch für das A+W Business Einkauf-Modul. Es enthält ein Tutorial zum elektronischen Dokumentenaustausch (EDI) mittels openTRANS und ASCII-Formaten sowie eine detaillierte Softwarereferenz für die verschiedenen Funktionen im Einkaufsprozess."
long_description: "Dieses Dokument dient als Tutorial und Softwarereferenz für Benutzer des A+W Business Einkauf-Moduls. Der erste Teil ist ein Tutorial, das den Benutzer schrittweise durch den Prozess des elektronischen Dokumentenaustauschs (EDI) führt. Es behandelt die Einrichtung des Datenaustauschs für Kunden mittels openTRANS, einschließlich der Konfiguration von Exportarten (Datei oder E-Mail) und Dokumententypen (Auftragsbestätigungen, Rechnungen). Es wird detailliert beschrieben, wie Partnerstammdaten geprüft, elektronische Dokumente (openTRANS, XML) eingelesen, geprüft und verarbeitet werden. Dies schließt die manuelle Zuordnung von Positionen, die Korrektur von Differenzen, die Erstellung von Teillieferungen und die Verteilung von Zuschlägen/Rabatten ein. Ein weiterer Abschnitt des Tutorials widmet sich dem Datenexport und -import im ASC-Format (EDI), einschließlich der notwendigen Einstellungen in den Firmen- und Partnerdaten. Der zweite Teil des Dokuments ist eine umfassende Softwarereferenz, die die einzelnen Dialoge, Menüs und Funktionen des Einkauf-Moduls detailliert beschreibt. Dies umfasst Anfragen, Bestellungen, Auftragsbestätigungen, Wareneingang, Rechnungen und deren Kontrollen. Jede Funktion wird mit Screenshots, Feld-für-Feld-Erklärungen und Verweisen auf zugehörige Prozesse erläutert, was es zu einem unverzichtbaren Nachschlagewerk für die tägliche Arbeit mit dem A+W Business Einkauf-Modul macht."
---

# Tutorial

---
## Elektronischer Dokumentenaustausch

5. Wählen Sie im Feld Typ (B) den Eintrag Standard (openTRANS basierend) aus.
   Mit dieser Einstellung erhalten die Dokumente für diesen Kunden automatisch das Kennzeichen für den openTRANS-Austausch.

6. Wählen Sie im Feld Exportart (A) aus, wie die Dateien ausgetauscht werden sollen.
    *   **Export in eine Datei:**
        Mit dieser Einstellung werden die Daten in eine Datei geschrieben. Die Felder für den Zielpfad werden freigeschaltet. Sie können ein Verzeichnis auswählen oder den Pfad manuell eintragen.
    *   **Export per E-Mail:**
        Mit dieser Einstellung werden die Daten als Anhang einer E-Mail gesendet. Dazu müssen Sie prüfen, ob in den Stammdaten des Kunden die E-Mail-Adresse korrekt eingetragen ist.
        ⇨ "Partnerstammdaten prüfen" auf Seite D-2202

7. Wählen Sie aus, ob Auftragsbestätigungen und/oder Rechnungen (D) exportiert werden sollen.

8. Wenn Sie die Daten per E-Mail senden, können Sie abweichende E-Mail-Adressen (E) für Auftragsbestätigungen, Rechnungen und/oder Lieferavis eintragen.

9. Wählen Sie im Menü Start > Speichern, um Änderungen zu speichern.
   Die Daten werden gespeichert.

10. Wiederholen Sie die Schritte 3 bis 9 für alle Kunden, mit denen Sie Daten austauschen.
    Um Auftragsbestätigungen und Rechnungen Ihrer Lieferanten importieren zu können, brauchen Sie keine weiteren Einstellungen festzulegen.

## Partnerstammdaten prüfen

In den Stammdaten der Lieferanten/Kunden müssen die Daten für die Kommunikation korrekt hinterlegt sein, damit Dokumente direkt aus A+W Business heraus versendet werden können.

### So prüfen Sie die Lieferanten-/Kundendaten

1.  Wählen Sie Stammdaten > Marktpartner > Lieferant, Kunde > Lieferanten, Kunden.

    