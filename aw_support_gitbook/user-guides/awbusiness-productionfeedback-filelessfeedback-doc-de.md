---
description: "D-AWBusiness-HB_24"
---


---
## Rückmeldungen aus der Produktion

### Erfassungsstellen für dateilose Rückmeldungen prüfen

> **Umstellung auf dateilose Rückmeldung**
> Wenn Sie A+W Business auf die dateilosen Rückmeldungen umstellen wollen, müssen folgende Einstellungen in A+W Production geprüft werden:
> - Einstellung in der CommonBase in A+W Production
> - Installation des PPS-Webservices
>
> Lassen Sie sich bei der Umstellung von Ihrem Service-Mitarbeiter bei der A+W Software GmbH unterstützen.

**So prüfen Sie eine Erfassungsstelle für die dateilose Rückmeldung**

In dieser Handlungssequenz werden nur die Einstellungen für die dateilosen Rückmeldungen beschrieben. Wie Sie neue Erfassungsstellen einrichten, ist in der Einheit für Produktionsrückmeldungen per Datei beschrieben.

⇨ "So ordnen Sie eine Erfassungsstelle für die Rückmeldung per Datei zu" auf Seite E-63

1.  Wählen Sie im Menü **Stammdaten > Fertigung > Erfassungsstellen Produktion**.
    
    *[Image of the 'Erfassungsstellen Produktion' dialog. Label A points to 'Typ der Rückmeldung' (Type of feedback). Label B points to a specific 'Erfassungsstelle' (data entry point) in the list to be checked.]*

2.  Markieren Sie in der Übersicht die Erfassungsstelle (B), die Sie prüfen wollen.
3.  Wählen Sie im Feld **Typ (A)** den Eintrag **1 - Sonstige** aus.
    Der Eintrag ist in einer Auswahlliste hinterlegt, die Sie mit einem Klick in die jeweilige Zelle öffnen können.
4.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.
5.  Ordnen Sie alle erforderlichen Erfassungsstellen zu.
    Prüfen Sie nun die Einstellung für dateilose Rückmeldungen in den Firmendaten.
    ⇨ "Einstellungen in den Firmendaten festlegen" auf Seite E-69

### Einstellungen in den Firmendaten festlegen

In den Firmendaten müssen Sie die Einstellungen für die dateilose Produktionsrückmeldung prüfen.

**So prüfen Sie die Einstellungen für dateilose Rückmeldungen**

1.  Wählen Sie im Menü **Stammdaten > Firma > Firmendaten** und wechseln Sie zum Register **Produktion**.
    
    *[Image of the company data settings under the 'Produktion' tab. Label A points to the 'Dateilose Produktionsrückmeldung' checkbox. Label B points to the 'PPS-Webservice-URL' input field.]*

2.  Markieren Sie die Checkbox **Dateilose Produktionsrückmeldung (A)**.
3.  Geben Sie im Feld **PPS-Webservice-URL (B)** die Web-Adresse ein.
    Mit einem Klick auf die Schaltfläche mit der Weltkugel können Sie prüfen, ob die Verbindung hergestellt werden kann.
4.  Wechseln Sie zum Register **Kapa-Planung**.
    
    *[Image of the company data settings under the 'Kapa-Planung' tab. Label A points to the version selection for capacity planning.]*

5.  Wenn Sie mit dem Programm A+W Production Capacity Planner arbeiten, prüfen Sie, ob dieses eingestellt ist (A).
    Zur Erinnerung: Dateilose Rückmeldungen können nicht in Verbindung mit der Kapazitätsplanung von A+W Business genutzt werden. Sie können jedoch genutzt werden, wenn keine Kapazitätsplanung genutzt wird.
6.  Legen Sie fest, an wen Fehlermeldungen gesendet werden sollen:
    *   **Auftragserfasser:**
        Die Fehlermeldungen werden automatisch an den Erfasser des Auftrags gemeldet.
    *   **Mitarbeiter:**
        Alle Fehlermeldungen sollen an einen bestimmten Mitarbeiter gemeldet werden.
        Wenn Sie diese Option gewählt haben, wird das Feld zur Auswahl des Mitarbeiters freigeschaltet.
7.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.

### Dateilose Rückmeldung und online-Produktionsübersicht

A+W Production ruft zum Einlagern der Produktionsrückmeldungen den ERP-Webservice auf. Der ERP-Webservice nimmt die Meldung entgegen und schreibt sie in die Datenbank. Diese eingelagerten Meldungen werden anschließend vom A+W Business Interface Service verbucht. Dabei wird der Status des Auftrags aktualisiert.

In A+W Business können Sie diese Produktionsfortschritte über dateilose Rückmeldung überwachen. Die abgerufenen Daten stellt A+W Business im Dialog **Übersicht Statusrückmeldung** dar.

*[Image of the 'Online-Produktionsübersicht' in A+W Business, showing order progress.]*

In der Spalte **Offene Bearbeitungen** wird die Anzahl aller Bearbeitungen einer Position angezeigt. Dabei zählen alle Arbeitsschritte vom Zuschnitt bis zur Verpackung jeweils als Bearbeitung.

Die Online-Abfrage ist zeit- und mengengenau, so dass Sie, im Gegensatz zu Rückmeldungen per Datei, immer den genauen Produktionsstand eines Auftrags sehen können.

**Beispiel: Auftrag**

*   **Position 1:** 15 x Float 5 mm
    *   Arbeitsschritte pro Scheibe = 3 (Zuschnitt, Verpackung, Lieferung)
    *   Gesamt (15x3) = 45
*   **Position 2:** 20 x ESG 6 mm
    *   Arbeitsschritte pro Scheibe = 5 (Zuschnitt, Säumen, Härten, Verpackung, Lieferung)
    *   Gesamt (20x5) = 100

Die dateilosen Produktionsrückmeldungen zeigen für diesen Auftrag im Verlauf der Produktion folgende Details an:

**Beispiel - Anzeige 1: Von Position 1 sind 10 Stück zugeschnitten**

| Pos | Menge | offene Arbeitsschritte | letzte Station | Status | nächste Station |
| :-- | :--- | :--- | :--- | :--- | :--- |
| 1 | 5 | 15 | | | Zuschnitt |
| 1 | 10 | 20 | Zuschnitt | Produktion | Verpackung |
| 2 | 20 | 100 | | | Zuschnitt |

Für Position 1 sind 5 x 3 (Zuschnitt, Verpackung, Versand) und 10 x 2 (Verpackung, Versand) Arbeitsschritte offen.
Für Position 2 sind alle 100 Arbeitsschritte offen.

**Beispiel - Anzeige 2: Von Position 1 sind die verbliebenen 5 Stück zugeschnitten**

| Pos | Menge | offene Arbeitsschritte | letzte Station | Status | nächste Station |
| :-- | :--- | :--- | :--- | :--- | :--- |
| 1 | 15 | 30 | Zuschnitt | Produktion | Verpackung |
| 2 | 20 | 100 | | | Zuschnitt |

Für Position 1 sind 15 x 2 (Verpackung, Versand) Arbeitsschritte offen.
Für Position 2 sind alle 100 Arbeitsschritte offen.

**Beispiel - Anzeige 3: Von Position 2 sind 10 Stück auf dem Weg zum Ofen und die restlichen 10 Stück zugeschnitten**

| Pos | Menge | offene Arbeitsschritte | letzte Station | Status | nächste Station |
| :-- | :--- | :--- | :--- | :--- | :--- |
| 1 | 15 | 30 | Zuschnitt | Produktion | Verpackung |
| 2 | 10 | 40 | Zuschnitt | Produktion | Schleifen |
| 2 | 10 | 30 | Schleifen | Produktion | Ofen 1 |

Für Position 2 sind 10 x 4 (Schleifen, Ofen, Verpackung, Versand) und 10 x 3 (Ofen, Verpackung, Versand) Arbeitsschritte offen.

Positionen, bei denen keine offenen Arbeitsschritte mehr vorhanden sind, werden aus der Anzeige gelöscht, so dass schließlich für den ausgewählten Auftrag keine Daten mehr angezeigt werden.

Die gemeldeten Mengen werden nicht gespeichert. Das bedeutet, dass immer nur der aktuelle Produktionsstand angezeigt wird.

### Übermengen

> Mit den dateilosen Rückmeldungen können Übermengen aus A+W Production akzeptiert werden. Das bedeutet, dass die Übermengen, die bei der Produktion eines Kundenauftrags entstanden sind, in den Auftrag übernommen und berechnet werden können. Dies betrifft Kundenaufträge, die regelmäßig wiederkehren und daher mögliche Übermengen von Kunden akzeptiert werden. Die zulässigen Übermengen müssen in den Stammdaten definiert werden.
> 
> *   ⇨ Stammdaten, “Produktverwaltung - Fertigung" auf Seite B-605
> *   ⇨ Stammdaten, "Übermengen" auf Seite B-859
> 
> **Übermengen nur mit dateiloser Rückmeldung**
> Übermengen können nicht akzeptiert werden, wenn Sie mit den Rückmeldedateien (STSP, STSL, STSD, STSB, STSG) arbeiten.

### Dateilose Rückmeldungen und Kapazitätsplanung

Für das Arbeiten mit dateilosen Produktionsrückmeldungen müssen Sie Folgendes beachten:

*   Dateilose Rückmeldungen können auch aus A+W Production Capacity Planner eingelesen werden. Wenn Sie mit der Kapazitätsplanung von A+W Business arbeiten, ist dies jedoch nicht möglich.
*   Die Erfassungsstellen müssen in A+W Business in Abstimmung mit A+W Production konfiguriert werden.

**Ergänzende Informationen**
*   ⇨ Stammdaten, "Erfassungsstellen Produktion" auf Seite B-882
*   ⇨ Stammdaten, "Firmendaten - Lager/EK/EDI" auf Seite B-970
*   ⇨ Stammdaten, "Firmendaten - Produktion" auf Seite B-1000
*   ⇨ Stammdaten, "Schnittstellen-Dienst" auf Seite B-1046
*   ⇨ Verkauf, "Übersicht Statusrückmeldung" auf Seite C-590

### A+W Business Interface Service

**Lernziele**
*   A+W Business Interface Service kennenlernen.
*   Einstellungen für den Service festlegen.

**Nutzen**
*   Über den A+W Business Interface Service werden alle Arten von Kommunikation mit anderen Programmen abgewickelt.

**Merke**
*   **A+W Business Interface Service**: Der A+W Business Interface Service ist ein Windows-Dienst.
*   **Voreinstellungen**:
    *   Stammdaten:
        *   Schnittstellen-Dienst
    *   Firmendaten:
        *   Register Produktion

### Einstellungen für den A+W Business Interface Service festlegen

In diesem Abschnitt lernen Sie, wie die Parameter für die Rückmeldedateien eingerichtet werden können.

**So legen Sie die Einstellungen für den A+W Business Interface Service fest**

1.  Wählen Sie im Menü **Stammdaten > Firma > Schnittstellen-Dienst** und wechseln Sie zum Register **Optionen**, um das Intervall zum Einlesen von Rückmeldungen anzugeben.
    
    *[Image of the 'Schnittstellen-Dienst' options dialog. Label A points to the interval setting for the A+W Business Interface Service.]*

2.  Legen Sie das Intervall (A) für den A+W Business Interface Service fest.
    Wenn Sie z. B. eine 2 eintragen, prüft der Service alle 2 Minuten, ob neue Rückmeldungen aus der Produktion vorliegen, und liest diese ein.
3.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.

**Ergänzende Informationen**
*   ⇨ Stammdaten, "Schnittstellen-Dienst" auf Seite B-1046

## Lieferwesen

In diesem Themenblock lernen Sie, wie Sie Lieferungen und Versand in A+W Business organisieren.
Dazu gehören folgende Lerneinheiten:
*   "Tourenplanung" auf Seite E-82
*   "Statusmeldung" auf Seite E-94
*   "Kommissionierung" auf Seite E-105

### Tourenplanung

**Lernziele**
*   Aufträge zu einer Tour zusammenstellen.
*   Liefertermin oder Tour ändern.
*   Kunden jeweils eine Tour und die Rangfolge innerhalb der Tour zuordnen.

**Nutzen**
*   Sie stellen Aufträge nach Liefertermin und Tour zusammen, um effektive Lieferungen zu erreichen.
*   Tourenlisten können Sie nach verschiedenen Kriterien zusammenstellen und so den Versand optimieren.

**Merke**
*   **Tour**: Eine Tour wird in den Stammdaten eingerichtet. Sie legt fest, an welchen Tagen welches Gebiet angefahren wird.
*   **Tourrangfolge**: Die Tourrangfolge legt fest, welcher Kunde in einer bestimmten Tour zuerst beliefert wird, wenn ein zweiter Kunde mit derselben Tour beliefert werden soll.
*   **Dialog Tourenliste**: Im Dialog Tourenliste können Sie den Versand planen. Die Aufträge einer Tour können Sie sich nach verschiedenen Auswahlkriterien zusammenstellen, z. B. nach Liefertermin, Produkt, Status.
*   **Änderungen**: Bei der Versandplanung können Sie einem Auftrag eine andere Tour und einen anderen Termin zuweisen. Beides wird in den Auftrag zurückgeschrieben.
*   **Voreinstellungen**:
    *   Stammdaten:
        *   Lieferbedingungen
        *   Touren
        *   Lkw
        *   Fahrer
    *   Kunde, Lieferant:
        *   Lieferdauer
    *   Kundendaten:
        *   Register Adresse > Tour 1, 2
        *   Register Auftrag > Tourrangfolge
    *   Firmendaten:
        *   Register Versand

#### Definierte Touren

Pro Tour werden in den Stammdaten die Wochentage festgelegt, an denen sie gefahren wird. So kann eine Tour z. B. von Frankfurt nach Karlsruhe so eingerichtet sein, dass sie montags und donnerstags gefahren wird. Mit dieser Tour sollen alle Kunden beliefert werden, die auf dieser Strecke im Umkreis von 50 km liegen.
Jedem Kunden werden eine passende Tour und eine Rangfolgenummer zugewiesen. Die Rangfolgenummer bestimmt die Reihenfolge, in der die Kunden pro Tour beliefert werden.

> **Beispiel**
> Kunde A und Kunde B werden mit Tour Süd beliefert. Kunde A hat die Tourrangfolge 1, Kunde B hat die Tourrangfolge 2.
> Kunde A wird also vor Kunde B beliefert.

Diese Einstellungen aus den Stammdaten werden in den Auftrag übernommen. Die Vorbelegung kann pro Auftrag geändert werden. Dabei wird automatisch geprüft, ob der eingegebene Liefertermin mit den Tourentagen des Kunden übereinstimmt. Bei einer Abweichung wird eine entsprechende Meldung ausgegeben. Abweichende Daten können gespeichert werden. Sie werden in der Tourenplanung übernommen.

