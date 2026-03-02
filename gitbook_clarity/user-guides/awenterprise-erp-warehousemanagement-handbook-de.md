---
description: "A+W Enterprise Lager Software Reference"
---


# Softwarereferenz

---
## Lager-Buchungen

### Bestände (Mengeneinheit)
Lagerbestand der Variante in den Mengen, die für diese Artikelvariante in den Stammdaten definiert ist.

- **Alt:** Alter Artikelbestand im Lager, bevor gebucht wird.
  **Technische Info:** Anzeige-Feld, DB-Feld: `wlbv.g_anz`
- **Buchung:** Artikelbestand, der gebucht wird.
  **Technische Info:** numerisches Feld, ohne DB-Bezug
- **Neu:** Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn der neue Artikel gebucht wird. Wenn Sie den Dialog mit `<Pos1>` verlassen, wird der alte Lagerbestand beibehalten.
  **Technische Info:** Anzeige-Feld, DB-Feld: `wlbv.g_anz`, `wlprot.g_anz`

### Preise
Die Anzeige der Währung richtet sich nach der Eigenwährung, die bei der Installation festgelegt wurde.

- **€/qm:** Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
  **Technische Info:** numerisches Feld, ohne DB-Bezug
- **Preis:** Gesamtpreis des Artikels pro Variante für die eingegebene Menge. Bei Lager-Eingangsbuchung geben Sie entweder Preis €/qm ein (hier wird der Gesamtpreis für die Eingangsbuchung errechnet), oder Sie geben den Gesamtpreis für die eingehende Lagerbuchung ein und Preis €/qm wird errechnet.
  **Technische Info:** numerisches Feld, DB-Feld: `wlbv.g_preis`, `wlprot.g_preis`

### (Spalte ohne Bezeichnung) Buchungsstatus der Artikelposition.

*Tab. F-3 Buchungsstatus der Artikelposition*

| Buchungsstatus mit Farbkennzeichen | Bedeutung |
| :--- | :--- |
| grau | Artikelposition ist vom Prozess (Programm) gebucht worden. |
| rot | Artikelposition ist vom Prozess (Programm) nicht oder noch nicht gebucht worden. |

---

## Lagerausgang

**Buchung > Ausgang**

*Abb. F-4 Lagerausgang*

In diesem Dialog erfassen und buchen Sie den Lagerausgang, z. B., wenn Lagerartikel an die Produktion geliefert werden. Die Lagerausgänge für Kisten, Fächer, Stapel, Gestelle und auftragsbezogenen Warenausgänge buchen Sie an folgender Stelle:

- "Kistenlagerausgang" auf Seite F-1710
- "Fachlagerausgang" auf Seite F-1716
- "Stapellageränderung" auf Seite F-1718
- "Gestelllagerausgang" auf Seite F-1723
- "Lagerausgang (Auftragsbezogen)" auf Seite F-1727

Sie können folgende Tastaturbefehle ausführen:

- Mit `<Strg>` + `<F8>` können Sie im ersten Feld zwischen dem Dialog Lagereingang und Lagerausgang wechseln.
- Mit `<F5>` können Sie aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.

Die Register, Felder und Spalten sind an folgender Stelle beschrieben:
- "Lagereingang" auf Seite F-1693

Die Werte in den Feldern zeigen jeweils die abzubuchenden Mengen an.

---

## Kistenlagereingang

**Buchung > Kisteneingang**

In diesem Dialog buchen Sie die Lagereingänge für Lagerartikel, die sich in Kisten im entsprechenden Lager befinden, z. B. Gitterboxen mit 50 gleichen Scheiben.

Sie können über die Auswahl des richtigen Lager im Feld Lager auswählen, ob Sie die Lagereingänge ins Kistenlager oder ins Einzelblattkistenlager buchen.

> **Kistenlager und Einzelblatt-Kistenlager**
> Der Unterschied der Lagerbuchungen zwischen Kistenlager und Einzelblattlager besteht in der Art der Kistenerfassung. Im Kistenlager werden die Glasscheiben mit gleichen Merkmalen (z.B.: Preis, Ausbeute) kistenweise gebucht. Im Einzelblatt-Kistenlager werden die Ware als Einzelscheiben (Blätter) mit dazugehöriger Information in der jeweiligen Kiste gebucht.

Die Lagerart legen Sie in den Stammdaten fest:
- "Lagerraumverwaltung" auf Seite F-1733

In dem Dialog Kisteneingang finden Sie folgende Register:

- "Kistenlagereingang - Register Stück" auf Seite F-1704
- "Kistenlagereingang - Menge" auf Seite F-1707

Wenn Sie ein Einzelblattkistenlager auswählen, können Sie die Blätter einzeln in Kisten verbuchen.
- "Kistenlagereingang - Menge" auf Seite F-1707

---

## Kistenlagereingang – Register Stück

**Buchung > Kisteneingang > Register Stück**

*Abb. F-5 Kistenlagereingang – Stück, Kistenlager und Einzelblattkistenlager*

In diesem Register erfassen Sie die Lagereingänge für komplette Kisten. Sie können folgende Tastaturbefehle ausführen:

- Mit `<Strg>` + `<F8>` können Sie im ersten Feld zwischen dem Dialog Kistenlagereingang und Kistenlagerausgang wechseln.
- Mit `<F5>` können Sie aus einer Spalte in die kistenbezogenen Angaben im Fußbereich (linke Seite) wechseln.
- Mit `<Shift>` + `<F8>` können Sie aus einer Spalte in die variantenbezogenen Angaben im Fußbereich (rechte Seite) wechseln.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.

### Kopfbereich
Die Felder sind an folgender Stelle beschrieben:
- "Lagereingang" auf Seite F-1693

### Rumpfbereich
In diesem Bereich buchen Sie die Bestände und Preise der Artikel in Stückzahlen.

- **Variante:** Maßvariante des Artikels. Mit `<F9>` können Sie die Variantenauswahl aufrufen. Dabei werden nur die Varianten angezeigt, die dem aktuellen Artikel in den Stammdaten zugewiesen sind.

---

### Technische Details (Fortsetzung Rumpfbereich)

- **Technische Info:** alphanumerisches Feld, DB-Bezug: `wlbv_massbez`, `wlprot.massbez`
- **Kiste:** Kistennummer. Beim Lagereingang wird die Kistennummer automatisch vom System vergeben.
  **Technische Info:** Anzeige-Feld, DB-Bezug: `wlbv_kinr`, `wlprot.kinr`
- **Kistenbezeichnung:** Bezeichnung der Kiste.
  **Technische Info:** alphanumerisches Feld, DB-Bezug: `wlbv_kistenbez`, `wlprot.kistenbez`
- **Lieferant:** Lieferantennummer.
  **Technische Info:** numerisches Feld, DB-Bezug: `wlprot.linr`
- **Verpackungsart:** Kennzeichen der Verpackungsart, z. B. 13 = Kleine Holzkiste.
  **Technische Info:** numerisches Feld, DB-Bezug: `wlprot.verpackart`
- **Neu:** Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn der neue Artikel gebucht wird. Wenn Sie den Dialog mit `<Pos1>` verlassen, wird der alte Lagerbestand beibehalten.
  **Technische Info:** Anzeige-Feld, DB-Feld: `wlbv.g_anz`

### Bestände
Lagerbestand der Variante in Stückzahlen. Mit `<F2>` können Sie durch folgende Anzeigen wechseln:

- **Alt:** Alter Artikelbestand im Lager, bevor gebucht wird.
  **Technische Info:** numerisches Feld, DB-Bezug: `wlxv.g_anz`
- **Buchung:** Artikelbestand, der gebucht wird.
  **Technische Info:** numerisches Feld, ohne DB-Bezug
- **Neu:** Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn der neue Artikel gebucht wird. Wenn Sie den Dialog mit `<Pos1>` verlassen, wird der alte Lagerbestand beibehalten.
  **Technische Info:** numerisches Feld, DB-Bezug: `wlxv.g_anz`

### Preise
Die Anzeige der Währung richtet sich nach der Eigenwährung, die bei der Installation festgelegt wurde.

- **€/qm:** Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
  **Technische Info:** numerisches Feld, ohne DB-Bezug
- **Preis:** Gesamtpreis des Artikels pro Variante für die eingegebene Menge. Bei Lager-Eingangsbuchung geben Sie entweder Preis €/qm ein (hier wird der Gesamtpreis für die Eingangsbuchung errechnet), oder Sie geben den Gesamtpreis für die eingehende Lagerbuchung ein und Preis €/qm wird errechnet.
  **Technische Info:** numerisches Feld, DB-Feld: `wlbv.g_preis`, `wlprot.g_preis`

**(Spalte ohne Bezeichnung):** Buchungsstatus der Artikelposition.

---

### Fußbereich – Kistenbezogene Angaben

Kistenbezogene Angaben können Sie mit `<F5>` aufrufen. Die meisten Felder sind bereits an folgender Stelle beschrieben:
- "Lagereingang" auf Seite F-1693

Zusätzlich werden folgende Felder beschrieben:

**Lieferant**
Lieferantennummer. Die Lieferantennummer wird aus dem Rumpfdialog übernommen und kann in den kistenbezogenen Angaben nicht geändert werden.
**Technische Info:** Anzeige-Feld

**Verpackungsart**
Kennzeichen der Verpackungsart. Die lieferantenbezogene Verpackungsart wird aus den Stammdaten übernommen und kann in den kistenbezogenen Angaben nicht geändert werden.
**Technische Info:** Anzeige-Feld

**Reserviert**
Auftragsnummer, für die die Kiste reserviert wurde.
**Technische Info:** numerisches Feld, DB-Feld: `wlbv.reserved`

**Etikett**
Anzeige für den Etikettendruck.
- J = Etiketten wurden bereits gedruckt.
- N = Keine Etiketten wurden bisher gedruckt.
**Technische Info:** Anzeige-Feld

*Tab. F-4 Buchungsstatus der Artikelposition*

| Buchungsstatus mit Farbkennzeichen | Bedeutung |
| :--- | :--- |
| grau | Artikelposition ist vom Prozess (Programm) gebucht worden. |
| rot | Artikelposition ist vom Prozess (Programm) nicht oder noch nicht gebucht worden. |

---

## Kistenlagereingang – Menge

**Buchung > Kisteneingang > Menge**

*Abb. F-6 Kistenlagereingang – Menge*

In diesem Register buchen Sie die Bestände und Preise der Artikel in Mengeneinheit.

Das Register Menge ist wie das Register Stück aufgebaut.
- "Kopfbereich" auf Seite F-1704
- "Fußbereich - Kistenbezogene Angaben" auf Seite F-1706

### Rumpfbereich
In diesem Bereich buchen Sie die Bestände und Preise der Artikel in Mengeneinheit.

**Variante**
Maßvariante des Artikels. Mit `<F9>` können Sie die Variantenauswahl aufrufen. Dabei werden nur die Varianten angezeigt, die dem aktuellen Artikel in den Stammdaten zugewiesen sind.
**Technische Info:** alphanumerisches Feld, DB-Bezug: `wlbv_massbez`, `wlprot.massbez`

**Kiste**
Kistennummer. Beim Lagereingang wird die Kistennummer automatisch vom System vergeben.
**Technische Info:** Anzeige-Feld, DB-Bezug: `wlbv_kinr`, `wlprot.kinr`

**Kistenbezeichnung**
Bezeichnung der Kiste.
**Technische Info:** alphanumerisches Feld, DB-Bezug: `wlbv_kistenbez`, `wlprot.kistenbez`

---

**Lieferant**
Lieferantennummer.
**Technische Info:** numerisches Feld, DB-Bezug: `wlprot.linr`

**Verpackungsart**
Kennzeichen der Verpackungsart, z. B. 13 = Kleine Holzkiste.
**Technische Info:** numerisches Feld, DB-Bezug: `wlprot.verpackart`

**Neu:**
Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn der neue Artikel gebucht wird. Wenn Sie den Dialog mit `<Pos1>` verlassen, wird der alte Lagerbestand beibehalten.
**Technische Info:** numerisches Feld, DB-Bezug: `wlbv.g_anz`

### Bestände
Lagerbestand der Variante in der Mengeneinheit, die in den Stammdaten definiert ist.

- **ME:** Neu berechneter Artikelbestand in Mengeneinheiten. Dieser Bestand wird übernommen, wenn der neue Artikel gebucht wird. Wenn Sie den Dialog mit `<Pos1>` verlassen, wird der alte Lagerbestand beibehalten.

### Preise
Die Anzeige der Währung richtet sich nach der Eigenwährung, die bei der Installation festgelegt wurde.

- **€/qm:** Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
- **Preis:** Gesamtpreis des Artikels.

**(Spalte ohne Bezeichnung)**
Buchungsstatus der Artikelposition.

---

## Einzelblattinformationen

*Abb. F-7 Kistenlagereingang - Einzelblattkistenlager*

Die Einzelblattinformationen können Sie nur aufrufen, wenn Sie im Kopfbereich im Feld Lager ein Einzelblattkistenlager ausgewählt haben. Im Weiteren können Sie:

- Mit `<Shift>` + `<F12>` sich die Einzelblattinformationen anzeigen lassen.
- Mit `<Strg>` + `<E>` Sie die Einzelblattinformationen bearbeiten.

Im Dialog rechts unten wird die Tabelle für die Einzelblattinformationen mit den folgenden Spalten angezeigt:

**Blatt**
Nummer des Blattes.
**Technische Info:** numerisches Feld, DB-Feld: `wlblatt.blatt`

**Bezeichnung**
Bezeichnung des Blattes.
**Technische Info:** numerisches Feld, DB-Feld: `wlblatt.blattbez`

