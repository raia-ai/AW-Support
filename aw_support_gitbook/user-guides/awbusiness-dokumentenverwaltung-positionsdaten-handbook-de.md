---
description: "D-HB-AWBusiness_18"
---


# Softwarereferenz: Dokumentenverwaltung

---
## Falz
Falzabzug in mm. Er wird bei der Produktion automatisch bei der Breite und Höhe berücksichtigt. Die Angabe des Falzmaßes ist für Glaser und den Fensterbau wichtig.

Der Falzabzug muss angegeben werden, wenn die vom Kunden genannten Maße das Innenmaß des Fensterrahmens angeben. Da zwischen Glas und Rahmen noch ein Abstand von 4 bis 5 mm benötigt wird, sind die tatsächlichen Glasmaße kleiner als die vom Kunden angegebenen Falzmaße.

## Dok.-Referenz
In einem Original-Dokument wird in diesem Feld der Wert **0** angezeigt. In Dokumenten, die aus einem Original-Dokument erstellt sind, wird die Nummer des Original-Auftrages angezeigt, z. B. in Teillieferungen, Reklamationen, Gutschriften.

## Verkaufspreisvorgaben, Einkaufspreisvorgaben
Für die Berechnung des Auftragswertes können Mindestmengen und Maßrundungen berücksichtigt werden. Sie werden in den Stammdaten des Produktes vorgegeben. Aus den Stammdaten des Kunden werden die entsprechenden Zuschläge herangezogen.

Für den aktuellen Auftrag können die Mindestmengen und die Maßrundungen geändert werden.

⇨ Tutorial, "Berechnungseinstellung" auf Seite C-1399
⇨ Stammdaten, "Preis-Parameter" auf Seite B-718

### Mindestmenge
Abweichende Mindestmenge für diesen Auftrag.

### Maßrundung
Abweichende Maßrundung für diesen Auftrag, nach der die Fläche berechnet werden soll.
Dieser Wert wird bei der Berechnung der technischen Summen berücksichtigt.
⇨ "Summen (technische Parameter)" auf Seite C-1797

## Parameter

### Monatsrechnung
Rechnungen können einzeln, gesammelt oder als Monatsrechnung gedruckt und versendet werden.
- Der Auftrag wird über eine eigene Rechnung abgerechnet.
- Die Rechnung für diesen Auftrag wird in eine Monatsrechnung aufgenommen.

### Sprossennoppen
Die Berechnung von Sprossennoppen wird in den Stammdaten des Kunden hinterlegt. Wenn Sprossennoppen eingebaut werden, können diese wahlweise berechnet werden.
- Die Sprossennoppen werden nicht berechnet.
- In den ISO-Einheiten eingebaute Sprossennoppen sollen berechnet werden.
⇨ "Noppen" auf Seite C-1773

### Gewicht gerundet
Das Gewicht kann für die Berechnung des Energiezuschlags herangezogen werden. Die Berechnung des Energiezuschlags wird in den Stammdaten des Kunden hinterlegt. In den Firmenstammdaten wird übergreifend festgelegt, ob und wie dieser Zuschlag berechnet werden soll.
- Der Energiezuschlag wird nach dem tatsächlichen Gewicht berechnet.
- Der Energiezuschlag wird nach dem gerundeten Gewicht berechnet.
⇨ Stammdaten, "Rundung" auf Seite B-1015
⇨ Stammdaten, "Energiezuschlag nicht nach Positionsgewicht berechnen" auf Seite B-1090

### Zuschläge/Rabatte
In diesem Feld sind die automatischen Zuschläge und Sonderrabatte aufgelistet. Die Zuschläge/Rabatte werden in den Stammdaten im Dialog Produktzuordnung Zuschläge angelegt.
- Der Zuschlag wird nicht berechnet.
- Der Zuschlag wird berechnet.
⇨ Stammdaten, "Sonstigen Zuschlag anlegen" auf Seite B-388
⇨ Stammdaten, "Zuschläge mit gerundeter Menge berechnen" auf Seite B-1091
⇨ Stammdaten, "Produktzuordnung Zuschläge" auf Seite B-1171

## Konditionen / Auftragsvolumen

### Kundenobj.
Durch die Auswahl eines Kundenobjektes werden automatisch die für dieses Objekt hinterlegten Preiskonditionen zur Preisberechnung herangezogen.
Dem Auftrag können alle Objekte zugeordnet werden, die in den Stammdaten zum Kunden angelegt sind.
⇨ Stammdaten, "Objekt-/Abrechnungsverwaltung" auf Seite B-568
⇨ Stammdaten, "Objekte (Kunde, Lieferant)" auf Seite B-952

### Lieferant
Standardmäßig werden die Bestellungen an den Lieferanten übergeben, der den betreffenden Produkten als Standard-Lieferant zugeordnet ist.
⇨ Stammdaten, "Lieferantenkartei" auf Seite B-987
Wenn Sie einen Lieferanten eintragen, werden die Bestellungen aus diesem Auftrag nur an diesen übergeben.
Wenn Sie die Änderung speichern, können Sie über die Abfrage entscheiden, ob der gesamte Auftrag bestellt werden soll oder nur die Bestellartikel.
Wenn Sie die Abfrage mit [Ja] bestätigen, wird die Beschaffungsart für alle Positionen auf Bestellartikel gesetzt.
⇨ Stammdaten, "Produktkennzeichen" auf Seite B-725

### Name
Name des eingetragenen Lieferanten.

### Lief.-objekt
Wenn Sie für ein bestimmtes Bauvorhaben besondere Konditionen mit Ihrem Lieferanten vereinbart haben, können Sie für diesen Auftrag das Lieferantenobjekt auswählen.
⇨ Stammdaten, "Objekte (Kunde, Lieferant)" auf Seite B-952

### Rech.legung
Der Tag der Rechnungslegung bildet die Basis für die Berechnung des Zahlungsziels.
Die Angabe legt den Tag fest, ab dem das Zahlungsziel berechnet werden soll, z. B. bedeutet 5, dass der 5. des Monats die Basis für die Berechnung sein soll.
⇨ Tutorial, "Fälligkeiten" auf Seite C-1469

### Zahltag 1., 2., 3.
Zahltag für die Berechnung des Zahlungsziels.
⇨ Stammdaten, “Fälligkeitsberechnung" auf Seite B-905

### Währung
Sie können für diesen Auftrag eine andere Währung einstellen als diejenige, die aus den Kundendaten übernommen wurde. Die Preise können in der gewählten Währung ausgewiesen werden.
⇨ Stammdaten, “Währungseinstellungen" auf Seite B-1059
⇨ Stammdaten, “Währungsanzeige in Auftragserfassung" auf Seite B-1060

### Kurs
Wenn für die gewählte Währung in den Stammdaten ein Kurs hinterlegt ist, wird dieser angezeigt und kann überschrieben werden.

### Kurs fixiert für Rechnungsdruck
Wenn Sie einen Kurs eingetragen haben, wird dieser für den Rechnungsdruck herangezogen. Wenn kein Kurs eingetragen ist, wird der Kurs aus den Stammdaten herangezogen.
Werden die Rechnungen für den Kunden als Sammelrechnung ausgegeben, wird eine Abfrage angezeigt, wenn Sie die Einstellung ändern. Sie können dann entscheiden, ob der aktuelle Kurs aus der Sammelrechnung herausgenommen werden soll.
- Standardmäßig wird zur Berechnung der jeweils aktuelle Kurs aus den Stammdaten herangezogen.
- Der aktuelle Kurs wird fixiert und zum Rechnungsdruck herangezogen, unabhängig davon, ob dieser in den Stammdaten nach dem Erstellen des Auftrags geändert wurde.

## Kopfdaten - Texte
**Dokumente > Auftrag > Auftrag auswählen > Register Kopfdaten > Register Texte**

[Image: Screenshot of the 'Kopfdaten - Texte' tab. It shows a block overview section, a text block with editing tools, and a list of documents at the bottom. The text block contains a sample message to a customer with a discount table.]

> **Textnummern nicht versehentlich ändern**
> Um versehentliches Überschreiben von (Standard-) Texten und Textnummern zu vermeiden, sollten Sie die Option Nachfrage bei Änderung der Textnummer aktivieren.
> ⇨ "Menü Optionen" auf Seite C-1684

In diesem Register können Sie Mitteilungen für den Auftrag hinzufügen, die z. B. für den Kunden, die Produktion oder den Versand wichtig sind.
⇨ Tutorial, "Text erfassen" auf Seite C-1308

### Blockübersicht
- **Nummer**: Sie können einen Standardtext auswählen, indem Sie die Textnummer eingeben. Wenn Sie für diesen Auftrag einen manuellen Text eingeben wollen, dann lassen Sie 0 stehen.
- **Schaltflächen**: Mit den Schaltflächen können Sie einen Text hinzufügen oder entfernen.
  ⇨ Tutorial, "Text erfassen" auf Seite C-1308
- **Textkennz.**: Das Textkennzeichen steuert, in welchen Formularen der Text gedruckt wird. Wenn Sie einen Text auswählen, wird das Textkennzeichen automatisch angezeigt. Wenn Sie das Textkennzeichen wechseln, wird der Text dem neuen Kennzeichen entsprechend auf den Formularen gedruckt.
  ⇨ Stammdaten, "Textkennzeichen" auf Seite B-1188
  ⇨ Stammdaten, "Texte" auf Seite B-1189
- **Manuell geändert**: Die Checkbox wird automatisch markiert, wenn Sie einen neuen Text hinzufügen oder einen hinzugefügten Text löschen.
- **Übersicht (Tabelle)**: In der Tabelle werden alle Texte angezeigt, die dem Auftrag angefügt sind.

### Textblock
- **Schaltflächen**: Sie können die Schriftart und -größe ändern und Hyperlinks, Bilder und Tabellen einfügen.
  ⇨ Tutorial, "Text erfassen" auf Seite C-1308
- **Textfeld**: Das Textfeld wird freigeschaltet, wenn Sie auf die Schaltfläche zum Hinzufügen eines Textes klicken. Schreiben Sie direkt in das Textfeld, wenn Sie einen Text eingeben oder ändern möchten.

## Kopfdaten – Anlagen
**Dokumente > Auftrag > Auftrag auswählen > Register Kopfdaten > Register Anlagen**

[Image: Screenshot of the 'Kopfdaten - Anlagen' tab. It shows a file attachment section where users can add, remove, and view attachments with remarks.]

In diesem Register können Sie Dateien als Anhang hinzufügen. Alle Anhänge werden in der Liste angezeigt. Pro Kunde wird ein Ordner angelegt, in dem Kopien der Dokumente gespeichert sind. Den Pfad für den Speicherort legen Sie in den Firmendaten fest.
⇨ Stammdaten, "Dateianhänge" auf Seite B-1071
⇨ Tutorial, "Dokumente anhängen" auf Seite C-1311
Zu jedem Dateianhang können Sie eine Bemerkung eintragen. Häufig verwendete Bemerkungen können in den Stammdaten hinterlegt werden und stehen in der Kombobox zur Verfügung.
⇨ Stammdaten, "Dateianhangs-Bemerkungen" auf Seite B-1194

## Kopfdaten - Technische Parameter
**Dokumente > Auftrag > Auftrag auswählen > Register Kopfdaten > Register Technische Parameter**

[Image: Screenshot of the 'Technische Parameter' tab. It shows various sections including Identifikation, Anschrift, Abstandhaltervorgabe, Produktionsetiketten, and Forderungen.]

In diesem Register legen Sie Details zu den Abstandhaltern und zu den Produktionsetiketten fest. Sie überschreiben damit die Vorgaben aus den Stammdaten.
Die Felder in den Bereichen **Identifikation** und **Anschrift** sind ausführlich zum Register Dokumente beschrieben.
⇨ "Kopfdaten - Dokument" auf Seite C-1688

### Abstandhaltervorgabe
Die Vorgaben aus den Stammdaten des Kunden werden bei der Erfassung von ISO-Produkten herangezogen. Diese Angaben können im Auftrag geändert werden.
⇨ Stammdaten, “Abstandhaltervorgaben” auf Seite B-917

**Typ**: Auswahl des Abstandhaltertyps, der in diesem Auftrag für ISO-Einheiten verwendet werden soll.

**Farbe**: Auswahl der Farbe, die für den Abstandhalter verwendet werden soll. Diese Angabe wird beim Erfassen von Abstandhaltern geprüft und ggf. eine Meldung angezeigt, wenn die Farbvariante nicht zur Verfügung steht.

**Rahmentext**: Standardmäßig wird der Rahmentext, der im Abstandhalter gedruckt werden soll, aus den Stammdaten übernommen. Sie können ihn für diesen Auftrag ändern.
⇨ Stammdaten, "Rahmentexte" auf Seite B-536

### Produktionsetiketten
**Layout**: Für den Druck von Etiketten werden die Angaben aus den Kundendaten herangezogen. Die Nummer des Layouts wird an den Etikettendrucker übergeben.
⇨ Stammdaten, "Produktionsetiketten" auf Seite B-916

**Etikettenparameter**: Sollen Etiketten aus dem Auftrag gedruckt werden, muss pro Auftrag festgelegt werden, wie viele Etiketten bei den ISO-Einheiten gedruckt werden sollen.
- **Keine**: Es werden keine Etiketten gedruckt.
- **Pro Einheit**: Pro ISO-Einheit wird ein Etikett gedruckt, z. B. bei vier ISO-Einheiten mit gleichem Aufbau werden vier Etiketten gedruckt.
- **Pro Position**: Pro Position wird unabhängig von der Stückzahl ein Etikett gedruckt.
⇨ Stammdaten, "Formularverwaltung" auf Seite B-1195
⇨ "Formular-/Etikettendruck - Etiketten" auf Seite C-1933

### Forderungen
Rahmenaufträge werden über Forderungen abgerechnet. Zu jeder Forderung(srechnung) wird ein Produktionsauftrag erstellt.

**Nummer**: Nummer der Forderung, zu der dieser Produktionsauftrag erstellt wird.

**Auftragsnr.**: Nummer des Rahmenauftrags, zu der dieser Produktionsauftrag erstellt wird.

## Kopfdaten – Kundeninfo
**Dokumente > Auftrag > Auftrag auswählen > Register Kopfdaten > Register Kundeninfo**

[Image: Screenshot of the 'Kundeninfo' tab. It shows customer information, including general info and a pop-up dialog for adding annotations.]

In diesem Register werden allgemeine Informationen zum aktuellen Kunden und zu den angehängten Anlagen angezeigt, die für den Kunden gelten. Die Angaben werden aus den Stammdaten übernommen. Zusätzlich können Sie Anmerkungen zu dem Auftrag speichern.
⇨ Stammdaten, "Spezifikation" auf Seite B-891
Die Felder in den Bereichen **Identifikation** und **Anschrift** sind ausführlich zum Register Dokumente beschrieben.
⇨ "Kopfdaten - Dokument" auf Seite C-1688

### Information
- **[Kundeninfo]**: Im Feld Information werden die allgemeinen Informationen angezeigt, die aus den Stammdaten übernommen werden.
- **[Anmerkung (...)]**: Im Feld Information wird eine Übersicht über alle Anmerkungen angezeigt, die für den Auftrag angelegt sind.
- **[Neue Anmerkung ...]**: Mit dieser Schaltfläche öffnen Sie den Dialog Manuellen Eintrag hinzufügen, in dem Sie eine Anmerkung zu dem Auftrag hinzufügen können.

# Positionsdaten
**Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Positionen**

Die Positionserfassung und die zugehörigen Menüs sind für alle Dokumentenarten gleich. Sie wird in dieser Anleitung am Beispiel **Auftrag** beschrieben.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menüs in der Positionserfassung" auf Seite C-1711
- "Dokument - Positionen" auf Seite C-1724

## Menüs in der Positionserfassung
**Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Positionen**

Über die Menüs der Positionserfassung können Sie die Standardeinstellung des Dialoges bestimmen und andere Dialoge öffnen, ohne die Positionserfassung zu schließen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Start" auf Seite C-1712
- "Menü Ansicht" auf Seite C-1712
- "Menü Funktionen" auf Seite C-1714
- "Menü Optionen" auf Seite C-1717
- "Menü Aufbau" auf Seite C-1722
- "Menü Customizing" auf Seite C-1723

### Menü Start
**Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Positionen > Menü Start**

Die Standard-Menüeinträge sind im Part Überblick erklärt.
⇨ Überblick, "Benutzeroberfläche" auf Seite A-26

Das Menü ist in folgende Gruppen gegliedert:
- Gruppe Preise
- Gruppe Konditionen
- Gruppe Dokument
- Gruppe Position
- Gruppe Produktion
- Gruppe Kapazitätsübersicht

#### Gruppe Druck
**Dokumente > Auftrag > Auftrag auswählen > Menü Start > Gruppe Druck**
Diese Gruppe ist nur im Register **Kopfdaten** freigeschaltet.
⇨ "Gruppe Druck" auf Seite C-1679

#### Gruppe iTOE
**Dokumente > Auftrag > Auftrag auswählen > Menü Start > Gruppe iTOE**
Diese Gruppe ist nur im Register **Positionen** freigeschaltet.
Öffnet den Dialog Produktabgleich, oder den A+W CAD Designer (Shapes), um die die importierte SN-Datei zu prüfen und/oder Regel zu definieren.
⇨ "Produktabgleich" auf Seite C-1874

### Menü Ansicht
**Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Positionen > Menü Ansicht**

Das Menü ist in folgende Gruppen gegliedert:
- Gruppe Preise
- Gruppe Konditionen
- Gruppe Dokument
- Gruppe Position
- Gruppe Produktion
- Gruppe Kapazitätsübersicht

#### Gruppe Preise
In der Positionserfassung werden die Preise standardmäßig als Verkaufspreise (VK) angezeigt. In der Spalte Schlüssel werden VK-Schlüssel zur Auswahl angeboten. Über die das Menü Ansicht können Sie die Preisanzeige umstellen:

- **EK (Einkaufspreise)**: Die Einkaufspreise der einzelnen Komponenten werden angezeigt. In der Spalte **Schlüssel** werden EK-Schlüssel zur Auswahl angeboten. Im Feld **Preis/PE** wird der Preis für die Hilfsstoffe angezeigt. Alle manuellen Änderungen beziehen sich auf die Einkaufspreise.
  ⇨ Stammdaten, "EK-Kalkulation" auf Seite B-765
- **FW (Preise in Fremdwährung)**: Die Verkaufspreise werden in Fremdwährung angezeigt. Die Eingabefelder **Schlüssel**, **Preis/PE**, **Einheit** und **Rabatt** werden gesperrt.
- **Euro (Preise in Euro)**: Diese Einstellung ist für die Staaten wichtig, die kurz vor der Umstellung auf die Währung Euro stehen. Die Preise werden in Euro angezeigt, wenn Sie die Preislisten in einer Fremdwährung führen. Die Eingabefelder **Schlüssel**, **Preis/PE**, **Einheit** und **Rabatt** werden gesperrt.

> **Umschaltung der Preise ist nicht möglich**
> Diese Umschaltung ist nicht möglich, wenn in den Firmendaten die Option **Keine Währung** aktiviert ist.
> ⇨ Stammdaten, "Währungsanzeige in Auftragserfassung" auf Seite B-1060

#### Gruppe Konditionen
- **Konditionen**: Öffnet den Dialog **Konditionen/Individueller Preis**, um Informationen über individuelle Preise und Rabatte zu erhalten.
  ⇨ "Konditionen" auf Seite C-1881
- **Preis-/Konditionsinformation**: Öffnet den Dialog, um Informationen über Preise und Rabatte zur markierten Position zu erhalten. Dieser Eintrag ist nur kundenspezifisch freigeschaltet.

#### Gruppe Dokument
- **Dokument anzeigen**: Öffnet den Dialog **Dokumentenansicht** als Vorschau auf das Dokument.
  ⇨ "Dokument anzeigen" auf Seite C-1829
- **Kundeninfo**: Öffnet einen Dialog mit einer Kurzinfo zum Kunden.
  ⇨ "Kundeninfo" auf Seite C-1830

#### Gruppe Position
- **Artikelinfo**: Öffnet einen Dialog mit Details zum aktuellen Produkt.
  ⇨ "Artikel-Informationen" auf Seite C-1887

#### Gruppe Produktion
- **Produktionsübersicht**: Über diese Option können Sie sich eine Übersicht über die Rückmeldungen aus der Produktion anzeigen lassen.
  ⇨ "Übersicht Statusrückmeldung" auf Seite C-1860

#### Gruppe Kapazitätsübersicht
Diese Gruppe ist nur freigeschaltet, wenn Sie mit A+W Business Capacity Planner und A+W Capa View arbeiten.
Über diese Option können Sie sich eine Übersicht über die freien und belegten Kapazitäten aus A+W Business Capacity Planner anzeigen lassen.
⇨ "Kapazitätsübersicht" auf Seite C-1831

#### Gruppe Bearbeitungen/Modelle
Die Gruppe ist nur für das Register **Modelle/Bearbeitungen** freigeschaltet. Mit den Schaltflächen wählen Sie die Darstellung im aus.
- Standard
- Skizze vergrößern
- ohne Stückliste
- Stückliste rechts unten

### Menü Funktionen
**Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Positionen > Menü Funktionen**

Die Gruppen sind im Kapitel **Dokumentenverwaltung** beschrieben.
Das Menü ist in folgende Gruppen gegliedert:
- "Gruppe Dokument" auf Seite C-1681
- "Gruppe Dokumentenübersicht" auf Seite C-1682
- "Gruppe Info" auf Seite C-1682
- "Gruppe Kapazitäten" auf Seite C-1683
- "Gruppe Finanzen" auf Seite C-1683
- "Gruppe Kalkulation" auf Seite C-1683
- "Gruppe Optimierung" auf Seite C-1684
- "Gruppe Position" auf Seite C-1714
- "Gruppe Einkauf" auf Seite C-1716

