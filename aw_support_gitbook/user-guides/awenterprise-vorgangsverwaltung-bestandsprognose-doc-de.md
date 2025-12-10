---
description: "DE_AWEnterprise_Verkauf_4_4"
---


# Softwarereferenz Vorgangsverwaltung

**Abstandhalter_Abzug2, Abstandhalter_Abzug3, ...** Abstandhalter-Abzugsmaße der Position in Millimeter bei einem Mehrfach-ISO-Artikel. Summe aus der Höhe des Innenrahmens und der Versiegelungstiefe.

---
## Bestandsprognose

> Verkauf > Auftragserfassung > Positionsebene > Lagerartikel wählen > <F4> > Lager > Lagerprognose

*Abb. D-56 Bestandsprognose*

In diesem Dialog rufen Sie die Bestandsprognose für einen Lagerartikel in einem festgelegten Zeitraum ab.

Standardmäßig wird die Bestandsprognose für den ausgewählten Lagerartikel aus dem Vorgang und dessen Standard-Lager angezeigt.

- Mit `<F12>` löschen Sie die Daten im Kopfbereich und können eine neue Abfrage starten.
- Mit `<F5>` werden zusätzliche Spalten für den Lagerartikel angezeigt.
- Mit `<Shift>` + `<F5>` wird eine grafische Darstellung der Bestandsprognose zu den angegebenen Kriterien in einem eigenen Dialog geöffnet.
  ⇨ "Grafische Darstellung der Bestandsprognose" auf Seite D-154

Sie können die Bestandsprognose für jeden beliebigen Lagerartikel abrufen.

### Kopfbereich

**Artikel** Artikelnummer. Wenn Sie eine Nummer angeben, wird die Bezeichnung des Artikels im Klartext angezeigt.
Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: wls.artnr

**Lager** Lagernummer. Wenn Sie eine Nummer angeben, wird die Bezeichnung des Lagers im Klartext angezeigt. Wenn Sie kein Lager auswählen, wird eine lagerübergreifende Bestandsprognose angezeigt.
Technische Info: numerisches Feld, DB-Feld: wls.Inr

**Variante** Variante des Lagerartikels. Wenn Sie keine Variante auswählen, werden alle Variantenartikel in der Übersicht angezeigt. Das Feld wird nur angezeigt, wenn dem ausgewählten Artikel Varianten zugeordnet sind.
Technische Info: alphanumerisches Feld, DB-Feld: wls.bitnr

**Farbe** Farbvariante des Lagerartikels. Wenn Sie keine Farbe auswählen, werden alle Farbartikel in der Übersicht angezeigt. Das Feld wird nur angezeigt, wenn dem ausgewählten Artikel Farben zugeordnet sind.
Technische Info: alphanumerisches Feld, DB-Feld: wls.farbnr

**Datum** Zeitraum der Bestandsprognose.
Technische Info: Pflichtfeld, Datumsfeld

**Periode...Tage** Intervall der Bestandsprognose in Tagen.
Technische Info: Pflichtfeld, numerisches Feld

**Mengeneinheit** Anzeige der Mengeneinheit, in der die Artikel angezeigt werden. Die Einheit steht in Klammern, z. B. Stück oder Quadratmeter. Die Mengeneinheit wird den einzelnen Artikeln in den Artikelstammdaten zugeordnet.
Technische Info: Anzeigefeld

### Bestände/Bezeichnungen

In diesem Bereich wird die Prognose für den gewählten Lagerartikel angezeigt. Die Spalten Variante und Farbe werden nur angezeigt, wenn dem Lagerartikel Varianten und/oder Farben zugeordnet sind.

- **Lager:**
  Lagernummer.
  Technische Info: Anzeigefeld, DB-Feld: wls.Inr
- **Datum:**
  Fortlaufendes Datum von Anfang bis Ende des angegebenen Zeitraums im festgelegten Intervall.
  Technische Info: Anzeigefeld, Datumsfeld
- **Variante:**
  Variante des Lagerartikels. Die Spalte wird nur angezeigt, wenn dem Lagerartikel Varianten und/oder Farben zugeordnet sind.
  Technische Info: Anzeigefeld, DB-Feld: wls.bitnr
- **Farbe:**
  Farbvariante des Lagerartikels. Die Spalte wird nur angezeigt, wenn dem Lagerartikel Varianten und/oder Farben zugeordnet sind.
  Technische Info: Anzeigefeld, DB-Feld: wls.farbnr
- **Verplant:**
  Verplante Menge des Artikels.
  Technische Info: Anzeigefeld
- **Bestellt:**
  Bestellte Menge des Artikels.
  Technische Info: Anzeigefeld
- **Bestand:**
  Aktuelle Bestandsmenge des Artikels.
  Technische Info: Anzeigefeld, DB-Feld: wlx.g_best

Mit `<F5>` werden zusätzliche Spalten für den Artikel angezeigt. Die Spalten zeigen die Vorgänge, für die der Artikel verplant und/oder bestellt ist:

- **Vorgangsart:**
  Bezeichnung der Vorgangsart:
  - Bestellung
  - Auftrag
  Technische Info: Anzeigefeld, DB-Feld: kauf.vorgang
- **Vorgang:**
  Vorgangsnummer. Je nach Vorgangsart wird entweder die Auftragsnummer oder die Bestellnummer angezeigt.
  Technische Info: Anzeigefeld, DB-Feld: kauf.auftrnr
- **Position:**
  Nummer der Position im Vorgang.
  Technische Info: Anzeigefeld, DB-Feld: kauf.posnr
- **Verplant:**
  Verplante Menge des Artikels im Vorgang. Die verplante Menge wird automatisch berechnet.
  Technische Info: Anzeigefeld
- **Bestellt:**
  Bestellte Menge des Artikels im Vorgang. Die bestellte Menge wird automatisch berechnet.
  Technische Info: Anzeigefeld

### Fußbereich

**Grafik**
Öffnet eine grafische Darstellung der Bestandsprognose zu den angegebenen Kriterien in einem eigenen Dialog.

### Grafische Darstellung der Bestandsprognose

In diesem Dialog wird eine grafische Darstellung der Bestandsprognose zu den angegebenen Kriterien angezeigt.

**(x-Achse)** Skala für den ausgewählten Zeitraum der Bestandsprognose. Die Einheit für den Zeitraum sind Tage, als Datum angegeben. Der Abstand zwischen den Tagen entspricht dem ausgewählten Intervall im Feld Periode...Tage im Dialog Bestandsprognose. Es werden maximal 15 Tage mit dem entsprechenden Datum angezeigt.
Es kann sein, dass nicht der gesamte ausgewählte Zeitraum dargestellt wird, weil er mehr als 15 Tage umfasst. In diesem Fall können Sie die Tageszahl für das Intervall vergrößern, oder einen kleineren Zeitraum auswählen.

**(y-Achse)** Skala der Artikelmenge. Die Mengeneinheit steht in Klammern, z. B. Stück oder Quadratmeter.

**MB** Mindestbestand des Artikels.

**AB** Alarmbestand des Artikels.

**Bestand** Bestandsmenge des Artikels.

## Produktaustausch

> Verkauf > Auftragserfassung > Positionsebene, Fußbereich > <F4> > Produktangaben > Produktaustausch

In diesen Dialogen können Sie den Produktaufbau ändern, indem Sie die Artikel innerhalb der Stücklisten austauschen. Sie können die Stücklisten gleichzeitig für andere Positionen mit identischer Stücklistennummer austauschen.

In diesem Abschnitt sind folgende Dialoge erklärt:

- "Produktaustausch" auf Seite D-155
- "Produktaustausch für Positionen" auf Seite D-157

*Abb. D-57 Produktaustausch*

In diesem Dialog ändern Sie den Produktaufbau, indem Sie Artikel im Stücklistenaufbau austauschen. Die Stückliste, die Sie bearbeiten wollen, wählen Sie anhand der Stücklistennummer in den Auftragspositionen aus. Wenn mehrere Positionen mit identischer Stücklistennummer erfasst sind, können Sie die Stücklisten dieser Positionen gleichzeitig bearbeiten.

Wenn Sie auswählen möchten, in welche Positionen mit identischer Stücklistennummer die Stücklisten ausgetauscht werden sollen, dann können Sie das in dem Dialog Produktaustausch für Positionen für jede Position einzeln angeben.

- Mit **[Start]** bestätigen Sie den Austausch.
- Wenn Sie eine Stückliste bearbeiten, die in mehreren Positionen identisch ist, wird nach Bestätigung des Austauschs eine Meldung angezeigt, ob der Austausch für alle Positionen mit dieser Stücklistennummer gelten soll:
  - Mit **[Ja]** werden die Artikel in allen Positionen mit derselben Stücklistennummer ausgetauscht.
  - Mit **[Nein]** öffnet sich der Dialog Produktaustausch für Positionen. Sie können in der Spalte Neu angeben, in welchen Positionen die Artikel ausgetauscht werden. Mit **[Start]** bestätigen Sie den Austausch.
    ⇨ "Produktaustausch für Positionen" auf Seite D-157

**Bearbeitungen neu erfassen**
> Wenn Sie eine Scheibe mit Bearbeitungen austauschen, dann wird die Bearbeitung aus der Stückliste entfernt. Wenn Sie die Bearbeitung hinzufügen möchten, dann können Sie diese für die Austauschscheibe neu erfassen.
> ⇨ "Stücklistendarstellung - Stücklistenaufbau" auf Seite D-196

**Alte Stückliste, Typ** Nummer der Stückliste, die Sie austauschen oder bearbeiten wollen. Die Stücklistennummern sind zu den Positionen in der Spalte SLNr zum Register Allgemein aufgelistet. Wenn Sie eine Nummer angeben, wird der Kopfartikel mit der Stückliste automatisch im Klartext angezeigt.
Technische Info: Pflichtfeld, alphanumerisches Feld, DB-Feld: kpos.poskonr
⇨ "Auftragspositionen - Allgemein" auf Seite D-113

**Alter Artikel** Anzeige der Nummer und der Bezeichnung des Artikels, der ausgetauscht oder bearbeitet wird. Wenn der Artikel mehrere Scheiben hat, werden die Artikelnummern und Bezeichnungen der Glascheiben angezeigt.
Technische Info: Anzeigefeld, DB-Feld: kpos.artnr

**Kundenartikel** Anzeige der kundenspezifische Artikelbezeichnung des auszutauschenden Artikels.
Technische Info: Anzeigefeld, DB-Feld: kpos.kuposnr

