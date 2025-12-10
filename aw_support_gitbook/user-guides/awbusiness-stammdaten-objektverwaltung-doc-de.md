---
description: "DE_AWBusiness_Stammdaten_9_6"
---


# Tutorial 2: Zusatzinformationen

[Symbol: Speichern]

6. Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
   Die Daten werden gespeichert. Die Preise werden berechnet und die Preisanzeigen werden aktualisiert.
7. Schließen Sie die Positionserfassung.
   Sie sich können eine Liste der bisher zum Objekt erfassten Aufträge anzeigen lassen.
8. Wechseln Sie zum Register **Konditionen** und klicken Sie auf die Lupe rechts neben dem Namen des Objekts.

[Abbildung: Screenshot der Kundenaufträge zum Objekt]
*Abb. B-313: Kundenaufträge zum Objekt*

*   **A**: Bisher zum Objekt erfasste Aufträge
*   **B**: Summe aus den erfassten Aufträgen
*   **C**: Maximalwerte aus der Objektdefinition

Die Anzeige gibt nur die Aufträge des aktuellen Kunden wieder.

---
## Erweiterte Objektverwaltung

Mit der erweiterten Objektverwaltung können Sie zu den Objekten zusätzliche Bedingungen definieren, z. B. Zahlungsbedingungen.

Stellen Sie zunächst sicher, dass Sie in den Firmendaten die **Erweiterte Objektverwaltung** aktiviert haben.
⇨ "Objektverwaltung einstellen" auf Seite B-497

Folgende Schritte müssen Sie ausführen, bevor Sie einen Auftrag zu einem Objekt erfassen:
*   Objekt anlegen
*   Objekt dem Kunden zuordnen
*   Preis zum Kunden und Objekt anlegen (optional)
*   Rabatt zum Objekt anlegen (optional)

### Mit erweiterten Objekten arbeiten

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So richten Sie ein Objekt ein" auf Seite B-502
*   "So prüfen Sie die aufgelaufene Summen" auf Seite B-504

### So richten Sie ein Objekt ein

1. Legen Sie ein Objekt an.
2. Ordnen Sie das Objekt dem Kunden zu.

[Abbildung: Screenshot der erweiterten Objekteinstellungen]
*Abb. B-314: Erweiterte Objekteinstellungen*

*   **A**: Zeitraum für die Erfassung von Aufträgen
*   **B**: Vertreter für die Provisionsabrechnung
*   **C**: Abweichende Zahlungsbedingung
*   **D**: Status

3. Legen Sie die Gültigkeit fest (A), wenn für diese Objekt nach einem bestimmten Datum keine Aufträge mehr erfasst werden dürfen.
   Wenn das Objekt früher abgeschlossen wird, können Sie den Status (D) auf **komplett** umsetzen.
4. Legen Sie einen abweichenden Vertreter (B) und/oder abweichende Zahlungsbedingung (C) fest.
   Bei der Erfassung von Aufträgen werden diese Informationen mit in den Auftrag übernommen, sobald das Objekt dem Auftrag zugeordnet ist.
5. Wechseln Sie zum Register **Veranschlagte Mengen**.

[Abbildung: Screenshot der erweiterten Objekteinstellungen - Veranschlagte Mengen]
*Abb. B-315: Erweiterte Objekteinstellungen - Veranschlagte Mengen*

*   **A**: Auswahl des Produkts
*   **B**: Auswahl der Warengruppe
*   **C**: Eingabefelder für die Mengen
*   **D**: Eingabefelder freischalten

6. Klicken Sie auf die Schaltfläche (D), um die Eingabefelder freizuschalten.
7. Wählen Sie die Option **Produkt** (A) oder **WGR** (B), für die Sie die Werte angeben wollen.
8. Tragen Sie die veranschlagten Mengen ein (C).

[Abbildung: Screenshot der veranschlagten Mengen mit eingegebenen Werten]

9. [Symbol: Speichern] Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
   Sie können jetzt Aufträge für den Kunden erfassen und dabei das Objekt angeben. Die aufgelaufenen Summen eines Objektes werden nach dem Speichern einer Auftragsposition aktualisiert.
   Wenn der Status eines Objektes auf **komplett** gesetzt ist, kann dafür kein Auftrag mehr erfasst werden. Damit können Sie das Objekt sperren, bevor die Gültigkeit abgelaufen ist. Wenn das Gültig-bis-Datum erreicht ist, wird das Objekt automatisch gesperrt.

### So prüfen Sie die aufgelaufene Summen

1. Wechseln Sie zum Dialog **Abrechnungen > Summen**.
   In diesem Register werden die Summen für den aktuellen Kunden aufgeführt.

[Abbildung: Screenshot der aufgelaufenen Summen für Produkte]
*Abb. B-316: Aufgelaufene Summen*

*   **A**: Produkt, zu dem Mengen hinterlegt sind
*   **B**: Warengruppen, zu denen die in den Aufträgen erfassten Produkte gehören

Für das Produkt (A) wird angezeigt, wie weit die Objektgrenzen aus dem Register **Veranschlagte Mengen** bereits erreicht sind.

[Abbildung: Screenshot der aufgelaufenen Summen für Produkte ohne vereinbarte Mengen]
*Abb. B-317: Aufgelaufene Summen*

*   **A**: Produkt ohne Vereinbarungen der Menge
*   **B**: Veranschlagter Umsatz erreicht

Sind für ein Produkt oder eine Warengruppe die veranschlagten Mengen erreicht oder sogar überschritten, werden diese Einträge in der ersten Zeile in roter Schrift (B) dargestellt.

Produkte, für die keine Mengen angegeben sind, werden ebenfalls aufgeführt. Auch für diese Produkte werden die entsprechenden Warengruppen angezeigt. Die Mengen werden jedoch lediglich bei der Gesamtsumme des Preises berücksichtigt.

Die in den Registern **Veranschlagte Mengen** und **Summen** angezeigten Informationen können gedruckt werden.

2. Wählen Sie im Menü **Druck > Bildschirm > Druck nach Produkt**, um sich die Übersicht anzeigen zu lassen.
3. Bestätigen Sie die Drucker-Einstellungen, um den Druck zu starten.
   Auf die gleiche Weise können Sie die Ausgabe der Übersicht direkt auf einen Drucker schicken.

[Abbildung: Screenshot des Ausdrucks "Objektübersicht nach Produkten"]
*Abb. B-318: Aufgelaufene Summen über alle beteiligten Kunden*

Im Ausdruck werden alle Objekte und Kunden aufgeführt.
Wenn Sie sich also einen Überblick über die Gesamtsummen zu einem Objekt verschaffen wollen, dann wählen Sie das Objekt aus und starten den Druck.

## Abrechnungsverwaltung mit zugeordneten Aufträgen

In diesem Modus können Sie einen Rahmenauftrag einem Objekt zuordnen. Im Rahmenauftrag erfassen Sie für die einzelnen Positionen Produkte ohne detaillierte Angaben über den Produktaufbau, also z. B. ein ISO-Produkt ohne Angaben zu Bearbeitungen, Sprossen oder Modellen.

Von dem Rahmenauftrag aus erstellen Sie Forderungen, in denen Sie angeben, wie viel Prozent, Stück oder welcher Betrag vom ursprünglichen Rahmenauftrag eingefordert wird. Wenn Sie eine Forderung erstellen, wird automatisch ein Auftrag vom Typ **Forderung** erstellt.

Für diese Forderungen werden keine Rechnungen erzeugt. Sie werden in einem speziellen Modus an die FiBu übergeben. Wenn der Rahmenauftrag erfüllt und damit abgeschlossen ist, stellen Sie den (gesamten) Rahmenauftrag in Rechnung.

Für die Produktion und Lieferung an den Kunden erzeugen Sie Produktionsaufträge und ordnen diese dem (Abrechnungs-)Objekt zu. Zu diesen Produktionsaufträgen können auch Bestellungen erzeugt werden, die ebenfalls dem Objekt zugeordnet werden. Diese Bestellungen können sowohl manuell als auch über die automatische Bestellübergabe erzeugt werden. Beide Arten von Bestellungen können in einer Übersicht separat angezeigt werden. Für die Produktionsaufträge werden keine Rechnungen erstellt.

[Abbildung: Flussdiagramm der Abrechnungsverwaltung]
*Abb. B-319: Abrechnungsverwaltung mit zugeordneten Aufträgen*

**Flussdiagramm-Beschreibung:**
- **Rahmenauftrag** (mit Betrag, Menge, Prozent) führt zu **Forderungsrechnungen**.
- **Forderungsrechnungen** führen zu einer **Spezielle FiBu-Übergabe**.
- Das **Abrechnungsverwaltung (Objekt)** ist zentral.
- Vom **Abrechnungsverwaltung (Objekt)** gehen Pfeile zu:
    - **Gesamtrechnung am Projektende**, welche zu einer **FiBu-Übergabe** führt.
    - **Produktionsaufträge**.
    - **Bestellungen**, die zu **Gutschriften** führen können.

> Wenn ein Objekt als **komplett** markiert ist, kann dazu kein Auftrag mehr erfasst werden. Dieser Status wird automatisch gesetzt, sobald die Mengen aus dem Rahmenauftrag in den Forderungsrechnungen erreicht ist.

## Rahmenauftrag abrechnen

Sie können Preise und Rabatte für den Kunden festlegen, für den Sie Rahmenaufträge erfassen. Wenn für den Rahmenauftrag gesonderte Konditionen gelten sollen, dann müssen Sie die entsprechenden Preise, Rabatte oder Zuschläge für den Kunden festlegen.

Für die Abrechnung von Rahmenaufträgen muss in den Firmendaten eine der folgenden Einstellungen gewählt sein:
*   Abrechnungsverwaltung mit zugeordneten Aufträgen
*   Standard Objektverwaltung + Abrechnungsverwaltung mit zugeordneten Aufträgen

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So legen Sie einen Rahmenauftrag an" auf Seite B-509
*   "So erfassen Sie einen Auftrag zu einem Rahmenauftrag" auf Seite B-512
*   "So erstellen Sie eine Forderungsrechnung" auf Seite B-514
*   "So schließen Sie einen Rahmenauftrag ab" auf Seite B-517

### So legen Sie einen Rahmenauftrag an

1.  Legen Sie in der Auftragserfassung den Rahmenauftrag mit dem Dokumententyp **Rahmenauftrag** an.

[Abbildung: Screenshot der Auftragserfassung mit Dokumententyp Rahmenauftrag]
*Abb. B-320: Rahmenauftrag*

*   **A**: Dokumententyp Rahmenauftrag

2.  Erfassen Sie die Produkte, die über diesen Rahmenauftrag abgerechnet werden sollen.
    Dabei reicht es aus, wenn Sie z. B. ein ISO-Produkt erfassen, ohne weitere Angaben zu Sprossen, Modellen oder Bearbeitungen zu machen.
3.  Speichern Sie den Auftrag und schließen Sie die Auftragserfassung.
4.  Wählen Sie **Dokumente > Objektabrechnungen > Abrechnungen**.
    Der Dialog **Abrechnungen** wird geöffnet.
5.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    Die Eingabefelder werden freigeschaltet.

[Abbildung: Screenshot zum Anlegen eines Abrechnungsobjekts]
*Abb. B-321: Abrechnungsobjekt zum Rahmenauftrag anlegen*

*   **A**: Referenz auf Angebot oder Kundenauftrag
*   **B**: Abrechnungsnummer
*   **C**: Kundennummer
*   **D**: Nummer des Rahmenauftrags
*   **E**: Status

6.  Tragen Sie folgende Daten ein:
    *   Abrechnungsnummer (B)
    *   Kundennummer (C) zu
    *   Nummer des Rahmenauftrags (D)
    Sie können als Referenz (A) die Nummer des Angebots und/oder die Nummer des Auftrags eintragen, den der Kunde erteilt hat.
    Wenn die Aufträge an eine andere Anschrift ausgeliefert werden sollen, tragen Sie die entsprechenden Daten ein, z. B. eine Filiale des Kunden.
7.  [Symbol: Speichern] Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Damit haben Sie ein Abrechnungsobjekt zu Ihrem Rahmenauftrag angelegt.
    Im Register **Rahmenauftrag** können Sie sich die Positionen des Rahmenauftrags anzeigen lassen. Wenn die Daten nicht sofort angezeigt werden, dann lesen Sie den Rahmenauftrag im Auswahlmodus neu ein.

[Abbildung: Screenshot der Positionen des Rahmenauftrags]
*Abb. B-322: Positionen des Rahmenauftrags*

Damit sind die Vorbereitungen für die Abrechnungen abgeschlossen. Sie können jetzt die Forderungsrechnungen und die zugehörigen Produktionsaufträge erfassen.

### So erfassen Sie einen Auftrag zu einem Rahmenauftrag

1.  Wählen Sie **Dokumente > Auftrag > Auftrag**.
2.  Wählen Sie im Menü **Bearbeiten > Neu**.
3.  Tragen Sie die Kopfdaten im Register **Dokument** ein.

[Abbildung: Screenshot eines Produktionsauftrags zum Rahmenauftrag]
*Abb. B-323: Produktionsauftrag zum Rahmenauftrag*

*   **A**: Dokumententyp Produktionsauftrag
*   **B**: Abrechnungsnummer

4.  Wählen Sie den Dokumententyp (A) **Produktionsauftrag**.
5.  Tragen Sie die Abrechnungsnummer (B) ein.
    Die Abrechnungsnummer steht nicht mehr zur Verfügung, wenn die veranschlagte Menge aus dem Rahmenauftrag ausgeschöpft ist.
6.  [Symbol: Speichern] Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
7.  Wechseln Sie zum Register **Positionen** und erfassen Sie die Positionen und Mengen, die gefertigt und geliefert werden sollen.
    Sie können jetzt auch Modelle, Sprossen und Bearbeitungen zu den Positionen erfassen.
8.  Bearbeiten Sie den Auftrag weiter, z. B. indem Sie ihn an die Produktion und/oder den Einkauf übergeben.

Im Dialog **Abrechnungen** können Sie sich anzeigen lassen, welche Aufträge bisher erfasst wurden und welche Mengen noch offen sind.

[Abbildung: Screenshot der zugeordneten Aufträge im Dialog Abrechnungen]
*Abb. B-324: Zugeordnete Aufträge*

### So erstellen Sie eine Forderungsrechnung

1.  Wählen Sie **Dokumente > Objektabrechnungen > Abrechnungen**.
    Der Dialog **Abrechnungen** wird geöffnet.
2.  Lassen Sie sich die Abrechnung anzeigen, zu der Sie eine Forderungsrechnung erstellen wollen.
3.  Wählen Sie im Menü **Funktionen > Forderungsrechnung erstellen**.

[Abbildung: Screenshot des Dialogs Forderungsrechnung]
*Abb. B-325: Forderungsrechnung*

*   **A**: Menge, die abgerechnet werden soll
*   **B**: Mengeneinheit

4.  Tragen Sie die Menge (A) und die Mengeneinheit (B) ein, die berechnet werden soll, z. B. 25 Stk.
    Sie können pro Position zwischen Menge, Prozent und Betrag wählen. Die Wahl der ersten Forderung müssen Sie bei den nächsten Forderungen pro Position beibehalten.
5.  Klicken Sie auf **[OK]**, um die Daten zu speichern.
    Die Daten werden gespeichert. Der Dialog wird geschlossen und der Dialog **Abrechnungen** wird wieder angezeigt. Im Register **Rahmenauftrag** werden die Werte in den entsprechenden Spalten aktualisiert.

[Abbildung: Screenshot der aktualisierten Positionen des Rahmenauftrags]

In der Dokumentenverwaltung wird ein Auftrag vom Typ **Forderung** angelegt.

[Abbildung: Screenshot des angelegten Dokuments vom Typ Forderung]
*Abb. B-326: Dokument Forderung*

*   **A**: Dokumententyp
*   **B**: Abrechnungsnummer

Der Typ **Forderung** (A) und die Abrechnungsnummer (B) werden automatisch gesetzt.
6.  Wechseln Sie in die Positionserfassung und prüfen Sie die Positionen.
    Zu diesem Auftrag können Sie keine Rechnung drucken. Wenn Sie den Rechnungsdruck starten, wird folgende Meldung angezeigt:

    > **Frage [3483]**
    > ? Es werden 1 Dokumente nicht verarbeitet! Möchten Sie den Druck dennoch starten?
    > [Ja] [Nein]

7.  Starten Sie den Rechnungsdruck trotzdem, damit der Auftragsstatus umgesetzt wird.
    Wenn der Vorgang beendet ist, wird die erfolgreiche Verarbeitung gemeldet.
    Eine Rechnung wurde jedoch nicht erzeugt.

[Abbildung: Screenshot des Rechnungsdruck-Dialogs nach einem Forderungsauftrag]
*Abb. B-327: Keine Rechnung für Forderungsaufträge*

*   **A**: Status
*   **B**: Rechnungsnummer

In den Feldern für die Rechnungsnummer und den Rechnungsbetrag wird jeweils der Wert 0 angezeigt. Der Status des Dokuments wird dennoch auf **gedruckt** umgesetzt.

Damit kann die Forderung an die FiBu übergeben und abgeschlossen werden.

### So schließen Sie einen Rahmenauftrag ab

1.  Wählen Sie **Dokumente > Objektabrechnungen > Abrechnungen**.
    Der Dialog **Abrechnungen** wird geöffnet.
2.  Lassen Sie sich das (Abrechnungs-)Objekt anzeigen, das Sie abschließen wollen.
    Wenn alle Mengen erfüllt sind, wird der Status des Objekts auf **komplett** gesetzt.