#### Neue Tour definieren

Sie können die hinterlegten Touren modifizieren oder durch neue Touren ergänzen. Wenn z. B. die Frachtkosten berechnet werden sollen, müssen Sie pro Tour die Kilometerpauschale eintragen. Die Berechnung der Frachtkosten lernen Sie in einer gesonderten Einheit kennen.
⇨ "Frachtkosten" auf Seite E-139

**So richten Sie eine neue Tour ein**

1.  Wählen Sie im Menü **Stammdaten > Versand > Touren**. Der gleichnamige Dialog wird geöffnet.
    ⇨ Stammdaten, "Touren" auf Seite B-873
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    
    *[Image of the 'Versand-Tour anlegen' dialog. Labels point to: A) Zeile für neue Tour, B) Tourentage, C) Lieferpauschale, D) Lieferdauer, E) Schicht, in der die Tour fährt.]*

3.  Geben Sie die Nummer und Bezeichnung (A) ein. Beide können frei gewählt werden.
4.  Aktivieren Sie die Checkboxen für die Tage (B), an denen diese neue Tour regelmäßig gefahren wird.
    Die Angaben werden in der Auftragserfassung mit dem eingetragenen Liefertermin verglichen. Eine Meldung macht Sie darauf aufmerksam, wenn Termin und Tourentag nicht übereinstimmen.
5.  Prüfen Sie, ob die Lieferpauschale (C) berechnet werden soll. Für Abholungen und Speditionen markieren Sie die Checkbox, damit die Lieferpauschale nicht berechnet wird.
    Wenn Sie mit der A+W Business-Kapazitätsplanung arbeiten, können Sie festlegen, in welchen Schichten (E) die Tour gefahren wird, z. B. am Montag in Schicht 2, von Dienstag bis Freitag in Schicht 1.
6.  Verschieben Sie die Ansicht nach rechts (scrollen), um z. B. die Abfahrzeiten einzugeben.
    
    *[Image of the tour settings, showing columns for departure times (Abfahrtzeit pro Tourentag - A) and cost per kilometer (Kilometerpauschale - B).]*
    
    Sie können die Abfahrtzeit (A) für jeden einzelnen Tourentag festlegen. Der Abfahrttermin wird nach der Produktionsübergabe von A+W Production Capacity Planner ausgewertet. Er wird bei der Produktionsübergabe im OrderXML-Format an die Produktion exportiert. Dadurch kennt auch die Produktionssoftware nach dem Import eines Auftrags die genaue Abfahrtszeit der Tour, mit der der Auftrag ausgeliefert werden soll.
7.  Tragen Sie den Betrag der Lieferpauschale (B) ein, der pro Kilometer berechnet werden soll.
8.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Daten werden gespeichert.
9.  Wiederholen Sie ggf. die Schritte 2 bis 8 für weitere Touren.

#### Sperrkennzeichen

Eine einmal eingerichtete und zugewiesene Tour können Sie nicht löschen. Sie können eine Tour, die nicht mehr zugewiesen werden soll, jedoch sperren. Eine gesperrte Tour wird nicht mehr zur Auswahl angeboten. In den gespeicherten Aufträgen wird sie aber weiterhin angezeigt.

*[Image comparison: A) A list of tours available for selection in a document. B) The same list, but a 'gesperrte' (blocked) tour is now missing from the selection.]*

**So sperren Sie eine Tour**

1.  Wählen Sie im Menü **Stammdaten > Versand > Touren**.
2.  Markieren Sie die Tour und verschieben Sie die Anzeige mit dem unteren Scroll-Balken bis die Spalte **Gesperrt** sichtbar wird.
3.  Markieren Sie die gewünschte Checkbox und speichern Sie die Änderung. Die Tour wird jetzt in der Dokumentenverwaltung nicht mehr zur Auswahl angeboten.

> **Sperren von Stammdaten**
> Auf die gleiche Weise können für den Bereich Fertigung/Versand auch Lieferbedingungen, Lkws, Fahrer, Zolltouren und Verpackungen gesperrt werden.

#### Tour planen

In diesem Abschnitt lernen Sie, wie Sie Tourenlisten zusammenstellen und ändern.

**So planen Sie eine Tour**

1.  Wählen Sie im Menü **Fertigung > Lieferwesen > Tourenliste**.
    ⇨ Softwarereferenz, "Tourenliste" auf Seite E-207
    
    Sie können folgende Alternativen für die Zusammenstellung wählen:
    *   **Liefertermin oder Zeitspanne eingeben (A):** In diesem Fall können Sie die Auswahl zusätzlich auf einen Status und/oder einen AV-Bereich einschränken.
    *   **Nummernverwalter wählen (D):** In diesem Fall können Sie die Auswahl zusätzlich nur auf einen AV-Bereich einschränken.
    
    In beiden Fällen können Sie außerdem die Details für die Auflösungstiefe (E) und den Druck (F) festlegen.
    
    *[Image of the 'Tourenliste - Tour zusammenstellen' dialog. Labels point to: A) Zeitliche Eingrenzung, B) Auswahl der Tour, C) Einschränkung über Status, D) Nummernverwalter, E) Auflösungstiefe, F) Status der Dokumente, die nicht gedruckt werden sollen, G) Ziel-Nummernverwalter.]*

2.  In diesem Beispiel wird eine Zeitspanne (A) angegeben. Stellen Sie eine Zeitspanne ein, in der die Liefertermine liegen sollen.
3.  Wählen Sie aus der Liste der verfügbaren Touren (B) diejenige aus, zu der Sie die Aufträge anzeigen lassen wollen.
    Wenn Sie eine Zeitspanne eingetragen haben, werden alle Aufträge pro Tag und ausgewählter Tour angezeigt. Das bedeutet, dass die Anzeige der Tourenliste schnell unübersichtlich wird, wenn die Zeitspanne und die Anzahl der Touren groß sind. In diesem Beispiel sind daher eine kurze Zeitspanne und nur eine Tour ausgewählt. Die Auswahl aller Touren an einem bestimmten Liefertermin ist ebenso denkbar.
4.  Grenzen Sie den Status der Aufträge ein (C), z. B. von **Dokument erfasst** bis **Lieferschein gedruckt**.
    Sie können Aufträge mit einem bestimmten Status vom Druck ausschließen (F). Für die Mehrfachauswahl brauchen Sie keine Taste zu drücken. Diese Einstellung ist sinnvoll, wenn Sie die Touren nach Liefertermin zusammenstellen.
    Wenn Sie eine Auswahl getroffen haben, werden die entsprechenden Aufträge im Register **Tabelle** in blauer Schrift dargestellt.
    In diesem Beispiel werden die Aufträge dazu auch in einen neuen Nummernverwalter kopiert (G), aus dem der Druck gestartet werden soll.
5.  Markieren Sie dazu die Checkbox **NV komplett füllen** und tragen Sie einen Namen des Nummernverwalters ein.
6.  Legen Sie die Auflösungstiefe (E) und ggf. die Sortierung innerhalb der Touren fest.
7.  Bestimmen Sie ggf., an welcher Stelle beim Druck ein Seitenwechsel eingefügt werden soll.
8.  Wählen Sie im Menü **Start > Ausführen**, um die Aktion zu starten.
    Die Anzeige wechselt automatisch zum Register **Tabelle**. Wenn die Auswahlkriterien mehrere Touren gefunden haben, können Sie sich jede einzelne anzeigen lassen.
    Wie Sie mit der Tourenliste weiterarbeiten können, lernen Sie in den nächsten Einheiten.
    *   "Versanddaten ändern" auf Seite E-89
    *   "Tourenliste drucken" auf Seite E-91

#### Versanddaten ändern

Sie können die Vorgaben aus den Stammdaten und dem Auftrag überschreiben, um mit diesen Änderungen die Versanddaten optimal zusammenzustellen.

**So ändern Sie die Tour oder den Liefertermin**

1.  Wählen Sie im Menü **Fertigung > Lieferwesen > Tourenliste**.
2.  Lassen Sie sich die Touren anzeigen, die Sie ändern wollen.
3.  Wechseln Sie zum Register **Tabelle**.
4.  Wählen Sie ggf. im Feld **Datum/Tour** das Datum und die Tour aus, um sich die Aufträge anzeigen zu lassen, die in dieser Tour enthalten sind.
5.  Markieren Sie in der Übersicht den Auftrag, den Sie ändern wollen mit einem Doppelklick in den Zeilenkopf.
    
    *[Image of the 'Tour bearbeiten' list. Label A points to the selection marker 'x' for changing an order. Label B points to the summary totals for the displayed orders.]*
    
    Nur die Aufträge werden geändert, bei denen im Zeilenkopf ein **x (A)** angezeigt wird. Sie können mehrere Aufträge markieren, die Sie gemeinsam ändern wollen.
    Sie können alle Aufträge markieren, indem Sie auf **[Alle]** klicken.
6.  Wählen Sie im Menü **Funktionen > Gruppe Tour > Versanddaten ändern**.
    
    *[Image of the 'Versanddaten ändern' dialog.]*

7.  Markieren Sie mindestens eine der Checkboxen:
    *   **Liefertermin**, wenn Sie das Datum ändern wollen.
    *   **Tour**, wenn Sie eine andere Tour zuordnen wollen.
    *   **Lieferbed.**, wenn Sie die Lieferbedingungen ändern wollen.
    *   **Fahrer**, wenn Sie einen anderen Fahrer zuordnen wollen.
    *   **LKW**, wenn Sie einen anderen Lkw zuordnen wollen.
8.  Tragen Sie hinter jeder markierten Checkbox die neuen Versanddaten ein.
    Die Änderungen gelten für alle Aufträge, die im Dialog **Versanddaten ändern** angezeigt werden.
9.  Klicken Sie auf **[OK]**, um die Daten zu speichern.
    Die neuen Versanddaten werden übernommen.
10. Klicken Sie auf **[Ende]**, um den Dialog zu schließen.
    Der Dialog **Tourenliste** wird wieder im Vordergrund angezeigt. Die geänderten Touren werden aus der Übersicht entfernt.

#### Tourenliste drucken

> **Lieferscheindruck nach Tourenliste**
> Wenn Sie Ihre Lieferscheine in der Reihenfolge der Tourenliste drucken wollen, können Sie die angezeigten Aufträge in einen anderen Nummernverwalter kopieren.
> *   Wählen Sie dazu im Menü **Funktionen > Alle in Nummernverwalter kopieren** und stellen Sie den gewünschten Nummernverwalter ein.
> *   Wenn Sie nur die markierten Aufträge in einen anderen Nummernverwalter kopieren wollen, wählen Sie im Menü **Funktionen > Selektierte in Nummernverwalter kopieren** und stellen Sie den gewünschten Nummernverwalter ein.
> *   Wenn Sie die Checkbox **Löschen** markieren, wird der gewählte Nummernverwalter zuvor geleert und neu gefüllt.

Das Ergebnis Ihrer Arbeit können Sie als Liste drucken, um einen Gesamtüberblick über die Touren in einem bestimmten Zeitraum zu gewinnen.

**So drucken Sie die Tourenliste**

1.  Stellen Sie die Tourenliste zusammen, wie in der Handlungsanleitung zuvor beschrieben.
    ⇨ "So planen Sie eine Tour" auf Seite E-87
2.  Achten Sie auf die Einstellung im Bereich **Seitenwechsel bei Druck**:
    *   **Tour/Datum**: Wenn Sie mehrere Touren ausgewählt haben, werden diese pro Tour nach Datum auf eine neue Seite gedruckt.
    *   **Tour/Datum/Kunde**: Wenn Sie mehrere Touren ausgewählt haben, werden diese pro Tour nach Datum und Kunde auf eine neue Seite gedruckt.
    *   **Kein Wechsel**: Die Touren werden fortlaufend pro Tour nach Datum und Kunde gedruckt.
    *   **Tour/Datum/Kunde/Lieferanschr.**: Wenn Sie mehrere Touren ausgewählt haben, werden diese pro Tour nach Datum und Kunde und Lieferanschrift auf eine neue Seite gedruckt.
3.  Wählen Sie im Menü **Optionen > Gruppe Druckoptionen** die Einstellungen für den Druck aus.
    Wenn z. B. der Eintrag **Zuschlags- und Leistungspositionen** ausgewählt ist (orangefarbener Hintergrund), werden die Zuschläge und Leistungen mit in die Tourenliste gedruckt.
4.  Wählen Sie im Menü **Druck > Bildschirm** oder **Drucker**.
    Der Dialog **Druck-Tourenliste** wird geöffnet.
5.  Prüfen Sie die aktuellen Einstellungen und wechseln Sie ggf. auf das Querformat, wenn Sie sehr viele Details mit drucken lassen wollen.
6.  Klicken Sie auf **[OK]**, um den Druck zu starten.
    
    *[Image of a sample tour list for shipping planning.]*
    
    Dargestellt werden je nach Auflösungstiefe pro Liefertermin und Tour mindestens:
    *   Kunde
    *   Auftragsnummer und Teillieferungsnummer
    *   Menge, Fläche und Gewicht pro Position
    *   Gesamtsummen pro Auftrag
    
    Der Name des Lieferanten wird nur angegeben, wenn diese Option gewählt wurde.

> **Weitere Listen drucken**
> Beladungs- und Bestätigungslisten für den Fahrer können Sie über den Dialog Listendruck erzeugen. Dazu sollten Sie zuvor in der Kommissionierung mindestens Fahrzeuge und Fahrer zuordnen.
> ⇨ "Listen drucken" auf Seite E-113

#### Übungen

*   Stellen Sie im Dialog **Tourenliste** verschieden Listen von Touren zusammen und vergleichen Sie die Ergebnisse, die im Register **Tabelle** angezeigt werden:
    *   Legen Sie dazu einen Nummernverwalter an und sammeln Sie darin verschiedene Aufträge.
    *   Stellen Sie eine Liste zusammen, indem Sie auf diesen Nummernverwalter zugreifen.
    *   Stellen Sie eine andere Liste zusammen, indem Sie die Dokumente nach einem bestimmten Status sammeln.
    *   Schränken Sie die Auswahl auf ein bestimmtes Lieferdatum ein.
*   Ändern Sie im Register **Tabelle** den Liefertermin in einem Auftrag und beobachten Sie die Anzeige. Prüfen Sie, nach welchen Auswahlkriterien der Auftrag jetzt angezeigt wird.
*   Lassen Sie sich für jede Liste auch den Bildschirmdruck anzeigen und vergleichen Sie die Ergebnisse.

