---
description: "DE-HB-AWEnterprise_12"
---


# Softwarereferenz

---
## Suchfunktionen

### Erläuterung der Schaltflächen im Fußbereich

**[Details]** Öffnet einen Dialog mit den Details zur markierten Lieferadresse. Alternativ können Sie den Dialog mit <F5> öffnen. Die Schaltfläche ist nur freigeschaltet, wenn eine Adresse in der Trefferliste markiert ist.

**[Neue Suche]** Löscht alle Suchkriterien für eine neue Suche ab.

## Artikel-Suche

> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <F9>

In diesem Dialog suchen Sie nach Artikeln, die Sie für die Erfassung eines Auftrags benötigen. Sie können die Artikel-Suche über verschiedene Menüpfade aufrufen. Der Dialog ist immer gleich aufgebaut.

Die Treffer der Suche werden in den Registern angezeigt. Wenn Sie die Artikel-Suche öffnen, werden Ihnen alle Artikel in der Trefferliste angezeigt. Über die Filterkriterien können Sie die Trefferliste beschränken.

- Mit <F3> starten Sie die Suche.
- Mit <F2> wechseln Sie nach der Suche die Register in der Trefferliste.

Die Ergebnisse der Suche werden in der Trefferliste angezeigt. Die Trefferliste wird erst angezeigt, wenn Sie die Suche gestartet haben.

In diesem Dialog finden Sie folgendes Register:
- "Artikel-Suche – Kopf-, Fußbereich" auf Seite D-1102
- "Artikel-Suche - Bezeichnungen" auf Seite D-1105
- "Artikel-Suche - Artikelcodes" auf Seite D-1107
- "Artikel-Suche - Details" auf Seite D-1108

Die Ergebnisse der Suche werden in der Trefferliste angezeigt. Die Trefferliste wird erst angezeigt, wenn Sie die Suche gestartet haben.

### Artikel-Suche – Kopf-, Fußbereich

> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <F9>

*(Abb. D-18: Artikel-Suche – Kopf-, Fußbereich zeigt eine Benutzeroberfläche mit Suchkriterien im Kopfbereich und einer Trefferliste von Artikeln in einem Tabellenformat darunter. Die Suchfelder umfassen Ab Nummer, Artikelcode, Hauptbezeichnung, Interne Bezeichnung, Artikeltyp, Warengruppe und Lieferant. Die Trefferliste zeigt Spalten wie Nummer, Hauptbezeichnung, Internbez., Kurzbezeichnung und Status (Still).)*

In diesem Dialog suchen Sie Artikel anhand von verschiedenen Suchkriterien.
Wenn Sie die Artikel-Suche öffnen, werden Ihnen alle Artikel in der Trefferliste angezeigt. Über die Filterkriterien können Sie die Trefferliste beschränken.

#### Kopfbereich

Im Kopfbereich geben Sie die Suchkriterien an. Die Treffer der Suche werden in den Registern angezeigt.

Mit <F3> starten Sie die Suche.

**Ab Nummer** Startnummer, ab der aufsteigend nach Artikeln gesucht wird. Die Artikel, deren Nummer kleiner als die angegebene Artikelnummer ist, werden aus der Trefferliste ausgeschlossen.
*Technische Info: numerisches Feld, DB-Feld: artikel.artnr*

**Matchcode** Alphanumerischer Matchcode des Artikels. Die Artikel, deren Matchcode nicht die angegebenen Daten enthält, werden aus der Trefferliste ausgeschlossen.
*Technische Info: alphanumerisches Feld, DB-Feld: artikel.artmc*

**Artikelcode** Artikelcode aus den Stammdaten. Die Artikel, deren Artikelcode nicht die angegebenen Daten enthält, werden aus der Trefferliste ausgeschlossen.
*Technische Info: alphanumerisches Feld, DB-Feld: artikel.artikelcode*

**Kurzbezeichnung** Kurzbezeichnung des Artikels. Die Artikel, deren Kurzbezeichnung nicht die angegebenen Daten enthält, werden aus der Trefferliste ausgeschlossen.
*Technische Info: alphanumerisches Feld, DB-Feld: artikel.kurzbez*

**Hauptbezeichnung, Interne Bezeichnung, Intern2** Hauptbezeichnung und zusätzliche Bezeichnungen des Artikels. Die Artikel, deren Hauptbezeichnung oder interne Bezeichnung nicht die angegebenen Daten enthält, werden aus der Trefferliste ausgeschlossen.
*Technische Info: alphanumerische Felder, DB-Felder: artikel.artbez1, artikel.artbez2, artikel.artbez3*

**Artikeltyp, bis** Nummer und Bezeichnung des Artikeltyps. Im Feld **Artikeltyp** geben Sie die Nummer an, ab der nach Artikeln gesucht wird. Im Feld **bis** beschränken Sie die Suche bis zu Artikeln mit dem entsprechenden Artikeltyp. Die Artikel, deren Artikeltypnummer kleiner als die angegebene Nummer im Feld **Artikeltyp** oder größer als die Nummer im Feld **bis** sind, werden aus der Trefferliste ausgeschlossen.Wenn Sie eine Nummer angeben, wird die Bezeichnung des Artikeltyps im Klartext angezeigt. Mit <F9> können Sie nach einem Artikeltyp suchen.
*Technische Info: numerische Felder, Anzeigefelder, DB-Felder: artikel.atyp*

**A+W Bearbeit.typ, bis** Nummer und Bezeichnung des A+W spezifischen Bearbeitungstyps. Im Feld **A+W Bearbeitung.typ** geben Sie die Nummer an, ab der nach Artikeln gesucht wird. Im Feld **bis** beschränken Sie die Suche bis zu Artikeln mit dem entsprechenden Bearbeitungstyp. Wenn Sie eine Nummer angeben, wird die Bezeichnung des Bearbeitungstyps im Klartext angezeigt. Mit <F9> können Sie nach einem Bearbeitungstyp suchen.
*Technische Info: numerische Felder, Anzeigefelder, DB-Feld: artikel.awtyp*

**Warengruppe** Kennzeichen der Warengruppe, der der Artikel zugeordnet ist.
*Technische Info: alphanumerisches Feld, DB-Feld: artikel.wagrp*

**Materialgrp.** Kennzeichen der Materialgruppe, der der Artikel zugeordnet ist.
*Technische Info: alphanumerisches Feld, DB-Feld: artikel.artgrp*

**Lieferant** Nummer des Lieferanten, bei dem der Artikel bestellt wird. Mit <F9> > <F8> wählen Sie den Lieferanten aus der Lieferantenliste aus.
*Technische Info: numerisches Feld, DB-Feld: artikel.stdlinr*

**Art** Anzeige des Artikelstatus. In der Vorgangserfassung werden nur aktive Artikel angezeigt. Das Feld kann nicht bearbeitet werden.
*Technische Info: Anzeigefeld, DB-Feld: artikel.still*

#### Artikeldarstellung

In diesem Bereich wird der Scheibenaufbau des markierten Artikels aus der Trefferliste im Querschnitt angezeigt. Die Sonne markiert die Außenseite der Scheibe.

#### Erläuterung der Schaltflächen im Fußbereich

Mit den Schaltflächen im Fußbereich navigieren Sie in der Trefferliste, zeigen weitere Treffer an und aktualisieren die Trefferliste.

**[OK]** Storniert den aktuellen Auftrag.
**[Abbrechen]** Bricht den Stornovorgang ab.
**[[<] und [>]]** Mit diesen Schaltflächen wechseln Sie zum ersten oder letzten Eintrag in der Trefferliste.
**[[<<] und [>>]]** Mit diesen Schaltflächen zeigen Sie die vorherige oder nächste Seite der Trefferliste an.
**[Refresh]** Aktualisiert die Einträge in den Suchfeldern. Korrigierte oder zusätzliche Einträge in den Suchfeldern werden dadurch bei der Suche berücksichtigt. Die Schaltfläche ist nur im Bereich Suchfelder freigeschaltet.
**[Weitere Daten]** Zeigt in der Trefferliste weitere Einträge an, die den Suchkriterien entsprechen. Wenn keine weiteren Treffer mehr angezeigt werden können, ist die Schaltfläche gesperrt.
**[Neue Suche]** Löscht alle Suchkriterien für eine neue Suche. Alternativ können Sie die Suchkriterien mit <Strg> + <R> löschen und eine neue Suche starten.

### Artikel-Suche – Bezeichnungen

> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <F9> > Suchkriterien eingeben > <F3>

*(Abb. D-19: Artikel-Suche - Bezeichnungen zeigt das Suchergebnis im Tab "Bezeichnungen" mit Artikeln wie "A+W VSG, 2x2 mm".)*

In diesem Register werden die Bezeichnungen der Artikel angezeigt, die den Suchkriterien entsprechen.
Die Suchkriterien geben Sie im Kopfbereich an.

- Mit <F2> wechseln Sie die Register in der Trefferliste.
- Mit den Pfeiltasten und <Bild runter>, <Bild hoch> navigieren Sie in der Trefferliste.

#### Kopfbereich
Die Felder im Kopfbereich sind zum Dialog Artikel-Suche – Kopf-, Fußbereich beschrieben:
⇨ "Artikel-Suche - Kopf-, Fußbereich" auf Seite D-1102

#### Satzanzeige für die Artikelübersicht
Die Anzahl der Treffer in der Liste wird rechts, über den Registern, in einem Rahmen angezeigt.
Die Satzanzeige ist zum Dialog Marktpartnersuche beschrieben:
⇨ "Marktpartnersuche" auf Seite D-1091

#### Register Bezeichnungen
Die Spalten entsprechen den Feldern im Kopfbereich.
Zusätzlich werden folgende Spalten angezeigt:

- **Nummer:**
  Artikelnummer.
  *Technische Info: Anzeigefeld, DB-Feld: artikel.artnr*
- **Still:**
  Anzeige, ob der Artikel stillgelegt ist.
  - J: Artikel ist stillgelegt.
  - N: Artikel ist aktiv.
  In der Vorgangserfassung werden nur aktive Artikel angezeigt.
  *Technische Info: Anzeigefeld, DB-Feld: artikel.still*

#### Fußbereich
Die Felder im Fußbereich sind zum Dialog Artikel-Suche – Kopf-, Fußbereich beschrieben:
⇨ "Artikel-Suche - Kopf-, Fußbereich" auf Seite D-1102

### Artikel-Suche - Artikelcodes

> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <F9> > Suchkriterien eingeben > <F3> > Register Artikelcodes

*(Abb. D-20: Artikel-Suche - Artikelcodes zeigt das Suchergebnis im Tab "Artikelcodes". Es werden zusätzliche Spalten wie Matchcode, Artikelcode, Lieferant und Name angezeigt.)*

In diesem Register werden zusätzliche Informationen der Artikel angezeigt, die den Suchkriterien entsprechen.
Die Suchkriterien geben Sie im Kopfbereich an.

- Mit <F2> wechseln Sie die Register in der Trefferliste.
- Mit den Pfeiltasten und <Bild runter>, <Bild hoch> navigieren Sie in der Trefferliste.

#### Kopfbereich
Die Felder im Kopfbereich sind zum Dialog Artikel-Suche – Kopf-, Fußbereich beschrieben:
⇨ "Artikel-Suche - Kopf-, Fußbereich" auf Seite D-1102

#### Satzanzeige für die Artikelübersicht
Die Anzahl der Treffer in der Liste wird rechts, über den Registern, in einem Rahmen angezeigt.
Die Satzanzeige ist zum Dialog Marktpartnersuche beschrieben:
⇨ "Marktpartnersuche" auf Seite D-1091

#### Register Artikelcodes
Die Spalten sind zum Register Bezeichnungen beschrieben:
⇨ "Artikel-Suche - Kopf-, Fußbereich" auf Seite D-1102

Zusätzlich werden folgende Spalten angezeigt:

- **Bezeichnung:**
  Bezeichnung des Artikels.
  *Technische Info: Anzeigefeld, DB-Feld: artikel.artbez1*
- **Lieferant, Name:**
  Lieferantennummer und Name des Lieferanten.
  *Technische Info: Anzeigefeld, DB-Feld: artikel.stdlinr*

#### Fußbereich
Die Felder im Fußbereich sind zum Dialog Artikel-Suche – Kopf-, Fußbereich beschrieben:
⇨ "Artikel-Suche - Kopf-, Fußbereich" auf Seite D-1102

### Artikel-Suche - Details

> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <F9> > Suchkriterien eingeben > <F3> > Register Details

*(Abb. D-21: Artikel-Suche - Details zeigt das Suchergebnis im Tab "Details" mit Spalten wie Atyp, Bezeichnung, A+W Typ, Warengrp und Materialgrp.)*

In diesem Register werden die Details der Artikel angezeigt, die den Suchkriterien entsprechen.

Die Suchkriterien geben Sie im Kopfbereich an.
- Mit <F2> wechseln Sie die Register in der Trefferliste.
- Mit den Pfeiltasten und <Bild runter>, <Bild hoch> navigieren Sie in der Trefferliste.

#### Kopfbereich
Die Felder im Kopfbereich sind zum Dialog Artikel-Suche – Kopf-, Fußbereich beschrieben:
⇨ "Artikel-Suche - Kopf-, Fußbereich" auf Seite D-1102

#### Satzanzeige für die Artikelübersicht
Die Anzahl der Treffer in der Liste wird rechts, über den Registern, in einem Rahmen angezeigt.
Die Satzanzeige ist zum Dialog Marktpartnersuche beschrieben:
⇨ "Marktpartnersuche" auf Seite D-1091

#### Register Details
Die Spalten sind zum Register Bezeichnungen beschrieben:
⇨ "Artikel-Suche - Kopf-, Fußbereich" auf Seite D-1102

Zusätzlich werden folgende Spalten angezeigt:

- **Bezeichnung (Artikelnummer):**
  Bezeichnung des Artikels.
  *Technische Info: Anzeigefeld, DB-Feld: artikel.artbez1*
- **Atyp, Bezeichnung:**
  Nummer und Bezeichnung des Artikeltyps. Die Bezeichnung wird automatisch in der gewählten Systemsprache angezeigt.
  *Technische Info: Anzeigefeld, DB-Feld: artikel.atyp*
- **A+W Typ, Bezeichnung:**
  Nummer und Bezeichnung des A+W-Bearbeitungstyps. Die Bezeichnung wird automatisch in der gewählten Systemsprache angezeigt.
  *Technische Info: Anzeigefeld, DB-Feld: artikel.awtyp*

#### Fußbereich
Die Felder im Fußbereich sind zum Dialog Artikel-Suche – Kopf-, Fußbereich beschrieben:
⇨ "Artikel-Suche - Kopf-, Fußbereich" auf Seite D-1102

## Artikel-Suche nach Typen

> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld B.Art > <F5> > <F6> > [A-Suche]

*(Abb. D-22: Artikel-Suche nach Typen zeigt zwei Dialogfenster. Das linke ("Bearbeitungen") listet Bearbeitungstypen wie "Abkleben", "Bohrung". Das rechte ("Artikeltypen") listet Artikeltypen wie "FLOAT-Gläser". Ein drittes Fenster zeigt Artikel, die zum ausgewählten Typ gehören.)*

In diesem Dialog suchen Sie Artikel anhand der A+W Bearbeitungstypen oder der Artikeltypen. Alle Artikel des gewählten Typen werden in einem weiteren Auswahldialog angezeigt.

### Register Bearbeitungen
In diesem Register werden die Bearbeitungstypen zur Auswahl angezeigt, die in den normierten A+W Bearbeitungskatalog aufgenommen sind und Bearbeitungen in den Artikelstammdaten enthalten. Stillgelegte Bearbeitungstypen werden nicht angezeigt.

- **Nummer:**
  Nummer des A+W Bearbeitungstyps
- **A+W Bearbeitungstyp:**
  Bezeichnung des A+W Bearbeitungstyps

### Register Artikeltypen
In diesem Register werden die Artikeltypen zur Auswahl angezeigt, die Artikel in den Artikelstammdaten enthalten. Stillgelegte Artikeltypen werden nicht angezeigt.

- **Nummer:**
  Nummer des Artikeltyps
- **Artikeltypen:**
  Bezeichnung des Artikeltyps

### Auswahldialog
- **Artikel:**
  Artikel-, Bearbeitungsnummer
- **Bezeichnung:**
  Artikel-, Bearbeitungsbezeichnung
- **2. Bezeichnung:**
  Zusätzlicher Informationstext zur Bezeichnung, z. B. Kurzbezeichnung des Artikels oder Bearbeitungstyp.

## Produktsuche nach Elementen

> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <Shift> + <F8>

In diesem Dialog suchen Sie nach Produkten anhand der enthaltenen Komponenten. Sie können die Produktsuche über verschiedene Menüpfade aufrufen. Der Dialog ist immer gleich aufgebaut.

Die Treffer der Suche werden in den Registern angezeigt. Die Trefferliste wird erst angezeigt, wenn Sie die Suche gestartet haben.

- Mit <F3> starten Sie die Suche.
- Mit <F2> wechseln Sie nach der Suche die Register in der Trefferliste.

In diesem Dialog finden Sie folgende Register:
- "Produktsuche - Kopf-, Fußbereich" auf Seite D-1112
- "Produktsuche - Kundenartikel" auf Seite D-1114
- "Produktsuche – Bezeichnungen" auf Seite D-1116
- "Produktsuche - Technische Werte" auf Seite D-1117

### Produktsuche – Kopf-, Fußbereich

> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <Shift> + <F8>

*(Abb. D-23: Produktsuche nach Elementen – Kopf-, Fußbereich zeigt den leeren Suchdialog mit Feldern für Produkttyp (ISO, VSG, Gießharz), Glas1, SZR, Glas2 etc. im Kopfbereich.)*

In diesem Dialog suchen Sie nach Produkten anhand von Elementen aus ihrem Stücklistenaufbau.

#### Kopfbereich
Im Kopfbereich geben Sie die Suchkriterien an. Die Treffer der Suche werden in den Registern angezeigt.
Mit <F3> starten Sie die Suche.

**Produkttyp** Typ des Produkts:
- ISO
- VSG
- Gießharz
*Technische Info: Toggle-Feld, DB-Feld: artikel.artgrp*

**Glas1** Nummer des ersten Glasartikels. Dieses Feld ist ein Pflichtfeld. Wenn Sie das Feld ohne Angabe einer Nummer verlassen, wird eine Liste der Glasartikel zur Auswahl angezeigt.
*Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: artkuzu.kuartnr*

**Glas2** Nummer des zweiten Glasartikels. Dieses Feld ist optional.
*Technische Info: numerisches Feld, DB-Feld: artkuzu.kuartnr*

> **Position der Glasartikel in der Scheibe**
> Die Suchkriterien Glas1 und Glas2 berücksichtigen nicht die Einbauposition der Glasartikel in der Scheibe. Es wird nach allen Scheiben gesucht, die die angegebenen Gläser enthalten.
> In der Trefferliste werden die Gläser nach ihrer Einbauposition in der Scheibe von außen nach innen angezeigt. Glas1 ist das Glas auf der Außenseite der Scheibe.

**Folientyp** Nummer des Folientyps. Das Feld ist nur für den Produkttyp VSG freigeschaltet.
*Technische Info: numerisches Feld, DB-Felder: artikel.folientyp*

**SZR** Größe des Abstandhalters in Millimeter. Das Feld ist nur für den Produkttyp ISO freigeschaltet.
*Technische Info: numerisches Feld, DB-Feld: musskenn.gv11*

#### Erläuterung der Schaltflächen im Fußbereich

**[OK]** Storniert den aktuellen Auftrag.
**[Abbrechen]** Bricht den Stornovorgang ab.
**Ausgewähltes Produkt** Zurzeit nicht genutzt.
**Artikelbezeichnung 1** Zurzeit nicht genutzt.
**[Tech. Werte]** Zeigt die technischen Werte in den Spalten Ug-Wert, g-Wert, dB-Wert und Tv-Wert an. Die Schaltfläche ist nur kundenspezifisch freigeschaltet.
**[Suchen]** Startet die Suche. Die Schaltfläche ist nur im Kopfbereich freigeschaltet.
**[Auswahl]** Öffnet einen Auswahldialog zum aktuellen Feld. Die Schaltfläche ist nur freigeschaltet, wenn für das Feld Auswahloptionen hinterlegt sind.

### Produktsuche – Kundenartikel

> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <Shift> + <F8> > Suchkriterien eingeben > <F3>

*(Abb. D-24: Produktsuche nach Elementen - Kundenartikel zeigt die Trefferliste im Tab "Kundenartikel". Die Liste zeigt den Aufbau von ISO-Gläsern mit Spalten für Artikel, Bezeichnung, Glas1, Glas2, Glas3, SZR1, SZR2, Zwischenraum und Gas.)*

In diesem Register werden Informationen zum Aufbau der Artikel angezeigt, die den Suchkriterien entsprechen.
- Mit <F2> wechseln Sie die Register in der Trefferliste.
- Mit den Pfeiltasten und <Bild runter>, <Bild hoch> navigieren Sie in der Trefferliste.
Im Kopfbereich geben Sie die Suchkriterien an.

#### Kopf-, Fußbereich
Die Felder im Kopf- und Fußbereich sind zum Dialog Produktsuche nach Elementen - Kopf-, Fußbereich beschrieben:
⇨ "Produktsuche - Kopf-, Fußbereich" auf Seite D-1112

#### Register Kundenartikel
- **Sta:**
  Statusanzeige der Position.
  ⇨ "Symbolerklärung" auf Seite D-1128
  *Technische Info: Anzeigefeld*
- **Artikel:**
  Artikelnummer.
  *Technische Info: Anzeigefeld, DB-Feld: artikel.artnr*
- **Bezeichnung:**
  Artikelbezeichnung.
  *Technische Info: Anzeigefeld, DB-Feld: artikel.artbez1*
- **Glas1, Glas2, Glas3:**
  Nummern der Glasartikel. Die Anzahl der Gläser ist abhängig vom Artikel. Bei Artikeln mit mehr als drei Gläsern werden nur die ersten drei Gläser der Scheibe angezeigt.
  *Technische Info: Anzeigefelder*
- **SZR1, SZR2:**
  Größe des Abstandhalters im ersten und zweiten Scheibenzwischenraum in Millimeter. Die Anzahl der Abstandhalter ist abhängig von der Anzahl der Scheiben im ISO. Bei Artikeln mit mehr als zwei Abstandhaltern werden nur die ersten zwei Abstandhalter angezeigt.
  *Technische Info: Anzeigefelder*
- **Zwischenraum:**
  Nummer und Bezeichnung des Abstandhalters oder der Folie. Bei Artikeln mit mehr als einem Abstandhalter oder einer Folie, wird nur der erste Abstandhalter bzw. die erste Folie angezeigt.
  *Technische Info: Anzeigefeld*
- **Gas:**
  Nummer des Gases im Zwischenraum.
  *Technische Info: Anzeigefeld*

### Produktsuche – Bezeichnungen

> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <Shift> + <F8> > Suchkriterien eingeben > <F3> > Register Bezeichnungen

*(Abb. D-25: Produktsuche nach Elementen – Bezeichnungen zeigt die Trefferliste im Tab "Bezeichnungen" mit den Spalten Produkt, Bezeichnung, Hauptbezeichnung, Internbez., Kurzbezeichnung.)*

In diesem Register werden Informationen zu den Bezeichnungen der Artikel angezeigt, die den Suchkriterien entsprechen.
- Mit <F2> wechseln Sie die Register in der Trefferliste.
- Mit den Pfeiltasten und <Bild runter>, <Bild hoch> navigieren Sie in der Trefferliste.

#### Kopf-, Fußbereich
Die Felder im Kopf- und Fußbereich sind zum Dialog Produktsuche nach Elementen - Kopf-, Fußbereich beschrieben:
⇨ "Produktsuche - Kopf-, Fußbereich" auf Seite D-1112

#### Register Bezeichnungen
- **Produkt:**
  Artikelnummer.
  *Technische Info: Anzeigefeld, DB-Feld: artikel.artnr*
- **Bezeichnung:**
  Artikelbezeichnung.
  *Technische Info: Anzeigefeld, DB-Feld: artikel.artbez1*
- **Hauptbezeichnung:**
  Hauptbezeichnung des Artikels.
  *Technische Info: Anzeigefeld, DB-Feld: artikel.artbez2*
- **Internbez.:**
  Interne Artikelbezeichnung.
  *Technische Info: Anzeigefeld, DB-Feld: artikel.artbez3*
- **Kurzbezeichnung:**
  Kurzbezeichnung des Artikels.
  *Technische Info: Anzeigefeld, DB-Feld: artikel.kurzbez*

### Produktsuche – Technische Werte

> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein > Feld Artikel > <Shift> + <F8> > Suchkriterien eingeben > <F3> > Register Technische Werte

*(Abb. D-26: Produktsuche nach Elementen - Techn. Werte zeigt die Trefferliste im Tab "Techn. Werte" mit Spalten für technische Daten wie Glas1, Glas2, SZR 1&2, Gas, Ug-Wert, g-Wert, dB-Wert und Tv-Wert.)*

