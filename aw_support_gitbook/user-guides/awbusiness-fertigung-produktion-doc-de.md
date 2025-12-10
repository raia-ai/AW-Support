---
description: "D-AWBusiness-HB_25"
---


# Softwarereferenz Produktion

---
## Menü Funktionen

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Dialog zu schließen. Folgende Einträge werden angezeigt:

- **Historie:**
  Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des markierten Dokuments.
  ⇨ Verkauf, "Historie" auf Seite C-564
- **Einstellungen:**
  Öffnet den Dialog Einstellungen-Produktionsübergabe, in dem Sie die Einstellungen für die Datenübergabe festlegen.
  ⇨ "Einstellungen Produktionsübergabe" auf Seite E-174

### Identifikation

**Mandant** Wenn Sie mit unterschiedlichen Mandanten arbeiten, werden diese zur Auswahl angeboten.

**Bereich** Wenn in der Produktion mit verschiedenen Bereichen gearbeitet wird, können Sie denjenigen auswählen, an den die Aufträge übergeben werden sollen.
Die Angabe wird für die Auswahl des Nummernkreises herangezogen, aus dem die Laufnummer für die Übergabe gezogen wird.

**Mitarbeiter** Name des Mitarbeiters, der sich in A+W Business angemeldet hat.

**Nummernverwalter** Wenn Sie einen Nummernverwalter ausgewählt haben, werden alle Aufträge übergeben, die in diesem Nummernverwalter stehen und den Mindeststatus erreicht haben.

**Modus** Auswahl des Übertragungsmodus. Folgende Modi stehen zur Wahl:
- **Produktionsübergabe:**
  Die in der Liste angezeigten Aufträge werden an die Produktion übergeben.
- **Produktionsfreigabe:**
  Die in der Liste angezeigten Aufträge werden zur Produktion freigegeben und an die Produktion übergeben.
- **Reservierungsauftrag:**
  Die in der Liste angezeigten Aufträge werden an die Produktion übergeben, um Kapazitäten in der Produktion zu reservieren. Die Aufträge sind nicht zur Produktion freigegeben.
- **Kostenkalkulation:**
  Die in der Liste angezeigten Aufträge werden an die Produktion übergeben, um die Material- und Maschinenkosten zu ermitteln. Die Aufträge belegen keine Zeiten in der Produktion und sind nicht zur Produktion freigegeben.
- **Übergabe nicht produktionsrelevanter Änderungen:**
  Wenn die in der Liste angezeigten Aufträge bereits an die Produktion übergeben sind, können Änderungen an nicht produktionsrelevanten Daten in den Positionen und Aufträgen nachträglich übergeben werden, z. B.:
  - Änderungen an Kundenadresse, Kunde und Lieferadresse, Änderungen der Tour,
  - Änderungen der Dateianhänge mit Kennzeichen für die Produktionsübergabe oder der Positionstexte mit Kennzeichen für die Produktionsübergabe,
  - Änderungen an Kommission und Kundenpositionen.
- **Storno:**
  Die in der Liste angezeigten Aufträge werden mit einem Storno-Kennzeichen erneut übergeben. Der Dokumentenstatus wird auf Übergabe Produktion storniert umgesetzt.
  ⇨ Tutorial, "So stornieren Sie die Produktionsübergabe manuell" auf Seite E-40

### Ausgabe

In diesem Bereich werden die Daten zu dem Auftrag angezeigt, der aktuell übertragen wird. Die Einstellungen zur Übergabedatei legen Sie über das Menü Funktionen fest:
⇨ "Einstellungen Produktionsübergabe" auf Seite E-174

**Ausgabe-Datei** Anzeige von Pfad und Namen der Übergabedatei.

**Release** Version der Übergabedatei.

**Lauf-Nummer** Anzeige der fortlaufenden Nummer der Produktionsübergabe. Die Nummer wird aus dem Nummernkreis für den Bereich gezogen, der in den Stammdaten hinterlegt ist. Die Trennung der Übergabe in verschiedene Bereiche ist dann sinnvoll, wenn Sie mehrere Produktionsstätten eingerichtet haben.
⇨ Stammdaten, "Nummernkreise" auf Seite B-903

**Positionsläufe** Anzahl der Läufe, die für die Positionen gebildet werden.

**Gesamt, Gesamtpositionen** Anzahl der übergebenen Aufträge und Positionen.

**Auftrag** Nummer des Auftrags, der aktuell übertragen wird.

### Aufträge

In der Übersicht werden alle Aufträge aus dem Nummernverwalter aufgelistet.
- **Nummer:**
  Nummer des Auftrags.
- **Nummer Kunde/Lief.:**
  Nummer des Kunden oder Lieferanten.
- **Kunde/Lieferant:**
  Name des Kunden oder Lieferanten.
- **Status:**
  Status des Auftrags
- **Datum Prod. ISO, VSG, ESG:**
  Datum, an dem das ISO, VSG oder ESG voraussichtlich produziert wird.
- **Lauf-Nr. Prod. ISO, VSG, ESG:**
  Nummer des Laufs, in dem das ISO, VSG oder ESG produziert wurde. Die Nummer wird nach der Rückmeldung angezeigt.
- **Datum Lieferung:**
  Lieferdatum aus dem Auftrag
- **Lieferschein:**
  Das Feld bleibt in dieser Anzeige normalerweise leer. Nur wenn Lieferscheine vor der Produktionsübergabe gedruckt werden, wird das Feld gefüllt.
- **Tour:**
  Name der Tour, mit der geliefert wird.
- **Gewicht gesamt:**
  Gewicht aller Auftragspositionen.
- **Stück gesamt:**
  Stückzahl aller Auftragspositionen.
- **Qm gesamt:**
  Fläche aller Auftragspositionen.
- **LFM gesamt:**
  Laufmeter der Kanten.
- **Datum Erfassung:**
  Erfassungsdatum des Auftrags.

### Export

Wenn Sie in der Übersicht auf das erste Feld in der Titelzeile der Tabelle klicken, können Sie weitere Einstellungen für den Export festlegen.

- **CSV-Datei schreiben:**
  Mit der Wahl dieser Funktion können Sie die Daten aus der Übersicht in eine CSV-Datei schreiben. Ein Dialog bietet Ihnen die Auswahl des Speicherortes.
- **Optionen:**
  Mit der Wahl dieser Funktion können Sie festlegen, nach welchen Einträgen eine neue Zeile geschrieben werden soll.
- **XML-Datei schreiben:**
  Mit der Wahl dieser Funktion können Sie die Daten aus der Übersicht in eine XML-Datei schreiben. Ein Dialog bietet Ihnen die Auswahl des Speicherortes.

## Einstellungen Produktionsübergabe

**Navigation:**
Fertigung > Produktion > Übergabe Produktion > Menü Funktionen > Einstellungen
Fertigung > Angebotsoptimierung > Übergabe Produktion > Menü Funktionen > Einstellungen

Im Dialog Einstellungen – Produktionsübergabe können Sie Einstellungen für die Übergabe an die Produktion festlegen. Die Einstellungen werden für Angebote und Aufträge getrennt eingerichtet und gespeichert.

> **Einstellungen pro Arbeitsplatz**
> Die Einstellungen gelten pro Arbeitsplatz, d. h., dass für jeden Mitarbeiter eigene Einstellungen verwendet werden können.

In diesem Dialog finden Sie folgende Register:
- "Einstellungen Produktionsübergabe - Schnittstelle" auf Seite E-175
- "Einstellungen Produktionsübergabe – Übergabe Parameter" auf Seite E-178
- "Einstellungen Produktionsübergabe – Zusätzliche Schnittstellen" auf Seite E-185
- "Einstellungen Produktionsübergabe – Texte/Anlagen" auf Seite E-187

## Einstellungen Produktionsügbergabe – Schnittstelle

**Navigation:** Fertigung > Produktion > Übergabe Produktion > Menü Funktionen > Einstellungen > Register Schnittstelle

[Image: Abb. E-86 Einstellungen-Produktionsübergabe - Schnittstelle]

In diesem Register legen Sie die Details zur Schnittstelle fest, über die Aufträge an die Produktion gesendet werden.

### Schnittstelle Produktion

In diesem Bereich legen Sie die Einstellungen für die Datei zur Produktionsübergabe fest. Wenn Sie das Format OrderXML verwenden, werden außer den Produktionsdaten auch die Daten für CAD Designer (Bars) in die jeweilige Übergabedatei geschrieben. Pro Auftrag wird eine Übergabedatei erstellt.

**Version** Standardmäßig werden die Daten per OrderXML übertragen.
Wenn Sie Pool.asc-Dateien erzeugen wollen, müssen Sie die Version auswählen, die in Ihrem System installiert ist. In diesem Fall müssen Sie im Register Übergabe Parameter die Checkbox A+W Production deaktivieren.
⇨ "A+W Production" auf Seite E-179

**Ohne ERP-Webservice** Die Produktionsübergabe kann optional dateilos übertragen werden.
☐ Die Übergabedateien werden durch den ERP-Webservice gespeichert.
☑ Die Übergabedaten können dateilos ohne den ERP-Webservice übertragen werden. Bei dieser Einstellung können Dateien nur mit dem Exchange Service übergeben werden.
Die Felder im Bereich Schnittstellt AWDesign und die Felder für den ERP-Webservice werden gesperrt.

**Dateiloser Export** Die Produktionsübergabe kann optional dateilos übertragen werden. Die checkbox ist nur freigeschaltet, wenn die Checkbox ohne ERP Webservice markiert ist.
☐ Die Übergabedateien werden durch den ERP-Webservice gespeichert.
☑ Die Übergabedaten werden dateilos übertragen. Mit dieser Einstellung wird das Feld Pfad/Dateiname gesperrt.

**Pfad/Dateiname** Eingabe von Verzeichnis und den Dateinamen, unter dem die Übergabedatei gespeichert werden soll. Achten Sie bei der Übergabe an A+W Production darauf, dass die Datei in ein Verzeichnis geschrieben wird, das von A+W Production überwacht wird.
Standardmäßig verwenden Sie den Dateinamen OrderXXXX.xml, wobei die Platzhalter (XXXX) durch die Auftragsnummer und einen Zeitstempel ersetzt werden.

### Schnittstelle AWDesign

In diesem Bereich legen Sie die Einstellungen für die Übergabe an CAD Designer (Bars) fest.

**Version** Standardmäßig wird die Übergabe per OrderXML genutzt.

**Pfad/Dateiname** Angabe von Verzeichnis und den Dateinamen für die Übergabedatei an CAD Designer (Bars).

### OrderXML

**Version** Auswahl der Version der OrderXML-Schnittstelle, die auf Ihrem System installiert ist.

**ERP-Webservice-URL** Webadresse, über die der ERP-Webservice angesteuert wird, z. B. http://localhost/albwir.erp.webservice.2011. Diese URL muss eingetragen werden, wenn Sie mit OrderXML arbeiten.
Das Feld ist gesperrt, wenn die Checkbox ohne ERP Webservice markiert ist.

**Speichern der OrderXML-Dateien durch ERP-Webservice** Bei der OrderXML-Übergabe kann die Übergabedatei durch A+W Business oder durch den ERP-Webservice gespeichert werden.
☑ Die Übergabedateien werden von A+W Business gespeichert (Standard).
☐ Die Übergabedateien werden durch den ERP-Webservice gespeichert.

**Unicode-Format schreiben** Die Übergabe-Daten können in zwei verschiedenen Formaten geschrieben werden.
☐ Die Übergabedateien werden im Standard-Format geschrieben.
☑ Die Übergabedateien werden im Unicode-Format geschrieben.

### Modus der Übergabe

Mit der Wahl der Option legen Sie den Modus für die automatische Übergabe fest:

- **Nach Mindest- und Sperrstatus Produktionsübergabe:**
  Für die automatische Produktionsübergabe wird der Auftragsstatus mit dem Mindest- und Sperrstatus für die Produktionsübergabe verglichen. Liegt der Auftragsstatus dazwischen, wird der Auftrag automatisch an die Produktion übergeben. Dies ist die Standardeinstellung.
- **Dokumente im Kapazitätsplanungs-Pool:**
  Mit dieser Einstellung werden die Aufträge zuerst an AWCapacity Planning übergeben.
  Sobald ein Auftrag neu erfasst oder geändert wird, landet er im Pool für die Kapazitätsplanung. Wenn die automatische Produktionsübergabe aktiviert ist, wird ein Auftrag in diesem Pool automatisch übergeben. Nach der Übergabe wird der Auftrag aus diesem Pool entfernt.
  Mit dieser Einstellung ist Übergabe zur Angebotsoptimierung gesperrt.

Sie können diese Einstellung ignorieren, wenn Sie die Übergabe nicht automatisiert haben. In diesem Fall wird im Dialog Produktionsübergabe die Datenübergabe aus dem Nummernverwalter manuell gestartet, wobei Mindest- und Sperrstatus berücksichtigt werden.
⇨ "Übergabe Produktion" auf Seite E-170

## Einstellungen Produktionsübergabe – Übergabe Parameter

**Navigation:** Fertigung > Produktion > Übergabe Produktion > Menü Funktionen > Einstellungen > Register Übergabe Parameter

[Image: Abb. E-87 Einstellungen-Produktionsübergabe – Übergabe Parameter]

In diesem Register legen Sie fest, welche Parameter in die Übergabedatei geschrieben und damit an die Produktion übergeben werden sollen.

**Benutzerabhängige Einstellungen verwenden** Die Einstellungen werden in die Datenbank geschrieben und beim Start von A+W Business geladen. Sie können Einstellungen pro Benutzer festlegen.
Diese Checkbox wird nicht angezeigt, wenn Sie den Dialog über Firmendaten > Register Produktion geöffnet haben.
☐ Die Einstellungen gelten für alle Mitarbeiter, die sich an A+W Business anmelden.
☑ Die Einstellungen gelten jeweils nur für den Mitarbeiter, der sich aktuell an A+W Business angemeldet hat.

**A+W Production** Sie können die Daten im Format OrderXML an A+W Production übergeben. Wenn Sie mit der Pool.asc-Übergabe arbeiten, dürfen Sie diese Einstellung nicht wählen.
☐ Die Daten werden nicht an A+W Production übergeben. Wählen Sie diese Einstellung, wenn die Daten an A+W Standard Optimizer oder ALFERT übergeben werden sollen.
☑ Die Daten werden direkt an A+W Production übergeben. Dazu muss im Register Schnittstelle der Pfad angegeben werden, unter dem die Übergabedateien gespeichert werden.
⇨ "Pfad/Dateiname" auf Seite E-176

**Laufnummer vorgeben** Die Laufnummer (Nummer der Übergabe) kann von A+W Business aus dem Nummernkreis von AWPool gezogen werden.
☐ Die Übergabelaufnummer wird in der Produktion selbst vergeben.
☑ Die Übergabelaufnummer wird von A+W Business aus dem Nummernkreis AWPool gezogen und in die Schnittstellendatei geschrieben.
⇨ Stammdaten, "Nummernkreise - Produktion" auf Seite B-907

**Positions-Splitting lizenziert** Nur Pool.asc-Übergabe. Wenn die Produktion von großen Aufträgen über mehrere Tage verteilt werden muss, können Sie bestimmen, ob die Teilung sich auch auf Positionen beziehen darf. Diese Einstellung betrifft nur die A+W Business-Kapazitätsplanung. Diese Checkbox ist nur freigeschaltet, wenn das Modul lizenziert ist.
☐ Positionen sollen immer so verplant werden, dass sie an einem Tag produziert werden.
☑ Positionen können auf mehrere Tage verteilt produziert werden.

**Automatische Übergabe bei Wareneingang** Wenn Sie in Aufträgen Positionen mit den Kennzeichen Produktion erfasst haben, in denen zusätzlich Komponenten enthalten sind, die bestellt werden müssen, können diese Aufträge erst produziert werden, wenn die Komponenten eingetroffen sind, z. B. ein ISO mit einem Ornamentglas, das nicht auf Lager gehalten wird.
Beim Eingang der bestellten Komponenten kann die Information über den Wareneingang an die Produktion weitergegeben werden.
Voraussetzung ist, dass der PPS-Webservice installiert ist und die URL in den Firmendaten > Register Produktion angegeben wurde.
⇨ Stammdaten, "Firmendaten - Produktion" auf Seite B-1000
☐ Der Wareneingang der Bestellartikel wird nicht automatisch an die Produktion übergeben. Er muss nach der Eingangsbuchung manuell an die Produktion übergeben werden.
☑ Der Wareneingang der Bestellartikel wird automatisch an die Produktion übergeben. Dazu muss diese Funktion auch im Wareneingang aktiviert werden.
⇨ Einkauf, "Menü Optionen" auf Seite D-228

**Bleiverglasung als Sprosse übergeben** Nur Pool.asc-Übergabe. Bleiverglasungen können als Sprossensätze an die Produktion übergeben werden.
☐ Bleiverglasungen werden als Bearbeitungen, nicht als Sprossensätze an die Produktion übergeben.
☑ Bleiverglasungen werden als Sprossensätze an die Produktion übergeben. Diese Information dient der Organisation der entsprechenden Arbeitsabläufe. Diese Einstellung sollten Sie nur in Absprache mit der A+W Software GmbH nutzen.

**Kantenschutz pro Auftrag** Nur Pool.asc-Übergabe. Ein Kantenschutz erfordert die Korrektur der Maße einer Position. Diese Korrektur kann automatisch bei allen Aufträgen durchgeführt werden, um den Kantenschutz anzubringen.
☐ Der Kantenschutz wird nur bei Aufträgen angebracht, in denen er als Bearbeitung eingetragen ist. Die Maßkorrektur ist dabei berücksichtigt.
☑ Der Kantenschutz wird standardmäßig bei allen Aufträgen angebracht.

**Artikel übergeben** Diese Einstellung betrifft alle Produkte der Produktart Artikel. Diese werden i. d. R. als Lagerartikel geführt, z. B. Handgriffe.
☐ Artikel werden standardmäßig nicht an die Produktion übergeben.
☑ Artikel werden mit an die Produktion übergeben.
Siehe dazu auch die Einstellungen in den Produktstammdaten (Register A+W Production) und in den Firmendaten (Register Produktion).