**Austauschartikel** Nummer und Bezeichnung des neuen Artikels, der gegen den alten Artikel ausgetauscht wird. Wenn Sie nicht den kompletten Artikel, sondern den Scheibenaufbau eines Artikels bearbeiten wollen, können Sie die alte Artikelnummer als Nummer des neuen Artikels angeben. Wenn Sie eine Nummer angeben, wird die Bezeichnung im Klartext angezeigt. Sie können die Bezeichnung überschreiben.
Technische Info: numerisches Feld, alphanumerisches Feld, DB-Feld: aufstrukt.artnr

**Kundenartikel** Externe Bestellnummer des Kunden für den Austauschartikel. Wenn Sie einen Kundenartikel angeben, wird der Austauschartikel überschrieben.
Technische Info: alphanumerisches Feld

**Originalaufbau** Anzeige des Aufbaus des neuen Artikels im Original-Zustand. Wenn Sie eine Nummer für den Austauschartikel angeben, wird der Originalaufbau im Klartext angezeigt.
Technische Info: Anzeigefeld

**Wunschaufbau** Aufbau des Artikels nach Wunsch des Kunden. Wenn Sie eine Nummer für den Austausch- oder Kundenartikel angeben, werden die Felder automatisch mit dem originalen Scheibenaufbau des Artikels gefüllt. Sie können eine oder mehrere Scheiben ändern. Die Felder sind nur bei Austauschartikeln mit mehreren Scheiben freigeschaltet.
Technische Info: numerische Felder

**Zusatzartikel** Nummer des Zusatzartikels, z. B. für ein Zubehörteil oder eine Bearbeitung. Die Auswahl eines Zusatzartikels ist optional.
Technische Info: numerisches Feld

### Produktaustausch für Positionen

> Verkauf > Auftragserfassung > Positionsebene, Fußbereich > <F4> > Produktangaben > Produktaustausch > Austausch starten > Austausch für alle Positionen verneinen

*Abb. D-58 Produktaustausch für Positionen*

In diesem Dialog können Sie angeben, in welchen Positionen mit gleicher Stücklistennummer die Stücklisten ausgetauscht werden sollen.

- Mit `<Toggle>` wählen Sie in der Spalte Neu zwischen J für Ja, Stückliste austauschen oder N für Nein, Stückliste nicht austauschen.
- Mit **[Start]** bestätigen Sie den Austausch.

#### Kopfbereich

Die Felder und Schaltflächen im Kopfbereich sind zum Dialog Produktaustausch beschrieben:
⇨ "Produktaustausch" auf Seite D-155

#### Positionsbereich

- **Pos:**
  Anzeige der Positionsnummer in der Auftragserfassung.
  Technische Info: Anzeigefeld, DB-Feld: kpos.Ifdpos
- **Artikel:**
  Anzeige der Artikelnummer.
  Technische Info: Anzeigefeld, DB-Feld: kpos.artnr
- **SL:**
  Anzeige der Stücklistennummer des Artikels.
  Technische Info: Anzeigefeld, DB-Feld: kpos.poskonr
- **Kundenartikel:**
  Anzeige der kundenspezifischen Artikelbezeichnung des auszutauschenden Artikels.
  Technische Info: Anzeigefeld, DB-Feld: kpos.kuposnr
- **Maß 1:**
  Anzeige der Breite in Millimeter.
  Technische Info: Anzeigefeld, DB-Feld: kpos.laenge
- **Maß 2:**
  Anzeige der Höhe in Millimeter.
  Technische Info: Anzeigefeld, DB-Feld: kpos.breite
- **Maß 3:**
  Anzeige des Scheibenzwischenraums in Millimeter.
  Technische Info: Anzeigefeld, DB-Feld: kpos.szr
- **Neu:**
  Angabe, ob die Stückliste des Artikels ausgetauscht werden soll.
  - J: Stückliste austauschen
  - N: nicht austauschen
  Technische Info: Toggle-Feld

## Reklamation

> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > <Ende> > Feld Nettototal > Werteingabe 0 > <Enter>

*Abb. D-59 Reklamation*

In diesem Dialog geben Sie die Daten für die Reklamation an. Die Reklamationsdaten können statistisch ausgewertet werden.

Je nach Konfiguration wird nach Eingabe des Werts 0 im Feld Nettototal eine Abfrage angezeigt, ob Sie den Vorgang überarbeiten wollen. Der Dialog Reklamation wird nur angezeigt, wenn Sie auf [Nein] klicken.

Alternativ geben Sie die Reklamationsdetails in der Auftragserfassung im Register Verschiedenes an.

Die Felder sind ausführlich zum Register Auftragserfassung – Verschiedenes beschrieben.
⇨ "Auftragserfassung - Verschiedenes" auf Seite D-99

## Auftragsarten

> Verkauf > Auftragserfassung > Feld Eingang, Rechnungstyp, Objekt > <Strg> + <F12>

*Abb. D-60 Auftragsarten*

In diesem Dialog wählen Sie eine Auftragsart aus. Standardmäßig ist der normale Auftrag als Auftragsart ausgewählt. Wenn Sie eine andere Auftragsart wählen, wird diese als Dialog-Name in der Kopfzeile des Dialogs angezeigt.

- **Normaler Auftrag:**
  Voreingestellter Standard der Auftragserfassung.
- **Hausinterner Auftrag:**
  Interner Auftrag im eigenen Haus. Der Auftrag wird nicht an die Versandsteuerung übergeben und kann nicht abgerechnet werden. Er wird zur internen Auftragsabwicklung zwischen dem eigenem und einem anderen Haus genutzt. Der Auftrag kann im eigenen Haus abgeschlossen werden. Im Zielhaus wird der Auftrag als normaler Auftrag erfasst.
- **Gruppeninterner Auftrag:**
  Interne Auftragsabwicklung zwischen zwei Häusern. Der Auftrag wird im Zielhaus als normaler Auftrag berechnet.
- **Abrufauftrag:**
  Auftrag auf Abruf. Wird nicht mehr genutzt. Für die Reservierung von Kapazitäten in A+W Production muss die Auftragsart Reservierungsauftrag gewählt werden.
- **Lagerauftrag:**
  Produktionsauftrag für das eigene Lager, ohne Rechnung. Ein Lagerauftrag wird bei Unterbelegung des Lagers erfasst. Nach der Fertigmeldung aus A+W Production muss der Wareneingang gebucht werden. Je nach Konfiguration werden Lageraufträge automatisch vom System erzeugt.
- **Kostenloser Auftrag:**
  Reklamationsauftrag. Ein kostenloser Auftrag wird erfasst, wenn der Rechnungsbetrag gleich Null und der Positionsbetrag ungleich Null ist. Am Ende der Erfassung öffnet sich ein Dialog zur Angabe des Reklamationsgrundes.
  ⇨ "Reklamation" auf Seite D-158
- **Reservierungsauftrag:**
  Auftrag, der Kapazitäten in A+W Production reserviert, z. B. wenn die genauen Maße für die Auftragspositionen fehlen.
  Reservierungsaufträge können mit den bekannten Auftragsdaten bereits eingelastet werden. Er wird nicht an die Versandsteuerung übergeben.
  Wenn die genauen Auftragsdaten vom Kunden vorliegen, werden diese in den bestehenden Auftrag eingepflegt, die Auftragsart zu normaler Auftrag gewechselt und der Auftrag wird erneut freigegeben.
- **Kalkulationstyp:**
  Der Kalkulationstyp dient zur Bestimmung eines VK-Preises auf Basis der Herstellungskosten. Für diese Auftragsart muss die Kostenkalkulation aktiv sein. Der Kalkulationstyp ist nur kundenspezifisch konfiguriert.
- **Chef-Auftrag:**
  Auftrag, der mit höherer Priorität in A+W Production eingelastet wird. Im Umlastungseditor kann der Auftrag mit normaler oder mit höchster Priorität bearbeitet werden. Aufträge mit höchster Priorität werden mit minimalen Übergangszeiten eingelastet. Sie werden auch dann noch vom System verplant, wenn keine Produktionskapazität mehr zur Verfügung steht. Sie können Chef-Aufträge nur mit den entsprechenden Rechten erfassen und bearbeiten.
- **Ersatz-Auftrag:**
  Kundenspezifischer Auftrag, z. B. um Ersatz- oder Grantieansprüchen nachzukommen. Der Ersatz-Auftrag wir wie ein normaler Auftrag berechnet und eingelastet. Ob der Auftrag kostenlos geliefert wird, entscheidet der Kundenbetreuer. Für statistische Auswertunge werden Informationen zu dem Ersatzauftrag, z. B. die Referenz zum Originalauftrag, gespeichert.
- **Versand-Auftrag:**
  Auftrag, der nicht an die Produktion sondern direkt an die Versandsteuerung übergeben wird. Das System muss entsprechend konfiguriert sein.
- **Referenz-Preisliste:**
  Angebots-Übersicht, um eine kundenspezifische Preisliste anzuzeigen. Die Preisliste kann vom Kunden auf einem Internetportal eingesehen werden. Sie können eine Referenz-Preisliste nur mit den entsprechenden Rechten erfassen und wenn die Schnittstelle iska-Filter aktiv ist.
- **Rücknahme-Auftrag:**
  Kundenspezifischer Auftrag, z. B. um Gutschriften zu bearbeiten. Für Rücknahmeaufträge ist als Wunschtermin immer das aktuelle Datum vordefiniert und die Auftragssumme ist gleich Null. Rücknahmeaufträge werden nach Freigabe nicht an die Produktion sondern nur an den Versand übergeben. Sie können eine Rücknahmeauftrag nur mit den entsprechenden Rechten erfassen, bearbeiten und/oder freigeben.

## Artikelangaben für bemaßte Varianten

> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Preisfeld > <Shift> + <F8> > [Ja] > Auftrag speichern und schließen

*Abb. D-61 Artikelangaben für bemaßte Varianten*

In diesem Dialog können Sie die im Auftrag erfasste Position zusammen mit ihrer Stückliste und den Maßen fixieren, um Sie später in anderen Vorgängen erfassen zu können. Der Dialog Artikelangaben für bemaßte Varianten öffnet sich erst, wenn Sie einen Auftrag mit Artikeln, die für die Produktfixierung gekennzeichnet sind, speichern und schließen. Wenn Sie mehrere Positionen für die Produktfixierung gekennzeichnet haben, öffnet sich nacheinander für jede Position jeweils ein Dialog.

