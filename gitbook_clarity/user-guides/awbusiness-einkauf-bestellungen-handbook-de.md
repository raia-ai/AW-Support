---
description: "A+W Business Einkauf Tutorial - Bestellungen und Wareneingang"
---


# A+W Business Einkauf Tutorial

---
## Bestellungen

### Sammelbestellungen pro Lieferant

Bestellungen aus verschiedenen Aufträgen an denselben Lieferanten werden zu Sammelbestellungen zusammengefasst. Dabei orientiert sich das System an der Reihenfolge, in der die Einträge im Bestellpool aufgeführt sind. In diesem Fall darf jedoch die Auftragsnummer nicht als Bestellnummer übernommen werden.

Wenn Sie im Bestellpool alle Positionen für einen Lieferanten markiert haben, können diese zu einer Sammelbestellung zusammengefasst werden.

Dazu müssen folgende Voraussetzungen erfüllt sein:
*   Identischer Lieferant
*   Identischer Liefertermin
*   Das Kennzeichen für Sammelbestellungen in den Lieferantenstammdaten muss gesetzt sein (Register Auftrag).

Im Menü **Funktionen > Markierungsoptionen** legen Sie fest, für welchen Lieferanten die Sammelbestellung erzeugt werden soll.

*Abb. D-33: Markierungsoptionen für Sammelbestellung*

Mit den Markierungsoptionen werden alle entsprechenden Positionen im Bestellpool automatisch markiert. Damit die Sammelbestellung erzeugt werden kann, muss im Menü **Optionen > Gruppe Übergabe > Auftragsbezogene Übergabe** deaktiviert sein.

### Dokument in den Bestellpool stellen

Für die Übergabe werden die Aufträge in einem Nummernverwalter gesammelt. Der Bestellpool greift auf den Nummernverwalter zu, den Sie auswählen. Mit der Bestellübergabe kann ein neuer Nummernverwalter erstellt werden, in den die erfolgreichen Bestellungen gestellt werden. Die Bestellungen können nur erzeugt werden, wenn die Aufträge vor der Übergabe geschlossen sind.

**So erzeugen Sie eine Bestellung zu einem Kundenauftrag**

1.  Wählen Sie **Dokumente > Auftrag > Bestellübergabe**.

*Abb. D-34: Aufträge aus dem Nummernverwalter übergeben*
*   **A** Nummernverwalter mit Aufträgen für die Übergabe
*   **B** Modus der Übergabe
*   **C** Ziel-Nummernverwalter
*   **D** Ziel-Nummernkreis

2.  Wählen Sie den Modus (B) aus:
    *   **Pool füllen:** Mit dieser Option werden die Aufträge im Register Bestellpool angezeigt und können vor der Übergabe geprüft und geändert werden.
    *   **Sofort bestellen:** Mit dieser Option werden die Daten sofort als Bestellung beim Standard-Lieferanten erzeugt. Diese Option ist dann sinnvoll, wenn Sie zuvor keine Preise oder Liefertermine prüfen möchten.
    *   **Sofort anfragen:** Mit dieser Option werden die Daten als Anfrage beim Standard-Lieferanten erzeugt. Die Bestellungen können Sie anschließend drucken und auf die gewohnte Art an den Lieferanten senden, z. B. per E-Mail-Anhang.

    In diesem Beispiel werden die Aufträge zunächst im Bestellpool geprüft.

3.  Wählen Sie den Nummernverwalter (A) aus, in dem die Aufträge mit Bestellpositionen stehen.
4.  Wählen Sie den Ziel-Nummernverwalter (C) aus, in den die erzeugten Bestellungen gestellt werden.
    Sie können einen neuen Namen eingeben und so einen neuen Nummernverwalter anlegen. Wenn Sie dazu einen anderen Mitarbeiter auswählen, wird der Nummernverwalter diesem zugeordnet.
5.  Wählen Sie ggf. einen anderen Ziel-Nummernkreis (D) aus.
6.  Wählen Sie im Menü **Start > Ausführen**, um die Aufträge in den Bestellpool zu stellen.

*Abb. D-35: Auftragspositionen im Bestellpool*

Der Bestellpool wird gefüllt. Pro Auftrag werden die Bestellpositionen angezeigt.

7.  Markieren Sie die Positionen, die Sie an den Einkauf übergeben möchten. Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf.

*Abb. D-36: Markierte Auftragspositionen übergeben*

Nur die Positionen sind markiert, die mit einem X gekennzeichnet sind.

8.  Wählen Sie im Menü **Start > Ausführen**, um die Aktion zu starten.
    Die aktivierten Prüfungen werden durchgeführt. Dies kann je nach Anzahl der Aufträge einige Momente dauern. Bestätigen Sie die jeweiligen Hinweise mit [Ja] oder [Nein], um die Prüfungen fortzusetzen. Wenn alle Prüfungen abgeschlossen sind, werden die zugehörigen Bestellungen angelegt und sind damit an den Einkauf übergeben.
    Die übergebenen Positionen werden aus dem Bestellpool gelöscht.
    Der Auftragsstatus wird hochgesetzt. In der Auftragshistorie wird die Nummer der Bestellung als Referenz angegeben.

*Abb. D-37: Bestellnummern nach der Übergabe*

Nach der Übergabe der Positionen wird die Bestellnummer zum Auftrag angezeigt.

Die erzeugten Bestellungen können Sie unter **Dokumente > Bestellung** öffnen und weiterbearbeiten. Drucken Sie die neue Bestellung und senden Sie sie an den Lieferanten.

### Bestellung im Bestellpool ändern

Wenn zu einer Position Terminschwierigkeiten angezeigt werden, können Sie im Bestellpool einen anderen Lieferanten auswählen. Den Dialog zur Änderung des Lieferanten können Sie auch ohne Terminschwierigkeiten öffnen, um einen anderen als den vorgeschlagenen Standard-Lieferanten auszuwählen.

**So ändern Sie den Liefertermin und den Lieferanten**

1.  Wählen Sie **Dokumente > Auftrag > Bestellübergabe**.
2.  Stellen Sie die Aufträge in den Bestellpool.
    Dieser Vorgang ist in der vorausgegangenen Einheit beschrieben.
    ⇨ "Dokument in den Bestellpool stellen" auf Seite D-2102
3.  Markieren Sie die Position, zu der Sie den Liefertermin ändern wollen. Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf.

*Abb. D-38: Position für die Änderung des Lieferanten markiert*

Nur die Positionen sind markiert, die mit einem X gekennzeichnet sind.

4.  Wählen Sie im Menü **Funktionen > Lieferant/Liefertermine ändern**.

Sie können jetzt folgende Angaben ändern:
*   den Lieferanten
*   den Liefertermin des Lieferanten
*   den Termin der Anlieferung beim Kunden.

5.  Klicken Sie auf [OK], um die Änderung zu übernehmen.
    Der Dialog **Lieferant und Liefertermine ändern** wird geschlossen. Im Bestellpool wird die Auftragsposition mit dem neuen Termin und/oder Lieferanten angezeigt.
6.  Wählen Sie im Menü **Start > Ausführen**, um die Position an den Einkauf zu übergeben.
    Die aktivierten Prüfungen werden durchgeführt. Dies kann je nach Anzahl der Aufträge einige Momente dauern. Bestätigen Sie die jeweiligen Hinweise mit [Ja] oder [Nein], um die Prüfungen fortzusetzen. Wenn alle Prüfungen abgeschlossen sind, werden die zugehörigen Bestellungen angelegt und sind damit an den Einkauf übergeben.
    Die geänderten Termine werden in den Auftrag zurückgeschrieben.
    Nach der Übergabe der Positionen wird die Bestellnummer zum Auftrag angezeigt.
    Die erzeugte Bestellung können Sie unter **Dokumente > Bestellung** öffnen und weiterbearbeiten. Drucken Sie die neue Bestellung und senden Sie sie an den Lieferanten.

### Preise im Bestellpool vergleichen

Wenn zu einem Produkt mehrere Lieferanten hinterlegt sind, können Sie im Bestellpool die Preise vergleichen und einen anderen Lieferanten auswählen.

**So vergleichen Sie die Preise im Bestellpool**

1.  Wählen Sie **Dokumente > Auftrag > Bestellübergabe**.
2.  Stellen Sie die Aufträge in den Bestellpool.
    Dieser Vorgang ist in der vorausgegangenen Einheit beschrieben.
    ⇨ "Dokument in den Bestellpool stellen" auf Seite D-2102
3.  Markieren Sie die Position, zu der Sie die EK-Preise vergleichen wollen. Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf.

*Abb. D-39: Position für den Preisvergleich markiert*

Nur die Positionen sind markiert, die mit einem X gekennzeichnet sind.

4.  Wählen Sie im Menü **Funktionen > Lieferantenpreise**.

*Abb. D-40: Preisvergleich für Position*
*   **A !!! Bei allen Textfarben:** Liefertermin gefährdet
*   **B Textfarbe rot:** Standard-Lieferant
*   **C Textfarbe grün:** preisgünstigster Lieferant
*   **D Textfarbe blau:** Standard-Lieferant ist preisgünstigster Lieferant

5.  Markieren Sie die Checkbox links des Lieferanten, an den die Bestellung der Position gesendet werden soll.
6.  Klicken Sie auf [OK], um die Änderung zu übernehmen.
    Der Dialog **Preisvergleich** wird geschlossen. Im Bestellpool wird die Auftragsposition mit dem neuen Lieferanten angezeigt.
7.  Markieren Sie die Aufträge oder Auftragspositionen, die Sie an den Einkauf übergeben möchten. Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf.

*Abb. D-41: Position mit geändertem Lieferanten*

Nur die Positionen sind markiert, die mit einem X gekennzeichnet sind.

8.  Wählen Sie im Menü **Start > Ausführen**, um die Übergabe zu starten.
    Die aktivierten Prüfungen werden durchgeführt. Dies kann je nach Anzahl der Aufträge einige Momente dauern. Bestätigen Sie die jeweiligen Hinweise mit [Ja] oder [Nein], um die Prüfungen fortzusetzen. Wenn alle Prüfungen abgeschlossen sind, werden die zugehörigen Bestellungen angelegt und sind damit an den Einkauf übergeben.
    Übergebene Positionen werden aus dem Bestellpool gelöscht.

*Abb. D-42: Bestellnummern nach der Übergabe*
*   **A Erste Bestellnummer**
*   **B Zweite Bestellnummer**

Nach der Übergabe der Positionen werden die alte und die neue Bestellnummer zum Auftrag angezeigt.

Die Bestellungen können Sie unter **Dokumente > Bestellung** öffnen und weiterbearbeiten. Drucken Sie die neue Bestellung und senden Sie sie an den Lieferanten.

Vergessen Sie nicht, den alten Lieferanten über die Änderung zu informieren.

### Auftrags- und Bestell-Info

Zu jedem Auftrag und zu jeder Bestellung können die referenzierten Dokumente in einer Übersicht angezeigt werden. Diese Funktion steht in der Bestellung (Kopfdaten) über das Menü **Funktion > Auftrags-/Bestell-Info** zur Verfügung.

*Abb. D-43: Auftrags- und Bestellinfo – Übersicht über die referenzierten Dokumente*

Dieser Dialog ist im Part Verkauf beschrieben.
⇨ Verkauf, "Auftrags-/Bestell-Info" auf Seite C-1845

### Manuelle Bestellung

> **Lernziele**
> *   Bestellung manuell erfassen.
> *   Dokumententyp Lagerbestellung kennenlernen.

> **Nutzen**
> Lagerbestellungen werden für die Bestandspflege im Lager erfasst. Sie können neben den Lagerartikeln auch Artikel enthalten, die nicht als Bestand im Lager gepflegt werden.

> **Merke**
> **Manuelle Bestellung**: Bestellungen, die nicht durch die Bestellübergabe aus einer Auftragsposition erzeugt werden, müssen manuell erfasst werden.
> **Unabhängige Bestellung**: In unabhängigen Bestellungen können Sie sämtliche Produkte erfassen, die eingekauft werden können. Unabhängige Bestellungen beziehen sich nicht auf einen Auftrag.
> **Lagerbestellungen**: Lagerbestellungen sind ein eigener Dokumententyp. Sie dienen dazu, den Lagerbestand aufzufüllen.
> **Voreinstellungen**:
> Stammdaten:
> *   Lieferantenkartei
>
> Lieferanten
> *   Register Auftrag
> *   Register Finanzen
> *   Register Saldo
>
> Firmendaten:
> *   Register Parameter
> *   Register Lager/EK/EDI

#### Unabhängige Bestellungen

Alle Bestellungen zu Produkten, die nicht das Bestellkennzeichen **Bestellung** oder **Bestellung (komplett)** haben und nicht aus einem Auftrag heraus erzeugt werden, müssen manuell erfasst werden.

Als Bestellung können Sie alle Produkte erfassen, die zur Produktion oder zum Verkauf benötigt werden. Dabei wird unterschieden, ob Sie Artikel bestellen, die als Lagerware verbucht werden können oder solche, die zwar im Lager vorgehalten, jedoch nicht in den Bestandslisten geführt werden. Bestellungen von Lagerartikeln und Kisten müssen mit dem Dokumententyp **Lagerbestellung** erfasst werden, damit der Wareneingang korrekt verbucht werden kann.

Wenn Sie für Ihre Lieferanten entsprechende Konditionen hinterlegen, werden in den Bestellungen sofort die aktuellen EK-Preise ausgewiesen. Diese dienen zur Kontrolle von Preisen in Auftragsbestätigungen (AB) und Rechnungen Ihrer Lieferanten.

#### Lagerbestellungen

Lagerbestellungen werden als eigener Dokumententyp erfasst und können als Positionen alle Zukaufartikel, Lagermaße, Kisten und Sondergrößen enthalten, die als Lagerartikel geführt werden. Die Wareneingänge von Lagerartikeln aus Lagerbestellungen werden direkt in den Lagerbestand gebucht.

Wenn Sie Lagerbestellungen mit Positionen erfassen, die nicht als Lagerartikel geführt werden, werden diese im Wareneingang nicht angezeigt. Sie können in den Firmendaten jedoch die entsprechende Option aktivieren.

Die Lagerbestellungen sind ausführlich im Part Lagerwirtschaft beschrieben.

#### Einkaufspreise

Der EK wird aus den Preislisten für den Einkauf herangezogen. Bei der Erfassung von Bestellpositionen werden die entsprechenden Preise angezeigt und bei Änderungen aktualisiert.

### Unabhängige Bestellung erfassen

Sie können in einer unabhängigen Bestellung alle Produkte erfassen, die in den Stammdaten hinterlegt sind.

> **Arbeiten mit Nummernverwaltern**
> Richten Sie sich für die Bestellungen die Nummernverwalter so ein, dass die Dokumente nach eindeutigen Kriterien zusammengefasst werden, z. B. nach Lieferanten, nach Datum, nach Lagerbestellungen, nach komplett gelieferten Bestellungen.

**So erfassen Sie eine unabhängige Bestellung**

1.  Wählen Sie **Dokumente > Bestellung > Bestellung**.
    Der Dialog Dokumentenverwaltung wird geöffnet.
    ⇨ Verkauf, "Dokument - Kopfdaten" auf Seite C-1687
2.  Prüfen Sie im Menü **Funktionen > NV Auswahl**, ob der richtige Nummernverwalter eingestellt ist, und korrigieren Sie ggf. die Einstellung.
3.  Erfassen Sie den Dokumentenkopf, indem Sie den Lieferanten auswählen.

