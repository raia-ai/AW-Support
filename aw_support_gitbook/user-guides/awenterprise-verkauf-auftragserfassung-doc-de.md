---
description: "DE_AWEnterprise_Verkauf_4_6"
---


# Softwarereferenz Anmerkungen

---
## Kunden-Artikel-, Lieferanten-Artikel-, Objekt-Artikel-Anmerkungen

**Navigation:** `Verkauf > Auftragserfassung > Positionsebene > <Shift> + <F4> > Anmerkungen > Kunden-Artikel-, Lieferanten-Artikel-, Objekt-Artikel-Anmerkungen`

[Image: Abb. D-105 Anmerkungen zum Kunden, Lieferanten oder Objekt mit einem bestimmten Artikel. The image displays three overlapping dialog boxes for "Anmerkungstexte" (Note Texts) related to an object, a supplier, and a customer respectively, each linked to a specific article.]

In diesen Dialogen werden jeweils Anmerkungen zum aktuellen Artikel des gewählten Kunden, Lieferanten oder Objekts angezeigt. Diese Anmerkungen können nur auf Positionsebene zur gewählten Position angezeigt werden.

Die Anmerkungstexte werden in der Regel in den Stammdaten angelegt. Wenn Sie die Anmerkungstexte bearbeiten und neue hinzufügen, speichern Sie diese mit `<F3>`. Die Änderungen werden in die Stammdaten übernommen und der Dialog wird geschlossen.

Lieferanten-Artikel-Anmerkungen im Verkauf werden nur angezeigt, wenn der markierten Position die Beschaffungsart Bestellung und ein Lieferant zugewiesen ist.

Objekt-Artikel-Anmerkungen werden nur angezeigt, wenn dem aktuellen Vorgang ein Objekt zugeordnet ist.

### Kopfbereich

Die Felder im Kopfbereich sind ausführlich zu den Dialogen Marktpartner-, Objekt-, Artikel-Anmerkungen beschrieben:
⇨ "Marktpartner-, Objekt-, Artikel-Anmerkungen" auf Seite D-248

### Rumpfbereich

**(Eingabezeilen für Text)** Anmerkungstext zum gewählten Artikel des aktuellen Kunden. Mit `<Enter>` wechseln Sie in die nächste Textzeile. Jede Textzeile wird einzeln konfiguriert, d. h. Sie können für jede Zeile die Priorität und den Info-Ort festlegen.
**Technische Info:** alphanumerische Felder, DB-Felder: memo.txt

### Fußbereich

Die Felder und Schaltflächen im Fußbereich sind ausführlich zu den Dialogen Marktpartner-, Objekt-, Artikel-Anmerkungen beschrieben:
⇨ "Marktpartner-, Objekt-, Artikel-Anmerkungen" auf Seite D-248

# Texte

## Texte

Mit Texten können zusätzliche Informationen zu Vorgängen angezeigt werden. Die Texte werden, je nach Text-Art, entweder vom System nach Vorgaben aus den Stammdaten und den Bewegungsdaten generiert oder manuell erfasst. Sie können Texte mit Informationen für Kunden auf verschiedenen Formularen ausdrucken. Texte mit internen Informationen können beim Aufrufen eines Vorgangs automatisch angezeigt werden.

Die Textverwaltung ist von den Einstellungen in den Stammdaten und der jeweiligen Systemkonfiguration abhängig.

Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Anmerkungen" auf Seite D-245
- "Kopf- und Fußtexte" auf Seite D-254
- "Artikel- und Positionstexte" auf Seite D-256
- "Spezielle Texte" auf Seite D-257
- "Floskeln" auf Seite D-258
- "Fremdinformationen" auf Seite D-260
- "Kistensignatur" auf Seite D-261

## Kopf- und Fußtexte

**Navigation:**
- `Verkauf > Auftragserfassung > Kopf-, Fußbereich > <F4> > Texte > Kopftext, Fußtext`
- `Verkauf > Auftragserfassung > Positionsebene > <F4> > Texte > Kopftext, Fußtext`

[Image: Abb. D-106 Kopf- und Fußtexte. The image shows a dialog box with two tabs, "Kopftext" and "Fußtext", for entering header and footer texts for various forms like Angebot, AB, Rechnung, etc.]

In diesem Dialog werden Texte mit zusätzlichen Informationen zum Vorgangskopf oder -fuß angezeigt. Die Texte werden anhand der Textverwaltung aus den Stammdaten generiert. Die Textverwaltung ist zu dem Part Stammdaten beschrieben:
⇨ "Textverwaltung" auf Seite J-395

Sie können die Texte vorgangsbezogen bearbeiten und Floskeln hinzufügen.

Die Texte können auf verschiedenen Formularen ausgedruckt werden. Sie können die Auswahl der entsprechenden Formulare im rechten Teil des Dialogs Texte im Bereich Formulare ändern.

### Register Kopftext

**(Eingabezeilen für Text)** Informationstext zum Kopfbereich. Mit `<Enter>` wechseln Sie in die nächste Textzeile.
**Technische Info:** alphanumerische Felder, DB-Felder: auftxt.txt

### Register Fußtext

**(Eingabezeilen für Text)** Informationstext zum Fußbereich. Mit `<Enter>` wechseln Sie in die nächste Textzeile.
**Technische Info:** alphanumerische Felder, DB-Felder: auftxt.txt

### Formulare

Im Bereich Formulare geben Sie an, auf welchen Formular-Arten der Informationstext ausgegeben wird.
- ☑ Der Informationstext wird auf das gewählte Formular gedruckt. In der Datenbank wird der Wert 1 zugeordnet.
- ☐ Auf das Formular wird kein Informationstext gedruckt. In der Datenbank wird der Wert 0 zugeordnet.
**Technische Info:** Checkboxen, DB-Felder: auftxt.formular

> **i Datenbankbezug für Formulare**
> In der Datenbank werden alle Eingaben pro Formular in einem Formularvektor gespeichert. Alle Formulare sind in der vorgegeben Reihenfolge unter der entsprechenden Nummer im Formularvektor festgelegt (Nr. in der Tabelle Formular-Arten).
> Wenn einem Formular eine 1 zugeordnet ist, dann wird es gedruckt. Ist eine 0 zugeordnet, wird das Formular nicht gedruckt.

**Tab. D-10 Formular-Arten**

| Nr. | Feldinhalt | Bedeutung |
| --- | --- | --- |
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

### Fußbereich

- **Floskeln**: Öffnet den Dialog Floskeln zur Auswahl von bestehenden Floskeln. ⇨ "Floskeln" auf Seite D-258
- **Floskeln neu**: Öffnet den Dialog Floskeln, in dem Sie eigene Floskeln anlegen können. ⇨ "Floskeln" auf Seite D-258

## Artikel- und Positionstexte

**Navigation:** `Verkauf > Auftragserfassung > Positionsebene > <F4> > Texte > Artikeltext, Positionstext`

[Image: Abb. D-107 Artikel- und Positionstexte. The image shows a dialog with tabs for "Artikeltext" and "Positionstext", allowing for specific text entry related to an article or an order position.]

In diesem Dialog werden Texte mit zusätzlichen Informationen zu den Artikeln oder Positionen eines Vorgangs angezeigt.

Die Texte werden aus den Stammdaten und entsprechend den Systemeinstellungen generiert. Die Textverwaltung wird kundenspezifisch konfiguriert und ist zu dem Part Stammdaten beschrieben:
⇨ Stammdaten, "Textverwaltung" auf Seite J-395

Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

Sie können die Texte vorgangsbezogen bearbeiten und Floskeln hinzufügen. Wenn Sie Floskeln für den Artikel- oder Positionstext gewählt haben, können Sie diese vorgangsbezogen bearbeiten.

Die Texte können auf verschiedenen Formularen ausgedruckt werden. Sie können die Auswahl der entsprechenden Formulare im rechten Teil des Dialogs im Bereich Formulare ändern.

### Register Artikeltext

**(Eingabezeile für Text)** Informationstext zum gewählten Artikel. Mit `<Enter>` wechseln Sie in die nächste Textzeile.
**Technische Info:** alphanumerische Felder, DB-Felder: auftxt.txt

### Register Positionstext

**(Eingabezeile für Text)** Informationstext zur gewählten Position. Mit `<Enter>` wechseln Sie in die nächste Textzeile.
**Technische Info:** alphanumerische Felder, DB-Felder: auftxt.txt

### Formulare

Dieser Bereich ist ausführlich zum Dialog Kopf- und Fußtexte beschrieben.
⇨ "Kopf- und Fußtexte" auf Seite D-254

### Fußbereich

Dieser Bereich ist ausführlich zum Dialog Kopf- und Fußtexte beschrieben.
⇨ "Kopf- und Fußtexte" auf Seite D-254

## Spezielle Texte

**Navigation:** `Verkauf > Auftragserfassung > Positionsebene > <F4> > Texte > Spezielle Texte > Rahmentext, Produktkennzeichen, Modelltexte, Logotexte`

[Image: Abb. D-108 Spezielle Texte. A small dialog box titled "Modelltexte" is shown with some dimension values.]

In diesen Dialogen werden spezielle Texte zu den einzelnen Artikeln angezeigt. Die speziellen Texte werden anhand der Stammdaten vom System generiert. Die Textverwaltung ist von den Einstellungen in den Stammdaten und der jeweiligen Systemkonfiguration abhängig. Je nach Konfiguration können Sie die Texte vorgangsbezogen bearbeiten.

Die Dialoge sind nur kundenspezifisch freigeschaltet.

Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

Jedem Text ist eine Textnummer zugewiesen. Unter Umständen wird die Textnummer an die Produktion übergeben, wenn sie dort benötigt wird.

**Tab. D-11 Spezielle Texte**

| Textart | Beschreibung | Textnummer |
| --- | --- | --- |
| **Rahmentext** | Zusätzliche Information zum Rahmentext, der auf den Rahmen gedruckt wird. | 1000 |
| **Produktkennzeichen** | Zusätzliche Informationen zum Produktkennzeichen, z. B. CEKAL-Zertifizierungs-Kennzeichen. | 1003 |
| **Modelltext** | Zusätzliche Information zum Modell. Die Parameter des Modells werden für jede Position als Text angezeigt. Sie können einen Modelltext nur zu Positionen mit einer Modellscheibe erfassen. | 1002 |
| **Logotext** | Zusätzliche Information zum Logo. Sie können einen Logotext nur zu Positionen mit einer Bearbeitung mit Logo erfassen. | 1010 |
| **Kistensignatur-Texte** | Kistensignatur für den Versand. ⇨ "Kistensignatur" auf Seite D-261 | ab 5000 |