#### Gruppe Position
- **Schnellanfrage**: Öffnet den Dialog **Schnellanfrage**, um eine (telefonische) Kundenanfrage aufzunehmen, ohne den aktuellen Auftrag zu schließen.
  ⇨ "Schnellanfrage" auf Seite C-1871
- **Reklamation**: Öffnet den Dialog **Reklamation**, um für die markierte Position eine Reklamation zu erfassen.
  ⇨ "Reklamationen" auf Seite C-1875
- **Zusatz Stückliste**: Öffnet den Dialog **Ergänzungen**, um zu einer Stücklisten-Komponente eine Kostenstelle und Kostenart einzutragen. Die Funktion ist nur freigeschaltet, wenn Sie im Register **Stückliste** eine Komponente markiert haben.
  ⇨ "Zusatz Stückliste - Ergänzungen" auf Seite C-1892
- **Lagersuche**: Öffnet den Dialog **Lagerinfo** um den aktuellen Bestand des gewünschten Produkts zu prüfen.
  ⇨ "Lagerinfo" auf Seite C-2034
- **SNEditor**: Dieser Eintrag ist nur freigeschaltet, wenn auf Ihrem System auch A+W CAD Designer installiert ist. Sie können damit Sprossenmuster und Modelle weiterbearbeiten.
- **Versicherungspreise**: Über diese Funktion erfassen Sie Versicherungsleistungen für eine Position.
  ⇨ "Versicherungsleistung" auf Seite C-1899
- **Vorgaben Position löschen**: Alle manuellen Preis- und Rabatteingaben der markierten Position werden gelöscht. Die Preise und Rabatte aus den Stammdaten werden wieder übernommen.
- **Vorgaben Stücklistenposition löschen**: Nur die manuellen Preis- und Rabatteingaben für die markierte Stücklisten-Komponente werden gelöscht. Die Preise und Rabatte aus den Stammdaten werden wieder übernommen.
- **Positionspreisvorgabe löschen**: Die manuellen Preiseingaben der markierten Position werden gelöscht. Der Preis aus den Stammdaten wird wieder übernommen.
- **Dokumentenreferenzvorgabe löschen**: Die Referenzen werden für Auftragsbestätigungen, Rechnungen und Lieferavis eingetragen. Diese Referenzen werden für den Datenaustausch mit openTRANS gebraucht.
- **Preisvorgaben auf nachfolgende Positionen übertragen**: Die Preise aus der markierten Position werden auf alle nachfolgenden Positionen übertragen.
- **Gesperrte Position ändern**: Diese Funktion ist nur freigeschaltet, wenn Sie eine bestellte Position ändern möchten. In der Erfassungszeile werden die Felder **Produkt**, **Stück**, **Höhe** und **Breite** freigeschaltet. Die (geänderte) Bestellung wird automatisch in den Bestellpool übergeben, wenn Sie die Positionserfassung schließen.
  ⇨ "Bestellübergabe - Bestellpool" auf Seite C-1946
- **Preisrecorder**: Öffnet den Dialog **Preisrecorder**, um die Preise des erfassten Produkts über einen bestimmten Zeitraum prüfen.
  ⇨ "Preisrecorder" auf Seite C-1893
- **Begründung für manuelle Preisvorgabe**: Bei manuellen Preisänderungen muss eine Begründung eingegeben werden. Diese Funktion ist nur freigeschaltet, wenn in den Firmendaten die zugehörige Checkbox markiert ist.
  ⇨ Stammdaten, "Erweiterte Preisfindung (Referenzpreis, manuelle Änderung)" auf Seite B-1092
- **Artikel fixieren**: Öffnet den Dialog **Artikel fixieren**, in dem Sie die Position z. B. als kundenindividuellen Artikel (Produkt) speichern können.
  ⇨ "Artikel fixieren" auf Seite C-1895
- **Preis/Konditionen fixieren**: Die Preise und Rabatte eines fixierten (kundenindividuellen) Produktes werden fixiert und können nicht mehr geändert werden.
- **Kosten- und Aufschlagskalkulation**:
    - **Übersicht**: Der Dialog **Kosten- und Aufschlagskalkulation** wird geöffnet, in dem Sie die Kalkulation prüfen können.
      ⇨ "Kosten- und Aufschlagskalkulation (Position)" auf Seite C-1898
    - **Detail - Position**: Der Dialog **Kosten- und Aufschlagskalkulation** wird in einer Detail-Ansicht zur markierten Position geöffnet.
    - **Detail - Stückliste**: Der Dialog **Kosten- und Aufschlagskalkulation** wird in einer Detail-Ansicht zur Stückliste der markierten Position geöffnet.
    - **Löschen und neu berechnen**: Die Preise der markierten Position werden gelöscht und neu berechnet.
- **Kopie aus Position...**: Öffnet den Dialog **Kopie erstellen aus...**, um die Werte einer Position auf die markierte Position zu übertragen.
  ⇨ "Position kopieren" auf Seite C-1896
- **Preisberechnung starten**: Über diese Funktion starten Sie die Preisberechnung für die markierte Position.
  ⇨ "Preise und Preisberechnung" auf Seite C-1398

#### Gruppe Einkauf
Diese Gruppe ist nur im Register **Positionen** freigeschaltet.
- **Anfrage für Position**: Öffnet den Dialog **Preisvergleich**, um nach dem günstigsten Angebot für eine Position zu suchen.
  ⇨ "Preisvergleich" auf Seite C-1951
- **Anfrage für Dokument**: Preisvergleich, um nach dem günstigsten Angebot für ein Dokument zu suchen.
  ⇨ "Preisvergleich" auf Seite C-1951

### Menü Optionen
**Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Positionen > Menü Optionen**

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

> **Aktivierte Optionen nach dem Öffnen des Dialogs**
> Bitte beachten Sie, dass geänderte Optionen erst beim nächsten Öffnen des Dialogs wirksam werden.
> Wenn durch eine aktivierte Option eine Prüfung gestartet wurde, kann sich das Öffnen eines Dokuments verzögern. Der Grad der Verzögerung hängt von der Leistungsfähigkeit des Rechners ab.
> Die folgenden Beschreibungen stellen die aktivierte Option dar.

Das Menü ist in folgende Gruppen gegliedert:
- Gruppe Dokumente
- Gruppe Positionen
- Gruppe Bearbeitungen/Modelle
- Gruppe Sprossen

#### Gruppe Dokumente
Diese Gruppe ist im Kapitel **Dokumentenverwaltung** beschrieben.
⇨ "Gruppe Dokumente" auf Seite C-1684

#### Gruppe Positionen
Folgende Einträge werden angezeigt:
- **Übernahme bei Neuerfassung**:
    - Sprossen übernehmen
    - Modelle übernehmen
    - Zuschläge/Bearbeitungen übernehmen
    - Gase übernehmen
  Die markierten Stücklisten-Komponenten werden immer in die nächste Position übernommen. Sie können danach bearbeitet oder gelöscht werden.
- **Zusätzliches Produktfeld**: Sie können sich ein zusätzliches Feld für die Produktnummer anzeigen lassen. Das zusätzliche Feld wird hinter dem Datenfeld für die Dicke des Glases angezeigt, wenn Sie in der Positionserfassung im Bereich **Positionen** eine Produktnummer eingeben oder ändern. Mit dieser Option haben Sie bei der Schnellerfassung von Aufträgen einen Überblick über die eingegebene Produktnummer.
- **Abstandhalter und Gase bei Eingabe von neuem Hauptprodukt beibehalten**: Bei der Änderung eines Hauptprodukts werden die Abstandhalter und Gase nicht gelöscht oder geändert.
- **CPIP-Code in der Stückliste anzeigen**: Der CPIP-Code wird in der Stückliste angezeigt. Diese Funktion wird nur in Frankreich benötigt.
- **Glas-, Gas-und SZR-Zuschl. löschen bei Pr./Einh.-Vorgabe (auch franz. Preisber.)**: Wenn Sie in einer ISO-Position ein Glas, Gas oder einen SZR austauschen und einen manuellen Preis für die Position eintragen, werden die entsprechenden Zuschläge gelöscht. Diese Option kann übergreifend in den Firmendaten aktiviert werden.
  ⇨ Stammdaten, "Glas-, Gas- und SZR-Zuschl. löschen bei Pr./Einh.-Vorgabe (nicht bei franz. Preisber.)" auf Seite B-1091
- **Mengeneingabe für aktuelle Position**: Die Menge (Fläche/Gewicht) kann für die aktuelle Position eingegeben werden.
- **Weitere Angaben übernehmen**: Die Einträge aus dem Register **Weitere Angaben** für die vorherige Position werden automatisch in die neue Position übernommen.
- **Automatischer Laschenwechsel auf**:
    - Stückliste
    - Zusatz
    - Texte
    - Weitere Angaben
  Mit der `<Tab>`-Taste springen Sie aus der Erfassungszeile direkt in das gewählte Register.
- **Reklamationsgrund und -verursacher nicht übernehmen**: Bei Reklamationen werden Reklamationsgrund und -verursacher nicht automatisch aus der vorherigen Position übernommen.
- **Automatische Lagersuche bei Lagerartikel**: Wenn Sie einen Lagerartikel erfasst haben, wird der Dialog **Lagerinfo** geöffnet.
  ⇨ "Lagerinfo - Lagersuche" auf Seite C-2035
- **Lagersuche im Auswahlmodus starten**: Der Dialog **Lagersuche** wird im Auswahlmodus gestartet. Sie starten die Suche manuell nachdem Sie die Suchkriterien eingegeben haben. Dadurch wird die Treffermenge verringert und die Geschwindigkeit der Abfrage wird erhöht.
- **Lagersuche auf Abmessung einschränken**: Im Dialog **Lagersuche** wird zusätzlich zur Artikelnummer die Abmessung in die Abfrage der Lagersuche übernommen. Dadurch wird die Geschwindigkeit der Abfrage erhöht.
- **Keine Meldung bei Fehlern in Preisfindung**: Fehler bei der Preisfindung werden nicht gemeldet. Sie sollten diese Option deaktivieren, da Sie sonst keine Fehler bei den Preisen bemerken.
- **Meldung wenn kein EK-Austauschzuschlag vorhanden**: Wenn Sie Gläser tauschen, werden fehlende EK-Austauschzuschläge beim Schließen der Positionserfassung gemeldet.
- **Meldung wenn kein Stücklistenpreis vorhanden**: Wenn Sie die Stückliste bearbeitet haben, werden fehlende Preise beim Schließen der Positionserfassung gemeldet.
- **Meldung bei Bestandsunterschreitung**: Wenn Sie die Positionserfassung schließen, wird eine Meldung dafür angezeigt, dass mehr Mengen erfasst wurden, als im Lager aktuell vorhanden sind. Sie können sich eine Meldung anzeigen lassen, wenn der kritische Bestand unterschritten ist oder wenn der Mindestbestand unterschritten ist. Darüber hinaus kann eine Verfügbarkeitsprüfung zum Zeitpunkt des Produktionsstarts aktiviert werden. Dadurch werden die Mindestbestände nur an diesem Termin geprüft. Geplante Lagerzugänge und Abgänge werden zu diesem Termin aufgerechnet und mit dem Ergebnis die Prüfung durchgeführt.
- **Nicht sichern bei Restriktionsfehlern**: Wenn Sie bei der Erfassung Restriktionen verletzt haben, wird eine Meldung angezeigt und die Position kann nicht gespeichert werden. Sie müssen dann die erfassten Werte entsprechend ändern.
- **Meldung bei Glasartikel ohne Abmessung**: Wenn Sie Gläser ohne Maße erfasst haben, wird eine Meldung angezeigt.
- **Übernahme der vorgeg. Flächen in Austauschzuschlägen**: Wenn Sie Gläser getauscht haben, werden die eingetragenen Flächen für die Berechnung der Austauschzuschläge herangezogen. Diese Option sollten Sie nutzen, wenn Sie die Option **Mengeneingabe für aktuelle Position** aktiviert haben.
- **Rabatt löschen bei manueller Preisvorgabe**: Wenn Sie die Preise manuell geändert haben, werden die Rabatte auf null gesetzt.
- **Preisberechnung nur beim Speichern**: Die Preisberechnung wird standardmäßig sofort durchgeführt, wenn die Position erfasst wird. Mit dieser Option wird die Preisberechnung für alle erfassten Positionen erst beim Speichern der Position durchgeführt. Damit verbessern Sie die Performance bei Aufträgen mit vielen Positionen.
- **Ermittlung der Beschaffungsart nur beim Speichern**: Standardmäßig wird die Beschaffungsart berechnet, wenn die Position erfasst wird. Mit dieser Option wird die Beschaffungsart für alle erfassten Positionen erst beim Speichern der Position ermittelt. Damit verbessern Sie die Performance bei Aufträgen mit vielen Positionen.
- **Keine Rückrechnung der automatischen Zuschläge**: Automatische Zuschläge werden nicht in Positionen zurückgerechnet.
- **Meldung bei fehlender Leistungserklärung**: Mit dieser Option wird eine Fehlermeldung ausgegeben, wenn zu einem Produkt keine Leistungserklärung vorhanden ist. Diese Option ist nur bei Dokumentenart **Auftrag** aktiviert.
- **Bearbeitungsparameter prüfen**:
    - Mindestens ein Parameter gesetzt
    - Alle prüfen
  Die Parameter werden entsprechend der aktivierten Option während der Eingabe geprüft. Je mehr Parameter Sie aktiviert haben, umso mehr belasten Sie die Datenverarbeitung.
- **Textpositionierung**:
    - Texte vor Position
    - Texte nach Position
- **Texte produktbezogen**: Mit dieser Option legen Sie die Standardeinstellung für die Position eines eingefügten Textes fest. Im Register **Texte** kann diese Einstellung pro Auftragsposition und Text geändert werden.
  ⇨ "Vor, nach Position, produktbezogen" auf Seite C-1791
- **Texte standardmäßig beibehalten**: Die Checkbox **Text beibehalten** im Register **Texte** der Positionserfassung ist standardmäßig aktiviert.
- **Einkauf**:
    - **Bestellartikel melden**: Auf Bestellartikel in einer Position wird automatisch mit einer Meldung hingewiesen.
    - **Statusänderung melden bei Bestellübergabe**: Wenn Bestellartikel erneut in die Bestellung übergeben werden, wird vor der Statusänderung des Auftrags eine Abfrage angezeigt.
    - **Produktbezeichnung aus Lieferantenkartei**: Für die Bestellung wird die Produktbezeichnung aus der Lieferantendatei übernommen.
- **Artikelsuche kundenindividuell**: Wenn Sie Produkte über die Suche einfügen wollen, werden auch die kundenindividuellen Produkte des aktuellen Kunden angezeigt.
- **Stücklistenbild Dickenanzeige**: Mit dieser Option können Sie sich die Dicke der einzelnen Stücklistenelemente der markierten Position anzeigen lassen. Die Dicke der Stücklistenelemente wird in der Seitenansicht im Register **Position** der Positionserfassung angezeigt.
- **ATP Anfrage nach Positionserfassung**: Die ATP-Anfragen sind nur kundspezifisch freigeschaltet. Der Dialog kann automatisch beim Verlassen der Positionserfassung aufgerufen werden, wenn mindestens eine Position verändert wurde.
- **Farbsuchdialog öffnen mit F4**: Mit dieser Option kann der Dialog zur Suche nach Produktvarianten (Farben) mit der `<F4>` geöffnet werden.

#### Gruppe Bearbeitungen/Modelle
Die Optionen sind nur im Register **Modelle/Bearbeitungen** freigeschaltet. Folgende Einträge werden angezeigt:
- **Alle Kanten markieren bei Neuerfassung**: Bei der Erfassung eines neuen Modells werden immer alle Kanten für die Bearbeitungen markiert. Die Markierung kann anschließend geändert werden.
- **Nachfrage, ob tangentiale Kanten markiert werden sollen**: Wenn die vorausgehende Option markiert ist, wird bei runden Kanten eine Abfrage zur automatischen Markierung angezeigt.
- **Mehrfach-Erfassung als Standard bei Neuerfassung**: Bei der Mehrfach-Erfassung kann bei den Bearbeitungen in der Regel nur die Menge eingegeben werden. Die Angabe von Maßen ist nicht möglich. Diese Einstellung eignet sich insbesondere für Angebote, bei denen die genauen Maße von Bearbeitungen nicht relevant sind.
    - Bei der Standard-Erfassung können alle Parameter eingegeben werden. Während der Erfassung der Bearbeitung kann der Modus über die Checkbox **Multi** geändert werden. Die Einstellung wird pro Dokumententyp und Mitarbeiter gespeichert.
- **Modell durch Doppel-Klick auswählen**: Standardmäßig können die Modelle durch einen einfachen Klick ausgewählt werden. Wenn diese Option aktiviert ist, wird ein Modell mit einem Doppel-Klick ausgewählt.
- **Keine automatische Neuanlage**: Standardmäßig wird mit einem Klick auf ein Stücklistenelement in der Bearbeitungserfassung automatisch eine Bearbeitung angehängt. Wenn diese Option aktiviert ist, müssen Sie zum Anhängen einer Bearbeitung an einem Stücklistenelement den Menüpunkt **Neu** auswählen.
- **Neuerfassung als Standard**: Beim Erfassen von Bearbeitung kann automatisch in den Erfassungsmodus gewechselt werden.
- **1. Feld ist Modellnummer**: Die Modellnummer wird in der Modellerfassung als 1. Feld angezeigt.
- **1. Feld ist Produktnummer**: Die Produktnummer wird in der Modellerfassung als 1. Feld angezeigt.
- **Selektierte Bearbeitung hervorheben**: Die ausgewählte Bearbeitung wird in der Anzeige farblich hervorgehoben.

#### Gruppe Sprossen
Die Optionen sind nur im Register **Sprossen** freigeschaltet. Folgende Einträge werden angezeigt:
- Bohrpunktsymmetrisch:
- Feldsymmetrisch:
- Bohrpunkt-asymmetrisch:
- Feld-asymmetrisch:
Je nach gewählter Option sind standardmäßig die entsprechenden Felder aktiviert und freigeschaltet.
- **Waagerechte auf senkrechte Sprossen übernehmen**: Bei der Erfassung von Sprossen wird die Artikelnummer der waagerechten Sprossen automatisch für die senkrechten Sprossen übernommen.
    - Mit dieser Einstellung können Sie festlegen, dass dieses Verhalten beibehalten wird, wenn Sie nachträglich die waagerechten Sprossen ändern.
    - Wenn Sie Option nicht auswählen, werden die senkrechten Sprossen nicht geändert, wenn Sie für die waagerechten eine andere Artikelnummer eintragen.

### Menü Aufbau
**Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Positionen > Menü Aufbau**

Über dieses Menü können Sie die Ebenen eines Glases festlegen und Makros für Bearbeitungen verwalten.

Das Menü ist in folgende Gruppen gegliedert:
- Gruppe Struktur
- Gruppe Beschichtung
- Gruppe Makro

#### Gruppe Struktur
- **Struktur Ebene 1 – 6**: Die Strukturseite des markierten Glases wird auf die gewählte Ebene gedreht. Sie können die Ebenen auch über das Register **Position** im Bereich **Preis** drehen.

#### Gruppe Beschichtung
- **Beschichtung Ebene 1 – 6**: Die Beschichtungsseite des markierten Glases wird auf die gewählte Ebene gedreht. Sie können die Ebenen auch über das Register **Position** im Bereich **Preis** drehen.

#### Gruppe Makro
- **Sichern**: Öffnet den Dialog **Makro**, um die Daten der markierten Position als Makro zu speichern.
  ⇨ Tutorial, "Makro speichern" auf Seite C-1420
  ⇨ "Makro sichern" auf Seite C-1908
- **Löschen**: Öffnet den Dialog **Makro**, um ein Makro zu löschen.
- **Ändern**: Öffnet den Dialog **Makro-Änderung**, um ein Makro zu bearbeiten.
  ⇨ "Makro ändern" auf Seite C-1909
- **Suchen**: Öffnet den Dialog **Makrosuche**, um ein bestimmtes Makro auszuwählen.
  ⇨ "Makro suchen" auf Seite C-1911
- **Kopieren**: Öffnet den Dialog **Makros kopieren**, um ein Makro zu kopieren.
  ⇨ "Makro kopieren" auf Seite C-1912
- **Nur Produktaufbau aus Makros übernehmen**: Bei der Eingabe einer Position über die Makro-Funktion werden die Preise nicht übernommen.

### Menü Customizing
**Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Positionen > Menü Customizing**

Diese Funktionen werden für Anpassungen in den Dialogen verwendet.
Dieses Menü ist nur freigeschaltet, wenn in den Firmendaten Customizing aktiv aktiviert ist.

## Dokument – Positionen
**Dokumente > Angebot, Auftrag, Gutschrift, Anfrage, Bestellung > Positionen, `<F9>`**

**Zu Dialogbeschreibung:**
⇨ Festpreis Vorgabe
⇨ Globale Änderungen
⇨ Konditionen
⇨ Kundeninfo
⇨ Makro sichern
⇨ Position kopieren
⇨ Reklamationen
⇨ Schnellanfrage

Die Register zur Positionserfassung sind für alle Dokumentenarten gleich. Sie wird in dieser Anleitung am Beispiel **Auftrag** beschrieben.
Alle Angaben zu den ausgewählten Produkten werden aus der Produktdefinition herangezogen. Sie können dem Auftrag entsprechend geändert werden.
⇨ Tutorial, "Auftragspositionen" auf Seite C-1313

> **Rote Schrift bei manuellen Änderungen**
> Alle Einträge, die Sie manuell geändert haben, werden in roter Schrift angezeigt. Diese Änderungen können Sie pro Position über das Menü **Funktionen > Vorgaben Position löschen** rückgängig machen.
> ⇨ "Menü Funktionen" auf Seite C-1681

