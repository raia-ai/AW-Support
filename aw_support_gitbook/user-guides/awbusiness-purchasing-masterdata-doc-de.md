---
title: "D-AWBusiness-HB_21"
source: "D-AWBusiness-HB_21.pdf"
tags: ["A+W Business", "Purchasing", "Master Data", "Price Lists", "Orders", "Supplier Management", "Goods Receipt", "ERP Software", "Tutorial", "Warehousing"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a tutorial for the purchasing module of the A+W Business software, covering master data setup for purchasing, price list management, document status, and the complete order processing cycle from inquiry to goods receipt."
long_description: "This comprehensive tutorial provides a step-by-step guide to the purchasing functionalities within the A+W Business software. It begins with the configuration of master data essential for purchasing, focusing on the setup and management of price lists. The document details the flexible, component-based price calculation system, including the hierarchy of price application from manual entries to general agreements. It then explains how to check and manage price master data. The tutorial moves on to document status management, explaining how statuses are assigned and updated for referenced documents like purchase orders linked to sales orders. A major section is dedicated to the creation and management of purchase orders, differentiating between automated handovers from sales orders and manual creation. This includes handling order items, selecting suppliers, managing changes, and processing supplier confirmations. The guide also covers delivery date control, generating inquiries to suppliers, and handling collective orders. The final part of the tutorial focuses on deliveries and goods receipt, explaining how to record incoming goods, manage partial deliveries, handle excess quantities, and process deliveries of special items like crates. It provides instructions for checking default settings and controlling the entire goods receipt process to ensure data accuracy in inventory and related documents."
---

---
## Stammdaten für den Einkauf

### Preislisten

Die Preisberechnung in A+W Business ist aus flexiblen Bausteinen zusammengesetzt, die alle Berechnungsmöglichkeiten abdecken. Sie können jedem Produkt die passende Art der Preisberechnung zuordnen.

Preisjahrgänge, -schlüssel und Tarife bilden den Rahmen für die Preislisten. In den Preistabellen selbst sind die Beträge hinterlegt, die in den Dokumenten herangezogen werden.

Preise legen Sie als Standard-Preislisten oder als Preislisten für bestimmte Kunden- oder Lieferantengruppen, für einzelne Kunden oder für einzelne Lieferanten fest.

Im Einkauf arbeiten Sie in der Regel nur mit einem Preisschlüssel, z. B. dem Schlüssel EK. Sie können aber auch im Einkaufsbereich nach verschiedenen Preisschlüsseln differenzieren.

Bei der Preisfindung wird folgende Hierarchie durchlaufen:

*   Manuelle Preiseingaben im Auftrag oder Angebot (oberste Priorität)
*   Objektbezogene Vereinbarungen
*   Kunden-/lieferantenbezogene Vereinbarungen
*   Gruppenspezifische Vereinbarungen
*   Allgemeine Vereinbarungen

Innerhalb dieser Hierarchiestufen können allgemeine Preise, Sonderbedingungen für Warengruppen und einzelne Produkte, Austauschpreise und Zuschläge für Modelle und Sprossen hinterlegt werden.

### Individualpreise

Bei der Gestaltung individueller Preise für Kunden und Lieferanten können Sie alle Bezugsgrößen nutzen, die auch für die allgemeinen Preislisten und Zuschläge gelten. So können Sie entweder Preistabellen für Ihre einzelnen Kunden oder Lieferanten anlegen oder die Preise im Dokument vereinbarungsgemäß anpassen.

### Preislistenimport

Preislisten Ihrer Lieferanten können Sie importieren, wenn diese als Datei vorliegen.

> **Historie der Preisänderungen**
> Wenn Sie mit einer Gupta-Datenbank arbeiten, können Sie Änderungen der Preise in einer Historie verfolgen. Diese Funktion ist im Part Stammdaten beschrieben.

### Stammdaten der Preise prüfen

In Bestellungen können die Preise nur berechnet werden, wenn die Einkaufspreise korrekt sind. Im Part Stammdaten ist ausführlich beschrieben, wie Sie die Stammdaten zu Ihren Preisen anlegen. In der folgenden Beschreibung wird daher nur auf die Besonderheiten eingegangen, die Sie für den Einkauf beachten müssen.

**So prüfen Sie die Stammdaten Ihrer Preislisten**

1.  Wählen Sie Stammdaten > Preise > Preise und prüfen Sie, ob der Jahrgang, der Schlüssel und der Tarif für die Einkaufspreise (EK) richtig definiert sind.
2.  Wechseln Sie zum Dialog Preise und lassen Sie sich die Tabelle und den Tarif für die EK-Preise anzeigen.
    Wenn Sie die Suche nicht einschränken, werden alle Preistabellen aufgelistet.

*Abb. D-13: EK-Preistabellen - Preisauswahl. Die Abbildung zeigt eine Benutzeroberfläche mit einer Preisauswahl (A) auf der linken Seite und einer Preistabelle (B) auf der rechten Seite.*

3.  Markieren Sie die Preistabelle (B), die Sie prüfen wollen, und wechseln Sie zu dem Register, in dem der Preis festgelegt ist.
    In diesem Beispiel ist der Einzelpreis (A) geprüft.

*Abb. D-14: Preisauswahl – Einzelpreis. Die Abbildung zeigt eine Übersichtstabelle mit Preisen (A), Preiseinheiten (B) und Währungen (C) für verschiedene Tarife. Nicht definierte Preise sind rot markiert.*

    In der Übersicht sind alle Tarife der ausgewählten Preistabelle aufgeführt. Die nicht definierten Preise sind in roter Schrift angezeigt.
4.  Prüfen Sie, ob der Preis auf dem aktuellen Stand ist, oder korrigieren Sie ihn. Setzen Sie dazu den Cursor in die Zelle Preis und überschreiben Sie den Eintrag.
5.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Daten werden gespeichert.

**Ergänzende Informationen**
⇨ Stammdaten, "Stammdaten für Preise" auf Seite B-214
⇨ Stammdaten, "Einzelpreise anlegen" auf Seite B-239
⇨ Stammdaten, "Firmendaten - Kalkulation" auf Seite B-994

## Dokumentenstatus

#### Lernziele
*   Statusumsetzung von referenzierten Dokumenten kennenlernen.
*   Statuszuordnung prüfen.

#### Nutzen
*   Statuszuordnungen für referenzierte Dokumente werden neben den Statuszuordnungen für unabhängige Dokumente gepflegt. Anhand des Status kann also erkannt werden, ob eine Bestellung referenziert ist.
*   Wareneingänge zu einer Bestellung setzen den Status des referenzierten Auftrags um. So kann am Auftrag der aktuelle Stand erkannt werden.

#### Merke
| Begriff | Erklärung |
| :--- | :--- |
| **Statuszuordnungen** | Statuszuordnungen für referenzierte Dokumente müssen den gleichen Mindeststatus haben. |
| **Statusumsetzung** | Der Status des referenzierten Auftrags wird beim Wareneingang der Bestellung umgesetzt. |
| **Voreinstellungen** | Stammdaten: Statuszuordnung |

### Statuszuordnung

Die Einkaufsdokumente durchlaufen von der Erfassung bis zur Archivierung mehrere Programmpunkte, die jeweils durch einen Status gekennzeichnet sind. An diesen Status können Bedingungen und Sperren geknüpft sein.
Wie Sie die Statuspunkte und -zuordnungen einrichten, hängt von den Geschäftsabläufen in Ihrem Unternehmen ab. Eine ausführliche Beschreibung finden Sie dazu im Part Stammdaten.

*Abb. D-15: Statuszuordnung für referenzierte Dokumente. Die Abbildung zeigt die Konfiguration von Statuszuordnungen. (A) zeigt den Status für einen Auftrag mit referenzierter Bestellung und (B) den korrespondierenden Status für die Bestellung.*

Statuszuordnungen werden für referenzierte Dokumente und für unabhängige Dokumente getrennt eingerichtet, z. B. für den Wareneingang.

### Statusvergabe

Der Status der Dokumente wird in der Regel umgesetzt, wenn eine Bestellung geändert, versendet usw. wird. Dabei wird unterschieden, ob die Bestellung durch einen Auftrag oder unabhängig erzeugt wurde.

**Beispiele**

| für Aufträge | für Bestellungen |
| :--- | :--- |
| 30 - Auftrag in Einkauf übergeben | |
| 31 - AB Lieferant teilweise/Auftrag | 62 - AB Lieferant teilweise/Bestellung |
| 32 - AB Lieferant komplett/Auftrag | 63 - AB Lieferant komplett/Bestellung |
| 33 - Wareneingang teilweise/Auftrag | 64 - Wareneingang teilweise/Bestellung |
| 34 - Wareneingang komplett/Auftrag | 65 - Wareneingang komplett/Bestellung |
| | 66 - Rechnungskontrolle |

Wenn im Wareneingang die Nummer der Auftragsbestätigung (AB) des Lieferanten eingegeben ist, wird der Status der Bestellung umgesetzt.

Wenn ein Wareneingang zu einer Bestellung aus einem Kundenauftrag (referenzierte Bestellung) verbucht wird, zu dem weitere Bestellungen noch offen sind, wird der Status des Auftrages auf Wareneingang teilweise/Auftrag gesetzt.

**Ergänzende Informationen**
⇨ Verkauf, "Status" auf Seite C-227
⇨ Stammdaten, "Geschäftsabläufe abbilden" auf Seite B-427
⇨ Stammdaten, "Statuszuordnung" auf Seite B-899

## Bestellungen

In diesem Themenblock lernen Sie, wie Sie Bestellungen erzeugen und Termine prüfen.

Dazu gehören folgende Lerneinheiten:

*   "Bestellübergabe vs. manuelle Bestellung" auf Seite D-44
*   "Bestellpositionen im Auftrag" auf Seite D-50
*   "Bestellübergabe" auf Seite D-60
*   "Manuelle Bestellung" auf Seite D-79
*   "Auftragsbestätigung des Lieferanten" auf Seite D-86
*   "Lieferterminkontrolle" auf Seite D-100
*   "Anfrage" auf Seite D-110

Üblicherweise erfassen Sie eine Bestellung in folgenden Schritten:

*   Anfrage erstellen (optional)
*   Bestellung erfassen
*   Bestellung an den Lieferanten senden
*   Auftragsbestätigung vom Lieferanten erfassen
    *   Preise prüfen
    *   Termine und Tourenplanung nach Rückmeldungen korrigieren
    *   Kunden über Terminänderungen informieren
*   Auftragsbestätigung des Lieferanten anmahnen

Diese Reihenfolge entspricht im Wesentlichen auch der Reihenfolge der Dialoganordnung in A+W Business. Einige der Schritte können jedoch über mehrere Dialoge ausgeführt werden. Sie sind daher in einer Lerneinheit zusammengefasst.

Die Preise können bereits auf einer Auftragsbestätigung des Lieferanten geprüft werden. In der Praxis kann durchaus vorkommen, dass Auftragsbestätigung und Lieferung zusammen mit der Rechnung eintreffen. Da die Dialoge für die Preiskontrolle und die Rechnungskontrolle identisch sind, wird das Konzept der Preis- und Rechnungskontrolle im Themenblock Wareneingang beschrieben.

⇨ "Eingangsrechnung" auf Seite D-144

Eine Anfrage wird logischerweise vor der Bestellung erstellt, sie ist jedoch nicht zwingend erforderlich. In diesem Tutorial wird die Anfrage nach den Bestellungen behandelt, weil Sie dann bereits mit allen Details der Bestellung vertraut sind.

### Bestellübergabe vs. manuelle Bestellung

#### Lernziele
*   Unterschied zwischen automatischer (referenzierter) und unabhängiger Bestellung kennenlernen.

#### Nutzen
*   Auftragspositionen, die bestellt werden müssen, können automatisch in eine (referenzierte) Bestellung geleitet werden.
*   Lagerbestände werden durch Lagerbestellungen ergänzt. Diese werden manuell erfasst. Sie können auch durch Unterschreitung von Mindestbeständen angelegt werden. (Diese Funktion ist im Part Lagerwirtschaft beschrieben.)

#### Merke
| Begriff | Erklärung |
| :--- | :--- |
| **Bestellung aus Auftrag** | Auftragspositionen, die bestellt werden müssen, werden im Bestellpool an den Einkauf übergeben. Mit der Übergabe wird automatisch eine Bestellung erzeugt. |
| **Referenzierte Bestellung** | Aus einer Auftragsposition, die an den Einkauf übergeben wurde, wird eine referenzierte Bestellung mit einer eigenen Dokumentennummer erzeugt. |
| **Unabhängige Bestellung** | Unabhängige Bestellungen werden manuell erfasst. Bei unabhängigen Bestellungen wird der Lagerbestand nicht aktualisiert, wenn der Wareneingang gebucht wird. |
| **Lagerbestellung** | Lagerbestellungen dienen dazu, den Lagerbestand aufzufüllen. Sie können manuell erfasst werden. |
| **Voreinstellungen** | **Stammdaten:**<br>- Lieferantendaten (Marktpartner)<br>- Lieferantenkartei<br>**Firmendaten:**<br>- Register Dokumente<br>- Register Parameter<br>- Register Lager/EK/EDI |

### Dokument Bestellung

Bestellungen können entweder auftragsabhängig oder unabhängig eingegeben werden:

*   **Auftragsabhängige (referenzierte) Bestellungen** beziehen sich auf eine Position im Kundenauftrag. Sie werden durch die Bestellübergabe erzeugt. Im Bestellpool schlägt A+W Business aufgrund der Daten aus der Lieferantenkartei einen Lieferanten vor.
*   **Unabhängige Bestellungen** dienen in der Regel nicht dazu, den Lagerbestand aufzufüllen, da der Wareneingang nicht automatisch den Lagerbestand aktualisiert. Sie werden manuell erfasst.
*   **Lagerbestellungen** dienen dazu, den Lagerbestand aufzufüllen. Sie können manuell erfasst oder durch Unterschreitung eines Mindestbestands erzeugt werden.

*Abb. D-16: Arten der Bestellung. Ein Diagramm zeigt, dass auftragsabhängige und unabhängige Bestellungen zu einem Wareneingang führen, der den Auftrag beeinflusst. Manuelle und automatische Lagerbestellungen führen ebenfalls zu einem Wareneingang, der das Lager (mit Mindestbestand) aktualisiert.*

In dieser vereinfachten Darstellung sehen Sie, wozu die unterschiedlichen Bestellungen erfasst werden. In den folgenden Einheiten werden die auftragsabhängigen und die unabhängigen Bestellungen ausführlich beschrieben.
Lagerbestellungen werden ausführlich im Part Lagerwirtschaft beschrieben.

Alle Bestellungen sind eigene Dokumente mit einem eigenen Nummernkreis. Sie werden im Dialog zur Dokumentenverwaltung angezeigt und können unabhängig davon, wie sie erzeugt wurden, bearbeitet werden.

*Abb. D-17: Dokument Bestellung. Ein Screenshot zeigt Details einer Bestellung, darunter Termine (A), Zusatzinformationen (B) und den Dokumententyp (C), der zwischen automatischer, manueller und Lagerbestellung unterscheidet.*

Bestellungen müssen an den Lieferanten gesendet werden. Dazu steht neben dem Fax- und dem E-Mail-Versand auch die Datenübertragung über Schnittstellen zur Verfügung.

### Voreinstellungen für Bestellungen prüfen

Für die Bestellungen müssen Sie die Voreinstellungen in den Firmendaten prüfen. Im Part Stammdaten ist ausführlich beschrieben, wie Sie die Stammdaten zu Ihrer Firma einrichten. In der folgenden Beschreibung wird daher nur auf die Besonderheiten eingegangen, die Sie für den Einkauf beachten müssen.

> **A+W Business neu starten**
> Nach Änderungen der Firmendaten sollten Sie A+W Business neu starten.

**So prüfen Sie die Einstellungen für Bestellungen**
1.  Wählen Sie Stammdaten > Firma > Firmendaten.
    Der Dialog Firmendaten wird geöffnet.
    ⇨ Stammdaten, "Firmendaten" auf Seite B-930
2.  Wechseln Sie zum Register Dokumente und prüfen Sie die Einstellungen für den Fax- und E-Mail-Versand.

*Abb. D-18: Firmendaten - Dokumente. Der Screenshot zeigt Einstellungen für den Dokumentenversand: (A) Faxversand einzeln oder gesammelt, (B) E-Mail-Versand einzeln oder gesammelt, und (C) Dateiformat für E-Mail-Anhänge.*

3.  Wechseln Sie zum Register Parameter und prüfen Sie die Einstellungen wie in der folgenden Abbildung gezeigt.

*Abb. D-19: Firmendaten - Parameter. Ein Screenshot zeigt verschiedene Parameter. (A) Rückschreibung von Änderungen in referenzierte Dokumente. (B) Übernahme von Bestelltexten für openTRANS. (C) Kennzeichnung von Positionen als Bestellung bei Überschreitung der Lagermaße. (D) Verwendung virtueller Positionsnummern für den Kisten-Wareneingang.*

Die Einstellungen werden in separaten Einheiten ausführlich beschrieben.
*   **Checkbox A:**
    ⇨ "Bestellte Auftragsposition ändern" auf Seite D-57
*   **Checkboxen B und D:**
    ⇨ "Kistengeschäft" auf Seite D-136
    ⇨ "Export/Import (openTRANS)" auf Seite D-151
*   **Lagerbestellungen (C)** sind ausführlich im Part Lagerwirtschaft beschrieben.

4.  Wechseln Sie zum Register Lager/EK/EDI und prüfen Sie die Einstellung im Bereich Einkauf.

*Abb. D-20: Firmendaten – Lager/EK/EDI. Der Screenshot zeigt Einstellungen für Einkauf und Lager. (A) Option, ISO-Einheiten mit Bearbeitungen als Bestellartikel zu kennzeichnen. (B) Option, Positionen aus Lagerbestellungen anzuzeigen, auch wenn sie keine Lagerartikel sind.*

5.  Markieren Sie die Checkbox **ISO als Bestellartikel (Bearb. können Eigenfertigung sein)** (A).
    Wenn bei Isolierglas (ISO) Bearbeitungen mit der Beschaffungsart Produktion (Eigenfertigung) in der Stückliste vorhanden sind, können diese mitbestellt werden. Diese Einstellung ist sinnvoll, wenn Sie ISO-Einheiten nur bei Engpässen in der Produktion bestellen.
6.  Wählen Sie im Menü Start > Speichern, um die Änderungen zu speichern.
    Die Daten werden gespeichert.

### Bestellpositionen im Auftrag

#### Lernziele
*   Bestellposition erfassen und Kennzeichen zuordnen.
*   Lieferanten in der Auftragsposition ändern.
*   Lieferanten für den gesamten Auftrag ändern.
*   Bestellte Position ändern.

#### Nutzen
Aus Auftragspositionen können Bestellungen erzeugt werden, ohne die Positionen als Bestellung neu zu erfassen.

#### Merke
| Begriff | Erklärung |
| :--- | :--- |
| **Bestellposition** | Bestellpositionen aus Aufträgen erzeugen pro Standard-Lieferant eine eigene Bestellung. |
| **Bestellkennzeichen** | Als Bestellkennzeichen werden folgende Beschaffungsarten bezeichnet: <br>- Bestellung <br>- Bestellung (komplett) |
| **Bestellung (komplett)** | Dieses Kennzeichen wird bei Produkten mit Stückliste verwendet, die als Ganzes bestellt werden sollen, z. B. eine komplette Tür mit Beschlägen. |
| **Bestellung** | Dieses Kennzeichen wird bei Produkten verwendet, deren einzelne Komponenten bestellt werden sollen, z. B. nur die Beschläge. |
| **Voreinstellungen** | **Stammdaten:**<br>- Lieferantendaten (Marktpartner)<br>- Lieferantenkartei<br>**Firmendaten:**<br>- Register Dokumente<br>- Register Parameter<br>- Register Lager/EK/EDI |

### Kundenbestellung

Im Kundenauftrag können Positionen enthalten sein, die aus unterschiedlichen Gründen bestellt werden müssen, z. B., weil das Produkt nicht im Lager geführt wird oder weil Engpässe in der Produktion den Liefertermin gefährden und darum die Position komplett bestellt werden muss. Grundsätzlich kann also jede Position eines Auftrags bestellt werden.

Bestellungen zu Auftragspositionen können aus den Aufträgen heraus erzeugt werden. Dazu muss mindestens eine Stücklisten-Komponente oder die gesamte Position als Bestellung gekennzeichnet sein.

Bestellungen werden nicht automatisch an den Einkauf übergeben. Sind Bestellartikel in einem Auftrag enthalten, können Sie sich dies durch eine Meldung anzeigen lassen, wenn Sie die Positionserfassung schließen.

*Abb. D-21: Bestellkennzeichen für Stücklisten-Komponente. Der Screenshot zeigt eine Auftragsposition, bei der eine Komponente zur Bestellung markiert ist (A) und die Beschaffungsart geändert wurde (B). Ein Hinweisdialog meldet "Es sind Bestellartikel enthalten".*

Für die Bestellpositionen in einem Auftrag wird ein neues Dokument erzeugt: eine Bestellung. Dieses Dokument wird durch die Übergabe des Auftrags an den Einkauf erzeugt. Die Bestellübergabe ist einer separaten Einheit beschrieben.

⇨ "Bestellübergabe" auf Seite D-60

Sind in einem Auftrag verschiedene Bestellpositionen enthalten, werden so viele Bestellungen erzeugt, wie unterschiedliche Standard-Lieferanten aus der Lieferantenkartei ausgelesen wurden.

### Lieferant für Auftragsposition

Achten Sie im Auftrag darauf, dass Sie für Bestellartikel den gewünschten Lieferanten auswählen. Sie haben dazu verschiedene Möglichkeiten:

*   **Dokumentenerfassung - Register Konditionen:**
    *Abb. D-16 zeigt das Feld "Lieferant" im Register "Konditionen".*
    Diese Einstellung gilt übergreifend für alle Positionen im aktuellen Auftrag, sofern sie nicht (anschließend) auf den Ebenen der Position oder der Stückliste überschrieben werden.

*   **Positionserfassung – Register Zusatz:**
    *Abb. D-16 zeigt das Feld "Lieferant" im Register "Zusatz".*
    Diese Einstellung gilt nur für die jeweils markierte Position.

*   **Positionserfassung - Register Stückliste:**
    *Abb. D-16 zeigt das Feld "Lieferant" in den Details der Stückliste.*
    Diese Einstellung gilt nur für die jeweils markierte Stücklisten-Komponente.

*   **Bestellübergabe:**
    Wenn bei den oben genannten Möglichkeiten keine Angaben gemacht sind, wird in der Bestellung automatisch der Standard-Lieferant eingesetzt.
    Die Einstellungen aus dem Auftrag und/oder den Produktstammdaten können im Bestellpool überschrieben werden.
    Die Bestellübergabe ist einer separaten Einheit beschrieben.
    ⇨ "Bestellübergabe" auf Seite D-60

### Änderung in bestellten Positionen

Auftragspositionen, die bereits bestellt wurden, werden für die weitere Bearbeitung gesperrt. Sie können nachträglich in der Positionserfassung des Auftrags (oder der Bestellung) erst geändert werden, wenn die Sperrung manuell aufgehoben wird. Änderungen können sich z. B. auf Preise, Mengen oder Maße beziehen. Der Tarif kann trotz der Sperrung geändert werden.

Die Änderungen müssen in die referenzierten Bestellungen übernommen werden. Wenn Sie Maße oder Stückzahl einer bestellten Position ändern, können Sie die Änderungen in der ursprünglichen Bestellung eintragen. Die Bestellung muss dann mit einem Hinweis auf die Änderungen erneut an den Lieferanten gesendet werden.

Der geänderte Auftrag muss anschließend wieder über den Bestellpool an den Einkauf übergeben werden.

#### Bestellposition im Auftrag erfassen

In einer Auftragsposition können Komponenten oder ganze Positionen erfasst sein, aus denen eine Bestellung erzeugt werden muss. Dazu muss die richtige Beschaffungsart (Bestellkennzeichen) zugewiesen sein.

**So erfassen Sie im Auftrag eine Position zur Bestellung**
1.  Erfassen Sie den Auftragskopf und wechseln Sie zum Register Positionen.
2.  Erfassen Sie das Produkt, das Ihr Kunde haben möchte.

*Abb. D-22: Bestellposition im Auftrag. Der Screenshot zeigt eine Auftragsposition (B) mit der zugewiesenen Beschaffungsart "Bestellung (komplett)" (A).*

3.  Prüfen Sie die korrekte Einstellung der Beschaffungsart (A).
4.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
5.  Erfassen Sie eine weitere Position, in der jedoch nur eine Komponente der Stückliste bestellt werden soll.
6.  Wechseln Sie zum Register Stückliste.

*Abb. D-23: Beschaffungsart für Stücklisten-Komponente. Der Screenshot zeigt die Detailansicht einer Stücklisten-Komponente (A), für die eine Beschaffungsart (C) und ein Lieferant (B) ausgewählt werden.*

7.  Markieren Sie die Komponente (A), die bestellt werden muss.
8.  Wählen Sie die Beschaffungsart (C) und den Lieferanten (B) aus.
9.  Wählen Sie im Menü Start > Speichern, um die Änderungen zu speichern.
    Sie können jetzt weitere Positionen erfassen oder die erfassten Positionen ändern.
    Wenn Sie alle Bestellpositionen bei demselben Lieferanten bestellen wollen, wählen im Auftragskopf Sie im Register Konditionen den neuen Lieferanten aus.
    ⇨ "So ändern Sie den Lieferanten aller Bestellpositionen" auf Seite D-56
10. Schließen Sie die Positionserfassung.
    Wenn für die Bestellpositionen kein Standard-Lieferant angegeben war, muss der Lieferant im Dialog Bestellübergabe – Bestellpool angegeben werden.
    ⇨ "So erzeugen Sie eine Bestellung zu einem Kundenauftrag" auf Seite D-68

#### Lieferanten im Auftrag ändern

Sie können im Auftragskopf einen anderen Lieferanten für die Bestellungen auswählen. Dieser Lieferant gilt dann für alle Bestellpositionen des Auftrags.

> **Bestellkennzeichen im Nummernverwalter ändern**
> Wenn Sie in mehreren Aufträgen das Bestellkennzeichen ändern müssen, können Sie diese Aufträge in einem neuen Nummernverwalter sammeln. In diesem Nummernverwalter können Sie über das Menü Funktionen > Kennzeichenänderung die Beschaffungsart und den Lieferanten für alle Dokumente gemeinsam ändern.

**So ändern Sie den Lieferanten aller Bestellpositionen**
1.  Öffnen Sie den Auftrag mit den Bestellpositionen.
2.  Wechseln Sie zum Register Konditionen.

*Abb. D-24: Auftragskopf - Register Konditionen. Der Screenshot zeigt das Feld "Lieferant" (A), in dem ein Lieferant für alle Bestellpositionen des Auftrags ausgewählt wird.*

3.  Wählen Sie den gewünschten Lieferanten (A) aus.
4.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Abfrage wird angezeigt: Soll das Bestellkennzeichen komplett für alle Positionen gesetzt werden.
5.  Wählen Sie:
    *   **[Ja]:** Der gesamte Auftrag wird an den Einkauf zur Bestellung bei dem gewählten Lieferanten übergeben.
    *   **[Nein]:** Nur die Bestellpositionen werden an den Einkauf übergeben.
6.  Schließen Sie den Auftrag.
    Sie können jetzt die Bestellungen an den Einkauf übergeben.
    ⇨ "So erzeugen Sie eine Bestellung zu einem Kundenauftrag" auf Seite D-68

#### Bestellte Auftragsposition ändern

Sie können eine bestellte Position im Auftrag nachträglich ändern und die Bestellung neu erzeugen. Vergessen Sie dabei nicht, dem Lieferanten deutlich zu machen, welche Bestellung neu ist und welche frühere Bestellung durch sie ersetzt wird.

> **Bestellte Position ändern**
> Sie können eine bestellte Position nur so lange ändern, wie keine Auftragsbestätigung des Lieferanten oder ein Wareneingang erfasst wurde oder ein Sperrstatus erreicht ist.

**So ändern Sie eine bestellte Position**
1.  Öffnen Sie das Dokument, in dem Sie eine bestellte Position ändern möchten, und wechseln Sie zur Positionserfassung.
2.  Markieren Sie die Position, die Sie ändern wollen.

*Abb. D-25: Beschaffungsart für Stücklisten-Komponente. Der Screenshot zeigt eine Liste von Auftragspositionen. Bestellte Positionen sind gesperrt (A) und haben einen entsprechenden Hinweis (B). Nur der Preis ist änderbar.*

    Die Felder (A) der bestellten Positionen sind gesperrt. In der Spalte Hinweis (B) wird der entsprechende Text angezeigt.
3.  Wählen Sie im Menü Funktionen > Gruppe Position > Gesperrte Position ändern.
    Die Felder werden freigeschaltet.
4.  Geben Sie die Änderungen ein, z. B. die Stückzahl.
5.  Wählen Sie im Menü Start > Speichern, um die Änderung zu speichern.
    Die Änderungen werden gespeichert. Sie können weitere Änderungen eintragen.
6.  Schließen Sie die Positionserfassung.
    Der Dialog Bestellübergabe – Bestellpool wird geöffnet und Sie können die Bestellungen an den Einkauf übergeben.
    ⇨ "So erzeugen Sie eine Bestellung zu einem Kundenauftrag" auf Seite D-68

*Abb. D-26: Bestellübergabe – Bestellpool. Der Screenshot zeigt den Bestellpool, in dem geänderte Bestellungen an den Einkauf übergeben werden können.*

    ⇨ Verkauf, "Bestellübergabe" auf Seite C-669
7.  Übergeben Sie die geänderte Bestellung wie unter Bestellung übergeben beschrieben.
    ⇨ "Dokument in den Bestellpool stellen" auf Seite D-68

> **Lieferanten informieren**
> Vergessen Sie nicht, Ihren Lieferanten über die Änderung zu informieren, wenn Sie die ursprüngliche Bestellung bereits an ihn weitergeleitet hatten.

### Bestellübergabe

#### Lernziele
*   Auftrag mit Bestellpositionen in den Bestellpool stellen.
*   Bestellpositionen im Bestellpool prüfen.
*   Lieferant und Liefertermin ändern.
*   Bestellpositionen an den Einkauf übergeben.

#### Nutzen
*   Auftragspositionen können direkt an den Einkauf übergeben werden. Die Bestellpositionen brauchen nicht im Bestellpool geprüft zu werden.
*   Im Bestellpool kann ein Preisvergleich geöffnet werden, um den günstigsten (oder schnellsten) Lieferanten auszuwählen.
*   Termine, Preise und Lieferanten von Bestellungen können vor der Übergabe geprüft werden.

#### Merke
| Begriff | Erklärung |
| :--- | :--- |
| **Bestellübergabe** | Durch die Bestellübergabe werden die Bestellungen zu Auftragspositionen erzeugt. |
| **Bestellpool** | Die Übergabe einer Bestellung muss manuell angestoßen werden. Aus dem Bestellpool werden nur die Auftragspositionen mit einem Bestellkennzeichen an den Einkauf übergeben. Der Bestellpool wird manuell gefüllt. Er listet immer alle Dokumente auf, die im gewählten Nummernverwalter stehen. |
| **Bestellungen** | Bestellpositionen aus verschiedenen Aufträgen können zu einer Sammelbestellung zusammengefasst werden, wenn für diese Positionen der Lieferant und das Lieferdatum identisch sind. |
| **Lieferant** | Wenn in einem Auftrag mehrere Positionen mit Bestellkennzeichen erfasst wurden, wird für jeden Lieferanten eine eigene Bestellung erzeugt. |
| **Preisvergleich** | Vor der Übergabe der Bestellung können Sie die Preise der Lieferanten vergleichen, die das Produkt liefern können. Dazu muss die Lieferantenkartei gepflegt werden. |
| **Terminänderung** | Wird im Bestellpool das Anlieferdatum beim Kunden geändert, wird diese Änderung auch in den referenzierten Auftrag übernommen. |
| **Bestellung senden** | Bestellungen, die über den Bestellpool erzeugt wurden, müssen über den Dialog Formular-/ Etikettendruck gedruckt und an den Lieferanten gesendet werden. |
| **Voreinstellungen** | **Bestellübergabe > Menü Optionen:**<br>- *Auftragsbezogene Übergabe:* Die Bestellungen werden pro Auftrag übergeben. Wenn diese Option nicht aktiviert ist, können Sammelbestellungen erzeugt werden.<br>- *Bestellnummer = Auftragsnummer:* Diese Option ist nur freigeschaltet, wenn die Option Auftragsbezogene Übergabe aktiviert ist. Diese Einstellung darf nicht aktiviert sein, wenn unterschiedliche Lieferanten in einem Auftrag erfasst sind.<br>**Stammdaten:**<br>- Nummernkreise<br>- Lieferantenkartei<br>**Firmendaten:**<br>- Register Produktion (Profit-Center-Abrechnung)<br>- Register Lager/EK/EDI (Abstandhalter mitbestellen) |

### Bestellpool

Bestellungen aus Kundenaufträgen werden automatisch erzeugt.

*Abb. D-27: Bestellpositionen im Bestellpool. Der Screenshot zeigt den Bestellpool mit Spalten für Auftragsnummer (A), Positionsnummer (B), Lieferant (C), Produktbezeichnung (D) und Optionen zur Erzeugung von Bestellungen (E) oder Anfragen (F). Nach der Übergabe wird die Dokumentennummer (G) angezeigt.*

Dazu werden die Auftragspositionen über den Bestellpool an den Einkauf übergeben. Auftragspositionen ohne Bestellartikel werden nicht weiterverarbeitet. Anhand des Dokumentenstatus erkennt das Programm, welche Positionen zur Bestellung übergeben werden können.

Die Prüfung der Kundenaufträge im Bestellpool bezieht sich nur auf Produkte mit der Beschaffungsart Bestellung oder Bestellung (komplett).

*Abb. D-28: Ablauf der Prüfung von Aufträgen im Bestellpool. Ein Flussdiagramm zeigt, wie Aufträge im Bestellpool geprüft werden: Hauptposition, Stücklisten-Komponente und untergeordnete Komponente. Pro Lieferant wird eine Bestellung erzeugt.*

Die Kundenaufträge werden zunächst auf der Ebene der Hauptposition und dann auf der Ebene der Stückliste nach Komponenten mit einer der beiden Beschaffungsarten durchsucht. Die Produkte werden dabei nach einfachen Bestellteilen und solchen Bestellteilen unterschieden, bei denen alle untergeordneten Produkte mitbestellt werden.

Wenn in einem Kundenauftrag mehrere Positionen erfasst sind, die bei unterschiedlichen Lieferanten bestellt werden, wird für jeden Lieferanten eine eigene Bestellung erzeugt.

Wenn in einem Kundenauftrag Lagerartikel in einer Stückzahl angegeben sind, die den aktuellen Lagerbestand überschreitet, müssen diese Lagerartikel durch eine (manuelle) Lagerbestellung erfasst und bestellt werden.

#### Prüfungen

Über das Menü Optionen können verschiedene Prüfungen aktiviert werden, z. B.:
*   **Lieferterminprüfung:**
    Der Liefertermin wird automatisch geprüft. Ändern Sie einen Liefertermin, der nicht an einem Tourentag liegt, wird eine entsprechende Meldung angezeigt.
*   **Lieferantentour berücksichtigen:**
    Wenn die Bestellung auf einen Liefertermin fällt, der nicht an einem Tourentag liegt, wird eine entsprechende Meldung angezeigt. Dazu müssen die Lieferantentouren in den Stammdaten hinterlegt werden.
*   **Vorlauftage mit Kombiwarengruppe ermitteln:**
    Wenn in den Kombiwarengruppen Vorlauftage hinterlegt sind, sollen diese zur Berechnung des Liefertermins herangezogen werden.
    ⇨ Stammdaten, "Vorlauftage" auf Seite B-576
*   **Produktbezeichnung aus Lieferantenkartei:**
    Die Bezeichnung der bestellten Produkte wird aus der Lieferantenkartei übernommen.
*   **Keine Kostenrückschreibung:**
    Die Kosten werden nicht in die EK-Preise des Auftrags zurückgeschrieben.
*   **Maßzuschläge berücksichtigen:**
    Bei der Bestellung sollen die Maßzuschläge mit übergeben werden.

#### Bestellübergabe

Vor der Übergabe der Bestellpositionen können Sie den Modus auswählen.

*Abb. D-29: Bestellmodus. Optionen: Pool füllen, Sofort bestellen, Sofort anfragen.*

*Abb. D-30: Lieferanten im Bestellpool ändern. Ein Flussdiagramm zeigt die Optionen der Bestellübergabe: Sofort anfragen (erzeugt Anfrage), Sofort bestellen (erzeugt Bestellung), Pool füllen (füllt Bestellpool). Im Bestellpool können Preisvergleiche, Terminprüfungen und Lieferantenänderungen durchgeführt werden.*

Mit der Option **Sofort bestellen**, werden die Bestellungen erzeugt, ohne sie in den Bestellpool zu stellen. Im Bestellpool können die Termine und die Lieferanten geändert werden.

#### Lieferantenauswahl und Preisvergleich

Bei gefährdeten Terminen können andere Lieferanten ausgewählt werden. Diese werden aus der Lieferantenkartei ausgelesen. Wenn dort auch Preise pro Lieferant hinterlegt sind, ist ein Preisvergleich möglich, so dass Sie unabhängig von Terminproblemen auch zu dem günstigsten Lieferanten wechseln können.

*Abb. D-31: Lieferanten im Bestellpool ändern. Ein Diagramm zeigt, wie aus Aufträgen mit Bestellpositionen im Bestellpool Sammel-Bestellungen für verschiedene Lieferanten generiert werden.*

> **Liefertermine**
> Damit Liefertermine berechnet werden können, muss in der Lieferantenkartei die Lieferzeit für jeden einzelnen Lieferanten hinterlegt sein. Bei der Übergabe von Kundenaufträgen wird der Termin der Auslieferung beim Kunden geprüft. Dazu wird angezeigt, ob der Lieferant aufgrund seiner spezifischen Lieferzeit in der Lage ist, die Bestellung rechtzeitig zu liefern.
> Der Liefertermin des Lieferanten im Bestellpool wird aus dem Versandtag minus der hinterlegten Vorlauftage zur jeweiligen WGR ermittelt.
> Dabei werden die Wochentage und die Tour berücksichtigt. Wenn keine Vorlauftage eintragen sind, wird der Versandtag als Liefertermin übernommen.
> Im Bestellpool wird farblich hervorgehoben, wenn ein Liefertermin aus dem Auftrag aufgrund der Liefertage aus der Lieferantenkartei für die Bestellung nicht eingehalten werden kann.
> Der Lieferant und/oder der Liefertermin kann dann schon im Bestellpool geändert werden. Die Änderungen werden in den Auftrag zurückgeschrieben.

#### Erzeugte Bestellungen

Nachdem die Übergabe abgeschlossen ist, zeigt eine Meldung an, wie viele Dokumente nicht übergeben (verarbeitet) wurden.

*Abb. D-32: Fehlerhafte Dokumente. Eine Hinweismeldung "Es wurden 4 Dokumente nicht verarbeitet!" wird über einer Liste von Dokumenten angezeigt.*

Diese müssen Sie dann einzeln prüfen und ggf. korrigieren. Dies können z. B. folgende Fehler sein:

*   Keine Bestellkennzeichen gefunden.
*   Auftrag ist noch geöffnet.
*   Status lässt die Übergabe nicht zu.

Aus den Auftragspositionen mit Bestellkennzeichen wurden Bestellungen erzeugt, die Sie in der Dokumentenverwaltung für Bestellungen öffnen und prüfen können. Diese Bestellungen senden Sie auf die übliche Weise an die betreffenden Lieferanten.

Für alle übergebenen Positionen wird der Status umgesetzt. In den referenzierten Aufträgen wird der Status umgesetzt.

**Bestellnummern**
Üblicherweise erhalten die automatisch erzeugten Bestellungen Nummern aus dem entsprechenden Nummernkreis. Sie können bei der Übergabe jedoch entscheiden, ob die Auftragsnummer auch als Bestellnummer verwendet werden soll.

#### Sammelbestellungen pro Lieferant

Bestellungen aus verschiedenen Aufträgen an denselben Lieferanten werden zu Sammelbestellungen zusammengefasst. Dabei orientiert sich das System an der Reihenfolge, in der die Einträge im Bestellpool aufgeführt sind. In diesem Fall darf jedoch die Auftragsnummer nicht als Bestellnummer übernommen werden.

Wenn Sie im Bestellpool alle Positionen für einen Lieferanten markiert haben, können diese zu einer Sammelbestellung zusammengefasst werden.

Dazu müssen folgende Voraussetzungen erfüllt sein:

*   Identischer Lieferant
*   Identischer Liefertermin
*   Das Kennzeichen für Sammelbestellungen in den Lieferantenstammdaten muss gesetzt sein (Register Auftrag).

Im Menü **Funktionen > Markierungsoptionen** legen Sie fest, für welchen Lieferanten die Sammelbestellung erzeugt werden soll.

*Abb. D-33: Markierungsoptionen für Sammelbestellung. Ein Dialogfenster ermöglicht die Auswahl von Positionen nach Kriterien wie Auftragsnummer, Lieferant oder Liefertermin.*

Mit den Markierungsoptionen werden alle entsprechenden Positionen im Bestellpool automatisch markiert. Damit die Sammelbestellung erzeugt werden kann, muss im Menü **Optionen > Gruppe Übergabe > Auftragsbezogene Übergabe** deaktiviert sein.

#### Dokument in den Bestellpool stellen

Für die Übergabe werden die Aufträge in einem Nummernverwalter gesammelt. Der Bestellpool greift auf den Nummernverwalter zu, den Sie auswählen. Mit der Bestellübergabe kann ein neuer Nummernverwalter erstellt werden, in den die erfolgreichen Bestellungen gestellt werden. Die Bestellungen können nur erzeugt werden, wenn die Aufträge vor der Übergabe geschlossen sind.

**So erzeugen Sie eine Bestellung zu einem Kundenauftrag**
1.  Wählen Sie Dokumente > Auftrag > Bestellübergabe.

*Abb. D-34: Aufträge aus dem Nummernverwalter übergeben. Der Screenshot zeigt den Dialog zur Bestellübergabe. (A) Nummernverwalter der Aufträge, (B) Modus der Übergabe (Pool füllen, etc.), (C) Ziel-Nummernverwalter, (D) Ziel-Nummernkreis.*

2.  Wählen Sie den Modus (B) aus:
    *   **Pool füllen:**
        Mit dieser Option werden die Aufträge im Register Bestellpool angezeigt und können vor der Übergabe geprüft und geändert werden.
    *   **Sofort bestellen:**
        Mit dieser Option werden die Daten sofort als Bestellung beim Standard-Lieferanten erzeugt. Diese Option ist dann sinnvoll, wenn Sie zuvor keine Preise oder Liefertermine prüfen möchten.
    *   **Sofort anfragen:**
        Mit dieser Option werden die Daten als Anfrage beim Standard-Lieferanten erzeugt.
        Die Bestellungen können Sie anschließend drucken und auf die gewohnte Art an den Lieferanten senden, z. B. per E-Mail-Anhang.

In diesem Beispiel werden die Aufträge zunächst im Bestellpool geprüft.
3.  Wählen Sie den Nummernverwalter (A) aus, in dem die Aufträge mit Bestellpositionen stehen.
4.  Wählen Sie den Ziel-Nummernverwalter (C) aus, in den die erzeugten Bestellungen gestellt werden.
    Sie können einen neuen Namen eingeben und so einen neuen Nummernverwalter anlegen. Wenn Sie dazu einen anderen Mitarbeiter auswählen, wird der Nummernverwalter diesem zugeordnet.
5.  Wählen Sie ggf. einen anderen Ziel-Nummernkreis (D) aus.
6.  Wählen Sie im Menü Start > Ausführen, um die Aufträge in den Bestellpool zu stellen.

*Abb. D-35: Auftragspositionen im Bestellpool. Der Bestellpool wird gefüllt. Pro Auftrag werden die Bestellpositionen angezeigt.*

7.  Markieren Sie die Positionen, die Sie an den Einkauf übergeben möchten. Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf.

*Abb. D-36: Markierte Auftragspositionen übergeben. Nur die Positionen sind markiert, die mit einem X gekennzeichnet sind.*

8.  Wählen Sie im Menü Start > Ausführen, um die Aktion zu starten.
    Die aktivierten Prüfungen werden durchgeführt. Dies kann je nach Anzahl der Aufträge einige Momente dauern. Bestätigen Sie die jeweiligen Hinweise mit [Ja] oder [Nein], um die Prüfungen fortzusetzen. Wenn alle Prüfungen abgeschlossen sind, werden die zugehörigen Bestellungen angelegt und sind damit an den Einkauf übergeben.
    Die übergebenen Positionen werden aus dem Bestellpool gelöscht.
    Der Auftragsstatus wird hochgesetzt. In der Auftragshistorie wird die Nummer der Bestellung als Referenz angegeben.

*Abb. D-37: Bestellnummern nach der Übergabe. Nach der Übergabe der Positionen wird die Bestellnummer zum Auftrag angezeigt.*

Die erzeugten Bestellungen können Sie unter **Dokumente > Bestellung** öffnen und weiterbearbeiten. Drucken Sie die neue Bestellung und senden Sie sie an den Lieferanten.

#### Bestellung im Bestellpool ändern

Wenn zu einer Position Terminschwierigkeiten angezeigt werden, können Sie im Bestellpool einen anderen Lieferanten auswählen. Den Dialog zur Änderung des Lieferanten können Sie auch ohne Terminschwierigkeiten öffnen, um einen anderen als den vorgeschlagenen Standard-Lieferanten auszuwählen.

**So ändern Sie den Liefertermin und den Lieferanten**
1.  Wählen Sie Dokumente > Auftrag > Bestellübergabe.
2.  Stellen Sie die Aufträge in den Bestellpool.
    Dieser Vorgang ist in der vorausgegangenen Einheit beschrieben.
    ⇨ "Dokument in den Bestellpool stellen" auf Seite D-68
3.  Markieren Sie die Position, zu der Sie den Liefertermin ändern wollen.
    Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf.

*Abb. D-38: Position für die Änderung des Lieferanten markiert. Nur die Positionen sind markiert, die mit einem X gekennzeichnet sind.*

4.  Wählen Sie im Menü Funktionen > Lieferant/Liefertermine ändern.

*Dialogfenster "Lieferant und Liefertermine ändern". Sie können jetzt folgende Angaben ändern: den Lieferanten, den Liefertermin des Lieferanten, den Termin der Anlieferung beim Kunden.*

5.  Klicken Sie auf [OK], um die Änderung zu übernehmen.
    Der Dialog Lieferant und Liefertermine ändern wird geschlossen. Im Bestellpool wird die Auftragsposition mit dem neuen Termin und/oder Lieferanten angezeigt.
6.  Wählen Sie im Menü Start > Ausführen, um die Position an den Einkauf zu übergeben.
    Die aktivierten Prüfungen werden durchgeführt. Dies kann je nach Anzahl der Aufträge einige Momente dauern. Bestätigen Sie die jeweiligen Hinweise mit [Ja] oder [Nein], um die Prüfungen fortzusetzen. Wenn alle Prüfungen abgeschlossen sind, werden die zugehörigen Bestellungen angelegt und sind damit an den Einkauf übergeben.
    Die geänderten Termine werden in den Auftrag zurückgeschrieben.
    Nach der Übergabe der Positionen wird die Bestellnummer zum Auftrag angezeigt.
    Die erzeugte Bestellung können Sie unter **Dokumente > Bestellung** öffnen und weiterbearbeiten. Drucken Sie die neue Bestellung und senden Sie sie an den Lieferanten.

#### Preise im Bestellpool vergleichen

Wenn zu einem Produkt mehrere Lieferanten hinterlegt sind, können Sie im Bestellpool die Preise vergleichen und einen anderen Lieferanten auswählen.

**So vergleichen Sie die Preise im Bestellpool**
1.  Wählen Sie Dokumente > Auftrag > Bestellübergabe.
2.  Stellen Sie die Aufträge in den Bestellpool.
    Dieser Vorgang ist in der vorausgegangenen Einheit beschrieben.
    ⇨ "Dokument in den Bestellpool stellen" auf Seite D-68
3.  Markieren Sie die Position, zu der Sie die EK-Preise vergleichen wollen.
    Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf.

*Abb. D-39: Position für den Preisvergleich markiert. Nur die Positionen sind markiert, die mit einem X gekennzeichnet sind.*

4.  Wählen Sie im Menü Funktionen > Lieferantenpreise.

*Abb. D-40: Preisvergleich für Position. Der Dialog zeigt einen Preisvergleich verschiedener Lieferanten für eine Position. Die Textfarbe signalisiert den Status: (A) !!! Liefertermin gefährdet, (B) Rot: Standard-Lieferant, (C) Grün: preisgünstigster Lieferant, (D) Blau: Standard-Lieferant ist preisgünstigster Lieferant.*

5.  Markieren Sie die Checkbox links des Lieferanten, an den die Bestellung der Position gesendet werden soll.
6.  Klicken Sie auf [OK], um die Änderung zu übernehmen.
    Der Dialog Preisvergleich wird geschlossen. Im Bestellpool wird die Auftragsposition mit dem neuen Lieferanten angezeigt.
7.  Markieren Sie die Aufträge oder Auftragspositionen, die Sie an den Einkauf übergeben möchten.
    Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf.

*Abb. D-41: Position mit geändertem Lieferanten. Nur die Positionen sind markiert, die mit einem X gekennzeichnet sind.*

8.  Wählen Sie im Menü Start > Ausführen, um die Übergabe zu starten.
    Die aktivierten Prüfungen werden durchgeführt. Dies kann je nach Anzahl der Aufträge einige Momente dauern. Bestätigen Sie die jeweiligen Hinweise mit [Ja] oder [Nein], um die Prüfungen fortzusetzen. Wenn alle Prüfungen abgeschlossen sind, werden die zugehörigen Bestellungen angelegt und sind damit an den Einkauf übergeben.
    Übergebene Positionen werden aus dem Bestellpool gelöscht.

*Abb. D-42: Bestellnummern nach der Übergabe. Nach der Übergabe werden die neue (B) und die alte (A) Bestellnummer zum Auftrag angezeigt.*

Die Bestellungen können Sie unter **Dokumente > Bestellung** öffnen und weiterbearbeiten. Drucken Sie die neue Bestellung und senden Sie sie an den Lieferanten.
Vergessen Sie nicht, den alten Lieferanten über die Änderung zu informieren.

#### Auftrags- und Bestell-Info

Zu jedem Auftrag und zu jeder Bestellung können die referenzierten Dokumente in einer Übersicht angezeigt werden. Diese Funktion steht in der Bestellung (Kopfdaten) über das Menü **Funktion > Auftrags-/Bestell-Info** zur Verfügung.

*Abb. D-43: Auftrags- und Bestellinfo – Übersicht über die referenzierten Dokumente. Zwei Screenshots zeigen den Dialog "Auftrags-/Bestell-Info", einmal aus Sicht des Auftrags und einmal aus Sicht der Bestellung, mit den jeweils verknüpften Dokumenten.*

Dieser Dialog ist im Part Verkauf beschrieben.
⇨ Verkauf, "Auftrags-/Bestell-Info" auf Seite C-574

### Manuelle Bestellung

#### Lernziele
*   Bestellung manuell erfassen.
*   Dokumententyp Lagerbestellung kennenlernen.

#### Nutzen
*   Lagerbestellungen werden für die Bestandspflege im Lager erfasst. Sie können neben den Lagerartikeln auch Artikel enthalten, die nicht als Bestand im Lager gepflegt werden.

#### Merke
| Begriff | Erklärung |
| :--- | :--- |
| **Manuelle Bestellung** | Bestellungen, die nicht durch die Bestellübergabe aus einer Auftragsposition erzeugt werden, müssen manuell erfasst werden. |
| **Unabhängige Bestellung** | In unabhängigen Bestellungen können Sie sämtliche Produkte erfassen, die eingekauft werden können. Unabhängige Bestellungen beziehen sich nicht auf einen Auftrag. |
| **Lagerbestellungen** | Lagerbestellungen sind ein eigener Dokumententyp. Sie dienen dazu, den Lagerbestand aufzufüllen. |
| **Voreinstellungen** | **Stammdaten:**<br>- Lieferantenkartei<br>- Lieferanten (Register Auftrag, Finanzen, Saldo)<br>**Firmendaten:**<br>- Register Parameter<br>- Register Lager/EK/EDI |

#### Unabhängige Bestellungen

Alle Bestellungen zu Produkten, die nicht das Bestellkennzeichen `Bestellung` oder `Bestellung (komplett)` haben und nicht aus einem Auftrag heraus erzeugt werden, müssen manuell erfasst werden.

Als Bestellung können Sie alle Produkte erfassen, die zur Produktion oder zum Verkauf benötigt werden. Dabei wird unterschieden, ob Sie Artikel bestellen, die als Lagerware verbucht werden können oder solche, die zwar im Lager vorgehalten, jedoch nicht in den Bestandslisten geführt werden. Bestellungen von Lagerartikeln und Kisten müssen mit dem Dokumententyp `Lagerbestellung` erfasst werden, damit der Wareneingang korrekt verbucht werden kann.

Wenn Sie für Ihre Lieferanten entsprechende Konditionen hinterlegen, werden in den Bestellungen sofort die aktuellen EK-Preise ausgewiesen. Diese dienen zur Kontrolle von Preisen in Auftragsbestätigungen (AB) und Rechnungen Ihrer Lieferanten.

**Lagerbestellungen**
Lagerbestellungen werden als eigener Dokumententyp erfasst und können als Positionen alle Zukaufartikel, Lagermaße, Kisten und Sondergrößen enthalten, die als Lagerartikel geführt werden. Die Wareneingänge von Lagerartikeln aus Lagerbestellungen werden direkt in den Lagerbestand gebucht.

Wenn Sie Lagerbestellungen mit Positionen erfassen, die nicht als Lagerartikel geführt werden, werden diese im Wareneingang nicht angezeigt. Sie können in den Firmendaten jedoch die entsprechende Option aktivieren.

Die Lagerbestellungen sind ausführlich im Part Lagerwirtschaft beschrieben.

**Einkaufspreise**
Der EK wird aus den Preislisten für den Einkauf herangezogen. Bei der Erfassung von Bestellpositionen werden die entsprechenden Preise angezeigt und bei Änderungen aktualisiert.

#### Unabhängige Bestellung erfassen

Sie können in einer unabhängigen Bestellung alle Produkte erfassen, die in den Stammdaten hinterlegt sind.

> **Arbeiten mit Nummernverwaltern**
> Richten Sie sich für die Bestellungen die Nummernverwalter so ein, dass die Dokumente nach eindeutigen Kriterien zusammengefasst werden, z. B. nach Lieferanten, nach Datum, nach Lagerbestellungen, nach komplett gelieferten Bestellungen.

**So erfassen Sie eine unabhängige Bestellung**
1.  Wählen Sie Dokumente > Bestellung > Bestellung.
    Der Dialog Dokumentenverwaltung wird geöffnet.
    ⇨ Verkauf, "Dokument - Kopfdaten" auf Seite C-424
2.  Prüfen Sie im Menü Funktionen > NV Auswahl, ob der richtige Nummernverwalter eingestellt ist, und korrigieren Sie ggf. die Einstellung.
3.  Erfassen Sie den Dokumentenkopf, indem Sie den Lieferanten auswählen.

*Abb. D-44: Unabhängige Bestellung erfassen. Der Screenshot zeigt den Kopf einer neuen Bestellung mit Feldern für den Termin der Anlieferung (A) und den Dokumententyp (B).*

4.  Prüfen Sie den Termin für die Anlieferung (A).
    Dies ist der Termin, zu dem Sie die Lieferung bei sich erwarten.
5.  Wählen Sie im Feld Typ (B) den Eintrag `<k.A.>`.
    Wenn Sie den Typ auf `<k.A.>` einstellen, wird der Wareneingang nicht auf das Lager gebucht.
    Die Lagerbestellung ist in einer separaten Einheit beschrieben.
    ⇨ "So erfassen Sie eine Lagerbestellung mit Kisten" auf Seite D-83
6.  Erfassen Sie die Positionen, wie im Kapitel Bestellpositionen im Auftrag beschrieben.
    ⇨ "So erfassen Sie im Auftrag eine Position zur Bestellung" auf Seite D-54
7.  Drucken und versenden Sie die Bestellung.
    Die Bestellung steht nun in dem von Ihnen bestimmten Nummernverwalter. Zu ihr kann später eine Auftragsbestätigung vom Lieferanten und/oder ein Wareneingang erfasst werden.
    ⇨ "Wareneingang erfassen" auf Seite D-127

#### Lagerbestellung erfassen

Sie können in einer Lagerbestellung auch Artikel bestellen, die nicht als Lagerartikel verbucht werden können. Ein Hinweis macht Sie beim Speichern auf solche Bestellpositionen aufmerksam. Diese Artikel werden beim Wareneingang jedoch nicht automatisch als Lagerbestand verbucht.

In der nachfolgenden Handlungsanleitung wird eine Lagerbestellung für Kisten erfasst. Diese Kistenbestellungen können in der Themenblock Kistengeschäft dann weiterbearbeitet werden.

**So erfassen Sie eine Lagerbestellung mit Kisten**
1.  Erfassen Sie das Dokument, wie im Abschnitt Unabhängige Bestellung beschrieben.
    ⇨ "So erfassen Sie eine unabhängige Bestellung" auf Seite D-81
2.  Wählen Sie im Feld Typ den Eintrag `Lagerbestellung`.

*Screenshot-Ausschnitt zeigt das Typ-Feld mit der ausgewählten Option "Lagerbestellung".*

    Wenn Sie den Typ auf `<k.A.>` einstellen, können Sie den Wareneingang nicht automatisch auf das Lager buchen.
3.  Wechseln Sie zum Register Positionen.
4.  Geben Sie die Produktnummer ein, z. B. 1005.
    Die Anzahl können Sie nach der Auswahl des Lagerartikels angeben. Maße brauchen Sie nicht einzutragen, diese werden aus dem Lagerartikel übernommen.
5.  Wählen Sie im Menü Start > Lagersuche, um den Dialog Lagerinfo zu öffnen.
    Sie können den Dialog auch über die Taste <F3> öffnen.

*Abb. D-45: Lagerinfo - Lagersuche. Der Dialog zeigt eine Liste von Lagerartikeln. (A) Produktnummer der Glasart. (B) Kiste ohne Identnummer, erkennbar an einem Inhalt > 1.*

    ⇨ Verkauf, "Lagerinfo" auf Seite C-758
    Der Dialog Lagerinfo wird mit einer Liste aller Lagermaße und Kisten angezeigt. Für Kisten ist in der Spalte `Inh.` der Wert größer als 1.
6.  Suchen Sie die gewünschte Kiste ohne Kisten-ID aus und übernehmen Sie sie mit einem Doppelklick.
    Der Dialog wird geschlossen und die Positionserfassung wird wieder angezeigt. In der Erfassungszeile werden für Kisten alle Felder ab `Menge` gesperrt. Die Preisfelder werden aktualisiert.

*Abb. D-46: Kiste in der Positionserfassung. Der Screenshot zeigt eine erfasste Kistenposition in der Bestellmaske. Die Stückzahl (A) kann eingegeben werden, die Menge (B) ist automatisch berechnet.*

7.  Geben Sie die gewünschte Stückzahl ein.
    Die Anzeige der Details wird aktualisiert.
8.  Wiederholen Sie die Schritte 4 bis 7, um alle Bestellpositionen zu erfassen.
9.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Daten werden gespeichert.
10. Drucken und versenden Sie die Bestellung.

### Auftragsbestätigung des Lieferanten

#### Lernziele
*   Auftragsbestätigung (AB) eines Lieferanten erfassen.
*   AB pro Position erfassen.
*   Preise in der AB prüfen.
*   Ausstehende Auftragsbestätigungen anmahnen.

#### Nutzen
*   Die Auftragsbestätigung des Lieferanten wird der Bestellung zugeordnet. Dabei wird der Liefertermin bestätigt oder angepasst, ohne die Bestellung selbst öffnen zu müssen. Die Terminänderungen werden in die referenzierten Dokumente übernommen.
*   Der Status von referenzierten Aufträgen wird automatisch zusammen mit dem Status der Bestellung umgesetzt.
*   AB für Teilmengen können erfasst werden, ohne die Daten neu einzugeben.
*   Überfällige Bestellungen können aus einem Nummernverwalter herausgefiltert werden, um den jeweiligen Lieferanten anzumahnen.

#### Merke
| Begriff | Erklärung |
| :--- | :--- |
| **Teilweise Bestätigung** | Wenn Ihr Lieferant die bestellte Menge in verschiedenen Untermengen bestätigt, können Sie die Auftragsbestätigung (AB) zu einzelnen Positionen oder Teilmengen erfassen. |
| **Status** | Der Status der referenzierten Dokumente wird hochgesetzt, wenn Sie in einem der Dokumente die Auftragsbestätigung des Lieferanten erfassen. |
| **Dokumentensperre** | Während der Preis- und Rechnungsprüfung sind die referenzierten Dokumente für den Zugriff durch andere Mitarbeiter gesperrt. |
| **Mahnung senden** | Die Mahnung wird auf demselben Kommunikationsweg an einen Lieferanten gesendet, wie die Bestellung. |
| **Voreinstellungen** | **Lieferantenstammdaten:**<br>- Fax- und E-Mail-Versand |

#### Lieferanten-AB

Ihr Lieferant bestätigt die eingegangene Bestellung durch eine Auftragsbestätigung (AB). Die Nummer dieser Auftragsbestätigung können Sie erfassen und der entsprechenden Bestellung zuordnen. Gleichzeitig können Sie die Termine und Preise prüfen und ggf. in Ihren Dokumenten anpassen.

Beim Erfassen einer Auftragsbestätigung haben Sie die Möglichkeit, die Bestellung und/oder den zugehörigen Kundenauftrag zur weiteren Bearbeitung in einen Ziel-Nummernverwalter zu verschieben.

**Teillieferungen**
Bei größeren Bestellungen kann es vorkommen, dass Ihr Lieferant nicht alle Positionen oder die gesamte Stückzahl zum gewünschten Termin bestätigt, sondern in mehreren Teillieferungen ankündigt. Sie können dann auch eine Teilmenge der Bestellung bestätigen, ohne ein neues Dokument erfassen zu müssen.

**Status**
Der Status aller referenzierten Dokumente wird umgesetzt, sobald die AB-Nummer bestätigt wurde. Die referenzierten Dokumente werden angezeigt, sobald die Auftrags- oder der Bestellnummer eingegeben wurde. Bei unabhängigen Bestellungen bleiben die entsprechenden Felder gesperrt.

**Auftragsbestätigung und Liefertermin**
Die AB des Lieferanten kann auf unterschiedliche Weise erfasst werden:
*   Auftragsbestätigung mit oder ohne Wareneingang. Dabei können Sie die Termine für die Lieferung prüfen und ggf. den Kunden über eine Verschiebung benachrichtigen.
*   Bestätigung einzelner Positionen einer Bestellung.
*   Auftragsbestätigung und Preiskontrolle. Dabei können Sie die Einkaufspreise und den Liefertermin prüfen und korrigieren und ggf. eine Teillieferung zur bestellten Menge erfassen. Die Beschreibung dieser Variante finden Sie unter.
    ⇨ "Preis- und Rechnungskontrolle" auf Seite D-143

Aus einem Kundenauftrag können mehrere Bestellungen an unterschiedliche Lieferanten erzeugt werden. Die verschiedenen AB-Nummern werden für die entsprechenden Auftragspositionen gespeichert.

#### Überfällige Lieferungen

Sie können überfällige Auftragsbestätigungen oder Lieferungen anmahnen. Die Suche nach offenen Bestellungen kann durch ein Datum, auf bestimmte Lieferanten und/oder Nummernverwalter eingeschränkt werden.

Für die Mahnung müssen Sie denselben Kommunikationsweg wählen, über den Sie auch die Bestellungen an den jeweiligen Lieferanten übermitteln. Dabei gilt:
*   **Faxversand:** Die Bestellungen werden aus A+W Business direkt auf ein Faxgerät gesendet und an den Lieferanten übermittelt.
*   **Postversand:** Die Bestellungen werden aus A+W Business direkt auf einen Drucker gesendet.

Die Mahnung wird immer für alle Bestellungen erstellt, die anhand der Suchkriterien ausgewählt wurde. Dabei werden die Bestellungen pro Lieferant zu einer Mahnung zusammengefasst.

#### Auftragsbestätigung erfassen

Zu einer Bestellung erfassen Sie die Auftragsbestätigung (AB) Ihres Lieferanten und setzen damit den Status der Bestellung hoch.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So erfassen Sie die Auftragsbestätigung für eine Bestellung insgesamt" auf Seite D-89
*   "So erfassen Sie die Auftragsbestätigung für eine Bestellposition" auf Seite D-91

**So erfassen Sie die Auftragsbestätigung für eine Bestellung insgesamt**
1.  Wählen Sie Dokumente > Bestellung > AB Lieferant.

*Abb. D-47: AB des Lieferanten erfassen. Der Screenshot zeigt den Dialog "AB Lieferant" mit Optionen für die Suche (A) nach Bestellnummer oder Auftragsnummer (B).*

    ⇨ Softwarereferenz, "AB-Lieferant" auf Seite D-197
2.  Wählen Sie die Option (A), mit der Sie die Suche nach offenen Bestellungen starten möchten, z. B. Bestellnummer.
3.  Tragen Sie die Bestellnummer (B) ein und springen Sie mit `<Tab>` in das nächste Feld.
    Die Daten werden eingelesen und angezeigt.

*Abb. D-48: AB-Lieferant - Dokumente. Die AB-Daten werden angezeigt, mit Optionen zur Weiterverarbeitung: (A) Ziel-Nummernverwalter, (B) Wareneingang komplett buchen, (C) Anliefertermin aus der AB, (D) Nummer der AB.*

4.  Wählen Sie den Ziel-Nummernverwalter (A) für Aufträge oder für Bestellungen, wenn die entsprechenden Dokumente in andere Nummernverwalter gestellt werden sollen.
5.  Markieren Sie die Checkbox **Wareneingang buchen** (B) nur, wenn Sie gleichzeitig den gesamten Wareneingang dieser Bestellung verbuchen möchten.
    Mit dieser Einstellung können Sie keinen teilweisen Wareneingang erfassen. Der Wareneingang ist in einer separaten Einheit beschrieben.
    ⇨ "Wareneingang erfassen" auf Seite D-127
6.  Prüfen Sie die Termine (C) in den Bereichen Bestelldaten und Auftragsdaten und korrigieren Sie diese ggf.
7.  Tragen Sie die Nummer der Auftragsbestätigung (D) ein, die der Lieferant Ihnen geschickt hat.
8.  Wählen Sie im Menü Start > Ausführen, um die Daten zu speichern.
    Die Daten werden gespeichert. Die AB-Nummer wird in der Übersicht angezeigt.
    Wenn Sie gleichzeitig einen Wareneingang gebucht haben, wird der Status der Bestellung entsprechend umgesetzt.

**So erfassen Sie die Auftragsbestätigung für eine Bestellposition**
1.  Füllen Sie die Felder wie in Schritt 2 bis 6 der vorigen Handlungssequenz beschrieben.
2.  Wechseln Sie zum Register Positionen.

*Abb. D-49: AB-Lieferant – Positionen. Der Screenshot zeigt das Register "Positionen" zum Erfassen einer AB für einzelne Positionsnummern (A) mit einem spezifischen Termin (B).*

3.  Tragen Sie die Nummer(n) der Positionen (A) ein, für die Sie die AB erhalten habe.
    Wenn Sie keine lückenlose Folge von Nummern haben, müssen Sie die Schritte für jede Position einzeln wiederholen, z. B. für Position 1, 3 und 7.
4.  Tragen Sie im Feld **Teilliefertermin** das Datum für die Lieferung der Positionen ein.
5.  Wählen Sie im Menü Start > Ausführen, um die Daten zu speichern.

*Abb. D-50: AB-Lieferant - Teillieferung. Nach dem Speichern werden die AB-Nummer (A) und der bestätigte Termin (B) in der Übersicht angezeigt.*

Die Daten werden gespeichert. Die Nummer der AB und der Teilliefertermin werden in der Übersicht angezeigt.

### AB erfassen und Preise prüfen

Die Preise können sowohl auf Basis der Auftragsbestätigung des Lieferanten als auch auf Basis der Lieferantenrechnung geprüft werden. Die Dialoge Preiskontrolle und Rechnungskontrolle sind identisch aufgebaut.

Ihr Lieferant kann in einer AB mehrere Bestellungen bestätigt haben. Diese können Sie im Dialog Preiskontrolle sammeln und gemeinsam kontrollieren.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So erfassen Sie eine Lieferanten-AB und prüfen die Preise" auf Seite D-93
*   "So erfassen Sie eine Sammel-AB Ihres Lieferanten" auf Seite D-95

Die Preis- und Rechnungskontrolle ist ausführlich in einer separaten Einheit beschrieben.
⇨ "Rechnung kontrollieren" auf Seite D-146

**So erfassen Sie eine Lieferanten-AB und prüfen die Preise**
1.  Wählen Sie Dokumente > Bestellungen > Auftragsbestätigung > Preiskontrolle.

*Abb. D-51: AB-Nummer des Lieferanten erfassen und Preise prüfen. Der Screenshot zeigt den Dialog "Auftragsbestätigung - Preiskontrolle". (A) Daten aus der AB, (B) Bestätigte Summe, (C) Anzeigemodus, (D) Suche nach Bestellung(en).*

    ⇨ Softwarereferenz, "Rechnungskontrolle - Bestellungen" auf Seite D-248
2.  Geben Sie die Nummer der Auftragsbestätigung (A) Ihres Lieferanten und den bestätigten Anliefertermin ein.
3.  Geben Sie die Bestellnummer (D) ein und springen Sie mit `<Tab>` in das nächste Feld.
    In der Übersicht Bestellungen wird die Bestellung angezeigt.
    Wenn in der AB mehrere Bestellungen zusammengefasst sind, können Sie nacheinander alle Bestellnummern angeben. Dies ist in der nachfolgenden Handlungssequenz beschrieben.
4.  Geben Sie im Feld **AB-Summe** (B) den Betrag ein, den Ihr Lieferant bestätigt hat.
    Der Betrag muss identisch mit dem aus der Bestellung angezeigten Betrag sein. Wenn der Lieferant einen anderen Betrag angegeben hat, den Sie akzeptieren wollen, müssen Sie die Preise in der Bestellung ändern. Sie können diese Änderung im Register Positionen erfassen.
    Achten Sie darauf, dass der Modus (C) für die Anzeige der Beträge richtig eingestellt ist.

> **Währung**
> Wenn Sie nur mit einer Währung (EUR) arbeiten, muss im Feld Kurs 1 eingetragen sein.

*Abb. D-52: AB-Nummer des Lieferanten erfassen und Preise prüfen. Die Felder AB-Summe (A) und der Betrag aus der Bestellung (B) werden angezeigt.*

5.  Wählen Sie im Menü Start > Ausführen, um die Eingabe zu bestätigen.
    Der Betrag wird geprüft und das Register Positionen wird angezeigt.

*Abb. D-53: Preise der Bestellpositionen prüfen. Im Register Positionen werden die Preise (A) der einzelnen Positionen angezeigt. Eine eventuelle Differenz (B) wird unten ausgewiesen.*

    Wenn Sie einen Positionspreis ändern müssen, überschreiben Sie den Betrag in der entsprechenden Position (A). Diese Änderung wird in die Bestellung zurückgeschrieben.
6.  Wählen Sie im Menü Start > Ausführen, wenn keine Differenz (mehr) angezeigt wird (B).
    Die Daten werden gespeichert und der Status der Bestellung wird umgesetzt. Anschließend wird das Register Bestellungen wieder angezeigt und Sie können die nächste AB erfassen. Die Preiskontrolle für diese Bestellung kann nicht nochmals durchgeführt werden.

**So erfassen Sie eine Sammel-AB Ihres Lieferanten**

> **Bestellungen sammeln**
> Sie können die Bestellungen, die in der AB des Lieferanten aufgeführt sind, in einem Nummernverwalter sammeln und diesen im Bereich Bestelldaten auswählen.
> Alternativ dazu können Sie die Bestellungen im Dialog Preiskontrolle sammeln. Dieses Vorgehen ist in den nachfolgenden Handlungsschritten beschrieben.

1.  Geben Sie im Dialog Preiskontrolle die Nummer der Auftragsbestätigung Ihres Lieferanten und den Anliefertermin ein, wie oben beschrieben.
    Wenn Sie die Bestellungen in einem Nummernverwalter gesammelt haben, so wählen Sie diesen aus und fahren mit Schritt 5 fort.
2.  Geben Sie die Nummer der ersten Bestellung ein und warten Sie, bis diese eingelesen wurde.
3.  Geben Sie nun die Nummer der nächsten Bestellung ein, die auf der AB aufgeführt ist.
    Die Bestellung wird in der Übersicht der Bestellungen hinzugefügt. Sie können jedoch nur Bestellungen mit identischem Steuersatz zusammenfassen.
4.  Wiederholen Sie diesen Schritt, bis alle Bestellungen in der Übersicht aufgeführt sind.
    Sie können eine Bestellung aus der Übersicht wieder entfernen, indem Sie den Eintrag markieren und auf `<Entf>` drücken.

*Abb. D-54: AB-Nummer des Lieferanten erfassen und Preise prüfen. Der Screenshot zeigt, wie mehrere Bestellungen für eine Sammel-AB zusammengefasst werden.*

5.  Geben Sie den Betrag ein, den Ihr Lieferant bestätigt hat.
    Der Betrag muss identisch mit der Summe der aufgeführten Bestellungen sein.
6.  Wählen Sie im Menü Start > Ausführen, um die Eingabe zu bestätigen.
    Der Betrag wird geprüft und das Register Positionen wird angezeigt. Wenn Sie einen Positionspreis ändern müssen, überschreiben Sie den Betrag in der entsprechenden Position. Diese Änderung wird in die Bestellung zurückgeschrieben.
7.  Wählen Sie im Menü Start > Ausführen, wenn keine Differenzen (mehr) angezeigt werden.
    Die Daten werden gespeichert und der Status der Bestellungen wird umgesetzt.

#### Lieferanten anmahnen

Für die korrekte Verarbeitung Ihrer Bestellungen werden Auftragsbestätigungen und Lieferungen erfasst. Säumige Lieferanten können Sie anmahnen.

> **Bestellungen sammeln**
> Sie können die Bestellungen, die in der AB des Lieferanten aufgeführt sind, in einem Nummernverwalter sammeln.

**So mahnen Sie einen Lieferanten an**
1.  Wählen Sie Dokumente > Bestellungen > Auftragsbestätigung > Mahnung.

*Abb. D-55: Lieferanten mahnen. Der Dialog "Mahnung" ermöglicht die Auswahl von Bestellungen nach Lieferant (A), Nummernverwalter (B), Statusbereich (C), Datum (E) und Versandweg (F). Die Option (D) erlaubt es, bereits gemahnte Lieferanten erneut zu mahnen.*

    ⇨ Softwarereferenz, "Mahnung" auf Seite D-225
2.  Filtern Sie die Anzeige:
    *   nach Lieferanten (A)
    *   nach einem Nummernverwalter (B)
3.  Wählen Sie in den Feldern Mindeststatus und Status kleiner (C) einen Statusbereich für die Bestellungen aus, deren Lieferung Sie anmahnen wollen.
    Ein Kriterium für den Mindeststatus könnte sein, dass die Bestellung gedruckt wurde oder dass die AB erfasst wurde.
    Ein Kriterium für den anderen Status sollte vor dem Status `Wareneingang erfasst` liegen.
4.  Grenzen Sie die Auswahl der Bestellungen auf ein Datum (E) ein.
    Standardmäßig wird das aktuelle Tagesdatum angezeigt.
5.  Wenn Sie die bereits gemahnten Lieferanten nicht nochmals mahnen wollen, deaktivieren Sie die Checkbox (D) für dieses Kriterium.
    Die bereits gemahnten Lieferanten werden dann in der Trefferliste nicht angezeigt. Wenn die Checkbox markiert ist, werden diese Lieferanten in roter Schrift angezeigt. Die ausstehenden Lieferungen werden dann nochmals angemahnt.
6.  Wählen Sie die Option (F) aus, mit der Sie Bestellungen gesendet haben.
    Wenn Sie die Bestellungen an Ihre Lieferanten auf unterschiedliche Weise senden, beachten Sie den Kommunikationsweg für den ausgewählten Lieferanten.
    Die Option Alle ist dann sinnvoll, wenn Sie die Bestellungen auf unterschiedliche Arten an die Lieferanten senden und die Auswahl auf keinen bestimmten Lieferanten eingeschränkt haben.
7.  Wählen Sie im Menü Start > Suchen, um in die Suche zu starten.

*Abb. D-56: Lieferanten zur Mahnung ausgewählt. Die Übersicht zeigt die gefundenen überfälligen Bestellungen.*

    Die offenen Bestellungen werden in der Übersicht aufgelistet.
8.  Wählen Sie im Menü Drucken die gewünschte Ausgabeform.
    Die Mahnung wird erstellt.

*Abb. D-57: Mahnungen erstellt. Anschließend werden alle Einträge in der Übersicht in roter Schrift dargestellt.*

### Lieferterminkontrolle

#### Lernziele
*   Liefertermine zu referenzierten Dokumenten prüfen.
*   Termine ändern.
*   Kunde über die Änderung benachrichtigen.

#### Nutzen
*   In referenzierten Dokumenten brauchen Termine nur in einem Dokument geändert zu werden.
*   Liefertermine können in verschiedenen Dialogen geändert werden. Bestellungen oder Aufträge, die in einem eigenen Nummernverwalter gesammelt sind, können geändert werden, ohne die Dokumente selbst zu öffnen.

#### Merke
| Begriff | Erklärung |
| :--- | :--- |
| **Terminänderungen in referenzierten Dokumenten** | Alle Änderungen in Bestellungen werden in die referenzierten Aufträge zurückgeschrieben. Dies gilt auch in der entgegengesetzten Richtung. |
| **Dialog Kundenbenachrichtigung** | In diesem Dialog können Sie den Anliefertermin ändern und den Kunden benachrichtigen. |
| **Dialog Dokumentendaten** | In diesem Dialog können Sie alle Termine in den Aufträgen und referenzierten Bestellungen anpassen. Zusätzlich können Sie die Tour in Aufträgen und mehrere Dokumente gemeinsam ändern. |
| **Voreinstellungen** | Kundenstammdaten (Fax- oder Mail-Versand) |

#### Prüfung und Korrektur von Lieferterminen

Ihr Lieferant wird die Termine aus Ihren Bestellungen bestätigen oder korrigieren. Die vom Lieferanten erhaltenen Auftragsbestätigungen und Liefertermine ordnen Sie den Bestellungen zu, indem Sie die Lieferanten-AB erfassen. Dabei werden die geänderten Termine automatisch in die referenzierten Dokumente übernommen.

Für die Benachrichtigung des Kunden können Sie den Dialog Kundenbenachrichtigung oder die Möglichkeiten im Menü Kommunikation nutzen – oder einfach anrufen.

Den Liefertermin selbst können Sie in verschiedenen Dialogen ändern:
*   Dokumentenverwaltung (Auftrag, Bestellung)
*   Dokumentendaten
*   Kundenbenachrichtigung (Lieferterminkontrolle)
*   AB Lieferant
*   Eingangskontrolle

Sie korrigieren die Termine in aller Regel in den Bestellungen, wodurch sie in die referenzierten Aufträge zurückgeschrieben werden.

**Kundenbenachrichtigung**
Sie können den Kunden aus dem Dialog Kundenbenachrichtigung (Lieferterminkontrolle) heraus über die Terminverschiebung informieren. Dazu muss in den Stammdaten des Kunden eine E-Mail-Adresse hinterlegt sein. Im Auftrag muss im Bereich Anschrift die Checkbox Mail aktiviert sein.

#### Liefertermine ändern und Kunden benachrichtigen

Zu den Bestellungen und referenzierten Aufträgen müssen Sie Liefertermine prüfen, korrigieren und den ggf. den Kunden benachrichtigen, wenn die Termine nicht eingehalten werden können. Diese Schritte sind über den Dialog Kundenbenachrichtigung möglich.

Sie können ihn auf folgende Weise öffnen:
*   Auftrag oder Bestellung > Funktionen > Gruppe Dokument > Lieferterminkontrolle
*   Dokumente > Kundenbenachrichtigung

Wenn Sie auch die Termine für die Produktion prüfen und korrigieren wollen, können Sie den Dialog Dokumentendaten nutzen.
⇨ "So prüfen und ändern Sie die Dokumentendaten" auf Seite D-105

**So ändern Sie den Liefertermin**
1.  Öffnen Sie ggf. den Auftrag, dessen Termine Sie prüfen wollen oder geändert haben.
2.  Wählen Sie Dokumente > Kundenbenachrichtigung.

*Abb. D-58: Liefertermin beim Kunden ändern. Der Dialog "Kundenbenachrichtigung" zeigt eine Liste von Dokumenten mit ihrem geplanten Lieferdatum (B) an.*

    ⇨ Verkauf, "Kundenbenachrichtigung (Lieferterminkontrolle)" auf Seite C-577
3.  Wählen Sie die Option (A) `Aufträge` oder `Bestellungen` und ggf. den Nummernverwalter.
    Wenn in dem Nummernverwalter sehr viele Dokumente aufgelistet sind, können Sie die Anzeige auf das ursprünglich geplante Lieferdatum (B) einschränken.
4.  Wählen Sie im Menü Start > Suchen, um die Daten einzulesen.

*Abb. D-59: Liefertermine prüfen. Die Liste zeigt Aufträge, bei denen der Kunde noch nicht über einen neuen Termin informiert wurde (A). Angezeigt werden der geplante Liefertermin (B) und der neue Liefertermin (C).*

5.  Markieren Sie den Auftrag, zu dem Sie den Liefertermin beim Kunden ändern müssen, und wechseln Sie zum Register Terminverschiebung.

*Abb. D-60: Liefertermin beim Kunden ändern. Im Register "Terminverschiebung" kann ein neuer Termin (A) für den markierten Auftrag (B) eingegeben werden.*

6.  Markieren Sie den Auftrag (B), zu dem der Kundentermin verschoben werden muss.
    Sie können mehrere Aufträge markieren, wenn diese alle denselben Liefertermin und dieselbe Tour haben.
7.  Tragen Sie den neuen Termin (A) ein und ändern Sie ggf. die Tour.
8.  Wählen Sie im Menü Start > Speichern, um die Änderung zu speichern.
    Sie können die Terminänderung für den Kunden drucken und auf dem üblichen Kommunikationsweg versenden.
9.  Wählen Sie über das Menü Druck den Drucker aus.
    Die Benachrichtigung wird erzeugt und kann versendet werden. Wenn Sie mehrere Termine geändert haben, wird pro Kunde eine Benachrichtigung erstellt.

#### Alle Termine prüfen und ändern

Im Dialog Dokumentendaten können Sie sich alle Bestellungen und Aufträge anzeigen lassen, um neben den Lieferterminen auch die Produktionstermine zu prüfen und ggf. zu ändern. Wenn Sie in mehreren Aufträgen gemeinsam z. B. die Termine ändern wollen, können Sie die Aufträge sammeln.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So prüfen und ändern Sie die Dokumentendaten" auf Seite D-105
*   "So sammeln Sie Dokumente für gemeinsame Änderungen" auf Seite D-108

**So prüfen und ändern Sie die Dokumentendaten**
1.  Wählen Sie Dokumente > Dokumentendaten.
    ⇨ Verkauf, "Dokumentendaten" auf Seite C-755

*Abb. D-61: Termine für Auftrag mit Bestellpositionen prüfen. Der Dialog "Dokumentendaten" ermöglicht die Suche nach Dokumententyp (A) und Nummer (B).*

2.  Wählen Sie den Dokumententyp, z. B. Auftrag oder Bestellung.
    Sie können sich auch alle Aufträge in einem Nummernverwalter anzeigen lassen. In diesem Beispiel soll ein einzelner Auftrag geprüft werden.
    Sie können die Termine für mehrere Aufträge und/oder Bestellungen ändern, die nicht in einem gemeinsamen Nummernverwalter stehen.
    ⇨ “So sammeln Sie Dokumente für gemeinsame Änderungen" auf Seite D-108
3.  Geben Sie die Auftragsnummer ein und übernehmen Sie die Daten mit `<Enter>`.

*Abb. D-62: Termine für Auftrag mit Bestellpositionen prüfen. Die Daten des Auftrags (A) und der zugehörigen Bestellung (B) werden angezeigt.*

    In den Feldern im Bereich Auftrag werden die Daten aus dem Auftragskopf angezeigt. In den Feldern im Bereich Bestellung werden die Daten aus der Bestellung angezeigt.
4.  Passen Sie den Lieferantentermin (B) und die Kundentermine (A) an.
    Wenn Sie die Termine über den Kalender auswählen, können Sie die Tourentage für den Kunden berücksichtigen.
5.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die neuen Termine werden gespeichert und in die zugehörigen Dokumente übernommen.

*Abb. D-63: Geänderte Termine. Sie können jetzt den Kunden über den geänderten Termin informieren.*

**So sammeln Sie Dokumente für gemeinsame Änderungen**
1.  Wählen Sie Dokumente > Dokumentendaten.

*Abb. D-64: Termine für Auftrag mit Bestellpositionen prüfen. Um Dokumente zu sammeln, wird der Dokumententyp (A) ausgewählt und die Nummer (B) eingegeben, während die Checkbox für den Nummernverwalter (C) deaktiviert ist.*

2.  Wählen Sie den Dokumententyp aus, z. B. Auftrag (A).
3.  Stellen Sie sicher, dass die Checkbox (C) `Nummernverwalter` nicht markiert ist.
4.  Geben Sie die Auftragsnummer (B) ein und übernehmen Sie die Daten mit `<Enter>`.
    In der Übersicht werden die Daten des Auftrags angezeigt. Im Bereich Bestellung werden die referenzierten Bestellungen aufgelistet.
5.  Wiederholen Sie diesen Schritt, bis Sie alle Aufträge zusammengestellt haben, die Sie gemeinsam ändern wollen.
    Achten Sie darauf, dass alle Aufträge mit derselben Tour geliefert werden können und dasselbe Lieferdatum haben.

*Abb. D-65: Aufträge für gemeinsame Terminänderung. Mehrere Aufträge (A) mit ihren zugehörigen Bestellungen (B) sind für eine gemeinsame Änderung in der Übersicht gesammelt.*

    In der Übersicht werden alle Aufträge aufgelistet.
6.  Markieren Sie alle aufgelisteten Aufträge, indem Sie die `<Strg>`-Taste gedrückt halten.
7.  Ändern Sie die Termine (A, B).
8.  Prüfen Sie die Tour und ändern Sie diese ggf.
9.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die neuen Termine werden in alle aufgelisteten Aufträge und referenzierten Bestellungen übernommen. Sie können jetzt die Kunden benachrichtigen.

### Anfrage

#### Lernziele
*   Anfragen beim Lieferanten einholen.
*   Aus einer Anfrage eine Bestellung erzeugen.
*   Anfragen zu einer Bestellposition einholen.

#### Nutzen
*   Anfragen können zur Abstimmung von Terminen und Kapazitäten über den Bestellpool erzeugt werden.
*   Aus einer Anfrage kann eine Bestellung erzeugt werden, ohne die Daten neu zu erfassen.

#### Merke
| Begriff | Erklärung |
| :--- | :--- |
| **Anfragen** | Wie bei den Bestellungen können Anfragen manuell erfasst oder über den Bestellpool aus einem Kundenauftrag heraus erzeugt werden. |
| **Bestellung** | Aus jeder Anfrage kann eine Bestellung erzeugt werden. |
| **Referenzen** | Die Referenz auf eine Auftragsposition bleibt in der Anfrage und in der Bestellung erhalten, wenn sie über den Bestellpool erzeugt werden. Wenn die Bestellung durch Kopieren aus einer Anfrage erzeugt wird, besteht die Referenz nur zwischen diesen beiden Dokumenten. |
| **Voreinstellungen** | **Stammdaten:**<br>- Lieferant > Register Auftrag |

#### Anfrage zu Bestellpositionen oder Bestellungen

Anfragen erstellen Sie genau wie eine Bestellung und senden Sie an den Lieferanten. Wenn das Angebot zurückkommt und angenommen werden soll, können Sie aus der Anfrage eine Bestellung erzeugen, ohne die Daten erneut eingeben zu müssen. Dazu nutzen Sie die Funktion Dokument kopieren.

Anfragen können Sie auch zu den Bestellpositionen aus einem Kundenauftrag erstellen.

*Abb. D-66: Anfrage - Bestellung. Ein Flussdiagramm zeigt die verschiedenen Wege, wie aus einem Auftrag (Nr. 1167) über eine Anfrage eine Bestellung erstellt werden kann, entweder mit oder ohne Referenz auf den ursprünglichen Auftrag.*

Wenn bei der Bestellübergabe die Option **Sofort Anfragen** gewählt wurde, werden auch aus einem Kundenauftrag Anfragen erzeugt. Wenn Sie dabei über den Bestellpool gehen, könne Sie auch zu einzelnen Auftragspositionen eine Anfrage erstellen und einen bestimmten Lieferanten auswählen.

Aus so erstellen Anfragen können natürlich auch Bestellungen erzeugt werden. Die Referenz zum Auftrag bleibt jedoch nur erhalten, wenn entsprechenden Bestellungen wieder über den Bestellpool erzeugt werden.

Unabhängige Anfragen werden analog zu Aufträgen und Bestellungen erzeugt. Dazu steht im Modul Dokumente das Menü Anfragen zur Verfügung.

### Anfrage zu einer Bestellposition erzeugen

Sie können zu einer Bestellposition zunächst eine Anfrage erzeugen, z. B., um festzustellen, ob der Lieferant die Kapazitäten frei hat. Aus jeder Anfrage kann über den Bestellpool auch eine Bestellung erzeugt werden.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So erzeugen Sie eine Anfrage zu einem Kundenauftrag" auf Seite D-112
*   "So erstellen Sie zu einer referenzierten Anfrage eine Bestellung" auf Seite D-113

**So erzeugen Sie eine Anfrage zu einem Kundenauftrag**
1.  Wählen Sie Dokumente > Auftrag > Bestellübergabe.

*Abb. D-67: Aufträge aus dem Nummernverwalter übergeben. Der Dialog zeigt den Modus "Sofort anfragen" (A), den Quell-Nummernverwalter (B) und den Ziel-Nummernverwalter (C).*

2.  Wählen Sie die den Modus **Sofort anfragen** (A) und den Nummernverwalter (B), in dem Sie die Aufträge mit Bestellpositionen gesammelt haben.
3.  Wählen Sie den Ziel-Nummernverwalter (C) aus, in den die Anfragen gestellt werden.
    Sie können einen neuen Namen eingeben und so einen neuen Nummernverwalter anlegen. Wenn Sie dazu einen anderen Mitarbeiter auswählen, wird der Nummernverwalter diesem zugeordnet.
4.  Wählen Sie ggf. im Bereich Ziel-Nummernkreis den Mandanten und den AV-Bereich aus.
5.  Wählen Sie im Menü Start > Ausführen, um die Positionen zu übergeben.
    Bestätigen Sie die Erfolgsmeldung.
    Für jede Bestellposition wurde eine Anfrage erzeugt. Die erzeugten Anfragen können Sie unter Dokumente > Anfrage öffnen, drucken und an den Lieferanten senden.

**So erstellen Sie zu einer referenzierten Anfrage eine Bestellung**
1.  Öffnen Sie den Dialog Bestellübergabe.

*Abb. D-68: Aufträge aus dem Nummernverwalter übergeben. Der Screenshot zeigt den Dialog, in dem der Quell-Nummernverwalter (B) mit den Anfragen ausgewählt ist und der Ziel-Nummernverwalter (C) für die zu erstellenden Bestellungen.*

2.  Wählen Sie den Nummernverwalter (B), in dem die Aufträge stehen, zu denen Sie Anfragen erzeugt haben.
3.  Wählen Sie die Option Pool füllen (A).
4.  Wählen Sie im Menü Start > Ausführen, um die Aufträge in den Bestellpool zu stellen.
    Die Bestellpositionen werden eingelesen und die Anzeige wechselt zum Register Bestellpool.

*Abb. D-69: Bestellungen zu Aufträgen erzeugen. Im Bestellpool werden die Anfragen (B) zum Auftrag angezeigt. Der Modus "Bestellung" (A) ist ausgewählt, um Bestellungen im Ziel-Nummernverwalter (C) zu erzeugen.*

    Zu den Anfragepositionen aus dem Auftrag werden die Dokumenten-Nummern der Anfragen angezeigt.
5.  Markieren Sie die Option Bestellung (A) und wählen Sie den Ziel-Nummernverwalter (C) für Bestellungen aus.
6.  Markieren Sie die Positionen, für die eine Bestellung erstellt werden soll.
    Klicken Sie dazu doppelt in den jeweiligen Zeilenkopf. Nur die Positionen sind markiert, die mit einem X gekennzeichnet sind.
7.  Wählen Sie im Menü Start > Ausführen, um die Bestellungen zu erzeugen.
    Die Bestellungen wurden erzeugt. Die übergebenen Positionen werden aus dem Bestellpool gelöscht.
    Die erzeugten Bestellungen können Sie unter **Dokumente > Bestellung** öffnen, drucken und an den Lieferanten senden.

### Bestellung aus unabhängiger Anfrage erstellen

Sie können aus jeder Anfrage durch Kopieren eine Bestellung erzeugen, unabhängig davon, ob die Anfrage referenziert ist oder nicht. Die Referenz auf einen Kundenauftrag wird dabei jedoch nicht übernommen.

Die Kopierfunktion ist ausführlich im Part Verkauf beschrieben.

**So erfassen Sie eine Bestellung zu einer Anfrage**
1.  Öffnen Sie die Anfrage, zu der Sie eine Bestellung erfassen möchten.
2.  Wählen Sie im Menü Funktionen > Gruppe Dokument > Dokument kopieren.

*Abb. D-70: Bestellung aus einer Anfrage erstellen. Der Screenshot zeigt den Dialog "Dokument kopieren" mit Ziel-Dokumententyp (A), Kopier-Modus (B) und Ziel-Nummernverwalter (C).*

3.  Wählen Sie den Dokumententyp **Bestellung** (A) aus.
    Im Bereich Ziel wird automatisch der erste Nummernverwalter für Bestellungen angezeigt.
4.  Wählen Sie ggf. einen anderen Ziel-Nummernverwalter (C) aus.
5.  Prüfen Sie die weiteren Einstellungen.
6.  Wählen Sie im Menü Start > Ausführen, um die Bestellung zu erzeugen.
    Die Positionen werden geprüft und kopiert. Die Bestellung wird gespeichert.
7.  Schließen Sie den Dialog.
    Der Dialog Dokumente kopieren wird geschlossen und der Dialog Dokumentenverwaltung wird wieder angezeigt.
    In der Historie der Anfrage und der Bestellung wird die Referenz angezeigt. Die erzeugte Bestellung können Sie unter **Dokumente > Bestellung** öffnen, drucken und an den Lieferanten senden.

### Übungen

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

**Liefertermine prüfen, ändern und Kunden benachrichtigen**
Tragen Sie folgende Änderungen ein:
*   Tragen Sie in einer referenzierten Bestellung eine größere Stückzahl in einer Position ein und übergeben Sie Position erneut.
*   Wählen Sie einen anderen Lieferanten, weil der ursprüngliche die Termine nicht einhalten wird.
*   Ändern den Liefertermin in einer Bestellung und benachrichtigen Sie anschließend den Kunden über die Verzögerung.

**Lieferanten mahnen**
Suchen Sie nach Bestellungen, zu denen Sie noch keine AB erfasst haben, und mahnen Sie den Lieferanten.

### Ergänzende Informationen
⇨ "Lieferantenkartei" auf Seite D-31
⇨ "Lieferungen im Wareneingang" auf Seite D-119
⇨ "Kistengeschäft" auf Seite D-136
⇨ "Wareneingang von Kisten" auf Seite D-135
⇨ "Elektronischer Dokumentenaustausch" auf Seite D-150

**Part Verkauf**
⇨ Verkauf, "Dokumente kopieren" auf Seite C-250
⇨ Verkauf, "Dokumente kopieren" auf Seite C-543
⇨ Verkauf, "Auftrags-/Bestell-Info" auf Seite C-574
⇨ Verkauf, "Dokumentendaten" auf Seite C-754

**Part Stammdaten**
⇨ Stammdaten, "Produkt" auf Seite B-141
⇨ Stammdaten, "Währungen" auf Seite B-464
⇨ Stammdaten, "Lagermaße" auf Seite B-646
⇨ Stammdaten, "Preise" auf Seite B-725
⇨ Stammdaten, "Partnerverwaltung" auf Seite B-770
⇨ Stammdaten, "Firmendaten" auf Seite B-930
⇨ Stammdaten, "Pos. ohne Lagerkennz. im WE anzeigen bei Lagerbestell." auf Seite B-972

**Part Lagerwirtschaft**
⇨ Lagerwirtschaft, "Lagerverwaltung" auf Seite G-68
⇨ Lagerwirtschaft, "Lagerbestellung (automatisch)" auf Seite G-107
⇨ Lagerwirtschaft, "Lagerverwaltung - Lagerartikel" auf Seite G-189
⇨ Lagerwirtschaft, "Lagerbewegung - Abgang, Zugang" auf Seite G-199

## Lieferungen im Wareneingang

In diesem Themenblock lernen Sie, wie Sie die Preise und Rechnungen kontrollieren und den Wareneingang erfassen.

Dazu gehören folgende Lerneinheiten:
*   "Wareneingang" auf Seite D-120
*   "Wareneingang von Kisten" auf Seite D-135
*   "Preis- und Rechnungskontrolle" auf Seite D-143

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

#### Lernziele
*   Dialog Wareneingang kennenlernen.
*   Unterscheidung von Wareneingängen aus Lagerbestellungen und aus referenzierten Bestellungen kennenlernen.
*   Wareneingänge auf Vollständigkeit prüfen.
*   Vergessene Eingangsbuchungen nachholen.

#### Nutzen
*   Lieferungen müssen erfasst werden, damit die Kundenaufträge fertiggestellt und ausgeliefert werden können.
*   Beim Erfassen von Wareneingängen aus Lagerbestellungen wird der Lagerbestand aktualisiert, so dass Sie sich immer über den aktuellen Bestand informieren können.
*   Wareneingänge können trotz Differenzen zwischen den bestellten und den gelieferten Mengen erfasst werden.

#### Merke
| Begriff | Erklärung |
| :--- | :--- |
| **Unvollständige Lieferung** | Der Wareneingang kann teilweise erfasst werden, wenn die gelieferte Menge nicht der bestellten Menge entspricht. |
| **Überzählige Stückzahlen** | Wenn die Liefermenge von Lagerartikeln (mit einer Lager-ID) die bestellte Menge einer Lagerbestellung überschreitet, wird diese Menge in den Lagerbestand gebucht. |
| | Der Wareneingang von Übermengen wird nur dann verbucht, wenn Sie die Checkbox `akzeptieren` markiert haben. |
| | Übermengen bei Kundenaufträgen müssen in den Stammdaten zugelassen und eingegrenzt werden. |
| **Voreinstellungen** | **Firmendaten:**<br>- Register Parameter<br>- Register Lager/EK/EDI<br>**Stammdaten (Übermengen):**<br>- Kunde, Lieferant<br>- Produkt |

#### Lieferungen

Bei der Erfassung von Wareneingängen wird zwischen Kisten, Lagerbestellungen, unabhängigen und referenzierten Bestellungen unterschieden.

*Abb. D-71: Wareneingang und Lagerbuchungen. Ein Flussdiagramm zeigt, wie verschiedene Bestellarten (Lagerbestellung, Kiste, referenziert, unabhängig) den Wareneingang und die Buchung im Bestand beeinflussen.*

Diese Unterscheidung dient in der Lagerverwaltung zur Pflege der Bestandsdaten.

Nach der Buchung des Wareneingangs werden sämtliche automatischen Zuschläge für die Bestellung überrechnet und gespeichert.

**Wareneingang von Lagerbestellungen**
Mit der Buchung des Wareneingangs von Lagerbestellungen werden die Stückzahlen im Lager aktualisiert. Im Dialog Lagerinfo werden neben den Lagerbeständen auch die reservierten Stückzahlen angezeigt. Damit haben Sie schon in der Positionserfassung einen Überblick über aktuelle und zukünftige Lagerbestände.

Auch Positionen einer Lagerbestellung mit Artikeln ohne Lagerkennzeichen werden im Wareneingang angezeigt und können verbucht werden. Diese Buchungen ändern jedoch nicht den Lagerbestand.

**Bestellposition für die Produktion**
Wenn Sie in einem Kundenauftrag eine Bestellposition erfasst haben, die für die Produktion des Auftrags benötigt wird, kann dieser erst nach dem Wareneingang weiterbearbeitet werden. Wenn Sie den Wareneingang erfassen, muss daher eine Meldung an die Produktion gesendet werden, damit der Auftrag produziert wird.

Im Wareneingang können Sie dazu eine Option aktivieren, mit der die Übergabe automatisch angestoßen wird, sobald der Eingang dieser Position erfasst wurde.

Für Auftragspositionen mit dem Kennzeichen `Bestellung (komplett)` wird der Status umgesetzt und an den Auftrag weitergegeben, damit der Auftrag ggf. ausgeliefert werden kann.

*Abb. D-72: Wareneingang – Bestellungen im Nummernverwalter. Der Screenshot zeigt eine Liste von Bestellungen mit ihrem Liefertermin (A), Status (B), Sperrstatus (C) und dem referenzierten Auftrag (D). Vollständig gebuchte Wareneingänge sind blau markiert.*

**Positionen ohne Lagerkennzeichen**
Wenn Sie Lagerbestellungen mit Positionen erfassen, die nicht als Lagerartikel geführt werden, werden diese im Wareneingang nicht angezeigt. Sie können in den Firmendaten jedoch die entsprechende Option aktivieren.

*Abb. D-73: Firmendaten - Register Lager/EK/EDI. Die Checkbox "Pos. ohne Lagerkennz. im WE anzeigen bei Lagerbestell." (A) aktiviert die Anzeige dieser Positionen.*

**Teilweiser Wareneingang**
Der Wareneingang kann vollständig oder auch teilweise gebucht werden. Der teilweise Wareneingang kann sowohl einzelne Positionen insgesamt betreffen als auch Teillieferungen zu einzelnen Positionen, z. B. die Positionen 5 und 7 einer Bestellung oder 15 Stück einer Position mit bestellten 30 Stück. Der Status der Bestellung und/oder des Auftrags wird danach entsprechend gesetzt.

**Wareneingang von Stücklisten-Komponenten**
Stücklisten-Komponenten werden nicht einzeln im Wareneingang aufgeführt, sondern gehören zu ihrem jeweiligen Hauptprodukt. In der Artikelbezeichnung werden die Stücklisten-Komponenten mit "/" getrennt aufgeführt.

**Lieferung mit Übermengen**
Wenn ein Lieferant eine größere Stückzahl (Übermenge) zu einer bestellten Position liefert, können Sie diese Lieferung im Wareneingang erfassen. Wenn es sich dabei um Lagerartikel (mit einer Lager-ID) aus einem Dokument vom Typ `Lagerbestellung` handelt, werden die gelieferten Stückzahlen in den Lagerbestand gebucht. In der Bestellung selbst werden die Stückzahlen dabei entsprechend geändert.

Dies gilt entsprechend auch für Untermengen, die jedoch in der Praxis eher selten vorkommen.

Die Über- und Untermengen werden in folgenden Dialogen festgelegt:
*   **Pro Kunde und pro Produkt:** prozentuale Höhe der Abweichung.

*Screenshot des Dialogs "Übermengen" zur Definition prozentualer Abweichungen pro Produkt.*

*   **Pro Auftragsposition:** zusätzlich abweichende Menge.

*Screenshot des Dialogs "Abweichende Mengen" zur Definition abweichender Mengen pro Auftragsposition.*

**Eingangskontrolle**
Einen schnellen Überblick über offene oder unvollständige Lieferungen können Sie sich über den Dialog Eingangskontrolle anzeigen lassen.

*Abb. D-74: Kontrolle des Wareneingangs. Der Dialog "Eingangskontrolle" zeigt eine Liste von Bestellungen (A) mit bestellter Menge (B), gelieferter Menge (C) und einem Status, ob der Wareneingang komplett ist (D).*

Sie können die Buchung für Bestellungen oder Bestellpositionen nachholen, für die der Wareneingang noch nicht erfasst wurde, obwohl die Lieferung eingetroffen ist.

#### Voreinstellungen für Wareneingang prüfen

In den Firmendaten müssen die Voreinstellungen festgelegt werden, die sich auf den Wareneingang beziehen. Die entsprechenden Parameter und Optionen finden Sie in folgenden Registern:
*   Parameter
*   Lager/EK/EDI

*Abb. D-75: Firmendaten – Register Parameter. Die Checkbox "Virtuelle Positionsnummern verwenden" (A) ist für den Wareneingang von Kisten relevant.*

Die virtuellen Positionsnummern werden erzeugt, damit der Wareneingang von Kisten korrekt verbucht werden kann. Diese Funktion wird in der Lerneinheit für den Wareneingang von Kisten beschrieben.
⇨ "Wareneingang von Kisten" auf Seite D-135

**Lagerbestand**
Um den Lagerbestand mit den Eingangsbuchungen aktualisieren zu können, müssen in den Firmendaten die Reservierungsoption und die Lagerführung auf Stücklistenebene aktiviert werden.

*Abb. D-76: Firmendaten – Register Lager/EK/EDI. Die Optionen "Bestandsaktualisierung bei Reservierung" (A) und "Lagerführung auf Stücklistenebene" (B) sind relevant.*

#### Wareneingang erfassen

Mit dem Wareneingang können Sie auch die Nummer der Auftragsbestätigung (AB) des Lieferanten erfassen und den Liefertermin ändern. Teillieferungen erfassen Sie, indem Sie die gelieferte Stückzahl einer Position angeben oder nur einzelne Positionen als vollständig geliefert kennzeichnen.

> **Erfassung im Wareneingang**
> In der Regel werden die Dokumentennummern über den Barcode-Scanner erfasst. Bei den folgenden Beispielen werden sie manuell erfasst. Alle weiteren Handlungsschritte sind für die beiden Varianten identisch.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So erfassen Sie einen Wareneingang ganz" auf Seite D-128
*   "So erfassen Sie einen Wareneingang teilweise" auf Seite D-130

**So erfassen Sie einen Wareneingang ganz**
1.  Wählen Sie Dokumente > Bestellung > Wareneingang > Wareneingang.

*Abb. D-77: Wareneingang – Auswahl nach Nummernverwalter. Der Dialog bietet verschiedene Auswahlmöglichkeiten, u.a. nach Nummernverwalter (A), mit Auswahl des spezifischen Nummernverwalters (B).*

    ⇨ Softwarereferenz, "Wareneingang (Dialog)" auf Seite D-227
2.  Wählen Sie im Bereich Auswahl die Option `nach Nummernverwalter`.
3.  Wählen Sie im Menü Start > Ausführen, um die Daten einzulesen.
    Die Anzeige wechselt zum Register Komplett, in dem die Bestellungen angezeigt werden, die im Nummernverwalter stehen.

*Abb. D-78: Wareneingang – Bestellungen. Die Liste der Bestellungen wird angezeigt, mit Feldern für den Anliefertermin und die AB-Nummer (A), Sperrstatus (B), eine Checkbox für den vollständigen Wareneingang (C) und eine Anzeige für Kisten (D).*

    Die Felder im Bereich Liefertermin (A) sind gesperrt, wenn zu der markierten Bestellung eine Auftragsbestätigung des Lieferanten erfasst wurde.
4.  Markieren Sie die Bestellung, zu der Sie den Wareneingang erfassen möchten.
    Die Felder im Bereich Liefertermin (A) werden freigeschaltet. In der Regel sind der Anliefertermin und die AB-Nummer des Lieferanten bereits erfasst. Sie können diese Daten jedoch nachtragen, falls sie noch fehlen.
5.  Markieren Sie die Checkbox `komplett buchen` (C).

*Abb. D-79: Wareneingang - Bestellung komplett melden. Die Checkbox "komplett buchen" ist für die ausgewählte Bestellung markiert.*

6.  Wählen Sie im Menü Start > Ausführen, um den Wareneingang zu erfassen.
    Die Daten werden gespeichert und der Status der Bestellung wird umgesetzt. Bei Lagerartikeln wird der Lagerbestand aktualisiert. Bei referenzierten Bestellungen wird der Wareneingang an die Produktion und/oder den Verkauf übergeben, um den zugehörigen Kundenauftrag weiterzubearbeiten oder abzuschließen.

**So erfassen Sie einen Wareneingang teilweise**
1.  Wählen Sie Dokumente > Bestellung > Wareneingang > Wareneingang.
2.  Wählen Sie im Bereich Auswahl die Option `nach Bestellnummer` (A) und geben Sie die Bestellnummer (B) ein.

*Abb. D-80: Wareneingang – Auswahl. Die Option "nach Bestellnummer" (A) ist ausgewählt und eine Nummer (B) ist eingegeben.*

3.  Wählen Sie im Menü Start > Ausführen, um die Daten einzulesen.
    Die Daten werden eingelesen und die Anzeige wechselt zum Register Komplett.
    Wenn Sie öfter nur über die Bestell- oder Auftragsnummer gehen, können Sie im Menü Optionen einstellen, dass die Anzeige nach dem Einlesen des Dokuments zum Register Positionsweise wechselt.
4.  Wechsel Sie ggf. zum Register Positionsweise.

*Abb. D-81: Wareneingang – Teilmenge der Bestellung melden. Im Register "Positionsweise" können Teilmengen erfasst werden. (A) Position komplett buchen, (B) Lagerort, (C) Teilmenge, (D) bereits gelieferte Menge, (E) Über-/Untermengen akzeptieren, (F) AB-Nummer.*

    Alle Positionen der Bestellung werden angezeigt. Sie haben folgende Möglichkeiten, einen teilweisen Wareneingang zu erfassen:
    *   Eine der Bestellpositionen komplett buchen (A).
    *   Zu einer Position eine Teilmenge (C) der bestellten Stückzahl erfassen.
    Wenn die Lieferung z. B. bei einer Lagerbestellung nicht exakt der Bestellmenge entspricht, können Sie die Über- oder Untermenge akzeptieren (E), und so den Wareneingang einer Position komplett buchen.
5.  Markieren Sie die Position, zu der Sie den Wareneingang erfassen wollen.
6.  Tragen Sie im Feld **Menge Eingang** (C) die Stückzahl der gelieferten Position ein oder markieren Sie die Checkbox `komplett buchen` (A), um die gesamte Position als geliefert zu melden.
7.  Tragen Sie ggf. AB-Nummer des Lieferanten (F) ein.
8.  Wählen Sie bei Lagerartikeln den Lagerort (B) aus.

*Abb. D-82: Wareneingang – Teilmenge der Bestellung melden. Der Screenshot zeigt die Erfassung einer Teilmenge von 15 aus 30 Stück.*

9.  Wählen Sie im Menü Start > Ausführen, um die Daten zu speichern.
    Der teilweise Wareneingang wird verbucht.
    Die Bestellpositionen werden in blauer Schrift angezeigt, wenn die Bestellung/Position komplett geliefert ist.
    Änderungen werden in die Bestellung und ggf. in den referenzierten Kundenauftrag übernommen.
    Eine Übermenge wird in die Bestellung zurückgeschrieben, ein referenzierter Auftrag bleibt davon unberührt. Im Lager wird die Übermenge nur bei Lagerartikeln aus einer Lagerbestellung automatisch verbucht. Dies gilt ebenso für Untermengen, jedoch wird dann in der Praxis eher eine Teillieferung erstellt und die fehlende Menge beanstandet.

#### Wareneingang kontrollieren

Sie müssen die Vollständigkeit der Lieferungen prüfen, um festzustellen, welche Bestellungen weiterverarbeitet werden können. Wenn Sie wissen, dass die Lieferung tatsächlich gekommen ist, können Sie den Wareneingang nachträglich erfassen. Sie können folgende Sachverhalte prüfen:
*   Komplette Bestellungen pro Nummernverwalter
*   Mengendiskrepanzen pro Bestellposition

**So kontrollieren Sie den Wareneingang**
1.  Wählen Sie Dokumente > Bestellung > Wareneingang > Eingangskontrolle.

*Abb. D-83: Eingangskontrolle – Komplette Bestellung. Das Register "Komplette Bestellungen" listet vollständig gebuchte Wareneingänge auf.*

    ⇨ Softwarereferenz, "Eingangskontrolle" auf Seite D-241
2.  Wählen Sie im Register Komplette Bestellungen den Nummernverwalter für die Bestellungen aus.
    In der Übersicht Wareneingang komplett werden alle Bestellungen aufgelistet, deren Bestellungen vollständig erfasst sind.
3.  Wechseln Sie zum Register Mengendiskrepanzen, um sich die unvollständigen Positionen anzeigen zu lassen.

*Abb. D-84: Eingangskontrolle – Mengendiskrepanzen. Das Register listet alle Positionen mit einer Differenz zwischen bestellter und gelieferter Menge (A) auf. Mit der Checkbox "OK" (B) kann der Wareneingang komplett gebucht werden.*

    In der Übersicht werden alle Bestellungen aufgelistet, zu denen noch kein oder ein unvollständiger Wareneingang gebucht wurde.
    Wenn Sie die Bestellungen beim Buchen des kompletten Wareneingangs in einen Ziel-Nummernverwalter geschoben haben, sollten hier keine Diskrepanzen angezeigt werden.
4.  Holen Sie ggf. versäumte Buchungen nach, indem Sie die Checkbox OK (B) markieren.
    Beachten Sie dabei, dass Sie nur komplette Wareneingänge nachholen können. Um Teilmengen zu erfassen, wechseln Sie zum Dialog Wareneingang.
5.  Wählen Sie im Menü Start > Ausführen, um den Wareneingang zu buchen.
    Der Wareneingang wird verbucht. Die vollständig verbuchten Bestellungen werden aus der Liste entfernt.

**Ergänzende Informationen**
⇨ Stammdaten, "Pos. ohne Lagerkennz. im WE anzeigen bei Lagerbestell." auf Seite B-972
⇨ Stammdaten, "Lagerführungsmodus" auf Seite B-973
⇨ Verkauf, "Lagerinfo" auf Seite C-758
⇨ Softwarereferenz, "Wareneingang" auf Seite D-227

### Wareneingang von Kisten

#### Lernziele
*   Sinn der Dummy-Kiste kennenlernen.
*   Vergabe von Identnummern (IDs) kennenlernen.
*   Einstellungen für automatische Vergabe der Kisten-ID kennenlernen.

#### Nutzen
*   Jede Kiste erhält im Wareneingang eine ID, damit sie im Lagerbestand eindeutig identifiziert und für einen Auftrag reserviert werden kann.
*   Die IDs können manuell oder automatisch vergeben werden. Sie können dabei auch die Kisten-ID des Lieferanten übernehmen.

#### Merke
| Begriff | Erklärung |
| :--- | :--- |
| **Virtuelle Positionsnummern** | Wenn die Stückzahl einer Kistenposition größer als 1 ist, wird für jede Kiste eine Unterposition erzeugt. Diese Unterpositionen erhalten virtuelle Positionsnummern, die sich aus der Positionsnummer und der Anzahl der Kisten zusammensetzt, z B. 1.1, 1.2 oder 3.1, 3.2 usw. |
| **ID** | Bei der Erfassung des Wareneingangs wird für die Kiste jeder Unterposition eine eigene Identnummer (ID) vergeben. |
| **Kisten identifizieren** | Nur eine Kiste mit einer ID kann als Lagerbestand gebucht und/oder einer Auftragsposition zugeordnet werden. |
| **Voreinstellungen** | **Stammdaten:**<br>- Produktverwaltung<br>**Firmendaten:**<br>- Register Parameter<br>- Register Lager/EK/EDI |

### Kistengeschäft

Für Kisten werden in der Regel Identnummern (ID) vergeben, die entweder vom Lieferanten stammen können oder im eigenen System gepflegt werden. Diese IDs werden beim Wareneingang von Kisten erfasst. Jede Kiste wird mit einer eigenen Kisten-ID verbucht und im Lager geführt.

Auch wenn die Anzahl von Kisten in einer Bestellposition größer als 1 ist, wird jede Kiste als ein eigener Wareneingang verbucht. Dazu legt das System automatisch Unterpositionen (virtuelle Positionen) zu der ursprünglichen Position an und ordnet jeder dieser Positionen genau eine Kiste zu. Diese Funktion muss in den Firmendaten aktiviert werden.

Zu jeder Unterposition muss eine eigene Kisten-ID angegeben werden, damit der Lagerbestand der Kisten gepflegt werden kann. Diese Kisten-IDs können nach selbst definierten Vorgaben automatisch eingefügt werden. Eine ID kann jedoch auch manuell eingegeben werden, z. B. um die Kisten-ID aus dem Lieferschein des Lieferanten zu übernehmen.

Im Rahmen des Wareneingangs kann im Dialog zur automatischen Kisten-ID auch ein Produktionsdatum angegeben werden. Für beschichtetes Glas wird dieses zur Berechnung des Verfallsdatums herangezogen, damit nach dem FiFo-Prinzip gearbeitet werden kann (FiFo = First in - First out).

Nach der Vergabe der IDs können über die Druckfunktion die Kistenetiketten mit den IDs als Barcode gedruckt und an den entsprechenden Kisten angebracht werden.

In der Regel werden die Barcodes von Kisten beim Warenausgang oder bei der Auflösung von Kisten gescannt. Damit ist der Bestand von Kisten nicht nur mengenmäßig aktuell, sondern die Kisten sind eindeutig identifiziert.

### Firmendaten prüfen

Im Part Stammdaten ist ausführlich beschrieben, wie Sie die Stammdaten zu Ihrer Firma einrichten. In der folgenden Beschreibung wird daher nur auf die Besonderheiten eingegangen, die Sie für den Wareneingang von Kisten beachten müssen.

> **A+W Business neu starten**
> Nach Änderungen der Firmendaten sollten Sie A+W Business neu starten.

**So prüfen Sie die Firmendaten**
1.  Wählen Sie Stammdaten > Firma > Firmendaten und prüfen Sie im Register Parameter die Einstellung für die Checkbox `Virtuelle Positionsnummern verwenden`.
    Diese Einstellung ist bereits in der Lerneinheit Wareneingang dargestellt.
    ⇨ "Firmendaten – Register Parameter" auf Seite D-126
2.  Wählen Sie im Menü Start > Speichern, um Änderungen zu speichern.
    Die Daten werden gespeichert.

