---
title: "DE_AWEnterprise_Verkauf_4_2"
source: "DE_AWEnterprise_Verkauf_4_2.pdf"
tags: ["A+W Enterprise", "Sales Module", "ERP Software", "Software Reference", "Order Entry", "Product Search", "Transaction Management", "German", "User Guide", "Technical Documentation"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for the A+W Enterprise Sales (Verkauf) module, version 4.00. It provides detailed descriptions of the search functions and transaction management capabilities within the system, intended for users and technical staff."
long_description: "This comprehensive software reference manual details the functionalities of the A+W Enterprise Sales (Verkauf) module, specifically version 4.00, dated February 2020. The guide is divided into two main parts: Search Functions (Suchfunktionen) and Transaction Management (Vorgangsverwaltung). The Search Functions section covers various methods for finding articles, products, and objects within the system. It explains search criteria for 'Artikel-Suche' (Article Search) by code, description, type, and more. It also details 'Produktsuche nach Elementen' (Product Search by Components) for complex products like insulated glass (ISO) or laminated glass (VSG), and 'Objekt-Suche' (Object Search) for site- or project-specific data. The Transaction Management section provides an in-depth overview of creating and managing sales documents, including quotes (Angebote), orders (Aufträge), and price-less entries. It describes the user interface, field definitions, process flows, and various options for order entry, customer data, shipping, invoicing, and printing. The document serves as a technical guide for users, explaining UI elements, navigation paths (e.g., Verkauf > Auftragserfassung), keyboard shortcuts, and the meaning of different system statuses and symbols."
---

# Softwarereferenz: Suchfunktionen

---
## Artikelcode
Artikelcode aus den Stammdaten. Die Artikel, deren Artikelcode nicht die angegebenen Daten enthält, werden aus der Trefferliste ausgeschlossen.
**Technische Info**: alphanumerisches Feld, DB-Feld: artikel.artikelcode

## Kurzbezeichnung
Kurzbezeichnung des Artikels. Die Artikel, deren Kurzbezeichnung nicht die angegebenen Daten enthält, werden aus der Trefferliste ausgeschlossen.
**Technische Info**: alphanumerisches Feld, DB-Feld: artikel.kurzbez

## Hauptbezeichnung, Interne Bezeichnung, Intern2
Hauptbezeichnung und zusätzliche Bezeichnungen des Artikels. Die Artikel, deren Hauptbezeichnung oder interne Bezeichnung nicht die angegebenen Daten enthält, werden aus der Trefferliste ausgeschlossen.
**Technische Info**: alphanumerische Felder, DB-Felder: artikel.artbez1, artikel.artbez2, artikel.artbez3

## Artikeltyp, bis
Nummer und Bezeichnung des Artikeltyps. Im Feld **Artikeltyp** geben Sie die Nummer an, ab der nach Artikeln gesucht wird. Im Feld **bis** beschränken Sie die Suche bis zu Artikeln mit dem entsprechenden Artikeltyp. Die Artikel, deren Artikeltypnummer kleiner als die angegebene Nummer im Feld Artikeltyp oder größer als die Nummer im Feld bis sind, werden aus der Trefferliste ausgeschlossen. Wenn Sie eine Nummer angeben, wird die Bezeichnung des Artikeltyps im Klartext angezeigt. Mit `<F9>` können Sie nach einem Artikeltyp suchen.
**Technische Info**: numerische Felder, Anzeigefelder, DB-Felder: artikel.atyp

## A+W Bearbeit.typ, bis
Nummer und Bezeichnung des A+W spezifischen Bearbeitungstyps. Im Feld **A+W Bearbeitung.typ** geben Sie die Nummer an, ab der nach Artikeln gesucht wird. Im Feld **bis** beschränken Sie die Suche bis zu Artikeln mit dem entsprechenden Bearbeitungstyp. Wenn Sie eine Nummer angeben, wird die Bezeichnung des Bearbeitungstyps im Klartext angezeigt. Mit `<F9>` können Sie nach einem Bearbeitungstyp suchen.
**Technische Info**: numerische Felder, Anzeigefelder, DB-Feld: artikel.awtyp

## Warengruppe
Kennzeichen der Warengruppe, der der Artikel zugeordnet ist.
**Technische Info**: alphanumerisches Feld, DB-Feld: artikel.wagrp

## Materialgrp.
Kennzeichen der Materialgruppe, der der Artikel zugeordnet ist.
**Technische Info**: alphanumerisches Feld, DB-Feld: artikel.artgrp

## Lieferant
Nummer des Lieferanten, bei dem der Artikel bestellt wird. Mit `<F9>` > `<F8>` wählen Sie den Lieferanten aus der Lieferantenliste aus.
**Technische Info**: numerisches Feld, DB-Feld: artikel.stdlinr

## Art
Anzeige des Artikelstatus. In der Vorgangserfassung werden nur aktive Artikel angezeigt. Das Feld kann nicht bearbeitet werden.
**Technische Info**: Anzeigefeld, DB-Feld: artikel.still

## Artikeldarstellung
In diesem Bereich wird der Scheibenaufbau des markierten Artikels aus der Trefferliste im Querschnitt angezeigt. Die Sonne markiert die Außenseite der Scheibe.

## Fußbereich
Mit den Schaltflächen im Fußbereich navigieren Sie in der Trefferliste, zeigen weitere Treffer an und aktualisieren die Trefferliste.

- **[<] und [>|]**: wechseln Sie zum ersten oder letzten Eintrag in der Trefferliste.
- **[<<] und [>>]**: zeigen Sie die vorherige oder nächste Seite der Trefferliste an.
- **Refresh**: Aktualisiert die Einträge in den Suchfeldern. Korrigierte oder zusätzliche Einträge in den Suchfeldern werden dadurch bei der Suche berücksichtigt. Die Schaltfläche ist nur im Bereich Suchfelder freigeschaltet.
- **Weitere Daten**: Zeigt in der Trefferliste weitere Einträge an, die den Suchkriterien entsprechen. Wenn keine weiteren Treffer mehr angezeigt werden können, ist die Schaltfläche gesperrt.
- **Neue Suche**: Löscht alle Suchkriterien für eine neue Suche. Alternativ können Sie die Suchkriterien mit `<Strg>` + `<R>` löschen und eine neue Suche starten.

## Artikel-Suche – Bezeichnungen
**Pfad:** `Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <F9> > Suchkriterien eingeben > <F3>`

**Abb. D-14: Artikel-Suche – Bezeichnungen**

In diesem Register werden die Bezeichnungen der Artikel angezeigt, die den Suchkriterien entsprechen.

Die Suchkriterien geben Sie im Kopfbereich an.
- Mit `<F2>` wechseln Sie die Register in der Trefferliste.
- Mit den Pfeiltasten und `<Bild runter>`, `<Bild hoch>` navigieren Sie in der Trefferliste.

### Kopfbereich
Die Felder im Kopfbereich sind zum Dialog Artikel-Suche - Kopf-, Fußbereich beschrieben:
⇨ "Artikel-Suche - Kopf-, Fußbereich" auf Seite D-50

### Satzanzeige für die Artikelübersicht
Die Anzahl der Treffer in der Liste wird rechts, über den Registern, in einem Rahmen angezeigt.
Die Satzanzeige ist zum Dialog Marktpartnersuche beschrieben:
⇨ "Marktpartnersuche" auf Seite D-39

### Register Bezeichnungen
Die Spalten entsprechen den Feldern im Kopfbereich. Zusätzlich werden folgende Spalten angezeigt:

- **Nummer**: Artikelnummer.
  - **Technische Info**: Anzeigefeld, DB-Feld: artikel.artnr
- **Still**: Anzeige, ob der Artikel stillgelegt ist.
  - J: Artikel ist stillgelegt.
  - N: Artikel ist aktiv.
  - In der Vorgangserfassung werden nur aktive Artikel angezeigt.
  - **Technische Info**: Anzeigefeld, DB-Feld: artikel.still

### Fußbereich
Die Felder im Fußbereich sind zum Dialog Artikel-Suche – Kopf-, Fußbereich beschrieben:
⇨ "Artikel-Suche - Kopf-, Fußbereich" auf Seite D-50

## Artikel-Suche - Artikelcodes
**Pfad:** `Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <F9> > Suchkriterien eingeben > <F3> > Register Artikelcodes`

**Abb. D-15: Artikel-Suche - Artikelcodes**

In diesem Register werden zusätzliche Informationen der Artikel angezeigt, die den Suchkriterien entsprechen.
Die Suchkriterien geben Sie im Kopfbereich an.
- Mit `<F2>` wechseln Sie die Register in der Trefferliste.
- Mit den Pfeiltasten und `<Bild runter>`, `<Bild hoch>` navigieren Sie in der Trefferliste.

### Kopfbereich
Die Felder im Kopfbereich sind zum Dialog Artikel-Suche – Kopf-, Fußbereich beschrieben:
⇨ "Artikel-Suche - Kopf-, Fußbereich" auf Seite D-50

### Satzanzeige für die Artikelübersicht
Die Anzahl der Treffer in der Liste wird rechts, über den Registern, in einem Rahmen angezeigt.
Die Satzanzeige ist zum Dialog Marktpartnersuche beschrieben:
⇨ "Marktpartnersuche" auf Seite D-39

### Register Artikelcodes
Die Spalten sind zum Register Bezeichnungen beschrieben:
⇨ "Artikel-Suche - Kopf-, Fußbereich" auf Seite D-50

Zusätzlich werden folgende Spalten angezeigt:
- **Bezeichnung**: Bezeichnung des Artikels.
  - **Technische Info**: Anzeigefeld, DB-Feld: artikel.artbez1
- **Lieferant, Name**: Lieferantennummer und Name des Lieferanten.
  - **Technische Info**: Anzeigefeld, DB-Feld: artikel.stdlinr

### Fußbereich
Die Felder im Fußbereich sind zum Dialog Artikel-Suche – Kopf-, Fußbereich beschrieben:
⇨ "Artikel-Suche - Kopf-, Fußbereich" auf Seite D-50

## Artikel-Suche - Details
**Pfad:** `Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <F9> > Suchkriterien eingeben > <F3> > Register Details`

**Abb. D-16: Artikel-Suche - Details**

In diesem Register werden die Details der Artikel angezeigt, die den Suchkriterien entsprechen.

### Kopfbereich und Navigation
Die Suchkriterien geben Sie im Kopfbereich an.
- Mit `<F2>` wechseln Sie die Register in der Trefferliste.
- Mit den Pfeiltasten und `<Bild runter>`, `<Bild hoch>` navigieren Sie in der Trefferliste.

Die Felder im Kopfbereich sind zum Dialog Artikel-Suche – Kopf-, Fußbereich beschrieben:
⇨ "Artikel-Suche - Kopf-, Fußbereich" auf Seite D-50

### Satzanzeige für die Artikelübersicht
Die Anzahl der Treffer in der Liste wird rechts, über den Registern, in einem Rahmen angezeigt. Die Satzanzeige ist zum Dialog Marktpartnersuche beschrieben:
⇨ "Marktpartnersuche" auf Seite D-39

### Register Details
Die Spalten sind zum Register **Bezeichnungen** beschrieben:
⇨ "Artikel-Suche - Kopf-, Fußbereich" auf Seite D-50

Zusätzlich werden folgende Spalten angezeigt:
- **Bezeichnung (Artikelnummer)**: Bezeichnung des Artikels.
  - **Technische Info**: Anzeigefeld, DB-Feld: artikel.artbez1
- **Atyp, Bezeichnung**: Nummer und Bezeichnung des Artikeltyps. Die Bezeichnung wird automatisch in der gewählten Systemsprache angezeigt.
  - **Technische Info**: Anzeigefeld, DB-Feld: artikel.atyp
- **A+W Typ, Bezeichnung**: Nummer und Bezeichnung des A+W-Bearbeitungstyps. Die Bezeichnung wird automatisch in der gewählten Systemsprache angezeigt.
  - **Technische Info**: Anzeigefeld, DB-Feld: artikel.awtyp

### Fußbereich
Die Felder im Fußbereich sind zum Dialog Artikel-Suche – Kopf-, Fußbereich beschrieben:
⇨ "Artikel-Suche - Kopf-, Fußbereich" auf Seite D-50

## Artikel-Suche nach Typen
**Pfad:** `Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld B.Art > <F5> > <F6> > [A-Suche]`

**Abb. D-17: Artikel-Suche nach Typen**

In diesem Dialog suchen Sie Artikel anhand der A+W Bearbeitungstypen oder der Artikeltypen. Alle Artikel des gewählten Typen werden in einem weiteren Auswahldialog angezeigt.

### Register Bearbeitungen
In diesem Register werden die Bearbeitungstypen zur Auswahl angezeigt, die in den normierten A+W Bearbeitungskatalog aufgenommen sind und Bearbeitungen in den Artikelstammdaten enthalten. Stillgelegte Bearbeitungstypen werden nicht angezeigt.
- **Nummer**: Nummer des A+W Bearbeitungstyps
- **A+W Bearbeitungstyp**: Bezeichnung des A+W Bearbeitungstyps

### Register Artikeltypen
In diesem Register werden die Artikeltypen zur Auswahl angezeigt, die Artikel in den Artikelstammdaten enthalten. Stillgelegte Artikeltypen werden nicht angezeigt.
- **Nummer**: Nummer des Artikeltyps
- **Artikeltypen**: Bezeichnung des Artikeltyps

### Auswahldialog
- **Artikel**: Artikel-, Bearbeitungsnummer
- **Bezeichnung**: Artikel-, Bearbeitungsbezeichnung
- **2. Bezeichnung**: Zusätzlicher Informationstext zur Bezeichnung, z. B. Kurzbezeichnung des Artikels oder Bearbeitungstyp.

## Produktsuche nach Elementen
**Pfad:** `Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <Shift> + <F8>`

In diesem Dialog suchen Sie nach Produkten anhand der enthaltenen Komponenten. Sie können die Produktsuche über verschiedene Menüpfade aufrufen. Der Dialog ist immer gleich aufgebaut.

Die Treffer der Suche werden in den Registern angezeigt. Die Trefferliste wird erst angezeigt, wenn Sie die Suche gestartet haben.
- Mit `<F3>` starten Sie die Suche.
- Mit `<F2>` wechseln Sie nach der Suche die Register in der Trefferliste.

In diesem Dialog finden Sie folgende Register:
- "Produktsuche nach Elementen - Kopf-, Fußbereich" auf Seite D-60
- "Produktsuche nach Elementen - Kundenartikel" auf Seite D-62
- "Produktsuche nach Elementen – Bezeichnungen" auf Seite D-64
- "Produktsuche nach Elementen - Techn. Werte" auf Seite D-65

### Produktsuche nach Elementen – Kopf-, Fußbereich
**Pfad:** `Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <Shift> + <F8>`

**Abb. D-18: Produktsuche nach Elementen – Kopf-, Fußbereich**

In diesem Dialog suchen Sie nach Produkten anhand von Elementen aus ihrem Stücklistenaufbau.

#### Kopfbereich
Im Kopfbereich geben Sie die Suchkriterien an. Die Treffer der Suche werden in den Registern angezeigt. Mit `<F3>` starten Sie die Suche.

- **Produkttyp**: Typ des Produkts:
  - ISO
  - VSG
  - Gießharz
  - **Technische Info**: Toggle-Feld, DB-Feld: artikel.artgrp

- **Glas1**: Nummer des ersten Glasartikels. Dieses Feld ist ein Pflichtfeld. Wenn Sie das Feld ohne Angabe einer Nummer verlassen, wird eine Liste der Glasartikel zur Auswahl angezeigt.
  - **Technische Info**: Pflichtfeld, numerisches Feld, DB-Feld: artkuzu.kuartnr

- **Glas2**: Nummer des zweiten Glasartikels. Dieses Feld ist optional.
  - **Technische Info**: numerisches Feld, DB-Feld: artkuzu.kuartnr

> **Position der Glasartikel in der Scheibe**
> Die Suchkriterien Glas1 und Glas2 berücksichtigen nicht die Einbauposition der Glasartikel in der Scheibe. Es wird nach allen Scheiben gesucht, die die angegebenen Gläser enthalten.
> In der Trefferliste werden die Gläser nach ihrer Einbauposition in der Scheibe von außen nach innen angezeigt. Glas1 ist das Glas auf der Außenseite der Scheibe.

- **Folientyp**: Nummer des Folientyps. Das Feld ist nur für den Produkttyp VSG freigeschaltet.
  - **Technische Info**: numerisches Feld, DB-Felder: artikel.folientyp

- **SZR**: Größe des Abstandhalters in Millimeter. Das Feld ist nur für den Produkttyp ISO freigeschaltet.
  - **Technische Info**: numerisches Feld, DB-Feld: musskenn.gv11

#### Fußbereich
- **Ausgewähltes Produkt**: Zurzeit nicht genutzt.
- **Artikelbezeichnung 1**: Zurzeit nicht genutzt.
- **Tech.Werte**: Zeigt die technischen Werte in den Spalten Ug-Wert, g-Wert, dB-Wert und Tv-Wert an. Die Schaltfläche ist nur kundenspezifisch freigeschaltet.
- **Suchen**: Startet die Suche. Die Schaltfläche ist nur im Kopfbereich freigeschaltet.
- **Auswahl**: Öffnet einen Auswahldialog zum aktuellen Feld. Die Schaltfläche ist nur freigeschaltet, wenn für das Feld Auswahloptionen hinterlegt sind.

### Produktsuche nach Elementen – Kundenartikel
**Pfad:** `Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <Shift> + <F8> > Suchkriterien eingeben > <F3>`

**Abb. D-19: Produktsuche nach Elementen - Kundenartikel**

In diesem Register werden Informationen zum Aufbau der Artikel angezeigt, die den Suchkriterien entsprechen.
- Mit `<F2>` wechseln Sie die Register in der Trefferliste.
- Mit den Pfeiltasten und `<Bild runter>`, `<Bild hoch>` navigieren Sie in der Trefferliste.
Im Kopfbereich geben Sie die Suchkriterien an.

#### Kopf-, Fußbereich
Die Felder im Kopf- und Fußbereich sind zum Dialog Produktsuche nach Elementen - Kopf-, Fußbereich beschrieben:
⇨ "Produktsuche nach Elementen - Kopf-, Fußbereich" auf Seite D-60

#### Register Kundenartikel
- **Sta**: Statusanzeige der Position.
  - ⇨ “Symbolerklärung" auf Seite D-76
  - **Technische Info**: Anzeigefeld
- **Artikel**: Artikelnummer.
  - **Technische Info**: Anzeigefeld, DB-Feld: artikel.artnr
- **Bezeichnung**: Artikelbezeichnung.
  - **Technische Info**: Anzeigefeld, DB-Feld: artikel.artbez1
- **Glas1, Glas2, Glas3**: Nummern der Glasartikel. Die Anzahl der Gläser ist abhängig vom Artikel. Bei Artikeln mit mehr als drei Gläsern werden nur die ersten drei Gläser der Scheibe angezeigt.
  - **Technische Info**: Anzeigefelder
- **SZR1, SZR2**: Größe des Abstandhalters im ersten und zweiten Scheibenzwischenraum in Millimeter. Die Anzahl der Abstandhalter ist abhängig von der Anzahl der Scheiben im ISO. Bei Artikeln mit mehr als zwei Abstandhaltern werden nur die ersten zwei Abstandhalter angezeigt.
  - **Technische Info**: Anzeigefelder
- **Zwischenraum**: Nummer und Bezeichnung des Abstandhalters oder der Folie. Bei Artikeln mit mehr als einem Abstandhalter oder einer Folie, wird nur der erste Abstandhalter bzw. die erste Folie angezeigt.
  - **Technische Info**: Anzeigefeld
- **Gas**: Nummer des Gases im Zwischenraum.
  - **Technische Info**: Anzeigefeld

### Produktsuche nach Elementen – Bezeichnungen
**Pfad:** `Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <Shift> + <F8> > Suchkriterien eingeben > <F3> > Register Bezeichnungen`

**Abb. D-20: Produktsuche nach Elementen - Bezeichnungen**

In diesem Register werden Informationen zu den Bezeichnungen der Artikel angezeigt, die den Suchkriterien entsprechen.
- Mit `<F2>` wechseln Sie die Register in der Trefferliste.
- Mit den Pfeiltasten und `<Bild runter>`, `<Bild hoch>` navigieren Sie in der Trefferliste.

#### Kopf-, Fußbereich
Die Felder im Kopf- und Fußbereich sind zum Dialog Produktsuche nach Elementen - Kopf-, Fußbereich beschrieben:
⇨ "Produktsuche nach Elementen - Kopf-, Fußbereich" auf Seite D-60

#### Register Bezeichnungen
- **Produkt**: Artikelnummer.
  - **Technische Info**: Anzeigefeld, DB-Feld: artikel.artnr
- **Bezeichnung**: Artikelbezeichnung.
  - **Technische Info**: Anzeigefeld, DB-Feld: artikel.artbez1
- **Hauptbezeichnung**: Hauptbezeichnung des Artikels.
  - **Technische Info**: Anzeigefeld, DB-Feld: artikel.artbez2
- **Internbez.**: Interne Artikelbezeichnung.
  - **Technische Info**: Anzeigefeld, DB-Feld: artikel.artbez3
- **Kurzbezeichnung**: Kurzbezeichnung des Artikels.
  - **Technische Info**: Anzeigefeld, DB-Feld: artikel.kurzbez

### Produktsuche nach Elementen – Techn. Werte
**Pfad:** `Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <Shift> + <F8> > Suchkriterien eingeben > <F3> > Register Technische Werte`

**Abb. D-21: Produktsuche nach Elementen - Techn. Werte**

In diesem Register werden Informationen zu den technischen Werten der Artikel angezeigt, die den Suchkriterien entsprechen.
- Mit `<F2>` wechseln Sie die Register in der Trefferliste.
- Mit den Pfeiltasten und `<Bild runter>`, `<Bild hoch>` navigieren Sie in der Trefferliste.

#### Kopf-, Fußbereich
Die Felder im Kopf- und Fußbereich sind zum Dialog Produktsuche nach Elementen - Kopf-, Fußbereich beschrieben:
⇨ "Produktsuche nach Elementen - Kopf-, Fußbereich" auf Seite D-60

#### Register Techn. Werte
Die Spalten sind teilweise zu den Dialogen Produktsuche nach Elementen – Kundenartikel und Produktsuche nach Elementen – Bezeichnungen beschrieben:
- ⇨ "Produktsuche nach Elementen - Kundenartikel" auf Seite D-62
- ⇨ "Produktsuche nach Elementen - Bezeichnungen" auf Seite D-64

Zusätzlich werden folgende Spalten angezeigt:
- **Gas 1, Gas 2**: Nummern der Gase in den Zwischenräumen.
  - **Technische Info**: Anzeigefelder
- **Ug-Wert**: Wärmedurchgangskoeffizient.
  - **Technische Info**: Anzeigefeld
- **g-Wert**: Energiedurchlasskoeffizient (Gesamtdurchlassgrad).
  - **Technische Info**: Anzeigefeld
- **dB-Wert**: Schalldämmungs-Wert der Position in Dezibel.
  - **Technische Info**: Anzeigefeld
- **Tv-Wert**: Lichtdurchlässigkeit (Lichttransmissionsgrad).
  - **Technische Info**: Anzeigefeld

## Objekt-Suche
**Pfad:** `Verkauf > Auftragserfassung > Feld Objekt > <F9>`

In diesem Dialog suchen Sie nach Objekten.
Wenn Sie im Feld **Objekt** die Suche öffnen, werden Ihnen alle Objekte des Marktpartners in der Trefferliste angezeigt. Über die Filterkriterien können Sie die Trefferliste beschränken.

> **Objekt vor Marktpartner wählen**
> Sie können mit `<Strg>` + `<F11>` im Feld **Kunde** nach Objekten suchen, bevor Sie den Marktpartner wählen. Im Dialog **Objekt-Suche** werden dann alle Objekte angezeigt. Wenn Sie ein Objekt wählen, werden in einem weiteren Dialog nur noch die Kunden angezeigt, denen das aktuelle Objekt zugeordnet ist. Wenn das Objekt nur einem Marktpartner zugeordnet ist, wird dieser automatisch herangezogen.

Wenn Sie ein Objekt wählen, werden je nach Systemkonfiguration einige Daten des gewählten Marktpartners oder Kreditors ggf. überschrieben, z. B. Lieferadresse, Kostenstelle, Rabatte.

Die Ergebnisse der Suche werden in der Trefferliste angezeigt.

In diesem Dialog finden Sie folgende Register:
- "Objekt-Suche - Kopf-, Fußbereich" auf Seite D-67
- "Objekt-Suche - Adresse" auf Seite D-69
- "Objekt-Suche - Identifikation" auf Seite D-70

### Objekt-Suche – Kopf-, Fußbereich
**Pfad:** `Verkauf > Auftragserfassung > Feld Objekt > <F9>`

**Abb. D-22: Objekt-Suche – Kopf**

In diesem Dialog suchen Sie nach Objekten anhand von verschiedenen Suchkriterien. Es werden nur die Objekte angezeigt, die dem Marktpartner zugeordnet sind, der im Feld **Kunde** in der Auftragserfassung ausgewählt wurde. Über die Filterkriterien können Sie die Trefferliste beschränken.

#### Suchfelder
Im Kopfbereich geben Sie die Suchkriterien an. Die Treffer der Suche werden in den Registern angezeigt. Je nach Systemkonfiguration werden nicht alle der folgenden Felder angezeigt.

- **Ab Objekt**: Startnummer, ab der aufsteigend nach Objekten gesucht wird.
  - **Technische Info**: numerisches Feld, DB-Feld: objekte.objnr
- **Objekt-Kürzel**: Zweibuchstabiges Kürzel des Objekts aus den Stammdaten, das auf dem Scheibenetikett ausgewiesen werden kann.
  - **Technische Info**: alphanumerisches Feld, DB-Feld: objekte.etitxt2
- **Bezeichnung**: Objektbezeichnung.
  - **Technische Info**: alphanumerisches Feld, DB-Feld: objekte.bez
- **Externe Nummer**: Objektnummer, die vom Kunden vorgegeben wird.
  - **Technische Info**: alphanumerisches Feld, DB-Feld: objekte.exobjnr
- **Etikettext**: Text zum Objekt, der auf dem Scheibenetikett ausgewiesen wird.
  - **Technische Info**: alphanumerisches Feld, DB-Feld: objekte.etitxt1
- **Alle**: Angabe, ob für das Objekt Verglasungsarbeiten vorgesehen sind:
  - J: Für das Objekt sind Verglasungsarbeiten geplant.
  - N: Für das Objekt sind keine Verglasungsarbeiten geplant.
  - **Technische Info**: Toggle-Feld, DB-Feld: objekte.vergl
- **Vertreter**: Mitarbeiternummer, dem das Objekt zugeordnet ist. Der Vertreter wird z. B. in die Provisionsberechnung einbezogen. Wenn Sie eine Nummer angeben, wird der Name des Mitarbeiters im Klartext angezeigt.
  - **Technische Info**: numerisches Feld, DB-Feld: objekte.vertreter
- **Route**: Routennummer, die dem Objekt zugeordnet ist. Wenn Sie eine Nummer angeben, wird die Bezeichnung der Route im Klartext angezeigt.
  - **Technische Info**: numerisches Feld, DB-Feld: objekte.routenr
- **Verglasungsmitarbeiter**: Mitarbeiternummer für die Verglasungsarbeiten. Wenn Sie eine Nummer angeben, wird der Name des Mitarbeiters im Klartext angezeigt.
  - **Technische Info**: numerisches Feld, DB-Feld: objekte.verglmanr
- **Kostenstelle**: Kurzbezeichnung der Kostenstelle für das Objekt. Wenn Sie eine Kurzbezeichnung angeben, wird der Name der Kostenstelle im Klartext angezeigt.
  - **Technische Info**: alphanumerisches Feld, DB-Feld: objekte.kostenst

#### Fußbereich
- **Neue Suche**: Löscht alle Suchkriterien für eine neue Suche.

### Objekt-Suche – Adresse
**Pfad:** `Verkauf > Auftragserfassung > Feld Objekt > <F9> > Register Adresse`

**Abb. D-23: Objekt-Suche – Adresse**

In diesem Register werden die adressbezogenen Daten der Objekte angezeigt, die den Suchkriterien entsprechen.
Die Suchkriterien geben Sie im Kopfbereich an.
- Mit `<Shift>` + `<F2>` wechseln Sie die Register in der Trefferliste.
- Mit den Pfeiltasten und `<Bild runter>`, `<Bild hoch>` navigieren Sie in der Trefferliste.
- Mit `<Strg>` + `<R>` löschen Sie die eingegebenen Suchkriterien.

#### Suchfelder
Die Felder im Kopfbereich sind zum Dialog Objekt-Suche – Kopf-, Fußbereich beschrieben:
⇨ "Objekt-Suche – Kopf-, Fußbereich" auf Seite D-67

#### Register Adresse
Die Spalten in der Trefferliste entsprechen den Feldern im Kopfbereich. Zusätzlich werden folgende Spalten angezeigt:
- **Kürzel**: Die Spalte entspricht dem Feld **Objekt-Kürzel** aus dem Kopfbereich.
  - ⇨ "Objekt-Kürzel" auf Seite D-67
  - **Technische Info**: Anzeigefeld, DB-Feld: objekte.etitxt2
- **Vertreter, Name**: Die Spalten entsprechen dem Feld **Vertreter** im Kopfbereich. Der Name des Vertreters wird aus den Mitarbeiterstammdaten herangezogen.
  - ⇨ "Vertreter" auf Seite D-68
  - **Technische Info**: Anzeigefelder, DB-Feld: objekte.vertreter
- **Routenr., Route**: Die Spalten entsprechen dem Feld **Route** im Kopfbereich. Die Routenbezeichnung wird aus dem Routenstamm herangezogen.
  - ⇨ "Route" auf Seite D-68
  - **Technische Info**: Anzeigefelder, DB-Feld: objekte.routenr

#### Fußbereich
- **Neue Suche**: Löscht alle Suchkriterien für eine neue Suche.

### Objekt-Suche – Identifikation
**Pfad:** `Verkauf > Auftragserfassung > Feld Objekt > <F9> > Register Identifikation`

**Abb. D-24: Objekt-Suche – Identifikation**

In diesem Register werden die Identifikationsmerkmale der Objekte angezeigt, die den Suchkriterien entsprechen.
Die Suchkriterien geben Sie im Kopfbereich an.
- Mit `<Shift>` + `<F2>` wechseln Sie die Register in der Trefferliste.
- Mit den Pfeiltasten und `<Bild runter>`, `<Bild hoch>` navigieren Sie in der Trefferliste.
- Mit `<Strg>` + `<R>` löschen Sie die eingegebenen Suchkriterien.

#### Suchfelder
Die Felder im Kopfbereich sind zum Dialog Objekt-Suche – Kopf-, Fußbereich beschrieben:
⇨ "Objekt-Suche - Kopf-, Fußbereich" auf Seite D-67

#### Identifikation
Die Spalten in der Trefferliste entsprechen den Feldern im Kopfbereich. Zusätzlich werden folgende Spalten angezeigt:
- **Kostenst., Bezeichnung**: Kurzbezeichnung und Bezeichnung der Kostenstelle, die dem Objekt zugeordnet ist. Der Name der Kostenstelle wird aus den Stammdaten herangezogen.
  - **Technische Info**: Anzeigefelder, DB-Feld: objekte.kostenst
- **Vergl.**: Angabe, ob für das Objekt Verglasungsarbeiten vorgesehen sind:
  - J: Für das Objekt sind Verglasungsarbeiten geplant.
  - N: Für das Objekt sind keine Verglasungsarbeiten geplant.
  - **Technische Info**: Anzeigefeld, DB-Feld: objekte.vergl
- **VergIMA, Name**: Mitarbeiternummer und Name des Mitarbeiters für die Verglasungsarbeiten. Der Name des Mitarbeiters wird aus den Stammdaten herangezogen.
  - **Technische Info**: Anzeigefelder, DB-Feld: objekte.verglmanr

## Werteingabe – Erweiterte Suche
**Pfad:** `Verkauf > Auftragserfassung > Feld Auftrag > <Shift> + <F5>` oder `<Strg> + <E>`

In diesen Dialogen können Sie anhand eines bestimmten Kriteriums nach Aufträgen suchen. Der Dialog wird für jedes Kriterium über eine andere Tastenkombination aufgerufen. Der Suchdialog Werteingabe ist für alle Kriterien analog aufgebaut, unterscheidet sich jedoch je nach Kriterium in der Bezeichnung des Suchfeldes.
In diesem Abschnitt sind folgende Dialoge erklärt:
- "Werteingabe – Suche nach Kommission" auf Seite D-72
- "Werteingabe – Suche nach Originalnummer" auf Seite D-73

### Werteingabe – Suche nach Kommission
**Pfad:** `Verkauf > Auftragserfassung > Feld Auftrag > <Shift> + <F5>`

**Abb. D-25: Suche nach Kommission**

In diesem Dialog suchen Sie Aufträge anhand des Kommissionstextes.

#### Werteingabe
- **Kommision**: Kommissionstext oder Teil des Kommissionstextes. Mit einem Stern `*` vor dem Suchwort weiten Sie die Suche auf alle Aufträge aus, in denen der Kommissionstext enthalten ist.

#### Auswahldialog
In diesem Dialog werden alle Aufträge mit dem angegebenen Kommissionstext angezeigt.
Mit den Pfeiltasten und `<Bild runter>`, `<Bild hoch>` navigieren Sie in dem Auswahldialog.
- **Kommision**: Kommissionstext der Position.
- **Kunde**: Kundenname.
- **Auftrag**: Auftragsnummer.

Mit `<Enter>` wird die Auftragsnummer des markierten Eintrags in die Auftragserfassung übernommen.

### Werteingabe – Suche nach Originalnummer
**Pfad:** `Verkauf > Auftragserfassung > Feld Auftrag > <Strg> + <E>`

**Abb. D-26: Suche nach Originalnummer**

In diesem Dialog suchen Sie Aufträge, die mit Bezug zu einem Original-Auftrag erfasst wurden. Sie können die Aufträge anhand der Original-Auftragsnummer suchen, auf die sie sich beziehen.

#### Werteingabe
- **Originalnummer**: Originalnummer des Auftrags, die als Bezug bei der Vorgangserfassung angegeben wurde. Mit `<F9>` können Sie nach einer Nummer suchen.

#### Suchdialog
Im Feld **Originalnummer** im Dialog **Werteingabe** öffnen Sie mit `<F9>` die Selo-Suche nach Original-Aufträgen.
- **Suche**: Original-Auftragsnummer, ab der nach Vorgängen gesucht wird. Wenn Sie keine Nummer eingeben, werden in der Trefferliste alle verfügbaren Original-Aufträgen angezeigt.

Mit den Pfeiltasten und `<Bild runter>`, `<Bild hoch>` navigieren Sie in der Trefferliste.
- **Original-Auftragsnummer**: Auftragsnummer des originalen Auftrags.
- **Haus**: Mandantennummer (Hausnummer).
- **Nummer**: Auftragsnummer des neuen Auftrags.
- **Subnr**: Subnummer des neuen Auftrags.
- **Kunde**: Kundenname des neuen Auftrags.

Wenn Sie eine Originalnummer mit `<Enter>` wählen, öffnet sich ein Auswahldialog, in dem alle Aufträge angezeigt werden, die sich auf diese Original-Auftragsnummer beziehen.

#### Auswahldialog
In diesem Dialog werden alle Aufträge mit Bezug auf den Auftrag mit der angegebenen Original-Auftragsnummer angezeigt.
Mit den Pfeiltasten und `<Bild runter>`, `<Bild hoch>` navigieren Sie in dem Auswahldialog.
- **Auftrag**: Auftragsnummer.
- **Original-Auftrag**: Auftragsnummer des originalen Auftrags.
- **Kunde**: Kundenname.

Mit `<Enter>` wird der markierte Auftrag in der Auftragserfassung geöffnet.

# Vorgangsverwaltung

In der Vorgangsverwaltung werden alle Dialoge und Funktionen beschrieben, mit der Sie Vorgänge bearbeiten können. In diesem Part erfassen und bearbeiten Sie die Vorgänge für den Verkauf, z. B. Angebote und Aufträge.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Symbolerklärung" auf Seite D-76
- "Schnellerfassung" auf Seite D-79
- "Angebotserfassung" auf Seite D-80
- "Preislose Erfassung" auf Seite D-81
- "Auftragserfassung" auf Seite D-82
- "Auftragspositionen" auf Seite D-113
- "Hauswechsel" auf Seite D-137
- "Neue Lieferadresse" auf Seite D-138
- "Endkundenanschrift" auf Seite D-140
- "Marktpartner-Info" auf Seite D-142
- "Ansprechpartner" auf Seite D-144
- "Storno" auf Seite D-145
- "Mitarbeiterzuordnung - Spezial" auf Seite D-146
- "Konfigurierbare Felder" auf Seite D-146
- "Übersicht" auf Seite D-147
- "Produktsets (Sash Master)" auf Seite D-148
- "Artikel-Maßangaben" auf Seite D-150
- "Bestandsprognose" auf Seite D-151
- "Produktaustausch" auf Seite D-154
- "Reklamation" auf Seite D-158
- "Auftragsarten" auf Seite D-159
- "Artikelangaben für bemaßte Varianten" auf Seite D-161
- "Varianten- und Farben-/Dickenauswahl" auf Seite D-164
- "Private Felder" auf Seite D-165
- "Fremddaten-Import" auf Seite D-166
- "Dokumentenarten" auf Seite D-168
- "Dokumentenartenzuordnung" auf Seite D-169
- "Dateizuordnung" auf Seite D-171
- "DXF Import" auf Seite D-172
- "Änderungs-Protokoll" auf Seite D-173
- "Lieferterminänderungs-Protokoll" auf Seite D-175
- "Modellkatalog" auf Seite D-176
- "Modell-Maßangaben" auf Seite D-177
- "Zahlungsverwaltung" auf Seite D-179
- "Zahlungsplan" auf Seite D-181
- "Fehlerinformationssystem" auf Seite D-183
- "Produktionsmonitor" auf Seite D-185

## Symbolerklärung
In diesem Abschnitt werden die Kennzeichen für den Dialogmodus, den Positionsstatus und das Positionskennzeichen beschrieben.

### Dialogmodus
Der Dialogmodus wird in der Titelzeile des Dialogs angezeigt.

**Tab. D-1: Dialogmodus**

| Symbol | Symbolbeschreibung | Bedeutung |
| :--- | :--- | :--- |
| `+` | Dialog mit Kreuzchen | In diesem Modus können Sie neue Datensätze anlegen. |
| 📝 | Dialog mit Stift | In diesem Modus können Sie einen Datensatz bearbeiten. |
| ⚠️ | Gelbes Dreieck mit Ausrufezeichen | In diesem Modus können Sie den Datensatz nicht bearbeiten, z. B., weil er bereits an die Produktion übergeben wurde. |
| 🔍 | Suche | In diesem Modus können Sie nach Datensätzen suchen. |

### Positionsstatus und Positionskennzeichen
Der Positionsstatus wird im Register **Positionen** vor dem Feld **Pos** angezeigt.

**Tab. D-2: Positionsstatus**

| Symbol | Symbolbeschreibung | Bedeutung |
| :--- | :--- | :--- |
| 🟢 | grün | Die Position kann frei bearbeitet werden, da die Produktion noch nicht begonnen hat. |
| 🟡 | gelb | Die Position oder Unterteile der Position sind bestellt und die Bestellung ist gedruckt worden. |
| 🔴 | rot | Die Position ist in der Produktion verplant. Sie kann nicht mehr bearbeitet werden. |
| 🔴¾ 🔵¼ | drei Viertel rot, ein Viertel blau | Die Position ist teilweise geliefert. |
| 🔴½ 🔵½ | halb rot, halb blau | Die Position ist komplett geliefert. |
| 🔴¼ 🔵¾ | zwei Viertel rot, zwei Viertel blau | Die Position ist teilfakturiert. |
| 🔵 | blau | Die Position ist komplett fakturiert. |
| ❌ | Kreuz rot | Die Position wird gelöscht. |

Das Positionskennzeichen wird vor dem Feld **Pos** angezeigt.

**Tab. D-3: Positionskennzeichen**

| Symbol | Symbolbeschreibung | Bedeutung |
| :--- | :--- | :--- |
| ⭐ (Gelber Stern) | Gelber Stern | Die Produktbemaßung sowie zusätzliche Bearbeitungen des Artikels sind für den ausgewählten Kunden hinterlegt. Nach dem Speichern des kundenindividuellen Artikels wird ein grüner Stern angezeigt. ⇨ "Artikelangaben für bemaßte Varianten" auf Seite D-161; ⇨ Help Cards, "Artikel fixieren" auf Seite D-29 |
| ⭐ (Grüner Stern) | Grüner Stern | Der Artikel ist kundenindividuell definiert und kann nur für den jeweiligen Kunden erfasst werden. In einem kundenindividuellen Artikel können Sie den Stücklistenaufbau mit zusätzlichen Bearbeitungen, Artikeln, Maßänderungen und weiteren kundenspezifischen Wünschen speichern. ⇨ "Artikelangaben für bemaßte Varianten" auf Seite D-161 |
| 🧾 | Modell | Die Position ist mit Modell erfasst. ⇨ "Modell-Maßangaben" auf Seite D-177 |
| 🪟 | Fenster mit Sprossen | Die Position ist mit Sprossen erfasst. ⇨ "Sprossenerfassung" auf Seite D-226 |
| 🧾🪟 | Modell mit Sprossen | Die Position ist mit Modell und Sprossen erfasst. ⇨ "Modell-Maßangaben" auf Seite D-177; ⇨ "Sprossenerfassung" auf Seite D-226 |

### Positionsstatus und Vorgangsstatus in Textform
Der Status des Vorgangs und der erfassten Positionen kann zusätzlich in Textform angezeigt werden.

**Abb. D-27: Statusanzeigen in Textform**

- **Vorgangsstatus (A)**: Wenn sich der Vorgangsstatus ändert, wird der aktuelle Status in der Titelzeile des Dialogs angezeigt, z. B. (Teil-) produziert, GLOBALKORREKTUR, VERSANDPLANUNG LIEGT VOR.
- **Positionsstatus (B)**: Wenn sich der Positionsstatus ändert, wird der Status der entsprechenden Position im rechten Teil des Dialogs auf Positionsebene angezeigt, z. B. Verpackt, FIXIERT, Lokal-Korrektur. Jede Position kann einen anderen Status haben. Der angezeigte Positionsstatus gilt jeweils für die markierte Position.

Für weitere Informationen zu den unterschiedlichen Statusanzeigen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

## Schnellerfassung
**Pfad:** `Verkauf > Schnellerfassung`

**Abb. D-28: Schnellerfassung – Kopfdaten**

In diesem Dialog erfassen Sie schnell einen Auftrag oder ein Angebot. Diese vereinfachte Form der Vorgangserfassung bietet nur einen eingeschränkten Zugriff auf die Funktionsmöglichkeiten und die Auswahl an Artikeln, Modellen und den Stücklistenaufbau.
Der Dialog ist nur kundenspezifisch freigeschaltet.
Für weitere Informationen zu diesem Modul kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

## Angebotserfassung
**Pfad:** `Verkauf > Angebotserfassung`

**Abb. D-29: Angebotserfassung**

In diesem Dialog erfassen und bearbeiten Sie Angebote. Mit `<Enter>` wird die Angebotsnummer vom System vergeben. Um ein erfasstes Angebot zu öffnen, geben Sie im Feld **Angebot** die Angebotsnummer ein oder wechseln mit `<F9>` in den Suchdialog.

Wenn Sie bei Angeboten einen Liefertermin eintragen, können Sie je nach Systemkonfiguration einen Wiedervorlage-Termin anlegen, um das Angebot nachzuverfolgen. Wenn der Wiedervorlage-Termin erreicht ist, wird beim Programmstart eine Meldung angezeigt oder eine Erinnerungs-Mail zugestellt.
⇨ "Wiedervorlage" auf Seite D-400

Sie können aus jedem Angebot einen Auftrag erstellen, indem Sie in der Auftragserfassung einen Bezug zu dem Angebot herstellten. Wenn Sie in der Auftragserfassung die Angebotsnummer in das Feld **Bezug** eintragen, dann werden die Daten aus dem Angebot in den Auftrag übernommen.

Der Dialog **Angebotserfassung** ist wie der Dialog **Auftragserfassung** aufgebaut. Abweichungen werden zum Dialog **Auftragserfassung** beschrieben:
⇨ "Auftragserfassung" auf Seite D-82

## Preislose Erfassung
**Pfad:** `Verkauf > Preislose Erfassung`

**Abb. D-30: Preislose Erfassung**

In diesem Dialog erfassen Sie Kundenaufträge ohne Preise. Bei Ladenaufträgen verhindern Sie auf diese Weise, dass Kunden die Einkaufspreise einsehen können. Zusätzlich können auch Mitarbeiter, die die Betriebspreise nicht einsehen können, Aufträge erfassen. Diese Aufträge werden nachträglich von einem Sachbearbeiter geprüft.

Die Preisberechnung des Auftrags erfolgt verdeckt, wenn Sie den Auftrag speichern. Der Vorgang wird unter der vom System vergebenen Auftragsnummer gespeichert.

Der Dialog **Preislose Erfassung** ist wie der Dialog **Auftragserfassung** aufgebaut:
⇨ "Auftragserfassung" auf Seite D-82

## Auftragserfassung
**Pfad:** `Verkauf > Auftragserfassung`

In diesem Dialog erfassen und bearbeiten Sie Aufträge. Der Dialog Auftragserfassung ist in drei Teile gegliedert:
- **Kopfbereich**: In diesem Bereich werden die Kundendaten und Lieferbedingungen angezeigt.
- **Positionsebene**: In diesem Bereich werden Informationen zu den Auftragspositionen angezeigt.
- **Fußbereich**: In diesem Bereich werden Informationen zu den Auftragssummen, den Rabatten und Zuschlägen angezeigt.

In diesem Dialog finden Sie folgende Register:
- "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-83
- "Auftragserfassung - Anschriften" auf Seite D-90
- "Auftragserfassung – Eigenschaften" auf Seite D-93
- "Auftragserfassung – Verschiedenes" auf Seite D-99
- "Auftragserfassung – Summen" auf Seite D-104
- "Auftragserfassung – Detailansicht Rabatte" auf Seite D-108

Im Bereich **Positionen** finden Sie folgende Register:
- "Auftragspositionen - Allgemein" auf Seite D-113
- "Auftragspositionen - Eigensch." auf Seite D-126
- "Auftragspositionen – Preise" auf Seite D-131
- "Auftragspositionen - Status" auf Seite D-134
- "Auftragspositionen – Kosten" auf Seite D-136

### Auftragserfassung – Kopf-, Fußbereich
**Pfad:** `Verkauf > Auftragserfassung`

**Abb. D-31: Auftragserfassung - Positionen**

In diesem Dialog erfassen Sie die Kopfdaten des Auftrags, z. B. die Kundendaten und Lieferbedingungen. Im Fußbereich werden Informationen zu den Auftragssummen angezeigt.

- Mit `<Enter>` wechseln Sie in das nächste Feld im Kopfbereich. Im letzten Feld des Kopfbereichs, dem Feld **Objekt**, wechseln Sie mit `<Enter>` in das Register **Positionen**.
- Aus den Feldern **Eingang**, **Rechnungstyp** oder **Objekt** können Sie mit `<F2>` in die Positionsebene zu den Register **Anschriften**, **Eigenschaften** und **Verschiedenes** wechseln.
  - ⇨ "Auftragserfassung - Anschriften" auf Seite D-90
  - ⇨ "Auftragserfassung - Eigenschaften" auf Seite D-93
  - ⇨ "Auftragserfassung – Verschiedenes” auf Seite D-99
- Mit `<Ende>` wechseln Sie aus der Positionsebene im Register **Allgemein** in den Fußbereich und schließen die Auftragserfassung ab.

#### Kopfbereich
- **Auftrag**: Auftragsnummer. Die Nummer wird vom System aus dem zugeordneten Nummernkreis vergeben. Wenn Sie eine bereits vergebene Nummer eintragen, wird der entsprechende Auftrag geöffnet. Je nach Status können Sie den Auftrag bearbeiten. Der Feldname variiert je nach Dialog, in dem Sie den Vorgang erfassen, z. B. **Angebot** in der Angebotserfassung. Wenn Sie die Vorgangsnummer eingeben, wird bei einigen Vorgangsarten ein weiteres Feld angezeigt, z. B. bei Rechnung oder Lieferschein. In diesem Feld wird die Subnummer zum Vorgang angezeigt. Sie können eine bereits vergebene Subnummer wählen oder die nächste freie Nummer vom System vergeben lassen.
  - **Technische Info**: Pflichtfeld, numerisches Feld, DB-Feld: kauf.auftrnr

> **Automatische Vergabe von Vorgangsnummern**
> Wenn Sie einen neuen Vorgang erfassen, wird die Vorgangsnummer automatisch vom System vergeben. Bei Rechnungen wird zunächst eine interne, temporäre Nummer vergeben. Auf diese Weise wird vom System sicher gestellt, dass Rechnungen fortlaufend durchnummeriert sind.

- **Kunde**: Kundennummer. Wenn Sie eine Nummer angeben, werden Name und Ort des Kunden im Klartext angezeigt. Es können nur Aufträge für aktive Kunden erfasst werden.
  - **Technische Info**: Pflichtfeld, numerisches Feld, Anzeigefelder, DB-Feld: kauf.kunr, kauf.orgname

- **Grund**: Begründung für eine Terminänderung. Das Feld **Grund** wird nur angezeigt, wenn Sie den Liefertermin in einem bereits erfassten Auftrag ändern.
  - **Technische Info**: alphanumerisches Feld, DB-Feld: kaufltedit.text

- **Bezug**: Vorgangsnummer, auf die Bezug genommen wird. Sie können ein Angebot, einen Auftrag, eine Lieferantenanfrage oder eine Bestellung als Bezug auswählen. Sie können alle Daten des Bezugsvorgangs oder nur die Kopfdaten des Bezugsvorgangs übernehmen. Mit `<F9>` öffnen Sie den Dialog **Suche Bezugsvorgang**:
  - ⇨ "Suche Bezugsvorgang" auf Seite D-45
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.referenz

- **Vorgangsart für den Bezug vorauswählen**: Je nach Systemkonfiguration ist es möglich, eine der Vorgangsarten als Vorauswahl für die Bezugserfassung festzulegen:
  - Mit `<F8>` wird im Feld **Bezug** die als Standard konfigurierte Vorgangsart im Feld angezeigt.
  - Mit `<F9>` öffnen Sie einen Auswahldialog mit allen Vorgangsarten, auf die Bezug genommen werden kann. Mit den Pfeiltasten können Sie eine Vorgangsart wählen.
  - Mit `<Enter>` bestätigen Sie die Auswahl.
  - Im Feld **Bezug** wird die Nummer des aktuellen Marktpartners angezeigt.
  - Wenn Sie den aktuellen Marktpartner als Vorauswahl festlegen möchten, dann bestätigen Sie mit `<Enter>`.
  - Wenn Sie einen anderen Marktpartner als Vorauswahl festlegen möchten, dann öffnen Sie mit `<F9>` den Dialog **Marktpartnersuche**, um einen Marktpartner auszuwählen. Alternativ können Sie die Marktpartnernummer direkt im Feld angeben. Mit `<Enter>` bestätigen Sie die Auswahl.
  - Das Feld **Bezug** ist leer. Wenn Sie jetzt den Dialog **Suche Bezugsvorgang** öffnen, dann sind die Vorgangsart und der Marktpartner, den Sie festgelegt haben, als Suchkriterien vorausgewählt.

- **Vorgang mit Bezug erfassen**:
  - Mit `<F9>` öffnen Sie den Dialog **Suche Bezugsvorgang**, um einen Bezugsvorgang zu den angegebenen Kriterien auszuwählen. Alternativ können Sie die Vorgangsnummer direkt im Feld angeben.
  - Mit `<Enter>` bestätigen Sie die Auswahl. Sie können alle Daten des Bezugsvorgangs oder nur die Kopfdaten des Bezugsvorgangs übernehmen.

- **Haus**: Firmennummer und Mandantennummer (Hausnummer), in der der Auftrag angelegt wird. Das Feld **Haus** ist nur freigeschaltet, wenn Sie mit interner Mandantentrennung arbeiten. Die Firmennummer wird automatisch aus den Systemstammdaten herangezogen und in einem Anzeigefeld angezeigt.
  - **Technische Info**: numerische Felder, DB-Felder: kauf.company, kauf.hausnr

- **Erf. Datum**: Erfassungsdatum. Standardmäßig ist das Feld mit dem aktuellen Datum vorbelegt. Wenn Sie den Eintrag ändern wollen, müssen Sie das neue Datum zweimal eingeben.
  - **Technische Info**: Pflichtfeld, Datumsfeld, DB-Feld: kauf.edat

- **Knd-Bestnr**: Externe Kundenbestellnummer. Für Aufträge aus einem anderen Haus steht in diesem Feld die Auftragsnummer des sendenden Hauses.
  - **Technische Info**: alphanumerisches Feld, DB-Feld: kauf.exaufnr

- **Termin**: Gewünschter Liefertermin des Kunden. Im ersten Feld können Sie die Kalenderwoche angeben. Im zweiten Feld können Sie das Datum im Format TT.MM.JJJJ angeben. Wenn Sie die Kalenderwoche und die Route angegeben haben, können Sie sich im zweiten Feld die möglichen Termine mit `<F9>` in einem Auswahldialog anzeigen lassen. Es werden nur die Termine angezeigt, die für die Tourenplanung in den Stammdaten angelegt sind. Ob alle Auftragspositionen zum gewünschten Liefertermin komplett bereitgestellt werden können, wird vom System nach der Auftragseinlastung in das Produktionssystem geprüft. Kann bis zum gewünschten Termin nicht geliefert werden, meldet das System diesen Umstand per E-Mail an den Auftragserfasser und verschiebt das Datum auf den nächstmöglichen Liefertermin.
  - **Technische Info**: Pflichtfeld, numerisches Feld, Datumsfeld, DB-Felder: kauf.kwideal, kauf.ltideal

> **Angebot mit Termin**
> Das System kann so konfiguriert werden, dass ein Angebot mit Termin zu einer Wiedervorlage führt. Der Erfasser erhält an dem entsprechenden Datum bei Programmstart eine Mitteilung, damit Angebote nachverfolgt werden können.

- **Route**: Routennummer. In der Routenauswahl sind die Fahrstrecken sowie die jeweiligen Routentage aufgelistet. Sie können in den Kundenstammdaten eine Hauptroute und drei alternative Routen hinterlegen. Die Route wird anhand der Kunden-, Adressdaten und Systemkonfiguration aus den Stammdaten ermittelt. Wenn die Via-Plant-Funktion konfiguriert ist, wählen Sie mit `<F5>` das Haus, über das die Auslieferung organisiert werden soll. Für Informationen zur Via-Plant-Funktion kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.
  - **Technische Info**: Pflichtfeld, numerisches Feld, DB-Feld: kauf.routenr
- **Geplant**: Anzeige des geplanten Lieferdatums. Der geplante Auslieferungstermin wird anhand verschiedener Daten, z. B. Handlingszeit, Fahrtdauer und Kapazitätsplanung, ermittelt und im Feld **Geplant** als geplantes Auslieferungsdatum eingetragen.
  - **Technische Info**: Anzeigefeld, DB-Feld: kauf.ltplan
- **Knd-Pos**: Angaben zur Position aus der Positionsliste des Kunden. Die Kundenpositionen werden im Register **Allgemein** in dem Feld **Ku.Pos.** angezeigt:
  - **Pos**: Das Feld **Ku.Pos** auf Positionsebene wird freigeschaltet. Die Auftragspositionen können nach kundenindividuellen Positionsbezeichnungen erfasst werden, z. B. 1.1, 4.2, A_1, G_4.
  - **Typ**: Die Positionen werden nach Glastypen erfasst.
  - **keine**: Das Feld **Ku.Pos** ist auf Positionsebene gesperrt. Die kundenindividuellen Positionsbezeichnungen können nicht verwendet werden.
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.kndposkz
- **Term. Art**: Information über die Terminierungsart, die auf den Auftrag gedruckt wird. Wenn als Terminierungsart **Abruf** oder **eilt** ausgewählt ist, dann wird der Termin an A+W Production weiter geleitet. Bei **eilt** wird die Produktion der Ware bei der Einlastung bevorzugt. Bei **Abruf** wird die Produktion so geplant, dass die Ware auf Abruf geliefert werden kann.
  - **(keine Auswahl)**: Terminierungsart ist nicht festgelegt.
  - **Abruf**: Termin auf Abruf.
  - **eilt**: Auftrag wird als Eilauftrag an die Produktion übergeben.
  - **mögl**: möglichst zum Termin.
  - **verbl**: Termin ist verbindlich. Das System kann den gewünschten Liefertermin nicht ändern.
  - **ohne**: ohne verbindlichen Termin.
  - **Auto**: Termin wird automatisch vergeben.
  - **folgt**: Termin folgt. Die Terminabsprache erfolgt erst noch.
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.abrufkz
- **Eingang**: Typ des Kommunikationskanals über den der Auftrag eingegangen ist. Diese Information wird für statistische Auswertungen, Tests und zu Recherchezwecken benutzt.
  - **Vertreter**: Der Auftrag wurde von einem Außendienstmitarbeiter entgegengenommen.
  - **Brief**: Der Auftrag ist per Post eingegangen.
  - **Fax**: Der Auftrag ist per Fax eingegangen.
  - **Telefon**: Der Auftrag ist per Telefon eingegangen.
  - **DFÜ**: Der Auftrag wurde elektronisch übermittelt.
  - **Theke**: Der Auftrag wurde im Geschäft erfasst.
  - **Test**: Der Auftrag wurde nur zu Testzwecken erfasst und geht nicht in die Produktion.
  - **Barverkauf**: Der Auftrag wurde im Geschäft gegen Barzahlung entgegengenommen.
  - **K-Dienst**: Der Auftrag wurde vom Kundendienst entgegengenommen.
  - **Ersatz**: Ein Ersatzauftrag kann ausgestellt werden, wenn der reguläre Auftrag verloren geht.
  - **EURO-Konv**: Funktionalität zur Umstellung auf Euro (nicht auswählbar).
  - **Abschlag**: Sobald eine Abschlagsrechnung erstellt ist, wird vom System die Bezeichnung **Abschlag** in das Feld eingetragen. Der Wert **Abschlag** kann nicht manuell ausgewählt werden.
  - **Schluss**: Sobald eine Schlussrechnung erstellt ist, wird vom System die Bezeichnung **Schluss** in das Feld eingetragen. Der Wert **Schluss** kann nicht manuell ausgewählt werden.
  - **Online**: Der Auftrag ist online eingegangen, z. B. über die Webanwendung oder iQuote.
  - **E-Mail**: Der Auftrag ist per Mail eingegangen.
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.eingang
- **Rechnungstyp**: Angabe, für welche Leistungen die Rechnung erstellt wird. In der Regel werden die Gläser und Montageleistungen gemeinsam berechnet. Auf Wunsch können Sie einzelne Rechnungen erstellen.
  - **Gesamt**: Die Rechnung wird für den kompletten Auftrag erstellt, d. h. für Material und Montageleistungen.
  - **Glas**: Die Rechnung wird nur für das Material des Auftrags erstellt.
  - **Dienstltg**: Die Rechnung wird nur für die Montageleistung des Auftrags erstellt.
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.rechart
- **Objekt**: Objektnummer. Ein Objekt ist dem Marktpartner zugeordnet und kann z. B. eine Baustelle des Kunden sein und eine andere Lieferadresse haben. Mit dem Objekt können Sie besondere Konditionen verknüpfen, die nur für dieses Objekt gelten, z. B. Rabatte oder Zahlungsoptionen. Sie haben die Möglichkeit objektbezogen abzurechnen. Mit `<F9>` öffnen Sie die Objekt-Suche.
  - ⇨ "Objekt-Suche" auf Seite D-66
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.objnr

#### Positionsebene
In diesem Bereich erfassen und bearbeiten Sie die Positionen eines Auftrags. Die Register zu den Auftragspositionen sind separat beschrieben:
⇨ "Auftragspositionen" auf Seite D-113

#### Fußbereich
Im Fußbereich werden die Gesamtauftragswerte der Positionen angezeigt. Sie können einen allgemeinen Rabatt gewähren und den Betrag im Feld **Nettototal** überschreiben. Die Felder können nur betreten werden, wenn Sie die Positionserfassung abgeschlossen haben.
- Mit `<Ende>` wechseln Sie aus der Positionsebene in den Fußbereich.
- Mit `<F2>` öffnen Sie den Dialog Auftragserfassung für die Berechnung von Rabatten und des Nettototalbetrags.
  - ⇨ "Auftragserfassung - Summen" auf Seite D-104

- **Sender**: Anzeige der Hausnummer (Mandantennummer) und der Referenznummer. Die Referenznummer kann die Vorgangsnummer sein, die als Bezug in der Vorgangserfassung für den Vorgang angegeben wurde, oder bei DFÜ-Aufträgen die Auftrags- oder Bestellnummer.
  - **Technische Info**: Anzeigefelder, DB-Felder: kauf.hausnr
- **ST, kg, qm**: Anzeige der Gesamtsumme der Auftragswerte für die Menge in Stück, Gewicht in Kilogramm und Fläche in Quadratmeter.
  - **Technische Info**: Anzeigefelder, DB-Felder: kauf.gesst, kauf.gesm2, kauf.gesgewicht
- **Gesamt**: Anzeige des Gesamtpreises aller Positionen abzüglich der Positionsrabatte aus dem Feld **Abzgl** im Register **Preise**. Der Gesamtpreis wird je nach Preisart unterschiedlich berechnet.
  - ⇨ "Auftragspositionen – Preise" auf Seite D-131
  - ⇨ Preise und Konditionen, "Preisarten" auf Seite K-49
  - **Technische Info**: Anzeigefeld, DB-Feld: kauf.gesnetto
- **Rabatt**: Auf den Gesamtbetrag gewährter Rabatt in Prozent. Bei gewährtem Rabatt wird der Betrag im Feld **Nettototal** angepasst.
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.gesfaktor
- **Nettototal**: Summe aller Positionspreise, inkl. Rabatte und Zuschläge. Wenn Sie den Betrag bearbeiten, wird die Differenz vom System berechnet und im Feld **Allg. Abschlag** oder **Allg. Aufschlag** im Berechnungsdialog angezeigt.
  - ⇨ "Auftragserfassung – Summen" auf Seite D-104
  - Wenn das Feld **Nettototal** leer ist oder der Wert 0 ist, wird eine Abfrage angezeigt, ob Sie den Vorgang überarbeiten wollen. Mit [Ja] gelangen Sie zurück in die Auftragserfassung. Mit [Nein] wird der Dialog **Reklamations-Statistik** geöffnet.
  - ⇨ "Reklamation" auf Seite D-158
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.nettototal
- **+MwSt ()**: Anzeige der Mehrwertsteuer. Im Feld steht der Mehrwertsteuerbetrag, der auf den Nettobetrag aufgeschlagen wird. In den Klammern wird der geltende Mehrwertsteuersatz in Prozent angezeigt.
  - **Technische Info**: Anzeigefeld, DB-Feld: kauf.mwstbetrag
- **Brutto**: Anzeige des Brutto-Gesamtbetrags. Der Betrag wird aus dem Nettobetrag zuzüglich der Mehrwertsteuer berechnet.
  - **Technische Info**: Anzeigefeld, DB-Feld: kauf.gesbrutto
- **D-Beitrag**: Anzeige des Deckungsbeitrags (Bruttogewinn), den die Gesamtmenge der Positionen zur Deckung der Fixkosten beiträgt. Der Deckungsbeitrag ist die Differenz zwischen dem Umsatz und den variablen Kosten der Positionen. Berücksichtigt werden alle Rabatte und Aufschläge.
  - **Technische Info**: Anzeigefeld, DB-Feld: kauf.dbdm
- **%**: Anzeige des Deckungsbeitrags in Prozent.
  - **Technische Info**: Anzeigefeld, DB-Feld: kauf.dbvh
- **Sichern**: Sichert die bereits eingetragenen Daten in der Vorgangserfassung. Bei einem Systemabsturz kann die Vorgangserfassung mit den gesicherten Daten fortgesetzt werden. Wird die Vorgangserfassung abgebrochen, erscheint ein Hinweis, dass die gesicherten Daten bei einem Abbruch verloren gehen. Wenn Sie bestätigen wird die Vorgangserfassung abgebrochen und die gesicherten Daten werden gelöscht.

### Auftragserfassung – Anschriften
**Pfad:** `Verkauf > Auftragserfassung > Register Anschriften`

**Abb. D-32: Auftragserfassung - Anschriften**

In diesem Register bearbeiten Sie die Kunden- und Lieferanschrift. Die Kundenanschrift wird aus den Stammdaten des Kunden oder des Objekts herangezogen.

Sie können die Ermittlung der Lieferanschrift kundenspezifisch konfigurieren. Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

#### Kopfbereich
Die Felder im Kopfbereich sind zum Register **Auftragserfassung – Kopf-, Fußbereich** beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-83

#### Kundenanschrift
- **Name, Vorname**: Name und Vorname des Kunden.
  - **Technische Info**: alphanumerische Felder, DB-Felder: kauf.orgname, kauf.orgvorname
- **Anrede**: Nummer der Anrede. Wenn Sie eine Nummer auswählen, wird die Anrede im Klartext angezeigt.
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.organrede
- **Z. Hd.**: Zu Händen. Name der Person, an die die Lieferung ausgehändigt werden soll.
  - **Technische Info**: alphanumerisches Feld, DB-Feld: kauf.orgzhd
- **Zusatz**: Zusatztext der Anschrift.
  - **Technische Info**: alphanumerisches Feld, DB-Feld: kauf.orgbranche
- **Straße**: Straßenname und Hausnummer der Lieferanschrift.
  - **Technische Info**: alphanumerisches Feld, DB-Feld: kauf.orgstr
- **PLZ, Fach**: Postleitzahl und Nummer des Postfachs.
  - **Technische Info**: alphanumerische Felder, DB-Felder: kauf.orgpfplz, kauf.orgpostfach
- **PF Ort**: Ortsname des Postfachs.
  - **Technische Info**: alphanumerisches Feld, DB-Feld: kauf.orgpfort
- **PLZ, Ort**: Postleitzahl und Ortsname der Lieferanschrift.
  - **Technische Info**: alphanumerische Felder, DB-Felder: kauf.orgplz, kauf.orgort
- **KFZ Land**: Internationales Landeskennzeichen für Kraftfahrzeuge des Ziellandes. Wenn Sie ein Kennzeichen angeben, wird der Landesname im Klartext angezeigt.
  - **Technische Info**: alphanumerische Felder, DB-Felder: kauf.orgkfzcode, kauf.orgland
- **Tel**: Telefonnummer des Kunden.
  - **Technische Info**: alphanumerisches Feld, DB-Feld: kauf.orgtel
- **Fax**: Faxnummer des Kunden.
  - **Technische Info**: alphanumerisches Feld, DB-Feld: kauf.faxnr
- **E-Mail**: E-Mail-Adresse des Kunden.
  - **Technische Info**: alphanumerisches Feld, DB-Feld: kauf.orgemail
- **Sprache**: Nummer der Landessprache des Kunden, in der die Dokumente gedruckt werden. Wenn Sie eine Nummer auswählen, wird die Sprache im Klartext angezeigt.
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.sprkz
- **Kennz.**: Schlüsselnummer für den Steuertyp. Der Steuertyp ist in den Systemstammdaten hinterlegt. Wenn Sie eine Nummer auswählen, wird die Bezeichnung des Steuertyps im Klartext angezeigt.
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.kukz

#### Lieferanschrift
Sie können eine abweichende Lieferanschrift angeben, z. B. die Adresse einer Baustelle.
- Mit `<Strg>` + `<N>` legen Sie eine neue Lieferanschrift für den Kunden an.
  - ⇨ "Neue Lieferadresse" auf Seite D-138
- Mit `<Strg>` + `<L>` wählen Sie eine hinterlegte Lieferanschrift des Kunden aus.
  - ⇨ "Adressen Suche" auf Seite D-47

Die Felder sind zum Bereich **Kundenanschrift** beschrieben:
⇨ “Kundenanschrift" auf Seite D-90

Zusätzlich ist folgendes Feld beschrieben:
- **Region**: Versandregion. Die Versandregion ist in den Systemstammdaten hinterlegt und wird über die PLZ ermittelt.
  - **Technische Info**: Anzeigefeld

#### Fußbereich
Die Felder und Schaltflächen im Fußbereich sind zum Register **Auftragserfassung - Kopf-, Fußbereich** beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-83
Sie können die Felder im Fußbereich erst bearbeiten, wenn Sie die Positionserfassung abgeschlossen haben. Mit `<Ende>` wechseln Sie aus der Positionsebene in den Fußbereich.

### Auftragserfassung – Eigenschaften
**Pfad:** `Verkauf > Auftragserfassung > Register Eigenschaften`

**Abb. D-33: Auftragserfassung – Eigenschaften**

In diesem Register bearbeiten Sie die Angaben zur Mitarbeiterzuordnung, den Versandinformationen und den Rechnungs- und Druckoptionen.

#### Kopfbereich
Die Felder im Kopfbereich sind zum Register **Auftragserfassung – Kopf-, Fußbereich** beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-83

#### Mitarbeiterzuordnung
- **Bestellt von**: Mitarbeiternummer. Wenn Sie eine Nummer auswählen, wird der Name des Mitarbeiters im Klartext angezeigt. Mit `<F5>` öffnen Sie den Dialog **Ansprechpartner**, in dem Sie einen Ansprechpartner wählen oder neu anlegen können.
  - ⇨ "Ansprechpartner" auf Seite D-144
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.busr
- **Bestelldatum**: Datum des Auftragseingangs.
  - **Technische Info**: Datumsfeld, DB-Feld: kauf.bdat
- **Erfasser**: Mitarbeiternummer und Name des Sachbearbeiters, der den Vorgang erfasst hat. Die Felder werden vom System vorbelegt. Sie können nicht bearbeitet werden.
  - **Technische Info**: Anzeigefelder, DB-Feld: kauf.esuer
- **Abteilung**: Nummer der Abteilung, der der Erfasser zugeordnet ist. Die Felder werden vom System vorbelegt. Sie können nicht bearbeitet werden.
  - **Technische Info**: Anzeigefelder, DB-Feld: mitarb.abtnr
- **Sachbearbeiter**: Mitarbeiternummer und Name des Sachbearbeiters, der den Vorgang bearbeitet, aber nicht erfasst hat. Wenn Sie eine Nummer auswählen, wird der Name des Sachbearbeiters im Klartext angezeigt.
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.abvertr
- **Außendienst**: Name des Außendienst-Mitarbeiters.
  - **Technische Info**: alphanumerisches Feld, DB-Feld: kauf.vertr
- **Vertr. (Erlös)**: Vertreter-Erlös. Mitarbeiternummer des Vertreters, an den die Provision ausgezahlt wird. Wenn Sie eine Nummer auswählen, wird der Name des Vertreters im Klartext angezeigt.
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.vertrerloe

#### Versandinformationen
- **Max. Abladung**: Maximales Gewicht, das der Kunde mit seinem technischen Gerät abladen kann.
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.gmaxgew
- **Zustellung**: Vermerk über die gewünschte Art der Zustellung:
  - **Abholung**: Der Kunde holt die Ware selbst ab.
  - **Streckengeschäft**: Die Ware wird vom beauftragten Produktionsbetrieb direkt an den Endkunden ausgeliefert.
  - **keine Auswahl**: Die Ware wird über die Route ausgeliefert, die im Kopfbereich erfasst ist.
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.geschart
- **Direktauslief.**: Angabe, ob der Kunde direkt von den Produktionsstätten beliefert wird oder ob die Ware ins Handelshaus geliefert wird. Das Kennzeichen wird vom System vorbelegt.
  - J: Die Ware wird direkt an den Kunden geliefert.
  - N: Die Ware wird an das bestellende Handelshaus geliefert.
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.drkliefkz
- **Lieferart**: Nummer der Lieferart, z. B. frei Haus. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Lieferart im Klartext angezeigt.
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.lieferart
- **Versandart**: Nummer der Versandart, z. B. LKW. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Versandart im Klartext angezeigt.
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.versandart
- **Verpackungsart**: Nummer der Verpackungsart, z. B. Kiste. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Verpackart im Klartext angezeigt.
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.verpackart
- **Gest.-Beladung**: Gestell-Beladung. Sie wählen aus, nach welchen Kriterien die Ware auf den Gestellen sortiert wird:
  - Pos: nach Positionen.
  - Größe: nach Größe.
  - SZR+Gr: nach Scheibenzwischenraum und Größe.
  - Pos(frei): Positionen zusammengehalten aber frei organisiert.
  - HM Glas Farb Dick: nach Hardmaß, Glasmaß, Farbe und Dicke.
  - HM GI.maß Farbe: nach Hardmaß, Glasmaß und Farbe.
  - HM GI.maß - Dicke: nach Hardmaß, Glasmaß und Dicke.
  - HM - Farbe Dicke: nach Hardmaß, Farbe und Dicke.
  - HM Glasmaß nach Hardmaß und Glasmaß.
  - HM - Farbe: nach Hardmaß und Farbe.
  - HM - - Dicke: nach Hardmaß und Dicke.
  - HM---: nach Hardmaß.
  - Kommission: nach Kommissionstext.
  - Die Auswertung der ausgewählten Kriterien ist von der Systemkonfiguration abhängig.
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.gbelad
- **Ausgangszoll**: Nummer der Ausgangszollstelle für die Lieferpapiere. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Zollstelle im Klartext angezeigt.
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.azsnr
- **Bestimmungszoll**: Nummer der Zollstelle des Empfängerlandes. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Zollstelle im Klartext angezeigt.
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.bzsnr
- **Fahrtdauer/km**: Voraussichtliche Fahrzeit und Anzeige der Fahrstrecke. Die Fahrtdauer wirkt sich auf den Liefertermin aus. Die Fahrstrecke wird aus dem Feld **Entfernung** der Lieferadresse herangezogen.
  - **Technische Info**: numerische Felder, DB-Felder: kauf.anfahrt
- **Auslief. Route**: Auslieferungsroute bei Auslieferung oder Versand über ein zweites Haus. Das Feld ist nur freigeschaltet, wenn die interne Mandantentrennung aktiv ist.
  - **Technische Info**: numerische Felder, DB-Felder: kauf.endroutenr
- **Via Haus**: Anzeige der Mandantennummer des Hauses, über das die Ware geschickt wird bei Auslieferung oder Versand über ein zweites Haus. Das Haus wird automatisch angezeigt, wenn Sie eine Auslieferungsroute angeben.
  - **Technische Info**: Anzeigefeld, DB-Feld: kauf._vsvia

#### Rechnungs- und Druckoptionen
- **USt-Ident-Nr.**: Umsatzsteuer-Identifikationsnummer des Kunden.
  - **Technische Info**: alphanumerisches Feld, DB-Feld: kauf.steuernr
- **FA-Steuer-Nr.**: Finanzamt-Steuer-Nummer des Kunden.
  - **Technische Info**: alphanumerisches Feld, DB-Feld: kauf.finstnr
- **Kostenstelle**: Bezeichnung der Kostenstelle für statistische Auswertungen.
  - **Technische Info**: alphanumerisches Feld, DB-Feld: kauf.kostenst
- **Rechnungsart**: Art der Rechnung.
  - **Einzelrechnung**: Der Rechnungsempfänger bekommt für jeden Auftrag eine separate Rechnung zugestellt.
  - **Deckblattrechnung**: Der Rechnungsempfänger bekommt für jeden Auftrag eine separate Deckblattrechnung zugestellt.
  - **Sammelrechnung**: Der Rechnungsempfänger bekommt mehrere Aufträge zusammengefasst in einer Rechnung zugestellt. Sie können auswählen, in welchen Intervallen eine Sammelrechnung ausgestellt wird (wöchentlich, 14-tägig, monatlich).
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.rechungsart
- **Sammelrechnungslimit**: Maximaler Rechnungsbetrag, bis zu dem Sie eine Sammelrechnung erstellen können. Wenn das Limit überschritten ist, werden die Rechnungen als Einzelrechnungen erstellt.
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.srechlimit

> **Hinweis zur Sammelrechnungserstellung**
> Das Einverständnis des Rechnungsempfängers zur Sammelrechnung sowie die Festlegung des Sammelrechnungslimits ist in den Marktpartner-Stammdaten hinterlegt.

- **Teilfaktura**: Angabe, ob Teilabrechnungen nach einer Teillieferung erstellt werden:
  - J: Die Teilabrechnungen zulassen.
  - N: Keine Teilabrechnungen zulassen.
  - Wenn Sie als Rechnungsart Sammelrechnung wählen und Teilabrechnungen zulassen, werden nach jeder Teillieferung die ausgelieferten Artikel mit der nächsten Sammelrechnung fakturiert.
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.teilfakkz
- **Fakturasperre**: Die Rechnungsstellung kann für den Vorgang gesperrt werden. Bei aktiver Sperre erhält der Rechnungsempfänger vorläufig keine Rechnung für den Auftrag.
  - J: Die Rechnungsstellung sperren.
  - N: Die Rechnungsstellung zulassen.
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.fakturastop
- **Teillieferung**: Angabe, ob der Kunde Teillieferungen akzeptiert, oder diese nicht wünscht. Die Angabe dient nur zur Information. Auch wenn N ausgewählt ist, ist es möglich Teillieferscheine für den Auftrag zu erstellen.
  - J: Die Teillieferungen zulassen.
  - N: Keine Teillieferungen zulassen.
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.teilfakkz
- **Eilauftrag**: Der aktuelle Auftrag kann bevorzugt und mit höherer Priorität in die Produktion eingelastet werden.
  - J: Den Auftrag mit höherer Priorität einlasten.
  - N: Keine höhere Priorität für den Auftrag vergeben.
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.schnell
- **Bruttopreise drucken**: Die Bruttopreise können auf den marktpartnerseitigen Dokumenten ausgewiesen und gedruckt werden.
  - J: Die Bruttopreise ausweisen und drucken.
  - N: Keine Bruttopreise ausweisen und drucken.
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.preisdrkz
- **Kundenfaktor drucken**: Der kundenspezifische Faktor kann auf den marktpartnerseitigen Dokumenten ausgewiesen und gedruckt werden.
  - J: Den Kundenfaktor ausweisen und drucken.
  - N: Keinen Kundenfaktor ausweisen und drucken.
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.rabdrkz
  - **Beispiel**: Wenn der Kunde 10% Rabatt bekommt, dann beträgt der Wert für den Kundenfaktor = 0,9.
- **Bearbeitungspreise drucken**: Die Bearbeitungspreise für Bearbeitungen können separat ausgewiesen und gedruckt werden.
  - J: Die Preise für Bearbeitungen separat ausweisen und drucken.
  - N: Keine separaten Preise für Bearbeitungen ausweisen und drucken.
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.explbearbkz
- **Verglasung**: Die Kosten der Verglasung können auf der Rechnung unterschiedlich angezeigt werden.
  - **In Position einrechnen**: Die Kosten der Verglasung werden in die Position eingerechnet.
  - **Nur im Fuß ausweisen**: Die Kosten der Verglasung werden im Fuß der Rechnung ausgewiesen.
  - **In Position und Fuß**: Die Kosten der Verglasung werden in die Position eingerechnet und im Fuß der Rechnung ausgewiesen.
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.verglaskz
- **Artikeltexte drucken**: Die Artikeltexte können auf den marktpartnerseitigen Dokumenten gedruckt werden.
  - J: Die Artikeltexte drucken.
  - N: Keine Artikeltexte drucken.
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.atxtdrukz
- **Modelle drucken**: Die Modellskizze der Positionen kann im Anhang der marktpartnerseitigen Dokumente gedruckt werden.
  - J: Die Modellskizze drucken.
  - N: Keine Modellskizze drucken.
  - Die Einstellung von J oder N in diesem Feld wird, je nach konfigurierter Report-Variante, entweder repgo oder CrystalReport, ausgewertet.
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.moddrkz
- **Positionspreise unterdrücken**: Die Positionspreise werden standardmäßig auf den marktpartnerseitigen Dokumenten gedruckt. Sie können die Auflistung der Positionspreise unterdrücken, z. B. wenn mit dem Kunden ein Fixpreis für den gesamten Auftrag vereinbart wurde.
  - J: Keine Positionspreise drucken.
  - N: Die Positionspreise drucken.
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.posdrkz

#### Fußbereich
Die Felder und Schaltflächen im Fußbereich sind zum Register **Auftragserfassung – Kopf-, Fußbereich** beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-83
Die Felder können nur betreten werden, wenn mindestens eine Position erfasst ist. Mit `<Ende>` wechseln Sie aus der Positionsebene in den Fußbereich.

### Auftragserfassung – Verschiedenes
**Pfad:** `Verkauf > Auftragserfassung > Register Verschiedenes`

**Abb. D-34: Auftragserfassung - Verschiedenes**

In diesem Register werden Reklamationsinformationen, private Felder, weitere technische Informationen, Details der Auslieferung und die Zahlungsoptionen angezeigt. Sie können die Einträge bearbeiten.

#### Kopfbereich
Die Felder sind zum Register **Auftragserfassung – Kopf-, Fußbereich** beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-83

#### Reklamationsinformation
Mit diesen Daten können Sie eine Reklamationsstatistik führen. Die **Art**, der **Ort** und der **Typ** der Reklamation müssen in den Stammdaten angelegt sein.

- **Art**: Nummer der Reklamationsart. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Reklamationsart im Klartext angezeigt, z. B. Glasbruch.
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.reklamart
- **Ort**: Nummer des Reklamationsorts. Wenn Sie eine Nummer auswählen, wird die Bezeichnung des Reklamationsorts im Klartext angezeigt, z. B. Entladung.
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.reklamort
- **Typ**: Nummer des Reklamationstyps. Wenn Sie eine Nummer auswählen, wird die Bezeichnung des Reklamationstyps im Klartext angezeigt, z. B. falsche Farbe.
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.reklamspec
- **Datum**: Reklamationsdatum im Format TT.MM.JJJJ. Standardmäßig wird der aktuelle Tag angezeigt. Sie können das Reklamationsdatum bearbeiten.
  - **Technische Info**: Datumsfeld, DB-Feld: kauf.reklamdat

#### Zahlungsoptionen
- **Währung Kurs**: Nummer und Name der Währung und Währungskurs. Der Preis wird kundenbezogen in der angegebenen Währung berechnet. Wenn Sie eine Nummer auswählen, werden Währungsname und Währungskurs im Klartext angezeigt. Das Feld **Kurs** ist gesperrt, wenn die Eigenwährung gewählt ist.
  - **Technische Info**: Pflichtfeld, numerische Felder, DB-Felder: kauf.waehrung, kauf.kurs
- **Kalkulation in**: Das Feld ist nur freigeschaltet, wenn im Feld **Währung** nicht die Eigenwährung gewählt ist. Sie können festlegen, ob die Preise in der Eigenwährung oder in der Fremdwährung des Marktpartners berechnet werden:
  - **Eigenwährung**: Die Preise werden in der Eigenwährung von A+W Enterprise berechnet.
  - **Fremdwährung**: Die Preise werden in der Währung berechnet, die dem Marktpartner im Feld **Währung** zugewiesen ist.
  - **Technische Info**: Toggle-Feld, DB-Feld: kauf.waehrprs
- **Ausdruck in**: Nummer für den Ausdruck der marktpartnerspezifischen Unterlagen in der kalkulierten Währung oder der Fremdwährung. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Druckoption im Klartext angezeigt. Für den Druck muss der entsprechende Report hinterlegt sein.
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.waehrdru

> **Die Felder Kalkulation in und Ausdruck in**
> Die Felder Kalkulation in und Ausdruck in sind nur zugänglich, wenn das Währungs-Modul lizenziert ist.

- **Zahlziel**: Zahlungsziel in Tagen, das mit dem Marktpartner vereinbart wurde.
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.zahlziel
- **Valuta**: Frist zur Wertstellung in Tagen.
  - **Technische Info**: numerisches Feld, DB-Feld: kauf.valuta
  - **Beispiel**: Ist eine Rechnung am 15. des Monats fällig, würde der Eintrag von 2 Tagen bewirken, dass der Fälligkeitstermin in der Finanzbuchhaltung um zwei Tage erhöht wird, also zum 17. des Monats. Diese Tage werden z. B. für den Postweg einkalkuliert.