In diesem Register werden Informationen zu den technischen Werten der Artikel angezeigt, die den Suchkriterien entsprechen.
- Mit <F2> wechseln Sie die Register in der Trefferliste.
- Mit den Pfeiltasten und <Bild runter>, <Bild hoch> navigieren Sie in der Trefferliste.

#### Kopf-, Fußbereich
Die Felder im Kopf- und Fußbereich sind zum Dialog Produktsuche nach Elementen - Kopf-, Fußbereich beschrieben:
⇨ "Produktsuche - Kopf-, Fußbereich" auf Seite D-1112

#### Register Techn. Werte
Die Spalten sind teilweise zu den Dialogen Produktsuche nach Elementen - Kundenartikel und Produktsuche nach Elementen – Bezeichnungen beschrieben:
⇨ "Produktsuche - Kundenartikel" auf Seite D-1114
⇨ "Produktsuche - Bezeichnungen" auf Seite D-1116

Zusätzlich werden folgende Spalten angezeigt:
- **Gas 1, Gas 2:**
  Nummern der Gase in den Zwischenräumen.
  *Technische Info: Anzeigefelder*
- **Ug-Wert:**
  Wärmedurchgangskoeffizient.
  *Technische Info: Anzeigefeld*
- **g-Wert:**
  Energiedurchlasskoeffizient (Gesamtdurchlassgrad).
  *Technische Info: Anzeigefeld*
- **dB-Wert:**
  Schalldämmungs-Wert der Position in Dezibel.
  *Technische Info: Anzeigefeld*
- **Tv-Wert:**
  Lichtdurchlässigkeit (Lichttransmissionsgrad).
  *Technische Info: Anzeigefeld*

## Objekt-Suche

> Verkauf > Auftragserfassung > Feld Objekt > <F9>

In diesem Dialog suchen Sie nach Objekten.
Wenn Sie im Feld Objekt die Suche öffnen, werden Ihnen alle Objekte des Marktpartners in der Trefferliste angezeigt. Über die Filterkriterien können Sie die Trefferliste beschränken.

> **Objekt vor Marktpartner wählen**
> Sie können mit <Strg> +<F11> im Feld Kunde nach Objekten suchen, bevor Sie den Marktpartner wählen. Im Dialog Objekt-Suche werden dann alle Objekte angezeigt. Wenn Sie ein Objekt wählen, werden in einem weiteren Dialog nur noch die Kunden angezeigt, denen das das aktuelle Objekt zugeordnet ist. Wenn das Objekt nur einem Marktpartner zugeordnet ist, wird dieser automatisch herangezogen.

Wenn Sie ein Objekt wählen, werden je nach Systemkonfiguration einige Daten des gewählten Marktpartners oder Kreditors ggf. überschrieben, z. B. Lieferadresse, Kostenstelle, Rabatte.
Die Ergebnisse der Suche werden in der Trefferliste angezeigt.

In diesem Dialog finden Sie folgende Register:
- "Objekt-Suche - Kopf-, Fußbereich" auf Seite D-1119
- "Objekt-Suche - Adresse" auf Seite D-1121
- "Objekt-Suche - Identifikation" auf Seite D-1122

### Objekt-Suche – Kopf-, Fußbereich

> Verkauf > Auftragserfassung > Feld Objekt > <F9>

*(Abb. D-27: Objekt-Suche – Kopf zeigt den Kopfbereich der Objektsuche mit Feldern wie Ab Objekt, Objekt-Kürzel, Bezeichnung, Externe Nummer, etc.)*

In diesem Dialog suchen Sie nach Objekten anhand von verschiedenen Suchkriterien. Es werden nur die Objekte angezeigt, die dem Marktpartner zugeordnet sind, der im Feld Kunde in der Auftragserfassung ausgewählt wurde. Über die Filterkriterien können Sie die Trefferliste beschränken.

#### Suchfelder
Im Kopfbereich geben Sie die Suchkriterien an. Die Treffer der Suche werden in den Registern angezeigt. Je nach Systemkonfiguration werden nicht alle der folgenden Felder angezeigt.

- **Ab Objekt** Startnummer, ab der aufsteigend nach Objekten gesucht wird.
  *Technische Info: numerisches Feld, DB-Feld: objekte.objnr*
- **Objekt-Kürzel** Zweibuchstabiges Kürzel des Objekts aus den Stammdaten, das auf dem Scheibenetikett ausgewiesen werden kann.
  *Technische Info: alphanumerisches Feld, DB-Feld: objekte.etitxt2*
- **Bezeichnung** Objektbezeichnung.
  *Technische Info: alphanumerisches Feld, DB-Feld: objekte.bez*
- **Externe Nummer** Objektnummer, die vom Kunden vorgegeben wird.
  *Technische Info: alphanumerisches Feld, DB-Feld: objekte.exobjnr*
- **Etikettext** Text zum Objekt, der auf dem Scheibenetikett ausgewiesen wird.
  *Technische Info: alphanumerisches Feld, DB-Feld: objekte.etitxt1*
- **Alle** Angabe, ob für das Objekt Verglasungsarbeiten vorgesehen sind:
  - J: Für das Objekt sind Verglasungsarbeiten geplant.
  - N: Für das Objekt sind keine Verglasungsarbeiten geplant.
  *Technische Info: Toggle-Feld, DB-Feld: objekte.vergl*
- **Vertreter** Mitarbeiternummer, dem das Objekt zugeordnet ist. Der Vertreter wird z. B. in die Provisionsberechnung einbezogen. Wenn Sie eine Nummer angeben, wird der Name des Mitarbeiters im Klartext angezeigt.
  *Technische Info: numerisches Feld, DB-Feld: objekte.vertreter*
- **Route** Routennummer, die dem Objekt zugeordnet ist. Wenn Sie eine Nummer angeben, wird die Bezeichnung der Route im Klartext angezeigt.
  *Technische Info: numerisches Feld, DB-Feld: objekte.routenr*
- **Verglasungsmitarbeiter** Mitarbeiternummer für die Verglasungsarbeiten. Wenn Sie eine Nummer angeben, wird der Name des Mitarbeiters im Klartext angezeigt.
  *Technische Info: numerisches Feld, DB-Feld: objekte.verglmanr*
- **Kostenstelle** Kurzbezeichnung der Kostenstelle für das Objekt. Wenn Sie eine Kurzbezeichnung angeben, wird der Name der Kostenstelle im Klartext angezeigt.
  *Technische Info: alphanumerisches Feld, DB-Feld: objekte.kostenst*

#### Erläuterung der Schaltflächen im Fußbereich
**[Neue Suche]** Löscht alle Suchkriterien für eine neue Suche.

### Objekt-Suche – Adresse

> Verkauf > Auftragserfassung > Feld Objekt > <F9> > Register Adresse

*(Abb. D-28: Objekt-Suche – Adresse zeigt die Trefferliste im Adress-Tab mit Spalten wie Kürzel, Vertreter, Name, Routennr., Route.)*

In diesem Register werden die adressbezogenen Daten der Objekte angezeigt, die den Suchkriterien entsprechen.
Die Suchkriterien geben Sie im Kopfbereich an.

- Mit <Shift> + <F2> wechseln Sie die Register in der Trefferliste.
- Mit den Pfeiltasten und <Bild runter>, <Bild hoch> navigieren Sie in der Trefferliste.
- Mit <Strg> + <R> löschen Sie die eingegebenen Suchkriterien.

#### Suchfelder
Die Felder im Kopfbereich sind zum Dialog Objekt-Suche – Kopf-, Fußbereich beschrieben:
⇨ "Objekt-Suche – Kopf-, Fußbereich" auf Seite D-1119

#### Register Adresse
Die Spalten in der Trefferliste entsprechen den Feldern im Kopfbereich. Zusätzlich werden folgende Spalten angezeigt:

- **Kürzel:**
  Die Spalte entspricht dem Feld Objekt-Kürzel aus dem Kopfbereich.
  ⇨ "Objekt-Kürzel" auf Seite D-1119
  *Technische Info: Anzeigefeld, DB-Feld: objekte.etitxt2*
- **Vertreter, Name:**
  Die Spalten entsprechen dem Feld Vertreter im Kopfbereich. Der Name des Vertreters wird aus den Mitarbeiterstammdaten herangezogen.
  ⇨ "Vertreter" auf Seite D-1120
  *Technische Info: Anzeigefelder, DB-Feld: objekte.vertreter*
- **Routenr., Route:**
  Die Spalten entsprechen dem Feld Route im Kopfbereich. Die Routenbezeichnung wird aus dem Routenstamm herangezogen.
  ⇨"Route" auf Seite D-1120
  *Technische Info: Anzeigefelder, DB-Feld: objekte.routenr*

#### Erläuterung der Schaltflächen im Fußbereich
**[Neue Suche]** Löscht alle Suchkriterien für eine neue Suche.

### Objekt-Suche – Identifikation

> Verkauf > Auftragserfassung > Feld Objekt > <F9> > Register Identifikation

*(Abb. D-29: Objekt-Suche – Identifikation zeigt die Trefferliste im Identifikations-Tab mit Spalten wie Etikettentexte, Kostenst. Bezeichnung, Vergl. und VergIMA Name.)*

In diesem Register werden die Identifikationsmerkmale der Objekte angezeigt, die den Suchkriterien entsprechen.
Die Suchkriterien geben Sie im Kopfbereich an.

- Mit <Shift> + <F2> wechseln Sie die Register in der Trefferliste.
- Mit den Pfeiltasten und <Bild runter>, <Bild hoch> navigieren Sie in der Trefferliste.
- Mit <Strg> + <R> löschen Sie die eingegebenen Suchkriterien.

#### Suchfelder
Die Felder im Kopfbereich sind zum Dialog Objekt-Suche – Kopf-, Fußbereich beschrieben:
⇨ "Objekt-Suche - Kopf-, Fußbereich" auf Seite D-1119

#### Identifikation
Die Spalten in der Trefferliste entsprechen den Feldern im Kopfbereich. Zusätzlich werden folgende Spalten angezeigt:
- **Kostenst., Bezeichnung:**
  Kurzbezeichnung und Bezeichnung der Kostenstelle, die dem Objekt zugeordnet ist. Der Name der Kostenstelle wird aus den Stammdaten herangezogen.
  *Technische Info: Anzeigefelder, DB-Feld: objekte.kostenst*
- **Vergl.:**
  Angabe, ob für das Objekt Verglasungsarbeiten vorgesehen sind:
  - J: Für das Objekt sind Verglasungsarbeiten geplant.
  - N: Für das Objekt sind keine Verglasungsarbeiten geplant.
  *Technische Info: Anzeigefeld, DB-Feld: objekte.vergl*
- **VergIMA, Name:**
  Mitarbeiternummer und Name des Mitarbeiters für die Verglasungsarbeiten. Der Name des Mitarbeiters wird aus den Stammdaten herangezogen.
  *Technische Info: Anzeigefelder, DB-Feld: objekte.verglmanr*

## Werteingabe – Erweiterte Suche

> Verkauf > Auftragserfassung > Feld Auftrag > <Shift> + <F5> oder <Strg> + <E>

In diesen Dialogen können Sie anhand eines bestimmten Kriteriums nach Aufträgen suchen. Der Dialog wird für jedes Kriterium über eine andere Tastenkombination aufgerufen. Der Suchdialog Werteingabe ist für alle Kriterien analog aufgebaut, unterscheidet sich jedoch je nach Kriterium in der Bezeichnung des Suchfeldes.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Werteingabe – Suche nach Kommission" auf Seite D-1124
- "Werteingabe – Suche nach Originalnummer" auf Seite D-1125

### Werteingabe – Suche nach Kommission

> Verkauf > Auftragserfassung > Feld Auftrag > <Shift> + <F5>

*(Abb. D-30: Suche nach Kommission zeigt einen Dialog zur Eingabe eines Kommissionstextes und eine Ergebnisliste von Aufträgen, die diesem Text entsprechen.)*

In diesem Dialog suchen Sie Aufträge anhand des Kommissionstextes.

#### Werteingabe
**Kommision** Kommissionstext oder Teil des Kommissionstextes. Mit einem Stern `*` vor dem Suchwort weiten Sie die Suche auf alle Aufträge aus, in denen der Kommissionstext enthalten ist.

#### Auswahldialog
In diesem Dialog werden alle Aufträge mit dem angegebenen Kommissionstext angezeigt.
Mit den Pfeiltasten und <Bild runter>, <Bild hoch> navigieren Sie in dem Auswahldialog.
- **Kommision:**
  Kommissionstext der Position.
- **Kunde:**
  Kundenname.
- **Auftrag:**
  Auftragsnummer.

Mit <Enter> wird die Auftragsnummer des markierten Eintrags in die Auftragserfassung übernommen.

### Werteingabe – Suche nach Originalnummer

> Verkauf > Auftragserfassung > Feld Auftrag > <Strg> + <E>

*(Abb. D-31: Suche nach Originalnummer zeigt einen Dialog zur Suche nach einer Original-Auftragsnummer. Nach der Suche wird eine Liste von Folgeaufträgen angezeigt, die sich auf den Originalauftrag beziehen.)*

In diesem Dialog suchen Sie Aufträge, die mit Bezug zu einem Original-Auftrag erfasst wurden. Sie können die Aufträge anhand der Original-Auftragsnummer suchen, auf die sie sich beziehen.

#### Werteingabe
**Originalnummer** Originalnummer des Auftrags, die als Bezug bei der Vorgangserfassung angegeben wurde. Mit <F9> können Sie nach einer Nummer suchen.

#### Suchdialog
Im Feld **Originalnummer** im Dialog **Werteingabe** öffnen Sie mit <F9> die Selo-Suche nach Original-Aufträgen.

**Suche** Original-Auftragsnummer, ab der nach Vorgängen gesucht wird. Wenn Sie keine Nummer eingeben, werden in der Trefferliste alle verfügbaren Original-Aufträgen angezeigt.
Mit den Pfeiltasten und <Bild runter>, <Bild hoch> navigieren Sie in der Trefferliste.
- **Original-Auftragsnummer:**
  Auftragsnummer des originalen Auftrags.
- **Haus:**
  Mandantennummer (Hausnummer).
- **Nummer:**
  Auftragsnummer des neuen Auftrags.
- **Subnr:**
  Subnummer des neuen Auftrags.
- **Kunde:**
  Kundenname des neuen Auftrags.

Wenn Sie eine Originalnummer mit <Enter> wählen, öffnet sich ein Auswahldialog, in dem alle Aufträge angezeigt werden, die sich auf diese Original-Auftragsnummer beziehen.

#### Auswahldialog
In diesem Dialog werden alle Aufträge mit Bezug auf den Auftrag mit der angegebenen Original-Auftragsnummer angezeigt.
Mit den Pfeiltasten und <Bild runter>, <Bild hoch> navigieren Sie in dem Auswahldialog.
- **Auftrag:**
  Auftragsnummer.
- **Original-Auftrag:**
  Auftragsnummer des originalen Auftrags.
- **Kunde:**
  Kundenname.

Mit <Enter> wird der markierte Auftrag in der Auftragserfassung geöffnet.

# Vorgangsverwaltung

In der Vorgangsverwaltung werden alle Dialoge und Funktionen beschrieben, mit der Sie Vorgänge bearbeiten können. In diesem Part erfassen und bearbeiten Sie die Vorgänge für den Verkauf, z. B. Angebote und Aufträge.

In diesem Abschnitt sind folgende Dialoge erklärt:
- "Symbolerklärung" auf Seite D-1128
- "Schnellerfassung" auf Seite D-1131
- "Angebotserfassung" auf Seite D-1132
- "Preislose Erfassung" auf Seite D-1133
- "Auftragserfassung" auf Seite D-1134
- "Auftragspositionen" auf Seite D-1167
- "Hauswechsel" auf Seite D-1192
- "Neue Lieferadresse" auf Seite D-1192
- "Endkundenanschrift" auf Seite D-1195
- "Marktpartner-Info" auf Seite D-1197
- "Ansprechpartner" auf Seite D-1199
- "Storno" auf Seite D-1200
- "Mitarbeiterzuordnung - Spezial" auf Seite D-1201
- "Konfigurierbare Felder" auf Seite D-1201
- "Übersicht" auf Seite D-1202
- "Produktsets (Sash Master)" auf Seite D-1203
- "Artikel-Maßangaben" auf Seite D-1205
- "Bestandsprognose" auf Seite D-1206
- "Produktaustausch" auf Seite D-1209
- "Reklamation" auf Seite D-1214
- "Auftragsarten" auf Seite D-1215
- "Artikelangaben für bemaßte Varianten" auf Seite D-1217
- "Varianten- und Farben-/Dickenauswahl" auf Seite D-1220
- "Private Felder" auf Seite D-1221
- "Fremddaten-Import" auf Seite D-1222
- "Dokumentenarten" auf Seite D-1224
- "Dokumentenartenzuordnung" auf Seite D-1225
- "Dateizuordnung" auf Seite D-1228
- "DXF Import" auf Seite D-1229
- "Änderungs-Protokoll" auf Seite D-1230
- "Lieferterminänderungs-Protokoll" auf Seite D-1232
- "Modellkatalog" auf Seite D-1233
- "Modell-Maßangaben" auf Seite D-1234
- "Zahlungsverwaltung" auf Seite D-1236
- "Zahlungsplan" auf Seite D-1238
- "Fehlerinformationssystem" auf Seite D-1240
- "Produktionsmonitor" auf Seite D-1242

## Symbolerklärung
In diesem Abschnitt werden die Kennzeichen für den Dialogmodus, den Positionsstatus und das Positionskennzeichen beschrieben.

### Dialogmodus
Der Dialogmodus wird in der Titelzeile des Dialogs angezeigt.

| Symbol | Symbolbeschreibung | Bedeutung |
| --- | --- | --- |
| Dialog mit Kreuzchen (+) | In diesem Modus können Sie neue Datensätze anlegen. |
| Dialog mit Stift | In diesem Modus können Sie einen Datensatz bearbeiten. |
| Gelbes Dreieck mit Ausrufezeichen | In diesem Modus können Sie den Datensatz nicht bearbeiten, z. B., weil er bereits an die Produktion übergeben wurde. |
| Suche | In diesem Modus können Sie nach Datensätzen suchen. |

*(Tab. D-1 Dialogmodus)*

### Positionsstatus und Positionskennzeichen
Der Positionsstatus wird im Register Positionen vor dem Feld Pos angezeigt.

| Symbol | Symbolbeschreibung | Bedeutung |
| --- | --- | --- |
| grün | Die Position kann frei bearbeitet werden, da die Produktion noch nicht begonnen hat. |
| gelb | Die Position oder Unterteile der Position sind bestellt und die Bestellung ist gedruckt worden. |
| rot | Die Position ist in der Produktion verplant. Sie kann nicht mehr bearbeitet werden. |
| drei Viertel rot, ein Viertel blau | Die Position ist teilweise geliefert. |
| halb rot, halb blau | Die Position ist komplett geliefert. |
| zwei Viertel rot, zwei Viertel blau | Die Position ist teilfakturiert. |
| blau | Die Position ist komplett fakturiert. |
| Kreuz rot | Die Position wird gelöscht. |

*(Tab. D-2 Positionsstatus)*

Das Positionskennzeichen wird vor dem Feld Pos angezeigt.

| Symbol | Symbolbeschreibung | Bedeutung |
| --- | --- | --- |
| Gelber Stern | Das Produkt ist für die Fixierung vermerkt. D. h., die Produktbemaßung sowie weitere zusätzliche Information kann für dieses Produkt beim Auftragsspeichern hinterlegt werden: ⇨ "Artikelangaben für bemaßte Varianten" auf Seite D-1217 |
| Grüner Stern (*) | Das erfasste Produkt wurde bereits fixiert Beim Bedarf können Sie nach einer Änderung (z. B. Stücklisteaufbau) das Produkt überfixieren. Wenn das Produkt für den jeweiligen Kunden bestimmt war, kann dieses für andere Kunden nicht erfasst werden. "Artikelangaben für bemaßte Varianten" auf Seite D-1217 |
| Modell | Die Position ist mit Modell erfasst. ⇨ "Modell-Maßangaben" auf Seite D-1234 |
| Fenster mit Sprossen | Die Position ist mit Sprossen erfasst. ⇨ "Sprossenerfassung" auf Seite D-1284 |
| Modell mit Sprossen | Die Position ist mit Modell und Sprossen erfasst. ⇨ "Modell-Maßangaben" auf Seite D-1234 ⇨ "Sprossenerfassung" auf Seite D-1284 |

*(Tab. D-3 Positionskennzeichen)*

## Positionsstatus und Vorgangsstatus in Textform
Der Status des Vorgangs und der erfassten Positionen kann zusätzlich in Textform angezeigt werden.

*(Abb. D-32: Statusanzeigen in Textform zeigt eine Auftragserfassungsmaske, in der der Vorgangsstatus (z.B. "GLOBALE - Lokal - Korrektur") in der Titelzeile und der Positionsstatus (z.B. "Produktion") in einer Spalte der Positionsliste angezeigt wird.)*

Wenn sich der Vorgangsstatus ändert, wird der aktuelle Status in der Titelzeile des Dialogs angezeigt, z. B. (Teil-) produziert, GLOBALKORREKTUR, VERSANDPLANUNG LIEGT VOR.

Wenn sich der Positionsstatus ändert, wird der Status der entsprechenden Position im rechten Teil des Dialogs auf Positionsebene angezeigt, z. B. Verpackt, FIXIERT, Lokal-Korrektur. Jede Position kann einen anderen Status haben. Der angezeigte Positionsstatus gilt jeweils für die markierte Position.

Für weitere Informationen zu den unterschiedlichen Statusanzeigen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

## Schnellerfassung
> Verkauf > Schnellerfassung

*(Abb. D-33: Schnellerfassung - Kopfdaten zeigt eine vereinfachte Erfassungsmaske für Aufträge mit Feldern für Kunde, Vorgang, Versandinformationen und Lieferanschrift.)*

In diesem Dialog erfassen Sie schnell einen Auftrag oder ein Angebot. Diese vereinfachte Form der Vorgangserfassung bietet nur einen eingeschränkten Zugriff auf die Funktionsmöglichkeiten und die Auswahl an Artikeln, Modellen und den Stücklistenaufbau.

Die Schnellerfassung ist auf einem Kundenwunsch bereitgestellt worden. Da jedoch der Umfang der Erfassung beschränkt ist, findet diese Erfassung keine breitere Anwendung. Für weitere Informationen zu diesem Modul kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

## Angebotserfassung
> Verkauf > Angebotserfassung

*(Abb. D-34: Angebotserfassung zeigt eine detaillierte Maske zur Erfassung von Angeboten, die der Auftragserfassungsmaske sehr ähnlich ist, mit Kopf-, Positions- und Fußbereich.)*

In diesem Dialog erfassen und bearbeiten Sie Angebote. Mit <Enter> wird die Angebotsnummer vom System vergeben. Um ein erfasstes Angebot zu öffnen, geben Sie im Feld Angebot die Angebotsnummer ein oder wechseln mit <F9> in den Suchdialog.

Wenn Sie bei Angeboten einen Liefertermin eintragen, können Sie je nach Systemkonfiguration einen Wiedervorlage-Termin anlegen, um das Angebot nachzuverfolgen. Wenn der Wiedervorlage-Termin erreicht ist, wird beim Programmstart eine Meldung angezeigt oder eine Erinnerungs-Mail zugestellt.
⇨ "Wiedervorlage" auf Seite D-1463

Sie können aus jedem Angebot einen Auftrag erstellen, indem Sie in der Auftragserfassung einen Bezug zu dem Angebot herstellten. Wenn Sie in der Auftragserfassung die Angebotsnummer in das Feld Bezug eintragen, dann werden die Daten aus dem Angebot in den Auftrag übernommen.

Der Dialog **Angebotserfassung** ist wie der Dialog **Auftragserfassung** aufgebaut. Abweichungen werden zum Dialog **Auftragserfassung** beschrieben:
⇨ "Auftragserfassung" auf Seite D-1134

## Preislose Erfassung
> Verkauf > Preislose Erfassung

*(Abb. D-35: Preislose Erfassung zeigt eine Erfassungsmaske, die der Auftragserfassung gleicht, jedoch ohne sichtbare Preisberechnungen für den Benutzer.)*

In diesem Dialog erfassen Sie Kundenaufträge ohne Preise. Bei Ladenaufträgen verhindern Sie auf diese Weise, dass Kunden die Einkaufspreise einsehen können. Zusätzlich können auch Mitarbeiter, die die Betriebspreise nicht einsehen können, Aufträge erfassen. Diese Aufträge werden nachträglich von einem Sachbearbeiter geprüft.

Die Preisberechnung des Auftrags erfolgt verdeckt, wenn Sie den Auftrag speichern. Der Vorgang wird unter der vom System vergebenen Auftragsnummer gespeichert.