[Abbildung: Screenshot des Objektstatus "Komplett"]

3.  Im Register **Rahmenauftrag** können Sie prüfen, ob alle berechneten Mengen auf 100 % gesetzt sind.

[Abbildung: Screenshot eines erfüllten Rahmenauftrags (100%)]
*Abb. B-328: Rahmenauftrag erfüllt*

4.  Öffnen Sie in der Dokumentenverwaltung den Rahmenauftrag und schließen Sie ihn mit dem Rechnungsdruck und der Übergabe an die FiBu ab.

# Softwarereferenz

## Übersicht

Im Modul **Stammdaten** werden alle Daten zu A+W Business eingerichtet und gepflegt, die übergreifend von allen Modulen genutzt werden.
Die Stammdaten sind in folgende Menüs gegliedert:
*   "Allgemein" auf Seite B-556
*   "Produkte" auf Seite B-564
*   "Preise" auf Seite B-661
*   "Lager" auf Seite B-735
*   "Marktpartner" auf Seite B-743
*   "Versand" auf Seite B-861
*   "Fertigung" auf Seite B-869
*   "Auftrag" auf Seite B-881
*   "Finanzen" auf Seite B-904
*   "Firma" auf Seite B-917
*   "Texte" auf Seite B-1044
*   "Formulare" auf Seite B-1050
*   "CEKAL" auf Seite B-1075
*   "CE-Kennzeichen" auf Seite B-1084
*   "B2B" auf Seite B-1088

> **Schaltflächen in den Dialogen**
> Die Standard-Schaltflächen und -menüs sind ausführlich im Part Übersicht und in den Tutorials beschrieben. Auf sie wird daher in der Beschreibung der Dialoge nicht eingegangen.

## Allgemein

*Stammdaten > Allgemein*

In diesem Programmbereich sind allgemeine Daten hinterlegt. Im Menü **Allgemein** finden Sie folgende Einträge:

*   "Sprachen" auf Seite B-556
*   "Monate" auf Seite B-558
*   "Tage" auf Seite B-558
*   "Landeskürzel" auf Seite B-559
*   "Kalender" auf Seite B-560
*   "Basisnummernkreise" auf Seite B-562

### Sprachen

*Stammdaten > Allgemein > Sprachen*

[Abbildung: Screenshot des Dialogs "Sprachen"]
*Abb. B-344: Sprache für Korrespondenz*

In diesem Dialog tragen Sie alle Sprachen ein, in denen Sie mit Ihren Kunden in schriftlicher Form korrespondieren. An erster Stelle steht immer Ihre Korrespondenzsprache. Sie können diese nicht nachträglich ändern.
Dieser Dialog steht nur mit dem Modul **Mehrsprachigkeit** zur Verfügung.

**Menü Funktionen**
Über dieses Menü können Sie den Dialog **Anlage Preis-/Mengeneinheit für Mehrsprachigkeit** öffnen, um die Bezeichnungen für Preis- und Mengeneinheiten in eine neu angelegte Sprache zu kopieren.

*   **Bezeichnung**: Name der Sprache.
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Produktion oder die Finanzbuchhaltung.

### Preis-/Mengeneinheit für Mehrsprachigkeit

*Stammdaten > Allgemein > Sprachen > Menü Funktionen > Einheiten kopieren*

[Abbildung: Screenshot des Dialogs "Anlage Preis-/Mengeneinheit für Mehrsprachigkeit"]
*Abb. B-345: Anlage Preis-/Mengeneinheit für Mehrsprachigkeit*

In diesem Dialog kopieren Sie die Bezeichnungen für Preis- und Mengeneinheiten in eine neu angelegte Sprache, wenn Sie das Modul **Mehrsprachigkeit** einsetzen. Anschließend müssen Sie diese Bezeichnungen in die neue Sprache übersetzen.

**Preis-/Mengeneinheit**

*   **Quellsprache**: Standardmäßig wird die Basissprache vorgeschlagen. Sie können jede andere Sprache auswählen, in der die Preis- und Mengeneinheiten vorhanden sind.
*   **Zielsprache**: Zielsprache, in die die Preis- und Mengeneinheiten kopiert werden sollen.
    Im Dialog **Preis/Menge** müssen anschließend Sie die Bezeichnungen in dem entsprechenden Sprachregister übersetzen.
    ⇨ "Preis- und Mengeneinheit" auf Seite B-702

### Monate

*Stammdaten > Allgemein > Monate*

[Abbildung: Screenshot des Dialogs "Monate"]
*Abb. B-346: Monate*

Die Monatsnamen sind standardmäßig mit der Basissprache vorbelegt und sollten nicht geändert werden.

*   **Bezeichnung**: Name des Monats.
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für statistische Auswertungen.

### Tage

*Stammdaten > Allgemein > Tage*

[Abbildung: Screenshot des Dialogs "Tage"]
*Abb. B-347: Wochentage*

Die Tagesnamen sind standardmäßig mit der Basissprache vorbelegt und sollten nicht geändert werden.

*   **Bezeichnung**: Name des Wochentags.
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für statistische Auswertungen.

### Landeskürzel

*Stammdaten > Allgemein > Landeskürzel*

[Abbildung: Screenshot des Dialogs "Landeskürzel"]
*Abb. B-348: Landeskürzel*

In diesem Dialog verwalten Sie die internationalen Landeskürzel und ordnen die Standardrundung für die Steuer zu.

*   **Landeskürzel**: Landeskürzel, z. B. D = Deutschland, F = Frankreich, USA = United States of America. Das Kürzel weisen Sie im Dialog **Partnerverwaltung** Ihren Kunden und Lieferanten zu, damit die Texte in der Sprache des Partners angezeigt und gedruckt werden, z. B. die Mengeneinheiten.
    ⇨ "(Land, Provinz)" auf Seite B-761
*   **Bezeichnung**: Name des Landes, z. B. Deutschland, Frankreich.
*   **Rundung Mwst**: Sie können für jedes Land festlegen, auf welchen Wert die Mehrwertsteuer gerundet werden soll. Zum Beispiel bedeutet 1, dass auf den nächsten Wert auf- oder abgerundet wird, bei 5 wird auf die nächste 5 auf- oder abgerundet.
    ⇨ Tutorial 2, "Rundungen" auf Seite B-442
    ⇨ "Rundung (Kunde, Lieferant)" auf Seite B-840
    ⇨ "Rundung" auf Seite B-881
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für statistische Auswertungen.
*   **Gesperrt**: Ein Landeskürzel kann für die Erfassung in der Partnerverwaltung und in den Dokumenten gesperrt werden, wenn es nicht mehr benötigt wird.
    *   ☐ Das Landeskürzel kann zugewiesen werden.
    *   ☑ Das Landeskürzel ist gesperrt und kann nicht mehr zugewiesen werden. Wenn es Partnern und in Dokumenten zugewiesen ist, wird es jedoch weiterhin angezeigt.
*   **Internationales Kennzeichen**: Zweistelliges internationales Landeskürzel, z. B. DE = Deutschland, FR = Frankreich, US = United States of America.

### Kalender

*Stammdaten > Allgemein > Kalender*

[Abbildung: Screenshot des Dialogs "Kalender"]
*Abb. B-349: Kalender*

In diesem Dialog pflegen Sie die Feiertage und die täglichen Arbeitsstunden in Ihrem Unternehmen. Wenn im Feld **Stunden** ein Wert größer 0 steht, gilt dieser als Arbeitstag. Wenn Sie einen Tag als Feiertag definieren möchten, müssen Sie den Wert 0 eintragen.
⇨ Tutorial 1, "Allgemeinen Kalender anlegen" auf Seite B-101

**Arbeitswoche**
*   **Wochentag**: Anzahl der regulären Arbeitsstunden für jeden Wochentag. Die Feiertage müssen Sie auf 0 (Stunden) setzen.
    *   ☐ Der Wochentag wird nicht in die Arbeitswoche aufgenommen.
    *   ☑ Der Wochentag wird in die Arbeitswoche aufgenommen.

**Auswahl**
*   **Jahr, KW**: Auswahl des Jahres und der Kalenderwoche, um die entsprechende Kalenderwoche in der Übersicht anzuzeigen.
*   **[Auf Jahr übertragen]**: Überträgt die Änderungen auf alle entsprechenden Wochentage des gesamten Kalenderjahrs. Die Freitage müssen Sie danach auf 0 setzen.
*   **[Auf KW übertragen]**: Überträgt die Änderungen auf alle Tage der aktuellen Kalenderwoche. Die entsprechenden Wochentage des restlichen Kalenderjahrs bleiben unverändert.
*   **[Zur aktuellen KW]**: Mit dieser Schaltfläche lassen Sie sich die aktuelle Kalenderwoche anzeigen.

**Übersicht**
In der Übersicht werden alle Kalenderwochen des aktuellen Kalenderjahrs mit den Tagesarbeitszeiten angezeigt. Die Wochenenden sind in roter Schrift dargestellt.

### Länder Kalender

*Stammdaten > Allgemein > Länder Kalender*

[Abbildung: Screenshot des Dialogs "Länder Kalender"]
*Abb. B-350: Kalender*

In diesem Dialog pflegen Sie die Feiertage in den Ländern und Provinzen, in denen die Unternehmen angesiedelt sind, mit denen Sie arbeiten.

**Identifikation**
*   **Provinz**: Auswahl der Provinz, für die der Feiertagskalender gilt. Die Provinzen sind unter **Marktpartner > Allgemein** hinterlegt.
    ⇨ "Provinz" auf Seite B-752
*   **Jahr**: Auswahl des Jahres, in dem die Feiertage gelten.
*   **Land**: Auswahl des Landes, zu dem die Provinz gehört. Die Länder sind unter **Stammdaten > Allgemein** hinterlegt.
    ⇨ "Landeskürzel" auf Seite B-559

**Tabelle**
In der Tabelle werden alle Kalender zu den Provinzen angezeigt, für die besondere Feiertage gelten.

### Basisnummernkreise

*Stammdaten > Allgemein > Basisnummernkreise*

[Abbildung: Screenshot des Dialogs "Basisnummernkreise"]
*Abb. B-351: Basisnummernkreise*

In diesem Dialog wird angezeigt, wie viele Datensätze Sie in der jeweiligen Stammdatentabelle anlegen können und wie viele Nummern bereits vergeben sind. Die Start- und Endnummern sind in der Regel fest vorgegeben und müssen nicht angepasst werden.

Diese Nummern können pro Datenbank (DB) gepflegt werden. D. h., dass sich die Nummernkreise der Master-DB und der Slave-DBs unterscheiden können. Diese Einstellungen werden nicht repliziert.

In den aufgeführten Stammdatendialogen ist die Anzahl der möglichen Datensätze auf die höchste Nummer begrenzt. Wenn weitere Datensätze angelegt werden sollen, müssen Sie die höchste Nummer erhöhen.

> **Nummernkreise für Dokumente**
> Nummernkreise für die Dokumente legen Sie im Programmbereich **Auftrag** fest.
> ⇨ "Nummernkreise" auf Seite B-891

**Übersicht**
*   **Tabelle**: Namen der Stammdatentabellen, zu denen Nummernkreise geführt werden.
*   **Letzte Nummer**: Nummer des Datensatzes, die in diesem Nummernkreis zuletzt vergeben wurde.
*   **Höchste Nummer**: Höchste Nummer, die in diesem Nummernkreis vergeben werden kann.

## Produkte

*Stammdaten > Produkte*

In diesem Programmbereich definieren Sie die allgemeinen Daten für die Verwaltung von Produkten und die Produktstammdaten.

Im Menü **Produkte** finden Sie folgende Einträge:
*   "Allgemein" auf Seite B-564
*   "Artikel" auf Seite B-637

### Allgemein

*Stammdaten > Produkte > Allgemein*

In diesem Programmbereich sind die allgemeinen Daten zu den Produkten hinterlegt.
Im Menü **Allgemein** finden Sie folgende Einträge:

*   "Produktarten" auf Seite B-565
*   "Produktgruppen" auf Seite B-566
*   "WGR" auf Seite B-567
*   "Kombi-WGR" auf Seite B-569
*   "Top-WGR" auf Seite B-571
*   "Varianten" auf Seite B-572
*   "Sprossentypen" auf Seite B-573
*   "Reklamationsverursacher" auf Seite B-575
*   "Reklamationsgrund" auf Seite B-576
*   "Struktur" auf Seite B-577
*   "Strukturseite" auf Seite B-578
*   "Beschichtungsseite" auf Seite B-579
*   "Beschichtungsart" auf Seite B-580
*   "Glasartgruppen" auf Seite B-581
*   "Gütetext" auf Seite B-582
*   "Leistungserklärung Verwaltung" auf Seite B-584
*   "Austauschgruppen" auf Seite B-585
*   "Austauschzuordnung" auf Seite B-586
*   "Klassifikatoren - Produkt" auf Seite B-587

### Produktarten

*Stammdaten > Produkte > Allgemein > Produktarten*

[Abbildung: Screenshot des Dialogs "Produktarten"]
*Abb. B-352: Produktarten*

In diesem Dialog werden die Produktarten angezeigt, die in A+W Business zur Verfügung stehen. Sie können diese nicht umbenennen oder ergänzen.
⇨ Tutorial 1, "Produktarten und Produktgruppen" auf Seite B-140

*   **Bezeichnung**: Name der Produktart.
*   **Schlüssel**: Schlüsselnummer (ID), mit der die Produktart im System eindeutig identifiziert wird.
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Produktion.
*   **Gesperrt**: Eine Produktart kann für die Erfassung in der Produktverwaltung und in den Dokumenten gesperrt werden, wenn sie nicht mehr benötigt wird.
    *   ☐ Die Produktart kann zugewiesen werden.
    *   ☑ Die Produktart ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie Produkten und in Dokumenten zugewiesen ist, wird sie jedoch weiterhin angezeigt.

> **Produktarten erweitern**
> Wenn Sie weitere Produktarten benötigen, sprechen Sie Ihren Service-Mitarbeiter bei der A+W Software GmbH an.

### Produktgruppen

*Stammdaten > Produkte > Allgemein > Produktgruppen*

[Abbildung: Screenshot des Dialogs "Produktgruppen"]
*Abb. B-353: Produktgruppen*

In diesem Dialog pflegen Sie die Produktgruppen, mit denen Sie in A+W Business arbeiten. Den Namen einer neuen Produktgruppe können Sie frei wählen. Anschließend ordnen Sie die Produktart zu.
⇨ Tutorial 1, "Produktarten und Produktgruppen" auf Seite B-140

*   **Produktart**: Produktart, die einer Produktgruppe zugeordnet ist.
*   **Bezeichnung**: Name der Produktgruppe.
*   **Schlüssel**: Schlüsselnummer, über die die Produktgruppe in System eindeutig identifiziert wird.
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Produktion.
*   **Schlüssel A+W Production**: Fremdschlüssel, der für den Datenaustausch mit A+W Production genutzt wird. Dieser Schlüssel muss auch in A+W Production bei der entsprechenden Produktgruppe hinterlegt sein.
*   **Gesperrt**: Eine Produktgruppe kann für die Erfassung in der Produktverwaltung und in den Dokumenten gesperrt werden, wenn sie nicht mehr benötigt wird.
    *   ☐ Die Produktgruppe kann zugewiesen werden.
    *   ☑ Die Produktgruppe ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie Produkten und in Dokumenten zugewiesen ist, wird sie jedoch weiterhin angezeigt.

### WGR

*Stammdaten > Produkte > Allgemein > WGR*

[Abbildung: Screenshot des Dialogs "Warengruppen (WGR)"]
*Abb. B-354: Warengruppen*

In diesem Dialog verwalten Sie die Warengruppen, mit denen Sie in A+W Business arbeiten. Die Warengruppen werden in drei Ebenen klassifiziert:
*   Warenhauptgruppe (WHG)
*   Warenobergruppe (WOG)
*   Warengruppe (WGR)

Die Abkürzung wird WGR auch für Warengruppen im Allgemeinen verwendet. Die WHG 0**, WOG 00* und WGR 000 sind fest angelegt.
Der Warengruppe 000 werden in der Regel nur Modelle zugeordnet. So kann in der Statistik z. B. der Modellumsatz automatisch dem Umsatz des Hauptproduktes zugeordnet werden.
Sprossen und Bearbeitungen haben in der Regel eine eigene Warengruppe.
⇨ Tutorial 1, "Warengruppen" auf Seite B-142

> **Kombi-Warengruppen**
> Wenn Sie mit Kombi-Warengruppen arbeiten möchten, müssen Sie diese wie jede andere WGR anlegen. Im Dialog Kombi-WGR können Sie dann die gewünschten Warengruppen kombinieren und zuordnen.
> ⇨ "Kombi-WGR" auf Seite B-569

#### Warengruppe

*   **Nummer**: Nummer der WGR. Sie können je nach Ebene bis zu 3 Stellen alphanumerisch angeben, z. B. 1АТ.
*   **Vorlauftage**: Vorlauftage für die Berechnung des Versandtags. Dies gilt nur für Bestellartikel. Der Wert gibt an, wie viele Tage ein Bestellartikel im Voraus beim Lieferanten bestellt werden muss, damit der Artikel rechtzeitig zur Produktion bereitsteht.
*   **Bezeichnung**: Eindeutiger Name der WGR.
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Produktion oder die Finanzbuchhaltung. Mit Hilfe eines Fremdschlüssels können Preise nach Warengruppen berechnet werden. Im Dialog zur Preisdefinition können Sie ihn für den Grenztyp **WGR Fremdkey** einsetzen.
    ⇨ "Preise" auf Seite B-714