Wenn Sie einen Artikel mit `<Shift> + <F8>` für die Fixierung kennzeichnen, wird neben der Position ein gelber Stern angezeigt. Bereits fixierte Artikel sind mit einem grünen Stern gekennzeichnet.
⇨ "Symbolerklärung" auf Seite D-76

Sie speichern fixierte Artikel kunden- oder lieferantenindividuell unter einer neuen Artikelnummer in den Stammdaten:

- Mit `<F2>` wechseln Sie im Fußbereich die Ansicht für ein lieferantenindividuelles oder ein kundenindividuelles Produkt.
- Mit `<Ende>` speichern Sie den festbemaßten Artikel ab.

### Kopfbereich

In diesem Bereich werden die Positionsnummer des Artikels, der für die Fixierung gekennzeichnet ist, die Artikelnummer und der Originalaufbau des Artikels mit Bearbeitungen angezeigt.

### Artikelangaben

**Artikel (neu)** Neue Artikelnummer für den fixierten Artikel. Mit `<F6>` vergeben Sie die nächste freie Artikelnummer.
Technische Info: numerisches Feld, DB-Feld: artikel.artnr

**Matchcode** Alphanumerischer Matchcode. Standardmäßig wird der Matchcode des alten Artikels übernommen. Sie können den Code bearbeiten.
Technische Info: alphanumerisches Feld, DB-Feld: artikel.artmc

**Warengruppe** Kennzeichen der Warengruppe. Standardmäßig wird die Warengruppe des alten Artikels übernommen. Sie können die Warengruppe bearbeiten.
Technische Info: alphanumerisches Feld, DB-Feld: artikel.wagrp

**Hauptbezeichnung** Hauptbezeichnung des Artikels. Standardmäßig wird die Hauptbezeichnung des alten Artikels übernommen. Sie können die Bezeichnung bearbeiten.
Technische Info: alphanumerisches Feld, DB-Feld: artikel.artbez1

**Nebenbezeichnung** Nebenbezeichnung des Artikels. Standardmäßig wird die Nebenbezeichnung des alten Artikels übernommen. Sie können die Bezeichnung bearbeiten.
Technische Info: alphanumerische Felder, DB-Felder: artikel.artbez2, artikel.artbez3

### Falls kundenindividuelles Produkt

Die Kundenangaben sind zur Erfassung eines bemaßten Kundenproduktes notwendig.

**Kunde** Kundennummer und Kundenname. Standardmäßig ist der Kunde ausgewählt, für den Sie den Vorgang erfasst haben. Sie können eine andere Kundennummer eintragen, um den Artikel für einen anderen Kunden anzulegen. Wenn Sie eine Nummer angeben, wird der Kundenname automatisch im Klartext angezeigt.
Wenn Sie im Feld Kunde die Nummer löschen, wird der Artikel für alle Kunden angelegt.
Technische Info: numerisches Feld, DB-Feld: arkuzu.kunr

**Artikel** Neue Artikelnummer für den kundenspezifischen Artikel.
Technische Info: alphanumerisches Feld, DB-Feld: arkuzu.kuartnr

**Artikelbezeichnung** Neue Artikelbezeichnung für den kundenspezifischen Artikel.
Technische Info: alphanumerisches Feld, DB-Feld: arkuzu.kuartbez

**VK-Preis (netto) Preis/Stück** Kundenspezifischer Netto-Verkaufs-Preis pro Stück.
Technische Info: numerisches Feld, DB-Feld: kuartprs.preis1

**EK-Preis (brutto) Preis/Stück** Kundenspezifischer Brutto-Einkaufs-Preis pro Stück.
Technische Info: numerisches Feld, DB-Feld: kuartprs.ekpreis

### Falls lieferantenindividuelles Produkt

Die Lieferantenangaben sind zur Erfassung eines bemaßten Lieferantenprodukts notwendig.

**Lieferant** Lieferantennummer und Name des Lieferanten. Standardmäßig ist der Lieferant ausgewählt, für den Sie den Vorgang erfasst haben. Sie können eine andere Lieferantennummer eintragen, um den Artikel für einen anderen Lieferanten anzulegen. Wenn Sie eine Nummer auswählen, wird der Lieferantenname automatisch im Klartext angezeigt.
Wenn Sie im Feld Lieferant die Nummer löschen, wird der Artikel für alle Lieferanten angelegt.
Technische Info: numerisches Feld, DB-Feld: arliefzu.linr

**Artikel** Neue lieferantenspezifische Artikelnummer, d. h. Lieferanten-Artikelnummer.
Technische Info: alphanumerisches Feld, DB-Feld: artliefzu.artnr

**Artikelbezeichnung** Neue lieferantenspezifische Artikelbezeichnung.
Technische Info: alphanumerisches Feld, DB-Feld: artliefzu.exartnr

**Preis (netto) Preis/Stück** Lieferantenspezifischer Nettopreis pro Stück.
Technische Info: numerisches Feld, DB-Feld: artliefzu.preis

## Varianten- und Farben-/Dickenauswahl

> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Lagermaß-Artikel wählen > Menge eingeben > <Enter>

*Abb. D-62 Varianten- und Farben-/Dickenauswahl*

In diesem Dialog wählen Sie die Maßvariante oder die Farb- und/oder Größenvariante des Artikels. Der Dialog öffnet sich automatisch, wenn für den gewählten Artikel mindestens eine Maß-, Farb- oder Größenvariante in den Artikelstammdaten angelegt ist.

- **Code:**
  Nummer des Variantenartikels.
  Technische Info: Anzeigefeld, DB-Feld: artvarzu.bitnr oder artvarmdzu.bitnr
- **Art:**
  Art der Variantenzuordnung. Diese Information ist nur bei interner Mandantentrennung relevant. Sie können in den Stammdaten hausspezifische Varianten anlegen.
  - Allgemein: Es stehen hausübergreifende Angaben zur Verfügung.
  - Mandantenbezogen: Es stehen hausspezifische Angaben zur Verfügung.
  Technische Info: Anzeigefeld
- **Variante:**
  Bezeichnung des Variantenartikels.
  Technische Info: Anzeigefeld
- **Lagerbez.:**
  Bezeichnung eines Stückes im Lager. Diese Spalte wird nur bei Artikeln mit Maßvariante angezeigt.
  Technische Info: Anzeigefeld
- **Bestand:**
  Aktueller Lagerbestand.
  Technische Info: Anzeigefeld
- **Beschaffung:**
  Beschaffungsart des Variantenartikels.
  Technische Info: Anzeigefeld
- **Lieferant:**
  Name des Standardlieferanten des Variantenartikels. Der Lieferant wird nur angezeigt, wenn die Beschaffungsart der Auftragsposition in den Artikelstammdaten auf Zukauf gesetzt ist.
  Technische Info: Anzeigefeld, DB-Feld: artvarzu.stdlinr oder artvarmd-zu.stdlinr
- **Standardlager:**
  Standardlager für den Variantenartikel. Diese Spalte wird nur bei Artikeln mit Farb-/ oder Größenvariante angezeigt.
  Technische Info: Anzeigefeld, DB-Feld: artvarzu.lager oder artvarmdzu.lager
- **Std.:**
  Anzeige, ob die Variante in den Artikelstammdaten als Standardvariante für den Artikel festgelegt ist. Diese Spalte wird nur bei Artikeln mit Farb-/ oder Größenvariante angezeigt.
  - ☐ Die Farb-/Größenvariante ist die Standardvariante für diesen Artikel.
  - ☑ Die Farb-/Größenvariante ist keine Standardvariante.
  Technische Info: Checkbox, Anzeigefeld

## Private Felder

> Verkauf > Auftragserfassung > Positionsebene > <F4> > Private Felder

*Abb. D-63 Private Felder*

In diesem Dialog geben Sie marktpartnerindividuelle Artikelangaben und artikelbezogene private Felder an.

Im oberen Bereich des Dialogs geben Sie je nach Beschaffungsart des Artikels die kunden- oder lieferantenspezifischen Angaben zum Artikel an.

Die Felder im unteren Bereich des Dialogs sind frei konfigurierbar.

Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

## Fremddaten-Import

> Verkauf > Auftragserfassung > Positionsebene > Feld Artikel > <Strg> + <L>

*Abb. D-64 Fremddaten-Import*

In diesem Dialog können Sie Daten aus einem externen Tabellenkalkulationsprogramm in A+W Enterprise importieren.

Pro Zeile können Sie eine Position mit verschiedenen Daten in bis zu zehn Spalten importieren. Welche Daten in den Spalten stehen, legen Sie in der Kopfzeile der Tabelle fest. Sie können zwischen zehn verschiedenen Kopffeldern wählen. Sie müssen mindestens die vier Pflichtfelder Artikel, Menge, Breite und Höhe in der Kopfzeile wählen, wenn Sie den Datenimport starten wollen. Wenn Sie die Felder nicht gewählt haben, wird eine Meldung mit einem entsprechenden Hinweis angezeigt.

Um die Daten zu importieren, müssen Sie die entsprechenden Zeilen und Spalten mit den Daten im Tabellenkalkulationsprogramm markieren und in die Zwischenablage kopieren.

Mit **[Import]** fügen Sie die Daten in den Dialog Fremddaten-Import in A+W Enterprise ein. Wenn Sie die Daten importiert haben, wird eine Abfrage angezeigt, ob Sie die bestehende Spaltenzuordnung beibehalten wollen. Mit **[Ja]** wird geprüft, ob die importierten Daten und die Formatvorgaben für die zugehörigen Felder im Kopfbereich übereinstimmen. Mit **[Nein]** können Sie die Felder in der ersten Zeile bearbeiten. Mit `<Ende>` schließen Sie die Bearbeitung ab und die importierten Daten werden geprüft.

Wenn die Daten die Vorgaben des jeweiligen Feldes erfüllen, wird vor der Position eine angewählte Checkbox angezeigt. Wenn die Daten fehlerhaft sind, wird ein rotes Kreuz angezeigt. Sie können Positionen nur in den Vorgang übernehmen, wenn das Datenformat aller Felder in der Positionszeile die Vorgaben erfüllt.

### Kopfbereich

**AWE Produkt** Anzeige der Artikelnummer und -bezeichnung des Kopfartikels, der im Feld Artikel in der Vorgangserfassung markiert ist. Wird der Import wiederholt, wird die Artikelnummer des zuletzt importierten Artikels angezeigt. Je nach Artikel werden weitere Artikelinformationen angezeigt, z. B. Wenn Sie die erste Position erfassen und noch keine Artikelnummer im Feld Artikel in der Vorgangserfassung angegeben haben, werden keine Informationen angezeigt.
Technische Info: Anzeigefeld

