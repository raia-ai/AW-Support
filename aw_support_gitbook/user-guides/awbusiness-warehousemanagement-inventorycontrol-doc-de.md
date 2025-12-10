---
description: "DE_AWBusiness_Lagerwirtschaft_6_3"
---


# Tutorial Lagerwirtschaft

*   Die Wiederbeschaffungszeit für den Artikel reicht aus, um die Ware bis zu dem Termin nachzubestellen. In der Lagervorschau werden die entsprechenden Zeilen gelb markiert.
*   Die Wiederbeschaffungszeit reicht nicht aus. In der Lagervorschau werden die entsprechenden Zeilen rot markiert.

Bei der Erfassung eines Dokuments können Sie dann den Lieferanten und/oder den Liefertermin ändern. In der Einheit Auftragserfassung von Lagerartikeln ist dies ausführlich beschrieben.
⇨ "Lagerartikel für Position suchen" auf Seite G-120

---
### Einstellungen zu Lagerverfügbarkeit und Wiederbeschaffungszeit

Zur Berechnung der zukünftigen Bestände werden vom aktuellen Bestand alle Reservierungen pro Tag abgezogen und bestellte Mengen addiert. Daraus ergibt sich der voraussichtliche Lagerbestand abhängig vom Tagesdatum.

Um die Performance zu erhöhen, können Sie die Anzeige im Dialog Lagerinfo durch folgende Einstellungen einschränken:

*   Im Dialog **Produktverwaltung > Register Lager/Einkauf > Checkbox keine Verfügbarkeitsprüfung** können Sie bestimmte Artikel aus der Lagervorschau und der Verfügbarkeitsprüfung herausnehmen, indem Sie die Verfügbarkeitsprüfung für diese Artikel ausschalten.
*   Im Dialog **Firmendaten** können Sie einstellen, über welchen Zeitraum die Vorschau dargestellt werden soll. In der Regel reichen zwei bis vier Wochen aus. Wenn Sie eine Null eintragen, wird die Vorschau für 14 Tage angezeigt.
*   Im Dialog **Lagerverwaltung** können Sie mehrere Lagermaße miteinander verknüpfen. Damit wird erreicht, dass Sie nur für den Hauptartikel einen Mindestbestand hinterlegen müssen, gegen den die Bestandsprüfung durchgeführt wird. Diese Funktion haben Sie bereits in der Einheit Lagerverwaltung kennengelernt.
⇨ "Lager-Hauptartikel" auf Seite G-70

### Buchungstermine

Um eine konkrete Aussage über den Lagerbestand zu einem bestimmten Termin treffen zu können, müssen alle Wareneingänge und Warenausgänge mit einem voraussichtlichen Buchungsdatum versehen werden.

Die voraussichtlichen Buchungstermine werden bei der Erfassung der Positionen wie folgt festgelegt:

*   Stücklistenelemente und Produkte mit der Beschaffungsart Lagerentnahme, die zugeschnitten werden müssen, werden zum Datum des Produktionsstarts eingetragen.
*   Für alle anderen Lagerartikel wird als Buchungsdatum das Lieferdatum aus dem Dokument verwendet.

Wenn der Auftrag anschließend in **AWCapacity Planning** eingelastet wird, so werden diese voraussichtlichen Termine durch die berechneten, tatsächlichen Termine ersetzt.

## Bestände in der Lagersuche anzeigen

Lagerbestände werden durch die Buchungen von Warenein- und -ausgängen aktualisiert. Das Lager ist eng gekoppelt mit den Dokumenten für den Verkauf und den Einkauf. Beim Erfassen von Dokumenten kann der aktuelle Lagerbestand daher über die Lagerinfo jederzeit erfragt werden.

Der aktuelle Lagerbestand wird auch bei der Erfassung von Angeboten, Auf-trägen und bei der Bestellung angezeigt. Dabei werden sowohl die Bestellungen als auch die Reservierungen berücksichtigt.

In dieser Einheit lernen Sie, wie Sie sich die Bestände und Reservierungen von Lagerartikeln anzeigen lassen.

> **Dialog Lagersuche öffnen**
> Der Dialog Lagersuche steht auch über das Modul Dokumente zur Verfügung. Damit kann schon bei der Erfassung eines Auftrags geprüft werden, ob die gewünschten Produkte in ausreichender Menge verfügbar sind.

**So lassen Sie die Bestände von Lagerartikeln anzeigen**

1.  Wählen Sie im Menü **Lagerwirtschaft > Suche**.

    *(Abb. G-50: Filter für die Suche nach Lagerartikeln)*
    *   **A Produkt - Lagerartikel**: Bereich zur Auswahl des Produkts, Artikels oder der Gruppe.
    *   **B Filter**: Bereich für Filteroptionen zur Eingrenzung der Suche.
    ⇨ Softwarereferenz, "Suche" auf Seite G-217

2.  Schränken Sie die Suche ein, indem Sie z. B. ein Produkt (A) auswählen.

3.  Wählen Sie im Bereich Filteroptionen (B) aus, welche Lagerartikel angezeigt werden sollen.
    Wenn Sie die Einstellung **Lagerware** deaktivieren, werden nur die Lagermaße angezeigt, die im Dialog **Produktverwaltung Lagermaße** angelegt sind, unabhängig davon, ob es sich um echte Lagerartikel handelt, das heißt, Lagerartikel aus der Lagerverwaltung.

4.  Wählen Sie im Menü **Start > Suchen**, um in die Suche zu starten.
    Die Trefferliste wird in der Übersicht angezeigt.

    *(Abb. G-51: Ergebnis der Suche - In diesem Beispiel wurde nach dem Produkt Float 5 mm gesucht.)*

5.  Wenn Sie sich die korrespondierenden Dokumente anzeigen lassen möchten, markieren Sie eine Zeile und öffnen das Kontextmenü (rechte Maustaste).

6.  Klicken Sie auf **korrespondierende Dokumente**.

    *(Abb. G-52: Korrespondierende Dokumente - In diesem Dialog werden alle Aufträge und Bestellungen angezeigt, in denen das Produkt erfasst wurde.)*

7.  Klicken Sie auf **[Ende]**, um den Dialog zu schließen.
    Der Dialog Lagersuche wird wieder angezeigt.

8.  Wenn Sie die nächsten Warenabgänge und -zugänge zu einem Produkt oder den zukünftigen Lagerbestand anschauen möchten, markieren Sie das Produkt und wechseln zum Register **Zukünftiger Lagerbestand**.

    *(Abb. G-53: Zukünftiger Lagerbestand)*

Der zukünftige Lagerbestand wird für den Zeitraum in der Zukunft angezeigt, den Sie in den Firmendaten für die Vorschau eingetragen haben. Die Sonn- und Feiertage werden mit angezeigt, jedoch nicht mitgezählt.

### Übungen

*   Prüfen Sie den Bestand und die Reservierungen für Float 4 mm. Notieren Sie sich die einzelnen Werte aus dem Register **Zukünftiger Lagerbestand**. In der nächsten Einheit werden Sie eine Bestellung erfassen und anschließend prüfen, wie sich die Werte geändert haben.

### Ergänzende Informationen

⇨ Softwarereferenz, "Suche" auf Seite G-217

## Lagerbestellung (automatisch)

### Lernziele

