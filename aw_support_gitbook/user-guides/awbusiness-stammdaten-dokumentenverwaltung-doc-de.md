---
title: "D-AWBusiness-HB_6"
source: "D-AWBusiness-HB_6.pdf"
tags: ["A+W Business", "Stammdaten", "Dokumentenverwaltung", "Statusvergabe", "Sperrkennzeichen", "Nummernkreise", "Rundungen", "Faktura", "Formulardruck", "Tutorial"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A technical tutorial (Tutorial 2) for the A+W Business software, covering document status management, lock indicators, number ranges, rounding rules, and invoice settings in the master data module."
long_description: "This document is a technical tutorial (Tutorial 2) for the A+W Business software, focusing on master data management for documents. It covers several key areas:
- **Status Management**: How to control document workflows using status points, including automatic, manual, and lock statuses. It details the process of status assignment and the use of lock indicators to prevent certain actions.
- **Lock Indicators (Sperrkennzeichen)**: Explains how to use lock indicators to block documents for specific processes (like invoicing for partial deliveries) and redirect them to different workflow steps.
- **Number Ranges (Nummernkreise)**: Describes the setup and function of number ranges for various document types (offers, orders, invoices) to ensure unique identification. It covers assigning ranges per client, business area, or even employee.
- **Rounding Rules (Rundungen)**: Details the configuration of rounding for prices, taxes, and other values. It explains rounding points (what is rounded), rounding methods (commercial, up, down), and how to create specific rounding rules for different market partners or product groups.
- **Invoice Settings (Einstellungen zur Faktura)**: Covers the financial data required for invoicing, such as tax rates, currencies, and payment terms.
- **Text and Document Printing**: Explains how to manage standardized texts, use variables and formulas in documents, and configure form printing, including direct printing and print jobs.
The tutorial provides step-by-step instructions, examples, and screenshots to guide the user through configuring these settings in the A+W Business Stammdaten module."
---

---
## Tutorial 2: Dokumente

### Sperrstatus

Bei jeder Zuordnung können Sie einen Sperrstatus (F) angeben, um die Abläufe weiter zu steuern. In diesem Beispiel ist der gleiche Anwenderstatus (D) angegeben, was bedeutet, dass die Rechnung nicht nochmals als Original gedruckt werden kann.

Neben dem Sperrstatus kann für Reklamationen und Teillieferungen ein Sperrkennzeichen gesetzt werden.

⇨ "Sperrkennzeichen" auf Seite B-433

### Statusvergabe

Der Status wird automatisch hochgesetzt, sobald das Dokument einen bestimmten Statuspunkt erreicht hat und die zugehörige Aktion ausgelöst wurde.

**Tab. B-20: Beispiele für Statuszuordnungen**

| Anwenderstatus | Dokument-Typ | Mind.-status | Sperr-status | Statuspunkt | Prozessname | Nr. |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 001 Dokument erfassen | Alle | | | | Dokument erfasst | 001 |
| 020 Dokument geändert | Alle | 001 | 750 | Dokument geändert | 002 |
| 200 Bestätigung gedruckt | Auftrag | 001 | 200 | AB-Druck | 100 |
| 300 Auftrag an Einkauf übergeben | Auftrag | 180 | 540 | Übergabe Bestellpool | 030 |
| 390 Auftrag für Produktion freigegeben | Auftrag | 001 | 390 | Produktionsfreigabe | 035 |
| 360 Wareneingang komplett/Auftrag | Auftrag | 030 | 360 | Wareneingang komplett/Auftrag | 034 |
| 450 Auftrag an Produktion übergeben | Auftrag | 400 | | Übergabe Produktion | 045 |
| 600 Lieferschein gedruckt | Auftrag | 400 | 600 | Lieferschein Druck | 102 |
| 750 Rechnung gedruckt | Auftrag | 600 | 750 | Rechnung Druck | 103 |
| 800 FiBu-Daten übergeben | Alle | 750 | 800 | Übergabe FiBu | 097 |
| 850 Übergabe Statistik | Alle | 800 | 850 | Übergabe Statistik | 500 |
| 990 Übergabe Archiv | Alle | 850 | 900 | Übergabe Archiv | 501 |
| 990 Löschfreigabe | Alle | 900 | 990 | Löschfreigabe | 502 |
| 995 Dokument gelöscht | Alle | 990 | | Dokument gelöscht | 503 |

In diesem Beispiel sehen Sie, wie der Status eines Auftrags bei der Verarbeitung umgesetzt wird. Für die Übergabe an die Bestellung (Einkauf) ist als Mindeststatus angegeben, dass der zugehörige Fertigungsschein gedruckt sein muss. Der Sperrstatus legt fest, dass das Dokument nach der Fertigung gesperrt ist und nicht nochmals übergeben werden kann. In der ersten Spalte ist die Reihenfolge zu sehen, in der das Dokument die Bearbeitungen durchläuft.

### Manuelle Statusvergabe

Für besondere Abläufe kann festgelegt werden, dass der Status manuell vergeben werden muss. In diesem Fall muss ein manueller Statuspunkt eingerichtet werden. Ein manueller Statuspunkt kann einem Dokument nur manuell vergeben werden. Er setzt das automatische Hochsetzen des Status außer Kraft.

**Beispiel**
Einen manuellen Statuspunkt setzen Sie z. B. dann, wenn eine Rechnung erst nach einer (manuellen) Prüfung gedruckt werden darf. Der Status eines Auftrags muss dabei nach der Prüfung manuell hochgesetzt werden, damit die Rechnung gedruckt werden kann.

Für die manuelle Statusvergabe sind folgende Schritte erforderlich:
*   Neuen Statuspunkt mit Nummer >10.000 anlegen.
*   Anwenderstatus im Geschäftsablauf festlegen.
*   Anwenderstatus dem Statuspunkt zuordnen.

> **Statuspunkt anlegen**
> Wenn Sie neue Statuspunkte anlegen und zuordnen wollen, lassen Sie sich von Ihrem Service-Mitarbeiter bei der A+W Software GmbH unterstützen. Sie vermeiden damit ungewollte Statusumsetzungen Ihrer Dokumente.

### Statusvergabe durch BDE-Rückmeldungen

Für Rückmeldungen aus der Betriebsdatenerfassung (BDE) müssen ebenfalls gesonderte Statuspunkte eingerichtet werden. Im Gegensatz zu den manuellen Statuspunkten wird der Dokumentenstatus aber automatisch umgesetzt, wenn die Rückmeldung aus der Produktion ankommt.

Für die Statusvergabe durch BDE-Meldungen sind die gleichen Schritte erforderlich, wie bei manuellen Statuspunkten. Zusätzlich müssen aber noch die Erfassungsstellen zugeordnet werden.

Die Statusumsetzung durch die BDE-Meldungen ist im Part Fertigung beschrieben.

### Sperrkennzeichen

Mit Hilfe eines Sperrkennzeichens können Sie Dokumente für bestimmte Vorgänge sperren und gleichzeitig deren Status automatisch hochsetzen. Das bedeutet, dass das Dokument den gesperrten Status nicht erreichen kann, stattdessen aber umgeleitet wird auf einen anderen Statuspunkt (Prozess).

**Beispiel: Teillieferung ohne Fakturierung**
Wenn aus einer Teillieferung keine Teillieferungsrechnung erzeugt werden darf, wird der Status der Teillieferung automatisch hochgesetzt. Bei der Umleitung auf die Archivübergabe kann die Teillieferung anschließend nicht mehr bearbeitet werden.

*[Image: Abb. B-267 Sperrkennzeichen mit Umleitung auf anderen Status. A: Bezeichnung des Sperrkennzeichens, B: Sperrkennzeichen sperren, C: Gesperrter Status (Anwenderstatus), D: Nächstmöglicher Status]*

Sperren ist z. B. bei Teillieferungen sinnvoll, wenn die Teillieferungsaufträge nicht fakturiert werden sollen. Das Sperrkennzeichen für Teillieferungen (und für Reklamationen) wird in den Firmendaten aktiviert.

⇨ Softwarereferenz, "Firmendaten - Dokumente" auf Seite B-941

**Sperrkennzeichen sperren**
> Verwechseln Sie das Sperrkennzeichen nicht mit der Sperre durch die Checkbox Gesperrt (B). Das Sperrkennzeichen leitet ein Dokument auf einen anderen Status um. Die Checkbox Gesperrt verhindert, dass das Sperrkennzeichen verwendet wird.

### Status zuordnen

Im Dialog Statuszuordnung stellen Sie den Bezug zwischen Statuspunkt und Anwenderstatus her. Bei der Vergabe von Status, Mindeststatus und Sperrstatus sind Sie an keine Vorgaben gebunden.

> **Änderungen absprechen**
> Sprechen Sie alle Änderungen in der Statusverwaltung und Statuszuordnung zuvor mit der A+W Software GmbH ab. Sie vermeiden damit, dass das System u. U. nicht mehr richtig arbeitet.

**So ordnen Sie einen Statuspunkt zu**

1.  Wählen Sie im Menü Stammdaten > Auftrag > Statuszuordnung.

    *[Image: Abb. B-268 Statuszuordnungen. The window shows a list of status points on the left and the details for the selected status point '001 Dokument erfaßt' on the right.]*

    ⇨ Softwarereferenz, "Statuszuordnung" auf Seite B-899

2.  Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wechseln.

    *[Image: Abb. B-269 Felder für neue Zuordnung freigeschaltet. The right panel now has editable fields. A: Statuspunkt, B: Dokumententyp, C: Anwenderstatus, D: Mindeststatus, E: Sperrstatus.]*

3.  Wählen Sie den Statuspunkt (A) und den Dokumententyp (B), für den die Zuordnung gelten soll.
    Achten Sie darauf, welchen Dokumententyp Sie gewählt haben. Wenn Sie alle wählen, gilt dieser Status für alle Dokumententypen, und zwar auch dann, wenn dies sinnlos oder hinderlich ist.

4.  Wählen Sie den Anwenderstatus (C) aus, den Sie dem Statuspunkt und dem Dokumententyp zuordnen wollen.

5.  Wählen Sie ggf. zusätzlich den passenden Mindeststatus (D) und den Sperrstatus (E) aus.
    Achten Sie darauf, dass die neue Zuordnung nicht im Widerspruch zu den vorhandenen Zuordnungen steht.

6.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Daten werden gespeichert. Die neue Zuordnung wird nun in den Dokumenten als Status angewendet.

### Sperrkennzeichen zuordnen

Sperrkennzeichen setzen Sie ein, um Dokumente aus bestimmten Abläufen in der automatischen Verarbeitung auszuschließen.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So legen Sie ein Sperrkennzeichen an" auf Seite B-436
*   "So aktivieren Sie das Sperrkennzeichen” auf Seite B-439

> **Änderungen absprechen**
> Sprechen Sie Änderungen der Sperrkennzeichen zuvor mit der A+W Software GmbH ab. Sie vermeiden damit, dass das System u. U. nicht mehr richtig arbeitet.

**So legen Sie ein Sperrkennzeichen an**

1.  Wählen Sie im Menü Stammdaten > Auftrag > Sperrkennzeichen.

    *[Image: Abb. B-270 Sperrkennzeichen anlegen. The window 'Sperrkennzeichen' is shown with empty fields for a new entry.]*

    ⇨ Softwarereferenz, "Sperrkennzeichen" auf Seite B-910

2.  Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wechseln.

    *[Image: Abb. B-271 Felder für neues Sperrkennzeichen freigeschaltet. A: Bezeichnung des Sperrkennzeichens, B: Anwenderstatus, der gesperrt wird, C: Nächstmöglicher Status.]*

3.  Tragen Sie die Bezeichnung (A) ein, z. B. Teillieferung ohne Rechnung.
4.  Wählen Sie den Anwenderstatus (B) aus, der gesperrt werden soll, z. B. den Rechnungsdruck.
5.  Wählen Sie den Anwenderstatus (C) aus, auf den umgeleitet werden soll, z. B. die Übergabe an die FiBu.

    *[Image: Abb. B-272 Neues Sperrkennzeichen. The fields are filled according to the example 'Teillieferung ohne Fakturierung'.]*

6.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Das Sperrkennzeichen für die Teillieferung ohne Fakturierung wird gespeichert. Sie müssen es nun in den Firmendaten aktivieren.

**So aktivieren Sie das Sperrkennzeichen**

1.  Wählen Sie im Menü Stammdaten > Firma > Firmendaten.
    Der Dialog Firmendaten wird mit dem Register Mandant geöffnet.
2.  Wechseln Sie zum Register Dokumente.

    *[Image: Abb. B-273 Firmendaten - Dokumente. The 'Dokumente' tab of the 'Firmendaten' window is shown. A: Sperrkennzeichen für Teillieferung aktivieren.]*

    ⇨ Softwarereferenz, "Firmendaten - Dokumente" auf Seite B-941

3.  Wählen Sie im Feld Teillieferung (A) das Sperrkennzeichen aus.
4.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Daten werden gespeichert. Zu Teillieferungen kann nun keine Rechnung mehr erstellt werden. Dies gilt für alle Kunden.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Statusverwaltung" auf Seite B-897
⇨ Softwarereferenz, "Statuspunkte" auf Seite B-898
⇨ Softwarereferenz, "Statuszuordnung" auf Seite B-899
⇨ Softwarereferenz, "Sperrkennzeichen" auf Seite B-910
⇨ Softwarereferenz, "Firmendaten - Dokumente" auf Seite B-941

## Nummernkreise

**Lernziele**
*   Funktion der Nummernkreise kennenlernen.
*   Nummernbereiche einrichten.

**Nutzen**
*   Nummernkreise legen die Vergabe von eindeutigen (Dokumenten-)Nummern fest.
*   Die eindeutigen Nummern gewährleisten, dass Dokumente (und andere Laufnummern) im Geschäftsprozess korrekt weitergeleitet werden.

> **Merke**
> **Nummernkreise**
> Nummernkreise sind:
> *   Logische Organisationseinheiten.
> *   Mittel zur Zusammenfassung von Arbeitsprozessen, die durch Nummernverwalter ausgelöst werden.
> *   Nummernkreise können für Dokumente, für die Produktion und für die Finanzbuchhaltung gepflegt werden.
> *   In den einzelnen Nummernkreisen sind die Nummernfolgen (Laufnummern) festgelegt, z. B. für die Dokumente. Die Nummernkreise dürfen sich nicht überschneiden.
>
> **Basisnummernkreise**
> Die Basisnummernkreise der Stammdaten sind vorgegeben und können nicht um zusätzliche Nummernkreise erweitert werden.
>
> **Mandant, AV-Bereich, Mitarbeiter**
> Nummernkreise können für Mandanten, AV-Bereiche und für Mitarbeiter getrennt festgelegt werden. Auch diese Nummernkreise dürfen sich nicht überschneiden.
>
> **Dokumententyp**
> Die Nummern für die einzelnen Dokumententypen werden in unterschiedlichen Nummernkreisen festgelegt. Eine Dokumenten-Nummer wird beim Anlegen automatisch aus dem zugeordneten Nummernkreis vergeben.

### Funktion der Nummernkreise

Nummernkreise sind zum einen logische Organisationseinheiten, zum anderen ein Mittel zur Zusammenfassung von Arbeitsprozessen, die durch einen sogenannten Nummernverwalter ausgelöst werden.

Die Nummernkreise für die Dokumente und andere Laufnummern müssen Sie so einrichten, wie es für Ihr Unternehmen erforderlich ist. Dies gilt insbesondere für folgende Bereiche:
*   Dokumenten-Nummern
*   Produktion
*   FiBu

Die Nummernkreise können für jeden Mandanten und für jeden Bereich der Auftragsverwaltung (AV-Bereich) festgelegt werden. Auf diese Weise kann z. B. ein Dokument anhand seiner Nummer zugeordnet werden.

Für jeden Nummernkreis legen Sie fest, aus welchem Zahlenbereich die (Lauf-)Nummern vergeben werden können.

*[Image: Abb. B-274 Nummernkreise. The window shows number ranges for different document types. A: Bereiche für Nummernkreise, B: Dokumententypen, C: Erste mögliche Nummer, D: Zuletzt vergebene Nummer, E: Letzte mögliche Nummer, F: Anzahl der vergebenen Nummern.]*

In diesem Beispiel sehen Sie die Nummernkreise für Dokumente. Pro aufgeführtem Dokumententyp (B) können Sie festlegen, welche Nummernbereiche (C, E) vergeben werden sollen. Eine Dokumenten-Nummer wird automatisch aus dem zugeordneten Nummernkreis vergeben, wenn Sie ein Dokument anlegen. Damit diese Nummer eindeutig ist, dürfen sich die Nummernkreise nicht überschneiden. Dies gilt für alle Nummernkreise, also für Dokumenten-Nummern, FiBu-Nummern und Produktionsnummern.

### Nummern für Dokumente

Einzelne Nummernkreise können gesperrt werden. Damit können Sie steuern, dass bestimmte Dokumente für gesonderte Bereiche nicht erfasst werden können.

**Tab. B-21: Beispiel für Nummernkreise**

| Dokumente | ESG-Fertigung | VSG-Fertigung | <k.A.> |
| :--- | :--- | :--- | :--- |
| | **von** | **bis** | **von** | **bis** | **von** | **aktuell** | **bis** |
| Angebote | 300 | 19.999 | 20.000 | 39.999 | 0 | 1 | 0 |
| Aufträge | 100.000 | 199.999 | 200.000 | 299.999 | 0 | 1 | 0 |
| Bestellungen | 300.000 | 399.999 | 400.000 | 499.999 | 0 | 1 | 0 |
| Bestellanfragen | 500.000 | 599.999 | 600.000 | 699.999 | 0 | 1 | 0 |
| Rechnungen | 700.000 | 799.999 | 800.000 | 899.999 | 0 | 1 | 0 |
| Gutschriften | 100 | 199 | 200 | 299 | 0 | 1 | 0 |
| Lieferscheine | 40.000 | 49.999 | 50.000 | 99.999 | 0 | 1 | 0 |
| **Produktion** | | | | | | | |
| Laufnummer AWPOOL | 0 | 0 | 0 | 0 | 1 | 1 | 9.999 |
| Teillieferung | 2.000.000 | 2.099.999 | 3.000.000 | 3.099.999 | 0 | 1 | 0 |
| Reklamation bei Bruch | 2.100.000 | 2.199.999 | 3.100.000 | 3.199.999 | 0 | 1 | 0 |
| **FiBu** | | | | | | | |
| Laufnummer FiBu | 0 | 0 | 0 | 0 | 1 | 1 | 99.999.999 |

In diesem Beispiel werden Dokumente in den AV-Bereichen ESG-Fertigung und VSG-Fertigung erfasst. Außerhalb dieser Bereiche können keine Dokumente erfasst werden.
*   Im AV-Bereich ESG-Fertigung liegt der Nummernbereich für das Dokument Aufträge im Bereich 100.000 bis 199.999. Für die Teillieferung ist der Bereich 2.000.000 bis 2.099.999 und für die Reklamationen der Bereich 2.100.000 bis 2.199.999 reserviert. Eine Überschneidung ist damit ausgeschlossen.
*   Standardmäßig existiert der AV-Bereich <k.A.>, für den aber keine Aufträge erfasst werden sollen. Der Nummernkreis ist daher durch die Werte 0 (von) und 0 (bis) gesperrt. Die 1 (aktuell) steht für ein leeres Dokument.
*   Die Laufnummer AWPOOL soll immer fortlaufend vergeben werden, unabhängig davon, um welchen AV-Bereich es sich handelt. In diesem Fall wird der Nummernbereich (1 bis 9999) im AV-Bereich <k.A.> angegeben. Alle anderen AV-Bereiche werden gesperrt.

Teillieferungen und Reklamation gehören zum Dokumententyp Aufträge. Daher dürfen sich deren Nummernkreise nicht überschneiden. Auch für Gutschriften und Rechnungen werden einzelne Nummernkreise gepflegt. Als Sonderfunktion kann für diese beiden Dokumentenarten denselben Nummernkreis verwendet werden.
⇨ Softwarereferenz, “Gutschrift-Rechnungsnummer" auf Seite B-944

Für Dokumente besteht zusätzlich die Möglichkeit, unterschiedliche Nummernkreise pro Mitarbeiter zu definieren. Wenn Sie mit verschiedenen AV-Bereichen arbeiten, können Sie z. B. dem Mitarbeiter der Dokumentenerfassung den AV-Bereich zuordnen, für den er zuständig ist.
⇨ Softwarereferenz, "Erfassungsparameter" auf Seite B-1027

> **Weitere Nummernkreise**
> Die Basisnummernkreise der Stammdaten sind standardmäßig vorgegeben und können nicht erweitert werden. Diese Nummernkreise sind im Dialog Basisnummernkreise aufgelistet.
> Der Nummernkreis für die Verwaltung der Gestelle wird im Dialog Firmendaten festgelegt.
> ⇨ Softwarereferenz, “Firmendaten – Versand" auf Seite B-1008

### AV-Bereiche

Zur Auftragsverwaltung können sogenannte AV-Bereiche definiert werden, denen die Aufträge zugeordnet werden.

Beispielsweise können AV-Bereiche eingerichtet werden, um Neukunden abzugrenzen oder um interne Aufträge zu verwalten. Über Schnittstellen können die Aufträge dann automatisch an den betreffenden AV-Bereich zur Produktion weitergeleitet werden. Der AV-Bereich dient außerdem als Sortierkriterium in der Umsatzstatistik.

*[Image: Abb. B-275 AV-Bereiche. A: Name des AV-Bereichs, B: Erlaubte Dokumententypen]*

Typischerweise beziehen sich AV-Bereiche auf einzelne Abteilungen oder Niederlassungen eines Unternehmens, mit denen standardmäßig zusammengearbeitet wird. Der AV-Bereich ESG-Herstellung ist z. B. zuständig für die Herstellung von ESG.

Jedem AV-Bereich müssen eigene Nummernkreise zugeordnet sein, damit die Dokumente korrekt weitergeleitet werden.

Zusätzlich kann jedem Mitarbeiter ein AV-Bereich und Dokumententyp zugeordnet werden. Wenn beispielsweise der AV-Bereich ISO (A) nur dafür gilt, fertige ISO-Einheiten (Lagerartikel) zu verwalten, dann muss ihm der Dokumententyp (B) Produktionsauftrag zugewiesen werden. Die Aufträge werden dann automatisch in diesem AV-Bereich und dem dazugehörigen Nummernkreis erfasst. Beides kann manuell im jeweiligen Auftrag geändert werden.

⇨ Softwarereferenz, "Erfassungsparameter" auf Seite B-1027
AV-Bereiche richten Sie nach demselben Muster ein, wie alle Basistabellen.
⇨ Tutorial 1, "Basistabelle erweitern" auf Seite B-34

> **AV-Bereiche für die unterschiedlichen Mandanten**
> Legen Sie alle AV-Bereiche fest, die von Ihren Mandanten benötigt werden. Erst beim Einrichten der Nummernkreise werden die AV-Bereiche dem jeweiligen Mandanten zugeordnet. Mandanten werden in einer separaten Einheit beschrieben.
> ⇨ Tutorial 1, "Mandanten und Filialen" auf Seite B-379

### Nummernkreise festlegen

Die Nummernkreise dürfen sich nicht überschneiden. Daher werden die Nummernkreise für jede Dokumentenart einzeln festgelegt, um so z. B. Auftrags- und Rechnungsnummern voneinander zu unterscheiden.

> **Nummernkreis nicht im laufenden Betrieb ändern**
> Wenn Sie die Nummernkreise im laufenden Betrieb ändern, kann das zu Konflikten mit alten Dokumenten-Nummern führen. Prüfen Sie bitte vorher sorgfältig, dass keine unverarbeiteten Dokumente in den Nummernverwaltern stehen.

> **Voraussetzung**
> Wenn Sie mit Mandanten arbeiten, müssen diese angelegt sein, bevor Sie die Nummernkreise einrichten. Legen Sie sich einen Schulungsmandanten auch dann an, wenn Sie in ihrem Geschäftsbetrieb nicht mit Mandanten arbeiten. Sie können ihn nach den Übungen wieder löschen.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So legen Sie die Nummernkreise fest" auf Seite B-445
*   "So sperren Sie einen Nummernkreis für einen AV-Bereich" auf Seite B-447

**So legen Sie die Nummernkreise fest**

1.  Wählen Sie im Menü Stammdaten > Auftrag > Nummernkreise.
    Der Dialog Nummernkreise wird geöffnet.
    ⇨ Softwarereferenz, "Nummernkreise" auf Seite B-903
    Prüfen und notieren Sie, welche Nummernfolgen noch nicht belegt sind. Wenn Sie keine „Lücken" entdecken können, dann reduzieren Sie die Nummernfolgen des aktuellen Mandanten.
    Unter Umständen können Sie die höheren Nummernfolgen freimachen, z. B. zwischen 100000 und 99999999.
2.  Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wechseln.

    *[Image: Abb. B-276 Felder für neue Nummernkreise freigeschaltet. A: Mandant auswählen, B: AV-Bereich auswählen, C: Mitarbeiter auswählen, D: Nummernfolge festlegen]*

    ⇨ Softwarereferenz, “Nummernkreise" auf Seite B-903
    Die Nummernfelder sind mit den Werten vorbelegt, die für den ersten Mandanten reserviert wurden.

3.  Wählen Sie ggf. den Mandanten (A) aus, z. B. Ihren Schulungsmandanten.
4.  Wählen Sie als AV-Bereich (B) und Mitarbeiter (C) jeweils den Eintrag <k.A.> aus.
5.  Tragen Sie für Angebote (D) in den Feldern von und bis die Nummern ein. Die Nummern können bis zu 8 Stellen haben.
    Wenn Sie für die gewählte Kombination von Mandant, AV-Bereich und Mitarbeiter die Erfassung sperren wollen, so geben in den Feldern von und bis jeweils den Wert 0 ein und im Feld aktuell den Wert 1.
6.  Wiederholen Sie diesen Schritt für alle Dokumente.
7.  Wählen Sie im Menü Funktionen > Prüfung.
    Wenn Überschneidungen mit anderen Nummernkreisen festgestellt wurden, wird eine Meldung angezeigt.

    *[Image: Meldung [1720]. A dialog box showing overlap errors between number ranges.]*

    In der Meldung können Sie sehen, mit welchen Nummernkreisen Konflikte entstanden sind.
8.  Korrigieren Sie Ihre Einträge, bis bei der Prüfung keine Fehler mehr gemeldet werden.
9.  Wiederholen Sie die Schritte 5 und 7 in den anderen Registern, um weitere Laufnummern einzutragen.
    Im Register Tabelle können Sie prüfen, welche Nummernkreise Sie bereits definiert haben.
10. Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Daten werden gespeichert.

**So sperren Sie einen Nummernkreis für einen AV-Bereich**

1.  Wählen Sie im Menü Stammdaten > Auftrag > Nummernkreise.
2.  Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wechseln.
3.  Wählen Sie den AV-Bereich aus.
4.  Tragen Sie für Angebote in den Feldern von und bis den Wert 0 ein.
5.  Geben im Feld aktuell den Wert 1 ein.
6.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Daten werden gespeichert. Damit können im gewählten AV-Bereich keine Angebote erfasst werden. Wiederholen Sie die Schritte für alle Dokumententypen, die in dem AV-Bereich nicht erfasst werden dürfen.

### Übungen

Um die Nummernfolgen in dieser Übung zu bearbeiten, benötigen Sie einen neuen (eigenen) Mandanten. Mandanten werden in den Firmendaten angelegt. Dazu gibt es eine separate Einheit. Die folgende Handlungssequenz ist daher stark verkürzt.

**So legen Sie einen Mandanten für die Übung an**

1.  Wählen Sie im Menü Stammdaten > Firma > Firmendaten.
    Der Dialog Firmendaten wird geöffnet.
2.  Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wechseln.
    Die Felder werden freigeschaltet.
3.  Tragen Sie die Nummer, den Matchcode und den Namen ein.
4.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Daten werden gespeichert.

**Legen Sie die Nummernkreise für Ihren Schulungsmandanten fest.**
*   Notieren Sie, welche Nummern bereits für Dokumente reserviert sind.
*   Legen Sie die Nummernfolgen für Dokumente fest.
*   Prüfen Sie, ob es Überschneidungen gibt, und korrigieren Sie diese ggf.
*   Erfassen Sie einen Auftrag für diesen Mandanten und prüfen Sie, ob die Auftragsnummer aus dem richtigen Nummernkreis genommen wurde.

**Ergänzende Informationen**
⇨ Tutorial 1, "Finanzbuchhaltung (FiBu)" auf Seite B-377
⇨ Softwarereferenz, "Nummernkreise" auf Seite B-903
⇨ Softwarereferenz, "Firmendaten - Mandant" auf Seite B-931
⇨ Softwarereferenz, "AV-Bereiche" auf Seite B-1033

## Rundungen

**Lernziele**
*   Rundungseinstellungen prüfen.
*   Rundungen zuordnen.
*   Rundungen für einzelne Marktpartner einrichten.

**Nutzen**
*   Im Programm errechnete Werte können auf eine gewünschte Anzahl von Stellen gerundet werden.
*   Die Rundungseinstellungen beziehen sich immer auf einen bestimmten Rundungspunkt. Sie können daher sehr fein abgestimmt werden.

> **Merke**
> **Rundungssatz**: Im Rundungssatz sind folgende Einstellungen enthalten:
> *   Anzahl der verbleibenden Nachkommastellen.
> *   Wert, auf den gerundet wird (letzte, beizubehaltende Stelle).
> *   Rundungsart.
>
> **Rundungsart**: Die Rundungsart gibt an, ob auf- oder abgerundet wird.
>
> **Rundungspunkt**: Rundungspunkte geben an, was gerundet werden soll. Die Rundungspunkte sind fest vorgegeben und können nicht bearbeitet werden.
>
> Gerundet werden in der Regel:
> *   Preise
> *   Zuschläge
> *   Steuerbeträge
> *   Flächen
>
> **Rundungszuordnung**: Rundungspunkte und Rundungen müssen einander zugeordnet werden, damit der errechnete Wert gerundet wird.
>
> Die allgemeinen Zuordnungen können für bestimmte Produktgruppen gelten. Für einzelne Partner oder Partnergruppen können abweichende Rundungen zugeordnet werden.

### Rundung

Zur Berechnung der Rundungen werden folgende Einstellungen herangezogen:
*   Die Rundung selbst: Sie gibt die Anzahl der Stellen und die Rundungsart an, wie gerundet werden soll, z. B. nach oben.
*   Der Rundungspunkt: Er gibt an, was gerundet werden soll, z. B. Preis, Steuer, Fläche.

*[Image: Abb. B-277 Rundung. A: Rundungswert, B: Stellen, auf die gerundet wird, C: Rundungsart]*

In diesem Beispiel sehen Sie, dass neben der Rundungsart (C) auch angegeben ist, auf wie viele Stellen (B) und auf welchen Wert (A) die Zahl gerundet werden soll.

Bei der Rundungsart haben Sie die folgenden Möglichkeiten zur Rundung:
*   **Kaufmännisch:** Die Beträge von 0 bis 4 werden abgerundet, von 5 bis 9 aufgerundet.
*   **Nach oben:** Die Ziffern von 1 bis 9 werden aufgerundet.
*   **Nach unten:** Die Ziffern von 1 bis 9 werden abgerundet.

**Tab. B-22: Rundungsbeispiele für zwei Stellen**

| Rundungs-wert | Stellen | Beispiel-wert | Rundungsart - kaufmännisch | Rundungsart - nach oben | Rundungsart - nach unten |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 2 | 10,2237 | 10,22 | 10,23 | 10,22 |
| 1 | 2 | 10,2279 | 10,23 | 10,23 | 10,22 |
| 5 | 2 | 10,2237 | 10,20 | 10,25 | 10,20 |
| 5 | 2 | 10,2421 | 10,25 | 10,25 | 10,20 |
| 10 | 2 | 10,2237 | 10,20 | 10,30 | 10,20 |
| 10 | 2 | 10,2711 | 10,30 | 10,30 | 10,20 |
| 20 | 2 | 10,2237 | 10,20 | 10,40 | 10,20 |
| 20 | 2 | 10,3392 | 10,40 | 10,40 | 10,20 |
| 50 | 2 | 10,2237 | 10,00 | 10,50 | 10,00 |
| 50 | 2 | 10,4566 | 10,50 | 10,50 | 10,00 |
| 100 | 2 | 10,2237 | 10,00 | 11,00 | 10,00 |
| 100 | 2 | 10,6389 | 11,00 | 11,00 | 10,00 |

In diesen Beispielen sehen Sie, zu welchen Ergebnissen die unterschiedlichen Runden der verschiedenen Rundungswerte führen.

### Rundungspunkte

Die Rundungspunkte geben an, was gerundet werden soll, z. B. der Preis für die Fläche, der Preis für die Bearbeitung, der Zuschlag. Rundungspunkte sind in A+W Business fest definiert und können nicht bearbeitet werden.

In der folgenden Tabelle finden Sie alle Rundungspunkte, die für die Berechnungen von Verkaufspreisen herangezogen werden. In der Spalte Beschreibung ist jeweils das Beispiel angegeben, in dem Sie diesen Rundungspunkt in den abgebildeten Beispieldialogen wiederfinden.

**Tab. B-23: Rundungspunkte (Abschnitt 1 und 2 von 2)**

| Nr. | Rundungspunkte VK | Nr. | Rundungspunkte EK | Beschreibung |
| :--- | :--- | :--- | :--- | :--- |
| 1 | qm-Preis/ME Glasposition | 51 | EK qm-Preis/ME Glasposition | Beispiel 2 |
| 2 | qm-Preis/ME Zuschläge | 52 | EK qm-Preis/ME Zuschläge | Beispiel 3 |
| 3 | qm-Preis/ME Bearbeitungen | 53 | EK qm-Preis/ME Bearbeitungen | Beispiel 3 |
| 4 | Brutto/Stk. Glasposition | 54 | EK Brutto/Stk. Glasposition | Bruttopreise werden nicht angezeigt. |
| 5 | Brutto/Stk. Zuschläge | 55 | EK Brutto/Stk. Zuschläge |
| 6 | Brutto/Stk. Bearbeitungen | 56 | EK Brutto/Stk. Bearbeitungen |
| 7 | Brutto/Stk. Stück Glasposition | 57 | EK Brutto/Stk. Stück Glasposition |
| 8 | Brutto/Stk. Stück Zuschläge | 58 | EK Brutto/Stk. Stück Zuschläge |
| 9 | Brutto/Stk. Stück Bearbeitungen | 59 | EK Brutto/Stk. Stück Bearbeitungen |
| 10 | Netto/Stk. Glasposition | 60 | EK Netto/Stk. Glasposition | Beispiel 2 |
| 11 | Netto/Stk. Zuschläge | 61 | EK Netto/Stk. Zuschläge | Beispiel 3 |
| 12 | Netto/Stk. Bearbeitungen | 62 | EK Netto/Stk. Bearbeitungen | Beispiel 3 |
| 13 | Gesamtpositions-Netto Glasposition * | 63 | EK Gesamtpositions-Netto Glasposition | |
| 14 | Gesamtpositions-Netto Zuschläge | 64 | EK Gesamtpositions-Netto Zuschläge | Beispiel 3 |
| 15 | Gesamtpositions-Netto Bearbeitungen | 65 | EK Gesamtpositions-Netto Bearbeitungen | Beispiel 3 |
| 16 | Qm-Fläche ISO | | | Beispiel 2 |
| 17 | Qm-Fläche sonstige Produkte | | | Beispiel 2 |
| 18 | MWST. 1 | | | Beispiel 1 |
| 19 | MWST. 2 | | | Beispiel 1 |
| 20 | Sonstiges | | | |
| 21 | Netto/Stk. Stück Glasposition | 71 | EK Netto/Stk. Stück Glasposition | Beispiel 2 |
| 22 | Netto/Stk. Stück Zuschläge | 72 | EK Netto/Stk. Stück Zuschläge | Beispiel 3 |
| 23 | Netto/Stk. Stück Bearbeitungen | 73 | EK Netto/Stk. Stück Bearbeitungen | Beispiel 3 |
| 24 | Gesamtpositions-Netto Stück Glasposition * | 74 | EK Gesamtpositions-Netto Stück Glasposition | |
| 25 | Gesamtpositions-Netto Stück Zuschläge | 75 | EK Gesamtpositions-Netto Stück Zuschläge | Beispiel 3 |
| 26 | Gesamtpositions-Netto Stück Bearbeitungen | 76 | EK Gesamtpositions-Netto Stück Bearbeitungen | Beispiel 3 |
| 27 | Gesamtpositions-Netto Endpreis | 77 | EK Gesamtpositions-Netto Endpreis | Beispiel 2 |
| 28 | Endbetrag ohne MwSt. | 78 | EK Endbetrag | Beispiel 1 |
| 79 | HKK Detailkalkulation | | | Herstellkosten-Kalkulation |
| 118 | FW MWST. 1 ** | | | Beispiel 1 |
| 119 | FW MWST. 2 | | | Beispiel 1 |
| 128 | FW Endbetrag ohne Mwst. | | | Beispiel 1 |
* Dieser Preis wird nicht angezeigt. Er ergibt sich aus Nettopreis x Positionsmenge.
** FW = Fremdwährung

### Beispiele für Rundung

In den folgenden Beispielen werden die Zuordnungen der Rundungspunkte zu den Feldern der Dokumentenerfassung verdeutlicht.

Die roten Zahlen verweisen auf die entsprechenden Nummern in der Spalte der Rundungspunkte für den Verkauf, die blauen auf die Spalte für den Einkauf.

**Beispiel 1**
*[Image: Abb. B-278 Beispiel 1: Auftrag - Register Summen. The summary tab shows rounding points 28, 128 for net/gross amounts and 18, 19, 118, 119 for taxes.]*

**Beispiel 2**
*[Image: Abb. B-279 Beispiel 2: Positionserfassung – Register ISO/Artikel. The item entry tab shows rounding points 27 for net price and 10, 16/17, 21 for quantity/price calculations.]*

**Beispiel 3**
*[Image: Abb. B-280 Beispiel 3: Positionserfassung – Register Stückliste. The bill of materials tab shows various rounding points for surcharges and net prices (2/3, 11/12/22/23, 14/15/25/26, 17).]*

### Rundungszuordnung

Die definierten Rundungen und die Rundungspunkte müssen einander zugeordnet werden. Dabei können die Zuordnungen für Produktarten/Produktgruppen, für Mandanten und für Partner unterschiedlich definiert werden.

Die im Dialog Rundungszuordnung festgelegten Zuordnungen gelten für alle Berechnungen eines Mandanten, es sei denn, sie werden von Zuordnungen für Kunden oder Lieferanten übersteuert.

*[Image: Abb. B-281 Standardzuordnung von Rundungen pro Mandant. A: Mandant, B: Rundungspunkt, C: Rundung auf Nettopreise, D: Verweis auf Rundung (Wert, Stellen, Rundungsart).]*

In diesem Beispiel sehen Sie, dass in der markierten Zeile der berechnete Flächenpreis auf drei Stellen nach dem Komma gerundet wird. Diese Einstellung gilt für alle Produktarten und Produktgruppen.

> **Maßrundungen**
> Maßrundungen sind von den Rundungseinstellungen nicht betroffen. Sie werden in verschiedenen Dialogen zur Produkt- und Preisdefinition angegeben. Das Programm sucht in der Reihenfolge Individualpreise > Rabatte > Preise > Produkte > Partner nach Angaben. Die Suche wird beendet, sobald eine Angabe gefunden wurde.

### Rundung für Marktpartner

Neben den allgemeinen Rundungszuordnungen können weitere Rundungssätze angelegt und diese einzelnen Kunden oder Lieferanten zugeordnet werden. So müssen z. B. bei Währungen, deren kleinste Münzeinheit 0,05 ist, Geldbeträge immer entsprechend gerundet werden.

Bei Schweizer Kunden wird z. B. die Mehrwertsteuer gerundet (5 Rappen). Dafür müssen Sie einen entsprechenden Satz anlegen und Ihren Schweizer Kunden zuordnen.

*[Image: Abb. B-282 Zuordnung von Rundungen pro Kunde. A: Kunde, für den die Einstellungen gelten, B: Abweichende Rundungen, C: Rundung auf Nettopreise.]*

In diesem Beispiel sehen Sie, dass für den ausgewählten Kunden eine eigene Rundung verwendet werden soll, wenn das erfasste Produkt ein ISO ist. Bei allen anderen Produkten gelten für ihn die allgemeinen Rundungszuordnungen.

### Rundung zuordnen

Rundungszuordnungen müssen in der Regel nur bei Änderungen neu festgelegt werden, z. B. für einen neuen Kunden oder einen neuen Mandanten. In der nachfolgenden Anleitung ist die gesamte Abfolge der Definition beschrieben, also wie Sie einen Rundungssatz anlegen und ihn zuordnen.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So legen Sie eine Rundung an" auf Seite B-457
*   "So ordnen Sie eine Rundungstabelle zu" auf Seite B-458

**So legen Sie eine Rundung an**

1.  Wählen Sie im Menü Stammdaten > Auftrag > Rundung.
    Der Dialog Rundung wird geöffnet. Wenn Sie einen Rundungssatz ändern wollen, können Sie die betreffenden Zellen einfach überschreiben.

2.  Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wechseln.

    *[Image: Abb. B-283 Felder für neuen Rundungssatz freigeschaltet. A: (Sprechende) Bezeichnung, B: Rundungswert, C: Stellen, D: Art der Rundung.]*

    ⇨ Softwarereferenz, "Rundung" auf Seite B-893

3.  Tragen Sie die Bezeichnung (A) ein.
    Wählen Sie einen sprechenden Namen, z. B. MwSt. Schweiz.

4.  Tragen Sie den Rundungswert (B) ein, auf den gerundet werden soll, z. B. 0,05.

5.  Tragen Sie die Anzahl der Stellen (C) ein, z. B. 2.

6.  Wählen Sie die Rundungsart (D) aus, z. B. kaufmännisch.

7.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Daten werden gespeichert. Sie können diese Rundung jetzt bei den allgemeingültigen Rundungszuordnungen oder bei den partnerspezifischen Rundungszuordnungen auswählen. Sie wird in den entsprechenden Dialogen als Rundungstabelle bezeichnet.
    Im nachfolgenden Beispiel wird eine Zuordnung für einen Kunden beschrieben. Die Schritte gelten in analoger Weise auch für Lieferanten und Partnergruppen und für die allgemeinen Rundungszuordnungen, z. B. für einen neuen Mandanten.

**So ordnen Sie eine Rundungstabelle zu**

1.  Wählen Sie im Menü Stammdaten > Marktpartner > Kunde > Rundung.
    Der Dialog Rundung wird geöffnet. Wenn bereits Rundungszuordnungen für Kunden festgelegt wurden, werden diese Daten angezeigt.

2.  Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wechseln.

    *[Image: Abb. B-284 Felder für neue Rundungszuordnung freigeschaltet. A: Kunde, B: Rundungspunkt, C: Produktart/Produktgruppe, D: Preiseinheit, E: Rundungstabelle, F: Abweichende Rundungszuordnungen.]*

    ⇨ Softwarereferenz, "Rundung" auf Seite B-893

3.  Wählen Sie den Kunden (A) aus.
4.  Wählen Sie den Rundungspunkt (B) aus, z. B. MWST 1.
    Damit haben Sie festgelegt, dass die Mehrwertsteuer 1 gerundet werden soll. Wenn für den Kunden auch ein zweiter Steuersatz gültig ist, wird dieser nicht gerundet.
5.  Wählen Sie in den Feldern die Produktart (C) und Preiseinheit (D) aus.
    Wenn Sie z. B. <k.A> wählen, gelten die Einstellungen für diesen Kunden immer.
    In diesem Beispiel wird die Rundung der Mehrwertsteuer festgelegt. Daher spielt die Preiseinheit keine Rolle.
6.  Wählen Sie die Rundungstabelle aus, die Sie für diesen Kunden eingerichtet haben, z. B. Rundung auf 0,05.
7.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Daten werden gespeichert. Für den ausgewählten Kunden wird diese neue Rundung verwendet. Bei allen anderen Rundungspunkten gelten für ihn weiterhin die allgemeinen Rundungszuordnungen.

### Übungen

*   Prüfen Sie, welche Rundungen und Rundungszuordnungen bereits angelegt sind.
*   Ordnen Sie Ihrem Schulungsmandanten folgende Rundungen zu:
    *   Bei allen Glaspositionen soll kaufmännisch auf 3 Stellen gerundet werden.
    *   Bei allen Stück-Preisen soll immer auf 0,05 aufgerundet werden. Legen Sie diese Rundung an, wenn im Dialog Rundung noch kein entsprechender Eintrag vorhanden ist.
*   Ordnen Sie Ihrem Schulungskunden eine kaufmännische Rundung der Mehrwertsteuer auf 0,05 zu.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Rundung (Kunde, Lieferant)" auf Seite B-851
⇨ Softwarereferenz, "Rundung Kunden-, Lieferantengruppen" auf Seite B-852
⇨ Softwarereferenz, "Rundung" auf Seite B-893
⇨ Softwarereferenz, "Rundungspunkte" auf Seite B-895
⇨ Softwarereferenz, “Rundungszuordnung" auf Seite B-896

## Einstellungen zur Faktura

Neben den Einstellungen zur Preisberechnung in den Dialogen für Preise, Marktpartner, Rabatte und Rundungen werden zur Verarbeitung der Dokumente weitere Angaben benötigt, z. B. für den Zahlungsverkehr und die Berechnung der Mehrwertsteuer.
In diesem Themenblock lernen Sie, welche Einstellungen Sie dazu bearbeiten können.

Dazu gehören folgende Lerneinheiten:
*   "Finanzen" auf Seite B-462
*   "Automatische Zuschläge" auf Seite B-332

In eine Rechnung müssen mindestens folgende Bestandteile aufgenommen werden:
*   **Angaben zum Aussteller**
    *   Name und Anschrift des Unternehmens
    *   Steuernummer und/oder Umsatzsteuer-Identifikationsnummer
    Diese Angaben legen Sie im Dialog Firmendaten fest.
*   **Angaben zum Empfänger (Kunde)**
    *   Name und Anschrift
    Diese Angaben legen Sie im Dialog Partnerverwaltung fest.
*   **Angaben zur Lieferung/Leistung**
    *   Termin der Lieferung
    *   Menge und Bezeichnung der gelieferten Produkte
    *   Nettobeträge, ggf. nach Steuersätzen aufgeschlüsselt
    *   Steuerbeträge
    *   Ausstellungsdatum (= Rechnungsdatum)
    *   Eindeutige Rechnungsnummer
    Diese Angaben sind im Auftrag enthalten.

Darüber hinaus können Sie u. a. Bankverbindungen für den Druck von Überweisungsträgern und Zahlungsbedingungen hinterlegen, Währungen pflegen und Steuersätze angeben.

### Finanzen

**Lernziele**
*   Dialoge der Basisdaten für das Rechnungswesen kennenlernen.
*   Einstellungen für Zahlungsbedingungen prüfen und festlegen.

**Nutzen**
*   Alle Daten, die für die kaufmännische Rechnungslegung und für die Finanzbuchhaltung benötigt werden, werden als Basisdaten angelegt und den Marktpartnern und Produkten zugeordnet. Diese Daten werden daher nur einmal erfasst und zentral gepflegt.

> **Merke**
> **Steuersätze**: Nur die Steuern können berechnet werden, die als Steuersatz hinterlegt sind. Steuersätze werden den Produkten und den Marktpartnern zugewiesen. Sie können im Dokument überschrieben werden.
> **Währungen**: Preise können in unterschiedlichen Währungen gepflegt werden. Dabei können Aufträgen in Landeswährung (Eigenwährung) oder Fremdwährung erfasst werden. Für statistische Vergleiche wird immer die Landeswährung herangezogen. Die Währungsbeträge werden dazu von A+W Business umgerechnet.
> **Banken**: Aus den (vollständig) hinterlegten Bankdaten kann in den Partnerstammdaten die IBAN erzeugt werden.
> **Zahlungsbedingungen**: Zahlungsbedingungen werden den Marktpartnern zugewiesen. Sie können im Dokument überschrieben werden.
> **Fremdschlüssel**: In den Dialogen, in denen Daten für die Buchhaltung hinterlegt werden, verweist ein Fremdschlüssel auf die entsprechenden Buchungsfelder im Programm zur Finanzbuchhaltung (FiBu). Der Wert des Fremdschlüssels ist von der jeweiligen FiBu abhängig.

### Steuern

Für die Berechnung der Steuern in den Dokumenten müssen Steuersätze hinterlegt werden. Diese Steuersätze werden den Produkten und den Marktpartnern zugewiesen.

*[Image: Abb. B-285 Steuersätze. A: Prozentsatz der Steuer, B: Erlöskonto Debitoren, Kreditoren, C: Fremdschlüssel (je nach FiBu-Programm).]*

Sie können beliebig viele Steuersätze anlegen. In den Stammdaten der Produkte und der Marktpartner können aber nur die ersten fünf zugewiesen werden. Die zusätzlichen Steuersätze stehen dagegen auch im Dokument zur Verfügung.

Wenn Sie mit Erlöskonten (B) arbeiten, werden die Steuerbeträge standardmäßig auf das Erlöskonto der zugehörigen Warengruppe gebucht. Wenn die Steuerbeträge auf die Erlöskonten für die Steuer gebucht werden sollen, müssen Sie die Kontonummern für Debitoren und Kreditoren eintragen, die in der Finanzbuchhaltung (FiBu) geführt werden.

### Währungen

Als international agierendes Unternehmen müssen Sie mit mehr als einer Währung arbeiten. Sie können in A+W Business die Preise für den Einkauf und für den Verkauf pflegen, auch wenn diese in unterschiedlichen Währungen anfallen. Für Ihre Kunden können die Preise in den Aufträgen in der Fremdwährung ausgewiesen werden.

Zum Erfassen von Aufträgen kann A+W Business auf der Basis von zwei verschiedenen Währungseinstellungen arbeiten:
*   **Landeswährung (Eigenwährung):** Die Währung im Land Ihres Hauptsitzes. In Europa ist dies in der Regel der Euro.
*   **Fremdwährung:** Die von der Landeswährung abweichende Währung, in der z. B. im Auftrag die Preise für ausländische Kunden ausgewiesen werden.

Für statistische Vergleiche wird immer die Landeswährung herangezogen. Die Währungsbeträge werden dazu von A+W Business umgerechnet.

Für die Pflege der Preise und für die Berechnungen in den Aufträgen ergeben sich folgende Möglichkeiten:
*   Die Preislisten und Aufträge werden in der Landeswährung geführt.
*   Die Preislisten werden in der Landeswährung geführt, für ausländische Kunden können die Beträge in den Aufträgen wahlweise in Landes- oder Fremdwährung angezeigt werden. Dazu müssen die Wechselkurse für die Fremdwährungen hinterlegt und gepflegt werden.
*   Die Preislisten werden in Fremdwährung geführt, in den Aufträgen können die Beträge wahlweise in Landes- oder Fremdwährung angezeigt werden. Für interne Zwecke wird der Wechselkurs hinterlegt.

In den Firmendaten legen Sie fest, welche Währung die Grundlage für Berechnungen ist und mit welcher Währung die Aufträge erfasst werden.

*[Image: Abb. B-286 Firmendaten – Register Steuer, Währungseinstellungen. A: Währung, in der A+W Business rechnet, B: Default-Einstellung für Auftragserfassung, C: Währung der Preisanzeige im Auftrag.]*

In diesem Beispiel sehen Sie, dass die Eigenwährung (A) Euro ist. In der Regel wählen Sie als Standard-Einstellung (B) für die Erfassung von Aufträgen die Landeswährung. Wenn Sie mit Preislisten in einer anderen als der Landeswährung arbeiten, dann wählen Sie für die Anzeige der Preise (C) in der Auftragserfassung die Einstellung Euro.

#### Preisberechnung bei Fremdwährungen

Die Berechnung von Preisen kann bei Fremdwährungen zu unterschiedlichen Ergebnissen führen, wenn Mengenpreise auf unterschiedlichen Ebenen ermittelt werden. Diese Einstellung legen Sie in den Firmendaten fest.

⇨ Softwarereferenz, "Fremdwährungsbetrag aus Stückpreis x Menge bilden" auf Seite B-963

Wenn der Fremdwährungsbetrag auf der Basis der Stückliste und der Menge gebildet werden soll, können die Beträge auf folgende Arten errechnet werden:
*   Der Positionspreis wird aus dem Positionspreis in Landeswährung gebildet.

| LW Preis/PE | x Faktor | = FW Preis/PE |
| :--- | :--- | :--- |
| LW Bruttostückpreis | x Faktor | = FW Bruttostückpreis |
| LW Nettostückpreis | x Faktor | = FW Nettostückpreis |
| **LW Positionspreis** | **x Faktor** | **= FW Positionspreis** |
> Legende: LW = Landeswährung, PE = Preiseinheit, FW = Fremdwährung

*   Der Positionspreis wird aus dem Nettostückpreis in Fremdwährung gebildet.

| LW Preis/PE | x Faktor | = FW Preis/PE |
| :--- | :--- | :--- |
| LW Bruttostückpreis | x Faktor | = FW Bruttostückpreis |
| LW Nettostückpreis | x Faktor | = FW Nettostückpreis |
| **FW Nettostückpreis** | **x Menge** | **= FW Positionspreis** |
> Legende: LW = Landeswährung, PE = Preiseinheit, FW = Fremdwährung

### Wechselkurse

Die Wechselkurse hinterlegen Sie im Dialog Währungen. Wenn eine der angegebenen Währungen nicht mehr verwendet werden soll, kann sie gesperrt werden.

*[Image: Abb. B-287 Währungen. A: Wechselkurs für die Fremdwährung, B: Name der Währung, C: Währung sperren.]*

> Wie intensiv Sie diese Wechselkurse pflegen, hängt von den Bedingungen in Ihrem Unternehmen ab.
> Sie können mit besonderen Kunden eigene Umrechnungsfaktoren vereinbaren, die jeweils im Auftrag angegeben werden. Die Preise des Auftrags werden dann nicht mit dem hinterlegten Umrechnungsfaktor berechnet, sondern mit dem im Auftrag angegebenen.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Steuer" auf Seite B-916
⇨ Softwarereferenz, “Zahlungsbedingungen" auf Seite B-918
⇨ Softwarereferenz, "Banken" auf Seite B-920
⇨ Softwarereferenz, "Währung" auf Seite B-921
⇨ Softwarereferenz, "Währungseinstellungen" auf Seite B-934
⇨ Softwarereferenz, "Währungsanzeige in Auftragserfassung" auf Seite B-935

## Text- und Dokumentendruck

Zu den Dokumenten können standardisierte Texte erfasst und wahlweise in den verschiedenen Dokumenten gedruckt werden.
In diesem Themenblock lernen Sie, welche Texte zur Verfügung stehen und wie Sie den Formulardruck steuern können.

Dazu gehören folgende Lerneinheiten:
*   "Texte" auf Seite B-468
*   "Formulare" auf Seite B-479

### Texte

**Lernziele**
*   Unterschiede der Textarten für automatische Texte kennenlernen.
*   Funktion der Textkennzeichen kennenlernen.
*   Variablen in Texten einsetzen.
*   Texte hinterlegen und bearbeiten.

**Nutzen**
*   Häufig benötigte Texte können hinterlegt und in die Dokumente übernommen werden, ohne dass sie jeweils eingegeben werden müssen.
*   Variablen vervollständigen einen Text anhand der Werte, die im Dokument erfasst wurden.

> **Merke**
> **Textarten**: Automatische Texte werden nach ihrer Verwendung unterschieden:
> *   Systemtexte
> *   Standardtexte
> *   Rahmentexte
> *   Mahntexte
> *   Gütetexte
> *   CEKAL-Texte
>
> **Textkennzeichen**: Texte werden anhand des Textkennzeichens in den Dokumenten zur Auswahl gefiltert und/oder an die Schnittstellen (Produktion, FiBu) übergeben.
>
> **Variablen**: In den Texten können Variablen (Platzhalter) eingesetzt werden. Diese lesen die Werte aus den Dokumenten aus.
>
> **Formeln**: Variablen können zu Formeln zusammengestellt werden, die einen Wert im Dokument errechnen.

#### Textarten

Immer wiederkehrende Texte können Sie hinterlegen und automatisch z. B. im Dokument einfügen lassen. Bei diesen Texten wird zwischen System-, Standard- und Rahmentexten unterschieden.

Zusätzlich können Sie Mahntexte hinterlegen, die in Mahnungen mit einer Mahngebühr verknüpft werden können.

**Systemtexte**
Dies sind Texte, die fest hinterlegt sind. Sie können keine neuen Systemtexte anlegen und die vorhandenen nicht löschen.

*[Image: Abb. B-288 Systemtexte. A: Textnummer, B: Änderbarer Wortlaut.]*

Den Wortlaut eines Systemtextes können Sie sinngemäß ändern, z. B., indem Sie die Norm im Text 111 anpassen.

**Standardtexte**
Alle Texte, die häufig in Ihren Dokumenten gedruckt werden, können Sie als Standardtexte hinterlegen. Die Texte werden in verschiedenen Dialogen eingegeben, ausgewählt und/oder bearbeitet:
*   In der Formularverwaltung können die hinterlegten Texte einem Formular fest zugewiesen werden.
*   In der Partnerverwaltung können kunden- und lieferantenspezifische Texte erfasst oder fest zugeordnet werden. In der Dokumentenerfassung werden diese Texte automatisch angezeigt und können bearbeitet werden.
*   In der Auftrags- und Auftragspositionserfassung können hinterlegte Texte ausgewählt oder auftrags-, positions- oder produktbezogene Texte eingegeben werden.

**Rahmentexte**
Für jede ISO-Einheit können spezielle Rahmentexte hinterlegt und dem Produkt zugeordnet werden.
Dabei werden zwei Varianten unterschieden:
*   Im Standardtext werden Variablen (Platzhalter) angegeben, so dass der Rahmentext anhand der Werte aus dem Dokument gebildet wird. Der aus den Variablen resultierende Text kann bis zu 80 Zeichen lang sein. Diese Variante setzt voraus, dass der Rahmenbieger in der Produktion die Übertragung von Texten zulässt.
*   Pro ISO-Einheit wird eine feste Nummer an den Rahmenbieger übergeben. In diesem Fall legen Sie Standardtexte an, die nur die Rahmennummer für den Rahmenbieger enthalten. Diese Nummer wird dann dem Produkt zugeordnet. Anhand der übergebenen Nummer setzt der Rahmenbieger automatisch den richtigen Text ein.

**Mahntexte**
Als Mahntext kann nur definiert werden, in welcher Art und Weise der Kunde gemahnt werden soll, z. B. ohne Mahntext, normal, hart, usw. Das Kennzeichen wird an die Finanzbuchhaltung übergeben.

**Gütetexte**
Für die Gütetexte gibt es pro Land unterschiedliche Anforderungen. Diese Texte hinterlegen Sie mit den entsprechenden Angaben.
Wenn Sie im Auftrag einen ISO-Aufbau erfassen, werden das Produkt, das Gas und die Produktart bzw. Produktgruppe geprüft. Anhand des Landeskennzeichens der Lieferadresse wird der entsprechende Gütetext in den Rahmentext eingefügt.
Enthält eine ISO-Einheit zwei Gläser, für die jeweils ein Gütetext hinterlegt ist, so wird über die festgelegte Priorität entschieden, welcher Gütetext in den Rahmentext übernommen wird.

**CEKAL**
In Frankreich müssen ISO-Gläser, die mit dem Zertifikat CEKAL gekennzeichnet sind, fest definierten Qualitätskriterien entsprechen.
Um die CEKAL-Normen bei Änderungen anpassen zu können, wurden die aktuellen CEKAL-Normen nicht fest in A+W Business integriert. Sie können frei definiert werden.
Bei der Erfassung einer ISO-Einheit wird ein CEKAL-Text anhand der hinterlegten Regeln erstellt. Er kann im Auftrag überschrieben werden. Dieser Text kann wie folgt eingesetzt werden:
*   CEKAL-Texte auf Formularen, Etiketten, Produktionspapieren drucken.
*   CEKAL-Texte an die Produktion für den Rahmenbieger übergeben.

#### Textkennzeichen und Standardtexte

Standardtexte werden anhand von Textkennzeichen unterschieden, z. B. das Textkennzeichen O für Angebote, P für Produktion, L für Lieferschein. Die Textkennzeichen können Sie nach den Erfordernissen in Ihrem Betrieb hinterlegen.

**Beispiele**
*   **Info-Texte (Textkennzeichen /):** Diese Texte sollen in allen Dokumenten gedruckt werden, z. B. die Ankündigung von Betriebsferien.
*   **Lieferscheinspezifische Texte (Textkennzeichen L):** Diese Texte sollen nur auf den Lieferscheinen gedruckt werden, z. B. die Reklamationsfrist.
*   **Angebotstexte (Textkennzeichen O):** Diese Texte sollen nur auf Angeboten gedruckt werden, z. B. Gültigkeitsdauer des Angebots.

Die Textkennzeichen dienen nicht nur der Gruppierung Ihrer Standardtexte. Über das Textkennzeichen steuern Sie, welche Texte in welchen Dokumenten gedruckt oder an die Produktion übergeben werden.

**Beispiel**
Produktionstexte (Textkennzeichen P) sollen auf dem Lieferschein nicht gedruckt werden. Pro Formular legen Sie in der Formularverwaltung fest, welche Textkennzeichen nicht gedruckt werden sollen.

Diese Funktion wird in einer separaten Einheit beschrieben.
⇨ “Formularverwaltung" auf Seite B-480

Bei der manuellen Auswahl eines Textes im Dokument kann die Suche über das Kennzeichen gefiltert werden.

*[Image: Abb. B-289 Standardtexte. A: Textnummern, B: Textkennzeichen, C: Hinterlegter Text, D: Liste der Standardtexte für Angebote.]*

Pro Textkennzeichen (B) können Sie beliebig viele Texte (D) hinterlegen. Jeder Text ist durch eine eigene Nummer (A) gekennzeichnet.

Vergeben Sie die Nummern der Texte in Blöcken, die sich an den Textkennzeichen orientieren, z. B. die Nummern 1 bis 199 für Kennzeichen O, 200 bis 299 für Kennzeichen 1, 300 bis 399 für Kennzeichen P.

Die Texte können im Dokument eingefügt und bearbeitet werden. Leerstellen werden dann manuell ergänzt oder durch die Platzhalter gefüllt.

*[Image: Abb. B-290 Standardtext im Angebot. A: Ausgewählter Text, B: Hinterlegter Text.]*

In diesem Beispiel für ein Angebot muss das Datum im Text manuell eingefügt werden.

#### Variablen

Allgemeine Texte und Systemtexte können mit Platzhaltervariablen definiert werden. Diese dienen dazu, die entsprechenden Daten erst dann einzutragen, wenn ein Dokument erstellt wird.

**Beispiel**
Die Angabe des Datums wird typischerweise mit einer Variablen geschrieben. Das Datum wird aus dem Systemdatum gelesen und eingesetzt, wenn das Dokument oder die Datei erzeugt wird.
Die Variable `<d1>` wird im Dokument automatisch durch das Datum Gültig von ausgetauscht und die Variable `<d2>` durch das Datum Gültig bis.

*[Image: Abb. B-291 Systemtext. A: Text mit Variablen, B: Variable. Example text: 'Anzahlung v. <ad> für Auftr. <aa> vom <aad>'.]*

Texte können in folgenden Dialogen eingefügt werden:
*   Partnerverwaltung > Register Texte
*   Produktverwaltung > Register Texte
*   Dokumentenverwaltung > Register Texte
*   Positionen > Register Texte

Die Variablen werden bei folgenden Ausgaben eingesetzt:
*   Bearbeitungstexte
*   Produktdefinition
*   Rahmentexte, CEKAL-Texte
*   Exportdateien

#### Formeln

Variablen können in einem Text zu Formeln verknüpft werden, in denen eine Größe anhand der Angaben aus dem Dokument berechnet wird.

*[Image: Abb. B-292 Text mit Formel in der Produktdefinition. Example text: 'Säumen von <%> Kante(n) *<§>*'.]*

In diesem Beispiel sehen Sie die Formel für die Berechnung der Kantenlänge. Die Formel ist folgendermaßen zu lesen:
*   `<%>`: Anzahl der Kanten
*   `<§>`: Nummern der Kanten
*   `<=>`: Gesamtlänge

Bei einer Scheibe mit den Maßen 1200 x 1800 mm ergibt sich daraus z. B. die Berechnung: 4 Kanten = 6000 mm Gesamtlänge der Bearbeitung.

Im Auftrag wird je nach Anzahl der Kanten folgender Text angezeigt:

*[Image: Abb. B-293 Beispiel Auftragsposition (2 oder 4 Kanten säumen). The description text changes based on the number of processed edges.]*

Die Gesamtlänge richtet sich nach den Kanten, die bearbeitet werden.
Bei der Erstellung einer solchen Definition werden Sie durch Erläuterungen unterstützt, denen Sie die zulässigen Variablen entnehmen können.

*[Image: Abb. B-294 Formel und Parameter für Bearbeitung Säumen. A: Entspricht dem Zeichen =, B: Entspricht dem Zeichen §, C: Entspricht dem Zeichen %, D: Formel.]*

In diesem Beispiel für die Bearbeitung Säumen werden die verfügbaren Variablen (A bis C) angezeigt. Der Text (D) zwischen den Variablen (in spitzen Klammern) kann frei eingetragen werden.
Die Formel heißt: (Anzahl der Kanten) * (Länge der Kante) = (Gesamtlänge)
Je nach Bearbeitungen werden jeweils nur die Parameter aufgelistet, die Sie einsetzen dürfen.
⇨ "Verfügbare Variablen (Platzhalter)" auf Seite B-533
⇨ Softwarereferenz, "Systemtexte" auf Seite B-1060

#### Dateianhang

Sie können an einen Auftrag auch Dateien anhängen, z. B. mit detaillierten Angaben zur Kalkulation oder zu Modellen. Über Kennzeichen können Sie steuern, welche Dateianhänge weitergeleitet werden, z. B. an die Produktion.

Dateianhänge werden in folgenden Fällen weitergeleitet:
*   **Produktionsübergabe:** Dateianhänge für Übergabe in OrderXML, z. B. Produktinformationen.
*   **Dokumente kopieren:** Angebot zu Auftrag, z. B. Kalkulationsinformationen.
*   **Bestellübergabe:** z. B. Produktinformationen.

*[Image: Abb. B-295 Typen der Dateianhänge. The dialog 'Dateianhangs-Typen' is shown with a standard entry 'A - Alle'.]*

Das Standard-Kennzeichen A zeigt an, dass alle Dateianhänge übergeben werden. Davon ist nur die Bestellübergabe ausgenommen.

Wie bei den Textkennzeichen können Sie auch die Kennzeichen für diese Dateianhänge definieren, z. B. P für die Produktion, O für Angebote.

Die Einstellungen für die Übergabe von Dateianhängen ist in den Parts Verkauf und Fertigung beschrieben.

#### Texte anlegen

Sie können Standardtexte hinterlegen, die zur Auswahl angeboten werden, z. B. in der Auftragserfassung.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So legen Sie einen Standardtext an" auf Seite B-477
*   "So tragen Sie einen kundenspezifischen Text ein" auf Seite B-73

> **Voraussetzung**
> Um Texte vollständig zu hinterlegen, müssen die Textkennzeichen angelegt sein. Diese werden im Dialog Textkennzeichen angelegt, wie im Tutorial 1 für Basistabellen beschrieben.

**So legen Sie einen Standardtext an**

1.  Wählen Sie im Menü Stammdaten > Texte > Texte.
    Der Dialog zur Erfassung von Standardtexten wird geöffnet.

2.  Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wechseln.

    *[Image: Abb. B-296 Felder für neuen Text freigeschaltet. A: Frei wählbare Nummer, B: Matchcode, C: Textkennzeichen, D: Eingabe des Textes.]*

    ⇨ Softwarereferenz, "Texte" auf Seite B-1059

3.  Geben Sie die Nummer (A) ein.
    Beachten Sie die Nummernblöcke, die Sie für die Kennzeichen reserviert haben.

4.  Geben Sie den Matchcode (B) ein.
    Der Matchcode sollte ein Schlagwort aus dem Text verwenden.

5.  Wählen Sie das Textkennzeichen (C) aus, z. B. `I` Infotext.
    Das Textkennzeichen entscheidet, in welchen Dokumenten der Text ausgewählt und gedruckt werden kann.

6.  Schreiben Sie den gewünschten Text in das Eingabefeld (D).
    Die Einstellungen für die Schriftart und Schriftgröße gelten nur für die Anzeige auf dem Bildschirm. Sie werden nicht in den Druck übernommen.

7.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Daten werden gespeichert. Der Text kann jetzt in den Dokumenten, in der Partnerverwaltung und in der Produktverwaltung zugeordnet werden.

> **Fremdsprachige Texte**
> Fügen Sie die Übersetzungen in den jeweiligen Sprachen auf die gleiche Weise ein. Um Verwechslungen zu vermeiden, wählen Sie dabei dasselbe Textnummern wie im Originaltext.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Produktverwaltung - Texte" auf Seite B-628
⇨ Softwarereferenz, "Partnerverwaltung – Texte" auf Seite B-782
⇨ Softwarereferenz, "Texte" auf Seite B-1059

### Formulare

**Lernziele**
*   Funktion der Formulare kennenlernen.
*   Einstellungen für den Druck von Preisen und Skizzen prüfen.
*   Druckausgabe von Formularen anpassen.
*   Direktdruck und Druckjobs einrichten.

**Nutzen**
*   Dokumente werden in Formulare gedruckt und in verschiedenen Formaten ausgegeben, um sie zu versenden.
*   Der Druck kann in geringem Maß angepasst werden.

> **Merke**
> **Druckpunkt**: Druckpunkte sind Programmpunkte, an denen ein Dokument gedruckt werden kann.
> **Status**: Durch den Druck eines Dokuments wird der Status hochgesetzt. Dabei kann ein Dokument nur einmal den Status für den Originaldruck erreichen. Danach kann nur noch der Wiederholungsdruck gestartet werden.
> **Formular**: Formulare sind fest definierte Dateien, die an das Layout in Ihrem Unternehmen angepasst sind. Für die Druckpunkte muss mindestens ein Formular hinterlegt sein, damit der Druck ausgeführt werden kann. Zu jedem Druckpunkt können mehrere Formulare hinterlegt werden.
> **Direktdruck**: Zu den fünf Dokumententypen können unterschiedliche Einstellungen gespeichert werden, mit denen ein Dokument direkt gedruckt werden kann, ohne den Dialog Formular-/Etikettendruck zu öffnen.
> **Druckauftrag**: Wenn der Druck über einen zentralen Printserver gestartet wird, können Druckaufträge definiert werden, die den Druck automatisieren.

#### Formularverwaltung

Dokumente werden in Formularen gedruckt. Die Formulare für den Druck von Auftragsbestätigungen, Rechnungen usw. sind im Standard-Layout Ihrer Firma gestaltet und stehen pro Sprache zur Verfügung. Neben den Formularen für die Dokumente sind auch Formulare für den Druck von Etiketten und für den Datenexport hinterlegt. Diese beiden Funktionen sind ausführlich im Part Verkauf beschrieben.

**Druckpunkt**
Druckpunkte sind Programmpunkte, an denen ein Dokument gedruckt werden kann. Diesen Druckpunkten entspricht jeweils ein Status(punkt), auf den das gedruckte Dokument gesetzt wird. Dabei wird zwischen der Ausgabe auf einem Drucker, einem Faxgerät oder als E-Mail unterschieden.

Druckpunkte sind jeweils für den Erstdruck und den Wiederholungsdruck angelegt. Das bedeutet, dass pro Dokument und Druckpunkt jeweils nur ein Original gedruckt werden kann. Wiederholungsdrucke sind mehrfach möglich.

**Beispiele**

| Kennzeichen | Typ | Bezeichnung |
| :--- | :--- | :--- |
| 100 | 2 (Auftrag) | AB Druck |
| 101 | 1 (Angebot) | Angebote Druck |
| 102 | 2 | Lieferschein Druck |
| 103 | 2 | Rechnung Druck |
| 104 | 3 (Gutschrift) | Gutschrift Druck |
| 105 | 2 | Reklamation Druck |
| 106 | 5 (Bestellung) | Bestellungsauftrag Druck |
| 107 | 4 (Bestellanfrage) | Bestellanfrage Druck |
| 108 | 2 | Fertigungsschein Druck |
| ... | | ... |
| 200 | 2 | AB WH-Druck |
| 201 | 1 | Angebote WH-Druck |
| 202 | 2 | Lieferschein WH-Druck |
| 203 | 2 | Rechnung WH-Druck |
| 300 | 2 | Fax AB Druck |
| 350 | 2 | Mail AB Druck |
| 400 | 2 | Fax AB WH-Druck |
| 450 | 2 | Mail AB WH-Druck |

In dieser Liste sehen Sie einige Druckpunkte. Für jeden Dokumententyp sind jeweils die Druckpunkte eingerichtet, die den Erst- und den Wiederholungsdruck in den unterschiedlichen Ausgabeformaten ermöglichen.

Jedem Druckpunkt muss mindestens ein Formular zugeordnet sein, damit die Ausgabe gestartet werden kann.

#### Formularzuordnung

Sie können jedem Druckpunkt beliebig viele Formulare zuordnen. Diese Zuordnungen werden beim Einrichten des Programms festgelegt und müssen in der Regel nicht geändert werden. Sie können jedoch zusätzliche Formulare zuordnen. Die Formulare müssen als Vorlagedatei im Format *.qrp abgelegt sein.

*[Image: Abb. B-297 Zuordnung von Formularen. A: Kennzeichnung des Standard-Formulars, B: Aktueller Druckpunkt, C: Anzahl der Druckexemplare, D: Dateiname des Formulars, E: Statusumleitung, z. B. Barverkauf, F: Liste der zugeordneten Formulare.]*

In diesem Beispiel sehen Sie, welche Formulare (F) dem Druckpunkt AB Druck (B) zugeordnet sind. Das markierte Formular ist das Standard-Formular (A), von dem jeweils ein Exemplar (C) gedruckt wird.

Sie können jedem Formular einen abweichenden Statuspunkt (E) zuordnen. Diese Zuordnung ist in der Regel nur bei einem Formular für Barverkäufe nötig. Dafür wählen Sie den abweichenden Statuspunkt Barverkauf aus. Wenn kein abweichender Statuspunkt eingetragen ist, wird das Dokument durch den Druck auf den Status umgesetzt, der dem Druckpunkt entspricht.

#### Druck

Beim Druck von Dokumenten werden nur die Formulare angeboten, die dem Dokumententyp zugeordnet sind.

*[Image: Abb. B-298 Auftrag aus Nummernverwalter drucken. A: Auswahl des Formulars, B: Dokumentenstatus nach dem Druck, C: Auswahl des Druckmodus.]*

Die Dokumente aus einem Nummernverwalter werden gemäß den Vorgaben zum Druckmodus (C) und zum Formular (A) gedruckt.

Für den Druck können Sie folgende Verfahren einrichten:
*   Direktdruck
*   Druckaufträge (Druckjobs)

Diese Verfahren sind in separaten Einheiten beschrieben.
⇨ "Direktdruck" auf Seite B-491
⇨ "Druckaufträge" auf Seite B-492

#### Ausgabeformat

Sie können alle Dokumente über die hinterlegten Formulare in verschiedenen Formaten ausgeben:
*   Druck auf Papier
*   PDF
*   RTF
*   E-Mail
*   Fax
*   XML

Welches Format Sie im Einzelfall wählen, hängt davon ab, was und zu welchem Zweck Sie das Dokument drucken möchten.

Bei allen Dokumenten, die Sie auf elektronischem Weg versenden möchten, müssen Sie darauf achten, dass der Empfänger in der Lage ist, das gesendete Dokument zu lesen.

**Beispiel**
Der Versand als PDF-Datei per E-Mail setzt voraus, dass der Empfänger einen sogenannten Viewer installiert hat, mit dem er das Dokument öffnen und lesen kann, z. B. den Acrobat Reader. Dieses Dokumentenformat ist immer dann am besten geeignet, wenn Sie mit den Aufträgen auch Skizzen der Modelle oder Sprossen darstellen möchten.

#### Druckanpassung

Die Druckausgabe können Sie in begrenztem Rahmen anpassen. Neben den Kopf- und Fußzeilen z. B.:
*   Druck von Skizzen, Preisen, Produktbezeichnungen usw.
*   Textkennzeichen für Texte, die nicht gedruckt werden.
*   Seitenumbruch
*   Standarddrucker

Der Druck von Skizzen und Preisen wird in verschiedenen Dialogen eingestellt. Diese Einstellungen sind in separaten Einheiten beschrieben.
⇨ "Preisdruck" auf Seite B-484
⇨ "Skizzendruck" auf Seite B-486

#### Preisdruck

Der Druck der Preise im Formular wird an unterschiedlichen Stellen festgelegt, die sich gegenseitig beeinflussen:
*   **Formularverwaltung:** Die Einstellungen gelten übergreifend und geben an, ob die Einstellung zum Preisdruck aus dem Dokument übernommen wird.
*   **Partnerverwaltung:** Die Einstellungen geben an, wie detailliert die Preise gedruckt werden sollen. Die Vorgaben können im Dokument überschrieben werden.
*   **Produktverwaltung:** Die Einstellungen geben an, ob die Preise explizit oder implizit dargestellt werden, z. B. bei Stücklisten-Komponenten.
*   **Dokumentenverwaltung (Auftrag):** Die Einstellungen geben an, wie detailliert die Preise gedruckt werden sollen. Die Einstellung wird nur übernommen, wenn dies durch die Einstellung in der Formularverwaltung zugelassen ist.

**Druckeinstellungen für Preise in der Formularverwaltung**
Die Einstellung in der Formularverwaltung lässt folgende Möglichkeiten zu:
*   **0 - Standard oder 2 - Preise immer drucken (Summenmodus):**
    Im Formulardruck werden die Angaben aus dem Dokument übernommen:
    *   **0 - Kein Druck:** Preise werden nicht gedruckt.
    *   **1 - Alle Preise:** Preise werden pro Auftragsposition gedruckt.
    *   **2 - Nur Summen:** Nur die Positionssummen werden gedruckt.
*   **1 - Preise immer drucken:**
    Die Einstellungen aus dem Dokument werden ignoriert. Die Preise werden pro Auftragsposition gedruckt.

*[Image: Abb. B-299 Einstellung für den Preisdruck. A: Register Optionen 1, B: Druck von Preisen.]*

#### Druck von Positions- und Summenpreisen

Der Druck der Preise wird von der Formularverwaltung und von der Einstellung im Dokument gesteuert.

| Einstellungen Dokument | Einstellungen Formularverw. | Druck Positionspreise | Druck Summenpreise |
| :--- | :--- | :--- | :--- |
| 0 | 0 | - | - |
| 1 | 0 | X | X |
| 2 | 0 | - | X |
| 0 | 1 | X | X |
| 1 | 1 | X | X |
| 2 | 1 | X | X |
| 0 | 2 | - | X |
| 1 | 2 | - | X |
| 2 | 2 | - | X |

**Legende:**
*   **Dokumente**: 0 = Kein Druck, 1 = Alle Preise, 2 = Nur Summen
*   **Formularverwaltung**: 0 = Standard (Dokument entscheidet), 1 = Preise immer drucken, 2 = Preise immer drucken (Summenmodus)
*   **-** = kein Druck, **X** = Druck

**Beispiel**
Wenn im Dokument Summen drucken (2) eingestellt ist und in der Formularverwaltung Standard (0), werden nur Summenpreise gedruckt, jedoch keine Positionspreise.

#### Skizzendruck

Beim Skizzendruck wird zwischen Modell- und Sprossenskizzen unterschieden. Die Anzeige und der Druck der Skizzen werden in verschiedenen Dialogen festgelegt:
*   **Firmendaten:** Die Einstellungen legen fest, wie Sprossenskizzen standardmäßig gedruckt werden sollen.
*   **Formularverwaltung:** Die Einstellungen legen die Details des Skizzendrucks für Modelle und Sprossenkonstruktionen fest.
*   **Produktverwaltung:** Die Einstellungen legen für Modelle und Sprossenkonstruktionen fest, ob Skizzen gedruckt werden. Dabei kann zwischen maßstäblicher und schematischer Darstellung gewählt werden.
*   **Positionserfassung:** Die Einstellungen legen für Modelle und Sprossenkonstruktionen getrennt fest, ob und wie Skizzen gedruckt werden sollen. Dabei kann pro Position zwischen maßstäblicher und schematischer Darstellung gewählt werden.

*[Image: Abb. B-300 Formularverwaltung – Einstellungen zum Skizzendruck. A: Druckmodus (Modell, Sprossen), B: Größe der Darstellung, C: Textgröße in Modellskizzen, D: Maßstab für Sprossenskizzen.]*

In der Formularverwaltung können Sie den Druck für Modell- und Sprossenskizzen einstellen. Die Entscheidung für den Druck differenzieren Sie weiter nach maßstäblicher oder schematischer Darstellung (A). Außerdem können Sie die Größe der gedruckten Skizze definieren (B).

Wenn Modellskizzen maßstäblich gedruckt werden, sind auch die Maße in der Skizze dargestellt. Die Position der Maße in der Skizze können Sie in der Vorlage bearbeiten, damit diese im Druck deutlich zu erkennen sind.

> **Gebogenes Glas**
> Die Wölbung von gebogenem Glas wird immer schematisch dargestellt.

#### Skizzendruck für Sprossen (Rechteckscheiben)

| Einstellung zur Position (Sprosse) | Einstellung in der Formularverwaltung (kein Druck) | Einstellung in der Formularverwaltung (schematisch) | Einstellung in der Formularverwaltung (maßstäblich) |
| :--- | :--- | :--- | :--- |
| maßstäblich | kein Druck | kein Druck | Sprosse maßstäblich |
| schematisch | kein Druck | schematisch | Sprosse schematisch |
| kein Druck | kein Druck | kein Druck | kein Druck |

In dieser Übersicht sehen Sie, dass Sprossen in einer Rechteckscheibe nur dann maßstäblich gedruckt werden, wenn sowohl im Dokument als auch in der Formularverwaltung der maßstäbliche Druck eingestellt ist.

Für den Druck von Sprossenkonstruktionen muss in den Firmendaten der Funktion Erweiterte Sprossenskizze im Formulardruck aktiviert werden.

#### Skizzendruck bei Modellscheiben

| Einstellung zur Position | Einstellung in der Formularverwaltung (kein Druck) | Einstellung in der Formularverwaltung (schematisch) | Einstellung in der Formularverwaltung (maßstäblich) |
| :--- | :--- | :--- | :--- |
| **Modell** maßstäblich | kein Druck | schematisch | maßstäblich |
| **Modell** schematisch | kein Druck | schematisch | schematisch |
| **kein Druck** | kein Druck | kein Druck | kein Druck |
| **Sprosse** maßstäblich | kein Druck | kein Druck | kein Druck |
| **Sprosse** schematisch | kein Druck | kein Druck | kein Druck |

In dieser Übersicht sehen Sie, dass Modelle nur dann maßstäblich gedruckt werden, wenn sowohl im Dokument als auch in der Formularverwaltung der maßstäbliche Druck eingestellt ist.

Der Druck von Modellskizzen wird in der Formularverwaltung im Register Optionen 1 übergreifend aktiviert oder deaktiviert.
Modellskizzen werden immer als separates Blatt gedruckt.

#### Vermaßte Skizze drucken

Im Modul Dokumente können Sie vermaßte Skizzen drucken. Hierbei können Sie die Funktion Erweiterte Modellskizze auswählen, um maßstäbliche Skizzen von Modellen und Sprossen auf ein separates Blatt zu drucken.

Um vermaßte Skizzen zu nutzen, muss die Funktion in den Firmendaten aktiviert sein.

*[Image: Abb. B-301 Firmendaten – Register Druck. Checkbox 'Erweiterte Sprossenskizze im Formulardruck' is activated.]*

Im Dialog Vermaßte Skizze drucken werden nur die Positionen angezeigt, in denen der Skizzendruck von Modellen oder Sprossen auf maßstäblich gesetzt ist.

*[Image: Abb. B-302 Maßstäbliche Skizzen drucken. A: Positionen mit Sprossen markieren, B: Positionen mit Modell markieren, C: Details zu Sprossen, D: Produktskizze.]*

Über die Schaltflächen (A) und (B) können Sie die Positionen markieren, in denen Sprossen (A) oder Modelle (B) enthalten sind.

Wenn Sie Details zu den Sprossen (C) aktiviert haben, werden zusätzlich die Stückliste und Angaben zu den Sprossen gedruckt.

*[Image: Abb. B-303 Beispiele für den Druck von vermaßten Skizzen. A: Sprossenskizze, B: Sprossenzuschnittsliste, C: Modellskizze.]*

Die Produktskizze (D) wird als Datei am Produkt angehängt. Sie können in der Produktverwaltung jedem Produkt eine Abbildung als Anhang hinzufügen. Diese Abbildung kann nur gedruckt werden, wenn in der Produktverwaltung die Checkbox Druck auf Formular aktiviert ist.

*[Image: Abb. B-304 Produktverwaltung - Beispiel für Artikelskizze. The 'Druck auf Formular' checkbox is shown.]*

Diese Abbildung gibt das Produkt selber wieder. Es zeigt weder das Modell noch die eingebauten Sprossen. Es ist daher nur für seltene Strukturgläser sinnvoll.
Das Bild kann ebenfalls auf Formulare gedruckt werden. Dazu muss die Checkbox (D) markiert sein.

#### Direktdruck

Für den Druck einzelner Dokumente können Sie Einstellungen für den so genannten Direktdruck festlegen. Im Direktdruck sind alle Einstellungen fixiert, so dass Sie nicht weiter eingreifen müssen.

*[Image: Abb. B-305 Direktdruck im Auftrag. A: Standard-Druckfunktionen, B: Direktdruck. Shows custom direct print buttons in the toolbar.]*

Die Einstellungen legen Sie im Dialog Auftragsformulare fest.

*[Image: Abb. B-306 Zuordnungen für den Direktdruck. A: Dokumententyp, B: Druckpunkt, C: Formular, D: Rückfrage vor Druck, E: Liste der definierten Direktdrucke.]*

In diesem Beispiel sehen Sie, dass zu einem Dokumententyp (A) mehrere Zuordnungen (E) zum Direktdruck eingerichtet werden können. Beim Druck aus dem Dokument heraus entfallen dann die manuellen Einstellungen. Wenn der Druck ohne Rückfrage (D) gestartet wird, wird der Dialog Formular-/Etikettendruck nicht angezeigt. Der Druck wird dann sofort zum ausgewählten Drucker gesendet.

Sie können Zuordnungen für den Direktdruck für folgende Dokumententypen anlegen:
*   Angebot
*   Auftrag, inklusive Auftragsbestätigung, Lieferschein, Rechnung, Reklamation usw.
*   Gutschrift
*   Bestellanfrage
*   Bestellung

#### Druckaufträge

Wenn Sie mit einem zentralen Printserver arbeiten, können Sie Druckaufträge definieren. Zu einem Druckauftrag können ein oder mehrere Druckläufe definiert werden. Auf dem Printserver werden diese Druckaufträge in der Reihenfolge abgearbeitet, in der sie in der Übersicht angezeigt werden, z. B.:
*   Drucken der Auftragsbestätigungen für interne Zwecke.
*   Auftragsbestätigungen als Wiederholungsdruck per Fax senden.
*   Auftragsbestätigungen als Wiederholungsdruck per E-Mail an den Vertreter senden.

*[Image: Abb. B-307 Druckauftrag. A: Name des Drucklaufs, Dokumententyp, B: Liste der Druckläufe, C: Einstellungen für Sammeldruck, D: Einstellungen für den Versand.]*

Jeder Druckauftrag bezieht sich immer auf einen bestimmten Dokumententyp und kann nur für diesen gestartet werden. Die Felder für die Einstellungen zum Druck (D) werden je nach Formular freigeschaltet.

Nach jedem Drucklauf wird der Status des Dokuments hochgesetzt. Die Reihenfolge (B) der Druckläufe muss daher mit der Vergabe des Status übereinstimmen. Wenn z. B. der Rechnungsdruck nur gestartet werden kann, nachdem der Lieferschein gedruckt wurde, muss der Drucklauf für den Lieferschein vor dem Drucklauf für die Rechnung stehen.

Wenn im Druckauftrag ein Sammeldruck (C) für Rechnungen definiert ist, muss die Option Sammelausdruck in den Stammdaten des Kunden aktiviert sein. Zu einer Sammelrechnung werden alle Aufträge eines Kunden zusammengefasst, in denen das entsprechende Kennzeichen aktiviert ist. Der Druck kann dann weiter definiert werden:
*   **Immer:** Diese Einstellung überschreibt die Einstellung zum Sammeldruck aus den Stammdaten.
*   **Pro Bestelltext 1:** Alle Dokumente für einen Kunden werden nach dem Bestelltext 1 gefiltert und zusammengefasst. Wenn z. B. für einen Kunden 10 Aufträge vorhanden sind, von denen fünf den gleichen Bestelltext 1 haben, werden sechs Auftragsbestätigungen gedruckt.
*   **Pro Lieferadresse:** Alle Dokumente mit derselben Lieferanschrift werden zusammengefasst.
*   **Standard:** Alle Dokumente mit demselben Kunden oder mit demselben Lieferanten werden zusammengefasst, wenn das Kennzeichen für den Sammeldruck gesetzt ist.

Der Druck von Sammelrechnungen ist ausführlich im Part Verkauf beschrieben.
⇨ Verkauf, "Sammelrechnungsdruck" auf Seite C-33

> **Druckername muss bekannt sein**
> Bei der Definition der Druckläufe muss der Drucker auf dem Server verfügbar sein. Dazu muss er auch auf dem Client eingerichtet sein.

#### Direktdruck definieren

Einstellungen für den Direktdruck können Sie für jeden Dokumententyp festlegen.

**So definieren Sie einen Direktdruck**

1.  Wählen Sie im Menü Stammdaten > Formulare > Auftragsformulare.
2.  Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wechseln.
    Die Felder sind mit dem markierten Direktdruck vorbelegt.

    *[Image: Abb. B-308 Felder für neuen Direktdruck freigeschaltet. A: Name des Direktdrucks, B: Dokumententyp, Druckpunkt, C: Drucker, D: Formular für den Direktdruck, E: Druck-Dialog anzeigen.]*

    ⇨ Softwarereferenz, "Auftragsformulare" auf Seite B-1082

3.  Tragen Sie die Bezeichnung (A) ein.
    Geben Sie den Namen so ein, dass sofort zu erkennen ist, ob es ein Erst- oder ein Wiederholungsdruck ist, z. B. **Angebot (WH)** für den Wiederholungsdruck von Angeboten.

4.  Wählen Sie den Dokumententyp und den Druckpunkt (B) aus, für den der Direktdruck gelten soll.
    Achten Sie darauf, dass der Druckpunkt zu dem gewählten Dokumententyp passt. Wenn Sie versehentlich einen falschen Druckpunkt wählen, kann das Dokument nicht gedruckt werden.

5.  Wählen Sie den Drucker (C) aus, auf dem der Druck gestartet werden soll.
    In der Auswahl werden alle Drucker angezeigt, die auf dem aktuellen Rechner eingerichtet sind. Wenn der Serverdrucker nicht angezeigt wird, müssen Sie ihn einrichten (lassen).

6.  Wählen Sie ggf. das Formular (D) für den Druckpunkt aus.
    Diese Auswahl ist nur notwendig, wenn dem Druckpunkt mehrere Formulare zugeordnet sind.

7.  Markieren Sie ggf. die Checkbox (E).
    Wenn die Checkbox markiert ist, wird der Dialog Formular-/Etikettendruck auch beim Aufruf des Direktdrucks angezeigt.

    *[Image: Abb. B-309 Einstellungen für Direktdruck festgelegt. The fields are filled for a repeat print of an offer.]*

8.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Daten werden gespeichert und die Übersicht wird aktualisiert. Im Angebot kann dieser Direktdruck jetzt abgerufen werden.

#### Druckauftrag anlegen

Ein Druckauftrag umfasst mehrere Druckläufe. Bei der Sortierung der Druckläufe müssen Sie unbedingt die Reihenfolge der Statusvergabe beachten. Beispielsweise darf der Lieferschein auch auf dem Printserver erst nach der Auftragsbestätigung gedruckt werden.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So legen Sie einen Druckauftrag an" auf Seite B-496
*   "So fügen Sie Druckläufe hinzu" auf Seite B-498

Die Mehrzahl der nachfolgenden Einstellungen für den Druck über den Server kann während des Formulardrucks nicht mehr verändert werden.

**So legen Sie einen Druckauftrag an**

1.  Wählen Sie im Menü Stammdaten > Formulare > Druckaufträge.
    Der Dialog Druckaufträge wird geöffnet.
2.  Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wechseln.

    *[Image: Abb. B-310 Felder für neuen Druckauftrag freigeschaltet. A: Name des Druckauftrags, B: Dokumententyp.]*

    ⇨ Softwarereferenz, "Druckaufträge" auf Seite B-1083

3.  Tragen Sie die Bezeichnung (A) ein.
    Wählen Sie die Bezeichnung so, dass deutlich wird, wofür der Druckauftrag verwendet werden soll. In diesem Beispiel wird ein Druckauftrag für den Wiederholungsdruck von Lieferschein und Rechnung angelegt.

4.  Wählen Sie den Dokumententyp (B) aus.
    In diesem Beispiel wird Auftrag gewählt.

5.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Daten werden gespeichert. Sie können nun die Druckläufe hinzufügen und die Einstellungen für den Druck festlegen.

> **Druckauftrag auswählen**
> In der Übersicht Druckaufträge können Sie den Druckauftrag markieren, den Sie bearbeiten wollen. Wenn ein neuer Druckauftrag noch nicht angezeigt wird, dann schließen Sie den Dialog und öffnen ihn wieder, damit die Daten neu eingelesen werden.

**So fügen Sie Druckläufe hinzu**

1.  Wählen Sie den Druckauftrag aus, zu dem Sie einen Drucklauf hinzufügen wollen.

    *[Image: Abb. B-311 Felder für neuen Druckläufe freigeschaltet. A: Auswahl Formular, B: Auswahl Drucker, C: Auswahl Druckaufträge, D: Formulare im Drucklauf, E: Drucklauf hinzufügen, F: Drucklauf löschen.]*

2.  Klicken Sie auf [Hinzufügen] (E).
    Die Felder im Bereich Formularauswahl werden freigeschaltet.

3.  Wählen Sie das Formular (A) aus, z. B. AB WH-Druck.
    Das Formular wird in die Übersicht (D) übernommen.

4.  Wählen Sie den Drucker (B) aus.
    Achten Sie darauf, dass Sie den richtigen Netzwerkdrucker wählen.

5.  Wiederholen Sie die Schritte 2 bis 4, um weitere Druckläufe hinzuzufügen.

    *[Image: Abb. B-312 Druckläufe sammeln. A: Vorgabe für Dokumentennummer, B: Einstellungen für Druckausgabe, C: Druckläufe sortieren, D: Liste der Druckläufe im Druckauftrag.]*

6.  Sortieren Sie die Druckläufe in der Übersicht mit Hilfe der Pfeilschaltflächen (C) in die Reihenfolge, die der Statusvergabe entspricht.

7.  Legen Sie ggf. die Details (B) zur Druckausgabe pro Formular fest.
    Die Einstellungen für die Druckausgabe sind je nach gewähltem Formular freigeschaltet. Sie gelten jeweils nur für dieses eine Formular.
    Die Nummer (A) für die Dokumente kann aus den Nummernkreisen der AV-Bereiche oder der Mandanten genommen werden.

8.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Daten werden gespeichert.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Modellskizze, Sprossenskizze" auf Seite B-609
⇨ Softwarereferenz, "Firmendaten - Dokumente" auf Seite B-941
⇨ Softwarereferenz, "Firmendaten - Druck" auf Seite B-996
⇨ Softwarereferenz, "Formulare" auf Seite B-1064
⇨ Softwarereferenz, "Formularverwaltung" auf Seite B-1064
⇨ Softwarereferenz, "Auftragsformulare" auf Seite B-1082
⇨ Softwarereferenz, "Druckaufträge" auf Seite B-1083
⇨ Verkauf, "Druck" auf Seite C-196

## Komplexübung

Die folgenden Aufgaben bauen auf den Lerneinheiten von Tutorial 1 und Tutorial 2 auf.
*   Legen Sie einen neuen Kalender für das kommende Jahr an.
*   Legen Sie zwei neue Preisschlüssel mit der Gültigkeit für 90 Tage an: einen für den Verkauf und einen für den Einkauf.
    Sie werden diese in den folgenden Aufgaben als Tarif verwenden!
*   Legen Sie ein Produkt VSG mit der Bearbeitung Schleifen an.
    Achten Sie darauf, an welchen Stücklisten-Komponenten die Bearbeitung hängt.
*   Legen Sie ein Produkt ISO an, in dem eine Scheibe Ihr VSG ist.
    Achten Sie darauf, dass die Beschaffungsart für dieses Glas korrekt ist.
*   Legen Sie Preistabellen für die Berechnung von EK- und von VK-Preisen für die neuen Produkte an. Richten Sie diese in Ihrem neuen Tarif ein.
*   Legen Sie einen Kunden mit folgenden Daten an:
    *   Tour
    *   Zahlungsbedingungen
    *   Lkw und Fahrer
*   Legen Sie für diesen Kunden ein Objekt an.
*   Legen Sie in Ihrem Tarif eine neue Preistabelle für dieses Objekt an und weisen Sie diese dem Kunden zu.
*   Erfassen Sie einen Auftrag mit Ihrem ISO.
    Der Auftrag muss sich auf das Objekt beziehen und automatisch den entsprechenden Preis anzeigen.
*   Prüfen Sie den Status des Objekts in den Stammdaten.
*   Legen Sie einen neuen Mitarbeiter an. Dieser soll das Recht haben, Aufträge zu erfassen und an die Produktion zu übergeben.

## Zusatzinformationen

In diesem Abschnitt finden Sie Ergänzungen zu Tutorial 1 und 2. Dies sind im Wesentlichen technische Informationen zu Berechnungen und Übersichten zu den fest definierten Vorgaben.
*   "Objekt-/Abrechnungsverwaltung" auf Seite B-502
*   "Verfügbare Dokumententypen” auf Seite B-527
*   "Verfügbare Grenztypen" auf Seite B-528
*   "Verfügbare Systemtexte" auf Seite B-532
*   "Verfügbare Variablen (Platzhalter)" auf Seite B-533
*   "Konstruktionstypen Bleiverglasung" auf Seite B-536
*   "Änderungsüberwachung" auf Seite B-537
*   "A+W Production" auf Seite B-540
*   "Mischkalkulation" auf Seite B-543
*   "Französische Preisberechnung" auf Seite B-544
*   "Kalkulation" auf Seite B-545

### Objekt-/Abrechnungsverwaltung

**Lernziele**
*   Varianten der Objektverwaltung kennenlernen.
*   Mit Objekten arbeiten.

**Nutzen**
*   Gesonderte Konditionen für Objekte werden automatisch herangezogen, solange das Objekt gültig ist.
*   Zu einem Rahmenvertrag können mehrere Aufträge erstellt werden, bis die vereinbarten Flächen, Stückzahlen oder Summen ausgeschöpft sind.

> **Merke**
> **Objekt**: Ein Objekt ist ein bestimmtes Bauvorhaben, an dem mehrere Kunden und Lieferanten beteiligt sein können. Es wird ein Objekt angelegt und den beteiligten Partnern zugewiesen.
> **Kundenobjekt**: Ein Objekt kann im Auftrag nur dann angegeben werden, wenn es dem Kunden zugeordnet ist. Im Kundenobjekt können abweichende Vertreter und Zahlungsbedingungen angegeben werden. Wenn ein Objekt als komplett gekennzeichnet ist, kann es nicht weiter verwendet werden.
> **Rahmenauftrag**: Ein Rahmenauftrag bezieht sich auf einen Kunden, der im Rahmen veranschlagter Höchstmengen und/oder Gesamtsummen mehrere Aufträge abruft.
> **Forderungsrechnung**: Zu Rahmenaufträgen können Produktionsaufträge und Forderungsrechnungen erstellt werden.
> **Abrechnungsverwaltung**: Bei der Abrechnungsverwaltung erfassen Sie Forderungen, Stundenforderungen und Einkaufsforderungen, die einem Auftrag zugewiesen werden. Objekte können dabei nicht verwendet werden.
> **Voreinstellungen**: Firmendaten > Register Dokumente > Objektverwaltung

> **Vorkenntnisse**
> Bitte beachten Sie, dass in den Beschreibungen die Abfolge der Handlungsschritte stark verkürzt ist, wenn diese Schritte in anderen Teilen der A+W Business-Dokumentation bereits ausführlich beschrieben sind.

#### Varianten der Objekt-/Abrechnungsverwaltung

Für die Arbeit mit Objekten stehen unterschiedliche Modi zur Verfügung, in denen Aufträge und Bestellungen abgerechnet werden.
*   Dabei sind mit Objekten bestimmte Bauvorhaben gemeint, zu denen besondere Konditionen für Aufträge und/oder Bestellungen gelten.
*   Rahmenaufträge können unabhängig von Bauvorhaben verwaltet werden. Dazu werden die Rahmenbedingungen in einem Rahmenauftrag festgelegt. Zu einem Rahmenauftrag können so lange einzelne Produktionsaufträge erstellt werden, bis die Vorgaben aus dem Rahmenvertrag ausgeschöpft sind. Über Forderungsrechnungen werden diese abgeschlossen.

In den Firmendaten muss die gewünschte Version der Abrechnungsverwaltung (Objektverwaltung) aktiviert werden.

Die unterschiedlichen Modi bieten folgende Funktionalitäten an:
*   **Standard-Objektverwaltung:** In diesem Modus können Sie einem Markpartner ein Objekt zuordnen. Wenn im Dokument das Objekt angegeben wird, werden die Konditionen für die Preisfindung herangezogen, die dem Objekt zugeordnet sind.
*   **Erweiterte Objektverwaltung:** In der erweiterten Objektverwaltung können Sie zusätzlich Angaben zum Vertreter und Zahlungsbedingungen hinterlegen. Diese Informationen werden in den Auftrag übernommen, wenn das Objekt dem Auftrag zugeordnet wird.
*   **Standard Objektverwaltung + Abrechnungsverwaltung mit zugeordneten Aufträgen:** Dieser Modus verbindet die Objektverwaltung mit der Abrechnungsverwaltung mit zugeordneten Aufträgen, so dass Sie beide Modi parallel nutzen können.
*   **Abrechnungsverwaltung mit zugeordneten Aufträgen:** In diesem Modus erfassen Sie einen Rahmenauftrag, aus dem Sie Forderungsrechnungen und damit verbunden Aufträge erstellen.
*   **Abrechnungsverwaltung:** In diesem Modus können Sie Forderungsrechnungen über geleistete Stunden und über den Zukauf von Bestellteilen erstellen und als Forderung einem Auftrag zuordnen.

In den Stammdaten sind die Dialoge für allgemeine Objekte, für die Zuordnung von Kunden und von Lieferanten gesperrt, wenn die Abrechnungsverwaltung aktiviert wurde. Im Modul Dokumente werden die Dialoge zur Abrechnungsverwaltung angezeigt, wenn eine der Abrechnungsverwaltungen aktiviert wurde.

Die Objekte selbst werden zunächst unabhängig angelegt und dann Kunden bzw. Lieferanten zugeordnet. Dabei können Sie ein Objekt einem oder mehreren Kunden bzw. Lieferanten zuordnen.

Ein Rahmenauftrag gilt jedoch immer nur für einen einzelnen Kunden.

#### Veranschlagte Mengen

Zu einem Objekt können Höchstmengen für ein Produkt oder eine Warengruppe angegeben werden. Diese können sich auf den Netto-Umsatz, die Stückzahl oder die Fläche beziehen:
*   Ein **Netto-Umsatz** ist z. B. sinnvoll, wenn Scheiben in unterschiedlichen Größen und/oder Gläsern geliefert werden sollen.
*   Die **Stückzahl** ist sinnvoll, wenn ein bestimmtes Produkt mit festen Maßen geliefert werden soll.
*   Die **Fläche** ist sinnvoll, wenn ein bestimmtes Produkt in unterschiedlichen Maßen geliefert werden soll.

**Mengen für ein Produkt oder eine WGR?**
Wenn Sie zu einem Objekt sehr unterschiedliche Produkte anbieten wollen, empfiehlt sich, eine Höchstwert für eine WGR anzugeben.
Wenn nur bestimmte Produkte vereinbart wurden, richtet sich die Höchstmenge nach der Größe. Bei festen Maßen ist eine Stückzahl angezeigt, ansonsten die Fläche.

#### Objektverwaltung einstellen

Für die Verwaltung von Objekten muss in den Firmendaten eine der folgenden Einstellungen gewählt sein:
*   Standard Objektverwaltung
*   Erweiterte Objektverwaltung
*   Standard Objektverwaltung + Abrechnungsverwaltung mit zugeordneten Aufträgen

Für die Abrechnungsverwaltung von Rahmenaufträgen muss in den Firmendaten eine der folgenden Einstellungen gewählt sein:
*   Abrechnungsverwaltung mit zugeordneten Aufträgen
*   Standard Objektverwaltung + Abrechnungsverwaltung mit zugeordneten Aufträgen

**So richten Sie die Vorgaben für die Verwaltung von Objekten ein**

1.  Stellen Sie sicher, dass in den Firmendaten der richtige Modus aktiviert ist, z. B. Standard Objektverwaltung.

    *[Image: Abb. B-313 Objektverwaltung aktivieren. A: Firmendaten - Register Dokumente, B: Modus der Objektverwaltung.]*

2.  Legen Sie ein Objekt an.
3.  Legen Sie die Konditionen fest, die für die Preisfindung herangezogen werden sollen, z. B. Tarif, Preis, Rabatt.
4.  Ordnen Sie das Objekt den beteiligten Kunden und Lieferanten zu.

Wenn Sie ein Objekt mehreren Kunden zuordnen, werden die Vorgaben zu Maximalwerten und Gültigkeit einzeln gespeichert. Sie können eine Übersicht über die erfassten Aufträge jeweils für einen Kunden erstellen.

Die Beschreibungen zu diesen Handlungsschritten finden Sie im Tutorial 1.
⇨ Tutorial 1, "Objekt anlegen und zuweisen" auf Seite B-126
⇨ Tutorial 1, "Einzelpreise anlegen" auf Seite B-239
⇨ Tutorial 1, "Rabatt anlegen" auf Seite B-361

#### Standard-Objektverwaltung

Mit der Standard-Objektverwaltung erfassen Sie einen Auftrag und geben dabei das Objekt an, auf das sich der Auftrag bezieht.

Stellen Sie zunächst sicher, dass Sie in den Firmendaten die Standard-Objektverwaltung aktiviert haben.
⇨ "Objektverwaltung einstellen" auf Seite B-504

Folgende Schritte müssen Sie ausführen, bevor Sie einen Auftrag zu einem Objekt erfassen:
*   Objekt anlegen
*   Objekt dem Kunden zuordnen
*   Preis zum Kunden und Objekt anlegen (optional)
*   Rabatt zum Objekt anlegen (optional)

*[Image: Abb. B-314 Objektvereinbarungen (Standard-Objektverwaltung). A: Gültigkeit des Projekts, B: Vereinbarte Höchstmengen im Projekt.]*

Für jeden Kunden bzw. Lieferanten legen Sie fest, in welchen Zeitraum (A) Aufträge oder Bestellungen zu diesem Objekt erfasst werden können. Zusätzlich können Sie Höchstwerte für Betrag, Fläche und/oder Stück (B) angeben.

#### Auftrag zu Standard-Objekt erfassen

Die objektbezogen Preise und Rabatte fließen in die Berechnung eines Auftrags ein, wenn der Kunde und das Objekt angegeben wurden.

**So erfassen Sie einen Auftrag zu einem Objekt**

1.  Wählen Sie Dokumente > Auftrag > Auftrag.
2.  Tragen Sie die Kopfdaten im Register Dokument ein.
3.  Wechseln Sie zum Register Konditionen.

    *[Image: Abb. B-315 Kundenauftrag - Objekt im Register Konditionen. A: Kunden-Objekt, B: Lieferanten-Objekt.]*

4.  Tragen Sie im Bereich Konditionen / Auftragsvolumen die Nummer des Kundenobjekts (A) ein.
    Wenn die Gültigkeit des Objekts abgelaufen oder das Objekt mit dem Status komplett abgeschlossen ist, können Sie die Nummer nicht eintragen.

5.  Öffnen Sie die Positionserfassung und erfassen Sie die Auftragspositionen.
    Da zu einem Standard-Objekt keine Produkte oder WGR angegeben werden, können Sie ein beliebiges Produkt erfassen.

6.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Daten werden gespeichert. Die Preise werden berechnet und die Preisanzeigen werden aktualisiert.

7.  Schließen Sie die Positionserfassung.
    Sie sich können eine Liste der bisher zum Objekt erfassten Aufträge anzeigen lassen.

8.  Wechseln Sie zum Register Konditionen und klicken Sie auf die Lupe rechts neben dem Namen des Objekts.

    *[Image: Abb. B-316 Kundenaufträge zum Objekt. A: Bisher zum Objekt erfasste Aufträge, B: Summe aus den erfassten Aufträgen, C: Maximalwerte aus der Objektdefinition.]*

    Die Anzeige gibt nur die Aufträge des aktuellen Kunden wieder.

#### Erweiterte Objektverwaltung

Mit der erweiterten Objektverwaltung können Sie zu den Objekten zusätzliche Bedingungen definieren, z. B. Zahlungsbedingungen.

Stellen Sie zunächst sicher, dass Sie in den Firmendaten die Erweiterte Objektverwaltung aktiviert haben.
⇨ "Objektverwaltung einstellen" auf Seite B-504

Folgende Schritte müssen Sie ausführen, bevor Sie einen Auftrag zu einem Objekt erfassen:
*   Objekt anlegen
*   Objekt dem Kunden zuordnen
*   Preis zum Kunden und Objekt anlegen (optional)
*   Rabatt zum Objekt anlegen (optional)

**Mit erweiterten Objekten arbeiten**

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So richten Sie ein Objekt ein" auf Seite B-509
*   "So prüfen Sie die aufgelaufene Summen" auf Seite B-512

**So richten Sie ein Objekt ein**

1.  Legen Sie ein Objekt an.
2.  Ordnen Sie das Objekt dem Kunden zu.

    *[Image: Abb. B-317 Erweitere Objekteinstellungen. A: Zeitraum für die Erfassung von Aufträgen, B: Vertreter für die Provisionsabrechnung, C: Abweichende Zahlungsbedingung, D: Status.]*

3.  Legen Sie die Gültigkeit fest (A), wenn für diese Objekt nach einem bestimmten Datum keine Aufträge mehr erfasst werden dürfen.
    Wenn das Objekt früher abgeschlossen wird, können Sie den Status (D) auf komplett umsetzen.

4.  Legen Sie einen abweichenden Vertreter (B) und/oder abweichende Zahlungsbedingung (C) fest.
    Bei der Erfassung von Aufträgen werden diese Informationen mit in den Auftrag übernommen, sobald das Objekt dem Auftrag zugeordnet ist.

5.  Wechseln Sie zum Register Veranschlagte Mengen.

    *[Image: Abb. B-318 Erweitere Objekteinstellungen – Veranschlagte Mengen. A: Auswahl des Produkts, B: Auswahl der Warengruppe, C: Eingabefelder für die Mengen, D: Eingabefelder freischalten.]*

6.  Klicken Sie auf die Schaltfläche (D), um die Eingabefelder freizuschalten.
7.  Wählen Sie die Option Produkt (A) oder WGR (B), für die Sie die Werte angeben wollen.
8.  Tragen Sie die veranschlagten Mengen ein (C).
9.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.

Sie können jetzt Aufträge für den Kunden erfassen und dabei das Objekt angeben. Die aufgelaufenen Summen eines Objektes werden nach dem Speichern einer Auftragsposition aktualisiert.

Wenn der Status eines Objektes auf komplett gesetzt ist, kann dafür kein Auftrag mehr erfasst werden. Damit können Sie das Objekt sperren, bevor die Gültigkeit abgelaufen ist. Wenn das Gültig-bis-Datum erreicht ist, wird das Objekt automatisch gesperrt.

**So prüfen Sie die aufgelaufene Summen**

1.  Wechseln Sie zum Dialog Abrechnungen > Summen.
    In diesem Register werden die Summen für den aktuellen Kunden aufgeführt.

    *[Image: Abb. B-319 Aufgelaufene Summen. A: Produkt, zu dem Mengen hinterlegt sind, B: Warengruppen, zu denen die in den Aufträgen erfassten Produkte gehören.]*

    Für das Produkt (A) wird angezeigt, wie weit die Objektgrenzen aus dem Register Veranschlagte Mengen bereits erreicht sind.

    *[Image: Abb. B-320 Aufgelaufene Summen. A: Produkt ohne Vereinbarungen der Menge, B: Veranschlagter Umsatz erreicht.]*

    Sind für ein Produkt oder eine Warengruppe die veranschlagten Mengen erreicht oder sogar überschritten, werden diese Einträge in der ersten Zeile in roter Schrift (B) dargestellt.
    Produkte, für die keine Mengen angegeben sind, werden ebenfalls aufgeführt. Auch für diese Produkte werden die entsprechenden Warengruppen angezeigt. Die Mengen werden jedoch lediglich bei der Gesamtsumme des Preises berücksichtigt.

    Die in den Registern Veranschlagte Mengen und Summen angezeigten Informationen können gedruckt werden.

2.  Wählen Sie im Menü Druck > Bildschirm > Druck nach Produkt, um sich die Übersicht anzeigen zu lassen.
3.  Bestätigen Sie die Drucker-Einstellungen, um den Druck zu starten.
    Auf die gleiche Weise können Sie die Ausgabe der Übersicht direkt auf einen Drucker schicken.

    *[Image: Abb. B-321 Aufgelaufene Summen über alle beteiligten Kunden. A print preview of the object summary report.]*

    Im Ausdruck werden alle Objekte und Kunden aufgeführt.
    Wenn Sie sich also einen Überblick über die Gesamtsummen zu einem Objekt verschaffen wollen, dann wählen Sie das Objekt aus und starten den Druck.

#### Abrechnungsverwaltung mit zugeordneten Aufträgen

In diesem Modus können Sie einen Rahmenauftrag einem Objekt zuordnen. Im Rahmenauftrag erfassen Sie für die einzelnen Positionen Produkte ohne detaillierte Angaben über den Produktaufbau, also z. B. ein ISO-Produkt ohne Angaben zu Bearbeitungen, Sprossen oder Modellen.

Von dem Rahmenauftrag aus erstellen Sie Forderungen, in denen Sie angeben, wie viel Prozent, Stück oder welcher Betrag vom ursprünglichen Rahmenauftrag eingefordert wird. Wenn Sie eine Forderung erstellen, wird automatisch ein Auftrag vom Typ Forderung erstellt.

Für diese Forderungen werden keine Rechnungen erzeugt. Sie werden in einem speziellen Modus an die FiBu übergeben. Wenn der Rahmenauftrag erfüllt und damit abgeschlossen ist, stellen Sie den (gesamten) Rahmenauftrag in Rechnung.

Für die Produktion und Lieferung an den Kunden erzeugen Sie Produktionsaufträge und ordnen diese dem (Abrechnungs-)Objekt zu. Zu diesen Produktionsaufträgen können auch Bestellungen erzeugt werden, die ebenfalls dem Objekt zugeordnet werden. Diese Bestellungen können sowohl manuell als auch über die automatische Bestellübergabe erzeugt werden. Beide Arten von Bestellungen können in einer Übersicht separat angezeigt werden. Für die Produktionsaufträge werden keine Rechnungen erstellt.

*[Image: Abb. B-322 Abrechnungsverwaltung mit zugeordneten Aufträgen. Flowchart showing the process from Rahmenauftrag (framework order) to Forderungsrechnung (claim invoice) and Produktionsaufträge (production orders).]*

Wenn ein Objekt als komplett markiert ist, kann dazu kein Auftrag mehr erfasst werden. Dieser Status wird automatisch gesetzt, sobald die Mengen aus dem Rahmenauftrag in den Forderungsrechnungen erreicht ist.

#### Rahmenauftrag abrechnen

Sie können Preise und Rabatte für den Kunden festlegen, für den Sie Rahmenaufträge erfassen. Wenn für den Rahmenauftrag gesonderte Konditionen gelten sollen, dann müssen Sie die entsprechenden Preise, Rabatte oder Zuschläge für den Kunden festlegen.

Für die Abrechnung von Rahmenaufträgen muss in den Firmendaten eine der folgenden Einstellungen gewählt sein:
*   Abrechnungsverwaltung mit zugeordneten Aufträgen
*   Standard Objektverwaltung + Abrechnungsverwaltung mit zugeordneten Aufträgen

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So legen Sie einen Rahmenauftrag an" auf Seite B-517
*   "So erfassen Sie einen Auftrag zu einem Rahmenauftrag" auf Seite B-520
*   "So erstellen Sie eine Forderungsrechnung" auf Seite B-522
*   "So schließen Sie einen Rahmenauftrag ab" auf Seite B-525

**So legen Sie einen Rahmenauftrag an**

1.  Legen Sie in der Auftragserfassung den Rahmenauftrag mit dem Dokumententyp Rahmenauftrag an.

    *[Image: Abb. B-323 Rahmenauftrag. A: Dokumententyp Rahmenauftrag.]*

2.  Erfassen Sie die Produkte, die über diesen Rahmenauftrag abgerechnet werden sollen.
    Dabei reicht es aus, wenn Sie z. B. ein ISO-Produkt erfassen, ohne weitere Angaben zu Sprossen, Modellen oder Bearbeitungen zu machen.

3.  Speichern Sie den Auftrag und schließen Sie die Auftragserfassung.

4.  Wählen Sie Dokumente > Objektabrechnungen > Abrechnungen.
    Der Dialog Abrechnungen wird geöffnet.

5.  Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wechseln.
    Die Eingabefelder werden freigeschaltet.

    *[Image: Abb. B-324 Abrechnungsobjekt zum Rahmenauftrag anlegen. A: Referenz auf Angebot oder Kundenauftrag, B: Abrechnungsnummer, C: Kundennummer, D: Nummer des Rahmenauftrags, E: Status.]*

6.  Tragen Sie folgende Daten ein:
    *   Abrechnungsnummer (B)
    *   Kundennummer (C)
    *   Nummer des Rahmenauftrags (D)

    Sie können als Referenz (A) die Nummer des Angebots und/oder die Nummer des Auftrags eintragen, den der Kunde erteilt hat.
    Wenn die Aufträge an eine andere Anschrift ausgeliefert werden sollen, tragen Sie die entsprechenden Daten ein, z. B. eine Filiale des Kunden.

7.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Damit haben Sie ein Abrechnungsobjekt zu Ihrem Rahmenauftrag angelegt.

Im Register Rahmenauftrag können Sie sich die Positionen des Rahmenauftrags anzeigen lassen. Wenn die Daten nicht sofort angezeigt werden, dann lesen Sie den Rahmenauftrag im Auswahlmodus neu ein.

*[Image: Abb. B-325 Positionen des Rahmenauftrags.]*

Damit sind die Vorbereitungen für die Abrechnungen abgeschlossen. Sie können jetzt die Forderungsrechnungen und die zugehörigen Produktionsaufträge erfassen.

**So erfassen Sie einen Auftrag zu einem Rahmenauftrag**

1.  Wählen Sie Dokumente > Auftrag > Auftrag.
2.  Wählen Sie im Menü Bearbeiten > Neu.
3.  Tragen Sie die Kopfdaten im Register Dokument ein.

    *[Image: Abb. B-326 Produktionsauftrag zum Rahmenauftrag. A: Dokumententyp Produktionsauftrag, B: Abrechnungsnummer.]*

4.  Wählen Sie den Dokumententyp (A) Produktionsauftrag.
5.  Tragen Sie die Abrechnungsnummer (B) ein.
    Die Abrechnungsnummer steht nicht mehr zur Verfügung, wenn die veranschlagte Menge aus dem Rahmenauftrag ausgeschöpft ist.
6.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
7.  Wechseln Sie zum Register Positionen und erfassen Sie die Positionen und Mengen, die gefertigt und geliefert werden sollen.
    Sie können jetzt auch Modelle, Sprossen und Bearbeitungen zu den Positionen erfassen.
8.  Bearbeiten Sie den Auftrag weiter, z. B. indem Sie ihn an die Produktion und /oder den Einkauf übergeben.

Im Dialog **Abrechnungen** können Sie sich anzeigen lassen, welche Aufträge bisher erfasst wurden und welche Mengen noch offen sind.

*[Image: Abb. B-327 Zugeordnete Aufträge.]*

**So erstellen Sie eine Forderungsrechnung**

1.  Wählen Sie Dokumente > Objektabrechnungen > Abrechnungen.
    Der Dialog Abrechnungen wird geöffnet.
2.  Lassen Sie sich die Abrechnung anzeigen, zu der Sie eine Forderungsrechnung erstellen wollen.
3.  Wählen Sie im Menü Funktionen > Forderungsrechnung erstellen.

    *[Image: Abb. B-328 Forderungsrechnung. A: Menge, die abgerechnet werden soll, B: Mengeneinheit.]*

4.  Tragen Sie die Menge (A) und die Mengeneinheit (B) ein, die berechnet werden soll, z. B. 25 Stk.
    Sie können pro Position zwischen Menge, Prozent und Betrag wählen. Die Wahl der ersten Forderung müssen Sie bei den nächsten Forderungen pro Position beibehalten.

5.  Klicken Sie auf [OK], um die Daten zu speichern.
    Die Daten werden gespeichert. Der Dialog wird geschlossen und der Dialog Abrechnungen wird wieder angezeigt. Im Register Rahmenauftrag werden die Werte in den entsprechenden Spalten aktualisiert.

In der Dokumentenverwaltung wird ein Auftrag vom Typ *Forderung* angelegt.

*[Image: Abb. B-329 Dokument Forderung. A: Dokumententyp, B: Abrechnungsnummer.]*

Der Typ *Forderung* (A) und die Abrechnungsnummer (B) werden automatisch gesetzt.

6.  Wechseln Sie in die Positionserfassung und prüfen Sie die Positionen.
    Zu diesem Auftrag können Sie keine Rechnung drucken. Wenn Sie den Rechnungsdruck starten, wird folgende Meldung angezeigt:

    > **Frage [3483]**
    > ? Es werden 1 Dokumente nicht verarbeitet! Möchten Sie den Druck dennoch starten ?
    > [Ja] [Nein]

7.  Starten Sie den Rechnungsdruck trotzdem, damit der Auftragsstatus umgesetzt wird.
    Wenn der Vorgang beendet ist, wird die erfolgreiche Verarbeitung gemeldet.
    Eine Rechnung wurde jedoch nicht erzeugt.

    *[Image: Abb. B-330 Keine Rechnung für Forderungsaufträge. A: Status, B: Rechnungsnummer. The status is set to '95 - Rechnung gedruckt' but the invoice number and amount are 0.]*

    In den Feldern für die Rechnungsnummer und den Rechnungsbetrag wird jeweils der Wert 0 angezeigt. Der Status des Dokuments wird dennoch auf gedruckt umgesetzt. Damit kann die Forderung an die FiBu übergeben und abgeschlossen werden.

**So schließen Sie einen Rahmenauftrag ab**

1.  Wählen Sie Dokumente > Objektabrechnungen > Abrechnungen.
    Der Dialog Abrechnungen wird geöffnet.
2.  Lassen Sie sich das (Abrechnungs-)Objekt anzeigen, das Sie abschließen wollen.
    Wenn alle Mengen erfüllt sind, wird der Status des Objekts auf komplett gesetzt.

3.  Im Register Rahmenauftrag können Sie prüfen, ob alle berechneten Mengen auf 100% gesetzt sind.

    *[Image: Abb. B-331 Rahmenauftrag erfüllt. The calculated percentage for the framework order position is 100%.]*

4.  Öffnen Sie in der Dokumentenverwaltung den Rahmenauftrag und schließen Sie ihn mit dem Rechnungsdruck und der Übergabe an die FiBu ab.

### Verfügbare Dokumententypen

Folgende Dokumententypen können unterschieden werden:

| Typ | Beschreibung |
| :--- | :--- |
| **Anzahlung** | Dieser Dokumententyp wird automatisch bei einer Anzahlung gesetzt. |
| **Eigenfertigung** | Dieser Dokumententyp wird bei der Erfassung eines Auftrages (Produktionsauftrag) gesetzt. |
| **Forderung** | Dieser Dokumententyp wird automatisch bei der Erstellung von Forderungsrechnungen gesetzt. Modul Objektabrechnungsverwaltung. |
| **Interne Verrechnung** | Dieser Dokumententyp wird automatisch bei der Bestellübergabe gesetzt. Modul Profit-Center-Verrechnung. |
| **Interner Auftrag** | Dieser Dokumententyp wird automatisch bei der Bestellübergabe gesetzt. Modul Interne Aufträge (mehrstufige Produktion). |
| **Kundenmaterial** | Dieses Kennzeichen muss manuell gesetzt werden. Es hat zur Folge, dass alle Positionen automatisch auf die Beschaffungsart Kundeneigenes Glas gesetzt werden. |
| **Lagerbestellung** | Dieser Dokumententyp wird bei der Lagerbestellung gesetzt. Dieses Kennzeichen kann aber auch manuell in einem Bestellauftrag gesetzt werden. |
| **Reklamation** | Der Dokumententyp wird automatisch bei der Reklamationserfassung gesetzt. Dieses Kennzeichen kann aber auch manuell im Auftrag gesetzt werden. |
| **Teillieferung** | Dieser Dokumententyp wird automatisch bei der Erstellung von Teillieferaufträgen gesetzt. |
| **Wertmäßige Buchung** | Dieser Dokumententyp wird automatisch während der Gutschriftenerfassung gesetzt. Mengenwerte wie Stück, Quadratmeter und Laufmeter werden dadurch nicht an die Statistik übergeben. |

⇨ Softwarereferenz, "Firmendaten - Archiv" auf Seite B-978

### Verfügbare Grenztypen

Die Grenztypen sind fest hinterlegt und können nicht bearbeitet werden. Wenn Sie weitere Grenztypen benötigen, wenden Sie sich bitte an die A+W Software GmbH.

**Tab. B-25: Grenztypen für die Preisdefinition**

| Grenztyp | Beschreibung | Beispiel |
| :--- | :--- | :--- |
| 1 x Breite+Höhe | Addition von Breite und Höhe. | 600 + 800 = 1400 mm |
| Anzahl Felder | Nur bei Sprossen. | |
| Anzahl Kreuze | Nur bei Sprossen. | |
| Bearbeitungsindex | Bis-Angabe. ⇨ "Bearbeitungsindex" auf Seite B-256 | Bis einschließlich 100. Dieser Wert wird mit Bezug auf die Glasdicke und die Produktart festgelegt. |
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
| Einbauposition | Glaspreis nach Einbauposition gestaffelt. | Beispiel 1: Hauptposition ISO: Einbauposition 1: Float, Einbauposition 2: SZR, Einbauposition 3: ESG... Beispiel 2: Hauptposition ISO: Einbauposition 1: VSG -> Einbauposition 1: Float, Einbauposition 2: Folie, Einbauposition 3: Float... |
| Entfernung | Zuschlagsberechnung der Transport-/ Mautkosten pro Kilometer. | 130 km |
| Hauptprodukt-Nr. | Produktnummer der Hauptposition | |
| Höhe | Bis-Wert der Höhe. | Bis 5800 mm eines Glases. |
| Höhe (Bearb.) | Bis-Wert für Bearbeitungen (Länge der Bearbeitung). | 950 mm bei Randausschnitte. |
| Höhe exakt | Genauer Wert. | 2100 mm für Türen. |
| Kanten-Bearbeitungsgröße | Bearbeitungen wie Facetten und Gehrung. Bei Facetten = Facettenbreite. | |
| Kantenlänge (größte/kleinste) | Bis-Angabe auf der Ebene der Hauptposition. | Kanten polieren. |
| kg/lbs | Gewicht der Einheit. | Zuschlag von Transport-/Mautkosten. |
| kg/lbs pro Pos | Gesamtgewicht der Position. | Zuschlag von Transport-/Mautkosten. |
| Laufmeter | Laufmeter der Einheit. | Sprossen. |
| Laufmeter (Bearb.) | Laufmeter der Bearbeitung. | Kanten polieren. |
| Lfm (gerundet) | Gerundete Laufmeter. ⇨ "Maßberechnung" auf Seite B-152 | |
| Lfm Auftrag Produkt/WGR/WHG/WOG | Gesamte Laufmeter eines Produkts oder einer Warengruppe innerhalb eines Auftrags. | Beispiel Produkt: Position 1: Produkt 1001 = 5 Ifm, Position 2: Produkt 1001 = 10 Ifm, Position 3: Produkt 1002 = 5 Ifm. Grenzmenge: bis 10 Ifm = 5 Euro/lfm, bis 99 Ifm = 4 Euro/lfm. Laufmeter insgesamt pro Auftrag: Produkt 1001 = 15 Ifm = 4 Euro/lfm, Produkt 1002 = 5 Ifm = 5 Euro/lfm. |
| Lfm Position | Gesamtlaufmeter der Position. | |
| Nettowert (Liefertag) | Gesamtauftragswert eines Kunden pro Liefertag. | Modul Anlieferpauschale: Die Anlieferpauschale wird bei der Rechnungsstellung ermittelt. |
| Produktart/-gruppe | Die Produktart/-gruppe eines Glases auf Ebene der Hauptposition oder Stückliste. | Glas, Beschichtung. |
| Qm | Quadratmeter der Position. | Glas |
| Qm (gerundet) | Gerundete Quadratmeter. | Glas |
| Qm (Liefertag) | Gesamtquadratmeter eines Kundenauftrags pro Liefertag. | Modul Anlieferpauschale: Die Anlieferpauschale wird bei der Rechnungsstellung ermittelt. |
| Qm Auftrag Produkt/WGR/WHG/WOG | Siehe Lfm Auftrag Produkt. | |
| Qm Position | Gesamtquadratmeter der Hauptposition. | Glas, Beschichtung. |
| Qm Position (gerundet) | Gerundeter Gesamtquadratmeter der Hauptposition. | Glas |
| Qm Rechteck | Umschriebenes Rechteck (bei Modellen). | Grenztyp für die Preisberechnung ohne Bedeutung. |
| Radius Rundecke (Bearb.) | Radius von Rundecken. | |
| Sprossen | | Grenztyp für die Preisberechnung ohne Bedeutung. |
| Stk Auftrag Produkt/WGR/WHG/WOG | Siehe Lfm Auftrag Produkt. | |
| Stk Position | Gesamtmenge der Position. | |
| Stück | Menge der Positionen. | |
| Stück (Bearb.) | Menge der Bearbeitungen. | |
| SZR | Dicke des SZRs. | |
| SZR (größter) | Größter SZR innerhalb einer ISO-Einheit. | |