### Tabelle

In den zehn ersten Feldern in der Kopfzeile geben Sie an, welche Daten in der jeweiligen Spalte in der Tabellen erfasst werden. Mit `<Toggle>` wählen Sie zwischen den möglichen Feldbezeichnungen:

- **LfdPos:** Positionsnummer.
- **Ku.Pos:** Kunden-Positionsbezeichnung.
- **Artikel:** Artikelnummer.
- **Ku.Artikel:** Kunden-Artikelnummer.
- **Kommis.:** Kommissionstext.
- **Menge:** Positionsmenge.
- **Breite:** Breite in Millimeter.
- **Höhe:** Höhe in Millimeter.
- **SZR:** Scheibenzwischenraum in Millimeter.
- **SZR2:** Zweiter Scheibenzwischenraum in Millimeter bei Mehrfach-ISO-Gläsern.

Die Felder sind ausführlich zum Dialog Auftragspositionen beschrieben:
⇨ "Auftragspositionen" auf Seite D-113

Alternativ können Sie den Anfangsbuchstaben der Feldbezeichnung eingeben, z. B. `<a>` für Artikel. Wenn mehrere Feldbezeichnungen mit dem eingegebenen Buchstaben beginnen, wechseln Sie mit erneutem Drücken der Buchstabentaste zu der nächsten Feldbezeichnung mit diesem Anfangsbuchstaben, z. B. `<s>` für SZR, `<s>`, `<s>` für SZR2.

In der letzten Spalte der Tabelle wählen Sie:
**J/N:** Angabe, ob die Zeile mit den Daten zur Position in den Vorgang übernommen werden soll.
- ☑ Die Positionsdaten in der Zeile werden in den Vorgang übernommen.
- ☐ Die Positionsdaten in der Zeile werden nicht in den Vorgang übernommen.

In den Feldern in der Tabelle werden die Daten angezeigt, die Sie aus dem Tabellenkalkulationsprogramm importieren. Sie können die importierten Daten bearbeiten.

Mit **[Übernehmen]** werden die Daten in den Vorgang übernommen.

### Fußbereich

**Import** Importiert die Daten aus der Zwischenablage.
**Zuordnung** Wechselt in die Kopfzeile der Tabelle, in der Sie die Spaltenzuordnung bearbeiten können.
**Test** Prüft, ob die importierten Daten den Formatvorgaben der entsprechenden Felder entspricht.
**Übernehmen** Übernimmt die Daten aus den Zeilen, in denen die Checkboxen aktiv sind, in den Vorgang.
**Löschen** Löscht die importierten Daten aus der Tabelle.

## Dokumentenarten

> Verkauf > Auftragserfassung > Kopf-, Fußbereich > <Shift> + <F4> > Dokumentenarten

*Abb. D-65 Dokumentenarten*

In diesem Dialog können Sie die Ausgabeart und die Formularausgabe der verschiedenen Dokumentearten bearbeiten.

- **Art:**
  Anzeige der Schlüsselnummer der Dokumentenart.
  Technische Info: Anzeigefeld, DB-Feld: kaufdokutype.dokuart
- **Bezeichnung:**
  Anzeige der Bezeichnung der Dokumentenart.
  Technische Info: Anzeigefeld, DB-Feld: xdokutype.dokubez
- **Dokumententyp:**
  Anzeige des Dokumententyps, z. B. Leistungserklärung.
  Technische Info: Anzeigefeld, DB-Feld: xdokutype.dokutyp
- **Art der Ausgabe:**
  Ausgabeart des Dokuments, z. B. per E-Mail.
  Technische Info: Toggle-Feld, DB-Feld: kaufdokutype.ausgabeart
- **Formulare:**
  Formularart, bei der die Dokumente ausgegeben werden sollen. Sie können eine oder mehrere Formulararten wählen.
  Technische Info: Auswahl-Feld, DB-Feld: kaufdokutype.formular
- **Prod:**
  Angabe, ob die Daten an die Produktion übergeben werden:
  - ☑ Die Daten werden übermittelt.
  - ☐ Die Daten werden nicht übermittelt.
  Technische Info: Checkbox, DB-Feld: kaufdokutype.prodflag

## Dokumentenartenzuordnung

> Verkauf > Auftragserfassung > Feld Termin > <Strg> + <K>
> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Menge > <Strg> + <K>

*Abb. D-66 Dokumentenartenzuordnung*

In diesem Dialog ordnen Sie einem Vorgang oder einzelnen Positionen Dateien zu. Wenn Sie die Datei dem kompletten Vorgang zuordnen wollen, müssen Sie den Dialog im Kopfbereich öffnen. Wenn Sie die Datei einer bestimmten Position in dem Vorgang zuordnen wollen, müssen Sie den Dialog auf Positionsebene in der Vorgangserfassung zu der entsprechenden Position öffnen.

Zuerst müssen Sie eine Serveradresse einrichten, wo die Dateien abgelegt werden. Diese Adresse muss über eine Umgebungsvariable definiert sein, damit sie dem System bekannt ist. Wenn dem Vorgang bereits Dateien zugeordnet wurden, werden diese im Dialog Dokumentenartenzuordnung angezeigt.

Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

Wenn Sie einsehen wollen, ob und welche Dateien dem Vorgang oder den Positionen zugeordnet sind, dann müssen Sie die Dokumentenartenzuordnung jeweils für den Vorgang oder die entsprechende Position öffnen. Wenn Sie den Dialog auf Positionsebene öffnen, werden Dokumente, die dem kompletten Vorgang zugeordnet sind, nicht angezeigt, sondern nur die Dokumente, die dieser Position zugeordneten sind.

- **Pos:**
  Positionsnummer, der die Datei zugeordnet ist. Wenn die Datei dem Vorgang zugeordnet ist, ist das Feld leer. Sie können dieses Feld nicht bearbeiten.
  Wenn Sie eine Datei einem Auftrag zuordnen, wird das Feld kaufref.posnr in der Datenbanktabelle mit dem Wert 0 gespeichert.
  Technische Info: numerisches Feld, DB-Feld: kaufref.posnr
- **DokArt, Bezeichnung:**
  Nummer und Bezeichnung der Dokumentenart, der das Dokument zugeordnet ist, z. B. Bilder/Skizzen. Wenn Sie im Feld DokArt eine Nummer angeben, wird die Bezeichnung im Klartext angezeigt. Wenn keine Nummer angegeben ist, wird als Bezeichnung standardmäßig allgemein angezeigt.
  Technische Info: numerisches Feld, Toggle-Feld, DB-Feld: kaufref.dokuart
- **Datei:**
  Name der Datei, die dem Vorgang oder der Position zugeordnet ist. Wenn Sie eine Datei zuordnen wollen, müssen Sie die entsprechende Datei aus Ihrem Explorer per Drag-and-Drop auf das Ordner-Symbol in der linken unteren Ecke des Dialogs ziehen. Das Ordner-Symbol ist nur aktiv, wenn der Cursor im Feld Datei steht.
  Technische Info: Pflichtfeld, Auswahl-Feld, DB-Feld: kaufref.datei
- **Sprache:**
  Auswahl der Sprache der Datei.
  Technische Info: Auswahl-Feld, DB-Feld: kaufref.sprkz
- **Art der Ausgabe:**
  Über dieses Feld steuern Sie die Ausgabeart:
  - **keine:** Der Marktpartner erhält keine Dokument.
  - **per E-Mail:** Der Marktpartner erhält das Dokument zusätzlich zum Formular per Mail.
  Technische Info: Toggle-Feld, DB-Feld: kaufref.ausgabeart
- **Formulare:**
  Auswahl der Formulare, z. B. Auftragsbestätigung, Lieferschein, bei denen das Dokument zusätzlich per Mail versendet wird, wenn bei Art der Ausgabe die Ausgabeart per E-Mail festgelegt ist. Sie können keine, eine oder mehrere Formulare auswählen.
  - Mit `<F9>` öffnen Sie den Dialog Formulare.
  - Mit den Pfeiltasten navigieren Sie zwischen den Formularen.
  - Mit `<Toggle>` markieren Sie ein Formular.
  - Mit `<Ende>` schließen Sie den Dialog und übernehmen die Auswahl.
  Technische Info: Auswahl-Feld, DB-Feld: kaufref.formular
- **Prod:**
  Angabe, ob das Dokument an die Produktion übergeben werden soll:
  - ☑ Das Dokument wird an die Produktion übermittelt.
  - ☐ Das Dokument wird nicht übermittelt.
  Technische Info: Checkbox, DB-Feld: kaufref.prodflag
- **O/L:**
  Anzeige, wie das Dokument angehängt ist. Wenn Sie eine Datei anhängen, wird das Feld vom System automatisch ausgefüllt.
  - **O:** Das Dokument ist als Original angehängt.
  - **L:** Der Dateiname und der Link zum Dokument werden angehängt. Der Link darf nicht länger als 200 Zeichen sein.
  Technische Info: Anzeigefeld
- **Entf.:**
  Angabe, ob ein Dokument gelöscht werden soll. Erst nach Abschluss der Vorgangserfassung wird das markierte Dokument aus dem Dialog entfernt.
  - ☑ Das Dokument soll gelöscht werden.
  - ☐ Das Dokument soll nicht gelöscht werden.
  Technische Info: Checkbox

> **Verworfene Vorgänge mit Dateizuordnungen**
> Wird ein neu angelegter Vorgang mit Dateizuordnungen nicht gespeichert sondern verworfen, bleiben die Dateien an dem gewählten Speicherort gespeichert.

## Dateizuordnung

> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld B.Art > <Strg> + <F8> > Bearbeitung markieren > Register Alle Parameter/Skizze > [Motiv(Indiv)]

*Abb. D-67 Dateizuordnung*

In diesem Dialog wählen Sie die Motivdatei aus oder ändern Sie sie Auswahl, die Sie einer Oberflächenbearbeitung zuordnen wollen.

Wenn Sie eine Motivdatei zuordnen wollen, müssen Sie die entsprechende Datei aus Ihrem Explorer per Drag-and-Drop auf das Ordner-Symbol im Dialog ziehen. Mit [OK] wird die Motivdatei in die gewählte Bearbeitung übernommen.

## DXF Import

> Verkauf > Auftragserfassung > Register Positionen > Register Eigensch. > Feld CAD Datei > <F9> > Dateiart DXF auswählen > <Enter> > DXF-Datei auswählen > [Open]

