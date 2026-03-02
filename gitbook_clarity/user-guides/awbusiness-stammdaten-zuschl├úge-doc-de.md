---
description: "D-AWBusiness-HB_5"
---


# Tutorial 1: Zuschläge

---
## Übungen

*   Legen Sie einen einfachen Zuschlag für Scheiben an, der erhoben wird, wenn das Gewicht 30 kg/lbs übersteigt.
*   Legen Sie einen Zuschlag an, bei dem die Kantenlänge und die Fläche berücksichtigt werden.
*   Legen Sie zu dem Zuschlag für die Kantenlängen mindestens zwei weitere Staffelungen an.
*   Löschen Sie eine der Staffelungen - ohne die gesamte Tabelle zu löschen.

### Ergänzende Informationen

*   ⇨Tutorial 2, "Verfügbare Grenztypen" auf Seite B-528
*   ⇨ Softwarereferenz, "Sonstige Zuschläge" auf Seite B-675

## Automatische Zuschläge

### Lernziele

*   Funktion der automatischen Zuschläge/Rabatte kennenlernen.
*   Automatische Zuschläge in den Stammdaten aktivieren.
*   Automatischen Zuschlag definieren.

### Nutzen

*   Mit den sogenannten automatischen Zuschlägen werden in der Regel Kosten abgedeckt, die z. B. durch den Transport, die Entsorgung oder ähnliche Situationen entstehen.
*   Diese Kosten werden als Zuschläge angelegt und im Dokument wie jedes Produkt als eigene Position eingefügt.

### Merke

*   **Automatischer Zuschläge**: Automatische Zuschläge werden in der Partnerverwaltung, der Produktverwaltung und im Auftrag im Bereich Zuschläge/Rabatte angezeigt.
*   **Produktzuordnung**: Sie können als Teuerungszuschläge oder als Sonderrabatte genutzt werden. Sie werden nur dann automatisch in die Dokumente eingefügt, wenn sie in den Stammdaten der Produkte und der Kunden aktiviert sind. Die Zuschläge oder Sonderrabatte werden wie Produkte behandelt und als eigene Position im Auftrag eingefügt.
*   **Zuschlag oder Rabatt**: Ein automatischer Zuschlag wird als Produkt mit einer eigenen Preistabelle (Einzelpreis) angelegt und einem der verfügbaren Zuschläge/Rabatte zugeordnet. Über den Wert im Einzelpreis wird entweder ein Zuschlag oder ein Rabatt berechnet.
*   **Anwendung**: Automatische Zuschläge werden von A+W Business als Auftragsposition eingefügt, wenn der Auftrag gespeichert wird.
*   **Berechnung im Dokument**: Der automatische Zuschlag bezieht sich jeweils auf eine einzelne Auftragsposition oder auf den gesamten Auftrag.
*   **Position im Dokument**: Die Nummer der Position im Dokument gibt an, an welcher Stelle der automatische Zuschlag eingefügt wird. Durch die Position im Dokument und durch die in der Produktdefinition gewählte Zuschlagsart kann ein Teuerungszuschlag/Sonderrabatt auf einen anderen Zuschlag wirken. So könnte sich z. B. ein Sonderrabatt auf den gesamten Auftrag einschließlich des automatischen Zuschlags für die Maut beziehen.

## Funktion der automatischen Zuschläge

Bei jedem Produkt und jedem Kunden können Sie einen oder mehrere automatische Zuschläge angeben, die immer berechnet werden. Diese automatischen Zuschläge können z. B. als Teuerungszuschläge für Transport-, Mautkosten, Energie genutzt werden oder als Sonderrabatte. Diese Zuschläge können allgemeingültig oder kundenspezifisch definiert werden.

Die Zuschläge oder Sonderrabatte werden wie Produkte behandelt und als eigene Position im Auftrag eingefügt.

Für die Definition der Zuschläge/Sonderrabatte gelten folgende Regeln:

*   Sie werden als Produkt angelegt.
*   Sie sind immer der Produktart und der Produktgruppe Leistungen/Zuschläge zugeordnet.
*   Sie haben grundsätzlich eine eigene Preistabelle.
*   Sie müssen im Dialog Produktzuordnung Zuschläge den Zuschlägen/Sonderrabatten zugeordnet werden.

Die Zuschläge/Sonderrabatte können mehrfach zugeordnet werden, entweder, indem sie allgemeingültig sind oder nur für spezielle Kunden.

Für eigene Definitionen stehen Ihnen zehn so genannte Sonderrabatte zur Verfügung, die Sie mit einem positiven Wert als Zuschlag, mit einem negativen Wert als Rabatt einsetzen können. Damit können Sie z. B. zeitlich begrenzte Sonderaktionen gestalten, in dem Sie eine Gültigkeitsdauer angegeben.

*Abbildung B-201: Produktzuordnung der Zuschläge/Sonderrabatte*
*(Das Diagramm zeigt, wie ein Produkt (z.B. Energie) mit einer Preistabelle (z.B. für Energiezuschlag) und einer Produktart/Produktgruppe (Leistungen/Zuschläge) verknüpft ist. Diese Produktdefinition wird dann in der "Produktzuordnung Zuschläge" (z.B. Energiezuschlag) entweder allgemein oder für einen spezifischen Kunden gültig gemacht. Die Aktivierung erfolgt in der Partnerverwaltung oder der Produktverwaltung.)*

Diese Zuschläge werden in den Stammdaten der Produkte oder der Partner aktiviert. Die aktivierten Zuschläge/Rabatte werden automatisch als Position im Dokument eingefügt, sobald der Dialog zur Positionserfassung geschlossen wird. Im Auftrag können Sie den automatischen Zuschlag/Rabatt deaktivieren oder einen anderen aktivieren.

*Abbildung B-202: Automatische Zuschläge*
*(Die Abbildungen zeigen zwei Auswahllisten für automatische Zuschläge. A - Produktstammdaten: Eine kürzere Liste mit produktspezifischen Zuschlägen wie Energiezuschlag, Schwerlastabgabe, Gestellzuschlag. B - Partnerstammdaten: Eine längere, allgemeine Liste mit Zuschlägen wie Struktur innen, Randentschichtung, Max. Fläche, Eilzuschlag, Recycling, etc.)*

Die Auswahl der Zuschläge/Sonderrabatte ist in der Produktverwaltung (A) reduziert. In der Partnerverwaltung (B) stehen alle zur Verfügung, die allgemeingültig sind. Zusätzlich werden beim jeweiligen Kunden auch die kundenspezifischen angezeigt.

### Produktzuordnung Zuschläge

Die automatischen Zuschläge definieren Sie im Dialog Produktzuordnung Zuschläge.

*Abbildung B-203: Produktzuordnung Zuschläge*
*(Die Abbildung zeigt eine Tabelle zur Zuschlagszuordnung mit den Spalten Mandant, Kunde, Zuschlag, Produkt, Gültig von, Gültig bis und Position im Dokument. A markiert die Spalte "Bezeichnung des Zuschlags". B markiert die Spalte "Nummer und Name des zugeordneten Produkts". C markiert die Spalte "Position, an der der Zuschlag im Dokument eingefügt wird".)*

In diesem Beispiel sehen Sie einige automatische Zuschläge, die allgemeingültig sind. Jedem dieser Zuschläge liegt ein eigenes Produkt (B) zugrunde, z. B. das Produkt Struktur innen oder Randentschichtung.

Das Datum 31.12.2099 zeigt an, dass dieser Zuschlag unbefristet gültig ist. Zeitlich begrenzt gültige Zuschläge haben ein Enddatum, das in der Spalte Gültig bis angezeigt wird. Nach dem Datum werden sie nicht mehr eingefügt und nicht zur Auswahl angeboten.

Durch die Festlegung der Positionsnummer (C) kann bestimmt werden, an welcher Stelle im Dokument der Zuschlag/Rabatt eingefügt werden soll. Diese Position bestimmt u. a. die Berechnung des Zuschlags/Rabatts. Die Ziffer 0 bedeutet, dass dieser Zuschlag auf eine Position im Auftrag bezogen werden soll. Der Zuschlag muss daher in der Produktverwaltung aktiviert werden.

> **Beispiel**
> Wenn ein Zuschlag/Rabatt mit der Positionsnummer 900 definiert ist, wird er am Ende des Dokuments aufgeführt. Ein Zuschlag/Rabatt mit der Positionsnummer 901 wird als darauf folgende Position eingefügt werden.
> Wenn generell ein Energiezuschlag berechnet werden soll, wird er in der Produktdefinition aktiviert. Als Zuschlag hat er eine Positionsnummer über 900, z. B. 970 und wird damit beim Speichern an letzter Position im Auftrag eingefügt.

Durch die Position im Dokument und durch die in der Produktdefinition gewählte Zuschlagsart kann ein Zuschlag/Rabatt auf einen anderen Zuschlag/Rabatt wirken. So könnte sich z. B. ein Sonderrabatt auf den gesamten Auftrag einschließlich des automatischen Zuschlags für die Maut beziehen.
⇨ "Zuschlagsarten" auf Seite B-317

### Verfügbare Teuerungszuschläge/Sonderrabatte

Folgende Zuschläge/Rabatte sind hinterlegt und können bearbeitet werden:

| Zuschlag/Rabatt | Beschreibung |
| :--- | :--- |
| **Anlieferpauschale** | Dieser Zuschlag wird für die Anlieferung berechnet. Er kann in der Partnerverwaltung aktiviert werden. |
| **Anzahlung** | Die Anzahlung wird als Anzahlungsrechnung erfasst und von der Auftragssumme abgezogen. Weitere Informationen dazu finden Sie im Part Verkauf.<br>⇨ Verkauf, "Anzahlungen" auf Seite C-280 |
| **Eilzuschlag** | Dieser Zuschlag wird berechnet, wenn der Auftrag innerhalb eines kürzeren Zeitraums geliefert werden muss. Er kann in der Partnerverwaltung aktiviert werden. |
| **Energiezuschlag** | Der Energiezuschlag wird auf das Gewicht der Lieferung bezogen. Er kann in der Produkt- und in der Partnerverwaltung aktiviert werden. Über die Firmendaten kann die Berechnung auf das Glasgewicht eingeschränkt werden.<br>⇨ Softwarereferenz, "Firmendaten - Preisberechnung" auf Seite B-959 |
| **Gestell 1, Gestell 2** | Die Gestellzuschläge werden im Rahmen der Gestellverwaltung berechnet. Sie können in der Produkt- und in der Partnerverwaltung aktiviert werden.<br>⇨ Softwarereferenz, "Firmendaten - Versand" auf Seite B-1008 |
| **Max. Fläche, Max. Seitenverhältnis** | Diese Zuschläge werden für die Überschreitung der maximalen Fläche und/oder des maximalen Seitenverhältnisses berechnet. Sie können in der Partnerverwaltung aktiviert werden. Zur Überprüfung der Werte werden die Maßangaben aus der Produktverwaltung herangezogen.<br>⇨ Softwarereferenz, "Preis-Parameter" auf Seite B-612 |
| **Mindermengen** | Dieser Zuschlag bezieht sich auf die in der Produktverwaltung angegebenen Mindestmenge. Er kann in der Partnerverwaltung aktiviert werden.<br>⇨ Softwarereferenz, "Preis-Parameter" auf Seite B-612 |
| **Randentschichtung** | Dieser Zuschlag wird für die Randentschichtung beschichteter Gläser berechnet. Er bezieht sich immer auf eine Position. Er kann in der Partnerverwaltung aktiviert werden. |
| **Rechnungsstellung** | Dieser Zuschlag wird erhoben, wenn die Rechnung ausgestellt wird. Er kann in der Partnerverwaltung aktiviert werden. |
| **Recycling ISO** | Dieser Zuschlag wird für die Entsorgung von ISO-Gläsern erhoben. Er kann in der Partnerverwaltung aktiviert werden. |
| **Sonderrabatt 1 – 10** | Die Sonderrabatte stehen für individuelle Definitionen zur Verfügung. Sie werden mit positiven Werten als Zuschlag oder mit negativen Werten als Rabatt definiert. Sie können in der Produkt- und in der Partnerverwaltung aktiviert werden. |
| **Struktur innen** | Dieser Zuschlag wird für den Einbau einer Ornamentscheibe berechnet, die mit der Strukturseite nach innen eingebaut wird, wenn diese Seite standardmäßig außen liegt. Er kann in der Partnerverwaltung aktiviert werden. |
| **Transport ISO** | Dieser Zuschlag wird für die Transportversicherung von ISO-Scheiben berechnet. Er kann in der Partnerverwaltung aktiviert werden. |

*Tab. B-15 Übersicht über die automatischen Zuschläge*

Alle weiteren Zuschläge, die nicht über die Stammdaten der Produkte und Partner automatisch eingefügt werden, müssen im Dokument manuell erfasst werden.

## Automatischen Zuschlag definieren

Einen automatischen Zuschlag legen Sie in dieser Reihenfolge an:

1.  **In der Produktverwaltung erfassen Sie ein Produkt (Zuschlagsprodukt):**
    *   Im Register **Produkt** wählen Sie als Produktart und Produktgruppe den Eintrag **Leistungen/Zuschläge** aus.
    *   Im Register **Fertigung** geben Sie die Mengeneinheit an und ob der Zuschlag/Rabatt in der Stückliste gedruckt werden soll.
    *   Im Register **Preis/Zuschlag** geben Sie die entsprechende **Zuschlagsart** an, z. B. Basisposition.
    Diese Schritte sind in der Einheit Produkt ausführlich beschrieben.
    ⇨ "Produkt anlegen" auf Seite B-184
2.  **In der Preisverwaltung erfassen Sie einen Einzelpreis für dieses Produkt.**
    Wenn Sie einen negativen Wert eintragen, führt der automatische Zuschlag zu einer Reduktion des Preises. Er wirkt als Rabatt.
    ⇨ "Einzelpreise anlegen" auf Seite B-239
3.  **Im Dialog Produktzuordnung Zuschläge weisen Sie das Produkt dem gewünschten automatischen Zuschlag zu.**
4.  **In den Kundenstammdaten aktivieren Sie im Register Auftrag im Bereich Zuschläge/Rabatte anwenden die Checkbox für die Zuschläge, die immer für den Kunden berechnet werden sollen.**
    ⇨ Softwarereferenz, “Zuschläge/Rabatte" auf Seite B-779
5.  **In den Produktstammdaten aktivieren Sie im Register Preis/Zuschlag im Bereich Zuschläge/Rabatte anwenden die Checkbox für die Zuschläge, die immer für das Produkt berechnet werden sollen.**
    ⇨ Softwarereferenz, "Zuschläge/Rabatte anwenden" auf Seite B-611

In der nachfolgenden Handlungsanleitung wird ein Sonderrabatt für einen Kunden eingerichtet. Dazu sind das Produkt Sonderrabatt Schulung und die zugehörige Preistabelle angelegt.

> **i Automatische Zuschläge als Rabatte nutzen**
> Sie können die automatischen Zuschläge als (Sonder-)Rabatte nutzen, indem Sie einen negativen Betrag eingeben. Daher wird in der folgenden Beschreibung immer von Zuschlag/Rabatt gesprochen.

### So definieren Sie einen automatischen Zuschlag für einen Kunden

1.  Wählen Sie im Menü **Stammdaten > Firma > Produktzuordnung Zuschläge**.
    Der Dialog **Produktzuordnung Zuschläge** wird geöffnet.
    ⇨ Softwarereferenz, "Produktzuordnung Zuschläge" auf Seite B-1043
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    *Abbildung B-204: Felder für automatischen Zuschlag freigeschaltet*
    *(Die Abbildung zeigt den Dialog "Produktzuordnung Zuschläge" im Erfassungsmodus. Die Felder Kunde (A), Auswahl des Zuschlags (B), Produkt für den Zuschlag (C) und Position (D) sind aktiv.)*
    Die Felder sind mit den Daten des Zuschlags vorbelegt, der in der Übersicht markiert ist.
3.  Wählen Sie die Option **Kunde** (A) und den Kunden, für den Sie diesen Zuschlag/Rabatt anlegen wollen.
4.  Wählen Sie den automatischen Zuschlag/Rabatt (B) aus, den Sie definieren wollen, z. B. den Eintrag **Sonderrabatt 3**.
5.  Wählen Sie das Produkt (C) aus, das Sie dem Zuschlag zuordnen wollen, z. B. das Produkt **Sonderrabatt Schulung**.
    Dem Produkt **Sonderrabatt Schulung** ist bereits ein Preis (prozentualer Aufschlag) zugeordnet.
6.  Wählen Sie im Feld **Gültig bis** einen langen Zeitraum, z. B. 2099, wenn der Zuschlag/Rabatt immer berechnet werden soll.
    In diesem Beispiel wird die Gültigkeit auf den 31.12. des aktuellen Jahres begrenzt.
7.  Tragen Sie die **Position im Dokument** (D) ein:
    *   **0** für einen positionsbezogenen Zuschlag/Rabatt, z. B. bei einem Zuschlag für die Überschreitung der maximalen Fläche. Er wird bei jeder Position eingefügt, auf die er zutrifft.
    *   **900 - 999** für Zuschläge/Rabatte, die auf alle vorherigen oder Teile der vorherigen Positionen wirken sollen.
    *Abbildung B-205: Kundenbezogener Sonderrabatt*
    *(Die Abbildung zeigt einen eingerichteten Sonderrabatt für einen bestimmten Kunden, dem das Produkt "Sonderrabatt-Schulung" zugeordnet ist. Die Positionsnummer ist auf 999 gesetzt.)*
    In diesem Beispiel wird die Positionsnummer 999 eingetragen. Damit wird der Sonderrabatt am Ende der Auftragspositionen eingetragen und für die Gesamtsumme berechnet.
8.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.
    Damit der Zuschlag/Rabatt berechnet wird, müssen Sie ihn in den Stammdaten des Kunden aktivieren. Wenn es zusätzlich einen allgemeinen Sonderrabatt gibt, dann wird für den Kunden nur der kundenbezogene Sonderrabatt berechnet.