**Ergänzende Informationen**
*   ⇨ Stammdaten, "Tourrangfolge" auf Seite B-803
*   ⇨ Stammdaten, "Lieferdauer (Kunde, Lieferant)" auf Seite B-832
*   ⇨ Stammdaten, "Touren" auf Seite B-873
*   ⇨ Stammdaten, "Lkw" auf Seite B-876
*   ⇨ Stammdaten, "Fahrer" auf Seite B-877
*   ⇨ Stammdaten, "Firmendaten - Versand" auf Seite B-1008
*   ⇨ Softwarereferenz, "Tourenliste" auf Seite E-207

### Statusmeldung

**Lernziele**
*   Statuszuordnungen für die Produktionsübergabe und Fertigmeldungen prüfen.
*   Regeln der Statusumsetzung kennenlernen.
*   Auftragsstatus per Tastatur-Scanner umsetzen.
*   Auftragsstatus per Tastatur umsetzen.

**Nutzen**
*   Aufträge können nur weiterbearbeitet werden, wenn der Auftragsstatus dies zulässt. Der Status wird in der Regel durch Rückmeldungen aus der Produktionssoftware umgesetzt.
*   Die (manuellen) Statusmeldungen per Scanner werden eingesetzt, wenn nicht mit (automatischen) Rückmeldungen aus der Betriebsdatenerfassung (BDE) gearbeitet werden kann.

**Merke**
*   **Status**: Der Status kann einer Auftragsposition und einem Auftrag zugewiesen werden. Er zeigt an, an welcher Stelle der Auftragsabwicklung sich ein Auftrag befindet und welche Aktionen als Nächstes möglich sind.
*   **Statuserhöhung**: Der Status des Auftrags wird erhöht (umgesetzt), wenn alle Auftragspositionen einen einheitlichen, höheren Status haben, z. B., wenn alle Positionen eines Auftrags fertig gemeldet wurden.
*   **Automatische Statuserhöhung**: Wenn Sie mit Rückmeldungen aus der Produktion (BDE) arbeiten, wird der Status einer Auftragsposition umgesetzt, wenn eine neue Rückmeldedatei vorliegt.
*   **Statuserhöhung (per Tastatur oder Scanner)**: Mit der Statusumsetzung simulieren Sie die Statuserhöhung durch Rückmeldungen. Pro Registrierungsstelle (Mitarbeiter) können die Statuspunkte festgelegt werden, die umgesetzt werden dürfen.
*   **Voreinstellungen**:
    *   Stammdaten:
        *   Statuszuordnung
    *   Fertigung:
        *   Statusmeldung > Einstellungen

#### Auftragsstatus

Aufträgen (Dokumenten) wird mit jeder Aktion ein spezifischer Status zugewiesen. Über die Zuordnung von Mindest- und oder Sperrstatus kann gesteuert werden, was mit dem Auftrag gemacht werden kann. Dazu müssen in den Stammdaten die Statuspunkte und Statuszuordnungen vollständig eingerichtet sein.

#### Statusverwaltung und -zuordnung prüfen

In diesem Abschnitt lernen Sie, wie Sie die Statuseinstellungen prüfen, die für die Produktionsübergabe und die Rückmeldungen benötigt werden. Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So prüfen Sie die Statusverwaltung" auf Seite E-95
*   "So prüfen Sie die Statuszuordnung" auf Seite E-96

**So prüfen Sie die Statusverwaltung**

1.  Wählen Sie im Menü **Stammdaten > Auftrag > Statusverwaltung**.
    
    *[Image of the 'Statusverwaltung' dialog.]*
    
    ⇨ Stammdaten, "Statusverwaltung" auf Seite B-897
2.  Prüfen Sie, ob der Anwenderstatus z. B. für folgende Vorgänge vorhanden ist und legen Sie diese ggf. an:
    *   Auftrag für Produktion freigegeben
    *   Auftrag an Produktion übergeben
    *   Auftrag fertig gemeldet
    *   Auftrag versandbereit
    *   Produziert (AWBar)
    *   Versandfertig (AWBar)
    *   Ausgeliefert (AWBar)
3.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
4.  Geben Sie die Nummer und die Bezeichnung ein.
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Daten werden gespeichert.
6.  Prüfen Sie als Nächstes die Statuszuordnungen.

**So prüfen Sie die Statuszuordnung**

1.  Wählen Sie im Menü **Stammdaten > Auftrag > Statuszuordnung**.
    
    *[Image of the 'Statuszuordnung' dialog.]*
    
    ⇨ Stammdaten, "Statuszuordnung" auf Seite B-899
2.  Prüfen Sie alle Statuszuordnungen für den Dokumententyp **Auftrag**, die Sie per Scanner melden wollen, z. B.:
    *   AWBar produziert
    *   AWBar versandfertig
    *   AWBar ausgeliefert
3.  Legen Sie die fehlenden Zuordnungen an und korrigieren Sie die vorhandenen ggf.
4.  Wählen Sie im Menü **Start > Speichern**, um Änderungen zu speichern. Die Änderungen werden gespeichert.

#### Manuelle Statusumsetzung

Wenn Sie in der Produktion nicht mit Rückmeldungen aus der Betriebsdatenerfassung (BDE) arbeiten, können Sie über den Dialog **Statusmeldung und Packmittelzuordnung** Aufträge einscannen. Damit können Sie die BDE-Meldungen simulieren.
Aufträge oder Auftragspositionen werden dabei in der Regel über einen Tastatur-Scanner erfasst. Im Auftrag setzen Sie den Status z. B. aus folgenden Gründen um:
*   Für den gesamten fertiggestellten Auftrag, damit er gepackt und ausgeliefert wird.
*   Für einzelne Auftragspositionen, damit ggf. eine Teillieferung eingeleitet werden kann.

Nach Abschluss des Scanvorgangs können z. B. die Versandpapiere gedruckt werden.
Für die Umsetzung des Status können die Zugriffsrechte unterschiedlich eingestellt werden:
*   Der Mitarbeiter kann nur den voreingestellten Status vergeben. Dies geschieht ohne weiteren Eingriff in dem Moment, in dem ein Auftrag oder eine Auftragsposition gescannt wird.
*   Der Mitarbeiter kann mehr als einen Status vergeben. In diesem Fall muss auch der zu vergebende Status gescannt werden.
*   Zusätzlich kann festgelegt werden, ob der Status nur erhöht oder auch zurückgesetzt werden kann.

#### Einstellungen für manuelle Statusmeldungen

Die Optionen für die Statusmeldungen können nur von einem Mitarbeiter mit Administratorrechten eingerichtet werden. Für jeden Arbeitsplatz kann festgelegt werden, welche Statuspunkte einlesbar sind.

**So legen Sie Statuspunkte für Statusmeldungen fest**

1.  Wählen Sie im Menü **Fertigung > Lieferwesen > Statusmeldung**.
    Der Dialog **Statusmeldung und Packmittelzuordnung** wird geöffnet.
2.  Wählen Sie im Menü **Funktionen > Gruppe Funktionen > Einstellungen**.
    
    *[Image of the options for status messages dialog.]*

3.  Markieren Sie im Feld **verfügbare Statuspunkte** den gewünschten Eintrag.
4.  Klicken Sie auf den Pfeil nach rechts, um den Statuspunkt in das Feld **änderbare Statuspunkte** zu verschieben.
5.  Wiederholen Sie diese Schritte für alle Statuspunkte, die geändert werden dürfen.
6.  Markieren Sie die Checkbox **Statusverminderung erlauben**, wenn ein Status auch zurückgesetzt werden darf.
7.  Sie können zusätzlich festlegen, ob automatisch die Laufnummer 9999 eingetragen werden soll, wenn keine eigene Laufnummer vorhanden ist.
    Die Checkbox **keine Laufnr., dann 9999 eintragen** wird freigeschaltet, wenn Sie im Feld **änderbare Statuspunkte** einen Eintrag markieren.
8.  Klicken Sie auf **[OK]**, um die Einstellungen zu speichern.
    Am aktuellen Arbeitsplatz können nur die Statuspunkte vergeben werden, die im Feld **verfügbare Statuspunkte** aufgelistet sind. An anderen Arbeitsplätzen müssen Sie die Optionen neu anpassen.

#### Status manuell umsetzen

> **Reihenfolge der Eingaben beachten**
> Tragen Sie zuerst alle Vorgaben ein, die für diese Sitzung gelten sollen. Beginnen Sie beim Scannen dann mit dem Status und lesen Sie erst danach den Auftrag ein.

Zu dieser Einheit gibt es folgende Handlungsanleitungen:
*   "So setzen Sie den Status eines Auftrags per Scanner um" auf Seite E-99
*   "So setzen Sie den Status einer Auftragsposition per Scanner um" auf Seite E-101
*   "So ordnen Sie den Auftragspositionen ein Gestell zu" auf Seite E-102

**So setzen Sie den Status eines Auftrags per Scanner um**

1.  Wählen Sie im Menü **Fertigung > Lieferwesen > Statusmeldung**.
    
    *[Image showing the status update dialog for an order using a barcode. Labels are: A) Display when only one status is allowed, B) Number range for reported orders, C) Function to activate the number range.]*
    
    ⇨ Softwarereferenz, "Statusmeldung und Packmittelzuordnung" auf Seite E-220
    
    Der Cursor steht automatisch im Feld **Auftrag/Statuspunkt**. Wenn Sie nur einen Status vergeben können, wird dieser in der Titelzeile (A) angezeigt.
2.  Wenn Sie mehr als einen Status vergeben können, scannen Sie zuerst den Barcode des Status.
3.  Geben Sie ggf. im Bereich **Vorgabe** ein neues Datum für das Ende der Produktion und/oder für die Anlieferung ein.
4.  Markieren Sie die Checkbox **In NV kopieren (C)**, wenn die geänderten Aufträge in einen Nummernverwalter kopiert werden sollen.
    Das Feld **Zielnummernverwalter** wird freigeschaltet und Sie können den gewünschten Nummernverwalter auswählen.
5.  Stellen Sie den Cursor in das Feld **Auftrag/Statuspunkt**.
6.  Scannen Sie die Auftragsnummer.
    Die Auftragsnummer wird im Feld **Auftrag/Statuspunkt** angezeigt und die Schaltfläche **[Speichern]** wird freigeschaltet.
7.  Wählen Sie im Menü **Start > Speichern**, um die Auftragsnummer zu bestätigen.
    Der Auftrag wird in der Übersicht angezeigt. Der Status ist umgesetzt. Wenn Sie einen Zielnummernverwalter angegeben haben, ist der Auftrag in diesen kopiert worden.
8.  Wiederholen Sie die Schritte 6 und 7, um den nächsten Auftrag zu scannen.
    Um dem aktuellen Auftrag ein Gestell zuzuordnen, wechseln Sie zum Register **Manuelle Packmittelzuordnung**.
    ⇨ "So ordnen Sie den Auftragspositionen ein Gestell zu" auf Seite E-102

> **Kein Scanner angeschlossen**
> Wenn Ihr Scanner ausgefallen ist, können Sie den Status über die Tastatur umsetzen. Geben Sie in diesem Fall ein **s** und den Code für den Status ein und ein **o** und die Auftragsnummer, z. B. **s68** und **o1234**.

**So setzen Sie den Status einer Auftragsposition per Scanner um**

1.  Wählen Sie im Menü **Fertigung > Lieferwesen > Statusmeldung** und wechseln Sie zum Register **Statusmeldung – Position**.
    Der Cursor steht automatisch im Feld **Auftrags-Pos/Statuspunkt**. Wenn Sie nur einen Status vergeben können, wird dieser im Info-Bereich angezeigt.
2.  Geben Sie ggf. im Bereich **Vorgabe** ein neues Datum für das Ende der Produktion und/oder die Anlieferung ein.
3.  Scannen Sie den Barcode der Auftragsposition.
    Der Barcode wird im Feld **Auftrags-Pos/Statuspunkt** angezeigt und die Schaltfläche **[Speichern]** wird freigeschaltet.
4.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    
    *[Image of the position status update via barcode scan.]*
    
    Die Auftragspositionen werden eingelesen. Der Status der gescannten Position ist umgesetzt.
5.  Wiederholen Sie die Schritte 3 und 4, um die nächste Position zu scannen.
    Der Status des Auftrags wird erst umgesetzt, wenn der Status aller Auftragspositionen identisch umgesetzt ist.

**So ordnen Sie den Auftragspositionen ein Gestell zu**

1.  Klicken Sie im Register **Statusmeldung - Auftrag** doppelt auf eine Auftragsnummer, um zum Register **Manuelle Packmittelzuordnung** zu wechseln.
    
    *[Image of the 'Packmittel zuordnen' (Assign Rack) dialog.]*
    
    Die Positionen des aktuellen Auftrags werden in der Übersicht angezeigt.
2.  Wählen Sie im Feld **Packmittel** die Gestellart aus.
3.  Markieren Sie die Position, die auf einem Gestell steht.
4.  Stellen Sie den Cursor in das Eingabefeld und scannen Sie die Gestellnummer.
    Der Fokus springt danach automatisch auf die nächste Auftragsposition.
5.  Drücken Sie auf **<Enter>**, um die Zuordnung zu übernehmen.
    Wenn allen Positionen ein Gestell zugeordnet ist, werden automatisch die Positionen des nächsten Auftrags aus dem Register **Statusmeldung – Auftrag** angezeigt.
    Wenn das nächste Gestell belegt wird, muss zuerst das Gestell gescannt werden.
    Wenn Sie keinen Scanner haben, können Sie die Gestellnummer über die Schaltfläche hinter dem Eingabefeld auswählen.
6.  Wählen Sie im Menü **Start > Speichern**, um die Gestellzuordnung zu speichern.
    Die Daten werden gespeichert. Sie können jetzt im Dialog **Listendruck** verschiedene Listen für die Beladung und den Fahrer drucken.
    ⇨ "Listendruck für den Fahrer" auf Seite E-113

#### Scan-Vorlage herstellen

> In der Regel stellt die A+W Software GmbH die Vorlagen zum Scannen des Status zur Verfügung. Sie können diese Vorlagen ergänzen oder neue Barcodes einrichten.
> **Voraussetzung**
> Auf dem Rechner müssen ein Programm zur Textverarbeitung und eine Barcode-Schriftart installiert sein. Achten Sie dabei darauf, welchen Codetyp Ihre Scanner lesen, z. B. Code 39.

**So stellen Sie sich eine Scan-Vorlage mit Barcodes her**

1.  Starten Sie das Programm zur Textverarbeitung, z. B. Word.
2.  Schreiben Sie die Nummer und die Bezeichnung des Barcodes.
3.  Wiederholen Sie in der nächsten Zeile die Nummer mit einem vorangestellten s, z. B. **s48**.
4.  Weisen Sie der Zeile die Barcode-Schriftart und eine geeignete Schriftgröße zu.
    
    *[Image of a Word document being used to create a barcode scan template.]*
    
