---
title: "DE_AWBusiness_Lagerwirtschaft_6_2"
source: "DE_AWBusiness_Lagerwirtschaft_6_2.pdf"
tags: ["A+W Business", "Inventory Management", "Lagerwirtschaft", "ERP", "Purchase Price", "Einkaufspreis", "Bill of Materials", "Stückliste", "Inventory Posting", "Lagerbuchung", "Tutorial"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a detailed tutorial from the A+W Business software manual, focusing on inventory and warehouse management (Lagerwirtschaft). It covers pricing, inventory control at the bill of materials (BOM) level, and general warehouse operations."
long_description: "This comprehensive tutorial provides step-by-step instructions for managing inventory and pricing within the A+W Business Fertigung ERP system. The first section, 'Preise' (Prices), explains how to define and calculate purchase prices (Einkaufspreis), including the last purchase price and the average purchase price (Durchschnitts-EK). It details the necessary system settings, the price determination process via a flowchart, and provides examples. The second major section, 'Lagerführung auf Stücklistenebene' (Inventory Management at BOM Level), describes how to manage BOM components as stock items, including reservation and booking processes. The main chapter, 'Lagerwirtschaft' (Inventory Management), covers core warehouse operations. It explains how to create and manage stock items, handle manual and automatic inventory postings (receipts, issues, transfers), and utilize various queries to monitor stock levels, movements, and statistics. The tutorial is highly visual, with numerous screenshots illustrating the user interface and guiding users through specific tasks like creating stock items, performing manual bookings, and analyzing inventory data."
---

# Tutorial: Stammdaten

---
## Preise

### Lernziele
- Preisdefinitionen für Einkaufspreis prüfen.
- Arten der Preisermittlung für den Einkaufspreis (EK) kennenlernen.

### Nutzen
- Die Preisentwicklung von Lagerartikeln kann unter alternativen Möglichkeiten verfolgt werden: Entweder wird der letzte Einkaufspreis betrachtet oder ein durchschnittlicher Einkaufspreis.
- In der Lagerverwaltung kann der Durchschnitts-EK jeweils für alle Abmessungen des Lagerartikels ermittelt werden oder nur für das aktuelle Lagermaß.

### Merke

| Begriff | Erklärung |
| :--- | :--- |
| **Einkaufspreis** | Einkaufspreise werden in den Preisstammdaten auf dieselbe Art wie Verkaufspreise angelegt. |
| **Durchschnitts-EK** | Der Durchschnitts-EK wird als Einzelpreis ermittelt. Die Funktion zur Berechnung muss in den Firmendaten aktiviert werden. |
| **Durchschnitts-EK pro Lagermaß** | Die Ermittlung des Durchschnitts-EK kann pro Lagermaß ausgeschaltet werden. |
| **Voreinstellungen** | - **Produktverwaltung Lagermaße** <br> - Checkbox EK Suche Lager <br> - **Firmendaten** <br> - Register Lager / EK / EDI |

---

## Einkaufspreis und Durchschnitts-EK

Sie können den Lagerwert eines Lagerartikels auf verschiedene Arten ermitteln lassen, nämlich als Durchschnitts-EK oder den letzten EK. Diese Entscheidung haben Sie bereits in den Firmendaten > Register Lager / EK / EDI getroffen.
⇨ "Firmendaten prüfen" auf Seite G-31

Für die Preisermittlung sind u. a. zwei Kennzeichen wichtig, die in den Lagermaßen und den Lagerartikeln gesetzt werden.

*(Abbildung G-21: Preisermittlung EK)*
*Die Abbildung zeigt zwei Dialogfenster der Software. A zeigt den Dialog 'Lagermaße' mit der Checkbox 'EK Suche Lager'. B zeigt den Dialog 'Lagerverwaltung' mit der Checkbox 'Einbeziehen in Gesamt-EK'.*

- **Lagermaße:**
  Dieses Kennzeichen (A) steuert, ob für dieses Lagermaß die durchschnittlichen Kosten aus dem Lager ermittelt werden oder nicht.
- **Lagerverwaltung:**
  Dieses Kennzeichen (B) steuert, ob der jeweilige Lagerartikel an der Berechnung des gesamten Durchschnittspreises aller Ausprägungen dieses Artikels teilnimmt oder nicht. Die entsprechenden Preise pro Lagerartikel und Lagerort werden in den Bereichen Einkaufpreise und Berechnung des geschnittenen Preises dargestellt.

Die ausführliche Beschreibung der Preisdarstellung im Dialog Lagerverwaltung finden Sie in der Softwarereferenz.
⇨ Softwarereferenz, "Lagerverwaltung - Preise" auf Seite G-190

---

## Durchschnitts-EK

Der Einkaufspreis wird bei jedem Lagerzugang oder bei Preisänderungen in der Bestellung neu berechnet. Das System speichert diese Informationen für jeden Lagereingang, um preisliche Änderungen an Bestellungen, die nach dem Wareneingang durchgeführt werden, wieder in den Durchschnitts-EK (geschnittener Preis) einrechnen zu können.

Der Durchschnitts-EK wird nach folgender Formel berechnet:
`Durchschnitts-EK = ((Lagermenge * Preis) + (Zugangsmenge * Preis des Zuganges)) / (Menge + Zugangsmenge)`

> **Beispiel**
> Von einem Artikel sind 100 qm zu 10 €/qm im Lager. (Durchschnitts-EK = 10 €/qm). Durch eine Bestellung werden 10 qm zu 15 €/qm zugebucht. Der Durchschnittspreis wird neu berechnet:
> `((100 qm * 10 €) + (10 qm * 15 €)) / (100 qm + 10 qm) = 10,45 € pro qm`

Der EK wird so lange aktualisiert, bis für alle Bestellungen eine Rechnungskontrolle durchgeführt wurde oder die Bestellung ins Archiv übergeben wurde. Danach werden preisliche Änderungen in der Bestellung für die Berechnung des Durchschnittspreises nicht mehr berücksichtigt. In der Ansicht in der Lagerverwaltung werden die Bestellungen nicht mehr aufgelistet, sobald sie (nach der Archivierung) gelöscht wurden.

### EK-Ermittlung bei kombiniertem Lagermodus

Wenn Sie mit kombiniert geführten Lagerartikeln arbeiten, wird durch die Rückmeldung aus der Produktion die auf den 0 x 0-Satz reservierte Menge gelöscht und die entsprechenden Lagerplatten werden abgebucht.
Wenn Sie aber keine Produktionsrückmeldung haben, werden die Bestände der qm-Artikel sehr schnell negativ und verfälschen die Kosten.
Daher können Sie in den Firmendaten festlegen, dass kombiniert geführte Lagerartikel ohne Abmessung bei der Bildung des Durchschnitts-EKs ignoriert werden. Dann werden nur die durchschnittlichen Kosten der Lagermaße berechnet.

---

## Ablaufplan zur Preisermittlung

*(Abbildung G-22: Ablaufplan zur Preisermittlung)*

Der folgende Prozess beschreibt den Ablaufplan zur Preisermittlung:

1.  **Start der Preissuche.**
2.  **Frage:** Manuelle Vorgabe des Preisschlüssels?
    *   **Ja:** Suche des EK in der Tarifzuordnung des vorgegebenen Preisschlüssels. → **Ende.**
    *   **Nein:** Weiter zu Schritt 3.
3.  **Frage:** In Produkt-Lagermaßen vorhanden?
    *   **Nein:** Weiter zu Schritt 4.
    *   **Ja:**
        1.  **Frage:** Produktausprägung exakt in Lagerverwaltung vorhanden?
            *   **Ja:** Selektion des durchschnittlichen EK aus dem Lagerartikel. → **Ende.**
            *   **Nein:**
                1.  Bilden des gewichteten durchschnittlichen Preises über all die Lagerprodukte, in denen das entsprechende Kennzeichen aktiviert ist.
                2.  **Frage:** Ist der ermittelte Preis > 0?
                    *   **Ja:** → **Ende.**
                    *   **Nein:** Weiter zu Schritt 5.
4.  **Frage:** Suche nach Durchschnittspreis aktiv?
    *   **Ja:** Gehe zu Schritt 3, Unterpunkt "Ja".
    *   **Nein:** Weiter zu Schritt 5.
5.  **Frage:** Abweichender Preisschlüssel für EK hinterlegt?
    *   **Ja:** Suche des EK in der Tarifzuordnung des vorgegebenen Preisschlüssels. → **Ende.**
    *   **Nein:** Suche des EK in der Standard-Tarifzuordnung. → **Ende.**

---

## Erläuterung zum Ablaufplan – Preisberechnung

Die Preisberechnung sucht zunächst in den Produkt-Lagermaßen, ob der Artikel in genau der angegebenen Ausprägung vorhanden ist.
- **Wenn ja,** wird abhängig vom dortigen Kennzeichen der Durchschnittspreis des Lagerartikels ermittelt oder nicht. Ist das Kennzeichen nicht aktiv, wird der Preis im Standard-Tarif für den Einkauf gesucht. Ist ein abweichender EK-Schlüssel hinterlegt, hat dieser Vorrang vor dem Standard-Tarif.
- **Wenn der Artikel nicht in den Produkt-Lagermaßen vorhanden ist,** wird mit der Suche des Durchschnittspreises im Lager fortgefahren.

### Durchschnittspreis

Bei der Ermittlung des Durchschnittspreises werden folgende Stufen durchlaufen:
- Wenn der Durchschnittspreis aus dem Lager ermittelt wird, so wird zunächst der genaue Lagerartikel gesucht. Wenn der Artikel vorhanden ist, wird der dort hinterlegte Preis verwendet.
- Wenn der Artikel nicht vorhanden ist, wird das gewichtete Mittel über alle Produkte mit dieser Artikelnummer und mit einem aktiven Kennzeichen ermittelt.
- Wenn der ermittelte Preis 0 ist, so wird der Preis aus der Standard-Tarifzuordnung des EK gesucht.
- Wurde in der Auftragserfassung der Preisschlüssel manuell vorgegeben, so wird der Preis nur aus der Tarifzuordnung des gewählten Preisschlüssels ermittelt, ohne Durchschnittspreissuche.

Die Kennzeichen haben auf die Rückschreibung der Kosten in den jeweiligen Lagerartikel keinen Einfluss.

Nachfolgend sind einige Beispiele zum Ablauf der Preissuche dargestellt.

**Produkt-Lagermaße**
| Artikel | Abmessung | Durchschnittspreis ermitteln | abw. Preisschlüssel |
| :--- | :--- | :--- | :--- |
| 1004 | 3210 x 6000 | ja | Lagermaße |
| 1004 | 3210 x 3000 | nein | <k.A.> |
| 1004 | 3210 x 2000 | nein | Lagermaße |

**Lagerverwaltung**
| Artikel | Abmessung | Ermittlung Gesamt-Durchschnittspreis | Bestand | Durchschnittspreis |
| :--- | :--- | :--- | :--- | :--- |
| 1004 | 3210 x 6000 | ja | 100 Stk | 1,25 €/qm |
| 1004 | 2000 x 2000 | ja | 40 Stk | 1,84 €/qm |
| 1004 | 1500 x 3000 | nein | 45 Stk | 1,99 €/qm |

**Preise laut Tarifzuordnung in der Preisverwaltung**
| Preisschlüssel | Preis |
| :--- | :--- |
| Standard | 1,50 €/qm |
| Lagermaße | 1,00 €/qm |

**Auftrag mit den ermittelten Einkaufspreisen**
| Pos. | Artikel | Abmessung | Vorgabe des Preisschlüssels | EK |
| :--- | :--- | :--- | :--- | :--- |
| 1 | 1004 | 3210 x 6000 | nein | 1,25 €/qm |
| 2 | 1004 | 2000 x 2000 | nein | 1,44 €/qm |
| 3 | 1004 | 3210 x 3000 | nein | 1,50 €/qm |
| 4 | 1004 | 3210 x 2000 | nein | 1,00 €/qm |
| 5 | 1004 | 1250 x 1433 | nein | 1,30 €/qm |
| 6 | 1004 | 3210 x 6000 | ja (Lagermaße) | 1,00 €/qm |

---

## Einstellung für EK-Ermittlung prüfen

In den Firmendaten haben Sie bereits den Lagerführungsmodus eingestellt. Dazu aktivieren Sie jetzt zunächst die Ermittlung des Einkaufspreises und wählen dann die Art der Ermittlung.

*(Abbildung G-23: Firmendaten – Lager / EK / EDI)*
*Die Abbildung zeigt den Einstellungsdialog 'Firmendaten' auf dem Register 'Lager / EK / EDI'. Callouts zeigen auf:*
*- A: Die Checkbox 'Einkaufspreis ermitteln'.*
*- B: Die Radio-Buttons für die Art der Ermittlung ('Durchschnitts EK' oder 'Letzter EK').*
*- C: Die Checkbox 'Kombiniert geführte Lagerartikel ohne Abmessung ignorieren'.*

**So prüfen Sie die Einstellungen für den Einkaufspreis**
1.  Wählen Sie im Menü **Stammdaten > Firma > Firmendaten**.
    ⇨ Stammdaten, "Firmendaten" auf Seite B-918
2.  Wechseln Sie zum Register **Lager / EK / EDI**.
3.  Aktivieren Sie die Checkbox **Einkaufspreis ermitteln (A)**, um die Optionen freizuschalten:
    - **Durchschnitts EK:** Bei jeder Lagerzubuchung wird der Durchschnitts-EK neu berechnet.
    - **Letzter EK:** Jeweils der letzte EK, der im Lager bei einem Wareneingang oder bei der Rechnungskontrolle gebucht wurde, wird zur Lagerbewertung herangezogen.
    - **Kombiniert geführte Lagerartikel ohne Abmessung ignorieren:** Aktivieren Sie diese Checkbox, wenn die Bestände von kombiniert geführten Lagerartikeln ohne Abmessung bei der Bestimmung des durchschnittlichen EKs nicht berücksichtigt werden sollen.
4.  Wählen Sie im Menü **Start > Speichern**, um die Änderungen zu speichern.
    Die Daten werden gespeichert.

## Preise prüfen

In dieser Einheit lernen Sie, wie Sie die Preise für den Einkauf festlegen.
Damit der Durchschnitts-EK ermittelt werden kann, müssen folgende Bedingungen erfüllt sein:
- Das Produkt muss als Lagerartikel angelegt sein.
- Das Kennzeichen für den EK muss in den Firmendaten gesetzt sein.

In der Regel legen Sie nur einen Preisschlüssel für den EK an, Sie können jedoch auch mehrere EK-Preisschlüssel nutzen. Alle Preisschlüssel für den EK müssen anschließend als Tarifkombination definiert werden. Bei mehreren Preisschlüsseln für den EK sollte eine Standard-Preisliste definiert sein. Sie können auch einen Preis anlegen. Dieser wird bei der Berechnung des Durchschnittspreises nicht überschrieben. Der Durchschnitts-EK wird in der Lagerverwaltung in gesonderten Feldern angezeigt.

**So prüfen Sie die Stammdaten Ihrer Preislisten**
1.  Wählen Sie im Menü **Stammdaten > Preise** und prüfen Sie die Einstellungen in den Dialogen **Jahrgang**, **Schlüssel** und **Tarif**. Sie brauchen nur die Einträge zu prüfen, die für Preise (und sonstige Eigenkalkulationen) für Lagermaße und Kisten verwendet werden.
2.  Wählen Sie im Menü **Stammdaten > Preise > Preise**.
    *(Abbildung G-24: EK-Preistabellen)*
    ⇨ Stammdaten, "Preise" auf Seite B-714
3.  Prüfen Sie, ob alle EK- und VK-Preise definiert und auf dem aktuellen Stand sind, und ergänzen oder korrigieren Sie diese ggf.
4.  Wechseln Sie zu dem Register, in dem der Preis definiert ist, und prüfen Sie, ob der EK-Preis korrekt eingetragen ist, oder korrigieren Sie diesen ggf.
    *(Abbildung G-25: Definierte Einkaufspreise)*
5.  Wählen Sie im Menü **Start > Speichern**, um die Änderungen zu speichern.
    Die Daten werden gespeichert.

## Übungen
- Prüfen Sie, ob den Lagermaßen die korrekten Preislisten zugeordnet sind.
- Legen Sie eine neue Preisliste mit einem EK-Einzelpreis für einen Lagerartikel an.

## Ergänzende Informationen
⇨ Softwarereferenz, "Reservierte Lagerartikel" auf Seite G-215
⇨ Softwarereferenz, "Einkaufspreise" auf Seite G-190
⇨ Stammdaten, "Status zuordnen" auf Seite B-427
⇨ Stammdaten, "Einzelpreise anlegen" auf Seite B-236
⇨ Stammdaten, "Preise" auf Seite B-714
⇨ Stammdaten, "Tarife" auf Seite B-664
⇨ Stammdaten, "Einkaufspreis ermitteln" auf Seite B-957
⇨ Stammdaten, "Lagerführungsmodus" auf Seite B-960

---

# Tutorial: Stammdaten

## Lagerführung auf Stücklistenebene

### Lernziele
- Zusammenhang der Beschaffungsart auf den Ebenen des Hauptprodukts und der Stücklisten-Komponenten kennenlernen.
- Einstellungen in den Firmendaten prüfen.

### Nutzen
- Stücklisten-Komponenten, die für die Produktion benötigt werden, können als Lagerartikel geführt werden.

### Merke

| Ebene | Erklärung |
| :--- | :--- |
| **Hauptartikel** | Wenn der Hauptartikel bereits als Lagerartikel definiert ist, sind automatisch alle Stücklisten-Komponenten auch als Lagerartikel definiert. |
| **Stückliste** | Jede Stücklisten-Komponente kann auch dann als Lagerartikel definiert werden, wenn das Hauptprodukt die Beschaffungsart *Produktion* hat. |
| **Voreinstellungen** | **Stammdaten:**<br>- Produktverwaltung<br>- Lieferantenkartei<br>**Firmendaten:**<br>- Register Parameter<br>- Register Lager / EK / EDI |

---

## Reservierung und Buchung für Stücklisten-Komponenten

Lagerartikel können sowohl Hauptprodukte als auch Stücklisten-Komponenten sein. So können Sie beispielsweise bei einer Fertigtür, die Sie inkl. Beschlägen verkaufen, das Glas als Eigenfertigung anlegen und die Beschläge als Lagerartikel führen.
Wenn der Hauptartikel bereits als Lagerartikel definiert ist, sind automatisch alle Stücklisten-Komponenten auch als Lagerartikel definiert.

*(Abbildung G-26: Einstellung der Beschaffungsart bei Hauptprodukt mit Stückliste)*
*Die Abbildung zeigt zwei Screenshots der Artikelverwaltung.*
*- A: Zeigt die Beschaffungsart des Hauptprodukts (z.B. Produktion).*
*- B: Zeigt die Beschaffungsart einer Stücklisten-Komponente (z.B. Lagerentnahme).*

Wenn Sie einen solchen Stücklistenartikel im Auftrag erfassen, wird jede Komponente, die als Lagerartikel definiert wurde, in der Lagersuche angezeigt. Wenn Sie dieses Hauptprodukt im Dialog Lagerinfo prüfen, werden alle Stücklisten-Komponenten mit angezeigt.

*(Abbildung G-27: Auftragserfassung und Lagerinfo)*
*Die Abbildung zeigt den Auftragserfassungsdialog. A zeigt die Auftragsposition mit dem Hauptprodukt und seinen Komponenten. B zeigt das "Lagerinfo"-Fenster, das den Lagerbestand der einzelnen Stücklisten-Komponenten anzeigt.*

Nachdem Sie den Auftrag gespeichert haben, werden alle Stücklisten-Komponenten reserviert.

*(Abbildung G-28: Reservierte Stücklisten-Komponenten)*
*Die Abbildung zeigt das Buchungsjournal, in dem die Stücklisten-Komponenten mit dem Buchungstyp "reserviert" aufgelistet sind.*

Wenn eine übergeordnete Komponente mit 2 Stück in der Stückliste geführt wird, so wird die im Lager zu verbuchende Menge der untergeordneten Komponenten (Kinder) mit 2 multipliziert.

### Einstellung prüfen

In den Firmendaten muss die Option Lagerführung auf Stücklistenebene aktiviert sein.

*(Abbildung G-29: Firmendaten – Lager / EK / EDI: Einstellungen zur Lagerführung von Stücklisten)*
*Die Abbildung zeigt die Checkbox "Lagerführung auf Stücklistenebene" im Firmendaten-Dialog, die aktiviert sein muss.*

---

## Produkte prüfen

In dieser Einheit lernen Sie, wie Sie die Beschaffungsart für die Stücklisten-Komponenten in der Produktverwaltung prüfen.

**So richten Sie Ihre Stücklisten für die Lagerführung ein**
1.  Wählen Sie im Menü **Stammdaten > Produkte > Artikel > Artikel**.
    Der Dialog Produktverwaltung wird geöffnet.
    ⇨ Stammdaten, "Produktverwaltung - Stückliste" auf Seite B-616
2.  Suchen Sie das Produkt, das Sie im Lager mit Stücklisten führen wollen.
3.  Wechseln Sie zum Register **Stückliste**.
    *(Abbildung G-30: Produktverwaltung – Stücklisten-Komponenten)*
4.  Markieren Sie die jeweilige Stücklisten-Komponente und wählen Sie die Beschaffungsart aus, wenn diese von der Definition in den Stammdaten der Komponente abweichen soll.
    - Wenn die Beschaffungsart für das Hauptprodukt auf **Lagerentnahme** gesetzt ist, gilt dies für alle Stücklisten-Komponenten.
    - Wenn die Beschaffungsart für das Hauptprodukt auf **Produktion** gesetzt ist, können die Stücklisten-Komponenten gleichzeitig als Lagerartikel geführt werden. Wenn Sie einen solches Hauptprodukt im Auftrag erfassen, werden in der Lagerinfo alle Stücklisten-Komponenten auf *reserviert* gesetzt.
5.  Wählen Sie im Menü **Start > Speichern**, um die Änderungen zu speichern.
    Die Daten werden gespeichert.
6.  Wiederholen Sie die Schritte für alle in Frage kommenden Produkte.

---

# Lagerwirtschaft

In diesem Themenblock lernen Sie, wie Sie die Lagerartikel erfassen und verwalten.

Dazu gehören folgende Lerneinheiten:
- "Lagerverwaltung" auf Seite G-68
- "Lagerbuchung" auf Seite G-78
- "Abfragen" auf Seite G-88
- "Lagerinformationen" auf Seite G-97
- "Lagerbestellung (automatisch)" auf Seite G-107

## Lagerverwaltung

### Lernziele
- Dialog Lagerverwaltung kennenlernen.
- Lagerartikel anlegen.

### Nutzen
- Mit Lagerartikeln können Sie den Lagerbestand erfassen und pflegen.
- Die Bestände von Lagerartikeln werden mit der Buchung von Warenab- und Warenzugänge aktualisiert.
- Über die Lagerartikel erhalten Sie die aktuelle Berechnung des Bestands inklusive der Reservierungen und der Bestellungen.

### Merke

| Thema | Erklärung |
| :--- | :--- |
| **Bestand berechnen** | Nur wenn Sie die Lagerartikel anlegen, kann die Berechnung von Stückzahlen und Flächen korrekt durchgeführt werden. |
| **Lagerartikel** | Im Lager können nur Bestände von Lagerartikeln verwaltetet werden. Die Produkte aus den Stammdaten werden nicht automatisch als Lagerbestand geführt. |
| **Wareneingang, -ausgang** | Der Wareneingang und Warenausgang kann nur für Lagerartikel gebucht werden. |
| **Voreinstellungen** | **Stammdaten:** <br>- Lagerorte <br>- Produkte <br>- Lagermaße |

---

### Elemente im Dialog Lagerverwaltung

Jeder Lagerartikel kann in verschiedenen Ausprägungen angelegt werden, z. B. Float 5 mm in mehreren Abmessungen.

*(Abbildung G-31: Definition des Lagerartikels)*
*Die Abbildung zeigt den Dialog "Lagerverwaltung" mit verschiedenen Feldern, die durch Buchstaben gekennzeichnet sind:*
- **A** Produktnummer
- **B** Maße des Lagerartikels
- **C** Standard-Lagerort
- **D** Lagerkategorie
- **E** Kennzeichen Lager-Hauptartikel
- **F** Bestandsprüfung für Lagervorschau
- **G** Definierte Lagerartikel
- **H** Hauptartikel
- **I** Blattzahl bei Kisten
- **J** Lagerort (4 Ebenen)

Wenn die Bestände nicht pro Lagerort (F) geprüft werden, muss ein Hauptartikel (E, H) zugeordnet werden, um die verfügbaren Quadratmeter des Glases zu ermitteln.
Bestandsmengen können pro Lagerort (J) gepflegt werden. Die definierten Lagerorte werden dazu den Lagerartikeln zugeordnet. Wenn ein Lagerartikel an verschiedenen Lagerorten vorgehalten wird, muss ein Standard-Lagerort (C) festgelegt werden.
Zu- und Abgänge werden automatisch am Standard-Lagerort verbucht, können aber manuell geändert werden.

### Lagerartikel
Die Produkte aus den Stammdaten werden nicht automatisch im Lager geführt. Damit ist gesichert, dass in der Bestandsführung nur die Artikel verwaltet werden, für die Lagerbestände vorgehalten werden. Andere Artikel, die nur kurzzeitig im Lager für die Produktion eines Auftrags gelagert sind, brauchen nicht als Lagerbestand gepflegt zu werden.
Zu jedem (Glas-)Produkt gehören auch ein Lagermaß und ein Lagerartikel. Die Zusammenhänge haben Sie bereits in der Lerneinheit Produkt kennengelernt.

### Lager-Hauptartikel
Sie können in der Lagerverwaltung mehrere Lagermaße miteinander verknüpfen, indem Sie einen Lager-Hauptartikel angeben. Die Bestandsprüfung (für die Lagervorschau im Dialog Lagerinfo) wird dann nur für den Lager-Hauptartikel durchgeführt und nur für diesen müssen Sie einen Mindestbestand hinterlegen.

> **Beispiel**
> Der Artikel 1004 ist mit folgenden Abmessungen angelegt:
> 0 x 0, 500 x 600, 1200 x 1800, 3210 x 4000 und 3210 x 5000.
> Für die Maße 3210 x 4000 und 3210 x 5000 ist als Lager-Hauptartikel jeweils der Artikel 0 x 0 angegeben. Für diesen ist der Mindestbestand mit 19.000,00 qm festgelegt.
> Die Bestände der Maße 3210 x 4000 und 3210 x 5000 werden gemeinsam gegen den Mindestbestand 19.000,00 qm geprüft.
> Für die Maße 500 x 600 und 1200 x 1800 sind jeweils eigene Mindestbestände festgelegt, die zur Prüfung herangezogen werden.

Wenn Sie die Lagerartikel bereits mit jeweils einem Mindestbestand angelegt haben, können Sie diese später dennoch einem Hauptartikel zuordnen. Bei der Ermittlung des Mindestbestands wird nur die Einstellung am Hauptartikel geprüft, die Mindestbestände an den Lagerartikeln werden ignoriert.

### Mindestmengen
Wenn der Lagerbestand eines Artikels eine bestimmte Mindestmenge (unter Berücksichtigung der Aufträge und Bestellungen) unterschreitet, muss rechtzeitig nachbestellt werden, um die Produktion nicht zu behindern. In A+W Business können Sie einen Schwellenwert für den Mindestbestand und einen Wert für den kritischen Lagerbestand angeben. Dieser wird für jeden Artikel gesondert festgelegt.

Der Mindestbestand ist also eine Kenngröße, die nicht unterschritten werden sollte, und zwar weder real noch im Rahmen von Reservierungen.
Mit Hilfe des definierten Mindestbestands erzeugt das Lager automatisch Bestellvorschläge. Diese müssen manuell freigegeben werden. Die automatischen Bestellvorschläge verwenden als Grundlage zur Berechnung der zu bestellenden Mengen folgende Kennzahlen:
- Bestellte Menge
- Reservierung
- Mindestbestand
- Standardbestellmenge
- Aktueller Bestand

Um den Artikel exakt zu bestimmen, werden u. a. Breite und Höhe ausgewertet.
Die Berechnung der Bestellmenge lernen Sie in einer gesonderten Einheit kennen.
⇨ "Bestellmenge nach Bestandsprüfung" auf Seite G-135

### Preise
Die Preise eines Lagerartikels werden als durchschnittliche Bezugspreise (EK-Preise) dargestellt, sofern diese Funktion in den Firmendaten aktiviert ist.
Die Anzeige der Durchschnittspreise wird bei der Archivierung und bei der Rechnungskontrolle für den jeweiligen Lagerartikel aktualisiert.
A+W Business geht davon aus, dass nach diesen Vorgängen die Preise nicht mehr geändert werden. Wenn Sie die Preise dennoch nach einem der Vorgänge ändern, fließen diese Änderungen nicht in die Berechnung des Durchschnittspreises ein.

*(Abbildung G-32: Durchschnittspreise für Lagerartikel)*
*Die Abbildung zeigt den "Preise"-Tab in der Lagerverwaltung.*
- **A** Anzeigemodus (z. B. für Scheiben mit unterschiedlichen Lagermaßen)
- **B** Durchschnittspreise im Einkauf
- **C** Checkbox: Einbeziehung in den Gesamt-EK
- **D** Durchschnittspreis pro Artikel oder über alle Abmessungen, wenn C aktiviert ist
- **E** Lagerwerte des markierten Artikels

Sie können festlegen, ob ein Artikel in die Berechnung des Durchschnittspreises über alle Abmessungen einbezogen werden soll. Nur wenn Sie die Checkbox **Einbeziehen in Gesamt-EK (C)** markiert haben, werden die Preise für den aktuellen Artikel in die Berechnung einbezogen.

Mit der Wahl des Modus (A) bestimmen Sie die Ansicht der Preisdarstellung:
- **Nur dieser Artikel:** Bei der Berechnung wird nur der angezeigte Artikel in der gewählten Abmessung berücksichtigt. Die EK-Historie des aktuellen Artikels wird angezeigt.
- **Alle Abmessungen:** Bei der Berechnung werden alle Abmessungen des angezeigten Glases berücksichtigt. Die EK-Historie aller Abmessungen des Artikels wird angezeigt.

Der Durchschnitts-EK wird für jeden Datensatz errechnet, außer für Warenabgänge. Warenabgänge reduzieren lediglich den Bestand. Die angezeigte Liste der Neuberechnungen (B) wird durch die Archivierung und durch die Rechnungskontrolle reduziert. Damit bleibt die Anzeige übersichtlicher.
Der erste Datensatz zeigt den Anfangsbestand und den ursprünglichen Preis. Darunter werden Zu- und Abgänge (negatives Vorzeichen) aufgeführt. Beim Zugang durch eine Lagerbestellung sind außerdem die Bestellnummer und die Bestellposition angezeigt.
Der Durchschnitts-EK wird bei der Erfassung oder Änderungen von Bestellungen aktualisiert. Er wird unter Berücksichtigung der gesamten Menge ermittelt.

> **Beispiel:**
> 100 Stück auf Lager à 15,00 € = 1500,00 €
> 40 Stück neue Einbuchung à 18,00 € = + 720,00 €
> **= 2220,00 €**
>
> 2220,00 / 140 Stück = 15,86 €

In die Berechnung fließen auch automatische Zuschläge ein, die in Bestellungen aufgeführt sind, z. B. Energie- oder Transportzuschlag.

### Verteilung von Zuschlägen
Kosten, die durch eine Lagerbestellung im Lager entstanden sind, werden im EK anteilig auf alle Artikel der Bestellung aufgeschlagen. Solche Kosten können beispielsweise Frachtkosten, Energiezuschlag oder beliebige sonstige Kosten sein, die für die Beschaffung der Lagerware eine Rolle spielen.
Diese Rückverteilung ist abhängig von der Preiseinheit des Zuschlages. Ist die Preiseinheit kg, so wird der Zuschlag auf Grundlage der Positionsgewichte rückverteilt. Bei allen anderen Preiseinheiten wird nach dem Preis der Positionen gewichtet.
Da jede Änderung an einer der Positionen Einfluss auf die Rückverteilung aller anderer Positionen hat, erfolgt diese Rückverteilung für das komplette Dokument immer nach einer Positionsänderung, also nach Abschluss der Eingabe in der Positionserfassung.
Änderungen an solchen Positionen aktualisieren den EK nur so lange, bis die Rechnungskontrolle durchgeführt wurde.
Die Fußzuschläge haben Sie in der Schulung zum Einkauf kennengelernt.
➡ Einkauf, "Fußzuschläge/-rabatte" auf Seite D-157

---

### Lagerartikel anlegen
In dieser Einheit lernen Sie, wie Sie die benötigten Lagerartikel anlegen. Dabei müssen Sie mindestens folgende Einstellungen festlegen, um das Lager verwalten zu können:
- Artikelnummer und Bezeichnung
- Maße bei Lagermaßen
- Lagerort und Standard-Lagerort (Default-Lagerort)
- Bestände

> **Inbetriebnahme des Lagers**
> Wenn noch gar keine Lagerartikel angelegt sind, können Sie sich diese Aufgabe durch die sogenannte Erstinventur erleichtern. Diesen Ablauf lernen Sie in einer gesonderten Einheit kennen.

**So legen Sie einen Lagerartikel an**
1.  Wählen Sie im Menü **Lagerwirtschaft > Lagerverwaltung**.
    Der Dialog Lagerverwaltung wird geöffnet.
    ⇨ Softwarereferenz, "Lagerverwaltung - Lagerartikel" auf Seite G-186
2.  Wählen Sie im Menü **Start > Neu**, um in den Erfassungs-Modus zu wechseln.
    Wenn Sie den Dialog Lagerverwaltung aus den Stammdaten heraus geöffnet haben, entfällt dieser Schritt. Die Felder für Artikel und Maße sind dann bereits gefüllt.
    *(Abbildung G-33: Felder für neuen Lagerartikel freigeschaltet)*
3.  Geben Sie die Nummer (A) und ggf. die Maße (B) ein.
4.  Wählen Sie einen Lagerort aus (C).
    Wenn Sie keinen Lagerort auswählen, wird der Lagerort `<k.A.>` eingetragen. In der Lagerwirtschaft wird dieser wie die definierten Lagerorte behandelt, z. B. bei der Inventur und bei Abfragen.
    Wenn Sie einen Lagerartikel an mehreren Lagerorten verwalten, müssen Sie einen dieser Lagerorte als Standard festlegen.
5.  Markieren Sie dazu die Checkbox **Default-Lagerort**.
6.  Wählen Sie im Feld **Hauptartikel (D)** den Artikel aus, für den Sie einen Mindestbestand für die Bestandsprüfung hinterlegen wollen.
    Wenn Sie für den neuen Lagerartikel einen eigenen Mindestbestand angeben wollen, müssen Sie die Maße des neuen Artikels auswählen. Die neuen Maße werden jedoch erst angezeigt, nachdem Sie den neuen Artikel gespeichert haben. Wählen Sie also zunächst irgendein Maß aus und ändern Sie dieses, nachdem Sie den Artikel gespeichert haben.
7.  Aktivieren Sie die Checkbox **Bestandsprüfung pro Lagerort (F)**, wenn für den Lagerartikel alle Lagerorte bei der Bestandsprüfung getrennt bewertet werden sollen.
8.  Geben Sie ggf. im Bereich **Bestände (E)** die Werte für die Mengen ein.
    Beachten Sie, dass der Mindestbestand entsprechend groß angegeben werden muss, wenn Sie für mehrere Maße denselben Hauptartikel angegeben haben.
    Die Checkboxen sind nur im Auswahlmodus freigeschaltet. Sie dienen dazu, die Suche nach Lagerartikeln zu filtern.
    Damit sind die Mindestangaben für den Lagerartikel hinterlegt.
9.  Wählen Sie im Menü **Start > Speichern**, um die Daten zu speichern.
    Die Daten werden gespeichert. Gleichzeitig wird ein Dummy-Lagerartikel ohne Maße für den kombinierten Lagerführungsmodus angelegt.
    Damit sind alle notwendigen Informationen hinterlegt, die A+W Business braucht, um Reservierungen und Buchungen durchzuführen. Der neue Lagerartikel kann nun bebucht werden.

### Übungen
- Legen Sie folgend Lagerartikel an und weisen Sie die korrekte Preisliste zu:
  - Lagerartikel, der in Stück auf Lager geführt wird.
  - Lagerartikel Handgriff, der in seiner eigenen Mengeneinheit auf Lager geführt wird.

### Ergänzende Informationen
⇨ Softwarereferenz, "Verwaltung" auf Seite G-176
⇨ Einkauf, "Dokument Bestellung" auf Seite D-45

---

## Lagerbuchung

### Lernziele
- Buchungsarten für Lagerartikel kennenlernen.
- Automatische Lagerbuchungen kennenlernen.
- Lagerbuchungen manuell auslösen.

### Nutzen
- Bei Bestellungen von Lagerartikeln wird der Wareneingang automatisch im Lager verbucht, bei Auftragspositionen der Warenausgang.
- Sie können den Lagerbestand an einzelnen Lagerorten korrigieren, indem Sie Lagerartikel umbuchen.

### Merke

| Thema | Erklärung |
| :--- | :--- |
| **Automatische Buchung** | - Automatische Zugangsbuchungen werden ausgelöst, wenn beim Wareneingang der Status in der Bestellung umgesetzt wird. <br>- Automatische Abgangsbuchungen werden ausgelöst, wenn in einem Auftrag der Status durch den Druck umgesetzt wird. |
| **Buchungsarten** | Die Buchungsarten für Lagerbuchungen sind fest im System hinterlegt. |
| **Manuelle Buchungen** | Manuell können z. B. folgende Buchungen ausgelöst werden: <br>- Zu- und Abgang von Waren <br>- Lagerort ändern |
| **Voreinstellungen** | **Stammdaten:**<br>- Statuszuordnungen<br>**Firmendaten:**<br>- Register Lager / EK / EDI |

---

### Lagerbewegungen
Die Lagerwirtschaft übernimmt Führung, Pflege und Kontrolle von Lagerbeständen. Zusätzlich steht der Dialog Lagerverwaltung für den manuellen Eingang, den manuellen Ausgang und zur Umbuchung von Lagerorten zur Verfügung.

*(Abbildung G-34: Lagerverwaltung für manuelle Lagerbuchungen)*

Alle Lagerbewegungen werden in einem Protokoll festgehalten, so dass Sie alle Vorgänge zurückverfolgen können.
Lagerbewegungen werden durch Aufträge, Bestellungen und Wareneingänge automatisch gebucht.

**Scannen**
In Verbindung mit AWPort können Lagerbuchungen auch über Barcodes erfasst werden. Dazu gehören nicht nur die Wareneingänge und Warenausgänge, sondern auch Umbuchungen.
Weitere Informationen zum Barcode und den Formaten entnehmen Sie bitte der Dokumentation zu AWPort.

### Buchungsarten
Die Buchungsarten für Lagerbuchungen sind fest im System hinterlegt und können nicht bearbeitet werden. Bei jeder Buchung eines Lagerartikels wird eine entsprechende Buchungsart zugewiesen. Anhand der Buchungsart können Auswertungen erstellt werden, die den Überblick über den Lagerbestand oder die Art der Lagerbewegungen verfeinern, z. B. über bestellte und reservierte Mengen.

Folgende Buchungsarten stehen zur Verfügung:
- **Reserviert:** Ein Artikel ist durch einen Auftrag so lange reserviert, bis der Lieferschein oder die Rechnung gedruckt wurde.
- **Ausgeliefert:** Ein Artikel wird als ausgeliefert gekennzeichnet, wenn der Lieferschein oder die Rechnung gedruckt wurde.
- **Verschnittenes LM:** Diese Buchungsart wird von Rückmeldung des A+W Optimizers verwendet, wenn eine Position aus einem Lagermaß zugeschnitten wurde. Die Anzahl der Lagerplatten wird ausgewertet.
- **Bestellt:** Das Kennzeichen wird durch eine Lagerbestellung gesetzt.
- **Empfangen:** Ein Artikel gilt dann als geliefert und empfangen, wenn er im Wareneingang verbucht wurde.
- **Lagereingang manuell, Lagerausgang manuell:** Die manuell gebuchten Lagerzu- oder Lagerabgänge sind durch eigene Buchungsarten gekennzeichnet.
- **Lagerumbuchung:** Lagerumbuchungen werden manuell ausgelöst.
- **Neuanlage:** Die Daten für neue Lagerartikel können im Rahmen einer Inventur oder manuell angelegt worden sein. Berücksichtigt werden alle neuen Artikel ab der letzten Archivierung.
- **Korrektur:** Im Rahmen einer Inventur können die Bestände von Lagerartikeln berichtigt werden. Berücksichtigt werden alle Korrekturen ab der letzten Archivierung.
- **Aus Lager gelöscht:** Interne Buchungsart.

### Ab- und Zubuchung
Lagerartikel werden je nach dem definierten Status abgebucht, wenn der Lieferschein oder die Rechnung für einen Auftrag gedruckt wird. Bis zu diesem Zeitpunkt sind die Lagerartikel lediglich reserviert.
Ob eine Reservierung den Bestand aktualisiert oder nicht, hängt vom Lagerführungsmodus ab, den Sie in den Firmendaten gewählt haben.
➡ "Lagerführungsmodus und Reservierung" auf Seite G-30

Durch den Wareneingang im Einkauf werden Lagerartikel aus Lagerbestellungen automatisch hinzugebucht.
Beim Wareneingang aus Lagerbestellungen können auch Waren erfasst werden, die nicht als Lagerartikel angelegt sind. Diese werden jedoch nicht mit Bestandsmengen gepflegt. Für diese Produkte werden keine Lagerbuchungen durchgeführt.

---

### Ab- oder Zugang manuell erfassen
In dieser Einheit lernen Sie, wie Sie einen Abgang oder Zugang von Lagerartikeln manuell buchen.

> **Lagerbuchungen für Kisten**
> Kisten werden in der Regel über Identnummern (ID) verbucht. Eine ausführliche Beschreibung finden Sie im Part Kistenmanagement.

**So buchen Sie einen Warenzugang manuell**
1.  Wählen Sie im Menü **Lagerwirtschaft > Lagerbewegung**.
    Der Dialog **Lagerbewegung** wird angezeigt.
    ⇨ Softwarereferenz, "Lagerbewegung - Abgang, Zugang" auf Seite G-196
2.  Wechseln Sie ggf. zum Register **Zugang**.
    *(Abbildung G-35: Lagerartikel suchen)*
3.  Geben Sie im Feld **Produkt** die Produktnummer ein und wählen Sie im Menü **Start > Suchen**.
    Im Bereich **Lagerorte** werden alle Lagerartikel aufgeführt, die dem Suchkriterium entsprechen.
4.  Markieren Sie den gewünschten Lagerartikel (A).
    Im Bereich **Bestandsveränderung** werden die Felder mit den aktuellen Werten gefüllt.
5.  Tragen Sie die Zugangsmenge (B) und/oder den neuen Bewertungspreis ein.
6.  Ändern Sie ggf. das Buchungsdatum.
7.  Wählen Sie im Menü **Start > Speichern**, um die Änderungen zu speichern.
    Die Daten werden gespeichert und der Bestand wird aktualisiert.
    Wenn Sie die Option **Protokoll beim Beenden** aktiviert haben, wird der Dialog **Lagerhistorie** geöffnet, wenn Sie den Dialog Lagerbewegung schließen.
    *(Abbildung G-37 & G-38: Lagerhistorie und Protokoll der Zugangsbuchung)*

**So buchen Sie einen Warenabgang manuell**
1.  Wählen Sie im Menü **Lagerwirtschaft > Lagerbewegung > Register Abgang**.
2.  Geben Sie im Feld **Produkt** die Produktnummer ein und wählen Sie im Menü **Start > Suchen**.
    Im Bereich **Lagerorte** werden alle Lagerartikel aufgeführt, die dem Suchkriterium entsprechen.
3.  Markieren Sie den gewünschten Lagerartikel.
    Im Bereich **Bestandsveränderungen** werden die Felder mit den aktuellen Werten gefüllt.
    *(Abbildung G-39: Manueller Lagerabgang)*
4.  Tragen Sie die Menge ein, die aus dem Bestand ausgebucht werden soll.
5.  Ändern Sie ggf. das Buchungsdatum.
6.  Wählen Sie im Menü **Start > Speichern**, um die Änderungen zu speichern.
    Die Daten werden gespeichert und der Bestand wird aktualisiert.

---

### Lagerort ändern
In dieser Einheit lernen Sie, wie Sie einen Lagerartikel von einem Lagerort zu einem anderen verschieben, z. B. aus der Lagerhalle in den Produktionsbereich. Diese Bewegung wird durch eine Umbuchung erfasst. Dadurch werden die Lagerartikel beim alten Lagerort als Abgang und beim neuen als Zugang verbucht.

> **Lagerort für einen Teil des Bestands ändern**
> Mit dem Umbuchen eines Lagerorts im Register **Umbuchen** wird immer der gesamte Bestand eines Lagerortes an einen anderen Lagerort umgebucht. Wenn Sie nur einen Teil der gelagerten Menge umbuchen wollen, müssen Sie diesen Teil am alten Lagerort ausbuchen und anschließend am neuen Lagerort zubuchen.

**So buchen Sie einen Lagerort um**
1.  Wählen Sie im Menü **Lagerwirtschaft > Lagerbewegung**.
    ⇨ Softwarereferenz, "Lagerbewegung" auf Seite G-195
2.  Wechseln Sie zum Register **Umbuchung**.
3.  Geben Sie im Feld **Produkt** die Produktnummer oder die ID ein.
4.  Wählen Sie im Menü **Start > Suchen**, um in die Suche zu starten.
5.  Markieren Sie den gewünschten Lagerartikel.
    *(Abbildung G-40: Lagerbewegung – Umbuchung)*
6.  Wählen Sie im Bereich **Lagerort (B)** den neuen Lagerort aus.
7.  Wählen Sie im Menü **Start > Speichern**, um die Änderungen zu speichern.
    Die Daten werden gespeichert. Der Lagerartikel wird am alten Lagerort aus- und am neuen zugebucht.

### Übungen
- Buchen Sie einen Lagerort um. Beachten Sie dabei, dass alle Lagerartikel umgebucht werden.
- Verbuchen Sie einen Lagerzugang manuell. Wenn Sie keine offene Lagerbestellung haben, holen Sie diese Übung in der Einheit Lagerbestellung nach.

### Ergänzende Informationen
⇨ "Lagerdefinition" auf Seite G-21
⇨ Softwarereferenz, "Buchungsart" auf Seite G-203
⇨ Einkauf, "Kistengeschäft" auf Seite D-136
➡ Einkauf, "Wareneingang von Kisten erfassen" auf Seite D-138

---

## Abfragen

### Lernziele
- Lagerbestand prüfen.
- Lagerbewegungen verfolgen.
- Lagerentwicklung prüfen.

### Nutzen
- Sie können sich mit den Abfragen (außerhalb der Inventur) einen schnellen Überblick über die Bestände verschaffen.
- Sie können Ladenhüter und Renner identifizieren und die Lagerverwaltung entsprechend anpassen.

### Merke

| Abfrage | Erklärung |
| :--- | :--- |
| **Buchungsjournal** | Im Buchungsjournal werden alle automatisch durchgeführten Buchungen angezeigt, die sich aus Dokumenten ergeben. |
| **Lagerhistorie** | In der Lagerhistorie werden alle Lager-Buchungsarten ausgewertet. |
| **Lagerstatistik** | Über die Lagerstatistik können Sie verschiedene Kennzahlen nach definierten Zeiträumen betrachten. |
| **Voreinstellungen** | Keine |

### Lagerabfrage
Mit verschiedenen Abfragen können Sie sich einen Überblick über die Buchungen, den Gesamtwert des Lagerbestands, statistische Auswertungen und eine Übersicht über Reservierungen anzeigen lassen.
Damit kann auch nachverfolgt werden, welche Daten von wem geändert wurden.

- **Buchungsjournal:** Das Buchungsjournal enthält Auswertungen zu den Lagerbuchungen, die aus Aufträgen und Bestellungen rühren. Sie können sich z. B. die Lagerbuchungen pro Produkt anzeigen lassen.
- **Lagerhistorie:** Über die Historie können Sie sich einen Überblick über das Tagesgeschehen im Lager pro Produkt verschaffen.
- **Lagerstatistik:** Die Lagerstatistik gibt Ihnen Aufschluss darüber, welche Ihrer Lagerartikel Renner und welche Ladenhüter sind. Damit haben Sie ein Kriterium, ob Artikel in das Lager auf- bzw. herausgenommen werden sollten. Die Entwicklung einzelner Lagerartikel kann über einen gewählten Zeitraum betrachtet werden. Die Auswertungen zeigen Anfangs- bzw. Endbestände und Zu- bzw. Abgänge Ihrer Lagerartikel pro Monat.
- **Lagerbewertung:** Der aktuelle Lagerwert des gesamten Lagers kann jederzeit und außerhalb der Inventur abgefragt werden. Daneben werden in der Lagerverwaltung zu jedem einzelnen Lagerartikel der höchste, niedrigste und Durchschnitts-EK und der zugehörige Lagerwert angezeigt.
- **Reservierte Lagerartikel:** Lagerartikel, die durch Aufträge reserviert sind, können pro Nummernverwalter aufgelistet werden. In der Ausgabe werden die reservierten Lagerartikel pro Artikelnummer und Lagerort dargestellt.

---

### Buchungsjournal anzeigen
In dieser Einheit lernen Sie, wie Sie welche Kriterien im Buchungsjournal und/oder in der Lagerhistorie einsetzen können. Diese beiden Dialoge sind analog aufgebaut, geben aber unterschiedliche Sachverhalte wieder:
- Im **Buchungsjournal** werden alle automatisch durchgeführten Buchungen angezeigt. Aufträge können nur so lange herangezogen werden, wie sie nicht archiviert und gelöscht sind.
- In der **Lagerhistorie** werden alle manuellen und automatischen Buchungen, Neuanlagen, Umbuchungen und Korrekturen aus der Inventur angezeigt.

**So lassen Sie sich Reservierungen anzeigen**
1.  Wählen Sie im Menü **Lagerwirtschaft > Abfragen > Buchungsjournal**.
    *(Abbildung G-41: Buchungsjournal)*
    ⇨ Softwarereferenz, "Buchungsjournal" auf Seite G-202
2.  Wählen Sie im Feld **Buchungsart (A)** den Eintrag `reserviert` aus. Wenn Sie das Feld frei lassen, werden alle Buchungen angezeigt.
3.  Grenzen Sie die Anzeige ggf. weiter ein, z. B. auf einen Artikel (C, D) und einen Zeitraum (B).
4.  Wählen Sie im Menü **Start > Ausführen**, um das Buchungsjournal zu erzeugen.
    *(Abbildung G-42: Buchungsjournal – Ergebnis)*
    Die Reservierungen werden in der Übersicht aufgelistet.

---

### Reservierte Lagerartikel drucken
Im Dialog **Reservierte Lagerartikel** erhalten Sie eine schnelle Übersicht über die Reservierungen aus Aufträgen in einem Nummernverwalter.

**So drucken Sie sich die Liste der reservierten Lagerartikel**
1.  Wählen Sie im Menü **Lagerwirtschaft > Abfragen > Reservierte Lagerartikel**.
    ⇨ Softwarereferenz, "Reservierte Lagerartikel" auf Seite G-215
2.  Wählen Sie den Nummernverwalter aus, in dem die aktuellen Aufträge gesammelt sind.
    *(Abbildung G-43: Reservierte Lagerartikel)*
3.  Wählen Sie im Menü **Druck > Bildschirm**, um sich die Liste auf den Bildschirm anzeigen zu lassen.
4.  Wählen Sie aus, wo der Druck umgebrochen werden soll.
5.  Klicken Sie auf **[OK]**, um die Einstellungen zu übernehmen.
    Der Dialog **Druck - Lagerprotokoll** wird geöffnet.
    *(Abbildung G-44: Reservierte Lagerartikel - Ausgabe auf dem Bildschirm)*
    Die reservierten Lagerartikel werden pro Artikelnummer und Lagerort aufgelistet. Bei mehreren Lagerorten wird die Gesamtsumme angezeigt.

---

### Lagerstatistik anzeigen
In dieser Einheit lernen Sie, wie Sie sich in der Lagerstatistik verschiedene Lagerkennzahlen eines Produkts anzeigen lassen können.

**So lassen Sie sich die Statistik zu Lagerbeständen anzeigen**
1.  Wählen Sie im Menü **Lagerwirtschaft > Abfragen > Lagerstatistik**.
    ⇨ Softwarereferenz, "Lagerstatistik – Produkte" auf Seite G-210
    Sie können die Anzeige auf ein Produkt und/oder einen Zeitraum einschränken.
    *(Abbildung G-45: Lagerstatistik – Produktauswahl)*
2.  Wählen Sie im Menü **Start > Ausführen**, um die Auswertung zu erstellen.
3.  Markieren Sie einen Eintrag und wechseln Sie zum Register **Statistik**, um die Details auszuwerten.
    *(Abbildung G-46: Lagerstatistik – Statistik)*
    Die Werte zum ausgewählten Produkt werden aufgelistet, z. B. die Bestände und Zu- und Abgänge pro Monat, die Umschlagshäufigkeit und Lagerdauer. In der Summenzeile werden die summierten Werte des angezeigten Zeitraums angezeigt.

### Übungen
- Prüfen Sie im Buchungsjournal die Reservierungen für das Float 4 mm.
- Drucken Sie die Reservierungen eines Float 5 mm für den nächsten Monat aus.

### Ergänzende Informationen
⇨ Softwarereferenz, "Buchungsjournal" auf Seite G-202
⇨ Softwarereferenz, "Lagerhistorie" auf Seite G-204
⇨ Softwarereferenz, "Lagerstatistik" auf Seite G-209
⇨ Softwarereferenz, "Reservierte Lagerartikel" auf Seite G-215

---

## Lagerinformationen

### Lernziele
- Dialog Lagersuche kennenlernen.
- Änderungen im Bestand und bei den Reservierungen erkennen.

### Nutzen
- Mit dem Überblick über die zukünftigen Lagerbestände und Reservierungen erhalten Sie ein weiteres Mittel zur Pflege der Bestände.
- Sie können erkennen, wann weitere Bestellungen erfasst werden müssen, damit die Produktion nicht unterbrochen wird.

### Merke

| Thema | Erklärung |
| :--- | :--- |
| **Lagerbestand** | Der Lagerbestand wird beim Wareneingang von Lagerartikeln und nach der Abbuchung aktualisiert. Die Abbuchung wird angestoßen, wenn der Lieferschein oder die Rechnung zu einem Auftrag gedruckt wird. |
| **Voreinstellungen** | **Stammdaten** <br> - Lieferantenkartei: Lieferzeit Tage (Wiederbeschaffungszeit) <br> - Statuszuordnung <br> **Firmendaten** <br> - Register Lager / EK / EDI > Lagervorschau <br> **Lagerverwaltung** <br> - Register Lager-Artikel > Hauptartikel |

### Lagersuche
Im Dialog Lagersuche können Sie sich alle Lagerartikel pro Lagerort und Abmessung anzeigen lassen. Diesen Dialog können Sie auch bei der Positionserfassung öffnen. Die Lagersuche ist dann bereits auf einen Lagerartikel eingeschränkt.

*(Abbildung G-47: Lagerinfo - Lagersuche)*
*Der Screenshot zeigt den Dialog "Lagersuche" mit Filtern und einer Liste von Lagerartikeln. Die Markierungen zeigen:*
- **A** Filter zum Einstellen der Suche
- **B** Wird als Lagerartikel geführt und entsprechend gebucht
- **C** Wird als Lagermaß geführt, ist aber kein Lagerartikel auf Lager
- **D** Bestellartikel, die nicht auf Lager geführt werden
- **E** Lagerartikel mit Mengenführung

**Bestand**
Die Berechnung des Bestands ist abhängig von dem Modus, in dem Sie das Lager führen.
⇨ "Wie soll das Lager geführt werden" auf Seite G-17
Bei der Berechnung von qm-Artikeln wird neben der Reservierung auch der Verschnitt berücksichtigt. Wenn Sie einem oder mehreren Artikeln einen Hauptartikel zugeordnet haben, wird der Bestand nicht mehr für die einzelnen Artikel angezeigt.
Bei der Erfassung eines Auftrags wird die Stückzahl oder die Anzahl der Quadratmeter (qm-Zahl) der Lagerartikel automatisch für den Kundenauftrag reserviert. Die Lagerabbuchung erfolgt dann automatisch bei Lieferschein- oder Rechnungsdruck.

### Lagerinfo und zukünftiger Lagerbestand
Eine detaillierte Ansicht im Dialog **Lagerinfo** gibt Auskunft über Liefertermin, Menge, Reservierungen usw. Dabei werden die verfügbaren Lagermaße einer Größe pro Lagerort angezeigt.

*(Abbildung G-48 & G-49: Lagerinfo - Zukünftiger Lagerbestand)*
*Die Screenshots zeigen den Tab "Zukünftiger Lagerbestand" im Lagersuche-Dialog.*
Der zukünftige Lagerbestand wird in drei Listen dargestellt:
1.  **Erste Liste (A):** Der ausgewählte Lagerartikel. Wenn dies ein Lagerhauptprodukt ist, werden in der dritten Liste die verknüpften Lagerartikel aufgeführt.
2.  **Zweite Liste (B):** Die Vorschau auf die nächsten Tage. Der Bestand wird für jeden Tag berechnet (Bestand zum Datum (H) - Reservierung (G) + Offene Bestellungen (F) = Errechneter Endbestand (E)).
3.  **Dritte Liste (C):** Die Lagermaße, die mit dem Hauptlagerartikel verknüpft sind.

Mit farblichen Markierungen werden Probleme für die erfassten Aufträge angezeigt:
- **Rot:** Termine können nicht eingehalten werden.
- **Gelb:** Die Wiederbeschaffungszeit reicht aus.

Offene Bestellmengen (F) zu einem Lagerartikel werden angezeigt, bis der Wareneingang verbucht wurde. Danach wird der aktuelle Bestand der gelieferten Menge aktualisiert.

**Wiederbeschaffungszeit**
Die Wiederbeschaffungszeit ergibt sich aus der Lieferzeit, die in der Lieferantenkartei für den Artikel hinterlegt ist, und aus den Tourentagen des Lieferanten, die in der Tourenverwaltung hinterlegt sind.
Wenn Sie eine Auftragsposition erfassen, können Sie den zukünftigen Lagerbestand abfragen. Wenn der Mindestbestand (D) zu einem bestimmten Termin unterschritten wird, können zwei Fälle eintreten.
