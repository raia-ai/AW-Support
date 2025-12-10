---
title: "A+W Business Master Data - Tutorial 2: Documents"
source: "D-HB-AWBusiness_6.pdf"
tags: ["A+W Business", "ERP", "Master Data", "Documents", "Status Assignment", "Number Ranges", "Rounding", "Invoicing", "Document Printing", "Tutorial"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a tutorial for the A+W Business software, focusing on the configuration and management of documents. It covers status assignments, lock indicators, number ranges, rounding rules, invoicing settings, and text/document printing."
long_description: "This document serves as the second tutorial for managing master data within the A+W Business ERP system, with a specific focus on the 'Documents' module. It provides step-by-step instructions for configuring various aspects of document processing and management. The tutorial begins with status assignments, explaining how to link user statuses to system status points for different document types. It then details how to set up and apply lock indicators (Sperrkennzeichen) to exclude documents from automatic processing steps. A significant portion is dedicated to establishing and managing number ranges (Nummernkreise) for different document types, clients (Mandanten), and work areas (AV-Bereiche) to ensure unique document identification. The guide also covers the configuration of rounding rules (Rundungen), including defining rounding rates, rounding points (e.g., for prices, taxes, areas), and assigning them to clients or specific products. Further, it explains essential settings for invoicing (Faktura), such as managing taxes, currencies, and exchange rates. The final major section focuses on text and document printing, detailing how to create and manage standard texts, use variables and formulas for dynamic content, and configure forms (Formulare) and print jobs for various output formats (paper, PDF, email). An extensive appendix provides supplementary technical details on object/billing management, available document types, system texts, and variables (placeholders)."
---

# Tutorial 2: Dokumente

---
## Statuszuordnung

In the status assignment, you define the relationships between status points and user statuses for documents.

> **Abb. B-271 Felder für neue Zuordnung freigeschaltet**
> This section refers to a user interface for 'Statuszuordnung' (Status Assignment) with the following fields:
> - **A Statuspunkt**: The status point to which the user status should be assigned.
> - **B Dokument**: The document for which the assignment is valid.
> - **C Anwenderstatus**: The user status to be assigned to the status point.
> - **D Mindeststatus**: The minimum status the document must have.
> - **E Sperrstatus**: The lock status that the document must not reach.

1.  (Step 1 and 2 are not detailed in this excerpt)
2.  **Wählen Sie den Statuspunkt (A) und den Dokumententyp (B), für den die Zuordnung gelten soll.**
    
    Achten Sie darauf, welchen Dokumententyp Sie gewählt haben. Wenn Sie `alle` wählen, gilt dieser Status für alle Dokumententypen, und zwar auch dann, wenn dies sinnlos oder hinderlich ist.
    
3.  **Wählen Sie den Anwenderstatus (C) aus, den Sie dem Statuspunkt und dem Dokumententyp zuordnen wollen.**
    
4.  **Wählen Sie ggf. zusätzlich den passenden Mindeststatus (D) und den Sperrstatus (E) aus.**
    
    Achten Sie darauf, dass die neue Zuordnung nicht im Widerspruch zu den vorhandenen Zuordnungen steht.
    
5.  **Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.**
    
    Die Daten werden gespeichert. Die neue Zuordnung wird nun in den Dokumenten als Status angewendet.

---

## Sperrkennzeichen zuordnen

Sperrkennzeichen setzen Sie ein, um Dokumente aus bestimmten Abläufen in der automatischen Verarbeitung auszuschließen.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
- "So legen Sie ein Sperrkennzeichen an" auf Seite B-502
- "So aktivieren Sie das Sperrkennzeichen" auf Seite B-505

> **Änderungen absprechen**
> Sprechen Sie Änderungen der Sperrkennzeichen zuvor mit der A+W Software GmbH ab. Sie vermeiden damit, dass das System u. U. nicht mehr richtig arbeitet.

### So legen Sie ein Sperrkennzeichen an

1.  Wählen Sie im Menü **Stammdaten > Auftrag > Sperrkennzeichen**.
    
    *(Referenced Image: Abb. B-272 Sperrkennzeichen anlegen)*
    
    ⇨ Softwarereferenz, "Sperrkennzeichen" auf Seite B-1034
    
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    
    *(Referenced Image: Abb. B-273 Felder für neues Sperrkennzeichen freigeschaltet)*
    
    - **A Bezeichnung des Sperrkennzeichens**: Description of the lock indicator.
    - **B Anwenderstatus, der gesperrt wird**: User status that is locked.
    - **C Nächstmöglicher Status**: Next possible status.
    
3.  Tragen Sie die Bezeichnung (A) ein, z. B. `Teillieferung ohne Rechnung`.
    
4.  Wählen Sie den Anwenderstatus (B) aus, der gesperrt werden soll, z. B. den `Rechnungsdruck`.
    
5.  Wählen Sie den Anwenderstatus (C) aus, auf den umgeleitet werden soll, z. B. die `Übergabe an die FiBu`.
    
    *(Referenced Image: Abb. B-274 Neues Sperrkennzeichen)*
    
6.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    
    Das Sperrkennzeichen für die Teillieferung ohne Fakturierung wird gespeichert. Sie müssen es nun in den Firmendaten aktivieren.

### So aktivieren Sie das Sperrkennzeichen

1.  Wählen Sie im Menü **Stammdaten > Firma > Firmendaten**.
    Der Dialog Firmendaten wird mit dem Register `Mandant` geöffnet.
2.  Wechseln Sie zum Register `Dokumente`.
    
    *(Referenced Image: Abb. B-275 Firmendaten - Dokumente)*
    
    - **A Sperrkennzeichen für Teillieferung aktivieren**: Activate lock indicator for partial delivery.
    
    ⇨ Softwarereferenz, "Firmendaten - Dokumente" auf Seite B-1066
    
3.  Wählen Sie im Feld `Teillieferung` (A) das Sperrkennzeichen aus.
    
4.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    
    Die Daten werden gespeichert. Zu Teillieferungen kann nun keine Rechnung mehr erstellt werden. Dies gilt für alle Kunden.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Statusverwaltung" auf Seite B-1020
⇨ Softwarereferenz, "Statuspunkte" auf Seite B-1021
⇨ Softwarereferenz, "Statuszuordnung" auf Seite B-1022
⇨ Softwarereferenz, "Sperrkennzeichen" auf Seite B-1034
⇨ Softwarereferenz, "Firmendaten - Dokumente" auf Seite B-1066

---

## Nummernkreise

### Lernziele
- Funktion der Nummernkreise kennenlernen.
- Nummernbereiche einrichten.

### Nutzen
- Nummernkreise legen die Vergabe von eindeutigen (Dokumenten-)Nummern fest.
- Die eindeutigen Nummern gewährleisten, dass Dokumente (und andere Laufnummern) im Geschäftsprozess korrekt weitergeleitet werden.

### Merke

| Begriff | Beschreibung |
| :--- | :--- |
| **Nummernkreise** | Nummernkreise sind: <ul><li>Logische Organisationseinheiten.</li><li>Mittel zur Zusammenfassung von Arbeitsprozessen, die durch Nummernverwalter ausgelöst werden.</li></ul>Nummernkreise können für Dokumente, für die Produktion und für die Finanzbuchhaltung gepflegt werden. In den einzelnen Nummernkreisen sind die Nummernfolgen (Laufnummern) festgelegt, z. B. für die Dokumente. Die Nummernkreise dürfen sich nicht überschneiden. |
| **Basisnummernkreise** | Die Basisnummernkreise der Stammdaten sind vorgegeben und können nicht um zusätzliche Nummernkreise erweitert werden. |
| **Mandant, AV-Bereich, Mitarbeiter** | Nummernkreise können für Mandanten, AV-Bereiche und für Mitarbeiter getrennt festgelegt werden. Auch diese Nummernkreise dürfen sich nicht überschneiden. |
| **Dokumententyp** | Die Nummern für die einzelnen Dokumententypen werden in unterschiedlichen Nummernkreisen festgelegt. Eine Dokumenten-Nummer wird beim Anlegen automatisch aus dem zugeordneten Nummernkreis vergeben. |

### Funktion der Nummernkreise

Nummernkreise sind zum einen logische Organisationseinheiten, zum anderen ein Mittel zur Zusammenfassung von Arbeitsprozessen, die durch einen sogenannten Nummernverwalter ausgelöst werden.

Die Nummernkreise für die Dokumente und andere Laufnummern müssen Sie so einrichten, wie es für Ihr Unternehmen erforderlich ist. Dies gilt insbesondere für folgende Bereiche:
- Dokumenten-Nummern
- Produktion
- FiBu

Die Nummernkreise können für jeden Mandanten und für jeden Bereich der Auftragsverwaltung (AV-Bereich) festgelegt werden. Auf diese Weise kann z. B. ein Dokument anhand seiner Nummer zugeordnet werden.

Für jeden Nummernkreis legen Sie fest, aus welchem Zahlenbereich die (Lauf-)Nummern vergeben werden können.

> **Abb. B-276 Nummernkreise**
> This refers to a UI screen for number ranges with the following fields:
> - **A Bereiche für Nummernkreise**: Areas for number ranges.
> - **B Dokumententypen**: Document types.
> - **C Erste mögliche Nummer**: First possible number.
> - **D Zuletzt vergebene Nummer**: Last used number.
> - **E Letzte mögliche Nummer**: Last possible number.
> - **F Anzahl der vergebenen Nummern**: Number of used numbers.

In diesem Beispiel sehen Sie die Nummernkreise für Dokumente. Pro aufgeführtem Dokumententyp (B) können Sie festlegen, welche Nummernbereiche (C, E) vergeben werden sollen. Eine Dokumenten-Nummer wird automatisch aus dem zugeordneten Nummernkreis vergeben, wenn Sie ein Dokument anlegen. Damit diese Nummer eindeutig ist, dürfen sich die Nummernkreise nicht überschneiden. Dies gilt für alle Nummernkreise, also für Dokumenten-Nummern, FiBu-Nummern und Produktionsnummern.

### Nummern für Dokumente

Einzelne Nummernkreise können gesperrt werden. Damit können Sie steuern, dass bestimmte Dokumente für gesonderte Bereiche nicht erfasst werden können.

**Tab. B-21 Beispiel für Nummernkreise**

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
- Im AV-Bereich ESG-Fertigung liegt der Nummernbereich für das Dokument `Aufträge` im Bereich 100.000 bis 199.999. Für die `Teillieferung` ist der Bereich 2.000.000 bis 2.099.999 und für die `Reklamationen` der Bereich 2.100.000 bis 2.199.999 reserviert. Eine Überschneidung ist damit ausgeschlossen.
- Standardmäßig existiert der AV-Bereich `<k.A.>`, für den aber keine Aufträge erfasst werden sollen. Der Nummernkreis ist daher durch die Werte 0 (von) und 0 (bis) gesperrt. Die 1 (aktuell) steht für ein leeres Dokument.
- Die `Laufnummer AWPOOL` soll immer fortlaufend vergeben werden, unabhängig davon, um welchen AV-Bereich es sich handelt. In diesem Fall wird der Nummernbereich (1 bis 9999) im AV-Bereich `<k.A.>` angegeben. Alle anderen AV-Bereiche werden gesperrt.

Teillieferungen und Reklamation gehören zum Dokumententyp `Aufträge`. Daher dürfen sich deren Nummernkreise nicht überschneiden. Auch für `Gutschriften` und `Rechnungen` werden einzelne Nummernkreise gepflegt. Als Sonderfunktion kann für diese beiden Dokumentenarten derselben Nummernkreis verwendet werden.
⇨ Softwarereferenz, “Gutschrift-Rechnungsnummer" auf Seite B-1069

Für Dokumente besteht zusätzlich die Möglichkeit, unterschiedliche Nummernkreise pro Mitarbeiter zu definieren. Wenn Sie mit verschiedenen AV-Bereichen arbeiten, können Sie z. B. dem Mitarbeiter der Dokumentenerfassung den AV-Bereich zuordnen, für den er zuständig ist.
⇨ Softwarereferenz, "Erfassungsparameter" auf Seite B-1154

> **Weitere Nummernkreise**
> Die Basisnummernkreise der Stammdaten sind standardmäßig vorgegeben und können nicht erweitert werden. Diese Nummernkreise sind im Dialog `Basisnummernkreise` aufgelistet.
>
> Der Nummernkreis für die Verwaltung der Gestelle wird im Dialog `Firmendaten` festgelegt.
> ⇨ Softwarereferenz, "Firmendaten - Versand" auf Seite B-1134

## AV-Bereiche

Zur Auftragsverwaltung können sogenannte AV-Bereiche definiert werden, denen die Aufträge zugeordnet werden.

Beispielsweise können AV-Bereiche eingerichtet werden, um Neukunden abzugrenzen oder um interne Aufträge zu verwalten. Über Schnittstellen können die Aufträge dann automatisch an den betreffenden AV-Bereich zur Produktion weitergeleitet werden. Der AV-Bereich dient außerdem als Sortierkriterium in der Umsatzstatistik.

> **Abb. B-277 AV-Bereiche**
> This refers to a UI screen for defining AV areas with fields for:
> - **A Name des AV-Bereichs**: Name of the AV area (e.g., `ESG-Fertigung`).
> - **B Erlaubte Dokumententypen**: Allowed document types.

Typischerweise beziehen sich AV-Bereiche auf einzelne Abteilungen oder Niederlassungen eines Unternehmens, mit denen standardmäßig zusammengearbeitet wird. Der AV-Bereich `ESG-Herstellung` ist z. B. zuständig für die Herstellung von ESG.

Jedem AV-Bereich müssen eigene Nummernkreise zugeordnet sein, damit die Dokumente korrekt weitergeleitet werden.

Zusätzlich kann jedem Mitarbeiter ein AV-Bereich und Dokumententyp zugeordnet werden. Wenn beispielsweise der AV-Bereich `ISO` (A) nur dafür gilt, fertige ISO-Einheiten (Lagerartikel) zu verwalten, dann muss ihm der Dokumententyp (B) `Produktionsauftrag` zugewiesen werden. Die Aufträge werden dann automatisch in diesem AV-Bereich und dem dazugehörigen Nummernkreis erfasst. Beides kann manuell im jeweiligen Auftrag geändert werden.

⇨ Softwarereferenz, "Erfassungsparameter" auf Seite B-1154
AV-Bereiche richten Sie nach demselben Muster ein, wie alle Basistabellen.
⇨ Tutorial 1, "Basistabelle erweitern" auf Seite B-93

> **AV-Bereiche für die unterschiedlichen Mandanten**
> Legen Sie alle AV-Bereiche fest, die von Ihren Mandanten benötigt werden. Erst beim Einrichten der Nummernkreise werden die AV-Bereiche dem jeweiligen Mandanten zugeordnet.
> Mandanten werden in einer separaten Einheit beschrieben.
> ⇨ Tutorial 1, "Mandanten und Filialen" auf Seite B-442

## Nummernkreise festlegen

Die Nummernkreise dürfen sich nicht überschneiden. Daher werden die Nummernkreise für jede Dokumentenart einzeln festgelegt, um so z. B. Auftrags- und Rechnungsnummern voneinander zu unterscheiden.

> **Nummernkreis nicht im laufenden Betrieb ändern**
> Wenn Sie die Nummernkreise im laufenden Betrieb ändern, kann das zu Konflikten mit alten Dokumenten-Nummern führen. Prüfen Sie bitte vorher sorgfältig, dass keine unverarbeiteten Dokumente in den Nummernverwaltern stehen.

> **Voraussetzung**
> Wenn Sie mit Mandanten arbeiten, müssen diese angelegt sein, bevor Sie die Nummernkreise einrichten. Legen Sie sich einen Schulungsmandanten auch dann an, wenn Sie in ihrem Geschäftsbetrieb nicht mit Mandanten arbeiten. Sie können ihn nach den Übungen wieder löschen.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
- "So legen Sie die Nummernkreise fest" auf Seite B-511
- "So sperren Sie einen Nummernkreis für einen AV-Bereich" auf Seite B-513

### So legen Sie die Nummernkreise fest

1.  Wählen Sie im Menü **Stammdaten > Auftrag > Nummernkreise**.
    Der Dialog `Nummernkreise` wird geöffnet.
    ⇨ Softwarereferenz, "Nummernkreise" auf Seite B-1028
    Prüfen und notieren Sie, welche Nummernfolgen noch nicht belegt sind. Wenn Sie keine „Lücken" entdecken können, dann reduzieren Sie die Nummernfolgen des aktuellen Mandanten.
    Unter Umständen können Sie die höheren Nummernfolgen freimachen, z. B. zwischen 100000 und 99999999.
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    > **Abb. B-278 Felder für neue Nummernkreise freigeschaltet**
    > This refers to a UI screen for setting up new number ranges with the following fields:
    > - **A Mandant auswählen**: Select client.
    > - **B AV-Bereich auswählen**: Select AV area.
    > - **C Mitarbeiter auswählen**: Select employee.
    > - **D Nummernfolge festlegen**: Define number sequence.
    Die Nummernfelder sind mit den Werten vorbelegt, die für den ersten Mandanten reserviert wurden.
3.  Wählen Sie ggf. den Mandanten (A) aus, z. B. Ihren Schulungsmandanten.
4.  Wählen Sie als AV-Bereich (B) und Mitarbeiter (C) jeweils den Eintrag `<k.A.>` aus.
5.  Tragen Sie für Angebote (D) in den Feldern `von` und `bis` die Nummern ein.
    Die Nummern können bis zu 8 Stellen haben.
    Wenn Sie für die gewählte Kombination von Mandant, AV-Bereich und Mitarbeiter die Erfassung sperren wollen, so geben in den Feldern `von` und `bis` jeweils den Wert 0 ein und im Feld `aktuell` den Wert 1.
6.  Wiederholen Sie diesen Schritt für alle Dokumente.
7.  Wählen Sie im Menü **Funktionen > Prüfung**.
    Wenn Überschneidungen mit anderen Nummernkreisen festgestellt wurden, wird eine Meldung angezeigt.
    > **Meldung [1720]**
    > Überschneidung zwischen AV-Bereich Vitropur, Nummernkreis Gutschrift und AV-Bereich Isolierglasfertigung, Nummernkreis Gutschrift...
8.  Korrigieren Sie Ihre Einträge, bis bei der Prüfung keine Fehler mehr gemeldet werden.
9.  Wiederholen Sie die Schritte 5 und 7 in den anderen Registern, um weitere Laufnummern einzutragen.
    Im Register `Tabelle` können Sie prüfen, welche Nummernkreise Sie bereits definiert haben.
10. Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.

### So sperren Sie einen Nummernkreis für einen AV-Bereich

1.  Wählen Sie im Menü **Stammdaten > Auftrag > Nummernkreise**.
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
3.  Wählen Sie den AV-Bereich aus.
4.  Tragen Sie für Angebote in den Feldern `von` und `bis` den Wert 0 ein.
5.  Geben im Feld `aktuell` den Wert 1 ein.
6.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert. Damit können im gewählten AV-Bereich keine Angebote erfasst werden. Wiederholen Sie die Schritte für alle Dokumententypen, die in dem AV-Bereich nicht erfasst werden dürfen.

### Übungen
Um die Nummernfolgen in dieser Übung zu bearbeiten, benötigen Sie einen neuen (eigenen) Mandanten. Mandanten werden in den Firmendaten angelegt. Dazu gibt es eine separate Einheit. Die folgende Handlungssequenz ist daher stark verkürzt.

#### So legen Sie einen Mandanten für die Übung an
1.  Wählen Sie im Menü **Stammdaten > Firma > Firmendaten**.
    Der Dialog `Firmendaten` wird geöffnet.
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    Die Felder werden freigeschaltet.
3.  Tragen Sie die Nummer, den Matchcode und den Namen ein.
4.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.

**Aufgaben:**
- Legen Sie die Nummernkreise für Ihren Schulungsmandanten fest.
- Notieren Sie, welche Nummern bereits für Dokumente reserviert sind.
- Legen Sie die Nummernfolgen für Dokumente fest.
- Prüfen Sie, ob es Überschneidungen gibt, und korrigieren Sie diese ggf.
- Erfassen Sie einen Auftrag für diesen Mandanten und prüfen Sie, ob die Auftragsnummer aus dem richtigen Nummernkreis genommen wurde.

**Ergänzende Informationen**
⇨ Tutorial 1, "Finanzbuchhaltung (FiBu)" auf Seite B-440
⇨ Softwarereferenz, "Nummernkreise" auf Seite B-1028
⇨ Softwarereferenz, "Firmendaten - Mandant" auf Seite B-1056
⇨ Softwarereferenz, "AV-Bereiche" auf Seite B-1160

---

## Rundungen

### Lernziele
- Rundungseinstellungen prüfen.
- Rundungen zuordnen.
- Rundungen für einzelne Marktpartner einrichten.

### Nutzen
- Im Programm errechnete Werte können auf eine gewünschte Anzahl von Stellen gerundet werden.
- Die Rundungseinstellungen beziehen sich immer auf einen bestimmten Rundungspunkt. Sie können daher sehr fein abgestimmt werden.

### Merke

| Begriff | Beschreibung |
| :--- | :--- |
| **Rundungssatz** | Im Rundungssatz sind folgende Einstellungen festgelegt: <ul><li>Anzahl der verbleibenden Nachkommastellen.</li><li>Wert, auf den gerundet wird (letzte, beizubehaltende Ziffer).</li><li>Rundungsart</li></ul> |
| **Rundungsart** | Die Rundungsart gibt an, ob auf- oder abgerundet wird. |
| **Rundungspunkt** | Rundungspunkte geben an, was gerundet werden soll. Die Rundungspunkte sind fest vorgegeben und können nicht bearbeitet werden. Gerundet werden in der Regel: <ul><li>Preise</li><li>Zuschläge</li><li>Steuerbeträge</li><li>Flächen</li></ul> |
| **Rundungszuordnung** | Rundungspunkte und Rundungen müssen einander zugeordnet werden, damit der errechnete Wert gerundet wird. Die allgemeinen Zuordnungen können für bestimmte Produktgruppen gelten. Für einzelne Partner oder Partnergruppen können abweichende Rundungen zugeordnet werden. |

### Rundung
Zur Berechnung der Rundungen werden folgende Einstellungen herangezogen:
- Die Rundung selbst: Sie gibt die Anzahl der Stellen und die Rundungsart an, wie gerundet werden soll, z. B. nach oben.
- Der Rundungspunkt: Er gibt an, was gerundet werden soll, z. B. Preis, Steuer, Fläche.

> **Abb. B-279 Rundung**
> This refers to a UI screen for defining rounding rules with the following fields:
> - **A Rundungswert**: The value to round to (e.g., 5 for rounding to the nearest 0.05).
> - **B Stellen, auf die gerundet wird**: Number of decimal places.
> - **C Rundungsart**: Rounding type.

Bei der Rundungsart haben Sie die folgenden Möglichkeiten zur Rundung:
- **Kaufmännisch**: Die Beträge von 0 bis 4 werden abgerundet, von 5 bis 9 aufgerundet.
- **Nach oben**: Die Ziffern von 1 bis 9 werden aufgerundet.
- **Nach unten**: Die Ziffern von 1 bis 9 werden abgerundet.

**Tab. B-22 Rundungsbeispiele für zwei Stellen**

| Rundungs-wert | Stellen | Beispiel-wert | Rundungsart | | |
| :--- | :--- | :--- | :--- | :--- | :--- |
| | | | **kaufmännisch** | **nach oben** | **nach unten** |
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

### Rundungspunkte
Die Rundungspunkte geben an, was gerundet werden soll, z. B. der Preis für die Fläche. Rundungspunkte sind in A+W Business fest definiert und können nicht bearbeitet werden. In der folgenden Tabelle finden Sie alle Rundungspunkte.

**Tab. B-23 Rundungspunkte**

| Nr. | Rundungspunkte VK | Nr. | Rundungspunkte EK | Beschreibung |
| :-- | :--- | :-: | :--- | :--- |
| 1 | qm-Preis/ME Glasposition | 51 | EK qm-Preis/ME Glasposition | Beispiel 2 |
| 2 | qm-Preis/ME Zuschläge | 52 | EK qm-Preis/ME Zuschläge | Beispiel 3 |
| 3 | qm-Preis/ME Bearbeitungen | 53 | EK qm-Preis/ME Bearbeitungen | Beispiel 3 |
| 4 | Brutto/Stk. Glasposition | 54 | EK Brutto/Stk. Glasposition | Bruttopreise werden nicht angezeigt. |
| 5 | Brutto/Stk. Zuschläge | 55 | EK Brutto/Stk. Zuschläge | |
| 6 | Brutto/Stk. Bearbeitungen | 56 | EK Brutto/Stk. Bearbeitungen | |
| 7 | Brutto/Stk. Stück Glasposition | 57 | EK Brutto/Stk. Stück Glasposition | |
| 8 | Brutto/Stk. Stück Zuschläge | 58 | EK Brutto/Stk. Stück Zuschläge | |
| 9 | Brutto/Stk. Stück Bearbeitungen | 59 | EK Brutto/Stk. Stück Bearbeitungen | |
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

*\* Dieser Preis wird nicht angezeigt. Er ergibt sich aus Nettopreis x Positionsmenge.*
*\*\* FW = Fremdwährung*

#### Beispiele für Rundung
- **Beispiel 1**: Auftrag - Register Summen (Abb. B-280) - Refers to rounding points 18, 19, 28, 118, 119, 128.
- **Beispiel 2**: Positionserfassung – Register ISO/Artikel (Abb. B-281) - Refers to rounding points 10, 16, 17, 21, 27.
- **Beispiel 3**: Positionserfassung – Register Stückliste (Abb. B-282) - Refers to rounding points 2, 3, 11, 12, 14, 15, 17, 22, 23, 25, 26.

### Rundungszuordnung
Die definierten Rundungen und die Rundungspunkte müssen einander zugeordnet werden. Dabei können die Zuordnungen für Produktarten/Produktgruppen, für Mandanten und für Partner unterschiedlich definiert werden.

Die im Dialog `Rundungszuordnung` festgelegten Zuordnungen gelten für alle Berechnungen eines Mandanten, es sei denn, sie werden von Zuordnungen für Kunden oder Lieferanten übersteuert.

> **Abb. B-283 Standardzuordnung von Rundungen pro Mandant**
> In diesem Beispiel sehen Sie, dass in der markierten Zeile der berechnete Flächenpreis auf drei Stellen nach dem Komma gerundet wird. Diese Einstellung gilt für alle Produktarten und Produktgruppen.

> **Maßrundungen**
> Maßrundungen sind von den Rundungseinstellungen nicht betroffen. Sie werden in verschiedenen Dialogen zur Produkt- und Preisdefinition angegeben. Das Programm sucht in der Reihenfolge Individualpreise > Rabatte > Preise > Produkte > Partner nach Angaben. Die Suche wird beendet, sobald eine Angabe gefunden wurde.

### Rundung für Marktpartner
Neben den allgemeinen Rundungszuordnungen können weitere Rundungssätze angelegt und diese einzelnen Kunden oder Lieferanten zugeordnet werden. So müssen z. B. bei Währungen, deren kleinste Münzeinheit 0,05 ist, Geldbeträge immer entsprechend gerundet werden.

Bei Schweizer Kunden wird z. B. die Mehrwertsteuer gerundet (5 Rappen). Dafür müssen Sie einen entsprechenden Satz anlegen und Ihren Schweizer Kunden zuordnen.

> **Abb. B-284 Zuordnung von Rundungen pro Kunde**
> In diesem Beispiel sehen Sie, dass für den ausgewählten Kunden eine eigene Rundung verwendet werden soll, wenn das erfasste Produkt ein ISO ist. Bei allen anderen Produkten gelten für ihn die allgemeinen Rundungszuordnungen.

## Rundung zuordnen
Rundungszuordnungen müssen in der Regel nur bei Änderungen neu festgelegt werden, z. B. für einen neuen Kunden oder einen neuen Mandanten.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
- "So legen Sie eine Rundung an" auf Seite B-523
- "So ordnen Sie eine Rundungstabelle zu" auf Seite B-524

### So legen Sie eine Rundung an
1.  Wählen Sie im Menü **Stammdaten > Auftrag > Rundung**.
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    > **Abb. B-285 Felder für neuen Rundungssatz freigeschaltet**
    > This refers to a UI for creating a new rounding rule.
    > - **A (Sprechende) Bezeichnung**: Descriptive name (e.g., MwSt. Schweiz).
    > - **B Rundungswert**: Value to round to (e.g., 0.05).
    > - **C Stellen**: Number of decimal places.
    > - **D Art der Rundung**: Rounding type.
3.  Tragen Sie die Bezeichnung (A) ein.
4.  Tragen Sie den Rundungswert (B) ein, auf den gerundet werden soll, z. B. 0,05.
5.  Tragen Sie die Anzahl der Stellen (C) ein, z. B. 2.
6.  Wählen Sie die Rundungsart (D) aus, z. B. `kaufmännisch`.
7.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert. Sie können diese Rundung jetzt bei den allgemeingültigen Rundungszuordnungen oder bei den partnerspezifischen Rundungszuordnungen auswählen.

### So ordnen Sie eine Rundungstabelle zu
1.  Wählen Sie im Menü **Stammdaten > Marktpartner > Kunde > Rundung**.
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    > **Abb. B-286 Felder für neue Rundungszuordnung freigeschaltet**
    > - **A Kunde, für den die Rundung gilt**
    > - **B Rundungspunkt**
    > - **C Produktart/Produktgruppe**
    > - **D Preiseinheit**
    > - **E Rundungstabelle**
    > - **F Abweichende Rundungszuordnungen**
3.  Wählen Sie den Kunden (A) aus.
4.  Wählen Sie den Rundungspunkt (B) aus, z. B. `MWST 1`.
5.  Wählen Sie in den Feldern die Produktart (C) und Preiseinheit (D) aus. Wenn Sie z. B. `<k.A>` wählen, gelten die Einstellungen für diesen Kunden immer.
6.  Wählen Sie die Rundungstabelle aus, die Sie für diesen Kunden eingerichtet haben, z. B. `Rundung auf 0,05`.
7.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Für den ausgewählten Kunden wird diese neue Rundung verwendet. Bei allen anderen Rundungspunkten gelten für ihn weiterhin die allgemeinen Rundungszuordnungen.

### Übungen
- Prüfen Sie, welche Rundungen und Rundungszuordnungen bereits angelegt sind.
- Ordnen Sie Ihrem Schulungsmandanten folgende Rundungen zu:
    - Bei allen Glaspositionen soll kaufmännisch auf 3 Stellen gerundet werden.
    - Bei allen Stück-Preisen soll immer auf 0,05 aufgerundet werden. Legen Sie diese Rundung an, wenn im Dialog `Rundung` noch kein entsprechender Eintrag vorhanden ist.
- Ordnen Sie Ihrem Schulungskunden eine kaufmännische Rundung der Mehrwertsteuer auf 0,05 zu.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Rundung (Kunde, Lieferant)" auf Seite B-970
⇨ Softwarereferenz, "Rundung Kunden-, Lieferantengruppen" auf Seite B-971
⇨ Softwarereferenz, "Rundung" auf Seite B-1015
⇨ Softwarereferenz, "Rundungspunkte" auf Seite B-1017
⇨ Softwarereferenz, "Rundungszuordnung" auf Seite B-1018

---

## Einstellungen zur Faktura
Neben den Einstellungen zur Preisberechnung werden zur Verarbeitung der Dokumente weitere Angaben benötigt, z. B. für den Zahlungsverkehr und die Berechnung der Mehrwertsteuer.

Dazu gehören folgende Lerneinheiten:
- "Finanzen" auf Seite B-528
- "Automatische Zuschläge" auf Seite B-394

In eine Rechnung müssen mindestens folgende Bestandteile aufgenommen werden:
- **Angaben zum Aussteller**
    - Name und Anschrift des Unternehmens
    - Steuernummer und/oder Umsatzsteuer-Identifikationsnummer
    (Diese Angaben legen Sie im Dialog `Firmendaten` fest.)
- **Angaben zum Empfänger (Kunde)**
    - Name und Anschrift
    (Diese Angaben legen Sie im Dialog `Partnerverwaltung` fest.)
- **Angaben zur Lieferung/Leistung**
    - Termin der Lieferung
    - Menge und Bezeichnung der gelieferten Produkte
    - Nettobeträge, ggf. nach Steuersätzen aufgeschlüsselt
    - Steuerbeträge
    - Ausstellungsdatum (= Rechnungsdatum)
    - Eindeutige Rechnungsnummer
    (Diese Angaben sind im Auftrag enthalten.)

Darüber hinaus können Sie u. a. Bankverbindungen, Zahlungsbedingungen, Währungen und Steuersätze angeben.

### Finanzen

#### Lernziele
- Dialoge der Basisdaten für das Rechnungswesen kennenlernen.
- Einstellungen für Zahlungsbedingungen prüfen und festlegen.

#### Nutzen
- Alle Daten, die für die kaufmännische Rechnungslegung und für die Finanzbuchhaltung benötigt werden, werden als Basisdaten angelegt und den Marktpartnern und Produkten zugeordnet. Diese Daten werden daher nur einmal erfasst und zentral gepflegt.

#### Merke

| Begriff | Beschreibung |
| :--- | :--- |
| **Steuersätze** | Nur die Steuern können berechnet werden, die als Steuersatz hinterlegt sind. Steuersätze werden den Produkten und den Marktpartnern zugewiesen. Sie können im Dokument überschrieben werden. |
| **Währungen** | Preise können in unterschiedlichen Währungen gepflegt werden. Dabei können Aufträge in Landeswährung (Eigenwährung) oder Fremdwährung erfasst werden. Für statistische Vergleiche wird immer die Landeswährung herangezogen. |
| **Banken** | Aus den (vollständig) hinterlegten Bankdaten kann in den Partnerstammdaten die IBAN erzeugt werden. |
| **Zahlungsbedingungen** | Zahlungsbedingungen werden den Marktpartnern zugewiesen. Sie können im Dokument überschrieben werden. |
| **Fremdschlüssel** | In den Dialogen, in denen Daten für die Buchhaltung hinterlegt werden, verweist ein Fremdschlüssel auf die entsprechenden Buchungsfelder im Programm zur Finanzbuchhaltung (FiBu). |

### Steuern
Für die Berechnung der Steuern in den Dokumenten müssen Steuersätze hinterlegt werden. Diese Steuersätze werden den Produkten und den Marktpartnern zugewiesen.

> **Abb. B-287 Steuersätze**
> This refers to a UI for defining tax rates with the following fields:
> - **A Prozentsatz der Steuer**: Tax percentage.
> - **B Erlöskonto Debitoren, Kreditoren**: Revenue account for debtors, creditors.
> - **C Fremdschlüssel (je nach FiBu-Programm)**: External key (depending on the accounting program).

Sie können beliebig viele Steuersätze anlegen. In den Stammdaten der Produkte und der Marktpartner können aber nur die ersten fünf zugewiesen werden. Die zusätzlichen Steuersätze stehen dagegen auch im Dokument zur Verfügung.

### Währungen
Als international agierendes Unternehmen müssen Sie mit mehr als einer Währung arbeiten. Sie können in A+W Business die Preise für den Einkauf und für den Verkauf pflegen, auch wenn diese in unterschiedlichen Währungen anfallen.

Zum Erfassen von Aufträgen kann A+W Business auf der Basis von zwei verschiedenen Währungseinstellungen arbeiten:
- **Landeswährung (Eigenwährung)**: Die Währung im Land Ihres Hauptsitzes. In Europa ist dies in der Regel der Euro.
- **Fremdwährung**: Die von der Landeswährung abweichende Währung, in der z. B. im Auftrag die Preise für ausländische Kunden ausgewiesen werden.

Für statistische Vergleiche wird immer die Landeswährung herangezogen. Die Währungsbeträge werden dazu von A+W Business umgerechnet.

> **Abb. B-288 Firmendaten – Register Steuer, Währungseinstellungen**
> - **A Währung, in der A+W Business rechnet**: Currency in which A+W Business calculates (home currency).
> - **B Default-Einstellung für Auftragserfassung**: Default setting for order entry (None, Home Currency, Foreign Currency).
> - **C Währung der Preisanzeige im Auftrag**: Currency for price display in the order.

#### Preisberechnung bei Fremdwährungen
Die Berechnung von Preisen kann bei Fremdwährungen zu unterschiedlichen Ergebnissen führen, wenn Mengenpreise auf unterschiedlichen Ebenen ermittelt werden. Diese Einstellung legen Sie in den Firmendaten fest.
⇨ Softwarereferenz, "Fremdwährungsbetrag aus Stückpreis x Menge bilden" auf Seite B-1089

Wenn der Fremdwährungsbetrag auf der Basis der Stückliste und der Menge gebildet werden soll, können die Beträge auf folgende Arten errechnet werden:

- Der Positionspreis wird aus dem Positionspreis in Landeswährung gebildet.

| Landeswährung (LW) | | Fremdwährung (FW) |
| :--- | :--- | :--- |
| LW Preis/PE | x Faktor | = FW Preis/PE |
| LW Bruttostückpreis | x Faktor | = FW Bruttostückpreis |
| LW Nettostückpreis | x Faktor | = FW Nettostückpreis |
| **LW Positionspreis** | **x Faktor** | **= FW Positionspreis** |

- Der Positionspreis wird aus dem Nettostückpreis in Fremdwährung gebildet.

| Landeswährung (LW) / Fremdwährung (FW) | | Ergebnis |
| :--- | :--- | :--- |
| LW Preis/PE | x Faktor | = FW Preis/PE |
| LW Bruttostückpreis | x Faktor | = FW Bruttostückpreis |
| LW Nettostückpreis | x Faktor | = FW Nettostückpreis |
| **FW Nettostückpreis** | **x Menge** | **= FW Positionspreis** |

### Wechselkurse
Die Wechselkurse hinterlegen Sie im Dialog `Währungen`. Wenn eine der angegebenen Währungen nicht mehr verwendet werden soll, kann sie gesperrt werden.

> **Abb. B-289 Währungen**
> This refers to a UI for managing exchange rates with the following fields:
> - **A Wechselkurs für die Fremdwährung**: Exchange rate for the foreign currency.
> - **B Name der Währung**: Name of the currency.
> - **C Währung sperren**: Lock currency.

Sie können mit besonderen Kunden eigene Umrechnungsfaktoren vereinbaren, die jeweils im Auftrag angegeben werden. Die Preise des Auftrags werden dann nicht mit dem hinterlegten Umrechnungsfaktor berechnet, sondern mit dem im Auftrag angegebenen.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Steuer" auf Seite B-1040
⇨ Softwarereferenz, "Zahlungsbedingungen" auf Seite B-1042
⇨ Softwarereferenz, "Banken" auf Seite B-1044
⇨ Softwarereferenz, "Währung" auf Seite B-1045
⇨ Softwarereferenz, "Währungseinstellungen" auf Seite B-1059
⇨ Softwarereferenz, "Währungsanzeige in Auftragserfassung" auf Seite B-1060

---

## Text- und Dokumentendruck

Zu den Dokumenten können standardisierte Texte erfasst und wahlweise in den verschiedenen Dokumenten gedruckt werden. In diesem Themenblock lernen Sie, welche Texte zur Verfügung stehen und wie Sie den Formulardruck steuern können.

Dazu gehören folgende Lerneinheiten:
- "Texte" auf Seite B-534
- "Formulare" auf Seite B-545

### Texte

#### Lernziele
- Unterschiede der Textarten für automatische Texte kennenlernen.
- Funktion der Textkennzeichen kennenlernen.
- Variablen in Texten einsetzen.
- Texte hinterlegen und bearbeiten.

#### Nutzen
- Häufig benötigte Texte können hinterlegt und in die Dokumente übernommen werden, ohne dass sie jeweils eingegeben werden müssen.
- Variablen vervollständigen einen Text anhand der Werte, die im Dokument erfasst wurden.

#### Merke

| Begriff | Beschreibung |
| :--- | :--- |
| **Textarten** | Automatische Texte werden nach ihrer Verwendung unterschieden: <ul><li>Systemtexte</li><li>Standardtexte</li><li>Rahmentexte</li><li>Mahntexte</li><li>Gütetexte</li><li>CEKAL-Texte</li></ul> |
| **Textkennzeichen** | Texte werden anhand des Textkennzeichens in den Dokumenten zur Auswahl gefiltert und/oder an die Schnittstellen (Produktion, FiBu) übergeben. |
| **Variablen** | In den Texten können Variablen (Platzhalter) eingesetzt werden. Diese lesen die Werte aus den Dokumenten aus. |
| **Formeln** | Variablen können zu Formeln zusammengestellt werden, die einen Wert im Dokument errechnen. |

### Textarten
Immer wiederkehrende Texte können Sie hinterlegen und automatisch z. B. im Dokument einfügen lassen. Bei diesen Texten wird zwischen System-, Standard- und Rahmentexten unterschieden. Zusätzlich können Sie Mahntexte hinterlegen, die in Mahnungen mit einer Mahngebühr verknüpft werden können.

#### Systemtexte
Dies sind Texte, die fest hinterlegt sind. Sie können keine neuen Systemtexte anlegen und die vorhandenen nicht löschen. Den Wortlaut eines Systemtextes können Sie sinngemäß ändern.

#### Standardtexte
Alle Texte, die häufig in Ihren Dokumenten gedruckt werden, können Sie als Standardtexte hinterlegen. Die Texte werden in verschiedenen Dialogen eingegeben, ausgewählt und/oder bearbeitet.

#### Rahmentexte
Für jede ISO-Einheit können spezielle Rahmentexte hinterlegt und dem Produkt zugeordnet werden. Dabei werden zwei Varianten unterschieden:
- Im Standardtext werden Variablen (Platzhalter) angegeben, so dass der Rahmentext anhand der Werte aus dem Dokument gebildet wird.
- Pro ISO-Einheit wird eine feste Nummer an den Rahmenbieger übergeben. Anhand der übergebenen Nummer setzt der Rahmenbieger automatisch den richtigen Text ein.

#### Mahntexte
Als Mahntext kann nur definiert werden, in welcher Art und Weise der Kunde gemahnt werden soll. Das Kennzeichen wird an die Finanzbuchhaltung übergeben.

#### Gütetexte
Für die Gütetexte gibt es pro Land unterschiedliche Anforderungen. Anhand des Landeskennzeichens der Lieferadresse wird der entsprechende Gütetext in den Rahmentext eingefügt.

#### CEKAL
In Frankreich müssen ISO-Gläser, die mit dem Zertifikat CEKAL gekennzeichnet sind, fest definierten Qualitätskriterien entsprechen. Die aktuellen CEKAL-Normen können frei definiert werden. Bei der Erfassung einer ISO-Einheit wird ein CEKAL-Text anhand der hinterlegten Regeln erstellt.

### Textkennzeichen und Standardtexte
Standardtexte werden anhand von Textkennzeichen unterschieden, z. B. das Textkennzeichen `O` für Angebote, `P` für Produktion, `L` für Lieferschein. Die Textkennzeichen können Sie nach den Erfordernissen in Ihrem Betrieb hinterlegen.

**Beispiele:**
- **Info-Texte (Textkennzeichen /):** Diese Texte sollen in allen Dokumenten gedruckt werden.
- **Lieferscheinspezifische Texte (Textkennzeichen L):** Diese Texte sollen nur auf den Lieferscheinen gedruckt werden.
- **Angebotstexte (Textkennzeichen O):** Diese Texte sollen nur auf Angeboten gedruckt werden.

Über das Textkennzeichen steuern Sie, welche Texte in welchen Dokumenten gedruckt oder an die Produktion übergeben werden.

### Variablen
Allgemeine Texte und Systemtexte können mit Platzhaltervariablen definiert werden. Diese dienen dazu, die entsprechenden Daten erst dann einzutragen, wenn ein Dokument erstellt wird.

**Beispiel:**
Die Angabe des Datums wird typischerweise mit einer Variablen geschrieben. Das Datum wird aus dem Systemdatum gelesen und eingesetzt, wenn das Dokument oder die Datei erzeugt wird. Die Variable `<d1>` wird im Dokument automatisch durch das Datum *Gültig von* ausgetauscht und die Variable `<d2>` durch das Datum *Gültig bis*.

Die Variablen werden bei folgenden Ausgaben eingesetzt:
- Bearbeitungstexte
- Produktdefinition
- Rahmentexte, CEKAL-Texte
- Exportdateien

### Formeln
Variablen können in einem Text zu Formeln verknüpft werden, in denen eine Größe anhand der Angaben aus dem Dokument berechnet wird.

**Beispiel:**
In der Produktdefinition für "Kante(n) gesäumt" lautet der Text: `Säumen von <%> Kante(n) *<§>*`.
- `<%>`: Anzahl der Kanten
- `<§>`: Nummern der Kanten
- `<=>`: Gesamtlänge

Bei einer Scheibe mit den Maßen 1200 x 1800 mm ergibt sich die Berechnung: 4 Kanten = 6000 mm Gesamtlänge der Bearbeitung.

### Dateianhang
Sie können an einen Auftrag auch Dateien anhängen, z. B. mit detaillierten Angaben zur Kalkulation oder zu Modellen. Über Kennzeichen können Sie steuern, welche Dateianhänge weitergeleitet werden, z. B. an die Produktion.

Dateianhänge werden in folgenden Fällen weitergeleitet:
- **Produktionsübergabe:** Dateianhänge für Übergabe in OrderXML.
- **Dokumente kopieren:** Angebot zu Auftrag, z. B. Kalkulationsinformationen.
- **Bestellübergabe:** z. B. Produktinformationen.

Das Standard-Kennzeichen `A` zeigt an, dass alle Dateianhänge übergeben werden. Davon ist nur die Bestellübergabe ausgenommen.

### Texte anlegen

> **Voraussetzung**
> Um Texte vollständig zu hinterlegen, müssen die Textkennzeichen angelegt sein.

#### So legen Sie einen Standardtext an
1.  Wählen Sie im Menü **Stammdaten > Texte > Texte**.
2.  Wählen Sie im Menü **Start > Neu**.
    > **Abb. B-298 Felder für neuen Text freigeschaltet**
    > - **A Frei wählbare Nummer**: Freely selectable number.
    > - **B Matchcode**: Matchcode.
    > - **C Textkennzeichen**: Text indicator.
    > - **D Eingabe des Textes**: Text input.
3.  Geben Sie die Nummer (A) ein.
4.  Geben Sie den Matchcode (B) ein. Der Matchcode sollte ein Schlagwort aus dem Text verwenden.
5.  Wählen Sie das Textkennzeichen (C) aus, z. B. `I Infotext`.
6.  Schreiben Sie den gewünschten Text in das Eingabefeld (D).
7.  Wählen Sie im Menü **Start > Speichern**.

> **Fremdsprachige Texte**
> Fügen Sie die Übersetzungen in den jeweiligen Sprachen auf die gleiche Weise ein. Um Verwechslungen zu vermeiden, wählen Sie dabei dasselbe Textnummern wie im Originaltext.

---

## Formulare

### Lernziele
- Funktion der Formulare kennenlernen.
- Einstellungen für den Druck von Preisen und Skizzen prüfen.
- Druckausgabe von Formularen anpassen.
- Direktdruck und Druckjobs einrichten.

### Nutzen
- Dokumente werden in Formulare gedruckt und in verschiedenen Formaten ausgegeben, um sie zu versenden.
- Der Druck kann in geringem Maß angepasst werden.

### Merke

| Begriff | Beschreibung |
| :--- | :--- |
| **Druckpunkt** | Druckpunkte sind Programmpunkte, an denen ein Dokument gedruckt werden kann. |
| **Status** | Durch den Druck eines Dokuments wird der Status hochgesetzt. Ein Dokument kann nur einmal den Status für den Originaldruck erreichen. |
| **Formular** | Formulare sind fest definierte Dateien, die an das Layout in Ihrem Unternehmen angepasst sind. Für die Druckpunkte muss mindestens ein Formular hinterlegt sein. |
| **Direktdruck** | Zu den fünf Dokumententypen können unterschiedliche Einstellungen gespeichert werden, mit denen ein Dokument direkt gedruckt werden kann, ohne den Dialog `Formular-/Etikettendruck` zu öffnen. |
| **Druckauftrag** | Wenn der Druck über einen zentralen Printserver gestartet wird, können Druckaufträge definiert werden, die den Druck automatisieren. |

### Formularverwaltung
Dokumente werden in Formularen gedruckt. Die Formulare sind im Standard-Layout Ihrer Firma gestaltet.

**Druckpunkt**
Druckpunkte sind Programmpunkte, an denen ein Dokument gedruckt werden kann. Diesen Druckpunkten entspricht jeweils ein Status(punkt). Es wird zwischen Erstdruck und Wiederholungsdruck unterschieden.

**Beispiele für Druckpunkte**

| Kennzeichen | Typ | Bezeichnung |
| :--- | :--- | :--- |
| 100 | 2 (Auftrag) | AB Druck |
| 101 | 1 (Angebot) | Angebote Druck |
| 102 | 2 | Lieferschein Druck |
| 103 | 2 | Rechnung Druck |
| 200 | 2 | AB WH-Druck (Wiederholung) |
| 300 | 2 | Fax AB Druck |
| 350 | 2 | Mail AB Druck |

### Formularzuordnung
Sie können jedem Druckpunkt beliebig viele Formulare zuordnen. Die Formulare müssen als Vorlagedatei im Format `*.qrp` abgelegt sein.

> **Abb. B-299 Zuordnung von Formularen**
> - **A Kennzeichnung des Standard-Formulars**: Indicator for the standard form.
> - **B Aktueller Druckpunkt**: Current print point.
> - **C Anzahl der Druckexemplare**: Number of copies.
> - **D Dateiname des Formulars**: Filename of the form.
> - **E Statusumleitung**: Status redirection (e.g., for cash sales).
> - **F Liste der zugeordneten Formulare**: List of assigned forms.

### Druck
Beim Druck von Dokumenten werden nur die Formulare angeboten, die dem Dokumententyp zugeordnet sind. Für den Druck können Sie Direktdruck oder Druckaufträge (Druckjobs) einrichten.

### Ausgabeformat
Sie können alle Dokumente über die hinterlegten Formulare in verschiedenen Formaten ausgeben:
- Druck auf Papier
- PDF
- RTF
- E-Mail
- Fax
- XML

### Druckanpassung
Die Druckausgabe können Sie in begrenztem Rahmen anpassen. Neben den Kopf- und Fußzeilen z. B.:
- Druck von Skizzen, Preisen, Produktbezeichnungen usw.
- Textkennzeichen für Texte, die nicht gedruckt werden.
- Seitenumbruch
- Standarddrucker

#### Preisdruck
Der Druck der Preise im Formular wird an unterschiedlichen Stellen festgelegt, die sich gegenseitig beeinflussen:
- **Formularverwaltung:** Übergreifende Einstellungen.
- **Partnerverwaltung:** Gibt an, wie detailliert Preise gedruckt werden.
- **Produktverwaltung:** Gibt an, ob Preise explizit oder implizit dargestellt werden.
- **Dokumentenverwaltung (Auftrag):** Gibt an, wie detailliert Preise gedruckt werden.

**Druckeinstellungen für Preise in der Formularverwaltung:**
- **0 - Standard** oder **2 - Preise immer drucken (Summenmodus):** Die Angaben aus dem Dokument werden übernommen.
- **1 - Preise immer drucken:** Die Einstellungen aus dem Dokument werden ignoriert. Die Preise werden pro Auftragsposition gedruckt.

**Druck von Positions- und Summenpreisen**

| Dokument | Formularverw. | Positionspreise | Summenpreise |
| :--- | :--- | :--- | :--- |
| 0 (Kein Druck) | 0 (Standard) | - | - |
| 1 (Alle Preise) | 0 (Standard) | X | X |
| 2 (Nur Summen) | 0 (Standard) | - | X |
| 0 (Kein Druck) | 1 (Immer) | X | X |
| 1 (Alle Preise) | 1 (Immer) | X | X |
| 2 (Nur Summen) | 1 (Immer) | X | X |
| 0 (Kein Druck) | 2 (Summenmodus) | - | - |
| 1 (Alle Preise) | 2 (Summenmodus) | X | X |
| 2 (Nur Summen) | 2 (Summenmodus) | - | X |
_Legende: - = kein Druck, X = Druck_

#### Skizzendruck
Beim Skizzendruck wird zwischen Modell- und Sprossenskizzen unterschieden. Die Anzeige und der Druck der Skizzen werden in verschiedenen Dialogen festgelegt:
- **Firmendaten:** Legt fest, wie Sprossenskizzen standardmäßig gedruckt werden.
- **Formularverwaltung:** Legt die Details des Skizzendrucks für Modelle und Sprossen fest (Druckmodus, Größe, Textgröße).
- **Produktverwaltung:** Legt fest, ob Skizzen gedruckt werden (maßstäblich oder schematisch).
- **Positionserfassung:** Legt pro Position fest, ob und wie Skizzen gedruckt werden.

> **Gebogenes Glas**
> Die Wölbung von gebogenem Glas wird immer schematisch dargestellt.

**Skizzendruck für Sprossen (Rechteckscheiben)**

| Einstellung zur Position (Sprosse) | Einstellung in der Formularverwaltung | | |
| :--- | :--- | :--- | :--- |
| | **kein Druck** | **schematisch** | **maßstäblich** |
| maßstäblich | kein Druck | schematisch | maßstäblich |
| schematisch | kein Druck | schematisch | schematisch |
| kein Druck | kein Druck | kein Druck | kein Druck |

**Skizzendruck bei Modellscheiben**

| Einstellung zur Position (Modell/Sprosse) | Einstellung in der Formularverwaltung | | |
| :--- | :--- | :--- | :--- |
| | **kein Druck** | **schematisch** | **maßstäblich** |
| Modell maßstäblich | kein Druck | schematisch | maßstäblich |
| Modell schematisch | kein Druck | schematisch | schematisch |
| kein Druck | kein Druck | kein Druck | kein Druck |
| Sprosse maßstäblich/schematisch | kein Druck | kein Druck | kein Druck |

#### Vermaßte Skizze drucken
Im Modul Dokumente können Sie die Funktion `Erweiterte Modellskizze` auswählen, um maßstäbliche Skizzen von Modellen und Sprossen auf ein separates Blatt zu drucken. Die Funktion muss in den Firmendaten aktiviert sein.

### Direktdruck
Für den Druck einzelner Dokumente können Sie Einstellungen für den Direktdruck festlegen. Im Direktdruck sind alle Einstellungen fixiert. Die Einstellungen legen Sie im Dialog `Auftragsformulare` fest.

### Druckaufträge
Wenn Sie mit einem zentralen Printserver arbeiten, können Sie Druckaufträge definieren. Zu einem Druckauftrag können ein oder mehrere Druckläufe definiert werden.

**Beispiele:**
- Drucken der Auftragsbestätigungen für interne Zwecke.
- Auftragsbestätigungen als Wiederholungsdruck per Fax senden.
- Auftragsbestätigungen als Wiederholungsdruck per E-Mail an den Vertreter senden.

Jeder Druckauftrag bezieht sich immer auf einen bestimmten Dokumententyp. Nach jedem Drucklauf wird der Status des Dokuments hochgesetzt. Die Reihenfolge der Druckläufe muss mit der Vergabe des Status übereinstimmen.

> **Druckername muss bekannt sein**
> Bei der Definition der Druckläufe muss der Drucker auf dem Server verfügbar sein. Dazu muss er auch auf dem Client eingerichtet sein.

### Direktdruck definieren

#### So definieren Sie einen Direktdruck
1.  Wählen Sie im Menü **Stammdaten > Formulare > Auftragsformulare**.
2.  Wählen Sie im Menü **Start > Neu**.
3.  Tragen Sie die Bezeichnung (A) ein (z. B. `Angebot (WH)`).
4.  Wählen Sie den Dokumententyp und den Druckpunkt (B) aus.
5.  Wählen Sie den Drucker (C) aus.
6.  Wählen Sie ggf. das Formular (D) für den Druckpunkt aus.
7.  Markieren Sie ggf. die Checkbox (E) `Rückfrage vor Druck`.
8.  Wählen Sie im Menü **Start > Speichern**.

### Druckauftrag anlegen

#### So legen Sie einen Druckauftrag an
1.  Wählen Sie im Menü **Stammdaten > Formulare > Druckaufträge**.
2.  Wählen Sie im Menü **Start > Neu**.
3.  Tragen Sie die Bezeichnung (A) ein.
4.  Wählen Sie den Dokumententyp (B) aus.
5.  Wählen Sie im Menü **Start > Speichern**.

#### So fügen Sie Druckläufe hinzu
1.  Wählen Sie den Druckauftrag aus, zu dem Sie einen Drucklauf hinzufügen wollen.
2.  Klicken Sie auf **[Hinzufügen]** (E).
3.  Wählen Sie das Formular (A) aus, z. B. `AB WH-Druck`.
4.  Wählen Sie den Drucker (B) aus.
5.  Wiederholen Sie die Schritte 2 bis 4, um weitere Druckläufe hinzuzufügen.
6.  Sortieren Sie die Druckläufe in der Übersicht mit Hilfe der Pfeilschaltflächen (C) in die Reihenfolge, die der Statusvergabe entspricht.
7.  Legen Sie ggf. die Details (B) zur Druckausgabe pro Formular fest.
8.  Wählen Sie im Menü **Start > Speichern**.

### Komplexübung
Die folgenden Aufgaben bauen auf den Lerneinheiten von Tutorial 1 und Tutorial 2 auf.
- Legen Sie einen neuen Kalender für das kommende Jahr an.
- Legen Sie zwei neue Preisschlüssel mit der Gültigkeit für 90 Tage an: einen für den Verkauf und einen für den Einkauf.
- Legen Sie ein Produkt VSG mit der Bearbeitung `Schleifen` an.
- Legen Sie ein Produkt ISO an, in dem eine Scheibe Ihr VSG ist.
- Legen Sie Preistabellen für die Berechnung von EK- und von VK-Preisen für die neuen Produkte an.
- Legen Sie einen Kunden mit folgenden Daten an: Tour, Zahlungsbedingungen, Lkw und Fahrer.
- Legen Sie für diesen Kunden ein Objekt an.
- Legen Sie in Ihrem Tarif eine neue Preistabelle für dieses Objekt an und weisen Sie diese dem Kunden zu.
- Erfassen Sie einen Auftrag mit Ihrem ISO. Der Auftrag muss sich auf das Objekt beziehen und automatisch den entsprechenden Preis anzeigen.
- Prüfen Sie den Status des Objekts in den Stammdaten.
- Legen Sie einen neuen Mitarbeiter an. Dieser soll das Recht haben, Aufträge zu erfassen und an die Produktion zu übergeben.

---

## Zusatzinformationen

In diesem Abschnitt finden Sie Ergänzungen zu Tutorial 1 und 2. Dies sind im Wesentlichen technische Informationen zu Berechnungen und Übersichten zu den fest definierten Vorgaben.
- "Objekt-/Abrechnungsverwaltung" auf Seite B-568
- "Verfügbare Dokumententypen" auf Seite B-593
- "Verfügbare Grenztypen" auf Seite B-594
- "Verfügbare Systemtexte" auf Seite B-598
- "Verfügbare Variablen (Platzhalter)" auf Seite B-599
- "Konstruktionstypen Bleiverglasung" auf Seite B-602
- "Änderungsüberwachung" auf Seite B-603
- "A+W Production" auf Seite B-606
- "Mischkalkulation" auf Seite B-609
- "Französische Preisberechnung" auf Seite B-610
- "Kalkulation" auf Seite B-611

### Objekt-/Abrechnungsverwaltung
Ein Objekt ist ein bestimmtes Bauvorhaben, an dem mehrere Kunden und Lieferanten beteiligt sein können. Zu einem Rahmenvertrag können mehrere Aufträge erstellt werden, bis die vereinbarten Flächen, Stückzahlen oder Summen ausgeschöpft sind.

#### Varianten der Objekt-/Abrechnungsverwaltung
- **Standard-Objektverwaltung:** Einem Marktpartner wird ein Objekt zugeordnet. Die Konditionen des Objekts werden für die Preisfindung herangezogen.
- **Erweiterte Objektverwaltung:** Zusätzlich können Vertreter und Zahlungsbedingungen hinterlegt werden.
- **Abrechnungsverwaltung mit zugeordneten Aufträgen:** Sie erfassen einen Rahmenauftrag, aus dem Sie Forderungsrechnungen erstellen.
- **Abrechnungsverwaltung:** Sie erfassen Forderungsrechnungen über geleistete Stunden und Zukauf von Bestellteilen.

#### Objektverwaltung einstellen
Für die Verwaltung von Objekten muss in den Firmendaten eine der folgenden Einstellungen gewählt sein:
- Standard Objektverwaltung
- Erweiterte Objektverwaltung
- Standard Objektverwaltung + Abrechnungsverwaltung mit zugeordneten Aufträgen

#### Standard-Objektverwaltung
Mit der Standard-Objektverwaltung erfassen Sie einen Auftrag und geben dabei das Objekt an, auf das sich der Auftrag bezieht. Sie legen ein Objekt an, ordnen es dem Kunden zu und definieren Preise/Rabatte.

#### Erweiterte Objektverwaltung
Hier können zusätzlich abweichende Vertreter und Zahlungsbedingungen festgelegt werden. Auch veranschlagte Mengen (Höchstmengen) für ein Produkt oder eine Warengruppe können hinterlegt werden.

#### Abrechnungsverwaltung mit zugeordneten Aufträgen
In diesem Modus können Sie einen Rahmenauftrag einem Objekt zuordnen. Von dem Rahmenauftrag aus erstellen Sie Forderungen (z.B. als Prozentsatz der Gesamtmenge). Für diese Forderungen werden keine Rechnungen erzeugt, sondern über einen speziellen Modus an die FiBu übergeben. Für die Produktion und Lieferung erzeugen Sie separate Produktionsaufträge.

> **Ablaufdiagramm (Abb. B-324)**
> 1.  **Rahmenauftrag** (Betrag, Menge, Prozent) führt zur Erstellung einer **Forderungsrechnung**.
> 2.  Die **Forderungsrechnung** wird an die **Spezielle FiBu-Übergabe** übergeben.
> 3.  Aus der **Abrechnungsverwaltung (Objekt)** werden **Produktionsaufträge** und **Bestellungen** generiert.
> 4.  Am Projektende wird eine **Gesamtrechnung** erstellt und an die **FiBu-Übergabe** übergeben.
> 5.  **Gutschriften** können ebenfalls erstellt werden.

#### Rahmenauftrag abrechnen

**So legen Sie einen Rahmenauftrag an:**
1.  Legen Sie in der Auftragserfassung einen Auftrag mit dem Dokumententyp `Rahmenauftrag` an.
2.  Erfassen Sie die Produkte ohne detaillierte Angaben.
3.  Speichern und schließen Sie den Auftrag.
4.  Wählen Sie **Dokumente > Objektabrechnungen > Abrechnungen**.
5.  Wählen Sie **Start > Neu**.
6.  Tragen Sie Abrechnungsnummer, Kundennummer und die Nummer des Rahmenauftrags ein.
7.  Speichern Sie das Abrechnungsobjekt.

**So erfassen Sie einen Auftrag zu einem Rahmenauftrag:**
1.  Legen Sie einen neuen Auftrag an.
2.  Wählen Sie den Dokumententyp `Produktionsauftrag`.
3.  Tragen Sie die Abrechnungsnummer ein.
4.  Speichern Sie und erfassen Sie die Positionen und Mengen, die gefertigt werden sollen.

**So erstellen Sie eine Forderungsrechnung:**
1.  Wählen Sie **Dokumente > Objektabrechnungen > Abrechnungen**.
2.  Wählen Sie im Menü **Funktionen > Forderungsrechnung erstellen**.
3.  Tragen Sie die Menge und Mengeneinheit ein, die berechnet werden soll.
4.  Klicken Sie auf [OK]. In der Dokumentenverwaltung wird ein Auftrag vom Typ `Forderung` angelegt.

**So schließen Sie einen Rahmenauftrag ab:**
1.  Lassen Sie sich in `Abrechnungen` das Objekt anzeigen. Wenn alle Mengen erfüllt sind, wird der Status auf `komplett` gesetzt.
2.  Im Register `Rahmenauftrag` prüfen Sie, ob alle berechneten Mengen auf 100% sind.
3.  Öffnen Sie in der Dokumentenverwaltung den Rahmenauftrag und schließen Sie ihn mit dem Rechnungsdruck und der Übergabe an die FiBu ab.

### Verfügbare Dokumententypen
| Typ | Beschreibung |
| :--- | :--- |
| **Anzahlung** | Wird automatisch bei einer Anzahlung gesetzt. |
| **Eigenfertigung** | Wird bei der Erfassung eines Produktionsauftrags gesetzt. |
| **Forderung** | Wird automatisch bei der Erstellung von Forderungsrechnungen gesetzt (Modul Objektabrechnungsverwaltung). |
| **Interne Verrechnung** | Wird automatisch bei der Bestellübergabe gesetzt (Modul Profit-Center-Verrechnung). |
| **Interner Auftrag** | Wird automatisch bei der Bestellübergabe gesetzt (Modul Interne Aufträge). |
| **Kundenmaterial** | Muss manuell gesetzt werden. Alle Positionen werden auf die Beschaffungsart "Kundeneigenes Glas" gesetzt. |
| **Lagerbestellung** | Wird bei der Lagerbestellung gesetzt, kann aber auch manuell in einem Bestellauftrag gesetzt werden. |
| **Reklamation** | Wird automatisch bei der Reklamationserfassung gesetzt, kann aber auch manuell im Auftrag gesetzt werden. |
| **Teillieferung** | Wird automatisch bei der Erstellung von Teillieferaufträgen gesetzt. |
| **Wertmäßige Buchung** | Wird automatisch während der Gutschriftenerfassung gesetzt. Mengenwerte werden nicht an die Statistik übergeben. |

### Verfügbare Grenztypen
Die Grenztypen sind fest hinterlegt und können nicht bearbeitet werden.
(Auszug)
| Grenztyp | Beschreibung | Beispiel |
| :--- | :--- | :--- |
| **Dicke (additiv nur Glas)** | Dicke aller Gläser der Stückliste. | Hauptposition VSG (4mm Float + Folie + 4mm Float) = Gesamtdicke 8mm |
| **Dicke (Stückliste)** | Auf Ebene der Hauptposition: Gesamtdicke. Auf Stücklistenebene: Dicke der Komponente. | Folie, Glas |
| **Einbauposition** | Glaspreis nach Einbauposition gestaffelt. | Bsp. ISO: 1:Float, 2:SZR, 3:ESG, 4:SZR, 5:Float |
| **Lfm Auftrag Produkt** | Gesamte Laufmeter eines Produkts innerhalb eines Auftrags. | Bis 10 lfm = 5 Euro/lfm, bis 99 lfm = 4 Euro/lfm |
| **Qm (Liefertag)** | Gesamtquadratmeter eines Kundenauftrags pro Liefertag. | Modul Anlieferpauschale |
| **Zuschlagsnettobasis** | Energiezuschlag in Prozent für Gläser. Basis ist die Summe der Nettopreise aller Gläser. | bis zu 1000,00 = 5% Zuschlag, ab 1000,00 = 2% Zuschlag |

### Verfügbare Systemtexte
(Auszug)
| Nr. | Text | Verwendung |
| :-: | :--- | :--- |
| 1 | Modell | |
| 2 | ;unten:;rechts:;oben:;links:; Scheibe;S | Vermaßung der Stufe |
| 50 | Rechnung <ar> v. <ard> f. Anzahlung v. <ad> | Anzahlungen |
| 100 | Abrechnungssumme original %X1 | Objektverwaltung DMS |
| 110 | Ug-Wert in W/qm | Techn. ISO-Parameter |
| 111 | Ug-Wert nach DIN 4108-4 | Techn. ISO-Parameter |
| 119 | Sprossen im SZR, einfach | Versicherungspreisliste |

### Verfügbare Variablen (Platzhalter)
In Texten können Variablen eingefügt werden, die erst im Dokument gefüllt werden.

**Formel:** `<@Formelnummer@>` = Ausführung einer Formel mit der Nummer (nn)

**Allgemein:**
| Bereich | Variable | Bedeutung |
| :--- | :--- | :--- |
| Allgemein | `%X1`, `%X2`, ... | Variablen, die durch A+W Business mit Werten gefüllt werden. |
| Anzahlung | `<aa>` | Anzahlungsauftragsnummer |
| CEKAL | `<fi>` | Firmennummer aus den Firmendaten |

**Bearbeitungen:**
| Variable | Bedeutung | Beispiel in Positionserfassung |
| :--- | :--- | :--- |
| `<%>` | Anzahl (Kanten, Bohrungen, ...) | `2` Kanten |
| `<$>` | Hauptparameter (Durchmesser, Radius, ...) | 20 mm |
| `<§>` | Ergänzungsparameter (welche Kanten, ...) | [2/3] |
| `<=>` | Berechnete lfm | 2,45 lfm |

**Rahmentexte:**
| Variable | Bedeutung |
| :--- | :--- |
| `<ab>` | Abstandhalterkurzbezeichnung |
| `<an>` | Auftragsnummer, ohne führende Null oder Leerzeichen |
| `<cn>` | Kundennummer |
| `<gt>` | Gütetext |