5.  Drucken Sie die Vorlage aus und prüfen Sie, ob die Barcodes korrekt gelesen werden.

#### Übungen

Setzen Sie den Status eines Auftrags um, indem Sie den Tastatur-Scanner simulieren.
*   Erhöhen Sie den Status.
*   Können Sie den Status vermindern? Wenn nein, warum nicht?
*   Ändern Sie die Einstellung und wiederholen Sie die Statusverminderung.

**Ergänzende Informationen**
*   ⇨ Stammdaten, "Statusverwaltung" auf Seite B-897
*   ⇨ Stammdaten, "Statuspunkte" auf Seite B-898
*   ⇨ Softwarereferenz, “Statusmeldung und Packmittelzuordnung" auf Seite E-220
*   ⇨ Softwarereferenz, "Optionen in Statusmeldung" auf Seite E-225

### Kommissionierung

**Lernziele**
*   Fahrzeug für eine Fahrt optimal beladen.
*   Listen für den Transport pro Datum und Tour erstellen, nach denen die Lieferfahrzeuge beladen werden.

**Nutzen**
*   Mit der Kommissionierung organisieren Sie den Versand mit Ihrem eigenen Fuhrpark. Das Gesamtgewicht der Aufträge, die mit einem Fahrzeug transportiert werden sollen, wird angezeigt. Eine Überladung oder ein nicht ausgelastetes Fahrzeug werden so schon bei der Planung vermieden.
*   Mit den Beladungslisten geben Sie dem Fahrer konkrete Informationen darüber, welche Gestelle für die aktuelle Fahrt geladen werden müssen.
*   Über Empfangsbestätigungslisten lässt der Fahrer sich die korrekte Auslieferung eines jeden Auftrags quittieren.

**Merke**
*   **Fuhrpark**: In den Stammdaten müssen mindestens die Fahrzeuge hinterlegt sein. Wenn Sie auch Fahrer zuordnen wollen, müssen diese ebenfalls in den Stammdaten hinterlegt sein.
*   **Gestelle**: Die Bezeichnungen Gestell und Packmittel werden synonym verwendet. Darunter sind die unterschiedlichen Formen von Gestellen, aber auch Gitterboxen, Paletten usw. zu verstehen.
*   **Fahrzeugbeladung**: Sie können die Liste für die Transportmittelbeladung nur drucken, wenn Sie den Auftragspositionen Gestelle zugeordnet haben.
*   **Transportmittel**: Alle Auftragspositionen werden transportgerecht verpackt. Dazu stehen verschiedene Packmittel zur Verfügung, z. B.:
    *   Gestelle unterschiedlicher Größe und Ausführung
    *   Container
    *   Böcke usw.
*   **Gestellzuordnung**: Auftragspositionen müssen Gestelle (Packmittel) zugeordnet sein, damit sie in der Beladungsliste aufgeführt werden können.
*   **Voreinstellungen**: Stammdaten
    *   Fahrzeuge

#### Organisation der Auslieferung

Mit der Tourenplanung haben Sie den Versand geplant. Sie können nun die Auslieferung der gefertigten Aufträge mit einem eigenen Fuhrpark planen. Die Kommissionierung dient dazu, die Aufträge pro Liefertermin und Tour zusammenzustellen und einem Fahrzeug zuzuweisen.

Damit Sie Fahrzeuge und Fahrer zuordnen können, müssen diese in den Stammdaten angelegt sein. Zu jedem Lkw hinterlegen Sie das Leergewicht und das zulässige Gesamtgewicht. A+W Business prüft bei der Zuordnung von Aufträgen, ob dieses Gesamtgewicht erreicht oder sogar überschritten ist. Wenn im Dialog Kommissionierung angezeigt wird, dass der Lkw überladen ist, müssen die selektierten Aufträge einer anderen Tour, einem anderen Lkw und/oder einem anderen Liefertermin zugeordnet werden.

Sie können jedem Fahrzeug auch einen Fahrer zuordnen, der jedoch nicht zwingend in die Kommissionierung übernommen wird.

Für die Kommissionierung können die Aufträge automatisch in einem Nummernverwalter gesammelt werden. Aus diesem heraus kann dann die entsprechende Packmittelbeladungsliste oder Empfangsbestätigungsliste gedruckt werden.

Mit dem Ausdruck verschiedener Listen unterstützen Sie die Fahrer bei der Beladung und bei der Lieferung.

> **Voraussetzung**
> Wenn Sie den Fahrzeugen Fahrer zuordnen wollen, müssen Sie zuerst die Namen der Fahrer in den Stammdaten hinterlegen.

#### Fahrzeug anlegen

Um die Lieferungen einer Tour zusammenzustellen, ordnen Sie die Aufträge einem Fahrzeug zu. Nur wenn die Daten für die Fahrzeuge korrekt eingetragen sind, kann das System prüfen, ob das ausgewählte Fahrzeug richtig ausgelastet oder überladen ist. In diesem Abschnitt lernen Sie, wie Sie Stammdaten für Fahrzeuge anlegen.

**So legen Sie ein Fahrzeug an**

1.  Wählen Sie im Menü **Stammdaten > Versand > LKW**.
    
    *[Image of the 'LKW-Verwaltung' dialog.]*
    
    ⇨ Stammdaten, "Lkw" auf Seite B-876
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    Die Felder werden freigeschaltet.
3.  Geben Sie die Bezeichnung, Leer-Gewicht und Gesamt-Gewicht ein.
    Leer- und Gesamt-Gewicht werden in der Kommissionierung angezeigt, so dass der Lkw nicht überladen werden kann.
    Als Bezeichnung können Sie auch die Spedition eintragen, mit der Sie die Aufträge ausliefern.
4.  Wählen Sie ggf. den Fahrer aus, der diesen Lkw in der Regel fährt.
    Der Fahrer kann in der Versandplanung geändert werden.
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.
6.  Wiederholen Sie ggf. die Schritte 2 bis 5 für weitere Fahrzeuge.

#### Fahrerdaten anlegen

Die Namen der Fahrer können einem bestimmten Fahrzeug und einer Tour zugeordnet werden. Diese einmal hinterlegten Namen können nicht wieder gelöscht werden. Wenn ein Fahrer nicht mehr eingesetzt werden soll, müssen Sie ihn sperren. In diesem Abschnitt lernen Sie, wie Sie Stammdaten für Fahrer anlegen.

**So legen Sie einen Fahrer an**

1.  Wählen Sie im Menü **Stammdaten > Versand > Fahrer**.
    
    *[Image of the 'Stammdaten - Fahrer anlegen' dialog.]*
    
    ⇨ Stammdaten, "Lkw" auf Seite B-876
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
3.  Geben Sie den Namen ein.
4.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.
5.  Wiederholen Sie ggf. die Schritte 2 bis 4 für weitere Fahrer.

#### Fahrzeugbeladung zusammenstellen

Um die Aufträge einer Tour auszuliefern, müssen die Packmittel (Gestelle) auf Fahrzeuge verladen werden. Dabei wird die Zuladung gegen das zulässige Gesamtgewicht des Fahrzeugs geprüft und eine Überladung angezeigt. In diesem Abschnitt lernen Sie, wie Sie die Aufträge einem Fahrzeug zuordnen.

> **Tipp**
> Legen Sie zunächst einen Nummernverwalter mit dem ersten Auftrag an, der kommissioniert werden soll. In diesem NV können Sie dann alle Aufträge sammeln, für die Sie die Beladungslisten erstellen.
> Wenn Sie die Touren in getrennten Nummernverwaltern sammeln, z. B. nach Lieferterminen, können Sie den Druck besser steuern.

**So stellen Sie die Beladung eines Lkws zusammen**

1.  Wählen Sie im Menü **Fertigung > Lieferwesen > Kommissionierung**.
    
    *[Image of the 'Beladung zusammenstellen' dialog. Labels point to: A) Nummernverwalter, B) Positionen des markierten Auftrags, C) Ausgewählter Lkw, D) Liste der Aufträge, E) Stückzahl, F) Gewicht, G) Maximalgewicht, H) Gesamtstückzahl, I) Gesamtgewicht.]*
    
    ⇨ Softwarereferenz, "Kommissionierung" auf Seite E-230
    
    In der Übersicht (D) werden alle Aufträge angezeigt, die sich im Nummernverwalter befinden. Im Bereich **Positionen (B)** werden jeweils die Positionen eines markierten Auftrags angezeigt.
    Wenn Sie eine Position im Bereich Positionen markiert haben, können Sie den Dialog **Statusmeldung und Packmittelzuordnung** öffnen, indem Sie im Menü **Funktionen > Gestellzuordnung** wählen. Damit können Sie die Gestellzuordnung nachholen, falls Sie eine Transportmittelbeladungsliste drucken wollen.
    ⇨ "So ordnen Sie den Auftragspositionen ein Gestell zu" auf Seite E-102
2.  Markieren Sie ggf. die Checkbox **in NV übernehmen**.
    Die Kombobox (A) zur Auswahl des Nummernverwalters wird freigeschaltet.
3.  Wählen Sie den gewünschten Nummernverwalter aus oder tragen Sie einen neuen Namen ein.
    *   Wenn Sie einen Nummernverwalter auswählen, werden die dort gesammelten Aufträge automatisch aufgelistet.
    *   Wenn Sie diesen Weg gewählt haben, fahren Sie mit Schritt 6 fort.
    *   Wenn Sie einen neuen Namen eingetragen haben, werden alle Aufträge aus der Übersicht entfernt.
    *   Wenn Sie diesen Weg gewählt haben, fahren Sie mit Schritt 4 fort.
4.  Tragen Sie im Feld **Nummer** die Nummer des Auftrags ein, den Sie kommissionieren wollen.
5.  Wählen Sie im Menü **Start > Ausführen**, um die Auftragsdaten einzulesen.
    
    *[Image of the 'Kommissionierung' dialog showing order details. Labels are: A) Lkw zuordnen, B) Fahrer zuordnen, C) Summen aller Aufträge für den Lkw, D) Summen aller markierten Aufträge.]*
    
    Der Auftrag wird im Bereich **Aufträge** angezeigt. Sammeln Sie auf diese Weise weitere Aufträge zusammen.
6.  Markieren Sie den Auftrag, den Sie kommissionieren wollen.
    In den Feldern der Bereiche **Eingabe** und **Positionen** werden die Auftragsdetails angezeigt, die für den Versand wichtig sind. Sie haben jetzt die Möglichkeit, diese Angaben aus dem Auftrag zu ändern, z. B. die Tour oder das Lieferdatum. Die Änderungen werden in den Auftrag zurückgeschrieben.
    Die Werte gelten immer für den gesamten Auftrag. Einzelne Positionen können nur kommissioniert werden, indem Sie eine Teillieferung erstellen.
7.  Prüfen Sie, ob die Lieferbedingung stimmt.
    Wenn ein Auftrag abgeholt werden soll, brauchen Sie ihn nicht weiter zu bearbeiten. Sie können ihn allerdings nicht wieder aus der Übersicht löschen.
8.  Wählen Sie den Lkw (A) aus.
9.  Wählen Sie im Menü **Start > Ausführen**, um die Zuordnung zu übernehmen.
    Wenn dem Lkw in den Stammdaten ein Standard-Fahrer zugeordnet ist, wird dieser automatisch angezeigt. Sie können einen anderen Fahrer auswählen. Die Angaben zum Lkw und zum Fahrer werden in den Auftrag zurückgeschrieben.
    
    Im Bereich **Summen** werden die Gewichte und Stückzahlen aller Aufträge angezeigt, die zum Liefertermin mit dem gewählten Lkw geliefert werden sollen.
    
    Wenn die maximale Zuladung überschritten ist, wird das Gewicht (C) in roten Ziffern angezeigt.
    
    Sie müssen dann dem (letzten) Auftrag eine andere Tour, ein anderes Fahrzeug und/oder ein anderes Lieferdatum zuweisen.
    
    *[Image of the 'Ladeliste' (Loading List) view. Labels are: A) Ladeliste, B) Aufträge für denselben Lkw, C) Summen aller Aufträge für den Lkw.]*
    
    Wenn die Beladung eines Lkws abgeschlossen ist, können Sie außer den Lieferscheinen auch die Transportmittelbeladungsliste und die Empfangsbestätigungsliste drucken.
    ⇨ "Listendruck für den Fahrer" auf Seite E-113

#### Listendruck für den Fahrer

Das Ergebnis der Kommissionierung wird in Form von Listen gedruckt:
*   Die **Transportmittelbeladungsliste** listet die Gestelle für den Lkw auf. Mit dieser Liste wird der Fahrer informiert, welche Gestelle er laden muss.
    ⇨ Softwarereferenz, "Listendruck" auf Seite E-235
*   Die **Empfangsbestätigungsliste** dient dem Fahrer, sich die Auslieferung eines Auftrags vom Kunden quittieren zu lassen. In der Liste sind pro Kunde und Auftrag alle Gestelle mit den darauf befindlichen Mengen aufgeführt.
*   Die **Gestellliste** verschafft Ihnen einen Überblick über die auswärtigen Gestelle. In der Liste sind pro Fahrer, Tour und Kunde alle Gestelle mit ihrem Ausgabedatum aufgeführt.

**Listen drucken**
In diesem Abschnitt lernen Sie, wie Sie die verschiedenen Listen drucken.

> **Gestell zuweisen**
> Sie müssen den Positionen eines Auftrags ein Gestell zuweisen, wenn Sie eine Transportmittelbeladungsliste drucken wollen.

**So drucken Sie die Transportmittelbeladungsliste für den Fahrer**

1.  Wählen Sie im Menü **Fertigung > Lieferwesen > Listendruck**.
    
    *[Image of the 'Listendruck' dialog. Label A points to the number range selection. Label B points to the print settings.]*

2.  Wählen Sie den Nummernverwalter (A) aus, in dem die kommissionierten Aufträge stehen.
    Die Aufträge werden in der Übersicht angezeigt.
3.  Klicken Sie auf die Schaltfläche **[Gestellausgabe]**, um zu prüfen, ob die Gestellzuweisung korrekt ist.
    Der gleichnamige Dialog wird geöffnet.
    
    *[Image of the 'Gestellausgabe prüfen' dialog.]*
    
    Über die Prüfung der Gestellausgabe wird sichergestellt, dass auf einem Gestell nur Aufträge eines Kunden gepackt sind. Auf keinem Gestell dürfen Aufträge unterschiedlicher Kunden gepackt sein.
    Aufträge, denen kein Gestell zugeordnet ist, werden nicht angezeigt.
4.  Klicken Sie auf **[OK]**, um die angezeigten Gestelle auszubuchen und schließen Sie den Dialog mit **[Ende]**.
    Der Dialog **Listendruck** wird wieder im Vordergrund angezeigt.