Der Dialog **Preislose Erfassung** ist wie der Dialog **Auftragserfassung** aufgebaut:
⇨ "Auftragserfassung" auf Seite D-1134

## Auftragserfassung
> Verkauf > Auftragserfassung

In diesem Dialog erfassen und bearbeiten Sie Aufträge. Der Dialog Auftragserfassung ist in drei Teile gegliedert:

- **Kopfbereich:**
  In diesem Bereich werden die Kundendaten und Lieferbedingungen angezeigt.
- **Positionsebene:**
  In diesem Bereich werden Informationen zu den Auftragspositionen angezeigt.
- **Fußbereich:**
  In diesem Bereich werden Informationen zu den Auftragssummen, den Rabatten und Zuschlägen angezeigt.

In diesem Dialog finden Sie folgende Register:
- "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-1135
- "Auftragserfassung – Anschriften" auf Seite D-1143
- "Auftragserfassung - Eigenschaften" auf Seite D-1146
- "Auftragserfassung - Verschiedenes" auf Seite D-1152
- "Auftragserfassung – Summen" auf Seite D-1157
- "Auftragserfassung - Detailansicht Rabatte" auf Seite D-1162

Im Bereich Positionen finden Sie folgende Register:
- "Auftragspositionen - Allgemein" auf Seite D-1167
- "Auftragspositionen - Eigensch." auf Seite D-1180
- "Auftragspositionen – Preise" auf Seite D-1185
- "Auftragspositionen – Status" auf Seite D-1188
- "Auftragspositionen – Kosten" auf Seite D-1190

### Auftragserfassung – Kopf-, Fußbereich
> Verkauf > Auftragserfassung

*(Abb. D-36: Auftragserfassung – Positionen zeigt die Hauptansicht der Auftragserfassung mit Kopfdaten (Auftrag, Kunde, Termin), einer Liste von Positionen und dem Fußbereich mit den Gesamtsummen.)*

In diesem Dialog erfassen Sie die Kopfdaten des Auftrags, z. B.die Kundendaten und Lieferbedingungen. Im Fußbereich werden Informationen zu den Auftragssummen angezeigt.

- Mit <Enter> wechseln Sie in das nächste Feld im Kopfbereich. Im letzten Feld des Kopfbereichs, dem Feld Objekt, wechseln Sie mit <Enter> in das Register Positionen.
- Aus den Feldern Eingang, Rechnungstyp oder Objekt können Sie mit <F2> in die Positionsebene zu den Register Anschriften, Eigenschaften und Verschiedenes wechseln.
  - ⇨ "Auftragserfassung - Anschriften" auf Seite D-1143
  - ⇨ "Auftragserfassung - Eigenschaften" auf Seite D-1146
  - ⇨ "Auftragserfassung - Verschiedenes" auf Seite D-1152
- Mit <Ende> wechseln Sie aus der Positionsebene im Register Allgemein in den Fußbereich und schließen die Auftragserfassung ab.

#### Kopfbereich
**Auftrag** Auftragsnummer. Die Nummer wird vom System aus dem zugeordneten Nummernkreis vergeben. Wenn Sie eine bereits vergebene Nummer eintragen, wird der entsprechende Auftrag geöffnet. Je nach Status können Sie den Auftrag bearbeiten. Der Feldname variiert je nach Dialog, in dem Sie den Vorgang erfassen, z. B. Angebot in der Angebotserfassung.
Wenn Sie die Vorgangsnummer eingeben, wird bei einigen Vorgangsarten ein weiteres Feld angezeigt, z. B. bei Rechnung oder Lieferschein. In diesem Feld wird die Subnummer zum Vorgang angezeigt. Sie können eine bereits vergebene Subnummer wählen oder die nächste freie Nummer vom System vergeben lassen.
*Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kauf.auftrnr*

> **Automatische Vergabe von Vorgangsnummern**
> Wenn Sie einen neuen Vorgang erfassen, wird die Vorgangsnummer automatisch vom System vergeben. Bei Rechnungen wird zunächst eine interne, temporäre Nummer vergeben. Auf diese Weise wird vom System sicher gestellt, dass Rechnungen fortlaufend durchnummeriert sind.

**Kunde** Kundennummer. Wenn Sie eine Nummer angeben, werden Name und Ort des Kunden im Klartext angezeigt. Es können nur Aufträge für aktive Kunden erfasst werden.
*Technische Info: Pflichtfeld, numerisches Feld, Anzeigefelder, DB-Feld: kauf.kunr, kauf.orgname*

**Grund** Begründung für eine Terminänderung. Das Feld Grund wird nur angezeigt, wenn Sie den Liefertermin in einem bereits erfassten Auftrag ändern.
*Technische Info: alphanumerisches Feld, DB-Feld: kaufltedit.text*

**Bezug** Vorgangsnummer, auf die Bezug genommen wird. Sie können ein Angebot, einen Auftrag, eine Lieferantenanfrage oder eine Bestellung als Bezug auswählen.
Sie können alle Daten des Bezugsvorgangs oder nur die Kopfdaten des Bezugsvorgangs übernehmen.
Mit <F9> öffnen Sie den Dialog Suche Bezugsvorgang:
⇨ "Suche Bezugsvorgang" auf Seite D-1097
*Technische Info: numerisches Feld, DB-Feld: kauf.referenz*

**Vorgangsart für den Bezug vorauswählen**
Je nach Systemkonfiguration ist es möglich, eine der Vorgangsarten als Vorauswahl für die Bezugserfassung festzulegen:
- Mit <F8> wird im Feld **Bezug** die als Standard konfigurierte Vorgangsart im Feld angezeigt.
- Mit <F9> öffnen Sie einen Auswahldialog mit allen Vorgangsarten, auf die Bezug genommen werden kann. Mit den Pfeiltasten können Sie eine Vorgangsart wählen.
- Mit <Enter> bestätigen Sie die Auswahl.
- Im Feld **Bezug** wird die Nummer des aktuellen Marktpartners angezeigt.
- Wenn Sie den aktuellen Marktpartner als Vorauswahl festlegen möchten, dann bestätigen Sie mit <Enter>.
- Wenn Sie einen anderen Marktpartner als Vorauswahl festlegen möchten, dann öffnen Sie mit <F9> den Dialog Marktpartnersuche, um einen Marktpartner auszuwählen. Alternativ können Sie die Marktpartnernummer direkt im Feld angeben. Mit <Enter> bestätigen Sie die Auswahl.
- Das Feld **Bezug** ist leer. Wenn Sie jetzt den Dialog Suche Bezugsvorgang öffnen, dann sind die Vorgangsart und der Marktpartner, den Sie festgelegt haben, als Suchkriterien vorausgewählt.

**Vorgang mit Bezug erfassen**
- Mit <F9> öffnen Sie den Dialog Suche Bezugsvorgang, um einen Bezugsvorgang zu den angegebenen Kriterien auszuwählen. Alternativ können Sie die Vorgangsnummer direkt im Feld angeben.
- Mit <Enter> bestätigen Sie die Auswahl. Sie können alle Daten des Bezugsvorgangs oder nur die Kopfdaten des Bezugsvorgangs übernehmen.

**Haus** Firmennummer und Mandantennummer (Hausnummer), in der der Auftrag angelegt wird. Das Feld Haus ist nur freigeschaltet, wenn Sie mit interner Mandantentrennung arbeiten. Die Firmennummer wird automatisch aus den Systemstammdaten herangezogen und in einem Anzeigefeld angezeigt.
*Technische Info: numerische Felder, DB-Felder: kauf.company, kauf.hausnr*

**Erf. Datum** Erfassungsdatum. Standardmäßig ist das Feld mit dem aktuellen Datum vorbelegt. Wenn Sie den Eintrag ändern wollen, müssen Sie das neue Datum zweimal eingeben.
*Technische Info: Pflichtfeld, Datumsfeld, DB-Feld: kauf.edat*

**Knd-Bestnr** Externe Kundenbestellnummer. Für Aufträge aus einem anderen Haus steht in diesem Feld die Auftragsnummer des sendenden Hauses.
*Technische Info: alphanumerisches Feld, DB-Feld: kauf.exaufnr*

**Termin** Gewünschter Liefertermin des Kunden. Im ersten Feld können Sie die Kalenderwoche angeben. Im zweiten Feld können Sie das Datum im Format TT.MM.JJJJ angeben. Wenn Sie die Kalenderwoche und die Route angegeben haben, können Sie sich im zweiten Feld die möglichen Termine mit <F9> in einem Auswahldialog anzeigen lassen. Es werden nur die Termine angezeigt, die für die Tourenplanung in den Stammdaten angelegt sind.
Ob alle Auftragspositionen zum gewünschten Liefertermin komplett bereitgestellt werden können, wird vom System nach der Auftragseinlastung in das Produktionssystem geprüft. Kann bis zum gewünschten Termin nicht geliefert werden, meldet das System diesen Umstand per E-Mail an den Auftragserfasser und verschiebt das Datum auf den nächstmöglichen Liefertermin.
*Technische Info: Pflichtfeld, numerisches Feld, Datumsfeld, DB-Felder: kauf.kwideal, kauf.Itideal*

> **Angebot mit Termin**
> Das System kann so konfiguriert werden, dass ein Angebot mit Termin zu einer Wiedervorlage führt. Der Erfasser erhält an dem entsprechenden Datum bei Programmstart eine Mitteilung, damit Angebote nachverfolgt werden können.

**Route** Routennummer. In der Routenauswahl sind die Fahrstrecken sowie die jeweiligen Routentage aufgelistet. Sie können in den Kundenstammdaten eine Hauptroute und drei alternative Routen hinterlegen. Die Route wird anhand der Kunden-, Adressdaten und Systemkonfiguration aus den Stammdaten ermittelt. Wenn die Via-Plant-Funktion konfiguriert ist, wählen Sie mit <F5> das Haus, über das die Auslieferung organisiert werden soll.
Für Informationen zur Via-Plant-Funktion kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.
*Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kauf.routenr*

**Geplant** Anzeige des geplanten Lieferdatums. Der geplante Auslieferungstermin wird anhand verschiedener Daten, z. B. Handlingszeit, Fahrtdauer und Kapazitätsplanung, ermittelt und im Feld Geplant als geplantes Auslieferungsdatum eingetragen.
*Technische Info: Anzeigefeld, DB-Feld: kauf.ltplan*

**Knd-Pos** Angaben zur Position aus der Positionsliste des Kunden. Die Kundenpositionen werden im Register Allgemein in dem Feld Ku.Pos. angezeigt:
- **Pos:** Das Feld Ku.Pos auf Positionsebene wird freigeschaltet. Die Auftragspositionen können nach kundenindividuellen Positionsbezeichnungen erfasst werden, z. B. 1.1, 4.2, A_1, G_4.
- **Typ:** Die Positionen werden nach Glastypen erfasst.
- **keine:** Das Feld Ku.Pos ist auf Positionsebene gesperrt. Die kundenindividuellen Positionsbezeichnungen können nicht verwendet werden.
*Technische Info: Toggle-Feld, DB-Feld: kauf.kndposkz*

**Term. Art** Information über die Terminierungsart, die auf den Auftrag gedruckt wird. Wenn als Terminierungsart Abruf oder eilt ausgewählt ist, dann wird der Termin an A+W Production weiter geleitet. Bei **eilt** wird die Produktion der Ware bei der Einlastung bevorzugt. Bei **Abruf** wird die Produktion so geplant, dass die Ware auf Abruf geliefert werden kann.
- (keine Auswahl): Terminierungsart ist nicht festgelegt.
- **Abruf:** Termin auf Abruf.
- **eilt:** Auftrag wird als Eilauftrag an die Produktion übergeben.
- **mögl:** möglichst zum Termin.
- **verbl:** Termin ist verbindlich. Das System kann den gewünschten Liefertermin nicht ändern.
- **ohne:** ohne verbindlichen Termin.
- **Auto:** Termin wird automatisch vergeben.
- **folgt:** Termin folgt. Die Terminabsprache erfolgt erst noch.
*Technische Info: Toggle-Feld, DB-Feld: kauf.abrufkz*

**Eingang** Typ des Kommunikationskanals über den der Auftrag eingegangen ist. Diese Information wird für statistische Auswertungen, Tests und zu Recherchezwecken benutzt.
- **Vertreter:** Der Auftrag wurde von einem Außendienstmitarbeiter entgegengenommen.
- **Brief:** Der Auftrag ist per Post eingegangen.
- **Fax:** Der Auftrag ist per Fax eingegangen.
- **Telefon:** Der Auftrag ist per Telefon eingegangen.
- **DFÜ:** Der Auftrag wurde elektronisch übermittelt. Wenn Sie eine Rabattmethode mit Kriterium DFÜ in den Stammdaten hinterlegt haben, wird dieser Rabatt bei dem gewählten Eingangstyp DFÜ für den Auftrag ausgewertet.
- **Theke:** Der Auftrag wurde im Geschäft erfasst.
- **Test:** Der Auftrag wurde nur zu Testzwecken erfasst und geht nicht in die Produktion.
- **Barverkauf:** Der Auftrag wurde im Geschäft gegen Barzahlung entgegengenommen.
- **K-Dienst:** Der Auftrag wurde vom Kundendienst entgegengenommen.
- **Ersatz:** Ein Ersatzauftrag kann ausgestellt werden, wenn der reguläre Auftrag verloren geht.
- **EURO-Konv:** Funktionalität zur Umstellung auf Euro (nicht auswählbar).
- **Abschlag:** Sobald eine Abschlagsrechnung erstellt ist, wird vom System die Bezeichnung Abschlag in das Feld eingetragen. Der Wert Abschlag kann nicht manuell ausgewählt werden.
- **Schluss:** Sobald eine Schlussrechnung erstellt ist, wird vom System die Bezeichnung Schluss in das Feld eingetragen. Der Wert Schluss kann nicht manuell ausgewählt werden.
- **Online:** Der Auftrag ist online eingegangen, z. B. über die Webanwendung oder iQuote. Wenn Sie eine Rabattmethode mit Kriterium online in den Stammdaten hinterlegt haben, wird dieser Rabatt bei dem gewählten Eingangstyp online für den Auftrag ausgewertet.
- **E-Mail:** Der Auftrag ist per Mail eingegangen.
*Technische Info: Toggle-Feld, DB-Feld: kauf.eingang*

**Rechnungstyp** Angabe, für welche Leistungen die Rechnung erstellt wird. In der Regel werden die Gläser und Montageleistungen gemeinsam berechnet. Auf Wunsch können Sie einzelne Rechnungen erstellen.
- **Gesamt:** Die Rechnung wird für den kompletten Auftrag erstellt, d. h. für Material und Montageleistungen.
- **Glas:** Die Rechnung wird nur für das Material des Auftrags erstellt.
- **Dienstltg:** Die Rechnung wird nur für die Montageleistung des Auftrags erstellt.
*Technische Info: Toggle-Feld, DB-Feld: kauf.rechart*

**Objekt** Objektnummer. Ein Objekt ist dem Marktpartner zugeordnet und kann z. B. eine Baustelle des Kunden sein und eine andere Lieferadresse haben. Mit dem Objekt können Sie besondere Konditionen verknüpfen, die nur für dieses Objekt gelten, z. B. Rabatte oder Zahlungsoptionen. Sie haben die Möglichkeit objektbezogen abzurechnen.
Mit <F9> öffnen Sie die Objekt-Suche.
⇨ "Objekt-Suche" auf Seite D-1118
*Technische Info: numerisches Feld, DB-Feld: kauf.objnr*

#### Positionsebene
In diesem Bereich erfassen und bearbeiten Sie die Positionen eines Auftrags. Die Register zu den Auftragspositionen sind separat beschrieben:
⇨ "Auftragspositionen" auf Seite D-1167

#### Fußbereich
Im Fußbereich werden die Gesamtauftragswerte der Positionen angezeigt. Sie können einen allgemeinen Rabatt gewähren und den Betrag im Feld Nettototal überschreiben. Die Felder können nur betreten werden, wenn Sie die Positionserfassung abgeschlossen haben.

- Mit <Ende> wechseln Sie aus der Positionsebene in den Fußbereich.
- Mit <F2> öffnen Sie den Dialog Auftragserfassung für die Berechnung von Rabatten und des Nettototalbetrags.
  ⇨ "Auftragserfassung - Summen" auf Seite D-1157

**Sender** Anzeige der Hausnummer (Mandantennummer) und der Referenznummer. Die Referenznummer kann die Vorgangsnummer sein, die als Bezug in der Vorgangserfassung für den Vorgang angegeben wurde, oder bei DFÜ-Aufträgen die Auftrags- oder Bestellnummer.
*Technische Info: Anzeigefelder, DB-Felder: kauf.hausnr*

**ST, kg, qm** Anzeige der Gesamtsumme der Auftragswerte für die Menge in Stück, Gewicht in Kilogramm und Fläche in Quadratmeter.
*Technische Info: Anzeigefelder, DB-Felder: kauf.gesst, kauf.gesm2, kauf.gesgewicht*

**Gesamt** Anzeige des Gesamtpreises aller Positionen abzüglich der Positionsrabatte aus dem Feld Abzgl im Register Preise. Der Gesamtpreis wird je nach Preisart unterschiedlich berechnet.
⇨ "Auftragspositionen – Preise" auf Seite D-1185
⇨ Preise und Konditionen, "Preisarten" auf Seite C-572
*Technische Info: Anzeigefeld, DB-Feld: kauf.gesnetto*

**Rabatt** Auf den Gesamtbetrag gewährter Rabatt in Prozent. Bei gewährtem Rabatt wird der Betrag im Feld Nettototal angepasst.
*Technische Info: numerisches Feld, DB-Feld: kauf.gesfaktor*

**Nettototal** Summe aller Positionspreise, inkl. Rabatte und Zuschläge. Wenn Sie den Betrag bearbeiten, wird die Differenz vom System berechnet und im Feld Allg. Abschlag oder Allg. Aufschlag im Berechnungsdialog angezeigt.
⇨ "Auftragserfassung - Summen" auf Seite D-1157
Wenn das Feld Nettototal leer ist oder der Wert 0 ist, wird eine Abfrage angezeigt, ob Sie den Vorgang überarbeiten wollen. Mit [Ja] gelangen Sie zurück in die Auftragserfassung. Mit [Nein] wird der Dialog Reklamations-Statistik geöffnet.
⇨ "Reklamation" auf Seite D-1214
*Technische Info: numerisches Feld, DB-Feld: kauf.nettototal*

**+MwSt ()** Anzeige der Mehrwertsteuer. Im Feld steht der Mehrwertsteuerbetrag, der auf den Nettobetrag aufgeschlagen wird. In den Klammern wird der geltende Mehrwertsteuersatz in Prozent angezeigt.
*Technische Info: Anzeigefeld, DB-Feld: kauf.mwstbetrag*

**Brutto** Anzeige des Brutto-Gesamtbetrags. Der Betrag wird aus dem Nettobetrag zuzüglich der Mehrwertsteuer berechnet.
*Technische Info: Anzeigefeld, DB-Feld: kauf.gesbrutto*

**D-Beitrag** Anzeige des Deckungsbeitrags (Bruttogewinn), den die Gesamtmenge der Positionen zur Deckung der Fixkosten beiträgt. Der Deckungsbeitrag ist die Differenz zwischen dem Umsatz und den variablen Kosten der Positionen. Berücksichtigt werden alle Rabatte und Aufschläge.
*Technische Info: Anzeigefeld, DB-Feld: kauf.dbdm*

**%** Anzeige des Deckungsbeitrags in Prozent.
*Technische Info: Anzeigefeld, DB-Feld: kauf.dbvh*

**[Sichern]** Sichert die bereits eingetragenen Daten in der Vorgangserfassung. Bei einem Systemabsturz kann die Vorgangserfassung mit den gesicherten Daten fortgesetzt werden.
Wird die Vorgangserfassung abgebrochen, erscheint ein Hinweis, dass die gesicherten Daten bei einem Abbruch verloren gehen. Wenn Sie bestätigen wird die Vorgangserfassung abgebrochen und die gesicherten Daten werden gelöscht.

**[Anhänge(0)]** Diese Schaltfläche zeigt in Klammern die Anzahl der Dokumente an, die an diesen Vorgang angehängt wurden aus der Datenbank-Tabelle KAUFREF. Auf Kopf-/Fuß-Ebene zeigt die Anzahl, die dem Vorgang global zugeordneten Dokumente und auf Positionseben die direkt der einzelnen Position zugeordneten, an.
Ist die Schaltfläche aktiv, so kann man durch Betätigen dieser den Dialog für die Dokumentenanhänge starten. Die Schaltfläche kann über eine Umgebungsvariable deaktiviert werden, wenn keine Interesse an der Information besteht.

### Auftragserfassung – Anschriften
> Verkauf > Auftragserfassung > Register Anschriften

*(Abb. D-37: Auftragserfassung - Anschriften zeigt den Anschriften-Tab mit zwei Hauptbereichen: "Kundenanschrift" und "Lieferanschrift", beide mit detaillierten Adressfeldern.)*

In diesem Register bearbeiten Sie die Kunden- und Lieferanschrift. Die Kundenanschrift wird aus den Stammdaten des Kunden oder des Objekts herangezogen.

Sie können die Ermittlung der Lieferanschrift kundenspezifisch konfigurieren. Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

#### Kopfbereich
Die Felder im Kopfbereich sind zum Register Auftragserfassung – Kopf-, Fußbereich beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-1135

#### Kundenanschrift
**Name, Vorname** Name und Vorname des Kunden.
*Technische Info: alphanumerische Felder, DB-Felder: kauf.orgname, kauf.orgvorname*

**Anrede** Nummer der Anrede. Wenn Sie eine Nummer auswählen, wird die Anrede im Klartext angezeigt.
*Technische Info: numerisches Feld, DB-Feld: kauf.organrede*

**Z. Hd.** Zu Händen. Name der Person, an die die Lieferung ausgehändigt werden soll.
*Technische Info: alphanumerisches Feld, DB-Feld: kauf.orgzhd*

**Zusatz** Zusatztext der Anschrift.
*Technische Info: alphanumerisches Feld, DB-Feld: kauf.orgbranche*

**Straße** Straßenname und Hausnummer der Lieferanschrift.
*Technische Info: alphanumerisches Feld, DB-Feld: kauf.orgstr*

**PLZ, Fach** Postleitzahl und Nummer des Postfachs.
*Technische Info: alphanumerische Felder, DB-Felder: kauf.orgpfplz, kauf.orgpostfach*

**PF Ort** Ortsname des Postfachs.
*Technische Info: alphanumerisches Feld, DB-Feld: kauf.orgpfort*

**PLZ, Ort** Postleitzahl und Ortsname der Lieferanschrift.
*Technische Info: alphanumerische Felder, DB-Felder: kauf.orgplz, kauf.orgort*

**KFZ Land** Internationales Landeskennzeichen für Kraftfahrzeuge des Ziel-Landes. Wenn Sie ein Kennzeichen angeben, wird der Landesname im Klartext angezeigt.
*Technische Info: alphanumerische Felder, DB-Felder: kauf.orgkfzcode, kauf.orgland*

**Tel** Zwei Felder für Telefonnummer des Kunden. Im ersten Feld ist die Nummer (Nummer des Festanschlusses) aus dem Kunden-Stammdaten - Adresse, Feld Telefon angezeigt. Im zweiten Feld ist die Nummer (Mobiltelefonnummer) aus dem Kunden-Stammdaten - Adresse, Feld Mobil angezeigt.
*Technische Info: alphanumerische Felder, DB-Felder: kauf.orgtel, kauf.c_dummy1*

**Fax** Faxnummer des Kunden.
*Technische Info: alphanumerisches Feld, DB-Feld: kauf.faxnr*

**E-Mail** E-Mail-Adresse des Kunden.
*Technische Info: alphanumerisches Feld, DB-Feld: kauf.orgemail*

**Sprache** Nummer der Landessprache des Kunden, in der die Dokumente gedruckt werden. Wenn Sie eine Nummer auswählen, wird die Sprache im Klartext angezeigt.
*Technische Info: numerisches Feld, DB-Feld: kauf.sprkz*

**Kennz.** Schlüsselnummer für den Steuertyp. Der Steuertyp ist in den Systemstammdaten hinterlegt. Wenn Sie eine Nummer auswählen, wird die Bezeichnung des Steuertyps im Klartext angezeigt.
*Technische Info: numerisches Feld, DB-Feld: kauf.kukz*

#### Lieferanschrift
Sie können eine abweichende Lieferanschrift angeben, z. B. die Adresse einer Baustelle.

- Mit <Strg> + <N> legen Sie eine neue Lieferanschrift für den Kunden an.
  ⇨ "Neue Lieferadresse" auf Seite D-1192
- Mit <Strg> + <L> wählen Sie eine hinterlegte Lieferanschrift des Kunden aus.
  ⇨ "Adressen Suche" auf Seite D-1099

Die Felder sind zum Bereich **Kundenanschrift** beschrieben:
"Kundenanschrift" auf Seite D-1143