*   Dialog Lagerbestellung kennenlernen.
*   Automatische Lagerbestellung kennenlernen.
*   Automatisch ausgelöste Bestellvorschläge an den Einkauf übergeben.
*   Änderung der angezeigten Werte im zukünftigen Lagerbestand prüfen.

### Nutzen

*   Mit Bestellungen ergänzen Sie die Lagerbestände auf den gewünschten Sollbestand oder den Reservierungen entsprechend.
*   Wenn der Mindestbestand unterschritten wird, wird automatisch ein Bestellvorschlag erzeugt. Diesen können Sie im Dialog Lagerbestellung prüfen und dann an den Einkauf übergeben.

### Merke

*   **Lagerbestellung manuell erfassen**: Lagerbestellungen werden im Modul **Dokumente** erfasst und bearbeitet. Dieser Vorgang ist im Part **Einkauf** beschrieben.
*   **Bestellvorschläge**: Automatische Bestellvorschläge werden ausgelöst, wenn die definierte Mindestmenge unterschritten wird. Dabei werden Reservierungen und offene Bestellungen berücksichtigt. Die Bestellvorschläge werden automatisch erzeugt und manuell an den Einkauf übergeben. Erst durch die Übergabe wird eine Bestellung erzeugt, die an den Lieferanten gesendet werden kann.
*   **Voreinstellungen**:
    *   **Stammdaten**:
        *   Produktverwaltung
        *   Lieferantenkartei
    *   **Firmendaten**:
        *   Register **Parameter**
        *   Register **Lager / EK / EDI**
    *   **Lagerverwaltung**
        *   Mindestbestand
        *   Bestellmenge

### Bestellvorschläge

In der Regel werden Bestellungen aus der Lagerwirtschaft heraus erzeugt, um die Bestände auf dem gewünschten Niveau zu halten.

*(Abb. G-54: Lagerverwaltung - Bestandszahlen)*
*   **A Mindestbestand**: Die definierte Mindestmenge für einen Lagerartikel.
*   **B Menge für Bestellvorschlag**: Die Menge, die für einen Bestellvorschlag generiert wird.

Wenn Sie im Dialog **Lagerverwaltung** Mindestmengen (A) für einen Lagerartikel hinterlegt haben, werden Bestellvorschläge automatisch mit der hinterlegten Bestellmenge (B) erzeugt. Sie können diese vor der Übergabe an den Einkauf prüfen und ggf. den Lieferanten und den Termin ändern. Mit der Übergabe an den Einkauf wird aus dem Vorschlag eine Lagerbestellung erzeugt.

Lagerbestellungen können auch manuell über die Dokumentenverwaltung erzeugt werden. Die manuelle Lagerbestellung lernen Sie in einer separaten Einheit kennen.
⇨ "Manuelle Lagerbestellung" auf Seite G-127

### Lagerbestellung an den Einkauf übergeben

Automatisch erzeugte Bestellvorschläge werden im Dialog **Lagerbestellung-Bestellpool** angezeigt. Sie können den Lieferanten und den Termin ändern. Mit der Übergabe an den Einkauf erzeugen Sie die Bestellung. Diese muss dann an den Lieferanten gesendet werden.

Wenn zu einem Produkt mehrere Lieferanten hinterlegt sind, können Sie im Bestellpool die Liefertermine und Preise vergleichen und einen anderen Lieferanten auswählen.

In dieser Einheit lernen Sie, wie Sie einen Bestellvorschlag an den Einkauf übergeben.

> **Dialog Lagerbestellung**
> Der Dialog **Lagerbestellung – Bestellpool** ist nahezu identisch wie der Dialog **Bestellübergabe** aufgebaut, den Sie aus der Schulung zum Einkauf kennen. Es handelt sich jedoch um verschiedene Dialoge. Sie werden daher für jeden Bestellvorschlag genau einen Eintrag finden, zu dem es keine referenzierten Dokumente gibt.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:

*   "So übergeben Sie die Bestellvorschläge an den Einkauf” auf Seite G-109
*   "So ändern Sie den Lieferanten und den Liefertermin" auf Seite G-112

**So übergeben Sie die Bestellvorschläge an den Einkauf**

1.  Wählen Sie im Menü **Lagerwirtschaft > Lagerbestellung**.
    Der Dialog **Lagerbestellung** wird geöffnet.
    ⇨ Softwarereferenz, "Lagerbestellung" auf Seite G-220
    Wenn Sie die Bestellvorschläge nicht für das gesamte Lager anzeigen lassen wollen, können Sie die Anzeige auf bestimmte Lagerorte einschränken.

2.  Stellen Sie zur Einschränkung der Anzeige in den Feldern **Warenhaus**, **Gang**, **Regal** und **Fach** den gewünschten Lagerort ein.

    *(Abb. G-55: Lagerbestellung - In diesem Beispiel wird kein Lagerort ausgewählt, damit der Bestand aller Lagerorte aufgelistet wird.)*

3.  Wählen Sie im Menü **Start > Suchen**, um in die Suche zu starten.
    Die Vorschläge werden eingelesen und in der Übersicht aufgelistet.

    *(Abb. G-56: Lagerbestellung - Bestellvorschläge)*

4.  Markieren Sie die Bestellvorschläge, die Sie an den Einkauf übergeben möchten.

    > **Einträge gemeinsam markieren**
    > Sie können Bestellvorschläge gemeinsam markieren, indem Sie über das Menü **Funktionen** den Dialog **Markierungsoptionen** öffnen. Wenn Sie in diesem Dialog z. B. ein bestimmtes Produkt angeben, werden alle Bestellvorschläge zu diesem Produkt mit einem Kreuz im Zeilenkopf markiert.

    *(Abb. G-57: Markierte Bestellvorschläge)*
    Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf. Nur die Vorschläge sind markiert, die mit einem X gekennzeichnet sind.

5.  Wählen Sie im Menü **Start > Ausführen**, um die Übergabe an den Einkauf zu starten.
    Bestätigen Sie die Meldung zur Anzahl der übergebenen Vorschläge.
    Die Bestellungen werden erzeugt und die übergebenen Vorschläge werden aus der Liste gelöscht.

**So ändern Sie den Lieferanten und den Liefertermin**

1.  Lesen Sie im Dialog **Lagerbestellung** die Bestellvorschläge ein, wie oben beschrieben.

2.  Markieren Sie den Vorschlag, zu dem Sie den Lieferanten und/oder Liefertermin ändern wollen.
    Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf. Nur die Vorschläge sind markiert, die mit einem X gekennzeichnet sind.

    *(Abb. G-58: Vorschlag, dem ein anderer Lieferant zugeordnet werden soll)*

3.  Wählen Sie im Menü **Funktionen > Lieferant/Liefertermine ändern**.

    *(Abb. G-59: Liefertermin ändern)*

4.  Tragen Sie einen anderen Lieferanten und/oder Liefertermin ein.

5.  Klicken Sie auf **[OK]**, um die Änderung zu übernehmen.
    Der Dialog **Lieferant und Liefertermin ändern** wird geschlossen. In der Übersicht wird der Vorschlag mit dem neuen Lieferanten und/oder Liefertermin angezeigt.
    Sie können den Bestellvorschlag jetzt an den Einkauf übergeben.

### Preise vor der Übergabe vergleichen