5.  Markieren Sie die Option (B) für die Liste, die Sie drucken wollen, z. B. **Transportmittelbeladungsliste**.
6.  Wählen Sie im Menü **Druck** eine der folgenden Möglichkeiten:
    *   **Bildschirm**: Die Liste wird auf dem Bildschirm dargestellt. Sie kann aus dieser Darstellung heraus ebenfalls an den Drucker gesendet werden.
    *   **Drucker**: Die Liste wird an den Standard-Drucker gesendet.

> **Weitere Listen drucken**
> Auf die gleiche Weise drucken Sie die Liste für die Empfangsbestätigungen und die auswärtigen Gestelle. Dazu wählen Sie in Schritt 5 die entsprechende Option.

#### Übungen

*   Legen Sie verschiedene Fahrzeuge an. Die zulässige Zuladung soll sich deutlich unterscheiden.
*   Ordnen Sie den Fahrzeugen so viele Aufträge zu, dass die Beladung gut ausgenutzt wird.
*   Was können Sie tun, wenn ein Auftrag mit keinem Ihrer Fahrzeuge ausgeliefert werden kann, weil das Gesamtgewicht der Positionen zu hoch ist? Setzen Sie Ihre Lösung um.

**Ergänzende Informationen**
*   ⇨ Stammdaten, "Tourrangfolge" auf Seite B-803
*   ⇨ Stammdaten, "Lieferdauer (Kunde, Lieferant)" auf Seite B-832
*   ⇨ Stammdaten, "Touren" auf Seite B-873
*   ⇨ Softwarereferenz, "Listendruck" auf Seite E-235

## Übersichten

In diesem Themenblock lernen Sie, wie Sie sich Übersichten über Ihre Termine und zu Kapazitäten erstellen.
Dazu gehören folgende Einheiten:
*   "Terminübersicht" auf Seite E-117
*   "Kapazitätsübersicht" auf Seite E-125

### Terminübersicht

**Lernziele**
*   Kriterien für die Prüfung des Materialbedarfs in einem bestimmten Zeitraum zusammenstellen.
*   Die Terminübersicht nach unterschiedlichen Kriterien erstellen und vergleichen.

**Nutzen**
*   Sie können sich einen Überblick über die benötigten Mengen verschaffen, die in einem bestimmten Zeitraum für die Produktion benötigt werden.
*   Damit können Sie feststellen, ob die Lagerbestände ausreichen, um die erfassten Aufträge termingerecht zu liefern.

**Merke**
*   **Auswahl von Merkmalen**: Die verschiedenen Kriterien, unter denen die Auswertung erstellt werden soll, hängt mit folgenden Einstellungen zusammen:
    *   Auswertungsmodus
    *   Auflösungstiefe
    *   Restriktionen
    Je nach den Einstellungen werden bestimmte Felder gesperrt oder freigeschaltet, um die Auswertung weiter einzugrenzen.
*   **Auswertungsmodus**: Mit der Wahl des Modus legen Sie fest, welche Produkte oder Produktgruppen betrachtet werden.
*   **Auflösungstiefe**: Mit der Wahl der Auflösungstiefe legen Sie fest, wie die gewählten Produkte gruppiert werden sollen.
*   **Restriktionen**: Mit der Wahl der Restriktionen legen Sie fest, auf welche Merkmale die Auswahl eingeschränkt werden soll.
*   **Voreinstellungen**: Keine

#### Materialbedarf pro Zeitraum

Sie können sich einen Überblick darüber verschaffen, welche Mengen in einem bestimmten Zeitraum zu fertigen oder zu liefern sind. Die Tiefe der Auswertung kann dabei bis auf die Auftragsebene und sogar auf die Positionsebene verfeinert werden.

In der Auswertung werden folgende Werte ausgewiesen:
*   Mengeneinheit
*   Summe der Mengeneinheit (bezogen auf die Haupt- oder die Stücklistenposition)
*   Gesamtmenge
*   Gesamtquadratmeter
*   Gesamtlaufmeter (immer bezogen auf die Hauptposition).

Zu jedem Auswahlkriterium werden Zwischensummen gebildet, welche wiederum eine Gesamtsumme ergeben.

Für die Auswertung wählen Sie aus, ob die Aufträge aus einem bestimmten Nummernverwalter oder der aktuelle Auftragsbestand unter bestimmten Kriterien betrachtet werden soll, z. B. nach dem Status. Folgende Auswertungsmodi stehen zur Verfügung: nach Produktionsbereich, nach Warengruppen oder nach Produkten.

#### Auswertungsmodus

Die Auswertung nach drei verschiedenen Modi erstellt werden:
*   **Produktionsbereich**: Innerhalb des Produktionsbereiches ist es möglich zwischen Isolierglas, VSG, ESG, EFG (Einfachglas), Zuschnitt und den ISO-Hilfsstoffen zu differenzieren. Wenn Sie z. B. den Produktionsbereich Zuschnitt ausgewählt haben, können Sie die Auswertung mit Hilfe der Restriktionen auf den Modellzuschnitt einschränken.
*   **Warengruppen**: Bei der Auswertung nach Warengruppen muss Folgendes beachtet werden: Einem Produkt können zwei unterschiedliche Warengruppen zugeordnet werden. Die eine gilt für die Preisberechnung, die andere für die Statistik. Sie müssen daher angeben, welche der beiden WGR-Bereiche zur Auswertung herangezogen werden soll. Bestehen Kombinationswarengruppen, kann auch auf dieser Ebene ausgewertet werden.
*   **Produkt**: Die Auswertung nach Produkt lässt eine Unterscheidung der Produktart und der Produktgruppe zu. Sie können die Auswertung auch auf eine Produktnummer einschränken.

> **Vergleichszeitraum anzeigen**
> Um sich den Verbrauch von Materialien in einem Vergleichszeitraum anzeigen lassen, können auch die archivierten Aufträge einbezogen werden. Dazu muss im Menü **Optionen** der Eintrag **Archiv** aktiviert werden.

#### Terminübersicht erstellen

In diesem Abschnitt lernen Sie, wie Sie sich im Dialog **Terminübersicht** anzeigen lassen, was in einem bestimmten Zeitraum produziert werden muss und welche Materialien dazu gebraucht werden.

> **Auswahl der Kriterien**
> Im Dialog Terminübersicht finden Sie eine Vielzahl von Kriterien, nach denen Sie sich den zukünftigen Verbrauch von Materialien anzeigen lassen können. In der folgenden Anleitung werden diese nicht alle im Einzelnen dargestellt. Sie werden aber auf Besonderheiten aufmerksam gemacht, die Ihnen eine andere Sicht erlauben.

**So erstellen Sie eine Übersicht über die benötigten Materialien**

1.  Wählen Sie im Menü **Fertigung > Terminübersicht > Terminübersicht**.
    
    *[Image of the 'Übersicht nach Materialien und Termin' dialog. Labels: A) Auswahl für Modus Produktionsbereiche, B) Auswertungsmodus, C) Restriktionen, D) Auswahl für Modus Warengruppen, E) Auswahl für Modus Produktion, F) Auflösungstiefe.]*
    
    ⇨ Softwarereferenz, "Terminübersicht (Dialog)" auf Seite E-270
2.  Wählen Sie den Nummernverwalter und ggf. den Mandanten und den AV-Bereich aus.
    Mit der Option **Nummer** und der Auftragsnummer können Sie sich einen Überblick über einen einzelnen Auftrag verschaffen.
3.  Wählen Sie den Auswertungsmodus (B) aus.
    Mit der Wahl des Modus werden unterschiedliche Felder für die weitere Auswahl von Kriterien freigeschaltet. In diesem Beispiel wird der Modus nach **Produktionsbereich** gewählt.
    Wenn Sie den Auswertungsmodus nach **Warengruppen** wählen, können Sie im Bereich **Auswahl Warengruppe (E)** eine Warengruppe (WGR), Warenobergruppe (WOG) oder Warenhauptgruppe (WHG) auswählen. Die Auswertung selbst zeigt jedoch immer nur die WHG.
    Die Warengruppen und ihre Hierarchie sind ausführlich im Part Stammdaten erklärt.
    ⇨ Stammdaten, "WGR" auf Seite B-575
    Wenn für Ihre Übersicht auch Warenhauptgruppen oder Warenobergruppen wichtig sind, können Sie zum Dialog **Kapazitätsübersicht** wechseln. Diesen Dialog lernen Sie in der nächsten Einheit kennen.
    ⇨ "Kapazitätsübersicht" auf Seite E-125
4.  Wählen Sie den Zeitraum aus, den Sie betrachten wollen.
    Wenn Sie in beiden Feldern dasselbe Datum eingeben, wird nur dieser eine Termin betrachtet.
5.  Wählen Sie die Auflösungstiefe.
    Die Einstellung betrifft die Darstellung der Daten in der Übersicht. Die Auflösungstiefe **pro Datum** ist z. B. sinnvoll, wenn Sie einen größeren Zeitraum betrachten wollen. In der Darstellung werden die Aufträge dann nach Datum in Gruppen zusammengestellt.
    Die Zwischensumme pro Mengeneinheit bezieht sich immer auf die Auflösungstiefe.
6.  Wählen Sie den Statusbereich der Aufträge aus, die berücksichtigt werden sollen.
    Wenn Sie eine weitsichtige Vorschau benötigen, sollten Sie z. B. als ersten Status **Dokument erfasst** wählen. Der zweite Status wird dann **Produktionsfreigabe** sein, denn diese Aufträge sind ja noch nicht abgeschlossen. Wenn Sie in beiden Feldern **Produktionsübergabe** wählen, erhalten Sie eine eher kurzfristige Übersicht.
    Wenn Sie eine Betrachtung der Vergangenheit benötigen, geben Sie das entsprechende Datum ein. Die Felder im Bereich **Auswertungszeitraum** werden freigeschaltet, wenn Sie im Bereich **Quelle** die Option **Nummer** wählen. Lassen Sie dann das Feld für die Auftragsnummer frei.
7.  Wählen Sie die Produktionsbereiche (A) und Restriktionen (C) aus, die angezeigt werden sollen.
    Die Einstellungen betreffen jeweils das Hauptprodukt. Wenn Sie z. B. das selbst zugeschnittene Float sehen wollen, müssen Sie die Option **Zuschnitt** markieren.
8.  Wählen Sie im Menü **Start > Ausführen**, um die Übersicht zu erstellen.
    
    *[Image of the results table for 'Terminübersicht nach Produktionsbereichen'.]*
    
    Die Auswertung wird im Register **Tabelle** den Auswahlkriterien entsprechend angezeigt. Wenn die Suche mit den gewählten Kriterien kein Ergebnis erzielt, wird eine Meldung angezeigt und das Register **Tabelle** enthält keine Daten.
    In der Druckversion wird die Übersicht auf dieselbe Art dargestellt.

#### Übungen

*   Lassen Sie sich für die Aufträge in Ihrem Übungs-NV anzeigen, welche Materialien Sie für die Produktion bis zum Ende des Quartals benötigen.
*   Ändern Sie nacheinander den Auswertungsmodus und die Auflösungstiefe und vergleichen Sie die Ergebnisse.

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Terminübersicht (Dialog)" auf Seite E-270

### Kapazitätsübersicht

**Lernziele**
*   Unterschiedliche Kriterien für die Auswertung festlegen.
*   Auswertung analysieren.

**Nutzen**
*   Sie können sich einen Überblick über die Produkte nach Warengruppen (WHG, WOG, WGR) verschaffen, die in einem bestimmten Zeitraum produziert werden sollen.
*   Damit können Sie bestimmen, ob die Produktionskapazitäten ausreichen, die erfassten Aufträge termingerecht zu liefern.

**Merke**
*   **Kapazitätsübersicht**: Diese Übersicht steht in keinem Zusammenhang mit der Kapazitätsplanung. Sie können keine Termine ändern oder die Produktionsreihenfolge bestimmen.
*   **Voreinstellungen**: Keine

#### Kapazitätsvorschau

Sie können sich einen groben Überblick darüber verschaffen, welche Produkte zu einem bestimmten Liefertermin fertig sein müssen.
Der Dialog **Kapazitätsübersicht** steht nicht in Verbindung mit der Produktion oder der Kapazitätsplanung. Die Auswertung zeigt die Mengen nach Warenhaupt-, Warenober- oder Warengruppen, nach Auftragsstatus und Liefertermin an.
Mit dieser einfachen Übersicht können Sie prüfen, ob die Warenbestände an Rohmaterial ausreichend sind und ob die geplanten Termine realistisch sind.

#### Kapazitätsvorschau zu einem Liefertermin erstellen

In diesem Abschnitt lernen Sie, wie Sie eine Übersicht über die Mengen erstellen, die zu einem bestimmten Termin geliefert werden müssen.

**So erstellen Sie eine Übersicht zu einem Liefertermin**

1.  Wählen Sie im Menü **Fertigung > Terminübersicht > Kapazitätsübersicht**.
    
    *[Image of the 'Kapazitätsübersicht nach Liefertermin' dialog. Label A points to 'Auflösungstiefe'. Label B points to 'Felder zur Auswahl der Warengruppen'.]*
    
    Eine Beschreibung des Dialogs finden Sie unter:
    ⇨ Softwarereferenz, "Kapazitätsübersicht" auf Seite E-278
2.  Wählen Sie die Auflösung (A).
    Wenn Sie z. B. sehen wollen, wie viel ISO produziert werden soll, wählen Sie nur die Warengruppen, in denen Sie das ISO organisiert haben.
3.  Deaktivieren Sie die Checkbox **alle**, wenn innerhalb der gewählten Auflösung nur nach bestimmten Warengruppen ausgewertet werden soll.
    Die Felder zur Auswahl der Warengruppen werden freigeschaltet und Sie können die Warengruppen auswählen.
4.  Markieren Sie die Checkbox **mit Stückl.**, wenn auch die Stücklisten ausgewertet werden sollen.
    Sie können damit z. B. einen Überblick über die Bearbeitungen erstellen.
5.  Wählen Sie den Statusbereich der Aufträge aus, z. B. von **Dokument erfasst** bis **Produktionsfreigabe**.
6.  Prüfen Sie den Liefertermin.
    Standardmäßig ist das aktuelle Tagesdatum angezeigt. Sie können es überschreiben.
7.  Wählen Sie im Menü **Start > Ausführen**, um die Übersicht zu erstellen.
    
    *[Image showing the results of the 'Kapazitätsübersicht nach Warengruppen pro Liefertermin'. Label A points to the sum per delivery date. Label B points to the total sum per product group.]*
    
    Die Summen der einzelnen Warengruppen (B) zeigen Ihnen an, was in dem angegebenen Zeitraum produziert werden muss.

#### Übungen