**Folien (VSG) übergeben** Nur Pool.asc-Übergabe. Wenn Sie VSG-Scheiben herstellen, können Sie festlegen, dass die Folien mit an die Produktion übergeben werden.
☐ Die Folien werden nicht an die Produktion übergeben.
☑ Die Folien werden an die Produktion übergeben.

**GH-Füllungen übergeben** Nur Pool.asc-Übergabe. Wenn Sie Gießharzfüllungen produzieren, können Sie festlegen, ob diese an die Produktion übergeben werden.
☐ Die Gießharzfüllung wird nicht an die Produktion übergeben.
☑ Die Gießharzfüllung wird an die Produktion übergeben.

**A+W Production-Sondertext übergeben** Nur Pool.asc-Übergabe. Diese Einstellung betrifft nur die Pool.asc-Übergabedateien. In diesen Dateien sind die Felder limitiert. Um bestimmte Texte, die für A+W Production wichtig sind, dennoch übergeben zu können, können Textnummern für entsprechende Zusatzinformationen festgelegt werden. Diese können übergeben werden. Die Textnummern werden durch die A+W Business- und A+W Production-Projektierung festgelegt.
☐ Sondertexte werden nicht übergeben.
☑ Die Textnummer für den Sondertext wird übergeben.

| Textnummer | Text |
| :--- | :--- |
| 3100 plus x | Stücklistenbezeichnung Abstandhalter |
| 3150 plus x | Kurzbezeichnung aus den Basisdaten zum Abstandhalter |
| 3200 plus x | Stücklistenbezeichnung UV-Randverbund, Schmaler Randverbund |
| 3250 plus x | Kurzbezeichnung aus den Basisdaten zum UV-Randverbund, Schmaler Randverbund |
| 3300 plus x | Stücklistenfarbe zum Abstandhalter |
| 3400 plus x | Stücklistenbezeichnung Gas |
| 3450 plus x | Kurzbezeichnung aus den Basisdaten zum Gas |
| dabei ist x ein fortlaufender Zähler, also 0, 1, 2, 3 | |
| 3600 | Positionsrückschnitt |
| 3700 | Teilegewicht in Gramm zur Satzart 8 |
| 4100 | CE-Kennzeichen |

**Touren-Rangfolge übergeben** Nur Pool.asc-Übergabe. Die Tour-Rangfolge wird aus den Stammdaten der Kunden ausgelesen. Sie kann für die Beladung der Lkws wichtig sein.
☐ Die Tour-Rangfolge wird nicht übergeben.
☑ Die Tour-Rangfolge wird übergeben.

**Direktanlieferung nicht übergeben** Bestellartikel können vom Lieferanten direkt an den Kunden gesendet werden. Das Kennzeichen wird im Auftragskopf im Register Abweichende Anschriften gesetzt.
☐ Alle Auftragspositionen werden an die Produktion übergeben. Das Kennzeichen zur Direktanlieferung wird nicht berücksichtigt.
☑ Bestellpositionen mit dem Kennzeichen zur Direktanlieferung werden nicht an die Produktion übergeben. Die Positionen werden direkt vom Lieferanten an den Kunden geliefert.

**OrderXML: Kurzbez. statt Matchcode übergeben** Bei der OrderXML-Übergabe wird für Produkte standardmäßig der Matchcode übergeben.
☐ Der Matchcode wird als Produktbezeichnung übergeben.
☑ Statt des Matchcodes wird die Kurzbezeichnung übergeben. Wenn Sie von der Pool-Übergabe auf OrderXML umgestellt haben, können Sie diese Einstellung wählen, um weiterhin die Kurzbezeichnung zu übertragen.

**Beschaffungsart Produktion aus Dokument vorr.** Nur Pool.asc-Übergabe. In der Regel sind die Beschaffungsarten für A+W Business und A+W Production identisch. Bei Abweichungen können Sie festlegen, welche Angabe vorrangig ausgewertet werden soll.
Die Einstellung ist z. B. wichtig für VSG, das sowohl produziert als auch zugeschnitten wird. In den Stammdaten ist das Produkt z. B. als Zuschnitt definiert. Das VSG soll jedoch in einem bestimmten Auftrag produziert werden. Dafür können Sie einstellen, welche Beschaffungsart vorrangig ausgewertet wird.
☐ Die Beschaffungsart aus A+W Production wird vorrangig ausgewertet. In diesem Fall würde der oben genannte Auftrag immer als Zuschnitt ausgewertet.
☑ Die Beschaffungsart aus dem Auftrag wird vorrangig ausgewertet. In diesem Fall würde das VSG im obigen Fall als Produktion ausgewertet, wenn im Auftrag die Beschaffungsart Produktion eingestellt wurde.

**Provinz in der Anschrift übergeben** Nur Pool.asc-Übergabe. Diese Einstellung betrifft nur Staaten, in denen die Provinz wichtig ist.
☐ Die Provinz wird nicht an die Produktion übergeben.
☑ Die Provinz wird an die Produktion übergeben und an den Namen des Ortes angehängt.

**Mengenfelder im Positionssatz tauschen** Nur Pool.asc-Übergabe. Wenn Sie mit der Kapazitätsplanung von A+W Business arbeiten, können deren Mengenfelder übernommen werden.
☐ Die Mengenfelder werden nicht aus der Kapazitätsplanung übernommen.
☑ Die Mengenfelder sollen aus der Kapazitätsplanung übernommen werden. Dabei werden die Felder für die Menge (Feld 11) und für die Positionsmenge (Feld 85) getauscht. Feld 11 enthält jetzt die von der Kapazitätsplanung gebildete Teilmenge und Feld 85 die Originalmenge.

**Noppen-KZ in Sondertext 1 im Positionssatz** Nur Pool.asc-Übergabe. Das Kennzeichen für Noppen kann an die Produktion übergeben werden. Diese Einstellung betrifft nur die Pool.asc-Schnittstelle in der Version 2.3.
☐ Das Kennzeichen für Noppen wird nicht übergeben.
☑ Das Noppen-KZ der ersten Sprosse wird als Sondertext 1 (im Feld 133) des Positionssatzes übergeben.

**Order-Tags erzeugen** Zurzeit nur kundenspezifisch genutzt.

**VSG-Auflösung (Rel. 2.1)** In Pool.asc 2.1 können für VSG (als Position oder als Komponente in der Stückliste) zusätzliche Sätze erzeugt werden. Diese Checkbox ist gesperrt, wenn Sie ein anderes Format gewählt haben.
☐ Bei der VSG-Auflösung werden keine zusätzlichen Sätze erzeugt.
☑ Für die VSG-Produktion werden Pseudopositionen erzeugt. Diese Einstellung sollten Sie nur in Absprache mit der A+W Software GmbH nutzen.

**VSG (2.1) Maßzugabe aus Stückliste** In Pool.asc 2.1 können für VSG, die Glaskomponenten mit Bearbeitungen enthalten, die Maßzugaben aus den Stücklisten übergeben werden. Diese Checkbox ist gesperrt, wenn Sie ein anderes Format gewählt haben.
☐ Maßzugaben der Stücklisten-Komponenten werden nicht berücksichtigt.
☑ Maßzugaben der Stücklisten-Komponenten werden übergeben.

**Inchwerte immer in 1/256 inch** Nur Pool.asc-Übergabe. In den Firmendaten im Register System ist festgelegt, wie die Maß-Präzision gerechnet wird. Diese Einstellung kann übersteuert werden.
⇨ Stammdaten, "Maßsystem" auf Seite B-987
☐ Die Maß-Präzision wird aus den Firmendaten übernommen.
☑ Für die Produktion soll die Maß-Präzision auf 1/256 fixiert werden.

**Verbundtyp an 2. Stelle** Nur Pool.asc-Übergabe. Wenn in der Stückliste ein Artikel der Produktgruppen UV-Randverbund oder Schmaler Randverbund vorhanden ist, kann an Stelle 2 des Randverbund-Feldes (Feld 77 des Positionssatz) das Kennzeichen 1 (für UV-Randverbund) oder 2 (für Schmaler Randverbund) geschrieben werden.
☐ Für diese Bearbeitungen wird kein Kennzeichen übergeben.
☑ Der Verbundtyp des Abstandhalter-Kennzeichens wird an Stelle 2 im Feld des Abstandhalter-Kennzeichens (Feld 80) exportiert.

**Kundenlogo anhand von Lieferanschrift** Wird nur kundenspezifisch genutzt.

**Stufung VSG auf Stücklistenebene übergeben** Nur Pool.asc-Übergabe. Die Übergabe der Stufung kann für die Produktion von VSG in einem ISO gesondert eingestellt werden.
☐ Die Stufung wird auf der Ebene des Hauptprodukts übergeben.
☑ Die VSG-Stufung wird als Bearbeitung an den gestuften Gläsern übergeben.

> **ISO mit VSG**
> Für die korrekte Übergabe von Daten an A+W Production sollten Sie das Kennzeichen immer dann setzen, wenn in Isolierglas-Einheiten ein VSG mit Stufung eingebaut wird.

**Übergabe Stufung am Stücklistenelement** Nur Pool.asc-Übergabe. Die Übergabe der Stufung aller Positionen, in denen kein VSG verarbeitet wird, kann insgesamt eingestellt werden.
☐ Die Stufung wird auf der Ebene des Hauptprodukts übergeben.
☑ Die Stufung wird als Bearbeitung an den entsprechenden Gläsern übergeben.

**Fremdschlüssel Verpackung übergeben** Nur Pool.asc-Übergabe. Pro Auftrag kann eine geeignete Verpackungsart angegeben werden. Wenn in den Stammdaten Fremdschlüssel für Verpackungsarten hinterlegt sind, können diese an die Produktion übergeben werden.
☐ Der Fremdschlüssel wird nicht übergeben.
☑ Der Fremdschlüssel wird als Gestellvorgabe mit an die Produktion übergeben.

**Artikel in Stückliste exportieren** Standardmäßig werden nur Artikel aus der Hauptproduktebene an die Produktion übergeben. Die Übergabe der einzelnen Stücklistenartikel kann eingestellt werden.
☐ Artikel aus der Stückliste werden nicht übergeben.
☑ Die einzelnen Artikel in der Stückliste werden übergeben.

### Sonstiges

**Positionslimit pro Übergabedatei** Bei der Pool.asc-Übergabe werden die Positionen aller Aufträge eines Nummernverwalters in eine Übergabedatei geschrieben. Wenn regelmäßig sehr viele Aufträge und/oder sehr viele Positionen übergeben werden, kann festgelegt werden, wann eine neue (zweite) Datei begonnen werden soll, z. B. nach 50 Positionen.
Wenn Sie mit OrderXML arbeiten, wird für jeden Auftrag eine eigene Datei erzeugt. In diesem Feld sollte dann eine 0 (null) stehen.

## Einstellungen Produktionsübergabe – Zusätzliche Schnittstellen

**Navigation:** Fertigung > Produktion > Übergabe Produktion > Menü Funktionen > Einstellungen > Register Spezielle Einstellungen

[Image: Abb. E-88 Einstellungen-Produktionsübergabe - Zusätzliche Schnittstellen]

In diesem Register legen Sie die Daten für weitere Schnittstellen fest.

### RONA / LIOPT

Wenn Sie nicht mit A+W Production arbeiten, müssen Sie den Export und den Pfad für zusätzliche Übergabedateien für diese Schnittstellen festlegen.
Die LIOPT-Schnittstelle steht ab A+W Business-Release 2012 nicht mehr zur Verfügung.

**Export aktiv** Der Export der zusätzlichen Übergabedatei muss für die entsprechende Schnittstelle aktiviert werden.
☐ Die Schnittstelle wird nicht benutzt, es wird keine Übergabedatei geschrieben.
☑ Eine zusätzliche Übergabedatei für RONA oder LIOPT soll in dem unten angegebenen Pfad geschrieben werden.

**Pfad/Dateiname** Wenn Sie den Export aktiviert haben, müssen Sie den Pfad und Dateinamen angeben.

### Sicherheitskopien

Diese Einstellungen betreffen nur die Pool.asc-Schnittstelle.

**Erstellen** Wenn Sie mit der Pool.asc-Schnittstelle arbeiten, können Sie eine Sicherheitskopie von der Übergabedatei erstellen lassen.
☐ Eine Sicherheitskopie wird nicht erstellt.
☑ Von jeder Pool.asc-Datei wird automatisch eine Sicherheitskopie gespeichert.

**Pfad/Dateiname** Wenn Sie eine automatische Sicherheitskopie speichern, müssen Sie den Pfad und Dateinamen angeben.

**Datei löschen nach ... Tag(en)** Wenn Sie eine automatische Sicherheitskopie speichern, können Sie festlegen, nach wie vielen Tagen diese automatisch wieder gelöscht werden soll. Wenn Sie 0 (null) eintragen, werden die Sicherheitskopien nicht automatisch gelöscht. Sie sollten dann das entsprechende Verzeichnis manuell von den nicht mehr benötigen Dateien bereinigen.

## Einstellungen Produktionsübergabe – Texte/Anlagen

**Navigation:** Fertigung > Produktion > Übergabe Produktion > Menü Funktionen > Einstellungen > Register Texte/Anlagen

[Image: Abb. E-89 Einstellungen-Produktionsübergabe - Texte/Analgen]

In diesem Register legen Sie fest, welche Texte und Dateianhänge mit an die Produktion übergeben werden sollen.

### Kennzeichen von zu übertragenden Texten

Im Auftrag können für den gesamten Auftrag und/oder für einzelne Positionen Texte hinterlegt werden. Über ein Textkennzeichen ist jeder Text einer Textart zugeordnet. Sie können die Checkbox der Textart markieren, die an die Produktion übergeben werden soll. In der Regel ist dies das Kennzeichen P. Sie können mehrere Textkennzeichen markieren.

### Kennzeichen von zu übertragenden Dateianhängen

Im Auftrag können für den gesamten Auftrag und/oder für einzelne Positionen Dateien mit zusätzlichen Informationen angehängt werden, z. B. grafische Darstellungen zu einem Modell oder zur Sprossenkonstruktion.
☐ Dateianhänge werden nicht an die Produktion übergeben.
☑ Dateianhänge werden mit übergeben.

## Modellliste

**Navigation:** Fertigung > Produktion > Modellliste

[Image: Abb. E-90 Modellliste]

In diesem Dialog können Sie sich die Aufträge anzeigen lassen, in denen ein bestimmtes Modell zu einem bestimmten Termin geliefert werden soll. Sie können sich damit z. B. einen Überblick über die Aufträge mit freien Formen verschaffen, die manuell zugeschnitten werden müssen.
Das Ergebnis der Suche kann als Report gedruckt werden.

### Selektion

**Artikelnummer** Eingabe der Artikelnummer (Produktnummer), nicht der Modellnummer.

**Lieferdatum** Eingabe des Lieferdatums, zu dem das angegebene Modell geliefert werden soll.

### Artikel

**Bezeichnung, Bezeichnung 2** Bezeichnung des gewählten Produkts aus den Stammdaten.

### Übersicht

In der Übersicht werden alle Aufträge aufgelistet, in denen das gewählte Modell zum angegebenen Termin geliefert werden soll.
- **Auftragsnummer:**
  Nummer des Auftrags, in dem das gesuchte Modell enthalten ist.
- **Pos:**
  Nummer der Auftragsposition.
- **Kunde:**
  Name des Kunden, für den dieser Auftrag gefertigt wird.
- **Artikelnummer:**
  Nummer des Produkts.
- **Bezeichnung 1, 2, 3:**
  Bezeichnungen zum Produkt.
- **Tour:**
  Tour, mit der der Auftrag ausgeliefert werden soll.

## Gestellbelegung prüfen

**Navigation:** Fertigung > Produktion > Gestellbelegung

**Zu Dialogbeschreibung:**
⇨ Einstellungen (Gestellbelegung prüfen)

[Image: Abb. E-91 Gestellbelegung]

In diesem Dialog können Sie die Gestellbelegung für die Aufträge prüfen, die produziert werden. Den Aufträgen müssen bereits Gestelle zugeordnet sein.

### Menü Funktionen

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Dialog zu schließen. Folgende Einträge werden angezeigt:
- **ASCII-Datei erstellen:**
  Schreibt die Daten werden in eine ASCII-Datei.
- **Einstellungen:**
  Öffnet den Dialog Einstellungen, in dem Sie die Einstellungen für die ASCII-Datei festlegen.
  ⇨ "Einstellungen (Gestellbelegung prüfen)" auf Seite E-191

### Auswahl

**Mitarbeiter** Name des Mitarbeiters, der sich in A+W Business angemeldet hat.

**Nummernverwalter** Auswahl des Nummernverwalters, auf den der Dialog zugreifen soll.

### Sortierkriterien

Mit der Wahl der Option legen Sie fest, in welcher Reihenfolge die Aufträge in der Übersicht dargestellt werden sollen:
- **Nach Auftrags- + Positionsnummern:**
  Die Anzeige wird zuerst nach Auftrags- und dann nach Positionsnummern sortiert.
- **Nach Bestelltext1 + Kundenposition:**
  Die Anzeige wird zuerst nach Bestelltext 1 und dann nach Kundenposition sortiert.
- **Alle:**
  Alle Aufträge im gewählten Nummernverwalter werden angezeigt.
- **Außer TPS:**
  Aufträge mit TPS werden nicht angezeigt.
- **Nur TPS:**
  Nur die Aufträge mit TPS werden angezeigt.

### Übersicht

In der Übersicht werden die Aufträge angezeigt, die sich im gewählten Nummernverwalter befinden.
- **Nummer:**
  Laufende Nummer in der Übersicht.
- **Nummer Kunde/Lief., Kunde/Lieferant:**
  Nummer und Name des Kunden oder Lieferanten.
- **Status:**
  Status des Auftrags oder der Position.
- **Bestelltext1:**
  Bestelltext 1 aus dem Auftrag.
- **Bock-/Fachnummer:**
  Bock- oder Fachnummer auf dem Gestell.
- **Sortierung:**
  Kennzeichen für die Sortierung.
- **Verpackungsart:**
  Art der Verpackung, z. B. Gestell, Kiste.
- **Datum Prod. ISO, VSG, ESG:**
  Datum, an dem das ISO, VSG oder ESG produziert wird.
