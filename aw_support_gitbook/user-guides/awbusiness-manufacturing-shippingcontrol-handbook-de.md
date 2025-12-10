---
title: "D-HB-AWBusiness_27"
source: "D-HB-AWBusiness_27.pdf"
tags: ["A+W Business", "ERP Software", "Manufacturing", "Shipping Control", "Warehouse Management", "Statistics", "German Technical Manual", "Glass Industry", "Windows and Doors", "Software Reference"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a comprehensive software reference manual for the A+W Business ERP system, focusing on the modules for Manufacturing (Fertigung), Statistics (Statistik), and Warehouse Management (Lagerwirtschaft). It details functionalities related to production and shipping control, data analysis, and inventory management."
long_description: "This extensive technical document serves as a detailed software reference guide for A+W Business, an ERP solution tailored for the glass, windows, and doors industry. The manual is structured into several key parts, each dedicated to a specific module of the software. Part E, 'Fertigung' (Manufacturing), covers shipping control functionalities, including processes for handling partial deliveries (Teillieferung) and creating loading lists (Ladelisten). It also describes legacy features like mullion construction (Sprossenkonstruktion), explaining how to manage, calculate, and visualize mullions in orders, noting that these functions have been superseded by the CAD Designer (Bars) module in newer versions. Part F, 'Statistik' (Statistics), provides an in-depth look at the software's data analysis and reporting capabilities. It outlines how to generate various sales and purchasing statistics, including order information, revenue analysis, and complaint statistics (Reklamationsstatistik). It details the creation of standard and 'Super' statistics, which allow for complex comparisons and data aggregation across different business units or time periods. Part G, 'Lagerwirtschaft' (Warehouse Management), functions as a tutorial and reference for inventory control. It covers the fundamental concepts of warehouse organization, from defining storage locations and categories to managing stock levels. The guide explains how to perform inventory transactions, conduct stocktakes (periodical and initial), manage warehouse articles within documents, and automate the reordering process. The document is intended for system administrators and power users who need to configure, manage, and utilize these advanced modules within the A+W Business environment."
---

# Softwarereferenz

---
## Teillieferung

**Fertigung > Versandsteuerung > Teillieferung**

*Abb. E-150: Übersicht – Teillieferungen*

In diesem Dialog können Sie sich anzeigen lassen, welche Aufträge in einem Nummernverwalter noch offene Mengen ausweisen.

### Identifikation

- **Mandant**: Wenn Sie mit unterschiedlichen Mandanten arbeiten, werden diese zur Auswahl angeboten.
- **Bereich**: Wenn in der Produktion mit verschiedenen Bereichen gearbeitet wird, können Sie denjenigen auswählen, dem die Aufträge zugeordnet sind.
- **Mitarbeiter**: Name des Mitarbeiters, der sich in A+W Business angemeldet hat.
- **Nummernverwalter**: Wenn Sie einen Nummernverwalter ausgewählt haben, werden alle Aufträge aufgelistet, die in diesem Nummernverwalter stehen.

### Ausgabe auf

Mit der Wahl der Option legen Sie die Ausgabe der Liste fest:

- **Drucker**: Die Liste wird an den Drucker gesendet.
- **Bildschirm**: Die Liste wird auf dem Bildschirm dargestellt.

## Übersicht

In der Übersicht werden alle Aufträge im gewählten Nummernverwalter angezeigt.

- **Dokument**: Auftragsnummer.
- **Pos**: Positionsnummer aus dem Auftrag.
- **Datum Lieferung**: Lieferdatum.
- **Breite, Höhe**: Breite und Höhe der Position.
- **Produkt Kunde**: Bei Kundenprodukten wird die Referenznummer angezeigt.
- **Produkt Nummer, Produkt Bezeichnung**: Nummer und Bezeichnung des Produkts in A+W Business.
- **Bestelltext/Kundenpos.**: Bestelltext oder Kundenposition aus dem Auftrag.
- **Menge original, Menge geliefert, Menge offen**: Gesamtmenge der Auftragsposition, davon gelieferte bzw. offene Menge.
- **Status Nummer, Status Bezeichnung**: Auftragsstatus.
- **Nummer Kunde, Name Kunde**: Nummer und Name des Kunden.

## Ladelisten

**Fertigung > Versandsteuerung > Ladelisten**

Sie können für Ihren Spediteur Ladelisten pro Kunde zusammenstellen. Dabei muss entweder in allen Aufträgen der Empfänger oder der Rechnungsempfänger identisch sein.

> **Voraussetzung**
> Sie können eine Ladeliste nur speichern, wenn Sie einen Spediteur ausgewählt haben. Spediteure werden als Lkws in den Stammdaten hinterlegt.

In diesem Dialog finden Sie folgende Register:
- "Ladeliste - Versandinfo" auf Seite E-2604
- "Ladeliste - Aufträge" auf Seite E-2606

### Menü Funktionen

**Fertigung > Versandsteuerung > Ladelisten > Menü Funktionen**

Über dieses Menü können Sie den Druck starten. Die Einträge sind nur freigeschaltet, wenn die angezeigte Ladeliste gespeichert ist.

- **Ladeliste drucken**: Öffnet den Dialog Formular-/Etikettendruck im Druckmodus Frachtliste. Eine ausführliche Beschreibung finden Sie im Part Verkauf.
  - Verkauf, "Formular-/Etikettendruck - Formulare" auf Seite C-1927
- **Etiketten drucken**: Öffnet den Dialog Formular-/Etikettendruck im Druckmodus Etiketten. Eine ausführliche Beschreibung finden Sie im Part Verkauf.
  - Verkauf, "Formular-/Etikettendruck - Etiketten" auf Seite C-1933

## Ladeliste – Versandinfo

**Fertigung > Versandsteuerung > Ladelisten > Register Versandinfo**

*Abb. E-151: Ladeliste - Versandinfo*

In diesem Register geben Sie die Details zu der Ladeliste an, für die Sie die Aufträge zusammengestellt haben.

> **Änderungen werden zurückgeschrieben**
> Wenn Sie die Lieferanschrift und/oder den Rechnungsempfänger ändern, werden diese Angaben in alle Aufträge zurückgeschrieben, die in der Ladeliste aufgeführt sind.

### Versandangaben

- **Ladeliste**: Die Nummer der Ladeliste wird vom System hochgezählt. Im Auswahlmodus können Sie eine gespeicherte Ladeliste aufrufen.
- **Datum**: Das Tagesdatum ist vorbelegt. Sie können es überschreiben.
- **Gewicht**: Das Gewicht wird standardmäßig auf 0 gesetzt.
- **Menge**: Die Menge wird standardmäßig auf 0 gesetzt.
- **Bemerkung**: Sie können eine Anmerkung eintragen.
- **Versender**: Versender ist immer der Kunde, für den die Aufträge angelegt wurden.
- **Empfänger**: Der Lieferungsempfänger muss für alle Dokumente der Ladeliste identisch sein. Der neue Empfänger wird in alle Dokumente der Ladeliste zurückgeschrieben.
- **Rechnungsempfänger**: Sie müssen den Rechnungsempfänger auswählen, wenn die Rechnung nicht an die Lieferanschrift und nicht an den Kunden geschickt werden soll. Der neue Empfänger wird in alle Dokumente der Ladeliste zurückgeschrieben.
- **Spediteur**: Sie müssen einen Spediteur auswählen. Nur die Spediteure werden zur Auswahl angeboten, die in den Stammdaten hinterlegt sind. Eine Beschreibung finden Sie im Part Stammdaten.
  - Stammdaten, "Lkw" auf Seite B-998

### Versandtext

Sie können einen Text aus den hinterlegten Texten auswählen oder einen eigenen Text einfügen. Der Text wird auf der Ladeliste gedruckt.

- **Nummer**: Sie können das Textkennzeichen eingeben oder den gewünschten Text suchen. Den gewählten Text können Sie im Anzeigefeld modifizieren.

## Ladeliste – Aufträge

**Fertigung > Versandsteuerung > Ladelisten > Register Aufträge**

*Abb. E-152: Ladeliste - Aufträge*

In diesem Register sammeln Sie die Aufträge und/oder Teillieferungen eines Kunden, die zu einer Ladeliste zusammengestellt werden sollen. Die Felder sind nur freigeschaltet, wenn Sie eine neue Ladeliste beginnen.

> **Ladeliste speichern**
> Sie können die Ladeliste nur speichern, wenn der Empfänger in allen zusammengestellten Aufträgen identisch ist.
> Sie können die Ladeliste erst speichern, wenn Sie im Register Versandinfo die Pflichtfelder gefüllt haben.

### Aufträge

- **[Hinzufügen]**: Öffnet den Dialog Dokumente suchen, um einen weiteren Auftrag hinzuzufügen.

> **Abweichende Anschrift**
> Wenn Sie einen Auftrag mit einer anderen Liefer- oder Rechnungsanschrift einfügen, macht eine Meldung Sie auf diesen Unterschied aufmerksam. Sie können den Auftrag dennoch in der Liste lassen und im Register Versandinfo die entsprechende Anschrift eintragen. Sie können den Auftrag aber auch wieder aus der Liste löschen, wenn er versehentlich hineingeraten ist. Änderungen und Löschen sind nur möglich, solange die Liste noch nicht gespeichert ist. Wenn Sie eine gespeicherte Liste ändern wollen, müssen Sie sie ganz löschen und neu anlegen.

- **Ziel-Nummernverwalter**: Die gesammelten Aufträge werden automatisch in einen Nummernverwalter kopiert, damit die Ladeliste gedruckt werden kann. Wenn Sie einen neuen Namen eintragen, wird der Nummernverwalter angelegt.

In der Übersicht werden alle Positionen der ausgewählten Aufträge aufgelistet:
- **Auftrag**: Nummer des Auftrags.
- **Pos.**: Positionsnummer im Auftrag.
- **Menge, Gewicht**: Stückzahl und Gesamtgewicht der Position.
- **Breite, Höhe**: Maße der Position.
- **Bezeichnung**: Bezeichnung des Produkts.
- **Rechnungsempfänger**: Ein Rechnungsempfänger ist nur eingetragen, wenn die Rechnungsadresse sich von der Lieferadresse unterscheidet, z. B. bei Lieferungen an eine Filiale.
- **Empfänger**: Ein Empfänger ist nur eingetragen, wenn im Auftrag eine Lieferanschrift eingetragen ist.

- **Gesamt Menge**: Gesamtsumme aller aufgeführten Positionen.
- **Gesamt Gewicht**: Gesamtgewicht aller aufgeführten Positionen.

### Tabelle

In der Übersicht sind Ladelisten aufgeführt. Sie können die Listen prüfen, drucken oder löschen.

# Anhang

## Übersicht

In diesem Kapitel sind Dialoge und Funktionen beschrieben, die bei der Neuinstallation von A+W Business nicht mehr enthalten sind. Bei der Aktualisierung früherer Installationen (Update) werden diese Programmteile nicht überschrieben oder deinstalliert.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Produktion" auf Seite E-2612
- "Sprossenkonstruktion” auf Seite E-2614

## Produktion

In diesem Abschnitt finden Sie Beschreibungen zu Dialogen und Funktionen aus dem Modul Fertigung, die ab der Programmversion 4.4 nicht mehr neu installiert werden.

### Stücklisten-Ansicht

**Fertigung > Produktion > Stücklisten-Ansicht**

*Abb. E-153: Stücklisten-Ansicht*

In diesem Dialog können Sie sich die Stückliste eines Auftrags und/oder einer Auftragsposition anzeigen lassen.

### Einstellungen (Stücklistenansicht)

**Fertigung > Produktion > Stkl.-Ansicht > Menü Optionen > Einstellungen**

*Abb. E-154: Gestellbelegung – Einstellungen für Texte*

In diesem Dialog können Sie die Darstellung von Texten in der Stücklistenansicht festlegen.

**Anzuzeigende Texte**
Zur Auswahl werden alle Textarten angeboten, die in den Stammdaten eingerichtet sind. Texte der ausgewählten Textart werden in der Stücklistenansicht angezeigt.

**Schrift**
Durch die Auswahl der Größe und einer der Optionen Normal oder Fett, legen Sie fest, wie die Texte dargestellt werden.

## Sprossenkonstruktion

**Fertigung > Produktion > Sprossenkonstruktion**

Sie können sich alle Aufträge mit Sprossen anzeigen lassen und die Maße berechnen, die in der Positionserfassung des Auftrags nicht angezeigt werden. Außerdem können Sie maßstäbliche Skizzen der Sprossenkonstruktion in Rechteckscheiben drucken.

> **Modul durch CAD Designer (Bars) ersetzt**
> Die Funktionen des Moduls Sprossenkonstruktion sind ab Release 2011 vollständig durch CAD Designer (Bars) ersetzt.
> In früheren Versionen steht die Funktion nur mit der Gupta-Datenbank zur Verfügung.

Zu dieser Funktion stehen Ihnen folgende Dialoge zur Verfügung:
- "NV-Sprossenkonstruktion" auf Seite E-2616
- "Sprossenkonstruktion (Dialog)" auf Seite E-2618
- "Einstellungen (Sprossen)" auf Seite E-2621
- "Sonderkonstruktionen" auf Seite E-2622
- "Teilberechnung" auf Seite E-2623

### Menüs in der Sprossenkonstruktion

**Fertigung > Produktion > Sprossenkonstruktion**

Über die Menüs der Sprossenkonstruktion können Sie die Vorgaben festlegen und andere Dialoge öffnen.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Einstellungen" auf Seite E-2615
- "Menü Sprossentypen" auf Seite E-2615
- "Menü Dokument" auf Seite E-2615

### Menü Einstellungen

**Fertigung > Produktion > Sprossenkonstruktion**

Über dieses Menü öffnen Sie die Dialoge für die Vorgaben und ordnen die Sprossen oder Bohrpunkte symmetrisch an.

- **Einstellungen**: Öffnet den gleichnamigen Dialog, um die Vorgaben für Bohrungen und Schnitte festzulegen.
  - "Einstellungen (Sprossen)" auf Seite E-2621
- **Sonderkonstr.**: Öffnet den gleichnamigen Dialog, um Vorgaben für Gehrungsschnitte festzulegen.
  - "Sonderkonstruktionen" auf Seite E-2622
- **Teilberechnung**: Öffnet den gleichnamigen Dialog, um Vorgaben für die Felder festzulegen.
  - "Teilberechnung" auf Seite E-2623
- **Symmetrie senkrecht, waagerecht**: Ordnet die senkrechten und/oder waagerechten Sprossen symmetrisch an.
- **G_Schnitt senkrecht, waagerecht**: Gehrungsschnitte
- **BP spiegeln senkrecht, waagerecht**: Spiegelt die Bohrpunkte der senkrechten und/oder waagerechten Sprosse.

### Menü Sprossentypen

**Fertigung > Produktion > Sprossenkonstruktion**

Über dieses Menü öffnen Sie den Stammdatendialog, in dem die Sprossentypen hinterlegt sind. Eine Beschreibung finden Sie im Part Stammdaten.
- Stammdaten, "Konstruktionstypen der Sprossen" auf Seite B-227

### Menü Dokument

**Fertigung > Produktion > Sprossenkonstruktion**

Über dieses Menü speichern Sie Änderungen in der Auftragsposition.

- **Bohrpunkte sichern**: Speichert nach Änderungen die neuen Bohrpunkte.
- **Austrags-Position**: Öffnet in der Auftragsposition den Dialog Sprossen, in dem Sie die Sprossen bearbeiten können. Eine Beschreibung finden Sie im Part Stammdaten.
  - Verkauf, "Positionen - Sprossen" auf Seite C-1770

## NV-Sprossenkonstruktion

**Fertigung > Produktion > Sprossenkonstruktion**

*Abb. E-155: NV-Sprossenkonstruktion*

In diesem Dialog werden alle Aufträge des gewählten Nummernverwalters angezeigt, in denen Sprossen angegeben sind. Von der Übersicht aus können Sie sich die Sprossenkonstruktion eines Auftrags anzeigen lassen und die Maße für die Produktion bearbeiten. Ggf. notwendige Änderungen können in die Auftragsposition zurückgespeichert werden, sofern die entsprechenden Felder angezeigt werden (abhängig von A+W Business-Version).

> **Modul durch CAD Designer (Bars) ersetzt**
> Die Funktionen des Moduls Sprossenkonstruktion sind ab Release 2011 vollständig durch CAD Designer (Bars) ersetzt.
> In früheren Versionen steht die Funktion nur mit der Gupta-Datenbank zur Verfügung.

### Selektion nach

- **Mitarbeiter**: Name des Mitarbeiters, der sich in A+W Business angemeldet hat.
- **Nummernverwalter**: Auswahl des Nummernverwalters, auf den der Dialog zugreifen soll.

### Ausgabe auf

Mit der Wahl der Option legen Sie fest, wie der Druck ausgegeben werden soll:
- **Drucker**: Der Druckauftrag wird an einen Drucker gesendet.
- **Bildschirm**: Der Druckauftrag wird auf den Bildschirm gesendet.

**Alle** Sie können festlegen, ob alle Aufträge im gewählten Nummernverwalter gedruckt werden sollen.
- ☐ Nur der markierte Auftrag wird gedruckt.
- ☑ Alle Aufträge werden gedruckt. Die Ausgabe auf dem Bildschirm kann immer nur einen Auftrag darstellen.

**Modelle als Rechteck** Modellskizzen können als Rechteck oder mit ihrer tatsächlichen Form gedruckt werden. Diese Einstellung übersteuert die Angaben aus dem Auftrag und aus den Stammdaten.
- ☐ Modellskizzen werden so gedruckt, wie es im Auftrag angegeben ist, z.B. maßstäblich.
- ☑ Modellskizzen werden als Rechteck gedruckt.

### Dokumente

In der Übersicht sind alle Aufträge aufgelistet, die im gewählten Nummernverwalter sind.

## Sprossenkonstruktion (Dialog)

**Fertigung > Produktion > Sprossenkonstruktion > Auswahl eines Auftrags**

Die Sprossendaten werden aus der jeweiligen Auftragsposition übernommen. Sie können sie bei Bedarf verändern, z. B. mehrere unterschiedliche Sprossenbreiten erfassen.
Im Dialog Sprossenkonstruktion finden Sie folgende Register:
- Sprossenkonstruktion – Grafik
- Sprossenkonstruktion – Info

### Sprossenkonstruktion – Grafik

**Fertigung > Produktion > Sprossenkonstruktion > Auswahl eines Auftrags > Grafik**

*Abb. E-156: Sprossenkonstruktion – Grafik*

In diesem Register können Sie sich die Sprossenkonstruktion anschauen und eine Skizze drucken.
Die Anzeige der Ziffern innerhalb der Sprossen können Sie nach Bedarf ein- und ausblenden. Die Ziffern geben an, welche Sprossen vom Typ und Maß her gleich sind.
- "Ziffern auf Skizze" auf Seite E-2621

**Auftrag/Pos** In diesen Feldern werden die Nummern des Auftrags und der Position angezeigt, zu der die Skizze gehört.
**Extra Window** Sie können sich eine Vergrößerung der Skizze in einem gesonderten Dialog anzeigen lassen.
- ☐ Die Skizze wird in dem Darstellungsbereich des aktuellen Dialogs angezeigt.
- ☑ Die Skizze wird in einem neuen Dialog vergrößert angezeigt. Diese Darstellung ist sinnvoll, wenn Sie sehr viele Maße ablesen wollen. Um zur Standarddarstellung zurückzukehren, minimieren Sie die Vergrößerung und deaktivieren die Checkbox.

**Ausgabe**
Sie können die Skizze an einen Drucker senden, als RTF- oder als PDF-Datei speichern. Der Pfad der gespeicherten Datei wird angezeigt.

**Funktionen**
- **[Stopfen integrieren]**: Mit dieser Schaltfläche werden die Randstopfen in die Berechnung integriert, z. B. damit die angrenzenden lichten Sprossenfelder alle gleich groß sind.
- **[Neuberechnung]**: Mit dieser Schaltfläche werden die Maße in der Skizze neu berechnet und aktualisiert.
- **[1/100mm - 1/10mm]**: Mit dieser Schaltfläche können Sie die Maßanzeige einstellen. Nach der Umstellung müssen Sie die Anzeige mit [Neuberechnung] aktualisieren.

### Sprossenkonstruktion – Info

**Fertigung > Produktion > Sprossenkonstruktion > Auswahl eines Auftrags > Info**

*Abb. E-157: Sprossenkonstruktion – Info*

In diesem Register können Sie Details für die Produktion der Sprossen prüfen.
Im oberen Bereich werden der Name des Kunden und der Name des Produkts angezeigt. Rechts daneben sind die Stückzahl und die Modellmaße angegeben.

- **Bohrpunkte senkrechte, waagerechte Sprossen**: In diesen Feldern sind die Bohrpunkte für die senkrechten und die waagerechten Sprossen angegeben.
- **Zuschnittsinfo**: In diesem Bereich werden Detailinformationen für die Produktion angezeigt. Dazu gehören der Sprossentyp und die Anzahl und Länge der einzelnen Sprossenstäbe.

### Einstellungen (Sprossen)

**Fertigung > Produktion > Sprossenkonstruktion > Auswahl eines Auftrags > Menü Einstellungen > Einstellungen**

*Abb. E-158: Einstellungen für Sprossenkonstruktionen*

In diesem Dialog legen Sie die Vorgaben für die Konstruktion der Sprossen fest. Einen Überblick über Sprossenkonstruktionen finden Sie im Part Stammdaten.
- Stammdaten, "Konstruktionstypen der Sprossen" auf Seite B-227

**Vorgaben**
- **Kennzeichen für Durchgang**: Mit dieser Einstellung legen Sie fest, welche Sprossen durchgängig sein sollen. Wenn Sie 0 (null) wählen, werden die Sprossen beider Richtungen gesägt. Sie können dann zusätzlich festlegen, ob die Sprossen stumpf aufeinander treffen sollen, oder ob Gehrungen geschnitten werden sollen. Wenn Sie 3 (beide) wählen, werden die Sprossen übereinander gelegt.
- **Bohrpunkte**: Mit der Wahl der Option legen Sie fest, wie die Bohrpunkte berechnet werden sollen.
  - **Absolut**: Jeder Bohrpunkt wird von derselben Ecke aus gemessen.
  - **Relativ**: Jeder Bohrpunkt wird vom vorigen Bohrpunkt aus gemessen.
- **Ziffern auf Skizze**: Sie können festlegen, ob die Ziffern der Sprossen in der Skizze angezeigt werden.
  - ☐ Die Ziffern zur Unterscheidung der Sprossen und Sprossenabschnitte werden nicht angezeigt.
  - ☑ Die Ziffern werden angezeigt. Sie sind als rote Zahlen den Sprossen zugeordnet. Diese Einstellung ist hilfreich, wenn Sie sehr umfangreiche Konstruktionen vorliegen haben.
- **Feldmaße anzeigen**: Sie können festlegen, ob die Maße der Felder in der Skizze angezeigt werden.
  - ☐ Die Feldmaße werden nicht angezeigt.
  - ☑ Die Feldmaße sind im jeweiligen Feld angezeigt. Diese Einstellung ist hilfreich, wenn Sie die Bohrpunkte so setzen wollen, dass die Felder symmetrisch sind.

### Sonderkonstruktionen

**Fertigung > Produktion > Sprossenkonstruktion > Auswahl eines Auftrags > Menü Einstellungen > Sonderkonstr.**

*Abb. E-159: Vorgaben für Sonderkonstruktionen*

In diesem Dialog können Sie festlegen, wie die Bohrpunkte und die Gehrungen berechnet werden sollen.

- **Waagerecht, senkrecht, V-Sprossen**: In diesen Feldern tragen Sie ein, ob die Bohrungen feldsymmetrisch oder bohrpunktsymmetrisch berechnet werden sollen. Wenn Sie >1 eintragen, werden die Bohrpunkte nicht neu berechnet. Eine Darstellung der Berechnungsarten finden Sie im Part Stammdaten.
  - Verkauf: Tutorial, “Sprossenkonstruktion" auf Seite C-1327

### Teilberechnung

**Fertigung > Produktion > Sprossenkonstruktion > Auswahl eines Auftrags > Menü Einstellungen > Teilberechnung**

*Abb. E-160: Teilberechnung*

In diesem Dialog legen Sie fest, zwischen welchen Sprossen die Felder gleich groß sein sollen.

# A+W Business Statistik

## Revisionsübersicht des Moduls:

| Datum | Änderung |
| :--- | :--- |
| 01-2017 | Produkt- und Firmennamen angepasst. |
| 06-2016 | Vollständige Überarbeitung |
| 01-2013 | Layout an A+W Business angepasst. |
| 09-2010 | Layout an Doku-Konzept 2010 angepasst. |
| 09-2008 | Abbildungen und Part-Nummer angepasst. |
| 08-2008 | Rechtschreibkorrekturen |
| 12-2003 | Struktureller Umbau auf Programmstruktur 4.0 |
| 08-2000 | Überarbeitung Statistik |
| 03-1998 | Ersterstellung |

Zu diesem Modul finden Sie folgende Kapitel:
⇨ Softwarereferenz

## Übersicht

A+W Business verfügt über verschiedene Auswertungsmöglichkeiten. Dabei wird, wie nachfolgend beschrieben, zwischen aktueller Auftragsbestandsauswertung, Umsatz-, Reklamations- und Provisionsstatistik unterschieden.

- "Verkaufsstatistiken" auf Seite F-2630
- "Einkaufsstatistiken" auf Seite F-2665
- "Provisionsstatistik" auf Seite F-2675
- "Intrastat Meldung" auf Seite F-2677

> **Systemeinstellungen**
> In den Firmendaten können Sie Details für die Übergabe der Aufträge und Bestellungen in die Statistik festlegen. Eine ausführliche Beschreibung finden Sie im Part Stammdaten.
> ⇨ Stammdaten, "Firmendaten - Archiv" auf Seite B-1104

## Verkaufsstatistiken

Die Statistik in A+W Business ist ein wichtiges Instrument für die Unternehmensanalyse. Sie erhalten Auswertungen über Ihre Kunden, Branchen, Produkte, Geschäftsbereiche, Vertreter, etc. Dazu wählen Sie aus, ob die Daten jahresweise oder monatsweise ausgewertet werden sollen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Auftragsinformation" auf Seite F-2630
- "Auswahl" auf Seite F-2641
- "Umsatz Verkauf" auf Seite F-2642
- "Superstatistik" auf Seite F-2653
- "Superstatistik – Export" auf Seite F-2655
- "Superstatistik - Import" auf Seite F-2656
- "Reklamationsstatistik Verkauf" auf Seite F-2657
- "Statistik nach Aufbau" auf Seite F-2658
- "Kunden nach AV-Bereich" auf Seite F-2663

### Auftragsinformation

**Statistik > Auftragsinfo**

In diesem Dialog werten Sie Ihren Auftragsbestand aus. Dabei können Sie zwischen den neuen Aufträgen, den an die Produktion übergebenen Aufträgen und den fakturierten Aufträgen unterscheiden.

In diesem Dialog finden Sie folgende Register:
- "Auftragsinfo – Optionen" auf Seite F-2632
- "Auftragsinfo – Erfasst" auf Seite F-2636
- "Auftragsinfo - Produziert" auf Seite F-2637
- "Auftragsinfo - Fakturiert" auf Seite F-2638
- "Auftragsinfo – Offen" auf Seite F-2639
- "Auftragsinfo – Grafik" auf Seite F-2640

### Menü Drucken

**Statistik > Auftragsinfo**

Über dieses Menü starten Sie den Druck der Auswertung auf dem Bildschirm oder dem Drucker:

- **Standard**: Öffnet den Dialog Auswahl, um festzulegen, welche Daten gedruckt werden sollen.
  - "Auswahl" auf Seite F-2641
- **Umsatz**: Startet den Druck der Umsatzdaten und der Vergleichdaten des Vorjahres. In der tabellarischen Gegenüberstellung werden die Arbeitstage pro Monat angegeben. Die Aufstellung schließt mit den Werten für den durchschnittlichen Umsatz pro Arbeitstag.

### Auftragsinfo – Optionen

**Statistik > Auftragsinfo > Register Optionen**

*Abb. F-1: Auftragsinfo - Optionen*

In diesem Register legen Sie die Auswahlkriterien und die Ausgabeeinstellungen fest. Das Ergebnis der Suche wird in den Registern Erfasst, Produziert, Fakturiert und Offen ausgegeben.

#### Spalten

Über die Checkboxen legen Sie die Spalten fest, die in den Registern angezeigt werden sollen.
- **Menge**: Gesamtmenge aller Aufträgspositionen im gewählten Zeitraum.
- **Fläche**: Gesamtfläche aller Auftragspositionen.
- **LFM**: Gesamtlänge aller Kanten.
- **EK**: Gesamtsumme EK.
- **VK**: Gesamtsumme VK.
- **Rohgewinn**: Rohgewinn als absoluter Wert.
- **Rohgewinn %**: Rohgewinn als prozentualer Wert.
- **DB 1**: Deckungsbeitrag 1 als absoluter Wert. Im Bereich Selektionskriterien werden die Optionen für den Deckungsbeitrag freigeschaltet.
- **DB 1%**: Deckungsbeitrag 1 als prozentualer Wert. Im Bereich Selektionskriterien werden die Optionen für den Deckungsbeitrag freigeschaltet.
- **DB 2**: Deckungsbeitrag 2 als absoluter Wert. Im Bereich Selektionskriterien werden die Optionen für den Deckungsbeitrag freigeschaltet.
- **DB 2%**: Deckungsbeitrag 2 als prozentualer Wert. Im Bereich Selektionskriterien werden die Optionen für den Deckungsbeitrag freigeschaltet.

Für alle oben aufgeführten Checkboxen gilt:
- ☐ Die Spalte wird nicht angezeigt.
- ☑ Die Spalte wird angezeigt.

#### Selektionskriterien

In diesem Bereich legen Sie die Auswahlkriterien fest.

- **Tag, Monat, Jahr, Kalenderwoche, Quartal**: Mit der Wahl einer Option legen Sie den Betrachtungszeitraum fest. Die Optionen Jahr und Quartal sind gesperrt, wenn Sie im Bereich Aufschlüsselung nach die Checkbox Aufträge markiert haben. Wenn Sie die Auflistung nach Zeitraum wählen, wird die Auswahl entsprechend eingeschränkt.
- **Auswahl Datum**: Mit dieser Einstellung schränken Sie den Betrachtungszeitraum auf ein bestimmtes Datum ein.
- **Klassifikator**: Nur die Klassifikatoren stehen zur Wahl, die übergreifend für alle Partner und/oder Kunden gelten.
  - Stammdaten, "Klassifikatoren" auf Seite B-881
- **Wert von, Wert bis**: Eingrenzung auf Klassifikatorenwerte.
  - Stammdaten, "Klassifikatoren Wertzuordnung" auf Seite B-929
- **Deckungsbeitrag**: Mit der Wahl der Option legen Sie fest, ob der Deckungsbeitrag als Betrag oder prozentual angezeigt werden soll. Die Felder sind nur freigeschaltet, wenn im Bereich Spalten die Checkboxen DB 1, DB 1 %, DB 2 oder DB 2% markiert ist.
  - Stammdaten, "Klassifikatoren" auf Seite B-881
- **(von - bis)**: Eingrenzung auf einen Wert oder eine Spanne von Werten. Sie können auch negative Zahlenwerte eintragen.

**Beispiele**

| Eingabe | Ergebnis |
| :--- | :--- |
| Negativer Wert: | Alle Aufträge, deren Kosten größer sind als der VK, z. B. von -99999 bis 0,00 |
| Null | Alle Aufträge, deren Kosten durch den VK gedeckt sind, z. B. von 0,00 bis 0,00 |
| Größer null | Alle Aufträge, deren Kosten kleiner sind als der VK, z. B. von 1,00 bis 1000 |

#### Auflistung nach

Mit der Wahl der Option legen Sie fest, wie die Werte der Trefferliste gegliedert werden:
- **Zeitraum**: Im Bereich Aufschlüsseln nach können Sie die Ausgabe zusätzlich nach AV-Bereichen, Warengruppen oder Aufträgen auflösen. Bei der Auswertung eines Jahres werden die Daten z. B. nach Monaten summiert. Wenn Sie z. B. die Auswahl auf einen Monat eingeschränkt haben, können Sie das Ergebnis zusätzlich nach Aufträgen aufschlüsseln.
- **Warengruppen**: Im Bereich Summieren nach werden die Felder freigeschaltet. Im Bereich Aufschlüsseln nach wird die Checkbox Warengruppen gesperrt.
- **AV-Bereiche**: Im Bereich Aufschlüsseln nach können Sie die Ausgabe zusätzlich nach Warengruppen oder Aufträgen auflösen.
- **Kunden**: Im Bereich Aufschlüsseln nach können Sie die Ausgabe zusätzlich nach AV-Bereichen, Warengruppen oder Aufträgen auflösen.

#### Summieren nach

Mit der Wahl der Option legen Sie fest, wie die Werte summiert werden sollen. Die zur Verfügung stehenden Optionen sind abhängig davon, welches Feld Sie im Bereich Auflistung nach gewählt haben. Es stehen folgende Optionen zur Verfügung:
- **AV-Bereiche**: Im Bereich Aufschlüsseln nach können Sie die Ausgabe zusätzlich nach Warenhauptgruppen, Warenobergruppen, Warengruppen oder Top-Warengruppen auflösen. Die Werte des Betrachtungszeitraums werden nach der gewählten Option summiert.
- **Warengruppen**: Im Bereich Aufschlüsseln nach können Sie die Ausgabe zusätzlich nach Warenhauptgruppen, Warenobergruppen, Warengruppen oder Top-Warengruppen auflösen. Die Werte des Betrachtungszeitraums werden nach der gewählten Option summiert.
- **Aufträgen**: Die Werte werden nach Aufträgen summiert.

#### Aufschlüsselung nach

Mit der Wahl der Option legen Sie fest, wie die Werte aufgelöst werden sollen. Damit wird die Gesamtmenge pro Warenhauptgruppe, Warenobergruppe, Warengruppe oder Top-Warengruppe angezeigt.
Sie können nur eine der angezeigten Checkboxen markieren. Wenn Sie keine Checkbox markieren, werden die Werte nach den Selektionskriterien gruppiert.

- **Warenhauptgruppen**: Die Werte werden nach Warenhauptgruppen aufgelöst.
- **Warenobergruppen**: Die Werte werden nach Warenobergruppen aufgelöst.
- **Warengruppen**: Die Werte werden nach Warengruppen aufgelöst.
- **Top-Warengruppen**: Die Werte werden nach Top-Warengruppen aufgelöst.

#### Optionen

- **Vergleich mit Vorjahreswerten**: In den Registern können die Vergleichswerte des Vorjahres angezeigt werden. Die Checkbox ist nur aktiv, wenn Sie im Bereich Auflistung nach die Option Zeitraum gewählt haben. In den Bereichen Summieren nach und Aufschlüsselung nach dürfen keine Kriterien ausgewählt sein.
  - ☐ Die Vergleichswerte werden nicht ausgegeben.
  - ☑ Die Vergleichswerte werden ausgegeben. Diese Einstellung wird auch in den Standard-Druck übernommen. Im Umsatzdruck werden die Vergleichswerte immer angezeigt.
- **Anzeige der Beträge durch Tausend geteilt**: Sie können die Geldbeträge durch 1000 geteilt darstellen lassen.
  - ☐ Die Geldbeträge werden unverändert angezeigt.
  - ☑ Die Geldbeträge werden durch 1000 geteilt angezeigt.

### Auftragsinfo – Erfasst

**Statistik > Auftragsinfo > Register Erfasst**

*Abb. F-2: Auftragsinfo - Erfasst*

In diesem Register werden alle Aufträge angezeigt, die noch nicht weiter bearbeitet wurden. Zur Auswahl wird das Erfassungsdatum herangezogen.
Die Ausgabe kann mit der Ausgabe im Register Offen übereinstimmen, wenn die Selektionskriterien nicht weiter eingegrenzt wurden.
Die Anzeige der Spalten wird im Register Optionen ausgewählt.
⇨ "Auftragsinfo - Optionen" auf Seite F-2632

### Auftragsinfo – Produziert

**Statistik > Auftragsinfo > Register Produziert**

*Abb. F-3: Auftragsinfo - Produziert*

In diesem Register werden alle Aufträge angezeigt, die aus der Produktion als fertig gemeldet sind.
Die Anzeige der Spalten wird im Register Optionen ausgewählt.
⇨ "Auftragsinfo - Optionen" auf Seite F-2632

### Auftragsinfo – Fakturiert

**Statistik > Auftragsinfo > Register Fakturiert**

*Abb. F-4: Auftragsinfo - Fakturiert*

In diesem Register werden alle Aufträge angezeigt, für die eine Rechnung geschrieben wurde. Dazu wird das Rechnungsdatum herangezogen.
Die Anzeige der Spalten wird im Register Optionen ausgewählt.
⇨ "Auftragsinfo - Optionen" auf Seite F-2632

### Auftragsinfo – Offen

**Statistik > Auftragsinfo > Register Offen**

*Abb. F-5: Auftragsinfo - Offen*

In diesem Register werden alle Aufträge angezeigt, die vor dem aktuellen Datum erfasst, aber noch nicht produziert wurden. Das sind alle Aufträge, zu denen weder ein Rechnungsdatum noch eine Laufnummer existiert.
Die Anzeige der Spalten wird im Register Optionen ausgewählt.
⇨ "Auftragsinfo – Optionen" auf Seite F-2632

### Auftragsinfo – Grafik

**Statistik > Auftragsinfo > Register Grafik**

*Abb. F-6: Auftragsinfo - Grafik und Legende*

in diesem Register werden die Daten der Auswahl grafisch dargestellt.
Die Anzeige der Daten wird im Register Optionen ausgewählt.
⇨ "Auftragsinfo - Optionen" auf Seite F-2632

**Anzeige**
Mit der Wahl der Option können Sie die Daten der Register einzeln anzeigen lassen.

### Auswahl

**Statistik > Auftragsinfo > Menü Druck**

*Abb. F-7: Druckeinstellung*

In diesem Dialog legen Sie fest, wie die Auftragsinformationen im Druck ausgegeben werden sollen.

**Auswahl Report**
Mit der Wahl der Option legen Sie fest, welches Register gedruckt werden soll.

**Auswahl Spalten (max. 3)**
In diesem Bereich wird für jede Spalte aus dem Register Offen eine Checkbox angezeigt. Wenn Sie im Bereich Auswahl Report die Option Alle ausgewählt haben, können Sie nur maximal drei Spalten drucken.
- ☐ Die Spalte wird nicht gedruckt.
- ☑ Die Spalte wird gedruckt.

### Umsatz Verkauf

**Statistik > Umsatz Verkauf**

Neben dem Druck der Umsatzinformationen aus dem Dialog Auftragsinfo stehen in diesem Dialog detaillierte Auswertungen für die Verkaufszahlen zur Verfügung.

In diesem Dialog finden Sie folgende Register:
- "Umsatz Verkauf - Auswahl" auf Seite F-2644
- "Umsatz Verkauf - Restriktionen" auf Seite F-2649
- "Umsatz Verkauf - Tabelle" auf Seite F-2650
- "Umsatzstatistik - Grafik" auf Seite F-2651
- "Umsatz Verkauf - SQL" auf Seite F-2652

In den Registern Auswahl und Restriktionen legen Sie die Kriterien für die Auswertung der Daten fest.
In den Registern Tabelle und Grafik wird das Ergebnis der Auswertung angezeigt.

#### Menü Optionen

**Statistik > Umsatz Verkauf**

Über dieses Menü können Sie die Standardeinstellung des Dialogs bestimmen. Sie können die Optionen aktivieren oder deaktivieren. Die Einstellung wird nicht zurückgesetzt, wenn Sie den Dialog schließen.

> **Aktivierte Optionen nach dem Öffnen des Dialogs**
> Bitte beachten Sie, dass geänderte Optionen erst beim nächsten Öffnen des Dialogs wirksam werden.
> Die folgenden Beschreibungen stellen die aktivierte Option dar.

Das Menü ist in folgende Gruppen gegliedert:
- Gruppe Einstellungen
- Gruppe Automatischer Seitenvorschub beim Druck

**Gruppe Einstellungen**
- **Mengen inklusive Stückliste**: Die Mengen aus der Stückliste werden in die Angabe der Menge aufgenommen.
- **Nur Positionsmengen**: Nur die Stückzahl der Positionen wird angezeigt, z. B. 5 Stk. ISO.
- **Nur Stücklistenmengen**: Nur die Stückzahlen der Stückliste werden angezeigt. Diese Einstellung eignet sich z. B. für Bearbeitungen.
- **Abweichendes Wirtschaftsjahr aktiv**: Bei Jahresauswertungen soll nicht das Kalenderjahr sondern das Wirtschaftsjahr betrachtet werden.
- **Statistiknamen drucken**: Im Druck soll die Bezeichnung der Statistik mit angegeben werden. Der Name wird aus der gespeicherten Datei entnommen.

**Gruppe Automatischer Seitenvorschub beim Druck**
- **Nach Zwischensumme 1 bis 5**: Nach den ausgewählten Zwischensummen wird im Druck ein Seitenumbruch eingefügt.
- **Vor Endsumme**: Vor der Endsumme wird ein Seitenumbruch eingefügt.

#### Menü Superstatistik

**Statistik > Umsatz Verkauf**

Über dieses Menü erstellen Sie eine Superstatistik.

- **Einstellungen**: Öffnet den Dialog Statistik, um die Einstellungen für die Superstatistik festzulegen.
  - "Superstatistik" auf Seite F-2653
- **Exportieren, Importieren**: Öffnet die Dialoge für manuellen Export oder Import einer Superstatistik.
  - "Superstatistik - Export" auf Seite F-2655

### Umsatz Verkauf – Auswahl

**Statistik > Umsatz Verkauf > Register Auswahl**

*Abb. F-8: Umsatzstatistik Verkauf*

in diesem Register legen Sie die Kriterien für die Auswertung der Umsatzzahlen fest. Die Einstellungen können Sie als Datei speichern, um eine gleichwertige Statistik später wieder erstellen zu können.

#### Auswahl Statistik

Wenn Sie bestimmte Einstellungen sehr häufig benutzen, können Sie diese als Datei speichern und wieder auswählen.
Wenn Sie eine der gespeicherten Einstellungen wieder auswählen, müssen Sie im Bereich Auswertungszeitraum nur den Zeitraum angeben.

#### Ausgabe / Summenbildung / Sortierung

**Ausgabe**: Im linken Feld sind alle Ausgabekriterien aufgeführt, auf die sich die statistischen Auswertungen beziehen können.
Für die Auswertung verschieben Sie alle die Ausgabekriterien, deren Werte herangezogen werden sollen.
Von den folgenden Checkboxen muss mindestens eine markiert sein, damit Daten ausgewertet werden.

- **Statistik gesamt bilden**: Sie können den Gesamtumsatz des Unternehmens anzeigen lassen.
  - ☐ Die Statistik wird nur über die ausgewählten Kriterien gebildet.
  - ☑ Die Statistik wird über den Gesamtumsatz gebildet. Diese Form dient insbesondere Vergleichszwecken.

> **Beispiel**
> Wenn im Bereich Ausgabe/Summenbildung/Sortierung das Merkmal Produkte/Artikel gewählt ist, wird der Umsatz der Produkte im Vergleich zum Gesamtumsatz des Unternehmens dargestellt, z. B. EUR 800.000 gegenüber EUR 20.000.000.

> **Performance**
> Diese Auswertung dauert einige Zeit, da alle Daten des gesamten Unternehmens eingelesen werden müssen.

- **Summe Selektion bilden**: Sie können im Ergebnis Zwischensummen anzeigen lassen.
  - ☐ Eine Zwischensumme wird nicht gebildet.
  - ☑ Pro Ausgabekriterium wird die Zwischensumme gebildet. Dazu werden die Einstellungen im Register Restriktionen berücksichtigt, z. B. die angegebenen Warengruppen.
- **Jahresauswertung**: Sie können die Ausgabe für ein ganzes Jahr zusammenfassen.
  - ☐ Das Ergebnis wird nicht pro Jahr angezeigt. Bei dieser Einstellung sollten Sie eine Monatsauswertung starten.
  - ☑ Das Ergebnis wird pro Jahr angezeigt. Betrachtet werden die Jahre, die im Bereich Auswertungszeitraum angegeben sind.
- **Monatsauswertung**: Sie können die Ausgabe pro Monat zusammenfassen.
  - ☐ Das Ergebnis wird nicht pro Monat angezeigt. Bei dieser Einstellung sollten Sie eine Jahresauswertung starten.
  - ☑ Das Ergebnis wird pro Monat angezeigt. Betrachtet werden die Jahre und Monate, die im Bereich Auswertungszeitraum angegeben sind.
- **Direkte Gegenüberstellung**: Sie können die Auswertung von mehreren Jahren monatsweise gegenüberstellen.
  - ☐ Die Auswertung über mehrere Jahre wird Jahr für Jahr dargestellt.
  - ☑ Die Auswertung über mehrere Jahre wird Monat für Monat über die angegebenen Jahre dargestellt.

**Beispiele für drei Jahre und Monat 1 bis 3**

| Einstellung | Ausgabe |
| :--- | :--- |
| ☐ | Jahr 1: Januar, Februar, März<br>Jahr 2: Januar, Februar, März<br>Jahr 3: Januar, Februar, März |
| ☑ | Januar: Jahr 1, Jahr 2, Jahr 3<br>Februar: Jahr 1, Jahr 2, Jahr 3<br>März: Jahr 1, Jahr 2, Jahr 3 |

- **Superstatistik**: Sie können Statistiken als Gegenüberstellung der Umsatzzahlen für Filialen und/oder Mandanten erstellen.
  - ☐ Die Superstatistik wird nicht erstellt.
  - ☑ Die Daten werden nach den Vorgaben erstellt, die im Dialog Statistik festgelegt wurden. Im Register Tabelle wird kein Ergebnis angezeigt. Eine Beschreibung dieser Superstatistik finden Sie in einem separaten Abschnitt.
    - "Superstatistik" auf Seite F-2653
- **Top-10-Modus**: Sie können die Ausgabe der Statistik auf die besten Ergebnisse einschränken.
  - ☐ Die Auswertung wird nicht auf die besten Ergebnisse eingeschränkt.
  - ☑ In der Auswertung sollen nur die besten Ergebnisse angezeigt werden. Dazu müssen Sie im Bereich Top 10 - Auswertung/Sortierung die Darstellung der Daten festlegen.
- **Startmonat Wirtschaftsjahr**: Bei Auswertungen soll nicht das Kalenderjahr sondern das Wirtschaftsjahr betrachtet werden. Das Feld zur Eingabe des ersten Monats ist nur freigeschaltet, wenn im Menü Optionen > Gruppe Einstellungen > Abweichendes Wirtschaftsjahr aktiv aktiviert wurde.

#### Auswahl Rubriken

Mit der Wahl der Rubriken entscheiden Sie, welche Werte im Einzelnen im Register Tabelle ausgegeben werden.

> **Tipp**
> Beachten Sie bei der Auswahl der Rubriken, dass die Übersichtlichkeit verloren gehen kann, wenn Sie zu viele Checkboxen markieren. Wenn Sie viele Detaildaten brauchen, erstellen Sie mehrere Statistiken mit unterschiedlichen Einstellungen, die Sie im Feld Auswahl Statistik jeweils (mit einem sprechenden Namen) speichern.

- **Umsatz**: Wird in der Spalte Rubrik als Umsatz dargestellt.
- **Umsatz %**: Wird in der Spalte Rubrik als % U. dargestellt.
- **Materialkosten**: Wird in der Spalte Rubrik als Materialkosten dargestellt.
- **Frachtkosten**: Wird in der Spalte Rubrik als Frachtkosten dargestellt.
- **Fertigungskosten**: Wird in der Spalte Rubrik als Fertigungskosten dargestellt.
- **Prozesskosten (Fertig.+Fracht)**: Wird in der Spalte Rubrik als Prozesskosten dargestellt.
- **Gesamtkosten**: Wird in der Spalte Rubrik als Gesamtkosten dargestellt.
- **Gemeinkosten (Vertr.+Verw.)**: Wird in der Spalte Rubrik als Gemeinkosten dargestellt.
- **Rohgewinn**: Wird in der Spalte Rubrik als Rohgewinn dargestellt.
- **in %**: Wird in der Spalte Rubrik als RG % dargestellt.
- **Umsatz Reklamation**: Nur im Dialog Reklamation Verkauf freigeschaltet. Wird in der Spalte Rubrik angezeigt.
- **DB 1**: Wird in der Spalte Rubrik als DB 1 dargestellt.
- **in %**: Wird in der Spalte Rubrik als DB 1% dargestellt.
- **DB 2**: Wird in der Spalte Rubrik als DB 2 dargestellt.
- **in %**: Wird in der Spalte Rubrik als DB 2% dargestellt.
- **Stück**: Wird in der Spalte Rubrik als Stück dargestellt.
- **Fläche**: Wird in der Spalte Rubrik als Fläche dargestellt.
- **Umfang**: Gesamte Kantenlänge. Wird in der Spalte Rubrik als Umfang dargestellt.
- **Gewicht**: Wird in der Spalte Rubrik als Gewicht dargestellt.
  - ☐ Die Werte werden nicht angezeigt.
  - ☑ Die Werte werden angezeigt.

#### TOP10 - Auswertung / Sortierung

Die Felder in diesem Bereich sind nur freigeschaltet, wenn die Checkbox Top10 Modus markiert ist. In diesem Modus werden jeweils nur die besten Ergebnisse angezeigt.

- **Sortierung nach**: Die Sortierungskriterien sind von der A+W Software GmbH vorgegeben: DB (Deckungsbeitrag), Fläche, Kosten, Stück, Umfang, Umsatz.
Mit der Wahl der Option legen Sie fest, welcher Wert zuerst aufgeführt wird:
  - **Absteigend**: Bei den Tops wird der höchste Wert zuerst angezeigt.
  - **Aufsteigend**: Bei den Flops wird niedrigste Wert zuerst angezeigt.
- **Zeilen maximal**: Anzahl der auszuwertenden Tops oder Flops. Damit können Sie die Anzeige z. B. auf die 3 umsatzstärksten Tops einschränken.
In der Tabelle ist das die Anzahl der Zeilen. In der Grafik ist das die Anzahl der Balken.

#### Auswertungszeitraum

- **Jahr von, bis**: Jahr oder Spanne von Jahren, die ausgewertet werden sollen.
- **Monat von, bis**: Monat oder Spanne von Monaten, die ausgewertet werden sollen.

#### Anzeige Beträge

- **Beträge**: Sie können die Geldbeträge durch 1000 geteilt darstellen lassen.
  - ☐ Die Geldbeträge werden unverändert angezeigt.
  - ☑ Die Geldbeträge werden durch 1000 geteilt angezeigt. Bei dieser Einstellung sollten Sie angeben, wie viele Nachkommastellen angezeigt werden sollen.
- **Nachkommastellen**: Anzahl der Nachkommastellen, wenn die Geldbeträge geteilt durch 1000 angezeigt werden.

#### Letzte Änderung

- **Mitarbeiter/Datum**: Name des letzten Bearbeiters und Datum der letzten Änderung.

### Umsatz Verkauf – Restriktionen

**Statistik > Umsatz Verkauf > Register Restriktionen**

*Abb. F-9: Umsatzstatistik - Restriktionen*

In diesem Register können Sie die Auswertungen auf bestimmte Bereiche eingrenzen oder diese Bereiche ausschließen.

**Beispiel**

| Register Auswahl: | Register Restriktionen: |
| :--- | :--- |
| • Vertreter | • Vertreter 1 |
| • Kundengruppe | • Kundengruppe 3 - 7 |
| • Kunde | • Nicht Kunde 4000 |
| • Produkt | • Produkt 103 - 106 |

#### Auswahl der Restriktionen

- **Nicht**: Sie können die in den Feldern von und bis angegebenen Bereiche ein- oder ausschließen.
  - ☐ Die Statistik wird auf die angegebenen Restriktionen eingeschränkt.
  - ☑ Die angegebenen Restriktionen werden nicht in die Statistik aufgenommen.
- **Von, bis**: Restriktion, die in die Statistik aufgenommen oder aus ihr ausgeschlossen werden soll.
- **Mindestumsatz für Auswertung**: Angabe des Mindestumsatzes, ab dem die Werte in die Auswertungen mit einbezogen werden. Mit der Wahl der Option legen Sie fest, ob sich der angegebene Mindestumsatz auf ein Jahr oder einen Monat bezieht.

### Umsatz Verkauf - Tabelle

**Statistik > Umsatz Verkauf > Register Tabelle**

*Abb. F-10: Umsatzstatistik - Tabelle*

In diesem Register wird das Ergebnis der Auswertung als Tabelle angezeigt. Über das Menü Druck können Sie das Ergebnis in tabellarischer Form drucken.

### Umsatzstatistik – Grafik

**Statistik > Umsatz Verkauf > Register Grafik**

*Abb. F-11: Umsatzstatistik – Grafik*

In diesem Register werden die Daten der Auswertung grafisch angezeigt.

### Umsatz Verkauf – SQL

**Statistik > Umsatz Verkauf > Register SQL**

*Abb. F-12: Umsatzstatistik - Grafik*

In diesem Register können Sie eigene SQL-Abfragen erstellen.

### Superstatistik

**Statistik > Umsatz Verkauf > Menü Superstatistik > Einstellungen**

*Abb. F-13: Gruppenstatistik Verwalten*

Über diesen Dialog werden die Daten für die Superstatistiken exportiert oder importiert.

#### Voraussetzung und Ziel der Superstatistik

Superstatistiken können nur von Hauptfirmen mit Filialen erstellt werden. Die Hauptfirma/Zentrale und die Filialen müssen per Datenaustausch miteinander kommunizieren können.
In der Superstatistik werden die Umsatzdaten der Hauptfirma/Zentrale und der Filialen einander gegenüber gestellt.
Die Filialen werden durch die Zuordnung in einer Superstatistik der Zentrale/Hauptfirma zu Mandanten.

*Abb. F-14: Superstatistik*

Die Zentrale legt fest, in welchen Abständen die Filialen ASCII-Dateien erstellen und exportieren müssen. In der Zentrale werden alle gesammelten Filial-Daten in die Superstatistik importiert.
Die Zentrale selbst kann auch eine Filiale sein und muss ihre eigenen Statistik-Daten ebenfalls exportieren.

#### Dialogbeschreibung

- **Mandant**: ID der Filiale oder des Mandanten, an den die Daten exportiert werden.
- **Statistik**: Statistik, für die die Daten erstellt werden.
- **Export Mandant**: ID des Mandanten, an den die Daten exportiert werden. Über diese ID liest das Importsystem die Daten beim (Ziel-)Mandanten ein.
- **Import Pfad**: Verzeichnis, in dem die exportierten Daten liegen. Sie werden beim Ziel-Mandanten in einer Schleife nacheinander eingelesen.
- **Protokoll Pfad**: Daten, die nicht importiert werden können, werden in einer Protokolldatei gespeichert. Der Administrator muss die fehlenden Stammdaten anlegen und/oder die falschen Stammdaten korrigieren. Beim nächsten Import wird erneut versucht, den entsprechenden Datensatz einzulesen.
- **Definition Import**: In diesem Bereich legt die importierende Zentrale fest, wie eingehende Daten standardmäßig gebucht werden sollen:
  - Integration immer auf default
  - Integration 1:1 oder auf default
  - Integration 1:1 zwingend
- **Auswahl default**: In diesen Feldern legen Sie den Default-Satz fest, in den die importierten Daten geschrieben werden.

### Superstatistik – Export

**Statistik > Umsatz Verkauf > Menü Superstatistik > Exportieren**

*Abb. F-15: Superstatistik – Export manuell*

In diesem Dialog exportieren Sie die ASCII-Dateien für die Superstatistik manuell. Der manuelle Export stellt in der Praxis die Ausnahme dar. Normalerweise werden die Einstellungen einmal in der Filiale vorgenommen, die Mandanten-Nummer wird eingestellt, und der Rest erfolgt automatisch.
In der Regel werden die Daten bei der Archivübergabe auch an die Statistik übergeben: Dokumente > Auftrag > Übergabe Archiv > Checkbox Umsatzstatistik.

#### Export

- **Mandant (lokal)**: Mandant, der die Daten exportiert.
- **Auswahl Datum von, bis**: Angabe der Zeitspanne, in der die Datei(en) mit den Umsatzdaten erzeugt wurden.
- **Zieldatei überschreiben**: Im Exportverzeichnis kann bereits eine gleichnamige Datei liegen. Wenn Sie sicher sind, dass diese bereits in die Auswertung der Superstatistik eingeflossen ist, können Sie die alte Datei überschreiben.
  - ☐ Die alte Datei wird nicht überschrieben. Die neue Datei unterscheidet sich durch Datum und Zeitstempel.
  - ☑ Die alte Datei wird überschrieben.
- **Export Mandant**: ID der Filiale oder des Mandanten, an den die Daten exportiert werden, d. h. der Ziel-Mandant.
- **Exportierte Sätze**: Anzahl der exportierten Datensätze in der Datei.
- **Export Pfad**: Pfad und Dateiname, z. B. C:\Superstat\Export\0001_20140506.asc.

### Superstatistik – Import

**Statistik > Umsatz Verkauf > Menü Superstatistik > Importieren**

*Abb. F-16: Superstatistik – Import manuell*

In diesem Dialog importieren Sie die ASCII-Dateien für die Superstatistik.
Die aufgelaufenen Fehler werden im Systemlogbuch angezeigt und können über Protokoll-Dateien identifiziert werden.
Protokolle werden mit der Endung .sav gespeichert.

### Reklamationsstatistik Verkauf

**Statistik > Reklamation Verkauf**

*Abb. F-17: Reklamationsstatistik Verkauf*

In diesem Dialog erstellen Sie Statistiken über die Reklamationen im Verkauf. Zu dieser Statistik werden alle Dokumente vom Typ Reklamationen herangezogen.
Die Felder sind ausführlich zum Dialog Umsatz Verkauf beschrieben.
- "Umsatz Verkauf" auf Seite F-2642
Für die Reklamationsstatistik müssen Sie eine Monatsauswertung erstellen.
Auswertungen über den Reklamationsgrund, Verursacher und Reklamationsort können nur erstellt werden, wenn Reklamationsgründe und Reklamationsverursacher in den Stammdaten angelegt sind.

### Statistik nach Aufbau

**Statistik > Statistik nach Aufbau**

In diesem Dialog erstellen Sie Auswertungen über den Aufbau Scheiben mit Stücklisten. Dabei werden nur fakturierte Aufträge ausgewertet.
Das Ergebnis der Auswertung wird im Register Tabelle angezeigt und kann gedruckt werden.
In diesem Dialog finden Sie folgende Register:
- "Statistik nach Aufbau - Auswahl" auf Seite F-2658
- "Statistik nach Aufbau - Tabelle" auf Seite F-2661

#### Statistik nach Aufbau – Auswahl

**Statistik > Statistik nach Aufbau > Register Auswahl**

*Abb. F-18: Statistik nach Aufbau – Auswahl*

In diesem Register legen Sie die Auswertungskriterien fest.

**Menü Sperre aufheben**
Sie können die Datensätze für die Dauer der Auswertung sperren, damit während der Auswertung keine Datensätze ergänzt oder verändert werden. Diese Funktion ist sinnvoll, wenn die Auswertung längere Zeit in Anspruch nimmt.
**Auswertungszeitraum**
Jahr, Monat von, bis: Angabe des Zeitraums, der ausgewertet werden soll.

**Abstandhalter**
Mit der Wahl der Option legen Sie für die Auswertung von ISO fest, welche Abstandhalter berücksichtigt werden sollen:
- **Gesamt**: Alle ISO-Scheiben werden ausgewertet.
- **TPS**: Nur ISO-Scheiben mit TPS werden ausgewertet.
- **ISO normal**: Nur ISO-Scheiben ohne TPS werden ausgewertet.

**Typ**
Mit der Wahl der Option legen Sie den Typ der Produkte fest, die ausgewertet werden sollen:
- **Isolierglas**: Nur ISO wird ausgewertet. Mit dieser Option können Sie zusätzlich auch ISO mit Zusatzarbeiten auswerten lassen.
- **Zusatzarbeiten**: Nur Zusatzarbeiten werden ausgewertet.
- **Glasarten**: Nur die Glasarten werden ausgewertet. Die Checkbox Mit Zusatzarbeiten ist gesperrt.

**Mit Zusatzarbeiten** Wenn Sie ISO auswerten wollen, können Sie zusätzlich das ISO mit Zusatzarbeiten auswerten.
- ☐ ISO-Scheiben werden ohne Zusatzarbeiten ausgewertet.
- ☑ Zusätzlich zu den ISO-Scheiben werden ISO-Scheiben mit Zusatzarbeiten ausgewertet.

**Auswahl von Restriktionen**
- **Vertreter von, bis**: Vertreter, auf die die Auswertung eingegrenzt werden soll.
- **Kunde von, bis**: Kunden, auf die die Auswertung eingegrenzt werden soll.
**Trennung nach**
Sie können die Auswertung weiter auflösen. Die Daten werden dann z. B. pro Kunde und Produkt ausgegeben.
- ☐ Im Druck wird kein zusätzlicher Seitenumbruch eingefügt.
- ☑ Im Druck wird der zusätzliche Seitenumbruch eingefügt.

> **Freigeschaltete Checkboxen**
> - Die Checkboxen Modell, SZR, Absth.-Typ und Gas sind nur freigeschaltet, wenn Sie den Typ ISO gewählt haben.
> - Die Checkbox Dicke wird gesperrt, wenn Sie die Checkbox Produkte markieren.

**Sortierung nach**
Mit der Wahl der Option legen Sie die Sortierung der Ausgabe fest:
- **Kunde-Umsatz**: Die Daten werden pro Kunde nach Umsatz absteigend sortiert.
- **Umsatz-Kunde**: Die Daten werden pro Umsatz nach Kunden sortiert.
- **Kunde-Fläche**: Die Daten werden pro Kunde nach Fläche absteigend sortiert.
- **Kunde-Aufbau**: Die Daten werden pro Kunde nach Aufbau sortiert.

**Summen**
- **Anzahl Einzel-Zeilen**: Anzahl der Zeilen, nach der eine Zwischensumme angezeigt werden soll. Wenn Sie 0 eintragen, werden keine Zwischensummen angezeigt.
- **Zeilen insgesamt**: Anzahl der Zeilen, die angezeigt werden sollen.

**Sonstiges**
- **Mit Firmensummen**: Sie können die Summen der beteiligten Firmen anzeigen lassen. Im Register Tabelle sind das die Spalten Stück Firma, Fläche Firma, Umsatz Firma, Wert/Fläche Firma.
  - ☐ Die Firmensummen werden nicht angezeigt.
  - ☑ Die Firmensummen werden angezeigt.
- **Spalten immer füllen**: Sie können die Anzeige von Namen und Kundennummern unterdrücken, wenn die gewählte Sortierung das übersichtlicher macht.
  - ☐ Die Spalten werden nur gefüllt, wenn die Daten für den nächsten Kunden angezeigt werden.
  - ☑ Die Spalten werden immer gefüllt.
- **Getr. n. Monaten**: Die Summen können nach Monaten gruppiert werden.
  - ☐ Die Summen werden chronologisch angezeigt.
  - ☑ Die Summen werden getrennt nach Monaten angezeigt.

#### Statistik nach Aufbau – Tabelle

**Statistik > Statistik nach Aufbau > Register Tabelle**

*Abb. F-19: Statistik nach Aufbau - Tabelle*

In diesem Register wird das Ergebnis der Auswertung angezeigt.
Abhängig von den Filterkriterien im Register Auswahl werden zusätzlich folgende Spalten angezeigt:
- **Modell**: Anzeige, ob Modelle enthalten sind.
- **SZR**: Dicke des Abstandhalters (Rahmen).
- **Rahmen Typ**: Nummer der Produktgruppe, zu der der Abstandhalter (Rahmen) gehört.
- **Gas**: Produktnummer des Gases.

Standardmäßig können folgende Spalten angezeigt werden:
- **Vertreter, Kunde**: Wenn Sie keine Eingrenzung im Bereich Auswahl von Restriktionen eingestellt haben, werden die Namen nicht angezeigt.
- **Aufbau**: Scheibenaufbau, z. B. Float 5 mm + Therm 6 mm, wenn Produkte angezeigt werden, oder 4 + 4 + 8 mm, wenn die Dicke angezeigt wird.
- **Stück**: Stückzahl.
- **Fläche**: Gesamtfläche.
- **Lfm**: Kantenlänge insgesamt.
- **Sprossenfelder**: Anzahle der Sprossenfelder. Die Anzahl wird nur angezeigt, wenn im Bereich Typ die Option Isolierglas ausgewählt ist.
- **Umsatz**: Gesamtumsatz
- **Fläche pro Stück**: Durchschnittliche Fläche pro Stück.
- **Wert pro Fläche**: Wert der Fläche in Eigenwährung. z. B. €/qm.
- **Wert Reklamationen**: Gesamtwert aller Reklamationen pro Kunde in Eigenwährung.
- **Wert Gutschriften**: Gesamtwert aller Gutschriften pro Kunde in Eigenwährung.
- **Stück Firma, Fläche Firma, Umsatz Firma, Wert/Fläche Firma**: Anzeige der Gesamtsummen. Werden nur angezeigt, wenn im Bereich Sonstiges die Checkbox mit Firmensummen ausgewählt ist.
- **Faktor**: Verhältnis von Wert/Fläche Firma zu Wert pro Fläche.
- **Zusatzarbeiten**: Anzahl der Zusatzarbeiten. Wird nur angezeigt, wenn im Bereich Typ die Checkbox mit Zusatzarbeiten ausgewählt ist.

### Kunden nach AV-Bereich

**Statistik > Kunden nach AV-Bereichen**

*Abb. F-20: AV-Bereiche*

In diesem Dialog erstellen Sie Auswertungen über die AV-Bereiche. Sie können die Auswertung über alle AV-Bereiche starten oder auf einzelne eingrenzen. Ausgegeben werden jeweils die Umsatzwerte des angegebenen Jahres pro Kunde und Monat.

#### Auswahl

Mit der Wahl der Option legen Sie fest, welche AV-Bereiche betrachtet werden sollen:
- **AV-Bereich auswählen**: Der Bereich Auswahl der AV-Bereiche wird freigeschaltet. Die Statistik wird über alle AV-Bereiche erstellt, die in dieser Auswahl markiert sind.
- **Alle AV-Bereiche mit Umsatz**: Die Statistik wird über alle AV-Bereiche erstellt, in denen Umsatzwerte gefunden wurden. Der Bereich Auswahl der AV-Bereiche wird gesperrt.
- **Jahr**: Jahr, das betrachtet werden soll.
- **Druck-Modus**: Mit der Wahl der Option legen Sie fest, ob die Statistik auf dem Bildschirm oder einem Drucker ausgegeben werden soll.
- **Auswahl der AV-Bereiche**: In diesem Bereich sind alle AV-Bereiche aufgelistet. Die Auswahl ist nur freigeschaltet, wenn die Option AV-Bereiche auswählen markiert ist. Die Statistik wird zu allen AV-Bereichen erstellt, deren Checkbox markiert ist.

## Einkaufsstatistiken

Neben den Umsatzinformationen stehen auch detaillierte Auswertungen für die Einkaufszahlen zur Verfügung.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Umsatzstatistik Einkauf" auf Seite F-2665
- "Reklamationsstatistik Einkauf" auf Seite F-2666
- "Liefertreue" auf Seite F-2667
- "Analyse Verbrauch" auf Seite F-2669

### Umsatzstatistik Einkauf

**Statistik > Umsatz Einkauf**

*Abb. F-21: Umsatzstatistik Einkauf*

In diesem Dialog erstellen Sie Statistiken zum Einkauf. Dazu werden die Bestellungen ausgewertet.
Die Felder sind ausführlich zum Dialog Umsatz Verkauf beschrieben.
- "Umsatz Verkauf" auf Seite F-2642

### Reklamationsstatistik Einkauf

**Statistik > Reklamation Einkauf**

*Abb. F-22: Reklamationsstatistik Einkauf*

In diesem Dialog erstellen Sie Statistiken über die Reklamationen im Einkauf. Zu dieser Statistik werden alle fakturierten Bestellungen herangezogen.
Die Felder sind ausführlich zum Dialog Umsatz Verkauf beschrieben.
- "Umsatz Verkauf" auf Seite F-2642

### Liefertreue

**Statistik > Liefertreue**

*Abb. F-23: Liefertreue*

In diesem Dialog erstellen Sie Statistiken über die Verzögerungen, die bei Lieferungen oder Aufträgen aufgetreten sind. Für die Auswertung werden die Terminverschiebungen herangezogen.

#### Auswahl

- **Modus**: Mit der Wahl der Option legen Sie fest, nach welchen Partnern ausgewertet werden soll:
  - **Kunden**: Die Lieferterminverschiebungen werden ausgewertet. Diese Verschiebungen können z. B. durch verspätete Lieferungen von Bestellteilen oder durch Produktionstermine entstanden sein.
  - **Lieferanten**: Verspätete Lieferungen durch die Lieferanten werden ausgewertet.
- **Datenbank**: Mit der Wahl der Option legen Sie fest, welcher Datenumfang ausgewertet werden soll:
  - **Hauptdatenbank + aktuelles Archiv**: Die Hauptdatenbank und das aktuell Archivjahr werden ausgewertet.
  - **Archivjahr**: Nur ein bestimmtes Archiv wird ausgewertet. Das Feld für die Auswahl des Archives wird freigeschaltet. Bei dieser Einstellung werden keine Dokumente berücksichtigt, die in der Hauptdatenbank liegen.

#### Einschränkungen

- **Zeitraum von, bis**: Zeitraum, der ausgewertet werden soll.
- **Auswertungsgrenze 1, 2**: Anzahl von Verspätungstagen. Mit der Auswahl ändert sich die Anzeige in den Tabellenspalten.
- **Kundennummer von, bis**: Kunden oder Folge von Kunden, zu denen Verzögerungen ausgewertet werden sollen.
- **Kundengruppe**: Kundengruppe, zu der Verzögerungen ausgewertet werden sollen.
- **Nicht einschränken**: Alle Kunden sollen ausgewertet werden.

#### Tabelle

In der Übersicht wird das Ergebnis der Auswertung pro Kunde oder Lieferant angezeigt.
- **Ø Tage früher, Ø Tage später**: Durchschnitt aus beiden Auswertungsgrenzen in Tagen.
- **> n Tage früher**: Anzahl der Aufträge pro Auswertungsgrenze, die über der Grenze lagen. Bei Lieferanten sind das die Bestellungen, die über der Grenze lagen.
- **< n Tage später**: Anzahl der Aufträge pro Auswertungsgrenze, die unter der Grenze lagen.
- **Pünktlich**: Anzahl der Aufträge, die zum vereinbarten Termin geliefert wurden.
Die Anzeige schließt mit einer Summenzeile.

### Analyse Verbrauch

**Statistik > Analyse Verbrauch**

Sie können den Materialverbrauch nach selbst gewählten Kriterien auswerten.
In diesem Dialog finden Sie folgende Register:
- "Analyse Verbrauch – Auswahl" auf Seite F-2669
- "Analyse Verbrauch - Restriktionen" auf Seite F-2672
- "Analyse Verbrauch - Tabelle" auf Seite F-2674

#### Menü Optionen

- **Automatischer Seitenvorschub aktiv**: Im Druck wird automatisch ein Seitenumbruch eingefügt.

#### Analyse Verbrauch – Auswahl

**Statistik > Analyse Verbrauch > Register Auswahl**

*Abb. F-24: Analyse Verbrauch – Auswahl*

In diesem Register legen Sie die Kriterien für die Auswertung fest.

**Quelle**
- **Nummer**: Auftrag, der ausgewertet werden soll.
- **Archiv**: Die Archive können in die Suche nach einem einzelnen Auftrag eingeschlossen werden.
  - ☐ Nur in der Hauptdatenbank wird nach dem Auftrag gesucht.
  - ☑ In der Hauptdatenbank und in den Archiven wird nach dem Auftrag gesucht.
- **Nummernverwalter**: Auswahl des Nummernverwalters. Mit dieser Option werden die Felder im Bereich Auswertungszeitraum gesperrt.
- **Mandant**: Mandant, auf den die Auswertung eingeschränkt werden soll.
- **AV-Bereich**: AV-Bereich, auf den die Auswertung eingeschränkt werden soll.

**Auswertungszeitraum**
Die Felder in diesem Bereich sind gesperrt, wenn die Option Nummernverwalter gewählt ist.
- **Nach Liefertermin von, bis**: Zeitraum von Lieferterminen, der ausgewertet werden soll.
- **Nach Produktionstermin von, bis**: Zeitraum von Produktionsterminen, der ausgewertet werden soll.

**Auswahl Statusbereich**
- **Von, bis**: Statusbereich der Dokumente, die ausgewertet werden sollen.

**Auswahl Produkt**
- **Produktart**: Produktart, die ausgewertet werden soll. Sie können die Standardauswahl <k.A.> löschen.
- **Produktgruppe**: Produktgruppe, die ausgewertet werden soll.
- **Artikel**: Produkt, das ausgewertet werden soll.

**Sortierung / Summenbildung**
Sie können festlegen, nach welchen Kriterien das Ergebnis sortiert werden soll. Pro ausgewähltem Kriterium wird eine Summe gebildet.
- **Auswahlfelder**: Die ausgewählten Kriterien werden im rechten Feld angezeigt und können dort mit den Pfeil-Schaltflächen in die gewünschte Reihenfolge verschoben werden.
- **Auflösung pro Auftrag**: Das Ergebnis kann detailliert nach Aufträgen angezeigt werden.
  - ☐ Pro Sortierkriterium wird eine Zeile angezeigt.
  - ☑ Pro Sortierkriterium und Auftrag wird eine Zeile angezeigt.
- **Auflösung pro Position**: Das Ergebnis kann nach Positionen angezeigt werden.
  - ☐ Pro Sortierkriterium wird eine Zeile angezeigt. Wenn nach Aufträgen aufgelöst wird, werden die Auftragspositionen nicht einzeln aufgeführt.
  - ☑ Pro Sortierkriterium und Auftragsposition wird eine Zeile angezeigt.

**Auswahl Produktbereich**
Sie können die Statistik auf einzelne Produktbereiche folgender Glasarten einschränken: EFG (Einfachglas), ESG, VSG, ISO.
- ☐ Die Daten aus diesem Produktbereich werden nicht in der Statistik ausgegeben.
- ☑ Die Daten aus diesem Produktbereich werden in der Statistik ausgegeben.

**Optionen**
- **Gasberechnung individuell**: Zur Zeit nicht genutzt.
- **Mengeneinheit**: Mengeneinheit, in der Gas angegeben werden soll.

#### Analyse Verbrauch – Restriktionen

**Statistik > Analyse Verbrauch > Register Restriktionen**

*Abb. F-25: Analyse Verbrauch – Restriktionen*

In diesem Register können Sie die Auswahl der Analyse nach Verbrauch weiter einschränken.

**Quelle**
Mit der Wahl der Option legen Sie fest, welche Dokumente ausgewertet werden sollen:
- **Nummer**: Ein einzelner Auftrag soll ausgewertet werden. Das Feld zur Eingabe der Auftragsnummer und die Checkbox Archiv werden freigeschaltet.
- **Nummernverwalter**: Die Aufträge eines Nummernverwalters sollen ausgewertet werden.

- **Archiv**: Das angegebene Dokument kann auch im Archiv gesucht werden.
  - ☐ Die Archive werden nicht durchsucht.
  - ☑ Das Dokument soll im Archiv gesucht werden, wenn es nicht in der Hauptdatenbank gefunden wurde. Diese Einstellung ist sinnvoll, wenn Sie Dokumente in kurzen Zeiträumen archivieren.
- **Mandant**: Mandant, auf den die Auswertung eingeschränkt werden soll.
- **AV-Bereich**: AV-Bereich, der ausgewertet werden soll.

**Auswertungszeitraum**
Mit der Wahl der Option legen Sie fest, aus welchem Zeitraum Dokumente ausgewertet werden sollen:
- **Nach Lieferdatum**: Der angegebene Zeitraum bezieht sich auf das Lieferdatum.
- **Nach Produktionstermin**: Der angegebene Zeitraum bezieht sich auf den Termin, an dem die Produktion begonnen wurde.
- **Von, bis**: Zeitraum, der ausgewertet werden soll.

**Auswahl Statusbereich**
- **Von, bis**: Statusbereich der Dokumente, die ausgewertet werden sollen.

**Auswahl Produkt**
- **Produktart**: Produktart, die ausgewertet werden soll.
- **Produktgruppe**: Produktgruppe, die ausgewertet werden soll.
- **Artikel**: Produkt, das ausgewertet werden soll.

**Auswahl Beschaffungsarten**
Die Auswertung kann zusätzlich auf Beschaffungsarten eingegrenzt werden.
- ☐ Die Beschaffungsart wird nicht berücksichtigt.
- ☑ Nur Produkte mit dieser Beschaffungsart sollen ausgewertet werden.

**Auswahl Produktarten**
Die Auswertung kann zusätzlich auf Produktarten eingegrenzt werden.
- ☐ Die Produktart wird nicht berücksichtigt.
- ☑ Nur Produkte dieser Produktart sollen ausgewertet werden.

#### Analyse Verbrauch – Tabelle

**Statistik > Analyse Verbrauch > Register Tabelle**

*Abb. F-26: Analyse Verbrauch - Tabelle*

In diesem Register wird das Ergebnis der Auswertung angezeigt. Die Anzeige der Spalten und Zeilen richtet sich nach den Einstellungen, die Sie im Register Auswahl festgelegt haben.

### Provisionsstatistik

**Statistik > Provisionsstatistik**

*Abb. F-27: Provisionsstatistik*

In diesem Dialog werten Sie die Vertreterprovisionen aus.

#### Auswahl

- **Vertreter**: Vertreter, wenn die Auswertung auf einen einzelnen Vertreter eingeschränkt werden soll.
- **Von, bis**: Zeitraum, der ausgewertet werden soll.
Mit der Wahl der Option legen Sie fest, worauf sich der Zeitraum bezieht:
  - **Nach Rechnungsdatum**: Mit dieser Einstellung werten Sie nur fakturierte Dokumente aus.
  - **Nach Erfassungsdatum**: Mit dieser Einstellung werten Sie alle Dokumente im angegebenen Zeitraum aus.
  - **Nach Übergabedatum**: Mit dieser Einstellung werten Sie die Dokumente aus, die im angegebenen Zeitraum an die Statistik übergeben wurden.

#### Zwischensumme

Sie können einstellen, ob und wo Zwischensummen gebildet werden sollen.

- **Pro Vertreter**: Wenn Sie die Dokumente für alle Vertreter auswerten, können Sie pro Vertreter eine Zwischensumme bilden lassen.
  - ☐ Zwischensummen werden nicht gebildet. Diese Einstellung ist dann sinnvoll, wenn Sie die Auswertung für einen bestimmten Vertreter erstellen lassen.
  - ☑ Nach jedem Vertreter wird eine Zwischensumme eingefügt.
- **Pro Kunde**: Wenn Sie die Dokumente über einen längeren Zeitraum auswerten, können Sie pro Kunde eine Zwischensumme bilden lassen.
  - ☐ Zwischensummen werden nicht gebildet.
  - ☑ Pro Kunde wird eine Zwischensumme eingefügt.

#### Ergebnis

In der Übersicht werden folgende Spalten angezeigt.
- **Vertreter**: Name des Vertreters.
- **Nr. Rechnung, Datum Rechnung**: Nummer und Datum der Rechnung.
- **Nr. Auftrag**: Auftragsnummer.
- **Datum Erfassung**: Erfassungsdatum.
- **Summe Umsatz**: Gesamtsumme des Auftrags.
- **% Provision**: Provisionssatz im Auftrag.
- **Summe Provision**: Betrag der Provision.
- **ID Kunde, Name Kunde**: Nummer und Name des Kunden.
- **Datum Übergabe**: Übergabe an die Statistik.
- **Land**: Land, in dem der Kunde ansässig ist.

### Intrastat Meldung

**Statistik > Intrastat Meldungen**

*Abb. F-28: Intrastat Meldung*

In diesem Dialog erstellen Sie Auswertungen zu den Intrastat-Meldungen.

#### Indentifikation

- **Mandant**: Mandant, für dessen Dokumente die Statistik erstellt wird.
- **Mitarbeiter**: Angemeldeter Mitarbeiter.
- **NV Aufträge**: Nummernverwalter, in dem die Aufträge gesammelt sind.
- **NV Gutschriften**: Nummernverwalter, in dem die Gutschriften gesammelt sind.

#### Vorgabe

- **Archiv**: Archiv, dessen Dokumente ausgewertet werden sollen.

#### Neuen NV anlegen

Die Felder in diesem Bereich sind nur freigeschaltet, wenn Sie einen neuen Nummernverwalter anlegen. Wählen Sie dazu Menü Start > [Neu].
- **Rechnungsdatum von, bis**: Zeitraum, in dem die Aufträge fakturiert wurden.
- **Länderkennzeichen**: Land, zu dem Sie die Statistik erstellen wollen. Zur Wahl stehen nur die Länderkennzeichen, die in den Stammdaten angelegt sind.
- **Name NV Aufträge**: Eingabe des Namens. Wählen Sie einen sprechenden Namen, damit Sie erkennen können, welche Dokumente in diesem Nummernverwalter gesammelt sind.
- **Name NV Gutschriften**: Eingabe des Namens. Wählen Sie einen sprechenden Namen, damit Sie erkennen können, welche Gutschriften in diesem Nummernverwalter gesammelt sind.

#### Zu meldende Dokumente

In der Übersicht werden alle Dokumente angezeigt, die im gewählten Nummernverwalter zusammengestellt sind.
- **Best. Land**: Land aus dem die Ware eingeführt wurde.
- **Nummer**: Auftragsnummer.
- **Bestell-Nr.**: Bestellnummer.
- **AB-Lieferant**: Nummer der Auftragsbestätigung durch den Lieferanten.
- **Rechnung**: Nummer der Rechnungsnummer zum Kundenautrag.
- **Datum Anlief. Lief.**: Datum der Anlieferung durch den Lieferanten.
- **Auftrags-Nummer**: Auftragsnummer.
- **Datum Auslieferung**: Lieferdatum ab Werk.
- **Kunde/Lieferant**: Kunden- oder Lieferantennummer.
- **Name, Matchcode**: Name und Matchcode des Kunden oder Lieferanten.
- **Status**: Dokumentenstatus.
- **Datum Erfass.**: Erfassungsdatum des Dokumentes.
- **Datum AB**: Datum der Auftragsbestätigung.
- **Datum Prod. ISO, VSG, ESG**: Produktionsdatum für die Glasart.
- **Lauf-Nr. Prod. ISO, VSG, ESG**: Nummer des Produktionslaufs.
- **Anlieferdatum**: Lieferdatum beim Kunden.
- **Lieferschein**: Lieferscheinnummer.
- **Datum Lieferung**: Lieferdatum.
- **Rechnung, Datum Rechnung**: Nummer und Datum der Rechnung.
- **Stück gesamt**: Gesamtstückzahl.
- **Qm real**: Fläche insgesamt.
- **LFM real**: Tatsächliche Laufmeter der Kantenlänge.
- **Gewicht gesamt**: Gesamtgewicht.
- **Qm fakturiert**: Fakturierte Gesamtfläche.
- **LFM fakturiert**: Fakturierte Kantenlänge.
- **Betrag Netto**: Rechnungsbetrag netto.
- **Tour**: Name der Liefertour.
- **Geschäftsart**: Bezeichnung der Geschäftsart.
- **AV-Bereich**: Bezeichnung des AV-Bereichs.
- **Vertreter 1, Vertreter 2**: Namen der beteiligten Vertreter.
- **Sperr-KZ**: Sperrkennzeichen aus den Zusatzinformationen zum Auftrag.

# A+W Business Lagerwirtschaft

## Revisionsübersicht des Moduls:

| Datum | Änderung |
| --- | --- |
| 04-2023 | Aktualisierung der Softwarereferenz. |
| 04-2020 | Neu: Lagerverwaltung > Kritischer Lagerbestand. |
| 10-2019 | Einstellungen Kistenmanagement in separaten Part übertragen und aus Part Lagerwirtschaft gelöscht. |
| 08-2019 | Einstellungen zur Inventurlisten und zum Druck von Kistenetiketten neu. |
| 01-2017 | Inventur überarbeitet, Dialog Lagerbewertung neu. |
| 08-2013 | Vollständige Überarbeitung der ALFAK-Dokumentation und Anpassung auf A+W Business. |
| 01-2013 | Layout an CI 2013 angepasst. |
| 02-2012 | Korrekturen |
| 11-2010 | Aktualisierung und Umstellung auf Doku-Konzept 2010 |
| 08-2009 | Vollständige Überarbeitung |
| 09-2008 | Abbildungen und Part-Nummer angepasst. |
| 08-2008 | Rechtschreibkorrekturen |
| 12-2003 | Struktureller Umbau auf Programmstruktur 4.0 |
| 08-2000 | Überarbeitung Lager |
| 03-1998 | Ersterstellung |

**Zu diesem Modul finden Sie folgende Kapitel:**
- Tutorial
- Softwarereferenz

# Tutorial

## Übersicht

Das Tutorial zum Modul Lagerwirtschaft beschäftigt sich mit den Grundlagen der Lagerverwaltung in A+W Business. Das Tutorial baut auf den Kenntnissen zu den Stammdaten, zum Einkauf und zum Verkauf auf.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen installiert und freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

### Themenblöcke

In diesem Tutorial finden Sie folgende Themenblöcke:
- Grundgedanken zum Lager
- Stammdaten
- Lagerwirtschaft
- Lagerartikel in Dokumenten
- Inventur

### Vorausgesetzte Kenntnisse

Das Tutorial richtet sich an Teilnehmer, die in A+W Business den Lagerbestand verwalten. Die Teilnehmer müssen das Konzept der Stammdaten, den Verkauf und den Einkauf in A+W Business kennen.

> **Kistenverwaltung im Lager**
> Die Einstellungen zum Kistenmanagement sind in dem separaten Part Kistenmanagement beschrieben.

### Aufbau des Tutorials

Das Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

- **Überblick**: Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
  - Lernziele: Was soll vermittelt werden?
  - Nutzen: Wofür können Sie dieses Wissen einsetzen?
  - Merksätze: Welche Zusammenhänge müssen Sie sich merken?
- **Konzepte**: Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.
- **Übungen**: Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen und Lösungsvorschlägen.
- **Querverweise**: Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf ergänzende Informationen in der Softwarereferenz und in anderen Parts hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.

> **Lesehinweis**
> Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen. Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.

### Menü-Übersicht

In diesem Abschnitt finden Sie eine kurze Übersicht über die Programmbereiche, die in den Themenblöcken dieser Schulung angesprochen werden.

*Abb. G-1: Menü Lagerwirtschaft*

#### Inventur

In diesem Bereich bereiten Sie die Inventur vor, tragen die gezählten Werte ein und schließen die Inventur ab.
- "Menü Lagerwirtschaft" auf Seite G-2689
- "Inventur" auf Seite G-2816
- Softwarereferenz, "Inventur" auf Seite G-2843

#### Lagerverwaltung

In diesem Dialog erfassen und pflegen Sie die Daten für Lagerartikel.
- "Lagerverwaltung" auf Seite G-2743
- Softwarereferenz, "Lagerverwaltung" auf Seite G-2861

#### Lagerbewegung

In diesem Dialog buchen Sie Warenzugänge und Warenabgänge, Änderungen von Lagerorten und den Aufbruch von Kisten.
- "Lagerbuchung" auf Seite G-2753
- Softwarereferenz, “Lagerbewegung" auf Seite G-2873
#### Abfragen

In diesem Bereich lassen Sie sich die Lagerhistorie, Auswertungen und Reservierungen anzeigen.
- "Abfragen" auf Seite G-2763
- Softwarereferenz, "Abfragen" auf Seite G-2881

#### Suche

In diesem Dialog prüfen Sie die Verfügbarkeit von Produkten in einem bestimmten Zeitraum.
- “Lagerinformationen" auf Seite G-2772
- Softwarereferenz, "Suche" auf Seite G-2898

#### Lagerbestellung

In diesem Dialog übergeben Sie Bestellungen zu Lagerartikeln an den Einkauf.
- "Lagerbestellung an den Einkauf übergeben" auf Seite G-2784
- Softwarereferenz, "Lagerbestellung" auf Seite G-2901

#### Ergänzende Informationen

- Überblick, "Elemente des Programmfensters" auf Seite A-65
- Verkauf, "Dialog Dokumentenverwaltung" auf Seite C-1294

## Grundgedanken zum Lager

Im Modul Lagerwirtschaft von A+W Business können Sie Bandmaße, Lagermaße, Restblätter, Kisten, Ganzglastüren, Beschläge, Rahmenteile und Zubehör wie Spiegelaufhängungen, Dichtungsbänder usw. verwalten.
Dabei ist es möglich, die Lagerorganisation Ihres Unternehmens im Programm abzubilden. Sie definieren Standorte, Gänge, Regale bis hin zu den einzelnen Fächern und legen fest, welche Stück-, Quadrat- oder Laufmeterartikel sich an welchem Lagerort befinden.

*Abb. G-2: Übersicht über die Lagerwirtschaft*

Alle kaufmännischen Vorgänge in A+W Business basieren auf den Stammdaten. Nur wenn diese korrekt gepflegt sind, kann die Verwaltung des Lagers problemlos abgewickelt werden. Zusammen mit dem Verkauf und dem Einkauf ergeben sich folgende Abläufe:

- **Auftrag**: In einem Auftrag fixieren Sie die Bestellung Ihres Kunden. Dabei erfassen Sie Positionen, die nach den Angaben des Kunden gefertigt werden müssen.
- **Übergabe Produktion**: An die Produktion werden die Auftragspositionen übergeben, die gefertigt werden müssen. Die benötigten Materialien werden reserviert und beim Druck von Lieferschein oder Rechnung ausgebucht. Gleichzeitig wird der verfügbare Lagerbestand aktualisiert.
- **Lagerbestellung**: Wenn der Mindestbestand von Lagerartikeln unterschritten wird, müssen diese Lagerartikel als Lagerbestellung erfasst werden.
- **Lagerzugang**: Mit der Erfassung des Wareneingangs wird der Lagerbestand der Lagerartikel aktualisiert. Artikel, die nicht als Lagerartikel geführt werden, können nicht als Lagerbestand geführt werden.
- **Inventur**: Mit der Inventur bereinigen Sie die Bestandszahlen in A+W Business.

### Handlungsablauf bei der Lagerverwaltung

Üblicherweise pflegen Sie den Lagerbestand durch folgende Aktivitäten:
- Stammdaten einrichten
- Lagerartikel erfassen (Erstinventur)
- Warenein- und -ausgänge buchen (automatisch, manuell)
- Abfragen zu Umschlagshäufigkeit, Preisen, Beständen usw.
- Lagerbestellung erfassen, prüfen, senden
- Inventur durchführen:
  - Inventurliste erstellen, Nachtragsinventur anhängen
  - Sollbestand ermitteln
  - Zähllisten drucken
  - Gezählte Werte erfassen
  - Inventur abschließen

### Wie soll das Lager geführt werden

Allen Produkten, die im Verkauf erfasst werden, wird ein Kennzeichen zugeordnet, das die Art der Beschaffung festlegt. Gläser, die im Lager geführt werden, haben neben dem Kennzeichen (Beschaffungsart) Lagerentnahme ein Kennzeichen (Lagerbuchungsart) für die Art, wie ihr Lagerbestand berechnet wird. Diese beiden Kennzeichen werden in der Themenblock Stammdaten beschrieben.

Bevor Sie Ihr Lager in A+W Business einrichten, müssen Sie entscheiden, auf welcher Basis die Bestände geführt werden sollen: als Fläche (qm) oder in Stückzahlen. Als dritte Möglichkeit steht die kombinierte Lagerführung zur Verfügung, wobei der maßabhängige Lagermodus mit den Rückmeldungen aus der Optimierung kombiniert wird, so dass neben den Lagermaßen auch die zugeschnittenen Bandmaße automatisch ausgebucht werden können.

Diese unterschiedlichen Möglichkeiten wirken sich folgendermaßen aus:

| Modus (Lagerkennzeichen) | Bedeutung, Beispiel | Nachteil |
| :--- | :--- | :--- |
| qm = Fläche: (nicht maßabhängig) | pro Glas wird die Fläche ermittelt:<br>- Float 4 => 10.500 qm<br>- Float 5 => 11.070 qm<br>- Float 6 => x qm | - keine Info über die Anzahl der Lagermaße<br>- keine Info darüber, wie viele Bandmaße verschnitten wurden |
| Stück: (maßabhängig) | pro Bandmaß und Lagermaß wird die Stückzahl ermittelt:<br>- Float 4<br>  3210/6000 3 Stück, 900/1200 3 Stück, x/x n Stück<br>- Float 5<br>  3210/6000 3 Stück, 800/1200 3 Stück, x/x n Stück | - keine Info über verschnittene Band- und Lagermaße<br>- Bandmaße müssen manuell ausgebucht werden |
| Stück inkl. Rückmeldungen: (kombiniert) | Kombination aus maßabhängigen Lagermaßen und Rückmeldungen. Die verschnittenen Bandmaße und die Lagermaße werden automatisch ausgebucht. Bestand der Stückzahlen wird aktualisiert. | (Für diesen Modus müssen A+W Optimizer-Rückmeldungen möglich sein.) |

Nach der Entscheidung zum Modus ordnen Sie das entsprechende Lagerkennzeichen pro Glasprodukt zu und legen in den Firmendaten den Lagerführungsmodus fest. Diese Einstellungen sind in der Themenblock Stammdaten detailliert beschrieben.
- "Lagerführungsmodus und Reservierung" auf Seite G-2705

## Stammdaten

In diesem Themenblock lernen Sie, wie Sie die Stammdaten für die Verwaltung des Lagers pflegen.

Dazu gehören folgende Lerneinheiten:
- "Lager" auf Seite G-2695
- "Firmendaten" auf Seite G-2704
- "Status" auf Seite G-2709
- "Produktdefinition" auf Seite G-2713
- "Preise" auf Seite G-2726

### Lager

**Lernziele**
- Lagerebenen benennen.
- Lagerort definieren.
- Lagerkategorien festlegen.

**Nutzen**
- Mit Lagerorten können Sie (gleiche) Materialien an unterschiedlichen Orten verwalten.
- Auswertungen können sich auf bestimmte Lagerorte oder Lagerartikel beziehen, die an unterschiedlichen Orten gelagert sind.

**Merke**
- **Ebenen**: Vier Differenzierungsebenen bezeichnen z. B. unterschiedliche Lagerhäuser, Gänge, Regale und Fächer.
- **Lagerorte**: Die Kombinationen der verschiedenen Differenzierungsebenen bilden die Lagerorte.
- **Lagerkategorien**: Mit Lagerkategorien können Sie die Suche und Auswertung auf bestimmte Produkte einschränken, die an unterschiedlichen Orten gelagert werden.
- **Voreinstellungen**: Keine

### Lagerdefinition

Für die Darstellung Ihres Lagers legen Sie folgende Einstellungen fest:
- Namen der Lagerebenen
- Lagerebenen
- Lagerorte

Die Bezeichnung der einzelnen Ebenen können Sie an die Erfordernisse im Unternehmen anpassen. Diese Möglichkeit sollten Sie auch dann nutzen, wenn Sie nur mit einer Ebene arbeiten.

#### Lagerort

Zur Definition von Lagerorten können Sie bis zu vier Differenzierungsebenen festlegen und damit z. B. Lagerhäuser, Gänge, Regale und Fächer unterscheiden. Die Lagerorte werden in der Lagerverwaltung und bei der Inventur herangezogen.

*Abb. G-3: Beispiel: Lagerort = Haus 1*

#### Lagerebene

Pro Ebene können Sie verschiedene Namen festlegen, z. B. auf der Ebene 1 die Lagerhäuser an unterschiedlichen Standorten, auf Ebene 2 die Gänge A bis F usw.

> **Mindestens einen Lagerort definieren**
> Sie müssen auch dann einen Lagerort definieren, wenn Sie Ihr Lager nicht weiter unterteilt haben. In diesem Fall legen Sie nur die Ebene 1 fest und definieren dann im Lagerort alle weiteren Ebenen als <k.A.>.

#### Lagerkategorien

Über Lagerkategorien haben Sie ein weiteres Suchkriterium für die Lagerverwaltung. Wenn Sie z. B. gleiches Material an verschiedenen Lagerorten verwalten, können Sie die Lagerkategorie dazu verwenden, das Material gemeinsam auszuwerten. Dazu sollten Sie alle Lagerorte definiert haben, an denen das Material tatsächlich vorgehalten wird.
Die definierten Lagerkategorien ordnen Sie im Dialog Lagerverwaltung den Produkten zu.

### Lagerebenen festlegen

In dieser Einheit lernen Sie, wie Sie die Lagerebenen an die Erfordernisse in Ihrem Unternehmen anpassen.
Zu dieser Lerneinheit gibt es folgende Handlungsanleitungen:
- "So legen Sie Ihre verschiedenen Lagerebenen fest" auf Seite G-2697
- “So benennen Sie die Lagerebenen" auf Seite G-2699

#### So legen Sie Ihre verschiedenen Lagerebenen fest

Die folgenden Schritte sind für alle Lagerebenen gleich. In diesem Beispiel wird eine Lagerebene 1 für Fertigprodukte angelegt.
1. Wählen Sie im Menü Stammdaten > Lager > Ebene 1.
   Der Dialog Ebene 1 wird geöffnet.
   - Stammdaten, "Ebene 1 bis 4" auf Seite B-864
2. Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wechseln.

   *Abb. G-4: Zeile für neue Lagerebene*

3. Geben Sie eine Bezeichnung für die Lagerebene ein, z. B. Ortsnamen, Zuschnitt usw.
4. Wählen Sie im Menü Start > Speichern, um die Daten zu speichern.
   Die Daten werden gespeichert.
5. Wiederholen die Schritte 1 bis 4 für alle Ebenen, die Sie in Ihrem Lager unterscheiden möchten. Öffnen Sie dazu auch die Dialoge zu den Lagerebenen 2 bis 4 und verfahren Sie auf die gleiche Weise.

#### So benennen Sie die Lagerebenen

1. Wählen Sie im Menü Stammdaten > Lager > Lagerdefinition.
   Der Dialog Lagerdefinition wird geöffnet.
   - Stammdaten, "Lagerdefinition" auf Seite B-865
2. Wählen Sie im Menü Definition > Ebenen.

   *Abb. G-5: Lagerebenen benennen*

3. Legen Sie die Namen der Lagerebenen fest, z. B. Lagerhaus für die Ebene 1.
4. Klicken Sie auf [OK], um die Namen zu speichern.
   Der Dialog wird geschlossen. Die Änderungen werden in den Dialog Lagerdefinition übernommen.
5. Schließen Sie den Dialog Lagerdefinition oder definieren Sie nun die Lagerorte.
   - "Lagerort definieren" auf Seite G-2699

### Lagerort definieren

In dieser Einheit lernen Sie, wie Sie in A+W Business die Lagerorte einrichten.
Sie müssen auch dann einen Lagerort definieren, wenn Sie Ihr Lager nicht weiter unterteilt haben. In diesem Fall legen Sie nur die Ebene 1 fest und definieren dann für den Lagerort alle weiteren Ebenen als <k.A.>. Beachten Sie, dass auch ein Lagerort mit der Definition <k.A.> für alle Ebenen als Lagerort bebucht werden kann.

> **Tipp**
> Sie können bestimmte Materialien von einer Lagerhalle in den Produktionsbereich verlagern. Dazu werden die Lagerorte umgebucht. Für diesen Fall ist es sinnvoll, Lagerorte so präzise (kleinteilig) wie möglich zu definieren, z. B. bei den Fächern.

#### So definieren Sie einen Lagerort

1. Wählen Sie im Menü Stammdaten > Lager > Lagerdefinition.

   *Abb. G-6: Lagerorte definieren*
   *(A: Selbst gewählte Bezeichnung der Ebenen, B: Liste der definierten Lagerorte)*

   - Stammdaten, "Lagerdefinition" auf Seite B-865
   In diesem Modus können Sie die definierten Lagerorte (A) ändern, indem Sie die Bezeichnungen der Ebenen ändern. Wenn Sie den Erfassungsmodus gewählt haben, werden die Felder der Tabelle gesperrt.
2. Wählen Sie im Menü Start > Neu, um in den Erfassungs-Modus zu wechseln.
