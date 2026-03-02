---
description: "DE-AWEnterprise_15"
---


# Softwarereferenz: A+W Enterprise Verkauf

---
## Rechnungen

### Positionsinfo

**Navigation:**
- `Verkauf > Rechnungen > Automatische Freigabe > Werte angeben > <F5>`
- `Verkauf > Rechnungen buchen > Werte angeben > <F5>`
- `Verkauf > Abschlagsrechnung, Schlussrechnung > Automatische Freigabe > Werte angeben > <F5>`
- `Verkauf > Gutschriften > Gutschriften buchen > Werte angeben > <F5>`

*Abb. D-147 Positionsinfo*

In diesem Dialog werden die Details zu den einzelnen Positionen aus der automatischen Rechnungs- oder Gutschrifterstellung angezeigt.

### Register PositionsInfo I

- **Vorgang:**
    - Vorgangsnummer.
    - Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr
- **Pos:**
    - Nummer der Position im Vorgang.
    - Technische Info: numerisches Feld, DB-Feld: kpos.lfdpos
- **Artikel, Bezeichnung:**
    - Nummer und Bezeichnung des Artikels.
    - Technische Info: numerisches Feld, alphanumerisches Feld, DB-Felder: kpos.artnr, kpos.artbez1
- **F:**
    - Anzeige, ob die Position fakturiert ist.
    - Technische Info: Anzeigefeld, DB-Feld: kauf.fakturakz
- **Menge:**
    - Anzahl der Einheiten der Position.
    - Technische Info: numerisches Feld, DB-Feld: kpos.menge
- **Breite:**
    - Breite der erfassten Glasscheibe in der Position in Millimetern.
    - Technische Info: numerisches Feld, DB-Feld: kpos.laenge
- **Höhe:**
    - Höhe der erfassten Glasscheibe in der Position in Millimetern.
    - Technische Info: numerisches Feld, DB-Feld: kpos.breite
- **Stückpreis:**
    - Preis pro Einheit der Position.
    - Technische Info: numerisches Feld, DB-Feld: kpos.nstpreis
- **Pos. Preis:**
    - Preis der kompletten Position.
    - Technische Info: numerisches Feld, DB-Feld: kpos.npospreis

Mit `<F2>` wechseln Sie zum Register PositionsInfo II.

### Register PositionsInfo II

Die Spalten sind zum Register PositionsInfo I beschrieben:
⇨ "Register PositionsInfo I" auf Seite D-1401

Zusätzlich werden folgende Spalten angezeigt:
- **Mod:**
    - Modellnummer für den Positionsartikel.
    - Technische Info: numerisches Feld, DB-Feld: kpos.modnr
- **gelief.:**
    - Anzahl der Einheiten, die bereits ausgeliefert wurden.
    - Technische Info: numerisches Feld, DB-Feld: kpos.geslief
- **(Feld ohne Bezeichnung):**
    - Anzeige, ob die Position fakturiert ist.
    - Technische Info: Anzeigefeld, DB-Feld: kauf.fakturakz
- **berech.:**
    - Anzahl der Einheiten, die bereits fakturiert wurden.
    - Technische Info: numerisches Feld, DB-Feld: kpos.gesberech
- **SZR 1,SZR 2:**
    - Breite des Scheibenzwischenraums in Millimeter. Bei einem Mehrfachisolierglas wird im SZR1 der erste und im SZR2 der zweiten Scheibenzwischenraum angezeigt.
    - Technische Info: numerische Felder, DB-Felder: kpos.szr, kpos.szr2

## Rechnungen (manuell)

**Navigation:** `Verkauf > Rechnungen > Manuelle Rechnung`

*Abb. D-148 Rechnungen (manuell)*

In diesem Dialog können Sie Rechnungen bearbeiten oder erstellen. Anschließend können Sie die Rechnungen an die FIBU übergeben, wenn das System entsprechend konfiguriert ist.
Wenn Sie eine manuelle Abschlags- oder Schlussrechnung erstellen möchten, können Sie diese auch direkt im entsprechenden Menüpunkt auswählen. Um z. B. eine Abschlagsrechnung manuell zu erstellen, wählen Sie im Menüpfad bei Abschlagsrechnungen die Manuelle Rechnung aus.

Die Felder sind zum Dialog Auftragserfassung beschrieben:
⇨ "Auftragserfassung" auf Seite D-1134

Zusätzlich werden die folgenden Felder angezeigt:

### Kopfbereich

**Rech-Nr.** Rechnungsnummer. Wenn Sie eine Rechnung anlegen, wird vom System eine temporäre Nummer für die Rechnung erstellt. Nach Abschluss der Rechnungserstellung vergibt das System eine endgültige Rechnungsnummer. Auf diese Weise werden die Rechnungen fortlaufend durchnummeriert. Wenn Sie eine vorhandene Rechnungsnummer angeben, wird die entsprechende Rechnung geöffnet.
Die Rechnungen werden in der Datenbanktabelle kauf unter vorgang mit dem Wert 7, mit ihrer endgültig vergebenen Rechnungsnummer gespeichert.
Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr

> **Rechnungen mit Bezug erfassen**
> In der Regel werden Rechnungen immer mit Bezug auf einen Vorgang, z. B. einen Lieferschein oder einen Auftrag, erfasst. Sie können die Vorgangsnummer, für den Sie die Rechnung ausstellen wollen, in dem Feld Bezug im Kopfbereich angeben.

### Register Allgemein

**Berech** Positionsmenge, die berechnet werden soll. Das Feld ist bei einer manuellen Rechnung standardmäßig mit dem Wert Menge aus dem Vorgang vorbelegt. Sie können den Wert verringern.
Technische Info: numerisches Feld, DB-Feld: kpos.berechnet

### Fußbereich

Wenn zu dem Bezugsvorgang bereits eine Rechnung erzeugt wurde, dann wird im Feld **Fakturasaldo** der Rechnungsbetrag aus allen Rechnungen angezeigt, die für diesen Vorgang bereits erfasst wurden.

## Thekenrechnung

**Navigation:** `Verkauf > Rechnungen > Thekenrechnung`

*Abb. D-149 Thekenrechnung*

In diesem Dialog wickeln Sie das Thekengeschäft ab, für Kunden, die ihre Ware selbst abholen und direkt bezahlen. Bei einem Thekengeschäft erfassen Sie die Auftragsdaten und die Rechnung und der Lieferschein werden sofort im Anschluss erstellt.
Die Felder sind zum Dialog Auftragserfassung beschrieben:
⇨ "Auftragserfassung" auf Seite D-1134

## Rechnungen buchen

**Navigation:** `Verkauf > Rechnungen > Rechnungen buchen`

*Abb. D-150 Rechnungen buchen*

In diesem Dialog buchen Sie Rechnungen, die noch nicht an die FIBU übergeben worden sind. In der Regel werden Rechnungen nach dem Erzeugen automatisch gebucht.

In Ausnahmefällen kann die Rechnung auch nachträglich gebucht werden. In der Rechnungserfassung wird je nach Konfiguration beim Erzeugen der Rechnung eine Abfrage angezeigt, ob die Rechnung gebucht werden soll. Wenn Sie die Abfrage mit [Nein] beantworten, können Sie diese ungebuchte Rechnung im Dialog Rechnungen buchen importieren und nachträglich buchen.

Mit `<Strg> + <F8>` importieren Sie die Daten aller Rechnungen, die in dem festgelegten Zeitraum erzeugt worden sind.

Mit `<Strg> + <F5>` können Sie in die ausgewählte Rechnung wechseln und kontrollieren, jedoch solange diese noch nicht gebucht ist. Wird die Rechnung bei dieser Vorgehensweise geändert und gespeichert, so kann sie in dem Dialog Rechnungen auch direkt verbucht werden. Beantworten Sie die entsprechende Frage mit Ja.

In der Fußzeile wird der Kundenname und der Gesamtbetrag aus dem Auftrag angezeigt, für den die Rechnung gebucht wird.

Mit `<F3>` werden die ausgewählten Rechnungen gebucht.

### Register Verkaufs-Rechnung

- **Rechnung:** Rechnungsnummer. Wenn Sie eine Nummer angeben, werden in die übrigen Spalten die entsprechenden Werte eingetragen.
  - Technische Info: Pflichtfeld, numerisches Feld
- **Subnr:** Anzeige der Subnummer für Teilrechnungen.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.subnr
- **Fremdnummer:** Anzeige der Vorgangsnummer, die vom Kunden vorgegeben wird. Für Aufträge aus einem anderen Haus steht in diesem Feld die Auftragsnummer des sendenden Hauses.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.exaufnr
- **Referenz:** Anzeige der Referenz-Vorgangsart, z. B. Auftrag.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.refvorgang
- **Nummer:** Anzeige der Referenz-Vorgangsnummer.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.auftrnr
- **Subnr:** Anzeige der Subnummer für Referenz-Teilvorgang.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.subnr
- **Belegdatum:** Anzeige des Datums der Rechnungserstellung.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.edat
- **Betrag:** Anzeige der Rechnungssumme.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.wpreis
- **Erfasser:** Anzeige des Mitarbeiters-Namen.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.eusr
- **Buch.datum:** Anzeige des Datums der Rechnungsbuchung. Standardmäßig ist das aktuelle Datum eingegeben. Wenn Sie ein anderes Buchungsdatum angeben wollen, müssen Sie das neue Datum in das Feld eingeben, die Eingabe bestätigen und das neue Datum nochmals eingeben. Das Datum wird erst nach der zweiten Eingabe in das Feld übernommen.
  - Technische Info: Datumsfeld, DB-Feld: kauf.bdat
- **Bu.:** Angabe, ob die Rechnung gebucht werden soll.
  - ☑ Die Rechnung wird gebucht.
  - ☐ Die Rechnung wird nicht gebucht.
  - Technische Info: Checkbox

### Register Information zum Vorgang

Das Register Information zum Vorgang ist nur in den Dialogen Rechnungen (automatisch) und Lieferscheine (automatisch) freigeschaltet:
⇨ "Rechnungen (automatisch)" auf Seite D-1398
⇨ "Lieferscheine (automatisch)" auf Seite D-1392

## Abschlagsrechnung (automatisch)

**Navigation:** `Verkauf > Rechnungen > Abschlagsrechnung > Automatische Freigabe`

*Abb. D-151 Abschlagsrechnung (automatisch)*

In diesem Dialog erstellen Sie die Abschlagsrechnungen für Aufträge anhand eines entsprechenden Zahlungsplans. Wenn es für den aktuellen Tag Aufträge gibt, für die ein Zahlungsplan existiert, dann können Sie die Aufträge mit `<Strg> + <F8>` importieren. Sie können die Auftragsnummern auch manuell eingeben oder mit `<F9>` nach Aufträgen suchen.

In der Fußzeile wird der Kundenname und der Gesamtbetrag aus dem Auftrag angezeigt, für den eine Abschlagsrechnung erstellt wird.

Mit `<F3>` werden die Abschlagsrechnungen zu den ausgewählten Aufträgen vom System erzeugt.

- **Auftrag:** Auftragsnummer.
  - Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kauf.auftrnr
- **Haus:** Anzeige der Mandantennummer (Hausnummer).
  - Technische Info: Anzeigefeld, DB-Feld: kauf.hausnr
- **Betrag:** Abschlagsbetrag aus dem Zahlungsplan.
  - Technische Info: numerisches Feld, DB-Feld: zahlplan.betrag
- **Lieferschein:** Anzeige, ob ein Lieferschein oder Teillieferschein existiert. Wenn ein Lieferschein existiert, steht in diesem Feld der Eintrag `existiert`.
  - Technische Info: Anzeigefeld
- **Datum:** Anzeige des Termins für die Fälligkeit des Abschlagsbetrags.
  - Technische Info: Anzeigefeld, DB-Feld: zahlplan.ztplan
- **Ko.:** Kontrolliert. Anzeige, ob die Rechnung bereits kontrolliert wurde. Je nach Konfiguration kann eine Rechnung nur erstellt werden, wenn diese bereits vom autorisierten Mitarbeiter kontrolliert wurde.
  - ☑ Die Rechnung wurde kontrolliert und kann erzeugt werden.
  - ☐ Die Rechnung wurde noch nicht kontrolliert. Je nach Konfiguration kann die Rechnung nicht erzeugt werden.
  - Technische Info: Checkbox, Anzeigefeld
- **Er.:** Erzeugen der Abschlagsrechnung, wenn Sie die Rechnungserstellung mit `<F3>` auslösen.
  - ☑ Abschlagsrechnung erstellen.
  - ☐ Keine Abschlagsrechnung erstellen.
  - Technische Info: Checkbox

> **Zahlungsbedingungen bei Abschlagsrechnung**
> In der Standard-Konfiguration werden die Abschlagsrechnungen ohne Zahlungsbedingungen (wie z. B., Skonto) erzeugt. Mithilfe einer separaten Systemkonfiguration kann das geändert werden. In diesem Fall werden Abschlagsrechnungen bereits mit Skonto des Auftrages erzeugt. Bei der Schlussrechnung werden alle automatisch erzeugten Rabatte für alle vorhandenen Abschlagsrechnungen als skontierbare Rabatte gekennzeichnet. Bei weiteren Fragen zur Nutzung der Funktion wenden Sie sich an zuständigen A+W-Mitarbeiter.

### Register Information zum Vorgang

Das Register Information zum Vorgang ist nur in den Dialogen Rechnungen (automatisch) und Lieferscheine (automatisch) freigeschaltet:
⇨ "Rechnungen (automatisch)" auf Seite D-1398
⇨ "Lieferscheine (automatisch)" auf Seite D-1392

## Abschlagsrechnung (manuell)

**Navigation:** `Verkauf > Rechnungen > Abschlagsrechnung > Manuelle Rechnung`

*Abb. D-152 Abschlagsrechnung (manuell)*

In diesem Dialog können Sie manuell Abschlagsrechnungen erstellen.
Wenn es zu dem Auftrag einen Zahlungsplan gibt, erscheint ein Hinweis mit der Frage, ob die Termine zu dem Zahlungsplan angezeigt werden sollen. Wenn Sie bestätigen, dann können Sie einen Termin aus dem Zahlungsplan auswählen.

Manuelle Abschlagsrechnungen werden wie manuellen Rechnungen erfasst. Die Dialoge Abschlagsrechnung (manuell) und Rechnungen (manuell) sind weitgehend analog aufgebaut.

Im Positionsbereich wird eine neue Position in der letzten Zeile angezeigt. Sie listet den Abschlag mit dem Betrag aus dem Zahlungsplan auf.

Die Felder sind zum Dialog Rechnungen (manuell) beschrieben:
⇨ "Rechnungen (manuell)" auf Seite D-1403

Zusätzlich werden die folgenden Felder angezeigt:

### Fußbereich

Der Gesamtbetrag des Auftrags wird im Feld **Auftragswert** angezeigt. Wenn zu dem Bezugsvorgang bereits eine Rechnung erzeugt wurde, wird der Gesamtbetrag der Rechnung, auf die Bezug genommen wird, im Feld **Fakturasaldo** angezeigt.

## Schlussrechnung (automatisch)

**Navigation:** `Verkauf > Rechnungen > Schlussrechnung > Automatische Freigabe`

*Abb. D-153 Schlussrechnung (automatisch)*

In diesem Dialog erstellen Sie die Schlussrechnung für Aufträge, zu denen ein Zahlungsplan erstellt wurde. Wenn es für den aktuellen Tag Aufträge gibt, für die ein Zahlungsplan existiert, dann können Sie die Aufträge mit `<Strg> + <F8>` importieren. Sie können die Auftragsnummern auch manuell eingeben oder mit `<F9>` nach Aufträgen suchen.

In der Fußzeile wird der Kundenname und der Gesamtbetrag aus dem Auftrag angezeigt, für den eine Schlussrechnung erstellt wird.

Mit `<F3>` werden die Schlussrechnungen zu den ausgewählten Aufträgen vom System erzeugt. In der Auftragserfassung werden die einzelnen Aufträge als fakturiert und mit der jeweiligen Rechnungsnummer angezeigt.

- **Auftrag:** Auftragsnummer mit Zahlungsplan. Wenn Sie eine Nummer angeben, werden die übrigen Felder automatisch mit den entsprechenden Werten belegt.
  - Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kauf.auftrnr, zahlplan.auftrnr
- **Betrag:** Betrag der Schlussrechnung. Die Schlussrechnung wird berechnet aus dem Gesamtbetrag des Auftrags zusammen mit den Gutschriften und abzüglich der bereits erfassten Abschlagsrechnungen.
  - Technische Info: Anzeigefeld, DB-Feld: zahlplan.betrag
- **Lieferschein:** Anzeige, ob ein Lieferschein oder Teillieferschein existiert. Wenn ein Lieferschein existiert, steht in diesem Feld der Eintrag `existiert`.
  - Technische Info: Anzeigefeld
- **Datum:** Anzeige des Erfassungsdatums des Vorgangs.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.edat
- **Ko.:** Kontrolliert. Anzeige, ob die Rechnung bereits kontrolliert wurde. Je nach Konfiguration kann eine Rechnung nur erstellt werden, wenn diese bereits vom Chef kontrolliert wurde.
  - ☑ Die Rechnung wurde kontrolliert und kann erzeugt werden.
  - ☐ Die Rechnung wurde noch nicht kontrolliert. Je nach Konfiguration kann die Rechnung nicht erzeugt werden.
  - Technische Info: Checkbox, Anzeigefeld
- **Er.:** Erzeugt. Angabe, ob die Rechnung erstellt werden soll.
  - ☑ Die Schlussrechnung wird erzeugt.
  - ☐ Die Schlussrechnung wird nicht erzeugt.
  - Technische Info: Checkbox

## Schlussrechnung (manuell)

**Navigation:** `Verkauf > Rechnungen > Schlussrechnung > Manuelle Rechnung`

*Abb. D-154 Schlussrechnung (manuell)*