Wenn zu einem Produkt mehrere Lieferanten hinterlegt sind, können Sie die Preise vor der Übergabe vergleichen und einen anderen Lieferanten auswählen. In dieser Einheit lernen Sie, wie Sie die Preise vergleichen und den günstigsten oder schnellsten Lieferanten auswählen können.

**So vergleichen Sie die Preise in einem Bestellvorschlag**

1.  Wählen Sie im Menü **Lagerwirtschaft > Lagerbestellung**.
    Der Dialog **Lagerbestellung** wird geöffnet.
    ⇨ Softwarereferenz, "Lagerbestellung" auf Seite G-220

2.  Wählen Sie in den Feldern **Warenhaus**, **Gang**, **Regal** und **Fach** den gewünschten Lagerort ein.

3.  Wählen Sie im Menü **Start > Ausführen**, um die Bestellvorschläge einzulesen.
    Die Vorschläge werden eingelesen und in der Übersicht aufgelistet.

4.  Markieren Sie den Vorschlag, zu dem Sie die Preise der Lieferanten vergleichen wollen.
    Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf. Nur die Vorschläge sind markiert, die mit einem X gekennzeichnet sind.

    *(Abb. G-60: Position, zu der die Preise verglichen werden sollen)*

5.  Wählen Sie im Menü **Funktionen > Lieferantenpreise**.

    *(Abb. G-61: Lieferanten für markierte Position ändern)*
    *   **A Standard-Lieferant (Textfarbe rot)**
    *   **B Checkbox des Standard-Lieferanten (abgewählt)**
    *   **C Ausgewählter Lieferant für aktuelle Bestellung**
    *   **D Checkbox zur Auswahl des Lieferanten (markiert)**
    *   **E Textfarbe rot:** Standard-Lieferant
    *   **F Textfarbe grün:** preisgünstigster Lieferant
    *   **G Textfarbe blau:** Standard-Lieferant ist am preisgünstigsten
    *   **H !!! bei allen Textfarben:** Liefertermin möglicherweise zu spät für rechtzeitige Produktion und Auslieferung an Kunden

6.  Markieren Sie die Checkbox links des Lieferanten, an den die Bestellung der Position gesendet werden soll.

7.  Klicken Sie auf **[OK]**, um die Änderung zu übernehmen.
    Der Dialog **Preisvergleich** wird geschlossen. In der Übersicht wird der Vorschlag mit dem neuen Lieferanten und/oder Liefertermin angezeigt.
    Sie können den Bestellvorschlag jetzt an den Einkauf übergeben.
    ⇨ "So übergeben Sie die Bestellvorschläge an den Einkauf" auf Seite G-109

### Übungen

*   Richten Sie die Mindest- und die Bestellmenge eines Lagerartikels so ein, dass ein automatischer Bestellvorschlag erzeugt wird. Wählen Sie dazu den Lagerartikel aus, für den Sie in der vorigen Übung die Werte aus dem zukünftigen Lagerbestand notiert haben.
*   Prüfen Sie einen Bestellvorschlag und ändern Sie den Lieferanten oder der Liefertermin. Wenn keine alternativen Lieferanten angezeigt werden, müssen Sie die Lieferantenkartei in den Stammdaten prüfen und anpassen.
*   Übergeben Sie die Bestellvorschläge an den Einkauf.
*   Prüfen Sie im Dialog **Lagersuche**, wie sich die Werte geändert haben.

### Ergänzende Informationen im Part Verkauf

⇨ Verkauf, "Auftragskopf" auf Seite C-39
⇨ Verkauf, "Bestellkennzeichen ändern" auf Seite C-310
⇨ Einkauf, "Lieferantenkartei anpassen" auf Seite D-33
⇨ Einkauf, "Dokument Bestellung" auf Seite D-45
➡ Einkauf, "Wareneingang erfassen" auf Seite D-127
➡ Einkauf, "Kistengeschäft" auf Seite D-136

## Lagerartikel in Dokumenten

In diesem Themenblock lernen Sie, wie Aufträge und manuelle Bestellungen auf die Lagerwirtschaft zugreifen.

Dazu gehören folgende Lerneinheiten:

*   "Auftragserfassung von Lagerartikeln" auf Seite G-118
*   "Manuelle Lagerbestellung" auf Seite G-127
*   "Produktionsaufträge" auf Seite G-131

### Auftragserfassung von Lagerartikeln

**Lernziele**
*   Nach Lagerartikeln für die Positionserfassung suchen.
*   Reservierung prüfen.
*   Änderungen im Lagerbestand nach Änderungen im Auftrag prüfen.

**Nutzen**
Bei der Erfassung von Positionen kann die Verfügbarkeit eines Produktes geprüft werden. Bei Engpässen können der Lieferant oder der Liefertermin direkt im Dokument geändert werden.

**Merke**
*   **Positionserfassung**: Lagerartikel werden in der Positionserfassung über die Lagersuche [F3] ausgewählt.
*   **Reservierung**: Ein im Auftrag erfasster Lagerartikel wird im Lager als reserviert gekennzeichnet.
*   **Voreinstellungen**:
    *   Stammdaten:
        *   Produktverwaltung
        *   Lieferantenkartei
    *   Firmendaten:
        *   Register Parameter
        *   Register Lager / EK / EDI

### Reservierung und Buchung von Lagerartikeln

Bei der Auftragserfassung wird die Stückzahl oder die Anzahl der Quadratmeter (qm-Zahl) der Lagerartikel für den Kundenauftrag reserviert. Die Lagerabbuchung erfolgt dann automatisch bei Lieferschein- oder Rechnungsdruck. Über die verkauften und bestellten Mengen errechnet A+W Business die aktuellen Bestände.

**Lagerbestand nach Änderung im Auftrag**
Was passiert mit dem Lagerbestand, wenn Aufträge geändert werden, für die bereits ein Warenabgang gebucht wurde? In den folgenden Beispielen wird der Warenabgang beim Druck des Lieferscheins gebucht.

| Änderung im Auftrag | Folge im Auftrag | Lagerbuchung |
| :--- | :--- | :--- |
| Auftragskopf ändern, keine Änderung der Positionen | Status bleibt unverändert. | Bei erneutem Erst-Druck des Lieferscheins wird kein neuer Warenabgang im Lager gebucht. |
| Position nachträglich löschen | Status ist bereits 72 und bleibt unverändert. | Abfrage, ob der Lagerbestand korrigiert werden soll. |
| Position nachträglich hinzufügen | | Abfrage, ob der Lagerbestand korrigiert werden soll. |
| Stückzahl nachträglich ändern | | Lagermenge wird automatisch ohne weiteren Hinweis korrigiert. |

In den nächsten Einheiten lernen Sie, wie Sie einen Lagerartikel in einem Dokument erfassen und die Buchung prüfen können.

### Lagerartikel für Position suchen

In dieser Einheit lernen Sie, wie Sie eine Position erfassen und dabei die Verfügbarkeit des gewünschten Produktes prüfen. Sie öffnen dazu den Dialog Lagersuche, den Sie bereits in der vorigen Einheit kennengelernt haben.

> **Lagersuche beim Erfassen einer Bestellung**
> Die Auswahl eines Lagerartikels über den Dialog **Lagersuche** können Sie auch beim Erfassen einer manuellen Lagerbestellung anwenden. Die manuelle Lagerbestellung ist in der gleichnamigen Einheit beschrieben.
> ⇨ "Manuelle Lagerbestellung" auf Seite G-127

