---
description: "D-AWBusiness-HB_29"
---


# Softwarereferenz Lagerverwaltung

---
## Menü Optionen

**Pfad:** Lagerwirtschaft > Lagerverwaltung > Menü Optionen

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

Folgende Einträge werden angezeigt:

-   **Artikel mit Bestand = 0 nicht drucken:** Nur Artikel, deren Bestand größer als 0 ist, werden gedruckt. Diese Einstellung ist sinnvoll, wenn es sehr viele Kisten mit einer ID aber ohne Bestand gibt. Diese sind dann in der Regel als Kiste ausgeliefert worden und aus dem Bestand gelöscht. Die Einstellung gilt nur für den Druck, im Dialog werden alle Artikel angezeigt.
-   **Identnummer automatisch vergeben:** Die ID der Kiste kann auch automatisch vergeben werden, wenn sie manuell als Bestand gebucht wird.

## Menü Druck

**Pfad:** Lagerwirtschaft > Lagerverwaltung > Menü Druck

Über dieses Menü können Sie den Druck von Etiketten starten.

Folgende Einträge werden angezeigt:

-   **Kistenetiketten:** Nur Etiketten für Kisten werden gedruckt. Dazu muss der Druckpunkt 973 angelegt und in der Formularverwaltung der Report boxlabel.qrp zugewiesen sein.
-   **Standard:** Etiketten für die Lagerartikel werden gedruckt.

## Lagerverwaltung

**Pfad:** Lagerwirtschaft > Lagerverwaltung

Im Dialog Lagerverwaltung werden die Lagerartikel erfasst, die im Lager mit Beständen gehalten werden.

Lagermaße werden in A+W Business auch in der Produktverwaltung gepflegt. Sie dienen dort dazu, Preisschlüssel, Warengruppen, usw. zuzuordnen.

Im Dialog Lagerverwaltung finden Sie folgende Register:

-   Lagerverwaltung - Lagerartikel
-   Lagerverwaltung – Preise
-   Lagerverwaltung - Zusatz

> **Lagerverwaltung auf der Ebene der Stücklisten**
> Sie können im Lager auch Produkte verwalten, die als Stücklisten-Komponenten in anderen Produkten enthalten sind. Dazu muss in den Firmendaten die Checkbox Lagerführung auf Stücklistenebene aktiviert sein.
>
> ⇨ Tutorial, "Lagerführung auf Stücklistenebene" auf Seite G-61
> ⇨ Stammdaten, "Lagerführung auf Stücklistenebene" auf Seite B-973

### Lagerverwaltung – Lagerartikel

**Pfad:** Lagerwirtschaft > Lagerverwaltung > Register Lager-Artikel

In diesem Register können Sie die Artikel prüfen, die im Lager verwaltet werden. Der angezeigte Bestand wird mit jeder Lagerbuchung aktualisiert. Sie können neue Artikel hinzufügen und die verschiedenen Mengen korrigieren.

Für das Bestellwesen legen Sie außerdem Mindest- und Bestellmengen fest.

⇨ Tutorial, "So legen Sie einen Lagerartikel an" auf Seite G-74

#### Identifikation

**Artikel**
Produktnummer aus den Stammdaten. Wenn Sie einen neuen Lagerartikel erfassen möchten, müssen Sie ihn zuerst in den Stammdaten anlegen.

**Lager-ID**
Identnummer, die beim Wareneingang vergeben wurde.

**Bezeichnung**
Produktbezeichnungen aus den Stammdaten.

**Breite x Höhe / Inhalt**
Maße des Lagerartikels in mm (nur Lagermaße) und Inhalt der Kiste. Bei Kisten tragen Sie ein, wie viele Blätter die Kiste enthält. Für alle anderen Lagerartikel steht automatisch eine 1.

**Variante**
Wenn zu einem Artikel Varianten angelegt sind, so wird die Farbe angezeigt.

**Default-Lagerort**
Wenn Sie Lagerorte definiert haben, werden diese zur Auswahl angeboten.
Wenn Sie einen Lagerartikel an mehreren Lagerorten halten, kann ein Standard-Lagerort festgelegt werden.
- Der angezeigte Lagerort ist für den Lagerartikel nicht als Standard festgelegt.
- Der angezeigte Lagerort ist für den Lagerartikel als Standard-Lagerort festgelegt.
⇨ Stammdaten, "Lagerdefinition" auf Seite B-748

> **Lagerort <k.A.>**
> Auch wenn Sie eigene Lagerorte hinterlegt haben, bleiben die Lagerorte <k.A.> erhalten und können bebucht werden.

**Ident.**
Die Kisten-ID, die beim Wareneingang oder manuell vergeben wurde. Die ID wird nur angezeigt, wenn Sie in der Übersicht der Lagerartikel eine Kiste markiert haben.

#### Details

**Kategorie**
Wenn Sie in den Stammdaten Lagerkategorien definiert haben, können Sie dieses Feld als Suchkriterium verwenden. Beim Anlegen neuer Lagerartikel können Sie eine Kategorie zuordnen.

**Lief.-Ident**
Die Kisten-ID des Lieferanten wird nur angezeigt, wenn Sie im Bereich Lagerartikel eine Kiste markiert haben.

**Hauptartikel**
Lagerartikel mit mehreren Maßen können Sie miteinander verknüpfen, indem Sie einen Hauptartikel angeben. Die Bestandsprüfung (für die Lagervorschau im Dialog Lagerinfo) wird dann nur für den Hauptartikel durchgeführt und nur für diesen müssen Sie einen Mindestbestand hinterlegen. Wenn bei den zugeordneten Lagerartikeln ebenfalls Mindestbestände festgelegt sind, werden diese bei der Prüfung ignoriert.
⇨ Tutorial, "Lager-Hauptartikel" auf Seite G-70

**Produktionslauf / Datum**
Zur Zeit nicht genutzt.

**Datum**
Datum, an dem der Lagerartikel zuletzt geändert wurde.

**In Produktion**
In Verbindung mit A+W Production können Sie festlegen, ob der Lagerartikel der Produktion zugeordnet ist.
- Der Lagerartikel ist frei verfügbar.
- Der Lagerartikel ist der Produktion zugeordnet (nur Info).

#### Bestände

**Lagerbestand**
Anzeige des aktuellen Bestands. Der Bestand wird bei jeder Ab- oder Zubuchung aktualisiert. Für Kisten mit einer ID wird jeweils der Bestand 1 angezeigt.
Wenn Sie den Lagerartikel neu angelegt haben, ist das Feld freigeschaltet und Sie können den Anfangsbestand eintragen.

**Bestand > 0**
Diese Checkbox ist nur im Auswahlmodus freigeschaltet. Sie können damit als Suchkriterium festlegen, ob Artikel ohne Bestandsmenge angezeigt werden.
- Im Suchergebnis werden auch Artikel angezeigt, deren aktueller Bestand 0 ist.
- Im Suchergebnis werden nur Artikel angezeigt, deren aktueller Bestand mindestens 1 ist.

**Mindestbestand**
Der Mindestbestand bildet die Grundlage für automatische Bestellvorschläge. Sie werden erzeugt, wenn der Lagerbestand den Mindestbestand unterschreitet. Dabei werden die Reservierungen und die Bestellungen mitberücksichtigt. Diese automatischen Bestellvorschläge können Sie im Dialog Lagerbestellung prüfen und an den Einkauf übergeben.
⇨ "Lagerbestellung" auf Seite G-223

**Mindestbestand > 0**
Diese Checkbox ist nur im Auswahlmodus freigeschaltet. Sie können damit als Suchkriterium festlegen, ob der Mindestbestand größer als 0 sein muss.
- Im Suchergebnis werden alle Artikel angezeigt.
- Im Suchergebnis werden nur Artikel angezeigt, deren Mindestbestand größer als Null ist.

**Bestellmenge**
Dieser Wert gibt an, welche Menge standardmäßig bestellt wird. Bei der automatischen Lagerbestellung wird der Wert übernommen.

**Bestand < Mindestbestand**
Diese Checkbox ist nur im Auswahlmodus freigeschaltet. Sie können damit als Suchkriterium festlegen, ob der Bestand unter dem Mindestbestand liegen soll.
- Im Suchergebnis werden alle Artikel angezeigt.
- Im Suchergebnis werden nur Artikel angezeigt, deren aktueller Bestand kleiner als der Mindestbestand ist.

**Maximalbestand**
Mit der Eingabe von Maximalmengen pro Lagerartikel kann verhindert werden, dass das Lager überfüllt ist. Der eingetragene Wert dient nur der manuellen Kontrolle.

**Sollbestand**
Zur Zeit nicht genutzt.

**Bestandsprüfung pro Lagerort**
Wenn Sie den Bestand pro Lagerort pflegen, können Sie die den Bestand pro Lager prüfen.
- Der Bestand wird für alle Lagerorte gemeinsam geprüft.
- Der Bestand wird pro Lagerort geprüft.

**Kritischer Lagerbestand**
Für jeden Lagerartikel können Sie die Menge angeben, ab der eine Bestellung zwingend erforderlich ist.
Damit der eingetragene Wert geprüft wird, muss die Option Bestandsprüfung pro Lagerort aktiviert sein.
In der Lagerwirtschaft wird das Datum berechnet, an dem der Bestand eines Lagerartikels unter diese kritische Menge fällt. Das Datum, an dem ein Lagerartikel die kritische Menge erreicht, wird im Bestellpool.
⇨ Verkauf, "Bestellübergabe - Bestellpool" auf Seite C-675

#### Lagerartikel

In den Übersichten werden die Lagerartikel angezeigt, die den Suchkriterien entsprechen. Die obere Liste zeigt die Lagerartikel insgesamt an. Wenn Sie einen Eintrag markieren, werden in der unteren Liste die Artikel pro Lagerort angezeigt. Wenn Checkbox Bestand > 0 aktiviert ist, werden nur Lagerorte aufgelistet, deren Bestand größer als 0 ist.

Folgende Spalten werden angezeigt:

-   **Artikel, Variante:** Artikelnummer, Bezeichnung und Farbe aus der Lagerverwaltung.
-   **Breite, Höhe:** Maße aus der Lagerverwaltung.
-   **Inhalt:** Anzahl der Blätter in einer Kiste.
-   **Ges. Bestand:** Bestand des Lagerartikels aller Lagerorte.
-   **Min. Bestand:** Menge des festgelegten Mindestbestands.
-   **Best. Menge:** Festgelegte Bestellmenge.

#### Lagerorte

-   **Ident:** Kisten-ID (manuelle Buchung oder aus dem Wareneingang).
-   **Lagerort:** Lagerort in der Reihenfolge von Ebene 1 bis 4.
-   **Lagerbestand:** Aktueller Bestand am Lagerort.
-   **Lief.-Ident:** Kisten-ID des Lieferanten (nur wenn diese im Wareneingang miterfasst wurde).

### Lagerverwaltung – Preise

**Pfad:** Lagerwirtschaft > Lagerverwaltung > Register Preise

In diesem Register werden die aktuellen Preise eines Lagerartikels angezeigt. Bei der Aktualisierung werden Aufträge, Bestellungen und Lagerumbuchungen berücksichtigt.

⇨ Tutorial, "Preise" auf Seite G-51

> **Voraussetzung**
> Der durchschnittliche Einkaufspreis (Durchschnitts-EK) wird nur dann berechnet und angezeigt, wenn in den Firmendaten die Checkbox Einkaufspreis ermitteln und die Option Durchschnitts EK aktiviert sind.
>
> ⇨ Stammdaten, "Durchschnitts EK: Der Durchschnittspreis für den Einkauf wird in folgenden Fällen neu berechnet:" auf Seite B-970

Die Felder in den Übersichten sind ausführlich zum Register Lagerartikel beschrieben.
⇨ "Lagerverwaltung - Lagerartikel" auf Seite G-189

#### Einkaufspreise

**Niedrigster Preis**
Der niedrigste Preis, zu dem der Artikel eingekauft wurde.

**Höchstpreis**
Der höchste Preis, zu dem der Artikel eingekauft wurde.

**Letzter Preis**
Der jüngste Preis, zu dem der Artikel eingekauft wurde.

**Lagerwert**
In dieser Spalte werden die aktuellen Lagerwerte angezeigt. Sie ergeben sich aus dem jeweiligen Preis und der Menge.

#### Berechnung des geschnittenen Preises (Durchschnitts-EK)

Mit der Wahl der Option bestimmen Sie, welche Lagermaße in dieser Übersicht bei der Berechnung berücksichtigt werden. Die Einstellung ist nur bei Scheiben mit unterschiedlichen Lagermaßen sinnvoll.

-   **Nur dieser Artikel:** Bei der Berechnung wird nur der angezeigte Artikel in der gewählten Abmessung berücksichtigt. Die EK-Historie des aktuellen Artikels wird angezeigt.
-   **Alle Abmessungen:** Bei der Berechnung werden alle Abmessungen des angezeigten Glases berücksichtigt. Die EK-Historie aller Abmessungen des Artikels wird angezeigt.

Der Durchschnitts-EK wird für jeden Wareneingang errechnet, unabhängig davon, wie er gebucht wurde. Warenabgänge reduzieren lediglich den Bestand. Die Liste wird durch die Archivierung und durch die Rechnungskontrolle reduziert.

Der erste Datensatz zeigt den Anfangsbestand und den ursprünglichen Preis. Darunter werden Zu- und Abgänge (negatives Vorzeichen) aufgeführt. Beim Zugang durch eine Lagerbestellung sind außerdem die Bestellnummer und die Bestellposition angezeigt.

Der Durchschnitts-EK wird bei der Erfassung oder Änderungen von Bestellungen aktualisiert. Er wird unter Berücksichtigung der gesamten Menge ermittelt.

**Beispiel:**
100 Stück auf Lager à 15,00 € = 1500,00 €
40 Stück neue Einbuchung à 18,00 € = + 720,00 €
========
2200,00 €
2200,00 / 140 Stück = 15,86 €

In die Berechnung fließen auch automatische Zuschläge ein, die in Bestellungen aufgeführt sind, z. B. Energie- oder Transportzuschlag.

#### Übersicht

Die jeweiligen Durchschnittspreise werden als Historie dargestellt. Auf diese Weise können Sie die Preisentwicklung leicht nachverfolgen. Angezeigt werden:

-   **Datum:** Datum der letzten Aktualisierung.
-   **Menge [ME]:** Ab- oder zugebuchte Menge und Mengeneinheit.
-   **Preis/[PE]:** EK-Preis pro Preiseinheit zum Zeitpunkt der Buchung.
-   **Bestand [ME]:** Bestand zum anzeigten Datum. Wenn der Durchschnitts-EK für alle Abmessungen angezeigt wird, wird der Bestand immer in qm angezeigt.
-   **Geschnittener Preis / [PE]:** Durchschnittspreis pro Preiseinheit zum Zeitpunkt der Buchung.
-   **Bestellung / Pos.:** Nummer der Bestellung und der Bestellposition.
-   **Lagerwert:** Lagerwert zum angezeigten Datum (Berechnung: EK-Preis * Bestand).
-   **Typ:** Art von Buchung, die den jeweiligen Eintrag verursacht hat.

**Einbeziehen in Gesamt-EK**
Sie können festlegen, ob der Artikel in die Berechnung des gesamten Durchschnittspreises aller Ausprägungen dieses Artikels einbezogen werden soll.
- Der Artikel wird bei der Berechnung des Durchschnittspreises nicht berücksichtigt.
- Der Artikel wird in die Berechnung mit einbezogen.

**Geschnittener Preis**
Aktueller Durchschnittspreis. Je nach der Option zur Berechnung des Durchschnitts-EKs gilt die Anzeige für den aktuellen Artikel oder für alle Abmessungen des Artikels.