- **Lauf-Nr. Prod. ISO, VSG, ESG:**
  Nummer des Laufs, in dem das ISO, VSG oder ESG produziert wird.
- **Datum Lieferung:**
  Lieferdatum aus dem Auftrag.
- **Lieferschein:**
  Nummer des Lieferscheins.
- **Tour:**
  Name der Tour, mit der geliefert wird.
- **Gewicht gesamt:**
  Gewicht aller Auftragspositionen.
- **Stück gesamt:**
  Stückzahl aller Auftragspositionen.
- **Qm gesamt:**
  Fläche aller Auftragspositionen.
- **LFM gesamt:**
  Laufmeter der Kanten.
- **Datum Erfassung:**
  Erfassungsdatum des Auftrags.

## Einstellungen (Gestellbelegung prüfen)

**Navigation:** Fertigung > Produktion > Gestellbelegung > Menü Funktionen > Einstellungen

Für L-Gestelle können Sie zusätzliche Voreinstellungen festlegen. Diese Einstellungen sind insbesondere für TPS wichtig.

In diesem Dialog finden Sie folgende Register:
- "Einstellungen – Gemeinsam" auf Seite E-192
- "Einstellungen – Kunden" auf Seite E-193

### Einstellungen – Gemeinsam

**Navigation:** Fertigung > Produktion > Gestellbelegung > Menü Funktionen > Einstellungen

[Image: Abb. E-92 Gestellbelegung – Einstellungen für den Datenexport]

In diesem Dialog können Sie die Kriterien für die Übergabedatei festlegen. Die Gestellbelegung kann in eine ASCII-Datei geschrieben werden.

**Pfad ASCII-Datei** Eingabe des Pfads für die ASCII-Datei. Standardmäßig wird in ein temporäres Verzeichnis auf C:\ gespeichert. Der Name der Datei wird aus Kundennummer, Tag und Monat gebildet.

**Verpackungsart**
Sie können die Verpackungsart für die Aufträge einstellen, deren Daten exportiert werden sollen. Nur die Verpackungsarten werden zur Auswahl angeboten, die in den Stammdaten hinterlegt sind.

**Druck**
Mit der Wahl der Option legen Sie fest, wie die Daten gedruckt werden sollen.

**L-Gestelle TPS, L-Gestelle**
Geben Sie an, wie groß die Anzahl der Fächer für die Gestelle sein darf. Die Höchstzahl für TPS ist 22, für die restlichen L-Gestelle 21. Sie können außerdem die Höchstmaße für die jeweiligen Fächer angeben.
Die Daten werden vor dem Schreiben der ASCII-Datei geprüft.

### Einstellungen – Kunden

**Navigation:** Fertigung > Produktion > Gestellbelegung > Menü Funktionen > Einstellungen > Kunden

[Image: Abb. E-93 Gestellbelegung – Einstellungen für den Datenexport]

Sie können für einzelne Kunden festlegen, mit welcher Startnummer die Zählung der benötigten Gestelle standardmäßig beginnen soll.

**Kundenindividuelle Einstellungen**
- **Kunde** Nummer und Name des Kunden, für den die Einstellungen festgelegt werden.
- **Zuschlagsartikel** Produktnummer des Zuschlags, der berechnet wird.
- **Gestellstartnummer** Startnummer des Gestells.
- **[Neu], [Löschen]** Schaltet eine neue Zeile in der Übersicht frei, löscht einen markierten Eintrag.

## Barcode-Übergabe

**Navigation:** Fertigung > Produktion > Übergabe Barcode Prod.

Sie können die einzelnen Positionen von Aufträgen per Barcode an die Produktion übergeben. Dazu steht Ihnen der Dialog Produktionsübergabe (pos. orient.) zur Verfügung.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite E-194
- "Übergabe Barcode Prod." auf Seite E-195

### Menü Funktionen

**Navigation:** Fertigung > Produktion > Übergabe Barcode Prod.

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Produktionsübergabe zu schließen.

Das Menü ist in folgende Gruppen gegliedert:
- Gruppe Produktion
- Gruppe Kapazitätsplanung

#### Gruppe Produktion
- **Einstellungen:**
  Öffnet den gleichnamigen Dialog, in dem Sie die Einstellungen für die Übergabedatei festlegen können.
  ⇨ "Einstellungen Produktionsübergabe" auf Seite E-174
- **Übersicht Auftrag:**
  Öffnet den Dialog Übersicht Statusrückmeldungen, in dem Sie sich pro Auftrag und Position anzeigen lassen können, welcher Status aus der Produktion zurückgemeldet wurde.
  ⇨ Verkauf, "Übersicht Statusrückmeldung" auf Seite C-590
- **Läufe löschen:**
  Löscht die angegebenen Läufe.

#### Gruppe Kapazitätsplanung
- **Bearbeitungen:**
  Öffnet den Dialog Arbeitsarten, in dem Sie sich die Auslastung pro Arbeitsarten anzeigen lassen können. Die entsprechenden Daten stehen nur zur Verfügung, wenn Sie mit der Kapazitätsplanung von A+W Business arbeiten.
  ⇨ Kapazitätsplanung, “Arbeitsarten" auf Seite H-198

## Übergabe Barcode Prod.

**Navigation:** Fertigung > Produktion > Übergabe Barcode Prod.

Wenn Sie mit Scannern arbeiten, können Sie die einzelnen Auftragspositionen per Barcode an die Produktion übergeben.

In diesem Dialog finden Sie folgende Register:
- "Übergabe Barcode Prod. – Übersicht" auf Seite E-195
- "Übergabe Barcode Prod. - Details" auf Seite E-196

### Übergabe Barcode Prod. – Übersicht

**Navigation:** Fertigung > Produktion > Übergabe Barcode Prod. > Register Übersicht

[Image: Abb. E-94 Übergabe Barcode Prod. - Übersicht]

In diesem Register legen Sie Läufe nach Arbeitsarten an. Die Laufnummer wird aus dem Nummernkreis für AWPool gewählt. Dabei können Mandanten und AV-Bereiche berücksichtigt werden.

#### Identifikation

**Mandant** Wenn Sie mit unterschiedlichen Mandanten arbeiten, werden diese zur Auswahl angeboten.

**Bereich** Wenn Sie unterschiedliche AV-Bereiche angelegt haben, werden diese zur Auswahl angeboten.

**Kommentar** Sie können einen Kommentar für die Mitarbeiter schreiben, um z. B. auf Besonderheiten aufmerksam zu machen.

#### Läufe

In der Übersicht sind alle Läufe aufgelistet, die an die Produktion übergeben werden sollen oder wurden. Dabei werden zuerst alle Läufe aufgeführt, die noch nicht übergeben wurden, und anschließend die bereits übergebenen. Die Anzahl der anzuzeigenden Läufe kann über das Menü Funktionen > Anzahl Läufe eingeschränkt werden.

- **Nummer:**
  Nummer des Laufs.
- **Status:**
  Aktueller Status des Laufs.
- **Kommentar:**
  Text, der im Feld Kommentar eingegeben wurde.

### Übergabe Barcode Prod. – Details

**Navigation:** Fertigung > Produktion > Übergabe Barcode Prod. > Register Details

[Image: Abb. E-95 Übergabe Barcode Prod. – Details]

In diesem Register fügen Sie Positionen per Barcode oder manuell hinzu.
Die aktuelle Laufnummer aus dem Register Übersicht wird angezeigt. Nur zu diesem Lauf können Aufträge und Positionen eingefügt werden.

#### Eingabe

**Barcode** Anzeige des gescannten Barcodes.
Wenn Sie die Position manuell erfassen, können Sie je nach gewähltem Typ den Arbeitsgang, die Auftragsnummer und/oder Gruppen- oder Positionsnummer eingeben. Im linken Feld können Sie maximal 11 Zeichen eingeben, im rechten 3.

**Typ** Mit der Wahl der Option legen Sie fest, welche Nummern Sie scannen bzw. eingeben:
- **Arbeitsgang:**
  Mit dieser Option scannen Sie den Arbeitsgang.
- **Auftrags-/Gruppennummer:**
  Mit dieser Option scannen Sie im linken Feld die Nummer des Auftrags, im rechten die Nummer der Gruppe.
- **Auftrags-/Positionsnummer:**
  Mit dieser Option scannen Sie im linken Feld die Nummer des Auftrags, im rechten die Nummer der Position.

Die Daten von Aufträgen oder Positionen werden nicht weiterverarbeitet, wenn sie schon in anderen Läufen vorhanden sind.

#### Einstellungen

**Anzahl Läufe** Anzahl der Läufe, die maximal angezeigt werden. Ein neuer Lauf kann auch dann angelegt werden, wenn diese Höchstzahl erreicht ist. In diesem Fall wird der älteste Lauf (kleinste Laufnummer) gelöscht.

**Erfassungsstelle** Angabe der Erfassungsstelle.

#### Prüfziffern

In diesem Bereich können Sie zu den Barcodes von Arbeitsgängen, Gruppen- und Auftragsnummern und/oder Auftrags- und Positionsnummern eine einstellige Prüfziffer eingeben.
Die Prüfziffer kann eine Zahl oder Buchstabe sein. Die Prüfziffern müssen nicht fortlaufend sein, z. B. sind folgende Eingaben möglich: 1, 2, 3 oder 7, 4, 6 oder G, 3, Z.

**Arbeitsgang** Prüfziffer für den Barcode des Arbeitsgangs, der gescannt wird.

**Auftrags-/Gruppennummer** Prüfziffer für den Barcode der Gruppe oder des Auftrags, die gescannt werden.

**Auftrags-/Positionsnummer** Prüfziffer für den Barcode der Aufträge oder Positionen, die gescannt werden.

#### Arbeitsgang

**Arbeitsgänge auswählen**
> Sie können nur Arbeitsgänge auswählen, die in den Stammdaten zur Fertigung eingerichtet sind. Die Arbeitsgänge können gescannt werden.

Wenn Sie die Option Arbeitsgang gewählt haben, können Sie in der Kombobox den gewünschten Arbeitsgang auswählen.

**Enthaltene Bearbeitungen** In diesem Feld werden alle Bearbeitungen angezeigt, die in dem gewählten Arbeitsgang enthalten sind.

**[Alles löschen]** Löscht alle Einträge aus dem Lauf. Wenn Sie einen einzelnen Eintrag aus dem Lauf entfernen möchten, müssen Sie diesen markieren und im Menü Start > Löschen wählen.

#### Lauf

In der Übersicht werden alle Auftragspositionen aufgelistet, die zu dem aktuellen Lauf hinzugefügt wurden.
- **Auftr.Nr.:**
  Nummer des Auftrags.
- **Pos. Nr.:**
  Nummer der Position im Auftrag.
- **Bezeichnung:**
  Produktbezeichnung.
- **Menge:**
  Menge der Position oder Gruppe.
- **QM:**
  Gesamtfläche der Position oder Gruppe.
- **Gewicht:**
  Gesamtgewicht der Position oder Gruppe.
- **Arbeitsgang:**
  Arbeitsgang, in dem die Position gefertigt wird.
- **Gesamt:**
  Gesamtsummen über alle aufgeführten Positionen.

## Produktionsdaten

**Navigation:** Fertigung > Produktion > Produktionsdaten

Aufträge des Typs Produktionsauftrag dienen dazu, Produkte für das eigene Lager zu produzieren. In Produktionsaufträgen werden die verwendeten Rohmaterialien und alle produktionsrelevanten Daten erfasst.

Als zusätzliche Möglichkeit kann durch die Eingabe der Produktionsdaten und den anschließenden Buchungsvorgang das verwendete Rohmaterial vom Lager abgebucht und die jeweiligen Positionen des Produktionsauftrages dem Lager zugebucht werden.

### Produktionsdaten (Dialog)

**Navigation:** Fertigung > Produktion > Produktionsdaten

In diesem Dialog können Sie alle Daten, die zur Produktion erforderlich sind, erfassen und verbuchen.
In diesem Dialog finden Sie folgende Register:
- "Produktionsdaten - Auftrag" auf Seite E-200
- "Produktionsdaten - Tabelle" auf Seite E-202
- "Produktionsdaten – Buchung" auf Seite E-203

### Produktionsdaten – Auftrag

**Navigation:** Fertigung > Produktion > Produktionsdaten > Register Auftrag

[Image: Abb. E-96 Produktionsdaten - Auftrag]

In diesem Dialog können Sie alle Daten, die zur Produktion erforderlich sind, erfassen und verbuchen. Beachten Sie dabei, dass alle Felder zwingend gefüllt werden müssen, bis auf die Angabe eines Ausfallgrundes.

#### Allgemein

**Datum** Datum der Fertigung. Wenn Sie die Daten für die Zugangsbuchung im Lager eingeben, ist dies das Datum, an dem der Produktionsauftrag gefertigt werden soll oder gefertigt wurde.

**Aggregat** Hier wählen Sie die Maschine aus, mit der der Produktionsauftrag gefertigt wird.

**Schicht** Schichten werden bei Produktionsaufträgen nicht berücksichtigt. Das Feld kann leer bleiben.

**Bearbeiter** Name des Mitarbeiters.

#### Produktionsdetails

**Rüstzeit/Laufzeit (Minuten)** Die Rüstzeit und die Dauer der Fertigung geben Sie in Minuten ein.

**Personenanzahl** Anzahl der Personen, die für die Fertigung des Produktionsauftrags eingesetzt werden.

**Ausfallzeit (Minuten)** Die Ausfallzeit wird in Minuten angegeben.

**Grund des Ausfalls** Wenn Sie eine Ausfallzeit angegeben haben, können Sie zusätzlich angeben, wodurch der Ausfall verursacht wurde. Einmal eingegebene Ausfallgründe bleiben in der Kombobox erhalten und können anschließend ausgewählt werden.

#### Produktionsauftragsdaten

**Auftrag** Nummer des Produktionsauftrags.

**Position/Menge** Nummer und Menge der Position im Auftrag.

#### Fertigprodukt

**Artikel** Produktnummer der gefertigten Einheiten, die in den Produktstammdaten hinterlegt ist. Mit dieser Nummer wird das Fertigprodukt in den Lagerbestand gebucht.

**Breite/Höhe** Wenn die Nummer eingetragen ist, werden die Beschreibungen, Maße und Gewicht aus den Stammdaten automatisch angezeigt.

**Anzahl Einheiten** Anzahl der gefertigten Einheiten der aktuellen Position.

**Identnummer automatisch erzeugen** Bei der Verbuchung können automatisch Kisten-Identnummern (Kisten-ID) vergeben werden.
☐ Kisten werden nicht verbucht.
☑ Im Produktionsauftrag sind Kisten enthalten, denen bei der Verbuchung automatisch IDs zugewiesen werden sollen. Nur so ist es auch möglich abweichende Inhalte anzugeben. Handelt es sich bei dem Produkt jedoch um eine Kiste mit tiefer Stückliste und enthält diese die Gläser nicht direkt als erstes Stücklistenelement, können die Inhalte nicht geändert werden.

**Scheiben pro Einheit** ISO-Scheiben können aus 2, 3 oder sogar 4 Scheiben bestehen. In der Regel werden 2 Scheiben pro Einheit verbaut.

**Scheiben fertiggestellt** Anzahl der zugeschnittenen Scheiben.

#### Rohmaterial

**Artikel** Produktnummer des Glases (oder der Lagerplatte), das geschnitten wird.

**Breite/Höhe** Maße des Rohmaterials.

**Bruch** In diesem Feld können Sie den Bruch von Rohmaterial eintragen.

**Bruch auf Maschine** Das Feld wird durch die Rückmeldung aus A+W Production gefüllt.

**Lieferant** Lieferant des Rohmaterials.

**Lagermaße im Lauf** Anzahl der Lagerplatten, die verschnitten wurden.

**Scheiben pro Lagermaß** In diesem Feld tragen Sie die Anzahl der Scheiben ein, die aus der Lagerplatte geschnitten wurden.

**Verschnitt** Verschnitt in qm, der beim Schneiden der Scheiben von einer Lagerplatte als Rest übrig bleibt.

**Beispiel**
Lagerplatte 3210 x 5000 mm = 16,05 qm
Zugeschnitten: 2 Stück Float 4:
2000 x 3210 mm = 6,42 qm/Stk = 12,84 qm
Verschnitt = 3,21 qm

### Produktionsdaten – Tabelle

**Navigation:** Fertigung > Produktion > Produktionsdaten > Register Tabelle

[Image: Abb. E-97 Produktionsdaten - Tabelle]

In diesem Register werden die Positionen eines Produktionsauftrags angezeigt, zu denen Sie Produktionsdaten erfasst haben.

### Produktionsdaten – Buchung

**Navigation:** Fertigung > Produktion > Produktionsdaten > Register Buchung

[Image: Abb. E-98 Produktionsdaten – Buchung]

In diesem Register können Sie die erfassten Daten verbuchen. Die Daten werden in komprimierter Form pro Aggregat (Maschine) angezeigt.
Die Buchung wird nur für die Einträge ausgeführt, die im Zeilenkopf mit einem x markiert sind. Mit der Verbuchung werden die Rohmaterialien vom Lager ab- und die produzierten Positionen zugebucht.

# Lieferwesen

**Navigation:** Fertigung > Lieferwesen

Sie können die Lieferung von produzierten Aufträgen planen und steuern, indem Sie Aufträge nach Touren, Datum, Gestell usw. zusammenfassen.

In diesem Abschnitt finden Sie Informationen zu folgenden Dialogen des Programmbereichs:
- "Tourenliste" auf Seite E-207
- "Statusmeldung und Packmittelzuordnung" auf Seite E-220
- "Kommissionierung" auf Seite E-230
- "Listendruck" auf Seite E-235
- "Warenausgang Kisten" auf Seite E-239

## Tourenliste

**Navigation:** Fertigung > Lieferwesen > Tourenliste

Mit Hilfe der Tourenliste können Sie den Versand planen. Die Liste können Sie sich nach verschiedenen Auswahlkriterien anzeigen und ausdrucken lassen, z. B. nach Liefertermin, Tour, Status.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menüs im Dialog Tourenliste" auf Seite E-205
- "Tourenliste" auf Seite E-207
- "Versanddaten ändern" auf Seite E-216
- "Einstellungen (KAPS-Datei)" auf Seite E-217