> **Exakte Grenzmenge für WGR-Fremdkey**
> Um eine exakte Grenzmenge für den WGR-Fremdkey zu haben, steht die Grenzmenge **140 WGR Fremdkey exakt** zur Verfügung. Die entsprechende Funktion kann in den Firmendaten aktiviert werden.
> ⇨ "WGR-Fremdkey als nicht exakte Grenzmenge berechnen" auf Seite B-955

#### Kosten und Aufschlagskalkulation

*   **Sonderzuschlag**: Prozentualer Zuschlag für eine Warengruppe. Dieser Sonderzuschlag wird bei der Berechnung der Selbstkosten berücksichtigt und entsprechend ausgewiesen.
*   **Steuercode**: Zur Steuerberechnung können die Daten an den Avalara Web-Service übergeben werden. Für die korrekte Steuerberechnung müssen sogenannte Steuercodes zu jeder Warengruppe eingetragen werden. Während der Übergabe wird für jede Position der Steuercode anhand der Kombi-Warengruppe des Hauptproduktes ermittelt und an Avalara übergeben. Die Zugangsdaten müssen in den Firmendaten eingerichtet werden.
    ⇨ "Firmendaten - Steuer" auf Seite B-921
*   **Bitmap**: Piktogramme, die einer WGR zugeordnet werden können. So können Sie die Produktart oder -gruppe schnell erkennen.
*   **Top-Warengruppen**: Top-Warengruppen aus dem Dialog Top-WGR. Sie können eine Warengruppe nur auf Warengruppenebene (WGR), nicht auf Warenhaupt- oder Warenobergruppenebene einer Top-Warengruppe zuordnen.
    *   ☐ Die Warengruppe ist nicht zugeordnet.
    *   ☑ Die Warengruppe ist der Top-WGR zugeordnet.
    ⇨ Tutorial 1, "Top-WGR" auf Seite B-149
    ⇨ "Top-WGR" auf Seite B-571

### Kombi-WGR

*Stammdaten > Produkte > Allgemein > Kombi-WGR*

[Abbildung: Screenshot des Dialogs "Kombi-WGR"]
*Abb. B-355: WGR-Kombinationen*

In diesem Dialog legen Sie Kombi-Warengruppen (Kombi-WGR) an. Wenn Sie in der Übersicht eine Zeile markieren, werden die entsprechenden Werte in den Feldern angezeigt und können bearbeitet werden.
⇨ Tutorial 1, "Regeln für Kombi-WGR" auf Seite B-144
⇨ Tutorial 1, "Warengruppen kombinieren" auf Seite B-152

**Ausgangswarengruppen**
*   **Warengruppe 1, 2**: Erste und zweite Warengruppe, die miteinander kombiniert sind. Hier sind alle Warengruppenebenen erlaubt.

**Kombinationswarengruppen**
*   **Warengruppe**: Kombi-WGR, nach deren Regeln die Warengruppe 1 und Warengruppe 2 kombiniert werden sollen. Die möglichen Kombi-WGR müssen im Dialog WGR angelegt sein.
    ⇨ "WGR" auf Seite B-567
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für statistische Auswertungen.
*   **Gültig für Rabattfindung**: Sie können angeben, ob die Kombi-WGR bei der Berechnung des Rabattes berücksichtigt werden soll.
    *   ☐ Die Kombi-WGR wird nicht bei der Berechnung des Preises berücksichtigt.
    *   ☑ Die Kombi-WGR wird bei der Preis- und Rabattfindung berücksichtigt. Die Checkbox **Kombi-Rabatt nur auf Hauptposition bilden** wird freigeschaltet.
*   **Gültig für Statistik**: Sie können angeben, ob die Kombi-WGR in der Statistik berücksichtigt werden soll.
    *   ☐ Die Kombi-WGR wird nicht in der Statistik berücksichtigt.
    *   ☑ Die Kombi-WGR wird in der Statistik berücksichtigt. Die Checkbox **Kombi-Statistik nur auf Hauptposition bilden** wird freigeschaltet.
*   **Kombi-Rabatt nur auf Hauptposition bilden**: Diese Checkbox ist nur freigeschaltet, wenn die Checkbox **Gültig für Rabattfindung** aktiviert wurde.
    *   ☐ Der gesamte Umsatz des Floats und der Bearbeitung wird zur Rabattfindung herangezogen.
    *   ☑ Nur die Hauptposition wird zur Rabattfindung herangezogen.

**Beispiel Kombiwarengruppe: 100 + 400 = 401**

| Produkt | WGR | Ergebnis Kombi-WGR ☐ | Ergebnis Kombi-WGR ☑ |
| :--- | :--- | :--- | :--- |
| Float | 100 | 401 | 401 |
| Bearbeitung | 400 | 401 | 400 |

*   **Kombi-Statistik nur auf Hauptposition bilden**: Diese Checkbox ist nur freigeschaltet, wenn die Checkbox **Gültig für Statistik** aktiviert wurde.
    *   ☐ Der gesamte Umsatz des Floats und der Bearbeitung wird auf die Kombi-Warengruppe gebucht.
    *   ☑ Sie können in der Auswertung unterscheiden, wie viel Float mit und ohne Bearbeitung produziert wurde. Der Umsatz für die Bearbeitung selbst wird jedoch separat verbucht.

**Übersicht**
In der Übersicht werden die angelegten Kombi-WGR aufgelistet.

### Top-WGR

*Stammdaten > Produkte > Allgemein > Top-WGR*

[Abbildung: Screenshot des Dialogs "Top-WGR"]
*Abb. B-356: Top-Warengruppen*

In diesem Dialog legen Sie Top-Warengruppen (Top-WGR) an. In der Umsatzstatistik können Sie Auswertungen für diese Top-Warengruppen erstellen.

*   **Bezeichnung**: Name der Top-Warengruppe. Im Dialog WGR können Sie die gewünschte Warengruppe zuordnen. ⇨ "WGR" auf Seite B-567
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für statistische Auswertungen.

### Varianten

*Stammdaten > Produkte > Allgemein > Varianten*

[Abbildung: Screenshot des Dialogs "Varianten" (Farben)]
*Abb. B-357: Farben für Produkt-Varianten*

In diesem Dialog hinterlegen Sie die Farben, die Sie für die Definition von Produktvarianten verwenden können.
⇨ "Produktvarianten" auf Seite B-643

*   **Sprache**: Auswahl der Sprache, wenn Sie mit der Mehrsprachigkeit arbeiten. Verwenden Sie in allen Sprachen dieselben Schlüssel. Die Bezeichnung kann übersetzt werden.
*   **Variante**: Interne Nummer der Farbe. Diese Nummer benötigen Sie für die Zuordnung der Farbe zur Produktvariante.
*   **Bezeichnung**: Name der Farbe.
*   **Fremdschlüssel**: Bei Dorma-Artikeln der Dorma-Farbschlüssel. Der Fremdschlüssel kann für die Kommunikation mit anderen Programmen verwendet werden, z. B. für die Übergabe an die Produktion.
*   **Farbauswahl**: Öffnet den Dialog **Farbe**, um die Farbe festzulegen, in der z. B. die Sprossen in der Positionserfassung angezeigt werden. Die Farbe wird nicht an die Produktion übergeben.
*   **Vorschau**: Anzeige der gewählten Farbe.
*   **Sonderfarbe**: Im Auftrag kann bei bestimmten Produkten eine Sonderfarbe verwendet werden, z. B. beim Siebdruck.
    *   ☐ Die Farbe wird nicht als Sonderfarbe verwendet.
    *   ☑ Bei dieser Einstellung kann im Auftrag angegeben werden, welche Farbe verwendet werden soll.

    **Beispiel**
    In einem Auftrag soll für einen Kunden ein Siebdruck mit einem bestimmten Motiv erfasst werden, z. B. ein Formel 1-Fahrzeug.
    Für diesen Fall muss eine Variante mit dem Kennzeichen **Sonderfarbe** für das Produkt **Siebdruck** angelegt sein. In der Positionserfassung wählen Sie dann für die Bearbeitung Siebdruck diese Produktvariante aus. Dadurch wird ein weiteres Feld angezeigt, in dem Sie den Namen des Motivs angegeben können. Dieser Name wird an die Produktion übergeben.

*   **Gesperrt**: Eine Variante kann für die Erfassung in der Produktverwaltung und in den Dokumenten gesperrt werden, wenn sie nicht mehr benötigt wird.
    *   ☐ Die Variante kann zugewiesen werden.
    *   ☑ Die Variante ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie Produkten und in Dokumenten zugewiesen ist, wird sie jedoch weiterhin angezeigt.

### Sprossentypen

*Stammdaten > Produkte > Allgemein > Sprossentypen*

[Abbildung: Screenshot des Dialogs "Sprossentypen"]
*Abb. B-358: Sprossentypen*

In diesem Dialog definieren Sie die Sprossentypen. Jeder Sprosse wird in der Produktverwaltung ein Sprossentyp zugeordnet.
⇨ "Konstruktionstyp" auf Seite B-599

> **Neue Sprossentypen**
> Wenn Sie mit A+W Production arbeiten, müssen Sie neue Sprossentypen mit Ihrem Service-Mitarbeiter der A+W Software GmbH absprechen.

*   **Typ**: Interne Nummer. Diese Nummer muss mit der Nummer in der Produktionssoftware übereinstimmen.
*   **Bezeichnung**: Name des Sprossentyps.
*   **Randstopfenmaß**: Wert für das Randstopfenmaß in mm. Das Randstopfenmaß wird bei der Preisberechnung der Sprossenkonstruktion ausgewertet.
    ⇨ Verkauf, "Gitter" auf Seite C-499
*   **Kennz. Durchgang**: Angabe zur Verbindung mit anderen Sprossen:
    *   **0 - keine**: Das Kennzeichen ist nicht gesetzt, Sprossen des Typs können beliebig verarbeitet werden.
    *   **1 - waagerecht**: Waagerechte Sprossen des Typs müssen durchgängig sein.
    *   **2 - senkrecht**: Senkrechte Sprossen des Typs müssen durchgängig sein.
    *   **3 - waagerecht + senkrecht**: Waagerechte und senkrechte Sprossen des Typs müssen durchgängig sein.
    *   **6 - überlappend**: Waagerechte und senkrechte Sprossen des Typs können sich überlappen.
    *   **7 - längste Sprosse**: Die längste Sprosse des Typs muss durchgängig sein.
    ⇨ Tutorial 1, "Konstruktionstypen der Sprossen" auf Seite B-162
*   **Frästiefe**: Tiefe des Einschnitts im Abstandhalter.
*   **Spezialkreuzung**: Bei einigen Sprossentypen sind Spezialkreuze für die Verbindung erforderlich.
    *   ☐ Für den Sprossentyp wird kein Spezialkreuz verwendet.
    *   ☑ Für den Sprossentyp muss ein Spezialkreuz verwendet werden. Zusätzlich muss die Breite angegeben werden. Bei dieser Einstellung müssen das Kennzeichen für den Durchgang und die Fräßtiefe auf 0 (keine) stehen.
*   **Breite Spezialkreuz, 0=Sprossenbreite**: Breite des Spezialkreuzes im mm. Der Wert 0 zeigt an, dass die Breite des Spezialkreuzes sich nach der Sprossenbreite richtet.

### Reklamationsverursacher

*Stammdaten > Produkte > Allgemein > Reklamationsverursacher*

[Abbildung: Screenshot des Dialogs "Reklamationsverursacher"]
*Abb. B-359: Reklamationsverursacher*

In diesem Dialog hinterlegen Sie die Verursacher einer Reklamation. Die Werte können beim Erfassen einer Reklamation ausgewählt werden. Sie werden durch das Modul **Reklamationsstatistik** ausgewertet.

*   **Bezeichnung**: Name des Verursachers, z. B. Produktion, Auftragserfassung, Versand. Die Bezeichnung soll sich deutlich vom Reklamationsgrund unterscheiden.
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Finanzbuchhaltung oder für statistische Auswertungen.
*   **Gesperrt**: Ein Reklamationsverursacher kann für die Erfassung in den Dokumenten gesperrt werden, wenn er nicht mehr benötigt wird.
    *   ☐ Der Reklamationsverursacher kann zugewiesen werden.
    *   ☑ Der Reklamationsverursacher ist gesperrt und kann nicht mehr zugewiesen werden. Wenn er in Dokumenten zugewiesen ist, wird er jedoch weiterhin angezeigt.

### Reklamationsgrund

*Stammdaten > Produkte > Allgemein > Reklamationsgrund*

[Abbildung: Screenshot des Dialogs "Reklamationsgrund"]
*Abb. B-360: Reklamationsgrund*

In diesem Dialog hinterlegen Sie Gründe, die zu einer Reklamation geführt haben.

*   **Bezeichnung**: Name für den Reklamationsgrund, z. B. Materialfehler, Produktionsfehler, Bruch.
*   **Kombi-WGR**: Kombi-WGR für die Auswertung. Über Kombi-WGR können die Stückzahlen ausgewertet werden, die aufgrund von Reklamationen produziert wurden. In der Reklamationsstatistik im Modul **Statistik** wird auch der entgangene Umsatz ausgewertet.
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Finanzbuchhaltung oder für statistische Auswertungen.
*   **Gesperrt**: Ein Reklamationsgrund kann für die Erfassung in den Dokumenten gesperrt werden, wenn er nicht mehr benötigt wird.
    *   ☐ Der Reklamationsgrund kann zugewiesen werden.
    *   ☑ Der Reklamationsgrund ist gesperrt und kann nicht mehr zugewiesen werden. Wenn er in Dokumenten zugewiesen ist, wird er jedoch weiterhin angezeigt.

### Struktur

*Stammdaten > Produkte > Allgemein > Struktur*

[Abbildung: Screenshot des Dialogs "Struktur"]
*Abb. B-361: Struktur*

In diesem Dialog werden die möglichen Strukturverläufe der Gläser angezeigt. Sie können die Einträge bearbeiten, jedoch nicht um weitere Verläufe ergänzen.

*   **Schlüssel**: Der Schlüssel (ID) ist von A+W Business vorgegeben und darf nicht verändert werden.
*   **Kurzbez.**: Einstellige alphanumerische Kurzbezeichnung, die geändert werden kann.

    **Beispiel**
    S = senkrecht oder V = vertikal
    W = waagrecht oder H = horizontal

*   **Bezeichnung**: Eindeutiger Name für den Strukturverlauf.

### Strukturseite

*Stammdaten > Produkte > Allgemein > Strukturseite*

[Abbildung: Screenshot des Dialogs "Strukturseite"]
*Abb. B-362: Strukturseite*

In diesem Dialog werden die möglichen Strukturseiten angezeigt. Sie können die Einträge bearbeiten und ergänzen, um bei Mehrfach-ISO oder VSG alle Seiten angeben zu können. Dabei hat jede Scheibe im ISO oder VSG zwei Seiten, die jeweils innen oder außen liegen.
⇨ Tutorial 1, "Strukturen und Beschichtungen" auf Seite B-160

*   **Ebene**: Die Nummern der Ebenen (Seiten im ISO-Aufbau) dürfen nicht verändert werden. Wenn Sie weitere Ebenen anlegen, wählen Sie fortlaufenden Nummern nach demselben Prinzip.
*   **Kurzbez.**: Einstellige alphanumerische Kurzbezeichnung für die Innen- und die Außenseite. Sie können sie ändern.
*   **Bezeichnung**: Eindeutiger Name der Ebene.

### Beschichtungsseite

*Stammdaten > Produkte > Allgemein > Beschichtungsseite*

[Abbildung: Screenshot des Dialogs "Beschichtungsseite"]
*Abb. B-363: Beschichtungsseite*

In diesem Dialog werden die möglichen Beschichtungsseiten angezeigt. Sie können die Einträge bearbeiten und ergänzen, um bei mehrfach ISO alle Ebenen angeben zu können. Dabei hat jede Scheibe im ISO zwei Seiten, die jeweils innen oder außen liegen.
⇨Tutorial 1, "Strukturen und Beschichtungen" auf Seite B-160

*   **Ebene**: Die Nummern der Ebenen dürfen nicht verändert werden. Wenn Sie weitere Ebenen anlegen, wählen Sie fortlaufende Nummern nach demselben Prinzip.
*   **Kurzbez.**: Einstellige alphanumerische Kurzbezeichnung für die Innen- und die Außenseite. Sie können sie ändern.
*   **Bezeichnung**: Eindeutiger Name der Ebene.

### Beschichtungsart

*Stammdaten > Produkte > Allgemein > Beschichtungsart*

[Abbildung: Screenshot des Dialogs "Beschichtungsart"]
*Abb. B-364: Beschichtungsart*

In diesem Dialog werden die möglichen Beschichtungsarten angezeigt. Sie können die Einträge bearbeiten und ergänzen.
⇨Tutorial 1, "Strukturen und Beschichtungen" auf Seite B-160

*   **Schlüssel**: Der Schlüssel ist von A+W Business vorgegeben und darf nicht verändert werden.
*   **Kurzbez.**: Einstellige alphanumerische Kurzbezeichnung.

    **Beispiel**
    N = nicht beschichtet oder O = ohne

*   **Bezeichnung**: Eindeutiger Name der Beschichtungsart.

### Glasartgruppen

*Stammdaten > Produkte > Allgemein > Glasartgruppen*