In diesem Dialog können Sie manuell Schlussrechnungen erstellen.
Manuelle Schlussrechnungen werden wie manuellen Rechnungen erfasst. Die Dialoge Schlussrechnung (manuell) und Rechnungen (manuell) sind weitgehend analog aufgebaut.

Die Felder sind zum Dialog Rechnungen (manuell) beschrieben:
⇨ "Rechnungen (manuell)" auf Seite D-1403

Zusätzlich werden die folgenden Felder angezeigt:

### Fußbereich

Der Gesamtbetrag des Auftrags wird im Feld **Auftragswert** angezeigt. Wenn zu dem Bezugsvorgang bereits eine Rechnung erzeugt wurde, wird der Gesamtbetrag der Rechnung, auf die Bezug genommen wird, im Feld **Fakturasaldo** angezeigt.

## Rechnungsprotokoll

**Navigation:** `Verkauf > Rechnungen > Protokoll`

*Abb. D-155 Rechnungsprotokoll*

In diesem Dialog wird das Rechnungsprotokoll angezeigt. Alle Vorgänge zu den Rechnungen sind mit der Angabe des Datums und der Zeit vermerkt.

Wenn Sie mit interner Mandantentrennung arbeiten, öffnet sich zunächst ein Dialog zur Angabe der Mandantennummer (Hausnummer). In dem Protokoll werden nur die Vorgänge zum ausgewählten Haus angezeigt.

> **Rechnungsprotokoll zu dem aktuellen Tag**
> Ein Rechnungsprotokoll wird zu dem aktuellen Tag erzeugt. Wenn die Fehlermeldung angezeigt wird, dass die Datei leer oder nicht lesbar ist, dann wurde an diesem Tag noch keine Rechnung erzeugt.

## Gutschriften

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Gutschriften" auf Seite D-1414
- "Gutschriften buchen" auf Seite D-1416

### Gutschriften

**Navigation:** `Verkauf > Gutschriften > Gutschrift erfassen`

*Abb. D-156 Gutschriften*

In diesem Dialog erfassen Sie Gutschriften. Sie können Mengengutschriften oder Preis-Gutschriften erfassen. Wenn Sie eine Mengengutschrift erfassen wollen, müssen Sie die Artikelstückzahl, die Sie gutschreiben wollen, im Feld **Gutschr.** der entsprechenden Position eingeben. Wenn Sie eine Preisgutschrift erfassen wollen, müssen Sie den Preis, den Sie gutschreiben wollen, im Preisfeld der entsprechenden Position eingeben.

Die Felder sind zum Dialog Auftragserfassung beschrieben:
⇨ "Auftragserfassung" auf Seite D-1134

Zusätzliche werden folgende Felder angezeigt:

### Kopfbereich

**Gutschr.** Temporäre Nummer der Gutschrift. Nach Abschluss der Gutschrifterstellung erstellt das System eine endgültige Gutschriftnummer.
Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr

**Bezug** Vorgangsnummer, auf die Bezug genommen wird. Standardmäßig wird bei einer Gutschrift eine Rechnungsnummer eingegeben.
Technische Info: numerisches Feld, DB-Feld: kauf.referenz

### Register Allgemein

**Gutschr.** Anzahl der gutgeschriebenen Einheiten der Position.
Technische Info: numerisches Feld, DB-Feld: kpos.berechnet

### Fußbereich

Wenn zu dem Bezugsvorgang bereits eine Rechnung erzeugt wurde, wird der Gesamtbetrag der Rechnung, auf die Bezug genommen wird im Feld **Fakturasaldo** angezeigt.

### Gutschriften buchen

**Navigation:** `Verkauf > Gutschriften > Gutschriften buchen`

*Abb. D-157 Gutschriften buchen*

In diesem Dialog buchen Sie Gutschriften, die noch nicht an die FIBU übergeben worden sind. In der Regel werden Gutschriften nach dem Erzeugen automatisch gebucht.

In Ausnahmefällen kann die Gutschrift auch nachträglich gebucht werden. In der Gutschriftenerfassung wird je nach Konfiguration beim Erzeugen der Gutschrift eine Abfrage angezeigt, ob die Gutschrift gebucht werden soll. Wenn Sie die Abfrage mit [Nein] beantworten, können Sie diese ungebuchte Gutschrift im Dialog Gutschriften buchen importieren und nachträglich buchen.

Mit `<Strg> + <F8>` importieren Sie die Daten aller Gutschriften, die in dem festgelegten Zeitraum erzeugt worden sind.

Mit `<Strg> + <F5>` können Sie in die ausgewählte Gutschrift wechseln und kontrollieren, jedoch solange diese noch nicht gebucht ist. Wird die Gutschrift bei dieser Vorgehensweise geändert und gespeichert, so kann sie in dem Dialog Gutschriften auch direkt verbucht werden. Beantworten Sie die entsprechende Frage mit Ja.
"Gutschriften" auf Seite D-1414

In der Fußzeile wird der Kundenname und der Gesamtbetrag aus dem Auftrag angezeigt, für den die Gutschrift gebucht wird.

Mit `<F3>` werden die ausgewählten Gutschriften gebucht.

### Register Gutschriften

- **Gutschr.:** Nummer der Gutschrift.
  - Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr
- **Fremdnummer:** Anzeige der Vorgangsnummer, die vom Kunden vorgegeben wird. Für Gutschriften aus einem anderen Haus steht in diesem Feld die Gutschriftennummer des sendenden Hauses.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.exaufnr
- **Referenz:** Anzeige der Referenz-Vorgangsart, z. B. Auftrag.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.refvorgang
- **Nummer:** Anzeige der Referenz-Vorgangsnummer.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.auftrnr
- **Subnr:** Anzeige der Subnummer für Referenz-Teilvorgang.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.subnr
- **Belegdatum:** Anzeige des Datums der Gutschrifterstellung.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.edat
- **Betrag:** Anzeige des gutgeschriebenen Beitrags.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.wpreis
- **Erfasser:** Anzeige des Mitarbeiters-Namen.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.eusr
- **Buch.datum:** Anzeige des Datums der Gutschriftbuchung. Standardmäßig ist das aktuelle Datum eingegeben. Wenn Sie ein anderes Buchungsdatum angeben wollen, müssen Sie das neue Datum in das Feld eingeben, die Eingabe bestätigen und das neue Datum nochmals eingeben. Das Datum wird erst nach der zweiten Eingabe in das Feld übernommen.
  - Technische Info: Datumsfeld, DB-Feld: kauf.bdat
- **Bu.:** Angabe, ob die Gutschrift gebucht werden soll.
  - ☑ Die Gutschrift wird gebucht.
  - ☐ Die Gutschrift wird nicht gebucht.
  - Technische Info: Checkbox

Mit `<F5>` öffnen Sie den Dialog Positionen, in dem weitere Details zu den Positionen angezeigt werden.
⇨"Positionsinfo" auf Seite D-1401

### Register Information zum Vorgang

Das Register Information zum Vorgang ist nur in den Dialogen Rechnungen (automatisch) und Lieferscheine (automatisch) freigeschaltet:
⇨ "Rechnungen (automatisch)" auf Seite D-1398
⇨ "Lieferscheine (automatisch)" auf Seite D-1392

## Formulare

Sie können zu den verschiedenen Vorgängen Formulare drucken oder per E-Mail versenden. Die Formulare können über einen REP-Generator oder einen Printservice mit Crystal Reports erzeugt werden.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Direktdruck" auf Seite D-1419
- "Formulardruck" auf Seite D-1420
- "E-Mail" auf Seite D-1424
- "Drucken auf" auf Seite D-1427
- "Listendruck" auf Seite D-1428

### Direktdruck

**Navigation:** `Verkauf > Auftragserfassung > Kopf-, Fußbereich > <F4> > Direktdruck`

*Abb. D-158 Direktdruck*

In diesem Dialog drucken Sie ein Formular zu dem geöffneten Vorgang aus. In den Auswahldialogen wählen Sie die Formularart sowie den Drucker für den Ausdruck aus.

**Formularart** Angabe der Formularart, die Sie zu dem geöffneten Vorgang drucken wollen. Mit `<F9>` öffnen Sie einen Auswahldialog mit den verfügbaren Formulararten. Die Formulararten werden in den Systemeinstellungen in der Druckverwaltung hinterlegt.
Technische Info: numerisches Feld, DB-Feld: rep.formart

**Drucker** Nummer des Druckers für den Druck. Mit `<F9>` öffnen Sie einen Auswahldialog mit den verfügbaren Druckern. Die Drucker werden in den Systemeinstellungen in der Druckverwaltung hinterlegt und den verschiedenen Formulararten zugeordnet.
Technische Info: numerisches Feld, DB-Feld: drucker.drunr

Der Druck startet, wenn Sie eine Formularart und einen Drucker gewählt haben und das System entsprechend konfiguriert ist. Der Dialog **Direktdruck** schließt sich automatisch.

### Formulardruck

**Navigation:** `Verkauf > Formulare > Druck`

*Abb. D-159 Formulardruck*

In diesen Dialogen wählen Sie einen oder mehrere Vorgänge für den Formulardruck aus.

Im Auswahldialog **Formularart** wählen Sie die Formularart, die Sie ausdrucken wollen. Die ausgewählte Formularart wird im Dialog **Formulardruck** in der linken oberen Ecke angezeigt. Unter Umständen können Sie auch mehrere Formulararten wählen, z. B. Auftragsbestätigung und Vorablieferschein.

**sortiert nach** Sortierung der Formulare. Standardmäßig sind die Formulare nach Vorgangsnummern sortiert. Das Feld ist nur freigeschaltet, wenn Sie mehrere Formulararten ausgewählt haben.
- **NUMMERN:** Die Formulare sind nach Vorgangsnummern sortiert.
- **FORMULARE:** Die Formulare sind nach Formularart sortiert.
Technische Info: Toggle-Feld

**zusätzliche Exemplare** Anzahl der zusätzlichen Druck-Exemplare bis maximal 99. Standardmäßig wird ein Formular gedruckt.
Technische Info: numerisches Feld

**(Feld ohne Bezeichnung)** Angabe, wie die Vorgänge für den Formulardruck ermittelt werden sollen.
- **Nummern auswählen:** Im Kopfbereich des Dialogs Formulardruck können Sie die Vorgänge nach verschiedenen Kriterien filtern. In der Übersicht werden nur die Vorgänge für den Formulardruck angezeigt, die den Filterkriterien entsprechen. Standardmäßig ist das Feld mit diesem Wert vorbelegt.
  ⇨ "Übersicht" auf Seite D-1422
- **diverse Nummern vorgeben:** In der Übersicht werden keine Vorgänge angezeigt. Sie stellen die Liste der Vorgänge manuell zusammen.
  ⇨ "Übersicht" auf Seite D-1422
Technische Info: Toggle-Feld

Mit `<Enter>` bestätigen Sie die Auswahl.

#### Kopfbereich (Nummern auswählen)

**von, bis** Anfangs- und Endwert der Filterkriterien:
- **Mitarb.:** Nummer des Mitarbeiters, der den Vorgang erfasst hat. Alle Mitarbeiter mit Nummern zwischen von und bis werden als Filterkriterium einbezogen.
  - Technische Info: numerisches Feld, DB-Feld: kauf.eust
- **Marktpart.:** Nummer des Marktpartners, für den der Vorgang erfasst wurde. Alle Marktpartner mit Nummern zwischen von und bis werden als Filterkriterium einbezogen.
  - Technische Info: numerisches Feld, DB-Feld: kauf.kunr
- **erfasst am:** Datum der Vorgangs-Erfassung. Standardmäßig ist im Feld bis das aktuelle Datum festgelegt. Wie groß der Zeitraum zwischen den beiden Feldern sein darf, ist von der Konfiguration in den Stammdaten abhängig.
  ⇨ Stammdaten, "Periodenende" auf Seite B-285
  - Technische Info: Pflichtfeld, Datumsfeld, DB-Feld: kauf.edat
- **Vorgang:** Vorgangsnummer. Alle Vorgänge mit Nummern zwischen von und bis werden als Filterkriterium einbezogen.
  - Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr
- **Abteilung:** Abteilungsnummer. Alle Abteilungen mit Nummern zwischen von und bis werden als Filterkriterium einbezogen.
  - Technische Info: numerisches Feld, DB-Feld: kauf.abtnr

#### Ausgabe drucken

Angabe, welche Vorgänge in der Übersicht aufgelistet werden sollen. Das System legt eine Druck-Historie an.
- **alle nicht ausgegebenen:** Nur Vorgänge, die noch nicht gedruckt worden sind und den Filterkriterien entsprechen, werden angezeigt.
- **alle:** Alle Vorgänge, die den Filterkriterien entsprechen, werden angezeigt. Die angezeigten Vorgänge können schon gedruckt worden sein. Bei Vorgängen, die bereits gedruckt worden sind, wird das Datum des Drucks in der Spalte gedruckt angezeigt.
- **alle neuen obligator.:** Geänderte Vorgänge, für die ein neuer Ausdruck als obligatorisch festgelegt wurde und die den Filterkriterien entsprechen, werden angezeigt. Die Auswahl ist nur möglich, wenn das System entsprechend konfiguriert ist. In diesem Fall wird beim Speichern eines geänderten Vorgangs eine Abfrage angezeigt, ob der Vorgang für den Ausdruck bereitgestellt werden soll. Bei Bestätigung der Abfrage wird der Vorgang für den Formulardruck unter alle neuen obligator. angezeigt.
  - Technische Info: Toggle-Feld

Mit `<F3>` starten Sie die Suche nach Vorgängen, die den Filterkriterien entsprechen.

#### Übersicht

Unter dem Bereich für die Eingabe der Filterkriterien, werden in einer Übersicht die Vorgänge angezeigt, die den Filterkriterien entsprechen und für den Formulardruck zur Verfügung stehen. Wenn Sie **diverse Nummern vorgeben** gewählt haben, ist die Übersicht leer und Sie können manuell Vorgänge hinzufügen. Wenn Sie **Nummern auswählen** gewählt haben, werden in der Übersicht alle Vorgänge angezeigt, die den angegebenen Filterkriterien entsprechen. Sie können manuell Vorgänge hinzufügen.
- **Dr:** Druckkennzeichen für den Vorgang.
  - **J:** Das Formular für den Vorgang drucken.
  - **N:** Kein Formular für den Vorgang drucken.
  - **X:** Den Vorgang für den Formulardruck sperren.
  - Technische Info: Toggle-Feld, DB-Feld: repform.drflag
- **Vorgang:** Vorgangsnummer.
  - Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: repform.auftrnr
- **Lfd.:** Subnummer der Teilvorgänge, z. B. Teilrechnungen oder Teillieferscheine.
  - Technische Info: numerisches Feld, DB-Feld: repform.subnr
- **Marktpart.:** Matchcode des Marktpartners.
  - Technische Info: Anzeigefeld, DB-Feld: repform.kumc
- **Änderung:** Datum der letzten Vorgangsänderung.
  - Technische Info: Anzeigefeld, DB-Feld: repform.updat
- **Mitarb.:** Nummer des Mitarbeiters, der den Vorgang erfasst hat.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.eusr
- **Gedruckt:** Datum, an dem der Vorgang gedruckt wurde. Wenn der Vorgang noch nicht gedruckt wurde, dann ist das Feld leer.
  - Technische Info: Anzeigefeld, DB-Feld: druckhist.ltzdat
- **Mitarb.:** Nummer des Mitarbeiters, der das Formular für den Vorgang zuletzt gedruckt hat.
  - Technische Info: Anzeigefeld, DB-Feld: druckhist.ltzmanr
- **Route:** Routennummer.
  - Technische Info: Anzeigefeld, DB-Feld: repform.routenr
- **Termin:** Liefertermin beim Kunden.
  - Technische Info: Anzeigefeld, DB-Feld: repform.liefdat

Mit `<F2>` zeigen Sie zusätzlich folgende Spalte an:
- **Marktpart.:** Marktpartnernummer.
  - Technische Info: Anzeigefeld, DB-Feld: repform.kunr
- **Fax:** Faxnummer des Marktpartners für den Vorgang.
  - Technische Info: alphanumerisches Feld, DB-Feld: repform.faxnr

Mit `<Shift> + <F3>` starten Sie den Druckvorgang.
⇨ "Drucken auf" auf Seite D-1427

### E-Mail

**Navigation:** `Verkauf > Formulare > E-Mail/Fax`

*Abb. D-160 Dialoge unter E-Mail/Fax - Menü*

Über die Dialoge unter Menüpunkt E-Mail/Fax wählen Sie einen Vorgang für den Versand von Formularen per E-Mail aus.
Damit Formulare per E-Mail versendet werden können, muss das System entsprechend konfiguriert sein. Zuerst wählen Sie die Formularart, z. B. Auftragsbestätigung aus, die versendet werden soll. Anschließend wählen Sie die Art, wie die Vorgangsnummer-Ermittlung gestaltet werden soll.

**Formularart** Angabe der Formularart, die Sie per E-Mail oder Fax versenden wollen. Die ausgewählte Formularart wird im Dialog E-Mail in der linken oberen Ecke angezeigt.
Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: rep.formart

**Vorgangswahl durch** Angabe, welche Vorgänge angezeigt werden sollen.
- **Nummern auswählen:** Beim Auswahl dieses Wertes startet ein weiterer Dialog, im dessen Kopfbereich können Sie die Vorgänge nach verschiedenen Kriterien filtern. In der Übersicht werden nur die Vorgänge für den Formulardruck angezeigt, die den Filterkriterien entsprechen.
  ⇨ "Übersicht" auf Seite D-1422
- **diverse Nummern vorgeben:** In der Übersicht werden keine Vorgänge angezeigt. Es startet ein leerer Übersichts-Dialog, in dem Sie die Liste der Vorgänge manuell zusammenstellen können.
  ⇨ "Übersicht" auf Seite D-1422
Technische Info: Toggle-Feld

Mit `<Enter>` bestätigen Sie die Auswahl.

