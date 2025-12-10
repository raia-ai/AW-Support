---
title: "DE_AWBusiness_Fertigung_5_7"
source: "DE_AWBusiness_Fertigung_5_7.pdf"
tags: ["A+W Business", "Fertigung", "Versandsteuerung", "Ladelisten", "Sprossenkonstruktion", "Stücklisten", "Software-Referenz", "ERP", "Produktionsplanung"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "A software reference manual for the A+W Business Fertigung module, version 5.11. This document details functionalities related to shipping control (Versandsteuerung), including creating and managing loading lists (Ladelisten), and provides information on legacy features in the appendix, such as parts lists (Stücklisten) and glazing bar construction (Sprossenkonstruktion)."
long_description: "This document serves as a detailed software reference for the 'A+W Business Fertigung' (Production) module, specifically version 5.11/01-2018. It guides users through various functionalities within the manufacturing and logistics processes. The main section focuses on 'Versandsteuerung' (Shipping Control), explaining how to create, manage, and print 'Ladelisten' (loading lists) for freight forwarders. It covers the necessary prerequisites, data entry in the 'Versandinfo' and 'Aufträge' tabs, and menu functions for printing lists and labels. The document includes an extensive appendix ('Anhang') that describes legacy modules and functions no longer included in new installations but potentially present in updated systems. These legacy features include 'Produktion' (Production) with its 'Stücklisten-Ansicht' (Parts List View) and the detailed 'Sprossenkonstruktion' (Glazing Bar Construction) module, which has since been replaced by CAD Designer (Bars). The appendix provides a comprehensive look at the user interface, settings, and operational steps for these older functions. The manual concludes with a thorough alphabetical index ('Partindex') for quick reference to specific terms and features within the Fertigung module."
---

# Softwarereferenz Versandsteuerung

---
## Ladelisten

**Pfad:** `Fertigung > Versandsteuerung > Ladelisten`

Sie können für Ihren Spediteur Ladelisten pro Kunde zusammenstellen. Dabei muss entweder in allen Aufträgen der Empfänger oder der Rechnungsempfänger identisch sein.

> **Voraussetzung**
> Sie können eine Ladeliste nur speichern, wenn Sie einen Spediteur ausgewählt haben. Spediteure werden als Lkws in den Stammdaten hinterlegt.

In diesem Dialog finden Sie folgende Register:
- "Ladeliste - Versandinfo" auf Seite E-302
- "Ladeliste - Aufträge" auf Seite E-304

### Menü Funktionen

**Pfad:** `Fertigung > Versandsteuerung > Ladelisten > Menü Funktionen`

Über dieses Menü können Sie den Druck starten. Die Einträge sind nur freigeschaltet, wenn die angezeigte Ladeliste gespeichert ist.

- **Ladeliste drucken:**
  Öffnet den Dialog Formular-/Etikettendruck im Druckmodus Frachtliste. Eine ausführliche Beschreibung finden Sie im Part Verkauf.
  → Verkauf, "Formular-/Etikettendruck - Formulare" auf Seite C-634
- **Etiketten drucken:**
  Öffnet den Dialog Formular-/Etikettendruck im Druckmodus Etiketten. Eine ausführliche Beschreibung finden Sie im Part Verkauf.
  → Verkauf, "Formular-/Etikettendruck - Etiketten" auf Seite C-640

## Ladeliste – Versandinfo

**Pfad:** `Fertigung > Versandsteuerung > Ladelisten > Register Versandinfo`

*Abb. E-151 Ladeliste - Versandinfo*

In diesem Register geben Sie die Details zu der Ladeliste an, für die Sie die Aufträge zusammengestellt haben.

> **Änderungen werden zurückgeschrieben**
> Wenn Sie die Lieferanschrift und/oder den Rechnungsempfänger ändern, werden diese Angaben in alle Aufträge zurückgeschrieben, die in der Ladeliste aufgeführt sind.

### Versandangaben

**Ladeliste**
Die Nummer der Ladeliste wird vom System hochgezählt. Im Auswahlmodus können Sie eine gespeicherte Ladeliste aufrufen.

**Datum**
Das Tagesdatum ist vorbelegt. Sie können es überschreiben.

**Gewicht**
Das Gewicht wird standardmäßig auf 0 gesetzt.

**Menge**
Die Menge wird standardmäßig auf 0 gesetzt.

**Bemerkung**
Sie können eine Anmerkung eintragen.

**Versender**
Versender ist immer der Kunde, für den die Aufträge angelegt wurden.

**Empfänger**
Der Lieferungsempfänger muss für alle Dokumente der Ladeliste identisch sein. Der neue Empfänger wird in alle Dokumente der Ladeliste zurückgeschrieben.

**Rechnungsempfänger**
Sie müssen den Rechnungsempfänger auswählen, wenn die Rechnung nicht an die Lieferanschrift und nicht an den Kunden geschickt werden soll. Der neue Empfänger wird in alle Dokumente der Ladeliste zurückgeschrieben.

**Spediteur**
Sie müssen einen Spediteur auswählen. Nur die Spediteure werden zur Auswahl angeboten, die in den Stammdaten hinterlegt sind. Eine Beschreibung finden Sie im Part Stammdaten.
→ Stammdaten, "Lkw" auf Seite B-858

### Versandtext
Sie können einen Text aus den hinterlegten Texten auswählen oder einen eigenen Text einfügen. Der Text wird auf der Ladeliste gedruckt.

**Nummer**
Sie können das Textkennzeichen eingeben oder den gewünschten Text suchen. Den gewählten Text können Sie im Anzeigefeld modifizieren.

## Ladeliste – Aufträge

**Pfad:** `Fertigung > Versandsteuerung > Ladelisten > Register Aufträge`

*Abb. E-152 Ladeliste - Aufträge*

In diesem Register sammeln Sie die Aufträge und/oder Teillieferungen eines Kunden, die zu einer Ladeliste zusammengestellt werden sollen. Die Felder sind nur freigeschaltet, wenn Sie eine neue Ladeliste beginnen.

> **Ladeliste speichern**
> Sie können die Ladeliste nur speichern, wenn der Empfänger in allen zusammengestellten Aufträgen identisch ist.
> Sie können die Ladeliste erst speichern, wenn Sie im Register Versandinfo die Pflichtfelder gefüllt haben.

### Aufträge

**[Hinzufügen]**
Öffnet den Dialog Dokumente suchen, um einen weiteren Auftrag hinzuzufügen.

> **Abweichende Anschrift**
> Wenn Sie einen Auftrag mit einer anderen Liefer- oder Rechnungsanschrift einfügen, macht eine Meldung Sie auf diesen Unterschied aufmerksam.
> Sie können den Auftrag dennoch in der Liste lassen und im Register Versandinfo die entsprechende Anschrift eintragen. Sie können den Auftrag aber auch wieder aus der Liste löschen, wenn er versehentlich hineingeraten ist.
> Änderungen und Löschen sind nur möglich, solange die Liste noch nicht gespeichert ist. Wenn Sie eine gespeicherte Liste ändern wollen, müssen Sie sie ganz löschen und neu anlegen.

**Ziel-Nummernverwalter**
Die gesammelten Aufträge werden automatisch in einen Nummernverwalter kopiert, damit die Ladeliste gedruckt werden kann. Wenn Sie einen neuen Namen eintragen, wird der Nummernverwalter angelegt.

In der Übersicht werden alle Positionen der ausgewählten Aufträge aufgelistet:

- **Auftrag:**
  Nummer des Auftrags.
- **Pos.:**
  Positionsnummer im Auftrag.
- **Menge, Gewicht:**
  Stückzahl und Gesamtgewicht der Position.
- **Breite, Höhe:**
  Maße der Position.
- **Bezeichnung:**
  Bezeichnung des Produkts.
- **Rechnungsempfänger:**
  Ein Rechnungsempfänger ist nur eingetragen, wenn die Rechnungsadresse sich von der Lieferadresse unterscheidet, z. B. bei Lieferungen an eine Filiale.
- **Empfänger:**
  Ein Empfänger ist nur eingetragen, wenn im Auftrag eine Lieferanschrift eingetragen ist.

**Gesamt Menge**
Gesamtsumme aller aufgeführten Positionen.

**Gesamt Gewicht**
Gesamtgewicht aller aufgeführten Positionen.

**Tabelle**
In der Übersicht sind Ladelisten aufgeführt. Sie können die Listen prüfen, drucken oder löschen.

# Anhang

## Übersicht

In diesem Kapitel sind Dialoge und Funktionen beschrieben, die bei der Neuinstallation von A+W Business nicht mehr enthalten sind. Bei der Aktualisierung früherer Installationen (Update) werden diese Programmteile nicht überschrieben oder deinstalliert.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Produktion" auf Seite E-310
- "Sprossenkonstruktion" auf Seite E-312

## Produktion

In diesem Abschnitt finden Sie Beschreibungen zu Dialogen und Funktionen aus dem Modul Fertigung, die ab der Programmversion 4.4 nicht mehr neu installiert werden.

### Stücklisten-Ansicht

**Pfad:** `Fertigung > Produktion > Stücklisten-Ansicht`

*Abb. E-153 Stücklisten-Ansicht*

In diesem Dialog können Sie sich die Stückliste eines Auftrags und/oder einer Auftragsposition anzeigen lassen.

### Einstellungen (Stücklistenansicht)

**Pfad:** `Fertigung > Produktion > Stkl.-Ansicht > Menü Optionen > Einstellungen`

*Abb. E-154 Gestellbelegung – Einstellungen für Texte*

In diesem Dialog können Sie die Darstellung von Texten in der Stücklistenansicht festlegen.

**Anzuzeigende Texte**
Zur Auswahl werden alle Textarten angeboten, die in den Stammdaten eingerichtet sind. Texte der ausgewählten Textart werden in der Stücklistenansicht angezeigt.

**Schrift**
Durch die Auswahl der Größe und einer der Optionen Normal oder Fett, legen Sie fest, wie die Texte dargestellt werden.

## Sprossenkonstruktion

**Pfad:** `Fertigung > Produktion > Sprossenkonstruktion`

Sie können sich alle Aufträge mit Sprossen anzeigen lassen und die Maße berechnen, die in der Positionserfassung des Auftrags nicht angezeigt werden. Außerdem können Sie maßstäbliche Skizzen der Sprossenkonstruktion in Rechteckscheiben drucken.

> **Modul durch CAD Designer (Bars) ersetzt**
> Die Funktionen des Moduls Sprossenkonstruktion sind ab Release 2011 vollständig durch CAD Designer (Bars) ersetzt.
> In früheren Versionen steht die Funktion nur mit der Gupta-Datenbank zur Verfügung.

Zu dieser Funktion stehen Ihnen folgende Dialoge zur Verfügung:
- "NV-Sprossenkonstruktion" auf Seite E-314
- "Sprossenkonstruktion (Dialog)" auf Seite E-316
- "Einstellungen (Sprossen)" auf Seite E-319
- "Sonderkonstruktionen" auf Seite E-320
- "Teilberechnung" auf Seite E-321

### Menüs in der Sprossenkonstruktion

**Pfad:** `Fertigung > Produktion > Sprossenkonstruktion`

Über die Menüs der Sprossenkonstruktion können Sie die Vorgaben festlegen und andere Dialoge öffnen.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Einstellungen" auf Seite E-313
- "Menü Sprossentypen" auf Seite E-313
- "Menü Dokument" auf Seite E-313

### Menü Einstellungen

**Pfad:** `Fertigung > Produktion > Sprossenkonstruktion`

Über dieses Menü öffnen Sie die Dialoge für die Vorgaben und ordnen die Sprossen oder Bohrpunkte symmetrisch an.

- **Einstellungen:**
  Öffnet den gleichnamigen Dialog, um die Vorgaben für Bohrungen und Schnitte festzulegen.
  → "Einstellungen (Sprossen)" auf Seite E-319
- **Sonderkonstr.:**
  Öffnet den gleichnamigen Dialog, um Vorgaben für Gehrungsschnitte festzulegen.
  → "Sonderkonstruktionen" auf Seite E-320
- **Teilberechnung:**
  Öffnet den gleichnamigen Dialog, um Vorgaben für die Felder festzulegen.
  → "Teilberechnung" auf Seite E-321
- **Symmetrie senkrecht, waagerecht:**
  Ordnet die senkrechten und/oder waagerechten Sprossen symmetrisch an.
- **G_Schnitt senkrecht, waagerecht:**
  Gehrungsschnitte
- **BP spiegeln senkrecht, waagerecht:**
  Spiegelt die Bohrpunkte der senkrechten und/oder waagerechten Sprosse.

### Menü Sprossentypen

**Pfad:** `Fertigung > Produktion > Sprossenkonstruktion`

Über dieses Menü öffnen Sie den Stammdatendialog, in dem die Sprossentypen hinterlegt sind. Eine Beschreibung finden Sie im Part Stammdaten.
→ Stammdaten, "Konstruktionstypen der Sprossen" auf Seite B-162

### Menü Dokument

**Pfad:** `Fertigung > Produktion > Sprossenkonstruktion`

Über dieses Menü speichern Sie Änderungen in der Auftragsposition.

- **Bohrpunkte sichern:**
  Speichert nach Änderungen die neuen Bohrpunkte.
- **Austrags-Position:**
  Öffnet in der Auftragsposition den Dialog Sprossen, in dem Sie die Sprossen bearbeiten können. Eine Beschreibung finden Sie im Part Stammdaten.
  → Verkauf, "Positionen - Sprossen" auf Seite C-492

### NV-Sprossenkonstruktion

**Pfad:** `Fertigung > Produktion > Sprossenkonstruktion`

*Abb. E-155 NV-Sprossenkonstruktion*

In diesem Dialog werden alle Aufträge des gewählten Nummernverwalters angezeigt, in denen Sprossen angegeben sind. Von der Übersicht aus können Sie sich die Sprossenkonstruktion eines Auftrags anzeigen lassen und die Maße für die Produktion bearbeiten. Ggf. notwendige Änderungen können in die Auftragsposition zurückgespeichert werden, sofern die entsprechenden Felder angezeigt werden (abhängig von A+W Business-Version).

> **Modul durch CAD Designer (Bars) ersetzt**
> Die Funktionen des Moduls Sprossenkonstruktion sind ab Release 2011 vollständig durch CAD Designer (Bars) ersetzt.
> In früheren Versionen steht die Funktion nur mit der Gupta-Datenbank zur Verfügung.

#### Selektion nach

**Mitarbeiter**
Name des Mitarbeiters, der sich in A+W Business angemeldet hat.

**Nummernverwalter**
Auswahl des Nummernverwalters, auf den der Dialog zugreifen soll.

#### Ausgabe auf
Mit der Wahl der Option legen Sie fest, wie der Druck ausgegeben werden soll:
- **Drucker:** Der Druckauftrag wird an einen Drucker gesendet.
- **Bildschirm:** Der Druckauftrag wird auf den Bildschirm gesendet.

#### Alle
Sie können festlegen, ob alle Aufträge im gewählten Nummernverwalter gedruckt werden sollen.
- Nur der markierte Auftrag wird gedruckt.
- Alle Aufträge werden gedruckt. Die Ausgabe auf dem Bildschirm kann immer nur einen Auftrag darstellen.

#### Modelle als Rechteck
Modellskizzen können als Rechteck oder mit ihrer tatsächlichen Form gedruckt werden. Diese Einstellung übersteuert die Angaben aus dem Auftrag und aus den Stammdaten.
- Modellskizzen werden so gedruckt, wie es im Auftrag angegeben ist, z. B. maßstäblich.
- Modellskizzen werden als Rechteck gedruckt.

#### Dokumente
In der Übersicht sind alle Aufträge aufgelistet, die im gewählten Nummernverwalter sind.

### Sprossenkonstruktion (Dialog)

**Pfad:** `Fertigung > Produktion > Sprossenkonstruktion > Auswahl eines Auftrags`

Die Sprossendaten werden aus der jeweiligen Auftragsposition übernommen. Sie können sie bei Bedarf verändern, z. B. mehrere unterschiedliche Sprossenbreiten erfassen.

Im Dialog Sprossenkonstruktion finden Sie folgende Register:
- Sprossenkonstruktion – Grafik
- Sprossenkonstruktion – Info

#### Sprossenkonstruktion – Grafik

**Pfad:** `Fertigung > Produktion > Sprossenkonstruktion > Auswahl eines Auftrags > Grafik`

*Abb. E-156 Sprossenkonstruktion – Grafik*

In diesem Register können Sie sich die Sprossenkonstruktion anschauen und eine Skizze drucken.
Die Anzeige der Ziffern innerhalb der Sprossen können Sie nach Bedarf ein- und ausblenden. Die Ziffern geben an, welche Sprossen vom Typ und Maß her gleich sind.
→ "Ziffern auf Skizze" auf Seite E-319

**Auftrag/Pos**
In diesen Feldern werden die Nummern des Auftrags und der Position angezeigt, zu der die Skizze gehört.

**Extra Window**
Sie können sich eine Vergrößerung der Skizze in einem gesonderten Dialog anzeigen lassen.
- Die Skizze wird in dem Darstellungsbereich des aktuellen Dialogs angezeigt.
- Die Skizze wird in einem neuen Dialog vergrößert angezeigt. Diese Darstellung ist sinnvoll, wenn Sie sehr viele Maße ablesen wollen. Um zur Standarddarstellung zurückzukehren, minimieren Sie die Vergrößerung und deaktivieren die Checkbox.

**Ausgabe**
Sie können die Skizze an einen Drucker senden, als RTF- oder als PDF-Datei speichern. Der Pfad der gespeicherten Datei wird angezeigt.

**Funktionen**
**[Stopfen integrieren]**
Mit dieser Schaltfläche werden die Randstopfen in die Berechnung integriert, z. B. damit die angrenzenden lichten Sprossenfelder alle gleich groß sind.

**[Neuberechnung]**
Mit dieser Schaltfläche werden die Maße in der Skizze neu berechnet und aktualisiert.

**[1/100mm - 1/10mm]**
Mit dieser Schaltfläche können Sie die Maßanzeige einstellen. Nach der Umstellung müssen Sie die Anzeige mit [Neuberechnung] aktualisieren.

#### Sprossenkonstruktion – Info

**Pfad:** `Fertigung > Produktion > Sprossenkonstruktion > Auswahl eines Auftrags > Info`

*Abb. E-157 Sprossenkonstruktion – Info*

In diesem Register können Sie Details für die Produktion der Sprossen prüfen.
Im oberen Bereich werden der Name des Kunden und der Name des Produkts angezeigt. Rechts daneben sind die Stückzahl und die Modellmaße angegeben.

**Bohrpunkte senkrechte, waagerechte Sprossen**
In diesen Feldern sind die Bohrpunkte für die senkrechten und die waagerechten Sprossen angegeben.

**Zuschnittsinfo**
In diesem Bereich werden Detailinformationen für die Produktion angezeigt. Dazu gehören der Sprossentyp und die Anzahl und Länge der einzelnen Sprossenstäbe.

### Einstellungen (Sprossen)

**Pfad:** `Fertigung > Produktion > Sprossenkonstruktion > Auswahl eines Auftrags > Menü Einstellungen > Einstellungen`

*Abb. E-158 Einstellungen für Sprossenkonstruktionen*

In diesem Dialog legen Sie die Vorgaben für die Konstruktion der Sprossen fest. Einen Überblick über Sprossenkonstruktionen finden Sie im Part Stammdaten.
→ Stammdaten, "Konstruktionstypen der Sprossen" auf Seite B-162

#### Vorgaben

**Kennzeichen für Durchgang**
Mit dieser Einstellung legen Sie fest, welche Sprossen durchgängig sein sollen.
Wenn Sie 0 (null) wählen, werden die Sprossen beider Richtungen gesägt. Sie können dann zusätzlich festlegen, ob die Sprossen stumpf aufeinander treffen sollen, oder ob Gehrungen geschnitten werden sollen.
Wenn Sie 3 (beide) wählen, werden die Sprossen übereinander gelegt.

**Bohrpunkte**
Mit der Wahl der Option legen Sie fest, wie die Bohrpunkte berechnet werden sollen.
- **Absolut:** Jeder Bohrpunkt wird von derselben Ecke aus gemessen.
- **Relativ:** Jeder Bohrpunkt wird vom vorigen Bohrpunkt aus gemessen.

**Ziffern auf Skizze**
Sie können festlegen, ob die Ziffern der Sprossen in der Skizze angezeigt werden.
- Die Ziffern zur Unterscheidung der Sprossen und Sprossenabschnitte werden nicht angezeigt.
- Die Ziffern werden angezeigt. Sie sind als rote Zahlen den Sprossen zugeordnet. Diese Einstellung ist hilfreich, wenn Sie sehr umfangreiche Konstruktionen vorliegen haben.

**Feldmaße anzeigen**
Sie können festlegen, ob die Maße der Felder in der Skizze angezeigt werden.
- Die Feldmaße werden nicht angezeigt.
- Die Feldmaße sind im jeweiligen Feld angezeigt. Diese Einstellung ist hilfreich, wenn Sie die Bohrpunkte so setzen wollen, dass die Felder symmetrisch sind.

### Sonderkonstruktionen

**Pfad:** `Fertigung > Produktion > Sprossenkonstruktion > Auswahl eines Auftrags > Menü Einstellungen > Sonderkonstr.`

*Abb. E-159 Vorgaben für Sonderkonstruktionen*

In diesem Dialog können Sie festlegen, wie die Bohrpunkte und die Gehrungen berechnet werden sollen.

**Waagerecht, senkrecht, V-Sprossen**
In diesen Feldern tragen Sie ein, ob die Bohrungen feldsymmetrisch oder bohrpunktsymmetrisch berechnet werden sollen.
Wenn Sie >1 eintragen, werden die Bohrpunkte nicht neu berechnet. Eine Darstellung der Berechnungsarten finden Sie im Part Stammdaten.
→ Verkauf: Tutorial, “Sprossenkonstruktion" auf Seite C-71

### Teilberechnung

**Pfad:** `Fertigung > Produktion > Sprossenkonstruktion > Auswahl eines Auftrags > Menü Einstellungen > Teilberechnung`

*Abb. E-160 Teilberechnung*

In diesem Dialog legen Sie fest, zwischen welchen Sprossen die Felder gleich groß sein sollen.

# Partindex

## Index Fertigung

### A
- **A+W Business 6 Interface Service**
  - Einstellungen E-80
- **Abladestelle**
  - Kundenkommission E-265
  - Zuordnung E-266
- **Ablaufschema der Versandorganisation** E-18
- **Angebot**
  - an Produktion übergeben E-55
  - Optimierung E-53, E-290
- **Angebotsoptimierung** E-290
- **Ansicht** E-310
  - Stücklisten E-310
- **Anwenderstatus**
  - für Fertigung prüfen E-95
- **Artikel**
  - Export von Stammdaten (Zoll) E-289
- **Auflösungstiefe**
  - Terminübersicht E-273
- **Auftrag**
  - an Produktion übergeben E-37
  - Dummy-Kiste zuweisen E-150
  - Gestell zuordnen E-102
  - kalkulatorische Frachtkosten anzeigen E-144
  - nach Übergabe ändern E-26
  - Produktionsdaten E-199
  - Produktionsrückmeldungen E-69
  - Produktionsübergabe stornieren E-39
  - Status scannen E-99
  - Status umsetzen E-218
  - versandfertig melden E-99
- **Aufträge**
  - zusammenstellen (Versand) E-292
- **Auftragsstatus**
  - manuell umsetzen E-97
- **Auswärtig**
  - Gestell mahnen E-251
- **Auswärtiges Gestell, Ausgang**
  - Gestell E-244
- **Automatisch**
  - Gestell anlegen E-242
- **AWDesign**
  - Schnittstelle E-176

### B
- **Barcode**
  - Positionsübergabe E-194
  - Scanvorlage herstellen E-103
  - Status umsetzen E-99
- **Barcodeübergabe**
  - Details E-195
  - Prüfziffer E-196
- **BDE**
  - Statusmeldungen E-99
- **Beladung**
  - Gewicht E-231
  - Liste drucken E-113
- **Bestellung**
  - Produktionsübergabe E-26
- **Betriebsdatenerfassung** siehe BDE
- **Bezugsschein**
  - Zollverwaltung E-283
- **Buchung**
  - Aggregate (Produktionsdaten) E-202

### D
- **Dateilose Produktionsrückmeldungen** E-75
- **Datenformate**
  - Rückmeldedateien E-60
- **Datenübergabe**
  - an Produktion E-21
  - OrderXML E-22
- **Definition**
  - Vorschauspalten E-280

### E
- **Eingang**
  - Gestell E-247
- **Einstellungen**
  - A+W Business 6 Interface Service E-80
  - für automatische Produktionsübergabe E-32
  - für dateilose Produktionsrückmeldung E-71
  - für Produktionsübergabe prüfen (A+W Business-Kapazitätsplanung) E-45
  - für Produktionsübergabe prüfen (A+W Production Capacity Planner) E-51
  - für Produktionsübergabe prüfen (Aufträge) E-46
  - für Produktionsübergabe prüfen (ohne Kapa) E-33
  - Gestellbelegung E-190
  - kalkulatorische Frachtkosten E-141
  - KAPS-Datei E-215
  - Produktionsübergabe E-174
  - Produktionsübergabe mit A+W Business-Kapazitätsplanung E-44
- **Produktionsübergabe mit A+W Production Capacity Planner** E-48
- **Produktionsübergabe ohne Kapa** E-31
- **Produktionsübergabe von Angeboten** E-54
- **Rückmeldungen aus der Produktion** E-66
- **Sprossenkonstruktion** E-319
- **Statusmeldung** E-223
- **Stücklistenansicht** E-311
- **Empfangsbetätigungsliste** E-233
- **Entfernungspauschale** E-85
- **Erfassungsstelle**
  - A+W Production-Beispiele E-60
  - für dateilose Rückmeldung prüfen E-71
  - für Fertigmeldung zuordnen E-65
  - für Produktionsauftrag zuweisen E-133
  - für Produktionsrückmeldungen E-62
  - für Rückmeldung aus Produktionsauftrag E-132
  - zuordnen E-63
- **ERP-Webservice** E-176
- **Export**
  - Artikelstammdaten (Zollverwaltung) E-289
  - Terminübersicht E-275

### F
- **Fahrer**
  - anlegen E-108
  - Empfangsbestätigungsliste drucken E-113
  - Kommissionierung E-228
  - Stammdaten anlegen E-108
- **Fahrzeug**
  - Beladung zusammenstellen E-109
  - Beladungsliste drucken E-113
  - Stammdaten anlegen E-107
  - Zuladung E-106
- **Fertigung**
  - Anwenderstatus prüfen E-95
  - Statuszuordnung prüfen E-96
  - Übersicht erstellen E-121
- **Fertigungsübersicht** siehe Terminübersicht
- **Fertigungsvorschau**
  - Funktionsprinzip E-161
  - Geschäftsarten E-281
  - Spaltendefinition E-280
- **Firmendaten**
  - Einstellung für dateilose Rückmeldung E-73
  - Erfassungsstelle für Fertigmeldung E-65
- **Frachtkosten**
  - anzeigen E-143
  - Berechnung E-140
  - Einstellungen für kalkulatorische Frachtkosten E-141
- **Pauschale in Tour** E-85
- **Speditionskosten** E-145

### G
- **Geschäftsarten**
  - Ausschluss aus der Vorschau E-281
- **Gesperrt**
  - Gestell E-242
- **Gestell**
  - Art E-254
  - Ausgang E-244
  - auswärtig E-251
  - automatisch angelegt E-242
  - Beladungsliste drucken E-113
  - Eingang E-247
  - Gestellübersicht E-256
  - Gestellverwaltung E-241
  - Historie E-248
  - Mahnstufe zurücksetzen E-259
  - Mahnung E-250
  - manuell zuordnen E-102
  - Packliste in Versandsteuerung E-298
  - sperren E-242
  - Übersicht Partner E-257
  - umbuchen E-258
  - verloren E-242
  - Wert E-254
  - Zubehör E-254
- **Gestellarten** E-254
- **Gestellausgabe**
  - Listendruck E-236
- **Gestellauswahl**
  - manuelle Packmittelzuordnung E-224
- **Gestellbelegung**
  - Einstellungen E-190
  - Liste E-233
  - nach Auftrag E-260
  - nach Gestell E-262
  - prüfen E-188
- **Gestellbelegungsliste** E-233
- **Gestell-Packliste** E-298
- **Gestelltransfer** E-231
- **Gestellübersicht** E-256
- **Gestellverwaltung**
  - Gestelle E-240
  - Kundenkommission E-264
- **Gewicht**
  - Lkw-Beladung E-231
- **Grafik**
  - Sprossenkonstruktion E-316

### H
- **Handlungsablauf**
  - Fertigung und Versand E-19
- **Historie**
  - Gestell E-248

### I
- **Interface-Service** E-80
- **Intervall für Workflow-Task** E-28

### K
- **Kalkulatorische Frachtkosten**
  - anzeigen E-143
  - Einstellungen E-141
- **Kapazitäten**
  - pro Liefertermin anzeigen E-126
- **Kapazitätsübersicht**
  - Vorschau E-126
  - Warengruppen E-276
- **Kiste**
  - im Warenausgang erfassen E-150
  - Reservierung E-150
  - Reservierung prüfen E-150
  - Warenausgang E-153
- **Kisten-ID** E-149
- **Kommissionierung**
  - Auslieferung planen E-106
  - Ergebnis drucken E-113
  - Fahrer anlegen E-108
  - Fahrzeug anlegen E-107
  - Fahrzeugbeladung zusammenstellen E-109
  - Gestelltransfer E-231
  - Lieferbedingung E-229
  - Listendruck E-233
  - Optionen E-232
  - Zeilenumbruch E-232
  - zugeladenes Gewicht E-231
- **Kundenkommissionen** E-264
  - Abladestelle E-265
  - Zuordnung E-266

### L
- **Ladeliste**
  - Aufträge E-304
  - drucken E-113
  - für eigenen Fuhrpark E-113
  - speichern (Versandsteuerung) E-304
  - Versandinfo E-302
- **Versandsteuerung** E-301
- **Zollverwaltung** E-283
- **Lagerbestand**
  - nach Produktionsauftrag aktualisieren E-137
  - Reservierung E-149
- **Lieferbedingung**
  - Kommissionierung E-229
- **Liefertermin**
  - in Tourenliste ändern E-89
  - Kapazitäten anzeigen E-126
- **Lieferung**
  - Lkw E-228
- **Liste**
  - Beispiel Transportmittelbelegung E-234
  - drucken E-113
  - Empfangsbestätigung E-233
  - Gestellausgabe E-236
  - Gestellbelegung E-233
  - Kommissionierung E-233
  - Nummer zurücksetzen (Zollverwaltung) E-286
  - Tourenliste drucken E-91
  - Tourenliste zusammenstellen E-87
  - Transportmittel E-233
  - Zollverwaltung E-282
- **Lkw**
  - anlegen E-107
  - Kommissionierung E-228

### M
- **Mahnung**
  - für Gestelle zurücksetzen E-259
  - Gestell E-250
- **Manuelle Packmittelzuordnung**
  - Gestellauswahl E-224
  - Statusmeldung E-222
- **Materialien**
  - für Lieferzeitraum anzeigen E-121
- **Menü-Übersicht** E-16
- **Modellliste** E-187

### O
- **Online-Produktionsübersicht** E-75
- **Optimierung**
  - Angebot E-55
- **Optionen**
  - Kommissionierung E-232
  - Statusmeldung E-223
  - Terminübersicht E-268
- **OrderXML** E-22

### P
- **Packliste**
  - Versandsteuerung E-298
- **Packmittel**
  - manuell zuordnen E-102
- **Partner**
  - auswärtige Gestelle E-257
  - Gestell umbuchen E-258
- **Position**
  - Gestell zuordnen E-102
  - manuelle Packmittelzuordnung E-222
  - Status prüfen E-69
  - Statusmeldung E-220
  - versandfertig melden E-101
- **Positionsübergabe**
  - Barcode E-194
  - Details E-195
  - Übersicht E-194
- **Produktgruppe**
  - Zollverwaltung E-286
- **Produktion** E-169
  - Auftrag übergeben E-37
  - automatische Übergabe an AWCapacity Planner E-176
  - Lagerartikel E-131
  - Rückmeldungen E-66, E-80
  - Übergabe E-170
  - Übergabe an CAD Designer E-176
  - Übergabe Angebot E-170
  - Übergabe Einstellungen E-174
  - Übergabe ERP-Webservice E-176
- **Produktionsauftrag**
  - buchen E-137
  - Daten für Fertigmeldung erfassen E-134
  - fertig melden E-134
  - Rückmeldungen E-132
- **Produktionsdaten**
  - Auftrag E-199
  - Buchung E-202
- **Produktionsrückmeldungen**
  - Arten E-58
  - Einstellung für dateilose Rückmeldungen E-73
  - Einstellung für Online-Meldung E-71
  - im Auftrag prüfen E-69
  - Kapazitätsplanung E-78
  - online E-75
  - Rückmeldedateien E-60
- **Produktionsübergabe**
  - Angebot E-290
  - Angebot zur Optimierung übergeben E-55
  - Auftrag mit Bestellungen E-26
  - Auftrag stornieren E-39
  - Auftrag übergeben E-37
  - Einstellungen für Übergabe mit A+W Business-Kapazitätsplanung E-44
  - Einstellungen für Übergabe mit A+W Production Capacity Planner E-48
  - für Angebote einrichten E-54
  - geänderte Auftragsposition E-26
  - Globale Einstellungen E-175
  - OrderXML E-22
  - Positionen E-193
  - schematischer Ablauf E-23
  - spezielle Einstellungen E-184
  - Storno E-22
  - Texte und Anlagen E-186
  - Überblick E-18
  - Übergabeparameter E-177
  - Varianten E-21
  - Voreinstellungen (Firmendaten) prüfen E-31
  - Workflow-Task E-26
- **Produktionsübersicht**
  - online E-75
  - per Rückmeldedateien E-69
- **Prüfziffer für Barcode** E-196

### R
- **Reihenfolge**
  - Statusmeldung E-99, E-218
- **Reservierung**
  - Kiste E-149
  - prüfen E-150
- **Rückmeldedatei**
  - A+W Production-Dateien E-60
  - im Schnittstellen-Dienst E-66
- **Rückmeldung**
  - Gestell (BDE) E-160
- **Rückmeldungen**
  - aus der Produktion E-58, E-66, E-80
  - Dateiformate E-60
  - Einstellung für dateilose Rückmeldungen E-71
  - Erfassungsstellen E-62
  - für Produktionsauftrag E-132
  - im Schnittstellen-Dienst einrichten E-66

### S
- **Scannen**
  - Barcode-Vorlage herstellen E-103
  - Status für Auftrag E-99
  - Status für Auftragsposition E-101
- **Schnittstelle**
  - Einstellungen für Rückmeldedateien E-66
  - Rückmeldungen aus Produktion einstellen E-66
  - Zolldaten E-287
- **Sonderkonstruktion** E-320
- **Speditionskosten**
  - verteilen E-145
- **Sperrkennzeichen**
  - in Stammdaten E-86
- **Sprossenkonstruktion**
  - Einstellungen E-319
  - Grafik E-316
  - Info E-318
  - Neuberechnung E-317
  - Nummernverwalter E-314
  - Sonderkonstruktion E-320
  - Teilberechnung E-321
- **Stammdaten**
  - Status für Fertigung prüfen E-95
  - Statuszuordnung für Fertigung prüfen E-96
  - Tour einrichten E-84
- **Status**
  - Einstellung für manuelle Statusumsetzung E-98
  - für Auftragsposition scannen E-101
  - manuell fertigmelden E-97
  - manuell für Versand umsetzen E-99
  - manuell umsetzen E-99
  - nach Produktionsrückmeldung prüfen E-69
  - scannen E-99
  - Zuordnung für Fertigung prüfen E-96
- **Statusmeldung**
  - manuelle Packmittelzuordnung E-222
  - manuelle Statusumsetzung E-99
  - Status per Scanner umsetzen E-99
- **Statusmeldung und Packmittelzuordnung** E-218
- **Statusmeldungen** E-216
  - Auftrag E-218
  - Einstellung E-98
  - Einstellungen E-223
  - Optionen E-223
  - Packmittelzuordnung E-218
  - Position E-220
  - Reihenfolge der Eingabe E-99, E-218
- **Statuspunkt für Rückmeldung zuordnen** E-63
- **Stückliste**
  - Auflösung für Zollverwaltung E-286
- **Stücklistenansicht** E-310
  - Einstellungen E-311

### T
- **Tastatur-Scanner**
  - Statusvergabe per Scanner E-97
- **Teilberechnung** E-321
- **Teillieferung** E-299
- **Terminübersicht** E-267, E-268
  - Auflösungstiefe E-273
  - Auswertungskriterien für Materialbedarf E-118
  - erstellen E-121
  - Exportieren E-275
  - Kapazitätsübersicht E-276
  - Materialien anzeigen E-121
- **Tour**
  - ändern E-89
  - anlegen E-84
  - Beladungsliste drucken E-113
  - einrichten E-84
  - Fahrzeugbeladung zusammenstellen E-109
  - Frachtkosten E-85
  - Konzept von Touren E-83
  - planen E-87
  - Speditionskosten verteilen E-145
  - sperren E-86
- **Tourenliste** E-204
  - Auflösungstiefe E-208
  - Auswahl E-207
  - Beispiel E-213
  - drucken E-91
  - Einstellungen KAPS E-215
  - Liefertermin ändern E-89
  - Querformat E-206
  - Selektion E-207
  - Tour ändern E-89
  - Touren/Liefertermin umsetzen E-214
  - Vorschau E-210
  - zusammenstellen E-87
- **Transport**
  - Versandsteuerung E-295
- **Transportmittelbeladungsliste** E-233
  - Voraussetzung E-113

### U
- **Überblick**
  - Produktionsübergabe, Versandorganisation E-18
- **Übergabe**
  - Angebot, Auftrag E-170
  - Produktion E-170
- **Übermengen** E-78

### V
- **Verfügbare Touren** E-208
- **Verloren**
  - Gestell E-242
- **Verpackung**
  - Versandsteuerung E-295
- **Versand** E-290
  - Auftrag fertigmelden E-99
  - Auftragsposition fertigmelden E-101
  - Fahrzeug Gesamtgewicht E-106
  - Handlungsablauf E-19
  - Tour anlegen E-84
  - Tour planen E-87
  - Versandaufträge löschen E-297
- **Versanddaten**
  - ändern E-214
- **Versandinfo**
  - Ladeliste E-294, E-302
- **Versandsteuerung**
  - Aufträge sammeln E-292
  - Gestell-Packliste E-298
  - Ladeliste E-301
  - per Spedition E-290
  - Teillieferung E-299
  - Verpackung, Transport E-295
  - Versand E-290
  - Versandauftrag löschen E-297
  - Versandinfo E-294
- **Vorschauspalten**
  - Definition E-280

### W
- **Warenausgang**
  - Kiste ausbuchen E-150
  - Kiste der Position zuweisen E-153
- **Warenausweis**
  - Zollverwaltung E-283
- **Workflow-Task**
  - Einstellungen für Produktionsübergabe prüfen E-27
  - Intervall festlegen E-28

### Z
- **Zollverwaltung** E-282
  - Datenexport E-287
  - Ladeliste E-283
  - Liste E-282, E-285
  - Listennummer zurücksetzen E-286
  - Produktgruppe E-286
- **Zollverwaltungslistennachweis** E-285
- **Zubehör**
  - Gestell E-254