### Menüs im Dialog Tourenliste

Über die Menüs im Dialog Tourenliste können Sie die Standardeinstellung des Dialoges bestimmen und andere Dialoge öffnen, ohne die Tourenliste zu schließen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite E-205
- "Menü Optionen" auf Seite E-206

### Menü Funktionen

**Navigation:** Fertigung > Lieferwesen > Tourenliste

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Tourenliste zu schließen.

Das Menü ist in folgende Gruppen gegliedert:
- Gruppe Tour
- Gruppe Navigation
- Gruppe KAPS
- Gruppe Sonstiges

#### Gruppe Tour
- **Historie:**
  Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des markierten Dokuments.
  ⇨ Verkauf, "Historie" auf Seite C-564
- **Teillieferung:**
  Öffnet den Dialog Dokumente kopieren im Modus Teillieferung, in dem Sie eine Teillieferung erstellen können.
  ⇨ Verkauf, "Dokumente kopieren" auf Seite C-543
- **Versanddaten ändern:**
  Öffnet den Dialog Touren/Liefertermine umsetzen, in dem Sie die Tour und/ oder den Liefertermin ändern können.
  ⇨ "Versanddaten ändern" auf Seite E-216
- **Selektierte, Alle in Nummernverwalter kopieren:**
  Öffnet den Dialog NV Auswahl, in dem Sie alle Aufträge in einen anderen Nummernverwalter stellen können.
  ⇨ Verkauf, "NV Auswahl" auf Seite C-567

#### Gruppe Navigation
- **Vorheriger Tag/Tour, Nächster Tag/Tour:**
  Wechselt die Darstellung in der Übersicht im Register Tabelle.

#### Gruppe KAPS
- **Datei erstellen:**
  Mit dieser Funktion starten Sie die Erstellung der KAPS-Datei. Wenn sich sehr viele Aufträge im gewählten Nummernverwalter befinden, kann dieser Vorgang einige Zeit in Anspruch nehmen.
- **Pfad für Datei:**
  Öffnet einen Dialog zum Festlegen des Speicherorts.
  ⇨ "Einstellungen (KAPS-Datei)" auf Seite E-217

#### Gruppe Sonstiges
- **Einstellungen:**
  Dieser Eintrag ist nur kundenspezifisch freigeschaltet. Über ihn können die Höchstmaße des Glases für die Tourenliste festgelegt werden.
- **Dokument anzeigen:**
  Öffnet die Vorschau auf das Dokument.

### Menü Optionen

**Navigation:** Fertigung > Lieferwesen > Tourenliste

Über dieses Menü können Sie die Standardeinstellung für den Druck bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

Das Menü ist in folgende Gruppen gegliedert:
- Gruppe Tabelle
- Gruppe Druckoptionen

#### Gruppe Tabelle
- **Mehrere Zeilen selektierbar:**
  Mit dieser Option können Sie in der Übersicht mehrere Zeilen markieren, wenn Sie die Taste <Strg> gedrückt halten.

#### Gruppe Druckoptionen

- **Name des Lieferanten:**
  Der Name des Lieferanten wird auf der Tourenliste gedruckt. Diese Option ist sinnvoll, wenn in der Lieferung Bestellartikel enthalten sind.
- **Ersten Positionstext:**
  Der Positionstext 1 aus dem Auftrag wird auf der Tourenliste gedruckt.
- **Produktbezeichnung 1 - 3:**
  Die Produktbezeichnungen 1 - 3 werden auf der Tourenliste gedruckt.
- **Bleiverglasung:**
  Scheiben mit Bleiverglasung werden auf der Tourenliste gekennzeichnet, damit der Versand die Scheiben entsprechend verpackt.
- **Zuschlags- und Leistungspositionen:**
  Zuschläge und Leistungen werden auf der Tourenliste gedruckt.

> **Angaben auf der Tourenliste nicht gedruckt**
> Wenn Sie sehr viele Optionen für den Druck der Tourenliste gewählt haben, sollten Sie im Drucker-Dialog die Einstellung Querformat wählen. Die gewünschten Spalten werden sonst nicht auf dem Bildschirm oder in der Liste dargestellt.

## Tourenliste

**Navigation:** Fertigung > Lieferwesen > Tourenliste

**Zu Dialogbeschreibung:**
- Versanddaten ändern
- ⇨ Einstellungen (KAPS-Datei)

Mit Hilfe der Tourenliste können Sie den Versand planen. Die Aufträge einer Tour können Sie sich nach verschiedenen Auswahlkriterien zusammenstellen, z. B. nach Liefertermin, Produkt, Status.

In diesem Dialog finden Sie folgende Register:
- "Tourenliste – Selektion" auf Seite E-208
- "Tourenliste – Tabelle" auf Seite E-212

### Tourenliste – Selektion

**Navigation:** Fertigung > Lieferwesen > Tourenliste > Register Selektion

[Image: Abb. E-99 Tourenliste – Selektion]

In diesem Register legen Sie die Kriterien fest, nach denen die Tour zusammengestellt werden soll.

#### Kriterien

Mit der Wahl der Option legen Sie fest, nach welchen Kriterien die Touren angezeigt werden sollen.
- **Versand:**
  Das angegebene Datum betrifft den Versandtag.
- **Anlieferung:**
  Das angegebene Datum betrifft den Tag der Anlieferung beim Kunden.

**(Termin) von ... bis** Diese Felder sind nur freigeschaltet, wenn Sie keinen Nummernverwalter ausgewählt haben. Sie können dann Touren nach einer gewünschten Zeitspanne zusammenstellen.
Wenn Sie einen Nummernverwalter gewählt haben, sind die Felder gesperrt und das aktuelle Tagedatum wird angezeigt.

**Tourenstamm** Mit der Wahl dieser Option legen Sie fest, welche Touren im Feld Verfügbare Touren angezeigt werden.
- **Stammdaten:**
  Alle Touren aus A+W Business werden angezeigt.
- **Routenoptimierung:**
  Alle optimierten Routen aus OTR werden angezeigt.

**Verfügbare Touren** In der Liste werden alle Touren angezeigt, die in den Stammdaten angelegt sind. Touren, die in das Feld Anzuzeigende Touren/Reihenfolge übernommen wurden, werden in der Liste nicht mehr angezeigt.

**Anzuzeigende Touren / Reihenfolge** In der Liste werden alle Touren angezeigt, zu denen Tourenlisten zusammengestellt werden sollen. Die Reihenfolge der Touren kann mit den Pfeilschaltflächen unter dem Feld geändert werden.

**Status von, Status bis** Sie können einen Anfangs- und einen End-Status einstellen, um nur die Aufträge auszuwählen, die diesen Kriterien entsprechen. Die Felder sind gesperrt, wenn Sie einen Nummernverwalter ausgewählt haben.

**Nummernverwalter** Sie können die Aufträge für die Tourenplanung vorab in einem Nummernverwalter zusammenstellen.
☐ Die Aufträge werden nicht aus einem Nummernverwalter angezeigt.
☑ Die Tourenlisten sollen aus den Aufträgen in einem Nummernverwalter zusammengestellt werden. Das Feld zur Auswahl des Nummernverwalters wird freigeschaltet.

**AV-Bereiche** Sie können als zusätzliches Kriterium einen oder mehrere AV-Bereiche auswählen. Für die Mehrfachauswahl halten Sie die Taste <Strg> gedrückt.

**Auflösungstiefe**
Mit der Wahl der Option legen Sie fest, wie die Liste auf dem Monitor und im Druck ausgegeben werden soll:
- **Auftrag:**
  Nur die Auftragsnummern werden angezeigt bzw. gedruckt.
- **Position:**
  Die Auftrags- und die Positionsnummern werden angezeigt bzw. gedruckt.
Wenn Sie den Liefertermin gewählt und bestätigt haben, können Sie die Einstellungen im Register Tabelle prüfen.

**Inklusive Bearbeitungen** Unabhängig von der Option zur Auflösungstiefe können Sie festlegen, ob Bearbeitungen angezeigt werden sollen.
☐ Bearbeitungen werden nicht ausgegeben.
☑ Bearbeitungen werden in der Tourenliste mit einem X in der Spalte Bearb. angezeigt.

**Sortierung innerhalb der Touren**
Mit der Wahl der Option legen Sie fest, wie die Reihenfolge der Lieferungen innerhalb einer Tour sortiert werden soll.
- **AV-Bereich/Rangfolge/Kundennummer:**
  Die Lieferungen werden zunächst nach AV-Bereichen sortiert. Innerhalb des AV-Bereiches wird die Tour nach der Rangfolgenummer sortiert, die in den Stammdaten der jeweiligen Kunden eingetragen ist.
- **Kundennummer/Status:**
  Die Lieferungen werden zunächst nach Kundennummern und dann nach Status sortiert. Diese Option ist dann sinnvoll, wenn in den Stammdaten keine Rangfolgenummern eingetragen sind.
- **Rangfolge/Kundennummer:**
  Die Lieferungen werden zunächst nach der Rangfolgenummer und dann nach Kunden sortiert.
- **Kundennummer/Lieferanschrift (PLZ, Ort, Str.):**
  Die Lieferungen werden zunächst nach Kundennummern und dann nach Lieferanschrift sortiert.
- **Routenoptimierung:**
  Die Lieferungen werden nach Routenoptimierung sortiert. Diese Option ist nur freigeschaltet, wenn beim Feld Tourenstamm die Option Routenoptimierung gewählt ist.

**Seitenwechsel bei Druck**
Mit der Wahl der Option legen Sie fest, wie die Liste gedruckt werden soll. Die Wahl richtet sich auch nach den Kriterien, mit denen Sie die Tourenliste zusammengestellt haben.
- **Tour/Datum:**
  Beim Wechsel der Tour und/oder des Datums wird eine neue Seite gedruckt.
- **Tour/Datum/Kunde:**
  Für jede Tour wird pro Datum und Kunde eine neue Seite gedruckt.
- **Kein Wechsel:**
  Die Tourenliste wird ohne Seitenwechsel gedruckt.
- **Tour/Datum/Kunde/Lieferanschr.:**
  Für jede Tour wird pro Datum und Kunde und Lieferanschrift eine neue Seite gedruckt.

**Auszuschließender Status bei Druck**
Sie können Aufträge mit einem bestimmten Status vom Druck ausschließen. Für die Mehrfachauswahl brauchen Sie keine Taste zu drücken. Diese Einstellung ist sinnvoll, wenn Sie die Touren nach Liefertermin zusammenstellen.
Wenn Sie eine Auswahl getroffen haben, werden die entsprechenden Aufträge im Register Tabelle in blauer Schrift dargestellt.

#### Optionen

**Druck von ausgewählter Tour/Datum** Sie können den Druck auf die aktuell angezeigte Tour begrenzen.
☐ Alle Touren zum eingestellten Datum oder aus dem gewählten Nummernverwalter werden gedruckt.
☑ Nur die im Register Tabelle ausgewählte Tour wird gedruckt.

**Ohne Direktanlieferung** Sie können den Druck von Auftragspositionen ausschließen, die direkt von Lieferanten geliefert werden.
☐ Alle Auftragspositionen zur ausgewählten Tour werden gedruckt.
☑ Auftragspositionen mit Direktanlieferung werden nicht gedruckt.

**NV komplett füllen** Sie können die Aufträge einer Tourenliste in einen bestimmten Nummernverwalter stellen.
☐ Kein Nummernverwalter wird gefüllt.
☑ Die Aufträge der Tourenlisten werden in einen Nummernverwalter gestellt. Sie können einen Nummernverwalter auswählen oder einen neuen Nummernverwalter anlegen, indem Sie den Namen eintragen. Diese Einstellung ist sinnvoll, wenn Sie nach der Kommissionierung Listen drucken wollen.
⇨ "Listendruck" auf Seite E-235

**NV löschen** Sie können die Aufträge einer Tourenliste aus einem Nummernverwalter löschen. Die Checkbox ist nur freigeschaltet, wenn Sie die Checkbox NV komplett füllen markiert haben.
☐ In dem gewählten Nummernverwalter werden keine Aufträge gelöscht.
☑ Im gewählten Nummernverwalter werden alle Aufträge gelöscht, so dass nur die neuen Aufträge darin stehen. Diese Einstellung ist sinnvoll, wenn Sie immer denselben Nummernverwalter verwenden wollen.

### Tourenliste – Tabelle

**Navigation:** Fertigung > Lieferwesen > Tourenliste > Register Tabelle

[Image: Abb. E-100 Tourenliste - Tabelle (Auflösungstiefe Auftrag)]

In diesem Register werden alle Aufträge aufgelistet, die den Auswahlkriterien im Register Selektion entsprechen. Sie können die Tourenliste in unterschiedlichen Sortierungen für den Druck anzeigen lassen.

Wenn Sie im Register Selektion > Auszuschließender Status bei Druck eine Auswahl getroffen haben, werden die entsprechenden Aufträge in blauer Schrift dargestellt.

In der Auflösungstiefe Position werden die Kopfdaten in roter Schrift angezeigt.

#### Auswahl

**Datum Tour** In diesem Feld können Sie jede Tour pro Datum auswählen. Aufgelistet werden nur die Touren, die den Auswahlkriterien entsprechen.

**[<], [>]** Mit diesen Schaltflächen können Sie die Liste der Touren im Feld Datum Tour durchblättern.

**Vorschau** In diesem Feld werden die Termine und/oder Lieferungen angezeigt, die zur ausgewählten Tour gehören.
Mit der Wahl der Option können Sie die Vorschau ändern:
- **Nach Datum:**
  In der Vorschau werden alle Touren zum gewählten Datum angezeigt.
- **Nach Tour:**
  In der Vorschau werden zur gewählten Tour alle Termine für 14 Tage im Voraus angezeigt. Anhand der Spalten Menge, Fläche und Gewicht können Sie prüfen, ob ein Lkw genügend ausgelastet ist. Ist die Auslastung eines Lkws z. B. nicht ausreichend, kann in der Übersicht nach einer anderen Tour gesucht werden. Dazu müssen die Fahrzeuge in den Stammdaten angelegt sein. Darüber hinaus wird Ihnen der Netto-Verkaufspreis sowie die Anzahl der Lieferstellen angezeigt. Die Felder können in der Bildschirmtabelle ein- und ausgeblendet werden.
  ⇨ Stammdaten, "Lkw" auf Seite B-876

**[Alle], [Keine]** Mit diesen Schaltflächen können Sie alle Lieferungen in der Übersicht markieren oder an allen die Markierung entfernen.
Sie können die Tour und/oder das Lieferdatum der angezeigten Aufträge ändern. Dazu müssen die Aufträge markiert werden. Sie können einzelne Einträge in der Übersicht mit einem Doppelklick in den Zeilenkopf markieren. Sie können beliebig viele Einträge markieren.
⇨ "Versanddaten ändern" auf Seite E-216

> **Markieren**
> Ein Auftrag ist erst dann markiert, wenn im Zeilenkopf ein x angezeigt wird.

**[Tabelle neu sortieren nach...]** Mit dieser Schaltfläche sortieren Sie die markierten Lieferungen in der Übersicht nach der gewählten Option im Register Selektion.
⇨ "Tourenliste - Selektion" auf Seite E-208

#### Legende

- **Blau:**
  Dokumente werden nicht gedruckt.
- **Rot:**
  Dokumente werden gedruckt.

#### Übersicht

In der Übersicht werden alle Aufträge zu einer Tour und einem Liefertermin aufgelistet. Die Übersicht wird automatisch aktualisiert, wenn Sie mit den Pfeil-Schaltflächen oder im Feld Datum Tour eine andere Tour wählen.
Die Spalten werden je nach Auflösungstiefe gefüllt. Die Einträge in blauer Schrift werden auf der Liste nicht gedruckt, z. B., weil ihr Status vom Druck ausgeschlossen ist.
- **Kunde:**
  Name des Kunden aus dem Auftrag.
- **Auftrag:**
  Auftragsnummer.
- **Menge:**
  Gesamtstückzahl des Auftrags.
- **Pos:**
  Diese Spalte wird nur angezeigt, wenn als Auflösungstiefe die Option Position gewählt wurde. Die folgenden Spalten werden dann pro Position dargestellt.
- **Fläche:**
  Gesamtfläche des Glases pro Auftrag oder Position.
- **Gewicht:**
  Gesamtgewicht pro Auftrag oder Position.
- **Status:**
  Status des Auftrags.
- **Lieferanschrift:**
  Anzeige einer abweichenden Lieferanschrift aus dem Auftrag. Je nach Auflösungstiefe wird zusätzlich auch die Produktbeschreibung angezeigt.
- **Kommission:**
  Kommission der ersten Position des Auftrags.
- **Mod.:**
  Modellnummer für eine Position mit Modell.
- **Rang:**
  Tourrangfolge aus den Kundenstammdaten.
- **Erf. Datum:**
  Erfassungsdatum des Auftrags.
- **QM/Position:**
  Gesamtfläche der Position.
- **Gewicht/Position:**
  Gesamtgewicht der Position.
- **Bearb.:**
  Bearbeitungen. Wenn im Register Selektion die Auflösungstiefe auf Positionsebene gewählt wurde, wird hier mit einem x gekennzeichnet, wenn in der Position Bearbeitungen enthalten sind.
- **AV-Bereich:**
  Name des AV-Bereichs, dem der Auftrag zugeordnet ist.
- **Bearbeitungen:**
  Nummer der Produktgruppe der einzelnen Bearbeitungen. Die Nummern sind durch ein Semikolon (;) getrennt.
- **Teillieferung:**
  Auftragsnummer der Teillieferung.
- **Haupt-Auftrag:**
  Nummer des Auftrags, zu dem der angezeigte Auftrag eine Teillieferung darstellt.
- **Dokumententyp:**
  Ein Dokumententyp wird nur angezeigt, wenn er vom Auftrag abweicht, z. B. Reklamation.
- **Summe:**
  Gesamtsumme der aufgelisteten Lieferungen für Menge, Fläche und Gewicht.

**Gesamt**
Anzeige der Summen über alle Aufträge, die in der Übersicht angezeigt werden.

**Beispiel: Gedruckte Tourenliste**
[Image: Abb. E-101 Tourenliste als Bildschirmausgabe]