Sie können Formulare per E-Mail oder Fax nur dann an einen Marktpartner versenden, wenn die E-Mail-Adresse und die Faxnummer in den Stammdaten des Markpartners hinterlegt ist. Diese Adresse oder Nummer wird standardmäßig im Dialog E-Mail herangezogen, wenn Sie einen Vorgang aufrufen.

In der Vorgangserfassung können Sie im Register Anschriften eine E-Mail-Adresse und Faxnummer hinterlegen, die sich von den Angaben in den Stammdaten unterscheidet. Wenn Sie im Dialog E-Mail einen Vorgang mit abweichender E-Mail-Adresse oder Faxnummer aufrufen, wird eine Meldung angezeigt, ob die abweichende Adresse oder Nummer aus dem Vorgang herangezogen werden soll.

#### Kopfbereich (Nummern auswählen)
Der Kopfbereich ist zum Dialog Formulardruck beschrieben:
"Formulardruck" auf Seite D-1420

#### Kopfbereich (diverse Nummern vorgeben)
Der Kopfbereich ist zum Dialog Formulardruck beschrieben:
"Formulardruck" auf Seite D-1420

#### Ergebnisbereich

*Abb. D-161 E-Mail: Ergebnisbereich*

Im Dialog E-Mail/Fax stehen nun im Ergebnisbereich zwei Register zur Verfügung: **Übersicht** und **Weitere Daten**.

Die Felder sind zum Dialog Formulardruck beschrieben:
"Formulardruck" auf Seite D-1420

Zusätzlich werden in den Registern folgende Felder angezeigt:

- **E-Mail:** E-Mail-Adresse, an die das Formular versendet wird. Die E-Mail-Adresse wird aus den Stammdaten oder dem Vorgang herangezogen.
  - Technische Info: Pflichtfeld, alphanumerisches Feld
- **gesendet:** Anzeige des Datums, an dem der Vorgang gesendet wurde.
  - Technische Info: Anzeigefeld, DB-Feld: druckhist.ltzdat
- **CC:** E-Mail-Adresse, an die das Formular zusätzlich zur Kenntnisnahme gesendet wird. Die E-Mail-Adresse wird aus den Stammdaten oder dem Vorgang übernommen und kann in diesem Dialog geändert bzw. neue erfasst werden. Das Programm prüft nicht, ob die E-Mail-Adresse regelkonform eingegeben wurde und/oder ob die E-Mail-Adresse existiert.
  - Technische Info: Kann-Feld, alphanumerisches Feld
- **Bcc:** E-Mail-Adresse, an die das Formular als Blind-Kopie zur Kenntnisnahme gesendet wird. Die E-Mail-Adresse wird aus den Stammdaten oder dem Vorgang übernommen und kann in diesem Dialog geändert bzw. neue erfasst werden. Das Programm prüft nicht, ob die E-Mail-Adresse regelkonform eingegeben wurde und/oder ob die E-Mail-Adresse existiert.
  - Technische Info: Kann-Feld, alphanumerisches Feld

### Drucken auf

**Navigation:** `Verkauf > Formulare > Druck > Formular auswählen > <Ende> > Daten eingeben und Auswahl treffen > <Shift> + <F3>`

*Abb. D-162 Drucken auf*

In diesem Dialog wählen Sie den Drucker aus. neben einem physikalischen Drucker können Sie das Formular auch als Datei ausgeben.
In der Fußzeile wird angezeigt, welche Formularart gedruckt wird.

**Druckerauswahl** Nummer und Bezeichnung des Druckers für den Druck. Mit `<F9>` öffnen Sie die Liste der verfügbaren Drucker.
Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: repdruck.drunr

**Dateiname** Für den Dateidruck müssen Sie einen Dateinamen angeben. Dieses Feld wird nur angezeigt, wenn Sie im Feld Druckerauswahl statt eines physikalischen Druckers den Dateidruck auswählen.
Die Ausgabeart der Drucker ist in den Systemeinstellungen in der Druckverwaltung hinterlegt.
Technische Info: Pflichtfeld, alphanumerisches Feld

### Listendruck

**Navigation:** `Verkauf > Listendruck > Liste auswählen`

*Abb. D-163 Listendruck*

In diesem Dialog drucken Sie Listen aus, z. B. die Liste aller Auftragseingänge bestimmter Vertreter innerhalb eines bestimmten Zeitraums.

Zunächst wählen Sie die Liste aus, die Sie drucken wollen. Im Dialog Listendruck können Sie die Liste anschließend nach bestimmten Kriterien filtern.

**Listenname** Name der Liste, die gedruckt werden soll.
Technische Info: Pflichtfeld, Auswahlfeld

Wenn Sie eine Liste gewählt haben, werden verschiedene Felder angezeigt, mit denen Sie die Einträge in der Liste einschränken können.
Die Anzeige der Felder hängt von der ausgewählten Liste der jeweiligen SQL-Abfrage ab.

Wenn Sie die Felder ausgefüllt haben, starten Sie den Listendruck mit `<F3>`.
⇨ "Drucken auf" auf Seite D-1427

## Auftragsstatus

Zu allen Aufträgen können Sie sich die Vorgangs-Informationen anzeigen lassen, z. B. die Statusänderungen.

### Auftragsinformation

**Navigation:** `Verkauf > Übersicht > Auftragsinformation > Auftragsnummer eingeben`

In diesem Dialog wird Ihnen der Bearbeitungsstatus zum gewählten Auftrag angezeigt.

In diesem Dialog finden Sie folgende Register:
- "Vorgangsinformationen – Vorgang" auf Seite D-1430
- "Vorgangsinformationen – Positionen" auf Seite D-1432
- "Vorgangsinformationen – Einkauf" auf Seite D-1433
- "Vorgangsinformationen - Wareneingang" auf Seite D-1435
- "Vorgangsinformationen – Produktion" auf Seite D-1436
- "Vorgangsinformationen – Versand" auf Seite D-1438
- "Vorgangsinformationen – BDE" auf Seite D-1439
- "Vorgangsinformationen – Gestelle" auf Seite D-1441
- "Vorgangsinformationen – Lager" auf Seite D-1442
- "Vorgangsinformationen – Verbundene Prod." auf Seite D-1443
- "Vorgangsinformationen – Zwischenversand" auf Seite D-1444

Für den aktuellen Auftrag können Sie diesen Dialog auch über die Auftragserfassung öffnen:
`Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > <Shift> + <F10>`

### Vorgangsinformationen – Vorgang

**Navigation:** `Verkauf > Übersicht > Auftragsinformation > Auftragsnummer angeben > Register Vorgang`

*Abb. D-164 Auftragsinformationen – Register Vorgang*

In diesem Register wird die Historie des Bearbeitungsstatus des gewählten Vorgangs angezeigt.

#### Register Vorgang

- **Datum:** Datum der Statusbuchung.
  - Technische Info: Anzeigefeld, DB-Feld: kaufstat.datum
- **Aktivität:** Beschreibung des Vorgangsstatus. Die angezeigten Informationen werden vom System herangezogen. Je nach Bearbeitungsstatus des Vorgangs werden die Daten aus A+W Enterprise oder aus einem anderen Programm übernommen, z. B. aus A+W Production.
  - Wenn Sie mit interner Mandantentrennung arbeiten, werden Bearbeitungsstatus pro Mandanten angezeigt.
  - Technische Info: Anzeigefeld

#### Erläuterung der Schaltflächen im Fußbereich

- **[Anmerkungen]** Verzweigt zu Vorgangsanmerkungen in Lese-Modus für den ausgewählten Auftrag, sofern diese existieren. Wenn das System entsprechend konfiguriert ist, können Anmerkungen geändert bzw. neue dazu erfasst werden. Beim Speichern bekommen Sie eine Sicherheitsabfrage. Ist der Auftrag anderweitig gesperrt, wird das Speichern abgewiesen. Nach der Anmerkungsänderungen erfolgt keine Auftragsübergabe an die Hintergrundprozesse. Diese Schaltfläche ist nur im Register Vorgang verfügbar.
- **[Prod.Bericht]** Verzweigt zu einen Produktionsbericht für den ausgewählten Auftrag, wenn dieser existiert und das System entsprechend konfiguriert ist. Der Produktionsbericht wird in einem Browserfenster geöffnet.
- **[Int.Auft.]** Verzweigt zu einem internen Auftrag mit eigener Auftragsnummer für die Produktion, wenn dieser existiert und das System entsprechend konfiguriert ist. Die internen Aufträge können nur erzeugt werden, wenn die Umgebungsvariable VORGANGSSTATUS_ADHOCSQL aktiv ist und Sie eine eigene Ad-Hoc-SQL eingebunden haben. Wenn die Variable nicht gesetzt ist, wird eine entsprechende Fehlermeldung angezeigt.

### Vorgangsinformationen – Positionen

**Navigation:** `Verkauf > Übersicht > Auftragsinformation > Auftragsnummer angeben > Register Positionen`

*Abb. D-165 Auftragsinformationen – Register Positionen*

In diesem Register werden Bestell- und Auftragsdetails zu den Positionen angezeigt.
Wenn sich der Positionsstatus ändert, wird der Status der entsprechenden Position im rechten Teil des Dialogs auf Positionsebene angezeigt, z. B. Verpackt, FIXIERT, Lokal-Korrektur. Jede Position kann einen anderen Status haben. Der angezeigte Positionsstatus gilt jeweils für die markierte Position.
⇨ "Symbolerklärung" auf Seite D-1128

Für weitere Informationen zu den unterschiedlichen Statusanzeigen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

#### Register Positionen

- **Pos.:** Positionsnummer.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.posnr
- **Artikel:** Artikelnummer.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.artnr
- **Menge:** Menge in der Artikelmengeneinheit der bestellten Artikel.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.menge
- **Eingang:** Menge in der Artikelmengeneinheit der bestellten Artikel, die bereits als Wareneingang gebucht sind.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.geslief
- **Verfügbar:** Menge in der Artikelmengeneinheit der fertiggemeldeten Artikel in der Produktion, die ausgeliefert werden können.
  - Technische Info: Anzeigefeld, DB-Feld: lapool.gefstk
- **Verpackt:** Menge in der Artikelmengeneinheit der verpackten Artikel, die bereits versandfertig sind.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.gespack
- **Gelief:** Menge in der Artikelmengeneinheit der Artikel, die bereits ausgeliefert wurden.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.geslief
- **Berech:** Menge in der Artikelmengeneinheit der Artikel, die bereits fakturiert wurden.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.gesberech

#### Fußbereich

Die Bezeichnung des Artikels zur ausgewählten Position wird im Dialog unten links angezeigt.
Die Schaltflächen sind zum Register Vorgang beschrieben:
⇨ "Vorgangsinformationen - Vorgang" auf Seite D-1430

Zusätzlich wird folgende Schaltfläche angezeigt:
- **[Info]** Zeigt die Fehlermeldung aus der Produktion zu der gewählten Position an. Die Schaltfläche ist nur aktiv, wenn zu der gewählten Position eine Fehlermeldung existiert.

### Vorgangsinformationen – Einkauf

**Navigation:** `Verkauf > Übersicht > Auftragsinformation > Auftragsnummer angeben > Register Einkauf`

*Abb. D-166 Auftragsinformationen – Register Einkauf*

In diesem Register werden die Informationen zum Status der Zukaufteile angezeigt.

> **Zwei Felder für Positionsnummern**
> In diesem Register werden zwei Pos. Felder angezeigt. Sie unterscheiden sich und zeigen verschiedene Positionsnummern an.

#### Register Einkauf

Die Spalten sind zum Register Positionen beschrieben:
⇨ "Vorgangsinformationen - Positionen" auf Seite D-1432

Zusätzlich werden folgende Spalten angezeigt:
- **Artikel:** Artikelnummer des bestellten Artikels. Die Nummer wird aus der Stückliste herangezogen.
  - Technische Info: Anzeigefeld, DB-Feld: aufstrukt.artnr
- **Bezeichnung:** Bezeichnung des bestellten Artikels.
  - Technische Info: Anzeigefeld, DB-Feld: artikel.artbez1
- **Best.Nr.:** Bestellnummer des bestellten Artikels. Die Nummer der Bestellung wird im Datenbankfeld kauf.auftrnr für vorgang = 2 gespeichert.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.auftrnr
- **Pos. (Feld zwischen Best.Nr. und Bestellt):** Positionsnummer des Artikels, für den die Artikel bestellt sind.
  - Technische Info: Anzeigefeld, DB-Feld: aufstrukt.posnr
- **Bestellt:** Menge der bestellten bestellten Artikel.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.menge
- **Erhalten:** Menge der erhaltenen Artikel im Wareneingang.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.geslief
- **Bestellt zum:** Gewünschter Liefertermin der bestellten Artikel.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.ltplan
- **EK-Preis:** Netto-Stückpreis der bestellten Artikel.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.nstpreis
- **Kompl:** Position ist komplett, wenn ein Stern * angezeigt wird.
  - Technische Info: Anzeigefeld, DB-Feld: kposp.liefkompl
- **LPI:** Lieferplan. Angabe, ob ein Lieferplan für die Position existiert.
  - **L:** Es existiert ein Lieferplan für die Position.
  - **(leer):** Es existiert kein Lieferplan.
  - Technische Info: Anzeigefeld

#### Fußbereich

Der Name des Lieferanten zur ausgewählten Position wird im Dialog unten links angezeigt.

Die Schaltflächen sind zum Register Positionen beschrieben:
⇨ "Vorgangsinformationen – Positionen" auf Seite D-1432

### Vorgangsinformationen – Wareneingang

**Navigation:** `Verkauf > Übersicht > Auftragsinformation > Auftragsnummer angeben > Register Wareneingang`

*Abb. D-167 Auftragsinformationen – Register Wareneingang*

In diesem Register werden die Informationen zum Status des Wareneingangs für Zukaufteile angezeigt.

> **Zwei Felder für Positionsnummern**
> In diesem Register werden zwei Pos. Felder angezeigt. Sie zeigen in Spalte 1 die Nummer der Auftragsposition und in Spalte 5 bei bestellten Artikeln die Nummer der Bestellposition an.

#### Register Wareneingang

Die Spalten sind zum Register Positionen beschrieben:
⇨ "Vorgangsinformationen - Positionen" auf Seite D-1432

Zusätzlich werden folgende Spalten angezeigt:
- **Bestellung:** Bestellnummer der Zukaufteile.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.auftrnr
- **Pos (Spalte 5 zwischen Bestellung und Lieferung):** Positionsnummer des bestellten Artikels in der Bestellung.
  - Technische Info: Anzeigefeld, DB-Feld: aufstrukt.posnr
- **Lieferung:** Auftragsbestätigungsnummer des Lieferanten. Die Nummer der Auftragsposition wird in DB-Feld kpos.abnr gespeichert.
  - Technische Info: Anzeigefeld, DB-Feld: bpos.abnr
- **Subnr:** Subnummer der Lieferung.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.subnr
- **Avisiert:** Datum der Liefer-Ankündigung.
  - Technische Info: Anzeigefeld, DB-Feld: bpos.ltavis
- **Menge:** Durch den Lieferanten avisierte Menge in der Artikelmengeneinheit.
  - Technische Info: Anzeigefeld, DB-Feld: bpos.avismenge
- **Anl.Datum:** Lieferdatum der Zukaufteile.
  - Technische Info: Anzeigefeld, DB-Feld: bpol.ltplan
- **Erhalten:** Gelieferte Menge in der Artikelmengeneinheit des bestellten Artikels, die im Wareneingang gebucht wurden.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.geliefert
- **LPI:** Lieferplan. Angabe, ob ein Lieferplan für die Position existiert.
  - **L:** Es existiert ein Lieferplan für die Position.
  - **(leer):** Es existiert kein Lieferplan.
  - Technische Info: Anzeigefeld

#### Fußbereich

Die Bezeichnung des Artikels und der Name des Lieferanten zur ausgewählten Position werden im Dialog unten links angezeigt.
Die Schaltflächen sind zum Register Positionen beschrieben:
⇨ "Vorgangsinformationen – Positionen" auf Seite D-1432

### Vorgangsinformationen – Produktion

**Navigation:** `Verkauf > Übersicht > Auftragsinformation > Auftragsnummer angeben > Register Produktion`

*Abb. D-168 Auftragsinformationen – Register Produktion*

In diesem Register wird der Auftragsstatus aus dem Produktionssystem angezeigt.

#### Register Produktion

Die Spalten sind zum Register Positionen beschrieben:
⇨ "Vorgangsinformationen - Positionen" auf Seite D-1432

Zusätzlich werden folgende Spalten angezeigt:
- **Status:** Nummer des Produktionsstatus.
  - Technische Info: Anzeigefeld, DB-Feld: kposstat.status
- **Informationstext:** Bezeichnung des Produktionsstatus. Der Text wird vom System vorbelegt und in der jeweils konfigurierten Systemsprache angezeigt.
  - Technische Info: Anzeigefeld, DB-Feld: kposstat.infotxt
- **Datum:** Datum der Rückmeldung des angezeigten Status.
  - Technische Info: Anzeigefeld, DB-Feld: kposstat.datum
- **Zeit:** Uhrzeit der Rückmeldung des angezeigten Status.
  - Technische Info: Anzeigefeld, DB-Feld: kposstat.zeit
- **Menge:** Menge aus der Rückmeldung in Artikelmengeneinheit.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.menge

#### Fußbereich

Die Bezeichnung des Artikels zur ausgewählten Position wird im Dialog unten links angezeigt.
Die Schaltflächen sind zum Register Positionen beschrieben:
⇨ "Vorgangsinformationen – Positionen" auf Seite D-1432

### Vorgangsinformationen – Versand

**Navigation:** `Verkauf > Übersicht > Auftragsinformation > Auftragsnummer angeben > Register Versand`

*Abb. D-169 Auftragsinformationen – Register Versand*

In diesem Register werden die Informationen zum Status des Versands angezeigt.

#### Register Versand

Die Spalten sind zum Register Positionen beschrieben:
⇨ "Vorgangsinformationen – Positionen" auf Seite D-1432