*Abb. D-44: Unabhängige Bestellung erfassen*
*   **A Termin der Anlieferung durch den Lieferanten**
*   **B Dokumententyp**

4.  Prüfen Sie den Termin für die Anlieferung (A).
    Dies ist der Termin, zu dem Sie die Lieferung bei sich erwarten.
5.  Wählen Sie im Feld **Typ (B)** den Eintrag `<k.A.>`.
    Wenn Sie den Typ auf `<k.A.>` einstellen, wird der Wareneingang nicht auf das Lager gebucht.
    Die Lagerbestellung ist in einer separaten Einheit beschrieben.
    ⇨ "So erfassen Sie eine Lagerbestellung mit Kisten" auf Seite D-2117
6.  Erfassen Sie die Positionen, wie im Kapitel Bestellpositionen im Auftrag beschrieben.
    ⇨ "So erfassen Sie im Auftrag eine Position zur Bestellung" auf Seite D-2088
7.  Drucken und versenden Sie die Bestellung.
    Die Bestellung steht nun in dem von Ihnen bestimmten Nummernverwalter. Zu ihr kann später eine Auftragsbestätigung vom Lieferanten und/oder ein Wareneingang erfasst werden.
    ⇨ "Wareneingang erfassen" auf Seite D-2161

### Lagerbestellung erfassen

Sie können in einer Lagerbestellung auch Artikel bestellen, die nicht als Lagerartikel verbucht werden können. Ein Hinweis macht Sie beim Speichern auf solche Bestellpositionen aufmerksam. Diese Artikel werden beim Wareneingang jedoch nicht automatisch als Lagerbestand verbucht.

In der nachfolgenden Handlungsanleitung wird eine Lagerbestellung für Kisten erfasst. Diese Kistenbestellungen können in der Themenblock Kistengeschäft dann weiterbearbeitet werden.

**So erfassen Sie eine Lagerbestellung mit Kisten**

1.  Erfassen Sie das Dokument, wie im Abschnitt **Unabhängige Bestellung** beschrieben.
    ⇨ "So erfassen Sie eine unabhängige Bestellung" auf Seite D-2115
2.  Wählen Sie im Feld **Typ** den Eintrag **Lagerbestellung**.
    Wenn Sie den Typ auf `<k.A.>` einstellen, können Sie den Wareneingang nicht automatisch auf das Lager buchen.
3.  Wechseln Sie zum Register **Positionen**.
4.  Geben Sie die Produktnummer ein, z. B. **1005**.
    Die Anzahl können Sie nach der Auswahl des Lagerartikels angeben. Maße brauchen Sie nicht einzutragen, diese werden aus dem Lagerartikel übernommen.
5.  Wählen Sie im Menü **Start > Lagersuche**, um den Dialog **Lagerinfo** zu öffnen.
    Sie können den Dialog auch über die Taste `<F3>` öffnen.

*Abb. D-45: Lagerinfo - Lagersuche*
*   **A Produktnummer der Glasart**
*   **B Kiste (ohne ID)**

⇨ Verkauf, "Lagerinfo" auf Seite C-2034

Der Dialog **Lagerinfo** wird mit einer Liste aller Lagermaße und Kisten angezeigt. Für Kisten ist in der Spalte **Inh.** der Wert größer als 1.

6.  Suchen Sie die gewünschte Kiste ohne Kisten-ID aus und übernehmen Sie sie mit einem Doppelklick.
    Der Dialog wird geschlossen und die Positionserfassung wird wieder angezeigt. In der Erfassungszeile werden für Kisten alle Felder ab Menge gesperrt. Die Preisfelder werden aktualisiert.

*Abb. D-46: Kiste in der Positionserfassung*
*   **A Stückzahl**
*   **B Menge**

7.  Geben Sie die gewünschte Stückzahl ein.
    Die Anzeige der Details wird aktualisiert.
8.  Wiederholen Sie die Schritte 4 bis 7, um alle Bestellpositionen zu erfassen.
9.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert.
10. Drucken und versenden Sie die Bestellung.

### Auftragsbestätigung des Lieferanten

> **Lernziele**
> *   Auftragsbestätigung (AB) eines Lieferanten erfassen.
> *   AB pro Position erfassen.
> *   Preise in der AB prüfen.
> *   Ausstehende Auftragsbestätigungen anmahnen.

> **Nutzen**
> *   Die Auftragsbestätigung des Lieferanten wird der Bestellung zugeordnet. Dabei wird der Liefertermin bestätigt oder angepasst, ohne die Bestellung selbst öffnen zu müssen. Die Terminänderungen werden in die referenzierten Dokumente übernommen.
> *   Der Status von referenzierten Aufträgen wird automatisch zusammen mit dem Status der Bestellung umgesetzt.
> *   AB für Bestätigungen Teilmengen können erfasst werden, ohne die Daten neu einzugeben.
> *   Überfällige Bestellungen können aus einem Nummernverwalter herausgefiltert werden, um den jeweiligen Lieferanten anzumahnen.

> **Merke**
> **Teilweise Bestätigung**: Wenn Ihr Lieferant die bestellte Menge in verschiedenen Untermengen bestätigt, können Sie die Auftragsbestätigung (AB) zu einzelnen Positionen oder Teilmengen erfassen.
> **Status**: Der Status der referenzierten Dokumente wird hochgesetzt, wenn Sie in einem der Dokumente die Auftragsbestätigung des Lieferanten erfassen.
> **Dokumentensperre**: Während der Preis- und Rechnungsprüfung sind die referenzierten Dokumente für den Zugriff durch andere Mitarbeiter gesperrt.
> **Mahnung senden**: Die Mahnung wird auf demselben Kommunikationsweg an einen Lieferanten gesendet, wie die Bestellung.
> **Voreinstellungen**: Lieferantenstammdaten: Fax- und E-Mail-Versand.

#### Lieferanten-AB

Ihr Lieferant bestätigt die eingegangene Bestellung durch eine Auftragsbestätigung (AB). Die Nummer dieser Auftragsbestätigung können Sie erfassen und der entsprechenden Bestellung zuordnen. Gleichzeitig können Sie die Termine und Preise prüfen und ggf. in Ihren Dokumenten anpassen.

Beim Erfassen einer Auftragsbestätigung haben Sie die Möglichkeit, die Bestellung und/oder den zugehörigen Kundenauftrag zur weiteren Bearbeitung in einen Ziel-Nummernverwalter zu verschieben.

#### Teillieferungen

Bei größeren Bestellungen kann es vorkommen, dass Ihr Lieferant nicht alle Positionen oder die gesamte Stückzahl zum gewünschten Termin bestätigt, sondern in mehreren Teillieferungen ankündigt. Sie können dann auch eine Teilmenge der Bestellung bestätigen, ohne ein neues Dokument erfassen zu müssen.

#### Status

Der Status aller referenzierten Dokumente wird umgesetzt, sobald die AB-Nummer bestätigt wurde. Die referenzierten Dokumente werden angezeigt, sobald die Auftrags- oder der Bestellnummer eingegeben wurde. Bei unabhängigen Bestellungen bleiben die entsprechenden Felder gesperrt.

#### Auftragsbestätigung und Liefertermin

Die AB des Lieferanten kann auf unterschiedliche Weise erfasst werden:
*   Auftragsbestätigung mit oder ohne Wareneingang. Dabei können Sie die Termine für die Lieferung prüfen und ggf. den Kunden über eine Verschiebung benachrichtigen.
*   Bestätigung einzelner Positionen einer Bestellung.
*   Auftragsbestätigung und Preiskontrolle. Dabei können Sie die Einkaufspreise und den Liefertermin prüfen und korrigieren und ggf. eine Teillieferung zur bestellten Menge erfassen. Die Beschreibung dieser Variante finden Sie unter.
    ⇨ "Preis- und Rechnungskontrolle" auf Seite D-2177

Aus einem Kundenauftrag können mehrere Bestellungen an unterschiedliche Lieferanten erzeugt werden. Die verschiedenen AB-Nummern werden für die entsprechenden Auftragspositionen gespeichert.

### Überfällige Lieferungen

Sie können überfällige Auftragsbestätigungen oder Lieferungen anmahnen. Die Suche nach offenen Bestellungen kann durch ein Datum, auf bestimmte Lieferanten und/oder Nummernverwalter eingeschränkt werden.

Für die Mahnung müssen Sie denselben Kommunikationsweg wählen, über den Sie auch die Bestellungen an den jeweiligen Lieferanten übermitteln. Dabei gilt:
*   **Faxversand:** Die Bestellungen werden aus A+W Business direkt auf ein Faxgerät gesendet und an den Lieferanten übermittelt.
*   **Postversand:** Die Bestellungen werden aus A+W Business direkt auf einen Drucker gesendet.

Die Mahnung wird immer für alle Bestellungen erstellt, die anhand der Suchkriterien ausgewählt wurde. Dabei werden die Bestellungen pro Lieferant zu einer Mahnung zusammengefasst.

### Auftragsbestätigung erfassen

Zu einer Bestellung erfassen Sie die Auftragsbestätigung (AB) Ihres Lieferanten und setzen damit den Status der Bestellung hoch.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So erfassen Sie die Auftragsbestätigung für eine Bestellung insgesamt" auf Seite D-2123
*   "So erfassen Sie die Auftragsbestätigung für eine Bestellposition" auf Seite D-2125

**So erfassen Sie die Auftragsbestätigung für eine Bestellung insgesamt**

1.  Wählen Sie **Dokumente > Bestellung > AB Lieferant**.

*Abb. D-47: AB des Lieferanten erfassen*
*   **A Modus der Suche**
*   **B Dokumentennummer**

⇨ Softwarereferenz, "AB-Lieferant" auf Seite D-2234

2.  Wählen Sie die Option (A), mit der Sie die Suche nach offenen Bestellungen starten möchten, z. B. **Bestellnummer**.
3.  Tragen Sie die Bestellnummer (B) ein und springen Sie mit `<Tab>` in das nächste Feld.
    Die Daten werden eingelesen und angezeigt.

*Abb. D-48: AB-Lieferant - Dokumente*
*   **A Ziel-Nummernverwalter**
*   **B Wareneingang komplett buchen**
*   **C Anliefertermin aus der AB**
*   **D Nummer der AB**

4.  Wählen Sie den Ziel-Nummernverwalter (A) für Aufträge oder für Bestellungen, wenn die entsprechenden Dokumente in andere Nummernverwalter gestellt werden sollen.
5.  Markieren Sie die Checkbox **Wareneingang buchen (B)** nur, wenn Sie gleichzeitig den gesamten Wareneingang dieser Bestellung verbuchen möchten.
    Mit dieser Einstellung können Sie keinen teilweisen Wareneingang erfassen. Der Wareneingang ist in einer separaten Einheit beschrieben.
    ⇨ "Wareneingang erfassen" auf Seite D-2161
6.  Prüfen Sie die Termine (C) in den Bereichen **Bestelldaten** und **Auftragsdaten** und korrigieren Sie diese ggf.
7.  Tragen Sie die Nummer der Auftragsbestätigung (D) ein, die der Lieferant Ihnen geschickt hat.
8.  Wählen Sie im Menü **Start > Ausführen**, um die Daten zu speichern.
    Die Daten werden gespeichert. Die AB-Nummer wird in der Übersicht angezeigt.
    Wenn Sie gleichzeitig einen Wareneingang gebucht haben, wird der Status der Bestellung entsprechend umgesetzt.

**So erfassen Sie die Auftragsbestätigung für eine Bestellposition**

1.  Füllen Sie die Felder wie in Schritt 2 bis 6 der vorigen Handlungssequenz beschrieben.
2.  Wechseln Sie zum Register **Positionen**.

*Abb. D-49: AB-Lieferant - Positionen*
*   **A Positionsnummern**
*   **B Termin der Teillieferung**

3.  Tragen Sie die Nummer(n) der Positionen (A) ein, für die Sie die AB erhalten habe.
    Wenn Sie keine lückenlose Folge von Nummern haben, müssen Sie die Schritte für jede Position einzeln wiederholen, z. B. für Position 1, 3 und 7.
4.  Tragen Sie im Feld **Teilliefertermin** das Datum für die Lieferung der Positionen ein.
5.  Wählen Sie im Menü **Start > Ausführen**, um die Daten zu speichern.

*Abb. D-50: AB-Lieferant - Teillieferung*
*   **A AB-Nummer**
*   **B Bestätigter Termin**

Die Daten werden gespeichert. Die Nummer der AB und der Teilliefertermin werden in der Übersicht angezeigt.

### AB erfassen und Preise prüfen

Die Preise können sowohl auf Basis der Auftragsbestätigung des Lieferanten als auch auf Basis der Lieferantenrechnung geprüft werden. Die Dialoge **Preiskontrolle** und **Rechnungskontrolle** sind identisch aufgebaut.

Ihr Lieferant kann in einer AB mehrere Bestellungen bestätigt haben. Diese können Sie im Dialog **Preiskontrolle** sammeln und gemeinsam kontrollieren.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So erfassen Sie eine Lieferanten-AB und prüfen die Preise" auf Seite D-2127
*   "So erfassen Sie eine Sammel-AB Ihres Lieferanten" auf Seite D-2129

Die Preis- und Rechnungskontrolle ist ausführlich in einer separaten Einheit beschrieben.
⇨ "Rechnung kontrollieren" auf Seite D-2180

**So erfassen Sie eine Lieferanten-AB und prüfen die Preise**

1.  Wählen Sie **Dokumente > Bestellungen > Auftragsbestätigung > Preiskontrolle**.

*Abb. D-51: AB-Nummer des Lieferanten erfassen und Preise prüfen*
*   **A Daten aus der Auftragsbestätigung**
*   **B Bestätigte Summe**
*   **C Anzeigemodus für Preise**
*   **D Bestellung(en) suchen**

⇨ Softwarereferenz, "Rechnungskontrolle - Bestellungen" auf Seite D-2285

2.  Geben Sie die Nummer der Auftragsbestätigung (A) Ihres Lieferanten und den bestätigten Anliefertermin ein.
3.  Geben Sie die Bestellnummer (D) ein und springen Sie mit `<Tab>` in das nächste Feld.
    In der Übersicht **Bestellungen** wird die Bestellung angezeigt.
    Wenn in der AB mehrere Bestellungen zusammengefasst sind, können Sie nacheinander alle Bestellnummern angeben. Dies ist in der nachfolgenden Handlungssequenz beschrieben.
4.  Geben Sie im Feld **AB-Summe (B)** den Betrag ein, den Ihr Lieferant bestätigt hat.
    Der Betrag muss identisch mit dem aus der Bestellung angezeigten Betrag sein. Wenn der Lieferant einen anderen Betrag angegeben hat, den Sie akzeptieren wollen, müssen Sie die Preise in der Bestellung ändern. Sie können diese Änderung im Register **Positionen** erfassen.
    Achten Sie darauf, dass der Modus (C) für die Anzeige der Beträge richtig eingestellt ist.

> **Währung**
> Wenn Sie nur mit einer Währung (EUR) arbeiten, muss im Feld **Kurs** 1 eingetragen sein.

*Abb. D-52: AB-Nummer des Lieferanten erfassen und Preise prüfen*
*   **A AB-Summe**
*   **B Betrag aus der Bestellung**

5.  Wählen Sie im Menü **Start > Ausführen**, um die Eingabe zu bestätigen.
    Der Betrag wird geprüft und das Register **Positionen** wird angezeigt.

*Abb. D-53: Preise der Bestellpositionen prüfen*
*   **A Positionspreis**
*   **B Differenz über alle Positionen**