## Versanddaten ändern

**Navigation:** Fertigung > Lieferwesen > Tourenliste > Menü Funktionen > Gruppe Tour > Versanddaten ändern

[Image: Abb. E-102 Versanddaten ändern]

In diesem Dialog können Sie die Tour, den Liefertermin, die Lieferbedingungen von Aufträgen, den Fahrer und/oder den LKW der Tour ändern. Im Dialog werden alle Aufträge angezeigt, die Sie im Dialog Tourenliste – Tabelle markiert haben.

### Markierte Aufträge

In der Übersicht werden alle Aufträge angezeigt, die Sie im Dialog Tourenliste - Tabelle markiert haben.

### Änderung von

Änderungen gelten immer für alle angezeigten Aufträge. Mit der Wahl der Option legen Sie fest, was geändert werden soll:

**Liefertermin** Sie können ein anderes Datum aus der Liste eintragen.

**Tour** Sie können eine andere Tour aus der Liste auswählen.
☐ Die Tour wird nicht geändert.
☑ Die ausgewählte Tour wird für die Aufträge übernommen.

**Lieferbed.** Sie können eine andere Lieferbedingung aus der Liste auswählen.
☐ Die Lieferbedingung wird nicht geändert.
☑ Die ausgewählte Lieferbedingung wird für die Aufträge übernommen.

**Fahrer** Sie können einen anderen Fahrer aus der Liste auswählen.
☐ Der Fahrer wird nicht geändert.
☑ Der ausgewählte Fahrer wird für die Aufträge übernommen.

**LKW** Sie können einen anderen LKW aus der Liste auswählen.
☐ Der LKW wird nicht geändert.
☑ Der ausgewählte LKW wird für die Aufträge übernommen.

## Einstellungen (KAPS-Datei)

**Navigation:** Fertigung > Lieferwesen > Tourenliste > Menü Funktionen > Gruppe KAPS > Pfad für Datei

[Image: Abb. E-103 Einstellungen KAPS-Datei]

In diesem Dialog können Sie den Pfad und den Dateinamen für die KAPS-Datei festlegen. Dies ist eine Datei für die KAPS-Turbosoft-Schnittstelle. Die Ausgabe bezieht sich immer auf den aktuellen Nummernverwalter.

### KAPS-Datei

**Pfad** In diesem Feld geben Sie den Pfad und Ordner an, in dem die KAPS-Datei gespeichert werden soll.

**Dateiname ... +Tag+Monat+_Lfd.Nr.** In diesem Feld geben Sie eine Kennzeichnung für die KAPS-Datei an. Sie können 2 Zeichen eintragen. Der Dateiname wird um das Datum und eine laufende Nummer erweitert.

**Endung (ohne Punkt!)** In diesem Feld geben Sie die Datei-Endung für die KAPS-Datei an.

## Statusmeldung

Wenn Sie nicht mit Rückmeldungen aus der Betriebsdatenerfassung (BDE) arbeiten, können Sie über den Dialog Statusmeldung und Packmittelzuordnung Aufträge einscannen und den Status umsetzen.

Mit dem Tastatur-Scanner kann einem Auftrag ein neuer Status zugewiesen und das notwendige Packmittel zugeordnet werden. Die benötigten Barcodes können Sie dazu selber herstellen.
⇨ Tutorial, "Scan-Vorlage herstellen" auf Seite E-103

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menüs im Dialog Statusmeldung" auf Seite E-218
- "Statusmeldung und Packmittelzuordnung" auf Seite E-220
- "Auswahl Gestell" auf Seite E-226

### Menüs im Dialog Statusmeldung

**Navigation:** Fertigung > Lieferwesen > Statusmeldung

Über die Menüs können Sie die Standardeinstellung des Dialoges bestimmen, Funktionen starten und andere Dialoge öffnen, ohne den Dialog zu schließen.
- "Menü Funktionen" auf Seite E-218
- "Menü Optionen" auf Seite E-219

### Menü Funktionen

**Navigation:** Fertigung > Lieferwesen > Statusmeldung

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Dokumentenverwaltung zu schließen. Folgende Einträge werden angezeigt:

Das Menü ist in folgende Gruppen gegliedert:
- "Gruppe Packmittel" auf Seite E-212
- "Gruppe Funktionen" auf Seite E-213

#### Gruppe Packmittel

Die Einträge sind nur im Register Manuelle Packmittelzuordnung freigeschaltet.
- **Hinzufügen:**
  Ordnet einem markierten Auftrag ein anderes Packmittel zu.
- **Löschen:**
  Löscht die Zuordnung.

#### Gruppe Funktionen
- **Alles markieren:**
  Der Eintrag ist nur im Register Manuelle Packmittelzuordnung freigeschaltet. Sie können damit alle Aufträge in der Liste markieren.
- **Einstellungen:**
  Öffnet den Dialog Optionen, um festzulegen, welche Statusänderungen erlaubt sind.
  ⇨ "Optionen in Statusmeldung" auf Seite E-225

### Menü Optionen

**Navigation:** Fertigung > Lieferwesen > Statusmeldung

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen.

Das Menü ist in folgende Gruppen gegliedert:
- "Gruppe Gestelltyp" auf Seite E-213
- "Gruppe Datum" auf Seite E-213
- "Gruppe Produktion" auf Seite E-213

#### Gruppe Gestelltyp
- **Eingabe Gestelltyp:**
  Mit dieser Einstellung springt der Fokus bei der Gestellzuordnung im Register Manuelle Packmittelzuordnung auf das Feld Packmittel statt auf das Feld für die Gestellnummer.
- **Ausgabe verfügbarer Gestelle:**
  Die Anzeige wird auf die Gestelle eingeschränkt, die verfügbar sind.

#### Gruppe Datum
- **Produktionsdatum vorgeben:**
  Schaltet das Feld Produktionsendedatum frei, um das Datum während dieser Sitzung manuell vorzugeben.
- **Anlieferdatum vorgeben:**
  Schaltet das Feld Anlieferdatum frei, um das Datum während dieser Sitzung manuell vorzugeben.

#### Gruppe Produktion
- **Prod.freigabe Auftrag, falls Subauftrag produziert:**
  Aufträge werden zur Produktion freigegeben, wenn der durch sie notwendige interne Auftrag fertig gemeldet wurde.

## Statusmeldung und Packmittelzuordnung

**Navigation:** Fertigung > Lieferwesen > Statusmeldung

**Zu Dialogbeschreibung:**
⇨ "Optionen in Statusmeldung" auf Seite E-219

Mit einem Tastatur-Scanner können Sie den Auftragsstatus manuell umsetzen. Den fertigen Aufträgen können Packmittel zugeordnet werden. Diese Zuordnungen können als Listen für den Versand gedruckt werden.
⇨ "Listendruck" auf Seite E-235

In diesem Dialog finden Sie folgende Register:
- "Statusmeldung - Auftrag" auf Seite E-220
- "Statusmeldung – Position" auf Seite E-222
- "Statusmeldung – Manuelle Packmittelzuordnung" auf Seite E-224

### Statusmeldung – Auftrag

**Navigation:** Fertigung > Lieferwesen > Statusmeldung > Register Statusmeldung – Auftrag

[Image: Abb. E-104 Statusmeldung – Auftrag]

In diesem Register können Sie den Auftragsstatus umsetzen, um den Auftrag für den Versand fertig zu machen.
⇨ Tutorial, "Manuelle Statusumsetzung" auf Seite E-97

#### Reihenfolge der Eingaben beachten

> Tragen Sie zuerst alle Vorgaben ein, die für diese Sitzung gelten sollen. Beginnen Sie beim Scannen dann mit dem Status und lesen Sie erst danach den Auftrag ein. Lesen die dazu die Handlungsbeschreibungen im Tutorial.

#### Zuordnung

**Auftrag/Statuspunkt** In dieses Feld stellen Sie den Cursor, bevor Sie den Auftrag oder den Status scannen. Sie können den Auftrag oder den Status manuell eingeben. Dazu tragen Sie ein S (Status) oder ein O (Order) ein und ergänzen die Status- oder Auftragsnummer. Nach dem Einlesen des Auftrags wird der Status automatisch umgesetzt.

#### Vorgabe

**Produktionsende** Dieses Feld ist nur freigeschaltet, wenn Sie im Menü Einstellungen die Option Produktionsdatum vorgeben aktiviert haben. Sie können vor dem Einlesen eines Auftrags ein neues Datum eingeben, an dem die Produktion abgeschlossen sein wird. Das neue Datum wird nicht in den Auftrag zurückgeschrieben.

**Anlieferdatum** Dieses Feld ist nur freigeschaltet, wenn Sie im Menü Einstellungen die Option Anlieferdatum vorgeben aktiviert haben. Sie können vor dem Einlesen eines Auftrags ein neues Lieferdatum eingeben, z. B., wenn sich der Produktionstermin verschoben hat. Das neue Datum wird in den Auftrag zurückgeschrieben.

#### Zielnummernverwalter

**(Zielnummernverwalter)** Sie können vor dem Einlesen einen Nummernverwalter auswählen oder einen Namen eintragen, um die eingelesenen Aufträge in diesen Nummernverwalter zu stellen. Dies ist sinnvoll, wenn Sie anschließend z. B. Versandpapiere drucken wollen. Das Feld wird freigeschaltet, wenn die Checkbox In NV kopieren markiert ist.

**In NV kopieren** Wenn die Checkbox In NV kopieren markiert ist, wird das Feld Zielnummernverwalter freigeschaltet, um einen Nummernverwalter einzutragen.
Damit der im Feld Zielnummernverwalter eingetragene Nummernverwalter gefüllt wird, muss die Checkbox In NV kopieren aktiviert sein.
☐ Die eingelesenen Aufträge werden nicht in den Nummernverwalter kopiert.
☑ Die eingelesenen Aufträge werden automatisch in den gewählten Nummernverwalter kopiert.

#### Übersicht

Der Status der Aufträge wird beim Einlesen umgesetzt. Alle während einer Sitzung eingelesenen Aufträge werden in der Übersicht angezeigt.
- **Nummer:** Nummer des eingelesenen Auftrags.
- **Kunde/Lieferant:** Nummer des Kunden.
- **Name:** Name des Kunden.
- **Status:** Neuer Auftragsstatus.
- **Datum Erfass.:** Datum, an dem der Auftrag erfasst wurde.
- **Datum AB:** Datum der Auftragsbestätigung.
- **Datum Lieferung:** Lieferdatum aus dem Auftrag oder geändertes Datum aus dem Feld Anlieferdatum.
- **Anz. Positionen:** Anzahl der Auftragspositionen.

### Statusmeldung – Position

**Navigation:** Fertigung > Lieferwesen > Statusmeldung > Register Statusmeldung – Position

[Image: Abb. E-105 Statusmeldung – Position]

In diesem Register können Sie den Status für einzelne Auftragspositionen umsetzen. Der Auftragsstatus wird erst umgesetzt, wenn alle Auftragspositionen denselben Status haben. Den einzelnen Positionen können keine Packmittel zugeordnet werden.

Die Felder in den Bereichen Zuordnung, Vorgabe und Zielnummernverwalter sind ausführlich zum Register Statusmeldung – Auftrag beschrieben.
⇨ "Statusmeldung - Auftrag" auf Seite E-220

#### Positionsübersicht

**Aktueller Auftrag** In diesem Feld wird die Auftragsnummer angezeigt, zu der die Positionen aufgelistet sind.

In der Übersicht sind alle Positionen des aktuellen Auftrags aufgeführt:
- **Pos:** Nummer der Auftragsposition.
- **Status:** Status der Auftragsposition. Er kann sich von dem der anderen Positionen unterscheiden.
- **Menge:** Stückzahl der Position.
- **Breite, Höhe:** Maße der Position.
- **Bezeichnung:** Bezeichnung des Glases.

### Statusmeldung – Manuelle Packmittelzuordnung

**Navigation:** Fertigung > Lieferwesen > Statusmeldung > Register Manuelle Packmittelzuordnung

[Image: Abb. E-106 Statusmeldung – Manuelle Packmittelzuordnung]

In diesem Register können Sie den Positionen eines Auftrags Packmittel (Gestelle und deren Gestellnummern) zuordnen. Gestelle können wahlweise per Scanner oder manuell zugeordnet werden.

#### Zuordnung

**Packmittel** In der Kombobox werden alle Packmittel angeboten, die im System hinterlegt sind. Das können Gestellarten, Kisten, Container usw. sein.

**[Ordner]** Mit dieser Schaltfläche öffnen Sie den Dialog Auswahl Gestell, um eine freie Gestellnummer aus der gewählten Gestellart zu suchen.
⇨ "Auswahl Gestell" auf Seite E-226

## Optionen in Statusmeldung

**Navigation:** Fertigung > Lieferwesen > Statusmeldung > Menü Funktionen > Gruppe Funktionen > Einstellungen

[Image: Abb. E-107 Optionen in Statusmeldung]

In diesem Dialog stellen Sie ein, welche Statuspunkte geändert werden können. Die Einstellungen können so eingerichtet werden, dass sie nur für den jeweils angemeldeten Mitarbeiter gelten.

> **Administratorrechte erforderlich**
> Die Optionen im Dialog Statusmeldung kann nur der Systemadministrator ändern.

**Verfügbare Statuspunkte** In der Liste sind alle Statuspunkte aufgeführt, die in den Stammdaten eingerichtet wurden.

**Änderbare Statuspunkte** In der Liste werden alle Statuspunkte aufgeführt, die als neuer Status gewählt werden dürfen.

**Statusverminderung erlauben** Standardmäßig wird der Status mit der Statusmeldung hochgesetzt. In einzelnen Fällen kann es jedoch notwendig sein, den Status zurückzusetzen, z. B., wenn ein Auftrag versehentlich als fertig gebucht wurde.
☐ Der Status eines Auftrags oder einer Position kann nicht zurückgesetzt werden. Wenn Sie dennoch einen Fehler korrigieren müssen, kann der Status des einzelnen Auftrags in der Dokumentenverwaltung zurückgesetzt werden.
⇨ Verkauf, "Menü Funktionen" auf Seite C-406
☑ Der Status kann zurückgesetzt werden. Die Checkbox Meldung bei erreichtem Sperrstatus wird freigeschaltet.

**Meldung bei erreichtem Sperrstatus** Sie können festlegen, ob bei einer Statusverminderung eine Meldung ausgeben wird.
Diese Checkbox ist nur freigeschaltet, wenn die Checkbox Statusverminderung erlaubt aktiviert ist.
☐ Es wird keine Meldung ausgegeben.
☑ Wenn bei einer Statusverminderung der Sperrstatus höher ist, als der Auftragsstatus, wird eine Meldung ausgegeben. Sie können dann entscheiden, ob Sie den Status ändern wollen.

**Keine Laufnr., dann 9999 eintragen** Standardmäßig wird eine Laufnummer vom System vergeben, wenn ein Produktionslauf angelegt wird. Mit dieser Option legen Sie fest, ob Läufen ohne eigene Laufnummer eine Laufnummer zugeordnet wird.
Diese Checkbox ist nur freigeschaltet, wenn ein Eintrag im Feld änderbare Statuspunkte markiert ist.
☐ Für den Lauf wird keine Laufnummer vergeben.
☑ Die Laufnummer 9999 wird vergeben, wenn keine eigene Laufnummer vorhanden ist.

## Auswahl Gestell

**Navigation:** Fertigung > Lieferwesen > Statusmeldung > Register Manuelle Packmittelzuordnung > [Ordner]

[Image: Abb. E-108 Manuelle Packmittelzuordnung – Gestell auswählen]

Wenn Sie nicht mit einem Tastatur-Scanner arbeiten, können Sie in diesem Dialog ein freies Gestell auswählen, um es dem aktuellen Auftrag zuzuordnen.

### Filter

**Gestellart** In der Kombobox werden alle Gestellarten zur Auswahl angeboten, die in den Stammdaten angelegt sind.

**Gestellnummer von, bis** Sie können die Anzeige von Gestellen auf eine Folge von Gestellnummern eingrenzen.
Die Gestellnummern werden im Dialog Gestelle hinterlegt.
⇨ "Gestelle" auf Seite E-242

**Nicht verfügbare Gestelle** Wenn Gestelle außer Haus gemeldet sind, können sie nicht nochmals belegt werden. Sie können die Anzeige dieser Gestellnummern ausschließen.
☐ Nur die Gestelle werden angezeigt, die für den aktuellen Auftrag verwendet werden können.
☑ Alle Gestelle werden angezeigt.

### Übersicht

In der Übersicht werden alle Gestelle angezeigt, die den Suchkriterien entsprechen.
- **Gestellnummer:**
  Gestellnummer, die in den Stammdaten hinterlegt wurde.
- **Bezeichnung:**
  Bezeichnung, die in den Stammdaten hinterlegt wurde.
- **Gestellart:**
  Wenn Sie die Suche nicht auf eine bestimmte Gestellart eingegrenzt haben, dient die Anzeige der Gestellart zur weiteren Differenzierung.
- **Ausgegeben:**
  Anzeige, ob das Gestell aktuell verwendet wird.
- **Ausgabedatum:**
  Ein Ausgabedatum wird nur angezeigt, wenn die Gestellnummer einem Auftrag zugeordnet ist. Wenn das Gestell wieder als frei gebucht wurde, bleibt das Feld leer.

## Kommissionierung

**Navigation:** Fertigung > Lieferwesen > Kommissionierung

Mit der Kommissionierung planen Sie die Beladung Ihrer Fahrzeuge.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menüs im Dialog Kommissionierung" auf Seite E-228
- "Kommissionierung" auf Seite E-230
- "Gestelltransfer" auf Seite E-233
- "Export Optionen" auf Seite E-234

### Menüs im Dialog Kommissionierung

**Navigation:** Fertigung > Lieferwesen > Kommissionierung

Über die Menüs können Sie die Standardeinstellung des Dialoges bestimmen, Funktionen starten und andere Dialoge öffnen, ohne den Dialog zu schließen.
- "Menü Funktionen" auf Seite E-228
- "Menü Optionen" auf Seite E-229

### Menü Funktionen

**Navigation:** Fertigung > Lieferwesen > Kommissionierung