**EU/Stück**
Stückpreis des Blattes, bezogen auf 100% der Ausbeute.
**Technische Info:** numerisches Feld, DB-Feld: `wlblatt.g_preis`

**Ausbeute**
Ausbeute in Prozent = nutzbare Fläche.
**Technische Info:** numerisches Feld, DB-Feld: `wlblatt.ausbeute`

**Reserviert**
Reservierungskennzeichen.
- J = Glasscheibe ist für einen Vorgang reserviert.
- N = Glasscheibe ist noch nicht für einen Vorgang reserviert.

---

## Kistenlagerausgang

**Buchung > Kistenausgang**

*Abb. F-8 Kistenlagerausgang*

In diesem Dialog buchen Sie Lagerausgänge für komplette Kisten. Wenn Sie nur einen Teil der Artikel aus einer Kiste ausbuchen möchten, müssen Sie zuerst die Kiste auflösen und die Artikel der Kiste auf ein anderes Lager buchen.

Sie können folgende Tastaturbefehle ausführen:

- Mit `<Strg>` + `<F8>` können Sie im ersten Feld zwischen dem Dialog Kisteneingang und Kistenausgang wechseln.
- Mit `<F5>` können Sie aus einer Spalte in die kistenbezogenen Angaben im Fußbereich (linke Seite) wechseln.
- Mit `<Shift>` + `<F8>` können Sie aus einer Spalte in die variantenbezogenen Angaben im Fußbereich (rechte Seite) wechseln.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.
- Mit `<Strg>` + `<F12>` können Sie komplette Kisten buchen. Damit wird die gesamte Kiste ausgebucht.
- Mit `<Strg>` + `<F8>` können Sie Kisten auflösen und die Artikel aus der Kiste auf ein Ziellager buchen. Damit werden die einzelnen Scheiben der Kiste in das Ziellager gebucht.

Die Register, Felder und Spalten sind an folgender Stelle beschrieben:
- "Kistenlagereingang" auf Seite F-1703

---

## Fachlagereingang

**Buchung > Facheingang**

In diesem Dialog können Sie Artikel auf Fächer eines Fachlagers buchen.
In diesem Dialog finden Sie folgende Register:

- Fachlagereingang – Stück
- Fachlagereingang - Menge

### Fachlagereingang – Stück

**Buchung > Facheingang > Stück**

*Abb. F-9 Fachlagereingang – Stück*

In diesem Register erfassen und buchen Sie die Bestände und Preise der aktuellen Artikelvariante in Stückzahlen.

Sie können folgende Tastaturbefehle ausführen:

- Mit `<Strg>` + `<F8>` können Sie im ersten Feld zwischen dem Dialog Fachlagereingang und Fachlagerausgang wechseln.
- Mit `<F5>` können Sie aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.

---

### Kopfbereich
Die Felder sind an folgender Stelle beschrieben:
- "Lagereingang" auf Seite F-1693

### Rumpfbereich
In diesem Register buchen Sie die Bestände und Preise der Artikel in Stückzahlen.

**Variante**
Maßvariante des Artikels. Mit `<F9>` können Sie die Variantenauswahl aufrufen. Dabei werden nur die Varianten angezeigt, die dem aktuellen Artikel in den Stammdaten zugewiesen sind.

- **Fach:** Bezeichnung des Fachs.

### Bestände (Stück)
Lagerbestand der Variante in Stückzahlen.

- **Alt:** Alter Artikelbestand im Lager, bevor gebucht wird.
- **Buchung:** Artikelbestand, der gebucht wird.
- **Neu:** Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn der neue Artikel gebucht wird. Wenn Sie den Dialog mit `<Pos1>` verlassen, wird der alte Lagerbestand beibehalten.

### Preise
Die Anzeige der Währung richtet sich nach der Eigenwährung, die bei der Installation festgelegt wurde.

- **€/qm:** Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
- **Preis:** Gesamtpreis des Artikels.
- **(Spalte ohne Bezeichnung):** Buchungsstatus der Artikelposition.

*Tab. F-5 Buchungsstatus der Artikelposition*

| Buchungsstatus mit Farbkennzeichen | Bedeutung |
| :--- | :--- |
| grau | Artikelposition ist vom Prozess (Programm) gebucht worden. |
| rot | Artikelposition ist vom Prozess (Programm) nicht oder noch nicht gebucht worden. |

### Fußbereich – Variantenbezogene Angaben

**Objekt**
Bezeichnung des Objekts bei auftragsbezogenen Lagerartikeln, z. B. Baustelle des Kunden.

**Kostenstelle**
Bezeichnung der Kostenstelle für statistische Auswertungen.

---

**Bemerkung**
Textfeld für zusätzliche Informationen.

> **Lauf- und Optimierungsnummer im Bemerkungsfeld**
> Bei der Rückmeldung von Lagerabbuchungen über den ERP Webservice werden nun die Lauf- und die Optimierungsnummer in das Bemerkungsfeld der Buchung geschrieben.

**Mindestbestand**
Minimal zulässiger Lagerbestand des Artikels, um Produktionsengpässe zu verhindern.

**Alarmbestand**
Stückzahl des Artikelbestands, die einen Bestellvorschlag im Einkauf anlegt. Durch Alarmbestände können Sie eine Unterdeckung des Lagers verhindern.

**Maximalbestand**
Maximal zulässiger Lagerbestand des Artikels, um Lagerkosten zu minimieren.

**Gesamtpreis**
Gesamtpreis der Artikelvariante.

**Durchschnittspreis**
Durchschnittlicher Einkaufspreis der Artikelvariante im Lager.

**Höchstpreis**
Höchster Einkaufspreis der Artikelvariante im Lager.

**Niedrigstpreis**
Niedrigster Einkaufspreis der Artikelvariante im Lager.

**LIFO-Gesamtpreis**
Gesamtpreis der Artikelvariante im Lager, wenn die zuletzt eingelagerten Lagerartikel als erste Artikel ausgelagert werden.

**FIFO-Gesamtpreis**
Gesamtpreis der Artikelvariante im Lager, wenn die zuerst eingelagerten Lagerartikel als erste Artikel ausgelagert werden.

---

## Fachlagereingang – Menge

**Buchung > Facheingang > Menge**

*Abb. F-10 Fachlagereingang – Menge*

In diesem Register erfassen und buchen Sie die Bestände und Preise der aktuellen Artikelvariante in Mengeneinheit.

Das Register Menge ist wie das Register Stück aufgebaut.
- "Kopfbereich" auf Seite F-1712
- "Fußbereich - Variantenbezogene Angaben" auf Seite F-1712

### Rumpfbereich
In diesem Bereich buchen Sie die Bestände und Preise der Artikel in Mengeneinheit.

- **Variante:** Maßvariante des Artikels. Mit `<F9>` können Sie die Variantenauswahl aufrufen. Dabei werden nur die Varianten angezeigt, die dem aktuellen Artikel in den Stammdaten zugewiesen sind.
- **Fach:** Bezeichnung des Fachs.

### Bestände (Mengeneinheit)
Lagerbestand der Variante in Mengeneinheit.

- **Alt:** Alter Artikelbestand im Lager, bevor gebucht wird.
- **Buchung:** Artikelbestand, der gebucht wird.

---

- **Neu:** Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn der neue Artikel gebucht wird. Wenn Sie den Dialog mit `<Pos1>` verlassen, wird der alte Lagerbestand beibehalten.

### Preise
Die Anzeige der Währung richtet sich nach der Eigenwährung, die bei der Installation festgelegt wurde.

- **€/qm:** Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
- **Preis:** Gesamtpreis des Artikels.
- **(Spalte ohne Bezeichnung):** Buchungsstatus der Artikelposition.

*Tab. F-6 Buchungsstatus der Artikelposition*

| Buchungsstatus mit Farbkennzeichen | Bedeutung |
| :--- | :--- |
| grau | Artikelposition ist vom Prozess (Programm) gebucht worden. |
| rot | Artikelposition ist vom Prozess (Programm) nicht oder noch nicht gebucht worden. |

---

## Fachlagerausgang

**Buchung > Fachlagerausgang**

*Abb. F-11 Fachlagerausgang*

In diesem Dialog können Sie Artikel vom Fachlager abbuchen.

Sie können folgende Tastaturbefehle ausführen:

- Mit `<Strg>` + `<F8>` können Sie im ersten Feld zwischen dem Dialog Fachlagereingang und Fachlagerausgang wechseln.
- Mit `<F5>` können Sie aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.

Die Register, Felder und Spalten sind an folgender Stelle beschrieben:
- "Fachlagereingang" auf Seite F-1711

---

## Stapellagereingang

**Buchung > Stapeleingang**

**Zu Dialogbeschreibung:**
- Stapellageränderung

*Abb. F-12 Stapellagereingang*

In diesem Dialog können Sie Artikel auf einen Stapel buchen. Sie können verschiedene Artikel mit unterschiedlichen Abmessungen auf einen Stapel buchen.

Sie können folgende Tastaturbefehle ausführen:

- Mit `<Strg>` + `<F8>` können Sie im ersten Feld zwischen dem Dialog Stapellagereingang und Stapellageränderung wechseln.
- Mit `<F2>` können Sie die Anzeige zwischen Artikel in Stückzahl und Artikel in Mengeneinheit umschalten.
- Mit `<Shift>` + `<F8>` können Sie vom System eine neue Stapelnummer vergeben lassen.
- Mit `<Shift>` + `<F9>` können Sie alle Stapelzeilen kopieren und einer neuen Stapelnummer zuordnen.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.
- Mit `<Strg>` + `<F12>` können Sie einen Stapel einbuchen.
- Mit `<Ende>` können Sie die Stapelbuchung buchen.

---

### Kopfbereich

**Lager**
Lagernummer und Lagerbezeichnung.

**Lieferant**
Lieferantennummer und Lieferantenname.

**Letzte Änderung am, von**
Datum der letzten Änderung am Buchungssatz und Name des Anwenders, der die letzte Buchung ausgeführt hat.

### Rumpfbereich

- **Stapel:** Nummer des Stapelplatzes.
- **Bezeichnung:** Bezeichnung des Stapelplatzes.
- **Artikel:** Artikelnummer des Artikels, der auf dem Stapelplatz eingelagert wird.
- **Variante:** Bezeichnung der Artikelvariante.
- **Anzahl:** Stückzahl des Artikels. Mit `<F2>` können Sie auf Artikel in Mengeneinheit umschalten.
- **Menge/qm:** Menge in Quadratmetern.
- **Preis /qm:** Preis pro Mengeneinheit.

## Stapellageränderung

**Buchung > Stapeländerung**

---

*Abb. F-13 Stapellageränderung*

In diesem Dialog können Sie nach Artikeln suchen die in Stapeln vorkommen, um sie in ein anderes Lager zu buchen.

---

Sie können folgende Tastaturbefehle ausführen:

- Mit `<Strg>` + `<F8>` können Sie im Kopfbereich zwischen dem Dialog Stapellagereingang und Stapellageränderung wechseln.
- Mit `<Strg>` + `<F8>` können Sie im Rumpfbereich den ausgewählten Stapel auflösen. Wenn ein Stapel aufgelöst wird, müssen die Artikel aus dem aufgelösten Stapel auf ein anderes Lager gebucht werden. Das Lager für die Artikel geben Sie in der Spalte Ziellager ein.
- Mit `<Shift>` + `<F9>` können Sie im Rumpfbereich den ausgewählten Datensatz kopieren.
- Mit `<F2>` können Sie die Anzeige zwischen Artikel in Stückzahl und Artikel in Mengeneinheit umschalten.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.
- Mit `<Strg>` + `<F12>` können Sie einen Stapel ausbuchen.
- Mit `<Ende>` können Sie die Stapeländerung buchen.

Die Felder und Spalten sind an folgender Stelle beschrieben:
- "Stapellagereingang" auf Seite F-1717

Zusätzlich werden folgende Felder angezeigt:

### Kopfbereich

**Artikel 1, Artikel 2**
Suche über eine Folge von Artikelnummern.

### Rumpfbereich

- **Ziellager:** Nummer des Ziellagers.

---

## Gestelllagereingang

**Buchung > Gestelllagereingang**

**Zu Dialogbeschreibung:**
- Gestelllagerausgang

*Abb. F-14 Gestelllagereingang*

In diesem Dialog können Sie Artikel auf Gestellen in ein Gestelllager einbuchen.

Sie können folgende Tastaturbefehle ausführen:

- Mit `<Strg>` + `<F8>` können Sie im ersten Feld zwischen dem Dialog Gestelllagereingang und Gestelllagerausgang wechseln.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.

### Kopfbereich
Im Kopfbereich müssen Sie entweder den Artikel und das Lager angeben oder das Gestell.

**Artikel**
Artikelnummer und Artikelbezeichnung.

**Lager**
Lagernummer und Lagerbezeichnung.

**Gestell**
Externe Bezeichnung des Lagergestells.

---

**Gesamtbestand**
Gesamtbestand des Artikels, einschließlich aller Artikelvarianten.

**Gesamtwert**
Gesamtbetrag des Lagerartikels.

**Buchungsstatus**
Status der Buchungen im Lager.

*Tab. F-7 Buchungsstatus des Lagers*

| Buchungsstatus mit Farbkennzeichen | Bedeutung |
| :--- | :--- |
| grau | Im Lagereingang sind alle Buchungspositionen vom Prozess (Programm) gebucht worden. |
| rot | Im Lagereingang ist mindestens eine Buchungsposition vom Prozess (Programm) nicht oder noch nicht gebucht worden. |

**Letzte Änderung am, von**
Datum der letzten Änderung am Buchungssatz und Name des Anwenders, der die letzte Buchung ausgeführt hat.