Wenn Sie einen Positionspreis ändern müssen, überschreiben Sie den Betrag in der entsprechenden Position (A). Diese Änderung wird in die Bestellung zurückgeschrieben.

6.  Wählen Sie im Menü **Start > Ausführen**, wenn keine Differenz (mehr) angezeigt wird (B).
    Die Daten werden gespeichert und der Status der Bestellung wird umgesetzt. Anschließend wird das Register **Bestellungen** wieder angezeigt und Sie können die nächste AB erfassen. Die Preiskontrolle für diese Bestellung kann nicht nochmals durchgeführt werden.

**So erfassen Sie eine Sammel-AB Ihres Lieferanten**

> **Bestellungen sammeln**
> Sie können die Bestellungen, die in der AB des Lieferanten aufgeführt sind, in einem Nummernverwalter sammeln und diesen im Bereich **Bestelldaten** auswählen.
> Alternativ dazu können Sie die Bestellungen im Dialog **Preiskontrolle** sammeln. Dieses Vorgehen ist in den nachfolgenden Handlungsschritten beschrieben.

1.  Geben Sie im Dialog **Preiskontrolle** die Nummer der Auftragsbestätigung Ihres Lieferanten und den Anliefertermin ein, wie oben beschrieben.
    Wenn Sie die Bestellungen in einem Nummernverwalter gesammelt haben, so wählen Sie diesen aus und fahren mit Schritt 5 fort.
2.  Geben Sie die Nummer der ersten Bestellung ein und warten Sie, bis diese eingelesen wurde.
3.  Geben Sie nun die Nummer der nächsten Bestellung ein, die auf der AB aufgeführt ist.
    Die Bestellung wird in der Übersicht der Bestellungen hinzugefügt. Sie können jedoch nur Bestellungen mit identischem Steuersatz zusammenfassen.
4.  Wiederholen Sie diesen Schritt, bis alle Bestellungen in der Übersicht aufgeführt sind.
    Sie können eine Bestellung aus der Übersicht wieder entfernen, indem Sie den Eintrag markieren und auf `<Entf>` drücken.

*Abb. D-54: AB-Nummer des Lieferanten erfassen und Preise prüfen*

5.  Geben Sie den Betrag ein, den Ihr Lieferant bestätigt hat.
    Der Betrag muss identisch mit der Summe der aufgeführten Bestellungen sein.
6.  Wählen Sie im Menü **Start > Ausführen**, um die Eingabe zu bestätigen.
    Der Betrag wird geprüft und das Register **Positionen** wird angezeigt. Wenn Sie einen Positionspreis ändern müssen, überschreiben Sie den Betrag in der entsprechenden Position. Diese Änderung wird in die Bestellung zurückgeschrieben.
7.  Wählen Sie im Menü **Start > Ausführen**, wenn keine Differenzen (mehr) angezeigt werden.
    Die Daten werden gespeichert und der Status der Bestellungen wird umgesetzt.

### Lieferanten anmahnen

Für die korrekte Verarbeitung Ihrer Bestellungen werden Auftragsbestätigungen und Lieferungen erfasst. Säumige Lieferanten können Sie anmahnen.

> **Bestellungen sammeln**
> Sie können die Bestellungen, die in der AB des Lieferanten aufgeführt sind, in einem Nummernverwalter sammeln.

**So mahnen Sie einen Lieferanten an**

1.  Wählen Sie **Dokumente > Bestellungen > Auftragsbestätigung > Mahnung**.

*Abb. D-55: Lieferanten mahnen*
*   **A Lieferant**
*   **B Nummernverwalter mit den überfälligen Bestellungen**
*   **C Eingrenzung der Auswahl auf einen Statusbereich**
*   **D Lieferanten (nicht) erneut mahnen**
*   **E Erfassungsdatum der Bestellung**
*   **F Versandwege der Bestellung**

⇨ Softwarereferenz, "Mahnung" auf Seite D-2262

2.  Filtern Sie die Anzeige:
    *   nach Lieferanten (A)
    *   nach einem Nummernverwalter (B)
3.  Wählen Sie in den Feldern **Mindeststatus** und **Status kleiner (C)** einen Statusbereich für die Bestellungen aus, deren Lieferung Sie anmahnen wollen.
    Ein Kriterium für den Mindeststatus könnte sein, dass die Bestellung gedruckt wurde oder dass die AB erfasst wurde.
    Ein Kriterium für den anderen Status sollte vor dem Status **Wareneingang** erfasst liegen.
4.  Grenzen Sie die Auswahl der Bestellungen auf ein Datum (E) ein.
    Standardmäßig wird das aktuelle Tagesdatum angezeigt.
5.  Wenn Sie die bereits gemahnten Lieferanten nicht nochmals mahnen wollen, deaktivieren Sie die Checkbox (C) für dieses Kriterium.
    Die bereits gemahnten Lieferanten werden dann in der Trefferliste nicht angezeigt. Wenn die Checkbox markiert ist, werden diese Lieferanten in roter Schrift angezeigt. Die ausstehenden Lieferungen werden dann nochmals angemahnt.
6.  Wählen Sie die Option (F) aus, mit der Sie Bestellungen gesendet haben.
    Wenn Sie die Bestellungen an Ihre Lieferanten auf unterschiedliche Weise senden, beachten Sie den Kommunikationsweg für den ausgewählten Lieferanten.
    Die Option **Alle** ist dann sinnvoll, wenn Sie die Bestellungen auf unterschiedliche Arten an die Lieferanten senden und die Auswahl auf keinen bestimmten Lieferanten eingeschränkt haben.
7.  Wählen Sie im Menü **Start > Suchen**, um in die Suche zu starten.

*Abb. D-56: Lieferanten zur Mahnung ausgewählt*

Die offenen Bestellungen werden in der Übersicht aufgelistet.

8.  Wählen Sie im Menü **Drucken** die gewünschte Ausgabeform.
    Die Mahnung wird erstellt.

*Abb. D-57: Mahnungen erstellt*

Anschließend werden alle Einträge in der Übersicht in roter Schrift dargestellt.

### Lieferterminkontrolle

> **Lernziele**
> *   Liefertermine zu referenzierten Dokumenten prüfen.
> *   Termine ändern.
> *   Kunde über die Änderung benachrichtigen.

> **Nutzen**
> *   In referenzierten Dokumenten brauchen Termine nur in einem Dokument geändert zu werden.
> *   Liefertermine können in verschiedenen Dialogen geändert werden. Bestellungen oder Aufträge, die in einem eigenen Nummernverwalter gesammelt sind, können geändert werden, ohne die Dokumente selbst zu öffnen.

> **Merke**
> **Terminänderungen in referenzierten Dokumenten**: Alle Änderungen in Bestellungen werden in die referenzierten Aufträge zurückgeschrieben. Dies gilt auch in der entgegengesetzten Richtung.
> **Dialog Kundenbenachrichtigung**: In diesem Dialog können Sie den Anliefertermin ändern und den Kunden benachrichtigen.
> **Dialog Dokumentendaten**: In diesem Dialog können Sie alle Termine in den Aufträgen und referenzierten Bestellungen anpassen. Zusätzlich können Sie die Tour in Aufträgen und mehrere Dokumente gemeinsam ändern.
> **Voreinstellungen**: Kundenstammdaten (Fax- oder Mail-Versand)

#### Prüfung und Korrektur von Lieferterminen

Ihr Lieferant wird die Termine aus Ihren Bestellungen bestätigen oder korrigieren. Die vom Lieferanten erhaltenen Auftragsbestätigungen und Liefertermine ordnen Sie den Bestellungen zu, indem Sie die Lieferanten-AB erfassen. Dabei werden die geänderten Termine automatisch in die referenzierten Dokumente übernommen.

Für die Benachrichtigung des Kunden können Sie den Dialog **Kundenbenachrichtigung** oder die Möglichkeiten im Menü **Kommunikation** nutzen – oder einfach anrufen.

Den Liefertermin selbst können Sie in verschiedenen Dialogen ändern:
*   Dokumentenverwaltung (Auftrag, Bestellung)
*   Dokumentendaten
*   Kundenbenachrichtigung (Lieferterminkontrolle)
*   AB Lieferant
*   Eingangskontrolle

Sie korrigieren die Termine in aller Regel in den Bestellungen, wodurch sie in die referenzierten Aufträge zurückgeschrieben werden.

#### Kundenbenachrichtigung

Sie können den Kunden aus dem Dialog **Kundenbenachrichtigung (Lieferterminkontrolle)** heraus über die Terminverschiebung informieren. Dazu muss in den Stammdaten des Kunden eine E-Mail-Adresse hinterlegt sein. Im Auftrag muss im Bereich Anschrift die Checkbox Mail aktiviert sein.

### Liefertermine ändern und Kunden benachrichtigen

Zu den Bestellungen und referenzierten Aufträgen müssen Sie Liefertermine prüfen, korrigieren und den ggf. den Kunden benachrichtigen, wenn die Termine nicht eingehalten werden können. Diese Schritte sind über den Dialog **Kundenbenachrichtigung** möglich.

Sie können ihn auf folgende Weise öffnen:
*   **Auftrag oder Bestellung > Funktionen > Gruppe Dokument > Lieferterminkontrolle**
*   **Dokumente > Kundenbenachrichtigung**

Wenn Sie auch die Termine für die Produktion prüfen und korrigieren wollen, können Sie den Dialog **Dokumentendaten** nutzen.
⇨ "So prüfen und ändern Sie die Dokumentendaten" auf Seite D-2139

**So ändern Sie den Liefertermin**

1.  Öffnen Sie ggf. den Auftrag, dessen Termine Sie prüfen wollen oder geändert haben.
2.  Wählen Sie **Dokumente > Kundenbenachrichtigung**.

*Abb. D-58: Liefertermin beim Kunden ändern*
*   **A Modus der Suche**
*   **B Geplantes Lieferdatum**

⇨ Verkauf, "Kundenbenachrichtigung (Lieferterminkontrolle)" auf Seite C-1848

3.  Wählen Sie die Option (A) **Aufträge** oder **Bestellungen** und ggf. den Nummernverwalter.
    Wenn in dem Nummernverwalter sehr viele Dokumente aufgelistet sind, können Sie die Anzeige auf das ursprünglich geplante Lieferdatum (B) einschränken.
4.  Wählen Sie im Menü **Start > Suchen**, um die Daten einzulesen.

*Abb. D-59: Liefertermine prüfen*
*   **A Kunde wurde noch nicht über den neuen Termin informiert**
*   **B Geplanter Liefertermin aus dem Auftrag**
*   **C Neuer Liefertermin**

5.  Markieren Sie den Auftrag, zu dem Sie den Liefertermin beim Kunden ändern müssen, und wechseln Sie zum Register **Terminverschiebung**.

*Abb. D-60: Liefertermin beim Kunden ändern*
*   **A Neuer Termin beim Kunden**
*   **B Auftrag, für den die Änderung gilt**

6.  Markieren Sie den Auftrag (B), zu dem der Kundentermin verschoben werden muss.
    Sie können mehrere Aufträge markieren, wenn diese alle denselben Liefertermin und dieselbe Tour haben.
7.  Tragen Sie den neuen Termin (A) ein und ändern Sie ggf. die Tour.
8.  Wählen Sie im Menü **Start > Speichern**, um die Änderung zu speichern.
    Sie können die Terminänderung für den Kunden drucken und auf dem üblichen Kommunikationsweg versenden.
9.  Wählen Sie über das Menü **Druck** den Drucker aus.
    Die Benachrichtigung wird erzeugt und kann versendet werden. Wenn Sie mehrere Termine geändert haben, wird pro Kunde eine Benachrichtigung erstellt.

### Alle Termine prüfen und ändern

Im Dialog **Dokumentendaten** können Sie sich alle Bestellungen und Aufträge anzeigen lassen, um neben den Lieferterminen auch die Produktionstermine zu prüfen und ggf. zu ändern. Wenn Sie in mehreren Aufträgen gemeinsam z. B. die Termine ändern wollen, können Sie die Aufträge sammeln.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So prüfen und ändern Sie die Dokumentendaten" auf Seite D-2139
*   "So sammeln Sie Dokumente für gemeinsame Änderungen" auf Seite D-2142

**So prüfen und ändern Sie die Dokumentendaten**

1.  Wählen Sie **Dokumente > Dokumentendaten**.
    ⇨ Verkauf, "Dokumentendaten" auf Seite C-2031

*Abb. D-61: Termine für Auftrag mit Bestellpositionen prüfen*
*   **A Dokumententyp**
*   **B Nummer des gesuchten Dokuments**

2.  Wählen Sie den Dokumententyp, z. B. **Auftrag** oder **Bestellung**.
    Sie können sich auch alle Aufträge in einem Nummernverwalter anzeigen lassen. In diesem Beispiel soll ein einzelner Auftrag geprüft werden.
    Sie können die Termine für mehrere Aufträge und/oder Bestellungen ändern, die nicht in einem gemeinsamen Nummernverwalter stehen.
    ⇨ "So sammeln Sie Dokumente für gemeinsame Änderungen" auf Seite D-2142
3.  Geben Sie die Auftragsnummer ein und übernehmen Sie die Daten mit `<Enter>`.

*Abb. D-62: Termine für Auftrag mit Bestellpositionen prüfen*
*   **A Kundentermine**
*   **B Neuer Termin des Lieferanten**

In den Feldern im Bereich **Auftrag** werden die Daten aus dem Auftragskopf angezeigt. In den Feldern im Bereich **Bestellung** werden die Daten aus der Bestellung angezeigt.
4.  Passen Sie den Lieferantentermin (B) und die Kundentermine (A) an.
    Wenn Sie die Termine über den Kalender auswählen, können Sie die Tourentage für den Kunden berücksichtigen.
5.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die neuen Termine werden gespeichert und in die zugehörigen Dokumente übernommen.

*Abb. D-63: Geänderte Termine*

Sie können jetzt den Kunden über den geänderten Termin informieren.

**So sammeln Sie Dokumente für gemeinsame Änderungen**

1.  Wählen Sie **Dokumente > Dokumentendaten**.

*Abb. D-64: Termine für Auftrag mit Bestellpositionen prüfen*
*   **A Dokumententyp**
*   **B Nummer des gesuchten Dokuments**
*   **C Nummernverwalter nicht markieren**

2.  Wählen Sie den Dokumententyp aus, z. B. **Auftrag (A)**.
3.  Stellen Sie sicher, dass die Checkbox (C) **Nummernverwalter** nicht markiert ist.
4.  Geben Sie die Auftragsnummer (B) ein und übernehmen Sie die Daten mit `<Enter>`.
    In der Übersicht werden die Daten des Auftrags angezeigt. Im Bereich **Bestellung** werden die referenzierten Bestellungen aufgelistet.
5.  Wiederholen Sie diesen Schritt, bis Sie alle Aufträge zusammengestellt haben, die Sie gemeinsam ändern wollen.
    Achten Sie darauf, dass alle Aufträge mit derselben Tour geliefert werden können und dasselbe Lieferdatum haben.

*Abb. D-65: Aufträge für gemeinsame Terminänderung*
*   **A Termine der Aufträge**
*   **B Termin der Bestellung**

In der Übersicht werden alle Aufträge aufgelistet.
6.  Markieren Sie alle aufgelisteten Aufträge, indem Sie die `<Strg>`-Taste gedrückt halten.
7.  Ändern Sie die Termine (A, B).
8.  Prüfen Sie die Tour und ändern Sie diese ggf.
9.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die neuen Termine werden in alle aufgelisteten Aufträge und referenzierten Bestellungen übernommen. Sie können jetzt die Kunden benachrichtigen.

