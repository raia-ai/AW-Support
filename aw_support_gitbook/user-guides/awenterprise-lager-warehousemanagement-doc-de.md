---
title: "DE_AWEnterprise_Lager_1.01"
source: "DE_AWEnterprise_Lager_1.01.pdf"
tags: ["A+W Enterprise", "Lager", "Warehouse Management", "Inventory", "ERP", "Glass Software", "Window Software", "Door Software", "Technical Manual", "Software Reference"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is the software reference manual for the A+W Enterprise 'Lager' (Warehouse) module, version 1.01. It provides a comprehensive guide for end-users on managing warehouse operations, including goods receipt, goods issue, inventory management, stock valuation, and system administration."
long_description: "This is the detailed software reference guide for the 'Lager' (Warehouse) module of the A+W Enterprise ERP system, specifically for version 1.01 dated January 2017. The document is intended for end-users and provides an exhaustive overview of all functions related to warehouse management for glass, windows, and doors. It covers core processes such as goods receipt (`Lagereingang`), goods issue (`Lagerausgang`), and various specialized storage types like crate (`Kistenlager`), bin (`Fachlager`), stack (`Stapellager`), and rack (`Gestelllager`) management. The manual details the procedures for performing inventory (`Inventur`) and stock valuation (`Bestandsbewertung`) across these different storage types. It also explains the use of the extensive information system (`Infosystem`) for searching and reporting on articles, variants, stock levels, and historical data. Furthermore, it outlines system administration tasks, printing functions, and service utilities. The guide uses screenshots and step-by-step descriptions to explain the user interface, dialogs, and menu structures, making it an essential resource for operating the A+W warehouse module effectively."
---

# A+W Lager
**A+W Enterprise**

*A+W - Software for Glass, Windows and Doors*

---
## Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part | Version / Datum | Beschreibung |
| :--- | :--- | :--- |
| | 1.00 / 12-2015 | Ersterstellung |
| | 1.01 / 01-2017 | Produkt- und Firmennamen angepasst. |

### Editorial

Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen
- Kontakte

#### Anmerkungen zu diesem Dokument

Diese Veröffentlichung ist ausschließlich für Endanwender von **A+W Enterprise** gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.

Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von A+W Enterprise.

#### Urheberrechte

© 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

#### Warenzeichen

Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

#### Kontakte

**A+W Software GmbH**

Am Pfahlgraben 4-10
35415 Pohlheim
- **Tel:** +49 6404 2051-0
- **Fax:** +49 6404 2051 877
- **Email:** Zentrale@a-w.com
- **Web:** http://www.a-w.com

## Softwarereferenz

### Übersicht

Im Modul **Lager** verfügen Sie über alle Funktionen, die zur erfolgreichen Lagerverwaltung erforderlich sind, z. B. Bestandsführungen, Bestandsbuchungen, Inventuren sowie die Planungen der Artikelzugänge und Artikelabgänge. In diesem Modul werden alle Preise als Nettopreise angegeben.

Im Part Lager finden Sie folgende Themen:
- "Lagerverwaltung" auf Seite E-15
- "Stammdatenverwaltung" auf Seite E-50
- "Inventurverwaltung" auf Seite E-53
- "Bewertung" auf Seite E-63
- "Informationssystem" auf Seite E-70
- "Druck" auf Seite E-112
- "Systemverwaltung" auf Seite E-114
- "Servicefunktionen" auf Seite E-116

### Menüs im Modul Lager

Über folgende Menüs öffnen Sie die Dialoge des Moduls Lager:
- "Menü Buchung" auf Seite E-9
- "Menü Stammdaten" auf Seite E-10
- "Menü Inventur" auf Seite E-10
- "Menü Bewertung" auf Seite E-11
- "Menü Infosystem" auf Seite E-11
- "Menü Druck" auf Seite E-12
- "Menü System" auf Seite E-12

#### Menü Buchung

Im Menü Buchung finden Sie auf der ersten Ebene folgende Einträge:

- **Eingang:**
  - "Lagereingang" auf Seite E-16
- **Ausgang:**
  - "Lagerausgang" auf Seite E-22
- **Kisteneingang:**
  - "Kistenlagereingang" auf Seite E-23
- **Kistenausgang:**
  - "Kistenlagerausgang" auf Seite E-28
- **Facheingang:**
  - "Fachlagereingang" auf Seite E-29
- **Fachausgang:**
  - "Fachlagerausgang" auf Seite E-34
- **Stapelverwaltung:**
  - Kundenspezifische Funktion, wird ausführlich in einem separaten Part erklärt.
- **Stapeleingang:**
  - "Stapellagereingang" auf Seite E-35
- **Stapeländerung:**
  - "Stapellageränderung" auf Seite E-36
- **Gestelleingang:**
  - "Gestelllagereingang" auf Seite E-38
- **Gestellausgang:**
  - "Gestelllagerausgang" auf Seite E-41
- **Stapelbuchung (Vorgangsbez.):**
  - Kundenspezifische Funktion, wird ausführlich in einem separaten Part erklärt.
- **Ausgang (Auftragsbezogen):**
  - "Lagerausgang (Auftragsbezogen)" auf Seite E-45
- **Korrektur:**
  - "Buchungskorrektur – Übersicht" auf Seite E-47

#### Menü Stammdaten

Im Menü Stammdaten finden Sie folgende Einträge:
- **Raum:**
  - "Lagerraumverwaltung" auf Seite E-50
- **Artikel:**
  - "Artikelstammdaten Lager" auf Seite E-51
- **Fächer:**
  - Kundenspezifische Funktion, wird ausführlich in einem separaten Part erklärt.
- **Stapeltypen:**
  - Kundenspezifische Funktion, wird ausführlich in einem separaten Part erklärt.

#### Menü Inventur

Im Menü Inventur finden Sie folgende Einträge:
- **Lager:**
  - "Inventur - Standardlager" auf Seite E-53
- **Kistenlager:**
  - "Inventur - Kistenlager" auf Seite E-56
- **Fachlager:**
  - "Inventur - Fachlager" auf Seite E-58
- **Stapellager:**
  - "Inventur - Stapellager" auf Seite E-59
- **Gestelllager:**
  - "Inventur - Gestelllager" auf Seite E-60

#### Menü Bewertung

Im Menü Bewertung finden Sie folgende Einträge:
- **Lager:**
  - "Bestandsbewertung - Standardlager" auf Seite E-63
- **Kistenlager:**
  - "Bestandsbewertung - Kistenlager" auf Seite E-66
- **Fachlager:**
  - "Bestandsbewertung - Fachlager" auf Seite E-67
- **Stapellager:**
  - "Bestandsbewertung - Stapellager" auf Seite E-68
- **Gestelllager:**
  - "Bestandsbewertung - Gestelllager" auf Seite E-69

#### Menü Infosystem

Im Menü Infosystem finden Sie auf der ersten Ebene folgende Einträge:
- **Artikel:**
  - "Info-Lager-Artikel - Filterdialog" auf Seite E-71
- **Variante:**
  - "Info-Lager-Varianten - Filterdialog" auf Seite E-75
- **Fach:**
  - "Info-Lager-Fächer" auf Seite E-79
- **Gestell:**
  - "Info-Lager-Gestelle - Filterdialog" auf Seite E-82
- **Stapel:**
  - "Info-Lager-Stapel - Filterdialog" auf Seite E-85
- **Blatt:**
  - "Info-Lager-Blätter - Filterdialog" auf Seite E-88
- **Historie:**
  - "Info-Lager-Historie - Filterdialog" auf Seite E-91
- **Aufträge/Bestellungen:**
  - "Aufträge/Bestellungen - Filterdialog" auf Seite E-96
- **Buchungsstatus:**
  - "Menü 2. Ebene - Buchungsstatus" auf Seite E-12
- **Auftragsliste:**
  - "Lagerinformationen - Pickliste" auf Seite E-105
- **LVR-Status:**
  - Dieser Dialog wird zur Zeit nicht genutzt.
- **Reichweite:**
  - "Reichweite - Bestandsprognose" auf Seite E-107
- **Dispositiver Bestand:**
  - "Dispositiver Bestand" auf Seite E-109
- **Prognose:**
  - "Bestandsprognose" auf Seite E-110

##### Menü 2. Ebene – Buchungsstatus
- **Ungebucht:**
  - "Buchungsstatus - Ungebucht" auf Seite E-100
- **Fehler:**
  - "Buchungsstatus – Fehler" auf Seite E-102
- **Inventur:**
  - "Buchungsstatus - Inventur" auf Seite E-103

#### Menü Druck

Im Menü Druck finden Sie folgende Einträge:
- **Etiketten:**
  - "Kistenetiketten drucken" auf Seite E-112
- **Listendruck:**
  - Der Dialog wird im Part Verkauf beschrieben.
  - Verkauf, "Listendruck" auf Seite D-162

#### Menü System

Im Menü System finden Sie folgende Einträge:
- **Lagerprotokoll löschen:**
  - "Lagerprotokoll löschen" auf Seite E-114
- **Preiskorrektur:**
  - "Lager-Preiskorrektur" auf Seite E-114

#### Zusatzmenü (<F4>)

Im Zusatzmenü finden Sie folgende Einträge:

##### Menü 1. Ebene
- **PKZ-Preise:** In den Lagereingängen können Sie Artikeln vordefinierte Preise über Preiskennzeichen zuweisen. Die Preiskennzeichen können Sie aus einer vordefinierten Liste auswählen.
- **Nullpreisbuchung:** In den Lagereingängen können Sie Artikel den Preis = 0 zuweisen.
- **Umbuchen:** Ausgewählten Datensatz in ein anderes Lager umbuchen. Die Buchung muss mit [OK] abgeschlossen werden.
- **Objektbuchung:** Ausgewählten Datensatz einem Objekt (z. B. Baustelle) zuweisen.
- **Kisten:**
  - "Menü 2. Ebene - Kisten" auf Seite E-13

##### Menü 2. Ebene - Kisten
- **Kiste abbuchen:** Entfernt die Kiste des aktuellen Datensatzes aus dem Kistenlager und bucht die Artikel der Kiste automatisch in das Normallager. Die Buchung muss mit [OK] abgeschlossen werden.
- **Kiste auflösen:** Entfernt die Kiste des aktuellen Datensatzes aus dem Kistenlager und bucht die Artikel in ein Ziellager. Die Buchung muss mit [OK] abgeschlossen werden.
- **Einzelblattinformation:**
  - "Menü 3. Ebene - Einzelblattinformationen" auf Seite E-13

##### Menü 3. Ebene - Einzelblattinformationen
- **Anzeige:**
  - "Fußbereich - Einzelblattinformationen" auf Seite E-25
- **Editieren:**
  - "Fußbereich - Einzelblattinformationen" auf Seite E-25

### Suchfunktionen

Informationen können Sie über die Suchfunktionen des Informationssystems suchen, z. B. zu Artikeln, Lagerarten, Aufträgen oder Bestellungen.
- "Informationssystem" auf Seite E-70

## Lagerverwaltung

In der Lagerverwaltung erfassen und bearbeiten Sie die Buchungen für das Warenlager, z. B. Lagereingänge für Artikel oder Buchungskorrekturen.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Lagereingang" auf Seite E-16
- "Lagerausgang" auf Seite E-22
- "Kistenlagereingang" auf Seite E-23
- "Kistenlagerausgang" auf Seite E-28
- "Fachlagereingang" auf Seite E-29
- "Fachlagerausgang" auf Seite E-34
- "Stapellagereingang" auf Seite E-35
- "Stapellageränderung" auf Seite E-36
- "Gestelllagereingang" auf Seite E-38
- "Gestelllagerausgang" auf Seite E-41
- "Lagerausgang (Auftragsbezogen)" auf Seite E-45
- "Buchungskorrektur – Übersicht" auf Seite E-47
- "Buchungskorrektur - Details" auf Seite E-48

### Lagereingang
**Buchung > Eingang**

In diesem Dialog erfassen und buchen Sie die Lagereingänge für die Lagerartikel des ausgewählten Lagers.

In diesem Dialog finden Sie folgende Register:
- "Lagereingang – Stück" auf Seite E-16
- "Lagereingang - Menge" auf Seite E-20

#### Lagereingang – Stück
**Buchung > Eingang > Stück**

*Abb. E-1: Lagereingang – Stück*

In diesem Register erfassen und buchen Sie die Lagereingänge in den Stückzahlen der aktuellen Artikelvariante. Sie können in ein anderes Lager wechseln, indem Sie eine andere Lagernummer eingeben. Das gilt auch für Lager eines anderen Lagertyps.

Die Lagereingänge für Kisten, Fächer, Stapel und Gestelle buchen Sie an folgender Stelle:
- "Kistenlagereingang" auf Seite E-23
- "Fachlagereingang" auf Seite E-29
- "Stapellagereingang" auf Seite E-35
- "Gestelllagereingang" auf Seite E-38

Sie können folgende Tastaturbefehle ausführen:
- Mit `<Strg>` + `<F8>` können Sie im ersten Feld zwischen dem Dialog Lagereingang und Lagerausgang wechseln.
- Mit `<F5>` können Sie aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Pos1>` verwerfen Sie Ihre Eingabe im Fußbereich.
- Mit `<Ende>` können Sie im Fußbereich Ihre Eingabe speichern und in den Rumpfbereich wechseln.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.

##### Kopfbereich
- **Artikel:** Artikelnummer und Artikelbezeichnung.
- **Lager:** Lagernummer und Lagerbezeichnung.
- **Lieferant:** Lieferantennummer und Lieferantenname.
- **Gesamtbestand:** Gesamtbestand des Artikels, einschließlich aller Artikelvarianten.
- **Gesamtwert:** Gesamtbetrag des Lagerartikels.
- **Buchungsstatus:** Status der Buchungen im Lager.

| Buchungsstatus mit Farbkennzeichen | Bedeutung |
| :--- | :--- |
| grau | Im Lagereingang sind alle Buchungspositionen vom Prozess (Programm) gebucht worden. |
| rot | Im Lagereingang ist mindestens eine Buchungsposition vom Prozess (Programm) nicht oder noch nicht gebucht worden. |
*Tab. E-1: Buchungsstatus des Lagers*

- **Letzte Änderung am, von:** Datum der letzten Änderung am Buchungssatz und Name des Anwenders, der die letzte Buchung ausgeführt hat.

##### Rumpfbereich
In diesem Bereich buchen Sie die Bestände und Preise der Artikelvariante in Stückzahlen.

- **Variante:** Maßvariante des Artikels. Mit `<F9>` können Sie die Variantenauswahl aufrufen. Dabei werden nur die Varianten angezeigt, die dem aktuellen Artikel in den Stammdaten zugewiesen sind.
- **Lagerbez.:** Lagerbezeichnung.
- **Bestände (Stück):** Lagerbestand der Variante in Stückzahlen.
  - **Alt:** Alter Artikelbestand im Lager, bevor gebucht wird.
  - **Buchung:** Artikelbestand, der gebucht wird.
  - **Neu:** Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn der neue Artikel gebucht wird. Wenn Sie den Dialog mit `<Pos1>` verlassen, wird der alte Lagerbestand beibehalten.
- **Preise:** Die Anzeige der Währung richtet sich nach der Eigenwährung, die bei der Installation festgelegt wurde.
  - **€/qm:** Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
  - **Preis:** Gesamtpreis des Artikels.
  - **(Spalte ohne Bezeichnung):** Buchungsstatus der Artikelposition.

| Buchungsstatus mit Farbkennzeichen | Bedeutung |
| :--- | :--- |
| grau | Artikelposition ist vom Prozess (Programm) gebucht worden. |
| rot | Artikelposition ist vom Prozess (Programm) nicht oder noch nicht gebucht worden. |
*Tab. E-2: Buchungsstatus der Artikelposition*

##### Fußbereich – Variantenbezogene Angaben
- **Objekt:** Bezeichnung des Objekts bei auftragsbezogenen Lagerartikeln, z. B. Baustelle des Kunden.
- **Kostenstelle:** Bezeichnung der Kostenstelle für statistische Auswertungen.
- **Bemerkung:** Textfeld für zusätzliche Informationen.
- **Mindestbestand:** Minimal zulässiger Lagerbestand des Artikels, um Produktionsengpässe zu verhindern.
- **Alarmbestand:** Stückzahl des Artikelbestands, die einen Bestellvorschlag im Einkauf anlegt. Durch Alarmbestände können Sie eine Unterdeckung des Lagers verhindern.
- **Maximalbestand:** Maximal zulässiger Lagerbestand des Artikels, um Lagerkosten zu minimieren.

> **Automatische Bestellvorschläge durch das Lager**
> Wenn der definierte Alarmbestand bei einer Ausgangsbuchung unterschritten wird, werden durch das Lager automatisch Bestellvorschläge im Einkauf angelegt. Automatische Bestellvorschläge werden auch durch die nächtliche Buchungsroutine im Einkauf angelegt, wenn der Artikelbestand langfristig unter den Mindestbestand fällt. Die Menge im Bestellvorschlag richtet sich nach dem definierten Maximalbestand. Diese Bestellvorschläge werden vom Einkauf freigeschaltet und in Bestellungen überführt.

- **Gesamtpreis:** Gesamtpreis der Artikelvariante.
- **Durchschnittspreis:** Durchschnittlicher Einkaufspreis der Artikelvariante im Lager.
- **Höchstpreis:** Höchster Einkaufspreis der Artikelvariante im Lager.
- **Niedrigstpreis:** Niedrigster Einkaufspreis der Artikelvariante im Lager.
- **LIFO-Gesamtpreis:** Gesamtpreis der Artikelvariante im Lager, wenn die zuletzt eingelagerten Lagerartikel als erste Artikel ausgelagert werden.
- **FIFO-Gesamtpreis:** Gesamtpreis der Artikelvariante im Lager, wenn die zuerst eingelagerten Lagerartikel als erste Artikel ausgelagert werden.

**Beispiel:**
1. Lagereingang 10 Stück zu 10,- € = 100,- €
2. Lagereingang 10 Stück zu 15,- € = 150,- €
Gesamtwert beider Lagereingänge = 250,- €
Lagerabgang 10 Stück nach LIFO = -150,- €
LIFO-Gesamtpreis = 100,- €
Lagerabgang 10 Stück nach FIFO = -100,- €
FIFO-Gesamtpreis = 150,- €

#### Lagereingang – Menge
**Buchung > Eingang > Menge**

*Abb. E-2: Lagereingang – Menge*

In diesem Register erfassen und buchen Sie die Lagereingänge in den Mengeneinheiten der aktuellen Artikelvariante.
Das Register Menge ist wie das Register Stück aufgebaut.
- "Kopfbereich" auf Seite E-17
- "Fußbereich – Variantenbezogene Angaben" auf Seite E-18

##### Rumpfbereich
In diesem Bereich buchen Sie die Bestände und Preise der Artikelvariante in Mengeneinheiten.
- **Variante:** Maßvariante des Artikels. Mit `<F9>` können Sie die Variantenauswahl aufrufen. Dabei werden nur die Varianten angezeigt, die dem aktuellen Artikel in den Stammdaten zugewiesen sind.
- **Farbe:** Farbe der Maßvariante des Artikels.
- **Bestände (Mengeneinheit):** Lagerbestand der Variante in den Mengen, die für diese Artikelvariante in den Stammdaten definiert ist.
  - **Alt:** Alter Artikelbestand im Lager, bevor gebucht wird.
  - **Buchung:** Artikelbestand, der gebucht wird.
  - **Neu:** Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn der neue Artikel gebucht wird. Wenn Sie den Dialog mit `<Pos1>` verlassen, wird der alte Lagerbestand beibehalten.
- **Preise:** Die Anzeige der Währung richtet sich nach der Eigenwährung, die bei der Installation festgelegt wurde.
  - **€/qm:** Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
  - **Preis:** Gesamtpreis des Artikels.
  - **(Spalte ohne Bezeichnung):** Buchungsstatus der Artikelposition.

| Buchungsstatus mit Farbkennzeichen | Bedeutung |
| :--- | :--- |
| grau | Artikelposition ist vom Prozess (Programm) gebucht worden. |
| rot | Artikelposition ist vom Prozess (Programm) nicht oder noch nicht gebucht worden. |
*Tab. E-3: Buchungsstatus der Artikelposition*

### Lagerausgang
**Buchung > Ausgang**

*Abb. E-3: Lagerausgang*

In diesem Dialog erfassen und buchen Sie den Lagerausgang, z. B., wenn Lagerartikel an die Produktion geliefert werden. Die Lagerausgänge für Kisten, Fächer, Stapel, Gestelle und auftragsbezogenen Warenausgänge buchen Sie an folgender Stelle:
- "Kistenlagerausgang" auf Seite E-28
- "Fachlagerausgang" auf Seite E-34
- "Stapellageränderung" auf Seite E-36
- "Gestelllagerausgang" auf Seite E-41
- "Lagerausgang (Auftragsbezogen)" auf Seite E-45

Sie können folgende Tastaturbefehle ausführen:
- Mit `<Strg>` + `<F8>` können Sie im ersten Feld zwischen dem Dialog Lagereingang und Lagerausgang wechseln.
- Mit `<F5>` können Sie aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.

Die Register, Felder und Spalten sind an folgender Stelle beschrieben:
- "Lagereingang" auf Seite E-16
Die Werte in den Feldern zeigen jeweils die abzubuchenden Mengen an.

### Kistenlagereingang
**Buchung > Kisteneingang**

In diesem Dialog buchen Sie die Lagereingänge für komplette Kisten, z. B. Gitterboxen mit 50 gleichen Scheiben.

In diesem Dialog finden Sie folgende Register:
- "Kistenlagereingang - Stück" auf Seite E-23
- "Kistenlagereingang - Menge" auf Seite E-26

#### Kistenlagereingang – Stück
**Buchung > Kisteneingang > Stück**

*Abb. E-4: Kistenlagereingang – Stück, Kistenlager und Einzelblattkistenlager*

In diesem Register buchen Sie die Lagereingänge für komplette Kisten. Sie können über die Auswahl der Lagerart im Feld Lager auswählen, ob Sie die Lagereingänge ins Kistenlager oder ins Einzelblattkistenlager buchen.
Wenn Sie ein Einzelblattkistenlager auswählen, können Sie die Blätter einzeln in Kisten buchen.
- "Fußbereich - Einzelblattinformationen" auf Seite E-25

Sie können folgende Tastaturbefehle ausführen:
- Mit `<Strg>` + `<F8>` können Sie im ersten Feld zwischen dem Dialog Kistenlagereingang und Kistenlagerausgang wechseln.
- Mit `<F5>` können Sie aus einer Spalte in die kistenbezogenen Angaben im Fußbereich (linke Seite) wechseln.
- Mit `<Shift>` + `<F8>` können Sie aus einer Spalte in die variantenbezogenen Angaben im Fußbereich (rechte Seite) wechseln.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.

##### Kopfbereich
Die Felder sind an folgender Stelle beschrieben:
- "Lagereingang" auf Seite E-16
Zusätzlich wird folgendes Feld beschrieben:
- **Lager:** Lagernummer und Lagerbezeichnung. Wenn Sie die Nummer für ein Einzelblattkistenlager eingeben, können Sie für jede Kiste die Scheiben einzeln erfassen.
  - "Fußbereich - Einzelblattinformationen" auf Seite E-25

##### Rumpfbereich
In diesem Bereich buchen Sie die Bestände und Preise der Artikel in Stückzahlen.
- **Variante:** Maßvariante des Artikels. Mit `<F9>` können Sie die Variantenauswahl aufrufen. Dabei werden nur die Varianten angezeigt, die dem aktuellen Artikel in den Stammdaten zugewiesen sind.
- **Kiste:** Kistennummer.
- **Kistenbezeichnung:** Bezeichnung der Kiste.
- **Lieferant:** Lieferantennummer.
- **Verpackungsart:** Kennzeichen der Verpackungsart, z. B. 13 = Kleine Holzkiste.
- **Neu:** Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn der neue Artikel gebucht wird. Wenn Sie den Dialog mit `<Pos1>` verlassen, wird der alte Lagerbestand beibehalten.
- **Bestände:** Lagerbestand der Variante in Stückzahlen. Mit `<F2>` können Sie durch folgende Anzeigen wechseln:
  - **Alt:** Alter Artikelbestand im Lager, bevor gebucht wird.
  - **Buchung:** Artikelbestand, der gebucht wird.
  - **Neu:** Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn der neue Artikel gebucht wird. Wenn Sie den Dialog mit `<Pos1>` verlassen, wird der alte Lagerbestand beibehalten.
- **Preise:** Die Anzeige der Währung richtet sich nach der Eigenwährung, die bei der Installation festgelegt wurde.
  - **€/qm:** Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
  - **Preis:** Gesamtpreis des Artikels.
  - **(Spalte ohne Bezeichnung):** Buchungsstatus der Artikelposition.

| Buchungsstatus mit Farbkennzeichen | Bedeutung |
| :--- | :--- |
| grau | Artikelposition ist vom Prozess (Programm) gebucht worden. |
| rot | Artikelposition ist vom Prozess (Programm) nicht oder noch nicht gebucht worden. |
*Tab. E-4: Buchungsstatus der Artikelposition*

##### Fußbereich – Kistenbezogene Angaben
Die Felder sind an folgender Stelle beschrieben:
- "Lagereingang" auf Seite E-16
Zusätzlich werden folgende Felder beschrieben:
- **Lieferant:** Lieferantennummer und Lieferantenname.
- **Verpackungsart:** Kennzeichen der Verpackungsart.
- **Reserviert:** Auftragsnummer, für die die Kiste reserviert wurde.
- **Etikett:** Anzeige für den Etikettendruck.
  - J = Etiketten drucken.
  - N = Keine Etiketten drucken.

##### Fußbereich - Einzelblattinformationen
Die Einzelblattinformationen können Sie nur aufrufen, wenn Sie im Kopfbereich im Feld Lager ein Einzelblattkistenlager ausgewählt haben.
- Mit `<Shift>` + `<F12>` können Sie sich die Einzelblattinformationen anzeigen lassen.
- Mit `<Strg>` + `<E>` können Sie die Einzelblattinformationen bearbeiten.
Im Dialog rechts unten wird die Tabelle für die Einzelblattinformationen mit den folgenden Spalten angezeigt:
- **Blatt:** Nummer des Blattes.
- **Bezeichnung:** Bezeichnung des Blattes.
- **EU/Stück:** Stückpreis des Blattes.
- **Ausbeute:** Ausbeute in Prozent.
- **Reserviert:** Reservierungskennzeichen.
  - J = Variante ist für einen Vorgang reserviert.
  - N = Variante ist nicht für einen Vorgang reserviert.

#### Kistenlagereingang – Menge
**Buchung > Kisteneingang > Menge**

*Abb. E-5: Kistenlagereingang – Menge*

In diesem Register buchen Sie die Bestände und Preise der Artikel in Mengeneinheit.
Das Register Menge ist wie das Register Stück aufgebaut.
- "Kopfbereich" auf Seite E-24
- "Fußbereich - Kistenbezogene Angaben" auf Seite E-25

##### Rumpfbereich
In diesem Bereich buchen Sie die Bestände und Preise der Artikel in Mengeneinheit.
- **Variante:** Maßvariante des Artikels. Mit `<F9>` können Sie die Variantenauswahl aufrufen. Dabei werden nur die Varianten angezeigt, die dem aktuellen Artikel in den Stammdaten zugewiesen sind.
- **Kiste:** Kistennummer.
- **Kistenbezeichnung:** Bezeichnung der Kiste.
- **Lieferant:** Lieferantennummer.
- **Verpackungsart:** Kennzeichen der Verpackungsart, z. B. 13 = Kleine Holzkiste.
- **Neu:** Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn der neue Artikel gebucht wird. Wenn Sie den Dialog mit `<Pos1>` verlassen, wird der alte Lagerbestand beibehalten.
- **Bestände:** Lagerbestand der Variante in der Mengeneinheit, die in den Stammdaten definiert ist.
- **ME:** Neu berechneter Artikelbestand in Mengeneinheiten. Dieser Bestand wird übernommen, wenn der neue Artikel gebucht wird. Wenn Sie den Dialog mit `<Pos1>` verlassen, wird der alte Lagerbestand beibehalten.
- **Preise:** Die Anzeige der Währung richtet sich nach der Eigenwährung, die bei der Installation festgelegt wurde.
  - **€/qm:** Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
  - **Preis:** Gesamtpreis des Artikels.
  - **(Spalte ohne Bezeichnung):** Buchungsstatus der Artikelposition.

| Buchungsstatus mit Farbkennzeichen | Bedeutung |
| :--- | :--- |
| grau | Artikelposition ist vom Prozess (Programm) gebucht worden. |
| rot | Artikelposition ist vom Prozess (Programm) nicht oder noch nicht gebucht worden. |
*Tab. E-5: Buchungsstatus der Artikelposition*

### Kistenlagerausgang
**Buchung > Kistenausgang**

*Abb. E-6: Kistenlagerausgang*

In diesem Dialog buchen Sie Lagerausgänge für komplette Kisten. Wenn Sie nur einen Teil der Artikel aus einer Kiste ausbuchen möchten, müssen Sie zuerst die Kiste auflösen und die Artikel der Kiste auf ein anderes Lager buchen.

Sie können folgende Tastaturbefehle ausführen:
- Mit `<Strg>` + `<F8>` können Sie im ersten Feld zwischen dem Dialog Kisteneingang und Kistenausgang wechseln.
- Mit `<F5>` können Sie aus einer Spalte in die kistenbezogenen Angaben im Fußbereich (linke Seite) wechseln.
- Mit `<Shift>` + `<F8>` können Sie aus einer Spalte in die variantenbezogenen Angaben im Fußbereich (rechte Seite) wechseln.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.
- Mit `<Strg>` + `<F12>` können Sie komplette Kisten buchen. Damit wird die gesamte Kiste ausgebucht.
- Mit `<Strg>` + `<F8>` können Sie Kisten auflösen und die Artikel aus der Kiste auf ein Ziellager buchen. Damit werden die einzelnen Scheiben der Kiste in das Ziellager gebucht.

Die Register, Felder und Spalten sind an folgender Stelle beschrieben:
- "Kistenlagereingang" auf Seite E-23

### Fachlagereingang
**Buchung > Facheingang**

In diesem Dialog können Sie Artikel auf Fächer eines Fachlagers buchen.

In diesem Dialog finden Sie folgende Register:
- "Fachlagereingang – Stück" auf Seite E-29
- "Fachlagereingang - Menge" auf Seite E-32

#### Fachlagereingang – Stück
**Buchung > Facheingang > Stück**

*Abb. E-7: Fachlagereingang – Stück*

In diesem Register erfassen und buchen Sie die Bestände und Preise der aktuellen Artikelvariante in Stückzahlen.

Sie können folgende Tastaturbefehle ausführen:
- Mit `<Strg>` + `<F8>` können Sie im ersten Feld zwischen dem Dialog Fachlagereingang und Fachlagerausgang wechseln.
- Mit `<F5>` können Sie aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.

##### Kopfbereich
Die Felder sind an folgender Stelle beschrieben:
- "Lagereingang" auf Seite E-16

##### Rumpfbereich
In diesem Register buchen Sie die Bestände und Preise der Artikel in Stückzahlen.
- **Variante:** Maßvariante des Artikels. Mit `<F9>` können Sie die Variantenauswahl aufrufen. Dabei werden nur die Varianten angezeigt, die dem aktuellen Artikel in den Stammdaten zugewiesen sind.
- **Fach:** Bezeichnung des Fachs.
- **Bestände (Stück):** Lagerbestand der Variante in Stückzahlen.
  - **Alt:** Alter Artikelbestand im Lager, bevor gebucht wird.
  - **Buchung:** Artikelbestand, der gebucht wird.
  - **Neu:** Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn der neue Artikel gebucht wird. Wenn Sie den Dialog mit `<Pos1>` verlassen, wird der alte Lagerbestand beibehalten.
- **Preise:** Die Anzeige der Währung richtet sich nach der Eigenwährung, die bei der Installation festgelegt wurde.
  - **€/qm:** Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
  - **Preis:** Gesamtpreis des Artikels.
  - **(Spalte ohne Bezeichnung):** Buchungsstatus der Artikelposition.

| Buchungsstatus mit Farbkennzeichen | Bedeutung |
| :--- | :--- |
| grau | Artikelposition ist vom Prozess (Programm) gebucht worden. |
| rot | Artikelposition ist vom Prozess (Programm) nicht oder noch nicht gebucht worden. |
*Tab. E-6: Buchungsstatus der Artikelposition*

##### Fußbereich – Variantenbezogene Angaben
- **Objekt:** Bezeichnung des Objekts bei auftragsbezogenen Lagerartikeln, z. B. Baustelle des Kunden.
- **Kostenstelle:** Bezeichnung der Kostenstelle für statistische Auswertungen.
- **Bemerkung:** Textfeld für zusätzliche Informationen.
- **Mindestbestand:** Minimal zulässiger Lagerbestand des Artikels, um Produktionsengpässe zu verhindern.
- **Alarmbestand:** Stückzahl des Artikelbestands, die einen Bestellvorschlag im Einkauf anlegt. Durch Alarmbestände können Sie eine Unterdeckung des Lagers verhindern.
- **Maximalbestand:** Maximal zulässiger Lagerbestand des Artikels, um Lagerkosten zu minimieren.
- **Gesamtpreis:** Gesamtpreis der Artikelvariante.
- **Durchschnittspreis:** Durchschnittlicher Einkaufspreis der Artikelvariante im Lager.
- **Höchstpreis:** Höchster Einkaufspreis der Artikelvariante im Lager.
- **Niedrigstpreis:** Niedrigster Einkaufspreis der Artikelvariante im Lager.
- **LIFO-Gesamtpreis:** Gesamtpreis der Artikelvariante im Lager, wenn die zuletzt eingelagerten Lagerartikel als erste Artikel ausgelagert werden.
- **FIFO-Gesamtpreis:** Gesamtpreis der Artikelvariante im Lager, wenn die zuerst eingelagerten Lagerartikel als erste Artikel ausgelagert werden.

#### Fachlagereingang – Menge
**Buchung > Facheingang > Menge**

*Abb. E-8: Fachlagereingang – Menge*

In diesem Register erfassen und buchen Sie die Bestände und Preise der aktuellen Artikelvariante in Mengeneinheit.
Das Register Menge ist wie das Register Stück aufgebaut.
- "Kopfbereich" auf Seite E-30
- "Fußbereich - Variantenbezogene Angaben" auf Seite E-30

##### Rumpfbereich
In diesem Bereich buchen Sie die Bestände und Preise der Artikel in Mengeneinheit.
- **Variante:** Maßvariante des Artikels. Mit `<F9>` können Sie die Variantenauswahl aufrufen. Dabei werden nur die Varianten angezeigt, die dem aktuellen Artikel in den Stammdaten zugewiesen sind.
- **Fach:** Bezeichnung des Fachs.
- **Bestände (Mengeneinheit):** Lagerbestand der Variante in Mengeneinheit.
  - **Alt:** Alter Artikelbestand im Lager, bevor gebucht wird.
  - **Buchung:** Artikelbestand, der gebucht wird.
  - **Neu:** Neu berechneter Artikelbestand. Dieser Bestand wird übernommen, wenn der neue Artikel gebucht wird. Wenn Sie den Dialog mit `<Pos1>` verlassen, wird der alte Lagerbestand beibehalten.
- **Preise:** Die Anzeige der Währung richtet sich nach der Eigenwährung, die bei der Installation festgelegt wurde.
  - **€/qm:** Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
  - **Preis:** Gesamtpreis des Artikels.
  - **(Spalte ohne Bezeichnung):** Buchungsstatus der Artikelposition.

| Buchungsstatus mit Farbkennzeichen | Bedeutung |
| :--- | :--- |
| grau | Artikelposition ist vom Prozess (Programm) gebucht worden. |
| rot | Artikelposition ist vom Prozess (Programm) nicht oder noch nicht gebucht worden. |
*Tab. E-7: Buchungsstatus der Artikelposition*

### Fachlagerausgang
**Buchung > Fachlagerausgang**

*Abb. E-9: Fachlagerausgang*

In diesem Dialog können Sie Artikel vom Fachlager abbuchen.

Sie können folgende Tastaturbefehle ausführen:
- Mit `<Strg>` + `<F8>` können Sie im ersten Feld zwischen dem Dialog Fachlagereingang und Fachlagerausgang wechseln.
- Mit `<F5>` können Sie aus einer Spalte in die variantenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.

Die Register, Felder und Spalten sind an folgender Stelle beschrieben:
- "Fachlagereingang" auf Seite E-29

### Stapellagereingang
**Buchung > Stapeleingang**

*Abb. E-10: Stapellagereingang*

In diesem Dialog können Sie Artikel auf einen Stapel buchen. Sie können verschiedene Artikel mit unterschiedlichen Abmessungen auf einen Stapel buchen.

Sie können folgende Tastaturbefehle ausführen:
- Mit `<Strg>` + `<F8>` können Sie im ersten Feld zwischen dem Dialog Stapellagereingang und Stapellageränderung wechseln.
- Mit `<F2>` können Sie die Anzeige zwischen Artikel in Stückzahl und Artikel in Mengeneinheit umschalten.
- Mit `<Shift>` + `<F8>` können Sie vom System eine neue Stapelnummer vergeben lassen.
- Mit `<Shift>` + `<F9>` können Sie alle Stapelzeilen kopieren und einer neuen Stapelnummer zuordnen.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.
- Mit `<Strg>` + `<F12>` können Sie einen Stapel einbuchen.
- Mit `<Ende>` können Sie die Stapelbuchung buchen.

#### Kopfbereich
- **Lager:** Lagernummer und Lagerbezeichnung.
- **Lieferant:** Lieferantennummer und Lieferantenname.
- **Letzte Änderung am, von:** Datum der letzten Änderung am Buchungssatz und Name des Anwenders, der die letzte Buchung ausgeführt hat.

#### Rumpfbereich
- **Stapel:** Nummer des Stapelplatzes.
- **Bezeichnung:** Bezeichnung des Stapelplatzes.
- **Artikel:** Artikelnummer des Artikels, der auf dem Stapelplatz eingelagert wird.
- **Variante:** Bezeichnung der Artikelvariante.
- **Anzahl:** Stückzahl des Artikels. Mit `<F2>` können Sie auf Artikel in Mengeneinheit umschalten.
- **Menge/qm:** Menge in Quadratmetern.
- **Preis /qm:** Preis pro Mengeneinheit.

### Stapellageränderung
**Buchung > Stapeländerung**

*Abb. E-11: Stapellageränderung*

In diesem Dialog können Sie nach Artikeln suchen die in Stapeln vorkommen, um sie in ein anderes Lager zu buchen.

Sie können folgende Tastaturbefehle ausführen:
- Mit `<Strg>` + `<F8>` können Sie im Kopfbereich zwischen dem Dialog Stapellagereingang und Stapellageränderung wechseln.
- Mit `<Strg>` + `<F8>` können Sie im Rumpfbereich den ausgewählten Stapel auflösen. Wenn ein Stapel aufgelöst wird, müssen die Artikel aus dem aufgelösten Stapel auf ein anderes Lager gebucht werden. Das Lager für die Artikel geben Sie in der Spalte **Ziellager** ein.
- Mit `<Shift>` + `<F9>` können Sie im Rumpfbereich den ausgewählten Datensatz kopieren.
- Mit `<F2>` können Sie die Anzeige zwischen Artikel in Stückzahl und Artikel in Mengeneinheit umschalten.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.
- Mit `<Strg>` + `<F12>` können Sie einen Stapel ausbuchen.
- Mit `<Ende>` können Sie die Stapeländerung buchen.

Die Felder und Spalten sind an folgender Stelle beschrieben:
- "Stapellagereingang" auf Seite E-35

Zusätzlich werden folgende Felder angezeigt:

#### Kopfbereich
- **Artikel 1, Artikel 2:** Suche über eine Folge von Artikelnummern.

#### Rumpfbereich
- **Ziellager:** Nummer des Ziellagers.

### Gestelllagereingang
**Buchung > Gestelleingang**

*Abb. E-12: Gestelllagereingang*

In diesem Dialog können Sie Artikel auf Gestellen in ein Gestelllager einbuchen.

Sie können folgende Tastaturbefehle ausführen:
- Mit `<Strg>` + `<F8>` können Sie im ersten Feld zwischen dem Dialog Gestelllagereingang und Gestelllagerausgang wechseln.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.

#### Kopfbereich
Im Kopfbereich müssen Sie entweder den Artikel und das Lager angeben oder das Gestell.
- **Artikel:** Artikelnummer und Artikelbezeichnung.
- **Lager:** Lagernummer und Lagerbezeichnung.
- **Gestell:** Externe Bezeichnung des Lagergestells.
- **Gesamtbestand:** Gesamtbestand des Artikels, einschließlich aller Artikelvarianten.
- **Gesamtwert:** Gesamtbetrag des Lagerartikels.
- **Buchungsstatus:** Status der Buchungen im Lager.

| Buchungsstatus mit Farbkennzeichen | Bedeutung |
| :--- | :--- |
| grau | Im Lagereingang sind alle Buchungspositionen vom Prozess (Programm) gebucht worden. |
| rot | Im Lagereingang ist mindestens eine Buchungsposition vom Prozess (Programm) nicht oder noch nicht gebucht worden. |
*Tab. E-8: Buchungsstatus des Lagers*

- **Letzte Änderung am, von:** Datum der letzten Änderung am Buchungssatz und Name des Anwenders, der die letzte Buchung ausgeführt hat.

#### Rumpfbereich
- **Variante:** Maßvariante des Artikels. Mit `<F9>` können Sie die Variantenauswahl aufrufen. Varianten eines Artikels werden nur angezeigt, wenn die Varianten im Stammdatenmodul angelegt sind.
- **Gestell:** Externe Gestellbezeichnung des Lagergestells.
- **G:** Artikelvarianten, die sich auf dem Gestell befinden.
  - ☑ Verschiedene Artikelvarianten stehen auf einem Gestell.
  - ☐ Nur gleiche Artikelvarianten stehen auf einem Gestell.
- **Fach:** Bezeichnung des Fachs.
- **Fifo-Datum:** Datum für die Gestellbuchung nach dem Fifo-Prinzip.
- **Menge:** Aktuelle Stückzahl der Artikel auf dem Lagergestell.
- **Buchung:** Artikelbestand, der gebucht wird.
- **€/qm:** Artikelpreis des Lieferanten in eigener Währung pro Mengeneinheit.
- **Preis:** Gesamtpreis des Artikels.
- **Buchungsstatus:** Status der Buchungen im Gestelllagereingang.

| Buchungsstatus mit Farbkennzeichen | Bedeutung |
| :--- | :--- |
| grau | Buchungsposition ist vom Prozess (Programm) gebucht worden. |
| rot | Buchungsposition ist vom Prozess (Programm) nicht oder noch nicht gebucht worden. |
*Tab. E-9: Buchungsstatus des Gestelllagereingangs*

### Gestelllagerausgang
**Buchung > Gestellausgang**

In diesem Dialog können Sie gestellbezogene Lagerabgänge buchen oder Artikel zwischen Gestellen umbuchen.

In diesem Dialog finden Sie folgende Register:
- "Gestelllagerausgang - Auftragsbezogen" auf Seite E-41
- "Gestelllagerausgang – Umbuchung" auf Seite E-43

#### Gestelllagerausgang – Auftragsbezogen
**Buchung > Gestellausgang > Auftragsbezogen**

*Abb. E-13: Gestelllagerausgang - Auftragsbezogen*

In diesem Register buchen Sie die auftragsbezogenen Lagerabgänge.

Sie können folgende Tastaturbefehle ausführen:
- Mit `<Strg>` + `<F8>` können Sie im ersten Feld zwischen dem Dialog Gestelllagereingang und Gestelllagerausgang wechseln.
- Mit `<F2>` können Sie zwischen den Registern Auftragsbezogen und Umbuchung umschalten.
- Mit `<F5>` können Sie in die variantenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.
- Mit `<Shift>` + `<F8>` können Sie eine Position auflösen.
- **[Zurücksetzen]:** Verwirft die eingegebenen Änderungen.

##### Kopfbereich
Im Kopfbereich müssen Sie entweder den Artikel und das Lager angeben oder das Gestell.
Die Felder sind an folgender Stelle beschrieben:
- "Gestelllagereingang" auf Seite E-38

##### Rumpfbereich
- **Variante:** Maßvariante des Artikels. Mit `<F9>` können Sie die Variantenauswahl aufrufen. Varianten eines Artikels werden nur angezeigt, wenn die Varianten im Stammdatenmodul angelegt sind.
- **Gestell:** Externe Gestellbezeichnung des Lagergestells.
- **G:** Artikelvarianten, die sich auf dem Gestell befinden.
  - ☑ Verschiedene Artikelvarianten stehen auf einem Gestell.
  - ☐ Nur gleiche Artikelvarianten stehen auf einem Gestell.
- **Fach:** Bezeichnung des Fachs.
- **Fifo-Datum:** Datum für die Gestellbuchung nach dem Fifo-Prinzip.
- **Menge:** Aktuelle Stückzahl der Artikel auf dem Lagergestell.
- **Buchung:** Artikelbestand, der gebucht wird.
- **Auftrag:** Auftragsnummer für die auftragsbezogene Gestellbuchung.
- **Position:** Nummer der Gestellposition im Gestelllager.
- **Buchungsstatus:** Status der Buchungen im Lager.

| Buchungsstatus mit Farbkennzeichen | Bedeutung |
| :--- | :--- |
| grau | Buchungsposition ist vom Prozess (Programm) gebucht worden. |
| rot | Buchungsposition ist vom Prozess (Programm) nicht oder noch nicht gebucht worden. |
| gelb | Gestelldaten wurden verändert: Bei der auftragsbezogenen Buchung wurde von diesem Gestell eine Menge oder Teilmenge für die Buchung verplant. |
| halb gelb / halb grau | Nachbearbeitung ist notwendig: Ein neuer Satz wurde angelegt, mit der verbleibenden Gestellmenge für das Unterteil der Auftragsposition. |
*Tab. E-10: Buchungsstatus des Gestelllagerausgangs*

#### Gestelllagerausgang – Umbuchung
**Buchung > Gestellausgang > Umbuchung**

*Abb. E-14: Gestelllagerausgang - Umbuchung*

In diesem Register können Sie die Artikel auf ein neues Gestell bzw. neues Fach umbuchen.

Sie können folgende Tastaturbefehle ausführen:
- Mit `<Strg>` + `<F8>` können Sie im ersten Feld zwischen dem Dialog Gestelllagereingang und Gestelllagerausgang wechseln.
- Mit `<F2>` können Sie zwischen den Registern Auftragsbezogen und Umbuchung umschalten.
- Mit `<F5>` können Sie in die variantenbezogenen Angaben im Fußbereich wechseln.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.
- Mit `<Shift>` + `<F8>` können Sie eine Position auflösen.
- **[Zurücksetzen]:** Verwirft die eingegebenen Änderungen.

##### Kopfbereich
Im Kopfbereich müssen Sie entweder den Artikel und das Lager angeben oder das Gestell.
Die Felder sind an folgender Stelle beschrieben:
- "Gestelllagereingang" auf Seite E-38

##### Rumpfbereich
- **Variante:** Maßvariante des Artikels. Mit `<F9>` können Sie die Variantenauswahl aufrufen. Varianten eines Artikels werden nur angezeigt, wenn die Varianten im Stammdatenmodul angelegt sind.
- **Gestell:** Externe Gestellbezeichnung des Lagergestells.
- **G:** Artikelvarianten, die sich auf dem Gestell befinden.
  - ☑ Verschiedene Artikelvarianten stehen auf einem Gestell.
  - ☐ Nur gleiche Artikelvarianten stehen auf einem Gestell.
- **Fach:** Bezeichnung des Fachs.
- **Fifo-Datum:** Datum für die Gestellbuchung nach dem Fifo-Prinzip.
- **Menge:** Aktuelle Stückzahl der Artikel auf dem Lagergestell.
- **Buchung:** Artikelbestand, der gebucht wird.
- **Gestell neu:** Nummer des Gestells, auf das der Artikel umgebucht wird.
- **Fach neu:** Bezeichnung des Fachs, auf das das Gestell umgebucht wird.
- **Buchungsstatus:** Status der Buchungen im Lager.

| Buchungsstatus mit Farbkennzeichen | Bedeutung |
| :--- | :--- |
| grau | Buchungsposition ist vom Prozess (Programm) gebucht worden. |
| rot | Buchungsposition ist vom Prozess (Programm) nicht oder noch nicht gebucht worden. |
| gelb | Gestelldaten wurden verändert: Bei der auftragsbezogenen Buchung wurde von diesem Gestell eine Menge oder Teilmenge für die Buchung verplant. |
| halb gelb / halb grau | Nachbearbeitung ist notwendig: Ein neuer Satz wurde angelegt, mit der verbleibenden Gestellmenge für das Unterteil der Auftragsposition. |
*Tab. E-11: Buchungsstatus des Gestelllagerausgangs*

### Lagerausgang (Auftragsbezogen)
**Buchung > Ausgang (Auftragsbezogen)**

*Abb. E-15: Lagerausgang (Auftragsbezogen)*

In diesem Dialog können Sie auftragsbezogene Lagerabgänge manuell buchen. In den Artikelstammdaten ist definiert, ob ein Artikel nur manuell gebucht werden kann.

Sie können folgende Tastaturbefehle ausführen:
- Mit `<F2>` können Sie sich die Spalte Termin für den Liefertermin der Position anzeigen lassen.
- Mit `<F3>` können Sie die Buchung auslösen.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.

#### Kopfbereich
- **Auftrag:** Auftragsnummer.
- **Anfahrt:** Liefertermin, an dem der Auftrag beim Kunden angeliefert wird.
- **Kunde:** Kundennummer und Kundenname.
- **Erfasst am, von:** Datum der Auftragserfassung und Name des Erfassers.
- **Gebucht am, von:** Datum der Lagerausgansbuchung und Name des Mitarbeiters, der die Lagerausgangsbuchung gebucht hat.

#### Rumpfbereich
- **Pos:** Nummer der Auftragsposition.
- **Artikel:** Artikelnummer.
- **Bezeichnung:** Artikelbezeichnung.
- **Variante:** Maßvariante der Position.
- **Gesamt:** Gesamtmenge pro Position.
- **Verbucht:** Menge der Position, die bereits abgebucht wurde.
- **Buchen:** Menge der Position, die vom Lager abgebucht werden soll.

Mit `<F2>` können Sie sich die Spalte Termin für den Liefertermin der Position anzeigen lassen.
- **Termin:** Liefertermin der Position.

### Buchungskorrektur – Übersicht
**Buchung > Korrektur**

*Abb. E-16: Buchungskorrektur – Übersicht*

In diesem Dialog können Sie die Suchkriterien festlegen, um sich die Buchungen anzeigen zu lassen und zu korrigieren.

Um Buchungen korrigieren zu können, müssen zuerst Lagerdaten durch das Lagerbuchungssystem angelegt worden sein. Sicherungs-Lagerdaten werden nur angelegt, wenn Zeitpunkte zur automatischen Speicherung der Lagerdaten definiert werden, z. B. der 15. eines jeden Monats. Fehlerhafte Buchungssätze dürfen nicht im Buchungssystem vorhanden sein.

Die Details der Übersicht können Sie sich in der Detailansicht anzeigen lassen.
- "Buchungskorrektur - Details" auf Seite E-48

Sie können folgende Tastaturbefehle ausführen:
- Mit `<F5>` wechseln Sie zwischen der Übersicht und der Detailansicht der ausgewählten Position.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.

#### Kopfbereich
- **Artikel:** Artikelnummer und Artikelbezeichnung.
- **Lager:** Lagernummer und Lagerbezeichnung.
- **von Datum, bis Datum:** Zeitraum, für den Buchungen aufgelistet werden.

#### Rumpfbereich
- **Variante:** Artikelvariante.
- **Farbe:** Farbvariante des Artikels.
- **Lieferant:** Lieferantennummer.
- **Menge:** Mengeneinheit des Artikels in der zu korrigierenden Buchung.
- **Anzahl:** Stückzahl der zu korrigierenden Buchung.
- **Preis:** Stückpreis der Variante.
- **Stat.:** Bezeichnung des Buchungsstatus, z. B. Lagereingang.
- **Datum:** Datum, an dem die Buchung korrigiert wurde.

### Buchungskorrektur – Details
**Buchung > Korrektur > Filtern > <F5>**

*Abb. E-17: Buchungskorrektur – Details*

In diesem Dialog werden die Details einer Buchungskorrektur aus der Übersicht angezeigt und korrigiert.

Sie können folgende Tastaturbefehle ausführen:
- Mit `<F5>` wechseln Sie zwischen der Übersicht und der Detailansicht der ausgewählten Position.
- Mit `<Shift>` + `<F12>` können Sie für den aktuellen Buchungssatz ein neues Datum eingeben.

#### Kopfbereich
Die Felder sind an folgender Stelle beschrieben:
- "Kopfbereich" auf Seite E-47

#### Rumpfbereich
- **Kiste:** Kistennummer.
- **Fach:** Bezeichnung des Fachs.
- **Variante:** Artikelvariante.
- **Farbe:** Farbvariante des Artikels.
- **Lieferant:** Lieferantennummer.
- **Auftrag:** Auftragsnummer, bei auftragsbezogenen Lagerbuchungen.
- **Position:** Nummer der Auftragsposition.
- **Menge:** Mengeneinheit des Artikels in der zu korrigierenden Buchung.
- **Anzahl:** Stückzahl der zu korrigierenden Buchung.
- **Preis:** Stückpreis der Variante.
- **Status:** Bezeichnung des Buchungsstatus, z. B. Lagereingang.
- **Datum:** Datum, an dem die Buchung korrigiert wurde.

## Stammdatenverwaltung

In den Stammdaten verwalten Sie den Lagerraum und die Bestandsgrenzen für Lagerartikel, z. B. legen Sie neue Lagerplätze im Lager an. Außerdem definieren Sie die Lagerartikel und deren Bestandsgrenzen.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Lagerraumverwaltung" auf Seite E-50
- "Artikelstammdaten Lager" auf Seite E-51

### Lagerraumverwaltung
**Stammdaten > Raum**

*Abb. E-18: Lagerraumverwaltung*

In diesem Dialog können Sie neue Lagerräume anlegen. Die festgelegte Zuordnung von Lagernummer, Lagerbezeichnung, Lagerart und Inventurart kann nach dem Speichern nicht mehr geändert werden. Für einen Lagerraum müssen Sie immer die Art des Lagers und der Inventur festlegen.
Mit `<Ende>` speichern Sie die Daten des Lagerraums.

#### Kopfbereich
- **Lager:** Nummer und Bezeichnung des Lagers.
- **Kurzbez.:** Kurzbezeichnung des Lagers.
- **im Haus:** Nummer und Bezeichnung des Hauses oder Mandanten.

#### Rumpfbereich
- **Inventurart:** Art der Bestandskontrolle.
  - **Permanent** = Permanente Inventur.
  - **Zyklisch** = Zyklische Inventur zum Bilanzstichtag.
    - "Inventur - Standardlager" auf Seite E-53
- **Lagerart:** Art des Lagers:
  - **Normallager** = Lager für alle Artikel ohne Restriktionen.
  - **Kistenlager** = Lager für komplette Kisten. Angebrochene Kisten müssen aufgelöst und auf ein anderes Lager gebucht werden.
  - **Fachlager** = Lager für alle Artikel mit zugewiesener Bezeichnung des Fachs.
  - **Hochregallager** = Lager mit Lagerplätzen in Hochregalen.
  - **Stapellager** = Lager für Scheiben mit einheitlichen Abmessungen.
  - **Einzelblattkistenlager** = Lager zur Buchung einzelner Glasblätter in Kisten.
  - **Gestelllager** = Lager mit Lagerplätzen auf Gestellen.
- **Schnittstelle:** Angabe der Softwareschnittstelle. Auswahl für ein kundenseitig angeschlossenes Lagerverwaltungssystem.
- **Größe:** Lagerfläche in Mengeneinheit.
- **Fixe Kosten:** Fixe Kosten der Lagerfläche in Eigenwährung pro Quadratmeter.
- **Variable Kosten:** Variable Kosten der Lagerfläche in Eigenwährung pro Quadratmeter.
- **WE-Lager:** Nummer des Wareneingangslagers.

### Artikelstammdaten Lager
**Stammdaten > Artikel**

*Abb. E-19: Artikelstammdaten Lager*

In diesem Dialog können Sie die Bestandsgrenzen der Lagerartikel festlegen. Die Bestandsgrenzen der Lagerartikel werden durch den Minimalbestand, Alarmbestand und Maximalbestand festgelegt.

Sie können folgende Tastaturbefehle ausführen:
- Wenn Sie sich in einer Spalte im Rumpfbereich befinden, können Sie mit `<Ende>` die Festlegung der Bestandsgrenzen speichern.
- Mit `<F5>` können Sie in den Fußbereich wechseln.

#### Kopfbereich
- **Artikel:** Artikelnummer und Artikelbezeichnung.
- **Lager:** Lagernummer und Lagerbezeichnung.
- **Bestellvariante:** Artikelvariante für Nachbestellungen.
- **Bestellfarbe:** Farbvariante des Artikels für Nachbestellungen.

#### Bestandsgrenzen
- **Mindestbestand:** Minimal zulässiger Lagerbestand des Artikels, um Produktionsengpässe zu verhindern.
- **Alarmbestand:** Stückzahl des Artikelbestands, die einen Bestellvorschlag im Einkauf anlegt. Durch Alarmbestände können Sie eine Unterdeckung des Lagers verhindern.
- **Maximalbestand:** Maximal zulässiger Lagerbestand des Artikels, um Lagerkosten zu minimieren.

#### Rumpfbereich
Mit `<F2>` können Sie die Anzeige zwischen Artikel in Stückzahl und Artikel in Mengeneinheit umschalten.
- **Variante:** Maßvariante des Artikels.
- **Farbe:** Farbvariante des Artikels.

#### Fußbereich
- **Bemerkung:** Mit `<F5>` können Sie in das Textfeld für Bemerkungen zur Artikelvariante wechseln.

## Inventurverwaltung

Mit der Inventurverwaltung gleichen Sie die gezählten Bestände mit den vom System gebuchten Beständen ab und korrigieren die Zahlen entsprechend im System.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Inventur - Standardlager" auf Seite E-53
- "Inventur - Kistenlager" auf Seite E-56
- "Inventur - Fachlager" auf Seite E-58
- "Inventur - Stapellager" auf Seite E-59
- "Inventur - Gestelllager" auf Seite E-60

### Inventur – Standardlager
**Inventur > Lager**

*Abb. E-20: Inventur-Standardlager*

In diesem Dialog können Sie die Inventur für das Standardlager durchführen und abschließen.

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

#### Kopfbereich
- **von Artikel, bis Artikel:** Wertebereich der Artikelnummern um die Inventurliste zu filtern.
- **von Lager, bis Lager:** Eingabe der Lagernummern:
  - Wenn Sie in den Feldern von Lager, bis Lager dieselbe Lagernummer eingeben, wird das Lager für die Inventur freigeschaltet.
  - Wenn Sie in den Feldern von Lager, bis Lager einen Bereich von Lagernummern eingeben, werden die Datensätze zur Ansicht in den Dialog geladen.
- **Inventur/Bewertung vom:** Datum der Inventur.

#### Rumpfbereich
Folgende Spalten werden angezeigt:
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Variante:** Maßvariante der Position.
- **S:** Storno des Artikels.
  - N = Kein Storno des Artikels.
  - J = Artikel wurde storniert.
- **Soll-Anzahl:** Anzeige für Soll-Stückzahl des Artikels im Lager.
- **Ist-Anzahl:** Eingabe für Ist-Stückzahl des gezählten Artikels im Lager.
- **Preis:** Gesamtpreis des Ist-Bestands des Artikels.
- **ME:** Durchschnittspreises pro Mengeneinheit für den Ist-Bestand, z. B. 75,00 € pro qm.
- **Bemerkung:** Inventurvermerk für statistische Auswertungen.

Mit `<F2>` können Sie die folgenden Spalten anzeigen lassen:
- **Soll-Bestand:** Anzeige für Soll-Wert der Mengeneinheit des Artikelbestands im Lager.
- **Ist-Bestand:** Eingabe für Ist-Wert der gezählten Mengeneinheit des Artikelbestands im Lager.

#### Fußbereich
- **Artikel:** Artikelbezeichnung des ausgewählten Artikels.
- **D-Preis:** Durchschnittspreis des ausgewählten Artikels für den Ist-Bestand.
- **G-Preis:** Gesamtpreis des ausgewählten Artikels für den Ist-Bestand.
- **Lager:** Lagerbezeichnung des ausgewählten Lagers.
- **LIFO-Preis:** Artikelpreis im Lager, wenn nach der LIFO-Buchungsmethode abgebucht und berechnet wird.
- **FIFO-Preis:** Artikelpreis im Lager, wenn nach der FIFO-Buchungsmethode abgebucht und berechnet wird.

### Inventur – Kistenlager
**Inventur > Kistenlager**

*Abb. E-21: Inventur-Kistenlager*

In diesem Dialog können Sie die Inventur für das Kistenlager durchführen und abschließen.
Die Beschreibung für die Felder finden Sie an folgender Stelle:
- "Kopfbereich" auf Seite E-54

#### Rumpfbereich
- **Kiste:** Kistennummer.
- **Lager:** Lagernummer.
- **Artikel:** Artikelnummer.
- **Variante:** Maßvariante der Position.
- **S:** Storno des Artikels.
  - N = Kein Storno des Artikels.
  - J = Artikel wurde storniert.
- **Menge:** Gesamte Scheibenfläche in einer Kiste.
- **Anzahl:** Anzahl der Scheiben in der Kiste.
- **VA:** Kennzeichen der Verpackungsart.
- **Liefnr.:** Lieferantennummer.
- **ME:** Durchschnittspreis pro Mengeneinheit für den Ist-Bestand, z. B. 75,00 € pro qm.
- **Bemerkung:** Inventurvermerk für statistische Auswertungen.

#### Fußbereich
- **Artikel:** Artikelbezeichnung.
- **Lager:** Lagerbezeichnung.
- **Kiste:** Kistenbezeichnung.
- **Verpackart:** Kennzeichen der Verpackungsart.
- **Lieferant:** Lieferantenname.

### Inventur – Fachlager
**Inventur > Fachlager**

*Abb. E-22: Inventur-Fachlager*

In diesem Dialog können Sie die Inventur für das Fachlager durchführen und abschließen.
Die Beschreibung für die Felder finden Sie an folgender Stelle:
- "Kopfbereich" auf Seite E-54
- "Fußbereich" auf Seite E-55

#### Rumpfbereich
- **Lager:** Lagernummer.
- **Artikel:** Artikelnummer.
- **Variante:** Maßvariante der Position.
- **S:** Storno des Artikels.
  - N = Kein Storno des Artikels.
  - J = Artikel wurde storniert.
- **Fach:** Bezeichnung des Fachs.
- **Menge:** Menge des Artikels in Mengeneinheit.
- **Anzahl:** Eingabe für Ist-Bestand des gezählten Artikelbestands im Stapel.
- **Preis:** Gesamtpreis des Ist-Bestands des Artikels.
- **Bemerkung:** Inventurvermerk für statistische Auswertungen.

### Inventur – Stapellager
**Inventur > Stapellager**

*Abb. E-23: Inventur-Stapellager*

In diesem Dialog können Sie die Inventur für das Stapellager durchführen und abschließen.
Die Beschreibung für die Felder finden Sie an folgender Stelle:
- "Kopfbereich" auf Seite E-54
- "Fußbereich" auf Seite E-55

#### Rumpfbereich
- **Lager:** Lagernummer.
- **Artikel:** Artikelnummer.
- **Variante:** Maßvariante der Position.
- **S:** Storno des Artikels.
  - N = Kein Storno des Artikels.
  - J = Artikel wurde storniert.
- **Stapel:** Stapelnummer.
- **Bezeichnung:** Bezeichnung des Stapels.
- **Anzahl:** Eingabe für Ist-Bestand des gezählten Artikelbestands im Stapel.
- **Preis:** Gesamtpreis des Ist-Bestands des Artikels.
- **Bemerkung:** Inventurvermerk für statistische Auswertungen.

### Inventur – Gestelllager
**Inventur > Gestelllager**

*Abb. E-24: Inventur-Gestelllager*

In diesem Dialog können Sie die Inventur für das Gestelllager durchführen und abschließen.
Die Beschreibung für die Felder finden Sie an folgender Stelle:
- "Kopfbereich" auf Seite E-54
- "Fußbereich" auf Seite E-55

#### Rumpfbereich
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
  - ☑ Verschiedene Artikelvarianten stehen auf einem Gestell.
  - ☐ Nur gleiche Artikelvarianten stehen auf einem Gestell.
- **Gestell:** Bezeichnung des Gestells.
- **Fach:** Bezeichnung des Fachs.
- **Soll:** Soll-Bestand des Artikels.
- **Ist:** Ist-Bestand des Artikels.
- **FIFO-Datum:** Datum für die Gestellbuchung nach dem Fifo-Prinzip.
- **Status:** Status der Buchungen im Gestelllager.

| Buchungsstatus mit Farbkennzeichen | Bedeutung |
| :--- | :--- |
| grau | Buchungsposition ist vom Prozess (Programm) gebucht worden. |
| rot | Buchungsposition ist vom Prozess (Programm) nicht oder noch nicht gebucht worden. |
| gelb | Buchungsposition ist geändert worden. |
| halb gelb / halb grau | Buchungsposition ist ein Unterteil eines Auftrags. Buchungsposition muss auf ein anderes Lager gebucht werden, z. B. Fachlager. |
*Tab. E-12: Buchungsstatus im Gestelllager*

## Bewertung

In der Bewertung können Sie die wertmäßigen Verluste des Umlaufvermögens innerhalb einer Inventur bearbeiten. Für die Inventur können die Gegenstände des Umlaufvermögens mit dem Niederstwertprinzip (Anschaffungs-, Herstellungs- oder Tageswert) in der Schlussbilanz eingesetzt werden.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Bestandsbewertung - Standardlager" auf Seite E-63
- "Bestandsbewertung – Kistenlager" auf Seite E-66
- "Bestandsbewertung – Fachlager" auf Seite E-67
- "Bestandsbewertung – Stapellager" auf Seite E-68
- "Bestandsbewertung – Gestelllager" auf Seite E-69

### Bestandsbewertung – Standardlager
**Bewertung > Lager**

*Abb. E-25: Bestandsbewertung - Standardlager*

In diesem Dialog können Sie eine wertmäßige Korrektur des Artikelbestands innerhalb einer Inventur durchführen, z. B. wenn die Werte eines Lagerartikels von den aktuellen Werten abweichen.

Die Dialoge für die Bestandsbewertung in den verschiedenen Lagerarten sind identisch aufgebaut und werden daher für das Standardlager beschrieben. Die Beschreibung gilt daher gleichermaßen für:
- Kistenlager
- Fachlager
- Stapellager
- Gestelllager

Sie können folgende Tastaturbefehle ausführen:
- Mit `<F2>` können Sie die Anzeige zwischen Artikel in Stückzahl und Artikel in Mengeneinheit umschalten. Die Funktion gilt nur für das Standardlager.
- Mit `<Ende>` können Sie die wertmäßige Korrektur abschließen.

#### Kopfbereich
- **von Artikel, bis Artikel:** Wertebereich der Artikelnummern um die Liste zu filtern.
- **von Lager, bis Lager:** Eingabe der Lagernummern:
  - Wenn Sie in den Feldern von Lager, bis Lager dieselbe Lagernummer eingeben, wird das Lager für die Bestandsbewertung freigeschaltet.
  - Wenn Sie in den Feldern von Lager, bis Lager einen Bereich von Lagernummern eingeben, werden die Datensätze zur Ansicht in den Dialog geladen.
- **Inventur/Bewertung vom:** Datum der Bestandsbewertung.

#### Rumpfbereich
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
- **ME:** Eingabe des Durchschnittspreises pro Mengeneinheit für den Ist-Bestand, z. B. 75,00 € pro qm.
- **Bemerkung:** Inventurvermerk für statistische Auswertungen.

Mit `<F2>` können Sie die folgenden Spalten anzeigen lassen:
- **Soll-Bestand:** Anzeige für Soll-Wert der Mengeneinheit des Artikelbestands im Lager.
- **Ist-Bestand:** Anzeige für Ist-Wert der gezählten Mengeneinheit des Artikelbestands im Lager.

#### Fußbereich
- **Artikel:** Artikelbezeichnung des ausgewählten Artikels.
- **D-Preis:** Durchschnittspreis des ausgewählten Artikels für den Ist-Bestand.
- **G-Preis:** Gesamtpreis des ausgewählten Artikels für den Ist-Bestand.
- **Lager:** Lagerbezeichnung des ausgewählten Lagers.
- **LIFO-Preis:** Artikelpreis im Lager, wenn nach der LIFO-Buchungsmethode abgebucht und berechnet wird.
- **FIFO-Preis:** Artikelpreis im Lager, wenn nach der FIFO-Buchungsmethode abgebucht und berechnet wird.

### Bestandsbewertung – Kistenlager
**Bewertung > Kistenlager**

*Abb. E-26: Bestandsbewertung-Kistenlager*

In diesem Dialog können Sie eine wertmäßige Korrektur des Artikelbestands innerhalb einer Inventur durchführen, z. B. wenn die Werte von Kisten von den aktuellen Werten abweichen.
Die Bestandsbewertung darf nur innerhalb eines einzelnen Lagers ausgeführt werden.
Die Felder und Spalten sind an folgender Stelle beschrieben:
- "Bestandsbewertung - Standardlager" auf Seite E-63

### Bestandsbewertung – Fachlager
**Bewertung > Fachlager**

*Abb. E-27: Bestandsbewertung-Fachlager*

In diesem Dialog können Sie eine wertmäßige Korrektur des Artikelbestands innerhalb einer Inventur durchführen, z. B. wenn die Werte von Lagerartikeln eines Faches von den aktuellen Werten abweichen.
Die Bestandsbewertung darf nur innerhalb eines einzelnen Lagers ausgeführt werden.
Die Felder und Spalten sind an folgender Stelle beschrieben:
- "Bestandsbewertung - Standardlager" auf Seite E-63

### Bestandsbewertung – Stapellager
**Bewertung > Stapellager**

*Abb. E-28: Bestandsbewertung-Stapellager*

In diesem Dialog können Sie eine wertmäßige Korrektur des Artikelbestands innerhalb einer Inventur durchführen, z. B. wenn die Werte von Artikeln eines Stapels von den aktuellen Werten abweichen.
Die Bestandsbewertung darf nur innerhalb eines einzelnen Lagers ausgeführt werden.
Die Felder und Spalten sind an folgender Stelle beschrieben:
- "Bestandsbewertung - Standardlager" auf Seite E-63

### Bestandsbewertung – Gestelllager
**Bewertung > Gestelllager**

*Abb. E-29: Bestandsbewertung-Gestelllager*

In diesem Dialog können Sie eine wertmäßige Korrektur des Artikelbestands innerhalb einer Inventur durchführen, z. B. wenn die Werte von Artikeln eines Gestells von den aktuellen Werten abweichen.
Die Bestandsbewertung darf nur innerhalb eines einzelnen Lagers ausgeführt werden.
Die Felder und Spalten sind an folgender Stelle beschrieben:
- "Bestandsbewertung - Standardlager" auf Seite E-63
Sie können folgenden Tastaturbefehl ausführen:
Mit `<F2>` können Sie die Anzeige für Artikel von Stückzahl zu Mengeneinheit umschalten. Die Funktion gilt nur für das Gestelllager.

## Informationssystem

Im Informationssystem können Sie die Lagerdaten überwachen. Über das Informationssystem können Sie die Suchfunktionen ausführen.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Info-Lager-Artikel" auf Seite E-71
- "Info-Lager-Varianten" auf Seite E-75
- "Info-Lager-Fächer" auf Seite E-79
- "Info-Lager-Gestelle" auf Seite E-82
- "Info-Lager-Stapel" auf Seite E-85
- "Info-Lager-Blätter" auf Seite E-88
- "Info-Lager-Historie" auf Seite E-91
- "Aufträge/Bestellungen" auf Seite E-96
- "Buchungsstatus" auf Seite E-100
- "Lagerinformationen – Pickliste" auf Seite E-105
- "Lagerinformationen - Trefferliste" auf Seite E-106
- "LVR-Status" auf Seite E-107
- "Reichweite - Bestandsprognose" auf Seite E-107
- "Reichweite - Trefferliste" auf Seite E-108
- "Dispositiver Bestand" auf Seite E-109
- "Bestandsprognose" auf Seite E-110

Zusätzlich können Sie sich individuelle Informationsübersichten mittels SQL-Abfragen zusammenstellen.
- Verkauf, "SQL-Abfragen - Ausführen" auf Seite D-217

### Info-Lager-Artikel
**Infosystem > Artikel**

In diesem Dialog können Sie sich die Lagerbestände oder Artikelbestände anzeigen lassen.

Zu diesem Dialog werden folgende Unterdialoge angezeigt:
- "Info-Lager-Artikel – Filterdialog" auf Seite E-71
- "Info-Lager-Artikel - Trefferliste" auf Seite E-72
- "Info-Lager-Artikel – Trefferliste-Details" auf Seite E-73

#### Info-Lager-Artikel – Filterdialog
**Infosystem > Artikel**

*Abb. E-30: Info-Lager-Artikel – Filterdialog*

In diesem Dialog können Sie die Suchkriterien festlegen, um sich die Lagerbestände oder Artikelbestände anzeigen zu lassen. Die Ergebnisse der Suche können Sie sich in der Trefferliste und in der Detailansicht anzeigen lassen.
- "Info-Lager-Artikel – Trefferliste" auf Seite E-72
- "Info-Lager-Artikel - Trefferliste-Details" auf Seite E-73
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Menge:** Artikel in Mengeneinheit.
- **Gesamtpreis:** Gesamtpreis des Artikelbestands im ausgewählten Lager.
- **Durchschnittspreis:** Durchschnittlicher Preis pro Mengeneinheit des Artikels.
- **Letzte Änderung:** Datum, an dem der Buchungssatz zuletzt gebucht wurde.

#### Info-Lager-Artikel – Trefferliste
**Infosystem > Artikel > Filtern**

*Abb. E-31: Info-Lager-Artikel – Trefferliste*

In diesem Dialog werden die Ergebnisse der Suche nach Lagerartikeln angezeigt.
Details zu den Lagerartikeln werden in der Detailansicht angezeigt.
- "Info-Lager-Artikel - Trefferliste-Details" auf Seite E-73
Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

##### Trefferliste
Folgende Spalten werden angezeigt:
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Bestand:** Lagerbestand des Artikels in Mengeneinheit.
- **G-Preis:** Gesamtpreis des Artikels.
- **D-Preis:** Durchschnittspreis pro Mengeneinheit.
- **H-Preis:** Höchster Einkaufspreis pro Mengeneinheit.
- **N-Preis:** Niedrigster Einkaufspreis pro Mengeneinheit.

#### Info-Lager-Artikel – Trefferliste-Details
**Infosystem > Artikel > Filtern > <F5>**

*Abb. E-32: Info-Lager-Artikel – Trefferliste-Details*

In diesem Dialog werden die Details zur Trefferliste der Lagerartikel angezeigt. Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

##### Details
- **Artikel:** Artikelnummer und Artikelbezeichnung.
- **Lager:** Lagernummer.
- **Bestand:** Lagerbestand des Artikels in Mengeneinheit.
- **Mindestbestand:** Minimalbestand des Artikels auf Lager.
- **Alarmbestand:** Alarmbestand des Artikels auf Lager.
- **Bestandobergrenze:** Maximalbestand des Artikels auf Lager.
- **Höchstbestand:** Maximalstückzahl des Artikels auf Lager, seit der letzten Inventur.
- **Niedrigstbestand:** Minimalstückzahl des Artikels auf Lager, seit der letzten Inventur.
- **D-Bestand:** Durchschnittlicher Lagerbestand des Artikels, seit der letzten Inventur.
- **D-Verbrauch:** Durchschnittliche Lagerabbuchung des Artikels, seit der letzten Inventur.
- **Gesamtpreis:** Gesamtpreis des Artikels.
- **D-Preis:** Durchschnittspreis pro Mengeneinheit.
- **Höchstpreis:** Höchster Einkaufspreis des Artikels.
- **Niedrigstpreis:** Niedrigster Einkaufspreis des Artikels.
- **LIFO-Gesamtpreis:** Gesamtpreis der Artikelvariante im Lager, wenn nach der LIFO-Buchungsmethode abgebucht und berechnet wird.
- **FIFO-Gesamtpreis:** Gesamtpreis der Artikelvariante im Lager, wenn nach der FIFO-Buchungsmethode abgebucht und berechnet wird.
- **Letzte Änderung am, von:** Datum, an dem der Buchungssatz gebucht wurde und Name des Anwenders, der die Buchung ausgeführt hat.

### Info-Lager-Varianten
**Infosystem > Variante**

In diesem Dialog können Sie sich die Informationen zu den Artikelvarianten nach ausgewählten Kriterien anzeigen lassen.

Zu diesem Dialog werden folgende Unterdialoge angezeigt:
- "Info-Lager-Varianten – Filterdialog" auf Seite E-75
- "Info-Lager-Varianten - Trefferliste" auf Seite E-76
- "Info-Lager-Varianten - Trefferliste-Details" auf Seite E-77

#### Info-Lager-Varianten – Filterdialog
**Infosystem > Variante**

*Abb. E-33: Info-Lager-Varianten - Filterdialog*

In diesem Dialog können Sie die Informationen zu den Artikelvarianten nach ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste angezeigt. Die Details können Sie in der Detailansicht einsehen.
- "Info-Lager-Varianten - Trefferliste" auf Seite E-76
- "Info-Lager-Varianten - Trefferliste-Details" auf Seite E-77
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Variante:** Maßvariante des Artikels in der Kiste.
- **Farbe:** Farbvariante des Artikels.
- **Kiste:** Kistennummer.
- **Kistenbezeichnung:** Bezeichnung der Kiste.
- **Letzte Änderung:** Datum, an dem der Buchungssatz gebucht wurde.
- **Menge:** Artikel in Mengeneinheit.
- **Anzahl:** Stückzahl des Artikels.
- **Gesamtpreis:** Gesamtpreis des Artikelbestands.
- **Durchschnittspreis:** Durchschnittlicher Preis pro Mengeneinheit des Artikels.

#### Info-Lager-Varianten – Trefferliste
**Infosystem > Variante > Filtern**

*Abb. E-34: Info-Lager-Varianten – Trefferliste*

In diesem Dialog können Sie die Informationen zu den Artikelvarianten nach ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste angezeigt. Die Details können Sie in der Detailansicht einsehen.
- "Info-Lager-Varianten - Trefferliste-Details" auf Seite E-77
Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

##### Trefferliste
- **Artikel:** Artikelnummer.
- **Bezeichnung:** Artikelbezeichnung.
- **Lager:** Lagernummer.
- **Kiste:** Kistennummer.
- **Variante:** Maßvariante des Artikels in der Kiste.
- **Farbe:** Farbvariante des Artikels.
- **Anzahl:** Stückzahl des Artikels.
- **Bestand:** Artikelbestand in Mengeneinheit.
- **Netto-ME:** Netto-Menge pro Kiste in Mengeneinheit des Artikels.
- **Preis:** Gesamtpreis des Artikels.

#### Info-Lager-Varianten – Trefferliste-Details
**Infosystem > Variante > Filtern > <F5>**

*Abb. E-35: Info-Lager-Varianten – Trefferliste-Details*

In diesem Dialog werden die Details zur Trefferliste der Artikelvarianten angezeigt.
Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

##### Details
- **Artikel:** Artikelnummer und Artikelbezeichnung.
- **Lager:** Lagernummer.
- **Kiste:** Kistennummer und Kistenbezeichnung.
- **Variante:** Abmessungen der Variante.
- **Farbe:** Farbvariante des Artikels.
- **Anzahl:** Stückzahl des Artikels.
- **Bestand:** Artikelbestand in Mengeneinheit.
- **Netto Menge:** Netto-Menge pro Kiste in Mengeneinheit des Artikels.
- **Mindestbestand:** Minimalbestand des Artikels auf Lager.
- **Alarmbestand:** Alarmbestand des Artikels auf Lager.
- **Bestandobergrenze:** Maximalbestand des Artikels auf Lager.
- **Höchstbestand:** Maximalstückzahl des Artikels auf Lager, seit der letzten Inventur.
- **Niedrigstbestand:** Minimalstückzahl des Artikels auf Lager, seit der letzten Inventur.
- **D-Bestand:** Durchschnittlicher Lagerbestand des Artikels, seit der letzten Inventur.
- **D-Verbrauch:** Durchschnittliche Lagerabbuchung des Artikels, seit der letzten Inventur.
- **Gesamtpreis:** Gesamtpreis des Artikels.
- **D-Preis:** Durchschnittspreis pro Mengeneinheit.
- **Höchstpreis:** Höchster Einkaufspreis des Artikels.
- **Niedrigstpreis:** Niedrigster Einkaufspreis des Artikels.
- **LIFO-Gesamtpreis:** Gesamtpreis der Artikelvariante im Lager, wenn nach der LIFO-Buchungsmethode abgebucht und berechnet wird.
- **FIFO-Gesamtpreis:** Gesamtpreis der Artikelvariante im Lager, wenn nach der FIFO-Buchungsmethode abgebucht und berechnet wird.
- **Letzte Änderung am, von:** Datum, an dem der Buchungssatz gebucht wurde und Name des Anwenders, der die Buchung ausgeführt hat.

### Info-Lager-Fächer
**Infosystem > Fach**

In diesem Dialog können Sie sich die Informationen zu den Lagerfächern anzeigen lassen.

Zu diesem Dialog werden folgende Unterdialoge angezeigt:
- "Info-Lager-Fächer – Filterdialog" auf Seite E-79
- "Info-Lager-Fächer – Trefferliste" auf Seite E-80
- "Info-Lager-Fächer – Trefferliste-Details" auf Seite E-81

#### Info-Lager-Fächer – Filterdialog
**Infosystem > Fach**

*Abb. E-36: Info-Lager-Fächer – Filterdialog*

In diesem Dialog können Sie die Informationen zu den Lagerfächern nach ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste angezeigt. Die Details können Sie in der Detailansicht einsehen.
- "Info-Lager-Fächer - Trefferliste" auf Seite E-80
- "Info-Lager-Fächer - Trefferliste-Details" auf Seite E-81
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Fach:** Bezeichnung des Fachs.
- **Variante:** Abmessungen der Variante.
- **Farbe:** Farbvariante des Artikels.
- **Datum:** Datum, an dem der Buchungssatz gebucht wurde.
- **Anzahl:** Stückzahl des Artikels.
- **Menge:** Artikel in Mengeneinheit.

#### Info-Lager-Fächer – Trefferliste
**Infosystem > Fach > Filtern**

*Abb. E-37: Info-Lager-Fächer – Trefferliste*

In diesem Dialog werden die Ergebnisse der Suche nach Lagerfächern angezeigt. Die Details können Sie in der Detailansicht einsehen.
- "Info-Lager-Artikel - Trefferliste-Details" auf Seite E-73
Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

##### Trefferliste
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Fach:** Bezeichnung des Fachs.
- **Variante:** Abmessungen der Variante.
- **Menge:** Artikel in Mengeneinheit.
- **Stück:** Stückzahl des Artikels.
- **Preis:** Gesamtpreis des Artikels.
- **Datum:** Datum, an dem der Buchungssatz gebucht wurde.

#### Info-Lager-Fächer – Trefferliste-Details
**Infosystem > Fach > Filtern > <F5>**

*Abb. E-38: Info-Lager-Fächer – Trefferliste-Details*

In diesem Dialog werden die Details zur Trefferliste der Lagerfächer angezeigt.
Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

##### Details
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Fach:** Bezeichnung des Fachs.
- **Variante:** Abmessungen der Variante.
- **Farbe:** Farbvariante des Artikels.
- **Menge:** Artikel in Mengeneinheit.
- **Stück:** Stückzahl des Artikels.
- **Preis:** Gesamtpreis des Artikels.

### Info-Lager-Gestelle
**Infosystem > Gestell**

In diesem Dialog können Sie sich die Informationen zu den Lagergestellen anzeigen lassen.

Zu diesem Dialog werden folgende Unterdialoge angezeigt:
- "Info-Lager-Gestelle - Filterdialog" auf Seite E-82
- "Info-Lager-Gestelle – Trefferliste-Allgemein" auf Seite E-83
- "Info-Lager-Gestelle - Trefferliste-Details" auf Seite E-84

#### Info-Lager-Gestelle – Filterdialog
**Infosystem > Gestell**

*Abb. E-39: Info-Lager-Gestelle - Filterdialog*

In diesem Dialog können Sie die Informationen zu den Lagergestellen nach ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste angezeigt. Die Details können Sie in der Detailansicht einsehen.
- "Info-Lager-Gestelle - Trefferliste-Allgemein" auf Seite E-83
- "Info-Lager-Gestelle - Trefferliste-Details" auf Seite E-84
- **Lager:** Lagernummer.
- **Gestellnr.:** Nummer des Lagergestells.
- **Gestell:** Bezeichnung des Gestells.
- **Fach:** Bezeichnung des Fachs.
- **Artikel:** Artikelnummer.
- **Variante:** Abmessungen der Variante.
- **Farbe:** Farbvariante des Artikels.
- **Anzahl:** Stückzahl des Artikels.
- **Fifo-Datum:** Datum für die Gestellbuchung nach dem Fifo-Prinzip.

#### Info-Lager-Gestelle – Trefferliste-Allgemein
**Infosystem > Gestell > Filtern > Allgemein**

*Abb. E-40: Info-Lager-Gestelle - Trefferliste-Allgemein*

In diesem Dialog werden die Ergebnisse der Suche nach Lagergestellen angezeigt. Die Details können Sie in der Detailansicht einsehen.
- "Info-Lager-Gestelle - Trefferliste-Details" auf Seite E-84
Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

##### Trefferliste
- **Lager:** Lagernummer.
- **Artikel:** Artikelnummer.
- **Variante:** Abmessungen der Variante.
- **Gestellnr.:** Nummer des Lagergestells.
- **Gestell:** Bezeichnung des Gestells.
- **Fach:** Bezeichnung des Fachs.
- **Bezeichnung:** Bezeichnung des Fachs.
- **Stück:** Stückzahl des Artikels.
- **Preis:** Gesamtpreis des Artikels.
- **Fifo-Datum:** Datum für die Gestellbuchung nach dem Fifo-Prinzip.

#### Info-Lager-Gestelle – Trefferliste-Details
**Infosystem > Gestell > Filtern > Details**

*Abb. E-41: Info-Lager-Gestelle - Trefferliste-Details*

In diesem Dialog werden die Details zur Trefferliste der Lagergestelle angezeigt. Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

##### Details
- **Artikel:** Artikelnummer.
- **Variante:** Abmessungen der Variante.
- **Farbe:** Farbvariante des Artikels.
- **Stück:** Stückzahl des Artikels.
- **Preis:** Gesamtpreis des Artikels.
- **Lager:** Lagernummer.
- **Gestell:** Bezeichnung des Gestells.
- **Fach:** Bezeichnung des Fachs.
- **Fifo-Datum:** Datum für die Gestellbuchung nach dem Fifo-Prinzip.
- **Letzte Änderung am, von:** Datum der letzten Änderung am Buchungssatz und Name des Anwenders, der die letzte Buchung ausgeführt hat.

### Info-Lager-Stapel
**Infosystem > Stapel**

In diesem Dialog können Sie sich die Informationen zu den Lagerstapeln anzeigen lassen.

Zu diesem Dialog werden folgende Unterdialoge angezeigt:
- "Info-Lager-Stapel – Filterdialog" auf Seite E-85
- "Info-Lager-Stapel - Trefferliste" auf Seite E-86
- "Info-Lager-Stapel - Trefferliste-Details" auf Seite E-87

#### Info-Lager-Stapel – Filterdialog
**Infosystem > Stapel**

*Abb. E-42: Info-Lager-Stapel - Filterdialog*

In diesem Dialog können Sie die Informationen zu den Lagerstapeln nach ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste angezeigt. Die Details können Sie in der Detailansicht einsehen.
- "Info-Lager-Stapel - Trefferliste" auf Seite E-86
- "Info-Lager-Stapel - Trefferliste-Details" auf Seite E-87
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Stapel:** Stapelnummer.
- **Stapelbez.:** Bezeichnung des Stapels.
- **Variante:** Abmessungen der Variante.
- **Farbe:** Farbvariante des Artikels.
- **Datum:** Datum, an dem der Buchungssatz gebucht wurde.
- **Anzahl:** Stückzahl des Artikels.
- **Menge:** Artikel in Mengeneinheit.

#### Info-Lager-Stapel – Trefferliste
**Infosystem > Stapel > Filtern**

*Abb. E-43: Info-Lager-Stapel - Trefferliste*

In diesem Dialog werden die Ergebnisse der Suche nach Lagerstapel angezeigt. Die Details können Sie in der Detailansicht einsehen.
- "Info-Lager-Stapel - Trefferliste-Details" auf Seite E-87
Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

##### Trefferliste
- **Stapel:** Stapelnummer.
- **Bezeichnung:** Bezeichnung des Stapels.
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Variante:** Abmessungen der Variante.
- **Menge:** Artikel in Mengeneinheit.
- **Stück:** Stückzahl des Artikels.
- **Preis:** Gesamtpreis des Artikels.
- **Datum:** Datum, an dem der Buchungssatz gebucht wurde.

#### Info-Lager-Stapel – Trefferliste-Details
**Infosystem > Stapel > Filtern > <F5>**

*Abb. E-44: Info-Lager-Stapel - Trefferliste-Details*

In diesem Dialog werden die Details zur Trefferliste der Lagerstapel angezeigt. Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

##### Details
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Stapel:** Stapelnummer.
- **Variante:** Abmessungen der Variante.
- **Farbe:** Farbvariante des Artikels.
- **Menge:** Artikel in Mengeneinheit.
- **Stück:** Stückzahl des Artikels.
- **Preis:** Gesamtpreis des Artikels.
- **Letzte Änderung am, von:** Datum der letzten Änderung am Buchungssatz und Name des Anwenders, der die letzte Buchung ausgeführt hat.

### Info-Lager-Blätter
**Infosystem > Blatt**

In diesem Dialog können Sie sich die Informationen zu den Glasblättern im Einzelblattkistenlager anzeigen lassen.

Zu diesem Dialog werden folgende Unterdialoge angezeigt:
- "Info-Lager-Blätter – Filterdialog" auf Seite E-88
- "Info-Lager-Blätter – Trefferliste" auf Seite E-89

#### Info-Lager-Blätter – Filterdialog
**Infosystem > Blatt**

*Abb. E-45: Info-Lager-Blätter - Filterdialog*

In diesem Dialog können Sie die Informationen zu den Glasblättern im Einzelblattkistenlager nach ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste angezeigt.
- "Info-Lager-Blätter - Trefferliste" auf Seite E-89
- **Blatt:** Nummer des Glasblattes.
- **Blattbezeichnung:** Bezeichnung des Glasblattes.
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Kiste:** Kistennummer.
- **Kistenbezeichnung:** Bezeichnung der Kiste.
- **Variante:** Abmessungen der Variante.
- **Farbe:** Farbvariante des Artikels.
- **Preis:** Stückpreis des Glasblattes.
- **Ausbeute:** Ausbeute des Glasblattes in Prozent.

#### Info-Lager-Blätter – Trefferliste
**Infosystem > Blatt > Filtern**

*Abb. E-46: Info-Lager-Blätter – Trefferliste*

In diesem Dialog werden die Ergebnisse der Suche nach Glasblättern im Einzelblattkistenlager angezeigt.

##### Trefferliste
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

### Info-Lager-Historie
**Infosystem > Historie**

In diesem Dialog können Sie die Informationen über die Lagerbuchungen anzeigen lassen.

Zu diesem Dialog werden folgende Unterdialoge angezeigt:
- "Info-Lager-Historie – Filterdialog" auf Seite E-91
- "Info-Lager-Historie – Trefferliste" auf Seite E-92
- "Info-Lager-Historie – Trefferliste-Details" auf Seite E-94

#### Info-Lager-Historie – Filterdialog
**Infosystem > Historie**

*Abb. E-47: Info-Lager-Historie – Filterdialog*

In diesem Dialog können Sie die Informationen über die Lagerbuchungen nach ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste angezeigt. Die Details können Sie in der Detailansicht einsehen.
- "Info-Lager-Historie - Trefferliste" auf Seite E-92
- "Info-Lager-Historie - Trefferliste-Details" auf Seite E-94
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Lieferant:** Lieferantennummer.
- **Auftrag:** Auftragsnummer.
- **Opti-Nr:** Die Job-Nummer für die Schnittstelle XTV wird nur angezeigt, wenn die Funktion entsprechend konfiguriert wurde.
- **Variante:** Maßvariante des Artikels.
- **Farbe:** Farbvariante des Artikels.
- **Stapel:** Stapelnummer.
- **Blattbez.:** Bezeichnung des Glasblattes.
- **Kiste:** Kistennummer.
- **Datum:** Datum, an dem der Buchungssatz gebucht wurde.
- **Anzahl:** Stückzahl des Artikels.
- **Menge:** Artikel in Mengeneinheit.
- **Preis:** Gesamtpreis des Artikels.
- **Kostenstelle:** Bezeichnung der Kostenstelle.
- **Status:** Status des aktuellen Satzes, z. B. Lagerausgang.

#### Info-Lager-Historie – Trefferliste
**Infosystem > Historie > Filtern**

*Abb. E-48: Info-Lager-Historie – Trefferliste*

In diesem Dialog werden die Ergebnisse der Suche nach Lagerbuchungen angezeigt. Die Details können Sie in der Detailansicht einsehen.
- "Info-Lager-Historie - Trefferliste-Details" auf Seite E-94
Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

##### Trefferliste
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Variante:** Maßvariante des Artikels.
- **Fach:** Bezeichnung des Fachs.
- **Stück:** Stückzahl des Artikels.
- **Menge:** Artikel in Mengeneinheit.
- **Preis:** Gesamtpreis des Artikels.
- **Status:** Status des aktuellen Satzes, z. B. Lagerausgang.
- **Datum:** Datum, an dem der Buchungssatz gebucht wurde.

Mit `<F2>` können Sie sich die folgenden Spalten anzeigen lassen:
- **Kiste:** Kistennummer.
- **VA:** Kennzeichen der Verpackungsart.
- **Lieferant:** Lieferantennummer.
- **Stapel:** Stapelnummer.
- **L-Preis:** Artikelpreis im Lager, wenn nach der LIFO-Buchungsmethode abgebucht und berechnet wird.
- **F-Preis:** Artikelpreis im Lager, wenn nach der FIFO-Buchungsmethode abgebucht und berechnet wird.
- **Auftr.:** Auftragsnummer.

#### Info-Lager-Historie – Trefferliste-Details
**Infosystem > Historie > Filtern > <F5>**

*Abb. E-49: Info-Lager-Historie – Trefferliste-Details*

In diesem Dialog werden die Details zur Trefferliste der Lagerbuchungen angezeigt.
Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

##### Details
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Kiste:** Kistennummer.
- **Verpackart:** Kennzeichen der Verpackungsart.
- **Lieferant:** Lieferantennummer.
- **Fach:** Bezeichnung des Fachs.
- **Blatt:** Nummer und Bezeichnung des Blattes.
- **Auftrag:** Auftragsnummer.
- **Opti-Nr:** Die Job-Nummer für die Schnittstelle XTV wird nur angezeigt, wenn die Funktion entsprechend konfiguriert wurde.
- **Kunde:** Kundennummer und Kundenname.
- **Variante:** Maßvariante des Artikels.
- **Farbe:** Farbvariante des Artikels.
- **Buchungsanzahl:** Stückzahl, die für diesen Buchungssatz gebucht wurde.
- **Buchungsmenge:** Gesamtmenge in Mengeneinheit, die gebucht wurde.
- **Buchungspreis:** Gesamtpreis der gebuchten Mengen.
- **LIFO-Preis:** Artikelpreis im Lager, wenn nach der LIFO-Buchungsmethode abgebucht und berechnet wird.
- **FIFO-Preis:** Artikelpreis im Lager, wenn nach der FIFO-Buchungsmethode abgebucht und berechnet wird.
- **Kostenstelle:** Bezeichnung der Kostenstelle.
- **Letzte Buchung am, von:** Datum der letzten Änderung am Buchungssatz und Name des Anwenders, der die letzte Buchung ausgeführt hat.
- **Bemerkung:** Zusätzliche Informationen aus der Lagereingangsbuchung.

### Aufträge/Bestellungen
**Infosystem > Aufträge/Bestellungen**

In diesem Dialog können Sie die Informationen zu auftrags- oder bestellbezogenen Buchungen anzeigen lassen.

Zu diesem Dialog werden folgende Unterdialoge angezeigt:
- "Aufträge/Bestellungen - Filterdialog" auf Seite E-96
- "Aufträge/Bestellungen - Trefferliste" auf Seite E-97
- "Aufträge/Bestellungen - Trefferliste-Details" auf Seite E-98

#### Aufträge/Bestellungen – Filterdialog
**Infosystem > Aufträge/Bestellungen**

*Abb. E-50: Aufträge/Bestellungen - Filterdialog*

In diesem Dialog können Sie die Informationen zu auftrags- oder bestellbezogenen Buchungen im Lager nach ausgewählten Kriterien filtern. Die Ergebnisse werden in einer Trefferliste angezeigt. Die Details können Sie in der Detailansicht einsehen.
- "Aufträge/Bestellungen - Trefferliste" auf Seite E-97
- "Aufträge/Bestellungen - Trefferliste-Details" auf Seite E-98
- **Auftrag:** Auftragsnummer oder Bestellnummer.
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Variante:** Nummer der Artikelvariante.
- **Farbe:** Nummer der Farbvariante.
- **Buchung:** Buchungsstatus des Auftrags oder der Bestellung.
  Folgende Optionen stehen zur Auswahl:
  - 0 = noch keine Buchung ausgeführt.
  - 1 = Teilbuchung einer Position ausgeführt.
  - 2 = Position komplett gebucht.
  - 3 = Auftrag oder Bestellung wurde komplett gebucht.
- **Datum:** Datum, an dem die Lagerbuchung zum Auftrag oder zur Bestellung ausgeführt wurde.

#### Aufträge/Bestellungen – Trefferliste
**Infosystem > Aufträge/Bestellungen > Filtern**

*Abb. E-51: Aufträge/Bestellungen - Trefferliste*

In diesem Dialog werden die Ergebnisse der Suche nach auftrags- oder bestellbezogenen Buchungen im Lager angezeigt. Die Details können Sie in der Detailansicht einsehen.
- "Aufträge/Bestellungen - Trefferliste-Details" auf Seite E-98
Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

##### Trefferliste
- **Auftrag:** Auftragsnummer oder Bestellnummer.
- **Position:** Nummer der Position im Auftrag oder in der Bestellung.
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Variante:** Nummer der Artikelvariante.
- **Anzahl:** Zu verbuchende Stückzahl pro Position.
- **Menge:** Buchungsmenge in der Mengeneinheit des Artikels.
- **Verbucht:** Buchungsanzahl in Stück, die gebucht wurde.
- **Datum:** Datum, an dem die Lagerbuchung zum Auftrag oder zur Bestellung ausgeführt wurde.

#### Aufträge/Bestellungen – Trefferliste-Details
**Infosystem > Aufträge/Bestellungen > Filtern > <F5>**

*Abb. E-52: Aufträge/Bestellungen - Trefferliste-Details*

In diesem Dialog werden die Details zur Trefferliste der auftrags- oder bestellbezogenen Buchungen im Lager angezeigt.
Mit `<F5>` wechseln Sie zwischen der Trefferliste und der Detailansicht der ausgewählten Position.

##### Details
- **Artikelnummer:** Artikelnummer und Artikelbezeichnung.
- **Lager:** Lagernummer.
- **Variante:** Nummer der Artikelvariante.
- **Farbe:** Nummer der Farbvariante.
- **Auftrag:** Auftragsnummer oder Bestellnummer.
- **Position:** Nummer der Position im Auftrag oder in der Bestellung.
- **Anzahl:** Zu verbuchende Stückzahl pro Position.
- **Menge:** Buchungsmenge in der Mengeneinheit des Artikels.
- **Buchung:** Buchungsstatus des Auftrags oder der Bestellung.
  Folgende Optionen stehen zur Auswahl:
  - 0 = noch keine Buchung ausgeführt.
  - 1 = Teilbuchung einer Position ausgeführt.
  - 2 = Position komplett gebucht.
  - 3 = Auftrag oder Bestellung wurde komplett gebucht.
- **Datum:** Datum, an dem die Lagerbuchung zum Auftrag oder zur Bestellung ausgeführt wurde.
- **Verbucht (Anzahl):** Verbuchte Stückzahl des Artikels.
- **Verbucht (Menge):** Verbuchte Menge in der Mengeneinheit des Artikels.
- **Erfasser (Mitarbeiter):** Erfassungsdatum und Mitarbeiter, der diese Buchung erfasst hat.
- **Verbucht (Mitarbeiter):** Buchungsdatum und Mitarbeiter, der diese Buchung durchgeführt hat.

### Buchungsstatus
**Infosystem > Buchungsstatus**

Im Buchungsstatus können Sie sich die Buchungsinformationen zu den Lagern anzeigen lassen, die nicht gebuchten oder fehlerhaften Buchungssätze enthalten oder Lager die sich gerade in der Inventur befinden. Im Dialog **Buchungsstatus – Korrektur** können Sie die Daten für den Buchungsstatus korrigieren.

Zu diesem Dialog werden folgende Unterdialoge angezeigt:
- "Buchungsstatus - Ungebucht" auf Seite E-100
- "Buchungsstatus – Fehler" auf Seite E-102
- "Buchungsstatus – Inventur" auf Seite E-103
- "Buchungsstatus - Korrektur" auf Seite E-104

#### Buchungsstatus – Ungebucht
**Infosystem > Buchungsstatus > Ungebucht**

*Abb. E-53: Buchungsstatus – Ungebucht*

In diesem Dialog können Sie sich Buchungsinformationen zu den Lagern anzeigen lassen, die nicht gebuchte Buchungssätze enthalten.

Sie können folgende Tastaturbefehle ausführen:
- Mit `<F5>` können Sie den Dialog **Buchungsstatus – Korrektur** aufrufen.
- Mit `<F2>` können Sie sich weitere Spalten anzeigen lassen.

##### Rumpfbereich
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
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

##### Fußbereich
Die Feldbeschreibungen entsprechen den Spaltenbeschreibungen des Dialogs.

#### Buchungsstatus – Fehler
**Infosystem > Buchungsstatus > Fehler**

*Abb. E-54: Buchungsstatus – Fehler*

In diesem Dialog können Sie sich Buchungsinformationen zu den Lagern anzeigen lassen, die fehlerhafte Buchungssätze enthalten. Im Dialog **Buchungsstatus - Korrektur** können Sie die Daten für den Buchungsstatus korrigieren.

Sie können folgende Tastaturbefehle ausführen:
- Mit `<F5>` können Sie den Dialog **Buchungsstatus – Korrektur** aufrufen.
- Mit `<F2>` können Sie sich weitere Spalten anzeigen lassen.

##### Rumpfbereich
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
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

##### Fußbereich
Die Feldbeschreibungen entsprechen den Spaltenbeschreibungen des Dialogs.

#### Buchungsstatus – Inventur
**Infosystem > Buchungsstatus > Inventur**

*Abb. E-55: Buchungsstatus – Inventur*

In diesem Dialog können Sie sich Buchungsinformationen zu den Lager anzeigen lassen, die nicht gebuchten oder fehlerhaften Buchungssätze enthalten oder Lager die sich gerade in der Inventur befinden. Im Dialog **Buchungsstatus – Korrektur** können Sie die Daten für den Buchungsstatus korrigieren.

Sie können folgenden Tastaturbefehl ausführen:
- Mit `<F5>` können Sie den Dialog **Buchungsstatus – Korrektur** aufrufen.

##### Rumpfbereich
- **Lager:** Lagernummer des Lagers, das zur Inventur freigeschaltet ist.
- **Bezeichnung:** Bezeichnung des Lagers in Inventur.
- **Datum:** Datum, an dem das Lager zur Inventur vorbereitet wurde.
- **Mitarbeiter:** Mitarbeiternummer des Mitarbeiters, der das Lager zur Inventur vorbereitet hat.

#### Buchungsstatus – Korrektur
**Infosystem > Buchungsstatus > Ungebucht, Fehler, Inventur > <F5>**

*Abb. E-56: Buchungsstatus – Korrektur*

In diesem Dialog können Sie die Daten des Buchungsstatus der folgenden Dialoge korrigieren:
- Buchungsstatus – Ungebucht
- Buchungsstatus – Fehler
- Buchungsstatus – Inventur

##### Rumpfbereich
- **Artikel:** Artikelnummer und Artikelbezeichnung.
- **Lager:** Lagernummer und Lagerbezeichnung.
- **Lieferant:** Lieferantennummer und Lieferantenname.
- **Kiste:** Kistennummer und Kistenbezeichnung.
- **Fach:** Bezeichnung des Fachs im Fachlager.
- **Auftrag:** Auftragsnummer, bei auftragsbezogenen Lagerbuchungen.
- **Variante:** Maßvariante des Artikels.
- **Farbe:** Nummer der Artikelfarbe.
- **Buchungsanzahl:** Gebuchte Menge in Stück.
- **Buchungsmenge:** Gebuchte Menge in der entsprechenden Mengeneinheit.
- **Buchungspreis:** Gesamtpreis der Artikel.
- **verbucht am:** Datum der letzten Buchung des aktuellen Buchungssatzes.
- **von:** Name des Mitarbeiters, der den aktuellen Buchungssatz zuletzt gebucht hat.

##### Fußbereich
- **Artikel:** Artikelbezeichnung.
- **Lager:** Lagerbezeichnung.
- **Fehler:** Fehlerstatus im Klartext.
- **Status:** Status der aktuellen Buchung im Klartext, z. B. Lagerausgang.

### Lagerinformationen – Pickliste
**Infosystem > Auftragsliste**

*Abb. E-57: Lagerinformationen – Pickliste*

In diesem Dialog können Sie sich die auftragsbezogenen Lagerartikel anzeigen lassen. Für die Ausgabe der Lagerinformationen der Pickliste wird die Adhoc-SQL Gruppe 1 und die SQL-Abfrage 26 verwendet. Bei Bedarf muss diese Abfrage separat angepasst werden. Die Abfrage können Sie über `<Strg>` + `<F4>` > SQL-Abfragen > Ändern anpassen.
- **Auftrag:** Auftragsnummer, für die die Pickliste erstellt wird.

### Lagerinformationen – Trefferliste
**Infosystem > Auftragsliste > Filtern**

*Abb. E-58: Lagerinformationen – Trefferliste*

In diesem Dialog wird Ihnen die Trefferliste für auftragsbezogene Lagerartikel angezeigt.

#### Trefferliste
- **Artikel:** Artikelnummer.
- **Bezeichnung:** Artikelbezeichnung.
- **Farbe:** Bezeichnung der Farbvariante des Artikels.
- **Variante:** Abmessungen der Artikelvariante.
- **Menge:** Stückzahl des Artikels.
- **Auftrag:** Auftragsnummer.
- **Spalten ohne Namen:** Positionsnummer im Auftrag.

### LVR-Status
**Infosystem > LVR-Status**

*Abb. E-59: SQL-Abfragen - Lagerverwaltungsrechner (LVR)*

Dieser Dialog wird zur Zeit nicht genutzt.

### Reichweite – Bestandsprognose
**Infosystem > Reichweite**

*Abb. E-60: Reichweite - SQL-Abfragen*

In diesem Dialog können Sie sich die Bestandsprognose für Lagerartikel anzeigen lassen. Für die Ausgabe der Bestandsprognose der Reichweite wird die Adhoc-SQL Gruppe 1 und die SQL-Abfrage 21 verwendet. Bei Bedarf muss diese Abfrage separat angepasst werden. Die Abfrage können Sie über `<Strg>` + `<F4>` > SQL-Abfragen > Ändern anpassen.
- **Von Artikel:** Startwert für den Wertebereich der Artikelnummer, um die Trefferliste zu filtern.
- **Bis Artikel:** Maximalwert für den Wertebereich der Artikelnummer, um die Trefferliste zu filtern.
- **Von Lager:** Startwert für den Wertebereich der Lagernummer, um die Trefferliste zu filtern.
- **Bis Lager:** Maximalwert für den Wertebereich der Lagernummer, um die Trefferliste zu filtern.

### Reichweite – Trefferliste
**Infosystem > Reichweite > Filtern**

*Abb. E-61: Reichweite - Trefferliste*

In diesem Dialog wird Ihnen anhand von Lagerbuchungen eine Prognose angezeigt, für wie viele Monate der aktuelle Bestand des Lagerartikels für die Produktion ausreicht.

#### Trefferliste
- **Artikel:** Artikelnummer.
- **Bestand:** Aktueller Lagerbestand des Artikels.
- **Verbrauch:** Verbrauch des Artikels in der Vergangenheit.
- **Reichweite (Mon):** Geschätzte Zeit in Monaten, die der Artikel noch auf Lager zur Verfügung steht.

### Dispositiver Bestand
**Infosystem > Dispositiver Bestand**

*Abb. E-62: Dispositiver Bestand*

In diesem Dialog können Sie sich den aktuellen Lagerbestand des Artikels, die bestellten, verplanten und verfügbaren Mengen des Lagerartikels anzeigen lassen.

#### Kopfbereich
- **Datum:** Filterkriterium nach Datum.
- **Artikel:** Filterkriterium für die Artikelnummer.
- **Variante:** Filterkriterium für die Maßvariante.

#### Rumpfbereich
- **Variante:** Maßvariante des Artikels.
- **Lager:** Lagernummer des Lagers, in dem der Artikel eingelagert ist.
- **Bezeichnung:** Bezeichnung des Lagerartikels.
- **Bestand:** Aktueller Bestand des Lagerartikels.
- **Bestellt:** Aktuell bestellte Menge des Lagerartikels.
- **Verplant:** Aktuell verplante Menge des Lagerartikels, z. B. für die Produktion.
- **Verfügbar:** Aktuell verfügbare Menge des Lagerartikels.

#### Fußbereich
- **Gesamtsumme:** Summierter Wert jeweils für eine Spalte. Folgende Spalten werden aufsummiert angezeigt:
  - Bestand
  - Bestellt
  - Verplant
  - Verfügbar

### Bestandsprognose
**Infosystem > Prognose**

*Abb. E-63: Bestandsprognose*

In diesem Dialog können Sie sich für einen ausgewählten Zeitraum die Prognose für den Lagerbestand des Artikels anzeigen lassen. Verplante Bestände entstehen durch erfasste Aufträge. Die Prognose zeigt den Lagerbestand aufgrund von im System vorhandenen Aufträgen und bereits bestehenden Bestellungen.
Die Unter- oder Überdeckung der Lagerbestände kann durch definierte Alarmbestände verhindert werden.
- "Artikelstammdaten Lager" auf Seite E-51
Mit `<Shift>` + `<F5>` lassen Sie sich für den ausgewählten Artikel die Bestandsprognose in der grafischen Übersicht anzeigen.

#### Kopfbereich
- **Artikel:** Artikelnummer für die gefilterte Auflistung.
- **Lager:** Lagernummer. Wenn in diesem Feld kein Eintrag erfolgt, wird eine lagerübergreifende Bestandsprognose erstellt.
- **Variante:** Maßvariante des Artikels.
- **Datum:** Zeitraum der Bestandsprognose.
- **Periode:** Zeitabstände in der Bestandsprognose.

#### Rumpfbereich
Die Spalten sind im Kopfbereich beschrieben. Zusätzlich werden folgende Spalten angezeigt:
- **Datum:** Datumsangabe für die Bestandsprognose zu verplanten, bestellten und zu dem Zeitpunkt auf Lager vorhandenen Artikeln.
- **Verplant:** Verplante Artikel aus dem Lager, zu dem entsprechend in der ersten Spalte angezeigten Datum.
- **Bestellt:** Bestellte Artikel für das Lager, zu dem entsprechend in der ersten Spalte angezeigten Datum.
- **Bestand:** Bestand des Artikels auf Lager, zu dem entsprechend in der ersten Spalte angezeigten Datum.

## Druck

Im Druck können Sie Informationen über die Lagerdaten oder Etiketten drucken. Sie können das Seitenlayout für den Listendruck oder die Etiketten frei definieren.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Kistenetiketten drucken" auf Seite E-112
- "Listendruck" auf Seite E-113

### Kistenetiketten drucken
**Druck > Etiketten**

*Abb. E-64: Kistenetiketten drucken*

In diesem Dialog können Sie sich die offenen Druckaufträge für Kistenetiketten anzeigen lassen und drucken.
Mit `<Shift>` + `<F3>` starten Sie den Etikettendruck.
- **Kiste:** Kistennummer.
- **Anzahl:** Stückzahl der Artikel in der Kiste.
- **Artikel:** Artikelnummer.
- **Variante:** Maßvariante des Artikels.
- **Lager:** Lagernummer.
- **Kost. St.:** Bezeichnung der Kostenstelle.
- **Spalte ohne Bezeichnung:** Anzeige für den Etikettendruck:
  - J = Etiketten drucken.
  - N = Keine Etiketten drucken.
- **Anz.:** Anzahl der zu druckenden Etiketten.
- **Erfasst:** Datum, an dem der Kisteneingang erfasst wurde.
- **Gedruckt:** Datum, an dem das Etikett der Kiste zuletzt ausgedruckt wurde.

### Listendruck
**Druck > Listendruck**

*Abb. E-65: Listendruck*

Der Dialog ist ausführlich an folgender Stelle beschrieben:
- Verkauf, "Listendruck" auf Seite D-162

## Systemverwaltung

In der Systemverwaltung können Sie die Lagerprotokolle und die Preiskorrekturen der Lagerartikel verwalten.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Lagerprotokoll löschen" auf Seite E-114
- "Lager-Preiskorrektur" auf Seite E-114

### Lagerprotokoll löschen
**System > Lagerprotokoll löschen**

*Abb. E-66: Lagerprotokoll löschen*

In diesem Dialog können Sie ein Lagerprotokoll im System löschen.
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Variante:** Maßvariante des Artikels.
- **Farbe:** Farbvariante des Artikels.

### Lager-Preiskorrektur
**System > Preiskorrektur**

*Abb. E-67: Lager-Preiskorrektur*

In diesem Dialog können Sie den Durchschnittspreis für eingekaufte Lagerartikel korrigieren. Fehlerhafte Preisbuchungen für Lagerartikel verfälschen den Durchschnittspreis in der Statistik und können nur über den Höchstpreis und den Niedrigstpreis korrigiert werden.
- **Artikel:** Artikelnummer.
- **Lager:** Lagernummer.
- **Variante:** Maßvariante des Artikels.
- **Farbe:** Farbvariante des Artikels.
- **Höchstpreis:** Höchster Einkaufspreis der Variante im Lager.
- **Niedrigstpreis:** Niedrigster Einkaufspreis der Variante im Lager.

## Servicefunktionen

Servicefunktionen werden nur auf Anforderung durch den Servicemitarbeiter der A+W Software GmbH ausgeführt.

Die Servicefunktionen finden Sie an folgender Stelle:
- Versandsteuerung, "Servicefunktionen" auf Seite E-90

## Partindex

### Index

**A**
- **Artikelbestand**
  - Fachlager korrigieren E-67
  - Gestelllager korrigieren E-69
  - Kistenlager korrigieren E-66
  - Standardlager korrigieren E-63
  - Stapellager korrigieren E-68
- **Artikelstammdaten**
  - Bestandsgrenzen für Lagerartikel E-51
- **Aufträge/Bestellungen**
  - Infosystem E-96, E-97, E-98

**B**
- **Bestände anzeigen**
  - Artikelvarianten E-75, E-76, E-77
  - Blätter E-88, E-89
  - Lagerartikel E-71, E-72, E-73
  - Lagerfächer E-79, E-80, E-81
  - Lagergestelle E-82, E-83, E-84
  - Lagerhistorie E-91, E-92, E-94
  - Lagerstapel E-85, E-86, E-87
- **Bestandsbewertung**
  - Fachlager E-67
  - Gestelllager E-69
  - Kistenlager E-66
  - Standardlager E-63
  - Stapellager E-68
- **Bestandsgrenzen für Lagerartikel**
  - Artikelstammdaten E-51
- **Bestandsprognose**
  - Infosystem E-110
- **Buchung**
  - Auftragsbezug, mit E-45
  - Fachlager E-29, E-34
  - Gestelllager E-38, E-41
  - Kistenlager E-23, E-28
  - Standardlager E-16, E-22
  - Stapellageränderung E-36
  - Stapellagereingang E-35
- **Buchungskorrektur**
  - offene Buchungen bearbeiten E-47, E-48
- **Buchungsstatus**
  - Fehler E-102
  - Inventur E-103
  - Korrektur E-104
  - nicht gebuchte Buchungssätze E-100

**D**
- **Dispositiver Bestand**
  - Infosystem E-109
- **Druck**
  - Kistenetiketten E-112
  - Listen E-113

**F**
- **Fachlager**
  - Artikelbestand korrigieren E-67
  - Ausgänge buchen E-34
  - Eingänge buchen E-29
  - Inventur E-58

**G**
- **Gestelllager**
  - Artikelbestand korrigieren E-69
  - Ausgänge buchen E-41
  - Eingänge buchen E-38
  - Inventur E-60

**I**
- **Info-Lager-Artikel**
  - Bestände anzeigen E-71, E-72, E-73
- **Info-Lager-Blätter**
  - Bestände anzeigen E-88, E-89
- **Info-Lager-Fächer**
  - Bestände anzeigen E-79, E-80, E-81
- **Info-Lager-Gestelle**
  - Bestände anzeigen E-82, E-83, E-84
- **Info-Lager-Historie**
  - Bestände anzeigen E-91, E-92, E-94
- **Info-Lager-Stapel**
  - Bestände anzeigen E-85, E-86, E-87
- **Info-Lager-Varianten**
  - Bestände anzeigen E-75, E-76, E-77
- **Infosystem**
  - Aufträge/Bestellungen E-96, E-97, E-98
  - Bestandsprognose E-110
  - Buchungsstatus, Fehler E-102
  - Buchungsstatus, Inventur E-103
  - Buchungsstatus, Korrektur E-104
  - Buchungsstatus, nicht gebuchte Buchungssätze E-100
  - Dispositiver Bestand E-109
  - Reichweite Bestand E-108
- **Inventur**
  - Fachlager E-58
  - Gestelllager E-60
  - Kistenlager E-56
  - Standardlager E-53
  - Stapellager E-59

**K**
- **Kistenetiketten**
  - Druck E-112
- **Kistenlager**
  - Artikelbestand korrigieren E-66
  - Ausgänge buchen E-28
  - Eingänge buchen E-23
  - Inventur E-56

**L**
- **Lagerartikel**
  - Preiskorrektur E-114
- **Lagerausgang**
  - auftragsbezogen buchen E-45
  - buchen E-22
- **Lagereingang**
  - buchen E-16
- **Lagerinformationen**
  - Pickliste E-106
  - SQL-Abfragen E-105
- **Lagerprotokoll**
  - löschen E-114
- **Lagerraumverwaltung**
  - Lagerräume, neu anlegen E-50
- **Listendruck**
  - drucken E-113
- **Löschen**
  - Lagerprotokoll E-114

**M**
- **Menüs** E-9

**P**
- **Pickliste**
  - Lagerinformationen E-106
- **Preiskorrektur**
  - Lagerartikel E-114

**R**
- **Reichweite**
  - Infosystem E-108
  - SQL-Abfragen E-107

**S**
- **SQL-Abfragen**
  - Lagerinformationen E-105
  - Reichweite Bestand E-107
- **Standardlager**
  - Artikelbestand korrigieren E-63
  - Ausgänge buchen E-22
  - Eingänge buchen E-16
  - Inventur E-53
- **Stapellager**
  - Änderungen buchen E-36
  - Artikelbestand korrigieren E-68
  - Ausgänge buchen E-36
  - Eingang buchen E-35
  - Inventur E-59