> **Ergänzende Informationen**
> ⇨ Tutorial, "Schnellerfassung" auf Seite C-1349
> ⇨ "Dokument - Kopfdaten" auf Seite C-1687

In diesem Dialog finden Sie folgende Register:
- "Positionen - Position" auf Seite C-1725
- "Positionen - Stückliste" auf Seite C-1736
- "Positionen - Modelle/Bearbeitungen" auf Seite C-1740
- "Positionen - Sprossen" auf Seite C-1770
- "Positionen - Leistung" auf Seite C-1780
- "Positionen - Zusatz" auf Seite C-1782
- "Positionen - Weitere Angaben" auf Seite C-1786
- "Positionen - Texte" auf Seite C-1790
- "Positionen - Anlagen" auf Seite C-1793
- "Positionen - Technische Werte" auf Seite C-1794
- "Positionen - Klassifikatoren" auf Seite C-1796

## Positionen - Position
**Dokumente > Auftrag > Auftrag auswählen > Register Positionen**

[Image: Screenshot of the order entry screen, 'Positionen' tab. It shows the product definition, sales prices, and a list of order items at the bottom.]

In diesem Register erfassen Sie Auftragspositionen. Sie können Produkte und Preise aller Stücklisten-Komponenten im ersten Register bearbeiten.
Die Positionen werden im Bereich **Positionen** eingegeben. In den Feldern werden die Daten der markierten Position angezeigt. Weitere Kennzeichen bearbeiten Sie im Register **Stückliste**. Alle manuellen Änderungen werden in roter Schrift angezeigt.
⇨ Tutorial, "Auftragspositionen" auf Seite C-1313

Über die Menüs können Sie verschiedene Einstellungen als Standard wählen, z. B. Übernahme von Daten, Aktualisierung nach Änderungen.
⇨ "Menüs in der Positionserfassung" auf Seite C-1711

> **Kreditlimit überschreiten**
> Wenn Sie mit dem aktuellen Auftrag das Kreditlimit überschreiten, das für diesen Kunden definiert ist, können Sie ggf. keine weiteren Aufträge erfassen. Der aktuelle Auftrag kann jedoch (in beliebiger Höhe) erfasst werden.
> ⇨ Tutorial, "Kreditlimit" auf Seite C-1301

### Produkt

**(Produktbezeichnungen)** Die Produktbezeichnung wird aus den Stammdaten übernommen. Sie kann für die jeweilige Auftragsposition geändert werden. Für das Hauptprodukt werden die Bezeichnungen 1 und 2 angezeigt. Die dritte Zeile zeigt bei ISO-Scheiben die technischen Parameter an. Die Angaben aus dieser Zeile können auf dem Formular gedruckt werden.
⇨ Stammdaten, "Produktbezeichnung aus Stückliste generieren" auf Seite B-1078
⇨ Stammdaten, "Formularverwaltung - Optionen 1" auf Seite B-1201

**Produktaufbau** In diesem Bereich wird der aktuelle Stücklistenaufbau der Position angezeigt. Über das Kontextmenü können Sie die Stückliste bearbeiten:
- Komponenten anhängen, einfügen (vorher), einfügen (nach), löschen.
- Modell/Bearbeitung anhängen.
- Produktionsstücklistenauflösung.
- Rückschnitt pro Kante.
In blauer Schrift werden die produktionsrelevanten Stücklisten-Komponenten aufgeführt. Sie zeigen an, an welcher Komponente die Bearbeitung durchgeführt wird.

> **Produktionsstücklisten drucken**
> Produktionsrelevante Stücklisten werden nur gedruckt, wenn in der Formularverwaltung die entsprechende Option gewählt wurde.
> ⇨ Stammdaten, “Produktionsstücklistenauflösung festlegen" auf Seite B-254
> ⇨ Stammdaten, "Stücklistendruck" auf Seite B-1203

Die Symbole stellen den Produktaufbau schematisch dar. Dabei symbolisiert die Sonne die Außenseite der Scheibe.
⇨ Tutorial, "Symbole in der Positionserfassung" auf Seite C-1318
⇨ Tutorial, "Auftragsposition erfassen" auf Seite C-1351

**Variante** Anzeige der Variante, die zum Hauptprodukt oder zu einer Komponente gewählt wurde.

**Dicke** Die Gesamtdicke ergibt sich aus der Addition der einzelnen Scheibendicken inklusive Folien, Abstandhalter usw. Wenn Sie eine andere Gesamtdicke eingeben, prüft A+W Business, ob ein passender Abstandhalter vorhanden ist. Wenn kein passender Abstandhalter vorhanden ist, wird wieder der ursprüngliche Wert angezeigt.
Die Dicke kann als Grundlage für die Berechnung eines Positionspreises herangezogen werden.
⇨ Stammdaten, "Preisverwaltung" auf Seite B-836

**Besch. Art** Die Beschaffungsart wird aus der Produktdefinition übernommen. Sie können eine andere Beschaffungsart auswählen.
Wenn eine Hauptposition oder eine übergeordnete Stücklisten-Komponente mit der Beschaffungsart **Bestellung** komplett gekennzeichnet ist, werden die zugehörigen Stücklisten-Komponenten auch dann nicht vom Lager abgebucht, wenn deren Beschaffungsart auf **Lagerentnahme** eingestellt ist. Die Beschaffungsart dieser Komponenten kann dann nicht geändert werden.

### Verkaufspreise
In der Übersicht werden alle Stücklisten-Komponenten des erfassten Produkts aufgelistet. Die Felder sind gesperrt, wenn der Auftrag an die Produktion übergeben wurde. Die Sperrung können Sie über die Funktion **Gesperrte Position ändern** aufheben.
⇨ "Gruppe Position" auf Seite C-1714

Standardmäßig werden Verkaufspreise (VK) angezeigt. Über die das Menü **Ansicht** können Sie die Preisanzeige umstellen.
⇨ "Gruppe Preise" auf Seite C-1712

Folgende Felder können angezeigt werden:
- **Art.Nr.**: Produktnummer der Stücklisten-Komponente. Um eine Stücklisten-Komponente zu tauschen, geben Sie die neue Produktnummer ein. Die Verwendung der Sternchenfunktion (*) ermöglicht Ihnen einen einfachen Austausch von Positionen, ohne einzelne Positionen zu löschen. Wenn Sie den Abstandhalter ändern, wird ggf. der Wert im Feld **Dicke** angepasst.
- **Suche**: Öffnet den Dialog zur Produktsuche.
- **Bezeichnung**: Bezeichnung 1 aus den Stammdaten.
- **PE**: Preiseinheit
- **Preis/PE**: Preis pro Preiseinheit.
- **Netto**: Preis der Stücklisten-Komponente abzüglich Rabatt. Diese Anzeige ist abhängig von der Einstellung der Preise (implizit) in der Produktdefinition. Wenn in den Firmendaten die Einzelpreisberechnung für ISO und VSG aktiviert ist, wird der Einzelpreis angezeigt. Wenn sie nicht aktiviert ist, dann werden hier die Austauschzuschläge angezeigt.
  ⇨ Stammdaten, “ISO + VSG Einzelpreisberechnung" auf Seite B-1088
- **Netto gesamt**: Wenn im Register **Stückliste** eine abweichende Menge eingegeben wird, dann unterscheiden sich die Werte in den Spalten **Netto** und **Netto gesamt**. Wenn z. B. zu einem Beschlagsset drei gleiche Abdeckungen gehören, dann wird diese Komponente einmal in der Stückliste erfasst und mit der Menge 3 eingetragen. Der Preis bei Netto gesamt ist dann = 3 x Netto.
- **Strukturverlauf, Strukturseite**: Über diese beiden Schaltflächen können Sie bestimmen, wie ein Ornamentglas in der ISO-Einheit eingebaut werden soll. Die Strukturebene wird dabei immer von außen nach innen betrachtet.
- **Beschichtungsseite**: Über die Schaltfläche können Sie bestimmen, wie ein beschichtetes Glas in der ISO-Einheit eingebaut werden soll. Die Beschichtungsebene wird dabei immer von außen nach innen betrachtet.
- **Beschaffungsart**: Beschaffungsart für die gewählte Stücklisten-Komponente.

Im Register **Stückliste** können Sie sich die Preise und weitere Details für jede einzelne Stücklistenkomponente anzeigen lassen und bearbeiten.

### Preis- und Kostenfelder

- **Anteil. Zuschlag (EK, VK)**: Anzeige des anteilig rückverteilten Fußzuschlags, z. B. Energiezuschlag. Die Fußzuschläge werden positionsgenau zurückgerechnet. Fußzuschläge einer Bestellung werden in die Kosten des Auftrags zurückgeschrieben. Die Rückverteilung kann im Menü **Optionen** ausgeschaltet werden.
  ⇨ "Menü Optionen" auf Seite C-1717
- **DB**: Deckungsbeitrag der Position. Bei dieser Anzeige sind das die Erlöse minus der Kosten (inklusive den anteiligen Fußzuschlägen EK). Die Felder werden nach dem Speichern der Position gefüllt.
- **DB %**: Prozentsatz des Deckungsbeitrags. Das ist das Verhältnis von Deckungsbeitrag zu Erlös.
- **Stückkosten**: Der Deckungsbeitrag wird aus den Stammdaten zur Preiskalkulation (EK) errechnet.
- **EK**: Der Gesamteinkaufspreis der markierten Position wird aus den Stammdaten und der Menge errechnet. Die Anzeige des Einkaufspreises (EK) ist abhängig von der Wahl der Option **Handel** oder **Produzent** in den Firmendaten.
  ⇨ Stammdaten, "Kundenversion" auf Seite B-1114
- **Erlös**: Positionsverkaufspreis zuzüglich der anteiligen Fußzuschläge VK.
- **Stückpreis**: Stückpreis der markierten Position inklusive aller Komponenten. Er wird über die Preiseinheit, die Zuschläge und Rabatte errechnet. Zu den möglichen Komponenten gehören z. B. auch Bearbeitungen, Modelle usw.
- **VK**: Gesamtverkaufspreis der markierten Position. Er kann geändert werden. Die Änderungen werden in den Gesamt-VK, den Stückpreis und in die Preise pro Preiseinheit zurückgerechnet. Wenn die Anzeige auf **Einkaufspreise** umgeschaltet ist, wird das Feld gesperrt.

> **Gesamtpreis des Auftrags**
> Der Gesamtpreis des Auftrags wird in der Titelzeile des Dialogs angezeigt.

- **Preisrelevant VK, EK**: Sie können bestimmen, ob der Preis der markierten Position in die Kalkulation des Verkaufs- und/oder Einkaufspreises einfließen soll. Die Standardeinstellung wird aus den Stammdaten übernommen.
  - Der Preis fließt nicht in die Kalkulation des VK und/oder EK ein.
  - Der Preis fließt in die Kalkulation des VK und/oder EK ein.
- **Preiskennzeichen**: Wenn zu einer erfassten Position in der Produktdefinition Besonderheiten festgelegt sind, werden die entsprechenden Symbole rot angezeigt. Wenn Sie auf das Symbol klicken, wird die entsprechende Standardeinstellung deaktiviert:
    - M: Mindestberechnung
    - /: Individualpreis
    - S: Sonstiger Zuschlag
    - L: Lagermaß
    - K: Kosten- und Aufschlagkalkulation
    - F: Formelpreis
- **Netto VK / EK**: Angabe der Nettopreise für VK und EK pro Quadratmeter. Die Angabe gilt für die aktuelle Position.
- **Kundenposition**: Die vom Kunden vorgegebene Kundenposition. In der Regel bezieht sich diese Angabe auf eine vom Kunden angegebene Kommission.
- **Kommission**: Die vom Kunden vorgegebene Kundenkommission. Diese Angabe kann auf der Versandliste und auf der Bestandsliste nach Warengruppen ausgegeben werden.
  ⇨ "Erste Kommission auf Versandliste" auf Seite C-2020
  ⇨ "Erste Kommission des Auftrags drucken" auf Seite C-2024

### Positionen (Listenansicht)
Die Anzeige der Spalten können Sie über die Tabelleneigenschaften auswählen oder ausschalten. Im Folgenden werden die wichtigsten Spalten in der Standard-Reihenfolge beschrieben.
⇨ Tutorial, "Auftragspositionen" auf Seite C-1313
⇨ Tutorial, "Automatisierte Erfassung" auf Seite C-1348

Wenn Bestellartikel an den Einkauf übergeben wurden, wird in der Spalte **Hinweis** ein entsprechender Text angezeigt. Wenn Sie die bestellte Position ändern, müssen Sie auch die referenzierte Bestellung ändern.
Wenn Sie eine Anzahlung mit der Option **Anzahlungsrechnung mit Positionen** erfasst haben, werden die Positionswerte in blauer Schrift angezeigt.
Wenn im Zeilenkopf ein Textsymbol angezeigt ist, können Sie sich den hinterlegten Text über das gleichnamige Register anzeigen lassen und bearbeiten.
⇨ "Positionen - Weitere Angaben" auf Seite C-1786

- **Pos.**: Die Positionsnummer wird bei Erfassung automatisch hochgezählt. Neue Positionen werden immer hinzugefügt, sie können nicht dazwischengeschoben werden.
- **Produkt**: Im Feld **Produkt** kann die Position auf unterschiedliche Arten erfasst werden:
    - Die Produktnummer eingeben.
    - Den Matchcode eingeben.
    - Das Produkt über die Produktsuche [Lupe] eingeben.
    - Ein gespeichertes Makro auswählen.
- **Produktsuche**: Das Produkt kann über die Suche ausgewählt werden.
- **Makrosuche**: Das Produkt kann über die Makro-Suche ausgewählt werden.
- **Dicke**: Die Gesamtdicke der Scheiben inklusive Folien, Abstandhalter usw. Wenn Sie eine andere Gesamtdicke eingeben, prüft A+W Business, ob ein passender Abstandhalter vorhanden ist.
- **Kundenposition**: Die vom Kunden vorgegebene Kundenposition.
- **Kommission**: Die vom Kunden vorgegebene Kundenkommission.
- **Bezeichnung 1, 2, 3**: Produktbezeichnungen des Hauptprodukts.
- **Stück**: Die Stückzahl kann aus der vorherigen Position vorbelegt sein. Der Wert sollte immer geprüft und ggf. geändert werden.
    > **Maße für Modelle eingeben**
    > Wenn Sie für diese Position ein Modell erfassen möchten, sollten Sie gleich nach Erfassung der Stückzahl den Dialog **Modell-/Stufenerfassung** öffnen. Sie brauchen dann Maße für Breite und Höhe nicht doppelt zu einzugeben. Aus den Angaben im Dialog Modell-/Stufenerfassung errechnet das System die Maße für das umschriebene Rechteck und übernimmt diese in die Felder **Breite** und **Höhe**.
    > ⇨ "Positionen - Modelle/Bearbeitungen" auf Seite C-1740
- **Breite**: Der Wert kann aus der vorigen Position übernommen sein und sollte immer geprüft und ggf. geändert werden. Geben Sie die Breite der Scheibe in mm (oder inch) ein.
- **Höhe**: Der Wert kann aus der vorigen Position übernommen sein und sollte immer geprüft und ggf. geändert werden. Geben Sie die Höhe der Scheibe in mm (oder inch) ein.
- **Menge**: Fläche pro Stück. Sie wird aus den Angaben für Breite und Höhe berechnet, wobei die Einstellungen zur Maßrundung aus den Stammdaten berücksichtigt werden.
  ⇨ Stammdaten, "Rundung" auf Seite B-1015
  ⇨ Stammdaten, "Tatsächliche Modellfläche zur Preisberechnung nutzen" auf Seite B-1090
  Der Wert kann nicht geändert werden. Falls mit einem Kunden vereinbart wurde, dass der Preis für eine Position nicht mit den gerundeten, sondern mit der genauen Fläche gerechnet werden soll, können Sie im Menü **Optionen > Positionen > Mengeneingabe für aktuelle Position** auswählen. Das Feld wird dann für die Eingabe eines neuen Wertes freigeschaltet. Sie müssen den neuen Wert speichern, um weitere Positionen erfassen zu können.
    > **Position als Kiste einfügen**
    > Wenn Sie über die **Lagersuche [F3]** eine Position als Kiste eingefügt haben, sind Felder ab der Spalte **Menge** gesperrt und die Position wird als Stückliste angezeigt.
    > ⇨ "Positionen - Stückliste" auf Seite C-1736
    > ⇨ "Lagersuche" auf Seite C-2034
- **SZR**: Maß für den Scheibenzwischenraum (Abstandhalter) aus der Produktdefinition. Wenn Sie den Wert überschreiben, wird der neue Abstandhalter in den Produktfeldern angezeigt. Die Änderung wird auch im Register **Stückliste** in den Stücklistenaufbau übernommen. Sie können keinen SZR auswählen, wenn im Auftrag bestimmte Vorgaben eingestellt sind:
  ⇨ "Abstandhaltervorgabe" auf Seite C-1707
- **Rückschnitt**: Der Rückschnitt wird für jede Position angezeigt, ohne dass die entsprechende Position explizit geöffnet werden muss.
- **Jahrgang, Schlüssel**: Preisjahrgang und Preisschlüssel, die dem Produkt über den Tarif zugeordnet sind.
    > **Preisanzeige ausblenden**
    > Falls Sie nicht möchten, dass bestimmte Mitarbeiter die Positionspreise sehen, können Sie die Anzeige über die Mitarbeiterrechte ausblenden.
    > ⇨ Stammdaten, "Mitarbeiterrechte" auf Seite B-1156
    > ⇨ Stammdaten, "Identifikation, Programmauswahl" auf Seite B-1157
- **Preis/PE**: Wenn dem erfassten Produkt ein Preis pro Einheit zugeordnet ist, wird dieser hier angezeigt.
    > **Stückpreis festlegen**
    > Wenn Sie in dieser Zeile einen Stückpreis festlegen, bezieht sich dieser nur auf das Hauptprodukt. Abstandhalter und andere Komponenten werden zusätzlich berechnet. Einen Stückpreis für das erfasste Produkt insgesamt legen Sie im Feld **Stückpreis** fest. Einen Festpreis für die gesamte Position legen Sie über das Kontextmenü fest.
    > ⇨ "Kontextmenü auf Position" auf Seite C-1733
- **Einheit**: Einheit, auf die sich der Preis bezieht.
- **Rabatt**: Rabatt, der für den Kunden hinterlegt ist. Sie können den angezeigten Wert ändern. Die Preise werden dann aktualisiert.
  ⇨ Stammdaten, "Kunde" auf Seite B-933
- **Netto**: Der Nettostückpreis wird nur für das Glas angezeigt. Er wird aktualisiert, wenn Sie Preis, Schlüssel, Preiseinheit und/oder Rabatt geändert haben. In ihm sind keine Preise für Modell, Bearbeitungen usw. enthalten.
    > **Preis- und Rabattkonditionen anzeigen**
    > Über das Menü **Anzeige > Konditionen** können Sie sich die aktuellen Konditionen für den Kunden anzeigen lassen.
    > ⇨ "Konditionen" auf Seite C-1881

    > **Zeitnahe Preisberechnung ausschalten**
    > Über das Menü **Optionen > Preisberechnung nur beim Speichern** können Sie die Aktualisierung bei jeder Preisänderung ausschalten. Dies ist sinnvoll, wenn Produkte mit sehr komplexen Stücklisten erfasst werden, deren Stücklisten-Komponenten alle preisrelevant sind.

- **Zusätzliche Spalten**: Zusätzlich zu den genannten Spalten können folgende Spalten angezeigt werden: Dicke, Kundenposition, Kommission, Bezeichnung 1, 2, 3, DB (Deckungsbeitrag), Strukturverlauf, Strukturseite, Beschichtungsseite, Hinweis.
- **DB**: Deckungsbeitrag für ein Stück der Position.
- **Strukturverlauf**: Art, wie das Ornamentglas in der ISO-Einheit eingebaut werden soll.
- **Strukturseite, Beschichtungsseite**: Die Seiten (Ebenen) werden von außen nach innen betrachtet.
- **Hinweis**: Warnhinweis bei Positionen, die bereits bestellt sind.
    > **Tabellenspalten**
    > Einzelne Tabellenspalten können über die Eigenschaften ein- und ausgeblendet werden.

### Kontextmenü auf Position
Sie öffnen das Kontextmenü mit der rechten Maustaste.
- **Gruppe bilden**: Die markierten Positionen werden als Gruppe zusammengefasst. Im Druck wird nach der Gruppe eine Zwischensumme gebildet. Die Gruppen werden durch Farben gekennzeichnet.
  [Image: Example of grouped positions highlighted in different colors in a table.]
- **Gruppe aufheben**: Die Gruppenbildung wird wieder aufgehoben.
- **Position einfügen davor, Position einfügen danach**: Die markierte Position wird kopiert und davor/danach eingefügt.
- **Position löschen und aufrücken**: Die markierte(n) Position(en) wird/werden gelöscht. Die Nummerierung der nachfolgenden Positionen wird aktualisiert.
- **Positionen neu sortieren**: Sortiert die Auftragspositionen neu. Wenn der Auftrag bereits an die Produktion übergeben, wird nach einer Rückfrage versucht den Auftrag in der Produktion zu stornieren. Der Auftrag muss danach neu an das Produktionssystem übergeben werden. Dies gilt auch, wenn Positionen hinzugefügt oder gelöscht werden.
- **Import aus Zwischenablage**: Fügt eine oder mehrere Positionen aus der Zwischenablage ein, z. B. aus Microsoft Excel. Siehe dazu den nachfolgenden Hinweis. Diese Funktionalität benötigt das lizenzpflichtige Modul **156 Excel Line Item Import**.
- **Festpreis vorgeben**: Öffnet den Dialog **Festpreis Vorgabe**, um einen Festpreis für mehrere markierte Positionen festzulegen. Der Festpreis wird anteilmäßig auf die markierten Positionen zurückgerechnet.
  ⇨ "Festpreis Vorgabe" auf Seite C-1878