### Anfrage

> **Lernziele**
> *   Anfragen beim Lieferanten einholen.
> *   Aus einer Anfrage eine Bestellung erzeugen.
> *   Anfragen zu einer Bestellposition einholen.

> **Nutzen**
> *   Anfragen können zur Abstimmung von Terminen und Kapazitäten über den Bestellpool erzeugt werden.
> *   Aus einer Anfrage kann eine Bestellung erzeugt werden, ohne die Daten neu zu erfassen.

> **Merke**
> **Anfragen**: Wie bei den Bestellungen können Anfragen manuell erfasst oder über den Bestellpool aus einem Kundenauftrag heraus erzeugt werden.
> **Bestellung**: Aus jeder Anfrage kann eine Bestellung erzeugt werden.
> **Referenzen**: Die Referenz auf eine Auftragsposition bleibt in der Anfrage und in der Bestellung erhalten, wenn sie über den Bestellpool erzeugt werden. Wenn die Bestellung durch Kopieren aus einer Anfrage erzeugt wird, besteht die Referenz nur zwischen diesen beiden Dokumenten.
> **Voreinstellungen**: Stammdaten: Lieferant > Register Auftrag

#### Anfrage zu Bestellpositionen oder Bestellungen

Anfragen erstellen Sie genau wie eine Bestellung und senden Sie an den Lieferanten. Wenn das Angebot zurückkommt und angenommen werden soll, können Sie aus der Anfrage eine Bestellung erzeugen, ohne die Daten erneut eingeben zu müssen. Dazu nutzen Sie die Funktion **Dokument kopieren**.

Anfragen können Sie auch zu den Bestellpositionen aus einem Kundenauftrag erstellen.

*Abb. D-66: Anfrage - Bestellung (Flussdiagramm)*
*   *Auftrag Nr. 1167* -> *Bestellübergabe (Sofort anfragen)* -> *Anfrage* -> *Kopieren in* -> *Bestellung (keine Referenz auf Auftrag 1167)*
*   *Auftrag Nr. 1167* -> *Bestellpool* -> *Anfrage (Referenz auf Auftrag 1167)* -> *Bestellung (Referenz auf Auftrag 1167)*
*   *Unabhängige Anfrage* -> *Kopieren in* -> *Unabhängige Bestellung*

Wenn bei der Bestellübergabe die Option **Sofort Anfragen** gewählt wurde, werden auch aus einem Kundenauftrag Anfragen erzeugt. Wenn Sie dabei über den Bestellpool gehen, können Sie auch zu einzelnen Auftragspositionen eine Anfrage erstellen und einen bestimmten Lieferanten auswählen.

Aus so erstellen Anfragen können natürlich auch Bestellungen erzeugt werden. Die Referenz zum Auftrag bleibt jedoch nur erhalten, wenn entsprechenden Bestellungen wieder über den Bestellpool erzeugt werden.

Unabhängige Anfragen werden analog zu Aufträgen und Bestellungen erzeugt. Dazu steht im Modul **Dokumente** das Menü **Anfragen** zur Verfügung.

### Anfrage zu einer Bestellposition erzeugen

Sie können zu einer Bestellposition zunächst eine Anfrage erzeugen, z. B., um festzustellen, ob der Lieferant die Kapazitäten frei hat. Aus jeder Anfrage kann über den Bestellpool auch eine Bestellung erzeugt werden.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So erzeugen Sie eine Anfrage zu einem Kundenauftrag" auf Seite D-2146
*   "So erstellen Sie zu einer referenzierten Anfrage eine Bestellung" auf Seite D-2147

**So erzeugen Sie eine Anfrage zu einem Kundenauftrag**

1.  Wählen Sie **Dokumente > Auftrag > Bestellübergabe**.

*Abb. D-67: Aufträge aus dem Nummernverwalter übergeben*
*   **A Modus der Übergabe**
*   **B Nummernverwalter mit Aufträgen für die Übergabe**
*   **C Ziel-Nummernverwalter**

2.  Wählen Sie die den Modus **Sofort anfragen (A)** und den Nummernverwalter (B), in dem Sie die Aufträge mit Bestellpositionen gesammelt haben.
3.  Wählen Sie den Ziel-Nummernverwalter (C) aus, in den die Anfragen gestellt werden.
    Sie können einen neuen Namen eingeben und so einen neuen Nummernverwalter anlegen. Wenn Sie dazu einen anderen Mitarbeiter auswählen, wird der Nummernverwalter diesem zugeordnet.
4.  Wählen Sie ggf. im Bereich Ziel-Nummernkreis den Mandanten und den AV-Bereich aus.
5.  Wählen Sie im Menü **Start > Ausführen**, um die Positionen zu übergeben.
    Bestätigen Sie die Erfolgsmeldung.
    Für jede Bestellposition wurde eine Anfrage erzeugt. Die erzeugten Anfragen können Sie unter **Dokumente > Anfrage** öffnen, drucken und an den Lieferanten senden.

**So erstellen Sie zu einer referenzierten Anfrage eine Bestellung**

1.  Öffnen Sie den Dialog **Bestellübergabe**.

*Abb. D-68: Aufträge aus dem Nummernverwalter übergeben*
*   **A Modus der Übergabe**
*   **B Nummernverwalter mit Aufträgen für die Übergabe**
*   **C Ziel-Nummernverwalter**

2.  Wählen Sie den Nummernverwalter (B), in dem die Aufträge stehen, zu denen Sie Anfragen erzeugt haben.
3.  Wählen Sie die Option **Pool füllen (A)**.
4.  Wählen Sie im Menü **Start > Ausführen**, um die Aufträge in den Bestellpool zu stellen.
    Die Bestellpositionen werden eingelesen und die Anzeige wechselt zum Register **Bestellpool**.

*Abb. D-69: Bestellungen zu Aufträgen erzeugen*
*   **A Modus Bestellung**
*   **B Anfragen, die zum angezeigten Auftrag erzeugt wurden**
*   **C Ziel-Nummernverwalter**

Zu den Anfragepositionen aus dem Auftrag werden die Dokumenten-Nummern der Anfragen angezeigt.

5.  Markieren Sie die Option **Bestellung (A)** und wählen Sie den Ziel-Nummernverwalter (C) für Bestellungen aus.
6.  Markieren Sie die Positionen, für die eine Bestellung erstellt werden soll.
    Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf. Nur die Positionen sind markiert, die mit einem X gekennzeichnet sind.
7.  Wählen Sie im Menü **Start > Ausführen**, um die Bestellungen zu erzeugen.
    Die Bestellungen wurden erzeugt. Die übergebenen Positionen werden aus dem Bestellpool gelöscht.
    Die erzeugten Bestellungen können Sie unter **Dokumente > Bestellung** öffnen, drucken und an den Lieferanten senden.

### Bestellung aus unabhängiger Anfrage erstellen

Sie können aus jeder Anfrage durch Kopieren eine Bestellung erzeugen, unabhängig davon, ob die Anfrage referenziert ist oder nicht. Die Referenz auf einen Kundenauftrag wird dabei jedoch nicht übernommen.

Die Kopierfunktion ist ausführlich im Part Verkauf beschrieben.

**So erfassen Sie eine Bestellung zu einer Anfrage**

1.  Öffnen Sie die Anfrage, zu der Sie eine Bestellung erfassen möchten.
2.  Wählen Sie im Menü **Funktionen > Gruppe Dokument > Dokument kopieren**.

*Abb. D-70: Bestellung aus einer Anfrage erstellen*
*   **A Ziel-Dokumententyp**
*   **B Kopier-Modus**
*   **C Ziel-Nummernverwalter**

3.  Wählen Sie den Dokumententyp **Bestellung (A)** aus.
    Im Bereich **Ziel** wird automatisch der erste Nummernverwalter für Bestellungen angezeigt.
4.  Wählen Sie ggf. einen anderen Ziel-Nummernverwalter (C) aus.
5.  Prüfen Sie die weiteren Einstellungen.
6.  Wählen Sie im Menü **Start > Ausführen**, um die Bestellung zu erzeugen.
    Die Positionen werden geprüft und kopiert. Die Bestellung wird gespeichert.
7.  Schließen Sie den Dialog.
    Der Dialog **Dokumente kopieren** wird geschlossen und der Dialog **Dokumentenverwaltung** wird wieder angezeigt.
    In der Historie der Anfrage und der Bestellung wird die Referenz angezeigt. Die erzeugte Bestellung können Sie unter **Dokumente > Bestellung** öffnen, drucken und an den Lieferanten senden.

### Übungen

Die Übungen sind so konzipiert, dass Sie den gesamten Einkauf trainieren. Das bedeutet, dass Sie die Bestellungen, die Sie mit den Aufgaben erstellen, im nächsten Themenblock weiterbearbeiten.

> **Vorbedingungen und Stammdaten prüfen**
> Wenn Sie in Ihrer eigenen Anwendung arbeiten, stellen Sie bitte sicher, dass die Voreinstellungen in den Stammdaten den Bedingungen für einen reibungslosen Ablauf der Erfassung von Dokumenten und Wareneingängen genügen.
> Achten Sie auch darauf, dass der Status der Dokumente richtig umgesetzt ist, wenn sie weiterverarbeitet werden sollen, z. B. im Bestellpool.

**Bestellposition im Auftrag erfassen**

Erfassen Sie einen Kundenauftrag mit folgenden Positionen:
*   Positionen mit unterschiedlichen Bestellkennzeichen.
*   Positionen, die von unterschiedlichen Lieferanten geliefert werden können.
*   Positionen, die nicht bestellt werden müssen.

> **Tipp**
> Stellen Sie 2 bis 3 Kopien der Aufträge und der manuellen Bestellungen her, damit Sie die unterschiedlichen Auswirkungen von Änderungen prüfen können, z. B. die Änderung des Lieferanten auf unterschiedlichen Ebenen.

**Manuelle Bestellung erfassen**

Erfassen Sie eine Bestellung mit folgenden Positionen:
*   Positionen mit Lagerartikeln und Produkten, die nicht im Lager gepflegt werden.
*   Positionen mit unterschiedlichen Kisten.
*   Mindestens 5 Kisten pro Position.

**Auftrag an den Einkauf übergeben**

Übergeben Sie Aufträge an den Einkauf:
*   Mindestens einen Auftrag direkt (ohne Bestellpool).
*   Mindestens einen Auftrag über den Bestellpool.
*   Prüfen Sie anschließend die neuen Bestellungen auf Unterschiede.

**Auftragsbestätigung erfassen und Preise prüfen**

Erfassen Sie eine AB zu mindestens je einer referenzierten und einer manuellen Bestellung.
Liefertermine prüfen, ändern und Kunden benachrichtigen

Tragen Sie folgende Änderungen ein:
*   Tragen Sie in einer referenzierten Bestellung eine größere Stückzahl in einer Position ein und übergeben Sie Position erneut.
*   Wählen Sie einen anderen Lieferanten, weil der ursprüngliche die Termine nicht einhalten wird.
*   Ändern den Liefertermin in einer Bestellung und benachrichtigen Sie anschließend den Kunden über die Verzögerung.

**Lieferanten mahnen**

Suchen Sie nach Bestellungen, zu denen Sie noch keine AB erfasst haben, und mahnen Sie den Lieferanten.

**Ergänzende Informationen**
*   ⇨ "Lieferantenkartei" auf Seite D-2065
*   ⇨ "Lieferungen im Wareneingang" auf Seite D-2153
*   ⇨ "Kistengeschäft" auf Seite D-2170
*   ⇨ "Wareneingang von Kisten" auf Seite D-2169
*   ⇨ "Elektronischer Dokumentenaustausch" auf Seite D-2184

**Part Verkauf**
*   ⇨ Verkauf, "Dokumente kopieren" auf Seite C-1505
*   ⇨ Verkauf, "Dokumente kopieren" auf Seite C-1813
*   ⇨ Verkauf, "Auftrags-/Bestell-Info" auf Seite C-1845
*   ⇨ Verkauf, "Dokumentendaten" auf Seite C-2030

**Part Stammdaten**
*   ⇨ Stammdaten, "Produkt" auf Seite B-201
*   ⇨ Stammdaten, "Währungen" auf Seite B-530
*   ⇨ Stammdaten, "Lagermaße" auf Seite B-753
*   ⇨ Stammdaten, "Preise" auf Seite B-839
*   ⇨ Stammdaten, "Partnerverwaltung" auf Seite B-887
*   ⇨ Stammdaten, "Firmendaten" auf Seite B-1055
*   ⇨ Stammdaten, "Pos. ohne Lagerkennz. im WE anzeigen bei Lagerbestell." auf Seite B-1098

**Part Lagerwirtschaft**
*   ⇨ Lagerwirtschaft, "Lagerverwaltung" auf Seite G-2743
*   ⇨ Lagerwirtschaft, "Lagerbestellung (automatisch)" auf Seite G-2782
*   ⇨ Lagerwirtschaft, "Lagerverwaltung - Lagerartikel" auf Seite G-2863
*   ⇨ Lagerwirtschaft, "Lagerbewegung - Abgang, Zugang" auf Seite G-2874

## Lieferungen im Wareneingang

In diesem Themenblock lernen Sie, wie Sie die Preise und Rechnungen kontrollieren und den Wareneingang erfassen.

Dazu gehören folgende Lerneinheiten:
*   "Wareneingang" auf Seite D-2154
*   "Wareneingang von Kisten" auf Seite D-2169
*   "Preis- und Rechnungskontrolle" auf Seite D-2177

Üblicherweise gehören zum Wareneingang folgende Schritte:
*   Lieferung als Wareneingang erfassen.
*   Wareneingang auf ausstehende oder unvollständige Lieferungen prüfen.
*   Rechnung prüfen.
*   Übergabe der Dokumente an Archiv und Statistik.
*   Dokument aus der Hauptdatenbank löschen.

Diese Reihenfolge entspricht im Wesentlichen auch der Reihenfolge der Dialoganordnung in A+W Business. Einige der Schritte können jedoch in verschiedenen Dialogen ausgeführt werden. Sie sind daher in einer Lerneinheit zusammengefasst.

Die Preise auf der Auftragsbestätigung werden logischerweise vor dem Wareneingang geprüft. In diesem Tutorial wird die Preiskontrolle zusammen mit der Rechnungskontrolle beschrieben, da diese Dialoge gleich aufgebaut sind.

Die Archivierung der Dokumente ist bereits aus dem Part Verkauf bekannt und wird hier daher nicht mehr behandelt.

### Wareneingang

> **Lernziele**
> *   Dialog Wareneingang kennenlernen.
> *   Unterscheidung von Wareneingängen aus Lagerbestellungen und aus referenzierten Bestellungen kennenlernen.
> *   Wareneingänge auf Vollständigkeit prüfen.
> *   Vergessene Eingangsbuchungen nachholen.

> **Nutzen**
> *   Lieferungen müssen erfasst werden, damit die Kundenaufträge fertiggestellt und ausgeliefert werden können.
> *   Beim Erfassen von Wareneingängen aus Lagerbestellungen wird der Lagerbestand aktualisiert, so dass Sie sich immer über den aktuellen Bestand informieren können.
> *   Wareneingänge können trotz Differenzen zwischen den bestellten und den gelieferten Mengen erfasst werden.

