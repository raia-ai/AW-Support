---
title: "A+W Business - Lagerwirtschaft Tutorial & Softwarereferenz"
source: "D-AWBusiness-HB_28.pdf"
tags: ["AW Business", "Lagerwirtschaft", "Inventur", "Bestandsführung", "ERP", "Tutorial", "Software-Referenz", "Bestellwesen", "Produktionsauftrag"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Dieses Dokument ist ein umfassendes Handbuch für das Modul Lagerwirtschaft in der A+W Business Fertigungssoftware. Es enthält einen Tutorial-Teil, der Benutzer durch verschiedene Prozesse wie Lagerabfragen, Inventur und Bestellungen führt, sowie einen Softwarereferenz-Teil, der die Dialoge und Funktionen detailliert beschreibt."
long_description: "Dieses Dokument dient als detaillierte Anleitung und Referenz für das Modul Lagerwirtschaft der A+W Business Fertigungssoftware. Es ist in zwei Hauptteile gegliedert: ein Tutorial und eine Softwarereferenz. Der Tutorial-Teil (gekennzeichnet durch 'Tutorial' in der Kopfzeile) bietet schrittweise Anleitungen für praxisnahe Anwendungsfälle. Dazu gehören das Durchführen von Lagerabfragen, das Anzeigen von Buchungsjournalen und Lagerhistorien, das Drucken von reservierten Artikeln, das Analysieren von Lagerstatistiken zur Identifizierung von 'Rennern und Pennern', und die Durchführung von Lagerbewertungen. Ein weiterer Schwerpunkt liegt auf der Verwaltung von Lagerinformationen, der Anzeige von Beständen in der Lagersuche und der Interpretation des zukünftigen Lagerbestands unter Berücksichtigung von Reservierungen und Bestellungen. Es werden sowohl automatische als auch manuelle Lagerbestellungen sowie die Erstellung von Produktionsaufträgen zur Auffüllung des Eigenbestands behandelt. Der zweite Teil, die Softwarereferenz (gekennzeichnet durch 'Softwarereferenz' in der Kopfzeile), bietet eine systematische Beschreibung aller Dialoge, Menüs und Felder des Moduls. Hier finden Benutzer detaillierte Erklärungen zu den Funktionen der Inventur (periodisch und Erstinventur), der Lagerverwaltung, der Lagerbewegungen, der Abfragen und der Bestellungen. Dieser Teil dient als Nachschlagewerk, um spezifische Einstellungen und Optionen zu verstehen. Das gesamte Dokument ist für Anwender konzipiert, die für die Bestandsführung, den Einkauf und die Produktionsplanung verantwortlich sind."
---

# Tutorial - Lagerwirtschaft

---
## Lagerabfrage

Mit verschiedenen Abfragen können Sie sich einen Überblick über die Buchungen, den Gesamtwert des Lagerbestands, statistische Auswertungen und eine Übersicht über Reservierungen anzeigen lassen.

Damit kann auch nachverfolgt werden, welche Daten von wem geändert wurden.

### Buchungsjournal

Das Buchungsjournal enthält Auswertungen zu den Lagerbuchungen, die aus Aufträgen und Bestellungen rühren. Sie können sich z. B. die Lagerbuchungen pro Produkt anzeigen lassen.

### Lagerhistorie

Über die Historie können Sie sich einen Überblick über das Tagesgeschehen im Lager pro Produkt verschaffen.

### Lagerstatistik

Die Lagerstatistik gibt Ihnen Aufschluss darüber, welche Ihrer Lagerartikel Renner und welche Ladenhüter sind. Damit haben Sie ein Kriterium, ob Artikel in das Lager auf- bzw. herausgenommen werden sollten.

Die Entwicklung einzelner Lagerartikel kann über einen gewählten Zeitraum betrachtet werden, z. B. über ein ganzes Jahr oder nur über einen Monat.

Die Auswertungen zeigen Anfangs- bzw. Endbestände und Zu- bzw. Abgänge Ihrer Lagerartikel pro Monat. Damit können Sie sich über die Umschlagshäufigkeit, die durchschnittliche Lagerdauer und den durchschnittlichen Lagerbestand Ihrer Lagerartikel informieren.

### Lagerbewertung

Der aktuelle Lagerwert des gesamten Lagers kann jederzeit und außerhalb der Inventur abgefragt werden.

Daneben werden in der Lagerverwaltung zu jedem einzelnen Lagerartikel der höchste, niedrigste und Durchschnitts-EK und der zugehörige Lagerwert angezeigt.

### Reservierte Lagerartikel

Lagerartikel, die durch Aufträge reserviert sind, können pro Nummernverwalter aufgelistet werden. In der Ausgabe werden die reservierten Lagerartikel pro Artikelnummer und Lagerort dargestellt.

---

## Buchungsjournal anzeigen

In dieser Einheit lernen Sie, wie Sie welche Kriterien im Buchungsjournal und/oder in der Lagerhistorie einsetzen können. Diese beiden Dialoge sind analog aufgebaut, geben aber unterschiedliche Sachverhalte wieder:

*   Im Buchungsjournal werden alle automatisch durchgeführten Buchungen angezeigt. Aufträge können nur so lange herangezogen werden, wie sie nicht archiviert und gelöscht sind.
*   In der Lagerhistorie werden alle manuellen und automatischen Buchungen, Neuanlagen, Umbuchungen und Korrekturen aus der Inventur angezeigt.

In dieser Anleitung werden die beiden Dialoge am Beispiel Buchungsjournal beschrieben.

### So lassen Sie sich Reservierungen anzeigen

1.  Wählen Sie im Menü **Lagerwirtschaft > Abfragen > Buchungsjournal**.

    *(Abb. G-41 Buchungsjournal)*

    *   **A**: Buchungsart
    *   **B**: Abfragezeitraum
    *   **C**: Artikel
    *   **D**: Artikelauswahl

    ⇨ Softwarereferenz, “Buchungsjournal" auf Seite G-205

    Sie können die Anzeige der Buchungen mit verschiedenen Filtern einschränken, z. B. auf einen Artikel.

2.  Wählen Sie im Feld **Buchungsart (A)** den Eintrag **reserviert** aus.
    Wenn Sie das Feld frei lassen, werden alle Buchungen angezeigt.

3.  Grenzen Sie die Anzeige ggf. weiter ein, z. B. auf einen Artikel (C, D) und einen Zeitraum (B).

4.  Wählen Sie im Menü **Start > Ausführen**, um das Buchungsjournal zu erzeugen.

    *(Abb. G-42 Buchungsjournal – Ergebnis)*

    Die Reservierungen werden in der Übersicht aufgelistet. Wenn Sie die Anzeige nicht weiter eingeschränkt haben, werden alle Aufträge und Bestellungen berücksichtigt, die noch nicht archiviert sind.

    Auf die gleiche Weise können Sie sich jede einzelne Buchungsart auswerten lassen.

    ⇨ Softwarereferenz, "Buchungsjournal" auf Seite G-205
    ⇨ Softwarereferenz, “Lagerhistorie – Tabelle" auf Seite G-211

---

## Reservierte Lagerartikel drucken

Reservierungen werden in den Dialogen Buchungsjournal, Lagerhistorie und Lagerinfo angezeigt. Im Dialog Reservierte Lagerartikel erhalten Sie eine schnelle Übersicht über die Reservierungen aus Aufträgen in einem Nummernverwalter. In dieser Einheit lernen Sie, wie Sie sich eine Liste dieser reservierten Lagerartikel ausdrucken lassen.

### So drucken Sie sich die Liste der reservierten Lagerartikel

1.  Wählen Sie im Menü **Lagerwirtschaft > Abfragen > Reservierte Lagerartikel**.
    Der Dialog **Reservierungen** wird geöffnet.
    ⇨ Softwarereferenz, "Reservierte Lagerartikel" auf Seite G-218

2.  Wählen Sie den Nummernverwalter aus, in dem die aktuellen Aufträge gesammelt sind.

    *(Abb. G-43 Reservierte Lagerartikel)*

    Die Aufträge werden im Bereich Tabelle aufgelistet. Sie können die Liste aus der Bildschirmanzeige heraus drucken. Über **Menü Druck > Drucker** können Sie die Liste direkt drucken.

3.  Wählen Sie im Menü **Druck > Bildschirm**, um sich die Liste auf den Bildschirm anzeigen zu lassen.

4.  Wählen Sie aus, wo der Druck umgebrochen werden soll.

    *(Dialog Druckoptionen)*

5.  Klicken Sie auf **[OK]**, um die Einstellungen zu übernehmen.
    Der Dialog **Druck - Lagerprotokoll** wird geöffnet.
    Wenn Sie die Ausgabe auf dem Bildschirm gewählt haben, wird die Liste der reservierten Lagerartikel angezeigt.

    *(Abb. G-44 Reservierte Lagerartikel – Ausgabe auf dem Bildschirm)*

    Die reservierten Lagerartikel werden pro Artikelnummer und Lagerort aufgelistet. Bei mehreren Lagerorten wird die Gesamtsumme angezeigt.

    Mit den Schaltflächen können Sie vor- und zurückblättern, wenn die Liste mehr als eine Seite hat.

---

## Lagerstatistik anzeigen

In dieser Einheit lernen Sie, wie Sie sich in der Lagerstatistik verschiedene Lagerkennzahlen eines Produkts anzeigen lassen können.

### So lassen Sie sich die Statistik zu Lagerbeständen anzeigen

1.  Wählen Sie im Menü **Lagerwirtschaft > Abfragen > Lagerstatistik**.
    Der Dialog **Statistik** wird geöffnet.
    ⇨ Softwarereferenz, "Lagerstatistik - Produkte" auf Seite G-213

    Sie können die Anzeige auf ein Produkt und/oder einen Zeitraum einschränken. Wenn Sie keine Auswahl treffen, werden alle Produkte angezeigt.

    *(Abb. G-45 Lagerstatistik – Produktauswahl)*

2.  Wählen Sie im Menü **Start > Ausführen**, um die Auswertung zu erstellen.
    Die Produkte werden den Filtereinstellungen entsprechend aufgelistet.

3.  Markieren Sie einen Eintrag und wechseln Sie zum Register **Statistik**, um die Details auszuwerten.

    *(Abb. G-46 Lagerstatistik – Statistik)*

    Die Werte zum ausgewählten Produkt werden aufgelistet, z. B. die Bestände und Zu- und Abgänge pro Monat, die Umschlagshäufigkeit und Lagerdauer. In der Summenzeile werden die summierten Werte des angezeigten Zeitraums angezeigt.

---

### Übungen

*   Prüfen Sie im Buchungsjournal die Reservierungen für das Float 4 mm.
*   Drucken Sie die Reservierungen eines Float 5 mm für den nächsten Monat aus.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Buchungsjournal" auf Seite G-205
⇨ Softwarereferenz, "Lagerhistorie" auf Seite G-207
⇨ Softwarereferenz, "Lagerstatistik" auf Seite G-212
⇨ Softwarereferenz, "Reservierte Lagerartikel" auf Seite G-218

---

# Lagerinformationen

**Lernziele**
*   Dialog Lagersuche kennenlernen.
*   Änderungen im Bestand und bei den Reservierungen erkennen.

**Nutzen**
*   Mit dem Überblick über die zukünftigen Lagerbestände und Reservierungen erhalten Sie ein weiteres Mittel zur Pflege der Bestände.
*   Sie können erkennen, wann weitere Bestellungen erfasst werden müssen, damit die Produktion nicht unterbrochen wird.

**Merke**
*   **Lagerbestand**: Der Lagerbestand wird beim Wareneingang von Lagerartikeln und nach der Abbuchung aktualisiert. Die Abbuchung wird angestoßen, wenn der Lieferschein oder die Rechnung zu einem Auftrag gedruckt wird.

**Voreinstellungen**
*   **Lieferantenkartei**:
    *   Lieferzeit Tage (Wiederbeschaffungszeit)
    *   Statuszuordnung
*   **Firmendaten**:
    *   Register Lager / EK / EDI > Lagervorschau
*   **Lagerverwaltung**:
    *   Register Lager-Artikel > Hauptartikel

---

## Lagersuche

Im Dialog **Lagersuche** können Sie sich alle Lagerartikel pro Lagerort und Abmessung anzeigen lassen. Diesen Dialog können Sie auch bei der Positionserfassung öffnen. Die Lagersuche ist dann bereits auf einen Lagerartikel eingeschränkt.

*(Abb. G-47 Lagerinfo - Lagersuche)*

*   **A**: Filter zum Einstellen der Suche
*   **B**: Wird als Lagerartikel geführt und entsprechend gebucht
*   **C**: Wird als Lagermaß geführt, ist aber kein Lagerartikel auf Lager, z. B. Bandmaße bei qm-Lager
*   **D**: Bestellartikel, die nicht auf Lager geführt werden, z. B. Lagermaße mit der Beschaffungsart Bestellung

### Bestand

Die Berechnung des Bestands ist abhängig von dem Modus, in dem Sie das Lager führen. Diese Zusammenhänge haben Sie ganz am Anfang der Schulung kennengelernt.
⇨ "Wie soll das Lager geführt werden" auf Seite G-17

Bei der Berechnung von qm-Artikeln wird neben der Reservierung auch der Verschnitt berücksichtigt. Wenn Sie einem oder mehreren Artikeln einen Hauptartikel zugeordnet haben, wird der Bestand nicht mehr für die einzelnen Artikel angezeigt.

Bei der Erfassung eines Auftrags wird die Stückzahl oder die Anzahl der Quadratmeter (qm-Zahl) der Lagerartikel automatisch für den Kundenauftrag reserviert. Die Lagerabbuchung erfolgt dann automatisch bei Lieferschein- oder Rechnungsdruck.

---

### Lagerinfo und zukünftiger Lagerbestand

Eine detaillierte Ansicht im Dialog Lagerinfo gibt Auskunft über Liefertermin, Menge, Reservierungen usw. Dabei werden die verfügbaren Lagermaße einer Größe pro Lagerort angezeigt.

*(Abb. G-48 Lagerinfo - Zukünftiger Lagerbestand)*

*   **A**: Ausgewählter Lagerartikel
*   **B**: Vorschau
*   **C**: Lagerartikel, die mit dem Hauptartikel verknüpft sind

Der zukünftige Lagerbestand wird in drei Listen dargestellt:
*   In der ersten Liste (A) ist der ausgewählte Lagerartikel aufgeführt. Wenn dies ein Lagerhauptprodukt ist, werden in der dritten Liste die verknüpften Lagerartikel aufgeführt.
*   In der zweiten Liste (B) finden Sie die Vorschau auf die nächsten Tage. Die Anzahl der Tage können Sie in den Firmendaten festlegen.
*   In der dritten Liste (C) sind die Lagermaße aufgeführt, die mit dem Hauptlagerartikel verknüpft sind.
    Dazu kann auch der kritische Lagerbestand angezeigt werden.

Mit farblichen Markierungen werden Probleme für die erfassten Aufträge angezeigt:
*   **Rot**: Termine können nicht eingehalten werden.
*   **Gelb**: Die Wiederbeschaffungszeit reicht aus.

*(Abb. G-49 Anzeige des zukünftigen Bestands)*

*   **A**: Ausgewählter Lagerartikel
*   **B**: Angezeigter Zeitraum
*   **C**: Lagerort
*   **D**: Mindestbestand aus der Lagerverwaltung
*   **E**: Errechneter Endbestand = H - G + F
*   **F**: Offene Bestellungen zum jeweiligen Datum (Liefertermin)
*   **G**: Reservierung zum Datum
*   **H**: Bestand zum Datum
*   **I**: Abmessung des Lagerartikels

Offene Bestellmengen (F) zu einem Lagerartikel werden angezeigt, bis der Wareneingang verbucht wurde. Danach wird der aktuelle Bestand der gelieferten Menge aktualisiert.

### Wiederbeschaffungszeit

Die Wiederbeschaffungszeit ergibt sich aus der Lieferzeit, die in der Lieferantenkartei für den Artikel hinterlegt ist, und aus den Tourentagen des Lieferanten, die in der Tourenverwaltung hinterlegt sind.

Wenn Sie eine Auftragsposition erfassen, können Sie den zukünftigen Lagerbestand abfragen. Wenn der Mindestbestand (D) zu einem bestimmten Termin unterschritten wird, können zwei Fälle eintreten:
*   Die Wiederbeschaffungszeit für den Artikel reicht aus, um die Ware bis zu dem Termin nachzubestellen. In der Lagervorschau werden die entsprechenden Zeilen gelb markiert.
*   Die Wiederbeschaffungszeit reicht nicht aus. In der Lagervorschau werden die entsprechenden Zeilen rot markiert.

Bei der Erfassung eines Dokuments können Sie dann den Lieferanten und/oder den Liefertermin ändern. In der Einheit Auftragserfassung von Lagerartikeln ist dies ausführlich beschrieben.
⇨ "Lagerartikel für Position suchen" auf Seite G-120

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

*   Stücklistenelemente und Produkte mit der Beschaffungsart **Lagerentnahme**, die zugeschnitten werden müssen, werden zum Datum des Produktionsstarts eingetragen.
*   Für alle anderen Lagerartikel wird als Buchungsdatum das Lieferdatum aus dem Dokument verwendet.

Wenn der Auftrag anschließend in AWCapacity Planning eingelastet wird, so werden diese voraussichtlichen Termine durch die berechneten, tatsächlichen Termine ersetzt.

---

## Bestände in der Lagersuche anzeigen

Lagerbestände werden durch die Buchungen von Warenein- und -ausgängen aktualisiert. Das Lager ist eng gekoppelt mit den Dokumenten für den Verkauf und den Einkauf. Beim Erfassen von Dokumenten kann der aktuelle Lagerbestand daher über die Lagerinfo jederzeit erfragt werden.

Der aktuelle Lagerbestand wird auch bei der Erfassung von Angeboten, Aufträgen und bei der Bestellung angezeigt. Dabei werden sowohl die Bestellungen als auch die Reservierungen berücksichtigt.

In dieser Einheit lernen Sie, wie Sie sich die Bestände und Reservierungen von Lagerartikeln anzeigen lassen.

> **Dialog Lagersuche öffnen**
> Der Dialog **Lagersuche** steht auch über das Modul **Dokumente** zur Verfügung. Damit kann schon bei der Erfassung eines Auftrags geprüft werden, ob die gewünschten Produkte in ausreichender Menge verfügbar sind.

> **Zwischensumme pro Ebene**
> Über diese Option wird in der Lagersuche eine Zwischensumme in der Tabelle angezeigt. Die Zwischensumme wird eingefügt bei Wechsel von Produktnummer, Breite, Höhe oder oberster Lagerort-Ebene. Die Option wird pro Mitarbeiter gespeichert.

### So lassen Sie die Bestände von Lagerartikeln anzeigen

1.  Wählen Sie im Menü **Lagerwirtschaft > Suche**.
    *(Abb. G-50 Filter für die Suche nach Lagerartikeln)*
    *   **A**: Produkt - Lagerartikel
    *   **B**: Filter
    ⇨Softwarereferenz, "Suche" auf Seite G-220

2.  Schränken Sie die Suche ein, indem Sie z. B. ein Produkt (A) auswählen.

3.  Wählen Sie im Bereich **Filteroptionen (B)** aus, welche Lagerartikel angezeigt werden sollen.
    Wenn Sie die Einstellung **Lagerware** deaktivieren, werden nur die Lagermaße angezeigt, die im Dialog **Produktverwaltung Lagermaße** angelegt sind, unabhängig davon, ob es sich um echte Lagerartikel handelt, das heißt, Lagerartikel aus der Lagerverwaltung.

4.  Wählen Sie im Menü **Start > Suchen**, um in die Suche zu starten.
    Die Trefferliste wird in der Übersicht angezeigt.

    *(Abb. G-51 Ergebnis der Suche)*
    In diesem Beispiel wurde nach dem Produkt Float 5 mm gesucht.

5.  Wenn Sie sich die korrespondierenden Dokumente anzeigen lassen möchten, markieren Sie eine Zeile und öffnen das Kontextmenü (rechte Maustaste).

6.  Klicken Sie auf **korrespondierende Dokumente**.

    *(Abb. G-52 Korrespondierende Dokumente)*
    In diesem Dialog werden alle Aufträge und Bestellungen angezeigt, in denen das Produkt erfasst wurde.

7.  Klicken Sie auf **[Ende]**, um den Dialog zu schließen.
    Der Dialog **Lagersuche** wird wieder angezeigt.

8.  Wenn Sie die nächsten Warenabgänge und -zugänge zu einem Produkt oder den zukünftigen Lagerbestand anschauen möchten, markieren Sie das Produkt und wechseln zum Register **Zukünftiger Lagerbestand**.

    *(Abb. G-53 Zukünftiger Lagerbestand)*
    Der zukünftige Lagerbestand wird für den Zeitraum in der Zukunft angezeigt, den Sie in den Firmendaten für die Vorschau eingetragen haben. Die Sonn- und Feiertage werden mit angezeigt, jedoch nicht mitgezählt.

---

### Übungen

*   Prüfen Sie den Bestand und die Reservierungen für Float 4 mm.
*   Notieren Sie sich die einzelnen Werte aus dem Register **Zukünftiger Lagerbestand**. In der nächsten Einheit werden Sie eine Bestellung erfassen und anschließend prüfen, wie sich die Werte geändert haben.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Suche" auf Seite G-220

---

# Lagerbestellung (automatisch)

**Lernziele**
*   Dialog Lagerbestellung kennenlernen.
*   Automatische Lagerbestellung kennenlernen.
*   Automatisch ausgelöste Bestellvorschläge an den Einkauf übergeben.
*   Änderung der angezeigten Werte im zukünftigen Lagerbestand prüfen.

**Nutzen**
*   Mit Bestellungen ergänzen Sie die Lagerbestände auf den gewünschten Sollbestand oder den Reservierungen entsprechend.
*   Wenn der Mindestbestand unterschritten wird, wird automatisch ein Bestellvorschlag erzeugt. Diesen können Sie im Dialog Lagerbestellung prüfen und dann an den Einkauf übergeben.

**Merke**
*   **Lagerbestellung manuell erfassen**: Lagerbestellungen werden im Modul **Dokumente** erfasst und bestellt. Dieser Vorgang ist im Part Einkauf beschrieben.
*   **Bestellvorschläge**: Automatische Bestellvorschläge werden ausgelöst, wenn die definierte Mindestmenge unterschritten wird. Dabei werden Reservierungen und offene Bestellungen berücksichtigt. Die Bestellvorschläge werden automatisch erzeugt und manuell an den Einkauf übergeben. Erst durch die Übergabe wird eine Bestellung erzeugt, die an den Lieferanten gesendet werden kann.

**Voreinstellungen**
*   **Stammdaten**:
    *   Produktverwaltung
    *   Lieferantenkartei
*   **Firmendaten**:
    *   Register Parameter
    *   Register Lager / EK / EDI
*   **Lagerverwaltung**:
    *   Mindestbestand
    *   Bestellmenge

---

## Bestellvorschläge

In der Regel werden Bestellungen aus der Lagerwirtschaft heraus erzeugt, um die Bestände auf dem gewünschten Niveau zu halten.

*(Abb. G-54 Lagerverwaltung – Bestandszahlen)*
*   **A**: Mindestbestand
*   **B**: Menge für Bestellvorschlag

Wenn Sie im Dialog **Lagerverwaltung** Mindestmengen (A) für einen Lagerartikel hinterlegt haben, werden Bestellvorschläge automatisch mit der hinterlegten Bestellmenge (B) erzeugt. Sie können diese vor der Übergabe an den Einkauf prüfen und ggf. den Lieferanten und den Termin ändern. Mit der Übergabe an den Einkauf wird aus dem Vorschlag eine Lagerbestellung erzeugt.

Lagerbestellungen können auch manuell über die Dokumentenverwaltung erzeugt werden. Die manuelle Lagerbestellung lernen Sie in einer separaten Einheit kennen.
⇨ "Manuelle Lagerbestellung" auf Seite G-127

---

## Lagerbestellung an den Einkauf übergeben

Automatisch erzeugte Bestellvorschläge werden im Dialog **Lagerbestellung – Bestellpool** angezeigt. Sie können den Lieferanten und den Termin ändern. Mit der Übergabe an den Einkauf erzeugen Sie die Bestellung. Diese muss dann an den Lieferanten gesendet werden.

Wenn zu einem Produkt mehrere Lieferanten hinterlegt sind, können Sie im Bestellpool die Liefertermine und Preise vergleichen und einen anderen Lieferanten auswählen.

In dieser Einheit lernen Sie, wie Sie einen Bestellvorschlag an den Einkauf übergeben.

> **Dialog Lagerbestellung**
> Der Dialog **Lagerbestellung – Bestellpool** ist nahezu identisch wie der Dialog **Bestellübergabe** aufgebaut, den Sie aus der Schulung zum Einkauf kennen. Es handelt sich jedoch um verschiedene Dialoge. Sie werden daher für jeden Bestellvorschlag genau einen Eintrag finden, zu dem es keine referenzierten Dokumente gibt.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So übergeben Sie die Bestellvorschläge an den Einkauf" auf Seite G-109
*   "So ändern Sie den Lieferanten und den Liefertermin" auf Seite G-112

### So übergeben Sie die Bestellvorschläge an den Einkauf

1.  Wählen Sie im Menü **Lagerwirtschaft > Lagerbestellung**.
    Der Dialog **Lagerbestellung** wird geöffnet.
    ⇨ Softwarereferenz, “Lagerbestellung" auf Seite G-223
    Wenn Sie die Bestellvorschläge nicht für das gesamte Lager anzeigen lassen wollen, können Sie die Anzeige auf bestimmte Lagerorte einschränken.

2.  Stellen Sie zur Einschränkung der Anzeige in den Feldern **Warenhaus, Gang, Regal und Fach** den gewünschten Lagerort ein.
    *(Abb. G-55 Lagerbestellung)*
    In diesem Beispiel wird kein Lagerort ausgewählt, damit der Bestand aller Lagerorte aufgelistet wird.

3.  Wählen Sie im Menü **Start > Suchen**, um in die Suche zu starten.
    Die Vorschläge werden eingelesen und in der Übersicht aufgelistet.
    *(Abb. G-56 Lagerbestellung – Bestellvorschläge)*

4.  Markieren Sie die Bestellvorschläge, die Sie an den Einkauf übergeben möchten.

    > **Einträge gemeinsam markieren**
    > Sie können Bestellvorschläge gemeinsam markieren, indem Sie über das Menü **Funktionen** den Dialog **Markierungsoptionen** öffnen. Wenn Sie in diesem Dialog z. B. ein bestimmtes Produkt angeben, werden alle Bestellvorschläge zu diesem Produkt mit einem Kreuz im Zeilenkopf markiert.

    *(Abb. G-57 Markierte Bestellvorschläge)*
    Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf. Nur die Vorschläge sind markiert, die mit einem X gekennzeichnet sind.

5.  Wählen Sie im Menü **Start > Ausführen**, um die Übergabe an den Einkauf zu starten.
    Bestätigen Sie die Meldung zur Anzahl der übergebenen Vorschläge.
    Die Bestellungen werden erzeugt und die übergebenen Vorschläge werden aus der Liste gelöscht.

### So ändern Sie den Lieferanten und den Liefertermin

1.  Lesen Sie im Dialog **Lagerbestellung** die Bestellvorschläge ein, wie oben beschrieben.

2.  Markieren Sie den Vorschlag, zu dem Sie den Lieferanten und/oder Liefertermin ändern wollen.
    Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf. Nur die Vorschläge sind markiert, die mit einem X gekennzeichnet sind.
    *(Abb. G-58 Vorschlag, dem ein anderer Lieferant zugeordnet werden soll)*

3.  Wählen Sie im Menü **Funktionen > Lieferant/Liefertermine ändern**.
    *(Abb. G-59 Liefertermin ändern)*

4.  Tragen Sie einen anderen Lieferanten und/oder Liefertermin ein.

5.  Klicken Sie auf **[OK]**, um die Änderung zu übernehmen.
    Der Dialog **Lieferant und Liefertermin ändern** wird geschlossen. In der Übersicht wird der Vorschlag mit dem neuen Lieferanten und/oder Liefertermin angezeigt.
    Sie können den Bestellvorschlag jetzt an den Einkauf übergeben.

---

## Preise vor der Übergabe vergleichen

Wenn zu einem Produkt mehrere Lieferanten hinterlegt sind, können Sie die Preise vor der Übergabe vergleichen und einen anderen Lieferanten auswählen. In dieser Einheit lernen Sie, wie Sie die Preise vergleichen und den günstigsten oder schnellsten Lieferanten auswählen können.

### So vergleichen Sie die Preise in einem Bestellvorschlag

1.  Wählen Sie im Menü **Lagerwirtschaft > Lagerbestellung**.
    Der Dialog **Lagerbestellung** wird geöffnet.
    ⇨ Softwarereferenz, "Lagerbestellung" auf Seite G-223

2.  Wählen Sie in den Feldern **Warenhaus, Gang, Regal und Fach** den gewünschten Lagerort ein.

3.  Wählen Sie im Menü **Start > Ausführen**, um die Bestellvorschläge einzulesen.
    Die Vorschläge werden eingelesen und in der Übersicht aufgelistet.

4.  Markieren Sie den Vorschlag, zu dem Sie die Preise der Lieferanten vergleichen wollen.
    Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf. Nur die Vorschläge sind markiert, die mit einem X gekennzeichnet sind.
    *(Abb. G-60 Position, zu der die Preise verglichen werden sollen)*

5.  Wählen Sie im Menü **Funktionen > Lieferantenpreise**.
    *(Abb. G-61 Lieferanten für markierte Position ändern)*

    *   **A**: Standard-Lieferant (Textfarbe rot)
    *   **B**: Checkbox des Standard-Lieferanten (abgewählt)
    *   **C**: Ausgewählter Lieferant für aktuelle Bestellung
    *   **D**: Checkbox zur Auswahl des Lieferanten (markiert)
    *   **E**: Textfarbe rot: Standard-Lieferant
    *   **F**: Textfarbe grün: preisgünstigster Lieferant
    *   **G**: Textfarbe blau: Standard-Lieferant ist am preisgünstigsten
    *   **H**: !!! bei allen Textfarben: Liefertermin möglicherweise zu spät für rechtzeitige Produktion und Auslieferung an Kunden

6.  Markieren Sie die Checkbox links des Lieferanten, an den die Bestellung der Position gesendet werden soll.

7.  Klicken Sie auf **[OK]**, um die Änderung zu übernehmen.
    Der Dialog **Preisvergleich** wird geschlossen. In der Übersicht wird der Vorschlag mit dem neuen Lieferanten und/oder Liefertermin angezeigt.
    Sie können den Bestellvorschlag jetzt an den Einkauf übergeben.
    ⇨ "So übergeben Sie die Bestellvorschläge an den Einkauf" auf Seite G-109

---

### Übungen

*   Richten Sie die Mindest- und die Bestellmenge eines Lagerartikels so ein, dass ein automatischer Bestellvorschlag erzeugt wird. Wählen Sie dazu den Lagerartikel aus, für den Sie in der vorigen Übung die Werte aus dem zukünftigen Lagerbestand notiert haben.
*   Prüfen Sie einen Bestellvorschlag und ändern Sie den Lieferanten oder der Liefertermin. Wenn keine alternativen Lieferanten angezeigt werden, müssen Sie die Lieferantenkartei in den Stammdaten prüfen und anpassen.
*   Übergeben Sie die Bestellvorschläge an den Einkauf.
*   Prüfen Sie im Dialog **Lagersuche**, wie sich die Werte geändert haben.

**Ergänzende Informationen im Part Verkauf**
⇨ Verkauf, "Auftragskopf" auf Seite C-39
⇨ Verkauf, "Bestellkennzeichen ändern" auf Seite C-317
⇨ Einkauf, "Lieferantenkartei anpassen" auf Seite D-33
⇨ Einkauf, "Dokument Bestellung" auf Seite D-45
⇨ Einkauf, "Wareneingang erfassen" auf Seite D-127
⇨ Einkauf, "Kistengeschäft" auf Seite D-136

---

# Lagerartikel in Dokumenten

In diesem Themenblock lernen Sie, wie Aufträge und manuelle Bestellungen auf die Lagerwirtschaft zugreifen.

Dazu gehören folgende Lerneinheiten:
*   "Auftragserfassung von Lagerartikeln" auf Seite G-118
*   "Manuelle Lagerbestellung" auf Seite G-127
*   "Produktionsaufträge" auf Seite G-131

---

## Auftragserfassung von Lagerartikeln

**Lernziele**
*   Nach Lagerartikeln für die Positionserfassung suchen.
*   Reservierung prüfen.
*   Änderungen im Lagerbestand nach Änderungen im Auftrag prüfen.

**Nutzen**
*   Bei der Erfassung von Positionen kann die Verfügbarkeit eines Produktes geprüft werden. Bei Engpässen können der Lieferant oder der Liefertermin direkt im Dokument geändert werden.

**Merke**
*   **Positionserfassung**: Lagerartikel werden in der Positionserfassung über die Lagersuche (F5) ausgewählt.
*   **Reservierung**: Ein im Auftrag erfasster Lagerartikel wird im Lager als reserviert/zugeschnitten bezeichnet.

**Voreinstellungen**
*   Produktverwaltung
*   Lieferantenkartei
*   **Firmendaten**:
    *   Register Parameter
    *   Register Lager / EK / EDI

---

### Reservierung und Buchung von Lagerartikeln

Bei der Auftragserfassung wird die Stückzahl oder die Anzahl der Quadratmeter (qm-Zahl) der Lagerartikel für den Kundenauftrag reserviert. Die Lagerabbuchung erfolgt dann automatisch bei Lieferschein- oder Rechnungsdruck. Über die verkauften und bestellten Mengen errechnet A+W Business die aktuellen Bestände.

#### Lagerbestand nach Änderung im Auftrag

Was passiert mit dem Lagerbestand, wenn Aufträge geändert werden, für die bereits ein Warenabgang gebucht wurde? In den folgenden Beispielen wird der Warenabgang beim Druck des Lieferscheins gebucht.

| Änderung im Auftrag | Folge im Auftrag | Lagerbuchung |
| :--- | :--- | :--- |
| Auftragskopf ändern, keine Änderung der Positionen | Status bleibt unverändert | Bei erneutem Erst-Druck des Lieferscheins wird kein neuer Warenabgang im Lager gebucht. |
| Position nachträglich löschen | Status ist bereits 72 und bleibt unverändert. | Abfrage, ob der Lagerbestand korrigiert werden soll. |
| Position nachträglich hinzufügen | | Abfrage, ob der Lagerbestand korrigiert werden soll. |
| Stückzahl nachträglich ändern | | Lagermenge wird automatisch ohne weiteren Hinweis korrigiert. |

In den nächsten Einheiten lernen Sie, wie Sie einen Lagerartikel in einem Dokument erfassen und die Buchung prüfen können.

---

## Lagerartikel für Position suchen

In dieser Einheit lernen Sie, wie Sie eine Position erfassen und dabei die Verfügbarkeit des gewünschten Produktes prüfen. Sie öffnen dazu den Dialog **Lagersuche**, den Sie bereits in der vorigen Einheit kennengelernt haben.

> **Lagersuche beim Erfassen einer Bestellung**
> Die Auswahl eines Lagerartikels über den Dialog **Lagersuche** können Sie auch beim Erfassen einer manuellen Lagerbestellung anwenden. Die manuelle Lagerbestellung ist in der gleichnamigen Einheit beschrieben.
> ⇨ "Manuelle Lagerbestellung" auf Seite G-127

### So erfassen Sie einen Lagerartikel als Position

1.  Wählen Sie im Menü **Dokumente > Auftrag > Auftrag** und erfassen Sie einen Auftragskopf.

2.  Wechseln Sie zur Positionserfassung und geben Sie in der Erfassungszeile die Produktnummer ein.

3.  Wählen Sie im Menü **Start > Lagersuche**, um den Dialog **Lagerinfo** zu öffnen.
    Die Auswahl im Dialog **Lagerinfo** ist bereits auf den Artikel eingeschränkt, den Sie in der Position erfasst haben. Sie müssen die Anzeige nun weiter filtern, indem Sie z. B. die Einstellungen auf Lagermaße und Bestände über null einschränken.

    *(Abb. G-62 Filter für die Suche nach Lagerartikeln)*
    *   **A**: Anzeige von Lagermaßen an- oder abschalten
    *   **B**: Nur Lagerartikel mit Bestandsmenge größer 0 anzeigen

4.  Wechseln Sie zum Register **Zukünftiger Lagerbestand**, um zu prüfen, ob die Produktionstermine gefährdet sind.
    Die Anzeige des zukünftigen Lagerbestands im Dialog Lagerinfo haben Sie bereits in der Einheit Lagerinfo kennengelernt.
    ⇨ "Anzeige des zukünftigen Bestands" auf Seite G-100

    *(Abb. G-63 Zukünftiger Lagerbestand)*
    Falls die Wiederbeschaffungszeit zu knapp ist, können Sie das Produkt dennoch erfassen und anschließend prüfen, ob ein anderer Lieferant verfügbar ist oder ob Sie den Liefertermin ändern müssen.

5.  Wechseln Sie zurück zum Register **Lagersuche** und klicken Sie doppelt auf den Lagerartikel, den Sie in die Positionserfassung übernehmen wollen.
    *(Abb. G-64 Lagerartikel auswählen)*
    Der Dialog **Lagerinfo** wird geschlossen und die Daten in der Positionserfassung werden aktualisiert.

6.  Erfassen Sie alle Positionsdaten und kehren Sie zurück zum Dokumentenkopf.
    Wenn die Wiederbeschaffungszeiten nicht ausreichen, können Sie sich die betroffenen Artikel im Dialog **Liefertermin ändern** anzeigen lassen.

7.  Klicken Sie auf die Symbolschaltfläche neben dem Versandtag, um den Dialog zu öffnen.
    *(Abb. G-65 Liefertermin im Auftrag prüfen)*
    *   **A**: Liefertermin prüfen
    *   **B**: Produkte mit zu geringem Lagerbestand
    *   **C**: Übersicht über die möglichen Lieferanten und Liefertermine zum markierten Produkt

    Alternative Lieferanten aus der Lieferantenkartei werden mit der hinterlegten Wiederbeschaffungszeit und dem entsprechenden Termin angezeigt.
    Mit einem Doppelklick auf den Artikel in der oberen Liste (B) öffnen Sie den Dialog **Lagerinfo** mit den Details zu den Artikeln.

8.  Wenn der geplante Liefertermin gefährdet ist, haben Sie folgende Möglichkeiten:
    *   Wechseln Sie den Lieferanten für die fragliche Position oder für den gesamten Auftrag.
    *   Ändern Sie den Liefertermin und benachrichtigen Sie den Kunden.
    Diese Handlungsschritte sind im Tutorial zum Verkauf ausführlich beschrieben.

9.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert. Sie können jetzt die Reservierung der Lagerartikel prüfen.

---

## Buchungen prüfen

In dieser Einheit lernen Sie, wie Sie die Buchungen der Lagerartikel prüfen können. Die Position wird nach dem Speichern reserviert. Der Warenabgang wird in der Regel mit dem Druck des Lieferscheins gebucht. Dieser Druck ist von den Einstellungen in der Statusverwaltung abhängig.
⇨ "Statusänderungen durch Zu- und Abgänge" auf Seite G-35

### So prüfen Sie die Buchungen

1.  Öffnen Sie den Dialog **Buchungsjournal**, wie in der Einheit Abfragen beschrieben.
    ⇨ "Buchungsjournal anzeigen" auf Seite G-90

2.  Schränken Sie die Auswahl auf den Auftrag ein, zu dem Sie die Reservierung prüfen wollen.
    In der Übersicht werden alle Auftragspositionen mit dem aktuellen Buchungstyp aufgelistet.

    *(Abb. G-66 Buchung - reserviert)*
    Im Buchungsjournal wird die Buchungsart **reserviert** nur so lange angezeigt, bis der Warenabgang gebucht wurde.

    Nach dem Warenabgang werden die Auftragspositionen als **ausgeliefert** gekennzeichnet.
    *(Abb. G-67 Buchung – ausgeliefert)*

    In der Auftragshistorie werden die einzelnen Statusänderungen anhand des Drucks und der Lagerbuchungen dargestellt.
    *(Abb. G-68 Auftragshistorie)*

---

### Übungen

*   Erfassen Sie einen Auftrag mit vorhandenen Lagerprodukten und prüfen Sie die Einträge im Buchungsjournal:
    *   Nach der Erfassung des Auftrags.
    *   Nach dem Druck des Lieferscheins. Welche Änderungen sehen Sie?
*   Erfassen Sie einen Auftrag und prüfen Sie dabei den Lagerbestand und die Reservierungen.
*   Erstellen Sie eine Rechnung zu dem Auftrag und prüfen Sie die Lagerreservierungen erneut.

---

## Manuelle Lagerbestellung

**Lernziele**
*   Besonderheiten der Lagerbestellung in der Dokumentenverwaltung kennenlernen.

**Nutzen**
*   Mit manuellen Lagerbestellungen ergänzen Sie Lagerbestände, z. B. für Großaufträge, zu denen die automatische Nachbestellung nicht ausreicht.

**Merke**
*   **Dokumententyp**: Das Dokument **Lagerbestellung** ist ein eigener Dokumententyp. Nur bei Bestellungen aus einer Lagerbestellung kann der Wareneingang auf das Lager gebucht werden.

**Voreinstellungen**
*   **Stammdaten**:
    *   Produktverwaltung
    *   Lieferantenkartei
*   **Firmendaten**:
    *   Register Parameter
    *   Register Lager / EK / EDI

---

## Lagerbestellung manuell erfassen

Bestellungen von Lagerartikeln können automatisch ausgelöst oder manuell erfasst werden. Die automatischen Bestellvorschläge haben Sie bereits in der Einheit zur automatischen Lagerbestellung kennengelernt.
⇨ "Lagerbestellung (automatisch)" auf Seite G-107

In dieser Einheit lernen Sie, wie Sie eine Lagerbestellung manuell erfassen. Die Erfassung von Dokumenten ist ausführlich in den Parts **Verkauf** und **Einkauf** beschrieben. Die folgende Handlungsanleitung konzentriert sich daher auf die wichtigsten Schritte.

### So erfassen Sie eine Lagerbestellung manuell

1.  Wählen Sie im Menü **Dokumente > Bestellung > Bestellung**.
    Der Dialog **Dokumentenverwaltung** wird geöffnet.
    ⇨ Verkauf, "Dokument - Kopfdaten" auf Seite C-424

2.  Erfassen Sie den Dokumentenkopf. Tragen Sie mindestens den Lieferanten und das Lieferdatum ein.
    *(Abb. G-69 Lagerbestellung)*
    *   **A**: Dokumententyp
    *   **B**: Einstellen des Dokumententyps

3.  Wählen Sie im Feld **Typ (B)** den Eintrag **Lagerbestellung**.
    Wenn Sie einen anderen Dokumententyp einstellen, wird der Wareneingang nicht automatisch in den Lagerbestand gebucht.

4.  Erfassen Sie die Position(en).

    > **Positionen ohne Lagerkennzeichen**
    > Wenn Sie Lagerbestellungen mit Positionen erfassen, die nicht als Lagerartikel geführt werden, werden diese im Wareneingang nicht angezeigt. Sie können in den Stammdaten **Firma > Firmendaten > Register Lager / EK / EDI** jedoch die entsprechende Option aktivieren.
    > ⇨ "Firmendaten - Lager / EK / EDI" auf Seite G-32

5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.

6.  Drucken und versenden Sie die Bestellung.
    Dieser Vorgang ist im Part Verkauf beschrieben.
    ⇨ Tutorial, "Auftragskopf" auf Seite C-39

---

### Übungen

*   Prüfen Sie die Lagerbestände für einen Lagerartikel.
*   Erfassen Sie eine Lagerbestellung manuell und prüfen Sie im Dialog **Lagerinfo** die entsprechenden Werte erneut.

---

## Produktionsaufträge

**Lernziele**
*   Produktionsauftrag kennenlernen.
*   Manuelle und automatische Erstellung von Produktionsaufträgen kennenlernen.

**Nutzen**
*   Produktionsaufträge werden verwendet, um den eigenen Lagerbestand aufzufüllen.
*   Produktionsaufträge können bei Unterdeckung des Mindestbestands automatisch erzeugt werden, wenn in der Lieferantenkartei die Umleitung auf einen internen Kunden aktiviert ist.

**Merke**
*   **Beschaffungsart**: Alle Artikel, die in einem Produktionsauftrag erfasst werden, haben automatisch die Beschaffungsart **Produktion**.
*   **Buchungsart**: Im Gegensatz zu normalen Aufträgen werden die erfassten Positionen nicht im Lager reserviert, sondern als **bestellt** markiert.
*   **Lagerzugang**: Der Lagerzugang aus Produktionsaufträgen kann manuell oder automatisch gebucht werden:
    *   Manuelle Statusumsetzung im Modul **Fertigung**.
    *   Automatische Status-Rückmeldungen aus der Produktion.

**Voreinstellungen**
*   **Lagerverwaltung**:
    *   Mindestbestand
    *   Bestellmenge
*   **Stammdaten**:
    *   Produktverwaltung
    *   Partnerverwaltung (interner Kunde)
    *   Lieferantenkartei (Umleitung auf internen Kunden)
*   **Firmendaten**:
    *   Register Parameter
    *   Register Lager / EK / EDI > Erfassungsstelle

---

### Lagerartikel im Produktionsauftrag

Produktionsaufträge werden verwendet, um den eigenen Lagerbestand aufzufüllen. Alle Artikel, die in einem solchen Auftrag erfasst werden, werden automatisch auf die Beschaffungsart **Produktion** umgesetzt. Im Gegensatz zu Kunden-Aufträgen werden die Positionen nicht im Lager reserviert, sondern als **bestellt** markiert.

*(Abb. G-70 Positionserfassung - Beschaffungsart Produktion)*
*(Abb. G-71 Auftragserfassung – Dokumententyp Produktionsauftrag)*

Produktionsaufträge können auf unterschiedliche Weise erfasst werden:
*   Manuelle Erfassung eines neuen Dokumentes.
*   Kopieren eines gespeicherten (Dummy-)Auftrags.
*   Automatische Erstellung durch Unterdeckung des Lagerbestands.

### Manuelle Erfassung durch Kopieren

Wenn Sie regelmäßig Produktionsaufträge erfassen, können Sie den zuvor erfassten Auftrag kopieren und sich so die Arbeit erleichtern.

*   Vor dem Kopieren müssen Sie den Dokumententyp des Ziel-Dokuments auf **Produktionsauftrag** einstellen.
*   Wenn nur bestimmte Positionen aus dem Auftrag übernommen werden sollen, können Sie diese auswählen.
*   Im neuen Dokument können Sie die Daten anpassen.

*(Abb. G-72 Produktionsauftrag durch Kopieren erstellen)*
*   **A**: Kopieren von Auftrag nach Auftrag
*   **B**: Dokumententyp des Ziel-Auftrags

Eine ausführliche Beschreibung der Funktion Dokumente kopieren finden Sie im Part Verkauf.
⇨ Verkauf, "Neuer Auftrag durch Kopieren" auf Seite C-251

### Einstellungen in der Lieferantenkartei

Wenn im Dialog **Lagerverwaltung** ein Mindestbestand und eine (Standard-) Bestellmenge für den Lagerartikel hinterlegt sind, kann das System automatische Bestellvorschläge generieren. Diese werden im Dialog **Lagerbestellung** aufgelistet.

Normalerweise werden auf diesem Weg Bestellungen vom Typ **Lagerbestellung** generiert. Wenn jedoch in der Lieferantenkartei statt eines Standard-Lieferanten ein interner Kunde hinterlegt ist, können Produktionsaufträge automatisch erzeugt werden.

*(Abb. G-73 Interner Kunde für Produktionsaufträge)*
*   **A**: Produkt, für das Produktionsaufträge erzeugt werden sollen
*   **B**: Umleitung auf internen Kunden
*   **C**: Auswahl des Kunden

In der Lieferantenkartei wird ein interner Kunde eingetragen, für den der Produktionsauftrag automatisch erfasst wird. Die Option **Interner Kunde** kann auf der Ebene der Warengruppen oder der Produkte aktiviert werden. Dabei haben die Einstellungen für Produkte Vorrang vor denen für Warengruppen.

### Bestellmenge nach Bestandsprüfung

Das Programm prüft, ob die aktuellen Lagerbestände zuzüglich der bereits bestellten Mengen und abzüglich der reservierten Mengen den Mindestbestand unterschreiten.

Wenn dies der Fall ist, wird als Vorschlag ein Vielfaches der (Standard-) Bestellmenge angezeigt.

**Manuelle und automatische Lagerbestellung (Ablauf)**
1.  Prüfung: Ist der Mindestbestand unterschritten?
2.  Wenn ja, Prüfung: Ist eine Standard-Bestellmenge vorhanden?
3.  Wenn ja, Suche in der Lieferanten-Kartei.
4.  Entscheidung:
    *   Wenn ein Standard-Lieferant gefunden wird: Es wird ein **Bestellvorschlag** für eine Lagerbestellung erstellt.
    *   Wenn ein interner Kunde gefunden wird: Es wird ein **Produktionsauftrag** in der Dokumentenverwaltung erstellt.

*(Abb. G-74 Lagerbestellung vs. Produktionsauftrag)*

### Bestellmenge

Der Multiplikator wird so berechnet, dass durch den Vorschlag der Mindestbestand überschritten wird.
*(Abb. G-75 Mengenangaben für Lagerartikel (Dialog Lagerverwaltung))*

**Beispiel**
Das ESG mit der Produktnummer 4008 wird als Lagerartikel geführt.
*   Aktueller Lagerbestand: 10 Stk.
*   Mindestbestand: 30 Stk.
*   Bestellmenge: 5 Stk.

Die Bestellmenge für das ESG 4008 wird folgendermaßen berechnet:
Differenz zwischen aktuellem Bestand und Mindestbestand: 20 Stk. In dieser Differenz ist die Bestellmenge 5 Stk. vier mal enthalten.
*   **Bestellmenge**: 4 x 5 = 20 Stk.
*   **Aktueller Bestand plus bestellte Menge**: 10 + 20 = 30 Stk.

Die errechnete Menge wird in den Bestellvorschlag übernommen. Sie kann im Dialog **Lagerbestellung** angepasst werden.

---
Wie Sie die Bestellungen bearbeiten und übergeben, haben Sie in der Einheit Lagerbestellung kennengelernt.
⇨"Lagerbestellung an den Einkauf übergeben" auf Seite G-109

Der Produktionsauftrag wird erst durch die Übergabe erzeugt und in dem Auftragsnummernverwalter angelegt, der zuletzt aktiviert war.

*(Abb. G-76 Lagerbestellung – Bestellvorschläge)*
*   **A**: Einschränkung auf Lagerort
*   **B**: Bestellvorschlag für Produktionsauftrag

*(Abb. G-77 Produktionsauftrag im Nummernverwalter für Aufträge)*
*   **A**: Automatisch erzeugter Produktionsauftrag

Der Produktionsauftrag kann nun als Dokument geöffnet werden.
*(Abb. G-78 Dokument Produktionsauftrag)*
*   **A**: Auftragskopf - Produktionsauftrag
*   **B**: Bestellte Menge

Der Produktionsauftrag kann bearbeitet und an die Produktion weitergeleitet werden.

### Lagerzugang durch Produktionsauftrag

In den Firmendaten müssen Sie ist im Register **Lager / EK / EDI** den Grenzstatus für die Erfassungsstellen einstellen, ab dem ein Auftrag als produziert gilt. Als Grenzstatus gilt der für die gewählte Erfassungsstelle hinterlegte Status.
*(Abb. G-79 Firmendaten – Lager / EK / EDI: Erfassungsstelle für Statusumsetzung)*

Den Lagerzugang aus einem Produktionsauftrag können Sie auf zwei Arten erfassen:
*   Sobald durch eine Produktionsrückmeldung der Status des Produktionsauftages über diesen Status hinaus steigt, wird der Lagerzugang automatisch verbucht.
*   Wenn Sie nicht mit Produktionsrückmeldungen arbeiten, können Sie den Zugang über die manuelle Statusmeldung im Modul **Fertigung** erfassen. Wenn Sie den Produktionsauftrag dort auf einen Status setzen, der über dem o. g. Grenzstatus liegt, werden der Lagerabgang der verbrauchten Materialien und der Lagerzugang der gefertigten Lagerartikel automatisch gebucht.

Wenn kein abweichender Lagerort definiert wurde, werden die Auftragsmengen dem Standard-Lagerort zugeordnet.
Die Verbuchung von Produktionsaufträgen wird im Part **Fertigung** ausführlich behandelt.

**Ergänzende Informationen**
⇨ Stammdaten, "Firmendaten - Lager/EK/EDI" auf Seite B-970
⇨ Verkauf, "Auftragskopf" auf Seite C-39
⇨ Verkauf, "Bestellkennzeichen ändern" auf Seite C-317
⇨ Fertigung, "Produktionsaufträge" auf Seite E-130

---

# Inventur

In diesem Themenblock lernen Sie, wie Sie die Bestandszahlen Ihres Lagers in A+W Business durch eine Inventur bereinigen.

Dazu gehören folgende Lerneinheiten:
*   "Periodische Inventur" auf Seite G-142
*   "Erstinventur" auf Seite G-159

---

## Periodische Inventur

**Lernziele**
*   Inventurablauf kennenlernen.
*   Dialoge für die Inventur kennenlernen.
*   Inventur durchführen.

**Nutzen**
*   Mit der Inventur können Sie die Bestandszahlen in A+W Business bereinigen.
*   Bei großen Lagerorten können Sie die Inventur so organisieren, dass der normale Geschäftsbetrieb möglichst wenig behindert wird.

**Merke**
*   **Keine Bestandsänderung während der Inventur**: Am Zähltag dürfen keine Aufträge, Bestellungen und Wareneingänge erfasst werden, Ware darf nicht aus dem Lager entnommen oder in es hineingestellt werden. Der Sollbestand sollte am Zähltag ermittelt werden.
*   **Verlauf der Inventur**: Die Inventur wird in folgenden Schritten durchgeführt: Inventurliste erstellen, Sollbestand ermitteln, Inventurwerte erfassen, Inventur abschließen.
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
| Verkauf | 01.01. bis 14.01. | -30 | -30 |
| Einkauf | | +10 | +10 |
| | 15.01. | Tatsächlicher Istbestand 60 | 80 |
| Inventurabschluss | | Sollbestand neu: 60 | |

Mit dem Inventurabschluss wird der Istbestand als neuer Sollbestand im System gespeichert.

#### qm-Artikel
Werden für einen qm-Artikel einzelne Blätter in bestimmten Abmessungen gezählt, so können diese als Stückartikel erfasst werden. Beim Inventurabschluss werden diese dann in qm umgewandelt und als solche in das Lager gebucht (in Ausdrucken des Inventurabschlusses stehen allerdings die gezählten Stückzahlen).

#### Inventarisieren einer Kiste
Zum Inventarisieren der Kiste, also um sie in einer Inventurliste zu erfassen, wird zunächst eine Inventurliste erstellt und dafür der Sollbestand ermittelt. Danach werden die Identnummer der Kiste, der Lagerort und ggf. eine abweichende Blattanzahl gescannt oder manuell eingegeben. Der Scanvorgang fügt diese Kiste immer der aktuellsten Inventurliste hinzu. Anschließend wird ggf. in der Inventurverwaltung noch der restliche Lagerbestand erfasst und am Ende der Inventurabschluss gebucht.

*(Beispiel für eine Zählliste, Abb. G-80)*

Die gezählten Mengen werden in der Zählliste eingetragen und später in der Inventurverwaltung erfasst.
⇨ "Inventurwerte erfassen" auf Seite G-152

---

## Inventurliste erstellen

Für die Inventur werden Listen benötigt, in denen die manuellen Zählmengen festgehalten werden. Diese Listen können nach verschiedenen Kriterien ausgeführt und gedruckt werden.

Wenn beim Druck festgestellt wird, dass bestimmte Artikel auf der Liste fehlen, kann eine Nachtragsinventur angehängt werden. Damit müssen nicht alle Listen neu gedruckt werden.

> **Keine Änderungen an den Stammdaten der Produkte**
> Sobald die Inventurliste erstellt ist, werden in der Produktverwaltung alle Produkte gekennzeichnet, die in der Inventurliste aufgeführt sind. Die Beschaffungsart und das Lagerkennzeichen in diesen Produkten sind dann gesperrt. Wenn die Inventur abgeschlossen ist, wird die Kennzeichnung gelöscht und die Daten können wieder bearbeitet werden.

In dieser Einheit lernen Sie, wie Sie Inventurlisten erstellen und wieder öffnen.
Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So beginnen Sie eine Inventur" auf Seite G-146
*   "So drucken Sie die Zähllisten" auf Seite G-148
*   "So laden Sie eine gespeicherte Inventurliste" auf Seite G-149
*   "So ergänzen Sie eine Inventurliste vor dem Zählen" auf Seite G-149

### So beginnen Sie eine Inventur

1.  Wählen Sie im Menü **Lagerwirtschaft > Inventur > Inventurliste**.
    Der Dialog **Inventurliste** wird geöffnet.
    ⇨ Softwarereferenz, "Inventurliste" auf Seite G-169

2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    *(Abb. G-81 Felder für neue Inventurliste freigeschaltet)*
    *   **A**: Alle Artikel oder Folge von Artikelnummern
    *   **B**: Datum der Inventur
    *   **C**: Eingrenzungen
    *   **D**: Lagerbewertung
    *   **E**: Sortierung der Liste

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

### So drucken Sie die Zähllisten

Wenn in der Zählliste der Sollbestand gedruckt werden soll, müssen Sie vor dem Druck den Sollbestand ermitteln.
⇨ "So ermitteln Sie den Sollbestand zu einer Inventurliste" auf Seite G-151

1.  Wählen Sie im Menü **Lagerwirtschaft > Inventur** und wählen Sie das Datum der Inventurliste aus.
2.  Wählen Sie im Menü **Start > Suchen**, um die Inventurliste zu laden.
    Diese Schritte entfallen, wenn Sie die Zählliste sofort nach dem Erstellen der Inventurliste drucken.
3.  Wählen Sie im Menü **Druck > Drucker**.
    Wenn Sie das Ergebnis zunächst am Bildschirm prüfen möchten, wählen Sie **Bildschirm**. Sie können dann den Druck starten, wenn Sie mit dem Ergebnis zufrieden sind. Die folgenden Schritte sind für beide Einstellungen gleich.
    *(Abb. G-82 Inventur - Zählliste drucken)*
    *   **A**: Seitenumbruch
    *   **B**: Artikel, die gedruckt werden sollen
    *   **C**: Sortierung

4.  Bestimmen Sie, an welcher Stelle eine neue Seite (A) gedruckt werden soll.
    Wenn Sie keine unterschiedlichen Lagerorte angelegt haben, entfällt diese Einstellung. Wenn Sie die Zählbereiche nach Lagerorten verteilt haben, machen Sie den Seitenumbruch nach den entsprechenden Lagerorten. Für den Druck müssen Sie mindestens **Lagerhaus (Ebene 1)** markieren.

5.  Legen Sie fest, welche Lagerware (B) in der Liste gedruckt werden soll.
    Wenn an den angegebenen Lagerorten unterschiedliche Lagerartikel vorkommen, können Sie nach **Fertigprodukten** oder **Rohmaterial** unterscheiden. Fertigprodukte sind alle Lagerartikel, die nicht im Lager für Rohmaterial gelagert sind.
    Die Zuordnung der Eigenschaften Fertigprodukte und Rohmaterial haben Sie in der Lagerdefinition getroffen.
    ⇨ "Lagerort definieren" auf Seite G-24

6.  Wählen Sie die Sortierung (C) der Artikel auf der Zählliste so, dass sie sich nach den ausgewählten Kriterien richten. Die Option **Artikel** ist z. B. dann sinnvoll, wenn Sie das Lager nach Produkten aufgebaut haben.

7.  Klicken Sie auf **[OK]**, um den Druck zu starten.
    Die Liste wird gedruckt und kann nun zur Zählung verwendet werden.

### So laden Sie eine gespeicherte Inventurliste

1.  Wählen Sie im Menü **Lagerwirtschaft > Inventur**.
2.  Wählen Sie im Feld **Inventurdatum** das Datum aus, unter dem die Inventurliste gespeichert wurde.
3.  Wählen Sie im Menü **Start > Suchen**, um die Inventurliste zu laden.
    Die Inventurliste wird angezeigt.

### So ergänzen Sie eine Inventurliste vor dem Zählen

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

---

## Sollbestand ermitteln

Der Sollbestand muss für jede Inventurliste durchgeführt werden. Er gibt die Mengen an, die sich laut System im Lager befinden müssen. Wenn der Sollbestand mit in den Zähllisten gedruckt werden soll, muss er vor dem Druck der Liste ermittelt werden.

> **Keine Lagerbuchungen am Zähltag**
> Nachdem der Sollbestand ermittelt wurde, müssen die Bestände gezählt werden. Am Tag der Zählung dürfen keine Lagerartikel entnommen und keine Lagerbewegungen gebucht werden, bis die Zählung abgeschlossen ist. Dies betrifft alle manuellen oder automatischen Lagerab-/zugänge und alle Wareneingänge für Lagerbestellungen. A+W Business wird nicht automatisch für Buchungen gesperrt.

In dieser Einheit lernen Sie, wie Sie den Sollbestand für eine gespeicherte Inventurliste ermitteln.

### So ermitteln Sie den Sollbestand zu einer Inventurliste

1.  Wählen Sie im Menü **Lagerwirtschaft > Inventur > Sollbestand**.
    Der Dialog **Sollbestand** wird geöffnet.
    ⇨ Softwarereferenz, "Sollbestand" auf Seite G-176

2.  Laden Sie die Inventurliste, zu der der Sollbestand ermittelt werden soll.
    *(Abb. G-83 Sollbestand ermitteln)*

3.  Wählen Sie im Menü **Start > Ausführen**, um den Sollbestand zu ermitteln und bestätigen Sie die Abfrage mit **[Ja]**.
    Der Sollbestand wird in der Spalte **Soll** eingetragen. Sie können den Sollbestand nur einmal pro Inventurliste ermitteln. Wenn Sie die Funktion mehrfach ausführen, wird das Ergebnis nicht aktualisiert.

Wenn der Sollbestand mit in die Zählliste gedruckt werden soll, können Sie jetzt den Druck starten.

Sie können jetzt die Zählung beginnen und anschließend die gezählten Mengen erfassen.

---

## Inventurwerte erfassen

Wenn die Zählmengen in die gedruckten Zähllisten eingetragen sind, können Sie die Werte im Dialog **Inventurverwaltung** eingeben.

> **Keine Lagerbuchungen am Zähltag**
> Nachdem der Sollbestand ermittelt wurde, müssen die Bestände gezählt werden. Am Tag der Zählung dürfen keine Lagerartikel entnommen und keine Lagerbewegungen gebucht werden, bis die Zählung abgeschlossen ist. Dies betrifft alle manuellen oder automatischen Lagerab-/zugänge und alle Wareneingänge für Lagerbestellungen. A+W Business wird nicht automatisch für Buchungen gesperrt.

In dieser Einheit lernen Sie, wie Sie die gezählten Mengen in A+W Business erfassen und ggf. einen neuen Lagerartikel anlegen.
Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So erfassen Sie die gezählten Mengen" auf Seite G-152
*   "So erfassen Sie einen neuen Lagerartikel während der Inventur" auf Seite G-154

### So erfassen Sie die gezählten Mengen

1.  Wählen Sie im Menü **Lagerwirtschaft > Inventur > Verwaltung**.
    Der Dialog **Verwaltung** wird geöffnet.
    ⇨ Softwarereferenz, “Verwaltung" auf Seite G-179

2.  Laden Sie die Inventurliste.
    In der Tabelle werden die Belege in derselben Reihenfolge angezeigt, wie in der gedruckten Liste.
    Über das Menü **Sortierung** kann eine andere Reihenfolge ausgewählt werden, wenn dadurch die Erfassung der gezählten Werte einfacher wird.

    *(Abb. G-84 Inventur - Zählmengen erfassen)*
    *   **A**: Gezählte Menge eingeben
    *   **B**: Liste der Belege

3.  Tragen Sie die Menge (A) der ersten Position im Feld **Menge** ein und bestätigen Sie mit `<Enter>`.
    Die Markierung wechselt danach automatisch in die nächste Zeile, so dass Sie sofort die nächste Menge eintragen können.

4.  Markieren Sie ggf. eine Zeile, wenn Sie die Mengen in einer anderen Reihenfolge erfassen möchten.

    > **Menge und Lagerort für mehrere Artikel**
    > Sie können mehrere Belege markieren und für alle gemeinsam über das Menü **Funktionen** die Menge auf null setzen oder den Lagerort ändern.

5.  Ändern Sie ggf. den Lagerort, den Inventurpreis und die Kategorie, die für die Bewertung des Lagers herangezogen werden.
    Geänderte Inventurpreise werden nach dem Abschluss der Inventur nicht in die EK-Preistabelle zurückgeschrieben und fließen nicht in die Berechnung des Durchschnitts-EKs ein.

6.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert. Wenn Sie die Daten noch nicht vollständig erfasst haben, können Sie die Eingabe zu einem späteren Zeitpunkt fortsetzen. Beginnen Sie dann mit Schritt 1.
    Wenn Sie alle Mengen erfasst haben, können Sie die Inventur abschließen.

### So erfassen Sie einen neuen Lagerartikel während der Inventur

1.  Wählen Sie im Menü **Lagerwirtschaft > Inventur > Verwaltung** und wählen Sie die aktuelle Inventur aus.
2.  Markieren Sie den Beleg, zu dem Sie einen neuen Lagerartikel anlegen möchten.
3.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    Alle Daten des ursprünglichen Lagerartikels werden damit kopiert, so dass Sie im neuen Lagerartikel nur die abweichenden Daten bearbeiten müssen.
4.  Tragen Sie die Breite, Höhe, den Lagerort usw. ein.
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Liste wird um den neuen Lagerartikel erweitert.

---

## Inventur abschließen

Die Inventur wird abgeschlossen, indem die Zählergebnisse verbucht und die Bestände im Lager aktualisiert werden.

Der Inventurabschluss kann nur einmal pro Inventurliste durchgeführt werden. Wenn Sie nach dem Abschluss Fehler in den gezählten oder erfassten Werten feststellen, müssen Sie die Mengen im Dialog **Lagerverwaltung** korrigieren oder für den entsprechenden Artikel eine neue Inventurliste erstellen und abschließen.

In dieser Einheit lernen Sie, wie Sie die Inventur zu einer Inventurliste abschließen.
Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So schließen Sie die Inventur ab" auf Seite G-155
*   "So löschen Sie eine Inventurliste nach dem Inventurabschluss" auf Seite G-156

### So schließen Sie die Inventur ab

1.  Wählen Sie im Menü **Lagerwirtschaft > Inventur > Abschluss**.
    Der Dialog **Abschluss** wird geöffnet.
    ⇨ Softwarereferenz, "Abschluss" auf Seite G-184

2.  Laden Sie die Inventur, die Sie abschließen möchten.
    *(Abb. G-85 Inventur - Abschluss)*
    In der Übersicht wird die Inventurliste mit den eingegebenen Mengen angezeigt.

3.  Prüfen Sie im Menü **Optionen**, ob der Bestand ohne oder mit Abfrage auf Null gesetzt werden soll, wenn keine Mengen erfasst sind.

4.  Wählen Sie ggf. den AV-Bereich aus, auf den die Inventur eingeschränkt wurde.

5.  Wählen Sie im Menü **Start > Ausführen** und bestätigen Sie die Abfrage mit **[Ja]**, um die Inventur abzuschließen.
    Die Daten werden gespeichert und die Bestandswerte und Preise für die Lagerbewertung werden aktualisiert. Die verbuchten Belege werden aus der Liste gelöscht. Die Sperrungen in den Produktstammdaten werden aufgehoben.

    Belege, die nicht verbucht werden konnten, bleiben in der Liste enthalten. Sie können die fehlenden Werte im Dialog **Verwaltung** ergänzen.
    Wenn alle Belege verbucht werden konnten, wird die gesamte Inventurliste aus dem Inventurabschluss gelöscht.

    > **Fehler bei der Inventur**
    > Wenn bei der Inventur Fehler aufgetreten sind und einzelne Belege nicht aus der Inventurliste gelöscht werden, können Sie im Logbuch nach der Ursache forschen. Öffnen Sie das Logbuch über **System > Logbuch**.

### So löschen Sie eine Inventurliste nach dem Inventurabschluss

> **Keine einzelnen Belege löschen**
> Sie können nach dem Inventurabschluss keine einzelnen Belege aus der Liste löschen.

1.  Wählen Sie im Menü **Lagerwirtschaft > Inventur > Inventurliste**.
2.  Laden Sie die Inventurliste, die Sie abgeschlossen haben.
3.  Wählen Sie im Menü **Start > Löschen** und bestätigen Sie die Abfrage mit **[Ja]**.
    Die Inventurliste wird gelöscht. Wenn Sie weitere Inventurlisten erzeugt haben, wird die nächste Liste geladen.

---

## Nachtragsinventur anhängen

Sie können zwei getrennte Inventuren für den Druck im Inventurabschluss zusammenfassen. Dazu müssen beide Inventuren abgeschlossen (also verbucht) sein.

Wie Sie eine Inventurliste um weitere Lagerartikel ergänzen, ist im Kapitel **Inventurliste erstellen** beschrieben.
⇨ "So ergänzen Sie eine Inventurliste vor dem Zählen" auf Seite G-149

In dieser Einheit lernen Sie, wie Sie eine Nachtragsinventur an eine Hauptinventur anhängen.

### So hängen Sie eine Nachtragsinventur an

1.  Wählen Sie im Menü **Lagerwirtschaft > Inventur > Abschluss**.
    Der Dialog **Abschluss** wird geöffnet.

2.  Wählen Sie in Feld **Inventurdatum** die Hauptinventur aus.

3.  Wählen Sie im Menü **Funktionen > Nachtragsinventur anhängen**.
    *(Abb. G-86 Nachtragsinventur auswählen)*

4.  Wählen Sie das Datum der Nachtragsinventur aus und übernehmen Sie diese mit **[OK]**.
    Die Liste der Hauptinventur wird um die Positionen der Nachtragsinventur erweitert. Die Liste der Nachtragsinventur wird aus dem Dialog **Inventurliste** gelöscht.

---

### Übungen

*   Erstellen Sie eine Inventurliste für eine Folge von 5 Artikeln.
*   Ergänzen Sie die Inventurliste um zwei Artikel.
*   Ermitteln Sie den Sollbestand für die gesamte Inventurliste.
*   Tragen Sie die Zählwerte ein.
*   Schließen Sie die Inventur ab.
*   Erstellen Sie eine weitere Inventurliste mit drei Artikeln. Hängen Sie diese als Nachtragsinventur an die erste Inventur an.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Inventurliste" auf Seite G-169
⇨ Softwarereferenz, "Listendruck" auf Seite G-174
⇨ Softwarereferenz, "Sollbestand" auf Seite G-176
⇨ Softwarereferenz, "Verwaltung" auf Seite G-179
⇨ Softwarereferenz, "Abschluss" auf Seite G-184

---

## Erstinventur

**Lernziele**
*   Funktion der Erstinventur kennenlernen.

**Nutzen**
*   Mit der Erstinventur können Sie Ihr Lager mit den Lagerartikeln und den aktuellen Beständen in Betrieb nehmen.

**Merke**
*   **Erstinventur mit Unterstützung**: Bevor Sie mit der Erstinventur beginnen, sollten Sie sich mit der A+W Software GmbH in Verbindung setzen. Ihre Ansprechpartner werden Sie dann bei der Durchführung unterstützen.
*   **Keine Auftragsbearbeitung**: Da während der Erstinventur keine Aufträge bearbeitet werden dürfen, sollten Sie die Erstinventur außerhalb des normalen Tagesgeschäfts durchführen, z. B. an einem Wochenende.
*   **Voraussetzung**: Sie müssen den Ablauf der periodischen Inventur kennen, bevor Sie eine Erstinventur beginnen. Lesen Sie daher die Lerneinheit **Periodische Inventur** aufmerksam durch.
*   **Voreinstellungen**: Keine

### Ablauf für die Erstinventur

*   **Lagerinitialisierung**: Das Lager wird gelöscht (Modul **Utilities**).
    Ab jetzt dürfen keine neuen Aufträge erfasst und die alten nicht bearbeitet werden.
*   Inventurliste erstellen.
*   Sollbestand ermitteln.
*   **Lagerverwaltung**: Alle Bestände auf 0 setzen und den Standard-Lagerort für alle Lagerartikel festlegen.
*   Inventur abschließen.
*   **Lagerinitialisierung** (Modul **Utilities**).
    Bis jetzt haben Sie alle echten Lagerartikel erfasst und deren Bestand auf 0 gesetzt. Alle alten (falschen) Werte, z. B. Testprodukte und Bestandszahlen zum Testen von Funktionen, sind gelöscht.
    Die Werte für Bestellungen und Reservierungen werden geprüft und ggf. berichtigt.
*   **Vollständige Inventur durchführen**:
    *   Neue Inventurliste erstellen.
    *   Zählliste drucken.
    *   Sollbestand ermitteln.
    *   Mengen der Lagerartikel zählen.
    *   Während der Zählphase keine Ab- und Zugänge im Lager buchen.
    *   Gezählte Werte erfassen.
    *   Inventur abschließen.
*   **Lagerinitialisierung** (Modul **Utilities**).
    Die Werte für Bestellungen und Reservierungen werden erneut geprüft und auf die Lagerartikel umgesetzt.

> **Keine Änderungen an den Stammdaten der Produkte**
> Sobald die Inventurliste erstellt ist, werden in der Produktverwaltung (Stammdaten) alle Produkte gekennzeichnet, die in der Inventurliste aufgeführt sind. Die Beschaffungsart und das Lagerkennzeichen in diesen Produkten sind dann gesperrt. Sobald die Inventur abgeschlossen ist, wird die Kennzeichnung gelöscht und die Daten können wieder bearbeitet werden.

---

## Erstinventur durchführen

Die Erstinventur wird durchgeführt, bevor Sie zum ersten Mal mit der A+W Business-Lagerwirtschaft arbeiten. Sie dient dazu, das Lager mit den Lagerartikeln und deren Anfangsbeständen in Betrieb zu nehmen.

> **Ablauf der normalen Inventur sollte bekannt sein**
> Bevor Sie mit den nachfolgend beschriebenen Handlungsabläufen beginnen, sollten Sie sich die Beschreibungen der normalen Inventur durchlesen. Die Beschreibung der Erstinventur setzt diese Kenntnis voraus.

### So führen Sie eine Erstinventur durch

> **Vor der Erstinventur Kontakt mit dem Service aufnehmen**
> Bevor Sie mit der Erstinventur beginnen, sollten Sie sich mit der A+W Software GmbH in Verbindung setzen. Ihre Ansprechpartner werden Sie dann bei der Durchführung unterstützen.

1.  Starten Sie das Modul **Utilities**.
2.  Wählen Sie im Menü **System > Lagerinitialisierung**.
    *(Abb. G-87 Utilities – Lagerinitialisierung)*

3.  Wählen Sie im Menü **Funktionen > Lager löschen**.
    Ab jetzt dürfen keine neuen Aufträge erfasst und keine alten Aufträge bearbeitet werden, bis Sie die Lagerinitialisierung erneut durchgeführt haben.
    Wenn doch im Dialog **Dokumentenverwaltung** gearbeitet wird, wird der Lagerort **k.A.** in der Lagerverwaltung wieder angelegt und allen Lagerartikeln zugeordnet.

4.  Führen Sie jetzt die Inventur in folgenden Schritten durch:
    *   **Inventurliste erstellen**.
        Wählen Sie im Dialog **Inventurliste** folgende Kriterien:
        *   Nur für Lagerartikel: Mit der Einstellung alle Artikel würden z. B. auch die Bestellartikel in die Liste aufgenommen.
        *   Alle Lagerorte.
    *   **Sollbestand ermitteln**.
    *   **Inventurwerte erfassen**.
        Setzen Sie im Dialog **Lagerwirtschaft > Verwaltung** die Mengen aller gezählten Artikel auf 0.
        Dieser Vorgang ist in der Handlungsanleitung zum Erfassen der gezählten Mengen in der Anmerkung zu Schritt 4 und in Schritt 5 beschrieben.
    *   **Inventur abschließen**.

5.  Wechseln Sie wieder zum Dialog **Lagerinitialisierung**.
6.  Wählen Sie im Menü **Start > Ausführen**, um die Aktion zu starten.
7.  Führen Sie mit einer neuen Inventurliste eine vollständige Inventur durch:
    *   "So beginnen Sie eine Inventur" auf Seite G-146
    *   "So drucken Sie die Zähllisten" auf Seite G-148
    *   "So ermitteln Sie den Sollbestand zu einer Inventurliste" auf Seite G-151
    Achten Sie darauf, dass während der Zählphase keine Ab- oder Zugänge im Lager gebucht werden. Dies betrifft auch das Erfassen von Wareneingängen.

8.  Tragen Sie die gezählten Mengen und die korrekten Lagerorte ein und schließen Sie die Inventur ab:
    *   "So erfassen Sie die gezählten Mengen" auf Seite G-152
    *   "So schließen Sie die Inventur ab" auf Seite G-155

9.  Öffnen Sie den Dialog **Lagerinitialisierung**, wie in Schritt 1 und 2 beschrieben.
10. Wählen Sie im Menü **Start > Ausführen**, um die Aktion zu starten.
    Ab jetzt stimmen die Bestände im Lager und die Lagerorte.

---

## Übungen

Beantworten Sie die folgenden Fragen, indem Sie die entsprechenden Einstellungen erklären.

*   Wann berücksichtigt das Lager Rückmeldungen aus der Produktion, z. B. von A+W Production?
*   Wo hinterlegt man, ob die Ausbuchung von reservierten Lagerprodukten nach Lieferscheindruck oder nach Rechnungsdruck erfolgt?
*   Was müssen Sie tun, um Lagerprodukte, die als Stücklisten-Komponenten in einer Position stehen, im Lager automatisch zu verbuchen?
*   Was ist der Unterschied zwischen der Definition von Lagermaßen im Dialog **Stammdaten > Produkte > Artikel > Lagermaße** und im Dialog **Lagerwirtschaft > Lagerverwaltung**?
*   Was wird in den ersten beiden Registern im Dialog **Lagerwirtschaft > Lagerverwaltung** angezeigt. Beschreiben Sie die Unterschiede!
*   Was ist der Unterschied zwischen dem Buchungsjournal und der Lagerhistorie?
*   Wozu dient der Dialog **Lagerwirtschaft > Lagerbestellung**?
*   Was ist der Unterschied zwischen einer manuellen und einer automatischen Lagerbestellung?

---
---

# Softwarereferenz

## Übersicht

Im Modul **Lagerwirtschaft** werden alle Daten zum Lager gepflegt und ausgewertet. Außerdem führen Sie in diesem Modul die Inventur durch und buchen Lagerbewegungen.

In der Softwarereferenz finden Sie Informationen zu folgenden Themen:
*   "Inventur" auf Seite G-168
*   "Lagerverwaltung" auf Seite G-187
*   "Lagerbewegung" auf Seite G-198
*   "Abfragen" auf Seite G-205
*   "Suche" auf Seite G-220
*   "Lagerbestellung" auf Seite G-223
*   "Lagerbewertung" auf Seite G-229

---

## Inventur
**Lagerwirtschaft > Inventur**

Über die Dialoge aus dem Menü **Inventur** führen Sie die Inventur in einzelnen Schritten durch: Sie erstellen eine Inventurliste, ermitteln den Sollbestand, erfassen die gezählten Mengen und schließen die Inventur ab.

Im Menü **Inventur** finden Sie sich folgende Programmpunkte:
*   Inventurliste
*   Sollbestand
*   Inventurverwaltung
*   Inventurabschluss

> **Ergänzende Informationen**
> ⇨ Tutorial, "Periodische Inventur" auf Seite G-142
> ⇨ Tutorial, "Erstinventur" auf Seite G-159

---

### Inventurliste
**Lagerwirtschaft > Inventur > Inventurliste**

**Zu Dialogbeschreibung:**
*   Listendruck

**Menü Funktionen**
Mit der Funktion **Lager bereinigen** wird die alte Inventurliste gelöscht. Gleichzeitig werden alle Produkte aus den Lager-Stammdaten gelöscht, die kein Lagerkennzeichen haben oder die unsinnig sind, z. B. ein Produkt, das keine Referenz auf einen Lagerort hat.

> **Der Vorgang kann erhebliche Zeit in Anspruch nehmen**
> Je nach Größe der Datenbank und Rechnerleistung kann die Bereinigung des Lagers über einen längeren Zeitraum laufen. Dies können auch mehrere Stunden sein. In dieser Zeit kann mit A+W Business nicht gearbeitet werden.

*(Abb. G-88 Inventurliste)*

Die Inventurliste bildet die Basis für den Inventurvorgang. Dazu wählen Sie die Kriterien aus, nach denen die Liste erstellt werden soll. Da während des Zählvorgangs keine Lagerveränderungen ausgeführt werden dürfen, ist es bei großen Lagern sinnvoll, die Inventur in kleineren Einheiten durchzuführen, z. B. nach Lagerorten.
⇨ Tutorial, "Inventurliste erstellen" auf Seite G-145

---

> **Keine Änderungen an den Stammdaten der Produkte**
> Sobald die Inventurliste erstellt ist, werden in der Produktverwaltung (Stammdaten) alle Produkte gekennzeichnet, die in der Inventurliste aufgeführt sind. Die Beschaffungsart und das Lagerkennzeichen in diesen Produkten sind dann gesperrt. Sobald die Inventur abgeschlossen ist, wird die Kennzeichnung gelöscht und die Daten können wieder bearbeitet werden.

> **Inventurliste löschen**
> Wenn eine Inventur vollständig durchgeführt und abgeschlossen ist, sollten Sie die zugehörige Inventurliste löschen. Sie können jedoch auch jede beliebige Inventurliste zu jedem Zeitpunkt wieder löschen. Das Kennzeichen "Artikel steht auf der Inventurliste im Auftrag" und die Sperrung der Produktstammdaten werden dann aufgehoben.

#### Parameter
Die Felder in diesem Bereich sind nur freigeschaltet, wenn Sie eine neue Inventurliste erstellen. Im Auswahlmodus können Sie eine Inventurliste über das Datum anzeigen lassen.

**Inventurdatum**
Die Inventurliste wird zu einem bestimmten Datum erstellt. Alle weiteren Inventurvorgänge beziehen sich immer auf das Inventurdatum. Das aktuelle Tagesdatum wird automatisch angezeigt. Es kann mit dem gewünschten Datum überschrieben werden, z. B., wenn Sie die Vorbereitungen zu einer Inventur treffen, die zu einem späteren Zeitpunkt durchgeführt werden soll.

**Alle Artikel**
Sie können die Inventur für alle Artikel durchführen, die als Produkte in den Stammdaten erfasst sind.

**Artikelnummer von ... bis**
Sie können die Inventurliste für einen bestimmten Bereich von Artikelnummern erstellen, indem Sie die entsprechenden Nummern eingeben. Diese Felder sind gesperrt, wenn die Checkbox **Alle Artikel** markiert ist.

#### Lagerbewertung
Mit der Wahl einer Option legen Sie fest, wie der Lagerwert zur Inventur ermittelt werden soll. Der entsprechende Wert wird in der Spalte **EK/PE** in der Inventurliste angezeigt. Der Wert kann auf der Zählliste gedruckt werden.
*   **EK-Preisliste**: Die Einzelpreise der Produkte aus der EK-Tarifzuordnung werden zur Lagerbewertung herangezogen.
*   **Niedrigster EK**: Für alle Artikel wird jeweils der niedrigste Wert zur Lagerbewertung herangezogen.
*   **Geschnittener EK**: Für alle Artikel wird jeweils der Durchschnitts-EK zur Lagerbewertung herangezogen. Dazu muss in den Firmendaten die Option **Durchschnitts-EK** aktiviert sein.
    ⇨ Stammdaten, "Durchschnitts EK: Der Durchschnittspreis für den Einkauf wird in folgenden Fällen neu berechnet:" auf Seite B-970

**Nur Produkte mit Lagerbestand > 0**
Sie können die Inventur auf die Lagerartikel mit Bestand einschränken.
*   ☐ Der komplette Produktstamm inklusive Lagermaßtabelle wird in die Inventurliste aufgenommen, sofern die Auswahl nicht durch andere Kriterien eingeschränkt wird.
*   ☑ Nur die Lagerartikel werden in die Inventurliste übernommen, zu denen ein Bestand vorhanden ist.
Die Checkboxen **Nur Produkte mit Lagerführung in dem Produkt** und **Keine Kisten mit Identnummer und Bestand = 0** werden markiert und gesperrt.

**Nur Produkte mit zugeordnetem Lagerprodukt**
Sie können die Inventur auf Lagerartikel einschränken.
*   ☐ Der komplette Produktstamm inklusive Lagermaßtabelle wird in die Inventurliste aufgenommen, sofern die Auswahl nicht durch andere Kriterien eingeschränkt wird.
*   ☑ Nur die Lagerartikel werden in die Inventurliste übernommen, die in der Lagerverwaltung angelegt sind.

**Nur Produkte mit Lagerführung in dem Produkt**
Sie können die Inventur auf die Produkte mit einem Lagerkennzeichen einschränken.
*   ☐ Der komplette Produktstamm inklusive Lagermaßtabelle wird in die Inventurliste aufgenommen, sofern die Auswahl nicht durch andere Kriterien eingeschränkt wird.
*   ☑ Nur Artikel mit der Beschaffungsart **Lagerentnahme** werden in die Inventurliste aufgenommen.
Die Checkbox ist markiert und gesperrt, wenn die Checkbox **Nur Produkte mit Lagerbestand > 0** markiert ist.

**Keine Kisten mit Identnummer und Bestand = 0**
Im Lagerbestand können sich Kisten befinden, die bereits ausgeliefert sind, aber nicht gelöscht wurden. Deren Bestand wird korrekt mit 0 angezeigt.
*   ☐ Alle Kisten werden in der Inventurliste aufgeführt.
*   ☑ Kisten mit einer ID und einem Bestand = 0 werden nicht in der Inventurliste aufgeführt.
Die Checkbox ist markiert und gesperrt, wenn die Checkbox **Nur Produkte mit Lagerbestand > 0** markiert ist.

**Nur für bestimmten Lagerort**
Sie können die Inventur auf einen Lagerort einschränken.
*   ☐ Die Inventur wird für alle Lagerorte durchgeführt. Sie wird nicht auf einen Lagerort eingeschränkt.
*   ☑ Die Inventur wird für einen Lagerort durchgeführt. Zur Bestimmung des Lagerorts werden die Komboboxen **Warenlager, Gang, Regal und Fach** (Ebene 1 bis 4) freigeschaltet. Diese Einstellung ist nur dann sinnvoll, wenn die Bestände Ihrer Lagerorte in unterschiedlichen Zeiträumen überprüft werden.

> **Lagerort <k.A.>**
> Auch wenn Sie eigene Lagerorte hinterlegt haben, bleiben die Lagerorte `<k.A.>` erhalten und können bebucht werden.

**Keine Produkte aus Produkt-Lagermaßen**
Sie können die Inventur ohne die Übernahme der Produkt-Lagermaße erstellen.
*   ☐ Die Inventur wird für alle Produkte erstellt.
*   ☑ Die Inventur wird ohne die automatische Übernahme der Produkt-Lagermaße erstellt.

**Warenhaus, Regal, Gang, Fach**
Sie können die Inventurliste auf einen Lagerort einschränken. Die Felder sind nur freigeschaltet, wenn die Checkbox **Nur für bestimmten Lagerort** markiert ist.

#### Sortierung
Mit der Wahl der Option legen Sie die Sortierung der Inventurliste fest. Standardmäßig ist die Option **Artikel** aktiviert.

#### Übersicht
In der Übersicht sind alle Artikel aufgelistet, die in der Inventur gezählt und bewertet werden sollen.
*   **Beleg Nr.**: Laufende Nummer in der Inventurliste.
*   **Art. Nr.**: Produktnummer aus den Stammdaten.
*   **Bezeichnung**: Produktbezeichnung aus den Stammdaten.
*   **Farbe**: Die Farbe wird nur angegeben, wenn das Produkt mit Varianten/Farben angelegt ist.
*   **Breite, Höhe**: Die Maße werden nur angezeigt, wenn das Produkt als Lagermaß oder Kiste mit festen Größen angelegt ist. Bei allen nicht maßabhängigen Produkten wird der Wert 0 angezeigt.
*   **EK/PE**: Einkaufspreis (EK) pro Preiseinheit. Je nach Einstellung ist das der niedrigste oder der Durchschnitts-EK.
*   **PE**: Preiseinheit für den EK.
*   **EK / Blatt**: Der EK-Preis pro Blatt wird nur bei Lagermaßen angezeigt. Er wird errechnet aus dem EK/PE und der tatsächlichen Größe der Platte. Wenn ein Stückpreis hinterlegt ist, sind die Werte in den Spalten **EK/PE** und **EK/Blatt** identisch.
*   **Soll**: Der Sollbestand gibt an, welche Menge in A+W Business den durchgeführten Buchungen gemäß gespeichert ist. Er wird erst angezeigt, wenn der Sollbestand ermittelt wurde.
    ⇨ "Sollbestand" auf Seite G-176
*   **ME**: Mengeneinheit, mit der das Produkt im Lager geführt wird.

---

### Listendruck
**Lagerwirtschaft > Inventur > Inventurliste > Menü Druck**

*(Abb. G-89 Druck - Inventurliste)*

In diesem Dialog können Sie einstellen, wie die Zähllisten gedruckt werden sollen. Damit können Sie die Blätter für die manuelle Erfassung der Bestände Ihrem Lager und den Inventur-Aufgaben Ihrer Mitarbeiter entsprechend gestalten.
⇨ Tutorial, "So drucken Sie die Zähllisten" auf Seite G-148

> **Sollbestand in der Zählliste**
> Der Sollbestand kann nur in der Zählliste gedruckt werden, wenn er vor dem Druck ermittelt wurde.
> ⇨ "Sollbestand" auf Seite G-176

**Seitenumbruch nach Wechsel von**
*   **Lagerhaus, Lagergang, Lagerregal, Lagerfach**: Wenn Sie die Zählliste nach dem Lagerort sortieren, können Sie zusätzlich angeben, nach welchen Lagerebenen ein Seitenumbruch erfolgen soll. Die Einstellung ist sinnvoll, wenn Sie die Zählliste nach Lagerorten sortiert drucken. Sie können damit für jede Ebene ein eigenes Blatt drucken.
    ⇨ "Sortiert nach" auf Seite G-175

**Parameter**
Mit der Wahl der Option legen Sie fest, welche Produkte in der Zählliste aufgeführt werden sollen. Die Optionen **Fertigprodukte** und **Rohmaterial** beziehen sich auf das Kennzeichen **Rohmaterial** aus der Lagerdefinition. Wenn das Kennzeichen Rohmaterial nicht gesetzt ist, wertet das System den entsprechenden Lagerort automatisch als Lagerort für Fertigprodukte.
⇨ Stammdaten, "Lagerdefinition" auf Seite B-748
*   **Alle Artikel**: Alle Artikel der Inventurliste werden in der Zählliste gedruckt.
*   **Fertigprodukte**: Nur die Artikel der Inventurliste werden gedruckt, deren Lagerort nicht für Rohmaterial bestimmt ist.
*   **Rohmaterial**: Nur die Produkte der Inventurliste werden gedruckt, die sich an einem Lagerort für Rohmaterial befinden.
*   **Preise drucken**: Die Zählliste kann wahlweise mit oder ohne die Preise gedruckt werden.
*   **Sollbestand drucken**: Der Sollbestand kann nur auf den Zähllisten gedruckt werden, wenn die Sollbestandsermittlung ausgeführt wurde.
*   **0x0 Sätze drucken für Glasartikel**: Wenn auf dem Ausdruck Glasartikel mit den Abmessungen 0x0 ausgegeben werden sollen, muss diese Option aktiviert werden. Ohne die Option werden nur Glasartikel mit korrekten Abmessungen auf die Inventurliste gedruckt.

**Sortiert nach**
Mit der Wahl der Option legen Sie fest, wie die Artikel auf der Zählliste sortiert werden sollen:
*   **Artikel**: Die Liste wird nach Produktnummern sortiert.
*   **Abmessung**: Wenn die Zählliste Lagermaße enthält, werden die Einträge nach Breite/Höhe sortiert gedruckt.
*   **Lagerort**: Wenn die Artikel der Zählliste an verschiedenen Lagerorten gehalten werden, ist die Sortierung nach Lagerorten sinnvoll. Zusätzlich können Sie Seitenumbrüche festlegen.
    ⇨ "Seitenumbruch nach Wechsel von" auf Seite G-174

**Lagerorte drucken**
In der Übersicht werden alle Lagerorte aufgeführt, die in den Stammdaten definiert oder für die Inventurliste ausgewählt wurden. Sie können bestimmen, ob die Lagerorte in der Zählliste gedruckt werden sollen. Wenn Sie Lagerorte mit drucken möchten, müssen Sie mindestens einen auswählen.

> **Lagerort <k.A.>**
> Auch wenn Sie eigene Lagerorte hinterlegt haben, bleiben die Lagerorte `<k.A.>` erhalten und können bebucht werden.

---

### Sollbestand
**Lagerwirtschaft > Inventur > Sollbestand**

*(Abb. G-90 Sollbestand)*

Der Sollbestand entspricht dem Bestand, der vom System durch automatische oder manuelle Buchungen ermittelt wird. Er wird jeweils für eine bestimmte Inventurliste und alle Artikel ermittelt, die in der gewählten Inventurliste aufgeführt sind.
⇨ Tutorial, "Sollbestand ermitteln" auf Seite G-150

> **Keine Lagerveränderungen am Zähltag**
> Nachdem der Sollbestand ermittelt wurde, müssen die Bestände gezählt werden. Am Tag der Zählung dürfen keine Lagerartikel entnommen und keine Lagerbewegungen gebucht werden, bis die Zählung abgeschlossen ist. A+W Business wird nicht automatisch für Buchungen gesperrt.

#### Parameter
**Inv. Datum**
In der Kombobox werden alle Inventurlisten aufgeführt, die noch im System gespeichert sind. Aus dem Datum ist nicht ersichtlich, ob die Inventur abgeschlossen ist.

#### Liste
*   **Beleg Nr.**: Laufende Nummer in der Inventurliste.
*   **Art. Nr.**: Produktnummer aus den Stammdaten.
*   **Bezeichnung**: Produktbezeichnung aus den Stammdaten.
*   **Ident**: Kisten-ID (manuelle Buchung oder aus dem Wareneingang).
*   **Inhalt**: Bei Lagerartikeln und Lagermaßen wird der Wert 1 angezeigt, bei Kisten die Anzahl der Blätter.
*   **Breite, Höhe**: Die Maße werden nur angezeigt, wenn das Produkt als Lagermaß oder Kiste angelegt ist.
*   **Farbe**: Die Farbe wird nur angegeben, wenn das Produkt als Variante angelegt ist.
*   **Lagerort**: Lagerort in der Reihenfolge von Ebene 1 bis 4.
*   **EK/PE**: Einkaufspreis (EK) pro Preiseinheit. Je nach Einstellung ist das der niedrigste oder der Durchschnitts-EK.
*   **PE**: Preiseinheit für den EK.
*   **Kat.**: Diese Funktion wird nur kundenspezifisch verwendet.
*   **Soll**: Bestand, der laut System vorhanden sein sollte. Die Werte werden erst angezeigt, wenn der Sollbestand ermittelt wurde.
*   **ME**: Mengeneinheit, mit der das Produkt im Lager geführt wird.

---

### Blockerfassung
Dieser Dialog wird nur kundenspezifisch verwendet.

#### Inventurblöcke löschen
Dieser Dialog wird nur kundenspezifisch verwendet.

---

## Inventurverwaltung
**Lagerwirtschaft > Inventur > Verwaltung**

Sie geben die gezählten Mengen im Dialog **Verwaltung** ein. Lagerbuchungen können direkt nach dem Zählen wieder durchgeführt werden.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menüs in der Inventurverwaltung" auf Seite G-178
*   "Verwaltung" auf Seite G-179
*   "Gehe zu Artikel" auf Seite G-182

### Menüs in der Inventurverwaltung
**Lagerwirtschaft > Inventur > Verwaltung**

Über die Menüs der Inventurverwaltung können Sie die Standardeinstellung des Dialoges bestimmen und andere Dialoge öffnen, ohne die Inventurverwaltung zu schließen.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menü Optionen" auf Seite G-178
*   "Menü Funktionen" auf Seite G-179

#### Menü Optionen
**Lagerwirtschaft > Inventur > Verwaltung**
Das Menü ist in folgende Gruppen gegliedert:
*   "Gruppe Lagermaße" auf Seite G-178
*   "Gruppe Sortierung" auf Seite G-178

**Gruppe Lagermaße**
*   **Fläche der Lagermaße automatisch berechnen**: Die Fläche der gezählten Lagerplatten wird automatisch in Quadratmetern angezeigt.

**Gruppe Sortierung**
*   **Artikel / Lagerort / Abmessung**: Die Liste ist nach Artikeln sortiert. Diese Sortierung ist sinnvoll, wenn gleiche Artikel an mehreren Lagerorten untergebracht sind.
*   **Abmessung / Artikel / Lagerort**: Die Liste ist nach den Größen der Lagermaße sortiert. Diese Sortierung ist sinnvoll, wenn Sie die Lagermaße in eigenen Zähllisten erfasst haben.
*   **Lagerort / Artikel / Abmessung**: Die Liste wird nach Lagerorten sortiert. Diese Sortierung ist sinnvoll, wenn Sie auch die Zähllisten nach Lagerorten sortiert haben.
*   **Beleg Nr.**: Belegnummer aus der Inventurliste

#### Menü Funktionen
**Lagerwirtschaft > Inventur > Verwaltung**
Folgende Einträge werden angezeigt:
*   **Gehe zu Artikel**: Öffnet den Dialog **Gehe zu Artikel**.
    ⇨ "Gehe zu Artikel" auf Seite G-182
*   **Menge für markierte Artikel auf Null setzen**: Die Menge wird auf null gesetzt. Diese Funktion ist sinnvoll, wenn Sie mehrere Belege markieren. Sie brauchen dann nicht jeden einzelnen auf null zu setzen.
*   **Lagerort für markierte Artikel setzen**: Der Lagerort wird für alle markierten Belege umgesetzt.

---

### Verwaltung
**Lagerwirtschaft > Inventur > Verwaltung**

**Zu Dialogbeschreibung:**
*   Gehe zu Artikel
*   Wertberichtigung

*(Abb. G-91 Inventurverwaltung)*

In diesem Dialog erfassen Sie die gezählten Mengen. Die Liste zeigt die Einträge, die Sie mit der Inventurliste ausgewählt haben. Lagerbuchungen können direkt nach dem Zählen wieder durchgeführt werden.
⇨ Tutorial, "Inventurwerte erfassen" auf Seite G-152

> **Kiste inventarisieren**
> Wenn für die Inventurliste der Sollbestand ermittelt wurde, können Kisten auch per Scanner erfasst und in die Inventurliste aufgenommen werden. Dazu müssen die Kisten-ID, der Lagerort und ggf. eine abweichende Blattanzahl gescannt werden.

#### Eingabemaske
*   **Inventurdatum**: Angabe des Datums der Inventurliste.
*   **Artikelnummer**: Nummer des Artikels, dessen Menge erfasst werden soll.
*   **Breite, Höhe**: Die Maße werden nur bei Lagerplatten und Kisten eingetragen. Für alle anderen Artikel steht in den beiden Feldern eine Null (0).
*   **Kategorie**: Diese Funktion wird nur kundenspezifisch verwendet, um Kategorien für die Wertberichtigung des Lagers zu verwenden.
*   **Inv. Preis**: Für die Lagerbewertung kann ein Inventurpreis manuell eingetragen werden. Dieser Preis wird nach dem Abschluss der Inventur nicht in die EK-Preistabelle zurückgeschrieben und fließt nicht in die Berechnung des Durchschnitts-EKs ein. Wenn kein Inventurpreis eingetragen wird, gilt der niedrigste oder der Durchschnitts-EK je nach Einstellung in der Inventurliste.
*   **Inhalt**: Anzeige der Stückzahl bei Kisten. Wenn Kisten als Einheit gezählt wurden, darf die Kiste nicht aufgelöst sein, d. h., es dürfen keine Platten entnommen sein.
*   **Bezeichnung**: Artikelbezeichnung aus den Produktstammdaten.
*   **Farbe**: Bei Artikeln mit Farbzuweisungen (Variante) kann die Stückzahl pro Farbe eingetragen werden.
*   **Ident**: Kisten-ID (manuelle Buchung oder aus dem Wareneingang).
*   **Lagerort**: Lagerort des gezählten Artikels.
    > **Lagerort <k.A.>**
    > Auch wenn Sie eigene Lagerorte hinterlegt haben, bleiben die Lagerorte `<k.A.>` erhalten und können bebucht werden.
*   **Menge**: In diesem Feld erfassen Sie die gezählte Menge aus der Zählliste. Sie können die Mengen erst eingeben, nachdem Sie den Sollbestand ermittelt haben.

#### Tabelle
In der Übersicht sind alle Artikel aufgelistet, die in der Inventur gezählt und bewertet werden sollen.
*   **Beleg Nr.**: Laufende Nummer in der Inventurliste.
*   **Art. Nr.**: Produktnummer aus den Stammdaten.
*   **Bezeichnung**: Produktbezeichnung aus den Stammdaten.
*   **Inhalt**: Bei Lagerartikeln und Lagermaßen wird der Wert 1 angezeigt, bei Kisten die Anzahl der Blätter.
*   **Ident**: Kisten-ID (manuelle Buchung oder aus dem Wareneingang).
*   **Breite, Höhe**: Die Maße werden nur angezeigt, wenn das Produkt als Lagermaß oder Kiste angelegt ist.
*   **Lagerort**: Lagerort in der Reihenfolge von Ebene 1 bis 4.
*   **EK / PE**: Einkaufspreis (EK) pro Preiseinheit. Je nach Einstellung ist das der niedrigste oder der Durchschnitts-EK.
*   **PE**: Preiseinheit für den EK.
*   **Kategorie**: Diese Funktion wird nur kundenspezifisch verwendet.
*   **Menge**: Wert, der als gezählte Menge eingegeben wurde.
*   **ME**: Mengeneinheit, mit der das Produkt im Lager geführt wird.

---

### Gehe zu Artikel
**Lagerwirtschaft > Inventur > Verwaltung > Menü Funktionen > Gehe zu Artikel...**

*(Abb. G-92 Gehe zu Artikel)*

In diesem Dialog können Sie die Markierung auf den ersten Beleg zum angegebenen Artikel setzen.
*   **Artikel**: Nummer des Lagerartikels, zu dem Sie in der Liste springen möchten.

### Wertberichtigung
**Lagerwirtschaft > Inventur > Verwaltung > Feld Kategorie > Symbol Ordner**

*(Abb. G-93 Wertberichtigung)*

In diesem Dialog hinterlegen Sie Kategorien und Prozentwerte für die Berichtigung des Lagerwerts.
Der Dialog ist nur kundenspezifisch freigeschaltet.

---

## Inventurabschluss
**Lagerwirtschaft > Inventur > Abschluss**

Mit dem Inventurabschluss beenden Sie die Inventur. Lagerbuchungen können direkt nach dem Zählen wieder durchgeführt werden.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menüs im Inventurabschluss" auf Seite G-183
*   "Abschluss" auf Seite G-184

### Menüs im Inventurabschluss
**Lagerwirtschaft > Inventur > Abschluss**
Über die Menüs können Sie die Standardeinstellung bestimmen und andere Dialoge öffnen, ohne den Dialog zu schließen.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menü Optionen" auf Seite G-183
*   "Menü Funktionen" auf Seite G-183

#### Menü Optionen
**Lagerwirtschaft > Inventur > Abschluss**
Folgende Einträge werden angezeigt:
*   **Artikel mit Bestand = 0 nicht drucken**: Nur Artikel, deren Bestand größer als 0 ist, werden gedruckt. Diese Einstellung ist sinnvoll, wenn es sehr viele Artikel ohne Bestandszahlen gibt. Die gedruckte Liste wird dann übersichtlicher.
*   **Bei nicht gezählten Artikeln nachfragen, ob Bestand auf 0 gesetzt werden soll**: Mit dieser Funktion legen Sie fest, dass die Menge von Artikel, zu denen kein Bestand erfasst wurde, erst dann auf 0 gesetzt wird, wenn Sie dies pro Artikel bestätigt haben.

#### Menü Funktionen
**Lagerwirtschaft > Inventur > Abschluss**
Folgende Einträge werden angezeigt:
*   **Nachtragsinventur anhängen**: Öffnet den Dialog **Inventurliste wählen**, um zwei verschiedene Inventuren in einer gemeinsamen Liste zu drucken und auszuwerten.
    ⇨ "Inventurliste wählen" auf Seite G-186

---

### Abschluss
**Lagerwirtschaft > Inventur > Abschluss**

**Zu Dialogbeschreibung:**
*   Inventurliste wählen

*(Abb. G-94 Inventurabschluss)*

In diesem Dialog schließen Sie die Inventur pro Inventurliste einzeln ab. Damit werden die erfassten Werte in die Lagerbestände (Bestandslisten) übernommen. Ab- und Zugänge, die in der Zwischenzeit erfasst wurden, werden dabei berücksichtigt. Neue Lagerartikel aus der Inventur werden automatisch in die Lagerverwaltung übernommen.
⇨ Tutorial, "Inventur abschließen" auf Seite G-155

> **Pro Inventurliste nur ein Abschluss**
> Der Inventurabschluss kann nur einmal pro Inventurliste ausgeführt werden. Eingabefehler können nach dem Abschluss nur in der Lagerverwaltung korrigiert werden. Alternativ dazu kann eine neue Inventurliste mit den fehlerhaft erfassten Artikeln erstellt werden.

#### Einbuchung
*   **Inventurdatum**: Datum der Inventur, die abgeschlossen werden soll.
*   **Verbuchung nach Beschaffungsart aus AV-Bereich**: Wenn Sie mit AV-Bereichen arbeiten, können die Bestände einem bestimmten AV-Bereich zugeordnet sein, z. B. für die Produktion von VSG. Das Feld zur Auswahl des AV-Bereichs ist nur freigeschaltet, wenn Sie die Checkbox markiert haben.
    *   ☐ Die gezählten Bestände werden dem Standard-Lagerort zugeordnet.
    *   ☑ Die Bestände sollen einem AV-Bereich zugeordnet werden.
        ⇨ Stammdaten, "AV-Bereiche" auf Seite B-1033
*   **Beleg Nr. von ... bis**: Anzeige der ersten und letzten Belegnummer der geladenen Inventurliste.

#### Übersicht
*   **Beleg Nr.**: Laufende Nummer in der Inventurliste.
*   **Art. Nr.**: Produktnummer aus den Stammdaten.
*   **Bezeichnung**: Produktbezeichnung aus den Stammdaten.
*   **Inhalt**: Bei Lagerartikeln und Lagermaßen wird der Wert 1 angezeigt, bei Kisten die Anzahl der Blätter.
*   **Ident**: Kisten-ID (manuelle Buchung oder aus dem Wareneingang).
*   **Breite, Höhe**: Die Maße werden nur angezeigt, wenn das Produkt als Lagermaß oder Kiste angelegt ist.
*   **Lagerort**: Lagerort in der Reihenfolge von Ebene 1 bis 4.
*   **Menge**: Wert, der als gezählte Menge eingegeben wurde.
*   **ME**: Mengeneinheit, mit der das Produkt im Lager geführt wird.
*   **Status**: Ein Status wird nur angezeigt, wenn der Beleg nicht verbucht werden konnte. Über das Logbuch können Sie nach den möglichen Ursachen suchen.

---

### Inventurliste wählen
**Lagerwirtschaft > Inventur > Abschluss > Menü Funktionen > Nachtragsinventur anhängen**

*(Abb. G-95 Nachtragsinventur anhängen)*

Eine Nachtragsinventur kann nur angehängt werden, wenn beide Inventuren abgeschlossen sind. Die beiden Inventuren können dann auf einer gemeinsamen Liste gedruckt und ausgewertet werden.
⇨ Tutorial, “So hängen Sie eine Nachtragsinventur an" auf Seite G-157

---

## Lagerverwaltung
**Lagerwirtschaft > Lagerverwaltung**

Im Dialog **Lagerverwaltung** können Sie sich alle Artikel anzeigen lassen, die im Lager verwaltet werden.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menüs in der Lageverwaltung" auf Seite G-187
*   "Lagerverwaltung" auf Seite G-188

### Menüs in der Lageverwaltung
**Lagerwirtschaft > Lagerverwaltung**

Über die Menüs können Sie die Standardeinstellung des Dialoges bestimmen und andere Dialoge öffnen, ohne den Dialog zu schließen.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menü Funktionen" auf Seite G-187
*   "Menü Optionen" auf Seite G-188
*   "Menü Druck" auf Seite G-188

#### Menü Funktionen
**Lagerwirtschaft > Lagerverwaltung > Menü Funktionen**
Über dieses Menü können Sie andere Dialoge öffnen, ohne die Lagerverwaltung zu schließen.
Folgende Einträge werden angezeigt:
*   **Lagerhistorie**: Öffnet den Dialog **Lagerhistorie** mit dem Protokoll der Vorgänge, die in der Lagerverwaltung gebucht wurden.
    ⇨ "Lagerhistorie" auf Seite G-207
*   **Buchungsjournal**: Öffnet den Dialog **Buchungsjournal** mit dem Protokoll der Lagerbuchungen aus Aufträgen und Bestellungen.
    ⇨ "Buchungsjournal" auf Seite G-205