- **Vorgabe Festpreis löschen**: Setzt den manuell vorgegebenen Festpreis zurück auf den vorigen Wert. Dies kann entweder der Standardpreis oder der manuell eingetragene Preis sein. Manuelle Preisänderungen werden über Menü **Funktionen > Vorgabe Positionen löschen** auf den Standardpreis zurückgesetzt.
- **Globale Änderungen**: Öffnet den Dialog **Globale Positionsänderungen**, in dem Sie die Kommissionierung für die aktuelle Position ändern können.
  ⇨ "Globale Änderungen" auf Seite C-1879
- **Inhalt in Zwischenablage**: Kopiert den Inhalt der markierten Position in die Zwischenablage, um sie in einem anderen Programm zu verwenden.

> **Import aus Zwischenablage**
> Über diesen Import können folgende Werte importiert werden:
> - Menge
> - Abmessung
> - Kommission
> - Kundenposition
> - Artikelnummer
> - Abstandhalter für die Stücklistenpositionen 2 und 4 (mit Typ und Dicke)
> - Angabe von Positionstext
>
> Für das Feld Produkt kann die Logik der Schnellerfassung angewendet werden, sodass Sprossen und andere Angaben direkt übernommen bzw. geändert werden können. Die Spalten in der Zwischenablage müssen per TAB getrennt sein und können eine Überschrift enthalten. Die verschiedenen Spalten können einer der möglichen Eigenschaften einer Position zugeordnet und als Vorlage für spätere Importe gespeichert werden.
>
> Wird eine Überschrift importiert, so versucht das Programm anhand der Überschrift die richtige Eigenschaft selbständig zuzuordnen. Dafür müssen die Überschriften die gleiche Bezeichnung haben wie die Eigenschaft in der Positionstabelle.
> Für die Artikelnummer können die B2B Referenzen für den jeweiligen Partner verwendet werden, um damit die dort hinterlegte Produktaufbauten samt Stückliste zu importieren. Wird keine Artikelnummer importiert, so wird die aktuelle Position der Positionserfassung samt Stückliste als Vorlage verwendet.

## Positionen – Stückliste
**Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Stückliste**

[Image: Screenshot of the 'Stückliste' (Bill of Materials) tab. It shows the components of the selected product position.]

In diesem Register können Sie die Details für die Preisberechnung von Stücklisten-Komponenten bearbeiten.
Die Felder werden so aktiviert und/oder aktualisiert, wie Sie es über die Menüs festgelegt haben.
⇨ "Menüs in der Positionserfassung" auf Seite C-1711

> **Leistungen**
> Wenn Sie Leistungen hinzugefügt haben, bleiben die zugehörigen Felder gesperrt. Sie können die Daten der Leistung nur über das Register **Leistungen** ändern.

### Produkt
In diesem Bereich werden die Daten der markierten Stücklisten-Komponente angezeigt. An dieser Stelle steht Ihnen auch die Sternchenfunktion (*) als Suche zur Verfügung. Wenn Sie das Hauptprodukt markiert haben, sind die Felder gesperrt.
- **(Nummer)**: Produktnummer der markierten Komponente. Über die Suche kann ein anderes Produkt ausgewählt werden. An dieser Stelle funktioniert auch die Sternchenfunktion (*).
- **(Bezeichnung)**: Die Bezeichnung wird aus den Stammdaten des Produkts übernommen.
- **(Beschreibung)**: Die Beschreibung wird aus den Stammdaten des Produkts übernommen und zeigt den Bearbeitungstext an.
- **Darstellung**: Sie können festlegen, wie die Preise im Druck dargestellt werden. Die Standardeinstellung wird aus den Stammdaten übernommen. Zusätzlich muss für den Druck die Checkbox **Druck** markiert werden. Preise können nur dann gedruckt werden, wenn in der Produktdefinition die Checkbox **Preisrelevant** markiert und ein Preis hinterlegt ist.
  ⇨ Stammdaten, "Preisrelevant VK, Preisrelevant EK" auf Seite B-733
    - **Implizit**: Der Netto-Preis der Hauptposition beinhaltet alle Preise der Stücklisten-Komponenten, also auch die Modell- und Austauschzuschläge und die Bearbeitungen.
    - **Explizit**: Die Preise der Stücklisten-Komponenten werden einzeln ausgewiesen.
    - **Implizit in Preis pro Mengeneinheit**: Die Preise der Stücklisten-Komponenten werden umgerechnet auf die Preiseinheit des Hauptproduktes. Dieser Gesamtpreis der Preiseinheit wird im Dokument ausgewiesen, aber nur dann, wenn allen Stücklisten-Komponenten einer Position die gleiche Darstellungsart zugewiesen ist.
- **Variante**: Die Felder sind nur freigeschaltet, wenn für das markierte Produkt Varianten hinterlegt sind. Über die Kombobox können Sie eine Variante auswählen.
- **Autom. Zuschnitt**: Die Angabe zum automatischen Zuschnitt wird aus den Stammdaten übernommen. Sie kann geändert werden.
  - Die Scheibe wird im Handzuschnitt produziert.
  - Die Scheibe wird am Schneidetisch automatisch zugeschnitten.
- **Druck**: Die Stückliste kann wahlweise im Auftragsformular gedruckt werden. Diese Einstellung kann die Einstellungen aus der Produktverwaltung und der Formularverwaltung nicht übersteuern.
  - Die Stücklisten-Komponente wird nicht auf dem Formular gedruckt.
  - Die Stücklisten-Komponente wird mit gedruckt.
> **Voraussetzung**
> Nur wenn das Druckkennzeichen für die Stücklisten-Komponenten oder das Produkt gesetzt ist, kann eine Stücklisten-Komponente im Auftrag gedruckt werden.
> ⇨ Stammdaten, "Wird gedruckt" auf Seite B-733

In den Firmendaten kann festgelegt werden, wie viele Stücklisten-Komponenten maximal gedruckt werden können.
⇨ Stammdaten, "Stückliste" auf Seite B-1123
⇨ Stammdaten, "Formularverwaltung - Optionen 1" auf Seite B-1201

- **Geändert**: Die Markierung wird gesetzt, wenn eine Stücklisten-Komponente ausgetauscht wurde, also z. B. Float 4 mm durch ein Ornamentglas.
  - Die Komponente wurde unverändert übernommen.
  - Die Komponente wurde für diesen Auftrag geändert.

### Verkaufspreise
In diesem Bereich werden für die markierte Stücklisten-Komponente die Preise für alle zusätzlichen Details angezeigt, z. B. für Abstandhalter, Bearbeitungen, Modelle, Lagermaße.
- **Jahrgang**: Der Preisjahrgang wird aus den Stammdaten des Produktpreises übernommen. Er kann für die markierte Komponente im aktuellen Auftrag geändert werden.
- **Schlüssel**: Der Preisschlüssel wird angezeigt, dem der Produktpreis zugeordnet ist. Sind mehrere Schlüssel zugeordnet, kann die Einstellung für die markierte Komponente im aktuellen Auftrag geändert werden.
- **Zuschlagsart**: Die Zuschlagsart wird aus den Stammdaten des Produkts übernommen. Sie kann für die markierte Komponente im aktuellen Auftrag geändert werden.
  ⇨ Stammdaten, "Berechnungen nach Zuschlagsarten" auf Seite B-381
- **Preis / PE**: Der Preis und die Preiseinheit werden aus den Stammdaten des Produkts übernommen. Sie bilden die Basis für die Berechnung des Preises.
- **Rabatt**: Ein Rabatt wird nur angezeigt, wenn dieser in den Kundendaten hinterlegt ist. Sie können den Wert ändern. Die Preisanzeige wird automatisch aktualisiert.
- **Preisrelevant VK, EK**: Sie können bestimmen, ob der Preis der markierten Komponente in die Kalkulation des Verkaufs- und/oder Einkaufspreises einfließen soll. Die Standardeinstellung wird aus den Stammdaten übernommen.
  - Der Preis fließt nicht in die Kalkulation des VK und/oder EK ein.
  - Der Preis fließt in die Kalkulation des VK und/oder EK ein.
- **Netto**: Aktualisierter Netto-Preis für die markierte Komponente.
- **Netto ges.**: Wenn in der Stückliste identische Komponenten enthalten sind, wird deren Gesamtpreis angezeigt, z. B. der Gesamtpreis für zwei Lochbohrungen.
- **Mind. Menge**: Anzeige der Mindestmenge, die auch dann berechnet wird, wenn die Menge pro Stück unter dieser Größe bleibt.
  ⇨ Tutorial, "Preise und Preisberechnung" auf Seite C-1398
  ⇨ Stammdaten, "Tatsächliche Modellfläche zur Preisberechnung nutzen" auf Seite B-1090
  ⇨ Stammdaten, "Mindestmengenprüfung vorrangig nach Preiseinheit" auf Seite B-1093
- **Maßrund.**: Maßrundung für die Berechnung der Fläche.
  ⇨ Stammdaten, "Maßberechnung" auf Seite B-212
- **WGR Rabatt, Statistik**: Anzeige der Warengruppen, denen das Produkt zugeordnet ist.

### Details
- **Lieferant**: Wenn die markierte Komponente bestellt werden muss, können Sie einen (abweichenden) Lieferanten auswählen.
  ⇨ Stammdaten, "Lieferantenkartei" auf Seite B-987
- **Stk/M/Br/Hö**: Stückzahl und die Maße der Komponente.
> **Geänderte Maße werden nicht in die Positionszeile übernommen**
> Wenn Sie die Maße für eine Stücklistenkomponente ändern, werden die neuen Maße nicht in die Erfassungsfelder für die Position übernommen.
- **Besch.-Art**: Die Beschaffungsart wird automatisch geprüft und ggf. umgesetzt, wenn Sie die Maße einer Komponente ändern.
- **Preiskennzeichen**: Wenn zu einer markierten Stücklisten-Komponente in der Produktdefinition Besonderheiten für die Preisberechnung festgelegt sind, werden die entsprechenden Symbole rot angezeigt. Wenn Sie auf das Symbol klicken, wird die entsprechende Standardeinstellung deaktiviert.
    - M: Mindestberechnung
    - /: Individualpreis
    - S: Sonstiger Zuschlag
    - F: Formelpreis
    - P: Produktionsstücklistenauflösung
  ⇨ Tutorial, “Symbole in der Positionserfassung" auf Seite C-1318

### Positionen
Die Felder sind zum Register **Position** beschrieben.
⇨ "Positionen" auf Seite C-1730

## Positionen – Modelle/Bearbeitungen
**Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Modelle/Bearbeitungen > Modell auswählen**

[Image: Screenshot of the 'Modelle/Bearbeitungen' tab showing a trapezoidal glass shape (Modell) with its parameters.]

In diesem Register erfassen Sie folgende Daten zu einer Auftragsposition:
- "Modelle" auf Seite C-1741
- "Positionen - Bearbeitungen" auf Seite C-1744
- "Positionen - Stufung" auf Seite C-1763
- "Positionen - Gebogenes Glas" auf Seite C-1765
- "Positionen - Bleiverglasungen" auf Seite C-1767
- "Positionen - Modell-Template" auf Seite C-1768

### Stückliste
Bearbeitungen können an einzelnen Komponenten der Stückliste ausgeführt werden. Angaben zum Modell betreffen immer das Hauptprodukt.
In der Ansicht wird das Modell schematisch angezeigt. Die Legende bezeichnet die Felder, in denen die Maße eingegeben werden.

### Bearbeitungen
**Schaltflächen**: Mit den Schaltflächen wählen Sie eine Produktgruppe aus, z. B. Modelle, Bearbeitungen, gebogenes Glas oder Bleiverglasung. Wenn der Produktgruppe verschiedene Produkte zugewiesen sind, können Sie das gewünschte Produkt im Dialog **Auswahl** markieren und übernehmen.

**Artikel**: Produktnummer und Bezeichnung aus den Stammdaten.

**Formel**: Auswahl und Anzeige der Formel für den Bearbeitungstext.
⇨ "Positionen - Bearbeitungen" auf Seite C-1744

### Modelle
- **(Symbole)**: Über die Schaltflächen können Sie ein Modell auswählen.
  ⇨ "Positionen - Bearbeitungen" auf Seite C-1744
  ⇨ "Positionen - Modell-Template" auf Seite C-1768
- **Artikel**: Die Produktnummer des Modells wird aus den Stammdaten übernommen.
- **Modell**: Die Modellnummer wird aus den Stammdaten übernommen.
- **(Bezeichnung)**: Die Bezeichnung des Modells wird aus den Stammdaten übernommen.

#### Modellparameter
- **W, H**: Zu jedem Modell werden nur die Felder freigeschaltet, die zur Produktion des Modells notwendig sind. Die Bezeichnungen für die Kanten werden in der Ansicht gezeigt.
- **Restriktionen**: In diesem Bereich finden Sie Angaben zu den Restriktionen. Beispiel: `H1>0` bedeutet, dass die Kante H1 nicht 0 sein darf.

#### S+N Datei
Wenn Sie häufiger ein bestimmtes Modell mit identischen Maßen erfassen, können Sie es als S+N-Datei speichern. In späteren Aufträgen können Sie diese Datei über die Schaltfläche [Ordner] dann auswählen und der Auftragsposition zuordnen, ohne die Details neu eingeben zu müssen.

In den Stammdaten können Regeln definiert werden, mit denen festgelegt wird, welcher Bearbeitungsartikel beim Abgleich in die Stückliste übertragen werden soll.
⇨ Stammdaten, "iTOE Regeln" auf Seite B-778

In der Bearbeitungserfassung kann der Abgleich entweder durch einen DXF-Datei-Import oder durch die Schaltfläche [iTOE] im Ribbon gestartet werden. Wenn im A+W CAD Designer (Shapes) die Änderungen an der Glas-Einheit in eine Datei übernommen wurden, können diese Änderung mit der Datei importiert werden.
Eine ausführliche Beschreibung der Funktion finden Sie in der Dokumentation zum A+W CAD Designer (Shapes).

Wenn Sie das Modell 99 ausgewählt haben, können Sie auch ein S+N-Template laden und zuordnen.
⇨ "SN-Datei und Template" auf Seite C-1430
⇨ "Positionen – Modell-Template" auf Seite C-1768

> **Als Makro sichern**
> Als Alternative zum Speichern eines Modells als S+N-Datei, können Sie den gesamten Produktaufbau einer Position als Makro speichern.
> ⇨ Tutorial, "Makro speichern" auf Seite C-1420
> ⇨ "Makro sichern" auf Seite C-1908

#### Umschriebenes Rechteck
Das umschriebene Rechteck wird standardmäßig zur Preisberechnung herangezogen. In den Firmendaten kann eingestellt werden, dass die tatsächliche Fläche zur Preisberechnung herangezogen werden soll.
⇨ Stammdaten, "Tatsächliche Modellfläche zur Preisberechnung nutzen" auf Seite B-1090

**(Skizzendruck)** Sie können auswählen, wie das Modell im Druck wiedergegeben werden soll:
- **Kein Druck**: Die Skizze wird nicht auf den Formularen gedruckt.
- **Modell (maßstäblich)**: Bei dieser Einstellung werden maßstabsgetreue Modellskizzen gedruckt.
- **Modell (schematisch)**: Bei dieser Einstellung werden die Standardskizzen gedruckt. Sie geben lediglich das Schema des Modells wieder.

**Drehung um**: Winkel, um den das Modell gedreht werden soll. Die Funktion steht muss in den Firmendaten aktiviert sein.
⇨ Stammdaten, "Firmendaten - Dokumente" auf Seite B-1066
Als Drehwinkel kann 90, 180 oder 270 Grad eingegeben werden. Im Druck auf den Papieren wird die gedrehte Form dargestellt.

**Ausnahmen**:
- Modelle mit den Modell-Nummern 0, 24, 98, 99, 60, 61 und 81 können nicht gedreht werden.
- In gedrehten Modellen können keine Sprossen erfasst werden, Modelle mit Sprossen können nicht gedreht werden.
- **Strukturgläser**: Wird ein Modell um 90 oder 270 Grad gedreht, gilt Folgendes:
    - Für die Produktion (OrderXML oder Produktionsmanager) und EDI Export werden die Modelle umgedreht übertragen. Das Kennzeichen für die Struktur wird dabei getauscht: waagrecht -> senkrecht, senkrecht -> waagrecht.
    - Die Prüfung der maximalen Maße bezieht sich auf das gedrehte Maß.

#### Verkaufspreise
- **Jahrgang / Schlüssel**: Preisjahrgang und -schlüssel für den Modellzuschlag werden aus den Stammdaten übernommen. Sie können geändert werden.
- **Preis / PE**: Preis und Preiseinheit für den Modellzuschlag aus den Stammdaten. Sie können geändert werden.
- **Rabatt**: Rabatt für den Modellzuschlag aus den Stammdaten. Er kann geändert werden.
- **Netto**: Der Nettobetrag für den Modellzuschlag wird automatisch angezeigt.

## Positionen – Bearbeitungen
**Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Modelle/Bearbeitungen > Bearbeitung auswählen**

[Image: Screenshot of the 'Bearbeitungen' (Machinings) tab. It shows a list of product components and the details for a selected machining, "Säumen von 4 Kante(n)".]

In diesem Dialog können Sie zu jeder Auftragsposition eine oder mehrere Bearbeitungen erfassen.
Die Bereiche **Stückliste**, **Bearbeitung**, **Verkaufspreise** und **Skizzendruck** sind zum Register **Modelle/Bearbeitungen** erklärt.
⇨ "Positionen – Modelle/Bearbeitungen" auf Seite C-1740
⇨ Tutorial, "Bearbeitung erfassen" auf Seite C-1373

### Bearbeitung
Mit den Schaltflächen wählen Sie eine Produktgruppe aus. Wenn der Produktgruppe verschiedene Produkte zugewiesen sind, können Sie das gewünschte Produkt im Dialog **Auswahl** markieren und übernehmen.
Dem gewählten Produkt entsprechend werden die Felder im Bereich **Parameter** angezeigt.

> **Bearbeitungen an Modellen**
> Bearbeitungen können auch auf dem Modell 99 und auf importierten SN Dateien angebracht werden.
> ⇨ "Positionen - Modell-Template" auf Seite C-1768

**[Formel]**: Die Parameter des Bearbeitungstextes können bearbeitet werden. Mit dieser Schaltfläche öffnen Sie den Dialog **Parameter-Ersetzung**.
⇨ "Parameter-Ersetzung" auf Seite C-1873

### Parameter
Die eingetragenen Werte werden in die Berechnungsformel für den Preis und an die Produktion übergeben. Die angezeigten Felder unterscheiden sich je nach der Bearbeitung, die Sie gewählt haben.
- Kantenbearbeitungen, Verklebung
- Lochbohrungen
- Senkbohrungen
- Stufenbohrungen
- Rundecken
- Eckausschnitte
- Schrägecken
- Randausschnitte, Bogenförmiger Randausschnitt
- Innenausschnitte, Durchsprechöffnung, Handgriffe
- Beschichtung, Mattierung, Siebdruck, Flächen-Emaillierung, Sandstrahlen, Kolorieren
- Randentschichtungen
- Biegen
- Rillenschliff
- Nachschleifen, Kantenschutz
- Logo, Stempel
- Makro Ecke, Makro Rand, Parametrisierbares Makro (Kante)
- Emaillierung
- Alarmspinne
- Bleiverglasung
- Gebogenes Glas
- Abkleben
- Entschichtung
- Randsiebdruck
- Makro Innen, Parametrisierbares Makro (Innen)
- Artikel

### Kantenbearbeitungen, Verklebung
- **Menge**: Das Feld ist gesperrt.
- **Alle Kanten, (Kante) 1-8**: Auswahl der Kanten, an denen die Kantenbearbeitungen ausgeführt werden sollen. Die ausgewählten Kanten werden in die Beschreibung übernommen.
  - Die Kante wird nicht bearbeitet.
  - Die Kante wird bearbeitet.
- **Exakte Berechnung**: Die Angabe ist zwingend notwendig, wenn das Modell mehr als vier Kanten hat.
  - Die Kantenbearbeitung wird (standardmäßig) nach den Maßen des umschriebenen Rechtecks berechnet. Die Felder **x Breite** und **x Höhe** sind freigeschaltet. Wenn das Modell mehr als vier Kanten hat, können Sie hier eintragen, wie diese Kanten gewertet werden sollen, z. B. 2 x Breite und 3 x Höhe.
  - Die Kantenbearbeitung wird nach den exakten Maßen berechnet. Die Felder **Kantenbearbeitungsgröße** werden freigeschaltet.
In den Firmenstammdaten wird übergreifend festgelegt, wie die Kantenbearbeitung berechnet werden soll.
⇨ Stammdaten, "Kantenbearbeitung mit exakten Lfm berechnen" auf Seite B-1073
⇨ Stammdaten, "Kantenmindestlänge pro Kante berechnen" auf Seite B-1088
⇨ Stammdaten, "Kaufmännische Maßrundung der Abmessung" auf Seite B-1088
- **...x Breite, ... x Höhe**: Die Felder sind nur freigeschaltet, wenn die exakte Berechnung deaktiviert ist. Die Angaben legen fest, mit welchem Faktor Breite und Höhe des umschreibenden Rechtecks multipliziert werden sollen.
    **Beispiele:**
    - Die Eingabe 2 x Breite und 2 x Höhe ergibt die Kantenlänge des umschreibenden Rechtecks.
    - Die Eingabe 2 x Breite und 3 x Höhe ergibt die Kantenlänge eines Fünfecks.