Über dieses Menü können Sie verschiedene Funktionen ausführen, ohne die Kommissionierung zu schließen.

Das Menü ist in folgende Gruppen gegliedert:
- "Gruppe Dokument" auf Seite E-222
- "Gruppe Position" auf Seite E-222
- "Gruppe Packmittelgruppen" auf Seite E-223
- "Gruppe Gestellzuordnung" auf Seite E-223

#### Gruppe Dokument
- **Historie:**
  Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des markierten Dokuments. Der Dialog ist ausführlich im Part Verkauf beschrieben.
  ⇨ Verkauf, "Historie" auf Seite C-564
- **Alles markieren:**
  Markiert alle Aufträge in der Übersicht.

#### Gruppe Position
- **Initialisierung:**
  Öffnet den Dialog Export-Optionen, in dem Sie die Zuordnung von Gestellnummern umorganisieren können.
  ⇨ "Export Optionen" auf Seite E-234
- **Auf Position vererben:**
  Überträgt die Packmittelgruppe auf alle Positionen des Auftrags.

#### Gruppe Packmittelgruppen
- **Packmittelgruppen:**
  Öffnet den Dialog Packmittelgruppen, um eine neue Packmittelgruppe zu vergeben. Diese Funktion wird in der Regel nur in älteren Installation der Software genutzt.

#### Gruppe Gestellzuordnung
- **Gestellzuordnung:**
  Öffnet den Dialog Statusmeldung – Manuelle Packmittelzuordnung, um Gestelle zuordnen.
  ⇨ "Statusmeldung - Manuelle Packmittelzuordnung" auf Seite E-224

### Menü Optionen

**Navigation:** Fertigung > Lieferwesen > Kommissionierung

#### Gruppe Optionen
- **Eingabe von einzelnen Auftragsnummern:**
  Nur dieser Auftrag wird in der Tabelle selektiert.
  Das Standardverhalten, dass die eingegebenen Auftragsnummern zusätzlich zu den bereits Selektierten für eine Änderung markiert werden, bleibt bestehen, wenn die Option nicht gesetzt ist.

## Kommissionierung

**Navigation:** Fertigung > Lieferwesen > Kommissionierung

[Image: Abb. E-109 Kommissionierung]

In diesem Dialog können Sie den Versand mit Ihrem eigenen Fuhrpark organisieren. Sie können die Tour, den Lkw und das Lieferdatum für einzelne oder mehrere Aufträge gleichzeitig ändern. Sie können sich das Ergebnis der Kommissionierung nach dem Speichern am Bildschirm anzeigen und/oder drucken lassen.

Wenn Sie mit Spediteuren arbeiten, können Sie den Versand über den Dialog Versand organisieren.
⇨ "Versand (Spedition)" auf Seite E-292

> **Anzeige der Aufträge**
> Bevor Sie sich die Aufträge anzeigen lassen, können Sie über Lieferwesen > Nummernverwalter einen Nummernverwalter aktivieren. Die in ihm enthaltenen Aufträge werden aufgelistet. Sie können Aufträge aber auch einzeln auswählen und in den gewünschten Nummernverwalter stellen.

### Auftrag

**Nummer** Sie können eine Auftragsnummer eingeben oder den Auftrag über die Suche auswählen. Der Auftrag wird mit [OK] übernommen und im Bereich Aufträge aufgelistet.

**In NV übernehmen** Sie können die bearbeiteten Aufträge automatisch in einen anderen Nummernverwalter stellen.
☐ Die Aufträge werden nicht in einen (anderen) Nummernverwalter gestellt.
☑ Das Feld Name (Nummernverwalter) wird freigeschaltet. Die Aufträge werden in den gewählten Nummernverwalter gestellt. Wenn in dem Nummernverwalter bereits Aufträge enthalten sind, werden diese im Bereich Aufträge angezeigt.

**Name (Nummernverwalter)** Das Feld ist nur freigeschaltet, wenn die Checkbox in NV übernehmen aktiviert ist. Sie können den Nummernverwalter auswählen, in den die bearbeiteten Aufträge gestellt werden sollen.

### Eingabe

**Tour** Sie können jedem im Feld Aufträge markierten Auftrag eine andere Tour zuweisen. Die Änderungen werden in den Auftrag und ggf. in die Ausgangsbuchung des Gestells zurückgeschrieben.

**Lieferbedingung** Sie können jedem im Feld Aufträge markierten Auftrag eine andere Lieferbedingung zuweisen.
Die Lieferbedingungen sind unter Stammdaten > Versand definiert.
⇨ Stammdaten, "Lieferbedingungen" auf Seite B-872

**Anlieferung** Sie können für jeden im Feld Aufträge markierten Auftrag einen neuen Liefertermin angeben. Die Änderungen werden in die Aufträge zurückgeschrieben.

**Lkw** Sie können jedem im Feld Aufträge markierten Auftrag einem Lkw zuweisen, indem Sie die Nummer (ID) eingeben oder ihn über die Kombobox auswählen.
Die Fahrzeuge sind unter Stammdaten > Versand definiert.
⇨ Stammdaten, "Lkw" auf Seite B-876

**Fahrer** Sie können jedem im Feld Aufträge markierten Auftrag einen Fahrer zuweisen.
Die Fahrer sind unter Stammdaten > Versand definiert.
⇨ Stammdaten, "Fahrer" auf Seite B-877

**Status** Sie können jedem im Feld Aufträge markierten Auftrag einen anderen Status zuweisen.
⇨ "Optionen in Statusmeldung" auf Seite E-225

### Aufträge

Alle ausgewählten Aufträge werden in der Übersicht angezeigt. Um die Daten einer Auslieferung zu ändern, müssen Sie den entsprechenden Auftrag markieren. Die Mehrfachauswahl ist mit den Tasten <Strg> oder <Shift> möglich.
- **Nummer, Status:** Nummer und Status des Auftrags.
- **Tour, Lieferbedingung:** Nummer der zugewiesenen Tour und Lieferbedingung, z. B. Lkw, Spedition.
- **Lieferdatum:** Datum der Lieferung.
- **Kundennummer, Name:** Nummer und Name des Kunden.
- **Abw. Straße, Abw. PLZ, Abw. Ort:** Eine abweichende Lieferanschrift wird nur dargestellt, wenn diese im Auftrag angegeben ist.
- **Menge:** Gesamtmenge aller Positionen des Auftrags.
- **Gewicht:** Gesamtgewicht aller Positionen des Auftrags.
- **LKW, Fahrer:** Nummer des LKW und Name des Fahrers.

### Positionen

> **Keine Verwaltung von einzelnen Positionen**
> Sie können in diesem Dialog nur gesamte Aufträge verwalten, die fertig gemeldet sind. Wenn nur einzelne Positionen fertiggemeldet sind, müssen Sie einen Teillieferungsauftrag für den Versand fertigmachen. Diese Funktion ist ausführlich im Part Verkauf beschrieben.
> ⇨ Verkauf, "Teillieferung zu einem Auftrag" auf Seite C-263

In der Übersicht werden alle Positionen des Auftrags angezeigt, der in der Auftragsübersicht markiert ist. Wenn mehrere Aufträge markiert sind, werden keine Positionen angezeigt.
- **Pos.:** Nummer der Auftragsposition.
- **Bezeichnung:** Name des Produkts.
- **Gestell:** Nummer des Gestells.
- **Gestelltyp:** In diesem Feld können Sie den passenden Gestelltyp auswählen. Wenn Sie den Cursor in das Feld setzen, wird die Schaltfläche zum Öffnen der Kombobox angezeigt.
- **Packmittelgruppe:** Sie können eine Packmittelgruppe eintragen.
- **Menge:** Stückzahl der Auftragsposition.

### Summen selektierter LKW

**Menge, Gewicht** Anzeige von Gesamtmenge und Gesamtgewicht für den Lkw, der für diese Tour an diesem Termin fährt.
Die Werte werden in roter Schrift dargestellt, wenn das Gewicht höher ist, als für den Lkw zulässig.

**Maximalgewicht** Gewicht, das der zugewiesene Lkw laden kann.

### Summen selektierte Aufträge

**Menge, Gewicht** Anzeige von Menge und Gewicht der markierten Aufträge.

## Gestelltransfer

**Navigation:** Fertigung > Lieferwesen > Kommissionierung > Menü Funktionen > Gruppe Position > Initialisierung

[Image: Abb. E-110 Kommissionierung – Gestelltransfer]

In diesem Dialog können Sie die Gestellverwaltung reorganisieren. Diese Funktion dürfen Sie nur nach Absprache mit der A+W Software GmbH ausführen.

## Export Optionen

**Navigation:** Fertigung > Lieferwesen > Kommissionierung > Tabelleneigenschaften > Export > Optionen

[Image: Abb. E-111 Export]

Mit dieser Funktion können Sie die Gestellzuordnung aus einer alten Datenbanktabelle in die neuen Felder übertragen. Wenn Sie Ihre Gestellzuordnung umorganisieren wollen, setzen Sie sich bitte mit dem Support der A+W Software GmbH in Verbindung.

## Listendruck

**Navigation:** Fertigung > Lieferwesen > Listendruck

[Image: Abb. E-112 Listendruck]

In diesem Dialog können Sie verschiedene Listen nach der Kommissionierung ausdrucken oder auf dem Monitor anzeigen lassen.

### Nummernverwalter

**(Nummernverwalter)** In diesem Feld wählen Sie den Nummernverwalter aus, in dem die Aufträge gesammelt sind, zu denen Sie die Liste drucken wollen.

**[Gestellausgabe]** Mit dieser Schaltfläche öffnen Sie den Dialog Gestellausgabe, in dem Sie die Gestellbelegung prüfen können.
⇨ "Gestellausgabe" auf Seite E-238

### Übersicht

In der Übersicht werden alle Aufträge angezeigt, die im ausgewählten Nummernverwalter stehen.
- **Nummer:** Nummer des Auftrags.
- **Kunde/Lieferant, Name:** Nummer und Name des Kunden.
- **Status:** Auftragsstatus.
- **Datum Erfass.:** Datum, an dem der Auftrag erfasst wurde.
- **Datum AB:** Datum der Auftragsbestätigung.
- **Datum Lieferung:** Lieferdatum aus dem Auftrag.
- **Lieferschein:** Nummer des Lieferscheins.

### Druckeinstellungen

Mit der Wahl der Option legen Sie fest, in welche Liste das Ergebnis der Kommissionierung gedruckt werden soll:
- **Transportmittelbeladungsliste:**
  In dieser Liste wird angezeigt, welche Gestelle auf dem Lkw stehen (sollen).
- **Empfangsbestätigungsliste:**
  In dieser Liste werden pro Auftrag Details zu den Positionen angezeigt, deren Empfang sich der Fahrer bestätigen lassen muss.
- **Gestellliste (auswärtig):**
  In dieser Liste werden pro Tour alle Gestelle aufgeführt, die derzeit außer Haus sind.

> **Seitenwechsel**
> Bei den beiden ersten Listen wird jeweils ein Seitenwechsel eingefügt, wenn sich der Lkw, die Tour und/oder der Liefertermin ändern.

### Beispiele:

[Image: Abb. E-113 Transportmittelbeladungsliste]
[Image: Abb. E-114 Empfangsbestätigungsliste]

## Gestellausgabe

**Navigation:** Fertigung > Lieferwesen > Listendruck > [Gestellausgabe]

[Image: Abb. E-115 Gestellausgabe]

In diesem Dialog können Sie die Gestellbelegung analysieren. Dabei wird geprüft, ob auf einem Gestell nur Aufträge eines Kunden sind.
Mit [OK] werden die Gestelle aus der Gestellverwaltung ausgebucht bzw. als auswärtig verbucht. Danach können Sie die Gestellbelegungsliste drucken.

### Tabelle

In der Übersicht werden alle auswärtigen Gestelle aufgelistet.
- **Gestellnr.:** Nummer des auswärtigen Gestells.
- **Gestellart:** Gestellart des auswärtigen Gestells.
- **Auftrag/Kunde:** Auftragsnummer und Kunde, bei dem das Gestell steht.
- **Auftrag:** Auftrag, der mit dem das Gestell ausgeliefert wurde.
- **Latten, Räder, Wagen:** Zubehör des auswärtigen Gestells.

### Optionen

**Keine Gestellausgabe für Positionen mit Menge 0** Sie können die Zuweisung zu Positionen ohne Menge unterdrücken.
☐ Allen Positionen werden Gestelle zugewiesen.
☑ Positionen ohne Menge wird kein Gestell zugeordnet.

## Warenausgang Kisten

**Navigation:** Fertigung > Lieferwesen > Warenausgang Kisten

Der Dialog Warenausgang Kiste ist im Part Einkauf beschrieben:
⇨ Einkauf, "Wareneingang - Identnummer" auf Seite D-237

### Warenausgang

**Navigation:** Fertigung > Lieferwesen > Warenausgang Kisten > Register Identnummern

[Image: Abb. E-116 Warenausgang von Kisten – Kiste ausbuchen]

In diesem Register können Sie eine Kiste reservieren oder aus dem Lagerbestand ausbuchen. Sie können nur Kisten reservieren, die beim Lagereingang mit einer Kisten-ID erfasst wurden.
⇨ Tutorial, "Warenausgang Kisten" auf Seite E-148

# Gestelle

## Gestelle

**Navigation:** Fertigung > Gestellverwaltung > Gestelle

Über den Dialog Gestelle können Sie die Verwendung der Gestelle überwachen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menüs im Dialog Gestelle" auf Seite E-240
- "Gestelle" auf Seite E-242

Über den Dialog Gestelle können Sie außerdem folgende Dialog öffnen.
- "Gestellübersicht" auf Seite E-258
- "Übersicht Partner" auf Seite E-259
- "Mahnstatus zurücksetzen" auf Seite E-261
- "Gestell umbuchen" auf Seite E-260

### Menüs im Dialog Gestelle

**Navigation:** Fertigung > Gestellverwaltung > Gestelle

Über die Menüs der Gestellverwaltung können Sie die Standardeinstellung des Dialoges bestimmen und andere Dialoge öffnen, ohne die Gestellverwaltung zu schließen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Optionen” auf Seite E-240
- "Menü Funktionen" auf Seite E-241

### Menü Optionen

**Navigation:** Fertigung > Gestellverwaltung > Gestelle > Menü Optionen

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

Das Menü ist in folgende Gruppen gegliedert:
- "Gruppe Gestelle" auf Seite E-234
- "Gruppe Ausgabe" auf Seite E-235
- "Gruppe Mahnstufen" auf Seite E-235

#### Gruppe Gestelle
- **Erweiterte Gestellsuche:**
  Mit dieser Option können Sie die Suche auch mit Teilen der Gestellnummer durchführen. Wenn Sie z. B. im Feld Nummer eine 5 eingeben, werden alle Gestelle gesucht, in deren Gestellnummer eine 5 vorkommt.
- **Ausgabe verfügbarer Gestelle:**
  Die Anzeige wird auf verfügbare Gestelle eingeschränkt. Die Option ist nur im Register Ausgang freigeschaltet.
- **Ausgabe an gesperrte Kunden:**
  Gestelle können keinem Kunden zugeordnet werden, der gesperrt ist. Die Option ist nur im Register Ausgang freigeschaltet.
- **Auswärtige Gestelle mit Ausgabeinfos:**
  Beim Druck einer Liste aller auswärtigen Gestelle werden zusätzlich der Name der Tour und des Kunden angegeben.
- **Faxnummer im Druckjobname:**
  Angabe der Faxnummer, wenn Sie den Druck über einen Druckjob steuern.
- **Gestellbelegung in Historiendruck:**
  Die Belegung der Gestelle aus der Historientabelle wird beim Historiendruck mitgedruckt.

#### Gruppe Mahnstufen
- **Verwendung von Mahnstufen:**
  Die Option ist nur im Register Mahnung freigeschaltet.
- **Neue Seite bei Wechsel der Mahnstufe:**
  Beim Druck der angemahnten Gestelle/Kunden wird jeweils ein Seitenvorschub geschaltet, wenn eine andere Mahnstufe beginnt. Die Option ist nur im Register Mahnung freigeschaltet.

### Menü Funktionen

**Navigation:** Fertigung > Gestellverwaltung > Gestelle > Menü Funktionen

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Gestellverwaltung zu schließen.

Das Menü ist in folgende Gruppen gegliedert:
- "Gruppe Ausführen" auf Seite E-235

#### Gruppe Ausführen
- **Gestell umbuchen:**
  Öffnet den Dialog Gestelle umbuchen, in dem Sie ein Gestell auf einen anderen Partner umbuchen können.
  ⇨"Gestell umbuchen" auf Seite E-260
- **Ausgang ändern:**
  Schaltet die Felder für Änderungen frei.
- **Mahnstatus zurücksetzen:**
  Öffnet den Dialog Mahnstatus zurücksetzen, in dem Sie den Mahnstatus zurücksetzen können.
  ⇨ "Mahnstatus zurücksetzen" auf Seite E-261
- **Gestellhistoriendetails initialisieren:**
  Alle vorhandenen Historiensätze der Gestellbelegung werden gelöscht und die aktuelle Belegung der Gestelle wird eingetragen.
  Diese Funktion sollte nur ausgeführt werden, bevor Sie A+W Business in Betrieb nehmen.
- **Barcodes für Gestelle drucken:**
  Öffnet den Dialog Druck – Gestell Barcodes, in dem Sie Barcodes für Gestelle drucken können.
- **Gestellbelegung:**
  Öffnet den Dialog Gestellbelegung, in dem Sie den Gestellen Auftragspositionen zuordnen können.
  ⇨ "Gestellbelegung" auf Seite E-261

## Gestelle

**Navigation:** Fertigung > Gestellverwaltung > Gestelle

In diesem Dialog können Sie Gestelle anlegen und deren Ein- und Ausgang buchen. Für säumige Rückgabe können Sie Mahnungen erstellen.

In diesem Dialog finden Sie folgende Register:
- "Gestellverwaltung – Gestelle" auf Seite E-243
- "Gestellverwaltung - Ausgang" auf Seite E-246
- "Gestellverwaltung – Eingang" auf Seite E-249
- "Gestellverwaltung – Historie" auf Seite E-250
- "Gestellverwaltung – Mahnung" auf Seite E-252