Zusätzlich ist folgendes Feld beschrieben:

**Region** Versandregion. Die Versandregion ist in den Systemstammdaten hinterlegt und wird über die PLZ ermitelt.
*Technische Info: Anzeigefeld*

#### Fußbereich
Die Felder und Schaltflächen im Fußbereich sind zum Register Auftragserfassung - Kopf-, Fußbereich beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-1135

Sie können die Felder im Fußbereich erst bearbeiten, wenn Sie die Positionserfassung abgeschlossen haben. Mit <Ende> wechseln Sie aus der Positionsebene in den Fußbereich.

### Auftragserfassung – Eigenschaften
> Verkauf > Auftragserfassung > Register Eigenschaften

*(Abb. D-38: Auftragserfassung – Eigenschaften zeigt den Eigenschaften-Tab, unterteilt in "Mitarbeiterzuordnung", "Versandinformationen" und "Rechnungs- und Druckoptionen" mit vielen Auswahlfeldern und Checkboxen.)*

In diesem Register bearbeiten Sie die Angaben zur Mitarbeiterzuordnung, den Versandinformationen und den Rechnungs- und Druckoptionen.

#### Kopfbereich
Die Felder im Kopfbereich sind zum Register Auftragserfassung – Kopf-, Fußbereich beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-1135

#### Mitarbeiterzuordnung
**Bestellt von** Mitarbeiternummer. Wenn Sie eine Nummer auswählen, wird der Name des Mitarbeiters im Klartext angezeigt. Mit <F5> öffnen Sie den Dialog Ansprechpartner, in dem Sie einen Ansprechpartner wählen oder neu anlegen können.
⇨ "Ansprechpartner" auf Seite D-1199
*Technische Info: numerisches Feld, DB-Feld: kauf.busr*

**Bestelldatum** Datum des Auftragseingangs.
*Technische Info: Datumsfeld, DB-Feld: kauf.bdat*

**Erfasser** Mitarbeiternummer und Name des Sachbearbeiters, der den Vorgang erfasst hat. Die Felder werden vom System vorbelegt. Sie können nicht bearbeitet werden.
*Technische Info: Anzeigefelder, DB-Feld: kauf.esuer*

**Abteilung** Nummer der Abteilung, der der Erfasser zugeordnet ist. Die Felder werden vom System vorbelegt. Sie können nicht bearbeitet werden.
*Technische Info: Anzeigefelder, DB-Feld: mitarb.abtnr*

**Sachbearbeiter** Mitarbeiternummer und Name des Sachbearbeiters, der den Vorgang bearbeitet, aber nicht erfasst hat. Wenn Sie eine Nummer auswählen, wird der Name des Sachbearbeiters im Klartext angezeigt.
*Technische Info: numerisches Feld, DB-Feld: kauf.abvertr*

**Außendienst** Name des Außendienst-Mitarbeiters.
*Technische Info: alphanumerisches Feld, DB-Feld: kauf.vertr*

**Vertr. (Erlös)** Vertreter-Erlös. Mitarbeiternummer des Vertreters, an den die Provision ausgezahlt wird. Wenn Sie eine Nummer auswählen, wird der Name des Vertreters im Klartext angezeigt.
*Technische Info: numerisches Feld, DB-Feld: kauf.vertrerloe*

#### Versandinformationen
**Max. Abladung** Maximales Gewicht, das der Kunde mit seinem technischen Gerät abladen kann.
*Technische Info: numerisches Feld, DB-Feld: kauf.gmaxgew*

**Zustellung** Vermerk über die gewünschte Art der Zustellung:
- **Abholung:** Der Kunde holt die Ware selbst ab.
- **Streckengeschäft:** Die Ware wird vom beauftragten Produktionsbetrieb direkt an den Endkunden ausgeliefert.
- **keine Auswahl:** Die Ware wird über die Route ausgeliefert, die im Kopfbereich erfasst ist.
*Technische Info: Toggle-Feld, DB-Feld: kauf.geschart*

**Direktauslief.** Angabe, ob der Kunde direkt von den Produktionsstätten beliefert wird oder ob die Ware ins Handelshaus geliefert wird. Das Kennzeichen wird vom System vorbelegt.
- J: Die Ware wird direkt an den Kunden geliefert.
- N: Die Ware wird an das bestellende Handelshaus geliefert.
*Technische Info: Toggle-Feld, DB-Feld: kauf.drkliefkz*

**Lieferart** Nummer der Lieferart, z. B. frei Haus. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Lieferart im Klartext angezeigt.
*Technische Info: numerisches Feld, DB-Feld: kauf. lieferart*

**Versandart** Nummer der Versandart, z. B. LKW. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Versandart im Klartext angezeigt.
*Technische Info: numerisches Feld, DB-Feld: kauf.versandart*

**Verpackungsart** Nummer der Verpackungsart, z. B. Kiste. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Verpackart im Klartext angezeigt.
*Technische Info: numerisches Feld, DB-Feld: kauf. verpackart*

**Gest.-Beladung** Gestell-Beladung. Sie wählen aus, nach welchen Kriterien die Ware auf den Gestellen sortiert wird:
- **Pos:** nach Positionen.
- **Größe:** nach Größe.
- **SZR+Gr:** nach Scheibenzwischenraum und Größe.
- **Pos(frei):** Positionen zusammengehalten aber frei organisiert.
- **HM Glas Farb Dick:** nach Hardmaß, Glasmaß, Farbe und Dicke.
- **HM Gl.maß Farbe:** nach Hardmaß, Glasmaß und Farbe.
- **HM Gl.maß - Dicke:** nach Hardmaß, Glasmaß und Dicke.
- **HM - Farbe Dicke:** nach Hardmaß, Farbe und Dicke.
- **HM Glasmaß:** nach Hardmaß und Glasmaß.
- **HM - Farbe:** nach Hardmaß und Farbe.
- **HM - - Dicke:** nach Hardmaß und Dicke.
- **HM---:** nach Hardmaß.
- **Kommission:** nach Kommissionstext.
Die Auswertung der ausgewählten Kriterien ist von der Systemkonfiguration abhängig.
*Technische Info: Toggle-Feld, DB-Feld: kauf.gbelad*

**Ausgangszoll** Nummer der Ausgangszollstelle für die Lieferpapiere. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Zollstelle im Klartext angezeigt.
*Technische Info: numerisches Feld, DB-Feld: kauf.azsnr*

**Bestimmungszoll** Nummer der Zollstelle des Empfängerlandes. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Zollstelle im Klartext angezeigt.
*Technische Info: numerisches Feld, DB-Feld: kauf.bzsnr*

**Fahrtdauer/km** Voraussichtliche Fahrzeit und Anzeige der Fahrstrecke. Die Fahrtdauer wirkt sich auf den Liefertermin aus. Die Fahrstrecke wird aus dem Feld Entfernung der Lieferadresse herangezogen.
*Technische Info: numerische Felder, DB-Felder: kauf.anfahrt*

**Auslief. Route** Auslieferungsroute bei Auslieferung oder Versand über ein zweites Haus. Das Feld ist nur freigeschaltet, wenn die interne Mandantentrennung aktiv ist.
*Technische Info: numerische Felder, DB-Felder: kauf.endroutenr*

**Via Haus** Anzeige der Mandantennummer des Hauses, über das die Ware geschickt wird bei Auslieferung oder Versand über ein zweites Haus. Das Haus wird automatisch angezeigt, wenn Sie eine Auslieferungsroute angeben.
*Technische Info: Anzeigefeld, DB-Feld: kauf._vsvia*

#### Rechnungs- und Druckoptionen
**USt-Ident-Nr.** Umsatzsteuer-Identifikationsnummer des Kunden.
*Technische Info: alphanumerisches Feld, DB-Feld: kauf.steuernr*

**FA-Steuer-Nr.** Finanzamt-Steuer-Nummer des Kunden.
*Technische Info: alphanumerisches Feld, DB-Feld: kauf.finstnr*

**Kostenstelle** Bezeichnung der Kostenstelle für statistische Auswertungen.
*Technische Info: alphanumerisches Feld, DB-Feld: kauf.kostenst*

**Rechnungsart** Art der Rechnung.
- **Einzelrechnung:** Der Rechnungsempfänger bekommt für jeden Auftrag eine separate Rechnung zugestellt.
- **Deckblattrechnung:** Der Rechnungsempfänger bekommt für jeden Auftrag eine separate Deckblattrechnung zugestellt.
- **Sammelrechnung:** Der Rechnungsempfänger bekommt mehrere Aufträge zusammengefasst in einer Rechnung zugestellt. Sie können auswählen, in welchen Intervallen eine Sammelrechnung ausgestellt wird.
  - wöchentlich
  - 14-tägig
  - monatlich
*Technische Info: Toggle-Feld, DB-Feld: kauf.rechungsart*

**Sammelrechnungslimit** Maximaler Rechnungsbetrag, bis zu dem Sie eine Sammelrechnung erstellen können. Wenn das Limit überschritten ist, werden die Rechnungen als Einzelrechnungen erstellt.
*Technische Info: numerisches Feld, DB-Feld: kauf.srechlimit*

> **Hinweis zur Sammelrechnungserstellung**
> Das Einverständnis des Rechnungsempfängers zur Sammelrechnung sowie die Festlegung des Sammelrechnungslimits ist in den Marktpartner-Stammdaten hinterlegt.

**Teilfaktura** Angabe, ob Teilabrechnungen nach einer Teillieferung erstellt werden:
- J: Die Teilabrechnungen zulassen.
- N: Keine Teilabrechnungen zulassen.
Wenn Sie als Rechnungsart Sammelrechnung wählen und Teilabrechnungen zulassen, werden nach jeder Teillieferung die ausgelieferten Artikel mit der nächsten Sammelrechnung fakturiert.
*Technische Info: Toggle-Feld, DB-Feld: kauf.teilfakkz*

**Fakturasperre** Die Rechnungsstellung kann für den Vorgang gesperrt werden. Bei aktiver Sperre erhält der Rechnungsempfänger vorläufig keine Rechnung für den Auftrag.
- J: Die Rechnungsstellung sperren.
- N: Die Rechnungsstellung zulassen.
*Technische Info: Toggle-Feld, DB-Feld: kauf.fakturastop*

**Teillieferung** Angabe, ob der Kunde Teillieferungen akzeptiert, oder diese nicht wünscht. Die Angabe dient nur zur Information. Auch wenn N ausgewählt ist, ist es möglich Teillieferscheine für den Auftrag zu erstellen.
- J: Die Teillieferungen zulassen.
- N: Keine Teillieferungen zulassen.
*Technische Info: Toggle-Feld, DB-Feld: kauf.teilfakkz*

**Eilauftrag** Der aktuelle Auftrag kann bevorzugt und mit höherer Priorität in die Produktion eingelastet werden.
- J: Den Auftrag mit höherer Priorität einlasten.
- N: Keine höhere Priorität für den Auftrag vergeben.
*Technische Info: Toggle-Feld, DB-Feld: kauf.schnell*

**Bruttopreise drucken** Die Bruttopreise können auf den marktpartnerseitigen Dokumenten ausgewiesen und gedruckt werden.
- J: Die Bruttopreise ausweisen und drucken.
- N: Keine Bruttopreise ausweisen und drucken.
*Technische Info: Toggle-Feld, DB-Feld: kauf.preisdrkz*

**Kundenfaktor drucken** Der kundenspezifische Faktor kann auf den marktpartnerseitigen Dokumenten ausgewiesen und gedruckt werden.
- J: Den Kundenfaktor ausweisen und drucken.
- N: Keinen Kundenfaktor ausweisen und drucken.
*Technische Info: Toggle-Feld, DB-Feld: kauf.rabdrkz*

**Beispiel:**
Wenn der Kunde 10% Rabatt bekommt, dann beträgt der Wert für den Kundenfaktor = 0,9.

**Bearbeitungspreise drucken** Die Bearbeitungspreise für Bearbeitungen können separat ausgewiesen und gedruckt werden.
- J: Die Preise für Bearbeitungen separat ausweisen und drucken.
- N: Keine separaten Preise für Bearbeitungen ausweisen und drucken.
- P: Die Preise für Bearbeitungen werden separat ausweisen und drucken, sofern diese vorhanden sind.
*Technische Info: Toggle-Feld, DB-Feld: kauf.explbearbkz*

**Verglasung** Die Kosten der Verglasung können auf der Rechnung unterschiedlich angezeigt werden.
- **In Position einrechnen:** Die Kosten der Verglasung werden in die Position eingerechnet.
- **Nur im Fuß ausweisen:** Die Kosten der Verglasung werden im Fuß der Rechnung ausgewiesen.
- **In Position und Fuß:** Die Kosten der Verglasung werden in die Position eingerechnet und im Fuß der Rechnung ausgewiesen.
*Technische Info: Toggle-Feld, DB-Feld: kauf.verglaskz*

**Artikeltexte drucken** Die Artikeltexte können auf den marktpartnerseitigen Dokumenten gedruckt werden.
- J: Die Artikeltexte drucken.
- N: Keine Artikeltexte drucken.
*Technische Info: Toggle-Feld, DB-Feld: kauf.atxtdrukz*

**Modelle drucken** Die Modellskizze der Positionen kann im Anhang der marktpartnerseitigen Dokumente gedruckt werden.
- J: Die Modellskizze drucken.
- N: Keine Modellskizze drucken.
Die Einstellung von J oder N in diesem Feld wird, je nach konfigurierter Report-Variante, entweder repgo oder CrystalReport, ausgewertet.
*Technische Info: Toggle-Feld, DB-Feld: kauf.moddrkz*

**Positionspreise unterdrücken** Die Positionspreise werden standardmäßig auf den marktpartnerseitigen Dokumenten gedruckt. Sie können die Auflistung der Positionspreise unterdrücken, z. B. wenn mit dem Kunden ein Fixpreis für den gesamten Auftrag vereinbart wurde.
- J: Keine Positionspreise drucken.
- N: Die Positionspreise drucken.
*Technische Info: Toggle-Feld, DB-Feld: kauf.posdrkz*

#### Fußbereich
Die Felder und Schaltflächen im Fußbereich sind zum Register Auftragserfassung – Kopf-, Fußbereich beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-1135
Die Felder können nur betreten werden, wenn mindestens eine Position erfasst ist. Mit <Ende> wechseln Sie aus der Positionsebene in den Fußbereich.

### Auftragserfassung – Verschiedenes
> Verkauf > Auftragserfassung > Register Verschiedenes

*(Abb. D-39: Auftragserfassung – Verschiedenes zeigt den Tab "Verschiedenes" mit Bereichen für "Reklamationsinformation", "Private Felder", "Zahlungsoptionen", "Weitere Optionen" und "Details der Auslieferung".)*

In diesem Register werden Reklamationsinformationen, private Felder, weitere technische Informationen, Details der Auslieferung und die Zahlungsoptionen angezeigt. Sie können die Einträge bearbeiten.

#### Kopfbereich
Die Felder sind zum Register **Auftragserfassung – Kopf-, Fußbereich** beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-1135

#### Reklamationsinformation
Mit diesen Daten können Sie eine Reklamationsstatistik führen. Die **Art**, der **Ort** und der **Typ** der Reklamation müssen in den Stammdaten angelegt sein.

**Art** Nummer der Reklamationsart. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Reklamationsart im Klartext angezeigt, z. B. Glasbruch.
*Technische Info: numerisches Feld, DB-Feld: kauf.reklamart*

**Ort** Nummer des Reklamationsorts. Wenn Sie eine Nummer auswählen, wird die Bezeichnung des Reklamationsorts im Klartext angezeigt, z. B. Entladung.
*Technische Info: numerisches Feld, DB-Feld: kauf.reklamort*

**Typ** Nummer des Reklamationstyps. Wenn Sie eine Nummer auswählen, wird die Bezeichnung des Reklamationstyps im Klartext angezeigt, z. B. falsche Farbe.
*Technische Info: numerisches Feld, DB-Feld: kauf.reklamspec*

**Datum** Reklamationsdatum im Format TT.MM.JJJJ. Standardmäßig wird der aktuelle Tag angezeigt. Sie können das Reklamationsdatum bearbeiten.
*Technische Info: Datumsfeld, DB-Feld: kauf.reklamdat*

#### Zahlungsoptionen
**Währung Kurs** Nummer und Name der Währung und Währungskurs. Der Preis wird kundenbezogen in der angegebenen Währung berechnet. Wenn Sie eine Nummer auswählen, werden Währungsname und Währungskurs im Klartext angezeigt. Das Feld **Kurs** ist gesperrt, wenn die Eigenwährung gewählt ist.
*Technische Info: Pflichtfeld, numerische Felder, DB-Felder: kauf.waehrung, kauf.kurs*

**Kalkulation in** Das Feld ist nur freigeschaltet, wenn im Feld **Währung** nicht die Eigenwährung gewählt ist. Sie können festlegen, ob die Preise in der Eigenwährung oder in der Fremdwährung des Marktpartners berechnet werden:
- **Eigenwährung:** Die Preise werden in der Eigenwährung von A+W Enterprise berechnet.
- **Fremdwährung:** Die Preise werden in der Währung berechnet, die dem Marktpartner im Feld Währung zugewiesen ist.
*Technische Info: Toggle-Feld, DB-Feld: kauf.waehrprs*

**Ausdruck in** Nummer für den Ausdruck der marktpartnerspezifischen Unterlagen in der kalkulierten Währung oder der Fremdwährung. Wenn Sie eine Nummer auswählen, wird die Bezeichnung der Druckoption im Klartext angezeigt. Für den Druck muss der entsprechende Report hinterlegt sein.
*Technische Info: numerisches Feld, DB-Feld: kauf.waehrdru*

> **Die Felder Kalkulation in und Ausdruck in**
> Die Felder Kalkulation in und Ausdruck in sind nur zugänglich, wenn das Währungs-Modul lizenziert ist.

**Zahlziel** Zahlungsziel in Tagen, das mit dem Marktpartner vereinbart wurde.
*Technische Info: numerisches Feld, DB-Feld: kauf.zahlziel*

**Valuta** Frist zur Wertstellung in Tagen.
*Technische Info: numerisches Feld, DB-Feld: kauf.valuta*

**Beispiel:**
Ist eine Rechnung am 15. des Monats fällig, würde der Eintrag von 2 Tagen bewirken, dass der Fälligkeitstermin in der Finanzbuchhaltung um zwei Tage erhöht wird, also zum 17. des Monats. Diese Tage werden z. B. für den Postweg einkalkuliert.

**Skonto 1, Skonto 2, Skonto 3** Schlüssel der Skontosätze für das Zahlungsziel. Sie können bis zu 3 verschiedene Schlüssel angeben. Auf diese Weise können Sie gestaffelte Zahlungsziele definieren.
*Technische Info: numerische Felder, DB-Felder: kauf._skonto1, kauf._skonto2, kauf._skonto3*

**Merkmal** Nummer der Form der Bezahlung, z. B. Banklastschrift, Bankabbuchung. Sie hinterlegen Merkmale in den Systemstammdaten als Zahlungsweisem. Wenn Sie eine Nummer angeben, wird die Bezeichnung des Merkmals im Klartext angezeigt.
*Technische Info: numerisches Feld, DB-Feld: kauf.zahlngmerk*

**Zahlungsverkehr** Art und Weise der Bezahlung, z. B. Vorauskasse, Bankeinzug. Die Angaben zum Zahlungsverkehr sind vom System vorgegeben.
*Technische Info: Toggle-Feld, DB-Feld: kauf.skontoart*

**FIBU-Key** Schlüssel zur Übergabe an die Finanzbuchhaltung. Die Schlüssel der Finanzbuchhaltung werden vom System eingetragen und an die Finanzbuchhaltung gesendet.
*Technische Info: alphanumerisches Feld, DB-Feld: kauf.fibukey*

**FIBU-Debitor** Kundennummer des Marktpartners, der als Rechnungsempfänger bestimmt ist. Das Feld ist standardmäßig vorbelegt.
*Technische Info: numerisches Feld, DB-Feld: kauf.stddebnr*

**Bonus** Vereinbarter Bonus für den Vorgang, den ein Lieferant seinem Kunden gewährt. Die Höhe des Bonus richtet sich z. B. nach dem Umsatz, der mit dem Kunden innerhalb eines festgelegten Zeitraums erzielt wird. Der Bonus wird prozentual angegeben.
*Technische Info: numerisches Feld, DB-Feld: kauf. bonusnr*

**Provision** Vertreterprovisionssatz für den Auftrag. Die Provision wird prozentual angegeben.
*Technische Info: numerisches Feld, DB-Feld: kauf.provnr*

#### Private Felder
Die privaten Felder werden kundenspezifisch für Zusatzinformationen genutzt. Sie sind frei konfigurierbar. Die Feldbezeichnungen werden über die Umgebungsvariablen gesetzt. Die beiden oberen Zeilen sind numerische Felder, die beiden unteren Zeilen sind freie Textfelder.
*Technische Info: numerische Felder, alphanumerische Felder, DB-Felder: kauf.private_long1, kauf.private_long2, kauf.private_char1, kauf.private_char2*

#### Weitere Optionen
**Kontrolle** Nummer des Mitarbeiters, der den Vorgang kontrolliert. Wenn das Feld gefüllt ist, werden die Vorgänge erst nach Prüfung durch den entsprechenden Mitarbeiter freigeschaltet.
*Technische Info: numerisches Feld, DB-Feld: kauf.kontrollmanr*

**Windlast** Windlast am Einbauort. Windlast (N/m²) ist der Druck, der durch direkte Windeinwirkung auf die äußere Oberfläche eines Gebäudes ausgeübt wird. Die Windlast kann nur für Gläser mit mehreren Scheiben angegeben werden.
*Technische Info: numerisches Feld, DB-Feld: kauf.wlast*

> **Restriktionsprüfung bei Eingabe der Windlast**
> Wenn für die Windlast ein entsprechender Eintrag in den Stammdaten angelegt ist, wird die angegebene Windlast einer Restriktionsprüfung unterzogen. Das System prüft z. B., ob die Dickengruppe der gewählten Gläser für die angegebene Windlast ausreichend ist. Bei Verletzung der Restriktionsprüfung wird eine Meldung angezeigt.

**Fassadenzone** Angabe der Fassadenzone, in der die Scheiben verbaut werden. Hohe Gebäude oder Gebäude, die an Randgebieten stehen, werden z. B. mit einer erhöhten Windlast belastet.
- **1 Rand:** Für Gebäude mit erhöhter Windlast.
- **2 Zentral:** Für Gebäude ohne erhöhte Windlast.
*Technische Info: numerisches Feld, DB-Feld: kauf. bereich*

**Min/Max ISO Ges-Stärke** Minimale und maximale Glasstärke des gesamten ISO-Artikels in Millimeter. Die Glasstärke ist abhängig von der gewählten Fassadenzone und der Windlast.
*Technische Info: numerische Felder, DB-Felder: kauf.minszr, kauf.maxszr*

**Falzmaß** Korrekturmaß in Millimeter. Das Falzmaß wird auf die Breite und Höhe der Positionen aufgeschlagen. Z. B. werden für ein Glas mit den Maßen 1050 mm x 1250 mm und einem Falzmaß von 2 mm in der Datenbank die Maße 1052 mm x 1252 mm hinterlegt. Der Wert wird an die Produktion übergeben. Wenn Sie mit A+W Production arbeiten, wird dieser Wert in der Regel ignoriert und das Falzmaß aus A+W Production herangezogen.
*Technische Info: numerisches Feld, DB-Feld: kauf.falzmass*

**Textformeln** Nummer und Bezeichnung der Produktkennzeichnung, z. B. Rahmentext. Die Textformeln müssen in den Stammdaten angelegt sein.
*Technische Info: numerisches Feld, DB-Feld: kauf.artkennfrm*

**Angeb. Status** Status des Angebots. Dieses Feld wird nur bei Angeboten angezeigt. Bei Bezugnahme wird der Feldinhalt übernommen.
- **offen:** Das Angebot wurde noch nicht bestätigt.
- **gewonnen:** Das Angebot wurde bestätigt.
- **verloren:** Das Angebot wurde abgelehnt.
- **verjährt:** Das Angebot ist nicht mehr gültig.
*Technische Info: Toggle-Feld, DB-Feld: kauf.angbstatus*

#### Details der Auslieferung
Diese Felder werden vorbelegt, wenn die Via-Plant-Funktion konfiguriert ist. Mit der Via-Plant-Funktion können Auslieferungen zum Kunden über ein weiteres Haus organisiert werden. Dazu muss auch die interne Mandantentrennung aktiv sein.

**Ankunft in via Haus** Datum, an dem die Lieferung voraussichtlich im Haus ankommt, über das die Lieferung versendet wird.
*Technische Info: Anzeigefeld, DB-Feld: kauf.ankunftvia*

**via Haus** Mandantennummer des Hauses, über das die Lieferung versendet wird. Dieses Ziel-Haus können Sie im Kopfbereich im Feld Route mit <F5> festlegen.
*Technische Info: Anzeigefeld, DB-Feld: kauf.vsvia*