- **Kantenbearbeitungsgröße**: Die Felder sind nur freigeschaltet, wenn die exakte Berechnung aktiviert ist. Diese Angaben legen fest, wie die Kantenbearbeitung berechnet werden soll.
- **Winkel**: Das Feld wird bei Polituren von Facetten und Gehrungen angezeigt. Die Angabe legt den Winkel fest, in dem die Politur ausgeführt werden soll.
- **Tiefe**: Das Feld wird bei Polituren von Facetten angezeigt. Die Angabe legt fest, wie tief die Politur ausgeführt werden soll.
- **(Facette, Gehrung) nach außen**: Die Checkbox wird bei Facetten und Gehrungen angezeigt.
  - Die polierte Facette, Gehrung wird nicht nach außen angebracht.
  - Die polierte Facette, Gehrung wird außen angebracht.

### Lochbohrungen
- **Menge**: Anzahl der Bohrungen. Das Feld wird gefüllt, wenn im Bereich **Parameter** die Koordinaten für die Bohrungen eingegeben sind. Wenn die Menge eingegeben wird, werden die Felder für die Bohrungskoordinaten gesperrt. Das Programm geht dann davon aus, dass nur der Preis ermittelt werden soll, z. B. im Angebot.
- **Durchmesser**: Durchmesser für alle Bohrungen in mm.
- **Vermaßungstyp**: Mit der Wahl des Vermaßungstyps legen Sie fest, wie die eingegebenen Werte interpretiert werden sollen. Unter den Feldern wird jeweils eine Grafik angezeigt, aus der Sie ersehen können, wie die Werte angegeben werden müssen.
  - **Absolute Koordinaten**: Bei dieser Einstellung wählen Sie die Ecke aus, von der aus gemessen werden soll.
  - **Abstand zu 2 Kanten**: Bei dieser Einstellung wählen Sie die beiden Kanten aus, von denen aus gemessen werden soll.
  - **Ecke, Kante, Abstand zur Kante**: Bei dieser Einstellung wählen Sie die Ecke und die Kante aus, von denen aus gemessen werden soll.
  [Image: Icons illustrating the three dimensioning types: Absolute Koordinaten, Abstand zu 2 Kanten, and Ecke, Kante, Abstand zur Kante.]
- **Bohrung 1-4 [x/y]**: Diese Angaben legen die Positionen der Bohrungen fest. Die Werte x und y werden dem Vermaßungstyp entsprechend interpretiert.
- **Ecke, Kante**: Die Bezugsecke und Kante können pro Bohrung gewählt werden.
- **Entlastungsschnitt**: Für Bohrlöcher, Senkbohrungen und Stufenbohrungen kann ein Entlastungsschnitt gesetzt werden, z. B., wenn die Bohrung zu nah an der Kante ist. Der Parameter kann über die OrderXML-Schnittstelle an die Produktion übergeben werden.
  - Ein Entlastungsschnitt wird nicht ausgeführt.
  - Ein Entlastungsschnitt wird ausgeführt.

### Senkbohrungen
Für diese Bearbeitungen werden auch die Felder **Vermaßungstyp**, **Bohrung 1-4 [x/y]** und **Entlastungsschnitt** angezeigt. Siehe dazu:
⇨ "Lochbohrungen" auf Seite C-1747
- **Menge**: Anzahl der Bohrungen. Das Feld wird gefüllt, wenn im Bereich Parameter die Koordinaten für die Bohrungen eingegeben sind. Wenn die Menge eingegeben wird, werden die Felder für die Bohrungskoordinaten gesperrt. Das Programm geht dann davon aus, dass nur der Preis ermittelt werden soll, z. B. im Angebot.
- **(Typ)**: Ebene der Senkung. Wenn Sie den Eintrag **Senkung beidseitig** gewählt haben, werden alle Felder freigeschaltet.
- **Auswahl der Erfassung**: Schaltfläche zur Art der Erfassung fest. Sie schaltet die entsprechenden Felder frei:
  - **D**: Der Durchmesser wird abgefragt. Die Felder D1, 2 werden angezeigt.
  - **T**: Die Tiefe der Senkung wird abgefragt. Die Felder T1, 2 werden angezeigt.
  Die grafische Darstellung zeigt die Interpretation der jeweiligen Werte an.
  [Image: Diagrams showing dimensioning for diameter and countersink depth.]
- **D1, 2**: Durchmesser der Senkung in mm (innen, außen). Die Felder sind nur freigeschaltet, wenn Sie **Durchmesser** gewählt haben.
- **T1, 2**: Angaben der Tiefe der Senkung in mm (innen, außen). Die Felder sind nur freigeschaltet, wenn Sie **Tiefe** gewählt haben.
- **D**: Durchmesser der Bohrung in mm.
- **<1, <2**: Öffnungswinkel in Grad. Standardmäßig werden für den Öffnungswinkel 60,00 Grad angegeben.
Die Felder D1, T1 und <1 sind gesperrt, wenn Sie im Feld **Typ** der Eintrag **Senkung innen** gewählt haben. Die Felder D2, T2 und <2 sind gesperrt, wenn Sie im Feld **Typ** der Eintrag **Senkung außen** gewählt haben.

### Stufenbohrungen
Für diese Bearbeitungen werden auch die Felder **Vermaßungstyp**, **Bohrung 1 – 4 [x/y]** und **Entlastungsschnitt** angezeigt. Siehe dazu:
⇨ "Lochbohrungen" auf Seite C-1747
- **Menge**: Anzahl der Bohrungen. Das Feld wird gefüllt, wenn im Bereich Parameter die Koordinaten für die Bohrungen eingegeben sind. Wenn die Menge eingegeben wird, werden die Felder für die Bohrungskoordinaten gesperrt. Das Programm geht dann davon aus, dass nur der Preis ermittelt werden soll, z. B. im Angebot.
- **Ø (Durchmesser)**: Durchmesser der Bohrung pro Glas in der ISO-Einheit. Die Angaben gelten für alle Bohrungen.
Die grafische Darstellung zeigt die Interpretation der Werte an.
[Image: Diagrams illustrating the input for diameters in a stepped hole.]

### Rundecken
- **Menge**: Anzahl der Rundecken. Das Feld ist gesperrt. Es wird gefüllt, wenn im Bereich **Alle Ecken, (Ecke) 1 - 8** die Anzahl der Rundecken ausgewählt wird.
- **Alle Ecken, (Ecke) 1-8**: Die Checkboxen bezeichnen die Ecken, an denen die Rundecken ausgeführt werden sollen.
  - Die Rundecke wird nicht geschnitten.
  - Die Rundecke wird geschnitten.
- **Radius**: Radius gilt für alle Rundecken. Er wird vom Scheibenmittelpunkt aus gemessen. Wenn für die Rundecken unterschiedliche Radien gelten sollen, müssen Sie für jede Rundecke eine eigene Bearbeitung angeben.

### Eckausschnitte
- **Menge**: Anzahl der Eckausschnitte. Das Feld ist gesperrt. Es wird gefüllt, wenn im Bereich **Alle Ecken, (Eckausschnitt) 1 – 8** die Anzahl der Eckausschnitte ausgewählt wird.
- **Alle Ecken, (Eckausschnitt) 1-8**: Auswahl der Ecken, an denen die Eckausschnitte ausgeführt werden sollen.
  - Der Eckausschnitt wird nicht geschnitten.
  - Der Eckausschnitt wird geschnitten.
- **Abstand A / B**: Abstand A und B für alle Eckausschnitte. Standardmäßig werden diese Abstände in der festen Verbindung A/B für die Ecken dargestellt. Wenn Sie für A und B unterschiedliche Werte eingeben möchten, damit z. B. hoch-rechteckige Ausschnitte produziert werden, müssen Sie im Feld **Ausschnittskante A / B** auswählen, wie der Ausschnitt gemessen werden soll.
- **Ausschnittskante A / B**: Standardmäßig ist für A und B **Senkrecht** eingestellt. Das bedeutet, dass z. B. A sowohl eine senkrechte als auch eine waagerechte Ausschnittskante bezeichnet. Sie können für diesen Auftrag festlegen, wie die Ausschnittskanten gemessen werden sollen:
  - **Senkrecht**: Die Ausschnittskanten sollen senkrecht gemessen werden.
  - **Parallel**: Die Ausschnittskanten sollen parallel gemessen werden.
  Wählen Sie z. B. für **A Senkrecht** und für **B Parallel**, so werden alle Ausschnittskanten A senkrecht und alle Ausschnittskanten B waagerecht gemessen.
  Sie können in den Firmendaten die Parameter für die Eckausschnitte generell ändern. Diese Änderung betrifft dann alle Aufträge!
  ⇨ Stammdaten, "Rechteckeckausschnitte als Breite x Höhe erfassen" auf Seite B-1077
- **Eckradius Aussen / Innen**: Eckradius für den Ausschnitt in mm.

### Schrägecken
- **Menge**: Anzahl der Eckabschnitte. Das Feld ist gesperrt. Es wird gefüllt, wenn im Bereich **Alle Ecken, (Schrägecke) 1 - 8** die Anzahl der Eckabschnitte ausgewählt wird.
- **Alle Ecken, (Schrägecke) 1-8**: Auswahl der Ecken, an denen die Eckabschnitte ausgeführt werden sollen.
  - Der Schrägschnitt wird nicht geschnitten.
  - Der Schrägschnitt wird geschnitten.
- **Abstand A / B**: Abstand A und B für alle Schrägecken. Standardmäßig werden diese Abstände in der festen Verbindung A/B für die Ecken dargestellt. Siehe dazu auch die Beschreibung zu den Eckausschnitten.
  ⇨ "Abstand A / B" auf Seite C-1750

### Randausschnitte, Bogenförmiger Randausschnitt
- **Abstand / Ecke / Kante, X/Y/Ecke**: Maße und Bezugsecke bzw. Bezugskanten, von denen aus gemessen werden soll. Die Felder sind ausgeblendet, wenn die Checkbox **Multi** markiert ist.
- **Menge**: Anzahl der Randausschnitt, die angebracht werden sollen. Das Feld wird nur angezeigt, wenn die Checkbox **Multi** markiert ist. Das Feld ist gesperrt. Es wird gefüllt, wenn im Bereich **Alle Kanten, (Kante) 1 – 8** die Anzahl der Randausschnitte ausgewählt wird.
- **Alle Kanten, (Kante) 1-8**: Auswahl der Kanten, an denen die Randausschnitte angebracht werden sollen. Die Felder werden nur angezeigt, wenn die Checkbox **Multi** markiert ist. In den Feldern geben Sie an, wie viele Randausschnitte an der jeweiligen Kante angebracht werden sollen.
  - An der Kante wird kein Randausschnitt angebracht.
  - An der Kante wird (mindestens) ein Randausschnitt angebracht.
- **Vermaßungsart**: Mit der Wahl der Vermaßungsart legen Sie fest, wie die eingegebenen Werte interpretiert werden sollen. Unter den Feldern wird jeweils eine Grafik angezeigt, aus der Sie ersehen können, wie die Werte angegeben werden müssen. Die Vermaßungsart wird nur bei bogenförmigen Randausschnitten angezeigt.
  - **Absolute Koordinaten**: Bei dieser Einstellung wählen Sie die Ecke aus, von der aus gemessen werden soll.
  - **Abstand, Ecke, Kante**: Bei dieser Einstellung wählen Sie die Ecke und die Kante aus, von denen aus gemessen werden soll.
  [Image: Diagrams showing absolute and relative dimensioning for cutouts.]
- **Länge (b), Tiefe (a)**: Größe des Randausschnitts in mm. Das Feld wird nur bei eckigen Randausschnitten angezeigt.
- **Sehne (a)**: Größe des bogenförmigen Randausschnitts in mm. Das Feld wird nur bei Vermaßungsart 2 angezeigt.
- **Radius**: Radius des bogenförmigen Randausschnitts in mm. Der Radius wird von der Kante aus gemessen. Das Feld wird nur bei bogenförmigen Randausschnitten angezeigt.
- **Eckradius Aussen / Innen, Eckradius Aussen**: Eckradius für den Ausschnitt in mm.
- **Multi**: Die Bearbeitung kann ohne Parameter erfasst werden.
  - Für den Ausschnitt werden alle Parameter eingegeben.
  - Für den Ausschnitt werden nur die Anzahl der Bearbeitungen und die für die Preisfindung notwendigen Parameter eingeben. Diese Einstellung ist nur bei Angeboten sinnvoll.

### Innenausschnitte, Durchsprechöffnung, Handgriffe
- **Menge**: Anzahl der Ausschnitte, die angebracht werden sollen. Das Feld wird nur angezeigt, wenn die Checkbox **Multi** markiert ist.
- **Vermaßungsart**: Mit der Wahl der Vermaßungsart legen Sie fest, wie die eingegebenen Werte interpretiert werden sollen. Unter den Feldern wird jeweils eine Grafik angezeigt, aus der Sie ersehen können, wie die Werte angegeben werden müssen.
  ⇨ "Vermaßungstyp" auf Seite C-1747
- **X / Y / Ecke / Kante**: Maße und Bezugsecke bzw. Bezugskanten der Scheibe, von denen aus gemessen wird. Die Felder für die Vermaßung sind ausgeblendet, wenn die Checkbox **Multi** markiert ist.
- **Breite (a), Höhe (b)**: Größe des Ausschnitts in mm.
- **Winkel**: Winkel (in Grad) des Ausschnitts in Bezug zur Referenzkante. Der Ausschnitt wird gegen den Uhrzeigersinn gedreht.
- **zu Kante**: Referenzkante der Scheibe.
- **Referenz**: Auswahl der Ecke des Ausschnitts in Bezug zum Einfügepunkt des Vermaßungstyps. Mit dieser Angabe legen Sie fest, welche Ecke des Ausschnitts (oder ob der Mittelpunkt) sich auf den Einfügepunkt des Vermaßungstyps bezieht.

**Beispiele:**
[Image: Two diagrams illustrating how reference points and angles define the position of an internal cutout.]
*Diagram 1:*
- Referenzkante: 1
- Referenzpunkt: (Ecke) 1
- Drehwinkel: 0 °C
*Diagram 2:*
- Referenzkante: 3
- Referenzpunkt: (Ecke) 3
- Drehwinkel: 0 °C

**Legende:**
- **A**: Einfügepunkt (abhängig vom Vermaßungstyp)
- **B**: Referenzpunkt (Ecke des Ausschnitts)
- **C**: Referenzkante (Kante der Scheibe)
- **D**: Nummerierung der Referenzpunkte (Ecke 1 - 4)
- **E**: Referenzpunkt (Mittelpunkt = 9)

- **Innenradius**: Das Feld wird nur bei Innenausschnitten angezeigt. Radius der Ecken des Ausschnitts in mm.
- **Bearbeitungsseite**: Das Feld wird nur bei Handgriffen angezeigt. Standardmäßig ist Ebene/Level 1 als Bearbeitungsseite ausgewählt. Die Ebenen werden von außen nach innen gezählt.
- **Multi**: Die Bearbeitung kann ohne Parameter erfasst werden.
  - Für den Ausschnitt werden alle Parameter eingegeben.
  - Für den Ausschnitt werden nur die Anzahl der Bearbeitungen und die für die Preisfindung notwendigen Parameter eingeben. Diese Einstellung ist nur bei Angeboten sinnvoll.

### Beschichtung, Mattierung, Siebdruck, Flächen-Emaillierung, Sandstrahlen, Kolorieren
Für diese Bearbeitungen werden auch die Felder **Menge**, **X/Y/Ecke / Kante**, **Winkel**, **zu Kante**, **Referenz** und **Multi** angezeigt. Siehe dazu:
⇨ “Innenausschnitte, Durchsprechöffnung, Handgriffe" auf Seite C-1752
- **Vermaßungsart**: Mit der Wahl der Vermaßungsart legen Sie fest, wie die eingegebenen Werte interpretiert werden sollen. Unter den Feldern wird jeweils eine Grafik angezeigt, aus der Sie ersehen können, wie die Werte angegeben werden müssen.
  - **Absolute Koordinaten**: Bei dieser Einstellung wählen Sie die Ecke aus, von der aus gemessen werden soll.
  - **Abstand zu 2 Kanten**: Bei dieser Einstellung wählen Sie die beiden Kanten aus, von denen aus gemessen werden soll.
  - **Ecke, Kante, Abstand zur Kante**: Bei dieser Einstellung wählen Sie die Ecke und die Kante aus, von denen aus gemessen werden soll.
  [Image: Icons illustrating the three dimensioning types.]
- **Breite (a), Höhe (b)**: Größe der zu bearbeitenden Fläche. Standardmäßig werden die Maße der Scheibe angezeigt.
  - **Beschichtung, Mattierung, Siebdruck, Flächen-Emaillierung, Sandstrahlen, Kolorieren**: Wenn nicht die gesamte Fläche bearbeitet werden soll, können Sie die Maße frei angeben.
  - **Motiv**: Wenn Sie ein Motiv auswählen, können Sie die Maße wie folgt ändern:
    - Wenn Sie im Feld **Nummer** die Siebnummer eines Motivs angeben, ist die Größe des Motivs durch die maximalen Abmessungen in den Stammdaten begrenzt. Sie können die maximale Breite und Höhe nicht überschreiten. Wenn Sie Maße innerhalb der Abmessungen des Siebs angeben, wird das Motiv beschnitten.
    - Wenn Sie ein Motiv ohne Siebnummer einfügen, können Sie die Maße frei angeben. Sie können den Skalierungsmodus des Motivs in der Kombobox **Skalierung** wählen.
      ⇨ "(Skalierung)" auf Seite C-1755
- **Variante**: Auswahl der Varianten (Farben), wenn für die gewählte Bearbeitung Varianten hinterlegt sind.
- **Nummer**: Nummer, die an die Produktion übergeben wird. Diese Angabe ist optional. Wenn Sie die Siebnummer eingeben, wird im Feld **Motiv** die Motivdatei angezeigt. Die Kombobox für die Skalierung wird gesperrt.
  ⇨ "Motive" auf Seite B-774
- **Sättigung**: Die Sättigung gibt an, wie intensiv die Beschichtung, Mattierung, Emaillierung, Sandstrahlen oder Farbe des Siebdrucks oder Kolorierens aufgetragen wird.
- **Bearbeitungsseite**: Standardmäßig ist Ebene/Level 1 als Bearbeitungsseite ausgewählt. Die Ebenen werden von außen nach innen gezählt.
Die folgenden Felder müssen Sie nur füllen, wenn Sie ein Motiv einfügen möchten.
- **Motiv**: Pfad und Name der Motivdatei.
  - Wenn Sie eine Siebnummer im Feld **Nummer** eintragen, wird ein Dateipfad angezeigt.
  - Wenn Sie keine Siebnummer eintragen, können Sie eine Motivdatei über die Schaltfläche [Ordner] wählen.
- **(Skalierung)**: Skalierung des Motivs. Sie können eine Skalierung nur wählen, wenn Sie das Motiv als Datei einfügen.
  - **Frei skalierbar**: Sie können Höhe und Breite des Motivs frei angeben. Das Motiv wird nicht proportional skaliert.
  - **Proportional Breite**: Sie können die Breite des Motivs angeben. Die Höhe des Motivs wird proportional zur Breite angepasst.
  - **Proportional Höhe**: Sie können die Höhe des Motivs angeben. Die Breite des Motivs wird proportional zur Höhe angepasst.
  - **Nicht skaliert**: Dieser Modus ist nur bei Angabe einer Siebnummer sinnvoll. Bei Angabe einer Siebnummer ist dieser Modus voreingestellt. Sie können Höhe und Breite des Motivs innerhalb der Abmessungen des Siebs frei angeben. Das Motiv wird beschnitten.
> **Motive beschneiden**
> Für die Beschneidung stehen folgende Möglichkeiten zur Verfügung:
> - Wenn Sie proportional skalieren, wird das Motiv u. U. beschnitten. In der Regel ist das Motiv ein Ausschnitt (Mitte) aus dem Gesamtmotiv.
> - Wenn Sie das Motiv über die Siebnummer einfügen, können Sie das Motiv nur innerhalb der Abmessungen des Siebs skalieren. Wenn die angegebenen Maße in den Feldern **Breite (a) / Höhe (b)** kleiner sind als die Maße des Siebs, wird das Motiv beschnitten. Im Allgemeinen ist das Motiv ein Ausschnitt (links unten) aus dem Gesamtmotiv.
- **Spiegeln**: Sie können das Motiv spiegeln.
  - Das Motiv wird nicht gespiegelt.
  - Das Motiv wird horizontal gespiegelt.
Eine Vorschau der Bearbeitung wird in der technischen Zeichnung in der linken unteren Ecke des Dialogs angezeigt.

### Randentschichtungen
- **Menge**: Das Feld ist gesperrt.
- **Alle Kanten, (Kante) 1-8**: Auswahl der Kanten, an denen die Randentschichtung ausgeführt werden soll.
  - Die Randentschichtung wird nicht ausgeführt.
  - Die Randentschichtung wird ausgeführt.
- **Breite**: Breite der Randentschichtung in mm.
- **Ebene**: Die Ebenen werden von außen nach innen gezählt. Die Auswahl gibt an, auf welcher Seite die Bearbeitung ausgeführt werden soll.

### Biegen
- **Menge**: Anzahl der Biegungen. Standardmäßig wird nur eine Biegung eingetragen.
- **Breite**: Angabe, wie weit das Glas gebogen werden soll (Sehnenmaß).
- **Höhe**: Angabe, wie hoch die Kante im Vergleich zum ebenen Glas gebogen werden soll (Stichhöhe).
Wenn Sie die Kanten unterschiedlich biegen möchten, müssen Sie für jede Biegung eine eigene Bearbeitung anlegen, um eine Biegung in der Vertikalen und in der Horizontalen festzulegen.
Die Randentschichtung wird im Register **Weitere Angaben** angezeigt.
⇨ "Positionen - Weitere Angaben" auf Seite C-1786

### Rillenschliff
- **Menge**: Das Feld ist gesperrt.
- **Alle Kanten, (Kante) 1-8**: Auswahl der Kanten, an denen die Rillen geschliffen werden sollen.
  - An der Kante wird keine Rille geschliffen.
  - An der Kante wird (mindestens) eine Rille geschliffen.