> **Aktualisierung der Anzeige**
> Die Anzeige der Durchschnittspreise wird bei der Archivierung und bei der Rechnungskontrolle für den jeweiligen Lagerartikel aktualisiert. Damit bleibt die Anzeige übersichtlicher.
> A+W Business geht davon aus, dass nach diesen Vorgängen die Preise nicht mehr geändert werden. Wenn Sie die Preise dennoch nach einem der Vorgänge ändern, fließen diese Änderungen nicht in die Berechnung des Durchschnittspreises ein.

### Lagerverwaltung – Zusatz

**Pfad:** Lagerwirtschaft > Lagerverwaltung > Register Zusatz

In diesem Register werden Reservierungen zu dem markierten Lagerartikel angezeigt.
Die Felder in den Übersichten sind ausführlich zum Register Lagerartikel beschrieben.
⇨ "Lagerverwaltung - Lagerartikel" auf Seite G-189

#### Reservierung

Die Felder in diesem Bereich sind kundenspezifisch freigeschaltet.

**Kunde**
Nummer und Name des Kunden, für den der markierte Lagerartikel reserviert ist.

**Voll gesperrt**
Zur Zeit nicht genutzt.

**Exklusive Reservierungen**
Zur Zeit nicht genutzt.

#### Lieferant

**Lieferant**
Nummer und Name des Lieferanten, bei dem der Lagerartikel bestellt wird.

#### Bemerkung

**Produktbezogen, Lagerortbezogen**
Sie können zu jedem Lagerartikel und zu jedem Lagerort weitere Angaben eintragen, z. B. wann und von welchem Lieferanten die Gläser/Kisten geliefert wurden, um die älteren Lieferungen zuerst zu verwerten.

## Lagerbewegung

**Pfad:** Lagerwirtschaft > Lagerbewegung

Sie können Ab- und Zugänge von Lagerartikeln manuell buchen, Bestandszahlen korrigieren, Lagerorte umbuchen und Kisten auflösen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:

-   "Menü Optionen" auf Seite G-198
-   "Lagerbewegung" auf Seite G-198

### Menü Optionen

**Pfad:** Lagerwirtschaft > Lagerbewegung
Folgende Einträge werden angezeigt:

-   **Protokoll beim Beenden:** Beim Beenden des Dialogs wird automatisch die Lagerhistorie angezeigt.
    ⇨ "Lagerhistorie" auf Seite G-207
-   **Bestand > 0:** Nur Lagerartikel mit einem Bestand größer 0 werden angezeigt.

### Lagerbewegung

**Pfad:** Lagerwirtschaft > Lagerbewegung

**Zu Dialogbeschreibung:**
⇨ Bemerkung (Lagerbewegung)
Zu- und Abgänge der Lagerartikel werden automatisch gebucht: bei Wareneingängen durch Lieferung, bei Warenabgängen durch Aufträge. Im Dialog Lagerbewegung können Sie Zu- oder Abgänge manuell buchen, z. B. um Bestandmengen zu korrigieren.

Im Dialog Lagerbewegung finden Sie folgende Register:

-   Lagerbewegung – Abgang, Zugang
-   Lagerbewegung – Umbuchung
-   Lagerbewegung – Blattanzahl
-   Lagerbewegung - Aufbruch

### Lagerbewegung – Abgang, Zugang

**Pfad:** Lagerwirtschaft > Lagerbewegung > Register Abgang, Register Zugang

In den Registern Abgang und Zugang können Sie manuell Ab- und Zugänge buchen. Sie können einen bestimmten Lagerartikel auswählen und die entsprechenden Daten eingeben. Wenn Sie sich alle Lagerartikel anzeigen lassen, können Sie den gewünschten Artikel in der Liste Lagerorte markieren. Die Felder im Bereich Bestandsveränderung werden dann freigeschaltet.

⇨ Tutorial, "Ab- und Zubuchung" auf Seite G-80

Wenn Sie die Option Protokoll beim Beenden aktiviert haben, wird automatisch die Lagerhistorie mit dem Register Tabelle angezeigt, wenn Sie den Dialog schließen.
⇨ "Lagerhistorie - Tabelle" auf Seite G-211

> **Zugang von Kisten manuell erfassen**
> Da jede Kiste mit einer eigenen ID geführt wird, können Sie Zugänge von Kisten nur über den Wareneingang oder in der Lagerverwaltung erfassen. Eine Beschreibung dazu finden Sie im Part Kistenmanagement.

#### Lagerprodukt

**Produkt**
Nummer und Bezeichnung des Lagerartikels.

**Ident Nr.**
Über die Identifikationsnummer können Sie nur Lagerabgänge verbuchen. Zugänge von Kisten müssen Sie in der Lagerverwaltung definieren, damit Sie eine neue ID eintragen können.

**Inhalt**
Wenn Sie eine Kiste ausgewählt haben, wird deren Inhalt angezeigt. Wenn eine Kiste mit Identnummer ausgeliefert oder geöffnet werden soll, die bereits einem Auftrag zugeordnet ist, wird eine Meldung angezeigt. Dadurch wird verhindert, dass durch den anschließenden Druck des Lieferscheins oder der Rechnung ein negativer Bestand entsteht.

**Lagerort**
Lagerort, der dem Lagerartikel zugeordnet wurde.

> **Lagerort <k.A.>**
> Auch wenn Sie eigene Lagerorte hinterlegt haben, bleiben die Lagerorte <k.A.> erhalten und können bebucht werden.

**Durchschnitts EK**
Der Durchschnitts-EK wird nur angezeigt, wenn die Funktion in den Stammdaten aktiviert ist.
⇨ Stammdaten, "Einkaufspreis ermitteln" auf Seite B-970

#### Bestandsveränderung

**Menge**
Eingabe die Menge in Stück, die ab- oder zugebucht werden soll. Wenn Sie mit einer manuellen Abbuchung den Mindestbestand unterschreiten, wird eine Warnmeldung angezeigt.

**Breite / Höhe**
Diese Felder werden nur bei Lagermaßen mit der Mengeneinheit qm gefüllt.

**Bewertungspreis**
Eingabe des EK-Preises, zu dem der Warenzugang geliefert wurde.

**Buchungsdatum**
Das aktuelle Tagesdatum wird automatisch angezeigt. Es kann überschrieben werden.

**Bemerkung**
Sie können eine Bemerkung eingetragen oder aus der Kombobox auswählen. Die Bemerkung wird in der Lagerhistorie angezeigt.
⇨ “Lagerhistorie – Tabelle" auf Seite G-211
Über die Schaltfläche können Sie der Liste eine neue Bemerkung hinzufügen.
⇨ "Bemerkung (Lagerbewegung)" auf Seite G-204

#### Lagerorte

-   **Farbe:** Die Farbe wird nur bei Varianten angezeigt.
-   **Breite, Höhe:** Die Maße werden nur angezeigt, wenn das Produkt als Lagermaß oder Kiste angelegt ist.
-   **Inhalt:** Bei Lagerartikeln und Lagermaßen wird der Wert 1 angezeigt, bei Kisten die Anzahl der Blätter.
-   **Lagerort:** Lagerort in der Reihenfolge von Ebene 1 bis 4.
-   **Ident Nr.:** Kisten-ID (manuelle Buchung oder aus dem Wareneingang).
-   **Bestand:** Aktueller Bestand
-   **ME:** Mengeneinheit, mit der das Produkt im Lager geführt wird.
-   **Lief-Ident:** Kisten-ID des Lieferanten.

### Lagerbewegung – Umbuchung

**Pfad:** Lagerwirtschaft > Lagerbewegung > Register Umbuchung

In diesem Register buchen Sie Lagerartikel an einen anderen Lagerort. Beim Umbuchen eines Lagerorts wird immer der gesamte Bestand eines Lagerortes an einen anderen Lagerort umgebucht.

⇨ Tutorial, "So buchen Sie einen Lagerort um" auf Seite G-85

Wenn Sie die Option Protokoll beim Beenden aktiviert haben, wird automatisch die Lagerhistorie mit dem Register Tabelle angezeigt, wenn Sie den Dialog schließen.
⇨ "Lagerhistorie - Tabelle" auf Seite G-211

Die Felder in den Bereichen Lagerprodukt und Lagerorte sind zum Register Abgang beschrieben.
⇨ "Lagerbewegung - Abgang, Zugang" auf Seite G-199

#### Lagerort

**Lagerort**
Anzeige des aktuellen Lagerorts. Sie können einen anderen Lagerort zuweisen. In der Kombobox werden alle hinterlegten Lagerorte aufgelistet.

> **Lagerort <k.A.>**
> Auch wenn Sie eigene Lagerorte hinterlegt haben, bleiben die Lagerorte <k.A.> erhalten und können bebucht werden.

### Lagerbewegung – Blattanzahl

**Pfad:** Lagerwirtschaft > Lagerbewegung > Register Blattanzahl

In diesem Register korrigieren Sie den Inhalt von Kisten.
⇨ Kistenmanagement, "Kisteninhalt korrigieren (Blattanzahl)" auf Seite K-66

Wenn Sie die Option Protokoll beim Beenden aktiviert haben, wird automatisch die Lagerhistorie mit dem Register Tabelle angezeigt, wenn Sie den Dialog schließen.
⇨ "Lagerhistorie - Tabelle" auf Seite G-211

Die Felder in den Bereichen Lagerprodukt und Lagerorte sind zum Register Abgang beschrieben.
⇨ "Lagerbewegung - Abgang, Zugang" auf Seite G-199

#### Inhaltsänderung

**Inhalt**
Nur wenn Sie eine Kiste mit ID ausgewählt haben, wird die Anzahl der Blätter angezeigt, die in der Kiste vorhanden sein sollten. Diesen Wert können Sie korrigieren.

### Lagerbewegung – Aufbruch

**Pfad:** Lagerwirtschaft > Lagerbewegung > Register Aufbruch

In diesem Register lösen Sie Kisten auf, damit die einzelnen Blätter für die Produktion zur Verfügung stehen. Bei diesem Vorgang wird die Kiste aus dem Bestand ausgebucht und die Anzahl der Blätter werden dem Bestand des Lagermaßes zugebucht.

⇨ Kistenmanagement, "Kisten aufbrechen (auflösen)" auf Seite K-67

> **Kisteninhalt an einen anderen Lagerort buchen**
> Wenn Sie eine Kiste aufbrechen, wird der Inhalt an denselben Lagerort gebucht, an dem die Kiste steht. Wenn Sie den Inhalt umbuchen wollen, müssen Sie diesen am alten Lagerort ausbuchen und anschließend am neuen Lagerort zubuchen.

Wenn Sie die Option Protokoll beim Beenden aktiviert haben, wird automatisch die Lagerhistorie mit dem Register Tabelle angezeigt, wenn Sie den Dialog schließen.
⇨ "Lagerhistorie - Tabelle" auf Seite G-211

Die Felder in den Bereichen Lagerprodukt und Lagerorte sind zum Register Abgang beschrieben.
⇨ "Lagerbewegung - Abgang, Zugang" auf Seite G-199

#### Kistenaufbruch

Wenn eine Kiste mit Identnummer ausgeliefert oder geöffnet werden soll, die bereits einem Auftrag zugeordnet ist, wird eine Meldung angezeigt. Dadurch wird verhindert, dass durch den anschließenden Druck des Lieferscheins oder der Rechnung ein negativer Bestand entsteht.

**Anzahl Kisten**
Anzahl der Kisten, die aufgebrochen werden sollen.

**Abweichender Inhalt**
Nur wenn Sie eine Kiste ausgewählt haben, wird die Anzahl der Blätter angezeigt. Sie können diesen Wert korrigieren.

### Bemerkung (Lagerbewegung)

**Pfad:** Lagerwirtschaft > Lagerbewegung > [Bemerkung]

In diesem Dialog hinterlegen Sie Bemerkungen, die im Dialog Lagerbewegung zur Auswahl angeboten werden. Wenn Sie die erste Zeile leer lassen, können Sie eine zugewiesene Bemerkung auch wieder entfernen.

## Abfragen

**Pfad:** Lagerwirtschaft > Abfragen

Über die verschiedenen Abfragen können Sie sich einen schnellen Überblick über Bestände, Bewegungen und Werte in Ihren Lägern verschaffen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:

-   "Buchungsjournal" auf Seite G-205
-   "Lagerhistorie" auf Seite G-207
-   "Lagerstatistik" auf Seite G-212
-   "Reservierte Lagerartikel" auf Seite G-218

### Buchungsjournal

**Pfad:** Lagerwirtschaft > Abfragen > Buchungsjournal

In diesem Dialog wählen Sie die Kriterien für die Abfrage aus. Im Buchungsjournal werden alle automatischen Auftrags- bzw. Bestellvorgänge protokolliert, die das Lager betreffen, z. B. Reservierungen, Bestellungen, Zu- und Abgänge.

⇨ Tutorial, "Buchungsjournal anzeigen" auf Seite G-90

#### Auswahl

**Buchungsart**
Sie können das Lager nach folgenden Buchungsarten durchsuchen:

-   **(Keine Angabe):** Wenn Sie keine Buchungsart angeben, werden alle Artikel angezeigt.
-   **Reserviert:** Nur die reservierten Artikel werden angezeigt. Ein Artikel ist so lange reserviert, bis der Lieferschein oder die Rechnung gedruckt wurde.
-   **Ausgeliefert:** Nur die ausgelieferten Lagerartikel werden angezeigt. Ein Artikel wird als ausgeliefert gekennzeichnet, wenn der Lieferschein oder die Rechnung gedruckt wurde.
-   **Bestellt:** Nur die bestellten Lagerartikel werden angezeigt. Das Kennzeichen wird durch eine Lagerbestellung gesetzt.
-   **Empfangen:** Nur die gelieferten Lagerartikel werden angezeigt. Ein Artikel gilt dann als geliefert und empfangen, wenn er im Wareneingang verbucht wurde.

**Buchungszeitpunkt von ... bis**
Sie können die Suche auf ein Datum oder einen Zeitraum einschränken, in dem die Artikel im Lager gebucht wurden. Achten Sie bei der Auswahl des Datums auf die Angabe der Uhrzeit, zu der die Buchung durchgeführt wurde.
Wenn Sie die Anzeige nicht weiter eingeschränkt haben, werden alle Buchungen im angegebenen Zeitraum angezeigt.

**Lagerort**
Sie können die Suche auf einen Lagerort einschränken.

> **Lagerort <k.A.>**
> Auch wenn Sie eigene Lagerorte hinterlegt haben, bleiben die Lagerorte <k.A.> erhalten und können bebucht werden.

**Ident-Nr.**
Sie können die Suche auf eine Kisten-ID einschränken.

**Auswahl nach**
Mit der Wahl der Option legen Sie fest, auf was sich die Suche beziehen soll:

-   **Artikel:** Sie können nach einem oder mehreren Artikeln suchen. Die Eingabe in den Feldern Nummer von und bis bezieht sich auf die Produktnummern. Wenn Sie keine Buchungsart gewählt haben, werden alle Buchungsarten aufgelistet.
-   **Auftrag:** Sie können nach Artikeln suchen, die in Aufträgen enthalten sind. Die Eingabe in den Feldern Nummer von und bis bezieht sich auf die Auftragsnummern.

**Nummer von, bis**
Die Suche kann auf eine Nummer oder eine Folge von Nummern eingeschränkt werden.

#### Tabelle

In der Übersicht wird das Ergebnis der Suche angezeigt.