**So erfassen Sie einen Lagerartikel als Position**

1.  Wählen Sie im Menü **Dokumente > Auftrag > Auftrag** und erfassen Sie einen Auftragskopf.

2.  Wechseln Sie zur Positionserfassung und geben Sie in der Erfassungszeile die Produktnummer ein.

3.  Wählen Sie im Menü **Start > Lagersuche**, um den Dialog **Lagerinfo** zu öffnen.
    Die Auswahl im Dialog **Lagerinfo** ist bereits auf den Artikel eingeschränkt, den Sie in der Position erfasst haben. Sie müssen die Anzeige nun weiter filtern, indem Sie z. B. die Einstellungen auf Lagermaße und Bestände über null einschränken.

    *(Abb. G-62: Filter für die Suche nach Lagerartikeln)*
    *   **A Anzeige von Lagermaßen an- oder abschalten**
    *   **B Nur Lagerartikel mit Bestandsmenge größer 0 anzeigen**

4.  Wechseln Sie zum Register **Zukünftiger Lagerbestand**, um zu prüfen, ob die Produktionstermine gefährdet sind.
    Die Anzeige des zukünftigen Lagerbestands im Dialog **Lagerinfo** haben Sie bereits in der Einheit Lagerinfo kennengelernt.
    ⇨ "Anzeige des zukünftigen Bestands" auf Seite G-100

    *(Abb. G-63: Zukünftiger Lagerbestand)*
    Falls die Wiederbeschaffungszeit zu knapp ist, können Sie das Produkt dennoch erfassen und anschließend prüfen, ob ein anderer Lieferant verfügbar ist oder ob Sie den Liefertermin ändern müssen.

5.  Wechseln Sie zurück zum Register **Lagersuche** und klicken Sie doppelt auf den Lagerartikel, den Sie in die Positionserfassung übernehmen wollen.

    *(Abb. G-64: Lagerartikel auswählen)*
    Der Dialog **Lagerinfo** wird geschlossen und die Daten in der Positionserfassung werden aktualisiert.

6.  Erfassen Sie alle Positionsdaten und kehren Sie zurück zum Dokumentenkopf.
    Wenn die Wiederbeschaffungszeiten nicht ausreichen, können Sie sich die betroffenen Artikel im Dialog **Liefertermin ändern** anzeigen lassen.

7.  Klicken Sie auf die Symbolschaltfläche neben dem Versandtag, um den Dialog zu öffnen.

    *(Abb. G-65: Liefertermin im Auftrag prüfen)*
    *   **A Liefertermin prüfen**
    *   **B Produkte mit zu geringem Lagerbestand**
    *   **C Übersicht über die möglichen Lieferanten und Liefertermine zum markierten Produkt**

    Alternative Lieferanten aus der Lieferantenkartei werden mit der hinterlegten Wiederbeschaffungszeit und dem entsprechenden Termin angezeigt.
    Mit einem Doppelklick auf den Artikel in der oberen Liste (B) öffnen Sie den Dialog **Lagerinfo** mit den Details zu den Artikeln.

8.  Wenn der geplante Liefertermin gefährdet ist, haben Sie folgende Möglichkeiten:
    *   Wechseln Sie den Lieferanten für die fragliche Position oder für den gesamten Auftrag.
    *   Ändern Sie den Liefertermin und benachrichtigen Sie den Kunden.
    Diese Handlungsschritte sind im Tutorial zum Verkauf ausführlich beschrieben.

9.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert. Sie können jetzt die Reservierung der Lagerartikel prüfen.

### Buchungen prüfen

In dieser Einheit lernen Sie, wie Sie die Buchungen der Lagerartikel prüfen können. Die Position wird nach dem Speichern reserviert. Der Warenabgang wird in der Regel mit dem Druck des Lieferscheins gebucht. Dieser Druck ist von den Einstellungen in der Statusverwaltung abhängig.
⇨ "Statusänderungen durch Zu- und Abgänge" auf Seite G-35

**So prüfen Sie die Buchungen**

1.  Öffnen Sie den Dialog **Buchungsjournal**, wie in der Einheit Abfragen beschrieben.
    ⇨ "Buchungsjournal anzeigen" auf Seite G-90

2.  Schränken Sie die Auswahl auf den Auftrag ein, zu dem Sie die Reservierung prüfen wollen.
    In der Übersicht werden alle Auftragspositionen mit dem aktuellen Buchungstyp aufgelistet.

    *(Abb. G-66: Buchung - reserviert)*
    Im Buchungsjournal wird die Buchungsart **reserviert** nur so lange angezeigt, bis der Warenabgang gebucht wurde.

Nach dem Warenabgang werden die Auftragspositionen als **ausgeliefert** gekennzeichnet.

*(Abb. G-67: Buchung - ausgeliefert)*

In der Auftragshistorie werden die einzelnen Statusänderungen anhand des Drucks und der Lagerbuchungen dargestellt.

*(Abb. G-68: Auftragshistorie)*

### Übungen

*   Erfassen Sie einen Auftrag mit vorhandenen Lagerprodukten und prüfen Sie die Einträge im Buchungsjournal:
    *   Nach der Erfassung des Auftrags.
    *   Nach dem Druck des Lieferscheins. Welche Änderungen sehen Sie?
*   Erfassen Sie einen Auftrag und prüfen Sie dabei den Lagerbestand und die Reservierungen.
*   Erstellen Sie eine Rechnung zu dem Auftrag und prüfen Sie die Lagerreservierungen erneut.

### Manuelle Lagerbestellung

**Lernziele**
*   Besonderheiten der Lagerbestellung in der Dokumentenverwaltung kennenlernen.

**Nutzen**
*   Mit manuellen Lagerbestellungen ergänzen Sie Lagerbestände, z. B. für Großaufträge, zu denen die automatische Nachbestellung nicht ausreicht.

**Merke**
*   **Dokumententyp**: Das Dokument **Lagerbestellung** ist ein eigener Dokumententyp. Nur bei Bestellungen aus einer Lagerbestellung kann der Wareneingang auf das Lager gebucht werden.
*   **Voreinstellungen**:
    *   Stammdaten:
        *   Produktverwaltung
        *   Lieferantenkartei
    *   Firmendaten:
        *   Register **Parameter**
        *   Register **Lager / EK / EDI**

### Lagerbestellung manuell erfassen

Bestellungen von Lagerartikeln können automatisch ausgelöst oder manuell erfasst werden. Die automatischen Bestellvorschläge haben Sie bereits in der Einheit zur automatischen Lagerbestellung kennengelernt.
⇨ "Lagerbestellung (automatisch)" auf Seite G-107

In dieser Einheit lernen Sie, wie Sie eine Lagerbestellung manuell erfassen. Die Erfassung von Dokumenten ist ausführlich in den Parts Verkauf und Einkauf beschrieben. Die folgende Handlungsanleitung konzentriert sich daher auf die wichtigsten Schritte.

**So erfassen Sie eine Lagerbestellung manuell**

1.  Wählen Sie im Menü **Dokumente > Bestellung > Bestellung**.
    Der Dialog **Dokumentenverwaltung** wird geöffnet.
    ⇨ Verkauf, "Dokument - Kopfdaten" auf Seite C-417