*Abb. D-68 DXF Import*

In diesem Dialog wird eine Vorschau der gewählten DXF-Datei angezeigt. Sie können einige der Parameter für die Bearbeitung anpassen. Welche Parameter Sie bearbeiten können ist von der Systemkonfiguration abhängig.

## Änderungs-Protokoll

> Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > <Shift> + <F4> > Änderungs-Protokoll

*Abb. D-69 Änderungs-Protokoll*

In diesem Dialog werden alle Änderungen des Vorgangs in einem Protokoll angezeigt.

**Sachbearbeiter** Name des Sachbearbeiters.
Technische Info: Anzeigefeld

### Freischaltung

- **Haus:**
  Mandantennummer (Hausnummer).
- **Mitarbeiter:**
  Name des Mitarbeiters.
- **Datum:**
  Datum der Vorgangsänderung.
- **Zeit:**
  Zeitstempel der Vorgangsänderung.
- **Modus:**
  Art der Vorgangsänderung.
- **ProdFlag:**
  Angabe, ob und wie die Daten an die Produktion übergeben worden sind:
  - **Prod:**
    Die Daten sind an die Produktion übergeben worden.
  - **Keine:**
    Die Daten sind noch nicht an die Produktion übergeben worden.
  - **Info:**
    Die Daten sind bereits in der Produktion verplant. Die nachträglichen Änderungen sind nicht produktionsrelevant und werden nur als Information an die Produktion übergeben, z. B. Preisänderungen.
  - **Info + P:**
    Die Änderungen werden je nach Positionsstatus verarbeitet:
    - Die Daten sind noch nicht in der Produktion verplant: Die nachträglichen Änderungen werden an die Produktion übergeben.
    - Die Daten sind bereits in der Produktion verplant: Die nachträglichen Änderungen werden nur als Information an die Produktion übergeben.
- **Frei:**
  Angabe, ob die Vorgangsänderung freigeschaltet ist:
  - J: Die Vorgangsänderung ist freigegeben.
  - N: Die Vorgangsänderung ist nicht freigegeben
- **V:**
  Angabe, ob die Änderungen an den Versand übergeben worden sind:
  - J: Die Änderungen sind an den Versand übermittelt worden.
  - N: Die Änderungen sind nicht übermittelt worden.

### Vorgangsänderungen

Die Änderungen werden mit folgenden Zeichen angezeigt:
- **Stern \***:
  Änderung durchgeführt.
- **Leeres Feld:**
  Keine Änderung durchgeführt.

Die Änderungen werden in folgenden Spalten angezeigt:
- **Termin:**
  Terminänderung im Vorgang.
- **Artikel:**
  Artikeländerung im Vorgang.
- **Preis:**
  Preisänderung im Vorgang.
- **Kond.:**
  Konditionenänderung im Vorgang.
- **Lief.:**
  Lieferantenänderung im Vorgang.

## Lieferterminänderungs-Protokoll

> Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > <Shift> + <F4> > Lieferterminänderungen

*Abb. D-70 Lieferterminänderungs-Protokoll*

In diesem Dialog werden alle Änderungen der Liefertermine angezeigt.

- **Termin alt:**
  Alter Liefertermin.
  Technische Info: Anzeigefeld, DB-Feld: kaufltedit.oldltplan
- **Termin neu:**
  Neuer Liefertermin.
  Technische Info: Anzeigefeld, DB-Feld: kaufltedit.newltplan
- **Begründung:**
  Begründung zur Lieferterminänderung.
  Technische Info: Anzeigefeld, DB-Feld: kaufltedit.text
- **Geändert von:**
  Name des Bearbeiters, der den Liefertermin bearbeitet hat.
  Technische Info: Anzeigefeld, DB-Feld: kaufltedit.moduser
- **am:**
  Datum der Lieferterminänderung.
  Technische Info: Anzeigefeld, DB-Feld: kaufltedit.moddatum
- **Uhrzeit:**
  Uhrzeit der Lieferterminänderung.
  Technische Info: Anzeigefeld, DB-Feld: kaufltedit.modzeit

## Modellkatalog

> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Menge > <Strg> + <F12> > <F2>

*Abb. D-71 Modellkatalog*

In diesem Dialog wählen Sie ein Modell aus dem Modellkatalog. Jedes Modell wird als Grafik mit entsprechender Nummer angezeigt.

Mit `<F2>` blättern Sie im Modellkatalog.

**Modell** Modellnummer aus dem Modellkatalog.
Technische Info: numerisches Feld, DB-Feld: kpos.modnr

> **Modellkatalog**
> Die angezeigten Modelle sind im A+W Modellkatalog enthalten, der standardmäßig für das System konfiguriert ist. Für die Konfiguration eines kundenindividuellen Modellkatalogs kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

Sie können das Modell auf mehrere Arten auswählen:

- Linksklick in das Kästchen neben der Grafik.
- Eingabe der Modellnummer in das Feld Modell.

Wenn Sie ein Modell gewählt haben, öffnet sich der Dialog Modell-Maßangaben, in dem Sie die Modellmaße definieren.
⇨ "Modell-Maßangaben" auf Seite D-177

## Modell-Maßangaben

> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Menge > <Strg> + <F12> > Modell wählen

*Abb. D-72 Modell-Maßangaben*

In diesem Dialog definieren Sie die Maße für die gewählte Modellscheibe. Für jede Seite geben Sie die Werte in Millimeter an. In der Mitte der Modellskizze wird die Modellnummer angezeigt.

Das System kann so konfiguriert werden, dass im Dialog rechts unten eine Vorschau der Modellscheibe angezeigt wird. Wenn Sie die Maße ändern, wird die Vorschau der Scheibe entsprechend aktualisiert.

Im Dialog rechts oben werden die Bedingungen der Eingabewerte für die Maßangaben-Felder angezeigt.

**Beispiel:**
> W > W1+W2
> Die Gesamtbreite im Feld W muss größer sein, als die Summe der Werte im Feld W1 und im Feld W2.

Mit `<Enter>` wechseln Sie im Dialog zum nächsten Eingabefeld.

Wenn Sie den Dialog aus der Stufenerfassung öffnen, definieren Sie die Maße des Referenzglases. Wenn dem Referenzglas kein Modell zugeordnet ist, wird eine rechteckige Scheibe mit der Modellnummer 0 angezeigt. Für diese Scheibe werden keine Bedingungen und keine Vorschau der Modellscheibe angezeigt. Sie können nur die Höhe und Breite der Scheibe angeben.

### Maßangaben am Modell

Die Maßangaben unterscheiden sich je nach gewähltem Modell. Daher ist keine genaue Beschreibung des Bezugs der Felder zur Datenbank möglich. Die Modellparameter werden unter den Datenbankfeldern kpodparam.param1 bis kpodparam.param10 gespeichert. Bei freien Modellformen wird der Wert in der Datenbank unter dem Eintrag kmpdparam.param99 gespeichert. Bei freien Modellformen wird zusätzlich die Modellbezeichnung im Datenbankfeld kmpdparam.param99 gespeichert.

**H, H(n)** Höhe der Scheibe. Je nach Modell existieren verschiedene Angaben für die Scheibenseiten. H steht für die Gesamthöhe und H(n) für eine Teilhöhe von H. Gibt es mehrere Höhenangaben, werden diese durchnummeriert.

**W, W(n)** Breite der Scheibe (aus dem Englischen: W = width = Breite). Je nach Modell existieren verschiedene Angaben für die Scheibenseiten. W steht für die Gesamtbreite und W(n) für eine Teilbreite von W. Gibt es mehrere Breitenangaben, werden diese durchnummeriert.

**R, R(n)** Radius der Scheibe. Der Radius wird nur bei Scheibenmodellen mit Kreisformen oder Bögen als Maßangabe herangezogen. Bei Modellen mit mehreren Kreisformen oder Bögen werden die verschiedenen Radien als R(n) angegeben. Gibt es mehrere Radiusangaben, werden diese durchnummeriert.

**D** Durchmesser der Scheibe. Der Durchmesser wird nur bei Modellscheiben in Kreisform als Maßangabe herangezogen.

**S** Segmenthöhe (Sagitta) der Scheibe. S steht für die Höhe des Segments, d. h. der Abstand zwischen Kreismitte und Kreissehne. Die Segmenthöhe wird nur bei Scheibenmodellen mit Kreissegmenten als Maßangabe herangezogen.

**(Textfeld ohne Bezeichnung)** Textfeld für zusätzliche Informationen.
Technische Info: alphanumerisches Feld

## Zahlungsverwaltung

> Verkauf > Auftragserfassung > Kopf-, Fußbereich > <F4> > Zahlungsverwaltung

*Abb. D-73 Zahlungsverwaltung*

In diesem Dialog werden die Anzahlungen zum Auftrag aus der FIBU angezeigt. Zudem können Sie manuell weitere Anzahlungen erfassen.

Der Dialog kann erst geöffnet werden, wenn mindestens eine Position zum aktuellen Auftrag erfasst ist. Sie können den Dialog Zahlungsverwaltung auch im Auftragsfuß mit `<Strg> + <F11>` öffnen.

Der Dialog wird nur angezeigt, wenn das System entsprechend konfiguriert ist und die Daten aus der FIBU per EDI eingelesen wurden. Die Daten aus der FIBU können nicht geändert werden.

Als Anzahlungen können Gutschriften und Storni erfasst werden. Wenn Sie den Dialog verlassen, wird je nach Konfiguration geprüft, ob die Summe der Anzahlungen den Auftragswert übersteigt. Ist dies der Fall, wird eine Meldung angezeigt, dass Sie die Anzahlungen überarbeiten müssen. Sie können den Dialog nur schließen, wenn der Restbetrag größer oder gleich Null ist.

### Register Anzahlungen

- **Nr.**
  Anzeige einer fortlaufenden Nummer der Anzahlung. Sie können den Inhalt im Feld nicht bearbeiten. Das System vergibt automatisch die nächste freie Nummer.
  Technische Info: Anzeigefeld, DB-Feld: anzahlung.zahlnr
- **Datum:**
  Datum der Anzahlung.
  Technische Info: Datumsfeld, DB-Feld: anzahlung.zahldat
- **Zahlungsweise:**
  Art und Weise der Bezahlung, z. B. Bankabbuchung oder Banklastschrift.
  Technische Info: Auswahl-Feld, DB-Feld: anzahlung.zahlweg