## Floskeln

**Navigation:** `Verkauf > Auftragserfassung > Positionsbene > <F4> > Texte > Kopftext, Fußtext, Artikeltext, Positionstext > [Floskeln neu]`

[Image: Abb. D-109 Floskeln. A dialog for creating or editing standard texts (Floskeln) is shown, with a field for an identifier (Kennung), a text entry area, and checkboxes for form types.]

In diesem Dialog können Sie Floskeln anlegen oder bearbeiten. Floskeln sind Standardtexte, die in den Stammdaten hinterlegt werden.

Floskeln können in den Kopf-, Fuß-, Artikel-, Positionstexten und den speziellen Texten als fertig vorformulierte Textbausteine herangezogen werden.

Im rechten Teil des Dialogs wählen Sie die Arten der Formulare aus, auf die die Floskeln gedruckt werden sollen.
**Technische Info:** alphanumerische Felder, DB-Feld: floskel.code, floskel.txt
⇨ "Formulare" auf Seite D-255

- **Kennung**: Kennzeichen und Bezeichnung der Floskel. Wenn Sie das Kennzeichen einer bestehenden Floskel angeben, wird die Bezeichnung im Klartext angezeigt.
  **Technische Info:** alphanumerische Felder, DB-Feld: floskel.code, floskel.txt

- **(Eingabezeile für Text)**: Standardtext, der der Floskel zugeordnet ist.
  **Technische Info:** alphanumerische Felder, DB-Felder: floskel.txt

> **i Bestehende Floskeln bearbeiten**
> Wenn Sie die Kennung einer bestehenden Floskel eintragen, können Sie diese Floskel bearbeiten und anschließend übernehmen.

Wenn Sie im Fußbereich der Text-Dialoge auf [Floskeln] klicken, wird ein Suchdialog angezeigt, in dem Sie nach angelegten Floskeln suchen können.

[Image: Abb. D-110 Auswahl der Floskeln. A search dialog to find existing "Floskeln" by their identifier (Kennung).]

- **Kennung**: Kennzeichen der Floskel. Mit [Suchen] werden alle bestehenden Floskeln in einem separaten Dialog angezeigt. Wenn Sie eine Floskel auswählen, wird der Floskeltext in den Eingabezeilen des aktuellen Text-Dialogs angezeigt.
  **Technische Info:** alphanumerisches Feld, DB-Feld: floskel.code

## Fremdinformationen

**Navigation:** `Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > <F4> > Texte > Fremdinformationen`

[Image: Abb. D-111 Fremdinformationen. A dialog box to enter external information, including an external number, purchasing info, and shipping info.]

In diesem Dialog hinterlegen Sie Fremdinformationen. Fremdinformationen sind Informationen zur weiteren Vorgangsbearbeitung, die firmenintern an verschiedene Abteilungen übermittelt werden sollen.

- **Fremdnummer**: Kundenseitige Vorgangsbezeichnung unter der der Kunde diesen Auftrag führt. Die Eingabe wird in das Feld Knd-Bestnr übernommen. Mit der Knd-Bestnr können Sie nach Aufträgen suchen.
  **Technische Info:** alphanumerisches Feld, DB-Feld: kauf.exaufnr

> **i Vorgang über die Fremdnummer öffnen**
> Wenn Sie einen Vorgang über die Fremdnummer öffnen wollen, können Sie in der Auftragserfassung im Feld Vorgangsnummer mit `<F5>` in das Feld Knd-Bestnr wechseln. Wenn Sie die Fremdnummer eingeben und mit `<Enter>` bestätigen, werden alle Vorgänge mit dieser Fremdnummer angezeigt. Wenn Sie einen Eintrag auswählen, wird der entsprechende Vorgang geöffnet.

- **Einkaufsinfo**: Informationstext, der an die Abteilung Einkauf übermittelt wird. Die Information kann im Bestellpool angezeigt werden. Mit `<Ende>` speichern Sie die Daten und schließen den Dialog.
  **Technische Info:** alphanumerisches Feld, DB-Feld: kauf.exbez1

- **Versandinfo**: Informationstext, der an die Versandsteuerung übermittelt wird. Die Versandinfo wird in der Versandsteuerung auf der Auftragsebene angezeigt. Mit `<Ende>` speichern Sie die Daten und schließen den Dialog.
  **Technische Info:** alphanumerisches Feld, DB-Feld: kauf.exbez2

## Kistensignatur

**Navigation:** `Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > <Shift> + <F4> > Kistensignatur`

[Image: Abb. D-112 Kistensignatur. A dialog showing texts to be printed on different sides of a crate (oben, vorne, unten, etc.).]

In diesem Dialog wird die Kistensignatur für den Versand angezeigt. Die Kistensignatur wird für die Versandsteuerung benötigt und wird automatisch generiert.

Die Funktionen sind von den Einstellungen in den Stammdaten und der jeweiligen Systemkonfiguration abhängig. Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

Im Dialog können jeder Kistenseite Texte zugeordnet werden. Die Texte werden über Textformeln aus den Stammdaten generiert.

Der Dialog Textformeln ist zum Part Stammdaten beschrieben:
⇨ Stammdaten, "Textformeln" auf Seite J-403

Die Zuordnung der Kistensignatur wird in den Stammdaten hinterlegt.

Der Dialog Bezeichnungen für Kistensignatur ist im Part Stammdaten beschrieben:
⇨ Stammdaten, "Bezeichnungen für Kistensignatur" auf Seite J-268

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

# Preise und Konditionen

## Preise und Konditionen

Für die Preisberechnung im Vorgang werden die Artikelpreise und Markpartner-Konditionen aus den Stammdaten herangezogen. Einzelne Preise und Konditionen können vorgangsbezogen bearbeitet werden.

Eine ausführliche Beschreibung finden Sie im Part Preise und Konditionen.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Auftragskonditionen" auf Seite D-264
- "Auftragspreise" auf Seite D-269
- "Auftragssprossenpreise" auf Seite D-271
- "Auftragsaustauschpreise" auf Seite D-274
- "Auftragsunterteilpreise" auf Seite D-276
- "Nachkalkulation" auf Seite D-277
- "Stufenpreise" auf Seite D-280
- "Positionskonditionen" auf Seite D-281
- "Produktionskostenkalkulation" auf Seite D-313
- "Preiskalkulation" auf Seite D-320

## Auftragskonditionen

**Navigation:**
- `Verkauf > Auftragserfassung > Positionsebene > <F4> > Preisangaben > Auftragskonditionen`
- `Verkauf > Auftragserfassung > Kopf-, Fußbereich > <F4> > Preisangaben > Vorgangskonditionen`

[Image: Abb. D-113 Auftragskonditionen. The image shows a detailed dialog for setting order-specific conditions for sales and purchasing, with fields for different glass types, components, and processing.]

In diesem Dialog hinterlegen Sie auftragsbezogene Preise und Konditionen. Sie können verschiedene Kriterien der Preisberechnung für die folgenden Komponenten festlegen:
- Glasarten
- Sprossen
- Farbartikel
- Zubehör
- Bearbeitungen
- Verglasungen

Die Werte geben Sie für Verkaufs- und Einkaufspreise getrennt an. Die Register Verkauf und Einkauf sind analog aufgebaut. Abweichungen werden im Folgenden explizit beschrieben.

### Kopfbereich

- **Auftrag**: Nummer des gewählten Auftrags.
  **Technische Info:** Anzeigefeld, DB-Feld: kauf.auftrnr
- **Kond-Debitor**: Kundennummer des Kunden, für den die Konditionen gelten. Wenn Sie ohne Konditionsdebitor arbeiten wollen, müssen Sie die Meldung, die beim Verlassen des Felds angezeigt wird mit [Ja] bestätigen. Das Feld wird nur angezeigt, wenn das Register Verkauf geöffnet ist.
  **Technische Info:** numerisches Feld, DB-Feld: aufkond.kalkkunr

### Verkauf und Einkauf

In diesem Register werden die Verkaufs- oder Einkaufspreise für die verschiedenen Preismethoden angezeigt.

**ISO, ESG, VSG, Basisglas, Veredelung, Farbartikel, Preise allg.** Die Werte gelten für die Artikel, denen die jeweilige Preismethode zugewiesen ist.
⇨ Preise und Konditionen, "Preismethoden" auf Seite K-45

**Sprossen** Die Werte gelten für Artikel, denen die Preismethode Sprossenpreise zugewiesen ist. Für Sprossen können keine Staffelstufen angegeben werden.

Sie können für jede Artikelgruppe verschiedene Berechnungskriterien angeben:

- **PKZ:** Preiskennzeichen, mit dem die Preise ermittelt werden. Das PKZ verweist auf eine Preisliste, in der die Preise für die Artikel mit den jeweiligen Preismethoden definiert sind.
  **Technische Info:** numerische Felder, DB-Felder: aufkond.isopkz, aufkond.pkzesgpkz, aufkond.pkzvsgpkz, aufkond.pkzbaspkz, aufkond.pkzverpkz, aufkond.pkzfarbpkz, aufkond.pkzallpkz, aufkond.sprospkz

- **TZ:** Teuerungszuschlag in Prozent. Der Teuerungszuschlag wird auf den Mengeneinheitspreis aufgeschlagen. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
  **Technische Info:** numerische Felder, DB-Felder: aufkond.isotz, aufkond.pkzesgtz, aufkond.pkzvsgtz, aufkond.pkzbastz, aufkond.pkzvertz, aufkond.pkzfarbtz, aufkond.pkzalltz, aufkond.vksprtz

- **Faktor:** Faktor des Preiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
  **Technische Info:** numerische Felder, DB-Felder: aufkond.isofaktor, aufkond.pkzesgfakt, aufkond.pkzvsgfakt, aufkond.pkzbasfakt, aufkond.pkzverfakt, aufkond.pkzfarbfakt, aufkond.pkzallfakt, aufkond.sprosfakt

- **Stufe:** Angabe der Preis-Staffelstufe, aus der der Preis für die jeweilige Glasart bzw. Preismethode ermittelt wird.
  **Technische Info:** numerische Felder, DB-Felder: aufkond.pkzesgstaff, aufkond.pkzvsgstaff, aufkond.pkzbasstaff, aufkond.pkzverstaff, aufkond.pkzfarbstaff, aufkond.pkzallstaff