### Rumpfbereich

- **Variante:** Maßvariante des Artikels. Mit `<F9>` können Sie die Variantenauswahl aufrufen. Varianten eines Artikels werden nur angezeigt, wenn die Varianten im Stammdatenmodul angelegt sind.
- **Gestell:** Externe Gestellbezeichnung des Lagergestells.
- **G:** Artikelvarianten, die sich auf dem Gestell befinden.
  - Verschiedene Artikelvarianten stehen auf einem Gestell.
  - Nur gleiche Artikelvarianten stehen auf einem Gestell.
- **Fach:** Bezeichnung des Fachs.
- **Fifo-Datum:** Datum für die Gestellbuchung nach dem Fifo-Prinzip.
- **Menge:** Aktuelle Stückzahl der Artikel auf dem Lagergestell.
- **Buchung:** Artikelbestand, der gebucht wird.
- **€/qm:** Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
- **Preis:** Gesamtpreis des Artikels.
- **Buchungsstatus:** Status der Buchungen im Gestelllagereingang.

---

## Gestelllagerausgang

**Buchung > Gestellausgang**

In diesem Dialog können Sie gestellbezogene Lagerabgänge buchen oder Artikel zwischen Gestellen umbuchen.

In diesem Dialog finden Sie folgende Register:

- "Gestelllagerausgang - Auftragsbezogen" auf Seite F-1723
- "Gestelllagerausgang – Umbuchung" auf Seite F-1725

### Gestelllagerausgang – Auftragsbezogen

**Buchung > Gestellausgang > Auftragsbezogen**

*Abb. F-15 Gestelllagerausgang - Auftragsbezogen*

In diesem Register buchen Sie die auftragsbezogenen Lagerabgänge.

Sie können folgende Tastaturbefehle ausführen:

- Mit `<Strg>` + `<F8>` können Sie im ersten Feld zwischen dem Dialog Gestelllagereingang und Gestelllagerausgang wechseln.
- Mit `<F2>` können Sie zwischen den Registern Auftragsbezogen und Umbuchung umschalten.
- Mit `<F5>` können Sie in die variantenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.
- Mit `<Shift>` + `<F8>` können Sie eine Position auflösen.

---

**[Zurücksetzen]**
Verwirft die eingegebenen Änderungen.

### Kopfbereich
Im Kopfbereich müssen Sie entweder den Artikel und das Lager angeben oder das Gestell.
Die Felder sind an folgender Stelle beschrieben:
- "Gestelllagereingang" auf Seite F-1721

### Rumpfbereich
- **Variante:** Maßvariante des Artikels. Mit `<F9>` können Sie die Variantenauswahl aufrufen. Varianten eines Artikels werden nur angezeigt, wenn die Varianten im Stammdatenmodul angelegt sind.
- **Gestell:** Externe Gestellbezeichnung des Lagergestells.
- **G:** Artikelvarianten, die sich auf dem Gestell befinden.
  - Verschiedene Artikelvarianten stehen auf einem Gestell.
  - Nur gleiche Artikelvarianten stehen auf einem Gestell.
- **Fach:** Bezeichnung des Fachs.
- **Fifo-Datum:** Datum für die Gestellbuchung nach dem Fifo-Prinzip.
- **Menge:** Aktuelle Stückzahl der Artikel auf dem Lagergestell.
- **Buchung:** Artikelbestand, der gebucht wird.
- **Auftrag:** Auftragsnummer für die auftragsbezogene Gestellbuchung.
- **Position:** Nummer der Gestellposition im Gestelllager.
- **Buchungsstatus:** Status der Buchungen im Lager.

*Tab. F-8 Buchungsstatus des Gestelllagerausgangs*

| Buchungsstatus | Bedeutung |
| :--- | :--- |
| grau | Buchungsposition ist vom Prozess (Programm) gebucht worden. |
| rot | Buchungsposition ist vom Prozess (Programm) nicht oder noch nicht gebucht worden. |
| gelb | Gestelldaten wurden verändert: Bei der auftragsbezogenen Buchung wurde von diesem Gestell eine Menge oder Teilmenge für die Buchung verplant. |
| halb gelb / halb grau | Nachbearbeitung ist notwendig: Ein neuer Satz wurde angelegt, mit der verbleibenden Gestellmenge für das Unterteil der Auftragsposition. |

---

## Gestelllagerausgang – Umbuchung

**Buchung > Gestellausgang > Umbuchung**

*Abb. F-16 Gestelllagerausgang - Umbuchung*

In diesem Register können Sie die Artikel auf ein neues Gestell bzw. neues Fach umbuchen.

Sie können folgende Tastaturbefehle ausführen:

- Mit `<Strg>` + `<F8>` können Sie im ersten Feld zwischen dem Dialog Gestelllagereingang und Gestelllagerausgang wechseln.
- Mit `<F2>` können Sie zwischen den Registern Auftragsbezogen und Umbuchung umschalten.
- Mit `<F5>` können Sie in die variantenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.
- Mit `<Shift>` + `<F8>` können Sie eine Position auflösen.

**[Zurücksetzen]**
Verwirft die eingegebenen Änderungen.

### Kopfbereich
Im Kopfbereich müssen Sie entweder den Artikel und das Lager angeben oder das Gestell.
Die Felder sind an folgender Stelle beschrieben:
- "Gestelllagereingang" auf Seite F-1721

---

### Rumpfbereich

- **Variante:** Maßvariante des Artikels. Mit `<F9>` können Sie die Variantenauswahl aufrufen. Varianten eines Artikels werden nur angezeigt, wenn die Varianten im Stammdatenmodul angelegt sind.
- **Gestell:** Externe Gestellbezeichnung des Lagergestells.
- **G:** Artikelvarianten, die sich auf dem Gestell befinden.
  - Verschiedene Artikelvarianten stehen auf einem Gestell.
  - Nur gleiche Artikelvarianten stehen auf einem Gestell.
- **Fach:** Bezeichnung des Fachs.
- **Fifo-Datum:** Datum für die Gestellbuchung nach dem Fifo-Prinzip.
- **Menge:** Aktuelle Stückzahl der Artikel auf dem Lagergestell.
- **Buchung:** Artikelbestand, der gebucht wird.
- **Gestell neu:** Nummer des Gestells, auf das der Artikel umgebucht wird.
- **Fach neu:** Bezeichnung des Fachs, auf das das Gestell umgebucht wird.
- **Buchungsstatus:** Status der Buchungen im Lager.

*Tab. F-9 Buchungsstatus des Gestelllagerausgangs*

| Buchungsstatus | Bedeutung |
| :--- | :--- |
| grau | Buchungsposition ist vom Prozess (Programm) gebucht worden. |
| rot | Buchungsposition ist vom Prozess (Programm) nicht oder noch nicht gebucht worden. |
| gelb | Gestelldaten wurden verändert: Bei der auftragsbezogenen Buchung wurde von diesem Gestell eine Menge oder Teilmenge für die Buchung verplant. |
| halb gelb / halb grau | Nachbearbeitung ist notwendig: Ein neuer Satz wurde angelegt, mit der verbleibenden Gestellmenge für das Unterteil der Auftragsposition. |

---

## Lagerausgang (Auftragsbezogen)

**Buchung > Ausgang (Auftragsbezogen)**

*Abb. F-17 Lagerausgang (Auftragsbezogen)*

In diesem Dialog können Sie auftragsbezogene Lagerabgänge manuell buchen. In den Artikelstammdaten ist definiert, ob ein Artikel nur manuell gebucht werden kann.

Sie können folgende Tastaturbefehle ausführen:

- Mit `<F2>` können Sie sich die Spalte Termin für den Liefertermin der Position anzeigen lassen.
- Mit `<F3>` können Sie die Buchung auslösen.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.

### Kopfbereich

**Auftrag**
Auftragsnummer.

**Anfahrt**
Liefertermin, an dem der Auftrag beim Kunden angeliefert wird.

**Kunde**
Kundennummer und Kundenname.

**Erfasst am, von**
Datum der Auftragserfassung und Name des Erfassers.

**Gebucht am, von**
Datum der Lagerausgangsbuchung und Name des Mitarbeiters, der die Lagerausgangsbuchung gebucht hat.

### Rumpfbereich

- **Pos:** Nummer der Auftragsposition.
- **Artikel:** Artikelnummer.

---

- **Bezeichnung:** Artikelbezeichnung.
- **Variante:** Maßvariante der Position.
- **Gesamt:** Gesamtmenge pro Position.
- **Verbucht:** Menge der Position, die bereits abgebucht wurde.
- **Buchen:** Menge der Position, die vom Lager abgebucht werden soll.

Mit `<F2>` können Sie sich die Spalte Termin für den Liefertermin der Position anzeigen lassen.

- **Termin:** Liefertermin der Position.

---

## Buchungskorrektur – Übersicht

**Buchung > Korrektur**

*Abb. F-18 Buchungskorrektur – Übersicht*

In diesem Dialog können Sie die Suchkriterien festlegen, um sich die Buchungen anzeigen zu lassen und zu korrigieren.

Um Buchungen korrigieren zu können, müssen zuerst Lagerdaten durch das Lagerbuchungssystem angelegt worden sein. Sicherungs-Lagerdaten werden nur angelegt, wenn Zeitpunkte zur automatischen Speicherung der Lagerdaten definiert werden, z. B. der 15. eines jeden Monats. Fehlerhafte Buchungssätze dürfen nicht im Buchungssystem vorhanden sein.

Die Details der Übersicht können Sie sich in der Detailansicht anzeigen lassen.
- "Buchungskorrektur - Details" auf Seite F-1731

Sie können folgende Tastaturbefehle ausführen:

- Mit `<F5>` wechseln Sie zwischen der Übersicht und der Detailansicht der ausgewählten Position.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.

### Kopfbereich

**Artikel**
Artikelnummer und Artikelbezeichnung.

**Lager**
Lagernummer und Lagerbezeichnung.

**von Datum, bis Datum**
Zeitraum, für den Buchungen aufgelistet werden.

---

### Rumpfbereich

- **Variante:** Artikelvariante.
- **Farbe:** Farbvariante des Artikels.
- **Lieferant:** Lieferantennummer.
- **Menge:** Mengeneinheit des Artikels in der zu korrigierenden Buchung.
- **Anzahl:** Stückzahl der zu korrigierenden Buchung.
- **Preis:** Stückpreis der Variante.
- **Stat.:** Bezeichnung des Buchungsstatus, z. B. Lagereingang.
- **Datum:** Datum, an dem die Buchung korrigiert wurde.

---

## Buchungskorrektur – Details

**Buchung > Korrektur > Filtern > <F5>**

*Abb. F-19 Buchungskorrektur – Details*

In diesem Dialog werden die Details einer Buchungskorrektur aus der Übersicht angezeigt und korrigiert.

Sie können folgende Tastaturbefehle ausführen:

- Mit `<F5>` wechseln Sie zwischen der Übersicht und der Detailansicht der ausgewählten Position.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.

### Kopfbereich
Die Felder sind an folgender Stelle beschrieben:
- "Kopfbereich" auf Seite F-1729

### Rumpfbereich

**Kiste**
Kistennummer.

**Fach**
Bezeichnung des Fachs.

**Variante**
Artikelvariante.

**Farbe**
Farbvariante des Artikels.

**Lieferant**
Lieferantennummer.

**Auftrag**
Auftragsnummer, bei auftragsbezogenen Lagerbuchungen.

**Position**
Nummer der Auftragsposition.

---

**Menge**
Mengeneinheit des Artikels in der zu korrigierenden Buchung.

**Anzahl**
Stückzahl der zu korrigierenden Buchung.

**Preis**
Stückpreis der Variante.

**Status**
Bezeichnung des Buchungsstatus, z. B. Lagereingang.

**Datum**
Datum, an dem die Buchung korrigiert wurde.

---

# Stammdatenverwaltung

In den Stammdaten verwalten Sie den Lagerraum und die Bestandsgrenzen für Lagerartikel, z. B. legen Sie neue Lagerplätze im Lager an. Außerdem definieren Sie die Lagerartikel und deren Bestandsgrenzen.

In diesem Abschnitt sind folgende Dialoge erklärt:

- Lagerraumverwaltung
- Artikelstammdaten Lager

## Lagerraumverwaltung

**Stammdaten > Raum**

*Abb. F-20 Lagerraumverwaltung*

In diesem Dialog können Sie neue Lagerräume anlegen. Die festgelegte Zuordnung von Lagernummer, Lagerbezeichnung, Lagerart und Inventurart kann nach dem Speichern nicht mehr geändert werden. Für einen Lagerraum müssen Sie immer die Art des Lagers und der Inventur festlegen.

Mit `<Ende>` speichern Sie die Daten des Lagerraums.
Mit `<Pos1>` verwerfen Sie die Angaben.

### Feldbeschreibungen

**Lager**
Nummer und Bezeichnung des Lagers.
**Technische Info:** numerisches Feld, DB-Feld: `wlraum.lnr`
**Technische Info:** alphanumerisches Feld, DB-Feld: `wlraum.lbez`

**Kurzbez.**
Kurzbezeichnung des Lagers.
**Technische Info:** alphanumerisches Feld, DB-Feld: `wlraum.kurzbez`

**im Haus**
Nummer und Bezeichnung des Hauses oder Mandanten.
**Technische Info:** Toggle-Feld, DB-Feld: `wlraum.hnr`

**Inventurart**
Art der Bestandskontrolle.
- **Permanent** = Permanente Inventur.

---

- **Zyklisch** = Zyklische Inventur zum Bilanzstichtag.
  - "Inventur - Standardlager" auf Seite F-1738
  **Technische Info:** Toggle-Feld, DB-Feld: `wlraum.invart`

