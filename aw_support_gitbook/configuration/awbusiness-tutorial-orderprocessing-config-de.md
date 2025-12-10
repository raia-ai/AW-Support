---
title: "D-AWBusiness-HB_14"
source: "D-AWBusiness-HB_14.pdf"
tags: ["A+W Business Verkauf", "Tutorial", "Order Processing", "Invoicing", "Mullion Configuration", "Product Models", "Macros", "Price Management", "ERP Software", "Document Management"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a comprehensive tutorial for the A+W Business sales module, guiding users through the complete process of document creation from order entry to invoicing. It covers creating positions, managing special items like crates, and using advanced features for efficiency."
long_description: "This tutorial provides detailed, step-by-step instructions for using the A+W Business sales software, focusing on the complete workflow from document creation to invoicing. The guide begins with basic position entry, including how to handle special cases like crates. It then introduces efficiency features such as quick entry (Schnellerfassung) and quick inquiries (Schnellanfrage), allowing users to rapidly enter data and respond to customer queries. A significant portion of the manual is dedicated to complex product configurations. This includes checking product availability, configuring standard and irregular mullion constructions (Sprossen), and defining custom product models and processing steps (Bearbeitungen). The document also explains how to create and use motifs (Motive) with or without screen numbers for surface treatments. To streamline repetitive tasks, the tutorial covers creating, saving, and applying macros for frequently used product assemblies and prices. The pricing section details how to view, manually change, and fix prices, manage surcharges, and use the price recorder. It also covers document organization through 'Nummernverwalter' (number administrators) and the final step of printing various documents like order confirmations, delivery notes, and invoices. The manual is rich with screenshots, labeled diagrams, and practical exercises to reinforce learning."
---

# Tutorial: Kompletterfassung von Dokumenten bis Faktura

Im folgenden Beispiel wurde eine Kiste ohne ID übernommen. Der Dialog wird geschlossen und die Positionserfassung wird wieder angezeigt.

*   **Abb. C-38: Position mit Kiste erfasst**
    *   In der Erfassungszeile werden für Kisten alle Felder ab Menge gesperrt. Im Bereich Produkt wird eine Stückliste angezeigt und die Preisfelder werden aktualisiert.
    *   Im Register Stückliste werden Details zum Inhalt der Kiste angezeigt, z. B. Stückzahl, Gesamtfläche, Preis/Preiseinheit, Gesamtpreis.

6.  Korrigieren Sie ggf. die Stückzahl, wenn Sie mehr als eine Kiste erfassen wollen.
7.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern. Die Daten werden gespeichert.

---
### So erfassen Sie eine Position über die Schnellerfassung

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet. Die Felder der Erfassungszeile sind freigeschaltet.
2.  Ziehen Sie die Spalte Produkt ggf. breiter auf.
3.  Tragen Sie die gesamten Positionsdaten den Regeln entsprechend ein.
    ⇨ "Schnellerfassung" auf Seite C-95

    *   **Abb. C-39: Eingabe als Schnellerfassung**

4.  Bestätigen Sie die Position mit <Enter>.
    Die Positionsdaten werden gespeichert und die Felder werden aktualisiert.

    *   **Abb. C-40: Resultat als Schnellerfassung**

Sie können die Daten weiterbearbeiten.

## Schnellanfrage beantworten

Bevor Sie die Schnellanfrage starten, müssen Sie das Dokument speichern, in dem Sie aktuell arbeiten. Ohne Speichern könnten die zuletzt erfassten Daten verloren gehen, sobald Sie die Schnellanfrage öffnen.

### So beantworten Sie eine Schnellanfrage

1.  Um eine Schnellanfrage zu beantworten, haben Sie zwei Möglichkeiten:
    *   Wählen Sie Dokumente > Auftrag > Schnellanfrage.
    *   Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Positionen. Wenn Sie die Positionserfassung bereits geöffnet haben, können Sie die Schnellanfrage im Menü Funktionen > Gruppe Position > Schnellanfrage starten. Vergessen Sie nicht, vorher die letzten Eingaben zu speichern.

    Der Dialog Schnellanfrage wird geöffnet.
    ⇨ Softwarereferenz, "Schnellanfrage" auf Seite C-601

2.  Wählen Sie den Kunden aus.

    *   **Abb. C-41: Schnellanfrage für Kunden starten**
    Die aktuellen Daten zum Kreditlimit des gewählten Kunden werden angezeigt.

3.  Bestätigen Sie die Daten mit [OK].
    Der Dialog Schnellanfrage wird geschlossen. Die Positionserfassung wird im Modus Schnellanfrage angezeigt.

4.  Geben Sie die Daten für das angefragte Produkt als Position ein.
    Sie können jede Position speichern und anschließend eine weitere Position erfassen. Die Preise werden für jede Position sofort aktualisiert.
    Wenn Sie alle angefragten Positionen erfasst haben, können Sie die Schnellanfrage beenden. Sie haben dabei die Möglichkeit, die erfassten Daten zu speichern.

    *   **Abb. C-42: Schnellanfrage – Produktnummer eingeben**

5.  Schließen Sie die Schnellanfrage.
    Die Abfrage zum Speichern der Daten wird angezeigt:
    *   Wählen Sie [Nein], wenn Sie die Daten nicht speichern möchten. Die Schnellanfrage wird geschlossen. Die Positionserfassung des Dokuments wird wieder angezeigt, das Sie zuletzt bearbeitet haben.
    *   Wählen Sie [Ja], wenn Sie die Daten speichern möchten. Der Dialog Schnellanfrage speichern wird angezeigt.

6.  Wählen Sie im Dialog Schnellanfrage speichern aus, ob Sie die Daten als Angebot oder als Auftrag speichern möchten.
7.  Wählen Sie den zugehörigen AV-Bereich und Nummernverwalter aus.
8.  Klicken Sie auf [OK], um die Daten zu speichern.
    Die Schnellanfrage wird geschlossen. Die Positionserfassung des Dokuments wird wieder angezeigt, das Sie zuletzt bearbeitet haben.

## Verfügbarkeit eines Produkts prüfen

Wenn Sie im Menü Optionen die Meldung für Bestandsunterschreitungen aktiviert haben, wird beim Speichern des Auftrags eine Meldung angezeigt, wenn Sie ein entsprechendes Produkt erfasst haben. Sie können dann von der Positionserfassung aus den Bestand und den zukünftigen Lagerbestand prüfen und die Liefertermine des aktuellen Auftrags anpassen.

### So prüfen Sie die Verfügbarkeit eines Produkts

1.  Markieren Sie die Position, zu der Sie Informationen abrufen wollen.
2.  Klicken Sie auf die Schaltfläche [Info].
    Der Dialog wird geöffnet. Im folgenden Beispiel wird der Liefertermin durch die Bestandsunterschreitung bei einer Stücklisten-Komponente gefährdet.

    *   **Abb. C-43: Bestandsunterschreitung bei einer Stücklisten-Komponente**
    In der Stückliste ist eine der Komponenten in roter Schrift dargestellt. Diese Komponente gefährdet den Liefertermin Ihres Auftrags.

3.  Klicken Sie auf [Ende], um den Dialog zu schließen.
    Der Dialog Artikel-Info wird geschlossen.

4.  Wählen Sie im Menü Start > Lagersuche, um in den Such-Modus zu wechseln.
    Wenn die Komponenten nicht als Lagerartikel geführt werden, müssen Sie die Produktnummer der kritischen Komponente eintragen und suchen. In diesem Beispiel werden die Komponenten als Lagerartikel geführt.

    *   **Abb. C-44: Lagerinfo**
        *   **A**: Aktueller Bestand liegt unter dem geforderten Mindestbestand
        *   **B**: Reservierte Menge
        *   **C**: Bestellte Menge

    Der Mindestbestand für die Komponente ist unterschritten. Die Reservierungen liegen weit über den aktuell offenen Bestellungen. Sie können daraus schließen, dass der Produktionstermin verschoben werden muss.

5.  Wechseln Sie zum Register Zukünftiger Lagerbestand, um zu prüfen, wie Sie die Termine im Auftrag einstellen können.

    *   **Abb. C-45: Zukünftiger Lagerbestand**
        *   **A**: Nachgefragtes Produkt: aktueller Bestand
        *   **B**: Bestand und Reservierungen der nächsten 14 Tage
        *   **C**: Endbestand für den angezeigten Zeitraum (nur Lagerartikel im selben Lagerführungsmodus)

    In der Anzeige des zukünftigen Lagerbestands ist der Zeitraum bis 14 Tage in die Zukunft berücksichtigt. Sie können daraus ersehen, wann der Lagerbestand die Fertigung des erfassten Auftrags zulässt.

6.  Klicken Sie auf [Ende], um den Dialog zu schließen.
    Die Positionserfassung wird wieder angezeigt. Sie können jetzt das Produkt oder die Termine im Auftragskopf ändern.

## Sprossen erfassen

Zu jedem Isolierglas können in allen Scheibenzwischenräumen Sprossenkonstruktionen erfasst werden. Sie gelten immer für die gesamte Position.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So erfassen Sie eine normale Sprossenkonstruktion" auf Seite C-109
*   "So erfassen Sie eine unregelmäßige Sprossenkonstruktion" auf Seite C-112

### So erfassen Sie eine normale Sprossenkonstruktion

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
2.  Erfassen Sie eine neue Position oder markieren Sie im Bereich Positionen die Position, zu der Sie Sprossen erfassen möchten.
3.  Wechseln Sie zum Register Sprossen.

    *   **Abb. C-46: Felder für Sprossen freigeschaltet**
        *   **A**: Auswahl des Sprossenmusters
        *   **B**: Bei Mehrfach-ISO: Auswahl des Abstandhalters
        *   **C**: Auswahl der Sprossen
        *   **D**: Berechnungsart

4.  Wählen Sie das Sprossenmuster über die entsprechende Symbolschaltfläche (A) aus.
    ⇨ Softwarereferenz, "Positionen - Sprossen" auf Seite C-504
5.  Wählen Sie die Sprossen (C) aus und tragen Sie die Anzahl ein.
    Wenn Sie ein Mehrfach-ISO erfasst haben, müssen Sie den Abstandhalter (B) auswählen, an den die Sprossen angehängt werden.
    Die Grafik und die Felder werden aktualisiert. Sie können für die waagerechten und senkrechten Sprossen unterschiedliche Produkte und/oder Varianten auswählen.
    Mit der Schaltfläche können Sie die Sprossen in den zweiten Abstandhalter übernehmen.
    Sie können die Sprossengitter in den Zwischenräumen jedoch auch unterschiedlich gestalten, z. B. die waagerechten Sprossen im ersten Zwischenraum und die senkrechten im zweiten.

    *   **Abb. C-47: Sprossenkonstruktion mit unterschiedlichen Sprossen**
        *   **A**: Bohrmaße
        *   **B**: Bezugspunkt für die Maße
        *   **C**: Kennzeichen für Noppen
        *   **D**: Berechnungsart
        *   **E**: Rückschnitt

6.  Bestimmen Sie die Berechnungsart (D) und geben Sie ggf. die Bohrmaße (A) ein.
    Die Felder für die Bohrmaße sind nur bei den asymmetrischen Berechnungsarten freigeschaltet.
    ⇨ "Sprossenkonstruktion" auf Seite C-73
7.  Prüfen Sie die Größe des Rückschnitts (E) und legen Sie fest, ob Noppen (C) eingebaut werden sollen oder nicht.
    Wenn der Rückschnitt nicht an allen Kanten gleich groß sein soll, müssen Sie den Dialog Rückschnitt öffnen, indem Sie auf die Schaltfläche (E) klicken. Tragen Sie dann pro Kante ein, wie groß der Rückschnitt sein soll.
8.  Prüfen Sie die Verkaufspreise und die Druckeinstellung.
9.  Wählen Sie im Menü Start > Speichern, um die Daten zu übernehmen.
    Die Ansicht wechselt zum Register Position. In der Stückliste ist für die waagerechten und die senkrechten Sprossen jeweils eine Komponente eingefügt.
10. Wählen Sie im Menü Start > Speichern, um die Position zu speichern.
    Die Daten werden gespeichert und die Preisfelder werden aktualisiert.

### So erfassen Sie eine unregelmäßige Sprossenkonstruktion

1.  Erfassen Sie die Sprossen, wie in den Schritten 1 bis 6 der Anleitung oben beschrieben.
    Achten Sie darauf, dass die Anzahl der Sprossen ein asymmetrisches Muster zulässt.

    *   **Abb. C-48: Grundmuster des Sprossengitters**
        *   **A**: Auswahl der waagerechten Sprossen
        *   **B**: Auswahl der senkrechten Sprossen
        *   **C**: Auswahl der diagonalen Sprossen
        *   **D**: Register Wegfallsprossen

2.  Wenn Sie V-Sprossen einbauen möchten, wechseln Sie zum Register Wegfallsprossen (D).
    Besondere Sprossenkonstruktionen, z. B. als Sonne oder Mond, sind ebenfalls möglich. Diese lernen Sie in einer separaten Schulung zu A+W CAD Designer kennen.
3.  Deaktivieren Sie die Checkboxen aller Sprossenabschnitte, die Sie nicht benötigen, z. B. die senkrechten Sprossen im oberen Drittel (B).
4.  Aktivieren Sie die Checkboxen für die Diagonalsprossen (C).

    *   **Abb. C-49: Unregelmäßige Sprossenkonstruktion**

5.  Wechseln Sie zum Register Preise, um die Verkaufspreise zu prüfen.
6.  Wählen Sie im Menü Start > Speichern, um die Sprossendaten zu übernehmen.
    Die Anzeige wechselt zum Register Position. In der Stückliste werden die Sprossen und die zugehörigen Preise angezeigt.
7.  Wählen Sie im Menü Start > Speichern, um die Position zu speichern.
    Die Daten werden gespeichert und die Preisfelder werden aktualisiert.

> **Häufig benötigte Produktaufbauten als Makro speichern**
> Wenn Sie einen Produktaufbau erfasst haben, den Sie für diesen Kunden oder ganz allgemein häufiger benötigen, können Sie diesen als Makro speichern und bei der nächsten Auftragserfassung abrufen.
> ⇨ "Makro speichern" auf Seite C-166

## Modell erfassen

Zu jeder Position kann ein Modell erfasst werden. Es gilt immer für die gesamte Position. Das erfasste Modell kann auf der Auftragsbestätigung gedruckt werden. Dazu müssen die Druckparameter festgelegt werden.
⇨ "Druck von Skizzen" auf Seite C-202

> **Modell ändern**
> Wenn Sie während der Erfassung das Modell wechseln, werden die Modellparameter beibehalten. Dies gilt nur für gespiegelte Modelle. Wenn die Parameter sich ändern, müssen Sie jedoch die Werte neu eingeben.
>
> **Bearbeitungen erfassen**
> Sie sollten zuerst das Modell mit allen Kanten und Längen erfassen. Erst danach werden alle vorhandenen Kanten angezeigt und können zur Bearbeitung ausgewählt werden.
> ⇨ "Bearbeitung erfassen" auf Seite C-119

### So erfassen Sie ein Modell

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
2.  Erfassen Sie eine neue Position oder markieren Sie im Bereich Positionen die Position, zu der Sie das Modell erfassen wollen.
    Als Maße müssen Sie die Größe des umschriebenen Rechtecks angeben. Wenn Sie die Maße im Register Modelle angegeben haben, werden die Werte in die Position zurückgeschrieben und können dort nicht mehr geändert werden.
3.  Wechseln Sie zum Register Modelle/Bearbeitungen.
4.  Wählen Sie über die Symbolschaltfläche Modelle aus.
    Die Felder zur Eingabe der Werte werden angezeigt.

5.  Wählen Sie das Modell aus, indem Sie die Modell- oder die Produktnummer eintragen oder über die entsprechende Symbolschaltfläche (B).
    ⇨ Softwarereferenz, "Positionen - Modelle/Bearbeitungen" auf Seite C-476
    Im Bereich Darstellung wird eine Skizze des Modells angezeigt und die Felder für die erforderlichen Maße werden freigeschaltet.

    *   **Abb. C-50: Modell erfassen**
        *   **A**: Maße eingeben
        *   **B**: Auswahl des Modells
        *   **C**: Maße zur Preisberechnung

6.  Tragen Sie die Maße für die Kanten ein (A).
    Beachten Sie dazu die Hinweise, z. B. bedeutet W1+W2<=W, dass die Summe der Werte für die Kanten W1 und W2 die Größe der Kante W nicht überschreiten darf.
    Wenn Sie alle Werte eingetragen haben, wird die Größe des umschriebenen Rechtecks angezeigt, das standardmäßig zur Preisberechnung herangezogen wird.

    *   **Abb. C-51: Modell erfasst**

7.  Wählen Sie im Menü Start > Speichern, um die Modelldaten zu übernehmen.
    Die Daten werden gespeichert.
8.  Wählen Sie im Menü Start > Speichern, um die Position zu speichern.
    Die Daten werden gespeichert und die Preisfelder werden aktualisiert.
    Sie können jetzt zusätzlich Bearbeitungen erfassen.
    ⇨ "So erfassen Sie eine Bearbeitung" auf Seite C-119

## Stufung erfassen

Zu jeder ISO-Position kann eine Stufung erfasst werden. Diese gilt immer für die gesamte Position.

### So erfassen Sie eine Stufung

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
2.  Erfassen Sie eine neue Position oder markieren Sie im Bereich Positionen die ISO-Position, zu der Sie die Stufung erfassen wollen.
3.  Wechseln Sie zum Register Modelle/Bearbeitungen.
4.  Wählen Sie die Stufung aus, indem Sie die Produktnummer eintragen oder über die entsprechende Symbolschaltfläche.
    Die Felder zur Eingabe der Werte werden angezeigt.

    *   **Abb. C-52: Stufung festlegen**
        *   **A**: Auswahl der Scheibe, für die die Stufung eingegeben wird: 1 = Außenscheibe, 2= Innenscheibe
        *   **B**: Eingabe der Werte pro Kante: positive Werte verkleinern die gewählte Scheibe, negative Werte vergrößern die Scheibe
    ⇨ Softwarereferenz, "Positionen - Stufung" auf Seite C-498

5.  Tragen Sie alle erforderlichen Maße ein.
    Die Felder für die Maße werden freigeschaltet. Wenn Sie kein Modell erfasst haben, wird automatisch eine rechteckige Scheibe dargestellt.
    Im Bereich Parameter bedeutet 1 die Außenscheibe und 2 die Innenscheibe.
    Achten Sie darauf, dass Sie die Checkbox 2 (A) für die Innenscheibe markiert haben. Sie müssen dann für diese Scheibe positive Werte in den Feldern eintragen, z. B. den Wert 15.
    Wenn Sie negative Werte (-15) eingeben, wird die Scheibe größer geschnitten. Das würde für die Scheibe 2 (innen) bedeuten, dass sie größer geschnitten wird als die Außenscheibe.
    Die Ansicht der Scheibe wird aktualisiert.

6.  Wählen Sie im Menü Start > Speichern, um die Daten der Stufung zu übernehmen.
    Die Daten werden gespeichert.
7.  Wählen Sie im Menü Start > Speichern, um die Position zu speichern.
    Die Daten werden gespeichert und die Preisfelder werden aktualisiert, wenn Sie einen Preis für die Stufung eingetragen oder aus den Preislisten übernommen haben.

> **Häufig benötigte Produktaufbauten als Makro speichern**
> Haben Sie einen Produktaufbau erfasst, den Sie für diesen Kunden oder ganz allgemein häufiger benötigen, können Sie diesen als Makro speichern und bei der nächsten Auftragserfassung abrufen.
> ⇨ Makro speichern

## Bearbeitung erfassen

Zu jeder Position können mehrere Bearbeitungen erfasst werden. Dazu müssen Sie jede weitere Bearbeitung zuerst als Komponente in die Stückliste einfügen. Bearbeitungen gelten immer für die gesamte Position.

> **Voraussetzung**
> Bearbeitungen müssen als Produkte in den Stammdaten angelegt sein.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So erfassen Sie eine Bearbeitung" auf Seite C-119
*   "So erfassen Sie Bearbeitungen für ein Modell" auf Seite C-121

### So erfassen Sie eine Bearbeitung

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
2.  Erfassen Sie eine neue Position oder markieren Sie im Bereich Positionen die Position, zu der Sie eine Bearbeitung erfassen möchten.
3.  Wechseln Sie zum Register Modelle/Bearbeitungen.
4.  Wählen Sie die Bearbeitung aus, indem Sie die Produktnummer eintragen oder über die entsprechende Symbolschaltfläche, z. B. Kantenbearbeitungen.
    Die Produktdaten für die Bearbeitung werden übernommen. Die Felder für die dazugehörigen Parameter werden angezeigt und freigeschaltet.
    Eine Beschreibung der Parameter pro Bearbeitungsart finden Sie in der Softwarereferenz.
    ⇨ Softwarereferenz, "Positionen - Bearbeitungen" auf Seite C-479

    *   **Abb. C-53: Bearbeitung: Beispiel Kanten sägen**
        *   **A**: Auswahl der Bearbeitung
        *   **B**: Auswahl der Kanten, die bearbeitet werden sollen
        *   **C**: Bezugsecken, Bezugskanten
        *   **D**: Gehrungswinkel

5.  Erfassen Sie die Parameter, indem Sie die Checkboxen (B) für die Kanten aktivieren oder deaktivieren und die Werte eingeben.
    Achten Sie dabei auf die Bezugsecken oder Bezugskanten (C) und rechnen Sie die Maße ggf. um.

> **Falsche oder fehlende Bearbeitungsparameter**
> Wenn zu einer Bearbeitung nicht die richtigen Parameter angezeigt werden, müssen Sie in der Produktverwaltung prüfen, ob dem Produkt die richtige Produktart und -gruppe zugeordnet ist.
> ⇨ Softwarereferenz, "Parameter" auf Seite C-480

6.  Wählen Sie im Menü Start > Speichern, um die Daten zu übernehmen.
    Die Daten werden gespeichert und die Preisfelder werden aktualisiert. In der Stückliste werden die Bearbeitung und der zugehörige Preis angezeigt.
    Wie Sie weitere Bearbeitungen erfassen, ist in der nachfolgenden Handlungssequenz beschrieben.
7.  Wählen Sie im Menü Start > Speichern, um die Position zu speichern.
    Die Daten werden gespeichert und die Preisfelder werden aktualisiert.

> **Häufig benötigte Produktaufbauten als Makro speichern**
> Haben Sie einen Produktaufbau erfasst, den Sie für diesen Kunden oder ganz allgemein häufiger benötigen, können Sie diesen als Makro speichern und bei der nächsten Auftragserfassung abrufen.
> ⇨ "Makro speichern" auf Seite C-166

### So erfassen Sie Bearbeitungen für ein Modell

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
2.  Erfassen Sie eine neue Position oder markieren Sie im Bereich Positionen die Position, zu der Sie das Modell erfasst haben.
    Die Handlungsschritte gelten auch für rechteckige Scheiben und für ISO-Positionen.
3.  Wechseln Sie zum Register Modelle/Bearbeitungen.
4.  Klicken Sie in der Stückliste auf das Hauptprodukt.
    Eine Komponente mit der Produktnummer 0 wird eingefügt.
5.  Markieren Sie die neue Komponente und wählen Sie die Bearbeitung aus, z. B. eine Stufung.
    Verfahren Sie so, wie in der vorausgehenden Handlungssequenz beschrieben.

## Motive erfassen

Sie können Motive bei Oberflächenbearbeitungen der Produktgruppe Beschichtung, Mattierung, Siebdruck, Flächen-Emaillierung, Sandstrahlung und Kolorieren erfassen.

Sie können ein Motiv auf zwei Arten erfassen:
*   Mit Siebnummer
*   Ohne Siebnummer

Die Unterschiede der beiden Erfassungsmethoden werden in der folgenden Lerneinheit gezeigt.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So legen Sie ein Motiv mit Siebnummer in den Stammdaten an" auf Seite C-123
*   "So erfassen Sie ein Motiv mit Siebnummer" auf Seite C-125
*   "So erfassen Sie ein Motiv ohne Siebnummer" auf Seite C-129

> **Voraussetzung**
> Die Motivdatei muss in einem Verzeichnis gespeichert sein, damit Sie ein Motiv erfassen und/oder ein Motiv mit Siebnummer anlegen können.

### So legen Sie ein Motiv mit Siebnummer in den Stammdaten an

1.  Speichern Sie die Motivdatei in dem Verzeichnis, über das Sie die Datei einfügen wollen.
2.  Wählen Sie Stammdaten > Produkte > Artikel > Motive.
    Der Dialog Motive wird geöffnet.
3.  Wählen Sie im Menü Start > Neu, um ein Motiv anzulegen.
    Die Felder im Bereich Motiv werden freigeschaltet.

    *   **Abb. C-54: Motiv mit Siebnummer anlegen**

4.  Tragen Sie eine Siebnummer (A) für das Motiv ein.
5.  Tragen Sie ggf. einen Namen (B) für das neue Motiv ein. Er sollte sprechend und eindeutig sein, damit Sie das Motiv anhand des Namens erkennen können.
6.  Fügen Sie die Motivdatei (C) über die Schaltfläche [Ordner] ein.
    Die Motivdatei wird im Vorschaufenster (D) angezeigt.

    *   **Abb. C-55: Beispiel - Motiv mit Siebnummer anlegen**
        *   **A**: Siebnummer
        *   **B**: Motivname
        *   **C**: Pfad für die Motivdatei
        *   **D**: Vorschau auf das Motiv
        *   **E**: Maximale Maße des Motivs

7.  Tragen Sie die maximale Breite und Höhe (E) des Siebs ein.
    Diese Maße aus den Stammdaten können nicht überschritten werden, wenn Sie in der Positionserfassung ein Motiv mit Siebnummer erfassen.
8.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Sie können das Motiv über die Siebnummer in der Bearbeitung erfassen.

### So erfassen Sie ein Motiv mit Siebnummer

> **Voraussetzung**
> Das Motiv muss in den Stammdaten angelegt sein, damit Sie es über die Siebnummer erfassen können.
> ⇨ "So legen Sie ein Motiv mit Siebnummer in den Stammdaten an" auf Seite C-123

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    Erfassen Sie eine neue Position oder markieren Sie im Bereich Positionen die Position, zu der Sie das Motiv erfassen wollen.
    In diesem Beispiel wird eine rechteckige ESG-Scheibe mit den Maßen 1100 x 2100mm gewählt.
2.  Wechseln Sie zum Register Modelle/Bearbeitungen.

    *   **Abb. C-56: Beschichtung als Produktgruppe wählen**
        *   **A**: Symbolschaltfläche für Beschichtung
        *   **B**: Produktnummer

3.  Wählen Sie die Bearbeitung aus, indem Sie die Produktnummer (B) eintragen oder auf die entsprechende Symbolschaltfläche (A) klicken.

    *   **Abb. C-57: Symbolschaltflächen der Produktgruppen für die Motiverfassung**
        *   **A**: Beschichtung
        *   **B**: Mattierung
        *   **C**: Siebdruck
        *   **D**: Flächen-Emaillierung
        *   **E**: Sandstrahlen
        *   **F**: Kolorieren

    In diesem Beispiel wird als Bearbeitung die Produktgruppe Beschichtung gewählt.
    Die Produktdaten für die Bearbeitung werden übernommen. Die Felder für die dazugehörigen Parameter werden angezeigt und freigeschaltet.
    Eine Beschreibung der Parameter pro Bearbeitungsart finden Sie in der Softwarereferenz.
    ⇨ Softwarereferenz, "Positionen - Bearbeitungen" auf Seite C-479

    *   **Abb. C-58: Motive erfassen: Beispiel Beschichtung**

4.  Wählen Sie die Vermaßungsart (A), den Referenzpunkt und die Referenzkante (D) und tragen Sie den Winkel (D) ein.
    Mit der Wahl der Vermaßungsart legen Sie fest, wie die eingegebenen Werte interpretiert werden sollen.
    Im Feld Referenz legen Sie fest, welche Ecke des Motivs (oder der Mittelpunkt des Motivs) sich auf den Einfügepunkt des Vermaßungstyps bezieht.
    Mit dem Winkel legen Sie fest, wie das Motiv in Bezug zur Referenzkante gedreht werden soll.

    *   **Abb. C-59: Bearbeitungsparameter mit Angabe einer Siebnummer**
        *   **A**: Vermaßungsart
        *   **B**: X-Wert, Y-Wert, Bezugsecke und Bezugskante für die Positionierung des Motivs
        *   **C**: Maße des Motivs
        *   **D**: Winkel, Referenzkante und Referenzpunkt des Motivs
        *   **E**: Farbvarianten
        *   **F**: Sättigung
        *   **G**: Ebene, auf der das Motiv angebracht wird
        *   **H**: Pfad der Motivdatei und Dateisuche
        *   **I**: Spiegeln
        *   **J**: Siebnummer

5.  Wählen Sie die Bezugskante(n) und/oder die Bezugsecke (B) und tragen Sie den X-Wert und Y-Wert (B) ein.
    Mit diesen Werten geben Sie den horizontalen und vertikalen Abstand zum Referenzpunkt, die Bezugskante(n) und/oder die Bezugsecke der Scheibe an, von denen aus das Motiv positioniert wird.
6.  Tragen Sie die Breite und Höhe (C) des Motivs ein.
    Mit den Maßen wählen Sie die Größe des Motivs. Standardmäßig werden die Maße der Scheibe angezeigt. Achten Sie darauf, dass der Ausschnitt nicht größer ist, als die Maximalmaße des Motivs aus den Stammdaten.

> **Motiv zu groß**
> Breite und Höhe des Motivs werden auf die Maximalmaße aus den Produktstammdaten gesetzt, wenn die eingetragenen Maße größer sind als die Maße aus den Stammdaten. Wiederholen Sie ggf. Schritt 6, um die Größe des Motivs anzupassen.

7.  Wählen Sie ggf. eine Variante (E).
8.  Tragen Sie die Siebnummer (J) der Motivdatei ein.
    ⇨ Tutorial, "So legen Sie ein Motiv mit Siebnummer in den Stammdaten an" auf Seite C-123
    Der Pfad der Motivdatei (H) wird im Feld Motiv angezeigt. Die Kombobox unter dem Feld wird gesperrt. Das Motiv wird in der grafischen Darstellung angezeigt.

> **Zugriff auf Motivdatei**
> Achten Sie darauf, dass die Motivdatei unter dem angegebenen Dateipfad gespeichert ist. Wenn die Datei verschoben wird, kann das Motiv nicht mehr über die Siebnummer gefunden werden.

*   **Abb. C-60: Motivvorschau nach Erfassen der Siebnummer**

9.  Tragen Sie ggf. die Sättigung (F) ein.
10. Wählen Sie die Bearbeitungsseite (G).
    Die Bearbeitungsseite Ebene/Level 1 entspricht der Außenseite der Scheibe, Ebene/Level 2 der Innenseite der Scheibe.
11. Markieren Sie ggf. die Checkbox Spiegeln (I).
    Das Motiv wird gespiegelt.
12. Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.

### So erfassen Sie ein Motiv ohne Siebnummer

1.  Speichern Sie die Motivdatei in dem Verzeichnis, über das Sie die Datei einfügen wollen.
2.  Erfassen Sie das Motiv wie in den Schritten 1 bis 7 und 9 bis 11 der vorausgehenden Handlungsanleitung beschrieben.
    ⇨ "So erfassen Sie ein Motiv mit Siebnummer" auf Seite C-125

    *   **Abb. C-61: Bearbeitungsparameter ohne Angabe der Siebnummer**
        *   **A**: Maße des Motivs
        *   **B**: Dateisuche und Pfad der Motivdatei
        *   **C**: Skalierungsmodus des Motivs

3.  Fügen Sie die Motivdatei über die Schaltfläche [Ordner] (B) ein.
4.  Wählen Sie in der Kombobox (C) die Skalierung des Motivs.
    Sie können die Option Frei skalierbar, Proportional Breite oder Proportional Höhe wählen:
    *   **Frei skalierbar**: Mit dieser Einstellung können Sie Maße (A) frei angeben. Dabei kann das Motiv verzerrt werden.
    *   **Proportional Breite/Proportional Höhe**: Mit diesen Einstellungen können Sie die Höhe oder die Breite des Motivs angeben. Das jeweils andere Maß wird proportional angepasst. Dabei kann das Motiv beschnitten werden.

    *   **Abb. C-62: Motivvorschau ohne proportionale Skalierung**
    *   **Abb. C-63: Motivvorschau mit proportionaler Skalierung**

5.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.

## Zuschlag für besondere Leistung erfassen

Sie können mehrere Zuschläge zu jeder Position erfassen, wenn zum Produktaufbau besondere Leistungen erbracht werden müssen. Eine solche besondere Leistung kann z. B. sein, dass in einer ISO-Einheit die Struktur- oder Beschichtungsebene geändert wird.

> **Voraussetzung**
> Leistungen müssen als Produkte in den Stammdaten angelegt sein. Sie sind in der Produktgruppe Leistungen zusammengefasst.

### So erfassen Sie einen Zuschlag für besondere Leistungen

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
    Beginnen Sie mit der Erfassung der Leistungen erst, wenn Sie alle Positionen des Auftrags vollständig erfasst und gespeichert haben. Wechseln Sie dazu ggf. zum Register Position.
2.  Wechseln Sie zum Register Leistung.

*   **Abb. C-64: Leistung erfassen – Beispiel Verpackungszuschlag**
    *   **A**: Auswahl der Position
    *   **B**: Produktnummer der Leistung

    Im Bereich Positionsbezug werden alle Auftragspositionen aufgelistet.
    ⇨ Softwarereferenz, "Positionen - Leistung" auf Seite C-513

3.  Wählen Sie die Leistung über die Suche aus oder geben Sie die Produktnummer (B) direkt in die Erfassungszeile ein.
    Die Felder werden mit den Werten aus den Stammdaten gefüllt.
4.  Prüfen Sie die Werte, z. B. den Preis oder die Darstellung.
    Der Preis der Leistung kann im Druck genauso dargestellt werden, wie bei jeder Stücklisten-Komponente.
    ⇨ "Berechnungseinstellung" auf Seite C-145
5.  Markieren Sie die Position(en) (A), für die diese Leistung berechnet werden soll.
    Mit [Alle] können Sie alle Auftragspositionen markieren, mit [Keine] entfernen Sie alle Markierungen. In der Erfassungszeile wird der Wert für die Leistungsgröße aktualisiert.
6.  Wählen Sie im Menü Start > Speichern, um die Daten zu übernehmen.
    Die Preise der Leistung werden aktualisiert. Die Leistung wird in die Stückliste aller markierten Positionen eingetragen.
7.  Wählen Sie im Menü Start > Neu und wiederholen Sie die Schritte 3 bis 6, um weitere Leistungen zu erfassen.
    Die Preise der Leistung werden aktualisiert. Die Leistung wird in die Stückliste aller markierten Positionen eingetragen.
8.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Daten werden gespeichert und die Preisfelder werden aktualisiert.

> **Leistung löschen**
> Sie können eine Leistung nicht über das Kontextmenü aus der Stückliste löschen. Wenn Sie eine Leistung wieder entfernen möchten, müssen Sie im Register Leistung die Zuordnung zu einer Position entfernen oder die gesamte Leistung löschen.

## Stücklistenaufbau bearbeiten

Sie können jeden Stücklistenaufbau an die Wünsche Ihres Kunden anpassen. Beachten Sie dabei Folgendes:

*   Gas wird immer als Komponente an den Abstandhalter angehängt.
*   Eine Folie können Sie vor oder nach einer Einzelscheibe in einem VSG einfügen.
*   Sprossen, Modelle, Bearbeitungen und Leistungen können Sie nur über die entsprechenden Register anhängen.
    *   ⇨ "Sprossen erfassen" auf Seite C-109
    *   ⇨ "Modell erfassen" auf Seite C-114
    *   ⇨ "Bearbeitung erfassen" auf Seite C-119

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So bearbeiten Sie den Stücklistenaufbau" auf Seite C-135
*   "So löschen Sie eine Stücklisten-Komponente" auf Seite C-137

### So bearbeiten Sie den Stücklistenaufbau

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
2.  Markieren Sie in der Stückliste die Komponente, hinter bzw. vor der Sie eine Komponente einfügen wollen.
3.  Öffnen Sie das Kontextmenü (rechte Maustaste) und wählen Sie den gewünschten Befehl aus.

    *   **Abb. C-65: Kontextmenü zur Stückliste öffnen**
    Die Anzeige wechselt zum Register Stückliste. Das Feld für die Produktnummer ist freigeschaltet.

4.  Geben Sie die Produktnummer ein oder wählen Sie das gewünschte Produkt aus, z. B. eine Füllung.

    *   **Abb. C-66: Produktnummer der neuen Komponente eingeben**
    *   **Abb. C-67: Produktnummer der neuen Komponente eingeben**

5.  Wählen Sie im Menü Start > Speichern, um die neue Komponente zu speichern.
    Die Daten werden gespeichert.

### So löschen Sie eine Stücklisten-Komponente

1.  Markieren Sie im Bereich Stückliste die Komponente, die Sie löschen möchten.
2.  Öffnen Sie das Kontextmenü und wählen Sie den Befehl Komponente löschen.
    Die Komponente wird aus der Stückliste entfernt.
3.  Klicken Sie auf [Speichern], um die Änderungen zu speichern.
    Die Daten werden gespeichert.

> **Leistung löschen**
> Sie können eine Leistung nicht über das Kontextmenü aus der Stückliste löschen. Wenn Sie eine Leistung wieder entfernen möchten, müssen Sie im Register Leistung die Zuordnung zu einer Position entfernen oder die gesamte Leistung löschen.
> ⇨ "Zuschlag für besondere Leistung erfassen" auf Seite C-132

## Auftragsposition bearbeiten oder hinzufügen

Sie können jeden Auftrag nach dem Speichern bearbeiten. Beachten Sie dabei, dass Bestellpositionen oder Zuschnitte bereits an die entsprechenden Schnittstellen übergeben sein können.

> **Bestellte Position ändern**
> Wenn Bestellpositionen bereits übergeben sind, werden die Eingabefelder gesperrt. Sie können über das Menü Funktionen > Gruppe Position > Gesperrte Position ändern freigeschaltet werden.
>
> **Auftragsposition kopieren**
> Sie können jede bereits erfasste und gespeicherte Position kopieren und als neue Position hinzufügen. Die Daten der neuen Position können anschießend angepasst werden, z. B. ein Glas austauschen. Diese Funktion eignet sich zum Erfassen von komplexen Stücklistenaufbauten, für die kein Produkt oder Makro angelegt ist.

### So kopieren Sie eine Auftragsposition

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
2.  Markieren Sie in der Übersicht die Position, die Sie kopieren möchten.
3.  Wählen Sie im Menü Start > Neu.
    Die neue Position wird mit den Daten der kopierten Position hinzugefügt.
4.  Bearbeiten Sie die Daten, z. B. die Maße.
5.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die neue Position wird gespeichert. Die Felder im Register Summen werden aktualisiert.
    ⇨ Softwarereferenz, "Dokument - Summen" auf Seite C-529

> **Alternative Kopierfunktion**
> Wenn Sie sehr viele Positionen erfasst haben, können Sie die gewünschte Position einfacher über die Funktion Kopie aus Position ... finden. Sie finden die Funktion im Menü Funktionen > Gruppe Position.

### Auftragsposition löschen

Sie können aus jedem Auftrag nach dem Speichern Positionen wieder entfernen. Beachten Sie dabei jedoch, dass Bestellpositionen oder Zuschnitte bereits an die entsprechenden Schnittstellen übergeben sein können.

#### So löschen Sie eine Auftragsposition

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
2.  Markieren Sie im Bereich Positionen die Zeile, die Sie löschen möchten.
3.  Wählen Sie im Menü Start > Löschen.
    Die Position wird aus der Liste und dem Auftrag entfernt. Die Felder im Register Summen werden aktualisiert.
    ⇨ Softwarereferenz, "Dokument - Summen" auf Seite C-529

## Übungen

### Positionen erfassen

Öffnen Sie Ihren Auftrag und erfassen folgende Positionen:
*   ISO-Einheiten mit Einfachgläsern Float 5 mm
    *   10 Stück à 600 x 800 mm
    *   10 Stück à 1000 x 1000 mm
*   Speichern Sie die Positionen und prüfen Sie, ob die automatischen Zuschläge eingefügt wurden.

### Positionen bearbeiten

Ändern Sie in den Positionen folgende Details:
*   Kopieren Sie eine Position, so dass Sie nun 3 Positionen erfasst haben.
*   Fügen Sie in einer der Positionen ein einfaches Sprossenmuster hinzu.
*   Ersetzen Sie in einer der Positionen die Außenscheibe durch ein Strukturglas.
*   Ergänzen Sie ein einfaches Modell mit Stufen.
*   Erfassen Sie zu diesem Modell zusätzliche Leistungen.

### Schnellanfrage beantworten

Erfassen Sie eine Schnellanfrage:
*   Speichern Sie alle Änderungen in Ihrem aktuellen Auftrag.
*   Starten Sie die Schnellanfrage und wählen Sie einen anderen Kunden aus.
*   Erfassen Sie eine ISO-Einheit mit VSG, die teilweise bestellt werden soll.
*   Erfassen Sie ein ESG, das vollständig bestellt werden soll.
*   Speichern Sie die Schnellanfrage so, dass ein neuer Auftrag erfasst ist.

### Position über Schnellerfassung eintragen

Erfassen Sie eine Position über die Schnellerfassung:
*   Aktivieren Sie die Option Produktfeld dynamisch.
*   Geben Sie folgende Werte ein:
    `215,8003-1000-500-1000-800`
*   Erfassen Sie eine weitere Position mit folgenden Werten:
    `150000,8001-1000-1000-120,8260-2-2`
*   Prüfen Sie, ob die Stückliste, das Modell und die Sprossen korrekt erfasst sind.

### Motive erfassen

Erfassen Sie ein Motiv:
*   Legen Sie ein Motiv in den Stammdaten an.
*   Wählen Sie eine bestehende Position und ergänzen Sie ein Motiv mit der angelegten Siebnummer.
*   Erfassen Sie eine neue Position und ergänzen Sie ein Motiv ohne Siebnummer.
*   Erfassen Sie ein Motiv mit proportionaler Skalierung und passen Sie die Parameter so an, dass das Motiv nicht beschnitten wird.

### Ergänzende Informationen

*   ⇨ Stammdaten, "Firmendaten - Parameter" auf Seite B-948
*   ⇨ Stammdaten, "Firmendaten - Preisberechnung" auf Seite B-959
*   ⇨ "Sprossen erfassen" auf Seite C-109
*   ⇨ "Modell erfassen" auf Seite C-114
*   ⇨ "Zuschlag für besondere Leistung erfassen" auf Seite C-132
*   ⇨ "Stücklistenaufbau bearbeiten" auf Seite C-134
*   ⇨ "Motive erfassen" auf Seite C-123

## Preise

### Lernziele

*   Preisberechnung in A+W Business kennenlernen (Preise, Zuschläge, Rabatte).
*   Darstellung der Preise kennenlernen.
*   Preise im Auftrag bearbeiten.

### Nutzen

*   Preisgestaltung durch vorgegebene Preise, Rabatte und Zuschläge macht individuelle Eingriffe i. d. R. überflüssig.
*   Wenn Sie die Zusammenhänge in der Preisgestaltung kennen, können Sie Preise individueller gestalten.

### Merke

*   **Preis muss am Produkt aktiviert werden**: Ein Preis kann nur dann aus den Stammdaten übernommen werden, wenn in der Produktverwaltung das Kennzeichen preisrelevant gesetzt ist.
*   **Manuelle Änderungen**: Preise und Zuschläge können für jede Position manuell erfasst werden, jedoch sind auch dafür entsprechende Definitionen in den Stammdaten hilfreich.
*   **Preisänderungen zurücksetzen**:
    *   In der Positionserfassung können Sie manuelle Preisänderungen insgesamt zurücknehmen:
    *   Menü `Funktionen > Positionspreisvorgabe löschen` löscht die manuellen Änderungen einer Position.
    *   Menü `Funktionen > Vorgaben Position löschen` setzt die Änderungen auf die Werte aus den Stammdaten zurück.
*   Die manuelle Bearbeitung von Preisen im Auftrag kann durch ein Passwort geschützt werden.

**Stammdaten:**
*   Zuschläge
*   Rundungen

**Firmendaten:**
*   Register Dokumente (Mindestpreisunterschreitung)
*   Register Preisberechnung

### Anzeige der Preise im Dialog

Wenn Sie ein Produkt im Dokument erfassen, werden die Preise aus den Stammdaten als Vorgabe übernommen.

*   **Abb. C-68: Anzeige der Positionspreise**
    *   **A**: Gesamtpreis des Auftrags
    *   **B**: Preis und Preiseinheit pro Komponente
    *   **C**: Positionspreis pro Stück im Einkauf
    *   **D**: Positionspreis im Verkauf
    *   **E**: Stückpreis pro Position (nur Hauptprodukt) einschließlich Rabatt
    *   **F**: Rabatt auf den Preis pro Stück
    *   **G**: Stückpreis pro Position
    *   **H**: Preis pro Preiseinheit

In diesem Beispiel sehen Sie, wie die aktuellen Preise in der Positionserfassung berechnet und angezeigt werden:
*   Der Positionspreis des Hauptproduktes (G) wird aus der berechneten Menge (Fläche), dem Preis pro Einheit (H) und dem Rabatt (F) errechnet.
*   Der Stückpreis (G) pro Position setzt sich aus dem Positionspreis für das Hauptprodukt (E), dem Preis für zusätzliche Komponenten, z. B. Sprossen, Modell und Bearbeitung, und ggf. dem Austauschzuschlag (B) zusammen.
*   Der Austauschzuschlag (B) gibt den Betrag pro berechnete Menge wieder.

Der Auftragswert wird im Register **Summen** angezeigt.

*   **Abb. C-69: Anzeige der Preise**
    *   **A**: Summe der Aufträge dieses Kunden
    *   **B**: Auftragssumme in Landeswährung + Fremdwährung
    *   **C**: Manuelle Vorgabe für Festpreis und Rabatt
    *   **D**: Steuerbetrag
    *   **E**: Bruttobetrag
    *   **F**: Angezahlter Betrag
    *   **G**: Anzahlung eingeben
    *   **H**: Kosten (nach Rückmeldung aus Kapazitätsplanung oder Produktion)

## Preise und Preisberechnung

Die Preise, Zuschläge und Rabatte werden aus den Stammdaten übernommen und können manuell pro Position und Auftrag überschrieben werden. Die Auftragssumme und die Positionssummen werden automatisch aktualisiert. Manuell bearbeitete Werte werden in roter Schrift dargestellt.
Die Preise können im Druck wahlweise als Netto- oder als Bruttopreise dargestellt werden.

> **Preise aus den Stammdaten übernehmen**
> Grundsätzlich kann ein Preis nur dann aus den Stammdaten übernommen werden, wenn in der Produktverwaltung das Kennzeichen preisrelevant gesetzt ist.
> ⇨ Stammdaten, "Preis-Parameter" auf Seite B-612

### Manuelle Preisänderung

Die Preisänderung einer Position bezieht sich immer auf das Hauptprodukt. Wenn Sie den Preis einer Stücklisten-Komponente ändern, wird der neue Preis im Hauptprodukt dazugerechnet.
⇨ "Preis der Stücklisten-Komponente bearbeiten" auf Seite C-154

Die vorgegebenen Preise können Sie auf folgenden Ebenen ändern:
*   Preisjahrgang und Preisschlüssel
*   Preis pro Preiseinheit
*   Festpreis für ein Stück der Position
*   Festpreis für die gesamte Position
*   Festpreis für eine Gruppe von Positionen
*   Festpreis für den gesamten Auftrag
*   Preis für eine Stücklisten-Komponente
*   Rabatte

Um den Positionspreis ohne Rabatte und individuelle Preise darzustellen, muss in den Firmendaten die Option Erweiterte Preisfindung gesetzt werden. Die angezeigten Daten werden nicht weiter verarbeitet. Das Feld dient nur zur Auswertung mit Reports.
⇨ Stammdaten, "Erweiterte Preisfindung (Referenzpreis, manuelle Änderung)" auf Seite B-967

### Berechnungseinstellung

Für die Berechnung der Preise können Sie unterschiedliche Einstellungen festlegen. Die Parameter zur Preisberechnung werden übergreifend in den Firmendaten festgelegt und können pro Auftrag überschrieben werden.
⇨ Stammdaten, "Firmendaten - Preisberechnung" auf Seite B-959

Daneben legen Sie im Produkt und in der Stückliste im Auftrag fest, wie die einzelnen Preise in der Berechnung dargestellt werden:
*   **Implizit**: Der Preis der Hauptposition beinhaltet alle Preise der Stücklisten-Komponenten, also auch die Modell- und Austauschzuschläge und die Bearbeitungen.
*   **Explizit**: Der Preis wird einzeln ausgewiesen.
*   **Implizit in Preis pro Mengeneinheit**: Die Preise der Stücklisten-Komponenten werden umgerechnet auf die Preiseinheit des Hauptproduktes. Dieser Gesamtpreis der Preiseinheit wird im Dokument ausgewiesen, aber nur dann, wenn allen Stücklisten-Komponenten einer Position die gleiche Darstellungsart zugewiesen wurde.

**Beispiel: Preisdarstellung implizit in Preis pro ME**
In diesem Beispiel ist ein Glas Float 5 mm, 1000 x 2000 mm mit zwei Lochbohrungen erfasst. Der Glaspreis beträgt 10 €/qm. Für die Lochbohrungen werden 5 €/Stk. berechnet, wobei das Preiskennzeichen auf implizit gesetzt ist.

Daraus ergibt sich folgende Berechnung:

| Beschreibung | Berechnung | Wert |
| :--- | :--- | :--- |
| Gesamtpreis pro qm | | 15 € |
| Gesamtpreis Glas | | 20 € |
| Gesamtpreis Lochbohrung | | 10 € |
| Gesamtpreis | | 30 € |
| ÷ Gesamt-qm | | ÷ 2 |
| **Preis/qm** | | **15 €** |

Der Preis der Lochbohrung wird in den Preis/Preiseinheit des Hauptprodukts (hier das Glas -> qm) hineingerechnet (impliziert).

### Preise fixieren

Wenn Aufträge in Ihrem Unternehmen von verschiedenen Mitarbeitern bearbeitet werden, können Sie die Preise in einem Auftrag fixieren. Diese sind dann für die weitere Bearbeitung gesperrt. Der Auftrag selbst kann weiterhin bearbeitet werden. Sie können daneben auch die gesamte Auftragsposition fixieren.
⇨ Softwarereferenz, "Artikel fixieren" auf Seite C-624

### Aktualisierung der Auftragssummen

Die Aktualisierung der Positionssummen kann wahlweise sofort oder erst beim Speichern des Auftrags durchgeführt werden.
Wenn die Preise geändert werden, müssen die Summen neu berechnet werden. Da dies durch den gesetzten Merker (Flag) nicht automatisch geschieht, müssen Sie die Neuberechnung durch die Funktion **Summen zwangsweise errechnen** aktivieren.
Wenn die Produkt- und Preisdefinitionen in den Stammdaten geändert werden, werden die neuen Daten nicht automatisch in bestehende Dokumente übernommen. Mit dem Menü **Überrechnen** stehen verschiedene Optionen zur Verfügung, mit denen Sie einstellen können, welche Daten neu eingelesen werden und was in den betreffenden Dokumenten neu berechnet werden soll.
⇨ Softwarereferenz, "Überrechnen" auf Seite C-692

Vor dem Überrechnen wird das Dokument auf Duplikate geprüft. Werden Duplikate gefunden, wird die Überrechnung abgebrochen.

> **Überrechnung nach Rücksprache starten**
> Lassen Sie sich vor dem Starten der Überrechnung von Ihrem Ansprechpartner bei der A+W Software GmbH unterstützen, bevor Sie die Funktion zum ersten Mal nutzen wollen.

### Preisrecorder

Über den Preisrecorder werden die manuellen Preise für einzelne Auftragspositionen aufgelistet. In einem bestimmbaren Vergleichszeitraum werden die Preiskonditionen für Angebote und Aufträge (inklusive Archiv) herangezogen. Der Preisrecorder unterscheidet bei der Suche die Hauptprodukt- und die Stücklistenebene.

So können Sie ein Angebot zu den gleichen Konditionen erstellen, die zuvor schon einmal gewährt wurden.

Das Suchergebnis ist abhängig von der Startposition, aus der Sie den Preisrekorder aufrufen:
*   **Stücklisten-Komponenten**: Wenn Sie in einer Stückliste z. B. das Austauschglas Ornament markiert haben und den Preisrecorder starten, wird nur das betreffende Ornamentglas als Teil einer Stückliste gesucht.
*   **Hauptprodukt**: Wenn Sie sich im Register ISO oder Artikel den Preisrecorder starten, sucht das Programm nur auf der Hauptproduktebene nach diesem Artikel bzw. Isolierglas.
*   **Produktaufbau**: Sie können zusätzlich einen Filter aktivieren, damit auch der Produktaufbau berücksichtigt wird.

Die gefundenen Preiskonditionen können in die aktuelle Position übernommen werden. Manuelle Preise und Rabatte müssen gesondert bestätigt werden.

*   **Abb. C-70: Preisrekorder**
    *   **A**: Eingrenzung auf Dokumentenart
    *   **B**: Eingrenzung auf Archivjahre
    *   **C**: Eingrenzung auf Erfassungszeitraum

### Formeln

In den Preisstammdaten können Preisformeln hinterlegt werden. Diese werden während der Preisberechnung im Dokument ausgeführt. Die Berechnung nach einer Formel wird für Preise von Positionen und der Stücklisten-Komponenten durchgeführt.

*   **Abb. C-71: Auswahl der Preisformel**

### Alternativen

Der Preis für alternative Positionen (im Angebot) fließt nicht in die Gesamtsumme des Auftrags ein.
Bei der Berechnung von Alternativangeboten werden auch die automatischen Zuschläge ermittelt.
Angebote werden Sie in einer separaten Lerneinheit kennenlernen:
⇨ "Angebote" auf Seite C-334

### Festlegung von Mindestwerten

Für die Berechnung können folgende Mindestwerte definiert werden:
*   **Auftragsmindestwert**: Ist in den Kundenstammdaten ein Mindestwert für einen Auftrag festgelegt, werden die Auftragssummen entsprechend berechnet.
*   **Rechnungsmindestwert**: In den Kundenstammdaten kann ein Mindestwert pro Rechnung festgelegt werden.
*   **Rechnungsstellungszuschlag**: In den Kundenstammdaten kann ein Rechnungsstellungszuschlag auf einen Mindestwert pro Rechnung festgelegt werden.
*   **Mindestpreis**: Wird der Standardpreis des Kunden durch manuelle Änderungen unterschritten, wird der Differenzbetrag angezeigt. Sie müssen dann eine Begründung für den neuen Preis eingeben. Sie können die Unterschreitung des Mindestpreises mit einem Passwort schützen.
    Die Änderung des Tarifs ist keine Preisänderung und muss daher nicht begründet werden.
    Die Begründungen können in einem Report ausgegeben werden. Nach dem Ausdruck kann das Druckkennzeichen zurückgesetzt werden und die Positionen werden im nächsten Druck nicht mehr aufgeführt.
    Diese Funktion steht zur Verfügung, wenn die erweiterte Preisfindung aktiviert ist.

**Ergänzende Informationen**
*   ⇨ Stammdaten, “Partnerverwaltung - Auftrag" auf Seite B-775
*   ⇨ Stammdaten, "Mindestpreisunterschreitung" auf Seite B-945
*   ⇨ Stammdaten, "Erweiterte Preisfindung (Referenzpreis, manuelle Änderung)" auf Seite B-967
*   ⇨ Softwarereferenz, "Gruppe Position" auf Seite C-452
*   ⇨ Softwarereferenz, "Preisänderung (Report)" auf Seite C-724

### Zuschläge und Leistungen

Die automatischen Zuschläge werden an letzter Position im Auftrag eingefügt und fließen in die Berechnung des Gesamtbetrags ein.
Wird ein Zuschlag oder Rabatt im Dokumentenkopf aktiviert oder deaktiviert, werden alle Positionen überrechnet.
⇨ Softwarereferenz, "Zuschläge/Rabatte" auf Seite C-439

Die Berechnung von Zuschlägen und Leistungen kann auf die gerundete Menge (Fläche) umgestellt werden. Im Auftrag kann diese Einstellung übersteuert werden, wenn nach tatsächlicher Fläche gerechnet werden soll. Sie müssen dazu die Option **Preiseinheit qm (tat.)** aktivieren.
⇨ Stammdaten, "Zuschläge mit gerundeter Menge berechnen" auf Seite B-965

## Positionspreis ändern

Sie können in einem Auftrag sowohl die Beträge als auch die Preiseinheit ändern. Diese Änderungen betreffen nur die markierte Position. In dieser Einheit lernen Sie, wie Sie die Preise, Rabatte und Zuschläge in einer erfassten Position ändern.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So ändern Sie den Stückpreis einer Position" auf Seite C-151
*   "So ändern Sie den Preis für ein Austauschglas" auf Seite C-153
*   “So ändern Sie Preisangaben zu einer Stücklisten-Komponente" auf Seite C-154
*   "So ändern Sie den Preis von Sprossen" auf Seite C-155

> **Preisänderungen zurücksetzen**
> Manuelle Änderungen können mit der Funktion **Positionspreisvorgaben löschen** auf die Standardwerte zurückgesetzt werden. Dies gilt nicht für Makro-Preise. Makro-Preise können Sie nur manuell ändern oder indem Sie das Makro bearbeiten und neu zuweisen.
>
> Wie Sie einen Festpreis für die Position festlegen, finden Sie unter:
> ⇨ "Festpreis eingeben" auf Seite C-158

### So ändern Sie den Stückpreis einer Position

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
2.  Markieren Sie die Position, in der Sie den Preis ändern möchten.
    Sie können den Stückpreis einer Position folgendermaßen ändern:
    *   Den Stückpreis oder den Wert im Feld VK überschreiben, um einen Festpreis festzulegen.
    *   In der Erfassungszeile den Schlüssel, den Preis pro Einheit, die Einheit und/oder den Rabatt ändern.
    In diesem Beispiel werden die Werte in der Erfassungszeile geändert.

    *   **Abb. C-72: Stückpreis der Position ändern**
        *   **A**: Preisjahrgang
        *   **B**: Preisschlüssel
        *   **C**: Preis pro Preiseinheit
        *   **D**: Preiseinheit
        *   **E**: Rabatt
        *   **F**: Stückpreis der Position (Glas)

3.  Wählen Sie in der Erfassungszeile eine oder mehrere der folgenden Möglichkeiten:
    *   **Im Feld Jahrgang (A)**: Mit der Änderung des Preisjahrgangs muss darauf geachtet werden, dass dem gewählten Jahrgang ein Schlüssel zugeordnet ist.
    *   **Im Feld Schlüssel (B)**: Die Änderung des Preisschlüssels ändert alle damit verbundenen Definitionen.
    *   **Im Feld Preis/PE (C)**: Die Änderung des Betrags wirkt sich nur auf das Hauptprodukt aus, Austauschzuschläge usw. bleiben davon unberührt.
    *   **Im Feld Einheit (D)**: Die Änderung der Preiseinheit wirkt sich nur auf das Hauptprodukt aus. Sie können auf diese Weise keine Festpreise für die Position erfassen.
        ⇨ "Festpreis eingeben" auf Seite C-158
    *   **Im Feld Rabatt (E)**: Die Änderung des Rabattsatzes wirkt sich nur auf das Hauptprodukt aus, Rabatte für Stücklisten-Komponenten bleiben standardmäßig davon unberührt.
        Ausnahmen: Bei Austauschgläsern und allen Stücklisten-Komponenten kann die Übernahme des Rabatts in den Firmendaten festgelegt werden.
        *   ⇨ Stammdaten, "Rabattübernahme Hauptpos. Vorrang vor Bearb.-Rabatt 0%" auf Seite B-963
        *   ⇨ Stammdaten, "Keine fixe Übern. des Pos.-Rabatts bei Austauschzuschl." auf Seite B-963

    *   **Abb. C-73: Preisänderung der Position**

    Die geänderten Werte werden in roter Schrift dargestellt. Im Bereich Verkaufspreise werden die Felder aktualisiert.

4.  Klicken Sie auf [Speichern], um die Daten zu speichern.
    Die Preise werden gespeichert. Die Werte im Register Summen werden aktualisiert.
    ⇨ Softwarereferenz, "Dokument - Summen" auf Seite C-529

### So ändern Sie den Preis für ein Austauschglas

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461

    *   **Abb. C-74: Preis für Austauschglas ändern**
        *   **A**: Preis des Austauschglases
        *   **B**: Austauschglas

2.  Markieren Sie das ausgetauschte Glas in der Stückliste (B).
3.  Ändern Sie den Preis und/oder die Preiseinheit (A) wie gewünscht.
    Die geänderten Werte werden in roter Schrift dargestellt. Die Felder werden aktualisiert.
4.  Klicken Sie auf [Speichern], um die Änderungen zu speichern.
    Die Preise werden gespeichert. Die Werte im Register Summen werden aktualisiert.

### Preis der Stücklisten-Komponente bearbeiten

Die Preisänderung einer Stücklisten-Komponente wird zum Hauptprodukt dazugerechnet und ergibt dann den neuen Stückpreis der Position.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So ändern Sie Preisangaben zu einer Stücklisten-Komponente" auf Seite C-154
*   "So ändern Sie den Preis von Sprossen" auf Seite C-155

#### So ändern Sie Preisangaben zu einer Stücklisten-Komponente

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
2.  Wechseln Sie zum Register Stückliste.
3.  Markieren Sie die Komponente, deren Preisangaben Sie ändern möchten.

    *   **Abb. C-75: Preis einer Komponente ändern**
        *   **A**: Preisangaben zur markierten Komponente
        *   **B**: Änderung des Preiskennzeichens

4.  Ändern Sie im Bereich **Verkaufspreise** (A) die Werte wie gewünscht, z. B. den Jahrgang.
    Wenn Sie die Zuschlagsart ändern, beachten Sie bitte die Erläuterungen und Beispiele im Part **Stammdaten**.
    ⇨ Stammdaten, "Berechnungen nach Zuschlagsarten" auf Seite B-319
    Die geänderten Werte werden in roter Schrift dargestellt.
5.  Klicken Sie auf [Speichern], um die Daten zu speichern.
    Die Preise werden gespeichert. Die Werte der Stück- und Positionspreise und die Werte im Register Summen werden aktualisiert.

#### So ändern Sie den Preis von Sprossen

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
2.  Erfassen Sie eine neue Position oder markieren Sie die Position, zu der Sie Sprossen erfasst haben.
3.  Wechseln Sie zum Register Sprossen.
    ⇨ Softwarereferenz, "Positionen - Sprossen" auf Seite C-504
    Im Bereich **Verkaufspreise (B)** wird der Gitterpreis für die gesamte Sprossenkonstruktion angezeigt. Sie können diesen Preis überschreiben, wenn Sie den Gesamtpreis (Stückpreis) des Gitters festlegen möchten.

    *   **Abb. C-76: Preis der Sprossen ändern**
        *   **A**: Register Preise (Sprossen)
        *   **B**: Preisvorgaben aus der Produktdefinition

4.  Wechseln Sie zum Register Preise (A).
    Die Standard-Preise für die Sprossen werden angezeigt.

    *   **Abb. C-77: Preis in der Sprossenkonstruktion ändern**
        *   **A**: Einzelpreise der Sprossenkonstruktion
        *   **B**: Preis pro Preiseinheit

5.  Ändern Sie die Preise und Preiseinheiten wie gewünscht.
    *   Im Bereich **Gitter** den Preis der einzelnen Teile der Konstruktion. Achten Sie dabei darauf, dass Sie die Angaben für die waagerechten und die senkrechten Sprossen getrennt eintragen müssen.
    *   Im Bereich **Verkaufspreise** den Tarif die Preiseinheit und/oder den Rabatt.
    *   Im Bereich **Sprossenartikel** den Preis pro Preiseinheit
    Die geänderten Werte werden in roter Schrift dargestellt. Im Bereich Preise werden die Felder aktualisiert.
    Sie können die Änderungen über das Menü **Funktionen > Vorgaben löschen** auf die Standardwerte zurücksetzen.

> **Gitterpreis ändern**
> Der Preis im Bereich Preise bezieht sich auf das gesamte Gitter. Wenn Sie diesen Preis ändern, müssen Sie die Menge (Lfm) der Sprossen mit bedenken.

6.  Wählen Sie im Menü Start > Speichern, um die Änderungen zu übernehmen.
    Die Anzeige wechselt zum Register Position.
7.  Wählen Sie im Menü Start > Speichern, um die Position zu speichern.
    Die Werte der Stück- und Positionspreise und die Werte im Register Summen werden aktualisiert.

### Festpreis eingeben

In jedem Auftrag können Sie die regulären Preise mit vereinbarten Festpreisen überschreiben. Ein Festpreis kann sich auf ein Stück einer Position beziehen, auf die gesamte Position oder auf den gesamten Auftrag.

Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
*   "So legen Sie den Festpreis für den gesamten Auftrag fest" auf Seite C-159
*   "So legen Sie einen Festpreis für die Position fest" auf Seite C-160
*   "So legen Sie einen gemeinsamen Festpreis für mehrere Positionen fest" auf Seite C-161

#### So legen Sie den Festpreis für den gesamten Auftrag fest

1.  Öffnen Sie den Auftrag, den Sie bearbeiten möchten.
    ⇨ Softwarereferenz, "Dokument - Kopfdaten" auf Seite C-424
2.  Wechseln Sie zum Register Summen.

    *   **Abb. C-78: Festpreis für den gesamten Auftrag festlegen**
        *   **A**: Festpreis für den gesamten Auftrag
        *   **B**: Rabattsatz für den gesamten Auftrag

3.  Tragen Sie den Festpreis (A) und ggf. den neuen Rabatt (B) für den gesamten Auftrag ein.
    Die geänderten Werte werden in roter Schrift dargestellt. Die Felder werden aktualisiert.
4.  Klicken Sie auf [Speichern], um die Daten zu speichern.
    Der Festpreis wird anteilig als Stückpreise auf die Positionen umgerechnet. Die Positionspreise und die Werte im Register Summen werden aktualisiert.

#### So legen Sie einen Festpreis für die Position fest

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
2.  Markieren Sie die Position, zu der Sie einen Festpreis angeben wollen.

    *   **Abb. C-79: Festpreis in der Position festlegen**
        *   **A**: Festpreis pro Stück
        *   **B**: Festpreis für die Position

3.  Wählen Sie eine der folgenden Möglichkeiten:
    *   Geben Sie im Feld **VK (B)** den Festpreis für die aktuelle Position ein.
    *   Geben Sie im Feld **Stückpreis (A)** den Festpreis pro Stück der Position ein.
    Die geänderten Werte werden in roter Schrift dargestellt. Die Felder **Stückpreis**, **Gesamt**, **Preis/PE** und **Einheit** werden aktualisiert. Die Preiseinheit wird immer auf **Stk** gesetzt.
4.  Klicken Sie auf [Speichern], um die Änderungen zu speichern.
    Die Preise und die Werte im Register Summen werden aktualisiert.

> **Stückpreis in der Erfassungszeile festlegen**
> Wenn Sie den Stückpreis in der Erfassungszeile festlegen, werden für die Berechnung der Position auch die Rabatte und Zuschläge herangezogen. Der errechnete Wert kann daher von einem Festpreis pro Stück abweichen.

#### So legen Sie einen gemeinsamen Festpreis für mehrere Positionen fest

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
2.  Markieren Sie die Positionen, zu denen Sie den Festpreis eingeben möchten.
3.  Öffnen Sie das Kontextmenü (rechte Maustaste).

    *   **Abb. C-80: Festpreis für mehrere Positionen festlegen**
        *   **A**: Markierte Positionen
        *   **B**: Kontextmenü

4.  Wählen Sie den Befehl **Festpreis vorgeben (B)**.

    *   **Abb. C-81: Gesamtpreis für mehrere Positionen**
        *   **A**: Festpreis für alle aufgeführten Positionen
        *   **B**: Positionspreise
    ⇨ Softwarereferenz, "Festpreis Vorgabe" auf Seite C-608

5.  Geben Sie den Betrag (A) ein, der für alle markierten Positionen insgesamt berechnet werden soll.
    Wenn Sie mit <Tab> weiter springen, werden die Beträge auf die aufgeführten Positionen umgerechnet. Die Rabatte werden in die Berechnung einbezogen. Die geänderten Werte werden in roter Schrift dargestellt.
6.  Klicken Sie auf [OK], um den Festpreis zu übernehmen.
    Der Dialog wird geschlossen. In der Positionserfassung werden die Felder **Stückpreis**, **Gesamt**, **Preis/PE** und **Einheit** aktualisiert.
7.  Klicken Sie auf [Speichern], um die Daten zu speichern.
    Die Felder **Stückpreis**, **Gesamt**, **Preis/PE** und **Einheit** und die Werte im Register **Summen** werden aktualisiert.

> **Festpreisvorgabe zurücksetzen**
> Sie können diesen Festpreis über das Kontextmenü und den Befehl **Vorgabe Festpreis löschen** rückgängig machen. Wenn Sie über das Menü **Funktionen > Positionspreisvorgabe löschen** gehen, werden alle manuellen Preisvorgaben in der Positionserfassung zurückgesetzt.

### Übungen

**Preise der Positionen ändern**
Erfassen Sie einen neuen Auftrag mit identischen 3 Positionen:
*   Einfachglas, Float 5 mm, 1000 x 1000 m, 10 Stück
*   Ändern Sie in Position 1 den Preis pro Preiseinheit.
*   Ändern Sie in Position 2 den Preis der gesamten Position.
*   Ändern Sie in Position 3 den Stückpreis.
*   Vergleichen Sie die Preise, die pro Position berechnet werden.

**Rabatt ändern und Festpreis eingeben**
Erfassen Sie einen neuen Auftrag wie in der Übung zuvor:
*   Ändern Sie nun den Rabatt für Position 1.
*   Erfassen Sie in Position 2 einen Festpreis.
*   Ändern Sie in Position 3 die Preisliste.

**Sprossenpreise ändern**
Öffnen Sie Ihren Auftrag mit den Sprossen-Positionen:
*   Ändern Sie die Preise pro Sprosse.
*   Ändern Sie den Preis für das gesamte Sprossengitter.

**Ergänzende Informationen**
*   ⇨ “Anzeige der Preise im Dialog" auf Seite C-142
*   ⇨ "Darstellung der Preise im Druck" auf Seite C-206
*   ⇨ "Einstellungen für den Preisdruck" auf Seite C-208
*   ⇨ Softwarereferenz, "Menü Funktionen" auf Seite C-417
*   ⇨ Softwarereferenz, "Preisänderung (Report)" auf Seite C-724
*   ⇨ Stammdaten, "Firmendaten" auf Seite B-930

## Makros

### Lernziele

*   Makros anlegen.
*   Mit Makros arbeiten.

### Nutzen

*   Mit Makros können Sie die Erfassung von Auftragspositionen für wiederkehrende Produktaufbauten und/oder Preise vereinfachen.

### Merke

*   **Makro anlegen**: Jeder Produktaufbau kann als Makro(befehl) gespeichert werden.
*   **Verfügbarkeit von gespeicherten Makros**: Makros werden auf unterschiedliche Art gespeichert:
    *   Sie können für alle Kunden ausgewählt werden.
    *   Sie stehen nur für den aktuellen Kunden zur Verfügung.
*   **Position über Makro erfassen**: Mit der Auswahl eines Makros werden alle Felder der Positionserfassung gefüllt. Die Werte können anschließend bearbeitet werden.
*   **Voreinstellungen**: Keine

### Makros für Produktaufbauten und Preise

Sie können einen Produktaufbau einschließlich der erfassten Preise als Makro speichern. Ein Makro wird allgemein oder kundenspezifisch abgelegt. Es steht dann entweder nur für den einen oder für alle Kunden zur Verfügung.
Alle Makros können gelöscht werden, ohne dass die erfassten Positionen davon berührt werden.

**Verfügbare Makros**
Wenn Sie ein Makro aus dem Suchdialog auswählen, können Sie den Produktaufbau und die Stückliste zuvor prüfen. Ist ein Produkt per Makro in die Positionserfassung übernommen worden, kann es ganz normal weiter bearbeitet werden.
Verfügbare Makros werden in der Erfassungszeile über eine eigene Suchfunktion eingefügt.
Wenn Sie häufig mit Makros arbeiten, können Sie die Makrosuche in der Erfassungszeile aktivieren.

*   **Abb. C-82: Makrosuche**
    *   **A**: Eigenschaften der Tabelle
    *   **B**: Makrosuche aktiviert

⇨ Softwarereferenz, "Makros" auf Seite C-637

### Makro speichern

In dieser Einheit lernen Sie, wie Sie ein Makro anlegen. Damit speichern Sie einen Produktaufbau und/oder Preis als Makro. Sie können die Funktion auch nutzen, um einen Produktaufbau als Makro für einen anderen Kunden zu übernehmen.

#### So speichern Sie ein Makro

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
2.  Erfassen Sie das Produkt mit allen benötigten Angaben, z. B. Maße, Preise, Stücklisten-Komponenten, Modelle und Bearbeitungen.
    ⇨ "So erfassen Sie eine Position" auf Seite C-97
3.  Speichern Sie die erfassten oder geänderten Daten.
    Achten Sie darauf, dass die Position markiert ist, deren Aufbau Sie als Makro speichern wollen.
4.  Prüfen Sie im Menü Aufbau, ob die Einstellungen für die Erfassung des Makros stimmen.
    Wenn der Eintrag **Nur Produktaufbau aus Makro übernehmen** nicht aktiviert ist, werden alle Angaben aus dem Makro gespeichert, also z. B. auch die Preise.
5.  Wählen Sie im Menü Aufbau > Makro > Sichern.

    *   **Abb. C-83: Makro speichern**
    Die Kundennummer und der Name des Kunden werden im Bereich Kunde angezeigt.

> **Makro für einen anderen Kunden übernehmen**
> Mit der Funktion **Makro kopieren** können Sie alle kundenspezifischen Makros anderen Kunden zuordnen.
> ⇨ "Makros kopieren" auf Seite C-172

6.  Tragen Sie den Namen für das Makro ein.
    Tragen Sie den Namen so ein, dass Sie die wesentlichen Merkmale sofort erkennen können, z. B. `1004 gebogen`.
7.  Wählen Sie die Option für die Speicherung:
    *   **Kundenbezogen**: Das Makro steht nur für den gewählten Kunden zur Verfügung. Wenn Sie das Makro für einen anderen Kunden speichern wollen, müssen Sie diesen Kunden auswählen.
    *   **Allgemein**: Das Makro kann für jeden Kunden gewählt werden.

    *   **Abb. C-84: Kundenspezifisches Makro speichern**

8.  Klicken Sie auf [OK], um das Makro zu speichern.
    Das Makro wird gespeichert und der Dialog wird geschlossen.
9.  Wählen Sie im Menü Start > Speichern, um die Position zu speichern.
    Das Makro kann jetzt über die Erfassungszeile ausgewählt werden.

### Position über Makro erfassen

Um Positionen über ein Makro erfassen zu können, müssen Makros entweder allgemein oder für den aktuellen Kunden gespeichert sein. Ein kundenspezifisches Makro können Sie nur auswählen, wenn Sie einen Auftrag für den entsprechenden Kunden erfassen.

#### So erfassen Sie eine Position über ein Makro

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
2.  Prüfen Sie im Menü Aufbau, ob die Einstellung für die Erfassung über ein Makro stimmen.
    Wenn der Eintrag **Nur Produktaufbau aus Makro übernehmen** nicht aktiviert ist, werden alle Angaben aus dem Makro übernommen, also z. B. auch die Preise.
3.  Öffnen Sie den Dialog **Makrosuche**:
    *   Über Menü Aufbau > Makro > Suche.
    *   Über die Erfassungszeile

    *   **Abb. C-85: Gespeichertes Makro auswählen**

4.  Markieren Sie das gewünschte Makro, um den Aufbau der Stückliste zu prüfen.
5.  Klicken Sie auf [OK], um die Daten zu übernehmen.
    Die Felder in der Erfassungszeile, im Bereich **Produkt** und die Stückliste werden aktualisiert. Sie können die Daten bearbeiten, z. B. die Maße.
6.  Bestätigen Sie die Position mit <Enter>.
    Die Positionsdaten werden gespeichert und in der nächsten Zeile als neue Position vorgeschlagen. Sie können diese Daten zum Erfassen einer weiteren Position überschreiben oder ignorieren, wenn Sie keine weitere Position erfassen möchten.
    Sie können die Daten aller Positionen weiterbearbeiten.
7.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Felder im Register Summen werden aktualisiert.
    ⇨ Softwarereferenz, "Dokument - Summen" auf Seite C-529

### Makros ändern

Mit dieser Funktion können Sie in allen Makros die Preise und/oder die Rundung ändern.

> **Einzelnes Makro ändern**
> Über diese Funktion können Sie nicht einen einzelnen Preis oder einzelne Makros ändern. Wenn Sie ein einzelnes Makro ändern möchten, müssen Sie das alte Makro löschen und die neuen Daten in einem neuen Makro speichern.

#### So ändern Sie Preise und Rundungen in Makros

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
2.  Wählen Sie im Menü Aufbau > Makro > Ändern.

    *   **Abb. C-86: Makros für Änderung suchen**
        *   **A**: Option zur Auswahl der Makros
        *   **B**: Preisänderung
        *   **C**: Änderung der Rundung
    ⇨ Softwarereferenz, “Makro ändern" auf Seite C-638

3.  Wählen Sie im Bereich Auswahl die gewünschte Option (A) oder den Kunden aus, dessen Makros Sie ändern möchten.
    Sie können auch eine Folge von Kundennummern angeben. In diesem Beispiel werden alle Makros geändert.
4.  Klicken Sie auf [OK], um die gewünschten Makros aufzulisten.
    Im Bereich Makros werden alle Makros aufgelistet, die den Filtereinstellungen entsprechen.

    *   **Abb. C-87: Makros ändern**
        *   **A**: Wert der Preisänderung
        *   **B**: Wert ist absolut
        *   **C**: Wert ist prozentual
        *   **D**: Änderung der Rundung

5.  Wählen Sie im Bereich Preisänderung die Option:
    *   **Absolut (B)** und einen Wert (A), z. B. 5 oder -5, wenn die Preise um 5 Euro erhöht oder vermindert werden sollen.
    *   **Prozentual (C)** und einen Wert (A), z. B. 2 oder -2, wenn die Preise um 2 Prozent erhöht oder vermindert werden sollen.
6.  Wählen Sie ggf. eine andere Rundung (D) aus.
7.  Klicken Sie auf [OK], um die Makros zu ändern.
    Die neuen Preise werden in der Übersicht in roter Schrift angezeigt. Die Brutto- und Netto-Beträge werden neu errechnet.
8.  Klicken Sie auf [Ende], um den Dialog zu schließen.
    Der Dialog wird geschlossen. Die Positionserfassung wird wieder im Vordergrund angezeigt.

> **Neue Makro-Preise anwenden**
> Die Preise in einem Auftrag werden nicht automatisch aktualisiert, wenn Sie die neuen Makro-Preise gespeichert haben.

9.  Markieren Sie die Position, die über ein Makro erfasst wurde, und ordnen Sie das entsprechende Makro erneut zu.
    Die geänderten Preise werden auf die markierte Position angewendet und die Beträge werden aktualisiert.

### Makros kopieren

Mit dieser Funktion kopieren Sie alle Makros eines Kunden zu dessen Filialen oder zu einem anderen Kunden. Die Makros stehen nur in eigenständigen Filialen zur Verfügung.

> **Einzelnes Makro kopieren**
> Mit dieser Funktion können Sie nur alle Makros aus der Quelle zum Ziel kopieren. Wenn Sie nur ein einzelnes Makro kopieren möchten, müssen Sie anschließend im Ziel die nicht gewünschten Makros löschen.

#### So kopieren Sie Makros

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
2.  Wählen Sie im Menü Aufbau > Makro > Kopieren.
    Der Dialog Makros kopieren wird geöffnet.

    *   **Abb. C-88: Makro kopieren**
        *   **A**: Kunde (Quelle)
        *   **B**: Ziel-Kunde
        *   **C**: Filiale oder Hauptkonto des (alten) Kunden
        *   **D**: Makros im Ziel aktualisieren
        *   **E**: Nur neue Makros im Ziel behalten
    ⇨ Softwarereferenz, "Makro kopieren" auf Seite C-641

3.  Wählen Sie den Kunden (A) aus, dessen Makros Sie kopieren möchten.
    Die Daten werden eingelesen.
4.  Wählen Sie eine Ziel-Option aus:
    *   **Kunde (B)**: Die Makros werden zu einem anderen Kunden kopiert. Das Feld zur Auswahl des Ziel-Kunden wird freigeschaltet.
    *   **Filialen (C)**: Die Makros werden zu einer oder mehreren Filialen des Kunden kopiert, der als Quelle angegeben ist. In der Anzeige werden alle Filialen des Kunden aufgelistet. Markieren Sie die Checkbox(en) aller Filialen, für die die Makros kopiert werden sollen.
    *   **Hauptktn (C)**: Die Makros werden aus einer Filiale zum Hauptkunden kopiert.
5.  Wählen Sie im Bereich Optionen:
    *   **Vorhandene Makros im Ziel updaten (D)**: Sind beim Ziel-Kunden bereits namensgleiche Makros gespeichert, so werden diese überschrieben. Neue Makros werden hinzugefügt.
    *   **Alle Makros im Ziel zuvor löschen (E)**: Alle Makros des Ziel-Kunden werden gelöscht. Die Makros des Quell-Kunden werden gespeichert.
6.  Klicken Sie auf [OK], um die Makros zu kopieren.
    Alle Makros werden kopiert. Anschließend zeigt eine Meldung an, wie viele Makros kopiert wurden.
7.  Klicken Sie auf [Ende], um den Dialog zu schließen.
    Der Dialog wird geschlossen. Die Positionserfassung wird wieder im Vordergrund angezeigt. Wenn Sie ein Dokument für eine eigenständige Filiale oder für den Ziel-Kunden erfassen, können die neuen Makros ausgewählt werden.

### Makro löschen

Mit dieser Funktion löschen Sie ein allgemeines oder kundenindividuelles Makro.

#### So löschen Sie ein Makro

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
2.  Wählen Sie im Menü Aufbau > Makro > Löschen.
    Der Dialog Makro wird geöffnet. Die Kundennummer und der Name des Kunden werden im Bereich Kunde angezeigt.
3.  Wählen Sie im Bereich Definition die Option und das Makro aus:
    *   **Kundenbezogen**: Nur die kundenbezogenen Makros werden zur Auswahl angeboten.
    *   **Allgemein**: Nur die allgemeinen Makros werden zur Auswahl angeboten.
4.  Wählen Sie das Makro aus, den Sie löschen möchten.
5.  Klicken Sie auf [OK], um das Makro zu löschen.
    Das Makro wird gelöscht und der Dialog wird geschlossen. Die Positionserfassung wird wieder im Vordergrund angezeigt.

### Übungen

**Makro speichern**
Öffnen Sie Ihren Auftrag mit den Positionen, die Sie über die Schnellerfassung eingegeben haben.
*   Speichern Sie die Position 1 als allgemeines Makro.
*   Speichern Sie die Position 2 als kundenspezifisches Makro.

**Position über Makro erfassen**
*   Erfassen Sie in einem anderen Auftrag zwei Positionen mit Hilfe der Makros.
    *   Können Sie das kundenindividuelle Makro verwenden?
    *   Wenn nicht: was müssen Sie ändern?
*   Kopieren Sie das kundenindividuelle Makro so, dass Sie es in allen Aufträgen verwenden können.

**Ergänzende Informationen**
⇨ Softwarereferenz, "Makros" auf Seite C-637

## SN-Datei und Template

### Lernziele

*   Unterschied zwischen Template und SN-Datei kennenlernen.
*   Häufig verwendete Modellmaße als SN-Datei speichern.

### Nutzen

*   Sie können aus Templates (Vorlagen) Standardmodelle für einen Kunden oder einen Großauftrag erstellen.
*   Sie können diese Kundenmodelle, die als Datei mit allen Bearbeitungen und Modifikationen gespeichert sind, schnell erfassen, ohne die Details manuell eingeben zu müssen.

### Merke

*   **SN-Datei**: In einer SN-Datei sind alle Daten des Modells einschließlich der Maße und Bearbeitungen gespeichert.
*   **Template**: Über ein Template können Sie eine (Modell-)Form auf eine Position übertragen. Sie müssen dann Maße und weitere Angaben ergänzen.
*   **Voreinstellungen**: Firmendaten: Register Produktion

### Modell aus eigener Datei oder Vorlage

Sie können aus einer vollständig erfassten Auftragsposition eine SN-Datei für CAD Designer (Shapes) erzeugen. Dabei wird das Modell mit allen Maßen und Bearbeitungen als Datei gespeichert.
In einem Template sind im Gegensatz zur SN-Datei keine festen Werte gespeichert, sondern Variablen, die erst beim Erfassen der Auftragsposition mit Werten gefüllt werden. Im Template wird nur die äußere Form des Modells angeboten.

**Beispiel**
Die Modelle 0, 98 und 99 sind offene Formen (Rechteck), deren Maße in der Auftragsposition festgelegt werden. Diese Maße werden nicht in das Template zurück geschrieben. Dies gilt auch für alle anderen Modelle.

*   **Abb. C-89: Schematische Darstellung eines Modells**
    *   **A**: Modell mit Platzhaltermaßen
    *   **B**: Maße des Modells im Auftrag
    *   **C**: Restriktionen für Maße
    *   **D**: Eingegebene Maße
    *   **E**: Modellnummer

In diesem Beispiel sehen Sie, dass das Modell 2 (E) zunächst ohne Maße angezeigt wird (A). Nachdem die Maße für die Position erfasst (D) sind, wird die Anzeige aktualisiert (B).

Wenn Sie ein Modell immer wieder mit denselben Maßen erfassen müssen, können Sie eine SN-Datei speichern, in der die Maße enthalten sind. Dazu muss die Auftragsposition vollständig erfasst und gespeichert sein.

Beim Speichern der SN-Datei wird ein Unterverzeichnis erstellt, dessen Namen aus den Zahlen des Jahres und des Monats zusammengesetzt ist. Die Datei selbst wird unter einer fortlaufenden Nummer gespeichert, z. B. `C:\Programme\A+W\Sn5\Catalog\sn3\201211\0001169`. Der Name und der Pfad können geändert werden. Sie können beim Speichern nur ein anderes Verzeichnis eintragen, das bereits angelegt ist.

Sie können ein Modell mit allen Maßen und Bearbeitungen aus einer zuvor gespeicherten SN-Datei für andere Aufträge oder Positionen übernehmen.

### Modell 99

Zum Modell 99 und bei importierten SN-Dateien können Bearbeitungen unter folgenden Voraussetzungen erfasst und gespeichert werden.

Dazu müssen folgende Voraussetzungen erfüllt sein:
*   **Firmendaten – Register System**: Checkbox **Kantenbearbeitungen und Bohrungen auf Modell 99** muss aktiviert sein.
*   A+W CAD Designer (Shapes) muss installiert sein.

Auf einer freien Form (Modell 99) können Kantenbearbeitungen nur an allen Kanten zusammen angebracht werden. Die Maße für Bohrungen können nur in Bezug auf das umschriebene Rechteck angegeben werden.
Bei einem Standardmodell aus einer SN-Datei können Kantenbearbeitungen auf einzelnen Kanten erfasst werden, wenn die Kanten in der SN-Datei nummeriert sind.
Die erfassten Bearbeitungen werden in der SN-Datei gespeichert.

> **SN-Daten in der Datenbank speichern**
> Mit dem MS Sql-Server ab Version 2016 werden zusätzlich alle SN-Dateien in der Datenbank gespeichert.
> - Änderungen an einem SN-Template werden rückgängig gemacht, wenn nach der Änderung der Template-Parameter die Position doch nicht gespeichert wird.
> - SN-Dateien müssen nicht kopiert werden. Das Vorhandensein der Datenbank genügt. Eine im Pfad nicht auffindbare SN-Datei wird aus der Datenbank rekonstruiert. Die SN-Datei wird rekonstruiert sobald in der Positionserfassung aus der SN-Datei gelesen wird oder spätestens beim Speichern der Position. Ist die SN-Datei vorhanden, so hat diese weiterhin immer den Vorrang.

### SN-Datei erstellen

In dieser Einheit lernen Sie, wie Sie einen Modellaufbau als SN-Datei speichern und in einem Auftrag wieder verwenden.
Das Verzeichnis, in das die Datei geschrieben werden soll, wird in den **Firmendaten > Register System** festgelegt.

> **Nachträgliche Änderungen der Position**
> Wenn Sie die Position ändern, aus der eine SN-Datei erzeugt wurde, werden die Änderungen beim Speichern auch in die SN-Datei geschrieben.
> Wenn Sie die Position, an die Sie eine SN-Datei angehängt haben, ändern, werden die Änderungen beim Speichern nicht in die SN-Datei geschrieben.

#### So erzeugen Sie eine SN-Datei aus einer Auftragsposition

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument – Positionen" auf Seite C-461
2.  Erfassen Sie das Produkt und geben Sie im Register Modelle/Bearbeitungen alle benötigten Maße ein.
    ⇨ "So erfassen Sie ein Modell" auf Seite C-114
    Erfassen Sie ggf. auch die benötigten Bearbeitungen.
    ⇨ “So erfassen Sie eine Bearbeitung" auf Seite C-119
3.  Markieren Sie die Checkbox **S+N-Datei (A)**.
    Die Ordner-Schaltflächen werden freigeschaltet.

    *   **Abb. C-90: Daten für SN-Datei erfassen**
        *   **A**: Checkbox zum Freischalten der SN-Datei
        *   **B**: Speichern der SN-Datei

4.  Klicken Sie auf die Ordner-Schaltfläche mit dem +-Zeichen (B), um die SN-Datei zu erzeugen.
    Der Name der Datei wird angezeigt. Er kann geändert werden.
5.  Wählen Sie im Menü Start > Speichern, um die Daten zu übernehmen.
    Das Modell wird in der Stückliste als Komponente gespeichert. Wechseln Sie zum Register Position, um weitere Positionen zu erfassen.
6.  Wählen Sie im Menü Start > Speichern, um die Daten zu übernehmen.
    Die Daten der Position werden gespeichert.

### Modell aus SN-Datei in eine Position übernehmen

Sie können das Modell aus einer zuvor erstellten SN-Datei in einen anderen Auftrag übernehmen. Dabei werden alle Maße, Bearbeitungen usw. identisch mit übernommen und können nicht modifiziert werden.

#### So übernehmen Sie eine SN-Datei in eine Auftragsposition

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
2.  Erfassen Sie das Produkt und wechseln Sie zum Register Modelle/Bearbeitungen.
    ⇨ Softwarereferenz, "Positionen – Modelle/Bearbeitungen" auf Seite C-476
3.  Wählen Sie das Modell SN aus oder tragen Sie die Modellnummer 99 ein und springen Sie mit der <Tab>-Taste weiter.
    Die zugehörigen Eingabefelder werden freigeschaltet.

    *   **Abb. C-91: SN-Modell erfassen**
        *   **A**: Modell auswählen
        *   **B**: SN-Template importieren
        *   **C**: SN-Funktion freischalten

4.  Markieren Sie die Checkbox **S+N-Datei** und klicken Sie auf das Ordner-Symbol, um die Datei auszuwählen.
    Der Dialog **Shaping + Nesting - Datei auswählen** wird geöffnet.
5.  Suchen Sie die Datei und übernehmen Sie diese mit [Öffnen].
    Wenn diese Datei zu einem anderen Modell erstellt wurde, müssen Sie die Abfrage mit [Ja] bestätigen.
    Der Dialog wird geschlossen und der Dateiname wird im Feld **S+N-Datei** angezeigt. Die Darstellung und Maße werden in die zugehörigen Felder übernommen.
6.  Passen Sie die Maße so an, wie der Kunde das Modell bestellt hat.
    Die grafische Darstellung wird angepasst.
    Achten Sie darauf, dass die Stücklisten in der SN-Datei und im Auftrag absolut identisch sind. Wenn Sie die Stückliste im Auftrag geändert haben, müssen Sie eine neue SN-Datei schreiben.
    Wenn die Stücklisten der Vorlage und der Position unterschiedlich sind, kann die Position in A+W Production nicht gefertigt werden.
7.  Wählen Sie im Menü Start > Speichern, um die Daten zu übernehmen.
8.  Wechseln Sie zum Register Position.
9.  Wählen Sie im Menü Start > Speichern, um die Position zu speichern.
    Die Daten werden gespeichert.

### Mit Templates arbeiten

Die Namen von Template-Dateien beginnen immer mit T_. Diese Dateien können auch über das Modul Stammdaten erzeugt und bearbeitet werden.
⇨ Stammdaten, "Template Editor" auf Seite B-660

#### So übernehmen Sie ein Template

1.  Wählen Sie Dokumente > Auftrag > Auftrag auswählen > Register Positionen oder <F9>.
    Die Positionserfassung wird geöffnet.
    ⇨ Softwarereferenz, "Dokument - Positionen" auf Seite C-461
2.  Erfassen Sie das Produkt und wechseln Sie zum Register Modelle/Bearbeitungen.
    ⇨ Softwarereferenz, "Positionen – Modelle/Bearbeitungen" auf Seite C-476
3.  Tragen Sie die Modellnummer 99 ein und springen Sie mit der <Tab>-Taste weiter.

    *   **Abb. C-92: SN-Modell erfassen**
        *   **A**: Modell auswählen
        *   **B**: SN-Template importieren
        *   **C**: SN-Funktion freischalten

4.  Markieren Sie die Checkbox **S+N-Datei** und klicken Sie auf das Ordner-symbol, um die Datei auszuwählen.
    Der Dialog **Datei auswählen** wird geöffnet.
5.  Suchen Sie die gewünschte Template-Datei und übernehmen Sie diese mit [Öffnen].
    Die Namen von Template-Dateien sind immer mit T_ gekennzeichnet.
    Die zugehörigen Eingabefelder werden freigeschaltet.

    *   **Abb. C-93: SN-Template verwenden**

6.  Geben Sie die Werte für die Parameter ein.
    Die grafische Darstellung wird entsprechend aktualisiert.
7.  Wählen Sie im Menü Start > Speichern, um die Daten zu übernehmen.
    Die neuen Werte werden nicht in das Template zurückgeschrieben.
    Eine neue SN-Datei wird angelegt. Im Feld **S+N-Datei** wird der neue Dateiname angezeigt.
8.  Wechseln Sie zum Register Position.
9.  Wählen Sie im Menü Start > Speichern, um die Position zu speichern.
    Die Daten werden gespeichert.

### Übungen

**SN-Datei speichern**
*   Öffnen Sie Ihren Auftrag mit den Positionen, die Sie über die Schnellerfassung eingegeben haben.
*   Speichern Sie die Position 1 als SN-Datei.
*   Erfassen Sie eine neue Position, indem Sie die SN-Datei verwenden.

**Modell über Template erfassen**
*   Erfassen Sie eine neue Position, indem Sie eine Vorlage (Template) verwenden.
*   Passen Sie die Vorbelegungen an.
*   Speichern Sie das Modell mit den eingegebenen Maßen als SN-Datei.
*   Erfassen Sie eine neue Position, indem Sie die neue SN-Datei verwenden.
*   Bearbeiten Sie in der neuen Position die Maße.

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, “Positionen – Modelle/Bearbeitungen" auf Seite C-476
*   ⇨ Softwarereferenz, "Positionen – Modell-Template" auf Seite C-502

## Nummernverwalter

### Lernziele

*   Funktion eines Nummernverwalters kennenlernen.
*   Nummernverwalter anlegen und füllen.
*   Dokument in einen Nummernverwalter kopieren.

### Nutzen

*   Sie können den Ablauf bei der Arbeit mit Dokumenten über Nummernverwalter organisieren.
*   Funktionen können Sie für mehrere Dokumente gleichzeitig ausführen, ohne die einzelnen Dokumente zu öffnen.

### Merke

*   **Organisation**: Nummernverwalter sind Organisationseinheiten, in denen Sie mehrere Dokumente sammeln, um diese gemeinsam weiter zu bearbeiten. Aufträge werden z. B. nach Lieferdatum gesammelt, um sie an die Kapazitätsplanung oder an die Produktion zu übergeben.
*   **Nummernverwalter können nicht leer sein**: Sie müssen einem neuen Nummernverwalter mindestens ein Dokument zuordnen. Ohne Dokument kann der Nummernverwalter nicht gespeichert werden.
*   **Nummernverwalter bearbeiten**: Alle Arbeiten mit den Nummernverwaltern ändern die einzelnen Dokumente nicht.
*   **Nummernverwalter in den A+W Business-Modulen**: Der Dialog Nummernverwalter ist für alle Dokumente gleich.
*   **Dokumente sammeln**: Funktionen für Dokumente mit identischem Status können über Nummernverwalter ausgelöst werden, z. B. der Druck von Lieferscheinen.
*   **Voreinstellungen**: Keine

### Organisation der Dokumente

Jedes Dokument wird automatisch einem Nummernverwalter zugeordnet. Sie können unterschiedliche Nummernverwalter anlegen und z. B. bestimmten Mitarbeitern oder Arbeitsbereichen zuordnen, z. B. Auftragserfassung, Produktion, Lieferung usw. Mit den Nummernverwaltern können Sie Arbeitsabläufe im Verkauf automatisieren, z. B. Bestellaufträge erstellen oder Lieferscheine drucken.

*   **Abb. C-94: Nummernverwalter**
    *   **A**: Aktueller Nummernverwalter (NV)
    *   **B**: Mitarbeiter, dem der NV zugeordnet ist
    *   **C**: Liste der Nummernverwalter
    *   **D**: Einstellung der Sortierung
    *   **E**: Dokumente im aktuellen NV

Sie können die Arbeit mit den Nummernverwaltern so organisieren, dass Sie die Dokumente in unterschiedlichen Nummernverwaltern (C) sammeln. Die Nummernverwalter können dann in anderen Dialogen ausgewählt und die Weiterverarbeitung der Dokumente gestartet werden.
Nummernverwalter werden personengebunden angelegt und genutzt, d. h., dass jeder Mitarbeiter (B) mit seinen eigenen Nummernverwaltern arbeitet. Wenn ein Nummernverwalter von mehreren Kollegen gemeinsam genutzt werden soll, kann er für jeden einzelnen kopiert werden.
Haben Sie z. B. in einem Nummernverwalter alle Dokumente zusammengefasst, die am aktuellen Tag (heute) erfasst oder geändert wurden, so können Sie diesen Nummernverwalter im Formulardruck öffnen und den Druck der Auftragsbestätigungen für alle Dokumente gemeinsam starten.

Mit Nummernverwaltern arbeiten Sie z. B. bei folgenden Vorgängen:
*   Druck, z. B. Auftragsbestätigungen (AB), Lieferscheine, Rechnungen
*   Datenübergabe, z. B. FiBu, Bestellung, Produktion
*   Journale
*   Archivierung
*   Import von Aufträgen (EDI)
*   Bankbelege drucken
*   Bestandslisten erstellen
*   Dokumentendaten prüfen, z. B. Terminkontrolle

Ausschlaggebend für die Verarbeitung der Dokumente ist in der Regel der (gemeinsame) Status. Dokumente, die sich irrtümlich in einem Nummernverwalter befinden, werden daher nicht mit verarbeitet.
Sie können Dokumente auch in einem Nummernverwalter zusammenfassen, um in ihnen gemeinsam den Status oder das Bestellkennzeichen zu ändern.
Nummernverwalter können gelöscht werden. Die Dokumente in einem Nummernverwalter werden dabei nicht gelöscht.

### Nummernverwalter erstellen

Der Dialog Nummernverwalter ist für alle Dokumente gleich. Er wird in dieser Anleitung am Beispiel Auftrag beschrieben.
In dieser Einheit lernen Sie, wie Sie mit Nummernverwaltern arbeiten.

#### So erstellen Sie einen neuen Nummernverwalter

1.  Wählen Sie Dokumente > Auftrag > NV Auftrag.
    Der Dialog Nummernverwalter wird geöffnet.
    ⇨ Softwarereferenz, "Nummernverwalter" auf Seite C-645
2.  Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wechseln.

    *   **Abb. C-95: Felder für neuen Nummernverwalter freigeschaltet**
        *   **A**: Name des NV
        *   **B**: Kriterien zur Auswahl der Dokumente

3.  Tragen Sie einen Namen (A) für den neuen Nummernverwalter ein.
4.  Ordnen Sie dem neuen Nummernverwalter mindestens ein Dokument zu.
    Sie haben die Möglichkeit, einen einzelnen Auftrag oder eine Reihe von Aufträgen auszuwählen, indem Sie in den Feldern Auftrag und/oder Statusbereich (B) die entsprechenden Daten eingeben.
    Sie können über die Suche die Aufträge auch nach selbst gewählten Kriterien auswählen, z. B. nach Kunden.
    In diesem Beispiel werden die Aufträge nach Status gesammelt.
5.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Dokumente werden eingelesen. Der neue Nummernverwalter wird im Feld Auswahl aufgelistet. Die Daten werden gespeichert.

    *   **Abb. C-96: Neuer Nummernverwalter**

6.  Sie können Aufträge aus der Übersicht aus dem Nummernverwalter löschen. Dabei werden nicht die Aufträge gelöscht, sondern nur die Zuweisung zum Nummernverwalter. Markieren Sie den Auftrag, die Sie entfernen wollen, und drücken Sie auf <Entf>.

    *   **Abb. C-97: Aufträge entfernen**
    Der Auftrag wird aus der Liste entfernt. Die verbleibenden Aufträge werden mit einem Häkchen gekennzeichnet. Wiederholen Sie diesen Schritt, bis nur noch die gewünschten Aufträge angezeigt werden.

7.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Der Nummernverwalter wird mit der aktuellen Liste der Aufträge gespeichert.

### Nummernverwalter kopieren

Sie können einen Nummernverwalter vollständig kopieren, z. B., um ihn einem anderen Mitarbeiter zuzuweisen.

#### So kopieren Sie einen Nummernverwalter

1.  Wählen Sie Dokumente > Auftrag > NV Auftrag.
    Der Dialog Nummernverwalter wird geöffnet.
    ⇨ Softwarereferenz, "Nummernverwalter" auf Seite C-645
2.  Wählen Sie im Menü Funktionen > Gruppe Bearbeiten > Kopieren nach.

    *   **Abb. C-98: Nummernverwalter kopieren**

3.  Wählen Sie in den Bereichen **Quelle** und **Ziel**:
    *   Den Mitarbeiter, wenn der Nummernverwalter einem bestimmten Mitarbeiter zugewiesen ist oder werden soll.
    *   Den Nummernverwalter, den Sie kopieren wollen.
4.  Tragen Sie im Bereich Ziel im Feld Nummernverwalter den Namen für den neuen Nummernverwalter ein.
5.  Klicken Sie auf [OK], um die Daten zu speichern.
    Die Daten werden gespeichert.
6.  Klicken Sie auf [Ende], um den Dialog zu schließen.
    Der Dialog Nummernverwalter kopieren wird geschlossen. Der neue Nummernverwalter wird im Dialog Nummernverwalter des entsprechenden Mitarbeiters im Feld Auswahl aufgelistet.

### Nummernverwalter leeren

Wenn alle Dokumente in einem Nummernverwalter abgearbeitet sind, können Sie den Nummernverwalter leeren, um anschließend darin neue Dokumente zu sammeln.

#### So leeren Sie einen Nummernverwalter

1.  Wählen Sie Dokumente > Auftrag > NV Auftrag.
    Der Dialog Nummernverwalter wird geöffnet.
    ⇨ Softwarereferenz, "Nummernverwalter" auf Seite C-645
2.  Markieren Sie den Nummernverwalter, den Sie leeren wollen.
3.  Wählen Sie im Menü Funktionen > Gruppe Bearbeiten > Überschreiben.

    *   **Abb. C-99: Nummernverwalter leeren**

    Die Liste der Dokumente wird gelöscht.
4.  Tragen Sie im Feld Auftrag oder im Feld Statusbereich die Daten für die Zuordnung von Aufträgen ein.
    Sie müssen mindestens einen Auftrag zuordnen, damit der Nummernverwalter gespeichert werden kann.
5.  Wechseln Sie zum Menü Start.
6.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    In der Übersicht werden die zugeordneten Aufträge aufgelistet.

### Dokument in einen Nummernverwalter stellen

Sie können ein einzelnes Dokument in einen anderen Nummernverwalter stellen.

#### So stellen Sie Dokumente in einen anderen Nummernverwalter

1.  Wählen Sie Dokumente > Auftrag > NV Auftrag.
    Der Dialog Nummernverwalter wird geöffnet.
    ⇨ Softwarereferenz, "Nummernverwalter" auf Seite C-645
2.  Wählen Sie im Bereich Auswahl den Ziel-Nummernverwalter aus.
    In der Übersicht werden alle Dokumente angezeigt, die sich in diesem Nummernverwalter befinden.
3.  Tragen Sie in den Feldern Auftrag von/bis die Auftragsnummern ein, die verschoben werden sollen.
4.  Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
    Die Dokumente werden in der Liste aufgeführt. Löschen Sie diese Dokumente ggf. aus dem Nummernverwalter, in dem sie sich zuvor befanden.

### Übungen

**Nummernverwalter erstellen**
Erstellen Sie einen neuen Nummernverwalter mit folgenden Dokumenten:
*   Aufträge von Nummer n bis nn.
*   Wählen Sie für n die Nummer des ersten Auftrags, den Sie angelegt haben.
*   Wählen Sie für nn eine beliebige höhere Nummer.
*   Status 1 bis 2.

**Nummernverwalter leeren**
*   Öffnen Sie einen Nummernverwalter und leeren Sie ihn, indem Sie Aufträge mit dem Status 30 einfügen.

**Ergänzende Informationen**
*   ⇨ Softwarereferenz, "Statusänderung" auf Seite C-566
*   ⇨ Softwarereferenz, "Nummernverwalter" auf Seite C-645
*   ⇨ Softwarereferenz, "Bestellkennzeichen ändern" auf Seite C-650

## Druck

### Lernziele

*   Einstellungen für Skizzendruck kennenlernen.
*   Einstellungen für Preisdruck kennenlernen.
*   Auftragsbestätigungen, Lieferscheine, Rechnungen und Etiketten drucken.

### Nutzen

*   Über das Layout von gedruckten Dokumenten müssen Sie sich keine Gedanken machen, da diese in hinterlegten Formularen gedruckt werden.
*   Preise und Skizzen können im Druck unterschiedlich dargestellt werden. Dazu lernen Sie die spezifischen Einstellungen kennen.

### Merke

*   **Ausgabe**: Jedes Dokument kann entweder auf dem Bildschirm ausgegeben oder an einen Drucker gesendet werden. Beide Druckmodi setzen den Status um.
*   **Formular**: Dokumente können nur gedruckt werden, wenn die zugehörigen Formulare im System hinterlegt sind.
*   **Bildschirmdruck**: Im Bildschirmdruck wird jeweils nur ein Dokument gedruckt. Nach dem Bildschirmdruck kann ein Dokument nur im Wiederholungsdruck an den Drucker gesendet werden.
*   **Druckpunkt**: Der Druckpunkt entspricht dem Statuspunkt, der programmintern genutzt wird, um ein bestimmtes Formular zu drucken.
*   **Voreinstellungen**:
    *   **Stammdaten**:
        *   Statuszuordnung
        *   Formularverwaltung
        *   Druckaufträge
    *   **Firmendaten**:
        *   Register Druck (Skizzendruck)
        *   Register Archiv

### Formular- und Etikettendruck

Für den Druck von Dokumenten werden in A+W Business Standardformulare genutzt. Die Dokumente können an einen Drucker gesendet oder als PDF-Datei auf dem Bildschirm angezeigt werden. Beide Ausgabeformen gelten als Druck.

*   **Abb. C-100: Druck von Aufträgen**
    *   **A**: Formular, auf das gedruckt wird
    *   **B**: Nummernverwalter, aus dem gedruckt wird
    *   **C**: Druckmodus
    *   **D**: Optionen für die Ausgabe des Drucks
    *   **E**: Sonderdruck

Über den Druckmodus (C) legen Sie fest, was gedruckt werden soll, z. B. ein Lieferschein. Beachten Sie dabei, dass der Status den Druck einschränken kann. So kann z. B. vorgegeben sein, dass eine Rechnung erst nach dem Lieferschein gedruckt werden darf.

Die Formulare (A) werden in der Formularverwaltung den einzelnen Druckpunkten zugeordnet. Damit stehen sie für den Druck zum Auswählen (A) zur Verfügung. Wenn einem Druckpunkt mehrere Formulare zugeordnet sind, muss eines als Standard festgelegt sein.

Formulare werden für die unterschiedlichen Ausgabeformate hinterlegt, z. B. Auftragsbestätigungen (AB) per (Papier-) Druck, E-Mail, PDF. Das Formular selbst kann auch die Ausgabe steuern: Wenn Sie ein Dokument z. B. über den maxxPDFMailer drucken, wird es automatisch per E-Mail gesendet. Ohne diesen PDFMailer müssen Sie den Versand manuell aktivieren.
⇨ Softwarereferenz, "Formular-/Etikettendruck - Formulare" auf Seite C-656

> **Kundenindividuelle Formulare**
> In Absprache mit der A+W Software GmbH können weitere Formulare zur Verfügung gestellt werden.
> Wenn Sie in A+W Business die Mehrsprachigkeit nutzen, werden Formulare standardmäßig in der Sprache des Kunden gedruckt. Diese Einstellung kann übersteuert werden, z. B. für Fertigungspapiere in Ihrer Landessprache.
> Für jedes Formular können Sie einen eigenen Text verfassen, der standardmäßig mit der E-Mail verschickt wird. Die PDF-Ausgabe erfolgt über den Standard-Formulardruck in A+W Business.

### Druckmodus im Nummernverwalter

Den Druck selbst steuern Sie aus den Dokumenten oder Nummernverwaltern heraus. Dabei entscheiden Sie, welches Formular und welches Ausgabeformat verwendet wird. Zu dem Druckauftrag legen Sie auch die Versandform fest, z. B. per Fax oder E-Mail.

Mit der Wahl des Druckmodus wird automatisch das zugehörige Standard-Formular ausgewählt. Folgende Druckmodi stehen zur Verfügung:
*   Auftragsbestätigung (Auftrag)
*   Fertigungsschein
*   Lieferschein
*   Rechnung
*   Sonstige

Nach dem Druck einer Rechnung wird das Dokument in der Regel gesperrt. Es kann dann nicht mehr bearbeitet werden.
⇨ Stammdaten, "Dokumente sperren nach Rechnungsdruck" auf Seite B-953

*   **Abb. C-101: Formulare für Wiederholungsdruck**
    *   **A**: Formularauswahl für Wiederholungsdruck
    *   **B**: Einstellung Wiederholungsdruck

Standardmäßig wird beim Druck eines Dokuments der Status hochgesetzt. Soll ein Dokument erneut gedruckt werden, muss der Druckpunkt für den **Wiederholungsdruck (B)** ausgewählt werden. Dadurch werden die möglichen Formulare (A) zur Auswahl angeboten.

> **Erstdruck kann nur einmal gestartet werden**
> Sie können ein Dokument nur einmal auf einem (Original-) Formular drucken. Wenn es erneut gedruckt werden soll, müssen Sie einen Wiederholungsdruck starten. Dabei spielt es keine Rolle, ob der Erstdruck auf dem Drucker oder auf dem Bildschirm ausgegeben wurde.
> Nur wenn Sie ein Dokument in der Dokumentenansicht geöffnet haben und drucken, wird der Status nicht hochgesetzt. Das Dokument wird in diesem Fall jedoch nicht als Formular gedruckt.

Üblicherweise wird der Druck aus einem Nummernverwalter heraus gestartet. Die Dokumente werden vor dem Druckbeginn gesperrt. Falls eine Sperre nicht ausgeführt werden kann, können Sie entscheiden, ob der Druck dennoch begonnen wird. Kann ein Dokument wegen eines mangelhaften Status nicht gedruckt werden, wird dies vor Druckbeginn angezeigt.
Die Anzahl der nicht verarbeiteten Dokumente wird in einer Meldung angezeigt. Die nicht gedruckten Dokumente werden in der Übersicht im Zeilenkopf markiert. Sie müssen bearbeitet werden, damit sie gedruckt werden können.

### Rechnungsdruck

Der Auftrag erhält mit dem Rechnungsdruck eine Rechnungsnummer. Dabei ist es unerheblich, ob die Druckfunktion auf den Drucker geleitet wurde oder eine PDF-Datei (Bildschirmausgabe) erstellt wurde.

Die Rechnungs- und die Anlieferpauschale werden vor dem Druckbeginn in die Dokumente eingefügt. Bei Sammelrechnungen wird vor dem Druckbeginn die Steuerkorrektur ausgeführt.

Bei Teillieferungen mit Teilfakturierung und bei Anzahlungen wird die Abschlussrechnung aus dem Original-Auftrag gedruckt. Dabei wird nach dem Druck der einzelnen Positionen die Auftragssumme gebildet, die aus dem Nettobetrag, der MwSt. und dem Bruttobetrag besteht. Danach werden alle erstellten Anzahlungsrechnungen und Teilrechnungen mit ihren Einzelbeträgen (Nettobeträgen, der jeweiligen MwSt. und dem Bruttobetrag) und schließlich die verbleibende Rechnungsendsumme gedruckt.

Anhand der Rechnungsnummer kann geprüft werden, ob für das Dokument bereits eine Rechnung erstellt wurde. Dokumente mit einer Rechnungsnummer können für die Bearbeitung gesperrt werden. Das Dokument kann auch dann nicht mehr bearbeitet werden, wenn der Status geändert wird.
⇨ Stammdaten, "Dokumente sperren nach Rechnungsdruck" auf Seite B-953

> **Rechnung schützen**
> PDF-Dokumente können mit einer digitalen Signatur oder mit Sicherheitsoptionen gespeichert werden. So können z. B. PDF-Dokumente durch ein Kennwort für Bearbeitungen gesperrt werden. Dies ist beim Versand von Rechnungen ein wichtiges Kriterium.