- **Länge der Kante**: Standardmäßig werden die Kantenlängen der Scheibe angezeigt. In der Regel entspricht die Länge der Rille der Kantenlänge.
- **X / Y**: Abstand von den Kanten. Die Maße gelten für alle Rillen. Wenn Sie einen asymmetrischen Aufbau der Rillen möchten, müssen Sie für jede Rille eine eigene Bearbeitung anlegen.
- **Schliffnummer**: Die Schliffnummer gibt an, nach welcher Art die Rille geschliffen werden soll.
- **Breite (b)**: Breite der Rillen.
- **Bearbeitungsseite**: Angabe der Ebene, auf der die Bearbeitung ausgeführt werden soll. Standardmäßig ist Ebene/Level 1 ausgewählt. Sie müssen diese Angabe daher zwingend prüfen. Die Ebenen werden von außen nach innen gezählt.

### Nachschleifen, Kantenschutz
- **Menge**: Das Feld ist gesperrt.
- **Alle Kanten, (Kante) 1-8**: Auswahl der Kanten, die nachgeschliffen bzw. für den Transport geschützt werden sollen.
  - Die Kante wird nicht bearbeitet.
  - Die Kante wird bearbeitet.
- **Gehrungswinkel**: Winkel in Grad für den Schliff. Das Feld wird nur beim Nachschleifen angezeigt.

### Logo, Stempel
Für diese Bearbeitungen werden auch die Felder **Vermaßungstyp**, **Breite (a) / Höhe (b)**, **Winkel**, **zu Kante** und **Referenz** angezeigt. Siehe dazu:
⇨ "Innenausschnitte, Durchsprechöffnung, Handgriffe" auf Seite C-1752
- **Typ**: Auswahl des Logo-Typs.
- **Nummer**: Nummer des Logos, die in den Stammdaten des Kunden hinterlegt ist. Sie wird die an die Produktion übergeben.
- **Distanz A/B**: Abstand von der Bezugsecke (A) und Bezugskante (B).
- **Ecke / Kante**: Angabe der Bezugsecke und Bezugskante.
- **Ebene**: Ebene, auf der das Logo angebracht werden soll. Standardmäßig ist Ebene/Level 1 ausgewählt. Sie müssen diese Angabe daher zwingend prüfen. Die Ebenen werden von außen nach innen gezählt.

### Makro Ecke, Makro Rand, Parametrisierbares Makro (Kante)
Mit dieser Wahl können Sie Eck- oder Randausschnitte angeben, die als SN-Makro gespeichert sind.
- **Menge**: Anzahl der Ausschnitte, die angebracht werden sollen. Das Feld wird nur angezeigt, wenn die Checkbox **Multi** markiert ist, ist jedoch gesperrt. Es wird gefüllt, wenn im Bereich **Alle Ecken/Kanten, (Ecke/Kante) 1 – 8** die Anzahl der Eck- oder Randausschnitte ausgewählt wird.
- **Alle Ecken/Kanten, (Ecke/Kante) 1-8**: Auswahl der Ecken oder Kanten, an denen die Bearbeitung ausgeführt werden soll. Die Felder werden nur angezeigt, wenn die Checkbox **Multi** markiert ist. In den Feldern geben Sie an, wie viele Bearbeitungen ausgeführt werden sollen.
  - Keine Bearbeitung wird ausgeführt.
  - An der Ecke/Kante wird (mindestens) eine Bearbeitung ausgeführt.
- **Abstand**: Das Feld wird durch die Werte aus dem Makro gefüllt, wenn diese in den Produktstammdaten des Makros erfasst sind. Das Feld wird nicht bei Makro Ecke angezeigt.
- **Ecke / Kante**: Angabe der Ecke und Kante, an der die Bearbeitung ausgeführt werden soll.
- **Makroname**: Dateiname des ausgewählten SN-Makros.
  - Über das Ordner-Symbol können Sie eine andere Datei auswählen.
  - Über die Lupe können Sie einen Dialog mit der Modellskizze öffnen.
- **Multi**: Die Bearbeitung kann ohne Parameter erfasst werden.
  - Für den Ausschnitt werden alle Parameter eingegeben.
  - Für den Ausschnitt werden nur die Anzahl der Bearbeitungen und die für die Preisfindung notwendigen Parameter eingeben. Diese Einstellung ist nur bei Angeboten sinnvoll.
- **(Parameter)**: Die Tabelle zeigt die Parameter des ausgewählten Makros. Sie können die Parameter in der Tabelle anpassen. Die Tabelle wird nur beim parametrisierbaren Makro angezeigt.

### Emaillierung
- **Menge**: Das Feld ist gesperrt.
- **Alle Kanten, (Kante) 1-8**: Angabe der Kanten, an denen die Bearbeitung ausgeführt werden soll.
  - Die Kante wird nicht bearbeitet.
  - Die Kante wird bearbeitet.
- **Tiefe (a)**: Tiefe der Emaillierungsschicht (Streifen). Die Tiefe wird aus dem Rückschnitt und der Breite des SZR ermittelt.
- **Kantenabstand (x)**: Abstand von den Kanten. Die Maße gelten für alle Kanten.
- **Bearbeitungsseite**: Angabe der Ebene, auf der die Bearbeitung ausgeführt werden soll. Standardmäßig ist die Ebene/Level 1 als Bearbeitungsseite ausgewählt. Die Ebenen werden von außen nach innen gezählt.

### Alarmspinne
**Ausgang an Ecke**: Die Bezugsecke kann frei gewählt werden. Weitere Angaben zu Maßen sind nicht erforderlich.

### Bleiverglasung
Die Bleiverglasungen sind separat beschrieben.
⇨ "Positionen - Bleiverglasungen" auf Seite C-1767

### Gebogenes Glas
Gebogenes Glas ist separat beschrieben.
⇨ "Positionen - Gebogenes Glas" auf Seite C-1765

### Abkleben
- **Menge**: Das Feld ist gesperrt.
- **Alle Kanten, (Kante) 1-8**: Auswahl der Kanten, an denen die Randbeschichtung ausgeführt werden soll.
  - Die Randbeschichtung wird nicht ausgeführt.
  - Die Randbeschichtung wird ausgeführt.
- **Breite**: Breite der Randbeschichtung in mm.
- **Ebene**: Die Ebenen werden von außen nach innen gezählt. Die Auswahl gibt an, auf welcher Seite die Bearbeitung ausgeführt werden soll.

### Entschichtung
- **Menge**: Anzahl der Ausschnitte, die angebracht werden sollen. Das Feld wird nur angezeigt, wenn die Checkbox **Multi** markiert ist.
- **Vermaßungsart**: Mit der Wahl der Vermaßungsart legen Sie fest, wie die eingegebenen Werte interpretiert werden sollen. Unter den Feldern wird jeweils eine Grafik angezeigt, aus der Sie ersehen können, wie die Werte angegeben werden müssen.
  ⇨ "Vermaßungstyp" auf Seite C-1747
- **X / Y / Ecke / Kante**: Maße und Bezugsecke bzw. Bezugskanten der Scheibe, von denen aus gemessen wird. Die Felder für die Vermaßung sind ausgeblendet, wenn die Checkbox **Multi** markiert ist.
- **Breite (a), Höhe (b)**: Größe des Ausschnitts in mm.
- **Winkel**: Winkel (in Grad) des Ausschnitts in Bezug zur Referenzkante. Der Ausschnitt wird gegen den Uhrzeigersinn gedreht.
- **zu Kante**: Referenzkante der Scheibe.
- **Referenz**: Auswahl der Ecke des Ausschnitts in Bezug zum Einfügepunkt des Vermaßungstyps. Mit dieser Angabe legen Sie fest, welche Ecke des Ausschnitts (oder ob der Mittelpunkt) sich auf den Einfügepunkt des Vermaßungstyps bezieht.
- **Bearbeitungsseite**: Angabe der Ebene, auf der die Bearbeitung ausgeführt werden soll. Standardmäßig ist die Ebene/Level 1 als Bearbeitungsseite ausgewählt. Die Ebenen werden von außen nach innen gezählt.
- **Multi**: Die Bearbeitung kann ohne Parameter erfasst werden.
  - Für den Ausschnitt werden alle Parameter eingegeben.
  - Für den Ausschnitt werden nur die Anzahl der Bearbeitungen und die für die Preisfindung notwendigen Parameter eingeben. Diese Einstellung ist nur bei Angeboten sinnvoll.

### Randsiebdruck
- **Menge**: Das Feld ist gesperrt.
- **Alle Kanten, (Kante) 1-8**: Auswahl der Kanten, an denen der Randsiebdruck ausgeführt werden soll.
  - Der Randsiebdruck wird nicht ausgeführt.
  - Der Randsiebdruck wird ausgeführt.
- **Breite**: Breite des Randsiebdrucks in mm.
- **Ebene**: Die Ebenen werden von außen nach innen gezählt. Die Auswahl gibt an, auf welcher Seite die Bearbeitung ausgeführt werden soll.
- **Variante**: Auswahl der Varianten (Farben), wenn für die gewählte Bearbeitung Varianten hinterlegt sind.
- **Nummer**: Nummer, die an die Produktion übergeben wird.
- **Sättigung**: Die Sättigung gibt an, wie intensiv der Randsiebdruck aufgetragen werden soll.

### Makro Innen, Parametrisierbares Makro (Innen)
- **Menge**: Anzahl der Ausschnitte, die angebracht werden sollen. Das Feld wird nur angezeigt, wenn die Checkbox **Multi** markiert ist.
- **Vermaßungsart**: Mit der Wahl der Vermaßungsart legen Sie fest, wie die eingegebenen Werte interpretiert werden sollen. Unter den Feldern wird jeweils eine Grafik angezeigt, aus der Sie ersehen können, wie die Werte angegeben werden müssen.
  ⇨ "Vermaßungstyp" auf Seite C-1747
- **X/Y/Ecke / Kante**: Maße und Bezugsecke bzw. Bezugskanten der Scheibe, von denen aus gemessen wird. Die Felder für die Vermaßung sind ausgeblendet, wenn die Checkbox **Multi** markiert ist.
- **Winkel**: Winkel (in Grad) des Ausschnitts in Bezug zur Referenzkante. Der Ausschnitt wird gegen den Uhrzeigersinn gedreht.
- **zu Kante**: Referenzkante der Scheibe.
- **Makroname**: Dateiname des ausgewählten SN-Makros.
  - Über das Ordner-Symbol können Sie eine andere Datei auswählen.
  - Über die Lupe können Sie einen Dialog mit der Modellskizze öffnen.
- **Multi**: Die Bearbeitung kann ohne Parameter erfasst werden.
  - Für den Ausschnitt werden alle Parameter eingegeben.
  - Für den Ausschnitt werden nur die Anzahl der Bearbeitungen und die für die Preisfindung notwendigen Parameter eingeben. Diese Einstellung ist nur bei Angeboten sinnvoll.
- **(Parameter)**: Die Tabelle zeigt die Parameter des ausgewählten Makros an. Sie können die Parameter in der Tabelle anpassen. Die Tabelle wird nur beim parametrisierbaren Makro angezeigt.

### Artikel
**Beschläge**: In der Übersicht werden alle Beschläge aufgelistet, die dem Produkt angehängt sind.
Folgende Felder werden angezeigt:
- **Bereich**: Anbringung und/oder Art des Beschlags, z. B. Griffstange, Schloss oder Band oben, Band mitte, Band unten.
- **Prod Nr.**: Produktnummer des Beschlags.
- **Bezeichnung**: Name des Beschlags.
- **Variante**: Aktuelle Variante (Farbe) des Beschlags.
- **Suche**: Auswahl der Variante (Farbe), wenn für den gewählten Beschlag Varianten hinterlegt sind.
- **Sonderfarbe**: Sonderfarbe, die für den Beschlag verwendet wird.

**Bandseite**: Seite, auf der das Band angebracht wird. Sie können zwischen den Optionen **Links** und **Rechts** wählen. Beim Wechsel der Bandseite werden die Beschläge automatisch getauscht, wenn in den Stammdaten für die Bandseiten unterschiedliche Artikel hinterlegt sind.

**Gemeinsame Variante**: Auswahl der gemeinsamen Variante (Farbe) für alle Beschläge in der Übersicht.
Eine gemeinsame Variante kann nur gewählt werden, wenn für die Beschläge in der Übersicht die gleiche Variante hinterlegt ist.
Wenn eine Sonderfarbe als gemeinsame Variante gewählt wird, wird hinter der Kombobox ein zusätzliches Textfeld angezeigt, in dem die Sonderfarbe angegeben wird.

## Positionen – Stufung
**Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Modelle/Bearbeitungen > Auswahl Stufung**

[Image: Screenshot of the 'Stufung' (Stepped IGU) screen. It shows a diagram of a stepped insulating glass unit and fields to enter the step dimensions for each pane.]

In diesem Register erfassen Sie die Stufen zu einer ISO-Einheit. Die Bereiche **Stückliste**, **Bearbeitung** und **Verkaufspreise** sind zum Register **Modelle/Bearbeitungen** erklärt.
⇨ "Positionen - Modelle/Bearbeitungen" auf Seite C-1740
⇨ Tutorial, "Modell erfassen" auf Seite C-1368

### Bearbeitung
[Image: Icon for the 'Stufung' machining type.]
Über die Schaltflächen wählen Sie die Bearbeitung **Stufung** aus.

### Parameter
Zur ausgewählten Position werden die Felder entsprechend der Anzahl der Scheiben anzeigt.
In den Checkboxen geben Sie an, für welche Scheibe die Maße gelten. Die Checkbox 1 bezeichnet die Außenscheibe. Wenn die Checkbox 2 markiert ist, müssen positive Werte in den Feldern eingetragen werden, z. B. den Wert 15.

**S1-Sn**: Größe der Stufung pro Scheibe in der Einheit.

### Skizzendruck, Preise
Diese Felder sind ausführlich zu Modellen beschrieben.
⇨ "Positionen - Modelle/Bearbeitungen" auf Seite C-1740

## Positionen – Gebogenes Glas
**Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Modelle/Bearbeitungen > Auswahl Gebogenes Glas**

[Image: Screenshot of the 'Gebogenes Glas' (Bent Glass) screen. It shows parameters for defining the curve, such as chord, height, and radius.]

In diesem Dialog können Sie Daten für ein gebogenes Glas eingeben. Die Bereiche **Stückliste**, **Bearbeitung** und **Verkaufspreise** sind zum Register **Modelle/Bearbeitungen** erklärt.
⇨ "Positionen - Modelle/Bearbeitungen" auf Seite C-1740

### Bearbeitung
[Image: Icon for the 'Gebogenes Glas' machining type.]
Über die Schaltflächen wählen Sie die Bearbeitung **Gebogenes Glas** aus.

### Parameter
- **Sehnenmaß**: Länge zwischen den inneren Kanten des gebogenen Glases
- **Stichhöhe**: Höhe zwischen der Kante und dem Scheitelpunkt der Biegung
- **Abwicklung**: Äußere Länge der Biegung zwischen den Kanten
- **Radius**: Radius der Biegung
- **Außen, Neutral, Innen**: Anzeige der errechneten Werte, wenn die Maße für Sehne/Stichhöhe oder Abwicklung/Radius eingetragen sind.
- **Format**: Die Art der Formung, wenn Beschichtungen oder Strukturen berücksichtigt werden müssen.
  - **Innen**: Die Scheibe wird so gebogen, dass die Biegung innen (im Raum) liegt.
  - **Außen**: Die Scheibe wird so gebogen, dass die Biegung außen liegt.
- **Gradmaß**: Das Gradmaß wird automatisch errechnet.

### Skizzendruck, Preise
Diese Felder sind ausführlich zu Modellen beschrieben.
⇨ "Positionen - Modelle/Bearbeitungen" auf Seite C-1740

## Positionen – Bleiverglasungen
**Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Modell/Bearbeitungen > Auswahl Bleiverglasung**

[Image: Screenshot of the 'Bleiverglasungen' (Leaded Glass) screen. It shows a schematic of the leaded glass pattern.]

In diesem Dialog erfassen Sie Bleiverglasungen zu einer Position. Nach der Wahl des Produktes und des Musters werden die Daten in die Stückliste übernommen.
Die Bereiche **Stückliste**, **Bearbeitung** und **Verkaufspreise** sind zum Register **Modelle/Bearbeitungen** erklärt.
⇨ "Positionen – Modelle/Bearbeitungen" auf Seite C-1740

### Bearbeitung
[Image: Icon for the 'Bleiverglasung' machining type.]
Über die Schaltflächen wählen Sie die Bleiverglasung aus.

### Skizzendruck, Preise
Diese Felder sind ausführlich zu Modellen beschrieben.
⇨ "Positionen - Modelle/Bearbeitungen" auf Seite C-1740

## Positionen – Modell-Template
**Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Modelle/Bearbeitungen > Auswahl S+N-Datei**

[Image: Screenshot of the 'Modell-Template' screen. It shows a free-form shape (Modell 99) and fields for loading an S+N template file.]

In diesem Register erfassen Sie ein Modell über ein Template. Die Felder sind nur freigeschaltet, wenn Sie ein Template ausgewählt haben.
Die Bereiche **Stückliste**, **Bearbeitung** und **Verkaufspreise** sind zum Register **Modelle/Bearbeitungen** erklärt.
⇨ “Positionen – Modelle/Bearbeitungen" auf Seite C-1740

Bearbeitungen können auch zu Modell 99 und zu importierten SN-Dateien erfasst werden. Die Bearbeitungen werden in der SN-Datei gespeichert.
Dazu müssen folgende Voraussetzungen erfüllt sein:
- **Firmendaten – Register System**: Checkbox **Kantenbearbeitungen und Bohrungen auf Modell 99** muss aktiviert sein.
- A+W CAD Designer (Shapes) muss installiert sein.

Auf einer freien Form (Modell 99) können Kantenbearbeitungen nur an allen Kanten zusammen angebracht werden. Die Maße für Bohrungen können nur mit Bezug auf das umschriebene Rechteck angegeben werden.
Bei einem Standardmodell aus einer SN-Datei können Kantenbearbeitungen auf einzelnen Kanten erfasst werden, wenn die Kanten in der SN-Datei nummeriert sind.

### Modellparameter, Restriktionen
Zu jedem Template werden die Parameter mit den Standardwerten anzeigt. Die Werte können Sie überschreiben. Die neuen Werte werden nicht in das Template zurückgeschrieben.
Im Bereich **Restriktionen** wird angezeigt, welche Größenvorgaben zu dem gewählten Modell bestehen. Dabei steht **H** für Höhe und **W** für Breite.
⇨ Tutorial, "SN-Datei und Template" auf Seite C-1430

[Image: Screenshot showing a selected S+N template with its specific parameters filled in.]

### S+N Datei
Sie können das Template über die Schaltfläche [Ordner] auswählen und der Auftragsposition zuordnen. Außer S+N-Dateien können auch Dateien im DFX- und im SHP-Format geladen werden.
- Sie möchten keine Datei auswählen oder die Angaben nicht als S+N-Datei speichern.
- Sie können ein Template auswählen oder die aktuellen Werte als S+N-Datei speichern. Die Schaltflächen und das Eingabefeld werden freigeschaltet.
Die gewünschte Datei können Sie entweder über die Schaltfläche auswählen oder den Pfad und Dateinamen in das Eingabefeld schreiben.
Beim Speichern wird automatisch ein Unterverzeichnis mit dem aktuellen Jahr und Monat als Namen angelegt und die Datei unter einer fortlaufenden Nummer gespeichert.

### Umschriebenes Rechteck
Die Werte werden automatisch errechnet. Sie werden standardmäßig zur Preisberechnung herangezogen. In den Firmendaten kann eingestellt werden, dass die tatsächliche Fläche zur Preisberechnung herangezogen werden soll.
⇨ Stammdaten, "Tatsächliche Modellfläche zur Preisberechnung nutzen" auf Seite B-1090

### Skizzendruck, Preise
Diese Felder sind ausführlich zu Modellen beschrieben.
⇨ "Positionen - Modelle/Bearbeitungen" auf Seite C-1740

## Positionen – Sprossen
**Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Sprossen**

In diesem Register finden Sie weitere Register:
- "Sprossen - Standard" auf Seite C-1771
- "Sprossen - Preise" auf Seite C-1776
- "Sprossen - Wegfallsprossen" auf Seite C-1778
- "Sprossen - Muster" auf Seite C-1779

### Sprossen – Standard
**Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Sprossen > Register Standard**

[Image: Screenshot of the 'Sprossen - Standard' tab. It shows a graphical representation of a mullion grid and fields for defining horizontal and vertical mullions.]

In diesem Register erfassen Sie eine Sprossenkonstruktion. Das gewählte Sprossenschema wird als Grafik angezeigt, sobald Sie in den Bereichen **Waagerechte, Senkrechte Sprossen** eine Sprosse ausgewählt haben.
⇨ Tutorial, "Sprossen erfassen" auf Seite C-1363

#### Auswahl Schema
Über die Schaltflächen wählen Sie eine Standardkonstruktion für die Sprossen aus.

#### Einbauposition
**Abstandhalter**: Wenn Sie die Sprossen in einem Mehrfach-ISO erfassen, können Sie festlegen, in welchen Zwischenräumen die Abstandhalter eingebaut werden sollen. Mit dieser Schaltfläche übertragen Sie die Einstellungen auf alle Abstandhalter.

#### Waagerechte, Senkrechte Sprossen
Die Felder werden dem Sprossenmuster entsprechend freigeschaltet, das Sie gewählt haben.
- **Artikel**: Produktnummer der Sprossen. Die Bezeichnung wird aus den Produktdaten übernommen.
- **Durchgang**: Angabe der durchgehenden Sprossenrichtung. Wenn Sie keine Checkbox markieren, werden alle Sprossen mit Gehrungen aneinandergesetzt.
  - Die Sprossen dieser Richtung werden geschnitten.
  - Die Sprossen dieser Richtung sind durchgängig.