[Abbildung: Screenshot des Dialogs "Glasartgruppen"]
*Abb. B-365: Glasartgruppen*

In diesem Dialog hinterlegen Sie die Glasartgruppen. Glasartgruppen benötigen Sie, wenn Sie mit A+W Production arbeiten. Die Glasartgruppen von A+W Production entsprechen den Produktarten von A+W Business.

**Beispiel**
1 = Float
2 = Isolierglas
3 = ...

Jedem Glasprodukt kann in der Produktverwaltung über das Register A+W Production eine Glasart und eine Glasartgruppe zugeordnet werden. Die Definition von Glasartgruppen dient in A+W Production zur Auswertung in Reports und in der Statistik. Für den Produktionslauf haben die Glasartgruppen keine Bedeutung.
⇨ "Glasarten" auf Seite B-635

*   **Bezeichnung**: Name der Glasartgruppe, z. B. Float, ESG, VSG.
*   **Schlüssel**: 1- bis 7-stellige Nummer der Glasartgruppe.

### Gütetext

*Stammdaten > Produkte > Allgemein > Gütetext*

Gütetexte werden abhängig vom ISO-Aufbau und Landeskennzeichen der Lieferadresse in den Rahmentext eingefügt.

> **Voraussetzung**
> Der Dialog kann nur geöffnet werden, wenn in den **Firmendaten > Register Dokumente** die entsprechende Funktion ausgewählt ist.
> ⇨ "Produktkennzeichnung" auf Seite B-934

Im Dialog **Gütetext** finden Sie folgende Register:
*   Gütetext – Grundeinstellungen
*   Gütetext – Restriktionen

#### Gütetext – Grundeinstellungen

*Stammdaten > Produkte > Allgemein > Gütetext > Register Grundeinstellungen*

[Abbildung: Screenshot des Dialogs "Gütetext - Grundeinstellungen"]
*Abb. B-366: Gütetext - Grundeinstellung*

In diesem Register hinterlegen Sie die (landesspezifischen) Gütetexte, die in die Rahmentexte eingefügt werden sollen.
⇨Tutorial 2, "Textarten" auf Seite B-462

**Produktauswahl**
*   **Glas**: Glasartikel, für den ein Gütetext definiert ist.
*   **Gas**: Gas in der ISO-Scheibe.

**Werte**
*   **Priorität**: Über die Priorität legen Sie fest, welcher Gütetext genommen wird, falls in einer ISO-Einheit unterschiedliche Gläser enthalten sind, für die jeweils ein Gütetext erfasst ist.
*   **Land**: Die Gütetextanforderungen können sich von Land zu Land unterscheiden. Mit Hilfe des Landeskennzeichens können Sie für ein Glas unterschiedliche Texte pro Land definieren.
*   **Text**: Gütetext, der in den Rahmen gedruckt wird.

#### Gütetext – Restriktionen

*Stammdaten > Produkte > Allgemein > Gütetext > Register Restriktionen*

[Abbildung: Screenshot des Dialogs "Gütetext - Restriktionen"]
*Abb. B-367: Gütetext - Restriktionen*

In diesem Register können Sie die automatische Verwendung des Gütetextes einschränken. Über eine Regel legen Sie fest, bei welchen Produktarten oder Produktgruppen der Gütetext nicht verwendet wird.
Die Felder im Bereiche **Produktauswahl** sind zum Register Grundeinstellungen beschrieben.
⇨ "Gütetext - Grundeinstellungen" auf Seite B-582

**Gültigkeitsbereich**
*   **Regel**: Die verfügbaren Regeln sind vom Programm vorgegeben.
*   **Parameter 1 - 4**: Die Anzahl der änderbaren Parameter hängt von der ausgewählten Regel ab.

**Restriktionen**
In der Übersicht werden für das ausgewählte Glas alle Regeln mit den zugehörigen Parametern aufgelistet.

### Leistungserklärung Verwaltung

*Stammdaten > Produkte > Allgemein > Leistungserklärung Verwaltung*

[Abbildung: Screenshot des Dialogs "Leistungserklärung Verwaltung"]
*Abb. B-368: Leistungserklärung Verwaltung*

In diesem Dialog verwalten Sie die Vorlagen für die Leistungserklärungen. Mit der Kombination von Nummer, Bezeichnung und Sprache haben Sie die Möglichkeit, eine Leistungserklärung in verschiedenen Sprachen mit derselben Nummer zu registrieren.
Zur Erstellung von Leistungserklärungen können die technischen Text in allen erforderlichen Sprachen hinterlegt werden.
⇨ "Technische Werte" auf Seite B-1049

Der Versand von Leistungserklärungen kann pro Kunde und Produkt aktiviert werden.

**Leistungserklärung**
*   **Nummer**: Nummer der Leistungserklärung.
*   **Bezeichnung**: Name der Leistungserklärung. Er sollte eindeutig und sprechend sein.

**Dateianhang**
*   **Sprache**: Sprache, in der die Leistungserklärung abgefasst ist.
*   **Link**: Pfad, in dem die Leistungserklärungen abgelegt sind. Standardmäßig liegen die Leistungserklärungen in demselben Verzeichnis, in dem die Dateianhänge abgelegt sind. Dieses Verzeichnis legen Sie in den Firmendaten fest.
    ⇨ "Dateianhänge" auf Seite B-934
*   **[Hinzufügen], [Entfernen]**: Über diese Schaltflächen stellen Sie eine sprachliche Version der Leistungserklärungen zur Verfügung oder entfernen sie aus der Auswahl.

**Übersicht**
In der Übersicht sind alle Leistungserklärungen aufgeführt, die den Produkten oder Kunden zugeordnet werden können.

### Austauschgruppen

*Stammdaten > Produkte > Allgemein > Austauschgruppen*

[Abbildung: Screenshot des Dialogs "Austauschgruppen"]
*Abb. B-369: Austauschgruppen*

In diesem Dialog legen Sie die Austauschgruppen fest. Diesen Gruppen müssen Sie die Produkte zuordnen, die für den Austausch zugelassen sind.
⇨ "Austauschzuordnung" auf Seite B-586

Mit diesen Definitionen legen Sie fest, dass in ISO und/oder VSG nur Gläser, Abstandhalter und Folien eingebaut werden können, die für diese Produkte vorgesehen oder geeignet sind.
Die Funktion müssen Sie in den Firmendaten aktivieren.
⇨ "Produktaustauschregeln für Stücklistenaustausch verwenden" auf Seite B-945

In den Stammdaten der Produkte mit Stückliste müssen Sie die gültige Gruppe angeben:
⇨ "Produktverwaltung – Stückliste" auf Seite B-616

*   **Nummer**: Nummer der Austauschgruppe.
*   **Bezeichnung**: Bezeichnung der Austauschgruppe.

### Austauschzuordnung

*Stammdaten > Produkte > Allgemein > Austauschzuordnung*

[Abbildung: Screenshot des Dialogs "Austauschzuordnung"]
*Abb. B-370: Zuordnung der Produkte zu Austauschgruppen*

In diesem Dialog ordnen Sie die Produkte einer Austauschgruppe zu. Damit legen Sie fest, welche Produkte für den Austausch verwendet werden dürfen.
In den Stammdaten der Produkte mit Stückliste können Sie die Gruppe mit den zulässigen Produkten angeben.
⇨ "Produktverwaltung - Stückliste" auf Seite B-616

Mit diesen Definitionen legen Sie fest, dass in ISO und/oder VSG nur Gläser, Abstandhalter und Folien eingebaut werden können, die für diese Produkte vorgesehen oder geeignet sind.
Die Funktion müssen Sie in den Firmendaten aktivieren.
⇨ "Produktaustauschregeln für Stücklistenaustausch verwenden" auf Seite B-945

**Neuanlage**
*   **Gruppe**: Bezeichnung der Austauschgruppe. Das Feld ist nur freigeschaltet, wenn Sie einer Gruppe ein Produkt zuordnen. Neue Austauschgruppen legen Sie im Dialog **Austauschgruppen** an.
    ⇨ "Austauschgruppen" auf Seite B-585
*   **Produkt**: Produkt, das der Austauschgruppe zugeordnet ist.

**Produktzuordnung**
In der Übersicht werden alle Zuordnungen angezeigt. Um eine Zuordnung zu ändern, müssen Sie die ungültige Zuordnung löschen und eine neue anlegen.

### Klassifikatoren – Produkt

*Stammdaten > Produkte > Allgemein > Klassifikatoren > Produkte*
*Stammdaten > Marktpartner > Allgemein > Klassifikatoren > Produkte*

[Abbildung: Screenshot des Dialogs "Klassifikatoren - Produkte"]
*Abb. B-371: Klassifikatoren - Produkte*

In diesem Register hinterlegen Sie Bezeichnungen für Produkt-Klassifikatoren. Der Dialog ist ausführlich zu Markpartnern beschrieben.
⇨ "Klassifikatoren" auf Seite B-753

Neben der Bezeichnung und einer Bemerkung müssen Sie zu jedem Klassifikator festlegen, welcher Wert ihm zugewiesen werden kann.
⇨ "Produktverwaltung – Anlagen/Klassifikatoren" auf Seite B-625

## Verfügbare Dokumententypen

Folgende Dokumententypen können unterschieden werden:

| Typ | Beschreibung |
| :--- | :--- |
| **Anzahlung** | Dieser Dokumententyp wird automatisch bei einer Anzahlung gesetzt. |
| **Eigenfertigung** | Dieser Dokumententyp wird bei der Erfassung eines Auftrages (Produktionsauftrag) gesetzt. |
| **Forderung** | Dieser Dokumententyp wird automatisch bei der Erstellung von Forderungsrechnungen gesetzt. Modul Objektabrechnungsverwaltung. |
| **Interne Verrechnung** | Dieser Dokumententyp wird automatisch bei der Bestellübergabe gesetzt. Modul Profit-Center-Verrechnung. |
| **Interner Auftrag** | Dieser Dokumententyp wird automatisch bei der Bestellübergabe gesetzt. Modul Interne Aufträge (mehrstufige Produktion). |
| **Kundenmaterial** | Dieses Kennzeichen muss manuell gesetzt werden. Es hat zur Folge, dass alle Positionen automatisch auf die Beschaffungsart **Kundeneigenes Glas** gesetzt werden. |
| **Lagerbestellung** | Dieser Dokumententyp wird bei der Lagerbestellung gesetzt. Dieses Kennzeichen kann aber auch manuell in einem Bestellauftrag gesetzt werden. |
| **Reklamation** | Der Dokumententyp wird automatisch bei der Reklamationserfassung gesetzt. Dieses Kennzeichen kann aber auch manuell im Auftrag gesetzt werden. |
| **Teillieferung** | Dieser Dokumententyp wird automatisch bei der Erstellung von Teillieferaufträgen gesetzt. |
| **Wertmäßige Buchung** | Dieser Dokumententyp wird automatisch während der Gutschriftenerfassung gesetzt. Mengenwerte wie Stück, Quadratmeter und Laufmeter werden dadurch nicht an die Statistik übergeben. |

*Tab. B-24: Dokumententypen*
⇨ Softwarereferenz, "Firmendaten - Archiv" auf Seite B-965

## Verfügbare Grenztypen

Die Grenztypen sind fest hinterlegt und können nicht bearbeitet werden. Wenn Sie weitere Grenztypen benötigen, wenden Sie sich bitte an die A+W Software GmbH.

| Grenztyp | Beschreibung | Beispiel |
| :--- | :--- | :--- |
| 1 x Breite+Höhe | Addition von Breite und Höhe. | 600 + 800 = 1400 mm |
| Anzahl Felder | Nur bei Sprossen. | |
| Anzahl Kreuze | Nur bei Sprossen. | |
| Bearbeitungsindex | Bis-Angabe. ⇨ "Bearbeitungsindex" auf Seite B-252 | Bis einschließlich 100. Dieser Wert wird mit Bezug auf die Glasdicke und die Produktart festgelegt. |
| Bearbeitungsindex exakt | Genauer Wert. | 101 für Türen. |
| Breite | Bis-Wert der Breite. | Bis 1800 mm eines Glases. |
| Breite (Bearb.) | Höchstwert für Bearbeitungen (Länge der Bearbeitung). | 450 mm bei Randausschnitte. |
| Breite exakt | Genauer Wert. | 1200 mm für Türen. |
| Breite/Höhe | Seitenverhältnis von Breite zu Höhe. | 1:2 |
| Dicke | Auf Ebene der Hauptposition: Dicke der Position. Auf der Stücklistenebene wird das übergeordnete Glas gesucht: Wenn ein übergeordnetes Glas gefunden wird: Dicke des Glases. Falls kein übergeordnetes Glas gefunden wird: Dicke der Position. | |
| Dicke (additiv nur Glas) | Dicke aller Gläser der Stückliste. | Hauptposition VSG + Stücklisten-Komponente 1 Float = 4 mm + Folie 0,75 + Stücklisten-Komponente 2 Float = 4 mm = Gesamtdicke aller Gläser = 8 mm |
| Dicke (nur Glas) | Dicke des einzelnen Stücklistenglases. | 26 mm |
| Dicke (Stückliste) | Auf Ebene der Hauptposition: Gesamtdicke der Position. Auf Stücklistenebene: Dicke der Stücklisten-Komponente. | Folie, Glas (bei Stücklisten-Komponente) |
| Dicke (Vaterprodukt) | Auf Ebene der Hauptposition: Gesamtdicke der Position. Auf Stücklistenebene: Dicke des Vaterprodukts. | ISO - ESG - Bearbeitung. In diesem Fall wäre das Vaterprodukt das ESG. |
| Durchmesser | Durchmesser der Lochbohrung. | 12 mm |
| Einbauposition | Glaspreis nach Einbauposition gestaffelt. | **Beispiel 1: Hauptposition ISO**<br>• Einbauposition 1: Float<br>• Einbauposition 2: SZR<br>• Einbauposition 3: ESG<br>• Einbauposition 4: SZR<br>• Einbauposition 5: Float<br>**Beispiel 2: Hauptposition ISO**<br>• Einbauposition 1: VSG<br>  - Einbauposition 1: Float<br>  - Einbauposition 2: Folie<br>  - Einbauposition 3: Float<br>• Einbauposition 2: SZR<br>• Einbauposition 3: ESG |
| Entfernung | Zuschlagsberechnung der Transport-/Mautkosten pro Kilometer. | 130 km |
| Hauptprodukt-Nr. | Produktnummer der Hauptposition. | |
| Höhe | Bis-Wert der Höhe. | Bis 5800 mm eines Glases. |
| Höhe (Bearb.) | Bis-Wert für Bearbeitungen (Länge der Bearbeitung). | 950 mm bei Randausschnitte. |
| Höhe exakt | Genauer Wert. | 2100 mm für Türen. |
| Kanten-Bearbeitungsgröße | Bearbeitungen wie Facetten und Gehrung. Bei Facetten = Facettenbreite. | |
| Kantenlänge (größte), Kantenlänge (kleinste) | Bis-Angabe auf der Ebene der Hauptposition. | Zuschlag von Transport-/Mautkosten. |
| kg/lbs | Gewicht der Einheit. | Zuschlag von Transport-/Mautkosten. |
| kg/lbs pro Pos | Gesamtgewicht der Position. | |
| Laufmeter | Laufmeter der Einheit. | Sprossen. |
| Laufmeter (Bearb.) | Laufmeter der Bearbeitung. | Kanten polieren. |
| Lfm (gerundet) | Gerundete Laufmeter. ⇨ "Maßberechnung" auf Seite B-150 | |
| Lfm Auftrag Produkt, Lfm Auftrag WGR, Lfm Auftrag WHG, Lfm Auftrag WOG | Gesamte Laufmeter eines Produkts oder einer Warengruppe innerhalb eines Auftrags. | • Beispiel Produkt:<br>  Position 1: Produkt 1001 = 5 lfm<br>  Position 2: Produkt 1001 = 10 lfm<br>  Position 3: Produkt 1002 = 5 lfm<br>• Grenzmenge:<br>  bis 10 lfm = 5 Euro/lfm,<br>  bis 99 lfm = 4 Euro/lfm<br>• Laufmeter insgesamt pro Auftrag<br>  Produkt 1001 = 15 lfm = 4 Euro/lfm<br>  Produkt 1002 = 5 lfm = 5 Euro/lfm |
| Lfm Position | Gesamtlaufmeter der Position | |
| Nettowert (Liefertag) | Gesamtauftragswert eines Kunden pro Liefertag. | Modul Anlieferpauschale: Die Anlieferpauschale wird bei der Rechnungsstellung ermittelt. |
| Produktart/-gruppe | Die Produktart/-gruppe eines Glases auf Ebene der Hauptposition oder Stückliste. | Glas, Beschichtung. |
| Qm | Quadratmeter der Position. | Glas, Beschichtung. |
| Qm (gerundet) | Gerundete Quadratmeter. | Glas |
| Qm (Liefertag) | Gesamtquadratmeter eines Kundenauftrags pro Liefertag. | Modul Anlieferpauschale: Die Anlieferpauschale wird bei der Rechnungsstellung ermittelt. |
| Qm Auftrag Produkt, Qm Auftrag WGR, Qm Auftrag WHG, Qm Auftrag WOG | Siehe Lfm Auftrag Produkt. | |
| Qm Position | Gesamtquadratmeter der Hauptposition. | Glas, Beschichtung |
| Qm Position (gerundet) | Gerundete Quadratmeter der Hauptposition. | Glas |
| Qm Rechteck | Umschriebenes Rechteck (bei Modellen). | Grenztyp für die Preisberechnung ohne Bedeutung. |
| Radius Rundecke (Bearb.) | Radius von Rundecken. | |
| Sprossen | | Grenztyp für die Preisberechnung ohne Bedeutung. |
| Stk Auftrag Produkt, Stk Auftrag WGR, Stk Auftrag WHG, Stk Auftrag WOG | Siehe Lfm Auftrag Produkt. | |
| Stk Position | Gesamtmenge der Position. | |
| Stück | Menge der Position. | |
| Stück (Bearb.) | Menge der Bearbeitungen. | |
| SZR | Dicke des SZRs. | |
| SZR (größter) | Größter SZR innerhalb einer ISO-Einheit. | |
| WGR Fremdkey, WGR Fremdkey exakt | Mit Hilfe des Fremdschlüssels können Preise nach Warengruppen berechnet werden. | Beispiel: Bearbeitungen für ESG und VSG. |
| Zuschlagsnettobasis | Energiezuschlag in Prozent für Gläser. Basis für den Energiezuschlag ist die Summe der Nettopreise aller Gläser innerhalb eines Auftrages. Der Zuschlag wird automatisch als Auftragsposition 900 eingefügt. | Beispiel: bis zu 1000,00 = 5% Zuschlag, ab 1000,00 = 2% Zuschlag |

