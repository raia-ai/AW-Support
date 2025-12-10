---
title: "A+W Business Einkauf - Rechnung und Rechnungskontrolle"
source: "DE_AWBusiness_Einkauf_3_6.pdf"
tags: ["A+W Business", "Einkauf", "Rechnungskontrolle", "Elektronische Rechnung", "Software-Dokumentation", "ERP", "Bestellprozess", "Lieferantenrechnung", "openTRANS"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Dieses Dokument ist ein Auszug aus der Softwarereferenz für A+W Business Einkauf. Es beschreibt die Funktionalitäten zur manuellen und elektronischen Rechnungskontrolle, einschließlich der Prüfung von Positionen, Stücklisten und der Verarbeitung von Lieferantenrechnungen."
long_description: "Diese Softwarereferenz bietet eine detaillierte Anleitung zur Handhabung von Lieferantenrechnungen im A+W Business Einkauf Modul. Der Fokus liegt auf der 'Rechnungskontrolle', einem Werkzeug zur Überprüfung von Rechnungen gegen die ursprünglichen Bestellungen. Das Dokument gliedert sich in die manuelle und die elektronische Rechnungskontrolle. Im manuellen Teil werden die Register 'Positionen' und 'Stückliste' erläutert, in denen Benutzer die Preise, Mengen und Maße jeder Bestellposition und ihrer Komponenten vergleichen und korrigieren können. Ein weiterer Abschnitt behandelt die Einschränkungsmöglichkeiten für das Rechnungsdatum, um Fehleingaben zu vermeiden. Der Hauptteil widmet sich der 'Elektronischen Rechnungskontrolle', die den Import und die Verarbeitung elektronischer Rechnungsdokumente (z.B. im openTRANS-Format) ermöglicht. Es werden die Menüfunktionen, Optionen zur Automatisierung, der Dokumentenimport-Dialog mit seinen Statusanzeigen und die Positionsübersicht zum Abgleich von Rechnungs- und Bestelldaten beschrieben. Das Dokument schließt mit einer kurzen Erläuterung der 'Basisglasverrechnung' und einem umfassenden Index für das gesamte Einkauf-Modul."
---

# Rechnungskontrolle – Positionen

**Pfad:** `Dokumente > Bestellung > Rechnung > Rechnungskontrolle > Register Positionen`

In diesem Register können Sie die Positionen aller Bestellungen prüfen, zu der Sie eine Lieferantenrechnung erfasst haben.

Das Register wird nur angezeigt, wenn im Register Bestellungen die Pflichtfelder gefüllt sind und mit [Ausführen] bestätigt wurden.

*(Siehe auch: Tutorial, "Rechnung kontrollieren" auf Seite D-146)*

*(Referenz: Abb. D-144 Rechnungskontrolle – Positionen)*

---
### Bestellpositionen

In der Übersicht werden alle Positionen der Bestellungen aufgeführt, auf die sich die Rechnung bezieht.

- **Bestell-Nr.:** Nummer, mit der die Bestellung in der Datenbank gespeichert ist.
- **Pos:** Nummer der Bestellposition.
- **Artikel:** Bezeichnung der bestellten Position.
- **Breite / Höhe:** Maße der bestellten Position.
- **Euro-Netto:** Preis der Position in der Landeswährung (hier Euro). Wenn Sie mit einer anderen Währung arbeiten, ändert sich die Bezeichnung entsprechend. Wenn Sie mit zwei Währungen arbeiten, wird für die zweite Währung eine weitere Spalte mit dem entsprechenden Betrag angezeigt.
- **Mwst.-Euro:** Betrag der Mehrwertsteuer in der Landeswährung (hier Euro). Die Spalte wird nicht angezeigt, wenn im Register Bestellungen die Option Netto gewählt ist. Für die Anzeige der Mehrwert-Steuer im Mehrwährungssystem gilt das gleiche, wie für die Anzeige des Betrags.
- **Stückl.genaue Eingabe:** In dieser Spalte wird angezeigt, ob Sie Preisdifferenzen auf der Ebene der Stücklisten-Komponenten oder der Positionen korrigiert haben.
    - **Deaktiv:** Der Preis wurde nicht geändert oder der Preis der gesamten Position wurde geändert.
    - **Aktiv:** Der Preis wurde in der Stückliste geändert.
- **Menge:** Gelieferte Menge.
- **Lieferant:** Nummer und Name des Lieferanten.

**Gesamtbetrag:** Anzeige der Summe der (eingegebenen) Positionsbeträge.
**Gesamtmenge:** Summe der Positionsmengen.
**Differenz:** Anzeige der Differenz zwischen der Rechnungssumme im Register Bestellungen und der Summe der (eingegebenen) Positionsbeträge. In diesem Fall kann der Preis nicht bestätigt werden, bevor Sie die Preise der Positionen oder der Stücklisten geändert haben.

> **Differenz**
> Eine Differenz wird auch angezeigt, wenn Sie im Register Bestellungen versehentlich eine falsche Rechnungssumme eingetragen haben oder der Wechselkurs nicht korrekt ist.

# Rechnungskontrolle – Stückliste

**Pfad:** `Dokumente > Bestellung > Rechnung > Rechnungskontrolle > Register Stückliste`

In diesem Register können Sie sich den Preis einer Position auf der Ebene der Stückliste und der Stücklisten-Komponenten anzeigen lassen. Das Register ist nur aktiv, wenn im Register Positionen eine Position mit Stückliste markiert ist.

*(Siehe auch: Tutorial, "Rechnung kontrollieren" auf Seite D-146)*

*(Referenz: Abb. D-145 Rechnungskontrolle – Stückliste)*

### Stücklistenaufbau
In diesem Feld wird die Stückliste der Position angezeigt, die im Register Positionen markiert ist.

### Preise
Die Anzeige der Felder hängt davon ab, welche Stücklisten-Komponente markiert ist.
Sie können die Preise auf der Hauptebene oder an den Stücklisten-Komponenten korrigieren. Sie können die Austauschzuschläge und Preise der einzelnen Komponenten ändern.

- **Preis / PE:** Anzeige des Preises und der Preiseinheit aus der Bestellung.
- **Rabatt:** Anzeige des Rabattes aus der Bestellung. Der Wert kann nicht geändert werden.
- **Netto / Positionsmenge:** Anzeige des Preises und der Menge aus der Bestellung, wenn die Hauptposition markiert ist. Der Wert kann nicht geändert werden.
- **Netto / Stücklistenmenge:** Anzeige des Preises und der Menge aus der Bestellung, wenn eine Komponente markiert ist. Der Wert kann nicht geändert werden.
- **Netto ges.:** Anzeige des Positions-Preises aus der Bestellung, wenn die Hauptposition markiert ist. Der Wert kann geändert werden.
- **Netto ges. / Pos. Menge:** Anzeige des Komponenten-Preises und der Menge, wenn eine Komponente markiert ist. Der Wert kann geändert werden.
- **Gesamtsumme:** Anzeige des Komponenten-Preises pro Position, wenn eine Komponente markiert ist. Der Wert kann geändert werden.

# Rechnungsdatum

**Pfad (1):** `Dokumente > Bestellung > Auftragsbestätigung > Preiskontrolle > Menü Optionen > Gruppe Verhalten > Einschränkung bei Rech.dat.`
**Pfad (2):** `Dokumente > Bestellung > Rechnung > Rechnungskontrolle > Menü Optionen > Gruppe Verhalten > Einschränkung bei Rech.dat.`

In diesem Dialog können Sie angeben, um wie viele Tage das Rechnungsdatum vom aktuellen Tagesdatum höchstens abweichen darf. Damit können fehlerhafte Eingaben des Datums verhindert werden.
Die Einstellung ist nur für die Rechnungskontrolle sinnvoll.

*(Referenz: Abb. D-146 Einschränkungen für Rechnungsdatum)*

### Abweichung
**In Tagen:** Der Wert gibt die Anzahl der Tage an, um die das Rechnungsdatum vom aktuellen Tagesdatum abweichen darf. Wenn der erlaubte Zeitraum durch eine fehlerhafte Eingabe des Datums überschritten wird, wird automatisch das maximal erlaubte Datum eingesetzt.

> **Beispiel**
> Angezeigt: 24.08. - erlaubt sind 10 Tage
> Eingabe 13.08. - Korrektur auf 14.08.

Wenn Sie eine 0 (Null) eintragen, ist die Funktion abgeschaltet.

# Elektronische Rechnungskontrolle

**Pfad:** `Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle`

Wenn Sie Rechnungen Ihrer Lieferanten elektronisch erhalten, können Sie die Zuordnung der Positionen zu Ihren Bestellungen, die Preise und Termine prüfen. Dazu steht Ihnen die elektronische Rechnungskontrolle zur Verfügung.

- *Siehe auch: Tutorial, "Export/Import (openTRANS)" auf Seite D-151*
- *Siehe auch: Tutorial, "Elektronisches Dokument prüfen" auf Seite D-170*

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite D-256
- "Menü Optionen" auf Seite D-257
- "Elektronische Rechnungskontrolle - Dokumentenimport" auf Seite D-259
- "Elektronische Rechnungskontrolle - Positionsübersicht" auf Seite D-262

## Menü Funktionen

**Pfad:** `Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Menü Funktionen`

Über dieses Menü können Sie andere Dialoge öffnen, ohne die elektronische Rechnungskontrolle zu schließen.

Folgende Einträge werden angezeigt:
- **Anlieferpauschale einfügen:** Die Lieferpauschale wird automatisch als Position im Register Positionen eingefügt. Wenn in der Bestellung bereits eine Lieferpauschale enthalten ist, wird die Option nicht ausgeführt.
- **Bestellerfassung öffnen:** Während der Rechnungskontrolle sind alle aufgelisteten Bestellungen für die Bearbeitung (durch andere Mitarbeiter) gesperrt. Mit dieser Funktion können Sie den Dialog Dokumentenverwaltung öffnen, um eine der angezeigten Bestellungen zu bearbeiten. Geänderte Werte werden in die Rechnungskontrolle übernommen. *(Siehe auch: Verkauf, "Dokument - Kopfdaten" auf Seite C-417)*
- **Positionen manuell zuordnen:** Öffnet den Dialog Positionen manuell zuordnen, um die Positionen des elektr. Dokuments den Positionen der Bestellung(en) zuzuordnen. *(Siehe auch: "Positionen manuell zuordnen" auf Seite D-221)*
- **Fußzuschläge/-rabatte auf Bestellungen verteilen:** Öffnet den Dialog Fußzuschläge/-rabatte auf Bestellungen verteilen, um den Zuschlag/Rabatt aus dem elektr. Dokument auf die zugeordneten Bestellungen zu verteilen. *(Siehe auch: "Fußzuschläge/-rabatte verteilen" auf Seite D-222)*
- **Manuelle Positionszuordnung aufheben:** Hebt die manuelle Zuordnung der markierten Rechnungs-/Bestellpositionen wieder auf.
- **Alle Positionszuordnungen aufheben:** Hebt alle manuellen Zuordnungen von Rechnungs- und Bestellpositionen wieder auf.

## Menü Optionen

**Pfad:** `Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Menü Optionen`

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

### Gruppe Allgemein
- **Betragsdifferenzen akzeptieren:** Bei der elektronischen Rechnungskontrolle können Betragsdifferenzen, die durch Rundungen auftreten können, generell akzeptiert werden.
- **Hinweis auf Betragsdiff./Ausgl.pos.:** Wenn Rundungsdifferenzen automatisch einer Ausgleichsposition zugeordnet wurden, wird ein Hinweis angezeigt.
- **Rabatt einfrieren:** Mit dieser Option wird der Rabatt fixiert. Diese Option sollten Sie aktivieren, wenn Sie neue Rabatte festgelegt haben, in den alten Bestellungen aber die alten Rabatte angewendet werden sollen. Die Preise werden dann nach der Rechnungskontrolle nicht neu errechnet.
- **Auftr.-EK nur korrigieren bis in Statistik:** Die Korrekturen des EK-Preises im referenzierten Auftrag werden nur durchgeführt, solange der Auftrag noch in der Hauptdatenbank vorhanden ist und nicht an die Statistik übergeben wurde.
- **Prod.Nr. für Ausgleichspos.:** Öffnet den Dialog Auswahl, um eine Ausgleichposition für Rundungsdifferenzen zuzuordnen. *(Siehe auch: "Auswahl (Prod. Nr. für Ausgleichspos.)" auf Seite D-220)*

### Gruppe Einstellungen
- **Hinweis auf Lieferterminüberschreitung:** Bei Überschreitung des geplanten Liefertermins wird eine Meldung angezeigt.
- **Automatische Zuordnung unterdrücken:** Im Dialog Positionen manuell zuordnen können Sie die Checkbox für die automatische Zuordnung aktivieren, damit die Fußzuschläge/-rabatte der Auftragsbestätigung automatisch einem A+W Business-Produkt zugeordnet werden. Diese automatische Zuordnung können Sie unterdrücken. *(Siehe auch: "Zuordnung des Fußzuschlags/-rabatts zukünftig automatisch auflösen" auf Seite D-222)*. Wenn diese Option geändert wurde, muss das aktuell eingelesene Dokument nochmals eingelesen werden. *(Siehe auch: Tutorial, "So lesen Sie ein XML-Dokument ein" auf Seite D-169)*
- **Referenzierenden Produktnummern des Lieferanten vertrauen:** Wenn im importierten Dokument eine A+W Business-Produktnummer als Referenz angegeben ist, kann die Zuordnung automatisch durchgeführt werden.

### Gruppe Xternal
- **Xternal-XML-Datei erstellen:** Für den elektronischen Datenaustausch wird eine XML-Datei erzeugt.
- **Einstellungen für Xternal:** Öffnet den Dialog Einstellungen, um Vorgaben für den XML-Export festzulegen. Diese Funktion ist nur freigeschaltet, wenn die Option Xternal-XML-Datei erstellen aktiviert ist.

## Elektronische Rechnungskontrolle – Dokumentenimport

**Pfad:** `Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Register Dokumentenimport`

In diesem Register prüfen Sie die importieren Rechnungen. Nur wenn der Dokumentenstatus fehlerfrei ist, kann die Rechnungskontrolle erfolgreich abgeschlossen werden.

- *Siehe auch: Tutorial, "Export/Import (openTRANS)" auf Seite D-151*
- *Siehe auch: Tutorial, "Elektronisches Dokument prüfen" auf Seite D-170*

*(Referenz: Abb. D-147 Elektronische Rechnungskontrolle – Dokumentenimport)*

### Buchungsart
Mit der Wahl der Option legen Sie fest, wie das elektronische Dokument verarbeitet werden soll. Die Optionen sind dem Dokumentenstatus entsprechend freigeschaltet.

- **Ablehnen:** Mit dieser Option werden die Dokumente nicht übernommen. Die Rechnungskontrolle wird nicht durchgeführt.
- **Akzeptieren:** Mit dieser Option wird die Rechnungskontrolle bestätigt. Die AB-Nummer, Preise und Liefertermine aus dem importierten Dokument werden in die Bestellungen zurückgeschrieben. Die Dokumentenhistorie wird aktualisiert.
- **Teillieferung erstellen:** Zu den im Dokument (Teilrechnung) enthaltenen Positionen wird eine (neue) Teillieferung erstellt und wie bei Akzeptieren verbucht. Die restlichen Positionen bleiben in der ursprünglichen Bestellung erhalten. Der Status dieser Bestellung wird entsprechend angepasst. Bei einem Lieferavis wird mit dieser Buchungsart eine Teilbestellung erzeugt.

### Rechnungen
In der Übersicht sind alle importierten Rechnungen aufgelistet. Diese können auch von unterschiedlichen Lieferanten stammen. Wenn Sie einen Eintrag markieren, werden die referenzierten Dokumente in der Übersicht Bestellungen / Teillieferungen angezeigt.

- **Rechnungsnummer:** Rechnungsnummer, die der Lieferant angegeben hat.
- **Lieferant:** Name des Lieferanten.
- **Netto:** Gesamtbetrag der Lieferung.
- **Mwst:** Betrag der Mehrwertsteuer dieser Rechnung.
- **Währung:** Währung, in der der Betrag in der Rechnung angegeben ist. Diese Anzeige ist nur dann von Bedeutung, wenn Sie mit einem Mehrwährungssystem arbeiten.

**Anzeige:** Sie können die Anzeige der Dokumente einschränken.
**Filtereinstellungen:** Sie können Filter für die Anzeige der importierten Dokumente festlegen. *(Siehe auch: "Filtereinstellungen" auf Seite D-223)*

### Dokumentenstatus
Die rote oder grüne Markierung gibt an, ob Unstimmigkeiten festgestellt wurden oder nicht. Die Optionen im Bereich Buchungsart sind entsprechend gesperrt oder freigeschaltet.

- **Kein Dokument ausgewählt:** Die Anzeige des Dokumentenstatus kann nicht aktualisiert werden, da kein Dokument in der Übersicht markiert ist. Dieser Eintrag wird nicht angezeigt, wenn eine Rechnung markiert ist.
- **Mindestens ein Fußzuschlag/-rabatt einer Bestellung konnte dem Dokument nicht zugeordnet werden:** Dieser Eintrag wird nur angezeigt, wenn eine Rechnung mit einem entsprechenden Fehler markiert ist.
- **Bestellungen vollständig referenziert:** Bei einer roten Anzeige stimmt mindestens eine der referenzierten Positionen nicht vollständig mit der importierten Rechnung überein. Die unvollständig referenzierten Bestellungen werden in der Übersicht gekennzeichnet.
- **Fehlende Artikelpositionen in Bestellungen:** In der Rechnung sind Positionen enthalten, die in der Bestellung nicht aufgeführt sind.
- **Fehlende Fußzuschläge/-rabatte in Bestellungen:** Fußzuschläge/-rabatte werden nicht mitbestellt. Da sie aber in der Rechnung aufgeführt sind, müssen sie für die Rechnungskontrolle als Positionen in den Bestellungen vorhanden sein. Die fehlenden Fußzuschläge/-rabatte müssen in der Bestellung manuell erfasst werden.
- **Preisdifferenz:** Die Gesamtpreise von Bestellung und Rechnung sind unterschiedlich. In zugehörigen Feldern wird die Abweichung als Betrag und prozentual angezeigt.
- **Mengendifferenz:** Die Positionsmengen von Bestellung und Rechnung sind unterschiedlich.

**[Dokument anzeigen]:** Öffnet die Dokumentenansicht des markierten Dokuments.

### Bestellungen / Teillieferungen
In der Übersicht werden die referenzierten Dokumente angezeigt, wenn Sie einen Eintrag im Bereich Rechnungen markiert haben. Teillieferungen werden in blauer Schrift angezeigt.

- **Bestellnummer:** Nummer der Bestellung, die von A+W Business erzeugt wurde.
- **Netto:** Gesamtbetrag der Bestellung.
- **Mwst:** Betrag der Mehrwertsteuer dieser Bestellung.
- **Währung:** Währung, in der der Betrag in der Bestellung angegeben ist. Diese Anzeige ist nur dann von Bedeutung, wenn Sie mit einem Mehrwährungssystem arbeiten.
- **Auftr.Nr.:** Nummer des referenzierten Auftrags.
- **Kundenliefertermin:** Datum der Anlieferung beim Kunden.
- **Bemerkung:** Wenn die Verknüpfung zwischen der Bestellung und dem importierten Dokument nicht vollständig ist, wird ggf. ein Hinweis auf den Fehler angezeigt.

## Elektronische Rechnungskontrolle – Positionsübersicht

**Pfad:** `Dokumente > Bestellung > Rechnung > Elektr. Rechnungskontrolle > Register Positionsübersicht`

In diesem Register können Sie die Positionen der Rechnung prüfen, die Ihr Lieferant gesendet hat. Die Optionen im Bereich Buchungsart sind zu Register Dokumentenimport erklärt.

*(Siehe auch: "Elektronische Rechnungskontrolle - Dokumentenimport" auf Seite D-259)*

*(Referenz: Abb. D-148 Elektronische Rechnungskontrolle – Positionsübersicht)*

### Positionsübersicht
In der Übersicht sind alle Positionen der Rechnung aufgeführt. Wenn Sie eine Position markieren, werden die Details in den Bereichen Dokumentenposition und Bestellposition angezeigt.

- **Pos-Nr.:** Positionsnummer aus der AB.
- **Bestell-Nummer:** Nummer der referenzierten Bestellung.
- **Bestell-Position:** Positionsnummer aus der Bestellung.
- **Netto Dokument/Netto 1 Bestellung:** Positionspreis aus der importierten AB und aus der Bestellung.
- **Menge Dokument/Menge 1 Bestellung:** Positionsmenge aus der importierten AB und aus der Bestellung.
- **Abmessung Dokument/Abmessung 1 Bestellung:** Positionsmaße aus der importierten AB und aus der Bestellung.
- **Differenz Preis:** Differenz aus Spalte Netto Dokumente und Netto Bestellung.
- **Differenz 1 Preis %:** Preisdifferenz in Prozent.
- **Differenz 2 Menge:** Differenz aus Spalte Menge Dokumente und Menge Bestellung.
- **Auftr.Nr.:** Nummer des referenzierten Auftrags.
- **Kundenliefertermin:** Datum der Anlieferung beim Kunden.

### Dokumentenposition, Bestellposition
In diesen beiden Bereichen werden Details zu der Position angezeigt, die in der Positionsübersicht markiert ist.

# Basisglasverrechnung

**Pfad:** `Dokumente > Bestellung > Basisglasverrechnung`

Diese Funktion ist nur kundenspezifisch freigeschaltet.
In der Basisglasverrechnung werden Modellscheiben mit ihrer tatsächlichen Fläche anstatt der fakturierten Fläche übergeben und verrechnet.

# Index Einkauf

### A
- **A+W B2B Purchasing Service** D-159
- **AB Lieferant** D-197
  - Auftragsdaten D-200
  - Bestelldaten D-199
  - Bestellpositionen D-201
  - Liefertermin D-203
- **AB siehe auch Auftragsbestätigung**
- **AB-Lieferant**
  - Wareneingang D-198
  - Wareneingang pro Position D-202
- **Anfrage**
  - Referenz D-111
  - über Bestellpool erzeugen D-113
  - unabhängige Bestellung erzeugen D-115
  - zu Kundenauftrag erzeugen D-112
  - zu Kundenposition D-111
- **Anfrage (Menü)** D-186
- **Anzeige**
  - im elektr. Dokument filtern D-223
- **Auftrag**
  - Lieferant pro Position D-52
- **Auftragsbestätigung**
  - des Lieferanten erfassen D-89
  - Einkauf D-87
  - elektr. Preiskontrolle D-213
  - für Position erfassen D-91
  - Lieferant D-197
  - Preis pro Position D-210
  - Preise prüfen D-146
  - Preiskontrolle D-204
  - Stücklistenpreise D-212
- **Auftragsdaten**
  - AB Lieferant D-200
- **Ausgleichposition** D-220
- **AW Common Base Service** D-159
- **AWProtocolService** D-159

### B
- **Bestellanfrage** D-186
- **Bestellarten**
  - Lagerbestellung D-80
  - referenzierte Bestellung D-45
  - unabhängige Bestellung D-80
- **Bestelldaten**
  - AB Lieferant D-199
- **Bestellkennzeichen**
  - Einkauf D-22
- **Bestellpool** D-62
  - Anfrage erzeugen D-113
  - Lieferant ändern D-72
  - Preise vergleichen D-74
  - Sammelbestellung D-67
- **Bestellposition**
  - AB erfassen D-91
  - im Auftrag erfassen D-54
  - Produktion D-122
- **Bestellte Position ändern** D-57
- **Bestellung**
  - Auftragsbestätigung D-87
  - aus Kundenauftrag D-51
  - aus unabhängiger Anfrage erzeugen D-115
  - automatisch D-60
  - Bestellpool D-62
  - bestellte Position ändern D-53, D-57
  - Eingangskontrolle D-125
  - elektr. Preiskontrolle D-213
  - elektr. Rechnungskontrolle D-256
  - Export (Dokument) D-193
  - Fremdwährung D-145
  - Kiste erfassen D-83
  - Kundenbestellung D-51
  - Lagerbestellung erfassen D-83
  - Lieferanten ändern D-72
  - Liefertermin D-65
  - Mahnung D-88
  - manuell D-45
  - manuell erfassen D-81
  - Mengendiskrepanzen D-243
  - Preiskontrolle D-207
  - Preisvergleich D-65
  - Rechnungskontrolle D-248
  - Sammelbestellung D-67
  - Teilbestellung D-259
  - Terminüberwachung D-101
  - übergeben D-68
  - unabhängige Bestellung D-80
  - unabhängige Bestellung erfassen D-81
  - Wareneingang komplett D-241
- **Bestellung (Menü)** D-188
- **Betragsdifferenz**
  - elektronisches Dokument D-158
  - Produktzuordnung D-220
- **Buchen**
  - Teillieferung D-216
  - Wareneingang D-127

### D
- **Buchungsart**
  - Dokumentenimport D-156
  - elektronische Preiskontrolle D-216
  - Preiskontrolle D-216
- **Darstellungskonventionen** D-13
- **Datenaustausch** D-150
  - Dokument D-151
  - Fremdschnittstellenverwaltung D-178
  - openTRANS-Dokument einlesen D-169
  - XML-Datei einlesen D-169
- **Datenexport**
  - EDI D-177
- **Dienste**
  - A+W B2B Purchasing Service D-159
  - AW Common Base Service D-159
  - AWProtocolService D-159
  - ERP-WebService D-159
- **Differenz**
  - Rechnungskontrolle D-251
- **Dokument**
  - Bestellung D-45
- **Dokumentation**
  - Arten D-12
- **Dokumente**
  - Bestellanfrage D-186
  - Bestellung D-188
  - Einkauf D-185
- **Dokumentenaustausch** D-150
  - Dienste D-159
  - openTRANS D-151
  - Referenzen D-154
  - XML-Datei D-151
- **Dokumentenimport** D-155
  - Buchungsart D-156
  - Fußzuschläge/-rabatte D-157
  - openTRANS-Datei einlesen D-169
  - Positionszuordnung D-157
  - Rundungsdifferenz D-158
  - XML-Datei einlesen D-169
- **Dokumentenstatus** D-217

### E
- **EDI**
  - Einstellungen für Datenexport D-178
  - Export D-177
  - Fremdschnittstellenverwaltung D-178
- **Eingangskontrolle** D-241
- **Einkauf**
  - Anfrage D-110, D-186
  - Beschaffungsart D-23
  - Bestellkennzeichen D-22
  - Bestellübergabe aus Auftrag D-60
  - Bestellung D-190
  - Dokumente D-185
  - Firmendaten für Bestellung prüfen D-47
  - Firmendaten prüfen D-161
  - Firmendaten prüfen (Kisten) D-136
  - Grundgedanken D-17
  - Handlungsablauf D-18
  - Liefertermin D-87
  - Menü-Übersicht D-14
  - Nachbestellung D-191
  - Preiskontrollen D-143
  - Preislisten D-37
  - Rechnungskontrolle D-144
  - Schema D-17
  - Schnittstellenverwaltung prüfen D-178
  - Stammdaten Lieferant prüfen D-32
  - Stammdaten Preise prüfen D-38
  - Stammdaten Produkt prüfen D-25
  - Stammdaten Währung prüfen D-162
  - Status D-41
  - Status für elektr. Dokument prüfen D-163
  - Statuszuordnung D-41
- **Einstellungen**
  - Kisten-ID D-240
- **EK-Rückschreibung**
  - Lagerbewertung D-145
- **Elektr. Dokument**
  - Status D-160
- **Elektronische Rechnungskontrolle** D-256
- **Elektronischer Datenaustausch** D-150
  - Anzeige D-223
  - Dokumentenstatus D-217
  - EDI-Schnittstelle (Einstellungen) D-178
  - Filtereinstellungen D-223
  - openTRANS-Einstellungen D-166
  - Preiskontrolle D-213
  - Rechnungskontrolle D-256
  - Referenzen D-161
  - Schnittstellenverwaltung D-166
  - Währungen D-162
- **Elektronischer Dokumentenaustausch**
  - Dienste D-159
  - Firmendaten D-161
  - Partnerstammdaten D-168
  - Position zuordnen D-221
- **Elektronisches Dokument**
  - Betragsdifferenz D-158
  - Position zuordnen D-173
  - prüfen D-170
  - Teillieferung erstellen D-172
  - Zuschlag/Rabatt verteilen D-175

### F
- **Elektronsicher Dokumentenaustausch**
  - Statusdefinition D-163
- **ERP-WebService** D-159
- **Etikett**
  - für Kiste drucken D-142
- **Export**
  - Bestellung D-195
  - Datenexport per EDI D-193
  - Dokument (openTRANS) D-153
  - EDI-Einstellungen D-178
  - Übertragungspool D-196
- **Externe Kundennummer** D-168
- **Firmendaten**
  - Einstellungen für Wareneingang D-126
  - Referenzen D-161
  - virtuelle Positionsnummer D-47, D-136
- **Fremdschnittstelle**
  - Export (EDI) D-193
  - Übertragungs-Pool D-196
- **Fußzuschlag/-rabatt**
  - auf Bestellungen verteilen D-222
  - Importdokument D-157

### H
- **Handlungsablauf**
  - Einkauf D-18

### I
- **Identnummer**
  - Einstellungen D-240
  - Kisten-ID D-237
- **Identnummern**
  - im Wareneingang D-137
- **Importdokument**
  - Bestellungen D-218
  - Buchungsart D-216, D-259
  - Dokumentenstatus D-217, D-260
  - Filtereinstellung D-223
  - Positionen D-219
  - Positionszuordnung D-221
  - Preiskontrolle D-213
  - prüfen D-170
  - Rechnungskontrolle D-259
- **Individualpreis** D-37

### K
- **Kiste**
  - Etikett drucken D-142
  - Kisten-ID D-237
  - virtuelle Positionsnummer D-238
  - Wareneingang D-136, D-230
  - Wareneingang erfassen D-138
- **Kistenbestellung**
  - virtuelle Positionsnummer D-47, D-136
- **Kisten-ID** D-136
  - Einstellungen D-240
- **Kontrolle**
  - elektronisches Dokument prüfen D-170
  - Lieferantenpreise prüfen D-146
  - Lieferantenrechnung D-245
  - Mengendiskrepanzen D-243
  - unvollständige Lieferungen D-243
  - vollständige Lieferungen D-241
  - Wareneingang D-133, D-241
- **Kunde**
  - Individualpreis D-37
- **Kundenauftrag**
  - Anfrage erzeugen D-112
  - Bestellposition erfassen D-54
  - Bestellung D-51
  - Bestellung erzeugen D-68
  - Lieferant ändern D-56

### L
- **Lagerartikel**
  - Lagermaß D-27
- **Lagerbestellung**
  - gemischte Bestellung erfassen D-83
  - Kiste D-136, D-230
  - Wareneingang D-121
- **Lagermaß**
  - in Stammdaten anlegen D-27
  - Lagerartikel D-27
- **Lieferant**
  - AB erfassen D-89
  - für Auftragsposition D-52
  - im Bestellpool ändern D-72
  - in Bestellposition ändern D-56
  - Lieferung anmahnen D-97
  - Preis in AB prüfen D-93
  - Preise vergleichen D-74
  - Preisvergleich D-65
  - Sammel-AB erfassen D-95
  - Stammdaten D-31
- **Lieferanten mahnen** D-225
- **Lieferantenkartei** D-31
  - Standard-Lieferant D-33
- **Lieferantenkartei prüfen** D-33
- **Lieferantenrechnung**
  - importierte Rechnung prüfen D-170
  - Kontrolle D-245
  - prüfen D-146
- **Liefertermin**
  - AB Lieferant D-203
  - ändern D-102, D-105
  - Bestellung D-87
  - im Bestellpool ändern D-72
  - in mehreren Dokumenten ändern D-108
  - Kontrolle und Korrektur D-101
  - Kunden benachrichtigen D-102
  - prüfen D-105
- **Lieferung**
  - buchen D-127
  - Teilmenge D-235
  - Wareneingang D-121
  - Wareneingang mit AB D-199

### M
- **Mahnung**
  - Lieferung D-97
- **Mengendiskrepanzen**
  - prüfen D-133
- **Modul**
  - Funktion D-11

### O
- **openTRANS** D-151
  - Dokumentenexport D-153
  - Dokumentenimport D-155
  - Einstellungen D-166
  - Preiskontrolle D-156
  - XML-Datei D-155

### P
- **Position**
  - im elektr. Dokument zuordnen D-173, D-221
  - Referenzen D-157
- **Preis**
  - in AB prüfen D-93
  - Individualpreis D-37
  - Rechnung prüfen D-146
- **Preiskontrolle**
  - Auftragsbestätigung D-204
  - Bestellungen D-207
  - EK-Rückschreibung D-145
  - elektr. Datei D-213
  - elektr. Dokument D-213
  - importiertes Dokument D-216
  - Position D-210
  - Positionsübersicht D-219
  - Rechnungsdatum D-255
  - Stückliste D-212
- **Produktion**
  - Meldung bei Wareneingang D-122

### R
- **Rechnung**
  - abweichendes Datum D-255
  - prüfen D-146
- **Rechnungskontrolle** D-245
  - Bestellungen D-248
  - Buchungsart D-259
  - Differenz D-251
  - Dokumentenstatus D-260
  - Einkauf D-144
  - elektr. Dokument D-256
  - Fußzuschläge D-145
  - importiertes Dokument D-259
  - Korrektur D-144
  - Positionsübersicht D-251, D-262
  - Stückliste D-253
  - Teilbestellung D-259
  - Teilrechnung D-259
  - Währung D-249
  - Wechselkurs D-249
- **Referenzen**
  - beim Dokumentenimport D-154
- **Referenzierte Bestellung** D-45
- **Rundungsdifferenz** D-158
  - Produktzuordnung D-220

### S
- **Schnittstellenverwaltung**
  - Lieferantendaten prüfen D-178
- **Stammdaten**
  - Firmendaten prüfen D-47, D-136, D-161
  - Lagermaß anlegen D-27
  - Lieferantendaten prüfen D-32
  - Preisdaten prüfen D-38
  - Produktdaten prüfen D-25
  - Status für elektr. Dokumente prüfen D-163
  - Währung prüfen D-162
- **Standard-Lieferant** D-33
- **Status**
  - Bestellungen D-41
  - elektronischer Dokumentenaustausch D-163
  - Vergabe beim elektr. Dokumenten D-160
  - Vergabe beim Wareneingang D-42
  - Wareneingang D-121

### T
- **Teillieferung**
  - aus elektr. Dokument erstellen D-172
  - Wareneingang D-123
  - Wareneingang erfassen D-130
- **Terminüberwachung** D-101

### U
- **Überblick**
  - offene Lieferungen D-243
  - Wareneingang D-133
- **Übergabe**
  - Bestellung D-68
- **Übermenge**
  - Wareneingang D-124
- **Unterposition**
  - Wareneingang Kiste D-237

### V
- **Virtuelle Positionsnummer** D-136, D-238
  - Firmendaten D-47, D-136

### W
- **Währung**
  - elektronischer Datenaustausch D-162
- **Wareneingang** D-227
  - Eingangskontrolle D-125
  - Einstellung für ID D-137
  - erfassen D-127
  - ID für Kiste D-237
  - Kiste D-136, D-230
  - Kisten erfassen D-138
  - komplett erfassen D-128
  - komplette Bestellungen D-241
  - kontrollieren D-133
  - Lagerbestellung D-121
  - Mengendiskrepanzen D-243
  - Mengendiskrepanzen prüfen D-133
  - mit automatischer Kisten-ID erfassen D-138
  - mit manueller Kisten-ID D-141
  - offene Bestellung suchen D-128
  - ohne Lagerkennzeichen D-123
  - Produktionsdatum D-136
  - Status D-42, D-121
  - Teillieferung D-123
  - Teillieferung erfassen D-130
  - Teilmenge D-235
  - Übermenge D-124
  - Unterposition (Kisten) D-237
  - unvollständige Lieferungen anzeigen D-133
  - vollständig D-233
  - Voreinstellungen prüfen D-126

### Z
- **Zuschlag/Rabatt**
  - auf Bestellungen verteilen D-175
  - Zuordnung D-157