**Lagerart**
Art des Lagers:
- **Normallager** = Lager für alle Artikel ohne Restriktionen.
- **Kistenlager** = Lager für komplette Kisten. Angebrochene Kisten müssen aufgelöst und auf ein anderes Lager gebucht werden.
- **Fachlager** = Lager für alle Artikel mit zugewiesener Bezeichnung des Fachs.
- **Hochregallager** = Lager mit Lagerplätzen in Hochregalen.
- **Stapellager** = Lager für Scheiben mit einheitlichen Abmessungen.
- **Einzelblattkistenlager** = Lager zur Buchung einzelner Glasblätter in Kisten.
- **Gestelllager** = Lager mit Lagerplätzen auf Gestellen.
  **Technische Info:** Toggle-Feld, DB-Feld: `wlraum.lagart`

**Schnittstelle**
Angabe der Softwareschnittstelle. Auswahl für ein kundenseitig angeschlossenes Lagerverwaltungssystem.
**Technische Info:** Toggle-Feld, DB-Feld: `wlraum.interface`

**Größe**
Lagerfläche in Mengeneinheit (Quadratmeter).
**Technische Info:** numerisches Feld, DB-Feld: `wlraum.groesse`

**Fixe Kosten**
Fixe Kosten der Lagerfläche in Eigenwährung pro Quadratmeter, z. B., Mietkosten.
**Technische Info:** numerisches Feld, DB-Feld: `wlraum.kofix`

**Variable Kosten**
Variable Kosten der Lagerfläche in Eigenwährung pro Quadratmeter, z. B. Stromkosten, Heizkosten.
**Technische Info:** numerisches Feld, DB-Feld: `wlraum.kovar`

**WE-Lager**
Nummer des zugeordneten Wareneingangslagers. Diese Angabe in den Stammdaten sind nur bei aktivierter Portallager-Logik relevant.
**Technische Info:** numerisches Feld, DB-Feld: `wlraum.welnr`

---

## Artikelstammdaten Lager

**Stammdaten > Artikel**

*Abb. F-21 Artikelstammdaten Lager*

In diesem Dialog können Sie die Bestandsgrenzen der Lagerartikel festlegen. Die Bestandsgrenzen der Lagerartikel werden durch den Minimalbestand, Alarmbestand und Maximalbestand festgelegt.

Sie können folgende Tastaturbefehle ausführen:

- Wenn Sie sich in einer Spalte im Rumpfbereich befinden, können Sie mit `<Ende>` die Festlegung der Bestandsgrenzen speichern.
- Mit `<F5>` können Sie in den Fußbereich wechseln.

### Kopfbereich

**Artikel**
Artikelnummer des lagerführenden Artikel. Nach der Auswahl wird die Artikelbezeichnung im Klartext angezeigt.
**Technische Info:** numerisches Feld, `<F9>`, DB-Feld: `wls.artnr`

**Lager**
Lagernummer. Nach der Auswahl wird die Lagerbezeichnung im Klartext angezeigt.
**Technische Info:** numerisches Feld, `<F9>` DB-Feld: `wls.Inr`

**Bestellvariante**
Artikelvariante für Nachbestellungen.
**Technische Info:** numerisches Feld, DB-Feld: `wls.stdbitnr`

**Bestellfarbe**
Farbvariante des Artikels für Nachbestellungen.
**Technische Info:** numerisches Feld, DB-Feld: `wls.stdfarbnr`

---

> **Maß- oder Farbvariante?**
> Variantenart des Artikels wird aus Artikelstammdaten übernommen und lagerintern in dem Datenbank-Feld `wls.varart` vermerkt. Es sind folgende Varianten möglich:
> - `wls.varart = 0` - keine Variante
> - `wls.varart = 1` - Maßvariante
> - `wls.varart = 2` - Farbvariante
> - `wls.varart = 3` - Doppelvariante (Maß- und Farbangaben sind zulässig)

### Bestandsgrenzen

**Mindestbestand**
Minimal zulässiger Lagerbestand des Artikels, um Produktionsengpässe zu verhindern.
**Technische Info:** numerisches Feld, DB-Feld: `wls.m_best`

**Alarmbestand**
Artikelbestand, bei dem ein Bestellvorschlag für Einkauf ausgelöst wird. Durch Alarmbestände können Sie eine Unterdeckung des Lagers verhindern.
**Technische Info:** numerisches Feld, DB-Feld: `wls.a_best`

**Maximalbestand**
Maximal zulässiger Lagerbestand des Artikels, um Lagerkosten zu minimieren.
**Technische Info:** numerisches Feld, DB-Feld: `wls.o_best`

> **Automatische Bestellvorschläge durch das Lager**
> Wenn der definierte Alarm- oder Mindestbestand unterschritten wird, werden durch das Lager automatisch Bestellvorschläge im Einkauf angelegt. Bei der Installation wird festgelegt, ob der Alarm- oder der Mindestbestand den Bestellvorschlag auslöst.
> Die Menge im Bestellvorschlag richtet sich nach dem definierten Maximalbestand. Diese Bestellvorschläge werden vom Einkauf freigeschaltet und in Bestellungen überführt.

### Rumpfbereich
Im Dialogrumpf lesen Sie abweichende Bestände variantengenau an. Mit `<F2>` können Sie die Angaben in Stückzahl oder in Artikel-Mengeneinheit machen.

**Variante**
Maßvariante des Artikels.
**Technische Info:** numerisches Feld, DB-Feld: `wlsv.massbez`

**Farbe**
Farbvariante des Artikels.
**Technische Info:** numerisches Feld, DB-Feld: `wlsv.farbbez`

> **Variantenbezogene Lagerbestände**
> Variantenbezogene Lagerbeständen im Lager-Artikelstammdaten werden pro Variante in der Datenbanktabelle w/sv geführt.

---

### Fußbereich

**Bemerkung**
Mit `<F5>` können Sie in das Textfeld für Bemerkungen zur Artikelvariante wechseln.
**Technische Info:** numerisches Feld, DB-Feld: `wlsv.bemerk`

---

# Inventurverwaltung

Mit der Inventurverwaltung gleichen Sie die gezählten Bestände mit den vom System gebuchten Beständen ab und korrigieren die Zahlen entsprechend im System.

In diesem Abschnitt sind folgende Dialoge erklärt:

- Inventur - Standardlager
- Inventur - Kistenlager
- Inventur - Fachlager
- Inventur - Stapellager
- Inventur - Gestelllager

## Inventur – Standardlager

**Inventur > Lager**

*Abb. F-22 Inventur-Standardlager*

In diesem Dialog können Sie die Inventur für das Standardlager durchführen und abschließen.

---

> **Lager in Inventur**
> Wenn ein Lager für die Inventur freigeschaltet wird, wird eine Kopie des Lagers mit negativen Lagernummern erzeugt, das sogenannte Inventurlager. In dieses Inventurlager werden die gezählten Bestände eingetragen.
> Während der Inventur werden die Eingänge und Ausgänge weiterhin auf die positive Lagernummer gebucht. Damit ist gewährleistet, dass während der Inventur Eingangs- und Ausgangsbuchungen für dieses Lager erfasst werden können.
> Nach einem Inventurabschluss werden die geänderten Bestände aus dem Inventurlager mit den Eingangs- und Ausgangsbuchungen aktualisiert, die während der Inventur erfasst wurden.

Die Dialoge für die Inventur in den verschiedenen Lagerarten sind identisch aufgebaut und werden daher für das Standardlager beschrieben. Die Beschreibung gilt daher gleichermaßen für:

- Kistenlager
- Fachlager
- Stapellager
- Gestelllager

Sie können folgende Tastaturbefehle ausführen:

- Mit `<F2>` können Sie die Anzeige zwischen Artikel in Stückzahl und Artikel in Mengeneinheit umschalten.
- Mit `<Shift>` + `<F8>` können Sie die Inventur abschließen.
- Mit `<Shift>` + `<F12>` können Sie die Inventur verwerfen.

### Kopfbereich

**von Artikel, bis Artikel**
Wertebereich der Artikelnummern, um die Inventurliste zu filtern.
**Technische Info:** numerisches Feld, DB-Feld: `wlbv.artnr`

**von Lager, bis Lager**
Wertebereich der Lagernummern, um die Inventurliste zu filtern:
- Wenn Sie in den Feldern von Lager, bis Lager dieselbe Lagernummer eingeben, wird das Lager für die Inventur freigeschaltet.
- Wenn Sie in den Feldern von Lager, bis Lager einen Bereich von Lagernummern eingeben, werden die Datensätze zur Ansicht in den Dialog geladen.
**Technische Info:** numerisches Feld, DB-Feld: `wlbv.Inr`

**Inventur/Bewertung vom**
Zeitpunkt an dem die Inventur durchgeführt wurde (Unixzeit).
**Technische Info:** numerisches Feld, DB-Feld: `wlinvv.ivzeit`

### Rumpfbereich
Folgende Felder werden angezeigt:

- **Artikel:** Artikelnummer.

---

- **Technische Info:** Anzeige-Feld, DB-Feld: `wlinvv.artnr`
- **Lager:** Lagernummer.
  **Technische Info:** Anzeige-Feld, DB-Feld: `wlinvv.Inr`
- **Variante:** Maßvariante der Position.
  **Technische Info:** Anzeige-Feld, DB-Feld: `wlinvv.massbez` oder `wlinvv.farbbez`
- **S:** Storno des Artikels.
  - N = Kein Storno des Artikels.
  - J = Artikel wurde storniert.
  **Technische Info:** Anzeige-Feld, DB-Feld: `artikel.still`
- **Soll-Anzahl:** Anzeige für Soll-Stückzahl des Artikels im Lager.
  **Technische Info:** Anzeige-Feld, DB-Feld: `wlinvv.g_best`
- **Ist-Anzahl:** Eingabe für Ist-Stückzahl des gezählten Artikels im Lager.
  **Technische Info:** numerisches Feld, DB-Feld: `wlinvv.g_anz`
- **Preis:** Gesamtpreis des Ist-Bestands des Artikels.
  **Technische Info:** Anzeige-Feld, ohne DB-Feld (Gesamtpreis wird zur Laufzeit errechnet)
- **ME:** Durchschnittspreises pro Mengeneinheit für den Ist-Bestand, z. B. 75,00 € pro qm.
  **Technische Info:** Anzeige-Feld, ohne DB-Feld (Durchschnittspreis wird zur Laufzeit errechnet)
- **Bemerkung:** Inventurvermerk für statistische Auswertungen.
  **Technische Info:** alphanumerisches Feld, DB-Feld `wlbv.bemerk`

Mit `<F2>` können Sie die folgenden Spalten anzeigen lassen:

- **Soll-Bestand:** Anzeige für Soll-Wert der Mengeneinheit des Artikelbestands im Lager.
  **Technische Info:** Anzeige-Feld, DB-Feld: `wlinvv.g_best`
- **Ist-Bestand:** Eingabe für Ist-Wert der gezählten Mengeneinheit des Artikelbestands im Lager.
  **Technische Info:** numerisches Feld, DB-Feld: `wlinvv.g_anz`

### Fußbereich

**Artikel**
Artikelbezeichnung des ausgewählten Artikels.
**Technische Info:** Anzeige-Feld

**D-Preis**
Durchschnittspreis des ausgewählten Artikels für den Ist-Bestand.
**Technische Info:** Anzeige-Feld

---

**G-Preis**
Gesamtpreis des ausgewählten Artikels für den Ist-Bestand.
**Technische Info:** Anzeige-Feld

**Lager**
Lagerbezeichnung des ausgewählten Lagers.
**Technische Info:** Anzeige-Feld

**LIFO-Preis**
Artikelpreis im Lager, wenn nach der LIFO-Buchungsmethode abgebucht und berechnet wird.
**Technische Info:** Anzeige-Feld

**FIFO-Preis**
Artikelpreis im Lager, wenn nach der FIFO-Buchungsmethode abgebucht und berechnet wird.
**Technische Info:** Anzeige-Feld

> **Inventur ohne Sollbestandsanzeige**
> Über eine Systemeinstellung ist möglich ein neues Inventurverfahren aktiviert werden. Dieses Verfahrensoll zu einem genaueren Zählverhalten führen, da die Sollwerte unbekannt sind. Somit können diese nicht einfach übernommen werden.
>
> Bei dieser Konfiguration wird der Sollbestand nicht angezeigt und der einzugebende Istbestand ist beim Öffnen der Inventur leer. Jetzt muss zu jedem Satz der gezählte Bestand eingetragen werden. Auch wenn kein Bestand vorhanden ist, muss eine 0 hinterlegt werden. Erst wenn alle Zeilen mit Werten gefüllt sind, kann die Inventur abgeschlossen werden.

---

## Inventur – Kistenlager

**Inventur > Kistenlager**

*Abb. F-23 Inventur-Kistenlager*

In diesem Dialog können Sie die Inventur für das Kistenlager durchführen und abschließen.

Die Beschreibung für die Felder finden Sie an folgender Stelle:
- "Kopfbereich" auf Seite F-1739

### Rumpfbereich

- **Kiste:** Kistennummer.
- **Lager:** Lagernummer.
- **Artikel:** Artikelnummer.
- **Variante:** Maßvariante der Position.
- **S:** Storno des Artikels.
  - N = Kein Storno des Artikels.
  - J = Artikel wurde storniert.
- **Menge:** Gesamte Scheibenfläche in einer Kiste.

---