- **Art:** Auswahl der Berechnungsart, nach der die Sprossenpreise berechnet werden. Die Berechnungsarten sind zum Register Positionskonditionen – Sprossenpreise beschrieben:
  ⇨ "Positionskonditionen - Sprossenpreise" auf Seite D-310
  **Technische Info:** numerisches Feld, DB-Feld: aufkond.sprosart

- **Sonderzuschlag:** Preiszuschlag für Sonderanfertigungen. Im zweiten Feld geben Sie den Preistyp an. Der Preistyp bestimmt, worauf sich der Preis bezieht:
  - **WE/Stück:** Der Preis gilt pro Stück.
  - **WE/qm:** Der Preis gilt pro Quadratmeter
  - **Prozent:** Der Preis wird als Prozentsatz auf den Grundpreis berechnet.
  Diese Felder werden nur im Register Verkauf angezeigt.
  **Technische Info:** numerische Feld, Toggle-Feld, DB-Felder: aufkond.isosonderzu, aufkond.isosonderzutyp

- **Gesamtzu.:** Prozentualer Zuschlag, der auf den Gesamtpreis aufgeschlagen wird. Dieses Feld wird nur im Register Verkauf angezeigt.
  **Technische Info:** numerische Felder, DB-Felder: aufkond.isozuschlag, aufkond.pkzesggeszu, aufkond.pkzvsggeszu, aufkond.pkzbastgeszu, aufkond.pkzvergeszu, aufkond.pkzfarbgeszu, aufkond.pkzallgeszu

### Teuerungszuschlag und Faktor

Zusätzlich können Sie Teuerungszuschläge und Faktoren für einzelne Komponenten angeben. Im ersten Feld geben Sie jeweils den Teuerungszuschlag und im zweiten Feld den Faktor an.

**Zubehör TZ Faktor** Prozentualer Teuerungszuschlag und Faktor für Zubehörartikel. Die Felder werden in den Registern Verkauf und Einkauf angezeigt.
**Technische Info:** numerische Felder, DB-Felder: aufkond.zubetz, aufkond.zubef, aufkond.ekzubetz, aufkond.ekzubef

### Bearbeitungen (Register Verkauf)

Im Register Verkauf können Sie für Teuerungszuschlag und Faktor unterschiedliche Werte für die jeweilige Eck-, Kanten- oder Flächenbearbeitung von ESG und Basisglas angeben.

**ESG TZ Faktor** Teuerungszuschlag und Faktor für Bearbeitungen in Einscheiben-Sicherheitsglas.

**Basisglas TZ Faktor** Teuerungszuschlag und Faktor für Bearbeitungen in Basis-Glas.

Sie können den Teuerungszuschlag und den Faktor für verschiedene Bearbeitungen angeben. Der Teuerungszuschlag wird in der Preisberechnung berücksichtigt.
- **Ecken:** Eckbearbeitungen, z. B. Eckabschnitt.
  **Technische Info:** numerische Felder, DB-Felder: aufkond.esgbecktz, esgbeckf, verbecktz, verbeckf
- **Kanten:** Kantenbearbeitungen, z. B. Polieren.
  **Technische Info:** numerische Felder, DB-Felder: aufkond.esgbkantz, es-gbkanf, verbkantz, verbkanf
- **Fläche:** Flächenbearbeitungen, z. B. Beschichtung.
  **Technische Info:** numerische Felder, DB-Felder: aufkond.esgbflatz, es-gbflaf, verbflatz, verbflaf

### Bearbeitungen (Register Einkauf)

Im Register Einkauf können Sie für Teuerungszuschlag und Faktor unterschiedliche Werte für die Bearbeitung von ESG und Basisglas angeben.

**ESG TZ Faktor** Teuerungszuschlag und Faktor für Bearbeitungen in Einscheiben-Sicherheitsglas.
**Technische Info:** numerische Felder, DB-Felder: aufkond.ekesgbtz, ekesgbfakt

**Basisglas TZ Faktor** Teuerungszuschlag und Faktor für Bearbeitungen in Basis-Glas.
**Technische Info:** numerische Felder, DB-Felder: aufkond.ekeverbtz, ekverbfakt

### Sonderkosten

- **Verglasungspreis**: Preis der Verglasungsarbeit in der Währungseinheit.
  **Technische Info:** numerisches Feld, DB-Feld: aufkond.verglaseins, aufkond.verglaseinsek
- **Versiegelungspreis**: Preis der Versiegelungsarbeit in der Währungseinheit.
  **Technische Info:** numerisches Feld, DB-Feld: aufkond.verglasversieg, aufkond.verglasversiegek
- **Min. Preis einsetzen**: Mindestpreis der Verglasungs- oder Versiegelungsarbeiten.
  **Technische Info:** numerisches Feld, DB-Feld: aufkond.verglasmineins, aufkond.verglasmineinsek
- **Stückpreisrundung**: Angabe, wie der Stückpreis gerundet werden soll.
  - Wenn 100 angegeben ist, wird der Preis auf den nächsten vollen Währungsbetrag gerundet.
  - Wenn 10 angegeben ist, wird der Preis auf den nächsten Zehntelbetrag gerundet.
  **Technische Info:** numerische Felder, DB-Felder: aufkond.stkprsrund, aufkond.ekstkprsrund
- **SZR-Zuschlag**: Angabe, ob für den Scheibenzwischenraum ein Preiszuschlag berechnet werden soll:
  - **J:** Der SZR-Zuschlag wird erhoben, wenn der SZR die im zugeordneten ISO-Artikel angegebenen Millimeter-Staffeln unterschreitet. ⇨ Preise und Konditionen, "SZR-Zuschläge" auf Seite K-213
  - **N:** Der SZR-Zuschlag wird nicht erhoben.
  Dieses Feld wird nur im Register Verkauf angezeigt.
  **Technische Info:** Toggle-Feld, DB-Feld: aufkond.szrflag
- **Stufenzuschlag**: Preiszuschlag für die Stufenbearbeitung. Im zweiten Feld geben Sie den Zuschlagstyp an. Der Zuschlagstyp gibt an, worauf sich der Zuschlag bezieht:
  - **WE/St ne:** Der Stufenzuschlag wird nach Berechnung des Faktors als fester Nettobetrag pro Stufe aufgeschlagen.
  - **WE/St br:** Der Stufenzuschlag wird vor Berechnung des Faktors als fester Bruttobetrag pro Stufe aufgeschlagen.
  - **Prozent:** Der Stufenzuschlag wird als prozentual auf den Glasmengeneinheitspreis und die Austauschpreise aufgeschlagen.
  - **%/Stück:** Der Stufenzuschlag wird pro Stufe prozentual auf den Glasmengeneinheitspreis und die Austauschpreise aufgeschlagen.
  **Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: aufkond.stufzuvk, aufkond.stufzutypvk, aufkond.stufzuek, aufkond.stufzutypek
- **Minber. ESG/VSG in ISO**: Mindestberechnung für ESG- oder VSG-Glas in ISO-Glasscheiben. In das erste Feld wird der Wert für das ESG-Glas, in das zweite Feld der Wert für das VSG-Glas eingetragen. Dieses Feld wird nur im Register Verkauf angezeigt.
  **Technische Info:** numerische Felder, DB-Felder: aufkond.minesginiso, aufkond.minvsginiso
- **Mindestberechnung**: Anzahl der Mengeneinheiten in Stück, Quadratmeter usw., für die der Preis berechnet wird. Wenn die Menge in der Auftragsposition kleiner ist als die Mindestmenge, wird der Preis für diese Mindestmenge berechnet. Dieses Feld wird nur im Register Verkauf angezeigt.
  **Technische Info:** numerisches Feld, DB-Feld: aufkond.minber
- **Maßrundung**: Angabe der Maßrundung in Millimeter für die Preisberechnung des Artikels. Für die Preisberechnung werden die Kantenlängen in der Auftragsposition auf den nächsthöheren Wert in Millimeter aufgerundet, der durch die angegebene Maßrundung teilbar ist. In der Produktion werden diese Angaben nicht berücksichtigt. Dieses Feld wird nur im Register Verkauf angezeigt.
  **Technische Info:** numerisches Feld, DB-Feld: aufkond.massrund

## Auftragspreise

**Navigation:** `Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > <F4> > Preisangaben > Auftragspreise > Artikelpreise`

[Image: Abb. D-114 Auftragspreise. A dialog box for managing order-specific prices for individual articles.]

In diesem Dialog hinterlegen oder ändern Sie die Artikelpreise auftragsbezogen. Wenn Sie z. B. Artikel durch einen Mengenrabatt günstiger einkaufen als zu den hinterlegten Preisen in den Stammdaten, müssen die Preise manuell für den Auftrag geändert werden, damit die korrekte Gewinnspanne berechnet werden kann.

- **Konditionsart:** Art der gewährten Sonderkondition:
  - **Kunde:** Der Preis für den ausgewählten Artikel wird nach den kundenspezifischen Konditionen berechnet.
  - **Materialkosten:** Auf den ausgewählten Artikel werden die angegebenen Materialkosten gerechnet.
  **Technische Info:** Pflichtfeld, Toggle-Feld, DB-Feld: aufpreise.kondkz

- **Artikel, Bezeichnung:** Artikelnummer und Bezeichnung des Artikels, für den die Sonderkondition gilt.
  **Technische Info:** Pflichtfeld, numerisches Feld, alphanumerisches Feld, DB-Felder: aufpreise.artnr, artikel.artbez1

- **Preis:** Preis des Artikels.
  **Technische Info:** numerisches Feld, DB-Feld: aufpreise.preis

- **Preistyp:** Angabe, worauf sich der Preis bezieht:
  - **WE/Stück:** Der Preis wird pro Stück berechnet.
  - **WE/GME:** Der Preis wird pro Grundmengeneinheit berechnet, z. B. pro Quadratmeter.
  **Technische Info:** Toggle-Feld, DB-Feld: aufpreise.preistyp

- **Faktor:** Faktor des Preiszuschlags in Prozent. In der Regel wird mit einem Faktor ein Rabatt gewährt.
  **Technische Info:** numerisches Feld, DB-Feld: aufpreise.faktor

Mit `<F2>` wechseln Sie in die Detailansicht.

