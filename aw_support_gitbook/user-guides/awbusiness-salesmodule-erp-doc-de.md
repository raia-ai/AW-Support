---
title: "D-AWBusiness-HB_19"
source: "D-AWBusiness-HB_19.pdf"
tags: ["A+W Business", "Software Reference", "Sales Module", "ERP", "Order Management", "Item Positions", "Pricing", "Macros", "Bill of Materials", "Technical Documentation"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical software reference guide for the \"A+W Business Verkauf\" (Sales) module, specifically focusing on overviews and references related to item positions within an order. It covers functionalities for product selection, handling inquiries, managing prices, and processing orders."
long_description: "This document is a comprehensive section from the A+W Business software reference manual, detailing features under \"Übersichten und Referenzen zu Positionen\" (Overviews and References for Items). It provides step-by-step guidance and explanations for various dialogs and functions within the sales and order processing workflow. Key topics include selecting products using different criteria like technical parameters and classifiers, handling quick inquiries (\"Schnellanfrage\"), replacing parameters in product descriptions, and performing product comparisons with CAD data (\"Produktabgleich\"). The guide also covers managing reclamations, setting cutback dimensions (\"Rückschnitt\"), selecting color variants, and applying fixed prices. Advanced features such as creating and managing macros, copying item positions, and detailed cost/surcharge calculations are explained. Furthermore, it details the processes for handling partial deliveries (\"Teillieferungen\"), managing production-related bills of materials, and interfacing with financial accounting (FiBu) through data export. The document is intended for users and administrators of the A+W Business software to understand and effectively utilize the extensive features related to managing order items from creation to final delivery and invoicing."
---

# Übersichten und Referenzen zu Positionen

---
### Dickentoleranz in mm
Die Dicke kann bei Isolierglas um wenige Millimeter differieren. Dieses Feld nutzen Sie, wenn die Dicke des gesuchten Produktes ausschlaggebend ist.

### Größentoleranz mm (<200 cm), (>=200 cm)
Angabe, um wie viel Millimeter die ISO-Scheibe von ihrer vorgegebenen Größe abweichen kann.

### Technische Parameter anzeigen
In der Produktliste werden standardmäßig neben der Produktnummer, dem Matchcode und den Bezeichnungen 1 und 2 nur die Standardhöhe und -breite angezeigt.

- Die technischen Parameter werden in der Produktliste nicht angezeigt.
- [x] Zusätzlich zu den Standardinformationen werden die technischen Parameter in der Produktliste angezeigt.

## Auswahl – Nach Klassifikatoren
> Dokumente > Auftrag > Auftrag auswählen > Positionen > [...] > Register Nach Klassifikatoren

*Abb. C-304 Auswahl - Nach Klassifikatoren*

In diesem Register schränken Sie die Suche über die Klassifikatoren ein, die zu einem Hauptprodukt hinterlegt sind.

- ⇨ Stammdaten, “Produktverwaltung - Anlagen/Klassifikatoren" auf Seite B-634

## Schnellanfrage
> Dokumente > Auftrag > Schnellanfrage
>
> Dokumente > Auftrag > Auftrag auswählen > Register Position > Menü Funktionen > Gruppe Position > Schnellanfrage

*Abb. C-305 Schnellanfrage für Kunden starten*

In diesem Dialog können Sie einen Kunden auswählen, um eine (telefonische) Anfrage schnell zu beantworten. Zum ausgewählten Kunden wird der aktuelle Stand des Kreditlimits angezeigt.

Wenn Sie während der Anfrage einen Auftrag mit Positionen erfasst haben, können Sie diesen speichern oder verwerfen.

- ⇨ Tutorial, “Schnellanfrage beantworten" auf Seite C-103

Wenn Sie die Schnellanfrage starten, wird zunächst ein Dialog zur Auswahl des anfragenden Kunden angezeigt. Nach der Wahl des Kunden werden die aktuellen Daten zum Kreditlimit und den offenen Posten angezeigt.

Anschließend wird die Positionserfassung mit leeren Feldern angezeigt. Der zugehörige Dokumentenkopf ist bereits mit den entsprechenden Kundendaten gefüllt.

- ⇨ "Dokument - Positionen" auf Seite C-461

Nachdem Sie die angefragten Positionen erfasst haben, können Sie die Anfrage beenden oder speichern. Zum Speichern können Sie festlegen, ob die Anfrage als Angebot oder als Auftrag gespeichert werden soll.

### Schnellanfrage speichern

*Abb. C-306 Schnellanfrage speichern*

#### Speicherort
- **Angebot:** Die Schnellanfrage wird als Angebot gespeichert.
- **Auftrag:** Die Schnellanfrage wird als Auftrag gespeichert.

#### Mandant
Die Wahl des Mandanten steuert die Anzeige im Feld Bereich.

#### Bereich
Sie können den zuständigen AV-Bereich auswählen.

#### Nummernverwalter
Das Dokument wird im entsprechenden Nummernverwalter gespeichert. Wenn Sie die Schnellanfrage als Auftrag speichern, wird automatisch der Nummernverwalter angezeigt, zu dem der zuletzt bearbeitete Auftrag gehört.

Nachdem Sie die Schnellanfrage beendet (schließen oder speichern) haben, wird automatisch das Dokument wieder angezeigt, in dem Sie zuletzt gearbeitet haben.

## Parameter-Ersetzung
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Modelle/ Bearbeitungen > [Formel]

*Abb. C-307 Parameter-Ersetzung*

In diesem Dialog werden die erlaubten Variablen angezeigt, die Sie zur Modifizierung der Beschreibung verwenden können.

### Textersetzung
Sie können den Beschreibungstext bearbeiten. Er wird im Dialog Bearbeitungen im Feld Beschreibung angezeigt.

### Parameter mit identischer Bedeutung
In diesem Bereich werden die Parameter angezeigt, die synonym verwendet werden können.

## Produktabgleich
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Modelle/ Bearbeitungen > Menü Start > iTOE

*Abb. C-308 Produktabgleich*

In diesem Dialog prüfen Sie die Regeln zu einer importierten DXF- oder SN-Datei für Bearbeitungen. Änderungen der Bearbeitung in der Auftragsposition werden gegen die hinterlegten Regeln geprüft.

- ⇨ Stammdaten, "¡TOE Regeln" auf Seite B-668

Wenn Sie ein Modell erfasst und im A+W CAD Designer bearbeitet haben, können Sie die Änderungen als SN-Datei (TOE-Datei) speichern. Damit wird eine SN-Datei in der Stückliste angelegt, ein Modellsatz eingefügt und mit der TOE-Datei verknüpft.

Die TOE-Dateien werden in der Form XXXX_TOE.SN gespeichert, wobei die vorangestellte Nummer aus dem Nummernkreisen der SN-Dateien bestimmt wird.

> **Eigenschaft von CAD-Bearbeitung**
> Änderungen von Eigenschaften, die nicht Bestandteil des A+W-Bearbeitungstypenkatalog sind, gehen beim Abgleich verloren, z. B. eine Bohrloch-Reihe mit Serienvermaßung: Die Serienvermaßung wird gelöscht, sobald eine der beteiligten Bohrungen in der Bearbeitungserfassung geändert wird. Solche Änderungen müssen im A+W CAD Designer durchgeführt werden.

### Übersicht
In der Übersicht werden die hinterlegten Regeln angezeigt. Bearbeitungen ohne Regel werden farbig hinterlegt.

Nach der Bestätigung des Produktabgleichs wird die Stückliste im Register Modelle/Bearbeitungen neu aufgebaut und die Preise werden neu berechnet. Jede weitere Änderung wird mit der verknüpften TOE-Datei abgeglichen.

- **CAD Bearbeitung:** Bezeichnung der Bearbeitung in A+W CAD Designer.
- **Produkt, Bezeichnung:** Nummer und Bezeichnung der Regel in A+W Business.
- **Regel bearbeiten/einfügen:** Wechsel zum Dialog iTOE Regeln, um eine Regel anzulegen oder zu bearbeiten.
  - ⇨ Stammdaten, "ITOE Regeln" auf Seite B-668
- **Gefundene Regel:** Bezeichnung der hinterlegte Regel zur Bearbeitung.
- **Eigenschaft:** Inhalt der hinterlegten Regel.

## Reklamationen
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Zusatz > [Ordner] neben dem Feld Grund

*Abb. C-309 Reklamation*

> In diesem Dialog können Sie pro Position einen Reklamationsverursacher und einen Reklamationsgrund auswählen, wenn Sie ein Dokument des Typs Reklamation erfassen.
>
> ⇨Tutorial, "Reklamationen" auf Seite C-289
>
> **Reklamation in anderen Dokumententypen**
> Wenn Sie den Dialog nicht im Dokumententyp Reklamation verwenden, werden die Angaben nicht in die Reklamationsstatistik übergeben.

### Verursacher
Der Verursacher kann in der Reklamationsstatistik zur Auswertung herangezogen werden. Die Eingabe ist optional.

### Grund
Der Grund kann in der Reklamationsstatistik zur Auswertung herangezogen werden. Die Eingabe ist optional.

### VK
Der Verkaufspreis für die beanstandete Position wird angezeigt. Dies ist der entgangene Umsatz.

### Kostenlos
Die Reklamationspositionen und auch -aufträge können statistisch ausgewertet werden, z. B. der Verkaufswert.
- Die Reklamation wird berechnet.
- Die Reklamation wird nicht berechnet, z. B. in Kulanzfällen oder bei eigenem Verschulden. Der VK-Wert zeigt den entgangenen Umsatz an.

## Rückschnitt
> Dokumente > Auftrag > Auftrag auswählen > Register Sprossen > [Rückschnitt]

*Abb. C-310 Rückschnitt*

In diesem Dialog legen Sie die Maße für den Rückschnitt pro Kante fest. Der Rückschnitt beschreibt den einfachen Abstand zwischen Fensteraußenkante und Rahmeninnenkante.

## Variantenauswahl (Farbsuche)
> Dokumente > Auftrag > Auftrag auswählen > Register Sprossen > Varianten suchen [Lupe]

*Abb. C-311 Variantenauswahl*

In diesem Dialog wählen Sie die Farb-Varianten zu einem erfassten Produkt aus.

### Suchkriterien
**Bezeichnung** Bezeichnung der Farbe, nach der gesucht werden soll.

**Fremdschlüssel** Fremdschlüssel der Farbe, nach der gesucht werden soll.

### Übersicht
- **Variante, Bezeichnung:** Interne Nummer und Bezeichnung der Farbe.
- **Fremdschlüssel:** Bei Dorma-Artikeln der Dorma-Farbschlüssel. Der Fremdschlüssel kann für die Kommunikation mit anderen Programmen verwendet werden, z. B. für die Übergabe an die Produktion.
- **Vorschau:** Anzeige der Farbvariante.
- **Sonderfarbe:** Sonderfarbe, z. B. beim Siebdruck.

## Festpreis Vorgabe
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Übersicht Positionen > Kontextmenü > Festpreis vorgeben

*Abb. C-312 Festpreis Vorgabe*

In diesem Dialog können Sie für markierte Position(en) einen Festpreis eintragen.

### Selektierte Positionen
Alle markierten Positionen werden aufgelistet. Der Festpreis gilt für diese Positionen insgesamt.

### Vorgabe
**Festpreis** Wenn Sie einen Festpreis für die markierten Positionen eingegeben haben, wird der Gesamtpreis für die einzelnen Positionen im Bereich Selektierte Positionen aktualisiert.

Die Werte werden in die Positionserfassung übernommen.

## Globale Änderungen
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Übersicht Positionen > Kontextmenü > Globale Änderungen

*Abb. C-313 Globale Änderungen*

In diesem Dialog ändern Sie die Kommissionsangabe übergreifend für die markierten Positionen.

### Selektierte Positionen
In der Übersicht werden alle markierten Positionen aufgeführt, für die die Kommission geändert werden soll.

### Änderung
**Kommission** Die Änderung gilt für alle Positionen, die in der Übersicht aufgeführt werden.
- Die Kundenkommission wird nicht geändert. Das Eingabefeld ist gesperrt.
- Die Kundenkommission kann geändert werden. Das Eingabefeld ist freigeschaltet.

## Produktionsstücklistenauflösung
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Stückliste > Stücklistenaufbau Kontextmenü (am Glas) > Produktionsstücklistenauflösung

*Abb. C-314 Produktionsstücklistenauflösung*

In diesem Dialog bearbeiten Sie die Produktionsstücklistenauflösung. Sie wird für Bearbeitungen immer am Glas definiert.

Bei Bearbeitungen kann die Produktionsstücklistenauflösung ausgeschaltet werden. Damit können Sie im aktuellen Auftrag eine Bearbeitung an den Einzelscheiben oder der gesamten Einheit festlegen.

- ⇨ Stammdaten, "Produktionsstücklistenauflösung festlegen" auf Seite B-192

## Konditionen
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Ansicht > Gruppe Konditionen > Konditionen

*Abb. C-315 Konditionen*

In diesem Dialog werden die Rabatte und individuellen Preise für den aktuellen Kunden angezeigt.

- ⇨ Stammdaten, "Rabatt anlegen" auf Seite B-361

### Rabatte
Anzeige der Rabatte, die für den aktuellen Kunden gelten. Diese können sich sowohl auf den einzelnen Kunden als auch auf die Kundengruppe beziehen, zu der der aktuelle Kunde gehört.

### Individuelle Preise
Anzeige der Preise, die speziell für den aktuellen Kunden oder seine Kundengruppe hinterlegt sind. Wenn keine kundenindividuellen Preise angelegt sind, bleibt das Feld leer.

## Preis-/Konditionsinformationen
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Ansicht > Gruppe Konditionen > Preis-/Konditionsinformation

In diesem Dialog können Sie sich über die Preise und Konditionen informieren, die für den aktuellen Kunden gelten.

> **Voraussetzung**
> Der Dialog steht nur zur Verfügung, wenn Sie in den Firmendaten die Preisberechnung nach Makro-Preisen aktiviert haben.

In diesem Dialog finden Sie folgende Register:
- "Preis-/Konditionsinformationen – Preisabfrage" auf Seite C-612
- "Preis-/Konditionsinformationen – Makropreise" auf Seite C-613
- "Preis-/Konditionsinformationen - Rabatte" auf Seite C-614
- "Preis-/Konditionsinformationen – Autom. Zuschläge" auf Seite C-615
- "Preis-/Konditionsinformationen – Kunde" auf Seite C-616

### Preis-/Konditionsinformationen – Preisabfrage
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Ansicht > Gruppe Konditionen > Preis-/Konditionsinformation > Register Preisabfrage

*Abb. C-316 Preis-/Konditionsinformationen – Preisabfrage*

In diesem Register können Sie sich über Details zu den Preisen informieren. Die Anzeige kann nach verschiedenen Kriterien gefiltert werden.

#### Auswahl
Mit der Wahl der Option legen Sie fest, ob die Preise für ein Produkt, eine Produktart oder eine Produktgruppe angezeigt werden sollen.

#### Jahrgang, Schlüssel
Sie können die Preise nach Tarifen filtern.

#### Druckoptionen
Sie können die Daten drucken. Dazu legen Sie fest, ob die Angaben aus allen oder nur aus bestimmten Registern ausgegeben werden sollen.
- Die Daten aus dem entsprechenden Register werden nicht mit gedruckt, z. B. aus dem Register Rabatte.
- [x] Die Daten aus dem entsprechenden Register werden mit gedruckt.

### Preis-/Konditionsinformationen – Makropreise
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Ansicht > Gruppe Konditionen > Preis-/Konditionsinformation > Register Makropreise

*Abb. C-317 Preis-/Konditionsinformationen – Makropreise*

In diesem Register werden die Makropreise und der zugehörige Produktaufbau aufgelistet.

Die Felder zu den Druckoptionen sind zu Register Preisabfrage erklärt.

- ⇨ "Preis-/Konditionsinformationen – Preisabfrage" auf Seite C-612

### Preis-/Konditionsinformationen – Rabatte
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Ansicht > Gruppe Konditionen > Preis-/Konditionsinformation > Register Rabatte

*Abb. C-318 Preis-/Konditionsinformationen - Rabatte*

In diesem Register werden die Rabatte angezeigt, die für den aktuellen Kunden gültig sind.

Die Felder zu den Druckoptionen sind zu Register Preisabfrage erklärt.

- ⇨ "Preis-/Konditionsinformationen - Preisabfrage" auf Seite C-612

### Preis-/Konditionsinformationen – Autom. Zuschläge
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Ansicht > Gruppe Konditionen > Preis-/Konditionsinformation > Register Autom. Zuschläge

*Abb. C-319 Preis-/Konditionsinformationen – Automatische Zuschläge*

In diesem Register werden die automatischen Zuschläge aufgelistet, die für den aktuellen Kunden berechnet werden.

Die Felder zu den Druckoptionen sind zu Register Preisabfrage erklärt.

- ⇨ "Preis-/Konditionsinformationen - Preisabfrage" auf Seite C-612

### Preis-/Konditionsinformationen – Kunde
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Ansicht > Gruppe Konditionen > Preis-/Konditionsinformation > Register Kunde

*Abb. C-320 Preis-/Konditionsinformationen - Kunde*

In diesem Register werden das aktuelle Kreditlimit und die Kundenanschrift aus den Kundenstammdaten angezeigt.

Die Felder zu den Druckoptionen sind zu Register Preisabfrage erklärt.

- ⇨ "Preis-/Konditionsinformationen - Preisabfrage" auf Seite C-612

## Artikel-Informationen
> Dokumente > Artikel-Info
>
> Dokumente > Angebot, Auftrag, Gutschrift > Angebot, Auftrag, Gutschrift > Positionen > Menü Ansicht > Artikelinfo

In diesem Dialog können Sie sich über Details zu einem Produkt informieren, ohne in die Stammdaten wechseln zu müssen.

In diesem Dialog finden Sie folgende Register:
- "Artikel-Info - Info" auf Seite C-617
- "Artikel-Info – Preise/Lager" auf Seite C-618
- "Artikel-Info - Anlagen" auf Seite C-620

### Artikel-Info – Info
> Dokumente > Artikel-Info > Register Info

*Abb. C-321 Artikel-Info – Info*

In diesem Register werden die Daten aus der Produktdefinition angezeigt.

#### Auswahl
Die Daten in diesem Bereich werden aus der Produktdefinition übernommen.

- ⇨ Stammdaten, "Produktverwaltung - Produkt" auf Seite B-600

**Artikel/Farbe** Die Nummer des Produktes wird automatisch angezeigt, wenn der Dialog aus der Positionserfassung geöffnet wurde. Im Feld Farbe stehen die hinterlegten Varianten zur Auswahl.

**Bezeichnung 1, 2, 3** Bezeichnungen aus den Stammdaten des Produkts.

**Produktart** Die Produktart wird automatisch angezeigt, wenn der Dialog aus der Positionserfassung geöffnet wurde.
Wenn die Produktart zur Suche eingesetzt wird, setzt die Anzeige von Daten beim ersten Produkt mit der gewählten Produktart ein.

**Produktgruppe** Die Produktgruppe wird automatisch angezeigt, wenn der Dialog aus der Positionserfassung geöffnet wurde.

**Referenznummer** Referenznummer bei kundeneigenen Produkten.

**Stückliste** Die gesamte Stückliste wird aus den Stammdaten übernommen.

**Artikel Info** Die Artikelinfo wird aus den Stammdaten übernommen.

**Ansicht** Wenn in den Produktstammdaten eine Ansicht (Bitmap) des Produkts verknüpft ist, wird das Produktbild angezeigt.

### Artikel-Info – Preise/Lager
> Dokumente > Artikel-Info > Register Preise/Lager

*Abb. C-322 Artikel-Info – Preise*

In diesem Register können Sie sich die Preise zu einem Produkt anzeigen lassen.

#### Auswahl
Diese Felder sind im Register Info beschrieben.

- "Artikel-Info - Info" auf Seite C-617

**Nur Default-Tarif** Die Anzeige der Preise kann auf den Standard-Tarif einschränken werden.
- Alle Tarife werden angezeigt, die dem Produkt zugeordnet sind.
- [x] Nur der Standard-Tarif wird angezeigt.

**Schlüssel nach Bezeichnungen sortieren** Die Anzeige der Preise kann nach Preisschlüsseln sortiert werden.
- Die Preise werden in der Reihenfolge angezeigt, in der sie im System hinterlegt sind.
- [x] Die Anzeige wird nach den Bezeichnungen für die Preisschlüssel sortiert.

**Jahrgang absteigend sortieren** Die Anzeige der Preise kann nach Jahrgang sortiert werden.
- Die Preise werden in der Reihenfolge angezeigt, in der sie im System hinterlegt sind.
- [x] Die Anzeige wird nach den Bezeichnungen für die Preisjahrgänge sortiert.

#### Standardmaße und Lager
**Breit, Höhe** Standardbreite und -höhe aus den Stammdaten. Wenn keine Standardmaße hinterlegt sind, bleibt die Anzeige auf 0.

**[F3]** Über die Schaltfläche können Sie den Dialog Lagerinfo öffnen, ohne die Artikel-Info zu schließen.

- ⇨ "Lagerinfo" auf Seite C-758

#### Anzeige
In der Anzeige werden die Preise aufgelistet, die dem Produkt zugeordnet sind. Einzelpreise werden direkt in dieser Tabelle angezeigt. Für alle anderen Preisformen wird eine Schaltfläche angezeigt, z. B. [Vektor]. Über die Schaltfläche können die entsprechenden Preise angezeigt werden.

### Artikel-Info – Anlagen
> Dokumente > Artikel-Info > Register Anlagen

*Abb. C-323 Artikel-Info – Anlagen*

In diesem Register können Sie sich die Anhänge anzeigen lassen, die zu dem aktuellen Produkt hinterlegt sind. Bei Stücklisten werden auch die Anhänge zu den Stücklisten-Komponenten aufgeführt.

#### Auswahl
Diese Felder sind im Register Info beschrieben.

- "Artikel-Info - Info" auf Seite C-617

#### Dateianhang
In der Übersicht werden alle angehängten Dateien aufgelistet. Dies können Anhänge zum Hauptprodukt und zu den Stücklisten-Komponenten sein.

Über das Kontext-Menü Verknüpfung hinzufügen können Sie eine Datei als Anlage hinzufügen.

## Zusatz Stückliste – Ergänzungen
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Funktionen > Gruppe Position > Zusatz Stückliste

*Abb. C-324 Zusatz Stückliste – Ergänzungen*

In diesem Dialog können Sie Angaben zu einer Stücklisten-Komponente ergänzen.

### Kosten
**Kostenstelle** Angabe der Kostenstelle zur markierten Stücklisten-Komponente. Die Angabe wird aus den Stammdaten übernommen. Sie kann geändert werden.

**Kostenart** Angabe der Kostenart zur markierten Stücklisten-Komponente. Die Angabe wird aus den Stammdaten übernommen. Sie kann geändert werden.

## Preisrecorder
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Funktionen > Gruppe Position > Preisrecorder

*Abb. C-325 Preisrecorder*

In diesem Dialog prüfen Sie die Preisentwicklung des erfassten Produkts über einen bestimmten Zeitraum. Dabei werden nur manuelle Preise berücksichtigt. Den Preis eines markierten Eintrags können Sie in den aktuellen Auftrag übernehmen.

### Auswahl
Sie können die Kriterien bestimmen, nach denen die Preisentwicklung dargestellt werden soll.

**Artikel** Anzeige der Stammdaten des markierten Produkts.

**Gleicher Produktaufbau** Als Vergleichskriterium kann der Aufbau des Produkts herangezogen werden.
- Der Produktaufbau wird nicht berücksichtigt.
- [x] Nur Positionen mit identischem Aufbau werden zum Vergleich herangezogen.

**Gleiche Abmessungen** Als Vergleichskriterium kann die Größe des Produkts herangezogen werden.
- Die Größe wird nicht berücksichtigt.
- [x] Nur Positionen mit identischen Abmessungen werden zum Vergleich herangezogen.

**Nur Dokumente der letzten ... Tage** Vergleichszeitraum
- Positionen aus allen verfügbaren Dokumenten werden berücksichtigt.
- [x] Das Feld für die Angabe der Tage wird freigeschaltet. Zum Vergleich werden nur Dokumente aus dem angegebenen Zeitraum herangezogen.

### Dokumente
Sie können entweder Aufträge und/oder Angebote auswerten oder Bestellungen und/oder Anfragen.

**Aufträge** Einschränkung der Suche auf Aufträge.
- Aufträge werden nicht ausgewertet.
- [x] Aufträge werden ausgewertet.

**Angebote** Einschränkung der Suche auf Angebote.
- Angebote werden nicht ausgewertet.
- [x] Angebote werden ausgewertet.

**Bestellungen** Einschränkung der Suche auf Bestellungen.
- [ ] Bestellungen werden nicht ausgewertet.
- [x] Bestellungen werden ausgewertet.

**Anfragen** Einschränkung der Suche auf Anfragen.
- Anfragen werden nicht ausgewertet.
- [x] Anfragen werden ausgewertet.

### Archiv
Wenn Ihnen mehrere Archive zur Verfügung stehen, können Sie diejenigen auswählen, auf die die Suche ausgedehnt werden soll.

## Artikel fixieren
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Funktionen > Gruppe Position > Artikel fixieren

*Abb. C-326 Artikel fixieren*

In diesem Dialog können Sie den aktuellen Produktaufbau fixieren und als kundenindividuelles Produkt unter einer neuen Produktnummer speichern.

Der Produktaufbau von fixierten Artikeln kann in der Positionserfassung und in der Produktverwaltung nicht geändert werden. Der Preis und der Rabatt können jedoch in der Positionserfassung geändert werden.

> **Fixierte Artikel als Position erfassen**
> Damit kundenindividuelle Produkte in die Produktsuche einbezogen werden, muss in der Positionserfassung im Menü Optionen > Gruppe Position der Eintrag Artikelsuche kundenindividuell aktiviert werden.
>
> ⇨ "Menü Optionen" auf Seite C-454

### Neuer Artikel
**Artikelnummer** Eingabe einer neuen Produktnummer. Mit der Lupe können Sie sich die freien Nummern anzeigen lassen.

**Matchcode** Der Matchcode dient als Suchkriterium.

**Preis fixieren** Der aktuelle Preis kann in die Produktdefinition übernommen werden.
- Der Preis wird nicht fixiert. Die Preisfindung wird über den Preisjahrgang und -schlüssel aus den Stammdaten gesteuert.
- [x] Der aktuelle Preis aus der Positionserfassung wird fixiert. Das Produkt hat einen festen Preis.

### Kundenindividueller Artikel
**Als kundenindividuellen Artikel speichern** Das neue Produkt kann so gespeichert werden, dass es für alle Kunden erfasst werden kann oder nur für den aktuellen.
- Das Produkt kann für alle Kunden im Auftrag erfasst werden.
- [x] Das Produkt wird kundenindividuell gespeichert und kann nur für den aktuellen Kunden im Auftrag erfasst werden. Das Feld Fremdartikel wird freigeschaltet.

**Fremdartikel** Wird das erfasste Produkt vom Kunden selbst geliefert, können Sie es als Fremdartikel speichern. In diesem Fall wird es nicht berechnet.

## Position kopieren
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Funktionen > Gruppe Position > Kopie aus Position

*Abb. C-327 Position kopieren*

In diesem Dialog können Sie die Daten einer Position kopieren, z. B. aus einem anderen Auftrag.

### Dokument wählen
**Typ** Auswahl des Dokumententyps, zu dem das Quelldokument gehört.

**Nummer** Nummer des Quelldokuments.

**Position** Eingabe der Positionsnummer. Sie können mehrere Nummern angeben und diese mit einem Komma trennen.
Statt der Eingabe der Positionsnummern können Sie die gewünschten Positionen in der Übersicht markieren.

### Optionen
**Neue Position erzeugen** Mit dieser Einstellung legen Sie fest, wie kopierte Positionen eingefügt werden.
- Die kopierte Position ersetzt die markierte Position im Ziel-Dokument. Der Produktaufbau wird mit allen Maßen übernommen.
  Diese Form der Übernahme ist nur möglich, wenn eine einzelne Position kopiert wird.
- [x] Die kopierte Position wird im Ziel-Dokument als neue (zusätzliche) Position eingefügt.

**Nur Produktaufbau kopieren** Mit dieser Einstellung legen Sie fest, ob Maße und Preise übernommen werden.
- Die kopierte Position wird vollständig mit allen Maßen übernommen. Diese Einstellung gilt immer, wenn Sie die kopierte Position als neue Position einfügen.
- [x] Aus der kopierten Position wird nur der Produktaufbau übernommen.

**Mengenfaktor** Mit dieser Einstellung können Sie die Stückzahl pro Position bestimmen.

> **Beispiel**
> Ein Kunde kopiert eine Auftragsposition mit der Stückzahl 1.
> Bei einem Mengenfaktor von 5 ergibt sich für die neue Position die Stückzahl 5.
>
> Die Preisberechnung orientiert sich an der neuen Stückzahl der Auftragsposition:
> Auftragsposition mit der Stückzahl 1 zu einem Preis von 100 €
> Mit dem Mengenfaktor 5 kopierte Auftragsposition = 100 € x 5 = 500 €

### Position wählen
Liste aller Positionen im ausgewählten Dokument.

Mit diesen Schaltflächen können Sie alle Positionen automatisch markieren, die kopiert werden sollen, oder alle Markierungen entfernen.

**[Anzeigen]** Öffnet den Dialog Dokumentenansicht als Vorschau auf das Dokument.
- ⇨ "Dokument anzeigen" auf Seite C-560

## Kosten- und Aufschlagskalkulation (Position)
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Funktionen > Gruppe Position > Kosten- und Aufschlagskalkulation > Übersicht, Detail - Position, Detail - Stückliste

*Abb. C-328 Kosten- und Aufschlagskalkulation*

In diesen Dialogen können Sie die aktuelle Kosten- und Aufschlagskalkulation pro Position bis auf die Ebene der Stücklisten-Komponenten prüfen.

> **Voraussetzung**
> Die Kosten- und Aufschlagskalkulation kann nur angezeigt werden, wenn in der Tarifzuordnung die Checkbox Herstellerkalkulation aktiviert ist und in den Firmendaten die Aufschläge hinterlegt sind.

## Versicherungsleistung
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Funktionen > Gruppe Position > Menü Versicherungspreise

*Abb. C-329 Versicherungsleistung*

In diesem Dialog geben Sie die Details an, die für die Abrechnung des Glasers mit der Versicherung benötigt werden.

Die Register nach Frankfurter und nach Gothaer stehen zur Verfügung. Diese Register sind nur freigeschaltet, wenn die zugehörigen Versicherungspreise angelegt sind.

- ⇨ Stammdaten, "Versicherungspreise" auf Seite B-713

### Kalkulationsart
Die Wahl der Option bestimmt die Kalkulationsart für die Auftragsposition:

- **Reparatur:** Die Reparatur wird nach dem mit der Versicherung vereinbarten Preis kalkuliert.
- **Notverglasung:** Die Notverglasung wird nach dem mit der Versicherung vereinbarten Preis kalkuliert.
- **Standard:** Die neue Scheibe wird nach dem mit der Versicherung vereinbarten Preis kalkuliert.

### Allgemein
**Werkstattarbeit, Entsorgungskosten, Arbeit auf Dächern** Zusätzlich Arbeiten können berechnet werden, wenn die entsprechenden Checkboxen markiert sind.
- Die zusätzlichen Kosten sind nicht entstanden und werden nicht berechnet.
- [x] Die zusätzlichen Kosten sind entstanden und sollen berechnet werden.

### Arbeitszeit
Die Wahl der Option bestimmt, ob Zuschläge für die Arbeitszeit anfallen:
- **reguläre Arbeitszeit:** Es werden keine weiteren Zuschläge für die Arbeitszeit erhoben.
- **außerhalb der regulären Arbeitszeit:** Für Arbeiten außerhalb der regulären Arbeitszeit werden die mit der Versicherung vereinbarten Zuschläge berechnet.
- **an Sonn-/Feiertagen:** Für Arbeiten an Sonn- und Feiertagen werden die mit der Versicherung vereinbarten Zuschläge berechnet.

**Abweichende Material-, Montagekosten** Diese beiden Felder werden nur im Register nach Gothaer angezeigt. Sie können die Kosten für Material und Montage abweichend von den in der Preistabelle hinterlegten Preisen eintragen.

### Versicherungspreis
**Schlüssel** Auswahl des Preisschlüssels, der für die Kalkulation des Preises herangezogen werden soll.

**Rahmen aus** Diese Felder werden nur im Register nach Gothaer angezeigt. Die Wahl der Option bestimmt, wie der Preis für den Rahmen berechnet werden soll:
- **Holz:** Für die Auftragsposition wird ein Holzrahmen berechnet.
- **Metall:** Für die Auftragsposition wird ein Metallrahmen berechnet.
- **Kunststoff:** Für die Auftragsposition wird ein Kunststoffrahmen berechnet.

### Glaskleber
Zur Berechnung des Klebers wählen Sie den zu verwendenden Kleber aus.

**Kanten Breite, Höhe** Zur Berechnung des verbrauchten Klebers geben Sie die Breite und Höhe der Kanten ein, die verklebt werden.

## Teillieferungen
> Dokumente > Auftrag > Teillieferung

In diesem Dialog können Sie Teillieferungen erstellen und sich eine Übersicht über den Auftragsstatus der Teillieferungen anzeigen lassen.

Der Dialog Teillieferungen ist für Auftrag und Bestellung gleich. Er wird in dieser Anleitung am Beispiel Auftrag beschrieben.

> **Voraussetzungen**
> Teillieferungen können nur ausgelöst werden, wenn diese Funktion in den Kundenstammdaten und in den Kopfdaten des Auftrags aktiviert ist. Wenn zusätzlich eine Teilrechnung gestellt werden soll, muss auch diese Option in den Kundenstammdaten und den Kopfdaten aktiviert sein.
> Eine Teillieferung kann nur ausgelöst werden, wenn mindestens ein Stück einer Auftragsposition aus der Produktion als fertig produziert gemeldet ist. In den Firmenstammdaten wird festgelegt, bei welchem Status eine Position als fertig produziert gilt.

In diesem Dialog finden Sie folgende Register:
- "Teillieferungen - Pro Fertigmeldung / Wareneingang" auf Seite C-631
- "Teillieferungen – Pro Gestell" auf Seite C-634

### Teillieferungen – Pro Fertigmeldung / Wareneingang
> Dokumente > Auftrag > Teillieferung > Register pro Fertigmeldung / Wareneingang

*Abb. C-330 Teillieferung - pro Fertigmeldung / Wareneingang*

In diesem Register können Sie Teillieferungen zu Aufträgen des gewählten Nummernverwalters erstellen.

#### Selektion
**Nummernverwalter** Auswahl des gewünschten Nummernverwalters.

#### Dokumente
In der Übersicht werden alle Dokumente des gewählten Nummernverwalters angezeigt.

Die Dokumente werden in roter oder grüner Schrift angezeigt. In grüner Schrift werden Aufträge und Bestellungen angezeigt, die komplett ausgeliefert sind. Zusätzlich ist die Checkbox in der Spalte Komplett markiert.
In roter Schrift werden Aufträge angezeigt, die noch nicht komplett ausgeliefert sind.

- **Auftrag:** Auftragsnummer.
- **Kunde, Name:** Nummer und Name des Marktpartners aus dem Auftrag.
- **Status:** Status des Auftrags.
- **Fertig %:** Anteil der Positionen, die als fertig produziert gemeldet sind. Der Anteil richtet sich nach der Gesamtstückzahl und wird in Prozent angezeigt.
- **Teillieferfähig %:** Anteil der Positionen, die teilgeliefert werden können. Der Anteil richtet sich nach der Gesamtstückzahl und wird in Prozent angezeigt. Wenn noch keine Positionen des Auftrags teilgeliefert sind, entspricht der Anteil Teillieferfähig % dem Anteil Fertig %.

> **Beispiel**
> Ein Auftrag hat 10 Auftragspositionen, von denen 6 als fertig produziert gemeldet sind. Es wurden noch keine Teillieferungen ausgelöst.
> Der Anteil Fertig % und der Anteil Teillieferfähig % beträgt jeweils 60%.
> Von dem Auftrag werden 2 Auftragspositionen teilgeliefert.
> Der Anteil Fertig % beträgt noch immer 60%, der Anteil Teillieferfähig % jedoch nur noch 40%, da 2 Positionen bereits teilgeliefert wurden und somit nur noch 4 Positionen für die Teillieferung bereitstehen.

- **Komplett:** Die Checkbox ist markiert, wenn der Auftrag komplett ausgeliefert ist.

> **Aufträge manuell als komplett melden**
> Sie können noch nicht fertiggemeldete Aufträge manuell als komplett melden, indem Sie in der Tabellenspalte Komplett die Checkbox aktivieren. Der Dokumentenstatus des markierten Auftrags wird geändert.

#### Positionen
In der Übersicht werden die Positionen des markierten Auftrags aus der Übersicht Dokumente angezeigt.

- **Pos.:** Nummer der Auftragsposition.
- **Status:** Status der Auftragsposition.
- **Fertig %:** Anteil der Positionen, die als fertig produziert gemeldet sind. Der Anteil richtet sich nach der Gesamtstückzahl und wird in Prozent angezeigt.
- **Teillieferfähig %:** Anteil der Positionen, die teilgeliefert werden können. Der Anteil richtet sich nach der fertiggemeldeten Menge und wird in Prozent angezeigt.
- **Menge (original):** Menge der Auftragsposition.
- **Menge (teilgeliefert):** Menge, die aus der Position teilgeliefert wurde.
- **Menge (fertig):** Menge der fertiggemeldeten Auftragsposition.
- **Teilliefermenge:** Menge, zu der eine Teillieferung erstellt werden soll.

Sie können in die Tabellenspalte **Teillieferung** eintragen, wie viel Stück der fertiggemeldeten Menge teilgeliefert werden sollen.

#### Ziel
**Nummernverwalter** Das Dokument kann in einen anderen Nummernverwalter gestellt werden, den Sie in der Kombobox wählen können.

**AV-Bereich** Das Dokument kann einem anderen AV-Bereich zugeordnet werden.
- Das Dokument wird keinem anderen AV-Bereich zugeordnet.
- [x] Das Dokument wird dem gewählten AV-Bereich zugeordnet. Die Kombobox zur Auswahl des AV-Bereichs wird freigeschaltet.

### Teillieferungen – Pro Gestell
> Dokumente > Auftrag > Teillieferung > Register pro Gestell

*Abb. C-331 Teillieferung - pro Gestell*

In diesem Register können Sie Teillieferungen zu Auftragspositionen erstellen, die auf ein Gestell gebucht sind. Sie können sich die Auftragspositionen auf einem Gestell nach Nummernverwalter oder nach Kunde anzeigen lassen.

#### Selektion
Mit der Wahl der Option können Sie die Suche auf einen bestimmten Nummernverwalter oder Kunden einschränken.

- **Nummernverwalter:** Auswahl eines Nummernverwalters.
- **Kunde:** Nummer und Name des Kunden.

**Liefertermin von, bis** Lieferzeitraum der Aufträge, nach denen gesucht werden soll.

**Status von, bis** Statusnummernbereich der Aufträge, nach denen gesucht werden soll.

#### Gestell - Aufträge
In dieser Übersicht wird angezeigt, von welchen Aufträgen einzelne oder alle Auftragspositionen auf ein Gestell gebucht sind.

- **Gestell:** Gestellnummer, auf die die Auftragsposition gebucht ist.
- **Auftrag:** Auftragsnummer.
- **Kunde, Name:** Nummer und Name des Marktpartners aus dem Auftrag.
- **Liefertermin:** Liefertermin aus dem Auftrag.
- **Status:** Status des Auftrags.
- **Teillieferfähig %:** Anteil der Positionen, die teilgeliefert werden können. Der Anteil richtet sich nach der Gesamtstückzahl und wird in Prozent angezeigt.
- **Teilgeliefert %:** Anteil der Positionen, die bereits teilgeliefert sind. Der Anteil richtet sich nach der Gesamtstückzahl und wird in Prozent angezeigt.

Sie können eine Teillieferung für ein Gestell erstellen, wenn Sie mit Doppelklick den Zeilenkopf des Auftrags für die Teillieferung auswählen. Der ausgewählte Auftrag wird mit einem roten X im Zeilenkopf markiert. Nach Erstellen einer Teillieferung wird der Dialog Formulardruck-/Etikettendruck geöffnet.

- ⇨ "Formular-/Etikettendruck" auf Seite C-655

#### Gestell - Positionen
In der Übersicht werden die Positionen des Auftrags angezeigt, der in der Übersicht Gestell-Aufträge markiert ist.

- **Pos.:** Nummer der Auftragsposition.
- **Status:** Status der Auftragsposition.
- **Produkt:** Produktnummer und -bezeichnung.
- **Breite, Höhe:** Maße der Position.
- **Menge (original):** Menge der Auftragsposition.
- **Menge (auf Gestell):** Menge der Auftragsposition auf dem Gestell.
- **Menge (teilgeliefert):** Menge, die aus der Position bereits teilgeliefert ist.

#### Ziel
**Nummernverwalter** Die erstellten Teillieferungen können in einen anderen Nummernverwalter gestellt werden. Wenn Sie einen neuen Namen eintragen, wird der Nummernverwalter angelegt. Standardmäßig ist der Nummernverwalter ausgewählt, in dem die Aufträge stehen.

**Lieferdatum** Sie können ein Lieferdatum für die Teillieferung festlegen.
- Das Lieferdatum wird aus den Kundenstammdaten oder dem Auftrag übernommen.
- [x] Sie können das Lieferdatum eintragen. Das Feld zur Eingabe wird freigeschaltet.

**LKW** Sie können einen Lkw für die Teillieferung wählen.
- Der Lkw wird aus den Kundenstammdaten oder dem Auftrag übernommen.
- [x] Sie können einen Lkw wählen. Die Kombobox zur Auswahl wird freigeschaltet.

**Tour** Sie können eine Tour für die Teillieferung wählen.
- Die Tour wird aus den Kundenstammdaten oder dem Auftrag übernommen.
- [x] Sie können eine Tour wählen. Die Kombobox zur Auswahl wird freigeschaltet.

**Fahrer** Sie können einen Fahrer für die Teillieferung wählen.
- Der Fahrer wird aus den Kundenstammdaten oder dem Auftrag übernommen.
- [x] Sie können einen Fahrer wählen. Die Kombobox zur Auswahl wird freigeschaltet.

## Makros
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Aufbau > Gruppe Makro

Produktaufbauten können als Makro(befehl) gespeichert werden und stehen dann ohne weitere Eingaben bei der Erfassung zur Verfügung.

Die Dialoge zum Speichern und Verwalten von Makros sind für alle Dokumentenarten gleich. Sie werden in dieser Anleitung am Beispiel Auftrag beschrieben.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Makro sichern" auf Seite C-637
- "Makro ändern" auf Seite C-638
- "Makro suchen" auf Seite C-640
- "Makro kopieren" auf Seite C-641

### Makro sichern
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Aufbau > Gruppe Makro > Sichern, Löschen

*Abb. C-332 Makro sichern (löschen)*

In diesem Dialog können Sie ein Produkt mit einer komplizierten Stückliste als Makro sichern.

- ⇨ Tutorial, "Makro speichern" auf Seite C-166

#### Definition
**Makroname** Name des neuen Makros, der zur Auswahl in der Positionserfassung angezeigt wird.

**Exakte Suche** Die Suche nach Makros kann Preise berücksichtigen. Die Checkbox wird nur angezeigt, wenn die Einstellung zur Makro-Preissuche in den Firmendaten aktiviert ist.
- Das Makro kann ohne den exakten Preis übernommen werden.
- [x] Das Makro kann mit dem exakten Preis übernommen werden.
  - ⇨ Stammdaten, "Firmendaten - Preisberechnung" auf Seite B-959

Mit der Wahl der Option legen Sie fest, wie das Makro gespeichert wird:
- **Kundenbezogen:** Das neue Makro wird kundenbezogen gespeichert. Er wird dann nur zur Auswahl angeboten, wenn ein Auftrag für den gewählten Kunden erfasst wird. Das Feld Nummer wird freigeschaltet.
- **Allgemein:** Das neue Makro wird so gespeichert, dass er für alle Kunden zur Auswahl angeboten wird. Das Feld Nummer wird gesperrt.

#### Kunde
**Nummer** Dieses Feld ist nur freigeschaltet, wenn die Option Kundenbezogen markiert ist. Die Kundennummer kann eingegeben oder über die Lupe ausgewählt werden.

**Name** Der Kundenname wird aus den Stammdaten übernommen, wenn eine Kundennummer eingetragen ist.

### Makro ändern
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Aufbau > Gruppe Makro > Ändern

*Abb. C-333 Makro ändern*

Über diesen Dialog können Sie gespeicherte Makros bearbeiten.

- ⇨ Tutorial, "Makros ändern" auf Seite C-169

#### Auswahl
Die Felder in diesem Bereich sind nur freigeschaltet, wenn der Auswahl-Modus aktiviert ist.

- **Alle Makros:** Die Auswahl wird auf alle gespeicherten Makros ausgedehnt.
- **Kundenbezogene Makros:** Die Auswahl wird auf kundenbezogenen Makros eingeschränkt. Die Felder von und bis werden freigeschaltet.

**Von... bis** Eingabefelder zum Einschränken der Suche nach kundenbezogenen Makros. Die Suche der Makros beschränkt sich auf die Nummernfolge zwischen den eingegebenen Kundennummern. Diese Felder sind nur freigeschaltet, wenn die Option kundenbezogene Makros markiert ist.

#### Preisänderung
Die Felder in diesem Bereich sind nur freigeschaltet, wenn Makros angezeigt werden.

**Wert** Betrag, um den der Preis des markierten Makros geändert werden soll.
Mit der Wahl der Option legen Sie fest, wie der Preis geändert werden soll:
- **Absolut** und ein Wert, z. B. 5 oder -5, wenn der Preis um 5 Euro erhöht oder vermindert werden soll.
- **Prozentual** und ein Wert, z. B. 2 oder -2, wenn der Preis um 2 Prozent erhöht oder vermindert werden soll.

#### Rundung
Die Rundung in allen markierten Makros wird auf die ausgewählte Rundungsart gesetzt.

#### Makros
Liste aller Makros, die den Auswahlkriterien entsprechen. Zur Änderung können mehrere Einträge markiert werden (Mehrfachmarkierung).

### Makro suchen
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Aufbau > Gruppe Makro > Suchen

*Abb. C-334 Makro suchen*

In diesem Dialog suchen Sie nach bestimmten Makros. Die Felder sind in den beiden Registern gleich. Die Wahl des Registers schränkt die Suche ein.

- ⇨ Tutorial, "Makros" auf Seite C-164

#### Makros
**Name** Name des Makros, das gesucht werden soll. Das Ergebnis der Suche wird in der Übersicht aufgelistet (Trefferliste).

#### Aufbau
Der Aufbau des Produktes wird angezeigt, wenn in der Trefferliste ein Makro markiert ist.

### Makro kopieren
> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Aufbau > Gruppe Makro > Kopieren

*Abb. C-335 Makro kopieren*

In diesem Dialog kopieren Sie ein kundenbezogenes Makro, z. B. zu den Filialen des Kunden oder zu einem anderen Kunden.

- ⇨ Tutorial, “Makros kopieren" auf Seite C-172

#### Quelle
**Kunde** Nummer des Kunden, dessen Makro(s) kopiert werden soll(en).

#### Ziel
Mit der Wahl der Option legen Sie fest, wohin die Makros kopiert werden sollen:
- **Kunde:** Nummer des Kunden, zu dem Makro(s) kopiert werden sollen.
- **Filialen:** Mit dieser Option werden die Filialen des Kunden angezeigt. Wenn mehrere Filialen aufgelistet werden, können diejenigen ausgewählt werden, zu denen das Makro kopiert werden soll.
- **Hauptktn.:** Mit dieser Option werden die Makros einer Filiale zum Hauptkunden kopiert.

#### Optionen
Mit der Wahl der Option legen Sie fest, ob vorhandene Makros gelöscht oder überschrieben werden sollen:

- **Vorhandene Makros im Ziel updaten:** Die neuen Makros werden hinzugefügt. Wenn bereits Makros für den Zielkunden gespeichert sind, bleiben diese unverändert erhalten.
- **Alle Makros im Ziel zuvor löschen:** Vor dem Kopieren werden alle Makros beim Zielkunden gelöscht. Nach dem Kopieren stehen für den Zielkunden nur die neuen Makros zur Verfügung.

## Nummernverwalter
> Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > NV Angebot, NV Auftrag, NV Gutschrift, NV Anfrage, NV Bestellung

Der Dialog Nummernverwalter ist für alle Dokumentenarten gleich. Er wird in dieser Anleitung am Beispiel Auftrag beschrieben.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite C-643
- "Nummernverwalter" auf Seite C-645
- "Nummernverwalter kopieren" auf Seite C-649

### Menü Funktionen
> Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > NV Angebot, NV Auftrag, NV Gutschrift, NV Anfrage, NV Bestellung

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Nummernverwalter zu schließen.

Das Menü ist in folgende Gruppen gegliedert:
- Gruppe Bearbeiten
- Gruppe Dokument
- Gruppe Dokumentenkopie
- Gruppe Übersicht
- Gruppe Export
- Gruppe Produktion
- Gruppe Routenoptimierung

#### Gruppe Bearbeiten
- **Kopieren nach:** Öffnet den Dialog Nummernverwalter Kopieren, um Dokumente in einem Nummernverwalter zu selektieren und diese dann in einen neuen Nummernverwalter zu kopieren.
  - ⇨ Tutorial, "Nummernverwalter kopieren" auf Seite C-192
  - ⇨ "Nummernverwalter kopieren" auf Seite C-649
- **Überschreiben:** Leert den gesamten Nummernverwalter. Der Modus wechselt automatisch zu Anlegen.
- **Statusänderung:** Öffnet den Dialog Statusänderung, um den Status manuell umzusetzen und den Nummernverwalter zu ändern.
  - ⇨ "Statusänderung" auf Seite C-566
- **Kennzeichenänderung:** Öffnet den Dialog Bestellkennzeichen ändern, um die Beschaffungsart zu ändern.
  - ⇨ "Bestellkennzeichen ändern" auf Seite C-650

#### Gruppe Dokument
- **Dokument anzeigen:** Öffnet den Dialog Dokumentenansicht als Vorschau auf das Dokument.
  - ⇨ "Dokument anzeigen" auf Seite C-560
- **Historie:** Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des Dokuments.
  - "Historie" auf Seite C-564
- **Dokumentendaten:** Öffnet den Dialog Dokumente, um ggf. die Termine und den Status in Aufträgen und Bestellungen zu korrigieren.
  - ⇨ "Dokumentendaten" auf Seite C-754
- **Dokumentenerfassung:** Öffnet das markierte Dokument.
  - ⇨ "Dokument - Kopfdaten" auf Seite C-424

#### Gruppe Dokumentenkopie
- **Dokumente kopieren:** Öffnet den Dialog Dokumente kopieren, um ein Dokument in den gleichen oder anderen Dokumententyp zu kopieren.
  - ⇨ Tutorial, "Dokumente kopieren" auf Seite C-250
  - ⇨ "Dokumente kopieren" auf Seite C-543
- **Teillieferung:** Öffnet den Dialog Dokumente kopieren im Modus Teillieferung, um eine Teillieferung zu erfassen.
  - ⇨ Tutorial, "Teillieferungen" auf Seite C-262
- **Reklamation:** Öffnet den Dialog Dokumente kopieren im Modus Reklamation, um eine Reklamation zu erfassen.
  - ⇨ Tutorial, "Reklamationen" auf Seite C-289
- **Anzahlung:** Öffnet den Dialog Dokumente kopieren im Modus Anzahlung, um eine Anzahlung zu erfassen.
  - ⇨Tutorial, "Anzahlungen" auf Seite C-280

#### Gruppe Übersicht
- **Artikel-Info:** Öffnet einen Dialog mit detaillierten Informationen zum Produkt, um Preise und Verfügbarkeit zu prüfen.
  - ⇨ "Artikel-Informationen" auf Seite C-616
- **Teillieferungsübersicht:** Öffnet die Liste der Teillieferungen zum aktuellen Auftrag.
  - ⇨ "Teillieferungsübersicht" auf Seite C-570
- **Anzahlungsübersicht:** Öffnet die Liste der geleisteten Anzahlungen zum aktuellen Auftrag.
  - ⇨ "Anzahlungsübersicht" auf Seite C-573

#### Gruppe Export
- **Xternal Dateien erstellen:** Erstellt für alle Bestellungen im Nummernverwalter eine Xternal Datei. Die Funktion ist nur kundenspezifisch freigeschaltet.

#### Gruppe Produktion
- **Produktionsübersicht:** Öffnet den Dialog Übersicht Statusrückmeldungen zum markierten Auftrag. Die Funktion ist gesperrt, wenn Sie im aktuellen Dokument keine Positionen enthalten sind, die an die Produktion übergeben werden sollen.
  - ⇨ "Übersicht Statusrückmeldung" auf Seite C-590

#### Gruppe Routenoptimierung
Diese Gruppe ist nur freigeschaltet, wenn auf Ihrem System auch A+W Logistics Optimizer installiert ist.

- **Nummernverwalter übergeben:** Übergibt Aufträge aus dem Nummernverwalter im Modus Lieferung. Die Auftragsnummern werden an den Logistic Service gesendet, der die erforderlichen Daten aus der Datenbank liest.

### Nummernverwalter
> Dokumente > Auftrag > NV Auftrag

Der Dialog Nummernverwalter und die zugehörigen Menüs sind für alle Dokumentenarten und Module gleich. Er wird in dieser Anleitung am Beispiel Auftrag beschrieben.

**Zu Dialogbeschreibung:**
- ⇨ Nummernverwalter - Sortierung
- ⇨ Nummernverwalter kopieren

*Abb. C-336 Nummernverwalter*

In diesem Dialog können Sie Nummernverwalter anlegen und verwalten.

- ⇨ Tutorial, "Nummernverwalter" auf Seite C-186

#### Identifikation
**Mitarbeiter** Name des Mitarbeiters, der sich in A+W Business angemeldet hat.

**Nummernverwalter** Name des ausgewählten Nummernverwalters. Das Feld ist freigeschaltet, wenn Sie einen neuen Nummernverwalter anlegen.
- ⇨ Tutorial, "Nummernverwalter" auf Seite C-186

**Auftrag, Statusbereich von ... bis** Sie können Dokumente innerhalb einer Folge von Nummern oder von Statusnummern auswählen.

#### Auswahl
In der Liste werden alle angelegten Nummernverwalter angezeigt. Der ausgewählte Nummernverwalter wird im Feld Nummernverwalter angezeigt.

#### Optionen
**Anzeige** Sie können die Anzeige von Tabellenspalten in der Übersicht ausblenden.
Mit der Wahl des Eintrags **Komplett** werden alle Kopfdaten des Dokumentes angezeigt, bei **Lieferung** werden nur die für die Lieferung relevanten Daten angezeigt.

**Sortierung** Mit dieser Schaltfläche öffnen Sie den Dialog Nummernverwalter-Sortierung, in dem Sie die Sortierung der Listeneinträge ändern können.
- ⇨ "Nummernverwalter - Sortierung" auf Seite C-648

#### Zugriff auf
**Mandant** Beim Anlegen können den Mandanten auswählen, für den der Nummernverwalter gelten soll.

**Datenbank** Datenbanken, aus der die Dokumente angezeigt werden, z. B. ein Archiv.

#### Dokumente
In diesem Bereich werden alle Dokumente des ausgewählten Nummernverwalters aufgelistet, die den eingegebenen Kriterien entsprechen.

> **Benutzerdefinierte Spalte einfügen**
> In der Übersicht der Dokumente können benutzerdefinierte Spalten eingefügt werden, die über das Customizing mit beliebigen Daten gefüllt werden können. Wenn Sie sich an Ihren Ansprechpartner bei der A+W Software GmbH, wenn Sie solche Spalten einfügen wollen.

### Nummernverwalter – Sortierung
> Dokumente > Auftrag > NV Auftrag > [Sortierung]

*Abb. C-337 Sortierung*

In diesem Dialog legen Sie fest, wie die Dokumente im Nummernverwalter sortiert werden sollen.

### Nummernverwalter kopieren
> Dokumente > Auftrag > NV Auftrag > Menü Funktionen > Gruppe Bearbeiten > Kopieren nach

*Abb. C-338 Kopieren*

In diesem Dialog kopieren Sie Auftragsnummern, um sie in einen anderen Nummernverwalter zu stellen, z. B. aus dem Nummernverwalter für die Produktion in den Nummernverwalter für den Lieferscheindruck oder zur Weiterbearbeitung von einem Mitarbeiter zu einem anderen.

- ⇨ Tutorial, "Nummernverwalter kopieren" auf Seite C-192

#### Dokument
In diesem Bereich wird angezeigt, zu welcher Dokumentenart der Nummernverwalter gehört.

**Typ** Dokumententyp der Quelle.

#### Quelle, Ziel
**Mitarbeiter** Auswahl des Mitarbeiters, der für den Nummernverwalter zuständig ist.

**Nummernverwalter** Auswahl des Nummernverwalters, den Sie kopieren möchten.

### Bestellkennzeichen ändern
> Dokumente > Auftrag > NV Auftrag > Menü Funktionen > Gruppe Bearbeiten > Kennzeichenänderung

*Abb. C-339 Bestellkennzeichen ändern*

In diesem Dialog ändern Sie das Bestellkennzeichen aller Dokumente, die sich in dem aktuellen Nummernverwalter befinden. Dabei ändern Sie die Beschaffungsart und/oder den Lieferanten.

- ⇨ Tutorial, "Bestellung" auf Seite C-302

#### Modus
Mit der Wahl der Option legen Sie fest, für welche Positionsebene das Kennzeichen geändert werden soll:

- **Ändern auf Positionsebene:** Das Kennzeichen wird für das Hauptprodukt der Auftragsposition umgesetzt.
- **Ändern auf Stücklistenebene:** Das Kennzeichen wird an den Stücklisten-Komponenten umgesetzt.
- **Alle Gläser bestellen:** Alle Gläser der Aufträge erhalten dasselbe Bestellkennzeichen.

#### Lieferant für alle Glas-Bestellartikel
**Lieferant ändern** Für die gewählte Option (Ebene) kann der Lieferant geändert werden.
- Der Lieferant wird nicht geändert. Die Felder des Bereichs sind gesperrt.
- [x] Der Lieferant wird geändert. Die Felder des Bereichs sind freigeschaltet. Der Name des gewählten Lieferanten wird aus den Stammdaten übernommen.
Beachten Sie dazu die Auswahl der Option im Bereich Modus.

> **Alle Dokumente werden geändert**
> Beachten Sie, dass immer alle Dokumente des Nummernverwalters geändert werden.

#### Ändern auf Dokumentenebene
**Bestellung direkt an den Kunden** Die Bestellung kann vom Lieferanten direkt an den Kunden ausgeliefert werden.
- Die Bestellung wird nicht direkt an den Kunden geliefert.
- [x] Die Bestellung wird direkt an den Kunden geliefert. Diese Einstellung kann sinnvoll sein, wenn die Bestellung nicht für die Fertigung benötigt wird.
Damit wird im Auftrag die Checkbox Direktanlieferung durch den Lieferanten ebenfalls aktiviert. Bei der Bestellübergabe wird dann als abweichende Lieferanschrift die Kundenanschrift eingefügt.
  - ⇨ "Direktanlieferung durch den Lieferanten" auf Seite C-431

#### Beschaffungsart
**Beschaffungsart ändern** Für die gewählte Option (Ebene) kann die Beschaffungsart geändert werden.
- Die Beschaffungsart wird nicht geändert. Die Felder des Bereichs sind gesperrt.
- [x] Die Beschaffungsart wird geändert. Die Felder des Bereichs sind freigeschaltet.

**Von, nach** Auswahl der Beschaffungsart, die geändert werden soll und der neuen Beschaffungsart. Die Felder sind nur freigeschaltet, wenn die Checkbox **Beschaffungsart ändern** markiert ist.

**Nur für Produkt** Die Änderung der Beschaffungsart kann auf ein einzelnes Produkt eingeschränkt werden. Die Bezeichnung des gewählten Produkts wird aus den Stammdaten übernommen.
Beachten Sie dazu die Auswahl der Option im Bereich Modus.

## Druck
> Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Druck Angebot, Auftrag, Gutschrift, Anfrage, Bestellung

Der Dialog Formular-/Etikettendruck und die zugehörigen Menüs sind für alle Dokumentenarten gleich. Er wird in dieser Anleitung am Beispiel Auftrag beschrieben.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menüs im Formular-/Etikettendruck" auf Seite C-652
- "Vermaßte Skizze drucken" auf Seite C-665
- "Formular-/Etikettendruck" auf Seite C-655
- Touren/Fahrer Zuordnung

### Menüs im Formular-/Etikettendruck
> Dokumente > Auftrag > Auftrag auswählen > Menü Start > Gruppe Druck > Allgemeiner Formulardruck
>
> Dokumente > Auftrag > Druck Auftrag

Über die Menüs des Druckdialogs können Sie die Standardeinstellung des Dialoges festlegen und Funktionen für den Druck auswählen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite C-652
- “Gruppe Druckmodi" auf Seite C-654
- "Menü Optionen" auf Seite C-653

#### Menü Funktionen
> Dokumente > Auftrag > Auftrag auswählen > Menü Start > Gruppe Druck > Allgemeiner Formulardruck > Menü Funktionen
>
> Dokumente > Auftrag > Druck Auftrag > Menü Funktionen

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Formular- und Etikettendruck zu schließen.

Das Menü ist in folgende Gruppen gegliedert:
- Gruppe Allgemeine
- Gruppe Rechnungsdruck
- Gruppe Druck Server

**Gruppe Allgemeine**
- **Touren/Fahrer Zuordnung.** Öffnet den Dialog Touren/Fahrer Zuordnung, in dem Sie der Lieferung einen bestimmten Fahrer zuordnen können. Diese Funktion ist nur beim Druck von Lieferscheinen freigeschaltet.
  - ⇨ "Touren/Fahrer Zuordnung" auf Seite C-668
- **Dokument anzeigen:** Öffnet den Dialog Dokumentenansicht als Vorschau auf das Dokument.
  - ⇨ "Dokument anzeigen" auf Seite C-560
- **Vermaßte Skizze drucken:** Öffnet den Dialog Vermaßte Skizze drucken, um eine maßstäbliche Skizze im DIN-A4 Format zu drucken.
  - ⇨ "Vermaßte Skizze drucken" auf Seite C-665
- **Dokumentendaten:** Öffnet den Dialog Dokumente, um ggf. die Termine und den Status in Aufträgen und Bestellungen zu korrigieren.
  - ⇨ "Dokumentendaten" auf Seite C-754
- **Artikel Info:** Öffnet einen Dialog mit detaillierten Informationen zum Produkt, um Preise und Verfügbarkeit zu prüfen.
  - ⇨ "Artikel-Informationen" auf Seite C-616

**Gruppe Rechnungsdruck**
- **Storno von Rechnungs-/Lieferscheinnummern:** Diese Option ist nur freigeschaltet, wenn in den Firmendaten die Checkboxen für die Nummernvergabe aktiviert sind.
  - ⇨ Stammdaten, “Nummernvergabe pro Seite bei" auf Seite B-943

**Gruppe Druck Server**
- **Druck Server Monitor starten:** Öffnet den Dialog Druckaufträge, in dem eine Liste der aktuellen Druckaufträge angezeigt wird, die zum Drucker-Server gesendet wurden.
  - ⇨ Tutorial, “Druckauftrag" auf Seite C-201

#### Menü Optionen
> Dokumente > Auftrag > Auftrag auswählen > Menü Start > Gruppe Druck > Allgemeiner Formulardruck > Menü Optionen
>
> Dokumente > Auftrag > Druck Auftrag > Menü Optionen

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

> **Aktivierte Optionen nach dem Öffnen des Dialogs**
> Bitte beachten Sie, dass geänderte Optionen erst beim nächsten Öffnen des Dialogs wirksam werden.
> Wenn durch eine aktivierte Option eine Prüfung gestartet wurde, kann sich das Öffnen eines Dokuments verzögern. Der Grad der Verzögerung hängt von der Leistungsfähigkeit des Rechners ab.
> Die folgenden Beschreibungen stellen die aktivierte Option dar.

Das Menü ist in folgende Gruppen gegliedert:
- Gruppe Meldungen
- Gruppe Druckoptionen
- Gruppe Druckmodi

**Gruppe Meldungen**
- **Verarbeitungsende melden:** Wenn der Druckauftrag verarbeitet wurde, d. h. an den Drucker oder Server übergeben wurde, wird eine Meldung angezeigt.

**Gruppe Druckoptionen**
- **Inchzeichen drucken:** Wenn Sie mit den Maßen in Inch arbeiten, sollten Sie diese Option aktivieren, damit das Zeichen für Inch (") gedruckt wird.
  - ⇨ Stammdaten, "Maßsystem" auf Seite B-987
- **Faxnummer im Druckjobname:** Wenn Sie Dokumente per Fax senden, kann die Faxnummer im Namen des Druckauftrags angezeigt werden. Damit können Sie die Druckaufträge besser überwachen. Diese Option gilt für Druck über einen Drucker-Server.
- **E-Mail im Druckjobname:** Wenn Sie Dokumente per Mail senden, kann die E-Mail-Adresse des Marktpartners im Namen des Druckauftrags angezeigt werden. Damit können Sie die Druckaufträge besser überwachen. Diese Option gilt für Druck über einen Drucker-Server.
- **Steuerkorrektur bei Sammelrechnung (Wiederholungsdruck):** Wenn der Steuersatz in den einzelnen Aufträgen unterschiedlich ist, wird die Steuer im Wiederholungsdruck neu berechnet.
- **Lieferscheindruck mit fertig gemeldeter Menge:** Diese Option ist nur freigeschaltet, wenn zum markierten Dokument eine Rückmeldung aus der Produktion vorliegt.

**Gruppe Druckmodi**
> Dokumente > Auftrag > Druck Auftrag > Gruppe Druckmodi

Mit der Wahl des Druckmodus legen Sie fest, welche Formulare zur Auswahl angeboten werden. Den Druckmodus können Sie auch im Dialog selbst auswählen.
- ⇨ "Druckmodus" auf Seite C-658

### Formular-/Etikettendruck
> Dokumente > Auftrag > Auftrag auswählen > Menü Start > Gruppe Druck > Allgemeiner Formulardruck
>
> Dokumente > Auftrag > Druck Auftrag

**Zu Dialogbeschreibung:**
- ⇨ "Touren/Fahrer Zuordnung" auf Seite C-668

Der Dialog Formular-/Etikettendruck ist für alle Dokumente gleich. Er wird in dieser Anleitung am Beispiel Auftrag beschrieben. Dokumente werden in vorgegebene Formulare gedruckt und können auf einem Drucker oder auf dem Bildschirm ausgegeben werden.

- ⇨ Tutorial, "Druck" auf Seite C-196

> **Einträge in der Gruppe Druck**
> Standardmäßig wird in der Gruppe Druck nur der Eintrag Allgemeiner Formulardruck angezeigt. Sie können eigene Voreinstellungen für den Druck definieren. Diese werden dann ebenfalls zur Auswahl angeboten.
>
> ⇨ Stammdaten, "Druckaufträge" auf Seite B-1083

In diesem Dialog finden Sie folgende Register:
- "Formular-/Etikettendruck - Formulare" auf Seite C-656
- "Formular-/Etikettendruck - Etiketten" auf Seite C-662
- “Formular-/Etikettendruck – Dokumentenexport" auf Seite C-664

#### Formular-/Etikettendruck – Formulare
> Dokumente > Auftrag > Auftrag auswählen > Menü Start > Gruppe Druck > Allgemeiner Formulardruck > Register Formulare
>
> Dokumente > Auftrag > Druck Auftrag > Register Formulare

*Abb. C-340 Formular-/Etikettendruck – Formulare*

In diesem Register legen Sie die Optionen für den Druck von Dokumenten fest. In der Formularverwaltung kann angegeben werden, wie viele Exemplare gedruckt werden sollen.

- ⇨ Stammdaten, "Formularverwaltung - Optionen 1" auf Seite B-1070

**Selektion nach**
**Mitarbeiter** Name des Mitarbeiters, der sich in A+W Business angemeldet hat.

**Nummernverwalter** Beim Druck über den Dialog Nummernverwalter können Sie den Nummernverwalter auswählen, in dem die Dokumente für den Druck bereitgestellt sind. Die Dokumente des gewählten Nummernverwalters werden in der Übersicht im Bereich Dokumente angezeigt. Alle weiteren Einstellungen gelten dann für alle Dokumente des Nummernverwalters.
- ⇨ Tutorial, "Nummernverwalter" auf Seite C-186
- ⇨ "Nummernverwalter" auf Seite C-643

**Formularauswahl**
**Formular** Zur Auswahl werden die Formulare angeboten, die für den gewählten Druckpunkt zur Verfügung stehen.
Das Formular wird automatisch geändert, wenn Sie eine der Checkboxen im Bereich Sonderdruck markieren.
- ⇨ Tutorial, "Formular- und Etikettendruck" auf Seite C-197
- ⇨ Stammdaten, "Formularverwaltung" auf Seite B-1064

**Status** Der Status der Dokumente wird automatisch auf den Status umgesetzt, der dem gewählten Formular zugeordnet ist.
- ⇨ Stammdaten, "Statusverwaltung" auf Seite B-897

**Nummernkreise**
**(Präfix)** Wenn Sie für Ihre AV-Bereiche unterschiedliche Nummernkreise eingerichtet haben, können Sie festlegen, dass die Dokumentennummern aus den zugehörigen Nummernkreisen gezogen werden.
Die Felder sind abhängig von der gewählten Einstellung für Lieferscheine (Präfix) und Rechnungen freigeschaltet.

- **0-Vorg. Mandant + Bereich:** Die Felder Mandant und Bereich sind freigeschaltet.
- **1-Doku. Mandant + Bereich:** Der Mandant und der Bereich werden aus dem Dokument übernommen.
- **2-Doku. Mandant + Vorg. Bereich:** Der Mandant wird aus dem Dokument übernommen. Das Feld Bereich ist freigeschaltet.
- ⇨ Stammdaten, "Funktion der Nummernkreise" auf Seite B-441
- ⇨ Stammdaten, "Nummernkreise" auf Seite B-903

**Mandant** Mandant, aus dessen Nummernkreis die Dokumentennummer gezogen wird.

**Bereich** Bereich, aus dessen Nummernkreis die Dokumentennummer gezogen wird.

**Details**
**Datenbank** Wenn Sie mit mehreren Datenbanken arbeiten, müssen Sie die Datenbank auswählen.

**Druckdatum** Anzeige des aktuellen Tagesdatums (Systemdatum). Es kann nur bei Rechnungen geändert werden, bei denen das Rechnungsdatum die Zahlungsfristen bestimmt.

**Ausgabe auf**
Mit der Wahl der Option legen Sie fest, wie die Dokumente ausgegeben werden.

- **Drucker:** Die Dokumente werden direkt an den Drucker übergeben und gedruckt. Wenn keine anderen Einstellungen im Bereich Sonderdruck aktiviert sind, werden Dokumente auf Papier gedruckt. Diese Einstellung sollten Sie dann wählen, wenn Sie Dokumente für den Post- oder Faxversand fertig machen möchten.
  Wenn Sie im Bereich Sonderdruck eine oder mehrere Checkboxen aktivieren, werden aus dem Nummernverwalter die entsprechenden Dokumente ausgefiltert.
- **Bildschirm:** Ein einzelnes Dokument wird auf dem Bildschirm angezeigt und kann geprüft werden. Es kann aus dieser Anzeige heraus gedruckt werden. Auch die Ausgabe auf den Bildschirm gilt als Druck, nach dem Sie weitere Drucke nur starten können, wenn Sie im Bereich Sonderdruck die Checkbox Wiederholungsdruck markiert haben.
  Auch wenn Sie die Checkbox Sammeldruck markiert haben, wird nur das Dokument angezeigt, das in der Übersicht markiert ist.
- **Datei:** Alle aufgelisteten Dokumente werden als Dateien gespeichert und können dann elektronisch (per Datenaustausch) weitergegeben werden.
- **Server:** Die Dokumente werden auf dem Drucker-Server gespeichert und von dort automatisch weiter verarbeitet. Die Option Server ist nur freigeschaltet, wenn mit dem Print-Server gearbeitet wird.

> **Vor dem Druck Bildschirmausgabe erzeugen**
> Wenn Sie Dokumente mit maßstäblichen Skizzen drucken möchten, sollten Sie sich das Dokument zunächst auf dem Bildschirm anzeigen lassen. Sie können dann prüfen, ob z. B. die Beschriftung und die Maße korrekt dargestellt werden.
> Wenn Korrekturen im Skizzendruck notwendig sind, können Sie die Skizzen über den S+N-Editor bearbeiten.

**Druckmodus**
Die Auswahl aus dieser Kombobox steht auch über das Menü Druckmodi zur Verfügung.
Der Druckmodus bestimmt, welche Art von Formular gedruckt wird. Die Auswahl gilt jeweils für alle Dokumente, die in der Übersicht aufgelistet sind. Über den Druckmodus werden die zugeordneten Formulare im gleichnamigen Feld zur Auswahl angeboten.

- **Auftrag:** Mit dieser Auswahl werden Auftragsbestätigungen gedruckt.
- **Fertigungsschein:** Mit dieser Auswahl werden Fertigungsscheine gedruckt.
- **Lieferschein:** Mit dieser Auswahl werden Lieferscheine und Teillieferscheine gedruckt.
- **Rechnung:** Mit dieser Auswahl werden Anzahlungsrechnungen, Rechnungen und Teilrechnungen gedruckt.
- **Sonstige:** Mit dieser Auswahl können spezielle Ausgaben erzeugt werden, z. B. Rechnungen für ein Daten-Management-System (DMS).

**Formularsprache**
In diesem Feld wird die Sprache angezeigt, in der die Dokumente gedruckt werden. Die Anzeige ist nur vorhanden, wenn mit Mehrsprachigkeit gearbeitet wird.

**Sonderdruck**
Über diese Checkboxen legen Sie die Kriterien fest, nach denen Dokumente aus dem Nummernverwalter gefiltert werden. Dokumente, auf die die Kriterien nicht zutreffen, werden nicht gedruckt.
Zusätzlich geben Sie damit an, wie die Dokumente gesendet werden sollen.

**Wiederholungsdruck** In der Regel kann ein Dokument nur einmal gedruckt werden. Sie können jedoch beliebig viele Wiederholungsdrucke starten. Ob Sie einen Wiederholungsdruck starten müssen oder nicht, können Sie am Status des Dokuments erkennen, der in der Übersicht in der gleichnamigen Spalte angezeigt wird.
- Das Dokument wird zum ersten Mal gedruckt. Bei Lieferscheinen, Fertigungsscheinen und Rechnungen wird automatisch eine Dokumentennummer erzeugt, z. B. die Rechnungsnummer.
- [x] Das Dokument wird als Wiederholungsdruck ausgegeben und erhält keine neue Nummer.

**Dokumentenarchivierung** Die Dokumente können an ein externes Archiv übergeben werden.
- Die gedruckten Dokumente werden nicht extern archiviert.
- [x] Die Dokumente werden an das externe Archiv übergeben.

**Sammelausdruck** Als Sammeldruck können alle Dokumente für einen Kunden ausgegeben werden, die im Nummernverwalter aufgelistet sind. Dazu muss in den Stammdaten und/oder im Dokument das Kennzeichen für den Sammeldruck aktiviert sein.
- Die Dokumente der angezeigten Liste werden einzeln gedruckt.
- [x] Die Dokumente im gewählten Nummernverwalter werden als Sammeldruck ausgegeben. Die Kombobox wird freigeschaltet. Zum Filtern der Dokumente stehen folgende Kriterien zur Wahl:
  - **Immer:** Diese Einstellung überschreibt die Einstellung zum Sammeldruck aus den Stammdaten.
  - **Pro Bestelltext 1:** Alle Dokumente für einen Kunden werden nach dem Bestelltext 1 gefiltert und zusammengefasst. Wenn z. B. für einen Kunden 10 Aufträge vorhanden sind, von denen fünf den gleichen Bestelltext 1 haben, werden sechs Auftragsbestätigungen gedruckt.
  - **Pro Lieferadresse:** Alle Dokumente mit derselben Lieferanschrift werden zusammengefasst.
  - **Standard:** Alle Dokumente mit demselben Kunden/Lieferanten werden zusammengefasst, wenn das Kennzeichen für den Sammeldruck gesetzt ist.
    - ⇨ Tutorial, "Sammelrechnungsdruck" auf Seite C-33
    - ⇨ "Teillieferung, Teilfaktura, Sammelrechnung" auf Seite C-434

> **Rechnungen für den Sammeldruck sortieren**
> Die Sammelrechnungen werden beim Druck nicht nach Kriterien sortiert. Sie müssen die Rechnungen vor dem Druck im Nummernverwalter so sortieren, dass der Sammelrechnungsdruck sinnvoll ausgeführt wird.
>
> ⇨ "Sortierung" auf Seite C-647

**Einschränkung** Mit der Wahl der Option legen Sie fest, ob bestimmte Dokumente vor dem Druck herausgefiltert werden:
- **Alle Dokumente:** Der Betrag der Dokumente wird nicht geprüft.
- **Betrag ungleich 0:** Alle Dokumente mit einem positiven oder negativen Betrag werden gedruckt, z. B. Rechnungen mit einem negativen Betrag, die als Gutschriften gewertet werden.
- **Betrag größer 0:** Alle Dokumente mit einem Betrag über null werden gedruckt.
- **Alle Dokumente mit Positionen:** Alle Dokumente mit Positionen werden gedruckt, der Ausdruck von Dokumenten ohne Positionen wird unterdrückt.

**Faxversand** Die Dokumente können direkt als Fax versendet werden. Dazu muss in den Stammdaten das Kennzeichen für den Versand per Fax aktiviert sein. Diese Einstellung kann im einzelnen Dokument geändert werden.
- Die Dokumente sollen nicht automatisch per Fax versendet werden.
- [x] Die Dokumente werden automatisch als Fax versendet, sofern eine Faxnummer hinterlegt ist. Dokumenten ohne Faxnummer werden nicht gedruckt und nicht gesendet.
  - ⇨ Stammdaten, "Verbindungen" auf Seite B-773

> **Faxnummer muss angegeben sein**
> Für den Versand als Fax muss für den Adressaten eine Faxnummer hinterlegt sein. Bedenken Sie, dass beim Faxversand die Skizzen ggf. nicht korrekt gedruckt werden können.

**Faxversand an Vertreter** Die Dokumente können automatisch an den zuständigen Vertreter gesendet werden. Dazu muss der Vertreter im Dokumentenkopf angegeben sein. Wenn für den Vertreter keine Faxnummer hinterlegt ist, wird das Dokument nicht gedruckt und gesendet.
- Die Dokumente werden nicht an den Vertreter gesendet.
- [x] Die Dokumente werden an den angegebenen Vertreter gesendet.
  - ⇨ "Vertreter" auf Seite C-401

> **Faxversand wahlweise an den Kunden oder den Vertreter**
> Sie können für den Versand der Dokumente nur eine der beiden Checkboxen markieren. Wollen Sie die Dokumente sowohl an den Kunden als auch an den Vertreter senden, so müssen Sie den Druck mit der geänderten Einstellung ein zweites Mal starten.

**Mail** Die Dokumente können als PDF-Datei per E-Mail an den Kunden oder den zuständigen Vertreter gesendet werden. Dazu muss in den Stammdaten das Kennzeichen für den Versand per E-Mail aktiviert sein. Diese Einstellung kann im einzelnen Dokument geändert werden.
- Die Dokumente sollen nicht automatisch per E-Mail gesendet werden.
- [x] Alle Dokumente werden automatisch als E-Mail gesendet, sofern eine E-Mail-Adresse hinterlegt ist. Die Checkbox Interaktion und die Optionen an Kunde und an Vertreter werden freigeschaltet. Dokumenten ohne E-Mail-Adresse werden nicht gedruckt und nicht gesendet.
  - **an Kunde:** Die Dokumente werden per E-Mail an den Kunden gesendet.
  - **an Vertreter:** Die Dokumente werden per E-Mail an den Vertreter gesendet.
    - ⇨ Stammdaten, "Dokumentenversand" auf Seite B-776
    - ⇨ “Fax, Mail" auf Seite C-426

> **E-Mail-Adresse muss angegeben sein**
> Für den Versand als E-Mail muss für den Adressaten eine E-Mail-Adresse hinterlegt sein. Bedenken Sie, dass beim E-Mail-Versand die Skizzen ggf. nicht korrekt gedruckt werden können.
>
> Sie können für den Versand der Dokumente nur eine der beiden Optionen markieren. Wollen Sie die Dokumente sowohl an den Kunden als auch an den Vertreter senden, so müssen Sie die Checkbox Interaktion markieren und die zweite E-Mail-Adresse manuell eingeben.

**Interaktion** Dokumente können direkt als E-Mail versendet werden oder Sie können eine Anmerkung dazu schreiben.
- Die Dokumente werden direkt per E-Mail an den Kunden oder den Vertreter gesendet.
- [x] Vor dem Versand wird der Browser-Dialog geöffnet und Sie können zusätzliche Anmerkungen oder eine zweite E-Mail-Adresse hinzufügen. Danach müssen Sie den Versand manuell starten.

**Nur Postversand** Die Informationen für den Dokumentenversand werden aus den Stammdaten des Kunden/Lieferanten übernommen und können im Dokumentenkopf geändert werden.
- Alle Dokumente werden gedruckt.
- [x] Aus dem Nummernverwalter werden alle Dokumente herausgefiltert, bei denen weder das Kennzeichen für den Fax- noch für den Mail-Versand gesetzt ist.
  - ⇨ Stammdaten, “Partnerverwaltung - Auftrag" auf Seite B-775
  - "Fax, Mail" auf Seite C-426

**Dokumente**
In der Übersicht werden alle Dokumente aufgelistet, die sich in dem gewählten Nummernverwalter befinden. Wenn Sie den Druckdialog über die Dokumentenverwaltung geöffnet haben, wird nur das aktuelle Dokument angezeigt.
- ⇨ "Nummernverwalter" auf Seite C-643

#### Formular-/Etikettendruck – Etiketten
> Dokumente > Auftrag > Auftrag auswählen > Menü Start > Gruppe Druck > Allgemeiner Formulardruck > Register Etiketten
>
> Dokumente > Auftrag > Druck Auftrag > Register Etiketten

*Abb. C-341 Formular-/Etikettendruck - Etiketten*

In diesem Register legen Sie die Optionen für den Druck von Etiketten fest.

**Selektion nach, Details, Ausgabe auf, Dokumente**
Diese Felder sind ausführlich zum Register Formulare beschrieben.
- "Formular-/Etikettendruck - Formulare" auf Seite C-656

**Etikettenauswahl**
**Etikett** Etiketten können direkt aus A+W Business heraus gedruckt werden, wenn der Etikettendruck nicht über die Produktion gesteuert wird.
- ⇨ "Produktionsetiketten" auf Seite C-445
- ⇨ "Etikettenparameter" auf Seite C-445

**Status** Der Status der Dokumente wird automatisch auf den Status umgesetzt, der dem gewählten Formular zugeordnet ist.

**Druckmodus**
Mit der Wahl der Option legen Sie fest, wie viele Etiketten gedruckt werden müssen:
- **Pro Einheit:** Für jede Bestelleinheit wird ein Etikett gedruckt. Beispielsweise wird für ein 3-fach ISO ein Etikett gedruckt, bei 5 Einheiten also 5 Etiketten.
- **Pro Position:** Für jede Position wird nur ein Etikett gedruckt, z. B. für 5 ISO-Einheiten nur ein Etikett.
- **Pro Auftrag:** Für den gesamten Auftrag wird nur ein Etikett gedruckt, unabhängig davon, wie viele Positionen und wie viele Stücke der Auftrag umfasst.
- **Nach Dokumenteneinstellung:** Der Druck richtet sich nach den Angaben aus dem Dokument. Mit dieser Einstellung können Sie für gemischte Aufträge genau die Etiketten drucken, die pro Position oder Scheibe erforderlich sind.
  - ⇨ "Etikettenparameter" auf Seite C-445

**Sonderdruck**
**Wiederholungsdruck** Wenn für den Etikettendruck ein Sperrstatus eingerichtet ist, muss der Wiederholungsdruck gesondert gekennzeichnet werden.
- Die Etiketten werden im regulären Druck gedruckt.
- [x] Der Druck für die Etiketten soll wiederholt werden.

**Nicht optimierte Gläser** Von Hand zugeschnittene Gläser sind nicht durch die Optimierung gelaufen und müssen gekennzeichnet werden, z. B. bei Modellen.
- Der Zuschnitt wurde über XOpt gesteuert.
- [x] Für diese Position sollen Etiketten ausgedruckt werden.

#### Formular-/Etikettendruck – Dokumentenexport
> Dokumente > Auftrag > Auftrag auswählen > Menü Start > Gruppe Druck > Allgemeiner Formulardruck > Register Dokumentenexport
>
> Dokumente > Auftrag > Druck Auftrag > Register Dokumentenexport

*Abb. C-342 Formular-/Etikettendruck – Dokumentenexport*

In diesem Register können Sie den Export von Dokumenten prüfen.

**Dokumentenexport-Pool**
In der Übersicht werden alle Dokumente aufgelistet, die übergeben werden sollen.

**[Löschen]** Die Schaltfläche ist nur freigeschaltet, wenn ein Fehler bei der Übertragung festgestellt wurde. Mit dieser Schaltfläche löschen Sie einen Eintrag aus dem Übertragungspool.

**[Aktivieren]** Die Schaltfläche ist nur freigeschaltet, wenn ein Fehler bei der Übertragung festgestellt wurde.
Wenn ein Fehler festgestellt wurde, können Sie die Daten korrigieren und erneut zur Übertragung übergeben. Sie lösen die Übertragung mit [Aktivieren] aus.

**[Abfragen]** Mit dieser Schaltfläche aktualisieren Sie die Anzeige, um den Übertragungsstatus zu prüfen.

### Vermaßte Skizze drucken
> Dokumente > Auftrag > Auftrag auswählen > Menü Start > Gruppe Druck > Vermaßte Skizze drucken
>
> Dokumente > Auftrag > NV Auftrag > Menü Druck > Gruppe NV Druck > Vermaßte Skizze drucken

*Abb. C-343 Vermaßte Skizze drucken*

In diesem Dialog können Sie eine maßstäbliche Skizze im Format DIN A4 drucken.

- Tutorial, "Druck von Skizzen" auf Seite C-202

> **Voraussetzung**
> Um vermaßte Skizzen zu drucken, muss die Funktion in den Firmendaten aktiviert sein.
>
> ⇨ Stammdaten, "Firmendaten - Druck" auf Seite B-996

**Nummernverwalter** Auswahl des Nummernverwalters. In der Übersicht im Bereich Dokumente werden nur die Positionen angezeigt, in denen der Skizzendruck von Modellen oder Sprossen auf maßstäblich gesetzt ist.
Wenn Sie den Druck für ein einzelnes Dokument starten, ist diese Anzeige ohne Bedeutung.

#### Formularauswahl
**Formular** Zur Auswahl werden die Formulare angeboten, die für den Skizzendruck zur Verfügung stehen.
Das Formular wird automatisch geändert, wenn Sie eine der Checkboxen im Bereich Sonderdruck markieren.

#### Ausgabe auf
Mit der Wahl der Option legen Sie fest, wie die Dokumente ausgegeben werden.

- **Drucker:** Die Dokumente werden direkt an den Drucker übergeben und gedruckt. Wenn keine anderen Einstellungen im Bereich Sonderdruck aktiviert sind, werden Dokumente auf Papier gedruckt.
  Diese Einstellung sollten Sie dann wählen, wenn Sie Dokumente für den Post- oder Faxversand fertig machen möchten.
  Wenn Sie im Bereich Sonderdruck eine oder mehrere Checkboxen aktivieren, werden aus dem Nummernverwalter die entsprechenden Dokumente ausgefiltert.
- **Bildschirm:** Ein einzelnes Dokument wird auf dem Bildschirm angezeigt und kann geprüft werden.

> **Vor dem Druck Bildschirmausgabe erzeugen**
> Sie sollten sich das Dokument zunächst auf dem Bildschirm anzeigen lassen. Sie können dann prüfen, ob z. B. die Beschriftung und die Maße korrekt dargestellt werden.
> Wenn Korrekturen im Skizzendruck notwendig sind, können Sie die Skizzen über den S+N-Editor bearbeiten.

#### Druckmodus
Mit der Wahl der Option legen Sie fest, wie der Druck gesendet wird:
- **Ausdruck:** Der Druck wird an einen Drucker gesendet.
- **Fax:** Der Druck wird an ein Faxgerät gesendet.
- **Mail:** Der Druck wird als PDF-Datei ausgegeben und kann per E-Mail gesendet werden. Für diese Einstellung muss im Auftrag der Versand der Auftragsbestätigung als Mail aktiviert sein.
  - ⇨ "Fax, Mail" auf Seite C-426

#### Optionen
**Um Rechteckscheiben mit Bearbeitungen erweitern** In der Regel werden Rechteckscheiben nur angezeigt, wenn in ihnen Sprossen enthalten sind.
- Rechteckscheiben werden nicht angezeigt, wenn in ihnen keine Sprossen enthalten sind.
- [x] Rechteckscheiben mit Bearbeitungen werden auch angezeigt.

**Auswahl auf EFG, ESG und VSG beschränken** Die Anzeige der Positionen kann auf Einfachglas, ESG und VSG eingeschränkt werden.
- Die Anzeige der Positionen wird nicht weiter eingeschränkt.
- [x] Die Anzeige der Positionen wird auf EFG, ESG und VSG eingeschränkt.

**Um Ganzglastüranlagen erweitern** Positionen mit Ganzglastüren werden in der Regel nicht angezeigt.
- Ganzglastüren werden nicht angezeigt.
- [x] Positionen mit Ganzglastüren werden angezeigt.

**Sprossenzuschnittsliste ausgeben** Details zu den Sprossen können zusätzlich gedruckt werden.
- Nur die Sprossenskizze wird gedruckt.
- [x] Längen und Zuschnittsinfos der einzelnen Sprossenstäbe werden in eine Detailliste gedruckt. Damit können die Sprossen anhand des Ausdrucks gefertigt werden.

**Template Variablennamen nicht anzeigen** Variablennamen aus einem SN-Template können ausgeblendet werden.
- Variablennamen werden angezeigt, z. B. Scheibenbreite.
- [x] Variablennamen werden nicht angezeigt.

#### Sonderdruck
**Erweitert** Hierbei können Sie die Funktion Erweiterte Modellskizze auswählen, um maßstäbliche Skizzen von Modellen und Sprossen auf ein separates Blatt zu drucken.

**Produktskizze** Produktbild aus den Produktstammdaten. Es kann nur gedruckt werden, wenn in der Produktverwaltung die Checkbox Druck auf Formular aktiviert ist.

Das Produktbild gibt das Produkt selbst wieder. Es zeigt weder das Modell noch die eingebauten Sprossen. Es ist daher nur für seltene Strukturgläser sinnvoll.
- ⇨ Stammdaten, "Artikelskizze" auf Seite B-605

#### Dokumente
In diesem Bereich werden alle Dokumente des Nummernverwalters aufgelistet, in denen Positionen mit Sprossen oder Modellen erfasst sind.

Mit diesen Schaltflächen können Sie alle Positionen markieren oder alle Markierungen entfernen.

Über die Schaltflächen können Sie die Positionen markieren, in denen Sprossen oder Modelle enthalten sind.

### Touren/Fahrer Zuordnung
> Dokumente > Auftrag > Druck Auftrag > Menü Funktionen > Gruppe Allgemein > Touren/Fahrer Zuordnung

*Abb. C-344 Touren/Fahrer Zuordnung*

In diesem Dialog können Sie sich die Touren zu Lieferscheinen anzeigen lassen, die zum Datum des markierten Auftrags gefahren werden.

Die Funktion ist nur freigeschaltet, wenn der Druckmodus Lieferschein eingestellt ist.

Sie können den Touren jeweils einen Fahrer zuordnen, so dass der Name des Fahrers auf den Lieferscheinen gedruckt wird.

## Übergabe Bestellungen
> Dokumente > Auftrag > Bestellübergabe

Bestellungen aus den Aufträgen können direkt an die Lieferanten übergeben werden.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Bestellübergabe" auf Seite C-669
- "Lieferant und Liefertermin ändern" auf Seite C-678
- "Markierungsoptionen" auf Seite C-679
- "Preisvergleich" auf Seite C-680
- "Erweiterte Einstellungen" auf Seite C-681
- "Stücklistenübersicht" auf Seite C-685

### Bestellübergabe
> Dokumente > Auftrag > Bestellübergabe

Mit der Bestellübergabe werden die Produkte aus den Aufträgen herausgefiltert, die bestellt werden müssen.

- ⇨ Tutorial, "Bestellübergabe" auf Seite C-303

> **Voraussetzung**
> Nur wenn die Lieferantenkartei korrekt geführt ist, können Bestellungen zu Aufträgen direkt erzeugt werden.
>
> Stammdaten, "Lieferantenkartei" auf Seite B-866

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite C-669
- "Menü Optionen" auf Seite C-670
- "Bestellübergabe - Bestellnummern" auf Seite C-673
- "Bestellübergabe - Bestellpool" auf Seite C-675

### Menü Funktionen
> Dokumente > Auftrag > Bestellübergabe > Menü Funktionen

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Bestellübergabe zu schließen. Folgende Einträge werden angezeigt:
- **Lieferant/Liefertermine ändern:** Öffnet den Dialog Lieferant und Liefertermin ändern.
  - "Lieferant und Liefertermin ändern" auf Seite C-678
- **Markierungsoptionen:** Öffnet den Dialog Markierungsoptionen.
  - ⇨ "Markierungsoptionen" auf Seite C-679
- **Lieferantenpreise:** Öffnet den Dialog Preisvergleich.
  - ⇨ "Preisvergleich" auf Seite C-680

### Menü Optionen
> Dokumente > Auftrag > Bestellübergabe > Menü Optionen

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

> **Aktivierte Optionen nach dem Öffnen des Dialogs**
> Bitte beachten Sie, dass geänderte Optionen erst beim nächsten Öffnen des Dialogs wirksam werden.
> Wenn durch eine aktivierte Option eine Prüfung gestartet wurde, kann sich das Öffnen eines Dokuments verzögern. Der Grad der Verzögerung hängt von der Leistungsfähigkeit des Rechners ab.
> Die folgenden Beschreibungen stellen die aktivierte Option dar.

Das Menü ist in folgende Gruppen gegliedert:
- Gruppe Übergabe
- Gruppe Liefertermin
- Gruppe Produktbezeichnung
- Gruppe Sonstige
- Gruppe Erweitert

#### Gruppe Übergabe
- **Auftragsbezogene Übergabe:** Die Bestellungen werden pro Auftrag übergeben. Wenn diese Option nicht aktiviert ist, können Sammelbestellungen erzeugt werden.
- **Bestellnummer = Auftragsnummer:** Diese Option ist nur freigeschaltet, wenn die Option Auftragsbezogene Übergabe aktiviert ist.
- **Bestellpool pro Mitarbeiter:** Pro Mitarbeiter kann ein eigener Bestellpool angelegt werden.

#### Gruppe Liefertermin
- **Lieferterminprüfung:** Der Liefertermin wird automatisch geprüft. Ändern Sie einen Liefertermin, der nicht an einem Tourentag liegt, wird eine entsprechende Meldung angezeigt.
- **Lieferantentour berücksichtigen:** Wenn die Bestellung auf einen Liefertermin fällt, der nicht an einem Tourentag liegt, wird eine entsprechende Meldung angezeigt. Dazu müssen die Lieferantentouren in den Stammdaten hinterlegt werden.
  - ⇨ Stammdaten, "Touren" auf Seite B-873
- **Lieferantentour ignorieren bei Direktanlieferung:** Wenn die Bestellung direkt zum Kunden geliefert wird, können Lieferantentouren ignoriert werden.
- **Vorlauftage mit Kombiwarengruppen ermitteln:** Wenn in den Kombiwarengruppen Vorlauftage hinterlegt sind, sollen diese zur Berechnung des Liefertermins herangezogen werden.
  - ⇨ Stammdaten, "Vorlauftage" auf Seite B-576

#### Gruppe Produktbezeichnung
- **Produktbezeichnung aus Lieferantenkartei:** Die Bezeichnung der bestellten Produkte wird aus der Lieferantenkartei übernommen.
- **Produktbezeichnung aus Basisdaten (interne Best.):** Für interne Bestellungen wird die Bezeichnung der bestellten Produkte aus den Produktstammdaten übernommen.

#### Gruppe Sonstige
- **Keine Kostenrückschreibung:** Die Kosten werden nicht in die EK-Preise des Auftrags zurückgeschrieben.
- **Maßzuschläge berücksichtigen:** Bei der Bestellung sollen die Maßzuschläge mit übergeben werden.
- **Rückschnitt vom Abstandhaltermaß abziehen:** Der Rückschnitt von Abstandhaltern wird in der Breite und Höhe der Bestellung abgezogen, jedoch nur, wenn keine Sprossen mitbestellt werden. Im Fall von unterschiedlichen Modellkanten wird der Rückschnitt vom Abstandhaltermaß immer abgezogen.
- **Druckkennzeichen für Bearbeitungen immer setzen:** In der Bestellung sollen Bearbeitungen immer gedruckt werden. Wenn die Option deaktiviert ist, werden die Druckkennzeichen unverändert aus dem Auftrag in die Bestellung übernommen.
- **Statistikwarengruppe aus dem Auftrag:** Die Angabe zur Statistikwarengruppe wird aus dem Auftrag übernommen, wenn für Auftrag und Bestellung unterschiedliche Statistikwarengruppen definiert sind.
- **Geschäftsart aus dem Auftrag:** Die Geschäftsart wird aus dem Auftrag übernommen, wenn für Auftrag und Bestellung unterschiedliche Geschäftsarten definiert sind.
- **AV-Bereich aus dem Auftrag:** Der AV-Bereich wird aus dem Auftrag übernommen, wenn für Auftrag und Bestellung unterschiedliche AV-Bereiche definiert sind.
- **Fachberater = Erfasser bei Neuanlage:** In der Bestellung wird automatisch der Name des Mitarbeiters eingetragen, der sich in A+W Business angemeldet hat.
- **Statusänderung erfragen:** Die Abfrage zur Änderung des Status wird angezeigt.
- **Wiederholte Übergabe nur bis Sperrstatus:** Bestellungen können mehrfach übergeben werden, allerdings nur, bis der Sperrstatus erreicht ist.
- **Autom. Zuschl.-Kennz. aus Produkten einlesen:** Die Zuschlagskennzeichen immer wieder aus dem Artikelstamm einlesen.

#### Gruppe Erweitert
- **Einstellungen:** Öffnet den Dialog Erweiterte Einstellungen, um Angaben zum Druck von Texten und Dateianhängen festzulegen.
  - ⇨ "Erweiterte Einstellungen" auf Seite C-681

### Bestellübergabe – Bestellnummern
> Dokumente > Auftrag > Bestellübergabe > Register Bestellnummern

*Abb. C-345 Bestellübergabe – Bestellnummern*

In diesem Register wählen Sie den Übergabe-Modus aus. Die sofort an den Einkauf übergebenen Bestellungen können Sie sich im Dialog Bestellungen anzeigen lassen.

- ⇨ Tutorial, "Bestellübergabe" auf Seite C-303

#### Modus
Mit der Wahl der Option legen Sie die Form der Übergabe von Bestellpositionen fest:
- **Pool füllen:** Mit dieser Option werden die Auftragspositionen mit Bestellteilen im Register Bestellpool angezeigt und können vor der Übergabe geprüft werden.
- **Sofort bestellen:** Mit dieser Option werden die Daten sofort an den Standard-Lieferanten übergeben. Diese Option ist dann sinnvoll, wenn Sie zuvor keine Preise oder Liefertermine prüfen möchten und die Lieferantenkartei entsprechend gepflegt ist.
- **Sofort anfragen:** Die Bestellungen werden zur Anfrage an die Standard-Lieferanten übergeben.

#### Selektion nach Nummernverwalter
**Name** Auswahl des Nummernverwalters, in dem die Aufträge zusammengefasst sind, die übergeben werden sollen.

#### Dokumente
- **Auftragsnummer:** Auftragsnummer aus dem Auftragskopf
- **Bestellnummer(n):** Wenn Aufträge bereits übergeben wurden, werden die Bestellnummern angezeigt.
- **Kundennummer, Kunde:** Kundennummer und Kundenname aus dem Auftragskopf bzw. den Stammdaten.
- **Status:** Aktueller Status des Auftrags. Bei neuen Aufträgen ist das in der Regel der Mindest-Status, z. B. Dokument gedruckt.
- **Datum Erfassung:** Datum, an dem der Auftrag erstellt wurde.
- **Datum Auslieferung:** Datum, an dem der Auftrag ausgeliefert wird.
- **Datum AB:** Datum, an dem die Auftragsbestätigung gedruckt wurde.
- **Sperr-KZ:** Ggf. Sperr-Kennzeichen des Auftrags.

#### Ziel-Nummernverwalter
**Mitarbeiter** Name des Mitarbeiters, in dessen Nummernverwalter die erzeugten Bestellungen gestellt werden sollen.

**Name** Nummernverwalters, in den die Bestellungen gestellt werden sollen. Wenn Sie einen neuen Namen eintragen, wird ein neuer Nummernverwalter angelegt.
- ⇨ Tutorial, "Nummernverwalter" auf Seite C-186
- ⇨ "Nummernverwalter" auf Seite C-643

#### Ziel-Nummernkreis
**Mandant** Mandant, aus dessen AV-Bereich die Bestellnummern genommen werden sollen. Die Wahl des Mandanten steuert die Anzeige im Feld AV-Bereich.

**AV-Bereich** Standard-AV-Bereich, der in den Stammdaten des Produkts hinterlegt ist. Sie können einen anderen AV-Bereich auswählen. Wenn die Auswahl der AV-Bereiche nicht eingeschränkt werden soll, müssen Sie den Eintrag <k.A.> wählen.

### Bestellübergabe – Bestellpool
> Dokumente > Auftrag > Bestellübergabe > Register Bestellpool

*Abb. C-346 Bestellübergabe – Bestellpool*

In diesem Register können Sie die Positionen prüfen und ggf. die Daten ergänzen, bevor Sie die Bestellung übergeben. Wenn Sie den Bestellpool nicht über das Register Bestellnummern gefüllt haben, können Sie Aufträge mit Bestellpositionen über die Schaltflächen nach Lieferant, Produkt und/oder Liefertermin zusammenstellen.

Die übergebenen Bestellungen können Sie sich im Dialog Bestellungen anzeigen lassen.
- ⇨ "Bestellung im Bestellpool ändern" auf Seite C-313

**Lieferant** Im Auswahlmodus können Sie Bestellpositionen für einen bestimmten Lieferanten zusammenstellen.
- ⇨ "Markierungsoptionen" auf Seite C-679

**Produkt** Im Auswahlmodus können Sie Bestellpositionen für ein bestimmtes Produkt zusammenstellen.

**Liefertermin** Im Auswahlmodus können Sie Bestellpositionen für einen bestimmten Liefertermin zusammenstellen.

**Auftrag** Im Auswahlmodus können Sie Bestellpositionen für eine Abfolge von Auftragsnummern zusammenstellen.

#### Bestellpool
Mit diesen Schaltflächen können Sie alle Positionen automatisch markieren, die an einen bestimmten Lieferanten gesendet werden sollen, oder alle Markierungen entfernen.

Über das Menü Funktionen können Sie Filter einstellen, anhand derer die Positionen automatisch markiert werden.
- ⇨ "Markierungsoptionen" auf Seite C-679

> **Positionen markieren**
> Nur die markierten Positionen werden übergeben. Bei langen Listen können Sie die Positionen insgesamt aus- oder abwählen, indem Sie auf die entsprechenden Schaltflächen klicken.

**Übergabe an:** Bestellungen können wahlweise direkt an die Lieferanten übergeben oder als Bestellanfrage gesendet werden.
- **Bestellung:** Mit dieser Option werden Bestellungen erzeugt. Bestellungen an denselben Lieferanten können zu Sammelbestellungen zusammengefasst werden. Dazu muss die Option Auftragsbezogene Übergabe deaktiviert sein und die Bestellpositionen müssen in der richtigen Reihenfolge aufgeführt sein.
- **Bestellanfrage:** Mit dieser Option werden Bestellanfragen erzeugt, um z. B. Liefertermine oder Preise zu erfragen.

#### Übersicht
In der Übersicht werden die Daten zu den Bestellpositionen angezeigt. Diese können bearbeitet werden. Zur Wahl eines alternativen Lieferanten können Sie sich einen Preisvergleich anzeigen lassen.

- **Auftrag, Pos.:** Nummer des Auftrags und der Position, zu der die Bestellung erzeugt werden soll.
- **Int. Kunde:** Name des internen Kunden. Die Spalte wird nur angezeigt, wenn im Bestellpool Dokumente für interne Aufträge vorhanden sind.
  - ⇨ Tutorial, "Interne Aufträge" auf Seite C-307
- **Lieferant:** Der Lieferant wird aus der Lieferantenkartei oder dem Auftrag übernommen. Wenn kein Lieferant eingetragen ist oder wenn Ihnen Lieferschwierigkeiten Ihres Standard-Lieferanten bekannt sind, können Sie den Namen ändern.
  - "Lieferant und Liefertermin ändern" auf Seite C-678
- **Artikel, Farbe:** Nummer und ggf. Variante des Produkts, das bestellt werden soll.
- **Menge:** Menge, die bestellt werden soll.
- **Breite, Höhe:** Maße der Scheibe, die bestellt werden soll.
- **Anlief.-Term. bei Kunde:** Der Liefertermin wird aus dem Auftrag übernommen. Lieferschwierigkeiten werden farblich gekennzeichnet und Sie können den Termin dann ändern.
- **Anlief.-Term. d. Lieferant:** Der Liefertermin des Lieferanten wird aus den Angaben in der Lieferantenkartei errechnet. Lieferschwierigkeiten werden farblich gekennzeichnet und Sie können den Termin dann ändern.
- **Übergeben an:** Die Bestell- oder Anfragenummern werden nach der Übergabe angezeigt.
- **Stkl.-Anz.:** Mit einem Klick in die entsprechende Zelle können Sie sich die Stückliste anzeigen lassen. In der Spalte sind die Zeilen mit Produkten gekennzeichnet, die komplett mit allen Stücklistenelementen bestellt werden.
- **Kritischer Lagerbestand erreicht am:** Damit, an dem die Menge erreicht wird, ab der Lagerbestand keine termingerechte Produktion mehr sicherstellen kann. Die entsprechend Lagerbestellung muss manuell angestoßen werden.

**Position für** Die aufgelisteten Positionen sind farblich gekennzeichnet.

#### Ziel-Nummernverwalter, Nummernkreise
Diese Felder sind zum Register Bestellnummer beschrieben.
- ⇨ "Bestellübergabe - Bestellnummern" auf Seite C-673

### Lieferant und Liefertermin ändern
> Dokumente > Auftrag > Bestellübergabe > Register Bestellpool > Doppelklick auf Position

*Abb. C-347 Lieferant und Liefertermin ändern*

In diesem Dialog können Sie den Lieferanten und die Liefertermine für die Bestellungen zu einem bestimmten Auftrag ändern.

Die Checkboxen werden automatisch markiert, wenn Sie im zugehörigen Feld eine Änderung eingetragen haben.

**Lieferant / Matchcode** Nummer des aktuellen Lieferanten. Über die Lieferantennummer oder den Matchcode können Sie einen anderen Lieferanten angeben.

**Anliefertermin bei Kunde** Aktueller Liefertermin beim Kunden. Zum Ändern können Sie das Datum überschreiben oder aus dem Kalender auswählen.

**Anliefertermin durch Lieferant** Aktueller Liefertermin für den Lieferanten. Zum Ändern können Sie das Datum überschreiben oder aus dem Kalender auswählen. Wenn Sie den Termin über den Kalender auswählen, werden die Tourentage hervorgehoben.

**Statt internem Auftrag reguläre Bestellung erzeugen.** Sie können interne Aufträge in Bestellungen an einen Lieferanten umwandeln, ohne den Lieferanten auswählen zu müssen.
- Interne Bestellungen bleiben erhalten, sofern Sie keinen externen Lieferanten ausgewählt haben.
- [x] Die interne Bestellung wird automatisch in eine reguläre Bestellung umgewandelt. Als Lieferant wird automatisch der Standard-Lieferant für den Artikel eingesetzt.

### Markierungsoptionen
> Dokumente > Auftrag > Bestellübergabe > Register Bestellpool > Menü Funktionen > Markierungsoptionen

*Abb. C-348 Markierungsoptionen*

In diesem Dialog stellen Sie Kriterien ein, nach denen die Bestellungen gefiltert und markiert werden, um sie dann zu bestellen. Die Felder werden freigeschaltet, wenn die zugehörige Checkbox markiert ist.

#### Markierungsoptionen
**Auftragsnummer von, bis** Alle Positionen werden markiert, deren Auftragsnummern im angegebenen Bereich liegen.

**Lieferant** Alle Positionen werden markiert, die bei einem bestimmten Lieferanten bestellt werden.

**Liefertermin** Alle Positionen werden markiert, die zum angegebenen Termin geliefert werden sollen.

**Produkt** Alle Positionen werden markiert, die das angegebene Produkt betreffen.

**Produktionstermin** Alle Positionen werden markiert, die zu einem bestimmten Termin produziert werden sollen.

**Warengruppe** Alle Positionen werden markiert, die die angegebene Warengruppe betreffen.

**Int. Kunde** Alle internen Bestellungen für einen internen Kunden werden markiert.

### Preisvergleich
> Dokumente > Auftrag > Bestellübergabe > Register Bestellpool > Menü Funktionen > Lieferantenpreise

*Abb. C-349 Lieferanten - Preisvergleich*

In diesem Dialog lassen Sie sich anzeigen, welche Lieferanten die Produkte zu welchen Preisen und Terminen liefern können.

Die Checkbox des Standard-Lieferanten ist automatisch markiert.

Wenn Sie einen anderen Lieferanten auswählen, werden die entsprechenden Angaben im Dialog Bestellübergabe im Register Bestellpool aktualisiert.

- ⇨ "Bestellübergabe - Bestellpool" auf Seite C-675

> **Die Zeile muss mit einem X markiert sein**
> Sie können den Preisvergleich nur starten, wenn Sie im Register Bestellpool die entsprechende Zeile markiert haben und ein X im Zeilenkopf angezeigt ist. Die einfache Markierung einer Zeile reicht nicht aus.

#### Lieferanten - Positionspreise
In der Übersicht werden die ausgewählten Aufträge angezeigt. Die aufgelisteten Positionen sind farblich gekennzeichnet:
- **Default-Lieferant:** In roter Schrift ist der Standard-Lieferant dargestellt.
- **!!! -> rechtzeit. Liefertermin gefaehrdet:** Mit drei Ausrufungszeichen sind die Einträge dargestellt, bei denen der Liefertermin gefährdet ist.
- **preisguenstigster Lieferant:** In grüner Schrift sind die Einträge des preisgünstigsten Lieferanten dargestellt.
- **Default- und preisguenstigster Lieferant:** In blauer Schrift sind die Einträge des Standard-Lieferanten dargestellt, die gleichzeitig die preisgünstigsten sind.

### Erweiterte Einstellungen
> Dokumente > Auftrag > Bestellübergabe > Menü Optionen > Gruppe Erweitert > Einstellungen

In diesem Dialog legen Sie Einstellungen für die Bestellübergabe fest.

In diesem Dialog finden Sie folgende Register:
- "Erweiterte Einstellungen – Allgemein" auf Seite C-682
- "Erweiterte Einstellungen – Sortierung" auf Seite C-683

#### Erweiterte Einstellungen – Allgemein
> Dokumente > Auftrag > Bestellübergabe > Menü Optionen > Gruppe Erweitert > Einstellungen > Register Allgemein

*Abb. C-350 Erweiterte Einstellungen - Allgemein*

In diesem Register können Sie bestimmen, welche Texte nicht in die Bestellung übernommen werden sollen.

**Textfilter**
**1.-6.** Textkennzeichen der Texte, die nicht in die Bestellung übernommen werden sollen, z. B. L für Lieferscheintexte.
- ⇨ Stammdaten, "Textkennzeichen" auf Seite B-1058

**Kommissionstext ersetzen**
**Die Kommission nicht aus dem Auftrag übernehmen** Sie können festlegen, ob die Kommissionstexte in die Bestellung übernommen werden sollen.
- Kommissionstexte aus dem Auftragskopf werden in die Bestellung übernommen.
- [x] Kommissionstexte aus dem Auftragskopf werden nicht in die Bestellung übernommen. Das Feld für die Formel ist freigeschaltet, um einen anderen Text einzutragen.

**Text für interne Bestellung**
**Nr.** Für interne Bestellungen können Sie eigene Texte hinterlegen. Mit der Textnummer bestimmen Sie, welcher Text übergeben werden soll.
- Tutorial, "Text erfassen" auf Seite C-54

**SZR Bestellung**
Wenn ein SZR aus einer Auftragsposition bestellt wird, wird die gewählte Produktgruppe mitbestellt, z. B. Sprossen.

**In die Bestellung übertragbare Dateianhänge**
In der Übersicht werden alle Typen von Dateianhängen aufgelistet. Nur die Dateianhänge werden mit der Bestellung übertragen, die zum markierten Typ gehören.

#### Erweiterte Einstellungen – Sortierung
> Dokumente > Auftrag > Bestellübergabe > Menü Optionen > Gruppe Erweitert > Einstellungen > Register Sortierung

*Abb. C-351 Erweiterte Einstellungen - Sortierung*

In diesem Register legen Sie fest, wie die Angaben im Bestellpool sortiert sein sollen.

**Sortierung nach**
Mit der Wahl der Option legen Sie die Sortierung auf dem Bestellschein fest:
- **Nach Auftrag - Lieferant - Position:** Die Positionen werden pro Auftrag nach Lieferanten aufgelistet.
- **Nach Auftrag - Position - Lieferant:** Die Lieferanten werden pro Auftrag nach Positionen aufgelistet.
- **Bestelloptimiert nach Lieferant:** Die Bestellungen werden nach AB-Nummer und Lieferanten sortiert.
- **Benutzerdefiniert:** Die Felder Verfügbare Sortierkriterien und Ausgewählte Kriterien und Reihenfolge werden freigeschaltet, so dass Sie die Kriterien auswählen und sortieren können.

**NV-Sortierung beibehalten** Die Sortierung kann aus dem jeweiligen Nummernverwalter übernommen werden.
- Die Sortierung des Nummernverwalters wird nicht berücksichtigt.
- [x] Die Sortierung richtet sich nach den Einstellungen im Nummernverwalter.

**Verfügbare Sortierkriterien**
In diesem Feld werden die möglichen Sortierkriterien aufgelistet. Das Feld ist nur freigeschaltet, wenn die Option Benutzerdefiniert gewählt wurde.

**Ausgewählte Sortierkriterien und Reihenfolge**
Aus dem Feld Verfügbare Sortierkriterien werden ausgewählte Sortierkriterien in dieses Feld verschoben. Zusätzlich kann die Reihenfolge bearbeitet werden. Das Feld ist nur freigeschaltet, wenn die Option Benutzerdefiniert gewählt wurde.

### Stücklistenübersicht
> Dokumente > Auftrag > Bestellübergabe > Register Bestellpool > Klick auf Spalte Stkl.Anz.

*Abb. C-352 Stücklistenübersicht*

In diesem Dialog lassen Sie sich die Stückliste der Bestellposition anzeigen.

## Auftrag
Über das Menü **Auftrag** erreichen Sie sich folgende Programmpunkte:

- **NV Auftrag:** Die Funktion des Nummernverwalters ist für alle Dokumente gleich. Sie wird am Beispiel Auftrag beschrieben.
  - ⇨ "Nummernverwalter" auf Seite C-643
- **Auftrag:** Die Erfassung von Dokumenten ist für alle Dokumentenarten gleich. Sie wird am Beispiel Auftrag beschrieben.
  - ⇨ "Dokument - Kopfdaten" auf Seite C-424
- **Teillieferung:** Öffnet den Dialog Teillieferung, in dem der Auftragsstatus der Dokumente angezeigt wird.
  - ⇨ "Teillieferungen" auf Seite C-630
- **Druck Auftrag:** Der Formular- und Etikettendruck ist für alle Dokumente gleich. Er wird am Beispiel Auftrag beschrieben.
  - "Druck" auf Seite C-652
- **FiBu-Übergabe:** Die FiBu-Übergabe ist für Aufträge und Gutschriften gleich. Sie wird am Beispiel Auftrag beschrieben.
  - ⇨ "FiBu-Übergabe" auf Seite C-695
- **Import/Export von Zahlungen:** Dieser Dialog steht nur für den brasilianischen Zahlungsverkehr zur Verfügung.
  - ⇨ "Import/Export von Zahlungen" auf Seite C-701
- **Journal:** Der Journaldruck ist für alle Dokumente gleich. Er wird am Beispiel Auftrag beschrieben.
  - "Journal" auf Seite C-742
- **Anzahlungen Aufträge:** Der Anzahlungsdruck ist für Aufträge und Gutschriften gleich. Er wird am Beispiel Auftrag beschrieben.
  - ⇨ "Anzahlungen" auf Seite C-689
- **Bestellübergabe:** Wenn in den Auftragspositionen Bestellungen enthalten sind, können diese direkt bestellt oder in einen Bestellpool übergeben werden.
  - ⇨ "Übergabe Bestellungen" auf Seite C-669
- **Übergabe Archiv:** Die Archivübergabe ist für alle Dokumente gleich. Sie wird am Beispiel Auftrag beschrieben.
  - ⇨ "Übergabe Archiv" auf Seite C-702
- **Suche:** Der Suchdialog ist für alle Dokumente gleich. Er wird am Beispiel Auftrag beschrieben.
  - ⇨ "Dokument suchen" auf Seite C-534
- **Import:** Mit dieser Funktion werden elektronische Kunden-Aufträge importiert.
  - ⇨ "Import" auf Seite C-704
- **Bankbelege:** Die Bankbelege sind für Aufträge und Gutschriften gleich. Sie werden am Beispiel Auftrag beschrieben.
  - ⇨ "Bankbelege" auf Seite C-690
- **Überrechnen:** Öffnet den Dialog Neuberechnung von Dokumenten, um Preisänderungen in den Stammdaten in das ausgewählte Dokument zu übernehmen.
  - ⇨ "Überrechnen" auf Seite C-692
- **Objektabrechnung:** Die folgenden Einträge sind abhängig von dem Modus der Objektverwaltung, der in den Firmendaten eingestellt ist.
  - **Nummernverwalter:** Öffnet den Nummernverwalter für die Objekt-/Abrechnungsverwaltung.
    - ⇨ "Nummernverwalter" auf Seite C-645
  - **Abrechnung:** Öffnet den Dialog Objekte, um objektbezogene Abrechnungen zu erstellen.
    - ⇨ "Abrechnung" auf Seite C-706
  - **Formulare:** Öffnet den Formular-/Etikettendruck für die Objekt-/Abrechnungsverwaltung.
    - ⇨ "Formular-/Etikettendruck" auf Seite C-655
  - **Stunden:** Öffnet den Dialog Einkauf, um eine Stundenforderung zu erfassen.
    - ⇨ "Stundenforderung" auf Seite C-719
  - **Einkauf:** Öffnet den Dialog Einkauf, um eine Einkaufsforderung zu erfassen.
    - ⇨ "Einkaufsforderung" auf Seite C-720
- **TPS Faktura:** Öffnet den Dialog TPS Faktura. Dieser Eintrag ist nur kundenspezifisch freigeschaltet.
- **Schnellanfrage:** Öffnet den Dialog Schnellanfrage, um eine (telefonische) Kundenanfrage aufzunehmen, ohne den aktuellen Auftrag zu schließen.
  - ⇨ "Schnellanfrage" auf Seite C-601
- **Garantiebelege:** Dieser Dialog ist nur kundenspezifisch freigeschaltet.
- **SAFT-PT-Export:** Öffnet den Dialog SAFT-PT Export. Dieser Eintrag ist für den portugiesischen Markt freigeschaltet.
  - ⇨ “SAFT-PT Export" auf Seite C-694
- **Auswertungen:**
  - **Preisänderung:** Öffnet den Dialog Preisänderungsreport, um alle Aufträge anzuzeigen, die von Preisänderungen betroffen sind.
    - ⇨ "Preisänderung (Report)" auf Seite C-724
  - **Null-Preisreport:** Öffnet den Dialog Null-Preisreport, um alle Auftragspositionen ohne Preis anzuzeigen.
    - ⇨ "Null-Preisreport" auf Seite C-726
  - **Deckungsbeitrags-Analyse:** Öffnet den Dialog Deckungsbeitrags-Analyse, um die Deckungsbeiträge von Aufträgen anzuzeigen.
    - ⇨ "Deckungsbeitrags-Analyse" auf Seite C-727
  - **Kalkulatorische Frachtkosten:** Öffnet den Dialog Kalkulatorische Frachtkosten, um Fracht- und Speditionskosten zu erfassen.
    - "Kalkulatorische Frachtkosten" auf Seite C-731
- **Interne Kontrolle**
  - **Gutschriftgründe:** Öffnet den Dialog Gutschriftgründe, um eine Auswertung zu Gutschriftgründen zu erstellen.
    - ⇨ "Gutschriftgründe" auf Seite C-735
  - **Verspätete Lieferung/Lieferung ohne Berechnung:** Öffnet einen Dialog, um eine Auswertung zu verspäteten Lieferungen oder Lieferungen ohne Preise zu erstellen.
    - ⇨ “Verspätete Lieferung/Lieferung ohne Berechnung" auf Seite C-738

### Anzahlungen
> Dokument > Auftrag > Anzahlungen Aufträge

*Abb. C-353 Anzahlungsdruck*

In diesem Dialog lassen Sie sich Listen der erfassten Anzahlungsrechnungen erstellen. Der Dialog ist für Aufträge und Gutschriften gleich.

- ⇨ Tutorial, “Anzahlungen" auf Seite C-280

#### Auswahl
**Nummernverwalter** Auswahl des Nummernverwalters, in dem die Anzahlungen gesammelt wurden.

**Seitenumbruch beim Wechsel von**
Für den Druck kann ein Seitenumbruch festgelegt werden:
- Das Anzahlungsdatum ist ausschlaggebend.
- Die Zahlungsart ist ausschlaggebend.
- Der Seitenumbruch wird nicht beim Anzahlungsdatum / bei der Zahlungsart eingefügt.
- [x] Der Seitenumbruch wird eingefügt.

**Anzahlungsdatum** Bei Druck kann

#### Dokumente
In der Übersicht werden alle Dokumente aus dem gewählten Nummernverwalter angezeigt. Die Liste wird über die Druckfunktion erstellt.

### Bankbelege
> Dokumente > Auftrag, Gutschrift > Bankbelege

*Abb. C-354 Bankbelege - Wechseldruck*

In diesem Dialog können Sie Überweisungsträger für Ihre Kunden drucken.

#### Menü Optionen
- **LGF Modus aktiv:** Diese Funktion ist nur kundenspezifisch freigeschaltet.

#### Menü Funktionen
- **Historie:** Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des Dokuments.
  - ⇨ "Historie" auf Seite C-564

#### Identifikation
**Mandant** Mandant, für den die Überweisung verbucht werden muss.
- ⇨ Stammdaten, "Firmendaten - Mandant" auf Seite B-931

**Bereich** Wenn Sie mit AV-Bereichen als eigene Profit-Center arbeiten, können den AV-Bereich auswählen, zu dem die Überweisung gehört.

**Mitarbeiter** Name des Mitarbeiters, der sich in A+W Business angemeldet hat.

**Nummernverwalter** Auswahl des Nummernverwalters, in dem die Rechnungen gesammelt sind.

**Einzeldruck** Die Überweisungen können gesammelt gedruckt werden.
- Die Überweisungen werden gemeinsam auf einen Datenträger gedruckt. Diese Einstellung ist nur sinnvoll, wenn alle Rechnungen für denselben Kunden gelten.
- [x] Die Überweisungen werden einzeln auf jeweils einen eigenen Datenträger gedruckt.

#### Modifikation
In diesem Bereich werden Details des Dokuments angezeigt.

**Rechnung** Rechnungsnummer des markieren Dokuments.

**Rechnungsdatum, Nettobetrag** Rechnungsdatum und Nettobetrag des markieren Dokuments.

**KZ Fälligkeitsberechnung** Kennzeichen für die Fälligkeit aus dem Auftrag.
- ⇨ Tutorial, "Fälligkeitsberechnung" auf Seite C-215

**Zahltage** Die Zahltage werden im Auftrag angegeben.

**Valuta-Datum** Das Datum der Wertstellung wird aus den Angaben zur Fälligkeit errechnet.

**Bruttotage** Die Bruttotage werden aus den Angaben zur Fälligkeit und den Zahltagen errechnet.

**Betrag Fakturieren** Anzeige Netto-Rechnungsbetrag. Er kann geändert werden. Die Änderungen gelten nur für das markierte Dokument.
Mit der Pfeil-Schaltfläche kann die Änderung zurückgesetzt werden.

#### Übersicht
Aus dem gewählten Nummernverwalter werden nur die Dokumente mit einer Rechnungsnummer angezeigt.

Im Zeilenkopf wird ein rotes X angezeigt, wenn der Sperrstatus des Dokumentes überschritten ist.

### Überrechnen
> Dokumente > Auftrag > Überrechnen

*Abb. C-355 Überrechnen – Neuberechnung von Dokumenten*

In diesem Dialog können Sie die Auftragssummen neu berechnen lassen, z. B. Mehrwertsteuer, Zuschläge, Flächen. Die Kosten der Fußzuschläge werden nur überrechnet, wenn die Überrechnung im Modus EK gestartet wird.

#### Dokumente
Mit der Wahl der Option geben Sie an, welche Dokumente aufgelistet werden sollen. Gleichzeitig wird die Wahl eines Nummernverwalters in der gleichnamigen Kombobox entsprechend eingeschränkt.

#### Optionen
Die Checkboxen in diesem Bereich sind in Abhängigkeit des Modus zur Neuberechnung freigeschaltet bzw. gesperrt.

**Preis auf Null setzen** Die Checkbox ist nur freigeschaltet, wenn der Modus Komplette Berechnung markiert ist.
- Die Preise in den Dokumenten werden nicht auf null gesetzt.
- [x] Die Preise werden auf null gesetzt.
**Mwst %-Satz neu einlesen** Der Mwst-Steuersatz kann nach einer Änderung für alle Dokumente neu eingelesen werden. Die Checkbox ist nur freigeschaltet, wenn der Modus Komplette Berechnung oder Mwstberechnung markiert ist.
- Der Mwst-Satz wird nicht neu eingelesen.
- [x] Der Mwst-Satz wird neu eingelesen. Anschließend wird die Mehrwert-Steuer neu berechnet.

**Manuelle Preisvorgaben löschen** Die Checkbox ist nur freigeschaltet, wenn der Modus Komplette Berechnung markiert ist.
- Die manuellen Preise werden nicht gelöscht.
- [x] Die manuellen Preise werden gelöscht. Zur Neuberechnung werden die Preise aus den Stammdaten herangezogen.

**Warengruppen neu einlesen** Die Checkbox ist nur freigeschaltet, wenn der Modus Komplette Berechnung oder Kombi-WGR bilden markiert ist.
- Die Warengruppen werden nicht neu eingelesen.
- [x] Die Warengruppen werden neu eingelesen.

**Autom. Zuschl.-Kennz. aus Produkten einlesen** Aus den Stammdaten der Produkte können automatische Zuschläge übergeben werden.
- Die Kennzeichen für automatische Zuschläge aus den Stammdaten der Produkte werden nicht berücksichtigt.
- [x] Die Kennzeichen für automatische Zuschläge aus den Stammdaten der Produkte werden neu eingelesen.

#### Modus
Mit der Wahl der Option geben Sie an, welche Daten neu berechnet bzw. neu eingelesen werden sollen. Im Bereich Optionen werden die zugehörigen Checkboxen freigeschaltet.

#### Selektion nach
- **Nummernverwalter:** Die Dokumente des gewählten Nummernverwalters sollen neu berechnet werden. Das Feld Nummernverwalter wird freigeschaltet.
- **SQL-Befehl:** Zur Auswahl der Dokumente wird ein SQL-Befehl eingegeben. Das Eingabefeld wird freigeschaltet.

**Mitarbeiter** Name des Mitarbeiters, der sich in A+W Business angemeldet hat.

**Nummernverwalter** Sie können den Nummernverwalter auswählen, in dem sich die zu überrechnenden Dokumente befinden. Die Auswahl wird durch die Wahl der Option im Bereich Dokumente eingeschränkt.
Das Feld ist gesperrt, wenn im Bereich Selektion nach die Option SQL-Befehl markiert ist.

**Eingabefeld, [Ausführen]** Das Eingabefeld für den SQL-Befehl ist nur freigeschaltet, wenn im Bereich Selektion nach die Option SQL-Befehl markiert ist.

#### Dokumente
In der Übersicht werden alle Dokumente aufgelistet, für die die Neuberechnung durchgeführt werden soll.

### TPS Faktura
> Dokumente > Auftrag > TPS Faktura

Dieser Dialog ist nur kundenspezifisch freigeschaltet.

### Garantiebelege
> Dokumente > Auftrag > Garantiebelege

Dieser Dialog wird nur kundenspezifisch genutzt.

### SAFT-PT Export
> Dokumente > Auftrag > SAFT-PT Export

*Abb. C-356 SAFT-PT Export*

In diesem Dialog legen Sie den Zeitraum fest, aus dem zertifizierte Rechnungen und Gutschriften für den portugiesischen Markt in eine XML-Datei exportiert werden sollen.

## Übergabe, Im-/Export von Dokumenten
Die Übergabe, der Import, der Export und die zugehörigen Menüs sind für Aufträge, Gutschriften und Bestellungen gleich. Die Dialoge werden in dieser Anleitung am Beispiel Auftrag beschrieben.

Zum diesem Thema finden Sie Informationen zu folgenden Themen:
- "FiBu-Übergabe" auf Seite C-695
- "Sollstellung FiBu" auf Seite C-698
- "Einstellungen FiBu-Übergabe" auf Seite C-700
- "Import/Export von Zahlungen" auf Seite C-701
- "Übergabe Archiv” auf Seite C-702
- "Import" auf Seite C-704
- "Fremddokumentenverwaltung" auf Seite C-705

### FiBu-Übergabe
> Dokumente > Auftrag, Gutschrift, Bestellung > FiBu-Übergabe

Sie können Rechnungen, Gutschriften und Bestellungen an ein externes Programm zur Finanzbuchhaltung (FiBu) übergeben.

Zum Thema FiBu-Übergabe finden Sie folgende Informationen:
- "Menü Funktionen" auf Seite C-696
- "Menü Optionen" auf Seite C-696
- "Sollstellung FiBu" auf Seite C-698
- "Einstellungen FiBu-Übergabe" auf Seite C-700
- "Import/Export von Zahlungen" auf Seite C-701

#### Menü Funktionen
> Dokumente > Auftrag, Gutschrift, Bestellung > FiBu-Übergabe > Menü Funktionen

Über dieses Menü können Sie andere Dialoge öffnen, ohne die FiBu-Übergabe zu schließen. Folgende Einträge werden angezeigt:
- **Historie:** Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des Dokuments.
  - ⇨ "Historie" auf Seite C-564
- **Produkt Export:** Dieser Eintrag ist nur in Verbindung mit FiBu-Programm Prodaja freigeschaltet. Die Produktstammdaten werden in eine ASCII-Datei exportiert.
- **Einstellungen:** Öffnet den Dialog Einstellungen FiBu-Übergabe, um zu den Dokumenten im Nummernverwalter Details für die Übergabe festzulegen.
  - ⇨ "Einstellungen FiBu-Übergabe” auf Seite C-700

#### Menü Optionen
> Dokumente > Auftrag, Gutschrift, Bestellung > FiBu-Übergabe > Menü Optionen

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

> **Aktivierte Optionen nach dem Öffnen des Dialogs**
> Bitte beachten Sie, dass geänderte Optionen erst beim nächsten Öffnen des Dialogs wirksam werden.
> Wenn durch eine aktivierte Option eine Prüfung gestartet wurde, kann sich das Öffnen eines Dokuments verzögern. Der Grad der Verzögerung hängt von der Leistungsfähigkeit des Rechners ab.
> Die folgenden Beschreibungen stellen die aktivierte Option dar.

Das Menü ist in folgende Gruppen gegliedert:
- "Gruppe Kosten" auf Seite C-696
- "Gruppe Kunden" auf Seite C-697
- "Gruppe Sonstige" auf Seite C-697

**Gruppe Kosten**
- **Übergabe Kostenrechnung:** Anzeige, ob die Kostenrechnung in den Firmendaten aktiviert wurde. Die Funktion kann über diesen Eintrag nicht aktiviert oder deaktiviert werden.
  - ⇨ Stammdaten, "Kostenrechnung aktiv" auf Seite B-938
- **Nur Rechnungen mit Wert > 0:** Nur die Rechnungen sollen an die FiBu übergeben werden, deren Rechnungssummer größer als Null ist.
- **Nur Buchungen mit Wert > 0:** Erlöskonten mit dem Betrag 0 sollen nicht an die FiBu übergeben werden.
- **Steuerkennzeichen separat verarbeiten:** Zur Ermittlung des korrekten Erlöskontos werden die Positionen und Stücklisten-Komponenten gemäß dem Steuerkennzeichen auf die Warengruppen gruppiert.
- **FiBu in Altwährung:** Die Funktion wird nur benötigt, wenn ein Kunde der gemeinsamen Währung Euro beitritt.
- **Fremdschlüssel als Währungskennzeichen übergeben:** Wenn Sie mit mehreren Währungen arbeiten und in den Stammdaten den Währungen den Fremdschlüssel Ihrer FiBu zugeordnet haben, können Sie diesen Fremdschlüssel an die FiBu übergeben. Die Währung wird dann anhand des Fremdschlüssels identifiziert.
  - ⇨ Stammdaten, "Währung" auf Seite B-921

**Gruppe Kunden**
- **Kundenübergabe deaktiviert:** Der Kundenname wird nicht übergeben.
- **Kundenkonto anstatt Kundennummer übergeben:** Wenn in den Kundendaten ein Debitorenkonto hinterlegt ist, wird dieses anstelle der Kundennummer übergeben.
  - ⇨ Stammdaten, “Partnerverwaltung - Finanzen" auf Seite B-785

**Gruppe Sonstige**
- **Automatische Sortierung aktiv (Kunde/Rechnung/Auftrag):** Die Daten werden zur Übergabe pro Kunde, Rechnung und/oder Auftrag automatisch sortiert. Wenn die Sortierung nicht aktiviert ist, wird die Sortierung aus dem Nummernverwalter übernommen.
- **Ausgabedatei überschreiben:** Diese Funktion wird nur benötigt, wenn die FiBu nicht mit Nummernkreisen sondern mit festen Dateinamen arbeitet. Die Ausgabedatei aus der vorigen Übertragung wird überschrieben. Wenn die Funktion ausgeschaltet ist, werden in der Ausgabedatei die neuen Daten hinzugefügt. Die Datei wird dabei immer größer.
- **OEM Konvertierung aktiv:** Für die FiBu-Übergabe kann die Konvertierung von Sonderzeichen aktiviert werden, z. B. ä in ae.
  Die OEM Konvertierung kann in den Firmendaten gesperrt werden.
  - ⇨ Stammdaten, "OEM/ANSI Konvertierung deaktivieren" auf Seite B-976

### Sollstellung FiBu
> Dokumente > Auftrag, Gutschrift, Bestellung > FiBu-Übergabe

*Abb. C-357 FiBu-Übergabe – Sollstellung FiBu*

In diesem Dialog geben Sie an, welche Rechnungen/Gutschriften an die FiBu (Finanzbuchhaltung) übergeben werden sollen. Der Dialog ist für alle FiBu-Programme gleich aufgebaut. In der Titelzeile wird jeweils der Name der FiBu angezeigt.

- ⇨ Tutorial, "Finanzbuchhaltung (FiBu)" auf Seite C-361

#### Identifikation
**Mandant** Mandant, für den die Rechnungen übergeben werden.

**Bereich** AV-Bereich, zu dem die Dokumente gehören.

**Mitarbeiter** Mitarbeiter, der sich in A+W Business angemeldet hat.

**Nummernverwalter** Nummernverwalter, in dem sich die zu übergebenden Rechnungen bzw. Gutschriften befinden.
Vor der FiBu-Übergabe prüft das Programm, ob mindestens ein Dokument im Nummernverwalter eine Rechnungsnummer enthält und den notwendigen Status für die Übergabe hat. Nur dann wird eine Laufnummer vergeben.

**Kontrollsumme** Wenn die Dokumente an die FiBu übergeben wurden, wird als Kontrollsumme die Gesamtsumme der übergebenen Beträge angezeigt.

**Lauf** Wenn die Dokumente an die FiBu übergeben wurden, wird die Nummer des Übergabelaufs angezeigt. Diese wird in aufsteigender Folge automatisch aus dem Nummernkreis genommen, der für den Mandanten und/oder AV-Bereich definiert ist.
- ⇨ Stammdaten, "Nummernkreise - FiBu" auf Seite B-908

#### Ausgabe
**Debitor/Kreditor** Pfad und Datei, in die die Daten geschrieben werden. Die Angaben werden aus den Firmendaten übernommen.
- ⇨ Stammdaten, "Pfad und Dateiname" auf Seite B-937

**Rechnung/Gutschrift** Pfad und Datei, in die die Daten geschrieben werden. Die Angaben werden aus den Firmendaten übernommen.

**Buchungsdatum** Als Buchungsdatum wird das Systemdatum angezeigt. Es kann überschrieben werden.

**Periode** Angabe der Buchungsperiode, zu der die Rechnungen und Gutschriften gehören.
- ⇨ Stammdaten, "Buchungsperioden" auf Seite B-1042

**Aktueller Auftrag** Nummer des Auftrags, der aktuell an die FiBu übergeben wird.

**Position** Nummer der Auftragsposition, die aktuell an die FiBu übergeben wird.

**Gesamt - Aufträge** Anzahl der Dokumente, die an die FiBu übergeben wurden.

**Positionen** Anzahl der Positionen, die an die FiBu übergeben wurden.

#### Übersicht
In der Übersicht werden alle Dokumente angezeigt, die sich im aktuellen Nummernverwalter befinden. Nur wenn Sie Rechnungen und Gutschriften über denselben Nummernverwalter übergeben, werden beide Dokumentenarten aufgelistet.

**Ergänzende Informationen**
- ⇨ Stammdaten, "Finanzen und Saldo" auf Seite B-82
- ⇨ Stammdaten, "Firmendaten - FiBu" auf Seite B-936
- ⇨ Tutorial, "Finanzbuchhaltung (FiBu)" auf Seite C-361