- **Anzahl:** Anzahl der Scheiben in der Kiste.
- **VA:** Kennzeichen der Verpackungsart.
- **Liefnr.:** Lieferantennummer.
- **ME:** Durchschnittspreis pro Mengeneinheit für den Ist-Bestand, z. B. 75,00 € pro qm.
- **Bemerkung:** Inventurvermerk für statistische Auswertungen.

### Fußbereich

**Artikel**
Artikelbezeichnung.

**Lager**
Lagerbezeichnung.

**Kiste**
Kistenbezeichnung.

**Verpackart**
Kennzeichen der Verpackungsart.

**Lieferant**
Lieferantenname.

---

## Inventur – Fachlager

**Inventur > Fachlager**

*Abb. F-24 Inventur-Fachlager*

In diesem Dialog können Sie die Inventur für das Fachlager durchführen und abschließen.

Die Beschreibung für die Felder finden Sie an folgender Stelle:
- "Kopfbereich" auf Seite F-1739
- "Fußbereich" auf Seite F-1740

### Rumpfbereich

- **Lager:** Lagernummer.
- **Artikel:** Artikelnummer.
- **Variante:** Maßvariante der Position.
- **S:** Storno des Artikels.
  - N = Kein Storno des Artikels.
  - J = Artikel wurde storniert.
- **Fach:** Bezeichnung des Fachs.
- **Menge:** Menge des Artikels in Mengeneinheit.

---

- **Anzahl:** Eingabe für Ist-Bestand des gezählten Artikelbestands im Stapel.
- **Preis:** Gesamtpreis des Ist-Bestands des Artikels.
- **Bemerkung:** Inventurvermerk für statistische Auswertungen.

## Inventur – Stapellager

**Inventur > Stapellager**

*Abb. F-25 Inventur-Stapellager*

In diesem Dialog können Sie die Inventur für das Stapellager durchführen und abschließen.

Die Beschreibung für die Felder finden Sie an folgender Stelle:
- "Kopfbereich" auf Seite F-1739
- "Fußbereich" auf Seite F-1740

### Rumpfbereich

- **Lager:** Lagernummer.
- **Artikel:** Artikelnummer.
- **Variante:** Maßvariante der Position.

---

- **S:** Storno des Artikels.
  - N = Kein Storno des Artikels.
  - J = Artikel wurde storniert.
- **Stapel:** Stapelnummer.
- **Bezeichnung:** Bezeichnung des Stapels.
- **Anzahl:** Eingabe für Ist-Bestand des gezählten Artikelbestands im Stapel.
- **Preis:** Gesamtpreis des Ist-Bestands des Artikels.
- **Bemerkung:** Inventurvermerk für statistische Auswertungen.

## Inventur – Gestelllager

**Inventur > Gestelllager**

**Zu Dialogbeschreibung:**
- Bestandsbewertung - Gestelllager

*Abb. F-26 Inventur-Gestelllager*

In diesem Dialog können Sie die Inventur für das Gestelllager durchführen und abschließen.

---

Die Beschreibung für die Felder finden Sie an folgender Stelle:
- "Kopfbereich" auf Seite F-1739
- "Fußbereich" auf Seite F-1740

### Rumpfbereich

- **Lager:** Lagernummer.
- **Artikel:** Artikelnummer.
- **Variante:** Maßvariante der Position.
- **S:** Storno des Artikels.
  - N = Kein Storno des Artikels.
  - J = Artikel wurde storniert.
- **Soll-Anzahl:** Soll-Bestand des Artikels.
- **Ist-Anzahl:** Eingabe für Ist-Bestand des gezählten Artikelbestands im Stapel.
- **Preis:** Gesamtpreis des Ist-Bestands des Artikels.
- **ME:** Menge.
- **Bemerkung:** Inventurvermerk für statistische Auswertungen.

Mit `<F2>` können Sie die folgenden Spalten anzeigen lassen:

- **G:** Artikelvarianten, die sich auf dem Gestell befinden.
  - Verschiedene Artikelvarianten stehen auf einem Gestell.
  - Nur gleiche Artikelvarianten stehen auf einem Gestell.
- **Gestell:** Bezeichnung des Gestells.
- **Fach:** Bezeichnung des Fachs.
- **Soll:** Soll-Bestand des Artikels.
- **Ist:** Ist-Bestand des Artikels.
- **FIFO-Datum:** Datum für die Gestellbuchung nach dem Fifo-Prinzip.
- **Status:** Status der Buchungen im Gestelllager.

---

*Tab. F-10 Buchungsstatus im Gestelllager*

| Buchungsstatus | Bedeutung |
| :--- | :--- |
| grau | Buchungsposition ist vom Prozess (Programm) gebucht worden. |
| rot | Buchungsposition ist vom Prozess (Programm) nicht oder noch nicht gebucht worden. |
| gelb | Buchungsposition ist geändert worden. |
| halb gelb / halb grau | Buchungsposition ist ein Unterteil eines Auftrags. Buchungsposition muss auf ein anderes Lager gebucht werden, z. B. Fachlager. |

---

# Bewertung

In der Bewertung können Sie die wertmäßigen Verluste des Umlaufvermögens innerhalb einer Inventur bearbeiten. Für die Inventur können die Gegenstände des Umlaufvermögens mit dem Niederstwertprinzip (Anschaffungs-, Herstellungs- oder Tageswert) in der Schlussbilanz eingesetzt werden.

In diesem Abschnitt sind folgende Dialoge erklärt:

- Bestandsbewertung - Standardlager
- Bestandsbewertung - Kistenlager
- Bestandsbewertung - Fachlager
- Bestandsbewertung - Stapellager
- Bestandsbewertung – Gestelllager

## Bestandsbewertung – Standardlager

**Bewertung > Lager**

*Abb. F-27 Bestandsbewertung - Standardlager*

In diesem Dialog können Sie eine wertmäßige Korrektur des Artikelbestands innerhalb einer Inventur durchführen, z. B. wenn die Werte eines Lagerartikels von den aktuellen Werten abweichen.

---

Die Dialoge für die Bestandsbewertung in den verschiedenen Lagerarten sind identisch aufgebaut und werden daher für das Standardlager beschrieben. Die Beschreibung gilt daher gleichermaßen für:

- Kistenlager
- Fachlager
- Stapellager
- Gestelllager

Sie können folgende Tastaturbefehle ausführen:

- Mit `<F2>` können Sie die Anzeige zwischen Artikel in Stückzahl und Artikel in Mengeneinheit umschalten. Die Funktion gilt nur für das Standardlager.
- Mit `<Ende>` können Sie die wertmäßige Korrektur abschließen.

### Kopfbereich

**von Artikel, bis Artikel**
Wertebereich der Artikelnummern um die Liste zu filtern.

**von Lager, bis Lager**
Eingabe der Lagernummern:
- Wenn Sie in den Feldern von Lager, bis Lager dieselbe Lagernummer eingeben, wird das Lager für die Bestandsbewertung freigeschaltet.
- Wenn Sie in den Feldern von Lager, bis Lager einen Bereich von Lagernummern eingeben, werden die Datensätze zur Ansicht in den Dialog geladen.

**Inventur/Bewertung vom**
Datum der Bestandsbewertung.

### Rumpfbereich
Folgende Spalten werden angezeigt:

- **Lager:** Lagernummer.
- **Artikel:** Artikelnummer.
- **Variante:** Maßvariante der Position.
- **S:** Storno des Artikels.
  - N = Kein Storno des Artikels.
  - J = Artikel wurde storniert.
- **Soll-Anzahl:** Anzeige für Soll-Stückzahl des Artikels im Lager.
- **Ist-Anzahl:** Anzeige für Ist-Stückzahl des gezählten Artikels im Lager.
- **Preis:** Eingabe für den Gesamtpreis des Ist-Bestands des Artikels.

---

- **ME:** Eingabe des Durchschnittspreises pro Mengeneinheit für den Ist-Bestand, z. B. 75,00 € pro qm.
- **Bemerkung:** Inventurvermerk für statistische Auswertungen.

Mit `<F2>` können Sie die folgenden Spalten anzeigen lassen:

- **Soll-Bestand:** Anzeige für Soll-Wert der Mengeneinheit des Artikelbestands im Lager.
- **Ist-Bestand:** Anzeige für Ist-Wert der gezählten Mengeneinheit des Artikelbestands im Lager.

### Fußbereich

**Artikel**
Artikelbezeichnung des ausgewählten Artikels.

**D-Preis**
Durchschnittspreis des ausgewählten Artikels für den Ist-Bestand.

**G-Preis**
Gesamtpreis des ausgewählten Artikels für den Ist-Bestand.

**Lager**
Lagerbezeichnung des ausgewählten Lagers.

**LIFO-Preis**
Artikelpreis im Lager, wenn nach der LIFO-Buchungsmethode abgebucht und berechnet wird.

**FIFO-Preis**
Artikelpreis im Lager, wenn nach der FIFO-Buchungsmethode abgebucht und berechnet wird.

---

## Bestandsbewertung – Kistenlager

**Bewertung > Kistenlager**

*Abb. F-28 Bestandsbewertung-Kistenlager*

In diesem Dialog können Sie eine wertmäßige Korrektur des Artikelbestands innerhalb einer Inventur durchführen, z. B. wenn die Werte von Kisten von den aktuellen Werten abweichen.

Die Bestandsbewertung darf nur innerhalb eines einzelnen Lagers ausgeführt werden.

Die Felder und Spalten sind an folgender Stelle beschrieben:
- "Bestandsbewertung - Standardlager" auf Seite F-1749

---

## Bestandsbewertung – Fachlager

**Bewertung > Fachlager**

*Abb. F-29 Bestandsbewertung-Fachlager*

In diesem Dialog können Sie eine wertmäßige Korrektur des Artikelbestands innerhalb einer Inventur durchführen, z. B. wenn die Werte von Lagerartikeln eines Faches von den aktuellen Werten abweichen.

Die Bestandsbewertung darf nur innerhalb eines einzelnen Lagers ausgeführt werden.

Die Felder und Spalten sind an folgender Stelle beschrieben:
- "Bestandsbewertung - Standardlager" auf Seite F-1749

---

## Bestandsbewertung – Stapellager

**Bewertung > Stapellager**

*Abb. F-30 Bestandsbewertung-Stapellager*

In diesem Dialog können Sie eine wertmäßige Korrektur des Artikelbestands innerhalb einer Inventur durchführen, z. B. wenn die Werte von Artikeln eines Stapels von den aktuellen Werten abweichen.

Die Bestandsbewertung darf nur innerhalb eines einzelnen Lagers ausgeführt werden.

Die Felder und Spalten sind an folgender Stelle beschrieben:
- "Bestandsbewertung - Standardlager" auf Seite F-1749

---

## Bestandsbewertung – Gestelllager

**Bewertung > Gestelllager**

*Abb. F-31 Bestandsbewertung-Gestelllager*

In diesem Dialog können Sie eine wertmäßige Korrektur des Artikelbestands innerhalb einer Inventur durchführen, z. B. wenn die Werte von Artikeln eines Gestells von den aktuellen Werten abweichen.

Die Bestandsbewertung darf nur innerhalb eines einzelnen Lagers ausgeführt werden.

Die Felder und Spalten sind an folgender Stelle beschrieben:
- "Bestandsbewertung - Standardlager" auf Seite F-1749

Sie können folgenden Tastaturbefehl ausführen:

Mit `<F2>` können Sie die Anzeige für Artikel von Stückzahl zu Mengeneinheit umschalten. Die Funktion gilt nur für das Gestelllager.

---

# Informationssystem

Im Informationssystem können Sie die Lagerdaten überwachen. Über das Informationssystem können Sie die Suchfunktionen ausführen.

In diesem Abschnitt sind folgende Dialoge erklärt:

- Info-Lager-Artikel
- Info-Lager-Varianten
- Info-Lager-Fächer
- Info-Lager-Gestelle
- Info-Lager-Stapel
- Info-Lager-Blätter
- Info-Lager-Historie
- Aufträge/Bestellungen
- Buchungsstatus
- Lagerinformationen – Pickliste
- Lagerinformationen – Trefferliste
- LVR-Status
- Reichweite - Bestandsprognose
- Reichweite - Trefferliste
- Dispositiver Bestand
- Bestandsprognose

Zusätzlich können Sie sich individuelle Informationsübersichten mittels SQL-Abfragen zusammenstellen.

---

## Info-Lager-Artikel

**Infosystem > Artikel**

In diesem Dialog können Sie sich die Lagerbestände oder Artikelbestände anzeigen lassen.

Zu diesem Dialog werden folgende Unterdialoge angezeigt:

- Info-Lager-Artikel – Filterdialog
- Info-Lager-Artikel – Trefferliste
- Info-Lager-Artikel – Trefferliste-Details

### Info-Lager-Artikel – Filterdialog

**Infosystem > Artikel**

*Abb. F-32 Info-Lager-Artikel – Filterdialog*

In diesem Dialog können Sie die Suchkriterien festlegen, um sich die Lagerbestände oder Artikelbestände anzeigen zu lassen. Die Ergebnisse der Suche können Sie sich in der Trefferliste und in der Detailansicht anzeigen lassen.

- "Info-Lager-Artikel – Trefferliste" auf Seite F-1758
- "Info-Lager-Artikel - Trefferliste-Details" auf Seite F-1759

**Artikel**
Artikelnummer.

**Lager**
Lagernummer.

**Menge**
Artikel in Mengeneinheit.

**Gesamtpreis**
Gesamtpreis des Artikelbestands im ausgewählten Lager.

**Durchschnittspreis**
Durchschnittlicher Preis pro Mengeneinheit des Artikels.

**Letzte Änderung**
Datum, an dem der Buchungssatz zuletzt gebucht wurde.

---

## Info-Lager-Artikel – Trefferliste

