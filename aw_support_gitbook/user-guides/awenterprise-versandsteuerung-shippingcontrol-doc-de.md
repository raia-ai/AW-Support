---
title: "DE_AWEnterprise_Versandsteuerung_HelpCards"
source: "DE_AWEnterprise_Versandsteuerung_HelpCards.pdf"
tags: ["A+W Enterprise", "Versandsteuerung", "Shipping Control", "ERP", "Software Guide", "Help Cards", "Logistics", "Tour Planning"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A collection of \"Help Cards\" providing step-by-step instructions for the \"Versandsteuerung\" (Shipping Control) module of the A+W Enterprise software. It covers tasks like managing tours, orders, and items, preparing shipments, and using various system functions."
long_description: "This document serves as a user guide in the form of \"Help Cards\" for the \"Versandsteuerung\" (Shipping Control) module within the A+W Enterprise 6 software, a system designed for the glass, windows, and doors industry. It provides concise, task-oriented instructions for logistics and shipping personnel. The guide details workflows for key shipping operations, distinguishing between different operational modes like with or without the \"Versand-Explorer\" (Shipping Explorer). Core topics include editing tours (rescheduling or rerouting), managing orders and positions (moving items to different dates or routes), and preparing shipments (checking for shortfalls, correcting packaged quantities, changing delivery addresses, and creating delivery notes). It also covers advanced functions such as managing the loading sequence, canceling processes, and visualizing tour capacity. Each help card clearly outlines the objective, prerequisites, additional information, and a step-by-step workflow for a specific task."
---

# A+W Versandsteuerung Help Cards

---
## Versandsteuerung

Die Darstellungen in den Help Cards basieren auf der Auslieferversion **A+W Enterprise 6**. Einzelne Schritte in den Workflows können je nach Konfiguration abweichen, z. B. das Arbeiten mit oder ohne Versand-Explorer (VS-Explorer).

**Zur Unterscheidung:**

*   **Die Route** ist eine festgelegte Fahrstrecke, die an bestimmten Tagen befahren wird, z. B. die Route 300 von Frankfurt nach München wird jeweils montags und donnerstags gefahren.
*   **Die Tour** ist die zu fahrende Strecke an einem bestimmten Liefertermin, z. B. die Tour auf der Route 300 liefert die Kundenaufträge am Donnerstag, dem 28.04.16 aus.

### Versand-Explorer

| Help Card | Themen |
| :--- | :--- |
| **Arbeiten ohne VS-Explorer** | - Lieferung(en) zu einem Datum suchen.<br>- Positionen zum Auftrag einsehen. |
| **Arbeiten mit VS-Explorer** | - Touren zu einem Datum suchen.<br>- Lieferung zu einem Datum suchen.<br>- Positionen zum Auftrag einsehen. |

### Tour bearbeiten

| Help Card | Themen |
| :--- | :--- |
| **Tour verschieben** | - Tour auf ein anderes Lieferdatum verschieben.<br>- Tour auf eine andere Route verschieben. |
| **Auftrag verschieben** | - Auftrag auf ein anderes Lieferdatum oder eine andere Route verschieben.<br>- Mehrere Aufträge verschieben. |
| **Position verschieben** | - Position auf ein anderes Lieferdatum verschieben.<br>- Position auf eine andere Route verschieben. |
| **Mehrere Positionen verschieben** | - Alle nicht gelieferten Positionen vom Vortag verschieben.<br>- Mehrere Positionen eines Auftrags auf eine andere Route oder ein anderes Lieferdatum verschieben.<br>- Einzelne Mengen auf ein anderes Lieferdatum verschieben. |
| **Verschieben mit Kontext-Menü** | - Touren, Aufträge oder Positionen im Explorer verschieben. |

## Versand vorbereiten

| Help Card | Themen |
| :--- | :--- |
| **Fehlmenge kontrollieren** | - Produzierte Menge prüfen.<br>- Verfügbare Menge als verpackt buchen.<br>- Fehlende Menge als Rückstand verschieben. |
| **Verpackte Menge korrigieren** | - Verpackte Menge prüfen.<br>- Verpackt gemeldete Menge ändern. |
| **Lieferanschrift ändern** | - Alternative Lieferanschrift auswählen.<br>- Neue Anschrift für Lieferung von Rückständen eingeben. |
| **Lieferschein erstellen** | - Vorab-Lieferschein drucken.<br>- End-Lieferschein erstellen. |
| **Ladefolge bearbeiten** | - Ladefolge ändern.<br>- Ladeliste für eine Tour drucken.<br>- Ladelisten für alle Touren drucken.<br>- Ergänzungsladeliste drucken. |
| **Vorgang stornieren** | Vorgang stornieren:<br>- Auftrag<br>- Lieferschein<br>- Versandstatus |

## Zusatzfunktionen

| Help Card | Themen |
| :--- | :--- |
| **Tourgrafik anzeigen** | - Auslastung der Touren eines Lieferdatums darstellen.<br>- Auslastung einer Tour an aufeinander folgenden Liefertagen darstellen. |
| **Auftragsinfos einsehen** | - Informationen zum Auftrag einsehen.<br>- Informationen des Fertigwarenlagers zum Auftrag einsehen.<br>- Buchungsprotokoll zum Fertigwarenlager einsehen. |

---

## Arbeiten ohne VS-Explorer (VS 01-001)

### Ziel der Handlung
- Lieferung(en) zu einem Datum suchen.
- Positionen zum Auftrag einsehen.

### Voraussetzungen
- Das Arbeiten ohne Versand-Explorer muss im Programm konfiguriert sein.
- Touren sind geplant.

### Zusatzinfo
- **VK-Aus.:** Standard-Modus für die Suche (Verkauf - Ausgang).
- **EK-WEin., EK-WAus.:** Modus für den Einkauf. Muss konfiguriert sein.
- **[Springen]:** Auftragssuche über die Auftrags- oder Kundennummer.
- ⇨ Tour verschieben
- ⇨ Auftrag verschieben
- ⇨ Position verschieben

### Workflow
1.  Menü **Logistik > Versandsteuerung** wählen.
    Dialog `Versandsteuerung` wird geöffnet.
2.  Mindestens die folgenden Suchkriterien eingeben:
    -   **Haus:** Mandant.
    -   **Gruppe:** Versandgruppe.
    -   **Lieferdatum:** Datum, für das die Tour geplant ist.
3.  Suche mit **<Enter>** starten.
    Dialog `Versandsteuerung – TourenInfo` mit der Trefferliste wird geöffnet.
    Von hier aus können alle Aktionen gestartet werden, um die Tourdaten zu bearbeiten.

**Positionen zum Auftrag einsehen:**
4.  Register **AuftragsInfo** öffnen: Doppelklick auf Tour oder **[Aufträge]** oder **<F5>**.
    Alle Aufträge der Tour werden angezeigt.
5.  Register **PositionsInfo** öffnen: Doppelklick auf Auftrag oder **[Positionen]** oder **<F5>**.
    Alle Positionen des Auftrags werden angezeigt.
6.  Register **PositionsInfo II** öffnen: Klick auf **[Maskenvariante]** oder auf Register **PositionsInfo II**.
    Register `PositionsInfo II` wird mit den Maßen zu den Positionen des Auftrags angezeigt.

---

## Arbeiten mit VS-Explorer (VS 01-002)

### Ziel der Handlung
- Touren zu einem Zeitraum suchen.
- Lieferung zu einem Datum einsehen.
- Positionen zum Auftrag einsehen.

### Voraussetzungen
- Das Arbeiten mit Versand-Explorer muss im Programm konfiguriert sein.
- Touren sind geplant.

### Zusatzinfo
Mit **<F4>** erreichen Sie alle wichtigen Befehle zur Versandsteuerung.
- Tour verschieben
- Auftrag verschieben
- Position verschieben

### Workflow
1.  Menü **Logistik > Versandsteuerung** wählen.
    Dialog `Versandsteuerung` wird geöffnet.
2.  Mindestens die folgenden Suchkriterien eingeben:
    -   **Haus:** Mandant.
    -   **Gruppe:** Versandgruppe.
    -   **Lieferdatum:** Anfangs- und Enddatum eintragen für Touren in einem Zeitraum.
3.  Suche mit **<Enter>** starten.
    Alle Tage mit geplanten Touren werden im Versand-Explorer angezeigt.
    In der Detailsicht werden die Touren des markierten Tages angezeigt.
4.  Ebenen aufklappen: Knoten **[+]** am gesuchten Tag öffnen.
5.  Schritt 4 für Tourebene wiederholen.
    Aufträge in der Tour werden in der Detailsicht angezeigt.
6.  Tour in der Explorersicht markieren und **[Details]** wählen.
    Register `TourenInfo` mit den Touren des gewählten Tages wird geöffnet.
    Von hier aus können alle Aktionen gestartet werden, um die Tourdaten zu bearbeiten.
7.  Mit **[Explorer]** zurück in die Explorersicht springen.
    -   Die Schritte 4 bis 7 gelten analog für die Auftrags- und die Positionsebene.

---

## Tour bearbeiten: Tour verschieben (VS 02-001)

### Ziel der Handlung
- Tour auf ein anderes Lieferdatum verschieben.
- Tour auf eine andere Route verschieben.

### Voraussetzungen
- Touren werden in der Versandsteuerung angezeigt.

### Zusatzinfo
Wenn das neue Lieferdatum nicht zur gewählten Route passt, wird die Tour nicht auf das neue Lieferdatum verschoben. Wenn eine Ausweichroute definiert ist, wird die Tour auf diese Route verschoben.
- ⇨ Auftrag verschieben
- ⇨ Position verschieben
- ⇨ Mehrere Positionen verschieben

### Workflow
1.  Register **TourenInfo**: Tour markieren > **[Verschieben]**.
    Dialog `Verschiebung (Versand)` wird geöffnet.
2.  Begründung für die Verschiebung mit **<Leertaste>** wählen und ggf. eine Anmerkung eintragen.
3.  Feld **Auf Tourtag**: Lieferdatum eintragen.
    Wenn das neue Datum kein gültiger Routentag ist, kann die Tour nicht verschoben werden.
    Wenn ein Tourplan erstellt ist: in Feld **Auf Tourtag <F9>** drücken und Tour auswählen.
4.  Verschiebung mit **[Start]** auslösen.
    Die Tour wird komplett auf das neue Lieferdatum verschoben. Im Register `TourenInfo` wird sie nicht mehr angezeigt.
5.  Verschiebung prüfen: Tourensuche mit neuem Lieferdatum starten.

**Tour für das gleiche Datum auf andere Route verschieben:**
6.  Feld **Auf Tourtag**: Lieferdatum prüfen.
7.  Feld **Route**: neue Route eintragen.
    Wenn das Lieferdatum kein Routentag ist, kann die Tour nicht verschoben werden.
8.  Verschiebung mit **[Start]** auslösen.
    Die Tour wird komplett auf die neue Route verschoben.
    Wenn das Lieferdatum beibehalten wurde, wird die Tour mit der neuen Routennummer angezeigt.

---

## Tour bearbeiten: Auftrag verschieben (VS 02-002)

### Ziel der Handlung
- Auftrag auf ein anderes Lieferdatum oder eine andere Route verschieben.
- Mehrere Aufträge verschieben.

### Voraussetzungen
- Touren werden in der Versandsteuerung angezeigt.

### Zusatzinfo
Wenn das neue Lieferdatum nicht zur gewählten Route passt, wird die Tour nicht auf das neue Lieferdatum verschoben. Wenn eine Ausweichroute definiert ist, wird auf diese verschoben.
Auswahl der Begründung: bei Betriebs- oder Kundenstorno wird die Position aus dem Auftrag gelöscht.
- ⇨ Position verschieben
- ⇨ Mehrere Positionen verschieben

### Workflow
1.  Register **TourenInfo > Auftragsebene** öffnen.
2.  Auftrag markieren > **[Verschieben]**.
    Dialog `Verschiebung (Versand)` wird geöffnet.
3.  Begründung für die Verschiebung mit **<Leertaste>** wählen und ggf. eine Anmerkung eintragen. Siehe dazu die Zusatzinfo.
4.  Feld **Auf Tourtag**: Lieferdatum ändern.
5.  Feld **Route**: ggf. neue Route eintragen.
    Wenn ein Tourplan erstellt ist: in Feld **Auf Tourtag <F9>** drücken und Tour auswählen.
6.  Verschiebung mit **[Start]** auslösen.
    Der Auftrag wird komplett auf das neue Lieferdatum und/oder die neue Tour verschoben.

**Mehrere Aufträge der Tour verschieben:**
7.  Lieferdatum und Route eintragen.
    Wenn das Lieferdatum kein Routentag ist, kann der Auftrag nicht verschoben werden.
8.  Feld **Mehrere Sätze verschieben: J** (ja) wählen.
9.  Verschiebung mit **[Start]** auslösen.
10. Ggf. die Abfrage mit **[Ja]** beantworten.
    Die Aufträge werden verschoben.
11. Verschiebung prüfen: Tourensuche mit neuem Lieferdatum starten.

---

## Tour bearbeiten: Position verschieben (VS 02-003)

### Ziel der Handlung
- Einzelne Position auf ein anderes Lieferdatum verschieben.
- Einzelne Position auf eine andere Route verschieben.

### Voraussetzungen
- Touren werden im Register **TourenInfo** angezeigt.
- Kunde erlaubt Teillieferung.

### Zusatzinfo
Wenn das neue Lieferdatum nicht zur gewählten Route passt, wird die Tour nicht auf das neue Lieferdatum verschoben. Wenn eine Ausweichroute definiert ist, wird auf diese verschoben.
Auswahl der Begründung: bei Betriebs- oder Kundenstorno wird die Position aus dem Auftrag gelöscht.
- ⇨ Mehrere Positionen verschieben

### Workflow
1.  Register **TourenInfo > Auftragsebene > Positionsebene** öffnen.
2.  Position markieren > **[Verschieben]**.
    Dialog `Verschiebung (Versand)` wird geöffnet.
3.  Begründung für die Verschiebung mit **<Leertaste>** wählen und ggf. eine Anmerkung eintragen. Siehe dazu die Zusatzinfo.
4.  Feld **Auf Tourtag**: Lieferdatum ändern.
5.  Feld **Route**: Route prüfen.
6.  Gesamte Position auf die neue Tour mit **[Start]** verschieben.
    Gesamte Position wird auf die neue Tour verschoben.
7.  Verschiebung prüfen: Tourensuche mit neuem Lieferdatum starten.

**Position für das gleiche Datum auf andere Route verschieben:**
8.  Feld **Auf Tourtag**: Lieferdatum prüfen.
9.  Feld **Route**: Route eintragen.
    Wenn das Lieferdatum kein Routentag ist, kann die Position nicht verschoben werden.
10. Verschiebung mit **[Start]** auslösen.
    Die Position wird komplett auf die neue Route verschoben. Wenn das Lieferdatum beibehalten wurde:
    -   Die Position wird mit der Original-Auftragsnummer mit der neuen Routennummer angezeigt.
    -   Die Position wird mit der Original-Auftragsnummer in eine bestehende Tour verschoben.
11. Verschiebung prüfen: Tourensuche mit neuem Lieferdatum starten.

---

## Tour bearbeiten: Mehrere Positionen verschieben (VS 02-004)

### Ziel der Handlung
- Alle nicht gelieferten Positionen vom Vortag verschieben.
- Mehrere Positionen eines Auftrags auf eine andere Route oder ein anderes Lieferdatum verschieben.
- Einzelne Mengen auf ein anderes Lieferdatum verschieben.

### Voraussetzungen
- Touren werden im Register **TourenInfo** angezeigt.
- Kunde erlaubt Teillieferung.

### Zusatzinfo
Positionen werden nur gebucht, wenn die Spalte **Buch.** markiert ist.
Auswahl der Begründung: bei Betriebs- oder Kundenstorno wird die Position aus dem Auftrag gelöscht.
- ⇨ Tour verschieben
- ⇨ Auftrag verschieben

### Workflow
1.  Register **TourenInfo** zum Lieferdatum vom Vortag anzeigen.
2.  Dialog zur Verschiebung mit **<Strg> + <E>** öffnen.
    Dialog `Verschiebung für` wird geöffnet.
3.  Aktuelles Lieferdatum prüfen und auf **[Auslösen]** klicken.
    Dialog `Verschiebung (Versand)` wird geöffnet.
4.  Ggf. in Spalte **Verschieben** die Stückzahl eintragen.
5.  Checkboxen in Spalte **Buch.** für die Verschiebung markieren.
    Die markierten Positionen werden komplett verschoben. Wenn nur Teilmengen angegeben sind, werden die entsprechenden Stückzahlen verschoben.
6.  Dialog für die Verschiebung mit **[Auslösen]** öffnen.
    Dialog `Verschiebung (Versand)` wird geöffnet.
7.  Daten für Verschiebung eintragen.
    Siehe Help Card "Position verschieben", Schritt 3 bis 5.
8.  Verschiebung mit **[Start]** auslösen.
9.  Abfragen mit **[Ja]** beantworten.
    Markierte Positionen werden auf das neue Lieferdatum verschoben.
    Die nicht verschobenen Positionen prüfen.
10. Verschiebung prüfen: Tourensuche mit neuem Lieferdatum starten.

---

## Tour bearbeiten: Verschieben mit Kontext-Menü (VS 02-005)

### Ziel der Handlung
- Touren, Aufträge oder Positionen im Explorer verschieben.

> **Hinweis:**
> Die Verschiebung von Touren, Aufträgen und Positionen über das Kontext-Menü löst keine Statusbuchungen im Auftrag aus. Diese Form der Verschiebung ist nur sinnvoll, wenn nur ein einziger Mitarbeiter mit der Versandplanung beauftragt ist.

### Voraussetzungen
- Versand-Explorer ist konfiguriert.
- Touren werden im Versand-Explorer angezeigt.

### Zusatzinfo
- ⇨ Mehrere Positionen verschieben

### Workflow
1.  Gewünschte Ebene im VS-Explorer öffnen.
2.  Cursor in Tour, Auftrag oder Position setzen.
3.  Kontext-Menü (rechte Maustaste) öffnen und Aktion auswählen, z. B. **Auftrag ausschneiden**.
4.  Kontext-Menü auf Zielebene öffnen, z. B. gleiche Tour am folgenden Tag.
5.  Aktion auswählen, z. B. **Auftrag einfügen**.
6.  Quell- und Zielebene öffnen und prüfen, ob die Daten wie gewünscht verschoben sind.
    Wenn eine einzelne Position an einem neuen Lieferdatum eingefügt wurde, wird die Position mit der Original-Auftragsnummer angezeigt.

---

## Versand vorbereiten: Fehlmenge kontrollieren (VS 03-001)

### Ziel der Handlung
- Produzierte Menge prüfen.
- Verfügbare Menge als verpackt buchen.
- Fehlende Menge als Rückstand verschieben.

### Voraussetzungen
- Touren werden im Register **TourenInfo** angezeigt.

### Zusatzinfo
Fehlmenge der Position kann unterschiedlich behandelt werden:
- Als Rückstand auf einen anderen Liefertermin verschieben.
- Als (Kunden-)Storno aus dem Auftrag entfernen und Position als komplett buchen.
- ⇨ Position verschieben
- ⇨ Mehrere Positionen verschieben

### Workflow
1.  Register **TourenInfo > Auftragsebene** öffnen.
2.  Auftrag markieren: **<Shift> + <F9>**.
    Dialog `Fehlmengenkontrolle für...` wird geöffnet.
3.  Auftragsdaten prüfen und ggf. korrigieren.
4.  Fehlmengenkontrolle mit **[Auslösen]** öffnen.
    Dialog `Versandsteuerung für Fehlmengenkontrolle` wird geöffnet.
5.  Mengen in Spalte **Fertig** prüfen.
    Wenn fertige Menge nicht identisch mit geplanter Menge ist, Fehlmenge verschieben. Siehe dazu die Zusatzinfo.
    ⇨ Mehrere Positionen verschieben, Schritt 4
6.  Fertige Menge nach Rücksprache korrigieren.
7.  Korrigierte Mengen mit **[Buchen]** speichern.
    Menge für den Rückstand wird in Spalte **Rück.** angezeigt.
    ⇨ Verpackte Menge korrigieren
8.  Fehlmenge mit **[Buchen]** verschieben.
    ⇨ Position verschieben, Schritt 3 bis 6
    Register **AuftragsInfo** wird angezeigt.
    Status des Auftrags ist umgesetzt auf komplett verpackt.

---

## Versand vorbereiten: Verpackte Menge korrigieren (VS 03-002)

### Ziel der Handlung
- Verpackte Menge prüfen.
- Verpackt gemeldete Menge ändern.

### Voraussetzungen
- Touren werden im Register **TourenInfo** angezeigt.

### Zusatzinfo
Fertig geplante Tour für weitere Bearbeitung sperren: Tourebene > **<Shift> + <F10>**

### Workflow
1.  Register **TourenInfo > Positionsebene** öffnen.
2.  Position für die Buchung der verpackten Menge wählen.
3.  Verpackte Menge in Spalte **Verp.** prüfen.
    Wenn verpackte Menge nicht identisch mit fertiger Menge ist, aktuellen Stand der Verpackung nachfragen.
4.  Verpackte Menge nach Rücksprache korrigieren: Korrekturmodus mit **<Shift> + <F10>** freischalten.
    Cursor springt in die Spalte **Verp.**
5.  Verpackte Menge in Spalte **Verp.** korrigieren.
6.  Verpackte Mengen buchen: Checkbox **Kmp** markieren.
    Verpackte Menge wird gebucht. Positionsstatus wird umgesetzt.
7.  Schritte 2 bis 3 nach Bedarf für jede Position wiederholen.

**Verpackt gemeldete Menge reduzieren:**
8.  Verpackte Menge in Spalte **Verp.** korrigieren.
    Dialog `Buchungsprotokoll` wird geöffnet.
9.  Buchungsdaten eingeben.
10. Reduzierung der verpackten Menge mit **[Buchen]** bestätigen.
    Verpackt gemeldete Menge wird gebucht. Nicht verpackte Menge wird im Feld **Rück.** angezeigt.
11. Reduzierte Menge auf ein anderes Lieferdatum verschieben.
    ⇨ Mehrere Positionen verschieben, Schritt 4

---

## Versand vorbereiten: Lieferanschrift ändern (VS 03-003)

### Ziel der Handlung
- Alternative Lieferanschrift auswählen.
- Neue Anschrift für Lieferung von Rückständen eingeben.

### Voraussetzungen
- Touren werden im Register **TourenInfo** angezeigt.

### Zusatzinfo
- Eine neue Anschrift kann mit **<F3>** in die Stammdaten des Kunden übernommen werden.
- Fertig geplante Tour für weitere Bearbeitung sperren: Tourebene > **<Shift> + <F10>**

### Workflow
1.  Register **TourenInfo > Auftragsebene** öffnen.
2.  Auftrag markieren: **<Shift> + <F8>**.
    Dialog `Lieferanschrift` wird geöffnet.
3.  Anschrift markieren und mit **[OK]** übernehmen.
    Register **Lieferanschrift**: Anschrift prüfen.

**Anschrift für Direktanlieferung erfassen:**
4.  Auftrag markieren: **<F4> > Lieferanschrift > Neue Lieferanschrift** wählen.
    Dialog zur Erfassung der Adresse wird angezeigt.
5.  Daten für Direktanlieferung eingeben.
6.  Ggf. Route ändern: **[Route suchen]**.
7.  Anschrift mit **[OK]** übernehmen.
    Register **Lieferanschrift**: Anschrift prüfen.

---

## Versand vorbereiten: Lieferschein erstellen (VS 03-004)

### Ziel der Handlung
- Vorab-Lieferschein drucken.
- End-Lieferschein erstellen.

### Voraussetzungen
- Druck von Vorab- und End-Lieferschein ist konfiguriert.
- Touren werden im Register **TourenInfo** angezeigt.
- Auftrag ist komplett verpackt gemeldet.

### Zusatzinfo
- Lieferscheine können nur gedruckt werden, wenn die Position als komplett verpackt gemeldet ist.
- Abhängig von der Konfiguration wird mit dem Lieferscheindruck auch die Rechnung gedruckt. Standardmäßig ist die Übergabe an den Rechnungsdruck nicht konfiguriert.

### Workflow
1.  Register **TourenInfo > Auftragsebene** öffnen.
2.  Auftrag markieren: **<Strg> + <F11>**.
    Dialog `Vorablieferschein für...` wird geöffnet.
3.  Daten prüfen und ggf. anpassen.
4.  Druck mit **[Auslösen]** starten.
    Dialog `Drucken auf...` wird geöffnet.
5.  Drucker und Anzahl der Druckexemplare angeben.
    In der Regel müssen Sie mindestens 2 Exemplare drucken.
6.  Druck des Vorab-Lieferscheins mit **<Enter>** starten.
7.  Druckabfrage mit **[Nein]** bestätigen.
    Die Exemplare des Vorab-Lieferscheins werden gedruckt.

**End-Lieferschein erstellen:**
8.  Auftrag markieren: **<F4> > <Strg> + <F9>**.
    Dialog `Lieferscheinfreigabe für...` wird geöffnet.
9.  Daten prüfen und ggf. anpassen.
10. Lieferscheinfreigabe mit **[Auslösen]** buchen.
    Dialog `Drucken auf` wird geöffnet.
11. Drucker und Anzahl der Druckexemplare angeben.
12. Lieferscheindruck mit **<Enter>** starten.
    Lieferschein wird gedruckt. Auftragsstatus wird auf **gesperrt** gesetzt.
    Je nach Konfiguration wird der Rechnungsdruck angestoßen.

---

## Versand vorbereiten: Ladefolge bearbeiten (VS 03-005)

### Ziel der Handlung
- Ladefolge ändern.
- Ladeliste für eine Tour drucken.
- Ladelisten für alle Touren drucken.
- Ergänzungsladeliste drucken.

### Voraussetzungen
- Funktionen für Ladefolge müssen konfiguriert sein.
- Touren werden im Register **TourenInfo** angezeigt.

### Zusatzinfo
- Nur für gedruckte Ladelisten können Ergänzungsladelisten gedruckt werden.
- Fertig geplante Tour für weitere Bearbeitung sperren: Tourebene > **<Shift> + <F10>**

### Workflow
1.  Register **TourenInfo > Auftragsebene** öffnen.
2.  Zum Register **Lieferanschrift** wechseln.
3.  Feld **LF**: Laufende Nummern ändern.
4.  Abfrage beantworten, ob die Nummer auf die anderen Aufträge des Kunden vererbt werden soll.
    Die laufende Nummer wird bei allen Aufträgen eingefügt, die zu demselben Kunden gehören.

**Ladeliste neu drucken**
1.  Register **TourenInfo**: **<Strg> + <F8>**.
2.  Drucker und Anzahl der Druckexemplare angeben.
3.  Druck mit **<Enter>** starten.
    Ladeliste wird gedruckt. Der Status der Tour wird auf **gesperrt** gesetzt.

**Ladelisten für alle angezeigten Touren drucken:**
4.  Register **TourenInfo**: **<Strg> + <F12>**.
5.  Haus (Mandant) und Zeitspanne prüfen und ggf. anpassen.
6.  Eingabe mit **<Enter>** bestätigen.
7.  Drucker und Anzahl der Druckexemplare angeben.
8.  Druck mit **<Enter>** starten.
    Ladeliste wird gedruckt. Der Status der Tour wird auf **gesperrt** gesetzt.

**Ergänzungsladeliste drucken:**
1.  Register **TourenInfo**: **<Strg> + <F10>**.
2.  Schritte 5 bis 8 wiederholen.
    Ladeliste mit den Ergänzungen zur Original-Ladeliste wird gedruckt.

---

## Versand vorbereiten: Vorgang stornieren (VS 03-006)

### Ziel der Handlung
Vorgang stornieren:
- Auftrag
- Lieferschein
- Versandstatus

### Voraussetzungen
- Storno-Funktion ist konfiguriert.
- Touren werden im Register **TourenInfo** angezeigt.

### Zusatzinfo
- ⇨ Auftragsinfos einsehen

### Workflow
1.  Menü **Logistik > Versandsteuerung > gewünschte Ebene** öffnen.
2.  Vorgang auswählen, z. B. Auftrag.
3.  Infomenü mit **<Shift> + <F4>** öffnen.
    Infomenü wird geöffnet.
4.  Eintrag **Storno** wählen.
    Untermenü wird geöffnet.
5.  Art des Stornos wählen, z. B. **Auftragsstorno**.
    Dialog `Auftragsstorno` wird geöffnet.
6.  Daten prüfen und mit **[Auslösen]** bestätigen.
7.  Ggf. Abfrage mit **[Ja]** bestätigen.
    Dialog für Begründung wird geöffnet.
8.  Begründung für Storno angeben und mit **<Enter>** bestätigen.
    Der Vorgang wird storniert. Das Stornokennzeichen und der Stornogrund werden in den Vorgang übernommen, z. B. in den Lieferschein oder den Auftrag.

---

## Zusatzfunktionen: Tourgrafik anzeigen (VS 04-001)

### Ziel der Handlung
- Auslastung der Touren eines Lieferdatums darstellen.
- Auslastung einer Tour an aufeinander folgenden Liefertagen darstellen.

### Voraussetzungen
- Touren werden im Register **TourenInfo** angezeigt.

### Zusatzinfo
(Keine Zusatzinformationen auf dieser Karte)

### Workflow
1.  Register **TourenInfo**.
2.  Parameterauswahl mit **<Shift> + <F11>** öffnen.
    Dialog `1. Parameter für Übersicht` wird geöffnet.
3.  Parameter 1 wählen: **Stück, QM, Gewicht**.
4.  Mit **<Enter>** bestätigen.
    Dialog `2. Parameter für Übersicht` wird geöffnet.
5.  Parameter wählen: **Alle Routen für den aktuellen Tourentag anzeigen**.
6.  Mit **<Enter>** bestätigen.
    Ist- und Soll-Stückzahlen für die Touren werden dargestellt.

**Auslastung einer Tour anzeigen.**
7.  Parameter 1 wählen und mit **<Enter>** bestätigen.
    Dialog `2. Parameter für Übersicht` wird geöffnet.
8.  Parameter wählen: **Nächste Tourentage für aktuelle Route anzeigen**.
9.  Mit **<Enter>** bestätigen.
    Auslastung der Tour an Folgetagen wird dargestellt.

---

## Zusatzfunktionen: Auftragsinfos einsehen (VS 04-002)

### Ziel der Handlung
- Informationen zum Auftrag einsehen.
- Informationen des Fertigwarenlagers zum Auftrag einsehen.
- Buchungsprotokoll zum Fertigwarenlager einsehen.

### Voraussetzungen
- Touren werden im Register **TourenInfo** angezeigt.
- Fertigwarenlager muss konfiguriert sein.

### Zusatzinfo
(Keine Zusatzinformationen auf dieser Karte)

### Workflow
1.  Register **TourenInfo > Auftragsebene** öffnen.
2.  Auftrag markieren: **<Strg> + <K>**.
    Dialog `Informationen zu Auftrag` wird geöffnet.
3.  Auftragsnummer eingeben.
4.  Modus prüfen: **VK-Aus.**
5.  Suche mit **[Auslösen]** starten.
    Dialog `Informationen zu Auftrag` wird geöffnet.
6.  Auftragsinfos verlassen: mit **[Springen]** zurück zum Register **PositionsInfo**.

**Aufträge im Fertigwarenlager einsehen:**
7.  Informationen zum Buchungsprotokoll des Fertigwarenlagers mit **[FW Lager]** öffnen.
    Dialog `Fertigwarenlager Buchungsprotokoll` wird geöffnet.

**Buchungen im Fertigwarenlager einsehen:**
8.  Übersicht für das Fertigwarenlager mit **[Protokoll]** öffnen.
    Dialog `Fertigwarenlager Übersicht` wird geöffnet.