- **Variante**: Auswahl einer Varianten (Farbe) der Sprossen.
- **Breite**: Sprossenbreite aus den Produktdaten. Sie können den Wert überschreiben.
- **Anzahl**: Die Anzahl wird aus dem gewählten Muster übernommen. Sie können so viele Sprossen einfügen, wie Sie wünschen. Die Grafik wird automatisch aktualisiert.
- **Dicke**: Sprossendicke aus den Produktdaten.
- **Typ**: Sprossentyp aus den Produktdaten.
- **Bohrmaße**: Die Bohrmaße können automatisch berechnet oder manuell eingetragen werden. Um manuelle Werte eintragen zu können, müssen Sie im Feld **Berechnungsart** eine asymmetrische Einstellung wählen.

> **Bohrmaße als letzte Eingabe festlegen**
> Wenn Sie die Bohrmaße manuell festlegen, sollten Sie zuerst alle anderen Felder ausgefüllt haben. Die manuellen Werte werden jeweils überschrieben, wenn Sie irgendeine Änderung vornehmen.

#### Verkaufspreise
- **Jahrgang / Schlüssel**: Preisjahrgang und -schlüssel aus den Produktdaten. Beide Einstellungen können geändert werden.
- **Preis / PE**: Der Gitterpreis wird automatisch errechnet. Änderungen in diesem Feld betreffen immer den Gesamtpreis des Gitters. Der Gesamtgitterpreis wird immer als Stückpreis angezeigt.

> **Preise ändern**
> Die Preise der Sprossen können Sie sich unter der Grafik im Register **Preise** anzeigen lassen. Dort können Sie die Preise und Preiseinheiten jeweils für die waagerechten und senkrechten Sprossen ändern.
> Geänderte Preise können Sie über das Menü **Funktionen > Vorgaben löschen** zurücksetzen.

Bei der Berechnung des Gitterpreises werden die Vorgaben für die Mindestlänge berücksichtigt.
⇨ Stammdaten, “Sprossenmindestlänge pro Gitter berechnen" auf Seite B-1088
- **Rabatt**: Rabatt aus den Produktdaten. Er kann geändert werden.
- **Netto**: Der Nettopreis für das gesamte Sprossengitter wird aus dem Gitterpreis und dem Rabatt automatisch errechnet. Er kann nicht geändert werden.

#### Konstruktion / Darstellung
- **Rückschnitt**: Der Rückschnitt wird bei der automatischen Berechnung der Sprossenlänge berücksichtigt. Der eingetragene Wert gilt für alle Kanten. Er wird aus der EK-Kalkulation übernommen. Sie können ihn überschreiben. Über die Schaltfläche können Sie den Rückschnitt pro Kante angeben.
  ⇨ "Rückschnitt" auf Seite C-1876
  Die Werte werden in die entsprechenden Felder im Rückschnitt im Register **Zusatz** übernommen.
  ⇨ "Positionen - Zusatz" auf Seite C-1782
- **Noppen**: Auf den Sprossenkreuzen können Noppen angebracht werden, wenn die Sprossendicke sehr viel geringer ist als der Abstandhalter. Die Noppen können wahlweise berechnet werden.
  - Die Noppen werden nicht eingebaut.
  - Die Noppen werden eingebaut.
  ⇨ "Sprossennoppen" auf Seite C-1701
- **Skizzendruck**: Sie können auswählen, wie die Sprossenkonstruktion im Druck wiedergegeben werden soll:
  - **Kein Druck**: Die Sprossenskizze wird nicht auf den Formularen gedruckt.
  - **Sprosse (maßstäblich)**: Bei dieser Einstellung werden maßstabsgetreue Sprossenskizzen gedruckt.
  - **Sprosse (schematisch)**: Bei dieser Einstellung werden die Standardskizzen gedruckt. Sie geben lediglich das Schema der Sprossen wieder.
  ⇨ Tutorial, "Druck von Skizzen" auf Seite C-1456
- **Berechnungsart**: Bohrungen werden angebracht, um die Sprossen im Rahmen zu befestigen. Die Maße werden dazu automatisch berechnet, wenn Sie eine symmetrische Sprossenkonstruktion wählen. Bei einer asymmetrischen Konstruktion werden die Felder freigeschaltet, in denen Sie die Maße eingeben können. Die Berechnungsart bestimmt, wie die Bohrungen angebracht werden sollen. Ein Beispiel finden Sie im Part Stammdaten.
  - **0 - bohrpunkt-symmetrisch**: Die Bohrungen werden automatisch berechnet. Sie werden symmetrisch im Abstandhalter angebracht. Dadurch werden die Felder bei mehr als einer Sprosse pro Richtung unterschiedlich groß. Bei sehr breiten Sprossen ist der Unterschied deutlich sichtbar.
  - **1 - feld-symmetrisch**: Die Bohrungen werden automatisch berechnet. Sie werden so angebracht, dass alle Felder gleich groß sind. Die Abstände der Bohrungen berücksichtigen die Breite der Sprossen und werden daher unterschiedlich groß.
  - **2 - bohrpunkt-asymmetrisch**: Sie können die Bohrmaße manuell ändern. Diese Einstellung müssen Sie wählen, wenn Sie bestimmte Vorgaben für die Bohrungen einhalten müssen.
  - **3 - feld-asymmetrisch**: Sie können die Bohrmaße manuell ändern. Diese Einstellung müssen Sie wählen, wenn Sie bestimmte Vorgaben für die Felder einhalten müssen. Dazu müssen Sie anhand der Sprossenbreite die Bohrungen selbst errechnen.
  - **4 - gleiche Stablänge**: Die Bohrpunkte werden so berechnet, dass alle Stäbe die gleiche Länge haben.
  - **5 - bohrpunkt-sym. Glaskante**: Die Bohrungen werden automatisch berechnet. Sie werden symmetrisch im Abstandhalter angebracht. Als Bezugsgröße wird die Glaskante herangezogen.
  - **6- bohrpunkt-asym. Glaskante**: Sie können die Bohrmaße manuell ändern. Als Bezugsgröße wird die Glaskante herangezogen.

**Berechnungsart wählen**: Sie können die Berechnungsart auch über das Menü **Berechnung** auswählen.
⇨ Stammdaten, "Berechnungsart für die Sprossenkonstruktion" auf Seite B-228

**Bohrpunkt-Vermaßung**: Mit der Wahl der Option legen Sie fest, wie die Eingaben für die Bohrpunkte gewertet werden sollen:
- **auf Bezugspunkt**: Jedes Maß wird vom Bezugspunkt aus gerechnet. Der Bezugspunkt liegt dabei immer in der Ecke unten links.
- **als Kettenmaß**: Die Werte werden von einem Bohrpunkt zum nächsten gewertet.
Wenn Sie die Option wechseln, wird die Anzeige in der Grafik entsprechend angepasst. Wenn Sie bei einer asymmetrischen Berechnungsart bereits Werte für die Bohrpunkte eingegeben haben, werden auch diese Werte angepasst.

### Sprossen - Preise
**Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Sprossen > Register Preise**

[Image: Screenshot of the 'Sprossen - Preise' tab. It shows a detailed price breakdown for different components of the mullion grid.]

In diesem Register bearbeiten Sie die Preise für die gesamte Sprossenkonstruktion.

#### Sprossenartikel
Unter der Grafik werden die Preise für die waagerechten und die senkrechten Sprossen getrennt angezeigt. Die Anzeige bezieht sich auf Verkaufs- oder Einkaufspreise. Sie kann über das Menü **Ansicht** umgestellt werden.
- **Menge**: Gesamtlänge der eingebauten Sprossen pro Richtung insgesamt.
- **Preis, Preiseinheit**: Die Werte werden aus der Preisliste übernommen, die im Bereich **Preise** ausgewählt ist.
Die Preise für die waagerechten und senkrechten Sprossen können sowohl im Feld **Menge** als auch im Feld **Preis** überschrieben werden.

#### Gitter
Für die Bestandteile der Konstruktion werden die Preise und Preiseinheiten getrennt angezeigt. Die Anzeige bezieht sich auf Verkaufs- oder Einkaufspreise.
Die Berechnung kann pro Randstopfen, Kreuz, Feld oder für T-Sprossen usw. durchgeführt werden. Der Gesamtpreis für das Gitter wird im Bereich **Preise** angezeigt.

**Sprossenartikel**: Mit der Wahl eines Eintrags und mit der Einstellung im Feld **Filter** legen Sie die Anzeige der Sprossenpreiselemente fest:
- **Alle**: Alle Elemente werden aufgelistet.
- **Geschnitten**: Geschnittene Sprossen werden angezeigt.
- **Aluminium-Sprosse - Senkrecht, Waagerecht**: ALU-Sprossen werden angezeigt.

> **Preisänderungen zurücksetzen**
> Wenn Sie die Änderungen nicht übernehmen möchten, können Sie die Standard-Preise über das Menü **Funktionen > Vorgaben löschen** wieder einsetzen lassen.

**Filter**: Sie können die Anzeige der Sprossenpreiselemente auf diejenigen reduzieren:
- **Alle**: Alle Elemente werden aufgelistet.
- **Menge < > 0**: Anzeige der Elemente, für die eine Menge gefunden wurde.
- **Nur Individuelle**: Anzeige der individuellen Elemente.
- **Standard**: Standard-Modus der vorherigen Version.

### Sprossen – Wegfallsprossen
**Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Sprossen > Register Wegfallsprossen**

[Image: Screenshot of the 'Wegfallsprossen' (Omitted Mullions) tab. It shows a mullion grid with checkboxes to omit certain segments, including diagonal ones.]

In diesem Register bearbeiten Sie das Sprossenschema. Asymmetrische Muster und gebogene Sprossen können Sie im Register **Muster** erfassen.

#### Diagonalsprossen
Sie können angeben, welcher Sprossenabschnitt diagonal eingebaut werden soll. Die Checkboxen bezeichnen jeweils die Randfelder.
- Der Sprossenabschnitt wird nicht eingebaut.
- Der Sprossenabschnitt wird eingebaut.

> **Produktionsübergabe von Diagonalsprossen**
> Dokumente mit Diagonalsprossen können nicht direkt an die Produktion übergeben werden. Die betroffenen Dokumenten- und Positionsnummern werden in einer Meldung angezeigt.

#### Waagerechte, Senkrechte Sprossen
Für jede Sprosse können Sie angeben, welcher Sprossenabschnitt nicht eingebaut werden soll. Standardmäßig sind alle waagerechten und senkrechten Sprossen markiert.
- Der Sprossenabschnitt wird nicht eingebaut.
- Der Sprossenabschnitt wird eingebaut.

### Sprossen – Muster
**Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Sprossen > Register Muster**

[Image: Screenshot of the 'Sprossen - Muster' (Mullion Pattern) tab. It shows a complex, custom mullion pattern with an arch.]

In diesem Register erfassen Sie eine individuelle Sprossenkonstruktion.
Die Felder sind in den Registern **Standard** und **Preise** beschrieben.

**Schaltfläche [F12]**: Mit dieser Schaltfläche öffnen Sie die Anwendung **A+W CAD Designer**, um die Sprossenkonstruktion zu gestalten. In dem Bearbeitungsdialog steht Ihnen eine eigene Online-Hilfe zur Verfügung.

## Positionen – Leistung
**Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Leistung**

[Image: Screenshot of the 'Leistung' (Service) tab. It shows a list of order positions and a section to add services like a packaging surcharge.]

In diesem Register erfassen Sie Leistungen, die zu den Positionen hinzugefügt werden sollen. Die Leistungen werden in die Positionen zurückgeschrieben und in der Stückliste aufgeführt, wenn die Angaben gespeichert werden.
⇨ Tutorial, "Zuschlag für besondere Leistung erfassen" auf Seite C-1386

### Positionsbezug
In dieser Übersicht sind alle Auftragspositionen mit Stückzahl und Preisen aufgeführt. Eine Leistung wird nur für die Positionen berechnet, deren Checkbox markiert ist.
**[Alle]**, **[Keine]**: Über die Schaltflächen können Sie alle Checkboxen markieren oder die Markierung(en) entfernen.

### Leistungen
In der Übersicht werden alle erfassten Leistungen aufgeführt. Um sich anzeigen zu lassen, für welche Positionen die Leistung berechnet wird, markieren Sie die Leistung. Die Checkboxen der entsprechenden Positionen sind im Bereich **Positionsbezug** markiert.

Folgende Angaben werden angezeigt und können bearbeitet werden:
- **Produkt, Auswahl, Bezeichnung**: Auswahl, Nummer und Bezeichnung der ausgewählten Leistung.
- **Leist.-einheit**: Bezugsgröße, nach der die Leistung berechnet wird. (Leistungseinheit = LE)
- **Leistungsgröße**: Faktor für die Preisberechnung. Wenn Sie z. B. zu 3 Auftragspositionen mit je 12 Scheiben die Leistung **Entsorgung pro Stück** berechnen möchten, wird die Anzahl der Scheiben aus diesen 3 Positionen (36) angezeigt. Der Preis/LE wird mit dem Wert der Leistungsgröße multipliziert. Wenn die Leistung nach qm berechnet wird, gibt die Leistungsgröße die gesamte Fläche der entsprechenden Auftragspositionen wieder.
- **Darstellung**: Die Leistung kann **implizit**, **explizit** und **implizit im Preis pro ME** dargestellt werden.
  ⇨ Tutorial, "Darstellung der Preise im Druck" auf Seite C-1460
- **Druck**: Angabe, ob die Leistung mit ausgedruckt werden soll.
- **Jahrgang, Schlüssel**: Preisjahrgang und -schlüssel aus den Stammdaten. Sie können geändert werden.
- **Preis / LE**: Preis pro Leistungseinheit aus den Stammdaten. Er kann geändert werden.
- **Rabatt**: Rabatt aus den Stammdaten. Er kann geändert werden.
- **Stk. Netto**: Der Netto-Betrag pro Stück wird aus dem Preis/LE und dem Rabatt errechnet.
- **Pos. Netto**: Der Netto-Betrag für die gesamte Position ergibt sich aus dem Preis/LE, dem Rabatt und der Leistungsgröße.
- **Min. Menge**: Mindestbetrag, der berechnet werden soll.

## Positionen – Zusatz
**Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Zusatz**

[Image: Screenshot of the 'Zusatz' (Additional) tab. It includes sections for mixed calculation, claims, tax, and other miscellaneous data.]

In diesem Register erfassen und bearbeiten Sie Daten zur Mischkalkulation und zur Reklamation. Die Felder zeigen jeweils die Werte der markierten Position an. Alle Angaben gelten für das Hauptprodukt.
Die Felder werden so aktiviert und/oder aktualisiert, wie Sie es über die Menüs festgelegt haben.
⇨ "Menüs in der Positionserfassung" auf Seite C-1711

### Mischkalkulation
Diese Form der Kalkulation wird nur in Österreich eingesetzt.
Die Mischkalkulation wird angewendet, wenn der Preis aus zwei bzw. drei ISO-Preistabellen errechnet werden soll.

> **Stammdaten: Mischkalkulation**
> Die in diesem Dialog angelegte Mischkalkulation steht nicht in Verbindung mit der Mischkalkulation in den Stammdaten der Produkte.
> Wenn Sie Ihre ISO-Einheiten über eine Mischkalkulation berechnen, müssen Sie die Felder in der Positionserfassung Register **Zusatz** ausfüllen.

- **ISO 1, 2, 3**: Auswahl der Gläser in der erfassten ISO-Einheit. Die Gläser werden nicht automatisch angezeigt, wenn Sie eine ISO-Position markieren. Zur Berechnung des Gesamtpreises werden die zugehörigen Preise mit dem zugehörigen Faktor multipliziert.
- **Faktor**: Der Faktor bestimmt, wie der Preis des gewählten Glases bei der Mischkalkulation gewichtet wird. Die Faktoren werden aus den Firmendaten übernommen. Sie können im Auftrag geändert werden.
  ⇨ Stammdaten, "Mischkalkulationsfaktoren" auf Seite B-1068

### Lieferant / Steuer / Zuschläge
- **Lieferant**: Wenn das Produkt bestellt werden muss, können Sie einen Lieferanten eintragen.
  ⇨ Stammdaten, "Lieferantenkartei" auf Seite B-987
- **KOMO-Nr.**: Zertifikatsnummer für niederländische Bauprodukte. Der eingetragene Wert wird an die Produktion und den Druck von Etiketten und Rahmentexten übergeben.
- **Steuer**: Auswahl der gültigen Steuern. Die Einstellung gilt jeweils für die Position, die im Bereich **Positionen** markiert ist.
- **Zuschläge**: Auswahl der gültigen Zuschläge. Die Einstellung gilt jeweils für die Position, die im Bereich **Positionen** markiert ist.

### Produktkennzeichnung
- **CE Kennzeichen**: CE-Kennzeichen aus den Stammdaten des Produktes.

### CPIP Daten
- **CPIP-Code**: Characteristic Performance Identification Paper (Kenndaten zu den Eigenschaften und dem Leistungsverhalten). Der CPIP-Code wird aus den Produktdaten herangezogen.
- **CE-Flag**: Die Suche nach dem CPIP-Code und nach Restriktionen wird aus der Produktdefinition übernommen und kann im Auftrag deaktiviert werden.
  - Die Suche nach dem CPIP-Code und nach Restriktionen ist deaktiviert. Sie kann nicht wieder aktiviert werden. Wenn die Funktion wieder aktiviert werden soll, müssen Sie das Produkt in einer neuen Position erfassen und die alte Position löschen.
  - Die Einstellung wird aus der Produktverwaltung übernommen. Wenn zu dem erfassten Produkt keine CPIP-Prüfung hinterlegt ist, kann die Funktion nicht ausgeführt werden.

### Reklamation
Diese Felder sind nur freigeschaltet, wenn Sie eine Reklamation erfasst haben oder bearbeiten.
Pro reklamierter Position können ein Verursacher, ein Grund und der VK-Preis angegeben werden. Diese Angaben können über die Reklamationsstatistik ausgewertet werden.

> **Dialog Reklamationen öffnen**
> Um die Felder zu füllten, öffnen Sie den Dialog Reklamationen über die Schaltfläche [Ordner].
> ⇨ Tutorial, "Reklamationen" auf Seite C-1544
> ⇨ "Reklamationen" auf Seite C-1875

- **Verursacher**: Der Verursacher kann in der Statistik zur Auswertung herangezogen werden. Die Eingabe ist optional.
- **VK**: Verkaufspreis für die beanstandete Position. In Kulanzfällen kann dieser Wert unter dem tatsächlichen Preis liegen.
- **Grund**: Der Grund kann in der Reklamationsstatistik zur Auswertung herangezogen werden. Die Eingabe ist optional.

### Warengruppen
**Rabatt, Statistik**: Warengruppen aus den Stammdaten der Produkte und aus Kombi-WGR. Die Einstellung gilt jeweils für die markierte Position.
⇨ Stammdaten, "Regeln für Kombi-WGR" auf Seite B-206

### Rahmen
- **Text**: Das Feld ist nur bei Produkten der Produktgruppe **Isolierglas** freigeschaltet. Sie können einen abweichenden Rahmentext angeben, der an die Produktion übergeben werden soll. Wenn Sie mit CEKAL arbeiten, werden die CEKAL-Angaben aus der Produktdefinition übernommen.
- **Rückschnitt**: Der Rückschnitt, der beim Zuschneiden des Glases berücksichtigt werden muss, wird in mm angezeigt. Er kann überschrieben werden. Die Werte werden in die entsprechenden Felder im Rückschnitt im Register **Sprossen** übernommen.
  ⇨ "Positionen - Sprossen" auf Seite C-1770

### Sonstiges
**Alternative zur Pos.**: Dieses Feld ist für Angebote vorgesehen. Damit legen Sie fest, zu welcher Position die markierte Position als Alternative angeboten wird.
⇨ Tutorial, "Alternative Position im Angebot erfassen" auf Seite C-1593

### Manuelle Vorgaben
- **Stückgewicht**: Gewicht pro Stück der aktuellen Position. Der Eintrag kann überschrieben werden. Diese Angabe wird zur Berechnung des Energiezuschlags herangezogen.
  ⇨ Stammdaten, "Energiezuschlag nicht nach Positionsgewicht berechnen" auf Seite B-1090
- **Teilgelief. Menge**: Im Original-Auftrag ist die Stückzahl angegeben, die als Teillieferung der aktuellen Position bereits geliefert wurde. In allen anderen Dokumenten bleibt das Feld leer.
- **Min. Menge**: Angabe der Mindestmenge, sofern diese von den kundenspezifischen oder den firmenübergreifenden Einstellungen abweichen soll. Die Angabe gilt für die aktuelle Position.
- **Maßrundung**: Angabe der Maßrundung, sofern diese von den kundenspezifischen oder den firmenübergreifenden Einstellungen abweichen soll. Die Angabe gilt für die aktuelle Position.
  ⇨ Stammdaten, "Kaufmännische Maßrundung der Abmessung" auf Seite B-1088
  ⇨ Stammdaten, "Standardrundung" auf Seite B-893

### Positionen
Die Felder sind zum Register **Position** beschrieben.
⇨ "Positionen" auf Seite C-1730

- **Skontofähig**: Die Einstellung wird aus der Produktdefinition übernommen. Sie kann überschrieben werden. Die Einstellung gilt für die markierte Position.
  - Die markierte Position wird nicht zur Skontoberechnung herangezogen.
  - Die markierte Position wird zur Skontoberechnung herangezogen.
- **Verp.-Einheit**: Die Verpackungseinheit wird an die Bestellung und die Produktion übergeben und kann ausgedruckt werden.

## Positionen – Weitere Angaben
**Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Weitere Angaben**

[Image: Screenshot of the 'Weitere Angaben' tab. It covers a wide range of fields including texts, production, shipping, costs, and references.]

