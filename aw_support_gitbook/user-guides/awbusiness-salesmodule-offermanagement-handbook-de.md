---
title: "D-HB-AWBusiness_17"
source: "D-HB-AWBusiness_17.pdf"
tags: ["A+W Business", "ERP Software", "Sales Module", "Offer Management", "Financial Accounting Integration", "FiBu", "CRM", "Data Archiving", "User Manual", "German"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a comprehensive tutorial and software reference for the A+W Business Verkauf (Sales) module. It guides users through creating and managing offers, handling alternative offers, tracking sales documents, analyzing success rates (statistics), and performing data transfers to financial accounting (FiBu) and archiving systems. It includes step-by-step instructions, exercises, and detailed descriptions of software dialogs and functions."
long_description: "This document serves as an in-depth guide for the 'A+W Business Verkauf' (Sales) module, a component of the A+W ERP software for the glass, windows, and doors industry. It is structured into two main parts: a tutorial and a software reference. The tutorial section provides practical, step-by-step instructions and exercises on key sales processes. This includes creating standard offers, defining alternative positions within an offer (e.g., using different materials or constructions), generating a separate alternative offer, and converting offers into orders. It also covers the process of setting up and managing follow-ups (Wiedervorlage) to track open offers. The software reference section provides a detailed breakdown of all menus, dialogs, and functions within the sales module. It explains concepts like offer statistics (Erfolgsquote) for analyzing conversion rates, the data transfer process to financial accounting systems (FiBu), including setup for accounts (Erlöskonten) and handling of open items (Offene Posten). Furthermore, it details the document import/export capabilities via EDI interfaces and the critical process of archiving completed or old documents to maintain system performance. The guide is intended for users who manage the sales lifecycle, from initial quotation to final data hand-off and analysis."
---

---
## Tutorial: Alternative Offers

[Image: Abb. C-201 Alternative Sprossen, showing a user interface for modifying horizontal (A) and vertical (B) muntins in a window design.]

**A** Waagerechte Sprossen ändern (Change horizontal muntins)
**B** Senkrechte Sprossen ändern (Change vertical muntins)

5.  Legen Sie die Alternative fest, z. B. breitere Sprossen oder eine andere Sprossenkonstruktion.
    Dazu müssen Sie die Sprossenkonstruktion auch dann angeben, wenn Sie nur die Sprossen selbst ändern wollen.
    Wie Sie Sprossenkonstruktionen aufbauen, ist ausführlich in einer separaten der Einheit erklärt.
    ⇨ "Sprossen erfassen" auf Seite C-1363

6.  Wählen Sie im Menü Start > Ausführen, um die Änderung zu übernehmen.
    Die Anzeige wechselt wieder zum Register Original. Prüfen Sie nochmals, ob die richtige Position markiert ist.

7.  Klicken Sie auf [Einfügen/Ersetzen], um die Sprossenkonstruktion einzulesen.
    Die Änderung wird im Feld Einfügen/ersetzen durch angezeigt.

8.  Wiederholen Sie die Schritte 4 bis 5 für den nächsten Modus der markierten Position oder für andere Positionen.

> **i Alternativen für markierte Positionen**
> Achten Sie darauf, dass nur die Positionen markiert sind, die im Alternativangebot mit geänderten Stücklisten-Komponenten aufgeführt werden sollen. Die Markierung einer Position wird nicht automatisch entfernt, wenn Sie eine andere Position markieren.

9.  Wechseln Sie zum Register Alternative, um den aktuellen Stand der Alternativen zu prüfen.

10. Wählen Sie im Menü Start > Ausführen, um das Alternativangebot zu erstellen.
    Das alternative (neue) Angebot wird erstellt. Die Nummer des neuen Angebots wird in der Titelzeile angezeigt.

11. Schließen Sie den Dialog Alternativen.
    Der Dialog Dokumentenverwaltung wird wieder angezeigt. In der Dokumentenübersicht wird das Alternativangebot aufgeführt und mit einem Pfeil im Zeilenkopf gekennzeichnet.

[Image: Abb. C-202 Alternativangebot, showing the document management view with the new alternative offer highlighted.]

Sie können die Daten des Alternativangebots weiter bearbeiten, z. B. den Termin zur Wiedervorlage oder die Preise.

## Übungen

### Angebot mit alternativer Position erfassen
Kopieren Sie einen Ihrer Aufträge in ein Angebot für einen anderen Kunden.
*   Erfassen Sie in diesem neuen Angebot zu Position 1 eine alternative Position.

### Alternativangebot erfassen
*   Erfassen Sie ein Alternativangebot zu dem Angebot.
*   Wechseln Sie in Position 2 die Außenscheibe in ein Ornamentglas.
*   Fügen Sie in Position 3 ein (anderes) Sprossengitter ein.

### Angebot in Auftrag überführen
Kopieren Sie Ihr Angebot in einen Auftrag.
*   Übernehmen Sie die Positionen vollständig (1:1).

### Ergänzende Informationen
⇨ "Alternativangebot" auf Seite C-1591
⇨ "Angebotsverfolgung" auf Seite C-1604
⇨ "Angebotsstatistik" auf Seite C-1610
⇨ Softwarereferenz, "Wiedervorlage" auf Seite C-1663
⇨ Softwarereferenz, "Angebotsstatistik" auf Seite C-1666
⇨ Softwarereferenz, "Dokument - Kopfdaten" auf Seite C-1687

## Angebotsverfolgung

**Lernziele**
*   Angebote als Wiedervorlage anzeigen lassen.

**Nutzen**
*   Nach einer automatischen Erinnerung an Angebote können Sie den Kontakt zum Kunden wieder aufnehmen und daraus einen neuen Auftrag erstellen.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Wiedervorlage** | Sie können sich automatisch an Angebote erinnern lassen, deren Wiedervorlagetermin erreicht ist. |
| **Voreinstellungen** | Stammdaten: Auftrag > Kategorien. Firmendaten: Register System > Vorlauftage |

## Wiedervorlage

Angebote sind dann erfolgreich, wenn sie in Aufträgen münden. Dazu können Sie beitragen, indem Sie den Kunden nach einer Bedenkfrist erneut ansprechen. Sie selbst können sich an die offenen Angebote erinnern lassen oder sich offene Angebote nach einem bestimmten Termin anzeigen lassen.

[Image: Abb. C-203 Termin zur Wiedervorlage, showing the date fields for setting a follow-up date.]

Zur Wiedervorlage können sowohl Angebot als auch Aufträge angezeigt werden. Die nachfolgenden Beschreibungen für Angebote gelten in gleicher Weise auch für Aufträge.

Die Erinnerungsfrist wird in den Firmendaten eingetragen. Danach wird beim Erfassen eines Angebots automatisch ein Datum zur Wiedervorlage eingefügt, das Sie jederzeit anpassen können, z. B., wenn Sie mit dem Kunden einen solchen Termin abgesprochen haben.

Wenn der Termin zur Wiedervorlage fällig ist, wird automatisch die Meldung angezeigt, dass ein Angebot vorliegt, zu dem Sie wieder Kontakt mit dem Kunden aufnehmen wollen.

[Image: Abb. C-204 Automatische Meldung beim Systemstart, showing a system prompt about documents due for follow-up.]

Aus der Übersicht der betreffenden Angebote können Sie sich jedes Angebot anzeigen lassen und nachverfolgen. Mit einem neuen Datum kann das Angebot erneut zur Wiedervorlage gespeichert werden. Soll es nicht wieder vorgelegt werden, können Sie es direkt archivieren und löschen.

## Angebot verfolgen

In dieser Einheit lernen Sie, wie Sie sich Angebote zur Weiterverfolgung anzeigen lassen.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So stellen Sie die automatische Erinnerung ein" auf Seite C-1606
*   "So lassen Sie sich Angebote zur Wiedervorlage anzeigen" auf Seite C-1607
*   "So geben Sie alte Angebote zur Archivierung oder zum Löschen frei" auf Seite C-1608

### So stellen Sie die automatische Erinnerung ein

1.  Wählen Sie Dokumente > Angebot > Wiedervorlage.

[Image: Abb. C-205 Wiedervorlage, showing the follow-up dialog with options for setting a follow-up date (A) and interval (B).]

**A** Vorlagedatum oder -zeitraum
**B** Intervall für die Wiedervorlage

⇨ Softwarereferenz, "Wiedervorlage" auf Seite C-1663

2.  Wählen Sie im Menü Optionen > Automatische Benachrichtigung.

[Image: Screenshot of the options menu to enable automatic notifications.]

Diese Einstellung gilt übergreifend für alle Angebote. Wenn Sie A+W Business das nächste Mal starten, wird im Kommentarbereich ein Hinweis auf die Angebote angezeigt, die zur Nachverfolgung anstehen.

3.  Markieren Sie das Angebot, in dem Sie das Datum zur Wiedervorlage prüfen und ggf. anpassen wollen.

4.  Markieren Sie die Checkbox Vorlage alle (B), wenn Sie sich das Angebot in Intervallen anzeigen lassen wollen.

5.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern. Die Änderungen werden gespeichert.

### So lassen Sie sich Angebote zur Wiedervorlage anzeigen

6.  Wählen Sie im Menü Start > Filter, um in den Such-Modus zu wechseln.

[Image: Abb. C-206 Wiedervorlage - Such-Modus, showing the follow-up dialog in search mode with fields for a date range.]

**A** Vorlagedatum
**B** Bis-Datum für Zeitraum

7.  Tragen Sie in den Feldern Vorlagedatum (A) und bis (B) den gewünschten Zeitraum ein.

8.  Wählen Sie im Menü Start > Suchen, um die Suche zu starten.

[Image: Abb. C-207 Wiedervorlage – Trefferliste, showing the search results for follow-up offers.]

Im Bereich Tabelle werden alle Angebote mit einem Vorlagedatum aus dem angegebenen Zeitraum aufgelistet. Sie können ein neues Datum zur Wiedervorlage einstellen und mit [OK] speichern.

9.  Klicken Sie in der Übersicht doppelt auf das Angebot, das Sie prüfen wollen. Das Angebot wird geöffnet.

### So geben Sie alte Angebote zur Archivierung oder zum Löschen frei

1.  Lassen Sie sich die alten Angebote anzeigen, indem Sie einen entsprechenden Zeitraum für die Vorlagetage einstellen.
2.  Markieren Sie in der Übersicht das Angebot, dessen Status Sie umsetzen wollen.
3.  Wählen Sie eine Kategorie aus.
4.  Markieren Sie die Checkbox Übergabe Archiv, wenn das Angebot zunächst archiviert werden soll.
5.  Wählen Sie im Menü Start > Speichern, um den Status zur Archivierung umzusetzen.
6.  Markieren Sie die Checkbox Löschfreigabe, wenn das Angebot gelöscht werden soll. Wenn Sie diese Checkbox zuerst markieren, können Sie das Angebot anschließend nicht archivieren.
7.  Wählen Sie im Menü Start > Speichern, um den Status umzusetzen. Der Status wird umgesetzt und Sie können das nächste Angebot markieren und ändern.

## Übungen

### Datum zur Wiedervorlage einstellen
Stellen Sie für Ihre Angebote das Datum zur Wiedervorlage ein.
*   Tragen Sie im Register Dokument das Datum im Feld Vorlage ein.
*   Wählen Sie dazu das Datum des Folgetags, wenn Sie die Lerneinheit am nächsten Tag nochmals durchgehen wollen.

### Angebote zur Wiedervorlage anzeigen
Lassen Sie sich die Angebote zum eingestellten Datum im Dialog Wiedervorlage anzeigen.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Wiedervorlage" auf Seite C-1663
⇨ Stammdaten, "Vorlauftage für Wiedervorlage" auf Seite B-1115

## Angebotsstatistik

**Lernziele**
*   Erfolgsquoten nach verschiedenen Kriterien anzeigen.

**Nutzen**
*   Die komprimierte Übersicht zum Erfolg von Angeboten erlaubt Ihnen einen schnellen Eindruck.
*   Durch eine detaillierte Darstellung der Erfolgsquote von Angeboten können Sie analysieren, wo die Schwerpunkte zur Akquise in der Zukunft liegen sollten.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Erfolg** | Ein Angebot ist dann erfolgreich gewesen, wenn aus ihm ein Auftrag erzeugt wurde. |
| **Auswertung** | Die Auswertung kann sich auf verschiedene Kriterien beziehen. |
| **Kategorie** | Beim Ablehnen eines Angebots kann ein Ablehnungsgrund erfasst werden. Diese Gründe können als Kategorie zur Auswertung herangezogen werden. |
| **Voreinstellungen** | Keine |

## Erfolgsquote

Über die Angebotsstatistik können Sie analysieren, wie viele aktuelle und/oder archivierte Angebote in Aufträge umgewandelt wurden. Durch die Kategorie kann ein Angebot nach verschiedenen Ablehnungsgründen klassifiziert werden. Die Kategorien legen Sie selbst fest, z. B. zu teuer, keine Rückmeldung.

Folgende Daten werden ausgewiesen:
*   Anzahl der Angebote pro Kunde
*   Anzahl der aus den Angeboten entstandenen Aufträge
*   Gesamtbruttobetrag über die Summe der Angebote
*   Gesamtbruttobetrag über die Summe der Aufträge
*   Erfolgsquote in Prozent für Anzahl und Betrag

Damit haben Sie aussagekräftige Werte zur Verfügung, anhand derer Sie z. B. notwendige Korrekturen einleiten können.

## Angebote auswerten

In dieser Einheit lernen Sie, wie Sie den Erfolg Ihrer Angebote feststellen.

### So stellen Sie die Erfolgsquote pro Kunde fest

1.  Wählen Sie Dokumente > Angebot > Angebotsstatistik.
2.  Wählen Sie ggf. den Auswahlmodus.

[Image: Abb. C-208 Erfolgsquote für einen Kunden prüfen, showing the offer statistics dialog.]

**A** Erfassungszeitraum
**B** Kategorie
**C** Archiv
**D** Detailauswahl

⇨ Softwarereferenz, "Angebotsstatistik" auf Seite C-1666

3.  Legen Sie den Erfassungszeitraum (A) fest und tragen Sie die Kundennummer ein.
4.  Markieren Sie die Kategorie (B), nach der ausgewertet werden soll.
5.  Markieren Sie ggf. das Archiv (C), wenn die Angebote bereits archiviert sind.
6.  Markieren Sie ggf. die Checkbox Detailauswertung (D), um die Angebote einzeln aufzuführen.
7.  Wählen Sie im Menü Start > Suchen, um in die Suche zu starten.

[Image: Abb. C-209 Detailauswertung zu einem Kunden, showing the detailed results of the offer statistics.]

**A** Anzahl der ausgewerteten Angebote
**B** Anzahl der Aufträge aus den Angeboten
**C** Erfolgsquote nach Anzahl
**D** Erfolgsquote nach Umsatz

Die Angebote werden je nach Auswertungskriterien als Summe oder mit Details angezeigt.

## Übungen

### Erfolgsquote prüfen
Stellen Sie fest, wie erfolgreich Ihre Angebote in Aufträge überführt wurden.
*   Wählen Sie als Zeitraum die Schulungstage, in denen Angebote und Aufträge erfasst haben.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Kategorie" auf Seite C-1662
⇨ Softwarereferenz, "Angebotsstatistik" auf Seite C-1666

## Datenübergabe

In diesem Themenblock lernen Sie, wie Sie Daten über Schnittstellen weiterleiten.

Dazu gehören folgende Lerneinheiten:
*   "Finanzbuchhaltung (FiBu)" auf Seite C-1616
*   "Statistikübergabe" auf Seite C-1625
*   "Archivierung" auf Seite C-1631

## Finanzbuchhaltung (FiBu)

**Lernziele**
*   Einstellungen für den Datenaustausch mit einem Programm zur Finanzbuchhaltung.
*   Daten übertragen.
*   Offene Posten abfragen.

**Nutzen**
*   A+W Business kann mit verschiedenen FiBu-Programmen kommunizieren, an die Sie die Rechnungen übergeben können.
*   Rechnungen und Gutschriften können Sie per Datenübergabe weiterleiten.
*   Offene Posten zu Kundenrechnungen werden von einigen Programmen zurückgemeldet, so dass Sie evtl. Mahnungen schreiben oder einen säumigen Kunden sperren können.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Finanzbuchhaltung** | A+W Business stellt Schnittstellen zu Programmen zur Finanzbuchhaltung (FiBu) zur Verfügung. |
| **Automatische Datenübergabe** | Nur wenn Sie mit der SQL-FiBu Syska arbeiten, kann die Datenübergabe automatisch gestartet werden. |
| **Erlöskonten** | In A+W Business werden die Erlöskonten der FiBu den Warengruppen zugeordnet. |
| **Datenübergabe** | Die Daten werden in eine Übertragungsdatei geschrieben. Die Auswahl der Daten, die übergeben werden sollen, kann angepasst werden. |
| **Offene Posten** | Die Abfrage von offenen Posten (OP-Abfrage) funktioniert nur mit der SQL-FiBu Syska. Das Ergebnis der Abfrage listet alle offenen Rechnungen mit ausstehenden Summen, Mahndatum und Mahnstufe auf. |
| **Buchungskreise** | Wenn Sie im eingesetzten FiBu-Programm Buchungskreise für Ihre Mandanten definiert haben, können Sie die FiBu der einzelnen Mandanten gesondert pflegen. |
| **Voreinstellungen** | **Stammdaten:** Statuszuordnung, Nummernkreise, Finanzen. **Firmendaten:** Register FiBu. **Utilities:** Debitoren/Kreditoren an FIBU, Offene Posten. |

## Datenübergabe

A+W Business stellt Schnittstellen zur Verfügung, mit denen Rechnungen und Gutschriften an Programme zur Finanzbuchhaltung (FiBu) übergeben werden können.

Die Daten werden über einen Nummernverwalter an die FiBu übergeben. Nur wenn Sie mit der FiBu Syska arbeiten, kann die Datenübergabe automatisch gestartet werden.

> **i Automatische Datenübergabe**
> Die Datenübergabe kann automatisiert werden. Dazu gibt es verschiedene Möglichkeiten, z. B. Workflow-Tasks. Von Ihrer Systemkonfiguration hängt ab, welche Möglichkeit Sie nutzen können. Sollten Sie hierzu Fragen haben, wenden Sie sich bitte an Ihren Service-Mitarbeiter bei der A+W Software GmbH.

Die Übergabe von Rechnungen an das FiBu-Programm wird in der Regel manuell ausgelöst. Die Daten werden für alle Rechnungen nach den gleichen Kriterien übergeben.

Die Dokumente werden in zwei Stufen analysiert und gruppiert:
*   Die erste Stufe fasst alle Positionen und Stücklisten-Komponenten nach ihrer Kombi-Warengruppe für die Statistik zusammen.
*   Die zweite Stufe gruppiert das Ergebnis noch einmal. Dabei wird das entsprechende Erlöskonto gesucht. Schlüssel der Suche sind die Warengruppe, die MwSt. 1, die MwSt. 2 und die Geschäftsart des Dokuments. Fehlt ein solcher Schlüssel, wird ein Dialog geöffnet, in dem das Erlöskonto eingetragen werden kann.

Wenn ein Schlüssel mit einem leeren Eintrag für das Erlöskonto vorhanden ist, wird dieses leere Erlöskonto in die Ausgabedatei geschrieben.

Sonderrabatte und Zuschläge mit der Produktart Leistungen und Zuschläge, die in Warengruppe 000 laufen, werden nicht übergeben, sondern auf die betreffenden Positionen oder Stücklisten-Komponenten (zurück) verteilt.

### Statuszuordnung
In der Statuszuordnung geben Sie an, welchen Mindeststatus das Dokument haben muss, um die FiBu-Übergabe machen zu können.

[Image: Abb. C-210 Beispiel Status für FiBu-Übergabe, showing the status assignment dialog for FiBu transfer.]

Damit das Dokument kein zweites Mal in die FiBu übergeben wird, muss außerdem ein Sperrstatus definiert werden.

### Tagesabschluss
Rechnungen können z. B. einmal pro Tag in einem nächtlichen Batchlauf an die FiBu übergeben werden. In der Regel werden die Dokumente bei der Übergabe an die FiBu (automatisch) sowohl ans Archiv als auch an die Statistik übergeben.

Für die automatische Übergabe sind folgende Einstellungen erforderlich:
*   Buchungsperioden
*   Pfade für die Import- und Export-Datei
*   Workflow-Task für den A+W Business 6 Interface Service
*   Übergabe-Intervall oder -Zeitpunkt

### Buchungsperioden
Die Buchungsperioden werden bei der Übergabe an das FiBu-Programm geprüft. Wenn das eingetragene Datum erreicht ist, kann kein Dokument mehr in diese Buchungsperiode übergeben werden.

[Image: Abb. C-211 Buchungsperioden, showing the dialog for closed accounting periods.]

Wenn ein Dokument zwischen dem Datum der ersten und dem Datum der nächsten Buchungsperiode liegt, prüft A+W Business, welches der beiden dem Datum des Dokuments am nächsten ist.

### Datenübergabedatei
Die Daten werden in eine Übertragungsdatei geschrieben. Mit verschiedenen Optionen können Sie die Datenübergabe anpassen, z. B.:
*   Ausgabedatei
*   Rechnungen nur mit Wert über 0
*   Automatische Sortierung
*   Steuerkennzeichen separat verarbeiten

Standardmäßig wird die Kundennummer als Kontonummer herangezogen. Wenn im Dokument eine vom Kunden abweichende Rechnungsanschrift eingetragen ist, wird diese als Kontonummer herangezogen. In den Stammdaten des Kunden kann aber auch eine Debitorennummer hinterlegt werden, die dann als Kontonummer übergeben werden kann.

An viele FiBu-Programme kann ein beliebiger Buchungstext übergeben werden. In der Regel ist dies die Rechnungs- oder Kundenanschrift in der Form Name, Straße, Postleitzahl und Ort.

### Erlöskonten
Für jede Warengruppe und jedes MwSt.-Kennzeichen richten Sie ein Erlöskonto ein. Damit die Produktumsätze auf das richtige Konto gebucht werden, ordnen Sie den Warengruppen die Erlöskonten zu.

Außerdem können Sie jeder Warengruppe ein oder mehrere Mehrwertsteuerkennzeichen zuweisen und so auch die Geschäfte mit Ihren ausländischen Kunden ohne Mehraufwand abwickeln und auswerten.

[Image: Abb. C-212 Erlöskontenverwaltung, showing the revenue account management interface.]

*   **Debitor (Kunde):** In den Feldern Rechnung und Gutschrift tragen Sie die Erlöskonten für die Rechnungen und Gutschriften der Kundenaufträge ein. Auch die Mehrwertsteuer wird auf dieses Erlöskonto gebucht, wenn nicht unter Stammdaten > Finanzen > MwSt. ein anderes Erlöskonto für das Mehrwertsteuer-Kennzeichen eingetragen wird.
*   **Kreditor (Lieferant):** In den Feldern Rechnung und Gutschrift tragen Sie die Erlöskonten für die Rechnungen und Gutschriften der Lieferantenbestellungen ein. Siehe auch Erläuterungen zu Debitor.

**Beispiel**

Ausgangsdaten:
2 Warengruppen: `5**` und `6**`
2 MwSt.-Kennzeichen 1: `1` und `2`
1 MwSt.-Kennzeichen 2: `= 1`

MwSt.-Zusammenstellungen:

| MwSt. 1 | MwSt. 2 |
| :--- | :--- |
| 1 | 0 |
| 2 | 0 |
| 2 | 1 |

2 Geschäftsarten: Streckengeschäft und Handelsgeschäft

Folgende Erlöskonten müssen angelegt werden:

| WGR | MwSt.-Kz. 1 | MwSt.-Kz. 2 | Geschäftsart |
| :-- | :--- | :--- | :--- |
| 5** | 1 | 0 | Streckengeschäft |
| 5** | 2 | 0 | Streckengeschäft |
| 5** | 2 | 1 | Streckengeschäft |
| 6** | 1 | 0 | Streckengeschäft |
| 6** | 2 | 0 | Streckengeschäft |
| 6** | 2 | 1 | Streckengeschäft |
| 5** | 1 | 0 | Handelsgeschäft |
| 5** | 2 | 0 | Handelsgeschäft |
| 5** | 2 | 1 | Handelsgeschäft |
| 6** | 1 | 0 | Handelsgeschäft |
| 6** | 2 | 0 | Handelsgeschäft |
| 6** | 2 | 1 | Handelsgeschäft |

*Tab. C-6: Beispiel Erlöskonten*

### Offene Posten (OP)
Über die OP-Rückmeldung werden alle offenen Rechnungen mit Angabe der ausstehenden Summe, Mahndatum und Mahnstufe gemeldet.

[Image: Abb. C-213 Anzeige der offenen Posten, showing the dunning/open items module.]

Mit dem Modul Mahnwesen können Sie bezahlte Rechnungen in A+W Business manuell verbuchen. Die Summe der offenen Posten wird automatisch um diese gebuchten Beträge und unter Einbeziehung der abgezogenen Skontobeträge reduziert. Dabei kann es sich sowohl um Gesamt- als auch Teilrechnungsbeträge einschließlich Skonto handeln.

Pro Rechnungseintrag wird ausgewiesen, welchen Gesamtbetrag der Kunde zu zahlen hat, welche Zahlungen (inklusive Teilbeträge) er bereits geleistet hat und welcher Betrag von dieser Rechnung noch offen steht. Die Summe wird in der Auftragserfassung angezeigt und ermöglicht die zeitnahe Entscheidung in "kritischen" Fällen.

### Rechnungen an die FiBu übergeben
In dieser Einheit lernen Sie, wie Sie Rechnungen an die FiBu übergeben.

#### So übergeben Sie Rechnungen an die FiBu

1.  Sammeln Sie alle Aufträge bzw. deren Rechnungen, die übergeben werden sollen, in einem Nummernverwalter.
2.  Wählen Sie Dokumente > Auftrag > FIBU-Übergabe.
    Der Dialog Sollstellung FIBU wird geöffnet.
    ⇨ Softwarereferenz, "Sollstellung FiBu" auf Seite C-1970
3.  Wählen Sie den Nummernverwalter aus, in dem Sie die Rechnungen zusammengestellt haben.

[Image: Abb. C-214 Rechnungen zur Übergabe an die FiBu bereit, showing the dialog for preparing invoices for FiBu transfer.]

Die Rechnungen werden in der Übersicht angezeigt.

4.  Prüfen Sie die Einstellungen im Menü Optionen, z. B., ob Rechnungen mit einem Betrag gleich 0 übergeben werden sollen.
5.  Wählen Sie ggf. den Mandanten und den Bereich.
6.  Wählen Sie im Menü Start > Ausführen, um die Daten zu übergeben. Die Daten werden übergeben.
7.  Bestätigen Sie die Meldung zur Übergabedatei.

Sie können die Datei in einem Editor prüfen, bevor Sie sie an das Buchhaltungsbüro weitergeben.

[Image: Abb. C-215 Rechnungen sind übergeben, showing the dialog after the FiBu transfer is complete.]

**A** Neuer Status
**B** Anzahl der übergebenen Aufträge und Positionen

Im Dialog Sollstellung FIBU werden die Anzeigefelder aktualisiert und der Status der Rechnungen umgesetzt. Damit können die Rechnungen nicht nochmals übergeben werden.

**Ergänzende Informationen**
⇨ Stammdaten, "Erlöskonten" auf Seite B-1047
⇨ Stammdaten, "Update OP-Saldo nach Übergabe" auf Seite B-1063
⇨ Stammdaten, "Firmendaten - FiBu" auf Seite B-1061
⇨ Stammdaten, "Erlöskonten" auf Seite B-1047
⇨ Stammdaten, "Schnittstellen-Dienst" auf Seite B-1175

## Statistikübergabe

**Lernziele**
*   Dokumente manuell übergeben.
*   Automatische Übergabe einrichten.

**Nutzen**
*   Alle Dokumente können nach verschiedenen Kriterien statistisch ausgewertet werden.
*   Sie können die Übergabe der Dokumente an die Statistik automatisieren und individuell einrichten.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Vorhaltetage** | Vorhaltetage legen eine Zeitspanne fest, in der Daten in der Hauptdatenbank gespeichert bleiben. |
| **Statistik** | Dokumente können separat übergeben werden für: Provisionsstatistik, Umsatzstatistik. |
| **Voreinstellungen** | **Stammdaten:** Top-WGR. **Firmendaten:** Register Archiv, Register Tagesabschluss. **Utilities:** Statistik-Update. |

## Berichte

Mit dem Modul Statistik stellt A+W Business eine Reihe von Berichten (Reports) zur Verfügung. Dazu werden die Dokumente an die Statistik übergeben. Für jede Dokumentenart legen Sie fest, ob und wann das entsprechende Dokument übergeben werden soll.

Die Dokumente werden gleichzeitig an die Statistik und ans Archiv übergeben. Für die Statistik werden bestimmte Auftragsdaten in eine eigene Tabelle in der Hauptdatenbank geschrieben. Anhand hinterlegter Fristen (Vorhaltetage) prüft das System, wie lange diese in der Hauptdatenbank gespeichert bleiben sollen, bis sie automatisch gelöscht werden.

Dabei werden alle Daten aus der Hauptdatenbank gelöscht, die älter sind als die eingetragenen Fristen. Die Fristen bestimmen Sie pro Dokumentenart selbst.

> **Beispiel**
> Wenn Sie Jahresübersichten erzeugen wollen, sollten Sie einen langen Zeitraum eintragen, um einen ausreichenden Spielraum für die Erstellung der Auswertung zu haben.
> Für die Provisionsstatistik ist der Rhythmus ausschlaggebend, in dem Sie Provisionen abrechnen.

Mit der Übergabe an die Statistik wird der Status der Dokumente umgesetzt. Ein Beispiel für die Statusumsetzung finden Sie in der Lerneinheit zum Status:
⇨ "Automatische Statusvergabe" auf Seite C-1495

### Tagesabschluss
Standardmäßig ist für die Übergabe an die Statistik der Monat des Dokumentendatums ausschlaggebend, für die Archivierung das Jahr. Nach der Archivierung sollten die Dokumente gelöscht werden, um die Hauptdatenbank so klein wie möglich zu halten.

In der Regel werden die Dokumente bei der Übergabe an die FiBu (automatisch) sowohl ans Archiv als auch an die Statistik übergeben.

## Aufträge an die Statistik übergeben

In dieser Einheit lernen Sie, wie Sie Aufträge manuell an die Statistik übergeben.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So richten Sie die Übergabe an die Statistik ein" auf Seite C-1627
*   "So übergeben Sie Aufträge ans Archiv" auf Seite C-1635

### So richten Sie die Übergabe an die Statistik ein

1.  Wählen Sie Stammdaten > Firma > Firmendaten > Register Archiv.

[Image: Abb. C-216 Einstellungen für die Übergabe an die Statistik, showing the archive settings dialog.]

**A** Details zur Archivierung
**B** Auswahl der Automatikoptionen
**C** Dokumententyp

⇨ Stammdaten, "Firmendaten - Archiv" auf Seite B-1104

2.  Wählen Sie den Dokumententyp (C) aus.
3.  Markieren Sie die Checkboxen (B) Übergabe Provisionsstatistik und/oder Übergabe Umsatzstatistik.
4.  Markieren Sie die Checkboxen (A), mit denen Sie die Details der Statistik festlegen können, z. B. den Export in die Superstatistik.
5.  Klicken Sie auf [Speichern], um die Daten zu speichern.
6.  Die Einstellungen werden für den gewählten Dokumententyp gespeichert.
7.  Wiederholen Sie die Schritte n bis n für alle Dokumententypen, die Sie an die Statistik übergeben wollen.
8.  Wechseln Sie zum Register Tagesabschluss und prüfen Sie die Angaben für die Vorhaltetage.

[Image of Vorhaltetage settings dialog.]

Mit diesen Einstellungen legen Sie fest, wie lange die Dokumente in der Hauptdatenbank gespeichert bleiben sollen, bis sie automatisch und endgültig gelöscht werden.

9.  Klicken Sie auf [Speichern], um die Änderungen zu speichern. Die Einstellungen werden gespeichert.

### So übergeben Sie Aufträge an die Statistik

1.  Sammeln Sie alle Aufträge, die übergeben werden sollen, in einem Nummernverwalter.
2.  Wählen Sie Dokumente > Auftrag > Übergabe Archiv.

[Image: Abb. C-217 Aufträge zur Übergabe an die Statistik bereit, showing the dialog for transferring orders to statistics.]

**A** Löschen
**B** Nummernverwalter
**C** Übergabe an
**D** Archivjahr
**E** Archivmonat

⇨ Softwarereferenz, "Übergabe Archiv" auf Seite C-1974

3.  Wählen Sie den Nummernverwalter aus (B), in dem Sie die Aufträge zusammengestellt haben. Die Übersicht der Aufträge wird aktualisiert.
4.  Wählen Sie ggf. den Mandanten.
5.  Markieren Sie die Checkboxen (C) Provisionsstatistik und/oder Umsatzstatistik.
6.  Geben Sie das Statistikjahr (D) und den -monat (E) an, z. B. 2011 und 12.
7.  Markieren Sie die Checkboxen Archiv und Löschen (A) nur, wenn Sie die Aufträge gleichzeitig archivieren und aus der Hauptdatenbank löschen wollen.
8.  Klicken Sie auf [Ausführen], um die Übergabe zu starten. Die Daten werden übergeben.

[Image: Abb. C-218 Aufträge sind übergeben, showing the dialog after the transfer to statistics is complete.]

Der Status der Aufträge ist umgesetzt. Sie können jetzt im Modul Statistik die Auswertungen starten.

**Ergänzende Informationen**
⇨ Stammdaten, "Firmendaten - Archiv" auf Seite B-1104
⇨ Stammdaten, "Firmendaten - Tagesabschluss" auf Seite B-1111

## Archivierung

**Lernziele**
*   Unterschiede zwischen Haupt- und Archivdatenbank kennenlernen.
*   Vorgaben für Archivierung einstellen.
*   Dokumente manuell archivieren.

**Nutzen**
*   Sie pflegen die Hauptdatenbank, indem Sie alte Aufträge archivieren.
*   Mit der Archivierung und der gleichzeitigen Löschung bleibt die Performance der Hauptdatenbank erhalten.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Dokumente** | Folgende Dokumente können archiviert werden: Angebote, Aufträge, Gutschriften, Anfragen, Bestellungen. |
| **Archivjahr** | A+W Business kann mehrere Archivjahre verwalten. Bei bestimmten Aktionen kann das Archiv ausgewählt werden, z. B. beim Kopieren von Dokumenten. |
| **Datenbanken** | Die aktuellen Daten werden in A+W Business in der Hauptdatenbank verwaltet. Daneben bestehen unabhängige Datenbanken für die Archive. Diese werden i. d. R. pro Kalenderjahr angelegt. |
| **Voreinstellungen** | **Firmendaten:** Register Archiv, Register Parameter (Vertreterprovisionierung), Register Tagesabschluss (Archivpfad). |

### Abgeschlossene Dokumente
Abgeschlossene Geschäftsvorgänge bleiben für eine von Ihnen definierte Zeit in der Hauptdatenbank und werden dann automatisch archiviert. Alle Dokumentendaten werden unverändert gespeichert. Sie können als Kopie aus dem Archiv geholt werden.

Die Dokumente werden gleichzeitig an das Archiv und die Statistik übergeben und anschließend standardmäßig aus der Hauptdatenbank gelöscht. Nach der Übergabe der Daten ans Archiv wird die Hauptdatenbank reindiziert, um die gewohnte Verarbeitungsgeschwindigkeit wieder herzustellen.

Da die Archivierung sehr rechenintensiv ist, erfolgt sie allabendlich und vollautomatisch.

### Archive
Die Archive bilden eigene Datenbanken, die jeweils ein Jahr zusammenfassen. Beim Jahreswechsel archiviert das System die Dokumente in Abhängigkeit vom Rechnungsdatum im entsprechenden Archiv.

Archivierte Dokumente können jederzeit zurück in die Hauptdatenbank kopiert werden.
⇨ "Dokumente kopieren" auf Seite C-1505

### Mehrfach archivieren
Wurde ein archiviertes Dokument in die Hauptdatenbank zurückkopiert, kann es nur dann erneut archiviert werden, wenn die Mehrfach-Archivierung in den Firmendaten aktiviert ist.

Wenn die Mehrfach-Archivierung nicht zugelassen ist, muss das Dokument entweder in der Hauptdatenbank bleiben oder sein Status muss manuell hochgesetzt werden, damit es gelöscht werden kann.

### Automatische Archivierung
In der Regel werden die Dokumente automatisch archiviert und anschließend gelöscht. In den Firmendaten können dazu der Mindeststatus und das Alter der Dokumente festgelegt werden.

### Manuelle Archivierung
Zur manuellen Archivierung werden alle Dokumente, die ans Archiv (und/oder an die Statistik) übergeben werden sollen, in den Nummernverwalter gestellt.
Mit der Funktion Übergabe Archiv werden alle Dokumente eines Nummernverwalters übergeben.
⇨ Stammdaten, "Dokumente nur löschen wenn bereits archiviert" auf Seite B-1106

### Referenzprüfung
Wenn die Referenzen beim Löschen von Dokumenten durch die Archivierung geprüft werden, wird auch geprüft, ob alle referenzierten Dokumente eines Auftrags bereits archiviert sind, z. B. Teillieferungen, Reklamationen. Erst danach ist es möglich, den Auftrag zu löschen.

### Auftrag ohne Rechnung
Wenn zu einem Auftrag kein Rechnungsdatum vorhanden ist, kann er nur archiviert werden, wenn der Status größer als Rechnungs-Original gedruckt und kleiner als Datenübergabe an Archiv ist. Dann wird davon ausgegangen, dass keine Rechnung mehr geschrieben werden soll und das Archivjahr wird durch das Erfassungsdatum bestimmt.

### Dokumente archivieren
In dieser Einheit lernen Sie, wie Sie Dokumente manuell archivieren.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So richten Sie die Übergabe ans Archiv ein" auf Seite C-1633
*   "So übergeben Sie Aufträge ans Archiv" auf Seite C-1635

#### So richten Sie die Übergabe ans Archiv ein

1.  Wählen Sie Stammdaten > Firma > Firmendaten > Register Archiv.

[Image: Abb. C-219 Einstellungen für die Übergabe an die Statistik, showing the archive settings dialog.]

**A** Details zur Archivierung
**B** Auswahl der Automatikoptionen
**C** Archivierungsmodus
**D** Dokumententyp

⇨ Stammdaten, "Firmendaten - Archiv" auf Seite B-1104

2.  Wählen Sie den Dokumententyp (D) aus.
3.  Markieren Sie die Checkboxen (B) Übergabe Archiv und/oder Dokument löschen.
4.  Wählen Sie den Modus (B) für die Archivierung.
    *   **Mindeststatus:** Status, ab die Dokumente automatische archiviert werden.
    *   **Dokument älter als X Tage:** Anzahl der Tage, die nach dem Erfassungsdatum verstrichen sein müssen, bevor das Dokument archiviert wird. Bei dieser Einstellung müssen Sie auch die Übergabe nach Erfassungsdatum (A) aktivieren. Dieser Wert bietet sich beispielsweise an, wenn eine Reklamationsfrist abgewartet werden soll.
    *   **Status + Dokument älter als:** Bei diesen Einstellungen müssen beide Kriterien erfüllt sein: Der entsprechende Status muss erreicht sein und das Dokument muss das eingetragene Alter erreicht haben.
5.  Markieren Sie die Checkboxen (A), mit denen Sie die Details für die Archivierung festlegen können, z. B. die Übergabe nach Erfassungsdatum.
6.  Klicken Sie auf [Speichern], um die Daten zu speichern.
7.  Die Einstellungen werden für den gewählten Dokumententyp gespeichert.
8.  Wiederholen Sie die Schritte 2 bis 6 für alle Dokumententypen, die Sie an das Archiv übergeben wollen.

#### So übergeben Sie Aufträge ans Archiv

1.  Sammeln Sie alle Aufträge, die übergeben werden sollen, in einem Nummernverwalter.
2.  Wählen Sie Dokumente > Auftrag > Übergabe Archiv.

[Image: Abb. C-220 Aufträge zur Übergabe ans Archiv bereit, showing the dialog for preparing orders for archiving.]

**A** Löschen
**B** Nummernverwalter
**C** Übergabe an Statistik und Archiv

⇨ Softwarereferenz, "Übergabe Archiv" auf Seite C-1974

3.  Wählen Sie den Nummernverwalter aus (B), in dem Sie die Aufträge zusammengestellt haben. Die Übersicht der Aufträge wird aktualisiert.
4.  Wählen Sie ggf. den Mandanten.
5.  Markieren Sie die Checkboxen (C) Archiv und/oder Löschen (A).
6.  Markieren Sie die Checkboxen Provisionsstatistik und Umsatzstatistik nur, wenn Sie die Aufträge gleichzeitig an die Statistik übergeben wollen. In diesem Fall müssen Sie das Statistikjahr und den -monat angeben, z. B. 2011 und 12.
7.  Wählen Sie im Menü Start > Ausführen, um die Aktion zu starten. Die Daten werden je nach den Einstellungen in den Firmendaten übergeben. Wenn die Archivierung das Rechnungsdatum abfragt, werden nur die Aufträge archiviert, zu denen eine Rechnung erstellt wurde.

[Image: Abb. C-221 Aufträge sind übergeben, showing the dialog after the archiving process is complete.]

Der Status der Aufträge wird umgesetzt. Dokumente, deren Status eine Archivierung nicht zuließ, werden gekennzeichnet.

## Übungen

### Rechnung an die FiBu übergeben
Übergeben Sie alle Rechnungen in Ihrem Nummernverwalter an die FiBu.
Wiederholen Sie die Übergabe, indem Sie die Rechnungen an die Statistik übergeben und anschließend archivieren.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Nummernverwalter" auf Seite C-1917
⇨ Softwarereferenz, "Sollstellung FiBu" auf Seite C-1970
⇨ Softwarereferenz, "Übergabe Archiv" auf Seite C-1974
⇨ Stammdaten, "Firmendaten - Archiv" auf Seite B-1104
⇨ Stammdaten, "Dokument ohne Referenzprüfung löschen" auf Seite B-1106
⇨ Stammdaten, “Mehrfach-Archivierung" auf Seite B-1107

## Zusatzfunktionen

In diesem Abschnitt finden Sie zusätzliche Informationen zur Arbeitsweise und zu den Funktionen in A+W Business.
*   "Import von Dokumenten" auf Seite C-1639
*   "Bestandslisten" auf Seite C-1645
*   "Journal" auf Seite C-1646
*   "Dokumentenüberwachung" auf Seite C-1648

### Import von Dokumenten
Über die EDI-Schnittstellen können Sie Kundenaufträge importieren und in A+W Business bearbeiten.

#### Stammdaten für den Import
Für eingehende Kundenaufträge läuft ein automatisierter Import (Batch-File), der in regelmäßigen Abständen in den entsprechenden Verzeichnissen nach eingegangenen Aufträgen sucht und diese in die A+W Business-Auftragsbearbeitung integriert. Sie können den Import auch manuell starten.

Aus den übernommenen Daten werden Aufträge für Rechteckscheiben inklusive Sprossen in A+W Business automatisch generiert.
⇨ Softwarereferenz, "Import" auf Seite C-1976

Dazu müssen die Stammdaten beim Kunden und in A+W Business identisch angelegt sein.

**Beispiel: Identische Stammdaten für den Import**

| Sender (Kunde) | Empfänger (A+W Business) |
| :--- | :--- |
| `500124 -->` | `500124 -->` | `1004 Float 4 mm`, `105012 SZR 12 mm`, `1004 Float 4 mm` |
| `500124 -->` | `105016 SZR 16 mm -->` | `500124 -->` | `1004 Float 4 mm`, `105016 SZR 16 mm`, `1004 Float 4 mm` |

In diesem Beispiel sehen Sie, dass das Produkt 500124 eine ISO-Scheibe mit Float 4 mm Gläsern und dem SZR mit 12 mm ist.
Im zweiten Beispiel ist der SZR durch das Produkt 105016 ersetzt.

Wenn sich die Stammdaten Ihres Kunden von Ihren eigenen unterscheiden, ist der Import mit Hilfe von Referenzierungstabellen möglich. Die integrierte Referenzierung wandelt die Kundendaten in A+W Business-Daten um.

**Beispiel: Umsetzen von Kundenartikeln in Stammdaten**

| Sender (Kunde) | Empfänger (A+W Business) |
| :--- | :--- |
| `ISO416 -->` | `20004 Float 4 mm`, `4016 SZR 16 mm`, `40004 Ornament 4 mm` | `--> 500124 -->` | `1004 Float 4 mm`, `105016 SZR 12 mm`, `1804 Ornament 4 mm` |

In diesem Beispiel wird aus dem alphanumerischen Kunden-Artikelnummer ISO416 die numerische A+W Business-Produktnummer 500124.
Mit dem Zusatz-Modul Connect II können Sie auch Standard-Modelle importieren.

**Beispiel: Umsetzen von Kundenauftrag mit Modell in Stammdaten**

| Sender (Kunde) | Empfänger (A+W Business) |
| :--- | :--- |
| `ISO416 -->` | `20004 Float 4 mm`, `4016 SZR 16 mm`, `40004 Ornament 4 mm`, `110145 Modell 3` | `--> 500124 -->` | `1004 Float 4 mm`, `105016 SZR 12 mm`, `1804 Ornament 4 mm`, `8003 Modell 3` |

In diesem Beispiel wird aus dem Kunden-Modell 110415 die A+W Business-Produktnummer 8003. Beide bezeichnen das Modell 3.

Wenn ein importierter Auftrag das Kreditlimit des Kunden überschreitet, kann der Auftrag mit einem entsprechenden Status gespeichert werden.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Import" auf Seite C-1976

### Dokumente importieren
In dieser Einheit lernen Sie, wie Sie Kundenaufträge direkt über die EDI-Schnittstelle an A+W Business übergeben. Die Aufträge können manuell oder automatisch importiert werden.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So legen Sie die Einstellungen zum automatischen Import fest" auf Seite C-1641
*   "So importieren Sie einen Kundenauftrag manuell" auf Seite C-1643
*   "So beheben Sie einen Fehler in der importierten Datei" auf Seite C-1644

> **i Voraussetzung**
> Damit die Daten aus den Kundenaufträgen richtig zugeordnet werden können, müssen die Stammdaten für Kundenreferenzen korrekt angelegt sein.

#### So legen Sie die Einstellungen zum automatischen Import fest

1.  Wählen Sie Stammdaten > Firma > Customizing.
    Der Dialog Customizing wird geöffnet.
    ⇨ Stammdaten, "Customizing" auf Seite B-1186
2.  Wechseln Sie zum Register Programme und markieren Sie den Eintrag für den EDI-Import.

[Image: Abb. C-222 Programm zum EDI-Import, showing the customizing dialog with the EDI import program selected.]

3.  Wechseln Sie zum Register Autom. Prozessausführung.

[Image: Abb. C-223 Einstellungen zur Fremdschnittstelle, showing settings for automatic process execution.]

**A** Intervall
**B** Art der Ausführung

4.  Wählen Sie die Art der Ausführung (B).
    Wenn die Dokumente laufend eingelesen werden sollen, müssen Sie die Einstellung zyklisch wählen.
5.  Geben Sie den Wert (A) für das Intervall ein, in dem neue Kundenaufträge importiert werden sollen.
6.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern. Die Daten werden gespeichert.

#### So importieren Sie einen Kundenauftrag manuell

1.  Wählen Sie Dokumente > Auftrag > Import.
    Der Dialog Import Pool wird geöffnet.
    ⇨ Softwarereferenz, "Import" auf Seite C-1976
2.  Markieren Sie die Dokumente, die Sie importieren wollen.

[Image: Abb. C-224 Import, showing the import pool dialog with available documents to import.]

Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf. Nur die Positionen sind markiert, die mit einem X gekennzeichnet sind.

3.  Wechseln Sie zum Register Dokumente erstellen, um die Ziel-Einstellungen zu prüfen.
4.  Wählen Sie im Bereich Zielnummernverwalter den Nummernverwalter für diesen Import aus.
    Im Bereich Dokumente werden alle Dokumente im aktuellen Nummernverwalter aufgelistet.
5.  Wählen Sie ggf. im Bereich Parameter den Mandanten und den AV-Bereich aus, denen die Kundenaufträge zugeordnet werden sollen.
6.  Wählen Sie im Menü Start > Ausführen, um den Import zu starten.
    Die Kundenaufträge werden importiert und als A+W Business-Aufträge gespeichert.
    Wenn ein Fehler zu einem Kundenauftrag gemeldet wird, müssen Sie im den Dialog Fremddokument öffnen.

#### So beheben Sie einen Fehler in der importierten Datei

1.  Klicken Sie im Register Import Pool doppelt auf die (EDI-) Datei, um den Dialog Fremddokumentenverwaltung zu öffnen.

[Image: Abb. C-225 Import, showing the foreign document management dialog for correcting import data.]

In diesem Dialog können Sie die Daten des Kundenauftrags prüfen und ggf. korrigieren, z. B. die Produktnummer.

2.  Speichern Sie die Korrekturen.
    Der Kundenauftrag wird in A+W Business übernommen und automatisch wird ein neuer Auftrag angelegt.

> **i Automatischer Import**
> Wenn Sie ein Intervall für den automatischen Import eingestellt haben, brauchen Sie die Kundenaufträge nicht einzeln und manuell zu importieren.

### Bestandslisten
Mit den Bestandslisten können Sie sich einen Überblick über den Dokumentenbestand nach Nummernkreisen oder Warengruppen anzeigen lassen.

Die Listen stellen folgende Daten dar:
*   **Nach Nummernkreis:**
    Die letzte Nummer der bereits gedruckten Liste wird gespeichert. Die nächste Liste führt dann nur die nachfolgenden (neuen) Nummern auf. Auf diese Weise werden keine Dokumente doppelt aufgeführt.
    -   Dokumentennummer, Liefertermin, Fertigungstermin ISO, Kundennummer, Kundenname, Stück, Status, Qm, Lfm, Netto-Betrag, EK, Rohertrag in %
    -   Gesamtsumme
    -   Gesamtsumme ISO
    -   Summe aller AV-Bereiche
    -   Summe aller AV-Bereiche ISO
*   **Nach Warengruppen:**
    Gliederung nach Warengruppen
    -   Kundennummer, Kundenname, Dokumentennummer, Kommission, Stück, Status, Qm ger., Qm tats., Lfm tats., Erfassungsdatum, Lieferdatum, Netto-Betrag, EK
    -   Zwischensumme pro Warengruppen oder Kunde
    -   Gesamtsumme aller Warengruppen oder Kunden

**Ergänzende Informationen**
⇨ Softwarereferenz, "Bestandslisten" auf Seite C-2021

### Journal
Mit den Journalen zu den verschiedenen Dokumententypen können Sie sich einen Überblick über den Dokumentenbestand verschaffen. Die unterschiedlichen Listen können nach Nummernverwaltern oder nach wählbaren Kriterien erstellt werden.

[Image: Abb. C-226 Journal - Bestandsliste, showing a sample journal report.]

⇨ Softwarereferenz, "Eingangs-/Ausgangs-Journal" auf Seite C-2018

Die Listen stellen folgende Daten dar:
*   **Bestandsliste:**
    bis zu 4 Zeilen pro Dokument
    -   LfNr, Auftragsnummer, Status, Erfassungsdatum, Kundennummer, Kundenname, Stück, Qm, Lfm, Netto-Betrag, EK, Deckungsbeitrag in %
    -   Datum der AB, Brutto-Betrag, MwSt.
    -   Datum und Nummer des Lieferscheins
    -   Datum und Nummer der Rechnung
*   **Ein-/Aus-Liste:**
    1 Zeile pro Dokument
    -   LfNr, Auftragsnummer, Status, Erfassungsdatum, Kundennummer, Kundenname, Stück, Gewicht, Qm, Lfm, Netto-Betrag, EK, Deckungsbeitrag in %
*   **Journal:**
    2 Zeilen pro Dokument
    -   LfNr, Auftragsnummer, Status, Erfassungsdatum, Kundennummer, Kundenname, Stück, Qm, Lfm, Netto-Betrag, EK, Deckungsbeitrag in %
    -   Datum und Nummer der Rechnung, Brutto-Betrag, MwSt.
*   **Rechnungsliste:**
    1 Zeile pro Rechnung/Sammelrechnung
    -   LfNr, Rechnungsnummer, Status, Erfassungsdatum, Kundennummer, Kundenname, Gewicht, Netto-Betrag, MwSt., Brutto-Betrag, EK, Deckungsbeitrag in %
    -   für Sammelrechnungen das Gesamtgewicht der Aufträge
*   **Versandliste:**
    4 Zeilen pro Dokument
    -   LfNr, Auftragsnummer, Status, Erfassungsdatum, Kundennummer, Kundenname, Stück, Qm, Lfm, Gewicht, Netto-Betrag
    -   Datum der AB
    -   Datum und Nummer des Lieferscheins
    -   Datum und Nummer der Rechnung
*   **Produktionsliste:**
    1 Zeile pro Dokument
    -   LfNr, Rechnungsnummer, Status, Erfassungsdatum, Kundennummer, Kundenname, Stück, Gewicht, Laufnummer, Anzahl Sprossen, Anzahl Modelle

Die Listen schließen mit den Gesamtsummen pro Spalte. Wahlweise können Sie sich Zwischensummen pro Kunde, Rechnung und/oder Vertreter bilden lassen.

### Dokumentenüberwachung
Das Zusatzmodul Dokumentenüberwachung prüft in regelmäßigen Intervallen den gesamten Dokumentenbestand in A+W Business. Diese Funktion kann beispielsweise folgende Kriterien berücksichtigen:
*   Angebote, deren Termin zur Wiedervorlage fällig ist.
*   Aufträge, die das Kunden-Kreditlimit überschritten haben und vorläufig für die Weiterbearbeitung gesperrt werden.
*   Aufträge, die vor einer bestimmbaren Frist den Kunden als Auftragsbestätigung zugestellt wurden.
*   Aufträge mit dem Status zur Produktionsfreigabe, um die Einspruchsfrist auf Basis der versendeten Auftragsbestätigungen einzuhalten.
*   Aufträge, deren Produktionsende-Datum überschritten wurde.
*   Aufträge mit Lieferscheinstatus, für die noch keine Rechnung gedruckt wurde.

Dieses Zusatzmodul wird außerhalb der Anwendung A+W Business gestartet (z. B. C:/Programme/A+W/A+W/Business/Program/German/abcAutoStatus.exe).

Die Dokumentenüberwachung startet automatisch. Die Prüfintervalle, die Dokumentenarten und der jeweilige Status (Prüf- und Zielstatus) werden von Ihnen festgelegt.

Das Programm arbeitet im Hintergrund. Werden Dokumente gefunden, die die Prüfkriterien erfüllen, wird automatisch eine entsprechende Meldung angezeigt.

#### Automatische Prüfung auf doppelt erfasste Dokumente
A+W Business prüft automatisch während der Erfassung bzw. Bearbeitung eines Dokumentes, ob schon ein anderes Dokument mit dem gleichen Produkt und Produktaufbau und den gleichen Maßen vorhanden ist. Geprüft werden dabei die Angebote und Aufträge in der Hauptdatenbank. Das Archiv wird nicht durchsucht.

> **i Voraussetzung**
> In der Statusverwaltung muss der Anwender-Status Duplikat vorhanden angelegt sein. Im Modul Utilities müssen die Kriterien der Überwachung angegeben sein.

Hat das Programm ein Duplikat gefunden, wird das neu erfasste Dokument automatisch gesperrt und eine entsprechende Meldung ausgegeben. Über die Funktion Duplikate anzeigen können Sie sich die Duplikate zum aktuellen Dokument auflisten lassen.

Duplikatsprüfungen werden nicht durchgeführt bei Reklamationen, Teillieferungen, Anzahlungen.

Die übergreifenden Duplikatsfilter richten Sie über das Modul Utilities ein. Dort legen Sie folgende Details fest:
*   Erfassungszeitraum in Tagen: Das ist der Zeitbereich, in dem gesucht werden soll.
*   Angaben dazu, was als Vergleichskriterium gelten soll, z. B. Kunde, Hauptprodukt, Produktaufbau, Maße.

---
[Page intentionally left blank]
---

# Softwarereferenz

## A+W Business Verkauf

[Cover Page Image]

---

### In diesem Kapitel finden Sie folgende Themen:
⇨ Übersicht
⇨ Angebot
⇨ Dokumentenverwaltung
⇨ Positionsdaten
⇨ Übersichten und Referenzen zu Kopfdaten
⇨ Übersichten und Referenzen zu Positionen
⇨ Makros
⇨ Nummernverwalter
⇨ Druck
⇨ Übergabe Bestellungen
⇨ Auftrag
⇨ Übergabe, Im-/Export von Dokumenten
⇨ Objektabrechnung
⇨ Auswertungen
⇨ Interne Kontrolle
⇨ Gutschrift
⇨ Journal
⇨ Bestandslisten
⇨ Mahnwesen
⇨ Dokumentendaten
⇨ Lagersuche

| Thema | Seite |
| :--- | :--- |
| Übersicht | C-1659 |
| Angebot | C-1660 |
| Angebot (Dokument) | C-1661 |
| Wiedervorlage | C-1663 |
| Angebotsstatistik | C-1666 |
| Alternativen | C-1668 |
| Menü Optionen | C-1668 |
| Menü Funktionen | C-1669 |
| Alternativen - Original | C-1670 |
| Alternativen - Alternative | C-1673 |
| Alternativen - Texte | C-1674 |
| Alternativen - Bearbeitungen/Modelle | C-1675 |
| Alternativen - Sprossen | C-1676 |
| Alternativangebotsübersicht | C-1677 |
| Dokumente freigeben | C-1678 |
| Dokumentenverwaltung | C-1679 |
| Menüs in der Dokumentenverwaltung | C-1679 |
| Menü Start | C-1679 |
| Menü Ansicht | C-1680 |
| Menü Funktionen | C-1681 |
| Menü Optionen | C-1684 |
| Menü Aufbau | C-1686 |
| Menü Customizing | C-1686 |
| Dokument - Kopfdaten | C-1687 |
| Kopfdaten - Dokument | C-1688 |
| Kopfdaten - Abweichende Anschriften | C-1694 |
| Kopfdaten - Zusatz | C-1696 |
| Kopfdaten - Konditionen | C-1700 |
| Kopfdaten - Texte | C-1704 |
| Kopfdaten - Anlagen | C-1706 |
| Kopfdaten - Technische Parameter | C-1707 |
| Kopfdaten - Kundeninfo | C-1709 |
| Positionsdaten | C-1711 |
| Menüs in der Positionserfassung | C-1711 |
| Menü Start | C-1712 |
| Menü Ansicht | C-1712 |
| Menü Funktionen | C-1714 |
| Menü Optionen | C-1717 |
| Menü Aufbau | C-1722 |
| Menü Customizing | C-1723 |
| Dokument - Positionen | C-1724 |
| Positionen - Position | C-1725 |
| Positionen - Stückliste | C-1736 |
| Positionen - Modelle/Bearbeitungen | C-1740 |
| Positionen - Bearbeitungen | C-1744 |
| Bearbeitung | C-1744 |
| Kantenbearbeitungen, Verklebung | C-1746 |
| Lochbohrungen | C-1747 |
| Senkbohrungen | C-1748 |
| Stufenbohrungen | C-1749 |
| Rundecken | C-1749 |
| Eckausschnitte | C-1750 |
| Schrägecken | C-1750 |
| Randausschnitte, Bogenförmiger Randausschnitt | C-1751 |
| Innenausschnitte, Durchsprechöffnung, Handgriffe | C-1752 |
| Beschichtung, Mattierung, Siebdruck, Flächen-Emaillierung, Sandstrahlen, Kolorieren | C-1754 |
| Randentschichtungen | C-1756 |
| Biegen | C-1756 |
| Rillenschliff | C-1756 |
| Nachschleifen, Kantenschutz | C-1757 |
| Logo, Stempel | C-1757 |
| Makro Ecke, Makro Rand, Parametrisierbares Makro (Kante) | C-1758 |
| Emaillierung | C-1758 |
| Alarmspinne | C-1759 |
| Bleiverglasung | C-1759 |
| Gebogenes Glas | C-1759 |
| Abkleben | C-1759 |
| Entschichtung | C-1759 |
| Randsiebdruck | C-1760 |
| Makro Innen, Parametrisierbares Makro (Innen) | C-1761 |
| Artikel | C-1762 |
| Positionen - Stufung | C-1763 |
| Positionen - Gebogenes Glas | C-1765 |
| Positionen - Bleiverglasungen | C-1767 |
| Positionen - Modell-Template | C-1768 |
| Positionen - Sprossen | C-1770 |
| Sprossen - Standard | C-1771 |
| Sprossen - Preise | C-1776 |
| Sprossen - Wegfallsprossen | C-1778 |
| Sprossen - Muster | C-1779 |
| Positionen - Leistung | C-1780 |
| Positionen - Zusatz | C-1782 |
| Positionen - Weitere Angaben | C-1786 |
| Positionen - Texte | C-1790 |
| Positionen - Anlagen | C-1793 |
| Positionen - Technische Werte | C-1794 |
| Positionen - Klassifikatoren | C-1796 |
| Dokument - Summen | C-1797 |
| Übersichten und Referenzen zu Kopfdaten | C-1802 |
| Dokument suchen | C-1803 |
| Gruppe Suche | C-1803 |
| Dokumente suchen - Auftragsbezogen | C-1804 |
| Dokumente suchen - Positionsbezogen | C-1806 |
| Dokumente suchen - Stücklistenbezogen | C-1807 |
| Dokumente suchen - Tabelle | C-1808 |
| Dokumente suchen - Optionen | C-1810 |
| Dokumente suchen - Detailübersicht | C-1812 |
| Dokumente kopieren | C-1813 |
| Menüs | C-1813 |
| Dokumente kopieren - Kopieren 1:1 | C-1817 |
| Dokumente kopieren - Kopieren positionsweise | C-1823 |
| Dokumente kopieren - Weitere Optionen Zieldokument | C-1825 |
| Dokumente kopieren - Optionen Quelldokument | C-1827 |
| Dokumente kopieren - Texte/Anlagen | C-1828 |
| Dokumente kopieren - Modellparameter | C-1829 |
| Dokument anzeigen | C-1829 |
| Kundeninfo | C-1830 |
| Kapazitätsübersicht | C-1831 |
| Historie | C-1834 |
| Statusänderung | C-1836 |
| NV Auswahl | C-1838 |
| Lagermaße in Kisten verpacken | C-1839 |
| Teillieferungsübersicht | C-1841 |
| Reklamationsübersicht | C-1843 |
| Anzahlungsübersicht | C-1844 |
| Auftrags-/Bestell-Info | C-1845 |
| Duplikate | C-1847 |
| Kundenbenachrichtigung (Lieferterminkontrolle) | C-1848 |
| Menüs | C-1848 |
| Kundenbenachrichtigung - Auswahl | C-1849 |
| Kundenbenachrichtigung – Terminverschiebung | C-1851 |
| Einstellungen für Kundenbenachrichtigungen | C-1852 |
| Kapazitätsinfo nach Kunde | C-1854 |
| OP Abfrage | C-1856 |
| Kreditlimitsperre | C-1857 |
| Kalkulatorische Frachtkosten | C-1858 |
| Kosten- und Aufschlagskalkulation | C-1859 |
| Übersicht Statusrückmeldung | C-1860 |
| Lieferterminbestimmung | C-1862 |
| Liefertermin ändern | C-1863 |
| Zahlungsverwaltung | C-1864 |
| Übersichten und Referenzen zu Positionen | C-1866 |
| Produktsuche | C-1866 |
| Auswahl - Nach Produkt | C-1867 |
| Auswahl - Nach technischen Parametern | C-1869 |
| Auswahl - Nach Klassifikatoren | C-1870 |
| Schnellanfrage | C-1871 |
| Parameter-Ersetzung | C-1873 |
| Produktabgleich | C-1874 |
| Reklamationen | C-1875 |
| Rückschnitt | C-1876 |
| Variantenauswahl (Farbsuche) | C-1877 |
| Festpreis Vorgabe | C-1878 |
| Globale Änderungen | C-1879 |
| Produktionsstücklistenauflösung | C-1880 |
| Konditionen | C-1881 |
| Preis-/Konditionsinformationen | C-1882 |
| Preis-/Konditionsinformationen – Preisabfrage | C-1882 |
| Preis-/Konditionsinformationen – Makropreise | C-1883 |
| Preis-/Konditionsinformationen - Rabatte | C-1884 |
| Preis-/Konditionsinformationen – Autom. Zuschläge | C-1885 |
| Preis-/Konditionsinformationen – Kunde | C-1886 |
| Artikel-Informationen | C-1887 |
| Artikel-Info - Info | C-1888 |
| Artikel-Info - Preise/Lager | C-1889 |
| Artikel-Info - Anlagen | C-1891 |
| Zusatz Stückliste - Ergänzungen | C-1892 |
| Preisrecorder | C-1893 |
| Artikel fixieren | C-1895 |
| Position kopieren | C-1896 |
| Kosten- und Aufschlagskalkulation (Position) | C-1898 |
| Versicherungsleistung | C-1899 |
| Teillieferungen | C-1901 |
| Teillieferungen - Pro Fertigmeldung / Wareneingang | C-1902 |
| Teillieferungen – Pro Gestell | C-1905 |
| Makros | C-1908 |
| Makro sichern | C-1908 |
| Makro ändern | C-1909 |
| Makro suchen | C-1911 |
| Makro kopieren | C-1912 |
| Nummernverwalter | C-1914 |
| Menü Funktionen | C-1914 |
| Nummernverwalter | C-1917 |
| Nummernverwalter - Sortierung | C-1919 |
| Nummernverwalter kopieren | C-1920 |
| Bestellkennzeichen ändern | C-1921 |
| Druck | C-1923 |
| Menüs im Formular-/Etikettendruck | C-1923 |
| Menü Funktionen | C-1923 |
| Menü Optionen | C-1924 |
| Formular-/Etikettendruck | C-1926 |
| Formular-/Etikettendruck - Formulare | C-1927 |
| Formular-/Etikettendruck - Etiketten | C-1933 |
| Formular-/Etikettendruck - Dokumentenexport | C-1935 |
| Vermaßte Skizze drucken | C-1936 |
| Touren/Fahrer Zuordnung | C-1939 |
| Übergabe Bestellungen | C-1940 |
| Bestellübergabe | C-1940 |
| Menü Funktionen | C-1940 |
| Menü Optionen | C-1941 |
| Bestellübergabe - Bestellnummern | C-1943 |
| Bestellübergabe - Bestellpool | C-1946 |
| Lieferant und Liefertermin ändern | C-1949 |
| Markierungsoptionen | C-1950 |
| Preisvergleich | C-1951 |
| Erweiterte Einstellungen | C-1953 |
| Erweiterte Einstellungen - Allgemein | C-1954 |
| Erweiterte Einstellungen - Sortierung | C-1955 |
| Stücklistenübersicht | C-1957 |
| Auftrag | C-1958 |
| Anzahlungen | C-1961 |
| Bankbelege | C-1962 |
| Überrechnen | C-1964 |
| TPS Faktura | C-1966 |
| Garantiebelege | C-1966 |
| SAFT-PT Export | C-1966 |
| Übergabe, Im-/Export von Dokumenten | C-1967 |
| FiBu-Übergabe | C-1967 |
| Menü Funktionen | C-1968 |
| Menü Optionen | C-1968 |
| Sollstellung FiBu | C-1970 |
| Einstellungen FiBu-Übergabe | C-1972 |
| Import/Export von Zahlungen | C-1973 |
| Übergabe Archiv | C-1974 |
| Import | C-1976 |
| Fehlende Referenzen | C-1978 |
| Dokumente erstellen | C-1979 |
| Fremddokumentenverwaltung | C-1980 |
| Objektabrechnung | C-1981 |
| Abrechnung | C-1981 |
| Menü Funktionen | C-1982 |
| Menü Druck | C-1982 |
| Objekte - Abrechnungen | C-1983 |
| Objekte - Rahmenauftrag | C-1986 |
| Objekte - Zugeordnete Aufträge | C-1987 |
| Objekte - Zugeordnete Bestellungen | C-1988 |
| Objekte - Summen | C-1989 |
| Objekte - Veranschlagte Mengen | C-1990 |
| Objekte - Tabelle | C-1991 |
| Objekte - Dokumente | C-1992 |
| Stundenforderung | C-1993 |
| Einkaufsforderung | C-1994 |
| Forderungsberechnung | C-1995 |
| Forderungs-Historie | C-1997 |
| Auswertungen | C-1998 |
| Preisänderung (Report) | C-1998 |
| Null-Preisreport | C-2000 |
| Deckungsbeitrags-Analyse | C-2002 |
| Deckungsbeitrags-Analyse – Auswahl | C-2003 |
| Deckungsbeitrags-Analyse - Tabelle | C-2005 |
| Kalkulatorische Frachtkosten | C-2006 |
| Kalkulatorische Frachtkosten - Druck | C-2007 |
| Kalkulatorische Frachtkosten - Speditionskosten | C-2009 |
| Interne Kontrolle | C-2011 |
| Gutschriftgründe | C-2011 |
| Änderungen am Kundenstamm | C-2012 |
| Preis-/Rabattänderungen | C-2013 |
| Verspätete Lieferung/Lieferung ohne Berechnung | C-2014 |
| Gutschrift | C-2016 |
| Gutschrift (Dokumentenverwaltung) | C-2017 |
| Journal | C-2018 |
| Eingangs-/Ausgangs-Journal | C-2018 |
| Bestandslisten | C-2021 |
| Nummernbereiche | C-2021 |
| Warengruppen | C-2023 |
| Mahnwesen | C-2025 |
| Menüs im Dialog Mahnwesen | C-2025 |
| Menü Zahlung | C-2025 |
| Menü Optionen | C-2025 |
| Menü Funktionen | C-2026 |
| Mahnwesen | C-2026 |
| Mahnstufen | C-2028 |
| Offene-Posten-Tabelle füllen | C-2029 |
| Dokumentendaten | C-2030 |
| Menüs im Dialog Dokumente | C-2030 |
| Menü Funktionen | C-2030 |
| Menü Optionen | C-2030 |
| Dokumentendaten | C-2031 |
| Lagersuche | C-2034 |
| Lagerinfo | C-2034 |
| Lagerinfo - Lagersuche | C-2035 |
| Lagerinfo - Zukünftiger Lagerbestand | C-2038 |
| Dokumentenübersicht | C-2039 |

## Übersicht

In der Dokumentenverwaltung können Sie alle Dokumente erfassen und bearbeiten, die im Rahmen des Verkaufs benötigt werden. Das sind Angebote, Aufträge, Lieferungen, Rechnungen, Gutschriften und Reklamationen. Außerdem können Sie in diesem Modul Bestellungen erfassen und bearbeiten.

Dokumente enthalten zwei Gruppen von Daten: Angaben zum Kunden und die Auftragspositionen. Diese Daten werden in unterschiedlichen Dialogen erfasst.

In der Softwarereferenz finden Sie Informationen zu folgenden Themen:
*   Angebot
*   Alternativen
*   Dokumentenverwaltung
*   Positionsdaten
*   Übersichten und Referenzen zu Kopfdaten
*   Übersichten und Referenzen zu Positionen
*   Dokumente kopieren
*   Makros
*   Nummernverwalter
*   Druck
*   Übergabe Bestellungen
*   Auftrag
*   Übergabe, Im-/Export von Dokumenten
*   Auswertungen
*   Interne Kontrolle
*   Gutschrift
*   Journal
*   Bestandslisten
*   Mahnwesen
*   Dokumentendaten
*   Lagersuche

> **i Dialoge können von unterschiedlichen Stellen aus geöffnet werden**
> Bitte beachten Sie, dass viele Funktionen zum Thema Verkauf in A+W Business aus unterschiedlichen Dialogen heraus gestartet werden können. In dieser Anleitung werden die entsprechenden Dialoge nur einmal beschrieben.

## Angebot

`Dokumente > Angebot`

Über das Menü Angebot erreichen Sie sich folgende Programmpunkte:
*   **NV Angebot:**
    Die Funktion des Nummernverwalters ist für alle Dokumente gleich. Sie wird am Beispiel Auftrag beschrieben.
    ⇨ "Nummernverwalter" auf Seite C-1917
*   **Angebot:**
    In diesem Dialog erfassen und bearbeiten Sie Angebote. Die Erfassung von Dokumenten ist für alle Dokumentenarten gleich. Sie wird am Beispiel Auftrag beschrieben.
    ⇨ "Dokument - Kopfdaten" auf Seite C-1687
*   **Druck Angebote:**
    Der Formular- und Etikettendruck ist für alle Dokumente gleich. Er wird am Beispiel Auftrag beschrieben.
    ⇨ "Druck" auf Seite C-1923
*   **Wiedervorlage:**
    Mit dieser Funktion lassen Sie sich eine Übersicht über alle Dokumente anzeigen, die mit einem Datum zur Wiedervorlage gekennzeichnet sind.
    ⇨ "Wiedervorlage" auf Seite C-1663
*   **Journal:**
    Der Journaldruck ist für alle Dokumente gleich. Er wird am Beispiel Auftrag beschrieben.
    ⇨ "Journal" auf Seite C-2018
*   **Übergabe Archiv:**
    Die Archivübergabe ist für alle Dokumente gleich. Sie wird am Beispiel Auftrag beschrieben.
    ⇨ "Übergabe Archiv" auf Seite C-1974
*   **Suche:**
    Die Suche ist für alle Dokumente gleich. Sie wird am Beispiel Auftrag beschrieben.
    ⇨ "Dokument suchen" auf Seite C-1803
*   **Angebotsstatistik:**
    In einer Übersicht können Sie sich die Angebote eines selbst gewählten Zeitraums anzeigen lassen.
    ⇨ "Angebotsstatistik" auf Seite C-1666
*   **Import:**
    Mit dieser Funktion werden elektronische Kunden-Aufträge importiert.
    ⇨ "Import" auf Seite C-1976

### Angebot (Dokument)
`Dokumente > Angebot > Angebot auswählen`

[Image: Abb. C-227 Angebot, showing the main offer creation dialog.]

In diesem Dialog erfassen und bearbeiten Sie Angebote.
Die Felder sind für alle Dokumententypen gleich. Eine ausführliche Beschreibung finden Sie unter:
⇨ "Dokument - Kopfdaten" auf Seite C-1687
⇨ "Dokument - Positionen" auf Seite C-1724

Für ein Angebot stehen zusätzlich folgende Felder zur Verfügung:

#### Kopfdaten - Register Dokumente

**Vorlage** Datum, mit dem das Angebot auf Wiedervorlage gesetzt wird. Wenn der Tag erreicht ist, wird beim Start von A+W Business automatisch eine Meldung angezeigt. Sie können dann entscheiden, ob Sie das Angebot sofort öffnen möchten.
⇨ "Wiedervorlage" auf Seite C-1663

#### Kopfdaten - Register Zusatz

**Kategorie** Durch die Kategorie kann ein Angebot nach verschiedenen Ablehnungsgründen klassifiziert werden, z. B. zu teuer, keine Rückmeldung. Über die Kategorie können Angebote in der Statistik ausgewertet werden.

#### Positionen - Register Zusatz

**Alternative zur Pos.** Sie können festlegen, dass die markierte Position alternativ zu der Position gelten soll, die Sie hier auswählen. Diese Alternative wird nicht im Gesamtpreis berücksichtigt.
Alternativpositionen werden wie alle anderen Positionen erfasst und angezeigt. Im Druck werden sie entsprechend gekennzeichnet.
⇨ Tutorial, "Alternative Position im Angebot erfassen" auf Seite C-1593

### Wiedervorlage
`Dokumente > Angebot > Wiedervorlage`

[Image: Abb. C-228 Angebot - Wiedervorlage, showing the follow-up management dialog.]

In diesem Dialog lassen Sie sich eine Übersicht über alle Dokumente anzeigen, die mit einem Datum zur Wiedervorlage gekennzeichnet sind.

In den Firmendaten können Sie für die Wiedervorlage eine Frist für Angebote und/oder Aufträge eintragen.
⇨ Tutorial, "Angebotsverfolgung" auf Seite C-1604
⇨ Stammdaten, "Firmendaten - System" auf Seite B-1113

> **i Anzeige zur Wiedervorlage einschränken**
> Die Anzeige der Dokumente in der Wiedervorlage kann durch ein Anwenderrecht auf die vom Anwender erfassten Dokumente eingeschränkt werden. Das kann z. B. dann sinnvoll sein, wenn ein Vertreter nicht die Dokumente der anderen Vertreter in der Wiedervorlage sehen darf.

#### Menü Funktionen
*   **Historie:**
    Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des Dokuments.
    ⇨ "Historie" auf Seite C-1834
*   **Alternativangebotsübersicht:**
    Öffnet die Liste der Angebotsalternativen zum aktuellen Angebot oder Auftrag.
    ⇨ "Alternativangebotsübersicht" auf Seite C-1677

#### Menü Optionen
*   **Mitarbeiter und Datum vorblenden:**
    Der Dialog wird im Auswahlmodus geöffnet. Das aktuelle Tagesdatum und der in A+W Business angemeldete Mitarbeiter sind vorbelegt.
*   **Automatische Benachrichtigung:**
    Wenn der Termin zur Wiedervorlage eines bestimmten Dokuments erreicht ist, wird eine entsprechende Meldung angezeigt, wenn der Erfasser des Angebots sich anmeldet.

#### Dokument

**Nummer** Nummer des Angebots, das auf Wiedervorlage gesetzt ist.

**Vorlagedatum, bis** Zeitraum zum Eingrenzen der Suche nach Wiedervorlagen.

**Erfassung** Datum, an dem das Dokument erfasst wurde, das auf Wiedervorlage gesetzt ist.

**Texte** Eingabefeld für Anmerkungen zum Dokument, z. B. Hinweise auf Ansprechpartner.

**AV-Bereich** AV-Bereich, dem das Dokument zugeordnet ist.
⇨ Tutorial, "AV-Bereich" auf Seite C-1297

**Fachberater** Name des zuständigen Fachberaters.

**Bearbeiter** Mitarbeiter, der das Dokument erfasst hat.

**Vertreter** Name des zuständigen Vertreters.

**Kunde** Nummer und Name des Kunden.

**Betrag brutto, netto** Beträge des Angebotswerts.

**Status** Status des Dokuments, das auf Wiedervorlage gesetzt ist.

**Typ** Typ des Dokuments, das auf Wiedervorlage gesetzt ist.

**Kategorie** Durch die Kategorie kann ein Angebot nach verschiedenen Ablehnungsgründen klassifiziert werden, z. B. zu teuer, keine Rückmeldung. Über die Kategorie können Angebote in der Statistik ausgewertet werden.

#### Neuer Status

**Übergabe Archiv** Für die Übergabe von Dokumenten an das Archiv muss der Status entsprechend gesetzt sein. In der Regel wird der Status automatisch hochgesetzt. Sie können ihn auch manuell hochsetzen.
- Der Status des angezeigten Angebots wird nicht hochgesetzt.
- Der Status des angezeigten Angebots wird hochgesetzt, das Angebot kann archiviert danach werden.
  ⇨ Tutorial, "Archivierung" auf Seite C-1631
  ⇨ Übergabe Archiv

**Löschfreigabe** Dokumente sollten aus der Hauptdatenbank gelöscht werden, sobald sie archiviert sind. Sie verhindern damit, dass die Hauptdatenbank zu groß wird.
Dieses Feld ist gesperrt, wenn der Status eines markierten Dokuments größer ist als der Lösch-Status, oder wenn das Dokument einen exklusiven Status hat.
- Der Status des angezeigten Angebots wird nicht hochgesetzt, das Angebot kann nicht gelöscht werden.
- Der Status des angezeigten Angebots wird hochgesetzt, das Angebot kann danach gelöscht werden.
  ⇨ Stammdaten, "Automatikoptionen" auf Seite B-1108

**Vorlage alle, min** Sie können die Wiedervorlage in definierten Intervallen anzeigen lassen. Das Feld min (Minuten) ist nur freigeschaltet, wenn die Checkbox alle markiert ist.
- Das Angebot wird nicht automatisch erneut angezeigt. Das Feld min ist gesperrt.
- Das Angebot wird automatisch im angegebenen Intervall angezeigt. Im Feld min kann das Intervall in Minuten angegeben werden. Das Intervall darf nicht kleiner als 5 Minuten sein.

#### Tabelle
Liste aller Angebote, die den Auswahlkriterien entsprechen.

### Angebotsstatistik
`Dokumente > Angebot > Angebotsstatistik`

[Image: Abb. C-229 Angebotsstatistik, showing the offer statistics report dialog.]

In diesem Dialog lassen Sie sich eine Auswertung über die Angebote eines selbst gewählten Zeitraums anzeigen.
⇨ Tutorial, "Angebotsstatistik" auf Seite C-1610

#### Selektion
**Erfassung von, bis** Zeitraum, aus dem archivierte Angebote angezeigt werden sollen. Es spielt keine Rolle, in welchem der beiden Felder Sie das jüngere Datum eintragen.
**Kunde** Nummer und Name des Kunden.
**AV-Bereich** Auswahl des AV-Bereichs, dem das Dokument zugeordnet ist.
⇨ Stammdaten, "Basistabelle erweitern" auf Seite B-93
**Erfasser** Auswahl des Mitarbeiters, der das Dokument erfasst hat.
**Fachberater** Auswahl des zuständigen Mitarbeiters.
**Außendienst** Auswahl des zuständigen Vertreters.
**Kategorie** Durch die Kategorie kann ein Angebot nach verschiedenen Ablehnungsgründen klassifiziert werden, z. B. zu teuer, keine Rückmeldung. Über die Kategorie können Angebote ausgefiltert werden.
**Dokumententyp** Auswahl des Dokumententyps, dem das Dokument zugeordnet ist.
**Branche** Auswahl der Branche, der das Dokument zugeordnet ist.
**Region** Auswahl der Region, der das Dokument zugeordnet ist.

#### Archive
Anzeige aller verfügbaren A+W Business-Archive. Das gewünschte Archiv markieren Sie mit einem einfachen Klick. Wenn Sie erneut auf den markierten Eintrag klicken, wird die Markierung aufgehoben.
Sie können mehrere Archive gleichzeitig markieren und durchsuchen lassen.

#### Auswertung Anzahl, Betrag
**Angebote** Anzeige der gefundenen Angebote und deren Gesamtsumme.
**In Aufträge überführt** Anzeige der Angebote, die in Aufträge überführt wurden.
**Quote** Verhältnis der erstellen Angebote zu den daraus entstandenen Aufträgen.
**Aufträge** Anzahl und Gesamtsumme der im gleichen Zeitraum archivierten Aufträge.

#### Detailauswertung
Sie können die Anzeige der Spalten über die Tabelleneigenschaften einstellen. Für eine detailliertere Auswertung können Sie sich alle Spalten anzeigen lassen.
- Nur die Spalten werden angezeigt, die in den Tabelleneigenschaften aktiviert sind.
- Alle verfügbaren Spalten werden angezeigt.

#### Details
Liste der archivierten Angebote, die die Suchkriterien erfüllen.

### Alternativen
`Dokumente > Angebot > Angebot auswählen > Menü Funktionen > Gruppe Dokument > Alternativen`

Sie können ein Angebot insgesamt als Alternative überarbeiten, z. B. um eine ISO-Scheibe mit einer alternativen Kombination von SZR und Gas anzubieten. Sie können auch einen gesamten Auftrag als Alternative überarbeiten, z. B. um Fehler zu bereinigen.
⇨ Tutorial, "Alternativangebot" auf Seite C-1591

Die Alternativen zu einem Angebot können Sie sich in einer Übersicht anzeigen lassen.
⇨ "Alternativangebotsübersicht" auf Seite C-1677

> **i Alternativpositionen**
> Alternative Positionen werden im Angebot als eigene Positionen eingefügt und entsprechend gekennzeichnet.
> ⇨ Tutorial, "So erfassen Sie eine alternative Position" auf Seite C-1593

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menü Optionen" auf Seite C-1668
*   "Menü Funktionen" auf Seite C-1669
*   "Alternativen – Original" auf Seite C-1670
*   "Alternativen - Alternative" auf Seite C-1673
*   "Alternativen - Texte" auf Seite C-1674
*   "Alternativen - Bearbeitungen/Modelle" auf Seite C-1675
*   "Alternativen - Sprossen" auf Seite C-1676

#### Menü Optionen
`Dokumente > Angebot > Angebot auswählen > Menü Funktionen > Gruppe Dokument > Alternativen > Menü Optionen`

Folgende Einträge werden im Menü Optionen angezeigt:
*   **Datumsfelder aktualisieren:** Die Datumsfelder werden automatisch aktualisiert, wenn das Alternativangebot gespeichert wird.

#### Menü Funktionen
`Dokumente > Angebot > Angebot auswählen > Menü Funktionen > Gruppe Dokument > Alternativen > Menü Funktionen`

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Dialog zu schließen. Folgende Einträge werden angezeigt:
*   **Alternativangebotsübersicht:** Öffnet die Liste der Angebotsalternativen zum aktuellen Angebot. Die Funktion ist nur in Angeboten freigeschaltet.
    ⇨ "Alternativangebotsübersicht" auf Seite C-1677
*   **Dokumentendaten:** Öffnet den Dialog Dokumente, um ggf. die Termine und den Status in Aufträgen und Bestellungen zu korrigieren.
    ⇨ "Dokumentendaten" auf Seite C-2030
*   **Lagersuche:** Öffnet den Dialog Lagerinfo, um die aktuellen Lagerbestände anzuzeigen.
    ⇨ "Lagerinfo - Lagersuche" auf Seite C-2035

### Alternativen – Original
`Dokumente > Angebot > Angebot auswählen > Menü Funktionen > Gruppe Dokument > Alternativen > Register Original`

[Image: Abb. C-230 Alternativen – Original, showing the 'Original' tab in the alternatives dialog.]

In diesem Register werden die Daten der Original-Position des Angebots angezeigt.
⇨ Tutorial, "Alternatives Angebot erfassen" auf Seite C-1596

#### Original
**Originalnummer gleich Alternative** Das Dokument kann entweder vollständig überschrieben werden oder es wird ein alternatives (neues) Dokument mit einer eigenen Dokumentennummer erstellt.
- Das Alternativdokument erhält eine eigene Dokumentennummer.
- Das Original-Dokument wird überschrieben.

**(Übersicht)** In der Übersicht werden alle Positionen des Original-Dokuments aufgelistet.

**(rotes Kästchen)** Bei Aufträgen, die als Alternative überarbeitet werden, sind die Positionen in roter Schrift angezeigt, die bereits an die Bestellungen übergeben sind. Bei diesen Positionen kann als Alternative nur ein anderer Preis erfasst werden.

#### Modus
**(Kombobox)** Liste aller Möglichkeiten, zu denen Alternativen erfasst werden können.

**[Definition]** Die Schaltfläche ist nur bei der Wahl von Modell, Sprosse oder Bearbeitung freigeschaltet. Sie öffnen mit ihr die zugehörigen Dialoge, um die alternativen Werte zu erfassen.
⇨ "Positionen - Modelle/Bearbeitungen" auf Seite C-1740
⇨ "Positionen - Bearbeitungen" auf Seite C-1744
⇨ "Positionen - Sprossen" auf Seite C-1770

#### Suchen von
In diesem Bereich tragen Sie die Nummer des Original-Produkts ein. Die Bezeichnungen aus den Stammdaten werden angezeigt.

#### Einfügen, ersetzen durch
In diesem Bereich können Sie ein alternatives Produkt eintragen. An dieser Stelle steht Ihnen auch die Sternchenfunktion (*) als Suche zur Verfügung. Wenn die Nummer eingetragen ist, werden in den Feldern die Bezeichnungen aus den Stammdaten angezeigt.
Das Eingabefeld wird nur angezeigt, wenn Sie Alternativen zum Hauptprodukt oder zu den Gläsern anbieten wollen. Bei Sprossen, Modellen und Bearbeitungen werden die Angaben aus den entsprechenden Dialogen übernommen.

**[Kopieren]** Die Schaltfläche ist nur freigeschaltet, wenn die Checkbox Originalnummer gleich Alternative nicht markiert ist. Sie können damit einzelne Positionen in das Alternativangebot kopieren.

**[Einfügen/Ersetzen]** Mit dieser Schaltfläche übernehmen Sie das alternative Produkt.

**[Preisberechnung]** Mit dieser Schaltfläche starten Sie die Preisberechnung für jeden Modus einzeln, in dem Sie Alternativen erfasst haben.

#### Verkaufspreise
**Jahrgang** Sie können zu jedem Modus einen anderen Preisjahrgang auswählen.
**Schlüssel** Sie können zu jedem Modus einen anderen Preisschlüssel auswählen.
**Preis / PE** Sie können zu jedem Modus einen manuellen Preis pro Preiseinheit erfassen.
**Rabatt** Sie können zu jedem Modus einen Rabatt erfassen.

**[Zurücksetzen]** Mit dieser Schaltfläche setzten Sie die manuellen Preisvorgaben zurück.

**Sonstige Preisvorgaben löschen** Sie können für die Alternativangebote die manuellen Preisvorgaben aus den Original-Positionen löschen.
- Die Preisvorgaben aus den Original-Positionen gelten auch für das Alternativangebot.
- Die manuellen Preisvorgaben aus den Original-Positionen werden für das Alternativangebot gelöscht.

### Alternativen – Alternative
`Dokumente > Angebot > Angebot auswählen > Menü Funktionen > Gruppe Dokument > Alternativen > Register Alternative`

[Image: Abb. C-231 Alternativen - Alternative, showing the 'Alternative' tab with a price comparison.]

In diesem Register werden die Alternativen angezeigt. Dazu erhalten Sie am Ende der Tabelle einen Vergleich über den VK, EK und den Deckungsbetrag vorher (Original-Dokument) und nachher (Alternative).
Die Preise werden erst aktualisiert, wenn Sie die Preisberechnung im Register Original gestartet haben.

### Alternativen – Texte
`Dokumente > Angebot > Angebot auswählen > Menü Funktionen > Gruppe Dokument > Alternativen > Register Texte`

[Image: Abb. C-232 Alternativen - Texte, showing the text editor for adding notes to the alternative.]

In diesem Register können Sie zu den Alternativen einen gesonderten Text hinterlegen.
⇨ Tutorial, "Text erfassen" auf Seite C-1308

### Alternativen – Bearbeitungen/Modelle
`Dokumente > Angebot > Angebot auswählen > Menü Funktionen > Gruppe Dokument > Alternativen > Register Bearbeitungen/Modelle`

[Image: Abb. C-233 Alternativen - Bearbeitungen/Modelle, showing the dialog for defining an alternative model/processing.]

In diesem Register können Sie eine Alternative zu einem Modell erfassen.
⇨ Tutorial, "Modell erfassen" auf Seite C-1368
⇨ Tutorial, "Bearbeitung erfassen" auf Seite C-1373
Die Felder sind ausführlich zu den Positionsdaten beschrieben:
⇨ "Positionen - Modelle/Bearbeitungen" auf Seite C-1740

### Alternativen – Sprossen
`Dokumente > Angebot > Angebot auswählen > Menü Funktionen > Gruppe Dokument > Alternativen > Register Sprossen`

[Image: Abb. C-234 Alternativen – Sprossen, showing the dialog for defining alternative muntins.]

In diesem Register können Sie eine Alternative zu einer Sprossenkonstruktion erfassen.
⇨ Tutorial, "Sprossen erfassen" auf Seite C-1363
Die Felder sind ausführlich zu den Positionsdaten beschrieben:
⇨ "Positionen - Sprossen" auf Seite C-1770

### Alternativangebotsübersicht
`Dokumente > Angebot > Angebot auswählen > Menü Funktionen > Gruppe Dokumentenübersicht > Alternativen`

[Image: Abb. C-235 Alternativangebotsübersicht, showing a list of alternative offers for an original offer.]

In diesem Dialog werden die Alternativangebote zum aktuellen Angebot (oder Auftrag) aufgelistet.
In der ersten Zeile sind in roter Schrift die Angebotsnummer und der Kundenname des Original-Angebots angezeigt.
Die Alternativangebote sind darunter angezeigt.
In der Tabelle werden Details zu dem Dokument angezeigt, das in der Anzeige markiert ist.
⇨ Tutorial, "Alternativangebot" auf Seite C-1591

### Dokumente freigeben
`Dokumente > Auftrag, Bestellung > Auftrag, Bestellung > Dokument öffnen > Menü Funktionen > Gruppe Dokument > Dokument freigeben`

[Image: Abb. C-236 Gesperrte Dokumente freigeben (Kundenverwaltung), showing the dialog to release locked documents.]

In dem Dialog können Sie Dokumente mit Kreditlimit- oder Duplikatssperre freigeben. In den entsperrten Dokumenten wird der Status aktualisiert.
Die gesperrten Dokumente eines Kunden können Sie auch in der Kundenverwaltung freigeben.
⇨ Stammdaten, “Partnerverwaltung" auf Seite B-887

> **i Voraussetzungen**
> Der Mitarbeiter muss das Recht zum Löschen der Sperren haben.
> Die Statuspunkte müssen zugeordnet sein.
> Das Recht 1338 - Dokumente - Funkt. - Dokumente freigeben wird dem Mitarbeiter in der Rechtverwaltung zugewiesen.
> ⇨ Stammdaten, "Mitarbeiterrechte" auf Seite B-1156
>
> Folgende müssen Statuspunkte zugeordnet sein:
> *   Statuspunkt 701 - Kreditlimitsperre gelöscht
> *   Statuspunkt 170 - Duplikatssperre gelöscht
> ⇨ Stammdaten, "Statuszuordnung" auf Seite B-1022

## Dokumentenverwaltung
`Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung`

Der Dialog Dokumentenverwaltung und die zugehörigen Menüs sind für alle Dokumentenarten gleich. Er wird in dieser Anleitung am Beispiel Auftrag beschrieben.

In diesem Dialog finden Sie folgende Hauptregister (seitlich):
*   "Dokument - Kopfdaten" auf Seite C-1687
*   "Dokument - Positionen" auf Seite C-1724
*   "Dokument - Summen" auf Seite C-1797

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menüs in der Dokumentenverwaltung" auf Seite C-1679
*   "Dokument - Kopfdaten" auf Seite C-1687

### Menüs in der Dokumentenverwaltung
`Dokumente > Auftrag > Auftrag auswählen > Register Kopfdaten`

Über die Menüs der Dokumentenverwaltung können Sie die Standardeinstellung des Dialoges bestimmen und andere Dialoge öffnen, ohne die Dokumentenverwaltung zu schließen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menü Start" auf Seite C-1679
*   "Menü Ansicht" auf Seite C-1680
*   "Menü Funktionen" auf Seite C-1681
*   "Menü Optionen" auf Seite C-1684
*   "Menü Aufbau" auf Seite C-1686
*   "Menü Customizing" auf Seite C-1686

#### Menü Start
Die Standard-Menüeinträge sind im Part Überblick erklärt.
⇨ Überblick, "Benutzeroberfläche" auf Seite A-26

##### Gruppe Druck
`Dokumente > Auftrag > Auftrag auswählen > Menü Start > Gruppe Druck`

In diesem Menü wird standardmäßig der Eintrag Allgemeiner Formulardruck angezeigt. Eigene Auftragsformulare für den Direktdruck werden im Eintrag Direktdruck angezeigt. Nur jeweils die Auftragsformulare für den Direktdruck werden angezeigt, die dem aktuellen Dokumententyp entsprechen.
Die Gruppe ist nur im Register Kopfdaten freigeschaltet.

Mit Klick auf den Eintrag Direktdruck wird der Dialog Formularauswahl geöffnet, in dem die eigenen Auftragsformulare aufgelistet sind. Bei der Wahl einer dieser Einträge wird der Dialog Formular-/Etikettendruck nicht geöffnet. Der Druck startet sofort.
⇨ "Formular-/Etikettendruck" auf Seite C-1926
⇨ Stammdaten, "Auftragsformulare" auf Seite B-1213

#### Menü Ansicht
`Dokumente > Auftrag > Auftrag auswählen > Register Kopfdaten > Menü Ansicht`

Das Menü ist in folgende Gruppen gegliedert:
*   Gruppe Preise
*   Gruppe Konditionen
*   Gruppe Dokument
*   Gruppe Position
*   Gruppe Produktion
*   Gruppe Kapazitätsübersicht

##### Gruppe Preise
Diese Gruppe ist nur im Register Positionen freigeschaltet.
⇨ "Gruppe Preise" auf Seite C-1712

##### Gruppe Konditionen
Diese Gruppe ist nur im Register Positionen freigeschaltet.
⇨ "Gruppe Konditionen" auf Seite C-1713

##### Gruppe Dokument
*   **Dokument anzeigen:**
    Öffnet den Dialog Dokumentenansicht als Vorschau auf das Dokument.
    ⇨ "Dokument anzeigen" auf Seite C-1829
*   **Kundeninfo:**
    Öffnet einen Dialog mit einer Kurzinfo zum Kunden.
    ⇨ "Kundeninfo" auf Seite C-1830

##### Gruppe Position
Diese Gruppe ist nur im Register Positionen freigeschaltet.
⇨ "Gruppe Position" auf Seite C-1713

##### Gruppe Produktion
Über diese Option können Sie sich eine Übersicht über die Rückmeldungen aus der Produktion anzeigen lassen.
Die Option ist gesperrt, wenn Sie im aktuellen Dokument keine Positionen enthalten sind, die an die Produktion übergeben werden sollen.
⇨ "Übersicht Statusrückmeldung" auf Seite C-1860

##### Gruppe Kapazitätsübersicht
Diese Gruppe ist nur freigeschaltet, wenn Sie mit A+W Business Capacity Planner und A+W Capa View arbeiten.
Über diese Option können Sie sich eine Übersicht über die freien und belegten Kapazitäten aus A+W Business Capacity Planner anzeigen lassen.
⇨ "Kapazitätsübersicht" auf Seite C-1831

#### Menü Funktionen
`Dokumente > Auftrag > Auftrag auswählen > Register Kopfdaten > Menü Funktionen`

##### Gruppe Dokument
Diese Gruppe ist nur im Register Kopfdaten freigeschaltet.
*   **Historie:** Öffnet eine Übersicht über die Verarbeitungen und Statusänderungen des Dokuments.
    ⇨ "Historie" auf Seite C-1834
*   **Statusänderung:** Öffnet den Dialog Statusänderung, um den Status manuell umzusetzen.
    ⇨ "Statusänderung" auf Seite C-1836
*   **NV Auswahl:** Öffnet den Dialog Auswahl, um den Nummernverwalter auszuwählen, in dem das aktuelle Dokument verwaltet werden soll.
    ⇨ "NV Auswahl" auf Seite C-1838
    Der gültige Nummernverwalter wird über der Liste der Dokumente angezeigt.
    ⇨ Tutorial, "Dialog Dokumentenverwaltung" auf Seite C-1294
*   **Dokumente kopieren:** Öffnet den Dialog Dokumente kopieren, um ein Dokument in den gleichen oder anderen Dokumententyp kopieren.
    ⇨ "Dokumente kopieren" auf Seite C-1813
*   **Teillieferung:** Öffnet den Dialog Dokumente kopieren im Modus Teillieferung, um eine Teillieferung zu erfassen.
    ⇨ "Dokumente kopieren" auf Seite C-1813
*   **Reklamation:** Öffnet den Dialog Dokumente kopieren im Modus Reklamation, um eine Reklamation zu erfassen.
    ⇨ "Dokumente kopieren" auf Seite C-1813
*   **Anzahlungen:** Öffnet den Dialog Dokumente kopieren im Modus Anzahlung, um eine Anzahlung zu erfassen.
    ⇨ "Dokumente kopieren" auf Seite C-1813
*   **Alternativen:** Öffnet den Dialog Alternativen, um ein alternatives Angebot zu erfassen.
    ⇨ "Alternativen" auf Seite C-1668
*   **Anschrift ändern:** Wechselt zum Register Dokument, um die Anschrift zu ändern.
*   **Dokument freigeben:** Öffnet den Dialog Dokumente freigeben, um eine Sperre aufzuheben.
    ⇨ "Dokumente freigeben" auf Seite C-1678
*   **Lagermaße in Kisten verpacken:** Öffnet den Dialog Lagermaße in Kisten verpacken.
    ⇨ "Lagermaße in Kisten verpacken" auf Seite C-1839

##### Gruppe Dokumentenübersicht
*   **Teillieferung:** Öffnet die Liste der Teillieferungen zum aktuellen Auftrag. Die Funktion ist nur freigeschaltet, wenn zu dem aktuellen Dokument Teillieferungen erstellt wurden oder wenn das Dokument eine Teillieferung ist.
    ⇨ "Teillieferungsübersicht" auf Seite C-1841
*   **Alternativen:** Öffnet die Liste der Angebotsalternativen zum aktuellen Angebot. Die Funktion ist nur in Angeboten freigeschaltet.
    ⇨ "Alternativangebotsübersicht" auf Seite C-1677
*   **Reklamation:** Öffnet die Liste der Reklamationen zu einem Auftrag. Die Funktion ist nur in Reklamationen freigeschaltet.
    ⇨ "Reklamationsübersicht" auf Seite C-1843
*   **Anzahlungen:** Öffnet die Übersicht über die geleisteten Anzahlungen zum aktuellen Auftrag.
    ⇨ "Anzahlungsübersicht" auf Seite C-1844

##### Gruppe Info
*   **Auftrags-/Bestell-Info:** Öffnet die Übersicht über Aufträge und die zugehörigen Bestellungen.
    ⇨ "Auftrags-/Bestell-Info" auf Seite C-1845
*   **Dokumentendaten:** Öffnet den Dialog Dokumente, um ggf. die Termine und den Status in Aufträgen und Bestellungen zu korrigieren.
    ⇨ "Dokumentendaten" auf Seite C-2030
*   **Lagersuche:** Öffnet den Dialog Lagerinfo, um den aktuellen Bestand und die reservierten Mengen eines Produkts anzuzeigen.
    ⇨ "Lagerinfo - Lagersuche" auf Seite C-2035
*   **Lagervorschau:** Öffnet den Dialog Lagerinfo, um den zukünftigen Bestand und die reservierten Mengen eines Produkts anzuzeigen.
    ⇨ "Lagerinfo - Zukünftiger Lagerbestand" auf Seite C-2038
*   **Artikel Info:** Öffnet den Dialog Artikelinfo, um sich die Details zu einem Produkt anzeigen zu lassen.
    ⇨ "Artikel-Informationen" auf Seite C-1887
*   **Duplikate anzeigen:** Öffnet die Übersicht mit den identischen Dokumenten.
    ⇨ "Duplikate" auf Seite C-1847

##### Gruppe Kapazitäten
*   **Lieferterminkontrolle:** Öffnet die Übersicht über die (überfälligen) Aufträge und Bestellungen, um ggf. den Liefertermin zu ändern und den Kunden über die Änderung zu informieren.
    ⇨ “Kundenbenachrichtigung (Lieferterminkontrolle)" auf Seite C-1848
*   **Kapazitätsinfo nach Kunde:** Öffnet die Übersicht über die freien und reservierten Kapazitäten zum aktuellen Kunden.
    ⇨ "Kapazitätsinfo nach Kunde" auf Seite C-1854

##### Gruppe Finanzen
*   **OP Abfrage:** Öffnet eine Übersicht über die offenen Posten des Kunden.
    ⇨ "OP Abfrage" auf Seite C-1856
*   **Summen zwangsweise errechnen:** Die Beträge im aktuellen Auftrag werden neu berechnen, z. B. nach einer Preisänderung.
*   **Dokument überrechnen:** Mit dieser Funktion wird das Dokument sofort überrechnet, wenn Sie Preise, Rabatte oder Zuschläge geändert haben. Die Markierung wird während der aktuellen Sitzung beibehalten.
    Ein Dokument kann nicht überrechnet werden, wenn bereits eine Rechnung erstellt wurde. Diese Einstellung kann in den Mitarbeiterrechten geändert werden.

##### Gruppe Kalkulation
*   **Kalkulatorische Frachtkosten:** Öffnet den Dialog Kalkulatorische Frachtkosten, in dem Sie die Frachtkosten zum aktuellen Auftrag erfassen oder prüfen können. Die Funktion ist nur freigeschaltet, wenn in der Tour eine Kilometerpauschale und in den Kundenstammdaten die Entfernung eingetragen sind.
    ⇨ "Kalkulatorische Frachtkosten" auf Seite C-1858
*   **Kosten- und Aufschlagskalkulation:** Öffnet die Anzeige der Kosten- und Aufschlagskalkulation zum aktuellen Auftrag.
    ⇨ "Kosten- und Aufschlagskalkulation" auf Seite C-1859

##### Gruppe Optimierung
Diese Gruppe ist nur freigeschaltet, wenn als Dokumentenart Angebot gewählt ist und Sie mit A+W Business Pro arbeiten.
*   **Angebotsoptimierung:** Mit dieser Funktion wird das Angebot zur Optimierung gegeben. Sie können verschiedene Optimierungsparameter einstellen und die Ergebnisse speichern und als PDF-Datei an das Angebot anhängen. Im Auftrag haben Sie im Register Anlagen Zugriff auf diese Dokumente.
*   **Verschnittwerte:** Öffnet den Dialog Verschnittwerte, in dem die Quoten von allen durchgeführten Optimierungen angezeigt werden. Wenn Sie eine alternative Verschnittquote auswählen, werden die Änderungen am Preis angezeigt.

##### Gruppe Position
Diese Gruppe ist nur im Register Positionen freigeschaltet.
⇨ "Gruppe Position" auf Seite C-1684

##### Gruppe Einkauf
Diese Gruppe ist nur im Register Positionen freigeschaltet.
⇨ "Gruppe Einkauf' auf Seite C-1684

#### Menü Optionen
`Dokumente > Auftrag > Auftrag auswählen > Register Kopfdaten > Menü Optionen`

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

> **i Aktivierte Optionen nach dem Öffnen des Dialogs**
> Bitte beachten Sie, dass geänderte Optionen erst beim nächsten Öffnen des Dialogs wirksam werden.
> Wenn durch eine aktivierte Option eine Prüfung gestartet wurde, kann sich das Öffnen eines Dokuments verzögern. Der Grad der Verzögerung hängt von der Leistungsfähigkeit des Rechners ab.
> Die folgenden Beschreibungen stellen die aktivierte Option dar.

##### Gruppe Dokumente
Folgende Einträge werden angezeigt:
*   **Termine übernehmen:** Der Termin in jedem neuen Dokument wird aus dem zuvor erfassten Dokument übernommen.
*   **Wunschtermin übernehmen:** Der Wert aus dem Feld Wunsch (Termin) wird in jedem neuen Dokument aus dem zuvor erfassten Dokument übernommen.
*   **Versandtag nach Touren suchen:** Als Liefertermin wird der nächstmögliche Tourentag vorgeschlagen. Sie können den Liefertermin davon unabhängig auf den gewünschten Tag legen. Wenn die Tour geändert wird, werden alle abhängigen Termine neu berechnet.
*   **Versandtag-/Tourenprüfung:** Beim Speichern des Dokuments prüft das Programm, ob ein manuell eingesetzter Liefertermin einem Tourentag entspricht. Eine entsprechende Meldung weist darauf hin, wenn dies nicht der Fall ist. Diese Option sollten Sie aktivieren, wenn Sie Termine automatisch aus dem vorigen Dokument übernehmen.
*   **Kunde übernehmen:** Der Kunde in jedem neuen Dokument wird aus dem zuvor erfassten Dokument übernommen.
*   **Teillieferung melden:** Beim Öffnen eines Dokuments wird angezeigt, dass Teillieferungen zum gewählten Auftrag vorhanden sind.
*   **Duplikate melden:** Beim Öffnen eines Dokuments wird angezeigt, dass Duplikate zum gewählten Auftrag vorhanden sind.
*   **Neuerfassung als Standard:** Beim Öffnen des Dialogs Dokumentenverwaltung wird automatisch der Modus zum Erfassen aktiviert. Wenn die Option deaktiviert ist, liest das Programm das letzte Dokument des Nummernverwalters ein, auf den die Dokumentenverwaltung aktuell zugreift. Sie können den Nummernverwalter über die Funktion NV-Auswahl wechseln.
*   **AV-Bereich erstes Feld:** Beim Öffnen des Dokuments steht der Cursor automatisch im Feld AV-Bereich (nur, wenn AV-Bereiche definiert sind).
*   **AV-Bereichsänderung beibehalten:** Die Änderung des AV-Bereichs wird in jedes neue Dokument aus dem zuvor erfassten Dokument übernommen.
*   **Geschäftsartänderung beibehalten:** Die Änderung der Geschäftsart wird in jedes neue Dokument aus dem zuvor erfassten Dokument übernommen.
*   **Nettopreiserfassung:** In allen Aufträgen wird im Register Dokument die Checkbox Nettopreise aktiviert. Die Einstellung aus der Partnerverwaltung wird dabei ggf. übersteuert. Auf den Formularen werden keine Rabatte ausgewiesen.
*   **Fachberater=Erfasser:** Im Register Dokument wird im Feld Fachberater automatisch der Name des Mitarbeiters eingetragen, der in A+W Business angemeldet ist.
*   **Bestelltext 1, 2 prüfen:** Aufträge können nach den Bestelltexten 1 oder 2 zu Sammelrechnungen zusammengefasst werden.
*   **Sprung von Anliefertermin auf Bestelltext:** Wenn der Anliefertermin erfasst wurde, springt der Cursor mit der Tab-Taste automatisch ins Feld Bestelltext.
*   **Vertretersuche nach Vorwahl bei div. Kunden:** Wenn bei Kunden das Kennzeichen Div. Kunden gesetzt ist, wird der zuständige Vertreter im gleichen Bereich der Vorwahlnummer gesucht.
*   **Provinz nach Fremdschlüssel sortieren:** Wenn Fremdschlüssel eingetragen sind, wird die Provinz nach diesen sortiert.
*   **Nachfrage bei Änderung der Textnummer:** Wenn Texte aus den Stammdaten des Kunden übernommen werden, wird eine Meldung angezeigt, sobald im Dokument die Textnummer überschrieben wird.

##### Gruppe Positionen
Diese Gruppe wird in der Positionserfassung beschrieben.
⇨ "Gruppe Positionen" auf Seite C-1717

##### Gruppe Bearbeitungen/Modelle
Diese Gruppe ist nur im Register Positionen freigeschaltet.
⇨ "Gruppe Bearbeitungen/Modelle" auf Seite C-1720

##### Gruppe Sprossen
Diese Gruppe ist nur im Register Positionen freigeschaltet.
⇨ "Gruppe Sprossen" auf Seite C-1721

#### Menü Aufbau
`Dokumente > Auftrag > Auftrag auswählen > Register Positionen > Menü Aufbau`
Dieses Menü ist nur im Register Positionen freigeschaltet.
⇨ "Menü Aufbau" auf Seite C-1722

#### Menü Customizing
`Dokumente > Auftrag > Auftrag auswählen > Menü Customizing`
Diese Funktionen werden für Anpassungen in den Dialogen verwendet.
Dieses Menü ist nur freigeschaltet, wenn in den Firmendaten Customizing aktiv aktiviert ist.

### Dokument – Kopfdaten
`Dokumente > Auftrag > Auftrag auswählen > Register Kopfdaten`

> **Zu Dialogbeschreibung:**
> ⇨ Teillieferungsübersicht
> ⇨ Anzahlungsübersicht

Alle Dokumente für den Verkauf werden über den Dialog Dokumentenverwaltung erstellt und bearbeitet. Die Felder werden mit den Daten aus den Stammdaten des gewählten Marktpartners vorbelegt und können pro Dokument überschrieben werden.
⇨ Stammdaten, "Partnerverwaltung" auf Seite B-884

Im Register Kopfdaten werden die Kopfdaten der Dokumente erfasst. Über das Register Positionen wird die Positionserfassung geöffnet. Dieses Register wird erst aktiv, wenn die erfassten Kopfdaten gespeichert werden.
⇨ Tutorial, "Dokumente und Folgedokumente" auf Seite C-1281
⇨ Tutorial, "Auftragskopf erfassen" auf Seite C-1304

> **i Voraussetzung**
> Dokumente können nur zu Kunden und Lieferanten erstellt werden, deren Daten in den Stammdaten hinterlegt sind. Dazu gehören auch die Marktpartner, die als so genannte diverse Kunden gekennzeichnet sind.

> **i Dokument durch Kopieren erstellen**
> Dokumente können erstellt werden, indem ein vorhandenes Dokument kopiert und bearbeitet wird. Dabei kann auch der Dokumententyp gewechselt werden, z. B. von Angebot zu Auftrag.
> ⇨ "Dokumente kopieren" auf Seite C-1813

> **i Ergänzende Informationen**
> ⇨ Überblick, "Standard-Menüs" auf Seite A-66
> ⇨ "Dokument - Positionen" auf Seite C-1724
> ⇨ "Dokument - Summen" auf Seite C-1797
> ⇨ "Übersichten und Referenzen zu Kopfdaten" auf Seite C-1802
> ⇨ "Übersichten und Referenzen zu Positionen" auf Seite C-1866
>
> In diesem Dialog finden Sie folgende Register:
> *   "Kopfdaten - Dokument" auf Seite C-1688
> *   "Kopfdaten - Abweichende Anschriften" auf Seite C-1694
> *   "Kopfdaten - Zusatz" auf Seite C-1696
> *   "Kopfdaten - Konditionen" auf Seite C-1700
> *   "Kopfdaten - Texte" auf Seite C-1704
> *   "Kopfdaten - Anlagen" auf Seite C-1706
> *   "Kopfdaten - Technische Parameter" auf Seite C-1707
> *   "Kopfdaten - Kundeninfo" auf Seite C-1709

#### Kopfdaten – Dokument
`Dokumente > Auftrag > Auftrag auswählen > Register Kopfdaten > Register Dokument`

[Image: Abb. C-237 Kopfdaten - Dokument, showing the main 'Document' tab for header data.]

In diesem Register legen Sie den Kunden fest und bestimmen die Termine und die Lieferbedingungen.
⇨ Tutorial, "Auftragskopf erfassen" auf Seite C-1304

> **i Voraussetzung**
> Dokumente können nur zu Kunden und Lieferanten erstellt werden, deren Daten in den Stammdaten hinterlegt sind. Dazu gehören auch die Marktpartner, die als so genannte diverse Kunden (ohne eigenes Konto) gekennzeichnet sind. Diese Einstellung wird aus den Stammdaten des Kunden ausgelesen.

##### Identifikation
**Mandant** Nummer des Mandanten, zu dessen Kundenstamm der Kunde gehört. Sie können nur Mandaten auswählen, zu denen die Nummernkreise eingerichtet sind.
⇨ Stammdaten, "Nummernkreise" auf Seite B-1028
⇨ Stammdaten, "Firmendaten - Mandant" auf Seite B-1056

**Nummer** Nummer des aktuellen Dokuments.

**Bereich** AV-Bereich, zu dem der Auftrag erfasst wird.
⇨ Stammdaten, "AV-Bereiche" auf Seite B-1160

**Gesch.Art** Geschäftsart, zu der der Auftrag erfasst wird. Zur Auswahl werden die Geschäftsarten angeboten, die Sie in den Stammdaten hinterlegt haben.
⇨ Stammdaten, "Geschäftsart" auf Seite B-1024

##### Anschrift
Die Angaben zum Kunden werden aus den Kundendaten übernommen. Sie können für diesen Auftrag überschrieben werden.
⇨ Stammdaten, “Partnerverwaltung - Adresse" auf Seite B-888

**Nummer** Nummer des Kunden.

**Fax, Mail** Auftragsbestätigungen (AB), Angebote (An), Rechnungen (Re) und Gutschriften (Gu) können per Fax oder E-Mail gesendet werden. Dazu muss in den Kundendaten die Fax-Nummer bzw. die E-Mail-Adresse hinterlegt sein. Die Optionen können pro Auftrag aktiviert oder deaktiviert werden.

> **i Fehlende Daten ergänzen**
> Sie können die Angaben zu Kunden ergänzen oder ändern. Diese neuen Daten werden jedoch nicht in die Kundenstammdaten zurückgeschrieben.

**Adressdaten** Die Daten in den Feldern Kopf bis Mail werden aus den Kundenstammdaten übernommen. Sie können diese Daten für den aktuellen Auftrag ändern. Die Änderungen werden nicht in die Stammdaten zurückgeschrieben.

**Liefer., Rech.** Anzeige der Rechnungs- oder Lieferanschrift, die im Register Abw. Anschriften angegeben wurde. Die Optionen sind nur freigeschaltet, wenn eine Rechnung und/oder eine Lieferanschrift angegeben ist.
⇨ "Kopfdaten - Abweichende Anschriften" auf Seite C-1694

##### Mitarbeiter
**Fachberater** Dieses Feld wird abhängig von der Einstellung im Menü Option > Fachberater=Erfasser gefüllt.
*   Wenn diese Option aktiviert ist, trägt das System automatisch den Login-Namen des Erfassers ein.
*   Wenn die Option deaktiviert ist, wird der zutreffende Fachberater aus den Stammdaten des Kunden angezeigt. Der Eintrag kann überschrieben werden.

**Vertreter** Name des zuständigen Vertreters, für den die Provision abgerechnet werden kann.

##### Termine
Im Menü Optionen können folgende Vorgaben aktiviert werden: Termine übernehmen, Wunschtermin übernehmen, Versandtag nach Touren suchen und Versandtag-/Tourenprüfung.
⇨ "Menü Optionen" auf Seite C-1684

Wenn dem Kunden eine Tour zugeordnet ist, werden die Tourentage im Kalender grün hinterlegt. Der Berechnung der Termine liegen die Angaben aus den Firmenstammdaten zugrunde.
⇨ Tutorial, "Lieferdauer" auf Seite C-1300
⇨ Stammdaten, "Vorlauftage" auf Seite B-1115

**Wunsch** Der vom Kunden gewünschte Liefertermin. Das kann auch ein alphanumerischer Eintrag sein, z. B. 08.04. vor 12 h.

**Anlieferung** Tag der gewünschten Anlieferung beim Kunden. Nach der Eingabe des Termins werden die Termine in den weiteren Feldern berechnet. Dieses Feld wird nicht bei Dokumentenart Gutschrift angezeigt.
Wenn der Liefertermin geändert wird, kann eine Angabe von Gründen zwingend erforderlich sein. Dazu können Gründe voreingestellt und zur Auswahl angeboten werden.
⇨ Stammdaten, "Firmendaten - Dokumente" auf Seite B-1066

**[Lieferterminbestimmung]** Dieses Feld wird nur bei Dokumentenart Angebot und Auftrag angezeigt.
Das Dokument wird an die Kapazitätsplanung übergeben und der frühestmögliche Liefertermin wird errechnet.
In A+W Business Pro wird nicht nur der Liefertermin angefragt und zurückgeschrieben, sondern auch der Auftrag in den Produktionsmanager eingelastet.
⇨ "Lieferterminbestimmung" auf Seite C-1862

**Anlieferzeit** Anlieferzeit beim Kunden, z.B. 08:00 - 11:00 Uhr. Dieses Feld wird nicht bei Dokumentenart Gutschrift und Anfrage angezeigt.

**Versandtag** Tag, an dem die Tour startet. Der Versandtag wird automatisch errechnet, wenn in den Stammdaten die entsprechenden Fristen hinterlegt sind.

**[Liefertermin ändern]** Öffnet den Dialog Liefertermin ändern, in dem Sie den Lieferanten oder den Liefertermin für den gesamten Auftrag ändern können. Dieses Feld wird nur bei Dokumentenart Auftrag angezeigt.
⇨ "Liefertermin ändern" auf Seite C-1863

**Bestellung** Tag, an dem der Kunde die Bestellung übermittelt hat. Standardmäßig ist das aktuelle Datum (Systemdatum) vorbelegt. Wenn der Auftrag aus einem früheren Auftrag erzeugt wird, wird dessen Datum angezeigt.

**Erfassung** Tag, an dem das Dokument erfasst wurde. Dieses Datum wird automatisch eingetragen und kann nicht geändert werden.

**Vorlage** Tag, an dem das Dokument zur Wiedervorlage angeboten werden soll. Dazu müssen in den Firmendaten die Vorlauftage eingetragen sein.
⇨ Stammdaten, "Firmendaten - System" auf Seite B-1113
Beim Start von A+W Business prüft das System, ob Dokumente zur Wiedervorlage existieren. Über eine Abfrage können die Dokumente zur Wiedervorlage angezeigt werden.
⇨ "Wiedervorlage" auf Seite C-1663

**Prod. Start** Tag, an dem die Produktion (spätestens) starten muss. Die Frist wird automatisch nach dem Termin im Feld Anlieferung errechnet.

**Anlief. Lief.** Tag, an dem die Lieferung von Bestellungen (spätestens) eintreffen muss. Die Frist wird automatisch nach dem Termin im Feld Anlieferung errechnet. Dazu muss die entsprechende Meldung mit [Ja] bestätigt werden. Dieses Feld wird nur angezeigt, wenn Sie in den Firmendaten die Option Handel gewählt haben.
⇨ Stammdaten, "Kundenversion" auf Seite B-1114

**VSG** Tag, an dem die Produktion des VSG (spätestens) starten muss. Die Fristen werden automatisch nach dem Termin im Feld Anlieferung errechnet. Dieses Feld wird nur angezeigt, wenn Sie in den Firmendaten die Option Produzent gewählt haben.
⇨ Stammdaten, "Kundenversion" auf Seite B-1114

**Prod. Ende** Die Fristen werden automatisch nach dem Termin im Feld Anlieferung errechnet.

**Priorität** Priorität, mit der der Auftrag ausgeführt werden soll. Die Angabe wird in die Kapazitätsplanung und in die Produktion übergeben.
*   **Abruf:** Der Auftrag wird erst abgewickelt, wenn der Kunde die Ware abruft.
*   **Eilt:** Der Auftrag wird mit hoher Priorität abgewickelt.
*   **Normal:** Der Auftrag wird ohne besondere Kennzeichnung abgewickelt.
*   **Zugabe:** Der Auftrag wird als sogenannter Füllauftrag an die Produktion übergeben. Er wird dann bei geeigneten Restblättern verarbeitet.

**Vorlage** Datum, mit dem das Angebot auf Wiedervorlage gesetzt wird. Dieses Feld wird nur bei Dokumentenart Angebot angezeigt.
⇨ "Angebot (Dokument)" auf Seite C-1661

##### Bestellung, Lieferung, Zahlung, Dokument
**Bestelltexte** Eingabefelder für ergänzende Angaben zur Bestellung, z. B. ein Bezug auf eine Bestellung per Fax. Die Felder können auch als Sortierkriterien herangezogen werden, z. B., wenn interne Nummern eingetragen sind.

**Tour** Die Tour wird aus den Kundendaten übernommen. Sie kann für diesen Auftrag geändert werden.

**Lieferbed.** Die Lieferbedingungen werden aus den Kundendaten übernommen. Sie können für diesen Auftrag geändert werden.

**Zahl.-bed.** Die Zahlungsbedingungen werden aus den Kundendaten übernommen. Sie können für diesen Auftrag geändert werden.

**Typ** Je nachdem, was für ein Dokument Sie erstellen, wird der Dokumententyp automatisch zugeordnet, z. B. bei Anzahlungen, Reklamationen. Für Aufträge steht immer `<k.A.>`. Dieses Feld kann zur Einschränkung der Suche nach bestimmten Dokumenten genutzt werden. Die Dokumententypen sind in den Stammdaten hinterlegt:
⇨ Stammdaten, "Dokumententyp" auf Seite B-1036

> **i Änderung des Dokumententyps kann zu Problemen führen**
> Bei normalen Aufträgen steht der Typ standardmäßig auf `<k.A.>`. In der Regel muss er manuell nicht geändert werden. Wählen Sie einen anderen Dokumententyp nur nach Rücksprache mit der A+W Software GmbH aus. Eine willkürliche Änderung kann zu ungewollten Ergebnissen führen.

**Preisdruck** Die Darstellung der Preise im Druck wird nur übernommen, wenn in der Formularverwaltung die Option 0 - Standard oder 2 - Preise immer drucken (Summenmodus) gewählt wurde. Diese Einstellung muss für das entsprechende Formular (Druckpunkt) gelten.
*   **0 - Kein Druck:** Die Preise werden nicht gedruckt.
*   **1 - Alle Preise:** Die Preise werden pro Auftragsposition gedruckt.
*   **2 - Nur Summen:** Nur die Summen von Gesamtwert, Gesamtstückzahlen usw. werden gedruckt. Diese Option steht nicht zur Verfügung, wenn in der Formularverwaltung der Modus 1 - Preise immer drucken gewählt wurde.
    ⇨ Tutorial, "Darstellung der Preise im Druck" auf Seite C-1460

**Nettopreise** Die Einstellung der Checkbox Nettopreise wird standardmäßig auch aus der Partnerverwaltung übernommen. Sie kann mit der Option Nettopreiserfassung im Menü Optionen übersteuert werden.
- Die Preise werden als Bruttopreise gedruckt.
- Die Preise werden als Nettopreise gedruckt.
⇨ "Menü Optionen" auf Seite C-1684

**Abrechnung** Nummer der Abrechnung (Forderungsrechnung), die für einen Rahmenauftrag erstellt wurde. Dieses Feld wird nur bei Dokumentenart Auftrag, Gutschrift, Bestellung angezeigt.
⇨ "Forderungen" auf Seite C-1708

**Transportunternehmen** Nummer des Spediteurs, der die Lieferung übernimmt. Dieses Feld wird nur bei Dokumentenart Angebot, Anfrage angezeigt.

**Frachtverantwortung** Auswahl der Frachtverantwortung in der brasilianischen Steuer. Die Auswahlmöglichkeiten in der Kombobox sind vordefiniert. Sie können zwischen Drittunternehmen, Kunde, nicht definiert und Selbst wählen. Das Feld wird nur angezeigt, wenn Sie in den Firmendaten die brasilianische Steuer aktiviert haben.

**CRM Referenz/Projekt** Hier können Sie eine Referenz- oder Projektnummer für dieses Dokument vergeben. Nach dieser Nummer kann dann sowohl in der Dokumentenerfassung als auch in der Dokumentensuche gesucht werden. Die Nummer wird auch in der Bildschirmtabelle des Nummernverwalter angezeigt. Beim Kopieren von Dokumenten und bei der Bestellübergabe wird die CRM Projektnummer in die Ziel-Dokumente übertragen. Beim Formulardruck mit Crystal Reports ist es ebenfalls möglich, die CRM Referenz-/Projektnummer via Parameter-Ersetzung (<<PROJ>>) in den PDF-Dateinamen zu schreiben. Das Feld wird nur angezeigt, wenn Sie in den Firmendaten das entsprechende Feld aktiviert haben.
⇨ Stammdaten: Softwarereferenz, "CRM Dokumentenreferenz" auf Seite B-1084

#### Kopfdaten – Abweichende Anschriften
`Dokumente > Auftrag > Auftrag auswählen > Register Kopfdaten > Register Abweichende Anschriften`

[Image: Abb. C-238 Kopfdaten - Abweichende Anschriften, showing the tab for alternative delivery and invoice addresses.]

In diesem Register können Sie eine Liefer- und/oder Rechnungsanschrift eintragen, die von der Anschrift aus den Kundendaten abweicht.
⇨ Stammdaten, "Filialen des Kunden" auf Seite B-121

##### Lieferanschrift, Rechnungsanschrift
Wenn in den Kundenstammdaten eine Liefer- und/oder Rechnungsanschrift hinterlegt ist, werden diese Daten übernommen.

**Direktanlieferung durch den Lieferanten** Wenn zum Auftrag Bestellungen gehören, können die bestellten Produkte vom Lieferanten direkt an den Kunden ausgeliefert werden.
- Die bestellten Produkte werden nicht direkt an den Kunden geliefert.
- Die Lieferanschrift wird automatisch mit der Bestellung an den Lieferanten gesendet. Die bestellten Produkte werden direkt an den Kunden geliefert.

Die eingetragene Anschrift wird im Register Dokument angezeigt.
Wenn eine Liefer- und eine Rechnungsanschrift eingetragen sind, werden im Register Dokument die Optionen Liefer. und Rech. zur Auswahl freigeschaltet.
⇨ "Liefer., Rech." auf Seite C-1689

Über die Suche [Lupe] kann die Anschrift eines anderen Marktpartners ausgewählt werden.

**Entfernung** Angabe der Entfernung zur Lieferanschrift. Der Wert wird aus den Kundenstammdaten übernommen. Er kann bei einer Änderung der Lieferanschrift angepasst werden und gilt nur für den aktuellen Auftrag. Der Wert wird für die Berechnung von Frachtkosten und Zuschlägen herangezogen, z. B. Mautzuschlag.

##### Filialen
Wenn in den Kundenstammdaten Filialen angelegt sind, werden deren Anschriften aufgelistet.
⇨ Stammdaten, "Filialen des Kunden" auf Seite B-121
⇨ Stammdaten, “Partnerverwaltung - Mitarbeiter/Filiale/Vorgänge" auf Seite B-899

Die markierte Anschrift wird mit den Pfeilschaltflächen übernommen. Die Daten können in den Bereichen Lieferanschrift und Rechnungsanschrift angepasst werden.

#### Kopfdaten – Zusatz
`Dokumente > Auftrag > Auftrag auswählen > Register Kopfdaten > Register Zusatz`

[Image: Abb. C-239 Kopfdaten - Zusatz, showing the 'Additional Info' tab.]

In diesem Register legen Sie Details zur Fakturierung und Zusatzinformationen für den Versand fest.
Die Felder in den Bereichen Identifikation und Anschrift sind ausführlich im Kapitel zum Register Dokumente beschrieben.
⇨ "Kopfdaten - Dokument" auf Seite C-1688

##### Faktura
**Ums.steuer-ID** Die Identifikationsnummer für die Umsatzsteuer-Vorauszahlungen des Kunden kann auf die Rechnung gedruckt werden.
**Steuernummer** Die Steuernummer des Kunden kann auf die Rechnung gedruckt werden.
**Re.Nr., Datum** Die Rechnungsnummer und das Datum werden automatisch beim Rechnungsdruck eingesetzt. Sie können nicht manuell vergeben werden. In allen Dokumenten vor dem Rechnungsdruck bleiben die Felder leer.

**Fälligkeitsdatum** Das Datum für die Fälligkeit wird automatisch aus den Zahlungsbedingungen ermittelt. Sie können das errechnete Datum überschreiben. Im Register Konditionen können Sie weitere Angaben zur Zahlung machen.
⇨ Stammdaten, "Partnerverwaltung - Finanzen" auf Seite B-904
⇨ Tutorial, "Fälligkeiten" auf Seite C-1469
⇨ "Bestellung, Lieferung, Zahlung, Dokument" auf Seite C-1692
⇨ "Kopfdaten - Konditionen" auf Seite C-1700

**Rechnung storniert** Über diese Checkboxen werden ein Auftrag und die Lagerabbuchungen storniert.
- Auftrag und Rechnung sind nicht storniert.
- Der Auftrag wurde storniert. Wenn das aktuelle Dokument Teil einer Sammelrechnung ist, werden alle Rechnungen dieser Sammelrechnung storniert. Alle zugehörigen Lagerbuchungen werden ebenfalls storniert.

**Teillieferung, Teilfaktura, Sammelrechnung** Über diese Checkboxen wird gesteuert, ob Teillieferungen mit und ohne Teilfaktura möglich sind oder ob dieser Auftrag in einer Sammelrechnung abgerechnet werden soll. Die Felder sind gesperrt, wenn die Funktionen in den Kundendaten nicht aktiviert sind.
- Der Auftrag wird ohne Teillieferung/Teilfaktura/Sammelrechnung abgewickelt.
- Die Positionen des Auftrags können sowohl teilgeliefert, teilfakturiert und/oder in einer Sammelrechnung berechnet werden.
⇨ Tutorial, "Rechnungen" auf Seite C-1467

##### Sprach-, Maßsystem
**Sprache** Die Texte werden im Formular in der ausgewählten Sprache gedruckt. Wenn die Texte nicht in der gewählten Sprache hinterlegt sind, bleiben die zugehörigen Felder leer.
⇨ Stammdaten, "Sprachen" auf Seite B-668
⇨ Stammdaten, "Preis-/Mengeneinheit für Mehrsprachigkeit" auf Seite B-669

**Maßsystem metrisch (mm), imperial (inch)** Mit der Auswahl einer der Optionen bestimmen Sie, wie die Maße in diesem Auftrag angegeben werden. Die Voreinstellung wird aus den Stammdaten übernommen.
⇨ Stammdaten, "Partnerverwaltung - Auftrag" auf Seite B-892
⇨ Stammdaten, "Firmendaten - System" auf Seite B-1113

##### Zusatz-Informationen
**Sperrkennz.** Mit dem Sperrkennzeichen können Sie das Dokument für die gewählte Transaktion sperren, z. B., wenn für die Produktionsübergabe noch Angaben geklärt werden müssen. Das Sperrkennzeichen wird vor der jeweiligen Übergabe abgefragt. Zur Wahl stehen die Sperrkennzeichen, die in den Stammdaten definiert sind.
⇨ Stammdaten, "Sperrkennzeichen" auf Seite B-1034

**Verpackung** Für den Versand können Sie eine der hinterlegten Verpackungsarten auswählen.

**Ausweichtour** Standardmäßig wird der Auftrag mit der Tour ausgeliefert, die in den Kundendaten hinterlegt ist oder die Sie im Register Dokument ausgewählt haben. Eine Ausweichtour kann festgelegt werden, um für diesen Auftrag eine Alternative zur Standardtour zu ermöglichen. Sie wird nur zur Information angezeigt.

**Zolltour** Mit den Angaben zur Zolltour wird festgelegt, welche zusätzlichen Papiere ausgestellt werden müssen. Sie wird nur zur Information angezeigt.

**LKW** Mit der Auswahl des Lkws planen Sie den Einsatz Ihrer Fahrzeuge. Die Daten können statistisch ausgewertet werden.

**Fahrer** Mit der Auswahl des Fahrers planen Sie den Einsatz Ihrer Fahrer. Die Daten können über statistisch ausgewertet werden.

**Gruppe** Die Kundengruppe wird aus den Stammdaten übernommen. Über die Kundengruppe können Preise und Rabatte vergeben werden. Wenn Sie diesen Auftrag einer (anderen) Kundengruppe zuordnen, werden die Preise und Rabatte aus dieser Gruppe zur Berechnung herangezogen.
⇨ Stammdaten, "Kundengruppen" auf Seite B-874

**Vertreter 2** Mit der Auswahl des zweiten Vertreters beteiligen Sie neben dem standardmäßig zuständigen Vertreter einen weiteren Mitarbeiter an diesem Auftrag.

**% Anteil am Umsatz d. Vertreter 2** Mit dieser Angabe bestimmen Sie, wie hoch die Provision des zweiten Vertreters sein soll. Zur Berechnung werden der Gesamtumsatz des Auftrags und der Umsatzanteil des Vertreters 1 herangezogen.
⇨ Stammdaten, "Vertreterprovision" auf Seite B-1163

**Kategorie** Durch die Kategorie kann ein Angebot nach verschiedenen Ablehnungsgründen klassifiziert werden, z. B. zu teuer, keine Rückmeldung. Über die Kategorie können Angebote in der Statistik ausgewertet werden.

**Fremdschlüssel** Über den Fremdschlüssel können Sie das Dokument an ein anderes System übergeben, z. B. zu externen Auswertungen.

**Textfeld 1, 2, 3** Frei verwendbare Textfelder. Die Bezeichnung der Felder kann mit den Systemtexten 2000-2002 angepasst werden. Die Felder können auf der Dokumentenansicht und auf den Formularen ausgegeben werden.
⇨ Stammdaten, "Systemtexte" auf Seite B-1191

> **i Textfeld 1 - Projekt-/auftragsbezogene Steuerbefreiung**
> Um eine Projekt-/auftragsbezogene Steuerbefreiung zu erreichen, wird das Textfeld 1 aus der Dokumentenerfassung an den Avalara Web-Service übergeben. Das Feld ist in der Avalara Schnittstelle als purchaseOrderNo enthalten. Darüber wird in der Konfiguration innerhalb des Avalara Accounts die Steuerbefreiung erreicht.

#### Kopfdaten – Konditionen
`Dokumente > Auftrag > Auftrag auswählen > Register Kopfdaten > Register Konditionen`

[Image: Abb. C-240 Kopfdaten - Konditionen, showing the 'Conditions' tab.]

In diesem Register legen Sie Zuschläge, Kunden-, Lieferantenobjekte und Wechselkurs fest.
Die Felder in den Bereichen Identifikation und Anschrift sind ausführlich im Kapitel zum Register Dokumente beschrieben.
⇨ "Kopfdaten - Dokument" auf Seite C-1688

##### Sonstige
**Zahl.-weg** Der Zahlungsweg wird aus den Kundendaten übernommen. Er kann für diesen Auftrag geändert werden. Mit der Auswahl legen Sie fest, wie die Rechnung durch den Kunden beglichen wird. Die Auswahlliste zeigt alle Zahlungswege, die in den Stammdaten hinterlegt sind.
⇨ Stammdaten, "Zahlungswege" auf Seite B-1052