### Übungen

*   Legen Sie für Ihren Schulungskunden einen Sonderrabatt von 3 % an, der automatisch als letzte Position im Auftrag eingefügt wird.
*   Beachten Sie dabei die Reihenfolge, in der Sie Produkt, Preis und Zuordnung festlegen müssen.
*   Sie werden in einer späteren Übung prüfen, ob der Sonderrabatt so eingesetzt wird, wie Sie es beabsichtigt haben.

#### Ergänzende Informationen

*   ⇨ "Finanzdaten des Kunden bearbeiten" auf Seite B-102
*   ⇨ "Produkt anlegen" auf Seite B-184
*   ⇨ "Einzelpreise anlegen" auf Seite B-239
*   ⇨ Softwarereferenz, "Produktverwaltung" auf Seite B-598
*   ⇨ Softwarereferenz, "Preisverwaltung" auf Seite B-723
*   ⇨ Softwarereferenz, “Partnerverwaltung" auf Seite B-770
*   ⇨ Softwarereferenz, "Produktzuordnung Zuschläge" auf Seite B-1043

## Komplexübung

In dieser Übung wird die Erfassung der Preise zu einem Produkt ausführlich an einem Beispiel vorgeführt.

### Aufgabenstellung

Zu Beginn ein Beispiel für die Preise eines Produktes, wie sie in Standard-Preislisten vorkommen können:

**Preise/qm x mm VSG-Scheibe**

| Fläche qm | 4 mm | 5 mm | 5 mm (>1600x3000) | 6 mm | 6 mm (>1600x3000) |
| :--- | :--- | :--- | :--- | :--- | :--- |
| | bis max. 1410 x 2400 mm | bis 1600 x 3000 mm | bis 2450 x 3000 mm | bis 1600 x 3000 mm | bis 2550 x 4500 mm |
| **> 0,50 qm** | 196,00 € | 202,00 € | 276,00 € | 208,00 € | 282,00 € |
| **A1: 0,16-0,50 qm** | 253,00 € | 263,00 € | | 271,00 € | |
| **A1: 0,10-0,15 qm** | 311,00 € | 323,00 € | | 333,00 € | |
| **> 0,50 qm** | 215,00 € | 224,00 € | 299,00 € | 230,00 € | 305,00 € |
| **A2: 0,16-0,50 qm** | 281,00 € | 291,00 € | | 299,00 € | |
| **A2: 0,10-0,15 qm** | 345,00 € | 358,00 € | | 368,00 € | |

*Tab. B-16: Preise eines Produktes*

Zusätzlich können z. B. folgende Berechnungsfaktoren gelten:

*   Ist die Kante länger als 3750 mm, soll ein Zuschlag von 30 % berechnet werden.
*   Die Mindestproduktionsmaße sind 200 x 300 mm.
*   Die Mindestberechnungslänge ist 300 mm pro Kante.

Für die Beispiele aus der Tabelle muss zunächst die Anzahl der Grenztypen (Größen) festgelegt werden, die berücksichtigt werden sollen:

*   **Die Flächenbegrenzung** (0,10 – 0,15 qm; 0,16 – 0,50 qm; über 0,50 qm).
*   **Die Breite**:
    *   Für VSG 5 mm gelten zwei Maßbegrenzungen (0 < B1 < 1600 mm und 1600 < B2 < 2450 mm) und für VSG 6 mm eine (2550 < B2 < 4500 mm).
*   **Die Höhe**:
    *   Für VSG 6 mm gelten zwei Maßbegrenzungen: unter und über 3000 mm.

Dies sind insgesamt vier Grenztypen. Durch den Würfel können höchstens drei von ihnen berücksichtigt werden. Die vierte Größe kann über einen Zuschlag abgedeckt werden.

Pro ISO-Einheit A1, A2 und VSG-Scheibendicke werden sechs ISO-Produkte erfasst.

*   **A1:**
    *   ISO A1 mit VSG 4 mm
    *   ISO A1 mit VSG 5 mm
    *   ISO A1 mit VSG 6 mm
*   **A2:**
    *   ISO A2 mit VSG 4 mm
    *   ISO A2 mit VSG 5 mm
    *   ISO A2 mit VSG 6 mm

Für jedes der sechs ISO-Produkte wird eine Preistabelle angelegt (= drei Preistabellen pro ISO-Einheit):

*   Für die ISO-Produkte mit der VSG-Scheibe 4 mm Vektor-Preistabellen mit einem Grenztypen: die Fläche.
*   Für die ISO-Produkte mit VSG 5 und 6 mm Würfel-Preistabellen mit drei Grenztypen: Fläche, Breite und Höhe.

Die vierte Größe wird als Zuschlag für Kantenüberlängen ab 3750 mm einbezogen.

## Lösung: Produkt und seinen Preis erfassen

Das Beispielprodukt ist eine Isolierglas-Einheit. Dabei kann ausführlich gezeigt werden, wie Sie vorgehen sollten. Gleichzeitig wird der Würfel (dreidimensionale Preisberechnung) dargestellt. Dies gibt Ihnen den besten Überblick darüber, wie die Preisberechnung funktioniert.

Zu diesem Thema gibt es folgende Handlungsanleitungen:

*   "So legen Sie den Preis als Würfel an" auf Seite B-342
*   "So erfassen Sie den Sonstigen Zuschlag" auf Seite B-346
*   "So erfassen Sie das ISO-Produkt" auf Seite B-347

### Preistabellen mit drei Grenzwerten

Zunächst prüfen Sie, welche Preisliste und welcher Preisschlüssel (Tarif) als Standard für den Verkaufspreis der Isolierglas-Einheit herangezogen wird.

#### ■ So legen Sie den Preis als Würfel an

1.  Wählen Sie im Menü **Stammdaten > Produkte > Preise > Preisjahrgang**.
    Der Dialog **Jahrgang** wird geöffnet.
    Anhand der Checkboxen können Sie erkennen, welche Preislisten standardmäßig für die Berechnung des ISO-Verkaufspreises herangezogen werden.
    *Abbildung B-206: Jahrgang*
    In diesem Beispiel ist die Spalte **Stn. ISO VK** wichtig. Die Preisliste, die für den VK ISO benutzt wird, ist in diesem Fall **EURO-Preis 97**.
2.  Schließen Sie den Dialog und wählen im Menü **Stammdaten > Preise > Tarife**.
    *Abbildung B-207: Tarif: Preisjahrgang + Schlüssel*
    Sie sehen, dass einer Preisliste mehrere Preisschlüssel zugeordnet sein können. Daher gibt es mehrere Möglichkeiten für die Kombination von Preisliste/Schlüssel, die zur Preisberechnung von ISO herangezogen werden. In diesem Fall **EURO-Preis 97** und **Hütte VEGLA 97**. Damit wird deutlich, wo die neue Preistabelle abgelegt werden muss, damit der Preis automatisch herangezogen wird.
3.  Wählen Sie **Stammdaten > Produkte > Artikel > Artikel**.
    Prüfen Sie im Dialog **Produktverwaltung**, in welchem Nummernbereich Ihrer ISO-Produkte angelegt sind. Da Sie für die Preistabelle und für das Produkt dieselbe Nummer eintragen sollten, notieren Sie sich, welche Nummer noch frei ist.
4.  Wählen Sie im Menü **Stammdaten > Preise > Preise**.
    Der Dialog **Preise** wird geöffnet.
5.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    *Abbildung B-208: Preis anlegen*
6.  Tragen Sie die Nummer für die Preistabelle ein und wählen Sie den Preisjahrgang und den Preisschlüssel aus.
7.  Wechseln Sie zum Register **Würfel**.
    Die Lösung der Aufgabenstellung sieht nun wie folgt aus:
    *   **Die Breite = Grenztyp 1:**
        *   Für VSG 5 mm 2 Maßbegrenzungen: 0 < W1 < 1600 mm und 1600 < W2 < 2450 mm und
        *   Für VSG 6 mm: 2550 < W2 < 4500 mm
    *   **Die Höhe = Grenztyp 2:**
        *   Für VSG 6 mm in zwei Flächen zerlegt: unter und über 3000 mm)
    *   **Die Flächenbegrenzung = Grenztyp 3:**
        *   (0,10-0,15 qm; 0,16 – 0,50 qm; über 0,50 qm)
    *Abbildung B-209: Preis anlegen*
    Für die dritte Dimension des Würfels wird für jede Maßgrenze des Grenz-typs 3 ein Register angelegt. Wenn Sie die Preise für 0,15 - 0,50 qm sehen möchten, dann müssen Sie zum entsprechenden Register wechseln. Das Register 0,15 enthält die Preise von 0 – 0,15 qm. Das Register 9999,99 gilt bei einer Fläche zwischen 0,50 und 9999,99 qm (die Werte verstehen sich immer inklusive).
8.  Geben Sie die Preise in allen Registern ein.
    Als zusätzlicher Berechnungsfaktor soll gelten, dass die Mindestberechnungsgröße 300 x 300 mm ist. Sie sehen, dass für die Breite und die Höhe der Wert 300 mm, als kleinster Grenzwert angegeben ist, obwohl für die Produktion die Mindestproduktionsmaße 200 x 300 mm gelten. Bei der Preisfindung werden nur die Grenzmaße für die Berechnung und nicht die Grenzmaße für die Produktion berücksichtigt.
9.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.

### Sonstiger Zuschlag

Wenn eine Kante länger als 3750 mm ist, soll ein Zuschlag von 30 % berechnet werden.

#### ■ So erfassen Sie den Sonstigen Zuschlag

1.  Wählen Sie im Menü **Stammdaten > Produkte > Preise > Sonstige Zuschläge**.
    *Abbildung B-210: Sonstiger Zuschlag*
    Kantenzuschläge werden unter **Sonstige Zuschläge** eingetragen. Im Beispiel finden Sie den Kantenzuschlag in der Zuschlagstabelle 10.
    Die erste Zeile definiert, dass zwischen 0 und 2400 mm kein Zuschlag (0 %) berechnet wird. Die zweite Zeile definiert, dass zwischen 2400,01 und 3000 mm ein Zuschlag von 35,00 % berechnet wird, ab 3000,01 mm 45 %.
    Damit ist jede Sonderregelung berücksichtigt.
    Die Tabellennummer 10 für **Sonstige Zuschläge** kann an zwei Stellen eingetragen werden:
    *   **Produkt:**
        Wird die Tabellennummer im Produkt selbst im Register **Preis/Zuschlag** eingetragen, dann wird der Kantenzuschlag immer berechnet, auch wenn eine andere Preistabelle zur Berechnung herangezogen wird, z. B. bei einer Bestellung.
    *   **Preistabelle:**
        Soll der Kantenzuschlag nicht generell berechnet werden, dann tragen Sie die Tabellennummer nur in die betreffende Preistabelle ein. Dies ist dann sinnvoll, wenn Sie z. B. ein Spezialangebot erstellen oder wenn für manche Kunden dieser Zuschlag nicht berechnet werden soll.
2.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.

Wenn alle preisrelevanten Daten einer ISO-Einheit abgeschlossen sind, kann die ISO-Einheit als Produkt angelegt werden.

### Produkt anlegen

Im diesem Beispiel wird das ISO-Produkt 151000 gezeigt, das schon angelegt ist. Sie können daran besser erkennen, was Sie machen müssen, um ein vergleichbares Produkt zu erfassen.

#### ■ So erfassen Sie das ISO-Produkt

1.  Wählen Sie im Menü **Stammdaten > Produkte > Artikel > Artikel**.
    Der Dialog **Produktverwaltung** wird geöffnet.
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    *Abbildung B-211: Produktverwaltung Isolierglas*
3.  Tragen Sie die Produktnummer und eine Bezeichnung ein.
4.  Wechseln Sie zum Register **Preis/Zuschlag** und geben Sie unter anderem die Nummern der Preistabellen und im Feld **Sonstiger Zuschlag** die Tabelle für den Kantenlängen-Zuschlag ein.
5.  Geben Sie das Steuerkennzeichen für das Produkt an.
6.  Wechseln Sie zum Register **Stückliste**, um die Zusammensetzung der ISO-Einheit zu erfassen.
    *Abbildung B-212: Produktverwaltung Isolierglas Stückliste*
7.  Markieren Sie die Komponente, nach der Sie eine neue Komponente hinzufügen möchten.
8.  Öffnen Sie das Kontextmenü und wählen Sie den entsprechen Eintrag:
    *   **Komponente einfügen (vorher/danach):**
        Damit fügen Sie eine Komponente auf der gleichen Ebene ein, z. B. ein Float an das Hauptprodukt.
    *   **Komponente anhängen:**
        Damit hängen Sie eine Komponente auf der unteren Ebene an, z. B. einen Rahmen an ein Glas.
    Auf die gleiche Weise können Sie weitere Komponenten einfügen.
9.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert. Das Produkt ist angelegt. Andere Programmteile können jetzt darauf zugreifen und den entsprechenden Preis anzeigen und berechnen, z. B. in der Auftragserfassung.

# Rabatte

Mit den Rabatten haben Sie eine weitere Möglichkeit, die Preis für jeden einzelnen Kunden anzupassen, ohne die Preislisten zu ändern.

In diesem Themenblock lernen Sie die Rabatte und ihre Funktionsweise kennen.

Dazu gehören folgende Lerneinheiten:

*   "Rabatthierarchie" auf Seite B-342
*   "Rabattdefinition" auf Seite B-346

## Rabatthierarchie

### Lernziele

*   Funktionsweise der Rabatte kennenlernen.
*   Rabatten staffeln.
*   Kundenrabatt anlegen.

### Nutzen

*   Rabatte reduzieren den Listenpreis von Produkten bei der Berechnung von Positionen in einem Dokument und sind daher ein wichtiges Instrument der Preisgestaltung.
*   Durch die feingliedrigen Zuweisungsmöglichkeiten von Rabatten kann die Preisberechnung sehr kundenspezifisch gesteuert werden.

### Merke

*   **Rabattverwaltung**: Rabatte können auf der Ebene von Kunden- oder Lieferantengruppen vergeben werden oder für einen einzelnen Kunden oder Lieferanten. Die Logik der Rabattverwaltungen ist für Kunden und Lieferanten identisch.
*   **Rabattwert**: Rabatte können mit einem Grenztyp gestaffelt werden. Der angegebene Wert wird immer als prozentualer Wert interpretiert.
*   **Rabatte im Tarifsystem**: Rabatte beziehen sich immer auf einen Preisjahrgang, einen Preisschlüssel und ein Produkt oder eine Warengruppe.
*   **Rabattkennzeichen**: Rabatte werden nur berücksichtigt, wenn das Kennzeichen in den Produktstammdaten gesetzt ist.
*   **Manueller Rabatt**: Rabatte können im Auftrag manuell eingetragen werden. Manuelle Rabatte überschreiben die für den Kunden definierten Rabatte.
*   **Rabatthierarchie**: Bei der Preisberechnung im Dokument werden zuerst die Angaben aus der Position geprüft. Die Suche nach einem Rabatt wird eingestellt, wenn in der Position oder in den Partner-Rabatten gültige Vereinbarungen gefunden wurden.

## Funktionsweise der Rabatte

Rabatte reduzieren den Listenpreis von Produkten bei der Berechnung von Positionen in einem Dokument. Rabatte werden für einzelne Kunden oder für Kundengruppen angelegt und beziehen sich auf ein Produkt oder eine Warengruppe.

Der Rabatt wird im Auftrag automatisch herangezogen, wenn das Produkt erfasst wird. Wenn kein Rabatt vorgesehen ist, kann im Auftrag ein Prozentsatz eingetragen werden. Dieser manuelle Rabatt kann entweder im Auftragskopf für den gesamten Auftrag oder in der Positionserfassung für eine Position oder eine Stücklisten-Komponente eingetragen werden.

Sie können unterschiedliche Rabatte anlegen:

*   Standardrabatte für einen Preisjahrgang und Preisschlüssel (Tarif)
*   Staffelrabatte mit einer Grenzmenge
*   Austauschrabatte

*Abbildung B-213: Rabatte für Kunde und für Kundengruppe*
*(Die Abbildung zeigt zwei Rabatt-Listen. Die Einträge sind farblich markiert: Blau für Warengruppen, Rot für Produkte, Grün für Warengruppe und Objekt.)*

In diesem Beispiel sehen Sie die Rabatte eines Kunden. Die Schriftfarben der Einträge haben folgende Bedeutung:

*   **Blau**: Warengruppen
*   **Rot**: Produkt
*   **Grün**: Warengruppe und Objekt

Da Rabatte nur berechnet werden, wenn das Produkt oder die jeweilige Stücklisten-Komponente als rabattfähig gekennzeichnet ist, können Sie Rabatte sehr feingliedrig den einzelnen Komponenten der Stückliste oder ganzen Produkten zuweisen.

*Abbildung B-214: Produktverwaltung – Preis/Zuschlag*
*(Die Abbildung zeigt Checkboxen: Preisrelevant VK, Preisrelevant EK, Rabattfähig, Skontofähig)*

*Abbildung B-215: Möglichkeiten der Rabattvergabe*

| Stammdaten | Rabattfähig | Kunde A | Kunde B | Kunde C |
| :--- | :--- | :--- | :--- | :--- |
| Produkt ISO 15000 | ✔ | Rabatt auf: WGR Float, WGR Safe | Rabatt auf: WGR ISO | Rabatt auf: WGR Float, WGR SZR, WGR ISO |
| Float 4 mm | ✔ | | | |
| SZR | ✔ | | | |
| ESG Safe | ✔ | | | |
| **Auftrag** | **Berechnung** | **Preis ISO**<br>- Rabatt Float<br>- Rabatt Safe | **Preis ISO**<br>- Rabatt ISO | **Preis ISO**<br>- Rabatt ISO<br>- Rabatt Float<br>- Rabatt SZR |