-   **Buch. Typ:** Buchungsart, in der das Produkt gebucht wurde.
-   **Auftr. Nr./Bestell. Nr.:** Nummer des Auftrags oder der Bestellung, aus denen die Buchung erzeugt wurde.
-   **Pos. Nr.:** Nummer der Auftrags- oder Bestellposition.
-   **Menge:** Menge der Position.
-   **Produkt, Bezeichnung:** Nummer und Bezeichnung aus den Stammdaten.
-   **Farbe:** Nur bei Varianten wird eine Farbe angezeigt.
-   **Breite, Höhe:** Maße der Position.
-   **Ident-Nr.:** Kisten-ID (manuelle Buchung oder aus dem Wareneingang). Wenn der Eintrag keine Kiste darstellt, wird eine Null angezeigt.
-   **Lief.-Ident:** Kisten-ID des Lieferanten.
-   **Lagerort:** Ort, bei dem das Produkt ab- oder zugebucht wurde.
-   **Buch. Datum:** Datum des Wareneingangs.
-   **EK:** Einkaufspreis der Position. Jede Änderung des EK im Wareneingang, bei der Kontrolle der Lieferanten-AB oder der Rechnung wird in die Bestellung zurückgeschrieben.

### Lagerhistorie

**Pfad:** Lagerwirtschaft > Abfragen > Lagerhistorie

In der Lagerhistorie werden alle Vorgänge protokolliert, die das Lager betreffen. Das sind neben den Buchungsarten z. B. auch die verschnittenen Lagerplatten, Korrekturen, neue Artikel.

Im Dialog Lagerhistorie finden Sie folgende Register:

-   Lagerhistorie - Auswahl
-   Lagerhistorie – Tabelle

#### Lagerhistorie – Auswahl

**Pfad:** Lagerwirtschaft > Abfragen > Lagerhistorie > Register Auswahl

In diesem Register wählen Sie die Kriterien für die Abfrage aus. Das Ergebnis wird automatisch im Register Tabelle angezeigt.
➡Tutorial, "Lagerbewegungen" auf Seite G-79
Tutorial, "Buchungsjournal anzeigen" auf Seite G-90

**Buchungsart**
Sie können das Lager nach folgenden Buchungsarten durchsuchen:

-   **(Keine Angabe):** Wenn Sie keine Buchungsart angeben, werden alle Artikel angezeigt.
-   **Reserviert:** Nur die reservierten Artikel werden angezeigt. Ein Artikel ist so lange reserviert, bis der Lieferschein oder die Rechnung gedruckt wurde.
-   **Ausgeliefert:** Nur die ausgelieferten Lagerartikel werden angezeigt. Ein Artikel wird als ausgeliefert gekennzeichnet, wenn der Lieferschein oder die Rechnung gedruckt wurde.
-   **Verschnittenes LM:** Diese Buchungsart wird von der A+W Optimizer-Rückmeldung verwendet, wenn eine Position aus einem Lagermaß zugeschnitten wurde. Die Anzahl der Lagerplatten wird ausgewertet.
-   **Bestellt:** Nur die bestellten Lagerartikel werden angezeigt. Das Kennzeichen wird durch eine Lagerbestellung gesetzt.
-   **Empfangen:** Nur die gelieferten Lagerartikel werden angezeigt. Ein Artikel gilt dann als geliefert und empfangen, wenn er im Wareneingang verbucht wurde.
-   **Lagereingang/Lagerausgang manuell:** Nur manuell gebuchte Lagerzu- oder Lagerabgänge werden angezeigt.
-   **Lagerumbuchung:** Nur Lagerumbuchungen werden angezeigt.
-   **Neuanlage:** Nur die Artikel werden angezeigt, die neu ins Lager aufgenommen wurden. Die Daten können im Rahmen einer Inventur oder manuell angelegt worden sein. Berücksichtigt werden alle neuen Artikel ab der letzten Archivierung.
-   **Korrektur:** Nur die Artikel werden angezeigt, deren Bestände bei der Inventur bearbeitet wurden. Berücksichtigt werden alle Korrekturen ab der letzten Archivierung.
-   **Umbuchung auf Papierkorb, Rückbuchung vom Papierkorb, Aus Lager gelöscht:** Interne Buchungsarten.

**Programm**
Sie können die Suche auf Artikel einschränken, die in einem bestimmten Dialog der Lagerwirtschaft bearbeitet wurden, z. B. Lagerumbuchungen.

**Bemerkungstext**
Sie können die Suche auf die Artikel einschränken, zu denen eine bestimmte Bemerkung hinterlegt ist. Die Bemerkung wird unter dem Eingabefeld angezeigt.

**Artikel/Auftragsnummer**
Mit der Wahl der Option schränken Sie die Suche auf bestimmte Artikel oder Aufträge ein:

-   **Nach Artikel von ... bis:** Sie können einen oder mehrere Artikel auswählen.
-   **Nach Dokumentennummer von ... bis:** Sie können einen oder mehrere Aufträge oder Bestellungen auswählen.

> **Tagesaktivitäten anzeigen**
> Wenn Sie in beiden Feldern dieselbe Artikel- bzw. Auftragsnummer eintragen, werden alle Aktivitäten angezeigt, die in einem bestimmten Zeitraum zu einem Artikel oder Auftrag gebucht wurden. Geben Sie dazu auch den Buchungszeitpunkt mit der Uhrzeit an.

**Lager-ID/Serial-Nr.**

**Lager-ID von ... bis**
Sie können eine oder mehrere Lager-IDs auswählen.

**Ident-Nr. / Lief.-Ident von ... bis**
Sie können eine oder mehrere IDs auswählen. Die Ident-Nr. bezieht sich auf die Kiste, die Lief.-Ident auf die Kisten-ID des Lieferanten.

**Lagerorte**
Sie können die Suche auf Lagerartikel einschränken, die von einer bestimmten Ebene des Lagerorts an eine anderen bestimmte Ebene des Lagerorts umgebucht wurden.

**Mitarbeiter/Buchungsdatum**

**Mitarbeiter**
Sie können die Suche auf Artikel einschränken, die vom gewählten Mitarbeiter bearbeitet wurden.

**Buchungszeitpunkt von ... bis**
Sie können die Suche auf einen Buchungszeitraum einschränken. Achten Sie bei der Eingabe darauf, dass die Uhrzeit mit angegeben werden muss.

#### Lagerhistorie – Tabelle

**Pfad:** Lagerwirtschaft > Abfragen > Lagerhistorie > Register Tabelle

In diesem Register wird das Ergebnis der Abfrage angezeigt.

**Tabelle**

-   **Buch. Typ:** Buchungsart, in der das Produkt gebucht wurde.
-   **Auftr./Bestell., Pos.:** Nummer des Auftrags/der Bestellung und der Position, aus denen die Buchung erzeugt wurde.
-   **Menge:** Menge der Position.
-   **Ident, Lief.-Ident:** Kisten-ID (manuelle Buchung oder aus dem Wareneingang) und Kisten-ID des Lieferanten.
-   **Produkt, Bezeichnung:** Nummer und Bezeichnung aus den Stammdaten.
-   **Farbe:** Nur bei Varianten wird eine Farbe angezeigt.
-   **Breite, Höhe:** Maße der Position.
-   **Inhalt:** Anzahl der Blätter bei Kisten.
-   **EK/PE:** Einkaufspreis pro Preiseinheit.
-   **Gesamt EK:** Einkaufspreis der Position.
-   **PE:** Preiseinheit des Gesamt-EK.
-   **ME:** Mengeneinheit der Position.
-   **Buch. Datum:** Datum und Uhrzeit der Buchung.
-   **Ausf. Datum:** Datum und Uhrzeit, zu denen der Vorgang gebucht wurde.
-   **Von Lagerort, Nach Lagerort:** Alter und neuer Lagerort bei Umbuchungen.
-   **Mitarbeiter, Programm:** Name des Mitarbeiters, der den Vorgang gebucht hat, und Name des Dialogs, in dem die Buchung durchgeführt wurde.
-   **Bemerkung:** Bei bestimmten Buchungsarten wird eine Bemerkung angezeigt, z. B. welche Korrektur bei der Inventur vorgenommen wurde.

### Lagerstatistik

**Pfad:** Lagerwirtschaft > Abfragen > Lagerstatistik

Die Lagerstatistik gibt Ihnen Aufschluss darüber, welche Ihrer Lagerartikel Renner und welche Ladenhüter sind. Die Auswertungen zeigen Anfangs- bzw. Endbestände und Zu- bzw. Abgänge Ihrer Lagerartikel pro Monat. Damit können Sie sich über die Umschlagshäufigkeit, die durchschnittliche Lagerdauer und den durchschnittlichen Lagerbestand Ihrer Produkte informieren.

Im Dialog Lagerstatistik finden Sie folgende Register:

-   Lagerstatistik - Produkte
-   Lagerstatistik - Statistik
-   Lagerstatistik – FIFO/LIFO

#### Lagerstatistik – Produkte

**Pfad:** Lagerwirtschaft > Abfragen > Lagerstatistik > Register Produkte

In diesem Register legen Sie die Kriterien für die statistische Auswertung fest. Wenn Sie einen Eintrag in der Trefferliste markieren, werden die zugehörigen Details im Register Statistik angezeigt.

⇨ Tutorial, "So lassen Sie sich die Statistik zu Lagerbeständen anzeigen" auf Seite G-94

**Auswahl**

**Jahr**
Auswahl des Jahres, aus dem die Daten ausgewertet werden sollen. Damit können Sie einen bestimmten Zeitraum mit demselben Zeitraum des Vorjahres vergleichen.

**Monat von ... bis**
Die Auswahl der Monate bezieht sich immer auf das eingestellte Jahr. Wenn Sie mehr als ein Jahr auswerten möchten, müssen Sie die Auswertung splitten. Wenn Sie eine Auswertung über den Jahreswechsel hinaus benötigen, müssen Sie zwei Auswertungen nacheinander durchführen.

**Produkt von ... bis**
Auswahl eines Produkts oder einer Folge von Produkten. Zu jeder Produktnummer werden alle zugehörigen Lagerartikel ausgewertet, z. B. zum Produkt Float 4 mm alle Lagermaße, Kisten, Lagerorte usw.

**Übersicht**
In der Übersicht werden alle Lagerartikel aufgelistet, die den Suchkriterien entsprechen. Wenn Sie einen Eintrag der Trefferliste markieren, werden die zugehörigen Details im Register Statistik angezeigt.

-   **Produkt:** Produktnummer aus den Stammdaten.
-   **Bezeichnung:** Bezeichnung aus den Stammdaten.
-   **Breite, Höhe:** Maße für die hinterlegten Lagermaße.
-   **Inhalt:** Anzahl der Blätter einer Kiste.
-   **Ident:** Kisten-ID (manuelle Buchung oder aus dem Wareneingang).
-   **Farbe:** Nur bei Varianten, die auf Lager gehalten werden.
-   **Lagerort:** Lagerort des Lagerartikels.

> **Lagerort <k.A.>**
> Auch wenn Sie eigene Lagerorte hinterlegt haben, bleiben die Lagerorte <k.A.> erhalten und können bebucht werden.

#### Lagerstatistik – Statistik

**Pfad:** Lagerwirtschaft > Abfragen > Lagerstatistik > Register Statistik

In diesem Register werden Details für den Eintrag angezeigt, der in der Trefferliste im Register Produkte markiert ist.

**Lagerartikel**
In diesem Bereich werden die Daten des markierten Lagerartikels angezeigt.

-   **Produkt:** Produktnummer und Bezeichnung aus den Stammdaten.
-   **Breite / Höhe:** Maße für die hinterlegten Lagermaße.
-   **Lagerort:** Lagerort des Lagerartikels.
-   **EK:** Durchschnitts-EK und Mengeneinheit.
-   **Inhalt:** Anzahl der Blätter einer Kiste.

**Übersicht**
In der Übersicht werden die statistischen Werte für den Lagerartikel pro Monat angezeigt.

-   **Monat:** Je nach Auswahl werden einzelne Monate oder das gesamte Jahr dargestellt.
-   **Anf.-bestand:** Als Anfangsbestand wird der Endbestand des Vormonats herangezogen.
-   **Zugang:** Summe aller Zugänge innerhalb des Monats. Bei den Zugängen handelt es sich u. a. um neu angelegte Lagerartikel, um manuelle Zubuchungen in der Lagerbewegung und/oder Wareneingänge aus dem Einkauf.
-   **Abgang:** Summe aller Abgänge innerhalb des Monats. Abgänge werden entweder bei Lieferschein- und/oder Rechnungsdruck automatisch gebucht oder als manuelle Lagerbewegung.
-   **Endbestand:** Berechnung: Anfangsbestand + Zugang - Abgang (innerhalb des Monats).
-   **Umschlagshäufigkeit:** Berechnung: Lagerabgang + durchschnittlicher Lagerbestand. Je höher der Wert, desto geringer ist die Verweildauer der Produkte im Lager.
-   **Durchschnittliche Lagerdauer (in Tagen):** Berechnung: Tage der Abrechnungsperiode + Umschlagshäufigkeit. Anzahl der Tage, die benötigt werden, um beim derzeitigen Abgang den aktuellen Endbestand abzubauen.
-   **Durchschnittlicher Lagerbestand:** Berechnung: (Anfangsbestand + Endbestand) / 2.
-   **Anfangswert/Zugangswert/Abgangswert/Endwert:** Die Lagerwerte werden auf der Basis des Einkaufspreises ermittelt.
-   **Summe Lagerbestand:** Berechnung: = (Anfangsbestand + (n * Endbestand)) / (n + 1), n = Anzahl der Monate.

#### Lagerstatistik – FIFO/LIFO

**Pfad:** Lagerwirtschaft > Abfragen > Lagerstatistik > Register FIFO/LIFO

In diesem Register werden die im Lager geführten Artikel nach dem FIFO und/oder LIFO Verfahren bewertet angezeigt. Die gewünschte Anzeige wählen Sie im Menü Optionen > Berechnung.

Die Daten werden erst angezeigt, wenn Sie im Dialog Lagerbewertung eine Berechnung der Lagerwerte gestartet haben.
⇨ "Lagerbewertung" auf Seite G-230

**Übersicht**
In der Übersicht werden die statistischen Werte für den Lagerartikel pro Monat angezeigt.

-   **Datum:** Datum der Bewertung oder der Inventur.
-   **Zugang:** Summe aller Zugänge im ausgewählten Bewertungszeitraum.
-   **ME:** Mengeneinheit des Lagerartikels.
-   **Preis, PE:** Preis und Preiseinheit
-   **Restmenge FIFO:** Verbleibende Menge nach der Berechnung.
-   **Preis FIFO:** Preis der verbleibenden Menge nach der FIFO-Berechnung.
-   **Restmenge LIFO:** Verbleibende Menge nach der Berechnung.
-   **Preis LIFO:** Preis der verbleibenden Menge nach der LIFO-Berechnung.

Ein Berechnungsbeispiel finden Sie im Abschnitt Lagerbewertung:
⇨ "Lagerbewertung" auf Seite G-229

### Reservierte Lagerartikel

**Pfad:** Lagerwirtschaft > Abfragen > Reservierte Lagerartikel

Über diesen Dialog können Sie sich die Aufträge eines Nummernverwalters anzeigen lassen, um zu prüfen, welche Lagerartikel reserviert sind. Die reservierten Artikel werden im Ausdruck aufgeführt.

⇨ Tutorial, "Lagerführungsmodus und Reservierung" auf Seite G-30
⇨ Tutorial, "So drucken Sie sich die Liste der reservierten Lagerartikel" auf Seite G-92

**Auswahl**

-   **Mitarbeiter:** Name des angemeldeten Mitarbeiters.
-   **Nummernverwalter:** Auswahl des Nummernverwalters, dessen Aufträge ausgewertet werden sollen.