Erstellen Sie sich eine Übersicht über die geplante Produktion. Wählen Sie dazu folgende Kriterien:
*   14 Tage am Anfang des nächsten Quartals
*   Auflösung nach Warenhauptgruppen
*   Auswahl der Warenhauptgruppen 1 und 2
Ändern Sie die Kriterien und beobachten Sie, wie sich die Auswertung verhält.

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Kapazitätsübersicht" auf Seite E-278

## Zusatzfunktionen

In diesem Themenblock lernen Sie Zusatzfunktionen des Moduls **Fertigung** kennen.
Dazu gehören folgende Lerneinheiten:
*   "Produktionsaufträge" auf Seite E-130
*   "Frachtkosten" auf Seite E-139
*   "Warenausgang Kisten" auf Seite E-148

### Produktionsaufträge

**Lernziele**
*   Manuelle und automatische Rückmeldungen von Produktionsaufträgen kennenlernen.
*   Produktionsdaten erfassen und Lagerbestände durch Buchung aktualisieren.

**Nutzen**
*   Produktionsaufträge werden verwendet, um den eigenen Lagerbestand aufzufüllen. Dazu müssen die Rückmeldungen eingerichtet und die Bestände aktualisiert werden.

**Merke**
*   **Lagerzugang**: Der Lagerzugang aus Produktionsaufträgen kann manuell oder automatisch gebucht werden:
    *   Manuelle Statusumsetzung im Modul Fertigung.
    *   Automatische Status-Rückmeldungen aus der Produktion.
*   **Voreinstellungen**:
    *   Firmendaten:
        *   Register Parameter
        *   Register Lager/EK/EDI > Erfassungsstelle

#### Lagerartikel im Produktionsauftrag

Produktionsaufträge werden verwendet, um den eigenen Lagerbestand aufzufüllen. Alle Artikel, die in einem solchen Auftrag erfasst werden, müssen die Beschaffungsart **Produktion** haben. Im Gegensatz zu normalen (Kunden-) Aufträgen werden die Positionen nicht im Lager reserviert, sondern als **bestellt** markiert.

Produktionsaufträge können auf unterschiedliche Weise erfasst werden:
*   Manuelle Erfassung eines neuen Dokumentes vom Typ Produktionsauftrag.
*   Kopieren eines gespeicherten (Dummy-)Auftrags.
*   Automatische Erstellung durch Unterdeckung des Lagerbestands.

Aus der Produktion wird der Auftrag fertiggemeldet und die Bestandsdaten im Lager werden aktualisiert.
Die manuelle und automatische Erfassung von Produktionsaufträgen ist ausführlich im Part **Lagerwirtschaft** beschrieben. Darum werden die einzelnen Schritte hier nur als Zusammenfassung dargestellt.
⇨ Lagerwirtschaft, “Produktionsaufträge" auf Seite G-131

Im Part **Fertigung** werden die Produktionsaufträge an die Produktion übergeben. Die anschließende Rückmeldung aus der Produktion und die manuelle Erfassung der Produktionsdaten werden dagegen ausführlich dargestellt.

#### Rückmeldung zu Produktionsaufträgen

Der Lagerzugang aus einem Produktionsauftrag wird nicht durch einen Rechnungs- oder Lieferscheindruck gebucht. Die Buchung kann durch folgende Aktionen angestoßen werden:
*   Statusrückmeldung über den A+W Business Interface Service aus der Produktion stoßen die Buchung automatisch an.
*   Durch eine manuelle Buchung im Dialog Produktionsdaten.
    ⇨ "Produktionsauftrag fertigmelden" auf Seite E-134

**So ordnen Sie einen Statuspunkt der Erfassungsstelle für Rückmeldungen zu**

1.  Legen Sie in den Stammdaten eine Erfassungsstelle für die Rückmeldung an.
    Wie Sie Erfassungsstellen zuordnen, ist in der Einheit zu Produktionsrückmeldungen per Datei beschrieben.
    ⇨ "So ordnen Sie eine Erfassungsstelle für die Rückmeldung per Datei zu" auf Seite E-63
2.  Ordnen Sie dieser Erfassungsstelle ein Statuspunkt zu, ab dem die Ware als produziert gilt, z. B. wenn die erste Position fertig ist.
    
    *[Image showing the assignment of a status point to a data entry point.]*

3.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.
4.  Ordnen Sie nun die Erfassungsstelle in den Firmendaten im Register **Lager / EK / EDI** der Rückmeldung zu.
    ⇨ "Einstellungen in den Firmendaten festlegen" auf Seite E-133

#### Einstellungen in den Firmendaten festlegen

In den Firmendaten müssen Sie die Einstellungen für die Produktionsrückmeldung prüfen. Die URL des ERP-Webservice ist für Produktionsübergabe und Produktionsrückmeldung im OrderXML-Format gültig. Diese Einstellungen sind im Themenblock Produktionsübergabe ausführlich beschrieben.
⇨ "So prüfen Sie die Einstellungen in den Firmendaten" auf Seite E-32

**So ordnen Sie die Erfassungsstelle zu**

1.  Wählen Sie im Menü **Stammdaten > Firma > Firmendaten** und wechseln Sie zum Register **Lager / EK / EDI**.
    
    *[Image of the Company Data dialog, 'Lager/EK/EDI' tab, showing the setting for 'Auftrag produziert bei Erfassungsstelle'.]*

2.  Wählen Sie im Bereich **Auftrag produziert bei** die Erfassungsstelle aus.
    Sobald eine Position aus einem Produktionsauftrag eine Statusrückmeldung von dieser Erfassungsstelle erhält, wird die Position im Lager gebucht. Diese Statusmeldung kann auf folgende Arten eintreffen:
    *   Automatisch durch den A+W Business Interface Service.
    *   Manuell im Dialog Statusmeldung.
3.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.

#### Produktionsauftrag fertigmelden

Mit der Fertigmeldung eines Produktionsauftrags können die Lagerbestände aktualisiert werden. Die verwendeten Rohmaterialien und alle produktionsrelevanten Daten zu einem Produktionsauftrag werden zunächst erfasst.
Durch den anschließenden Buchungsvorgang werden die verwendeten Rohmaterialien vom Lager abgebucht und die Positionen des Produktionsauftrages werden dem Lager zugebucht.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So erfassten Sie die Produktionsdaten" auf Seite E-134
*   "So verbuchen Sie den Produktionsauftrag" auf Seite E-137

**So erfassten Sie die Produktionsdaten**

1.  Wählen Sie im Menü **Fertigung > Produktion > Produktionsdaten**.
    Der gleichnamige Dialog wird geöffnet.
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    
    *[Image showing the fields for entering production data, which are now active. Labels are: A) Production order number, B) Product number and description, C) Production details, D) Raw material consumption.]*
    
    ⇨ Softwarereferenz, "Produktionsdaten (Dialog)" auf Seite E-199
    
    Bis auf die Angabe eines Ausfallgrundes müssen alle Felder gefüllt werden.
3.  Tragen Sie im Bereich **Allgemein** das Datum ein, an dem der Produktionsauftrag gefertigt wurde, und füllen Sie die weiteren Felder des Bereichs mit den entsprechenden Angaben.
4.  Tragen Sie die Nummer des Produktionsauftrags (A) ein.
    Die Daten des Auftrags werden eingelesen.
5.  Wählen Sie die Nummer der Position aus, zu der Sie die Produktionsdaten erfassen wollen.
    Das Programm zeigt automatisch die Stückzahl und die Daten des Fertigproduktes (B) an, das in der Position erfasst wurde. Die folgenden Eingaben gelten jeweils nur für die ausgewählte Position.
6.  Tragen Sie die Anzahl der Einheiten ein, die zum angegebenen Datum gefertigt wurden.
7.  Wenn in der Position eine Kiste erfasst wurde, können Sie die ID automatisch vergeben lassen. Markieren Sie dazu die Checkbox **Identnummer automatisch vergeben**.
    Nur wenn die Kisten mit jeweils einer eigenen ID erfasst sind, kann ggf. der Kisteninhalt korrigiert oder die Kiste aufgelöst werde.
8.  Erfassen Sie im Bereich **Produktionsdetails (C)** die Zeiten, die für die Herstellung benötigt wurden, und die Anzahl der mit der Herstellung beschäftigten Mitarbeiter.
9.  Tragen Sie im Feld **Ausfallzeit (Minuten)** eine Null (0) ein, wenn Sie keine Ausfallzeiten erfassen müssen, ansonsten tragen Sie die Zeit ein, in der nicht produziert werden konnte.
    Über die Kombobox **Grund des Ausfalls** können Sie einen Grund eintragen, wenn die Produktion nicht in der geplanten Form abgelaufen ist. Wenn zuvor schon unterschiedliche Gründe eingetragen worden sind, können diese auch ausgewählt werden.
10. Tragen Sie im Bereich **Rohmaterial (D)** die Daten des Produkts ein, das für die Produktion der Position verbraucht wurde.
    Zusätzlich können Sie den Bruch von Rohmaterial angeben und den Lieferanten eintragen. Der Bruch von Rohmaterial sollte immer eingetragen werden, damit die entsprechenden Lagerbestände aktualisiert werden.
11. Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden im Register **Tabelle** in komprimierter Form aufgelistet.
    
    *[Image showing the list of positions for which data has been entered (A) but not yet posted, and a posted position (B) which is no longer in the list for posting.]*
    
    Im Register **Buchung** werden die Positionen aufgelistet, zu denen Daten erfasst wurden. Sie können diese Position jetzt im Register **Buchung** verbuchen oder im Register **Auftrag** weitere Daten erfassen.
12. Wiederholen Sie die Schritte 2 bis 11, bis Sie alle Daten erfasst haben, die Sie verbuchen wollen.
    Wenn Sie alle Daten erfasst haben, können Sie im Register **Buchung** die Verbuchung starten.

**So verbuchen Sie den Produktionsauftrag**

1.  Wechseln Sie zum Register **Buchung**.
    Die Fertigungsdaten sind pro Produktionsdatum und Aggregat verdichtet aufgelistet. Wenn Sie Daten zu verschiedenen Aggregaten erfasst haben, wird pro Aggregat eine Zeile aufgeführt.
    Bereits verbuchte Daten werden nicht mehr aufgeführt.
2.  Markieren Sie die Einträge, die Sie verbuchen wollen:
    *   Mit einem Doppelklick in eine Zeile markieren Sie einen einzelnen Eintrag.
    *   Mit einem Klick auf die Symbolschaltfläche **[Alle]** markieren Sie alle Einträge der Liste.
    
    *[Image showing the 'Buchung der Produktionsdaten' (Posting of Production Data) view.]*
    
    Nur die Positionen sind markiert, die mit einem x gekennzeichnet sind.
3.  Wählen Sie im Menü **Start > Speichern**, um die Verbuchung zu starten.
    *   Die Daten werden zunächst geprüft. Danach werden die betroffenen Produktionsaufträge für die Zeit der Verbuchung gesperrt.
    *   Die Lagerartikel aus den Produktionsaufträgen werden zugebucht. Bei Kisten werden ggf. neue Sub-Positionen angelegt, um jede Kiste mit einer ID zu verbuchen.
    *   Anschließend wird das Rohmaterial vom Lager abgebucht. Wenn der Produktionsauftrag vollständig gefertigt ist, wird der Status hochgesetzt und ein Eintrag in der Historie geschrieben.
    *   Schließlich werden die gesperrten Dokumente wieder freigegeben.
    
    Die verbuchten Datensätze werden aus der Anzeige gelöscht. Bei Positionen aus Produktionsaufträgen, die mindestens einen verbuchten Lagerartikel enthalten, kann in der Positionserfassung der Produktaufbau nicht mehr bearbeitet werden.

#### Übungen

*   Erfassen Sie einen Produktionsauftrag manuell und setzen Sie den Status manuell um auf **produziert**.
*   Verbuchen Sie die den Lagerzugang im Dialog **Produktionsdaten**.
*   Prüfen Sie den neuen Lagerbestand der Produkte und des Rohmaterials.

**Ergänzende Informationen**
*   ⇨ Stammdaten, “Übermengen" auf Seite B-859
*   ⇨ Stammdaten, "Firmendaten - Lager/EK/EDI" auf Seite B-970
*   ⇨ Stammdaten, "Firmendaten - Produktion" auf Seite B-1000
*   ⇨ Verkauf, "Neuer Auftrag durch Kopieren" auf Seite C-251
*   ⇨ Verkauf, "Dokument - Kopfdaten" auf Seite C-424
*   ⇨ Verkauf, "Lagerinfo" auf Seite C-758
*   ⇨ Softwarereferenz, “Produktionsdaten (Dialog)" auf Seite E-199

### Frachtkosten

**Lernziele**
*   Kalkulatorische Frachtkosten ermitteln und beurteilen.
*   Speditionskosten auf Kundenaufträge verteilen.

**Nutzen**
*   Ermittlung der kalkulatorischen Frachtkosten dient der Feststellung, ob sich eine Tour zu einem bestimmten Liefertermin überhaupt lohnt.
*   Speditionskosten für Touren, die nicht mit dem eigenen Fuhrpark gefahren werden, können auf die Kundenaufträge der jeweiligen Tour verteilt werden.

**Merke**
*   **Kalkulatorische Frachtkosten**: Touren mit hohen Frachtkosten in Bezug auf den Umsatz können aus einer Liste von Lieferterminen ermittelt werden.
*   **Entfernung und Kilometerpauschale**: Pro Tour wird eine Kilometerpauschale hinterlegt, die zusammen mit der Entfernung aus den Kundendaten zur Berechnung der Lieferkosten herangezogen wird.
*   **Sternförmige Berechnung**: Die kalkulatorischen Frachtkosten werden sternförmig berechnet: Es gilt jeweils die Entfernung zwischen dem Werk und dem einzelnen Kunden, auch wenn mehrere Kunden mit derselben Tour beliefert werden.
*   **Speditionskosten**: Die Speditionskosten werden anteilig auf alle Kundenaufträge eines Liefertermins derselben Tour im Verhältnis zur Entfernung und zur transportierten Glasfläche verteilt.
*   **Voreinstellungen**:
    *   Stammdaten:
        *   Touren > Frachtkosten
    *   Kundendaten:
        *   Register Produktion > Entfernung
    *   Firmendaten:
        *   Register Versand (Krit. Frachtkostengrenze)

#### Berechnungen

Zur Berechnung von Frachtkosten stehen zwei Funktionen zur Verfügung:
*   **Kalkulatorischer Frachtkosten**
    *   Berechnung und Druck in Form einer Liste
    *   Ermittlung der Frachtkosten auf der Basis von Lieferterminen, Kunden und Touren
    *   Überprüfung einer kritischen Frachtkostengrenze
*   **Verteilung von Speditionskosten auf Kundenaufträge**