*Tab. B-25: Grenztypen für die Preisdefinition*

## Verfügbare Systemtexte

| Nr. | Text | Anmerkung |
| :-- | :--- | :--- |
| 1 | Modell | |
| 2 | ;unten:;rechts:;oben:;links:;Scheibe;S | Vermaßung der Stufe |
| 3 | Glas wird mitgeliefert! | |
| 50 | Rechnung `<ar>` v. `<ard>` f. Anzahlung v. `<ad>` | Anzahlungen |
| 51 | Anzahlung v. `<ad>` für Auftr. `<aa>` vom `<aad>` | Anzahlungen |
| 100 | Abrechnungssumme original %X1 | Nr. 100 bis 108: Objektverwaltung DMS |
| 101 | Vorherige Veränderungen %X2 | |
| 102 | Veränderungen mit dieser Rechnung %X3 | |
| 103 | Gesamtveränderung %X4 | |
| 104 | Abrechnungssumme neu %X5 | |
| 105 | - Nicht fertige Arbeiten %X6 | |
| 106 | Wert der kompletten Arbeit %X7 | |
| 107 | - Vorherige Forderungsrechnung %X8 | |
| 108 | HEUTIGE FORDERUNG NR.%X9 %X10 | |
| 110 | Ug-Wert in W/qm | Techn. ISO-Parameter |
| 111 | Ug-Wert nach DIN 4108-4 | Techn. ISO-Parameter |
| 112 | Lichtdurchl. in % | Techn. ISO-Parameter |
| 113 | g-Wert in % | Techn. ISO-Parameter |
| 114 | b-Faktor | Techn. ISO-Parameter |
| 115 | Schalldämmmaß in dB | Techn. ISO-Parameter |
| 116 | Dickentoleranz in mm | Techn. ISO-Parameter |
| 117 | Größentoleranz mm (<200 cm) | Techn. ISO-Parameter |
| 118 | Größentoleranz mm (>=200 cm) | Techn. ISO-Parameter |
| 119 | Sprossen im SZR, einfach | Versicherungspreisliste |
| 120 | Sprossen im SZR, mehrfach | Versicherungspreisliste |

*Tab. B-26: Systemtexte*
⇨ Softwarereferenz, "Systemtexte" auf Seite B-1046
⇨ Tutorial 2, "Texte anlegen" auf Seite B-470

## Verfügbare Variablen (Platzhalter)

In Texten können Variablen eingefügt werden, die erst im Dokument gefüllt werden.

**Formel**
`<@Formelnummer@>` = Ausführung einer Formel mit der Nummer (nn)

### Allgemein

| Bereich | Variable | Bedeutung |
| :--- | :--- | :--- |
| Allgemein | %X1, %X2, %X3 usw. | Variablen, die durch A+W Business mit den entsprechenden Werten gefüllt werden. ⇨ Softwarereferenz, "Systemtexte" auf Seite B-1046 |
| Anzahlung | `<aa>` | Anzahlungsauftragsnummer |
| Anzahlung | `<aad>` | Anzahlungsauftragsdatum |
| Anzahlung | `<ad>` | Anzahlungsdatum |
| Anzahlung | `<ar>` | Anzahlungsrechnungsnummer |
| Anzahlung | `<ard>` | Anzahlungsrechnungsdatum |
| CEKAL | `<h>` | Firmennummer aus den Firmendaten |
| CEKAL | `<jj>` | Jahr und Quartal im Format JJJJ-QQ |
| CEKAL | `<p1>` | Bezeichnung 1 |

*Tab. B-27: Variablen*

### Bearbeitungen

| Variable | Bedeutung |
| :--- | :--- |
| `<%>` | Anzahl (Kanten, Bohrungen, Eckausschnitte, ...) |
| `<$>` | Hauptparameter (Durchmesser, Radius, Breite, Höhe) |
| `<§>` | Ergänzungsparameter (welche Kanten, Ecken oder x, y, d bei Bohrungen) |
| `<=>` | Berechnete lfm |
| `<?>` | Berechnete qm |

| Bezeichnung 3 in Produktverwaltung | Bearbeitungsdialog, Positionserfassung |
| :--- | :--- |
| `<%>` Kanten [`<§>`] mit Gehrung 45° poliert (`<=>` lfm) | 2 Kanten [2/3] mit Gehrung 45° poliert (2,45 lfm) |
| Sägen von `<%>` Kanten `*<§>*` | Sägen von 3 Kanten *2/3/4* |
| `<%>` Lochbohrung(en) mit d = `<$>` mm | 2 Lochbohrungen mit d = 20 mm |
| `<%>` Bohrung(en) d=`<$>`mm X, Y [`<§>`] | 2 Bohrungen d = 20 mm X, Y [100, 100] |
| `<%>` x `<$>` mm Rundecke [`<§>`] | 4 x 15 mm Rundecke [1/2/3/4] |
| `<$>` Eckausschnitte / `<%>` Stück / [`<§>`] | 100 x 75 Eckausschnitte / 2 Stück / [3/4] |

### Rahmentexte

Die Rahmentexte können im Produkt eingetragen werden und verweisen auf die Standardtexte. Soll beim Kunden nur eine Nummer übergeben werden, so muss dort eine Nummer in den Standardtext eingetragen werden. Der gesamte Text kann mit Variablen übergeben werden.

| Variable | Bedeutung |
| :--- | :--- |
| `<ab>` | Abstandhalterkurzbezeichnung |
| `<ak>` | Abstandhalterkennzeichen |
| `<an>` | Auftragsnummer, ohne führende Null oder Leerzeichen |
| `<br>` | Breite, ohne führende Null oder Leerzeichen |
| `<c1>` | Kundenname 1 |
| `<cn>` | Kundennummer |
| `<esg>` | ESG Kurzbezeichnung |
| `<g>` | Gas |
| `<gt>` | Gütetext |
| `<ho>` | Höhe, ohne führende Null oder Leerzeichen |
| `<kp>` | Kundenposition |
| `<no>` | Auftragsnummer/Position |
| `<p1>` | Produktbezeichnung 1 |
| `<p2>` | Scheibenaufbau |
| `<pd>` | Produktionsdatum |
| `<pn>` | Produktnummer |
| `<po>` | Positionsnummer mit führenden Nullen, 3-stellig |
| `<ps>` | Positionsnummer, ohne führende Null oder Leerzeichen |
| `<sn>` | Schlüsselnummer |
| `<vs>` | VSG Bezeichnung |
| `<vsg>` | VSG Kurzbezeichnung |
| `<wh>` | Maße der Position |
| `<kk>` | Bestellübergabe: Kundenkommission |

*Tab. B-28: Variablen für Rahmentexte*

**Beispiel**
*   **Eingabe:** `<c1> <p1> <p2> <wh> <no>`
*   **Ausgabe:** John+Partner Standard ISO FL4/18/ORN528 540x1030 109384/001

## Konstruktionstypen Bleiverglasung

Für die Verarbeitung von Bleiverglasungen sind folgende Konstruktionstypen standardmäßig hinterlegt:

| Typ | Konstruktion |
| :--- | :--- |
| Typ 1 | Gothic |
| Typ 2 | Stuart |
| Typ 3 | Diamonds |
| Typ 4 | Cumberland |
| Typ 5 | Hanover |
| Typ 6 | Jacobean |
| Typ 7 | Northumberland |
| Typ 8 | Queen Anne |
| Typ 9 | Queen Caroline |
| Typ 10 | Rectangles |
| Typ 11 | Square Gothic |
| Typ 12 | Diamond Pillar |
| Typ 13 | Westmorland |
| Typ 14 | Windsor |

*Abb. B-329: Konstruktionstyp Bleiverglasung*

## Änderungsüberwachung

Änderungen in der Kunden-, Lieferanten-, Preis- und Rabattverwaltung können überwacht werden. Dazu steht in den entsprechenden Dialogen das Menü **Historie** zur Verfügung.

Für alle Datenbank-Tabellen, auf die ein Dialog zugreift, kann festgelegt werden, wie Änderungen überwacht werden sollen. Eine sehr detaillierte Überwachung wird möglich, wenn die betreffenden Tabellen auf der Ebene der Felder überwacht werden.

Die Änderungsüberwachung wird für jeden der genannten Dialoge getrennt eingestellt und aktiviert. In Allgemeinen werden in der Auswertung die Änderungen des aktuell ausgewählten Datensatzes angezeigt. Daneben kann die Auswertung aber auch nach Nummernverwaltern oder für alle Datensätze angezeigt werden.

Sowohl die Einstellungen als auch die Auswertungen beziehen sich immer auf den gerade eingestellten Laufzeit-Modus. Zum Beispiel betrifft das in der Preisverwaltung die Auswertung von Änderungen der Standardpreise, der Kundenpreise, der Kundengruppenpreise usw.

Daneben können die Auswertungen zusätzlich durch verschiedene Filter eingeschränkt werden, z. B. auf einen bestimmten Mitarbeiter oder einen Zeitraum.

### Änderungsüberwachung Verwaltung

*Utilities > System > Änderungsüberwachung Verwaltung*

[Abbildung: Screenshot des Dialogs "Änderungsüberwachung Verwaltung"]
*Abb. B-330: Änderungsüberwachung – Verwaltung*

In diesem Dialog legen Sie fest, welche Änderungen überwacht und dokumentiert werden sollen. Diese Funktion ist nur freigeschaltet, wenn Sie die entsprechenden Lizenzen erworben haben.

#### Menü Initialisierung
Über den Eintrag **Auswertung initialisieren** wird die Auswertung vorbereitet. Danach kann sie über das Menü **Historie > Auswertung** angezeigt oder gedruckt werden.

#### Allgemeine Einstellungen

*   **Sprache**: Sprache, in der die Auswertungen ausgegeben werden.
*   **Trigger erstellen**: Die Schaltfläche ist nur freigeschaltet, wenn:
    *   eine Änderungsüberwachung initialisiert wurde.
    *   die Einstellung für eine Tabelle oder ein Feld bearbeitet wurde.

> Die Datenbank-Trigger für die Überwachung müssen neu gebildet werden, wenn die Einstellungen neu festgelegt oder geändert wurden. Dies kann manuell gestartet werden (empfohlen). Es erfolgt automatisch beim Beenden des Dialogs. Dieser Vorgang kann einige Zeit in Anspruch nehmen.

#### Tabelleneinstellungen

**Übergreifende Einstellungen**
Wenn Sie die Einstellungen zur Überwachung von Änderungen über den Programmbereich **Utilities > System > Änderungsüberwachung Verwaltung** festlegen, gelten sie für alle verfügbaren Tabellen. Sie können die Einstellungen aber auch für den aktuellen Dialog festlegen.

*   **Name**: Bezeichnung der Tabelle. Sie kann geändert werden. Die Bezeichnungen werden in der Auswertung angezeigt.
    Wenn die Überwachung aktiviert ist, werden alle Felder dieser Tabelle im Bereich **Feldbeschreibungen** angezeigt.
*   **Historie**: In den Komboboxen der Spalte **Historie** stehen folgende Einstellungen zur Wahl:
    *   **Keine**: Die Änderungen werden nicht überwacht. Mit dieser Einstellung kann keine Auswertung angezeigt werden.
    *   **Komplett**: Die Änderungen werden für die gesamte Datenbank-Tabelle überwacht. In der Preisverwaltung müssen Sie diese Einstellung für alle Preistabellen wählen, wenn Sie sich auch alte Stände anzeigen lassen möchten.
    *   **Detailliert**: Die Änderungen werden auch auf Feldebene überwacht.

#### Feldeinstellungen

Wenn die Tabelle auf Feldebene überwacht wird, kann eingestellt werden, welche Felder eine Überwachung auslösen.

*   **Name**: Bezeichnung des Feldes. Sie kann geändert werden. Die Bezeichnungen werden in der Auswertung angezeigt.
*   **Referenziert auf**: Zum Identifizieren von Änderungen werden die Schlüsselspalten der jeweiligen Tabelle herangezogen. Handelt es sich bei den Schlüsselfeldern um referenzierende Felder, so wird in dieser Spalte die referenzierte Tabelle angegeben.
*   **Anzeigespalte**: In einer Tabelle, auf die verwiesen wird, kann neben dem Schlüsselwert auch eine Bezeichnung angezeigt werden. Die möglichen Bezeichnungen können aus der Kombobox in dieser Spalte ausgewählt werden. Z. B. verweist das Feld **Preisschlüssel** auf die Datenbank-Tabelle **Preisschlüssel**. Aus dieser Tabelle kann die Preisschlüsselnummer oder die Bezeichnung angezeigt werden. Wenn neben dem Schlüsselwert keine Bezeichnungen zur Verfügung stehen, ist die Kombobox leer.
*   **An/aus**: Diese Spalte und die Checkboxen werden nur angezeigt, wenn in den Tabelleneinstellungen in der Spalte **Historie** der Wert **detailliert** ausgewählt ist. In der Auswertung werden nur die Felder angezeigt, die über diese Checkboxen aktiviert sind. Sie können höchstens 80 Felder anzeigen lassen.
*   **Auswahl**: Über die beiden Schaltflächen zur Auswahl können alle Checkboxen in der Spalte **an/aus** aktiviert oder deaktiviert werden. Die Checkboxen können danach einzeln aktiviert oder deaktiviert werden.

## A+W Production

Produktionsrelevante Daten können an A+W Production übergeben werden. A+W Production verwendet die gleichen Stammdaten wie A+W Business. Änderungen in den Stammdaten müssen an A+W Production übergeben werden. Über die Produktnummer ist sichergestellt, dass beide Programme das gleiche Produkt verwenden. In jedem Produkt wird in A+W Business ein Kennzeichen zur Bearbeitung gesetzt. Dieses erzeugt die sogenannten Produktionsstücklisten für die Übergabe.

### Übergabedatei

Für die Übergabe wird eine ASCII-Datei in das Verzeichnis **AWPOOL** geschrieben. Für diese legen Sie fest, welche Parameter übergeben werden sollen.

**Beispiel**
*   Kundenspezifische Logo-Nummer
*   Relevante Textkennzeichen
*   Kantenschutz pro Auftrag (Aluband, nur ISO)
*   Abstandhalter (über den Fremdschlüssel aus der Produktdefinition)
*   Kennzeichen für das Gas

### Stammdatentransfer von A+W Business an A+W Production

Wenn das Zusatz-Modul **Stammdatentransfer** installiert ist, können folgende Daten übertragen werden. Ohne das Modul müssen die Daten in beiden Programmen identisch angelegt werden.

| Dialog in A+W Business | Feld | Dialog in A+W Production | Feld |
| :--- | :--- | :--- | :--- |
| **Produktverwaltung** | | | |
| Register Produkt: | Bezeichnung (1 - 3) | Artikelstammdaten: | Bezeichnung |
| | bei Produktarten: HW, TVG, ESG, ISO, VSG, GH | | Artikeltext (1 – 2) |
| | | | Checkbox Freigabeteil aktiv |
| | Sprossendicke | | Dicke |
| Bei Bearbeitungen | Produktgruppe, Mengeneinheit | Bearbeitungsartikel: | Klasse, Dauer s/ |
| Register Fertigung: | Struktur - Verlauf | Glasarten: | Struktur |
| Register Lager/Einkauf: | Beschaffungsart, Automatischer Zuschnitt, Technische Artikelnummer | Artikelstammdaten: | Beschaffungsart |
| | | Glasartikel: | Optimierbar, Artikelcode |
| Register A+W Production: | Glasart, Schleifgruppe, Modell, Bruchränder (o, u, r, I), Max. Traverenbreite, Min. Abst. X-Z Schnitte, Reihenf. Opti., Strukturlage, Beschichtungslage | Artikelstammdaten: | Glasart, Schleifgruppe |
| | | Glasartikel: | Modellbruchrand, Bruchränder, Max. Traverenbreite, Mindestabstand X-Z, Opti-Rang, Strukturlage, Schichtlage |
| Glasarten | Bezeichnung, Produktgruppe, Glasartgruppe, Struktur, Beschichtung | Glasarten: | Bezeichnung, Artikeltyp, Glasartgruppe, Struktur, Beschichtung |
| Glasart-Jumbos | Produktgruppe, Bezeichnung, Breite / Höhe Jumbo, Priorität für Opti., Traverenflag (X-Richtung, Y-Richtung, wahlweise) | Artikelstammdaten: | Artikeltyp, Bezeichnung |
| | | Lagermaße: | Breite / Höhe, Preis, Traveren |
| Jumbo-Zuschneidetische | Auflegercode, Anzahl | Lagermaße: | Auflegercode, Anzahl |
| **Zuschneidetische** | | | |
| Register Werte: | Bezeichnung, Breite / Höhe, Referenzpunkt, Z-Schnitt, Brechbeginn, Böcke per Zyklus, Spezial, Rang | Tische: | Beschreibung, Breite / Höhe, Referenz, Z-Schnitt, Brechbeginn, Böcke / Zyklus, Spezial, Rang |
| Register Einstellungen: | Autobrechen, Autoaufleger, Formen, VSG, Entschichten, Handzuschnitt, max. Traverenbreite darf | Tische: | Autobrechen, Autoaufleger, Formen, VSG, Entschichten, Handzuschnitt, maximale Traverenbreite |
| Register Schnitte: | Min. Abst. Y-Y Schnitte, Min. Abst. X-X Schnitte, Max. Abst. Y-Y Schnitte, Max. Abst. X-X Schnitte | Tische: | Min X-X, Max X-X, Min Y-Y |