> **Merke**
> **Unvollständige Lieferung**: Der Wareneingang kann teilweise erfasst werden, wenn die gelieferte Menge nicht der bestellten Menge entspricht.
> **Überzählige Stückzahlen**: Wenn die Liefermenge von Lagerartikeln (mit einer Lager-ID) die bestellte Menge einer Lagerbestellung überschreitet, wird diese Menge in den Lagerbestand gebucht. Der Wareneingang von Übermengen wird nur dann verbucht, wenn Sie die Checkbox akzeptieren markiert haben. Übermengen bei Kundenaufträgen müssen in den Stammdaten zugelassen und eingegrenzt werden.
> **Voreinstellungen**
> Firmendaten:
> *   Register Parameter
> *   Register Lager/EK/EDI
> Stammdaten (Übermengen):
> *   Kunde, Lieferant
> *   Produkt

#### Lieferungen

Bei der Erfassung von Wareneingängen wird zwischen Kisten, Lagerbestellungen, unabhängigen und referenzierten Bestellungen unterschieden.

| Wareneingang | Buchung, Status |
| :--- | :--- |
| **Lagerbestellung** | Buchung in Bestand |
| **Kiste** (Vergabe von IDs) | Buchung in Bestand, Status in ref. Dokumenten |
| **Referenzierte Bestellung** | Buchung in Bestand nur für Lagerartikel, Status in ref. Dokumenten |
| **Unabhängige Bestellung** | Keine Buchung in Bestand |

*Abb. D-71: Wareneingang und Lagerbuchungen*

Diese Unterscheidung dient in der Lagerverwaltung zur Pflege der Bestandsdaten.

Nach der Buchung des Wareneingangs werden sämtliche automatischen Zuschläge für die Bestellung überrechnet und gespeichert.

**Wareneingang von Lagerbestellungen**

Mit der Buchung des Wareneingangs von Lagerbestellungen werden die Stückzahlen im Lager aktualisiert. Im Dialog Lagerinfo werden neben den Lagerbeständen auch die reservierten Stückzahlen angezeigt. Damit haben Sie schon in der Positionserfassung einen Überblick über aktuelle und zukünftige Lagerbestände.

Auch Positionen einer Lagerbestellung mit Artikeln ohne Lagerkennzeichen werden im Wareneingang angezeigt und können verbucht werden. Diese Buchungen ändern jedoch nicht den Lagerbestand.

*Abb. D-72: Wareneingang – Bestellungen im Nummernverwalter*
*   **A Liefertermin der markierten Bestellung**
*   **B Vollständig gebuchter Wareneingang in blauer Schrift**
*   **C Hinweis auf Sperrstatus**
*   **D Referenzierter Auftrag zur markierten Bestellung**

**Bestellposition für die Produktion**

Wenn Sie in einem Kundenauftrag eine Bestellposition erfasst haben, die für die Produktion des Auftrags benötigt wird, kann dieser erst nach dem Wareneingang weiterbearbeitet werden. Wenn Sie den Wareneingang erfassen, muss daher eine Meldung an die Produktion gesendet werden, damit der Auftrag produziert wird.

Im Wareneingang können Sie dazu eine Option aktivieren, mit der die Übergabe automatisch angestoßen wird, sobald der Eingang dieser Position erfasst wurde.

Für Auftragspositionen mit dem Kennzeichen **Bestellung (komplett)** wird der Status umgesetzt und an den Auftrag weitergegeben, damit der Auftrag ggf. ausgeliefert werden kann.

#### Positionen ohne Lagerkennzeichen

Wenn Sie Lagerbestellungen mit Positionen erfassen, die nicht als Lagerartikel geführt werden, werden diese im Wareneingang nicht angezeigt. Sie können in den Firmendaten jedoch die entsprechende Option aktivieren.

*Abb. D-73: Firmendaten – Register Lager/EK/EDI, Anzeige im Wareneingang aktivieren*

#### Teilweiser Wareneingang

Der Wareneingang kann vollständig oder auch teilweise gebucht werden. Der teilweise Wareneingang kann sowohl einzelne Positionen insgesamt betreffen als auch Teillieferungen zu einzelnen Positionen, z. B. die Positionen 5 und 7 einer Bestellung oder 15 Stück einer Position mit bestellten 30 Stück. Der Status der Bestellung und/oder des Auftrags wird danach entsprechend gesetzt.

#### Wareneingang von Stücklisten-Komponenten

Stücklisten-Komponenten werden nicht einzeln im Wareneingang aufgeführt, sondern gehören zu ihrem jeweiligen Hauptprodukt. In der Artikelbezeichnung werden die Stücklisten-Komponenten mit "/" getrennt aufgeführt.

#### Lieferung mit Übermengen

Wenn ein Lieferant eine größere Stückzahl (Übermenge) zu einer bestellten Position liefert, können Sie diese Lieferung im Wareneingang erfassen. Wenn es sich dabei um Lagerartikel (mit einer Lager-ID) aus einem Dokument vom Typ Lagerbestellung handelt, werden die gelieferten Stückzahlen in den Lagerbestand gebucht. In der Bestellung selbst werden die Stückzahlen dabei entsprechend geändert.

Dies gilt entsprechend auch für Untermengen, die jedoch in der Praxis eher selten vorkommen.

Die Über- und Untermengen werden in folgenden Dialogen festgelegt:
*   **Pro Kunde und pro Produkt:** prozentuale Höhe der Abweichung.
*   **Pro Produkt:** prozentuale Höhe der Abweichung.
*   **Pro Auftragsposition:** zusätzlich abweichende Menge.

#### Eingangskontrolle

Einen schnellen Überblick über offene oder unvollständige Lieferungen können Sie sich über den Dialog **Eingangskontrolle** anzeigen lassen.

*Abb. D-74: Kontrolle des Wareneingangs*
*   **A Bestellnummer**
*   **B Bestellte Menge**
*   **C Gelieferte Menge**
*   **D Wareneingang komplett**

Sie können die Buchung für Bestellungen oder Bestellpositionen nachholen, für die der Wareneingang noch nicht erfasst wurde, obwohl die Lieferung eingetroffen ist.

### Voreinstellungen für Wareneingang prüfen

In den Firmendaten müssen die Voreinstellungen festgelegt werden, die sich auf den Wareneingang beziehen. Die entsprechenden Parameter und Optionen finden Sie in folgenden Registern:
*   Parameter
*   Lager/EK/EDI

*Abb. D-75: Firmendaten – Register Parameter*
*   **A Virtuelle Positionsnummern für den Wareneingang von Kisten**

Die virtuellen Positionsnummern werden erzeugt, damit der Wareneingang von Kisten korrekt verbucht werden kann. Diese Funktion wird in der Lerneinheit für den Wareneingang von Kisten beschrieben.
⇨ "Wareneingang von Kisten" auf Seite D-2169

#### Lagerbestand

Um den Lagerbestand mit den Eingangsbuchungen aktualisieren zu können, müssen in den Firmendaten die Reservierungsoption und die Lagerführung auf Stücklistenebene aktiviert werden.

*Abb. D-76: Firmendaten – Register Lager/EK/EDI*
*   **A Reservierung mit Bestandsaktualisierung**
*   **B Lagerführung auf Stücklistenebene**

### Wareneingang erfassen

Mit dem Wareneingang können Sie auch die Nummer der Auftragsbestätigung (AB) des Lieferanten erfassen und den Liefertermin ändern. Teillieferungen erfassen Sie, indem Sie die gelieferte Stückzahl einer Position angeben oder nur einzelne Positionen als vollständig geliefert kennzeichnen.

> **Erfassung im Wareneingang**
> In der Regel werden die Dokumentennummern über den Barcode-Scanner erfasst. Bei den folgenden Beispielen werden sie manuell erfasst. Alle weiteren Handlungsschritte sind für die beiden Varianten identisch.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So erfassen Sie einen Wareneingang ganz" auf Seite D-2162
*   "So erfassen Sie einen Wareneingang teilweise" auf Seite D-2164

**So erfassen Sie einen Wareneingang ganz**

1.  Wählen Sie **Dokumente > Bestellung > Wareneingang > Wareneingang**.

*Abb. D-77: Wareneingang - Auswahl nach Nummernverwalter*
*   **A Auswahl nach Nummernverwalter**
*   **B Auswahl des Nummernverwalters**

⇨ Softwarereferenz, "Wareneingang (Dialog)" auf Seite D-2264

2.  Wählen Sie im Bereich **Auswahl** die Option **nach Nummernverwalter**.
3.  Wählen Sie im Menü **Start > Ausführen**, um die Daten einzulesen.
    Die Anzeige wechselt zum Register **Komplett**, in dem die Bestellungen angezeigt werden, die im Nummernverwalter stehen.

*Abb. D-78: Wareneingang - Bestellungen*
*   **A Anliefertermin und AB der markierten Bestellung**
*   **B Hinweis auf Sperrstatus**
*   **C Checkbox für vollständigen Wareneingang**
*   **D Anzeige für Kisten in der Bestellung**

Die Felder im Bereich **Liefertermin (A)** sind gesperrt, wenn zu der markierten Bestellung eine Auftragsbestätigung des Lieferanten erfasst wurde.

4.  Markieren Sie die Bestellung, zu der Sie den Wareneingang erfassen möchten.
    Die Felder im Bereich **Liefertermin (A)** werden freigeschaltet. In der Regel sind der Anliefertermin und die AB-Nummer des Lieferanten bereits erfasst. Sie können diese Daten jedoch nachtragen, falls sie noch fehlen.
5.  Markieren Sie die Checkbox **komplett buchen (C)**.

*Abb. D-79: Wareneingang - Bestellung komplett melden*

6.  Wählen Sie im Menü **Start > Ausführen**, um den Wareneingang zu erfassen.
    Die Daten werden gespeichert und der Status der Bestellung wird umgesetzt. Bei Lagerartikeln wird der Lagerbestand aktualisiert. Bei referenzierten Bestellungen wird der Wareneingang an die Produktion und/oder den Verkauf übergeben, um den zugehörigen Kundenauftrag weiterzubearbeiten oder abzuschließen.

**So erfassen Sie einen Wareneingang teilweise**

1.  Wählen Sie **Dokumente > Bestellung > Wareneingang > Wareneingang**.
2.  Wählen Sie im Bereich **Auswahl** die Option **nach Bestellnummer (A)** und geben Sie die Bestellnummer (B) ein.

*Abb. D-80: Wareneingang – Auswahl*
*   **A Auswahl nach Bestellnummer**
*   **B Nummer der Bestellung**

3.  Wählen Sie im Menü **Start > Ausführen**, um die Daten einzulesen.
    Die Daten werden eingelesen und die Anzeige wechselt zum Register **Komplett**.
    Wenn Sie öfter nur über die Bestell- oder Auftragsnummer gehen, können Sie im Menü **Optionen** einstellen, dass die Anzeige nach dem Einlesen des Dokuments zum Register **Positionsweise** wechselt.
4.  Wechsel Sie ggf. zum Register **Positionsweise**.

*Abb. D-81: Wareneingang - Teilmenge der Bestellung melden*
*   **A Position komplett buchen**
*   **B Lagerort für Lagerartikel**
*   **C Teilmenge als Wareneingang erfassen**
*   **D Bereits gelieferte Menge**
*   **E Über- oder Untermengen akzeptieren**
*   **F Nummer der Auftragsbestätigung**

Alle Positionen der Bestellung werden angezeigt. Sie haben folgende Möglichkeiten, einen teilweisen Wareneingang zu erfassen:
*   Eine der Bestellpositionen komplett buchen (A).
*   Zu einer Position eine Teilmenge (C) der bestellten Stückzahl erfassen.

Wenn die Lieferung z. B. bei einer Lagerbestellung nicht exakt der Bestellmenge entspricht, können Sie die Über- oder Untermenge akzeptieren (E), und so den Wareneingang einer Position komplett buchen.

5.  Markieren Sie die Position, zu der Sie den Wareneingang erfassen wollen.
6.  Tragen Sie im Feld **Menge Eingang (C)** die Stückzahl der gelieferten Position ein oder markieren Sie die Checkbox **komplett buchen (A)**, um die gesamte Position als geliefert zu melden.
7.  Tragen Sie ggf. AB-Nummer des Lieferanten (F) ein.
8.  Wählen Sie bei Lagerartikeln den Lagerort (B) aus.

*Abb. D-82: Wareneingang – Teilmenge der Bestellung melden*

9.  Wählen Sie im Menü **Start > Ausführen**, um die Daten zu speichern.
    Der teilweise Wareneingang wird verbucht.
    Die Bestellpositionen werden in blauer Schrift angezeigt, wenn die Bestellung/Position komplett geliefert ist.
    Änderungen werden in die Bestellung und ggf. in den referenzierten Kundenauftrag übernommen.
    Eine Übermenge wird in die Bestellung zurückgeschrieben, ein referenzierter Auftrag bleibt davon unberührt. Im Lager wird die Übermenge nur bei Lagerartikeln aus einer Lagerbestellung automatisch verbucht. Dies gilt ebenso für Untermengen, jedoch wird dann in der Praxis eher eine Teillieferung erstellt und die fehlende Menge beanstandet.

### Wareneingang kontrollieren

Sie müssen die Vollständigkeit der Lieferungen prüfen, um festzustellen, welche Bestellungen weiterverarbeitet werden können. Wenn Sie wissen, dass die Lieferung tatsächlich gekommen ist, können Sie den Wareneingang nachträglich erfassen. Sie können folgende Sachverhalte prüfen:
*   Komplette Bestellungen pro Nummernverwalter
*   Mengendiskrepanzen pro Bestellposition

**So kontrollieren Sie den Wareneingang**

1.  Wählen Sie **Dokumente > Bestellung > Wareneingang > Eingangskontrolle**.

*Abb. D-83: Eingangskontrolle – Komplette Bestellung*

⇨ Softwarereferenz, "Eingangskontrolle" auf Seite D-2278

2.  Wählen Sie im Register **Komplette Bestellungen** den Nummernverwalter für die Bestellungen aus.
    In der Übersicht **Wareneingang komplett** werden alle Bestellungen aufgelistet, deren Bestellungen vollständig erfasst sind.
3.  Wechseln Sie zum Register **Mengendiskrepanzen**, um sich die unvollständigen Positionen anzeigen zu lassen.

*Abb. D-84: Eingangskontrolle – Mengendiskrepanzen*
*   **A Teilgelieferte Menge**
*   **B Wareneingang komplett buchen**

In der Übersicht werden alle Bestellungen aufgelistet, zu denen noch kein oder ein unvollständiger Wareneingang gebucht wurde.

Wenn Sie die Bestellungen beim Buchen des kompletten Wareneingangs in einen Ziel-Nummernverwalter geschoben haben, sollten hier keine Diskrepanzen angezeigt werden.

4.  Holen Sie ggf. versäumte Buchungen nach, indem Sie die Checkbox **OK (B)** markieren.
    Beachten Sie dabei, dass Sie nur komplette Wareneingänge nachholen können. Um Teilmengen zu erfassen, wechseln Sie zum Dialog **Wareneingang**.
5.  Wählen Sie im Menü **Start > Ausführen**, um den Wareneingang zu buchen.
    Der Wareneingang wird verbucht. Die vollständig verbuchten Bestellungen werden aus der Liste entfernt.

> **Ergänzende Informationen**
> *   ⇨ Stammdaten, "Pos. ohne Lagerkennz. im WE anzeigen bei Lagerbestell." auf Seite B-1098
> *   ⇨ Stammdaten, "Lagerführungsmodus" auf Seite B-1099
> *   ⇨ Verkauf, "Lagerinfo" auf Seite C-2034
> *   ⇨ Softwarereferenz, "Wareneingang" auf Seite D-2264