Die meisten Felder in der Detailansicht entsprechen den Spalten in der Übersicht. Zusätzlich werden folgende Felder angezeigt:

- **Mindestberechnung**: Anzahl der Mengeneinheiten in Stück, Quadratmeter usw., für die der Preis berechnet wird. Wenn die Menge in der Auftragsposition kleiner ist als die Mindestmenge, wird der Preis für diese Mindestmenge berechnet.
  **Technische Info:** numerisches Feld, DB-Feld: aufpreise.minber

- **Maßrundung**: Angabe der Maßrundung in Millimeter für die Preisberechnung des Artikels. Für die Preisberechnung werden die Kantenlängen in der Auftragsposition auf den nächsthöheren Wert in Millimeter aufgerundet, der durch die angegebene Maßrundung teilbar ist. In der Produktion werden diese Angaben nicht berücksichtigt.
  **Technische Info:** numerisches Feld, DB-Feld: aufpreise.massrund

- **Min.Kantenlänge**: Angabe der Kantenlänge in Millimeter für die Preisberechnung. Diese Größe wird herangezogen, wenn die Höhe oder Breite des Glases in der Auftragsposition kleiner ist als diese Mindestkantenlänge.
  **Technische Info:** numerisches Feld, DB-Feld: aufpreise.minkant

Die Artikelpreise sind ausführlich zum Part Preise und Konditionen beschrieben:
⇨ Preise und Konditionen, "Artikelpreise" auf Seite K-365

## Auftragssprossenpreise

**Navigation:** `Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > <F4> > Preisangaben > Auftragspreise > Sprossenpreise`

[Image: Abb. D-115 Auftragssprossenpreise. A dialog to define order-specific prices for crosspieces (Sprossen), based on various calculation methods.]

In diesem Dialog hinterlegen oder ändern Sie die Sprossenpreise auftragsbezogen.

- **Artikel:** Artikelnummer.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: aufspropr.artnr

- **Berechnungsart:** Auswahl der Berechnungsart, nach der die Sprossenpreise berechnet werden:
  1.  **Felder:** Der Preis wird pro Feld berechnet.
  2.  **LM+K+R:** Der Preis wird pro laufendem Meter, pro Kreuz und pro Randanschluss berechnet.
  3.  **LM:** Der Preis wird pro laufendem Meter berechnet.
  4.  **LM+K:** Der Preis wird pro laufendem Meter und pro Kreuz berechnet.
  5.  **LM+R:** Der Preis wird pro laufendem Meter und pro Randanschluss berechnet.
  6.  **K:** Der Preis wird pro Kreuz berechnet.
  7.  **K+R:** Der Preis wird pro Kreuz und pro Randanschluss berechnet.
  8.  **R:** Der Preis wird pro Randanschluss berechnet.
  9.  **Spezial:** Diese Form der Berechnung ist kundenindividuell konfiguriert.
  10. **Prozent:** Der Preis wird prozentual aus dem Grundpreis des Kopfartikels berechnet. Der Prozentsatz wird in der Detailansicht im Feld Prozent angegeben.
  11. **qm-Preis:** Der Preis wird pro Quadratmeter des Glases berechnet. Der Preis wird in der Detailansicht im Feld Qm-Preis angegeben.
  12. **Feld+LM:** Der Preis wird pro Feld und pro laufendem Meter berechnet.
  13. **Stück:** Für den Sprossenaufbau wird ein Gesamtpreis berechnet. Der Preis wird in der Detailansicht im Feld Stückpreis angegeben.
  14. **K oder LM:** Der Preis wird pro Kreuz oder pro laufendem Meter berechnet.
      - Wenn sich im Sprossenaufbau Kreuzungspunkte ergeben, werden die Sprossen nach Anzahl der Kreuze berechnet.
      - Wenn keine Kreuzungspunkte vorhanden sind, werden die Sprossen nach laufenden Metern berechnet.
  15. **Feld+K+R:** Der Preis wird pro Feld, pro Kreuz und pro Randanschluss berechnet.
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

- **Felder2**: Angabe des Preises pro Feld, wenn im Sprossenaufbau keine Kreuzungspunkte vorhanden sind. Der Preis wird bei der Berechnungsart Spezial ausgewertet.
  **Technische Info:** numerisches Feld, DB-Feld: aufspropr.pfe2
- **Prozent**: Angabe des Prozentsatzes. Der Preis wird bei den Berechnungsarten Prozent und Spezial ausgewertet.
  **Technische Info:** numerisches Feld, DB-Feld: aufspropr.prozent
- **Quadratmeter**: Angabe des Quadratmeterpreises. Der Preis wird bei der Berechnungsart qm-Preis ausgewertet.
  **Technische Info:** numerisches Feld, DB-Feld: aufspropr.qmpreis
- **Stückpreis**: Angabe des Stückpreises. Der Preis wird bei der Berechnungsart Stück ausgewertet.
  **Technische Info:** numerisches Feld, DB-Feld: aufspropr.stckpreis
- **Mindestlaufmeter**: Angabe der Sprossenlänge in Meter, für die der Preis mindestens berechnet wird. Der Preis wird bei der Berechnungsart LM ausgewertet.
  **Technische Info:** numerisches Feld, DB-Feld: aufspropr.minlm
- **Mindestfeldanzahl**: Angabe der Sprossenfelder, für die der Preis mindestens berechnet wird. Der Preis wird bei der Berechnungsart Felder ausgewertet.
  **Technische Info:** numerisches Feld, DB-Feld: aufspropr.minfeld
- **Faktor**: Faktor des Preiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
  **Technische Info:** numerisches Feld, DB-Feld: aufspropr.faktor

Eine ausführliche Beschreibung der Sprossenpreise finden Sie im Part Preise und Konditionen:
⇨ Preise und Konditionen, "Sprossenpreise" auf Seite K-383

## Auftragsaustauschpreise

**Navigation:** `Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > <F4> > Preisangaben > Auftragspreise > Austauschpreise`

[Image: Abb. D-116 Auftragsaustauschpreise. A dialog for defining prices for articles that are exchanged or added within a bill of materials.]

In diesem Dialog hinterlegen oder bearbeiten Sie auftragsbezogen die Preise für Artikel, die innerhalb der Stückliste ausgetauscht oder hinzugefügt wurden.

- **Typ:** Produkttyp des Artikels dessen Preis ausgetauscht wird.
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

- **Faktor**: Faktor des Preiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
  **Technische Info:** numerisches Feld, DB-Feld: aufaustpr.faktor

- **Mindestberechnung**: Angabe der Mindestfläche in Quadratmeter, für die der Preis berechnet wird. Wenn die Fläche des Austauschglases in der Auftragsposition kleiner ist als die Mindestberechnungsfläche, wird der Preis für diese Mindestberechnungsfläche berechnet.
  **Technische Info:** numerisches Feld, DB-Feld: aufaustpr.minber

- **Maßrundung**: Angabe der Maßrundung in Millimeter für die Preisberechnung des Artikels. Für die Preisberechnung werden die Kantenlängen in der Auftragsposition auf den nächsthöheren Wert in Millimeter aufgerundet, der durch die angegebene Maßrundung teilbar ist. In der Produktion werden diese Angaben nicht berücksichtigt.
  **Technische Info:** numerisches Feld, DB-Feld: aufaustpr.massrund

Eine ausführliche Beschreibung der Austausch- und Zusatzpreise finden Sie im Part Preise und Konditionen:
⇨ Preise und Konditionen, “ISO-Austauschpreise" auf Seite K-393
⇨ Preise und Konditionen, "Spezielle VSG-Austausch-/Zusatzpreise" auf Seite K-422

## Auftragsunterteilpreise

**Navigation:** `Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > <F4> > Preisangaben > Auftragspreise > Unterteilpreise`

[Image: Abb. D-117 Auftragsunterteilpreise. A dialog for defining order-specific prices for sub-components (Unterteile).]

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

- **Faktor**: Faktor des Preiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
  **Technische Info:** numerisches Feld, DB-Feld: aufuteilpr.faktor
- **Mindestberechnung**: Anzahl der Mengeneinheiten in Stück, Quadratmeter usw., für die der Preis berechnet wird. Wenn die Menge der Unterteile in der Auftragsposition kleiner ist als die Mindestmenge, wird der Preis für diese Mindestmenge berechnet.
  **Technische Info:** numerisches Feld, DB-Feld: aufuteilpr.minber
- **Maßrundung**: Angabe der Maßrundung in Millimeter für die Preisberechnung des Artikels. Für die Preisberechnung werden die Kantenlängen in der Auftragsposition auf den nächsthöheren Wert in Millimeter aufgerundet, der durch die angegebene Maßrundung teilbar ist. In der Produktion werden diese Angaben nicht berücksichtigt.
  **Technische Info:** numerisches Feld, DB-Feld: aufuteilpr.massrund

## Nachkalkulation

**Navigation:** `Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > <F4> > Preisangaben > Teilkalkulation`

[Image: Abb. D-118 Nachkalkulation. A dialog for post-calculation, showing sales and purchase prices and factors for various components and processes.]

In diesem Dialog hinterlegen Sie auftragsbezogen Konditionen für die Verkaufs- und Einkaufspreise.
Mit `<F3>` können Sie die Preise mit den neuen Konditionen berechnen lassen. Die Werte der Nachkalkulation werden in die Positionskonditionen übernommen.

Wenn Sie die Werte bearbeiten, werden diese in die entsprechenden Preiskonditionen übernommen. Die technische Information und der Datenbankbezug der Felder entspricht den jeweiligen Preiskonditionen.
⇨ "Positionskonditionen" auf Seite D-281

### Kopfbereich

- **Stückliste**: Nummer der Stückliste, für die die Konditionen festgelegt werden sollen.
  **Technische Info:** numerisches Feld, DB-Feld: kpos.poskonr
- **Konditionen holen**: Angabe, ob die Konditionen zur Preisermittlung aus den Stammdaten gezogen werden sollen.
  - **J:** Die Konditionen aus den Stammdaten werden zur Preisermittlung herangezogen. Die angegebenen Werte im Rumpfbereich werden von den Werten aus den Stammdaten überschrieben, falls der entsprechende Wert in den Stammdaten hinterlegt wurde.
  - **N:** Die Konditionen aus den Stammdaten werden nicht herangezogen. Sie können die Konditionen auftragsbezogen im Rumpfbereich angeben.
  **Technische Info:** Toggle-Feld

### Verkauf und Einkauf