*Tab. B-29: Übergabe der Stammdaten aus A+W Business an A+W Production*
*(Kurzinfo und Produktinfo werden nicht übergeben. Die Schleifgruppe wird aus A+W Production übernommen. Die Übergangszeit wird nicht übergeben. Die Werte zum maximalen Verschnitt werden nicht übergeben.)*

### Bearbeitungskatalog

Der hinterlegte Bearbeitungskatalog enthält alle Bearbeitungstypen und die erforderlichen Parameter. Er dient als zentrales Bindeglied zwischen den bestehenden Programmen der A+W Software GmbH.

Damit können aus A+W Business die Bearbeitungen inklusive aller dazugehöriger Daten an A+W Production oder per OrderXML übergeben werden.

Um immer wiederkehrende komplizierte Kombinationen von Bearbeitungen schnell erfassen zu können, kann zusätzlich ein von **Shaping & Nesting** generiertes Bearbeitungsmakro angehängt werden.

## Mischkalkulation

Für die Preisberechnung von kundenspezifischen Preisen kann statt eines Austauschzuschlages die sogenannte Mischkalkulation angewendet werden. Diese Art der Kalkulation wird in Österreich verwendet.

Dazu werden bis zu drei Produkte herangezogen, bei deren Kombination ein gemischter Preis kalkuliert werden soll. Für die Kalkulation wird angegeben, auf welche (kundenspezifische) Preistabelle dabei zurückgegriffen werden soll.

Die Berechnungsfaktoren für die Mischkalkulation werden in den Firmendaten hinterlegt. Außerdem wird dort festgelegt, ob eine Rabatt- und/oder Individualpreissuche bei der ISO-Mischkalkulation möglich sein soll.

Standardmäßig ist die Suche nach Individualpreisen und nach Rabatten bei der Mischkalkulation ausgeschaltet.

**Beispiel**
*   Basispreis 2-fach Isolierglas = 50% ISO-Preistabelle 1 + 50% ISO-Preistabelle 2.
*   Basispreis 3-fach Isolierglas = 50% ISO-Preistab. 1 + 80% ISO-Preistab. 2 + 50% ISO-Preistab. 3.

Für die erste Scheibe der ISO-Einheit wird der Preis für aus der ISO-Preistabelle 1 und für die zweite Scheibe der ISO-Einheit der Preis aus der ISO-Preistabelle 2 genommen. Bei einem 3-fach Isolierglas wird für die dritte Scheibe der ISO-Einheit der Preis aus der ISO-Preistabelle 3 genommen.

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Produktverwaltung - A+W Production" auf Seite B-621
*   ⇨ Softwarereferenz, "Firmendaten - Produktion" auf Seite B-987
*   ⇨ Verkauf, "Parameter" auf Seite C-469
*   ⇨ Softwarereferenz, "Mischkalkulation" auf Seite B-698
*   ⇨ Softwarereferenz, "Mischkalkulationsfaktoren" auf Seite B-931
*   ⇨ Softwarereferenz, "Rabattsuche bei ISO-Mischkalkulation" auf Seite B-948
*   ⇨ Softwarereferenz, "Individualpreissuche bei ISO-Mischkalkulation" auf Seite B-949

## Französische Preisberechnung

Bei der sog. französischen Preisberechnung von ISO setzt sich der Preis für das ISO aus folgenden Komponenten zusammen:
*   Basispreis für den Zusammenbau des ISO
*   Einzelpreise für die Gläser

Dafür werden in der Regel eigene Schlüssel und Tarife definiert. Die Preise für die jeweiligen Einzelgläser werden in der gewohnten Form definiert. Sie müssen im selben Preisschlüssel liegt wie der ISO-Basispreis. Für das ISO muss die Preiseinheit `<qm+EP>` gewählt werden.

Die Produkte werden in der üblichen Form angelegt. Für die Abstandhalter wird ein Sonstiger Zuschlag angelegt und dem ISO-Preis zugeordnet.

> **ISO und VSG**
> Bei der frz. Preisberechnung darf in den Firmendaten die Option **Iso und VSG-Einzelpreisberechnung** nicht aktiviert werden.
> ⇨ Softwarereferenz, "ISO + VSG Einzelpreisberechnung" auf Seite B-949

## Kalkulation

**Lernziele**
*   Komponenten der Kostenkalkulation.
*   Vorgaben für die Eigenkosten-Kalkulation festlegen.
*   Kalkulation des Deckungsbeitrags festlegen.

**Nutzen**
*   Die Höhe der Eigenkosten wird übergreifend eingestellt und in die Kalkulationen des Deckungsbeitrags und der Einkaufspreise einbezogen.
*   Der Deckungsbeitrag wird automatisch neu berechnet, wenn im Dokument die Preise bei der Erfassung von Positionen geändert werden.

| Merkmal | Beschreibung |
| :--- | :--- |
| **Herstellkosten** | Die Herstellkosten setzen sich zusammen aus: Material-, Maschinen- und Personalkosten zuzüglich Gemeinkosten. |
| **Gemeinkosten** | Die prozentualen Anteile für die Gemeinkosten legen Sie in den Firmendaten fest. |
| **Kalkulation** | Die Kostenkalkulation wird pro Tarif (Preisjahrgang und -schlüssel) aktiviert: <br> • Wenn die Kalkulation in den Tarifen nur für die EK-Preisberechnung aktiviert ist, wird die Kosten- und Aufschlagskalkulation nur bis zum Selbstkostenpreis durchgeführt. <br> • Wenn auch in den VK-Tarifen die Kalkulation aktiviert ist, geht die Kalkulation weiter bis zum Verkaufspreis. |
| **Teilmaterialkosten** | Die Teilmaterialkosten errechnen sich aus der Menge (inkl. produktbezogenem Verschnitt) und dem Preis pro Mengeneinheit. |
| **Vollmaterialkosten** | Auf die Teilmaterialkosten wird ein Gemeinkostenzuschlag berechnet, der die Beschaffungsart des Produkts berücksichtigt. |
| **Deckungsbeitrag** | Für die Ermittlung des Deckungsbeitrags werden Mindest- und Höchstwerte pro Kunde und Warengruppe gepflegt. Die aktuellen Deckungsbeiträge werden pro Dokument ermittelt und angezeigt. Die Deckungsbeitrags-Analyse ermittelt die Deckungsbeiträge über einen beliebigen Zeitraum. |

### Deckungsbeitrags-Grenzwerte

Deckungsbeiträge werden im Auftrag direkt angezeigt und beziehen sich nur auf die im Auftrag enthaltenen Positionen.

[Abbildung: Screenshot der Anzeige des Deckungsbeitrags im Auftrag]
*Abb. B-331: Anzeige des aktuellen Deckungsbeitrags im Auftrag und pro Position*

Mit Hilfe der Deckungsbeitrags-Analyse kann der Deckungsbeitrag von Auftragspositionen über einen beliebigen Zeitraum untersucht und gedruckt werden. Diese Auswertung wird im Modul **Dokumente** gestartet.

[Abbildung: Screenshot der Deckungsbeitrags-Analyse]
*Abb. B-332: Deckungsbeitrags-Analyse*

Die minimalen und maximalen Deckungsbeiträge werden im Dialog **Deckungsbeitrags-Grenzen** pro Kunde und Warengruppe gepflegt.

[Abbildung: Screenshot des Dialogs "Deckungsbeitragsgrenzen"]
*Abb. B-333: Deckungsbeitragsgrenzen*

*   **A**: Auswahl Kunde oder Kundengruppe
*   **B**: Auswahl Warengruppe
*   **C**: Angabe der Grenzwerte

Die Grenzwerte legen Sie pro Kunde oder Kundengruppe (A) fest. Die Analyse bezieht sich jeweils auf eine Warengruppe (B), wobei Sie alle drei Ebenen (WGR, WOG, WHG) wählen können.

Für jede Kombination von (A) und (B) können Sie prozentualen Werte (C) für die Deckungsobergrenze und die Deckungsuntergrenze festlegen. Damit können Sie z. B. leichter prüfen, ob der Deckungsbeitrag für den Kunden oder die Kundengruppe im gewünschten Rahmen liegt.

Da jede Kalkulation von Preisen im einzelnen Auftrag überschrieben werden kann, können ein Höchst- und ein Mindestbetrag für Deckungsbeiträge hinterlegt werden. Damit werden grobe Fehlkalkulationen bei der manuellen Preisgestaltung im Auftrag verhindert, z. B. ein Verkaufspreis unter den Selbstkosten.

[Abbildung: Screenshot der Firmendaten mit Standardwerten für Deckungsbeitrag]
*Abb. B-334: Firmendaten - Standardwerte für Deckungsbeitrag*

*   **A**: Mindestbeitrag für Deckungsbeiträge
*   **B**: Höchstbeitrag für Deckungsbeiträge

Für alle nicht explizit definierten Kombinationen von Kunden und WGR gelten die Standardwerte, die in den Firmendaten im Register **Kalkulation** festgelegt sind.

### Kosten- und Aufschlagskalkulation

Mit der Kosten-/Aufschlagkalkulation wird der Preis pro Preiseinheit ermittelt. Dazu werden die Anteile der Selbstkosten aus den Firmendaten berücksichtigt.

**Herstellungskosten**
Auf der Basis von Material-, Maschinen- und Personalkosten werden Herstellkosten ermittelt. Zuzüglich der Gemeinkostenzuschläge für Material und Sondereinzelkosten ergeben sich daraus die Vollherstellkosten.

Zu den Materialgemeinkosten zählen die Beschaffungsarten:
*   Bestellung
*   Lagerentnahme
*   Produktion

Auf diese werden Gemeinkosten für Verwaltung und Vertrieb aufgeschlagen. Zuzüglich einer prozentualen Gewinnerwartung ergibt sich daraus der Verkaufspreis.

Zu den Gemeinkosten zählen:
*   **Lohnnebenkosten**: z. B. Kosten für Sozialversicherungen.
*   **Vertriebsgemeinkosten**: Kosten, die den Produkten nicht im Einzelnen zugeordnet werden können, z. B. Provisionen.
*   **Verwaltungsgemeinkosten**: z. B. Kosten für Büro, Energie, Verwaltungsmitarbeiter usw.
*   **Gewinnspanne**

Die prozentualen Anteile für die Gemeinkosten legen Sie in den Firmendaten fest.

[Abbildung: Screenshot der Firmendaten - Vorgaben für die Kostenkalkulation]
*Abb. B-335: Firmendaten – Vorgaben für die Kostenkalkulation*

*   **A**: Zuschläge für die Materialkosten
*   **B**: Zuschläge für Gemeinkosten

Diese prozentualen Aufschläge (A, B) beziehen sich auf die Einkaufspreise (netto).
Die Kostenkalkulation wird pro Tarif (Preisjahrgang und -schlüssel) aktiviert.

[Abbildung: Screenshot der Aktivierung der Kostenkalkulation in den Tarifen]
*Abb. B-336: Aktivierung der Kostenkalkulation in den Tarifen*

*   **A**: Kostenkalkulation für EK-Tarif
*   **B**: Kostenkalkulation für VK-Tarif

Wenn die Kalkulation in den Tarifen nur für die EK-Preisberechnung aktiviert ist, wird die Kosten- und Aufschlagskalkulation nur bis zum Selbstkostenpreis durchgeführt. Wenn auch in den VK-Tarifen die Kalkulation aktiviert ist, geht die Kalkulation weiter bis zum Verkaufspreis.

Im Dokument und in den Positionen können Sie sich die Kalkulationen für den aktuellen Auftrag anzeigen lassen.

[Abbildung: Beispiele für Übersichten zur Kalkulation]
*Abb. B-337: Beispiele für Übersichten zur Kalkulation*

*   **A**: Position
*   **B**: Kosten der Stücklisten-Komponenten

In diesen Beispielen sehen Sie die Kalkulation für eine Position (A). In der Positionserfassung kann die Kalkulation für die Stückliste (B) geprüft werden. Preise, die implizit in einem Produkt enthalten sind, werden dabei nicht angezeigt.

Die Kalkulation kann pro Position angepasst werden, z. B. um bestimmte Nebenkosten mit einem abweichenden Prozentsatz zu kalkulieren oder um Sonderkosten zu berücksichtigen.

[Abbildung: Übersicht zur Kalkulation einer Position]
*Abb. B-338: Übersichten zur Kalkulation einer Position*

*   **A**: Anpassung der Gemeinkosten und Sonderzuschläge
*   **B**: Anpassung der Gewinnerwartung
*   **C**: Eingabe von Sonderkosten

Die Kostenkalkulation kann pro Position auch um Sonderzuschläge erweitert werden. Wenn diese Zuschläge als negativer Wert angegeben werden, entspricht das einem Sonderrabatt für diese eine Position.

> **Maschinen- und Personalkosten aus der Produktion**
> Die Anteile aus Maschinen- und Personalkosten werden über die zugehörigen Basisdaten aus der Kapazitätsplanung errechnet. Diese Kostenfaktoren stehen daher nur zur Verfügung, wenn die **A+W Business-Kapazitätsplanung** freigeschaltet ist und wenn Rückmeldungen zu den tatsächlichen Kosten aus der Produktion vorliegen.

### Kalkulation der Eigenkosten festlegen

Für die Kalkulation der Eigenkosten für Isolierglas legen Sie pro Abstandhalter den durchschnittlichen Verbrauch von Hilfsstoffen wie Butyl, Thiokol usw. fest. Ein ausführliches Beispiel finden Sie in einer separaten Einheit.
⇨ "Komplexbeispiel: Kalkulation ISO" auf Seite B-547

> **Voraussetzung**
> Die Verbrauchsartikel, die im Bereich **Stücklistenprodukt** eingetragen werden sollen, müssen als Produkte angelegt sein.

**So legen Sie Vorgaben für die Kalkulation der Eigenkosten fest**

1.  Wählen Sie im Menü **Stammdaten > Produkte > Artikel > EK-Kalkulation**. Der Dialog **Kalkulationsvorgaben** wird geöffnet.
    ⇨ Softwarereferenz, "EK-Kalkulation" auf Seite B-647
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.

[Abbildung: Screenshot des Dialogs EK-Kalkulation]
*Abb. B-339: Felder für neuen Preis freigeschaltet*

*   **A**: Angaben für Abstandhalter (SZR)
*   **B**: Rückschnitt
*   **C**: Gasmenge
*   **D**: Angaben für Produkte aus Stückliste

3.  Geben Sie die Artikelnummer des Abstandhalters (A) ein, dem der Verbrauch an Gas, Trockenmittel oder Randverbund zugeordnet werden soll. Detaillierte Beispiele finden Sie in der nachfolgenden Einheit.
4.  Tragen Sie die gewünschten Werte in die Felder ein:
    *   **Rückschnitt (einfach)** in mm (B)
    *   **Entspannte Menge für Gas** in Liter (C)
5.  Wechseln Sie zum Register **Stückliste**.
6.  Markieren Sie im Bereich **Stückliste** eine Zeile mit der Artikelnummer 0.
7.  Tragen Sie im Bereich **Stücklistenprodukt** (D) die Produktnummer, den Verbrauch des Artikels und dessen Bezugseinheit ein. Die Einträge werden im Bereich **Stückliste** angezeigt.
8.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern. Die Daten werden gespeichert.

> **Rückschnitt**
> Mit dem **Rückschnitt (einfach)** ist der Abstand von der Glasaußenkante bis zum Alurahmen außen gemeint. Er ist wichtig für den Bieger der Alurahmen. Beträgt das Glasmaß z. B. 1000 x 1000 mm, der **Rückschnitt (einfach)** 5 mm, so beträgt das Rahmenmaß 990 x 900 mm.

### Komplexbeispiel: Kalkulation ISO

In diesem Beispiel wird gezeigt, wie die Eigenkalkulation (EK) einer Isolierglas-Einheit bei Eigenfertigung eingerichtet und im Auftrag angezeigt wird.

Die Kalkulation wird in folgenden Einheiten dargestellt:
*   Berechnung der Scheiben
*   Berechnung des Rahmens
*   Berechnung für das Gas
*   Berechnung der Verbrauchsmaterialien

Bei der Beispielberechnung wurde auf Rundungen, Rabatte und Zuschläge verzichtet, damit die Kalkulation einfach nachzuvollziehen ist.

**Anzeige in der Positionserfassung**