**Infosystem > Artikel > Filtern**

*Abb. F-33 Info-Lager-Artikel – Trefferliste*

In diesem Dialog werden die Ergebnisse der Suche nach Lagerartikeln angezeigt.

Details zu den Lagerartikeln werden in der Detailansicht angezeigt.
- "Info-Lager-Artikel - Trefferliste-Details" auf Seite F-1759

Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

### Trefferliste
Folgende Spalten werden angezeigt:

- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Bestand:** Lagerbestand des Artikels in Mengeneinheit.
- **G-Preis:** Gesamtpreis des Artikels.
- **D-Preis:** Durchschnittspreis pro Mengeneinheit.
- **H-Preis:** Höchster Einkaufspreis pro Mengeneinheit.
- **N-Preis:** Niedrigster Einkaufspreis pro Mengeneinheit.

---

## Info-Lager-Artikel – Trefferliste-Details

**Infosystem > Artikel > Filtern > <F5>**

*Abb. F-34 Info-Lager-Artikel – Trefferliste-Details*

In diesem Dialog werden die Details zur Trefferliste der Lagerartikel angezeigt.
Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

### Details

**Artikel**
Artikelnummer und Artikelbezeichnung.

**Lager**
Lagernummer.

**Bestand**
Lagerbestand des Artikels in Mengeneinheit.

**Mindestbestand**
Minimalbestand des Artikels auf Lager.

**Alarmbestand**
Alarmbestand des Artikels auf Lager.

**Bestandobergrenze**
Maximalbestand des Artikels auf Lager.

**Höchstbestand**
Maximalstückzahl des Artikels auf Lager, seit der letzten Inventur.

**Niedrigstbestand**
Minimalstückzahl des Artikels auf Lager, seit der letzten Inventur.

**D-Bestand**
Durchschnittlicher Lagerbestand des Artikels, seit der letzten Inventur.

**D-Verbrauch**
Durchschnittliche Lagerabbuchung des Artikels, seit der letzten Inventur.

---

**Gesamtpreis**
Gesamtpreis des Artikels.

**D-Preis**
Durchschnittspreis pro Mengeneinheit.

**Höchstpreis**
Höchster Einkaufspreis des Artikels.

**Niedrigstpreis**
Niedrigster Einkaufspreis des Artikels.

**LIFO-Gesamtpreis**
Gesamtpreis der Artikelvariante im Lager, wenn nach der LIFO-Buchungsmethode abgebucht und berechnet wird.

**FIFO-Gesamtpreis**
Gesamtpreis der Artikelvariante im Lager, wenn nach der FIFO-Buchungsmethode abgebucht und berechnet wird.

**Letzte Änderung am, von**
Datum, an dem der Buchungssatz gebucht wurde und Name des Anwenders, der die Buchung ausgeführt hat.

---

## Info-Lager-Varianten

**Infosystem > Variante**

In diesem Dialog können Sie sich die Informationen zu den Artikelvarianten nach ausgewählten Kriterien anzeigen lassen.

Zu diesem Dialog werden folgende Unterdialoge angezeigt:

- Info-Lager-Varianten – Filterdialog
- Info-Lager-Varianten – Trefferliste
- Info-Lager-Varianten - Trefferliste-Details

### Info-Lager-Varianten – Filterdialog

**Infosystem > Variante**

*Abb. F-35 Info-Lager-Varianten – Filterdialog*

In diesem Dialog können Sie die Informationen zu den Artikelvarianten nach ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste angezeigt. Die Details können Sie in der Detailansicht einsehen.

- "Info-Lager-Varianten - Trefferliste" auf Seite F-1762
- "Info-Lager-Varianten - Trefferliste-Details" auf Seite F-1763

**Artikel**
Artikelnummer.

**Lager**
Lagernummer.

**Variante**
Maßvariante des Artikels in der Kiste.

**Farbe**
Farbvariante des Artikels.

**Kiste**
Kistennummer.

**Kistenbezeichnung**
Bezeichnung der Kiste.

**Letzte Änderung**
Datum, an dem der Buchungssatz gebucht wurde.

**Menge**
Artikel in Mengeneinheit.

---

**Anzahl**
Stückzahl des Artikels.

**Gesamtpreis**
Gesamtpreis des Artikelbestands.

**Durchschnittspreis**
Durchschnittlicher Preis pro Mengeneinheit des Artikels.

### Info-Lager-Varianten – Trefferliste

**Infosystem > Variante > Filtern**

*Abb. F-36 Info-Lager-Varianten – Trefferliste*

In diesem Dialog können Sie die Informationen zu den Artikelvarianten nach ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste angezeigt. Die Details können Sie in der Detailansicht einsehen.

- "Info-Lager-Varianten - Trefferliste-Details" auf Seite F-1763

Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

#### Trefferliste

- **Artikel:** Artikelnummer.
- **Bezeichnung:** Artikelbezeichnung.
- **Lager:** Lagernummer.

---

- **Kiste:** Kistennummer.
- **Variante:** Maßvariante des Artikels in der Kiste.
- **Farbe:** Farbvariante des Artikels.
- **Anzahl:** Stückzahl des Artikels.
- **Bestand:** Artikelbestand in Mengeneinheit.
- **Netto-ME:** Netto-Menge pro Kiste in Mengeneinheit des Artikels.
- **Preis:** Gesamtpreis des Artikels.

### Info-Lager-Varianten – Trefferliste-Details

**Infosystem > Variante > Filtern > <F5>**

*Abb. F-37 Info-Lager-Varianten – Trefferliste-Details*

In diesem Dialog werden die Details zur Trefferliste der Artikelvarianten angezeigt.

Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

#### Details

**Artikel**
Artikelnummer und Artikelbezeichnung.

**Lager**
Lagernummer.

**Kiste**
Kistennummer und Kistenbezeichnung.

**Variante**
Abmessungen der Variante.

---

**Farbe**
Farbvariante des Artikels.

**Anzahl**
Stückzahl des Artikels.

**Bestand**
Artikelbestand in Mengeneinheit.

**Netto Menge**
Netto-Menge pro Kiste in Mengeneinheit des Artikels.

**Mindestbestand**
Minimalbestand des Artikels auf Lager.

**Alarmbestand**
Alarmbestand des Artikels auf Lager.

**Bestandobergrenze**
Maximalbestand des Artikels auf Lager.

**Höchstbestand**
Maximalstückzahl des Artikels auf Lager, seit der letzten Inventur.

**Niedrigstbestand**
Minimalstückzahl des Artikels auf Lager, seit der letzten Inventur.

**D-Bestand**
Durchschnittlicher Lagerbestand des Artikels, seit der letzten Inventur.

**D-Verbrauch**
Durchschnittliche Lagerabbuchung des Artikels, seit der letzten Inventur.

**Gesamtpreis**
Gesamtpreis des Artikels.

**D-Preis**
Durchschnittspreis pro Mengeneinheit.

**Höchstpreis**
Höchster Einkaufspreis des Artikels.

**Niedrigstpreis**
Niedrigster Einkaufspreis des Artikels.

**LIFO-Gesamtpreis**
Gesamtpreis der Artikelvariante im Lager, wenn nach der LIFO-Buchungsmethode abgebucht und berechnet wird.

**FIFO-Gesamtpreis**
Gesamtpreis der Artikelvariante im Lager, wenn nach der FIFO-Buchungsmethode abgebucht und berechnet wird.

**Letzte Änderung am, von**
Datum, an dem der Buchungssatz gebucht wurde und Name des Anwenders, der die Buchung ausgeführt hat.

---

## Info-Lager-Fächer

**Infosystem > Fach**

In diesem Dialog können Sie sich die Informationen zu den Lagerfächern anzeigen lassen.

Zu diesem Dialog werden folgende Unterdialoge angezeigt:

- Info-Lager-Fächer – Filterdialog
- Info-Lager-Fächer - Trefferliste
- Info-Lager-Fächer - Trefferliste-Details

### Info-Lager-Fächer – Filterdialog

**Infosystem > Fach**

*Abb. F-38 Info-Lager-Fächer – Filterdialog*

In diesem Dialog können Sie die Informationen zu den Lagerfächern nach ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste angezeigt. Die Details können Sie in der Detailansicht einsehen.

- "Info-Lager-Fächer - Trefferliste" auf Seite F-1766
- "Info-Lager-Fächer - Trefferliste-Details" auf Seite F-1767

**Artikel**
Artikelnummer.

**Lager**
Lagernummer.

**Fach**
Bezeichnung des Fachs.

**Variante**
Abmessungen der Variante.

**Farbe**
Farbvariante des Artikels.

**Datum**
Datum, an dem der Buchungssatz gebucht wurde.

**Anzahl**
Stückzahl des Artikels.

**Menge**
Artikel in Mengeneinheit.

---

## Info-Lager-Fächer – Trefferliste

**Infosystem > Fach > Filtern**

*Abb. F-39 Info-Lager-Fächer – Trefferliste*

In diesem Dialog werden die Ergebnisse der Suche nach Lagerfächern angezeigt. Die Details können Sie in der Detailansicht einsehen.

- "Info-Lager-Artikel - Trefferliste-Details" auf Seite F-1759

Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

### Trefferliste

- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Fach:** Bezeichnung des Fachs.
- **Variante:** Abmessungen der Variante.
- **Menge:** Artikel in Mengeneinheit.
- **Stück:** Stückzahl des Artikels.
- **Preis:** Gesamtpreis des Artikels.
- **Datum:** Datum, an dem der Buchungssatz gebucht wurde.

---

## Info-Lager-Fächer – Trefferliste-Details

**Infosystem > Fach > Filtern > <F5>**

*Abb. F-40 Info-Lager-Fächer – Trefferliste-Details*

In diesem Dialog werden die Details zur Trefferliste der Lagerfächer angezeigt.

Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

### Details

**Artikel**
Artikelnummer.

**Lager**
Lagernummer.

**Fach**
Bezeichnung des Fachs.

**Variante**
Abmessungen der Variante.

**Farbe**
Farbvariante des Artikels.

**Menge**
Artikel in Mengeneinheit.

**Stück**
Stückzahl des Artikels.

**Preis**
Gesamtpreis des Artikels.

---

## Info-Lager-Gestelle

**Infosystem > Gestell**

In diesem Dialog können Sie sich die Informationen zu den Lagergestellen anzeigen lassen.

Zu diesem Dialog werden folgende Unterdialoge angezeigt:

- Info-Lager-Gestelle - Filterdialog
- Info-Lager-Gestelle – Trefferliste-Allgemein
- Info-Lager-Gestelle - Trefferliste-Details

### Info-Lager-Gestelle – Filterdialog

**Infosystem > Gestell**

*Abb. F-41 Info-Lager-Gestelle - Filterdialog*

In diesem Dialog können Sie die Informationen zu den Lagergestellen nach ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste angezeigt. Die Details können Sie in der Detailansicht einsehen.

- "Info-Lager-Gestelle - Trefferliste-Allgemein" auf Seite F-1769
- "Info-Lager-Gestelle - Trefferliste-Details" auf Seite F-1770

**Lager**
Lagernummer.

**Gestellnr.**
Nummer des Lagergestells.

**Gestell**
Bezeichnung des Gestells.

**Fach**
Bezeichnung des Fachs.

**Artikel**
Artikelnummer.

**Variante**
Abmessungen der Variante.

**Farbe**
Farbvariante des Artikels.

**Anzahl**
Stückzahl des Artikels.

**Fifo-Datum**
Datum für die Gestellbuchung nach dem Fifo-Prinzip.

---

## Info-Lager-Gestelle – Trefferliste-Allgemein

**Infosystem > Gestell > Filtern > Allgemein**

*Abb. F-42 Info-Lager-Gestelle – Trefferliste-Allgemein*

In diesem Dialog werden die Ergebnisse der Suche nach Lagergestellen angezeigt. Die Details können Sie in der Detailansicht einsehen.

- "Info-Lager-Gestelle - Trefferliste-Details" auf Seite F-1770

Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

### Trefferliste

- **Lager:** Lagernummer.
- **Artikel:** Artikelnummer.
- **Variante:** Abmessungen der Variante.
- **Gestellnr.:** Nummer des Lagergestells.
- **Gestell:** Bezeichnung des Gestells.
- **Fach:** Bezeichnung des Fachs.
- **Bezeichnung:** Bezeichnung des Fachs.
- **Stück:** Stückzahl des Artikels.

---

- **Preis:** Gesamtpreis des Artikels.
- **Fifo-Datum:** Datum für die Gestellbuchung nach dem Fifo-Prinzip.

### Info-Lager-Gestelle – Trefferliste-Details

**Infosystem > Gestell > Filtern > Details**

*Abb. F-43 Info-Lager-Gestelle - Trefferliste-Details*

In diesem Dialog werden die Details zur Trefferliste der Lagergestelle angezeigt.
Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

#### Details

**Artikel**
Artikelnummer.

**Variante**
Abmessungen der Variante.

**Farbe**
Farbvariante des Artikels.

**Stück**
Stückzahl des Artikels.

**Preis**
Gesamtpreis des Artikels.

**Lager**
Lagernummer.

---

**Gestell**
Bezeichnung des Gestells.

**Fach**
Bezeichnung des Fachs.

**Fifo-Datum**
Datum für die Gestellbuchung nach dem Fifo-Prinzip.

**Letzte Änderung am, von**
Datum der letzten Änderung am Buchungssatz und Name des Anwenders, der die letzte Buchung ausgeführt hat.

## Info-Lager-Stapel

**Infosystem > Stapel**

In diesem Dialog können Sie sich die Informationen zu den Lagerstapeln anzeigen lassen.