**Zu Dialogbeschreibung:**
- Gestellübersicht
- Übersicht Partner
- Gestell umbuchen
- Mahnstatus zurücksetzen
- Gestellbelegung

### Gestellverwaltung – Gestelle

**Navigation:** Fertigung > Gestellverwaltung > Gestelle > Register Gestelle

[Image: Abb. E-117 Gestellverwaltung – Gestelle]

In diesem Register können Sie neue Gestelle hinzufügen oder die Daten der Gestelle bearbeiten.

#### Gestelldaten

**Nummer** Beim Anlegen kann die Gestellnummer alphanumerisch eingegeben werden. Jede Nummer darf nur einmal verwendet werden. Sie können sich die freien Nummern anzeigen lassen, indem Sie auf die Schaltfläche [Ordner] klicken.
⇨ "Gestellübersicht" auf Seite E-258

**Art** Sie können nur die Gestellarten zuordnen, die im Dialog Gestellarten angelegt sind.

**Bezeichnung** Sie können eine alphanumerische Bezeichnung für das Gestell eintragen, z. B. einen Typnamen. Diese Bezeichnung kann auf den Listen gedruckt werden.

**Bemerkung** Sie können eine Bemerkung zum Gestell eintragen, z. B. bei Kundengestellen den Namen des Kunden.

**Latten/Räder/Wagen** Sie können angeben, wie viele Latten, Räder oder Wagen das Gestell hat.

**Mietsatz/Tage frei** Wenn Sie für Ihre Gestelle eine Miete berechnen, können Sie hier den Tagessatz und die Anzahl der Tage eingeben, die das Gestell kostenlos zur Verfügung steht.

**Änderung** Name des letzten Bearbeiters und Datum der letzten Bearbeitung.

#### Eigenschaften

Mit der Wahl der Eigenschaft geben Sie an, ob und wie das Gestell verwendet wird. Mit Kombinationen von Suchkriterien können Sie die Suche weiter einschränken. Bitte beachten Sie, dass nicht jede Kombination sinnvoll ist.

- **Verfügbar** Als verfügbar gelten alle Gestelle, die nicht belegt und nicht verloren oder gesperrt sind.
  - ☐ Das Gestell ist nicht verfügbar.
  - ☑ Das Gestell ist verfügbar und kann belegt werden.
- **Gesperrt** Ein Gestell kann für die Verwendung gesperrt werden, z. B., weil es zur Reparatur ist.
  - ☐ Das Gestell ist nicht gesperrt. Dies bedeutet jedoch nicht automatisch, dass es verfügbar ist.
  - ☑ Das Gestell ist gesperrt und kann nicht belegt werden.
- **Verloren** Gestelle können auf unterschiedliche Weise abhandenkommen.
  - ☐ Das Gestell ist nicht verloren. Dies bedeutet jedoch nicht automatisch, dass es verfügbar ist.
  - ☑ Das Gestell ist verloren.
- **Stationär** Gestelle können fest an einen Ort in der Produktion gebunden sein.
  - ☐ Das Gestell wird nicht stationär verwendet.
  - ☑ Das Gestell wird stationär verwendet. Es kann nicht für eine Lieferung außer Haus eingesetzt werden.
- **Keine Mahnung** Gestelle können vorübergehend beim Kunden stehen. Wenn Sie Miete berechnen oder nur über eine geringe Anzahl von Gestellen verfügen, können Sie die säumige Rückgabe anmahnen.
  - ☐ Das Gestell soll nicht angemahnt werden, z. B. bei Fremdgestellen.
  - ☑ Das Gestell kann angemahnt werden.
- **Automatisch angelegt** Gestelle können automatisch angelegt werden, wenn ein Barcode gescannt wurde, der im System nicht bekannt ist.
  - ☐ Das Gestell wurde manuell angelegt.
  - ☑ Das Gestell wurde automatisch angelegt.
- **Fremdgestell** Gestelle können von einem Lieferanten oder dem Kunden zur Verfügung gestellt worden sein.
  - ☐ Das Gestell gehört zum Unternehmen.
  - ☑ Das Gestell gehört einem Lieferanten oder Kunden. In diesem Falle wird der Name mit angegeben.

**Auswärtig von ... bis** Das Gestell kann für einen bestimmten Zeitraum außer Haus gebucht werden, z. B., weil es an einen Kunden vermietet wurde.
☐ Das Gestell ist nicht für einen Zeitraum ausgebucht.
☑ Das Gestell ist für einen bestimmten Zeitraum außer Haus. Zusätzlich wird der Zeitraum angegeben.

**Bei Kunde** Der Kunde, an den das Gestell für einen bestimmten Zeitraum verliehen wurde.

**Abw. Adresse** Wenn das vermietete Gestell an einen anderen Standort als die Kundenadresse geliefert wurde, kann der aktuelle Standort eingetragen werden.

**Tour** Das Gestell wurde für eine Tour ausgewählt.

**Gemahnt** Gestelle können vorübergehend beim Kunden stehen. Wenn Sie Miete berechnen oder nur über eine geringe Anzahl von Gestellen verfügen, können Sie die säumige Rückgabe anmahnen.
☐ Das Gestell ist nicht angemahnt.
☑ Das Gestell ist angemahnt, was gleichzeitig bedeutet, dass es nicht verfügbar ist.

**Abholbereit** Datum, ab dem das Gestell beim Kunden abgeholt werden kann.

#### Wiedervorlage

**Am** Datum der Wiedervorlage zur Erinnerung.

**An** Partner, der die Erinnerung erhalten soll.

#### Gestelle

In der Übersicht werden alle Gestelle angezeigt, die den Suchkriterien entsprechen. In den einzelnen Spalten werden die Gestelldaten und Eigenschaften angezeigt, die oben beschrieben sind.

Zusätzlich werden folgende Spalten angezeigt:
- **Partner:** Kunde oder Lieferant, an den das Gestell ausgegeben wurde.
- **Ausgabedatum:** Datum, an dem die Ausgabe gebucht wurde.
- **Lieferant:** Lieferant, wenn das Gestell (Fremdgestell) von diesem zur Verfügung gestellt wurde.
- **Auswärtig:** Das Gestell ist außer Haus und damit nicht verfügbar.
- **Nicht mahnbar:** Das Gestell kann nicht angemahnt werden.
- **Tour-Nr.:** Nummer der Tour, mit der das Gestell außer Haus gebucht wurde.

### Gestellverwaltung – Ausgang

**Navigation:** Fertigung > Gestellverwaltung > Gestelle > Register Ausgang

[Image: Abb. E-118 Gestellverwaltung – Ausgang]

In diesem Register können Sie Gestelle aus dem verfügbaren Bestand ausbuchen und sich einen Überblick über die verfügbaren Gestelle anzeigen lassen.

#### Ausgabe

Mit der Wahl der Option legen Sie die Suchkriterien fest:
- **Gestell:** Die Suche bezieht sich auf Gestelle.
- **Zubehör:** Die Suche bezieht sich auf Zubehör.

#### An

Mit der Wahl der Option legen Sie die fest, an wen das Gestell ausgeliehen ist:
- **Kunde:** Die Suche bezieht sich auf Gestelle, die an Kunden ausgegeben wurden.
- **Lieferant:** Die Suche bezieht sich auf Gestelle, die an Lieferanten ausgegeben wurden.

#### Ausgabeinformationen

Die Felder werden erst freigeschaltet, wenn Sie ein neues Gestell anlegen oder wenn Sie in der Übersicht eines der verfügbaren Gestelle markiert haben, für das Sie einen Ausgang buchen wollen.

**Nummer** Nummer des Gestells.
**Art** Gestellart, z. B. A-Gestell groß.
**Kunde** Nummer des Kunden, an den die Lieferung geht.
**Straße, PLZ/Ort** Sie können eine abweichende Lieferanschrift für alle angezeigten Aufträge eintragen. Die Adressfelder werden freigeschaltet, wenn Sie die Checkbox **abw. Lieferadresse** markiert haben.
**Datum** Datum der Gestellbelegung. Standardmäßig ist das aktuelle Tagesdatum angezeigt. Es kann überschrieben werden.
**Versand** Bemerkung zum Versand. Diese Bemerkung wird in der Übersicht in der Spalte Versandinfo angezeigt.
**Fahrer, Tour** Fahrer und Tour, mit der das Gestell ausgeliefert wird.
**Spannlatten/Räder/Wagen** Zubehör, das zusätzlich zum Gestell ausgeliefert wird.
**Lieferschein** Nummer des Lieferscheins.
**Abw. Lieferadresse** Sie können eine abweichende Lieferadresse eintragen.
☐ Das Gestell wird an die Adresse des Auftrags geliefert.
☑ Das Gestell soll an eine abweichende Adresse geliefert werden. Die Adressfelder für Straße und Ort werden freigeschaltet.

#### Wiedervorlage

**Am** Datum der Wiedervorlage zur Erinnerung.
**An** Partner, der die Erinnerung erhalten soll.
**Bemerkung** Anmerkung zur Erinnerung.

#### Verfügbare Gestelle

> **Anzeige filtern**
> Nur wenn Sie die Option Ausgabe verfügbarer Gestelle aktiviert haben, werden alle Gestelle ausgeblendet, die nicht verfügbar sind. Die Option muss vor dem Start der Suche ausgewählt sein. Nicht verfügbare Gestelle werden nicht aus der Übersicht entfernt, wenn die Option nach der Suche aktiviert wurde.

In der Übersicht werden alle (verfügbaren) Gestelle mit folgenden Details angezeigt:
- **Nummer:** Gestellnummer.
- **Art:** Gestellart.
- **Ausgabe:** Datum der Ausgabe.
- **Partner:** Kunde oder Lieferant, an den das Gestell ausgegeben wurde.
- **Spannlatten, Räder, Wagen:** Jeweilige Anzahl des Zubehörs.
- **Versandinfo:** Text, der im Feld Versand eingegeben wurde.
- **Fremdgestell:** Gestell des Kunden oder Lieferanten.
- **Fahrer:** Fahrer, der das Gestell ausgeliefert hat.
- **Tour:** Tournummer, mit der das Gestell ausgeliefert wurde.
- **Tourbezeichnung:** Name der Tour.

### Gestellverwaltung – Eingang

**Navigation:** Fertigung > Gestellverwaltung > Gestelle > Register Eingang

[Image: Abb. E-119 Gestellverwaltung – Eingang]

In diesem Register können Sie die Gestelle wieder in den verfügbaren Bestand übernehmen, wenn sie von einer Lieferung oder einem Kunden zurückgekommen sind.
Die Felder sind ausführlich zum Register Ausgang beschrieben.
⇨ "Gestellverwaltung - Ausgang" auf Seite E-246

Sie können über das Menü Funktionen ein Gestell von einem Kunden an einen anderen umbuchen.
⇨ "Gestell umbuchen" auf Seite E-260

### Gestellverwaltung – Historie

**Navigation:** Fertigung > Gestellverwaltung > Gestelle > Register Historie

[Image: Abb. E-120 Gestellverwaltung – Historie]

In diesem Register können Sie die Historie einzelner Gestelle verfolgen. Wenn Sie ein Gestell in der Übersicht markiert haben, können Sie sich über die Schaltfläche [Ordner] anzeigen lassen, welche weiteren Gestelle bei dem Partner stehen.
⇨ "Übersicht Partner" auf Seite E-259

#### Auswahl

**Gestellnummer** Sie können die Auswahl auf eine bestimmte Gestellnummer einschränken. Wenn Sie keine Nummer eingeben, werden alle Gestelle aufgelistet, die den übrigen Kriterien entsprechen.

**Letzte Buchung zuerst** Sie können die Übersicht der Gestelle nach dem Buchungsdatum sortieren. Wenn Sie die Option aktivieren, bleibt die Sortierung auch in späteren Sitzungen aktiviert.
☐ Die Übersicht ist nach Spalte Art sortiert.
☑ Die Übersicht wird sortiert. Die zuletzt gebuchten Gestelle stehen am Anfang der Liste.

**Gestellart** Sie können die Auswahl auf eine bestimmte Gestellart einschränken. Wenn Sie keine Gestellart angeben, werden alle Gestelle aufgelistet, die den übrigen Kriterien entsprechen.
**Zeitraum von ... bis** Sie können die Auswahl auf einen Zeitraum einschränken, in dem Ausgang und/oder Eingang gebucht wurden.

**Buchungstyp** Sie können Sie Auswahl auf einen der folgenden Buchungstypen einschränken:
- **Gestellbelegung:**
  Mit dieser Option werden die Buchungen der Gestelle angezeigt.
- **Gestellbewegung:**
  Mit dieser Option werden alle Gestelle angezeigt, für die es eine Ausgangs- und/oder Eingangsbuchung gibt.

#### Auswahl Partner
Mit der Wahl der Option legen Sie fest, nach welchen Kriterien die Gestelle in der Übersicht angezeigt werden sollen:
- **Alle:**
  Mit dieser Option werden alle Gestelle angezeigt, unabhängig davon, ob sie sich bei einem Kunden oder Lieferanten befinden.
- **Kunden, Lieferanten:**
  Mit dieser Option werden nur die Gestelle angezeigt, die sich bei einem Kunden oder einem Lieferanten befinden. In diesem Fall werden die Felder von und bis freigeschaltet.

**Sammelgestelle** Sammelgestelle können gesondert angezeigt werden.
☐ Alle Gestelle werden angezeigt, die den übrigen Kriterien entsprechen.
☑ Die Anzeige wird auf Sammelgestelle eingeschränkt.

**[Ordner]** Mit dieser Schaltfläche öffnen Sie den Dialog Übersicht Partner, in dem alle Gestelle aufgelistet sind, die bei dem aktuellen Partner stehen.
⇨ "Übersicht Partner" auf Seite E-259

**Von, bis** Sie können die Anzeige auf Gestelle einschränken, die sich bei einem bestimmten Kunden oder Lieferanten befinden. Wenn Sie eine Anfangs- und eine Endnummer eingeben, werden alle Partner berücksichtigt, deren Nummer in dieser Spanne liegt.

#### Gestelle
In der Übersicht werden alle Gestelle aufgelistet, die den Auswahlkriterien entsprechen.
- **Nummer:** Gestellnummer.
- **Art:** Gestellart.
- **Partner:** Kunde oder Lieferant, bei dem sich das Gestell befindet.
- **Ausgabe:** Datum, zu dem das Gestell außer Haus gebucht wurde.
- **Rückgabe:** Datum, zu dem der Gestelleingang gebucht wurde.
- **Buchung:** Datum der Buchung. Bei automatischen Buchungen sind das Datum der Rückgabe und das Datum der Buchung identisch.
- **Mitarbeiter:** Mitarbeiter, der die Buchung veranlasst hat.
- **Latten, Räder, Wagen:** Anzahl der Latten, Räder oder Wagen, die zu dem Gestell gehören.
- **Buchungstyp:** Bei Buchungen werden folgende Typen unterschieden: manuelle Buchung, Gestellausgang, Gestelleingang, Gestellzuordnung zu Auftrag.

### Gestellverwaltung – Mahnung

**Navigation:** Fertigung > Gestellverwaltung > Gestelle > Register Mahnung

[Image: Abb. E-121 Gestellverwaltung – Mahnung]

In diesem Register können Sie prüfen, welche Gestelle überfällig sind und angemahnt werden sollen. Die Mahnung bezieht sich immer auf alle Gestelle, die in der Übersicht mit einem Häkchen aktiviert sind.

> **Einheitlicher Kunde**
> Achten Sie darauf, dass Sie zum Druck nur Gestelle aktivieren, die an einen einzigen Kunden oder Lieferanten gegangen sind. Markieren Sie die Zeile mit einem Doppelklick in die erste Zelle. Für jeden Kunden wird eine Mahnung gedruckt

#### Auswahl
- **Kunde von, bis:** Sie können eine einzelne Kundennummer eingeben oder eine Spanne von Nummern. Der Name des ersten und des letzten Kunden wird angezeigt.
- **Auswärtig ... Tage:** Sie können nach Gestellen suchen, die seit einer bestimmten Anzahl von Tagen außer Haus sind, z. B. 30 - 60 Tage.
- **Mahnstatus:** Sie können die Anzeige auf die Gestelle einschränken, die bereits angemahnt wurden. Wenn Sie die Suche nicht auf eine bestimmte Mahnstufe einschränken, werden alle Gestelle angezeigt.

> **Mahnstatus zurücksetzen**
> Wenn Sie in diesem Register den Mahnstatus zurücksetzen, wird bei allen in der Übersicht angezeigten Gestellen der Mahnstatus auf Null gesetzt. Wenn Sie den Mahnstatus für einzelne Gestelle zurücksetzen wollen, müssen Sie entweder nur das entsprechende Gestell in die Übersicht holen oder den Dialog Mahnstatus zurücksetzen im Auswahlmodus starten.
> ⇨ "Mahnstatus zurücksetzen" auf Seite E-261

#### Optionen
- **Wiederholungsdruck:** Den Wiederholungsdruck müssen Sie dann starten, wenn Sie eine Mahnung erneut drucken wollen.
  - ☐ Die Mahnung wird zum ersten Mal gedruckt.
  - ☑ Die Mahnung wird erneut gedruckt.
- **(Versandart):** Die Mahnung kann auf verschiedene Arten versendet werden.
  - **Postversand:** Die Mahnung wird per Post versendet. Das Dokument wird ausgedruckt.
  - **Faxversand:** Die Mahnung wird per Fax versendet.
  - **Faxversand Vertreter:** Die Mahnung wird per Fax an den zuständigen Vertreter versendet.
  - **Mail:** Die Mahnung wird per Mail versendet.
  - **Mail Vertreter:** Die Mahnung wird per Mail an den zuständigen Vertreter versendet.

#### Mahntexte
- **Kopf, Fuß:** Sie können für die Kopf- und Fußzeilen der Mahnung unterschiedliche Texte auswählen. Alternativ zu den hinterlegten Texten können Sie auch in beiden Feldern einen eigenen Text schreiben.