**Fahrtdauer** Voraussichtliche Fahrzeit zum Ziel-Haus. Die Fahrtdauer wirkt sich auf den Liefertermin aus.
*Technische Info: Anzeigefeld, DB-Feld: kauf.anfahrt*

**Handlingsz.** Handlings-Zeit, um die Lieferung im Ziel-Haus auf- oder abzuladen.
*Technische Info: Anzeigefeld, DB-Feld: kauf.handlingvia*

**Geplant in via** Datum der geplanten Auslieferung im Ziel-Haus. Das Datum gibt an, an welchem Tag die Lieferung das Ziel-Haus voraussichtlich verlässt.
*Technische Info: Anzeigefeld, DB-Feld: kauf.ltplanvia*

**Route** Nummer der Route. Auslieferungsroute zum Kunden hin. Die Route unterscheidet sich von der Route im Start-Haus.
*Technische Info: Anzeigefeld, DB-Feld: kauf.endroutenr*

**Ankunftstag bei Kunden** Datum, an dem die Lieferung beim Kunden ankommt.
*Technische Info: Anzeigefeld, DB-Feld: kauf.ankunft*

**Fahrtdauer** Voraussichtliche Fahrzeit vom Ziel-Haus zum Kunden. Die Fahrtdauer wirkt sich auf den Liefertermin aus.
*Technische Info: Anzeigefeld, DB-Feld: kauf.anfahrtvia*

**Wareneingangstermin** Datum, an dem die Lieferung am Wareneingang eintrifft. Das Datum wird im Format TT.MM.JJJJ angegeben.
*Technische Info: Datumsfeld, DB-Feld: kauf.ptermin1*

#### Fußbereich
Die Felder und Schaltflächen im Fußbereich sind zum Register Auftragserfassung – Kopf-, Fußbereich beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-1135
Die Felder können nur betreten werden, wenn Sie die Positionserfassung abgeschlossen haben. Mit <Ende> wechseln Sie aus der Positionsebene in den Fußbereich.

### Auftragserfassung – Summen
> Verkauf > Auftragserfassung > Auftragsfuß > Feld Rabatt, Nettototal > <F2>

*(Abb. D-40: Auftragserfassung (Summen) zeigt den Summen-Dialog zur Definition von auftragsweiten Rabatten, Ab- und Aufschlägen. Er enthält eine Liste von Rabatten und Felder zur Berechnung der Gesamtsumme, Skonto und Bruttobetrag.)*

In diesem Dialog definieren Sie Rabatte, Ab- und Aufschläge für den gesamten Auftrag und bearbeiten verschiedene Zahlungsoptionen.

Sie können prozentuale, fixe Rabatte und Rabatte pro Mengeneinheit gewähren und jeden Rabatt nach Mengeneinheit oder Auftragswert staffeln. Je nach Rabattart werden die Angaben als Preisnachlass oder Zuschlag berechnet. Wenn das System entsprechend konfiguriert ist, wird der Rabatt aus den Stammdaten herangezogen.

Die Änderungen der Gewinnspanne durch Rabatte müssen Sie an die FIBU übermitteln. Sie können die Rückverteilung automatisch vom System an die FIBU übergeben lassen oder manuell übergeben. Die manuelle Übergabe ist zum Register Detailansicht Rabatte beschrieben:
⇨ "Auftragserfassung - Detailansicht Rabatte" auf Seite D-1162

#### Kopfbereich
**Auftrag** Anzeige der Auftragsnummer.
*Technische Info: Anzeigefeld, DB-Feld: kauf.auftrnr*

**Kunde** Anzeige der Kundennummer und des Kundennamens.
*Technische Info: Anzeigefeld, DB-Feld: kauf.kunr*

**Verkauf** Anzeige der Summe der Positionspreise.
*Technische Info: Anzeigefeld, DB-Feld: kauf.nettototal*

**Kosten** Anzeige der Summe der Kosten, z. B. Einkaufspreise, Produktionskosten.
*Technische Info: Anzeigefeld, DB-Feld: kauf.ektotal*

#### Übersicht Rabatte
In diesem Bereich werden alle auftragsspezifischen Rabatte angezeigt. Sie können die Zuschläge und Rabatte prüfen, bearbeiten und neue Rabatte für den Auftrag gewähren.

- **(Checkbox ohne Bezeichnung):**
  Angabe, ob der Rabatt aktiv ist:
  - ☑ Der Rabatt wird auf den Auftragspreis berechnet.
  - ☐ Der Rabatt wird nicht berechnet.
  *Technische Info: Checkbox, DB-Feld: kaufrab.geloescht*
- **Name:**
  Bezeichnung des Rabatts.
  *Technische Info: Pflichtfeld, alphanumerisches Feld, DB-Feld: kaufrab.txt*
- **Seqnr:**
  Sequenznummer. Die Zuschläge und Rabatte werden in aufsteigender Reihenfolge der Sequenznummern berechnet.
  *Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kaufrab.seqnr*
- **Wert:**
  Festgelegter Berechnungswert des Rabatts. Der Berechnungswert ist abhängig von der gewählten Rabattart.
  *Technische Info: numerisches Feld, DB-Feld: kaufrab.wert*
- **Rabattart:**
  Angabe der Rabattart. Die Rabattart legt fest, ob der Rabatt ein Preisnachlass oder ein Zuschlag ist:
  - **(-):** Der Wert wird als Rabatt berechnet.
  - **(+):** Der Wert wird als Zuschlag berechnet.
  Im zweiten Feld geben Sie an, worauf sich der Rabatt bezieht:
    - **WE:** Der Rabatt wird als fester Betrag in der Währungseinheit gewährt.
    - **%:** Der Rabatt wird prozentual vom Gesamtauftragswert gewährt.
    - **WE/St:** Der Rabatt wird als fester Betrag in der Währungseinheit pro Stück gewährt.
    - **WE/qm:** Der Rabatt wird pro Quadratmeter der Gesamtscheibenfläche in der Währungseinheit gewährt.
    - **WE/kg:** Der Rabatt wird pro Kilogramm des Gesamtgewichts in der Währungseinheit gewährt.
    - **WE/km:** Der Rabatt wird pro Kilometer der Gesamtroute in der Währungseinheit gewährt.
    - **%/VK:** Kostenrabatt auf Basis des Verkaufsbetrags. Dieser Rabatt wird mit dem Basiswert des Verkaufsbetrages berechnet.
    - **%/Kst:** Verkaufsrabatt auf Basis der Kosten. Dieser Rabatt wird mit dem Basiswert des Kostenbetrages berechnet.
    - **WE/G*E:** Wert pro Gewicht in kg multipliziert mit der Entfernung in km. Dieser Rabatt wird nur dann angewendet, wenn die Entfernung in den Adressen oder im Marktpartner hinterlegt wurde.
  *Technische Info: Toggle-Felder, DB-Felder: kaufrab.satzart, kaufrab.rabtyp*
- **Typ:**
  Angabe des Rabatttyps. Der Rabatttyp gibt an, auf welchen Preis der Rabatt sich bezieht:
  - **Verkauf:** Zur Berechnung des Rabatts wird der Verkaufspreis herangezogen.
  - **Kosten:** Zur Berechnung des Rabatts wird die Summe der Kosten herangezogen.
  *Technische Info: Toggle-Feld, DB-Feld: kaufrab.ekvkkz*
- **Wargrp.:**
  Kennzeichen der Warengruppe. Wenn Sie ein Kennzeichen angeben, wird der Rabatt auf die entsprechende Warengruppe eingeschränkt.
  *Technische Info: alphanumerisches Feld, DB-Feld: kaufrab.wagrp*
- **Pos.:**
  Rückverteilung des Rabatts auf die Positionen.
  - ☑ Der Rabatt wird auf die einzelnen Positionen rückverteilt.
  - ☐ Der Rabatt wird nicht rückverteilt.
  Die Rückverteilung ist ausführlich zum Register Detailansicht Rabatte beschrieben:
  ⇨ "Auftragserfassung – Detailansicht Rabatte" auf Seite D-1162
  *Technische Info: Checkbox, DB-Feld: kaufrab.verteil*
- **Verkauf:**
  Anzeige des Rabatts in der gewählten Zeile mit dem Typ Verkauf.
  *Technische Info: Anzeigefeld, DB-Feld: kauf.nettototal*
- **Kosten:**
  Anzeige des Rabatts in der gewählten Zeile mit dem Typ Kosten.
  *Technische Info: Anzeigefeld, DB-Feld: kauf.ektotal*

#### Feldbeschreibungen
**Spanne, WE** Anzeige der Gewinnspanne in Währungseinheit und Prozent.
*Technische Info: Anzeigefelder, DB-Felder: kauf.dbdm, kauf.dbvh*

**Skonto** Nummer der Skontogruppe. In der Skontogruppe sind die Zahlungsbedingungen hinterlegt, z. B. der Zeitraum, in dem Skonto gewährt wird und der Skontosatz. Wenn Sie eine Nummer angeben, werden die Zahlungsbedingungen im Klartext angezeigt.
*Technische Info: numerisches Feld, DB-Feld: kauf._skonto1*

**MwSt.** Mehrwertsteuersatz. Wenn mehrere Mehrwertsteuersätze für einen Auftrag angegeben sind, werden die einzelnen Mehrwertsteuersätze in Prozent und in der Währungseinheit angezeigt. Dies ist wichtig für Länder, bei denen unterschiedliche Steuersätze herangezogen werden. Die Felder werden nur angezeigt, wenn das Multi-Mehrwertsteuer-Modul aktiv ist.
*Technische Info: Anzeigefelder, DB-Felder: kauf.mwst, kauf.mwstbetrag, kauf.mwst1, kauf.mwstbetrag1, kauf.mwst2, kauf.mwstbetrag2, kauf.mwst3, kauf.mwstbetrag3, kauf.mwst4, kauf.mwstbetrag*

**Mindestwert** Auftragsmindestwert. Wenn der Nettototal-Wert des Auftrag kleiner ist als der Mindestwert, wird der Mindestwert als Nettototal-Wert herangezogen. Die Differenz wird als allgemeiner Aufschlag berechnet.
*Technische Info: numerisches Feld, DB-Feld: kauf._relimwert*

**Ausdruck** Auswahl für den Druck auf die kundenspezifischen Formulare.
- **unterdrücken:** Kein Druck von Rabatten und Nachlässen.
- **nur Rabatte:** Nur die Rabatte werden ausgewiesen und gedruckt.
- **nur Nachlass:** Nur die Nachlässe werden ausgewiesen und gedruckt.
- **Rabatt u. Nachlass:** Rabatte und Nachlässe werden ausgewiesen und gedruckt.
- **Mindestwert:** Der Mindestwert wird ausgewiesen und gedruckt. Wenn der Mindestwert als Nettototal-Wert herangezogen wird, wird diese Druckoption ausgewählt. Die Option kann nicht bearbeitet werden.
- **kostenlos:** Zurzeit nicht genutzt.
*Technische Info: Toggle-Feld, DB-Feld: kauf.gesrnkz*

**Materialko./Lohnkosten/Maschinenko.** Anzeige der Summe der Kosten aller Auftragspositionen.
*Technische Info: Anzeigefelder*

#### (Berechnung)
In diesem Bereich werden alle Rabatte und Zuschläge mit den anfallenden Preisen und Kosten summiert und der Auftragsbetrag berechnet. Im ersten Feld werden jeweils die verkaufsseitigen Werte angegeben und im zweiten Feld die kostenseitigen Werte.

**Rabattsumme** Anzeige der Summe der gewährten Rabatte und Zuschläge.
*Technische Info: Anzeigefelder, DB-Felder: kauf.gesrab*

**Allg. Abschlag** Fixer Betrag, der von der Auftragssumme abgezogen wird.
*Technische Info: numerische Felder, DB-Felder: kauf.gesrab, kauf.ekgesrab*

**Allg. Aufschlag** Fixer Betrag, der zur Auftragssumme hinzugefügt wird, z. B. wenn der Mindestauftragswert noch nicht erreicht ist oder bei Sonderzuschlägen.
*Technische Info: numerische Felder, DB-Felder: kauf.sonderrab, kauf.eksondarrab*

**Nettototal** Summe aller Positionspreise abzüglich der Rabatte und zuzüglich aller Zuschläge. Sie können den Betrag bearbeiten. Die Differenz wird im Feld **Allg. Abschlag** oder **Allg. Aufschlag** angezeigt.
*Technische Info: numerische Felder, DB-Felder: kauf.nettototal, kauf.ektotal*

**Skontierbar** Summe aus dem Nettobetrag und der Mehrwertsteuer, auf die Skonto gewährt wird. Der Betrag wird automatisch berechnet und kann nicht bearbeitet werden.
*Technische Info: numerisches Feld, DB-Feld: kauf.skontierbar*

**MwSt** Anzeige des Mehrwertsteuersatz in Prozent und als Betrag. Wenn mehrere Mehrwertsteuersätze für einen Auftrag hinterlegt sind, wird kein Prozentsatz angezeigt.
*Technische Info: Anzeigefelder, DB-Felder: kauf.mwstkz, kauf.mwstbetrag*

**Skonto** Anzeige des Skontosatzes und des Skontobetrags. Der Skontobetrag wird vom System berechnet.
*Technische Info: Anzeigefelder, DB-Felder: kauf.skvh1*

**Brutto** Anzeige des Brutto-Gesamtbetrags. Der Gesamtbetrag ist die Summe des Nettototalbetrags und der Mehrwertsteuer abzüglich des Skontobetrags.
*Technische Info: Anzeigefeld, DB-Feld: kauf.gesbrutto*

#### Fußbereich
Die Schaltflächen im Fußbereich sind zum Register Auftragserfassung – Kopf-, Fußbereich beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-1135

### Auftragserfassung – Detailansicht Rabatte
> Verkauf > Auftragserfassung > Auftragsfuß > Feld Rabatt, Nettototal > <F2> > <F5> > <F5>

*(Abb. D-41: Detailansicht Rabatte zeigt einen detaillierten Dialog für einen einzelnen Rabatt, mit Feldern für Name, Methode, Rabattwert, Rückverteilungsoptionen und Konfigurations-Checkboxen.)*

In diesem Dialog geben Sie Details zum ausgewählten Rabatt an. Wenn das System entsprechend konfiguriert ist, wird der Rabatt aus den Stammdaten herangezogen. Sie können die Einträge auftragsbezogen bearbeiten. Die Änderungen werden nicht in die Stammdaten übernommen.

Einige der Felder sind zum Dialog **Auftragserfassung (Summen)** beschrieben:
⇨ "Auftragserfassung - Summen" auf Seite D-1157

Zusätzlich werden folgende Felder angezeigt:

**Aktiviert** Angabe, ob der Rabatt berechnet werden soll.
- ☑ Der Rabatt wird berechnet.
- ☐ Der Rabatt wird nicht berücksichtigt.
*Technische Info: Checkbox, DB-Feld: kaufrab.geloescht*

#### Berechnung
**Sequenz** Sequenznummer. Das Feld entspricht der Spalte **Seqnr.** im Dialog **Auftragserfassung (Summen)**. Die Zuschläge und Rabatte werden in aufsteigender Reihenfolge der Sequenznummern berechnet.
*Technische Info: numerisches Feld, DB-Feld: kaufrab.seqnr*

**Minimalwert** Mindestwert des Rabatts. Wenn der Rabattwert kleiner ist als der Minimalwert, wird der Minimalwert zur Berechnung herangezogen.
*Technische Info: numerisches Feld, DB-Feld: kaufrab.minbetrag*

**Maximalwert** Höchstwert des Rabatts. Wenn der Rabattwert größer ist als der Maximalwert, wird der Maximalwert zur Berechnung herangezogen.
*Technische Info: numerisches Feld, DB-Feld: kaufrab.maxbetrag*

**Rabattwert** Wert des Rabatts und Rabattart. Die Felder entsprechen der Spalte **Rabattart** im Dialog **Auftragserfassung (Summen)**. Mit <F8> werden die Werte im Feld **Betrag (Basiswert)** berechnet.
*Technische Info: numerisches Feld, Toggle-Felder, DB-Felder: kaufrab.wert, kaufrab.satzart, kaufrab.rabtyp*

**Methode** Anzeige der Nummer der Rabattmethode, der der Rabattwert zugeordnet ist. Die Rabattmethode wird in den Stammdaten definiert und zugeordnet.
*Technische Info: Anzeigefeld, DB-Feld: kaufrab.methode*

**Betrag (Basiswert)** Anzeige des gesamten Rabatt-Betrags. Der Basiswert in den Klammern gibt an, auf welchen Grundbetrag der Rabatt berechnet wird. Die Felder sind abhängig von der gewählten Rabattart. Mit <F8> aktualisieren Sie die Anzeige, z. B., wenn Sie die Werte in den Feldern **Rabattwert** geändert haben.
*Technische Info: Anzeigefelder, DB-Felder: kaufrab.betrag, kaufrab.grundwert*

#### Rückverteilung
**Rückverteilen** Rückverteilung des Rabatts auf die Positionen. Das Feld entspricht der Checkbox in dem Feld **Pos.** im Dialog **Auftragserfassung (Summen)**.
- ☑ Der Rabatt wird auf die einzelnen Positionen rückverteilt und an die FIBU übermittelt. Die Felder **Stat. Warengruppe**, **Kostenstelle** und **Konto** werden gesperrt. Das Feld **Methode (Rückverteilung)** wird freigeschaltet, wenn **WE** als Rabattart im Feld **Rabattwert** gewählt ist.
- ☐ Der Rabatt wird nicht rückverteilt.
*Technische Info: Checkbox, DB-Feld: kaufrab.verteil*

**Methode (Rückverteilung)** Die Methode zur Rückverteilung gibt an, wie der Rabatt auf die Positionen rückverteilt wird. Das Feld ist nur freigeschaltet, wenn die Rückverteilung des Rabatts aktiv ist und **WE** als Rabattart im Feld **Rabattwert** gewählt ist:
- **nach % Wert:** Der Rabatt wird prozentual nach dem Positionspreis rückverteilt.
- **nach kg:** Der Rabatt wird nach Gewicht der Positionen rückverteilt.

Wenn im Feld **Rabattwert** nicht **WE** als Rabattart gewählt ist, wird der Rabatt immer auf die Positionspreise rückverteilt.
*Technische Info: Toggle-Feld, DB-Feld: kaufrab.verteil*

Die folgenden drei Felder sind nur freigeschaltet, wenn die Rückverteilung des Rabatts nicht aktiv ist:

**Stat. Warengruppe** Kennzeichen der statistischen Warengruppe. Die Warengruppe muss für Statistik-Buchungen angegeben werden.
*Technische Info: Pflichtfeld, alphanumerisches Feld, DB-Feld: kaufrab.statwagrp*

**Kostenstelle** Kennzeichen der Kostenstelle. Auf die angegebene Kostenstelle wird der Rabatt gebucht.
*Technische Info: Pflichtfeld, alphanumerisches Feld, DB-Feld: kaufrab.kstelle*

**Konto** Bezeichnung des Buchungskontos der Rabatt-Kostenstelle. Die Kontonummer hinterlegen Sie in den Stammdaten.
*Technische Info: alphanumerisches Feld, DB-Feld: kaufrab.konto*

#### Konfiguration
**Rabattierbar** Angabe, ob auf den Rabatt oder Zuschlag ein weiterer Rabatt berechnet werden kann.
- ☑ Der Rabatt oder Zuschlag ist rabattierbar.
- ☐ Der Rabatt oder Zuschlag ist von einem weiteren Rabatt ausgeschlossen.
*Technische Info: Checkbox, DB-Feld: kaufrab.rabattierbar*

**Skontierbar** Angabe, ob auf den Rabatt oder Zuschlag Skonto berechnet werden kann.
- ☑ Der Rabatt oder Zuschlag ist skontierbar.
- ☐ Der Rabatt oder Zuschlag ist vom Skonto ausgeschlossen.
*Technische Info: Checkbox, DB-Feld: kaufrab.skonto*

**Nullposition** Angabe, ob Positionen mit einem Positionsbetrag von 0 bei der Rabattierung berücksichtigt werden. Die Checkbox wird bei Positionen mit der Rabattart **WE** oder **WE/km** nicht berücksichtigt.
- ☑ Die Nullpositionen werden in die Rabattierung einbezogen. Der Rabatt wird auf alle Positionen rückverteilt.
- ☐ Die Nullpositionen werden von der Rabattierung ausgeschlossen. Der Rabatt wird nur auf Positionen mit einem Preis > 0 rückverteilt.
*Technische Info: Checkbox, DB-Feld: kaufrab.nullpositionen*

**Lieferzuschlag** Angabe, ob ein Lieferzuschlag berechnet wird.
- ☑ Der Lieferzuschlag wird pro Tag und pro Lieferadresse berechnet.
- ☐ Der Lieferzuschlag wird nicht berechnet.
*Technische Info: Checkbox, DB-Feld: kaufrab.lieferzuschlag*

**Verglasung** Angabe, ob sich der Rabatt auf Verglasungsarbeiten bezieht. Das Feld ist nur freigeschaltet, wenn im Feld **Rabattwert** die Rabattart **%** gewählt ist.
- ☑ Der Rabatt wird nur auf den Verglasungsartikel gewährt.
- ☐ Der Rabatt wird auf den gesamten Glaspreis gewährt.
*Technische Info: Checkbox, DB-Feld: kaufrab.verglkz*

**SP-Aufruf - Position** Angabe, ob die Rabatte über die Stored Procedure berechnet werden sollen. Die Stored Procedure kann kundenspezifisch in das System konfiguriert werden. Für weitere Informationen zu der Stored Procedure kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.
- ☑ Der Stored Procedure-Aufruf der Rabatte pro Position ist aktiv.
- ☐ Der Stored Procedure-Aufruf der Rabatte pro Position ist nicht aktiv.
*Technische Info: Checkbox, DB-Feld: kaufrab.spaufrufkz*

**SP-Aufruf - Vorgang** Angabe, ob die Rabatte pro Vorgang über die Stored Procedure aufgerufen werden sollen.
- ☑ Der Stored Procedure-Aufruf der Rabatte pro Vorgang ist aktiv.
- ☐ Der Stored Procedure-Aufruf der Rabatte pro Vorgang ist nicht aktiv.
*Technische Info: Checkbox, DB-Feld: kaufrab.spaufrufkzkauf*

**Min. bei Nullbetrag** Angabe, ob bei einem Nullbetrag des Rabattwerts der Minimalwert des Rabatts berechnet wird.
- ☑ Der Minimalwert wird bei Nullbetrag herangezogen.
- ☐ Der Minimalwert wird bei Nullbetrag nicht berücksichtigt.
*Technische Info: Checkbox, DB-Feld: kaufrab.minbeinullbetragkz*

**In Gutschrift** Angabe, ob der Rabatt bei einer Gutschrift berechnet wird.
- **Ja:** Der Rabatt wird in Gutschriften miteinbezogen.
- **Nein:** Der Rabatt gilt nicht für Gutschriften.
- **Frage:** Bei der Erstellung der Gutschrift, wird eine Abfrage angezeigt, ob der Rabatt in die Gutschrift miteinbezogen werden soll.
*Technische Info: Toggle-Feld, DB-Feld: kaufrab.gutschrift*

**Glasgewicht** Angabe, auf welches Glasgewicht sich der Rabatt bezieht. Das Feld ist nur freigeschaltet, wenn als Rabattart **WE/kg** oder als Methode der Rückverteilung **nach kg** gewählt ist.
- **Posgew.:** Der Rabatt gilt für das Gewicht der Position.
- **Nur Glasgew.:** Der Rabatt gilt nur für das Gewicht des Glases.
- **Glasgew.:** Der Rabatt gilt für das Gewicht des Glases. Wenn das Glasgewicht den Wert 0 besitzt, wird das Positionsgewicht zur Rabattberechnung herangezogen.
- **Fak. Posgew.:** Der Rabatt gilt für das fakturierte Positionsgewicht.
- **Nur fak. GGew.:** Der Rabatt gilt nur für das fakturierte Glasgewicht.
- **Fak. Glasgew.:** Der Rabatt gilt für das fakturierte Glasgewicht. Wenn das fakturierte Glasgewicht den Wert 0 besitzt, wird das fakturierte Positionsgewicht zur Rabattberechnung herangezogen.
*Technische Info: Toggle-Feld, DB-Feld: kaufrab.glasgewicht*

**Mehrwertsteuer** Nummer des Mehrwertsteuersatzes, der auf den Rabatt berechnet wird. Sie können dem Rabatt einen oder mehrere Steuersätze zuweisen.
- Mit <F9> öffnen Sie die Liste der Mehrwertsteuersätze.
- Mit den Pfeiltasten navigieren Sie zwischen den Steuersätzen.
- Mit <Toggle> markieren Sie einen Mehrwertsteuersatz.
- Mit <Ende> schließen Sie den Dialog und übernehmen die Auswahl.
*Technische Info: Auswahl-Feld, DB-Feld: kaufrab.verteil*