Zusätzlich werden folgende Spalten angezeigt:
- **Sta:** Ampelanzeige für den aktuellen Positionsstatus.
  - Technische Info: Anzeigefeld
  - ⇨ "Symbolerklärung" auf Seite D-1128
- **Haus:** Mandantennummer (Hausnummer), in der der Auftrag angelegt ist.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.hausnr
- **Route:** Nummer der Versand-Route.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.route
- **Liefertermin:** Datum der Lieferung.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.ltplan
- **Abruf:** Abrufmenge in der Artikelmengeneinheit, die der Kunde zum Liefertermin abruft.
  - Technische Info: Anzeigefeld, DB-Feld: lapool.abrufstk
- **Geplant:** Geplante Menge in der Artikelmengeneinheit, die zum Liefertermin geplant sind.
  - Technische Info: Anzeigefeld, DB-Feld: lapool.sollstk
- **Verfügbar:** Menge in der Artikelmengeneinheit der fertiggemeldeten Artikel, die geliefert werden können.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.gefstk
- **Verpackt:** Verpackte Menge in der Artikelmengeneinheit, die bereits versandfertig ist.
  - Technische Info: Anzeigefeld, DB-Feld: lapool.iststk
- **Versand:** Art des Versands:
  - **Ausgang:** Ware wird versendet.
  - **Eingang:** Ware wird eintreffen, z. B. nach der Bearbeitung durch ein anderes Haus.
  - Technische Info: Anzeigefeld, DB-Feld: kposstat.status

#### Fußbereich

Die Bezeichnung des Artikels zur ausgewählten Position wird im Dialog unten links angezeigt.
Die Schaltflächen sind zum Register Positionen beschrieben:
⇨ "Vorgangsinformationen - Positionen" auf Seite D-1432

### Vorgangsinformationen – BDE

**Navigation:** `Verkauf > Übersicht > Auftragsinformation > Auftragsnummer angeben > Register BDE`

*Abb. D-170 Auftragsinformationen – Register BDE*

In diesem Register werden die Informationen zum BDE-Status angezeigt, wenn Sie mit der Betriebsdatenerfassung arbeiten.
Mit `<F5>` wechseln Sie die Ansicht des Registers. Die Werte werden dann nach Positions- und Betriebsmittelnummer zusammengefasst angezeigt.

#### Register BDE

Die Spalten sind zum Register Positionen beschrieben:
⇨ "Vorgangsinformationen - Positionen" auf Seite D-1432

Zusätzlich werden folgende Spalten angezeigt:
- **Bmnr:** Nummer der Betriebsmittel.
  - Technische Info: Anzeigefeld
- **Datum:** Fertigungsdatum.
  - Technische Info: Anzeigefeld
- **Schicht:** Nummer der Schicht im Mehrschichten-Betrieb.
  - Technische Info: Anzeigefeld
- **Jobnr:** Laufende Nummer des Jobs.
  - Technische Info: Anzeigefeld
- **Etikett:** Nummer des Etiketts für den Druck.
  - Technische Info: Anzeigefeld
- **SollStk:** Stückzahl der Artikel, die produziert werden sollen.
  - Technische Info: Anzeigefeld
- **IstStk:** Stückzahl der Artikel, die bereits produziert sind.
  - Technische Info: Anzeigefeld
- **Bruch:** Stückzahl der Artikel, die zu Bruch gegangen sind.
  - Technische Info: Anzeigefeld

#### Fußbereich

Die Bezeichnung des Artikels zur ausgewählten Position wird im Dialog unten links angezeigt.
Die Schaltflächen sind zum Register Positionen beschrieben:
⇨ "Vorgangsinformationen – Positionen" auf Seite D-1432

### Vorgangsinformationen – Gestelle

**Navigation:** `Verkauf > Übersicht > Auftragsinformation > Auftragsnummer angeben > Register Gestelle`

*Abb. D-171 Auftragsinformationen – Register Gestelle*

In diesem Register werden pro Gestell die Informationen aus der Packmittelplanung angezeigt.
Pro Gestell wird ein Zeile angezeigt, wobei auf einem Gestell mehrere Positionen verpackt sein können, oder eine Position auf mehrere Gestelle verteilt sein kann.

#### Register Gestelle

Die Spalten sind zum Register Positionen beschrieben:
⇨ "Vorgangsinformationen - Positionen" auf Seite D-1432

Zusätzlich werden folgende Spalten angezeigt:
- **Gestell:** Nummer des Gestells, auf das die Artikel verplant sind. Die Nummer wird automatisch vom System vergeben.
  - Technische Info: Anzeigefeld, DB-Feld: kposgest.vsgnr
- **Externe Nummer:** Externe Bestellnummer des Kunden. Bei Aufträgen aus einem anderen Haus steht in diesem Feld die Auftragsnummer des sendenden Hauses.
  - Technische Info: Anzeigefeld, DB-Feld: gestellz.exgnr
- **LfdNr:** Positionsnummer aus dem Auftrag.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.lfdpos
- **Lieferdatum:** Datum der Lieferung für das Gestell.
  - Technische Info: Anzeigefeld, DB-Feld: vsaufgest.ltplan
- **Route:** Nummer der Route, auf der das Gestell transportiert wird.
  - Technische Info: Anzeigefeld, DB-Feld: vsaufgest.routennr
- **IstStk:** Stückzahl der Artikel, die auf das Gestell verplant sind.
  - Technische Info: Anzeigefeld, DB-Feld: lapool.iststk

#### Fußbereich

Die Bezeichnung des Artikels zur ausgewählten Position wird im Dialog unten links angezeigt.
Die Schaltflächen sind zum Register Positionen beschrieben:
⇨ "Vorgangsinformationen – Positionen" auf Seite D-1432

### Vorgangsinformationen – Lager

**Navigation:** `Verkauf > Übersicht > Auftragsinformation > Auftragsnummer angeben > Register Lager`

*Abb. D-172 Auftragsinformationen – Register Lager*

In diesem Register werden die Status-Informationen des Lagerartikels angezeigt, der im Auftrag erfasst ist.

#### Register Lager

Die Spalten sind zum Register Positionen beschrieben:
⇨ "Vorgangsinformationen - Positionen" auf Seite D-1432

Zusätzlich werden folgende Spalten angezeigt:
- **LagerArt:** Nummer des Lagerartikels. Die Lagerartikel sind Unterteile der Positionen, für die eine Lagerbuchung durchgeführt werden muss.
  - Technische Info: Anzeigefeld, DB-Feld: auftrukt.artnr
- **Lager:** Nummer des Lagers, aus dem der Artikel entnommen wird.
  - Technische Info: Anzeigefeld, DB-Feld: bpos.nr
- **Variante:** Variante des Lagerartikels aus dem Artikelstamm.
  - Technische Info: Anzeigefeld, DB-Feld: artvarzu.bitnr
- **Anzahl:** Menge in der Artikelmengeneinheit, die für die Position benötigt werden.
  - Technische Info: Anzeigefeld
- **Verbucht:** Stückzahl der Lagerartikel, die verbucht sind.
  - Technische Info: Anzeigefeld
- **Status:** Lagerstatus:
  - Noch keine Buchung
  - Teil-Buchung
  - Gebucht
  - Technische Info: Anzeigefeld, DB-Feld: kposstat.status

#### Fußbereich

Zusätzliche Artikel-Informationen zur ausgewählten Position.
Die Schaltflächen sind zum Register Positionen beschrieben:
⇨ "Vorgangsinformationen – Positionen" auf Seite D-1432

### Vorgangsinformationen – Verbundene Prod.

**Navigation:** `Verkauf > Übersicht > Auftragsinformation > Auftragsnummer angeben > Register Verbundene Prod.`

*Abb. D-173 Auftragsinformationen – Register Verbundene Prod.*

In diesem Register werden die Status-Informationen aus der verbundenen Produktion angezeigt, wenn Sie mit interner Mandantentrennung arbeiten.
Für weitere Informationen zu diesem Bereich kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

#### Register Verbundene Produktion

Das Register ist genauso aufgebaut wie das Register Produktion:
⇨ "Vorgangsinformationen - Produktion" auf Seite D-1436

#### Fußbereich

Die Bezeichnung des Artikels zur ausgewählten Position wird im Dialog unten links angezeigt.
Die Schaltflächen sind zum Register Positionen beschrieben:
⇨ "Vorgangsinformationen - Positionen" auf Seite D-1432

### Vorgangsinformationen – Zwischenversand

**Navigation:** `Verkauf > Übersicht > Auftragsinformation > Auftragsnummer angeben > Register Zwischenversand`

*Abb. D-174 Auftragsinformationen – Register Zwischenversand*

In diesem Register werden die Informationen zum Status des Versands von Artikeln aus der verlängerten Werkbank angezeigt.

#### Register Zwischenversand

Das Register ist genauso aufgebaut wie das Register Produktion:
⇨ "Vorgangsinformationen - Produktion" auf Seite D-1436

## Recherche zu Vorgängen

Um Vorgänge zu suchen, steht Ihnen eine Suche mit umfangreichen Suchkriterien zur Verfügung.
In diesem Abschnitt sind folgende Dialoge erklärt:
- "Vorgangs-Recherche" auf Seite D-1445
- "Positionen" auf Seite D-1457

### Vorgangs-Recherche

**Navigation:** `Verkauf > Übersicht > Vorgangs-Recherche`

In diesem Dialog suchen Sie nach Vorgängen. Die Ergebnisse werden in einer Trefferliste angezeigt.

In diesem Dialog finden Sie folgende Register:
- "Vorgangs-Recherche – Suchmodus" auf Seite D-1445
- "Vorgangs-Recherche – Übersicht" auf Seite D-1449
- "Vorgangs-Recherche – Mitarbeiter" auf Seite D-1451
- "Vorgangs-Recherche – Details" auf Seite D-1452
- "Vorgangsänderungs-Protokoll" auf Seite D-1455

Diesen Dialog können Sie auch über das Infomenü mit `<Shift> + <F4>` im Kopfbereich der Auftragserfassung öffnen.

### Vorgangs-Recherche – Suchmodus

**Navigation:** `Verkauf > Übersicht > Vorgangs-Recherche`

*Abb. D-175 Vorgangs-Recherche – Suchmodus*

In diesem Dialog schränken Sie die Suche mit den vorgegebenen Kriterien ein. Die Kriterien legen Sie mit Bedingungen fest. Je mehr Kriterien Sie für die Suche angeben, desto mehr schränken Sie die Suche ein.
Mit `<Shift> + <F8>` oder `<Shift> + <F12>` ändern Sie die Bedingung. In der Infozeile wird die Bedeutung der ausgewählten Bedingung angezeigt.

| Bedingung | Bedeutung |
| :--- | :--- |
| **=** | Suche nach genau diesem Wert (z. B. Feld `Marktpartner = 600004` listet nur Vorgänge zu diesem Marktpartner auf). |
| **>** | Suche nach größeren Werten (z. B. Feld `Marktpartner > 600004` listet nur Vorgänge mit Marktpartnernummern größer als 600004 auf). |
| **m** | Suche nach Muster in Textfeldern (z. B. Feld `Modell 12` listet alle Vorgänge mit dem Kommissionstext `Modell 12` auf.) |
| **0** | Suche nach Werten = 0 (z. B. Feld `Marktpartner 0` listet den Marktpartner mit der Nummer 0 auf). |
| **z** | Suche alle Werte im Bereich. |
| **!** | Suche alles außer diesem Wert (z. B. Feld `Abteilung ! 10` listet alle Abteilungen außer der Abteilung mit der Nummer 10 auf). |
| **<** | Suche nach kleineren Werten (z. B. Feld `Marktpartner < 600004` listet nur Vorgänge mit Marktpartnernummern kleiner als 600004 auf). |

*Tab. D-13 Bedeutung der Filterbedingungen*

- **Hausnummer** • Mandantennummer (Hausnummer) und Bezeichnung des Hauses. Wenn Sie eine Nummer angeben, wird die Bezeichnung des Hauses im Klartext angezeigt.
  - Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: kauf.hausnr
- **Firma** Nummer der Firma oder Gesellschaft, die dem Haus zugeordnet ist. Das Feld ist nur freigeschaltet, wenn Sie mit interner Mandantentrennung arbeiten.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.company
- **Vorgang** Vorgangsart. Wenn Sie eine Vorgangsart auswählen, wird die Schlüsselnummer der Vorgangsart im Klartext angezeigt.
  - Anfragen
  - Bestellungen
  - Wareneing.
  - Angebote
  - Aufträge
  - Lieferscheine
  - Rechnungen
  - EK-Rechng.
  - Gutschriften
  - EK-Gutschr.
  - VK-Stornos (Verkaufsvorgänge, die storniert wurden)
  - EK-Stornos (Einkaufsvorgänge, die storniert wurden)
  - Änderungen (Vorgänge, die geändert wurden)
  Der Dialog Vorgangsänderungs-Protokoll wird geöffnet.
  ⇨ "Vorgangsänderungs-Protokoll" auf Seite D-1455
- **Technische Info:** Toggle-Feld, Anzeigefeld, DB-Felder: kauf.vorgang
- **Belegdatum** Erfassungsdatum des Vorgangs im Format TT.MM.JJJJ.
  - Technische Info: Datumsfeld, DB-Feld: kauf.edat
- **Marktpartner** Marktpartnernummer und -bezeichnung. Wenn Sie eine Nummer angeben, wird die Bezeichnung des Marktpartners im Klartext angezeigt. Der Matchcode des Martpartners wird einem Marktpartnertyp zugeordnet.
  - Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: kauf.kunr, mp.name
- **(Matchcode)** Marktpartnertyp. Im Verkauf ist Kunde als Marktpartnertyp voreingestellt. Wenn Sie einen Marktpartner wählen, wird der Matchcode des Marktpartners automatisch vor dem Feld angezeigt.
  - Technische Info: Toggle-Feld, DB-Feld: mp.mpmc
- **Knd-Bestnr** Kunden-Bestellnummer.
  - Technische Info: alphanumerisches Feld, DB-Feld: kauf.exaufnr
- **Kommission** Kommissionstext.
  - Technische Info: alphanumerisches Feld, DB-Feld: komm.kommtxt
- **Objekt** Objektnummer und Bezeichung des Objekts, z. B. Baustelle. Wenn Sie eine Nummer angeben, wird die Bezeichnung des Objekts im Klartext angezeigt.
  - Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: kauf.objnr, mp.name
- **Nummer** Vorgangsnummer.
  - Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr
- **Subnr** Subnummer, z. B. Teil-Lieferschein.
  - Technische Info: numerisches Feld, DB-Feld: kauf.subnr
- **Abteilung** Nummer und Name der Abteilung des Vorgangserfassers. Wenn Sie eine Nummer angeben, wird der Name der Abteilung im Klartext angezeigt.
  - Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: kauf.abtnr
- **Rechnung** Rechnungsnummer. Die Nummer wird in der Datenbanktabelle vorgang mit dem Wert 7 gespeichert.
  - Technische Info: numerisches Feld, DB-Feld: kauf.auftrnr
- **Vertreter** Nummer und Name des Vertreters. Wenn Sie eine Nummer angeben, wird der Name des Vertreters im Klartext angezeigt.
  - Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: kauf.vertrerloe
- **Bestellt** Bestelldatum im Format TT.MM.JJJJ.
  - Technische Info: Datumsfeld, DB-Feld: kauf.bdat
- **Route** Nummer und Bezeichnung der Route. Wenn Sie eine Nummer angeben, wird die Bezeichnung der Route im Klartext angezeigt.
  - Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: kauf.routenr
- **Liefertermin** Geplanter Liefertermin im Format TT.MM.JJJJ.
  - Technische Info: Datumsfeld, DB-Feld: kauf.ltplan
- **Erfasst** Nummer und Name des Vorgangserfassers. Wenn Sie eine Nummer angeben, wird der Name des Erfassers im Klartext angezeigt.
  - Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: kauf.eusr, mitarb.maname
- **Stillgelegt** Anzeige, ob der Vorgang storniert ist. Das Kennzeichen und die Schlüsselnummer werden automatisch gesetzt, wenn Sie einen Vorgang auswählen.
  - **n:** Der Vorgang ist nicht storniert. Die Schlüsselnummer 0 wird angezeigt. Das Feld ist standardmäßig mit dem Kennzeichen n vorbelegt.
  - **j:** Der Vorgang ist storniert. Die Schlüsselnummer 1 wird angezeigt. Das Kennzeichen wird gesetzt, wenn Sie im Feld Vorgang die Vorgangsart VK-Stornos oder EK-Stornos gewählt haben.
  - Technische Info: Toggle-Feld, Anzeigefeld, DB-Felder: kauf.storno

#### Fußbereich
- **Start**: Suche nach Vorgängen mit den angegebenen Kriterien starten.

### Vorgangs-Recherche – Übersicht

**Navigation:** `Verkauf > Übersicht > Vorgangs-Recherche > Suchkriterien eingeben > <F3> > Register Übersicht`

*Abb. D-176 Vorgangs-Recherche – Übersicht*

In diesem Register werden die Trefferliste der Vorgänge angezeigt, die den Suchkriterien entsprechen.

#### Kopfbereich

Die Felder im Kopfbereich dienen nur der Information. Sie können die Einträge nicht bearbeiten.

- **Marktpartner** Nummer, Matchcode und Name des Marktpartners.
  - Technische Info: Anzeigefelder, DB-Felder: mp.kuliflag, mp.mpnr, mp.mpmc
- **Anschrift** Straße und Hausnummer des Marktpartners.
  - Technische Info: Anzeigefeld, DB-Feld: mp.str
- **PLZ, Ort** Postleitzahl und Ort des Marktpartners.
  - Technische Info: Anzeigefelder, DB-Felder: mp.plz, mp.ort
- **Telefon** Telefonnummer des Marktpartners.
  - Technische Info: Anzeigefeld, DB-Feld: mp.telefon