#### Auswärtige Gestelle
In der Übersicht werden alle Gestelle angezeigt, die den Auswahlkriterien entsprechen.
- **Nummer:** Gestellnummer.
- **Art:** Gestellart.
- **Kunde:** Name des Kunden, an den das Gestell ausgeliefert wurde.
- **Faxnummer:** Faxnummer des Kunden.
- **Mail:** Mail-Adresse des Kunden.
- **Mahnstatus:** Nur bei bereits gemahnten Gestellen wird ein Mahnstatus angezeigt.
- **Ausgabedatum:** Datum, zu dem das Gestell ausgebucht wurde.
- **Tage ausw.:** Anzahl der Tage seit dem Ausgabedatum.
- **Latten, Räder, Wagen:** Anzahl der Latten, Räder und Wagen, die zum Gestell gehören.
- **Gesperrt:** Das Gestell ist für weitere Buchungen gesperrt.
- **Verloren:** Das Gestell ist nicht im Bestand, sein Verbleib kann nicht geklärt werden.
- **Stationär:** Das Gestell wird nur stationär verwendet.

## Gestellverwaltung

**Navigation:** Fertigung > Gestellverwaltung

Sie können die Verpackung von produzierten Aufträgen auf Gestellen planen und steuern. Dazu stehen im Menü Gestellverwaltung folgende Dialoge zur Verfügung.
- Gestellarten
- Gestelle
- Kundenkommissionen

In diesem Abschnitt finden Sie Informationen zu folgenden Dialogen des Programmbereichs:
- "Gestellarten" auf Seite E-256
- "Gestelle" auf Seite E-240
- "Gestellübersicht" auf Seite E-258
- "Übersicht Partner" auf Seite E-259
- "Mahnstatus zurücksetzen" auf Seite E-261
- "Gestell umbuchen" auf Seite E-260
- "Kundenkommissionen" auf Seite E-266

### Gestellarten

**Navigation:** Fertigung > Gestellverwaltung > Gestellarten

[Image: Abb. E-122 Gestellarten]

In diesem Dialog können Sie unterschiedliche Gestellarten anlegen. Die Gestellarten werden den Gestellen zugewiesen. Sie dienen zur Organisation von Gestellen gleicher Machart.

#### Gestellart
- **Bezeichnung:** Name der Gestellart.
- **Bemerkung:** Anmerkung zur Gestellart, z. B. Verwendung nicht außer Haus.
- **Max. Breite / Max. Höhe:** Größte zulässige Breite und Höhe der Scheiben, die das Gestell aufnehmen kann.
- **Eigengewicht / Max. Gew.:** Eigengewicht der Gestellart und Höchstgewicht im beladenen Zustand. Die Differenz ergibt die zulässige Beladung.
- **Gestellwert:** Als Wert des Gestells können Sie z. B. den Anschaffungspreis angeben, oder den Verleihwert.
- **Gestelltyp:** Typ des Gestells, z. B. A-Gestell oder Fächerwagen.
- **Standard bei Neuanlage**
- **Anzahl Spannlatten:** Die Angabe der Spannlatten dient dazu, bei der Rückgabe des Gestells dessen Vollständigkeit zu prüfen.
- **Anzahl Räder:** Die Angabe der Räder dient dazu, bei der Rückgabe des Gestells dessen Vollständigkeit zu prüfen.
- **Anzahl Wagen:** Die Angabe der Wagen dient dazu, bei der Rückgabe des Gestells dessen Vollständigkeit zu prüfen.
- **Stationär:** Gestelle können sowohl zum Transport von Gläsern dienen, als auch als Abstellplatz.
  - ☐ Das Gestell kann frei verwendet werden, z. B. auch für Lieferungen außer Haus.
  - ☑ Das Gestell hat einen festen Standort. Es kann nicht für Lieferungen verwendet werden.

#### Tabelle
In der Übersicht werden alle Gestellarten aufgelistet, die den Suchkriterien entsprechen.
- **Bezeichnung:** Name der Gestellart.
- **Bemerkung:** Bemerkung zur besonderen Verwendung, Größe usw.
- **Max. Breite, max. Höhe:** Höchste zulässige Größe der Scheiben.
- **Eigengewicht:** Gewicht ohne Beladung.
- **Max. Gewicht:** Höchstgewicht im beladenen Zustand.
- **Wert:** Anschaffungs- oder Verleihwert.
- **Latten, Räder, Wagen:** Anzahl der Spannlatten, Räder und Wagen.
- **Stat.:** Angabe, ob das Gestell stationär verwendet wird.

### Gestellübersicht

**Navigation:** Fertigung > Gestellverwaltung > Gestelle > Register Gestelle > Schaltfläche am Feld Nummer

[Image: Abb. E-123 Gestellübersicht]

In diesem Dialog prüfen Sie die Gestellnummern, wenn Sie ein neues Gestell anlegen möchten.

#### Gestelle
- **Gesamt:** Anzahl der angelegten Gestellnummern.
- **Verfügbar:** Anzahl der verfügbaren Gestelle.

#### Auswahl
- **Gestellnummer:** Nummer des Gestells.
- **Gestellart:** Art des Gestells.
- **Kundennummer, Name:** Nummer und Name des Kunden.
- **Ausgabedatum:** Datum, zu dem das Gestell außer Haus gebucht wurde.

### Übersicht Partner

**Navigation:** Fertigung > Gestellverwaltung > Gestelle > Register Historie > [Ordner]

[Image: Abb. E-124 Gestelle - Übersicht Partner]

In diesem Dialog prüfen Sie, welche Gestelle bei einem bestimmten Marktpartner stehen oder gestanden haben.

#### Auswärtig
In diesen Feldern werden die Summen angezeigt:
- **Gestelle:** Anzahl der Gestelle, die zurzeit bei diesem Partner sind.
- **Latten:** Anzahl der Latten, die zurzeit beim Partner sind.
- **Räder:** Anzahl der Räder, die zurzeit beim Partner sind.
- **Wagen:** Anzahl der Wagen, die zurzeit beim Partner sind.

#### Gestelle
- **Gestellnr.:** Nummer des angelegten Gestells.
- **Gestellart:** Art des Gestells.
- **Ausgabe:** Datum, zu dem das Gestell außer Haus gebucht wurde.
- **Rückgabe:** Datum, zu dem der Gestelleingang gebucht wurde.
- **Latten, Räder, Wagen:** Anzahl der Latten, Räder oder Wagen, die zu dem Gestell gehören.

### Gestell umbuchen

**Navigation:** Fertigung > Gestellverwaltung > Gestelle > Menü Funktionen > Gruppe Ausführen > Gestell umbuchen

[Image: Abb. E-125 Gestell umbuchen]

In diesem Dialog buchen Sie ein Gestell von einem Partner auf einen anderen um.

#### Auswärtige Gestelle
In der Übersicht werden alle Gestelle angezeigt, die zurzeit außer Haus sind.
- **Nummer:** Nummer des angelegten Gestells.
- **Gestellart:** Art des Gestells.
- **Kunde:** Nummer des Kunden.
- **Ausgabe:** Datum, zu dem das Gestell außer Haus gebucht wurde.

#### Gestell
- **Nummer:** Nummer des markierten Gestells
- **Art:** Gestellart des markierten Gestells

#### Umbuchen
- **Von:** Nummer und Name des Partners, auf den das auswärtige Gestell gebucht ist.
- **Nach:** Sie können die Nummer des neuen Partners eintragen oder über die Suche auswählen.

### Mahnstatus zurücksetzen

**Navigation:** Fertigung > Gestellverwaltung > Gestelle > Menü Funktionen > Gruppe Ausführen > Mahnstatus zurücksetzen

[Image: Abb. E-126 Mahnstatus zurücksetzen]

In diesem Dialog setzen Sie den Mahnstatus für einzelne Gestelle zurück.

## Gestellbelegung

**Navigation:** Fertigung > Gestellverwaltung > Gestelle > Register Gestelle > Menü Funktionen > Gruppe Ausführen > Gestellbelegung

In diesem Dialog können Sie die Zuordnung von Auftragspositionen zu Gestellen festlegen.

> **Voraussetzung**
> Sie können eine Zuordnung nur festlegen, wenn Sie Gestelle angelegt haben und die Gestelle verfügbar sind. Gestelle können Sie in der Gestellverwaltung im Register Gestelle anlegen.

In diesem Dialog finden Sie folgende Register:
- "Gestellbelegung - Nach Auftrag" auf Seite E-262
- "Gestellbelegung - Nach Gestell" auf Seite E-264

### Gestellbelegung – Nach Auftrag

**Navigation:** Fertigung > Gestellverwaltung > Gestelle > Menü Funktionen > Gruppe Ausführen > Gestellbelegung > Register Nach Auftrag

[Image: Abb. E-127 Gestellbelegung – Nach Auftrag]

In diesem Register ordnen Sie den einzelnen Positionen eines Auftrags die Gestelle zu. Sie können zusätzlich festlegen, welche Menge einer Position auf dem Gestell abgestellt werden soll. Sie können mehrere Positionen demselben Gestell zuordnen.

#### Auswahl

**Auftrag** Nummer des Auftrags.
**Kunde** Nummer und Name des Kunden. Die Felder werden gefüllt, wenn Sie die Auftragsnummer eintragen.
**[Zuordnungen entfernen]** Löscht alle Zuordnungen der Auftragspositionen zu den Gestellen aus der Übersicht.
Wenn Sie nur eine Auftragsposition aus der Zuordnung löschen wollen, müssen Sie im Menü Start auf [Löschen] klicken.

#### Übersicht

In der Übersicht werden alle Positionen des ausgewählten Auftrags mit den Zuordnungen zu den Gestellen angezeigt. Sie können Zuordnungen zu einem Gestell bearbeiten oder neue Zuordnungen erstellen. Nur die Felder Gestell, Suche und Scheiben auf Gestell können bearbeitet werden, die anderen Felder werden automatisch gefüllt.
- **Pos:** Nummer der Auftragsposition.
- **Bezeichnung:** Bezeichnung des Glases.
- **Breite, Höhe:** Maße der Position.
- **Positionsmenge:** Stückzahl der Position.
- **Gewicht pro Stück:** Gewicht eines Stücks der Position.
- **Noch nicht abgestellt:** Stückzahl der Position, die noch keinem Gestell zugeordnet ist.
- **Gestell:** Nummer des Gestells, dem die Position zugeordnet werden soll.
- **Max. Höhe, Max Breite:** Höchste zulässige Maße der Scheiben. Die Felder werden automatisch gefüllt, wenn eine Gestellnummer eintragen ist.
- **Max. Gewicht:** Höchstgewicht im beladenen Zustand. Das Feld wird automatisch gefüllt, wenn eine Gestellnummer eintragen ist.
- **Suche:** Öffnet den Dialog Gestellübersicht, in dem Sie ein Gestell wählen können. Die Maße und das Gewicht des gewählten Gestells werden in der Tabelle übernommen. Das Feld Scheiben auf Gestell wird standardmäßig mit der Stückzahl aus dem Feld Positionsmenge gefüllt.
- **Scheiben auf Gestell:** Stückzahl der Scheiben, die dem gewählten Gestell zugeordnet werden sollen.
  Wenn Sie dem Gestell weniger Scheiben zuordnen als die Gesamtstückzahl der Position, wird automatisch eine neue Zeile mit der Differenzstückzahl der Position angezeigt. Sie können diese Stückzahl einem anderen Gestell zuordnen.

**Gesamt** Gesamtstückzahl der Auftragspositionen.
**Rest** Gesamtstückzahl der Positionen, die keinem Gestell zugeordnet sind.
**Auf Gestell** Gesamtstückzahl der Positionen, die einem Gestell zugeordnet sind.

### Gestellbelegung – Nach Gestell

**Navigation:** Fertigung > Gestellverwaltung > Gestelle > Menü Funktionen > Gruppe Ausführen > Gestellbelegung > Register Nach Gestell

[Image: Abb. E-128 Gestellbelegung – Nach Gestell]

In diesem Register ordnen Sie einem Gestell einzelne Positionen eines Auftrags zu. Sie können zusätzlich festlegen, welche Menge einer Position auf dem Gestell abgestellt werden soll.

#### Auswahl

**Gestell/Gestellart** Nummer und Art des Gestells. Sie können nur die Nummer des Gestells angeben, dem Positionen zugeordnet werden sollen. Das Feld Gestellart wird gefüllt.

**Max. Breite/Höhe/Gewicht** Höchste zulässige Maße der Scheiben und Höchstgewicht des beladenen Gestells. Die Felder werden gefüllt, wenn Sie eine Gestellnummer eintragen.
**[Gestell leeren]** Löscht alle Zuordnungen der Auftragspositionen zu dem markierten Gestell aus der Übersicht.
Wenn Sie nur eine Auftragsposition aus der Zuordnung löschen wollen, müssen Sie im Menü Start auf [Löschen] klicken.

#### Übersicht

In der Übersicht werden alle Positionen angezeigt, die dem ausgewählten Gestell zugeordnet sind. Sie können die Zuordnungen bearbeiten oder Positionen neu zuordnen. Nur die Felder Auftrag, Pos und Scheiben auf Gestell können bearbeitet werden, die anderen Felder werden automatisch gefüllt.
- **Auftrag:** Nummer des Auftrags.
- **Pos:** Nummer der Auftragsposition.
- **Bezeichnung:** Bezeichnung des Glases.
- **Maße:** Maße der Position.
- **Kunde:** Nummer des Kunden.
- **Maximal abstellbar:** Stückzahl der Position, die noch keinem Gestell zugeordnet ist.
- **Gewicht:** Gewicht der Stückzahl einer Position, die einem Gestell zugeordnet ist.
- **Scheiben auf Gestell:** Stückzahl der Scheiben, die dem gewählten Gestell zugeordnet werden sollen.

**Gesamt** Gesamtstückzahl der Auftragspositionen.
**(Gewicht) Auf Gestell** Gesamtgewicht der Positionen, die dem Gestell zugeordnet sind.
**Auf Gestell** Gesamtstückzahl der Positionen, die dem Gestell zugeordnet sind.

### Kundenkommissionen

**Navigation:** Fertigung > Gestellverwaltung > Kundenkommissionen

Mit der Kundenkommission werden weitere Details für den Versand festgelegt.

In diesem Dialog finden Sie folgende Register:
- "Kundenkommissionen - Kommission" auf Seite E-266
- "Kundenkommissionen - Abladestelle" auf Seite E-267
- "Kundenkommissionen – Zuordnung" auf Seite E-268

#### Kundenkommissionen – Kommission

**Navigation:** Fertigung > Gestellverwaltung > Kundenkommissionen > Register Kommission

[Image: Abb. E-129 Kundenkommissionen - Kommission]

In diesem Register legen Sie die Standard-Kommission des Kunden fest. Dadurch können Sie im Auftrag bei der Positionserfassung die gewünschte Kommission auswählen.
⇨ Softwarereferenz, "Kommission" auf Seite C-467

#### Kundenkommissionen – Abladestelle

**Navigation:** Fertigung > Gestellverwaltung > Kundenkommissionen > Register Abladestelle

[Image: Abb. E-130 Kundenkommissionen - Abladestelle]

In diesem Register geben Sie an, welche Abladestellen beim Kunden in der Regel angefahren werden.

#### Kundenkommissionen – Zuordnung

**Navigation:** Fertigung > Gestellverwaltung > Kundenkommissionen > Register Zuordnung

[Image: Abb. E-131 Kundenkommissionen – Zuordnung]

In diesem Register ordnen Sie die Kommissionen den Abladestellen zu.

## Terminübersicht

**Navigation:** Fertigung > Terminübersicht > Terminübersicht

In der Terminübersicht können Sie sich anzeigen lassen, was in einem bestimmten Zeitraum produziert werden muss und welche Materialien dazu benötigt werden.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menüs in der Terminübersicht" auf Seite E-269
- "Terminübersicht (Dialog)" auf Seite E-270
- "Exportieren" auf Seite E-277

### Menüs in der Terminübersicht

Über die Menüs im Dialog Terminübersicht können Sie die Standardeinstellung des Dialoges festlegen und andere Dialoge öffnen, ohne die Terminübersicht zu schließen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite E-269
- "Menü Optionen" auf Seite E-270

### Menü Funktionen

**Navigation:** Fertigung > Terminübersicht > Terminübersicht > Menü Funktionen

Im Register Tabelle können Sie über dieses Menü andere Dialoge öffnen, ohne die Terminübersicht zu schließen.

Das Menü ist in folgende Gruppen gegliedert:
- "Gruppe Dokument" auf Seite E-263
- "Gruppe Auswahl" auf Seite E-264

#### Gruppe Dokument
- **Historie:**
  Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des markierten Dokuments. Eine ausführliche Beschreibung finden Sie im Part Verkauf.
  ⇨ Verkauf, "Historie" auf Seite C-564
- **Anzeigen:**
  Öffnet den Dialog Dokumentenansicht zu einer Vorschau auf das Dokument. Eine ausführliche Beschreibung finden Sie im Part Verkauf.
  ⇨ Verkauf, "Reklamationen" auf Seite C-605

#### Gruppe Auswahl
- **Exportieren:**
  Öffnet den Dialog Export, in dem Sie auswählen können, welche Daten in eine Exportdatei geschrieben werden sollen.
  ⇨ "Exportieren" auf Seite E-277

### Menü Optionen

**Navigation:** Fertigung > Terminübersicht > Terminübersicht > Menü Optionen

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellungen werden nicht zurückgesetzt, wenn Sie den Dialog schließen. Folgende Einträge werden angezeigt:
- **Automatischer Seitenvorschub aktiv:**
  Im Druck wird nach jedem Datum und Auftrag ein Seitenumbruch eingefügt.
- **Archiv:**
  Das Archiv wird herangezogen, z. B. um Vergleichszeiträume des Vorjahrs zu auszuwerten.

### Terminübersicht (Dialog)

**Navigation:** Fertigung > Terminübersicht > Terminübersicht

In der Terminübersicht wird angezeigt, welche Mengen in einem bestimmten Zeitraum produziert werden müssen und welche Materialien dazu benötigt werden. Die Auswertungen können gedruckt oder exportiert werden.

In diesem Dialog finden Sie folgende Register:
- "Terminübersicht - Auswahl" auf Seite E-271
- "Terminübersicht - Tabelle" auf Seite E-276

**Zu Dialogbeschreibung:**
⇨ Analyse Verbrauch