In diesen Beispielen sehen Sie ein Produkt ISO, das aus einem Float, dem SZR und einem ESG aufgebaut ist. Dabei sind alle Produkte rabattfähig. Ob der Rabatt im Auftrag gewährt wird, hängt aber von den Rabattvereinbarungen ab, die mit jedem einzelnen Kunden getroffen wurde.

*   Kunde A erhält Rabatte auf das Float und das ESG.
*   Kunde B erhält einen Rabatt auf das ISO.
*   Kunde C erhält Rabatte auf das ISO, das Float und den SZR.

Sie sehen auch, dass die Rabatte sich summieren, d. h., dass sowohl für das ISO ein Rabatt berechnet wird, also auch für die Komponenten der Stückliste.

In diesem Beispiel sind Rabatte auf ganze Warengruppen (WGR) aufgeführt. Rabattvereinbarungen können sich auch auf einzelne Produkte beziehen.

> **i Sonderrabatt**
> Über die automatischen Zuschläge können Sie übergreifende (allgemeingültige) Rabatte anlegen, z. B. für Sonderaktionen. Diese Sonderrabatte werden niemals in der Rabattübersicht angezeigt.
> Sonderrabatten dürfen Sie nicht mit den Partner-Rabatte verwechseln, die in dieser Einheit beschrieben werden.
> ⇨ "Automatische Zuschläge" auf Seite B-332

## Rabattsuche

Für alle Berechnungen in den Aufträgen gilt die Hierarchie:

*   Angaben im Auftrag (oberste Priorität)
*   Vereinbarungen aus den Partner-Rabatten

In dieser Reihenfolge wird der nächste Schritt nur dann ausgeführt, wenn bei der Suche keine Angaben gefunden wurden. In der Preisberechnung gilt dann für die Rabatte folgende Hierarchie:

1.  Produkt - Kunde
2.  Produkt - Kundengruppe
3.  WGR (Warengruppe) - Kunde
4.  WGR - Kundengruppe
5.  WOG (Waren-Obergruppe) - Kunde
6.  WOG - Kundengruppe
7.  WHG (Waren-Hauptgruppe) - Kunde
8.  WHG - Kundengruppe

*Abbildung B-216: Hierarchie der Preisfindung*

Die Berechnung der Preise im Dokument wird zusätzlich auch von den Einstellungen gesteuert, die in den Firmendaten systemweit festgelegt sind. Die Beschreibung der einzelnen Einstellungen finden Sie in der Softwarereferenz.
⇨ Softwarereferenz, "Firmendaten - Preisberechnung" auf Seite B-959

## Rabattdefinition

### Lernziele

*   Standard-, Austausch- und Staffelrabatte kennenlernen.
*   Rabatt anlegen.
*   Rabattumleitung festlegen.

### Nutzen

*   Rabatte sind ein Mittel der Preisberechnung, mit dem die Preise von Aufträgen sehr fein auf Kunden oder Kundengruppen abgestimmt werden können.
*   Anhand von Lieferantenrabatten können die EK-Preise so genau kalkuliert werden, dass die Deckungssummen, z. B. in günstigen Angeboten, nicht unterschritten werden.

### Merke

*   **Kundenrabatt**: Kundenrabatte werden bei der Preisermittlung von Aufträgen ausgewertet.
*   **Lieferantenrabatt**: Lieferantenrabatte werden bei der Ermittlung der Einkaufspreise ausgewertet.
*   **Standard-Rabatt**: Für eine Warengruppe oder ein Produkt können mehrere Rabatte angelegt werden, die sich jeweils auf unterschiedliche Preisjahrgänge und Preisschlüssel beziehen. Dabei muss einer der Rabatte als Default (Standard) gekennzeichnet werden.
*   **Austauschrabatt**: Austauschrabatte werden für die Komponente gewährt, die in einer Stückliste statt der Original-Komponente eingebaut werden.
*   **Staffelrabatt**: Rabatte können nach einem Grenztyp gestaffelt werden.
*   **Rabattumleitung**: In der Rabattverwaltung können Umleitungen auf andere Tarife, Rundungen, Mindestmengen und Zuschläge eingestellt werden. Damit können pro Kunde die Standardeinstellungen übersteuert werden.

> **i Kunden- und Lieferantenrabatte**
> Kunden- und Lieferantenrabatte werden auf dieselbe Weise angelegt und zur Berechnung in den Dokumenten herangezogen. In dieser Einheit wird jeweils nur von Kundenrabatten gesprochen, um die Beschreibungen leichter verständlich zu halten.

### Dialog Rabattverwaltung

Den Dialog Rabattverwaltung können Sie entweder für Kunden oder für Lieferanten öffnen. Der Unterschied beschränkt sich auf die Auswahl des Partners oder der Partnergruppe. Ansonsten sind die Register und Felder identisch.

*Abbildung B-217: Rabattverwaltung - Beispiel Kundenrabatte*
*(Die Abbildung zeigt den Dialog "Kundenrabatte". A: Register mit Detailinformationen; B: Rabatt für Partner oder Gruppe; C: Rabatt für Produkt oder WGR; D: Rabattsatz und Gültigkeit; E: Kennzeichen Standard-Rabatt; F: Rabattsatz; G: Preisjahrgang; H: Preisschlüssel; I: Gültigkeitsdatum.)*

Rabatte beziehen sich immer auf einen Preisjahrgang (G), einen Preisschlüssel (H) und ein Produkt oder eine Warengruppe (C).

#### Zeitliche Begrenzung

Eine zeitliche Begrenzung (D) können Sie für Rabatte definieren, wenn Sie für einen Kunden und ein Produkt oder eine Warengruppe mehrere Rabattsätze anlegen. Die Rabatte werden dann nur im angegebenen Zeitraum berücksichtigt. Damit können Sie z. B. Sonderaktionen im Voraus einrichten.

#### Standardrabatt

Sie können für dieselbe Warengruppe unterschiedliche Rabattsätze anlegen, indem Sie auf zwei unterschiedliche Jahrgänge und Preisschlüssel (Tarife) verweisen. Als Standard (E) kann jedoch immer nur ein Rabattsatz gekennzeichnet werden. Dieser wird im Auftrag automatisch vorgeschlagen und kann ggf. geändert werden.

### Objektbezogene Rabatte

Ein Rabatt kann sich auf ein bestimmtes Objekt begrenzen. Damit wird er nur zur Preisberechnung herangezogen, wenn sich der Auftrag auf dieses Objekt bezieht. Da das Objekt selbst mit einem Gültigkeitsdatum definiert werden kann, muss der objektbezogene Rabatt nicht zeitlich beschränkt werden.

### Staffelrabatte

Staffelrabatte können Sie auf alle Grenztypen beziehen, die auch für die Preislisten und für Zuschläge gelten. Jedoch kann der Rabatt nur mit einem Grenztyp gestaffelt werden.

### Austauschrabatte

Bei Austauschrabatten kann auf das Glas, das eingesetzt wird, ein anderer Rabatt vergeben werden als auf die ISO-Einheit selbst. Der Austauschrabatt kann zusätzlich zum Rabatt für die ISO-Einheit gewährt werden, wenn die Einstellungen in den Produktstammdaten entsprechend festgelegt sind.

> **Beispiel**
> Auf den Zuschlag des Austauschglases wird 5 % Rabatt gewährt.
> Auf das ISO werden 10 % Rabatt gewährt.
>
> *   **Übernahme Hauptposition:** 10 % Rabatt aus ISO wird ausgewertet.
> *   **Keine Übernahme:** 5 % Rabatt aus Austauschrabatt wird ausgewertet.

Die Einstellungen zur Preisübernahme sind ausführlich in der Softwarereferenz beschrieben.
⇨ Softwarereferenz, "Übernahme Hauptpos." auf Seite B-612

Wenn beim Austausch eines Glases in einem ISO ein Zuschlag berechnet wird, so kann der sich daraus ergebende Austauschpreis durch den Austauschrabatt reduziert werden.

> **Beispiel**
> 
> | Produkt | Preis | Rabatt | Gesamt |
> | :--- | :--- | :--- | :--- |
| ISO-Einheit 2 x 4 mm Float, 1 qm, (1000 x 1000 mm) | 60,00 € | 50 % | 30,00 € |
| Austausch durch ESG | 75,00 € | 30 % | 52,50 € |
| **Summe** | | | **82,50 €** |
| Austausch durch ESG mit kundenindividuellem Netto-Preis * | 75,00 € | 0 % | 75,00 € |
| **Summe** | | | **105,00 €** |
> * In diesem Beispiel wird für das Austauschglas ein kundenindividueller Preis berechnet, daher entfällt der Rabatt.

Wenn in den Firmendaten nur ein Individualpreis erlaubt ist, prüft A+W Business zunächst, ob ein Individualpreis hinterlegt ist. Erst danach wird die Rabattdefinition herangezogen. Die Tarifkombination des Individualpreises überschreibt diejenige aus den Rabatten.
⇨ Softwarereferenz, "Mehrere Individualpreise erlaubt" auf Seite B-960

### Abweichende Vereinbarungen

Über die partnerspezifische Rabatte können Sie abweichende Vereinbarungen angeben, z. B. abweichende Mindestmengen, Rundungen, Tarife (Tarifumleitung).

### Tarifumleitungen

Über die Abweichungen kann auf andere Tarife verwiesen werden, wenn für den Kunden andere Zuschläge gelten sollen, als diejenigen, die in den Standard-Preislisten vereinbart sind.

*Abbildung B-218: Umleitung von Zuschlägen*
*(Das Diagramm zeigt zwei Preislisten-Setups. Das obere Setup (Jahrgang 12, Schlüssel 12) wird für Kunde/Produkt A verwendet. Das untere Setup (Jahrgang 10, Schlüssel 10) ist der Standard für Produkt B, wird aber für den spezifischen Kunden für Produkt B verwendet, was eine Tarifumleitung darstellt.)*

*   **Preisgruppenabhängige Zuschläge:**
    Wenn kein preisgruppenabhängiger Zuschlag angegeben ist, werden zur Berechnung der Zuschläge automatisch der Jahrgang und Schlüssel (Tarif) der Hauptposition herangezogen. Diese Zuschläge können auch aus einem anderen Jahrgang und/oder Schlüssel herangezogen werden. Das System prüft dann, ob entsprechende Preisgruppen für den Jahrgang, den Preisschlüssel und das Produkt definiert sind.
    Wenn ja, sucht das Programm in den Gruppenzuschlägen nach entsprechenden Einträgen. Sind keine Einträge vorhanden, wird bei der Auftragserfassung eine Nachricht ausgegeben, dass keine Zuschläge gefunden wurden.
*   **Preisgruppenunabhängige Zuschläge (Austauschzuschläge):**
    Bei den Austauschzuschlägen gilt das gleiche Prinzip wie bei den preisgruppenunabhängigen Zuschlägen. Nur wenn sich der Jahrgang und/oder der Schlüssel für den Zuschlag von dem der Hauptposition unterscheiden soll, muss die Einstellung bearbeitet werden.
*   **Sonstige Zuschläge:**
    Wenn für den Kunden bzw. die Kundengruppe ein anderer Sonstiger Zuschlag gelten soll, kann auf diesen umgeleitet werden, z. B. andere Zuschläge für Kantenüberlängen.

### Kopierfunktion

Sie können Rabatte kopieren und dabei gleichzeitig folgende Änderungen durchführen:

*   Rabatte in einen anderen Preisjahrgang oder Preisschlüssel übertragen.
*   Rabatte auf einen anderen Partner oder eine Gruppe übertragen.
*   Rabatte insgesamt um einen prozentualen Wert oder einen festen Betrag erhöhen oder vermindern.
*   Rabatte eines Produkts oder einer WGR übertragen oder ändern.

In der Kopierfunktion haben Sie auch die Möglichkeit, alle Rabatte gemeinsam zu ändern, ohne sie dabei in einen anderen Tarif zu kopieren. Dabei stehen folgende Varianten zur Wahl:

*   Erhöhung um einen Prozentsatz oder um einen absoluten Wert.
*   Verminderung um einen Prozentsatz oder um einen absoluten Wert.
*   Erhöhung oder Verminderung auf einen festen Wert.
*   Rundung ändern.

*Abbildung B-219: Kopierfunktion für Rabatte*
*(Das Diagramm illustriert, wie Rabatte von einem Quell-Tarif (Kunde/Gruppe, Produkt/WGR, Jahrgang 11, Schlüssel 11) entweder innerhalb desselben Tarifs geändert, auf einen anderen Partner/Gruppe kopiert oder in einen neuen Tarif (z.B. Jahrgang 12, Schlüssel 12) kopiert und geändert werden können.)*

### Einstellungen zur Rabattberechnung (Firmendaten)

In den Firmendaten können Sie die Standard-Berechnung von Rabatten modifizieren.

*Abbildung B-220: Firmendaten – Preisberechnung*
*(Die Abbildung zeigt einen Dialog mit zahlreichen Checkboxen für Preisberechnungsparameter. Mehrere Optionen (A) beziehen sich auf die Rabattberechnung, wie "Keine Rabattsuche für Defaultsätze" oder "Rabattübernahme Hauptpos. Vorrang vor Bearb.-Rabatt 0%".)*

In diesem Register legen Sie Optionen für die Dokumente fest. Änderungen in diesem Register setzen die Standardberechnung in A+W Business außer Kraft.

Eine ausführliche Beschreibung der Checkboxen finden Sie in der Softwarereferenz.
⇨ Softwarereferenz, “Firmendaten – Preisberechnung" auf Seite B-959

### Rabatt anlegen

Rabatte werden für Kunden oder Lieferanten oder Gruppen von Kunden oder Lieferanten angelegt. In der folgenden Handlungsanleitung wird der Dialog Rabattverwaltung für Kunden geöffnet. Die Handlungsschritte gelten in gleicher Weise für Lieferanten.

> **i Rabatte kopieren**
> Wenn bereits Rabatte angelegt sind, können diese für neue Kunden oder Lieferanten kopiert und bearbeitet werden. In den so erstellten neuen Rabatten können die eingetragenen Werte einzeln geändert oder pauschal um einen Betrag oder Prozentsatz erhöht oder vermindert werden. Auf diese Weise sind neue Rabatte schnell erstellt. Dabei gilt, dass Preisjahrgang, Preisschlüssel und Tarif für den Ziel-Rabatt angelegt sein müssen.

#### ■ So legen Sie einen Rabatt an

1.  Wählen Sie im Menü **Stammdaten > Marktpartner > Kunden > Kundenrabatte**.
    Der Dialog **Rabattverwaltung** wird geöffnet.
    ⇨ Softwarereferenz, “Rabattverwaltung (Kunden, Lieferanten)" auf Seite B-815
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    *Abbildung B-221: Felder für neuen Rabatt freigeschaltet*
    *(Die Abbildung zeigt den Dialog "Kundenrabatte" im Neuanlage-Modus. A: Kunde, für den der Rabatt gilt; B: Tarif (Jahrgang/Schlüssel); C: Produkt, für das der Rabatt gilt; D: Defaultrabatt (Standardrabatt); E: Höhe des Rabatts.)*
    Die Register **Rabattübersicht** und **Tabelle** werden erst freigeschaltet, wenn Sie den neuen Rabatt gespeichert haben.
3.  Wählen Sie die Option **Kunde** (A) und wählen Sie die den Kunden aus, für den Sie den Rabatt angelegen.
4.  Wählen Sie den Preisjahrgang und Preisschlüssel (B) aus.
5.  Wählen Sie die Option **Produkt** (C) und das Produkt aus, auf das der Rabatt gewährt werden soll.
    Die zugehörigen Felder werden mit der Wahl der Option freigeschaltet.
6.  Geben Sie im Feld **Rabatt** den Wert (E) ein.
    Der Wert wird immer als Prozentsatz interpretiert.
7.  Markieren Sie die Checkbox **Defaultrabatt** (D), wenn dieser Rabatt standardmäßig gewährt werden soll.
    Damit haben Sie die Pflichtfelder gefüllt. Alle zusätzlichen Angaben können Sie später nachtragen.
    *Abbildung B-222: Neuer Rabatt*
8.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert. Im Register **Rabattübersicht** wird der neue Rabatt angezeigt. Sie können jetzt weitere Daten ergänzen, z. B. eine Staffelung.

### Staffelrabatt anlegen

Sie können jeden Rabatt nach einem Grenztyp staffeln. Dafür stehen dieselben Grenztypen zur Verfügung, die auch für die Staffelung von Preisen und Zuschlägen eingesetzt werden.

#### ■ So legen Sie einen gestaffelten Rabatt an

1.  Wählen Sie im Menü **Stammdaten > Marktpartner > Kunden > Kundenrabatte**.
    Der Dialog **Rabattverwaltung** wird geöffnet.
    ⇨ Softwarereferenz, "Rabattverwaltung (Kunden, Lieferanten)" auf Seite B-815
2.  Legen Sie einen neuen Rabatt an oder wählen Sie den Rabatt aus, den Sie staffeln wollen.
    ⇨ "Rabatt anlegen" auf Seite B-361
3.  Wechseln Sie zum Register **Staffelrabatt**, um die Stufen für die Staffelung einzutragen.
    *Abbildung B-223: Staffelung anlegen*
    *(A: Grenztyp für die Staffelung; B: Spaltenkopf der Rabattstufen)*
4.  Wählen Sie im Feld **Grenzmengeneinheit** (A) den Grenztyp aus, z. B. **Stück**.
    Die Auswahl wird in den Spaltenkopf (B) übernommen.
5.  Springen Sie mit der `<Tab>`-Taste ins nächste Feld und drücken Sie auf `<Einfg>`.
    *Abbildung B-224: Felder für Staffelrabatt freigeschaltet*
    *(A: Wert der Stufe (Grenzwert); B: Höhe des Rabatts)*