**openTRANS - Id** Identifikationsnummer bei interner Verrechnung zwischen den einzelnen Häusern, z. B. für nachträgliche Rabatte.
*Technische Info: alphanumerisches Feld, DB-Feld: kaufrab.otrabattid*

#### Abschlagsrechnungen
**Artikel** Artikelnummer der Abschlagsrechnung aus dem Zahlungsplan. Das Feld wird automatisch vorbelegt, wenn ein Zahlungsplan aktiv ist.
*Technische Info: numerisches Feld, DB-Feld: kaufrab.artnr*

**Rechnungsnummer** Rechnungsnummer der Abschlagsrechnung aus dem Zahlungsplan. Das Feld wird automatisch vorbelegt, wenn ein Zahlungsplan aktiv ist.
*Technische Info: Anzeigefeld, DB-Feld: kaufrab.rechnr*

## Auftragspositionen
> Verkauf > Auftragserfassung > Register Positionen

Im Bereich Positionen finden Sie folgende Register:
- "Auftragspositionen - Allgemein" auf Seite D-1167
- "Auftragspositionen – Eigensch." auf Seite D-1180
- "Auftragspositionen - Preise" auf Seite D-1185
- "Auftragspositionen – Status" auf Seite D-1188
- "Auftragspositionen – Kosten" auf Seite D-1190

Im Bereich Positionen stellen Sie Kundenprodukte zusammen, bestimmen den Produktaufbau und legen die Mengen fest.

### Auftragspositionen – Allgemein
> Verkauf > Auftragserfassung > Register Positionen > Register Allgemein

*(Abb. D-42: Auftragspositionen – Allgemein zeigt die Hauptansicht der Positionsliste mit Spalten wie Pos, Ku.Pos, Artikel, Menge, Breite, Höhe, B.Art, etc. Links neben den Positionen sind Status-Icons zu sehen.)*

In diesem Register erfassen und bearbeiten Sie die Positionen eines Auftrags. Sie können die Artikel auswählen, die Maße, Menge und Beschaffungsart bestimmen und den Artikeln Bearbeitungen zuordnen.

Bei bereits erfassten Aufträgen wird auf Höhe des Registers der Positionsstatus der markierten Position angezeigt, z. B. **Ausgeliefert Lokal – Korrektur**. Vor dem Feld **Pos** werden das Symbol des Positionsstatus und ggf. das Positionskennzeichen angezeigt.
⇨ "Symbolerklärung" auf Seite D-1128

In der Regel erfassen Sie Auftragsposition im dem Register Allgemein. In den anderen Registern im Bereich **Positionen** können Sie weitere Informationen zu den Positionseigenschaften und Preisen einsehen.

Der Artikelaufbau einer Position geht aus der Stücklistenbeschreibung hervor und wird aus dem Artikelstamm in den Vorgang kopiert. Sie können die Stückliste den Kundenwünschen entsprechend anpassen.
⇨ "Stücklistendarstellung" auf Seite D-1252
- Mit <Enter> wechseln Sie in das nächste Feld, mit <Bild hoch> wechseln Sie zur ersten Position, mit <Bild runter> zur letzten Position.
- Mit <Ende> wechseln Sie in den Fußbereich und schließen die Auftragserfassung ab.

#### Kopfbereich
Die Felder im Kopfbereich sind zum Register **Auftragserfassung – Kopf-, Fußbereich** beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-1135

#### Register Positionen (linker Bereich)
Im Infobereich werden verschiedene Informationen zur markierten Position angezeigt. Die technischen Werte können bearbeitet werden.
⇨ "Register Positionen (Info-Bereich - Grafik, Technische Werte)" auf Seite D-1170

*(Abb. D-43: Register Positionen (Infobereich links – Beispiel technische Werte) zeigt eine Detailansicht der markierten Position mit Kommissionstext und einer Aufschlüsselung des Artikelaufbaus, z.B. Kopfartikel und zugeordnete Bearbeitungen.)*

In diesem Bereich werden Informationen zur markierten Position angezeigt. Die Information zu dem Kopfartikel wird immer angezeigt. Alle anderen Informationen werden nur angezeigt, wenn sie vorhanden sind. Ist keine Information vorhanden bleibt die entsprechende Stelle leer.

- Mit <F2> wechseln Sie zu den Registern **Anschriften**, **Eigenschaften** oder **Verschiedenes**.
  - ⇨ "Auftragserfassung - Anschriften" auf Seite D-1143
  - ⇨ "Auftragserfassung - Eigenschaften" auf Seite D-1146
  - ⇨ "Auftragserfassung - Verschiedenes" auf Seite D-1152
- Mit <Enter> wechseln Sie in das Register **Allgemein**, das sich im Register **Positionen** befindet.
  - ⇨ "Auftragspositionen - Allgemein" auf Seite D-1167

**Kommis** Kommissionstext für den Druck. Der Text kann über die angezeigte Etikettenlänge hinausgehen. Wenn Sie eine neue Position erfassen, wird automatisch der Kommissionstext der vorangehenden Position übernommen.
Sie können für jede Position auch einen eigenen Kommissionstext eingeben, z. B. um in einem Auftrag für zwei Baustellen die Positionen über den Kommissionstext zuzuordnen.
- Mit <F4> > Kommissionen > neue Kommission oder Kommission ändern legen Sie über das Zusatzmenü einen neuen Kommissionstext an oder bearbeiten einen bestehenden Kommissionstext für den gesamten Auftrag.
- Mit <Shift> + <F11> wechseln Sie aus der Positionsebene in die Texterfassung der Kommission, um einen Kommissionstext für die ausgewählte Position anzulegen.
*Technische Info: alphanumerisches Feld, DB-Feld: komm.kommtxt*

> **Kommissionstext vererben**
> Wenn Sie einer Position mit <Shift> + <F11> einen Kommissionstext zuordnen, kann der Kommissionstext für alle folgenden Auftragspositionen übernommen werden. Dazu müssen Sie die Abfrage, ob die Kommission nach unten vererbt werden soll, mit [Ja] bestätigen. Wenn Sie [Nein] klicken, wird der Kommissionstext nur für die aktuelle Position übernommen. Die Abfrage wird nur angezeigt, wenn nach der aktuellen Position weitere Auftragspositionen erfasst sind.

**LE:** Leistungserklärung. Bezeichnung der Leistungserklärung, die dem Artikel zugeordnet ist. Das Feld wird nur angezeigt, wenn dem aktuellen Artikel eine Leistungserklärung zugeordnet ist.
*Technische Info: Anzeigefeld, DB-Feld: kposp.lbrefnr*

**(CAD-Kennzeichen)** Kennzeichen, ob der Position eine CAD-Datei zugeordnet ist. Wenn eine CAD-Datei angehängt ist, wird das Kennzeichen CAD angezeigt. Bei S/N-Positionen wird der S/N-Code in Klammern hinter dem CAD-Kennzeichen angezeigt.
*Technische Info: Anzeigefeld*

**(Kostenstelle)** Bezeichnung der Kostenstelle, die der Position zugeordnet ist. Wenn der Position keine Kostenstelle zugeordnet ist, wird die marktpartnerspezifische Ksotenstelle herangezogen. Wenn dem Marktpartner auch keine Kostenstelle zugeordnet ist, wird die Hauptkostenstelle herangezogen.
*Technische Info: Anzeigefeld, DB-Feld: kpos.kostenst*

**(Sprossenkennzeichen)** Kennzeichen, ob in der Position Sprossen erfasst sind.
- **S:** In der Position sind Sprossen erfasst. Der Sprossenaufbau wurde nicht bearbeitet.
- **E:** In der Position sind Sprossen erfasst. Der Sprossenaufbau wurde im Editor bearbeitet.
- **(Kein Kennzeichen):** In der Position sind keine Sprossen erfasst.
*Technische Info: Anzeigefeld*

**(Kopfartikel, Artikel)** Bezeichnung des Kopfartikels. Bei Mehrfachgläsern werden neben dem Kopfartikel die Bezeichnungen der einzelnen Gläser angezeigt.
*Technische Info: Anzeigefelder, DB-Feld: aufstrukt.artbez1*

**(Austausch-, Zusatzartikel, Anzahl1/Anzahl2)** Bezeichnung der Austausch- und Zusatzartikel und Anzahl der Artikel in der Stückliste. Austauschartikel werden mit einem A, Zusatzartikel mit einem Z vor der Bezeichnung angezeigt. Hinter der Artikelbezeichnung wird angezeigt, wie oft für den Artikel der Wert Breite und wie oft der Wert Höhe berechnet werden muss.
*Technische Info: Anzeigefelder, DB-Felder: aufstrukt.artbez1, aufstrukt.anzahl1, aufstrukt.anzahl2*

**(Sprossenaustausch-, Sprossenzusatzartikel, Anzahl1/Anzahl2)** Bezeichnung der Sprossenaustausch- und/oder Sprossenzusatzartikel und Anzahl der Sprossen in der Stückliste. Sprossenaustauschartikel werden mit einem A, Sprossenzusatzartikel mit einem Z vor der Bezeichnung angezeigt. Hinter der Sprossenbezeichnung wird die Anzahl der waagerechten und/oder senkrechten Sprossen angezeigt.
*Technische Info: Anzeigefelder, DB-Felder: aufstrukt.artbez1, aufstrukt.anzahl1, aufstrukt.anzahl2*

#### Register Positionen (Info-Bereich – Grafik, Technische Werte)
Im rechten Bereich im Register Positionen werden, abhängig von der Systemkonfiguration und den Einstellungen, eine der folgenden Informationen angezeigt:
- Beschaffung, Warengruppe und Modell
- Technische Werte
- Verdeckte Maßangaben

*(Abb. D-44: Register Positionen (Info-Bereich) zeigt den rechten Infobereich. Oben ist eine schematische Darstellung des Produktaufbaus, darunter sind Felder für technische Werte wie Ug-Wert und Artikeldetails wie Ges-Stärke.)*

Rechts wird ein schematischer Aufbau des Produkts angezeigt. Wenn Sie in der Position ein Modell und/oder Sprossen erfasst haben, wird links neben dem schematischen Aufbau auch eine schematische Produktdarstellung angezeigt.
⇨ "Grafische Darstellung der Position" auf Seite D-1175

**(Beschaffungsart)** Bezeichnung der Beschaffungsart. Die Beschaffungsart wählen Sie im Feld **B.Art**. Für die Beschaffungsarten **Produktion**, **Lagerentnahme** oder **Mitlieferung** wird ein entsprechender Hinweis angezeigt. Bei einer **Bestellung** wird die Lieferantennummer angezeigt.
- Mit <Shift> + <F12> können Sie den Lieferanten und die Lieferzeit von Bestellungen bearbeiten. Wenn Sie einen Lieferanten für eine Position angeben, wird die Beschaffungsart der Position automatisch auf **Bestellung** festgelegt.
*Technische Info: Anzeigefeld, DB-Feld: kpos.beschaffart*

**Lieferant** Lieferantennummer. Das Feld wird angezeigt, wenn als Beschaffungsart der Position **Bestellung** ausgewählt ist. Wenn Sie eine Lieferantennummer angeben, wird der Name des Lieferanten in der folgenden Zeile im Klartext angezeigt.
- Mit <Shift> + <F12> können Sie den Lieferanten und die Lieferzeit von Bestellungen bearbeiten.
*Technische Info: Anzeigefeld, DB-Feld: kpos.liefnr*

**Lief.zeit** Dauer der Lieferung in Tagen. Das Feld ist nur verfügbar, wenn als Beschaffungsart der Position **Bestellung** gewählt ist. Die Lieferzeit wird aus den Stammdaten herangezogen.
- Mit <Shift> + <F12> können Sie den Lieferanten und die Lieferzeit von Bestellungen bearbeiten.
*Technische Info: Anzeigefeld, DB-Feld: mp.liefzeit*

**Warengrp** Warengruppennummer der Position. Artikel sind zur Produktgliederung und zur Auswertung in Verkaufsstatistiken in Warengruppen eingeteilt. Wenn Sie die Stückliste einer Position ändern, wird die Angabe der Warengruppe angepasst. Das Feld ist nur verfügbar, wenn als Beschaffungsart des Artikels **Lager** gewählt ist.
- Mit <Strg> + <F9> wechseln Sie aus der Positionsebene in das Eingabefeld der Warengruppe.
- Mit <F9> > <F8> öffnen Sie die Auswahlliste der Warengruppen. Alternativ können Sie eine Warengruppennummer angeben. Eine Korrektur der Warengruppe ist möglich, aber nur in Ausnahmefällen erforderlich.
*Technische Info: Anzeigefeld, DB-Feld: kpos.wgrp*

**Modell** Modellnummer.
- Mit <Strg> + <F12> wechseln Sie aus der Positionsebene in das Eingabefeld für die Modellnummer.
- Mit <F2> öffnen Sie den Modellkatalog.
- Mit <F9> öffnen Sie eine Auswahl an Modellbezeichnungen.
Alternativ können Sie die Modellnummer direkt im Feld angeben. Nach Angabe einer Modellnummer startet die Modellerfassung. Standardmäßig ist das System mit dem A+W Modellkatalog konfiguriert. Für die Konfiguration eines kundenindividuellen Modellkatalogs kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.
⇨ "Modell-Maßangaben" auf Seite D-1234
*Technische Info: Anzeigefeld, DB-Feld: kpos.modnr*

#### Technische Werte
- Mit <F4> > Produktangaben > Technische Werte können Sie im Zusatzmenü einen der folgenden Einträge auswählen:
  - **Technische Werte anzeigen:** Zeigt die technischen Werte der gewählten Position an. Wenn die Berechnung der technischen Werten über A+W SLT im System konfiguriert ist, dann öffnet sich das Register Berechnete technische Werte.
    ⇨ "Berechnete technische Werte" auf Seite D-1244
  - **Technische Werte ändern:** Wechselt in die Eingabefelder für die technischen Werte der gewählten Position. Sie können die Felder bearbeiten.
  - **Verdeckte Maßangaben anzeigen:** Zeigt die verdeckten Maßangaben der gewählten Position neben der grafischen Darstellung der Position an, z. B. das Abstandshalter-Abzugsmaß. Wenn Sie Verdeckte Maßangaben anzeigen im Menü auswählen, während diese angezeigt werden, dann werden sie wieder ausgeblendet.
  - **Verdeckte Maßangaben ändern:** Öffnet den Dialog Artikel-Maßangaben, in dem Sie die verschiedenen Maßangaben der Position bearbeiten können.
    ⇨ “Artikel-Maßangaben" auf Seite D-1205
Je nach ausgewählter Position werden unterschiedliche Parameter aufgelistet. Mit [OK] oder <Ende> speichern Sie die Änderungen und schließen den Dialog.

**Position** Positionsnummer der gewählten Position. Das Feld wird nur angezeigt, wenn Sie die technischen Werte ändern.
*Technische Info: Anzeigefeld, DB-Feld: kpos.posnr*

**Ug-WertDIN** Wärmedurchgangskoeffizient nach DIN-Norm. Zentrale Maßeinheit, um den Wärmeverlust eines Bauteils zu ermitteln. Die Maßeinheit ist W/m²K. Je kleiner der Ug-Wert, desto größer ist die Wärmedämmung.
*Technische Info: numerisches Feld, DB-Feld: ktechw.kwert*

**Ug-Wert** Wärmedurchgangskoeffizient.
*Technische Info: numerisches Feld, DB-Feld: ktechw.kbazwert*

**Transmiss.** Lichtdurchlässigkeit für den direkt durchgelassenen Strahlungsanteil. Die Bezugsgröße von 100% ist eine unverglaste Maueröffnung.
*Technische Info: numerisches Feld, DB-Feld: ktechw.trwert*

**g-Wert** Energiedurchlasskoeffizient (Gesamtdurchlassgrad). Die Größe setzt sich zusammen aus direkter Sonnenenergietransmission und sekundärer Wärmeabgabe nach innen, infolge langwelliger Strahlung und Konvektion.
*Technische Info: numerisches Feld, DB-Feld: ktechw.gwert*

**dB-Wert** Schalldämmungs-Wert der Position in Dezibel.
*Technische Info: numerisches Feld, DB-Feld: ktechw.dbwert*

Wenn Sie die technischen Werte bearbeiten, werden mit <F2> weitere Felder angezeigt:

**Artikelcode** Artikelnummer der gewählten Position. Das Feld wird nur angezeigt, wenn Sie die technischen Werte ändern.
*Technische Info: Anzeigefeld, DB-Feld: ktechw.artnrgen*

**Ges-Stärke** Glasstärke für den gesamten Artikel der Position. Die Glasstärke ist abhängig von der gewählten Fassadenzone und der Windlast. Der Eintrag erfolgt in Millimeter. Das Feld wird nur angezeigt, wenn Sie die technischen Werte ändern.
*Technische Info: numerisches Feld, DB-Feld: ktechw.dicke*

**Windlast** Windlast am Einbauort. Windlast (N/m²) ist der Druck, der durch direkte Windeinwirkung auf die äußere Oberfläche eines Gebäudes ausgeübt wird. Das System führt mit diesem Wert eine Plausibilitätsprüfung durch, um zu prüfen, ob die Dickengruppe der gewählten Gläser für die angegebene Windlast ausreichend ist. Das Feld wird nur angezeigt, wenn Sie die technischen Werte ändern.
*Technische Info: numerisches Feld, DB-Feld: ktechw.wlast*

**Bereich** Angabe der Fassadenzone, in der die Scheiben verbaut werden. Hohe Gebäude oder Gebäude, die an Randgebieten stehen, werden z. B. mit einer erhöhten Windlast belastet. Das Feld wird nur angezeigt, wenn Sie die technischen Werte ändern.
- **Rand:** Für Gebäude mit erhöhter Windlast.
- **zentral:** Für Gebäude ohne erhöhte Windlast.
*Technische Info: Toggle-Feld, DB-Feld: ktechw.bereich*

#### Verdeckte Maßangaben
- Mit <F4> > Produktangaben > Technische Werte können Sie im Zusatzmenü einen der folgenden Einträge auswählen:
  - **Verdeckte Maßangaben anzeigen:** Zeigt die verdeckten Maßangaben der gewählten Position neben der grafischen Darstellung der Position an, z. B. das Abstandshalter-Abzugsmaß.
    Wenn Sie **Verdeckte Maßangaben anzeigen** im Menü auswählen, während diese im rechten Bereich im Register **Positionen** angezeigt werden, dann werden sie wieder ausgeblendet.
  - **Verdeckte Maßangaben ändern:** Öffnet den Dialog **Artikel-Maßangaben**, in dem Sie die verschiedenen Maßangaben der Position bearbeiten können.

Je nach ausgewählter Position werden unterschiedliche Parameter aufgelistet. Mit [OK] oder <Ende> speichern Sie die Änderungen und schließen den Dialog.
Die Felder sind ausführlich zum Dialog **Artikel-Maßangaben** beschrieben.
⇨ "Artikel-Maßangaben" auf Seite D-1205

#### Grafische Darstellung der Position
Für die Position werden verschiedene Voransichten angezeigt:

*(Abb. D-45: Grafische Darstellungen des Produkts (Beispiele) zeigt verschiedene schematische Darstellungen: ein einfaches Modell, eine Sprossenkonstruktion, ein Modell mit Sprossen, ein Modell mit Stufen und ein ISO-Glas mit Stufe.)*

- **Schematische Produktdarstellung:**
  Zeigt schematisch das Modell, die Sprossenkonstruktion und die Stufe für die Position an. Die schematische Produktdarstellung wird nur angezeigt, wenn Sie in der Position ein Modell und/oder Sprossen erfasst haben.
- **Schematischer Aufbau:**
  Zeigt den Scheibenaufbau im Querschnitt an. Die Sonne markiert die Außenseite der Scheibe. Der schematische Aufbau der Position wird immer angezeigt.

#### Register Allgemein
Die Felder im Register Allgemein variieren je nach Artikel, den Sie wählen.

**Pos** Positionsnummer. Vor dem Feld **Pos** wird der Positionsstatus und ggf. das Positionskennzeichen der jeweiligen Position angezeigt. Der Positionsstatus wird erst nach Speichern des Vorgangs angezeigt. Der Status der Position wird von der Produktion, dem Lager und dem Versand gemeldet.
*Technische Info: numerisches Feld, DB-Feld: kpos.Ifdpos*

**Ku.Pos** Kunden-Positionsbezeichnung. Angabe der vorgegebenen Positionsbezeichnung aus der Positionsliste des Kunden. Das Feld ist nur freigeschaltet, wenn im Kopfbereich im Feld **Knd-Pos** der Eintrag **Pos.** ausgewählt ist.
Die Positionsbezeichnung kann auf allen kunden- und lieferantenseitigen Dokumenten ausgedruckt werden.
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-1135
Alternativ können Sie die Artikelbezeichnung eines festbemaßten Artikels angeben. Das System belegt die Felder mit den Artikeldaten vor.
⇨ "Artikelangaben für bemaßte Varianten" auf Seite D-1217
*Technische Info: numerisches Feld, DB-Feld: kpos.kuposnr*

**Typ** Glastyp der Position. Das Feld wird kundenspezifisch genutzt und kann frei konfiguriert werden.
Das Feld wird nur angezeigt, wenn im Kopfbereich im Feld **Knd-Pos** der Eintrag **Typ** ausgewählt ist.
*Technische Info: numerisches Feld, DB-Feld: kpos.kuposnr*

**Artikel** Artikelnummer. Sie können im Feld **Artikel** eine kunden- oder lieferantenindividuelle Artikelnummer angeben.
- Mit <F9> öffnen Sie die Artikel-Suche.
- Mit <F10> suchen Sie nach kundenindividuellen Artikeln.
  ⇨ "Artikelangaben für bemaßte Varianten" auf Seite D-1217
- Mit <Strg> + <L> öffnen Sie den Dialog Fremddaten-Import.
  ⇨ "Fremddaten-Import" auf Seite D-1222
- Mit Keyboard scannen Sie Artikelnummern per EAN Code ein. Keyboard Scanner muss so eingestellt werden, dass er als Prefix ein '-' sendet und als Suffix eine <ENTER>/oder <TAB> - Taste weitergibt. Wenn Sie weitere Fragen haben, wenden Sie sich an zuständigen A+W - Mitarbeiter.
*Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kpos.artnr*

> **Stücklistennummern zuordnen lassen**
> Mit der SLNr zählt das System die unterschiedlichen Stücklisten, die dem Auftrag hinzugefügt werden. Nicht die Menge an Stücklisten wird gezählt, sondern wie viele Stücklisten mit unterschiedlichem Aufbau vorliegen.
> Jede neue Position mit einem Stücklistenaufbau, der sich vom Stücklistenaufbau in den bereits erfassten Positionen unterscheidet, bekommt die nummerisch nächste SLNr zugeordnet. Wenn der gleiche Artikel in verschiedenen Positionen erfasst ist, dann haben diese Positionen die gleiche SLNr, da sich ihr Stücklistenaufbau nicht unterscheidet.
> Wenn Sie einen Artikel hinzufügen, der bereits in einer anderen Position erfasst ist, also eine identische Stückliste hat, können Sie diesem auch eine neue SLNr vom System zuordnen lassen:
> - Mit <Shift> + <F5> im Feld **Artikel** wird dem Artikel vom System die nächste freie Stücklistennummer zugeordnet.
> - Mit <F5> im Feld **Artikel** übernehmen Sie die originale Stückliste des Artikels. Die Stücklistennummer wird vom System zugewiesen.

**SLNr** Stücklistennummer des Artikels. Die Nummer wird standardmäßig vom System vergeben. Die Stückliste beinhaltet alle Teile und Bearbeitungen, die zur Herstellung des Artikels erforderlich sind. Die Stücklistennummer ist abhängig von der Stücklistenaufbau der jeweiligen Position. Positionen mit der gleichen Stückliste wird die gleiche Stücklistennummer zugewiesen. Die Nummer wird im Feld SLNr angezeigt. Wenn Sie den Stücklistenaufbau einer Position ändern, wird die Stücklistennummer ggf. vom System geändert.
Nachdem die Maße der Position festgelegt wurden, können Sie mit <F5> die Stückliste der Position anzeigen und bearbeiten.
⇨ "Bearbeitungen zu Position" auf Seite D-1276
*Technische Info: numerisches Feld, DB-Feld: kpos.poskonr*

**Lieferant** Nummer des Kistenlieferanten. Das Feld wird nur angezeigt, wenn Sie einen Kistenartikel gewählt haben.
*Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kposk.liliefnr*

**Menge** Menge der Position. Die Mengeneinheiten hängt davon ab, welcher Artikel erfasst wird, z. B. Stück, Quadratmeter. Bei Artikeln mit hinterlegten Maß-, Farb- oder Dickenvarianten öffnet sich nach Eingabe der Menge ein Dialog zur Auswahl der jeweiligen Variante.
⇨ "Varianten- und Farben-/Dickenauswahl" auf Seite D-1220
Wenn Sie einen Kistenartikel erfassen, können Sie keine Menge angeben. Das System berechnet die Menge und belegt das Feld, wenn Sie die Kisten- und Blattanzahl angegeben haben.
Mit <Strg> + <B> wird das Register **Eigenschaften** geöffnet und Sie können der gewählten Position eine CAD-Datei zuweisen.
⇨ "CAD Datei" auf Seite D-1183
*Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kpos.menge*