### Wareneingang von Kisten

> **Lernziele**
> *   Sinn der Dummy-Kiste kennenlernen.
> *   Vergabe von Identnummern (IDs) kennenlernen.
> *   Einstellungen für automatische Vergabe der Kisten-ID kennenlernen.

> **Nutzen**
> *   Jede Kiste erhält im Wareneingang eine ID, damit sie im Lagerbestand eindeutig identifiziert und für einen Auftrag reserviert werden kann.
> *   Die IDs können manuell oder automatisch vergeben werden. Sie können dabei auch die Kisten-ID des Lieferanten übernehmen.

> **Merke**
> **Virtuelle Positionsnummern**: Wenn die Stückzahl einer Kistenposition größer als 1 ist, wird für jede Kiste eine Unterposition erzeugt. Diese Unterpositionen erhalten virtuelle Positionsnummern, die sich aus der Positionsnummer und der Anzahl der Kisten zusammensetzt, z. B. 1.1, 1.2 oder 3.1, 3.2 usw.
> **ID**: Bei der Erfassung des Wareneingangs wird für die Kiste jeder Unterposition eine eigene Identnummer (ID) vergeben.
> **Kisten identifizieren**: Nur eine Kiste mit einer ID kann als Lagerbestand gebucht und/oder einer Auftragsposition zugeordnet werden.
> **Voreinstellungen**:
> Stammdaten:
> *   Produktverwaltung
> Firmendaten:
> *   Register Parameter
> *   Register Lager/EK/EDI

#### Kistengeschäft

Für Kisten werden in der Regel Identnummern (ID) vergeben, die entweder vom Lieferanten stammen können oder im eigenen System gepflegt werden. Diese IDs werden beim Wareneingang von Kisten erfasst. Jede Kiste wird mit einer eigenen Kisten-ID verbucht und im Lager geführt.

Auch wenn die Anzahl von Kisten in einer Bestellposition größer als 1 ist, wird jede Kiste als ein eigener Wareneingang verbucht. Dazu legt das System automatisch Unterpositionen (virtuelle Positionen) zu der ursprünglichen Position an und ordnet jeder dieser Positionen genau eine Kiste zu. Diese Funktion muss in den Firmendaten aktiviert werden.

Zu jeder Unterposition muss eine eigene Kisten-ID angegeben werden, damit der Lagerbestand der Kisten gepflegt werden kann. Diese Kisten-IDs können nach selbst definierten Vorgaben automatisch eingefügt werden. Eine ID kann jedoch auch manuell eingegeben werden, z. B. um die Kisten-ID aus dem Lieferschein des Lieferanten zu übernehmen.

Im Rahmen des Wareneingangs kann im Dialog zur automatischen Kisten-ID auch ein Produktionsdatum angegeben werden. Für beschichtetes Glas wird dieses zur Berechnung des Verfallsdatums herangezogen, damit nach dem FiFo-Prinzip gearbeitet werden kann (FiFo = First in - First out).

Nach der Vergabe der IDs können über die Druckfunktion die Kistenetiketten mit den IDs als Barcode gedruckt und an den entsprechenden Kisten angebracht werden.

In der Regel werden die Barcodes von Kisten beim Warenausgang oder bei der Auflösung von Kisten gescannt. Damit ist der Bestand von Kisten nicht nur mengenmäßig aktuell, sondern die Kisten sind eindeutig identifiziert.

#### Firmendaten prüfen

Im Part Stammdaten ist ausführlich beschrieben, wie Sie die Stammdaten zu Ihrer Firma einrichten. In der folgenden Beschreibung wird daher nur auf die Besonderheiten eingegangen, die Sie für den Wareneingang von Kisten beachten müssen.

> **A+W Business neu starten**
> Nach Änderungen der Firmendaten sollten Sie A+W Business neu starten.

**So prüfen Sie die Firmendaten**

1.  Wählen Sie **Stammdaten > Firma > Firmendaten** und prüfen Sie im Register **Parameter** die Einstellung für die Checkbox **Virtuelle Positionsnummern verwenden**.
    Diese Einstellung ist bereits in der Lerneinheit Wareneingang dargestellt.
    ⇨ "Firmendaten - Register Parameter" auf Seite D-2160
2.  Wählen Sie im Menü **Start > Speichern**, um Änderungen zu speichern.
    Die Daten werden gespeichert.

#### Einstellungen für Identnummern prüfen

Wenn Sie die Kisten mit einer eigenen Kisten-ID erfassen wollen, können Sie diese ID automatisch vergeben lassen. Dazu müssen Sie die Einstellungen festlegen. Diese Einstellungen können vor jedem Wareneingang für Kisten angepasst werden, z. B. um die ID um ein Kennzeichen für den Lieferanten zu ergänzen.

Sie können maximal 20 Zeichen verwenden, die automatisch durch eine 5-stellige Zahl ergänzt werden. Die eingegebene Zeichenfolge bleibt so lange bestehen, bis sie manuell geändert wird. Wenn Sie also die Kisten-ID mit einem Kennzeichen für den Lieferanten versehen, müssen Sie darauf achten, die ID zu ändern, wenn Sie den Wareneingang von Kisten eines anderen Lieferanten erfassen.

**So prüfen Sie die Einstellungen für die automatische Vergabe von Identnummern**

1.  Wählen Sie **Dokumente > Bestellung > Wareneingang > Wareneingang**.
    Der Dialog **Wareneingang** wird geöffnet.
2.  Wählen Sie im Menü **Optionen > Gruppe Identnummernvergabe > Einstellungen**.

⇨ Softwarereferenz, "Einstellungen (ID)" auf Seite D-2277

3.  Tragen Sie das Kennzeichen ein.
    Achten Sie darauf, dass Sie die Platzhalter (X) für die Ziffern nicht überschreiben.
4.  Klicken Sie auf [OK], um die Änderung zu speichern.
    Der Dialog wird geschlossen. Die Einstellungen werden gespeichert und bleiben erhalten, bis sie erneut manuell geändert werden.
5.  Wählen Sie im Menü **Optionen > Gruppe Identnummernvergabe > Automatische Vergabe**.
    Damit ist die automatische Vergabe der ID für Kisten eingerichtet.

### Wareneingang von Kisten erfassen

Bei der Erfassung des Wareneingangs von Kisten, wird pro Kiste eine Kisten-ID vergeben. Anschließend werden die zugehörigen Etiketten gedruckt.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So erfassen Sie den Wareneingang einer Kiste mit einer automatischen ID" auf Seite D-2172
*   "So vergeben Sie Kisten-IDs manuell" auf Seite D-2175
*   "So drucken Sie Kistenetiketten" auf Seite D-2176

**So erfassen Sie den Wareneingang einer Kiste mit einer automatischen ID**

1.  Wählen Sie **Dokumente > Bestellung > Wareneingang > Wareneingang**.

*Abb. D-85: Wareneingang für Kisten – nach Nummernverwalter*
*   **A Suchoption**
*   **B Bestellnummer**

⇨ Softwarereferenz, "Wareneingang (Dialog)" auf Seite D-2264

Stellen Sie sicher, dass die automatische Vergabe für Kisten-IDs aktiviert ist.

2.  Wählen Sie die Option (A), mit der Sie die Suche nach offenen Bestellungen starten möchten, z. B. **nach Bestellnummer**.
3.  Geben Sie die Bestellnummer (B) ein.
4.  Wählen Sie im Menü **Start > Ausführen**, um die Daten einzulesen.
    Die Anzeige wechselt zum Register **Komplett**. Sie können die Daten nochmals prüfen.
5.  Wechseln Sie zum Register **Identnummern**.

*Abb. D-86: Wareneingang für Kisten – Eingang erfassen*
*   **A Ausgewählte Bestellung**
*   **B Eingabe der Kisten-ID des Lieferanten**
*   **C Lagerort**
*   **D Pro Kiste eine Zeile (Unterposition)**

Wenn die Stückzahl der bestellten Position größer als 1 ist, wird in der Übersicht **Kistenpositionen** für jede Kiste eine Zeile angezeigt.
Sie können mehrere Kisten auf einmal auswählen, um diese in einem Schritt zu buchen.

6.  Markieren Sie eine Zeile, in der noch keine virtuelle Positionsnummer angezeigt ist.
7.  Geben Sie im Feld **Lieferanten-Identnummer (B)** die Kisten-ID des Lieferanten ein oder scannen Sie die Kisten-ID und springen Sie mit `<Tab>` in das nächste Feld.
    Wenn mehr als eine Kiste ausgewählt ist und die Lieferanten-Identnummer eingegeben ist, berechnet das System die Kisten-Identnummern für alle markierte Einträge.
8.  Wählen Sie den Lagerort aus und prüfen und korrigieren ggf. den Inhalt und den Preis.

*Abb. D-87: Wareneingang für Kisten – Daten für markierte Zeile*
*   **A Kisten-ID des Lieferanten**
*   **B Wareneingang für diese Kiste buchen**

Die Eingaben werden in die markierte Zeile übernommen.

9.  Wählen Sie im Menü **Start > Ausführen**, um die Eingaben zu bestätigen und den Wareneingang zu buchen.

*Abb. D-88: Wareneingang für Kisten – neue virtuelle Positionsnummer erzeugt*
*   **A Virtuelle Positionsnummer (verbuchte Unterposition)**
*   **B (Automatische) Kisten-ID**

Die Kiste wird verbucht und mit der nächsten virtuellen Positionsunternummer an das Ende der Liste **Kistenpositionen** verschoben.

10. Wiederholen Sie die Schritte 7 bis 9, bis Sie den gesamten Wareneingang erfasst haben.
    Wenn Sie alle Kisten erfasst haben, können Sie den Druck der Kistenetiketten und des Protokolls starten.
    ⇨ "So drucken Sie Kistenetiketten" auf Seite D-2176

**So vergeben Sie Kisten-IDs manuell**

1.  Wählen Sie **Dokumente > Bestellung > Wareneingang > Wareneingang**.
2.  Deaktivieren Sie im Menü **Optionen > Gruppe Identnummernvergabe > Automatische Vergabe**.
3.  Bereiten Sie die Erfassung des Wareneingangs vor, wie in den Schritten 2 bis 7 der vorhergehenden Handlungssequenz gezeigt.

*Abb. D-89: Wareneingang für Kisten – Eingang erfassen*
*   **A Ausgewählte Bestellung**
*   **B Kisten-ID des Lieferanten**
*   **C Manuelle Kisten-ID**
*   **D Pro Kiste eine Zeile (Unterposition)**

Wenn die Stückzahl der bestellten Position größer als 1 ist, wird in der Übersicht **Kistenpositionen** für jede Kiste eine Zeile angezeigt.

4.  Geben Sie die Kisten-ID (C) ein, mit der die Kiste in Ihrem Lager verbucht werden soll.
    Sie können die ID des Lieferanten übernehmen, indem Sie den Cursor in das Feld stellen und Lieferanten-ID erneut scannen.
5.  Wählen Sie den Lagerort aus und prüfen und korrigieren ggf. den Inhalt und den Preis.
    Diese Eingaben gelten nur für die Kistenposition, die in der Übersicht markiert ist.
6.  Wählen Sie im Menü **Start > Ausführen**, um die Eingaben zu bestätigen.
    Die Kiste wird verbucht und mit der nächsten virtuellen Positionsunternummer an das Ende der Liste **Kistenpositionen** verschoben.
7.  Wiederholen Sie die Schritte 4 bis 6, bis Sie den gesamten Wareneingang erfasst haben.
    Wenn Sie alle Kisten erfasst haben, können Sie den Druck der Kistenetiketten starten, um die Etiketten mit den manuell vergebenen IDs zu drucken.

**So drucken Sie Kistenetiketten**

1.  Nachdem Sie die Kisten einer Lieferung erfasst haben, wählen Sie im Menü **Druck > Gruppe Drucker > Etiketten**.
    Wenn Sie den Eintrag **Etiketten und Protokoll** wählen, wird zusätzlich das Protokoll gedruckt, das Sie sich auch im Register **Protokoll (Identnummern)** anzeigen lassen können.

*Abb. D-90: Kistenetiketten drucken*
*   **A Anzahl**
*   **B Drucker**

2.  Wählen Sie den Drucker (B) und die Anzahl (A) der erforderlichen Kopien.
3.  Klicken Sie auf [OK], um den Druck zu starten.
    Der Dialog wird geschlossen und die Etiketten werden gedruckt. Im Protokoll werden alle verbuchten Kisten mit den Kisten-IDs aufgeführt.

> **Ergänzende Informationen**
> *   ⇨ Stammdaten, “Fälligkeitsberechnung für Februar (28 oder 29 Tage)" auf Seite B-1080
> *   ⇨ Softwarereferenz, "Einstellungen (ID)" auf Seite D-2277

### Preis- und Rechnungskontrolle

> **Lernziele**
> *   Auftragsbestätigung des Lieferanten erfassen.
> *   Preise prüfen.
> *   Gesammelte Auftragsbestätigung zu mehreren Bestellungen erfassen.

> **Nutzen**
> *   Zusammen mit der Auftragsbestätigung können die Preise geprüft werden.
> *   Preise mehrerer Bestellungen können in einer gemeinsamen Auftragsbestätigung geprüft werden.

> **Merke**
> **Status**: Nach der Preis- und nach der Rechnungskontrolle wird der Status der Dokumente hochgesetzt. In Verbindung mit einem Sperrstatus ist eine erneute Preis- und/oder Rechnungskontrolle daher nicht möglich.
> **Differenzen**: Sie können die Preis- oder Rechnungskontrolle nur dann abschließen, wenn keine Differenz zwischen dem eingegebenen Gesamtbetrag und der Summe der angezeigten Bestellungen besteht.
> **Schnellerfassung**: Wenn Sie im Menü **Optionen > Schnellerfassung** aktivieren, springt der Cursor nach der Eingabe der Bestellnummer direkt in das Feld **Rechnungssumme** bzw. **AB-Summe**. Sie können diese Option dann nutzen, wenn Sie in der Regel nur eine Bestellnummer eintragen.
> **Dokumentensperre**: Während der Preis- und Rechnungsprüfung sind die referenzierten Dokumente für den Zugriff durch andere Mitarbeiter gesperrt.
> **Voreinstellungen**:
> Firmendaten:
> *   Register Steuer
> *   Register Preisberechnung
> *   Register Druck
> *   Register Lager/EK/EDI

#### Eingangsrechnung

Die Preise können sowohl auf Basis der Auftragsbestätigung des Lieferanten als auch auf Basis der Lieferantenrechnung geprüft werden. Die Dialoge **Preiskontrolle** und **Rechnungskontrolle** sind identisch aufgebaut. In beiden Dialogen können Sie die Preise korrigieren und Ihre Einkaufspreise (EK) in den Dokumenten aktualisieren.

Während der Preis-/Rechnungskontrolle ist die zugehörige Bestellung für den Zugriff durch andere Benutzer gesperrt. Um die Bestellung während der Preis- bzw. Rechnungskontrolle anpassen zu können, kann das Dokument direkt geöffnet werden. So können Sie z. B. fehlende Zuschläge erfassen, ohne die Preis- und Rechnungskontrolle zu verlassen.

Die Prüfungen von Preisen und Rechnungen können auch in elektronisch ausgetauschten Dokumenten durchgeführt werden. Diese Funktionalität ist im Themenblock **Elektronischer Dokumentenaustausch** beschrieben:
⇨ "Export/Import (openTRANS)" auf Seite D-2185