- **Fax** Faxnummer des Marktpartners.
  - Technische Info: Anzeigefeld, DB-Feld: mp.faxnr
- **Bewertung** Nummer der Bewertung der Qualität des Marktpartners. Die Bewertung wird in den Marktpartnerstammdaten angelegt.
  - Technische Info: Anzeigefeld, DB-Feld: mp.qqual
> **Bewertung in den Stammdaten anlegen**
> Die Bewertung legen Sie unter folgendem Pfad an: `Stammdaten > Marktpartner > Marktpartner auswählen > Register Bewertung > Feld Qualität`.

#### Register Übersicht
- **Vorgang:** Vorgangsnummer.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.auftrnr
- **Subnr:** Nummer des Teil-Lieferscheins oder der Teil-Rechnung.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.subnr
- **Haus:** Mandantennummer (Hausnummer).
  - Technische Info: Anzeigefeld, DB-Feld: kauf.hausnr
- **Art:** Art des Vorgangs, z. B. Auftrag.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.vorgang
- **Lieferdat:** Lieferdatum.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.ltplan
- **Rabatt:** Vom Gesamtbetrag gewährter Rabatt in Prozent.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.gesfaktor
- **Nachlass:** Vom Gesamtbetrag gewährter Nachlass in Prozent.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.gesfaktor
- **Netto:** Netto-Endbetrag der Position.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.nettototal
- **Spanne:** Gewinnspanne der Position in Währungseinheiten.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.dbdm
- **%:** Gewinnspanne der Position in Prozent.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.dbvh

#### Fußzeile
Für die Werte Netto und Spanne sind die Summen der Werte aller Positionen aufgelistet. Für % (Preisspanne) ist der Durchschnittswert aller Positionen aufgelistet.

### Vorgangs-Recherche – Mitarbeiter

**Navigation:** `Verkauf > Übersicht > Vorgangs-Recherche > Suchkriterien eingeben > <F3> > Register Mitarbeiter`

*Abb. D-177 Vorgangs-Recherche – Mitarbeiter*

In diesem Register werden die Mitarbeiterinformationen zu den Vorgängen des Mitarbeiters angezeigt.

#### Kopfbereich

Die Felder sind zum Register Übersicht beschrieben:
⇨ "Vorgangs-Recherche – Übersicht" auf Seite D-1449

#### Register Mitarbeiter

Einige Spalten sind zum Register Übersicht beschrieben:
⇨ "Vorgangs-Recherche – Übersicht" auf Seite D-1449

Zusätzlich werden folgende Spalten angezeigt:
- **Hausnr.:** Mandantennummer (Hausnummer).
  - Technische Info: Anzeigefeld, DB-Feld: kauf.hausnr
- **Marktpart.:** Nummer des Marktpartners.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.kunr
- **Erfasst:** Datum der Vorgangs-Erfassung.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.edat
- **Vertreter:** Nummer des Vertreters.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.vertrerloe
- **Sachbearb.:** Name des Sachbearbeiters.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.abvertr
- **Route, Routenname:** Nummer und Bezeichnung der Versand-Route.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.routenr

### Vorgangs-Recherche – Details

**Navigation:** `Verkauf > Übersicht > Vorgangs-Recherche > Suchkriterien eingeben > <F3> > Register Details`

*Abb. D-178 Vorgangs-Recherche – Details*

In diesem Register werden die Details zu dem gewählten Vorgang angezeigt. Mit `<Bild runter>` wechseln Sie zum nächsten Vorgang, mit `<Bild hoch>` zum vorherigen Vorgang.

#### Kopfbereich

Die Felder sind zum Register Übersicht beschrieben:
⇨ "Vorgangs-Recherche – Übersicht" auf Seite D-1449

#### Register Details

- **Vorgang** Nummer und Sub-Nummer des Vorgangs.
  - Technische Info: numerisches Feld, Anzeigefeld, DB-Felder: kauf.auftrnr, kauf.subnr
- **Org. Vorgang** Nummer des Original-Vorgangs bei übertragenen Vorgängen. Im ersten Feld steht die Mandantennummer (Hausnummer) des Absenders, im zweiten Feld die originale Vorgangs-Nummer.
  - Technische Info: Anzeigefelder, DB-Felder: kauf._orgauftrnr
- **Vor. Vorgang** Vorherige Vorgangs-Nummer bei übertragenen Vorgängen, z. B. die Bezugs-Nummer zum Original-Vorgang.
  - Technische Info: Anzeigefelder, DB-Feld: kauf.referenz
- **Marktpartner** Nummer und Name des Marktpartners.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.kunr, mp.name
- **Liefertermin** Lieferdatum.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.ltplan
- **Rechnung** Rechnungsnummer des Vorgangs.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.rechnr
- **Knd-Bestnr** Externe Bestellnummer vom Kunden. Bei Aufträgen aus einem anderen Haus wird in diesem Feld die Auftragsnummer des sendenden Hauses angezeigt.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.exaufnr
- **Bestelldatum** Datum der Bestellung.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.edat
- **Objekt** Nummer und Bezeichnung des Objekts. Ein Objekt kann z. B. eine Baustelle oder Lieferadresse sein.
  - Technische Info: Anzeigefelder, DB-Felder: kauf.objnr, kauf.orgname
- **Abteilung** Nummer und Bezeichnung der Abteilung, in der der Vorgang erfasst wurde.
  - Technische Info: Anzeigefelder, DB-Feld: kauf.abtnr
- **Gesamt-Qm.** Gesamt-Glasfläche des Vorgangs in Quadratmeter.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.gesm2
- **Gesamtstück** Gesamtstückzahl der Artikel aus allen Positionen des Vorgangs.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.gesst
- **Rabatt** Auf den Gesamtbetrag gewährter Rabatt in Prozent und als Betrag.
  - Technische Info: Anzeigefelder, DB-Felder: kauf.gesfaktor
- **Nettototal** Summe aller Positionspreise, abzüglich der Rabatte und zuzüglich der Zuschläge.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.nettototal
- **Spanne** Gewinnspanne des Vorgangs in Prozent und in Währungseinheiten.
  - Technische Info: Anzeigefelder, DB-Felder: kauf.dbvh, kauf.dbdm
- **Zahlziel** Zahlungsziel und Skontoabzüge, die mit dem Marktpartner vereinbart sind.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.zahlziel
- **Valuta** Frist bis zur Wertstellung in Tagen.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.valuta
- **Skonto 1, 2, %** Zeitraum in Tagen, in dem Skonto gewährt wird. Im zweiten Feld (%) steht der Skontosatz. Die Felder sind mit den Daten aus dem Marktpartnerstamm vorbelegt.
  - Technische Info: Anzeigefelder, DB-Felder: kauf._skonto1, kauf.skvh1, kauf._skonto2, kauf.skvh2
- **Erfasst am, von** Datum der Vorgangs-Erfassung, Nummer und Name des Erfassers.
  - Technische Info: Anzeigefelder, DB-Felder: kauf.edat, kauf.eusr
- **Eingang** Art des Kommunikation der Vorgangserfassung, z. B. Fax.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.eingang
  - ⇨ "Eingang" auf Seite D-1138

### Vorgangsänderungs-Protokoll

**Navigation:** `Verkauf > Übersicht > Vorgangs-Recherche > Feld Vorgang > Wert Änderung als Suchkriterium festlegen > <Enter>`

*Abb. D-179 Vorgangs-Recherche – Vorgangsänderungs-Protokoll*

In diesem Dialog wird ein Protokoll zu Vorgangsänderungen angezeigt.

> **Automatische Anzeige des Dialogs**
> Der Dialog Vorgangsänderungs -Protokoll wird automatisch angezeigt, wenn sie in der Vorgangsrecherche im Feld Vorgang als Suchkriterium Änderung festlegen und in das nächste Feld wechseln.

Sie können die Anzeige der Vorgangsänderungen nach Datum und Vorgangsart eingrenzen. Nach Eingabe der Suchkriterien, wird das Protokoll in einer Ansicht angezeigt.
Mit `<Enter>` wird das Protokoll der Vorgangsänderungen angezeigt.

#### Protokollsuche

**Vorgang** Art des Vorgangs.
- Alle
- Anfragen
- Bestellungen
- Wareneingänge
- Angebote
- Aufträge
- Lieferscheine
- Rechnungen
- EK-Rechn.
- Gutschriften
- EK-Gutschr.
  - Technische Info: Toggle-Feld, DB-Feld: kauf.vorgang

**von Datum** Anzeige von Vorgangsänderungen ab diesem Datum. Das Format ist TT.MM.JJJJ. Standardmäßig ist das aktuelle Datum voreingestellt.
Technische Info: Datumsfeld

**bis Datum** Anzeige von Vorgangsänderungen bis zu diesem Datum. Das Format ist TT.MM.JJJJ. Standardmäßig ist das aktuelle Datum voreingestellt.
Technische Info: Datumsfeld

#### Protokollanzeige

In der Ansicht wird Ihnen ein Protokoll der Vorgangsänderungen angezeigt, die den Suchkriterien entsprechen. Das Protokoll kann nicht bearbeitet werden.
- **Vorgang:** Vorgangsnummer.
  - Technische Info: Anzeigefeld, DB-Feld: kaufedit.auftrnr
- **(Spalte ohne Benennung):** Sub-Nummer des Vorgangs.
  - Technische Info: Anzeigefeld, DB-Feld: kaufedit.subnr
- **Vorg:** Vorgangsart.
  - Technische Info: Anzeigefeld, DB-Feld: kaufedit.vorgang
- **Änderung:** Datum, an dem der Vorgang geändert wurde.
  - Technische Info: Anzeigefeld, DB-Feld: kaufedit.datum
- **Zeit:** Uhrzeit, zu der der Vorgang geändert wurde.
  - Technische Info: Anzeigefeld, DB-Feld: kaufedit.zeit
- **Änderungsart:** Art der Änderung.
  - Technische Info: Anzeigefeld, DB-Feld: kaufedit.modus
- **Mitarb:** Nummer des Mitarbeiters, der den Vorgang geändert hat.
  - Technische Info: Anzeigefeld, DB-Feld: kaufedit.manr
- **Name:** Name des Mitarbeiters, der den Vorgang geändert hat.
  - Technische Info: Anzeigefeld, DB-Feld: mitarb.maname

### Positionen

**Navigation:** `Verkauf > Übersicht > Vorgangs-Recherche > Suchkriterium eingeben > <F3> > Vorgang auswählen > <Shift> + <F9>`

In diesem Dialog werden Ihnen die Informationen zu den Positionen des ausgewählten Vorgangs angezeigt.

In diesem Dialog finden Sie folgende Register:
- "Positionen - Übersicht" auf Seite D-1457
- "Positionen - Details" auf Seite D-1459

### Positionen – Übersicht

**Navigation:** `Verkauf > Übersicht > Vorgangs-Recherche > Suchkriterium eingeben > [Start] > Register auswählen > Vorgang auswählen > <Shift> + <F9> > Register Übersicht`

*Abb. D-180 Positionen – Übersicht*

In diesem Register werden die Positionen des Vorgangs angezeigt.

- **Position:** Positionsnummer.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.posnr
- **Artikel:** Artikelnummer.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.artnr
- **(Spalte ohne Bezeichnung):** Artikelbezeichnung.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.artbez1
- **Menge:** Einheiten der Position.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.geliefert
- **Nettostp.:** Netto-Stückpreis der Position.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.nstpreis
- **Spanne:** Spanne zwischen VK-Preis und EK-Preis.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.spanne
- **Änd:** Kennzeichen, ob die Position geändert wurde.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.poskoaendkz
- **Materialkosten:** Materialkosten der Position aus den Stammdaten, wenn mit der Kostenkalkulation gearbeitet wird. Materialkosten können z. B. Einkaufspreise oder der Materialwert inklusive Verschnitt bei Lagerentnahme sein.
  - Technische Info: Anzeigefeld, DB-Feld: kposp.komat
- **Lohnkosten:** Lohnkosten für die Produktion / Bearbeitung der Position. Wird in A+W Production berechnet und zurückgemeldet.
  - Technische Info: Anzeigefeld, DB-Feld: kposp.kolohn
- **Maschinenko.:** Maschinenkosten für die Produktion / Bearbeitung der Position. Wird in A+W Production berechnet und zurückgemeldet.
  - Technische Info: Anzeigefeld, DB-Feld: kposp.kobm

#### Fußzeile

In der Fußzeile werden Art und Nummer des gewählten Vorgangs angezeigt.

### Positionen – Details

**Navigation:** `Verkauf > Übersicht > Vorgangs-Recherche > Suchkriterium eingeben > [Start] > Register auswählen > Vorgang auswählen > <Shift> + <F9> > Register Details`

*Abb. D-181 Positionen – Details*

In diesem Register werden die Details zu den Positionen des Vorgangs angezeigt.

- **Position** Nummer der Position.
  - Technische Info: numerisches Feld, DB-Feld: kpos.lfdpos
- **Artikel** Nummer und Bezeichnung des Artikels.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.artnr
- **Modell** Modellnummer des Artikels.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.modnr
- **Warengruppe** Kennzeichen der Warengruppe, die dem Artikel zugewiesen ist.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.wagrp
- **Lieferant** Lieferantennummer.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.liefnr
- **Menge** Positionsmenge.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.menge
- **Maße** Breite, Höhe und Scheibenzwischenraum dieser Position in Millimeter und die Gesamt-Fläche in Quadratmeter.
  - Technische Info: Anzeigefelder, DB-Felder: kpos.laenge, kpos.breite, kpos.szr, kpos.qm

#### VK-Preis, EK-Preis

- **Netto** Netto-Endbetrag der Position.
  - Technische Info: Anzeigefelder, DB-Felder: kpos.nstpreis, kpos.eknstpreis
- **Brutto** Brutto-Betrag der Position.
  - Technische Info: Anzeigefelder, DB-Felder: kpos.bstpreis, kpos.ekbstpreis
- **Faktor** Berechnungs-Faktor der Position.
  - Technische Info: Anzeigefelder, DB-Felder: kpos.vorvkfaktor, kpos.ekfaktor
- **PKZ** Preiskennzeichen aus der Preisliste.
  - Technische Info: Anzeigefelder, DB-Felder: kpos.vorvkpkz. kpos.ekpkz
- **Rabatt** Preis-Rabatt der Position in Prozent. Das Feld wird nur für den Verkaufspreis angezeigt.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.rabatt
- **Nachlass** Nachlass der Position in Prozent. Das Feld wird nur für den Verkaufspreis angezeigt.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.gesfaktor

#### Kosten

- **Materialkosten** Materialkosten der Position, z. B. Materialwert mit Verschnitt.
  - Technische Info: Anzeigefeld, DB-Feld: kposp.komat
- **Lohnkosten** Lohnkosten der Position.
  - Technische Info: Anzeigefeld, DB-Feld: kposp.kolohn
- **Maschinenko.** Maschinenkosten, errechnet aus Laufzeit und Kostensatz des Betriebsmittels.
  - Technische Info: Anzeigefeld, DB-Feld: kposp.kobm
- **Erlös** Geldwert des Umsatzes.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.erloes
- **Spanne** Spanne zwischen VK-Preis und EK-Preis.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.spanne

#### Fußzeile

In der Fußzeile werden Art und Nummer des gewählten Vorgangs angezeigt.

## Übersichten zu Vorgängen

Um sich zu dem Stand der Vorgänge zu informieren, stehen Ihnen diverse Dialoge zur Verfügung. In den Dialogen werden Ihnen Übersichten von Daten angezeigt, die aus den Vorgängen ermittelt werden.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Auftragsanzeige" auf Seite D-1461
- "Angebotsanzeige" auf Seite D-1462
- "Wiedervorlage" auf Seite D-1463
- "Vorgangsänderung" auf Seite D-1466
- "Übersicht zu Vorgängen" auf Seite D-1471

### Auftragsanzeige

**Navigation:** `Verkauf > Übersicht > Auftragsanzeige`

*Abb. D-182 Auftragsanzeige*

In diesem Dialog öffnen Sie einen Auftrag im Anzeigemodus. Sie können eine Auftrag jederzeit im Anzeigemodus öffnen, z. B. auch dann, wenn der Auftrag durch einen Hintergrundprozess gesperrt ist oder von einem anderen Benutzer bearbeitet wird.
Die Daten im Dialog **Auftragsanzeige** dienen nur der Information. Sie können nicht alle Auftragsfunktionen aufrufen und die Einträge nicht bearbeiten.

Die Register und Felder sind zum Dialog Auftragserfassung beschrieben:
⇨ "Auftragserfassung" auf Seite D-1134

### Angebotsanzeige

**Navigation:** `Verkauf > Übersicht > Angebotsanzeige`

*Abb. D-183 Angebotsanzeige*

In diesem Dialog öffnen Sie ein Angebot im Anzeigemodus. Sie können ein Angebot jederzeit im Anzeigemodus öffnen, z. B. auch dann, wenn das Angebot durch einen Hintergrundprozess gesperrt ist oder von einem anderen Benutzer bearbeitet wird.

Die Daten im Dialog **Angebotsanzeige** dienen nur der Information. Sie können nicht alle Angebotsfunktionen aufrufen und die Einträge nicht bearbeiten.

Die Register und Felder sind zum Dialog Auftragserfassung beschrieben:
⇨ "Auftragserfassung" auf Seite D-1134

### Wiedervorlage

**Navigation:**
- `Verkauf > Wiedervorlagen`
- `Verkauf > Vorgangserfassung > Kopf-, Fußbereich, Positionsebene > <F4> > Wiedervorlage`

*Abb. D-184 Wiedervorlage*

In diesem Dialog legen Sie Bearbeitungsvermerke für die Wiedervorlage an. Wenn der Wiedervorlage-Termin erreicht ist, bekommt der gewählte Mitarbeiter beim Programmstart eine Pop-up-Nachricht angezeigt oder eine Erinnerungs-Mail zugestellt.