**Breite, Höhe** Breite und Höhe in Millimeter. Für Variantenartikel übernimmt das System die Maßangaben aus dem Artikelstamm. Wenn Sie die Lagermaße ändern, erscheint die Variantenabfrage: *Kann der Variantenbezug wirklich entfernt werden?*
- Klicken Sie auf [Nein], werden die eingegebenen Maße auf die Lagermaße zurückgesetzt.
- Klicken Sie auf [Ja], ändern Sie die Lagermaße. Das kann ggf. zu Problemen im Lager und bei der Preisberechnung führen.
*Technische Info: Pflichtfelder, numerische Felder, DB-Felder: kpos.laenge, kpos.breite*

**(Feld ohne Bezeichnung)** Bei Längen-, Zeit- und Stückartikeln wird anstelle von Breite, Höhe und SZR die Maßangabe und die entsprechende Maßeinheit angezeigt, die dem gewählten Artikel zugeordnet ist. Die Maßeinheit des Artikels wird aus den Stammdaten herangezogen und kann nicht bearbeitet werden. Bei Montagearbeiten wird z. B. die Maßeinheit **std** (Stunden) angezeigt, bei Gasfüllungen **l** (Liter) und bei Klebeband **m** (Meter). Die Maßangabe können Sie frei wählen.
*Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kpos.me*

**SZR** Scheibenzwischenraum in Millimeter.
*Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kpos.szr*

> **Stückliste der Position aufrufen**
> Mit <F3> oder <F5> öffnen Sie die Stückliste zu der gewählten Position. Sie können die Stückliste einer Position erst nach Angabe der Maße öffnen. Wenn Sie vorher versuchen, die Stückliste zu öffnen, merkt sich das System diese Aktion und öffnet die Stückliste automatisch nach Angabe der Maße. Neben der Position wird eine graue Checkbox angezeigt. Zusätzlich wird eine Meldung mit dieser Information angezeigt.

**KA** Kistenanzahl. Die Menge wird vom System aus **Kistenanzahl x Blattzahl** berechnet. Das Feld wird nur angezeigt, wenn Sie einen Kistenartikel gewählt haben und das System entsprechend konfiguriert ist.
*Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kposk.kianz*

**Blatt** Anzahl der Glasblätter pro Kiste. Die Menge wird vom System aus **Kistenanzahl x Blattzahl** berechnet. Das Feld wird nur angezeigt, wenn Sie einen Kistenartikel gewählt haben und das System entsprechend konfiguriert ist.
*Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kposk.blattanz*

**VA** Kennzeichen der Verpackungsart, z. B. 12 = Kistenverpackung. Das Feld wird nur angezeigt, wenn Sie einen Kistenartikel gewählt haben.
*Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: kpos.verpackart*

**Kammer-Dicke** Dicke der Gel-Schicht im Scheibenzwischenraum bei Brandschutzgläsern. Das Feld wird nur angezeigt, wenn Sie einen Brandschutzartikel gewählt haben, die Information in den Stammdaten hinterlegt ist und das System entsprechend konfiguriert ist.
*Technische Info: numerisches Feld, DB-Feld: kpos.szr*

**SN** Anzeige, ob der Position eine SN-Datei für den A+W CAD Designer (Shapes) zugeordnet ist. In der SN-Datei werden z. B. alle Bearbeitungen definiert, die im Produktionsvorgang von der Maschine vollautomatisch durchgeführt werden. Im Register **Eigensch.** im Feld **CAD-Datei** können Sie die zugewiesene Dateien ansehen oder eine Datei manuell zuweisen.
- ☑ Der Position ist eine SN-Datei zugewiesen.
- ☐ Der Position ist keine SN-Datei zugewiesen.
*Technische Info: Checkbox, Anzeigefeld, DB-Feld: kpos.brokefile*

**Prov** Provision bei aktiver Vertreter-Provisionsberechnung. Sie können den gewährten Provisionsschlüssel für jede Position einzeln angeben. Bei nicht aktiver oder spannenorientierter Provisionsberechnung ist das Feld gesperrt und wird nicht berücksichtigt.
*Technische Info: numerisches Feld, DB-Feld: kpos.provnr*

**B.Art** Die Beschaffungsart bestimmt, wie ein Artikel beschafft wird. Standardmäßig werden die Beschaffungsarten vom System aus den Artikelstammdaten übernommen. Die Beschaffungsart, die dem Artikel in den Stammdaten als Priorität 1 zugeordnet ist, wird in der Vorgangserfassung im Feld **B.Art** vorbelegt. Sie können das Feld auftragsbezogen bearbeiten.
- **Produktion:** Der Artikel wird produziert.
- **Mitgelief.:** Der Artikel wird vom Kunden mitgeliefert, z. B. zur weiteren Bearbeitung.
- **n. verfüg.:** Der Artikel ist nicht verfügbar.
- **Keine:** Keine Beschaffungsart, z. B. für Dienstleistungen.
- **Bestellung:** Der Artikel wird beim Lieferanten bestellt.
- **Lager:** Der Artikel wird dem Lager entnommen.
*Technische Info: Toggle-Feld, DB-Feld: kpos.beschaffart*

**kg/St, ME/St** Gewicht in Kilogramm pro Stück, Mengeneinheit in Quadratmetern pro Stück.
Wenn Sie ins Preisfeld wechseln, können Sie die Anzeige des Feldes **kg/St, ME/St** mit <Strg> + <M> umschalten.
*Technische Info: Anzeigefeld, DB-Feld: kpos.gewme*

**Preisfeld** Nettopreis der Position. Der Feldname variiert je nach Eigenwährung und Konfiguration, z. B. Preis/Stück, Preis/m2. Das System berechnet den Gesamtpreis der Position inklusive der Konditionen in der gewählten Währung. Die Währung bestimmen Sie im Feld **Währung/Kurs** im Register **Verschiedenes**.
- Mit <Shift> + <F11> wechseln Sie die Anzeige des Preisfeldes.
- Mit <Shift> + <F8> markieren Sie die Position als festbemaßtes Produkt. Wenn Sie den Auftrag speichern wird die Position als festbemaßtes Produkt in den Stammdaten hinterlegt.
  ⇨ "Artikelangaben für bemaßte Varianten" auf Seite D-1217
- Mit <Strg> + <F9> wird der VK-Preis mit den Positionskonditionen ermittelt und der Preis neu berechnet.
- Mit <Shift> + <F9> öffnen Sie den Dialog Positionskonditionen.
  ⇨ "Positionskonditionen" auf Seite D-1340
- Mit <Shift> + <F10> wird der Positionspreis neu berechnet.
- Mit <F3> wird eine Übersicht der Maße der einzelnen Positionen angezeigt.
  ⇨ "Maße der einzelnen Stücklistenteile" auf Seite D-1277
- Mit <Strg> + <M> wechseln Sie die Anzeige des Feldes kg/St, ME/St.
*Technische Info: numerisches Feld, DB-Feld: kpos.nstpreis*

Mit <F4> > Preisangaben > Preiskontrolle zeigen Sie weitere Felder im Register an:

**aVK** Vorab-Verkaufs-Preiskennzeichen aus dem übertragenen Haus.
*Technische Info: Anzeigefeld, DB-Feld: kpos.vorvkpkz*

**PKZ** Vorab-Preiskennzeichen aus dem übertragenen Haus.
*Technische Info: Anzeigefeld, DB-Feld: kpos.vorpkz*

**nVK** Neu ermitteltes Verkaufs-Preiskennzeichen.
*Technische Info: Anzeigefeld, DB-Feld: kpos.neuvkpkz*

**aVF** Vorab-Verkaufs-Faktor aus dem übertragenen Haus.
*Technische Info: Anzeigefeld, DB-Feld: kpos.vorvkfaktor*

**Faktor** Vorab-Faktor in Prozent aus dem übertragenen Haus.
*Technische Info: Anzeigefeld, DB-Feld: kpos.vorfaktor*

**nVF** Neu ermittelter Verkaufs-Faktor.
*Technische Info: Anzeigefeld, DB-Feld: kpos.neuvkfaktor*

**aVK-Pr.** Vorab-Verkaufs-Preis aus dem übertragenen Haus.
*Technische Info: Anzeigefeld, DB-Feld: kpos.vorpreis*

**nVK-Pr.** Neu ermittelter Verkaufs-Preis.
*Technische Info: Anzeigefeld, DB-Feld: kpos.neuvknstpreis*

#### Fußbereich
Die Felder und Schaltflächen im Fußbereich sind zum Register **Auftragserfassung – Kopf-, Fußbereich** beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-1135

Zusätzlich werden folgende Schaltflächen angezeigt:

**[Pos. Kopieren]** Kopiert die aktuelle Position und fügt sie hinter der letzten Position ein. Sie können die Parameter der kopierten Position bearbeiten, z. B. Menge und Maßangaben.

**[Stückliste]** Öffnet den Dialog **Stücklistendarstellung** zur aktuellen Position. Alternativ können Sie den Dialog mit <F5> öffnen.
⇨ "Register Akt. Stücklistenebene" auf Seite D-1259

### Auftragspositionen – Eigensch.
> Verkauf > Auftragserfassung > Register Positionen > Register Eigensch.

*(Abb. D-46: Auftragserfassung – Eigensch. zeigt den Eigenschaften-Tab für eine einzelne Position. Oben wird die Position und ihre Grafik angezeigt, darunter sind detaillierte Felder zu Gewicht, Maßen, Kostenstelle, CAD-Datei etc. aufgeführt.)*

In diesem Register können Sie weitere Eigenschaften der aktuellen Position einsehen und bearbeiten, z. B. Lagerzuordnung, Verpackart. Im oberen Bereich des Registers wird die gewählte Position angezeigt und im unteren Bereich die Eigenschaften dieser Position.

- Mit <Bild hoch> und <Bild runter> wechseln Sie zur vorherigen bzw. nächsten Position. Im unteren Bereich des Registers werden entsprechend die Eigenschaften der vorherigen bzw. nächsten Position angezeigt.
- Mit <F5> wechseln Sie von der aktuellen Position ins Feld **Bezeichnung**.

In der Regel müssen Sie die Angaben im Register **Eigensch.** nicht bearbeiten.
Wenn sich der Status ändert, wird auf Höhe des Registers ein entsprechender Hinweis zum Bearbeitungsstand der markierten Position angezeigt, z. B. **Ausgeliefert Lokal – Korrektur**. Vor dem Feld **Pos** werden der Positionsstatus und ggf. das Positionskennzeichen angezeigt.
⇨ "Symbolerklärung" auf Seite D-1128

#### Kopfbereich
Die Felder im Kopfbereich sind zum Register **Auftragserfassung – Kopf-, Fußbereich** beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-1135

#### Register Eigensch.
Die meisten Felder sind zum Register **Allgemein** beschrieben:
⇨ "Register Allgemein" auf Seite D-1175

Zusätzlich werden folgende Felder angezeigt:

**Bezeichnung** Bezeichnung des Kopfartikels. Sie können die Bezeichnung bearbeiten. Die Änderung wird nur auftragsbezogen übernommen.
*Technische Info: alphanumerisches Feld, DB-Feld: kpos.artbez1*

> **Änderungen der Bezeichnung**
> Die für diese Position geänderte Artikelbezeichnung wird auf allen auftragsbezogenen Dokumenten und in allen weiteren Dialogen dieses Vorgangs angezeigt.

**Kostenstelle** Bezeichnung der Kostenstelle, z. B. für statistische Auswertungen.
*Technische Info: alphanumerisches Feld, DB-Feld: kpos.kostenst*

**Lager** Nummer des Standardlagers für Lagerartikel. Wenn Sie eine Nummer auswählen, wird die Bezeichnung des Lagers im Klartext angezeigt. Wenn dem Artikel in den Stammdaten ein Standardlager zugewiesen ist, wird das Feld mit diesem Wert vorbelegt. Das Feld ist nur freigeschaltet, wenn dem Artikel in den Stammdaten als Beschaffungsart-Priorität 1 oder 2 Lager zugewiesen ist.
*Technische Info: numerisches Feld, DB-Feld: kpos.Inr*

**Stapel** Nummer des Stapellagers für Lagerartikel. Wenn Sie eine Nummer auswählen, wird die Bezeichnung des Lagers im Klartext angezeigt. Wenn dem Artikel in den Stammdaten ein Stapellager zugewiesen ist, wird das Feld mit diesem Wert vorbelegt. Das Feld ist nur freigeschaltet, wenn dem Artikel in den Stammdaten als Beschaffungsart-Priorität 1 oder 2 Lager zugewiesen ist und als Standardlager das Stapellager ausgewählt ist.
*Technische Info: numerisches Feld, DB-Feld: kpos.sfill1*

**Produktset** Anzeige der Bezeichnung, der Nummer des Produktsets und der Positionsnummer des Artikels im Produktset. Die Felder sind nur vorbelegt, wenn Sie eine Position mit Produktset auswählen.
*Technische Info: alphanumerisches Feld, numerische Felder, DB-Felder: kposex.sashcode, kposex.prodset, kposex.posnr*

**kg/ME, kg/Stück, kg/Pos, kg/Glas** Gewicht der Position. Die Angaben können in den folgenden Feldern dargestellt werden:
- **kg/ME:** Kilogramm pro Mengeneinheit
- **kg/Stück:** Kilogramm pro Stück
- **kg/Pos.:** Kilogramm pro Position
- **kg/Glas:** Kilogramm pro Glas
Nur das Feld ist freigeschaltet, dessen Gewichtsangabe in den Stammdaten des aktuellen Artikels zugeordnet ist.
*Technische Info: numerische Felder, DB-Felder: kpos.gewme, kpos.gewst, kpos.gewicht, kpos.glasgew*

**Physik ME/St** Physikalische Menge in Mengeneinheit pro Stück.
*Technische Info: numerisches Feld, DB-Feld: kpos.phymestk*

**Berech ME/St** Berechnete Menge in Mengeneinheit pro Stück.
*Technische Info: numerisches Feld, DB-Feld: kpos.qm*

**ME/Pos.** Gesamtmenge in der Mengeneinheit pro Position. Der Wert ergibt sich aus berechneter Mengeneinheit pro Stück x Positionsmenge. Für Flächenartikel gilt z. B. ME/Pos = Gesamtfläche der Position x Positionsmenge, für Stückartikel gilt ME/Pos = Geamtstückzahl der Position.
*Technische Info: numerisches Feld, DB-Feld: kpos.geslief*

**Bonus** Nummer des Bonusverfahrens. Wenn Sie eine Nummer auswählen, wird der Prozentsatz des positionsbezogenen Preisnachlasses im Klartext angezeigt.
*Technische Info: numerisches Feld, DB-Feld: kpos.bonusnr*

**CAD Datei** Name der CAD-Datei, die der Position angehängt ist.
- Mit <Strg> + <F> öffnen Sie die Technische Auftragserfassung (TOE). Dafür können Sie CAD-Dateien im A+W CAD Designer (Shapes) erfassen und bearbeiten.
  ⇨ Help Cards, "Position in CAD erfassen" auf Seite D-22
- Mit <F9> öffnen Sie einen Dialog zur Auswahl der Dateiart:
  - **SN:** Im Explorer werden alle SN-Dateien zur Auswahl angezeigt.
    ⇨ Help Cards, "SN-Datei anhängen" auf Seite D-20
  - **DXF:** Im Explorer werden alle DXF-Dateien zur Auswahl angezeigt. Wenn Sie eine Datei auswählen, öffnet sich der Dialog DXF Import.
    ⇨ "DXF Import" auf Seite D-1229
- Mit <Strg> + <F9> löschen Sie die CAD-Datei, die der Position angehängt ist.
*Technische Info: Auswahl-Feld, DB-Feld: kpos.brokefile*

> **Sonder- oder Leerzeichen im Dateinamen**
> Sonder- oder Leerzeichen für den CAD-Dateinamen dürfen nicht verwenden werden.

**Knd-Artnr** Anzeige der Kundenartikelnummer der Position. Der gewählte Artikel muss dem Kunden in den Marktpartnerstammdaten zugeordnet sein.
*Technische Info: numerisches Feld, DB-Feld: kpos.kuposnr*

**Bezeichnung** Anzeige der Kundenartikel-Bezeichnung.
*Technische Info: alphanumerisches Feld*

**LE-Nummer** Nummer der Leistungserklärung. Eine Leistungserklärung kann einem Artikel nur zugeordnet werden, wenn in den Stammdaten des entsprechenden Artikels die Checkbox Leistungserklärung aktiv ist.
Wenn dem gewählten Artikel in den Stammdaten bereits eine Leistungserklärung zugeordnet ist, wird das Feld mit dieser LE-Nummer vorbelegt.
Mit <Strg> + <T> öffnen Sie das Register **Berechnete technische Werte**, in dem Sie eine neue Leistungserklärung erfassen können. Eine Leistungserklärung kann nur erfasst werden, wenn das System entsprechend konfiguriert ist.
⇨ "Berechnete technische Werte" auf Seite D-1244
*Technische Info: alphanumerisches Feld, DB-Feld: kposp.lenr*

**CE Kennz** CE-Kennzeichen. Sie können ein CE-Kennzeichen nur vergeben, wenn das System entsprechend konfiguriert ist.
*Technische Info: alphanumerisches Feld, DB-Feld: kpos.cekz*

**Skizzendruck** Art des Skizzendrucks, z. B. SNLive. Sie können die Einstellungen für den Print Service festlegen. Beim Formulardruck mit Crystal Reports können neben den Positionsangaben auch verschiedene Skizzen gedruckt werden:
- **SNLive:** Skizze des Produktaufbaus inklusive Bearbeitungen aus der Stückliste
- **AWBom:** Skizze des Stücklistenaufbaus
- **AWDesign:** Skizze des Sprossenaufbaus
- **Prinzip:** Prinzip-Skizze
Sie können keine, eine oder mehrere Skizzenarten für den Druck auswählen.
- Mit <F9> öffnen Sie die Liste der Skizzenarten.
- Mit den Pfeiltasten navigieren Sie zwischen den Skizzenarten.
- Mit <Toggle> markieren Sie eine Skizzenart. Markierte Skizzen werden hellblau hervorgehoben.
- Mit <Ende> schließen Sie den Dialog und übernehmen die Auswahl.
*Technische Info: Auswahl-Feld, DB-Feld: kpos.imagedrkz*

**Verpackart** Nummer der Verpackungsart, z. B. Kiste. Wenn Sie eine Nummer auswählen, wird die Bezeichnung im Klartext angezeigt.
*Technische Info: numerisches Feld, DB-Feld: kpos.verpackart*

**Zustellung** Gewünschte Zustellart:
- **Abholung:** Der Kunde holt die Ware selbst ab.
- **Streckengeschäft:** Die Ware wird vom beauftragten Produktionsbetrieb direkt an den Endkunden ausgeliefert. Dabei wird automatisch eine Direktroute, ggf. auch mandantengenau, aus den Stammdaten ermittelt und herangezogen. Wenn mehrere Routen zur Verfügung stehen, haben Sie eine Auswahlmöglichkeit in dem darauf kommenden Dialog. Die Beschaffungsart der Auftragsposition muss in den Artikelstammdaten auf **Zukauf** gesetzt sein.
- **keine Auswahl:** Die Ware wird über die Route geliefert, die im Kopfbereich erfasst wurde.
*Technische Info: Toggle-Feld, DB-Feld: kpos.geschart*

**Konto** Bezeichnung des Buchungskontos der Kostenstelle.
*Technische Info: alphanumerisches Feld, DB-Feld: kposp.mankonto*

**Fertg-Folge** Reihenfolge der Fertigung, die pro Position der Produktion vorgesehen wird.
*Technische Info: numerisches Feld, DB-Feld: kpos.ferts*

**Ansicht** Richtung der Nummerierungsfolge im Positionsaufbau der Erfassungsansicht. Wichtig ist diese Angabe z. B. für den Positionsaufbau bei Gläsern mit Beschichtungen.
- **Außen:** Die Elemente sind von außen nach innen durchnummeriert.
- **Innen:** Die Elemente sind von innen nach außen durchnummeriert.
Das Feld wird zurzeit nicht genutzt.
⇨ "Produktdarstellung" auf Seite D-1254
*Technische Info: Toggle-Feld, DB-Feld: kposp.ansicht*

#### Fußbereich
Die Felder und Schaltflächen im Fußbereich sind zum Register **Auftragspositionen – Allgemein** beschrieben:
⇨ "Auftragspositionen - Allgemein" auf Seite D-1167

### Auftragspositionen – Preise
> Verkauf > Auftragserfassung > Register Positionen > Register Preise

*(Abb. D-47: Auftragserfassung – Preise zeigt den Preise-Tab für eine Position. Er ist in zwei Bereiche unterteilt: Der obere zeigt den Gesamtpreis der Position, der untere schlüsselt die Berechnung auf (ME-Preis, Stück-Brutto, Faktor, Stück-Netto, Kosten, Spanne etc.).)*

In diesem Register wird die Berechnung der Preise der aktuellen Position angezeigt. Die Preise werden zu jeder Position einzeln angezeigt.
- Mit <Bild hoch> und <Bild runter> wechseln Sie zur vorherigen bzw. nächsten Position.
- Mit <F5> wechseln Sie von der aktuellen Position ins Feld **Stück-Verglas**.

Wenn Sie die Preise der Position bearbeiten wollen, müssen Sie die Auftrags- und/oder Positionskonditionen bearbeiten.
⇨"Positionskonditionen" auf Seite D-1340

Wenn sich der Status ändert, wird auf Höhe des Registers ein entsprechender Hinweis zum Bearbeitungsstand der markierten Position angezeigt, z. B. **Ausgeliefert Lokal – Korrektur**. Vor dem Feld **Pos** werden der Positionsstatus und ggf. das Positionskennzeichen angezeigt.
⇨ "Symbolerklärung" auf Seite D-1128

#### Kopfbereich
Die Felder im Kopfbereich sind zum Register **Auftragserfassung – Kopf-, Fußbereich** beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-1135

#### Register Preise
Die Felder auf Positionsebene im Register **Preise** sind zum Register **Allgemein** beschrieben:
⇨ "Auftragspositionen - Allgemein" auf Seite D-1167

Bei einigen Feldern werden mehrere Preisen angegeben:
- **VK-Preis:** Netto-Verkaufspreis, der durch die Konditionen berechnet wird.
- **VK-druckbar:** Netto-Verkaufspreis, der auf den Papieren gedruckt wird.
- **Kosten:** Kostenanteil des Verkaufspreises.

Für jeden Preis wird eine eigene Spalte angezeigt. Bei den folgenden Feldern werden die Preise in den drei Spalten unterschieden:

Mit <F4> öffnen Sie das Zusatzmenü. Mit **Preisangaben > Auftragskonditionen** öffnen Sie den Dialog **Auftragskonditionen**, in dem Sie die auftragsbezogenen Konditionen zur Preisberechnung bearbeiten können, wie z. B. Preiskennzeichen, Faktor, Mindestberechnungsflächen und Bearbeitungszuschläge.
⇨ "Positionskonditionen" auf Seite D-1340

**ME-Preis** Anzeige des Preises pro Mengeneinheit. Der Preis wird aus dem Glaspreis zuzüglich des Teuerungszuschlags berechnet.
*Technische Info: Anzeigefelder, DB-Felder: kpos.bmepreis, kpos.drbmepreis, kpos.ekbmepreis*

**Stück-Brutto** Anzeige des Brutto-Stückpreises.
*Technische Info: Anzeigefelder, DB-Felder: kpos.bstpreis, kpos.drbstpreis, kpos.ekbstpreis*

**Faktor** Anzeige des Faktors für den Preiszuschlag in Prozent. Über den Faktor können Sie die Preisberechnung für den Artikel ändern, ohne alle Preise anpassen zu müssen, z. B. für Preiserhöhungen oder Rabatte. In der Regel wird mit einem Faktor ein Rabatt gewährt.
*Technische Info: Anzeigefelder, DB-Felder: kpos.faktor, kpos.drfaktor, kpos.ekfaktor*

**Stück-Netto** Netto-Stückpreis.
*Technische Info: Anzeigefeld, numerisches Feld, DB-Felder: kpos.nstpreis, kpos.eknstpreis*

**Stück-Verglas** Stückpreis für Verglasungs- oder Montagearbeiten.
*Technische Info: numerische Felder, DB-Felder: kpos.vkverglas, kpos.ekverglas*

**Gesamtpreis** Anzeige des Netto-Gesamt-Preises der Position. Der Gesamtpreis berechnet sich aus Stückpreis x Menge der Artikel.
*Technische Info: Anzeigefelder, DB-Felder: kpos.nstpreis, kpos.ekpospreis*

