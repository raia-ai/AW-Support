---
title: "DE_AWBusiness_Verkauf_4_4"
source: "DE_AWBusiness_Verkauf_4_4.pdf"
tags: ["A+W Business", "ERP", "Sales Management", "Order Processing", "Tutorial", "Technical Manual", "German", "Bestellung", "Angebot", "FiBu"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A comprehensive tutorial for the A+W Business Verkauf software, covering order management, purchasing, and data transfer. This guide details processes from modifying ordered items and submitting orders to managing supplier data and handling financial accounting integration."
long_description: "This document is a detailed technical tutorial for the A+W Business Verkauf (Sales) module, part of the A+W Business ERP system. It provides step-by-step instructions for various sales and purchasing-related tasks. The guide begins with instructions on how to modify an existing ordered position, explaining that after an order is transferred, relevant data fields are locked but can be manually unlocked for correction. It then covers the process of transferring an order to the purchasing department, using the 'Bestellpool' (order pool) to manage and review orders before they are finalized. The manual explains how to change delivery dates, select different suppliers, and compare supplier prices directly within the order pool. It also addresses how to change procurement types and suppliers for orders within a number manager. A significant portion is dedicated to the 'Bestellungen' (Orders) section, which differentiates between referenced orders (created from a customer order) and independent stock orders. It details how to view and manage these orders, including their document headers and item details. The tutorial also covers the creation and management of 'Angebote' (quotes), including how to create alternative positions and entire alternative quotes to offer customers different options. It explains the quote follow-up process using a 'Wiedervorlage' (reminder) system and how to analyze quote success rates through the 'Angebotsstatistik' (quote statistics) feature. Finally, the document details the 'Datenübergabe' (data transfer) process, including transferring invoice data to financial accounting (FiBu) systems, transferring data for statistical analysis, and archiving old documents to maintain system performance. It also touches on additional functions like importing customer orders via EDI and document monitoring."
---

# Tutorial: Bestellung

---
## Änderung einer bestellten Position

Wenn nach der Bestellübergabe eine Bestellung existiert, werden alle aufbaurelevanten Datenfelder in der Positionserfassung des Auftrages gesperrt. Die Position kann manuell freigeschaltet und korrigiert werden.

Wenn die Werte einer Bestellposition bearbeitet wurden, muss die Bestellung erneut übergeben werden. Damit die Bestellung nicht doppelt geliefert wird, muss der Lieferant über die Änderung informiert werden. Vergessen Sie dabei nicht, dem Lieferanten deutlich zu machen, welche Bestellung neu ist und welche frühere Bestellung durch sie ersetzt wird.

**Abb. C-172 Gesperrte Position**

**Produktaufbau:**
| Produkt | Beschreibung |
| :--- | :--- |
| Dreifach ISO | Float 4 mm+Float 4 mm+Float 4 mm |
| 350000/Dreifach ISO | |
| 1004/Float 4 mm | |
| 12012/12 mm ALU Profil | |
| 8270/Abstandhaltersprosse 20 mm | |
| 8270/Abstandhaltersprosse 20 mm | |
| 1004/Float 4 mm | |
| 12012/12 mm ALU Profil | |
| 1004/Float 4 mm | |

**Preisdetails:**
| Art.Nr. | Bezeichnung | Preis/PE | PE | Rabatt | Netto | Netto | EK | Anteil. Zuschl | DB | DB% | Stückkosten |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| 1004 | Float 4 mm | 0,0000 | Stk | 0,00 | 0,0000 | 51,72 | | | | | |
| 12012 | 12 mm ALU Profil | 0,0000 | Stk | 0,00 | 0,0000 | 480,75 | | | | | |
| 8270 | Abstandhalters... | 0,0000 | Stk | 0,00 | 0,0000 | 29,61 | | | | | |
| 8270 | Abstandhalters... | 0,0000 | Stk | 0,00 | 0,0000 | 139,86 | | | | | |
| 1004 | Float 4 mm | 0,0000 | Stk | 0,00 | 0,0000 | 1.090,908 | | | | | |
| 12012 | 12 mm ALU Profil | 0,0000 | Stk | 0,00 | 0,0000 | | | | | | |
| 1004 | Float 4 mm | 0,0000 | Stk | 0,00 | 0,0000 | | | | | | |

## Auftrag zur Bestellung übergeben

Wenn Sie Aufträge mit Bestellpositionen erfasst haben, müssen Sie diese an den Einkauf übergeben. In dieser Einheit lernen Sie, wie Sie Bestellungen im Bestellpool bearbeiten und an den Einkauf übergeben.

### So übergeben Sie einen Auftrag an die Bestellung

1. Wählen Sie `Dokumente > Auftrag > Bestellübergabe`.

**Abb. C-173 Aufträge aus dem Nummernverwalter übergeben**

*   **A**: Option `Pool füllen`
*   **B**: `Ziel-NV`
*   **C**: `Nummernverwalter`

2. Wählen Sie den Modus `Pool füllen` (A) und den `Nummernverwalter` (C). Damit können Sie im Bestellpool prüfen, ob die Liefertermine eingehalten werden.
3. Wählen Sie den Ziel-Nummernverwalter (B) aus, in den die übergebenen Bestellungen gestellt werden. Sie können einen neuen Namen eingeben und so einen neuen Nummernverwalter anlegen. Wenn Sie dazu einen anderen Mitarbeiter auswählen, wird der Nummernverwalter diesem zugeordnet.
4. Wählen Sie ggf. im Bereich Ziel-Nummernkreis den Mandanten und den AV-Bereich aus.
5. Wählen Sie im Menü `Start > Ausführen`, um die Aktion zu starten. Der Bestellpool wird gefüllt. Das Register Bestellpool wird angezeigt.

**Abb. C-174 Aufträge im Bestellpool**

*   **A**: Aufträge mit Bestellposition
*   **B**: Auftragsposition
*   **C**: Standard-Lieferant
*   **D**: Lieferung nicht rechtzeitig
*   **E**: Position enthält eine Stückliste

6. Markieren Sie die Positionen, die Sie zur Bestellung an den Einkauf übergeben möchten. Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf. Nur die Positionen sind markiert, die mit einem X gekennzeichnet sind.

**Abb. C-175 Auftragspositionen zur Übergabe markieren**

*   **A**: Schaltflächen zur Markierung aller oder keiner Position
*   **B**: Kennzeichen zur Übergabe
*   **C**: Position ist nicht markiert

7. Wählen Sie im Menü `Start > Ausführen`, um die Aktion zu starten.
   Die aktivierten Prüfungen werden durchgeführt. Dies kann je nach Anzahl der Aufträge einige Momente dauern. Bestätigen Sie die jeweiligen Hinweise mit [Ja] oder [Nein], um die Prüfungen fortzusetzen. Wenn alle Prüfungen abgeschlossen sind, werden die zugehörigen Bestellungen angelegt und damit an den Einkauf übergeben.
   Der Auftragsstatus wird hochgesetzt. In der Auftragshistorie wird die Nummer der Bestellung als Referenz angegeben.

**Abb. C-176 Bestellnummern nach der Übergabe**

*   **A**: Position nicht übergeben
*   **B**: Nummer des Auftrags und der erzeugten Bestellung

Die erzeugten Bestellungen können Sie unter `Dokumente > Bestellung öffnen` und weiter bearbeiten.
⇨ "Bestellungen" auf Seite C-313

## Bestellung im Bestellpool ändern

Wenn zu einem Produkt mehrere Lieferanten hinterlegt sind, können Sie im Bestellpool die Preise und Liefertermine vergleichen und einen anderen Lieferanten auswählen.

Außerdem müssen Sie einer Position einen Lieferanten zuweisen, wenn in den Stammdaten zu dem entsprechenden Produkt kein Lieferant angegeben ist.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So ändern Sie den Liefertermin und den Lieferanten" auf Seite C-306
*   "So vergleichen Sie die Preise im Bestellpool" auf Seite C-308

### So ändern Sie den Liefertermin und den Lieferanten

1. Wählen Sie `Dokumente > Auftrag > Bestellübergabe`.
2. Wechseln Sie zum Register `Bestellpool`.

**Abb. C-177 Gefährdeten Liefertermin ändern**

*   **A**: Markierung
*   **B**: Bestellung bereits erzeugt
*   **C**: Gefährdeter Termin

3. Markieren Sie die Position (A), zu der Sie den Liefertermin ändern wollen. Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf. Nur die Positionen sind markiert, die mit einem X gekennzeichnet sind.
   Wenn Sie mehrere Positionen markiert haben, wird allen Positionen derselbe neue Liefertermin zugewiesen.
   Wenn Sie nur eine einzelne Position ändern wollen, können Sie den nachfolgenden Dialog mit einem Doppelklick öffnen.

4. Wählen Sie im Menü `Funktionen > Lieferant/Liefertermine ändern`.

**Abb. C-178 Liefertermin ändern**

5. Tragen Sie die neuen Liefertermine ein.
6. Suchen Sie ggf. nach einem anderen Lieferanten.
7. Klicken Sie auf [OK], um die Änderung zu übernehmen. Der Dialog `Lieferant und Liefertermine ändern` wird geschlossen. Im Bestellpool wird die Auftragsposition mit dem neuen Termin angezeigt.
8. Wählen Sie im Menü `Start > Ausführen`, um die Aktion zu starten. Die aktivierten Prüfungen werden durchgeführt. Dies kann je nach Anzahl der Aufträge einige Momente dauern. Bestätigen Sie die jeweiligen Hinweise mit [Ja] oder [Nein], um die Prüfungen fortzusetzen. Wenn alle Prüfungen abgeschlossen sind, werden die Bestellungen übergeben. Die geänderten Termine werden in den Auftrag zurückgeschrieben.

### So vergleichen Sie die Preise im Bestellpool

1. Wählen Sie `Dokumente > Auftrag > Bestellübergabe`.
2. Wechseln Sie zum Register `Bestellpool`.
3. Markieren Sie die Position, zu der Sie die Lieferantenpreise vergleichen wollen. Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf. Nur die Positionen sind markiert, die mit einem X gekennzeichnet sind.

**Abb. C-179 Position, der ein günstigerer Lieferant zugeordnet werden soll**

4. Wählen Sie im Menü `Funktionen > Lieferantenpreise`.

**Abb. C-180 Lieferanten für den Auftrag ändern**

5. Markieren Sie die Checkbox links des Lieferanten, an den die Bestellung der Position gesendet werden soll.
6. Klicken Sie auf [OK], um die Änderung zu übernehmen. Der Dialog `Preisvergleich` wird geschlossen. Im Bestellpool wird die Auftragsposition mit dem neuen Lieferanten angezeigt.

**Abb. C-181 Position mit neuem Lieferanten**

7. Übergeben Sie die Positionen zur Bestellung an den Einkauf, wie in der ersten Handlungssequenz beschrieben.

## Bestellkennzeichen ändern

Sie können für Aufträge in einem Nummernverwalter die Beschaffungsart und den Lieferanten ändern. Wenn Sie nur die Beschaffungsart ändern, werden die Bestellpositionen jeweils beim Standard-Lieferanten bestellt.

### So ändern Sie das Bestellkennzeichen

1. Wählen Sie `Dokumente > Auftrag > NV Auftrag`. Der Dialog `Nummernverwalter` wird geöffnet.
2. Wählen Sie im Menü `Funktionen > Gruppe Bearbeiten > Kennzeichenänderung`.

**Abb. C-182 Bestellkennzeichen auf Positionsebene ändern**

*   **A**: Ebene der Änderung
*   **B**: Lieferant
*   **C**: Kennzeichen zur Änderung der Beschaffungsart
*   **D**: Einschränkung auf Produkt

3. Wählen Sie den Modus (A). In diesem Beispiel wird `Ändern auf Positionsebene` gewählt, um das Kennzeichen für die Auftragspositionen (Hauptprodukt) insgesamt umzusetzen.
4. Markieren Sie die Checkbox `Beschaffungsart ändern` (C) und wählen Sie die alte und die neue Beschaffungsart aus. Für alle Positionen wird die Beschaffungsart geändert. Wenn Sie die Beschaffungsart `Bestellung` gewählt haben, können Sie auch einen bestimmten Lieferanten auswählen.
5. Wenn die Änderung nur für ein bestimmtes Produkt gelten soll, tragen Sie die Produktnummer (C) ein. Die Produktbezeichnung wird angezeigt.
6. Markieren Sie ggf. die Checkbox `Lieferant ändern` (B) und wählen Sie einen neuen Lieferanten aus. Alle Bestellpositionen werden beim gewählten Lieferanten bestellt. Diese Einstellung können Sie auch wählen, ohne die Beschaffungsart zu ändern.
7. Markieren Sie ggf. die Checkbox `Bestellung direkt an den Kunden`. Die Bestellung wird in diesem Fall direkt beim Kunden angeliefert. Das ist nur sinnvoll, wenn die Bestellteile nicht für die Produktion benötigt werden.
8. Klicken Sie auf [OK], um die Daten zu speichern. Das neue Kennzeichen wird in allen Dokumenten des aktuellen Nummernverwalters gespeichert.
9. Klicken Sie auf [Ende], um den Dialog zu schließen. Der Dialog `Bestellkennzeichen ändern` wird geschlossen. Die Änderungen werden in die Aufträge zurückgeschrieben.

> Wenn Positionen geändert wurden, die bereits übergeben waren, müssen Sie entscheiden, was als nächstes zu tun ist:
> *   **Der Lieferant hat die Bestellung bereits bestätigt:** Besprechen Sie die Änderung mit dem Einkauf und mit dem Lieferanten. Stornieren Sie ggf. die alte Bestellung und übergeben Sie die geänderte Position erneut.
> *   **Die Bestellung wurde noch nicht an den Lieferanten gesendet oder der Lieferant hat noch nicht bestätigt:** Übergeben Sie die Position erneut und machen Sie ggf. den Einkauf auf die Änderung aufmerksam.

Im Dialog `Dokumentendaten` können Sie die Termine bearbeiten und den Kunden über diese Änderungen benachrichtigen.

## Übungen

### Bestellposition erfassen
Öffnen Sie einen Auftrag und erfassen Sie zwei Positionen.
*   Wählen Sie für eine Position das Kennzeichen `Bestellung`.
*   Wählen Sie für die andere Position das Kennzeichen `Bestellung (komplett)`.

### Auftrag übergeben
Stellen Sie den Auftrag in den Bestellpool.
*   Prüfen Sie die Lieferanten und Preise im Bestellpool.
*   Ändern Sie den Liefertermin.
*   Übergeben Sie die Bestellungen:
    *   Prüfen Sie, ob zu allen Positionen mit dem Bestellkennzeichen eine Bestellung erzeugt wurde.
    *   Prüfen Sie in den neuen Bestellungen die Termine und den Lieferanten.

### Ergänzende Informationen

## Bestellungen

### Lernziele
*   Bestellung kennenlernen.
*   Referenzierte Bestellung vs. Lagerbestellung.

### Nutzen
*   Sie kennen den Unterschied zwischen referenzierten und unabhängigen Bestellungen.
*   Sie können sich eine Übersicht zu den Bestellungen anzeigen lassen, die aus einem bestimmten Auftrag erzeugt wurden, und daran erkennen, ob der Auftrag weiter bearbeitet werden kann.

### Merke
| Begriff | Beschreibung |
| :--- | :--- |
| **Dokument erzeugen** | Bestellungen können auf unterschiedliche Weise erzeugt werden: <ul><li>Durch die Bestellübergabe werden Bestellungen aus einem Auftrag erzeugt.</li><li>Durch das Erfassen einer Bestellung. Diese Bestellungen dienen i. d. R. dazu, die Lagerbestände zu ergänzen. Sie werden in der Schulung zum Thema Einkauf behandelt.</li></ul> |
| **Bestellung** | Bestellungen sind genauso aufgebaut wie Aufträge. |
| **Referenzen** | Durch Referenzen ist gekennzeichnet, aus welchem Auftrag die Bestellung erzeugt wurde. |
| **Bestell-Info** | Zu einem Auftrag werden alle referenzierten Bestellungen angezeigt. |
| **Änderungen** | Wenn in einer referenzierten Bestellung ein Termin geändert wurde, wird die Änderung in den Auftrag zurückgeschrieben. |
| **Voreinstellungen** | Keine |

### Dokumentenkopf Bestellung
Bestellungen werden im Rahmen dieser Schulung aus Aufträgen erzeugt, in denen Positionen mit Bestellkennzeichen enthalten sind.

Bestellungen, die unabhängig von Aufträgen erfasst werden, sind ausführlich im Part Einkauf beschrieben.

Aus dem Auftrag der vorausgegangenen Lerneinheit wurden zwei Bestellungen erzeugt. Beide Bestellungen sind genauso aufgebaut wie die Aufträge, die am Anfang dieser Schulung behandelt wurde.

In der folgenden Abbildung ist der Dokumentenkopf der ersten Bestellung wiedergegeben. Zu dieser Bestellung wurde zusätzlich der Termin der Anlieferung beim Kunden geändert.

**Abb. C-183 Bestellung aus einem Auftrag**
*   **A**: Geänderter Anliefertermin
*   **B**: Auftrag, zu dem die Bestellung erzeugt wurde

### Bestellposition
Auch in den Positionen einer Bestellung wird auf den Kundenauftrag hingewiesen.

**Abb. C-184 Bestellposition aus Auftrag**
*   **A**: Referenz auf den Kunden
*   **B**: Hinweis

In der Spalte `Hinweis` (B) wird angezeigt, dass diese Bestellung aus einem Auftrag erzeugt wurde.

### Auftrags-/Bestellinfo
Im Abschnitt zur Historie haben Sie gelernt, dass alle referenzierten Dokumente zu einem Antrag angezeigt werden. Aus der Historie können Sie aber keine Details über diese Dokumente ersehen. Um sich über referenzierten Bestellungen zu einem Auftrag zu informieren, steht der Dialog `Auftrag-/Bestell-Info` zur Verfügung.

**Abb. C-185 Auftrags- und Bestell-Info**

In dieser Übersicht werden alle Bestellungen angezeigt, die zu den Auftragspositionen erzeugt wurden. Sie können sehen, zu welchen Bestellungen bereits Lieferungen eingegangen sind und wann mit der Lieferung insgesamt zu rechnen ist.

## Übungen

### Bestellung erfassen
Erfassen Sie eine unabhängige Bestellung.
*   Erfassen Sie in einer Position fünf Kisten mit Float 5 mm.
*   Erfassen Sie in einer zweiten Position fünf Kisten mit Float 5 mm.

### Bestellung ändern
Ändern Sie den Lieferanten in der referenzierten Bestellung.
*   Ändern Sie den Lieferanten für die Position 1.
*   Ändern Sie den Lieferanten für den gesamten Auftrag.

### Referenzen anzeigen
Prüfen Sie die Referenzen:
*   im Dialog `Auftrags-/Bestell-Info`.
*   im Dialog `Historie`.

## Dokumentendaten

### Lernziele
*   Funktionen des Dialogs kennenlernen.
*   Liefertermin im Auftrag ändern.
*   Dokumente für gemeinsame Änderungen sammeln.

### Nutzen
*   Termine und Lieferanten können Sie in referenzierten Dokumenten gemeinsam prüfen und ändern.
*   Wenn Sie Ihre Nummernverwalter entsprechend organisiert haben, können Sie Änderungen für alle darin gesammelten Dokumente gemeinsam durchführen.

### Merke
| Begriff | Beschreibung |
| :--- | :--- |
| **Dialog Dokumentendaten** | Im Dialog `Dokumentendaten` können die Termine für folgende Dokumente und Referenz-Dokumente geprüft werden: <ul><li>Angebot</li><li>Auftrag, Bestellung</li><li>Anfrage</li><li>Gutschrift</li></ul> |
| **Referenz-Dokumente** | Referenzierte Bestellungen werden nur zu einem einzelnen Auftrag angezeigt. Sie werden nicht angezeigt, wenn die Dokumente eines Nummernverwalters aufgelistet werden. |
| **Gemeinsame Änderungen** | Status, Termine, Tour und Lieferbedingungen können für mehrere Dokumente gemeinsam geändert werden. |
| **Voreinstellungen** | **Stammdaten** <ul><li>Kunden: Faxnummer und/oder E-Mail-Adresse</li><li>Texte: Standardtexte für die Kundenbenachrichtigungen</li><li>Formularverwaltung: Druckpunkte, Formulare</li><li>Status: Statuspunkte müssen angelegt und zugeordnet sein.</li></ul> |

## Lieferdaten anzeigen

Eine Übersicht über die Daten eines Dokuments steht im Dialog `Dokumentendaten` zur Verfügung. Aus diesem Dialog heraus können Teile der Kopfdaten bearbeitet werden, z. B. der Status oder die Termine.

Sie können dabei wahlweise ein einzelnes Dokument oder mehrere Dokumente gleichzeitig ändern. Die Dokumente können aus einem Nummernverwalter genommen werden oder müssen über die Dokumentennummer gesammelt werden.

Der Dialog bietet außerdem die Möglichkeit, alle referenzierten Bestellungen gemeinsam mit dem Auftrag aufzulisten. In dieser Konstellation betreffen die Änderungen dann auch die referenzierten Bestellungen.

**Abb. C-186 Termine für Auftrag mit Bestellpositionen prüfen**
*   **A**: Auftrag mit Bestellpositionen
*   **B**: Referenzierte Bestellungen

## Lieferterminkontrolle

Sie können die Liefertermine für Aufträge und für Bestellungen prüfen und ggf. korrigieren. Dies führen Sie in zwei Schritten durch:

*   Im Dialog `Dokumentendaten` prüfen und korrigieren Sie die Termine. Mit diesem Vorgehen werden die Termine automatisch auch im Auftrag und in der Bestellung geändert.
*   Im Dialog `Kundenbenachrichtigung` (Lieferterminkontrolle) benachrichtigen Sie den Kunden über die Verzögerung. Für die Benachrichtigung des Kunden können Sie auch die Möglichkeiten im Menü `Kommunikation` nutzen - oder einfach anrufen.

Über die Lieferterminkontrolle können Bestellungen geprüft werden. Bei ausstehenden Lieferungen können die Termine geändert und der Kunde direkt benachrichtigt werden.

## Dokumentenansicht

Die Dokumentenansicht kann aus dem Dialog `Dokumentendaten` heraus angezeigt und gedruckt werden. Damit können Sie die Details eines Dokuments prüfen, ohne den Dialog `Dokumentendaten` zu verlassen.

Wenn Sie die Dokumentenansicht drucken, werden nicht die hinterlegten Formulare verwendet und der Status des Dokuments wird nicht erhöht. Dieser Druck kann nicht mit dem "offiziellen" Druck verwechselt werden, da die wesentlichen Kopf- und Fußdaten nicht wiedergegeben sind.
⇨ "Formular- und Etikettendruck" auf Seite C-191

## Liefertermin prüfen und ändern

Im Dialog `Dokumentendaten` können Sie sich die referenzierten Bestellungen zusammen mit dem Auftrag anzeigen lassen, um die Termine zu prüfen und ggf. zu ändern.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So prüfen und ändern Sie referenzierte Dokumente" auf Seite C-321
*   "So benachrichtigen Sie den Kunden über neue Liefertermine" auf Seite C-323

### So prüfen und ändern Sie referenzierte Dokumente
1. Wählen Sie `Dokumente > Dokumentendaten`. Der Dialog `Dokumente` wird geöffnet.
2. Stellen Sie sicher, dass die Checkbox `Nummernverwalter` nicht markiert ist. Das Feld für die Auftragsnummer ist nur freigeschaltet, wenn keine Nummernverwalter angezeigt werden.
3. Geben Sie die Auftragsnummer ein und übernehmen Sie die Daten mit `<Enter>`.

**Abb. C-187 Termine für Auftrag mit Bestellpositionen prüfen**
*   **A**: Versandtag anpassen
*   **B**: Bestätigten Termin des Lieferanten anpassen

Die Kopfdaten des Auftrags und der Bestellung(en) werden angezeigt.

4. Passen Sie den Liefertermin (B) an, den der Lieferant für die Bestellung angegeben hat.
5. Passen Sie das Datum für den Versandtag (A) und/oder für die Anlieferung beim Kunden an. Wenn Sie die Termine über den Kalender auswählen, können Sie die Tourentage für den Kunden berücksichtigen.

**Abb. C-188 Geänderte Termine**

6. Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern. Die neuen Termine werden gespeichert und in die zugehörigen Dokumente übernommen. Sie können jetzt den Kunden über den geänderten Termin informieren.

### So benachrichtigen Sie den Kunden über neue Liefertermine

> **Voraussetzung**
> In den Stammdaten des Kunden muss eine E-Mail-Adresse hinterlegt sein. Im Auftrag muss im Bereich Anschrift die Checkbox Mail aktiviert sein.

1. Wählen Sie `Dokumente > Kundenbenachrichtigung`. Sie können diesen Dialog auch aus einem Auftrag heraus öffnen. Bei diesem Weg können Sie das Lieferdatum des aktuellen Auftrags jedoch nicht mehr ändern, da der geöffnet ist und damit gesperrt.

**Abb. C-189 Kundenbenachrichtigung**
*   **A**: Modus Aufträge oder Bestellungen
*   **B**: Einschränkung auf Nummernverwalter
*   **C**: Einschränkung auf Status
*   **D**: Einschränkung auf Datum

2. Wählen Sie den Modus (A) `Aufträge` oder `Bestellungen`. In diesem Beispiel soll ein Kunde über die Lieferterminverschiebung seines Auftrags informiert werden.
3. Schränken Sie die Auswahl auf einen Nummernverwalter (B) oder einen Status (C) ein. Wenn in dem Nummernverwalter sehr viele Dokumente aufgelistet sind, können Sie die Anzeige auf ein Lieferdatum (D) einschränken.
4. Wählen Sie im Menü `Start > Suchen`, um in die Daten einzulesen.

**Abb. C-190 Liefertermin beim Kunden ändern**
*   **A**: Neuer Liefertermin
*   **B**: Liefertermin verschoben
*   **C**: Kundenbenachrichtigung für markierten Auftrag erstellen

5. Markieren Sie im Register `Terminverschiebung` den Auftrag (C), zu dem Sie den Liefertermin beim Kunden ändern müssen, und prüfen Sie den neuen Termin (A). Sie können mehrere Aufträge markieren und einen neuen Liefertermin festlegen. In diesem Fall können Sie die Tour nur ändern, wenn alle Aufträge mit derselben Tour ausgeliefert werden.
6. Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern.
7. Wählen Sie im Menü `Drucken > Drucker`. Die Benachrichtigung wird angezeigt und kann entsprechend dem Ausgabeformat gespeichert und versendet werden.

### Dokumente für gemeinsame Änderungen sammeln

Wenn Sie z. B. in mehreren Aufträgen gemeinsam die Tour ändern wollen, können Sie diese Dokumente in einem Nummernverwalter zusammenstellen und dann ändern.
Alternativ dazu haben Sie die Möglichkeit, die Aufträge im Dialog `Dokumentendaten` zu sammeln und gemeinsam zu ändern.

#### So sammeln Sie Dokumente für gemeinsame Änderungen
1. Wählen Sie `Dokumente > Dokumentendaten`. Der Dialog `Dokumentendaten` wird geöffnet.
2. Wählen Sie im Feld `Dokument` die Dokumentenart aus, z. B. `Auftrag`.
3. Stellen Sie sicher, dass die Checkbox `Nummernverwalter` nicht markiert ist.
4. Geben Sie die Auftragsnummer ein und übernehmen Sie die Daten mit `<Enter>`. In der Übersicht werden die Daten des Auftrags angezeigt.
5. Wiederholen Sie diesen Schritt, bis Sie alle Aufträge zusammengestellt haben, die Sie gemeinsam ändern wollen. In der Übersicht werden alle Aufträge aufgelistet.
6. Ändern Sie im Bereich `Auftrag` z. B. die Tour. Sie können zusätzlich das Lieferdatum ändern, wenn alle Aufträge am selben Tag geliefert werden sollen.
7. Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern. Die neue Tour wird in alle aufgelisteten Aufträge übernommen.

## Übungen

### Dokumentendaten prüfen
*   Prüfen Sie im Dialog `Dokumentendaten` die referenzierten Dokumente.
*   Ändern Sie den Produktionstermin und passen Sie den Liefertermin entsprechend an.

### Ergänzende Informationen
⇨ Softwarereferenz, "Dokumentendaten" auf Seite C-738
⇨ Softwarereferenz, "Kundenbenachrichtigung (Lieferterminkontrolle)" auf Seite C-565

# Tutorial: Angebote

## Angebote
In diesem Themenblock lernen Sie, wie Sie Angebote und Alternativen zu einem Angebot erfassen.

Dazu gehören folgende Lerneinheiten:
*   "Angebotserfassung" auf Seite C-328
*   "Angebotsverfolgung" auf Seite C-342
*   "Angebotsstatistik" auf Seite C-348

## Angebotserfassung

### Lernziele
*   Unterschied zwischen Angebot und Auftrag kennenlernen.
*   Unterschiede zwischen alternativem Angebot und alternativer Position kennenlernen.
*   Alternative Position erfassen.
*   Zu einem Angebot ein vollständiges Alternativangebot erstellen.

### Nutzen
*   Mit einem alternativen Angebot können Sie Vorschläge zu den Wünschen eines Kunden erfassen und später diejenigen Positionen in einen Auftrag übernehmen, für die sich der Kunde entschieden hat.
*   Sie müssen die Daten aus Angeboten nicht erneut erfassen, wenn Sie einen entsprechenden Auftrag erfassen wollen.

### Merke
| Begriff | Beschreibung |
| :--- | :--- |
| **Angebot** | In A+W Business wird bei folgenden Sachverhalten ein Angebot erfasst: <ul><li>Kostenvoranschlag für den Kunden</li><li>Alternative Vorschläge zu einem zukünftigen Auftrag</li><li>Preisliche Alternativen beim Austausch von Gläsern, Sprossen, Modellen und Bearbeitungen</li></ul> |
| **Dokument** | Angebote sind eigenständige Dokumente. Für die Angebote wird ein eigener Nummernkreis verwendet. Das Angebot kann auf unterschiedliche Weise erzeugt werden: <ul><li>durch Kopieren aus einem Auftrag</li><li>durch Erfassen eines neuen Dokuments</li></ul> |
| **Alternativangebot** | Alternativangebote werden im Nummernkreis der Angebote verwaltet. |
| **Voreinstellungen** | **Stammdaten:** <ul><li>Nummernkreise</li></ul> **Firmendaten:** <ul><li>Register System (Wiedervorlage)</li><li>Register Produktion (Optimierung)</li></ul> |

## Angebot und Alternativen
Zu Beginn eines kaufmännischen Prozesses steht ein Angebot. Für dieses erfassen Sie alle Daten mit den gewünschten Spezifikationen. A+W Business prüft dabei bereits während der Eingabe, ob die erfassten Produkte im Lager vorrätig sind oder angefertigt werden müssen und ob die hinterlegten Restriktionen verletzt werden. So wird sichergestellt, dass die angebotenen Positionen tatsächlich produziert werden können.

Angebote werden auf die gleiche Weise erfasst wie Aufträge.

### Alternative Positionen
Zu den Positionen können alternative Positionen erfasst werden, die nicht mit in die Angebotssumme gerechnet werden.

Hat der Kunde sich für ein Angebot entschieden, können Sie mit der Kopierfunktion das Angebot in einen Auftrag umwandeln und dabei die gewünschten Positionen auswählen.

### Alternativangebot
Neben den alternativen Angebotspositionen können Sie auch alternative Angebote erzeugen. So können Sie beispielsweise Gläser austauschen, Modelle, Sprossen und Bearbeitungen zu Positionen ändern, hinzufügen oder löschen.

Wenn Sie ein Alternativangebot erstellen, werden die Daten aus dem Dokumentenkopf automatisch übernommen. Sie müssen also lediglich die Positionsdaten bearbeiten. Das Alternativangebot kann als separates Dokument gespeichert werden.

In einem Überblick können Sie sich anzeigen lassen, welche Alternativangebote zu einem Angebot erstellt wurden.

### Wiedervorlage
Im Dialog `Wiedervorlage` können Sie sich alle Angebote anzeigen lassen, die innerhalb eines bestimmten Zeitraums wieder vorgelegt werden sollen.

**Abb. C-191 Automatische Meldung beim Systemstart**

Sie können jedem Angebot einen Termin zur Wiedervorlage mitgeben, an dem Sie automatisch erinnert werden, sich erneut mit dem Kunden in Verbindung zu setzen.

Die Wiedervorlage wird ausführlich in einer separaten Einheit erklärt.
⇨ "Angebotsverfolgung" auf Seite C-342

## Angebotsoptimierung
Bei ungewöhnlichen Scheibengrößen oder Mengen können Sie ein Angebot probehalber an die Produktion übergeben, um den Verschnitt berechnen zu lassen. Aus den zurückgemeldeten Daten können Sie dann die Preise im Angebot neu kalkulieren.

Die Angebotsoptimierung wird in der Schulung zum Part Fertigung behandelt.

## Alternativangebotsübersicht
Zu einem Angebot werden alle Alternativangebote aufgelistet. Details zu den Alternativen werden angezeigt, wenn die jeweilige Alternative markiert ist.

**Abb. C-192 Übersicht über die Alternativangebote zu einem Angebot**

Alternative Positionen werden in dieser Übersicht nicht aufgeführt. Wenn Sie in einem Angebot alternative Positionen erfasst haben, können Sie diese im Angebot selbst an der blauen Schrift erkennen.

## Alternative Position im Angebot erfassen
In dieser Einheit lernen Sie, wie Sie ein Angebot mit alternativen Positionen erfassen. Den Dokumentenkopf und die Positionen erfassen Sie in gleicher Weise wie im Auftrag. Auf diese Bedienschritte wird hier daher nicht nochmal eingegangen.

### So erfassen Sie eine alternative Position
1. Wählen Sie `Dokumente > Angebot > Angebot auswählen > Register Positionen` oder `<F9>`. Die Positionserfassung wird geöffnet.
2. Erfassen Sie die Alternativposition genauso, wie Sie jede andere Position erfassen.

**Abb. C-193 Alternative Position erfassen**

3. Markieren Sie im Bereich `Positionen` die Alternativposition und wechseln Sie zum Register `Zusatz`.

**Abb. C-194 Alternative Position speichern**
*   **A**: Auswahl der Bezugsposition
*   **B**: Alternative Position

4. Wählen Sie die Position (A) aus, zu der Sie die Alternativposition erfasst haben.
5. Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern.
   Die alternative Position wird gespeichert. Die alternativen Positionen werden mit orangefarbenem Hintergrund dargestellt und im Ausdruck gekennzeichnet.
6. Schließen Sie die Positionserfassung, um zum Register `Summen` zu wechseln.
   Im Gesamtpreis wird die alternative Position nicht berücksichtigt.

**Abb. C-195 Preis der Alternativposition wird nicht ins Angebot übernommen**
*   **A**: Preis der Original-Position
*   **B**: Auftragswert im Register Summen

Im Register `Summen` beziehen die Felder in den Bereichen Kosten/Deckungsbeitrag, Kreditlimit und Wertvolumen alternative Positionen nicht mit ein.

7. Prüfen Sie in den Kopfdaten im Register `Dokument` das Datum im Feld `Vorlage`, damit Sie automatisch daran erinnert werden, das Angebot weiterzuverfolgen.
8. Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern.

## Alternatives Angebot erfassen
In dieser Einheit lernen Sie, wie Sie ein Alternativangebot zu einem bestehenden Angebot erfassen.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So erfassen Sie alternative Gläser oder Abstandhalter" auf Seite C-334
*   "So erfassen Sie eine alternative Sprossenkonstruktion" auf Seite C-338

### So erfassen Sie alternative Gläser oder Abstandhalter
1. Öffnen Sie das Angebot, zu dem Sie ein Alternativangebot erfassen wollen.

**Abb. C-196 Original-Angebot**

2. Wählen Sie im Menü `Funktionen > Gruppe Dokument > Alternativen`.

**Abb. C-197 Alternatives Angebot erstellen**
*   **A**: Originalnummer nicht übernehmen
*   **B**: Markierte Position
*   **C**: Kopieren

3. Markieren Sie die Position(en), die Sie in das Alternativangebot übernehmen möchten. Sie können mehrere Positionen markieren. In der Spalte `Neu` der markierten Position(en) ist die Checkbox (B) markiert.

> **Dokumentennummer für Alternativen**
> Wenn Sie die Checkbox `Originalnummer gleich Alternative` (A) markiert haben, wird das Original-Dokument überschrieben. Wenn Sie ein neues Dokument als Alternative zum Original erstellen möchten, darf die Checkbox nicht markiert sein. Das neue Dokument erhält dann eine neue Nummer.

4. Klicken Sie auf [Kopieren] (C) und prüfen Sie im Register `Alternative`, ob alle Positionen aufgeführt sind, die Sie übernehmen möchten.
5. Markieren Sie im Register `Original` die Position, zu der Sie eine Alternative erfassen möchten. Um alle Markierungen zu entfernen, können Sie auf [Keine] klicken und dann die gewünschte(n) Position(en) einzeln markieren.

**Abb. C-198 1. Glas tauschen**
*   **A**: Modus auswählen
*   **B**: Glas, das ersetzt werden soll
*   **C**: Glas, das eingebaut werden soll
*   **D**: Änderung starten

6. Wählen Sie den Modus (A), z. B. `1. Glas`, wenn Sie für diese Stücklisten-Komponente eine Alternative angeben möchten. Sie können zu jeder Position mehrere Modi wählen und Alternativen eintragen. Die folgenden Handlungsschritte müssen für jeden Modus einzeln ausgeführt werden.

> **Modus Modell, Sprosse und Bearbeitung**
> Wenn Sie den Modus `Modelle/Bearbeitungen` oder `Sprossenkonstruktion` wählen, wird die Schaltfläche [Definition] freigeschaltet.
> ⇨ "So erfassen Sie eine alternative Sprossenkonstruktion" auf Seite C-338

7. Tragen Sie im Feld `Suchen von` (B) die Produktnummer ein, zu der Sie eine Alternative angeben möchten, z. B. `1004` für das 1. Glas einer ISO-Einheit.
8. Tragen Sie im Feld `Einfügen/Ersetzen durch` (C) die alternative Produktnummer ein, z. B. `1005`.

> **Generelle Ersetzungen**
> Wenn Sie alle Positionen markiert haben und den Modus `Hauptprodukt` gewählt haben, wird ein Glas in allen Positionen ersetzt, in denen die entsprechende Produktnummer vorkommt. Bei dem Beispiel in Schritt 7/8 würde in allen Positionen das Produkt 1004 durch das Produkt 1005 ersetzt, also auch in VSG-Scheiben oder die einfachen Gläser.
> Wenn Sie das Feld `Suchen von` leer lassen, werden alle Gläser in allen markierten Positionen durch das alternative Produkt ersetzt.

9. Bestätigen Sie die beiden Werte mit [Einfügen/Ersetzen] (D). Sie können die Preise für die Alternative sofort mit [Preisberechnung] berechnen lassen. Sie können die Preise auch neu berechnen lassen, nachdem Sie alle Alternativen angegeben haben.
10. Wiederholen Sie die Schritte 3 bis 9 für den nächsten Modus der markierten Position oder für andere Positionen. Sie können als Alternative auch andere Preise und/oder Rabatte auswählen und diese mit [Einfügen/Ersetzen] speichern.

> **Alternativen für markierte Positionen**
> Achten Sie darauf, dass nur die Positionen markiert sind, die im Alternativangebot mit geänderten Stücklisten-Komponenten aufgeführt werden sollen. Die Markierung einer Position wird nicht automatisch entfernt, wenn Sie eine andere Position markieren.

11. Wechseln Sie zum Register `Alternative`, um den aktuellen Stand der Alternativen zu prüfen.

**Abb. C-199 1. Glas getauscht**

12. Wählen Sie im Menü `Start > Ausführen`, um das Alternativangebot zu erstellen. Beantworten Sie die Abfragen und Meldungen. Das alternative (neue) Angebot wird erstellt. In der Titelzeile wird die neue Nummer angezeigt.
13. Schließen Sie den Dialog. Die Dokumentenverwaltung wird wieder im Vordergrund angezeigt. In der Dokumentenübersicht wird das neue Dokument aufgeführt und mit einem Pfeil im Zeilenkopf gekennzeichnet. Wenn Sie das Original-Dokument überschrieben haben, werden die neuen Daten angezeigt.

### So erfassen Sie eine alternative Sprossenkonstruktion
1. Führen Sie die Schritte 1 bis 5 wie in der vorhergehenden Handlungssequenz aus.

**Abb. C-200 Sprossenkonstruktion ändern**
*   **A**: Markierte Position
*   **B**: Modus

2. Wählen Sie den Modus (B), z. B. `Sprossenkonstruktion`. Die Schaltfläche [Definition] wird freigeschaltet. Sie können zu jeder Position mehrere Modi wählen und Alternativen eintragen. Die folgenden Handlungsschritte müssen für jeden Modus einzeln ausgeführt werden.
3. Geben Sie die Produktnummer der Sprossen an, die ersetzt werden sollen.
4. Klicken Sie auf [Definition], um zum Register `Sprossen` zu wechseln. Wenn Sie ein Modell oder die Bearbeitung ändern wollen, wird je nach Modus zum entsprechenden Register gewechselt.

**Abb. C-201 Alternative Sprossen**
*   **A**: Waagerechte Sprossen ändern
*   **B**: Senkrechte Sprossen ändern

5. Legen Sie die Alternative fest, z. B. breitere Sprossen oder eine andere Sprossenkonstruktion. Dazu müssen Sie die Sprossenkonstruktion auch dann angeben, wenn Sie nur die Sprossen selbst ändern wollen. Wie Sie Sprossenkonstruktionen aufbauen, ist ausführlich einer separaten der Einheit erklärt.
   ⇨ "Sprossen erfassen" auf Seite C-107
6. Wählen Sie im Menü `Start > Ausführen`, um die Änderung zu übernehmen. Die Anzeige wechselt wieder zum Register `Original`. Prüfen Sie nochmals, ob die richtige Position markiert ist.
7. Klicken Sie auf [Einfügen/Ersetzen], um die Sprossenkonstruktion einzulesen. Die Änderung wird im Feld `Einfügen/ersetzen durch` angezeigt.
8. Wiederholen Sie die Schritte 4 bis 5 für den nächsten Modus der markierten Position oder für andere Positionen.

> **Alternativen für markierte Positionen**
> Achten Sie darauf, dass nur die Positionen markiert sind, die im Alternativangebot mit geänderten Stücklisten-Komponenten aufgeführt werden sollen. Die Markierung einer Position wird nicht automatisch entfernt, wenn Sie eine andere Position markieren.

9. Wechseln Sie zum Register `Alternative`, um den aktuellen Stand der Alternativen zu prüfen.
10. Wählen Sie im Menü `Start > Ausführen`, um das Alternativangebot zu erstellen. Das alternative (neue) Angebot wird erstellt. Die Nummer des neuen Angebots wird in der Titelzeile angezeigt.
11. Schließen Sie den Dialog `Alternativen`. Der Dialog `Dokumentenverwaltung` wird wieder angezeigt. In der Dokumentenübersicht wird das Alternativangebot aufgeführt und mit einem Pfeil im Zeilenkopf gekennzeichnet.

**Abb. C-202 Alternativangebot**

Sie können die Daten des Alternativangebots weiter bearbeiten, z. B. den Termin zur Wiedervorlage oder die Preise.

## Übungen

### Angebot mit alternativer Position erfassen
*   Kopieren Sie einen Ihrer Aufträge in ein Angebot für einen anderen Kunden.
*   Erfassen Sie in diesem neuen Angebot zu Position 1 eine alternative Position.

### Alternativangebot erfassen
*   Erfassen Sie ein Alternativangebot zu dem Angebot.
*   Wechseln Sie in Position 2 die Außenscheibe in ein Ornamentglas.
*   Fügen Sie in Position 3 ein (anderes) Sprossengitter ein.

### Angebot in Auftrag überführen
Kopieren Sie Ihr Angebot in einen Auftrag.
*   Übernehmen Sie die Positionen vollständig (1:1).

### Ergänzende Informationen
⇨ "Alternativangebot" auf Seite C-329
⇨ "Angebotsverfolgung" auf Seite C-342
⇨ "Angebotsstatistik" auf Seite C-348
⇨ Softwarereferenz, "Wiedervorlage" auf Seite C-394
⇨ Softwarereferenz, "Angebotsstatistik" auf Seite C-397
⇨ Softwarereferenz, "Dokument - Kopfdaten" auf Seite C-417

## Angebotsverfolgung

### Lernziele
*   Angebote als Wiedervorlage anzeigen lassen.

### Nutzen
*   Nach einer automatischen Erinnerung an Angebote können Sie den Kontakt zum Kunden wieder aufnehmen und daraus einen neuen Auftrag erstellen.

### Merke
| Begriff | Beschreibung |
| :--- | :--- |
| **Wiedervorlage** | Sie können sich automatisch an Angebote erinnern lassen, deren Wiedervorlagetermin erreicht ist. |
| **Voreinstellungen** | **Stammdaten** <ul><li>Auftrag > Kategorien</li></ul> **Firmendaten:** <ul><li>Register System > Vorlauftage</li></ul> |

## Wiedervorlage
Angebote sind dann erfolgreich, wenn sie in Aufträgen münden. Dazu können Sie beitragen, indem Sie den Kunden nach einer Bedenkfrist erneut ansprechen. Sie selbst können sich an die offenen Angebote erinnern lassen oder sich offene Angebote nach einem bestimmten Termin anzeigen lassen.

**Abb. C-203 Termin zur Wiedervorlage**

Zur Wiedervorlage können sowohl Angebot als auch Aufträge angezeigt werden. Die nachfolgenden Beschreibungen für Angebote gelten in gleicher Weise auch für Aufträge.

Die Erinnerungsfrist wird in den Firmendaten eingetragen. Danach wird beim Erfassen eines Angebots automatisch ein Datum zur Wiedervorlage eingefügt, das Sie jederzeit anpassen können, z. B., wenn Sie mit dem Kunden einen solchen Termin abgesprochen haben.

Wenn der Termin zur Wiedervorlage fällig ist, wird automatisch die Meldung angezeigt, dass ein Angebot vorliegt, zu dem Sie wieder Kontakt mit dem Kunden aufnehmen wollen.

**Abb. C-204 Automatische Meldung beim Systemstart**

Aus der Übersicht der betreffenden Angebote können Sie sich jedes Angebot anzeigen lassen und nachverfolgen. Mit einem neuen Datum kann das Angebot erneut zur Wiedervorlage gespeichert werden. Soll es nicht wieder vorgelegt werden, können Sie es direkt archivieren und löschen.

## Angebot verfolgen
In dieser Einheit lernen Sie, wie Sie sich Angebote zur Weiterverfolgung anzeigen lassen.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So stellen Sie die automatische Erinnerung ein" auf Seite C-344
*   "So lassen Sie sich Angebote zur Wiedervorlage anzeigen" auf Seite C-345
*   "So geben Sie alte Angebote zur Archivierung oder zum Löschen frei" auf Seite C-346

### So stellen Sie die automatische Erinnerung ein
1. Wählen Sie `Dokumente > Angebot > Wiedervorlage`.

**Abb. C-205 Wiedervorlage**
*   **A**: Vorlagedatum oder -zeitraum
*   **B**: Intervall für die Wiedervorlage

2. Wählen Sie im Menü `Optionen > Automatische Benachrichtigung`.

Diese Einstellung gilt übergreifend für alle Angebote. Wenn Sie A+W Business das nächste Mal starten, wird im Kommentarbereich ein Hinweis auf die Angebote angezeigt, die zur Nachverfolgung anstehen.
3. Markieren Sie das Angebot, in dem Sie das Datum zur Wiedervorlage prüfen und ggf. anpassen wollen.
4. Markieren Sie die Checkbox `Vorlage alle` (B), wenn Sie sich das Angebot in Intervallen anzeigen lassen wollen.
5. Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern. Die Änderungen werden gespeichert.

### So lassen Sie sich Angebote zur Wiedervorlage anzeigen
6. Wählen Sie im Menü `Start > Filter`, um in den Such-Modus zu wechseln.

**Abb. C-206 Wiedervorlage – Such-Modus**
*   **A**: Vorlagedatum
*   **B**: Bis-Datum für Zeitraum

7. Tragen Sie in den Feldern `Vorlagedatum` (A) und `bis` (B) den gewünschten Zeitraum ein.
8. Wählen Sie im Menü `Start > Suchen`, um in die Suche zu starten.

**Abb. C-207 Wiedervorlage – Trefferliste**

Im Bereich `Tabelle` werden alle Angebote mit einem Vorlagedatum aus dem angegebenen Zeitraum aufgelistet. Sie können ein neues Datum zur Wiedervorlage einstellen und mit [OK] speichern.
9. Klicken Sie in der Übersicht doppelt auf das Angebot, das Sie prüfen wollen. Das Angebot wird geöffnet.

### So geben Sie alte Angebote zur Archivierung oder zum Löschen frei
1. Lassen Sie sich die alten Angebote anzeigen, indem Sie einen entsprechenden Zeitraum für die Vorlagetage einstellen.
2. Markieren Sie in der Übersicht das Angebot, dessen Status Sie umsetzen wollen.
3. Wählen Sie eine Kategorie aus.
4. Markieren Sie die Checkbox `Übergabe Archiv`, wenn das Angebot zunächst archiviert werden soll.
5. Wählen Sie im Menü `Start > Speichern`, um den Status zur Archivierung umzusetzen.
6. Markieren Sie die Checkbox `Löschfreigabe`, wenn das Angebot gelöscht werden soll. Wenn Sie diese Checkbox zuerst markieren, können Sie das Angebot anschließend nicht archivieren.
7. Wählen Sie im Menü `Start > Speichern`, um den Status umzusetzen. Der Status wird umgesetzt und Sie können das nächste Angebot markieren und ändern.

## Übungen

### Datum zur Wiedervorlage einstellen
Stellen Sie für Ihre Angebote das Datum zur Wiedervorlage ein.
*   Tragen Sie im Register `Dokument` das Datum im Feld `Vorlage` ein.
*   Wählen Sie dazu das Datum des Folgetags, wenn Sie die Lerneinheit am nächsten Tag nochmals durchgehen wollen.

### Angebote zur Wiedervorlage anzeigen
Lassen Sie sich die Angebote zum eingestellten Datum im Dialog `Wiedervorlage` anzeigen.

### Ergänzende Informationen
⇨ Softwarereferenz, "Wiedervorlage" auf Seite C-394
⇨ Stammdaten, "Vorlauftage für Wiedervorlage" auf Seite B-976

## Angebotsstatistik

### Lernziele
*   Erfolgsquoten nach verschiedenen Kriterien anzeigen.

### Nutzen
*   Die komprimierte Übersicht zum Erfolg von Angeboten erlaubt Ihnen einen schnellen Eindruck.
*   Durch eine detaillierte Darstellung der Erfolgsquote von Angeboten können Sie analysieren, wo die Schwerpunkte zur Akquise in der Zukunft liegen sollten.

### Merke
| Begriff | Beschreibung |
| :--- | :--- |
| **Erfolg** | Ein Angebot ist dann erfolgreich gewesen, wenn aus ihm ein Auftrag erzeugt wurde. |
| **Auswertung** | Die Auswertung kann sich auf verschiedene Kriterien beziehen. |
| **Kategorie** | Beim Ablehnen eines Angebots kann ein Ablehnungsgrund erfasst werden. Diese Gründe können als Kategorie zur Auswertung herangezogen werden. |
| **Voreinstellungen** | Keine |

## Erfolgsquote
Über die Angebotsstatistik können Sie analysieren, wie viele aktuelle und/oder archivierte Angebote in Aufträge umgewandelt wurden. Durch die Kategorie kann ein Angebot nach verschiedenen Ablehnungsgründen klassifiziert werden. Die Kategorien legen Sie selbst fest, z. B. zu teuer, keine Rückmeldung.

Folgende Daten werden ausgewiesen:
*   Anzahl der Angebote pro Kunde
*   Anzahl der aus den Angeboten entstandenen Aufträge
*   Gesamtbruttobetrag über die Summe der Angebote
*   Gesamtbruttobetrag über die Summe der Aufträge
*   Erfolgsquote in Prozent für Anzahl und Betrag

Damit haben Sie aussagekräftige Werte zur Verfügung, anhand derer Sie z. B. notwendige Korrekturen einleiten können.

## Angebote auswerten
In dieser Einheit lernen Sie, wie Sie den Erfolg Ihrer Angebote feststellen.

### So stellen Sie die Erfolgsquote pro Kunde fest
1. Wählen Sie `Dokumente > Angebot > Angebotsstatistik`.
2. Wählen Sie ggf. den Auswahlmodus.

**Abb. C-208 Erfolgsquote für einen Kunden prüfen**
*   **A**: Erfassungszeitraum
*   **B**: Kategorie
*   **C**: Archiv
*   **D**: Detailauswahl

3. Legen Sie den Erfassungszeitraum (A) fest und tragen Sie die Kundennummer ein.
4. Markieren Sie die Kategorie (B), nach der ausgewertet werden soll.
5. Markieren Sie ggf. das Archiv (C), wenn die Angebote bereits archiviert sind.
6. Markieren Sie ggf. die Checkbox `Detailauswertung` (D), um die Angebote einzeln aufzuführen.
7. Wählen Sie im Menü `Start > Suchen`, um in die Suche zu starten.

**Abb. C-209 Detailauswertung zu einem Kunden**
*   **A**: Anzahl der ausgewerteten Angebote
*   **B**: Anzahl der Aufträge aus den Angeboten
*   **C**: Erfolgsquote nach Anzahl
*   **D**: Erfolgsquote nach Umsatz

Die Angebote werden je nach Auswertungskriterien als Summe oder mit Details angezeigt.

## Übungen

### Erfolgsquote prüfen
Stellen Sie fest, wie erfolgreich Ihre Angebote in Aufträge überführt wurden.
*   Wählen Sie als Zeitraum die Schulungstage, in denen Angebote und Aufträge erfasst haben.

### Ergänzende Informationen
⇨ Softwarereferenz, "Kategorie" auf Seite C-394
⇨ Softwarereferenz, "Angebotsstatistik" auf Seite C-397

# Datenübergabe

## Datenübergabe
In diesem Themenblock lernen Sie, wie Sie Daten über Schnittstellen weiterleiten.

Dazu gehören folgende Lerneinheiten:
*   "Finanzbuchhaltung (FiBu)" auf Seite C-354
*   "Statistikübergabe" auf Seite C-363
*   "Archivierung" auf Seite C-369

## Finanzbuchhaltung (FiBu)

### Lernziele
*   Einstellungen für den Datenaustausch mit einem Programm zur Finanzbuchhaltung.
*   Daten übertragen.
*   Offene Posten abfragen.

### Nutzen
*   A+W Business kann mit verschiedenen FiBu-Programmen kommunizieren, an die Sie die Rechnungen übergeben können.
*   Rechnungen und Gutschriften können Sie per Datenübergabe weiterleiten.
*   Offene Posten zu Kundenrechnungen werden von einigen Programmen zurückgemeldet, so dass Sie evtl. Mahnungen schreiben oder einen säumigen Kunden sperren können.

### Merke
| Begriff | Beschreibung |
| :--- | :--- |
| **Finanzbuchhaltung** | A+W Business stellt Schnittstellen zu Programmen zur Finanzbuchhaltung (FiBu) zur Verfügung. |
| **Automatische Datenübergabe** | Nur wenn Sie mit der SQL-FiBu Syska arbeiten, kann die Datenübergabe automatisch gestartet werden. |
| **Erlöskonten** | In A+W Business werden die Erlöskonten der FiBu den Warengruppen zugeordnet. |
| **Datenübergabe** | Die Daten werden in eine Übertragungsdatei geschrieben. Die Auswahl der Daten, die übergeben werden sollen, kann angepasst werden. |
| **Offene Posten** | Die Abfrage von offenen Posten (OP-Abfrage) funktioniert nur mit der SQL-FiBu Syska. Das Ergebnis der Abfrage listet alle offenen Rechnungen mit ausstehenden Summen, Mahndatum und Mahnstufe auf. |
| **Buchungskreise** | Wenn Sie im eingesetzten FiBu-Programm Buchungskreise für Ihre Mandanten definiert haben, können Sie die FiBu der einzelnen Mandanten gesondert pflegen. |
| **Voreinstellungen** | **Stammdaten:** Statuszuordnung, Nummernkreise, Finanzen. **Firmendaten:** Register FiBu. **Utilities:** Debitoren/Kreditoren an FIBU, Offene Posten. |

## Datenübergabe
A+W Business stellt Schnittstellen zur Verfügung, mit denen Rechnungen und Gutschriften an Programme zur Finanzbuchhaltung (FiBu) übergeben werden können.
Die Daten werden über einen Nummernverwalter an die FiBu übergeben. Nur wenn Sie mit der FiBu Syska arbeiten, kann die Datenübergabe automatisch gestartet werden.

> **Automatische Datenübergabe**
> Die Datenübergabe kann automatisiert werden. Dazu gibt es verschiedene Möglichkeiten, z. B. Workflow-Tasks. Von Ihrer Systemkonfiguration hängt ab, welche Möglichkeit Sie nutzen können. Sollten Sie hierzu Fragen haben, wenden Sie sich bitte an Ihren Service-Mitarbeiter bei der A+W Software GmbH.

Die Übergabe von Rechnungen an das FiBu-Programm wird in der Regel manuell ausgelöst. Die Daten werden für alle Rechnungen nach den gleichen Kriterien übergeben.

Die Dokumente werden in zwei Stufen analysiert und gruppiert:
*   Die erste Stufe fasst alle Positionen und Stücklisten-Komponenten nach ihrer Kombi-Warengruppe für die Statistik zusammen.
*   Die zweite Stufe gruppiert das Ergebnis noch einmal. Dabei wird das entsprechende Erlöskonto gesucht. Schlüssel der Suche sind die Warengruppe, die MwSt. 1, die MwSt. 2 und die Geschäftsart des Dokuments. Fehlt ein solcher Schlüssel, wird ein Dialog geöffnet, in dem das Erlöskonto eingetragen werden kann.

Wenn ein Schlüssel mit einem leeren Eintrag für das Erlöskonto vorhanden ist, wird dieses leere Erlöskonto in die Ausgabedatei geschrieben.

Sonderrabatte und Zuschläge mit der Produktart Leistungen und Zuschläge, die in Warengruppe 000 laufen, werden nicht übergeben, sondern auf die betreffenden Positionen oder Stücklisten-Komponenten (zurück) verteilt.

## Statuszuordnung
In der Statuszuordnung geben Sie an, welchen Mindeststatus das Dokument haben muss, um die FiBu-Übergabe machen zu können.

**Abb. C-210 Beispiel Status für FiBu-Übergabe**

Damit das Dokument kein zweites Mal in die FiBu übergeben wird, muss außerdem ein Sperrstatus definiert werden.

## Tagesabschluss
Rechnungen können z. B. einmal pro Tag in einem nächtlichen Batchlauf an die FiBu übergeben werden. In der Regel werden die Dokumente bei der Übergabe an die FiBu (automatisch) sowohl ans Archiv als auch an die Statistik übergeben.

Für die automatische Übergabe sind folgende Einstellungen erforderlich:
*   Buchungsperioden
*   Pfade für die Import- und Export-Datei
*   Workflow-Task für den A+W Business 6 Interface Service
*   Übergabe-Intervall oder -Zeitpunkt

## Buchungsperioden
Die Buchungsperioden werden bei der Übergabe an das FiBu-Programm geprüft. Wenn das eingetragene Datum erreicht ist, kann kein Dokument mehr in diese Buchungsperiode übergeben werden.

**Abb. C-211 Buchungsperioden**

Wenn ein Dokument zwischen dem Datum der ersten und dem Datum der nächsten Buchungsperiode liegt, prüft A+W Business, welches der beiden dem Datum des Dokuments am nächsten ist.

## Datenübergabedatei
Die Daten werden in eine Übertragungsdatei geschrieben. Mit verschiedenen Optionen können Sie die Datenübergabe anpassen, z. B.:
*   Ausgabedatei
*   Rechnungen nur mit Wert über 0
*   Automatische Sortierung
*   Steuerkennzeichen separat verarbeiten

Standardmäßig wird die Kundennummer als Kontonummer herangezogen. Wenn im Dokument eine vom Kunden abweichende Rechnungsanschrift eingetragen ist, wird diese als Kontonummer herangezogen. In den Stammdaten des Kunden kann aber auch eine Debitorennummer hinterlegt werden, die dann als Kontonummer übergeben werden kann.

An viele FiBu-Programme kann ein beliebiger Buchungstext übergeben werden. In der Regel ist dies die Rechnungs- oder Kundenanschrift in der Form Name, Straße, Postleitzahl und Ort.

## Erlöskonten
Für jede Warengruppe und jedes MwSt.-Kennzeichen richten Sie ein Erlöskonto ein. Damit die Produktumsätze auf das richtige Konto gebucht werden, ordnen Sie den Warengruppen die Erlöskonten zu.

Außerdem können Sie jeder Warengruppe ein oder mehrere Mehrwertsteuer-kennzeichen zuweisen und so auch die Geschäfte mit Ihren ausländischen Kunden ohne Mehraufwand abwickeln und auswerten.

**Abb. C-212 Erlöskontenverwaltung**

*   **Debitor (Kunde):**
    In den Feldern Rechnung und Gutschrift tragen Sie die Erlöskonten für die Rechnungen und Gutschriften der Kundenaufträge ein. Auch die Mehrwertsteuer wird auf dieses Erlöskonto gebucht, wenn nicht unter `Stammdaten > Finanzen > MwSt.` ein anderes Erlöskonto für das Mehrwertsteuer-Kennzeichen eingetragen wird.
*   **Kreditor (Lieferant):**
    In den Feldern Rechnung und Gutschrift tragen Sie die Erlöskonten für die Rechnungen und Gutschriften der Lieferantenbestellungen ein. Siehe auch Erläuterungen zu Debitor.

### Beispiel
**Ausgangsdaten:**
*   2 Warengruppen: 5** und 6**
*   2 MwSt.-Kennzeichen 1: 1 und 2
*   1 MwSt.-Kennzeichen 2: = 1
*   MwSt.-Zusammenstellungen:
    *   MwSt. 1: 1, MwSt. 2: 0
    *   MwSt. 1: 2, MwSt. 2: 0
    *   MwSt. 1: 2, MwSt. 2: 1
*   2 Geschäftsarten: Streckengeschäft und Handelsgeschäft

Folgende Erlöskonten müssen angelegt werden:

**Tab. C-6 Beispiel Erlöskonten**

| WGR | MwSt.-Kz. 1 | MwSt.-Kz. 2 | Geschäftsart |
| :-- | :-- | :-- | :--- |
| 5** | 1 | 0 | Streckengeschäft |
| 5** | 2 | 0 | Streckengeschäft |
| 5** | 2 | 1 | Streckengeschäft |
| 6** | 1 | 0 | Streckengeschäft |
| 6** | 2 | 0 | Streckengeschäft |
| 6** | 2 | 1 | Streckengeschäft |
| 5** | 1 | 0 | Handelsgeschäft |
| 5** | 2 | 0 | Handelsgeschäft |
| 5** | 2 | 1 | Handelsgeschäft |
| 6** | 1 | 0 | Handelsgeschäft |
| 6** | 2 | 0 | Handelsgeschäft |
| 6** | 2 | 1 | Handelsgeschäft |

## Offene Posten (OP)
Über die OP-Rückmeldung werden alle offenen Rechnungen mit Angabe der ausstehenden Summe, Mahndatum und Mahnstufe gemeldet.

**Abb. C-213 Anzeige der offenen Posten**

Mit dem Modul `Mahnwesen` können Sie bezahlte Rechnungen in A+W Business manuell verbuchen. Die Summe der offenen Posten wird automatisch um diese gebuchten Beträge und unter Einbeziehung der abgezogenen Skontobeträge reduziert. Dabei kann es sich sowohl um Gesamt- als auch Teilrechnungsbeträge einschließlich Skonto handeln.

Pro Rechnungseintrag wird ausgewiesen, welchen Gesamtbetrag der Kunde zu zahlen hat, welche Zahlungen (inklusive Teilbeträge) er bereits geleistet hat und welcher Betrag von dieser Rechnung noch offen steht. Die Summe wird in der Auftragserfassung angezeigt und ermöglicht die zeitnahe Entscheidung in "kritischen" Fällen.

## Rechnungen an die FiBu übergeben
In dieser Einheit lernen Sie, wie Sie Rechnungen an die FiBu übergeben.

### So übergeben Sie Rechnungen an die FiBu
1. Sammeln Sie alle Aufträge bzw. deren Rechnungen, die übergeben werden sollen, in einem Nummernverwalter.
2. Wählen Sie `Dokumente > Auftrag > FIBU-Übergabe`. Der Dialog `Sollstellung FIBU` wird geöffnet.
3. Wählen Sie den Nummernverwalter aus, in dem Sie die Rechnungen zusammengestellt haben.

**Abb. C-214 Rechnungen zur Übergabe an die FiBu bereit**

Die Rechnungen werden in der Übersicht angezeigt.
4. Prüfen Sie die Einstellungen im Menü `Optionen`, z. B., ob Rechnungen mit einem Betrag gleich 0 übergeben werden sollen.
5. Wählen Sie ggf. den Mandanten und den Bereich.
6. Wählen Sie im Menü `Start > Ausführen`, um die Daten zu übergeben. Die Daten werden übergeben.
7. Bestätigen Sie die Meldung zur Übergabedatei. Sie können die Datei in einem Editor prüfen, bevor Sie sie an das Buchhaltungsbüro weitergeben.

**Abb. C-215 Rechnungen sind übergeben**
*   **A**: Neuer Status
*   **B**: Anzahl der übergebenen Aufträge und Positionen

Im Dialog `Sollstellung FIBU` werden die Anzeigefelder aktualisiert und der Status der Rechnungen umgesetzt. Damit können die Rechnungen nicht nochmals übergeben werden.

### Ergänzende Informationen
⇨ Stammdaten, "Erlöskonten" auf Seite B-910
⇨ Stammdaten, "Update OP-Saldo nach Übergabe" auf Seite B-926
⇨ Stammdaten, "Firmendaten - FiBu" auf Seite B-924
⇨ Stammdaten, "Erlöskonten" auf Seite B-910
⇨ Stammdaten, "Schnittstellen-Dienst" auf Seite B-1032

## Statistikübergabe

### Lernziele
*   Dokumente manuell übergeben.
*   Automatische Übergabe einrichten.

### Nutzen
*   Alle Dokumente können nach verschiedenen Kriterien statistisch ausgewertet werden.
*   Sie können die Übergabe der Dokumente an die Statistik automatisieren und individuell einrichten.

### Merke
| Begriff | Beschreibung |
| :--- | :--- |
| **Vorhaltetage** | Vorhaltetage legen eine Zeitspanne fest, in der Daten in der Hauptdatenbank gespeichert bleiben. |
| **Statistik** | Dokumente können separat übergeben werden für: <ul><li>Provisionsstatistik</li><li>Umsatzstatistik</li></ul> |
| **Voreinstellungen** | **Stammdaten:** Top-WGR. **Firmendaten:** Register Archiv, Register Tagesabschluss. **Utilities:** Statistik-Update |

## Berichte
Mit dem Modul `Statistik` stellt A+W Business eine Reihe von Berichten (Reports) zur Verfügung. Dazu werden die Dokumente an die Statistik übergeben. Für jede Dokumentenart legen Sie fest, ob und wann das entsprechende Dokument übergeben werden soll.

Die Dokumente werden gleichzeitig an die Statistik und ans Archiv übergeben. Für die Statistik werden bestimmte Auftragsdaten in eine eigene Tabelle in der Hauptdatenbank geschrieben. Anhand hinterlegter Fristen (Vorhaltetage) prüft das System, wie lange diese in der Hauptdatenbank gespeichert bleiben sollen, bis sie automatisch gelöscht werden.

Dabei werden alle Daten aus der Hauptdatenbank gelöscht, die älter sind als die eingetragenen Fristen. Die Fristen bestimmen Sie pro Dokumentenart selbst.

> **Beispiel**
> Wenn Sie Jahresübersichten erzeugen wollen, sollten Sie einen langen Zeitraum eintragen, um einen ausreichenden Spielraum für die Erstellung der Auswertung zu haben.
> Für die Provisionsstatistik ist der Rhythmus ausschlaggebend, in dem Sie Provisionen abrechnen.

Mit der Übergabe an die Statistik wird der Status der Dokumente umgesetzt. Ein Beispiel für die Statusumsetzung finden Sie in der Lerneinheit zum Status:
⇨ "Automatische Statusvergabe" auf Seite C-234

## Tagesabschluss
Standardmäßig ist für die Übergabe an die Statistik der Monat des Dokumentendatums ausschlaggebend, für die Archivierung das Jahr. Nach der Archivierung sollten die Dokumente gelöscht werden, um die Hauptdatenbank so klein wie möglich zu halten.

In der Regel werden die Dokumente bei der Übergabe an die FiBu (automatisch) sowohl ans Archiv als auch an die Statistik übergeben.

## Aufträge an die Statistik übergeben
In dieser Einheit lernen Sie, wie Sie Aufträge manuell an die Statistik übergeben.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So richten Sie die Übergabe an die Statistik ein" auf Seite C-365
*   "So übergeben Sie Aufträge ans Archiv" auf Seite C-373

### So richten Sie die Übergabe an die Statistik ein
1. Wählen Sie `Stammdaten > Firma > Firmendaten > Register Archiv`.

**Abb. C-216 Einstellungen für die Übergabe an die Statistik**
*   **A**: Details zur Archivierung
*   **B**: Auswahl der Automatikoptionen
*   **C**: Dokumententyp

2. Wählen Sie den Dokumententyp (C) aus.
3. Markieren Sie die Checkboxen (B) `Übergabe Provisionsstatistik` und/oder `Übergabe Umsatzstatistik`.
4. Markieren Sie die Checkboxen (A), mit denen Sie die Details der Statistik festlegen können, z. B. den `Export in die Superstatistik`.
5. Klicken Sie auf [Speichern], um die Daten zu speichern.
6. Die Einstellungen werden für den gewählten Dokumententyp gespeichert.
7. Wiederholen Sie die Schritte n bis n für alle Dokumententypen, die Sie an die Statistik übergeben wollen.
8. Wechseln Sie zum Register `Tagesabschluss` und prüfen Sie die Angaben für die Vorhaltetage.
   Mit diesen Einstellungen legen Sie fest, wie lange die Dokumente in der Hauptdatenbank gespeichert bleiben sollen, bis sie automatisch und endgültig gelöscht werden.
9. Klicken Sie auf [Speichern], um die Änderungen zu speichern. Die Einstellungen werden gespeichert.

### So übergeben Sie Aufträge an die Statistik
1. Sammeln Sie alle Aufträge, die übergeben werden sollen, in einem Nummernverwalter.
2. Wählen Sie `Dokumente > Auftrag > Übergabe Archiv`.

**Abb. C-217 Aufträge zur Übergabe an die Statistik bereit**
*   **A**: Löschen
*   **B**: Nummernverwalter
*   **C**: Übergabe an
*   **D**: Archivjahr
*   **E**: Archivmonat

3. Wählen Sie den Nummernverwalter aus (B), in dem Sie die Aufträge zusammengestellt haben. Die Übersicht der Aufträge wird aktualisiert.
4. Wählen Sie ggf. den Mandanten.
5. Markieren Sie die Checkboxen (C) `Provisionsstatistik` und/oder `Umsatzstatistik`.
6. Geben Sie das Statistikjahr (D) und den -monat (E) an, z. B. 2011 und 12.
7. Markieren Sie die Checkboxen `Archiv` und `Löschen` (A) nur, wenn Sie die Aufträge gleichzeitig archivieren und aus der Hauptdatenbank löschen wollen.
8. Klicken Sie auf [Ausführen], um die Übergabe zu starten. Die Daten werden übergeben.

**Abb. C-218 Aufträge sind übergeben**

Der Status der Aufträge ist umgesetzt. Sie können jetzt im Modul Statistik die Auswertungen starten.

### Ergänzende Informationen
⇨ Stammdaten, "Firmendaten - Archiv" auf Seite B-965
⇨ Stammdaten, "Firmendaten - Tagesabschluss" auf Seite B-972

## Archivierung

### Lernziele
*   Unterschiede zwischen Haupt- und Archivdatenbank kennenlernen.
*   Vorgaben für Archivierung einstellen.
*   Dokumente manuell archivieren.

### Nutzen
*   Sie pflegen die Hauptdatenbank, indem Sie alte Aufträge archivieren.
*   Mit der Archivierung und der gleichzeitigen Löschung bleibt die Performance der Hauptdatenbank erhalten.

### Merke
| Begriff | Beschreibung |
| :--- | :--- |
| **Dokumente** | Folgende Dokumente können archiviert werden: Angebote, Aufträge, Gutschriften, Anfragen, Bestellungen. |
| **Archivjahr** | A+W Business kann mehrere Archivjahre verwalten. Bei bestimmten Aktionen kann das Archiv ausgewählt werden, z. B. beim Kopieren von Dokumenten. |
| **Datenbanken** | Die aktuellen Daten werden in A+W Business in der Hauptdatenbank verwaltet. Daneben bestehen unabhängige Datenbanken für die Archive. Diese werden i. d. R. pro Kalenderjahr angelegt. |
| **Voreinstellungen** | **Firmendaten:** Register Archiv, Register Parameter (Vertreterprovisionierung), Register Tagesabschluss (Archivpfad). |

## Abgeschlossene Dokumente
Abgeschlossene Geschäftsvorgänge bleiben für eine von Ihnen definierte Zeit in der Hauptdatenbank und werden dann automatisch archiviert. Alle Dokumentendaten werden unverändert gespeichert. Sie können als Kopie aus dem Archiv geholt werden.

Die Dokumente werden gleichzeitig an das Archiv und die Statistik übergeben und anschließend standardmäßig aus der Hauptdatenbank gelöscht. Nach der Übergabe der Daten ans Archiv wird die Hauptdatenbank reindiziert, um die gewohnte Verarbeitungsgeschwindigkeit wieder herzustellen.

Da die Archivierung sehr rechenintensiv ist, erfolgt sie allabendlich und vollautomatisch.

### Archive
Die Archive bilden eigene Datenbanken, die jeweils ein Jahr zusammenfassen. Beim Jahreswechsel archiviert das System die Dokumente in Abhängigkeit vom Rechnungsdatum im entsprechenden Archiv.

Archivierte Dokumente können jederzeit zurück in die Hauptdatenbank kopiert werden.

### Mehrfach archivieren
Wurde ein archiviertes Dokument in die Hauptdatenbank zurückkopiert, kann es nur dann erneut archiviert werden, wenn die Mehrfach-Archivierung in den Firmendaten aktiviert ist.

Wenn die Mehrfach-Archivierung nicht zugelassen ist, muss das Dokument entweder in der Hauptdatenbank bleiben oder sein Status muss manuell hochgesetzt werden, damit es gelöscht werden kann.

### Automatische Archivierung
In der Regel werden die Dokumente automatisch archiviert und anschließend gelöscht. In den Firmendaten können dazu der Mindeststatus und das Alter der Dokumente festgelegt werden.

### Manuelle Archivierung
Zur manuellen Archivierung werden alle Dokumente, die ans Archiv (und/oder an die Statistik) übergeben werden sollen, in den Nummernverwalter gestellt.
Mit der Funktion `Übergabe Archiv` werden alle Dokumente eines Nummernverwalters übergeben.

### Referenzprüfung
Wenn die Referenzen beim Löschen von Dokumenten durch die Archivierung geprüft werden, wird auch geprüft, ob alle referenzierten Dokumente eines Auftrags bereits archiviert sind, z. B. Teillieferungen, Reklamationen. Erst danach ist es möglich, den Auftrag zu löschen.

## Auftrag ohne Rechnung
Wenn zu einem Auftrag kein Rechnungsdatum vorhanden ist, kann er nur archiviert werden, wenn der Status größer als `Rechnungs-Original gedruckt` und kleiner als `Datenübergabe an Archiv` ist. Dann wird davon ausgegangen, dass keine Rechnung mehr geschrieben werden soll und das Archivjahr wird durch das Erfassungsdatum bestimmt.

## Dokumente archivieren
In dieser Einheit lernen Sie, wie Sie Dokumente manuell archivieren.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So richten Sie die Übergabe ans Archiv ein" auf Seite C-371
*   "So übergeben Sie Aufträge ans Archiv" auf Seite C-373

### So richten Sie die Übergabe ans Archiv ein
1. Wählen Sie `Stammdaten > Firma > Firmendaten > Register Archiv`.

**Abb. C-219 Einstellungen für die Übergabe an die Statistik**
*   **A**: Details zur Archivierung
*   **B**: Auswahl der Automatikoptionen
*   **C**: Archivierungsmodus
*   **D**: Dokumententyp

2. Wählen Sie den Dokumententyp (D) aus.
3. Markieren Sie die Checkboxen (B) `Übergabe Archiv` und/oder `Dokument löschen`.
4. Wählen Sie den Modus (B) für die Archivierung.
    *   **Mindeststatus:** Status, ab die Dokumente automatische archiviert werden.
    *   **Dokument älter als X Tage:** Anzahl der Tage, die nach dem Erfassungsdatum verstrichen sein müssen, bevor das Dokument archiviert wird. Bei dieser Einstellung müssen Sie auch die `Übergabe nach Erfassungsdatum` (A) aktivieren. Dieser Wert bietet sich beispielsweise an, wenn eine Reklamationsfrist abgewartet werden soll.
    *   **Status + Dokument älter als:** Bei diesen Einstellungen müssen beide Kriterien erfüllt sein: Der entsprechende Status muss erreicht sein und das Dokument muss das eingetragene Alter erreicht haben.
5. Markieren Sie die Checkboxen (A), mit denen Sie die Details für die Archivierung festlegen können, z. B. die Übergabe nach Erfassungsdatum.
6. Klicken Sie auf [Speichern], um die Daten zu speichern.
7. Die Einstellungen werden für den gewählten Dokumententyp gespeichert.
8. Wiederholen Sie die Schritte 2 bis 6 für alle Dokumententypen, die Sie an das Archiv übergeben wollen.

### So übergeben Sie Aufträge ans Archiv
1. Sammeln Sie alle Aufträge, die übergeben werden sollen, in einem Nummernverwalter.
2. Wählen Sie `Dokumente > Auftrag > Übergabe Archiv`.

**Abb. C-220 Aufträge zur Übergabe ans Archiv bereit**
*   **A**: Löschen
*   **B**: Nummernverwalter
*   **C**: Übergabe an Statistik und Archiv

3. Wählen Sie den Nummernverwalter aus (B), in dem Sie die Aufträge zusammengestellt haben. Die Übersicht der Aufträge wird aktualisiert.
4. Wählen Sie ggf. den Mandanten.
5. Markieren Sie die Checkboxen (C) `Archiv` und/oder `Löschen` (A).
6. Markieren Sie die Checkboxen `Provisionsstatistik` und `Umsatzstatistik` nur, wenn Sie die Aufträge gleichzeitig an die Statistik übergeben wollen. In diesem Fall müssen Sie das Statistikjahr und den -monat angeben, z. B. 2011 und 12.
7. Wählen Sie im Menü `Start > Ausführen`, um die Aktion zu starten. Die Daten werden je nach den Einstellungen in den Firmendaten übergeben. Wenn die Archivierung das Rechnungsdatum abfragt, werden nur die Aufträge archiviert, zu denen eine Rechnung erstellt wurde.

**Abb. C-221 Aufträge sind übergeben**

Der Status der Aufträge wird umgesetzt. Dokumente, deren Status eine Archivierung nicht zuließ, werden gekennzeichnet.

## Übungen

### Rechnung an die FiBu übergeben
Übergeben Sie alle Rechnungen in Ihrem Nummernverwalter an die FiBu.
Wiederholen Sie die Übergabe, indem Sie die Rechnungen an die Statistik übergeben und anschließend archivieren.

### Ergänzende Informationen
⇨ Softwarereferenz, "Nummernverwalter" auf Seite C-631
⇨ Softwarereferenz, “Sollstellung FiBu" auf Seite C-682
⇨ Softwarereferenz, "Übergabe Archiv" auf Seite C-686
⇨ Stammdaten, "Firmendaten - Archiv" auf Seite B-965
⇨ Stammdaten, "Dokument ohne Referenzprüfung löschen" auf Seite B-967
⇨ Stammdaten, "Mehrfach-Archivierung" auf Seite B-968

# Zusatzfunktionen

## Zusatzfunktionen
In diesem Abschnitt finden Sie zusätzliche Informationen zur Arbeitsweise und zu den Funktionen in A+W Business.
*   "Import von Dokumenten" auf Seite C-377
*   "Bestandslisten" auf Seite C-383
*   "Journal" auf Seite C-384
*   "Dokumentenüberwachung" auf Seite C-386

## Import von Dokumenten
Über die EDI-Schnittstellen können Sie Kundenaufträge importieren und in A+W Business bearbeiten.

### Stammdaten für den Import
Für eingehende Kundenaufträge läuft ein automatisierter Import (Batch-File), der in regelmäßigen Abständen in den entsprechenden Verzeichnissen nach eingegangenen Aufträgen sucht und diese in die A+W Business-Auftragsbearbeitung integriert. Sie können den Import auch manuell starten.

Aus den übernommenen Daten werden Aufträge für Rechteckscheiben inklusive Sprossen in A+W Business automatisch generiert.
⇨ Softwarereferenz, "Import" auf Seite C-688

Dazu müssen die Stammdaten beim Kunden und in A+W Business identisch angelegt sein.

**Beispiel: Identische Stammdaten für den Import**

| Sender (Kunde) | Empfänger (A+W Business) |
| :--- | :--- |
| 500124 --> | `1004 Float 4 mm`, `105012 SZR 12 mm`, `1004 Float 4 mm` |
| 500124 --> 105016 SZR 16 mm --> 500124 --> | `1004 Float 4 mm`, `105016 SZR 16 mm`, `1004 Float 4 mm` |

In diesem Beispiel sehen Sie, dass das Produkt 500124 eine ISO-Scheibe mit Float 4 mm Gläsern und dem SZR mit 12 mm ist.
Im zweiten Beispiel ist der SZR durch das Produkt 105016 ersetzt.

Wenn sich die Stammdaten Ihres Kunden von Ihren eigenen unterscheiden, ist der Import mit Hilfe von Referenzierungstabellen möglich. Die integrierte Referenzierung wandelt die Kundendaten in A+W Business-Daten um.

**Beispiel: Umsetzen von Kundenartikeln in Stammdaten**

| Sender (Kunde) | Empfänger (A+W Business) |
| :--- | :--- |
| ISO416 --> `20004 Float 4 mm`, `4016 SZR 16 mm`, `40004 Ornament 4 mm` | --> 500124 --> `1004 Float 4 mm`, `105016 SZR 12 mm`, `1804 Ornament 4 mm` |

In diesem Beispiel wird aus dem alphanumerischen Kunden-Artikelnummer `ISO416` die numerische A+W Business-Produktnummer 500124.

Mit dem Zusatz-Modul `Connect II` können Sie auch Standard-Modelle importieren.

**Beispiel: Umsetzen von Kundenauftrag mit Modell in Stammdaten**

| Sender (Kunde) | Empfänger (A+W Business) |
| :--- | :--- |
| ISO416 --> `20004 Float 4 mm`, `4016 SZR 16 mm`, `40004 Ornament 4 mm`, `110145 Modell 3` | --> 500124 --> `1004 Float 4 mm`, `105016 SZR 12 mm`, `1804 Ornament 4 mm`, `8003 Modell 3` |

In diesem Beispiel wird aus dem Kunden-Modell 110415 die A+W Business-Produktnummer 8003. Beide bezeichnen das Modell 3.

Wenn ein importierter Auftrag das Kreditlimit des Kunden überschreitet, kann der Auftrag mit einem entsprechenden Status gespeichert werden.

### Ergänzende Informationen
⇨ Softwarereferenz, "Import" auf Seite C-688

## Dokumente importieren
In dieser Einheit lernen Sie, wie Sie Kundenaufträge direkt über die EDI-Schnittstelle an A+W Business übergeben. Die Aufträge können manuell oder automatisch importiert werden.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So legen Sie die Einstellungen zum automatischen Import fest" auf Seite C-379
*   "So importieren Sie einen Kundenauftrag manuell" auf Seite C-381
*   "So beheben Sie einen Fehler in der importierten Datei" auf Seite C-382

> **Voraussetzung**
> Damit die Daten aus den Kundenaufträgen richtig zugeordnet werden können, müssen die Stammdaten für Kundenreferenzen korrekt angelegt sein.

### So legen Sie die Einstellungen zum automatischen Import fest
1. Wählen Sie `Stammdaten > Firma > Customizing`. Der Dialog `Customizing` wird geöffnet.
   ⇨ Stammdaten, "Customizing" auf Seite B-1042
2. Wechseln Sie zum Register `Programme` und markieren Sie den Eintrag für den EDI-Import.

**Abb. C-222 Programm zum EDI-Import**

3. Wechseln Sie zum Register `Autom. Prozessausführung`.

**Abb. C-223 Einstellungen zur Fremdschnittstelle**
*   **A**: Intervall
*   **B**: Art der Ausführung

4. Wählen Sie die Art der Ausführung (B). Wenn die Dokumente laufend eingelesen werden sollen, müssen Sie die Einstellung zyklisch wählen.
5. Geben Sie den Wert (A) für das Intervall ein, in dem neue Kundenaufträge importiert werden sollen.
6. Wählen Sie im Menü `Start > Speichern`, um die Daten zu speichern. Die Daten werden gespeichert.

### So importieren Sie einen Kundenauftrag manuell
1. Wählen Sie `Dokumente > Auftrag > Import`. Der Dialog `Import Pool` wird geöffnet.
   ⇨ Softwarereferenz, "Import" auf Seite C-688
2. Markieren Sie die Dokumente, die Sie importieren wollen.

**Abb. C-224 Import**

Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf. Nur die Positionen sind markiert, die mit einem X gekennzeichnet sind.
3. Wechseln Sie zum Register `Dokumente erstellen`, um die Ziel-Einstellungen zu prüfen.
4. Wählen Sie im Bereich `Zielnummernverwalter` den Nummernverwalter für diesen Import aus. Im Bereich `Dokumente` werden alle Dokumente im aktuellen Nummernverwalter aufgelistet.
5. Wählen Sie ggf. im Bereich `Parameter` den Mandanten und den AV-Bereich aus, denen die Kundenaufträge zugeordnet werden sollen.
6. Wählen Sie im Menü `Start > Ausführen`, um den Import zu starten. Die Kundenaufträge werden importiert und als A+W Business-Aufträge gespeichert. Wenn ein Fehler zu einem Kundenauftrag gemeldet wird, müssen Sie im den Dialog `Fremddokument` öffnen.

### So beheben Sie einen Fehler in der importierten Datei
1. Klicken Sie im Register `Import Pool` doppelt auf die (EDI-) Datei, um den Dialog `Fremddokumentenverwaltung` zu öffnen.

**Abb. C-225 Import**

In diesem Dialog können Sie die Daten des Kundenauftrags prüfen und ggf. korrigieren, z. B. die Produktnummer.
2. Speichern Sie die Korrekturen. Der Kundenauftrag wird in A+W Business übernommen und automatisch wird ein neuer Auftrag angelegt.

> **Automatischer Import**
> Wenn Sie ein Intervall für den automatischen Import eingestellt haben, brauchen Sie die Kundenaufträge nicht einzeln und manuell zu importieren.

## Bestandslisten
Mit den Bestandslisten können Sie sich einen Überblick über den Dokumentenbestand nach Nummernkreisen oder Warengruppen anzeigen lassen.

Die Listen stellen folgende Daten dar:
*   **Nach Nummernkreis:**
    Die letzte Nummer der bereits gedruckten Liste wird gespeichert. Die nächste Liste führt dann nur die nachfolgenden (neuen) Nummern auf. Auf diese Weise werden keine Dokumente doppelt aufgeführt.
    *   Dokumentennummer, Liefertermin, Fertigungstermin ISO, Kundennummer, Kundenname, Stück, Status, Qm, Lfm, Netto-Betrag, EK, Rohertrag in %
    *   Gesamtsumme
    *   Gesamtsumme ISO
    *   Summe aller AV-Bereiche
    *   Summe aller AV-Bereiche ISO
*   **Nach Warengruppen:**
    Gliederung nach Warengruppen
    *   Kundennummer, Kundenname, Dokumentennummer, Kommission, Stück, Status, Qm ger., Qm tats., Lfm tats., Erfassungsdatum, Lieferdatum, Netto-Betrag, EK
    *   Zwischensumme pro Warengruppen oder Kunde
    *   Gesamtsumme aller Warengruppen oder Kunden

### Ergänzende Informationen
⇨ Softwarereferenz, "Bestandslisten" auf Seite C-728

## Journal
Mit den Journalen zu den verschiedenen Dokumententypen können Sie sich einen Überblick über den Dokumentenbestand verschaffen. Die unterschiedlichen Listen können nach Nummernverwaltern oder nach wählbaren Kriterien erstellt werden.

**Abb. C-226 Journal - Bestandsliste**
⇨ Softwarereferenz, "Eingangs-/Ausgangs-Journal" auf Seite C-725

Die Listen stellen folgende Daten dar:
*   **Bestandsliste:**
    *   bis zu 4 Zeilen pro Dokument
    *   LfNr, Auftragsnummer, Status, Erfassungsdatum, Kundennummer, Kundenname, Stück, Qm, Lfm, Netto-Betrag, EK, Deckungsbeitrag in %
    *   Datum der AB, Brutto-Betrag, MwSt.
    *   Datum und Nummer des Lieferscheins
    *   Datum und Nummer der Rechnung
*   **Ein-/Aus-Liste:**
    *   1 Zeile pro Dokument
    *   LfNr, Auftragsnummer, Status, Erfassungsdatum, Kundennummer, Kundenname, Stück, Gewicht, Qm, Lfm, Netto-Betrag, EK, Deckungsbeitrag in %
*   **Journal:**
    *   2 Zeilen pro Dokument
    *   LfNr, Auftragsnummer, Status, Erfassungsdatum, Kundennummer, Kundenname, Stück, Qm, Lfm, Netto-Betrag, EK, Deckungsbeitrag in %
    *   Datum und Nummer der Rechnung, Brutto-Betrag, MwSt.
*   **Rechnungsliste:**
    *   1 Zeile pro Rechnung/Sammelrechnung
    *   LfNr, Rechnungsnummer, Status, Erfassungsdatum, Kundennummer, Kundenname, Gewicht, Netto-Betrag, MwSt., Brutto-Betrag, EK, Deckungsbeitrag in %
    *   für Sammelrechnungen das Gesamtgewicht der Aufträge
*   **Versandliste:**
    *   4 Zeilen pro Dokument
    *   LfNr, Auftragsnummer, Status, Erfassungsdatum, Kundennummer, Kundenname, Stück, Qm, Lfm, Gewicht, Netto-Betrag
    *   Datum der AB
    *   Datum und Nummer des Lieferscheins
    *   Datum und Nummer der Rechnung
*   **Produktionsliste:**
    *   1 Zeile pro Dokument
    *   LfNr, Rechnungsnummer, Status, Erfassungsdatum, Kundennummer, Kundenname, Stück, Gewicht, Laufnummer, Anzahl Sprossen, Anzahl Modelle

Die Listen schließen mit den Gesamtsummen pro Spalte. Wahlweise können Sie sich Zwischensummen pro Kunde, Rechnung und/oder Vertreter bilden lassen.

## Dokumentenüberwachung
Das Zusatzmodul Dokumentenüberwachung prüft in regelmäßigen Intervallen den gesamten Dokumentenbestand in A+W Business. Diese Funktion kann beispielsweise folgende Kriterien berücksichtigen:
*   Angebote, deren Termin zur Wiedervorlage fällig ist.
*   Aufträge, die das Kunden-Kreditlimit überschritten haben und vorläufig für die Weiterbearbeitung gesperrt werden.
*   Aufträge, die vor einer bestimmbaren Frist den Kunden als Auftragsbestätigung zugestellt wurden.
*   Aufträge mit dem Status zur Produktionsfreigabe, um die Einspruchsfrist auf Basis der versendeten Auftragsbestätigungen einzuhalten.
*   Aufträge, deren Produktionsende-Datum überschritten wurde.
*   Aufträge mit Lieferscheinstatus, für die noch keine Rechnung gedruckt wurde.

Dieses Zusatzmodul wird außerhalb der Anwendung A+W Business gestartet (z. B. `C:/Programme/A+W/A+W/Business/Program/German/abcAutoStatus.exe`).

Die Dokumentenüberwachung startet automatisch. Die Prüfintervalle, die Dokumentenarten und der jeweilige Status (Prüf- und Zielstatus) werden von Ihnen festgelegt.

Das Programm arbeitet im Hintergrund. Werden Dokumente gefunden, die die Prüfkriterien erfüllen, wird automatisch eine entsprechende Meldung angezeigt.

### Automatische Prüfung auf doppelt erfasste Dokumente
A+W Business prüft automatisch während der Erfassung bzw. Bearbeitung eines Dokumentes, ob schon ein anderes Dokument mit dem gleichen Produkt und Produktaufbau und den gleichen Maßen vorhanden ist. Geprüft werden dabei die Angebote und Aufträge in der Hauptdatenbank. Das Archiv wird nicht durchsucht.

> **Voraussetzung**
> In der Statusverwaltung muss der Anwender-Status Duplikat vorhanden angelegt sein. Im Modul Utilities müssen die Kriterien der Überwachung angegeben sein.

Hat das Programm ein Duplikat gefunden, wird das neu erfasste Dokument automatisch gesperrt und eine entsprechende Meldung ausgegeben. Über die Funktion `Duplikate anzeigen` können Sie sich die Duplikate zum aktuellen Dokument auflisten lassen.

Duplikatsprüfungen werden nicht durchgeführt bei Reklamationen, Teillieferungen, Anzahlungen.

Die übergreifenden Duplikatsfilter richten Sie über das Modul `Utilities` ein. Dort legen Sie folgende Details fest:
*   **Erfassungszeitraum in Tagen:** Das ist der Zeitbereich, in dem gesucht werden soll.
*   **Angaben dazu, was als Vergleichskriterium gelten soll,** z. B. Kunde, Hauptprodukt, Produktaufbau, Maße.

# Softwarereferenz

## Übersicht
In der Dokumentenverwaltung können Sie alle Dokumente erfassen und bearbeiten, die im Rahmen des Verkaufs benötigt werden. Das sind Angebote, Aufträge, Lieferungen, Rechnungen, Gutschriften und Reklamationen. Außerdem können Sie in diesem Modul Bestellungen erfassen und bearbeiten.

Dokumente enthalten zwei Gruppen von Daten: Angaben zum Kunden und die Auftragspositionen. Diese Daten werden in unterschiedlichen Dialogen erfasst.

In der Softwarereferenz finden Sie Informationen zu folgenden Themen:
*   Angebot
*   Alternativen
*   Dokumentenverwaltung
*   Positionsdaten
*   Übersichten und Referenzen zu Kopfdaten
*   Übersichten und Referenzen zu Positionen
*   Dokumente kopieren
*   Makros
*   Nummernverwalter
*   Druck
*   Übergabe Bestellungen
*   Auftrag
*   Übergabe, Im-/Export von Dokumenten
*   Auswertungen
*   Interne Kontrolle
*   Gutschrift
*   Journal
*   Bestandslisten
*   Mahnwesen
*   Dokumentendaten
*   Lagersuche

> **Dialoge können von unterschiedlichen Stellen aus geöffnet werden**
> Bitte beachten Sie, dass viele Funktionen zum Thema Verkauf in A+W Business aus unterschiedlichen Dialogen heraus gestartet werden können. In dieser Anleitung werden die entsprechenden Dialoge nur einmal beschrieben.

## Angebot
`Dokumente > Angebot`

Über das Menü `Angebot` erreichen Sie sich folgende Programmpunkte:
*   **NV Angebot:** Die Funktion des Nummernverwalters ist für alle Dokumente gleich. Sie wird am Beispiel `Auftrag` beschrieben.
    ⇨ "Nummernverwalter" auf Seite C-631
*   **Angebot:** In diesem Dialog erfassen und bearbeiten Sie Angebote. Die Erfassung von Dokumenten ist für alle Dokumentenarten gleich. Sie wird am Beispiel `Auftrag` beschrieben.
    ⇨ "Dokument - Kopfdaten" auf Seite C-417
*   **Druck Angebote:** Der Formular- und Etikettendruck ist für alle Dokumente gleich. Er wird am Beispiel `Auftrag` beschrieben.
    ⇨ "Druck" auf Seite C-637
*   **Wiedervorlage:** Mit dieser Funktion lassen Sie sich eine Übersicht über alle Dokumente anzeigen, die mit einem Datum zur Wiedervorlage gekennzeichnet sind.
    ⇨ "Wiedervorlage" auf Seite C-394
*   **Journal:** Der Journaldruck ist für alle Dokumente gleich. Er wird am Beispiel `Auftrag` beschrieben.
    ⇨ "Journal" auf Seite C-725
*   **Übergabe Archiv:** Die Archivübergabe ist für alle Dokumente gleich. Sie wird am Beispiel `Auftrag` beschrieben.
    ⇨ "Übergabe Archiv" auf Seite C-686
*   **Suche:** Die Suche ist für alle Dokumente gleich. Sie wird am Beispiel `Auftrag` beschrieben.
    ⇨ "Dokument suchen" auf Seite C-523
*   **Angebotsstatistik:** In einer Übersicht können Sie sich die Angebote eines selbst gewählten Zeitraums anzeigen lassen.
    ⇨ "Angebotsstatistik" auf Seite C-397
*   **Import:** Mit dieser Funktion werden elektronische Kunden-Aufträge importiert.
    ⇨ "Import" auf Seite C-688

## Angebot (Dokument)
`Dokumente > Angebot > Angebot auswählen`

**Abb. C-227 Angebot**

In diesem Dialog erfassen und bearbeiten Sie Angebote.
Die Felder sind für alle Dokumententypen gleich. Eine ausführliche Beschreibung finden Sie unter:
⇨ "Dokument - Kopfdaten" auf Seite C-417
⇨ "Dokument - Positionen" auf Seite C-451

Für ein Angebot stehen zusätzlich folgende Felder zur Verfügung:

### Kopfdaten - Register Dokumente
**Vorlage** Datum, mit dem das Angebot auf Wiedervorlage gesetzt wird. Wenn der Tag erreicht ist, wird beim Start von A+W Business automatisch eine Meldung angezeigt. Sie können dann entscheiden, ob Sie das Angebot sofort öffnen möchten.
⇨ "Wiedervorlage" auf Seite C-394

### Kopfdaten - Register Zusatz
**Kategorie** Durch die Kategorie kann ein Angebot nach verschiedenen Ablehnungsgründen klassifiziert werden, z. B. zu teuer, keine Rückmeldung. Über die Kategorie können Angebote in der Statistik ausgewertet werden.

### Positionen - Register Zusatz
**Alternative zur Pos.** Sie können festlegen, dass die markierte Position alternativ zu der Position gelten soll, die Sie hier auswählen. Diese Alternative wird nicht im Gesamtpreis berücksichtigt.
Alternativpositionen werden wie alle anderen Positionen erfasst und angezeigt. Im Druck werden sie entsprechend gekennzeichnet.
⇨ Tutorial, "Alternative Position im Angebot erfassen" auf Seite C-331

## Wiedervorlage
`Dokumente > Angebot > Wiedervorlage`

**Abb. C-228 Angebot - Wiedervorlage**

In diesem Dialog lassen Sie sich eine Übersicht über alle Dokumente anzeigen, die mit einem Datum zur Wiedervorlage gekennzeichnet sind.

In den Firmendaten können Sie für die Wiedervorlage eine Frist für Angebote und/oder Aufträge eintragen.
⇨ Tutorial, "Angebotsverfolgung" auf Seite C-342
⇨ Stammdaten, "Firmendaten - System" auf Seite B-974

> **Anzeige zur Wiedervorlage einschränken**
> Die Anzeige der Dokumente in der Wiedervorlage kann durch ein Anwenderrecht auf die vom Anwender erfassten Dokumente eingeschränkt werden. Das kann z. B. dann sinnvoll sein, wenn ein Vertreter nicht die Dokumente der anderen Vertreter in der Wiedervorlage sehen darf.

### Menü Funktionen
*   **Historie:** Öffnet eine Übersicht über die Bearbeitungen und Statusänderungen des Dokuments.
    ⇨ "Historie" auf Seite C-552
*   **Alternativangebotsübersicht:** Öffnet die Liste der Angebotsalternativen zum aktuellen Angebot oder Auftrag.
    ⇨ "Alternativangebotsübersicht" auf Seite C-407

### Menü Optionen
*   **Mitarbeiter und Datum vorblenden:** Der Dialog wird im Auswahlmodus geöffnet. Das aktuelle Tagesdatum und der in A+W Business angemeldete Mitarbeiter sind vorbelegt.
*   **Automatische Benachrichtigung:** Wenn der Termin zur Wiedervorlage eines bestimmten Dokuments erreicht ist, wird eine entsprechende Meldung angezeigt, wenn der Erfasser des Angebots sich anmeldet.

### Dokument
*   **Nummer:** Nummer des Angebots, das auf Wiedervorlage gesetzt ist.
*   **Vorlagedatum, bis:** Zeitraum zum Eingrenzen der Suche nach Wiedervorlagen.
*   **Erfassung:** Datum, an dem das Dokument erfasst wurde, das auf Wiedervorlage gesetzt ist.
*   **Texte:** Eingabefeld für Anmerkungen zum Dokument, z. B. Hinweise auf Ansprechpartner.
*   **AV-Bereich:** AV-Bereich, dem das Dokument zugeordnet ist.
    ⇨ Tutorial, "AV-Bereich" auf Seite C-43
*   **Fachberater:** Name des zuständigen Fachberaters.
*   **Bearbeiter:** Mitarbeiter, der das Dokument erfasst hat.
*   **Vertreter:** Name des zuständigen Vertreters.
*   **Kunde:** Nummer und Name des Kunden.
*   **Betrag brutto, netto:** Beträge des Angebotswerts.
*   **Status:** Status des Dokuments, das auf Wiedervorlage gesetzt ist.
*   **Typ:** Typ des Dokuments, das auf Wiedervorlage gesetzt ist.
*   **Kategorie:** Durch die Kategorie kann ein Angebot nach verschiedenen Ablehnungsgründen klassifiziert werden, z. B. zu teuer, keine Rückmeldung. Über die Kategorie können Angebote in der Statistik ausgewertet werden.

### Neuer Status
*   **Übergabe Archiv:** Für die Übergabe von Dokumenten an das Archiv muss der Status entsprechend gesetzt sein. In der Regel wird der Status automatisch hochgesetzt. Sie können ihn auch manuell hochsetzen.
    *   Der Status des angezeigten Angebots wird nicht hochgesetzt.
    *   Der Status des angezeigten Angebots wird hochgesetzt, das Angebot kann archiviert danach werden.
    ⇨ Tutorial, "Archivierung" auf Seite C-369
*   **Löschfreigabe:** Dokumente sollten aus der Hauptdatenbank gelöscht werden, sobald sie archiviert sind. Sie verhindern damit, dass die Hauptdatenbank zu groß wird. Dieses Feld ist gesperrt, wenn der Status eines markierten Dokuments größer ist als der Lösch-Status, oder wenn das Dokument einen exklusiven Status hat.
    *   Der Status des angezeigten Angebots wird nicht hochgesetzt, das Angebot kann nicht gelöscht werden.
    *   Der Status des angezeigten Angebots wird hochgesetzt, das Angebot kann danach gelöscht werden.
    ⇨ Stammdaten, "Automatikoptionen" auf Seite B-969
*   **Vorlage alle, min:** Sie können die Wiedervorlage in definierten Intervallen anzeigen lassen. Das Feld `min` (Minuten) ist nur freigeschaltet, wenn die Checkbox `alle` markiert ist.
    *   Das Angebot wird nicht automatisch erneut angezeigt. Das Feld `min` ist gesperrt.
    *   Das Angebot wird automatisch im angegebenen Intervall angezeigt. Im Feld `min` kann das Intervall in Minuten angegeben werden. Das Intervall darf nicht kleiner als 5 Minuten sein.

### Tabelle
Liste aller Angebote, die den Auswahlkriterien entsprechen.

## Angebotsstatistik
`Dokumente > Angebot > Angebotsstatistik`

**Abb. C-229 Angebotsstatistik**

In diesem Dialog lassen Sie sich eine Auswertung über die Angebote eines selbst gewählten Zeitraums anzeigen.
⇨ Tutorial, "Angebotsstatistik" auf Seite C-348

### Selektion
*   **Erfassung von, bis:** Zeitraum, aus dem archivierte Angebote angezeigt werden sollen. Es spielt keine Rolle, in welchem der beiden Felder Sie das jüngere Datum eintragen.
*   **Kunde:** Nummer und Name des Kunden.
*   **AV-Bereich:** Auswahl des AV-Bereichs, dem das Dokument zugeordnet ist. ⇨ Stammdaten, "Basistabelle erweitern" auf Seite B-33
*   **Erfasser:** Auswahl des Mitarbeiters, der das Dokument erfasst hat.
*   **Fachberater:** Auswahl des zuständigen Mitarbeiters.
*   **Außendienst:** Auswahl des zuständigen Vertreters.
*   **Kategorie:** Durch die Kategorie kann ein Angebot nach verschiedenen Ablehnungsgründen klassifiziert werden, z. B. zu teuer, keine Rückmeldung. Über die Kategorie können Angebote ausgefiltert werden.
*   **Dokumententyp:** Auswahl des Dokumententyps, dem das Dokument zugeordnet ist.
*   **Branche:** Auswahl der Branche, der das Dokument zugeordnet ist.
*   **Region:** Auswahl der Region, der das Dokument zugeordnet ist.

### Archive
Anzeige aller verfügbaren A+W Business-Archive. Das gewünschte Archiv markieren Sie mit einem einfachen Klick. Wenn Sie erneut auf den markierten Eintrag klicken, wird die Markierung aufgehoben.
Sie können mehrere Archive gleichzeitig markieren und durchsuchen lassen.

### Auswertung Anzahl, Betrag
*   **Angebote:** Anzeige der gefundenen Angebote und deren Gesamtsumme.
*   **In Aufträge überführt:** Anzeige der Angebote, die in Aufträge überführt wurden.
*   **Quote:** Verhältnis der erstellen Angebote zu den daraus entstandenen Aufträgen.
*   **Aufträge:** Anzahl und Gesamtsumme der im gleichen Zeitraum archivierten Aufträge.

### Detailauswertung
Sie können die Anzeige der Spalten über die Tabelleneigenschaften einstellen. Für eine detailliertere Auswertung können Sie sich alle Spalten anzeigen lassen.
*   Nur die Spalten werden angezeigt, die in den Tabelleneigenschaften aktiviert sind.
*   Alle verfügbaren Spalten werden angezeigt.

### Details
Liste der archivierten Angebote, die die Suchkriterien erfüllen.

## Alternativen
`Dokumente > Angebot > Angebot auswählen > Menü Funktionen > Gruppe Dokument > Alternativen`

Sie können ein Angebot insgesamt als Alternative überarbeiten, z. B. um eine ISO-Scheibe mit einer alternativen Kombination von SZR und Gas anzubieten. Sie können auch einen gesamten Auftrag als Alternative überarbeiten, z. B. um Fehler zu bereinigen.
⇨ Tutorial, "Alternativangebot" auf Seite C-329

Die Alternativen zu einem Angebot können Sie sich in einer Übersicht anzeigen lassen.
⇨ "Alternativangebotsübersicht" auf Seite C-407

> **Alternativpositionen**
> Alternative Positionen werden im Angebot als eigene Positionen eingefügt und entsprechend gekennzeichnet.
> ⇨ Tutorial, "So erfassen Sie eine alternative Position" auf Seite C-331

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
*   "Menü Optionen" auf Seite C-399
*   "Menü Funktionen" auf Seite C-400
*   "Alternativen – Original" auf Seite C-401
*   "Alternativen - Alternative" auf Seite C-403
*   "Alternativen - Texte" auf Seite C-404
*   "Alternativen – Bearbeitungen/Modelle” auf Seite C-405
*   "Alternativen - Sprossen" auf Seite C-406

## Menü Optionen
`Dokumente > Angebot > Angebot auswählen > Menü Funktionen > Gruppe Dokument > Alternativen > Menü Optionen`

Folgende Einträge werden im Menü Optionen angezeigt:
*   **Datumsfelder aktualisieren:** Die Datumsfelder werden automatisch aktualisiert, wenn das Alternativangebot gespeichert wird.

## Menü Funktionen
`Dokumente > Angebot > Angebot auswählen > Menü Funktionen > Gruppe Dokument > Alternativen > Menü Funktionen`

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Dialog zu schließen. Folgende Einträge werden angezeigt:
*   **Alternativangebotsübersicht:** Öffnet die Liste der Angebotsalternativen zum aktuellen Angebot. Die Funktion ist nur in Angeboten freigeschaltet.
    ⇨ "Alternativangebotsübersicht" auf Seite C-407
*   **Dokumentendaten:** Öffnet den Dialog Dokumente, um ggf. die Termine und den Status in Aufträgen und Bestellungen zu korrigieren.
    ⇨ "Dokumentendaten" auf Seite C-737
*   **Lagersuche:** Öffnet den Dialog Lagerinfo, um die aktuellen Lagerbestände anzuzeigen.
    ⇨ "Lagerinfo - Lagersuche" auf Seite C-742