2.  Erfassen Sie den Dokumentenkopf. Tragen Sie mindestens den Lieferanten und das Lieferdatum ein.

    *(Abb. G-69: Lagerbestellung)*
    *   **A Dokumententyp**
    *   **B Einstellen des Dokumententyps**

3.  Wählen Sie im Feld **Typ (B)** den Eintrag **Lagerbestellung**.
    Wenn Sie einen anderen Dokumententyp einstellen, wird der Wareneingang nicht automatisch in den Lagerbestand gebucht.

4.  Erfassen Sie die Position(en).

    > **Positionen ohne Lagerkennzeichen**
    > Wenn Sie Lagerbestellungen mit Positionen erfassen, die nicht als Lagerartikel geführt werden, werden diese im Wareneingang nicht angezeigt. Sie können in den **Stammdaten > Firma > Firmendaten > Register Lager / EK/ EDI** jedoch die entsprechende Option aktivieren.
    > ⇨ "Firmendaten - Lager / EK / EDI" auf Seite G-32

5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.

6.  Drucken und versenden Sie die Bestellung.
    Dieser Vorgang ist im Part Verkauf beschrieben.
    ⇨ Tutorial, "Auftragskopf" auf Seite C-39

### Übungen

*   Prüfen Sie die Lagerbestände für einen Lagerartikel.
*   Erfassen Sie eine Lagerbestellung manuell und prüfen Sie im Dialog **Lagerinfo** die entsprechenden Werte erneut.

## Produktionsaufträge

### Lernziele

*   Produktionsauftrag kennenlernen.
*   Manuelle und automatische Erstellung von Produktionsaufträgen kennenlernen.

### Nutzen

*   Produktionsaufträge werden verwendet, um den eigenen Lagerbestand aufzufüllen.
*   Produktionsaufträge können bei Unterdeckung des Mindestbestands automatisch erzeugt werden, wenn in der Lieferantenkartei die Umleitung auf einen internen Kunden aktiviert ist.

### Merke

*   **Beschaffungsart**: Alle Artikel, die in einem Produktionsauftrag erfasst werden, müssen die Beschaffungsart **Produktion** haben.
*   **Buchungsart**: Im Gegensatz zu normalen Aufträgen werden die erfassten Positionen nicht im Lager reserviert, sondern als **bestellt** markiert.
*   **Lagerzugang**: Der Lagerzugang aus Produktionsaufträgen kann manuell oder automatisch gebucht werden:
    *   Manuelle Statusumsetzung im Modul **Fertigung**.
    *   Automatische Status-Rückmeldungen aus der Produktion.
*   **Voreinstellungen**:
    *   Lagerverwaltung:
        *   Mindestbestand
        *   Bestellmenge
    *   Stammdaten:
        *   Produktverwaltung
        *   Partnerverwaltung (interner Kunde)
        *   Lieferantenkartei (Umleitung auf internen Kunden)
    *   Firmendaten:
        *   Register **Parameter**
        *   Register **Lager / EK / EDI > Erfassungsstelle**

### Lagerartikel im Produktionsauftrag

Produktionsaufträge werden verwendet, um den eigenen Lagerbestand aufzufüllen. Alle Artikel, die in einem solchen Auftrag erfasst werden, werden automatisch auf die Beschaffungsart **Produktion** umgesetzt. Im Gegensatz zu Kunden-Aufträgen werden die Positionen nicht im Lager reserviert, sondern als **bestellt** markiert.

*(Abb. G-70: Positionserfassung – Beschaffungsart Produktion)*
*(Abb. G-71: Auftragserfassung – Dokumententyp Produktionsauftrag)*

Produktionsaufträge können auf unterschiedliche Weise erfasst werden:

*   Manuelle Erfassung eines neuen Dokumentes.
*   Kopieren eines gespeicherten (Dummy-)Auftrags.
*   Automatische Erstellung durch Unterdeckung des Lagerbestands.

### Manuelle Erfassung durch Kopieren

Wenn Sie regelmäßig Produktionsaufträge erfassen, können Sie den zuvor erfassten Auftrag kopieren und sich so die Arbeit erleichtern.

*   Vor dem Kopieren müssen Sie den Dokumententyp des Ziel-Dokuments auf **Produktionsauftrag** einstellen.
*   Wenn nur bestimmte Positionen aus dem Auftrag übernommen werden sollen, können Sie diese auswählen.
*   Im neuen Dokument können Sie die Daten anpassen.

*(Abb. G-72: Produktionsauftrag durch Kopieren erstellen)*
*   **A Kopieren von Auftrag nach Auftrag**
*   **B Dokumententyp des Ziel-Auftrags**

Eine ausführliche Beschreibung der Funktion Dokumente kopieren finden Sie im Part Verkauf.
⇨ Verkauf, "Neuer Auftrag durch Kopieren" auf Seite C-245

### Einstellungen in der Lieferantenkartei

Wenn im Dialog **Lagerverwaltung** ein Mindestbestand und eine (Standard-) Bestellmenge für den Lagerartikel hinterlegt sind, kann das System automatische Bestellvorschläge generieren. Diese werden im Dialog **Lagerbestellung** aufgelistet.

Normalerweise werden auf diesem Weg Bestellungen vom Typ **Lagerbestellung** generiert. Wenn jedoch in der Lieferantenkartei statt eines Standard-Lieferanten ein interner Kunde hinterlegt ist, können Produktionsaufträge automatisch erzeugt werden.

*(Abb. G-73: Interner Kunde für Produktionsaufträge)*
*   **A Produkt, für das Produktionsaufträge erzeugt werden sollen**
*   **B Umleitung auf internen Kunden**
*   **C Auswahl des Kunden**

In der Lieferantenkartei wird ein interner Kunde eingetragen, für den der Produktionsauftrag automatisch erfasst wird. Die Option **Interner Kunde** kann auf der Ebene der Warengruppen oder der Produkte aktiviert werden. Dabei haben die Einstellungen für Produkte Vorrang vor denen für Warengruppen.

### Bestellmenge nach Bestandsprüfung

Das Programm prüft, ob die aktuellen Lagerbestände zuzüglich der bereits bestellten Mengen und abzüglich der reservierten Mengen den Mindestbestand unterschreiten.

Wenn dies der Fall ist, wird als Vorschlag ein Vielfaches der (Standard-) Bestellmenge angezeigt.

**Manuelle und automatische Lagerbestellung**

*Ablaufplan (Abb. G-74: Lagerbestellung vs. Produktionsauftrag)*
1.  Lagerbestellung / Lagerort wird geprüft.
2.  **Frage:** Mindestbestand unterschritten?
    *   **Ja:** Weiter zu Schritt 3.
3.  **Frage:** Standard-Bestellmenge vorhanden?
    *   **Ja:** Weiter zu Schritt 4.
4.  Suche in der Lieferanten-Kartei.
5.  **Frage:** Standard-Lieferant?
    *   **Ja:** Erzeuge "Bestellvorschlag Lagerbestellung".
6.  **Frage:** Interner Kunde?
    *   **Ja:** Erzeuge "Produktionsauftrag Dokumentenverwaltung".

In diesem Ablaufplan ist dargestellt, wie A+W Business auf die unterschiedlichen Voreinstellungen in der Lieferantenkartei reagiert.