6.  Tragen Sie den Wert (A) für die erste Stufe ein, z. B. 5 (Stück).
7.  Tragen Sie den Wert (B) für den Rabatt ein, z. B. 0 (%) wenn der Rabatt erst ab 6 Stück gewährt werden soll.
8.  Drücken Sie auf `<Einfg>` und wiederholen Sie die Schritte 6 bis 8, bis alle Stufen angelegt sind.
    Sie können die Staffelung des Rabatts genauso anlegen, wie den gestaffelten Vektor-Preis.
9.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert. Im Register **Rabattübersicht** wird der neue Rabatt angezeigt.
    *Abbildung B-225: Übersicht Staffelrabatt*

### Austauschrabatt anlegen

Austauschrabatte werden für die Komponenten einer Stückliste angelegt, die anstelle der Original-Komponente eingebaut werden. Wenn beim Austausch eines Glases in einem ISO oder VSG ein Zuschlag berechnet wird, so kann sich dieser Zuschlag durch den Austauschrabatt reduzieren.

Ein Austauschrabatt kann sich auf ein einzelnes Produkt beziehen oder auf eine ganze Produktgruppe.

#### ■ So legen Sie einen Austauschrabatt an

1.  Wählen Sie im Menü **Stammdaten > Marktpartner > Kunden > Kundenrabatte**.
    Der Dialog **Rabattverwaltung** wird geöffnet.
2.  Legen Sie einen neuen Rabatt an oder wählen Sie den Rabatt aus, den Sie bearbeiten wollen.
    ⇨ "Rabatt anlegen" auf Seite B-361
3.  Wechseln Sie zum Register **Austauschrabatte**, um das Austauschprodukt einzutragen, für das der Rabatt gewährt werden soll.
    *Abbildung B-226: Austauschrabatt anlegen*
    *(A: Produkt (oder WGR), in dem für den Austausch ein anderer Rabatt gilt; B: Rabattsatz für das Produkt; C: Freigeschaltete Zeile; D: Produkt, das eingebaut werden soll; E: Austauschrabatt für das Produkt)*
    ⇨ Softwarereferenz, "Rabattverwaltung (Kunden, Lieferanten)" auf Seite B-815
    Die Felder für die Rabattinformationen (A, B) haben Sie beim Anlegen des Rabatts gefüllt. In den folgenden Schritten wird der Austauschrabatt für ein Produkt angelegt. Die Handlungsschritte für eine Produktgruppe gelten analog.
4.  Markieren Sie die erste Zeile (C) im Bereich **Produkte** und drücken Sie auf `<Einfg>`.
    Sie können mit der `<Tab>`-Taste springen, bis der Fokus im Bereich **Produkte** liegt.
5.  Wählen Sie im Feld **Produkt** (D) das Produkt aus, das eingesetzt werden soll.
    Die Produktbezeichnung wird in der Übersicht angezeigt.
6.  Tragen Sie im Feld **Rabatt** (E) den Prozentsatz ein, der für das getauschte Produkt gewährt werden soll.
7.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert. Um weitere Austauschrabatte einzutragen, markieren Sie den jeweils letzten Eintrag in der Übersicht und wiederholen die Schritte 4 bis 7.

### Tarifumleitung festlegen

Preise, Rabatte und Zuschläge sind immer einem Tarif (Preisjahrgang und -schlüssel) zugeordnet. Wenn im Dokument ein Produkt erfasst wird, werden der Preis und die Zuschläge aus der zugeordneten Preisliste herangezogen. Für einzelne Kunden kann jedoch festgelegt werden, dass die Preise und/oder Zuschläge aus einem anderen Tarif genommen werden sollen, z. B., wenn sich der Auftrag auf ein Objekt bezieht, zu dem eigene Tarife hinterlegt sind.

#### ■ So legen Sie eine Umleitung auf einen anderen Tarif fest

1.  Wählen Sie im Menü **Stammdaten > Marktpartner > Kunden > Kundenrabatte**.
    Der Dialog **Rabattverwaltung** wird geöffnet.
    ⇨ Softwarereferenz, "Rabattverwaltung (Kunden, Lieferanten)" auf Seite B-815
2.  Legen Sie einen neuen Rabatt an oder wählen Sie den Rabatt aus, den Sie bearbeiten wollen.
    ⇨ "Rabatt anlegen" auf Seite B-361
3.  Wechseln Sie zum Register **Abweichungen**, um andere Tarife auszuwählen.
    *Abbildung B-227: Abweichung in andere Tarife festlegen*
    *(A: Produkt (oder WGR), zu dem die Abweichungen gelten sollen. B: Objekt, bei dem die Abweichungen gelten sollen. C: Abweichender Tarif für Preise. D: Abweichender Tarif bei Gruppenzuschlägen. E: Abweichender Tarif bei Austausch- und Modellbearbeitungszuschlägen. F: Abweichender Rabatt)*
    In diesem Beispiel werden Abweichungen für ein Objekt festgelegt, wenn im Auftrag für dieses Objekt ein bestimmtes Produkt erfasst wird. Die Handlungsschritte gelten analog für eine Warengruppe.
4.  Wählen Sie das Objekt (B) aus, für das die abweichenden Tarife gelten sollen.
5.  Wählen Sie das Produkt (A) aus, für das die abweichenden Tarife gelten sollen.
6.  Tragen Sie ggf. einen abweichenden Rabatt (F) für das Produkt ein.
7.  Wählen Sie die abweichenden Tarife aus:
    *   für die Preise (C)
    *   für die preisgruppenabhängige Zuschläge (D)
    *   für die preisgruppenunabhängige Zuschläge (E).
    Wenn Sie keinen abweichenden Tarif einstellen, wird der Standard-Tarif herangezogen.
8.  Wählen Sie ggf. einen anderen **Sonstigen Zuschlag**, der für diesen Kunden gilt.
    Sie müssen einen anderen Sonstigen Zuschlag nur auswählen, wenn dieser Zuschlag von dem aus der Produktdefinition abweichen soll.
9.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert. Damit haben Sie die Umleitungen für einen Tarif festgelegt.

### Rabatte kopieren und ändern

Sie können Rabatte kopieren und dabei gleichzeitig erhöhen oder vermindern.

> **i Voraussetzung**
> Wenn ein Rabatt zu einem neuen Tarif (Jahrgang, Schlüssel) kopiert werden soll, muss der neue Tarif definiert sein.
> ⇨ "Tarife bearbeiten" auf Seite B-230

Zu diesem Thema gibt es folgende Handlungsanleitungen:

*   "So kopieren Sie Rabatte" auf Seite B-369
*   "So ändern Sie Rabatte insgesamt" auf Seite B-371

#### ■ So kopieren Sie Rabatte

1.  Wählen Sie im Menü **Stammdaten > Marktpartner > Kunden > Kundenrabatte**.
    Der Dialog **Rabattverwaltung** wird geöffnet.
    ⇨ Softwarereferenz, "Kunde" auf Seite B-814
2.  Wählen Sie im Menü **Funktionen > Rabatte kopieren**.
    *Abbildung B-228: Quell- und Ziel-Daten zum Kopieren*
    *(A: Gruppe auswählen; B: Kunde, dessen Rabatte kopiert werden; C: Tarif (Jahrgang, Schlüssel); D: Warengruppe auswählen; E: Aktion für Ziel-Rabatte)*
    ⇨ Softwarereferenz, "Rabatte kopieren, ändern" auf Seite B-823
    In diesem Beispiel wird der WGR-Rabatt eines Kunden auf eine Kundengruppe übertragen.
3.  Wählen Sie den Kunden (B) aus, dessen WGR-Rabatt Sie kopieren wollen.
    Der Kundenname wird eingelesen, wenn Sie mit der `<Tab>`-Taste weiterspringen.
4.  Aktivieren Sie Option **Gruppe** (A) wählen Sie die Kundengruppe aus, auf die der Rabatt übertragen werden soll.
5.  Markieren Sie Checkboxen für den Tarif (C).
    Die Felder **Jahrgang** und **Schlüssel** für die Quelle und das Ziel werden freigeschaltet.
6.  Wählen Sie jeweils den Jahrgang und den Schlüssel aus.
7.  Markieren Sie Checkbox **WGR** (D).
    Die Felder für die Auswahl der Warengruppen werden freigeschaltet.
8.  Wählen Sie die WGR oder die Folge von Warengruppen aus, deren Rabatte Sie kopieren wollen.
    Wenn Sie in beiden Feldern dieselbe WGR eintragen, wird nur diese eine kopiert.
9.  Markieren Sie die Checkboxen (E) für den Zielrabatt:
    *   Die vorhandenen Rabatte können überschrieben werden. Wenn Sie die Checkbox nicht markieren, werden die vorhandenen Rabatte nicht überschrieben, sondern um die neuen Rabatte ergänzt.
    *   Alle kopierten Rabatte können das Kennzeichen Default-Rabatt erhalten. Dabei wird dieses Kennzeichen an den vorhandenen Rabatten gelöscht.
10. Klicken Sie auf [OK], um die Daten zu übernehmen.
    *Abbildung B-229: Rabatte kopieren*
    Die Rabatte werden kopiert und für die Kundengruppe gespeichert. Eine Meldung zeigt an, wie viele Rabatte kopiert wurden. In der Rabattverwaltung können Sie sich die Rabatte der Kundengruppe anzeigen lassen und ggf. bearbeiten.

#### ■ So ändern Sie Rabatte insgesamt

1.  Wählen Sie im Menü **Stammdaten > Marktpartner > Kunden > Kundenrabatte**.
    Der Dialog **Rabattverwaltung** wird geöffnet.
2.  Wählen Sie im Menü **Funktionen > Rabatte ändern**.
    Der Dialog **Rabatte kopieren** wird mit dem Register **Rabatte ändern** geöffnet.
    *Abbildung B-230: Rabatte ändern*
    *(A: Wert der Änderung; B: Art der Änderung; C: Alle Rabatte auswählen; D: Kunde oder Gruppe auswählen; E: Tarif (Jahrgang, Schlüssel); F: Rabatte, die geändert werden; G: Tarif (Jahrgang, Schlüssel), in den kopiert wird)*
3.  Wählen Sie in den Feldern im Bereich **Quelle** eine der folgenden Möglichkeiten:
    *   Markieren Sie die Checkbox **alle** (C), wenn Sie sämtliche Rabatte ändern wollen. Tragen Sie dann den Preisjahrgang und den Preisschlüssel (E) ein, denen die Rabatte zugeordnet sind.
    *   Bestimmen Sie den Rabatt, indem Sie den Kunden (D) oder die Kundengruppe, den Jahrgang, den Schlüssel, die Warengruppe und das Produkt auswählen.
4.  Wählen Sie im Bereich **Rabattänderung** die Option (B) für die Änderung aus und tragen Sie den zugehörigen Wert (A) ein:
    *   **Absolut** und einen Wert, z. B. 5 oder -5, wenn die Rabatte um 5 Euro erhöht oder vermindert werden sollen.
    *   **Prozentual** und einen Wert, z. B. 2 oder -2, wenn die Rabatte um 2 % erhöht oder vermindert werden sollen.
    *   **Fix**, wenn für die Rabatte ein fester Wert eingetragen werden soll, z. B. 12, wenn alle ausgewählten Rabatte auf den Wert 12 % gesetzt werden sollen.
5.  Wählen Sie zuerst den Preisjahrgang und -schlüssel (G), in den die Änderungen geschrieben werden.
6.  Markieren Sie dann die Checkboxen (F) für die Rabatte, die geändert werden sollen.
7.  Klicken Sie auf [OK], um die Daten zu übernehmen.
    Die Daten werden gespeichert.

### Übungen

*   Legen Sie für Ihren Schulungskunden folgende Rabatte an:
    *   Standardrabatt für farbiges Floatglas
    *   Staffelrabatt für VSG-Scheiben der Dicke 8 mm
    *   Austauschrabatt für die Warengruppe ISO
*   Kopieren Sie diese Rabatte in einen anderen Tarif und erhöhen Sie den Rabattsatz um 5 %.
*   Legen Sie eine Tarifumleitung für Ihren Kunden fest, in der die nicht preisgruppenabhängigen Austauschzuschläge auf WGR 2** geleitet werden.

#### Ergänzende Informationen

*   ⇨ Softwarereferenz, "Rabatte kopieren, ändern" auf Seite B-823
*   ⇨ Softwarereferenz, "Rabatte löschen" auf Seite B-827
*   ⇨ Softwarereferenz, "Firmendaten – Preisberechnung" auf Seite B-959

# Zusatzinformationen zur Firma

Für firmenbezogene Einstellungen stehen eine Reihe von Dialogen zur Verfügung, z. B. um die Zugriffsberechtigungen für A+W Business zu hinterlegen, Mandanten und Filialen zu pflegen. Die wichtigsten dieser Einstellungen sind in diesem Themenblock beschrieben.

Dazu gehören folgende Lerneinheiten:

*   "Firmenbezogene Daten" auf Seite B-367
*   "Mitarbeiterverwaltung" auf Seite B-382

## Firmenbezogene Daten

### Lernziele

*   Überblick über die globalen Einstellungen.
*   Mandanten und Filialen kennenlernen.
*   Eigene Bankverbindungen hinterlegen.
*   Außendienst und Provisionen einrichten.

### Nutzen

*   Übergreifende Einstellungen regeln das Programmverhalten unabhängig von Kunden, Preisen und Produkten.
*   Diese Einstellungen gelten jeweils für einen Mandanten und alle seine Filialen.
*   Mit den Außendienstmitarbeitern werden Provisionen abgerechnet, die sich auf die Umsätze von Warengruppen und/oder in geografischen Bereichen beziehen.

### Merke

*   **Systemeinstellungen**: Globale Einstellungen gelten für den Mandanten, für den sie festgelegt wurden. Sie beziehen sich z. B. auf die Preisfindung, auf Schnittstellen, auf die Archivierung.
*   **Datenbank**: Die aktuellen Daten werden in der Hauptdatenbank gehalten. Abgerechnete Dokumente werden in separaten Datenbanken archiviert. Dokumente können aus der Archivdatenbank in die Hauptdatenbank kopiert werden.
*   **Finanzbuchhaltung (FiBu)**: Für den Datenaustausch mit Programmen zur Finanzbuchhaltung (FiBu) stehen verschiedene Schnittstellen zur Verfügung. Vom jeweiligen FiBu-Programm hängen verschiedene Funktionen ab, z. B. die Fremdschlüssel, Rückmeldungen zu offenen Posten (OP).
*   **Datenübergabe**: Die Übergabe von Daten an andere Programme wird in aller Regel durch einen Workflow-Task gesteuert, z. B. die Übergabe an die FiBu oder an das Archiv.
*   **Mandanten**: Mandanten greifen auf denselben Server und dieselbe Datenbank zu. Sie nutzen dieselben Stammdaten, z. B. Produkte, Warengruppen, Preise, Konditionen.
*   **Filialen**: Zu einem Mandanten können mehrere Filialen eingerichtet werden. Sie nutzen dieselben Kunden- und Auftragsdaten. Filialen der Mandanten können getrennt abgerechnet werden.
*   **Außendienst-Bereich**: Ein Außendienst-Bereich (AD-Bereich) dient folgenden Funktionen:
    *   Provisionsberechnung (Vertreterprovisionierung)
    *   Sortierkriterium in der A+W Business-Umsatzstatistik
*   **Vertreter**: Vertreter werden als Mitarbeiter angelegt. Zur Kennzeichnung eines Mitarbeiters als Vertreter wird dem Mitarbeiter ein Außendienstbereich zugeordnet.
*   **Provision**: Provisionen können sich auf einzelne Vertreter, Warengruppen und/oder Tarife beziehen.
*   **Provisionssplit**: Provisionen können prozentual zwischen zwei Vertretern aufgeteilt werden. Die Verteilung wird im Auftrag angegeben.

## Systemeinstellungen

Im Dialog **Firmendaten** definieren Sie die Standardeinstellungen für Ihr Unternehmen. Dazu gehört neben den Angaben zur FiBu und zu weiteren Schnittstellen vor allem, wie die Preisberechnung durchgeführt werden soll, z. B. in welcher Währung gerechnet wird und wie Rabatte angewendet werden.

Mit A+W Business können Sie mehrere Mandanten und deren Filialen verwalten. Für jeden Mandanten können Sie die Standardeinstellungen (Defaults) genau so definieren, wie es den jeweiligen Geschäftsabläufen entspricht.

## Finanzbuchhaltung (FiBu)

Standardmäßig wird A+W Business mit Schnittstellen zu verschiedenen FiBu-Programmen installiert. Sie müssen daher die richtige Schnittstelle für den Import und Export der Rechnungsdaten auswählen. Vom jeweiligen Programm für die FiBu hängen verschiedene Funktionen ab, z. B. die Fremdschlüssel.

Rechnungen werden je nach Schnittstelle automatisch oder manuell an die FiBu übergeben. Mit der Definition des Status legen Sie fest, welchen Mindeststatus die Rechnung erreicht haben muss. Damit sie kein zweites Mal an die FiBu übergeben wird, definieren dazu auch einen Sperrstatus.
⇨Tutorial 2, "Sperrstatus" auf Seite B-431

Barverkaufsrechnungen werden von der Übergabe an die FiBu ausgeschlossen, indem Sie diesen einen entsprechenden Status zuordnen.

Bietet das FiBu-Programm die Möglichkeit, die in A+W Business erfassten Kunden und Lieferanten per Schnittstelle zu übernehmen, entfällt das zweifache Pflegen der Kunden- bzw. Lieferantendaten. Über die Kunden- oder Lieferanten-Nummer werden Aufträge und Bestellungen zugeordnet und verbucht.

Ihre Kleinkunden rechnen Sie als sogenannte Diverse Kunden ab, für die Sie in der FiBu ein Sammelkonto nutzen. Damit müssen Sie für diese nicht einzelne Konten anlegen.

Bei der OP-Rückmeldung (Offene Posten) werden alle offenen Rechnungen mit Angabe der ausstehenden Summe, Mahndatum und Mahnstufe aufgelistet. Im Zusammenspiel mit dem Kreditlimit und dem Kreditlimit-Snapshot sehen Sie immer den aktuellen Kontostand jedes einzelnen Kunden.

