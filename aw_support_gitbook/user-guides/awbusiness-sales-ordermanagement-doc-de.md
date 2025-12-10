---
title: "DE_AWBusiness_Verkauf_4_6"
source: "DE_AWBusiness_Verkauf_4_6.pdf"
tags: ["A+W Business", "Software Reference", "Sales", "Order Management", "Positionsdaten", "Sprossen", "Kalkulation", "Dokumente kopieren", "ERP", "Technical Documentation"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a detailed software reference manual for the A+W Business Verkauf (Sales) module, focusing on the management of position data within orders. It covers various functionalities such as configuring muntin bars (Sprossen), adding services (Leistung), managing additional data (Zusatz), and handling technical values and attachments for order items."
long_description: "This comprehensive software reference guide provides an in-depth explanation of the A+W Business Verkauf (Sales) application, specifically detailing the 'Positionsdaten' (Position Data) section for managing order items. The manual is structured to guide users through the various tabs and functions available for each order position. Key topics include the configuration of horizontal and vertical muntins (Sprossen), including the use of the A+W CAD Designer for custom constructions. It describes how to add and manage services (Leistung) and their relation to order items, as well as how to handle additional data (Zusatz) such as mixed-price calculations (Mischkalkulation) used in specific regions, supplier information, tax settings, and product-specific markings like CE and CPIP. The document also covers adding texts, file attachments, and technical values to positions. Further sections detail the document summary screen, which aggregates costs, credit limits, and totals for an entire order. A significant portion of the manual is dedicated to overviews and reference dialogs, explaining how to search for documents using various criteria, copy documents (fully or selectively), view document history, manage status changes, and handle partial deliveries, complaints, and down payments. It also explains functionalities for capacity planning, cost calculation, and production status feedback. The guide is intended for users who manage sales orders and need a thorough understanding of the software's capabilities for detailed and accurate order processing."
---

---
## Positionsdaten

### Waagerechte, Senkrechte Sprossen

Für jede Sprosse können Sie angeben, welcher Sprossenabschnitt nicht ein-gebaut werden soll. Standardmäßig sind alle waagerechten und senkrechten Sprossen markiert.

- Der Sprossenabschnitt wird nicht eingebaut.
- Der Sprossenabschnitt wird eingebaut.

### Sprossen – Muster

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Sprossen > Register Muster

*Abb. C-257 Sprossen - Muster*

In diesem Register erfassen Sie eine individuelle Sprossenkonstruktion.
Die Felder sind in den Registern **Standard** und **Preise** beschrieben.

**Schaltfläche [F12]** Mit dieser Schaltfläche öffnen Sie die Anwendung A+W CAD Designer, um die Sprossenkonstruktion zu gestalten. In dem Bearbeitungsdialog steht Ihnen eine eigene Online-Hilfe zur Verfügung.

### Positionen – Leistung

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Leistung

*Abb. C-258 Positionen - Leistung*

In diesem Register erfassen Sie Leistungen, die zu den Positionen hinzugefügt werden sollen. Die Leistungen werden in die Positionen zurückgeschrieben und in der Stückliste aufgeführt, wenn die Angaben gespeichert werden.

- ⇨ Tutorial, "Zuschlag für besondere Leistung erfassen" auf Seite C-129

#### Positionsbezug

In dieser Übersicht sind alle Auftragspositionen mit Stückzahl und Preisen aufgeführt. Eine Leistung wird nur für die Positionen berechnet, deren Checkbox markiert ist.

**[Alle], [Keine]** Über die Schaltflächen können Sie alle Checkboxen markieren oder die Markierung(en) entfernen.

### Leistungen

In der Übersicht werden alle erfassten Leistungen aufgeführt. Um sich anzeigen zu lassen, für welche Positionen die Leistung berechnet wird, markieren Sie die Leistung. Die Checkboxen der entsprechenden Positionen sind im Bereich Positionsbezug markiert.

Folgende Angaben werden angezeigt und können bearbeitet werden:

- **Produkt, Auswahl, Bezeichnung**: Auswahl, Nummer und Bezeichnung der ausgewählten Leistung.
- **Leist.-einheit**: Bezugsgröße, nach der die Leistung berechnet wird. (Leistungseinheit = LE)
- **Leistungsgröße**: Faktor für die Preisberechnung. Wenn Sie z. B. zu 3 Auftragspositionen mit je 12 Scheiben die Leistung Entsorgung pro Stück berechnen möchten, wird die Anzahl der Scheiben aus diesen 3 Positionen (36) angezeigt. Der Preis/LE wird mit dem Wert der Leistungsgröße multipliziert. Wenn die Leistung nach qm berechnet wird, gibt die Leistungsgröße die gesamte Fläche der entsprechenden Auftragspositionen wieder.
- **Darstellung**: Die Leistung kann implizit, explizit und implizit im Preis pro ME dargestellt werden.
    - ⇨ Tutorial, "Darstellung der Preise im Druck" auf Seite C-200
- **Druck**: Angabe, ob die Leistung mit ausgedruckt werden soll.
- **Jahrgang, Schlüssel**: Preisjahrgang und -schlüssel aus den Stammdaten. Sie können geändert werden.
- **Preis / LE**: Preis pro Leistungseinheit aus den Stammdaten. Er kann geändert werden.
- **Rabatt**: Rabatt aus den Stammdaten. Er kann geändert werden.
- **Stk. Netto**: Der Netto-Betrag pro Stück wird aus dem Preis/LE und dem Rabatt errechnet.
- **Pos. Netto**: Der Netto-Betrag für die gesamte Position ergibt sich aus dem Preis/LE, dem Rabatt und der Leistungsgröße.
- **Min. Menge**: Mindestbetrag, der berechnet werden soll.

### Positionen – Zusatz

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Zusatz

*Abb. C-259 Positionen – Zusatz*

In diesem Register erfassen und bearbeiten Sie Daten zur Mischkalkulation und zur Reklamation. Die Felder zeigen jeweils die Werte der markierten Position an. Alle Angaben gelten für das Hauptprodukt.

Die Felder werden so aktiviert und/oder aktualisiert, wie Sie es über die Menüs festgelegt haben.

- ⇨ "Menüs in der Positionserfassung" auf Seite C-440

### Mischkalkulation

> **i**
> Diese Form der Kalkulation wird nur in Österreich eingesetzt.
> Die Mischkalkulation wird angewendet, wenn der Preis aus zwei bzw. drei ISO-Preistabellen errechnet werden soll.
>
> **Stammdaten: Mischkalkulation**
> Die in diesem Dialog angelegte Mischkalkulation steht nicht in Verbindung mit der Mischkalkulation in den Stammdaten der Produkte.
> Wenn Sie Ihre ISO-Einheiten über eine Mischkalkulation berechnen, müssen Sie die Felder in der Positionserfassung Register Zusatz ausfüllen.

**ISO 1, 2, 3** Auswahl der Gläser in der erfassten ISO-Einheit. Die Gläser werden nicht automatisch angezeigt, wenn Sie eine ISO-Position markieren. Zur Berechnung des Gesamtpreises werden die zugehörigen Preise mit dem zugehörigen Faktor multipliziert.

**Faktor** Der Faktor bestimmt, wie der Preis des gewählten Glases bei der Mischkalkulation gewichtet wird. Die Faktoren werden aus den Firmendaten übernommen. Sie können im Auftrag geändert werden.
- ⇨ Stammdaten, "Mischkalkulationsfaktoren" auf Seite B-931

### Lieferant / Steuer / Zuschläge

**Lieferant** Wenn das Produkt bestellt werden muss, können Sie einen Lieferanten eintragen.
- ⇨ Stammdaten, "Lieferantenkartei" auf Seite B-855

**KOMO-Nr.** Zertifikatsnummer für niederländische Bauprodukte. Der eingetragene Wert wird an die Produktion und den Druck von Etiketten und Rahmentexten übergeben.

**Steuer** Auswahl der gültigen Steuern. Die Einstellung gilt jeweils für die Position, die im Bereich Positionen markiert ist.

**Zuschläge** Auswahl der gültigen Zuschläge. Die Einstellung gilt jeweils für die Position, die im Bereich Positionen markiert ist.

### Produktkennzeichnung

**CE Kennzeichen** CE-Kennzeichen aus den Stammdaten des Produktes.

#### CPIP Daten

**CPIP-Code** Characteristic Performance Identification Paper (Kenndaten zu den Eigenschaften und dem Leistungsverhalten). Der CPIP-Code wird aus den Produktdaten herangezogen.

**CE-Flag** Die Suche nach dem CPIP-Code und nach Restriktionen wird aus der Produktdefinition übernommen und kann im Auftrag deaktiviert werden.

- Die Suche nach dem CPIP-Code und nach Restriktionen ist deaktiviert. Sie kann nicht wieder aktiviert werden. Wenn die Funktion wieder aktiviert werden soll, müssen Sie das Produkt in einer neuen Position erfassen und die alte Position löschen.

> **i**
> Die Einstellung wird aus der Produktverwaltung übernommen. Wenn zu dem erfassten Produkt keine CPIP-Prüfung hinterlegt ist, kann die Funktion nicht ausgeführt werden.

### Reklamation

Diese Felder sind nur freigeschaltet, wenn Sie eine Reklamation erfasst haben oder bearbeiten.

Pro reklamierter Position können ein Verursacher, ein Grund und der VK-Preis angegeben werden. Diese Angaben können über die Reklamationsstatistik ausgewertet werden.

> **Dialog Reklamationen öffnen**
> Um die Felder zu füllten, öffnen Sie den Dialog Reklamationen über die Schaltfläche [Ordner].

- ⇨Tutorial, "Reklamationen" auf Seite C-282
- ⇨ "Reklamationen" auf Seite C-591

**Verursacher** Der Verursacher kann in der Statistik zur Auswertung herangezogen werden. Die Eingabe ist optional.

**VK** Verkaufspreis für die beanstandete Position. In Kulanzfällen kann dieser Wert unter dem tatsächlichen Preis liegen.

**Grund** Der Grund kann in der Reklamationsstatistik zur Auswertung herangezogen werden. Die Eingabe ist optional.

### Warengruppen

**Rabatt, Statistik** Warengruppen aus den Stammdaten der Produkte und aus Kombi-WGR. Die Einstellung gilt jeweils für die markierte Position.
- ⇨ Stammdaten, "Regeln für Kombi-WGR" auf Seite B-144

### Rahmen

**Text** Das Feld ist nur bei Produkten der Produktgruppe Isolierglas freigeschaltet. Sie können einen abweichenden Rahmentext angeben, der an die Produktion übergeben werden soll.
Wenn Sie mit CEKAL arbeiten, werden die CEKAL-Angaben aus der Produktdefinition übernommen.

**Rückschnitt** Der Rückschnitt, der beim Zuschneiden des Glases berücksichtigt werden muss, wird in mm angezeigt. Er kann überschrieben werden. Die Werte werden in die entsprechenden Felder im Rückschnitt im Register Sprossen übernommen.
- ⇨ "Positionen - Sprossen" auf Seite C-493

### Sonstiges

**Alternative zur Pos.** Dieses Feld ist für Angebote vorgesehen. Damit legen Sie fest, zu welcher Position die markierte Position als Alternative angeboten wird.
- ⇨ Tutorial, "Alternative Position im Angebot erfassen" auf Seite C-331

**Skontofähig** Die Einstellung wird aus der Produktdefinition übernommen. Sie kann überschrieben werden. Die Einstellung gilt für die markierte Position.

- Die markierte Position wird nicht zur Skontoberechnung herangezogen.
- Die markierte Position wird zur Skontoberechnung herangezogen.

**Verp.-Einheit** Die Verpackungseinheit wird an die Bestellung und die Produktion übergeben und kann ausgedruckt werden.

### Manuelle Vorgaben

**Stückgewicht** Gewicht pro Stück der aktuellen Position. Der Eintrag kann überschrieben werden. Diese Angabe wird zur Berechnung des Energiezuschlags herangezogen.
- ⇨ Stammdaten, "Energiezuschlag nicht nach Positionsgewicht berechnen" auf Seite B-952

**Teilgelief. Menge** Im Original-Auftrag ist die Stückzahl angegeben, die als Teillieferung der aktuellen Position bereits geliefert wurde. In allen anderen Dokumenten bleibt das Feld leer.

**Min. Menge** Angabe der Mindestmenge, sofern diese von den kundenspezifischen oder den firmenübergreifenden Einstellungen abweichen soll. Die Angabe gilt für die aktuelle Position.

**Maßrundung** Angabe der Maßrundung, sofern diese von den kundenspezifischen oder den firmenübergreifenden Einstellungen abweichen soll. Die Angabe gilt für die aktuelle Position.
- ⇨ Stammdaten, "Kaufmännische Maßrundung der Abmessung" auf Seite B-950
- ⇨ Stammdaten, "Standardrundung" auf Seite B-765

### Positionen

Die Felder sind zum Register Position beschrieben.
- ⇨ "Positionen" auf Seite C-456

### Positionen – Weitere Angaben

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Weitere Angaben

*Abb. C-260 Positionen - Weitere Angaben*

In diesem Register können Sie weitere Angaben zu Rahmentexten, zur Lagerverwaltung, zum Versand und zur Berechnung von Kosten und Provisionen eingeben. Die Angaben gelten jeweils für die markierte Position.

#### Texte

Die Felder in diesem Bereich beziehen sich auf die CEKAL-Angaben, wenn die CEKAL-Funktion freigeschaltet ist (nur in Frankreich).

**Pos. Gruppe** Nummer der markierten Position. Wenn mehrere Positionen zu einer Gruppe zusammengefasst wurden, ist dies die Nummer der Gruppe.

**Serienpos.** Die aktuelle Position kann zu einer Serie gehören.
- Die aktuelle Position gehört nicht zu einer Serie.
- Die aktuelle Position gehört zu einer Serie.

**Positionstext 1-5** Die Texte der aktuellen Position werden aus den Stammdaten übernommen. Sie können für diesen Auftrag geändert und ergänzt werden. Die Texte werden an die Produktion übergeben.
Im Feld Positionstext 5 wird der Wert für die Zuschlagsbasis angezeigt.
- ⇨ "Zuschlagsbasis" auf Seite C-510

**CEKAL Etikett** Text, der auf das CEKAL-Etikett gedruckt wird. Er wird aus den Stammdaten übernommen und kann geändert werden.
- ⇨ Stammdaten, "Produkttexte" auf Seite B-1082

**CEKAL Allgemein** Allgemeiner Text bei CEKAL-Aufträgen. Er wird aus den Stammdaten übernommen und kann geändert werden.

**CEKAL Produktion** Text, der bei CEKAL-Aufträgen an die Produktion übergeben wird. Er wird aus den Stammdaten übernommen und kann geändert werden.

#### Produktion

**Produktionslinie** Angabe, in welcher Produktionslinie die Position gefertigt werden soll. Die Angabe kann an die Produktion übergeben werden.

**Etikettenlogo** Nummer des Logos aus den Stammdaten des Kunden. Die Einstellung kann für diesen Auftrag überschrieben werden.
- ⇨ Stammdaten, "Produktionsetiketten" auf Seite B-786

**Autom. Zuschnitt** Angabe aus den Stammdaten des Produktes. Diese Information wird an A+W Production weitergegeben. Die Einstellung kann für diesen Auftrag überschrieben werden.
- Das Glas wird nicht automatisch zugeschnitten. Es muss von Hand geschnitten werden.
- Das Glas wird automatisch zugeschnitten.
- ⇨ Stammdaten, "Produktkennzeichen" auf Seite B-610

**Randentschichtung** Die Randentschichtung wird als Bearbeitung eingefügt.
- An den Gläsern wird keine Randentschichtung ausgeführt.
- ✔ Die Gläser werden randentschichtet.
- ⇨ "Randentschichtungen" auf Seite C-480

#### Abweichende Mengen

**Über-/Untermenge** Zulässige Über- und Untermengen aus den Produktstammdaten. Die Werte können pro Auftrag überschrieben werden. Übermengen aus A+W Production können akzeptiert werden, wenn dateilose Rückmeldungen empfangen werden.
- ⇨ Stammdaten, "Produktverwaltung - Fertigung" auf Seite B-596
- ⇨ Fertigung, "Übermengen” auf Seite E-78

#### Gestell

**Typ / Anzahl** Gestelltyp und Anzahl der Gestelle, auf die die Position gepackt werden soll.
- ⇨ Stammdaten, "Produktverwaltung - Fertigung" auf Seite B-596

#### Zuschlag

**Zuschlagsbasis** Wenn im aktuellen Auftrag ein automatischer Zuschlag berechnet wird, wird in diesem Feld der Wert angezeigt, der als Basis für die Berechnung herangezogen wird, z. B. das Gewicht.
- ⇨ "Automatische Zuschläge" auf Seite B-324

#### Kosten

Die Kostenart und die Kostenstellen sind in den Stammdaten der Produkte hinterlegt. Die Daten können über externe Berichte ausgewertet werden.
- ⇨ Stammdaten, "Kostenrechnung" auf Seite B-603

**Kostenstelle** Kostenstelle, auf die das Produkt gebucht wird.
- ⇨ Stammdaten, "Kostenstellen" auf Seite B-914

**Kostenart** Kostenart, auf die das Produkt gebucht wird.
- ⇨ Stammdaten, "Kostenart" auf Seite B-913

#### Auslieferung

Die Angaben in diesem Bereich können auf den Lieferschein gedruckt werden. Die Auswahl in den Feldern wird im Modul Fertigung hinterlegt.
- ⇨ "Kommissionierung" auf Seite E-230

**Abladestelle** Standard-Abladestelle beim Kunden. Sie kann für den aktuellen Auftrag geändert werden.

**Packregel** Standard-Packregel für den Kunden. Sie kann für den aktuellen Auftrag geändert werden.

**Gruppenbildung** Standard-Packmittelgruppe des Kunden. Sie kann für den aktuellen Auftrag geändert werden.

#### Skizzendruck

Standardmäßig werden die Angaben zum Skizzendruck aus den Stammdaten der Produkte übernommen.
- ⇨Tutorial, "Druck von Skizzen" auf Seite C-196

> **i**
> **Skizzendruck festlegen**
> Sie können den Skizzendruck in verschiedenen Dialogen pro Position festlegen. Wenn Sie die Einstellung ändern, werden die Angaben in allen entsprechenden Feldern aktualisiert.
> Sie können die Druckausgabe über den S+N-Editor anpassen, wenn z. B. die Maßangaben nicht deutlich zu erkennen sind.

**Modell / Sprosse** Einstellung, wie die Skizze auf den Formularen gedruckt werden soll:
- **Kein Druck**: Skizzen werden auf den Formularen nicht gedruckt.
- **Maßstäblich**: Bei dieser Einstellung werden maßstabsgetreue Skizzen gedruckt.
- **Schematisch**: Bei dieser Einstellung werden die Standardskizzen gedruckt. Sie geben lediglich das Schema des Modells oder Sprossenaufbaus wieder und enthalten keine Maße.

Diese Einstellungen werden abhängig von den Einstellungen im Formulardruck ausgewertet.
- ⇨ Stammdaten, "Formularverwaltung - Skizzendruck" auf Seite B-1063

#### Dokumentenreferenzen

**Bestellreferenz, Auslieferungsauftrag, Endkundennr. / -Pos** Sie können zu jeder Position eine Referenz auf die Bestellung, den Auftrag und den Kunden eingeben. Diese Referenz kann alphanumerisch angegeben und durch die Positionsnummer aus dem Referenzdokument ergänzt werden.

#### Provision

Die Angaben für die Provision werden aus den Stammdaten der Produkte übernommen. In den Firmendaten kann eingestellt werden, wie die Berechnung der Provision durchgeführt werden soll.
- ⇨ Stammdaten, "Interaktive Vertreterprovisionierung" auf Seite B-939

**Satz 1 / 2** Der hinterlegte Provisionssatz wird nur angezeigt, wenn in den Firmendaten die interaktive Vertreterprovisionierung aktiviert ist.
Pro Position können zwei verschiedene Provisionssätze angegeben werden. Diese werden jeweils dem Vertreter 1 bzw. Vertreter 2 zugeordnet.
- ⇨ Stammdaten, "Vertreterprovision" auf Seite B-376

#### Positionen

Die Felder sind zum Register Position beschrieben.
- ⇨ "Positionen" auf Seite C-456

### Positionen - Texte

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Texte

*Abb. C-261 Positionen - Texte*

In diesem Register können Sie zu jeder Auftragsposition einen Text erfassen.
Die Angaben gelten jeweils für die markierte Position. Mit den Schaltflächen zur Navigation können Sie durch die Positionen blättern.
- ⇨Tutorial, "Text erfassen" auf Seite C-54

#### Blockübersicht

Sie können einen Text hinzufügen, indem Sie entweder einen der hinterlegten Standardtexte auswählen oder einen neuen Text eingeben.

Die Felder werden über die Schaltfläche freigeschaltet.

Ein eingefügter Text wird vollständig über die Schaltfläche entfernt.

**Nummer** Textnummer des Standardtextes. Wenn Sie einen eigenen Text hinzufügen, tragen Sie die Nummer 0 (null) ein.
- ⇨ Stammdaten, "Texte" auf Seite B-1045

**Textkennz.** Das Textkennzeichen gibt an, für welchen Dokumententyp der Text gültig ist.

Zum Beispiel wird der Text mit dem Textkennzeichen P nur auf den Produktionspapieren gedruckt.

In der Formularverwaltung können Sie Texte zum Druck auf bestimmten Formularen ausschließen.
- ⇨ Stammdaten, "Textarten" auf Seite B-462
- ⇨ Stammdaten, "Formularverwaltung - Texte" auf Seite B-1055

**Vor, nach Position, produktbezogen** Über die Wahl der Option bestimmen Sie, an welcher Stelle im Dokument der Text gedruckt werden soll. Die Angaben beziehen sich immer auf die markierte Position.

Bei mehreren Texten pro Position beziehen sich die Angaben nur auf den Text, der in der Übersicht der zugewiesenen Texte markiert ist.

Folgenden Angaben werden gedruckt:
- **Vor Position:** Vor der Produktbezeichnung.
- **Produktbezogen:** Vor der Positionszeile mit Maßen.
- **Nach Position:** Nach der Positionszeile mit Maßen.

Die Standard-Option kann im Menü Optionen > Textpositionierung eingestellt werden.
- ⇨ "Menü Optionen" auf Seite C-445

**(Übersicht)** In der Tabelle werden alle Texte aufgelistet, die in diesem Dokument gedruckt werden sollen. Die Checkbox Nachher zeigt an, welche Option zum Einfügen des Textes gewählt wurde.

#### Textblock

**Text beibehalten** Diese Checkbox ist nur freigeschaltet, wenn Sie einen Text hinzufügen.
- Der Text wird nur zu der aktuellen Position hinzugefügt.
- Der Text wird zu allen Positionen hinzugefügt, die nach der aktuellen Position erfasst werden. Er kann von jeder einzelnen Position wieder entfernt werden.

**Manuell geändert** Diese Checkbox zeigt an, welche Texte manuell hinzugefügt oder geändert wurden. Diese Texte können im Formulardruck nicht übersetzt werden. Bei Standardtexten ist die Checkbox nicht markiert.
- Der Standardtext ist unverändert übernommen.
- Der Text wurde manuell erstellt oder ein Standardtext wurde geändert.

**Schaltflächen** Sie können die Schriftart und -größe ändern und Hyperlinks, Bilder und Tabellen einfügen.
- ⇨ Tutorial, "Text erfassen" auf Seite C-54

**Textfeld** Das Textfeld wird freigeschaltet, wenn Sie auf die Schaltfläche zum Hinzufügen eines Textes klicken.
Schreiben Sie direkt in das Textfeld, wenn Sie einen Text eingeben oder ändern möchten.

#### Position

Die Felder sind zum Register Position beschrieben.
- ⇨ "Positionen" auf Seite C-456

### Positionen – Anlagen

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Anlagen

*Abb. C-262 Positionen - Anlagen*

In diesem Register können Sie Dateien als Anhang hinterlegen und prüfen, welche Anhänge mit dem Dokument gespeichert sind. Dateianhänge können Sie mit einem Doppelklick öffnen.

Der Anhang gilt jeweils für die markierte Position.
- ⇨ Tutorial, "Dokumente anhängen" auf Seite C-57

#### Dateianhang

Der Dateiname und der Pfad werden angezeigt. Sie können zu jedem Anhang eine Bemerkung hinzufügen, die den Anhang kurz beschreibt.

In den Firmendaten ist festgelegt, wo die Anhänge gespeichert werden.
- ⇨ Stammdaten, "Dateianhänge" auf Seite B-934

#### Positionen

Die Felder sind zum Register Position beschrieben.
- ⇨ "Positionen" auf Seite C-456

### Positionen – Technische Werte

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Technische Werte

*Abb. C-263 Positionen - Technische Werte*

In diesem Register können Sie die technischen Werte eines Produkts festlegen. Wenn die A+W SLT-Schnittstelle konfiguriert ist, werden die Werte über die A+W SLT-Schnittstelle ermittelt.

### Technische Werte

**[Schaltflächen]** Über die Schaltflächen können Sie einen Eintrag hinzufügen oder löschen.

> **i**
> **Leistungserklärung**
> Pro Kunde und Produkt kann in den Stammdaten festgelegt werden, ob eine Leistungserklärung angegeben werden muss.

**Leistungserklärung** Nummer der Leistungserklärung, die dem Auftrag zugeordnet werden soll. Die Nummer kann eingegeben oder über die Schaltfläche [Lupe] oder [Ordner] ausgewählt werden.
Die Nummer wird automatisch erzeugt, wenn die A+W SLT-Schnittstelle konfiguriert ist und der Produktaufbau zum ersten Mal generiert wird.

**[Taschenrechner]** Die Schaltfläche ist nur kunden- und/oder produktspezifisch freigeschaltet. Über die Schaltfläche können Sie die Technischen Werte für die Leistungserklärung berechnen lassen.

### Positionen

Die Felder sind zum Register Position beschrieben.
- ⇨ "Positionen" auf Seite C-456

### Positionen - Klassifikatoren

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Klassifikatoren

*Abb. C-264 Positionen - Klassifikatoren*

In diesem Register können Sie die Klassifikatoren des erfassten Produkts prüfen und bearbeiten. Die Klassifikatoren werden auch angezeigt, wenn das Produkt eine Stücklistenkomponente ist.

Im Formulardruck und in der Dokumentenansicht können die Klassifikatoren an den Report übergeben werden.

#### Positionen

Die Felder sind zum Register Position beschrieben.
- ⇨ "Positionen" auf Seite C-456

### Dokument – Summen

> Dokumente > Auftrag > Auftrag auswählen > Register Summen

*Abb. C-265 Dokument – Summen*

In diesem Register prüfen Sie die Kosten und das Kreditlimit. Zur Information werden Summen zum Auftrag und zu technischen Größen angezeigt. Außerdem können Sie einen Festpreis für den Auftrag insgesamt angeben.

#### Summen (technische Parameter)

In diesem Bereich werden die Summen zu Flächen, Umfang und Gewicht angezeigt. Die Felder sind leer, wenn Sie den Auftrag anlegen und noch keine Positionen erfasst sind. Die Felder geben die tatsächlichen Werte und die gerundeten Werte an.

**Stückzahl (gesamt / ISO-Einheiten)** Anzeige der gesamten Stückzahl und der Stückzahl der ISO-Einheiten.

**Summe Fläche (real / fakt.)** Anzeige der gesamten Fläche, die aus den Angaben zur Breite und Höhe errechnet ist. (fakt. = fakturiert)
- Der erste Wert zeigt die tatsächliche Summe der Fläche an.
- Der zweite Wert zeigt die Summe an, bei der die Einstellungen zur Berechnung berücksichtigt wurden. Wenn für die Preisberechnung das umschreibende Rechteck und/oder Mindestmengen zugrunde gelegt werden, sind unterschiedliche Werte möglich.

**Summe Umfang (real / fakt.)** Anzeige der gesamten Kantenlänge, die aus den Angaben zur Breite und Höhe errechnet ist.
- Der erste Wert zeigt die tatsächliche Summe der Kanten an.
- Der zweite Wert zeigt die Summe an, bei der die Einstellungen zur Berechnung berücksichtigt wurden. Wenn für die Preisberechnung das umschreibende Rechteck und/oder Mindestmengen zugrunde gelegt werden, sind unterschiedliche Werte möglich.

**Summe Gewicht (real / Tara)** Anzeige des Gesamtgewichts des Auftrags und des Gewichts der Verpackung. Das Feld Tara bleibt leer, wenn keine Angaben zur Verpackung erfasst sind.

**Summe Sprossenlänge (real / fakt.)** Anzeige der gesamten Länge aller Sprossen, die in diesem Auftrag erfasst wurden.
- Der erste Wert zeigt die tatsächliche Summe der Sprossenlängen an.
- Der zweite Wert zeigt die Summe an, bei der die Einstellungen zur Berechnung berücksichtigt wurden. Wenn für die Preisberechnung Mindestmengen zugrunde gelegt werden, sind unterschiedliche Werte möglich.

**Ergänzende Informationen**
- ⇨ Stammdaten, "Maßrundung Breite / Höhe" auf Seite B-606
- ⇨ Stammdaten, "Kaufmännische Maßrundung der Abmessung" auf Seite B-950
- ⇨ Stammdaten, "Firmendaten - Preisberechnung" auf Seite B-946
- ⇨ "Maßrundung" auf Seite C-430

#### Kosten/Deckungsbeitrag

Diese Anzeigen der Kosten und Deckungsbeiträge sind insbesondere dann von Interesse, wenn die vorgegebenen Preise manuell geändert werden. Bei dieser Anzeige gilt die Differenz zwischen VK und EK als Deckungsbeitrag.
Wenn Sie mit der Kostenkalkulation arbeiten, wird der Deckungsbeitrag auf der Grundlage der Produktpreise errechnet.
Die Felder sind leer, wenn noch keine Positionen erfasst sind.

**Materialkosten** Anzeige der Materialkosten, die in diesem Auftrag enthalten sind.

**Zeitkosten** Anzeige der Zeitkosten, die in diesem Auftrag enthalten sind. Diese Kosten werden nur angezeigt, wenn der Auftrag an die Kapazitätsplanung übergeben und eingelastet wurde.

**DB% 1, 2** Für Material-, die Zeit- und Frachtkosten werden die Deckungsbeiträge ermittelt.
- Der erste Wert zeigt den absoluten Wert des errechneten Deckungsbeitrags für diesen Auftrag an.
- Der zweite Wert zeigt den prozentualen Wert des errechneten Deckungsbeitrags für diesen Auftrag an.

**Frachtkosten** Die Frachtkosten werden aus der Entfernung und dem in den Stammdaten der Touren hinterlegten Preis pro Kilometer errechnet. Die Entfernung ist in den Kundenstammdaten hinterlegt oder im Register Abweichende Anschriften für den aktuellen Auftrag angepasst.
Über die Schaltfläche öffnen Sie die Übersicht zu den kalkulatorischen Frachtkosten.
- "Kalkulatorische Frachtkosten" auf Seite C-574

**Frachtkosten %** Der prozentuale Anteil der Frachtkosten bezieht sich auf den Gesamtwert des Auftrags.

**Gesamtkosten** Anzeige der Gesamtkosten aller Positionen, die im Auftrag enthalten sind.

**Festkosten** Sie können einen Wert für die Festkosten (EK) des gesamten Auftrags festlegen.

#### Kreditlimit

Das Kreditlimit wird auch dann automatisch aktualisiert, wenn aus dem Programm zur Finanzbuchhaltung (FiBu) keine offenen Posten zurückgemeldet werden. Die Aufträge werden bis zur FiBu-Übergabe berücksichtigt.

Das Limit 1 gibt den versicherten Betrag an, das Limit 2 den unversicherten.

Zur Berechnung des Saldos werden die Angaben aus den Kundendaten herangezogen.

Der Saldo ergibt sich aus folgender Berechnung:
Limit 1/2 - OP (FiBu) - Obligo - Aufträge = Saldo 1/2

Die Werte in den Feldern für Saldo 1/2 werden in roter Schrift angezeigt, wenn das Kreditlimit überschritten ist.
- ⇨ Stammdaten, "Partnerverwaltung - Saldo" auf Seite B-779
- ⇨Tutorial, "Kreditlimit" auf Seite C-47

#### Wertvolumen

In den beiden Spalten dieses Bereichs werden die Beträge in der Landeswährung und in der Fremdwährung angezeigt. Die Summen werden automatisch aktualisiert, wenn Änderungen gespeichert werden.

**Währung** Anzeige der Währung, die im Register Konditionen festgelegt wurde.
- ⇨ "Währung" auf Seite C-432

**Auftragssumme** Anzeige der aktuellen Summen, die aus den Preisen zu den erfassten Positionen berechnet werden. Wenn Sie einen Festpreis oder einen Rabatt eingegeben haben, werden die Preise beim Speichern neu berechnet.

**Festpreis** Sie können einen Festpreis für den gesamten Auftrag eintragen. Die Preise der erfassten Positionen werden anteilsmäßig umgerechnet, wenn Sie den Festpreis speichern. Die Preiseinheit wird für alle Positionen auf Stück gesetzt.

**Rabatt %** Sie können einen Rabatt auf den gesamten Auftragswert eingeben. Die Rabatte in den Positionen werden dann auf null gesetzt. Die Preise der Positionen werden auf Stückpreise umgerechnet.

> **i**
> **Beträge in roter Schrift**
> Die Beträge für Auftragssumme, Netto und Brutto werden nur zur Verdeutlichung in roter Schrift angezeigt.

**= Netto** Anzeige des errechneten Nettowertes für diesen Auftrag.

**Steuersatz** Sie können den Steuersatz aus den Stammdaten für diesen Auftrag überschreiben. Zur Auswahl werden alle Steuersätze angezeigt, die in den Stammdaten hinterlegt sind.
Wenn Sie den Steuersatz für diesen Auftrag ändern, prüft A+W Business, ob für den Kunden Sammelrechnungen vereinbart sind. Bei Sammelrechnung wird eine Meldung angezeigt, mit der die Steuer neu berechnet werden kann.
- ⇨ Stammdaten, "Steuer" auf Seite B-904

**Steuerbasis** Anzeige des Betrages, aus dem die Steuer berechnet wird.

**= Brutto** Anzeige des Bruttoauftragswerts, der sich aus dem Auftragswert und der Steuer ergibt.

**Skonto** Anzeige des Betrages, der als Skonto abgezogen werden kann. Der prozentuale Wert für die Skonto-Berechnung wird in den Zahlungsbedingungen festgelegt, die dem Kunden zugeordnet sind.
- ⇨ Stammdaten, "Fälligkeitsberechnung" auf Seite B-775
- ⇨ Stammdaten, "Skontoberechnung" auf Seite B-782
- ⇨ Stammdaten, "Zahlungsbedingungen" auf Seite B-906

**Anzahlungssumme** Anzeige der bereits geleisteten Anzahlungssumme. Dieses Feld ist nur gefüllt, wenn Anzahlungen geleistet wurden.
Über die Schaltfläche öffnen Sie den Dialog Zahlungsverwaltung, um eine Anzahlung zu erfassen.
- ⇨ Tutorial, "Anzahlung erfassen" auf Seite C-277
- ⇨ "Zahlungsverwaltung" auf Seite C-580

## Übersichten und Referenzen zu Kopfdaten

> Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung

Sie können sich über die Menüs in der Dokumentenverwaltung verschiedene Informationen anzeigen lassen, ohne den Dialog zu schließen. Die Dialoge sind für alle Dokumentenarten gleich. Sie werden in dieser Anleitung am Beispiel Auftrag beschrieben.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:

- "Dokument suchen" auf Seite C-523
- "Dokumente kopieren" auf Seite C-532
- "Dokument anzeigen" auf Seite C-548
- "Kundeninfo" auf Seite C-549
- "Kapazitätsübersicht" auf Seite C-550
- "Historie" auf Seite C-552
- "Statusänderung" auf Seite C-554
- "NV Auswahl" auf Seite C-555
- "Lagermaße in Kisten verpacken" auf Seite C-556
- "Teillieferungsübersicht" auf Seite C-558
- "Reklamationsübersicht" auf Seite C-560
- "Anzahlungsübersicht" auf Seite C-561
- "Auftrags-/Bestell-Info" auf Seite C-562
- "Duplikate” auf Seite C-564
- “Kundenbenachrichtigung (Lieferterminkontrolle)" auf Seite C-565
- "Kapazitätsinfo nach Kunde" auf Seite C-570
- "OP Abfrage" auf Seite C-572
- "Kalkulatorische Frachtkosten" auf Seite C-574
- "Kosten- und Aufschlagskalkulation" auf Seite C-575
- "Übersicht Statusrückmeldung" auf Seite C-576
- "Lieferterminbestimmung" auf Seite C-578
- "Liefertermin ändern" auf Seite C-579
- "Zahlungsverwaltung" auf Seite C-580

### Dokument suchen

> Dokumente > Auftrag > Suche
> Dokumente > Auftrag > Auftrag> [Lupe] am Feld Nummer

Sie können die Dokumente über unterschiedliche Kriterien suchen. Die gewählten Kriterien werden beim Schließen des Dialogs gespeichert und beim Öffnen wieder geladen.

Die Dokumentensuche ist für alle Dokumentenarten gleich. Der Dialog wird in dieser Anleitung am Beispiel Auftrag beschrieben.

In diesem Dialog finden Sie folgende Register:

- "Dokumente suchen - Auftragsbezogen" auf Seite C-524
- "Dokumente suchen – Positionsbezogen" auf Seite C-525
- "Dokumente suchen – Stücklistenbezogen" auf Seite C-526
- "Dokumente suchen - Tabelle" auf Seite C-527
- "Dokumente suchen – Optionen" auf Seite C-529
- "Dokumente suchen - Detailübersicht" auf Seite C-531

#### Gruppe Suche

> Dokumente > Auftrag > Suche > Menü Start > Gruppe Suche

Die Suche kann sich auf die Hauptdatenbank und auf die Archive beziehen. Sie können folgende Einträge wählen:

- **Haupt (F2)**: Startet die Suche in der Hauptdatenbank. Sie können alternativ auch die Taste <F2> drücken.
- **Archiv (Shift+F2)**: Startet die Suche im Archiv. Sie können alternativ auch die Tastenkombination <Shift>+<F2> drücken.
- **Komplett (F3)**: Startet die Suche in der Haupt- und in der Archivdatenbank. Die Schaltfläche ist nur freigeschaltet, wenn im Register Optionen die Checkbox Archiv markiert und mindestens ein Archiv ausgewählt ist. Sie können alternativ auch die Taste <F3> drücken.
- **Werte löschen**: Setzt die Suchkriterien zurück.

### Dokumente suchen – Auftragsbezogen

> Dokumente > Auftrag > Suche > Register Auftragsbezogen

*Abb. C-266 Dokumente suchen – Auftragsbezogen*

In diesem Register können Sie Suchkriterien festlegen, die sich auf den Dokumentenkopf beziehen. Um die Suche auf die Archivdatenbanken auszudehnen oder einzuschränken, können Sie im Register Optionen das gewünschte Archiv auswählen.

#### Kriterien von, bis

Die Auswahllisten zeigen nur Einträge an, die sich auf Angaben zum Auftragskopf beziehen.

Der erste Wert wird automatisch im zweiten Feld wiederholt. Die Suche kann mit beliebig vielen Kriterien eingeschränkt werden.

**Suchkriterium (erstes Feld)** Auswahl des Suchkriteriums, z. B. Erfassungsdatum. Das zweite Feld wird freigeschaltet.

**Operator (zweites Feld)** Die nachfolgenden Einschränkungen können als Folge oder als exakter Wert angegeben werden:
- **Von-Bis**: Mit dieser Einstellung wird eine Folge definiert. Die Felder von und bis werden freigeschaltet.
- **=**: Mit dieser Einstellung wird die Suche auf einem exakten Wert eingeschränkt. Das Feld bis wird gesperrt.

**Kunde** Dokumente zu einem bestimmten Kunden werden gesucht. Name und Ort werden aus den Kundendaten eingelesen.

**Objekte** Dokumente zu einem bestimmten Objekt werden gesucht. Der Name wird aus den Stammdaten eingelesen.

### Dokumente suchen – Positionsbezogen

> Dokumente > Auftrag > Suche > Register Positionsbezogen

*Abb. C-267 Dokumente suchen - Positionsbezogen*

In diesem Register können Sie Suchkriterien festlegen, die sich auf die Auftragspositionen beziehen. Über die Kombination von Produktnummer und Maßangaben können Aufträge mit identischen Positionen gesucht werden.

#### Kriterien von, bis

Die Auswahllisten zeigen nur Einträge an, die sich auf Angaben zu Positionen beziehen.

Die Felder werden auf die gleiche Weise genutzt wie im Register Auftragsbezogen.
- ⇨ "Dokumente suchen – Auftragsbezogen" auf Seite C-524

**Produktnummer, Produktbezeichnung** Die Suche wird auf Dokumente eingeschränkt, in denen ein bestimmtes Produkt erfasst ist.

**Produktart** Die Suche wird auf Dokumente eingeschränkt, in denen eine bestimmte Produktart erfasst ist.

#### Warengruppe

Die Suche kann auf Dokumente eingeschränkt werden, in denen eine bestimmte Warengruppe für Rabatte oder die Statistik angesprochen wird. Folgende Einträge stehen zur Wahl:

- **Kombi. Rab.**: Kombi-Warengruppe für Rabatte.
- **Kombi. Stat.**: Kombi-Warengruppe für die Statistik.
- **Rabatt**: Warengruppe für Rabatte.
- **Statistik**: Warengruppe für die Statistik.

### Dokumente suchen – Stücklistenbezogen

> Dokumente > Auftrag > Suche > Register Stücklistenbezogen

*Abb. C-268 Dokumente suchen – Stücklistenbezogen*

In diesem Register können Sie Suchkriterien festlegen, die sich auf die Angaben in der Stückliste beziehen.

#### Kriterien von, bis

Die Auswahllisten zeigen nur Einträge an, die sich auf Angaben zur Stückliste beziehen.
Die Felder werden auf die gleiche Weise genutzt wie im Register Positionsbezogen.
- ⇨ "Dokumente suchen - Auftragsbezogen" auf Seite C-524

### Dokumente suchen – Tabelle

> Dokumente > Auftrag > Suche > Register Tabelle

*Abb. C-269 Dokumente suchen - Tabelle*

In diesem Register wird das Suchergebnis als Trefferliste angezeigt.

#### Tabelle

In der Tabelle sind die Suchkriterien aus den Registern als Spalten dargestellt.
- **Nr.**: Nummer des Dokuments
- **Kunde / Lieferant**: Name des Marktpartners.
- **Archiv**: Archivjahr des Dokuments.
- **Status**: Statusnummer des Dokuments.
- **Erfass. Datum**: Erfassungsdatum des Dokuments.
- **Lieferscheindatum**: Datum der Lieferscheinerstellung.
- **Versandtag**: Versanddatum des Dokuments.
- **Rechnung Nummer**: Rechnungsnummer des Dokuments.
- **Rechnung Datum**: Rechnungsdatum des Dokuments.
- **Kommission**: Die vom Kunden vorgegebene Kundenkommission.
- **Tour**: Tour, die von der Spedition gefahren wird.
- **Betrag Netto**: Nettopreis des Dokuments.
- **Betrag Netto (FW)**: Nettopreis des Dokuments in Fremdwährung.
- **Deckungsbeitrag (%)**: Prozentsatz des Deckungsbeitrags.
- **Prod. Start**: Tag, an dem die Produktion (spätestens) starten muss.
- **Anlief. Lief.**: Tag, an dem die Lieferung (spätestens) eintreffen muss.
- **Prod. Ende**: Tag, an dem die Produktion abgeschlossen ist.
- **Anlieferung**: Tag der gewünschten Anlieferung beim Kunden.
- **Bestelltext 1, Bestelltext 2**: Ergänzende Angaben zur Bestellung.
- **Laufnummer Produktionsübergabe**: Laufnummer der Produktionsübergabe.
- **Laufnummer Produktionsrückmeldung**: Laufnummer(n) der Produktionsrückmeldung(en).
- **Gesamtstückzahl**: Gesamte Stückzahl.
- **Gesamt-QM**: Gesamte Quadratmeterzahl.
- **Lieferant(en)**: Name des Lieferanten.
- **AB-Lieferant**: Nummer der Auftragsbestätigung durch den Lieferanten.
- **Lieferanschrift- Name, Adresse, Ort**: Lieferanschrift des Marktpartners.
- **Telefon, Fax**: Kontaktdaten des Marktpartners.
- **Abrechnung**: Nummer der Abrechnung.
- **Zahlungsweg**: Zahlungsweg, der mit dem Kunden vereinbart wurde, z. B. Rechnung, per Scheck, per Überweisung usw.
- **Zahlungsbedingung**: Zahlungsbedingung, die mit dem Kunden vereinbart wurde.

### Dokumente suchen – Optionen

> Dokumente > Auftrag > Suche > Register Optionen

*Abb. C-270 Dokumente suchen – Optionen*

In diesem Register können Sie die Archive auswählen, in denen gesucht werden soll.

#### Suche in

Mit der Wahl der Option legen Sie fest, nach welchem Dokumententyp gesucht werden soll, z. B. nach Angeboten.

**(Archivjahr)** Die Suche nach Dokumenten kann Dokumente im Archiv mit einbeziehen. Sie können die Suche auf ein oder mehrere Archivjahre einschränken. In der Trefferliste werden die archivierten Dokumente in roter Schrift angezeigt.
- Das Archivjahr wird nicht durchsucht.
- Das Archivjahr wird durchsucht.

**[Alle]** Die Schaltfläche wählt alle Archivjahre für die Suche aus.

**[Keine]** Die Schaltfläche wählt alle Archivjahre ab. Die Suche bezieht sich nur auf die Hauptdatenbank.

**Gesperrte Einträge anzeigen** Dokumente mit Kriterien, die gesperrt sind, können angezeigt werden, z. B. für die Suche nach einer (inzwischen) gesperrten Tour.
- Dokumente mit gesperrten Kriterien werden nicht angezeigt.
- Dokumente mit gesperrten Kriterien werden angezeigt. Die Kriterien können für die Suche ausgewählt werden.

**Groß- und Kleinschreibung beachten** Die Groß- und Kleinschreibung kann bei Suchkriterien beachtet werden, die sich auf Text beziehen.
- Die Groß- und Kleinschreibung wird nicht berücksichtigt. Diese Einstellung sollten Sie wählen, wenn die Bezeichnungen für Produkte, Kunden usw. nicht nach einheitlichen Regeln eingegeben wurden.
- Die Groß- und Kleinschreibung wird bei der Suche berücksichtigt.

**Archivdokumente farbig kennzeichnen** In der Dokumentensuche können die Einträge für Archivdokumente automatisch farblich markiert werden.
- Die Archivdokumente werden nicht farbig gekennzeichnet.
- Die Archivdokumente werden rot gekennzeichnet.

**Dokumentenerfassung per Doppelklick** Sie können Dokumente per Doppelklick aus der Dokumentensuche heraus öffnen.
- Das markierte Dokument kann nicht per Doppelklick geöffnet werden. Die Dokumentenerfassung kann über das Kontextmenü aufgerufen werden.
- Das markierte Dokument kann per Doppelklick geöffnet werden.

#### Sortierreihenfolge

Mit der Wahl der Option legen Sie fest, wie die Einträge in der Trefferliste im Register Tabelle sortiert werden sollen:

- Nach Auftragsnummer aufsteigend
- Nach Auftragsnummer absteigend
- Nach Erfassungsdatum aufsteigend
- Nach Erfassungsdatum absteigend

### Dokumente suchen – Detailübersicht

> Dokumente > Auftrag > Suche > Register Detailübersicht

*Abb. C-271 Dokument suchen - Detailübersicht*

In diesem Register wird eine Übersicht zu den Dokumentenpositionen des im Register Tabelle markierten Dokuments angezeigt.

### Dokumente kopieren

> Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Menü Funktionen > Gruppe Dokument > Dokumente kopieren

Der Dialog Dokumente kopieren und die zugehörigen Menüs können aus verschiedenen Dialogen geöffnet werden. Er kann dann bereits in den Modus Teillieferung, Reklamation oder Anzahlung geschaltet sein. Der Dialog wird in dieser Anleitung am Beispiel Auftrag beschrieben.
- ⇨ Tutorial, "Dokumente kopieren" auf Seite C-244

> **i**
> **Teillieferung, Reklamation, Anzahlung**
> Wenn Sie über das Menü Funktionen > Teillieferung, Reklamation oder Anzahlung wählen, werden die entsprechenden Felder im Dialog Dokumente kopieren automatisch freigeschaltet bzw. gesperrt.

In diesem Dialog finden Sie folgende Register:

- "Dokumente kopieren - Kopieren 1:1" auf Seite C-536
- "Dokumente kopieren - Kopieren positionsweise" auf Seite C-542
- "Dokumente kopieren – Weitere Optionen Zieldokument" auf Seite C-544
- "Dokumente kopieren - Optionen Quelldokument" auf Seite C-546
- "Dokumente kopieren - Texte/Anlagen" auf Seite C-547
- "Dokumente kopieren - Modellparameter" auf Seite C-548

#### Menüs

- "Menü Optionen" auf Seite C-532
- "Menü Übersichten" auf Seite C-534

#### Menü Optionen

> Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Menü Funktionen > Gruppe Dokument > Dokumente kopieren > Menü Optionen

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

> **i**
> **Aktivierte Optionen nach dem Öffnen des Dialogs**
> Bitte beachten Sie, dass geänderte Optionen erst beim nächsten Öffnen des Dialogs wirksam werden.
> Wenn durch eine aktivierte Option eine Prüfung gestartet wurde, kann sich das Öffnen eines Dokuments verzögern. Der Grad der Verzögerung hängt von der Leistungsfähigkeit des Rechners ab.
> Die folgenden Beschreibungen stellen die aktivierte Option dar.

##### Gruppe Allgemein

- **Liefertermin nach Touren suchen**: Der Liefertermin wird automatisch auf den nächstmöglichen Tourentag gesetzt.
- **EK-Preisberechnung immer durchführen**: Die EK-Preisberechnung wird immer durchgeführt, auch wenn im Bereich Ziel die Preisberechnung nicht aktiviert ist.
- **Anzahlungsrechnung mit Positionen**: In den Anzahlungsrechnungen werden die Auftragspositionen aufgeführt.
- **Teillieferungsnummernkreis ist vom AV-Bereich unabhängig**: Die Nummern für Teillieferscheine berücksichtigen nicht die Nummernkreise der AV-Bereiche. Die Nummern werden immer aus dem Nummernkreis <k.A.> genommen.
- **Reklamationsnummernkreis ist vom AV-Bereich unabhängig**: Die Nummern für Reklamationen berücksichtigen nicht die Nummernkreise der AV-Bereiche. Die Nummern werden immer aus dem Nummernkreis <k.A.> genommen.
- **Lagerkennzeichen löschen wenn Status >= Warenabgang**: Die Funktion ist nur freigeschaltet, wenn Sie in ein Dokument eine andere Datenbank kopieren. Die Lagerkennzeichen werden dann gelöscht, damit die Lagerdaten der Zieldatenbank nicht überschrieben werden.
- **Keine Anlieferpauschale bei Teillieferungen**: Bei Teillieferungen wird die Anlieferpauschale auch dann nicht berechnet, wenn das Kennzeichen für diesen Zuschlag in den Stammdaten gesetzt ist.
- **Reklamationsmenge ist die Positionsmenge**: Bei Reklamationen wird automatisch gesamte Positionsmenge vorgeschlagen.
- **Einstellung für Preisberechnung wieder herstellen**: Die Option EK-Preisberechnung immer durchführen wird beim Verlassen des Dialoges benutzerbezogen gespeichert. Wird der Dialog danach wieder geöffnet, wird die Option wieder hergestellt. Wenn diese Einstellung nicht aktiviert ist, wird die Option EK-Preisberechnung immer durchführen immer beim Öffnen des Dialoges deaktiviert.
- **Fachberater=Erfasser**: Im Auftrag wird im Feld Fachberater automatisch der Name des Mitarbeiters eingetragen, der sich in A+W Business angemeldet hat, bzw. der das Dokument erfasst.
- **Positionsreferenz beibehalten**: Die Referenzen aus dem Auftrag werden in den neuen Auftrag übernommen.
    - ⇨ "Kommission" auf Seite C-456
- **Produktprüfung durchführen**: Beim Kopieren jeder Position wird geprüft, ob das Hauptprodukt oder ein Stücklistenelement gesperrt oder gelöscht wurde. Wenn dies der Fall ist, wird eine entsprechende Meldung am Ende des Kopiervorgangs angezeigt.

##### Gruppe Übermengen bei Teillieferungen

- **Keine Aktion**: Versehentlich eingegebene Übermengen für eine Teillieferung erzeugen keine Meldung.
- **Meldung**: Wenn die Menge der Teillieferung größer als die Positionsmenge ist, wird eine Meldung angezeigt.
- **Nicht möglich**: Eine Übermenge kann nicht eingegeben werden.

##### Gruppe Teillieferungsmenge

- **Gestellrückmeldung bei Teillieferung berücksichtigen**: Die Gestellnummer wird bei Teillieferungen zurückgemeldet.
- **Wareneingangsmenge bei Teillieferung berücksichtigen**: Die Menge der Teillieferung wird mit der Menge des Wareneingangs vorbelegt.

##### Gruppe Anzahlungsbetrag

- **Anzahlungsbetrag**:
    - **Brutto**: Der Anzahlungsbetrag wird als Bruttobetrag eingegeben.
    - **Netto**: Der Anzahlungsbetrag wird als Nettobetrag eingegeben.
    - **Prozentual**: Der Anzahlungsbetrag wird als prozentualer Anteil der Auftragssumme eingegeben.

##### Gruppe Meldungen

- **Fehlermeldung Anlieferdatum unterdrücken**: Wenn der Liefertermin aus dem Quellauftrag im Zielauftrag nicht eingehalten werden kann, wird eine Fehlermeldung angezeigt. Diese Meldung können Sie ausschalten, z. B., wenn Sie den neuen Auftrag nach dem Kopieren bearbeiten.
- **Fehlermeldung Teillieferung unterdrücken**: Wenn für die Teillieferung nur ein Teil einer Position übernommen wird, wird eine entsprechende Meldung angezeigt. Diese kann ausgeschaltet werden, z. B., wenn Sie i. d. R. Teillieferungen mit Teilmengen erstellen.
- **Alle Fehlermeldungen und Prüfungen unterdrücken**: Wenn Sie diese Option aktivieren, werden alle Fehlermeldungen und Prüfungen ausgeschaltet.

#### Menü Übersichten

> Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Menü Funktionen > Gruppe Dokument > Dokumente kopieren > Menü Übersichten

Über dieses Menü können Sie sich Übersichten anzeigen lassen, ohne den Dialog zu schließen.

##### Gruppe Übersicht

- **Teillieferung**: Öffnet den Dialog Teillieferungsübersicht.
    - ⇨ "Teillieferungsübersicht" auf Seite C-558
- **Reklamation**: Öffnet den Dialog Reklamationsübersicht.
    - "Reklamationsübersicht" auf Seite C-560
- **Anzahlung**: Öffnet den Dialog Anzahlungsübersicht.
    - ⇨ "Anzahlungsübersicht" auf Seite C-561

##### Gruppe Anzeige

- **Quelldokument anzeigen**: Öffnet den Dialog Dokumentenansicht als Vorschau auf das Quelldokument.
- **Zieldokument anzeigen**: Öffnet den Dialog Dokumentenansicht als Vorschau auf das Dokument, das durch das Kopieren erstellt wurde.
    - ⇨ "Dokument anzeigen" auf Seite C-548

### Dokumente kopieren – Kopieren 1:1

> Dokumente > Auftrag > Auftrag > Menü Funktionen > Gruppe Dokument > Dokumente kopieren > Register Kopieren 1:1

*Abb. C-272 Dokumente kopieren – Kopieren 1:1*

In diesem Register legen Sie die Angaben für den Dokumentenkopf fest.

> **i**
> **Dokumentendaten ändern**
> Bitte beachten Sie, dass ein neues Dokument erstellt wird, wenn Sie die Eingaben speichern. Nachträgliche Änderungen können Sie dann nur im neuen Dokument eintragen.

#### Auswahl Bereiche

**Von, nach** Sie können Dokumente aus jedem Bereich im Feld von in jeden Bereich im Feld nach kopieren. Sie können auch Dokumente aus einem Archiv kopieren.

**Zielserver/-datenbank** Wenn Sie mit mehreren Datenbanken auf verschiedenen Servern arbeiten, können Sie eine andere Datenbank auswählen. Sprechen Sie mit Ihrem Ansprechpartner bei der A+W Software GmbH, wenn Sie zusätzliche Datenbanken auf anderen Servern nutzen wollen.

#### Modus

Mit der Wahl der Option bestimmen Sie, welchen Dokumententyp Sie erstellen wollen. Der Modus kann bereits aktiviert sein, wenn Sie im Dokument > Menü Funktionen den Eintrag Teillieferung, Anzahlung oder Reklamation gewählt haben.

- **Kopieren**: Schaltet alle Felder frei, die Sie zum Anlegen eines neuen Dokuments benötigen. Mit dieser Option können Sie auch alle Dokumente eines Nummernverwalters kopieren.
    - ⇨ Tutorial, "Dokumente kopieren" auf Seite C-244
- **Teillieferung**: Sperrt alle Felder, die unverändert aus dem Auftragskopf übernommen werden müssen.
    - ⇨ Tutorial, "Teillieferungen" auf Seite C-256
- **Reklamation**: Sperrt alle Felder, die unverändert aus dem Auftragskopf übernommen werden müssen, und schaltet den Bereich Reklamation frei.
    - ⇨Tutorial, "Reklamationen" auf Seite C-282
- **Anzahlung**: Sperrt alle Felder, die unverändert aus dem Auftragskopf übernommen werden müssen, und schaltet den Bereich Anzahlung frei.
    - ⇨ Tutorial, "Anzahlungen" auf Seite C-274

#### Quelle

Sie können ein einzelnes Dokument oder Dokumente eines Nummernverwalters kopieren.

**Nummer** Nummer und Auswahl eines einzelnen Dokuments. Nur wenn Sie den Modus Kopieren gewählt haben, können Sie ein Dokument aus einem anderen Nummernverwalter auswählen.

**Nummernverwalter** Name und Auswahl eines Nummernverwalters. Diese Option ist nur freigeschaltet, wenn Sie den Modus Kopieren oder Reklamation gewählt haben.
Mit dieser Option schalten Sie den Bereich Übersicht frei.

#### Reklamation

Reklamationen können nur für einzelne Dokumente erstellt werden. Die Felder in diesem Bereich sind nur freigeschaltet, wenn Sie den Modus Reklamation gewählt haben.

> **i**
> **Grund und Verursacher pro Position angeben**
> Sie können die Details für die reklamierten Positionen getrennt erfassen, z. B., wenn unterschiedliche Verursacher vorliegen.
> - ⇨ "Reklamation" auf Seite C-506

**Verursacher** Sie können den Verursacher auswählen. Diese Angabe kann zur Auswertung in der Statistik herangezogen werden. Angeboten werden alle Verursacher, die in den Stammdaten hinterlegt sind.
- ⇨ Stammdaten, "Reklamationsverursacher" auf Seite B-575

**Grund** Sie können den Reklamationsgrund auswählen. Diese Angabe kann zur Auswertung in der Statistik herangezogen werden. Angeboten werden alle Reklamationsgründe, die in den Stammdaten hinterlegt sind.
- ⇨ Stammdaten, "Reklamationsgrund" auf Seite B-576

**Kostenlos** Eine Reklamation kann wahlweise mit oder ohne Berechnung erstellt werden.
- Die Reklamation wird berechnet. So können Sie z. B. in der Reklamation andere Preise angeben als im Original-Auftrag, um eine vereinbarte Kulanz zu gewähren.
- Die Reklamation ist kostenlos. Mit der Ersatzlieferung erhält der Kunde keine neue Rechnung. In der Reklamationsstatistik werden der VK und der entgangene Erlös gegenübergestellt.

> **i**
> **Reklamation über Gutschrift**
> Sie können für die reklamierte Position eine Gutschrift ausstellen. Die Ersatzlieferung muss in diesem Fall berechnet werden.

#### Übersicht

Die Übersicht ist nur freigeschaltet, wenn Sie den Modus Kopieren und die Quelle Nummernverwalter gewählt haben. Die markierten Dokumente werden kopiert. Sie können mehrere Dokumente gleichzeitig markieren.

#### Anzahlung

Die Felder in diesem Bereich sind nur freigeschaltet, wenn der Modus Anzahlung gewählt ist.

> **i**
> **Voraussetzung**
> Die Anzahlung muss als Produkt mit der Produktart Leistungen/Zuschläge angelegt sein. Sie muss zusätzlich als automatischer Zuschlag in der Produktzuordnung Zuschläge zugewiesen sein.
> - ⇨ Stammdaten, "Produktverwaltung - Produkt" auf Seite B-591
> - ⇨ Stammdaten, "Produktzuordnung Zuschläge" auf Seite B-1029

**Brutto-, Nettobetrag, Prozentual** Der Anzahlung kann als Brutto- oder Nettobetrag eingetragen werden oder als prozentualer Anteil der Auftragssumme. Die Art der Angabe wird über das Menü Optionen ausgewählt.
- ⇨ "Gruppe Anzahlungsbetrag" auf Seite C-534

**Datum** Das aktuelle Tagesdatum wird vorbelegt. Sie können es ändern.

#### Archiv

Das Feld Quelle ist freigeschaltet, wenn Sie aus einem Archiv kopieren wollen. Sie können das jeweilige Archivjahr auswählen.

#### Änderung

**AV-Bereich** Wenn Sie mit AV-Bereichen arbeiten, wird der AV-Bereich angezeigt, der im Quell-Dokument angegeben ist.
- Der AV-Bereich wird aus dem Quelldokument übernommen. Die Kombobox ist gesperrt.
- Der AV-Bereich kann geändert werden. Die Kombobox ist freigeschaltet.
- ⇨ Stammdaten, "AV-Bereiche" auf Seite B-1019

**Dokumententyp** Die Felder sind nur freigeschaltet, wenn Sie den Modus Kopieren gewählt haben. Bei den anderen Modi ist der Dokumententyp bereits festgelegt.
- Der Dokumententyp wird aus dem Quelldokument oder dem Modus übernommen. Die Kombobox ist gesperrt.
- Der Dokumententyp kann geändert werden. Die Kombobox ist freigeschaltet.

**Geschäftsart** Mit der Geschäftsart legen Sie fest, wie der Umsatz statistisch gewertet werden soll.
- Die Geschäftsart wird aus dem Quelldokument übernommen. Die Kombobox ist gesperrt.
- Die Geschäftsart kann geändert werden. Die Kombobox ist freigeschaltet.
- ⇨ Stammdaten, "Geschäftsart" auf Seite B-888

**Mandant** Wenn Sie mit mehreren Mandanten arbeiten, können Sie auf diese Weise Auftragspositionen übernehmen. Unter Umständen müssen Sie zusätzlich eine andere Zieldatenbank auswählen.
- Der Mandant wird aus dem Quelldokument übernommen. Die Kombobox ist gesperrt.
- Der Mandant kann geändert werden. Die Kombobox ist freigeschaltet.

**Sperrkennzeichen** Die Felder sind nur freigeschaltet, wenn Sie den Modus Kopieren gewählt haben. Bei Teillieferungen wird es automatisch nach den Einstellungen in den Kundendaten bzw. im Auftrag gesetzt.
- Das Sperrkennzeichen wird aus dem Quelldokument übernommen. Die Kombobox ist gesperrt.
- Das Sperrkennzeichen kann geändert werden. Die Kombobox ist freigeschaltet.
- "Faktura" auf Seite C-426
- ⇨ Stammdaten, "Sperrstatus" auf Seite B-424
- ⇨ Stammdaten, "Sperrkennzeichen" auf Seite B-898

**Netto Preise** Die Felder sind nur freigeschaltet, wenn Sie den Modus Kopieren gewählt haben. Mit der Angabe legen Sie fest, ob im Druck die Rabatte ausgewiesen werden.
- Die Einstellung zur Preiseingabe wird aus dem Quelldokument übernommen. Die Optionen ja und nein sind gesperrt.
- Die Einstellung zur Preiseingabe kann geändert werden. Die Optionen ja und nein sind freigeschaltet.

**Status** Die Felder sind gesperrt, wenn Sie den Modus Anzahlung gewählt haben. Der Status wird automatisch auf Anzahlungsrechnung erstellt gesetzt.
- Der Status kann nicht geändert werden. Die Kombobox ist gesperrt.
- Der Status kann geändert werden. Die Kombobox ist freigeschaltet.

#### Ziel

Die Nummer eines neuen Dokuments wird beim Kopieren automatisch ermittelt.

> **i**
> **Kunde und Lieferant ändern**
> Im Register Weitere Optionen Zieldokument können Sie neben dem Kunden und dem Lieferanten auch eine andere Lieferanschrift eingeben.
>
> ⇨ Dokumente kopieren - Weitere Optionen Zieldokument

Die drei Optionen sind nur freigeschaltet, wenn Sie den Modus Kopieren gewählt haben.

- **Nummer automatisch ermitteln**: Das neue Dokument wird mit einer neuen Nummer erstellt. Diese Option ist im Modus Kopieren automatisch aktiviert.
- **Manuelle Vorgabe der Nummer**: Mit dieser Option können Sie die Positionen aus dem Quelldokument in ein Zieldokument kopieren. Das Eingabefeld wird freigeschaltet, in dem Sie die Nummer des Zieldokuments eintragen können.
- **Nummer aus Quelle übernehmen**: Diese Option ist nur freigeschaltet, wenn Sie ein Dokument aus einem Archiv oder einer anderen Datenbank kopieren. Sie können damit das archivierte Dokument aus dem Archiv zurückholen, um es ggf. zu bearbeiten.

**Ziel-Nummernverwalter** Der Nummernverwalter des Quelldokuments wird angezeigt. Sie können das neue Dokument in einen anderen Nummernverwalter stellen.

**Preisberechnung** Die Preisberechnung kann neu durchgeführt werden, damit die richtigen (kundenindividuellen) Preise ermittelt werden.
- Die Preisberechnung wird nicht erneut durchgeführt. Die berechneten Preise werden aus dem Quelldokument übernommen. Diese Einstellung sollten Sie wählen, wenn Sie eine Gutschrift erstellen, damit der identische Preis gutgeschrieben wird.
- Die Preise werden neu berechnet. Die Checkbox Vorgaben lösch. wird freigeschaltet. Für die Preisberechnung werden entweder die Standard-Preislisten oder die kundenindividuellen Preislisten herangezogen.

> **i**
> **Kundenindividuelle Preise**
> Die kundenindividuellen Preise aus dem Quelldokument werden auch dann in den neuen Auftrag übernommen, wenn Sie diesen für einen anderen Kunden erfassen.

**Vorgaben lösch.** Mit dieser Einstellung können Sie festlegen, ob manuelle Preisvorgaben gelöscht werden sollen.
- Bei der Neuberechnung der Preise bleiben manuelle Preisvorgaben erhalten.
- Die manuellen Preisvorgaben werden bei der Neuberechnung der Preise zurückgesetzt.

**Kundendaten aus Kundenstamm aktualisieren** Geänderte Kundendaten werden beim Kopieren nicht automatisch aktualisiert.
- Die Kundendaten werden nicht neu eingelesen. Wenn die Stammdaten des Kunden nach dem Quelldokument nicht bearbeitet wurden, kann die Checkbox deaktiviert bleiben.
- Die Kundendaten werden neu eingelesen. Wenn die Stammdaten des Kunden geändert wurden, sollten Sie diese Funktion aktivieren.

**Produktkennzeichen neu einlesen** Produktdaten werden beim Kopieren nicht automatisch neu eingelesen.
- Die Produktkennzeichen werden nicht neu eingelesen.
- Die Produktkennzeichen werden neu eingelesen. Diese Funktion sollen Sie dann aktivieren, wenn die Produktkennzeichen für die Kunden unterschiedlich gesetzt sind, z. B. die Beschaffungsart.

> **i**
> **Einstellungen bleiben erhalten**
> Die Einstellungen Preisberechnung, Kundendaten aktualisieren und Produktkennzeichen neu einlesen werden für die Modi Dokumente kopieren und Reklamationen getrennt gespeichert. Damit kann der Dialog im Modus Dokumente kopieren andere Einstellungen annehmen wie im Modus Reklamationen.

### Dokumente kopieren – Kopieren positionsweise

> Dokumente > Auftrag > Auftrag > Menü Funktionen > Gruppe Dokument > Dokumente kopieren > Register Positionsweise

*Abb. C-273 Dokumente kopieren – Positionsweise*

In diesem Register legen Sie fest, welche Positionen in das Zieldokument übernommen werden sollen.

> **i**
> **Dokumentendaten ändern**
> Bitte beachten Sie, dass ein neues Dokument erstellt wird, wenn Sie die Eingaben speichern. Nur im neuen Dokument können Sie die Daten bearbeiten.

#### Quelle

In diesem Bereich werden die Positionen des Quelldokuments angezeigt.
- ⇨ Tutorial, "Bedienelemente im Dokumentenkopf" auf Seite C-41

> **i**
> **Markierungszeichen**
> Nur die Positionen mit einem Markierungszeichen werden in das neue Dokument kopiert. Die Menge kann dabei geändert werden.

**Dokument** Dokumentennummer des Dokuments, aus dem Positionen kopiert werden.

**Pos.** Anzahl der Positionen.
In der Übersicht werden alle Positionen des Quelldokuments aufgelistet.

#### Ziel

Die Positionen werden erst angezeigt, wenn die Kopie erstellt ist.

**Pos. (1:1)** Sie können die Positionsnummern unverändert in das neue Dokument übernehmen, z. B. in Teillieferungen mit Teilmengen einer Position.
- Die Positionsnummern werden nicht übernommen. Im neuen Dokument werden die übernommenen Positionen neu durchnummeriert.
- Die Positionsnummern werden übernommen.

**Dokument** Die neue Dokumentennummer wird angezeigt, wenn das Dokument erstellt wurde.

**Pos.** Die Anzahl der Positionen im neuen Dokument wird angezeigt, wenn das Dokument erstellt wurde.

### Dokumente kopieren – Weitere Optionen Zieldokument

> Dokumente > Auftrag > Auftrag > Menü Funktionen > Gruppe Dokument > Dokumente kopieren > Register Weitere Optionen Zieldokument

*Abb. C-274 Dokumente kopieren - Weitere Optionen Zieldokument*

In diesem Register legen Sie die Termine und die Lieferanschrift für das neue Dokument fest. Das Register ist nur freigeschaltet, wenn Sie im Register Kopieren 1:1 die Option Nummer automatisch ermitteln gewählt haben.

#### Termine

Die Felder in diesem Bereich sind ausführlich zu den Kopfdaten der Dokumente beschrieben.
- ⇨ "Kopfdaten - Dokument" auf Seite C-418

#### Abweichender

Einen abweichenden Lieferanten müssen Sie unter Umständen dann angeben, wenn das Zieldokument eine Bestellung ist.

**Kunde, Lieferant** Sie können einen anderen Kunden und einen anderen Lieferanten für das neue Dokument angeben.
Bei Bestellungen betreffen diese Felder den Lieferanten und Unterlieferanten.

#### Lieferanschrift

Sie können eine Lieferanschrift angeben. Wenn Sie diese Felder leer lassen, wird der Auftrag an die Kundenanschrift ausgeliefert.

Über die Pfeilschaltflächen können Sie als Lieferanschrift eine der Kundenadressen übernehmen, die Sie in der Tabelle markiert haben.

#### Tabelle

Wenn es zu dem gewählten Kunden oder Lieferanten eine abweichende Lieferanschrift hinterlegt ist, wird diese angezeigt. Wenn nur eine Lieferanschrift angegeben ist, werden die Daten automatisch in den Bereich Lieferanschrift übernommen. Sie können geändert werden.

### Dokumente kopieren – Optionen Quelldokument

> Dokumente > Auftrag > Auftrag > Menü Funktionen > Gruppe Dokument > Dokumente kopieren > Register Optionen Quelldokument

*Abb. C-275 Dokumente kopieren – Optionen Quelldokument*

In diesem Register können Sie folgende Daten festlegen:
- Bei einer Teillieferung den Liefertermin.
- Bei einem Angebot die Kategorie.

#### Termine

**Versandtag des Original-Auftrags bei Teillieferungen ändern** Für den Original-Auftrag können Sie ein neues Datum für die restliche Lieferung festlegen.
- **Datum**: Für die Restlieferung geben Sie ein festes Datum an.
- **Automatisch um**: Das Lieferdatum wird automatisch im Original-Auftrag um die Anzahl der eingetragenen Tage hochgerechnet.
- **Nächster Versandtag**: Als Lieferdatum wird automatisch der nächstfolgende Versandtag eingetragen.

#### Änderungen

**Kategorie** Durch die Kategorie kann ein Angebot nach verschiedenen Ablehnungsgründen klassifiziert werden, z. B. zu teuer, keine Rückmeldung. Über die Kategorie können Angebote in der Statistik ausgewertet werden.

### Dokumente kopieren - Texte/Anlagen

> Dokumente > Auftrag > Auftrag > Menü Funktionen > Gruppe Dokument > Dokumente kopieren > Register Texte/Anlagen

*Abb. C-276 Dokumente kopieren – Texte/Anlagen*

In diesem Register können Sie einen Text für das Zieldokument hinzufügen oder eine Datei als Anhang hinzufügen.

Die Felder sind ausführlich zu den Kopfdaten der Dokumente beschrieben.
- ⇨ "Kopfdaten - Anlagen" auf Seite C-435

Sie können einen Ihrer, in den Stammdaten eingetragenen, Texte auswählen oder einen neuen erfassen. Sie können bestimmen, ob der Text als Kopf- oder Fußtext erscheinen soll.

### Dokumente kopieren – Modellparameter

> Dokumente > Auftrag > Auftrag auswählen > Menü Funktionen > Gruppe Dokument > Dokumente kopieren > Register Modellparameter

In diesem Register können Sie die Parameter für Modelle prüfen.

### Dokument anzeigen

> Dokumente > Auftrag > Auftrag auswählen > Menü Ansicht > Gruppe Dokument > Dokument anzeigen

*Abb. C-277 Dokument anzeigen*

In diesem Dialog wird eine Kurzübersicht zu allen im Dokument enthaltenen Positionen angezeigt.

> **i**
> **Angezeigtes Dokument drucken**
> Sie können die angezeigten Dokumente drucken. Dieser Druck unterscheidet sich vom Formulardruck. Nur im Formulardruck wird der Status des Dokuments hochgesetzt.
>
> ⇨ "Formular-/Etikettendruck" auf Seite C-640

### Kundeninfo

> Dokumente > Auftrag > Auftrag auswählen > Menü Ansicht > Gruppe Dokument > Kundeninfo

*Abb. C-278 Kundeninfo*

In diesem Dialog werden allgemeine Informationen zum aktuellen Kunden und zu den angehängten Anlagen angezeigt, die für den Kunden gelten. Die Angaben werden aus den Stammdaten übernommen.
- ⇨ Stammdaten, "Spezifikation" auf Seite B-763

Diese Informationen können Sie auch von der Positionserfassung aus abrufen.

In der Dokumentenverwaltung können Sie diese Informationen auch im Register Kundeninfo abrufen.
- ⇨ "Kopfdaten - Kundeninfo" auf Seite C-438

Der Dialog wird automatisch angezeigt, wenn die Option in den Kundenstammdaten aktiviert ist.

### Kapazitätsübersicht

> Dokumente > Auftrag > Auftrag auswählen > Menü Ansicht > Gruppe Kapazitätsübersicht > Kapazitätsübersicht

*Abb. C-279 Kapazitätsübersicht*

In diesem Dialog werden die freien Kapazitäten und belegten Zeiten, der Status und der Fortschritt der Produktion aus A+W Production Capacity Planner angezeigt.

Dieser Dialog wird nur angezeigt, wenn Sie mit A+W Production Capacity Planner und A+W Capa View arbeiten. Ausführliche Informationen zu den Dialogen der Kapazitätsübersicht finden Sie in der Dokumentation für A+W Capa View.

**[Schichten]** Die Übersicht wird nach Schichten angezeigt.

**[Tage]** Die Übersicht wird nach Tagen angezeigt.

**[Maschinen]** Die Belegung einer bestimmten Maschine wird angezeigt. Die Maschine wählen Sie in der Kombobox aus, in der die zur Verfügung stehenden Maschinen angezeigt werden.

**[Gruppen]** Die Belegung einer bestimmten Maschinengruppe wird angezeigt. Die Maschinengruppe wählen Sie in der Kombobox aus, in der die zur Verfügung stehenden Maschinengruppen angezeigt werden.

**(Kombobox)** Auswahl der Maschine oder Maschinengruppe. Die definierten Maschinen und Maschinengruppen werden zur Auswahl angeboten.

**Startdatum** Angabe des Datums, ab dem die Kapazitätsübersicht angezeigt werden soll. Sie können das Datum manuell eintragen oder über die Schaltfläche [Kalender] auswählen.

**[7 Tage], [10 Tage], [14 Tage]** Die Belegung der Maschine oder Maschinengruppe wird über einen Zeitraum von 7, 10 oder 14 Tagen angezeigt.

**[Pfeil links]** Das Startdatum wird um den angegebenen Zeitraum zurückgestellt. Die Kapazitätsübersicht wird aktualisiert.

**[Pfeil rechts]** Das Startdatum wird um den angegebenen Zeitraum vorgestellt. Die Kapazitätsübersicht wird aktualisiert.

> **i**
> **Ansicht wechseln**
> Sie können in die Detailansicht der Kapazitätsübersicht wechseln, wenn Sie in der Kapazitätsanzeige auf einen der Balken klicken. Sie können die Detailansicht wieder schließen, wenn Sie auf die Schaltfläche [x] in der linken oberen Ecke klicken.

#### Detailansicht

*Abb. C-280 Kapazitätsübersicht – Detailansicht*

In der Detailansicht der Kapazitätsübersicht werden die ausgewählten Daten nach Auftrag oder Lauf angezeigt.

Im oberen Teil des Dialogs werden die ausgewählten Daten nach Zeit, Fläche und Stück angezeigt.

Sie können wählen, wie die Daten im unteren Teil des Dialogs angezeigt werden:

**[Lauf]** Die Übersicht wird pro Produktionslauf angezeigt. Sie kann summiert nach Zeit, Stück oder Menge angezeigt werden.

**[Auftrag]** Die Übersicht wird pro Auftrag angezeigt. Sie kann summiert nach Zeit, Stück oder Menge angezeigt werden.

**[Zeit]** Die Übersicht wird pro Auftrag oder Lauf summiert nach Zeit angezeigt.

**[Stück]** Die Übersicht wird pro Auftrag oder Lauf summiert nach der Stückzahl angezeigt.

**[Menge]** Die Übersicht wird pro Auftrag oder Lauf summiert nach der Fläche angezeigt.

### Historie

> Dokumente > Auftrag > Auftrag auswählen > Menü Funktionen > Gruppe Dokument > Historie

*Abb. C-281 Historie*

In diesem Dialog können Sie zurückverfolgen, wie mit dem Dokument gearbeitet wurde. Die Anzeige wird aktualisiert, wenn das aktuelle Dokument geschlossen wird.

Im oberen Bereich werden die Dokumentenart, die Nummer und der Status des aktuellen Dokuments angezeigt.
- ⇨ Tutorial, "Dokumenten-Historie" auf Seite C-217

#### Übersicht

**Datum / Uhrzeit** Datum und Uhrzeit der Bearbeitung.

**Vorgang / Aktion** Art der Bearbeitung.

**Status** Status, der durch die Bearbeitung erzeugt wurde.

> **i**
> **Automatische Statusänderungen**
> Bei den automatischen Statusänderungen kann das Dokument immer nur auf einen höheren Status gesetzt werden. Nur durch manuelle Änderungen kann der Status zurückgesetzt werden.

**Bearbeiter** Name des Mitarbeiters, der sich in A+W Business angemeldet und das Dokument bearbeitet hat.

**Referenz** Nummer des referenzierten Dokuments:
- Das referenzierte Dokument wurde aus dem aktuellen Dokument erzeugt, z. B. Lieferscheinnummer.
- Das aktuelle Dokument wurde aus dem referenzierten erzeugt, z. B. Auftragsnummer bei einer Bestellung.

**Bemerkung** Details zur inhaltlichen Änderung, z. B. Preisänderung.

**Letzte Aktion zuerst anzeigen** Sie können die Reihenfolge der angezeigten Einträge sortieren. Diese Einstellung wird pro Dokumentenart gespeichert.
- Die erste Aktion wird zuerst angezeigt.
- Die letzte Aktion wird zuerst angezeigt.

### Statusänderung

> Dokumente > Auftrag > Auftrag auswählen > Menü Funktionen > Gruppe Dokument > Statusänderung

*Abb. C-282 Status ändern*

Statusänderungen können für einen einzelnen Auftrag, für mehrere ausgewählte Aufträge oder für alle Aufträge in einem Nummernverwalter durchgeführt werden. Eine Änderung pro Nummernverwalter kann z. B. notwendig sein, wenn Rechnungen in einem falschen Nummernkreis gedruckt wurden.
- ⇨ Tutorial, "Dokument vollständig kopieren" auf Seite C-248

> **i**
> **Änderung für einen gesamten Nummernverwalter**
> Prüfen Sie vor der Änderung des Status aller Dokumente in einem Nummernverwalter, ob tatsächlich nur die zu ändernden Dokumente in diesem Nummernverwalter aufgeführt werden.

#### Modus

Mit der Wahl der Option legen Sie fest, ob ein einzelnes oder mehrere Dokumente geändert werden sollen:

- **Nummernverwalter**: Der Status aller Dokumente eines Nummernverwalters wird geändert. Die Kombobox zur Auswahl eines Nummernverwalters wird freigeschaltet.
- **Selektion**: Nur im Nummernverwalter. Der Status der markierten Dokumente wird geändert. Die Mehrfachauswahl mit der <Strg>-Taste ist möglich.
- **Nummer**: Der Status eines bestimmten Dokuments wird geändert. Im Bereich Dokument wird das Feld Nummer freigeschaltet.

#### Dokument

**Nummer** Nummer des Dokuments, dessen Status geändert werden soll. Das Feld ist nur freigeschaltet, wenn die Option Nummer aktiviert wurde.

**Name** Name des Kunden, dessen Dokument geändert werden soll.

**Straße, Ort** Anschrift aus dem Dokument, das geändert werden soll.

**Nummernverwalter füllen** Wenn Sie den Status eines einzelnen Dokuments ändern, können Sie das Dokument gleichzeitig an den zugehörigen Nummernverwalter übergeben.
Die Checkbox ist nur freigeschaltet, wenn die Option Nummer aktiviert ist.
- Das Dokument wird nicht an einen Nummernverwalter übergeben.
- Das Dokument wird seinem neuen Status entsprechend an einen Nummernverwalter übergeben.

#### Status

**Alt** Anzeige des Status, der geändert wird. Das Feld wird nur gefüllt, wenn die Option Nummer aktiviert wurde.

**Neu** Kombobox zur Auswahl des neuen Status.

### NV Auswahl

> Dokumente > Auftrag > Auftrag auswählen > Menü Funktionen > Gruppe Dokument > NV Auswahl

*Abb. C-283 NV Auswahl*

In diesem Dialog können Sie den Nummernverwalter für das aktuelle Dokument ändern.
- ⇨ Tutorial, "Nummernverwalter" auf Seite C-180
- ⇨ "Nummernverwalter" auf Seite C-629

**Aktueller Nummernverwalter** Auswahl des Nummernverwalters, auf den die Dokumentenverwaltung zugreifen soll.
Wenn Sie einen neuen Namen eingeben, wird ein neuer Nummernverwalter mit diesem Namen angelegt. Beachten Sie dabei, dass das aktuelle Dokument automatisch in diesen neuen Nummernverwalter gestellt wird.

**Löschen** Der aktuelle Nummernverwalter kann geleert werden.
- Der angezeigte Nummernverwalter wird nicht geleert.
- Der angezeigte Nummernverwalter wird geleert und enthält dann nur noch das aktuelle Dokument.
- ⇨ Tutorial, "Nummernverwalter leeren" auf Seite C-187

### Lagermaße in Kisten verpacken

> Dokumente > Auftrag > Auftrag auswählen > Menü Funktionen > Gruppe Dokument > Lagermaße in Kisten verpacken

*Abb. C-284 Lagermaße in Kisten verpacken*

In diesem Dialog können Sie die Positionen aus fertig gemeldeten Produktionsaufträgen in Kisten verpacken.

> **i**
> **Voraussetzungen**
> Die Kisten müssen als Lagermaße mit dem jeweiligen Inhalt angelegt sein. Die Identnummer für die Kistenbuchung im Lagerbestand können nur automatisch vergeben werden, wenn die entsprechende Option in der Lagerverwaltung eingeschaltet ist.
> Informationen zu diesen Voraussetzungen finden Sie in der Parts Stammdaten und Lagerwirtschaft.

Die Funktion ist nur für Produktionsaufträge mit Lagermaßen freigeschaltet.

In der oberen Tabelle werden die Positionen mit den Lagermaßen angezeigt. In der unteren Tabelle werden Vorschläge für die Verpackung in Kisten und deren Inhalt angezeigt.

Diese Vorschläge können geändert werden, indem Sie in der oberen Tabelle die Anzahl der Kisten oder deren Inhalt ändern. Das System berechnet die Kisten dann neu und zeigt das neue Resultat in der unteren Tabelle an.

Nach dem Bestätigen werden die Lagermaße vom Lager abgebucht und die Kisten angelegt. Danach können die Etiketten für die erzeugten Kisten gedruckt werden.

#### Übersicht - obere Tabelle

- **Pos.**: Nummer der Auftragsposition mit Lagermaßen.
- **Produkt**: Produkt, zu dem Lagermaße angelegt sind.
- **Bereit, Höhe**: Maße der Scheiben.
- **Anzahl Scheiben**: Anzahl der Scheiben in der Auftragsposition.
- **Anzahl Kisten**: Anzahl der Kisten, die aus den definierten Lagermaßen zu Kisten resultieren. Der Wert kann geändert werden.
- **Kisteninhalt**: Inhalt der Kiste. Der Wert kann geändert werden.

#### Übersicht - untere Tabelle

- **Pos.**: Nummer der Auftragsposition, zu der die Kiste erzeugt wird.
- **Produkt**: Produkt, zu dem Lagermaße angelegt sind.
- **Bereit, Höhe**: Maße der Scheiben.
- **Identnummer**: Identnummer, mit der die Kiste im Lagerbestand verbucht wird.
- **Inhalt**: Berechneter Inhalt der Kiste.

### Teillieferungsübersicht

> Dokumente > Auftrag > Auftrag auswählen > Menü Funktionen > Gruppe Dokumentenübersicht > Teillieferung

*Abb. C-285 Teillieferungsübersicht*

In diesem Dialog werden die Teillieferungen zum aktuellen Auftrag aufgelistet.
- ⇨ Tutorial, "Teillieferungen" auf Seite C-256

In der ersten Zeile ist der Original-Auftrag in roter Schrift angezeigt. Darunter werden die Teillieferungen aufgeführt.

Die Mengen geben die Summen der Stückzahlen aller Auftragspositionen wieder, z. B. kann die Menge 15 die Summe aus 3 Positionen zu je 5 Stück sein. Wenn Sie die Teillieferungspositionen löschen lassen, verringern sich die angezeigten Mengen des Original-Auftrags mit jeder Teillieferung.

Der Betrag bezeichnet den Auftragswert. Nur bei Teillieferungen mit Teilfaktura wird ein Betrag für die Teillieferung angezeigt. In diesem Fall wird der Betrag des Original-Auftrags um den Betrag der Teillieferung(en) vermindert.
- ⇨ Stammdaten, "Teillieferungsposition nicht löschen" auf Seite B-937
- ⇨ Stammdaten, "Teillieferungsdatum von Originalauftrag übernehmen" auf Seite B-937

#### Tabelle

Die angezeigten Werte beziehen sich immer auf die Zeile, die in der Übersicht markiert ist.

**Pos.** Nummer der Auftragsposition. Wenn teilgelieferte Positionen aus dem Auftrag gelöscht wurden, fehlen die entsprechenden Positionsnummern bei der Anzeige des Original-Auftrags.
- ⇨ Stammdaten, "Teillieferungsposition nicht löschen" auf Seite B-937

**Produkt** Produktbezeichnung der Position.

**Orig. Menge** Die Originalmenge bezeichnet die Menge des markierten Original-Auftrags oder der markierten Teillieferung.

**Teilgelief. Menge** Die teilgelieferte Menge bezeichnet die Menge, die aus der Position teilgeliefert wurde. In einer Teillieferung wird i. d. R. der Wert Null angezeigt. Für den Original-Auftrag ist dies die Summe aller Teillieferungen der Position.

**Pos. Menge** Für den Original-Auftrag und die Teillieferung ist dies die Menge, die fakturiert wird. Für die Teillieferung ohne Teilfaktura wird zu dieser Menge der Betrag Null angezeigt.

**Betrag** Für den Original-Auftrag sind dies die Beträge der einzelnen Positionen, die fakturiert werden. Bei Teillieferungen mit Teilfaktura werden die Beträge im Original-Auftrag um die bereits fakturierten Beträge reduziert.
Für die Teillieferung mit Teilfaktura sind dies die Beträge der einzelnen Positionen, die fakturiert werden. Für die Teillieferung ohne Teilfaktura werden keine Beträge angezeigt.
- ⇨ "Teillieferung, Teilfaktura, Sammelrechnung" auf Seite C-427

### Reklamationsübersicht

> Dokumente > Auftrag > Auftrag auswählen > Menü Funktionen > Gruppe Dokumentenübersicht > Reklamation

*Abb. C-286 Reklamationsübersicht*

In diesem Dialog werden die Reklamationen zum aktuellen Auftrag aufgelistet.

In der ersten Zeile sind in roter Schrift die Auftragsnummer und der Kundenname des Original-Auftrags angezeigt.

Darunter sind die Reklamationen aufgelistet, die zu diesem Auftrag erstellt wurden.

In der Tabelle werden Details zu dem Eintrag angezeigt, der im oberen Bereich markiert ist.
- ⇨Tutorial, "Reklamationen" auf Seite C-282

### Anzahlungsübersicht

> Dokumente > Auftrag > Auftrag auswählen > Menü Funktionen > Gruppe Dokumentenübersicht > Anzahlungen

*Abb. C-287 Anzahlungsübersicht*

In diesem Dialog werden die Anzahlungen zum aktuellen Auftrag aufgelistet.

In der ersten Zeile sind Auftragsnummer und Kundenname des Original-Auftrags in roter Schrift angezeigt.

In der Tabelle werden Details zu den erfassten Anzahlungen angezeigt.
- ⇨Tutorial, "Anzahlungen" auf Seite C-274

### Auftrags-/Bestell-Info

> Dokumente > Auftrag > Auftrag auswählen > Menü Funktionen > Gruppe Info > Auftrags-/Bestell-Info

*Abb. C-288 Auftrags-/Bestell-Info*

In diesem Dialog werden die Bestellungen zum aktuellen Auftrag aufgelistet.

#### Modus

Die Option ist automatisch gewählt und richtet sich danach, ob Sie den Dialog aus einem Auftrag oder einer Bestellung heraus geöffnet haben. Mit der Option ist festgelegt, welche Daten angezeigt werden:

- **Auftrag**: Bestellungen zum ausgewählten Auftrag.
- **Bestellung**: Aufträge zur ausgewählten Bestellung.

#### Auswahl

**Dokument-Nr.** Nummer des Dokuments, zu dem die Bestellungen bzw. ein Auftrag angezeigt werden.

**Name / Ort** Name und Sitz des Kunden bzw. Lieferanten, zu dem Dokumente angezeigt werden.

#### Tabelle

In der Tabelle werden je nach der gewählten Option die Aufträge zu einer Bestellung oder alle Bestellungen zu einem Auftrag angezeigt.

- **Pos.**: Positionsnummer aus dem Auftrag.
- **Best.Nr./Auftr.Nr.**: Nummer der Bestellung bzw. des Auftrags.
- **Best.Pos./Auftr.Pos.**: Positionsnummer in der Bestellung bzw. im Auftrag.
- **Menge**: Bestellte Menge aus dem Auftrag.
- **geliefert**: Bereits gelieferte Menge nach Rückmeldung aus dem verbuchten Wareneingang.
- **Breit, Höhe**: Maße des bestellten Glases aus dem Auftrag.
- **Bezeichnung**: Produktbezeichnung aus den Stammdaten.
- **Preis**: In der Auftragsinfo ist dies der VK, in der Bestellinfo der EK.
- **Liefertermin**: Liefertermin aus dem Auftrag.
- **AB-Lieferant**: Datum der Auftragsbestätigung durch den Lieferanten.
- **Rechnung**: Nummer der Rechnung des Lieferanten.
- **Lieferant, Kunde**: Name des Lieferanten, an den die Bestellung gesendet wurde, bzw. des Kunden, aus dessen Auftrag die Bestellung erzeugt wurde.

**[Anzeigen]** Öffnet den Dialog Dokumentenansicht als Vorschau auf das Dokument.
- ⇨ "Dokument anzeigen" auf Seite C-548

### Duplikate

> Dokumente > Auftrag > Auftrag auswählen > Menü Funktionen > Gruppe Info > Duplikate anzeigen

*Abb. C-289 Duplikate anzeigen*

In diesem Dialog werden die Aufträge und Auftragspositionen aufgelistet, die mit dem aktuellen Auftrag und den Positionen identisch sind. An erster Stelle wird das aktuelle Dokument angezeigt, darunter werden die Duplikate aufgelistet.

> **i**
> **Voraussetzung**
> Damit Sie Duplikate anzeigen lassen können, müssen Sie im Modul Utilities festlegen, welche Daten verglichen werden sollen und welcher Zeitraum überwacht werden soll. Für den Zeitraum muss mindestens 1 Tag eingetragen sein.
>
> Das aktuelle Dokument wird z. B. auf identische Aufträge geprüft, die innerhalb eines bestimmten Zeitraums angefertigt wurden. Im Modul Utilities stellen Sie die Filter für die Suche ein.
>
> ⇨ Tutorial, "Dokumentenüberwachung" auf Seite C-386

### Kundenbenachrichtigung (Lieferterminkontrolle)

> Dokumente > Auftrag > Auftrag auswählen > Menü Funktionen > Gruppe Kapazitäten > Lieferterminkontrolle

Diesen Dialog können Sie auch unabhängig von einem Dokument öffnen über
> Dokumente > Kundenbenachrichtigung.

Über diesen Dialog können Sie Aufträge auswählen, deren Liefertermin verschoben werden musste und zu dem Sie den Kunden benachrichtigen wollen.

> **i**
> **Voraussetzungen**
> Folgende Voraussetzungen müssen erfüllt sein, damit die Kundenbenachrichtigungen automatisch versendet werden können:
>
> - Faxnummer und/oder E-Mail-Adresse in den Kundendaten.
> - Standardtexte für die Kundenbenachrichtigung.
> - Statuspunkte 560 und 900 müssen angelegt und zugeordnet sein.

In diesem Dialog finden Sie folgende Register:

- “Kundenbenachrichtigung – Auswahl" auf Seite C-566
- “Kundenbenachrichtigung – Terminverschiebung" auf Seite C-568

#### Menüs

- "Menü Funktionen" auf Seite C-565
- "Menü Opionen" auf Seite C-565

#### Menü Funktionen

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Dialog Kundenbenachrichtigung zu schließen.

- **Einstellungen**: Öffnet den Dialog Einstellungen für Kundenbenachrichtigungen, um Details für den Versand festzulegen.
    - ⇨ “Einstellungen für Kundenbenachrichtigungen" auf Seite C-569
- **Historie**: Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des markierten Dokuments.
    - ⇨ "Historie" auf Seite C-552
- **Dokument anzeigen**: Öffnet den Dialog Dokumentenansicht als Vorschau auf das Dokument.
    - ⇨ "Dokument anzeigen" auf Seite C-548

#### Menü Opionen

Berechnet den Versandtag zu einem neuen Anliefertermin. Der Anliefertermin und der Versandtag werden in den Auftragskopf zurückgeschrieben.

### Kundenbenachrichtigung – Auswahl

> Dokumente > Auftrag > Auftrag auswählen > Menü Funktionen > Gruppe Kapazitäten > Lieferterminkontrolle > Register Auswahl
> Dokumente > Kundenbenachrichtigung > Register Auswahl

*Abb. C-290 Kundenbenachrichtigung – Auswahl*

In diesem Register können Sie die Dokumente suchen und die Liefertermine prüfen. Angezeigt werden auch Aufträge/Bestellungen, für die erst teilweise Wareneingänge gebucht wurden.
- ⇨Tutorial, "Lieferterminkontrolle" auf Seite C-320

#### Modus

Mit der Wahl der Option legen Sie fest, welchen Dokumententyp Sie prüfen wollen:

- **Aufträge**: Aufträge mit offenen Lieferterminen werden angezeigt.
- **Bestellungen**: Bestellungen mit offenen Lieferterminen werden angezeigt.

#### Auswahl

Mit der Wahl der Option legen Sie fest, nach welchen Kriterien Sie Dokumententyp suchen.

- **Nummernverwalter**: Der Nummernverwalter für Aufträge oder Bestellungen kann ausgewählt werden.
- **Alle bis Status**: Der Höchst-Status für Aufträge oder Bestellungen kann ausgewählt werden.

#### Einschränkungen

**Lieferdatum bis** Sie können die Suche auf ein Lieferdatum einschränken.
- Die Suche wird nicht weiter eingeschränkt.
- Das Feld für das Lieferdatum wird freigeschaltet, auf das Sie die Suche einschränken wollen.

**Alle auf 1. Register anzeigen** Sie können die Anzeige der Trefferliste wechseln. Diese Einstellung können Sie nutzen, um Aufträge auszudrucken, die nicht verschoben wurden oder um bereits gedruckte Aufträge nochmals zu drucken.
- Im 1. Register werden die Kunden angezeigt, die benachrichtigt werden müssen. Im 2. Register werden alle Dokumente angezeigt, die den Auswahlkriterien entsprechen.
- Die Trefferliste wird vollständig im 1. Register angezeigt.

#### Übersicht

In der Übersicht werden alle Kunden aufgelistet, die benachrichtigt werden müssen.

Ein Symbol im Zeilenkopf zeigt an, dass der Kunde benachrichtigt werden muss oder bereits einmal benachrichtigt wurde.

### Kundenbenachrichtigung – Terminverschiebung

> Dokumente > Auftrag > Auftrag auswählen > Menü Funktionen > Gruppe Dokumente > Lieferterminkontrolle > Register Terminverschiebung
> Dokumente > Kundenbenachrichtigung > Register Terminverschiebung

*Abb. C-291 Kundenbenachrichtigung – Terminverschiebung*

In diesem Register werden alle Dokumente aufgelistet, die den Auswahlkriterien entsprechen. Sie können die Liefertermine prüfen und ggf. ändern und den Kunden über die Änderung benachrichtigen.

**Neuer Anliefertermin bei Kunde** Der aktuelle Liefertermin beim Kunden wird für den markierten Auftrag angezeigt. Sie können mehrere Aufträge markieren und für alle dasselbe neue Lieferdatum angeben.

> **i**
> **Terminänderung an den Kunden senden**
> Mitteilungen zu Terminänderungen können Sie über das Menü Drucken erstellen und an den Kunden senden.

**Tour** Die aktuelle Tour für den markierten Auftrag wird angezeigt. Sie können ggf. eine andere Tour auswählen. Sie können mehrere Aufträge markieren und für alle dieselbe neue Tour angeben.

### Einstellungen für Kundenbenachrichtigungen

> Dokumente > Kundenbenachrichtigung > Menü Funktionen > Einstellungen

*Abb. C-292 Kundenbenachrichtigung – Auswahl*

In diesem Dialog legen Sie Details für den Versand von Kundenbenachrichtigungen fest. Die Einstellungen gelten jeweils für alle markierten Dokumente, zu denen im Dialog Kundenbenachrichtigung der Druck gestartet wird.

#### Drucker und Formulare

In diesem Bereich legen Sie pro Versandart fest, welcher Drucker und welches Formular verwendet werden soll.

#### Texte für Benachrichtigungen

In diesem Bereich legen Sie fest, welche Standardtexte in das Formular geschrieben werden sollen. Die Einstellungen gelten jeweils pro Textkennzeichen.

**Textkennzeichen** Das Textkennzeichen schränkt die Auswahl der Standardtexte ein. Wenn Sie ein Textkennzeichen für die Kundenbenachrichtigungen verwendet haben, wählen Sie dieses Kennzeichen aus.

**1. Verschiebung** Standardtext für die erste Terminverschiebung.

**Weitere Verschiebungen** Standardtext für alle weiteren Terminverschiebungen.

**E-Mail-Betreff** Standardtext für die Betreffzeile der E-Mail-Benachrichtigung.

**E-Mail-Text** Standardtext für die E-Mail-Benachrichtigung.

#### Priorität für den Versand

In diesem Bereich legen Sie fest, welche Versandart vorrangig gewählt werden soll. Mit den Pfeilschaltflächen können Sie den markierten Eintrag nach oben oder nach unten verschieben.

#### Registerwechsel

**Nach Selektion auf Register 2 wechseln** Im Dialog Kundenbenachrichtigung wird die Trefferliste standardmäßig im zweiten Register angezeigt.
- Nach der Suche müssen Sie manuell in das Register Terminverschiebung wechseln. Diese Einstellung ist sinnvoll, wenn Sie sich die Trefferliste im Register Auswahl anzeigen lassen.
- Nach der Suche wird automatisch das Register Terminverschiebung angezeigt.

### Kapazitätsinfo nach Kunde

> Dokumente > Auftrag > Auftrag auswählen > Menü Funktionen > Gruppe Kapazitäten > Kapazitätsinfo nach Kunde

*Abb. C-293 Kapazitätsinformationssystem*

In diesem Dialog lassen Sie anzeigen, wie viel der reservierten Kapazitäten verplant ist.
- ⇨ Stammdaten, "Partnerverwaltung - Produktion" auf Seite B-785
- ⇨ Stammdaten, "Flächenkapazitäten" auf Seite B-982

> **i**
> **Kapazitäten sind nicht eingelastet**
> Die Anzeige gibt keine Auskunft über die aktuelle Kapazitätsplanung. Um die Auslastung der Maschinen/Produktion zu prüfen, müssen Sie das Modul Kapazitätsplanung starten.

#### Auflösung nach

**Isolierglas, VSG, ESG** Die Anzeige der reservierten Flächen kann für die jeweilige Produktart insgesamt ein oder ausgeblendet werden.
- Die Reservierungen für die Produktart werden nicht angezeigt.
- Die Reservierungen für die Produktart werden angezeigt.

#### Auswahl

**Nur Key-Kunden** Die Anzeige der reservierten Flächen für alle restlichen Kunden insgesamt kann ein oder ausgeblendet werden.
- Alle reservierten Flächen werden angezeigt.
- Nur die reservierten Flächen für die Key-Kunden werden angezeigt.

**Versandtag** Die Anzeige der reservierten Flächen beginnt mit dem ausgewählten Versandtag. Der angezeigte Zeitraum umfasst zwei Wochen.

#### Flächenkapazität pro Tag

In der Übersicht werden die reservierten Flächen entsprechend den Einstellungen in den Bereichen **Auflösung nach** und **Auswahl** angezeigt.
- **Kunde**: Name des Key-Kunden, für den Flächenkapazitäten reserviert sind.
- **Produktart**: Produktart, für die Flächenkapazitäten reserviert werden können.
- **Wochentag**: Anzeige der Flächensumme aus den offenen Aufträgen/reservierte Fläche.

Wenn die Summe der Flächen aus den offenen Aufträgen größer als die reservierte Fläche ist, wird der Eintrag rot markiert.

### OP Abfrage

> Dokumente > Auftrag > Auftrag auswählen > Menü Funktionen > Gruppe Finanzen > OP Abfrage

*Abb. C-294 OP-Abfrage*

In diesem Dialog werden alle offenen Posten des ausgewählten Kunden angezeigt.

Die Funktion Offene Posten Abfrage ist nur freigeschaltet, wenn das Programm zur Finanzbuchhaltung diese Funktion unterstützt. Zusätzlich muss in den Firmendaten die OP-Abfrage zugelassen sein.
- ⇨ Stammdaten, "Firmendaten - FiBu" auf Seite B-924

#### Kunde

**Nummer** Nummer und Name des Kunden, zu dem die offenen Posten angezeigt werden.

**Gebuchter Umsatz** Gesamtumsatz, der bereits verbucht aber noch nicht ausgeglichen wurde.

#### Offene Posten

Liste der Rechnungen, aus denen offene Posten zurückgemeldet wurden. Im unteren Bereich werden die Summen angezeigt.
- **Rechnungsnummer**: Nummer der offenen Rechnung. Die Nummer wurde beim Druck der Rechnung erzeugt.
- **Rechnungsdatum**: Das Datum der Rechnung, das standardmäßig dem Druckdatum entspricht.
- **Rechnungsbetrag brutto**: Der Gesamtbetrag der Rechnung. Anzahlungen oder Teilzahlungen sind in diesem Betrag nicht berücksichtigt.
- **Zahlungsbetrag**: Anzahlungen oder Teilzahlungen zur Rechnung.
- **Bemerkung**: Bemerkung, die zur Rechnung, Anzahlung oder Teilzahlung hinzugefügt wurde.
- **Fälligkeitsdatum**: Datum der Fälligkeit, das im Auftrag festgelegt wurde.
    - ⇨ "Kopfdaten - Zusatz" auf Seite C-426
- **Mahndatum**: Datum der letzten Mahnung
- **Mahnstufe**: Stufe der letzten Mahnung
- "Mahnstufe" auf Seite C-734

### Kreditlimitsperre

> Dokumente > Auftrag > Auftrag auswählen > Menü Funktionen > Gruppe Finanzen > Kreditlimitsperre löschen

*Abb. C-295 Kreditlimitsperre löschen*

In diesem Dialog werden alle Aufträge angezeigt, die aufgrund eines überschrittenen Kreditlimits gesperrt sind. Sie können Kundenaufträge auswählen und die Kreditlimitsperre löschen.

#### Dokumente

**[Alle], [Keine]** Über die Schaltflächen können alle Sie alle Checkboxen markieren oder die Markierung (en) entfernen.

### Kalkulatorische Frachtkosten

> Dokumente > Auftrag > Auftrag auswählen > Menü Funktionen > Gruppe Kalkulation > Kalkulatorische Frachtkosten

*Abb. C-296 Kalkulatorische Frachtkosten*

In diesem Dialog können Sie die aktuelle Kostenkalkulation für die Frachtkosten des Auftrags prüfen.

**Beispiel**
Ein Kunde wird mit Tour Regional à 0,68 €/km beliefert.
Bei einer Entfernung von 10 km ergeben sich pro Liefertermin kalkulatorische Frachtkosten von 6,80 €.

Verteilung der Frachtkosten anteilig bezogen auf tatsächliche Fläche je Auftrag:
2 Aufträge mit Gesamtfläche von 40 qm.
Auftrag 200188 mit Gesamtfläche von 30 qm = 75%
Auftrag 200189 mit Gesamtfläche von 10 qm = 25%

Verteilung der kalkulatorischen Frachtkosten von 6,80 €:
Auftrag 200188 = 5,10 € = 75%
Auftrag 200189 = 1,70 € = 25%

Wenn die kritische Frachtkostengrenze überschritten ist, werden die Beträge in roter Schrift angezeigt. Diese Grenze wird in den Firmendaten festgelegt.
- Stammdaten, "Firmendaten - Versand" auf Seite B-994

Eine übergreifende Kalkulation steht in Dialog Kalkulatorische Frachtkosten zur Verfügung:
- "Kalkulatorische Frachtkosten" auf Seite C-714

### Kosten- und Aufschlagskalkulation

> Dokumente > Auftrag > Auftrag auswählen > Menü Funktionen > Gruppe Kalkulation > Kosten- und Aufschlagskalkulation

*Abb. C-297 Kosten- und Aufschlagskalkulation*

In diesem Dialog können Sie die aktuelle Kosten- und Aufschlagskalkulation prüfen.
- ⇨ Stammdaten, "Firmendaten - Kalkulation" auf Seite B-981

### Übersicht Statusrückmeldung

> Dokumente > Auftrag > NV Auftrag > Menü Funktionen > Gruppe Produktion > Produktionsübersicht
> Dokumente > Auftrag > Menü Ansicht > Gruppe Produktion > Produktionsübersicht

*Abb. C-298 Produktionsübersicht/Übersicht Statusrückmeldung*

In diesem Dialog können Sie den aktuellen Produktionsstatus jeder einzelnen Auftragsposition prüfen. Wenn Sie die Rückmeldungen aus der Produktion per Datei empfangen, wird jeweils der zuletzt gemeldete Status angezeigt.

Bei der dateilosen Rückmeldung werden alle Statusänderungen online übertragen und angezeigt. In dieser Variante zeigt der Dialog immer den tatsächlichen Fortschritt der Produktion an.

#### Menü Optionen

**Nach Erfassungsstellentext sortiert** Die Einträge im Bereich Erfassungsstellen können nach dem Text oder nach der Nummer sortiert werden.

#### Auftragsinformationen

**Auftrag** Nummer des Auftrags, für den Statusmeldungen angezeigt werden sollen.

**Anschrift** Name und Anschrift des Kunden aus dem Auftrag.

**Status** Status des Auftrags. Der Status wird umgesetzt, wenn die Positionen fertig gemeldet werden.

**Positionen** Liste der Auftragspositionen.

**Stücklistenaufbau** Stückliste der markierten Auftragspositionen.

#### Erfassungsstellen

Für jede Auftragsposition wird eine Spalte mit den aktuellen Rückmeldungen angezeigt. Je nach Einstellung wird der Positionsstatus umgesetzt, wenn die erste Scheibe einer Position fertig gemeldet wird oder wenn alle Scheiben fertig gemeldet werden.
- ⇨ Stammdaten, "Erfassungsstellen Produktion" auf Seite B-870

Die zurückgemeldeten Zahlen werden in unterschiedlichen Farben dargestellt:
- **Grün**: Die gemeldete Stückzahl entspricht der Positionsmenge.
- **Blau**: Die gemeldete Stückzahl ist nur eine Teilmenge der Position.
- **Rot**: Die gemeldete Stückzahl muss erneut beauftragt werden, z. B. wegen Bruch.

**Symbol Produktionsrückmeldung** Rückmeldungen über die Betriebsdatenerfassung (BDE) werden in schwarzer Schrift angezeigt.

**Symbol A+W Production Rückmeldung** Rückmeldungen von A+W Production werden in blauer Schrift angezeigt.

### Lieferterminbestimmung

> Dokumente > Auftrag > Auftrag auswählen > Register Dokument > Schaltfläche am Feld Anlieferung

*Abb. C-299 Automatische Lieferterminbestimmung*

In diesem Dialog werden die Details zur Lieferterminbestimmung angezeigt, wenn der Auftrag an die Kapazitätsplanung übergeben wurde. Wenn der Liefertermin verschoben werden muss oder ein anderes Problem auftritt, wird eine Meldung mit dem neuen Liefertermin oder der Fehlerbeschreibung ausgegeben.

> **i**
> **Kapazitätsbelegung**
> Wenn für einen Auftrag eine Lieferterminbestimmung gestartet wird, wird der Auftrag in die Kapazitätsplanung eingelastet und belegt damit für eine bestimmte Zeit Maschinenkapazitäten in der Produktion.
> Ein Angebot wird nur temporär eingelastet und belegt keine Maschinen. Diese Option kann in A+W Production entsprechend eingerichtet werden.

### Liefertermin ändern

> Dokumente > Auftrag > Auftrag auswählen > Register Dokument > Schaltfläche am Feld Versandtag

*Abb. C-300 Liefertermin ändern*

In diesem Dialog können Sie einen alternativen Lieferanten auswählen, wenn die Wiederbeschaffungszeit beim Standard-Lieferanten die Produktion des Auftrags behindert.

### Zahlungsverwaltung

> Dokumente > Auftrag > Auftrag auswählen > Register Summen > [Anzahlungssumme]

*Abb. C-301 Anzahlungsverwaltung*

In diesem Dialog können Sie eine Anzahlung erfassen. Der Betrag wird nicht an die FiBu übergeben und vermindert die Auftragssumme nicht. Der Betrag wird erst mit der Fakturierung übergeben und verbucht.
- ⇨Tutorial, "Anzahlungen" auf Seite C-274

> **i**
> **Anzahlungsrechnung**
> Nur Anzahlungen, die über eine Anzahlungsrechnung erfasst wurden, werden sofort an die FiBu übergeben. Der Betrag der Anzahlungsrechnung vermindert den Gesamtbetrag des Auftrags.

#### Anzahlung

**Zahlungsdatum** Anzeige des Tagesdatums (Systemdatum).

**Typ** Der Betrag der Zahlung kann als Anzahlung oder als Teilzahlung erfasst werden. Bei einer Teilzahlung gehen Sie davon aus, dass der Auftrag in Form von Ratenzahlungen beglichen wird.

**Zahlungsart** Auswahl einer der hinterlegten Anzahlungsarten.

**Betrag / Währung** Betrag und Währung der erfassten Anzahlung.

**Status** Der Status wird automatisch auf Erfasst gesetzt, wenn die Anzahlung gespeichert wurde.

**Mitarbeiter** Name des Mitarbeiters, der sich in A+W Business angemeldet hat.

**Bemerkung** Sie können eine Bemerkung zur Anzahlung eintragen, z. B. Absprachen, die mit dieser Anzahlung oder Teilzahlung verbunden sind.

**Zahlungsrichtung** Auswahl einer der hinterlegten Zahlungsrichtungen.

**Zahlungsverfahren** Angabe des Zahlungsverfahrens.

**Zahlungsreferenz** Angabe der Zahlungsreferenz.

**Übersicht** In der Übersicht werden alle Zahlungen zum aktuellen Auftrag aufgelistet, die über diesen Dialog erfasst wurden. Anzahlungen, die über eine Anzahlungsrechnung erfasst wurden, sind hier nicht aufgeführt.

#### Summen

**Bruttobetrag** Bruttobetrag des Auftrags.

**- Anzahlung** Summe der Anzahlungen, die über diesen Dialog erfasst wurden.

**= Restbetrag** Differenz aus dem Gesamtbetrag des Auftrags und der Summe aller Anzahlungen, die über diesen Dialog erfasst wurden.

#### Sicherung

**Import Datei, Export Datei** Die Daten können importiert und exportiert werden.

#### Sonstiges

**Anzahlung per EDI** Sie können festlegen, ob Anzahlungen per EDI importiert werden können.
- Anzahlungen werden nicht per EDI importiert.
- Anzahlungen können auch per EDI importiert werden. Diese Einstellung ist automatisch gesetzt, wenn Aufträge per EDI importiert, die Anzahlungen enthalten.

## Übersichten und Referenzen zu Positionen

Sie können sich über die Menüs in der Positionserfassung verschiedene Informationen anzeigen lassen, ohne den Dialog zu schließen. Die Dialoge sind für alle Dokumentenarten gleich. Sie werden in dieser Anleitung am Beispiel Auftrag beschrieben.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Produktsuche" auf Seite C-582
- "Schnellanfrage" auf Seite C-587
- "Parameter-Ersetzung" auf Seite C-589
- "Produktabgleich" auf Seite C-590
- "Reklamationen" auf Seite C-591
- "Rückschnitt" auf Seite C-592
- "Variantenauswahl (Farbsuche)" auf Seite C-593
- "Festpreis Vorgabe" auf Seite C-594
- "Globale Änderungen" auf Seite C-595
- "Produktionsstücklistenauflösung" auf Seite C-596
- "Konditionen" auf Seite C-597
- "Preis-/Konditionsinformationen" auf Seite C-598
- "Artikel-Informationen" auf Seite C-602
- "Zusatz Stückliste – Ergänzungen" auf Seite C-607
- "Preisrecorder" auf Seite C-608
- "Artikel fixieren" auf Seite C-610
- "Position kopieren" auf Seite C-611
- "Kosten- und Aufschlagskalkulation (Position)" auf Seite C-613
- "Versicherungsleistung" auf Seite C-614
- "Teillieferungen" auf Seite C-616

### Produktsuche

> Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Positionen, Modelle/Bearbeitungen > [...], [Lupe]

In diesem Dialog finden Sie folgende Register:
- "Auswahl - Nach Produkt" auf Seite C-583
- "Auswahl - Nach technischen Parametern" auf Seite C-585
- "Auswahl - Nach Klassifikatoren" auf Seite C-586

### Auswahl – Nach Produkt

> Dokumente > Auftrag > Auftrag auswählen > Positionen > [...] > Register Nach Produkt

*Abb. C-302 Auswahl - Nach Produkt*

In diesem Register wählen Sie die Suchkriterien aus. Als Ergebnis werden jeweils alle Produkte angezeigt, die den gewählten Kriterien entsprechen. Wenn Sie keine Kriterien auswählen, werden alle Produkte aufgelistet.

**Produktart** Einschränkung der Suche auf die Produktart, der das gesuchte Produkt zugeordnet ist.
- ⇨ Stammdaten, "Produktarten und Produktgruppen" auf Seite B-140

**Produktgruppe** Einschränkung der Suche auf die Produktgruppe, der das gesuchte Produkt zugeordnet ist. Die Auswahl der Produktgruppe ist von der Produktart abhängig.

**Matchcode** Matchcode des gesuchten Produkts.

**Gesperrte Produkte anzeigen** Produkte können gesperrt sein, wenn sie nicht mehr im Auftrag erfasst werden sollen.
- Nur die Produkte werden gesucht, die aktuell im Verkauf angeboten werden können.
- Alle Produkte mit den gewählten Kriterien werden gesucht. Dazu gehören auch diejenigen, die nicht mehr im Verkauf angeboten werden können.
- ⇨ Stammdaten, "Produkt anlegen" auf Seite B-182

**Produktnr. von, bis** Einschränkung der Suche auf eine Folge von Produktnummern.

**Warengruppe** Einschränkung der Suche auf die Warengruppe, der das gesuchte Produkt zugeordnet ist.

**Bezeichnung 1, Bezeichnung 2** Einschränkung der Suche auf die Bezeichnungen, die in den Stammdaten hinterlegt sind. Bei Float-Glas ist in der Regel nur die Bezeichnung 1 hinterlegt.

**Artikelinfo enthält** Einschränkung der Suche auf einen Begriff in der Artikelinformation. Groß- und Kleinschreibung werden unterschieden.

#### Übersicht

In der Liste werden alle Produkte angezeigt, die die gewählten Suchkriterien erfüllen.

**Automatisch suchen** Die Suche kann manuell oder automatisch gestartet werden.
- Die Suche wird über die Schaltfläche [Suchen] gestartet, wenn alle Kriterien eingetragen sind.
- Die Suche beginnt mit der Eingabe des ersten Suchkriteriums.

**Klassifikatoren in Stückliste suchen** Die Suche anhand von Klassifikatoren kann sich auf das Hauptprodukt und auf die Stückliste beziehen.
- Die Suche über Klassifikatoren sucht nur in den Hauprodukten. Bei Produkten mit Stücklisten, werden die Ebenen nicht durchsucht.
- Die Suche bezieht die Stückliste mit ein.

### Auswahl - Nach technischen Parametern

> Dokumente > Auftrag > Auftrag auswählen > Positionen > [...] > Register Nach technischen Parametern

*Abb. C-303 Auswahl - nach technischen Parametern*

In diesem Register schränken Sie die Suche über technische Kriterien ein.

**Ug-Wert in W/qm** Wärmedurchgangskoeffizient. Der Ug-Wert gibt den Wärmeverlust eines Bauteils in W/qm an. Je kleiner der Ug-Wert desto größer ist die Wärmedämmung.

**Ug-Wert nach DIN 4108-4** Wärmedurchgangskoeffizient der Verglasung

**Lichtdurchl. in %** Die Lichtdurchlässigkeit drückt den direkt durchgelassenen, sichtbaren Strahlungsanteil in Prozent aus. Die Bezugsgröße von 100% gilt bei einer unverglasten Maueröffnung.

**g-Wert in %** Der Energiedurchlasswert setzt sich zusammen aus der direkten Sonnenenergietransmission und der sekundären Wärmeabgabe nach innen infolge langwelliger Strahlung und Konvektion.

**b-Faktor** Diese Größe stellt den mittleren Durchlassfaktor der Sonnenenergie dar, bezogen auf den Gesamtenergiedurchlassgrad einer 4-mm-Scheibe. Dies ist für die Kühllastberechnung eines Gebäudes notwendig.

**Schalldämmmaß in dB** Das Schalldämmmaß ist die kennzeichnende Wirkung beim Schallschutz. Je niedriger der dB-Wert, umso höher ist der Geräuschpegel von außen.

**Dickentoleranz in mm** Die Dicke kann bei Isolierglas um wenige Millimeter differieren. Dieses Feld nutzen Sie, wenn die Dicke des gesuchten Produktes ausschlaggebend ist.

**Größentoleranz mm (<200 cm), (>=200 cm)** Angabe, um wie viel Millimeter die ISO-Scheibe von ihrer vorgegebenen Größe abweichen kann.

**Technische Parameter anzeigen** In der Produktliste werden standardmäßig neben der Produktnummer, dem Matchcode und den Bezeichnungen 1 und 2 nur die Standardhöhe und -breite angezeigt.
- Die technischen Parameter werden in der Produktliste nicht angezeigt.
- Zusätzlich zu den Standardinformationen werden die technischen Parameter werden in der Produktliste angezeigt.

### Auswahl - Nach Klassifikatoren

> Dokumente > Auftrag > Auftrag auswählen > Positionen > [...] > Register Nach Klassifikatoren

*Abb. C-304 Auswahl - Nach Klassifikatoren*

In diesem Register schränken Sie die Suche über die Klassifikatoren ein, die zu einem Hauptprodukt hinterlegt sind.
- ⇨ Stammdaten, “Produktverwaltung - Anlagen/Klassifikatoren" auf Seite B-625

### Schnellanfrage

> Dokumente > Auftrag > Schnellanfrage
> Dokumente > Auftrag > Auftrag auswählen > Register Position > Menü Funktionen > Gruppe Position > Schnellanfrage

*Abb. C-305 Schnellanfrage für Kunden starten*

In diesem Dialog können Sie einen Kunden auswählen, um eine (telefonische) Anfrage schnell zu beantworten. Zum ausgewählten Kunden wird der aktuelle Stand des Kreditlimits angezeigt.

Wenn Sie während der Anfrage einen Auftrag mit Positionen erfasst haben, können Sie diesen speichern oder verwerfen.
- ⇨ Tutorial, "Schnellanfrage beantworten" auf Seite C-101

Wenn Sie die Schnellanfrage starten, wird zunächst ein Dialog zur Auswahl des anfragenden Kunden angezeigt. Nach der Wahl des Kunden werden die aktuellen Daten zum Kreditlimit und den offenen Posten angezeigt.

Anschließend wird die Positionserfassung mit leeren Feldern angezeigt. Der zugehörige Dokumentenkopf ist bereits mit den entsprechenden Kundendaten gefüllt.
- ⇨ "Dokument - Positionen" auf Seite C-451

Nachdem Sie die angefragten Positionen erfasst haben, können Sie die Anfrage beenden oder speichern. Zum Speichern können Sie festlegen, ob die Anfrage als Angebot oder als Auftrag gespeichert werden soll.

*Abb. C-306 Schnellanfrage speichern*

#### Speicherort

- **Angebot**: Die Schnellanfrage wird als Angebot gespeichert.
- **Auftrag**: Die Schnellanfrage wird als Auftrag gespeichert.

**Mandant** Die Wahl des Mandanten steuert die Anzeige im Feld Bereich.

**Bereich** Sie können den zuständigen AV-Bereich auswählen.

**Nummernverwalter** Das Dokument wird im entsprechenden Nummernverwalter gespeichert. Wenn Sie die Schnellanfrage als Auftrag speichern, wird automatisch der Nummernverwalter angezeigt, zu dem der zuletzt bearbeitete Auftrag gehört.

Nachdem Sie die Schnellanfrage beendet (schließen oder speichern) haben, wird automatisch das Dokument wieder angezeigt, in dem Sie zuletzt gearbeitet haben.

### Parameter-Ersetzung

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Modelle/Bearbeitungen > [Formel]

*Abb. C-307 Parameter-Ersetzung*

In diesem Dialog werden die erlaubten Variablen angezeigt, die Sie zur Modifizierung der Beschreibung verwenden können.

**Textersetzung** Sie können den Beschreibungstext bearbeiten. Er wird im Dialog Bearbeitungen im Feld Beschreibung angezeigt.

**Parameter mit identischer Bedeutung** In diesem Bereich werden die Parameter angezeigt, die synonym verwendet werden können.

### Produktabgleich

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Modelle/Bearbeitungen > Menü Start > iTOE

*Abb. C-308 Produktabgleich*

In diesem Dialog prüfen Sie die Regeln zu einer importierten DXF- oder SN-Datei für Bearbeitungen. Änderungen der Bearbeitung in der Auftragsposition werden gegen die hinterlegten Regeln geprüft.
- ⇨ Stammdaten, "iTOE Regeln" auf Seite B-659

Wenn Sie ein Modell erfasst und im A+W CAD Designer bearbeitet haben, können Sie die Änderungen als SN-Datei (TOE-Datei) speichern. Damit wird eine SN-Datei in der Stückliste angelegt, ein Modellsatz eingefügt und mit der TOE-Datei verknüpft.

Die TOE-Dateien werden in der Form XXXX_TOE.SN gespeichert, wobei die vorangestellte Nummer aus dem Nummernkreisen der SN-Dateien bestimmt wird.

> **i**
> **Eigenschaft von CAD-Bearbeitung**
> Änderungen von Eigenschaften, die nicht Bestandteil des A+W-Bearbeitungstypenkatalog sind, gehen beim Abgleich verloren, z. B. eine Bohrloch-Reihe mit Serienvermaßung: Die Serienvermaßung wirde gelöscht, sobald eine der beteiligten Bohrungen in der Bearbeitungserfassung geändert wird. Solche Änderungen müssen im A+W CAD Designer durchgeführt werden.

#### Übersicht

In der Übersicht werden die hinterlegten Regeln angezeigt. Bearbeitungen ohne Regel werden farbig hinterlegt.

Nach der Bestätigung des Produktabgleichs wird die Stückliste im Register Modelle/Bearbeitungen neu aufgebaut und die Preise werden neu berechnet. Jede weitere Änderung wird mit der verknüpften TOE-Datei abgeglichen.

- **CAD Bearbeitung**: Bezeichnung der Bearbeitung in A+W CAD Designer.
- **Produkt, Bezeichnung**: Nummer und Bezeichnung der Regel in A+W Business.
- **Regel bearbeiten/einfügen**: Wechsel zum Dialog iTOE Regeln, um eine Regel anzulegen oder zu bearbeiten.
    - ⇨ Stammdaten, "iTOE Regeln" auf Seite B-659
- **Gefundene Regel**: Bezeichnung der hinterlegte Regel zur Bearbeitung.
- **Eigenschaft**: Inhalt der hinterlegten Regel.

### Reklamationen

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Zusatz > [Ordner] neben dem Feld Grund

*Abb. C-309 Reklamation*

In diesem Dialog können Sie pro Position einen Reklamationsverursacher und einen Reklamationsgrund auswählen, wenn Sie ein Dokument des Typs Reklamation erfassen.
- ⇨Tutorial, "Reklamationen" auf Seite C-282

> **i**
> **Reklamation in anderen Dokumententypen**
> Wenn Sie den Dialog nicht im Dokumententyp Reklamation verwenden, werden die Angaben nicht in die Reklamationsstatistik übergeben.

**Verursacher** Der Verursacher kann in der Reklamationsstatistik zur Auswertung herangezogen werden. Die Eingabe ist optional.

**Grund** Der Grund kann in der Reklamationsstatistik zur Auswertung herangezogen werden. Die Eingabe ist optional.

**VK** Der Verkaufspreis für die beanstandete Position wird angezeigt. Dies ist der entgangene Umsatz.

**Kostenlos** Die Reklamationspositionen und auch -aufträge können statistisch ausgewertet werden, z. B. der Verkaufswert.
- Die Reklamation wird berechnet.
- Die Reklamation wird nicht berechnet, z. B. in Kulanzfällen oder bei eigenem Verschulden. Der VK-Wert zeigt den entgangenen Umsatz an.

### Rückschnitt

> Dokumente > Auftrag > Auftrag auswählen > Register Sprossen > [Rückschnitt]

*Abb. C-310 Rückschnitt*

In diesem Dialog legen Sie die Maße für den Rückschnitt pro Kante fest. Der Rückschnitt beschreibt den einfachen Abstand zwischen Fensteraußenkante und Rahmeninnenkante.

### Variantenauswahl (Farbsuche)

> Dokumente > Auftrag > Auftrag auswählen > Register Sprossen > Varianten suchen [Lupe]

*Abb. C-311 Variantenauswahl*

In diesem Dialog wählen Sie die Farb-Varianten zu einem erfassten Produkt aus.

#### Suchkriterien

**Bezeichnung** Bezeichnung der Farbe, nach der gesucht werden soll.

**Fremdschlüssel** Fremdschlüssel der Farbe, nach der gesucht werden soll.

#### Übersicht

- **Variante, Bezeichnung**: Interne Nummer und Bezeichnung der Farbe.
- **Fremdschlüssel**: Bei Dorma-Artikeln der Dorma-Farbschlüssel. Der Fremdschlüssel kann für die Kommunikation mit anderen Programmen verwendet werden, z. B. für die Übergabe an die Produktion.
- **Vorschau**: Anzeige der Farbvariante.
- **Sonderfarbe**: Sonderfarbe, z. B. beim Siebdruck.

### Festpreis Vorgabe

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Übersicht Positionen > Kontextmenü > Festpreis vorgeben

*Abb. C-312 Festpreis Vorgabe*

In diesem Dialog können Sie für markierte Position(en) einen Festpreis eintragen.

#### Selektierte Positionen

Alle markierten Positionen werden aufgelistet. Der Festpreis gilt für diese Positionen insgesamt.

#### Vorgabe

**Festpreis** Wenn Sie einen Festpreis für die markierten Positionen eingegeben haben, wird der Gesamtpreis für die einzelnen Positionen im Bereich Selektierte Positionen aktualisiert.

Die Werte werden in die Positionserfassung übernommen.

### Globale Änderungen

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Übersicht Positionen > Kontextmenü > Globale Änderungen

*Abb. C-313 Globale Änderungen*

In diesem Dialog ändern Sie die Kommissionsangabe übergreifend für die markierten Positionen.

#### Selektierte Positionen

In der Übersicht werden alle markierten Positionen aufgeführt, für die die Kommission geändert werden soll.

#### Änderung

**Kommission** Die Änderung gilt für alle Positionen, die in der Übersicht aufgeführt werden.
- Die Kundenkommission wird nicht geändert. Das Eingabefeld ist gesperrt.
- Die Kundenkommission kann geändert werden. Das Eingabefeld ist freigeschaltet.

### Produktionsstücklistenauflösung

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Stückliste > Stücklistenaufbau Kontextmenü (am Glas) > Produktionsstücklistenauflösung

*Abb. C-314 Produktionsstücklistenauflösung*

In diesem Dialog bearbeiten Sie die Produktionsstücklistenauflösung. Sie wird für Bearbeitungen immer am Glas definiert.

Bei Bearbeitungen kann die Produktionsstücklistenauflösung ausgeschaltet werden. Damit können Sie im aktuellen Auftrag eine Bearbeitung an den Einzelscheiben oder der gesamten Einheit festlegen.
- ⇨ Stammdaten, “Produktionsstücklistenauflösung festlegen" auf Seite B-189

### Konditionen

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Ansicht > Gruppe Konditionen > Konditionen

*Abb. C-315 Konditionen*

In diesem Dialog werden die Rabatte und individuellen Preise für den aktuellen Kunden angezeigt.
- ⇨ Stammdaten, "Rabatt anlegen" auf Seite B-353

#### Rabatte

Anzeige der Rabatte, die für den aktuellen Kunden gelten. Diese können sich sowohl auf den einzelnen Kunden als auch auf die Kundengruppe beziehen, zu der der aktuelle Kunde gehört.

#### Individuelle Preise

Anzeige der Preise, die speziell für den aktuellen Kunden oder seine Kundengruppe hinterlegt sind. Wenn keine kundenindividuellen Preise angelegt sind, bleibt das Feld leer.

### Preis-/Konditionsinformationen

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Ansicht > Gruppe Konditionen > Preis-/Konditionsinformation

In diesem Dialog können Sie sich über die Preise und Konditionen informieren, die für den aktuellen Kunden gelten.

> **i**
> **Voraussetzung**
> Der Dialog steht nur zur Verfügung, wenn Sie in den Firmendaten die Preisberechnung nach Makro-Preisen aktiviert haben.

In diesem Dialog finden Sie folgende Register:
- "Preis-/Konditionsinformationen – Preisabfrage" auf Seite C-598
- "Preis-/Konditionsinformationen – Makropreise" auf Seite C-599
- "Preis-/Konditionsinformationen - Rabatte" auf Seite C-600
- "Preis-/Konditionsinformationen – Autom. Zuschläge" auf Seite C-601
- "Preis-/Konditionsinformationen - Kunde" auf Seite C-602

### Preis-/Konditionsinformationen – Preisabfrage

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Ansicht > Gruppe Konditionen > Preis-/Konditionsinformation > Register Preisabfrage

*Abb. C-316 Preis-/Konditionsinformationen – Preisabfrage*

In diesem Register können Sie sich über Details zu den Preisen informieren. Die Anzeige kann nach verschiedenen Kriterien gefiltert werden.

#### Auswahl

Mit der Wahl der Option legen Sie fest, ob die Preise für ein Produkt, eine Produktart oder eine Produktgruppe angezeigt werden sollen.

**Jahrgang, Schlüssel** Sie können die Preise nach Tarifen filtern.

#### Druckoptionen

Sie können die Daten drucken. Dazu legen Sie fest, ob die Angaben aus allen oder nur aus bestimmten Registern ausgegeben werden sollen.
- Die Daten aus dem entsprechenden Register werden nicht mit gedruckt, z. B. aus dem Register Rabatte.
- Die Daten aus dem entsprechenden Register werden mit gedruckt.

### Preis-/Konditionsinformationen – Makropreise

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Ansicht > Gruppe Konditionen > Preis-/Konditionsinformation > Register Makropreise

*Abb. C-317 Preis-/Konditionsinformationen – Makropreise*

In diesem Register werden die Makropreise und der zugehörige Produktaufbau aufgelistet.

Die Felder zu den Druckoptionen sind zu Register Preisabfrage erklärt.
- ⇨ "Preis-/Konditionsinformationen – Preisabfrage" auf Seite C-598

### Preis-/Konditionsinformationen – Rabatte

> Dokumente > Auftrag > Auftrag auswählen > Positionen > Menü Ansicht > Gruppe Konditionen > Preis-/Konditionsinformation > Register Rabatte

*Abb. C-318 Preis-/Konditionsinformationen - Rabatte*

In diesem Register werden die Rabatte angezeigt, die für den aktuellen Kunden gültig sind.

Die Felder zu den Druckoptionen sind zu Register Preisabfrage erklärt.
- ⇨ "Preis-/Konditionsinformationen – Preisabfrage" auf Seite C-598