**Bestellmenge**
Der Multiplikator wird so berechnet, dass durch den Vorschlag der Mindestbestand überschritten wird.

*(Abb. G-75: Mengenangaben für Lagerartikel (Dialog Lagerverwaltung))*

> **Beispiel**
> Das ESG mit der Produktnummer 4008 wird als Lagerartikel geführt.
> Aktueller Lagerbestand: 10 Stk.
> Mindestbestand: 30 Stk.
> Bestellmenge: 5 Stk.
>
> Die Bestellmenge für das ESG 4008 wird folgendermaßen berechnet:
> Differenz zwischen aktuellem Bestand und Mindestbestand: 20 Stk. In dieser Differenz ist die Bestellmenge 5 Stk. vier mal enthalten.
> Bestellmenge: 4 x 5 = 20 Stk.
> Aktueller Bestand plus bestellte Menge: 10 + 20 = 30 Stk.

Die errechnete Menge wird in den Bestellvorschlag übernommen. Sie kann im Dialog **Lagerbestellung** angepasst werden.

*(Abb. G-76: Lagerbestellung - Bestellvorschläge)*
*   **A Einschränkung auf Lagerort**
*   **B Bestellvorschlag für Produktionsauftrag**

Wie Sie die Bestellungen bearbeiten und übergeben, haben Sie in der Einheit Lagerbestellung kennengelernt.
⇨ "Lagerbestellung an den Einkauf übergeben" auf Seite G-109

Der Produktionsauftrag wird erst durch die Übergabe erzeugt und in dem Auftragsnummernverwalter angelegt, der zuletzt aktiviert war.

*(Abb. G-77: Produktionsauftrag im Nummernverwalter für Aufträge)*
*   **A Automatisch erzeugter Produktionsauftrag**

Der Produktionsauftrag kann nun als Dokument geöffnet werden.

*(Abb. G-78: Dokument Produktionsauftrag)*
*   **A Auftragskopf – Produktionsauftrag**
*   **B Bestellte Menge**

Der Produktionsauftrag kann bearbeitet und an die Produktion weitergeleitet werden.

### Lagerzugang durch Produktionsauftrag

In den Firmendaten müssen Sie ist im Register **Lager / EK / EDI** den Grenzstatus für die Erfassungsstellen einstellen, ab dem ein Auftrag als produziert gilt. Als Grenzstatus gilt der für die gewählte Erfassungsstelle hinterlegte Status.

*(Abb. G-79: Firmendaten – Lager / EK / EDI: Erfassungsstelle für Statusumsetzung)*

Den Lagerzugang aus einem Produktionsauftrag können Sie auf zwei Arten erfassen:

*   Sobald durch eine Produktionsrückmeldung der Status des Produktionsauftrages über diesen Status hinaus steigt, wird der Lagerzugang automatisch verbucht.
*   Wenn Sie nicht mit Produktionsrückmeldungen arbeiten, können Sie den Zugang über die manuelle Statusmeldung im Modul **Fertigung** erfassen. Wenn Sie den Produktionsauftrag dort auf einen Status setzen, der über dem o. g. Grenzstatus liegt, werden der Lagerabgang der verbrauchten Materialien und der Lagerzugang der gefertigten Lagerartikel automatisch gebucht.

Wenn kein abweichender Lagerort definiert wurde, werden die Auftragsmengen dem Standard-Lagerort zugeordnet.

Die Verbuchung von Produktionsaufträgen wird im Part **Fertigung** ausführlich behandelt.

### Ergänzende Informationen

⇨ Stammdaten, "Firmendaten - Lager/EK/EDI" auf Seite B-957
⇨ Verkauf, "Auftragskopf" auf Seite C-39
⇨ Verkauf, "Bestellkennzeichen ändern" auf Seite C-310
⇨ Fertigung, "Produktionsaufträge" auf Seite E-130

## Inventur

In diesem Themenblock lernen Sie, wie Sie die Bestandszahlen Ihres Lagers in A+W Business durch eine Inventur bereinigen.

Dazu gehören folgende Lerneinheiten:

*   "Periodische Inventur" auf Seite G-142
*   "Erstinventur" auf Seite G-158

### Periodische Inventur

**Lernziele**
*   Inventurablauf kennenlernen.
*   Dialoge für die Inventur kennenlernen.
*   Inventur durchführen.

**Nutzen**
*   Mit der Inventur können Sie die Bestandszahlen in A+W Business bereinigen.
*   Bei großen Lagerorten können Sie die Inventur so organisieren, dass der normale Geschäftsbetrieb möglichst wenig behindert wird.

**Merke**
*   **Keine Bestandsänderung während der Inventur**: Am Zähltag dürfen keine Aufträge, Bestellungen und Wareneingänge erfasst werden, Ware darf nicht aus dem Lager entnommen oder in es hineingestellt werden. Der Sollbestand sollte am Zähltag ermittelt werden.
*   **Verlauf der Inventur**: Die Inventur wird in folgenden Schritten durchgeführt:
    *   Inventurliste erstellen
    *   Sollbestand ermitteln
    *   Inventurwerte erfassen
    *   Inventur abschließen
*   **Inventur splitten**: Bei großen Lagerorten ist es sinnvoll, die Inventur in kleineren Einheiten durchzuführen.
*   **Kisten gesondert inventarisieren**: Für Kisten wird eine eigene Inventurliste erstellt. Die vorhandenen Kisten werden dann einzeln per Scanner erfasst.
*   **Keine Änderungen an den Stammdaten der Produkte**: Sobald die Inventurliste erstellt ist, werden in der Produktverwaltung (Stammdaten) alle Produkte gekennzeichnet, die in der Inventurliste aufgeführt sind. Die Beschaffungsart und das Lagerkennzeichen in diesen Produkten sind dann gesperrt. Die Kennzeichnung wird gelöscht, sobald die Inventur abgeschlossen ist.
*   **Inventurliste ergänzen**: Ergänzungen dürfen nur vor Ermittlung des Sollbestands eingefügt werden.
*   **Sollbestand in der Zählliste**: Wenn in der Zählliste der Sollbestand gedruckt werden soll, müssen Sie den Sollbestand vor dem Druck ermitteln.
*   **Inventurabschluss pro Inventurliste**: Der Inventurabschluss kann nur einmal pro Inventurliste durchgeführt werden.
*   **Voreinstellungen**: Keine

### Bestandaufnahme

In jedem Geschäftsjahr muss mindestens einmal durch körperliche Bestandsaufnahme geprüft werden, ob der jeweilige Buch- bzw. Sollbestand in der A+W Business-Lagerwirtschaft mit dem tatsächlich vorhandenen Bestand (Istbestand) übereinstimmt. Für diese gesetzlich vorgeschriebene Jahresinventur werden Inventurlisten erstellt, anhand derer die Bestände gezählt und erfasst werden können. Die Inventur stellt den Bestand des Vorratsvermögens nach Art, Menge und Wert fest.

Grundlage jeder Inventur ist die Inventurliste, die sich auf ausgewählte Lagerartikel und/oder Lagerorte beziehen kann. Auf diese Weise kann die Inventur in mehreren Etappen durchgeführt werden und behindert so das Tagesgeschäft weniger.