> **Frachtkosten bei gesperrten Aufträgen**
> Durch einen anderen Mitarbeiter gesperrte Aufträge werden bei der Auswertung nicht berücksichtigt, ohne dass eine Fehlermeldung angezeigt wird. Das kann daher zu fehlerhaften Frachtkosten in den Aufträgen führen. Dies gilt sowohl für die Frachtkostenkalkulation als auch für die Speditionskostenverteilung.

#### Einstellungen zur Berechnung von kalkulatorischen Frachtkosten

Um die Frachtkosten berechnen zu können, müssen folgende Daten hinterlegt sein:
*   Frachtkosten pro Kilometer und Tour
*   Entfernung in Kilometer pro Kunde
*   Kritische Frachtkostengrenze

**So richten Sie die Voraussetzung zur Berechnung ein**

1.  Wählen Sie **Stammdaten > Versand > Touren**.
    
    *[Image showing the shipping tours dialog with the cost per kilometer (€/km) column highlighted.]*
    
2.  Tragen Sie in der Spalte **€/km** für jede Tour die Frachtkosten pro Kilometer ein.
    
    > **Tour für Spedition**
    > Wenn Sie Lieferungen auch mit einer Spedition versenden, richten Sie zusätzlich eine weitere Tour ein, z. B. mit der Bezeichnung **Spedition**. Hinterlegen Sie zu dieser Tour keine Frachtkosten.
    > Wie Sie eine neue Tour anlegen, ist in der Einheit Tourenplanung beschrieben:
    > ⇨ "So richten Sie eine neue Tour ein" auf Seite E-84
    
3.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
4.  Wählen Sie **Stammdaten > Marktpartner > Kunde > Kunden**.
5.  Tragen Sie bei jedem Kunden im Register **Produktion** die Entfernung in Kilometern ein.
    
    *[Image of customer master data showing the distance field.]*
    
6.  Schließen Sie die Partnerverwaltung, wenn Sie alle Daten geprüft und nachgetragen haben.
7.  Wählen Sie **Stammdaten > Firma > Firmendaten > Register Versand**.
8.  Tragen Sie im Bereich **Frachtkosten** die kritische Frachtkostengrenze in Prozent ein.
    
    *[Image of company data showing the critical freight cost limit field.]*
    
9.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Damit haben Sie die Voraussetzungen zur Berechnung der kalkulatorischen Frachtkosten erfüllt.

#### Darstellung der kalkulatorischen Frachtkosten

Durch die Berechnung der kalkulatorischen Frachtkosten wird ersichtlich, ob sich eine Tour zu einem bestimmten Liefertermin lohnt. In einer Übersicht können Sie Touren mit zu hohen Frachtkosten in Bezug auf den Umsatz identifizieren.

Über das Menü **Dokumente > Auftrag > Auswertungen > Kalkulatorische Frachtkosten** können Sie sich die Kostenverteilung anzeigen lassen.

*[Image showing the calculated freight costs for a tour on a specific delivery date. Labels point to: A) Subtotal per customer, B) Grand total for the date, C) Grand total for all tours on the date, D) Selected tour(s), E) Grand total for the tour.]*

Die Kosten werden sternförmig berechnet. Das bedeutet, dass immer die Entfernung zwischen dem Werk und dem einzelnen Kunden herangezogen wird.
Die kalkulatorischen Frachtkosten werden zunächst in der Auftragserfassung berechnet. Wenn ein Auftrag erfasst wird, werden die kalkulatorischen Frachtkosten des aktuellen Auftrags und aller Aufträge des Kunden, die den gleichen Liefertermin und dieselbe Tour haben, berechnet.

> **Beispiel**
> Ein Kunde wird mit Tour Regional à 0,68 €/km beliefert.
> Bei einer Entfernung von 10 km ergeben pro Liefertermin kalkulatorische Frachtkosten von 6,80 €.
> Verteilung der Frachtkosten anteilig bezogen auf tatsächliche Fläche je Auftrag:
> 2 Aufträge mit Gesamtfläche von 40 qm.
> Auftrag 200188 mit Gesamtfläche von 30 qm = 75%
> Auftrag 200189 mit Gesamtfläche von 10 qm = 25%
> Verteilung der kalkulatorischen Frachtkosten von 6,80 €:
> Auftrag 200188 = 5,10 € = 75%
> Auftrag 200189 = 1,70 € = 25%

Wenn Sie Frachtkosten hinterlegt haben, haben Sie die Möglichkeit, eine kritische Frachtkostengrenze als Prozentwert in den Firmendaten festzulegen.
Im Auftrag können Sie sich die Kalkulation über das Menü **Funktionen** anzeigen lassen. Während der Kalkulation kennzeichnet A+W Business die Frachtkosten, die diese kritische Frachtkostengrenze erreichen oder überschreiten durch rote Schrift.

*[Image comparison of calculated freight costs. A) Freight cost share of the order, B) Critical freight cost limit, C) Critical freight cost limit exceeded (shown in red).]*

#### Speditionskosten verteilen

Speditionskosten, die durch ein Speditionsunternehmen entstehen, können folgendermaßen auf mehrere Aufträge verteilt werden:
*   Verteilung von Speditionskosten auf Aufträge nach Liefertermin und Tour
*   Verteilung der gesamten Speditionskosten im Verhältnis zur Entfernung und zur transportierten Glasfläche

Zur Berechnung des Anteils wird die tatsächliche Glasfläche ohne Maßrundungen betrachtet.

**So verteilen Sie die Speditionskosten einer Tour**

1.  Wählen Sie **Dokumente > Auftrag > Auswertungen > Kalkulatorische Frachtkosten**.
    Der Dialog **Kalkulatorische Frachtkosten** wird geöffnet.
2.  Wechseln Sie zum Register **Speditionskosten**.
    
    *[Image of the 'Speditionskosten' tab. Labels are: A) Liefertermin, B) Tour ohne Frachtkosten, C) Speditionskosten für diese Tour.]*
    
3.  Tragen Sie den Liefertermin (A) ein:
    Sie müssen ein Datum in der Zukunft oder das aktuelle Tagesdatum eintragen.
4.  Wählen Sie die Tour (B) aus, z. B. **Spedition**.
    Zu dieser Tour dürfen keine Frachtkosten hinterlegt sein. Als Ergebnis werden alle Aufträge angezeigt, auf die der Liefertermin und die Tour zutreffen.
5.  Tragen Sie den Netto-Betrag der Speditionsrechnung (C) ein.
6.  Wählen Sie im Menü **Start > Ausführen**, um die Speditionskosten zu berechnen.
    
    *[Image showing the distribution of freight costs. Labels are: A) Tour ohne Frachtkosten, B) Glasfläche pro Auftrag, C) Anteil der Speditionskosten, D) Eingabe der Speditionskosten für diese Tour.]*
    
    Die eingetragenen Speditionskosten sind nach Entfernung und Glasfläche auf die Aufträge verteilt.
    Wenn Sie in der Liste Aufträge vermissen, so sind diese entweder durch einen anderen Mitarbeiter gesperrt, haben ein anderes Lieferdatum oder eine andere Tour.

#### Übungen

*   Tragen Sie in den Stammdaten die Frachtkosten bei zwei Touren ein, zu denen Sie Aufträge erfasst haben.
*   Tragen Sie in den Kundendaten die Entfernung ein.
*   Erfassen Sie ggf. neue Aufträge mit Kunden und Touren, zu denen Sie die Kosten und die Entfernung hinterlegt haben.
*   Prüfen Sie in der Auftragserfassung die kalkulatorischen Frachtkosten.
*   Verteilen Sie die Speditionskosten auf die Lieferung, die Sie in der Kommissionierung zusammengestellt haben.

**Ergänzende Informationen**
*   ⇨ Stammdaten, "Touren" auf Seite B-873
*   ⇨ Stammdaten, "Partnerverwaltung - Produktion" auf Seite B-796
*   ⇨ Stammdaten, "Firmendaten - Versand" auf Seite B-1008
*   ⇨ Verkauf, "Kalkulatorische Frachtkosten" auf Seite C-731

### Warenausgang Kisten

**Lernziele**
*   Varianten der Ausgangsbuchungen von Kisten verstehen.
*   Warenausgang von Kisten buchen.

**Nutzen**
*   Die tatsächlich im Lager vorhandenen Kisten werden einem Auftrag im Warenausgang zugewiesen und sind dann als reserviert gekennzeichnet.
*   Je nach betrieblichen Einstellungen werden die reservierten Kisten vor oder nach dem Druck des Lieferscheins aus dem Lagerbestand gebucht.

**Merke**
*   **Warenausgang buchen**: Kisten können vor oder nach dem Druck des Lieferscheins ausgebucht werden.
*   **Kisten dem Auftrag zuordnen**: Kisten können vor oder nach dem Druck des Lieferscheins zugeordnet und damit im Bestand reserviert werden.
*   **Lagerbestand**: Nur die Kisten können zugewiesen werden, die im Lagerbestand mit einer Kisten-ID erfasst sind.
*   **Voreinstellungen**:
    *   Firmendaten:
        *   Register Lager / EK / EDI > Lagerführungsmodus
        *   Register Parameter (Virtuelle Positionsnummern)

#### Kistenausbuchung

In der Regel werden Kisten mit dem Druck des Lieferscheins aus dem Lagerbestand ausgebucht. Statt des Lieferscheindrucks kann aber auch der Rechnungsdruck die Buchung auslösen.
Da der Erfasser eines Auftrags nicht weiß, welche Kiste tatsächlich ausgeliefert wird, erfasst er zunächst die Dummy-Kiste mit den gewünschten Maßen. Der Lagerbestand kann jedoch erst aktualisiert werden, wenn die tatsächlich im Lager stehende Kiste mit einer eigenen ID erfasst und ausgebucht wird.

> **Beispiel**
> Im Auftrag wird eine Dummy-Kiste (ohne ID) mit den gewünschten Maßen erfasst. Als Menge wird 3 angegeben. Damit werden drei Stück der Dummy-Kiste reserviert.

**Ausbuchung**

| vor Lieferscheindruck | nach Lieferscheindruck |
| :--- | :--- |
| Im Warenausgang werden die echten Kisten mit ID gescannt. | Der Lieferschein wird gedruckt. |
| Die Reservierung auf die Dummy-Kiste wird storniert. | Damit werden die reservierten Dummy-Kisten ausgebucht. |
| Die drei Kisten mit ID werden als reserviert gekennzeichnet. | Mit dem Warenausgang Kiste werden drei echte Kisten mit ID gescannt. |
| Der Lieferschein wird gedruckt. Mit dem Warenausgang werden die drei Kisten ausgebucht. | Die Reservierung der Dummy-Kisten wird storniert. |
| | Die drei Kisten werden ausgebucht. |
*Tab. E-2: Ausbuchung von Kisten vor oder nach Druck des Lieferscheins*

#### Kiste ausbuchen

In diesem Abschnitt lernen Sie, wie Sie Kisten für den Versand ausbuchen. Folgende Schritte sind i. d. R. vorausgegangen:
*   Im Kundenauftrag wurde z. B. das Produkt 1005 erfasst.
    
    *[Image showing product 1005 entered in an order.]*
    
*   Über [F1] im Dialog Lagerinfo wurde die Dummy-Kiste 1004, 400x500 ausgewählt.
    
    *[Image showing the selection of a dummy crate (without ID - A) and the resulting reservations (B).]*
    
*   Die Kiste wurde in den Auftrag übernommen und z. B. mit der Positionsmenge 3 gespeichert.
    
    *[Image showing the position quantity of 3 has been saved.]*
    
*   Im Lager wurden 3 zusätzliche Reservierungen auf die Dummy-Kiste gebucht.
    
    *[Image showing the reservations for the dummy crate have increased by 3.]*
    
*   Im Buchungsjournal (Lagerwirtschaft) ist die Positionsmenge als reserviert gekennzeichnet.
    
    *[Image of the booking journal showing the reserved position.]*

Als nächstes sollen Kisten mit ID zugewiesen und nach dem Druck des Lieferscheins ausgebucht werden.

**So buchen Sie den Warenausgang von Kisten**

1.  Wählen Sie im Menü **Fertigung > Lieferwesen > Warenausgang Kisten**.
    
    *[Image showing the initial dialog for 'Warenausgang-Kiste'.]*
    
2.  Wählen Sie die Option **nach Scanner**.
3.  Erfassen Sie den Barcode der Auftragsnummer und der Positionsnummer.
    Die Nummern werden in den Feldern **Dokument** angezeigt.
    Wenn Sie nicht mit einem Scanner arbeiten, wählen Sie die Option **nach Auftragsnummer** und geben die Nummer ein.
4.  Wählen Sie im Menü **Start > Ausführen**, um die Auftragsdaten einzulesen.
    Die Anzeige wechselt zum Register **Identnummern**.
    
    *[Image showing the order position with its sub-positions (crates).]*
    
    Jede Kiste wird in einer eigenen Zeile als virtuelle Position angezeigt. Die Felder in der Spalte **Identnummer** sind leer, da noch keine Kiste mit ID zugewiesen wurde.
5.  Scannen Sie die Kisten-ID der ersten Kiste, die reserviert werden soll.
    Wenn Sie nicht mit einem Scanner arbeiten, wählen Sie im Feld **Identnummer** eine der angezeigten IDs aus. Nur Kisten-IDs von Kisten des erfassten Typs werden angezeigt.
6.  Wählen Sie im Menü **Start > Ausführen**, um die Kiste zuzuordnen.
    Die ID wird der ersten virtuellen Position zugeordnet. Gleichzeitig erhält die Zeile eine virtuelle Positionsnummer. Die Markierung springt in die nächste Zeile.
    
    *[Image showing a sub-position with an assigned crate ID (B) and a virtual position number (A).]*
    
    Damit ist die Reservierung von der Dummy-Kiste gelöscht und stattdessen die zugewiesene Kiste mit ID reserviert. Die beiden anderen Kisten sind immer noch auf die Dummy-Kiste reserviert.
    
    Im Buchungsjournal wird dies ebenfalls angezeigt:
    
    *[Image of the booking journal showing the remaining dummy reservations (A) and the new virtual position with an assigned crate ID (B).]*
    
7.  Wiederholen Sie die Schritte 5 und 6, um weitere Kisten mit ID zuzuordnen.
    
    *[Image showing all crates fully assigned with IDs.]*
    
    Zu jeder Kiste wird eine fortlaufende virtuelle Positionsnummer angezeigt. Allen Positionen ist jetzt eine bestimmte, im Lager vorhandene, Kiste mit ID zugeordnet.
    
    Diese tatsächlichen Kisten sind damit im Lager reserviert, was Sie z. B. im Buchungsjournal prüfen können:
    
    *[Image of the booking journal showing the reserved real crates.]*
    