[Abbildung: Screenshot der EK-Preise im Auftrag]
*Abb. B-340: Anzeige der EK-Preise im Auftrag*

Die EK-Preise einer Auftragsposition können über das Menü **Ansicht** angezeigt werden. Die im Beispiel angezeigten Werte sind in der folgenden Berechnung enthalten:

| Legende | Produkt | Operator | Preis |
| :--- | :--- | :--- | :--- |
| 1 | 1. Scheibe | + | 8,57 |
| 2 | 2. Scheibe | + | 10,91 |
| 3 | Verbrauchsmaterialien | + | 3,68 |
| 4 | Rahmen | + | 1,60 |
| 5 | Gas | + | 0,12 |
| 6 | Stückkosten | = | 24,88 |

*Tab. B-30: Berechnung des Einkaufspreises*

Die Kalkulation der Nummern 1 - 5 wird im Folgenden detailliert dargestellt.

#### Berechnung der Scheiben

Bei der Berechnung der Scheiben werden der Einkaufpreis aus der zugeordneten Preistabelle, der Verschnitt und die Rundung berücksichtigt. Im gezeigten Beispiel ist keine Rundung der Fläche definiert.

**Erste Scheibe**
Der EK-Preis aus der Preistabelle wird mit der Fläche multipliziert. In diesem Beispiel ist die Höhe x Breite = 1 qm. Zum errechneten Wert wird ein Betrag für den Verschnitt addiert.

| EK |
| :--- |
| EK x (Fläche + Verschnitt) |
| 8,24 x (1 + 4/100) |
| **8,57** |

*Tab. B-31: EK-Berechnung der ersten Scheibe*

**Verschnitt**
In den Produktstammdaten werden im Register **Preis/Zuschlag** die Preistabellen für den VK und den EK zugeordnet und der mittlere Verschnitt definiert.

[Abbildung: Screenshot der Produktstammdaten mit Fokus auf den prozentualen Verschnitt]
*Abb. B-341: Produktstammdaten – prozentualer Verschnitt, Beispiel: erste Scheibe*

**Preis**
In der Preistabelle wird der Einkaufspreis hinterlegt, den Sie mit Ihrem Lieferanten vereinbart haben.

[Abbildung: Screenshot der Preistabelle mit dem Preis pro Einheit]
*Abb. B-342: Preis pro Einheit der ersten Scheibe*

**Zweite Scheibe**
Die Berechnung der zweiten Scheibe basiert ebenfalls auf den Stammdaten. Die Werte können sich von der ersten Scheibe unterscheiden.

| EK |
| :--- |
| EK x (Fläche + Verschnitt) |
| 10,20 x (1 + 7/100) |
| **10,91** |

*Tab. B-32: Berechnung der zweiten Scheibe*

Verschnitt und Preis werden so wie bei der ersten Scheibe in den Stammdaten festgelegt.

#### Berechnung des Rahmens

In diesem Beispiel beträgt die Kantenlänge genau 1000 mm. Die Gesamtlänge des Rahmens beträgt also 4 m.

| EK |
| :--- |
| EK Rahmen x effektive Lfm |
| 0,40 x 4 |
| **1,60** \* |

\* Nr. 4 der Tabelle "Berechnung des Einkaufspreises" auf Seite B-547
*Tab. B-33: Berechnung des Rahmens*

Der Preis wird ebenfalls als Einzelpreis in den Stammdaten festgelegt. In der Preistabelle wird der Einkaufspreis pro Preiseinheit hinterlegt, den Sie mit Ihrem Lieferanten vereinbart haben. In diesem Beispiel ist das 0,40/lfm.

#### Berechnung für das Gas

Zur Berechnung des Gases wird die hinterlegte Gasmenge mit der Dicke des Scheibenzwischenraums multipliziert.

| EK |
| :--- |
| m³ x SZR/Entspannte Menge Gas x EK Gas (1 + Verschnitt/100) |
| 1 x 12/21000 x 215,90/(1 + 0/100)\* |
| **0,12**\*\* |

\* In diesem Beispiel wird ohne Verschnitt für das Gas gerechnet.
\*\* Nr. 5 der Tabelle “Berechnung des Einkaufspreises" auf Seite B-547
*Tab. B-34: Berechnung des Gases*

**Kalkulationsgrundlage**
Unter **Stammdaten > Produkte > Artikel > EK Kalkulation** wird die entspannte Menge des Gases (ohne Druck, ohne Kühlung) pro Kubikmeter angegeben.

[Abbildung: Screenshot der Kalkulationsgrundlage für Wärmedämmgas]
*Abb. B-343: Kalkulationsgrundlage für den Verbrauch von Wärmedämmgas*

Der Preis wird ebenfalls als Einzelpreis in den Stammdaten festgelegt. In der Preistabelle wird der Einkaufspreis pro Preiseinheit hinterlegt, den Sie mit Ihrem Lieferanten vereinbart haben.

#### Berechnung der Verbrauchsmaterialien

Zusätzlich zu Scheiben, Rahmen und Gasfüllung können Verbrauchsmaterialien angegeben werden, die bei der Produktion der ISO-Einheit benötigt werden.

| | EK |
| :--- | :--- |
| EK Butyl | 2,2 |
| + EK Thiokol | 0,028696 |
| + EK Trockenmittel | 1,4484 |
| | **3,68** \* |

\* Nr. 3 der Tabelle "Berechnung des Einkaufspreises" auf Seite B-547
*Tab. B-35: Berechnung der Verbrauchsmaterialien*

In den folgenden Abschnitten ist dargestellt, wie die drei Einzelbeträge errechnet wurden.

**Berechnung für das Butyl**
| EK |
| :--- |
| EK Butyl x tatsächliche Laufmeter x Verbrauch pro Einheit |
| 100 x 4 x 0,0055 |
| **2,20** |

*Tab. B-36: Berechnung des Butyls*

Zur Berechnung des Verbrauchs ist die Menge pro Einheit festgelegt. In diesem Beispiel werden 0,0055 kg pro laufendem Meter (Rahmen) berechnet. Der Preis wird ebenfalls als Einzelpreis in den Stammdaten festgelegt. In der Preistabelle wird der Einkaufspreis pro Preiseinheit hinterlegt, den Sie mit Ihrem Lieferanten vereinbart haben.

**Berechnung für das Thiokol**
| EK |
| :--- |
| EK Thiokol x effektive Lfm x Verbrauch pro Einheit |
| 1,17 x 4 x 0,0422 |
| **0,028696** |

*Tab. B-37: Berechnung des Thiokols*

Zur Berechnung des Verbrauchs ist die Menge pro Einheit festgelegt. In diesem Beispiel werden 0,0422 Liter pro laufendem Meter (Rahmen) berechnet. In der Preistabelle wird der Einkaufspreis pro Preiseinheit als Einzelpreis hinterlegt.

**Berechnung der Trockenmittel**
| EK |
| :--- |
| EK Trockenmittel x effektive lfm x Verbrauch pro Einheit |
| 8,50 x 4 x 0,0426 |
| **1,4484** |

*Tab. B-38: Berechnung des Trockenmittels*

Zur Berechnung des Verbrauchs ist die Menge pro Einheit festgelegt. In diesem Beispiel werden 0,0426 kg pro laufendem Meter (Rahmen) berechnet. In der Preistabelle wird der Einkaufspreis pro Preiseinheit als Einzelpreis hinterlegt.

**Ergänzende Informationen**
*   ⇨ Tutorial 2, "Kalkulation der Eigenkosten festlegen" auf Seite B-545
*   ⇨ Softwarereferenz, "Einkauf" auf Seite B-957
*   ⇨ Softwarereferenz, "Firmendaten – Kalkulation" auf Seite B-981

## Produktverwaltung

*Stammdaten > Produkte > Artikel > Artikel*

In A+W Business können Sie Ihre firmeneigene Produktstruktur abbilden. Sie sind frei in der Vergabe sowohl der Artikelnummer (bis zu 8 Stellen) als auch eines alphanumerischen Codes (Matchcode mit bis zu 15 Stellen).

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menüs in der Produktverwaltung" auf Seite B-588
*   "Produktverwaltung" auf Seite B-590
*   "Technische Parameter" auf Seite B-628
*   "Technische Parameter kopieren" auf Seite B-630
*   "Produktänderung" auf Seite B-631
*   "Produktkennzeichen Verwaltung" auf Seite B-632
*   "Glasarten" auf Seite B-635

### Menüs in der Produktverwaltung

*Stammdaten > Produkte > Artikel > Artikel*

Über die Menüs der Produktverwaltung können Sie die Standardeinstellung des Dialoges bestimmen und andere Dialoge öffnen, ohne die Produktverwaltung zu schließen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menü Optionen" auf Seite B-588
*   "Menü Funktionen" auf Seite B-589

#### Menü Optionen

*Stammdaten > Produkte > Artikel > Artikel > Menü Optionen*

Über dieses Menü können Sie die Standardeinstellungen des Dialogs festlegen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen. Folgende Einträge werden angezeigt:
*   Fehlermeldungen A+W Production-Übergabe gesammelt ausgeben: Übertragungsfehler bei der Übergabe der Produktionsdaten werden gesammelt in einer Meldung angezeigt.

#### Menü Funktionen

*Stammdaten > Produkte > Artikel > Artikel > Menü Funktionen*

Über dieses Menü können Sie weitere Dialoge öffnen, ohne den Dialog zu schließen.

**Gruppe Technische Parameter**
*   **Technische Parameter allgemein**: Öffnet den Dialog Technische Parameter, um technische Parameter auszulesen oder zu ändern. ⇨ "Technische Parameter" auf Seite B-628
*   **Technische Parameter Isolierglas**: Öffnet den Dialog Technische Parameter, um technische Parameter für ein ausgewähltes ISO-Glas auszulesen oder zu ändern. ⇨ "Technische Parameter" auf Seite B-628
*   **Technische Parameter kopieren**: Öffnet den Dialog Technische Parameter, um technische Parameter für ein ausgewähltes ISO-Glas zu kopieren. ⇨ "Technische Parameter kopieren" auf Seite B-630

**Gruppe Preisverwaltung, Gruppe VK-Relevant, Gruppe EK-Relevant**
*   **Aufruf Preisverwaltung VK, ΕΚ**: Öffnet die Preisverwaltung, in der der Verkaufs- oder der Einkaufspreis für das gewählte Produkt geändert werden kann. ⇨ "Preisverwaltung" auf Seite B-712
*   **Setzen für alle Stücklistenelemente**: Aktiviert das entsprechende Preiskennzeichen für alle Stücklisten-Komponenten. ⇨ "Produktverwaltung - Stückliste" auf Seite B-616
*   **Löschen für alle Stücklistenelemente**: Deaktiviert das entsprechende Preiskennzeichen für alle Stücklisten-Komponenten.

**Gruppe Druckkennzeichen**
*   **Setzen für alle Stücklistenelemente**: Aktiviert das Druckkennzeichen für alle Stücklisten-Komponenten.
*   **Löschen für alle Stücklistenelemente**: Deaktiviert das Druckkennzeichen für alle Stücklisten-Komponenten.

**Gruppe A + W Production**
*   **Selektierte Produkte an A+W Production übergeben**: Sendet die Daten des ausgewählten Produktes an A+W Production.
*   **Alle Stammdaten an A + W Production übergeben**: Sendet alle Glasartengruppen, Glasarten, Jumbos, Tische und Tischzuordnungen an A+W Production.
*   **A + W Production Stammdaten einlesen**: übernimmt die Stammdaten von A+W Production.

**Gruppe Ändern/Löschen**
*   **Selektierte Produkte ändern**: Öffnet den Dialog Produktänderung, in dem Sie die automatischen Zuschläge für das gewählte Produkt aktivieren oder deaktivieren können. ⇨ "Produktänderung" auf Seite B-631
*   **Selektierte Produkte löschen**: Löscht alle Produkte, die in der Übersicht aufgelistet sind.

**Gruppe CE**
*   **CE-Stammdaten importieren**: Diese Funktion ist nur freigeschaltet, wenn die entsprechenden Dateien zum Import bereitliegen. In der Regel werden die Daten bei der Installation und Konfiguration von A+W Business importiert.

### Produktverwaltung

*Stammdaten > Produkte > Artikel > Artikel*

In diesem Dialog verwalten Sie Ihre Produkte, z. B. Einfachglas, ISO, VSG, ESG, Modelle, Sprossen, Bearbeitungen, Stückartikel wie Türgriffe, usw.

Im Dialog **Produktverwaltung** finden Sie folgende Register:
*   Produktverwaltung – Produkt
*   Produktverwaltung – Fertigung
*   Produktverwaltung – Preis/Zuschlag
*   Produktverwaltung – Lager/Einkauf
*   Produktverwaltung – Modelle/Bearbeitungen
*   Produktverwaltung – Stückliste
*   Produktverwaltung – Texte
*   Produktverwaltung - Sprachen
*   Produktverwaltung – A+W Production
*   Produktverwaltung – Anlagen/Klassifikatoren
*   Produktverwaltung – Sprossen
⇨ Tutorial 1, "Produktdaten" auf Seite B-133

#### Produktverwaltung – Produkt

*Stammdaten > Produkte > Artikel > Artikel > Register Produkt*

[Abbildung: Screenshot des Registers "Produkt" in der Produktverwaltung]
*Abb. B-372: Produktverwaltung – Produkt*

In diesem Dialog können Sie Ihre firmeneigenen Produkte anlegen und bearbeiten. Sie können die Artikelnummer (bis zu 8 Stellen) und den alphanumerischen Matchcode frei wählen. Die Artikelnummer kann nach dem Speichern neuer Produktdaten nicht mehr geändert werden.
⇨Tutorial 1, "Produkt anlegen" auf Seite B-182

**Artikel**
*   **Nummer**: Anzeige der Artikelnummer (Produktnummer). Wenn Sie neue Produktdaten anlegen, können Sie sich über die Lupe die freien Nummern anzeigen lassen.
    ⇨ "Freie Nummern / Bereiche" auf Seite B-789
*   **Matchcode**: Der Matchcode dient als Suchkriterium. Er kann bis zu 15 alphanumerische Zeichen enthalten.
*   **EAN**: EAN-Code bzw. GTIN-Code. In den USA kann das Feld für den UPC-Code verwendet werden.
*   **Bezeichnung (1 bis 3)**: Name und kurze Beschreibung des Produkts. Die Bezeichnung wird in der Positionserfassung angezeigt und beim Formulardruck ausgewertet.
    *   Bei Einzelscheiben, die in eine ISO-Einheit eingebaut werden, wird nur die erste Bezeichnung ausgelesen.
    *   Für die Bezeichnung 1 können Sie Variablen (Platzhalter) verwenden, um die Gültigkeitsdauer von Sonderrabatten bzw. Teuerungszuschlägen (Produktzuordnung Zuschläge) mit auszuweisen.
        ⇨Tutorial 2, "Variablen" auf Seite B-466
    *   Für die Bezeichnung 3 können Sie bei der Produktart Bearbeitungen Variablen (mit Formeln) verwenden. Im Dokument wird dieser Text vom System mit den Werten der Bearbeitungsparameter gefüllt.
        ⇨ Tutorial 2, "Verfügbare Variablen (Platzhalter)" auf Seite B-525
*   **[Formel]**: Öffnet den Dialog Parameter-Ersetzung, in dem Sie die zulässigen Parameter auswählen können. Achten Sie auf die Schreibweise, wenn Sie das Feld für Formeln nutzen, damit A+W Business den Text korrekt interpretieren kann.

    **Beispiele**
    | Bezeichnung 3 im Dialog Produktverwaltung | Beschreibung im Dialog Positionserfassung |
    | :--- | :--- |
    | `<%>` Kanten `*<§>*` mit Gehrung 45° poliert (`<=>` lfm) | 2 Kanten `*2/3*` mit Gehrung 45° poliert (2,45 lfm) |
    | Sägen von `<%>` Kanten `*<§>*` | Sägen von 3 Kanten `*2/3/4*` |
    | `<%>` Lochbohrung(en) mit d = `<$>` mm | 2 Lochbohrungen mit d = 20 mm |
    | `<%>` Bohrung(en) x/y/D in mm `*<§>*` | 2 Bohrungen x/y/D in mm `*100,100, 25-200,200,16*` |
    | `<%>` x `<$>` mm Rundecke `*<§>*` | 4 x 15 mm Rundecke `*1/2/3/4*` |
    | `<$>` Eckausschnitte/`<%>` Stück/`*<§>*` | 100 x 75 Eckausschnitte/2 Stück/3/4* |
    | `<%>` Kante(n) `*<$>*` mit `<$>` mm Facette | 2 Kante(n) `*1/4*` mit 20,0 mm Facette |

    ⇨ Verkauf, "Parameter-Ersetzung" auf Seite C-589
*   **Kurzinfo**: Kurzinfo für den Etikettendruck (maximal 20 Zeichen), z. B. ISO 2 x FL4 für Isolierglas 2 x Float 4 mm oder FL4 für Floatglas 4 mm.
*   **Artikelinfo**: Feld für zusätzliche produktspezifische Informationen (ohne Zeichenlimitierung). Die Info kann in der Positionserfassung angezeigt werden.
*   **Anzeige**: Der Text aus dem Feld **Artikelinfo** kann beim Erfassen einer Position angezeigt werden.
    *   ☐ Der Text wird nicht automatisch angezeigt.
    *   ☑ Beim Erfassen des Produkts wird automatisch der Dialog **Artikel-Info** geöffnet, in dem der Aufbau der Stückliste und die Preise geprüft werden können.