Sie können für die folgenden Felder jeweils einen Wert für den Verkauf und einen Wert für den Einkauf angeben.

- **Grundpreis**: Grundpreis des Artikels. Im zweiten Feld geben Sie den Preistyp an. Der Preistyp bestimmt, worauf sich der Preis bezieht:
  - **WE/Stück:** Der Preis gilt pro Stück.
  - **WE/GME:** Der Preis gilt pro Grundmengeneinheit, z. B. pro Quadratmeter.
  **Technische Info:** numerisches Feld
- **Faktor**: Faktor des Preiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
  **Technische Info:** numerisches Feld
- **TZ**: Teuerungszuschlag in Prozent. Der Teuerungszuschlag wird auf den Mengeneinheitspreis aufgeschlagen. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
  **Technische Info:** numerisches Feld
- **Bearbeitungs-Faktor**: Faktor für Bearbeitungen in Prozent.
  **Technische Info:** numerisches Feld
- **Bearbeitungs-TZ**: Teuerungszuschlag für Bearbeitungen in Prozent.
  **Technische Info:** numerisches Feld
- **Zubehör-Faktor**: Faktor für Zubehörartikel in Prozent.
  **Technische Info:** numerisches Feld
- **Zubehör TZ**: Teuerungszuschlag für Zubehörartikel in Prozent.
  **Technische Info:** numerisches Feld
- **Sprossen-TZ**: Teuerungszuschlag für Sprossenartikel in Prozent.
  **Technische Info:** numerisches Feld
- **Sprossenberechnungsart**: Auswahl der Berechnungsart, nach der die Sprossenpreise berechnet werden. Die Berechnungsarten sind zum Register Positionskonditionen – Sprossenpreise beschrieben.
  ⇨ "Positionskonditionen - Sprossenpreise" auf Seite D-310
  **Technische Info:** numerisches Feld
- **Verglasungspreis**: Preis der Verglasung pro Quadratmeter.
  **Technische Info:** numerisches Feld
- **Mindestpreis Verglasung**: Preis, der mindestens für die Verglasung berechnet wird. Wenn im Auftrag bei einem Artikel der Preis der Verglasung kleiner ist als der angegebene Mindestpreis, wird dieser Mindestpreis berechnet.
  **Technische Info:** numerisches Feld
- **Versiegelungspreis**: Preis der Versiegelung pro Quadratmeter.
  **Technische Info:** numerisches Feld
- **Mindestpreis Versiegelung**: Preis, der mindestens für die Versiegelung berechnet wird. Wenn im Auftrag bei einem Artikel der Preis der Versiegelung kleiner ist als der angegebene Mindestpreis, wird dieser Mindestpreis berechnet.
  **Technische Info:** numerisches Feld

### Austausch

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

## Stufenpreise

**Navigation:** `Verkauf > Auftragserfassung > Register Positionen > gestuften Artikel erfassen > Preisfeld > <Shift> + <F9> > <F8>`

[Image: Abb. D-119 Stufenpreise. A dialog for defining tiered prices for stepped articles.]

In diesem Dialog geben Sie gestaffelte Preise für einen Stufenartikel an, z. B. für ISO-Artikel.
- **VK/EK:** Die Eingaben gelten für Einkauf oder Verkauf.
- **Ab Stufenbreite (mm):** Wert der Stufenbreite in Millimeter, z. B. ab einer Stufenbreite von 100 mm 3,50 € und ab einer Stufenbreite von 200 mm 7,80 €.
- **Anzahl:** Anzahl der Stufen zur Berechnung.
- **Zuschlag:** Wert des Stufenzuschlags in Währungseinheiten, z. B. in Euro.
- **Zuschlagstyp:** Berechnungsart des gestaffelten Preiszuschlags für Stufen.
  - **WE/Stück:** Preis (Währungseinheit) zur Staffelung der Stufenbreite wird mit der Stückzahl der Stufen und dem Wert im Feld Zuschlag multipliziert. Dieser Wert wird zum Glaspreis addiert.
  - **WE/Stück/qm netto:** Staffelung der Stufenbreite wird mit der Stückzahl der Stufen und dem Wert im Feld Zuschlag multipliziert. Das Ergebnis wird mit der Fläche des umschriebenen Rechtecks des Artikels multipliziert und zum Stückpreis addiert.

## Positionskonditionen

**Navigation:** `Verkauf > Auftragserfassung > Register Positionen > Preisfeld > <Shift> + <F9>`

In diesen Dialogen werden die Preiskonditionen eines Positionsartikels angezeigt.

Die Dialoge sind in zwei Register oder Bereiche aufgeteilt, die die Preiskonditionen für Verkauf und Einkauf anzeigen. Das Register Einkauf ist nur aktiv, wenn die Beschaffungsart Bestellung oder Mitgelief. für die Position gewählt ist. Der Aufbau der Register und Bereiche unterscheidet sich, je nachdem welche Preismethode dem Positionsartikel zugeordnet ist. Es werden die Werte angezeigt, die für die Preisberechnung relevant sind.

Die einzelnen Preismethoden sind zu dem Part Preise und Konditionen beschrieben:
⇨ Preise und Konditionen, "Preismethoden" auf Seite K-45

Sie können die Werte für die Preiskonditionen bearbeiten. Wenn Sie den Preis neu berechnen lassen möchten, schließen Sie den Dialog. Eine Abfrage wird angezeigt, ob Sie den Preis neu berechnen lassen möchten. Wenn Sie die Abfrage bestätigen, werden die Preise mit den vorgangsbezogenen Positionskonditionen berechnet.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG" auf Seite D-282
- "Konditionen für PKZ-VSG, PKZ-ESG" auf Seite D-286
- "Konditionen ISO" auf Seite D-288
- "Konditionen für ISO (SCHWEIZ)" auf Seite D-293
- "Konditionen für PKZ-FARBARTIKEL" auf Seite D-297
- "Konditionen für PKZ-PREISE-ALLGEMEIN" auf Seite D-298
- "Konditionen für PKZ-GLASTÜREN" auf Seite D-300
- "Konditionen für Manuelle Preise" auf Seite D-303
- "VSG-Austausch-/Zusatzpreise" auf Seite D-304

Je nachdem, welche preisrelevanten Bearbeitungen in der Stückliste der Position enthalten sind, werden die Register Bearbeitungspreise (VK), (EK) und Sprossenpreise aktiv. Die Preiseigenschaften für Bearbeitungspreise werden in den Stammdaten festgelegt.
⇨ Stammdaten, "Preiseigenschaften" auf Seite J-342

Die Register Bearbeitungspreise (VK), (EK) und Sprossenpreise werden separat beschrieben.

In diesem Abschnitt sind zusätzlich folgende Register erklärt:
- "Positionskonditionen – Bearbeitungspreise (VK), (EK), Detailansicht" auf Seite D-307
- "Positionskonditionen – Sprossenpreise" auf Seite D-310

## Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG

**Navigation:** `Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Preismethode PKZ-Basisglas, PKZ-Veredelung > <Shift> + <F9>`

[Image: Abb. D-120 Konditionen PKZ-BASISGLAS, PKZ-VEREDELUNG. A detailed dialog showing price conditions for articles with the pricing method PKZ-Basisglas or PKZ-Veredelung.]

In diesem Dialog werden die Preiskonditionen eines Positionsartikels angezeigt, dem die Preismethode PKZ-Basisglas oder PKZ-Veredelung zugeordnet ist. Sie können die Preiskonditionen bearbeiten.

In den Dialogen Konditionen PKZ-BASISGLAS und Konditionen PKZ-VEREDELUNG sind die Register Verkauf und Einkauf weitgehend analog aufgebaut. Das Feld Gesamtzuschlag wird im Register Einkauf nicht angezeigt.

Wenn Zusatz-Bearbeitungen in der Stückliste der Position enthalten sind, dann sind die Register Bearbeitungspreise (VK), (EK) aktiv:
⇨ "Positionskonditionen - Bearbeitungspreise (VK), (EK), Detailansicht" auf Seite D-307

Wenn Sprossen in der Stückliste der Position enthalten sind, dann ist das Register Sprossenpreise aktiv:
⇨ "Positionskonditionen - Sprossenpreise" auf Seite D-310

### Kopfbereich

- **VK-PKZ**: Preiskennzeichen der vordefinierten Preisliste für den Verkauf.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.pkz
- **EK-PKZ**: Preiskennzeichen der vordefinierten Preisliste für den Einkauf.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.ekpkz
- **Vektor**: Nummer des Vektors, aus dem der Preis gezogen werden soll.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.matnr

### Register Verkauf, Einkauf

- **Preisart**: Art der Preisberechnung. Standardmäßig ist die Preisart Einzelpreis ausgewählt. Das Feld ist ein Anzeigefeld. Wenn Sie den Glas- oder Grundpreis ändern oder den Preis in der Position manuell eingeben, ohne eine Preisberechnung durchzuführen, dann wird als Preisart manueller Preis angezeigt.
  **Technische Info:** Anzeigefeld, DB-Feld: pokokon.flag6
- **Staffelstufe**: Preisstufe, aus der der Preis verwendet wird. Das Feld wird von der Preisberechnung nur ausgewertet, wenn für den relevanten Artikelpreisvektor die Preisart 2 – Staffelstufe angegeben ist.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.flag1, pokokon.ekflag1
- **Preistyp**: Anzeige, worauf sich der angegebene Preis bezieht.
  - **WE/Stück:** Der Preis gilt pro Stück.
  - **WE/GME:** Der Preis gilt pro Grundmengeneinheit, z. B. pro Quadratmeter.
  **Technische Info:** Toggle-Feld, Anzeigefeld
- **Glaspreis**: Grundpreis einer Glasscheibe. Der Preistyp wird aus dem vorherigen Feld herangezogen.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu1, pokokon.zuk1
- **Modellzuschlag**: Preiszuschlag, der bei Modellen erhoben wird. Sie können den Wert in Prozent oder als Betrag mit Währungseinheit angeben. Als Zuschlag wird immer der höhere Wert herangezogen.
  **Technische Info:** numerische Felder, DB-Felder: pokokon.zu2, pokokon.zuk2