Sie können vorgangsfreie Wiedervorlagen erstellen, die keinen Bezug zu einem Vorgang haben.
Vorgangsbezogene Wiedervorlagen können Sie nur erstellen, wenn Sie ein Angebot mit Liefertermin erfassen. Diese Wiedervorlagen stehen immer in Bezug zu einem kaufmännischen Vorgang.

- Mit `<F6>` legen Sie weitere Wiedervorlagen an.
- Mit `<F7>` löschen Sie einzelne Wiedervorlagen.
- Mit `<Ende>` speichern Sie Wiedervorlagen und schließen den Dialog.

**Vorl-Datum** Vorlage-Datum, an dem an den Vorgang erinnert wird. Je nach Systemkonfiguration kann die Wiedervorlage auch automatisch angezeigt werden oder wenn bestimmte Bedingungen erfüllt werden.
Technische Info: Pflichtfeld, Datumsfeld, DB-Feld: vorlage.vldat

**Vorlageart:** Art der Wiedervorlage.
- **Mitteilung in Meldesystem:** Die Nachrichten werden dem Anwender über das Nachrichtensystem übermittelt. Mit `<Strg> + <F4>` können Sie die Nachrichten im Mail-System abrufen. Wenn Sie mit einem externen Mail-Programm arbeiten, kann das System auch so konfiguriert werden, dass Sie die Mails auch über das entsprechende Programm abrufen können. Falls eine E-Mail-Adresse hinterlegt ist, wird dem Nachrichtenempfänger eine externe E-Mail zugesendet.
- **Aktive Wiedervorlage:** Alle Nachrichten werden beim Starten des Programms auf dem Bildschirm angezeigt.
- **direktes Löschen des Vorgangs:** Die Funktion ist nur zulässig bei Kundenangeboten und Lieferantenanfragen. Damit wird die Wiedervorlage für den Vorgang beim Erreichen des Vorlagedatums storniert.
  - Technische Info: Toggle-Feld, DB-Feld: vorlage.modus

**Vorlage an Mitarbeiter** Nummer des Mitarbeiters, der die Wiedervorlage erhält. Standardmäßig ist der Vorgangserfasser voreingestellt. Wenn Sie eine Nummer angeben, wird der Name des Mitarbeiters im Klartext angezeigt.
Technische Info: numerisches Feld, DB-Feld: vorlage.outmanr

**Textfelder** Felder für Informationstexte zum Vorgang, die zum Wiedervorlagezeitpunkt angezeigt werden. Wenn Sie eine vorgangsbezogene Wiedervorlage erfassen, wird vor dem ersten Textfeld die Nummer des Angebots angezeigt.
Technische Info: alphanumerische Felder, DB-Felder: vorlage.text1, vorlage.text2

### Fertigmeldung

**Navigation:** `Verkauf > Fertigmeldung`

*Abb. D-185 Fertigmeldung*

In diesem Dialog können Sie Positionen zu einem Auftrag fertig melden.
In der Regel werden Fertigmeldungen aus der Produktion oder aus dem Einkauf gemeldet und müssen nicht manuell übermittelt werden.
- Mit `<F5>` löschen Sie die Positionen, deren gesamte Positionsmenge bereits fertig gemeldet ist. Bei den Positionen ist das Feld **Fertig** leer.
- Mit `<F3>` buchen Sie die Fertigmeldung.

#### Kopfbereich

- **Haus** Anzeige der Mandantennummer (Hausnummer).
  - Technische Info: Anzeigefeld, DB-Feld: kauf.hausnr
- **Auftrag** Auftragsnummer.
  - Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kauf.auftrnr
- **Abteilg** Nummer der Abteilung des Auftrag-Erfassers.
  - Technische Info: numerisches Feld, DB-Feld: kauf.abtnr
- **Liefertermin** Geplanter Liefertermin des Auftrags.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.ltplan
- **Fertigmeldung** Datum im Format TT.MM.JJJJ, an dem der Auftrag fertig gemeldet werden soll. Standardmäßig ist das aktuelle Datum voreingestellt.
  - Technische Info: Pflichtfeld, Datumsfeld, DB-Feld: kauf.bdat

#### Übersicht

- **Auftrag:** Auftragsnummer.
  - Technische Info: Anzeigefeld, DB-Feld: kauf.auftrnr
- **Pos:** Positionsnummer im Auftrag.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.posnr
- **Artikel:** Bezeichnung des Artikels aus der gewählten Position.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.artnr, kpos.artbez1
- **Gesamt:** Gesamtmenge der Position.
  - Technische Info: Anzeigefeld, DB-Feld: kpos.menge
- **Bisher:** Bisher fertig gemeldete Menge der Position.
  - Technische Info: Anzeigefeld, DB-Feld:
- **Fertig:** Menge der Position, die fertig gemeldet werden soll. Standardmäßig ist hier die Differenz aus der Gesamtmenge der Position und der bisher fertig gemeldeten Menge festgelegt. Sie können die Menge, die fertig gemeldet werden soll, bearbeiten.
  - Technische Info: numerisches Feld, DB-Feld:

#### Fußbereich

- **Buchen:** Bucht die Fertigmeldung.
- **Abbrechen:** Bricht die Fertigmeldung ab.

### Vorgangsänderung

**Navigation:** `Verkauf > Vorgangsänderung`

*Abb. D-186 Vorgangsänderung*

In diesem Dialog können Sie mehrere Vorgänge gleichzeitig korrigieren. Die Vorgänge können schneller korrigiert werden als in anderen Dialogen, da keine Zeit für das Laden eines gesamten Vorgangs benötigt wird. Korrekturen an Vorgängen können Sie nicht jederzeit durchführen, sie sind abhängig vom Positionsstatus.
"Positionsstatus und Positionskennzeichen" auf Seite D-1128

Der Dialog ist in drei Register aufgeteilt, in der diverse Felder angezeigt werden.

- Mit `<F2>` wechseln Sie zwischen den Register im Dialog.
- Mit rechten Maustaste rufen Sie den Kontextmenü auf.
- Mit `<Strg> + <F10>` suchen Sie nach Vorgängen mit Leistungserklärungen zu einem Liefertermin. Es werden alle Vorgänge mit Leistungserklärungen für den gesuchten Liefertermin angezeigt.
- Mit `<Strg> + <F11>` werden alle Sätze, ab dem aktuellen markiert.
- Mit `<Strg> + <F8>` importieren Sie die Daten für die Vorgangsänderung. Die Daten werden über eine frei konfigurierbare SQL-Abfrage importiert. Die Anzahl der importierten Daten ist von der jeweiligen SQL-Abfrage abhängig.
- Mit `<F5>` wird die Zusatzinformation zum Vorgang angezeigt, wenn eine hinterlegt ist.
- Mit `<F3>` lösen Sie die Buchung der Korrekturen aus.
- Mit `<Shift> + <F5>` wechseln Sie in die Auftragserfassung.
  ⇨ "Auftragserfassung" auf Seite D-1134

#### Register Allgemein

- **Vorgang:** Art des Vorgangs.
  - Auftrag
  - Lief: Lieferung
  - Angeb: Angebot
  - Technische Info: Toggle-Feld, DB-Feld: zuaufint.vorgang
- **Nummer:** Vorgangsnummer.
  - Technische Info: numerisches Feld, DB-Feld: zuaufint.auftrnr
- **Subnr.:** Sub-Nummer des Vorgangs.
  - Technische Info: Anzeigefeld, DB-Feld: zuaufint.subr
- **Info:** Anzeige, ob es Zusatzinformationen zu dem Vorgang gibt.
  - **(leer):** Es gibt keine Zusatzinformationen.
  - **/:** Es gibt Zusatzinformationen.
  - Technische Info: Anzeigefeld, Toggle-Feld
- **Lokale Korrekt.:** Information, ob sich der Vorgang im Status der lokalen Korrektur befindet. Der Hinweis wird nur angezeigt, wenn sich der Vorgang in diesem Status befindet. Das Feld ist gesperrt.
  - Technische Info: Anzeigefeld, DB-Feld:
- **Sto.:** Stornierung. Angabe, ob der Vorgang storniert werden soll.
  - ☑ Der Vorgang wird storniert.
  - ☐ Der Vorgang wird nicht storniert.
  - Technische Info: Checkbox, DB-Feld: zuaufint.storno
- **Haus:** Mandantennummer (Hausnummer), die dem Vorgang zugeordnet ist.
  - Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: zuaufint.hnr
- **Route:** Nummer der Versandroute.
  - Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: zuaufint.route
- **Termin:** Datum der geplanten Lieferung im Format TT.MM.JJJJ.
  - Technische Info: Datumsfeld, DB-Feld: zuaufint.ltideal
- **PMS:** Angabe, ob der Vorgang an das Produktions-Management-System übergeben werden soll. Die Angabe ist nur gültig, wenn das Produktions-Management-System genutzt wird.
  - ☑ Der Vorgang wird an das Produktions-Management-System übergeben.
  - ☐ Der Vorgang wird nicht übergeben.
  - Technische Info: Checkbox, DB-Feld: zuaufint.pmsflag
- **Vrs.:** Versandsteuerung. Angabe, ob der Vorgang an die Versandsteuerung übergeben werden soll.
  - ☑ Der Vorgang wird an die Versandsteuerung übergeben.
  - ☐ Der Vorgang wird nicht übergeben.
  - Technische Info: Checkbox, DB-Feld: zuaufint.lapoolflag
- **Txt.:** Angabe, ob die Texte für den Vorgang neu generiert werden sollen.
  - ☑ Die Texte werden vom System neu generiert.
  - ☐ Die Texte werden vom System nicht neu generiert.
  - Technische Info: Checkbox, DB-Feld: zuaufint.txtflag
- **WGR:** Angabe, ob die Warengruppenzuordnung für den Vorgang erneut erstellt werden soll.
  - ☑ Die Zuordnung wird für den Vorgang aktualisiert.
  - ☐ Die Zuordnung für den Vorgang wird nicht aktualisiert.
  - Technische Info: Checkbox, DB-Feld: zuaufint.wgrpflag
- **Frei:** Angabe, ob der Vorgang freigeschaltet werden soll.
  - ☑ Der Vorgang wird freigeschaltet.
  - ☐ Der Vorgang wird nicht freigeschaltet.
  - Technische Info: Checkbox, DB-Feld: kauf.tekapkz

Mit `<F2>` wechseln Sie in den Register **Versand**. Hier werden folgende Felder angezeigt:
- **Vorgang:** Art des Vorgangs.
  - Auftrag
  - Lief: Lieferung
  - Angeb: Angebot
  - Technische Info: Toggle-Feld, DB-Feld: zuaufint.vorgang
- **Auftrag:** Vorgangsnummer.
  - Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: zuaufint.auftrnr
- **Subnr.:** Sub-Nummer des Vorgangs.
  - Technische Info: Anzeigefeld, DB-Feld: zuaufint.subr
- **Versandart:** Nummer der Versandart.
  - Technische Info: numerisches Feld, DB-Feld: zuaufint.sfill1
- **Lieferart:** Nummer der Lieferart.
  - Technische Info: numerisches Feld, DB-Feld: zuaufint.sfill2
- **A-Zoll:** Schlüsselnummer der Ausgangs-Zollstelle.
  - Technische Info: numerisches Feld, DB-Feld: zuaufint.sfill3
- **B-Zoll:** Schlüsselnummer der Bestimmungs-Zollstelle.
  - Technische Info: numerisches Feld, DB-Feld: zuaufint.lfill1
- **Versandinfo:** Firmeninterner Informationstext zum Versand.
  - Technische Info: alphanumerisches Feld, DB-Feld: zuaufint.cfill1
- **LE:** Angabe, ob eine Leistungserklärung vorliegt.
  - ☑ Es liegt eine Leistungserklärung vor.
  - ☐ Es liegt keine Leistungserklärung vor.
  - Technische Info: Checkbox
- **Frei:** Angabe, ob der Vorgang freigeschaltet werden soll.
  - ☑ Der Vorgang wird freigeschaltet.
  - ☐ Der Vorgang wird nicht freigeschaltet.
  - Technische Info: Checkbox, DB-Feld: kauf.tekapkz

Mit weiterer `<F2>` wechseln Sie in den Register **Kalkulation**. Hier werden folgende Felder angezeigt:
- **Vorgang:** Art des Vorgangs.
  - Auftrag
  - Lief: Lieferung
  - Angeb: Angebot
  - Technische Info: Toggle-Feld, DB-Feld: zuaufint.vorgang
- **Auftrag:** Vorgangsnummer.
  - Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: zuaufint.auftrnr
- **Subnr.:** Sub-Nummer des Vorgangs.
  - Technische Info: Anzeigefeld, DB-Feld: zuaufint.subr
- **LE:** Angabe, ob eine Leistungserklärung vorliegt.
  - ☑ Es liegt eine Leistungserklärung vor.
  - ☐ Es liegt keine Leistungserklärung vor.
  - Technische Info: Checkbox
- **Kalkulation:** Art der Kalkulation, die durchgeführt werden kann. Folgende Auswahl über die [Leertaste] möglich.
  - Keine Neukalkulation
  - Verkaufs- und Einkaufspreise
  - Verkaufspreise
  - Einkaufspreise
  - Technische Info: alphanumerisches Feld, DB-Feld: zuaufint.rechart
- **Rabatte:** Art der Korrektur für die im Vorgang vorhandenen Rabatten. Folgende Auswahl über die [Leertaste] möglich.
  - Spezielle Rabatte aktualisieren
  - Neue Rabattmethoden
  - Alle Rabatte neu
  - Technische Info: alphanumerisches Feld, DB-Feld: zuaufint.rabrechart
- **Frei:** Angabe, ob der Vorgang freigeschaltet werden soll.
  - ☑ Der Vorgang wird freigeschaltet.
  - ☐ Der Vorgang wird nicht freigeschaltet.
  - Technische Info: Checkbox, DB-Feld: kauf.tekapkz

### Übersicht zu Vorgängen

**Navigation:** `Verkauf > Übersicht > Unberechnete Aufträge, Ungebuchte Rechnungen, Unvollständige Lieferungen, Aufträge mit Fakturasperre > Datum eingeben > [OK]`

*Abb. D-187 Unberechnete Aufträge, Ungebuchte Rechnungen, Unvollständige Lieferungen und Aufträge mit Fakturasperre*

In diesen Dialogen werden die Übersichten zu folgenden Vorgängen im gewählten Zeitraum angezeigt:
- **Unberechnete Aufträge:** Zeigt alle Aufträge an, zu denen noch keine Rechnung erstellt wurde.
- **Ungebuchte Rechnungen:** Zeigt alle Vorgänge an, zu denen eine Rechnung erstellt ist, die noch nicht gebucht wurde.
- **Unvollständige Lieferungen:** Zeigt alle Vorgänge an, bei denen noch unvollständige Lieferungen ausstehen.
- **Aufträge mit Fakturasperre:** Zeigt alle Aufträge an, für die die Rechnungsstellung gesperrt ist.

Wenn Sie eine der Übersichten öffnen wollen, müssen Sie zunächst in einem Dialog das Startdatum der Suche eingeben. Wenn Sie kein Datum angeben, werden in der Übersicht alle entsprechenden Vorgänge angezeigt.

Die Anzeige der Spalten ist frei konfigurierbar und hängt von der kundenindividuellen Formatierung der jeweiligen SQL-Abfrage ab.
Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

## Vertrieb

Im Vertrieb werden Ihnen Informationen zur Akquise und Provisionsberechnung angezeigt und Sie können die Objektbudgetierung verwalten.
Alle Dialoge, die Sie über den Menüpunkt Vertrieb öffnen können, sind kundenindividuelle Programmanpassungen.
Für weitere Informationen zu diesem Bereich kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

---

# Help Cards

## In diesem Kapitel finden Sie folgende Themen:

- **Informationen zu den Help Cards**
- **Angebot**
- **Auftrag**
- **Auftragsposition**
- **Preisberechnung**
- **Rechnung**
- **Weitere Themen**

### Detaillierter Index der Help Cards

- **Informationen zu den Help Cards** (D-1478)
- **Angebot** (D-1479)
  - Schnellerfassung (D-1480)
  - Angebot erfassen (D-1481)
- **Auftrag** (D-1482)
  - Kopfdaten erfassen (D-1483)
  - Auftrag mit Bezug erfassen (D-1484)
  - Auftragsart festlegen (D-1485)
  - Eigenschaften bearbeiten (D-1486)
  - Lieferanschrift bearbeiten (D-1487)
  - Lieferplan bearbeiten (D-1488)
  - Zahlungsoptionen bearbeiten (D-1489)
  - Auftrag freischalten (D-1490)
  - Auftragsinformationen anzeigen (D-1491)
  - Text im Auftrag bearbeiten (D-1492)
  - Anmerkungen bearbeiten (D-1493)
  - Datei anhängen (D-1494)
- **Auftragsposition** (D-1495)
  - Position erfassen (D-1496)
  - Lieferant bearbeiten (D-1497)
  - Glas austauschen (D-1498)
  - Modell erfassen (D-1499)
  - Bearbeitung erfassen (D-1500)
  - Bearbeitung aus SN-Datei übernehmen (D-1501)
  - SN-Datei anhängen (D-1502)
  - Änderungen mit SN-Datei abgleichen (D-1503)
  - Position in CAD erfassen (D-1504)
  - Stufenglas erfassen (D-1505)
  - Sprossen erfassen (D-1506)
  - Sprossenaufbau bearbeiten (D-1507)
  - Einstand und Versiegelungstiefe (D-1508)
  - Randentschichtung erfassen (D-1509)
  - Produkt austauschen (D-1510)
  - Artikel fixieren (D-1511)
  - Leistungserklärung zuordnen (D-1512)
  - Technische Werte erfassen (D-1513)
- **Preisberechnung** (D-1514)
  - Positionskonditionen ändern (D-1515)
  - Artikelpreise ändern (D-1516)
  - Fußrabatt, Zuschlag bearbeiten (D-1517)
  - Produktionskosten prüfen (D-1518)
  - Preisprotokoll für VSG (D-1519)