Bei der Inventur erhalten Sie von A+W Business Inventurlisten und Sollbestände. Die Inventur können Sie nach konventionellen Methoden durchführen oder für Kisten auch mit Hilfe der Barcode-Lesung.

Die Inventur wird mit dem Inventurabschluss beendet. Erst damit werden die Bestandsmengen in A+W Business aktualisiert.

#### Istbestand

Die Istbestände werden anhand von Zähllisten eingegeben. Dabei können neue Lagerartikel angelegt werden. Während der Inventur sind die Lagerartikel für die Dokumentenerfassung nicht gesperrt, wenn sie sich in der Inventurliste befinden. Daher sollten am Zähltag keine Aufträge, Bestellungen und Wareneingänge erfasst werden.

#### Sollbestand

Der Sollbestand muss spätestens am Tag der Zählung ermittelt werden. Damit haben Sie die Möglichkeit, die Inventurliste zu einem früheren Zeitpunkt zu erstellen, als die Zählung und die Erfassung der gezählten Mengen und den Inventurabschluss.

**Beispiel**

| Aktion | Datum | Bestand | Sollbestand |
| :--- | :--- | :--- | :--- |
| Inventurliste erstellt | 15.12. | | 100 |
| Zählung Istbestand | 31.12. | 80 | 100 |
| Verkauf | 01.01. bis | -30 | -30 |
| Einkauf | 14.01. | +10 | +10 |
| | 15.01. | Tatsächlicher Istbestand 60 | 80 |
| Inventurabschluss | | Sollbestand neu: | 60 |

Mit dem Inventurabschluss wird der Istbestand als neuer Sollbestand im System gespeichert.

Der Sollbestand kann wahlweise in den Zähllisten gedruckt werden. Wenn Sie den Sollbestand nicht drucken, können Sie "gezählte" Mengen, die aufgrund des Sollbestandes geschätzt wurden, nahezu ausschließen.

**qm-Artikel**
Werden für einen qm-Artikel einzelne Blätter in bestimmten Abmessungen gezählt, so können diese als Stückartikel erfasst werden. Beim Inventurabschluss werden diese dann in qm umgewandelt und als solche in das Lager gebucht (in Ausdrucken des Inventurabschlusses stehen allerdings die gezählten Stückzahlen).

**Inventarisieren einer Kiste**
Zum Inventarisieren der Kiste, also um sie in einer Inventurliste zu erfassen, wird zunächst eine Inventurliste erstellt und dafür der Sollbestand ermittelt. Danach werden die Identnummer der Kiste, der Lagerort und ggf. eine abweichende Blattanzahl gescannt oder manuell eingegeben. Der Scanvorgang fügt diese Kiste immer der aktuellsten Inventurliste hinzu. Anschließend wird ggf. in der Inventurverwaltung noch der restliche Lagerbestand erfasst und am Ende der Inventurabschluss gebucht.

*(Abb. G-80: Zählliste mit Feldern für die gezählten Mengen)*

Die gezählten Mengen werden in der Zählliste eingetragen und später in der Inventurverwaltung erfasst.
⇨ "Inventurwerte erfassen" auf Seite G-152

### Inventurliste erstellen

Für die Inventur werden Listen benötigt, in denen die manuellen Zählmengen festgehalten werden. Diese Listen können nach verschiedenen Kriterien ausgeführt und gedruckt werden.

Wenn beim Druck festgestellt wird, dass bestimmte Artikel auf der Liste fehlen, kann eine Nachtragsinventur angehängt werden. Damit müssen nicht alle Listen neu gedruckt werden.

> **Keine Änderungen an den Stammdaten der Produkte**
> Sobald die Inventurliste erstellt ist, werden in der Produktverwaltung alle Produkte gekennzeichnet, die in der Inventurliste aufgeführt sind. Die Beschaffungsart und das Lagerkennzeichen in diesen Produkten sind dann gesperrt.
> Wenn die Inventur abgeschlossen ist, wird die Kennzeichnung gelöscht und die Daten können wieder bearbeitet werden.

In dieser Einheit lernen Sie, wie Sie Inventurlisten erstellen und wieder öffnen. Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:

*   "So beginnen Sie eine Inventur" auf Seite G-146
*   "So drucken Sie die Zähllisten" auf Seite G-148
*   "So laden Sie eine gespeicherte Inventurliste" auf Seite G-149
*   "So ergänzen Sie eine Inventurliste vor dem Zählen" auf Seite G-149

**So beginnen Sie eine Inventur**

1.  Wählen Sie im Menü **Lagerwirtschaft > Inventur > Inventurliste**.
    Der Dialog **Inventurliste** wird geöffnet.
    ⇨ Softwarereferenz, "Inventurliste" auf Seite G-167

2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.

    *(Abb. G-81: Felder für neue Inventurliste freigeschaltet)*
    *   **A** Alle Artikel oder Folge von Artikelnummern
    *   **B** Datum der Inventur
    *   **C** Eingrenzungen
    *   **D** Lagerbewertung
    *   **E** Sortierung der Liste

    Als Name wird für die Inventur ein Datum (B) verwendet. Standardmäßig wird das aktuelle Tagesdatum vorgeschlagen. Sie können jedes beliebige andere Datum eintragen oder auswählen.

3.  Wählen Sie die Artikel (A) für die Inventur aus:
    *   **Alle Artikel**: Sie können die Inventur für alle Artikel durchführen, die als Produkte in den Stammdaten erfasst sind. In diesem Fall sind die Felder für die Artikelnummern gesperrt. Bei der Erstinventur aktivieren Sie diese Option, bei allen anderen Inventuren können Sie die Inventurlisten auf bestimmte Artikel beschränken.
    *   **Artikelnummer**: Sie können die Inventurliste auf eine Folge von Artikelnummern einschränken. Die Felder sind gesperrt, wenn Sie die Option **Alle Artikel** markiert haben.

4.  Schränken Sie die Liste ggf. weiter ein (C):
    *   **Nur Produkte mit Lagerbestand > 0**: Sie können die Inventur auf die Lagerartikel mit Bestand einschränken. Wenn Sie die Checkbox nicht markieren, wird der komplette Produktstamm in die Inventurliste aufgenommen, sofern die Auswahl nicht durch andere Kriterien eingeschränkt wird.
    *   **Nur Produkte mit zugeordnetem Lagerprodukt**: Sie können die Inventur auf die Lagerartikel aus der Lagerverwaltung einschränken. Wenn Sie die Checkbox nicht markieren, wird der komplette Produktstamm inklusive Lagermaßtabelle in die Inventurliste aufgenommen, sofern die Auswahl nicht durch andere Kriterien eingeschränkt wird.
    *   **Nur Produkte mit Lagerführung in dem Produkt**: Sie können die Inventur auf die Produkte mit der Beschaffungsart **Lagerentnahme** einschränken.
    *   **Keine Kisten mit Identnummer und Bestand = 0**: Im Lagerbestand können sich Kisten befinden, die bereits ausgeliefert sind, aber nicht gelöscht wurden. Deren Bestand wird korrekt mit 0 angezeigt. Diese Kisten können Sie ausblenden, da zu ihnen keine Menge erfasst werden wird.
    *   **Nur für bestimmten Lagerort**: Mit dieser Einstellung werden die Felder für die Auswahl des Lagerorts freigeschaltet. Wenn Sie die Inventur nur für bestimmte Lagerorte durchführen möchten, können Sie für diese je eine eigene Inventurliste erstellen. Beachten Sie dabei, dass Artikel auch auf den Lagerort `<k.A.>` gebucht sein können. Wenn Sie eine gesamte Inventur durchführen wollen, können Sie die Inventurliste auch im Druck nach Lagerorten splitten.