**Tabelle**

-   **Nummer:** Auftragsnummer.
-   **Nummer Kunde/Lief.:** Kundennummer.
-   **Kunde/Lieferant:** Name des Kunden oder Lieferanten.
-   **Status:** Status des Auftrags.
-   **Datum Erfassung:** Datum, an dem der Auftrag erfasst wurde.
-   **Datum Lieferung:** Datum, zu dem der Auftrag geliefert werden soll.
-   **Datum AB:** Datum der Auftragsbestätigung durch den Lieferanten.
-   **Sperr-KZ:** Sperrkennzeichen aus dem Auftrag.

**Gedruckte Liste**
Die reservierten Lagerartikel werden pro Artikelnummer und Lagerort aufgelistet. Bei mehreren Lagerorten wird die Gesamtsumme angezeigt.

## Suche

**Pfad:** Lagerwirtschaft > Suche

Sie können den Lagerbestand nach einzelnen Lagerartikeln oder nach Warengruppen abfragen.

> **Filter setzen**
> Wenn keine Filter gesetzt sind, werden keine Daten angezeigt.

Der Dialog ist ausführlich im Part Verkauf beschrieben.
⇨ Verkauf, "Lagerinfo" auf Seite C-758

Im Dialog Lagersuche finden Sie folgende Register:

-   Lagersuche - Lagersuche
-   Lagersuche - Zukünftiger Lagerbestand

### Lagersuche – Lagersuche

**Pfad:** Lagerwirtschaft > Suche > Register Lagersuche

In diesem Register können Sie sich die aktuellen Bestände, die reservierten Mengen und die zukünftigen Bestände zu Lagerartikeln anzeigen lassen.

⇨ Tutorial, "Lagerführungsmodus und Reservierung" auf Seite G-30
⇨ Tutorial, "Bestände in der Lagersuche anzeigen" auf Seite G-102

### Lagersuche – Zukünftiger Lagerbestand

**Pfad:** Lagerwirtschaft > Suche > Register Zukünftiger Lagerbestand

In diesem Register können Sie prüfen, ob die Wiederbeschaffungszeiten für ein bestimmtes Produkt ausreichen, um einen Auftrag termingerecht ausliefern zu können. Die Farbe Rot zeigt an, dass die Termine nicht eingehalten werden können. Gelb zeigt an, dass die Wiederbeschaffungszeit ausreicht, sofern die Bestellungen termingerecht eintreffen.

⇨ Tutorial, "Lagerinfo und zukünftiger Lagerbestand" auf Seite G-99

Die Wiederbeschaffungszeit ergibt sich aus der Lieferzeit, die in der Lieferantenkartei für den Artikel hinterlegt ist, und aus den Tourentagen des Lieferanten, die in der Tourenverwaltung hinterlegt sind.

Über die Checkbox Tage ohne Reservierungen und Bestellung anzeigen können Sie sich für eine bessere Übersicht die Tage ohne Reservierungen und Bestellungen ein- oder ausblenden.

Um die Performance zu erhöhen, können Sie die Anzeige der Vorschau durch folgende Einstellungen einschränken:

-   Im Dialog Produktverwaltung > Register Lager/Einkauf > Checkbox keine Verfügbarkeitsprüfung können Sie bestimmte Artikel aus der Lagervorschau und der Verfügbarkeitsprüfung herausnehmen, indem Sie die Verfügbarkeitsprüfung für diese Artikel ausschalten.
-   Im Dialog Firmendaten können Sie einstellen, über welchen Zeitraum die Vorschau dargestellt werden soll.
    ⇨ Tutorial, "Einstellung prüfen" auf Seite G-64
-   Im Dialog Lagerverwaltung können Sie mehrere Lagermaße miteinander verknüpfen, damit die Bestandsprüfung nur für den definierten Lager-Hauptartikel durchgeführt wird.
    ⇨ "Hauptartikel" auf Seite G-190

## Lagerbestellung

**Pfad:** Lagerwirtschaft > Lagerbestellung

In diesem Dialog können Sie alle vorgeschlagenen Lagerbestellungen prüfen und an den Einkauf übergeben.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:

-   "Menüs im Bestellpool" auf Seite G-223
-   "Lagerbestellung" auf Seite G-226

### Menüs im Bestellpool

Über die Menüs können Sie automatisch die Datumsfelder aktualisieren lassen und zusätzlich andere Dialoge öffnen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:

-   "Menü Funktionen" auf Seite G-223
-   "Menü Optionen" auf Seite G-224

#### Menü Funktionen

**Pfad:** Lagerwirtschaft > Lagerbestellung > Menü Funktionen

Über dieses Menü können Sie andere Dialoge öffnen, ohne die Bestellübergabe zu schließen. Folgende Einträge werden angezeigt:

-   **Lieferant/Liefertermine ändern:** Öffnet den Dialog Lieferant und Liefertermine ändern.
    "Lieferant und Liefertermin ändern" auf Seite C-678
-   **Markierungsoptionen:** Öffnet den Dialog Markierungsoptionen.
    ⇨ "Markierungsoptionen" auf Seite C-679
-   **Lieferantenpreise:** Öffnet den Dialog Preisvergleich.
    ⇨ "Preisvergleich" auf Seite C-680

#### Menü Optionen

**Pfad:** Lagerwirtschaft > Lagerbestellung > Menü Optionen

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

> **Aktivierte Optionen nach dem Öffnen des Dialogs**
> Bitte beachten Sie, dass geänderte Optionen erst beim nächsten Öffnen des Dialogs wirksam werden.
> Wenn durch eine aktivierte Option eine Prüfung gestartet wurde, kann sich das Öffnen eines Dokuments verzögern. Der Grad der Verzögerung hängt von der Leistungsfähigkeit des Rechners ab.
> Die folgenden Beschreibungen stellen die aktivierte Option dar.

Das Menü ist in folgende Gruppen gegliedert:

-   Gruppe Übergabe
-   Gruppe Liefertermin
-   Gruppe Produktbezeichnung
-   Gruppe Sonstige
-   Gruppe Erweitert

##### Gruppe Übergabe

-   **Auftragsbezogene Übergabe:** Die Bestellungen werden pro Auftrag übergeben. Wenn diese Option nicht aktiviert ist, können Sammelbestellungen erzeugt werden.
-   **Bestellnummer = Auftragsnummer:** Diese Option ist nur freigeschaltet, wenn die Option Auftragsbezogene Übergabe aktiviert ist.
-   **Bestellpool pro Mitarbeiter:** Pro Mitarbeiter kann ein eigener Bestellpool angelegt werden.

##### Gruppe Liefertermin

-   **Lieferterminprüfung:** Der Liefertermin wird automatisch geprüft. Ändern Sie einen Liefertermin, der nicht an einem Tourentag liegt, wird eine entsprechende Meldung angezeigt.
-   **Lieferantentour berücksichtigen:** Wenn die Bestellung auf einen Liefertermin fällt, der nicht an einem Tourentag liegt, wird eine entsprechende Meldung angezeigt. Dazu müssen die Lieferantentouren in den Stammdaten hinterlegt werden.
    ⇨ Stammdaten, "Touren" auf Seite B-873
-   **Vorlauftage mit Kombiwarengruppe ermitteln:** Wenn in den Kombiwarengruppen Vorlauftage hinterlegt sind, sollen diese zur Berechnung des Liefertermins herangezogen werden.
    ⇨ Stammdaten, "Vorlauftage" auf Seite B-576

##### Gruppe Produktbezeichnung

-   **Produktbezeichnungen aus Lieferantenkartei:** Die Bezeichnung der bestellten Produkte wird aus der Lieferantenkartei übernommen.
-   **Produktbezeichnungen aus Basisdaten (interne Best.):** Für interne Bestellungen wird die Bezeichnung der bestellten Produkte aus den Produktstammdaten übernommen.

##### Gruppe Sonstige

-   **Keine Kostenrückschreibung:** Die Kosten werden nicht in die EK-Preise des Auftrags zurückgeschrieben.
-   **Maßzuschläge berücksichtigen:** Bei der Bestellung sollen die Maßzuschläge mit übergeben werden.
-   **Druckkennzeichen für Bearbeitungen immer setzen:** In der Bestellung sollen Bearbeitungen immer gedruckt werden. Wenn die Option deaktiviert ist, werden die Druckkennzeichen unverändert aus dem Auftrag in die Bestellung übernommen.
-   **Statistikwarengruppe aus dem Auftrag:** Die Angabe zur Statistikwarengruppe wird aus dem Auftrag übernommen, wenn für Auftrag und Bestellung unterschiedliche Statistikwarengruppen definiert sind.
-   **Geschäftsart aus dem Auftrag:** Die Geschäftsart wird aus dem Auftrag übernommen, wenn für Auftrag und Bestellung unterschiedliche Geschäftsarten definiert sind.
-   **AV-Bereich aus dem Auftrag:** Der AV-Bereich wird aus dem Auftrag übernommen, wenn für Auftrag und Bestellung unterschiedliche AV-Bereiche definiert sind.
-   **Fachberater = Erfasser bei Neuanlage:** In der Bestellung wird automatisch der Name des Mitarbeiters eingetragen, der sich in A+W Business angemeldet hat.
-   **Statusänderung erfragen:** Die Abfrage zur Änderung des Status wird angezeigt.
-   **Wiederholte Übergabe nur bis Sperrstatus:** Bestellungen können mehrfach übergeben werden, allerdings nur, bis der Sperrstatus erreicht ist.

##### Gruppe Erweitert

-   **Einstellungen:** Öffnet den Dialog Erweiterte Einstellungen, um Angaben zum Druck von Texten und Dateianhängen festzulegen.

### Lagerbestellung

**Pfad:** Lagerwirtschaft > Lagerbestellung

In diesem Dialog können Sie alle vorgeschlagenen Bestellungen für Artikel sehen, deren Mindestbestand unterschritten wurde. Die Bestellmenge wird nach der Menge berechnet, die im Dialog Lagerverwaltung festgelegt ist.

Mit der Übergabe werden die Bestellungen angelegt und können gedruckt und versendet werden.

⇨ Tutorial, "Lagerbestellung (automatisch)" auf Seite G-107
⇨ Tutorial, "Bestellmenge nach Bestandsprüfung" auf Seite G-135

**Lagerort**
Warenhaus, Gang, Regal, Fach: Sie können die Anzeige auf einzelne Lagerorte einschränken. Bedenken Sie dabei, dass auch auf den Lagerort <k.A.> Lagerartikel gebucht sein können. Wenn Sie die Auswahl nicht einschränken, werden Bestellvorschläge zu allen Artikeln angezeigt, deren Mindestbestand unterschritten ist.
Die Bezeichnung der Lagerorte kann in den Stammdaten geändert werden.
⇨ Tutorial, "Lagerebenen festlegen" auf Seite G-22

#### Übersicht

In der Übersicht werden die Daten zu den Bestellvorschlägen angezeigt. Sie können einen anderen Lieferanten auswählen und sich einen Preisvergleich anzeigen lassen.

-   **Lieferant:** Der Lieferant wird aus der Lieferantenkartei übernommen. Wenn kein Lieferant eingetragen ist oder wenn Ihnen Lieferschwierigkeiten Ihres Standard-Lieferanten bekannt sind, können Sie den Namen ändern.
-   **Artikel/Farbe:** Nummer und ggf. Variante des Produkts, das bestellt werden soll.
-   **Ident-Nr.:** Kisten-ID (manuelle Buchung oder aus dem Wareneingang)
-   **Lagerort:** Lagerort, an dem der Bestand des Lagerartikels unterschritten ist.
-   **Menge:** Menge, die bestellt werden soll. Die Standard-Bestellmenge wird so oft multipliziert, bis der Mindestbestand überschritten ist. Sie können den Wert direkt in der Übersicht überschreiben.
-   **Breite, Höhe:** Maße der Scheibe, die bestellt werden soll.
-   **Inhalt:** Der Inhalt wird nur bei Kisten angezeigt.
-   **Anlief.-Lief.:** Der Liefertermin des Lieferanten wird aus den Angaben in der Lieferantenkartei errechnet. Wenn Ihnen Lieferschwierigkeiten Ihres Standard-Lieferanten bekannt sind, können Sie den Termin ändern.
    ⇨ Verkauf, "Lieferant und Liefertermin ändern" auf Seite C-678
    ⇨ Verkauf, "Preisvergleich" auf Seite C-680

**Position für**
Die Bestellvorschläge sind in unterschiedlichen Farben dargestellt:
-   **Rot: interner Auftrag:** Interne Aufträge sind Produktionsaufträge, die erzeugt werden, um den Lagerbestand aufzufüllen. Der Vorschlag wird automatisch erzeugt, wenn in der Lieferantenkartei für das Produkt die entsprechende Option aktiviert ist.
-   **Blau: Anfrage:** Bestellanfragen an einen Lieferanten, um z. B. Preise und Liefertermine zu erfragen.
-   **Grün: Liefertermin für Auftr./Best. gefährdet:** Als Liefertermin wird automatisch das aktuelle Tagesdatum eingesetzt. Damit ist die Lieferung i. d. R. nicht termingerecht möglich. Wenn Sie das Datum ändern, wechselt die Schriftfarbe für den Eintrag zu Schwarz.

#### Ziel-Nummernverwalter

**Mitarbeiter**
Name des Mitarbeiters, der sich in A+W Business angemeldet hat oder der den Nummernverwalter eingerichtet hat. Wenn Sie einen neuen Nummernverwalter anlegen, können Sie diesen einem bestimmten Mitarbeiter zuweisen.

**Name**
Name des Nummernverwalters, in den die Bestellungen übergeben werden sollen. Wenn Sie einen neuen Namen eintragen, wird ein neuer Nummernverwalter angelegt.

#### Ziel-Nummernkreis

**Mandant**
Wenn Sie für Ihre Mandanten gesonderte Nummernkreise eingerichtet haben, können Sie den gewünschten Mandanten auswählen.

**AV-Bereich**
Wenn Sie mit AV-Bereichen arbeiten, können Sie die Bestellung einem bestimmten AV-Bereich zuordnen.

## Lagerbewertung

Bei der Lagerbewertung werden die Lagerbestände nach dem periodischen Verfahren bewertet. Dazu werden die Lagerabgänge der gesamten Periode zunächst summiert. Anschließend werden die Lagerabgänge von den Wareneingängen abgezogen. Dieser Vorgang hängt vom gewählten Verfahren ab:

-   **LIFO:** Die zuletzt eingegangenen Artikel werden zuerst abgezogen.
-   **FIFO:** Die zuerst eingegangenen Artikel werden zuerst abgezogen.

Der Lagerwert wird jeweils aus der nicht verbrauchten Menge berechnet. Dabei wird der Zeitraum von der letzten Lagerbewertung bis zum Auswertungszeitpunkt berücksichtigt.

**Beispiel**

| Lager | Artikel | Datum | Wert in € | Menge (Nach LIFO) | Wert |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 111 | 1.5.2016 | 8,50 | 15 (15) | 15*8,50 |
| 1 | 111 | 4.5.2016 | 8,70 | 20 (10) | 15*8,50 + 20*8,70 |
| 1 | 111 | 5.5.2016 | 8,20 | 10 (0) | 15*8,50 + 20*8,70 + 10*8,20 |

Der LIFO Wert beträgt (15*8,50+10*8,70) / 25 = 8,58

| Lager | Artikel | Datum | Wert in € | Menge (Nach FIFO) | Wert |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 111 | 1.5.2016 | 8,50 | 15 (15) | 15*8,50 |
| 1 | 111 | 4.5.2016 | 8,70 | 20 (10) | 15*8,50 + 20*8,70 |
| 1 | 111 | 5.5.2016 | 8,20 | 10 (0) | 15*8,50 + 20*8,70 + 10*8,20 |