- **Rechnung** (D-1520)
  - Rechnung manuell erstellen (D-1521)
  - Rechnungen automatisch erzeugen (D-1522)
  - Rechnung buchen (D-1523)
  - Rechnung drucken (D-1524)
  - Elektronische Rechnung (E-Invoicing) versenden (D-1525)
  - Kunden für elektronische Rechnungen konfigurieren (D-1526)
  - Gutschrift erfassen (D-1527)
- **Weitere Themen** (D-1528)
  - Vorgang suchen (D-1529)
  - Vorgangsänderung (D-1530)

## Informationen zu den Help Cards

Die Darstellungen in den Help Cards basieren auf der Auslieferversion A+W Enterprise V 6. Einzelne Schritte in den Workflows können je nach Konfiguration abweichen.

- **Aufträge als Beispiel**
  Verschiedene Funktionalitäten können in mehreren Vorgangsarten gestartet werden. In diesen Help Cards werden sie immer am Beispiel Auftrag gezeigt.

- **Tasten und Tastenkombinationen**
  Die Kenntnis der Bedienung wird als bekannt vorausgesetzt. In den Handlungsschritten wird jeweils nur eine der möglichen Tasten oder Tastenkombinationen genannt, mit denen eine Funktion oder ein Menü aufgerufen werden können.
  Die im geöffneten Dialog möglichen Funktionen und Tasten können in der Prompt-Zeile am unteren Rand des Dialogs angezeigt werden.

## Angebot

| Help Card | Themen |
| :--- | :--- |
| Schnellerfassung | - Angebot schnell anlegen.<br>- Auftrag schnell anlegen. |
| Angebot erfassen | - Angebot erfassen.<br>- Wiedervorlage bearbeiten.<br>- Manuelle Wiedervorlage anlegen. |

### VK 01-001: Angebot Schnellerfassung

**Ziel der Handlung**
- Auftrag schnell erfassen.
- Angebot schnell erfassen.

**Voraussetzungen**
- Schnellerfassung muss konfiguriert sein.
- Stammdaten müssen angepasst sein.

**Zusatzinfo**
- Keine

**Workflow**

1.  Menü `Verkauf > Schnellerfassung` wählen.
    Dialog **Auftragserfassung** wird mit Marktpartnersuche geöffnet.
2.  Kunde wählen und übernehmen.
3.  Pflichtfelder * prüfen und füllen.
4.  Bereich **Lieferanschrift**: mit `[Suche Adresse]` Lieferadresse auswählen. Ggf. mit `[Neue Adresse]` Adresse anlegen.
5.  Zum Register **Positionen** wechseln.
6.  Feld **ProduktCode**: Artikelnummer auswählen oder eingeben.
7.  Positionsdaten ergänzen.
8.  Schritt 6 und 7 für weitere Positionen bei Bedarf wiederholen.
9.  Zum Register **Übersicht** wechseln.
10. Auftrag mit `[Speichern]` anlegen.
11. **Angebot schnell erfassen:** Schritte 1 bis 9 ausführen.
12. Angebot mit `[Als Angebot speichern]` anlegen. Dialog **Grund** für das Angebot wird geöffnet.
13. Grund eingeben und mit `[OK]` übernehmen.
14. Hinweis auf neuen Angebotsnummer bestätigen.
15. **Nächster Schritt:**
    - Weiteren Auftrag über die Schnellerfassung anlegen.
    - Dialog mit `<Esc>` schließen.

### VK 01-002: Angebot erfassen

**Ziel der Handlung**
- Angebot erfassen.
- Wiedervorlage bearbeiten.
- Manuelle Wiedervorlage anlegen.

**Voraussetzungen**
- Automatische Wiedervorlage ist eingerichtet: Menü `System > Vorgangsverwaltung > Wiedervorlage-modus`

**Zusatzinfo**
- Wiedervorlage löschen: `<F7>` drücken.
- Automatische Wiedervorlagen werden pro Vorgangsart eingerichtet.
- Manuelle Wiedervorlage zu Auftrag erfassen: Feld `Termin > <Shift>+<F4> > Wiedervorlage`.
- ⇨ Position erfassen
- ⇨ Vorgang suchen

**Workflow**

1.  Menü `Verkauf > Angebotserfassung` wählen. Dialog **Angebotserfassung** wird geöffnet.
2.  Kunde auswählen.
3.  Feld **Termin**: ggf. möglichen Liefertermin eintragen. Alternativ: der Liefertermin wird von A+W Production ermittelt und zurückgeschrieben.
4.  Positionen erfassen und Angebot speichern.
5.  **Wiedervorlage bearbeiten:** Menü `Verkauf > Wiedervorlage` wählen. Dialog **Wiedervorlage** wird geöffnet.
6.  Aktuelles Angebot auswählen:
    - Termin für Wiedervorlage bearbeiten.
    - Bemerkung eingeben.
7.  **Manuelle Wiedervorlage anlegen:** Menü `Verkauf > Wiedervorlage > <F6>` wählen. Am Ende der Liste wird eine neue Zeile eingefügt.
8.  Felder der neuen Zeile ausfüllen:
    - Datum eintragen.
    - Vorlageart auswählen und Text eintragen.
    - Mitarbeiter auswählen.
9.  Dialog mit `<Ende>` schließen.

## Auftrag

| Help Card | Themen |
| :--- | :--- |
| Kopfdaten erfassen | Auftrag anlegen. |
| Auftrag mit Bezug erfassen | Auftrag mit Bezug auf Angebot erfassen. Angebot mit Bezug auf früheren Auftrag erfassen. |
| Auftragsart festlegen | Lagerauftrag erfassen. Chef-Auftrag erfassen. Nachlieferung als Kulanzauftrag erfassen. |
| Eigenschaften bearbeiten | Versandinformation ändern. Rechnungs- und Druckoptionen für kaufmännische Papiere ändern. Außendienstmitarbeiter ändern. |
| Lieferanschrift bearbeiten | Lieferanschrift für Auftrag eingeben. Neue Lieferanschrift in Stammdaten übernehmen. |
| Lieferplan bearbeiten | Lieferdatum für Position und Gesamtmenge festlegen. Lieferplan für Teillieferungen einer Position anlegen. |
| Zahlungsoptionen bearbeiten | Zahlungsoptionen ändern. |
| Auftrag freischalten | Aufträge einer Abteilung und/oder eines Erfassers freischalten. Alle Aufträge freischalten. Gründe für Sperre prüfen. |
| Auftragsinformationen anzeigen | Produktionsstatus des Auftrags prüfen. Lieferterminänderungen prüfen. |
| Text im Auftrag bearbeiten | Kopf- oder Fußtext zum Auftrag erfassen. Artikel- und Positionstext bearbeiten. Artikeltext in Kundensprache prüfen. |
| Anmerkungen bearbeiten | Interne Anmerkung zum Auftragskopf oder -fuß erfassen. Interne Anmerkung zur Position oder zum Artikel erfassen. |
| Datei anhängen | Dokument für den Kunden anhängen. Dokument zur Position anhängen. |

### VK 02-001: Auftrag Kopfdaten erfassen

**Ziel der Handlung**
- Auftrag anlegen.

**Voraussetzungen**
- Stammdaten sind vollständig erfasst.

**Zusatzinfo**
- Angebote werden auf dieselbe Weise erfasst wie Aufträge: Menü `Verkauf > Angebotserfassung`.
- ⇨ Angebot erfassen
- ⇨ Auftrag mit Bezug erfassen
- ⇨ Position erfassen

**Workflow**

1.  Menü `Verkauf > Auftragserfassung` wählen. Dialog **Auftragserfassung** wird geöffnet.
2.  Feld **Auftrag**: mit `<Enter>` in das Feld **Kunde** springen. Im Feld **Auftrag** wird die nächste freie Vorgangsnummer eingefügt.
3.  Kundennummer eintragen oder auswählen.
4.  Mit `<Enter>` durch die nachfolgenden Felder gehen und prüfen.
5.  Feld **Bezug**: ggf. mit `<F9>` Angebot auswählen oder Nummer eintragen.
6.  Feld **Termin**: ggf. möglichen Liefertermin eintragen. Alternativ: der Liefertermin wird von A+W Production ermittelt und zurückgeschrieben.
7.  Feld **Route**: Standardroute aus dem Kundenstamm prüfen und ggf. ändern.
8.  Daten in den weiteren Feldern prüfen und ergänzen.
9.  Feld **Objekt**: ggf. Objektnummer auswählen oder eintragen.
10. Kopfdaten mit `<Enter>` speichern.

### VK 02-002: Auftrag mit Bezug erfassen

**Ziel der Handlung**
- Auftrag mit Bezug auf Angebot erfassen.
- Angebot mit Bezug auf früheren Auftrag erfassen.

**Voraussetzungen**
- Stammdaten sind vollständig erfasst.

**Zusatzinfo**
- Auf die gleiche Weise wird ein Angebot mit Bezug auf einen Auftrag erfasst.
- ⇨ Vorgang suchen
- ⇨ Position erfassen

**Workflow**

1.  Menü `Verkauf > Auftragserfassung` wählen. Dialog **Auftragserfassung** wird geöffnet.
2.  Feld **Auftrag**: mit `<Enter>` das Feld **Kunde** springen. Im Feld **Auftrag** wird die nächste freie Vorgangsnummer eingefügt.
3.  Kundennummer eintragen oder auswählen.
4.  Mit `<Enter>` durch die nachfolgenden Felder gehen und prüfen.
5.  Feld **Bezug**: `<F9>` drücken. Dialog **Suche Bezugsvorgang** wird geöffnet.
6.  Feld **Vorgang**: mit `<F9>` Eintrag **Angebot** auswählen und Suche starten.
7.  Angebot markieren und übernehmen.
8.  Abfrage zur Übernahme der Daten bestätigen:
    - `[Ja]`: Kopf- und Positionsdaten übernehmen.
    - `[Nein]`: Nur die Kopfdaten übernehmen.
9.  Ggf. Abfrage zu den Rabatten bestätigen.
10. Restliche Kopfdaten prüfen und ggf. ergänzen.
11. Positionen prüfen und ggf. ergänzen.
12. Auftrag speichern und beenden.

### VK 02-003: Auftragsart festlegen

**Ziel der Handlung**
- Lagerauftrag erfassen.
- Chef-Auftrag erfassen.
- Nachlieferung als Kulanzauftrag erfassen.

**Voraussetzungen**
- Auftragserfassung ist geöffnet.

**Zusatzinfo**
- Auf die gleiche Weise werden alle Auftragsarten erfasst.
- Auftrag ohne Preisanzeige erfassen: Menü `Verkauf > Preislose Erfassung`.
- Die VK-Preise werden berechnet, wenn der Auftrag gedruckt wird.
- ⇨ Elektronische Rechnung (E-Invoicing) versenden

**Workflow**

1.  Auftragskopf bis zum Feld **Bezug** erfassen.
2.  Auftrag auswählen, auf den sich die Nachlieferung bezieht.
3.  Felder weiter füllen bis Feld **Eingang**.
4.  Feld **Eingang**: `<Strg>+<F12>` Eingang. Dialog **Auftragsarten** wird geöffnet.
5.  Auftragsart wählen, z. B. **Kostenloser Auftrag**. Dialog **Kostenloser Auftrag** wird geöffnet.
6.  Position erfassen und Erfassung abschließen.
7.  Hinweis auf Nullbetrag mit `[Nein]` bestätigen.
8.  Ggf. Angaben zur Reklamation auswählen.
9.  Angaben mit `<Enter>` bestätigen und übernehmen.
10. Abfragen bestätigen.
11. Frage nach Vollständigkeit des Auftrags mit `[Ja]` bestätigen.
12. Frage zur Freischaltung mit `[Ja]` bestätigen.

### VK 02-004: Eigenschaften bearbeiten

**Ziel der Handlung**
- Versandinformation bearbeiten.
- Rechnungs- und Druckoptionen für kaufmännische Papiere bearbeiten.
- Außendienstmitarbeiter ändern.

**Voraussetzungen**
- Auftragserfassung ist geöffnet.
- Auftrag ist erfasst.

**Zusatzinfo**
- Änderungen der Felder **Zustellungsart** und **Direktauslieferung** haben Einfluss auf den gesamte Auftrags- und Bestellungsablauf.
- Änderungen der Rechnungsoptionen können Zuschläge aktivieren, z. B. Eilauftrag.
- ⇨ Zahlungsoptionen bearbeiten

**Workflow**

1.  Zum Register **Eigenschaften** wechseln.
2.  Daten im Bereich **Mitarbeiterformationen** bearbeiten, z. B.:
    - Feld **Bestellt von**: Ansprechpartner beim Kunden ändern.
    - Feld **Bestelldatum**: Datum prüfen und ggf. ändern.
3.  Daten im Bereich **Versandinformationen** bearbeiten, z. B.:
    - Feld **Verpackungsart**: Verpackungsart auswählen, z. B. Kiste.
    - Feld **Gest.-Beladung**: Sortierfolge für Verpackung in Kisten oder auf Gestellen auswählen, z. B. nach Kommission.
4.  Druckoptionen für kaufmännische Papiere bearbeiten, z. B.:
    - Feld **Verglasung**: Preis der Verglasung ausweisen, z. B. in Position einrechnen.
    - Feld **Artikeltexte drucken**: J = Texte drucken.
    - Feld **Modelle drucken**: J = Modellskizze drucken.
    - Feld **Positionspreise unterdrücken**: J = Positionspreise nicht drucken.
5.  Mit `<Ende>` zum Auftragskopf wechseln.
6.  Erfassung fortsetzen oder Auftrag speichern und beenden.

### VK 02-005: Lieferanschrift bearbeiten

**Ziel der Handlung**
- Lieferanschrift für Auftrag eingeben.
- Neue Lieferanschrift in Stammdaten übernehmen.

**Voraussetzungen**
- Auftragserfassung ist geöffnet.
- Auftragskopf ist erfasst.

**Zusatzinfo**
- Änderungen betreffen nur den aktuellen Auftrag.

**Workflow**

1.  Zum Register **Anschriften** wechseln.
2.  **Anschrift aus Stammdaten wählen:** `<Shift>+<F8>` drücken. Die Adressen aus den Kundenstammdaten werden angezeigt.
3.  Adresse auswählen und übernehmen.
4.  **Adresse suchen:** Adressensuche starten: `<Strg>+<L>` drücken. Dialog **Adressen Suche** wird angezeigt.
5.  Adresse suchen und übernehmen.
6.  **Alternative Lieferanschrift für den Auftrag eingeben:** Menü `<F4> > Adressen > Neue Lieferadresse` wählen. Dialog zur Erfassung der Adressdaten wird geöffnet.
7.  Alle erforderlichen Daten eingeben.
8.  Neue Adresse mit `[OK]` in den Auftrag übernehmen und speichern.
9.  **Neue Anschrift in Kundenstammdaten übernehmen:** Neue Lieferanschrift erfassen.
10. Übernahme mit `<F3>` starten und Abfrage bestätigen.
11. Neue Adresse mit `[OK]` in den Auftrag übernehmen und speichern. Die Lieferadresse wird für den Auftrag gespeichert.
12. Erfassung fortsetzen oder Auftrag speichern und beenden.

### VK 02-007: Lieferplan bearbeiten

**Ziel der Handlung**
- Lieferdatum für Position und Gesamtmenge festlegen.
- Lieferplan für Teillieferungen einer Position anlegen.

**Voraussetzungen**
- Auftragserfassung ist geöffnet.
- Kunde erlaubt Teillieferung.

**Zusatzinfo**
- Lieferscheine werden je nach Konfiguration in der Versandplanung erstellt.

**Workflow**

1.  Auftrag: `<F4> > Lieferplan` wählen. Dialog **Lieferplan** wird angezeigt.
2.  Feld **Lieferdatum**: Lieferdatum festlegen.
3.  Feld **Route**: ggf. alternative Route wählen.
4.  Schritte für alle Positionen wiederholen.
5.  Änderungen mit `[OK]` speichern.

**Teillieferung einer Position:**

6.  Feld **Geplant**: Teilmenge angeben. Eine neue Zeile mit der Restmenge wird eingefügt.
7.  Feld **Lieferdatum**: Lieferdatum für Restmenge angeben.
8.  Feld **Route**: ggf. Route für Restmenge wählen.
9.  Änderungen mit `[OK]` speichern.

**Nächster Schritt:** Lieferschein erstellen und Versand planen

### VK 02-006: Zahlungsoptionen bearbeiten

**Ziel der Handlung**
- Zahlungsoptionen ändern.

**Voraussetzungen**
- Auftragserfassung ist geöffnet.
- Auftragskopf ist erfasst.

**Zusatzinfo**
- Die Zahlungsoptionen sind mit den Daten aus den Kundenstammdaten vorbelegt.
- Änderungen betreffen nur den aktuellen Auftrag.

**Workflow**

1.  Zum Register **Verschiedenes** wechseln.
2.  Daten für Reklamation im Bereich **Reklamationsinformation** eintragen, z. B.:
    - Feld **Art**: Reklamationsart auswählen, z. B. Verpackung.
    - Feld **Ort**: Reklamationsort auswählen, z. B. Verladung.
3.  Daten für Zahlungsmodus im Bereich **Zahlungsoptionen** eintragen, z. B.:
    - Feld **Zahlungsziel**: Anzahl der Tage bis zur Fälligkeit eingeben, z. B. 30 Tage.
    - Felder **Skonto 1, 2, 3**: Skontosätze für gestaffelte Zahlungsziele auswählen.
    - Felder **Merkmal, Zahlungsverkehr**: Art und Weise der Zahlung auswählen, z. B. Bankabbuchung.
4.  Bereich **Details der Auslieferung**: Ggf. Termin des Wareneingangs von Zukauf angegeben.
5.  Mit `<Ende>` zum Auftragskopf wechseln.
6.  Erfassung fortsetzen oder Auftrag speichern und beenden.

**Nächster Schritt:** Position erfassen

### VK 02-008: Auftrag freischalten