- **TZ**: Prozentualer Teuerungszuschlag, der auf den Mengeneinheitspreis aufgeschlagen wird. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu3, pokokon.zuk3
- **Faktor**: Faktor des Preiszuschlags in Prozent.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu4, pokokon.zuk4
- **Gesamtzuschlag**: Preiszuschlag für die Position in Prozent.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu26, pokokon.zuk26
- **Maßrundung**: Maßrundung in Millimeter.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu5, pokokon.zuk5
- **Mindestberechnung**: Mindestfläche in Quadratmeter.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu6, pokokon.zuk6
- **Gebindegröße**: Fassungsvermögen des Gebindes in Mengeneinheiten.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu8, pokokon.zuk8
- **Stückpreisrundung**: Ab- oder Aufrundung für den Stückpreis einer Position.
  **Technische Info:** numerisches Feld, DB-Feld: pokokonp.vkstkprsrund, pokokonp.ekstkprsrund
- **Zuschlagsart**: Die Zuschlagsart gibt an, wonach der Zuschlag gestaffelt und wie der Zuschlag ermittelt wird:
  - **Fläche:** Der Zuschlag gilt jeweils ab den angegebenen Flächen.
  - **Längere Kante:** Der Zuschlag gilt jeweils für die längere Kante.
  - **Seitenverhältnis:** Der Zuschlag gilt ab dem angegebenen Seitenverhältnis.
  - **Übermaßzuschlag:** Der Zuschlag gilt ab der angegebenen Größe, z. B. Kantenlänge.
  **Technische Info:** Toggle-Feld, Anzeigefeld
- **Zuschlag**: Zuschlag, der auf den Preis erhoben wird. Es ist von der Konfiguration abhängig, ob der Zuschlag auf den Glasgrund-, den Grundmengen- oder den Stückpreis erhoben wird.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu24, pokokon.zuk24
- **Abschlag pro Stück**: Angabe des Abschlags.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu25, pokokon.zuk25
- **Mindestpreis**: Mindestpreis für die Glasscheibe.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu20, pokokon.zuk20

### Größenzuschläge

In diesem Bereich werden die Werte für Preiszuschläge und den Zuschlagstyp angezeigt. Sie können die Werte bearbeiten. Der Zuschlagstyp gibt an, worauf sich der Zuschlag bezieht:
- **WE Wert:** Der Zu- oder Abschlag wird als fester Betrag auf den Artikelpreis berechnet. Wenn der Zuschlag im Auftrag als fester Betrag erhoben wird, gilt die Währung des für den Kopfartikel ermittelten PLKZ. Die Währung wird nicht umgerechnet.
- **Prozent:** Der Zuschlag wird prozentual aus dem Grundpreis des Kopfartikels berechnet. Dieser Zuschlagstyp wird nur bei Austauschartikeln oder Bearbeitungen gewählt.

- **Kleinglaszuschlag**: Preiszuschlag für Kleingläser, wenn die Fläche des Glases kleiner ist als der angegebene Grenzwert. Im zweiten Feld wählen Sie den Zuschlagstyp.
  **Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu10, pokokon.zuk10
- **Überlängenzuschlag**: Preiszuschlag für Überlängen, wenn eine Kantenlänge länger ist, als der angegebene Grenzwert. Im zweiten Feld wählen Sie den Zuschlagstyp.
  **Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu11, pokokon.zuk11
- **Übergrößenzuschlag**: Preiszuschlag für Übergrößen, wenn beide Glaskanten eine festgelegte Länge überschreiten. Im zweiten Feld wählen Sie den Zuschlagstyp.
  **Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu12, pokokon.zuk12

### Verglasung

In diesem Bereich werden die Werte für Verglasung und Versiegelung angezeigt. Sie können die Werte bearbeiten.

- **Min.Preis einsetzen**: Mindestpreis, der für Verglasung und/oder Versiegelung gilt.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu21, pokokon.zuk21
- **Verglasungspreis**: Preis der Verglasung.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu22, pokokon.zuk22
- **Versiegelungspreis**: Preis der Versiegelung.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu23, pokokon.zuk23

### Fußzeile

In diesem Bereich werden die Bezeichnung des Artikels und das Kennzeichen der Warengruppe des Artikels angezeigt.

## Konditionen für PKZ-VSG, PKZ-ESG

**Navigation:** `Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Preismethode PKZ-VSG oder PKZ-ESG > <Shift> + <F9>`

[Image: Abb. D-121 Konditionen für PKZ-ESG, PKZ-VSG. A dialog showing price conditions for articles with the pricing method PKZ-ESG or PKZ-VSG.]

In diesem Dialog werden die Preiskonditionen eines Positionsartikels angezeigt, dem die Preismethode PKZ-ESG oder PKZ-VSG zugeordnet ist. Sie können die Preiskonditionen bearbeiten.

In den Dialogen Konditionen PKZ-ESG und Konditionen PKZ-VSG sind die Register Verkauf und Einkauf weitgehend analog aufgebaut. Das Feld Gesamtzuschlag wird im Register Einkauf nicht angezeigt.

Wenn Zusatz-Bearbeitungen in der Stückliste der Position enthalten sind, dann sind die Register Bearbeitungspreise (VK), (EK) aktiv:
⇨ "Positionskonditionen - Bearbeitungspreise (VK), (EK), Detailansicht" auf Seite D-307

Wenn Sprossen in der Stückliste der Position enthalten sind, dann ist das Register Sprossenpreise aktiv:
⇨ "Positionskonditionen - Sprossenpreise" auf Seite D-310

Wenn Sie einen VSG-Artikel erfasst haben, werden Ihnen mit `<Shift> + <F10>` die Konditionen der Austausch- und Zusatzpreise für die einzelnen Glasscheiben in dem VSG-Artikel in einem eigenen Dialog angezeigt:
⇨ "Produktionskostenkalkulation" auf Seite D-313

### Kopfbereich

Die Felder sind zum Dialog Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG beschrieben:
⇨ "Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG" auf Seite D-282

### Register Verkauf, Einkauf

Die meisten Felder sind zum Dialog Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG beschrieben:
⇨ "Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG" auf Seite D-282

### Größenzuschläge

Die meisten Felder sind zum Dialog Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG beschrieben:
⇨ "Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG" auf Seite D-282

Zusätzlich werden folgende Felder im Register Verkauf angezeigt:

- **Seitenverhältnis**: Preiszuschlag für bestimmte Seitenverhältnisse. Im zweiten Feld wählen Sie den Zuschlagstyp. Das Feld im wird nur im Dialog Konditionen PKZ-ESG angezeigt.
  **Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu28, pokokon.zuk28

### Verglasung

Die Felder sind zum Dialog Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG beschrieben:
⇨ "Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG" auf Seite D-282

### Fußzeile

In diesem Bereich werden die Bezeichnung des Artikels und das Kennzeichen der Warengruppe des Artikels angezeigt.

## Konditionen ISO

**Navigation:** `Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Preismethode ISO > <Shift> + <F9>`

[Image: Abb. D-122 Konditionen ISO. A detailed dialog showing price conditions for articles with the ISO pricing method, including settings for surcharges, exchange articles, and glazing.]

In diesem Dialog werden die Preiskonditionen eines Positionsartikels angezeigt, dem die Preismethode ISO zugeordnet ist. Sie können die Preiskonditionen bearbeiten.

Im Dialog Konditionen ISO sind die Register Verkauf und Einkauf analog aufgebaut.

Wenn Zusatz-Bearbeitungen in der Stückliste der Position enthalten sind, dann sind die Register Bearbeitungspreise (VK), (EK) aktiv:
⇨ "Positionskonditionen – Bearbeitungspreise (VK), (EK), Detailansicht" auf Seite D-307

Wenn Sprossen in der Stückliste der Position enthalten sind, dann ist das Register Sprossenpreise aktiv:
⇨ "Positionskonditionen - Sprossenpreise" auf Seite D-310

### Kopfbereich

- **PKZ**: Preiskennzeichen der vordefinierten Preisliste.
  **Technische Info:** numerisches Feld, DB-Feld:pokokon.pkz, pokokon.ekpkz
- **PLKZ**: Das Preislisten-Kennzeichen ist die eindeutige Nummerierung für regionale, nationale und ausländische Preislisten.
  **Technische Info:** numerisches Feld

### Register Verkauf, Einkauf

- **Preisart**: Art der Preisberechnung.
  - **Matrix:** Der Preis wird aus der zugeordneten Preismatrix berechnet. In der Preismatrix sind die Preise nach Höhe und Breite des Glases gestaffelt.
  - **Vektor:** Der Preis wird aus dem zugeordnetem Vektor berechnet. In einem Vektor können die Preise nach der Größe gestaffelt werden.
  - **Einzelscheiben:** Der Preis wird aus den Einzelpreisen der Gläser berechnet, aus denen sich die Scheibe zusammensetzt.
  - **Prs/qm:** Der Preis wird pro Quadratmeter berechnet. Diese Preisart wird automatisch gewählt, wenn Sie in den Konditionen den Grundpreis oder einen Austauschpreis bearbeiten.
  **Technische Info:** Toggle-Feld

- **Matrix / Vektor**: Nummer der Matrix oder des Vektors. Die Matrix ist eine zweidimensionale Preistabelle mit zwei Bezugsgrößen für die Staffelung, z. B. Breite und Höhe. Der Vektor ist eine eindimensionale Preistabelle mit einer Bezugsgröße für die Staffelung, z. B. Fläche. Wenn Sie eine Matrix oder einen Vektor gewählt haben, wird der Name der Matrix oder des Vektors im Klartext angezeigt.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.matnr, pokokon.ekmatnr

- **Grundpreis**: Grundpreis einer Glasscheibe. Der Grundpreis ist abhängig vom gewählten Preistyp. Im zweiten Feld wählen Sie den Preistyp aus. Der Preistyp gibt an, worauf sich der Preis bezieht:
  - **WE/Stück:** Der Preis gilt pro Stück.
  - **WE/GME:** Der Preis gilt pro Grundmengeneinheit, z. B. pro Quadratmeter.
  **Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu1, pokokon.zuk1

- **Zuschlag**: Preiszuschlag, der auf den Grundpreis erhoben wird.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu20, pokokon.zuk20