- **Zahlungsrichtung:**
  Angabe, in welche Richtung die Anzahlung fließt. Sie können die Anzahlung als Gutschrift oder als Storno erfassen. Wenn Sie Gutschrift wählen, wird der Anzahlungsbetrag vom Bruttobetrag abgezogen, wenn Sie Storno wählen, wird der Anzahlungsbetrag auf den Bruttobetrag aufgeschlagen.
  Technische Info: Toggle-Feld, DB-Feld: anzahlung.zahlrichtung
- **Betrag/Brutto:**
  Bruttobetrag der Anzahlung. Wenn Sie einen Betrag eingegeben haben, wird der Betrag in der Fußzeile unter - Anzahlung einberechnet.
  Technische Info: numerisches Feld, DB-Feld: anzahlung.betrag
- **Währung:**
  Währungseinheit der Anzahlung. Standardmäßig ist die Währung des Marktpartners eingestellt.
  Technische Info: Auswahl-Feld, DB-Feld: anzahlung.waehrung
- **Zahlungsverfahren:**
  Frei konfigurierbares Feld. Das Feld wird automatisch mit Daten über eine kundenindividuelle Schnittstelle gefüllt.
  Technische Info: alphanumerisches Feld, DB-Feld: anzahlung.zahlverfahren
- **Zahlungsreferenz:**
  Frei konfigurierbares Feld. Das Feld wird automatisch mit Daten über eine kundenindividuelle Schnittstelle gefüllt.
  Technische Info: alphanumerisches Feld, DB-Feld: anzahlung.zahlref_auftr

### Fußzeile

- **Brutto (Auftrag):**
  Bruttobetrag des Vorgangs.
- **- Anzahlung:**
  Summe der bisher geleisteten Anzahlungen, abzüglich der Gutschriften.
- **= Restbetrag:**
  Differenz aus dem Gesamtbetrag des Auftrags und der Summe aller Anzahlungen.

### Register Details

Die meisten Felder sind zum Register Anzahlungen beschrieben:
⇨ "Register Anzahlungen" auf Seite D-179

Zusätzlich werden folgende Felder angezeigt:

**Währung/Kurs** Währungseinheit und Währungskurs der Anzahlung. Standardmäßig ist die Währung des Marktpartners eingestellt. Der Währungskurs ist gesperrt.
Technische Info: numerische Felder, DB-Feld: anzahlung.waehrung, anzahlung.kurs

**Mitarbeiter** Anzeige des Namens des Mitarbeiters, der die Anzahlung erfasst hat.
Technische Info: Anzeigefeld, DB-Feld: anzahlung.aendmanr

**Bemerkung** Sie können eine Bemerkung zur Anzahlung eintragen, z. B. Absprachen, die mit dieser Anzahlung verbunden sind.
Technische Info: alphanumerisches Feld, DB-Feld: anzahlung.bemerkung

### Fußzeile

Die Felder in diesem Bereich sind zum Register Anzahlungen beschrieben:
⇨ "Register Anzahlungen" auf Seite D-179

## Zahlungsplan

> Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > <F4> > Zahlungsplan

*Abb. D-74 Zahlungsplan*

In diesem Dialog erstellen Sie einen Zahlungsplan für den Kunden, z. B. bei Ratenzahlung. Sie sollten den Zahlungsplan erst erstellen, wenn Sie die Auftragspositionen vollständig erfasst haben.

Mit `<Ende>` speichern Sie den Zahlungsplan.

In der Regel werden bei einem Zahlungsplan Abschlagsrechnungen und Schlussrechnung erfasst.

Wenn Sie die Abschlagsrechnungen manuell erfassen, wird ein Hinweis angezeigt, dass ein Zahlungsplan vorliegt und Sie die Daten übernehmen können.
⇨ "Abschlagsrechnung (manuell)" auf Seite D-350

Wenn Sie die Abschlagsrechnungen automatisch erstellen, wird für jede Abschlagszahlung im Zahlungsplan eine eigene Abschlagsrechnung angezeigt.
⇨ "Abschlagsrechnung (automatisch)" auf Seite D-348

Für den Restbetrag im Auftrag müssen Sie eine Schlussrechnung erstellen.
⇨ "Schlussrechnung (automatisch)" auf Seite D-351
⇨ "Schlussrechnung (manuell)" auf Seite D-352

> **Eingaben im Zahlungsplan**
> Wenn Sie für einen Auftrag einen Zahlungsplan erstellen, müssen Sie in dem Dialog Zahlungsplan nur das Datum, die Rechnungsart und die Höhe der jeweiligen Abschlagszahlung festlegen. Die Rechnungs- und Gutschriftennummern werden erst angezeigt, wenn zu den Abschlagszahlungen Rechnungen erstellt wurden.

- **Rechnung:**
  Rechnungs- und Gutschriftennummer der Abschlagsrechnung.
  Technische Info: Anzeigefeld, DB-Feld: kauf.auftrnr
- **Datum:**
  Datum, an dem der Rechnungsbetrag fällig wird.
  Technische Info: Datumsfeld, DB-Feld: zahlplan.Itplan
- **Artikel:**
  Nummer der Rechnungsart. Wenn Sie eine Nummer angeben, wird die Bezeichnung im Klartext angezeigt. In der Regel wählen Sie als Rechnungsart Abschlagsrechnung.
  Bevor Sie den Zahlungsplan nutzen können, müssen die folgenden beiden Artikel in den Artikelstammdaten hinterlegt sein:
  - Artikelnummer für Abschlagsrechnung (Artikeltyp = 995)
  - Artikelnummer für Schlussrechnung (Artikeltyp = 994)
  Technische Info: numerisches Feld, DB-Feld: zahlplan.artnr
- **Spalte ohne Bezeichnung:**
  Bezeichnung der Rechnungsart. Das Feld wird automatisch ausgefüllt, wenn Sie eine Nummer in der Spalte Artikel angeben.
  Technische Info: Anzeigefeld, DB-Feld: artikel.artbez1
- **Satz:**
  Prozentsatz des gesamten Rechnungsbetrags, der in der Abschlagsrechnung fakturiert wird. Wenn Sie einen Prozentsatz angeben, wird der entsprechende Betrag berechnet und im Feld Betrag eingetragen.
  Technische Info: numerisches Feld, DB-Feld: zahlplan.satz
- **Betrag:**
  Betrag der Abschlagsrechnung. Wenn Sie einen Prozentsatz in der Spalte Satz angegeben haben, wird der Betrag automatisch berechnet und Sie können den Inhalt im Feld nicht bearbeiten.
  Technische Info: numerisches Feld, DB-Feld: zahlplan.betrag

> **Gutschriften im Zahlungsplan**
> Wenn zu einer Abschlagsrechnung im Zahlungsplan eine Gutschrift erfasst wurde, wird diese im Zahlungsplan mit einem negativen Wert angezeigt.

## Fehlerinformationssystem

> Verkauf > Hintergrund-Kontrolle > Datum eingeben > <F3>

*Abb. D-75 Fehlerinformationssystem*

In diesem Dialog werden bestimmte Bearbeitungsfehler durch den Hintergrundprozess INTAUF ab dem ausgewählten Datum angezeigt. Die Aufträge, deren Bearbeitung fehlgeschlagen ist, werden in einer Tabelle aufgeführt.

- Mit `<F3>` starten Sie die Suche.
- Mit den Pfeiltasten und `<Bild runter>`, `<Bild hoch>` navigieren Sie in der Tabelle.

Die folgenden Fehler können angezeigt werden:

| Fehlernummer | Fehlertext | Bedeutung |
| :--- | :--- | :--- |
| 90 | INTAUF fehlerhafter Aufruf | Die Bearbeitung durch INTAUF ist fehlerhaft. Für mehr Informationen können Sie das INTAUF-Protokoll auswerten. |
| 91 | INTAUF Ladefehler | Das INTAUF konnte den Vorgang nicht laden. |
| 92 | INTAUF Schreibfehler | Das INTAUF konnte den Vorgang nicht speichern. |
| 93 | INTAUF x Versuche | Die Bearbeitung des Vorgangs wurde nach dem x-ten Fehlversuch abgebrochen. |
| 100 | INTAUF Preisdifferent | Der eigene VK-Preis und der EK-DFÜ-Preis sind unterschiedlich. |

*Tab. D-4 Fehleranzeige*

### Kopfbereich

**Anzeigen ab Datum** Startdatum, ab dem nach Fehlern gesucht wird.
Technische Info: Datumsfeld

### Trefferliste

In der Trefferliste werden folgende Felder angezeigt:

- **Auftrag:**
  Nummer des Auftrags, in dem der Fehler aufgetreten ist.
  Technische Info: Anzeigefeld, DB-Feld: kauferr.auftrnr
- **Zähl.:**
  Subnummer, z. B. bei Rechnungen oder Lieferscheinen.
  Technische Info: Anzeigefeld, DB-Feld: kauferr.subnr
- **Vorgang:**
  Art des Vorgangs.
  Technische Info: Anzeigefeld, DB-Feld: kauferr.vorgang
- **Err:**
  Nummer des aufgetretenen Fehlers.
  Technische Info: Anzeigefeld, DB-Feld: kauferr.errno
- **Fehlertext:**
  Informationstext zum aufgetretenen Fehler.
  Technische Info: Anzeigefeld, DB-Feld: kauferr.txt
- **Datum:**
  Datum, an dem der Fehler aufgetreten ist.
  Technische Info: Anzeigefeld, DB-Feld: kauferr.datum
- **Zeit:**
  Uhrzeit, zu der der Fehler aufgetreten ist.
  Technische Info: Anzeigefeld, DB-Feld: kauferr.zeit

Wenn Sie eine Zeile markieren, können Sie mit `<F3>` den entsprechenden Auftrag im Anzeigemodus öffnen.

## Produktionsmonitor

> Verkauf > Auftragserfassung > Kopf-, Fußbereich > <F4> > Produktionsmonitor

*Abb. D-76 Produktionsmonitor*

In diesem Dialog wird die Kapazitätsübersicht aus A+W Production über den Browser angezeigt.

Sie können den Produktionsmonitor alternativ mit `<F5>` im Feld Termin im Kopfbereich der Vorgangserfassung öffnen.

Der Dialog wird nur angezeigt, wenn Sie die Lizenz Capacity View besitzen und das System entsprechend konfiguriert ist.

Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

# Technische Werte

Eine Leistungserklärung spiegelt die technischen Merkmale und die Leistungsmerkmale eines Produktaufbaus wider.

in den Stammdaten können Sie unterschiedliche Leistungserklärungen (Dateien) für Produkte in verschiedenen Sprachen hinterlegen und diese den Produkten zuordnen. Eine Zuordnung kann nur von dem Mitarbeiter mit dem Recht KYLE='w' gemacht werden.