**Preiskorrekturen**

Sie können die Preis- oder Rechnungskontrolle nur dann abschließen, wenn keine Differenz zwischen dem eingegebenen Gesamtbetrag und der Summe der angezeigten Bestellungen besteht. Eine solche Differenz kann z. B. durch unterschiedliche Preise, nicht erfasste Zuschläge oder durch Fehleingaben entstehen.

Wenn der eingegebene Betrag nicht mit der Bestellung oder der Summe der Bestellungen übereinstimmt, müssen Sie die Preise in den Positionen oder in den Stücklisten korrigieren – oder die AB/Rechnung zur Korrektur zurückschicken.

Nach der Rechnungskontrolle werden die Bestellungen mit dem entsprechenden Status versehen und sind damit zur Anweisung und zur Übergabe an die FiBu bereit.

Nach der Prüfung, Korrektur und Bestätigung der Preise wird der Status der Bestellung umgesetzt.
⇨ "Dokumentenstatus" auf Seite D-2074

**EK-Preise im Auftrag**

Der EK eines referenzierten Auftrags kann nur so lange aktualisiert werden, wie der Sperrstatus dies zulässt. Nach der Rechnungskontrolle wird der Status der Bestellung hochgesetzt. Die Preis- oder Rechnungskontrolle kann dann nicht nochmals durchgeführt werden.

#### Fußzuschläge und Fußrabatte

Die Fußzuschläge/-rabatte einer Bestellung, z. B. ein Energiezuschlag, werden in die Kosten des Auftrags zurückgeschrieben. Die Fußzuschläge/-rabatte werden positionsgenau zurückgerechnet und in der Dokumentenverwaltung angezeigt. Damit ist auch bei bestellten Produkten der Deckungsbeitrag immer aktuell, der in der Positionserfassung angezeigt wird.

Optional kann bei der Rechnungskontrolle automatisch die Position **Anlieferpauschale pro Bestellung** angefügt werden. Damit entfällt die manuelle Nacherfassung in der Bestellung.

#### Fremdwährung

Wenn Sie mit mehreren Währungen arbeiten, können Sie die Preise und Rechnungen in einer Fremdwährung bestätigen. Die Preise der Bestellpositionen werden in der Landeswährung gespeichert. Die Einkaufspreise werden unter Berücksichtigung der Währungsumrechnung aktualisiert.

#### Sammel-AB und Sammelrechnung

Wenn Ihr Lieferant mehrere Bestellungen gesammelt in einer AB oder Rechnung aufgeführt hat, kann diese nur geprüft und akzeptiert werden, wenn in allen Bestellungen derselbe MwSt-Satz und dieselbe Währung angegeben sind.

Wenn einer Ihrer Lieferanten in der Regel Sammelrechnungen erstellt, kann es sinnvoll sein, für diesen Lieferanten einen eigenen Nummernverwalter für die Bestellungen einzurichten.

#### EK-Rückschreibung

Der EK wird in die referenzierten Aufträge zurückgeschrieben, wenn er bei der Preis- oder Rechnungskontrolle und/oder beim Buchen des Wareneingangs geändert wurde. Diese angepassten Einkaufspreise werden zur Kalkulation des Deckungsbeitrags und bei der Lagerbewertung oder bei Lagerbestellungen herangezogen.

Dazu müssen in den Firmendaten die Option zur Ermittlung der Einkaufspreise aktiviert und die Preistabellen für den Einkauf gepflegt sein.

*Abb. D-91: Firmendaten – Register Lager/EK/EDI*

### Rechnung kontrollieren

Sie können die Preise sowohl in der Auftragsbestätigung als auch in der Rechnung des Lieferanten prüfen. Dazu stehen zwei Dialoge zur Verfügung, die im Aufbau und in den Funktionen identisch sind:
*   Preiskontrolle
*   Rechnungskontrolle

Die Preiskontrolle haben Sie bereits in der Einheit **AB erfassen und Preise prüfen** kennengelernt. Analog zur Preiskontrolle können Sie die Lieferantenrechnung prüfen und damit zur Anweisung freigeben.

> **Cursorposition bestimmen**
> Wenn Sie im Menü **Optionen > Schnellerfassung** aktivieren, springt der Cursor nach der Eingabe der Bestellnummer direkt in das Feld **Rechnungssumme** bzw. **AB-Summe**. Sie können diese Option dann nutzen, wenn Sie in der Regel nur eine Bestellnummer eintragen.

**So prüfen Sie eine eingegangene Lieferantenrechnung**

1.  Wählen Sie **Dokumente > Bestellungen > Rechnung > Rechnungskontrolle**.

*Abb. D-92: Rechnungskontrolle*
*   **A Rechnungsnummer**
*   **B Rechnungsdatum**
*   **C Betrag der Rechnung (netto/brutto)**
*   **D Bestellnummer(n)**
*   **E Kurs**

⇨ Softwarereferenz, "Rechnungskontrolle - Bestellungen" auf Seite D-2285

2.  Geben Sie die Rechnungsnummer (A), das Datum (B) und die Bestellnummer (D) ein und springen Sie mit `<Tab>` in das nächste Feld.
    In der Übersicht **Bestellungen** wird die Bestellung angezeigt.
    Wenn in der Rechnung mehrere Bestellungen zusammengefasst sind, können Sie nacheinander alle Bestellnummern angeben. Die Bestellungen werden dann jeweils in der Übersicht hinzugefügt. Sie können jedoch nur Bestellungen mit identischem Steuersatz zusammenfassen. Geben Sie einfach die nächste Bestellnummer ein und drücken Sie die `<Tab>`-Taste.
    Sie können eine Bestellung aus der Übersicht wieder entfernen, indem Sie den Eintrag markieren und auf `<Entf>` drücken.
3.  Geben Sie die Rechnungssumme (C) ein.

> **Währung**
> Wenn Sie nur mit einer Währung (EUR) arbeiten, muss im Feld **Kurs (E)** 1 eingetragen sein.

4.  Wählen Sie im Menü **Start > Ausführen**, um die Eingabe zu bestätigen.
    Der Betrag wird geprüft und das Register **Positionen** wird angezeigt.

*Abb. D-93: Rechnungskontrolle – Positionen*
*   **A Positionspreis**
*   **B Differenz über alle Positionen**

Sie können Preisdifferenzen ausgleichen, indem Sie einen Positionspreis überschreiben. Geänderte Beträge werden in die referenzierten Dokumente zurückgeschrieben.

5.  Wählen Sie im Menü **Start > Ausführen**, wenn keine Differenz (mehr) angezeigt wird.
    Die Daten werden gespeichert und der Status der Bestellung(en) wird umgesetzt. Die Rechnungskontrolle für diese Dokumente kann danach nicht nochmals durchgeführt werden.
    Die Berechnung der EK-Preise wird in den zugehörigen Bestellungen und Aufträgen korrigiert, sofern diese Option im Menü **Optionen > Gruppe Einstellungen** aktiviert ist.

> **Ergänzende Informationen**
> *   ⇨ Softwarereferenz, "Preiskontrolle" auf Seite D-2242
> *   ⇨ Softwarereferenz, "Rechnungskontrolle - Bestellungen" auf Seite D-2285

### Übungen

Die Übungen sind so konzipiert, dass Sie den gesamten Einkauf trainieren. Das bedeutet, dass Sie die Bestellungen aus dem vorigen Themenblock jetzt weiterbearbeiten.

**Wareneingang erfassen**
Erfassen Sie den Wareneingang zu einer referenzierten Bestellung vollständig und prüfen Sie die Statusumsetzung im Auftrag.

**Wareneingang teilweise erfassen**
Erfassen Sie eine Teillieferung zu einer referenzierten und zu einer manuellen Bestellung.
Erfassen Sie den Wareneingang einer Lagerbestellung und einer Position mit Produkten, die nicht als Lagerartikel geführt werden (ganz oder teilweise).

**Wareneingang von Kisten erfassen**
Erfassen Sie den Wareneingang von Kisten ganz oder teilweise.

**Vollständigkeit der Lieferungen prüfen**
Suchen Sie nach Bestellungen, zu denen Positionen oder Teilpositionen nicht geliefert wurden.
Holen Sie ggf. die Erfassung des Wareneingangs durch eine komplett-Buchung nach.

**Rechnung prüfen**
Erfassen Sie die Rechnung zu einem Wareneingang.

## Elektronischer Dokumentenaustausch

In diesem Themenblock lernen Sie, wie Sie A+W Business für elektronischen Dokumentenaustausch anpassen und Dokumente exportieren und importieren.

Dazu gehören folgende Lerneinheiten:
*   "Export/Import (openTRANS)" auf Seite D-2185
*   "Datenexport/-import (EDI)" auf Seite D-2211

Sie können Dokumente mit Ihren Lieferanten/Kunden elektronisch austauschen.

Für den Austausch von Bestellungen werden die Daten in eine ASC-Datei geschrieben. Für den Austausch von Rechnungen oder Auftragsbestätigungen müssen die Daten im openTRANS-Format (XML-Format) vorliegen.

*Abb. D-94: Daten Ex- und Import*
*   **EDI:** Ein Kundenauftrag (Bestellung) fließt vom Kunden (A+W Business) zu A+W Business.
*   **openTRANS:** Eine Auftragsbestätigung (AB) und Rechnung fließen vom Lieferanten (A+W Business) zu A+W Business.

Per EDI können Bestellungen ausgetauscht werden. Ein Kundenauftrag ist dabei aus Sicht des Kunden eine Bestellung, aus Sicht von A+W Business ein Auftrag.

Im Format openTRANS können Auftragsbestätigungen (ABs) und Rechnungen ausgetauscht werden. Dazu müssen alle Beteiligten mit A+W Business arbeiten. Diese Funktion ist in den folgenden Kapiteln ausführlich dargestellt.

### Export/Import (openTRANS)

> **Lernziele**
> *   Funktionsweise des elektronischen Dokumentenaustauschs kennenlernen.
> *   Voreinstellungen kennenlernen und anpassen.
> *   Pflichtfelder in Dokumenten kennenlernen.
> *   Elektronische Dokumente senden und einlesen.

> **Nutzen**
> *   Mit dem elektronischen Dokumentenaustausch können Sie Dokumente Ihrer Kunden und Lieferanten einlesen, ohne die Daten einzeln erfassen zu müssen.
> *   Mit dem Einlesen von Daten vermindern sich Fehler bei der Erfassung.

> **Merke**
> **Voraussetzung**: Beim Lieferanten/Kunden und Ihnen muss die gleiche Version von A+W Business installiert sein, mindestens A+W Business 5. Die notwendigen Dienste müssen installiert und gestartet sein.
> **Datenformat**: Elektronische Dokumente können in den Formaten openTRANS und XML ausgetauscht werden.
> **Datenimport**: Die Daten können als Datei per E-Mail gesendet oder auf einem gemeinsamen freigegebenen Laufwerk auf einem Server gespeichert werden.
> **Datenexport**: Bei jedem Drucklauf von Auftragsbestätigungen oder Rechnungen wird geprüft, ob Dokumente mit dem Kennzeichen für den Export vorhanden sind. Diese Dokumente werden dann automatisch an die hinterlegte E-Mail-Adresse gesendet.
> **Referenzen**: Dokumentenreferenzen werden aus folgenden Feldern gebildet:
>    *   Im Auftragskopf Feld **Bestelltext1**
>    *   In der Positionserfassung Feld **Kundenposition**.
>    Diese Felder müssen daher immer gefüllt sein. Wenn diese Referenzen in eingelesenen Dokumenten nicht hergestellt werden können, muss die Zuordnung beim Prüfen des elektronischen Dokuments manuell nachgeholt werden.
> **Teillieferungen**: Aus einer elektronischen AB können Teillieferungen erstellt werden.
> **Rundungsdifferenzen**: Bei der Preis- und Rechnungskontrolle können Rundungsdifferenzen im Cent-Bereich akzeptiert werden, wenn in der Produktverwaltung ein Ausgleichsprodukt angelegt ist, dem diese Differenzen zugeordnet werden können.
> **Sammelrechnungen**: Bei Sammelrechnungen des Lieferanten kann ein einmal aufgeführter Zuschlag auf alle Positionen der zugehörigen Bestellungen oder Bestellpositionen verteilt werden.
> **Dokumentensperre**: Während der Preis- und Rechnungsprüfung sind die referenzierten Dokumente für den Zugriff durch andere Mitarbeiter gesperrt.
> **Voreinstellungen**:
>   Stammdaten:
>    *   Produktdaten
>    *   Kunden-/Lieferantendaten
>    *   Statusdefinition
>    *   Statuszuordnung
>    *   Währungen
>   Firmendaten:
>    *   Register Parameter
>   Stammdaten:
>    *   B2B Kunde/Lieferant

#### Dokumentenaustausch

Auftragsbestätigungen und Rechnungen können im openTRANS-Format exportiert und importiert werden. Dieses Format wurde für A+W Business erweitert. Es können jedoch auch Dokumente im Standard-Format und XML-Dateien eingelesen werden.

Der Datenaustausch über das openTRANS-Format setzt voraus, dass beim Lieferanten/Kunden und Ihnen die gleichen Versionen von A+W Business installiert sind, mindestens A+W Business 5. Außerdem müssen in der Schnittstellenverwaltung die Parameter beim Lieferanten/Kunden genauso festgelegt werden wie in Ihrem A+W Business.

#### Dokumenten-Export

Der Export von Auftragsbestätigungen und Rechnungen wird pro Kunde/Lieferant im Modul **Stammdaten > B2B** konfiguriert. Dazu wird festgelegt, ob und welche Dokumente exportiert werden sollen und welcher Modus dazu verwendet wird.

*Abb. D-95: Einstellungen für den elektronischen Datenaustausch*
*   **A Export-Modus**
*   **B Export-Format**
*   **C Auswahl der Dokumente**
*   **D Einstellungen für E-Mail-Modus**

**Export-Modus (A):**
*   **Automatischer Versand per E-Mail:**
    Dazu muss im Netzwerk ein E-Mail-Server zur Verfügung stehen. Standardmäßig wird die E-Mail-Adresse aus den Stammdaten des Kunden/Lieferanten verwendet. Für Auftragsbestätigungen und für Rechnungen können aber auch abweichende E-Mail-Adressen hinterlegt werden.
*   **Ablage in einem bestimmten Verzeichnis (auf dem Server):**
    Diese Dateien können anschließend manuell übermittelt werden.

Bei jedem Drucklauf von Auftragsbestätigungen oder Rechnungen wird geprüft, ob Dokumente mit dem Kennzeichen für den Export vorhanden sind. Der eigentliche Export wird über einen Dienst zyklisch im Hintergrund durchgeführt. Zur Kontrolle werden die entsprechenden Dokumente im Dialog **Export** angezeigt. Durch den Export werden folgende Dateien erzeugt:
*   **RESPONSExxxx.awotres** für Auftragsbestätigungen.
*   **DISPATCHxxxx.awotdis** für ein Liefer-Avis.
*   **INVOICExxxx.awotinv** für Rechnungen.

Bei den Dateinamen wird zwischen Groß- und Kleinschreibung unterschieden.

#### Dokumentenreferenzen

Die Dokumentenreferenzen auf Positionsebene werden benötigt, um Auftragspositionen automatisch ihren jeweiligen Bestellpositionen zuzuordnen (Referenzierung). Bei der manuellen Erfassung eines Auftrags werden diese Dokumentenreferenzen automatisch aus den Feldern **Bestelltext1** im Auftragskopf und **Kundenposition** in der Positionserfassung gebildet.