*   **Anzeige in Stückliste**: Der Text aus dem Feld **Artikelinfo** kann in der Stückliste angezeigt werden, z. B. beim Austausch.
    *   ☐ Der Text wird nicht angezeigt, wenn das Produkt in einer Stückliste verwendet wird.
    *   ☑ Wenn die Checkbox Anzeige aktiviert ist, wird der Text in der Positionserfassung nur angezeigt, wenn das Produkt als Hauptprodukt erfasst wird.
    *   ☑ Der Text wird auch dann angezeigt, wenn das Produkt eine Stücklisten-Komponente ist.
*   **[Icon Info]**: Öffnet den Dialog **Artikel-Info**, um Details zum Produkt zu prüfen.
    ⇨ Verkauf, "Artikel-Informationen" auf Seite C-602
*   **[Icon Varianten]**: Öffnet den Dialog **Produktvarianten**, um Varianten zum Produkt zu prüfen oder anzulegen.
    ⇨ "Varianten" auf Seite B-572

**Eigenschaften**
*   **Produktart, Produktgruppe**: Jedem Produkt werden eine Produktart und eine Produktgruppe zugewiesen. Sie dienen als Ordnungskriterium bei der Suche und können in Auswertungen und zur Preisfindung bei Modellzuschlägen herangezogen werden.

    **Beispiele**
    | Produktart | Produktgruppe | Produkt |
    | :--- | :--- | :--- |
    | Einfachglas | Einfachglas | Float 6 mm |
    | | Ornamentglas | Ornm. Altd. Glatt 4 mm, Ornm. Kathedral weiß 4 mm |
    | Bearbeitungen | Rundecken | Rundecke fein, Rundecke grob |
    | | Randausschnitt | Randausschnitt - 100 x 200 mm ESG |
    | ESG | ESG | ESG klar 12 mm |
    | | Ganzglastür | ESG Tür weiß |
    | ISO | ISO | CLIMALIT Standard 2 x 4 mm Float |

    ⇨ "Produktarten" auf Seite B-565
    ⇨ "Produktgruppen" auf Seite B-566
*   **WGR**: Jede der drei Warengruppenebenen kann dem Produkt zugewiesen werden. Wenn Sie z. B. zwischen ISO und ISO mit Modellen unterscheiden wollen, müssen Sie dem Modell eine WGR zuordnen. Zur Unterscheidung legen Sie dann für jede Auswertung eine Kombi-WGR an. Wenn Sie keine differenzierte Auswertung benötigen, tragen Sie den Wert **0** ein. Das Modell wird dann automatisch der Warengruppe des Hauptprodukts zugeordnet, also dem ISO oder dem Einfachglas.
    ⇨Tutorial 1, "Kombi-WGR" auf Seite B-143
    ⇨ Softwarereferenz, "Kombi-WGR" auf Seite B-569
*   **WGR-Statistik**: In der Regel wird dieselbe WGR eingetragen wie im Feld WGR. Die WGR-Statistik bietet die Möglichkeit, für den Rabatt- und Statistikbereich unterschiedliche Warengruppenstrukturen aufzubauen.

**Einheiten / Restriktionen**
Die nachfolgenden Maße werden für die Beladung des Transportmittels und für technische oder preisliche Restriktionen herangezogen.

*   **Dicke / Sprossendicke**: Bei Gläsern die Glasdicke, bei Sprossen die Sprossendicke in mm
*   **Gewicht**: Gewicht des Glases pro Mengeneinheit. Im Auftrag dient das Gewicht zur Berechnung eines Zuschlags, z. B. für den Transport bei besonders schweren Positionen.

    **Beispiel**
    1 mm Float wiegt 2,5 kg pro qm
    5 mm Float wiegen 5 x 2,5 kg = 12,5 kg pro qm

*   **Breite / Höhe min.**: Mindestmaße für Breite und Höhe für die Positionserfassung. Die Werte werden während der Positionserfassung geprüft. Bei Unterschreitung wird eine Meldung angezeigt. Der Auftrag kann dann abgelehnt, mit einem anderen Produkt oder evtl. mit einem entsprechenden Zuschlag gefertigt werden, z. B. für Handzuschnitt.
*   **Fläche / Seitenverhältnis max.**: Höchstmaße für Fläche und Seitenverhältnis für die Positionserfassung. Seitenverhältnis 1:6 bedeutet, dass z. B. bei einer Breite von 600 mm die Höhe höchstens 3600 mm betragen darf. Die Werte werden bei der Positionserfassung geprüft. Bei Überschreitung wird in einer Meldung ein Ausweichartikel vorgeschlagen. Dieser kann dann abgelehnt oder akzeptiert werden. Wenn der Ausweichartikel abgelehnt wird, kann der Auftrag nicht gefertigt werden.
    ⇨ "Ausweichartikel" auf Seite B-595
    Im Register Preis/Zuschlag kann ein Zuschlag angegeben werden, der bei Überschreitung der Maße erhoben wird. Die Werte für die Fläche und Seitenverhältnis sollten sich an den entsprechenden Werten im Register **Preis/Zuschlag** orientieren.
    ⇨ "Produktverwaltung - Preis/Zuschlag" auf Seite B-602
*   **Breite / Höhe Standard**: Die eingetragenen Werte werden bei der Auftragserfassung vorgeschlagen. Sie können im Auftrag überschrieben werden.
*   **Mengeneinheit**: Die Mengeneinheit (Maßeinheit) legt fest, auf welcher Basis das Produkt im Auftrag erfasst und der Preis berechnet wird.

    **Beispiele**
    | Einheit | Beschreibung |
    | :--- | :--- |
    | **qm:** | Auftragserfassung durch Menge, Breite und Höhe. |
    | **Stk:** | Auftragserfassung durch Menge, die Felder für Breite und Höhe sind gesperrt. |
    | **lfm:** | Auftragserfassung als laufende Meter (Menge und Meter). Der Wert für die Länge wird in das Feld Höhe in m (Meter) eingetragen werden. |

    ⇨ "Preis- und Mengeneinheit" auf Seite B-702
*   **Sperrkennzeichen**: Für das Sperrkennzeichen stehen folgende Einträge zur Wahl:
    *   **Nicht gesperrt**: Das Produkt kann im Auftrag erfasst werden.
    *   **Gesperrt**: Das Produkt wird in der Produktsuche nicht angezeigt und kann im Auftrag nicht erfasst werden. Wenn die Produktnummer in der Positionserfassung eingegeben wird, wird eine entsprechende Meldung wird angezeigt.
    *   **Repliziert**: Wenn die Stammdaten nur in der Master-Datenbank (DB) gepflegt werden, können die Daten durch Replikation aktualisiert werden. Stammdaten mit dem Kennzeichen repliziert können in der Slave-DB nicht bearbeitet werden.

**Ausweichartikel / Fremdschlüssel**
*   **Ausweichartikel**: Der Ausweichartikel wird in der Auftragserfassung automatisch vorgeschlagen, wenn beispielsweise bestimmte Restriktionen überschritten wurden. Eine entsprechende Meldung wird dann angezeigt.
*   **Fremdschlüssel**: Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Produktion oder die Finanzbuchhaltung.
*   **Fremdschlüssel Statistik**: Fremdschlüssel für den Datenaustausch mit einer externen Software für statistische Auswertungen.

**Artikelskizze**
*   **Dateiname**: Dateinamen der Grafik, die dem Produkt zugeordnet ist. Diese grafische Darstellung des Produkts kann im Dokument nur gedruckt werden, wenn die Checkbox **Druck auf Formular** aktiviert ist. Dieses Bild gibt nicht das Modell oder die eingebauten Sprossen wieder. Es ist daher nur für seltene Strukturgläser sinnvoll. Der Pfad wird in den Firmendaten > Register System angegeben.
    ⇨ "Pfad zu Produktbildern" auf Seite B-979
*   **Druck auf Formular**: Die Artikelskizze kann in den Formularen gedruckt werden.
    *   ☐ Die Skizze wird nicht in den Formularen gedruckt.
    *   ☑ Die Skizze wird in den Formularen gedruckt.

#### Produktverwaltung – Fertigung

*Stammdaten > Produkte > Artikel > Artikel > Register Fertigung*

[Abbildung: Screenshot des Registers "Fertigung" in der Produktverwaltung]
*Abb. B-373: Produktverwaltung – Fertigung*

In diesem Register legen Sie Parameter für die Fertigung fest, z. B. die Strukturseite oder die Verwendung in einer Stückliste. Die Felder im Bereich **Artikel** sind zum Register **Produkt** beschrieben:
⇨ "Produktverwaltung – Produkt" auf Seite B-591

**Shaping+Nesting - Parameter**
*   **Kantenqualität**: Die Kantenqualität muss dem Produkt zugewiesen werden, damit in der Produktion die richtige Kantenbearbeitung ausgeführt wird. Neben den Standard-Qualitäten können weitere (individuelle) Qualitäten ausgewählt werden, die der Produktion mit derselben Nummer bekannt sein müssen.

**Parameter Stücklisten**
*   **Stückliste nicht relevant für Fertigung**: Die Stückliste kann an die Produktion übergeben werden.
    *   ☑ Die Stückliste wird an die Produktion übergeben. Wählen Sie diese Einstellung, wenn der gesamte Produktaufbau selbst gefertigt wird. Sie können dann beim Erfassen eines Auftrags die Stückliste modifizieren, z. B. eine Scheibe austauschen.
    *   ☐ Die Stückliste wird nicht an die Produktion übergeben. Wählen Sie diese Einstellung, wenn Sie z. B. ein VSG nicht selbst produzieren. Das VSG ist dann ein Bestellartikel. Im Register Lager/Einkauf muss die Beschaffungsart **Bestellung** eingestellt werden.
        ⇨ "Beschaffungsart" auf Seite B-610
*   **Für ISO geeignet**: Ein Produkt kann für einen ISO-Aufbau ungeeignet sein.
    *   ☐ Das Produkt sollte nicht für ISO-Scheiben verwendet werden.
    *   ☑ Das Produkt kann in ISO-Scheiben verwendet werden.
*   **Strukturebene drehbar**: Bei Ornamentgläsern muss angegeben sein, ob die Strukturseite nach innen und außen eingebaut werden kann. Diese Einstellung gilt nicht für beschichtete Gläser.
    *   ☐ Wenn das Glas innen oder außen angebracht wird, ist in der Positionserfassung die Schaltfläche **Strukturebene** freigeschaltet. Dies gilt für Ornamentgläser. Für beschichtete Gläser gibt es in der Positionserfassung eigene Schaltflächen.
    *   ☑ Die Strukturebene kann nicht geändert werden. Das Glas muss immer auf der Standard-Ebene eingebaut werden, die im Bereich **Struktur** festgelegt ist.
    *   ☑ Das Glas kann beliebig eingebaut werden. In der Positionserfassung wird im Register **Stückliste** die Standard-Ebene angezeigt und kann geändert werden.
        ⇨Tutorial 1, "Strukturverlauf" auf Seite B-160
        ⇨ "Struktur, Beschichtung" auf Seite B-600
*   **Wird in Stückliste gedruckt**: Das Produkt in der Stückliste kann im Formular gedruckt wird.
    *   ☐ Das Produkt wird nicht in der Stückliste gedruckt.
    *   ☑ Das Produkt wird im Druck als Stücklisten-Komponente ausgewiesen.

**Standard-Werte für abweichende Mengen**
Wenn Sie mit kaufmännischen Übermengen arbeiten, können Sie zu jedem Produkt angeben, wie viel Prozent der tatsächlich angegebenen Menge als Übermenge produziert werden darf. Das gilt entsprechend für die Angabe der Untermenge. In den Kundendaten muss festgelegt sein, ob der Kunde abweichende Mengen zulässt.
*   **Untermenge, Übermenge**: Prozentwert, z. B. 10 %. Die produzierte Menge darf dann 10% unter oder über der im Auftrag erfassten Menge liegen. Diese Werte können kundenbezogen abweichend eingestellt werden.
    ⇨ "Übermengen" auf Seite B-848

**Abstandhalterkennzeichen**
Bei Produkten der Produktgruppe **Abstandhalter** können Sie weitere Kennzeichen festlegen. Das Abstandhalterkennzeichen aus den Varianten übersteuert das Kennzeichen aus den Produktstammdaten.
*   **Frei**: Zurzeit nicht genutzt.
*   **Verbundtyp**: Typ des Randverbunds, z. B. UV-Randverbund. Die Angabe wird von A+W Production vorgeben.
*   **Rahmentyp**: Nummer des Rahmentyps, z. B. für Edelstahl, TPS, ALU. Die Nummer ist von A+W Production vorgegeben.
*   **Farbe**: Die Farbe wird von A+W Production vorgeben.

**Parameter Fertigung**
*   **AW-Broke**: Fremdschlüssel, der an AWBroke und A+W CAD Designer (Shapes) übergeben wird. Insgesamt stehen elf Fremdschlüssel zur Verfügung, die teilweise fest vorgegeben sind. Für die bekannten Glasarten sind folgende Kennzeichen definiert:
    *   G01: Floatglas
    *   G02: ESG
    *   G03: VSG
    *   G04: Gussglas
    *   G05: Drahtglas
    *   G06: ISO
    *   G07: Ganzglasanlage
    *   G53: VSG-Folie
    *   G99: Metateil

    **Beispiel**
    G028000
    Dies ist ein ESG mit der Produktnummer 8000.

    Der vollständige Schlüssel besteht jeweils aus dem Buchstaben (= Kennzeichen), dem numerischen Anteil der Produktnummer und einem Punkt. Damit können z. B. Bearbeitungen für einzelne Glasarten getrennt von der Standard-Bearbeitung definiert werden. Fremdschlüssel für Farben werden an den Anfang des Glasfremdschlüssels gestellt.

    **Beispiele**
    *   **GF10.028000:** ESG, die zu F10 gehörenden Farbe, Produktnummer 8000.
    *   **KGF15.02111:** Polierung auf ESG mit der zu F15 gehörenden Farbe.
*   **Schlüssel Optimierung**: Der Schlüssel wird zur Klassifizierung an A+W Production übergeben. Sie können eine abweichende Produktnummer (Schlüssel) eingeben, die für die Buchungen im kombinierten Lagerführungsmodus genutzt wird.
    ⇨ "Optimierung" auf Seite B-869
    ⇨ Lagerwirtschaft, "Lagerbuchungen bei kombinierter Lagerführung" auf Seite G-41
*   **Konstruktionstyp**: Die Felder sind nur bei Sprossen oder Bleiverglasung freigeschaltet. Sie können den jeweiligen Konstruktionstyp auswählen. Der Wert wird an A+W Production übergeben. Im ersten Feld tragen Sie den Konstruktionstyp, im zweiten Feld den Sprossentyp ein.
    ⇨ Tutorial 1, "Konstruktionstypen der Sprossen" auf Seite B-162
    ⇨ "Sprossentypen" auf Seite B-573
*   **Maßzuschlag Breite, Höhe**: Kennzeichen für den Zuschlag oder Abzug für Bearbeitungen. Die möglichen Zu- und Abschläge sind im Dialog **Maßzuschlag** hinterlegt.
    ⇨ "Maßzuschlag" auf Seite B-641
    Der Maßzuschlag gleicht den Materialverlust aus, der bei den unterschiedlichen Bearbeitungen entsteht. Der Maßzuschlag wird beim Zuschnitt berücksichtigt.

    **Beispiel**
    Durch Polieren aller vier Kanten reduziert sich ein Float von 1000 x 1000 mm auf die Maße 998 x 998 mm.
    Als Maßzuschlag werden 2 mm angegeben. Die Scheibe wird mit den Maßen 1002 x 1002 mm zugeschnitten.

**Struktur, Beschichtung**
*   **Seite**: Bei Ornamentgläsern und bei beschichteten Gläsern wird angegeben, auf welcher Seite (Ebene) die Struktur oder die Beschichtung liegen soll. Die Angabe kann im Auftrag überschrieben werden.

    **Beispiel**
    Die Strukturebene eines Ornamentglases liegt z. B. standardmäßig außen. Wird ausdrücklich gewünscht, dass sie innen liegen soll, so wird in den meisten Fällen ein sogenannter Strukturinnenzuschlag erhoben.
    Bei beschichtetem Glas liegt die Struktur durch die Produktion bedingt standardmäßig innen.

    ⇨ Tutorial 1, "Strukturen und Beschichtungen" auf Seite B-160
*   **Verlauf**: Bei Ornamentgläsern ist der (Struktur-)Verlauf angegeben. Diese Angabe wird für den Zuschnitt benötigt.
    ⇨ "Struktur" auf Seite B-577
*   **Art**: Die Beschichtung muss oben liegen, um Beschädigungen durch die weitertransportierenden Rollen beim Zuschnitt zu vermeiden. Dies gilt insbesondere für weiche und mittelharte Beschichtungen. Bei harten Beschichtungen kann das Glas auch anders herum aufgelegt werden.

**Druck**
*   **Modellskizze, Sprossenskizze**: Im Formular können schematische oder maßstäbliche Skizzen für Modelle oder Sprossenkonstruktionen gedruckt werden. Die Einstellungen für den Druck können Sie in der Produktverwaltung, in der Positionserfassung und in der Formularverwaltung festlegen. In der Produktverwaltung können Sie den Druck zulassen oder unterbinden. Das Zusammenspiel der Einstellungen ist im Tutorial beschrieben.
    ⇨Tutorial 2, "Skizzendruck" auf Seite B-479