## Datenbank

In der Hauptdatenbank sind alle Dokumente verfügbar, die in A+W Business erfasst wurden. Um die gewohnte Verarbeitungsgeschwindigkeit aufrechtzuerhalten, müssen die alten Dokumente archiviert und aus dieser Datenbank gelöscht werden.

Die Dokumente werden gleichzeitig an das Archiv und die Statistik übergeben und anschließend standardmäßig aus der Hauptdatenbank gelöscht. Für die Übergabe an die Statistik ist in der Regel der Monat des Dokumentendatums ausschlaggebend, für die Archivierung ist das Jahr ausschlaggebend.

Nach der Übergabe der Daten an das Archiv wird die Hauptdatenbank reindiziert, um die gewohnte Verarbeitungsgeschwindigkeit wieder herzustellen.

## Archivierung

Abgeschlossene Geschäftsvorgänge bleiben für eine von Ihnen definierte Zeit in der Hauptdatenbank und werden dann automatisch archiviert. Ausschlaggebend dafür ist der Mindeststatus, den Sie für die Archivierung festgelegt haben. Alle Dokumentendaten werden unverändert gespeichert. Sie können als Kopie aus dem Archiv geholt werden.

*Abbildung B-231: Einstellungen für die Archivierung*
*(Die Abbildung zeigt den Archivierungsdialog. A: Globale Einstellungen zur Archivierung. B: Dokumentenbezogene Einstellungen. C: Archivjahr. D: Voraussetzungen für die Archivierung.)*

In diesem Beispiel sehen Sie welche Einstellungen übergreifend (A) und welche für die einzelnen Dokumententypen (B) festgelegt werden können.

Die Archive bilden eigene Datenbanken, die jeweils ein Jahr (C) zusammenfassen. Beim Jahreswechsel archiviert das System die Dokumente in Abhängigkeit vom Rechnungsdatum im entsprechenden Archiv.

Die Dokumente können manuell per Nummernverwalter an das Archiv übergeben werden. Da die Archivierung sehr rechenintensiv ist, wird sie in der Regel allabendlich und vollautomatisch ausgeführt.

## Statistik

Mit dem Modul Statistik stellt A+W Business eine Reihe von Berichten (Reports) zur Verfügung. Für die Auswertung werden die Dokumente an die Statistik übergeben. Für jede Dokumentenart legen Sie fest, ob und wann das entsprechende Dokument übergeben werden soll.

Die Dokumente werden gleichzeitig an die Statistik und an das Archiv übergeben. Für die Statistik werden bestimmte Auftragsdaten in eine eigene Tabelle in der Hauptdatenbank geschrieben.

## Tagesabschluss

Rechnungen können z. B. einmal pro Tag in einem nächtlichen Batch-Lauf an die FiBu übergeben werden. In der Regel werden die Dokumente bei der Übergabe an die FiBu (automatisch) sowohl an das Archiv als auch an die Statistik übergeben.

Anhand hinterlegter Fristen (Vorhaltetage) prüft das System, wie lange die Dokumente in der Hauptdatenbank gespeichert bleiben sollen, bis sie automatisch gelöscht werden.

Dabei werden alle Daten aus der Hauptdatenbank gelöscht, die älter sind als die eingetragenen Fristen. Die Fristen bestimmen Sie pro Dokumentenart selbst.

> **Beispiel**
> Wenn Sie Jahresübersichten erzeugen wollen, sollten Sie einen langen Zeitraum eintragen, um einen ausreichenden Spielraum für die Erstellung der Auswertung zu haben.
> Für die Provisionsstatistik ist der Rhythmus ausschlaggebend, in dem Sie Provisionen abrechnen.

## Mandanten und Filialen

Mandanten setzen Sie dann ein, wenn mehrere Firmen auf den gleichen Server und die gleiche Datenbank zugreifen wollen. Mandanten nutzen dieselben Stammdaten, z. B. Produkte, Warengruppen, Preise, Konditionen. Sie pflegen aber jeweils einen eigenen Kundenstamm.

Sie können in Ihrem Unternehmen (Firma) sowohl Filialen als auch Mandanten mit Filialen verwalten. Welche Version Sie wählen, hängt davon ab, wie die Kundendaten und die Aufträge verwaltet werden sollen:

*   Sie richten Mandanten ein, wenn Ihre Zweigstellen (Subunternehmen) jeweils eigene Kundendaten und Aufträge verwalten sollen.
*   Sie richten Filialen ein, wenn die Zweigstellen mit denselben Kundendaten arbeiten.

Auch die FiBu-Konten können getrennt pro Mandant geführt werden. Interne Leistungen der Mandanten können gegeneinander verrechnet werden.

*Abbildung B-232: Firma, Mandant, Filialen – Stammdaten, Kunden, Aufträge*
*(Das Diagramm zeigt zwei Architekturen. Links: Eine Firma mit Filialen (A, B, C) teilt sich eine Datenbank für Stammdaten, Kunden und Aufträge. Rechts: Zwei Mandanten (1 und 2) auf demselben Datenbank-Server teilen sich Stammdaten (Produkte, Warengruppen, Preise), haben aber getrennte Nummernkreise für Kunden und Aufträge.)*

In diesem Beispiel sehen Sie, dass z. B. die Nummernbereiche für die Kundennummern pro Mandant festgelegt sind. Die Dokumentennummern werden aus getrennten Nummernkreisen vergeben.

Die Einstellungen für Dokumente und Preisberechnung werden pro Mandant festgelegt. Damit bestimmen Sie u. a., wie Positionen erfasst und im Dokument dargestellt werden. Mit den Parametern für die Preisberechnung überschreiben Sie teilweise die Standard-Berechnungen aus den Stammdaten. Grundsätzlich haben aber die Einstellungen zu Preisen und Rabatten für einzelne Kunden oder Kundengruppen oberste Priorität.

Bei Filialen werden die Stammdaten nur im Hauptsitz gepflegt und dann an die Filialen übertragen (Replikation). Jedoch wird ein Produkt nicht automatisch auch bei den Filialen gelöscht, wenn es im Hauptsitz gelöscht wurde. Es muss in allen Filialen manuell gelöscht werden. Damit können die Filialen ein Produkt dann aus der Produktverwaltung löschen, wenn es ausverkauft ist.

Voraussetzung für die Replikation ist, dass alle Filialen mit A+W Business arbeiten und alle Datenbanken den gleichen Release-Stand haben.

## Mandant anlegen

Sie können mit A+W Business mehrere Mandanten mit jeweils mehreren Filialen verwalten. Die Firmeneinstellungen gelten jeweils für einen Mandanten und seine Filialen. Mandanten können nicht gelöscht werden (referentielle Integrität).

Bevor Sie einen Mandanten anlegen, sollten Sie festlegen, wodurch er sich von anderen Mandanten unterscheidet. Das hilft Ihnen, die spezifischen Einstellungen für den Mandanten anzupassen, z. B. Nummernkreise, automatische Zuschläge, Rundungszuordnungen, Kundennummern.

> **i Einstellungen pro Mandant pflegen**
> Beachten Sie bitte, dass Sie neue Mandanten auf der Basis von bereits hinterlegten Daten anlegen. Sie sollten anschließend in allen relevanten Dialogen die Einstellungen prüfen und anpassen.

### ■ So legen Sie einen Mandanten an

1.  Wählen Sie im Menü **Stammdaten > Firma > Firmendaten**.
    Der Dialog **Firmendaten** wird geöffnet.
2.  Wählen Sie in der Übersicht **Tabelle** den Mandanten aus, der die meisten Übereinstimmungen mit dem neuen Mandanten aufweist.
3.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    *Abbildung B-233: Felder für neuen Mandanten freigeschaltet*
    *(A: Nummer, interne Firmennummer; B: Anschrift; C: Kommunikationsdaten)*
    ⇨ Softwarereferenz, "Firmendaten - Mandant" auf Seite B-931
4.  Passen Sie die Mandanten- und Firmennummern an.
    Die Mandantennummer kann nach dem Speichern nicht mehr geändert werden.
5.  Tragen Sie ggf. einen eindeutigen Matchcode ein.
6.  Tragen Sie mindestens die Adress- und Kommunikationsdaten ein.
7.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.
8.  Passen Sie ggf. weitere Einstellungen im Dialog **Firmendaten** an.
9.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert. Sie sollten jetzt prüfen, welche weiteren Anpassungen für den Mandanten notwendig sind, z. B. Nummernkreise, automatische Zuschläge.

## Bankverbindung hinterlegen

Sie können für Ihre eigene Firma und pro Mandant mehrere Konten bei unterschiedlichen Banken hinterlegen.

Wenn für einen Mandanten mehrere Bankverbindungen eingetragen sind, muss eine als Hauptbank gekennzeichnet werden.

> **i Voraussetzung**
> Um die Kontonummer für einen Mandanten eintragen können, müssen die Bankdaten angelegt sein. Die IBAN wird nur dann automatisch berechnet, wenn die Bankdaten vollständig hinterlegt sind.
> ⇨ "Banken" auf Seite B-91

### ■ So hinterlegen Sie Bankverbindungen für einen Mandanten

1.  Wählen Sie im Menü **Stammdaten > Firma > Banken**.
    Der Dialog **Banken** wird geöffnet.
    ⇨ Softwarereferenz, "Banken" auf Seite B-1039
2.  Wählen Sie den Mandanten aus, zu dem Sie die Daten hinterlegen wollen.
3.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    Alle Felder werden gelöscht, wenn zu dem gewählten Mandanten noch keine Bankverbindung hinterlegt ist.
    *Abbildung B-234: Felder für neue Bankverbindung freigeschaltet*
    *(A: Bank auswählen; B: Kontonummer; C: Kennzeichen für Hauptbank)*
4.  Klicken Sie auf die Lupe, um die Bank (A) auszuwählen.
    Die Daten der Bank werden eingelesen.
    Wenn die Bankdaten noch nicht hinterlegt sind, können Sie den entsprechenden Dialog über die Ordner-Schaltfläche öffnen und die Daten nachtragen.
5.  Tragen Sie die Kontonummer (B) ein.
    Die IBAN wird automatisch errechnet und angezeigt.
6.  Markieren Sie ggf. die Checkbox **Hauptbank** (C).
    Sie können dieses Kennzeichen später ändern, wenn Sie alle Bankverbindungen hinterlegt haben.
7.  Wählen Sie den Mandanten aus, zu dem Sie die Daten hinterlegen wollen.
    Die Auswahl des Mandanten ist nur erforderlich, wenn Sie die erste Bankverbindung hinterlegen. Wenn Sie weitere Bankverbindungen für den Mandanten hinterlegen, entfällt dieser Schritt.
8.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.

## Vertreterprovision

Im Dialog **Vertreterprovision** legen Sie die Provisionssätze für jeden einzelnen Vertreter fest. Sie müssen für jeden Vertreter und mindestens für jede Warenhauptgruppe (WHG) einen Provisionssatz anlegen.

Die Provision können Sie nach verschiedenen Preislisten unterscheiden. Wenn für Jahrgang und Schlüssel `<k.A.>` angegeben ist, gilt der Provisionssatz für alle Tarife.

*Abbildung B-235: Verwaltung – Vertreterprovision*
*(A: Provision ist allgemeingültig; B: Basis der Berechnung; C: Menge in Stück, für die der Provisionssatz berechnet wird; D: Provisionssatz pro Staffelmenge)*

Die Provision kann beliebig gestaffelt werden.

**Beispiele Staffelung nach Rabatt, Staffelung nach Umsatz**

| Bis %-Rabatt | %-Provision | Bis Umsatz | %-Provision |
| :--- | :--- | :--- | :--- |
| 10 | 5 | 999.999.999 | 5 |
| 20 | 3 | 5.000 | 3 |
| 40 | 1 | 1.000 | 1 |
| 99 | 0 | 0 | 0 |

Die Staffelmenge hängt von der Provisionsart ab.

**Beispiel Provisionsarten**

| Provisionsart | Menge |
| :--- | :--- |
| Rabatt % | Gewährter Rabattsatz pro Auftrag/Position |
| Deckungsbeitrag % | Deckungsbeitrag in Prozent |
| Umsatz | Gesamtumsatz des Vertreters |
| Deckungsbeitrag | Deckungsbetrag |
| Preis/PE | Preis pro Mengeneinheit |

### Provisionssplitt und manuelle Provisionssätze

Die Vertreter werden in den Partnerdaten zugewiesen. Wenn zwei Vertreter angegeben werden, kann festgelegt werden, wie die Provision verteilt werden soll. Vertreterprovisionen werden anhand der Aufträge errechnet.

*Abbildung B-236: Kundendaten – Register Vertrieb*
Die Angaben den Kundendaten wird in den Auftrag übernommen und können geändert werden.

*Abbildung B-237: Auftrag - Voreinstellungen der Vertreter*
*(A: Register Dokument: Vertreter 1; B: Register Zusatz: Vertreter 2; C: Provisionsanteil)*

Wenn Sie für den zweiten Vertreter (im Auftrag) keine Angaben machen, erhält er aus diesem Auftrag keine Provision. Das Provisionssplitting bezieht sich auf die Provision, die nach den Angaben im Dialog **Vertreterprovision** berechnet wird.

Im Auftrag können Sie die Voreinstellung in der Positionserfassung überschreiben.

*Abbildung B-238: Position - Register Zusatz*
Pro Position können zwei verschiedene Provisionssätze angegeben werden. Diese werden jeweils dem Vertreter 1 und Vertreter 2 zugeordnet.

**Beispiele für die Berechnung**

*   **Provision 0,75 % auf Glaspreis**
    *   Auftrag = 2000,00 € für Glas, Provisionssplit
        *   **Gesamt: 15,00 €**
        *   Vertreter 1: 10,05 €
        *   Vertreter 2 (33,5%): 4,95 €
*   **Position = 2000,00 €, manuelle Provisionssätze**
    *   Vertreter 1 (1,00 %): 20,00 €
    *   Vertreter 2 (0,75 %): 15,00 €

### Abrechnung der Provision

Die Vertreterprovision wird positionsweise anhand der WGR der Position errechnet. Wenn die Reklamationen bei der Berechnung berücksichtig werden, verringert sich die Provision. Für statistische Auswertungen können die Aufträge an die Provisionsstatistik übergeben werden. Die Aufträge werden dann mit der Übergabe an das Archiv auch an die Provisionsstatistik übergeben. Diese Funktionen müssen in den Firmendaten aktiviert werden.

⇨ Softwarereferenz, "Firmendaten - Archiv" auf Seite B-978

Standardmäßig wird die Vertreterprovision bei der Übergabe der Dokumente an das Archiv ermittelt. Dazu müssen in den Firmendaten folgende Einstellungen aktiviert sein:

*   Im Register **Archiv** die Checkbox **Übergabe Provisionsstatistik**.
*   Im Register **Parameter** die Checkbox **Interaktive Vertreterprovisionierung**.

*Abbildung B-239: Firmendaten - Register Parameter*

Wenn diese Funktion nicht aktiviert ist, werden die Provisionssätze aus den Stammdaten zur Berechnung der Provision erst bei der Übergabe an die Provisionsstatistik herangezogen.

Die Aufträge können auch manuell übergeben werden. Dazu nutzen Sie den Dialog zur Archivierung im Modul **Dokumente**.

Diese Einstellungen für die Provisionierung gelten für Aufträge und für Gutschriften.

### Provision anlegen

In diesem Beispiel wird eine gestaffelte Provision angelegt, die für alle Preislisten gelten soll.

#### ■ So legen Sie eine Vertreterprovision an

1.  Wählen Sie im Menü **Stammdaten > Firma > Vertreterprovision**.
    Der Dialog **Vertreterprovision** wird geöffnet.
    ⇨ Softwarereferenz, “Vertreterprovision" auf Seite B-1036
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    *Abbildung B-240: Felder für neuen Provisionssatz freigeschaltet*
    *(A: Vertreter; B: Tarif; C: Provisionsart; D: Staffelmenge; E: Prozentsatz der Provision)*
3.  Tragen Sie ggf. den Tarif (Jahrgang und Schlüssel) ein (B).
    Wenn Sie jeweils den Wert `<k.A.>` eintragen, gilt die Provision für alle Preislisten.
4.  Wählen Sie den Vertreter (A) aus.
    Als Vertreter werden nur die Mitarbeiter angeboten, die im Dialog **AD-Bereiche** hinterlegt sind. Wenn Sie `<k.A.>` auswählen, gilt die Provision für alle Vertreter.
5.  Wählen Sie die Provisionsart (C) aus, z. B. **Umsatz**.
    Damit haben Sie die Mindestangaben für die Kopfdaten erfüllt. Diese Angaben können nachträglich nicht geändert werden. Wenn Sie den Provisionssatz jetzt einfügen, können Sie nur noch die Staffelmenge und den Prozentsatz der Provision angeben. Wenn die Provision weiter differenziert werden soll, geben Sie auch die Daten für Kunden usw. ein.
6.  Wählen Sie ggf. einen Kunden, die Warengruppe und/oder das Produkt aus.
    Wenn Sie in diesen Feldern keine Werte eingeben, gilt die Provision für alle Kunden, Warengruppen und Produkte.

> **i Angaben ändern**
> Die Angaben aus den Schritten 3 bis 6 können Sie nachträglich nicht ändern. Prüfen Sie die Felder daher sorgfältig, bevor Sie den nächsten Schritt ausführen.
> Wenn Sie später feststellen, dass die Provision nicht richtig angelegt ist, müssen Sie den gesamten Eintrag löschen und neu anlegen.

7.  Tragen Sie den Wert für **Staffelmenge** (D) und den **Provisionssatz** (E) ein.
    Wenn Sie die Provision nicht staffeln wollen, tragen Sie für die Menge **99999999** ein.
8.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.

#### ■ So legen Sie eine gestaffelte Provision an

1.  Legen Sie einen Provisionssatz an, wie in der vorhergehenden Handlungssequenz beschrieben.
    Es spielt keine Rolle, wie groß Sie die erste Stufe für die Staffelung wählen.
