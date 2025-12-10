---
title: "DE-HB-AWEnterprise_14"
source: "DE-HB-AWEnterprise_14.pdf"
tags: ["A+W Enterprise", "Verkauf", "Packmittelplanung", "Auftragserfassung", "Preise und Konditionen", "Software-Referenz", "Lieferscheine", "Rechnungen", "ERP", "Benutzerhandbuch"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "Dieses Dokument ist ein Software-Referenzhandbuch für das A+W Enterprise Verkaufsmodul. Es beschreibt Funktionen wie die Packmittelplanung, die Verwaltung von Anmerkungen, die Textbearbeitung, die Konfiguration von Preisen und Konditionen, die Auftragsfreischaltung, die Lieferungs- und Rechnungsstellung."
long_description: "Dieses Dokument dient als umfassendes Referenzhandbuch für das Verkaufsmodul der ERP-Software A+W Enterprise. Es bietet detaillierte Beschreibungen der Benutzeroberflächen, Dialoge, Felder und Funktionen, die für die Auftragsabwicklung relevant sind. Das Handbuch ist in mehrere Hauptabschnitte gegliedert. Der Abschnitt 'Packmittelplanung' erklärt, wie Artikel auf Gestelle geplant und Fütterungen sowie Abstände konfiguriert werden. Der Abschnitt 'Anmerkungen' beschreibt, wie interne Informationen zu Vorgängen, Marktpartnern, Artikeln und Objekten mit unterschiedlichen Prioritäten hinterlegt werden. Der Abschnitt 'Texte' behandelt die Verwaltung von Kopf-, Fuß-, Artikel- und Positionstexten, die auf verschiedenen Formularen gedruckt werden können, einschließlich der Verwendung von Floskeln und speziellen Texten wie Kistignaturen. Ein umfangreicher Teil des Dokuments widmet sich den 'Preisen und Konditionen' und erläutert die verschiedenen Dialoge zur Definition von auftragsbezogenen Preisen für Glasarten, Sprossen, Zubehör und Bearbeitungen. Dies schließt Auftragskonditionen, Auftragspreise, Nachkalkulationen und Stufenpreise mit ein. Weitere Abschnitte behandeln die 'Freischaltung' von Aufträgen, die aus verschiedenen Gründen gesperrt sein können, sowie die 'Lieferung' mit der Erstellung von Lieferplänen und Lieferscheinen. Schließlich wird die 'Rechnungen'-Funktionalität detailliert, die die automatische und manuelle Erstellung von Rechnungen, Abschlagsrechnungen und Schlussrechnungen abdeckt. Jeder Abschnitt enthält technische Informationen zu den Datenbankfeldern und Navigationspfade zur jeweiligen Funktion."
---

# Softwarereferenz: A+W Enterprise Verkauf

---
## Packmittelplanung

- **(Unbenannt):** fest, wieviele der Positionsartikel zu der Gruppe zugeordnet werden sollen.
    - **Technische Info:** numerisches Feld, DB-Feld: kposgpl.gruppe

- **Zwraum:** Fütterung im Zwischenraum. Die Dicke der Fütterung zwischen den Scheiben in mm.
    - **Technische Info:** numerisches Feld, DB-Feld: kposgpl.zwraum

- **Anz:** Anzahl an Scheiben je Fütterung. Es soll z. B. alle fünf Scheiben jeweils eine Fütterung eingefügt werden.
    - **Technische Info:** numerisches Feld, DB-Feld: kposgpl.zwabs

- **Quer:** Anzahl an nebeneinander stehenden Scheiben. Die Anzahl kann nur geändert werden, wenn für den Gestelltyp nebeneinander packen erlaubt ist. Wenn für die Position der Gesamt-Algorithmus oder eine Gruppierung festgelegt wurde, dann kann die Anzahl nicht bearbeitet werden.
    - **Technische Info:** numerisches Feld, DB-Feld: kposgpl.anzquer

- **Hoch:** Anzahl an übereinander stehenden Scheiben. Die Anzahl kann nur geändert werden, wenn für den Gestelltyp übereinander packen erlaubt ist. Wenn für die Position der Gesamt-Algorithmus oder eine Gruppierung festgelegt wurde, dann kann die Anzahl nicht bearbeitet werden.
    - **Technische Info:** numerisches Feld, DB-Feld: kposgpl.anzhoch

### Fußzeile

In der Fußzeile werden die Artikelnummer, die Artikelhauptbezeichnung, sowie die Breite und Höhe des Artikels der ausgewählten Position angezeigt.

## Packmittelplanung

**Verkauf > Auftragserfassung > Fußbereich > Feld Rabatt > `<Strg>` + `<G>` > Positionen auf Gestelle verplanen > `<F3>`**

**Abb. D-107 Packmittelplanung**

In diesem Dialog wird das Ergebnis der Packmittelplanung angezeigt. In der Übersicht sehen Sie den geplanten Bedarf an Packmitteln und deren Beladung. Die Packmittelplanung wird vom System berechnet. Sie können das Ergebnis der Packmittelplanung nicht bearbeiten. Wenn Sie die Packmittelplanung ändern möchten, weil Sie z. B. sehen, dass die Gestelle nicht optimal ausgelastet sind, dann können Sie in den Dialog Vorgaben Packmittelplanung wechseln. In dem Dialog können Sie die Vorgaben, die das System für die Berechnung heranzieht, ändern und die Packmittelplanung neu starten.

⇨ "Vorgaben Packmittelplanung" auf Seite D-1295

Sie können den Dialog Packmittelplanung nicht schließen. Wenn Sie den Dialog verlassen möchten, dann wechseln Sie in den Dialog Vorgaben Packmittelplanung.

- Mit `<Strg>` + `<F10>` können Sie in den Dialog Vorgaben Packmittelplanung wechseln.
- Mit `<F2>` können Sie für jedes Packmittel bis zu vier Texte hinterlegen. Sie können für jeden Text durch die Auswahl von J für Ja und N für Nein in der Spalte Bestellungen entscheiden, ob dieser auf den Bestellunterlagen ausgedruckt wird.
- Das Hinterlegen von Texten für die Packmittel ist von den Einstellungen in den Stammdaten und der jeweiligen Systemkonfiguration abhängig.

Folgende Ansichten sind nur kundenspezifisch freigeschaltet:
- Mit `<F5>` wechseln Sie in die Ansicht Kistenmaße.
- Mit `<Shift>` + `<F5>` wechseln Sie in die Ansicht KistenInfo.

### Kopfbereich

Die Felder im Kopfbereich sind zum Dialog Vorgaben Packmittelplanung beschrieben:
⇨ "Vorgaben Packmittelplanung" auf Seite D-1295

### Übersicht Packmittelplanung

Die Spalten sind zum Dialog Vorgaben Packmittelplanung beschrieben:
⇨ "Vorgaben Packmittelplanung" auf Seite D-1295

Zusätzlich werden folgende Spalten angezeigt:

**Gestellnr** Packmittelnummer. Die Packmittelnummer wird vom System vergeben.
**Technische Info:** Anzeigefeld, DB-Feld: kposgest.vsgnr

**Lfd** Laufende Nummerierung der Packmittel.
**Technische Info:** Anzeigefeld, DB-Feld: kposgest.Ifdpos

**Breite** Breite der Glasscheibe.
**Technische Info:** Anzeigefeld, DB-Feld: kpos.laenge

**Höhe** Höhe der Glasscheibe.
**Technische Info:** Anzeigefeld, DB-Feld: kpos.breite

**Tiefe** Tiefe der Beladung. Die Beladungstiefe, berechnet aus Dicke aller Glasscheiben zusammen und den Fütterungen.
**Technische Info:** Anzeigefeld

**Gewicht** Summiertes Gewicht der Glasscheiben auf dem Gestell.
**Technische Info:** Anzeigefeld

### Fußzeile

Folgende Packmittelinformationen zu der ausgewählten Position werden angezeigt:
- **Gestell:** Packmittelnummer.
- **GesAnzahl:** Anzahl der Artikel, die auf das Packmittel beladen werden.
- **Ges Tiefe:** Die Artikel-Beladungstiefe, berechnet aus der Anzahl der Artikel, aber ohne die Fütterungen.
- **GesGewicht:** Die Summe aus dem Packmitteleigengewicht und dem Gewicht der Artikel.

## Anmerkungen

Anmerkungen sind interne Informationen, die nicht auf Formularen ausgegeben werden. Sie werden je nach Konfiguration automatisch angezeigt oder können manuell aufgerufen werden.

Sie können in einer Anmerkung mehrere Textzeilen erfassen. Für jede Textzeile können Sie eine eigene Priorität und einen Info-Ort festlegen.

Die Marktpartner-, Artikel- und Objekt-Anmerkungen können in den Stammdaten hinterlegt werden. Die Vorgangs-Anmerkungen werden nur im jeweiligen Vorgang und nicht in den Stammdaten hinterlegt.

> **Datenbankbezug in den Anmerkungstexten**
> Die Anmerkungen werden in der Datenbanktabelle memo gespeichert. Die Art der Anmerkung wird durch die entsprechenden Einträge memp.typ, memo.key1-3 und memp.flag1-3 festgelegt.

**Tab. D-8 Stufen der Priorität**

| Priorität | Bedeutung |
| :--- | :--- |
| **Niedrig** | Anmerkungen sind für den jeweiligen Anmerkungs-Typ über das Info-Menü einsehbar, werden aber nicht automatisch angezeigt. |
| **Mittel** | Anmerkungen sind für den jeweiligen Anmerkungs-Typ über das Info-Menü einsehbar, werden aber nicht automatisch angezeigt. |
| **Hoch** | Anmerkungen werden für den jeweiligen Anmerkungs-Typ automatisch angezeigt, wenn der Marktpartner, der Vorgang, das Objekt oder der Artikel, zu dem die Anmerkung erfasst wurde, aufgerufen wird. Wenn die Anmerkung angezeigt wird, wird der komplette Anmerkungstext angezeigt, d. h. in der Anmerkung werden auch alle Textzeilen der Priorität Niedrig oder Mittel angezeigt. |
| **Sperre für Bezug** | Auf Vorgänge mit Anmerkungen dieser Priorität kann kein Bezug genommen werden. Der hinterlegte Informationstext wird automatisch angezeigt, wenn der Vorgang als Bezugsvorgang herangezogen werden soll oder der Vorgang geöffnet wird. Diese Priorität kann nur für Vorgangs-Anmerkungen gewählt werden. |

Je nach Anmerkungstyp wird der Anmerkungstext automatisch zu dem entsprechenden Bearbeitungsschritt angezeigt, wenn seine Priorität auf hoch gesetzt ist:

- **Vorgangs-Anmerkungen:** Diese Anmerkungstexte werden angezeigt, sobald der Vorgang geöffnet wird.
- **Marktpartner-Anmerkungen:** Diese Anmerkungstexte werden angezeigt, sobald der Marktpartner ausgewählt wird. Die Anmerkung bezieht sich auf den ausgewählten Marktpartner, z. B. den Kunden oder den Lieferanten.
- **Objekt-Anmerkung:** Diese Anmerkungstexte werden angezeigt, sobald das Objekt ausgewählt wird. Sie können nur Anmerkungen für ein Objekt hinterlegen, wenn Sie für den Auftrag ein Objekt ausgewählt haben.
- **Artikel-Anmerkungen:** Diese Anmerkungstexte werden angezeigt, sobald der Artikel ausgewählt wird.
- **Kunden-Anmerkungen:** Diese Anmerkungstexte werden angezeigt, sobald der Kunde ausgewählt wird.
- **Kunden-Artikel-Anmerkungen:** Diese Anmerkungstexte werden angezeigt, sobald er Artikel für diesen Kunden ausgewählt wird.
- **Objekt-Artikel-Anmerkungen:** Diese Anmerkungstexte werden angezeigt, sobald der Artikel für dieses Objekt ausgewählt wird.
- **Lieferanten-Anmerkungen:** Diese Anmerkungstexte werden angezeigt, sobald der Lieferant ausgewählt wird.
- **Lieferanten-Artikel-Anmerkungen:** Diese Anmerkungstexte werden angezeigt, sobald der Artikel für diesen Lieferanten ausgewählt wird.

Sie können sich Anmerkungen zu Vorgängen, Marktpartnern, Artikeln, Objekten und verschiedenen Kombinationen aus diesen Typen, z. B. Objekt-Artikel-Anmerkungen, anzeigen lassen und bearbeiten.

- "Vorgangs-Anmerkungen" auf Seite D-1306
- "Marktpartner-, Objekt-, Artikel-Anmerkungen" auf Seite D-1307
- "Marktpartner-Artikel-Anmerkungen" auf Seite D-1310

### Vorgangs-Anmerkungen

**Verkauf > Auftragserfassung > Kopf-, Fußbereich > `<Shift>` + `<F4>` > Vorgangs-Anmerkungen**
**Verkauf > Auftragserfassung > Positionsebene > `<Shift>` + `<F4>` > Anmerkungen > Vorgangs-Anmerkungen**

**Abb. D-108 Anmerkungen zum Vorgang**

In diesem Dialog hinterlegen Sie Anmerkungen zu dem geöffneten Vorgang. Sie können die Vorgangs-Anmerkungen im Kopfbereich und auf der Positionsebene eines Vorgangs erfassen. Die Anmerkungen können Sie nur für den aktuellen Vorgang hinterlegen. Sie werden nicht in den Stammdaten gespeichert.

#### Rumpfbereich

**(Eingabezeilen für Text)** Anmerkungstext zum geöffneten Vorgang. Mit `<Enter>` wechseln Sie in die nächste Textzeile. Jede Textzeile wird einzeln konfiguriert, d. h. Sie können für jede Zeile die Priorität festlegen.
**Technische Info:** alphanumerische Felder, DB-Felder: infokauf.atxt

#### Fußbereich

In der Fußzeile wird die Priorität für die aktuelle Anmerkung angezeigt.
Ändert die Priorität für die gewählte Textzeile.
Alternativ können Sie die Priorität mit `<Shift>` + `<F10>` ändern.

### Marktpartner-, Objekt-, Artikel-Anmerkungen

**Verkauf > Auftragserfassung > Kopf-, Fußbereich > `<Shift>` + `<F4>` > Marktpartner-, Objekt-, Artikel-Anmerkungen**
**Verkauf > Auftragserfassung > Positionsebene > `<Shift>` + `<F4>` > Anmerkungen > Kunden-, Lieferanten-, Objekt-, Artikel-Anmerkungen**

**Abb. D-109 Anmerkungen zum Marktpartner, Objekt oder Artikel**

In diesen Dialogen werden Anmerkungen zum Marktpartner, zum Objekt oder zum Artikel angezeigt. Die Dialoge sind analog aufgebaut. Abweichungen werden im Folgenden explizit beschrieben.

Die Anmerkungstexte werden in der Regel in den Stammdaten angelegt. Wenn Sie die Anmerkungstexte bearbeiten und neue hinzufügen, speichern Sie diese mit `<F3>`. Die Änderungen werden in die Stammdaten übernommen und der Dialog wird geschlossen.

In Verkaufs-Vorgängen werden die Kunden-Anmerkungen angezeigt und in Einkaufs-Vorgängen die Lieferanten-Anmerkungen.

Auf Positionsebene können Sie im Verkauf die Lieferanten-Anmerkungen nur dann öffnen, wenn der markierten Position die Beschaffungsart Bestellung und ein Lieferant zugewiesen ist.

Sie können Objekt-Anmerkungen nur bearbeiten, wenn dem aktuellen Vorgang ein Objekt zugeordnet ist. Die Anmerkungen können Sie im Kopfbereich und auf der Positionsebene eines Vorgangs bearbeiten.

Artikel-Anmerkungen bearbeiten Sie zum aktuellen Artikel. Sie können die Artikel-Anmerkungen nur auf Positionsebene zur gewählten Position bearbeiten.

#### Kopfbereich

In den Dialogen werden nur die Felder angezeigt, die für den jeweiligen Anmerkungs-Typ relevant sind.

**Kunde** Kundennummer.
**Technische Info:** Anzeigefeld, DB-Feld: memo.key1

**Lieferant** Lieferantennummer.
**Technische Info:** Anzeigefeld, DB-Feld: memo.key1

**Objekt** Objektnummer.
**Technische Info:** Anzeigefeld, DB-Feld: memo.key1

**Artikel** Artikelnummer.
**Technische Info:** Anzeigefeld, DB-Feld: memo.key2

#### Rumpfbereich

**(Eingabezeilen für Text)** Anmerkungstext zum gewählten Marktpartner. Mit `<Enter>` wechseln Sie in die nächste Textzeile. Jede Textzeile wird einzeln konfiguriert, d. h. Sie können für jede Zeile die Priorität und den Info-Ort festlegen.
**Technische Info:** alphanumerische Felder, DB-Felder: memo.text

#### Fußbereich

In der Fußzeile werden die Priorität und der Info-Ort für die aktuelle Anmerkung angezeigt.
Die Schaltfläche Priorität ist ausführlich zum Dialog Vorgangs-Anmerkungen beschrieben:
⇨ "Vorgangs-Anmerkungen" auf Seite D-1306

Mit `<Shift>` + `<F9>` wechseln Sie den Info-Ort:

**Tab. D-9 Einstellungen zum Info-Ort**

| Info-Ort | Bedeutung |
| :--- | :--- |
| **Überall** | Information wird in den Stammdaten, den Verkaufs- und Einkaufsvorgängen angezeigt. |
| **VK-Auftrag** | Information wird in den Stammdaten und den Verkaufsvorgängen angezeigt. |
| **EK-Auftrag** | Information wird in allen Einkaufsvorgängen und den Stammdaten angezeigt. |
| **Stammdaten** | Information wird nur in den Stammdaten angezeigt. |

### Marktpartner-Artikel-Anmerkungen

**Verkauf > Auftragserfassung > Positionsebene > `<Shift>` + `<F4>` > Anmerkungen > Kunden-Artikel-, Lieferanten-Artikel-, Objekt-Artikel-Anmerkungen**

**Abb. D-110 Anmerkungen zum Kunden, Lieferanten oder Objekt mit einem bestimmten Artikel**

In diesen Dialogen werden jeweils Anmerkungen zum aktuellen Artikel des gewählten Kunden, Lieferanten oder Objekts angezeigt. Diese Anmerkungen können nur auf Positionsebene zur gewählten Position angezeigt werden.

Die Anmerkungstexte werden in der Regel in den Stammdaten angelegt. Wenn Sie die Anmerkungstexte bearbeiten und neue hinzufügen, speichern Sie diese mit `<F3>`. Die Änderungen werden in die Stammdaten übernommen und der Dialog wird geschlossen.

Lieferanten-Artikel-Anmerkungen im Verkauf werden nur angezeigt, wenn der markierten Position die Beschaffungsart Bestellung und ein Lieferant zugewiesen ist.

Objekt-Artikel-Anmerkungen werden nur angezeigt, wenn dem aktuellen Vorgang ein Objekt zugeordnet ist.

#### Kopfbereich

Die Felder im Kopfbereich sind ausführlich zu den Dialogen Marktpartner-, Objekt-, Artikel-Anmerkungen beschrieben:
⇨ "Marktpartner-, Objekt-, Artikel-Anmerkungen" auf Seite D-1307

#### Rumpfbereich

**(Eingabezeilen für Text)** Anmerkungstext zum gewählten Artikel des aktuellen Kunden. Mit `<Enter>` wechseln Sie in die nächste Textzeile. Jede Textzeile wird einzeln konfiguriert, d. h. Sie können für jede Zeile die Priorität und den Info-Ort festlegen.
**Technische Info:** alphanumerische Felder, DB-Felder: memo.txt

#### Fußbereich

Die Felder und Schaltflächen im Fußbereich sind ausführlich zu den Dialogen Marktpartner-, Objekt-, Artikel-Anmerkungen beschrieben:
⇨ "Marktpartner-, Objekt-, Artikel-Anmerkungen" auf Seite D-1307

## Texte

Mit Texten können zusätzliche Informationen zu Vorgängen angezeigt werden. Die Texte werden, je nach Text-Art, entweder vom System nach Vorgaben aus den Stammdaten und den Bewegungsdaten generiert oder manuell erfasst. Sie können Texte mit Informationen für Kunden auf verschiedenen Formularen ausdrucken. Texte mit internen Informationen können beim Aufrufen eines Vorgangs automatisch angezeigt werden.

Die Textverwaltung ist von den Einstellungen in den Stammdaten und der jeweiligen Systemkonfiguration abhängig.

Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Kopf- und Fußtexte" auf Seite D-1313
- "Artikel- und Positionstexte" auf Seite D-1315
- "Spezielle Texte" auf Seite D-1316
- "Floskeln" auf Seite D-1317
- "Fremdinformationen" auf Seite D-1319
- "Kistensignatur" auf Seite D-1320

### Kopf- und Fußtexte

**Verkauf > Auftragserfassung > Kopf-, Fußbereich > `<F4>` > Texte > Kopftext, Fußtext**
**Verkauf > Auftragserfassung > Positionsebene > `<F4>` > Texte > Kopftext, Fußtext**

**Abb. D-111 Kopf- und Fußtexte**

In diesem Dialog werden Texte mit zusätzlichen Informationen zum Vorgangskopf oder -fuß angezeigt. Die Texte werden anhand der Textverwaltung aus den Stammdaten generiert. Die Textverwaltung ist zu dem Part Stammdaten beschrieben:
⇨ Stammdaten, "Textverwaltung" auf Seite B-513

Sie können die Texte vorgangsbezogen bearbeiten und Floskeln hinzufügen.
Die Texte können auf verschiedenen Formularen ausgedruckt werden. Sie können die Auswahl der entsprechenden Formulare im rechten Teil des Dialogs Texte im Bereich Formulare ändern.

#### Register Kopftext

**(Eingabezeilen für Text)** Informationstext zum Kopfbereich. Mit `<Enter>` wechseln Sie in die nächste Textzeile.
**Technische Info:** alphanumerische Felder, DB-Felder: auftxt.txt

#### Register Fußtext

**(Eingabezeilen für Text)** Informationstext zum Fußbereich. Mit `<Enter>` wechseln Sie in die nächste Textzeile.
**Technische Info:** alphanumerische Felder, DB-Felder: auftxt.txt

#### Formulare

Im Bereich Formulare geben Sie an, auf welchen Formular-Arten der Informationstext ausgegeben wird.
- Der Informationstext wird auf das gewählte Formular gedruckt. In der Datenbank wird der Wert 1 zugeordnet.
- Auf das Formular wird kein Informationstext gedruckt. In der Datenbank wird der Wert 0 zugeordnet.
**Technische Info:** Checkboxen, DB-Felder: auftxt.formular

> **Datenbankbezug für Formulare**
> In der Datenbank werden alle Eingaben pro Formular in einem Formularvektor gespeichert. Alle Formulare sind in der vorgegeben Reihenfolge unter der entsprechenden Nummer im Formularvektor festgelegt (Nr. in der Tabelle Formular-Arten).
> Wenn einem Formular eine 1 zugeordnet ist, dann wird es gedruckt. Ist eine 0 zugeordnet, wird das Formular nicht gedruckt.

**Tab. D-10 Formular-Arten**

| Nr. | Feldinhalt | Bedeutung |
| :-- | :--- | :--- |
| 1 | Angebot | Text wird im Angebot gedruckt. |
| 2 | AB | Text wird in der Auftragsbestätigung gedruckt. |
| 3 | Anfrage | Text wird in der Lieferantenanfrage gedruckt. |
| 4 | Rechnung | Text wird auf die Rechnung gedruckt. |
| 5 | Gutschrift | Text wird auf die Gutschrift gedruckt. |
| 6 | Handzuschnitt-Liste | Text wird in der Handzuschnitt-Liste gedruckt. |
| 7 | Lieferschein | Text wird auf den Lieferschein gedruckt. |
| 8 | Produktion | Text wird auf die produktionsseitigen Papiere gedruckt. |
| 9 | Bestellung | Text wird auf die Einkaufsbestellung gedruckt. |
| 10 | Sprossenpapiere | Text wird in den Sprossenpapieren gedruckt. |
| 11 | Betriebsauftrag | Text wird im Betriebsauftrag gedruckt. |
| 12 | Etikett | Text wird auf die Etiketten gedruckt. |
| | Rahmentext | Text wird auf die produktionsseitigen Papiere gedruckt. |

#### Fußbereich

**Floskeln**
Öffnet den Dialog Floskeln zur Auswahl von bestehenden Floskeln.
⇨"Floskeln" auf Seite D-1317

**Floskeln neu**
Öffnet den Dialog Floskeln, in dem Sie eigene Floskeln anlegen können.
⇨"Floskeln" auf Seite D-1317

### Artikel- und Positionstexte

**Verkauf > Auftragserfassung > Positionsebene > `<F4>` > Texte > Artikeltext, Positionstext**

**Abb. D-112 Artikel- und Positionstexte**

In diesem Dialog werden Texte mit zusätzlichen Informationen zu den Artikeln oder Positionen eines Vorgangs angezeigt.
Die Texte werden aus den Stammdaten und entsprechend den Systemeinstellungen generiert. Die Textverwaltung wird kundenspezifisch konfiguriert und ist zu dem Part Stammdaten beschrieben:
⇨ Stammdaten, "Textverwaltung" auf Seite B-513

Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

Sie können die Texte vorgangsbezogen bearbeiten und Floskeln hinzufügen. Wenn Sie Floskeln für den Artikel- oder Positionstext gewählt haben, können Sie diese vorgangsbezogen bearbeiten.

Die Texte können auf verschiedenen Formularen ausgedruckt werden. Sie können die Auswahl der entsprechenden Formulare im rechten Teil des Dialogs im Bereich Formulare ändern.

#### Register Artikeltext

**(Eingabezeile für Text)** Informationstext zum gewählten Artikel. Mit `<Enter>` wechseln Sie in die nächste Textzeile.
**Technische Info:** alphanumerische Felder, DB-Felder: auftxt.txt

#### Register Positionstext

**(Eingabezeile für Text)** Informationstext zur gewählten Position. Mit `<Enter>` wechseln Sie in die nächste Textzeile.
**Technische Info:** alphanumerische Felder, DB-Felder: auftxt.txt

#### Formulare

Dieser Bereich ist ausführlich zum Dialog Kopf- und Fußtexte beschrieben.
⇨ "Kopf- und Fußtexte" auf Seite D-1313

#### Fußbereich

Dieser Bereich ist ausführlich zum Dialog Kopf- und Fußtexte beschrieben.
⇨ "Kopf- und Fußtexte" auf Seite D-1313

### Spezielle Texte

**Verkauf > Auftragserfassung > Positionsebene > `<F4>` > Texte > Spezielle Texte > Rahmentext, Produktkennzeichen, Modelltexte, Logotexte**

**Abb. D-113 Spezielle Texte**

In diesen Dialogen werden spezielle Texte zu den einzelnen Artikeln angezeigt. Die speziellen Texte werden anhand der Stammdaten vom System generiert. Die Textverwaltung ist von den Einstellungen in den Stammdaten und der jeweiligen Systemkonfiguration abhängig. Je nach Konfiguration können Sie die Texte vorgangsbezogen bearbeiten.

Die Dialoge sind nur kundenspezifisch freigeschaltet.

Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

Jedem Text ist eine Textnummer zugewiesen. Unter Umständen wird die Textnummer an die Produktion übergeben, wenn sie dort benötigt wird.

**Tab. D-11 Spezielle Texte**

| Textart | Beschreibung | Textnummer |
| :--- | :--- | :--- |
| **Rahmentext** | Zusätzliche Information zum Rahmentext, der auf den Rahmen gedruckt wird. | 1000 |
| **Produktkennzeichen** | Zusätzliche Informationen zum Produktkennzeichen, z. B. CEKAL-Zertifizierungs-Kennzeichen. | 1003 |
| **Modelltext** | Zusätzliche Information zum Modell. Die Parameter des Modells werden für jede Position als Text angezeigt. Sie können einen Modelltext nur zu Positionen mit einer Modellscheibe erfassen. | 1002 |
| **Logotext** | Zusätzliche Information zum Logo. Sie können einen Logotext nur zu Positionen mit einer Bearbeitung mit Logo erfassen. | 1010 |
| **Kistensignatur-Texte** | Kistensignatur für den Versand. ⇨ "Kistensignatur" auf Seite D-1320 | ab 5000 |

### Floskeln

**Verkauf > Auftragserfassung > Positionsbene > `<F4>` > Texte > Kopftext, Fußtext, Artikeltext, Positionstext > [Floskeln neu]**

**Abb. D-114 Floskeln**

In diesem Dialog können Sie Floskeln anlegen oder bearbeiten. Floskeln sind Standardtexte, die in den Stammdaten hinterlegt werden.

Floskeln können in den Kopf-, Fuß-, Artikel-, Positionstexten und den speziellen Texten als fertig vorformulierte Textbausteine herangezogen werden.

Im rechten Teil des Dialogs wählen Sie die Arten der Formulare aus, auf die die Floskeln gedruckt werden sollen.
**Technische Info:** alphanumerische Felder, DB-Feld: `floskel.code`, `floskel.txt`
"Formulare" auf Seite D-1314

**Kennung** Kennzeichen und Bezeichnung der Floskel. Wenn Sie das Kennzeichen einer bestehenden Floskel angeben, wird die Bezeichnung im Klartext angezeigt.
**Technische Info:** alphanumerische Felder, DB-Feld: `floskel.code`, `floskel.txt`

**(Eingabezeile für Text)** Standardtext, der der Floskel zugeordnet ist.
**Technische Info:** alphanumerische Felder, DB-Felder: `floskel.txt`

> **Bestehende Floskeln bearbeiten**
> Wenn Sie die Kennung einer bestehenden Floskel eintragen, können Sie diese Floskel bearbeiten und anschließend übernehmen.

Wenn Sie im Fußbereich der Text-Dialoge auf [Floskeln] klicken, wird ein Suchdialog angezeigt, in dem Sie nach angelegten Floskeln suchen können.

**Abb. D-115 Auswahl der Floskeln**

**Kennung** Kennzeichen der Floskel. Mit [Suchen] werden alle bestehenden Floskeln in einem separaten Dialog angezeigt. Wenn Sie eine Floskel auswählen, wird der Floskeltext in den Eingabezeilen des aktuellen Text-Dialogs angezeigt.
**Technische Info:** alphanumerisches Feld, DB-Feld: `floskel.code`

### Fremdinformationen

**Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > `<F4>` > Texte > Fremdinformationen**

**Abb. D-116 Fremdinformationen**

In diesem Dialog hinterlegen Sie Fremdinformationen. Fremdinformationen sind Informationen zur weiteren Vorgangsbearbeitung, die firmenintern an verschiedene Abteilungen übermittelt werden sollen.

**Fremdnummer** Kundenseitige Vorgangsbezeichnung unter der der Kunde diesen Auftrag führt. Die Eingabe wird in das Feld Knd-Bestnr übernommen. Mit der Knd-Bestnr können Sie nach Aufträgen suchen.
**Technische Info:** alphanumerisches Feld, DB-Feld: kauf.exaufnr

> **Vorgang über die Fremdnummer öffnen**
> Wenn Sie einen Vorgang über die Fremdnummer öffnen wollen, können Sie in der Auftragserfassung im Feld Vorgangsnummer mit `<F5>` in das Feld Knd-Bestnr wechseln. Wenn Sie die Fremdnummer eingeben und mit `<Enter>` bestätigen, werden alle Vorgänge mit dieser Fremdnummer angezeigt. Wenn Sie einen Eintrag auswählen, wird der entsprechende Vorgang geöffnet.

**Einkaufsinfo** Informationstext, der an die Abteilung Einkauf übermittelt wird. Die Information kann im Bestellpool angezeigt werden. Mit `<Ende>` speichern Sie die Daten und schließen den Dialog.
**Technische Info:** alphanumerisches Feld, DB-Feld: kauf.exbez1

**Versandinfo** Informationstext, der an die Versandsteuerung übermittelt wird. Die Versandinfo wird in der Versandsteuerung auf der Auftragsebene angezeigt. Mit `<Ende>` speichern Sie die Daten und schließen den Dialog.
**Technische Info:** alphanumerisches Feld, DB-Feld: kauf.exbez2

### Kistensignatur

**Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > `<Shift>` + `<F4>` > Kistensignatur**

**Abb. D-117 Kistensignatur**

In diesem Dialog wird die Kistensignatur für den Versand angezeigt. Die Kistensignatur wird für die Versandsteuerung benötigt und wird automatisch generiert.

Die Funktionen sind von den Einstellungen in den Stammdaten und der jeweiligen Systemkonfiguration abhängig. Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

Im Dialog können jeder Kistenseite Texte zugeordnet werden. Die Texte werden über Textformeln aus den Stammdaten generiert.

Der Dialog Textformeln ist zum Part Stammdaten beschrieben:
⇨ Stammdaten, "Textformeln" auf Seite B-521

Die Zuordnung der Kistensignatur wird in den Stammdaten hinterlegt.

Der Dialog Bezeichnungen für Kistensignatur ist im Part Stammdaten beschrieben:
⇨ Stammdaten, "Bezeichnungen für Kistensignatur" auf Seite B-355

Mit `<F3>` können Sie die Kistensignatur erzeugen. Dabei werden die Daten aus den Stammdaten herangezogen. Wenn sich die Kistensignatur in den Stammdaten verändert hat, werden die Daten in der Vorgangserfassung entsprechend aktualisiert.

Sie können die Kistensignatur auftragsbezogen bearbeiten.

- **Anordn.:** Druckposition der Signatur auf der Kiste:
    - vorne
    - hinten
    - oben
    - unten
    - links
    - rechts
    **Technische Info:** alphanumerisches Feld, DB-Feld: artkennfrm.formelbez

- **Seq.:** Sequenznummer. Auf jeder Kistenseite können mehrere Texte jeweils in einer eigenen Zeile gedruckt werden. Die Sequenznummer bestimmt die Reihenfolge, in der die Texte gedruckt werden. Der Text mit der Sequenznummer 1 wird in die 1. Zeile gedruckt, der Text mit der Sequenznummer 2 in die 2. Zeile usw.
    **Technische Info:** numerisches Feld, DB-Feld: infokauf.seqnr

- **Text:** Beschriftungstext für die Kistensignatur. Wenn Sie Kistensignaturen in den Stammdaten hinterlegt haben, wird der Text automatisch angezeigt. Sie können den Text aus den Stammdaten überschreiben.
    **Technische Info:** alphanumerisches Feld, DB-Feld: infokauf.atxt

## Preise und Konditionen

Für die Preisberechnung im Vorgang werden die Artikelpreise und Markpartner-Konditionen aus den Stammdaten herangezogen. Einzelne Preise und Konditionen können vorgangsbezogen bearbeitet werden.

Eine ausführliche Beschreibung finden Sie im Part Preise und Konditionen.

In diesem Abschnitt sind folgende Dialoge erklärt:

- "Auftragskonditionen" auf Seite D-1323
- "Auftragspreise" auf Seite D-1328
- "Auftragssprossenpreise" auf Seite D-1330
- "Auftragsaustauschpreise" auf Seite D-1333
- "Auftragsunterteilpreise" auf Seite D-1335
- "Nachkalkulation" auf Seite D-1336
- "Stufenpreise" auf Seite D-1339
- "Positionskonditionen" auf Seite D-1340
- "Produktionskostenkalkulation" auf Seite D-1372
- "Preiskalkulation" auf Seite D-1379

### Auftragskonditionen

**Verkauf > Auftragserfassung > Positionsebene > `<F4>` > Preisangaben > Auftragskonditionen**
**Verkauf > Auftragserfassung > Kopf-, Fußbereich > `<F4>` > Preisangaben > Vorgangskonditionen**

**Abb. D-118 Auftragskonditionen**

In diesem Dialog hinterlegen Sie auftragsbezogene Preise und Konditionen. Sie können verschiedene Kriterien der Preisberechnung für die folgenden Komponenten festlegen:

- Glasarten
- Sprossen
- Farbartikel
- Zubehör
- Bearbeitungen
- Verglasungen

Die Werte geben Sie für Verkaufs- und Einkaufspreise getrennt an. Die Register **Verkauf** und **Einkauf** sind analog aufgebaut. Abweichungen werden im Folgenden explizit beschrieben.

#### Kopfbereich

**Auftrag** Nummer des gewählten Auftrags.
**Technische Info:** Anzeigefeld, DB-Feld: kauf.auftrnr

**Kond-Debitor** Kundennummer des Kunden, für den die Konditionen gelten. Wenn Sie ohne Konditionsdebitor arbeiten wollen, müssen Sie die Meldung, die beim Verlassen des Felds angezeigt wird mit [Ja] bestätigen. Das Feld wird nur angezeigt, wenn das Register Verkauf geöffnet ist.
**Technische Info:** numerisches Feld, DB-Feld: aufkond.kalkkunr

#### Verkauf und Einkauf

In diesem Register werden die Verkaufs- oder Einkaufspreise für die verschiedenen Preismethoden angezeigt.

**ISO, ESG, VSG, Basisglas, Veredelung, Farbartikel, Preise allg.** Die Werte gelten für die Artikel, denen die jeweilige Preismethode zugewiesen ist.
⇨ Preise und Konditionen, "Preismethoden" auf Seite C-567

**Sprossen** Die Werte gelten für Artikel, denen die Preismethode Sprossenpreise zugewiesen ist. Für Sprossen können keine Staffelstufen angegeben werden.

Sie können für jede Artikelgruppe verschiedene Berechnungskriterien angeben:

- **PKZ:** Preiskennzeichen, mit dem die Preise ermittelt werden. Das PKZ verweist auf eine Preisliste, in der die Preise für die Artikel mit den jeweiligen Preismethoden definiert sind.
    - **Technische Info:** numerische Felder, DB-Felder: aufkond.isopkz, aufkond.pkzesgpkz, aufkond.pkzvsgpkz, aufkond.pkzbaspkz, aufkond.pkzverpkz, aufkond.pkzfarbpkz, aufkond.pkzallpkz, aufkond.sprospkz
- **TZ:** Teuerungszuschlag in Prozent. Der Teuerungszuschlag wird auf den Mengeneinheitspreis aufgeschlagen. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
    - **Technische Info:** numerische Felder, DB-Felder: aufkond.isotz, aufkond.pkzesgtz, aufkond.pkzvsgtz, aufkond.pkzbastz, aufkond.pkzvertz, aufkond.pkzfarbtz, aufkond.pkzalltz, aufkond.vksprtz
- **Faktor:** Faktor des Preiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
    - **Technische Info:** numerische Felder, DB-Felder: aufkond.isofaktor, aufkond.pkzesgfakt, aufkond.pkzvsgfakt, aufkond.pkzbasfakt, aufkond.pkzverfakt, aufkond.pkzfarbfakt, aufkond.pkzallfakt, aufkond.sprosfakt
- **Stufe:** Angabe der Preis-Staffelstufe, aus der der Preis für die jeweilige Glasart bzw. Preismethode ermittelt wird.
    - **Technische Info:** numerische Felder, DB-Felder: aufkond.pkzesgstaff, aufkond.pkzvsgstaff, aufkond.pkzbasstaff, aufkond.pkzverstaff, aufkond.pkzfarbstaff, aufkond.pkzallstaff
- **Art:** Auswahl der Berechnungsart, nach der die Sprossenpreise berechnet werden. Die Berechnungsarten sind zum Register Positionskonditionen – Sprossenpreise beschrieben:
    - ⇨ "Positionskonditionen - Sprossenpreise" auf Seite D-1369
    - **Technische Info:** numerisches Feld, DB-Feld: aufkond.sprosart
- **Sonderzuschlag:** Preiszuschlag für Sonderanfertigungen. Im zweiten Feld geben Sie den Preistyp an. Der Preistyp bestimmt, worauf sich der Preis bezieht:
    - **WE/Stück:** Der Preis gilt pro Stück.
    - **WE/qm:** Der Preis gilt pro Quadratmeter
    - **Prozent:** Der Preis wird als Prozentsatz auf den Grundpreis berechnet.
    Diese Felder werden nur im Register Verkauf angezeigt.
    - **Technische Info:** numerische Feld, Toggle-Feld, DB-Felder: aufkond.isosonderzu, aufkond.isosonderzutyp
- **Gesamtzu.:** Prozentualer Zuschlag, der auf den Gesamtpreis aufgeschlagen wird. Dieses Feld wird nur im Register Verkauf angezeigt.
    - **Technische Info:** numerische Felder, DB-Felder: aufkond.isozuschlag, aufkond.pkzesggeszu, aufkond.pkzvsggeszu, aufkond.pkzbastgeszu, aufkond.pkzvergeszu, aufkond.pkzfarbgeszu, aufkond.pkzallgeszu

#### Teuerungszuschlag und Faktor

Zusätzlich können Sie Teuerungszuschläge und Faktoren für einzelne Komponenten angeben. Im ersten Feld geben Sie jeweils den Teuerungszuschlag und im zweiten Feld den Faktor an.

**Zubehör TZ Faktor** Prozentualer Teuerungszuschlag und Faktor für Zubehörartikel. Die Felder werden in den Registern Verkauf und Einkauf angezeigt.
**Technische Info:** numerische Felder, DB-Felder: aufkond.zubetz, aukond.zubef, aufkond.ekzubetz, aukond.ekzubef

#### Bearbeitungen (Register Verkauf)

Im Register Verkauf können Sie für Teuerungszuschlag und Faktor unterschiedliche Werte für die jeweilige Eck-, Kanten- oder Flächenbearbeitung von ESG und Basisglas angeben.

**ESG TZ Faktor** Teuerungszuschlag und Faktor für Bearbeitungen in Einscheiben-Sicherheitsglas.

**Basisglas TZ Faktor** Teuerungszuschlag und Faktor für Bearbeitungen in Basis-Glas.

Sie können den Teuerungszuschlag und den Faktor für verschiedene Bearbeitungen angeben. Der Teuerungszuschlag wird in der Preisberechnung berücksichtigt.
- **Ecken:** Eckbearbeitungen, z. B. Eckabschnitt.
    - **Technische Info:** numerische Felder, DB-Felder: aufkond.esgbecktz, esgbeckf, verbecktz, verbeckf
- **Kanten:** Kantenbearbeitungen, z. B. Polieren.
    - **Technische Info:** numerische Felder, DB-Felder: aufkond.esgbkantz, esgbkanf, verbkantz, verbkanf
- **Fläche:** Flächenbearbeitungen, z. B. Beschichtung.
    - **Technische Info:** numerische Felder, DB-Felder: aufkond.esgbflatz, esgbflaf, verbflatz, verbflaf

#### Bearbeitungen (Register Einkauf)

Im Register Einkauf können Sie für Teuerungszuschlag und Faktor unterschiedliche Werte für die Bearbeitung von ESG und Basisglas angeben.

**ESG TZ Faktor** Teuerungszuschlag und Faktor für Bearbeitungen in Einscheiben-Sicherheitsglas.
**Technische Info:** numerische Felder, DB-Felder: aufkond.ekesgbtz, ekesgbfakt

**Basisglas TZ Faktor** Teuerungszuschlag und Faktor für Bearbeitungen in Basis-Glas.
**Technische Info:** numerische Felder, DB-Felder: aufkond.ekeverbtz, ekverbfakt

#### Sonderkosten

**Verglasungspreis** Preis der Verglasungsarbeit in der Währungseinheit.
**Technische Info:** numerisches Feld, DB-Feld: aufkond.verglaseins, aufkond.verglaseinsek

**Versiegelungspreis** Preis der Versiegelungsarbeit in der Währungseinheit.
**Technische Info:** numerisches Feld, DB-Feld: aufkond.verglasversieg, aufkond.verglasversiegek

**Min. Preis einsetzen** Mindestpreis der Verglasungs- oder Versiegelungsarbeiten.
**Technische Info:** numerisches Feld, DB-Feld: aufkond.verglasmineins, aufkond.verglasmineinsek

**Stückpreisrundung** Angabe, wie der Stückpreis gerundet werden soll.
- Wenn 100 angegeben ist, wird der Preis auf den nächsten vollen Währungsbetrag gerundet.
- Wenn 10 angegeben ist, wird der Preis auf den nächsten Zehntelbetrag gerundet.
**Technische Info:** numerische Felder, DB-Felder: aufkond.stkprsrund, aufkond.ekstkprsrund

**SZR-Zuschlag** Angabe, ob für den Scheibenzwischenraum ein Preiszuschlag berechnet werden soll:
- **J:** Der SZR-Zuschlag wird erhoben, wenn der SZR die im zugeordneten ISO-Artikel angegebenen Millimeter-Staffeln unterschreitet.
    ⇨ Preise und Konditionen, "SZR-Zuschläge" auf Seite C-743
- **N:** Der SZR-Zuschlag wird nicht erhoben.
Dieses Feld wird nur im Register Verkauf angezeigt.
**Technische Info:** Toggle-Feld, DB-Feld: aufkond.szrflag

**Stufenzuschlag** Preiszuschlag für die Stufenbearbeitung. Im zweiten Feld geben Sie den Zuschlagstyp an. Der Zuschlagstyp gibt an, worauf sich der Zuschlag bezieht:
- **WE/St ne:** Der Stufenzuschlag wird nach Berechnung des Faktors als fester Nettobetrag pro Stufe aufgeschlagen.
- **WE/St br:** Der Stufenzuschlag wird vor Berechnung des Faktors als fester Bruttobetrag pro Stufe aufgeschlagen.
- **Prozent:** Der Stufenzuschlag wird als prozentual auf den Glasmengeneinheitspreis und die Austauschpreise aufgeschlagen.
- **%/Stück:** Der Stufenzuschlag wird pro Stufe prozentual auf den Glasmengeneinheitspreis und die Austauschpreise aufgeschlagen.
**Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: aufkond.stufzuvk, aufkond.stufzutypvk, aufkond.stufzuek, aufkond.stufzutypek

**Minber. ESG/VSG in ISO** Mindestberechnung für ESG- oder VSG-Glas in ISO-Glasscheiben. In das erste Feld wird der Wert für das ESG-Glas, in das zweite Feld der Wert für das VSG-Glas eingetragen. Dieses Feld wird nur im Register Verkauf angezeigt.
**Technische Info:** numerische Felder, DB-Felder: aufkond.minesginiso, aufkond.minvsginiso

**Mindestberechnung** Anzahl der Mengeneinheiten in Stück, Quadratmeter usw., für die der Preis berechnet wird. Wenn die Menge in der Auftragsposition kleiner ist als die Mindestmenge, wird der Preis für diese Mindestmenge berechnet. Dieses Feld wird nur im Register Verkauf angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: aufkond.minber

**Maßrundung** Angabe der Maßrundung in Millimeter für die Preisberechnung des Artikels. Für die Preisberechnung werden die Kantenlängen in der Auftragsposition auf den nächsthöheren Wert in Millimeter aufgerundet, der durch die angegebene Maßrundung teilbar ist. In der Produktion werden diese Angaben nicht berücksichtigt. Dieses Feld wird nur im Register Verkauf angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: aufkond.massrund

### Auftragspreise

**Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > `<F4>` > Preisangaben > Auftragspreise > Artikelpreise**

**Abb. D-119 Auftragspreise**

In diesem Dialog hinterlegen oder ändern Sie die Artikelpreise auftragsbezogen. Wenn Sie z. B. Artikel durch einen Mengenrabatt günstiger einkaufen als zu den hinterlegten Preisen in den Stammdaten, müssen die Preise manuell für den Auftrag geändert werden, damit die korrekte Gewinnspanne berechnet werden kann.

- **Konditionsart:** Art der gewährten Sonderkondition:
    - **Kunde:** Der Preis für den ausgewählten Artikel wird nach den kundenspezifischen Konditionen berechnet.
- **Materialkosten:** Auf den ausgewählten Artikel werden die angegebenen Materialkosten gerechnet.
    - **Technische Info:** Pflichtfeld, Toggle-Feld, DB-Feld: aufpreise.kondkz
- **Artikel, Bezeichnung:** Artikelnummer und Bezeichnung des Artikels, für den die Sonderkondition gilt.
    - **Technische Info:** Pflichtfeld, numerisches Feld, alphanumerisches Feld, DB-Felder: aufpreise.artnr, artikel.artbez1
- **Preis:** Preis des Artikels.
    - **Technische Info:** numerisches Feld, DB-Feld: aufpreise.preis
- **Preistyp:** Angabe, worauf sich der Preis bezieht:
    - **WE/Stück:** Der Preis wird pro Stück berechnet.
    - **WE/GME:** Der Preis wird pro Grundmengeneinheit berechnet, z. B. pro Quadratmeter.
    - **Technische Info:** Toggle-Feld, DB-Feld: aufpreise.preistyp
- **Faktor:** Faktor des Preiszuschlags in Prozent. In der Regel wird mit einem Faktor ein Rabatt gewährt.
    - **Technische Info:** numerisches Feld, DB-Feld: aufpreise.faktor

Mit `<F2>` wechseln Sie in die Detailansicht.
Die meisten Felder in der Detailansicht entsprechen den Spalten in der Übersicht. Zusätzlich werden folgende Felder angezeigt:

**Mindestberechnung** Anzahl der Mengeneinheiten in Stück, Quadratmeter usw., für die der Preis berechnet wird. Wenn die Menge in der Auftragsposition kleiner ist als die Mindestmenge, wird der Preis für diese Mindestmenge berechnet.
**Technische Info:** numerisches Feld, DB-Feld: aufpreise.minber

**Maßrundung** Angabe der Maßrundung in Millimeter für die Preisberechnung des Artikels. Für die Preisberechnung werden die Kantenlängen in der Auftragsposition auf den nächsthöheren Wert in Millimeter aufgerundet, der durch die angegebene Maßrundung teilbar ist. In der Produktion werden diese Angaben nicht berücksichtigt.
**Technische Info:** numerisches Feld, DB-Feld: aufpreise.massrund

**Min.Kantenlänge** Angabe der Kantenlänge in Millimeter für die Preisberechnung. Diese Größe wird herangezogen, wenn die Höhe oder Breite des Glases in der Auftragsposition kleiner ist als diese Mindestkantenlänge.
**Technische Info:** numerisches Feld, DB-Feld: aufpreise.minkant

Die Artikelpreise sind ausführlich zum Part Preise und Konditionen beschrieben:
⇨ Preise und Konditionen, "Artikelpreise" auf Seite C-906

### Auftragssprossenpreise

**Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > `<F4>` > Preisangaben > Auftragspreise > Sprossenpreise**

**Abb. D-120 Auftragssprossenpreise**

In diesem Dialog hinterlegen oder ändern Sie die Sprossenpreise auftragsbezogen.

- **Artikel:** Artikelnummer.
    **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: aufspropr.artnr
- **Berechnungsart:** Auswahl der Berechnungsart, nach der die Sprossenpreise berechnet werden:
    - **1 - Felder:** Der Preis wird pro Feld berechnet.
    - **2 - LM+K+R:** Der Preis wird pro laufendem Meter, pro Kreuz und pro Randanschluss berechnet.
    - **3 - LM:** Der Preis wird pro laufendem Meter berechnet.
    - **4 - LM+K:** Der Preis wird pro laufendem Meter und pro Kreuz berechnet.
    - **5 - LM+R:** Der Preis wird pro laufendem Meter und pro Randanschluss berechnet.
    - **6 - K:** Der Preis wird pro Kreuz berechnet.
    - **7 - K+R:** Der Preis wird pro Kreuz und pro Randanschluss berechnet.
    - **8 - R:** Der Preis wird pro Randanschluss berechnet.
    - **9 - Spezial:** Diese Form der Berechnung ist kundenindividuell konfiguriert.
    - **10 - Prozent:** Der Preis wird prozentual aus dem Grundpreis des Kopfartikels berechnet. Der Prozentsatz wird in der Detailansicht im Feld **Prozent** angegeben.
    - **11 - qm-Preis:** Der Preis wird pro Quadratmeter des Glases berechnet. Der Preis wird in der Detailansicht im Feld **Qm-Preis** angegeben.
    - **12 - Feld+LM:** Der Preis wird pro Feld und pro laufendem Meter berechnet.
    - **13 - Stück:** Für den Sprossenaufbau wird ein Gesamtpreis berechnet. Der Preis wird in der Detailansicht im Feld **Stückpreis** angegeben.
    - **14 - K oder LM:** Der Preis wird pro Kreuz oder pro laufendem Meter berechnet.
        - Wenn sich im Sprossenaufbau Kreuzungspunkte ergeben, werden die Sprossen nach Anzahl der Kreuze berechnet.
        - Wenn keine Kreuzungspunkte vorhanden sind, werden die Sprossen nach laufenden Metern berechnet.
    - **15 - Feld+K+R:** Der Preis wird pro Feld, pro Kreuz und pro Randanschluss berechnet.
    **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: aufspropr.berart

Die folgenden Felder werden nur je nach Berechnungsart berücksichtigt:
- **Laufmeter:** Angabe des Preises pro laufendem Meter. Der Preis wird bei den Berechnungsarten LM, LM+K+R, LM+K, LM+R, Feld+LM und Spezial ausgewertet.
    **Technische Info:** numerisches Feld, DB-Feld: aufspropr.plm
- **Kreuz:** Angabe des Preises pro Kreuzungspunkt. Der Preis wird bei den Berechnungsarten K, K+R, LM+K, LM+K+R, K oder LM, Feld+K+R und Spezial ausgewertet.
    **Technische Info:** numerisches Feld, DB-Feld: aufspropr.pkr
- **Rand:** Angabe des Preises pro Randstopfen. Der Preis wird bei den Berechnungsarten R, LM+K+R, LM+R, K+R, Feld+K+R und Spezial ausgewertet.
    **Technische Info:** numerisches Feld, DB-Feld: aufspropr.pra
- **Felder:** Angabe des Preises pro Feld. Der Preis wird bei den Berechnungsarten Felder, Feld +LM, Feld+K+R und Spezial ausgewertet.
    **Technische Info:** numerisches Feld, DB-Feld: aufspropr.pfe

Mit `<F2>` wechseln Sie in die Detailansicht.
Die meisten Felder in der Detailansicht entsprechen den Spalten in der Übersicht. Zusätzlich werden folgende Felder angezeigt:

**Felder2** Angabe des Preises pro Feld, wenn im Sprossenaufbau keine Kreuzungspunkte vorhanden sind. Der Preis wird bei der Berechnungsart Spezial ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: aufspropr.pfe2

**Prozent** Angabe des Prozentsatzes. Der Preis wird bei den Berechnungsarten Prozent und Spezial ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: aufspropr.prozent

**Quadratmeter** Angabe des Quadratmeterpreises. Der Preis wird bei der Berechnungsart qm-Preis ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: aufspropr.qmpreis

**Stückpreis** Angabe des Stückpreises. Der Preis wird bei der Berechnungsart Stück ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: aufspropr.stckpreis

**Mindestlaufmeter** Angabe der Sprossenlänge in Meter, für die der Preis mindestens berechnet wird. Der Preis wird bei der Berechnungsart LM ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: aufspropr.minlm

**Mindestfeldanzahl** Angabe der Sprossenfelder, für die der Preis mindestens berechnet wird. Der Preis wird bei der Berechnungsart Felder ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: aufspropr.minfeld

**Faktor** Faktor des Preiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerisches Feld, DB-Feld: aufspropr.faktor

Eine ausführliche Beschreibung der Sprossenpreise finden Sie im Part Preise und Konditionen:
⇨ Preise und Konditionen, "Sprossenpreise" auf Seite C-925

### Auftragsaustauschpreise

**Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > `<F4>` > Preisangaben > Auftragspreise > Austauschpreise**

**Abb. D-121 Auftragsaustauschpreise**

In diesem Dialog hinterlegen oder bearbeiten Sie auftragsbezogen die Preise für Artikel, die innerhalb der Stückliste ausgetauscht oder hinzugefügt wurden.

- **Typ:** Produktyp des Artikels dessen Preis ausgetauscht wird.
    - **ISO-Austausch:** Der Austauschpreis wird herangezogen, wenn der Artikel in einem Isolier-Glas ausgetauscht wird.
    - **VSG-Aust./-Zusatz:** Der Austauschpreis wird herangezogen, wenn der Artikel in einem Verbund-Sicherheitsglas ausgetauscht oder zusätzlich erfasst wird.
    - **VSG-Austausch:** Der Austauschpreis wird herangezogen, wenn der Artikel in einem Verbund-Sicherheitsglas ausgetauscht wird.
    - **VSG-Zusatz:** Der Austauschpreis wird herangezogen, wenn der Artikel in einem Verbund-Sicherheitsglas zusätzlich erfasst wird.
    **Technische Info:** Toggle-Feld, DB-Feld: aufaustpr.austkz
- **Artikel, Bezeichnung:** Nummer und Bezeichnung des Artikels. Wenn Sie eine Nummer angeben, wird die Bezeichnung im Klartext angezeigt.
    **Technische Info:** Pflichtfeld, numerisches Feld, Anzeigefeld, DB-Felder: aufaustpr.artnr, artikel.artbez1
- **Preis:** Preis des Austauschglases.
    **Technische Info:** numerisches Feld, DB-Feld: aufaustpr.preis
- **Preistyp:** Angabe, worauf sich der Preis bezieht.
    - **WE/qm:** Der Preis gilt pro Quadratmeter.
    - **Prozent:** Der Zuschlag wird als Prozentwert auf den Glasgrundpreis berechnet.
    **Technische Info:** Toggle-Feld, DB-Feld: aufaustpr.preistyp

Mit `<F2>` wechseln Sie in die Detailansicht.
Die meisten Felder in der Detailansicht entsprechen den Spalten in der Übersicht. Zusätzlich werden folgende Felder angezeigt:

**Faktor** Faktor des Preiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerisches Feld, DB-Feld: aufaustpr.faktor

**Mindestberechnung** Angabe der Mindestfläche in Quadratmeter, für die der Preis berechnet wird. Wenn die Fläche des Austauschglases in der Auftragsposition kleiner ist als die Mindestberechnungsfläche, wird der Preis für diese Mindestberechnungsfläche berechnet.
**Technische Info:** numerisches Feld, DB-Feld: aufaustpr.minber

**Maßrundung** Angabe der Maßrundung in Millimeter für die Preisberechnung des Artikels. Für die Preisberechnung werden die Kantenlängen in der Auftragsposition auf den nächsthöheren Wert in Millimeter aufgerundet, der durch die angegebene Maßrundung teilbar ist. In der Produktion werden diese Angaben nicht berücksichtigt.
**Technische Info:** numerisches Feld, DB-Feld: aufaustpr.massrund

Eine ausführliche Beschreibung der Austausch- und Zusatzpreise finden Sie im Part Preise und Konditionen:
⇨ Preise und Konditionen, “ISO-Austauschpreise" auf Seite C-937
⇨ Preise und Konditionen, "Spezielle VSG-Austausch-/Zusatzpreise" auf Seite C-970

### Auftragsunterteilpreise

**Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > `<F4>` > Preisangaben > Auftragspreise > Unterteilpreise**

**Abb. D-122 Auftragsunterteilpreise**

In diesem Dialog hinterlegen oder ändern Sie den Preis für Unterteile auftragsbezogen.

- **Artikel, Bezeichnung:** Nummer und Bezeichnung des Artikels.
    **Technische Info:** Pflichtfeld, numerisches Feld, Anzeigefeld, DB-Felder: aufuteilpr.artnr, artikel.artbez1
- **Preis:** Preis des Unterteils.
    **Technische Info:** numerisches Feld, DB-Feld: aufuteilpr.preis
- **Preistyp:** Angabe, worauf sich der Preis bezieht.
    - **WE/Stück:** Der Preis gilt pro Stück.
    - **WE/GME:** Der Preis gilt pro Grundmengeneinheit, z. B. pro Quadratmeter.
    **Technische Info:** Toggle-Feld, DB-Feld: aufuteilpr.preistyp

Mit `<F2>` wechseln Sie in die Detailansicht.
Die meisten Felder in der Detailansicht entsprechen den Spalten in der Übersicht. Zusätzlich werden folgende Felder angezeigt:

**Faktor** Faktor des Preiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerisches Feld, DB-Feld: aufuteilpr.faktor

**Mindestberechnung** Anzahl der Mengeneinheiten in Stück, Quadratmeter usw., für die der Preis berechnet wird. Wenn die Menge der Unterteile in der Auftragsposition kleiner ist als die Mindestmenge, wird der Preis für diese Mindestmenge berechnet.
**Technische Info:** numerisches Feld, DB-Feld: aufuteilpr.minber

**Maßrundung** Angabe der Maßrundung in Millimeter für die Preisberechnung des Artikels. Für die Preisberechnung werden die Kantenlängen in der Auftragsposition auf den nächsthöheren Wert in Millimeter aufgerundet, der durch die angegebene Maßrundung teilbar ist. In der Produktion werden diese Angaben nicht berücksichtigt.
**Technische Info:** numerisches Feld, DB-Feld: aufuteilpr.massrund

### Nachkalkulation

**Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > `<F4>` > Preisangaben > Teilkalkulation**

**Abb. D-123 Nachkalkulation**

In diesem Dialog hinterlegen Sie auftragsbezogen Konditionen für die Verkaufs- und Einkaufspreise.
- Mit `<F3>` können Sie die Preise mit den neuen Konditionen berechnen lassen. Die Werte der Nachkalkulation werden in die Positionskonditionen übernommen.

Wenn Sie die Werte bearbeiten, werden diese in die entsprechenden Preiskonditionen übernommen. Die technische Information und der Datenbankbezug der Felder entspricht den jeweiligen Preiskonditionen.
⇨ "Positionskonditionen" auf Seite D-1340

#### Kopfbereich

**Stückliste** Nummer der Stückliste, für die die Konditionen festgelegt werden sollen.
**Technische Info:** numerisches Feld, DB-Feld: kpos.poskonr

**Konditionen holen** Angabe, ob die Konditionen zur Preisermittlung aus den Stammdaten gezogen werden sollen.
- **J:** Die Konditionen aus den Stammdaten werden zur Preisermittlung herangezogen. Die angegebenen Werte im Rumpfbereich werden von den Werten aus den Stammdaten überschrieben, falls der entsprechende Wert in den Stammdaten hinterlegt wurde.
- **N:** Die Konditionen aus den Stammdaten werden nicht herangezogen. Sie können die Konditionen auftragsbezogen im Rumpfbereich angeben.
**Technische Info:** Toggle-Feld

#### Verkauf und Einkauf

Sie können für die folgenden Felder jeweils einen Wert für den Verkauf und einen Wert für den Einkauf angeben.

**Grundpreis** Grundpreis des Artikels. Im zweiten Feld geben Sie den Preistyp an. Der Preistyp bestimmt, worauf sich der Preis bezieht:
- **WE/Stück:** Der Preis gilt pro Stück.
- **WE/GME:** Der Preis gilt pro Grundmengeneinheit, z. B. pro Quadratmeter.
**Technische Info:** numerisches Feld

**Faktor** Faktor des Preiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerisches Feld

**TZ** Teuerungszuschlag in Prozent. Der Teuerungszuschlag wird auf den Mengeneinheitspreis aufgeschlagen. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
**Technische Info:** numerisches Feld

**Bearbeitungs-Faktor** Faktor für Bearbeitungen in Prozent.
**Technische Info:** numerisches Feld

**Bearbeitungs-TZ** Teuerungszuschlag für Bearbeitungen in Prozent.
**Technische Info:** numerisches Feld

**Zubehör-Faktor** Faktor für Zubehörartikel in Prozent.
**Technische Info:** numerisches Feld

**Zubehör TZ** Teuerungszuschlag für Zubehörartikel in Prozent.
**Technische Info:** numerisches Feld

**Sprossen-TZ** Teuerungszuschlag für Sprossenartikel in Prozent.
**Technische Info:** numerisches Feld

**Sprossenberechnungsart** Auswahl der Berechnungsart, nach der die Sprossenpreise berechnet werden. Die Berechnungsarten sind zum Register Positionskonditionen – Sprossenpreise beschrieben.
⇨ "Positionskonditionen - Sprossenpreise" auf Seite D-1369
**Technische Info:** numerisches Feld

**Verglasungspreis** Preis der Verglasung pro Quadratmeter.
**Technische Info:** numerisches Feld

**Mindestpreis Verglasung** Preis, der mindestens für die Verglasung berechnet wird. Wenn im Auftrag bei einem Artikel der Preis der Verglasung kleiner ist als der angegebene Mindestpreis, wird dieser Mindestpreis berechnet.
**Technische Info:** numerisches Feld

**Versiegelungspreis** Preis der Versiegelung pro Quadratmeter.
**Technische Info:** numerisches Feld

**Mindestpreis Versiegelung** Preis, der mindestens für die Versiegelung berechnet wird. Wenn im Auftrag bei einem Artikel der Preis der Versiegelung kleiner ist als der angegebene Mindestpreis, wird dieser Mindestpreis berechnet.
**Technische Info:** numerisches Feld

#### Austausch

- **ISO_Austausch, Bezeichnung:** Nummer und Bezeichnung des Austauschartikels.
    **Technische Info:** Pflichtfeld, numerisches Feld, Anzeigefeld
- **VK-Faktor:** Faktor für den Verkaufspreis des Preiszuschlags in Prozent.
    **Technische Info:** numerisches Feld
- **VK-Preis:** Verkaufspreis des Artikels in Prozent.
    **Technische Info:** numerisches Feld
- **EK-Faktor:** Faktor für den Einkaufspreis des Preiszuschlags in Prozent.
    **Technische Info:** numerisches Feld
- **EK-Preis:** Einkaufspreis des Artikels.
    **Technische Info:** numerisches Feld

### Stufenpreise

**Verkauf > Auftragserfassung > Register Positionen > gestuften Artikel erfassen > Preisfeld > `<Shift>` + `<F9>` > `<F8>`**

**Abb. D-124 Stufenpreise**

In diesem Dialog geben Sie gestaffelte Preise für einen Stufenartikel an, z. B. für ISO-Artikel.

- **VK/EK:** Die Eingaben gelten für Einkauf oder Verkauf.
- **ab Stufenbreite (mm):** Wert der Stufenbreite in Millimeter, z. B. ab einer Stufenbreite von 100 mm 3,50 € und ab einer Stufenbreite von 200 mm 7,80 €.
- **Anzahl:** Anzahl der Stufen zur Berechnung.
- **Zuschlag:** Wert des Stufenzuschlags in Währungseinheiten, z. B. in Euro.
- **Zuschlagstyp:** Berechnungsart des gestaffelten Preiszuschlags für Stufen.
    - **WE/Stück:** Preis (Währungseinheit) zur Staffelung der Stufenbreite wird mit der Stückzahl der Stufen und dem Wert im Feld Zuschlag multipliziert. Dieser Wert wird zum Glaspreis addiert.
    - **WE/Stück/qm netto:** Staffelung der Stufenbreite wird mit der Stückzahl der Stufen und dem Wert im Feld Zuschlag multipliziert. Das Ergebnis wird mit der Fläche des umschriebenen Rechtecks des Artikels multipliziert und zum Stückpreis addiert.

### Positionskonditionen

**Verkauf > Auftragserfassung > Register Positionen > Preisfeld > `<Shift>` + `<F9>`**

In diesen Dialogen werden die Preiskonditionen eines Positionsartikels angezeigt.

Die Dialoge sind in zwei Register oder Bereiche aufgeteilt, die die Preiskonditionen für **Verkauf** und **Einkauf** anzeigen. Das Register Einkauf ist nur aktiv, wenn die Beschaffungsart Bestellung oder Mitgelief. für die Position gewählt ist. Der Aufbau der Register und Bereiche unterscheidet sich, je nachdem welche Preismethode dem Positionsartikel zugeordnet ist. Es werden die Werte angezeigt, die für die Preisberechnung relevant sind.

Die einzelnen Preismethoden sind zu dem Part Preise und Konditionen beschrieben:
⇨ Preise und Konditionen, "Preismethoden" auf Seite C-567

Sie können die Werte für die Preiskonditionen bearbeiten. Wenn Sie den Preis neu berechnen lassen möchten, schließen Sie den Dialog. Eine Abfrage wird angezeigt, ob Sie den Preis neu berechnen lassen möchten. Wenn Sie die Abfrage bestätigen, werden die Preise mit den vorgangsbezogenen Positionskonditionen berechnet.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG" auf Seite D-1341
- "Konditionen für PKZ-VSG, PKZ-ESG" auf Seite D-1345
- "Konditionen ISO" auf Seite D-1347
- "Konditionen für ISO (SCHWEIZ)" auf Seite D-1352
- "Konditionen für PKZ-FARBARTIKEL" auf Seite D-1356
- "Konditionen für PKZ-PREISE-ALLGEMEIN" auf Seite D-1357
- "Konditionen für PKZ-GLASTÜREN" auf Seite D-1359
- "Konditionen für Manuelle Preise" auf Seite D-1362
- "VSG-Austausch-/Zusatzpreise" auf Seite D-1363

Je nachdem, welche preisrelevanten Bearbeitungen in der Stückliste der Position enthalten sind, werden die Register Bearbeitungspreise (VK), (EK) und Sprossenpreise aktiv. Die Preiseigenschaften für Bearbeitungspreise werden in den Stammdaten festgelegt.
⇨ Stammdaten, "Preiseigenschaften" auf Seite B-449

Die Register Bearbeitungspreise (VK), (EK) und Sprossenpreise werden separat beschrieben.

In diesem Abschnitt sind zusätzlich folgende Register erklärt:
- "Positionskonditionen - Bearbeitungspreise" auf Seite D-1366
- "Positionskonditionen – Sprossenpreise" auf Seite D-1369

### Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG

**Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Preismethode PKZ-Basisglas, PKZ-Veredelung > `<Shift>` + `<F9>`**

**Abb. D-125 Konditionen PKZ-BASISGLAS, PKZ-VEREDELUNG**

In diesem Dialog werden die Preiskonditionen eines Positionsartikels angezeigt, dem die Preismethode PKZ-Basisglas oder PKZ-Veredelung zugeordnet ist. Sie können die Preiskonditionen bearbeiten.

In den Dialogen Konditionen PKZ-BASISGLAS und Konditionen PKZ-VEREDELUNG sind die Register Verkauf und Einkauf weitgehend analog aufgebaut. Das Feld Gesamtzuschlag wird im Register Einkauf nicht angezeigt.

Wenn Zusatz-Bearbeitungen in der Stückliste der Position enthalten sind, dann sind die Register Bearbeitungspreise (VK), (EK) aktiv:
⇨ "Positionskonditionen - Bearbeitungspreise" auf Seite D-1366

Wenn Sprossen in der Stückliste der Position enthalten sind, dann ist das Register Sprossenpreise aktiv:
⇨ "Positionskonditionen - Sprossenpreise" auf Seite D-1369

#### Kopfbereich

**VK-PKZ** Preiskennzeichen der vordefinierten Preisliste für den Verkauf.
**Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.pkz

**EK-PKZ** Preiskennzeichen der vordefinierten Preisliste für den Einkauf.
**Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.ekpkz

**Vektor** Nummer des Vektors, aus dem der Preis gezogen werden soll.
**Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.matnr

#### Register Verkauf, Einkauf

**Preisart** Art der Preisberechnung. Standardmäßig ist die Preisart **Einzelpreis** ausgewählt. Das Feld ist ein Anzeigefeld. Wenn Sie den Glas- oder Grundpreis ändern oder den Preis in der Position manuell eingeben, ohne eine Preisberechnung durchzuführen, dann wird als Preisart **manueller Preis** angezeigt.
**Technische Info:** Anzeigefeld, DB-Feld: pokokon.flag6

**Staffelstufe** Preisstufe, aus der der Preis verwendet wird. Das Feld wird von der Preisberechnung nur ausgewertet, wenn für den relevanten Artikelpreisvektor die Preisart **2 - Staffelstufe** angegeben ist.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.flag1, pokokon.ekflag1

**Preistyp** Anzeige, worauf sich der angegebene Preis bezieht.
- **WE/Stück:** Der Preis gilt pro Stück.
- **WE/GME:** Der Preis gilt pro Grundmengeneinheit, z. B. pro Quadratmeter.
**Technische Info:** Toggle-Feld, Anzeigefeld

**Glaspreis** Grundpreis einer Glasscheibe. Der Preistyp wird aus dem vorherigen Feld herangezogen.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu1, pokokon.zuk1

**Modellzuschlag** Preiszuschlag, der bei Modellen erhoben wird. Sie können den Wert in Prozent oder als Betrag mit Währungseinheit angeben. Als Zuschlag wird immer der höhere Wert herangezogen.
**Technische Info:** numerische Felder, DB-Felder: pokokon.zu2, pokokon.zuk2

**TZ** Prozentualer Teuerungszuschlag, der auf den Mengeneinheitspreis aufgeschlagen wird. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu3, pokokon.zuk3

**Faktor** Faktor des Preiszuschlags in Prozent.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu4, pokokon.zuk4

**Gesamtzuschlag** Preiszuschlag für die Position in Prozent.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu26, pokokon.zuk26

**Maßrundung** Maßrundung in Millimeter.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu5, pokokon.zuk5

**Mindestberechnung** Mindestfläche in Quadratmeter.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu6, pokokon.zuk6

**Gebindegröße** Fassungsvermögen des Gebindes in Mengeneinheiten.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu8, pokokon.zuk8

**Stückpreisrundung** Ab- oder Aufrundung für den Stückpreis einer Position.
**Technische Info:** numerisches Feld, DB-Feld: pokokonp.vkstkprsrund, pokokonp.ekstkprsrund

**Zuschlagsart** Die Zuschlagsart gibt an, wonach der Zuschlag gestaffelt und wie der Zuschlag ermittelt wird:
- **Fläche:** Der Zuschlag gilt jeweils ab den angegebenen Flächen.
- **Längere Kante:** Der Zuschlag gilt jeweils für die längere Kante.
- **Seitenverhältnis:** Der Zuschlag gilt ab dem angegebenen Seitenverhältnis.
- **Übermaßzuschlag:** Der Zuschlag gilt ab der angegebenen Größe, z. B. Kantenlänge.
**Technische Info:** Toggle-Feld, Anzeigefeld

**Zuschlag** Zuschlag, der auf den Preis erhoben wird. Es ist von der Konfiguration abhängig, ob der Zuschlag auf den Glasgrund-, den Grundmengen- oder den Stückpreis erhoben wird.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu24, pokokon.zuk24

**Abschlag pro Stück** Angabe des Abschlags.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu25, pokokon.zuk25

**Mindestpreis** Mindestpreis für die Glasscheibe.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu20, pokokon.zuk20

#### Größenzuschläge

In diesem Bereich werden die Werte für Preiszuschläge und den Zuschlagstyp angezeigt. Sie können die Werte bearbeiten. Der Zuschlagstyp gibt an, worauf sich der Zuschlag bezieht:
- **WE Wert:** Der Zu- oder Abschlag wird als fester Betrag auf den Artikelpreis berechnet. Wenn der Zuschlag im Auftrag als fester Betrag erhoben wird, gilt die Währung des für den Kopfartikel ermittelten PLKZ. Die Währung wird nicht umgerechnet.
- **Prozent:** Der Zuschlag wird prozentual aus dem Grundpreis des Kopfartikels berechnet. Dieser Zuschlagstyp wird nur bei Austauschartikeln oder Bearbeitungen gewählt.

**Kleinglaszuschlag** Preiszuschlag für Kleingläser, wenn die Fläche des Glases kleiner ist als der angegebene Grenzwert. Im zweiten Feld wählen Sie den Zuschlagstyp.
**Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu10, pokokon.zuk10

**Überlängenzuschlag** Preiszuschlag für Überlängen, wenn eine Kantenlänge länger ist, als der angegebene Grenzwert. Im zweiten Feld wählen Sie den Zuschlagstyp.
**Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu11, pokokon.zuk11

**Übergrößenzuschlag** Preiszuschlag für Übergrößen, wenn beide Glaskanten eine festgelegte Länge überschreiten. Im zweiten Feld wählen Sie den Zuschlagstyp.
**Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu12, pokokon.zuk12

#### Verglasung

In diesem Bereich werden die Werte für Verglasung und Versiegelung angezeigt. Sie können die Werte bearbeiten.

**Min.Preis einsetzen** Mindestpreis, der für Verglasung und/oder Versiegelung gilt.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu21, pokokon.zuk21

**Verglasungspreis** Preis der Verglasung.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu22, pokokon.zuk22

**Versiegelungspreis** Preis der Versiegelung.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu23, pokokon.zuk23

#### Fußzeile

In diesem Bereich werden die Bezeichnung des Artikels und das Kennzeichen der Warengruppe des Artikels angezeigt.

### Konditionen für PKZ-VSG, PKZ-ESG

**Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Preismethode PKZ-VSG oder PKZ-ESG > `<Shift>` + `<F9>`**

**Abb. D-126 Konditionen für PKZ-ESG, PKZ-VSG**

In diesem Dialog werden die Preiskonditionen eines Positionsartikels angezeigt, dem die Preismethode PKZ-ESG oder PKZ-VSG zugeordnet ist. Sie können die Preiskonditionen bearbeiten.

In den Dialogen **Konditionen PKZ-ESG** und **Konditionen PKZ-VSG** sind die Register **Verkauf** und **Einkauf** weitgehend analog aufgebaut. Das Feld **Gesamtzuschlag** wird im Register Einkauf nicht angezeigt.

Wenn Zusatz-Bearbeitungen in der Stückliste der Position enthalten sind, dann sind die Register **Bearbeitungspreise (VK), (EK)** aktiv:
⇨ "Positionskonditionen - Bearbeitungspreise" auf Seite D-1366

Wenn Sprossen in der Stückliste der Position enthalten sind, dann ist das Register **Sprossenpreise** aktiv:
⇨ "Positionskonditionen - Sprossenpreise" auf Seite D-1369

Wenn Sie einen VSG-Artikel erfasst haben, werden Ihnen mit `<Shift>` + `<F10>` die Konditionen der Austausch- und Zusatzpreise für die einzelnen Glasscheiben in dem VSG-Artikel in einem eigenen Dialog angezeigt:
⇨ "Produktionskostenkalkulation" auf Seite D-1372

#### Kopfbereich

Die Felder sind zum Dialog **Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG** beschrieben:
⇨ "Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG" auf Seite D-1341

#### Register Verkauf, Einkauf

Die meisten Felder sind zum Dialog **Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG** beschrieben:
⇨ "Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG" auf Seite D-1341

#### Größenzuschläge

Die meisten Felder sind zum Dialog **Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG** beschrieben:
⇨ "Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG" auf Seite D-1341
Zusätzlich werden folgende Felder im Register Verkauf angezeigt:

**Seitenverhältnis** Preiszuschlag für bestimmte Seitenverhältnisse. Im zweiten Feld wählen Sie den Zuschlagstyp. Das Feld im wird nur im Dialog **Konditionen PKZ-ESG** angezeigt.
**Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu28, pokokon.zuk28

#### Verglasung

Die Felder sind zum Dialog **Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG** beschrieben:
⇨ "Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG" auf Seite D-1341

#### Fußzeile

In diesem Bereich werden die Bezeichnung des Artikels und das Kennzeichen der Warengruppe des Artikels angezeigt.

### Konditionen ISO

**Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Preismethode ISO > `<Shift>` + `<F9>`**

**Abb. D-127 Konditionen ISO**

In diesem Dialog werden die Preiskonditionen eines Positionsartikels angezeigt, dem die Preismethode ISO zugeordnet ist. Sie können die Preiskonditionen bearbeiten.

Im Dialog Konditionen ISO sind die Register Verkauf und Einkauf analog aufgebaut.

Wenn Zusatz-Bearbeitungen in der Stückliste der Position enthalten sind, dann sind die Register Bearbeitungspreise (VK), (EK) aktiv:
⇨ "Positionskonditionen - Bearbeitungspreise" auf Seite D-1366

Wenn Sprossen in der Stückliste der Position enthalten sind, dann ist das Register **Sprossenpreise** aktiv:
⇨ "Positionskonditionen - Sprossenpreise" auf Seite D-1369

#### Kopfbereich

**PKZ** Preiskennzeichen der vordefinierten Preisliste.
**Technische Info:** numerisches Feld, DB-Feld:pokokon.pkz, pokokon.ekpkz

**PLKZ** Das Preislisten-Kennzeichen ist die eindeutige Nummerierung für regionale, nationale und ausländische Preislisten.
**Technische Info:** numerisches Feld

#### Register Verkauf, Einkauf

**Preisart** Art der Preisberechnung.
- **Matrix:** Der Preis wird aus der zugeordneten Preismatrix berechnet. In der Preismatrix sind die Preise nach Höhe und Breite des Glases gestaffelt.
- **Vektor:** Der Preis wird aus dem zugeordnetem Vektor berechnet. In einem Vektor können die Preise nach der Größe gestaffelt werden.
- **Einzelscheiben:** Der Preis wird aus den Einzelpreisen der Gläser berechnet, aus denen sich die Scheibe zusammensetzt.
- **Prs/qm:** Der Preis wird pro Quadratmeter berechnet. Diese Preisart wird automatisch gewählt, wenn Sie in den Konditionen den Grundpreis oder einen Austauschpreis bearbeiten.
**Technische Info:** Toggle-Feld

**Matrix / Vektor** Nummer der Matrix oder des Vektors. Die Matrix ist eine zweidimensionale Preistabelle mit zwei Bezugsgrößen für die Staffelung, z. B. Breite und Höhe. Der Vektor ist eine eindimensionale Preistabelle mit einer Bezugsgröße für die Staffelung, z. B. Fläche. Wenn Sie eine Matrix oder einen Vektor gewählt haben, wird der Name der Matrix oder des Vektors im Klartext angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.matnr, pokokon.ekmatnr

**Grundpreis** Grundpreis einer Glasscheibe. Der Grundpreis ist abhängig vom gewählten Preistyp. Im zweiten Feld wählen Sie den Preistyp aus. Der Preistyp gibt an, worauf sich der Preis bezieht:
- **WE/Stück:** Der Preis gilt pro Stück.
- **WE/GME:** Der Preis gilt pro Grundmengeneinheit, z. B. pro Quadratmeter.
**Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu1, pokokon.zuk1

**Zuschlag** Preiszuschlag, der auf den Grundpreis erhoben wird.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu20, pokokon.zuk20

**1. Austausch, 2. Austausch, 3. Austausch** Austausch-Unterteile der Position. In den Feldern können Sie folgende Werte angeben:
- **Erstes Feld:** Nummer der Austauschliste.
    **Technische Info:** numerische Felder, alphanumerische Felder, DB-Felder: pokokon.atmat1, pokokon.atmat2, pokokon.atmat3
- **Zweites Feld:** Austauschkennzeichen A (Austausch) oder Z (Zusatz).
    **Technische Info:** numerische Felder, alphanumerische Felder, DB-Felder: pokokon.atkz1, pokokon.atkz2, pokokon.atkz3
- **Drittes Feld:** Preis des Austausch-Artikels.
    **Technische Info:** numerische Felder, alphanumerische Felder, DB-Felder: pokokon.atp1, pokokon.atp2, pokokon.atp3
- **Viertes Feld:** Preiszuschlag des Austausch-Artikels in Prozent.
    **Technische Info:** numerische Felder, alphanumerische Felder, DB-Felder: pokokon.zu11, pokokon.zu12, pokokon.zu13, pokokon.zu14, pokokon.zu15, pokokon.zu16

**Modellzuschlag** Preiszuschlag, der bei Modellen erhoben wird. Sie können den Wert in Prozent oder als Betrag mit Währungseinheit angeben. Als Zuschlag wird immer der höhere Wert herangezogen.
**Technische Info:** numerische Felder, DB-Felder: pokokon.zu2, pokokon.zuk2

**Teuerungszuschlag** Prozentualer Teuerungszuschlag, der auf den Mengeneinheitspreis aufgeschlagen wird. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu3, pokokon.zuk3

**Faktor** Faktor des Preiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu4, pokokon.zuk4

**Maßrundung** Angabe der Maßrundung in Millimeter für die Preisberechnung des Artikels. Für die Preisberechnung werden die Kantenlängen in der Auftragsposition auf den nächsthöheren Wert in Millimeter aufgerundet, der durch die angegebene Maßrundung teilbar ist. In der Produktion werden diese Angaben nicht berücksichtigt. Dieses Feld wird nur im Register Verkauf angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu5, pokokon.zuk5

**Mindestberechnung** Angabe der Mindestfläche in Quadratmeter, für die der Preis berechnet wird. Wenn die Fläche in der Auftragsposition kleiner ist als die Mindestberechnungsfläche, wird der Preis für diese Fläche berechnet. Dieses Feld wird nur im Register Verkauf angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu6, pokokon.zuk6

**Mindestkantenlänge** Angabe der Kantenlänge in Millimeter für die Preisberechnung. Diese Größe wird herangezogen, wenn die Höhe oder Breite des Glases in der Auftragsposition kleiner ist als diese Mindestkantenlänge. Das Feld wird nur im Dialog Konditionen ISO angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu7, pokokon.zuk7

**SZR-Zuschlag** Preiszuschlag für den Scheibenzwischenraum. Im zweiten Feld geben Sie den Zuschlagstyp an. Der Zuschlagstyp gibt an, worauf sich der Zuschlag bezieht:
- **WE/Stück:** Der Zuschlag wird als fester Betrag auf den Stückpreis der Position aufgeschlagen.
- **WE/qm:** Der Zuschlag wird pro Quadratmeter der Scheibenfläche aufgeschlagen.
- **Prozent:** Der Zuschlag wird pro Scheibenzwischenraum als Prozentwert auf den Glasgrundpreis aufgeschlagen.
**Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu8, pokokon.zuk8

**Stufenzuschlag** Preiszuschlag für ein Glas mit einer Stufe. Im zweiten Feld geben Sie den Zuschlagstyp an. Der Zuschlagstyp gibt an, worauf sich der Zuschlag bezieht:
- **WE/St netto:** Der Stufenzuschlag wird nach Berechnung des Faktors als fester Nettobetrag pro Stufe aufgeschlagen.
- **WE/St brutto:** Der Stufenzuschlag wird vor Berechnung des Faktors als fester Bruttobetrag pro Stufe aufgeschlagen.
- **Prozent:** Der Stufenzuschlag wird prozentual auf den Glasmengeneinheitspreis und die Austauschpreise aufgeschlagen.
- **%/Stück:** Der Stufenzuschlag wird pro Stufe prozentual auf den Glasmengeneinheitspreis und die Austauschpreise aufgeschlagen.
**Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu9, pokokon.zuk9

**Kunstverglasung** Preiszuschlag der Kunstverglasung in Prozent, wenn in der Stückliste ein Glas mit dem Artikeltyp Kunstverglasung eingehängt ist.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu28, pokokon.zuk28

**Überlängenzuschläge** Preiszuschlag für Überlängen in Prozent, wenn eine Kantenlänge länger ist, als der angegebene Grenzwert.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu19, pokokon.zuk19

**Sonderzuschlag** Preiszuschlag für Sonderanfertigungen. Im zweiten Feld geben Sie den Zuschlagstyp an. Der Zuschlagstyp gibt an, worauf sich der Zuschlag bezieht:
- **WE/Stück:** Der Zuschlag wird als fester Betrag auf den Stückpreis der Position aufgeschlagen.
- **WE/GMR:** Der Zuschlag wird pro Grundmengeneinheit, z. B. pro Quadratmeter, aufgeschlagen.
- **Prozent:** Der Zuschlag wird als Prozentwert auf den Glasgrundpreis aufgeschlagen.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu25, pokokon.zuk25

**Gesamtzuschlag** Preiszuschlag für die Position in Prozent.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu26, pokokon.zuk26

**Mindestpreis** Mindestpreis für die Position.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu18, pokokon.zuk18

**Stückpreisrundung** Ab- oder Aufrundung für den Stückpreis einer Position.
**Technische Info:** numerisches Feld, DB-Feld: pokokonp.vkstkprsrund, pokokonp.ekstkprsrund

#### Größenzuschläge

Die meisten Felder sind zum Dialog Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG beschrieben:
⇨ "Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG" auf Seite D-1341
Zusätzlich werden folgende Felder angezeigt:

**Seitenverhältnis** Preiszuschlag für bestimmte Seitenverhältnisse. Im zweiten Feld wählen Sie den Zuschlagstyp.
**Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu28,

**Flächenzuschlag** Preiszuschlag für bestimmte Flächen. Im zweiten Feld wählen Sie den Zuschlagstyp. Das Feld wird nur im Dialog Konditionen ISO angezeigt.
**Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu9

#### Verglasung

**Verglasungspreis** Preis der Verglasung.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu21, pokokon.zuk21

**Versiegelungspreis** Preis der Versiegelung.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu22, pokokon.zuk22

**Mindestpreis Verglasung** Mindestpreis der Verglasung.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu23, pokokon.zuk23

**Mindestpreis Versiegelung** Mindestpreis der Versiegelung.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu24, pokokon.zuk24

#### Fußzeile

In diesem Bereich werden die Bezeichnung des Artikels und das Kennzeichen der Warengruppe des Artikels angezeigt.

### Konditionen für ISO (SCHWEIZ)

**Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Preismethode ISO-Schweiz > `<Shift>` + `<F9>`**

**Abb. D-128 Konditionen ISO (SCHWEIZ)**

In diesem Dialog werden die Preiskonditionen eines Positionsartikels angezeigt, dem die Preismethode ISO-Schweiz zugeordnet ist. Sie können die Preiskonditionen bearbeiten.

Im Dialog **Konditionen ISO-Schweiz** gibt es das Register **Verkauf**, aber kein Register **Einkauf**.

Wenn Zusatz-Bearbeitungen in der Stückliste der Position enthalten sind, dann sind die Register Bearbeitungspreise (VK), (EK) aktiv:
⇨ "Positionskonditionen - Bearbeitungspreise" auf Seite D-1366

Wenn Sprossen in der Stückliste der Position enthalten sind, dann ist das Register Sprossenpreise aktiv:
⇨ "Positionskonditionen - Sprossenpreise" auf Seite D-1369

#### Register Verkauf

**VK-PKZ** Preiskennzeichen der vordefinierten Preisliste für den Verkauf.
**Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.pkz

**Vektor** Nummer des Vektors, aus dem der Preis gezogen werden soll.
**Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.matnr

**Glasgrundpreis** Anzeige des Mindestpreises für den Glasgrundpreis. Der Glasgrundpreis ist durch den Vektor festgelegt und kann vorgangsbezogen bearbeitet werden:
- **Glasgrundpreis:** Glasgrundpreis in der Währungseinheit.
    **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu1
- **(Preistyp):** Angabe, worauf sich der Glasgrundpreis bezieht:
    - **WE/Stück:** Der Preis gilt pro Stück.
    - **WE/GME:** Der Preis gilt pro Grundmengeneinheit, z. B. pro Quadratmeter.
    **Technische Info:** Toggle-Feld, DB-Feld: pokokon.flag2
- **Mindestpreise (in Zeile Glasgrundpreis):** Mindestpreis für den Glasgrundpreis. Dieser Preis wird festgelegt, wenn der berechnete Preis in der Auftragsposition niedriger ist als der angegebene Mindestpreis.
    **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu20

**Mengenstaffelrabatt 1** Rabatt auf den Glasgrundpreis in Prozent. Der Rabatt gilt ab der Menge, die für den Kunden festgelegt ist.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu2

**Gasgrundpreis** Grundpreis für die Gasfüllung bei ISO-Artikeln. In den Feldern können Sie folgende Werte angeben:
- **Gasgrundpreis:** Gasgrundpreis pro Quadratmeter.
    **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu3
- **Mindestpreise (in Zeile Gasgrundpreis):** Mindestpreis für den Gasgrundpreis. Der Preis, der festgelegt wird, wenn der berechnete Preis in der Auftragsposition niedriger ist als der angegebene Mindestpreis.
    **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu21

**1. Austausch, 2. Austausch, 3. Austausch** In den Feldern geben Sie die Preise für die Austauschartikel in der Stückliste an. Sie können max. drei Austauschpreise festlegen:
- **1. Austausch, 2. Austausch, 3. Austausch:** Nummer der Austauschliste.
    **Technische Info:** numerische Felder, DB-Felder: pokokon.atmat1, pokokon.atmat2, pokokon.atmat3
- **PG:** Preisgruppe.
    **Technische Info:** Anzeigefelder, DB-Felder
- **(Artikelpreis):** Preis des Austausch-Artikels pro Quadratmeter.
    **Technische Info:** numerische Felder, alphanumerische Felder, DB-Felder: pokokon.atp1, pokokon.atp2, pokokon.atp3
- **Mindestpreise (in Zeile 1. Austausch, 2. Austausch, 3. Austausch):** Mindestpreis für den Austausch. Der Preis, der festgelegt wird, wenn der berechnete Preis in der Auftragsposition niedriger ist als der angegebene Mindestpreis.
    **Technische Info:** numerische Felder, DB-Felder: pokokon.zu22, pokokon.zu23, pokokon.zu25

**Mengenstaffelrabatt 2** Rabatt auf den Austauschpreis in Prozent. Der Rabatt gilt ab der Menge, die für den Kunden festgelegt ist.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu4

#### Zuschläge

**Teuerungszuschlag** Prozentualer Teuerungszuschlag, der auf den Mengeneinheitspreis aufgeschlagen wird. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu5

**Druckausgleich** Zuschlag für Druckausgleich in Prozent.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu6

**Serienrabatt** Rabatt auf den Glaspreis in Prozent. Der Rabatt gilt ab der Anzahl an Scheiben, die für den Kunden festgelegt ist.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu7

**Warengruppenfaktor** Faktor, der bei Erreichen der Grenzmenge für die Warengruppe berücksichtig wird. Wenn Sie einen Faktor < 100 % angeben, wird er als Rabatt verwendet und reduziert den Preis.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu8

**Modellzuschlag** Preiszuschlag in Prozent, der bei Modellen erhoben wird.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu9

**Mindestmodellzusch.** Mindestpreiszuschlag, der bei Modellen erhoben wird. Wenn der berechnete Modellzuschlag im Auftrag kleiner ist als der definierte Mindestmodellzuschlag, wird dieser Mindestzuschlag erhoben.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu10

**Einzelmodellzuschlag** Preiszuschlag in Prozent für bestimmte Modelle.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu11

**Stufenzuschlag** Preiszuschlag für die Stufenbearbeitung pro Stück.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu19

**Transportzuschlag** Preiszuschlag für den Transport in der Währungseinheit.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu12

**Gesamtzuschlag** Preiszuschlag für die Position in Prozent.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu13

**Verglasung** Preiszuschlag für die Verglasung in der Währungseinheit pro Quadratmeter.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu14

**Versiegelung** Preiszuschlag für die Versiegelung in der Währungseinheit pro laufendem Meter.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu15

**UV-Abdeckung** Preiszuschlag für die UV-Abdeckung pro laufendem Meter.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu24

#### (Bereich ohne Bezeichnung)

**Maßrundung** Maßrundung in Millimeter.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu16

**Minberech.** Mindestanzahl der Mengeneinheiten, für die der Preis berechnet wird. Wenn die Menge in der Auftragsposition kleiner ist als die Mindestmenge, wird der Preis für diese Mindestmenge berechnet.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu17

**Minkant.** Mindestkantenlänge in Millimeter.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu18

#### Bearbeitungen

**Ecken TZ, Ecken Faktor** Teuerungszuschlag und Faktor des Preiszuschlags in Prozent für Eckbearbeitungen, z. B. Eckabschnitt.
**Technische Info:** numerische Felder, DB-Feld: pokokon.zu26

**Kanten TZ, Kanten Faktor** Teuerungszuschlag und Faktor des Preiszuschlags in Prozent für Kantenbearbeitungen, z. B. Polieren.
**Technische Info:** numerische Felder, DB-Feld: pokokon.zu27, pokokon.zu28

**Fläche TZ, Fläche Faktor** Teuerungszuschlag und Faktor des Preiszuschlags in Prozent für Flächenbearbeitungen, z. B. Beschichtung.
**Technische Info:** numerische Felder, DB-Feld: pokokon.zu29, pokokon.zu30

#### Fußzeile

In diesem Bereich werden die Bezeichnung des Artikels und das Kennzeichen der Warengruppe des Artikels angezeigt.

### Konditionen für PKZ-FARBARTIKEL

**Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Preismethode PKZ-Farbartikel > `<Shift>` + `<F9>`**

**Abb. D-129 Konditionen für PKZ-FARBARTIKEL**

In diesem Dialog werden die Preiskonditionen eines Positionsartikels angezeigt, dem die Preismethode PKZ-Farbartikel zugeordnet ist. Sie können die Konditionen bearbeiten.

Im Dialog Konditionen für PKZ-FARBARTIKEL sind die Bereiche Verkauf und Einkauf analog aufgebaut.

Wenn Zusatz-Bearbeitungen in der Stückliste der Position enthalten sind, dann sind die Register Bearbeitungspreise (VK), (EK) aktiv:
⇨ "Positionskonditionen – Bearbeitungspreise" auf Seite D-1366

#### Kopfbereich

**VK-PKZ** Preiskennzeichen der vordefinierten Preisliste für den Verkauf.
**Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.pkz

**EK-PKZ** Preiskennzeichen der vordefinierten Preisliste für den Einkauf.
**Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.ekpkz

#### Register Konditionen

Die meisten Felder sind zum Dialog Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG beschrieben:
⇨ "Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG" auf Seite D-1341

Zusätzlich werden folgende Felder angezeigt:

**Grundpreis** Grundpreis des Artikels. Der Preistyp bestimmt, worauf sich der Preis bezieht:
- **WE/Stück:** Der Preis gilt pro Stück.
- **WE/GME:** Der Preis gilt pro Grundmengeneinheit, z. B. pro Quadratmeter.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.flag2

**Mindestberechnung** Mindestanzahl der Mengeneinheiten, für die der Preis berechnet wird. Wenn die Menge in der Auftragsposition kleiner ist als die Mindestmenge, wird der Preis für diese Mindestmenge berechnet.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu6, pokokon.zuk6

#### Fußzeile

In diesem Bereich werden die Bezeichnung des Artikels und das Kennzeichen der Warengruppe des Artikels angezeigt.

### Konditionen für PKZ-PREISE-ALLGEMEIN

**Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Preismethode PKZ-Preise-Allgemein > `<Shift>` + `<F9>`**

**Abb. D-130 Konditionen für PKZ-PREISE-ALLGEMEIN**

In diesem Dialog werden die Preiskonditionen eines Positionsartikels angezeigt, dem die Preismethode PKZ-Preise-Allgemein zugeordnet ist. Sie können die Preiskonditionen bearbeiten.

Im Dialog Konditionen für PKZ-PREISE-ALLGEMEIN sind die Bereiche Verkauf und Einkauf weitgehend analog aufgebaut. Das Feld Gesamtzuschlag wird im Bereich Einkauf nicht angezeigt.

Wenn Zusatz-Bearbeitungen in der Stückliste der Position enthalten sind, dann sind die Register Bearbeitungspreise (VK), (EK) aktiv:
⇨ "Positionskonditionen - Bearbeitungspreise" auf Seite D-1366

#### Kopfbereich

**VK-PKZ** Preiskennzeichen der vordefinierten Preisliste für den Verkauf.
**Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.pkz

**EK-PKZ** Preiskennzeichen der vordefinierten Preisliste für den Einkauf.
**Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.ekpkz

**Vektor** Nummer des Vektors, aus dem der Preis gezogen werden soll.
**Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.matnr

#### Register Konditionen

Die meisten Felder sind zum Dialog Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG beschrieben:
⇨ "Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG" auf Seite D-1341
Zusätzlich werden folgende Felder angezeigt:

**Grundpreis** Grundpreis des Artikels. Der Preistyp bestimmt, worauf sich der Preis bezieht:
- **WE/Stück:** Der Preis gilt pro Stück.
- **WE/GME:** Der Preis gilt pro Grundmengeneinheit, z. B. pro Quadratmeter.
**Technische Info:** Toggle-Feld Feld, DB-Feld: pokokon.flag2

**Mindestberechnung** Mindestanzahl der Mengeneinheiten, für die der Preis berechnet wird. Wenn die Menge in der Auftragsposition kleiner ist als die Mindestmenge, wird der Preis für diese Mindestmenge berechnet.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu6, pokokon.zuk6

#### Fußzeile

In diesem Bereich werden die Bezeichnung des Artikels und das Kennzeichen der Warengruppe des Artikels angezeigt.

### Konditionen für PKZ-GLASTÜREN

**Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Preismethode PKZ-Glastüren > `<Shift>` + `<F9>`**

**Abb. D-131 Konditionen für PKZ-GLASTÜREN**

In diesem Dialog werden die Preiskonditionen eines Positionsartikels angezeigt, dem die Preismethode PKZ-Glastüren zugeordnet ist. Sie können die Preiskonditionen bearbeiten.

In den Bereichen **Verkauf** und **Einkauf** werden weitgehend die gleichen Felder angezeigt. Im Bereich **Verkauf** geben Sie die Verkaufspreise an, im Bereich **Einkauf** die Einkaufspreise.

#### Kopfzeile

**VK-PKZ** Preiskennzeichen der vordefinierten Preisliste für den Verkauf.
**Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.pkz

**EK-PKZ** Preiskennzeichen der vordefinierten Preisliste für den Einkauf.
**Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.ekpkz

#### (Bereich ohne Bezeichnung)

**Scheibe 1, 2, ..., 7** Fläche der Scheiben in der GGA. In den nebenstehenden Feldern in den Bereichen **Verkauf** und **Einkauf** wird der Quadratmeterpreis für die jeweilige Scheibe angezeigt.
**Technische Info:** numerische Felder, DB-Felder: pokokon.zu5, pokokon.zu7, pokokon.zu9, pokokon.zu11, pokokon.zu13, pokokon.zu15, pokokon.zu17

#### Verkauf und Einkauf

**Staffelstufe** Preisstufe, aus der der Preis verwendet wird. Das Feld wird von der Preisberechnung nur ausgewertet, wenn für den relevanten Artikelpreisvektor die Preisart 2 – Staffelstufe angegeben ist.
**Technische Info:** numerische Felder, DB-Felder: pokokon.flag1, pokokon.ekflag1

**TZ** Teuerungszuschlag in Prozent. Der Teuerungszuschlag wird auf den Mengeneinheitspreis aufgeschlagen. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
**Technische Info:** numerische Felder, DB-Felder: pokokon.zu3, pokokon.zuk3

**Faktor** Faktor des Preiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerische Felder, DB-Felder: pokokon.zu4, pokokon.zuk4

**Scheibe €/qm** Preis pro Quadratmeter für die jeweilige Scheibe.
- **Verkauf:** Verkaufspreis pro Quadratmeter für die nebenstehende Scheibe.
    **Technische Info:** numerische Felder, DB-Felder: pokokon.zu6, pokokon.zu8, pokokon.zu10, pokokon.zu12, pokokon.zu14, pokokon.zu16, pokokon.zu18
- **Einkauf:** Einkaufspreis pro Quadratmeter für die nebenstehende Scheibe.
    **Technische Info:** numerische Felder, DB-Felder: pokokon.zuk6, pokokon.zuk8, pokokon.zuk10, pokokon.zuk12, pokokon.zuk14, pokokon.zuk16, pokokon.zuk18

**Zuschlag** Zuschlag, der auf den Preis erhoben wird. Im zweiten Feld geben Sie den Zuschlagstyp an. Der Zuschlagstyp gibt an, auf welchen Preis sich der Zuschlag bezieht:
- **WE/Stück:** Der Zuschlag wird als fester Betrag auf den Stückpreis der Position aufgeschlagen.
- **WE/GME:** Der Zuschlag wird auf den Preis pro Grundmengeneinheit aufgeschlagen, z. B. pro Quadratmeter.
- **Prozent:** Der Zuschlag wird als Prozentwert auf den Glasgrundpreis aufgeschlagen.
Dieses Feld wird nur im Bereich Verkauf angezeigt.
**Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu19

**VK-Kantenbearbeitungen/TZ** Teuerungszuschlag für Kantenbearbeitungen auf den Verkaufspreis in Prozent. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu20

**VK-Kantenbearbeitungen/Faktor** Faktor für Kantenbearbeitungen auf den Verkaufspreis in Prozent. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zuk20

**VK-Eckenbearbeitungen/TZ** Teuerungszuschlag für Eckenbearbeitungen auf den Verkaufspreis in Prozent. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu21

**VK-Eckenbearbeitungen/Faktor** Faktor für Eckenbearbeitungen auf den Verkaufspreis in Prozent. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zuk21

**VK-Flächenbearbeitungen/TZ** Teuerungszuschlag für Flächenbearbeitungen auf den Verkaufspreis in Prozent. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu22

**VK-Flächenbearbeitungen/Faktor** Faktor für Flächenbearbeitungen auf den Verkaufspreis in Prozent. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zuk22

**EK alle Bearbeitungen/TZ** Teuerungszuschlag für alle Bearbeitungen auf den Einkaufspreis in Prozent. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zu23

**EK alle Bearbeitungen/Faktor** Faktor für alle Bearbeitungen auf den Einkaufspreis in Prozent. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerisches Feld, DB-Feld: pokokon.zuk23

**Zubehör/TZ** Teuerungszuschlag für Zubehörartikel auf den Einkaufs- und/oder Verkaufspreis in Prozent. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
**Technische Info:** numerische Felder, DB-Felder: pokokon.zu24, pokokon.zuk24

**Zubehör/Faktor** Faktor für Zubehörartikel auf den Einkaufs- und/oder Verkaufspreis in Prozent. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerische Felder, DB-Felder: pokokon.zu25, pokokon.zuk25

#### Fußzeile

In diesem Bereich werden die Bezeichnung des Artikels und das Kennzeichen der Warengruppe des Artikels angezeigt.

### Konditionen für Manuelle Preise

**Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Preismethode Manuelle Preise > `<Shift>` + `<F9>`**

**Abb. D-132 Positionskonditionen – Konditionen Manuelle Preise**

In diesem Dialog werden die Preiskonditionen eines Positionsartikels angezeigt, dem die Preismethode Manuelle Preise in den Stammdaten zugeordnet ist. Sie können die Preiskonditionen bearbeiten.

> **Automatische Preismethodenänderung**
> Sie können auch für Positionsartikel mit einer anderen Preismethode einen Preis manuell festlegen. Die Preismethode für diesen Positionsartikel wird dann automatisch auf Manuelle Preise geändert.

**Preistyp** Angabe, worauf sich der Preis bezieht.
- **WE/Stück:** Der Preis gilt pro Stück.
- **WE/GME:** Der Preis gilt pro Grundmengeneinheit, z. B. pro Quadratmeter.
**Technische Info:** Toggle-Feld, DB-Feld: `pokokon.flag2`

Die folgenden Werte geben Sie für Verkaufs- und Einkaufspreise getrennt an.

**Preis** Grundpreis einer Glasscheibe. Der Preistyp wird aus dem vorherigen Feld herangezogen.
**Technische Info:** numerische Felder, DB-Felder: `pokokon.zu1`, `pokokon.zuk1`

**TZ** Teuerungszuschlag in Prozent. Der Teuerungszuschlag wird auf den Mengeneinheitspreis aufgeschlagen.
**Technische Info:** numerische Felder, DB-Felder: `pokokon.zu2`, `pokokon.zuk2`

**Faktor** Faktor des Preiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerische Felder, DB-Felder: `pokokon.zu3`, `pokokon.zuk3`

**Maßrundung** Maßrundung in Millimeter für die Preisberechnung des Artikels. Für die Preisberechnung werden die Kantenlängen in der Auftragsposition auf den nächsthöheren Wert in Millimeter aufgerundet, der durch die angegebene Maßrundung teilbar ist. In der Produktion werden diese Angaben nicht berücksichtigt.
**Technische Info:** numerische Felder, DB-Felder: `pokokon.zu5`, `pokokon.zuk5`

**Mindestberechnung** Wenn der Wert in der Auftragsposition kleiner ist als der Mindestberechnungswert, wird der Preis für diesen Wert berechnet. Bei z. B. einem Artikel, der als Fläche angegeben wird, wird die Mindestfläche in Quadratmeter als Mindestberechnungswert angegeben.
**Technische Info:** numerische Felder, DB-Felder: `pokokon.zu5`, `pokokon.zuk5`

### VSG-Austausch-/Zusatzpreise

**Verkauf > Auftragserfassung > Register Positionen > Preisfeld von VSG-Artikel > `<Shift>` + `<F9>` > `<Shift>` + `<F10>`**

**Abb. D-133 VSG-Austausch-/Zusatzpreise**

In diesem Dialog werden die Konditionen der Austausch- und Zusatzpreise für die einzelnen Glasscheiben in einem VSG-Artikel angezeigt. Sie können die Preiskonditionen bearbeiten.

Die Werte für **Verkauf**, **Einkauf** und die **Detailansicht** der Austausch- und Zusatzpreise werden jeweils in einer eigenen Ansicht angezeigt.
- Mit `<F2>` wechseln Sie zwischen den Ansichten für Verkauf, Einkauf und der Detailansicht.

Der Dialog ist nur freigeschaltet, wenn in der gewählten Position VSG-Artikel erfasst sind.

#### Verkauf und Einkauf

- **Artikel:** Artikelnummer.
    **Technische Info:** Anzeigefeld, numerisches Feld, DB-Feld: `pokoaust.artnr`
- **Austausch-/Zusatzliste, Bezeichnung:** Nummer der Austauschliste. Wenn eine Nummer angeben ist, wird die Bezeichnung im Klartext angezeigt.
    **Technische Info:** numerisches Feld, Anzeigefeld, DB-Felder: `pokoaust.vkatinr`, `pokoaust.ekatInr`, `xatl.bez`
- **Min.ber.:** Mindestberechnung. Angabe der Mindestfläche in Quadratmeter, für die der Preis berechnet wird. Wenn die Fläche des Austauschglases in der Auftragsposition kleiner ist als die Mindestberechnungsfläche, dann wird der Preis für diese Mindestberechnungsfläche berechnet.
    **Technische Info:** numerisches Feld, DB-Felder: `pokoaust.vkminber`, `pokoaust.ekminber`
- **Faktor:** Faktor des Preiszuschlags in Prozent.
    **Technische Info:** numerisches Feld, DB-Felder: `pokoaust.vkfaktor`, `pokoaust.ekfaktor`
- **VK-Preis, EK-Preis:** Verkaufs- oder Einkaufspreis des Austauschglases.
    **Technische Info:** numerisches Feld, DB-Feld: `pokoaust.vkmepreis`, `pokoaust.ekmepreis`
- **Preistyp:** Angabe, worauf sich der Preis bezieht.
    - **WE/qm:** Der Preis gilt pro Quadratmeter.
    - **Prozent:** Der Zuschlag wird als Prozentwert auf den Glasgrundpreis berechnet.
    **Technische Info:** Toggle-Feld, DB-Feld: `pokoaust.vkpreistyp`, `pokoaust.ekpreistyp`

#### Detailansicht

Die Felder in der Detailansicht entsprechen den Spalten in Verkauf und Einkauf. Zusätzlich werden die Felder für die Größenzuschläge jeweils für den Verkauf und Einkauf angezeigt. Der Zuschlagstyp gibt an, worauf sich der Zuschlag bezieht:
- **WE Wert:** Der Zu- oder Abschlag wird als fester Betrag auf den Verkaufs-/Einkaufspreis berechnet.
- **Prozent:** Der Zuschlag wird prozentual aus dem Verkaufs-/Einkaufspreis berechnet.

**Kleinglaszuschlag** Preiszuschlag für Kleingläser, wenn die Fläche des Glases kleiner ist als der angegebene Grenzwert. Im zweiten Feld wählen Sie den Zuschlagstyp.
**Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: `pokoaust.vkklzuschlag`, `pokoaust.vkklzutyp`, `pokoaust.ekklzuschlag`, `pokoaust.ekklzutyp`

**Überlängenzuschlag** Preiszuschlag für Überlängen, wenn eine Kantenlänge länger ist, als der angegebene Grenzwert. Im zweiten Feld wählen Sie den Zuschlagstyp.
**Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: `pokoaust.vkuebzuschlag`, `pokoaust.vkuebzutyp`, `pokoaust.ekuebzuschlag`, `pokoaust.ekuebzutyp`

**Übergrößenzuschlag** Preiszuschlag für Übergrößen, wenn beide Glaskanten eine festgelegte Länge überschreiten. Im zweiten Feld wählen Sie den Zuschlagstyp.
**Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: `pokoaust.vkuebgrzuschlag`, `pokoaust.vkuebgrzutyp`, `pokoaust.ekuebgrzuschlag`, `pokoaust.ekuebgrzutyp`

### Positionskonditionen – Bearbeitungspreise

**Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Zusatz-Bearbeitung wählen > `<Shift>` + `<F9>`**

**Abb. D-134 Positionskonditionen – Bearbeitungspreise (VK), (EK), Detailansicht**

In diesen Registern werden die Preiskonditionen für eine preisrelevante Bearbeitung angezeigt, je nachdem ob diese in der Positionsstückliste enthalten ist. Sie können die Preiskonditionen bearbeiten.

Die Bearbeitungspreise sind in **Verkauf** und **Einkauf** aufgeteilt. Außerdem gibt es eine **Detailansicht**, die für beide Register analog aufgebaut ist. In der Detailansicht werden mehr Werte des Bearbeitungspreises für die einzelne Bearbeitung angezeigt.

- Mit `<F5>` wechseln Sie in die Detailansicht.

Die Register sind nur freigeschaltet, wenn in der gewählten Position Zusatz-Bearbeitungen erfasst sind. Das Register **Bearbeitungspreise (EK)** ist nur aktiv, wenn die Beschaffungsart **Bestellung** oder **Mitgelief.** für die Position gewählt ist.

#### Register Bearbeitungspreise (VK)

- **Artikel:** Bezeichnung der Bearbeitung.
    **Technische Info:** Anzeigefeld, DB-Feld: `aufstrukt.artnr`
- **Bre, Höh:** Anzahl der bearbeiteten Breiten und Höhen der Scheibe.
    **Technische Info:** numerische Felder, DB-Felder: `poszu.panz1`, `poszu.panz2`
- **Preistyp:** Angabe, worauf sich der Preis der Bearbeitung bezieht:
    - **WE/Stück:** Der Preis gilt pro Stück.
    - **WE/GME:** Der Preis gilt pro Grundmengeneinheit, z. B. pro Quadratmeter.
    - **Prozent:** Der Preis wird als Prozentwert vom Grundpreis des Kopfartikels berechnet.
    - **WE/qm:** Der Preis gilt pro Quadratmeter
    - **WE/lfm:** Der Preis gilt pro laufender Meter.
    **Technische Info:** Toggle-Feld, DB-Feld: `poszu.part`
- **Menge:** Menge der Bearbeitung pro Grundmengeneinheit.
    **Technische Info:** numerisches Feld, DB-Feld: `poszu.pme`
- **Faktor:** Verkaufspreis-Faktor des Bearbeitungspreiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
    **Technische Info:** numerisches Feld, DB-Feld: `poszu.vkfaktor`
- **TZ:** Verkaufspreis-Teuerungszuschlag für die Bearbeitung in Prozent. Der Teuerungszuschlag wird auf den Mengeneinheitspreis aufgeschlagen. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
    **Technische Info:** numerisches Feld, DB-Feld: `poszu.vktz`
- **ModZu:** Modellzuschlag in Prozent.
    **Technische Info:** numerisches Feld, DB-Feld: `poszu.vkmodzusch`
- **VK-Preis:** Verkaufspreis der Bearbeitung.
    **Technische Info:** numerisches Feld, DB-Feld: `poszu.ppme`
- **Grp:** Nummer der Gruppierung. Die Bearbeitungen können unter einer Nummer gruppiert werden.
    **Technische Info:** numerisches Feld, DB-Feld: `poszu.masflag`

#### Register Bearbeitungspreise (EK)

Die meisten Spalten sind zum Register **Bearbeitungspreise (VK)** beschrieben.
⇨ "Register Bearbeitungspreise (VK)" auf Seite D-1367
Zusätzlich werden folgende Spalten angezeigt:

- **EK-Faktor:** Einkaufspreis-Faktor des Bearbeitungspreiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
    **Technische Info:** numerisches Feld, DB-Feld: `poszu.ekfaktor`
- **EK-TZ:** Einkaufspreis-Teuerungszuschlag für die Bearbeitung in Prozent. Der Teuerungszuschlag wird auf den Mengeneinheitspreis aufgeschlagen. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
    **Technische Info:** numerisches Feld, DB-Feld: `poszu.ektz`
- **EK-ModZu:** Einkaufspreis-Modellzuschlag in Prozent.
    **Technische Info:** numerisches Feld, DB-Feld: `poszu.ekmodzusch`
- **EK-Preis:** Einkaufspreis der Bearbeitung.
    **Technische Info:** numerisches Feld, DB-Feld: `poszu.ppmeek`

#### Bearbeitungspreise Detailansicht

Die meisten Felder in der Detailansicht sind zum Register **Bearbeitungspreise (VK)** beschrieben:
⇨ "Register Bearbeitungspreise (VK)" auf Seite D-1367
Zusätzlich werden folgende Felder angezeigt:

**Maßrundung** Maßrundung pro Bearbeitung in der Mengeneinheit.
**Technische Info:** Anzeigefeld, DB-Feld: `poszu.massrund`

**Mindestberechnung** Angabe der mindest berechneten Mengeneinheit der Bearbeitung.
**Technische Info:** Anzeigefeld, DB-Feld: `poszu.minber`, `poszu.minberek`

**Grundpreis** Grundpreis einer preisrelevanten Bearbeitung für Verkauf und Einkauf. Der Grundpreis für den Verkauf entspricht dem Wert im Feld VK-Preis im Register Bearbeitungspreise (VK), der Grundpreis für den Einkauf dem Wert im Feld EK-Preis im Register Bearbeitungspreise (EK).
**Technische Info:** numerische Felder, DB-Felder: `poszu.ppme`, `poszu.ppmeek`

**Mindestpreis** Mindestpreis für die Bearbeitung.
**Technische Info:** numerisches Feld, DB-Feld: `poszu.minpreis`

#### Fußzeile

In diesem Bereich werden die Bezeichnung des Artikels und das Kennzeichen der Warengruppe des Artikels angezeigt.

### Positionskonditionen – Sprossenpreise

**Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Sprossen > `<Shift>` + `<F9>`**

**Abb. D-135 Positionskonditionen - Sprossenpreise**

In diesem Register werden die Preiskonditionen für Sprossenpreise eines Positionsartikels angezeigt. Sie können die Preiskonditionen bearbeiten.

Das Register ist nur freigeschaltet, wenn in der gewählten Position Sprossen erfasst sind. Die Werte für Verkaufs- und Einkaufspreise werden in zwei eigenen Bereichen angezeigt.

#### Verkauf und Einkauf

**Sprossen-PKZ** Sprossenpreiskennzeichen aus der vordefinierten Preisliste der Sprossenberechnung.
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vkpkz`, `pokospro.ekpkz`

**Sprossenberechnungsart** Berechnungsart der Sprossen. Die Sprossenberechnungsarten sind ausführlich an anderer Stelle beschrieben:
⇨ "Auftragssprossenpreise" auf Seite D-1330
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vkberart`, `pokospro.ekberart`

**Sprossen-Faktor** Faktor des Sprossenpreiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vkfaktor`, `pokospro.ekfaktor`

**Sprossen-TZ** Sprossen-Teuerungszuschlag in Prozent. Der Teuerungszuschlag wird auf den Mengeneinheitspreis aufgeschlagen. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vktz`, `pokospro.ektz`

**Preis pro Feld** Sprossenpreis nach Anzahl der Felder, wenn im Sprossenaufbau Kreuzungspunkte vorhanden sind. Wenn z. B. zwei Sprossen senkrecht und zwei waagerecht das Fenster in neun Felder teilen, dann wird der Preis neunmal berechnet. Der Preis wird bei den Berechnungsarten `Felder`, `Feld +LM`, `Feld+K+R` und `Spezial` ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vkfeld`, `pokospro.ekfeld`

**Preis pro Feld 2** Sprossenpreis nach Anzahl der Felder, wenn im Sprossenaufbau keine Kreuzungspunkte vorhanden sind. Wenn z. B. vier Sprossen senkrecht und keine waagerecht das Fenster in fünf Felder teilen, dann wird der Preis fünfmal berechnet. Der Preis wird bei den Berechnungsarten `Felder`, `Feld +LM`, `Feld+K+R` und `Spezial` ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vk2feld`, `pokospro.ek2feld`

**Preis pro Laufmeter** Preis pro laufendem Meter der Sprosse. Der Preis wird bei den Berechnungsarten `LM`, `LM+K+R`, `LM+K`, `LM+R`, `Feld+LM` und `Spezial` ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vklaufm`, `pokospro.eklaufm`

**Preis pro Rand** Preis pro Randverbindung. Der Preis wird bei den Berechnungsarten `R`, `LM+K+R`, `LM+R`, `K+R`, `Feld+K+R` und `Spezial` ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vkrand`, `pokospro.ekrand`

**Preis pro Kreuz** Preis pro Kreuzungspunkt. Der Preis wird bei den Berechnungsarten `K`, `K+R`, `LM+K`, `LM+K+R`, `K oder LM`, `Feld+K+R` und `Spezial` ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vkkreuz`, `pokospro.ekkreuz`

**Prozent** Preis als Prozentwert auf den Preis des Kopfartikels. Der Preis wird bei der Berechnungsart `Prozent` ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vkprozent`, `pokospro.ekprozent`

**Qm-Preis** Preis pro Quadratmeter. Der Preis wird bei der Berechnungsart `qm-Preis` ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vkqmpreis`, `pokospro.ekqmpreis`

**Stückpreis** Preis pro Sprossenkonstruktion. Der Preis wird bei der Berechnungsart `Stück` ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vkstueckprs`, `pokospro.ekstueckprs`

**Mindestlaufmeter** Mindestlänge der Sprosse in Meter, die für den Preis berechnet wird. Wenn die Sprosse weniger Laufmeter misst, als die Mindestlaufmeter, dann wird der Preis für die Mindestlaufmeter berechnet. Der Preis wird bei der Berechnungsart `LM` ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vkminlm`, `pokospro.ekminlm`

**Mindestfeldanzahl** Anzahl der Sprossenfelder, für die der Preis mindestens berechnet wird. Der Preis wird bei der Berechnungsart `Felder` ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vkminfeld`, `pokospro.ekminfeld`

**Sprossen Faktor 2** Faktor des Sprossenpreiszuschlags in Prozent für die zweite Sprosse. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vkfaktor2`, `pokospro.ekfaktor2`

**Preis pro Feld (2.Sprosse)** Sprossenpreis nach Anzahl der Felder für die zweite Sprosse, wenn im Sprossenaufbau Kreuzungspunkte vorhanden sind. Der Preis wird bei den Berechnungsarten `Felder`, `Feld +LM`, `Feld+K+R` und `Spezial` ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vkfeld2`, `pokospro.ekfeld2`

**Preis pro Feld 2 (2.Sprosse)** Sprossenpreis nach Anzahl der Felder für die zweite Sprosse, wenn im Sprossenaufbau keine Kreuzungspunkte vorhanden sind. Der Preis wird bei den Berechnungsarten `Felder`, `Feld +LM`, `Feld+K+R` und `Spezial` ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vk2feld2`, `pokospro.ek2feld2`

**Preis pro Laufmeter (2.Sprosse)** Preis pro laufendem Meter für die zweite Sprosse. Der Preis wird bei den Berechnungsarten `LM`, `LM+K+R`, `LM+K`, `LM+R`, `Feld+LM` und `Spezial` ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vklaufm2`, `pokospro.eklaufm2`

**Preis pro Rand (2.Sprosse)** Preis pro Randverbindung für die zweite Sprosse. Der Preis wird bei den Berechnungsarten `R`, `LM+K+R`, `LM+R`, `K+R`, `Feld+K+R` und `Spezial` ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vkrand2`, `pokospro.ekrand2`

**Mindestlaufmeter (2.Sprosse)** Mindestlänge der zweiten Sprosse in Meter, die für den Preis berechnet wird. Wenn die Sprosse weniger Laufmeter misst, als die Mindestlaufmeter, dann wird der Preis für die Mindestlaufmeter berechnet. Der Preis wird bei der Berechnungsart `LM` ausgewertet.
**Technische Info:** numerisches Feld, DB-Feld: `pokospro.vkminlm2`, `pokospro.ekminlm2`

#### Fußzeile

In diesem Bereich werden die Bezeichnung des Artikels und das Kennzeichen der Warengruppe des Artikels angezeigt.

### Produktionskostenkalkulation

**Verkauf > Auftragserfassung > Register Positionen > Preisfeld > `<Strg>` + `<F10>`**

In diesem Dialog werden die Ergebnisse der Kostenkalkulation angezeigt. Sie können die Werte teilweise bearbeiten.

In der Vorgangserfassung werden zunächst nur die Materialkosten angezeigt. Die Maschinen- und Personalkosten werden Ihnen erst angezeigt, wenn der Vorgang in ein Produktionssystem eingelastet wurde.

Der Dialog hat folgende Register:
- "Produktionskostenkalkulation - Übersicht" auf Seite D-1373
- "Produktionskostenkalkulation - Details" auf Seite D-1375

### Produktionskostenkalkulation – Übersicht

**Verkauf > Auftragserfassung > Register Positionen > Preisfeld > `<Strg>` + `<F10>` > Übersicht**

**Abb. D-136 Produktionskostenkalkulation – Übersicht**

In diesem Register werden die Produktionskosten der gewählten Position angezeigt. Sie können die kalkulierte Menge und den Stückpreis der Positionen bearbeiten.

Wenn für einen Bearbeitungsartikel Maschinen- oder Personalkosten berechnet werden, dann wird die entsprechende Artikelnummer und -bezeichnung des Positionsartikels in der Registerüberschrift über der Tabelle angezeigt.

Mit `<F2>` wechseln Sie in die Detailansicht, in der Sie weitere Daten bearbeiten können.

> **Kalkulation erst nach Übermittlung an die Produktion**
> Je nach Systemkonfiguration werden Ihnen die Produktionskosten erst angezeigt, wenn Sie den Auftrag bereits an die Produktion übergeben haben. Wenn Sie den Auftrag noch nicht an die Produktion übergeben haben, werden nur die Materialkosten angezeigt.

#### Übersicht

- **Kostentyp:** Anzeige des Typs der Produktionskosten.
    - Materialkosten
    - interner DB
    - Montagekosten
    - Maschinenkosten
    - Personalkosten
    - Fixkosten
    - Zukauf
    **Technische Info:** Anzeigefeld, DB-Feld: `poskost.satztyp`
- **Artikel:** Anzeige der Artikelnummer.
    **Technische Info:** Anzeigefeld, DB-Feld: `poskost.artnr`
- **Kostenstelle:** Bezeichnung der Kostenstelle für statistische Auswertungen.
    **Technische Info:** alphanumerisches Feld, DB-Feld: `poskost.kostenst`
- **Phy. Menge:** Anzeige der physikalischen Positionsmenge (tatsächliche Menge), z. B. Glasfläche.
    **Technische Info:** Anzeigefeld, DB-Feld: `poskost.phymenge`
- **Kalk. Menge:** Anzeige der kalkulierten Positionsmenge, z. B. Glasfläche + Verschnitt.
    **Technische Info:** Anzeigefeld, DB-Feld: `poskost.pme`
- **ME-Preis:** Anzeige des Preises pro Mengeneinheit der Position.
    **Technische Info:** Anzeigefeld, DB-Feld: `poskost.ppme`
- **Stückpreis:** Preis pro Stück der Position.
    **Technische Info:** numerisches Feld, DB-Feld: `poskost.stprs`

#### Fußzeile

Summen der jeweiligen Satztypen. Folgende Abkürzungen werden angezeigt:
- **Mat.:** Materialkosten.
- **IntDB:** Interner Deckungsbeitrag.
- **Mont.:** Montagekosten.
- **Masch.:** Maschinenkosten.
- **Pers.:** Personalkosten.

### Produktionskostenkalkulation – Details

**Verkauf > Auftragserfassung > Register Positionen > Preisfeld > `<Strg>` + `<F10>` > Register Details**

**Abb. D-137 Produktionskostenkalkulation - Details**

In diesem Register werden die Detaildaten der ermittelten Produktionskosten angezeigt. Sie können die Werte der gewählten Position bearbeiten und so die Produktionskosten neu kalkulieren.

Mit `<Bild hoch>`, `<Bild runter>` können Sie zwischen den einzelnen Kosten der aktuellen Position navigieren.

Wenn für einen Bearbeitungsartikel Maschinen- oder Personalkosten berechnet werden, dann wird die entsprechende Artikelnummer und -bezeichnung des Positionsartikels in der Registerüberschrift über der Tabelle angezeigt.

#### Details

Je nach Kostentyp werden verschiedene Felder angezeigt:

**Produktionsposition** Produktionspositionsnummer bei Produktionskosten. Bei bestellten Bearbeitungen wird hier die entsprechende Positionsnummer der Bestellung angezeigt, in der das Unterteilt bestellt ist.
**Technische Info:** Anzeigefeld, DB-Feld: `poskost.plfdpos`

**Kostentyp** Anzeige des Typs der Produktionskosten.
**Technische Info:** Anzeigefeld, DB-Feld: `poskost.satztyp`

**Manuelle Änderung** Angabe, ob die Werte überschrieben wurden. Wenn die Produktionskosten geändert werden, wird **Manuell** in dem Feld angezeigt. Sie können den Inhalt im Feld nicht bearbeiten.
**Technische Info:** Anzeigefeld, DB-Feld: `poskost.manuell`

**Beschaffungsart** Anzeige der Beschaffungsart des gewählten Artikels. Der Wert kann nur bei den Satztypen Maschinenkosten und Personalkosten bearbeitet werden.
- **Keine:** Keine Beschaffungsart, z. B. für Dienstleistungen.
- **Bestellung:** Artikel muss beim Lieferanten bestellt werden.
- **Lager:** Artikel wird dem Lager entnommen.
- **Produktion:** Artikel wird produziert.
- **Mitgelief.:** Artikel wird vom Kunden mitgeliefert, z. B. zur weiteren Bearbeitung.
- **n. verfüg.:** Artikel ist nicht verfügbar.
**Technische Info:** Toggle-Feld, DB-Feld: `poskost.beschaffart`

**Stückzahl** Artikelmenge in der Stückliste der Position. Bei den Produktionskosten entspricht die Stückzahl immer 1. Für Maschinenkosten wird in der Regel keine Stückzahl angezeigt.
**Technische Info:** Anzeigefeld, DB-Feld: `poskost.menge`

**Artikel** Nummer des Artikels, für den die Kosten ermittelt werden.
**Technische Info:** Anzeigefeld, DB-Feld: `poskost.artnr`

**Kopfartikel** Artikels, dem der gewählte Artikel als Unterteil angehängt ist. Wenn der Artikel selbst der Kopfartikel ist, bleibt das Feld leer.
**Technische Info:** Anzeigefeld, DB-Feld: `poskost.refartnr`

**Produktionssubnr.** Personal-Betriebsmittelnummer. Sie können den Wert nicht bearbeiten. Dieses Feld wird nur beim Satztypen Maschinenkosten angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: `poskost.psbmnr`

**Betriebsmittelnr.** Nummer des Betriebsmittels, das für die Berechnung herangezogen wird. Bei Anbindung an A+W Production wird hier die Maschinen-ID und die Bezeichnung angezeigt. Dieses Feld wird nur beim Satztypen Maschinenkosten und Personalkosten angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: `poskost.bmnr`

**Logisches Betriebsmittel** Logisches Betriebsmittelnummer. Bei Anbindung an A+W Production wird hier die ID der logischen Maschine und deren Bezeichnung angezeigt. Dieses Feld wird nur beim Satztypen Maschinenkosten angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: `poskost.psbmnr`

**Arbeitsgangklasse** Nummer der Arbeitsgangklasse für die Produktionsplanung. In einer Arbeitsgangklasse können mehrere Arbeitsgänge zusammengefasst werden. Dieses Feld wird nur bei den Satztypen Maschinenkosten und Personalkosten angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: `poskost.agknr`

**Arbeitsgang** Nummer des Arbeitsgangs für die Produktionsplanung. Dieses Feld wird nur bei den Satztypen Maschinenkosten und Personalkosten angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: `poskost.agnr`

**Personalnummer** Personalklassennummer. Sie können den Wert nicht bearbeiten. Dieses Feld wird nur beim Satztypen Personalkosten angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: `poskost.pknr`

**Kostenstelle** Bezeichnung der Kostenstelle für statistische Auswertungen.
**Technische Info:** alphanumerisches Feld, DB-Feld: `poskost.kostenst`

**Grundmengeneinheit** Grundmengeneinheit, die dem Artikel in den Stammdaten zugewiesen wurde, z. B. Quadratmeter, Stück. Der Wert wird zur Berechnung des Stückpreises für die Satztypen Maschinenkosten und Personalkosten herangezogen. Sie können den Wert nicht bearbeiten. Dieses Feld wird nur bei den Satztypen Maschinenkosten und Personalkosten angezeigt.
**Technische Info:** numerisches Feld, DB-Feld: `poskost.lugme`

**Variante** Anzeige der Variantennummer des Artikels.
**Technische Info:** numerisches Feld, DB-Feld: `poskost.variante`

**Menge/Physikalische** Physikalische Menge der Position (tatsächliche Menge), z B. Glasfläche, Arbeitsdauer. Die physikalische Menge dient als Berechnungsgrundlage für die kalkulatorische Menge und den Stückpreis. Das Feld entspricht der Spalte **Phy. Menge** im Register **Übersicht**.
**Technische Info:** numerisches Feld, DB-Feld: `poskost.phymenge`

**Verlust** Prozentualer Verlust der Position, z. B. Materialverlust, Zeitverlust. Der Prozentsatz des Verlusts wird auf die kalkulierte Menge gerechnet. Wenn Sie einen negativen Verlust angeben, wird die kalkulierte Menge geringer.
**Technische Info:** numerisches Feld, DB-Feld: `poskost.verlust`

**Menge/Kalkulation** Kalkulierte Menge der Position, z. B. Glasfläche + Verschnitt. Die kalkulierte Menge wird aus der physikalischen Menge inklusive Verlust berechnet:
`physikalische Menge + Verlust / 100 x physikalische Menge`
Das Feld entspricht der Spalte **Kalk. Menge** im Register **Übersicht**.
**Technische Info:** numerisches Feld, DB-Feld: `poskost.pme`

**Mengeneinheitspreis** Preis pro Grundmengeneinheit der Position. Der Mengeneinheitspreis wird zur Berechnung des Stückpreises herangezogen. Das Feld entspricht der Spalte **ME-Preis** im Register **Übersicht**.
**Technische Info:** numerisches Feld, DB-Feld: `poskost.ppme`

**Stückpreis** Preis pro Stück der Position. Der Stückpreis berechnet sich aus Mengeneinheitspreis und der kalkulierten Mengen:
`Mengeneinheitspreis x kalkulierte Menge`
Bei den Satztypen Maschinenkosten und Personalkosten wird zusätzlich die Grundmengeneinheit zur Berechnung des Stückpreises herangezogen:
`Mengeneinheitspreis x kalkulierte Menge / Grundmengeneinheit`
**Technische Info:** numerisches Feld, DB-Feld: `poskost.stkprs`

**Datum** Erfassungsdatum der Position.
**Technische Info:** Datumsfeld, DB-Feld: `poskost.datum`

**Mengeneinheitspreis/Fertigmeldung** Preis pro Mengeneinheit bei Fertigmeldung.
**Technische Info:** numerisches Feld, DB-Feld: `poskost.fppme`

**Stückpreis/Fertigmeldung** Stückpreis bei Fertigmeldung in Eigenwährung.
**Technische Info:** numerisches Feld, DB-Feld: `poskost.fstprs`

**(Stückpreis) in Fremdwährung** Stückpreis in Fremdwährung.
**Technische Info:** numerisches Feld, DB-Feld: `poskost.stkprsfw`

**(Stückpreis/Fertigmeldung in Fremdwährung)** Stückpreis bei Fertigmeldung in Fremdwährung.
**Technische Info:** numerisches Feld, DB-Feld: `poskost.fstkprsfw`

#### Fußzeile

Die Fußzeile ist zum Register **Übersicht** beschrieben:
⇨"Fußzeile" auf Seite D-1374

### Preiskalkulation

**Verkauf > Preiskalkulation**

**Abb. D-138 Preiskalkulation**

In diesem Dialog berechnen Sie die Verkaufspreise anhand der definierten Konditionen. Der berechnete Preis dient nur Informationszwecken und wird nicht gespeichert.

Die Steuerelemente sind zum Dialog Auftragserfassung beschrieben:
⇨ "Auftragserfassung" auf Seite D-1134

## Freischaltung

Je nach Systemkonfiguration werden Aufträge bei der Erfassung nicht freigeschaltet, z. B. wenn der Erfasser nicht ausreichend Rechte hat, der Deckungsbeitrag unterschritten oder das Firmenlimit überschritten wird. Diese Aufträge müssen für die weitere Bearbeitung manuell freigeschaltet werden, um sie weiter an das System, also an Produktion, Einkauf, Versand, und Lager, zu übergeben.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Auftragsfreischaltung" auf Seite D-1380
- "Autorisierung" auf Seite D-1383

### Auftragsfreischaltung

**Verkauf > Auftragsfreischaltung > Freischaltung**

**Abb. D-139 Auftragsfreischaltung**

In diesen Dialogen suchen und schalten Sie einen Auftrag zur weiteren Bearbeitung frei. Sie können einen Auftrag nur freischalten, wenn Sie die entsprechenden Rechte besitzen. Je nach Grund der Auftragssperrung werden unterschiedliche Rechte für die Auftragsfreischaltung benötigt.

Im Suchdialog **Auftragsfreischaltung** können Sie die Suche zur Freischaltung filtern:
- **Suchkriterien eingeben > [Start]:** Sie können Abteilung oder Erfasser und/oder Grund in dem vorgegebenen Haus wählen. Es werden alle Aufträge angezeigt, die den Kriterien entsprechen. Wenn Sie keine Kriterien angeben, werden in der Trefferliste alle nicht freigeschalteten Aufträge angezeigt.
- **[Individuell] > Grund eingeben > Haus, Erfasser angeben > [OK]:** Sie müssen zunächst einen Grund eingeben und können anschließend im Dialog Freischaltung das Haus und/oder den Erfasser wählen.

Im Dialog **Auftragsfreischaltung** werden alle Aufträge angezeigt, die den Suchkriterien entsprechen.
- Mit `<Shift>` + `<F5>` können Sie den markierten Auftrag in der Auftragserfassung öffnen.
- Mit `<Strg>` + `<F9>` können Sie alle Aufträge freischalten.
- Mit `<Shift>` + `<F9>` können Sie ab dem markierten Auftrag alle Aufträge freischalten.
- Mit `<Shift>` + `<F12>` öffnen Sie den Dialog Sperrgründe für die nicht erfolgte Freischaltung. In diesem Dialog werden die Gründe für die Sperrung des Auftrags angezeigt. Der Dialog wird nur angezeigt, wenn ein Auftrag aus mehr als einem Grund gesperrt ist.
- Mit `<F3>` schalten Sie die gewählten Aufträge frei.

#### Kopfzeile

In diesem Bereich werden die Suchkriterien angezeigt, die Sie festgelegt haben. Sie können die Suchkriterien nachträglich nicht mehr bearbeiten. Für eine neue Suche müssen Sie den Dialog schließen und neu aufrufen.

#### Übersicht

In diesem Bereich werden die Aufträge angezeigt, die den Suchkriterien entsprechen und freigeschaltet werden können. Sie können nur die Werte in den Spalten **Frei** und **LSp** bearbeiten. Die übrigen Spalten dienen der Information.

- **Auftrag:** Nummer des Auftrags, der noch nicht freigeschaltet ist.
    **Technische Info:** Anzeigefeld, DB-Feld: `kauf.auftrnr`
- **Frei:** Angabe über die Freischaltung des Auftrags. Wenn das Feld ausgegraut ist, dann ist die Freischaltung aus datentechnischen Gründen nicht möglich, oder Sie besitzen nicht die entsprechenden Rechte für die Freischaltung.
    - **NEIN:** Der Auftrag wird noch nicht freigeschaltet.
    - **JA:** Der Auftrag wird sofort freigeschaltet.
    - **NIE:** Der Auftrag wird nie freigeschaltet.
    - **VS:** Der Auftrag wird nur an die Versandsteuerung übergeben.
    **Technische Info:** Toggle-Feld, DB-Feld: `kauf.tekap.kz`
- **Kunde, Name:** Nummer und Name des Kunden aus dem Auftrag.
    **Technische Info:** Anzeigefelder, DB-Felder: `kauf.kunr`, `mp.name`
- **Termin:** Geplanter Liefertermin.
    **Technische Info:** Anzeigefeld, DB-Feld: `kauf.Itideal`
- **Abruf:** Angabe, ob der Auftrag nur bei Abruf geliefert wird.
    - **J:** Der Auftrag wird nur bei Anforderung durch den Kunden geliefert.
    - **N:** Der Auftrag wird standardmäßig geliefert.
    **Technische Info:** Anzeigefeld, DB-Feld: `kauf.abrufkz`
- **User, Abtnr:** Nummer und Abteilungsnummer des Auftrags-Erfassers.
    **Technische Info:** Anzeigefelder, DB-Felder: `kauf.eusr`, `kauf.abtnr`
- **Erfasst:** Datum der Auftragserfassung.
    **Technische Info:** Anzeigefeld, DB-Feld: `kauf.edat`
- **Haus:** Mandantennummer (Hausnummer), zu der der Auftrag zugeordnet ist.
    **Technische Info:** Anzeigefeld, DB-Feld: `kauf.hausnr`
- **LSp:** Limit-Sperre. Angabe, ob der Auftrag gesperrt ist. Sie können Aufträge nur freischalten, wenn Sie die entsprechenden Rechte besitzen. Sie benötigen spezielle Rechte, wenn Sie Aufträge freischalten wollen, die das Firmenlimit oder das Allgemeines Kredit-Versicherungslimit (AKV-Limit) überschritten haben.
    - **J:** Die Limit-Sperre ist aktiv. Das Feld **Frei** wird gesperrt und der Wert automatisch auf NEIN gesetzt.
    - **N:** Die Limit-Sperre ist deaktiviert. Der Auftrag kann freigeschaltet werden.
    **Technische Info:** Toggle-Feld, DB-Feld: `kauf.limsperre`
- **Bemerkung:** Zusatz-Information zum Auftrag.
    **Technische Info:** Anzeigefeld, DB-Feld: `kauf.lusperrmodus`
- **Info:** Anzeige, ob Auftrags-Informationen hinterlegt sind. Wenn in der Spalte ein I angezeigt wird, sind Informationen für den Auftrag hinterlegt. Mit `<F5>` öffnen Sie den Dialog Anmerkungen mit den hinterlegten Informationen.
    **Technische Info:** Anzeigefeld

> **Status-Anzeige**
> In dem Dialog Auftragserfassung wird in dem Auftrag, der durch lokale Einstellungen oder nicht geeignete Daten nicht direkt freigeschaltet wurde, die Status-Anzeige (rechts oben) ausgegeben, dass der Auftrag nicht freigeschaltet wurde.

### Autorisierung

**Verkauf > Auftragsfreischaltung > Autorisierung**

**Abb. D-140 Autorisierung**

In diesem Dialog autorisieren Sie einen Mitarbeiter, einen Auftrag freizuschalten, selbst wenn dieser Auftrag das Kreditlimit überschreitet. Die maximale Höhe der Überschreitung legen Sie fest, indem Sie den neuen Wert entsprechend erhöhen oder einen Wert im Feld Maximale Werterhöhung eintragen.

Die Funktionen sind von den Einstellungen in den Stammdaten und der jeweiligen Systemkonfiguration und abhängig. Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

**Vorgang** Nummer und Art des Vorgangs. Wenn Sie eine Nummer angegeben haben, wird die Vorgangsart im Klartext angezeigt.
**Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: `kauffrei.auftrnr`

**Laufende Änderungsnr.** Nummer des Änderungsvorgangs. Die aktuelle Änderungsnummer wird automatisch eingetragen. Sie können eine kleinere Änderungsnummer angeben, um den entsprechenden Änderungsstand einzusehen.
**Technische Info:** numerisches Feld, DB-Feld: `kauffrei.aendernr`

> **Erhöhung der Änderungsnummer**
> Sie können nur den jeweils letzten Änderungsstand bearbeiten, ohne dass die Änderungsnummer erhöht wird. Wenn Sie einen weiter zurückliegenden Änderungsstand abrufen und bearbeiten, werden die Änderungen unter einer neuen Änderungsnummer gespeichert.

**Kunde** Kundenname aus dem Vorgang. Wenn Sie die Vorgangs-Nummer angegeben haben, wird der Kunde im Klartext angezeigt.
**Technische Info:** Anzeigefeld, DB-Feld: `kauf.kunr`

**Autorisierter Mitarbeiter** Nummer und Name des Mitarbeiters, für den die Autorisierung eingerichtet wird. Wenn Sie eine Nummer angegeben haben, wird der Name des Mitarbeiters im Klartext angezeigt.
**Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: `kauffrei.aendmanr`

**Alter Wert** Alter Nettototal-Wert des Vorgangs. Als Wert wird immer der aktuelle Nettototal-Wert des Vorgangs herangezogen.
**Technische Info:** numerisches Feld

**Neuer Wert** Obergrenze für den neuen Nettototal-Wert des Vorgangs. Der Wert muss höher sein, als der alte Nettototal-Wert. Der Wert ist abhängig vom Feld **Maximale Werterhöhung**:
- Wenn das Feld **Maximale Werterhöhung** leer ist und Sie einen neuen Nettototal-Wert angeben, wird im Feld **Maximale Werterhöhung** automatisch die Differenz zwischen altem und neuem Nettototal-Wert angezeigt.
- Wenn im Feld **Maximale Werterhöhung** bereits ein Wert steht und Sie einen neuen Nettototal-Wert angeben, wird der Wert im Feld **Maximale Werterhöhung** automatisch an den neuen Wert angepasst.
**Technische Info:** numerisches Feld

**Maximale Werterhöhung** Maximale Erhöhung der Kosten, die den alten Nettototal-Wert des Auftrags übersteigt. Der Wert ist abhängig vom Feld **Neuer Wert**:
- Wenn das Feld **Neuer Wert** leer ist und Sie einen neuen Maximalwert angeben, wird im Feld **Neuer Wert** automatisch die Differenz zwischen altem und neuem Nettototal-Wert angezeigt.
- Wenn im Feld **Neuer Wert** bereits ein Wert steht und Sie einen neuen Maximalwert angeben, wird der Wert im Feld **Neuer Wert** an den neuen Wert angepasst.
**Technische Info:** numerisches Feld, DB-Feld: `kauffrei.maxpreisdiff`

#### Fußbereich

**Mitarbeiter** Anzeige des Namens des autorisierenden Mitarbeiters.
**Technische Info:** Anzeigefeld, DB-Feld: `kauffrei.automanr`

**Datum** Anzeige des Datums, an dem die Autorisierung freigeschaltet wurde. Standardmäßig wird das aktuelle Datum angezeigt.
**Technische Info:** Anzeigefeld

## Lieferung

Standardmäßig werden Lieferscheine im Modul **Versandsteuerung** erfasst und verwaltet, weil die Buchungen von verpackten und fertigen Produkten aus anderen Modulen bzw. Programmen automatisch an die Versandsteuerung weitergeleitet werden. Wenn das Modul Versandsteuerung nicht konfiguriert ist, können Sie die Lieferscheine im Modul **Verkauf** erstellen.

Je nach Konfiguration können Sie zu einem Auftrag einen Lieferplan erstellen. Im Lieferplan können Sie den Auftrag in Teillieferungen aufteilen. Für jede (Teil-)Lieferung eines Auftrags wird ein Lieferschein erstellt. Der Lieferschein dient zum Nachweis der Auftragsabwicklung für die Logistik und Spedition und zur Auskunft für den Kunden. Je nach Art der Lieferungen unterscheidet das System zwischen Komplett- und Teillieferscheinen. Sie können Lieferscheine automatisch oder manuell erstellen und bearbeiten.

Die Funktionen sind von den Einstellungen in den Stammdaten und der jeweiligen Systemkonfiguration und abhängig.

Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Lieferplan" auf Seite D-1386
- "Lieferinformation – Details der Auslieferung" auf Seite D-1388
- "Lieferscheine (automatisch)" auf Seite D-1392
- "Lieferscheine (manuell)" auf Seite D-1394
- "Lieferscheinprotokoll" auf Seite D-1396

### Lieferplan

**Verkauf > Auftragserfassung > Positionsebene > `<F4>` > Lieferplan**

**Abb. D-141 Lieferplan**

In diesem Dialog erfassen Sie den Lieferplan. Sie können für einen Auftrag mehrere Teillieferungen festlegen. Wenn Sie einen Lieferschein erzeugen, werden die Daten aus dem Lieferplan herangezogen und ausgewertet. Sie können einen Lieferschein für einen Auftrag erst dann erzeugen, wenn die Erfassung der Positionen abgeschlossen ist.

#### Übersicht

- **Pos.:** Nummer der Position aus dem Auftrag.
    **Technische Info:** Anzeigefeld, DB-Feld: lieferplan.posnr
- **Lief.:** Nummer der (Teil-)Lieferung.
    **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: liefplan.subnr
- **Lieferdatum:** Voraussichtlicher Termin der (Teil-)Lieferung.
    **Technische Info:** Datumsfeld, DB-Feld: liefplan.ltplan
- **Ankunftstag:** Voraussichtlicher Ankunftstag der (Teil-)Lieferung.
    **Technische Info:** Anzeigefeld, DB-Feld: liefplan.ankunft
- **Artikel:** Bezeichnung des Artikels.
    **Technische Info:** Anzeigefeld, DB-Feld: liefplan.artbez1
- **Route:** Nummer der Route der (Teil-)Lieferung.
    **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: liefplan.route
- **Gesamt:** Gesamt-Stückzahl der bestellten Position aus dem Auftrag.
    **Technische Info:** numerisches Feld, DB-Feld: liefplan.geslief
- **Gelief:** Bereits ausgelieferte Menge aus der Position des Auftrags.
    **Technische Info:** numerisches Feld, DB-Feld: liefplan.geliefert
- **Verpackt:** Stückzahl der verpackten Position des Auftrags.
    **Technische Info:** numerisches Feld, DB-Feld: liefplan.gespack
- **Geplant:** Geplante Stückzahl der Position, die in dieser (Teil-)Lieferung ausgeliefert werden soll.
    **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: liefplan.zuliefern

#### Details

Das Register Details wird zurzeit nicht genutzt.

### Lieferinformation – Details der Auslieferung

**Verkauf > Auftragserfassung > Kopf-, Fußbereich > `<F4>` > Lieferinformation**

**Abb. D-142 Details der Auslieferung**

In diesem Dialog werden die Details der Auslieferung angezeigt, z. B die Route und der geplante Liefertermin. Die verschiedenen Lieferinformationen sind besonders wichtig, wenn sich Produktions- und Auslieferungshaus unterscheiden.

Einige Felder in den Bereichen Produktions- und Auslieferungshaus können nur vorbelegt werden, wenn Sie mit interner Mandantentrennung arbeiten und die Via-Plant-Logik aktiv ist.

Die Felder in diesem Dialog werden vom System vorbelegt. In der Regel müssen Sie die Felder nicht bearbeiten.

#### Produktionshaus

**Lieferadresscode, Lieferadressname** Code und Name der gespeicherten Lieferadresse des Produktionshauses.
**Technische Info:** alphanumerische Felder, DB-Felder: kauf.lort, kauf.lort

**Versandart** Nummer und Bezeichnung der Versandart. Wenn eine Nummer angegeben wird, wird die Bezeichnung der Versandart im Klartext angezeigt.
**Technische Info:** numerisches Feld, Anzeigefeld, DB-Feld: kauf.versandartvia

**gepl.Liefertermin** Datum der geplanten Auslieferung im Produktionshaus. Das Datum gibt an, an welchem Tag die Lieferung das Produktionshaus voraussichtlich verlässt.
**Technische Info:** Datumsfeld, DB-Feld: kauf.ltplan

**Route** Nummer der Route, über die ausgeliefert wird.
**Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: kauf.routenr

**Fahrtzeit** Voraussichtliche Fahrtdauer zum Auslieferungshaus. Wenn eine Route angegeben ist, für die eine Fahrtzeit hinterlegt ist, wird die Fahrtzeit im Klartext angezeigt. Sie kann sich auf den Liefertermin auswirken.
**Technische Info:** Anzeigefeld

**Routentage** Anzeige der Wochentage, an denen die gewählte Route gefahren wird. Wenn eine Route angegeben ist, werden die zugehörigen Routentage aus den Stammdaten herangezogen und im Klartext angezeigt.
**Technische Info:** Anzeigefeld

**Region** Anzeige der Versandregion. Mehrere Auslieferungsrouten können zu einer Versandregion zusammengefasst werden, wenn das System entsprechend konfiguriert ist. Die Versandregion wird zu der entsprechenden via Route aus den Stammdaten herangezogen. Das Feld ist vorbelegt, wenn das Modul Regionalrouten konfiguriert ist und der aktuellen Route eine Versandregion zugeordnet ist. Zudem müssen Sie mit interner Mandantentrennung arbeiten und die Via-Plant-Logik muss aktiv sein.
**Technische Info:** Anzeigefeld, DB-Feld: route.region

**via Haus** Nummer des Auslieferungshauses, über das die Lieferung versendet wird. Das Auslieferungshaus legen Sie im Kopfbereich im Feld Route mit `<F5>` fest.
**Technische Info:** Anzeigefeld, DB-Feld: kauf.vsvia

**Haus** Anzeige der Mandantennummer (Hausnummer), in der der Auftrag angelegt wird.
**Technische Info:** Anzeigefeld, DB-Feld: kauf.hausnr

**Tonnage** Anzeige der Nutzlast des Fahrzeugs in Kilogramm. Dieses Feld ist frei konfigurierbar.
**Technische Info:** Anzeigefeld

**Kalender** Anzeige, ob der Kalender bei der Lieferterminbestimmung herangezogen wird. Sie können in den Routenstammdaten für jede Route festlegen, ob der Kalender ausgewertet wird.
- Der Kalender wird bei der Lieferterminbestimmung berücksichtigt.
- Der Kalender wird bei der Lieferterminbestimmung nicht berücksichtigt.
**Technische Info:** Checkbox

#### Auslieferungshaus

Dieser Bereich wird nur angezeigt, wenn Sie mit interner Mandantentrennung arbeiten und die Via-Plant-Logik aktiv ist.

**Lieferadresscode, Lieferadressname** Code und Name der Lieferadresse des Auslieferungshaus.
**Technische Info:** alphanumerische Felder, DB-Felder: kauf.lort, kauf.lort

**Versandart** Nummer der Versandart, z. B. LKW. Wenn eine Nummer ausgewählt ist, wird die Bezeichnung der Versandart im Klartext angezeigt.
**Technische Info:** Anzeigefeld, DB-Feld: kauf.versandartvia

**Ankunft in via Haus** Datum, an dem die Lieferung voraussichtlich im Auslieferungshaus ankommt.
**Technische Info:** Anzeigefeld

**Handlingszeit** Handlings-Zeit, um die Lieferung im Auslieferungshaus auf- oder abzuladen.
**Technische Info:** numerisches Feld

**Route** Nummer der Route, über die an den Kunden ausgeliefert wird. Die Route muss in den Stammdaten als via Route für das Auslieferungshaus angelegt sein:
⇨ Stammdaten, "Routen" auf Seite B-259
**Technische Info:** Plichtfeld, numerisches Feld, DB-Feld: kauf.routenr

**Fahrtzeit** Anzeige der Fahrtdauer zum Auslieferungshaus. Wenn eine Route angegeben ist, für die eine Fahrtzeit hinterlegt ist, wird die Fahrtzeit im Klartext angezeigt.
**Technische Info:** Anzeigefeld

**Routentage** Anzeige der Wochentage, an denen die gewählte Route gefahren wird. Wenn eine Route angegeben ist, werden die zugehörigen Routentage aus den Stammdaten herangezogen und im Klartext angezeigt.
**Technische Info:** Anzeigefeld

**Region** Anzeige des Länderkennzeichens mit Benennung der Versandregion.
**Technische Info:** Anzeigefeld

**Tonnage** Anzeige der Nutzlast des Fahrzeugs in Kilogramm. Dieses Feld ist frei konfigurierbar.
**Technische Info:** Anzeigefeld

**Gepl.LiefTerm** Geplantes Lieferdatum vom Auslieferungshaus zum Kunden.
**Technische Info:** Anzeigefeld, DB-Feld: kauf.ltplan

**Kalender** Anzeige, ob der Kalender bei der Lieferterminbestimmung herangezogen wird. Sie können in den Routenstammdaten für jede Route festlegen, ob der Kalender ausgewertet wird.
- Der Kalender wird bei der Lieferterminbestimmung berücksichtigt.
- Der Kalender wird bei der Lieferterminbestimmung nicht berücksichtigt.
**Technische Info:** Checkbox

#### Kunde

**Wunschtermin** Gewünschter Liefertermin des Kunden.
**Technische Info:** Datumsfeld, DB-Feld: kauf.Itideal

**Ankunftstag** Datum, an dem die Lieferung voraussichtlich beim Kunden eintrifft. Der Ankunftstag wird anhand des Liefertermins, der Fahrtdauer und der Routentage errechnet.
**Technische Info:** Anzeigefeld

**Terminstatus** Statuskennzeichen, ob der Wunschtermin des Kunden und der berechnete Ankunftstermin der Lieferung übereinstimmen.
**Technische Info:** Anzeigefeld

**Tab. D-12 Terminstatus**

| Symbol | Statuskennzeichen | Bedeutung |
| :--- | :--- | :--- |
| (grün) | grün | Der voraussichtliche Liefertermin entspricht exakt dem Wunschtermin des Kunden. |
| (gelb) | gelb | Der voraussichtliche Liefertermin liegt vor dem Wunschtermin des Kunden. |
| (rot) | rot | Der voraussichtliche Liefertermin liegt nach dem Wunschtermin des Kunden. |

#### Kalenderausschnitt

Der Kalenderausschnitt zeigt einen Ausschnitt von drei Wochen um den Wunschtermin des Kunden. Alle Termine, z. B. geplanter Liefertermin, Kundenwunschtermin, Liefertermin im Produktionshaus usw., die in diesem Zeitraum liegen, werden an den entsprechenden Tagen angezeigt. Sie können sich auf den Kalendertagen Informationen über den jeweiligen Termin als Tooltipp anzeigen lassen.

### Lieferscheine (automatisch)

**Verkauf > Lieferscheine > Automatische Freigabe**

**Abb. D-143 Lieferscheine (automatisch)**

In diesem Dialog erzeugen Sie Lieferscheine als Begleitdokumente für die Auftragsauslieferung. Sie können in diesem Dialog auch Rechnungen erzeugen und Vorgänge abschließen.

Wenn das Modul Versandsteuerung in Ihrem System konfiguriert ist, sollten Sie die Lieferscheine nur in der Versandsteurung erstellen. Das System ist standardmäßig nicht für die Erstellung von Lieferscheinen im Modul Verkauf konfiguriert.

> **Inkonsistenz mit der Versandsteuerung**
> Lieferscheine im Verkauf zu erstellen, kann zu Inkonsistenzen mit der Versandsteuerung führen, da die Statusbuchungen, wie z. B. verpackte oder fertig gemeldete Mengen, nur in der Versandsteuerung auf dem aktuellen Stand sind.
> Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

- **Freigabe:** Angabe der Freigabe-Art für den gewählten Vorgang.
    - **Lieferschein:** Für den gewählten Vorgang wird ein Lieferschein erzeugt.
    - **Rechnung:** Für den gewählten Vorgang wird eine Rechnung erzeugt. Sie können eine Rechnung nur für Vorgänge erzeugt, zu denen bereits ein Lieferschein existiert.
    - **LS + Rechnung:** Für den gewählten Vorgang werden Lieferschein und Rechnung erzeugt.
    - **Vorgang abschließen:** Der gewählte Vorgang wird abgeschlossen. Änderungen am Vorgang werden nicht mehr an das System weitergegeben.
- **Hnr:** Mandantennummer (Hausnummer).
- **Vorgang:** Vorgangsnummer. Bei Lieferscheinerzeugung geben Sie die Nummer des Auftrags, bei Rechnungserzeugung die Nummer des Lieferscheins an. Die Auftrags- und die Lieferscheinnummer sind identisch. Für den Lieferschein können Sie zusätzlich die Subnummer bei Teillieferungen angeben.
- **Subnr:** Subnummer des Vorgangs, z. B. vom Teillieferschein. Die Subnummer muss für die Erzeugung eines Lieferscheins angegeben werden.
- **Grp:** Versandgruppe. Lieferscheine können in der Versandplanung einer Versandgruppe zugeordnet werden. Die Versandgruppen werden in den Systemstammdaten hinterlegt. Die Versandgruppe dient als zusätzliches Kennzeichen für die Toursperre.
- **Lieferschein:** Angabe, ob ein Lieferschein oder Teillieferschein existiert. Existiert bereits ein Lieferschein, dann steht in diesem Feld die Angabe existiert.
- **Rechnung:** Rechnungsnummer.
- **Kundennr:** Kundennummer.
- **Kunde:** Kundenname.
- **Datum:** Erfassungsdatum des Vorgangs.
- **Valuta:** Frist der Wertstellung in Tagen.
- **Er.:** Erzeugen. Angabe, ob die Lieferscheine und/oder Rechnungen erzeugt werden sollen.
    - **Ja, erzeugen.**
    - **Nicht erzeugen.**

#### Fußzeile

Kundenname und die Höhe des Nettototal-Betrags werden angezeigt.

Mit `<F2>` werden die folgenden Felder angezeigt:
- **Betrag:** Höhe des Nettototal-Betrags.
- **Erf.:** Mitarbeiternummer des Vorgangserfassers.
- **Erfasser:** Name des Vorgangserfassers.
- **Belegdatum:** Entspricht dem Feld Datum.

### Lieferscheine (manuell)

**Verkauf > Lieferscheine > Manuelle Lieferscheine**

**Abb. D-144 Lieferscheine (manuell)**

In diesem Dialog erzeugen und bearbeiten Sie Lieferscheine manuell. Lieferscheine erzeugen Sie nur dann manuell, wenn Sie Korrekturen in den Auftragsdaten vornehmen müssen, z. B. bei einer abweichenden Liefermenge.

Wenn das Modul Versandsteuerung in Ihrem System konfiguriert ist, sollten Sie die Lieferscheine nur in der Versandsteuerung erzeugen. Das System ist standardmäßig nicht für die Erzeugung von Lieferscheinen im Modul Verkauf konfiguriert.

> **Inkonsistenz mit der Versandsteuerung**
> Lieferscheine im Verkauf zu erzeugen, kann zu Inkonsistenzen mit der Versandsteuerung führen, da die Statusbuchungen, wie z. B. verpackte oder fertig gemeldete Mengen, nur in der Versandsteuerung auf dem aktuellen Stand sind.
> Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

Die Felder und Register sind zum Dialog Auftragserfassung beschrieben:
⇨ "Auftragserfassung" auf Seite D-1134

Zusätzliche werden folgende Felder angezeigt:

#### Kopfbereich

**Auftrag** Nummer des Auftrags und Subnummer. Subnummern vergeben Sie für Teil-Lieferscheine. Mit `<TAB>` wird die nächste freie Subnummer automatisch vergeben. Wenn zu einem Auftrag bereits Lieferscheine erfasst sind, können Sie die Subnummer eingeben und den bereits erstellten Lieferschein aufrufen.

#### Register Allgemein

**Erhalten** Positionsmenge, die bereits mit vorherigen Lieferscheinen ausgeliefert worden ist.

**Gelief.** Menge der Artikel, die mit dem ausgewählten Lieferschein ausgeliefert werden.

### Lieferscheinprotokoll

**Verkauf > Lieferscheine > Protokoll**

**Abb. D-145 Lieferscheinprotokoll**

In diesem Dialog wird das Lieferscheinprotokoll angezeigt. Alle Vorgänge zu den Lieferscheinen sind mit der Angabe des Datums und der Zeit vermerkt.

Wenn Sie mit interner Mandantentrennung arbeiten, öffnet sich zunächst ein Dialog zur Angabe der Mandantennummer (Hausnummer). In dem Protokoll werden nur die Vorgänge zum ausgewählten Haus angezeigt.

> **Lieferscheinprotokoll zu dem aktuellen Tag**
> Ein Lieferscheinprotokoll wird zu dem aktuellen Tag erzeugt. Wenn die Fehlermeldung angezeigt wird, dass die Datei leer oder nicht lesbar ist, dann wurde an diesem Tag noch kein Lieferschein erzeugt.

## Rechnungen

Um Kundenaufträge abzurechnen, werden Rechnungen erzeugt und an die Finanzbuchhaltung (FIBU) übergeben.

Sie können die Rechnungen automatisch oder manuell erstellen. Eine Rechnung kann erst automatisch erstellt werden, wenn ein Lieferschein existiert.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Rechnungen (automatisch)" auf Seite D-1398
- "Positionsinfo" auf Seite D-1401
- "Rechnungen (manuell)" auf Seite D-1403
- "Thekenrechnung" auf Seite D-1404
- "Rechnungen buchen" auf Seite D-1405
- "Abschlagsrechnung (automatisch)" auf Seite D-1408
- "Abschlagsrechnung (manuell)" auf Seite D-1410
- "Schlussrechnung (automatisch)" auf Seite D-1411
- "Schlussrechnung (manuell)" auf Seite D-1412
- "Rechnungsprotokoll" auf Seite D-1413

### Rechnungen (automatisch)

**Verkauf > Rechnungen > Automatische Freigabe**

**Abb. D-146 Rechnungen (automatisch)**

In diesem Dialog erstellen Sie Rechnungen zu Vorgängen und übergeben sie an die FIBU. Sie können die Vorgänge importieren, zu denen Rechnungen erzeugt werden können, oder Sie können die Vorgangsnummern manuell angeben.

Mit `<Strg>` + `<F8>` importieren Sie die Daten aller Vorgänge, für die eine Rechnung erzeugt werden kann. Die Daten werden über eine frei konfigurierbare SQL-Abfrage importiert. Die Anzahl der importierten Daten ist von der jeweiligen SQL-Abfrage abhängig. Sie können die Abfrage nutzen, die standardmäßig von A+W konfiguriert ist oder eine kundenspezifische SQL-Abfrage für den Datenimport festlegen.

Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

In der Fußzeile wird der Kundenname und der Gesamtbetrag aus dem Auftrag angezeigt, für den eine Rechnung erstellt wird.

Wenn Sie eine Rechnung noch nicht gebucht haben, können Sie im Dialog **Rechnungen** zusätzliche Informationen einsehen und die Rechnung bearbeiten, z. B. um Korrekturen vorzunehmen.
⇨ "Rechnungen (manuell)" auf Seite D-1403

In diesem Dialog können Sie zusammen mit der Rechnung auch gleichzeitig den Lieferschein erzeugen oder den Vorgang abschließen.

Mit `<F3>` werden die Rechnungen zu den ausgewählten Aufträgen vom System erzeugt.

#### Register Vorgänge

- **Freigabe:** Angabe, welche Dokumente Sie für den Vorgang freigeben, der im Feld Vorgang angegeben ist.
    - **Rechnung:** Für den Vorgang wird die Rechnung erzeugt.
    - **LS + Rechnung:** Für den Vorgang werden der Lieferschein und die Rechnung erzeugt.
    - **Vorgang abschließen:** Der Vorgang wird abgeschlossen, d. h. er kann nicht mehr bearbeitet werden.
    - **Lieferschein:** Für den Vorgang wird der Lieferschein erzeugt.
    **Technische Info:** Toggle-Feld, DB-Feld: `kauf.vorgang`
- **Hnr:** Anzeige der Mandantennummer (Hausnummer).
    **Technische Info:** Anzeigefeld, DB-Feld: `kauf.hausnr`
- **Vorgang:** Vorgangsnummer.
    **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: `kauf.auftrnr`
- **Subnr:** Nummer des Teillieferscheins. Wenn das Dokument für eine Komplettlieferung erzeugt wird, wird eine 1 angezeigt.
    **Technische Info:** numerisches Feld, DB-Feld: `kauf.subnr`
- **Grp:** Versandgruppe. Lieferscheine können in der Versandplanung einer Versandgruppe zugeordnet werden. Die Versandgruppen werden in den Systemstammdaten hinterlegt. Die Versandgruppe dient als zusätzliches Kennzeichen für die Toursperre.
    **Technische Info:** numerisches Feld, DB-Feld: `lapool.vsgruppe`
- **Lieferschein:** Anzeige, ob ein Lieferschein oder Teillieferschein existiert. Wenn ein Lieferschein existiert, steht in diesem Feld der Eintrag **existiert**.
    **Technische Info:** Anzeigefeld
- **Rechnung:** Nummer des Rechnungsvorgangs, wenn eine Rechnung existiert.
    **Technische Info:** Anzeigefeld
- **Kundennr:** Anzeige der Kundennummer.
    **Technische Info:** Anzeigefeld, DB-Feld: `kauf.kunr`
- **Kunde:** Anzeige des Kundennamens.
    **Technische Info:** Anzeigefeld, DB-Feld: `mp.name`
- **Belegdatum:** Datum der Rechnungserstellung oder Rechnungsbuchung. Standardmäßig wird das Feld mit dem aktuellen Datum vorbelegt. Für Rechnungen und Lieferscheine können Sie mit `<Strg>` + `<B>` zwischen Beleg- und Buchungsdatum wechseln. Über dem Spaltenkopf wird angezeigt, welches Datum gerade angezeigt wird.
    **Technische Info:** Pflichtfeld, Datumsfeld, DB-Feld: `kauf.edat`
- **Valuta:** Frist zur Wertstellung in Tagen bis maximal 99 Tage.
    **Technische Info:** Anzeigefeld, DB-Feld: `kauf.valuta`
- **Er.:** Erzeugen. Angabe, ob die gewählten Dokumente erzeugt werden sollen.
    - Ja, erzeugen.
    - Nicht erzeugen.
    **Technische Info:** Checkbox

Mit `<F2>` wechseln Sie zum Register **Information zum Vorgang**.

#### Register Information zum Vorgang

Die Spalten sind zum Register **Vorgänge** beschrieben:
⇨ "Register Vorgänge" auf Seite D-1399
Zusätzlich werden folgende Spalten angezeigt:

- **Betrag:** Anzeige der Höhe des Rechnungsbetrages.
    **Technische Info:** Anzeigefeld, DB-Feld: `kauf.nettototal`
- **Erf., Erfasser:** Anzeige der Erfassernummer und des Erfassernamens.
    **Technische Info:** Anzeigefelder, DB-Felder: `kauf.eust`, `mitarb.maname`

#### Fußzeile

In der Fußzeile werden der Kundenname und der Rechnungsbetrag aus dem Vorgang angezeigt.

Mit `<F5>` öffnen Sie den Dialog **Positionen**, in dem weitere Details zu den Rechnungspositionen angezeigt werden.
⇨ "Positionsinfo" auf Seite D-1401