*Abb. D-96: Referenzen für den Datenaustausch*
*   **A Kopfdaten – Dokument**
*   **B Positionen – Register Position**

Außerdem muss in den Firmendaten im Register **Parameter** die Option **Bestelltext1 und Kundenposition in Dokumentenreferenzen übernehmen** aktiviert sein.

*Abb. D-97: Firmendaten - Parameter*

#### Dokumenten-Import

Auftragsbestätigungen und Rechnungen im openTRANS-Format werden über das **A+W openTRANS ImportTool** importiert. Es wird standardmäßig auf dem A+W Business-Client installiert.

Zum Einlesen stehen damit unterschiedliche Möglichkeiten zur Verfügung:
*   Doppelklick auf die gespeicherte Datei.
*   Doppelklick auf die als E-Mail-Anhang gesendete Datei.

Durch den Doppelklick werden die Daten in die Datenbank importiert und können in den Import-Dialogen von A+W Business angezeigt werden.

Wenn die Dateien auf der Festplatte abgelegt sind, so kann über das Kontextmenü die Option **Anzeigen** gestartet und eine generische Ansicht des Dokuments angezeigt werden.

**XML-Dateien**

XML-Dateien können nicht direkt aus dem E-Mail-Client heraus eingelesen werden. Diese Dateien müssen zunächst gespeichert werden. Danach können sie über das Kontextmenü eingelesen oder als generische Ansicht angezeigt werden.

Nachdem ein Dokument erfolgreich eingelesen wurde, steht es im jeweiligen Dialog **Elektr. Preiskontrolle** oder **Elektr. Rechnungskontrolle** zur Verfügung.

#### Dokumentenkontrolle

Die Dialoge **Elektr. Preiskontrolle** und **Elektr. Rechnungskontrolle** sind identisch aufgebaut.

*Abb. D-98: Elektronische Rechnungskontrolle*
*   **A Eingelesenes Dokument**
*   **B Anzeige- und Filtereinstellungen**
*   **C Status**
*   **D Referenzierte Dokumente**

In beiden Dialogen werden alle Dokumente (D) einschließlich möglicher Teillieferungen angezeigt, die mit dem importierten Dokument (A) verknüpft sind. Zu jeder Bestellung wird optisch signalisiert (C), ob die Verknüpfungen zwischen Bestellung und importiertem Dokument vollständig sind. Nur vollständig referenzierte Dokumente können akzeptiert werden.

Wenn das importierte Dokument akzeptiert wurde, wird der Status der referenzierten Bestellungen entsprechend umgesetzt. Die Preis- oder Rechnungskontrolle kann dann nicht nochmals durchgeführt werden.

**Buchungsarten**

Bei der Kontrolle der importierten Dokumente werden je nach Status die Optionen **Akzeptieren**, **Teillieferung erstellen** und **Ablehnen** angeboten.

Die Buchungsart **Akzeptieren** ist nur dann freigeschaltet, wenn ein importiertes Dokument vollständig und fehlerfrei referenziert ist. Wenn nur die Bestellmengen nicht vollständig referenziert sind, das Dokument jedoch ansonsten vollständig ist, so kann über die Buchungsart automatisch eine Teillieferung erzeugt werden.

#### Positionszuordnung

Sind in einem openTRANS-Dokument die Bestellreferenzen fehlerhaft oder gar nicht vorhanden, kann das System Dokumenten- und Bestellpositionen nicht automatisch miteinander verknüpfen. Diese (nicht verknüpften) Positionen werden in der Positionsübersicht gekennzeichnet und müssen manuell verknüpft werden.

In der Rechnung kann z. B. die Referenz zu einer Position fehlen oder fehlerhaft aufgeführt sein. Anhand der Produktbezeichnungen können Sie diese Referenzen im Dialog **Positionen** manuell zuordnen herstellen.

#### Fußzuschläge/-rabatte

Fußzuschläge oder -rabatte werden im Normalfall nicht in der Bestellung erfasst. In der Auftragsbestätigung oder Rechnung sind sie jedoch aufgeführt. Um eine Rechnungskontrolle durchführen zu können, müssen diese Positionen in den Bestellungen nachträglich erfasst werden. Dazu kann die Bestellerfassung aus dem Dialog **Rechnungskontrolle** heraus geöffnet werden. Nachdem der Zuschlag in der Bestellung eingefügt ist, muss er in der Rechnung zugeordnet werden.

Wenn mehrere Bestellungen vom Lieferanten in einer Rechnung zusammengefasst sind, in der ein Fußzuschlag/-rabatt nur einmal aufgeführt ist, so kann diese Position auf alle verknüpften Bestellungen verteilt werden. Das Programm versucht, für die anteiligen Beträge anhand der Zuschlagsbasis sinnvolle Vorschlagswerte zu finden und bietet diese an. Diese Werte können überschrieben werden.

Außerdem können die Fußzuschläge/-rabatte anhand der Produktnummer für diesen Lieferanten automatisch zugeordnet werden. Dabei wird die Zuordnung der Produktnummer des Lieferanten zur eigenen Produktnummer gespeichert.

#### Sammelrechnungen in A+W Business

Wenn in A+W Business Sammelrechnungen erstellt werden, so werden für jeden Auftrag die Fußzuschläge/-rabatte als eigene Position aufgeführt. Da eine direkte manuelle Zuordnung oft schwer ist, können in diesem Fall mehrere Dokumentenpositionen zusammengefasst und den Bestellpositionen zugeordnet werden. In der Positionsübersicht ist anschließend nur noch die zusammengefasste Dokumentenposition aufgeführt.

#### Betragsdifferenzen

Üblicherweise können Sie eine Rechnung nur akzeptieren, wenn keine Differenzen auftreten. Wenn Sie bei einem Lieferanten mit Betragsdifferenzen rechnen (müssen), können Sie diese auf unterschiedliche Weise behandeln:
*   Sie können die Rechnung ablehnen und den Lieferanten über die Unstimmigkeiten (telefonisch) informieren.
*   Betragsdifferenzen können auch durch unterschiedliche Rundungen entstehen. Mit der Option **Betragsdifferenzen akzeptieren** können Sie die Rechnungskontrolle trotz solcher Differenzen durchführen. Die Differenz darf sich nur im Cent-Bereich bewegen. Sie sollten sich mit der Option **Hinweis auf Betragsdifferenz/Ausgleichsposition** darauf aufmerksam machen lassen.
*   Die Rundungsdifferenzen im Cent-Bereich können automatisch akzeptiert werden. Dazu muss ein sogenanntes Ausgleichsprodukt angelegt sein, auf das der Differenzbetrag gebucht werden kann.
*   Mit der Funktion **Prod.Nr. für Ausgleichspos.** können Sie ein Produkt auswählen, auf das Rundungsdifferenzen (im Cent-Bereich) verbucht werden sollen.

#### Dienste prüfen

Folgende Dienste müssen installiert und gestartet sein:
*   **A+W Business 6 Interface Service**: Dieser Dienst wird in aller Regel auf einem separaten Rechner installiert. Bei der Installation durch einen Service-Mitarbeiter der A+W Software GmbH muss die Funktion **Interface Service handles B2B documents** aktiviert werden.
*   **AWProtocol**: Diesen Dienst finden Sie unter **Systemsteuerung > Verwaltung > Dienste**.
*   **ERP-WebService**: Diesen Service finden Sie unter **Systemsteuerung > Computerverwaltung > Dienste und Anwendungen > Sites > Default Web Site**.

*Abb. D-99: ERP-Service prüfen*

Die Dienste werden in der Regel mit A+W Business zusammen installiert. Sie sind auf den Starttyp **Automatisch** eingestellt. Dadurch sollten sie beim Start des Rechners automatisch gestartet werden.

Wenn der Datenaustausch nicht funktioniert, sollten Sie die Dienste prüfen und ggf. manuell starten. Eine Anleitung dazu finden Sie in der Online-Hilfe des Betriebssystems.

Außerdem benötigen Sie das **A+W openTRANS ImportTool**, das vom A+W Business-Setup automatisch installiert wird.

#### Statusvergabe

Der Status der Dokumente wird auch beim Im- und Export umgesetzt. Dazu müssen folgende Statuspunkte zugeordnet sein.

| Statuspunkte für Import | Statuspunkte für Export |
| :--- | :--- |
| 61 - Auftragsbestätigung nicht akzeptieren | 830 - Rechnungsexport |
| 64 - Rechnung nicht akzeptieren | 840 - Auftragsbestätigungsexport |

Beim Import wird der Status manuell umgesetzt, beim Export automatisch.
Im Part **Stammdaten** sind die Statuspunkte und Statuszuordnungen ausführlich beschrieben. In dieser Einheit wird daher nur auf die Besonderheiten eingegangen, die Sie für den Austausch von elektronischen Dokumenten beachten müssen.

### Voreinstellungen für Datenaustausch prüfen

In den Firmendaten müssen die Einstellungen für den Austausch von Produktdaten korrekt eingestellt sein. Nur wenn die entsprechenden Produktdaten hinterlegt und zugeordnet sind, können die Dokumente korrekt eingelesen werden.

> **A+W Business neu starten**
> Nach Änderungen der Firmendaten sollten Sie A+W Business neu starten.

**So prüfen Sie die Firmendaten**

1.  Wählen Sie **Stammdaten > Firma > Firmendaten** und wechseln Sie zum Register **Parameter**.

*Abb. D-100: Firmendaten - Parameter*
*   **A Bestelltext übernehmen**

⇨ Stammdaten, "Firmendaten - Parameter" auf Seite B-1073

2.  Aktivieren Sie die Checkbox **Bestelltext1 und Kundenposition in Dokumentenreferenzen übernehmen**.
3.  Wählen Sie im Menü **Start > Speichern**, um Änderungen zu speichern.
    Die Daten werden gespeichert.

### Währungseinstellungen prüfen

Für die Währungen, die in den Aufträgen und Bestellungen verwendet werden, muss das internationale Währungskennzeichen hinterlegt sein. Die Einstellungen müssen Sie prüfen, wenn Sie mit mehreren Währungen arbeiten.

**So prüfen Sie die Währungseinstellungen**

1.  Wählen Sie **Stammdaten > Finanzen > Währung**.

*Abb. D-101: Internationales Währungskennzeichen*
*   **A Wechselkurs für Umrechnung von Preisen**
*   **B Internationales Währungskennzeichen**

⇨ Stammdaten, "Währung" auf Seite B-1045

Jeder Währung muss das internationale Kennzeichen (B) zugewiesen sein.

2.  Markieren Sie die Zeile der Währung, der Sie das Kennzeichen zuweisen wollen.
3.  Öffnen Sie in der Spalte **Internat. Kennzeichen** die Kombobox und wählen Sie aus der Liste das entsprechende Kennzeichen aus.
4.  Prüfen Sie die jeweils eingetragenen Wechselkurse (A) und aktualisieren Sie diese ggf.
5.  Wählen Sie im Menü **Start > Speichern**, um Änderungen zu speichern.
    Die Daten werden gespeichert.

### Statusdefinitionen prüfen

Damit die elektronischen Dokumente verarbeitet werden können, müssen die Statuspunkte 61, 64, 830, 840 definiert und zugeordnet sein. Diese Statuspunkte werden für folgende Aktionen benötigt:
*   Dokumente ex- und importieren.
*   Importiertes Dokument ablehnen oder akzeptieren.

Zu diesem Thema gibt es folgende Handlungsanleitungen:
*   "So prüfen Sie die Statuspunkte" auf Seite D-2197
*   "So prüfen Sie die Statusverwaltung" auf Seite D-2198
*   "So prüfen Sie die Statuszuordnung" auf Seite D-2199

**So prüfen Sie die Statuspunkte**

1.  Wählen Sie **Stammdaten > Auftrag > Statuspunkte**.

*Abb. D-102: Statuspunkte*

⇨ Stammdaten, "Statuspunkte" auf Seite B-1021

2.  Prüfen Sie, ob die Statuspunkte 61, 64, 830 und 840 vorhanden sind.
    Die Nummern der Statuspunkte sind in der Spalte **Kennz.** angegeben.
    In der Regel werden die Statuspunkte mit der Installation zusammen erstellt. Sie müssen immer manuell zugeordnet werden.
3.  Wenn diese Statuspunkte nicht vollständig vorhanden sind, legen Sie die fehlenden an.
4.  Wählen Sie im Menü **Start > Speichern**, um Änderungen zu speichern.
    Die Daten werden gespeichert. Diese Statuspunkte müssen einem entsprechenden Anwenderstatus zugeordnet sein.

**So prüfen Sie die Statusverwaltung**

1.  Wählen Sie **Stammdaten > Auftrag > Statusverwaltung**.

*Abb. D-103: Statusverwaltung*

⇨ Stammdaten, "Statusverwaltung" auf Seite B-1020

Wenn die Anwenderstatus 61/64 und 830/840 nicht vollständig vorhanden sind, legen Sie die fehlenden an.

2.  Wählen Sie im Menü **Start > Speichern**, um Änderungen zu speichern.
    Prüfen Sie als Nächstes, ob alle Zuordnungen vorhanden und vollständig sind.

**So prüfen Sie die Statuszuordnung**

1.  Wählen Sie **Stammdaten > Auftrag > Statuszuordnung**.

*Abb. D-104: Statuszuordnung*
*   **A Statuspunkt**
*   **B Dokumententyp**
*   **C Zugeordneter Anwenderstatus**

⇨ Stammdaten, "Statuszuordnung" auf Seite B-1022

2.  Prüfen Sie, ob die Statuspunkte 61, 64, 830 und 840 zugeordnet sind.
    Wenn Sie in der Tabelle **Statuszuordnung** einen Statuspunkt markieren, muss mindestens der Anwenderstatus (C) angezeigt werden.
    Wenn diese Statuspunkte nicht vollständig zugeordnet sind, holen Sie die Zuordnung nach.
3.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
4.  Wählen Sie in den Feldern **Statuspunkt**, **Dokumententyp** und **Anwenderstatus** die entsprechenden Einträge aus.
5.  Wählen Sie im Menü **Start > Speichern**, um Änderungen zu speichern.
    Die Daten werden gespeichert.

### Datenexport per openTRANS einstellen

Im Modul **Stammdaten > B2B** müssen Sie festlegen, wie die Daten ausgetauscht werden sollen.

**So legen Sie die Exportart für openTRANS fest**

1.  Wählen Sie **Stammdaten > B2B > Kunde > Dokumentenexport**.
    Der Dialog **openTRANS-Dokumentenexport** wird mit dem Register **Auswahl** angezeigt.
2.  Wählen Sie im Menü **Start > Suchen**, um in die Kunden einzulesen.
    Die Kunden werden im Register **Tabelle** aufgelistet.
3.  Markieren Sie den Kunden (C), mit dem Dokumente über das openTRANS-Format ausgetauscht werden sollen.
4.  Wechseln Sie zum Register **Auswahl**.
    *   Wenn die Angaben für den Kunden korrekt sind, können Sie den nächsten Kunden prüfen.
    *   Wenn keine Angaben vorhanden sind, müssen Sie diese einpflegen.

*Abb. D-105: openTRANS-Dokumentenexport*
*   **A Exportart per Datei oder per E-Mail**
*   **B Übertragungstyp**
*   **C Kundennummer**
*   **D Auswahl der Dokumentenart**
*   **E E-Mail-Adressen für unterschiedliche Dokumentenarten**