**Abzgl** Abzüglich. Individuell vereinbarter Rabatt der Position. Sie können den Rabatt im ersten Feld als Prozentsatz oder im zweiten Feld als Betrag angeben. Das System errechnet den Wert für die anderen Felder.
*Technische Info: numerische Felder, Anzeigefeld, DB-Felder: kpos.rabatt, kpos.nachlass*

**Positionspr.** Positionspreis. Der Positionspreis berechnet sich aus dem Gesamtpreis abzüglich dem Rabatt aus dem Feld **Abzgl**. Sie können diesen Wert überschreiben, z. B. wenn ein Pauschalpreis vereinbart ist. Wenn Sie den Positionspreis ändern, wird der Rabatt im Feld **Abzgl** automatisch angepasst.
*Technische Info: numerisches Feld, Anzeigefeld, DB-Feld: kpos.npospreis*

Bei den folgenden Feldern wird nur ein Betrag angezeigt:

**DFÜ-Preis** Der DFÜ-Preis ist nur für Betriebe mit Filialstruktur von Bedeutung. Im Handelsbetrieb findet die Preisermittlung des Einkaufspreises statt. Dieser wird als DFÜ-Preis mit openTRANS an die Produktion übertragen und gilt als vorab ermittelter Verkaufspreis. Produktionsseitig kann die Gültigkeit dieses vorgegebenen Verkaufspreises durch die Kontrollpreisberechnung festgestellt werden.
*Technische Info: numerisches Feld, DB-Feld: kpos.dfuenstpreis*

**Spanne** Anzeige der Handelsspanne in Prozent zwischen Preis und Kosten.
*Technische Info: Anzeigefeld, DB-Feld: kpos.spanne*

**Materialko.** Anzeige der Materialkosten für die Position.
*Technische Info: Anzeigefeld, DB-Feld: kposp.komat*

**Lohnkosten** Anzeige der Lohnkosten für die Position. Die Lohnkosten werden erst angezeigt, wenn der Auftrag gespeichert und an die Produktion übergeben wurde. Die Kostenkalkulation in A+W Production berechnet die Kosten und schreibt sie in den Auftrag zurück. Die Kosten werden erst beim erneuten Öffnen des Auftrags angezeigt.
*Technische Info: Anzeigefeld, DB-Feld: kposp.kolohn*

**Maschinenko.** Anzeige der Maschinenkosten für die Position.
*Technische Info: Anzeigefeld, DB-Feld: kposp.kobm*

**Steuersätze** Nummer des Mehrwertsteuersatzes pro Position. Je nach Konfiguration können Sie pro Position einen Mehrwertsteuersatz oder mehrere Mehrwertsteuersätze zuweisen.
- Mit <F9> öffnen Sie die Liste der Mehrwertsteuersätze.
- Mit den Pfeiltasten navigieren Sie zwischen den Steuersätzen.
- Mit <Toggle> markieren Sie einen Mehrwertsteuersatz.
- Mit <Ende> schließen Sie den Dialog und übernehmen die Auswahl.
*Technische Info: Auswahl-Feld, DB-Feld: kpos.steuerzu*

#### Fußbereich
Die Felder und Schaltflächen im Fußbereich sind zum Register **Auftragspositionen – Allgemein** beschrieben:
⇨ "Auftragspositionen - Allgemein" auf Seite D-1167

### Auftragspositionen – Status
> Verkauf > Auftragserfassung > Register Positionen > Register Status

*(Abb. D-48: Auftragserfassung – Status zeigt den Status-Tab mit einer Übersicht über die Mengen in verschiedenen Fertigungsstadien: Fertig, Verpackt, Geliefert, Berechnet, Storno.)*

In diesem Register werden die Positionswerte entsprechend dem aktuellen Status der Positionen angezeigt, z. B. Anzahl der gelieferten und fakturierten Artikel. Als erste Position wird in der Positionsübersicht die Position angezeigt, die im Register **Allgemein** markiert ist. Mit den Pfeiltasten und <Bild hoch>, <Bild runter> navigieren Sie in der Positionsübersicht.
In der Regel müssen Sie die Angaben im Register **Status** nicht bearbeiten.

Wenn sich der Status ändert, wird auf Höhe des Registers ein entsprechender Hinweis zum Bearbeitungsstand der markierten Position angezeigt, z. B. **Ausgeliefert Lokal – Korrektur**. Vor dem Feld **Pos** werden der Positionsstatus und ggf. das Positionskennzeichen angezeigt.
⇨ "Symbolerklärung" auf Seite D-1128

#### Kopfbereich
Die Felder im Kopfbereich sind zum Register **Auftragserfassung – Kopf-, Fußbereich** beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-1135

#### Register Status
Die meisten Felder im Register **Status** sind zum Register **Allgemein** beschrieben:
⇨ "Auftragspositionen - Allgemein" auf Seite D-1167

Zusätzlich werden folgende Felder angezeigt:
**Fertig** Anzeige der gefertigten Einheiten pro Position.
*Technische Info: Anzeigefeld, DB-Feld: kpos.lugesfert*

**Verpackt** Anzeige der verpackten und zum Transport vorbereiteten Einheiten pro Position.
*Technische Info: Anzeigefeld, DB-Feld: kpos.gespack*

**Gelief.** Anzeige der ausgelieferten Einheiten pro Position.
*Technische Info: Anzeigefeld, DB-Feld: kpos.geslief*

**Berech** Anzeige der fakturierten Einheiten pro Position.
*Technische Info: Anzeigefeld, DB-Feld: kpos.gesberech*

**Storno** Anzeige der stornierten Einheiten pro Position.
*Technische Info: Anzeigefeld, DB-Feld: kpos.gesstorno*

#### Fußbereich
Die Felder und Schaltflächen im Fußbereich sind zum Register **Auftragspositionen – Allgemein** beschrieben:
⇨ "Auftragspositionen - Allgemein" auf Seite D-1167

### Auftragspositionen – Kosten
> Verkauf > Auftragserfassung > Register Positionen > Register Kosten

*(Abb. D-49: Auftragserfassung – Kosten zeigt den Kosten-Tab mit einer Aufschlüsselung der Kosten pro Position in Materialkosten, Lohnkosten und Maschinenkosten.)*

In diesem Register werden die Auftragskosten der Positionen angezeigt, z. B. Materialkosten, Lohnkosten. Als erste Position wird in der Positionsübersicht die Position angezeigt, die im Register **Allgemein** markiert ist. Mit den Pfeiltasten und <Bild hoch>, <Bild runter> navigieren Sie in der Positionsübersicht.
In der Regel müssen Sie die Angaben im Register **Kosten** nicht bearbeiten.

Wenn sich der Status ändert, wird auf Höhe des Registers ein entsprechender Hinweis zum Bearbeitungsstand der markierten Position angezeigt, z. B. **Ausgeliefert Lokal – Korrektur**. Vor dem Feld **Pos** werden der Positionsstatus und ggf. das Positionskennzeichen angezeigt.
⇨ "Symbolerklärung" auf Seite D-1128

#### Kopfbereich
Die Felder im Kopfbereich sind zum Register **Auftragserfassung – Kopf-, Fußbereich** beschrieben:
⇨ "Auftragserfassung - Kopf-, Fußbereich" auf Seite D-1135

#### Register Kosten
Die meisten Felder im Register **Kosten** sind zum Register **Allgemein** beschrieben:
⇨ "Auftragspositionen - Allgemein" auf Seite D-1167

Zusätzlich werden folgende Felder angezeigt:
**Materialk.** Anzeige der Materialkosten für die Position.
*Technische Info: Anzeigefeld, DB-Feld: kposp.komat*

> **Anzeige der Lohn- und Maschinenkosten**
> Die Lohn- und Maschinenkosten werden erst angezeigt, wenn der Auftrag gespeichert und an die Produktion übergeben wurde. Die Kostenkalkulation in A+W Production berechnet die Kosten und schreibt sie in den Auftrag zurück. Die Kosten werden erst beim erneuten Öffnen des Auftrags angezeigt.

**Lohnkosten** Anzeige der Lohnkosten für die Position.
*Technische Info: Anzeigefeld, DB-Feld: kposp.kolohn*

**Maschinenk.** Anzeige der Maschinenkosten für die Position.
*Technische Info: Anzeigefeld, DB-Feld: kposp.kobm*

#### Fußbereich
Die Felder und Schaltflächen im Fußbereich sind zum Register **Auftragspositionen - Allgemein** beschrieben:
⇨ "Auftragspositionen - Allgemein" auf Seite D-1167

## Hauswechsel
> Verkauf > Auftragserfassung > Kopf-, Fußbereich > <F4> > Hauswechsel

*(Abb. D-50: Hauswechsel zeigt einen Dialog "Werteingabe" mit einer Suchleiste und einer Ergebnisliste von verfügbaren "Häusern" (Mandanten) mit Nummer und Name.)*

In diesem Dialog wechseln Sie das Haus. Der Dialog ist nur freigeschaltet, wenn die interne Mandantentrennung aktiv ist, Sie die erforderlichen Rechte besitzen und das System entsprechend konfiguriert ist.
Alternativ können Sie den Dialog **Hauswechsel** auch mit <F5> im Feld **Eingang** im Kopfbereich öffnen.

> **Mehrsprachige Bezeichnungen**
> Seit QR2209 können Sie in A+W Enterprise zu einigen Stammdaten-Schlüsseln mehrsprachige Bezeichnungen hinterlegen, um allen Anwendern zu ermöglichen in deren Sprache das Programm zu bedienen. Wenn jedoch der Hauswechsel über diesen Dialog vorgenommen wird, so wird die Anwendersprache nicht gewechselt. Es bleibt die Sprache des ursprünglichen - im Mitarbeiterstamm zugeordneten – Hauses bestehen.

**Haus** Mandantennummer (Hausnummer), zu der gewechselt wird.
Mit <F9> werden die verfügbaren Häuser angezeigt.

> **Automatischer Hauswechsel**
> Je nach Konfiguration kann dem Auftrag automatisch ein anderes Haus zugeordnet werden.
> Für kundenindividuelle Anpassungen kontaktieren Sie Ihren Ansprechpartner der A+W Software GmbH.

## Neue Lieferadresse
> Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > <F4> > Adressen > Neue Lieferadresse

*(Abb. D-51: Neue Lieferadresse zeigt einen Dialog zur Erfassung einer neuen Lieferadresse mit Feldern für Name, Straße, PLZ, Ort, Land und weiteren logistischen Informationen wie Route und Ladefolge.)*

In diesem Dialog erfassen Sie eine neue Lieferadresse.
- Mit [OK] speichern Sie die neue Lieferadresse des Auftrags.
- Mit <F3> speichern Sie die neue Lieferadresse in den Stammdaten.

### Kopfbereich
Im diesem Bereich werden die aktuelle Nummer der Adresse, die Kundennummer und die Hauptlieferadresse des Kunden angezeigt.

### Lieferadresse
**Name, Vorname** Nachname und Vorname des Kunden.
*Technische Info: Pflichtfeld, alphanumerische Felder, DB-Felder: adr.adrname, adr.adrvname*

**Anrede** Nummer der Anrede des Kunden. Wenn Sie eine Nummer angeben, wird die Anrede im Klartext angezeigt.
*Technische Info: numerisches Feld, DB-Feld: adr.anrede*

**z. Hd.** Name des Mitarbeiters, der die Lieferung in Empfang nimmt.
*Technische Info: alphanumerisches Feld, DB-Feld: adr.zhd*

**Zusatz** Zusätzliche Information zur Adresse.
*Technische Info: alphanumerisches Feld, DB-Feld: adr.branche*

**Straße** Straßenname und Hausnummer der Lieferanschrift.
*Technische Info: Pflichtfeld, alphanumerisches Feld, DB-Feld: adr.str*

**PLZ, Fach** Postleitzahl und Nummer des Postfachs.
*Technische Info: alphanumerische Felder, DB-Felder: adr.pfplz, adr.postfach*

**PF Ort** Ortsname des Postfachs.
*Technische Info: alphanumerisches Feld, DB-Feld: adr.pfort*

**PLZ, Ort** Postleitzahl und Ortsname der Lieferanschrift.
*Technische Info: Pflichtfelder, alphanumerische Felder, DB-Felder: adr.plz, adr.ort*

**Versandregion** Versandregion. Die Versandregion ist in den Systemstammdaten hinterlegt und wird über die PLZ ermitelt.
*Technische Info: Anzeigefeld*

**KFZ Land** Internationales Landeskennzeichen für Kraftfahrzeuge des Ziel-Landes. Wenn Sie ein Kennzeichen angeben, wird der Landesname im Klartext angezeigt.
*Technische Info: alphanumerisches Feld, DB-Feld: adr.kfzcode*

**Entfernung** Entfernung bis zum Kunden in Kilometer.
*Technische Info: numerisches Feld, DB-Feld: adr.kilometer*

**Fahrtzeit** Fahrtzeit bis zum Kunden in Tagen.
*Technische Info: numerisches Feld, DB-Feld: adr.fahrtzeit*

**Tel** Telefonnummer des Kunden.
*Technische Info: alphanumerisches Feld, DB-Feld: adr.orgtel*

**Fax** Faxnummer des Kunden.
*Technische Info: alphanumerisches Feld, DB-Feld: adr.faxnr*

**E-Mail** E-Mail-Adresse des Kunden.
*Technische Info: alphanumerisches Feld, DB-Feld: adr.email*

**Std. Route** Nummer der Standardroute des Kunden. Wenn Sie eine Nummer angeben, wird die Bezeichnung der Route im Klartext angezeigt.
*Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: adr.routenr*

**Ladefolge** Nummer der gewünschten Ladefolge. Die Ladefolge legt fest, in welcher Reihenfolge ein LKW beladen wird. Sie dient dem Logistikmitarbeiter zur Information bei der Beladung des LKWs und kann je nach Konfiguration auf den Lieferschein gedruckt werden. Standardmäßig wird die Ladefolge in der Versandsteuerung festgelegt. Wenn Sie eine Nummer angeben, wird diese an die Versandsteuerung übermittelt.
*Technische Info: numerisches Feld, DB-Feld: adr.routeposnr*

**Bemerkung** Textbereich für zusätzliche Informationen.
*Technische Info: alphanumerische Felder, DB-Felder: adr.text1, adr.text2, adr.text3*

## Endkundenanschrift
> Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > <F4> > Adressen > Endkundenanschrift

*(Abb. D-52: Endkundenanschrift zeigt einen Dialog zur Erfassung der Adresse des Endkunden, insbesondere für Abholungen oder Direktlieferungen, mit Feldern für Name, Straße, Anlieferstelle, Route und Ladefolge.)*

In diesem Dialog hinterlegen Sie eine Endkundenanschrift. Wenn vom Kunden die Ware selbst abgeholt wird, müssen Sie im Einkauf eine Abholadresse angeben.

**Name, Vorname** Name und Vorname des Endkunden.
*Technische Info: Pflichtfeld, alphanumerische Felder, DB-Felder: adr.adrname, adr.vname*

**Anrede** Nummer der Anrede des Endkunden. Wenn Sie eine Nummer angeben, wird die Anrede im Klartext angezeigt.
*Technische Info: numerisches Feld, DB-Feld: adr.anrede*

**z. Hd.** Name des Mitarbeiters, der die Lieferung in Empfang nimmt.
*Technische Info: alphanumerisches Feld, DB-Feld: adr.zhd*

**Branche** Branche des Mitarbeiters.
*Technische Info: alphanumerisches Feld, DB-Feld: adr.branche*

**Straße** Straßenname und Hausnummer des Endkunden.
*Technische Info: alphanumerisches Feld, DB-Feld: adr.str*

**Postfach** Postleitzahl und Ort des Postfachs.
*Technische Info: alphanumerische Felder, DB-Felder: adr.pfplz, adr.postfach*

**PF Ort** Ortsname des Postfachs.
*Technische Info: alphanumerisches Feld, DB-Feld: adr.pfort*

**PLZ, Ort** Postleitzahl und Ortsname der Endkundenanschrift.
*Technische Info: alphanumerische Felder, DB-Felder: adr.plz, adr.ort*

**KFZ Land** Internationales Landeskennzeichen für Kraftfahrzeuge des Empfänger-Landes. Wenn Sie ein Kennzeichen angeben, wird der Landesname im Klartext angezeigt.
*Technische Info: alphanumerische Felder, DB-Feld: adr.kfzcode, adr.land*

**Entfernung** Entfernung bis zum Endkunden in Kilometer.
*Technische Info: numerisches Feld, DB-Feld: adr.kilometer*

**Fahrtzeit** Voraussichtliche Fahrtzeit bis zum Endkunden. Die Fahrtdauer wirkt sich auf den Liefertermin aus.
*Technische Info: numerisches Feld, DB-Feld: adr.fahrtzeit*

**Handlingszeit** Zeit zum Beladen und Entladen der Lieferung.
*Technische Info: numerisches Feld, DB-Feld: adr.handlingszeit*

**Ankunftszeit** Gewünschte Ankunftszeit beim Kunden im Format hh:mm.
*Technische Info: alphanumerisches Feld, DB-Feld: adr.ankunftszeit*

**Anlieferstelle** Genauere Beschreibung der Anlieferstelle, z. B. Tor A.
*Technische Info: alphanumerisches Feld, DB-Feld: adr.anlieferstelle*

**Faxnummer** Faxnummer des Endkunden.
*Technische Info: alphanumerisches Feld, DB-Feld: adr.fax*

**Route** Nummer der Fahrtroute.
*Technische Info: numerisches Feld, DB-Feld: adr.routenr*

**Ladefolge** Nummer der gewünschten Ladefolge. Die Ladefolge legt fest, in welcher Reihenfolge ein LKW beladen wird. Sie dient dem Logistikmitarbeiter als Information bei der Beladung des LKWs und kann je nach Konfiguration auf den Lieferschein gedruckt werden. Standardmäßig wird die Ladefolge in der Versandsteuerung festgelegt. Wenn Sie eine Nummer angeben, wird diese an die Versandsteuerung übermittelt.
*Technische Info: numerisches Feld, DB-Feld: adr.routeposnr*

**Bemerkung** Textfelder für zusätzliche Informationen.
*Technische Info: alphanumerische Felder, DB-Felder: adr.text1, adr.text2, adr.text3*

## Marktpartner-Info
> Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > <Shift> + <F4> > Marktpartner-Information

*(Abb. D-53: Marktpartner-Info zeigt einen Informationsdialog über einen Kunden. Er enthält offene Posten, offene Aufträge, Kreditlimits sowie eine Tabelle mit dem letzten Angebot, Auftrag und der letzten Rechnung.)*

In diesem Dialog werden Informationen über den ausgewählten Marktpartner aus den Stammdaten angezeigt.

### Kopfbereich
**Kunde** Nummer und Kundenname. Standardmäßig ist der Kunde aus dem aktuellen Vorgang ausgewählt. Sie können die Nummer überschreiben und einen anderen Kunden wählen. Wenn Sie eine Nummer angeben, wird der Kundenname im Klartext angezeigt.
*Technische Info: Pflichtfeld, numerisches Feld, DB-Feld: limits.kunr*

**Haus** Nummer und Bezeichnung des Hauses. Standardmäßig ist das Haus aus dem aktuellen Vorgang ausgewählt. Sie können die Nummer überschreiben und ein anderes Haus wählen. Wenn Sie eine Nummer angeben, wird die Bezeichnung des Hauses im Klartext angezeigt. Das Feld wird nur angezeigt, wenn Sie mit interner Mandantentrennung arbeiten.
*Technische Info: numerisches Feld, DB-Feld: kauf.hausnr*

### O.-Posten FIBU
In diesem Bereich werden die offenen Posten aus der Finanzbuchhaltung (FIBU) angezeigt.

**Offene Posten** Anzeige des Postens für Rechungen, die noch nicht an die FIBU übergeben sind.
*Technische Info: Anzeigefeld, DB-Feld: limits.op*

**Firmenlimit** Anzeige des definierten Firmenlimits, das die unbezahlten Rechnungen nicht übersteigen darf.
*Technische Info: Anzeigefeld, DB-Feld: limits.sglimit*

**Offene Aufträge** Anzeige der Aufträge, die noch nicht geliefert und/oder fakturiert sind.
*Technische Info: Anzeigefeld, DB-Feld: limits.oa*

**AKV-Limit** Anzeige des versicherten Kreditlimits.
*Technische Info: Anzeigefeld, DB-Feld: limits.akvlimit*

### Tabelle
In der Tabelle werden Informationen zum letzten Angebot, zum letzten Auftrag und zur letzten Rechnung des ausgewählten Kunden angezeigt:
- **Datum:** Erfassungs- oder Änderungsdatum des Vorgangs.
- **Nummer:** Vorgangsnummer.
- **Haus:** Mandantennummer (Hausnummer), die dem Vorgang zugeordnet ist.
- **Betrag:** Netto-End-Betrag des Vorgangs.
*Technische Info: Anzeigefelder, DB-Felder: kauf.auftrnr*

### Fußbereich
In diesem Bereich wird der aufgelaufene Umsatz des ausgewählten Kunden im aktuellen Jahr angezeigt.

## Ansprechpartner
> Verkauf > Auftragserfassung > Kopf-, Fußbereich > <F4> > Ansprechpartner

*(Abb. D-54: Ansprechpartner zeigt einen Dialog zur Verwaltung von Ansprechpartnern eines Kunden. Es können Name, Anrede, Abteilung, Position und Kontaktdaten erfasst oder bearbeitet werden.)*

In diesem Dialog erfassen Sie einen Ansprechpartner für den gewählten Marktpartner oder weisen dem Marktpartner einen Ansprechpartner aus den Stammdaten zu.
- Mit <Bild hoch> und <Bild runter> werden die Ansprechpartner angezeigt, die für den Marktpartner hinterlegt sind.
- Mit <F6> können Sie einen neuen Ansprechpartner erfassen.

### Kopfbereich
In diesem Bereich werden die aktuelle Nummer des Ansprechpartners, die Kundennummer und der Hauptansprechpartner angezeigt.

> **Hauptansprechpartner festlegen**
> Wenn für einen Marktpartner mehrere Ansprechpartner hinterlegt sind, können Sie in den Marktpartnerstammdaten einen Hauptansprechpartner festlegen.

### Ansprechpartner
In diesem Bereich erfassen oder bearbeiten Sie die Daten eines Ansprechpartners.

**Name, Vorname** Nachname und Vorname des Ansprechpartners.
*Technische Info: Pflichtfeld, alphanumerische Felder, DB-Felder: anspr.apname, anspr.apvname*

**Anrede** Nummer der Anrede des Ansprechpartners. Wenn Sie eine Nummer angeben, wird die Bezeichnung im Klartext angezeigt.
*Technische Info: numerisches Feld, DB-Feld: anspr.anrede*

**Abteilung** Abteilung, in der der Ansprechpartner arbeitet.
*Technische Info: alphanumerisches Feld, DB-Feld: anspr.abteilung*

**Position** Position des Ansprechpartners im Unternehmen.
*Technische Info: alphanumerisches Feld, DB-Feld: anspr.position*

**Geb-Datum** Geburtsdatum des Ansprechpartners im Format TT.MM.JJJJ.
*Technische Info: Datumsfeld, DB-Feld: anspr.gebdat*

**Telefon** Telefonnummer des Ansprechpartners.
*Technische Info: alphanumerisches Feld, DB-Feld: anspr.telefon*

**Fax** Faxnummer des Ansprechpartners.
*Technische Info: alphanumerisches Feld, DB-Feld: anspr.telefax*

**Mobil** Mobilnummer des Ansprechpartners.
*Technische Info: alphanumerisches Feld, DB-Feld: anspr.telex*

**E-Mail** E-Mail-Adresse des Ansprechpartners.
*Technische Info: alphanumerisches Feld, DB-Feld: anspr.email*

**Felder ohne Bezeichnung** Zusätzliche Bemerkung zum Ansprechpartner.
*Technische Info: alphanumerische Felder, DB-Felder: anspr.text1, anspr.text2, anspr.text3*

## Storno
> Verkauf > Auftragserfassung > Kopf-, Fußbereich, Positionsebene > <F4> > Storno

*(Abb. D-55: Storno zeigt einen einfachen Dialog mit einem Textfeld "Stornoinfo", in das ein Grund für die Stornierung eingegeben werden kann, z.B. "Terminänderung".)*

In diesem Dialog stornieren Sie einen Auftrag. Sie können zusätzliche Information zur Stornierung angeben.

Wenn Sie einen Auftrag stornieren wollen, wird zunächst eine Abfrage angezeigt, die Sie mit [Ja] bestätigen müssen.

**Stornoinfo** zusätzliche Information zur Stornierung, z. B. Grund des Stornos. Wenn ein stornierter Vorgang aufgerufen wird, dann wird diese Information angezeigt. Die Angabe der Information ist optional.
*Technische Info: alphanumerisches Feld, DB-Feld: kauf.exbez2*

### Erläuterung der Schaltflächen
**[OK]** Storniert den aktuellen Auftrag.