2.  Markieren Sie den Provisionssatz, zu dem Sie eine weitere Stufe festlegen wollen.
3.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    Achten Sie darauf, dass die Einstellungen im Bereich **Auswahl Vertreter/Warengruppe** unverändert übernommen werden.
4.  Tragen Sie den Wert für **Staffelmenge** (D) und den **Provisionssatz** (E) ein.
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.
6.  Wiederholen Sie die Schritte 3 bis 5, bis Sie alle Stufen angelegt haben.

Die Reihenfolge, in der die Provisionssätze in der Übersicht aufgeführt werden, hat keinen Einfluss auf die Berechnung. Sie können sie mit einem Doppelklick in einen Spaltenkopf sortieren.

#### ■ So löschen Sie eine Vertreterprovision

1.  Wählen Sie im Menü **Stammdaten > Firma > Vertreterprovision**.
    Der Dialog **Verwaltung – Vertreterprovision** wird geöffnet.
2.  Markieren Sie in der Übersicht den Provisionssatz, den Sie löschen wollen.
3.  Wählen Sie im Menü **Start > Löschen**.
4.  Bestätigen Sie die Sicherheitsabfrage mit [Ja].
    Der markierte Provisionssatz wird gelöscht.

## Mitarbeiterverwaltung

### Lernziele

*   Mitarbeiterdaten anlegen und in Gruppen verwalten.
*   Zugriffsrechte für Mitarbeiter einrichten.

### Nutzen

*   Nur eingetragene Mitarbeiter können mit A+W Business arbeiten. Damit ist der unberechtigte Zugriff auf die Daten erschwert.
*   Mitarbeiter können unterschiedliche Rechte erhalten. So können Sie steuern, welche Mitarbeiter Zugriff auf bestimmte Daten haben.

### Merke

*   **Datenschutz beachten**: Personenbezogene Daten unterliegen dem Datenschutz. Achten Sie daher darauf, dass diese Daten durch entsprechende Zugriffsrechte vor Missbrauch geschützt sind.
*   **Mitarbeiterdaten**: Um mit A+W Business arbeiten zu können, müssen die Zugangsdaten der Mitarbeiter hinterlegt werden. Nur die angelegten Mitarbeiter können das Programm starten.
*   **Mitarbeiterrechte**: Die Mitarbeiter Ihres Unternehmens können unterschiedliche Zugriffsrechte auf die Daten in A+W Business erhalten. Die Rechte werden durch Restriktionen definiert.
*   **Mitarbeitergruppe**: Standardmäßig sind folgende Mitarbeitergruppen eingerichtet:
    *   Manager
    *   Supervisor
    *   Anwender
    *   Geschäftsleitung
    Jede dieser Gruppen hat unterschiedliche Zugriffsrechte, die an die betrieblichen Aufgabenstellungen angepasst sind.
*   **Profil**: Die Rechtevergabe kann über vordefinierte Profile vereinfacht werden.
*   **Voraussetzung**: Sie können neue Mitarbeiter nur anlegen und Rechte vergeben, wenn Sie die Rechte des Systemadministrators haben.

> **i Mitarbeiterinnen und Mitarbeiter**
> Selbstverständlich können sowohl weibliche als auch männliche Mitarbeiter mit A+W Business arbeiten. In dieser Einheit wird aus Gründen der Vereinfachung und besseren Lesbarkeit die männliche Form verwendet. Darin ist das weibliche Geschlecht mit einbezogen.
> Zusammenfassungen (MitarbeiterInnen) entsprechen nicht den Regeln der deutschen Rechtschreibung und werden daher nicht benutzt.

### Mitarbeiter

Alle Mitarbeiter, die mit A+W Business arbeiten, müssen im System angelegt werden. Der sogenannte Klarname des Mitarbeiters wird bei jeder Aktion mit gespeichert. In einigen Dialogen wird dieser Name auch angezeigt, z. B. im Dialog Nummernverwalter. Außerdem können Sie für jeden Mitarbeiter eigene Nummernkreise einrichten. Jeder Mitarbeiter kann seine eigenen Nummernverwalter anlegen.

Die Anmeldung im Programm wird mit einem Passwort ermöglicht. Sie kann in den Firmendaten mit der Windows-Anmeldung gekoppelt werden.

> **i Datenschutz beachten**
> Personenbezogene Daten unterliegen dem Datenschutz. Achten Sie daher darauf, dass diese Daten durch entsprechende Zugriffsrechte vor Missbrauch geschützt sind.

Mitarbeiterdaten können nicht gelöscht werden. Scheidet ein Mitarbeiter aus dem Betrieb aus, muss er in der Mitarbeiterverwaltung gesperrt werden.

### Voreinstellungen für Dokumente und AV-Bereiche

Mit Vorgaben zu Dokumenten und AV-Bereichen kann die Bearbeitung von Dokumenten auf einen Mandanten, einen AV-Bereich und bestimmte Dokumententypen festgelegt werden. Diese Einstellungen können im Dokument überschrieben werden.

*Abbildung B-241: Voreinstellungen für Dokumente*
*(A: Dokumentenarten und AV-Bereiche; B: Standard-Dokument des Mitarbeiters)*

In diesem Beispiel sehen Sie, dass dem Mitarbeiter eine bestimmte Dokumentenart zugeordnet ist, wenn er Bestellungen erfasst.

Wenn Sie auch den AV-Bereich angeben, legen Sie fest, dass die Dokumente des Mitarbeiters automatisch dem AV-Bereich zugeordnet werden und dabei die Nummern aus dem zugehörigen Nummernkreis gezogen werden.

Der Eintrag in der Spalte **Allgemein** (A) übersteuert die Einträge für die anderen Dokumententypen und AV-Bereiche. Das bedeutet, dass Sie dann keine weitere Auswahl treffen können:

*   **<k.A.> oder eine andere Auswahl:**
    In allen anderen Spalten wird `<deaktiviert>` angezeigt.
*   **<deaktiviert>:**
    In den anderen Spalten können der Dokumententyp oder AV-Bereiche ausgewählt werden.

> **Beispiel AV-Bereich - Spalte Allgemein**
> 
> *   **<k.A.>**
>     Wenn keine Vorgaben zu den Dokumenten eingestellt sind, werden in den AV-Bereichen keine Vorbelegungen verwendet. Der Mitarbeiter muss dann darauf achten, den richtigen AV-Bereich und die Dokumentenart auszuwählen.
> *   **ESG**
>     Für die Dokumente können keine Vorbelegungen eingestellt werden. Wenn der Mitarbeiter ein Dokument erfasst, wird standardmäßig der AV-Bereich ESG vorgegeben. Das Dokument erhält die Nummer aus dem entsprechenden Nummernkreis. Die Nummer wird beim erst Speichern des Dokuments vergeben.

### Mitarbeitergruppen

Standardmäßig sind folgende Mitarbeitergruppen eingerichtet: Manager, Supervisor, Anwender, Geschäftsleitung. Jede dieser Gruppen hat unterschiedliche Zugriffsrechte, die an die betriebliche Aufgabenstellung angepasst sind. Diese vordefinierten Mitarbeitergruppen und Mitarbeiterrechte können bearbeitet und ergänzt werden.

Für umfangreiche Modifikationen legen Sie am besten eine neue Gruppe mit den entsprechenden Rechten an.

Wenn Sie einen (neuen) Mitarbeiter einer der Mitarbeitergruppen zuordnen, so erhält er automatisch alle Rechte dieser Gruppe. Soll er modifizierte Rechte erhalten, so können Sie diese speziell für ihn ergänzen oder anpassen.

### Mitarbeiterrechte

Die Mitarbeiter Ihres Unternehmens können unterschiedliche Zugriffsrechte auf die Daten in A+W Business erhalten, so dass Sie sehr fein steuern können, welche Bereiche für wen offen oder gesperrt sind.

Folgende Rechte können aktiviert bzw. deaktiviert werden:

*   **Ändern:**
    Daten dürfen bearbeitet werden.
*   **Einfügen:**
    Neue Datensätze dürfen angelegt werden.
*   **Löschen:**
    Datensätze dürfen gelöscht werden.
*   **Ausführen/Lesen:**
    Der Dialog darf geöffnet werden.

Bei diesen Einstellungen müssen Sie die logischen Zusammenhänge beachten: Wenn ein Mitarbeiter das Recht zum Anlegen von Daten hat, muss er auch das Recht haben, den Dialog zu öffnen.

Die Rechtevergabe bezieht sich auf alle Programmbereiche von A+W Business bis auf die Ebene der Dialoge und zum Teil auch auf die Felder.

> **Beispiel**
> Soll ein Mitarbeiter im Modul Dokumente Preise in archivierten Aufträgen einsehen dürfen, so muss er für die Programmpunkte 0055 Dokumente-Archive-Auftrag-Suche und 0002 Preisanzeige das Recht zum Ausführen haben.

*Abbildung B-242: Rechteverwaltung*
*(A: Mitarbeitergruppe oder Mitarbeiter; B: Programm und Subrecht; C: Anzeige der Rechte für das markierte Programm)*

Im Beispiel sehen Sie, dass die ausgewählte Gruppe im Auftrag die Einkaufspreise **lesen** darf, jedoch nicht ändern, einfügen oder löschen (C).

> **i Die Rechte werden durch Restriktionen definiert**
> Alle angezeigten Programmpunkte sind mit eingeschränkten Rechten definiert. Alle nicht angezeigten Programmpunkte stehen uneingeschränkt zur Verfügung.
>
> Für die Zuteilung oder den Entzug von Rechten gilt folgende Systematik:
> 
> | Programmpunkt (Dialog, Feld) | Recht |
> | :--- | :--- |
> | Nicht in der Liste aufgeführt. | = Voller Zugriff |
| In der Liste aufgeführt, keine Checkbox ist markiert. | = Dialog oder Feld ist gesperrt. |
| In der Liste aufgeführt, eine oder mehrere Checkboxen sind markiert. | = Die jeweilige Aktion ist erlaubt. |

### Mitarbeiterprofile

Die Rechtevergabe kann über vordefinierte Profile vereinfacht werden. Diese bieten folgende Einstellungen an:

*   **Alle Programme ohne Rechte**
    Für alle Programme werden Sätze angelegt und die Rechte zum Ausführen, Ändern, Einfügen und Löschen werden deaktiviert, z. B. für ausgeschiedene Mitarbeiter.
*   **Alle Programme ausführbar**
    Für alle Programme werden Sätze angelegt. Nur das Recht zum Ausführen wird aktiviert. Alle anderen werden deaktiviert. Die Dialoge dürfen damit nur geöffnet werden.
*   **Alle Programme mit allen Rechten**
    In diesem Fall werden bei der betreffenden Gruppe alle Einträge gelöscht, sie hat dann wie der Supervisor alle Rechte.

### Beispiele für Gruppen- und Mitarbeiterrechte

Im Dialog Rechteverwaltung werden die Rechte mit Hilfe von Checkboxen erteilt oder entzogen.

Die Markierung einer Checkbox bedeutet immer eine Ausnahme von der übergeordneten Einstellung. Dies wird in den nachfolgenden Beispielen gezeigt.

In den stark vereinfachten Beispielen sind nur die Hauptprogramme aufgeführt, da die Darstellung aller Unterpunkte zu unübersichtlich wäre. Natürlich können auch Rechte für alle Unterpunkte festgelegt werden.

#### Gruppe: Supervisor = Systemadministrator

| Programm | Subrecht | Ausführen | Ändern | Einfügen | Löschen |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Stammdaten | | x | x | x | x |
| Dokumente | | x | x | x | x |
| Fertigung | | x | x | x | x |
| Statistik | | x | x | x | x |
| Lager | | x | x | x | x |
| Kapazitätspl. | | x | x | x | x |
| Utilities | | x | x | x | x |
| Referenzen | | x | x | x | x |
*x: alle Rechte (kein Eintrag)*
*Tab. B-17: Zugriffsrechte Supervisor*

Der Supervisor hat automatisch alle Rechte. Daher sind keine Programme aufgelistet und keine Checkboxen markiert.

#### Gruppe: Anwender

| Programm | Subrecht | Ausführen | Ändern | Einfügen | Löschen |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Stammdaten | | ☑ | ☐ | ☐ | ☐ |
| Dokumente | | ☑ | ☑ | ☑ | ☑ |
| Fertigung | | ☑ | ☐ | ☐ | ☐ |
| Statistik | | ☐ | ☐ | ☐ | ☐ |
| Lager | | ☑ | ☐ | ☐ | ☐ |
| Kapazitätspl. | | ☑ | ☐ | ☐ | ☐ |
| Utilities | Auftragsinfo | ☐ | ☐ | ☐ | ☐ |
| | Debit./Kredit. | ☐ | ☐ | ☐ | ☐ |
| Referenzen | | ☐ | ☐ | ☐ | ☐ |
*x: alle Rechte (kein Eintrag)*
*Tab. B-18: Zugriffsrechte Anwender*

Die Gruppe **Anwender** kann Dokumente erfassen, ändern, löschen und ausführen. In den Modulen **Stammdaten, Fertigung, Lager und Kapazitätsplanung** kann sie die einzelnen Dialoge nur öffnen, da die Checkboxen **Ändern, Einfügen und Löschen** nicht markiert sind. Im Modul **Utilities** kann sie die Dialoge **Auftragsinfo** und **Debitoren/Kreditoren an FIBU** nicht öffnen, auf alle anderen Dialoge des Moduls hat sie vollen Zugriff. In den Modulen **Statistik** und **Referenzen** hat die Gruppe keine Rechte.

#### Mitarbeiter: Marc Tender, Anwender

| Programm | Subrecht | Ausführen | Ändern | Einfügen | Löschen |
| :--- | :--- | :--- | :--- | :--- | :--- |
| Stammdaten | | ☑ | ☐ | ☐ | ☐ |
| | Partner | ☑ | ☑ | ☑ | ☑ |
| Dokumente | | ☑ | ☑ | ☑ | ☑ |
| Fertigung | | ☑ | ☐ | ☐ | ☐ |
| Statistik | x | | | | |
| Lager | | ☑ | ☐ | ☐ | ☐ |
| Kapazitätspl. | x | | | | |
| Utilities | Auftragsinfo | ☐ | ☐ | ☐ | ☐ |
| | Debit./Kredit. | ☐ | ☐ | ☐ | ☐ |
| Referenzen | x | | | | |
*x: alle Rechte (kein Eintrag)*
*Tab. B-19: Zugriffsrechte eines Mitarbeiters*

Der Mitarbeiter Marc Tender gehört zur Gruppe **Anwender**. Er hat zusätzlich vollen Zugriff auf die Module **Statistik, Kapazitätsplanung und Referenzen**. Außerdem kann er in den Stammdaten **Partner** anlegen, bearbeiten und löschen.

### Mitarbeiterdaten anlegen

Wenn Sie die Daten eines Mitarbeiters anlegen, müssen Sie den sogenannten Klarnamen eingeben. Dieser Eintrag kann nach dem Speichern nicht mehr geändert werden.

Außerdem vergeben Sie ein Passwort, mit dem sich der Mitarbeiter in A+W Business anmeldet. Wenn Sie in den Firmendaten die Login-Funktion mit der Windows-Anmeldung aktiviert haben, müssen der Benutzername und das Passwort der Windows-Anmeldung in A+W Business eingetragen werden.

⇨ Softwarereferenz, "Windows-Anmeldung für A+W Business-Login benutzen" auf Seite B-990

> **i Voraussetzung**
> Sie können neue Mitarbeiter nur anlegen, wenn Sie die Rechte des Systemadministrators haben.

Zu diesem Thema gibt es folgende Handlungsanleitungen:

*   "So legen Sie einen Mitarbeiter an" auf Seite B-399
*   "So kopieren Sie Standard-Einstellungen für die Dokumente" auf Seite B-401

> **i Datenschutz beachten**
> Personenbezogene Daten unterliegen dem Datenschutz. Achten Sie daher darauf, dass diese Daten durch entsprechende Zugriffsrechte vor Missbrauch geschützt sind.

In den folgenden Handlungssequenzen wird ein Praktikant für die Lagerverwaltung angelegt, der mit eingeschränkten Rechten zur Gruppe Anwender gehört.

#### ■ So legen Sie einen Mitarbeiter an

1.  Wählen Sie im Menü **Stammdaten > Firma > Mitarbeiter**.
    Der Dialog **Mitarbeiter** wird geöffnet.
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    *Abbildung B-243: Felder für neue Mitarbeiterdaten freigeschaltet*
    *(A: Klarname; B: Domäne; C: Loginname)*
    ⇨ Softwarereferenz, "Mitarbeiter - Mitarbeiter" auf Seite B-1022
3.  Tragen Sie die Daten im Bereich **Identifikation** ein:
    *   **Klarname (A):** Name des Mitarbeiters, vorzugweise der Nachname. Er kann nach dem Speichern nicht mehr geändert werden. Der Klarname wird zu jeder Aktion gespeichert, die der betreffende Mitarbeiter in A+W Business ausführt. Der Klarname wird in der Statuszeile von Dialogen und in Auswahllisten angezeigt, z. B. in der Auftragserfassung.
    *   **Domäne (B):** Name der Domäne, wenn der Computer in einem Netzwerk installiert ist.
    *   **Loginname (C):** Name, mit dem sich der Mitarbeiter im System anmeldet.
    Die weiteren Felder müssen nicht zwingend gefüllt werden. Bei externen Mitarbeitern können z. B. die Kommunikationsdaten hilfreich sein.
4.  Wechseln Sie zum Register **Spezifikation**.
    *Abbildung B-244: Spezifische Einstellungen für den Aufruf von A+W Business*
    *(A: Mandant, für den der Mitarbeiter tätig ist; B: Erfassung von Dokumenten einschränken; C: Passwort; D: Mitarbeiter sperren; E: Mitarbeitergruppe; F: Sprache)*