5.  Wählen Sie die Art der Lagerbewertung (D) aus.
    Wenn Sie in den Firmendaten die Optionen für die EK-Berechnung aktiviert haben, können Sie die Lagerbewertung folgendermaßen berechnen lassen:
    *   **EK-Preisliste**: Die Einzelpreise der Produkte aus der EK-Tarifzuordnung werden herangezogen.
    *   **Niedrigster EK**: Für alle Artikel wird jeweils der niedrigste Wert herangezogen.
    *   **Geschnittener EK**: Für alle Artikel wird jeweils der Durchschnitts-EK herangezogen. Dazu muss in den Firmendaten die Option **Durchschnitts-EK** aktiviert sein.

6.  Wählen Sie die Art der Sortierung (E) aus.
    Die Sortierung der Artikel auf der Inventurliste sollte sich nach den ausgewählten Kriterien richten. Die Option **Abmessung** ist z. B. für Lagermaße sinnvoll.

7.  Wählen Sie im Menü **Start > Speichern**, um die Inventurliste zu erstellen.

Die Inventurliste wird in der Übersicht angezeigt. Sie können jetzt die Zähllisten drucken und/oder den Sollbestand ermitteln.

> **Keine Änderungen an den Stammdaten der Produkte**
> Sobald die Inventurliste erstellt ist, werden in der Produktverwaltung (Stammdaten) alle Produkte gekennzeichnet, die in der Inventurliste aufgeführt sind. Die Beschaffungsart und das Lagerkennzeichen in diesen Produkten sind dann gesperrt. Sobald die Inventur abgeschlossen ist, wird die Kennzeichnung gelöscht und die Daten können wieder bearbeitet werden.

**So drucken Sie die Zähllisten**
Wenn in der Zählliste der Sollbestand gedruckt werden soll, müssen Sie vor dem Druck den Sollbestand ermitteln.
⇨ "So ermitteln Sie den Sollbestand zu einer Inventurliste" auf Seite G-151

1.  Wählen Sie im Menü **Lagerwirtschaft > Inventur** und wählen Sie das Datum der Inventurliste aus.

2.  Wählen Sie im Menü **Start > Suchen**, um die Inventurliste zu laden.
    Diese Schritte entfallen, wenn Sie die Zählliste sofort nach dem Erstellen der Inventurliste drucken.

3.  Wählen Sie im Menü **Druck > Drucker**.
    Wenn Sie das Ergebnis zunächst am Bildschirm prüfen möchten, wählen Sie **Bildschirm**. Sie können dann den Druck starten, wenn Sie mit dem Ergebnis zufrieden sind. Die folgenden Schritte sind für beide Einstellungen gleich.

    *(Abb. G-82: Inventur - Zählliste drucken)*
    *   **A Seitenumbruch**
    *   **B Artikel, die gedruckt werden sollen**
    *   **C Sortierung**
    ⇨ Softwarereferenz, "Listendruck" auf Seite G-171

    Drucken Sie die Zähllisten so aus, dass sie den Aufgaben Ihrer Inventur-Mitarbeiter entsprechen.

4.  Bestimmen Sie, an welcher Stelle eine neue Seite (A) gedruckt werden soll.
    Wenn Sie keine unterschiedlichen Lagerorte angelegt haben, entfällt diese Einstellung. Wenn Sie die Zählbereiche nach Lagerorten verteilt haben, machen Sie den Seitenumbruch nach den entsprechenden Lagerorten. Für den Druck müssen Sie mindestens **Lagerhaus** (Ebene 1) markieren.

5.  Legen Sie fest, welche Lagerware (B) in der Liste gedruckt werden soll.
    Wenn an den angegebenen Lagerorten unterschiedliche Lagerartikel vorkommen, können Sie nach **Fertigprodukten** oder **Rohmaterial** unterscheiden. Fertigprodukte sind alle Lagerartikel, die nicht im Lager für Rohmaterial gelagert sind.
    Die Zuordnung der Eigenschaften **Fertigprodukte** und **Rohmaterial** haben Sie in der Lagerdefinition getroffen.
    ⇨ "Lagerort definieren" auf Seite G-24

6.  Wählen Sie die Sortierung (C) der Artikel auf der Zählliste so, dass sie sich nach den ausgewählten Kriterien richten. Die Option **Artikel** ist z. B. dann sinnvoll, wenn Sie das Lager nach Produkten aufgebaut haben.

7.  Klicken Sie auf **[OK]**, um den Druck zu starten.
    Die Liste wird gedruckt und kann nun zur Zählung verwendet werden.

**So laden Sie eine gespeicherte Inventurliste**

1.  Wählen Sie im Menü **Lagerwirtschaft > Inventur**.
2.  Wählen Sie im Feld **Inventurdatum** das Datum aus, unter dem die Inventurliste gespeichert wurde.
3.  Wählen Sie im Menü **Start > Suchen**, um die Inventurliste zu laden.
    Die Inventurliste wird angezeigt.

**So ergänzen Sie eine Inventurliste vor dem Zählen**
Wenn Sie den Sollbestand zu einer Inventurliste bereits ermittelt haben, können Sie die Liste nicht mehr ergänzen. Beenden Sie in diesem Fall die Inventur und erfassen Sie die fehlenden Artikel in einer neuen Inventurliste.

1.  Wählen Sie im Menü **Lagerwirtschaft > Inventur**.
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln. Die Felder werden freigeschaltet.
3.  Wählen Sie die Inventurliste aus, zu der Sie weitere Artikel hinzufügen möchten.
4.  Wählen Sie die Lagerartikel und/oder Standorte aus.
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.

Eine Abfrage wird angezeigt, in der Sie den Vorgang abbrechen oder zu Ende führen können.

6.  Wählen Sie:
    *   **[Ja]**: Die bestehende Liste wird angezeigt und die neuen Artikel werden am Ende hinzugefügt.
    *   **[Nein]** oder **[Abbrechen]**: Die Abfrage wird geschlossen. Sie können das Datum und weitere Kriterien ändern und damit eine neue Inventurliste erstellen.

### Sollbestand ermitteln

Der Sollbestand muss für jede Inventurliste durchgeführt werden. Er gibt die Mengen an, die sich laut System im Lager befinden müssen. Wenn der Sollbestand mit in den Zähllisten gedruckt werden soll, muss er vor dem Druck der Liste ermittelt werden.

> **Keine Lagerbuchungen am Zähltag**
> Nachdem der Sollbestand ermittelt wurde, müssen die Bestände gezählt werden. Am Tag der Zählung dürfen keine Lagerartikel entnommen und keine Lagerbewegungen gebucht werden, bis die Zählung abgeschlossen ist. Dies betrifft alle manuellen oder automatischen Lagerab-/zugänge und alle Wareneingänge für Lagerbestellungen. A+W Business wird nicht automatisch für Buchungen gesperrt.

In dieser Einheit lernen Sie, wie Sie den Sollbestand für eine gespeicherte Inventurliste ermitteln.