Die virtuellen Positionsnummern werden in den Auftrag zurückgeschrieben.
    
*[Image showing the sub-positions in the order.]*

Im Dialog **Lagerinfo** sind die drei Kisten als Reservierung gekennzeichnet. Damit ist für den Erfasser eines Auftrags deutlich, dass diese Kisten nicht in einen anderen Auftrag übernommen werden können. Die Reservierungen wurden von der Dummy-Kiste storniert.

*[Image of the stock info dialog showing the dummy crate reservation is gone (A), the real crate IDs were found in goods issue (B), and reservations are now on the real crates (C).]*

Je nach Einstellung werden die Kisten aus dem Bestand ausgebucht, wenn der Lieferschein oder die Rechnung gedruckt wird. Die ausgebuchten Kisten werden im Dialog **Lagerinfo** nicht mehr angezeigt.

*[Image showing the stock info after the crates have been booked out.]*

#### Übungen

*   Erfassen Sie einen Auftrag mit Kisten.
*   Prüfen Sie im Dialog Lagerinfo die Reservierung und den Bestand der Kiste.
*   Erfassen Sie den Warenausgang der Kisten und vergleichen Sie anschließend, wie sich der Lagerbestand geändert hat.

**Ergänzende Informationen**
*   ⇨ Stammdaten, "Firmendaten - Parameter" auf Seite B-948
*   ⇨ Stammdaten, "Fälligkeitsberechnung für Februar (28 oder 29 Tage)" auf Seite B-955
*   ⇨ Verkauf, "Lagerinfo" auf Seite C-758
*   ⇨ Softwarereferenz, "Warenausgang" auf Seite E-239

### Gestellverwaltung

Mit A+W Business können Sie sowohl eigene als auch Fremdgestelle verwalten. Übersichten zeigen den aktuellen Bestand inkl. Außer-Haus-Gestellen und deren Rückgabetermin an.

**L-Gestellbelegung**
Die Zusatzfunktion L-Gestellbelegung wird pro Kunde aktiviert. Außerdem können dazu eigene Zuschläge für L-Gestelle berechnet werden.
Bei der Nutzung der Funktion muss für den jeweiligen Kunden die Bock- und Fachnummer ermittelt werden. Hierzu werden die entsprechenden Auftragsnummern in einem Nummernverwalter zusammengestellt.
Eine Position kann über mehrere L-Gestelle verteilt werden. Dabei müssen die Restriktionen für L-Gestelle beachtet werden.
Das Programm ermittelt pro Position jeweils die Start- und Endenummer.

> **Beispiel**
> 0101 = Gestell 1, Fach 1
> 0315 = Gestell 3, Fach 15

Das Ergebnis wird in der Übergabe-Datei in das Feld Kommission geschrieben. Hierzu werden die Start- und Endenummer dem Kommissionsfeld vorangestellt:
`0101-0421 + Kommissionsfeld aus Auftrag` (bis maximale Feldlänge).
Für die Aufträge werden dann Etiketten gedruckt und eine Liste der L-Gestellbelegung pro Auftrag. Die Information, ob eine Position auf einem L-Gestell verpackt werden kann, wird auch an den Formulardruck übergeben.
Außerdem werden die Daten in einer ASCII Datei gespeichert. Der Name der ASCII-Datei besteht aus der Kundennummer, Tag und Monat.

Für TPS und nicht TPS Positionen gibt es unterschiedliche Restriktionsprüfungen. Welcher Artikel zur Prüfung zu verwenden ist, ergibt sich aus der Zuordnung zu dem Abstandhalterartikel.
Geprüft wird:
*   **TPS**
    *   Maximales Maß 1100 x 1700
    *   Max. Einbaustärke 26 mm
    *   Anzahl Fächer: 22
*   **Nicht TPS**
    *   Maximales Maß 1080 x 1960
    *   Max. Einbaustärke 99 mm
    *   Anzahl Fächer: 21

Im Falle einer Restriktionsverletzung, wird der Text SEPA/ + Kommission übergeben. Falls eine Position nicht auf L-Gestell verpackt werden kann, wird kein Datensatz geschrieben.

#### Gestellverwaltung

Zur A+W Business-Gestellverwaltung gehört die Verwaltung der Gestelle nach Typ und Nummer. Sie definieren pro Gestell dessen Eigenschaften, z. B. verfügbar, gesperrt, verloren, stationär, Fremdgestell, Anzahl Latten, Räder. Für das Mahnwesen legen Sie den Mietsatz und die Anzahl an kostenfreien Tagen fest.
Wird ein Gestell an einen Kunden ausgeliefert, tragen Sie in der Ausgangsbuchung das Ausgangsdatum, die Nummer des Lieferscheins und die Kundennummer ein. Die Rückkehr des Gestells buchen Sie über das Eingangsdatum. Das Gestell ist somit wieder für die Auslieferung verfügbar.

Mit Hilfe des Mahnwesens können Sie alle auswärtigen Gestelle anmahnen. Sie geben an, wie viel Tage das Gestell mindestens auswärtig sein muss, um die Auswahl für die Mahnung einzugrenzen. Sie erhalten dann automatisch eine Liste aller anzumahnenden Kunden. A+W Business kann unterschiedliche Mahnstufen unterscheiden.

#### Fremdgestelle

Neben den eigenen Gestellen können Sie auch die Gestelle von Kunden und Lieferanten verwalten, die Ihnen zur Verfügung stehen.
Daneben können Sie in der Kundenkommission Details zu Standorten oder Abladeorten von (regelmäßigen) Lieferungen hinterlegen.

#### BDE Gestellrückmeldung

Ihre mit Barcode-Etiketten versehenen Gestelle werden vor dem Versand bzw. nach ihrer Rückkehr per Barcode-Scanner erfasst. Diese Daten werden in A+W Business eingelesen und entsprechend verbucht. A+W Business verfügt dadurch immer über aktuelle Informationen, welche Gestelle wieder für den Versand zur Verfügung stehen und welche sich noch beim Kunden befinden.

#### Gestellhistorie

Die Belegung eines Gestells wird in der Historie festgehalten, sodass Sie zurückverfolgen können, wann ein Gestell an wen ausgeliefert und zurückgemeldet wurde.
In der Gestellverwaltung können Sie Ihre Gestelle nach Gestellart und Gestellnummer organisieren. Versand und Erhalt der Gestelle dokumentieren Sie über die Ein-/Ausgangsbuchungen.

### Fertigungsvorschau

Der Dialog Fertigungsvorschau zeigt pro Liefertermin zu den Produktarten Isolierglas, Einfachglas, ESG und VSG die Summe der entsprechenden Aufträge an. Dazu werden alle Aufträge mit Liefertermin größer gleich dem aktuellen Tagesdatum ausgewertet.

Pro Liefertermin stehen 50 Spalten zur Verfügung, die individuell eingestellt werden können. Die Festlegung welcher Inhalt in welcher Spalte angezeigt werden soll, wird firmenübergreifend durch den Systemadministrator festgelegt. Die Auswertungskriterien sind jeweils eine Kombination von Produktart und Produktgruppe. Das Ergebnis kann sowohl in Stück als auch in qm dargestellt werden.

Die sichtbaren Spalten können für jede Produktart und für extra Zuordnungen pro Arbeitsplatz eingestellt werden. Auch die Spaltenbreite lässt sich pro Arbeitsplatz individuell einstellen.

#### Prinzip der Vorschauspalten

In der Kombination der Spalten Typ HP und Typ 0 können folgende Kombinationen definiert werden:

| Kombination | Beispiel |
| :--- | :--- |
| Produktart/Produktart | Isolierglas/Isolierglas |
| Produktart/Produktgruppe | Einfachglas/Ornament |

Mit der Kombination der Spalten Typ 0 und Nr. 0 kann das Hauptprodukt auch in der Stückliste gesucht werden.
Mit der Kombination der Spalten Typ 1 und Nr. 1 wird auf der Stücklistenebene gesucht.

| Spalte | Kombination |
| :--- | :--- |
| Typ 1 | Typauswahl auf Basis 1. Stücklistenebene |
| Nr. 1 | Produktart/Produktgruppe je nach Typ |

Mit der Kombination der Spalten Typ 2 und Nr. 2 wird nach einem Produkt oder einer Bearbeitung in der Stückliste gesucht, z. B. in VSG nach ESG oder Einfachglas, Ornament, Modell usw.

| Spalte | Kombination |
| :--- | :--- |
| Typ 2 | Typauswahl auf Basis 2. Stücklistenebene |
| Nr. 2 | Produktart/Produktgruppe je nach Typ |

**Beispiel: Konfiguration für Auswertung von Einfachglas**

*[Image of the 'Vorschauspalten Definition' dialog for single glass. Labels are: A) Typ HP, B) HP, C) ST/QM, D) Typ 0, E) Nr 0, F) Typ 1, G) Nr 1.]*

*   In Zeile 30 ist die Selektion so gewählt, dass alle Einfachgläser ohne weitere Einschränkung angezeigt werden.
*   Die Definitionen in Zeile 30 und 31 unterscheiden sich nur in der ausgewählten Maßeinheit für die Anzeige (qm bzw. Stück).
*   In Zeile 32 und 33 wird die Selektion von Einfachglas auf ausschließlich Ornamente eingegrenzt und keine weiteren Veredelungen berücksichtigt.
*   In Zeile 33 und 34 liegt der Schwerpunkt der Analyse auf der Bearbeitung und in Zeile 35 und 36 auf der Modellinformation.

Als Ergebnis der beschriebenen Einstellung werden in der Auswertung die Einfachgläser pro Datum angezeigt.

*[Image of the 'Fertigungsvorschau für Einfachglas' showing results per date.]*

## Softwarereferenz

### Übersicht

Im Modul **Fertigung** können Sie die Aufträge an die Produktion übergeben und den Versand steuern und überwachen.

In der Softwarereferenz finden Sie Informationen zu folgenden Themen:
*   "Produktion" auf Seite E-169
*   "Barcode-Übergabe" auf Seite E-194
*   "Produktionsdaten" auf Seite E-199
*   "Lieferwesen" auf Seite E-204
*   "Tourenliste" auf Seite E-205
*   "Statusmeldung" auf Seite E-218
*   "Kommissionierung" auf Seite E-228
*   "Listendruck" auf Seite E-235
*   "Warenausgang Kisten" auf Seite E-239
*   "Gestellverwaltung" auf Seite E-255
*   "Gestelle" auf Seite E-240
*   "Terminübersicht" auf Seite E-269
*   "Zollverwaltung" auf Seite E-284
*   "Angebotsoptimierung" auf Seite E-292
*   "Versandsteuerung" auf Seite E-292

Im Modul **Fertigung** werden auch die Dialoge zur Kapazitätsplanung angezeigt. Diese Dialoge werden im Part Kapazitätsplanung beschrieben.

> **Dialoge können von unterschiedlichen Stellen aus geöffnet werden**
> Bitte beachten Sie, dass einige Dialoge und Funktionen zum Modul Fertigung in A+W Business aus unterschiedlichen Modulen heraus gestartet werden können. In dieser Anleitung werden sie jedoch nur einmal beschrieben. Sie finden an den entsprechenden Stellen aktive Querverweise, über die Sie direkt zu der zugehörigen Beschreibung springen können.

**Nummernverwalter**
*   Fertigung > Produktion > Nummernverwalter
*   Fertigung > Lieferwesen > Nummernverwalter
*   Fertigung > Terminübersicht > Nummernverwalter
*   Fertigung > Zollverwaltung > Nummernverwalter
*   Fertigung > Angebotsoptimierung > Nummernverwalter

Der Dialog Nummernverwalter ist im Part Verkauf beschrieben.
⇨ Verkauf, "Nummernverwalter" auf Seite C-645

**Formular-/Etikettendruck**
*   Fertigung > Produktion > Formular
*   Fertigung > Lieferwesen > Formular
*   Fertigung > Zollverwaltung > Formular

Der Dialog Formular-/Etikettendruck ist im Part Verkauf beschrieben.
⇨ Verkauf, "Formular-/Etikettendruck" auf Seite C-655

**Dokumentendaten**
*   Fertigung > Dokumentendaten

Der Dialog Dokumentendaten ist im Part Verkauf beschrieben.
⇨ Verkauf, "Dokumentendaten" auf Seite C-754

**Artikel-Info**
*   Fertigung > Artikel-Info

Der Dialog Artikelinfo ist Part Verkauf beschrieben.
⇨ Verkauf, "Artikel-Informationen" auf Seite C-616

**Faxnachricht**
*   Fertigung > Faxnachricht

Der Dialog Faxnachricht ist im Part Überblick beschrieben.
⇨ Überblick, “Standard-Menüs" auf Seite A-53

### Produktion

**Fertigung > Produktion**
Produktionsaufträge können automatisch oder manuell an die Produktion übergeben werden. In der Regel werden die Aufträge in einen Nummernverwalter gestellt und im Dialog **Produktionsübergabe** an die Produktion übergeben. Sie können jedoch auch einzeln gescannt und per Barcode übergeben werden.

> **Automatische Übergabe**
> Die automatische Produktionsübergabe und das Abfrage-Intervall müssen in einem Workflow-Task als Formel eingerichtet sein.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Übergabe Produktion" auf Seite E-170
*   "Einstellungen Produktionsübergabe" auf Seite E-174
*   "Modellliste" auf Seite E-188
*   "Gestellbelegung prüfen" auf Seite E-189
*   "Einstellungen (Gestellbelegung prüfen)" auf Seite E-191
*   "Produktionsdaten (Dialog)" auf Seite E-199

**Ergänzende Informationen**
*   ⇨ “Barcode-Übergabe" auf Seite E-194
*   ⇨ "Produktionsdaten" auf Seite E-199

#### Übergabe Produktion

**Fertigung > Produktion > Übergabe Produktion**

*[Image of the 'Übergabe Produktion' dialog.]*

In diesem Dialog übergeben Sie die Aufträge aus einem Nummernverwalter an die Produktion. Die Übergabe starten Sie mit [OK]. Die Daten werden in eine XML-Datei geschrieben, die von A+W Production eingelesen werden kann.

Für die automatische Produktionsübergabe und den Abfrage-Intervall müssen Sie einen Workflow-Task einrichten. Eine Beschreibung dazu finden Sie im Tutorial.
⇨ Tutorial, "Produktionsübergabe mit A+W Business Kapazitätsplanung" auf Seite E-43

> **Übergabe von Angeboten**
> Angebote können über **Fertigung > Angebotsoptimierung > Übergabe Produktion** zur Optimierung an die Produktion übergeben werden. Der Dialog unterscheidet sich nicht von demjenigen für die Übergabe der Aufträge. Allerdings müssen die Einstellungen für die Übergabe von Angeboten getrennt eingerichtet werden.