5.  Markieren Sie die Checkbox (B), wenn der Mitarbeiter nur die Dokumente eines bestimmten Mandanten erfassen darf.
    Die Kombobox (A) zur Auswahl des Mandanten wird freigeschaltet. Wenn Sie die Checkbox nicht markieren, darf der Mitarbeiter für alle Mandanten Dokumente erfassen.
6.  Wählen Sie ggf. den Mandanten aus.
7.  Geben Sie das Passwort (C) ein, mit dem der Mitarbeiter sich identifizieren muss.
    Dieses Passwort kann der Mitarbeiter bei der Anmeldung in A+W Business ändern.
8.  Wählen Sie die Gruppe (E) aus, zu der der Mitarbeiter gehören soll.
    Mit der Zuordnung der Gruppe erhält der Mitarbeiter alle Rechte dieser Gruppe. Diese können Sie im Einzelnen modifizieren.
    ⇨ Tutorial 1, "So bearbeiten Sie die Rechte eines Mitarbeiters" auf Seite B-407
9.  Wählen Sie die Sprache (F) aus.
    Mit dieser Einstellung wird nur die Sprache des Hauptmenüs festgelegt.
10. Wählen Sie den Drucker und das Fax-Gerät aus.
    Damit haben Sie die notwendigen Daten angelegt. Wenn Sie jetzt speichern, kann der Klarname nicht mehr geändert werden. Sie können die Daten des Mitarbeiters jedoch sofort vollständig löschen. Nachdem er sich in A+W Business angemeldet hat, kann er nicht mehr gelöscht werden.
11. Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert. Das Register **Einstellungen** wird freigeschaltet. Sie können jetzt weitere Daten ergänzen und die Mitarbeiterrechte anpassen.

#### ■ So kopieren Sie Standard-Einstellungen für die Dokumente

1.  Wählen Sie im Register **Mitarbeiter** den Benutzer aus, dessen Einstellungen Sie kopieren wollen.
2.  Wechseln Sie zum Register **Einstellungen**.
    *Abbildung B-245: Benutzereinstellungen kopieren*
    *(A: Quelle; B: Einstellung kopieren; C: Ziel-Mitarbeiter; D: Liste der Mitarbeiter)*
    ⇨ Softwarereferenz, "Mitarbeiter – Einstellungen" auf Seite B-1026
3.  Wählen Sie in der Kombobox **Ziel** (C) den neuen Mitarbeiter aus.
4.  Klicken Sie auf **[Benutzereinstellungen]** (B), um die Einstellungen zu kopieren.
    Eine Sicherheitsabfrage wird angezeigt, in der Sie die Quelle und das Ziel nochmals prüfen können und bestätigen müssen. Danach werden die Einstellungen übertragen.
    Sie können diese Einstellungen jetzt weiter anpassen.
5.  Markieren Sie den neuen Mitarbeiter in der Liste (D).
    *Abbildung B-246: Benutzereinstellungen anpassen*
    *(A: Übernommene Einstellung; B: Einstellungen anpassen.)*
    Die Einstellung für die Dokumentenart **Bestellung** (A) wurde übernommen. Beachten Sie, dass Sie die Einstellungen in den einzelnen Spalten nur anpassen können, wenn in der Spalte **Allgemein** der Eintrag `<deaktiviert>` steht.
6.  Wählen Sie für die anderen Dokumentenarten und für die AV-Bereiche (B) Standardeinstellung aus.
    Wenn Sie in eine Zelle klicken, können Sie die gewünschten Daten in der Kombobox auswählen.
7.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.

> **i Daten löschen**
> Wenn der Mitarbeiter sich noch nicht im Programm angemeldet hat, können Sie seine Daten wieder löschen. Dazu müssen Sie Ihr Passwort eintragen, mit dem Sie im Programm angemeldet sind.
> Wenn Sie bereits Rechte zugeteilt hatten, dann müssen Sie diese zuerst löschen.

### Passwort ändern

Das Passwort für die Anmeldung in A+W Business kann vom jeweiligen Mitarbeiter geändert werden.

#### ■ So ändern Sie Ihr Passwort

1.  Klicken Sie auf das Icon, mit dem Sie A+W Business starten.
2.  Markieren Sie die Checkbox **Passwort ändern**.
3.  Tragen Sie Ihr altes Passwort und Ihr neues Passwort in die zugehörigen Felder ein.
4.  Tragen Sie das neue Passwort nochmals in das Feld **Bestätigung** ein.
5.  Klicken Sie auf [OK], um die Daten zu speichern.
    Das Passwort wird geändert und A+W Business wird gestartet. Beim nächsten Start von A+W Business müssen Sie die Markierung der Checkbox **Passwort ändern** zurücksetzen.

### Mitarbeiter sperren

Mitarbeiterdaten können nicht gelöscht werden, nachdem der Mitarbeiter mit A+W Business gearbeitet hat. Sie können ihn für den Zugriff auf A+W Business sperren.

> **i Voraussetzung**
> Sie können Mitarbeiter nur sperren, wenn Sie die Rechte des Systemadministrators haben.

#### ■ So sperren Sie einen Mitarbeiter

1.  Wählen Sie im Menü **Stammdaten > Firma > Mitarbeiter**.
    Der Dialog **Mitarbeiter** wird geöffnet.
2.  Wechseln Sie zum Register **Mitarbeiter** und markieren Sie den Mitarbeiter, den Sie sperren möchten.
3.  Wechseln Sie zum Register **Spezifikation**.
    *Abbildung B-247: Mitarbeiter sperren*
    *(Die Abbildung zeigt die Checkbox "gesperrt" (A) im Spezifikationsregister des Mitarbeiters.)*
    ⇨ Softwarereferenz, "Mitarbeiter - Spezifikation" auf Seite B-1024
4.  Markieren Sie die Checkbox **gesperrt** (A).
    Der Mitarbeiter kann nun nicht mehr mit A+W Business arbeiten und in den Komboboxen der Dialoge nicht mehr ausgewählt werden.
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.

### Mitarbeiterrechte bearbeiten

In der Regel erhält ein Mitarbeiter die Rechte der Mitarbeitergruppe, der er zugeordnet ist. Diese Rechte können Sie ausdehnen oder einschränken. Wenn der Mitarbeiter einer anderen Gruppe zugeordnet wird, erhält er automatisch die Rechte dieser Gruppe. Sie können die Rechte ergänzen, indem Sie die Rechte einer anderen Gruppe kopieren, so dass der Mitarbeiter die Rechte beider Gruppen hat.

> **i Voraussetzung**
> Mitarbeiterrechte werden für eine Gruppe oder für einen einzelnen Mitarbeiter eingerichtet. Sowohl die Gruppe als auch der Mitarbeiter müssen bereits angelegt sein, damit die Rechte zugeteilt werden können.
> Sie können Mitarbeiterrechte nur festlegen, wenn Sie die Rechte des Systemadministrators haben.

Zu diesem Thema gibt es folgende Handlungsanleitungen:

*   "So ergänzen Sie die Mitarbeiterrechte durch Kopieren" auf Seite B-405
*   "So schränken Sie die Rechte eines Mitarbeiters ein" auf Seite B-409

In den folgenden Handlungsschritten wird der Weg über die Kopierfunktion gezeigt, mit der die Rechte schneller und leichter eingerichtet werden.

#### ■ So ergänzen Sie die Mitarbeiterrechte durch Kopieren

1.  Wählen Sie im Menü **Stammdaten > Firma > Mitarbeiterrechte**.
    *Abbildung B-248: Mitarbeiterrechte festlegen*
    ⇨ Softwarereferenz, "Mitarbeiterrechte" auf Seite B-1029
2.  Wählen Sie im Menü **Funktionen > Rechte kopieren**.
    *Abbildung B-249: Mitarbeiterrechte kopieren*
    *(A: Quelle festlegen; B: Ziel festlegen; C: Vorhandene Rechte löschen oder beibehalten)*
3.  Wählen Sie im Bereich **Quelle** die Gruppe (A) aus.
    In diesem Beispiel sollen die Rechte einer Gruppe auf einen Mitarbeiter übertragen werden.
4.  Wählen Sie im Bereich **Ziel** den Mitarbeiter (B) aus.
5.  Entscheiden Sie, ob die vorhanden Rechte (C) gelöscht oder beibehalten werden sollen:
    *   Wenn Sie die Checkbox markieren, werden alle Rechte des Ziels gelöscht und die der Quelle übertragen.
    *   Wenn Sie die Checkbox nicht markieren, werden nur die Rechte übertragen, die noch nicht zugeteilt waren.
    In diesem Beispiel werden die vorhandenen Rechte durch die neuen ergänzt: Die Checkbox wird nicht markiert.
6.  Klicken Sie auf [OK], um die Kopierfunktion zu starten.
    Wenn der Vorgang beendet ist, wird in einer Meldung die Anzahl der übertragenen Rechte angezeigt.
7.  Bestätigen Sie die Meldung und schließen Sie den Dialog **Rechte kopieren**.
    *Abbildung B-250: Kopierte Rechte*
    Die Rechte der neuen Gruppe oder des neuen Mitarbeiters werden im Dialog **Rechteverwaltung** im Bereich **Übersicht** aufgelistet. Sie können die einzelnen Rechte jetzt bearbeiten.

#### ■ So bearbeiten Sie die Rechte eines Mitarbeiters

1.  Wählen Sie im Menü **Stammdaten > Firma > Mitarbeiterrechte**.
    Der Dialog **Rechteverwaltung** wird geöffnet.
2.  Markieren Sie die Option **Mitarbeiter** und wählen Sie den Mitarbeiter aus.
    In der Übersicht werden die Gruppe und der Mitarbeiter angezeigt.
    *Abbildung B-251: Zugeteilte Rechte bearbeiten*
    *(A: Mitarbeiter; B: Rechte zuteilen oder entziehen; C: Liste öffnen)*
3.  Öffnen Sie die Liste der vorhandenen Rechte mit einem Klick auf [+].
    In der Übersicht werden alle Rechte angezeigt, die dem Mitarbeiter oder der Mitarbeitergruppe zugeordnet sind. Für alle Programmpunkte oder Dialoge, die nicht aufgeführt sind, gelten uneingeschränkte Rechte.
4.  Markieren Sie den Programmpunkt, zu dem Sie die Rechte ändern wollen.
    Die Rechte werden in den Checkboxen (B) angezeigt.
5.  Markieren Sie im Bereich **Rechte** die Checkboxen (B) so, wie das Recht eingeschränkt werden soll:
    *   **Ändern:** Daten dürfen bearbeitet werden.
    *   **Einfügen:** Neue Datensätze dürfen angelegt werden.
    *   **Löschen:** Datensätze dürfen gelöscht werden.
    *   **Ausführen/Lesen:** Der Dialog darf geöffnet werden.
    Beachten Sie, dass Sie das entsprechende Recht entziehen, wenn Sie eine Checkbox nicht markieren. Wenn Sie z. B. die Checkbox **Ausführen** markieren, kann der Mitarbeiter den entsprechenden Dialog öffnen, aber nicht bearbeiten.
6.  Wählen Sie im Menü **Start > Speichern**, um die Änderungen zu speichern.
    Die neuen Rechte werden für den Mitarbeiter gespeichert und gelten, wenn er sich das nächste Mal in A+W Business anmeldet.

#### ■ So schränken Sie die Rechte eines Mitarbeiters ein

1.  Wählen Sie im Menü **Stammdaten > Firma > Mitarbeiterrechte**.
    Der Dialog **Rechteverwaltung** wird geöffnet.
    In den folgenden Handlungsschritten wird der Zugriff auf einen zusätzlichen Programmpunkt für einen Mitarbeiter eingeschränkt.
2.  Wählen Sie im Menü **Bearbeiten > Neu**.
    *Abbildung B-252: Felder für Rechtevergabe freigeschaltet*
    *(A: Mitarbeiter; B: Programm (Dialog))*
3.  Wählen Sie den Mitarbeiter (A) aus, dessen Rechte Sie einschränken wollen.
4.  Wählen Sie das Programm (B) aus, für das Sie die Rechte einschränken möchten, z. B. **Crystal Reports-Ausgabe**.
5.  Markieren Sie im Bereich **Rechte** die Checkboxen so, wie das Recht eingeschränkt werden soll.
    Beachten Sie, dass Sie das entsprechende Recht entziehen, wenn Sie eine Checkbox nicht markieren. Wenn Sie z. B. die Checkbox **Ausführen** markieren, kann der Mitarbeiter den entsprechenden Dialog öffnen, aber nicht bearbeiten.
    In diesem Beispiel soll der Mitarbeiter den Dialog nicht öffnen können. Daher darf keine Checkbox markiert sein.
6.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    *Abbildung B-253: Zusätzliche Rechtevergabe für den Mitarbeiter*
    Die Daten werden gespeichert. Der Mitarbeiter wird im Bereich **Übersicht** aufgeführt. In diesem Beispiel ist keine Checkbox markiert. Das bedeutet, dass der Mitarbeiter diesen Dialog nicht mehr öffnen kann.
7.  Wählen Sie den Mitarbeiter erneut aus, um seine gesamten Rechte zu prüfen.
    *Abbildung B-254: Rechte des Mitarbeiters*
    In diesem Beispiel ist der Eintrag **Crystal Reports-Ausgabe** das Recht, das zusätzlich zu den Rechten der Gruppe eingerichtet wurde.

#### ■ So löschen Sie die Rechte eines Mitarbeiters

1.  Wählen Sie im Menü **Stammdaten > Firma > Mitarbeiterrechte**.
    Der Dialog **Rechteverwaltung** wird geöffnet.
2.  Wählen Sie den Mitarbeiter aus, dessen Rechte Sie löschen wollen.
3.  Markieren Sie das Recht, das Sie löschen wollen.
4.  Wählen Sie im Menü **Start > Löschen** und bestätigen Sie die Abfrage mit [Ja].
    Das markierte Recht wird aus der Liste gelöscht. In der Übersicht werden alle Rechte angezeigt, die dem Mitarbeiter zugeordnet sind. Für alle Programmpunkte oder Dialoge, die nicht aufgeführt sind, gelten uneingeschränkte Rechte.

> **i Alle Rechte löschen**
> Wenn Sie alle Rechte löschen wollen, wählen Sie im Menü **Funktionen > Rechte löschen**. Sämtliche Rechte des Mitarbeiters werden damit gelöscht. Einen neuen Mitarbeiter, der sich noch nicht im System angemeldet hatte, können Sie nun ebenfalls löschen.

### Übungen

*   Legen Sie einen (Schulungs-)Mandanten an.
*   Weisen Sie einem Mitarbeiter einen AD-Bereich zu. Wählen Sie für diese Übung sich selbst als Vertreter aus.
*   Legen Sie zu diesem Vertreter eine gestaffelte Provision an, die sich auf die Umsätze Ihres Schulungskunden und Schulungsprodukte bezieht.

Die folgenden Übungen können Sie nur ausführen, wenn Sie Administratorrechte haben. Achten Sie darauf, dass Sie die Übungen für Ihren Schulungsmandanten ausführen.

*   Legen Sie eine Gruppe für Lagermitarbeiter an.
*   Richten Sie die Rechte dieser Gruppe so ein, dass nur die Lagerdialoge zur Verfügung stehen.
*   Legen Sie einen neuen Mitarbeiter an, z. B. einen Werkstudenten für die Lagerverwaltung.
*   Ordnen Sie ihm die Rechte zu, die in der Gruppe der Lagermitarbeiter zusammengefasst sind.
*   Entziehen Sie ihm das Recht, zum Erfassen von Lagerbestellungen und zum Erstellen der Inventurliste.
*   Melden Sie sich mit seinen Zugangsdaten an und prüfen Sie in der Lagerverwaltung, ob die Rechte korrekt vergeben sind.

### Ergänzende Informationen

*   ⇨ Softwarereferenz, "Firmendaten" auf Seite B-930
*   ⇨ Softwarereferenz, “AD-Bereiche" auf Seite B-1034
*   ⇨ Softwarereferenz, "Vertreterprovision" auf Seite B-1036
*   ⇨ Softwarereferenz, "Banken" auf Seite B-1039
*   ⇨ Softwarereferenz, "Filialen" auf Seite B-1041
*   ⇨ Softwarereferenz, "Mitarbeiter" auf Seite B-1022
*   ⇨ Softwarereferenz, "Mitarbeitergruppen" auf Seite B-1028
*   ⇨ Softwarereferenz, "Mitarbeiterrechte" auf Seite B-1029

# Tutorial 2: Dokumente

Dokumente bilden die Grundlage der kaufmännischen Abläufe in A+W Business. In diesem Themenblock lernen Sie, wie Sie neue oder bearbeitete Stammdaten testen können und wie die Verarbeitung der Dokumente in A+W Business gesteuert wird.

Dazu gehören folgende Lerneinheiten:

*   "Auftrag für Stammdatentest" auf Seite B-416
*   "Statusverwaltung" auf Seite B-426
*   "Nummernkreise" auf Seite B-440
*   "Rundungen" auf Seite B-449

> **i Voraussetzung**
> In diesem Tutorial werden die Kenntnisse aus dem Tutorial 1 vorausgesetzt.

## Auftrag für Stammdatentest

### Lernziele

*   Zusammenspiel der Stammdaten prüfen.
*   Auftrag erfassen.
*   Nummernverwalter anlegen.

### Nutzen

*   Sie können die neuen oder geänderten Stammdaten testen, bevor sie im Tagesgeschäft eingesetzt werden.

### Merke

*   **Auftrag**: Ein Auftrag (Dokument) wird immer in einen Nummernverwalter gestellt.
*   **Nummernverwalter**: Nummernverwalter (NV) dienen zur Organisation der Abläufe im Tagesgeschäft. Ein NV kann nicht leer sein.
*   **Hierarchie der Konditionen**: Bei der Berechnung von Aufträgen (oder Bestellungen) werden die Konditionen in folgender Reihenfolge berücksichtig:
    *   Angaben aus dem Dokument
    *   Definitionen aus den Stammdaten
    *   Gruppenspezifische Konditionen