Zu diesem Dialog werden folgende Unterdialoge angezeigt:

- Info-Lager-Stapel – Filterdialog
- Info-Lager-Stapel - Trefferliste
- Info-Lager-Stapel – Trefferliste-Details

### Info-Lager-Stapel – Filterdialog

**Infosystem > Stapel**

*Abb. F-44 Info-Lager-Stapel - Filterdialog*

In diesem Dialog können Sie die Informationen zu den Lagerstapeln nach ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste angezeigt. Die Details können Sie in der Detailansicht einsehen.

- "Info-Lager-Stapel - Trefferliste" auf Seite F-1772
- "Info-Lager-Stapel - Trefferliste-Details" auf Seite F-1773

**Artikel**
Artikelnummer.

**Lager**
Lagernummer.

**Stapel**
Stapelnummer.

**Stapelbez.**
Bezeichnung des Stapels.

---

**Variante**
Abmessungen der Variante.

**Farbe**
Farbvariante des Artikels.

**Datum**
Datum, an dem der Buchungssatz gebucht wurde.

**Anzahl**
Stückzahl des Artikels.

**Menge**
Artikel in Mengeneinheit.

### Info-Lager-Stapel – Trefferliste

**Infosystem > Stapel > Filtern**

*Abb. F-45 Info-Lager-Stapel – Trefferliste*

In diesem Dialog werden die Ergebnisse der Suche nach Lagerstapel angezeigt. Die Details können Sie in der Detailansicht einsehen.
- "Info-Lager-Stapel - Trefferliste-Details" auf Seite F-1773

Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

#### Trefferliste

- **Stapel:** Stapelnummer.
- **Bezeichnung:** Bezeichnung des Stapels.
- **Artikel:** Artikelnummer.

---

- **Lager:** Lagernummer.
- **Variante:** Abmessungen der Variante.
- **Menge:** Artikel in Mengeneinheit.
- **Stück:** Stückzahl des Artikels.
- **Preis:** Gesamtpreis des Artikels.
- **Datum:** Datum, an dem der Buchungssatz gebucht wurde.

### Info-Lager-Stapel – Trefferliste-Details

**Infosystem > Stapel > Filtern > <F5>**

*Abb. F-46 Info-Lager-Stapel - Trefferliste-Details*

In diesem Dialog werden die Details zur Trefferliste der Lagerstapel angezeigt.
Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

#### Details

**Artikel**
Artikelnummer.

**Lager**
Lagernummer.

---

**Stapel**
Stapelnummer.

**Variante**
Abmessungen der Variante.

**Farbe**
Farbvariante des Artikels.

**Menge**
Artikel in Mengeneinheit.

**Stück**
Stückzahl des Artikels.

**Preis**
Gesamtpreis des Artikels.

**Letzte Änderung am, von**
Datum der letzten Änderung am Buchungssatz und Name des Anwenders, der die letzte Buchung ausgeführt hat.

---

## Info-Lager-Blätter

**Infosystem > Blatt**

In diesem Dialog können Sie sich die Informationen zu den Glasblättern im Einzelblattkistenlager anzeigen lassen.

Zu diesem Dialog werden folgende Unterdialoge angezeigt:

- Info-Lager-Blätter – Filterdialog
- Info-Lager-Blätter - Trefferliste

### Info-Lager-Blätter – Filterdialog

**Infosystem > Blatt**

*Abb. F-47 Info-Lager-Blätter - Filterdialog*

In diesem Dialog können Sie die Informationen zu den Glasblättern im Einzelblattkistenlager nach ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste angezeigt.
- "Info-Lager-Blätter - Trefferliste" auf Seite F-1776

---

**Blatt**
Nummer des Glasblattes.

**Blattbezeichnung**
Bezeichnung des Glasblattes.

**Artikel**
Artikelnummer.

**Lager**
Lagernummer.

**Kiste**
Kistennummer.

**Kistenbezeichnung**
Bezeichnung der Kiste.

**Variante**
Abmessungen der Variante.

**Farbe**
Farbvariante des Artikels.

**Preis**
Stückpreis des Glasblattes.

**Ausbeute**
Ausbeute des Glasblattes in Prozent.

### Info-Lager-Blätter – Trefferliste

**Infosystem > Blatt > Filtern**

*Abb. F-48 Info-Lager-Blätter – Trefferliste*

In diesem Dialog werden die Ergebnisse der Suche nach Glasblättern im Einzelblattkistenlager angezeigt.

---

#### Trefferliste

- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Kiste:** Kistennummer.
- **Variante:** Abmessungen der Variante.
- **Blatt:** Nummer des Glasblattes.
- **Bezeichnung:** Bezeichnung des Glasblattes.
- **Preis:** Stückpreis des Glasblattes.
- **Ausb.:** Ausbeute des Glasblattes in Prozent.
- **R.:** Reservierungskennzeichen.
  - J = Variante ist für einen Vorgang reserviert.
  - N = Variante ist nicht für einen Vorgang reserviert.

---

## Info-Lager-Historie

**Infosystem > Historie**

In diesem Dialog können Sie die Informationen über die Lagerbuchungen anzeigen lassen.

Zu diesem Dialog werden folgende Unterdialoge angezeigt:

- Info-Lager-Historie – Filterdialog
- Info-Lager-Historie – Trefferliste
- Info-Lager-Historie – Trefferliste-Details

### Info-Lager-Historie – Filterdialog

**Infosystem > Historie**

*Abb. F-49 Info-Lager-Historie – Filterdialog*

In diesem Dialog können Sie die Informationen über die Lagerbuchungen nach ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste angezeigt. Die Details können Sie in der Detailansicht einsehen.

- "Info-Lager-Historie - Trefferliste" auf Seite F-1779
- "Info-Lager-Historie - Trefferliste-Details" auf Seite F-1781

**Artikel**
Artikelnummer.

**Lager**
Lagernummer.

**Lieferant**
Lieferantennummer.

**Auftrag**
Auftragsnummer.

**Opti-Nr**
Die Job-Nummer für die Schnittstelle XTV wird nur angezeigt, wenn die Funktion entsprechend konfiguriert wurde.

**Variante**
Maßvariante des Artikels.

**Farbe**
Farbvariante des Artikels.

**Stapel**
Stapelnummer.

---

**Blattbez.**
Bezeichnung des Glasblattes.

**Kiste**
Kistennummer.

**Datum**
Datum, an dem der Buchungssatz gebucht wurde.

**Anzahl**
Stückzahl des Artikels.

**Menge**
Artikel in Mengeneinheit.

**Preis**
Gesamtpreis des Artikels.

**Kostenstelle**
Bezeichnung der Kostenstelle.

**Status**
Status des aktuellen Satzes, z. B. Lagerausgang.

### Info-Lager-Historie – Trefferliste

**Infosystem > Historie > Filtern**

*Abb. F-50 Info-Lager-Historie – Trefferliste*

In diesem Dialog werden die Ergebnisse der Suche nach Lagerbuchungen angezeigt. Die Details können Sie in der Detailansicht einsehen.

- "Info-Lager-Historie - Trefferliste-Details" auf Seite F-1781

Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

---

#### Trefferliste

- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Variante:** Maßvariante des Artikels.
- **Fach:** Bezeichnung des Fachs.
- **Stück:** Stückzahl des Artikels.

Mit `<F2>` können Sie sich die folgenden Spalten anzeigen lassen:

- **Kiste:** Kistennummer.
- **VA:** Kennzeichen der Verpackungsart.
- **Lieferant:** Lieferantennummer.
- **Stapel:** Stapelnummer.
- **L-Preis:** Artikelpreis im Lager, wenn nach der LIFO-Buchungsmethode abgebucht und berechnet wird.
- **F-Preis:** Artikelpreis im Lager, wenn nach der FIFO-Buchungsmethode abgebucht und berechnet wird.
- **Auftr.:** Auftragsnummer.

---

## Info-Lager-Historie – Trefferliste-Details

**Infosystem > Historie > Filtern > <F5>**

*Abb. F-51 Info-Lager-Historie – Trefferliste-Details*

In diesem Dialog werden die Details zur Trefferliste der Lagerbuchungen angezeigt.

Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

### Details

**Artikel**
Artikelnummer.

**Lager**
Lagernummer.

**Kiste**
Kistennummer.

**Verpackart**
Kennzeichen der Verpackungsart.

**Lieferant**
Lieferantennummer.

**Fach**
Bezeichnung des Fachs.

**Blatt**
Nummer und Bezeichnung des Blattes.

**Auftrag**
Auftragsnummer.

---

**Opti-Nr**
Die Job-Nummer für die Schnittstelle XTV wird nur angezeigt, wenn die Funktion entsprechend konfiguriert wurde.

**Kunde**
Kundennummer und Kundenname.

**Variante**
Maßvariante des Artikels.

**Farbe**
Farbvariante des Artikels.

**Buchungsanzahl**
Stückzahl, die für diesen Buchungssatz gebucht wurde.

**Buchungsmenge**
Gesamtmenge in Mengeneinheit, die gebucht wurde.

**Buchungspreis**
Gesamtpreis der gebuchten Mengen.

**LIFO-Preis**
Artikelpreis im Lager, wenn nach der LIFO-Buchungsmethode abgebucht und berechnet wird.

**FIFO-Preis**
Artikelpreis im Lager, wenn nach der FIFO-Buchungsmethode abgebucht und berechnet wird.

**Kostenstelle**
Bezeichnung der Kostenstelle.

**Letzte Buchung am, von**
Datum der letzten Änderung am Buchungssatz und Name des Anwenders, der die letzte Buchung ausgeführt hat.

**Bemerkung**
Zusätzliche Informationen aus der Lagereingangsbuchung.

---

## Aufträge/Bestellungen

**Infosystem > Aufträge/Bestellungen**

In diesem Dialog können Sie die Informationen zu auftrags- oder bestellbezogenen Buchungen anzeigen lassen.

Zu diesem Dialog werden folgende Unterdialoge angezeigt:

- Aufträge/Bestellungen - Filterdialog
- Aufträge/Bestellungen - Trefferliste
- Aufträge/Bestellungen - Trefferliste-Details

### Aufträge/Bestellungen – Filterdialog

**Infosystem > Aufträge/Bestellungen**

*Abb. F-52 Aufträge/Bestellungen - Filterdialog*

In diesem Dialog können Sie die Informationen zu auftrags- oder bestellbezogenen Buchungen im Lager nach ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste angezeigt. Die Details können Sie in der Detailansicht einsehen.

- "Aufträge/Bestellungen - Trefferliste" auf Seite F-1784
- "Aufträge/Bestellungen - Trefferliste-Details" auf Seite F-1785

**Auftrag**
Auftragsnummer oder Bestellnummer.

**Artikel**
Artikelnummer.

**Lager**
Lagernummer.

**Variante**
Nummer der Artikelvariante.

**Farbe**
Nummer der Farbvariante.

---

**Buchung**
Buchungsstatus des Auftrags oder der Bestellung.
Folgende Optionen stehen zur Auswahl:
- 0 = noch keine Buchung ausgeführt.
- 1 = Teilbuchung einer Position ausgeführt.
- 2 = Position komplett gebucht.
- 3 = Auftrag oder Bestellung wurde komplett gebucht.

**Datum**
Datum, an dem die Lagerbuchung zum Auftrag oder zur Bestellung ausgeführt wurde.

### Aufträge/Bestellungen – Trefferliste

**Infosystem > Aufträge/Bestellungen > Filtern**

*Abb. F-53 Aufträge/Bestellungen - Trefferliste*

In diesem Dialog werden die Ergebnisse der Suche nach auftrags- oder bestellbezogenen Buchungen im Lager angezeigt. Die Details können Sie in der Detailansicht einsehen.
- "Aufträge/Bestellungen - Trefferliste-Details" auf Seite F-1785

Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

#### Trefferliste

- **Auftrag:** Auftragsnummer oder Bestellnummer.
- **Position:** Nummer der Position im Auftrag oder in der Bestellung.

---

- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Variante:** Nummer der Artikelvariante.
- **Anzahl:** Zu verbuchende Stückzahl pro Position.
- **Menge:** Buchungsmenge in der Mengeneinheit des Artikels.
- **Verbucht:** Buchungsanzahl in Stück, die gebucht wurde.
- **Datum:** Datum, an dem die Lagerbuchung zum Auftrag oder zur Bestellung ausgeführt wurde.

### Aufträge/Bestellungen – Trefferliste-Details

**Infosystem > Aufträge/Bestellungen > Filtern > <F5>**

*Abb. F-54 Aufträge/Bestellungen - Trefferliste-Details*

In diesem Dialog werden die Details zur Trefferliste der auftrags- oder bestellbezogenen Buchungen im Lager angezeigt.

Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

---

### Details

**Artikelnummer**
Artikelnummer und Artikelbezeichnung.

**Lager**
Lagernummer.

**Variante**
Nummer der Artikelvariante.

**Farbe**
Nummer der Farbvariante.

**Auftrag**
Auftragsnummer oder Bestellnummer.

**Position**
Nummer der Position im Auftrag oder in der Bestellung.

**Anzahl**
Zu verbuchende Stückzahl pro Position.

**Menge**
Buchungsmenge in der Mengeneinheit des Artikels.

**Buchung**
Buchungsstatus des Auftrags oder der Bestellung.
Folgende Optionen stehen zur Auswahl:
- 0 = noch keine Buchung ausgeführt.
- 1 = Teilbuchung einer Position ausgeführt.
- 2 = Position komplett gebucht.
- 3 = Auftrag oder Bestellung wurde komplett gebucht.

**Datum**
Datum, an dem die Lagerbuchung zum Auftrag oder zur Bestellung ausgeführt wurde.