- **1. Austausch, 2. Austausch, 3. Austausch**: Austausch-Unterteile der Position. In den Feldern können Sie folgende Werte angeben:
  - **Erstes Feld:** Nummer der Austauschliste.
    **Technische Info:** numerische Felder, alphanumerische Felder, DB-Felder: pokokon.atmat1, pokokon.atmat2, pokokon.atmat3
  - **Zweites Feld:** Austauschkennzeichen A (Austausch) oder Z (Zusatz).
    **Technische Info:** numerische Felder, alphanumerische Felder, DB-Felder: pokokon.atkz1, pokokon.atkz2, pokokon.atkz3
  - **Drittes Feld:** Preis des Austausch-Artikels.
    **Technische Info:** numerische Felder, alphanumerische Felder, DB-Felder: pokokon.atp1, pokokon.atp2, pokokon.atp3
  - **Viertes Feld:** Preiszuschlag des Austausch-Artikels in Prozent.
    **Technische Info:** numerische Felder, alphanumerische Felder, DB-Felder: pokokon.zu11, pokokon.zu12, pokokon.zu13, pokokon.zu14, pokokon.zu15, pokokon.zu16

- **Modellzuschlag**: Preiszuschlag, der bei Modellen erhoben wird. Sie können den Wert in Prozent oder als Betrag mit Währungseinheit angeben. Als Zuschlag wird immer der höhere Wert herangezogen.
  **Technische Info:** numerische Felder, DB-Felder: pokokon.zu2, pokokon.zuk2
- **Teuerungszuschlag**: Prozentualer Teuerungszuschlag, der auf den Mengeneinheitspreis aufgeschlagen wird. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu3, pokokon.zuk3
- **Faktor**: Faktor des Preiszuschlags in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu4, pokokon.zuk4
- **Maßrundung**: Angabe der Maßrundung in Millimeter für die Preisberechnung des Artikels. Für die Preisberechnung werden die Kantenlängen in der Auftragsposition auf den nächsthöheren Wert in Millimeter aufgerundet, der durch die angegebene Maßrundung teilbar ist. In der Produktion werden diese Angaben nicht berücksichtigt. Dieses Feld wird nur im Register Verkauf angezeigt.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu5, pokokon.zuk5
- **Mindestberechnung**: Angabe der Mindestfläche in Quadratmeter, für die der Preis berechnet wird. Wenn die Fläche in der Auftragsposition kleiner ist als die Mindestberechnungsfläche, wird der Preis für diese Fläche berechnet. Dieses Feld wird nur im Register Verkauf angezeigt.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu6, pokokon.zuk6
- **Mindestkantenlänge**: Angabe der Kantenlänge in Millimeter für die Preisberechnung. Diese Größe wird herangezogen, wenn die Höhe oder Breite des Glases in der Auftragsposition kleiner ist als diese Mindestkantenlänge. Das Feld wird nur im Dialog Konditionen ISO angezeigt.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu7, pokokon.zuk7
- **SZR-Zuschlag**: Preiszuschlag für den Scheibenzwischenraum. Im zweiten Feld geben Sie den Zuschlagstyp an. Der Zuschlagstyp gibt an, worauf sich der Zuschlag bezieht:
  - **WE/Stück:** Der Zuschlag wird als fester Betrag auf den Stückpreis der Position aufgeschlagen.
  - **WE/qm:** Der Zuschlag wird pro Quadratmeter der Scheibenfläche aufgeschlagen.
  - **Prozent:** Der Zuschlag wird pro Scheibenzwischenraum als Prozentwert auf den Glasgrundpreis aufgeschlagen.
  **Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu8, pokokon.zuk8
- **Stufenzuschlag**: Preiszuschlag für ein Glas mit einer Stufe. Im zweiten Feld geben Sie den Zuschlagstyp an. Der Zuschlagstyp gibt an, worauf sich der Zuschlag bezieht:
  - **WE/St netto:** Der Stufenzuschlag wird nach Berechnung des Faktors als fester Nettobetrag pro Stufe aufgeschlagen.
  - **WE/St brutto:** Der Stufenzuschlag wird vor Berechnung des Faktors als fester Bruttobetrag pro Stufe aufgeschlagen.
  - **Prozent:** Der Stufenzuschlag wird prozentual auf den Glasmengeneinheitspreis und die Austauschpreise aufgeschlagen.
  - **%/Stück:** Der Stufenzuschlag wird pro Stufe prozentual auf den Glasmengeneinheitspreis und die Austauschpreise aufgeschlagen.
  **Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu9, pokokon.zuk9
- **Kunstverglasung**: Preiszuschlag der Kunstverglasung in Prozent, wenn in der Stückliste ein Glas mit dem Artikeltyp Kunstverglasung eingehängt ist.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu28, pokokon.zuk28
- **Überlängenzuschläge**: Preiszuschlag für Überlängen in Prozent, wenn eine Kantenlänge länger ist, als der angegebene Grenzwert.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu19, pokokon.zuk19
- **Sonderzuschlag**: Preiszuschlag für Sonderanfertigungen. Im zweiten Feld geben Sie den Zuschlagstyp an. Der Zuschlagstyp gibt an, worauf sich der Zuschlag bezieht:
  - **WE/Stück:** Der Zuschlag wird als fester Betrag auf den Stückpreis der Position aufgeschlagen.
  - **WE/GMR:** Der Zuschlag wird pro Grundmengeneinheit, z. B. pro Quadratmeter, aufgeschlagen.
  - **Prozent:** Der Zuschlag wird als Prozentwert auf den Glasgrundpreis aufgeschlagen.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu25, pokokon.zuk25
- **Gesamtzuschlag**: Preiszuschlag für die Position in Prozent.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu26, pokokon.zuk26
- **Mindestpreis**: Mindestpreis für die Position.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu18, pokokon.zuk18
- **Stückpreisrundung**: Ab- oder Aufrundung für den Stückpreis einer Position.
  **Technische Info:** numerisches Feld, DB-Feld: pokokonp.vkstkprsrund, pokokonp.ekstkprsrund

### Größenzuschläge

Die meisten Felder sind zum Dialog Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG beschrieben:
⇨ "Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG" auf Seite D-282

Zusätzlich werden folgende Felder angezeigt:

- **Seitenverhältnis**: Preiszuschlag für bestimmte Seitenverhältnisse. Im zweiten Feld wählen Sie den Zuschlagstyp.
  **Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu28,
- **Flächenzuschlag**: Preiszuschlag für bestimmte Flächen. Im zweiten Feld wählen Sie den Zuschlagstyp. Das Feld wird nur im Dialog Konditionen ISO angezeigt.
  **Technische Info:** numerisches Feld, Toggle-Feld, DB-Felder: pokokon.zu9

### Verglasung

- **Verglasungspreis**: Preis der Verglasung.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu21, pokokon.zuk21
- **Versiegelungspreis**: Preis der Versiegelung.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu22, pokokon.zuk22
- **Mindestpreis Verglasung**: Mindestpreis der Verglasung.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu23, pokokon.zuk23
- **Mindestpreis Versiegelung**: Mindestpreis der Versiegelung.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu24, pokokon.zuk24

### Fußzeile

In diesem Bereich werden die Bezeichnung des Artikels und das Kennzeichen der Warengruppe des Artikels angezeigt.

## Konditionen für ISO (SCHWEIZ)

**Navigation:** `Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Preismethode ISO-Schweiz > <Shift> + <F9>`

[Image: Abb. D-123 Konditionen ISO (SCHWEIZ). A dialog showing specific price conditions for the Swiss market (ISO-Schweiz pricing method).]

In diesem Dialog werden die Preiskonditionen eines Positionsartikels angezeigt, dem die Preismethode ISO-Schweiz zugeordnet ist. Sie können die Preiskonditionen bearbeiten.

Im Dialog Konditionen ISO-Schweiz gibt es das Register Verkauf, aber kein Register Einkauf.

Wenn Zusatz-Bearbeitungen in der Stückliste der Position enthalten sind, dann sind die Register Bearbeitungspreise (VK), (EK) aktiv:
⇨ "Positionskonditionen - Bearbeitungspreise (VK), (EK), Detailansicht" auf Seite D-307

Wenn Sprossen in der Stückliste der Position enthalten sind, dann ist das Register Sprossenpreise aktiv:
⇨ "Positionskonditionen - Sprossenpreise" auf Seite D-310

### Register Verkauf

- **VK-PKZ**: Preiskennzeichen der vordefinierten Preisliste für den Verkauf.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.pkz
- **Vektor**: Nummer des Vektors, aus dem der Preis gezogen werden soll.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.matnr
- **Glasgrundpreis**: Anzeige des Mindestpreises für den Glasgrundpreis. Der Glasgrundpreis ist durch den Vektor festgelegt und kann vorgangsbezogen bearbeitet werden:
  - **Glasgrundpreis:** Glasgrundpreis in der Währungseinheit.
    **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu1
  - **(Preistyp):** Angabe, worauf sich der Glasgrundpreis bezieht:
    - **WE/Stück:** Der Preis gilt pro Stück.
    - **WE/GME:** Der Preis gilt pro Grundmengeneinheit, z. B. pro Quadratmeter.
    **Technische Info:** Toggle-Feld, DB-Feld: pokokon.flag2
  - **Mindestpreise (in Zeile Glasgrundpreis):** Mindestpreis für den Glasgrundpreis. Dieser Preis wird festgelegt, wenn der berechnete Preis in der Auftragsposition niedriger ist als der angegebene Mindestpreis.
    **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu20
- **Mengenstaffelrabatt 1**: Rabatt auf den Glasgrundpreis in Prozent. Der Rabatt gilt ab der Menge, die für den Kunden festgelegt ist.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu2
- **Gasgrundpreis**: Grundpreis für die Gasfüllung bei ISO-Artikeln. In den Feldern können Sie folgende Werte angeben:
  - **Gasgrundpreis:** Gasgrundpreis pro Quadratmeter.
    **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu3
  - **Mindestpreise (in Zeile Gasgrundpreis):** Mindestpreis für den Gasgrundpreis. Der Preis, der festgelegt wird, wenn der berechnete Preis in der Auftragsposition niedriger ist als der angegebene Mindestpreis.
    **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu21
- **1. Austausch, 2. Austausch, 3. Austausch**: In den Feldern geben Sie die Preise für die Austauschartikel in der Stückliste an. Sie können max. drei Austauschpreise festlegen:
  - **1. Austausch, 2. Austausch, 3. Austausch:** Nummer der Austauschliste.
    **Technische Info:** numerische Felder, DB-Felder: pokokon.atmat1, pokokon.atmat2, pokokon.atmat3
  - **PG:** Preisgruppe.
    **Technische Info:** Anzeigefelder, DB-Felder
  - **(Artikelpreis):** Preis des Austausch-Artikels pro Quadratmeter.
    **Technische Info:** numerische Felder, alphanumerische Felder, DB-Felder: pokokon.atp1, pokokon.atp2, pokokon.atp3
  - **Mindestpreise (in Zeile 1. Austausch, 2. Austausch, 3. Austausch):** Mindestpreis für den Austausch. Der Preis, der festgelegt wird, wenn der berechnete Preis in der Auftragsposition niedriger ist als der angegebene Mindestpreis.
    **Technische Info:** numerische Felder, DB-Felder: pokokon.zu22, pokokon.zu23, pokokon.zu25