### Zusammenspiel der Stammdaten im Auftrag

Die Daten für Marktpartner, Produkte, Preise, Zuschläge und Rabatte haben Sie angelegt oder bearbeitet. Diese Daten laufen in den Dokumenten zusammen und bilden die Grundlage, auf der Aufträge und Bestellungen erfasst werden.

*Abbildung B-255: Zusammenwirken der Stammdaten im Auftrag*
*(Das Diagramm zeigt, wie Stammdaten (Tour, Rabatte, Kundengruppe für einen Kunden und Produktart, Produktgruppe, Preis für ein Produkt) in einem Dokument (Auftrag) zusammenfließen.)*

In dieser vereinfachten Übersicht sehen Sie, dass ein Auftrag für einen Kunden erfasst wird, der ein bestimmtes Produkt bestellt. Zusammen mit den Stammdaten des Kunden und des Produkts werden weitere Stammdaten herangezogen, die z. B. den Preis bestimmen.

Bevor Sie die neuen Daten im Tagesgeschäft einsetzen, müssen Sie prüfen, ob die Ergebnisse der Preis- und Terminberechnung Ihren Erwartungen entsprechen. In den folgenden Einheiten wird kurz beschrieben, wie die Daten im Dialog **Dokumentenverwaltung** erfasst werden.

Eine vollständige Beschreibung der Auftragserfassung finden Sie im Part **Verkauf**.

### Kopfdaten des Auftrags

Die Kopfdaten sind auftragsweit gültige Daten. Sie stellen die Auftragsteile dar, die pro Kunde nie oder selten geändert werden, z. B. Kundennummer, Rechnungsanschrift, Konditionen. Außerdem werden Daten über Gesamtsummen pro Auftrag dargestellt.

*Abbildung B-256: Dialog Dokumentenverwaltung*
*(A: Dokumentenart und Nummer des aktuellen Dokuments; B: Register für Kopfdaten; C: Aktueller Nummernverwalter; D: Status (Anzeige in Tabelleneigenschaften aktiviert); E: Register für Positionsdaten)*

In dieser kurzen Übersicht sehen Sie einen Auftrag mit den Kopfdaten für den Kunden und den Versanddaten. Das Register **Positionen** wird erst freigeschaltet, wenn die Kopfdaten gespeichert sind.

### Positionsdaten

Die Positionsdaten bilden den variablen Teil eines Dokuments. Sie enthalten neben den Produkten, Preisen, Größen und Mengen auch Informationen für die Produktion und den Einkauf (Bestellung).

*Abbildung B-257: Dialog zur Positionserfassung*
*(A: Titelzeile: Auftragsnummer, Anzahl der Positionen, Gesamtpreis; B: Positionen; C: Positionspreise (rote Schrift für manuelle Eingaben); D: Stückpreis; E: Details zur Stückliste)*

In dieser Übersicht sehen Sie, wie Auftragspositionen angezeigt werden. Zu jeder Position werden die Preise und Rabatte angezeigt, die aus den Stammdaten herangezogen werden.

Eine ausführliche Beschreibung der Dokumente finden Sie im Part **Verkauf**.
⇨ Verkauf, "Kompletterfassung von Dokumenten bis Faktura" auf Seite C-26

### Nummernverwalter für Aufträge

Aufträge werden in Nummernverwaltern (NV) organisiert, so dass sie gemeinsam weiterverarbeitet werden können. Jedes Dokument wird automatisch einem Nummernverwalter zugeordnet. Mit den Nummernverwaltern können Sie Arbeitsabläufe im Verkauf automatisieren, z. B. Auftragsbestätigungen und Lieferscheine drucken.

*Abbildung B-258: Nummernverwalter*
*(A: Aktueller NV; B: Liste der Dokumente im NV)*

Nummernverwalter können nicht leer sein. Zur Prüfung der Stammdaten müssen Sie also zunächst einen Auftrag erfassen. Diesen können Sie anschließend in einen neuen Nummernverwalter stellen.

Die Funktionen der Nummernverwalter sind ausführlich im Part **Verkauf** beschrieben.
⇨ Verkauf, "Nummernverwalter" auf Seite C-186

### Auftrag erfassen

In der folgenden Anleitung wird ein neuer Auftrag erfasst, in dem keine Felder aus einem vorherigen Auftrag vorbelegt sind.

Das Arbeiten mit Dokumenten ist ausführlich im Part **Verkauf** beschrieben. An dieser Stelle werden die Handlungsschritte daher nur verkürzt wiedergegeben.

⇨ Verkauf, "Auftragskopf erfassen" auf Seite C-50
⇨ Verkauf, "Auftragsposition erfassen" auf Seite C-97

#### ■ So erfassen Sie einen Auftrag

1.  Wählen Sie im Menü **Dokumente > Auftrag > Auftrag**.
    Der Dialog **Dokumentenverwaltung** wird geöffnet. Leeren Sie ggf. die Vorbelegung, indem Sie auf [Auswahl] klicken.
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    *Abbildung B-259: Felder für neuen Auftrag freigeschaltet*
    *(A: Titelzeile; B: Eingabefeld Kundennummer; C: Register Positionen)*
    ⇨ Softwarereferenz, "Partnerverwaltung" auf Seite B-770
3.  Geben Sie die Nummer (B) Ihres (Schulungs-)Kunden ein.
    Wenn Sie die Kundennummer nicht wissen, können Sie über die Lupe nach dem Kunden suchen.
4.  Springen Sie mit `<Tab>` in das nächste Feld.
    Die Kundendaten werden eingelesen.
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Kopfdaten werden gespeichert. In der Titelzeile (A) wird die Auftragsnummer angezeigt und das Register **Positionen** wird freigeschaltet.
6.  Klicken Sie auf das Register **Positionen** (C).
    *Abbildung B-260: Felder für neue Position freigeschaltet*
    *(A: Produktnummer eingeben; B: Produkt suchen; C: Anzahl; D: Breite; E: Höhe)*
    Das Eingabefeld (A) für die Produktnummer ist freigeschaltet. Nur wenn Sie Eingaben oder Änderungen zwischendurch gespeichert haben, müssen Sie den Erfassungsmodus im Menü **Bearbeiten > Neu** starten, um eine neue Position zu erfassen.
7.  Tragen Sie in der Erfassungszeile die Nummer (A) Ihres (Schulungs-)Produkts ein.
    Wenn Sie die Produktnummer nicht wissen, können Sie das gewünschte Produkt auch über **Produktsuche** (B) auswählen.
8.  Springen Sie mit `<Tab>` ins nächste Feld.
    Alle Eingabefelder werden freigeschaltet.
9.  Geben Sie in den nächsten Feldern die Stückzahl (C) und die Maße (D, E) ein.
    Wenn Sie nur 1 Stück und die Maße 1000 x 1000 eintragen, können Sie einfacher prüfen, ob die Preise korrekt angezeigt werden.
    *Abbildung B-261: Anzeige von Preisen*
    *(A: Preisjahrgang; B: Preisschlüssel; C: Preiseinheit; D: Positionspreis)*
10. Prüfen Sie, ob der Tarif (Preisschlüssel (B), Preisjahrgang (A)) und die Preiseinheit (C) korrekt angezeigt werden.
    Wenn zu Ihrem Produkt und Kunden keine Zuschläge und Rabatte berechnet werden, dann muss der Positionspreis (D) korrekt berechnet sein. In diesem Beispiel sind das 71,38 €/qm x 1,04 qm (Maßrundung). Wenn Zuschläge und Rabatte zugeordnet sind, können Sie den Positionspreis entsprechend berechnen.
11. Speichern Sie die Position mit `<Enter>`.
    Die Positionsdaten werden gespeichert und in der nächsten Zeile als neue Position vorgeschlagen. Sie können diese Daten zum Erfassen einer weiteren Position überschreiben oder ignorieren, wenn Sie keine weitere Position erfassen möchten.
    Notieren Sie sich die Auftragsnummer, um anschließend einen Nummernverwalter für diesen Auftrag zu erstellen.
12. Schließen Sie die Positionserfassung und danach den Auftrag.
    Erstellen Sie nun einen Nummernverwalter, in dem Sie alle Aufträge sammeln, die Sie zu Testzwecken erfassen.

### Nummernverwalter

Für den Test der Stammdaten sollten Sie sich einen eigenen Nummernverwalter (NV) anlegen. An dieser Stelle werden die Handlungsschritte nur verkürzt wiedergegeben. Das Arbeiten mit Nummernverwaltern ist ausführlich im Part **Verkauf** beschrieben.

⇨ Verkauf, "Nummernverwalter" auf Seite C-186

#### ■ So erstellen Sie einen neuen Nummernverwalter

1.  Wählen Sie im Menü **Dokumente > Auftrag > NV Auftrag**.
    Der Dialog **Nummernverwalter** wird geöffnet. In der Übersicht werden alle Dokumente angezeigt, die sich im aktiven Nummernverwalter befinden.
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    *Abbildung B-262: Felder für neuen Nummernverwalter freigeschaltet*
    *(A: Name des Nummernverwalters; B: Nummer des Auftrags)*
3.  Tragen Sie den Namen (A) für den neuen Nummernverwalter ein, z. B. **Schulung**.
4.  Tragen Sie die Nummer Ihres Testauftrags in beiden Feldern (B) ein.
    Wenn Sie die Nummer nicht wissen, können Sie nach dem Auftrag suchen, indem Sie die Auswahl auf den Status 1 einschränken. In diesem Fall werden zwar alle Aufträge mit dem Status 1 in den Nummernverwalter geladen. Sie können jedoch die nicht gewünschten aus dem NV löschen, indem Sie diese markieren und auf `<Entf>` drücken.
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert. Der neue Nummernverwalter wird im Feld **Auswahl** angezeigt.
    *Abbildung B-263: Neuer Nummernverwalter*
    Der zugewiesene Auftrag wird in der Übersicht aufgeführt.

### Übungen

*   Legen Sie unterschiedliche Aufträge zu Ihrem Schulungskunden an und erfassen Sie darin Ihre Schulungsprodukte.
    Wählen Sie jeweils nur ein Stück und die Maße 1000 x 1000 mm, damit Sie die Berechnung des Positionspreises einfacher prüfen können.
*   Prüfen Sie folgende Daten:
    *   Sind Zuschläge und Rabatte berechnet.
    *   Wird die Kalkulation des Deckungsbeitrags und der Kosten angezeigt.
    *   Sind die Tour und das Lieferdatum korrekt.

## Statusverwaltung

### Lernziele

*   Funktion des Status kennenlernen.
*   Unterschied zwischen Statuspunkt und Anwenderstatus kennenlernen.
*   Statuszuordnung prüfen.
*   Statusumsetzung, Sperrstatus und Statusumleitung einrichten.

### Nutzen

*   Mit der Statuszuordnung werden die Geschäftsabläufe im Betrieb abgebildet.
*   Über die Statuszuordnungen wird gesteuert, wie ein Dokument nach der Erfassung weiter bearbeitet werden kann.

### Merke

*   **Statuspunkt**: Signalisiert das Ende eines Prozesses. Die Statuspunkte sind fest codiert und können nicht geändert werden.
*   **Anwenderstatus**: Stand der Bearbeitung, den ein Dokument in Ihrem Unternehmen erreicht hat. Die Nummern und Bezeichnungen werden bei der Installation für Ihr Unternehmen eingerichtet.
*   **Statuszuordnung**: Jeder Anwenderstatus muss einem Statuspunkt zugeordnet werden. Wenn eine Zuordnung fehlt, können bestimmte Funktionen nicht ausgeführt werden.
*   **Status**: Nummer, die kennzeichnet, an welcher Stelle im Programmablauf ein Dokument steht. Jeder Status ist eindeutig. Jedes Dokument wird mit einem Status gekennzeichnet.
*   **Statusumsetzung**: Am Ende eines Programmprozesses wird der Status automatisch umgesetzt. Der Status wird dabei immer erhöht. Mit besonderen Mitarbeiterrechten kann der Status manuell zurückgesetzt werden.
*   **Dokumententyp**: Nicht jeder Status kann auf jedes Dokument angewendet werden, z. B. durchlaufen alle Dokumente den Status **Dokument erfasst**, aber ein Angebot kann den Status **Lieferschein gedruckt** nicht erreichen.
*   **Manueller Statuspunkt**: Ein manueller Statuspunkt kann nur manuell vergeben werden. Er setzt das automatische Hochsetzen des Status außer Kraft.

### Geschäftsabläufe abbilden

Ihre Geschäftsabläufe bestimmen, welche Stationen ein Auftrag von der Erfassung bis zur Archivierung durchläuft.

> **Beispiel**
> *   Auftrag wird erfasst.
> *   Auftrag wird geändert.
> *   Auftragsbestätigung wird gedruckt.
> *   Aufträge werden an die Kapazitätsplanung übergeben (optional).
> *   Aufträge werden an die Produktion übergeben.
> *   Rückmeldung des Fertigungsstands.
> *   Lieferschein wird gedruckt.
> *   Rechnung wird gedruckt.
> *   Auftrag wird an die FiBu übergeben.
> *   Auftrag wird an Statistik und Archiv übergeben.
> *   Auftragsdaten werden aus der Hauptdatenbank gelöscht.

Der Auftrag durchläuft von der Erfassung bis zur Archivierung definierte Programmpunkte, die Statuspunkte. Diesen Statuspunkten können Sie die Stationen zuordnen, die der Auftrag in Ihrem Unternehmen durchläuft. Dabei legen Sie als Mindeststatus fest, welche Voraussetzungen erfüllt sein müssen, damit der Auftrag weitergeleitet werden kann. Sie können auch festlegen, wann ein Auftrag für bestimmte Vorgänge gesperrt wird.

Diese Zusammenhänge definieren Sie in den Dialogen **Statusverwaltung**, **Statuspunkte** und **Statuszuordnung**.

> **i Bearbeitung in den Dialogen**
> In den Dialogen **Statusverwaltung** und **Statuspunkte** brauchen Sie nichts zu bearbeiten. Lediglich die **Statuszuordnung** müssen Sie bearbeiten können, wenn sich z. B. die Geschäftsabläufe ändern.

### Statuspunkt (Prozessname und -nummer)

Für die automatische Verarbeitung von Dokumenten sind im Programm sogenannte Statuspunkte definiert. Sie signalisieren das Ende verschiedener interner Prozesse, die ein Dokument von der Erfassung bis zum Rechnungsdruck, einschließlich von Reklamation oder Gutschrift, durchläuft.

*Abbildung B-264: Statuspunkte*
*(A: Internes Kennzeichen (ID des Statuspunkts); B: Dokumententyp; C: Abgeschlossener Prozess)*

Die Statuspunkte sind fest im System verankert und werden genutzt, um Bedingungen für die weitere Bearbeitung zu definieren, z. B. für den Druck einer Rechnung. Jedem Statuspunkt kann pro Dokumententyp (B) ein Anwenderstatus zugeordnet werden.

Der Anwenderstatus zeigt den Stand der Bearbeitung an, den ein Dokument in Ihrem Unternehmen erreicht hat. Dieser Zusammenhang wird im Folgenden beschrieben.

⇨ "Statusverwaltung" auf Seite B-429
⇨ "Statuszuordnung" auf Seite B-430

Nicht jeder Status kann auf jedes Dokument angewendet werden, z. B. durchlaufen alle Dokumente den Status **Dokument erfasst**, aber ein Angebot kann den Status **Lieferschein gedruckt** nicht erreichen.

Folgende Dokumententypen stehen zur Verfügung:

*   0 = alle Dokumente
*   1 = Angebote
*   2 = Auftrag
*   3 = Gutschrift
*   4 = Bestellanfrage
*   5 = Bestellung

### Statusverwaltung

Der sogenannte Anwenderstatus kennzeichnet den Stand der Bearbeitung eines Dokumentes innerhalb des Ablaufs in Ihrem Unternehmen.

*Abbildung B-265: Statusverwaltung (Anwenderstatus)*
*(A: Status: Kennzeichen in den Dokumenten; B: Bezeichnung (im Geschäftsablauf))*

Der Status zeigt an, wo das Dokument sich im Geschäftsablauf befindet. Er wird als Nummer und mit der zugehörigen Bezeichnung angezeigt, z. B. in der Auftragserfassung oder in der Historie.

> **i Anwenderstatus ändern**
> Bevor Sie einen Anwenderstatus nach Ihren Vorstellungen ändern bzw. anlegen, sprechen Sie dies bitte mit der A+W Software GmbH ab. Sie vermeiden damit, dass das System u. U. nicht mehr richtig arbeitet.

### Statuszuordnung

Sie können jedem Statuspunkt Ihren eigenen Anwenderstatus zuordnen. Die Nummerierung der Statuspunkte hat nichts mit der Reihenfolge des Firmenablaufs zu tun.

*Abbildung B-266: Zuordnung: Statuspunkt – Anwenderstatus*
*(A: Statuspunkte; B: Markierter Statuspunkt; C: Dokumententyp, für den die Zuordnung gilt; D: Zugeordneter Anwenderstatus; E: Mindeststatus, den das Dokument erreicht haben muss; F: Sperrstatus)*

In diesem Beispiel ist dem Statuspunkt **Rechnung Druck** (B) der Anwenderstatus **Rechnung gedruckt** (D) zugeordnet. Die Zuordnung gilt für den Dokumententyp **Auftrag** (C). Das bedeutet, dass der Status eines Auftrags nach dem Rechnungsdruck mit der Statusnummer und -bezeichnung des Anwenderstatus angezeigt wird.

#### Mindeststatus

Bei jeder Zuordnung können Sie angeben, welche Voraussetzung das Dokument erfüllen muss, um den angegebenen Anwenderstatus zu erreichen. In diesem Beispiel ist als Mindeststatus (E) der Druck des Lieferscheins angegeben. Das bedeutet, dass die Rechnung nicht vor dem Lieferschein gedruckt werden kann.
