---
description: "D-AWBusiness-HB_22"
---


# Tutorial

---
## Lieferungen im Wareneingang

### Einstellungen für Identnummern prüfen

Wenn Sie die Kisten mit einer eigenen Kisten-ID erfassen wollen, können Sie diese ID automatisch vergeben lassen. Dazu müssen Sie die Einstellungen festlegen. Diese Einstellungen können vor jedem Wareneingang für Kisten angepasst werden, z. B. um die ID um ein Kennzeichen für den Lieferanten zu ergänzen.

Sie können maximal 20 Zeichen verwenden, die automatisch durch eine 5-stellige Zahl ergänzt werden. Die eingegebene Zeichenfolge bleibt so lange bestehen, bis sie manuell geändert wird. Wenn Sie also die Kisten-ID mit einem Kennzeichen für den Lieferanten versehen, müssen Sie darauf achten, die ID zu ändern, wenn Sie den Wareneingang von Kisten eines anderen Lieferanten erfassen.

**So prüfen Sie die Einstellungen für die automatische Vergabe von Identnummern**

1.  Wählen Sie `Dokumente > Bestellung > Wareneingang > Wareneingang`.
    Der Dialog `Wareneingang` wird geöffnet.

2.  Wählen Sie im Menü `Optionen > Gruppe Identnummernvergabe > Einstellungen`.

    [Image: Screenshot of the 'Einstellungen' dialog box for warehouse ID numbers.]
    **Einstellungen**
    Lageridentnummer
    Vorgabe: AUTOXXXXXX
    Beispiel: 'NRXXXXXXX' oder 'AUTOXXXXX'
    Die X (min. 5) müssen am Ende stehen und werden durch fortlaufende Zahlen ausgetauscht. Max. dürfen 20 Zeichen verwendet werden.
    [Ok] [Ende]

    ⇨ Softwarereferenz, "Einstellungen (ID)" auf Seite D-240

3.  Tragen Sie das Kennzeichen ein.
    Achten Sie darauf, dass Sie die Platzhalter (X) für die Ziffern nicht überschreiben.

4.  Klicken Sie auf `[OK]`, um die Änderung zu speichern.
    Der Dialog wird geschlossen. Die Einstellungen werden gespeichert und bleiben erhalten, bis sie erneut manuell geändert werden.

5.  Wählen Sie im Menü `Optionen > Gruppe Identnummernvergabe > Automatische Vergabe`.
    Damit ist die automatische Vergabe der ID für Kisten eingerichtet.

### Wareneingang von Kisten erfassen

Bei der Erfassung des Wareneingangs von Kisten, wird pro Kiste eine Kisten-ID vergeben. Anschließend werden die zugehörigen Etiketten gedruckt.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:

*   "So erfassen Sie den Wareneingang einer Kiste mit einer automatischen ID" auf Seite D-138
*   "So vergeben Sie Kisten-IDs manuell" auf Seite D-141
*   "So drucken Sie Kistenetiketten" auf Seite D-142

**So erfassen Sie den Wareneingang einer Kiste mit einer automatischen ID**

1.  Wählen Sie `Dokumente > Bestellung > Wareneingang > Wareneingang`.

    [Image: Screenshot of the Wareneingang dialog, tab '1.Auswahl'.]
    *   **A**: Suchoption
    *   **B**: Bestellnummer
    **Abb. D-85**: Wareneingang für Kisten – nach Nummernverwalter

    ⇨ Softwarereferenz, "Wareneingang (Dialog)" auf Seite D-227

    Stellen Sie sicher, dass die automatische Vergabe für Kisten-IDs aktiviert ist.

2.  Wählen Sie die Option (A), mit der Sie die Suche nach offenen Bestellungen starten möchten, z. B. nach `Bestellnummer`.

3.  Geben Sie die Bestellnummer (B) ein.

4.  Wählen Sie im Menü `Start > Ausführen`, um die Daten einzulesen.

Die Anzeige wechselt zum Register `Komplett`. Sie können die Daten nochmals prüfen.

5.  Wechseln Sie zum Register `Identnummern`.

    [Image: Screenshot of the Wareneingang dialog, tab '4.Identnummern'.]
    *   **A**: Ausgewählte Bestellung
    *   **B**: Eingabe der Kisten-ID des Lieferanten
    *   **C**: Lagerort
    *   **D**: Pro Kiste eine Zeile (Unterposition)
    **Abb. D-86**: Wareneingang für Kisten – Eingang erfassen

    Wenn die Stückzahl der bestellten Position größer als 1 ist, wird in der Übersicht `Kistenpositionen` für jede Kiste eine Zeile angezeigt.

    Sie können mehrere Kisten auf einmal auswählen, um diese in einem Schritt zu buchen.

6.  Markieren Sie eine Zeile, in der noch keine virtuelle Positionsnummer angezeigt ist.

7.  Geben Sie im Feld `Lieferanten-Identnummer` (B) die Kisten-ID des Lieferanten ein oder scannen Sie die Kisten-ID und springen Sie mit `<Tab>` in das nächste Feld.
    Wenn mehr als eine Kiste ausgewählt ist und die Lieferanten-Identnummer eingegeben ist, berechnet das System die Kisten-Identnummern für alle markierte Einträge.