Diese Leistungserklärungen können Sie auch bei der Auftragserfassung zuordnen. Alternativ dazu können Sie die technischen Werte zu einer Auftragsposition anzeigen lassen und bearbeiten.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:

- "Leistungserklärung" auf Seite D-186
- "Auftragserfassung - Technische Werte" auf Seite D-187

## Leistungserklärung

> Verkauf > Auftragserfassung > Register Positionen > Register Eigensch. > Feld LE-Nummer > <Strg> + <K>

*Abb. D-77 Leistungserklärung*

In diesem Dialog ordnen Sie dem Produktaufbau einer Position eine Leistungserklärung zu. In den Stammdaten sind Leistungserklärungen für verschiedene Produktaufbauten hinterlegt. Sie können die Einträge nur bearbeiten, wenn das System entsprechend konfiguriert ist.
Damit Sie mit Leistungserklärungen arbeiten können, muss das entsprechende Modul aktiviert und konfiguriert sein und die Stammdaten müssen angepasst sein.

Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

Der Dialog ist ausführlich zum Part Stammdaten beschrieben:
⇨ Stammdaten, "Leistungserklärung" auf Seite J-254

## Auftragserfassung – Technische Werte

> Verkauf > Auftragserfassung > Positionsebene > Artikel wählen > <F4> > Produktangaben > Technische Werte > Leistungserklärung

In diesem Dialog erfassen und bearbeiten Sie Leistungserklärungen.

In diesem Dialog finden Sie folgende Register:

- "Auftragserfassung - Berechnete technische Werte" auf Seite D-187
- "Auftragserfassung – Deklarierte Leistungen" auf Seite D-190

### Auftragserfassung – Berechnete technische Werte

> Verkauf > Auftragserfassung > Positionsebene > Artikel wählen > <F4> > Produktangaben > Technische Werte > Leistungserklärung > Register Berechnete technische Werte

*Abb. D-78 Leistungserklärung – Berechnete technische Werte*

In diesem Register legen Sie die Daten für die Leistungserklärung fest. Zusätzlich werden die technischen Werte der gewählten Position angezeigt.
Wenn die technischen Werte mit einem externen Programm berechnet werden, z. B. mit A+W SLT, dann werden die Werte aus dem Programm übernommen und im Dialog angezeigt.

#### Kopfbereich

Die Felder im Kopfbereich sind zum Dialog Auftragserfassung – Kopf-, Fußbereich beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-83

**Position** Anzeige der Nummer der gewählten Position.
Technische Info: Anzeigefeld, DB-Feld: ktechw.posnr

**Artikel** Anzeige der Artikelnummer.
Technische Info: Anzeigefeld, DB-Feld: kpos.artnr

#### Berechnete technische Werte (AWE)

**Artikelcode** Artikelcode der gewählten Position. Der Artikelcode wird von einem externen Programmgeneriert, das die technischen Werte berechnet, z. B. von A+W SLT.
Technische Info: Anzeigefeld, DB-Feld: ktechw.artnrgen

**Direkte Luftschalldämmung** Schalldämmungs-Wert der Position in Dezibel.
Technische Info: Anzeigefeld, DB-Feld: ktechw.dbwert

**Ug-WertDIN** Wärmedurchgangskoeffizient nach DIN-Norm. Zentrale Maßeinheit, um den Wärmeverlust eines Bauteils zu ermitteln. Die Maßeinheit ist W/m²K. Je kleiner der Ug-Wert, desto größer ist die Wärmedämmung.
Technische Info: Anzeigefeld, DB-Feld: ktechw.kwert

**Ug-Wert** Wärmedurchgangskoeffizient.
Technische Info: Anzeigefeld, DB-Feld: ktechw.kbazwert

**Lichttransmissionsgrad** Lichtdurchlässigkeit für den direkt durchgelassenen Strahlungsanteil. Die Bezugsgröße von 100 % ist eine unverglaste Maueröffnung.
Technische Info: Anzeigefeld, DB-Feld: ktechw.trwert

**Gesamtenergiedurchlass** Energiedurchlasskoeffizient. Die Größe setzt sich zusammen aus direkter Sonnenenergietransmission und sekundärer Wärmeabgabe nach innen, infolge langwelliger Strahlung und Konvektion.
Technische Info: Anzeigefeld, DB-Feld: ktechw.gwert

**Ges-Stärke** Anzeige der Glasstärke in Millimeter für den gesamten Artikel der Position. Die Glasstärke ist abhängig von der gewählten Fassadenzone und der Windlast.
Technische Info: Anzeigefeld, DB-Feld: ktechw.dicke

**SZR1/SZR2** Anzeige der Größe der Abstandhalter im ersten und zweiten Scheibenzwischenraum in Millimeter. Die Anzahl der Abstandhalter ist abhängig von der Anzahl der Scheiben im ISO. Bei Artikeln mit mehr als zwei Abstandhaltern wird nur die Größe der ersten beiden Abstandhalter angezeigt.
Technische Info: Anzeigefelder, DB-Felder: xledesc.szr1, xledesc.szr2

**Windlast** Windlast am Einbauort. Windlast (N/m²) ist der Druck, der durch direkte Windeinwirkung auf die äußere Oberfläche eines Gebäudes ausgeübt wird. Das System führt mit diesem Wert eine Plausibilitätsprüfung durch, um zu prüfen, ob die Dickengruppe der gewählten Gläser für die angegebene Windlast ausreichend ist.
Technische Info: numerisches Feld, DB-Feld: ktechw.wlast

**Bereich** Anzeige der Fassadenzone, in der die Scheiben verbaut werden. Hohe Gebäude oder Gebäude, die an Randgebieten stehen, werden z. B. mit einer erhöhten Windlast belastet.
- **Rand:** Für Gebäude mit erhöhter Windlast.
- **zentral:** Für Gebäude ohne erhöhte Windlast.
Technische Info: Anzeigefeld, DB-Feld: ktechw.bereich

#### Kopfdaten der Leistungserklärung

**Leistungserklärung** Anzeige der alphanumerischen Nummer der Leistungserklärung. In diesem Feld wird der Inhalt aus dem Feld LE-Nummer im Register Eigensch. der Postionsebene angezeigt.
Technische Info: Anzeigefeld, DB-Feld: xlesprzu.lenr

**Bezeichnung** Bezeichnung (Titel) der zugeordneten Leistungserklärung.
Technische Info: alphanumerisches Feld, DB-Feld: xlesprzu.lebez

**Produkt** Bezeichnung des Produkts, dem die Leistungserklärung zugeordnet wird.
Technische Info: alphanumerisches Feld, DB-Feld: xledesc.prodbez

**Produkttyp** Bezeichnung des Produkttyps, dem die Leistungserklärung zugeordnet wird.
Technische Info: alphanumerisches Feld, DB-Feld: xledesc.prodtypbez

**Verwendungszweck** Nummer des Verwendungszwecks aus den Stammdaten. Wenn Sie eine Nummer eingeben, wird der Verwendungszweck als Klartext angezeigt.
Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: xledesc.zweck

**System zur Bewertung der Leistungsbeständigkeit** Anzeige der Konformitätsbewertung des Artikels. Je nach Konfiguration ist das Feld mit einem Wert von SommerGlobal vorbelegt.
Technische Info: Anzeigefeld

**Harmonisierte Produktnorm** Alphanumerischer Schlüssel der Produktnorm aus den Stammdaten.
Technische Info: alphanumerisches Feld, DB-Feld: xledesc.pnorm

**Notifizierte Stelle** Anzeige der Prüfstelle für die Konformitätsbewertung. Je nach Konfiguration ist das Feld mit einem Wert von SommerGlobal vorbelegt.
Technische Info: Anzeigefeld

#### Fußbereich

**Zurücksetzen** Verwirft die Leistungserklärung und alle zugehörigen technischen Werte. Das Feld ist nur freigeschaltet, wenn die Anbindung an SommerGlobal entsprechend im System konfiguriert ist.

### Auftragserfassung – Deklarierte Leistungen

> Verkauf > Auftragserfassung > Positionsebene > Artikel wählen > <F4> > Produktangaben > Technische Werte > Leistungserklärung > Register Deklarierte Leistungen

*Abb. D-79 Leistungserklärung – Deklarierte Leistungen*

In diesem Register legen Sie fest, welche Produktmerkmale des ausgewählten Artikels in der Leistungserklärung ausgegeben werden sollen. Die Werte für die Produktmerkmale können Sie bearbeiten.

Wenn die SLT-Schnittstelle für externe Berechnung konfiguriert ist, können alle Felder, die mit einem Stern \* markiert sind, über die A+W SLT-Schnittstelle und das externe Berechnungsprogramm berechnet werden. Die Felder werden mit den entsprechenden Werten vorbelegt.

Welche der Produktmerkmale in der Leistungserklärung ausgegeben werden sollen, können Sie über die Aktivierung der jeweiligen Checkbox festlegen. Wenn Sie eine Leistungserklärung erzeugen wollen, muss mindestens eine Checkbox aktiv sein.

> **Anzeige von NPD im Feld**
> Wenn ein Wert über die SLT-Schnittstelle nicht ermittelt werden kann, dann wird NPD (No Performance Determined) in dem Feld angezeigt.

#### Kopfbereich

Die Felder im Kopfbereich sind zum Dialog Auftragserfassung – Kopf-, Fußbereich beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-83

**Position** Anzeige der Positionsnummer des gewählten Artikels.
Technische Info: Anzeigefeld, DB-Feld: ktechw.posnr

**Artikel** Anzeige der Artikelnummer.
Technische Info: Anzeigefeld, DB-Feld: ktechw.artnr

**Leistungserklärung** Anzeige der alphanumerischen Angabe der Leistungserklärung.
Technische Info: Anzeigefeld, DB-Feld: xlesprzu.lenr

#### Deklarierte Leistungen

**(Checkboxen)** Angabe, ob der entsprechende technische Wert vor der Checkbox in der Leistungserklärung ausgegeben wird.
- ☑ Der technische Wert wird im Dokument ausgegeben.
- ☐ Der technische Wert wird nicht im Dokument ausgegeben.
Technische Info: Checkbox

#### Sicherheit im Brandfall

**Feuerwiderstand** Feuerwiderstandsklasse der Artikels, die angibt, wie lange ein Bauteil einem Feuer standhält.
Technische Info: alphanumerisches Feld, DB-Feld: ktechw.feuerw