Der FIFO Wert beträgt (15*8,70+10*8,20) / 25 = 8,50

*Tab. G-1 Berechnungsbeispiele*

> **Lagerartikel mit ID**
> Lagerartikel mit Identnummern können nicht nach FIFO/LIFO bewertet werden, da diese eindeutig identifizierbar sind. Von diesen Lagerartikeln ist entweder 1 oder kein Stück vorhanden. Daher gibt es keine Entnahmereihenfolge.
>
> Bei der Erstbewertung darf der Lagerbestand nicht negativ sein. Die Erstbewertung kann nur nach durchschnittlichem EK oder manuellem Wert erfolgen. Ab dem Zeitpunkt der Erstbewertung kann dann mit dem FIFO oder LIFO Verfahren gerechnet werden.

### Lagerbewertung

**Pfad:** Lagerwirtschaft > Lagerbewertung > Selektion

In diesem Dialog starten Sie die Berechnung des Lagerwerts.

Im Dialog Lagerbewertung finden Sie folgende Register:

-   Lagerbewertung – Selektion
-   Lagerbewertung – Bewertung

#### Menü Optionen

**Pfad:** Lagerwirtschaft > Lagerbewertung
Folgende Einträge werden angezeigt:

-   **Erstbewertung nach:** Für die Erstbewertung des Lagerbestands können Sie eines der folgenden Verfahren auswählen:
    -   FIFO, LIFO
    -   Durch. EK
    -   Manuell

### Lagerbewertung – Selektion

**Pfad:** Lagerwirtschaft > Lagerbewertung > Selektion

In diesem Register stellen Sie die Kriterien ein, nach denen der Lagerwert berechnet werden soll. Zusätzlich können Sie in den Firmendaten festlegen, wie der EK berechnet werden soll.

"Inventurliste" auf Seite G-169

#### Auswahl

**Nicht bewertet seit**
Angabe des letzten Bewertungsdatums. Sie können ein beliebiges Datum in der Vergangenheit wählen. Damit werden nur die Produkte bewertet, deren letzte Bewertung vor diesem Datum liegt. Der Bewertungszeitraum liege zwischen diesem Datum und dem Datum, das Sie im Feld Bewertung eintragen.

**Produkt von ... bis**
Auswahl der Produkte, die bewertet werden sollen.

**Produktart**
Auswahl der Produktart, deren Produkte bewertet werden sollen.

**Stat. Warengruppe**
Auswahl der Statistik-Warengruppe, die dem Produkt zugewiesen ist.

**Warenhaus, Gang, Regal, Fach**
Auswahl des Lagerorts, dessen Produkte bewertet werden sollen.

**Nur gültige Bestände (Bestand nicht negativ)**
Sie können Produkte von der Bewertung ausschließen, deren Bestand aufgrund von Reservierungen negativ ist.
- Alle Produkte werden bewertet, die den Auswahlkriterien in den Feldern Produkt und Produktart entsprechen.
- Nur die Produkte werden bewertet, deren Bestand nicht negativ ist. Darin sind auch Produkte enthalten, deren Bestand = 0 ist.

**Kein Glas mit Abmessungen (0x0)**
Für die kombinierte Lagerführung werden Produkte mit den Abmessungen 0x0 angelegt, auf die reservierte Mengen bis zum Abbuchen der verbrauchten Lagerplatten gebucht werden.
- Alle Produkte werden bewertet, die den Auswahlkriterien in den Feldern Produkt und Produktart entsprechen.
- Produkte mit den Abmessungen 0x0 werden nicht bewertet.

**Bewertung**
Angabe des Datums, zu dem die Lagerwertung berechnet werden soll. Damit können Sie eine Lagerbewertung in der Vergangenheit durchzuführen. Die Lagerbestände werden zu diesem Datum berechnet.

### Lagerbewertung – Bewertung

**Pfad:** Lagerwirtschaft > Lagerbewertung > Bewertung

In diesem Register werden zunächst die Artikel angezeigt, die den Auswahlkriterien entsprechen. Wenn Sie die Bewertung über eine der Schaltflächen gestartet haben, werden die berechneten Werte angezeigt.

Diese Werte werden auch in der Lagerstatistik angezeigt:
"Lagerstatistik – FIFO/LIFO" auf Seite G-217

Die Werte können gespeichert werden. Vor dem Speichern werden alle eingestellten Bewertungen nochmal auf ihre Konsistenz geprüft. Wenn hierbei ein Fehler festgestellt wird, wird dieser angezeigt und keiner der Sätze gespeichert. Sie müssen den Fehler bereinigen, um anschließend die Datensätze speichern zu können.

Wenn Sie die Daten gespeichert haben, können Sie die Bewertung nicht mehr ändern.

#### Bewertung

**Alle selektieren**
Sie können aus der Liste einzelne Produkte auswählen. Mit der Mehrfachauswahl können Sie beliebig viele Produkte markieren. Über die Schaltflächen können Sie alle Produkte auswählen oder die Auswahl vollständig aufheben.

**[LIFO berechnen]**
startet die Bewertung der markierten Produkte nach dem LIFO-Verfahren.

**[FIFO berechnen]**
startet die Bewertung der markierten Produkte nach dem FIFO-Verfahren.

**[Beide berechnen]**
startet die Bewertung der markierten Produkte nach dem beiden Verfahren.

**Bewertungsart ändern**
Auswahl der Bewertungsart. Die Änderung der Bewertungsart wirkt sich nur auf die markierten Einträge aus.

#### Übersicht

Folgende Spalten können angezeigt werden:

-   **Produkt, Bezeichnung:** Nummer und Bezeichnung des Produkts.
-   **Breite, Höhe:** Maße der Scheibe.
-   **Inhalt:** Inhalt eine Kiste.
-   **Farbe:** Farbvariante des Glases.
-   **Lagerort:** Vollständiger Lagerort.
-   **PE:** Preiseinheit des Produkts.
-   **Lagerbestand:** Aktueller Lagerbestand ohne Reservierungen.
-   **ME:** Mengeneinheit, in der das Produkt im Lager geführt wird.
-   **Bewertung:** Art der Bewertung:
    -   **Keine:** Der Bestand dieses Produkts wurde nicht berechnet.
    -   **LIFO, FIFO:** Der Lagerwert ist als LIFO-, FIFO-Wert berechnet.
    -   **Durch. EK:** Der Lagerwert ist ein durchschnittlicher EK-Wert.
    -   **Manuell:** Der Lagerwert ist manuell eingetragen.
-   **FIFO, LIFO:** Berechneter Lagerwert des Produkts.
-   **Durch. EK:** Durchschnittlicher Einkaufspreis. Dieser Preis wird nur berechnet, wenn in den Firmendaten die entsprechende Option aktiviert ist.
-   **Manuell:** Der Wert der manuellen Eingabe wird als Lagerwert eingetragen.
-   **Bemerkung FIFO/LIFO:** Anzeige des Status nach der Bewertung:
    -   **OK:** Der Bestand dieses Produkts wurde berechnet. Dieser Status ist bei der Erstbewertung nicht möglich.
    -   **Bestand ist negativ!:** Der Bestand dieses Produkts kann nicht berechnet werden, weil der Bestand negative Werte enthält.
    -   **Es wurde kein Anfangssatz gefunden:** Der Bestand dieses Produkts kann nur nach durchschnittlichen EK oder manuell bewertet werden.
    -   **Menge muss größer 0 sein:** Der Bestand dieses Produkts kann nicht berechnet werden, weil kein Bestand vorhanden ist.
-   **Letzte Bewertung:** Datum der letzten Lagerbewertung.
-   **Bewertung:** Wert der letzten Bewertung.

# Kapazitätsplanung

## Editorial

Das Editorial enthält Informationen zu folgenden Themen:
-   Anmerkungen zu diesem Dokument
-   Urheberrechte
-   Warenzeichen
-   Kontakte

### Revisionsübersicht

| Part Version/Datum | Beschreibung |
| :--- | :--- |
| 4.10/08-2017 | Strukturelle Überarbeitung. Dialoge Aggregate, Positionssplit, Vorgabezeiten aktualisiert. |
| 4.02/01-2017 | Produkt- und Firmennamen angepasst. |
| 4.01/02-2015 | Anpassung an A+W Business Pro. Rechtschreibkorrekturen. |
| 4.00/04-2014 | Vollständige Überarbeitung. |
| 3.00/08-2013 | Anpassung der ALFAK-Dokumentation auf A+W Business. |
| 2.00/05-2012 | Ersterstellung des Tutorials; Softwarereferenz vollständig überarbeitet. |
| 1.02/09-2010 | Layout an Doku-Konzept 2010 angepasst. |
| 1.01/08-2008 | Rechtschreibkorrekturen, grafische Tabellen umgewandelt, Abbildungen und Part-Nummerierung angepasst. |
| 1.00/12-2003 | Ersterstellung. |

### Anmerkungen zu diesem Dokument

Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Business Pro gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Dieses Dokument beschreibt die volle Ausbaustufe von A+W Business Pro.

### Urheberrechte

© 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung von A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

### Kontakte

A+W Software GmbH
Siemensstr. 3
D-35463 Fernwald
Germany

-   +49 64196620-0
-   Siemensstr. 3
-   Zentrale@a-w.com
-   http://www.a-w.com

## Tutorial

### Überblick

Das Tutorial zum Modul Kapazitätsplanung beschäftigt sich mit den Grundlagen der Planung von Produktionskapazitäten in A+W Business Pro. Das Tutorial baut auf den Kenntnissen zu den Stammdaten und zu Dokumenten auf.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

#### Themenblöcke

In diesem Tutorial finden Sie folgende Themenblöcke:
-   Stammdaten
-   Kapazitätsplanung

#### Vorausgesetzte Kenntnisse

Das Tutorial richtet sich an Teilnehmer, die in A+W Business die Kapazitäten planen und damit die Auslastung der Maschinen überwachen. Die Teilnehmer müssen das Konzept der Stammdaten in A+W Business und das Modul Dokumente kennen. Kenntnisse der Module Fertigung und Lagerwirtschaft sind von Vorteil.

### Dokumentation

Für das Modul Kapazitätsplanung stehen folgende Dokumente zur Verfügung:

| Format | Umfang |
| :--- | :--- |
| Handout | Ausdruck des Tutorials für die Schulung |
| PDF | Vollständige Unterlagen: Tutorial, Softwarereferenz, Index |
| Online-Hilfe <F1> | Kontextsensitive Dialog-Hilfe der A+W Business Pro-Softwarereferenz und Tutorials |

### Aufbau des Tutorials

Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

-   **Überblick**: Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
    -   Lernziele: Was soll vermittelt werden?
    -   Nutzen: Wofür können Sie dieses Wissen einsetzen?
    -   Merksätze: Welche Zusammenhänge müssen Sie sich merken?
-   **Konzepte**: Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.
-   **Übungen**: Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen und Lösungsvorschlägen.
-   **Querverweise**: Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf ergänzende Informationen in der Softwarereferenz und in anderen Parts hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.

### Darstellungskonventionen

Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

-   *Kursiv*: sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Nummernverwalter*.
-   **Fett**: sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B.: Geben Sie den Wert **0** ein.
-   `>`: Mit dem sogenannten Brotkrumenpfad ist der Weg kennzeichnet, auf dem Sie einen Dialog öffnen, z. B. `Fertigung > Kapazitätsplanung > Leitstand`.
-   `[]`: Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B.: Mit [OK] speichern Sie die Daten.
-   `<>`: Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B.: Mit <F1> öffnen Sie die Online-Hilfe.

#### Lesehinweis

Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.
Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

### Menü-Übersicht

Die Kapazitätsplanung in A+W Business Pro gliedert sich in zwei Bereiche: das Einrichten der Kapazitätsplanung und die Planung und Überwachung der Kapazitäten. Die zugehörigen Dialoge finden Sie in den Modulen Kapazitätsplanung und Fertigung. Diese beiden Module werden im Folgenden kurz vorgestellt.

#### Modul Kapazitätsplanung

Im Modul Kapazitätsplanung richten Sie die Stammdaten und weitere Vorgaben für die Planung der Kapazitäten ein.

##### Stammdaten

Das Menü Stammdaten ist in drei Untermenüs gegliedert:

-   **Allgemein:** In diesem Bereich richten Sie die allgemeinen Daten ein, z. B. Aggregat-Typen (Maschinentypen), Arbeitsarten, Übergangzeiten.
    ⇨ Softwarereferenz, "Allgemein" auf Seite H-195
-   **Organisation:** In diesem Bereich richten Sie die Stammdaten zur betrieblichen Organisation ein, z. B. Produktionsbereiche, Maschinen, Kalender und Restriktionen.
    ⇨ Softwarereferenz, "Organisation" auf Seite H-205
-   **Vorgabezeiten:** In diesem Bereich richten Sie die Daten zur Berechnung von Produktionszeiten ein, z. B. Vorgabezeiten und Sonderzeiten.
    ⇨ Softwarereferenz, "Vorgabezeiten" auf Seite H-229

##### Zuordnen

Hier ordnen Sie den Arbeitsarten z. B. die Produkte oder Warengruppen (WGR) zu. Zu einigen Arbeitsarten legen Sie einen Faktor für die Berechnung der Zeiten fest, wenn ein besonderer Aufwand dies erforderlich macht, z. B. bei der Fertigung von Modellen.
⇨ Softwarereferenz, "Zuordnen" auf Seite H-242

##### Sperren

Hier legen Sie fest, welche Maschinen nicht eingesetzt werden dürfen, wenn z. B. bestimmte Produkte oder Warengruppen in einem Auftrag erfasst sind.
⇨ Softwarereferenz, "Sperren" auf Seite H-259

##### Übersicht

Hier können Sie sich Übersichten über die Auslastung der Maschinen und Produktionsbereiche erstellen lassen.
⇨ Softwarereferenz, "Übersichten" auf Seite H-270

#### Modul Fertigung

Im Modul Fertigung lasten Sie die Aufträge in die Kapazitätsplanung ein und überwachen die Rückmeldungen aus der Produktion.
In diesem Modul finden Sie auch die Programmbereiche, in denen Sie die Aufträge an die Produktion übergeben. Diese werden im Part Fertigung beschrieben.

##### Einlasten

Im Menü Einlasten finden Sie folgende Dialoge:

-   **Nummernverwalter:** Im Nummernverwalter sammeln Sie die Aufträge für die manuelle Einlastung.
-   **Einlasten NV:** Über diesen Dialog lasten Sie die Aufträge ein.
-   **Einlasten Auftrag:** Über diesen Dialog lasten Sie einen einzelnen Auftrag ein.
-   **Aggregate Ausfall:** In diesem Dialog sperren Sie ein Aggregat für die Einlastung.
    ⇨ Softwarereferenz, "Einlastung" auf Seite H-282

##### Fertigmeldung

Im Menü Fertigmeldung finden Sie folgende Dialoge:

-   **Datum:** In diesem Dialog melden Sie die Aufträge an einem Aggregat fertig.
-   **Lauf:** In diesem Dialog melden Sie Aufträge pro Lauf fertig.
-   **Manuell:** In diesem Dialog melden Sie Aufträge komplett oder in Teilen fertig.
    ⇨ Softwarereferenz, "Produktionsmeldungen" auf Seite H-307

##### Produktionslisten

Hier erstellen Sie pro Maschine Listen über die Stückzahlen, die gefertigt werden müssen.
⇨ Softwarereferenz, “Produktionsmeldungen" auf Seite H-307

##### Fertigungsstand Auftrag