**Verbucht (Anzahl)**
Verbuchte Stückzahl des Artikels.

**Verbucht (Menge)**
Verbuchte Menge in der Mengeneinheit des Artikels.

**Erfasser (Mitarbeiter)**
Erfassungsdatum und Mitarbeiter, der diese Buchung erfasst hat.

**Verbucht (Mitarbeiter)**
Buchungsdatum und Mitarbeiter, der diese Buchung durchgeführt hat.

---

## Buchungsstatus

**Infosystem > Buchungsstatus**

Im Buchungsstatus können Sie sich die Buchungsinformationen zu den Lagern anzeigen lassen, die nicht gebuchten oder fehlerhaften Buchungssätze enthalten oder Lager die sich gerade in der Inventur befinden. Im Dialog Buchungsstatus – Korrektur können Sie die Daten für den Buchungsstatus korrigieren.

Zu diesem Dialog werden folgende Unterdialoge angezeigt:

- Buchungsstatus – Ungebucht
- Buchungsstatus – Fehler
- Buchungsstatus – Inventur
- Buchungsstatus - Korrektur

### Buchungsstatus – Ungebucht

**Infosystem > Buchungsstatus > Ungebucht**

*Abb. F-55 Buchungsstatus – Ungebucht*

In diesem Dialog können Sie sich Buchungsinformationen zu den Lagern anzeigen lassen, die nicht gebuchte Buchungssätze enthalten.

Sie können folgende Tastaturbefehle ausführen:

- Mit `<F5>` können Sie den Dialog **Buchungsstatus – Korrektur** aufrufen.
- Mit `<F2>` können Sie sich weitere Spalten anzeigen lassen.

#### Rumpfbereich

- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.

---

- **Kiste:** Kistennummer.
- **Variante:** Maßvariante des Artikels.
- **Farbe:** Nummer der Artikelfarbe.
- **Anzahl:** Anzahl der nicht gebuchten Artikel.
- **Status:** Nummer des Status der aktuellen Buchung, z. B. Lagerausgang.
- **Fehler:** Nummer für den Fehlerstatus. Der Fehlerstatus steht im Fußbereich im Klartext.

Mit `<F2>` können Sie sich weitere Spalten anzeigen lassen.

- **Menge:** Mengeneinheit des Artikels.
- **Preis:** Preis pro Mengeneinheit, z. B. Artikel pro Stück.
- **Datum:** Datum der Lagerbuchung.
- **Auftrag:** Auftragsnummer.
- **Position:** Positionsnummer im Auftrag.

#### Fußbereich
Die Feldbeschreibungen entsprechen den Spaltenbeschreibungen des Dialogs.

---

### Buchungsstatus – Fehler

**Infosystem > Buchungsstatus > Fehler**

*Abb. F-56 Buchungsstatus – Fehler*

In diesem Dialog können Sie sich Buchungsinformationen zu den Lagern anzeigen lassen, die fehlerhafte Buchungssätze enthalten. Im Dialog **Buchungsstatus - Korrektur** können Sie die Daten für den Buchungsstatus korrigieren.

Sie können folgende Tastaturbefehle ausführen:

- Mit `<F5>` können Sie den Dialog **Buchungsstatus – Korrektur** aufrufen.
- Mit `<F2>` können Sie sich weitere Spalten anzeigen lassen.

#### Rumpfbereich

- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Kiste:** Kistennummer.
- **Variante:** Maßvariante des Artikels.
- **Farbe:** Nummer der Artikelfarbe.
- **Anzahl:** Anzahl der nicht gebuchten Artikel.
- **Status:** Nummer des Status der aktuellen Buchung, z. B. Lagerausgang.
- **Fehler:** Nummer für den Fehlerstatus. Der Fehlerstatus steht im Fußbereich im Klartext.

---

Mit `<F2>` können Sie sich weitere Spalten anzeigen lassen.

- **Menge:** Mengeneinheit des Artikels.
- **Preis:** Preis pro Mengeneinheit, z. B. Artikel pro Stück.
- **Datum:** Datum der Lagerbuchung.
- **Auftrag:** Auftragsnummer.
- **Position:** Positionsnummer im Auftrag.

#### Fußbereich
Die Feldbeschreibungen entsprechen den Spaltenbeschreibungen des Dialogs.

---

### Buchungsstatus – Inventur

**Infosystem > Buchungsstatus > Inventur**

*Abb. F-57 Buchungsstatus – Inventur*

In diesem Dialog können Sie sich Buchungsinformationen zu den Lagern anzeigen lassen, die nicht gebuchten oder fehlerhaften Buchungssätze enthalten oder Lager die sich gerade in der Inventur befinden. Im Dialog **Buchungsstatus – Korrektur** können Sie die Daten für den Buchungsstatus korrigieren.

> **Lager in Inventur**
> Wenn ein Lager für die Inventur freigeschaltet wird, wird eine Kopie des Lagers mit negativen Lagernummern erzeugt, das sogenannte Inventurlager. In dieses Inventurlager werden die gezählten Bestände eingetragen. Während der Inventur werden die Eingänge und Ausgänge weiterhin auf die positive Lagernummer gebucht. Damit ist gewährleistet, dass während der Inventur Eingangs- und Ausgangsbuchungen für dieses Lager erfasst werden können. Nach einem Inventurabschluss werden die geänderten Bestände aus dem Inventurlager mit den Eingangs- und Ausgangsbuchungen aktualisiert, die während der Inventur erfasst wurden.

Sie können folgenden Tastaturbefehl ausführen:

- Mit `<F5>` können Sie den Dialog **Buchungsstatus – Korrektur** aufrufen.

#### Rumpfbereich

- **Lager:** Lagernummer des Lagers, das zur Inventur freigeschaltet ist.
- **Bezeichnung:** Bezeichnung des Lagers in Inventur.
- **Datum:** Datum, an dem das Lager zur Inventur vorbereitet wurde.

---

- **Mitarbeiter:** Mitarbeiternummer des Mitarbeiters, der das Lager zur Inventur vorbereitet hat.

### Buchungsstatus – Korrektur

**Infosystem > Buchungsstatus > Ungebucht, Fehler, Inventur > <F5>**

*Abb. F-58 Buchungsstatus – Korrektur*

In diesem Dialog können Sie die Daten des Buchungsstatus der folgenden Dialoge korrigieren:

- Buchungsstatus – Ungebucht
- Buchungsstatus – Fehler
- Buchungsstatus – Inventur

#### Rumpfbereich

**Artikel**
Artikelnummer und Artikelbezeichnung.

**Lager**
Lagernummer und Lagerbezeichnung.

**Lieferant**
Lieferantennummer und Lieferantenname.

**Kiste**
Kistennummer und Kistenbezeichnung.

**Fach**
Bezeichnung des Fachs im Fachlager.

**Auftrag**
Auftragsnummer, bei auftragsbezogenen Lagerbuchungen.

**Variante**
Maßvariante des Artikels.

**Farbe**
Nummer der Artikelfarbe.

**Buchungsanzahl**
Gebuchte Menge in Stück.

---

**Buchungsmenge**
Gebuchte Menge in der entsprechenden Mengeneinheit.

**Buchungspreis**
Gesamtpreis der Artikel.

**verbucht am**
Datum der letzten Buchung des aktuellen Buchungssatzes.

**von**
Name des Mitarbeiters, der den aktuellen Buchungssatz zuletzt gebucht hat.

#### Fußbereich

**Artikel**
Artikelbezeichnung.

**Lager**
Lagerbezeichnung.

**Fehler**
Fehlerstatus im Klartext.

**Status**
Status der aktuellen Buchung im Klartext, z. B. Lagerausgang.

---

## Lagerinformationen – Pickliste

**Infosystem > Auftragsliste**

*Abb. F-59 Lagerinformationen – Pickliste*

In diesem Dialog können Sie sich die auftragsbezogenen Lagerartikel anzeigen lassen. Für die Ausgabe der Lagerinformationen der Pickliste wird die Adhoc-SQL Gruppe 1 und die SQL-Abfrage 26 verwendet. Bei Bedarf muss diese Abfrage separat angepasst werden. Die Abfrage können Sie über `<Strg>` + `<F4>` > SQL-Abfragen > Ändern anpassen.

**Auftrag**
Auftragsnummer, für die die Pickliste erstellt wird.

---

## Lagerinformationen – Trefferliste

**Infosystem > Auftragsliste > Filtern**

*Abb. F-60 Lagerinformationen – Trefferliste*

In diesem Dialog wird Ihnen die Trefferliste für auftragsbezogene Lagerartikel angezeigt.

### Trefferliste

- **Artikel:** Artikelnummer.
- **Bezeichnung:** Artikelbezeichnung.
- **Farbe:** Bezeichnung der Farbvariante des Artikels.
- **Variante:** Abmessungen der Artikelvariante.
- **Menge:** Stückzahl des Artikels.
- **Auftrag:** Auftragsnummer.
- **Spalten ohne Namen:** Positionsnummer im Auftrag.

---

## LVR-Status

**Infosystem > LVR-Status**

*Abb. F-61 SQL-Abfragen - Lagerverwaltungsrechner (LVR)*

In diesem Dialog können Sie sich die LVR-Status für Lagerartikel anzeigen lassen. Für die Ausgabe der Bestandsprognose der Reichweite wird die Adhoc-SQL Gruppe 1 und die SQL-Abfrage 19 verwendet. Bei Bedarf muss diese Abfrage separat angepasst werden. Die Abfrage können Sie über `<Strg>` + `<F4>` > SQL-Abfragen > Ändern anpassen

## Reichweite – Bestandsprognose

**Infosystem > Reichweite**

*Abb. F-62 Reichweite - SQL-Abfragen*

In diesem Dialog können Sie sich die Bestandsprognose für Lagerartikel anzeigen lassen. Für die Ausgabe der Bestandsprognose der Reichweite wird die Adhoc-SQL Gruppe 1 und die SQL-Abfrage 21 verwendet. Bei Bedarf muss diese Abfrage separat angepasst werden. Die Abfrage können Sie über `<Strg>` + `<F4>` > SQL-Abfragen > Ändern anpassen.

**Von Artikel**
Startwert für den Wertebereich der Artikelnummer, um die Trefferliste zu filtern.

**Bis Artikel**
Maximalwert für den Wertebereich der Artikelnummer, um die Trefferliste zu filtern.

**Von Lager**
Startwert für den Wertebereich der Lagernummer, um die Trefferliste zu filtern.

**Bis Lager**
Maximalwert für den Wertebereich der Lagernummer, um die Trefferliste zu filtern.

---

## Reichweite – Trefferliste

**Infosystem > Reichweite > Filtern**

*Abb. F-63 Reichweite – Trefferliste*

In diesem Dialog wird Ihnen anhand von Lagerbuchungen eine Prognose angezeigt, für wie viele Monate der aktuelle Bestand des Lagerartikels für die Produktion ausreicht.

### Trefferliste

- **Artikel:** Artikelnummer.
- **Bestand:** Aktueller Lagerbestand des Artikels.
- **Verbrauch:** Verbrauch des Artikels in der Vergangenheit.
- **Reichweite (Mon):** Geschätzte Zeit in Monaten, die der Artikel noch auf Lager zur Verfügung steht.

---

## Dispositiver Bestand

**Infosystem > Dispositiver Bestand**

*Abb. F-64 Dispositiver Bestand*

In diesem Dialog können Sie sich den aktuellen Lagerbestand des Artikels, die bestellten, verplanten und verfügbaren Mengen des Lagerartikels anzeigen lassen.

### Kopfbereich

**Datum**
Filterkriterium nach Datum.

**Artikel**
Filterkriterium für die Artikelnummer.

**Variante**
Filterkriterium für die Maßvariante.

### Rumpfbereich

- **Variante:** Maßvariante des Artikels.
- **Lager:** Lagernummer des Lagers, in dem der Artikel eingelagert ist.
- **Bezeichnung:** Bezeichnung des Lagerartikels.
- **Bestand:** Aktueller Bestand des Lagerartikels.
- **Bestellt:** Aktuell bestellte Menge des Lagerartikels.
- **Verplant:** Aktuell verplante Menge des Lagerartikels, z. B. für die Produktion.
- **Verfügbar:** Aktuell verfügbare Menge des Lagerartikels.

---

### Fußbereich

**Gesamtsumme**
Summierter Wert jeweils für eine Spalte. Folgende Spalten werden aufsummiert angezeigt:

- Bestand
- Bestellt
- Verplant
- Verfügbar

---

## Bestandsprognose

**Infosystem > Prognose**

*Abb. F-65 Bestandsprognose*

In diesem Dialog können Sie sich für einen ausgewählten Zeitraum die Prognose für den Lagerbestand des Artikels anzeigen lassen. Verplante Bestände entstehen durch erfasste Aufträge. Die Prognose zeigt den Lagerbestand aufgrund von im System vorhandenen Aufträgen und bereits bestehenden Bestellungen.

Die Unter- oder Überdeckung der Lagerbestände kann durch definierte Alarmbestände verhindert werden.
- "Artikelstammdaten Lager" auf Seite F-1735

Mit `<Shift>` + `<F5>` lassen Sie sich für den ausgewählten Artikel die Bestandsprognose in der grafischen Übersicht anzeigen.

### Kopfbereich

**Artikel**
Artikelnummer für die gefilterte Auflistung.

**Lager**
Lagernummer. Wenn in diesem Feld kein Eintrag erfolgt, wird eine lagerübergreifende Bestandsprognose erstellt.

**Variante**
Maßvariante des Artikels.

**Datum**
Zeitraum der Bestandsprognose.

**Periode**
Zeitabstände in der Bestandsprognose.