**Brandverhalten** Baustoffklasse des Artikels, die angibt, ob und/oder wie schnell ein Baustoff entflammbar ist.
Technische Info: alphanumerisches Feld, DB-Feld: ktechw.brandvh

**Brandbeanspruchung** Art der Brandbeanspruchung, die angibt, ob ein Bauteil ein- oder mehrseitig vom Feuer beansprucht wird. Raumabschließende Bauteile werden z. B. nur einseitig beansprucht:
- 1: einseitige Brandbeanspruchung
- 2: zweiseitige Brandbeanspruchung
- 3: dreiseitige Brandbeanspruchung
- 4: vierseitige Brandbeanspruchung
Technische Info: alphanumerisches Feld, DB-Feld: ktechw.brandbea

#### Nutzungssicherheit

**Durchschusshemmung** Widerstandsklasse des Glases bei Durchschuss. Die Widerstandsklassen berücksichtigen Art und Kaliber der Waffe. Zusätzlich wird angegeben, ob das Glas bei Durchschuss splitterfrei bleibt oder ob Material- oder Glassplitter abplatzen. Entsprechend erhält die Widerstandsklasse der Zusatz NS für splitterfrei oder S für Splitterabgang.
Technische Info: alphanumerisches Feld, DB-Feld: ktechw.dschussh

**Sprengwirkungshemmung** Widerstandsklasse des Glases bei Sprengwirkung. Die Gläser werden einer von vier Widerstandsklassen zugeordnet, die den Widerstand eines Glases auf den Druck einer Stoßwelle festlegen.
Technische Info: alphanumerisches Feld, DB-Feld: ktechw.sprwirkh

**Einbruchhemmung** Widerstandsklasse des Bauteils bei Einbruch. Die Widerstandsklassen berücksichtigen den Tätertypen und sein mutmaßliches Vorgehen, die Widerstandszeit und die Einsatzmöglichkeit des Bauteils. Die Verglasung wird in einer separaten Widerstandsklasse definiert.
Technische Info: alphanumerisches Feld, DB-Feld: ktechw.ebruchh

**Widerstand gegen Pendelschlag** Widerstandsklasse des Glases bei Pendelschlag. Der Pendelschlag simuliert den Aufprall eines menschlichen Körpers auf das Glas. Die Widerstandsklassen berücksichtigen das Bruchbild und die Splitterung des Glases nach der Prüfung.
Technische Info: alphanumerisches Feld, DB-Feld: ktechw.pschagw

**Temperaturbeständigkeit K** Temperaturwechselbeständigkeit von Glas bei Temperaturwechseln in Kelvin.
Technische Info: numerisches Feld, DB-Feld: ktechw.tempbest1

**Lastwiderstand mm** Glasstärke in Millimeter. Das Feld ist mit der Stärke vom Glas vorbelegt.
Technische Info: numerisches Feld, DB-Feld: ktechw.lastwidst1

**2/3 Glas / SZR** Lastwiderstand des zweiten und dritten Glases und Scheibenzwischenraum.
In den ersten beiden Feldern wird die Glasstärke des zweiten und dritten Glases für den Lastwiderstand in Millimeter angegeben.
Im dritten und vierten Feld wird der Scheibenzwischenraum angegeben.
Die Felder werden vom System vorbelegt und können nicht bearbeitet werden.
Technische Info: Anzeigefelder, DB-Felder: ktechw.lastwidst2, ktechw.lastwidst3, arttechw.szr1, arttechw.szr2

#### Energieerhaltung (EN 13363-2)

> **Felder mit \***
> Die Werte in den Feldern mit einem \* werden automatisch aus der Stückliste berechnet und in den Dialog übernommen.

**Wärmestrahlungsfaktor** Faktor der Wärmestrahlung in Prozent.

**Konvektionsfaktor** Faktor der Wärmeübertragung in Prozent.

**Belüftungsfaktor** Faktor der Belüftung in Prozent.

**Gesamtenergiedurchlass** Energiedurchlasskoeffizient (Gesamtdurchlassgrad). Die Größe setzt sich zusammen aus direkter Sonnenenergietransmission und sekundärer Wärmeabgabe nach innen infolge langwelliger Strahlung und Konvektion.

**Wärmeabgabe nach innen (sekundär)** Die sekundäre Wärmeabgabe bezeichnet den Vorgang, dass der absorbierte Strahlungsanteil durch die Verglasung in Form von Strahlung wieder abgegeben wird. Sie wird in sekundäre Wärmeabgabe nach außen und sekundäre Wärmeabgabe nach innen unterschieden.

#### Schallschutz

**Direkte Luftschalldämmung (... ; ...)** Schalldämmaß Rw (C ; Ctr) der Position in Dezibel, z. B. 40 (-3; -5) dB.

#### Energieerhaltung und Wärmeschutz

**Thermische Eigenschaften W/(m²K)** Wärmedurchgangskoeffizient nach DIN-Norm. Zentrale Maßeinheit, um den Wärmeverlust eines Bauteils zu ermitteln. Die Maßeinheit ist W/m²K. Je kleiner der Ug-Wert, desto größer ist die Wärmedämmung.

**Lichttransmissionsgrad** Lichtdurchlässigkeit.

**Strahlungstransmissionsgrad (direkt)** Strahlung, die durch die Verglasung durchgelassen wird.

**Sonnenenergietransmissionsgrad** Sonnenstrahlung, die durch die Verglasung durchgelassen wird.

**Lichtreflexionsgrad Glasseite** Sonnenstrahlung, die von der Glasseite nach außen reflektiert wird.

**(Lichtreflexionsgrad) Schichtseite** Sonnenstrahlung, die von der Schichtseite eines Glases nach außen reflektiert wird. Wenn ein Glas beschichtet ist, ist die Reflexion der beschichteten Seite in der Regel höher als die unbeschichtete Glasseite.

**Strahlungsreflexionsgrad** Strahlung, die von der Verglasung direkt nach außen reflektiert wird.

**Strahlungsabsorptionsgrad (Layer)** Strahlung, die durch die Verglasung aufgenommen wird.

#### Farbwiedergabe

**Farbwiedergabeindex** Index für die Veränderung des Lichtes durch die Verglasung. Je höher der Farbwiedergabeindex ist, desto weniger werden die Farben geändert.

#### Energieerhaltung (EN410)

**Gesamtenergiedurchlass** Energiedurchlasskoeffizient (Gesamtdurchlassgrad). Die Größe setzt sich zusammen aus direkter Sonnenenergietransmission und sekundärer Wärmeabgabe nach innen, infolge langwelliger Strahlung und Konvektion.

**Wärmeabgabe nach innen (sekundär)** Die sekundäre Wärmeabgabe bezeichnet den Vorgang, dass der absorbierte Strahlungsanteil durch die Verglasung in Form von Strahlung wieder abgegeben wird. Sie wird in sekundäre Wärmeabgabe nach außen und sekundäre Wärmeabgabe nach innen unterschieden.

**Shading Coeffizient** Beschattungskoeffizient, auch b-Faktor. Der Beschattungskoeffizient dient der Berechnung von Kühllasten.

# Stückliste

In der Stückliste ist der Aufbau der Scheibenartikel festgelegt. Sie können zu den einzelnen Scheiben Bearbeitungen, Stufen, Modelle, einen Einstand und Sprossen erfassen und anpassen.

In diesem Abschnitt sind folgende Dialoge erklärt:

- "Stücklistendarstellung" auf Seite D-195
- "Kantenzuordnung" auf Seite D-217
- "Bearbeitungen zu Position" auf Seite D-218
- "Maße der einzelnen Stücklistenteile" auf Seite D-219
- "Einstand" auf Seite D-221
- "Versiegelungstiefen" auf Seite D-222
- "Stufenerfassung (relevante Teile)" auf Seite D-223
- "Stufen Abzugsmaße" auf Seite D-225
- "Sprossenerfassung" auf Seite D-226
- "Sprossenstückliste – Sprossenartikel" auf Seite D-230
- "Sprosseneditor" auf Seite D-231
- "Bohrpunkt" auf Seite D-232
- "Lichtes Feld" auf Seite D-233
- "Sprossenabschnitte" auf Seite D-233
- "Sprossenaufteilung" auf Seite D-234

## Stücklistendarstellung

> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld B.Art > <F3>

In diesem Dialog wird die Positionsstückliste angezeigt. Auf den aktuellen Stücklistenebenen können Sie zu den einzelnen Artikeln in der Stückliste Bearbeitungen erfassen und anpassen.

In diesem Dialog finden Sie folgende Register:

- "Stücklistendarstellung - Stücklistenaufbau" auf Seite D-196
- "Stücklistendarstellung – Produktaufbau" auf Seite D-199
- "Stücklistendarstellung - Produktionsskizze" auf Seite D-200
- "Stücklistendarstellung – Akt. Stücklistenebene" auf Seite D-202
- "Stücklistendarstellung – Bearbeitungsparameter (kurz)" auf Seite D-207
- "Stücklistendarstellung – Alle Parameter/Skizze" auf Seite D-209

### Stücklistendarstellung – Stücklistenaufbau

> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld B.Art > <F3>

*Abb. D-80 Stücklistendarstellung*

In diesem Dialog wird die Stückliste der gewählten Position angezeigt. Die Stückliste ist eine detaillierte Auflistung einer Position der Auftragserfassung und wird in einem Stücklistenbaum angezeigt.

- Mit `<F3>` klappen Sie die einzelnen Knoten der Stückliste auf und zu.
- Mit `<Strg> + <F8>` klappen Sie alle Knoten der Stückliste auf.
- Mit `<F5>` wechseln Sie in das Register Akt. Stücklistenebene im unteren Bereich des Dialogs, in dem Sie die Stückliste bearbeiten können.
  ⇨ "Stücklistendarstellung - Akt. Stücklistenebene" auf Seite D-202

In der ersten Zeile des Stücklistenbaums wird die ausgewählte Position angezeigt. In den darunterliegenden Zeilen werden Informationen zu den Baugruppen, Einzelkomponenten oder Bearbeitungen, die zur Fertigung der Position benötigt werden, angezeigt.

Eine Baugruppe entspricht einem Knoten. Über das vorangestellte Plus- oder Minuszeichen können Sie die Baugruppe auf- und zuklappen.
Zur besseren Übersicht sind den Komponenten und Bearbeitungen festgelegte Bildzeichen zugeordnet:

| Symbol | Symbolbeschreibung | Bedeutung |
| :--- | :--- | :--- |
| 