Hier können Sie den aktuellen Stand der Fertigung pro Auftrag prüfen und ggf. ausgelassene Fertigmeldungen nachholen.
⇨ Softwarereferenz, "Fertigungsstand Auftrag" auf Seite H-323

##### Leitstand

Hier prüfen Sie die Auslastung der Maschinen und schichten ggf. Aufträge um, indem Sie zugewiesene Aggregate, Schichten, Produktions- oder Liefertermine ändern.
⇨ Softwarereferenz, "Leitstand" auf Seite H-341

> **A+W Business Pro Capacity Planning vs. A+W Production Capacity Planning**
> In dieser Anleitung ist immer die Kapazitätsplanung in A+W Business Pro gemeint. Capacity Planning meint die Kapazitätsplanung von A+W Production.

### Grundgedanken der Kapazitätsplanung

Mit der Kapazitätsplanung können Sie die Auslastung Ihrer Produktionskapazitäten vorplanen und Produktions- und Zeitkosten ermitteln. Die Planungsdaten helfen Ihnen, Kapazitätsengpässe frühzeitig zu erkennen. Sie können dann in die Planung eingreifen und manuell korrigieren.

Dazu müssen Sie die Stammdaten der Kapazitätsplanung anlegen und so aufeinander abstimmen, dass die Abläufe in Ihrer Produktion abgebildet werden. Die nachfolgende Abbildung zeigt wie diese Stammdaten zusammenwirken am Beispiel der Vorgaben, aus denen die Termine für den Produktionsbeginn errechnet werden.

(Beschreibung des Diagramms auf Seite H-20: Aggregattypen, Produktionsbereiche und Arbeitsarten werden zu Aggregaten zusammengefasst. Diese, zusammen mit Kalender, Vorgabezeiten und Zuordnungen, fließen in die Terminberechnung für den Produktionsbeginn ein, welche sich auf die A+W Business Pro-Produktstammdaten auswirkt.)

In dieser Übersicht sehen Sie, wie z. B. Aggregate (Maschinen) bei der Planung der Kapazitäten eingesetzt werden:

-   Für die einzelnen Arbeitsarten sind pro Aggregat Vorgabezeiten hinterlegt, aus denen die (freie) Kapazität und die benötigte Zeit für eine Auftragsposition berechnet werden.
-   Pro Aggregat ist festlegt, an welchen Tagen es wie lange verplant werden kann (Schichtzeiten im Kalender).
-   Aus den Zeiten, die eine Position in einem Produktionsbereich verweilt (Übergangsmatrix, Übergangzeiten), den Schichtzeiten (Kalender) und Vorgabezeiten wird der Termin für die Fertigung einer Auftragsposition berechnet.

Wenn die Stammdaten der Kapazitätsplanung erfasst sind, können die Aufträge in die Kapazitätsplanung eingelastet werden. Alle Auftragspositionen und deren Stücklisten-Komponenten werden den entsprechenden Arbeitsarten zugeordnet. Danach werden die benötigten Maschinenzeiten und die Kosten berechnet. Gleichzeitig wird der Liefertermin geprüft und der Termin zum Beginn der Produktion berechnet. Während und/oder nach der Einlastung können Sie in die Planung eingreifen und Arbeitsgänge einer Auftragsposition manuell auf andere gleichartige Maschinen umbuchen.

Die aktuelle Planung überwachen Sie im Dialog Leitstand. Von diesem Dialog aus können Sie in die Planung eingreifen und sich verschiedenen Übersichten und Grafiken zur Auslastung anzeigen lassen.

Bei Anbindung an die Produktionssoftware A+W Production werden die Ergebnisse der Kapazitätsplanung (Grobplanung) an A+W Production übergeben. Von A+W Production werden wiederum Rückmeldungen an A+W Business Pro übergeben, wenn Aufträge bzw. Positionen in der Produktion fertig gemeldet wurden. Dies führt in A+W Business Pro u. a. zur Erhöhung des Auftrags- bzw. Positionsstatus. Die Daten über Maschinenkosten und -zeiten werden nach der Fertigstellung des Auftrags aktualisiert.

> **Zeit- und Kostenermittlung**
> Aus den Vorgaben der Kapazitätsplanung werden die Zeit- und Maschinenkosten errechnet. Mit dieser Grobplanung wird auch geprüft, ob die Aufträge termingerecht versandfertig werden. Die Kapazitätsplanung in A+W Business Pro hat keinen Einfluss darauf, an welchen realen Maschinen im Produktionsprozess die Aufträge tatsächlich gefertigt werden.

#### Nutzung der Kapazitätsplanung

Sie können mit der Kapazitätsplanung die Produktionskapazitäten aufgrund der Auftrags-, Maschinen- und Zeitdaten in A+W Business Pro planen. Dazu ist keine Anbindung an A+W Production erforderlich.

Folgende Hauptmerkmale charakterisieren die Kapazitätsplanung von A+W Business Pro:

-   Flexibles Anlegen der Stammdaten für die Kapazitätsplanung
-   Ermittlung von Kapazitätsengpässen
-   Prüfung des Liefertermins
-   Kalkulation der Produktionskosten
-   Leitstand mit Übersichten und Funktionen zum Umlasten
-   Bei Anbindung an die Produktions-Software A+W Production:
    -   Übergabe der Plandaten an A+W Production
    -   Rückmeldung der Ist-Daten an A+W Business Pro
    -   Vergleich von Soll- und Ist-Werten

> **Begriffsklärung**
> In A+W Business Pro und in dieser Dokumentation werden die Begriffe Kapazitätsplanung und Zeitwirtschaft synonym verwendet.

## Stammdaten (Kapazitätsplanung)

Die Kapazitätsplanung kann mit Hilfe der Stammdaten an unterschiedliche Unternehmensstrukturen und Produktionsprozesse angepasst werden.
In diesem Themenblock lernen Sie, wie die Stammdaten der Kapazitätsplanung zusammenwirken und wie Sie diese Daten anlegen und pflegen.

Dazu gehören folgende Lerneinheiten:

-   "Maschinen und Produktionsbereiche" auf Seite H-24
-   "Schicht- und Arbeitszeiten" auf Seite H-40
-   "Zuordnen der A+W Business Pro-Stammdaten" auf Seite H-107

### Rechteverwaltung

Fast alle Zugriffe auf die Stammdatendialoge der Kapazitätsplanung können über die Rechteverwaltung eingeschränkt werden.

### Historie

Jede Änderung des Auftragsstatus pro Produktionsbereich wird automatisch in der Auftrags-Historie dokumentiert. Damit können die Mitarbeiter, die nur Zugriffsrechte auf die Dokumente haben, immer erkennen, wann und welche Statusänderung im Auftragskopf durch die Kapazitätsplanung und die Rückmeldungen aus der Produktion verursacht wurde.

> **Stammdaten der Kapazitätsplanung**
> Die Stammdaten für Maschinen und Produktionsbereiche legen Sie im Modul Kapazitätsplanung an. Diese Stammdaten können nicht über die Dialoge im Modul Stammdaten angelegt werden.
> Wenn Sie die Einstellungen in den Stammdaten der Kapazitätsplanung geändert haben, müssen Sie A+W Business Pro neu starten, damit die Daten neu eingelesen werden.

### Reihenfolge zur Erfassung der Stammdaten

Beim Anlegen der maschinenbezogenen Stammdaten ist es sinnvoll, diese Reihenfolge einzuhalten:

1.  **Aggregattypen**, z. B. Schneidtische, ESG-Öfen, Versand usw.: Art und Umfang technischer Restriktionen von Maschinen werden u. a. über die Zuweisung zu Aggregattypen definiert.
    ⇨ "Aggregattypen und Aggregate" auf Seite H-26
2.  **Produktionsbereiche (Arbeitszentren)**: Produktion und Versand werden in Bereiche unterteilt, z. B. Zuschnitt, Kantenbearbeitung, Bohren, Kontrolle, Verpacken, usw.
    ⇨ "Produktionsbereiche (Arbeitszentren)" auf Seite H-32
3.  **Arbeitseinheiten**: Zu jedem einzelnen Aggregat wird festgelegt, wie viele Arbeitseinheiten die Berechnungsgrundlage der Kapazität bilden.
    ⇨ "Arbeitseinheiten" auf Seite H-45
4.  **Aggregate**, z. B. Bystronic-Schneidtisch, Lisec-Schneidtisch, ESG-Ofen A, ESG-Ofen B usw.: Nachdem Sie die Produktionsbereiche und Aggregattypen angelegt haben, erfassen Sie die einzelnen Maschinen und ordnen Sie den Produktionsbereichen und Aggregattypen zu.
    ⇨ "Aggregat anlegen" auf Seite H-35
5.  **Arbeitsarten (Vorgänge)**: Alle Arbeiten, für die Zeiten berechnet werden, müssen als Arbeitsart definiert werden, z. B. Schneiden, Schleifen, Bohren, Verpacken usw.
    ⇨ "Arbeitsarten" auf Seite H-30
6.  **Vorgabezeiten**: Die Zeiten für Arbeitsarten sind von den jeweiligen Maschinen abhängig. Die Zeiten der Arbeitsart Bohren sind z. B. von der Glasstärke und der Maschine abhängig, mit der gebohrt wird. Pro Maschine und Arbeitsart müssen daher Zeiten gemessen und erfasst werden. Über diese Vorgabezeiten werden den Arbeitsarten die Maschinen zugeordnet.
    ⇨ "Vorgabezeiten" auf Seite H-62
7.  **Zeitzuschläge**: Zusätzlich zu den Vorgabezeiten können Zeitzuschläge definiert werden, die auf den Basiswert aufgeschlagen werden, z. B. für den Zuschnitt von Modellen.
    ⇨ "Arbeitsarten und Zeitzuschläge" auf Seite H-66

## Maschinen und Produktionsbereiche

**Lernziele**
-   Zusammenhang von Aggregat-Typen und Aggregaten (Maschinen) kennenlernen.
-   Produktionsbereiche anlegen.
-   Arbeitsarten definieren und anlegen.

**Nutzen**
-   Mit den Stammdaten der Kapazitätsplanung bilden Sie die Abläufe in Ihrer Produktion ab. Damit beziehen sich die Plandaten auf die vorhandenen Maschinen.

**Merke**
-   **Aggregattyp**: Aggregattypen sind die Maschinentypen, die Sie in Ihrer Produktion einsetzen, z. B. Schneidtische, Bohrmaschinen, Schleifmaschinen, ESG-Öfen usw. Ein Aggregattyp kann mehrere einzelne Arbeitsstationen zusammenfassen, z. B. die ISO-Linie. Zu jedem Aggregattyp legen Sie fest, welche Restriktionen jeweils geprüft werden.
-   **Aggregat**: Aggregate sind alle Stationen, an denen Zeiten verbraucht werden. Neben den eigentlichen Maschinen zum Schneiden, Bohren usw. gilt auch Kontrolle, Versand, Verpacken als Aggregat. In A+W Business Pro gibt es keine logischen Maschinen.
-   **Produktionsbereich**: Produktionsbereiche fassen die Aggregate zusammen, die die gleichen Tätigkeiten ausführen oder in denen eine Folge von Tätigkeiten ausgeführt wird, z. B. ISO-Fertigung.
-   **Arbeitsart**: Die Arbeitsart bezeichnet die Tätigkeit, die an einem Aggregat ausgeführt wird. Alle Tätigkeit, für die Zeiten berechnet werden, müssen als Arbeitsart definiert werden, z. B. Schneiden, Schleifen, Bohren, Verpacken usw.
-   **Arbeitsgang**: Der Begriff bezeichnet in dieser Dokumentation die Ausführung einer Arbeitsart für eine Auftragsposition. In der Regel sind in einer Auftragsposition mehrere Arbeitsgänge nötig.
-   **Restriktionen**: Einschränkungen bei bestimmten Aggregaten (Maschinen), müssen geprüft werden.
    -   Diese Prüfungen werden übergreifend für den Aggregattyp aktiviert.
    -   In der Definition eines Aggregats legen Sie die Werte fest, die für die Prüfung herangezogen werden sollen und nicht über- oder unterschritten werden dürfen.

### Aggregattypen und Aggregate

Als Aggregate werden in der Kapazitätsplanung alle technischen Arbeitsmittel bezeichnet, an denen die Arbeitsschritte ausgeführt werden. Das können sowohl einzelne Maschinen als auch ganze Linien oder der Versand sein. Da unterschiedliche Maschinen gleiche Arbeitsschritte ausführen können, können jedem Aggregattyp mehrere Maschinen zugeordnet sein.

**Beispiel: Aggregattyp Zuschnitt und zugeordnete Aggregate**
Als Beispiel sehen Sie hier den Aggregattyp Zuschnitt, zu dem mehrere Aggregate (Maschinen) gehören. Bei der Planung der Kapazitäten werden die jeweils zur Verfügung stehenden Aggregate auf ihre Auslastung hin abgefragt. Dabei wird auch geprüft, ob beim jeweiligen Aggregattyp Einschränkungen (Restriktionen) geprüft werden müssen und ob die für die Maschine hinterlegten Werte durch die Auftragsposition verletzt werden.

#### Restriktionen

Zu jedem Aggregattyp legen Sie fest, welche Restriktionen jeweils geprüft werden müssen.

**Beispiel**
Bei Aggregattyp Zuschnitt sollen folgende Werte geprüft werden:

| Feld | Grund |
| :--- | :--- |
| Maße | Einer der Schneidtische kann eine bestimmte Größe der Lagerplatten nicht mehr aufnehmen. |
| Einzelstärke | Der Schneidkopf muss bei bestimmten Glasstärken geändert werden. |
| Gewicht | Je nach Gewicht ist ein zweiter Werker erforderlich, der an nur einem der Schneidtische arbeitet. |
| Modell | Der automatische Zuschnitt ist für Modelle nicht geeignet. |
| Drehbarkeit | Ornamentgläser dürfen nicht gedreht werden. |

Bei den Aggregaten sind die Felder freigeschaltet, in denen die Werte für die aktivierten Prüfungen eingetragen werden.

In dem Beispiel sollen für den Aggregattyp Zuschnitt die Maße und die Dicke des Glases geprüft werden. Dazu müssen die Werte hinterlegt werden, die nicht über- oder unterschritten werden dürfen.

In diesem Beispiel sehen Sie, dass das Aggregat Zuschnitt keine Schnitte unter 100 mm (A) machen kann. Außerdem kann es nur Glasstärken von 4 bis 10 mm (B) schneiden. Im Handzuschnitt könnte die Glasstärke z. B. zwischen 2 und 99 mm angegeben werden, was bedeutet, dass dann Auftragspositionen mit einer Glasstärke von 12 mm von Hand zugeschnitten werden müssen.

> **Aktivierte Restriktionsprüfungen**
> Wenn eine Restriktion geprüft wird, darf das entsprechende Feld nicht leer bleiben. Wenn der Wert nicht geprüft werden soll, tragen Sie in den Feldern Werte ein, die nicht unter- oder überschritten werden können, z. B. 0,1 und 9999.
> ⇨ "Produktionsbereich anlegen" auf Seite H-33

In diesem Beispiel sehen Sie, dass der Zuschnitt von Modellen bei dem Aggregat Zuschnitt nicht möglich ist. Darum wird die Auftragsposition geprüft und nicht an diese Maschine weitergegeben, wenn ein Modell enthalten ist. Für das Aggregat Handzuschnitt wäre der Modellzuschnitt möglich, die Checkbox ist dann markiert.

Beim Aggregat Handzuschnitt ist das Gewicht auf 30 kg eingestellt. Für den normalen Zuschnitt könnte hier z. B. das Gewicht 999 kg eintragen sein, weil die Scheiben automatisch transportiert werden.

#### Zeit und Kosten pro Aggregat