**Ziel der Handlung**
- Aufträge einer Abteilung und/oder eines Erfassers freischalten.
- Alle Aufträge freischalten.
- Gründe für Sperre prüfen.

**Voraussetzungen**
- Mitarbeiterrechte sind erteilt.
- Auftrag steht im Freischaltpool.

**Zusatzinfo**
- Keine

**Workflow**

1.  Menü `Verkauf > Auftragsfreischaltung > Freischaltung` wählen. Dialog **Auftragsfreischaltung** wird geöffnet.
2.  Auswahlkriterien wählen, z. B. Abteilung oder Erfasser.
3.  Suche mit `[Start]` auslösen. Liste der Aufträge wird angezeigt.
4.  Feld **Frei**: JA wählen.
5.  Feld **LSp**: J wählen.
6.  Änderung mit `<F3>` auslösen.

**Reihe von Aufträgen freischalten:**

7.  Ersten Auftrag wählen, ab dem alle freigeschaltet werden sollen: `<Shift>+<F9>` drücken.

**Alle Aufträge freischalten:**

8.  `<Strg>+<F9>` drücken.
9.  Abfragen mit `[Ja]` bestätigen.

**Sperrgründe prüfen:**

10. Nicht freigeschalteten Auftrag markieren.
11. Auf `[Sperrliste]` klicken. Dialog **Sperrgründe für nicht erfolgte Freischaltung** wird angezeigt. Dialog **Sperrgründe für nicht erfolgte Freischaltung** wird angezeigt.

### VK 02-009: Auftragsinformationen anzeigen

**Ziel der Handlung**
- Produktionsstatus des Auftrags prüfen.
- Lieferterminänderungen prüfen.

**Voraussetzungen**
- Keine

**Zusatzinfo**
- ⇨ Vorgang suchen

**Workflow**

1.  Menü `Verkauf > Auftragserfassung` wählen. Dialog **Auftragserfassung** wird geöffnet.
2.  Feld **Auftrag**: `<F9>` drücken. Dialog **Suche Aufträge** wird geöffnet.
3.  Auftrag suchen:
    - Feld **Aufträge ab**: Startnummer angeben.
    - Feld **Kunde**: Kundennummer angeben.
4.  Suche mit `<F3>` starten und Auftrag aus Trefferliste übernehmen.
5.  Feld **Menge**: `<Shift>+<F10>` drücken. Dialog **Auftragsinformationen** wird geöffnet.

### VK 02-010: Text im Auftrag bearbeiten

**Ziel der Handlung**
- Internen Kopf- oder Fußtext zum Auftrag erfassen.
- Artikel- und Positionstext bearbeiten.

**Voraussetzungen**
- Auftragserfassung ist geöffnet.
- Position ist vollständig erfasst.

**Zusatzinfo**
- Texte können als Textbausteine gespeichert werden.
- Texte werden in Kundensprache angezeigt.
- Artikel- oder Positionstext erfassen: im Preisfeld `<F5>` drücken.
- Rahmen-, Modelltexte, Produktkennzeichen erfassen: `<F4> > Texte > Spezielle Texte`.

**Workflow**

1.  Cursor im Auftragskopf oder im Auftragsfuß.
2.  Texterfassung aufrufen: `<F4> > Texte > Kopftext` oder `Fußtext`. Der Dialog **Texte** wird geöffnet.
3.  Register wählen.
4.  Text frei eingeben und mit `[OK]` übernehmen.

**Textbausteine verwenden:**

5.  Textbaustein einsetzen: `[Floskeln]` > Kennung eingeben > `[OK]`.
6.  Textbaustein auswählen: `[Floskeln]` > Suche starten > Textbaustein markieren > `[Übernehmen]`.
7.  Bereich **Formulare**: Checkboxen der Formulare markieren, auf denen der Text gedruckt soll.
8.  Text mit `[OK]` bestätigen.

**Artikeltext prüfen:**

9.  Im Preisfeld `<F5>` drücken. Der Dialog **Texte** wird geöffnet.
10. Einträge prüfen.

### VK 02-011: Anmerkungen bearbeiten

**Ziel der Handlung**
- Interne Anmerkung zum Auftragskopf oder -fuß erfassen.
- Interne Anmerkung zur Position oder zum Artikel erfassen.

**Voraussetzungen**
- Vorgang ist geöffnet.
- Anmerkungen: sind ggf. in den Stammdaten hinterlegt.

**Zusatzinfo**
- Anmerkungen werden nur automatisch angezeigt, wenn mindestens eine Zeile mit der Priorität hoch enthalten ist.
- Anmerkungen aus den Stammdaten werden im Auftrag ebenfalls mit `<Shift>+<F4>` angezeigt.

**Workflow**

1.  Cursor im Auftragskopf oder -fuß: `<Shift>+<F4> > Anmerkungen > Vorgangs-Anmerkungen` wählen. Dialog **Anmerkungen** wird geöffnet.
2.  Anmerkung eintragen.
3.  `[Priorität]`: Priorität hoch wählen.
4.  Anmerkung mit `[OK]` speichern und übernehmen.
5.  Auftrag speichern.

**Interne Anmerkung zur Position oder zum Artikel erfassen:**

6.  Register **Positionen**: Register **Allgemein** > `<Shift>+<F4> > Anmerkungen > Artikel-Anmerkungen` wählen.
7.  Schritte 2 bis 4 wiederholen.
8.  Änderungen speichern.

### VK 01-012: Datei anhängen

**Ziel der Handlung**
- Dokument für den Kunden anhängen.
- Dokument zur Position anhängen.

**Voraussetzungen**
- Dokumentenpfad muss eingerichtet sein.
- Datei muss verfügbar sein.
- Auswahl der Formulare muss konfiguriert sein.

**Zusatzinfo**
- `[Löschen]`: Dokumentenzuordnung löschen.
- `[Reaktivieren]`: Dokumentenzuordnung wieder herstellen.
- `[Link trennen]`: Nur bei Aufträgen, die mit Bezug erfasst sind, zur Trennung des Links zum Dokumentenpfad.

**Workflow**

1.  Menü `Verkauf > Vorgang öffnen`.
2.  Feld **Eingang**, Feld **Rechnungstyp**, Feld **Objekt**: `<Strg>+<K>` drücken. Dialog **Dokumentenartenzuordnung** wird angezeigt.
3.  Feld **DokArt**: Dokumentenart auswählen und mit `<Tab>` in Feld **Datei** springen.
4.  Datei im Windows-Explorer suchen.
5.  Datei auf Ordnersymbol im Dialog **Dokumentenartenzuordnung** ziehen und fallen lassen. Dateiname wird im Feld **Datei** angezeigt, Ordnersymbol wechselt zum Symbol **Dokument**.
6.  Feld **Formulare**: `<F9>` drücken und Formular auswählen.
7.  Dokument an die Produktion übergeben: Feld **Prod** mit `<Leer>` Checkbox markieren oder Markierung entfernen.
8.  Zuordnung mit `[OK]` bestätigen.

**Dokument zur Position anhängen:**

9.  Register **Allgemein**: Position markieren.
10. `<Strg>+<K>` drücken.
11. Schritte 3 bis 8 wiederholen.
12. Speichern.

## Auftragsposition

| Help Card | Themen |
| :--- | :--- |
| Position erfassen | Auftragsposition erfassen. Positionen hinzufügen. |
| Lieferant bearbeiten | Lieferant ändern. Beschaffungsart ändern. |
| Glas austauschen | Glas in Produktaufbau ändern. Einbauposition von Glas ändern. |
| Modell erfassen | Auftragsposition mit Modell erfassen. |
| Bearbeitung erfassen | Bearbeitung manuell erfassen. |
| Bearbeitung aus SN-Datei übernehmen | Bearbeitungen aus SN-Datei in Stückliste übernehmen. |
| SN-Datei anhängen | Bearbeitungen aus SN-Datei in Stückliste übernehmen. Kopie von SN-Datei anhängen. |
| Änderungen mit SN-Datei abgleichen | Bearbeitungen in angehängter SN-Datei ändern oder ergänzen. Bearbeitungen in Stückliste ändern oder ergänzen. |
| Position in CAD erfassen | Geometrie und Bearbeitungen in A+W CAD Designer (Shapes) erfassen, in Position übernehmen und als SN-Datei speichern. Interaktive Erfassung in A+W CAD Designer (Shapes). |
| Stufenglas erfassen | Stufung in Mehrfach-Scheibe erfassen. |
| Sprossen erfassen | Sprossenaufbau erfassen. |
| Sprossenaufbau bearbeiten | Sprossenbild mit dem Sprosseneditor bearbeiten. Nicht symmetrischen Sprossenaufbau erfassen. |
| Einstand und Versiegelungstiefe | Einstand und Versiegelungstiefe in ISO-Scheiben erfassen. |
| Randentschichtung erfassen | Randentschichtung erfassen. |
| Produkt austauschen | Artikel in mehreren Auftragspositionen austauschen. Scheibenaufbau in mehreren Auftragspositionen bearbeiten. |
| Artikel fixieren | Artikel einer Auftragsposition fixieren. Fixierten Artikel in die Stammdaten aufnehmen. |
| Leistungserklärung zuordnen | Leistungserklärung prüfen und/oder zuordnen. |
| Technische Werte erfassen | Technische Werte erfassen. Neue Leistungserklärung generieren. |

### VK 03-001: Position erfassen

**Ziel der Handlung**
- Auftragsposition erfassen.
- Positionen nachträglich hinzufügen.

**Voraussetzungen**
- Artikelstammdaten sind vorhanden.
- Auftragserfassung ist geöffnet.
- Auftragskopf ist erfasst.

**Zusatzinfo**
- ⇨ Lieferant bearbeiten
- ⇨ Stufenglas erfassen
- ⇨ Modell erfassen
- ⇨ Sprossen erfassen
- ⇨ Bearbeitung erfassen

**Workflow**

1.  Mit `<Enter>` vom Auftragskopf zum Register **Positionen > Allgemein** wechseln.
2.  Feld **Artikel**: Artikel auswählen:
    - Artikelnummer eingeben.
    - Mit `<F9>` Artikelsuche starten.
    Abhängig von den Artikeldaten werden verschiedene Eingabefelder angezeigt.
3.  Stückzahl eingeben und mit `<Enter>` zum nächsten Feld springen.
4.  Maße eingeben oder ggf. Variante auswählen. Bei ISO-Gläsern zusätzlich das Maß für den Abstandhalter (SZR) angegeben.
5.  Feld **Prov**: ggf. mit `<F9>` den Provisionsschlüssel ändern.
6.  Feld **B.Art**: Beschaffungsart prüfen und ggf. ändern.
    Die Werte für die Felder ME/St, kg/St und die Preise werden berechnet und gefüllt.
7.  **Weitere Position hinzufügen:**
    - Am Ende einfügen: `<F6>` drücken.
    - Über markierter Positionen einfügen: `<Shift>+<F6>` drücken.
    - Position kopieren: Position markieren und `<Alt>+<C>` oder `[Pos. kopieren]`. Beim Erfassen einer Position mit derselben Artikelnummer wird der Stücklistenaufbau übernommen.
8.  Erfassung im Feld **Preis** abschließen:
    - `<Ende>`: Auftrag zu speichern und Fußdaten prüfen.
    - `<F2>`: zum Auftragskopf wechseln.
9.  Erfassung fortsetzen oder Auftrag speichern und beenden.

### VK 03-002: Lieferant bearbeiten

**Ziel der Handlung**
- Lieferant ändern.
- Beschaffungsart ändern.

**Voraussetzungen**
- Lieferanten sind angelegt.
- Auftragserfassung ist geöffnet.
- Position ist erfasst.

**Zusatzinfo**
- Mit der Angabe eines Lieferanten wird die Beschaffungsart immer auf Bestellung geändert.
- Mit der Änderung der Beschaffungsart auf Bestellung muss immer ein Lieferant angegeben werden.

**Workflow**

1.  Zum Register **Positionen > Allgemein** wechseln.
2.  Feld **Menge**: `<Shift>+<F12>` drücken. Neben der Grafik werden die Felder **Lieferant** und **Lief.zeit** angezeigt.
3.  Feld **Lieferant**: Lieferantennummer eingeben oder mit `<F9>` auswählen.
4.  Feld **Lief.zeit**: Lieferzeit in Tagen eintragen.
5.  Mit `<Enter>` weiterspringen und die Abfragen bestätigen. Der Lieferant kann für den gesamten Auftrag, für die nachfolgenden Positionen oder nur für die aktuelle Position übernommen werden.
6.  Erfassung fortsetzen oder Auftrag speichern und beenden.
7.  **Beschaffungsart ändern:** Position erfassen und Lieferanten eingeben.
8.  Feld **B.Art**: Mit `<Leer>`-Taste zur Beschaffungsart blättern, z. B. **Bestellung**.
9.  Position speichern und Erfassung fortsetzen.

### VK 03-003: Glas austauschen

**Ziel der Handlung**
- Glas in Produktaufbau ändern.
- Einbauposition von Glas ändern.

**Voraussetzungen**
- Auftragserfassung ist geöffnet.
- Position ist mit Menge und Maßen erfasst.

**Zusatzinfo**
- Austauschgläser können in ISO- und VSG-Scheiben erfasst werden.
- Einbaupositionen werden von außen nach innen gezählt.

**Workflow**

1.  Register **Positionen > Allgemein** > ISO-Position erfassen, z. B. ISO-Artikel.
2.  Dialog **Stücklistendarstellung** öffnen: `[Stückliste]`.
3.  Register **Akt. Stücklistenebene**: Unterteil markieren > `[Stückliste]`. Im Stücklistenbaum wird die aktuelle Stücklistenebene gekennzeichnet.
4.  Register **Akt. Stücklistenebene**: Artikelnummer des Austauschglases ändern.
5.  Je nach Glas folgende Details angeben:
    - Feld **Strkt**: Strukturverlauf auswählen.
    - Feld **Lieferant**: Lieferant auswählen.
    - Feld **Druck**: Druckoption für Produktions- oder Verkaufspapiere auswählen.
6.  Änderungen mit `[OK]` übernehmen. Im Register **Akt. Stücklistenebene** werden alle Unterteile angezeigt.
7.  **Einbauposition ändern:** Feld **EP**: Nummer der Einbauposition des Austauschglases eingeben. Die Nummer des zweiten Glases wird automatisch geändert.
8.  **Strukturposition tauschen:** Stückliste zu Austauschglas öffnen.
9.  Feld **EP**: Nummer der Einbauposition des Glases eingeben.
10. Dialoge **Stücklistendarstellung** mit `[OK]` schließen. Dialog **Auftragserfassung** wird wieder angezeigt.
11. Abfrage zur Preisberechnung bestätigen.
12. Änderungen speichern.

### VK 03-004: Modell erfassen

**Ziel der Handlung**
- Auftragsposition mit Modell erfassen.

**Voraussetzungen**
- Modellkatalog ist installiert, z. B. der A+W Modellkatalog.
- Auftragserfassung ist geöffnet.

**Zusatzinfo**
- Für die Preisberechnung werden die Maße des umschreibenden Rechtecks aus der Positionserfassung herangezogen.

**Workflow**

1.  Zum Register **Positionen > Allgemein** wechseln.
2.  Artikel erfassen.
3.  Feld **Breite**: `<Strg>+<F12>` drücken. Neben der Grafik wird das Feld **Modell** angezeigt.
4.  Modellnummer eingeben oder mit `<F2>` auswählen. Dialog **Modell-Maßangaben** wird geöffnet.
5.  Maße für alle angezeigten Längen eingeben. Restriktion beachten, z. B. für W (Breite) und H (Höhe).
6.  Angaben mit `[OK]` übernehmen. Die Position wird mit dem Modell-Icon gekennzeichnet. Das Modell wird im Grafikbereich maßstabsgerecht angezeigt.
7.  Position speichern.
8.  Erfassung fortsetzen oder Auftrag speichern und beenden.

### VK 03-005: Bearbeitung erfassen

**Ziel der Handlung**
- Bearbeitung manuell erfassen.

**Voraussetzungen**
- Auftragserfassung ist geöffnet.
- Bearbeitungsartikel sind angelegt.

**Zusatzinfo**
- Auf die gleiche Weise werden alle Bearbeitungen angefügt.
- Bei unsymmetrischen Ausschnitten jeden Ausschnitt als separate Bearbeitung erfassen.
- Bei ISO-Scheiben Bearbeitung, z. B. Siebdruck, für jede Scheibe separat erfassen.
- Stückliste öffnen: in Feld Artikel mit `<Shift>+<F5>`, in Feld Menge mit `<F5>`.
- ⇨ Bearbeitung aus SN-Datei übernehmen

**Workflow**

1.  Register **Positionen > Allgemein** > Position erfassen.
2.  Dialog **Stücklistendarstellung** öffnen: in Feld **Menge** `<F5>` drücken.
3.  Stücklistenbaum: Ebene auswählen.
4.  Neue Zeile einfügen: `<F6>` drücken.
5.  Bearbeitung suchen: `[A-Suche]`.
6.  Bearbeitung auswählen, z. B. Eckausschnitt, und übernehmen.
7.  Maße eingeben: `[Parameter]`.
8.  Checkboxen markieren für die Ecken, die denselben Ausschnitt erhalten sollen.
9.  Werte für Eckausschnitte angeben:
    - Abstände A und B.
    - Bezugskante, z. B. senkrecht.
    - Abrundung für die Ausschnitte Radius innen und Radius außen.
10. Angaben prüfen, ggf. korrigieren: mit `[Skizze]` Produktskizze öffnen.
11. Werte mit `[OK]` übernehmen. Produktskizze wird geschlossen.
12. Ggf. Schritte 3 bis 11 für weitere Bearbeitungen wiederholen.
13. Bearbeitung mit `[OK]` abschließen. Dialog **Auftragserfassung** wird geöffnet.
14. Position speichern.
15. Erfassung fortsetzen oder Auftrag speichern und beenden.