- **Mengenstaffelrabatt 2**: Rabatt auf den Austauschpreis in Prozent. Der Rabatt gilt ab der Menge, die für den Kunden festgelegt ist.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu4

### Zuschläge

- **Teuerungszuschlag**: Prozentualer Teuerungszuschlag, der auf den Mengeneinheitspreis aufgeschlagen wird. Wenn Sie den Wert 0 oder einen Wert <0 eintragen, wird kein Teuerungszuschlag berechnet.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu5
- **Druckausgleich**: Zuschlag für Druckausgleich in Prozent.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu6
- **Serienrabatt**: Rabatt auf den Glaspreis in Prozent. Der Rabatt gilt ab der Anzahl an Scheiben, die für den Kunden festgelegt ist.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu7
- **Warengruppenfaktor**: Faktor, der bei Erreichen der Grenzmenge für die Warengruppe berücksichtig wird. Wenn Sie einen Faktor < 100 % angeben, wird er als Rabatt verwendet und reduziert den Preis.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu8
- **Modellzuschlag**: Preiszuschlag in Prozent, der bei Modellen erhoben wird.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu9
- **Mindestmodellzusch.**: Mindestpreiszuschlag, der bei Modellen erhoben wird. Wenn der berechnete Modellzuschlag im Auftrag kleiner ist als der definierte Mindestmodellzuschlag, wird dieser Mindestzuschlag erhoben.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu10
- **Einzelmodellzuschlag**: Preiszuschlag in Prozent für bestimmte Modelle.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu11
- **Stufenzuschlag**: Preiszuschlag für die Stufenbearbeitung pro Stück.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu19
- **Transportzuschlag**: Preiszuschlag für den Transport in der Währungseinheit.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu12
- **Gesamtzuschlag**: Preiszuschlag für die Position in Prozent.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu13
- **Verglasung**: Preiszuschlag für die Verglasung in der Währungseinheit pro Quadratmeter.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu14
- **Versiegelung**: Preiszuschlag für die Versiegelung in der Währungseinheit pro laufendem Meter.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu15
- **UV-Abdeckung**: Preiszuschlag für die UV-Abdeckung pro laufendem Meter.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu24

### (Bereich ohne Bezeichnung)

- **Maßrundung**: Maßrundung in Millimeter.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu16
- **Minberech.**: Mindestanzahl der Mengeneinheiten, für die der Preis berechnet wird. Wenn die Menge in der Auftragsposition kleiner ist als die Mindestmenge, wird der Preis für diese Mindestmenge berechnet.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu17
- **Minkant.**: Mindestkantenlänge in Millimeter.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu18

### Bearbeitungen

- **Ecken TZ, Ecken Faktor**: Teuerungszuschlag und Faktor des Preiszuschlags in Prozent für Eckbearbeitungen, z. B. Eckabschnitt.
  **Technische Info:** numerische Felder, DB-Feld: pokokon.zu26
- **Kanten TZ, Kanten Faktor**: Teuerungszuschlag und Faktor des Preiszuschlags in Prozent für Kantenbearbeitungen, z. B. Polieren.
  **Technische Info:** numerische Felder, DB-Feld: pokokon.zu27, pokokon.zu28
- **Fläche TZ, Fläche Faktor**: Teuerungszuschlag und Faktor des Preiszuschlags in Prozent für Flächenbearbeitungen, z. B. Beschichtung.
  **Technische Info:** numerische Felder, DB-Feld: pokokon.zu29, pokokon.zu30

### Fußzeile

In diesem Bereich werden die Bezeichnung des Artikels und das Kennzeichen der Warengruppe des Artikels angezeigt.

## Konditionen für PKZ-FARBARTIKEL

**Navigation:** `Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Preismethode PKZ-Farbartikel > <Shift> + <F9>`

[Image: Abb. D-124 Konditionen für PKZ-FARBARTIKEL. A dialog showing price conditions for color articles, with separate sections for sales and purchase.]

In diesem Dialog werden die Preiskonditionen eines Positionsartikels angezeigt, dem die Preismethode PKZ-Farbartikel zugeordnet ist. Sie können die Konditionen bearbeiten.

Im Dialog Konditionen für PKZ-FARBARTIKEL sind die Breiche Verkauf und Einkauf analog aufgebaut.

Wenn Zusatz-Bearbeitungen in der Stückliste der Position enthalten sind, dann sind die Register Bearbeitungspreise (VK), (EK) aktiv:
⇨ "Positionskonditionen - Bearbeitungspreise (VK), (EK), Detailansicht" auf Seite D-307

### Kopfbereich

- **VK-PKZ**: Preiskennzeichen der vordefinierten Preisliste für den Verkauf.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.pkz
- **EK-PKZ**: Preiskennzeichen der vordefinierten Preisliste für den Einkauf.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.ekpkz

### Register Konditionen

Die meisten Felder sind zum Dialog Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG beschrieben:
⇨ "Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG" auf Seite D-282

Zusätzlich werden folgende Felder angezeigt:

- **Grundpreis**: Grundpreis des Artikels. Der Preistyp bestimmt, worauf sich der Preis bezieht:
  - **WE/Stück:** Der Preis gilt pro Stück.
  - **WE/GME:** Der Preis gilt pro Grundmengeneinheit, z. B. pro Quadratmeter.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.flag2
- **Mindestberechnung**: Mindestanzahl der Mengeneinheiten, für die der Preis berechnet wird. Wenn die Menge in der Auftragsposition kleiner ist als die Mindestmenge, wird der Preis für diese Mindestmenge berechnet.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu6, pokokon.zuk6

### Fußzeile

In diesem Bereich werden die Bezeichnung des Artikels und das Kennzeichen der Warengruppe des Artikels angezeigt.

## Konditionen für PKZ-PREISE-ALLGEMEIN

**Navigation:** `Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Preismethode PKZ-Preise-Allgemein > <Shift> + <F9>`

[Image: Abb. D-125 Konditionen für PKZ-PREISE-ALLGEMEIN. A dialog showing conditions for general articles, with sales and purchase sections.]

In diesem Dialog werden die Preiskonditionen eines Positionsartikels angezeigt, dem die Preismethode PKZ-Preise-Allgemein zugeordnet ist. Sie können die Preiskonditionen bearbeiten.

Im Dialog Konditionen für PKZ-PREISE-ALLGEMEIN sind die Bereiche Verkauf und Einkauf weitgehend analog aufgebaut. Das Feld Gesamtzuschlag wird im Bereich Einkauf nicht angezeigt.

Wenn Zusatz-Bearbeitungen in der Stückliste der Position enthalten sind, dann sind die Register Bearbeitungspreise (VK), (EK) aktiv:
⇨ "Positionskonditionen - Bearbeitungspreise (VK), (EK), Detailansicht" auf Seite D-307

### Kopfbereich

- **VK-PKZ**: Preiskennzeichen der vordefinierten Preisliste für den Verkauf.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.pkz
- **EK-PKZ**: Preiskennzeichen der vordefinierten Preisliste für den Einkauf.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.ekpkz
- **Vektor**: Nummer des Vektors, aus dem der Preis gezogen werden soll.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.matnr

### Register Konditionen

Die meisten Felder sind zum Dialog Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG beschrieben:
⇨ "Konditionen für PKZ-BASISGLAS, PKZ-VEREDELUNG" auf Seite D-282

Zusätzlich werden folgende Felder angezeigt:

- **Grundpreis**: Grundpreis des Artikels. Der Preistyp bestimmt, worauf sich der Preis bezieht:
  - **WE/Stück:** Der Preis gilt pro Stück.
  - **WE/GME:** Der Preis gilt pro Grundmengeneinheit, z. B. pro Quadratmeter.
  **Technische Info:** Toggle-Feld Feld, DB-Feld: pokokon.flag2
- **Mindestberechnung**: Mindestanzahl der Mengeneinheiten, für die der Preis berechnet wird. Wenn die Menge in der Auftragsposition kleiner ist als die Mindestmenge, wird der Preis für diese Mindestmenge berechnet.
  **Technische Info:** numerisches Feld, DB-Feld: pokokon.zu6, pokokon.zuk6

### Fußzeile

In diesem Bereich werden die Bezeichnung des Artikels und das Kennzeichen der Warengruppe des Artikels angezeigt.

## Konditionen für PKZ-GLASTÜREN

**Navigation:** `Verkauf > Auftragserfassung > Register Positionen > Preisfeld von Positionsartikel mit Preismethode PKZ-Glastüren > <Shift> + <F9>`

[Image: Abb. D-126 Konditionen für PKZ-GLASTÜREN. A dialog for setting price conditions for glass doors, showing prices for up to 7 glass panes and surcharges for various processing steps.]

In diesem Dialog werden die Preiskonditionen eines Positionsartikels angezeigt, dem die Preismethode PKZ-Glastüren zugeordnet ist. Sie können die Preiskonditionen bearbeiten.

In den Bereichen Verkauf und Einkauf werden weitgehend die gleichen Felder angezeigt. Im Bereich Verkauf geben Sie die Verkaufspreise an, im Bereich Einkauf die Einkaufspreise.

### Kopfzeile

- **VK-PKZ**: Preiskennzeichen der vordefinierten Preisliste für den Verkauf.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.pkz
- **EK-PKZ**: Preiskennzeichen der vordefinierten Preisliste für den Einkauf.
  **Technische Info:** Pflichtfeld, numerisches Feld, DB-Feld: pokokon.ekpkz

### (Bereich ohne Bezeichnung)

- **Scheibe 1, 2, ..., 7**: Fläche der Scheiben in der GGA. In den nebenstehenden Feldern in den Bereichen Verkauf und Einkauf wird der Quadratmeterpreis für die jeweilige Scheibe angezeigt.
  **Technische Info:** numerische Felder, DB-Felder: pokokon.zu5, pokokon.zu7, pokokon.zu9, pokokon.zu11, pokokon.zu13, pokokon.zu15, pokokon.zu17