Zu jedem Aggregat (Maschine) hinterlegen Sie Angaben, aus denen die Kosten für die Maschine und die Zeit errechnet werden, die bei der Produktion einer Auftragsposition anfallen.

Aus den Angaben für die Zeit werden die Kapazitäten der einzelnen Maschine und des gesamten Produktionsbereichs berechnet.

Zu jedem Aggregat werden die Kosten hinterlegt, die pro Einheit entstehen. Die Anzahl der Einheiten pro Stunde ergibt sich aus der gemessenen Zeit für die Arbeitsart. Die Kapazität des Aggregats ergibt sich aus:

-   Einheiten pro Stunde
-   Anzahl der Stunden pro Schicht
-   Anzahl der Schichten, in denen das Aggregat arbeitet.

Die Ermittlung der Einheiten pro Aggregat und die Berechnung der Zeit- und Maschinenkosten pro Auftrag sind in separaten Einheiten beschrieben.
-   "Arbeitseinheiten" auf Seite H-45
-   "Produktionskosten" auf Seite H-164

Zur Definition der Daten eines neuen Aggregats gehören weitere Angaben, z. B. technische Restriktionen und Prioritäten, die in den folgenden Abschnitten beschrieben werden. Anschließend finden Sie dann eine ausführliche Handlungsanleitung, nach der Sie die Daten erfassen können.
⇨ "Aggregat anlegen" auf Seite H-35

Wie Sie die Auswahl eines Aggregats bei der automatischen Auslastung steuern können, lernen Sie in einer separaten Einheit.
⇨ "Auswahl der Aggregate" auf Seite H-90

### Arbeitsarten

Arbeitsarten (Vorgänge, Tätigkeiten) bilden die Grundlage für die Produktionsreihenfolge. Den Arbeitsarten werden jeweils die Aggregate zugeordnet, die diese Arbeitsarten ausführen können. Eine Arbeitsart kann von mehreren Maschinen ausgeführt werden. Manche Aggregate können mehrere Arbeitsarten ausführen.

**Beispiel**
Arbeitsart Polieren kann auf mehreren Aggregaten ausgeführt werden:
-   Einseitige Schleifmaschine
-   Zweiseitige Schleifmaschine
-   Schleifmaschine für Serien
-   CNC-Maschine

Ein Produktionsprozess kann mehrere Arbeitsarten umfassen, z. B. bei der VSG-Fertigung eine Arbeitsart VSG-Vorverbund und eine Arbeitsart VSG-Autoklav.

In diesem Beispiel sehen Sie, dass für den Zuschnitt (A) mehrere Arbeitsarten eingerichtet sind: maschineller Zuschnitt, Handzuschnitt und Zuschnitt von VSG-Glas. Diese Unterscheidung ist notwendig, weil für diese Arbeitsarten unterschiedliche Maschinen eingesetzt werden und unterschiedliche Kosten anfallen.
Die Sequenz (B) gibt die Produktionsreihenfolge der einzelnen Arbeitsarten innerhalb der Kapazitätsplanung an. Die ersten Arbeitsarten betreffen in aller Regel den Zuschnitt, die anschließenden Arbeitsarten müssen dann so definiert werden, dass die Reihenfolge stimmt. Da z. B. bei der Fertigung einer ISO-Einheit auch eine ESG-Scheibe verwendet werden könnte, muss die Arbeitsart ESG-Vorspannen immer vor der ISO-Fertigung ausgeführt werden, sie hat also eine höhere Priorität als ISO-Fertigung.

Arbeitsarten, für die bei der Planung eine Maschine nur manuell ausgewählt werden darf, müssen gekennzeichnet werden (C), z. B. da Aggregat Handzuschnitt.

Den Arbeitsarten werden die Maschinen über die Vorgabezeiten zugeordnet. Die Vorgabezeiten werden ausführlich in der Einheit Zeitvorgaben beschrieben.
⇨ "Zeitvorgaben" auf Seite H-59

#### Ausweich-Arbeitsart

Ausweich-Arbeitsarten (D) werden festgelegt, um auf besondere Situationen zu reagieren, z. B. auf das Bohren dicker Scheiben, für die andere Zeiten und andere Aggregate erforderlich sind. Das System erkennt anhand der technischen Vorgaben und der Auftragsposition, wann die Ausweich-Arbeitsart gewählt werden muss und berechnet die Zeit und die Kosten dann entsprechend.

In diesem Beispiel sehen Sie, dass die Ausweich-Arbeitsart gewählt wird, weil die Standard-Maschine die dicke Scheibe nicht bohren kann. Die Bohrmaschine II wird gewählt, weil der Ausweich-Arbeitsart diese Maschine zugewiesen ist.

> **Neue Arbeitsart anlegen**
> Planen Sie Ihre Arbeitsarten so, dass anhand der Nummer eine Gruppierung verwandter Arbeitsarten oder der Arbeitsarten eines Produktionsprozesses zu erkennen ist.
> Neue Arbeitsarten legen Sie in der gleichen Weise an, wie alle Basistabellen. Das Vorgehen ist am Beispiel Produktionsbereich beschrieben.

### Produktionsbereiche (Arbeitszentren)

Ein Betrieb ist in der Regel in verschiedene Produktionsbereiche untergliedert, z. B. Zuschnitt, Schleiferei, Bohren usw. In jedem Produktionsbereich können mehrere Maschinen stehen, die von einer festen Anzahl von Werkern bedient werden. Gleichartige Maschinen können in unterschiedlichen Produktionsbereichen stehen.

Von den Produktionsbereichen werden Statusmeldungen aus der Produktion gesendet, wenn die Position fertig produziert ist. Dazu geben Sie die Erfassungsstelle an, von der die Meldung gesendet wird. In diesem Beispiel werden die Meldungen über die Betriebsdatenerfassung (BDE) gesendet.

Sie sehen, dass auch für den Versand ein Produktionsbereich angelegt ist. Dies ist wichtig, damit auch die Zeiten im Versand mit eingeplant werden und die Aufträge versandfertig gemeldet werden können.

Statusmeldungen können nur von Produktionsbereichen gesendet werden, nicht von Aggregaten. Wenn Sie z. B. bei der ESG-Fertigung zwei Statusmeldungen benötigen, müssen Sie dazu zwei Produktionsbereiche einrichten: ESG-Ofen und Heat-Soak.

### Produktionsbereich anlegen

Wenn Sie die Produktionsbereiche ganz neu einrichten, sollten Sie zunächst planen, welche Maschinen und Arbeitsarten zu ihnen gehören.

> **Voraussetzungen**
> Um die Daten sofort vollständig anlegen zu können, müssen Sie die Werte für die Einheiten pro Stunde, die Übergangszeiten und die Erfassungsstellen für die Rückmeldungen kennen. Sie können die Daten aber auch später nachtragen.

**So legen Sie die Daten für einen Produktionsbereich an**
1.  Wählen Sie im Modul Kapazitätsplanung > Stammdaten > Organisation > Produktionsbereich.
    Der Dialog Produktionsbereiche wird geöffnet.
    Eine Beschreibung des Dialogs finden Sie in der Softwarereferenz.
    ⇨ Softwarereferenz, "Produktionsbereich" auf Seite H-206
2.  Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wechseln.
    Die Nummer des Produktionsbereichs wird automatisch eingesetzt und kann geändert werden.
3.  Tragen Sie den Namen des Produktionsbereichs ein und überschreiben Sie ggf. die Nummer.
    Wenn Sie die Werte für die übrigen Felder bereits kennen, dann tragen Sie diese in die entsprechenden Felder ein.
4.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.

Die Daten werden gespeichert. Sie können jetzt die Aggregate anlegen, die dem neuen Produktionsbereich zugeordnet werden sollen.

### Aggregat anlegen

Sie können alle Daten eines neuen Aggregats einzeln eingeben. Wenn Sie jedoch bereits ein vergleichbares Aggregat in Ihrem Bestand haben, sollten Sie dessen Daten als Basis verwenden. Sie erleichtern sich damit die Arbeit erheblich. In der folgenden Handlungsanleitung wird dieser Weg vorgeführt.

> **Voraussetzungen**
> Um die Daten sofort vollständig anlegen zu können, müssen Sie die Werte für die Kosten und die technischen Restriktionen bereithalten. Welche Werte Sie brauchen, können Sie der Softwarereferenz entnehmen. Sie können die fehlenden Daten aber auch später nachtragen.
> ⇨ Softwarereferenz, "Aggregate" auf Seite H-207

**So legen Sie die Daten für eine neue Maschine an**
1.  Wählen Sie im Modul Kapazitätsplanung > Stammdaten > Organisation > Aggregate.
2.  Wählen Sie den Produktionsbereich aus, dem die neue Maschine zugeordnet werden soll, z. B. Bearbeitungen.
3.  Wählen Sie im Menü Start > Suchen, um die Daten der Maschinen aus diesem Produktionsbereich einzulesen.
    In der Übersicht (C) werden alle Aggregate aufgeführt, die diesem Produktionsbereich zugeordnet sind.
    Die Felder der Werte (A) sind mit den Daten des markierten Aggregats vorbelegt.
4.  Markieren Sie in der Übersicht das Aggregat, dessen Werte Sie übernehmen wollen.
5.  Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wechseln.
    Das Feld für die Aggregatnummer (B) wird freigeschaltet.
6.  Überschreiben Sie die Nummer und den Namen des Aggregats.
7.  Wählen ggf. einen anderen Produktionsbereich aus.
8.  Passen in den Feldern für die Kosten (A) die Werte an.
9.  Tragen Sie im Feld Erfassungsstelle (D) die ID der Erfassungsstelle ein, von der die Fertigmeldung kommt.
10. Wählen Sie im Menü Start > Speichern, um die neuen Daten zu speichern.
    Damit haben Sie die neue Maschine angelegt. Die Maschine wird in der Übersicht aufgeführt. Sie können jetzt die Prüfungen (A) aktivieren und die Angaben für die technischen Restriktionen anpassen.

> **Neues Aggregat sperren**
> Wenn Sie ein neues Aggregat angelegt haben, auf das noch nicht eingelastet werden soll, dann müssen Sie es unbedingt sperren (B).

#### So passen Sie die technischen Restriktionen an

1.  Wechseln Sie zum Register Restriktionen.
2.  Prüfen Sie im Bereich Technische Restriktionen (B), welche Werte für die Maschine gelten.
    > **Neue Restriktionsprüfung aktiviert**
    > Wenn eine benötigte Prüfung gesperrt ist, haben Sie unter Umständen im Register Aggregat den falschen Aggregattyp zugewiesen. Wenn der Aggregattyp richtig eingestellt ist, sollten Sie im Dialog Aggregattypen prüfen, ob die Checkboxen für die Prüfungen korrekt markiert sind.
    > Wenn Sie im Aggregattyp eine Restriktionsprüfung aktivieren, müssen Sie in allen Aggregaten die entsprechenden Felder füllen. Tragen Sie mindestens null (0) ein, damit das Feld nicht leer bleibt.
3.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Daten werden gespeichert. Die Angaben zu den zugewiesenen Arbeitsarten (A) werden erst angezeigt, wenn Sie diese in den Dialogen zur Zuordnung festgelegt haben.

### Übungen

-   Überlegen Sie, wie die Produktion räumlich organisiert ist und wie Sie diese Organisation in den Stammdaten mit Produktionsbereichen und Maschinen abbilden können.
-   Legen Sie einen Produktionsbereich ISO-2 und die zugehörigen Maschinen an.
    Die Übungen bauen aufeinander auf. Sie sollten sich daher mehrere unterschiedliche Maschinen anlegen, um in den Übungen der nächsten Einheiten Vergleichsmöglichkeiten zu haben.
-   Legen Sie eine Arbeitsart für 3-fach-ISO an.

> **Übungen im realen Betrieb**
> Wenn Ihre Kapazitätsplanung bereits im Tagesgeschäft eingesetzt wird, dann müssen Sie neue Maschinen unbedingt sperren, damit diese nicht in der Planung berücksichtigt werden.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Aggregattypen" auf Seite H-195
⇨ Softwarereferenz, "Arbeitsarten" auf Seite H-198
⇨ Softwarereferenz, "Zugeordnete Aggregate" auf Seite H-201
⇨ Softwarereferenz, "Produktionsbereich" auf Seite H-206
⇨ Softwarereferenz, "Aggregate" auf Seite H-207

## Schicht- und Arbeitszeiten

**Lernziele**
-   Schichtzeiten und Kalender einrichten.
-   Arbeitseinheiten kennenlernen.
-   Kapazitäten pro Produktionsbereich und pro Aggregat berechnen.

**Nutzen**
-   Mit den hinterlegten Schichten und den Angaben zu Arbeitseinheiten wird die Kapazität eines jeden Produktionsbereichs errechnet. Anhand dieser Kapazität wird die Terminierung der eingelasteten Aufträge durchgeführt.

**Merke**
-   **Schicht**: Die Schichten in den verschiedenen Produktionsbereichen können unterschiedlich lang sein. Der Schichtbeginn muss für alle Produktionsbereiche zur selben Uhrzeit festgelegt werden, damit keine Überschneidungen beim Schichtwechsel und Übergang von einem zum nächsten Produktionsbereich entstehen.
-   **Arbeitseinheit**: Mit Arbeitseinheiten geben Sie an, wie viel pro Stunde gefertigt werden kann. Arbeitseinheiten können als Mannstunden oder als Maschinenstunden angegeben werden.
-   **Kapazität**: Die Kapazität einer Maschine ist das Produkt aus Arbeitseinheiten und Schichtstunden. Die Kapazität eines Produktionsbereichs ist die Summe aller Maschinenkapazitäten im Produktionsbereich.
-   **Geschlossene Kapazität**: Bei geschlossenen Kapazitäten wird automatisch nach einem anderen Termin gesucht, wenn die verfügbaren Schichten und Maschinen ausgelastet sind.
-   **Offene Kapazität**: Bei offenen Kapazitäten wird die Schichtzeit nicht geprüft.
-   **Voreinstellungen**: Firmendaten: Register Kapa-Planung > Anzahl der Schichten

### Arbeitszeiten

Für die Berechnung von Terminen werden Vorgaben herangezogen, die Sie in unterschiedlichen Dialogen hinterlegen. Dies sind z. B. Werte für:

-   Zeit, die eine Maschine eingesetzt werden kann (Schichtzeit).
-   Zeit, die benötigt wird, um ein Stück zu fertigen (Vorgabezeit).
-   Zeit, die mehr aufgewendet wird, wenn der Arbeitsgang aufwendiger ist (Zeitzuschlag).
-   Rüstzeit.

Im Folgenden werden die Zusammenhänge der unterschiedlichen Zeitvorgaben und der Voreinstellungen für die Arbeitszeiten näher erklärt.

### Arbeitstage und Schichten

Für die Terminberechnung in der Kapazitätsplanung ist es wichtig, ob Ihr Betrieb in Schichten arbeitet oder nicht.

-   Wenn nicht in Schichten gearbeitet wird, greift die Kapazitätsplanung auf den A+W Business Pro-Standard-Kalender zu.
-   Wenn in Schichten gearbeitet wird, können die Schichtzeiten pro Produktionsbereich hinterlegt werden.

Wenn nicht alle Produktionsbereiche in allen Schichten arbeiten, richtet sich die Anzahl der Schichten nach dem Produktionsbereich mit den meisten Schichten. Die Anzahl der Schichten legen Sie im Modul Stammdaten > Firma > Firmendaten fest.