8.  Wählen Sie den Lagerort aus und prüfen und korrigieren ggf. den Inhalt und den Preis.

    [Image: Screenshot showing the supplier's crate ID entered for a marked line.]
    *   **A**: Kisten-ID des Lieferanten
    *   **B**: Wareneingang für diese Kiste buchen
    **Abb. D-87**: Wareneingang für Kisten – Daten für markierte Zeile

    Die Eingaben werden in die markierte Zeile übernommen.

9.  Wählen Sie im Menü `Start > Ausführen`, um die Eingaben zu bestätigen und den Wareneingang zu buchen.

    [Image: Screenshot showing the booked crate with a new virtual position number.]
    *   **A**: Virtuelle Positionsnummer (verbuchte Unterposition)
    *   **B**: (Automatische) Kisten-ID
    **Abb. D-88**: Wareneingang für Kisten – neue virtuelle Positionsnummer erzeugt

    Die Kiste wird verbucht und mit der nächsten virtuellen Positionsunternummer an das Ende der Liste `Kistenpositionen` verschoben.

10. Wiederholen Sie die Schritte 7 bis 9, bis Sie den gesamten Wareneingang erfasst haben.
    Wenn Sie alle Kisten erfasst haben, können Sie den Druck der Kistenetiketten und des Protokolls starten.
    ⇨ "So drucken Sie Kistenetiketten" auf Seite D-142

**So vergeben Sie Kisten-IDs manuell**

1.  Wählen Sie `Dokumente > Bestellung > Wareneingang > Wareneingang`.
2.  Deaktivieren Sie im Menü `Optionen > Gruppe Identnummernvergabe > Automatische Vergabe`.
3.  Bereiten Sie die Erfassung des Wareneingangs vor, wie in den Schritten 2 bis 7 der vorhergehenden Handlungssequenz gezeigt.

    [Image: Screenshot of the Wareneingang dialog ready for manual ID entry.]
    *   **A**: Ausgewählte Bestellung
    *   **B**: Kisten-ID des Lieferanten
    *   **C**: Manuelle Kisten-ID
    *   **D**: Pro Kiste eine Zeile (Unterposition)
    **Abb. D-89**: Wareneingang für Kisten – Eingang erfassen

    Wenn die Stückzahl der bestellten Position größer als 1 ist, wird in der Übersicht Kistenpositionen für jede Kiste eine Zeile angezeigt.

4.  Geben Sie die Kisten-ID (C) ein, mit der die Kiste in Ihrem Lager verbucht werden soll.
    Sie können die ID des Lieferanten übernehmen, indem Sie den Cursor in das Feld stellen und Lieferanten-ID erneut scannen.

5.  Wählen Sie den Lagerort aus und prüfen und korrigieren ggf. den Inhalt und den Preis.
    Diese Eingaben gelten nur für die Kistenposition, die in der Übersicht markiert ist.

6.  Wählen Sie im Menü `Start > Ausführen`, um die Eingaben zu bestätigen.
    Die Kiste wird verbucht und mit der nächsten virtuellen Positionsunternummer an das Ende der Liste `Kistenpositionen` verschoben.

7.  Wiederholen Sie die Schritte 4 bis 6, bis Sie den gesamten Wareneingang erfasst haben.
    Wenn Sie alle Kisten erfasst haben, können Sie den Druck der Kistenetiketten starten, um die Etiketten mit den manuell vergebenen IDs zu drucken.

**So drucken Sie Kistenetiketten**

1.  Nachdem Sie die Kisten einer Lieferung erfasst haben, wählen Sie im Menü `Druck > Gruppe Drucker > Etiketten`.
    Wenn Sie den Eintrag `Etiketten und Protokoll` wählen, wird zusätzlich das Protokoll gedruckt, das Sie sich auch im Register `Protokoll (Identnummern)` anzeigen lassen können.

    [Image: Screenshot of the 'Druck - Kistenetiketten' dialog.]
    *   **A**: Anzahl
    *   **B**: Drucker
    **Abb. D-90**: Kistenetiketten drucken

2.  Wählen Sie den Drucker (B) und die Anzahl (A) der erforderlichen Kopien.

3.  Klicken Sie auf `[OK]`, um den Druck zu starten.
    Der Dialog wird geschlossen und die Etiketten werden gedruckt. Im Protokoll werden alle verbuchten Kisten mit den Kisten-IDs aufgeführt.

**Ergänzende Informationen**
⇨ Stammdaten, "Fälligkeitsberechnung für Februar (28 oder 29 Tage)" auf Seite B-955
⇨ Softwarereferenz, "Einstellungen (ID)" auf Seite D-240

## Preis- und Rechnungskontrolle

### Lernziele
*   Auftragsbestätigung des Lieferanten erfassen.
*   Preise prüfen.
*   Gesammelte Auftragsbestätigung zu mehreren Bestellungen erfassen.

### Nutzen
*   Zusammen mit der Auftragsbestätigung können die Preise geprüft werden.
*   Preise mehrerer Bestellungen können in einer gemeinsamen Auftragsbestätigung geprüft werden.

### Merke

*   **Status**: Nach der Preis- und nach der Rechnungskontrolle wird der Status der Dokumente hochgesetzt. In Verbindung mit einem Sperrstatus ist eine erneute Preis- und/oder Rechnungskontrolle daher nicht möglich.
*   **Differenzen**: Sie können die Preis- oder Rechnungskontrolle nur dann abschließen, wenn keine Differenz zwischen dem eingegebenen Gesamtbetrag und der Summe der angezeigten Bestellungen besteht.
*   **Schnellerfassung**: Wenn Sie im Menü `Optionen > Schnellerfassung` aktivieren, springt der Cursor nach der Eingabe der Bestellnummer direkt in das Feld `Rechnungssumme` bzw. `AB-Summe`. Sie können diese Option dann nutzen, wenn Sie in der Regel nur eine Bestellnummer eintragen.
*   **Dokumentensperre**: Während der Preis- und Rechnungsprüfung sind die referenzierten Dokumente für den Zugriff durch andere Mitarbeiter gesperrt.
*   **Firmendaten**:
    *   Register Steuer
    *   Register Preisberechnung
    *   Register Druck
    *   Register Lager/EK/EDI

### Eingangsrechnung

Die Preise können sowohl auf Basis der Auftragsbestätigung des Lieferanten als auch auf Basis der Lieferantenrechnung geprüft werden. Die Dialoge `Preiskontrolle` und `Rechnungskontrolle` sind identisch aufgebaut. In beiden Dialogen können Sie die Preise korrigieren und Ihre Einkaufspreise (EK) in den Dokumenten aktualisieren.

Während der Preis-/Rechnungskontrolle ist die zugehörige Bestellung für den Zugriff durch andere Benutzer gesperrt. Um die Bestellung während der Preis- bzw. Rechnungskontrolle anpassen zu können, kann das Dokument direkt geöffnet werden. So können Sie z. B. fehlende Zuschläge erfassen, ohne die Preis- und Rechnungskontrolle zu verlassen.

Die Prüfungen von Preisen und Rechnungen können auch in elektronisch ausgetauschten Dokumenten durchgeführt werden. Diese Funktionalität ist im Themenblock `Elektronischer Dokumentenaustausch` beschrieben:
⇨ "Export/Import (openTRANS)" auf Seite D-151

### Preiskorrekturen

Sie können die Preis- oder Rechnungskontrolle nur dann abschließen, wenn keine Differenz zwischen dem eingegebenen Gesamtbetrag und der Summe der angezeigten Bestellungen besteht. Eine solche Differenz kann z. B. durch unterschiedliche Preise, nicht erfasste Zuschläge oder durch Fehleingaben entstehen.

Wenn der eingegebene Betrag nicht mit der Bestellung oder der Summe der Bestellungen übereinstimmt, müssen Sie die Preise in den Positionen oder in den Stücklisten korrigieren – oder die AB/Rechnung zur Korrektur zurückschicken.

Nach der Rechnungskontrolle werden die Bestellungen mit dem entsprechenden Status versehen und sind damit zur Anweisung und zur Übergabe an die FiBu bereit.

Nach der Prüfung, Korrektur und Bestätigung der Preise wird der Status der Bestellung umgesetzt.
⇨ "Dokumentenstatus" auf Seite D-40

### EK-Preise im Auftrag

Der EK eines referenzierten Auftrags kann nur so lange aktualisiert werden, wie der Sperrstatus dies zulässt. Nach der Rechnungskontrolle wird der Status der Bestellung hochgesetzt. Die Preis- oder Rechnungskontrolle kann dann nicht nochmals durchgeführt werden.

### Fußzuschläge und Fußrabatte

Die Fußzuschläge/-rabatte einer Bestellung, z. B. ein Energiezuschlag, werden in die Kosten des Auftrags zurückgeschrieben. Die Fußzuschläge/-rabatte werden positionsgenau zurückgerechnet und in der Dokumentenverwaltung angezeigt. Damit ist auch bei bestellten Produkten der Deckungsbeitrag immer aktuell, der in der Positionserfassung angezeigt wird.

Optional kann bei der Rechnungskontrolle automatisch die Position Anlieferpauschale pro Bestellung angefügt werden. Damit entfällt die manuelle Nacherfassung in der Bestellung.

### Fremdwährung

Wenn Sie mit mehreren Währungen arbeiten, können Sie die Preise und Rechnungen in einer Fremdwährung bestätigen. Die Preise der Bestellpositionen werden in der Landeswährung gespeichert. Die Einkaufspreise werden unter Berücksichtigung der Währungsumrechnung aktualisiert.

### Sammel-AB und Sammelrechnung

Wenn Ihr Lieferant mehrere Bestellungen gesammelt in einer AB oder Rechnung aufgeführt hat, kann diese nur geprüft und akzeptiert werden, wenn in allen Bestellungen derselbe MwSt-Satz und dieselbe Währung angegeben sind.

Wenn einer Ihrer Lieferanten in der Regel Sammelrechnungen erstellt, kann es sinnvoll sein, für diesen Lieferanten einen eigenen Nummernverwalter für die Bestellungen einzurichten.

### EK-Rückschreibung

Der EK wird in die referenzierten Aufträge zurückgeschrieben, wenn er bei der Preis- oder Rechnungskontrolle und/oder beim Buchen des Wareneingangs geändert wurde. Diese angepassten Einkaufspreise werden zur Kalkulation des Deckungsbeitrags und bei der Lagerbewertung oder bei Lagerbestellungen herangezogen.

Dazu müssen in den Firmendaten die Option zur Ermittlung der Einkaufspreise aktiviert und die Preistabellen für den Einkauf gepflegt sein.

[Image: Screenshot of company data settings in the Lager/EK/EDI tab.]
**Abb. D-91**: Firmendaten – Register Lager/EK/EDI

### Rechnung kontrollieren

Sie können die Preise sowohl in der Auftragsbestätigung als auch in der Rechnung des Lieferanten prüfen. Dazu stehen zwei Dialoge zur Verfügung, die im Aufbau und in den Funktionen identisch sind:
*   Preiskontrolle
*   Rechnungskontrolle

Die Preiskontrolle haben Sie bereits in der Einheit `AB erfassen und Preise prüfen` kennengelernt. Analog zur Preiskontrolle können Sie die Lieferantenrechnung prüfen und damit zur Anweisung freigeben.

> **Cursorposition bestimmen**
> Wenn Sie im Menü `Optionen > Schnellerfassung` aktivieren, springt der Cursor nach der Eingabe der Bestellnummer direkt in das Feld `Rechnungssumme` bzw. `AB-Summe`. Sie können diese Option dann nutzen, wenn Sie in der Regel nur eine Bestellnummer eintragen.

**So prüfen Sie eine eingegangene Lieferantenrechnung**

1.  Wählen Sie `Dokumente > Bestellungen > Rechnung > Rechnungskontrolle`.

    [Image: Screenshot of the Rechnungskontrolle dialog, initial view.]
    *   **A**: Rechnungsnummer
    *   **B**: Rechnungsdatum
    *   **C**: Betrag der Rechnung (netto/brutto)
    *   **D**: Bestellnummer(n)
    *   **E**: Kurs
    **Abb. D-92**: Rechnungskontrolle

    ⇨ Softwarereferenz, "Rechnungskontrolle - Bestellungen" auf Seite D-248

2.  Geben Sie die Rechnungsnummer (A), das Datum (B) und die Bestellnummer (D) ein und springen Sie mit `<Tab>` in das nächste Feld.
    In der Übersicht `Bestellungen` wird die Bestellung angezeigt.
    Wenn in der Rechnung mehrere Bestellungen zusammengefasst sind, können Sie nacheinander alle Bestellnummern angeben. Die Bestellungen werden dann jeweils in der Übersicht hinzugefügt. Sie können jedoch nur Bestellungen mit identischem Steuersatz zusammenfassen. Geben Sie einfach die nächste Bestellnummer ein und drücken Sie die `<Tab>`-Taste.
    Sie können eine Bestellung aus der Übersicht wieder entfernen, indem Sie den Eintrag markieren und auf `<Entf>` drücken.

3.  Geben Sie die Rechnungssumme (C) ein.
    > **Währung**
    > Wenn Sie nur mit einer Währung (EUR) arbeiten, muss im Feld `Kurs` (E) `1` eingetragen sein.

4.  Wählen Sie im Menü `Start > Ausführen`, um die Eingabe zu bestätigen.
    Der Betrag wird geprüft und das Register `Positionen` wird angezeigt.

    [Image: Screenshot of the Rechnungskontrolle dialog, 'Positionen' tab.]
    *   **A**: Positionspreis
    *   **B**: Differenz über alle Positionen
    **Abb. D-93**: Rechnungskontrolle – Positionen

    Sie können Preisdifferenzen ausgleichen, indem Sie einen Positionspreis überschreiben. Geänderte Beträge werden in die referenzierten Dokumente zurückgeschrieben.

5.  Wählen Sie im Menü `Start > Ausführen`, wenn keine Differenz (mehr) angezeigt wird.
    Die Daten werden gespeichert und der Status der Bestellung(en) wird umgesetzt. Die Rechnungskontrolle für diese Dokumente kann danach nicht nochmals durchgeführt werden.
    Die Berechnung der EK-Preise wird in den zugehörigen Bestellungen und Aufträgen korrigiert, sofern diese Option im Menü `Optionen > Gruppe Einstellungen` aktiviert ist.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Preiskontrolle" auf Seite D-205
⇨ Softwarereferenz, "Rechnungskontrolle - Bestellungen" auf Seite D-248

### Übungen

Die Übungen sind so konzipiert, dass Sie den gesamten Einkauf trainieren. Das bedeutet, dass Sie die Bestellungen aus dem vorigen Themenblock jetzt weiterbearbeiten.

**Wareneingang erfassen**
Erfassen Sie den Wareneingang zu einer referenzierten Bestellung vollständig und prüfen Sie die Statusumsetzung im Auftrag.

**Wareneingang teilweise erfassen**
Erfassen Sie eine Teillieferung zu einer referenzierten und zu einer manuellen Bestellung.
Erfassen Sie den Wareneingang einer Lagerbestellung und einer Position mit Produkten, die nicht als Lagerartikel geführt werden (ganz oder teilweise).

**Wareneingang von Kisten erfassen**
Erfassen Sie den Wareneingang von Kisten ganz oder teilweise.

**Vollständigkeit der Lieferungen prüfen**
Suchen Sie nach Bestellungen, zu denen Positionen oder Teilpositionen nicht geliefert wurden.
Holen Sie ggf. die Erfassung des Wareneingangs durch eine komplett-Buchung nach.

**Rechnung prüfen**
Erfassen Sie die Rechnung zu einem Wareneingang.

# Elektronischer Dokumentenaustausch

In diesem Themenblock lernen Sie, wie Sie A+W Business für elektronischen Dokumentenaustausch anpassen und Dokumente exportieren und importieren.

Dazu gehören folgende Lerneinheiten:
*   "Export/Import (openTRANS)" auf Seite D-151
*   "Datenexport/-import (EDI)" auf Seite D-177

Sie können Dokumente mit Ihren Lieferanten/Kunden elektronisch austauschen.

Für den Austausch von Bestellungen werden die Daten in eine ASC-Datei geschrieben. Für den Austausch von Rechnungen oder Auftragsbestätigungen müssen die Daten im openTRANS-Format (XML-Format) vorliegen.

[Image: Diagram showing data exchange between Kunde (Customer) and Lieferant (Supplier) via A+W Business using EDI and openTRANS.]
**Abb. D-94**: Daten Ex- und Import

Per EDI können Bestellungen ausgetauscht werden. Ein Kundenauftrag ist dabei aus Sicht des Kunden eine Bestellung, aus Sicht von A+W Business ein Auftrag.

Im Format openTRANS können Auftragsbestätigungen (ABs) und Rechnungen ausgetauscht werden. Dazu müssen alle Beteiligten mit A+W Business arbeiten. Diese Funktion ist in den folgenden Kapiteln ausführlich dargestellt.

## Export/Import (openTRANS)

### Lernziele
*   Funktionsweise des elektronischen Dokumentenaustauschs kennenlernen.
*   Voreinstellungen kennenlernen und anpassen.
*   Pflichtfelder in Dokumenten kennenlernen.
*   Elektronische Dokumente senden und einlesen.

### Nutzen
*   Mit dem elektronischen Dokumentenaustausch können Sie Dokumente Ihrer Kunden und Lieferanten einlesen, ohne die Daten einzeln erfassen zu müssen.
*   Mit dem Einlesen von Daten vermindern sich Fehler bei der Erfassung.

### Merke
*   **Voraussetzung**: Beim Lieferanten/Kunden und Ihnen muss die gleiche Version von A+W Business installiert sein, mindestens A+W Business 5. Die notwendigen Dienste müssen installiert und gestartet sein.
*   **Datenformat**: Elektronische Dokumente können in den Formaten openTRANS und XML ausgetauscht werden.
*   **Datenimport**: Die Daten können als Datei per E-Mail gesendet oder auf einem gemeinsamen freigegebenen Laufwerk auf einem Server gespeichert werden.
*   **Datenexport**: Bei jedem Drucklauf von Auftragsbestätigungen oder Rechnungen wird geprüft, ob Dokumente mit dem Kennzeichen für den Export vorhanden sind. Diese Dokumente werden dann automatisch an die hinterlegte E-Mail-Adresse gesendet.
*   **Referenzen**: Dokumentenreferenzen werden aus folgenden Feldern gebildet:
    *   Im Auftragskopf Feld Bestelltext1
    *   In der Positionserfassung Feld Kundenposition.
    Diese Felder müssen daher immer gefüllt sein.
    Wenn diese Referenzen in eingelesenen Dokumenten nicht hergestellt werden können, muss die Zuordnung beim Prüfen des elektronischen Dokuments manuell nachgeholt werden.
*   **Teillieferungen**: Aus einer elektronischen AB können Teillieferungen erstellt werden.
*   **Rundungsdifferenzen**: Bei der Preis- und Rechnungskontrolle können Rundungsdifferenzen im Cent-Bereich akzeptiert werden, wenn in der Produktverwaltung ein Ausgleichsprodukt angelegt ist, dem diese Differenzen zugeordnet werden können.
*   **Sammelrechnungen**: Bei Sammelrechnungen des Lieferanten kann ein einmal aufgeführter Zuschlag auf alle Positionen der zugehörigen Bestellungen oder Bestellpositionen verteilt werden.
*   **Dokumentensperre**: Während der Preis- und Rechnungsprüfung sind die referenzierten Dokumente für den Zugriff durch andere Mitarbeiter gesperrt.
*   **Voreinstellungen**:
    *   **Stammdaten**:
        *   Produktdaten
        *   Kunden-/Lieferantendaten
        *   Statusdefinition
        *   Statuszuordnung
        *   Währungen
    *   **Firmendaten**:
        *   Register Parameter
    *   **Stammdaten**:
        *   B2B Kunde/Lieferant

### Dokumentenaustausch

Auftragsbestätigungen und Rechnungen können im openTRANS-Format exportiert und importiert werden. Dieses Format wurde für A+W Business erweitert. Es können jedoch auch Dokumente im Standard-Format und XML-Dateien eingelesen werden.

Der Datenaustausch über das openTRANS-Format setzt voraus, dass beim Lieferanten/Kunden und Ihnen die gleichen Versionen von A+W Business installiert sind, mindestens A+W Business 5. Außerdem müssen in der Schnittstellenverwaltung die Parameter beim Lieferanten/Kunden genauso festgelegt werden wie in Ihrem A+W Business.

### Dokumenten-Export

Der Export von Auftragsbestätigungen und Rechnungen wird pro Kunde/Lieferant im Modul `Stammdaten > B2B` konfiguriert. Dazu wird festgelegt, ob und welche Dokumente exportiert werden sollen und welcher Modus dazu verwendet wird.

[Image: Screenshot of the openTRANS document export settings dialog.]
*   **A**: Export-Modus
*   **B**: Export-Format
*   **C**: Auswahl der Dokumente
*   **D**: Einstellungen für E-Mail-Modus
**Abb. D-95**: Einstellungen für den elektronischen Datenaustausch

**Export-Modus (A):**
*   **Automatischer Versand per E-Mail:**
    Dazu muss im Netzwerk ein E-Mail-Server zur Verfügung stehen. Standardmäßig wird die E-Mail-Adresse aus den Stammdaten des Kunden/Lieferanten verwendet. Für Auftragsbestätigungen und für Rechnungen können aber auch abweichende E-Mail-Adressen hinterlegt werden.
*   **Ablage in einem bestimmten Verzeichnis (auf dem Server):**
    Diese Dateien können anschließend manuell übermittelt werden.

Bei jedem Drucklauf von Auftragsbestätigungen oder Rechnungen wird geprüft, ob Dokumente mit dem Kennzeichen für den Export vorhanden sind. Der eigentliche Export wird über einen Dienst zyklisch im Hintergrund durchgeführt. Zur Kontrolle werden die entsprechenden Dokumente im Dialog `Export` angezeigt. Durch den Export werden folgende Dateien erzeugt:

*   `RESPONSExxxx.awotres` für Auftragsbestätigungen.
*   `DISPATCHxxxx.awotdis` für ein Liefer-Avis.
*   `INVOICExxxx.awotinv` für Rechnungen.

Bei den Dateinamen wird zwischen Groß- und Kleinschreibung unterschieden.

### Dokumentenreferenzen

Die Dokumentenreferenzen auf Positionsebene werden benötigt, um Auftragspositionen automatisch ihren jeweiligen Bestellpositionen zuzuordnen (Referenzierung). Bei der manuellen Erfassung eines Auftrags werden diese Dokumentenreferenzen automatisch aus den Feldern `Bestelltext1` im Auftragskopf und `Kundenposition` in der Positionserfassung gebildet.

[Image: Screenshot showing the fields 'Bestelltexte' and 'Kundenposition' used for data exchange references.]
*   **A**: Kopfdaten – Dokument
*   **B**: Positionen – Register Position
**Abb. D-96**: Referenzen für den Datenaustausch

Außerdem muss in den Firmendaten im Register `Parameter` die Option `Bestelltext1 und Kundenposition in Dokumentenreferenzen übernehmen` aktiviert sein.

[Image: Screenshot of the parameter setting 'Bestelltext1 und Kundenposition in Dokumentenreferenzen übernehmen'.]
**Abb. D-97**: Firmendaten - Parameter

### Dokumenten-Import

Auftragsbestätigungen und Rechnungen im openTRANS-Format werden über das `A+W openTRANS Import Tool` importiert. Es wird standardmäßig auf dem A+W Business-Client installiert.

Zum Einlesen stehen damit unterschiedliche Möglichkeiten zur Verfügung:
*   Doppelklick auf die gespeicherte Datei.
*   Doppelklick auf die als E-Mail-Anhang gesendete Datei.

Durch den Doppelklick werden die Daten in die Datenbank importiert und können in den Import-Dialogen von A+W Business angezeigt werden.

Wenn die Dateien auf der Festplatte abgelegt sind, so kann über das Kontextmenü die Option `Anzeigen` gestartet und eine generische Ansicht des Dokuments angezeigt werden.

### XML-Dateien

XML-Dateien können nicht direkt aus dem E-Mail-Client heraus eingelesen werden. Diese Dateien müssen zunächst gespeichert werden. Danach können sie über das Kontextmenü eingelesen oder als generische Ansicht angezeigt werden.

Nachdem ein Dokument erfolgreich eingelesen wurde, steht es im jeweiligen Dialog `Elektr. Preiskontrolle` oder `Elektr. Rechnungskontrolle` zur Verfügung.

### Dokumentenkontrolle

Die Dialoge `Elektr. Preiskontrolle` und `Elektr. Rechnungskontrolle` sind identisch aufgebaut.

[Image: Screenshot of the electronic invoice control dialog.]
*   **A**: Eingelesenes Dokument
*   **B**: Anzeige- und Filtereinstellungen
*   **C**: Status
*   **D**: Referenzierte Dokumente
**Abb. D-98**: Elektronische Rechnungskontrolle

In beiden Dialogen werden alle Dokumente (D) einschließlich möglicher Teillieferungen angezeigt, die mit dem importierten Dokument (A) verknüpft sind. Zu jeder Bestellung wird optisch signalisiert (C), ob die Verknüpfungen zwischen Bestellung und importiertem Dokument vollständig sind. Nur vollständig referenzierte Dokumente können akzeptiert werden.

Wenn das importierte Dokument akzeptiert wurde, wird der Status der referenzierten Bestellungen entsprechend umgesetzt. Die Preis- oder Rechnungskontrolle kann dann nicht nochmals durchgeführt werden.

**Buchungsarten**

Bei der Kontrolle der importierten Dokumente werden je nach Status die Optionen `Akzeptieren`, `Teillieferung erstellen` und `Ablehnen` angeboten.

Die Buchungsart `Akzeptieren` ist nur dann freigeschaltet, wenn ein importiertes Dokument vollständig und fehlerfrei referenziert ist. Wenn nur die Bestellmengen nicht vollständig referenziert sind, das Dokument jedoch ansonsten vollständig ist, so kann über die Buchungsart automatisch eine `Teillieferung` erzeugt werden.

### Positionszuordnung

Sind in einem openTRANS-Dokument die Bestellreferenzen fehlerhaft oder gar nicht vorhanden, kann das System Dokumenten- und Bestellpositionen nicht automatisch miteinander verknüpfen. Diese (nicht verknüpften) Positionen werden in der Positionsübersicht gekennzeichnet und müssen manuell verknüpft werden.

In der Rechnung kann z. B. die Referenz zu einer Position fehlen oder fehlerhaft aufgeführt sein. Anhand der Produktbezeichnungen können Sie diese Referenzen im Dialog `Positionen` manuell zuordnen herstellen.

### Fußzuschläge/-rabatte

Fußzuschläge oder -rabatte werden im Normalfall nicht in der Bestellung erfasst. In der Auftragsbestätigung oder Rechnung sind sie jedoch aufgeführt. Um eine Rechnungskontrolle durchführen zu können, müssen diese Positionen in den Bestellungen nachträglich erfasst werden. Dazu kann die Bestellerfassung aus dem Dialog `Rechnungskontrolle` heraus geöffnet werden. Nachdem der Zuschlag in der Bestellung eingefügt ist, muss er in der Rechnung zugeordnet werden.

Wenn mehrere Bestellungen vom Lieferanten in einer Rechnung zusammengefasst sind, in der ein Fußzuschlag/-rabatt nur einmal aufgeführt ist, so kann diese Position auf alle verknüpften Bestellungen verteilt werden. Das Programm versucht, für die anteiligen Beträge anhand der Zuschlagsbasis sinnvolle Vorschlagswerte zu finden und bietet diese an. Diese Werte können überschrieben werden.

Außerdem können die Fußzuschläge/-rabatte anhand der Produktnummer für diesen Lieferanten automatisch zugeordnet werden. Dabei wird die Zuordnung der Produktnummer des Lieferanten zur eigenen Produktnummer gespeichert.

**Sammelrechnungen in A+W Business**

Wenn in A+W Business Sammelrechnungen erstellt werden, so werden für jeden Auftrag die Fußzuschläge/-rabatte als eigene Position aufgeführt. Da eine direkte manuelle Zuordnung oft schwer ist, können in diesem Fall mehrere Dokumentenpositionen zusammengefasst und den Bestellpositionen zugeordnet werden. In der Positionsübersicht ist anschließend nur noch die zusammengefasste Dokumentenposition aufgeführt.

### Betragsdifferenzen

Üblicherweise können Sie eine Rechnung nur akzeptieren, wenn keine Differenzen auftreten. Wenn Sie bei einem Lieferanten mit Betragsdifferenzen rechnen (müssen), können Sie diese auf unterschiedliche Weise behandeln:

*   Sie können die Rechnung ablehnen und den Lieferanten über die Unstimmigkeiten (telefonisch) informieren.
*   Betragsdifferenzen können auch durch unterschiedliche Rundungen entstehen. Mit der Option `Betragsdifferenzen akzeptieren` können Sie die Rechnungskontrolle trotz solcher Differenzen durchführen. Die Differenz darf sich nur im Cent-Bereich bewegen. Sie sollten sich mit der Option `Hinweis auf Betragsdifferenz/Ausgleichsposition` darauf aufmerksam machen lassen.
*   Die Rundungsdifferenzen im Cent-Bereich können automatisch akzeptiert werden. Dazu muss ein sogenanntes Ausgleichsprodukt angelegt sein, auf das der Differenzbetrag gebucht werden kann.
*   Mit der Funktion `Prod.Nr. für Ausgleichspos.` können Sie ein Produkt auswählen, auf das Rundungsdifferenzen (im Cent-Bereich) verbucht werden sollen.

### Dienste prüfen

Folgende Dienste müssen installiert und gestartet sein:

*   **A+W Business 6 Interface Service**: Dieser Dienst wird in aller Regel auf einem separaten Rechner installiert. Bei der Installation durch einen Service-Mitarbeiter der A+W Software GmbH muss die Funktion `Interface Service handles B2B documents` aktiviert werden.
*   **AWProtocol**: Diesen Dienst finden Sie unter `Systemsteuerung > Verwaltung > Dienste`.
*   **ERP-WebService**: Diesen Service finden Sie unter `Systemsteuerung > Computerverwaltung > Dienste und Anwendungen > Sites > Default Web Site`.

[Image: Screenshot of Windows Computer Management showing the ERP-WebService under IIS Sites.]
**Abb. D-99**: ERP-Service prüfen

Die Dienste werden in der Regel mit A+W Business zusammen installiert. Sie sind auf den Starttyp `Automatisch` eingestellt. Dadurch sollten sie beim Start des Rechners automatisch gestartet werden.

Wenn der Datenaustausch nicht funktioniert, sollten Sie die Dienste prüfen und ggf. manuell starten. Eine Anleitung dazu finden Sie in der Online-Hilfe des Betriebssystems.

Außerdem benötigen Sie das A+W openTRANS ImportTool, das vom A+W Business-Setup automatisch installiert wird.

### Statusvergabe

Der Status der Dokumente wird auch beim Im- und Export umgesetzt. Dazu müssen folgende Statuspunkte zugeordnet sein.

| Statuspunkte für Import | für Export |
| :--- | :--- |
| 61 - Auftragsbestätigung nicht akzeptieren | 830 - Rechnungsexport |
| 64 - Rechnung nicht akzeptieren | 840 - Auftragsbestätigungsexport |

Beim Import wird der Status manuell umgesetzt, beim Export automatisch.
Im Part Stammdaten sind die Statuspunkte und Statuszuordnungen ausführlich beschrieben. In dieser Einheit wird daher nur auf die Besonderheiten eingegangen, die Sie für den Austausch von elektronischen Dokumenten beachten müssen.

### Voreinstellungen für Datenaustausch prüfen

In den Firmendaten müssen die Einstellungen für den Austausch von Produktdaten korrekt eingestellt sein. Nur wenn die entsprechenden Produktdaten hinterlegt und zugeordnet sind, können die Dokumente korrekt eingelesen werden.

> **A+W Business neu starten**
> Nach Änderungen der Firmendaten sollten Sie A+W Business neu starten.

**So prüfen Sie die Firmendaten**

1.  Wählen Sie `Stammdaten > Firma > Firmendaten` und wechseln Sie zum Register `Parameter`.

    [Image: Screenshot of the company data settings, 'Parameter' tab.]
    *   **A**: Bestelltext übernehmen
    **Abb. D-100**: Firmendaten - Parameter

    ⇨ Stammdaten, "Firmendaten - Parameter" auf Seite B-948

2.  Aktivieren Sie die Checkbox `Bestelltext1 und Kundenposition in Dokumentenreferenzen übernehmen`.

3.  Wählen Sie im Menü `Start > Speichern`, um Änderungen zu speichern.
    Die Daten werden gespeichert.

### Währungseinstellungen prüfen

Für die Währungen, die in den Aufträgen und Bestellungen verwendet werden, muss das internationale Währungskennzeichen hinterlegt sein. Die Einstellungen müssen Sie prüfen, wenn Sie mit mehreren Währungen arbeiten.

**So prüfen Sie die Währungseinstellungen**

1.  Wählen Sie `Stammdaten > Finanzen > Währung`.

    [Image: Screenshot of the currency settings dialog.]
    *   **A**: Wechselkurs für Umrechnung von Preisen
    *   **B**: Internationales Währungskennzeichen
    **Abb. D-101**: Internationales Währungskennzeichen

    ⇨ Stammdaten, "Währung" auf Seite B-921

    Jeder Währung muss das internationale Kennzeichen (B) zugewiesen sein.

2.  Markieren Sie die Zeile der Währung, der Sie das Kennzeichen zuweisen wollen.

3.  Öffnen Sie in der Spalte `Internat. Kennzeichen` die Kombobox und wählen Sie aus der Liste das entsprechende Kennzeichen aus.

4.  Prüfen Sie die jeweils eingetragenen Wechselkurse (A) und aktualisieren Sie diese ggf.

5.  Wählen Sie im Menü `Start > Speichern`, um Änderungen zu speichern.
    Die Daten werden gespeichert.

### Statusdefinitionen prüfen

Damit die elektronischen Dokumente verarbeitet werden können, müssen die Statuspunkte 61, 64, 830, 840 definiert und zugeordnet sein. Diese Statuspunkte werden für folgende Aktionen benötigt:
*   Dokumente ex- und importieren.
*   Importiertes Dokument ablehnen oder akzeptieren.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So prüfen Sie die Statuspunkte" auf Seite D-163
*   "So prüfen Sie die Statusverwaltung" auf Seite D-164
*   "So prüfen Sie die Statuszuordnung" auf Seite D-165

**So prüfen Sie die Statuspunkte**

1.  Wählen Sie `Stammdaten > Auftrag > Statuspunkte`.

    [Image: Screenshot of the Status Points definition dialog.]
    **Abb. D-102**: Statuspunkte

    ⇨ Stammdaten, "Statuspunkte" auf Seite B-898

2.  Prüfen Sie, ob die Statuspunkte 61, 64, 830 und 840 vorhanden sind.
    Die Nummern der Statuspunkte sind in der Spalte `Kennz.` angegeben.
    In der Regel werden die Statuspunkte mit der Installation zusammen erstellt. Sie müssen immer manuell zugeordnet werden.

3.  Wenn diese Statuspunkte nicht vollständig vorhanden sind, legen Sie die fehlenden an.

4.  Wählen Sie im Menü `Start > Speichern`, um Änderungen zu speichern.
    Die Daten werden gespeichert. Diese Statuspunkte müssen einem entsprechenden Anwenderstatus zugeordnet sein.

**So prüfen Sie die Statusverwaltung**

1.  Wählen Sie `Stammdaten > Auftrag > Statusverwaltung`.

    [Image: Screenshot of the Status Administration dialog.]
    **Abb. D-103**: Statusverwaltung

    ⇨ Stammdaten, “Statusverwaltung" auf Seite B-897

    Wenn die Anwenderstatus 61/64 und 830/840 nicht vollständig vorhanden sind, legen Sie die fehlenden an.

2.  Wählen Sie im Menü `Start > Speichern`, um Änderungen zu speichern.
    Prüfen Sie als Nächstes, ob alle Zuordnungen vorhanden und vollständig sind.

**So prüfen Sie die Statuszuordnung**

1.  Wählen Sie `Stammdaten > Auftrag > Statuszuordnung`.

    [Image: Screenshot of the Status Assignment dialog.]
    *   **A**: Statuspunkt
    *   **B**: Dokumententyp
    *   **C**: Zugeordneter Anwenderstatus
    **Abb. D-104**: Statuszuordnung

    ⇨ Stammdaten, “Statuszuordnung" auf Seite B-899

2.  Prüfen Sie, ob die Statuspunkte 61, 64, 830 und 840 zugeordnet sind.
    Wenn Sie in der Tabelle `Statuszuordnung` einen Statuspunkt markieren, muss mindestens der Anwenderstatus (C) angezeigt werden.
    Wenn diese Statuspunkte nicht vollständig zugeordnet sind, holen Sie die Zuordnung nach.

3.  Wählen Sie im Menü `Start > Neu`, um in den Erfassungs-Modus zu wechseln.

4.  Wählen Sie in den Feldern `Statuspunkt`, `Dokumententyp` und `Anwenderstatus` die entsprechenden Einträge aus.

5.  Wählen Sie im Menü `Start > Speichern`, um Änderungen zu speichern.
    Die Daten werden gespeichert.

### Datenexport per openTRANS einstellen

Im Modul `Stammdaten > B2B` müssen Sie festlegen, wie die Daten ausgetauscht werden sollen.

**So legen Sie die Exportart für openTRANS fest**

1.  Wählen Sie `Stammdaten > B2B > Kunde > Dokumentenexport`.
    Der Dialog `openTRANS-Dokumentenexport` wird mit dem Register `Auswahl` angezeigt.

2.  Wählen Sie im Menü `Start > Suchen`, um in die Kunden einzulesen.
    Die Kunden werden im Register `Tabelle` aufgelistet.

3.  Markieren Sie den Kunden (C), mit dem Dokumente über das openTRANS-Format ausgetauscht werden sollen.

4.  Wechseln Sie zum Register `Auswahl`.
    *   Wenn die Angaben für den Kunden korrekt sind, können Sie den nächsten Kunden prüfen.
    *   Wenn keine Angaben vorhanden sind, müssen Sie diese einpflegen.

    [Image: Screenshot of the openTRANS document export settings dialog.]
    *   **A**: Exportart per Datei oder per E-Mail
    *   **B**: Übertragungstyp
    *   **C**: Kundennummer
    *   **D**: Auswahl der Dokumentenart
    *   **E**: E-Mail-Adressen für unterschiedliche Dokumentenarten
    **Abb. D-105**: openTRANS-Dokumentenexport

5.  Wählen Sie im Feld `Typ` (B) den Eintrag `Standard (openTRANS basierend)` aus.
    Mit dieser Einstellung erhalten die Dokumente für diesen Kunden automatisch das Kennzeichen für den openTRANS-Austausch.

6.  Wählen Sie im Feld `Exportart` (A) aus, wie die Dateien ausgetauscht werden sollen.
    *   **Export in eine Datei:** Mit dieser Einstellung werden die Daten in eine Datei geschrieben. Die Felder für den Zielpfad werden freigeschaltet. Sie können ein Verzeichnis auswählen oder den Pfad manuell eintragen.
    *   **Export per E-Mail:** Mit dieser Einstellung werden die Daten als Anhang einer E-Mail gesendet. Dazu müssen Sie prüfen, ob in den Stammdaten des Kunden die E-Mail-Adresse korrekt eingetragen ist.
        ⇨ "Partnerstammdaten prüfen" auf Seite D-168

7.  Wählen Sie aus, ob Auftragsbestätigungen und/oder Rechnungen (D) exportiert werden sollen.

8.  Wenn Sie die Daten per E-Mail senden, können Sie abweichende E-Mail-Adressen (E) für Auftragsbestätigungen, Rechnungen und/oder Lieferavis eintragen.

9.  Wählen Sie im Menü `Start > Speichern`, um Änderungen zu speichern.
    Die Daten werden gespeichert.

10. Wiederholen Sie die Schritte 3 bis 9 für alle Kunden, mit denen Sie Daten austauschen.
    Um Auftragsbestätigungen und Rechnungen Ihrer Lieferanten importieren zu können, brauchen Sie keine weiteren Einstellungen festzulegen.

### Partnerstammdaten prüfen

In den Stammdaten der Lieferanten/Kunden müssen die Daten für die Kommunikation korrekt hinterlegt sein, damit Dokumente direkt aus A+W Business heraus versendet werden können.

**So prüfen Sie die Lieferanten-/Kundendaten**

1.  Wählen Sie `Stammdaten > Marktpartner > Lieferant, Kunde > Lieferanten, Kunden`.

    [Image: Screenshot of partner master data, address section.]
    *   **A**: E-Mail-Adresse für den Dokumentenaustausch
    **Abb. D-106**: Partnerdaten - Adresse

    ⇨ Stammdaten, "Partnerverwaltung" auf Seite B-770

2.  Prüfen Sie, ob die E-Mail-Adresse des Lieferanten, Kunden korrekt ist.
    Wenn Ihr Lieferanten oder Kunden mehrere E-Mail-Adressen haben, können Sie in den Einstellungen für den Dokumentenaustausch auch alternative E-Mail-Adressen eingeben.
    ⇨ "Datenexport per openTRANS einstellen" auf Seite D-166

3.  Wechseln Sie zum Register `Auftrag` und prüfen Sie, ob die externe Nummer eingetragen ist.

    [Image: Screenshot of partner master data, order tab.]
    *   **A**: Externe Nummer angeben
    **Abb. D-107**: Partnerdaten – Auftrag

    In den Kunden- und Lieferantendaten hat diese Nummer folgende Bedeutung:
    *   **Lieferantendaten**: Die externe Kundennummer erhalten Sie von Ihrem Lieferanten. Sie muss auch dann eingetragen werden, wenn Sie mit Ihrer internen Nummer identisch ist.
    *   **Kundendaten**: In den Stammdaten zu Ihren Kunden muss in diesem Feld die Nummer stehen, die Sie bei Ihrem Kunden als Lieferant kennzeichnet.

4.  Wählen Sie im Menü `Start > Speichern`, um Änderungen zu speichern.

### Elektronisches Dokument einlesen

Elektronische Dokumente können Sie in zwei Formaten erhalten haben: als openTRANS-Datei oder als XML-Datei. Je nach den Einstellungen in Ihrem Betrieb sind diese Dateien in einem bestimmten Verzeichnis auf dem Server abgelegt oder als Anhang einer E-Mail verfügbar.

**So lesen Sie ein openTRANS-Dokument ein**

1.  Öffnen Sie das Verzeichnis mit den gesendeten Dateien oder die E-Mail, mit der die Datei gesendet wurde.
    Die openTRANS-Datei hat die Dateiendung `*.awotdis`, `*.awotres` oder `*.awotinv`.
2.  Starten Sie den Import mit einem Doppelklick auf die Datei.
    Die Daten werden eingelesen und in den Dialogen für die elektronische Preis- oder Rechnungskontrolle angezeigt.

**So lesen Sie ein XML-Dokument ein**

1.  Öffnen Sie das Verzeichnis mit den gesendeten Dateien oder die E-Mail, mit der die Datei gesendet wurde.
2.  Speichern Sie die XML-Datei auf Ihren Rechner.
3.  Wählen Sie die Datei im Explorer aus und öffnen Sie das Kontext-Menü.
4.  Wählen Sie die Option `Als openTRANS-Dokument einlesen`.
    Die Daten werden eingelesen und in den Dialogen für die elektronische Preis- oder Rechnungskontrolle angezeigt.

### Elektronisches Dokument prüfen

Sie können in importierten Dokumenten Ihrer Lieferanten die Preise sowohl in der Auftragsbestätigung als auch in der Rechnung prüfen. Dazu stehen zwei Dialoge zur Verfügung, die im Aufbau und den Funktionen identisch sind:
*   Elektronische Preiskontrolle
*   Elektronische Rechnungskontrolle

Die Handlungsschritte werden im Folgenden am Beispiel der elektronischen Rechnungskontrolle beschrieben.

**So prüfen und akzeptieren Sie eine importierte Lieferantenrechnung**

1.  Wählen Sie `Dokumente > Bestellungen > Rechnung > Elektr. Rechnungskontrolle`.

    [Image: Screenshot of the electronic invoice control document import screen.]
    *   **A**: Optionen für die Buchungsart
    *   **B**: Einschränkung der Anzeige
    *   **C**: Status des markierten Dokuments
    *   **D**: Hinweis zu Diskrepanzen
    *   **E**: Filterung der angezeigten Dokumente
    *   **F**: Referenzierte Dokumente
    **Abb. D-108**: Elektronische Rechnungskontrolle – Dokumentenimport

2.  Schränken Sie die Anzeige ein, wenn zu viele Dokumente angezeigt werden:
    *   Wählen Sie für die Anzeige (B) den Eintrag `Nur offene Dokumente`.
    *   Klicken Sie auf die Schaltfläche (E) und stellen Sie die gewünschten Filter ein. Im Dialog `Filtereinstellungen` können Sie mehrere Lieferanten auswählen und mit `[OK]` übernehmen.
        ⇨ Softwarereferenz, "Filtereinstellungen" auf Seite D-223

3.  Markieren Sie eine der angezeigten Rechnungen.
    In der Übersicht `Bestellungen/Teillieferungen` (F) werden alle Bestellungen aufgelistet, die zu dieser Rechnung gehören.
    Im Bereich `Dokumentenstatus` (C) können Sie sehen, ob Referenzen fehlen und/oder Differenzen in Preisen oder Mengen auftreten.
    *   Wenn Sie Preisdifferenzen nicht akzeptieren wollen, wählen Sie die Option `Ablehnen` (A) und schicken Sie die Rechnung zurück. Das Dokument wird als abgelehnt gekennzeichnet und kann archiviert werden.
    *   Korrigieren Sie die Differenzen wie in den folgenden Handlungsschritten erläutert wird.
    *   Stellen Sie die fehlenden Referenzen her.
        ⇨ "So ordnen Sie Positionen in einer importierten Rechnung zu" auf Seite D-173

4.  Wechseln Sie ggf. zum Register `Positionsübersicht`, um die Differenzen der Einkaufspreise einzelner Positionen zu prüfen.
    Wenn Betragsdifferenzen durch unterschiedliche Rundungen aufgetreten sind, können Sie diese über `Menü Optionen > Betragsdifferenzen akzeptieren` generell zulassen. In diesem Fall können Sie eine der Buchungsarten `Ablehnen` oder `Akzeptieren` wählen.

    [Image: Screenshot of the electronic invoice control - position overview.]
    **Abb. D-109**: Elektronische Rechnungskontrolle – Positionsübersicht

    Sie können die Positionspreise und -mengen nicht direkt korrigieren.
5.  Markieren Sie die Position, die Sie korrigieren möchten.

6.  Wählen Sie im Menü `Funktionen > Bestellerfassung öffnen` und korrigieren Sie die Menge.
    Wenn Sie die Differenzen korrigiert und gespeichert haben und die Bestellerfassung wieder schließen, werden die neuen Werte in der elektronischen Rechnungskontrolle angezeigt.
    Preisdifferenzen brauchen Sie nicht manuell zu korrigieren. Es genügt, wenn Sie das Dokument trotz dieser Differenzen akzeptieren. Die Korrektur führt das Programm automatisch aus.

7.  Wenn alle Fehler behoben sind, wählen Sie die Option `Akzeptieren`.

8.  Wählen Sie im Menü `Start > Speichern`, um die Rechnungskontrolle abzuschließen.
    Die Daten werden gespeichert und der Status der Bestellung(en) wird umgesetzt. Die Rechnungskontrolle für diese Dokumente kann danach nicht nochmals durchgeführt werden.

### Teillieferung aus elektronischem Dokument erstellen

Wenn in dem eingelesenen Dokument nur ein Teil der Bestellpositionen oder bestellten Mengen aufgeführt ist, können Sie eine Teillieferung erstellen.

**So erstellen Sie eine Teillieferung zu einer importierten Lieferantenrechnung**

1.  Wählen Sie `Dokumente > Bestellungen > Rechnung > Elektr. Rechnungskontrolle`.
    ⇨ Softwarereferenz, "Elektronische Rechnungskontrolle" auf Seite D-256

2.  Markieren Sie die Rechnung, zu der Sie eine Teillieferung erfassen möchten.
    Wenn der Dokumentenstatus außer Mengendifferenzen keine weiteren Fehler anzeigt, können Sie eine Teillieferung erzeugen. Nur dann ist die Option `Teillieferung erstellen` freigeschaltet.
    Wie Sie fehlende Referenzen herstellen, finden Sie unter:
    ⇨ "So ordnen Sie Positionen in einer importierten Rechnung zu" auf Seite D-173

3.  Wählen Sie die Option `Teillieferung erstellen`.

4.  Wählen Sie im Menü `Start > Ausführen`, um die Teillieferung zu erzeugen.
    Damit wird eine Teillieferung mit der Rechnungsnummer, der gelieferten Menge und den Preisen aus dem importierten Dokument erzeugt. Der Status der Original-Bestellung wird entsprechend umgesetzt.
    Die Original-Bestellung kann so lange wieder zugeordnet werden, bis alle Positionen vollständig geliefert und referenziert sind.

### Positionen im elektronischen Dokument zuordnen

Wenn die Referenzen im elektronischen Dokument nicht eindeutig sind, kann die Position nicht zugeordnet werden. Diese Zuordnung können Sie bei der Prüfung des Dokuments nachholen.

Wenn eine Position in der Bestellung vollständig fehlt, z. B. ein Energiezuschlag, müssen Sie diese Position in der entsprechenden Bestellung zunächst erfassen. Sie können dazu die Bestellung aus der Preis-/Rechnungskontrolle heraus öffnen. Wenn Sie die Position erfasst und gespeichert haben, fahren Sie in der Rechnungskontrolle fort.

**So ordnen Sie Positionen in einer importierten Rechnung zu**

1.  Wählen Sie `Dokumente > Bestellungen > Rechnung > Elektr. Rechnungskontrolle`.
    Der Dialog (elektronische) Rechnungskontrolle wird geöffnet und die importierten Rechnungen werden angezeigt.
    ⇨ Softwarereferenz, “Elektronische Rechnungskontrolle" auf Seite D-256

2.  Markieren Sie die Rechnung, deren Positionen Sie zuordnen möchten.

3.  Wechseln Sie zum Register `Positionsübersicht`.
    Sie können eine Position in der Bestellung nachträglich erfassen, indem Sie über das Menü `Funktionen > Bestellerfassung öffnen` zum Dokument wechseln. Wenn Sie die Position erfasst und gespeichert haben, fahren Sie in der Rechnungskontrolle mit Schritt 4 fort.

    [Image: Screenshot of the position overview in the electronic invoice control dialog.]
    **Abb. D-110**: Elektronische Rechnungskontrolle – Positionsübersicht

4.  Markieren Sie die Position, die nicht zugeordnet werden konnte, und wählen Sie im Menü `Funktionen > Positionen manuell zuordnen`.

    [Image: Screenshot of the manual position assignment dialog.]
    *   **A**: Position aus der Rechnung
    *   **B**: Zuordnung des Fußzuschlags für die aktuelle Sitzung beibehalten
    *   **C**: Zuordnung des Fußzuschlags für alle künftigen Importe speichern
    *   **D**: Position in der Bestellung
    **Abb. D-111**: Elektronische Rechnungskontrolle – Positionen zuordnen

    ⇨ Softwarereferenz, "Positionen manuell zuordnen" auf Seite D-221

5.  Markieren Sie in der linken und der rechten Übersicht jeweils die Positionen (A, D), die Sie einander zuordnen möchten.

6.  Klicken Sie auf `[OK]`, um die Zuordnung zu speichern.

7.  Wiederholen Sie den Vorgang, bis alle Positionen zugeordnet sind.
    Wenn Sie Fußzuschläge/-rabatte zugeordnet haben, können Sie über die beiden Checkboxen (B, C) festlegen, ob die Zuordnung für diese Rechnung und/oder diesen Lieferanten beibehalten werden soll.
    Wie Sie einen Fußzuschlag/-rabatt auf mehrere Bestellungen verteilen, finden Sie unter:
    ⇨ "Zuschläge/Rabatte manuell zuordnen" auf Seite D-175

8.  Klicken Sie auf `[Ende]`, wenn alle Zuordnungen korrekt sind.
    Im Dialog `Elektr. Rechnungskontrolle` sind alle Buchungsarten freigeschaltet.

9.  Wählen Sie die gewünschte Buchungsart, z. B. `Akzeptieren`.

10. Wählen Sie im Menü `Start > Ausführen`, um die Aktion zu starten.

11. Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern.
    Die Daten werden gespeichert und der Status der Bestellung(en) wird umgesetzt.

### Zuschläge/Rabatte manuell zuordnen

Wenn in einer Rechnung zu mehreren Bestellungen nur ein Fußzuschlag/-rabatt aufgeführt ist, können Sie diesen manuell auf die einzelnen Bestellungen und/oder Bestellpositionen verteilen. Der Zuschlag/Rabatt wird dann anteilig berechnet und in die Bestellungen zurückgeschrieben.

**So verteilen Sie den Fußzuschlag/-rabatt auf Bestellungen**

1.  Wählen Sie `Dokumente > Bestellungen > Rechnung > Elektr. Rechnungskontrolle`.
    Der Dialog `Elektr. Rechnungskontrolle` wird geöffnet und die importierten Rechnungen werden angezeigt.
2.  Markieren Sie die Rechnung, aus der Sie den Fußzuschlag/-rabatt verteilen möchten.

    [Image: Screenshot of the dialog to distribute surcharges/discounts on orders.]

    ⇨ Softwarereferenz, "Fußzuschläge/-rabatte verteilen" auf Seite D-222
    In der Übersicht `Bestellungen/Teillieferungen` werden alle referenzierten Dokumente angezeigt.
3.  Wählen Sie im Menü `Funktionen > Fußzuschläge/-rabatte auf Bestellungen verteilen`.
4.  Halten Sie die Taste `<Strg>` gedrückt und markieren Sie alle Position, auf die der Zuschlag/Rabatt verteilt werden soll.
5.  Klicken Sie auf `[OK]`, um die Verteilung zu speichern.
    Die Daten werden in die betreffenden Bestellungen zurückgeschrieben. Die Einkaufspreise in den Bestellungen werden aktualisiert.
6.  Schließen Sie den Dialog mit `[Ende]` und fahren Sie mit der Rechnungskontrolle fort.
    ⇨ "So prüfen und akzeptieren Sie eine importierte Lieferantenrechnung" auf Seite D-170

### Ergänzende Informationen
⇨ Softwarereferenz, "Elektronische Preiskontrolle" auf Seite D-213
⇨ Softwarereferenz, "Elektronische Rechnungskontrolle" auf Seite D-256
⇨ Softwarereferenz, "Positionen manuell zuordnen" auf Seite D-221
⇨ Stammdaten, "Geschäftsabläufe abbilden" auf Seite B-427
⇨ Stammdaten, "Firmendaten - Parameter" auf Seite B-948

## Datenexport/-import (EDI)

### Lernziele
*   Funktion der Fremdschnittstelle kennenlernen.
*   Voreinstellungen für den Datenaustausch per EDI-Schnittstelle kennenlernen.

### Nutzen
*   Durch den Datenaustausch über EDI-Schnittstellen müssen Dokumente nicht manuell erfasst werden.

### Merke
*   **EDI**: EDI = Electronic Data Interchange, Elektronischer Datenaustausch per ASCII-Datei
*   **Schnittstellen**: Die Schnittstellen müssen für Kunden und Lieferanten eingerichtet werden.
*   **Voreinstellungen**:
    *   Register Lager/EK/EDI
    *   B2B: Kunde, Lieferant

### Datenaustausch im ASC-Format

Über eine EDI-Schnittstelle können Angebote, Aufträge, Bestellungen und Gutschriften ausgetauscht werden. Dabei werden die Daten in eine ASC-Datei (ascii) geschrieben. Den Pfad für diese Datei legen Sie für jeden Kunden und jeden Lieferanten fest.

Standardmäßig werden die Daten der zu transferierenden Datei automatisch im ANSI-Format konvertiert, z. B. `ä` in `ae`.

### Firmendaten prüfen

In den Firmendaten müssen Sie im Register `Lager/EK/EDI` die Voreinstellungen prüfen, die sich auf die Konvertierung beziehen.

[Image: Screenshot of EDI interface settings in company data.]
**Abb. D-112**: Firmendaten – Register Lager/EK/EDI

In der Regel sollte die OEM/ANSI-Konvertierung nur deaktiviert werden, wenn die verwendete Schnittstelle dies explizit fordert.

### Einstellungen prüfen

Wenn Sie mit Ihren Lieferanten/Kunden Aufträge und Bestellungen im ASC-Format austauschen, müssen Sie die Parameter für jeden einzelnen Lieferanten/Kunden einstellen.

**So prüfen Sie die Einstellungen für den Datenexport per EDI**

1.  Wählen Sie `Stammdaten > B2B > Lieferant > Lieferant`.
    Für den Datenimport per EDI wählen Sie `Stammdaten > B2B > Kunde > Kunde`. Die nachfolgenden Handlungsschritte gelten analog.
2.  Wählen Sie im Menü `Start > Suchen`, um in die Suche zu starten.
    Die Trefferliste wird im Register `Tabelle` angezeigt.
3.  Markieren Sie den Lieferanten, an den Bestellungen über die EDI-Schnittstelle gesendet werden sollen.

4.  Wechseln Sie zum Register `Auswahl`.

    [Image: Screenshot of the interface administration dialog.]
    *   **A**: Typ der Schnittstelle
    *   **B**: Angaben für die Zieldatei
    *   **C**: Angaben für die Protokolldatei
    *   **D**: Pfad für die Sicherungsdatei
    **Abb. D-113**: Schnittstellenverwaltung

5.  Geben Sie die Verzeichnisse und Dateinamen (B) für die Export- und die Sicherungsdatei an (D).
6.  Wählen Sie die Schnittstellenversion (A) aus, mit der Ihr System arbeitet.
    Wenn Sie Auftragsbestätigungen und Rechnungen ebenfalls elektronisch austauschen (openTRANS-Format), müssen Sie die Version wählen, mit der Sie die Daten bisher übertragen haben. Die Version wird bei der Installation von A+W Business festgelegt.

    [Image: Screenshot showing filled-in settings for EDI document export.]
    **Abb. D-114**: Einstellungen für EDI-Dokumentenexport

7.  Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern.
    Die Daten werden gespeichert.
8.  Wechseln Sie zum Register `Parameter`.

    [Image: Screenshot of parameters for EDI exchange.]
    *   **A**: Zwangsreferenzierung
    *   **B**: Sperre für den Zugriff und Zeit der Sperre
    *   **C**: Parameter für den EDI-Import von Aufträgen (nur bei Kunden)
    **Abb. D-115**: Parameter für den EDI-Austausch

9.  Markieren Sie die Checkboxen für Export:
    *   **Zwangsreferenzierung (A):** Wenn eine Position ohne Referenz auf ein (externes) Produkt gesendet wird, kann diese Position ignoriert werden. In diesem Fall wird eine Fehlermeldung im Logbuch eingetragen. Wenn die Checkbox nicht markiert ist, wird die Produktnummer aus den Stammdaten in die Schnittstellendatei geschrieben. Das ist z. B. dann sinnvoll, wenn das sendende und das empfangende System die gleichen Produktstammdaten benutzen. In dem Fall ist es nicht nötig, Daten in die Referenztabellen einzutragen.
    *   **Locking aktiv und Maximale Lock-Zeit (B):** Mit dieser Einstellung verhindern Sie, dass für den eingegebenen Zeitraum nur ein Programm auf dieselbe Schnittstellendatei zugreifen kann.
    *   **Import von Kundenaufträgen (C):** Wenn Sie die Daten für Kunden einrichten, können Sie zusätzlich Einstellungen für den Import festlegen.

10. Wiederholen Sie die Schritte für alle Lieferanten, mit denen Sie Daten per EDI austauschen.

11. Wechseln Sie zu `Stammdaten > B2B > Kunde > Kunde` und wiederholen Sie die Schritte für alle Kunden, mit denen Sie Daten per EDI austauschen.

### Bestellung exportieren

Wenn Sie Bestellungen exportieren, werden die Daten in eine ASC-Datei geschrieben. Diese wird im festgelegten Verzeichnis abgelegt. Die Datei wird danach über die EDI-Schnittstelle zum Lieferanten übertragen.

**So exportieren Sie eine Bestellung**

1.  Wählen Sie `Dokumente > Bestellungen > Export`.
    Der Dialog `Export` wird geöffnet und die Bestellungen im aktuellen Nummernverwalter werden angezeigt.

    [Image: Screenshot of the order export dialog.]
    **Abb. D-116**: Export von Bestellungen

2.  Wählen Sie im Menü `Start > Ausführen`, um den Export zu starten.
    Der Export wird gestartet. Eine Verlaufsmeldung zeigt an, welche Bestellung aktuell übertragen wird.

3.  Wechseln Sie zum Register `Pool`, um den Status des Exports zu prüfen.
    Sie können die Anzeige mit `[Abfragen]` aktualisieren.

**Ergänzende Informationen**
⇨ Verkauf, "Import von Dokumenten" auf Seite C-384
⇨ Stammdaten, "Schnittstellen-Dienst" auf Seite B-1046

# Softwarereferenz

## Übersicht

In der Dokumentenverwaltung können Sie alle Dokumente erfassen und bearbeiten, die im Rahmen des Einkaufs benötigt werden, z. B. Anfragen zu Lieferungen und Bestellungen. Außerdem können Sie Wareneingänge erfassen, Liefertermine prüfen und korrigieren und die Lieferanten-Rechnungen kontrollieren.

In der Softwarereferenz finden Sie Informationen zu folgenden Themen:
*   Anfrage (Menü)
*   Bestellung (Menü)
*   Auftragsbestätigung
*   Wareneingang
*   Rechnung
*   Basisglasverrechnung

Folgende Dialoge sind für alle Dokumentenarten gleich und sind daher nur einmal im Part `Verkauf` erklärt:
*   FiBu-Übergabe
*   Übergabe Archiv
*   Suche

> **Dialoge können von unterschiedlichen Stellen aus geöffnet werden**
> Bitte beachten Sie, dass viele Übersichten und Funktionen zum Thema Einkauf in A+W Business aus unterschiedlichen Dialogen heraus gestartet werden können. In dieser Anleitung werden die entsprechenden Dialoge nur einmal beschrieben.

> **Dialoge, die auch für den Verkauf benötigt werden, sind ausführlich im Part Verkauf beschrieben.**

**Dialogbeschreibungen im Part Verkauf**
⇨ Softwarereferenz, “Dokumentenverwaltung" auf Seite C-415
⇨ Softwarereferenz, “Übersichten und Referenzen zu Kopfdaten" auf Seite C-533
⇨ Softwarereferenz, "Positionsdaten" auf Seite C-448
⇨ Softwarereferenz, "Übersichten und Referenzen zu Positionen" auf Seite C-596
⇨ Softwarereferenz, "Nummernverwalter" auf Seite C-643
⇨ Softwarereferenz, "Druck" auf Seite C-652
⇨ Softwarereferenz, "Übergabe Archiv" auf Seite C-702

## Anfrage (Menü)

`Dokumente > Anfrage`

Über das Menü `Anfrage` erreichen Sie folgende Programmpunkte:

*   **NV Anfrage:** Die Funktion des Nummernverwalters ist für alle Dokumente gleich. Sie wird ausführlich zu den Aufträgen erklärt.
    *   Verkauf, "Nummernverwalter" auf Seite C-643
*   **Anfrage:** Die Erfassung von Dokumenten ist für alle Dokumentenarten gleich. Sie wird ausführlich zu den Aufträgen erklärt.
    *   ⇨ Verkauf, "Dokumentenverwaltung" auf Seite C-415
    *   Verkauf, "Positionsdaten" auf Seite C-448
*   **Druck Anfrage:** Der Formular- und Etikettendruck ist für alle Dokumente gleich. Er wird ausführlich zu den Aufträgen erklärt.
    *   Verkauf, "Druck" auf Seite C-652
*   **Journal:** Der Journaldruck ist für alle Dokumente gleich. Er wird ausführlich zu den Aufträgen erklärt.
    *   Verkauf, "Journal" auf Seite C-742
*   **Übergabe Archiv:** Die Archivübergabe ist für alle Dokumente gleich. Sie wird ausführlich zu den Aufträgen erklärt.
    *   ⇨ Verkauf, "Übergabe Archiv" auf Seite C-702
*   **Suche:** Die Suche ist für alle Dokumente gleich. Sie wird ausführlich zu den Aufträgen erklärt.
    *   Verkauf, "Dokument suchen" auf Seite C-534

### Anfrage (Dokumentenverwaltung)

`Dokumente > Anfrage > Anfrage`

[Image: Screenshot of the request document management dialog.]
**Abb. D-117**: Dokumentenverwaltung – Anfrage

In diesem Dialog erfassen und bearbeiten Sie Anfragen an Ihren Lieferanten. Anfragen können entweder manuell erfasst werden oder sie werden bei der Bestellübergabe erzeugt, wenn im Bestellpool die Option `Sofort anfragen` gewählt ist.
*   ⇨ Tutorial, "Anfrage" auf Seite D-110
*   Verkauf, "Bestellübergabe - Bestellnummern" auf Seite C-673

Die Felder im Dialog Dokumentenverwaltung und in der Positionserfassung sind für alle Dokumententypen gleich. Sie sind ausführlich zu den Aufträgen erklärt:
*   ⇨ Verkauf, "Dokument - Kopfdaten" auf Seite C-424
*   Verkauf, "Dokument - Positionen" auf Seite C-461

## Bestellung (Menü)

`Dokumente > Bestellung`

Über das Menü `Bestellung` erreichen Sie folgende Programmpunkte:

*   **NV Bestellung:** Die Funktion des Nummernverwalters ist für alle Dokumente gleich. Sie wird ausführlich zu den Aufträgen erklärt.
    *   Verkauf, "Nummernverwalter" auf Seite C-643
*   **Bestellung:** Die Erfassung von Dokumenten ist für alle Dokumentenarten gleich. Sie wird ausführlich zu den Aufträgen erklärt.
    *   ⇨ Verkauf, "Dokumentenverwaltung" auf Seite C-415
    *   Verkauf, "Positionsdaten" auf Seite C-448
*   **Teillieferung:** Die Erstellung von Teillieferungen ist für alle Dokumentenarten gleich. Sie wird ausführlich zu den Aufträgen erklärt.
    *   Verkauf, "Teillieferungen" auf Seite C-630
*   **Nachbestellung:** In diesem Dialog können Sie Bestellteile, die als Bruch gemeldet sind, nachbestellen, reklamieren, verrechnen oder die Auftragsmenge reduzieren.
    *   ⇨ "Nachbestellung" auf Seite D-191
*   **Druck Bestellung:** Der Formular- und Etikettendruck ist für alle Dokumente gleich. Er wird ausführlich zu den Aufträgen erklärt.
    *   Verkauf, "Druck" auf Seite C-652
*   **Export (EDI):** In diesem Dialog exportieren Sie Bestellungen über die EDI-Schnittstelle.
    *   ⇨ "Export (EDI)" auf Seite D-193
*   **Journal:** Der Journaldruck ist für alle Dokumente gleich. Er wird ausführlich zu den Aufträgen erklärt.
    *   Verkauf, "Journal" auf Seite C-742
*   **AB Lieferant:** In diesem Dialog erfassen und prüfen Sie die Auftragsbestätigungen (AB) Ihrer Lieferanten.
    *   ⇨ "AB-Lieferant" auf Seite D-197
*   **Auftragsbestätigung:**
    *   **Preiskontrolle:** In diesem Dialog prüfen Sie die Auftragsbestätigungen Ihrer Lieferanten und korrigieren ggf. Preise.
        *   ⇨ "Auftragsbestätigung" auf Seite D-204
    *   **Elektr. Preiskontrolle:** In diesem Dialog prüfen Sie die Preise und Referenzen in elektronisch übermittelten Auftragsbestätigungen.
        *   ⇨ "Auftragsbestätigung" auf Seite D-204
*   **Mahnung:** In diesem Dialog erfassen Sie Mahnungen für ausstehende Lieferungen.
    *   ⇨ "Mahnung" auf Seite D-225
*   **Wareneingang**
    *   **Wareneingang:** In diesem Dialog erfassen Sie Wareneingänge zu Bestellungen und Lagerbestellungen.
        *   ⇨ "Wareneingang" auf Seite D-227
    *   **Eingangskontrolle:** In diesem Dialog prüfen Sie die Vollständigkeit der Wareneingänge.
        *   ⇨ "Eingangskontrolle" auf Seite D-241
*   **Rechnung:**
    *   **Rechnungskontrolle:** In diesem Dialog prüfen Sie die Rechnungen Ihrer Lieferanten und korrigieren ggf. die Preise.
        *   ⇨ "Rechnungskontrolle - Bestellungen" auf Seite D-248
    *   **Elektr. Rechnungskontrolle:** In diesem Dialog prüfen Sie die Preise und die Referenzen in elektronisch übermittelten Rechnungen.
        *   ⇨ "Elektronische Rechnungskontrolle" auf Seite D-256
*   **FiBu-Übergabe:** Die FiBu-Übergabe ist für alle Dokumente gleich. Sie wird am Beispiel Auftrag erklärt.
    *   ⇨ Verkauf, "FiBu-Übergabe" auf Seite C-695
*   **Übergabe Archiv:** Die Archivübergabe ist für alle Dokumente gleich. Sie wird ausführlich zu den Aufträgen erklärt.
    *   Verkauf, "Übergabe Archiv" auf Seite C-702
*   **Suche:** Die Suche ist für alle Dokumente gleich. Sie wird ausführlich zu den Aufträgen erklärt.
    *   Verkauf, "Dokument suchen" auf Seite C-534
*   **Basisglasverrechnung:** Hier werden interne Verrechnungen von Profit Centern verwaltet. Die Basisglasverrechnung ist nur kundenspezifisch freigeschaltet.

### Bestellung (Dokumentenverwaltung)

`Dokumente > Bestellung > Bestellung`

[Image: Screenshot of the order document management dialog.]
**Abb. D-118**: Dokumentenverwaltung – Bestellung

In diesem Dialog erfassen und bearbeiten Sie Bestellungen.
⇨ Tutorial, "Manuelle Bestellung" auf Seite D-79

Der Dialog `Dokumentenverwaltung` und die zugehörigen Menüs sind für alle Dokumentenarten gleich. Er wird am Beispiel Auftrag beschrieben.
*   ⇨ Verkauf, "Dokument - Kopfdaten" auf Seite C-424
*   Verkauf, "Dokument - Positionen" auf Seite C-461

> **Bestellung erfassen**
> Die Bestellungen erfassen Sie auf die gleiche Weise wie einen Auftrag. Achten Sie dabei darauf, dass Sie den richtigen Dokumententyp auswählen:
> *   **Lagerbestellung:** Mit dieser Einstellung bestellen Sie Lagerprodukte. Mit dem Wareneingang werden die gelieferten Positionen automatisch auf Lager verbucht. In dieser Bestellung müssen Sie den Lagerartikel über die Lagersuche `<F3>` auswählen. Der Typ `Lagerbestellung` wird im Feld `Typ` angezeigt.
> *   **<k.A>:** Mit dieser Einstellung bestellen Sie alle Produkte, die nicht über das Lager verbucht werden.
>     *   ⇨ Verkauf, "Typ" auf Seite C-429
>     *   ⇨ Tutorial, "Unabhängige Bestellung erfassen" auf Seite D-81

Wenn Sie eine Lagerbestellung mit Produkten erfassen, die nicht als Lagerartikel geführt werden, kann der Wareneingang für diese Produkte nicht automatisch ins Lager verbucht werden. Eine entsprechende Meldung weist Sie beim Erfassen der Bestellung darauf hin.

> **Positionen ohne Lagerkennzeichen**
> Wenn Sie Lagerbestellungen mit Positionen erfassen, die nicht als Lagerartikel geführt werden, werden diese im Wareneingang nicht angezeigt. Sie können in den Firmendaten die entsprechende Option aktivieren.
>
> ⇨ Stammdaten, "Pos. ohne Lagerkennz. im WE anzeigen bei Lagerbestell." auf Seite B-972

### Nachbestellung

`Dokumente > Bestellung > Nachbestellung`

[Image: Screenshot of the reorder dialog showing a list of items reported as broken.]
**Abb. D-119**: Nachbestellung

In diesem Dialog verwalten Sie Aufträge mit Bestellteilen, die aus der Produktion als Bruch gemeldet sind. Sie können die Bestellteile nachbestellen, reklamieren, verrechnen oder die Auftragsmenge reduzieren.

**Selektion**

*   **Auftrag von, bis**: Einschränkung der Suche auf einen Auftrag oder eine Folge von Aufträgen.
*   **Liefertermin von, bis**: Einschränkung der Suche auf einen bestimmten Liefertermin oder eine Reihe von Lieferterminen.

**Dokumente**

In der Übersicht werden alle Aufträge mit Bruchscheiben angezeigt, die den Suchkriterien entsprechen.

*   **Auftrag**: Auftragsnummer.
*   **Auftragsposition**: Positionsnummer aus dem Auftrag.
*   **Lieferdatum**: Lieferdatum aus dem Auftragskopf.
*   **Bestellung**: Bestellnummer.
*   **Bestellposition**: Positionsnummer aus der Bestellung.
*   **Lieferant**: Name des Lieferanten aus der Bestellung.
*   **Produkt**: Nummer und Bezeichnung des Produkts.
*   **Auftragsmenge**: Menge aus dem Auftrag.
*   **Bestellmenge**: Menge, die bestellt ist.
*   **Bruchmenge**: Menge, die als Bruch gemeldet ist.
*   **Rückmeldedatum**: Datum der Bruchmeldung.
*   **Aktion**: Auswahl der Aktion:
    *   **Nachbestellung**: Die Bestellung wird erstellt und in den ausgewählten Nummernverwalter gestellt.
    *   **Reklamation**: Für die Bestellteile wird eine Reklamation erstellt. Wenn diese Option gewählt wird, können Reklamationsgrund und -verursacher angegeben werden.
    *   **wertmäßige Buchung**: Die Bestellung wird mit einer negativen Positionsmenge erstellt. Damit wird die Bruchmenge ausgebucht und der Wert der Bruchmenge mit dem Wert des Auftrags verrechnet.
    *   **Auftragsmenge reduzieren**: Der Ursprungsauftrag wird um die Bruchmenge reduziert. Damit wird eine Nachbestellung ausgeschlossen.
*   **Reklamationsgrund**: Der Reklamationsgrund wird nur angegeben, wenn als Aktion `Reklamation` gewählt ist.
*   **Reklamationsverursacher**: Der Reklamationsverursacher wird nur angegeben, wenn als Aktion `Reklamation` gewählt ist.
*   **Bemerkung**: Sie können eine Bemerkung eintragen, z. B. Absprachen, die mit dieser Nachbestellung oder Reklamation verbunden sind.
*   **Etikett**: Nummer des Etiketts aus der Produktion. Die Nummer kann nicht geändert werden.

**Ziel**

*   **Nummernverwalter**: Nummernverwalter, in den die Nachbestellungen gestellt werden sollen.

### Export (EDI)

`Dokumente > Bestellung > Export`

**Zu Dialogbeschreibung:**
*   ⇨ Fremddokumentenverwaltung
*   ⇨ Nummernverwalter kopieren

In diesem Dialog können Sie Bestellungen exportieren, um Sie über die EDI-Schnittstelle an den betreffenden Lieferanten zu übertragen.
⇨ Tutorial, “Datenexport/-import (EDI)" auf Seite D-177

> **Voraussetzung**
> Die Parameter für die Schnittstelle müssen für jeden einzelnen Lieferanten/Kunden festgelegt werden, mit dem Dokumente über die Fremdschnittstelle ausgetauscht werden sollen. Diese Parameter werden im Menü `Stammdaten > B2B` eingestellt.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menü Funktionen" auf Seite D-194
*   "Export - Export" auf Seite D-195
*   "Export - Pool" auf Seite D-196

### Menü Funktionen

`Dokumente > Bestellung > Export > Menü Funktionen`

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Dialog Export zu schließen.

Das Menü ist in folgende Gruppen gegliedert:
*   Gruppe Bearbeiten
*   Gruppe Dokument
*   Gruppe Dokumentenkopie

**Gruppe Bearbeiten**

*   **Kopieren:** Öffnet den Dialog `Nummernverwalter kopieren`, um einen neuen Nummernverwalter zu erstellen.
    *   ⇨ Verkauf, "Nummernverwalter kopieren" auf Seite C-649
*   **Statusänderung:** Öffnet den Dialog `Statusänderung`, um den Status manuell umzusetzen und den Nummernverwalter zu ändern.
    *   ⇨ Verkauf, "Statusänderung” auf Seite C-566

**Gruppe Dokument**

*   **Dokument anzeigen:** Öffnet den Dialog `Dokumentenansicht` zu einer Vorschau auf den Druck.
    *   Verkauf, "Reklamationen" auf Seite C-605
*   **Historie:** Öffnet eine Übersicht über die Statusänderungen des markierten Dokuments.
    *   Verkauf, "Historie" auf Seite C-564
*   **Dokumentendaten:** Öffnet den Dialog `Dokumentendaten`, um ggf. die Termine und den Status zu korrigieren.
    *   Verkauf, "Dokumentendaten" auf Seite C-755
*   **Dokumentenerfassung:** Öffnet den Dialog `Dokumentenverwaltung`, in dem Sie Dokumente anlegen oder ändern können.
    *   ⇨ Verkauf, "Dokumentenverwaltung" auf Seite C-415

**Gruppe Dokumentenkopie**

*   **Dokumente kopieren:** Öffnet den Dialog `Dokumente kopieren`, um ein Dokument in den gleichen oder einen anderen Dokumententyp zu kopieren.
    *   Verkauf, "Dokumente kopieren" auf Seite C-543
*   **Teillieferung:** Öffnet den Dialog `Dokumente kopieren`, um eine Teillieferung zu erfassen.
    *   Verkauf, "Dokumente kopieren" auf Seite C-543

### Export - Export

`Dokumente > Bestellung > Export > Register Export`

[Image: Screenshot of the 'Export - Export' register showing a list of documents for export.]
**Abb. D-120**: Export – Export

In diesem Register exportieren Sie die Bestellungen. Die Daten werden in eine ASC-Datei geschrieben. Diese wird im festgelegten Verzeichnis abgelegt. Die Datei wird danach über die EDI-Schnittstelle zum Lieferanten übertragen.

Die Einstellungen für den Export werden pro Lieferant im Modul `Stammdaten > B2B` festgelegt.
⇨ Tutorial, "Datenexport/-import (EDI)" auf Seite D-177

**Selektion nach**

*   **Mitarbeiter**: Name des Mitarbeiters, der sich in A+W Business angemeldet hat.
*   **Nummernverwalter**: Auswahl des Nummernverwalters, auf den der Dialog Export zugreifen soll.
*   **[Logbuch]**: Schaltfläche zum Öffnen des Systemlogbuchs.

**Dokumente**

Liste aller Dokumente, die im gewählten Nummernverwalter stehen. Sie sollen über die Schnittstellen an den Lieferanten gesendet werden.

*   **Nummer:** Nummer des Dokuments.
*   **Nummer Kunde/Lief.:** Nummer des Kunden oder Lieferanten.
*   **Kunde/Lieferant:** Name des Kunden oder Lieferanten.
*   **Status:** Status des Dokuments.
*   **Datum Erfassung:** Datum, an dem das Dokument erfasst wurde.
*   **Datum Lieferung:** Lieferdatum
*   **Datum AB:** Datum der Auftragsbestätigung
*   **Sperr-KZ:** Kennzeichen, ob das Dokument gesperrt ist. Das Sperrkennzeichen wird bei Bestellungen selten gesetzt.

### Export - Pool

`Dokumente > Bestellung > Export > Register Pool`

[Image: Screenshot of the 'Export - Pool' register.]
**Abb. D-121**: Export - Pool

In diesem Register können Sie die aufgelisteten Bestellungen elektronisch über die EDI-Schnittstelle übergeben.

**Übertragungs-Pool**

In der Übersicht werden alle Bestellungen aufgelistet, die elektronisch übergeben werden sollen.

*   **[Löschen]**: Die Schaltfläche ist nur freigeschaltet, wenn ein Fehler bei der Übertragung festgestellt wurde. Sie können dann einen Eintrag aus dem Übertragungspool löschen.
*   **[Aktivieren]**: Die Schaltfläche ist nur freigeschaltet, wenn ein Fehler bei der Übertragung festgestellt wurde. Wenn ein Fehler festgestellt wurde, können Sie die Daten korrigieren und erneut zur Übertragung übergeben. Sie lösen die Übertragung mit [Aktivieren] aus.
*   **[Abfragen]**: Mit dieser Schaltfläche aktualisieren Sie die Anzeige, um den Übertragungsstatus zu prüfen.

## AB-Lieferant

`Dokumente > Bestellung > AB Lieferant`

In diesem Dialog können Sie die Auftragsbestätigung erfassen, die Ihr Lieferant zu einer Bestellung gesendet hat. Außerdem können Sie den zugehörigen Wareneingang erfassen und/oder die Termine für Bestellungen und Lieferungen prüfen und ggf. korrigieren.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menü Optionen" auf Seite D-197
*   "AB-Lieferant - Dokumente" auf Seite D-198
*   "AB-Lieferant - Positionen" auf Seite D-202
*   "AB-Lieferant - Liefertermine ändern" auf Seite D-203

**Zu Dialogbeschreibung:**
*   ⇨ Einstellungen (ID)

### Menü Optionen

`Dokumente > Bestellung > AB Lieferant > Menü Optionen`

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

Folgende Einträge werden angezeigt:
*   **Lagerbuchungsdatum = Lieferdatum:** Als Buchungsdatum wird automatisch das Lieferdatum aus der Bestellung übernommen. Wenn die Option deaktiviert ist, wird standardmäßig das Tagesdatum übernommen.
*   **AB-Nummer prüfen:** Mit dieser Einstellung wird eine Meldung angezeigt, wenn die Nummer der Auftragsbestätigung durch den Lieferanten nicht eingegeben ist.
*   **Identnummernvergabe:** Diese Einstellung wird für den Wareneingang von Kisten und Lagerplatten benötigt.
    *   **Manuell:** Mit dieser Option müssen Sie die ID manuell vergeben. Die Checkbox `Identnummer(n) vergeben` im Bereich Optionen wird freigeschaltet.
        *   ⇨ "Optionen" auf Seite D-199
    *   **Automatisch:** Mit dieser Option wird die ID automatisch vergeben. Dazu kann eine Vorgabe festgelegt werden. Wenn die Option nicht aktiviert ist, müssen Sie die ID manuell eingeben.
    *   **Einstellungen:** Öffnet den Dialog `Einstellungen`, in dem Sie die Vorgabe für die automatische Vergabe von IDs festlegen.
        *   ⇨ "Einstellungen (ID)" auf Seite D-240

### AB-Lieferant – Dokumente

`Dokumente > Bestellung > AB Lieferant > Register Dokumente`

[Image: Screenshot of the 'AB Lieferant - Dokumente' register.]
**Abb. D-122**: AB-Lieferant – Dokumente

In diesem Register können Sie eine Auftragsbestätigung des Lieferanten und/oder den zugehörigen Wareneingang erfassen. Außerdem können Sie die Termine für Bestellungen und Lieferungen prüfen und ggf. korrigieren.

Alle Daten, die Sie in diesem Register eintragen, gelten jeweils für alle Positionen, die in der Bestellübersicht aufgeführt sind. Wenn Sie die Daten zu einzelnen Positionen erfassen möchten, müssen Sie zum Register `Positionen` wechseln.
⇨ Tutorial, "Lieferanten-AB" auf Seite D-87

**Dokumente**

Mit der Wahl der Option legen Sie fest, zu welcher Dokumentenart Sie die Auftragsbestätigung erfassen möchten. Mit der Lupe können Sie nach der Bestellung oder dem Auftrag suchen.
*   **Bestellnummer:** Auswahl einer Bestellung. Das Eingabefeld für die Bestellnummer ist freigeschaltet.
*   **Auftragsnummer:** Auswahl eines Kundenauftrags, aus dem eine Bestellung erzeugt wurde. Das Eingabefeld für die Auftragsnummer ist freigeschaltet.

**Optionen**

*   **Auftrags-NV füllen**: Wenn Sie eine Auftragsbestätigung Ihres Lieferanten und ggf. auch den zugehörigen Wareneingang buchen, kann der zugehörige (Kunden-) Auftrag automatisch in einen anderen Nummernverwalter gestellt werden.
    *   ✅ Der referenzierte (Kunden-) Auftrag wird nicht in einen anderen Nummernverwalter gestellt.
    *   ✅ Der referenzierte (Kunden-) Auftrag wird in den ausgewählten Nummernverwalter gestellt.
*   **Bestell-NV füllen**: Wenn Sie eine Auftragsbestätigung Ihres Lieferanten und ggf. auch den zugehörigen Wareneingang buchen, kann die zugehörige Bestellung automatisch in einen anderen Nummernverwalter gestellt werden.
    *   ✅ Die Bestellung wird nicht in einen anderen Nummernverwalter gestellt.
    *   ✅ Die Bestellung wird in den ausgewählten Nummernverwalter gestellt.
*   **Wareneingang buchen**: Sie können den kompletten Wareneingang erfassen, wenn Ihr Lieferant die Ware zusammen mit der AB geliefert hat.
    *   ✅ Der Wareneingang wird nicht erfasst.
    *   ✅ Der Wareneingang wird als komplett verbucht. Wenn in der Lieferung Kisten enthalten sind, müssen Sie die Einstellungen für die Kisten-ID prüfen.

> **Wareneingang teilweise erfassen**
> Den vollständigen Wareneingang für einzelne Positionen können Sie im Register `Positionen` erfassen. Wenn Sie den teilweisen Wareneingang einer Position erfassen möchten, müssen Sie zum Dialog `Wareneingang` wechseln.
> ⇨ "Wareneingang (Dialog)" auf Seite D-227

*   **Identnummer(n) vergeben**: Die Checkbox wird über die Einstellung zur Identnummernvergabe aktiviert oder deaktiviert. Identnummern (IDs) werden in der Regel für Kisten vergeben. Sie können eine Vorgabe für die ID festlegen, mit der der Wareneingang im Lager verbucht werden soll.
    *   ✅ Die Checkbox ist nur freigeschaltet, wenn Sie im Menü `Optionen` die Einstellung `Manuell` gewählt haben.
    *   ✅ Die Checkbox ist deaktiviert, wenn Sie im Menü `Optionen` die Einstellung `Manuell` gewählt haben. Die ID muss manuell eingegeben werden.
    *   ✅ Die Checkbox ist aktiviert, wenn Sie im Menü `Optionen` die Einstellung `Automatisch` gewählt haben.
        *   ⇨ "Einstellungen (ID)" auf Seite D-240

**Bestelldaten**

*   **Lieferant**: Name des Lieferanten aus der Bestellung oder dem Kundenauftrag.
*   **Status**: Status des ausgewählten Dokuments.
*   **Gesamtstückzahl**: Stückzahl aller Positionen insgesamt im ausgewählten Dokument.
*   **Bestätigter Anliefertermin**: Termin der Lieferung durch den Lieferanten. Das Datum ist aus der Bestellung übernommen. Sie können es ggf. ändern. Ein geänderter Termin wird in die Bestellung und ggf. in den referenzierten Auftrag zurückgeschrieben.
    *   ⇨ "AB-Lieferant - Liefertermine ändern" auf Seite D-203
*   **Teilliefertermin**: Liefertermin, der in der Auftragsbestätigung durch den Lieferanten gemeldet wird.
*   **AB-Nummer**: Nummer der Auftragsbestätigung, die der Lieferant gesendet hat. Diese Nummer wird in alle Positionen eingetragen, die in der Bestellübersicht angezeigt werden. Wenn die AB-Nummer nur für eine Position gelten soll, müssen Sie zum Register `Positionen` wechseln.
    *   "AB-Lieferant - Positionen" auf Seite D-202

**Auftragsdaten**

Die Daten in diesem Bereich werden nur angezeigt, wenn ein Auftrag oder eine Bestellung zu einem Auftrag ausgewählt ist. Bei einer Lagerbestellung (ohne Auftrag) bleiben die Felder leer.

*   **Kunde**: Name des Kunden, für den die Bestellung erzeugt wurde.
*   **Status**: Status des Kundenauftrags.
*   **Gesamtstückzahl**: Stückzahl aller Positionen insgesamt im Kundenauftrag.
*   **Anliefertermin bei Kunden**: Termin der Anlieferung beim Kunden. Das Datum wird aus dem Auftrag übernommen. Sie können es ggf. ändern. Ein geänderter Termin wird in die Bestellung und ggf. in den referenzierten Auftrag zurückgeschrieben.
    *   ⇨ Verkauf, "Kundenbenachrichtigung (Lieferterminkontrolle)" auf Seite C-577
    *   ⇨ Tutorial, "Liefertermine ändern und Kunden benachrichtigen" auf Seite D-102
    *   ⇨ "AB-Lieferant - Liefertermine ändern" auf Seite D-203
*   **Geplant**: Ursprünglich geplanter Anliefertermin beim Kunden.
*   **Versandtag**: Termin, an dem die Lieferung an den Kunden gesendet wird. In der Regel ist dieser Termin mit dem Termin der Anlieferung identisch. Nur wenn die Lieferung länger als einen Tag benötigt, muss der Versandtag vor dem Anliefertermin liegen.
*   **Tour**: Auswahl der Tour, mit der die Lieferung an den Kunden geht.

**Bestellpositionen**

Übersicht über alle Positionen der Bestellung. Wenn die Bestellung aus einem Kundenauftrag erzeugt wurde, können die Bestellpositionen zugleich die Positionen des referenzierten Auftrags sein.

*   **Pos. Nr.:** Nummer der Bestellposition. Bei einer Kundenbestellung kann dies auch die Positionsnummer aus dem Auftrag sein.
*   **Artikelbezeichnung:** Nummer und Bezeichnung der bestellten Position.
*   **Menge:** Menge der bestellten Position.
*   **Breite / Höhe:** Maße der bestellten Position.
*   **Lieferanten-AB:** Nummer der Auftragsbestätigung des Lieferanten. Wenn Sie die AB-Nummer für die gesamte Bestellung erfasst haben, wird für alle Positionen dieselbe Nummer angezeigt.
*   **Teilliefertermin:** Liefertermin für die Teillieferung.
*   **Pr./PE:** EK-Preis pro Preiseinheit der bestellten Position.
*   **Pr./PE Gesamt:** Gesamtpreis pro Preiseinheit der bestellten Position.
*   **Liste/Schlüssel:** Preisliste und Preisschlüssel, die für den zugrundegelegten Einkaufspreis (EK) gelten.
*   **Rabatt:** Rabatt, der auf den EK gewährt wird.
*   **Netto/Pos:** Betrag der Position ohne Rabatt und/oder Zuschläge.
*   **Netto/Pos Gesamt:** Betrag aller Positionen der Bestellung ohne Rabatt und/oder Zuschläge.
*   **Preiseinheit Anzahl:** Menge in der angezeigten Preiseinheit.
*   **Preiseinheit:** Preiseinheit für den angezeigten Preis.
*   **Stückpreis:** Stückpreis der markierten Position inklusive aller Komponenten. Er wird über die Preiseinheit, die Zuschläge und Rabatte errechnet.
*   **Auftrag:** Auftragsnummer.
*   **Bezeichnung:** Produktbezeichnung aus dem referenzierten Auftrag. Sie können in der Bestellung eine abweichende Lieferantenbezeichnung angeben.

### AB-Lieferant - Positionen

`Dokumente > Bestellung > AB Lieferant > Register Positionen`

[Image: Screenshot of the 'AB Lieferant - Positionen' register.]
**Abb. D-123**: AB-Lieferant - Positionen

In diesem Register können Sie die gleichen Daten erfassen wie im Register `Dokumente`. Die erfassten Daten beziehen sich jeweils nur auf die angegebenen Positionen.

Die Felder in diesem Register sind ausführlich zum Register `Dokumente` beschrieben.
"AB-Lieferant - Dokumente" auf Seite D-198

**Positionen von - bis**: Positionsnummern, zu denen Sie eine AB-Nummer und/oder einen Wareneingang verbuchen. Dabei gelten die Positionen als vollständig geliefert. Die Auftragsnummer wird in der Bestellübersicht nur für die eingetragenen Positionen angezeigt.

Wenn Sie zu einzelnen Positionen Teillieferungen/-wareneingänge verbuchen wollen, müssen Sie zum Dialog `Wareneingang` wechseln.
*   ⇨ Tutorial, "Wareneingang erfassen" auf Seite D-127
*   ⇨ "Wareneingang (Dialog)" auf Seite D-227

### AB-Lieferant - Liefertermine ändern

`Dokumente > Bestellung > AB Lieferant > Register Liefertermine ändern`

[Image: Screenshot of the 'AB Lieferant - Liefertermine ändern' register.]
**Abb. D-124**: AB-Lieferant - Liefertermine ändern

In diesem Register können Sie die Termine für die Lieferung durch den Lieferanten anpassen.

Die Felder in diesem Register sind ausführlich zum Register `Dokumente` beschrieben.
"AB-Lieferant - Dokumente" auf Seite D-198

## Auftragsbestätigung

`Dokumente > Bestellung > Auftragsbestätigung > Preiskontrolle`

Sie können die Preise Ihrer Lieferanten prüfen, bevor Sie eine Auftragsbestätigung akzeptieren. Wenn ein Lieferant die vereinbarten Termine nicht einhält, können Sie eine Mahnung an ihn senden.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Preiskontrolle" auf Seite D-205
*   "Elektronische Preiskontrolle" auf Seite D-213
*   "Auswahl (Prod. Nr. für Ausgleichspos.)" auf Seite D-220
*   "Einstellungen für Xternal" auf Seite D-221
*   "Positionen manuell zuordnen" auf Seite D-221
*   "Fußzuschläge/-rabatte verteilen" auf Seite D-222
*   "Filtereinstellungen" auf Seite D-223
*   "Mahnung" auf Seite D-225

### Preiskontrolle

`Dokumente > Bestellung > Auftragsbestätigung > Preiskontrolle`

**Zu Dialogbeschreibung:**
*   ⇨ Elektronische Preiskontrolle
*   ⇨ Rechnungsdatum
*   ⇨ Auswahl (Prod. Nr. für Ausgleichspos.)
*   Positionen manuell zuordnen
*   ⇨ Fußzuschläge/-rabatte verteilen
*   ⇨ Filtereinstellungen

Sie können die von Ihren Lieferanten bestätigten Preise prüfen und ggf. korrigieren.
⇨ Tutorial, "AB erfassen und Preise prüfen" auf Seite D-93

> **Sammelrechnung**
> Wenn Ihr Lieferant mehrere Bestellungen in einer Sammelbestätigung zusammengefasst hat, kann diese nur geprüft und akzeptiert werden, wenn in allen Bestellungen derselbe MwSt.-Satz und dieselbe Währung angegeben sind.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menü Funktionen" auf Seite D-205
*   "Menü Optionen" auf Seite D-206
*   "Preiskontrolle - Bestellungen" auf Seite D-207
*   "Preiskontrolle - Position" auf Seite D-210
*   "Preiskontrolle - Stückliste" auf Seite D-212

#### Menü Funktionen

`Dokumente > Bestellung > Auftragsbestätigung > Preiskontrolle > Menü Funktionen`

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Preiskontrolle zu schließen.

Folgende Einträge werden angezeigt:
*   **Teillieferungen erstellen:** Öffnet den Dialog `Dokumente kopieren`, um eine Teillieferung zu erfassen.
    *   Verkauf, "Dokumente kopieren" auf Seite C-543
*   **Anlieferpauschale einfügen:** Die Lieferpauschale wird automatisch als Position im Register `Positionen` eingefügt. Wenn in der Bestellung bereits eine Lieferpauschale enthalten ist, wird die Option nicht ausgeführt.
*   **Bestellerfassung öffnen:** Während der Preiskontrolle sind alle aufgelisteten Bestellungen für die Bearbeitung (durch andere Mitarbeiter) gesperrt. Mit dieser Funktion öffnen Sie den Dialog `Dokumentenverwaltung`, um eine der angezeigten Bestellungen zu bearbeiten. Geänderte Werte werden in die Preiskontrolle übernommen.
    *   ⇨ Verkauf, "Dokument - Kopfdaten" auf Seite C-424
*   **Bestelldaten aktualisieren:** Mit dieser Funktion werden die geänderte Werte sofort in die Bestellung zurückgeschrieben.

#### Menü Optionen

`Dokumente > Bestellung > Auftragsbestätigung > Preiskontrolle > Menü Optionen`

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

In diesem Menü finden Sie folgende Gruppen:
*   Gruppe Standard
*   Gruppe Verhalten
*   Gruppe Einstellungen
*   Gruppe Xternal

**Gruppe Standard**

*   **NettoMwst.:** Nettobeträge werden inkl. Mwst. angezeigt.
*   **BruttoMwst.:** Bruttobeträge werden inkl. Mwst. angezeigt.
*   **Netto:** Nettobeträge werden ohne Mwst. angezeigt.

**Gruppe Verhalten**

*   **Schnellerfassung:** Mit dieser Option springt der Cursor nach der Eingabe einer Bestellnummer in das Feld Auftragssumme. Diese Einstellung wird benutzerbezogen gespeichert.
*   **Einschränkung bei Rech.dat.:** Öffnet den Dialog `Rechnungsdatum`, um eine Abweichung in Tagen festzulegen.
    *   ⇨ "Rechnungsdatum" auf Seite D-255
*   **Ziel-NV füllen:** Schaltet die Felder im Bereich Ziel-Nummernverwalter frei, um einen Mitarbeiter und den zugehörigen Nummernverwalter auszuwählen.

**Gruppe Einstellungen**

*   **Rabatt einfrieren:** Der Rabatt wird fixiert. Diese Option sollten Sie aktivieren, wenn Sie neue Rabatte festgelegt haben, in den alten Bestellungen aber die alten Rabatte angewendet werden sollen. Die Preise werden dann nach der Preiskontrolle nicht neu errechnet.
*   **Auftragskosten nicht in Statistik korrigieren:** Die EK-Preise im referenzierten Auftrag werden nur korrigiert, solange der Auftrag noch in der Hauptdatenbank vorhanden ist und nicht an die Statistik übergeben wurde.
*   **Hinweis auf Lieferterminüberschreitung:** Wenn der bestätigte Liefertermin später als der gewünschte Liefertermin der Bestellung ist, wird eine Meldung angezeigt.

**Gruppe Xternal**
*   **Xternal-XML-Datei erstellen:** Diese Option ist nur kundenspezifisch aktiviert.
*   **Einstellungen für Xternal:** Öffnet den Dialog `Einstellungen`, um Vorgaben für den XML-Export festzulegen. Diese Funktion ist nur freigeschaltet, wenn die Option `Xternal-XML-Datei erstellen` aktiviert ist.

### Preiskontrolle – Bestellungen

`Dokumente > Bestellung > Auftragsbestätigung > Preiskontrolle > Register Bestellungen`

[Image: Screenshot of the 'Preiskontrolle - Bestellungen' register.]
**Abb. D-125**: Preiskontrolle – Bestellungen

In diesem Register wählen Sie eine Bestellung aus, um die Preise der Auftragsbestätigung zu prüfen. Die Daten werden erst angezeigt, wenn die Felder zur Bestellnummer oder zum Nummernverwalter im Bereich `Bestelldaten` gefüllt sind und der Cursor in einem anderen Feld steht.
⇨ Tutorial, "AB erfassen und Preise prüfen" auf Seite D-93

**AB-Daten**

*   **AB-Nummer**: Pflichtfeld. Sie müssen die Nummer der Auftragsbestätigung des Lieferanten eingeben.
*   **Bestätigter Anliefertermin**: Pflichtfeld. Termin, der auf der Auftragsbestätigung angegeben ist. Sie können das Datum über den Kalender auswählen oder manuell eingeben.

**Bestelldaten**

Mit der Wahl der Option werden die zugehörigen Felder freigeschaltet, um die Bestellung(en) auszuwählen, zu denen die Preise geprüft werden sollen.

*   **Bestellnummer, bis:** Wenn Sie in beiden Feldern dieselbe Nummer eintragen, wird nur diese eine Bestellung eingelesen. Wenn zu einer Auftragsbestätigung mehrere Bestellungen gehören, können Sie nacheinander mehrere Bestellnummern eingeben und in die Übersicht übernehmen. Dazu müssen alle Bestellungen zum selben Lieferanten gehören und denselben MwSt.-Satz haben.
*   **Nummernverwalter:** Wenn Sie einen Nummernverwalter ausgewählt haben, werden im Bereich `Bestellungen` alle Bestellungen aufgelistet, die in diesem Nummernverwalter stehen.

**Summen**

Erst wenn Sie den Betrag aus der Auftragsbestätigung des Lieferanten eingegeben und mit `[Ausführen]` bestätigt haben, können Sie zu einem der anderen Register wechseln.

*   **AB-Summe/Mwst.**: Pflichtfeld. Gesamtbetrag der bestätigten Lieferung und der Mehrwertsteuer. Der Betrag der Mehrwertsteuer wird nicht angezeigt, wenn der Modus `Netto` ausgewählt ist.
*   **Modus**: Mit der Wahl des Modus wird die Mehrwertsteuer angezeigt oder ausgeblendet. Den Standard-Modus können Sie im Menü `Optionen > Gruppe Standard` festlegen.
    *   **Netto mit Mwst.:** Der Gesamtbetrag wird als Nettobetrag gewertet, der Betrag der Mehrwertsteuer wird angezeigt.
    *   **Brutto mit Mwst.:** Der Gesamtbetrag wird als Bruttobetrag gewertet, der Betrag der Mehrwertsteuer wird angezeigt.
    *   **Netto:** Der Gesamtbetrag wird als Nettobetrag gewertet, der Betrag der Mehrwertsteuer wird nicht angezeigt.
*   **Währung**: Auswahl der Währung, wenn Sie mit mehreren Währungen arbeiten.
    In der Kombobox werden alle Währungen zur Auswahl angeboten, die in den Stammdaten hinterlegt sind. Mit der Auswahl einer anderen Währung als Euro werden in der Übersicht die Beträge für die Aufträge und die Mehrwertsteuer zusätzlich in der gewählten Währung angezeigt.
    ⇨ Stammdaten, "Währungen" auf Seite B-464
*   **Kurs**: Wenn Sie mit mehreren Währungen arbeiten, wird der Wechselkurs angezeigt, der in den Stammdaten hinterlegt ist. Er kann überschrieben werden. Wenn Sie nur mit Euro arbeiten, muss in diesem Feld `1` stehen.
    > **Wechselkurs fixieren**
    > Sie können pro Bestellung einen abweichenden Wechselkurs vereinbaren. Dieser wird automatisch zur Berechnung in der Preiskontrolle herangezogen. Sie können ihn nur überschreiben, wenn er in der Bestellung nicht fixiert ist.
    >
    > Verkauf, "Kurs fixiert für Rechnungsdruck" auf Seite C-440

**Ziel-Nummernverwalter**

Diese beiden Felder sind nur freigeschaltet, wenn die Option `Ziel-NV füllen` aktiviert ist.
⇨ "Menü Optionen" auf Seite D-206

*   **Mitarbeiter**: Name des Mitarbeiters, dem der Ziel-Nummernverwalter zugeordnet ist.
*   **Nummernverwalter**: Nummernverwalter, in den die Bestellungen nach der Prüfung gestellt werden sollen.

**Bestellungen**

In der Übersicht werden alle Bestellungen angezeigt, die sich im Nummernverwalter befinden. Wenn Sie im Bereich `Bestelldaten` über die Bestellnummern gefiltert haben, werden nur die entsprechenden Bestellungen angezeigt.
Die Spalten mit den Beträgen der Mehrwertsteuer und der Fremdwährung werden nur angezeigt, wenn ein Modus mit Mehrwertsteuer und/oder eine Fremdwährung ausgewählt ist.

*   **Summe**: Anzeige der Gesamtsumme und der Mehrwertsteuer der aufgelisteten Bestellungen.
*   **Zugrundeliegender Mwst-Satz**: Anzeige des Mehrwertsteuersatzes aus der Bestellung.
    *   Verkauf, "Steuersatz" auf Seite C-532

### Preiskontrolle – Position

`Dokumente > Bestellung > Auftragsbestätigung > Preiskontrolle > Register Position`

[Image: Screenshot of the 'Preiskontrolle - Position' register.]
**Abb. D-126**: Preiskontrolle – Position

In diesem Register werden die Preise der Bestellpositionen angezeigt.
Das Register wird nur angezeigt, wenn im Register `Bestellungen` die Pflichtfelder gefüllt sind und mit `[Ausführen]` bestätigt wurden.
⇨ Tutorial, "AB erfassen und Preise prüfen" auf Seite D-93

**Bestellpositionen**

In der Übersicht werden alle Positionen der Bestellung aufgeführt, zu der Sie die Preise und die Rechnungssumme kontrollieren.

*   **Bestell-Nr.:** Nummer, mit der die Bestellung in der Datenbank gespeichert ist.
*   **Pos:** Nummer der Bestellposition
*   **Artikel:** Bezeichnung der bestellten Position
*   **Breite / Höhe:** Maße der bestellten Position
*   **Euro-Netto:** Preis der Position in der Landeswährung (hier Euro). Wenn Sie mit einer anderen Währung arbeiten, ändert sich die Bezeichnung entsprechend. Wenn Sie mit zwei Währungen arbeiten, wird für die zweite Währung eine weitere Spalte mit dem entsprechenden Betrag angezeigt.
*   **Mwst.-Euro:** Betrag der Mehrwertsteuer in der Landeswährung (hier Euro). Die Spalte wird nicht angezeigt, wenn im Register `Bestellungen` die Option `Netto` gewählt ist. Für die Anzeige der Mehrwert-Steuer im Mehrwährungssystem gilt das gleiche wie für die Anzeige des Betrags.
*   **Stückl.genaue Eingabe:** In dieser Spalte wird angezeigt, ob Sie Preisdifferenzen auf der Ebene der Stücklisten-Komponenten oder der Positionen korrigiert haben.
    *   **Deaktiv:** Der Preis wurde nicht geändert oder der Preis der gesamten Position wurde geändert.
    *   **Aktiv:** Der Preis wurde an einer Stücklisten-Komponente geändert.
*   **Lieferant:** Nummer und Name des Lieferanten.
*   **Menge:** Bestellte Menge
*   **Kundenliefertermin:** Datum der Anlieferung beim Kunden.
*   **Auftr.Nr.:** Nummer des referenzierten Auftrags.

*   **Gesamtbetrag**: Anzeige der Summe der (eingegebenen) Positionsbeträge.
*   **Gesamtmenge**: Summe der Positionsmengen.
*   **Differenz**: Anzeige der Differenz zwischen der Rechnungssumme im Register `Bestellungen` und der Summe der (eingegebenen) Positionsbeträge. In diesem Fall kann der Preis nicht bestätigt werden, bevor Sie die Preise der Positionen oder der Stücklisten geändert haben.

> **Differenz**
> Eine Differenz wird auch angezeigt, wenn Sie im Register `Bestellungen` versehentlich eine falsche AB-Summe eingetragen haben oder der Wechselkurs nicht korrekt ist.

### Preiskontrolle – Stückliste

`Dokumente > Bestellung > Auftragsbestätigung > Preiskontrolle > Register Stückliste`

[Image: Screenshot of the 'Preiskontrolle - Stückliste' register.]
**Abb. D-127**: Preiskontrolle – Stückliste

In diesem Register können Sie sich den Preis einer Position auf der Ebene der Stückliste und der Stücklisten-Komponenten anzeigen lassen. Das Register ist nur aktiv, wenn im Register `Positionen` eine Position mit Stückliste markiert ist.
⇨ Tutorial, "AB erfassen und Preise prüfen" auf Seite D-93

**Stücklistenaufbau**

In diesem Feld wird die Stückliste der Position angezeigt, die im Register `Positionen` markiert ist.

**Preise**

Die Anzeige der Felder hängt davon ab, welche Stücklisten-Komponente markiert ist.
Sie können die Preise auf der Hauptebene oder an den Stücklisten-Komponenten korrigieren.
Sie können die Austauschzuschläge und Preise der einzelnen Komponenten ändern.

*   **Preis / PE**: Anzeige des Preises und der Preiseinheit aus der Bestellung.
*   **Rabatt**: Anzeige des Rabattes aus der Bestellung. Der Wert kann nicht geändert werden.
*   **Netto / Positionsmenge**: Anzeige des Preises und der Menge aus der Bestellung, wenn die Hauptposition markiert ist. Der Wert kann nicht geändert werden.
*   **Netto / Stücklistenmenge**: Anzeige des Preises und der Menge aus der Bestellung, wenn eine Komponente markiert ist. Der Wert kann nicht geändert werden.
*   **Netto ges.**: Anzeige des Positions-Preises aus der Bestellung, wenn die Hauptposition markiert ist. Der Wert kann geändert werden.
*   **Netto ges. / Pos. Menge**: Anzeige des Komponenten-Preises und der Menge, wenn eine Komponente markiert ist. Der Wert kann geändert werden.
*   **Gesamtsumme**: Anzeige des Komponenten-Preises pro Position, wenn eine Komponente markiert ist. Der Wert kann geändert werden.

### Elektronische Preiskontrolle

`Dokumente > Bestellung > Auftragsbestätigung > Elektr. Preiskontrolle`

**Zu Dialogbeschreibung:**
*   ⇨ Auswahl (Prod. Nr. für Ausgleichspos.)
*   Positionen manuell zuordnen
*   Fußzuschläge/-rabatte verteilen
*   ⇨ Filtereinstellungen

Wenn Sie Auftragsbestätigungen Ihrer Lieferanten elektronisch (openTRANS-Format) erhalten, können Sie die Zuordnung der Positionen zu Ihren Bestellungen, die Preise und Termine prüfen. Dazu steht Ihnen der Dialog `Auftragsbestätigung - Elektr. Preiskontrolle` zur Verfügung.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menü Funktionen" auf Seite D-214
*   "Menü Optionen" auf Seite D-214
*   "Elektronische Preiskontrolle - Dokumentenimport" auf Seite D-216
*   "Elektronische Preiskontrolle - Positionsübersicht" auf Seite D-219

#### Menü Funktionen

`Dokumente > Bestellung > Auftragsbestätigung > Elektr. Preiskontrolle > Menü Funktionen`

Über dieses Menü können Sie andere Dialoge öffnen, ohne die elektronische Preiskontrolle zu schließen.

Folgende Einträge werden angezeigt:
*   **Anlieferpauschale einfügen:** Die Lieferpauschale wird automatisch als Position im Register `Positionen` eingefügt. Wenn in der Bestellung bereits eine Lieferpauschale enthalten ist, wird die Option nicht ausgeführt.
*   **Bestellerfassung öffnen:** Während der Preiskontrolle sind alle aufgelisteten Bestellungen für die Bearbeitung (durch andere Mitarbeiter) gesperrt. Mit dieser Funktion können Sie den Dialog `Dokumentenverwaltung` öffnen, um eine der angezeigten Bestellungen zu bearbeiten. Geänderte Werte werden in die Preiskontrolle übernommen.
    *   Verkauf, "Dokument - Kopfdaten" auf Seite C-424
*   **Positionen manuell zuordnen:** Öffnet den Dialog `Positionen manuell zuordnen`, um Positionen des elektr. Dokuments den entsprechenden Positionen der Bestellung(en) zuzuordnen.
    *   ⇨ "Positionen manuell zuordnen" auf Seite D-221
*   **Fußzuschläge/-rabatte auf Bestellungen verteilen:** Öffnet den Dialog `Fußzuschläge/-rabatte auf Bestellungen verteilen`, um den Zuschlag/Rabatt aus dem elektr. Dokument auf die zugeordneten Bestellungen zu verteilen.
    *   ⇨ "Fußzuschläge/-rabatte verteilen" auf Seite D-222
*   **Manuelle Positionszuordnung aufheben:** Hebt die manuelle Zuordnung der markierten Rechnungs-/Bestellpositionen wieder auf.
*   **Alle Positionszuordnungen aufheben:** Hebt alle manuellen Zuordnungen von Rechnungs- und Bestellpositionen wieder auf.

#### Menü Optionen

`Dokumente > Bestellung > Auftragsbestätigung > Elektr. Preiskontrolle > Menü Optionen`

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

In diesem Menü finden Sie folgende Gruppen:
*   Gruppe Allgemein
*   Gruppe Einstellungen
*   Gruppe Xternal

**Gruppe Allgemein**

*   **Betragsdifferenzen akzeptieren:** Bei der elektronischen Preiskontrolle können Betragsdifferenzen, die durch Rundungen auftreten können, generell akzeptiert werden.
*   **Hinweis auf Betragsdiff./Ausgl.pos.:** Wenn Rundungsdifferenzen automatisch einer Ausgleichsposition zugeordnet wurden, wird ein Hinweis angezeigt.
*   **Rabatt einfrieren:** Mit dieser Option wird der Rabatt fixiert. Diese Option sollten Sie aktivieren, wenn Sie neue Rabatte festgelegt haben, in den alten Bestellungen aber die alten Rabatte angewendet werden sollen. Die Preise werden dann nach der Preiskontrolle nicht neu errechnet.
*   **Auftr.-EK nur korrigieren bis in Statistik:** Die Korrekturen des EK-Preises im referenzierten Auftrag werden nur durchgeführt, solange der Auftrag noch in der Hauptdatenbank vorhanden ist und nicht an die Statistik übergeben wurde.
*   **Prod.Nr. für Ausgleichspos.:** Öffnet den Dialog `Auswahl`, um eine Ausgleichposition für Rundungsdifferenzen auszuwählen.
    *   ⇨ "Auswahl (Prod. Nr. für Ausgleichspos.)" auf Seite D-220

**Gruppe Einstellungen**

*   **Hinweis auf Lieferterminüberschreitung:** Bei Überschreitung des geplanten Liefertermins wird eine Meldung angezeigt.
*   **Automatische Zuordnung unterdrücken:** Im Dialog `Positionen manuell zuordnen` können Sie die Checkbox für die automatische Zuordnung aktivieren, damit die Fußzuschläge-/rabatte der Auftragsbestätigung automatisch einem A+W Business-Produkt zugeordnet werden. Diese automatische Zuordnung können Sie unterdrücken.
    *   "Zuordnung des Fußzuschlags/-rabatts zukünftig automatisch auflösen" auf Seite D-222
Wenn diese Option geändert wurde, muss das aktuell eingelesene Dokument nochmals eingelesen werden.
    *   ⇨ Tutorial, "So lesen Sie ein openTRANS-Dokument ein" auf Seite D-169
*   **Referenzierenden Produktnummern des Lieferanten vertrauen:** Wenn im importierten Dokument eine A+W Business-Produktnummer als Referenz angegeben ist, kann die Zuordnung automatisch durchgeführt werden.

**Gruppe Xternal**

*   **Xternal-XML-Datei erstellen:** Diese Option ist nur kundenspezifisch aktiviert.
*   **Einstellungen für Xternal:** Öffnet den Dialog `Einstellungen`, um Vorgaben für den XML-Export festzulegen. Diese Funktion ist nur freigeschaltet, wenn die Option `Xternal-XML-Datei erstellen` aktiviert ist.

### Elektronische Preiskontrolle – Dokumentenimport

`Dokumente > Bestellung > Auftragsbestätigung > Elektr. Preiskontrolle > Register Dokumentenimport`

[Image: Screenshot of the electronic price control document import screen.]
**Abb. D-128**: Elektronische Preiskontrolle – Dokumentenimport

In diesem Register prüfen Sie die importierten Auftragsbestätigungen. Nur wenn der Dokumentenstatus fehlerfrei ist, kann die Preiskontrolle erfolgreich abgeschlossen werden.
⇨ Tutorial, "Elektronisches Dokument prüfen" auf Seite D-170

**Buchungsart**

Mit der Wahl der Option legen Sie fest, wie das elektronische Dokument verarbeitet werden soll. Die Optionen sind dem Dokumentenstatus entsprechend freigeschaltet.

*   **Ablehnen:** Mit dieser Option werden die Dokumente nicht übernommen. Die Preiskontrolle wird nicht durchgeführt.
*   **Akzeptieren:** Mit dieser Option wird die Preiskontrolle bestätigt. Die AB-Nummer, Preise und Liefertermine aus dem importierten Dokument werden in die Bestellungen zurückgeschrieben. Die Dokumentenhistorie wird aktualisiert.
*   **Teillieferung erstellen:** Zu den im Dokument enthaltenen Positionen wird eine (neue) Teillieferung erstellt und wie bei `Akzeptieren` verbucht. Die restlichen Positionen bleiben in der ursprünglichen Bestellung erhalten. Der Status dieser Bestellung wird entsprechend angepasst. Bei einem Lieferavis wird mit dieser Buchungsart eine Teilbestellung erzeugt.

**Auftragsbestätigungen**

In der Übersicht sind alle importierten Auftragsbestätigungen aufgelistet. Diese können von unterschiedlichen Lieferanten stammen.
Wenn Sie einen Eintrag markieren, werden die referenzierten Dokumente in der Übersicht `Bestellungen / Teillieferungen` angezeigt.

*   **AB-Nummer:** AB-Nummer, die der Lieferant angegeben hat.
*   **Lieferant:** Name des Lieferanten.
*   **Lieferdatum bestätigt:** Lieferdatum, das der Lieferant in der AB angegeben hat.
*   **Netto:** Gesamtbetrag der Lieferung.
*   **Währung:** Währung, in der der Betrag in der AB angegeben ist. Diese Anzeige ist nur dann von Bedeutung, wenn Sie mit einem Mehrwährungssystem arbeiten.

**Anzeige** Sie können die Anzeige der Dokumente einschränken.

**Filtereinstellungen** Sie können Filter für die Anzeige der importierten Dokumente festlegen.
⇨ "Filtereinstellungen" auf Seite D-223

**Dokumentenstatus**

Die rote oder grüne Markierung gibt an, ob Unstimmigkeiten festgestellt wurden oder nicht. Die Optionen im Bereich `Buchungsart` sind entsprechend gesperrt oder freigeschaltet.

*   **Kein Dokument ausgewählt:** Die Anzeige des Dokumentenstatus kann nicht aktualisiert werden, da kein Dokument in der Übersicht markiert ist. Dieser Eintrag wird nicht angezeigt, wenn eine AB markiert ist.
*   **Mindestens ein Fußzuschlag/-rabatt einer Bestellung konnte dem Dokument nicht zugeordnet werden:** Dieser Eintrag wird nur angezeigt, wenn eine AB mit einem entsprechenden Fehler markiert ist.
*   **Bestellungen vollständig referenziert:** Bei einer roten Anzeige stimmt mindestens eine der referenzierten Positionen nicht vollständig mit der importierten AB überein. Die unvollständig referenzierten Bestellungen werden in der Übersicht gekennzeichnet.
*   **Fehlende Artikelpositionen in Bestellungen:** In der Auftragsbestätigung sind Positionen enthalten, die in der Bestellung nicht aufgeführt sind.
*   **Fehlende Fußzuschläge/-rabatte in Bestellungen:** Fußzuschläge/-rabatte werden nicht mitbestellt. Da sie aber in der AB aufgeführt sind, müssen sie für die Preiskontrolle als Positionen in den Bestellungen vorhanden sein. Die fehlenden Fußzuschläge/-rabatte müssen in der Bestellung manuell erfasst werden.
*   **Preisdifferenz:** Die Gesamtpreise von Bestellung und AB sind unterschiedlich. In den zugehörigen Feldern wird die Abweichung als Betrag und prozentual angezeigt.
*   **Mengendifferenzen:** Die Positionsmengen von Bestellung und AB sind unterschiedlich.

**[Dokument anzeigen]** Öffnet die Dokumentenansicht des markierten Dokuments.

**Bestellungen / Teillieferungen**

In der Übersicht werden die referenzierten Dokumente angezeigt, wenn Sie einen Eintrag im Bereich `Auftragsbestätigungen` markiert haben. Teillieferungen werden in blauer Schrift angezeigt.

*   **Bestellnummer:** Nummer der Bestellung, die von A+W Business erzeugt wurde.
*   **Lieferdatum gewünscht:** Datum aus der Lagerbestellung oder dem Kundenauftrag.
*   **Netto:** Gesamtbetrag der Bestellung oder des Auftrags.
*   **Währung:** Währung, in der der Betrag in der Bestellung angegeben ist. Diese Anzeige ist nur dann von Bedeutung, wenn Sie mit einem Mehrwährungssystem arbeiten.
*   **Auftr.Nr.:** Auftragsnummer.
*   **Kundenliefertermin:** Datum der Anlieferung beim Kunden.
*   **Bemerkung:** Wenn die Verknüpfung zwischen der Bestellung und dem importierten Dokument nicht vollständig ist, wird ggf. ein Hinweis auf den Fehler angezeigt.

### Elektronische Preiskontrolle – Positionsübersicht

`Dokumente > Bestellung > Auftragsbestätigung > Elektr. Preiskontrolle > Register Positionsübersicht`

[Image: Screenshot of the electronic price control position overview.]
**Abb. D-129**: Elektronische Preiskontrolle – Positionsübersicht

In diesem Register können Sie die Positionen der Auftragsbestätigung (AB) prüfen, die Ihr Lieferant gesendet hat. Sie können die Preise der Positionen korrigieren. Die Korrekturen werden in die referenzierten Bestellungen zurückgeschrieben.

Die Optionen im Bereich `Buchungsart` sind zu Register `Dokumentenimport` erklärt.
⇨ "Elektronische Preiskontrolle - Dokumentenimport" auf Seite D-216

**Positionsübersicht**

In der Übersicht sind alle Positionen der Auftragsbestätigung aufgeführt. Wenn Sie eine Position markieren, werden die Details in den Bereichen `Dokumentenposition` und `Bestellposition` angezeigt.

*   **Pos-Nr.:** Positionsnummer aus der AB.
*   **Bestell-Nummer:** Nummer der referenzierten Bestellung.
*   **Bestell-Position:** Positionsnummer aus der Bestellung.
*   **Netto Dokument/Netto 1 Bestellung:** Positionspreis aus der importierten AB und aus der Bestellung.
*   **Menge Dokument/Menge 1 Bestellung:** Positionsmenge aus der importierten AB und aus der Bestellung.
*   **Abmessung Dokument/Abmessung 1 Bestellung:** Positionsmaße aus der importierten AB und aus der Bestellung.
*   **Differenz Preis:** Differenz aus Spalte Netto Dokumente und Netto Bestellung.
*   **Differenz 1 Preis %:** Preisdifferenz in Prozent.
*   **Differenz 2 Menge:** Differenz aus Spalte Menge Dokumente und Menge Bestellung.
*   **Auftr.Nr.:** Auftragsnummer.
*   **Kundenliefertermin:** Datum der Anlieferung beim Kunden.

**Dokumentenposition, Bestellposition**

In diesen beiden Bereichen werden Details zu der Position angezeigt, die in der Positionsübersicht markiert ist.

### Auswahl (Prod. Nr. für Ausgleichspos.)

`Dokumente > Bestellung > Auftragsbestätigung > Elektr. Preiskontrolle > Menü Optionen > Prod.Nr. für Ausgleichspos.`

`Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Menü Optionen > Prod.Nr. für Ausgleichspos.`

[Image: Screenshot of the product selection dialog for balancing items.]
**Abb. D-130**: Auswahl

In diesem Dialog können Sie die Produktnummer eintragen, mit der Rundungsdifferenzen verbucht werden.

Der Dialog kann nur bei der elektronischen Preis-/Rechnungskontrolle geöffnet werden.
*   ⇨ Tutorial, "Betragsdifferenzen" auf Seite D-158
*   ⇨ Tutorial, "Elektronisches Dokument prüfen" auf Seite D-170

> **Voraussetzung**
> In der Produktverwaltung muss ein Produkt angelegt sein, auf das die Rundungsdifferenzen verbucht werden können.

**Artikelnummer**: Nummer des Produktes, auf das die Preisdifferenz verbucht werden soll.

### Einstellungen für Xternal

Diese Funktion und der Dialog sind nur kundenspezifisch freigeschaltet.

Während der Rechnungskontrolle kann eine XML-Datei zur Schnittstelle Xternal gesendet werden. Darin enthalten ist ein Auszug aus den Kopf- und Positionsdaten der vorliegenden Bestellungen.

### Positionen manuell zuordnen

`Dokumente > Bestellung > Auftragsbestätigung > Elektr. Preiskontrolle > Menü Funktionen > Positionen manuell zuordnen`

`Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Menü Funktionen > Positionen manuell zuordnen`

[Image: Screenshot of the manual position assignment dialog.]
**Abb. D-131**: Positionen in der elektr. Preis- oder Rechnungskontrolle manuell zuordnen

In diesem Dialog ordnen Sie die Positionen des importierten Dokuments den Positionen der Bestellung(en) zu. Diesen Dialog können Sie nur öffnen, wenn Sie die automatische Zuordnung im Menü `Funktionen` deaktiviert haben.
*   "Menü Funktionen" auf Seite D-214
*   ⇨ Tutorial, "Positionen im elektronischen Dokument zuordnen" auf Seite D-173

**Dokumenten-Positionen, Bestell-Positionen**

In diesen beiden Bereichen werden die Positionen aus dem importierten Dokument und der zugehörigen Bestellung aufgelistet. Um die Positionen einander zuzuordnen, markieren Sie jeweils die entsprechenden Einträge und bestätigen die Zuordnung mit `[OK]`. Die zugeordneten Positionen werden danach nicht mehr angezeigt.

Die Zuordnungen können Sie aufheben, wenn Sie im Menü `Funktionen` den Eintrag `Alle Positionszuordnungen aufheben` wählen.
"Menü Funktionen" auf Seite D-214

**Produktzuordnung des Fußzuschlages/-rabatts merken** Die Checkbox ist nur freigeschaltet, wenn Sie einen Fußzuschlag/-rabatt zugeordnet haben. Sie können diese Zuordnung für die aktuelle Sitzung speichern. Die Speicherung gilt nicht, wenn Sie den Dokumentenimport erneut starten.
*   ✅ Die Zuordnung gilt nur für dieses eine Dokument und die zugehörigen Bestellungen.
*   ✅ Die Zuordnung gilt für alle weiteren Dokumente, die der Importfilter ausgewählt hat.

**Zuordnung des Fußzuschlags/-rabatts zukünftig automatisch auflösen** Die Checkbox ist nur freigeschaltet, wenn die Checkbox `Produktzuordnung des Fußzuschlages/-rabatts merken` markiert ist.
Wenn Sie einen Fußzuschlag/-rabatt zugeordnet haben, können Sie diese Zuordnung für alle künftigen Importe speichern.
*   ✅ Die Zuordnung gilt nur für dieses eine Dokument und die zugehörigen Bestellungen.
*   ✅ Die Zuordnung wird für alle weiteren importierten Dokumente des Lieferanten automatisch durchgeführt.

### Fußzuschläge/-rabatte verteilen

`Dokumente > Bestellung > Auftragsbestätigung > Elektr. Preiskontrolle > Menü Funktionen > Fußzuschläge/-rabatte auf Bestellungen verteilen`

`Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Menü Funktionen > Fußzuschläge/-rabatte auf Bestellungen verteilen`

[Image: Screenshot of the dialog for distributing surcharges/discounts on orders.]
**Abb. D-132**: Fußzuschläge/-rabatte auf Bestellungen verteilen

In diesem Dialog können Sie den Fußzuschlag/-rabatt in einem elektronischen Dokument mehreren Bestellungen zuordnen.

In der Übersicht werden alle Bestellpositionen aufgelistet, die zu dem importierten Dokument gehören.
*   ⇨ Tutorial, "Fußzuschläge/-rabatte" auf Seite D-157
*   ⇨ Tutorial, "Zuschläge/Rabatte manuell zuordnen" auf Seite D-175

### Filtereinstellungen

`Dokumente > Bestellung > Auftragsbestätigung > Elektr. Preiskontrolle > Schaltfläche Filtereinstellungen`

`Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Menü Funktionen > Schaltfläche Filtereinstellungen`

[Image: Screenshot of the filter settings dialog for importing documents.]
**Abb. D-133**: Filtereinstellungen für die Anzeige von importierten Dokumenten

In diesem Dialog können Sie festlegen, welche Bestellungen zu importierten Dokumenten angezeigt werden sollen. Die Filter können sich auf den Erfasser und/oder auf den Lieferanten beziehen.

**Nach Erfasser**

Sie können festlegen, wessen Bestellungen zum importierten Dokument angezeigt werden können.

*   **Alle**: Sie können sich alle Bestellungen zu den importieren Dokumenten anzeigen lassen.
    *   ✅ Die Anzeige der Bestellungen soll über die weiteren Filter eingeschränkt werden. Die Checkboxen `Nur eigene` und `Festlegen` sind freigeschaltet.
    *   ✅ Die Anzeige der Bestellungen wird nicht auf Erfasser oder Nummernverwalter eingeschränkt. Die Checkboxen `Nur eigene` und `Festlegen` sind gesperrt.
*   **Nur eigene**: Die Checkbox ist gesperrt, wenn die Checkbox `Alle` markiert ist.
    *   ✅ Die Anzeige wird nicht auf die eigenen Bestellungen eingeschränkt.
    *   ✅ Die Anzeige wird auf die Bestellungen eingeschränkt, die Sie selbst erfasst haben. Wenn Sie zusätzlich einen Nummernverwalter auswählen, werden Ihnen nur Ihre Bestellungen aus dem gewählten Nummernverwalter angezeigt.
*   **Festlegen**: Die Checkbox ist gesperrt, wenn die Checkbox `Alle` markiert ist.
    *   ✅ Die Anzeige der Bestellungen wird nicht auf einen Nummernverwalter eingeschränkt.
    *   ✅ Nur die Bestellungen aus dem angezeigten Nummernverwalter werden angezeigt. Wenn Sie zusätzlich die Checkbox `Nur eigene` markiert haben, werden Ihnen nur Ihre Bestellungen aus dem gewählten Nummernverwalter angezeigt.

**Nach Lieferanten**

Sie können die Anzeige der Bestellungen auf einen oder mehrere Lieferanten einschränken.

*   **Lieferant**: Sie können einen oder mehrere Lieferanten auswählen.
*   **Schaltflächen**: Mit den Schaltflächen übernehmen Sie den gewählten Lieferanten in die Übersicht oder entfernen einen Eintrag aus ihr.
    *   ⇨ Tutorial, "Schaltflächen in Suchdialogen" auf Seite C-42

**Übersicht**

In der Übersicht werden alle Lieferanten angezeigt, die als Filter für die Anzeige von Bestellungen gelten.

> **Einstellungen speichern**
> Beim Verlassen werden die Einstellungen gespeichert und gelten so lange, bis sie geändert oder zurückgesetzt werden.

### Mahnung

`Dokumente > Bestellung > Auftragsbestätigung > Mahnung`

[Image: Screenshot of the dunning dialog for suppliers.]
**Abb. D-134**: Lieferanten mahnen

In diesem Dialog können Sie nach offenen Bestellungen suchen, deren Lieferung überfällig ist. Die Suche kann durch ein Datum, auf bestimmte Lieferanten, Nummernverwalter und/oder Status eingeschränkt werden.
⇨ Tutorial, "Lieferanten anmahnen" auf Seite D-97

**Menü Funktionen**

*   **Mahnkennzeichen löschen:** Löscht das Mahnkennzeichen aus den angezeigten Bestellungen.

**Auswahl**

*   **Lieferant von, bis**: Einschränkung der Suche auf einen Lieferanten oder eine Folge von Lieferanten.
*   **Nummernverwalter**: Anzeige der Bestellungen in einem Nummernverwalter.
*   **Status von, bis**: Einschränkung der Suche auf Bestellungen, die in einem bestimmten Statusbereich liegen.

**Optionen**

*   **Bis Erfassungsdatum**: Angabe des Erfassungsdatums, zu dem nach offenen Bestellungen gesucht werden soll. Standardmäßig ist das aktuelle Tagesdatum ausgewählt. Mit dieser Einstellung werden ggf. auch Bestellungen angezeigt, die noch gar nicht geliefert sein können.
*   **Bereits gemahnte Lieferanten nochmals mahnen**: Wenn Sie eine Lieferung angemahnt haben, wird an der betreffenden Bestellung ein Mahnkennzeichen gesetzt.
    *   ✅ Bereits angemahnte Bestellungen werden nicht angezeigt.
    *   ✅ Offene Bestellungen werden auch dann angezeigt, wenn sie bereits angemahnt wurden. Sie können erneut angemahnt werden.
*   **Faxversand/Postversand/Mailversand/Alle**: Die Suche kann zusätzlich auf Bestellungen eingeschränkt werden, die als Fax, als Post oder als Mail versendet wurde. Als Postversand gilt auch, wenn Sie eine PDF-Datei als Anhang einer E-Mail gesendet haben. Wenn Sie die Suche nicht einschränken wollen, wählen Sie die Option `Alle`. Die Mahnungen werden auf dem Weg versendet, der für den entsprechenden Lieferanten als Standard für Bestellungen festgelegt ist.

**Tabelle**

In der Übersicht werden alle Lieferanten aufgeführt, zu denen offene Bestellungen vorliegen, die den Filterkriterien entsprechen. In roter Schrift sind die Lieferanten angezeigt, an die bereits eine Mahnung geschickt wurde.

*   **Bestellnummer:** Nummer der offenen Bestellung.
*   **Stat.:** Status der offenen Bestellung.
*   **Lieferant:** Lieferant, an den die Bestellung gesendet wurde.
*   **Erfassungsdatum:** Erfassungsdatum der Bestellung.
*   **Liefertermin:** Geplanter und/oder bestätigter Liefertermin aus der Bestellung.

## Wareneingang

`Dokumente > Bestellung > Wareneingang > Wareneingang`

Sie können den Wareneingang und die Auftragsbestätigung vom Lieferanten erfassen sowie die gelieferten Positionen prüfen und ggf. korrigieren.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Wareneingang (Dialog)" auf Seite D-227
*   "Eingangskontrolle" auf Seite D-241

### Wareneingang (Dialog)

`Dokumente > Bestellung > Wareneingang > Wareneingang`

**Zu Dialogbeschreibung:**
*   ⇨ Einstellungen (ID)

In diesem Dialog können Sie den Wareneingang zu einzelnen Bestellungen oder zu den Bestellungen in einem Nummernverwalter erfassen.

Für die jeweilige Bestandsbuchung können Sie Vorgaben für die Identifikationsnummern (ID) festlegen, die automatisch vergeben wird, wenn in der Lagerbestellung Positionen mit einer Menge größer als 1 erfasst sind. Die Identnummern werden für Kisten und Gläser (Lagerplatten) vergeben.

> **Voraussetzung**
> In den Firmendaten muss die Checkbox für die virtuelle Vergabe von Positionsnummern markiert sein.
> ⇨ Stammdaten, "Fälligkeitsberechnung für Februar (28 oder 29 Tage)" auf Seite B-955

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menü Funktionen" auf Seite D-228
*   "Menü Optionen" auf Seite D-228
*   "Menü Druck" auf Seite D-229
*   "Wareneingang – Auswahl" auf Seite D-230
*   "Wareneingang – Komplett" auf Seite D-232
*   "Wareneingang – Positionsweise" auf Seite D-234
*   "Wareneingang - Identnummer" auf Seite D-237
*   "Wareneingang - Protokoll (Identnummern)" auf Seite D-239

### Menü Funktionen

`Dokumente > Bestellung > Wareneingang > Wareneingang > Menü Funktionen`

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Wareneingang zu schließen.

Folgende Einträge werden angezeigt:
*   **Dokument anzeigen:** Öffnet den Dialog `Dokumentenansicht` zu einer Vorschau auf den Druck.
    *   Verkauf, "Reklamationen" auf Seite C-605
*   **Dokumentendaten:** Öffnet den Dialog `Dokumentendaten`, um ggf. die Termine und den Status zu korrigieren.
    *   Verkauf, "Dokumentendaten" auf Seite C-755
*   **Lagersuche:** Öffnet den Dialog `Lagerinfo`, um die aktuellen Lagerbestände anzuzeigen.
    *   Verkauf, "Lagerinfo" auf Seite C-758
*   **Artikel Info:** Öffnet einen Dialog `Artikelinfo`, um Detailinformationen zum aktuellen Produkt zu erhalten.
    *   Verkauf, "Artikel-Informationen" auf Seite C-616

### Menü Optionen

`Dokumente > Bestellung > Wareneingang > Wareneingang > Menü Optionen`

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

Folgende Einträge werden angezeigt:
*   **Positionsansicht bei Auswahl von einzelnem Dokument:** Mit dieser Option wechselt die Ansicht zum Register `Positionsweise`, wenn Sie sich ein einzelnes Dokument anzeigen lassen.
*   **Identnummernvergabe:** Diese Einstellung wird für den Wareneingang von Kisten und Lagerplatten benötigt.
    *   **Automatische Vergabe:** Mit dieser Option wird die ID automatisch vergeben. Dazu kann eine Vorgabe festgelegt werden. Wenn die Option nicht aktiviert ist, müssen Sie die ID manuell eingeben.
    *   **Einstellungen:** Öffnet den Dialog `Einstellungen`, in dem Sie die Vorgabe für die automatische Vergabe von IDs festlegen.
        *   ⇨ "Einstellungen (ID)" auf Seite D-240
*   **Lagerort für Identnummern aus Position vorblenden:** Mit dieser Option wird der Lagerort vorgeschlagen, der in der zuvor verbuchten Position angegeben war.
*   **Lagerbuchungsdatum = Lieferdatum:** Als Buchungsdatum wird automatisch das Lieferdatum aus der Bestellung übernommen. Wenn die Option deaktiviert ist, wird standardmäßig das Tagesdatum übernommen.
*   **AB-Nummer prüfen:** Mit dieser Einstellung wird eine Meldung angezeigt, wenn die Nummer der Auftragsbestätigung durch den Lieferanten nicht eingegeben ist.

### Menü Druck

`Dokumente > Bestellung > Wareneingang > Wareneingang > Menü Druck`

Über dieses Menü können Sie die Druckfunktionen starten.

Folgende Einträge werden angezeigt:
*   **Wareneingang:** Startet den Druck einer Liste mit allen Bestellungen und referenzierten Aufträgen, die im Dialog aufgeführt sind.
*   **Etiketten:** Startet den Druck von Kistenetiketten.
*   **Protokoll:** Startet den Druck eines Protokolls mit allen Kistenpositionen und den vergebenen Kisten-IDs.
*   **Etiketten und Protokoll (nur Gruppe Drucker):** Startet den Druck der Kistenetiketten und eines Protokolls mit den vergebenen Kisten-IDs.
*   **Einstellungen:** Öffnet die Druckereinstellungen.

### Wareneingang – Auswahl

`Dokumente > Bestellung > Wareneingang > Wareneingang > Register Auswahl`

[Image: Screenshot of the goods receipt 'Auswahl' (selection) register.]
**Abb. D-135**: Wareneingang – Auswahl

In diesem Register können Sie die Auswahl und Anzeige der Dokumente filtern, zu denen Sie Wareneingänge prüfen und/oder erfassen möchten.
⇨ Tutorial, "Wareneingang" auf Seite D-120

**Auswahl**

Mit der Wahl der Option legen Sie fest, wie die Bestellungen gefiltert werden. Die offenen Bestellungen werden nach der Suche im Register `Komplett` angezeigt, damit die Wareneingänge verbucht werden können.

*   **Nach Bestellnummer:** Das Eingabefeld für die Bestellnummer wird freigeschaltet. Im Register `Komplett` werden die gesuchte Bestellung und alle referenzierten Aufträge angezeigt.
*   **Nach Auftragsnummer:** Das Eingabefeld für die Auftragsnummer wird freigeschaltet. Im Register `Komplett` werden alle Bestellungen angezeigt, die zur eingetragenen Auftragsnummer erzeugt wurden.
*   **Nach Lieferanten:** Das Eingabefeld für die Lieferantennummer wird freigeschaltet. Im Register `Komplett` werden alle Bestellungen beim gewählten Lieferanten angezeigt.
*   **Nach Lieferscheinnummer / Lieferavis, Gesamtliefermenge:** Das Eingabefeld für die Nummer des Lieferscheins oder des Lieferavis und das Feld für die Gesamtmenge werden freigeschaltet. Wurde ein Lieferavis importiert, müssen die tatsächlich gelieferten Mengen eingetragen werden.
*   **Nach Anliefertermin des Lieferanten:** Das Eingabefeld für den Liefertermin wird freigeschaltet. Im Register `Komplett` werden alle Bestellungen angezeigt, die zum gewählten Termin angeliefert werden sollen.
*   **Nach Nummernverwalter:** Die Kombobox zur Auswahl des Nummernverwalters wird freigeschaltet. Im Register `Komplett` werden alle Bestellungen im gewählten Nummernverwalter angezeigt.
*   **Nach Scanner / Dokument:** Die Felder für den Barcode der Bestellnummer oder einer Bestellposition werden freigeschaltet.

**Ziel-Nummernverwalter**

*   **Ziel-Nummernverwalter**: Die Lagerbestellungen können nach dem Buchen des Wareneingangs automatisch in einen anderen Nummernverwalter gestellt werden.
    *   ✅ Die Lagerbestellungen werden nicht in einen anderen Nummernverwalter gestellt.
    *   ✅ Die Felder im Bereich `Ziel-Nummernverwalter` werden freigeschaltet. Die Lagerbestellungen werden in den gewählten Nummernverwalter gestellt.
*   **Mitarbeiter**: Name des Mitarbeiters, dem der Ziel-Nummernverwalter zugeordnet ist.
*   **Nummernverwalter**: Nummernverwalter, in den die Lagerbestellungen mit (vollständigen) Wareneingängen gestellt werden sollen.

### Wareneingang – Komplett

`Dokumente > Bestellung > Wareneingang > Wareneingang > Register Komplett`

[Image: Screenshot of the goods receipt 'Komplett' (complete) register.]
**Abb. D-136**: Wareneingang – Komplett

In diesem Register werden alle Bestellungen angezeigt, die den Suchkriterien entsprechen. Wenn Sie eine Bestellung markieren, werden die referenzierten Aufträge aufgelistet.
⇨ Tutorial, "Wareneingang erfassen" auf Seite D-127

**Liefertermin**

*   **Anliefertermin des Lieferanten**: Anzeige des aktuellen Tagesdatums. Sie können es überschreiben, wenn Sie eine Lieferung erfassen wollen, die vor diesem Datum eingetroffen ist. Das Datum wird nur für die Dokumente übernommen, die in der Übersicht markiert sind.
*   **AB-Lieferant**: Sie können zu einem Wareneingang auch die Nummer der Auftragsbestätigung durch den Lieferanten erfassen.

**Dokumente**

Mit den Schaltflächen können Sie alle oder einige Dokumente markieren oder die Markierung entfernen.

In der Übersicht werden alle Bestellungen angezeigt, die den Suchkriterien im Register `Auswahl` entsprechen. Der vollständige Wareneingang wird für die Dokumente erfasst, bei denen die Checkbox `Komplett buchen` markiert ist.

*   **Bestell-Nr.:** Nummer der Bestellung.
*   **Komplett buchen:** Eine Bestellung kann als komplett gebucht werden, wenn alle Positionen vollständig geliefert wurden.
    *   ✅ Der Wareneingang ist nicht vollständig. Es stehen noch Lieferungen aus.
    *   ✅ Der Wareneingang ist vollständig und die Bestellung soll als komplett verbucht werden.
*   **Status:** Aktueller Status. Der Status wird nach der Erfassung des Wareneingangs umgesetzt.
*   **Lieferant:** Nummer und Name des Lieferanten.
*   **Anlief.-Term. d. Lieferant:** Anliefertermin des Lieferanten. Der Termin wird aus der Bestellung oder der AB übernommen. Wenn Sie den Wareneingang erfasst haben, wird der Termin auf das aktuelle Tagesdatum oder das von Ihnen gewählte Datum umgesetzt.
*   **Enthält Kisten:** Anzeige der Bestellungen, in denen Kisten enthalten sind. Die Markierung der Checkbox kann nicht geändert werden.

**Zugehörige Aufträge**

In der Übersicht werden nur die referenzierten Aufträge angezeigt, die zu der ausgewählten Bestellung gehören. Wenn mehrere Bestellungen ausgewählt sind, bleibt die Liste leer.

*   **Anliefertermin bei Kunde**: Das Datum wird aus dem referenzierten Auftrag übernommen. Sie können es überschreiben, wenn der ursprüngliche Termin nicht eingehalten werden kann.

### Wareneingang – Positionsweise

`Dokumente > Bestellung > Wareneingang > Wareneingang Kiste > Register Positionsweise`

[Image: Screenshot of the goods receipt 'Positionsweise' (by position) register.]
**Abb. D-137**: Wareneingang – Positionsweise

In diesem Register können Sie Wareneingänge positionsweise für eine Bestellung erfassen, die im Register `Komplett` ausgewählt wurde.

**Warenein-/ausgang**

*   **Menge Eingang**: Menge, die für die markierte Position geliefert wurde.
*   **Menge bestellt, Bereits geliefert, Menge avisiert**: In diesen Feldern werden die entsprechenden Mengen für die markierte Position angezeigt. Die Felder werden nach der Erfassung aktualisiert.
*   **Lagerort**: Zur markierten Position können Sie einen Lagerort auswählen, an dem der Lagerartikel verbucht werden soll. Beachten Sie dabei, dass Lagerartikel auch auf den Lagerort `<k.A.>` gebucht werden können. Der Lagerort aus der Bestellung kann über das Menü `Optionen` vorgeblendet werden.
    *   ⇨ "Menü Optionen" auf Seite D-228