In diesem Register können Sie weitere Angaben zu Rahmentexten, zur Lagerverwaltung, zum Versand und zur Berechnung von Kosten und Provisionen eingeben. Die Angaben gelten jeweils für die markierte Position.

### Texte
Die Felder in diesem Bereich beziehen sich auf die CEKAL-Angaben, wenn die CEKAL-Funktion freigeschaltet ist (nur in Frankreich).
- **Pos. Gruppe**: Nummer der markierten Position. Wenn mehrere Positionen zu einer Gruppe zusammengefasst wurden, ist dies die Nummer der Gruppe.
- **Serienpos.**: Die aktuelle Position kann zu einer Serie gehören.
  - Die aktuelle Position gehört nicht zu einer Serie.
  - Die aktuelle Position gehört zu einer Serie.
- **Positionstext 1-5**: Die Texte der aktuellen Position werden aus den Stammdaten übernommen. Sie können für diesen Auftrag geändert und ergänzt werden. Die Texte werden an die Produktion übergeben. Im Feld **Positionstext 5** wird der Wert für die Zuschlagsbasis angezeigt.
  ⇨ "Zuschlagsbasis" auf Seite C-1788
- **CEKAL Etikett**: Text, der auf das CEKAL-Etikett gedruckt wird. Er wird aus den Stammdaten übernommen und kann geändert werden.
  ⇨ Stammdaten, "Produkttexte" auf Seite B-1231
- **CEKAL Allgemein**: Allgemeiner Text bei CEKAL-Aufträgen. Er wird aus den Stammdaten übernommen und kann geändert werden.
- **CEKAL Produktion**: Text, der bei CEKAL-Aufträgen an die Produktion übergeben wird. Er wird aus den Stammdaten übernommen und kann geändert werden.

### Produktion
- **Produktionslinie**: Angabe, in welcher Produktionslinie die Position gefertigt werden soll. Die Angabe kann an die Produktion übergeben werden.
- **Etikettenlogo**: Nummer des Logos aus den Stammdaten des Kunden. Die Einstellung kann für diesen Auftrag überschrieben werden.
  ⇨ Stammdaten, "Produktionsetiketten" auf Seite B-916
- **Autom. Zuschnitt**: Angabe aus den Stammdaten des Produktes. Diese Information wird an A+W Production weitergegeben. Die Einstellung kann für diesen Auftrag überschrieben werden.
  - Das Glas wird nicht automatisch zugeschnitten. Es muss von Hand geschnitten werden.
  - Das Glas wird automatisch zugeschnitten.
  ⇨ Stammdaten, "Produktkennzeichen" auf Seite B-725
- **Randentschichtung**: Die Randentschichtung wird als Bearbeitung eingefügt.
  - An den Gläsern wird keine Randentschichtung ausgeführt.
  - Die Gläser werden randentschichtet.
  ⇨ "Randentschichtungen" auf Seite C-1756

### Abweichende Mengen
**Über-/Untermenge**: Zulässige Über- und Untermengen aus den Produktstammdaten. Die Werte können pro Auftrag überschrieben werden. Übermengen aus A+W Production können akzeptiert werden, wenn dateilose Rückmeldungen empfangen werden.
⇨ Stammdaten, “Produktverwaltung - Fertigung" auf Seite B-711
⇨ Fertigung, "Übermengen” auf Seite E-2373

### Gestell
**Typ / Anzahl**: Gestelltyp und Anzahl der Gestelle, auf die die Position gepackt werden soll.
⇨ Stammdaten, "Produktverwaltung - Fertigung" auf Seite B-711

### Zuschlag
**Zuschlagsbasis**: Wenn im aktuellen Auftrag ein automatischer Zuschlag berechnet wird, wird in diesem Feld der Wert angezeigt, der als Basis für die Berechnung herangezogen wird, z. B. das Gewicht.
⇨ "Automatische Zuschläge" auf Seite B-394

### Kosten
Die Kostenart und die Kostenstellen sind in den Stammdaten der Produkte hinterlegt. Die Daten können über externe Berichte ausgewertet werden.
⇨ Stammdaten, "Kostenrechnung" auf Seite B-718
- **Kostenstelle**: Kostenstelle, auf die das Produkt gebucht wird.
  ⇨ Stammdaten, "Kostenstellen" auf Seite B-1051
- **Kostenart**: Kostenart, auf die das Produkt gebucht wird.
  ⇨ Stammdaten, "Kostenart" auf Seite B-1050

### Auslieferung
Die Angaben in diesem Bereich können auf den Lieferschein gedruckt werden. Die Auswahl in den Feldern wird im Modul **Fertigung** hinterlegt.
⇨ "Kommissionierung" auf Seite E-2528
- **Abladestelle**: Standard-Abladestelle beim Kunden. Sie kann für den aktuellen Auftrag geändert werden.
- **Packregel**: Standard-Packregel für den Kunden. Sie kann für den aktuellen Auftrag geändert werden.
- **Gruppenbildung**: Standard-Packmittelgruppe des Kunden. Sie kann für den aktuellen Auftrag geändert werden.

### Skizzendruck
Standardmäßig werden die Angaben zum Skizzendruck aus den Stammdaten der Produkte übernommen.
⇨ Tutorial, "Druck von Skizzen" auf Seite C-1456
> **Skizzendruck festlegen**
> Sie können den Skizzendruck in verschiedenen Dialogen pro Position festlegen. Wenn Sie die Einstellung ändern, werden die Angaben in allen entsprechenden Feldern aktualisiert.
> Sie können die Druckausgabe über den S+N-Editor anpassen, wenn z. B. die Maßangaben nicht deutlich zu erkennen sind.

- **Modell / Sprosse**: Einstellung, wie die Skizze auf den Formularen gedruckt werden soll:
  - **Kein Druck**: Skizzen werden auf den Formularen nicht gedruckt.
  - **Maßstäblich**: Bei dieser Einstellung werden maßstabsgetreue Skizzen gedruckt.
  - **Schematisch**: Bei dieser Einstellung werden die Standardskizzen gedruckt. Sie geben lediglich das Schema des Modells oder Sprossenaufbaus wieder und enthalten keine Maße.
Diese Einstellungen werden abhängig von den Einstellungen im Formulardruck ausgewertet.
⇨ Stammdaten, "Formularverwaltung - Skizzendruck" auf Seite B-1210

### Dokumentenreferenzen
**Bestellreferenz, Auslieferungsauftrag, Endkundennr. / -Pos**: Sie können zu jeder Position eine Referenz auf die Bestellung, den Auftrag und den Kunden eingeben. Diese Referenz kann alphanumerisch angegeben und durch die Positionsnummer aus dem Referenzdokument ergänzt werden.

### Provision
Die Angaben für die Provision werden aus den Stammdaten der Produkte übernommen. In den Firmendaten kann eingestellt werden, wie die Berechnung der Provision durchgeführt werden soll.
⇨ Stammdaten, "Interaktive Vertreterprovisionierung" auf Seite B-1076
- **Satz 1 / 2**: Der hinterlegte Provisionssatz wird nur angezeigt, wenn in den Firmendaten die interaktive Vertreterprovisionierung aktiviert ist. Pro Position können zwei verschiedene Provisionssätze angegeben werden. Diese werden jeweils dem Vertreter 1 bzw. Vertreter 2 zugeordnet.
  ⇨ Stammdaten, "Vertreterprovision" auf Seite B-447

### Positionen
Die Felder sind zum Register **Position** beschrieben.
⇨ "Positionen" auf Seite C-1730

## Positionen - Texte
**Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Texte**

[Image: Screenshot of the 'Texte' tab for a position. It allows adding and editing text blocks associated with a specific order item.]

In diesem Register können Sie zu jeder Auftragsposition einen Text erfassen. Die Angaben gelten jeweils für die markierte Position. Mit den Schaltflächen zur Navigation können Sie durch die Positionen blättern.
⇨ Tutorial, "Text erfassen" auf Seite C-1308

### Blockübersicht
Sie können einen Text hinzufügen, indem Sie entweder einen der hinterlegten Standardtexte auswählen oder einen neuen Text eingeben.
Die Felder werden über die Schaltfläche freigeschaltet.
Ein eingefügter Text wird vollständig über die Schaltfläche entfernt.
- **Nummer**: Textnummer des Standardtextes. Wenn Sie einen eigenen Text hinzufügen, tragen Sie die Nummer 0 (null) ein.
  ⇨ Stammdaten, "Texte" auf Seite B-1189
- **Textkennz.**: Das Textkennzeichen gibt an, für welchen Dokumententyp der Text gültig ist. Zum Beispiel wird der Text mit dem Textkennzeichen **P** nur auf den Produktionspapieren gedruckt. In der Formularverwaltung können Sie Texte zum Druck auf bestimmten Formularen ausschließen.
  ⇨ Stammdaten, "Textarten" auf Seite B-535
  ⇨ Stammdaten, "Formularverwaltung - Texte" auf Seite B-1200
- **Vor, nach Position, produktbezogen**: Über die Wahl der Option bestimmen Sie, an welcher Stelle im Dokument der Text gedruckt werden soll. Die Angaben beziehen sich immer auf die markierte Position. Bei mehreren Texten pro Position beziehen sich die Angaben nur auf den Text, der in der Übersicht der zugewiesenen Texte markiert ist. Folgenden Angaben werden gedruckt:
  - **Vor Position**: Vor der Produktbezeichnung.
  - **Produktbezogen**: Vor der Positionszeile mit Maßen.
  - **Nach Position**: Nach der Positionszeile mit Maßen.
  Die Standard-Option kann im Menü **Optionen > Textpositionierung** eingestellt werden.
  ⇨ "Menü Optionen" auf Seite C-1717
- **(Übersicht)**: In der Tabelle werden alle Texte aufgelistet, die in diesem Dokument gedruckt werden sollen. Die Checkbox **Nachher** zeigt an, welche Option zum Einfügen des Textes gewählt wurde.

### Textblock
- **Text beibehalten**: Diese Checkbox ist nur freigeschaltet, wenn Sie einen Text hinzufügen.
  - Der Text wird nur zu der aktuellen Position hinzugefügt.
  - Der Text wird zu allen Positionen hinzugefügt, die nach der aktuellen Position erfasst werden. Er kann von jeder einzelnen Position wieder entfernt werden.
- **Manuell geändert**: Diese Checkbox zeigt an, welche Texte manuell hinzugefügt oder geändert wurden. Diese Texte können im Formulardruck nicht übersetzt werden. Bei Standardtexten ist die Checkbox nicht markiert.
  - Der Standardtext ist unverändert übernommen.
  - Der Text wurde manuell erstellt oder ein Standardtext wurde geändert.
- **Schaltflächen**: Sie können die Schriftart und -größe ändern und Hyperlinks, Bilder und Tabellen einfügen.
  ⇨ Tutorial, "Text erfassen" auf Seite C-1308
- **Textfeld**: Das Textfeld wird freigeschaltet, wenn Sie auf die Schaltfläche zum Hinzufügen eines Textes klicken. Schreiben Sie direkt in das Textfeld, wenn Sie einen Text eingeben oder ändern möchten.

### Position
Die Felder sind zum Register **Position** beschrieben.
⇨ "Positionen" auf Seite C-1730

## Positionen – Anlagen
**Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Anlagen**

[Image: Screenshot of the 'Anlagen' (Attachments) tab for a position. It shows a file attached to a specific order item.]

In diesem Register können Sie Dateien als Anhang hinterlegen und prüfen, welche Anhänge mit dem Dokument gespeichert sind. Dateianhänge können Sie mit einem Doppelklick öffnen.
Der Anhang gilt jeweils für die markierte Position.
⇨ Tutorial, "Dokumente anhängen" auf Seite C-1311

### Dateianhang
Der Dateiname und der Pfad werden angezeigt. Sie können zu jedem Anhang eine Bemerkung hinzufügen, die den Anhang kurz beschreibt.
In den Firmendaten ist festgelegt, wo die Anhänge gespeichert werden.
⇨ Stammdaten, "Dateianhänge" auf Seite B-1071
Über das Kontext-Menü **Verknüpfung hinzufügen** können Sie eine Datei als Anlage hinzufügen.

### Positionen
Die Felder sind zum Register **Position** beschrieben.
⇨ "Positionen" auf Seite C-1730

## Positionen – Technische Werte
**Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Technische Werte**

[Image: Screenshot of the 'Technische Werte' tab. It lists various technical characteristics of the product, such as U-value, light transmission, and fire resistance, with their corresponding values.]

In diesem Register können Sie die technischen Werte eines Produkts festlegen. Wenn die A+W SLT-Schnittstelle konfiguriert ist, werden die Werte über die A+W SLT-Schnittstelle ermittelt.

### Technische Werte
[Image: Icons for adding and deleting entries.]
Über die Schaltflächen können Sie einen Eintrag hinzufügen oder löschen.

> **Leistungserklärung**
> Pro Kunde und Produkt kann in den Stammdaten festgelegt werden, ob eine Leistungserklärung angegeben werden muss.

- **Leistungserklärung**: Nummer der Leistungserklärung, die dem Auftrag zugeordnet werden soll. Die Nummer kann eingegeben oder über die Schaltfläche [Lupe] oder [Ordner] ausgewählt werden. Die Nummer wird automatisch erzeugt, wenn die A+W SLT-Schnittstelle konfiguriert ist und der Produktaufbau zum ersten Mal generiert wird.
- **[Taschenrechner]**: Die Schaltfläche ist nur kunden- und/oder produktspezifisch freigeschaltet. Über die Schaltfläche können Sie die Technischen Werte für die Leistungserklärung berechnen lassen.

### Positionen
Die Felder sind zum Register **Position** beschrieben.
⇨ "Positionen" auf Seite C-1730

## Positionen – Klassifikatoren
**Dokumente > Auftrag > Auftrag auswählen > Positionen > Register Klassifikatoren**

[Image: Screenshot of the 'Klassifikatoren' (Classifiers) tab. It shows a list of classifiers like 'Brandschutz' and 'Herkunft' that can be assigned to the product.]

In diesem Register können Sie die Klassifikatoren des erfassten Produkts prüfen und bearbeiten. Die Klassifikatoren werden auch angezeigt, wenn das Produkt eine Stücklistenkomponente ist.
Im Formulardruck und in der Dokumentenansicht können die Klassifikatoren an den Report übergeben werden.

### Positionen
Die Felder sind zum Register **Position** beschrieben.
⇨ "Positionen" auf Seite C-1730

# Dokument – Summen
**Dokumente > Auftrag > Auftrag auswählen > Register Summen**

[Image: Screenshot of the 'Summen' (Totals) tab. It provides a comprehensive financial overview including technical sums, credit limit status, cost/contribution margin breakdown, and tax calculation.]

In diesem Register prüfen Sie die Kosten und das Kreditlimit. Zur Information werden Summen zum Auftrag und zu technischen Größen angezeigt. Außerdem können Sie einen Festpreis für den Auftrag insgesamt angeben.

## Summen (technische Parameter)
In diesem Bereich werden die Summen zu Flächen, Umfang und Gewicht angezeigt. Die Felder sind leer, wenn Sie den Auftrag anlegen und noch keine Positionen erfasst sind. Die Felder geben die tatsächlichen Werte und die gerundeten Werte an.

- **Stückzahl (gesamt / ISO-Einheiten)**: Anzeige der gesamten Stückzahl und der Stückzahl der ISO-Einheiten.
- **Summe Fläche (real / fakt.)**: Anzeige der gesamten Fläche, die aus den Angaben zur Breite und Höhe errechnet ist. (fakt. = fakturiert)
  - Der erste Wert zeigt die tatsächliche Summe der Fläche an.
  - Der zweite Wert zeigt die Summe an, bei der die Einstellungen zur Berechnung berücksichtigt wurden. Wenn für die Preisberechnung das umschreibende Rechteck und/oder Mindestmengen zugrunde gelegt werden, sind unterschiedliche Werte möglich.
- **Summe Umfang (real / fakt.)**: Anzeige der gesamten Kantenlänge, die aus den Angaben zur Breite und Höhe errechnet ist.
  - Der erste Wert zeigt die tatsächliche Summe der Kanten an.
  - Der zweite Wert zeigt die Summe an, bei der die Einstellungen zur Berechnung berücksichtigt wurden. Wenn für die Preisberechnung das umschreibende Rechteck und/oder Mindestmengen zugrunde gelegt werden, sind unterschiedliche Werte möglich.
- **Summe Gewicht (real / Tara)**: Anzeige des Gesamtgewichts des Auftrags und des Gewichts der Verpackung. Das Feld **Tara** bleibt leer, wenn keine Angaben zur Verpackung erfasst sind.
- **Summe Sprossenlänge (real / fakt.)**: Anzeige der gesamten Länge aller Sprossen, die in diesem Auftrag erfasst wurden.
  - Der erste Wert zeigt die tatsächliche Summe der Sprossenlängen an.
  - Der zweite Wert zeigt die Summe an, bei der die Einstellungen zur Berechnung berücksichtigt wurden. Wenn für die Preisberechnung Mindestmengen zugrunde gelegt werden, sind unterschiedliche Werte möglich.

**Ergänzende Informationen**
⇨ Stammdaten, "Maßrundung Breite / Höhe" auf Seite B-721
⇨ Stammdaten, “Kaufmännische Maßrundung der Abmessung" auf Seite B-1088
⇨ Stammdaten, "Firmendaten - Preisberechnung" auf Seite B-1085
⇨ "Maßrundung" auf Seite C-1701

## Kosten/Deckungsbeitrag
Diese Anzeigen der Kosten und Deckungsbeiträge sind insbesondere dann von Interesse, wenn die vorgegebenen Preise manuell geändert werden. Bei dieser Anzeige gilt die Differenz zwischen VK und EK als Deckungsbeitrag.
Wenn Sie mit der Kostenkalkulation arbeiten, wird der Deckungsbeitrag auf der Grundlage der Produktpreise errechnet.
Die Felder sind leer, wenn noch keine Positionen erfasst sind.

- **Materialkosten**: Anzeige der Materialkosten, die in diesem Auftrag enthalten sind.
- **Rohgewinn / %**: Der Rohgewinn wird ermittelt, durch den Verkaufspreis abzüglich der Materialkosten. Die Zahl im ersten Feld zeigt den Rohgewinn in € an, im zweiten Feld den Rohgewinn in Prozent.
- **Fertigungskosten**: Anzeige der Fertigungskosten, die in diesem Auftrag enthalten sind. Diese Kosten werden nur angezeigt, wenn der Auftrag an die Kapazitätsplanung übergeben und eingelastet wurde.
- **Frachtkosten**: Die Frachtkosten werden aus der Entfernung und dem in den Stammdaten der Touren hinterlegten Preis pro Kilometer errechnet. Die Entfernung ist in den Kundenstammdaten hinterlegt oder im Register **Abweichende Anschriften** für den aktuellen Auftrag angepasst. Über die Schaltfläche öffnen Sie die Übersicht zu den kalkulatorischen Frachtkosten.
  ⇨ "Kalkulatorische Frachtkosten" auf Seite C-1858
- **Frachtkosten %**: Der prozentuale Anteil der Frachtkosten bezieht sich auf den Gesamtwert des Auftrags.
- **Prozesskosten**: Die Prozesskosten ergeben sich aus der Summe der Fertigungskosten und Frachtkosten.
- **Deckungsbeitrag**: Diese Schaltfläche öffnet das genaue Kalkulationsschema mit allen darin enthaltenen Kosten. Das Feld **Betrag** zeigt den absoluten Wert und das Feld **Prozent** den prozentualen Wert.
- **Gesamtkosten**: Anzeige der Gesamtkosten (Materialkosten, Fertigungskosten und Frachtkosten) aller Positionen, die im Auftrag enthalten sind.
- **DB % 1**: Der Deckungsbeitrag 1 errechnet sich aus dem Rohgewinn abzüglich der Fertigungs- und Frachtkosten.
  - Der erste Wert zeigt den absoluten Wert des errechneten Deckungsbeitrags für diesen Auftrag an.
  - Der zweite Wert zeigt den prozentualen Wert des errechneten Deckungsbeitrags für diesen Auftrag an.
- **Gemeinkosten**: Anzeige der Gemeinkosten (Verwaltung und Vertrieb).
- **DB % 2**: Der Deckungsbeitrag 2 errechnet sich aus dem Deckungsbeitrag 1 abzüglich der Gemeinkosten.
  - Der erste Wert zeigt den absoluten Wert des errechneten Deckungsbeitrags für diesen Auftrag an.
  - Der zweite Wert zeigt den prozentualen Wert des errechneten Deckungsbeitrags für diesen Auftrag an.
- **Festkosten**: Sie können einen Wert für die Festkosten (EK) des gesamten Auftrags festlegen.

## Kreditlimit
Das Kreditlimit wird auch dann automatisch aktualisiert, wenn aus dem Programm zur Finanzbuchhaltung (FiBu) keine offenen Posten zurückgemeldet werden. Die Aufträge werden bis zur FiBu-Übergabe berücksichtigt.
Das Limit 1 gibt den versicherten Betrag an, das Limit 2 den unversicherten.
Zur Berechnung des Saldos werden die Angaben aus den Kundendaten herangezogen.
Der Saldo ergibt sich aus folgender Berechnung:
`Limit 1/2 - OP (FiBu) - Obligo - Aufträge = Saldo 1/2`
Die Werte in den Feldern für Saldo 1/2 werden in roter Schrift angezeigt, wenn das Kreditlimit überschritten ist.
⇨ Stammdaten, "Partnerverwaltung - Saldo" auf Seite B-909
⇨ Tutorial, "Kreditlimit" auf Seite C-1301

## Wertvolumen
In den beiden Spalten dieses Bereichs werden die Beträge in der Landeswährung und in der Fremdwährung angezeigt. Die Summen werden automatisch aktualisiert, wenn Änderungen gespeichert werden.
**Währung**: Anzeige der Währung, die im Register **Konditionen** festgelegt wurde.
⇨ "Währung" auf Seite C-1703