Die Länge einer Schicht wird im Kalender pro Aggregat oder Produktionsbereich festgelegt. Wenn z. B. mehrere Produktionsbereiche in drei Schichten mit unterschiedlichen Schichtlängen arbeiten, dann müssen Sie die Schichten so einteilen, dass die Schichten 2 und 3 in allen Produktionsbereichen zur gleichen Uhrzeit beginnen.

Die Schichten der verschiedenen Produktionsbereiche dürfen sich zeitlich nicht überlagern, weil sonst der Übergang von einer Schicht in die nächste beim Wechsel des Produktionsbereichs nicht eindeutig ist.

**Beispiel**

| Produktions-Bereich | Beginn 1. Schicht | Anzahl Std. | Beginn 2. Schicht | Anzahl Std. | Beginn 3. Schicht | Anzahl Std. | Ende |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Zuschnitt | 06:00 | 6 | 12:00 | 4 | 16:00 | 4 | 20:00 |
| VSG | 08:00 | 4 | 12:00 | 4 | 16:00 | 4 | 20:00 |
| Bohren | 10:00 | 2 | 12:00 | 4 | 16:00 | 2 | 18:00 |
| Heat-Soak-Test | 08:00 | 12 | | 0 | | 0 | 20:00 |

Bei einer solchen Schichtorganisation ist gewährleistet, dass sich keine Arbeitsverzögerungen von einer Schicht zur anderen ergeben, da die Schichtwechsel in den Produktionsbereichen zur selben Zeit stattfinden.

Die Zeiten des Schichtwechsels legen Sie im Modul Kapazitätsplanung > Stammdaten > Organisation > Kalender > Menü Funktionen > Schichtzeiten fest.

In diesem Beispiel sehen Sie, dass die Schicht 2 um 12:00 Uhr beginnt und um 16:00 Uhr endet. Darauf folgt, dass Schicht 1 bei einer Schichtzeit von 6 Std. um 6:00 Uhr beginnt. Der Übergang von Schicht 2 zu Schicht 3 ist um 16:00 Uhr, was bedeutet, dass die Schicht 2 nur 4 Stunden lang ist.

### Maximale Kapazität pro Tag

Die Kapazität einer Maschine pro Tag wird in Arbeitseinheiten gerechnet. Die Kapazität für den jeweiligen Produktionsbereich setzt sich aus den Einheiten pro Stunde aller Maschinen zusammen, die zum Produktionsbereich gehören.

Die maximale Kapazität einer Maschine ergibt sich aus den im Kalender eingetragenen Summen der Stunden pro Tag, multipliziert mit den Arbeitseinheiten pro Stunde, die für die Maschine im Dialog Aggregat hinterlegt sind.

**Beispiel**
Tag: Dienstag, Produktionsbereich Zuschnitt, Maschine Schneidtisch.
Am Schneidtisch können 4 Arbeitseinheiten pro Stunde gemacht werden.

| Schicht | Stunden | x 4 Arbeitseinh./Std | = Max. Arbeitseinh./Schicht |
| :--- | :--- | :--- | :--- |
| 1. Schicht | 6 Std. | x 4 A.Einh./Std. | = 24 A.Einh./Schicht |
| 2. Schicht | 4 Std. | x 4 A.Einh./Std. | = 16 A.Einh./Schicht |
| 3. Schicht | 4 Std. | x 4 A.Einh./Std. | = 16 A.Einh./Schicht |
| **Max. Kapazität pro Tag am Schneidtisch** | | | **= 56 A.Einh./Tag** |

⇨ "Arbeitseinheiten" auf Seite H-45
⇨ "Kalender anpassen" auf Seite H-52

Die Kapazität eines Produktionsbereichs ergibt sich aus der Summe der Tageskapazitäten aller Maschinen in diesem Produktionsbereich.

Sie müssen dabei jedoch berücksichtigen, ob alle Aggregate jederzeit einsetzbar sind. Wenn Sie z. B. 6 Schleifmaschinen haben, aber nur drei Werker, die an diesen Maschinen arbeiten können, können Sie die Gesamtkapazität nur für drei Maschinen berechnen. Die Prüfung der freien Kapazitäten bezieht sich daher nicht nur auf die Maschinen selbst, sondern auch auf die maximale Anzahl von Einheiten, die in einem Produktionsbereich gefertigt werden können.

Wie Sie die Arbeitseinheiten bestimmen, lernen Sie in der folgenden Einheit.

### Arbeitseinheiten

Arbeitseinheiten kann sowohl für jedes einzelne Aggregat als auch für den gesamten Produktionsbereich angegeben werden. Für beide Angaben legen Sie dieselbe Berechnungsart der Arbeitseinheit zugrunde.
Bevor Sie die Werte hinterlegen, müssen Sie festlegen, welche Arbeitseinheit verwendet wird. Es gibt viele Möglichkeiten, z. B.:

-   Arbeitseinheit = Mannstunde
-   Arbeitseinheit = Maschinenstunde

Folgende Fragen müssen Sie beantworten, um die Arbeitseinheiten pro Stunde und die Vorgabezeiten einrichten zu können:

-   In welcher Arbeitseinheit soll die Kapazitätsberechnung der Maschine erfolgen?
-   Was ist unter Mannstunde, Maschinenstunde usw. zu verstehen?
    ⇨ "Arbeitseinheit = Mannstunde" auf Seite H-46
    ⇨ "Arbeitseinheit = Maschinenstunde " auf Seite H-49
-   Welcher Wert muss für die Einheit/Std. eingetragen werden?
    ⇨ Softwarereferenz, "Aggregate" auf Seite H-207
-   Wie viel Zeit braucht die Maschine für eine Einheit (lfm, qm, Stück) bezogen auf die Arbeitseinheit?
    ⇨ "Ermittlung der Mannstunden" auf Seite H-47

#### Arbeitseinheit = Mannstunde

Anhand der Arbeitseinheiten wird beim Einlasten geprüft, ob noch Kapazitäten für diesen Tag zur Verfügung stehen.

**Beispiel**
Im Produktionsbereich Bohren (5 Maschinen) arbeiten 12 Personen in insgesamt drei Schichten pro Tag. Pro Schicht arbeiten also vier Personen. Diese vier Personen entsprechen vier Arbeitseinheiten im Produktionsbereich Bohren.

Auch wenn nur vier Personen im Produktionsbereich für fünf Maschinen zur Verfügung stehen, kann theoretisch jede Maschine die ganze Schichtzeit, z. B. acht Stunden, laufen. Das heißt, Sie tragen bei jeder Maschine die Arbeitseinheit gleich 1 ein. Welche vier der fünf Maschinen jedoch letztlich eingesetzt werden, hängt von den Einlastungsdaten ab.

Folgendes wird geprüft:
-   Ist die Maschine ausgelastet?
-   Wenn ja, stehen noch andere Maschinen zur Verfügung? Das heißt: Ist die maximale Kapazität des Produktionsbereiches von vier Arbeitseinheiten bereits erreicht?
    -   Wenn ja, kann auf eine freie Maschine eingelastet werden.
    -   Wenn nein, muss der Arbeitsgang auf den nächsten Tag oder die nächste Schicht verschoben werden oder es wird entschieden, dass Überstunden gemacht werden müssen.

> **Anwesende Werker**
> Die Kapazitätsplanung geht davon aus, dass immer alle Personen (Werker) da sind.

#### Ermittlung der Mannstunden

Um die Mannstunden zu ermitteln, müssen die Zeitwerte mit der Anzahl der Personen, die an der Maschine arbeiten, multipliziert werden. Je nachdem, ob Sie Einzelzeiten oder eine Staffelung, z. B. nach Dicke, definieren, wird die Vorgabezeit anders berechnet.
Die folgenden Beispiele sind reine Berechnungsbeispiele.

**Beispiel: 3 Personen, Einzelzeit**
Berechnung von Mannstunden am Schneidtisch:
-   3 Personen arbeiten am Schneidtisch.
-   In einer Stunde können 200 qm zugeschnitten werden.
-   Die Vorgabezeit wird als Einzelzeit hinterlegt.

**Formel:**
Vorgabezeit 1 qm = (1 Std / Anzahl qm pro Stunde) x Anzahl Personen [Mannstunden]

**Rechenbeispiel:**
Vorgabezeit 1 qm = (1 Std / 200 qm) x 3 Personen = 0,015 [Mannstunden]

**Beispiel: gestaffelte Zeit (Vektor)**
Berechnung von Mannstunden am Schneidtisch, gestaffelt nach Dicke:
-   3 Personen arbeiten am Schneidtisch.
-   Gestoppte Zeit pro gefertigte Einheit, nach Dicke des Glases gestaffelt.
-   Die Vorgabezeiten werden im Vektor-Format hinterlegt.

**Formel:**
Vorgabezeit 1 qm = gestoppte Zeit x Anzahl Personen [Mannstunden]

**Rechenbeispiel:**
Vorgabezeit 1 qm Float 4 mm = 0,009 Std. x 3 Personen = 0,027 Mannstunden
Vorgabezeit 1 qm Float 6 mm = 0,010 Std. x 3 Personen = 0,03 Mannstunden

**Beispiel: 2 Personen, Einzelzeit**
Berechnung von Mannstunden an der Schleifmaschine:
-   2 Personen arbeiten an der Schleifmaschine.
-   In einer Stunde können 3 Laufmeter geschliffen werden.
-   Die Vorgabezeit wird als Einzelzeit hinterlegt.

**Formel:**
Vorgabezeit = (1 Std / Anzahl lfm pro Stunde) x Anzahl Personen [Mannstunden]

**Rechenbeispiel:**
Vorgabezeit = (1 Std / 3 lfm) x 2 Personen = 0,66 [Mannstunden]

#### Arbeitseinheit = Maschinenstunde

Wenn die Zeiten unabhängig von der Anzahl der Werker an der Maschine sind, können Sie die Arbeitseinheit Maschinenstunden einsetzen.
In diesem Fall muss als Arbeitseinheit für das Aggregat immer eine 1 eingetragen werden.

Standardmäßig wird der Wert 1 für die Anzahl der Einheiten eingegeben. Damit können Sie besser nachvollziehen, wie die Kapazitäten berechnet werden.

**Arbeitseinheiten pro Produktionsbereich**
Im Normalfall entspricht die Anzahl der Arbeitseinheiten je Produktionsbereich der Anzahl der Maschinen, die dort eingesetzt werden. Wenn 3 Maschinen eingesetzt werden, dann ist die Anzahl der Arbeitseinheiten gleich 3.

Die Bedingungen in einem Betrieb könnten jedoch folgendermaßen eingeschränkt sein:

-   Sie setzen in Ihrem Produktionsbereich z. B. 3 Maschinen ein.
-   Die Stromversorgung lässt aber nur den gleichzeitigen Betrieb von 2 Maschinen zu. Das heißt, dass eine Maschine immer abgeschaltet sein muss.

In diesem Fall müssen Sie als Arbeitseinheit pro Stunde für den gesamten Produktionsbereich den Wert 2 eintragen.

### Voreinstellungen für Schichten und Kapazitäten

Im Modul Stammdaten legen Sie die Grundeinstellungen für die Kapazitätsplanung in A+W Business Pro fest.

Die Anzahl der Schichten (A) richtet sich nach dem Produktionsbereich, in dem die meisten Schichten gefahren werden. Die Schichten werden u. a. bei der Berechnung von Übergangsmatrix und Übergangszeiten berücksichtigt.

Sie müssen festlegen, ob Sie mit geschlossenen oder offenen Kapazitäten arbeiten wollen.

-   Bei geschlossenen Kapazitäten wird automatisch nach einem anderen Termin gesucht, wenn die verfügbaren Schichten und Maschinen ausgelastet sind.
-   Bei offenen Kapazitäten wird die Schichtzeit nicht geprüft.

Außerdem müssen Sie festlegen, wie stark eine Schicht ausgelastet werden darf, wenn die Aufträge automatisch an die Kapazitätsplanung übergeben werden. Wenn Sie die Schichten immer voll oder nahezu voll auslasten, haben Sie keinen Spielraum mehr für Umlastungen, für Eilaufträge oder für Restmengen vom Vortag.

Folgende Einstellungen im Feld **Fertigungsterminmodus (B)** stehen für den Auslastungsgrad zur Verfügung.

-   **Automatisch Normalkapazität:** Die Aufträge werden entsprechend der zur Verfügung stehenden Schichtzeiten eingelastet. Die Überbuchung ist nicht möglich. Dies ist die Standard-Einstellung.
-   **Automatisch volle Tage:** Bei dieser Einstellung werden die Angaben im Kalender für die Anzahl Schichten und Stunden ignoriert. Die Einlastung geht dann von einem Arbeitstag mit 24 Stunden aus. Dies gilt jedoch nur für reguläre Arbeitstage, nicht für Feiertage.
-   **Nur Aggregatwechsel:** Bei ausgelasteten Kapazitäten soll automatisch nur nach einem anderen Aggregat gesucht werden. Wenn das ebenfalls ausgelastet wird, wird die Einlastung unterbrochen und Sie müssen manuell eingreifen.
-   **Einlasten ohne Kontrolle:** Diese Einstellung entspricht der offenen Schicht. Das heißt z. B., dass trotz der Schichtzeit von 8 Std. auch 16 Std. eingelastet werden können. Dabei wird keine Meldung ausgegeben, wenn ein Tag voll ausgelastet ist.

Große Positionen können auf mehrere Aggregate, Schichten oder Tage verteilt werden. Dazu geben Sie im Feld **Schichtfüllung bei Positionssplit (C)** an, zu wie viel Prozent die Schicht eines Aggregats durch das Splitting gefüllt werden darf, um Platz für andere Aufträge zu behalten.

> **Einstellungen ändern**
> Wenn Sie Einstellungen in den Firmendaten geändert haben, sollten Sie A+W Business Pro neu starten.
> Die weiteren Einstellungen für Arbeitstage und Schichten werden Sie in den zugehörigen Lerneinheiten kennenlernen.

### Kalender anpassen

Standardmäßig geht die Kapazitätsplanung von einer Schicht pro Tag aus. Wenn Sie jedoch in Ihrem Betrieb mit mehr als einer Schicht arbeiten wollen, dann müssen Sie als ersten Schritt die Anzahl der Schichten in den Firmendaten festlegen.
Danach können Sie pro Arbeitsart und Aggregat oder pro Produktionsbereich einen eigenen Kalender mit den jeweiligen Schichten bzw. Schichtzeiten anlegen. Wenn Sie für einen Produktionsbereich oder ein Aggregat keinen eigenen Kalender anlegen, gilt der allgemeine Kalender.

> **Jahreswechsel**
> Wenn Sie die Kapazitäten über den Jahreswechsel hinaus planen wollen, müssen Sie den Kalender für das neue Jahr mit allen Schichtzeiten angelegt haben.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:

-   "So legen Sie die Anzahl der Schichten fest" auf Seite H-52
-   "So legen Sie einen neuen Kalender an" auf Seite H-53
-   "So richten Sie weitere Schichtzeiten ein" auf Seite H-56
-   "So richten Sie eine Sonderschicht ein" auf Seite H-57

> **Kalender ändern**
> Wenn Sie einen Kalender bearbeitet oder angelegt haben, müssen Sie A+W Business Pro neu starten, damit die Daten beim Einlasten zur Verfügung stehen.

**So legen Sie die Anzahl der Schichten fest**
1.  Wählen Sie im Modul Stammdaten > Firma > Firmendaten.
2.  Wechseln Sie zum Register Kapa-Planung.
3.  Tragen Sie im Bereich A+W Business Kapazitätsplanung die Anzahl der Schichten ein.
4.  Wählen Sie im Menü Start > Speichern, um die Änderungen zu speichern.
    Die Daten werden gespeichert. Im Kalender der Kapazitätsplanung werden die Felder für die Schichtzeiten freigeschaltet.
