---
title: "DE-HB-AWEnterprise_6"
source: "DE-HB-AWEnterprise_6.pdf"
tags: ["A+W Enterprise", "Software Reference", "Master Data", "Field Configuration", "Pricing", "Commissions", "Technical Manual", "German", "ERP"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a segment of the A+W Enterprise software reference manual, focusing on master data configuration. It covers field configuration, commissions, text management, cost master data, and an extensive tutorial on prices and conditions."
long_description: "This document serves as a detailed technical reference and tutorial for the A+W Enterprise software, specifically for modules related to master data management and pricing. The first part is a software reference for 'Stammdaten' (Master Data), covering Feldkonfiguration (Field Configuration) for market partners, articles, and processes; Provisionen (Commissions) including commission keys and assignments; Textverwaltung (Text Management) for generating dynamic and static texts; and Kostenstamm (Cost Master Data) for defining cost types, cost centers, and cost objects. The second, more extensive part is a comprehensive tutorial on 'Preise und Konditionen' (Prices and Conditions). This tutorial details the fundamentals of price determination, the setup of various price definitions (keys, logic, components), and the management of master data for prices, including matrices for insulating glass, price vectors, surcharges, and global price changes. It provides step-by-step workflows, examples, and exercises to guide users in configuring and managing the complex pricing and conditions system within A+W Enterprise."
---

# A+W Enterprise Stammdaten

---
## Feldkonfiguration
Stammdaten > Feldkonfiguration

In diesem Bereich können Sie kundenspezifisch zusätzliche (private) Felder definieren, die dann im Marktpartnerstamm, im Artikelstamm oder in der Vorgangsverwaltung zur Verwendung stehen. Die Auswertung dieser Felder ist immer kundenindividuell und muss mit der Entwicklung abgestimmt werden. Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "MP-Feldkonfiguration" auf Seite B-502
- "Artikel-Feldkonfiguration" auf Seite B-504
- "Vorgangs-Feldkonfiguration" auf Seite B-506
- "Konfiguration Bezugnahme" auf Seite B-508

### MP-Feldkonfiguration
Stammdaten > Feldkonfiguration > MP-Feldkonfiguration

*Abb. B-235 MP-Feldkonfiguration*

In diesem Dialog bestimmen Sie, welche privaten Felder Sie für die Marktpartner anlegen möchten.

#### Erläuterung der Felder

**Datentyp**
Datentyp, der gespeichert werden soll:
- **ALPHANUM**: Text
- **NUM**: Zahl
- **DEC**: Dezimalzahl
- **DATUM**: Datumsfeld
*Technische Info: Toggle-Feld, DB-Feld: mpcomfld.fldtyp*

**Feldname**
Feldname (max. 20 Zeichen).
*Technische Info: Alphanumerisches Feld, DB-Feld: mpcomfld.fldbez*

**S-Typ**
mit dem STYP setzen Sie die Eigenschaften des Bewegungsdatenfeldes. Wenn Sie den STYP auf 2056 setzen, können Sie auch eine Überschrift für eine Gruppe von Feldern definieren. Setzen Sie dann das Feld in der Sequenz vor das erste Feld der Gruppe und hinterlegen Sie im Label einfach die gewünschte Gruppenüberschrift.
*Technische Info: Numerisches Feld, DB-Feld: mpcomfld.styp*

**Selo**
Dateiname für ein Selo.
*Technische Info: alphabetisches Feld, DB-Feld: mpcomfld.selo*

### Artikel-Feldkonfiguration
Stammdaten > Feldkonfiguration > Artikel-Feldkonfiguration

*Abb. B-236 Artikel-Feldkonfiguration*

In diesem Dialog bestimmen Sie, welche privaten Felder Sie für den Artikelstamm anlegen möchten.

#### Erläuterung der Felder

**Feldpos.**
An welcher vertikalen Position erscheint das Feld im Dialog.
*Technische Info: Numerisches Feld, DB-Feld: artcomfld.fldpos*

**Datentyp**
Datentyp, der gespeichert werden soll:
- **ALPHANUM**: Text
- **NUM**: Zahl
- **DEC**: Dezimalzahl
- **DATUM**: Datumsfeld
*Technische Info: Toggle-Feld, DB-Feld: artcomfld.fldtyp*

**Feldname**
Feldname (max. 20 Zeichen).
*Technische Info: Alphanumerisches Feld, DB-Feld: artcomfld.fldbez*

**S-Typ**
mit dem STYP setzen Sie die Eigenschaften des Bewegungsdatenfeldes. Wenn Sie den STYP auf 2056 setzen, können Sie auch eine Überschrift für eine Gruppe von Feldern definieren. Setzen Sie dann das Feld in der Sequenz vor das erste Feld der Gruppe und hinterlegen Sie im Label einfach die gewünschte Gruppenüberschrift.
*Technische Info: Numerisches Feld, DB-Feld: artcomfld.styp*

**Selo**
Dateiname für ein Selo.
*Technische Info: alphabetisches Feld, DB-Feld: artcomfld.selo*

### Vorgangs-Feldkonfiguration
Stammdaten > Feldkonfiguration > Vorgangs-Feldkonfiguration

*Abb. B-237 Vorgangs-Feldkonfiguration*

In diesem Dialog haben Sie die Möglichkeit, kundenspezifische Felder vorgangskopf- (kauf) bzw. positionsgenau (kpos) zu definieren. In diese Felder können dann individuelle Daten erfasst oder vorbelegt werden. Bei entsprechender kundenindividueller Bereitstellung sind auch die Belegung und Auswertung durch das System möglich.
Mit <F5> öffnen Sie einen Dialog, in dem Sie die entsprechenden fremdsprachige Bezeichnungen hinterlegen können.

#### Erläuterung der Felder

**Tabellenname**
Name der Bezugstabelle.
*Technische Info: alphabetisches Feld, DB-Feld: kflddef.tabname*

**Variablen-Set**
Nummer des zu konfigurierenden Variablen-Sets. Jedes Variablen-Set kann von den Datentypen char, decimal und integer jeweils bis zu 5 Felder enthalten.
*Technische Info: Numerisches Feld, DB-Feld: kflddef.setid*

**Überschrift**
Technische Info: alphabetisches Feld, DB-Feld: kflddef.ueberschrift

**Feldname**
Name des Feldes der Bezugstabelle, z. B. decval1).
*Technische Info: alphabetisches Feld, DB-Feld: kflddef.fieldname*

**Gruppe**
Gruppennummer. Mit Hilfe dieser Nummer kann AWE-Funktionalität, wie beispielsweise eine Wertberechnung, an diese Felder gebunden werden.
*Technische Info: Numerisches Feld, DB-Feld: kflddef.grpid*

**Seqnr**
Sequenznummer. Sie muss zwischen 1 und 20 liegen und eindeutig sein. Über diese Sequenznummer wird die Feldreihenfolge in den Bewegungsdaten festgelegt. Ein Sprung in der Sequenz bedeutet später in der Bewegungsdatenmaske eine Leerzeile zwischen den Feldern.
*Technische Info: Numerisches Feld, DB-Feld: kflddef.seqnr*

**Label**
Label im Vorgangsdialog. Es wird später in den Bewegungsdaten vor dem Feld angezeigt.
*Technische Info: Alphanumerisches Feld, DB-Feld: kflddef.label*

**S-Typ**
mit dem STYP setzen Sie die Eigenschaften des Bewegungsdatenfeldes. Wenn Sie den STYP auf 2056 setzen, können Sie auch eine Überschrift für eine Gruppe von Feldern definieren. Setzen Sie dann das Feld in der Sequenz vor das erste Feld der Gruppe und hinterlegen Sie im Label einfach die gewünschte Gruppenüberschrift.
*Technische Info: Numerisches Feld, DB-Feld: kflddef.styp*

**Länge**
Hier geben Sie die gewünschte Feldlänge ein. Sie darf die Maximallänge des Feldes nicht überschreiten.
*Technische Info: Numerisches Feld, DB-Feld: kflddef.length*

**Referenzfeld**
In dem Referenzfeld kann ein Datenbankfeld in der Notation `<Tabellenname>.<Spaltenname>` angegeben werden. Das konfigurierbare Feld wird dann mit dem Wert dieses Feldes vorbelegt. Dabei ist darauf zu achten, dass für kposprvfld nur Datenbanktabellen ausgewählt werden dürfen, die als Schlüssel das Feld artnr haben. Bei kaufprvfld können nur Tabellen verwendet werden, die als Schlüssel mpnr und kuliflag haben. Im Verkauf erfolgt die Vorbelegung immer aus dem Kundenstamm und im Einkauf immer aus dem Lieferantenstamm. Eventuell vorhandene Objekte bleiben bei der Vorbelegung unberücksichtigt. In diesem Feld kann auch ein fester Defaultwert angegeben werden. Damit das System erkennt, dass dort ein Defaultwert steht, muss eine Raute vorangestellt werden (z. B. #678 für ein Long-Feld oder #ABC für ein Char-Feld).
*Technische Info: Alphanumerisches Feld, DB-Feld: kflddef.reffield*

**Priv. Feld**
Hier können Sie die Nummer eines konfigurierbaren Feldes aus den Stammdaten angeben. Es steht bei kposprvfld der Artikelstamm und bei kaufprvfld der Marktpartnerstamm zur Verfügung. Dieser Eintrag übersteuert den Eintrag des Feldes Referenzfeld.
*Technische Info: Alphanumerisches Feld, DB-Feld: kflddef.prvfldnr*

### Konfiguration Bezugnahme
Stammdaten > Feldkonfiguration > Konfiguration Bezugnahme

*Abb. B-238 Konfiguration Bezugnahme*

Mit diesem Dialog steht Ihnen ein Konfigurationstool für die Feldübernahme in der Vorgangserfassung zur Verfügung. Sie können das gewünschte Programmverhalten bei der Bezugnahme und entsprechende Verhaltensweisen definieren.

#### Erläuterung der Felder

**Vorgang**
Auswahl der Vorgangsart.
*Technische Info: <F9>, DB-Feld: kfldrefdefk.vorgang*

**Bezugsvorgang**
Auswahl der Art des Bezugsvorgangs.
*Technische Info: <F9>, DB-Feld: kfldrefdefk.refvorgang*

**Marktpartnerwechsel**
Über diese Checkbox steuern Sie das Verhalten bei einem Marktpartnerwechsel. Bei der Übernahme der Daten aus dem Bezugsvorgang wird darauf geachtet, ob ein Marktpartnerwechsel stattgefunden hat. Wenn dies der Fall war, so werden die im Bezugsvorgang vorhandenen Daten übernommen, die Daten aber, die im Stamm durch Referenzeingabe einen Bezug zum Marktpartner besitzen, werden neu aus den Stammdaten des neuen Marktpartners gezogen.
- ☑ Für die Bezugserfassung MIT Marktpartnerwechsel.
- ☐ Für die Bezugserfassung ohne Marktpartnerwechsel.
*Technische Info: Toggle-Feld, DB-Feld: kfldrefdefk.mpwechsel*

**Positionen kopieren**
Über diese Einstellung steuern Sie, wie mit den Positionen des Bezugsvorgang verfahren werden soll.
- **Ja**: Die Positionen des Bezugsvorgangs sollen automatisch kopiert werden.
- **Frage**: Die Positionen des Bezugsvorgangs werden erst nach Rückfrage an den Anwender kopiert.
*Technische Info: <F9>, DB-Feld: kfldrefdefk.poskopieren*

**Freigabetext kopieren**
Über diese Einstellung steuern Sie, wie mit den Freigabetexten verfahren werden soll.
- **Ja**: Die Freigabetexte sollen kopiert werden.
- **Nein**: Die Freigabetexte sollen nicht kopiert werden.
*Technische Info: Toggle-Feld, DB-Feld: kfldrefdefk.freigabekopieren*

**Konfigurierbare Felder kopieren (Kopf)**
Über diese Einstellung steuern Sie, wie mit den konfigurierbaren Feldern des Vorgangskopfes verfahren werden soll.
- **Ja**: Die konfigurierbaren Felder sollen kopiert werden.
- **Nein**: Die konfigurierbaren Felder sollen nicht kopiert werden.
*Technische Info: Toggle-Feld, DB-Feld: kfldrefdefk.kaufprvkopieren*

**Konfigurierbare Felder kopieren (Positionen)**
Über diese Einstellung steuern Sie, wie mit den konfigurierbaren Feldern der Vorgangspositionen verfahren werden soll.
- **Ja**: Die konfigurierbaren Felder sollen kopiert werden.
- **Nein**: Die konfigurierbaren Felder sollen nicht kopiert werden.
*Technische Info: Toggle-Feld, DB-Feld: kfldrefdefk.kposprvkopieren*

**Feldname (intern)**
Auswahl des Feldnamen. Die Bezeichnung wird im Feld dahinter angezeigt.
*Technische Info: <F9>, DB-Feld: kfldrefdef.feldname*

**Bezeichnung**
Bezeichnung des Feldnamen in Klarsicht.
*Technische Info: Anzeige-Feld*

**Maskenname**
Interner Name der Dialogs.
*Technische Info: Anzeige-Feld*

**Neuermittlung**
In diesem Feld sehen Sie, ob die Neuermittlung aufgrund der Stammdaten erfolgt oder ob das Feld den Standardwert des entsprechenden Dialogs (z. B. Auftragserfassungs-Dialog) erhält.
*Technische Info: Anzeige-Feld*

## Provisionen
Stammdaten > Provisionen

Provisionen werden bereits bei der Auftragserfassung berücksichtigt und auf der Grundlage von Warengruppen, Kunden und Spannen berechnet. Bei der Rechnungs- bzw. Gutschriftsbuchung werden die Provisionen in einer Provisionstabelle (Verkauf > Vertrieb > Provisionen > Auftragsübersicht) auftragsbezogen gebucht und protokolliert. A+W Enterprise ermöglicht Provisionsberechnungen nach folgenden Verfahren:

- **Standardverfahren**: Es wird ein globaler Provisionsschlüssel im System hinterlegt, der im Auftrag manuell überschrieben werden kann.
- **Vertreter/Warengruppe**: Pro Vertreter und Warengruppe kann in A+W Enterprise ein Provisionsschlüssel hinterlegt werden. Die Pflege erfolgt über den Menüpunkt Provisionszuordnung (Stammdaten > Provisionen > Provisionszuordnung).
- **Kunde**: Im Kundenstamm kann zu jedem Kunden ein Provisionsschlüssel hinterlegt werden.
- **Spanne**: Abhängig vom Deckungsbeitrag der Position wird ein Provisionsschlüssel errechnet. Die Pflege erfolgt über den Menüpunkt Provisionszuordnung (Stammdaten > Provisionen > Provisionszuordnung).
- **Spanne/Warengruppe**: Pro Warengruppe kann eine spannenorientierte Provisionierung erfolgen.
- **Kunden/Warengruppe**: Die Provisionierung erfolgt kundenorientiert pro Warengruppe.
- **Vertreter/Kunde**: Eine warengruppenorientierte Provisionierung kann pro Vertreter kundenindividuell eingestellt werden (erlösmäßiger Vertreter).

Die Einstellung der entsprechenden Provisionsberechnung ist in A+W Enterprise fest eingestellt. Bei Bedarf ist eine Änderung des Standardverfahrens über den A+W Enterprise-Support möglich.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Provisionskürzel" auf Seite B-511
- "Provisionszuordnung" auf Seite B-512

### Provisionskürzel
Stammdaten > Provisionen > Provisionskürzel

*Abb. B-239 Provisionskürzel*

Hier können Sie für verschiedene Schlüsselwerte (Kürzel) Provisionssätze hinterlegen.
Damit ist es möglich, dass von den auftragserfassenden Mitarbeitern Provisionsschlüssel verwendet werden, ohne dass ihnen die konkreten Provisionssätze bekannt sind.

#### Erläuterung der Felder

**Kürzel**
Provisionsnummer. Zum Anlegen eines neuen Kürzels geben Sie die nächste freie Nummer ein.
*Technische Info: Numerisches Feld, DB-Feld: xprov.provnr*

**Provision**
Provisionsprozentsatz.
*Technische Info: Numerisches Feld, DB-Feld: xprov.provision*

### Provisionszuordnung
Stammdaten > Provisionen > Provisionszuordnung

*Abb. B-240 Provisionszuordnung*

Für den Fall, dass mit Vertreter/Warengruppen-, Spannen-, Spannen/Warengruppen-, Kunden/Warengruppen- und Vertreter/Kunden/Warengruppen-Verfahren gearbeitet wird, erfolgen die Provisionszuordnung über diesen Menüpunkt.

> **Entsprechende Felder**
> Der Provisionszuordnungsdialog ist dem eingesetzten Verfahren angepasst und präsentiert sich jeweils mit den benötigten Feldern.

Provisionen können durch die Kombination Vertreter, Kunde und Warengruppe spezifiziert werden. Jedem Vertreter können differenzierte Provisionssätze für Warengruppen oder kundenorientierte Warengruppen zugeordnet werden.

#### Erläuterung der Felder

**Vertreter**
Auswahl der Vertreternummer. Der Name wird im Feld dahinter angezeigt.
*Technische Info: <F9>, DB-Feld: provzu.vertreter*

**Warengruppe**
Auswahl der Warengruppe. Der Name wird im Feld dahinter angezeigt.
*Technische Info: Numerisches Feld, DB-Feld: xprov.wagrp*

**ab Datum**
Der vereinbarte Provisionszeitraum kann bereits im voraus erfasst werden. Die Verwaltung von mehreren Provisionszeiträumen eines Vertreters ist so möglich.
*Technische Info: Numerisches Feld, DB-Feld: xprov.datum*

**Prov-Kürzel**
Unterschiedliche Provisionssätze werden durch das Provisionskürzel an jedem Zeilenende spezifiziert.
*Technische Info: Numerisches Feld, DB-Feld: xprov.provnr*

## Textverwaltung
Stammdaten > Textverwaltung

Im diesem Bereich werden grundlegende Daten für die Textgenerierung innerhalb der Vorgangserfassung definiert. Variable und konstante Textpassagen bzw. Textformeln, die hier gepflegt werden, erscheinen später in der Vorgangs-Erfassung, auf Produktionspapieren oder kundenbezogenen Unterlagen. Die Texte haben somit nicht nur informativen, sondern auch Werbecharakter und können so den Einfluss auf Geschäftsbeziehungen nehmen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Aktuelle Texte" auf Seite B-514
- "Gruppentexte" auf Seite B-515
- "Objekttexte" auf Seite B-516
- "Warengruppentexte" auf Seite B-517
- "Konfigurierbare Texte" auf Seite B-518
- "Floskeln" auf Seite B-519
- "Variablenbezeichnung" auf Seite B-520
- "Textformeln" auf Seite B-521

### Aktuelle Texte
Stammdaten > Textverwaltung > Aktuelle Texte

*Abb. B-241 Aktuelle Texte*

In diesem Dialog können Texte hinterlegt werden, die auf den kundenseitigen Papieren ausgedruckt werden sollen. Über <F5> wird bestimmt, auf welchen Formularen die Texte auszugeben sind. Die ausgewählten Formulare werden am unteren Rand des Fensters präsentiert.

#### Erläuterung der Felder

**Datei**
Name der Textdatei, in der die Texte gespeichert werden.
*Technische Info: Alphanumerisches Feld, DB-Feld: akttxt.datei*

**Nr**
Für den Fall, dass mehrere Texte innerhalb einer Druckposition vorgesehen sind, kann über dieses Feld die Reihenfolge festgelegt werden.
*Technische Info: Alphanumerisches Feld, DB-Feld: akttxt.Ifdnr*

**Druckposition**
Die Druckposition bestimmt, ob der jeweilige Text im Kopf, im Fuß oder im Rumpf gedruckt werden soll.
*Technische Info: Toggle-Feld, DB-Feld: akttxt.drupos*

**Ablaufdatum**
Die hinterlegten Texte sind bis zum Zeitpunkt des Ablaufdatums gültig. So ist es z. B. möglich, den Briefverkehr bis zum 14.12. mit Weihnachtsgrüßen zu versehen.
*Technische Info: Numerisches Feld, DB-Feld: stammtxt.verfalldat*

### Gruppentexte
Stammdaten > Textverwaltung > Gruppentexte

*Abb. B-242 Gruppentexte*

Die Gruppenzuordnung im Kundenstamm ermöglicht eine individuelle Vertextung pro Gruppe. Den verschiedenen Kundengruppen können hier im Rahmen der Textverwaltung Texte zugeordnet werden, die auf den kundenseitigen Papieren ihre Ausgabe finden. Damit kann beispielsweise die Kundengruppe der Fensterbauer über die Einführung eines neuen Isolierglasproduktes informiert werden.

#### Erläuterung der Felder

**Gruppe**
Auswahl der Gruppennummer. Der Name wird im Feld dahinter angezeigt.
*Technische Info: <F9>, DB-Feld: grptxt.grpnr*

**Datei**
Auswahl der Datei.
*Technische Info: <F9>, DB-Feld: grptxt.datei*

**Nr**
Für den Fall, dass mehrere Texte innerhalb einer Druckposition vorgesehen sind, kann über dieses Feld die Reihenfolge festgelegt werden.
*Technische Info: Alphanumerisches Feld, DB-Feld: grptxt.Ifdnr*

**Druckposition**
Die Druckposition bestimmt, ob der jeweilige Text im Kopf, im Fuß oder im Rumpf gedruckt werden soll.
*Technische Info: Toggle-Feld, DB-Feld: akttxt.drupos*

### Objekttexte
Stammdaten > Textverwaltung > Objekttexte

*Abb. B-243 Objekttexte*

Dieser Dialog ermöglicht eine individuelle Vertextung pro Objekt. Den verschiedenen Objekten können hier im Rahmen der Textverwaltung Texte zugeordnet werden, die auf den kundenseitigen Papieren ihre Ausgabe finden.

#### Erläuterung der Felder

**Objekt**
Auswahl der Objektnummer. Der Name wird im Feld dahinter angezeigt.
*Technische Info: <F9>, DB-Feld: objtxtzu.objnr*

**Datei**
Auswahl der Datei.
*Technische Info: <F9>, DB-Feld: objtxtzu.datei*

**Nr**
Für den Fall, dass mehrere Texte innerhalb einer Druckposition vorgesehen sind, kann über dieses Feld die Reihenfolge festgelegt werden.
*Technische Info: Alphanumerisches Feld, DB-Feld: objtxtzu.Ifdnr*

**Druckposition**
Die Druckposition bestimmt, ob der jeweilige Text im Kopf, im Fuß oder im Rumpf gedruckt werden soll.
*Technische Info: Toggle-Feld, DB-Feld: objtxtzu.drupos*

### Warengruppentexte
Stammdaten > Textverwaltung > Warengruppentexte

*Abb. B-244 Warengruppentexte*

Dieser Dialog ermöglicht eine individuelle Vertextung pro Warengruppe. Den verschiedenen Warengruppen können hier im Rahmen der Textverwaltung Texte zugeordnet werden, die auf den kundenseitigen Papieren ihre Ausgabe finden.

#### Erläuterung der Felder

**Warengruppe**
Auswahl der Warengruppe. Der Name wird im Feld dahinter angezeigt.
*Technische Info: <F9>, DB-Feld: wargrptxt.wgrnr*

**Datei**
Auswahl der Datei.
*Technische Info: <F9>, DB-Feld: wargrptxt.datei*

**Nr**
Für den Fall, dass mehrere Texte innerhalb einer Druckposition vorgesehen sind, kann über dieses Feld die Reihenfolge festgelegt werden.
*Technische Info: Alphanumerisches Feld, DB-Feld: wargrptxt.Ifdnr*

**Druckposition**
Die Druckposition bestimmt, ob der jeweilige Text im Kopf, im Fuß oder im Rumpf gedruckt werden soll.
*Technische Info: Toggle-Feld, DB-Feld: wargrptxt.drupos*

### Konfigurierbare Texte
Stammdaten > Textverwaltung > Konfigurierbare Texte

*Abb. B-245 Konfigurierbare Texte*

Dieser Dialog bietet Ihnen die Möglichkeit, Texte frei zu konfigurieren, z. B. für interne Zwecke auf Produktionspapieren.

#### Erläuterung der Felder

**Stored Procedure**
Auswahl der Stored Procedure. Der Übergabewert für die SP wird im Feld dahinter angezeigt.
*Technische Info: <F9>, DB-Feld: auftxtzu.spiname*

**Wert**
Übergabewert für Stored Procedure.
*Technische Info: <F9>, DB-Feld: auftxtzu.ret*

**Datei**
Auswahl der Datei.
*Technische Info: <F9>, DB-Feld: auftxtzu.datei*

**Nr**
Für den Fall, dass mehrere Texte innerhalb einer Druckposition vorgesehen sind, kann über dieses Feld die Reihenfolge festgelegt werden.
*Technische Info: Alphanumerisches Feld, DB-Feld: auftxtzu.Ifdnr*

**Druckposition**
Die Druckposition bestimmt, ob der jeweilige Text im Kopf, im Fuß oder im Rumpf gedruckt werden soll.
*Technische Info: Toggle-Feld, DB-Feld: auftxtzu.drupos*

**Ablaufdatum**
Die hinterlegten Texte sind bis zum Zeitpunkt des Ablaufdatums gültig.
*Technische Info: Numerisches Feld, DB-Feld: auftxtzu.verfalldat*

### Floskeln
Stammdaten > Textverwaltung > Floskeln

*Abb. B-246 Floskeln*

Dieser Dialog bietet Ihnen die Möglichkeit, neue Floskeln anzulegen bzw. zu bearbeiten.

#### Erläuterung der Felder

**Kennung**
Auswahl der Floskel. Zum Anlegen einer neuen Floskel geben Sie die nächste freie Nummer ein. Im Feld dahinter wird der Name angezeigt.
*Technische Info: <F9>, DB-Feld: floskel.code/txt*

**Feld darunter**
Hier wird Ihnen der Text der Floskel angezeigt. Einen neuen Text können Sie hier eingeben.
*Technische Info: <F9>, DB-Feld: floskel.txt*

**Bereich rechts**
Über die Checkboxen steuern Sie, auf welchen Formularen die Floskel ausgegeben wird.
*Technische Info: Toggle-Feld, DB-Feld: floskel.formular*

### Variablenbezeichnung
Stammdaten > Textverwaltung > Textgenerierung > Variablenbezeichnung

*Abb. B-247 Variablenbezeichnung*

In diesem Dialog können Sie eigene Variablen für die spätere Textgenerierung definieren. Diese werden auch bei der Erstellung von Textformeln verwendet. Dadurch können Sie nach eigenen Wünschen beliebige Daten in die generierten Texte integrieren.

#### Erläuterung der Felder

**Variable**
Name der Variablen. Zum Anlegen einer neuen Variablen, geben Sie die entsprechende Bezeichnung ein. Die Variablen werden in der Regel in Großbuchstaben hinterlegt.
*Technische Info: Alphanumerisches Feld, DB-Feld: frmvarname.varname*

**Tabelle**
Auswahl der entsprechenden Tabelle.
*Technische Info: <F9>, DB-Feld: frmvarname.dbtable*

**Feld**
Auswahl des Feldnamen.
*Technische Info: <F9>, DB-Feld: frmvarname.dbfield*

### Textformeln
Stammdaten > Textverwaltung > Textgenerierung > Textformeln

*Abb. B-248 Textformeln*

In diesem Dialog erstellen Sie die Formeln für die Textgenerierung. Diese werden z. B. bei der Erzeugung von Kistensignaturen verwendet.

#### Erläuterung der Felder

**Nummer**
Nummer der Textformel. Zum Anlegen einer neuen Formel geben Sie die nächste freie Nummer ein.
*Technische Info: Numerisches Feld, DB-Feld: artkennfrm.artkennfrm*

**Formelbezeichnung**
Formelbezeichnung. Für neue Formeln geben Sie die gewünschte Bezeichnung ein.
*Technische Info: Alphanumerisches Feld, DB-Feld: artkennfrm.formelbez*

**Formeltext**
In diesem Feld befindet sich der Formeltext. Über <F9> haben Sie Zugriff auf die Variablen.
*Technische Info: Alphanumerisches Feld, <F9>, DB-Feld: artkennfrm.formeltxt*

## Kostenstamm
Stammdaten > Kostenstamm

Die Gliederung des Aufwandes kann nach Kostenträgern (z. B. Herstellungskosten für Produkt A, Produkt B usw.), nach Kostenstellen (z. B. Kosten des Fertigungs-, des Verwaltungs-, des Vertriebsbereiches) oder nach Kostenarten (Löhne, Gehälter, Material, Abschreibungen, Steuern usw.) erfolgen.

Das hier eingerichtete System zur Aufwandserfassung ist nicht in die kaufmännischen oder fertigungstechnischen Bereiche integriert. Es dient lediglich einer manuellen Erfassung von Aufwendungen, die im Statistikbereich nach unterschiedlichen Gesichtspunkten ausgewertet werden.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Kostenarten" auf Seite B-523
- "Kostenträger" auf Seite B-524
- "Kostenstellen" auf Seite B-526

### Kostenarten
Stammdaten > Kostenstamm > Kostenarten > Einzelne Bezeichnung
Stammdaten > Kostenstamm > Kostenarten > Alle Bezeichnung

*Abb. B-249 Kostenarten*

Hier können sämtliche Kostenarten mit ihrer Bezeichnung und Angabe der übergeordneten Kostenart tabellarisch eingetragen werden. Über die Hauptkostenart ist dabei eine Zusammenfassung bestimmter Kostenarten möglich.

> **Mehrsprachige Bezeichnungen**
> Seit QR2209 können Sie in A+W Enterprise auch für Kostenarten mehrsprachige Bezeichnungen hinterlegen.

#### Erläuterung der Felder

**K-Art**
Anzeige der Schlüssel-Nummer. Zum Anlegen einer neuen Kostenart geben Sie die nächste freie Nummer ein.
*Technische Info: Numerisches Feld, DB-Feld: kart.kartnr*

**Spr**
Sprachkennzeichen.
*Technische Info: <F9>, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Bezeichnung der Kostenart.
*Technische Info: Alphanumerisches Feld, DB-Feld: kart.bez*

**Hpt. K-Art**
Hier erfolgt die Zuordnung der Kostenart zur Hauptkostenart.
*Technische Info: Numerisches Feld, DB-Feld: kart.hkart*

### Kostenträger
Stammdaten > Kostenstamm > Kostenträger > Einzelne Bezeichnung
Stammdaten > Kostenstamm > Kostenträger > Alle Bezeichnung

*Abb. B-250 Kostenträger*

Produkte verursachen Kosten, die über Kostenträger verbucht werden.
Hier können sämtliche Kostenträger mit ihrer Bezeichnung und Angabe des übergeordneten Kostenträgers tabellarisch eingetragen werden. Über die Hauptkostenart ist dabei eine Zusammenfassung bestimmter Kostenarten möglich.

> **Mehrsprachige Bezeichnungen**
> Seit QR2209 können Sie in A+W Enterprise auch für Kostenträger mehrsprachige Bezeichnungen hinterlegen.

#### Erläuterung der Felder

**K-Träger**
Anzeige der Schlüssel-Nummer. Zum Anlegen eines neuen Kostenträgers wählen Sie den nächsten freien Eintrag.
*Technische Info: Alphanumerisches Feld, DB-Feld: ktr.ktrnr*

**Spr**
Sprachkennzeichen.
*Technische Info: <F9>, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Bezeichnung des Kostenträgers.
*Technische Info: Alphanumerisches Feld, DB-Feld: ktr.bez*

**Hpt-Träger**
Hier erfolgt die Zuordnung des Kostenträgers zum Hauptkostenträger.
*Technische Info: Numerisches Feld, DB-Feld: ktr.hktr*

### Kostenstellen
Stammdaten > Kostenstamm > Kostenstellen > Kostenstellen
Stammdaten > Kostenstamm > Kostenstellen > Einzelne Bezeichnung
Stammdaten > Kostenstamm > Kostenstellen > Alle Bezeichnung

*Abb. B-251 Kostenstellen*

Alle Stellen im Unternehmen, die durch die Leistungserstellung und Verwertung Kosten verursachen, werden als Kostenstelle bezeichnet. Von den Kostenstellen her ist eine verursachungsgerechte Zuteilung dieser Kosten auf die Kostenträger und damit eine kostengerechte Preisfestsetzung gewährleistet.
Die Kostenstelle sowie die Bezeichnung und die Angabe der übergeordneten Kostenstelle sind hier tabellarisch aufgelistet. Über das Feld Hauptkostenstelle ist eine Gliederung von Kostenstellen möglich.

> **Mehrsprachige Bezeichnungen**
> Seit QR2209 können Sie in A+W Enterprise auch für Kostenstellen mehrsprachige Bezeichnungen hinterlegen.

#### Erläuterung der Felder

**Kostenstelle**
Anzeige der Schlüssel-Nummer. Zum Anlegen einer neuen Kostenstelle geben Sie die nächste freie Nummer ein.
*Technische Info: Alphanumerisches Feld, DB-Feld: kstelle.kostenst*

**Bezeichnung**
Bezeichnung der Kostenstelle.
*Technische Info: Alphanumerisches Feld, DB-Feld: kstelle.bez*

**Hauptkostenstelle**
Hier erfolgt die Zuordnung der Kostenstelle zur Hauptkostenstelle.
*Technische Info: Numerisches Feld, DB-Feld: kstelle.hkst*

**HK-Elementnr.**
Herstellkosten-Elementnummer.
*Technische Info: Numerisches Feld, DB-Feld: kstelle.hkelemnr*

**Spr**
Sprachkennzeichen.
*Technische Info: <F9>, DB-Feld: xsprbez.sprkz*

## Preise
Die differenzierten Methoden der Flachglasbrache im Bereich Preisfindung sind sehr umfangreich und werden daher detailliert im Kapitel Preise + Konditionen beschrieben.

## Konditionen
Die Konditionspflege ist sehr eng mit der Preispflege verknüpft. Aus diesem Grund wird sie detailliert im Kapitel Preise + Konditionen beschrieben.

## Listendruck
Häufig benötigte Listen im Bereich der Stammdaten werden über den Listendruck erzeugt. Der Listendruck ist aus verschiedenen Programmbereichen anwählbar und ist in einem separaten Dokument beschrieben.

---

# C A+W Enterprise - Preise und Konditionen

### Revisionsübersicht des Moduls
| Datum | Änderung |
| :--- | :--- |
| 02-2023 | Div. Feldbeschreibungen aktualisiert |
| 05-2019 | Vollständige Überarbeitung der Softwarereferenz |
| 07-2018 | Ersterstellung Tutorial. |
| 01-2017 | Produkt- und Firmennamen angepasst. |
| 10-2016 | Preise und Konditionen aus Part Stammdaten ausgegliedert. |

**Zu diesem Modul finden Sie folgende Kapitel:**
- ⇨ Tutorial
- ⇨ Softwarereferenz

## Tutorial

### In diesem Kapitel finden Sie folgende Themen:
- ⇨ Einführung
- ⇨ Grundgedanken der Preisermittlung
- ⇨ Preisdefinitionen
- ⇨ Stammdaten für Preise
- ⇨ Konditionen
- ⇨ Stammdaten für Konditionen
- ⇨ Kostenkalkulation

| Thema | Seite |
| :--- | :--- |
| **Einführung** | C-536 |
| Menü-Übersicht | C-538 |
| **Grundgedanken der Preisermittlung** | C-539 |
| Charakteristika von Preisen und Konditionen | C-541 |
| Preisberechnung im Auftrag | C-542 |
| Artikelstammdaten | C-543 |
| ISO- und PKZ-Preise | C-544 |
| **Preisdefinitionen** | C-546 |
| Preisschlüssel | C-547 |
| Preislistenkennzeichen (PLKZ) | C-548 |
| Preiskennzeichen (PKZ) | C-549 |
| Preisschlüssel für Matrizen, Vektoren und Listen | C-553 |
| Preisschlüssel für Sprossen | C-555 |
| Währungen | C-556 |
| PLKZ-Logiken | C-558 |
| Ab-PLKZ-Logik | C-560 |
| Nur-PLKZ Logik | C-561 |
| Basis-PLKZ mit Ab-PLKZ-Logik | C-562 |
| Basis-PLKZ ohne Ab-PLKZ-Logik | C-562 |
| Preislistensteuerung | C-563 |
| Komponenten der Preisberechnung | C-566 |
| Preismethoden | C-567 |
| Rundungsmethoden (Preisberechnung) | C-568 |
| Preisrelevante Menge | C-571 |
| Preisarten | C-572 |
| Preistyp | C-574 |
| Mengenberechnung nach GME | C-575 |
| Schlüssel anlegen | C-577 |
| Übungen | C-579 |
| **Stammdaten für Preise** | C-580 |
| Workflow: Preise anlegen | C-581 |
| Preismatrizen für ISO-Scheiben | C-582 |
| Matrix-Editor | C-584 |
| Preismatrix für ISO-Scheiben anlegen | C-588 |
| Grundpreise für ISO-Scheiben | C-593 |
| Übungen | C-595 |
| Preisvektoren | C-596 |
| Vektorpreise | C-598 |
| Vektorzuordnung | C-602 |
| Artikelpreise anlegen | C-603 |
| Bearbeitungspreis anlegen | C-609 |
| Grundpreise für VSG-Scheiben | C-612 |
| Übungen | C-613 |
| Austausch- und Zusatzpreise | C-614 |
| Austausch-/Zusatzlisten | C-615 |
| Austauschpreise für Gussglas | C-617 |
| Austauschpreise anlegen | C-619 |
| Sprossenpreise | C-626 |
| Definitionsschema für Sprossenpreise | C-627 |
| Sprossenpreis anlegen | C-629 |
| Zuschläge | C-632 |
| Zuschlagsarten | C-633 |
| Modellzuschläge | C-633 |
| Zuschlagsmatrix | C-636 |
| Größenzuschläge | C-638 |
| Bearbeitungsgruppenzuschläge | C-641 |
| Stufenzuschläge | C-642 |
| Übungen | C-643 |
| Globale Preisänderungen | C-644 |
| **Konditionen** | C-645 |
| Prioritäten der Konditionsermittlung | C-646 |
| Komponenten der Konditionen | C-650 |
| **Stammdaten für Konditionen** | C-652 |
| Allgemeine und spezielle Konditionen | C-653 |
| Allgemeine Tageskonditionen | C-655 |
| Warengruppen-Konditionen | C-658 |
| Artikelkonditionen | C-660 |
| Rabattstaffeln | C-661 |
| Spezielle Faktoren | C-662 |
| Zuschläge für Modelle, SZR | C-665 |
| SZR-Zuschläge anlegen | C-666 |
| Spezielle Preise | C-669 |
| Spezielle Preise für Artikel und Farbartikel | C-671 |
| Spezielle Preise für ISO-Einzelscheibenpreise | C-672 |
| Komplexübung | C-675 |
| **Kostenkalkulation** | C-676 |
| Materialkosten | C-678 |
| Zusammenhang von Beschaffungsart und Kostenkalkulation | C-681 |

## Einführung
Das Tutorial zum Modul Preise und Konditionen beschäftigt sich mit den Grundlagen der Preisberechnung in A+W Enterprise. Das Tutorial baut auf den Kenntnissen zu den Artikel-Stammdaten auf.

> **Funktionen sind von den freigeschalteten Modulen abhängig**
> Bitte beachten Sie, dass die unterschiedlichen Funktionen nur dann zur Verfügung stehen, wenn die zugehörigen Module und Schnittstellen freigeschaltet sind.
> Wenn Sie in dieser Beschreibung Funktionen finden, die in Ihrer Installation nicht zugänglich sind, wenden Sie sich bitte an die A+W Software GmbH.

### Themenblöcke
In diesem Tutorial finden Sie folgende Themenblöcke:
- "Grundgedanken der Preisermittlung" auf Seite C-539
- "Preisdefinitionen" auf Seite C-546
- "Stammdaten für Preise" auf Seite C-580
- "Konditionen" auf Seite C-645
- "Stammdaten für Konditionen" auf Seite C-652
- "Kostenkalkulation" auf Seite C-676

### Vorausgesetzte Kenntnisse
Das Tutorial richtet sich an Anwender, die in A+W Enterprise die Stammdaten für die Preisberechnung verwalten.
Die Teilnehmer müssen das Konzept der allgemeinen Stammdaten und die Bedienelemente kennen, mit denen Funktionen aufgerufen und gestartet werden. Die Grundlagen der Bedienung sind im Part Überblick beschrieben.

### Ziel des Tutorials
- Unterschied zwischen Preisen und Konditionen verstehen.
- Preise und Konditionen in den Stammdaten bearbeiten und definieren.
- Preisermittlung der Auftragserfassung nachvollziehen.

### Aufbau des Tutorials
Das Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

**Überblick**
Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
- **Lernziele**: Was soll vermittelt werden?
- **Nutzen**: Wofür können Sie dieses Wissen einsetzen?
- **Merksätze**: Welche Zusammenhänge müssen Sie sich merken?

**Konzepte**
Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.

**Übungen**
Zu einigen Lerneinheiten finden Sie Übungen, mit denen Sie die beschriebenen Handlungssequenzen anwenden können.

#### Lesehinweis
Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.
Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.
Beachten Sie auch, dass die einzelnen Dialoge in der Softwarereferenz beschrieben sind. Auf diese Beschreibungen wird nicht im Einzelnen hingewiesen.

### Menü-Übersicht
In diesem Abschnitt finden Sie eine kurze Übersicht über die Programmbereiche, die in den Themenblöcken dieser Schulung angesprochen werden.

*Abb. C-1 Menüs Preise, Konditionen*

#### Preise
Über dieses Menü erreichen Sie alle Dialoge, in denen Sie die Daten für die Preise festlegen:
- **a - d**: Über diese Menüpunkte erreichen Sie die Dialoge, in denen Sie die Preise und Zuschläge anlegen.
- **e - g**: Über diese Menüpunkte erreichen Sie die Dialoge, in denen Sie die Schlüssel und die Preissteuerung definieren.
- **h**: Über diesen Menüpunkt erreichen Sie den Dialog zu Auswahl der Liste, die gedruckt werden soll.

#### Konditionen
Über dieses Menü erreichen Sie alle Dialoge, in denen Sie die Konditionen für die Berechnung der Preise festlegen:
- **a**: Über diesen Menüpunkt erreichen Sie die Dialoge, in denen Sie die allgemeinen Tageskonditionen und die Warengruppenkonditionen anlegen.
- **b**: Über diesen Menüpunkt erreichen Sie die Dialoge, in denen Sie die speziellen Konditionen anlegen.
- **c**: Über diesen Menüpunkt erreichen Sie die Dialoge, in denen Sie spezielle Preise anlegen.

## Grundgedanken der Preisermittlung
Die Preisberechnung in A+W Enterprise berücksichtigt neben den festen Artikelpreisen auch Abweichungen, z. B. den Austausch eines Glases in einem ISO-Artikel oder zusätzliche Bearbeitungen. Um alle Möglichkeiten abzudecken, stehen verschieden Bausteine zur Verfügung, die automatisch herangezogen werden, z. B. die Preise für die Glasartikel, besondere Zuschläge oder Nachlässe usw.
Ziel dieses Tutorials ist, die Zusammenhänge von Artikel-Stammdaten, Preisen und Konditionen zu erklären.
Im Auftrag kann eine Position mit einem mehr oder weniger komplexen Stücklistenaufbau erfasst werden, ohne dass die Preise für die Komponenten einzeln angegeben werden müssen.

*Abb. C-2 Schematischer Aufbau einer einfachen ISO-Scheibe*

In diesem vereinfachten Beispiel sehen Sie den Stücklistenaufbau für eine ISO-Scheibe. Wie der Preis für eine solche Position im Auftrag zustande kommt, wird in den folgenden Kapiteln erklärt.

### Glossar

| Begriff | Erklärung |
| :--- | :--- |
| **Matrix** | Zweidimensionale Preistabelle mit einer Matrixnummer, einer Bezeichnung und den Werten für die Preise. Die Preise sind von Höhe und Breite abhängig. ⇨ "Matrix-Editor" auf Seite C-584 |
| **Vektor** | Eindimensionale Preistabelle mit einer Vektornummer, einer Bezeichnung und den Werten für die Preise. Die Preise sind z. B. von der Stückzahl oder der Fläche abhängig. ⇨ "Vektorzuordnung" auf Seite C-602 |
| **PKZ** | PreisKennZeichen. Das (logische) Preiskennzeichen ist ein Link zu einem PLKZ. ⇨ "Preiskennzeichen (PKZ)" auf Seite C-549 |
| **PLKZ** | PreisListenKennZeichen. Das Preislistenkennzeichen ist eine physikalische Preisliste, die eine beliebige Anzahl von Matrizen und Vektoren enthält. ⇨ "Preislistenkennzeichen (PLKZ)" auf Seite C-548 |
| **Preisschlüssel** | Preisschlüssel sind Nummern und Bezeichnungen für Listen, Matrizen und Vektoren. ⇨"Preisschlüssel" auf Seite C-547 |
| **Preismethoden** | Die Preismethode steuert, wie der Preis für den im Auftrag oder in der Bestellung erfassten Artikel berechnet wird. ⇨ "Preismethoden" auf Seite C-567 |
| **Positionsartikel** | Der Positionsartikel ist ein Artikel, der im Auftrag oder in der Bestellung erfasst ist, z. B. ein VSG-Artikel. Zu diesem Artikel wird der Preis berechnet. Er kann eine Stückliste enthalten. |
| **PLKZ-Logik** | Die PLKZ-Logik legt fest, wie nach Preisen in den Preislisten gesucht werden soll. ⇨ "PLKZ-Logiken" auf Seite C-558 |
| **Artikel** | Alle Artikel sind in den Stammdaten angelegt, z. B. Float 4 mm, ISO 2 x 5 mm, Säumen. |
| **Glas** | Das Glas ist immer das Material einer Einzelscheibe, z. B. Drahtglas, Float. |
| **Scheibe** | Scheiben werden in der Auftragsposition erfasst, und genau für diese wird der Preis berechnet. |

### Charakteristika von Preisen und Konditionen
*Abb. C-3 Preis*

Die Preise sind immer den Artikeln zugeordnet. Sie werden jedoch nicht direkt mit den Artikeln in den Stammdaten des Artikels erfasst, sondern in separaten Matrizen, Artikelvektoren, Bearbeitungsvektoren und Austauschlisten, die den Artikeln zugeordnet werden.

*Abb. C-4 Konditionen*

Konditionen sind Marktpartnern, Kundengruppen oder Objekten zugeordnet und sind hierarchisch aufgebaut. Sie sind über ein Kennzeichen mit den Preisen verknüpft.

### Preisberechnung im Auftrag
Im Auftrag werden Produkte erfasst, zu denen ein Preis berechnet wird. Ein Produkt kann eine Stückliste mit Artikeln enthalten. In der Regel haben Standardaufbauten einen Preis, in dem Preise für die Stücklistenartikel schon enthalten sind.
Zusätzlich können Konditionen definiert werden, in denen aktuelle Abweichungen für die Preisberechnung festgelegt sind, z B. Aufschläge auf bestimmte Warengruppen oder Sonderpreise für bestimmte Marktpartner.

*Abb. C-5 Zuordnungen für die Preisfindung*

In dieser vereinfachten Darstellung sehen Sie, wie die Preise über die Zuordnungen von Artikeln und Marktpartnern für die Berechnung von Auftragspositionen zusammengeführt werden.
Für die Preisberechnung sucht A+W Enterprise nach dem Preis für das Produkt oder nach den Preisen für die Stücklistenartikel. Dabei werden auch Austauschgläser, Zusätze und Bearbeitungen berücksichtigt. Anschließend werden die aktuellen Konditionen durchsucht. Aus den Resultaten dieser Suchen wird dann der Preis berechnet.
Im Auftrag selbst können Sie diesen Preis pro Artikel, Position oder insgesamt manuell ändern. Zusätzlich können Sie im Auftrag auch die Konditionen ändern.

**Beispiel**
`+ Preis für den Positionsartikel, z. B. ISO 2 x 5 mm - Preis pro qm.`
`Preis für Unterteile mit Austausch-/Zusatz-Flag, z. B. Austauschgläser, Zubehörartikel und Bearbeitungen.`
`= Preis des Produkts`

### Artikelstammdaten
In den Stammdaten der Artikel muss die Preismethode angegeben sein.

*Abb. C-6 Preisrelevante Einstellungen in den Artikelstammdaten*

| Kürzel | Beschreibung |
| :--- | :--- |
| A | Preiseigenschaften für Bearbeitungen, Zubehör |
| B | Preismethode |
| C | Preishistorie (kundenspezifisch) |
| D | Preisdarstellung für den Formulardruck |
| E | Kostenkalkulation |
| F | Skontierbar |
| G | Materialverlust (Kostenkalkulation) |
| H | Korrekturfaktor (Kostenkalkulation) |
| I | Standardpreis (kundenspezifisch) |
| J | Preistyp (kundenspezifisch) |

Pro Artikel geben Sie neben der Preismethode (B) an, ob auf den Preis Skonto gewährt werden kann (F).
⇨ "Preismethoden" auf Seite C-567

Wenn Sie mit dem Modul Kostenkalkulation arbeiten, können Sie festlegen, ob der Artikel bei der Kostenkalkulation (E) herangezogen wird und/oder wie die Kosten für den Artikel kalkuliert werden.
Die Kostenkalkulation ist in einem separaten Part beschrieben.
⇨"Kostenkalkulation" auf Seite C-676

Die Preiseigenschaften für Bearbeitungen und Zubehör (A) finden Sie unter: Artikel > <F4> > Preiseigenschaften. Diese Einstellungen werden nur ausgewertet, wenn der Artikel als Unterteil verbaut wird.
Die Preiseigenschaften können Sie für den Artikel, den Artikeltypen, den A+W-Bearbeitungstypen oder eine Kombination aus Artikel und A+W-Bearbeitungstyp festlegen.
Wenn dem Artikel ein A+W-Bearbeitungstyp zugeordnet ist, kann kein Satz für den Artikeltypen angegeben werden. Die Preiseigenschaften werden dann in dieser Reihenfolge ausgewertet:
- Artikel
- Artikel und A+W Bearbeitungstypen
- A+W Bearbeitungstypen

Wenn dem Artikel kein A+W-Bearbeitungstyp zugeordnet ist, kann nur ein Satz für den Artikel oder den Artikeltypen angegeben werden.
Eine ausführliche Beschreibung der Dialoge finden Sie im Part Stammdaten.

### ISO- und PKZ-Preise
- A+W Enterprise unterscheidet bei der Preisberechnung zwischen ISO-Artikeln und anderen Gläsern.
- Nicht-ISO-Gläser und Bearbeitungen erhalten normalerweise Preisvektoren.
- Preise für ISO-Scheiben können nach drei verschiedenen Methoden definiert werden: in Preismatrizen, in Vektoren oder als Einzelscheiben.
- Austauschlisten gibt es nur für ISO- und VSG-Scheiben.

*Abb. C-7 ISO- und PKZ-Preise*

Für die exakte Berechnung einer Scheibe wirken verschiedene Preisdefinitionen zusammen. Für Sonderanfertigungen werden jedoch Zuschläge erhoben, die den Artikeln zugeordnet sind, z. B. für Bearbeitungen an den Ecken und/oder Kanten, für Übergrößen, für kleine Scheiben. Das bedeutet, dass alle Elemente, die im Auftrag in der Stückliste erfasst werden können, einen Preis haben können.

## Preisdefinitionen
In diesem Themenblock lernen Sie, wie mit welchen Komponenten die Preise in A+W Enterprise definiert sind.
Zu den Komponenten gehören die „Werkzeuge" oder Schlüssel, die Preissteuerung und die Preise selbst.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Preisschlüssel" auf Seite C-547
- "PLKZ-Logiken" auf Seite C-558
- "Komponenten der Preisberechnung" auf Seite C-566

### Preisschlüssel

**Lernziele**
- Unterschied zwischen Preisschlüsseln und Preisdefinitionen kennenlernen.
- Funktion der Preisschlüssel kennenlernen.
- Nutzen von PKZ und PLKZ verstehen.
- Währungen

**Nutzen**
- Die Stammdaten für die Preisberechnung werden in zwei Schritten definiert. Sie können z. B. eine Preismatrix nur mit Preisen füllen, wenn Sie zuvor einen Schlüssel für diese neue Matrix hinterlegt haben.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **PLKZ** | Das PLKZ ist eine (physikalische) Preisliste, in der eine beliebige Anzahl von Preismatrizen und Preisvektoren zusammengefasst sind, z. B. alle Preislisten, die für die Berechnung von ISO-Scheiben einschließlich Austausch und Bearbeitungen gelten.<br>- Die Preislistennummer ist die numerische Bezeichnung einer Preisliste.<br>- Das PLKZ ist durch eine Nummer, eine Bezeichnung und eine Währung definiert.<br>- Die PLKZ werden verwendet, um Preislisten zu sortieren.<br>- Die Nummerierung ist aufsteigend. |
| **PKZ** | Das (logische) Preiskennzeichen (PKZ) ist ein Link zu einer physikalischen Preisliste (PLKZ), mit dem die Preisliste einem Marktpartner zugewiesen wird. |
| **Preisschlüssel** | Preisschlüssel sind Nummern und Bezeichnungen für alle Listen, Matrizen und Vektoren. |
| **Matrixnummer** | Die Matrixnummer ist eine Schlüsselnummer und Bezeichnung, der eine zweidimensionale Preistabelle, die Matrix, zugeordnet wird. |
| **Vektornummer** | Die Vektornummer ist eine Schlüsselnummer und Bezeichnung, der eine eindimensionale Preistabelle zugeordnet wird. Schlüssel für Vektoren werden getrennt angelegt:<br>- Artikel<br>- Bearbeitungen. |
| **Sprossenzuordnung** | Zur Berechnung von Sprossenartikeln werden Sprossenpreisklassen und Sprossenkennzeichen einander zugeordnet. |
| **Währung** | Preise in unterschiedlichen Währungen können nur verwendet werden, wenn die Mehrwährungsfähigheit konfiguriert ist. |

### Preislistenkennzeichen (PLKZ)
Das Preislistenkennzeichen ist eine (physikalische) Preisliste, in der eine beliebige Anzahl von Preismatrizen und Preisvektoren zusammengefasst sind, z. B. alle Preislisten, die für die Berechnung von ISO-Scheiben einschließlich Austausch und Bearbeitungen gelten. Das PLKZ selbst enthält keine Preise.

- Das PLKZ ist durch eine Nummer, eine Bezeichnung und eine Währung definiert.
- Die PLKZ werden verwendet, um Preislisten zu sortieren.
- Die Nummerierung ist aufsteigend.

Damit die Suche nach einem Preis fehlerfrei funktioniert, sollten Sie Nummernkreise für die einzelnen Preislisten/Glasarten festlegen, z. B. 1000 - 1999 für Float, 2000 - 2999 für Gussglas usw.

*Abb. C-8 Preislistenkennzeichen und Nummernkreis*

| Kürzel | Beschreibung |
| :--- | :--- |
| A | Nummernkreis |
| B | Unterstes PLKZ im Nummernkreis |
| C | Höchstes PLKZ im Nummernkreis |
| D | Nummer des PLKZ |
| E | Währung |

Die Nummernkreise (A) spielen eine entscheidende Rolle bei der Logik der Preisfindung. Diese Logik ist in einer separaten Lerneinheit ausführlich beschrieben.
⇨ "PLKZ-Logiken" auf Seite C-558

Bevor Sie irgendeinen Preis festlegen können, müssen Sie das PLKZ festlegen, zu dem der Preis gehören soll. Da das PLKZ auch bei der Ermittlung von EK-Preisen herangezogen wird, sollten Sie die PLKZ-Nummern für EK und VK getrennt führen.

> **Für jede Währung eine eigene Preisliste**
> Wenn Sie in Ihrem Unternehmen Preise in unterschiedlichen Währungen verwenden, müssen Sie für jede Währung eigene Preislisten anlegen.
> In der Vorgangserfassung wird geprüft, ob die Währung des Marktpartners und die Währung der Preisliste übereinstimmen. Ist dies nicht der Fall, wird eine Meldung angezeigt. Die Preise aus der Preisliste werden aber nicht in die Währung des Marktpartners umgerechnet.

Wenn Sie ein PLKZ anlegen, müssen Sie auf Folgendes achten, damit mit der Ab-PLKZ-Logik gearbeitet werden kann:
- Die Preislisten müssen in Gruppen sortiert sein, z. B. nach VK, EK.
- Die Verkaufs-Preislisten müssen sich in einem dafür vorgesehenen Nummernkreis befinden, z. B. PLKZ 1*** bis 3***. Im jeweiligen Nummernkreis müssen die Preislisten numerisch aufsteigend angelegt sein.
- Die Einkaufs-Preislisten müssen sich in einem dafür vorgesehenen Nummernkreis befinden, z. B. PLKZ 4*** bis 6***.
- Jede Fremdwährung muss ebenfalls einen eigenen Nummernkreis haben.
- Eine neuere Preisliste muss immer eine höhere Nummer (PLKZ) haben als die Vorgängerpreisliste. Die Nummerierung muss jedoch nicht lückenlos sein.

### Preiskennzeichen (PKZ)
Die Abkürzung PKZ steht für PreisKennZeichen. Hierunter sind Preisgenerationen zu verstehen, die in Form von Preislisten angelegt sind. Das (logische) PKZ ist ein Zeiger auf eine physikalische Preisliste (PLKZ), mit dem die Preisliste einem Marktpartner zugeordnet ist.
Das PKZ enthält keine Preisdaten es stellt aber die Verknüpfung zwischen der Preisliste und den aktuellen Konditionen her, ohne die kein Preis berechnet werden kann.

*Abb. C-9 Zuordnung von PKZ und PLKZ*

In dieser Darstellung sehen Sie, dass von einem PKZ auf ein PLKZ verwiesen wird. Das PKZ macht die Zuordnung von Marktpartnern und Preisliste zweistufig.

Wenn Sie eine neue Preisliste angelegt haben oder wenn die Preise eines Marktpartners nach einer anderen Preisliste berechnet werden sollen, muss bei dieser zweistufigen Zuordnung nur das PKZ geändert werden. Um die Preisfindung zu ändern, haben Sie also folgende Möglichkeiten:
- In den allgemeinen Konditionen geben Sie für den Marktpartner ein anderes PKZ an.
- Ein (neues) PKZ wird einem neuen PLKZ zugeordnet.

*Abb. C-10 Zuordnung von PKZ und PLKZ*

In diesem Beispiel sehen Sie, dass dem Kunden genau 1 PKZ zugeordnet ist, aber einem PKZ mehrere Kunden zugeordnet sein können (n:1). Jedes PKZ verweist jeweils auf genau eine Preisliste (PLKZ).
Das bedeutet, dass die Kunden A, B und F die Preise aus PLKZ 100 erhalten. Die Kunden C und D erhalten die Preise aus PLKZ 200 und Kunde F aus PLKZ 300.
Für das kommende Jahr sollen die alten ISO-Preise angepasst werden. Dazu wird eine neue Preisliste mit dem PLKZ 400 angelegt. Die neuen Preise werden noch nicht zur Berechnung von Aufträgen herangezogen und können daher in Ruhe vorbereitet werden.

*Abb. C-11 Zuordnung umgehängt*

Ab einem definierten Zeitpunkt wird nun das PKZ auf die neue Preisliste umgehängt.
Die Zuordnung muss nur für das PKZ geändert werden, in den Kundendaten und in den Konditionen muss nichts angepasst werden.
Von nun an erhalten die Kunden A, B und F die Preise aus PLKZ 400. Für alle anderen Kunden ändert sich dadurch nichts.
Für diese Zuordnungen stehen die Dialoge Preislistenreferenz und Allgemeine Tageskonditionen zur Verfügung.

*Abb. C-12 PKZ-PLKZ-Zuordnung und Tageskonditionen*

| Kürzel | Beschreibung |
| :--- | :--- |
| A | PKZ verweist auf PLKZ |
| B | PLKZ, auf das verwiesen ist |
| C | PKZ pro Preismethode |
| D | Kundennummer |

Erst wenn Sie in den Allgemeinen Tageskonditionen angegeben haben, welches PKZ für die jeweilige Berechnungsmethode gilt, können die Preislisten und daraus die Preise ermittelt werden.
In der Lerneinheit zu den Konditionen werden Sie erfahren, wie Sie diese Zuordnungen auch für einzelne Marktpartner steuern können.
⇨ "Allgemeine und spezielle Konditionen" auf Seite C-653

#### Vorteile der Trennung von PLKZ und PKZ
Durch die Trennung von PLKZ und PKZ haben Sie folgende Vorteile:
- Sie können Preislisten vorab ohne Zeitdruck erfassen.
- Sie können alle entsprechenden Preislisten zu einem bestimmten Zeitpunkt gemeinsam aktivieren.
- Sie können sehr einfach auf alte Preislisten zurückgreifen.
- Sie müssen bei Preisänderungen die Konditionen von Marktpartnern nicht unbedingt anpassen.

### Preisschlüssel für Matrizen, Vektoren und Listen
Bevor Sie Preise erfassen, müssen Sie die notwendigen Schlüssel anlegen. Das sind spezielle Kennzeichen für die Matrix- und Vektorpreise und für einfache Preislisten.

| Kennzeichen für | Beschreibung |
| :--- | :--- |
| **Matrizen** | Die Matrixnummer ist eine Schlüsselnummer und Bezeichnung, der eine zweidimensionale Preistabelle, die Matrix, zugeordnet wird. |
| **Vektoren** | Die Vektornummer ist eine Schlüsselnummer und Bezeichnung, der eine eindimensionale Preistabelle zugeordnet wird. Schlüssel für Vektoren werden getrennt angelegt: - Artikel - Bearbeitungen |
| **Austausch-/ Zusatzlisten** | Die Listennummer ist eine Schlüsselnummer und Bezeichnung, der eine Preisliste für Artikel zugeordnet wird, die in der Stückliste ausgetauscht oder zusätzlich eingebaut werden. |

Diese Schlüssel werden jeweils in einem eigenen Dialog hinterlegt.

*Abb. C-13 Dialoge zur Hinterlegung der Preisschlüssel*

| Kürzel | Beschreibung |
| :--- | :--- |
| A | Matrixnummer |
| B | Vektornummer |
| C | Listennummer |
| D | Definition: Master-Liste |

#### Master-Liste für Austausch-/Zusatzlisten
Bei den Listennummern für Austausch-/Zusatzlisten müssen Sie angeben, ob die Liste als Master-Liste gelten soll. Aus der Master-Liste wird z. B. der Austauschpreis ermittelt, wenn in der Austauschliste, die dem Positionsartikel zugeordnet ist, kein Austauschpreis gefunden wird.

#### Verknüpfung der Schlüssel
Die Schlüssel, die Sie für die Vektoren, Matrizen und Austausch-/Zusatzlisten definiert haben, benötigen Sie zusammen mit den Preislistenschlüsseln, um eine Preismatrix, einen Preisvektor oder eine Preisliste anzulegen.
Wenn Sie z. B. die Preise für einen Matrix-Preis anlegen, geben Sie die Schlüsselnummer der Matrix und der Preisliste an.

*Abb. C-14 Zuordnung von Preisschlüssel und Preisliste*
- **A Matrix: Schlüssel und Preisdefinition**
- **B Preisliste: Schlüssel und Preisdefinition**

Auf die gleiche Weise verwenden Sie auch die Schlüsselnummern für Vektor- und Austauschpreise.

**Ergänzende Informationen**
- ⇨ "Preismatrizen für ISO-Scheiben" auf Seite C-582
- "Preisvektoren" auf Seite C-596
- ⇨ "Austausch- und Zusatzpreise" auf Seite C-614

### Preisschlüssel für Sprossen
Zur Berechnung von Sprossenartikeln werden Sprossenpreisklassen und Sprossenkennzeichen verwendet.
- Dem Schlüssel Sprossenpreisklasse ordnen Sie alle Sprossen zu, die zu denselben Preisen berechnet werden.
- Dem Schlüssel Sprossenkennzeichen ordnen Sie die Währung zu, in der die Sprossenpreise berechnet werden sollen.

*Abb. C-15 Definitionen von Sprossenpreisen*

*Abb. C-16 Schlüssel für Sprossenpreise*
- **A Sprossenpreisklasse (SP-Klasse)**
- **B Sprossenpreiskennzeichen (S-PKZ)**

Im Schlüssel für das Sprossenkennzeichen ist die Währung zugeordnet.
Wenn Sie mit mehreren Währungen arbeiten, müssen Sie für jede Währung eigene Preislisten anlegen.

### Währungen
In einer Systemkonfiguration mit mehreren Währungen können Sie die Preise in unterschiedlichen Währungen pflegen und bearbeiten. Dazu müssen die Währungen angelegt sein, in denen Preislisten geführt werden sollen. Die Währungen legen Sie in den Stammdaten an.
⇨ Stammdaten, "Währung" auf Seite B-274

*Abb. C-17 Währungen*

| Kürzel | Beschreibung |
| :--- | :--- |
| A | Nummer der Währung |
| B | Kürzel |
| C | Wechselkurs |
| D | Nachkommastellen für die Rundung und Rundungsrichtung |

Wenn Sie nicht mit mehreren Währungen arbeiten, muss mindestens die Landeswährung angelegt sein.
Zu jeder Währung geben Sie eine Nummer, das Kürzel und den Kurs (C) an. Außerdem müssen Sie festlegen, wie die errechneten Beträge (D) gerundet werden sollen.

**Beispiel**

| Währung | Nachkommstellen | Rundung | Beträge |
| :--- | :--- | :--- | :--- |
| Euro | 2 Nachkommstellen | auf 0,01 | 179,321 -> 179,33 |
| SFr | 2 Nachkommstellen | auf 0,05 | 179,321 -> 179,35 |
| CAD | 2 Nachkommstellen | ab 0,10 | 179,321 -> 179,30 |

In diesem Beispiel sehen Sie, dass die Währungen mit 2 Nachkommstellen gerechnet werden. Bei den Preisen in Euro werden die errechneten Ergebnisse auf die 2. Nachkommastelle aufgerundet, bei den Schweizer Franken wird auf 0,05 SFr aufgerundet, bei den Kanadischen Dollar wird auf 0,10 abgerundet.
Wenn Sie keine kleinste Währungseinheit eintragen, wird die Währung mit 2 Nachkommastellen gerechnet. Wenn Sie keine Angaben zur Rundung hinterlegen, wird die Währung kaufmännisch gerundet.

#### EK-Preisberechnung
Wenn in den Stammdaten eines Lieferanten angegeben ist, dass die Preise in Fremdwährung gerechnet werden, muss die Währung der zugeordneten Preisliste zwingend mit der Währung des Lieferanten übereinstimmen.
Wenn Sie in der Bestellverwaltung einen Artikel erfassen oder die EK-Preisliste ändern, wird geprüft, ob die Währung aus der Preisliste und die Währung aus den Lieferantenstammdaten übereinstimmen. Ist dies nicht der Fall, wird ein Hinweis angezeigt.
In der Auftragserfassung wird die Währungsverträglichkeit nicht geprüft.

### PLKZ-Logiken

**Lernziele**
- Auswertungslogik und Preislistensteuerung verstehen.
- Ab-PLKZ-Logik richtig einsetzen können.
- Nur-PLKZ-Logik verwenden.
- Unterschied von Basis-PLKZ mit Ab-PLKZ-Logik und Basis-PLKZ ohne Ab-PLKZ-Logik verstehen.

**Nutzen**
- Mit Hilfe der PLKZ-Logik können Preise für den Verkauf und für den Einkauf in unterschiedlichen Listen gepflegt werden.
- Mit den unterschiedlichen Vorgaben aus den Preiszuordnungen und mit den Zuschlägen können Preislisten sehr flexibel gestaltet werden.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **PLKZ** | Das PLKZ ist eine (physikalische) Preisliste, in der eine beliebige Anzahl von Preismatrizen und Preisvektoren zusammengefasst sind, z. B. alle Preislisten, die für die Berechnung von ISO-Scheiben einschließlich Austausch und Bearbeitungen gelten.<br>- Die Preislistennummer ist die numerische Bezeichnung einer Preisliste.<br>- Das PLKZ ist durch eine Nummer, eine Bezeichnung und eine Währung definiert.<br>- Die PLKZ werden verwendet, um Preislisten zu sortieren.<br>- Die Nummerierung ist aufsteigend. |
| **PKZ** | Das (logische) Preiskennzeichen (PKZ) ist ein Link zu einer physikalischen Preisliste (PLKZ), mit dem die Preisliste einem Marktpartner zugewiesen wird. |
| **PLKZ-Logik** | Preise können in einer anderen Preisliste gesucht werden, wenn im aktuellen PLKZ kein Preis gefunden wurde. Die konfigurierte PLKZ-Logik gilt für alle Dialoge in den Preisstammdaten und Konditionen, in denen ein Ab-PLKZ angegeben werden kann. Standardmäßig arbeitet A+W Enterprise mit der Ab-Logik. |
| **Preislisten-Steuerung** | Die Ab-PLKZ-Logik kann für einzelne Preislistenkennzeichen übersteuert werden. Die Übersteuerung gilt jeweils für alle Preissuchen, in denen das angegebene PLKZ eingetragen ist. |
| **Ab-PLKZ-Logik** | Wenn bei der Auftragserfassung für den Artikel kein Preis zum aktuellen PLKZ gefunden wird, ermittelt das Programm in numerischer Reihenfolge das vorausgehende PLKZ, zu dem ein Preis definiert ist. |
| **Nur-PLKZ-Logik** | Bei der Preisfindung wird der Preis nur aus dem angegebenen PLKZ ermittelt. |
| **Basis-PLKZ mit Ab-PLKZ-Logik** | Bei der Preisfindung wird zunächst das aktuelle PLKZ ermittelt. Danach wird geprüft, welche PLKZ-Logik angewendet werden soll, und die Suche wird bis zum Basis-PLKZ fortgesetzt. |
| **Basis-PLKZ ohne Ab-PLKZ-Logik** | Bei der Preisfindung wird zunächst das aktuelle PLKZ ermittelt. Danach wird geprüft, welche PLKZ-Logik angewendet werden soll und in dem PLKZ gesucht, das als Basis angegeben ist. |

#### Ab-PLKZ-Logik
A+W Enterprise arbeitet mit der Ab-PLKZ-Logik: Wenn bei der Auftragserfassung für den Artikel kein Preis zum aktuellen PLKZ gefunden wird, ermittelt das Programm in numerischer Reihenfolge das vorausgehende PLKZ, zu dem ein Preis definiert ist. Damit gilt der gefundene Preis ab diesem PLKZ.
Ein Preis wird also nicht nur in der Preisliste (PLKZ) gesucht, die über das PKZ zugeordnet ist. Wenn in diesem PLKZ kein Preis gefunden wurde, wird im numerisch nächstniedrigeren PLKZ gesucht.

*Abb. C-18 Aufsteigende PLKZ und Ab-PLKZ-Logik*

In diesen Beispielen sehen Sie, dass der Preis aus Vektoren so lange gilt, bis ein neuer Preis gefunden ist. Wenn also im PLKZ 2017 kein Preis gefunden wurde, wird die Suche im PLKZ 2016 fortgesetzt, danach im PLKZ 2015 und dann im PLKZ 2014.
Von dieser Ab-PLKZ-Logik können Sie im Dialog Preislistensteuerung für jedes einzelne PLKZ abweichen.
⇨ "Preislistensteuerung" auf Seite C-563

> **Ausnahme ISO-Matrizen**
> ISO-Matrizen sind von der Ab-PLKZ-Logik ausgenommen. Daher müssen die Preise komplett je PLKZ gepflegt werden.
> Für die 2. Matrize endet die Preissuche im PLKZ 2016 selbst dann, wenn bereits höhere Kennzeichen eingerichtet sind. Im Umkehrschluss heißt das, dass die Preise für die 2. Matrize für das PLKZ 2017 neu eingepflegt werden müssen. Dazu stehen Kopierfunktionen zur Verfügung.
> ⇨ Softwarereferenz, "Matrix-Übernahme" auf Seite C-730

**Vorteile der Ab-PLKZ-Logik**
Mit der Ab-PLKZ-Logik ergeben sich folgende Vorteile.
- Preise können nach Preislisten gruppiert werden, z. B. um EK-Listen von VK-Listen zu trennen.
- Sie müssen nicht immer alle Preise pro Preisliste erfassen, sondern nur die Änderungen.
- Sie können neue Preislisten während des normalen Tagesgeschäfts erfassen und zu einem späteren Zeitpunkt aktivieren.
- Sie können die Änderungen in der Preislistenhistorie verfolgen.

**Besonderheiten bei der Ab-PLKZ-Logik**
Bei der Ab-PLKZ-Logik gibt es Folgendes zu beachten:
- Mit dieser Logik kann auf Preislisten zugegriffen werden, die eventuell einer anderen Preislistengruppe zugeordnet sind oder in einer anderen Währung geführt werden. Deshalb ist es wichtig, die Nummernkreise einzuhalten, und im untersten PLKZ einer Gruppe sollten alle Preise komplett gepflegt sein.
- Im Auftrag können Sie nicht erkennen, wenn der Preis als Folge der Ab-PLKZ-Logik aus einem niedrigeren PLKZ ermittelt wurde.

### Nur-PLKZ Logik
Wenn Sie die Ab-PLKZ-Logik für ein bestimmtes PLKZ nicht verwenden wollen, müssen Sie für dieses PLKZ die Ab-PLKZ-Logik abschalten. Diese Einstellung legen Sie im Dialog Preislistensteuerung fest.

*Abb. C-19 Preislisten-Steuerung*

- **A** PLKZ, für das die Abweichung gilt
- **B** Dasselbe PLKZ soll verwendet werden
- **C** Ab-PLKZ-Logik gilt nicht

Für die Nur-PLKZ-Logik müssen Sie für das PLKZ (A) und das Basis-PLKZ (B) dieselbe Nummer angeben und im Feld ab-Logik (C) N (Nein) auswählen. Damit haben Sie die Ab-PLKZ-Logik für diese PLKZ deaktiviert.
Bei der Preisfindung in der Vorgangsverwaltung wird zunächst das aktuelle PLKZ ermittelt. Danach prüft A+W Enterprise, welche PLKZ-Logik (C) angewendet werden soll. Der Preis wird nur aus dem angegebenen PLKZ ermittelt. Wird in der angegebenen Preisliste kein Preis gefunden, wird ein entsprechender Hinweis angezeigt. Die Suche wird nicht in einem anderen PLKZ fortgesetzt.

### Basis-PLKZ mit Ab-PLKZ-Logik
Wenn Sie die Ab-PLKZ-Logik für einen bestimmten Nummernkreis begrenzen wollen, müssen Sie für dieses PLKZ die Ab-PLKZ-Logik übersteuern, z. B. für unterschiedliche Währungen.

*Abb. C-20 Preislisten-Steuerung*

- **A** PLKZ, für das die Abweichung gilt
- **B** Basis-PLKZ
- **C** Ab-PLKZ-Logik gilt

Zum aktuellen PLKZ (A) müssen Sie ein niedrigeres Basis-PLKZ (B) angeben und im Feld ab-Logik (C) J (Ja) auswählen.
Bei der Preisfindung in der Vorgangsverwaltung wird zunächst das aktuelle PLKZ ermittelt. Danach prüft A+W Enterprise, welche PLKZ-Logik angewendet werden soll. Wenn für den Artikel kein Preis im aktuellen PLKZ gefunden wird, ermittelt das Programm nur bis zum Basis-PLKZ zurück. Wird kein Preis gefunden, wird in der Vorgangsverwaltung ein entsprechender Hinweis angezeigt.

### Basis-PLKZ ohne Ab-PLKZ-Logik
Wenn Sie für ein bestimmtes PLKZ eine Ausweichpreisliste angeben wollen, müssen Sie für dieses PLKZ die Ab-PLKZ-Logik übersteuern.

*Abb. C-21 Preislisten-Steuerung*

- **A** PLKZ, für das die Abweichung gilt
- **B** PLKZ, auf das verwiesen ist
- **C** Ab-PLKZ-Logik gilt nicht

Zum aktuellen PLKZ (A) geben Sie ein niedrigeres Basis-PLKZ (B) an und wählen im Feld ab-Logik (C) N (Nein) aus.
Bei der Preisfindung in der Vorgangsverwaltung wird zunächst das aktuelle PLKZ ermittelt. Danach prüft A+W Enterprise, welche PLKZ-Logik angewendet werden soll und sucht in dem PLKZ, das als Basis angegeben ist. Wird in der angegebenen Preisliste kein Preis gefunden, wird in der Vorgangsverwaltung ein entsprechender Hinweis angezeigt.
Daher sollten Sie darauf achten, dass in dem Basis-PLKZ alle Preise angegeben sind.

### Preislistensteuerung
Da Sie in der Regel Preislistenkennzeichen über Jahrgänge hinaus auch für die unterschiedlichen Glasarten anlegen und pflegen, müssen Sie steuern, welches PLKZ zur Preisberechnung herangezogen werden soll.
Über die Preislistensteuerung wird eingestellt, aus welcher Preisliste ein Preis gezogen wird, wenn in der zugeordneten Preisliste kein Preis gefunden wurde.
Wenn in der Vorgangsverwaltung im Sinne der eingestellten PLKZ-Logik kein Preis gefunden wird, wird eine Fehlermeldung ausgegeben.
In fast allen Dialogen, die zur Preisfindung herangezogen werden, können Sie ein PLKZ angeben, ab dem der Preis gilt. Die Ab-PLKZ-Logik gilt für alle Dialoge getrennt, in denen ein Ab-PLKZ angegeben werden kann.
Die Ab-PLKZ-Logik kann in Einzelfällen übersteuert werden. Dazu steht der Dialog Preislistensteuerung zur Verfügung:

*Abb. C-22 Preislisten-Steuerung*

- **A** PLKZ, für das die Abweichung gilt
- **B** PLKZ, auf das verwiesen ist
- **C** Angabe zur Verwendung der Ab-PLKZ-Logik (J, N)

In diesem Dialog legen Sie für ein bestimmtes PLKZ (A) eine abweichende Vorgehensweise fest. Bei der Preisfindung wird zunächst das aktuelle PLKZ ermittelt. Danach prüft A+W Enterprise, welche abweichende PLKZ-Logik angewendet werden soll.
Wenn Sie mit der internen Mandantentrennung arbeiten, können Sie so auch die Preisfindung in den unterschiedlichen Häusern steuern.

### Globale und lokale Preislisten
Bei Betrieben mit interner Mandantentrennung kann die Preisberechnung über globale (hausübergreifend) und lokale (hausspezifisch) Preislisten gesteuert werden.
Dazu wird ein Preis-Master-Haus eingerichtet, dem die Mitarbeiter zugeordnet sind, die für die Pflege der Stammdaten von Preisen und Konditionen zuständig sind.
Für die globalen Preislisten des Preis-Master-Hauses können alle Arten der Preissteuerung verwendet werden, während für die lokalen Preislisten nur die Methoden PLKZ und PLKZ-Basis verwendet werden können.

> **Voraussetzungen**
> Die Funktion zur Arbeit mit globalen und lokalen Preislisten muss durch den Service der A+W Software GmbH konfiguriert werden.

*Abb. C-23 Globale/lokale Preislisten*

In dieser schematischen Darstellung sehen Sie, dass die Mandanten jeweils mit eigenen lokalen Preislisten arbeiten. Der Kunde 5000 ist als Debitor dem Haus 5130 zugeordnet. In den Allgemeinen Konditionen und/oder den Kundenkonditionen werden ihm die entsprechenden Preislisten zugeordnet. Damit werden die Aufträge für ihn über die lokalen Preislisten des Mandanten 5130 berechnet.
Der Kunde kann über die hausspezifischen Angaben zusätzlich auch dem Mandanten 5400 zugeordnet sein, so dass seine Aufträge auch über die Preise des Mandanten 5400 berechnet werden können. Für diese Einstellung benötigen Sie spezielle Administratorrechte.
Die globale Preisliste des Preis-Masters ist allen Mandanten übergeordnet, so dass Sie diese Preislisten in den Konditionen der einzelnen Mandanten zuordnen können. Damit haben die Mandanten auch Zugriff auf alle Preismethoden.
Über die Rechteverwaltung können Sie steuern, welche Mitarbeiter auch in der Auftragserfassung auf die globalen Preislisten zugreigen dürfen.

## Komponenten der Preisberechnung

**Lernziele**
- Einstellungen zur Preisberechnung verstehen.
- Preismethoden für die Berechnung von Scheiben unterscheiden.
- Rundungsmethoden in der Preisberechnung richtig einsetzen.
- Preisrelevante Menge berechnen.
- Preisarten nach Grundmengen berechnen.

**Nutzen**
- Die unterschiedlichen Produkte können nur dann exakt berechnet werden, wenn die Preisdefinition auf die Produktart abgestimmt ist.
- Dazu können Sie die Komponenten der Preisdefinitionen zielgerichtet einsetzen.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Preismethode** | Die Art der Preisberechnung und der Konditionen für einen Artikel wird durch die Preismethode gesteuert, die dem Artikel zugewiesen ist. Die Preismethode ist ein Algorithmus zur Preisberechnung für die Artikel einer bestimmten Produktart. Die Preismethoden sind vom System fest vorgegeben. |
| **Preisrundung** | Die Preisrundung gibt an, ob der errechnete Preis nach oben oder unten und auf wie viele Stellen gerundet wird. |
| **Preisrelevante Menge** | Menge, für die der Preis berechnet wird. Sie wird durch die Mindestkantenlänge, die Maßrundung und die Mindestberechnungsmenge beeinflusst. Die preisrelevante Menge kann von der tatsächlichen physikalischen Menge abweichen. |
| **Preisart** | Die Preisart gibt an, wie der Preis ermittelt wird, z. B. als Einzelpreis, Staffelpreis, Variantenpreis usw. |
| **Preisermittlung** | Die Suche nach den Vorgaben für die Preisberechnung wird in diesem Dokument als Preisermittlung bezeichnet. |
| **Preistyp** | Der Preistyp gibt an, worauf sich der angegebene Preis bezieht, z. B. auf die Mengeneinheit aus den Artikeldaten, auf Meter usw. |
| **Grundmengeneinheit (GME)** | Einheit der Artikelmenge aus den Artikelstammdaten. |

### Preismethoden
Die Art der Preisberechnung und der Konditionen für einen Artikel wird durch die Preismethode gesteuert, die dem Artikel zugewiesen ist. Die Preismethode ist ein Algorithmus zur Preisberechnung für die Artikel einer bestimmten Produktart.

*Abb. C-24 Auswahl Preismethoden in den Artikelstammdaten*

Für jede Produktgruppe existiert eine eigene Preismethode, die die speziellen Eigenschaften der Produktgruppe bei der Preisberechnung berücksichtigt. Die Preismethode wird dem Artikel in den Artikelstammdaten zugewiesen.

| Produktart | Preismethode | Preisdefinitionen |
| :--- | :--- | :--- |
| **ISO-Artikel** | 40 - ISO Schweiz<br>41 - ISO-Aktuell | - Preise in Matrizen oder Vektoren<br>- Austauschpreise für bis zu 3 Austauschgläser<br>- Einzelscheibenpreise<br>- Bearbeitungs- und Zubehörpreise<br>- Zuschläge für Stufen, Größen, Modelle<br>- Zuschlag abhängig von der Breite des SZR |
| **VSG-Artikel** | 29 - PKZ-VSG | - Preise in Artikelvektoren<br>- Austauschpreis für jedes Austauschglas und jede Austauschfolie<br>- Zusatzpreis für zusätzliche Artikel<br>- Stufenpreise<br>- Bearbeitungs- und Zubehörpreise<br>- Varianten-Preise |
| **ESG-Artikel** | 22 - PKZ-ESG | - Preise in Artikelvektoren<br>- Bearbeitungs- und Zubehörpreise<br>- Varianten-Preise |
| **Float-Artikel** | 23 - PKZ-Basisglas | - Preise in Artikelvektoren<br>- Bearbeitungs- und Zubehörpreise<br>- Varianten-Preise<br>- Zuschläge für Größen, Modelle |
| **Zubehör-Artikel** | 25 - PKZ-Preise allgemein | - Preise in Artikelvektoren<br>- Keine zusätzlichen Bearbeitungs- und Zubehörpreise |
| **Farbige Zubehör-Artikel** | 31 - PKZ-Farbartikel | - Preise für jede Farbe einzeln möglich |
| **Bearbeitungs-Artikel** | 26 - PKZ-Bearbeitungen | - Preise in Bearbeitungsvektoren |
| **Gussglas-Artikel** | 24 - PKZ-veredeltes Glas | - Preise in Gussglas-Klassen |
| **Sprossen-Artikel** | 5 - Sprossenpreise | - Preise für Sprossenartikel<br>- Preise für Sprossenkonstruktionselemente, z. B. Kreuze, Felder usw. |
| **GGA** | 12 - PKZ-Glastüren | - Preise in Artikelvektoren<br>- Verschiedene Artikeltypen zugelassen (60, 100, 110, 120, 130, 140, 150, 170, 200)<br>- Gläser mit bestimmten Preismethoden zugelassen (PKZ-Preise allgemein, PKZ-ESG, PKZ-VSG, PKZ-Basisglas, PKZ-veredeltes Glas) |
| **Verglasung** | 28 - PKZ-Verglasung | - Preise in Artikelvektoren |
| **UV-Abdeckungen** | 60 - Abdeckung | - Vektorpreis |
| **Manuelle Preiserfassung** | 99 - manuelle Preise | - Preise werden ausschließlich im Auftrag angegeben |

*Tab. C-1 Preismethoden für die verschiedenen Produktarten*

### Rundungsmethoden (Preisberechnung)
Standardmäßig werden die Preise auf die kleinsten Währungseinheiten gerundet, die in der Währung angegeben sind, z. B. auf 2 Nachkommastellen. Die Rundungsmethoden können sich auf den einzelnen Preis oder auf den Stückpreis beziehen.

*Abb. C-25 Preisrundungen*
- **A** Kaufmännische Rundungen für die Globale Preispflege
- **B** Stückpreisrundung aus den Tageskonditionen

> **Maßrundungen**
> Maßrundungen werden immer vor der Ermittlung und Berechnung von Preisen berechnet. Mit den gerundeten Maßen werden die preisrelevanten Mengen berechnet, zu denen die Preise berechnet werden. Erst danach werden die errechneten Preise gerundet.

#### Rundungsvariablen
Neben den Einstellungen zur Maß- und Preisrundung werden über die Systemkonfiguration weitere Einstellungen definiert.
Wenn Sie weitere Einstellungen benötigen, sprechen Sie Ihren Service-Mitarbeiter bei der A+W Software GmbH an.

#### Kaufmännische Rundung
Nach jedem Rechenschritt der Preisberechnung wird das Zwischenergebnis gerundet. Dazu stehen folgende Rundungsmethoden zur Verfügung:
- **Auf**: Der Preis wird auf den hundertstel-Wert in Währungseinheiten aufgerundet.
- **Ab**: Der Preis wird auf den hundertstel-Wert in Währungseinheiten abgerundet.
- **Kau**: Der Preis wird kaufmännisch auf den hundertstel-Wert auf- oder abgerundet.

**Beispiel**

| Rundung | Wert | von | auf |
| :--- | :--- | :--- | :--- |
| Auf 10 | 4,38 € | 4,40 € | aufgerundet |
| | 4,73 € | 4,80 € | |
| Ab 10 | 4,38 € | 4,30 € | abgerundet |
| | 4,73 € | 4,70 € | |
| Kau 10 | 4,35 € | 4,40 € | aufgerundet |
| | 4,34 € | 4,30 € | abgerundet |
| Kau 100 | 4,38 € | 4,00 € | abgerundet |
| | 4,73 € | 5,00 € | aufgerundet |

#### Stückpreis-Rundung
Zum Berechnen des Stückpreises wird eine Stückpreisrundung verwendet, die in den Konditionen angegeben werden kann.

**Beispiel für Stückpreis-Rundung**
Wenn `Stückpreisrundung = 100` angegeben ist, wird der Preis auf den nächsten vollen Währungsbetrag gerundet:
54.56 -> 55.00
54.46 -> 54.00

Wenn `Stückpreisrundung = 10` angegeben ist, wird der Preis auf den nächsten Zehntelbetrag gerundet, z. B. 10 Cent:
54.65 -> 54.70
54.64 -> 54.60

### Preisrelevante Menge
Die Glasartikel legen Sie in der Regel in den Stammdaten mit der Grundmengeneinheit (GME) Quadratmeter an.
Zur Berechnung der Preise können Sie angeben, wie die preisrelevante Menge berechnet wird. Dazu gehören die Mindestkantenlänge, die Maßrundung und die Mindestberechnung.

*Abb. C-26 Artikelvektoren – Details*

- **A** Mindestberechnung
- **B** Mindestkantenlänge
- **C** Maßrundung

Die Fläche des Glases wird wie folgt berechnet:

1.  **Mindestkantenlänge**
    Die Höhe und die Breite der Scheibe werden mit der hinterlegten Mindestkantenlänge verglichen. Wenn der hinterlegte Wert nicht erreicht ist, wird die Mindestkantenlänge zur weiteren Berechnung herangezogen.

2.  **Maßrundung**
    Die Breite und Höhe werden der angegebenen Maßrundung entsprechend gerundet.
    Zur Maßrundung wird ein Maß angeben, z. B. 30 mm. Die Kantenlänge wird damit auf das nächste Maß aufgerundet, das durch diesen Wert (30mm) teilbar ist.

3.  **Fläche**
    Mit der aktuellen oder der Mindestlänge von Breite und Höhe wird die Fläche des Glases berechnet:
    - (Breite x Höhe) / 1.000.000 ergibt die Fläche in qm.
    - Die berechnete Fläche wird der Systemkonfiguration entsprechend gerundet.

Die gerundete Fläche wird mit der hinterlegten Mindestfläche verglichen. Der höhere Wert wird zur Preisberechnung des Glases herangezogen.

| Schritt | Maße | Berechnung | Rundung |
| :--- | :--- | :--- | :--- |
| | Mindestkantenlänge = 800 mm<br>Mindestfläche = 0,5 qm | | Maßrundung = 30 mm |
| 1. | Breite 1235 mm<br>Höhe 1895 mm | | (Mindestkantenlänge erreicht) |
| 2. | 1235 mm<br>1895 mm | Maßrundung 1260 mm<br>Maßrundung 1920 mm | |
| 3. | 1260 mm<br>1920 mm | Fläche 2,4192 qm | (Mindestfläche erreicht)<br>Fläche 2,42 qm |
| | Glaspreis 46,53 € | | |
| | Preisberechnung mit der größeren Fläche = 2,42 qm | 112,6026 € | 112,60 € |

*Tab. C-2 Beispiel für Rundungen bei der Preisberechnung*

### Preisarten
Preisarten geben bei gestaffelten Preisen an, aus welcher Preisstufe der Preis ermittelt wird:

1.  **1 - Einzelpreis**: Zur Preisberechnung im Auftrag wird der Preis der Stufe 1 herangezogen.
2.  **2 - Staffelstufe**: Zur Preisberechnung im Auftrag wird die Preisstufe ermittelt, die in den Konditionen angegeben ist.
3.  **3 - Mengenstaffel pro Position (GME)**: Zur Ermittlung der Preisstufe wird die Menge der Position anhand der Grundmengeneinheit (GME) des Artikels ermittelt. Der Preis wird im Auftrag nach der Preisstufe berechnet, die durch die Gesamtmenge der Position erreicht ist.
4.  **4 - Mengenstaffel pro Stück (GME)**: Zur Ermittlung der Preisstufe wird die Grundmenge in einem Stück der Position ermittelt.
5.  **5 - Gesamtmenge pro Vektor**: Im Auftrag werden die Preise auf Basis der Gesamtmenge berechnet. Dazu werden alle Positionen ermittelt, für die derselbe Preisvektor gilt. Die Mengen der entsprechenden Positionen werden summiert. Diese Summe wird mit den definierten Preisstufen verglichen. Der Preis wird anhand der ermittelten Preisstufe berechnet.
6.  **6 - Gesamtmenge pro Stücklistenkopf**: Im Auftrag werden alle Positionen ermittelt, die dieselbe Stücklistenkopfnummer haben. Die Mengen der entsprechenden Positionen werden summiert. Diese Summe wird mit den definierten Preisstufen verglichen. Der Preis wird anhand der ermittelten Preisstufe berechnet.
7.  **7 - Gesamtmenge pro Farbbeschichtung**: Im Auftrag werden alle Positionen ermittelt, die dieselbe Farbbeschichtung haben. Dazu wird nicht die Farbvariante des Artikels geprüft, sondern in der Auftragsposition die Angabe im Register Eigenschaften > Feld Fertg-Folge. Die Mengen der entsprechenden Positionen werden summiert. Diese Summe wird mit den definierten Preisstufen verglichen. Der Preis wird anhand der ermittelten Preisstufe berechnet.
8.  **8 - Gesamtmenge pro Warengruppe**: Im Auftrag werden alle Positionen ermittelt, die dieselbe Warengruppe haben. Die Mengen der entsprechenden Positionen werden summiert. Diese Summe wird mit den definierten Preisstufen verglichen. Der Preis wird anhand der ermittelten Preisstufe berechnet.
9.  **9 - Stück pro Position**: Zur Ermittlung der Preisstufe wird die Stückzahl der Position verwendet.
10. **10 - Gesamtmenge pro Auftrag**: Zur Ermittlung der Preisstufe wird die Gesamtmenge aller Positionen im Auftrag ermittelt.
11. **11 - Variantenartig**: Bei dieser Preisart können die Preise abhängig von 2 Maßen gestaffelt werden, z. B. von Höhe und Breite. Zur Ermittlung der Preisstufe wird das kleinere Maß mit der ersten Spalte verglichen, das größere mit der zweiten Spalte. Der Preis wird im Auftrag nach der Preisstufe berechnet, bei der die Grenzwerte von beiden Maßen erreicht sind. ⇨ Softwarereferenz, "Artikelvektoren" auf Seite C-749
12. **12 - Variantenstaffel**: Die Preisart ist sinnvoll für Glastüren. Bei dieser Preisart wird die Breite der Glastür mit dem Wert aus der ersten Spalte verglichen und die Höhe der Glastür mit dem Wert aus der zweiten Spalte. Dabei ist wichtig, dass die Maße aufsteigend eingegeben werden, zuerst nach der ersten Spalte und dann nach der zweiten Spalte. Der Preis wird im Auftrag nach der Preisstufe berechnet, bei der die Grenzwerte von beiden Maßen erreicht sind.

> **Variantenstaffel vs. Variantenpreise**
> Für Glastüren mit Standard-Maßen werden herkömmlicherweise Variantenpreise hinterlegt. Wenn Glastüren mit Standard-Maßen bestellt werden, werden die Variantenpreise herangezogen.
> Für Glastüren mit Sondermaßen werden Vektorpreise mit der Preisart Variantenstaffel hinterlegt. Zur Preisberechnung ermittelt A+W Enterprise die Vektorpreise mit der Preisart Variantenstaffel.

13. **13 - Mengenstaffel/Gebindegröße**: Diese Preisart wird dann verwendet, wenn ein Preis für einen Artikel einen sehr geringen Wert hat, der nicht mit einer Genauigkeit von zwei Nachkommastellen dargestellt werden kann.

**Beispiel**
Artikel mit Stückpreis von 0,0254 Euro: bei Menge 100 = 2,54 WE/Stück.
Der Stückpreis für einen Sack mit 1000 Korkblättchen beträgt 25,40 €.
Pro Scheibe werden 5 Blättchen verbraucht.
Bei einer Positionsmenge von 15 Scheiben werden 75 Blättchen gebraucht.
Der Positionspreis wird als genauer Stückpreis berechnet und anschließend auf zwei Nachkommastellen gerundet.
- Berechnung: 75 Stück x 0,0254 € = 1,905 €
- nach Rundung = 1,91 €.

### Preistyp
Zu jedem Preis müssen Sie angeben, worauf sich der angegebene Wert bezieht. Für jeden Preis muss ein Preistyp und eine Preisart ausgewählt werden. Die Preistypen und Preisarten sind fest vom System vorgegeben.

*Abb. C-27 Beispiel für Preistypen und Preisarten*

- **A Preisarten**
- **B Preistypen**

Der Preistyp gibt an, worauf sich der angegebene Preis bezieht. Dabei wird die Währungseinheit (WE) zugrunde gelegt, in der das System rechnet.

- **WE/GME**: Der Preis wird pro Grundmengeneinheit (GME) angegeben, die in den Artikelstammdaten hinterlegt ist, z. B. pro Stück, Ifm usw.
- **WE/Stück**: Der Preis wird pro Stück angegeben.
- **WE/qm**: Der Preis wird pro Quadratmeter angegeben.
- **WE/Im**: Der Preis wird pro laufendem Meter angegeben. Dieser Preistyp wird nur bei Bearbeitungen gewählt.
- **Prozent**: Die Preise werden prozentual aus dem Grundpreis des Positionsartikels errechnet. Dieser Preistyp wird nur bei Austauschartikeln oder Bearbeitungen gewählt.

### Mengenberechnung nach GME
Preise können sich nach der Menge im Auftrag richten. Daher besteht die Möglichkeit, Preise in Mengenstaffeln zu hinterlegen.
Dazu stehen verschiedene Gesamtmengen-Preisarten zur Verfügung.

> **Maßrundungen**
> Maßrundungen werden immer vor der Ermittlung und Berechnung von Preisen berechnet. Mit den gerundeten Maßen werden die preisrelevanten Mengen berechnet, zu denen die Preise berechnet werden. Erst danach werden die errechneten Preise gerundet.
> In den folgenden Beispielen werden Maßrundungen und andere Maßdefinitionen nicht berücksichtigt.
> Anzahl bezeichnet je nach Preisart die Anzahl der ISO-Einheiten, der Einzelscheiben oder die Positionsstückzahl.

| Grundmengen-Einheiten (GME) | Erklärung |
| :--- | :--- |
| Tonne, Liter, Kilogramm, Stunden | Eindimensionale Einheiten. Zur Berechnung der Menge wird die Anzahl mit dem Wert aus dem Feld Breite (mas1) multipliziert. Wenn der Preis jedoch mit Mengenstaffel pro Stück berechnet wird, geht das System von der Anzahl = 1 aus. Je nach Konfiguration wird auf eine Nachkommastelle aufgerundet oder auf 2 Nachkomastellen kaufmännisch gerundet. |
| Millimeter | Dies ist i. d. R. eine eindimensionale Einheit. Die Millimeter werden zuerst in Meter umgewandelt (Division durch 1000). Danach wird zur Berechnung der Menge die Anzahl mit dem Wert aus dem Feld Breite (mas1) multipliziert. Wenn der Preis jedoch mit Mengenstaffel pro Stück berechnet wird, geht das System von der Anzahl = 1 aus. Die berechnete Menge wird auf eine Nachkommastelle aufgerundet. Wenn ein Millimeterartikel für einen zweidimensionalen Artikel erfasst wird, ist mas2 größer als 0. Die Millimeter werden zuerst in Meter umgewandelt. Zur Berechnung der Menge wird die Positionsmenge multipliziert mit (2 x mas1 + 2 x mas2). Die berechnete Menge wird auf eine Nachkommastelle aufgerundet. Die Variable AUFRUNDEN_FLAECHE wird nicht ausgewertet. |
| Meter | Eindimensionale Einheit. Zur Berechnung der Menge wird die Anzahl mit dem Wert aus dem Feld Breite (mas1) multipliziert. Wenn der Preis jedoch mit Mengenstaffel pro Stück berechnet wird, geht das System von der Anzahl = 1 aus. Die berechnete Menge wird nicht gerundet. Wenn jedoch ein Millimeterartikel unter einem zweidimensionalen Artikel erfasst wird, ist mas2 größer als 0. Zur Berechnung der Menge wird die Anzahl multipliziert mit (2 x mas1 + 2 x mas2). Die Variable AUFRUNDEN_FLAECHE wird nicht ausgewertet. |
| Quadratmeter | Zweidimensionale Einheit. Zur Berechnung der Menge wird zuerst Feld Breite mit Feld Höhe (mas1 x mas2) multipliziert. Da die Positionen immer in Millimetern erfasst werden, wird anschließend von Quadratmillimeter in Quadratmeter umgerechnet (Division durch 1.000.000). Die resultierenden Quadratmeter werden je nach Konfiguration auf eine Nachkommastelle aufgerundet oder auf 2 Nachkommastellen kaufmännisch gerundet. Zum Schluss werden die gerundeten Quadratmeter mit der Anzahl multipliziert. Wenn der Preis jedoch mit Mengenstaffel pro Stück berechnet wird, geht das System von der Anzahl = 1 aus. |
| Stück | Anzahl gleich Menge. Wenn der Preis jedoch mit Mengenstaffel pro Stück berechnet wird, geht das System von der Anzahl = 1 aus. Die Variable AUFRUNDEN_FLAECHE wird nicht ausgewertet. |
| Umfang | Zweidimensionale Einheit. Die Millimeter werden zuerst in Meter umgewandelt (Division durch 1000). Die resultierende Menge wird je nach Konfiguration auf eine Nachkommastelle aufgerundet oder auf 2 Nachkommastellen kaufmännisch gerundet. Mit diesen gerundeten Metern wird anschließend der Umfang berechnet (2 x mas1 + 2 x mas2). Bei dieser GME wird nicht mit der Anzahl multipliziert. |

*Tab. C-3 Mengenberechnung nach GME*

## Schlüssel anlegen
In dieser Einheit lernen Sie, wie Sie die Schlüssel für die Preisdefinitionen anlegen. Die gezeigten Handlungsschritte gelten analog für alle Preisschlüssel.
Zu dieser Einheit gehören folgende Handlungssequenzen:
- So legen Sie ein Sprossenpreiskennzeichen an
- So legen Sie eine Sprossenpreisklasse an

### So legen Sie ein Sprossenpreiskennzeichen an
1.  Wählen Sie im Menü Stammdaten > Schlüssel > Preise > Sprossenpreiskennzeichen.
2.  Drücken Sie <F6>, um eine neue Zeile einzufügen.

*Abb. C-28 Neue Zeile freigeschaltet*

- **A** Neue Zeile
- **B** Schlüsselnummer
- **C** Bezeichnung für das S-PKZ
- **D** Währung

3.  Tragen Sie die Schlüsselnummer (B) für das neue S-PKZ ein.
4.  Tragen Sie eine sprechende Bezeichnung (C) ein, z. B. wofür der Schlüssel verwendet werden soll.
5.  Wählen Sie die Währung aus.
6.  Bestätigen Sie die Daten mit <Enter>.
    Die Daten werden gespeichert und eine neue Zeile wird eingefügt.
7.  Wiederholen Sie die Schritte 3 bis 6 für ein weiteres S-PKZ oder schließen Sie den Dialog.
    Als nächstes legen Sie eine Sprossenpreisklasse an.

### So legen Sie eine Sprossenpreisklasse an
1.  Wählen Sie im Menü Stammdaten > Schlüssel > Preise > Sprossenpreisklassen.
2.  Drücken Sie <F6>, um eine neue Zeile einzufügen.

*Abb. C-29 Neue Zeile freigeschaltet*

- **A** Neue Zeile
- **B** Schlüsselnummer
- **C** Bezeichnung für die Sprossenpreisklasse

3.  Tragen Sie die Schlüsselnummer (B) für die neue Sprossenpreisklasse ein.
4.  Bestätigen Sie die Daten mit <Enter>.
    Die Daten werden gespeichert und eine neue Zeile wird eingefügt.
5.  Wiederholen Sie die Schritte 3 und 4 für eine weitere Sprossenpreisklasse oder schließen Sie den Dialog.

### Übungen
Stellen Sie sicher, dass Sie mit der Anmeldung in A+W Enterprise alle Benutzerrechte erworben haben, die für die Arbeiten mit den Stammdaten erforderlich sind.
Legen Sie für die Übungen in den nachfolgenden Lerneinheiten folgende Schlüssel an:
- Preislistenkennzeichen, z B. 9999 - Schulung.
- Legen Sie mindestens je einen Schlüssel für eine Matrix, einen Artikel-, einen Bearbeitungsvektor und eine Austauschliste an. Wählen Sie auch dazu Nummern und Bezeichnungen, die sich deutlich von den Standardschlüsseln unterscheiden.
- Achten Sie bei den Listen darauf, dass Sie die Angabe der Master-Liste nicht ändern.
- Legen Sie eine Sprossenpreisklasse und ein Sprossenkennzeichen an. Denken Sie dabei daran, die richtige Währung zuzuordnen.

## Stammdaten für Preise
In diesem Themenblock lernen Sie, wie Sie die Preise in A+W Enterprise anlegen. Die Preise können Sie nur anlegen, wenn Sie die notwendigen Schlüssel hinterlegt haben.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Workflow: Preise anlegen" auf Seite C-581
- "Preismatrizen für ISO-Scheiben" auf Seite C-582
- "Preisvektoren" auf Seite C-596
- "Austausch- und Zusatzpreise" auf Seite C-614
- "Sprossenpreise" auf Seite C-626
- "Zuschläge" auf Seite C-632
- "Globale Preisänderungen" auf Seite C-644

### Workflow: Preise anlegen
Damit die Preise korrekt berechnet werden können, sind folgende Schritte notwendig:

1.  **Schritt: Preislistenkennzeichen (PLKZ) anlegen**
    Jede Preisliste wird mit einer eindeutigen Nummer und einer Bezeichnung angelegt, dem Preislistenkennzeichen (PLKZ). Zusätzlich wird die Währung angegeben, mit der die Preise berechnet werden, z. B. Euro.
    ⇨ Softwarereferenz, "Preislisten (PLKZ)" auf Seite C-696

2.  **Schritt: Schlüssel für Matrizen, Vektoren u. a. erfassen**
    Zu jedem Schlüssel wird eine Nummer und eine Bezeichnung angegeben.

3.  **Schritt: Preise in Preislisten erfassen**
    Artikelpreise werden in Matrizen und Vektoren erfasst. Eine Preisliste kann aus vielen Matrizen und Vektoren bestehen.

4.  **Schritt: Preislistenreferenz festlegen**
    Für die Referenzen werden die Preiskennzeichen (PKZ) definiert. Dem Preiskennzeichen (PKZ) wird die jeweils gültige Preisliste (PLKZ) mit den Artikelpreisen zugeordnet.
    ⇨ Softwarereferenz, "Preiskennzeichen (PKZ)" auf Seite C-697

5.  **Schritt: Preiskennzeichen (PKZ) den Marktpartnern zuordnen**
    Die aktuellen PKZ für jede Preismethode werden in den Allgemeinen Tageskonditionen festgelegt.
    Jedem Marktpartner kann pro Preismethode ein abweichendes Preiskennzeichen (PKZ) zugeordnet werden. Dasselbe PKZ kann für mehrere Marktpartner gelten.

## Preismatrizen für ISO-Scheiben

**Lernziele**
- Unterschiede der Matrixformen verstehen.
- Einsatzmöglichkeiten für Preismatrizen kennenlernen.
- Auswertung der Matrix bei der Preissuche verstehen.
- Funktion der Grundpreise kennenlernen.
- Grundpreise definieren und zuordnen.

**Nutzen**
- Mit Preismatrizen können Preise sehr fein gestaffelt werden. Dabei muss jeweils der Artikel berücksichtigt werden, der über eine Preismatrix berechnet werden soll.
- Mit der Definition der Grundpreise können Sie besonders die Preisberechnungen mit Preismatrizen sehr detailliert festlegen.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Dreiecksform** | In der Dreiecksform können die Grenzwerte vertauscht werden. Daher müssen nicht alle Kombinationen der Grenzwerte mit Preisen gefüllt sein. Preise in einer Dreiecksmatrix sind dann sinnvoll, wenn z. B. für die Maße 500 × 750 mm und 750 x 500 mm derselbe Preis gilt. |
| **Grenzwert** | Der Grenzwert gibt die Stufen einer Staffelung an. Abhängig vom Matrixtyp beziehen sich die Grenzwerte auf Kantenlängen, Flächen und Stückzahlen. |
| **Grundpreise** | Mit der Definition von Grundpreisen legen Sie Details für die Berechnung der ISO-Scheiben fest. |
| **Matrix** | Zweidimensionale Preistabelle zur Staffelung der Preise. In Preismatrizen werden ISO-Preise definiert, die von zwei Grenzwerten abhängig sind, z. B. von Höhe und Breite. |
| **Matrixart** | Die Matrixart gibt an, ob die Preise in einer Dreiecks- oder einer Quadratmatrix angelegt sind. Die Wahl der Matrixart hängt mit dem Matrixtyp zusammen. |
| **Matrixtyp** | Der Matrixtyp gibt an, ob die Grenzwerte mit den Kantenlängen verglichen werden oder mit der Stückzahl und der Fläche.<br>- **Breite x Höhe**: Die beiden Grenzwerte für die Staffelung werden in mm angegeben.<br>- **Stück x qm**: Der Grenzwert der Spalte wird in Stückzahlen angegeben, der Grenzwert für die Zeilen in qm. |
| **Quadratform** | In der Quadratform dürfen die Grenzwerte nicht vertauscht werden. Daher müssen alle Kombinationen der Grenzwerte mit Preisen gefüllt sein. Die Quadratform wird für Gläser mit Strukturverlauf verwendet, bei denen die Struktur eine Richtung hat. Diese Form muss auch für den Matrixtyp Stück x qm verwendet werden. |
| **Voraussetzungen** | Schlüssel für Preislisten und Matrizen sind angelegt. Grenzwerte sind als Grenzmaße angelegt (optional). |

### Matrix-Editor
Eine Matrix ist eine zweidimensionale Preistabelle, in der der Preis von zwei Größen abhängt, z. B. von Breite und Höhe der erfassten Position.
Matrizen eignen sich für ISO-Artikel mit der Preismethode ISO-Aktuell oder Bearbeitungen mit der Preismethode Bearbeitungsmatrizen.

*Abb. C-30 Matrix-Editor*

| Kürzel | Beschreibung |
| :--- | :--- |
| A | Zeilenkopf |
| B | Spaltenkopf |
| C | Matrixnummer |
| D | PLKZ |
| E | Matrixtyp |
| F | Matrixart |
| G | Preistyp |

In diesem Beispiel sehen Sie eine Preismatrix für die Berechnung von ISO-Preisen:
- Im Kopfbereich des Dialogs sind die Schlüssel (C, D), der Preistyp und die Form der Matrix (G, E und F) angegeben.
- Im Spaltenkopf (A) und im Zeilenkopf (B) sind Grenzwerte angegeben.

In einer Matrix können Sie bis zu 30 x 30 Werte festlegen. Das bedeutet, dass Sie bis zu 900 Preise angeben können, die im Auftrag herangezogen werden.
A+W Enterprise bietet außerdem die Möglichkeit, Matrizen aus ASCII-Dateien mit festen Formaten einzulesen, z. B. csv-Dateien.

> **Tipp**
> Wenn Sie eine neue Matrix anlegen wollen, können Sie eine ähnliche Matrix kopieren und dann die Werte anpassen.
> Beachten Sie, dass die Ab-PLKZ-Logik für Matrizen nicht gilt. Wenn Sie eine neue Matrix anlegen, muss sie genau dem PLKZ zugewiesen sein, nach dem die Preise berechnet werden sollen. Ggf. müssen Sie also zunächst ein neues PLKZ anlegen.

#### Matrixtyp
Der Matrixtyp gibt an, ob die Grenzwerte mit den Kantenlängen verglichen werden oder mit der Stückzahl und der Fläche.
- **Breite x Höhe**:
  - Wenn die Maße aus der Auftragsposition gedreht werden dürfen, gilt:
    - Das kleinere Maß wird mit den Spaltengrenzwerten verglichen.
    - Das größere Maß wird mit den Zeilengrenzwerten verglichen.
  - Wenn die Maße aus der Auftragsposition nicht gedreht werden dürfen, gilt:
    - Die Spaltengrenzwerte werden mit dem Maß der Breite verglichen.
    - Die Zeilengrenzwerte werden mit dem Maß der Höhe verglichen.
  Ob die Maße aus einer Auftragsposition gedreht werden dürfen, hängt von der Matrixart und den gesetzten Umgebungsvariablen ab.
  ⇨ "Matrixart" auf Seite C-585
- **Stück x qm**:
  - Die Spaltengrenzwerte werden mit der Fläche verglichen.
  - Die Zeilengrenzwerte werden mit der Stückzahl verglichen.

#### Matrixart
Eine Matrix kann als Dreiecksmatrix oder als Quadratmatrix definiert werden. Welche Form Sie wählen, hängt von dem Artikel ab, der mit der Matrix berechnet werden soll.

- **Dreiecksmatrix**:
  Preise in einer Dreiecksmatrix sind dann sinnvoll, wenn z. B. für die Maße 500 × 750 mm und 750 × 500 mm derselbe Preis gilt.
  Standardmäßig wird das kleinere Längenmaß der Position mit den Spaltengrenzwerten verglichen, das größere mit den Zeilengrenzwerten. Gegebenenfalls werden die Maßangaben dazu gedreht.

*Tab. C-4 Beispiel für eine Dreiecksmatrix*
In diesem Beispiel müssen die farbigen Felder der Dreiecksmatrix nicht gefüllt werden, weil sie sich aus Länge = Breite ergeben.

> **Dreiecksform nicht anwenden**
> Sie müssen Preise für Gläser, die nicht gedreht werden dürfen, z. B. Strukturgläser, deren Struktur eine Richtung hat, als Quadratmatrix eingeben.
> Dies gilt auch, wenn die Umgebungsvariable MATRIXMASSE_UNGEDREHT in Ihrem Unternehmen gesetzt ist und die Maße nicht gedreht werden dürfen.
> Grundsätzlich wird die erste Längenangabe im Auftrag mit den Spaltengrenzwerten und die zweite Längenangabe mit den Zeilengrenzwerten verglichen.

- **Quadratmatrix**:
  Wenn der Preis aus einer Quadratmatrix ermittelt wird, müssen Sie sämtliche Felder der Matrix füllen. Die Quadratmatrix ist dann sinnvoll, wenn die Maße zur Preisermittlung nicht gedreht werden dürfen, z. B. bei Strukturgläsern, deren Struktur eine Richtung hat oder beim Matrixtyp Stück × qm für ISO-Scheiben.

*Tab. C-5 Beispiel für eine Quadratmatrix*
In diesem Beispiel sind die farbigen Felder gefüllt, weil sich die Preise von Länge x Breite und Breite x Länge unterscheiden.

#### Preistyp
Für die Berechnung der Preise im Auftrag werden folgende Preistypen verwendet:
- **Stk-Prs**: Der Preis wird pro Stück berechnet. Dieser Preistyp wird nicht für Austauschgläser oder Bearbeitungen unterstützt.
- **qm-Prs**: Der Preis wird pro Quadratmeter berechnet. Dieser Preistyp wird für alle Artikel unterstützt.
- **Prozent**: Der Preis wird prozentual aus dem Grundpreis des Positionsartikels berechnet. Dieser Preistyp wird nicht für Austausch- oder ISO-Gläser unterstützt.
- **Im**: Der Preis wird pro Laufmeter berechnet. Dieser Preistyp wird nur für Bearbeitungen unterstützt.

#### Grenzmaße
Wenn das Maß den angegebenen Grenzwert überschreitet, gilt der nächste Wert. Dabei werden die Maße vor dem Abgleich der Werte gerundet.
⇨ "Preisrelevante Menge" auf Seite C-571

Sie können Vorlagen für Längengrenzmaße im Dialog Matrix-Grenzmaße definieren. Diesen Dialog können Sie im Matrix-Editor in den Feldern PLKZ und Matrix mit <Shift> + <F11> aufrufen. Die Grenzmaße können Sie für den Matrixtyp Breite × Höhe verwenden, wenn Sie eine neue Matrix anlegen. Sie können dann diese Grenzmaße über die Felder Spalten und Zeilen importieren und anpassen.

*Abb. C-31 Matrix-Grenzmaße für Typ Br x Ho*
- **A** Sprechende Bezeichnung
- **B** Anzahl der definierten Maße
- **C** Maße

Geben Sie in der Vorlage eine sprechende Bezeichnung ein, aus der ersichtlich ist, wofür die Maße gedacht sind. Die Anzahl gibt an, wie viele Spalten oder Zeilen für die Grenzmaße in dieser Matrix angelegt werden sollen.
Sie können zudem Vorlagen für Flächengrenzmaße im Dialog Matrix-Flächengrenzmaße definieren. Diesen Dialog können Sie im Matrix-Editor in den Feldern PLKZ und Matrix mit <Ctrl>+ <F11> aufrufen. Die Grenzmaße können Sie für den Matrixtyp Stk x qm und den Preistyp qm-Prs verwenden, wenn Sie eine neue Matrix anlegen. Sie können dann diese Grenzmaße über das Feld Zeilen importieren und anpassen.
Wenn Sie die Werte in eine neue Matrix importiert haben, können Sie die Maße anpassen und auch weitere Spalten und Zeilen definieren.

## Preismatrix für ISO-Scheiben anlegen
In diesem Beispiel legen Sie eine Matrix an, indem Sie die Grenzmaße importieren und anschließend die Preise eintragen. Als Alternative importieren Sie eine (alte) Matrix und ändern dabei die Preise.
Zu dieser Einheit gehören folgende Handlungssequenzen:
- "So legen Sie eine Matrix an" auf Seite C-589
- "So übernehmen Sie die Preise aus einer anderen Matrix" auf Seite C-591
- "So rechnen Sie die Matrixpreise insgesamt um" auf Seite C-592

Wenn Sie eine Preismatrix anlegen, werden Sie sehen, dass Sie keine zusätzlichen Angaben machen können, z. B. Zuschläge für kleine Scheiben oder für welchen ISO-Artikel die Matrix gilt. Diese Details zur Preisberechnung legen Sie im Dialog ISO-Grundpreise an.
⇨ "Grundpreise für ISO-Scheiben" auf Seite C-593

> **Voraussetzung**
> Sie haben die erforderlichen Benutzerrechte.
> Sie haben mindestens einen Schlüssel für Matrizen angelegt.
> Beachten Sie, dass die Ab-PLKZ-Logik für Matrizen nicht gilt. Wenn Sie eine neue Matrix anlegen, muss sie genau dem PLKZ zugewiesen sein, nach dem die Preise berechnet werden sollen. Ggf. müssen Sie also zuerst ein neues PLKZ anlegen.

### So legen Sie eine Matrix an
1.  Wählen Sie im Menü Stammdaten > Preise > ISO-Preise > Matrix-Editor.
*Abb. C-32 Kopfdaten füllen*
    - **A** PLKZ
    - **B** Matrixnummer
    - **C** Matrixtyp
    - **D** Matrixart
    - **E** Preistyp
    - **F** Spaltenanzahl
    - **G** Zeilenanzahl
2.  Wählen Sie mit <F9> ein PLKZ (A) und eine Matrixnummer (B) aus, die Sie zum Üben hinterlegt haben.
    Überspringen Sie die folgenden Schritte und wechseln Sie zur nächsten Handlungssequenz, wenn Sie die Preise aus einer anderen Matrix übernehmen wollen.
    ⇨ "So übernehmen Sie die Preise aus einer anderen Matrix" auf Seite C-591
3.  Wählen Sie die folgenden Daten aus und bestätigen Sie jeweils mit <Enter>:
    - **C**: den Matrixtyp Br x Ho.
    - **D**: Matrixart Dreieck.
    - **E**: Preistyp qm-Prs.
4.  Wählen Sie mit <F9> die Spalten (F) und Zeilen (G) für ein ISO aus.
*Abb. C-33 Spaltenauswahl*
    Damit haben Sie die Matrix angelegt.
5.  Tragen Sie die gewünschten Preise in die Matrix ein und bestätigen Sie jeweils mit <Enter>.
6.  Wählen Sie [OK], um die Matrix zu speichern.

### So übernehmen Sie die Preise aus einer anderen Matrix

**Voraussetzung**
Eine Matrix, aus der Preise importiert werden können, muss angelegt sein.
1.  Stellen Sie den Cursor in das Feld Matrixtyp.
2.  Wählen Sie <F5>, um eine Matrix auszuwählen.
3.  Wählen Sie jeweils mit <F9> das PLKZ und die Matrixnummer aus.
4.  Lösen Sie die Übernahme mit <F3> aus.
5.  Bestätigen Sie die Abfrage zum Überschreiben der Matrix mit [Ja].
*Abb. C-34 Importierte Preise*
6.  Prüfen und korrigieren und/oder ergänzen Sie die Preise.
> **Alle Matrixpreise ändern**
> Sie können alle Preise insgesamt korrigieren, indem Sie die Werte um einen Betrag oder einen Prozentsatz erhöhen oder verringern.
> ⇨ "So rechnen Sie die Matrixpreise insgesamt um" auf Seite C-592
7.  Wählen Sie [OK], um die Matrix zu speichern.

### So rechnen Sie die Matrixpreise insgesamt um

**Voraussetzung**
Der Schlüssel für das Ziel muss angelegt sein.
1.  Wählen Sie im Menü Stammdaten > Preise > ISO-Preise > Matrix umrechnen.

*Abb. C-35 Preise importieren und umrechnen*
- **A** PLKZ, Matrixnummer der Quelle
- **B** PLKZ, Matrixnummer des Ziels
- **C** Berechnungsart der Änderung
- **D** Rundung der neuen Preise
- **E** Feld für die Eingabe der Änderung (wird nach der Auswahl C angezeigt)

2.  Tragen Sie das PLKZ und die Nummer der Matrix (A) ein, aus der die Preise importiert werden sollen.
3.  Tragen Sie das PLKZ und die Nummer der Matrix (B) ein, in die die Preise importiert werden sollen.
    Quelle und Ziel müssen unterschiedliche PLKZ oder Matrixnummern haben.
4.  Wenn die Zielmatrix bereits existiert, wird eine Abfrage angezeigt.
    Bestätigen Sie die Abfrage mit [Ja].
5.  Wählen Sie mit <Toggle> im Feld Ziel = Quelle (C) den Eintrag + WE Wert.
    Das Eingabefeld (E) für den Wert wird angezeigt.
6.  Tragen Sie den Betrag ein, mit dem die Preise erhöht werden sollen, z. B. 5.
7.  Prüfen Sie die Rundungsvorschrift (D) und korrigieren Sie diese, wenn die Währung andere Rundungen vorschreibt.
8.  Lösen Sie die Aktion mit <F3> aus.
9.  Schließen Sie den Dialog und öffnen Sie Ihre Schulungsmatrix.
10. Prüfen Sie, ob die Preise in der gewünschten Weise geändert sind.

## Grundpreise für ISO-Scheiben
Die Preise für ISO-Scheiben werden in der Regel mit der Preismethode ISO-Aktuell berechnet. Dazu legen Sie z. B. Preismatrizen an und ordnen sie dem jeweiligen ISO-Artikel zu. Außerdem geben Sie die Berechnungsvorschriften an, z. B. Angaben zur Mindestberechnung, Rundung oder zu Zuschlägen und Austauschpreisen. Dafür steht der Dialog ISO-Grundpreise zur Verfügung.

*Abb. C-36 ISO-Grundpreise – Details*

- **A** Artikelnummer
- **B** Berechnungstyp
- **C** Mindestangaben
- **D** Maßrundung
- **E** Zuschläge
- **F** Austauschlisten

In diesem Dialog ordnen Sie den ISO-Artikeln pro Preisliste die Berechnungsvorschriften zu, mit denen die Preise im Auftrag berechnet werden sollen. Bei der Zuordnung der ISO-Grundpreise gilt wieder die Ab-PLKZ-Logik, d. h., wenn in der angegebenen Preisliste kein Preis gefunden wird, wird in der numerisch nächstniedrigeren Preisliste gesucht. In der Regel werden die Preise für ISO-Artikel aus einer Matrix (B) gezogen. Die ISO-Preise können auch nach Vektoren oder Einzelscheiben berechnet werden.

> **Berechnungstyp Einzelscheiben**
> Wenn als Berechnungstyp Einzelscheiben gewählt ist, werden die Preise nach einer besonderen Berechnungsvorschrift ermittelt. Dazu müssen die Einzelscheibenpreise für ISO getrennt angegeben werden. Diese Art der Preisberechnung für ISO-Scheiben wird hauptsächlich in Frankreich genutzt.
> Die Preise werden im Dialog Einzelscheiben für ISO-Artikel festgelegt.

Zusätzlich können Sie die Details festlegen, mit denen die Berechnung der zugeordneten Preismatrix ergänzt wird.
Als Mindestangaben (C) können Sie die Kantenlänge und/oder die Fläche angeben. Damit legen Sie fest, dass der Preis für mindestens diese Größe berechnet wird.
⇨ "Preisrelevante Menge" auf Seite C-571
Mit der Maßrundung (D) legen Sie fest, wie die Maße der Auftragsposition für die Preisberechnung gerundet werden.

**Beispiel**
Als Maßrundung ist 30 mm definiert.
Der erfasste ISO-Artikel hat die Maße 1000 × 1000 mm. Die nächste, durch 30 mm teilbare Kantenlänge ist 1020 mm.
Der Preis wird aus den Maßen 1020 × 1020 mm = 1,04 qm berechnet.

Außerdem können Sie die Rundung der Zuschläge festlegen und verschiedene Zuschläge (E) zuordnen, z. B. für den Einbau von Stufen, für Übergrößen usw. Die Zuschläge werden in den dafür vorgesehenen Dialogen angelegt. Die Zuschläge werden in einer separaten Lerneinheit ausführlich beschrieben.
⇨ "Zuschläge" auf Seite C-632

Schließlich können Sie Austauschlisten (F) zuordnen, mit denen die Gläser berechnet werden, die im ISO eingetauscht werden. Um Austauschlisten zuzuordnen, müssen diese im Dialog Austausch-/Zusatzlisten angelegt sein. Die Listen werden in einer separaten Lerneinheit ausführlich beschrieben.
⇨ "Austausch- und Zusatzpreise" auf Seite C-614

Damit die ISO-Scheiben nach Ihren Definitionen berechnet werden, müssen Sie das Preiskennzeichen (PKZ) in den Tageskonditionen angeben. Die Konditionen sind in einer separaten Lerneinheit beschrieben.
⇨ "Konditionen" auf Seite C-645

### Übungen
Verwenden Sie für die Übung die Schlüssel, die Sie für die Schulung angelegt haben. Ergänzen Sie ggf. die Schlüssel für die Übungen. Verwenden Sie für das PLKZ und das PKZ nur Ihre Schulungsschlüssel.
- Legen Sie eine Preismatrix für einen ISO-Artikel an.
- Kopieren Sie für eine zweite Preismatrix die Preise und erhöhen Sie die kopierten Preise um 5 %.
- Ordnen Sie die neuen Matrizen den ISO-Artikeln zu.

## Preisvektoren

**Lernziele**
- Einsatzmöglichkeiten für Preisvektoren kennenlernen.
- Auswertung der Preisvektoren bei der Preissuche verstehen.

**Nutzen**
- Mit Preisvektoren können Preise sehr fein gestaffelt werden. Dabei muss jeweils der Artikel berücksichtigt werden, der über einen Preisvektor berechnet werden soll.
- Mit der Ab-PLKZ-Logik können Sie die Preissuche bei Vektorpreisen steuern.

**Merke**

| Begriff | Erklärung |
| :--- | :--- |
| **Artikelvektoren** | Sinnvollerweise haben Vektoren die gleiche Nummer wie der Artikel, dessen Preise in dem Vektor angelegt werden sollen. |
| **Bearbeitungsvektoren** | Bearbeitungsvektoren können zusätzlich nach Glasdicke, Warengruppe und Menge unterschieden werden. Bearbeitungspreise können alternativ auch in Matrizen definiert werden. |
| **Grenzwert** | Der Grenzwert gibt die Stufen einer Staffelung an. Abhängig von der Preisart beziehen sich die Grenzwerte auf Stückzahlen, Grundmengeneinheit, Fläche oder bei Bearbeitungen auf Kantenlängen. |
| **Maßrundung** | Für die Preisberechnung werden die Höhe und die Breite der Auftragsposition auf die nächsthöhere Länge in mm aufgerundet, die durch die angegebene Maßrundung teilbar ist. |
| **Mindestberechnung** | Bei Vektorpreisen können Mindestgrößen angegeben werden, z. B.:<br>- Mindestberechnung nach Mengeneinheiten aus den Artikelstammdaten.<br>- Mindestpreis pro Stück.<br>- Mindestkantenlänge pro Stück. |
| **PLKZ-Logik** | Für Vektorpreise gilt standardmäßig die Ab-PLKZ-Logik. Die Ab-PLKZ-Logik kann für einzelne Preislistenkennzeichen im Dialog Preislisten-Steuerung übersteuert werden. |
| **Vektor** | Eindimensionale Preistabelle zur Staffelung der Preise. Liste mit Preisen, die in der Regel nur von einem Wert abhängig sind, z. B. Stückzahl oder Quadratmeter. Vektoren, denen die Preisart 11- Variantenartig oder 12-Variantenstaffel zugeordnet ist, können auch von zwei Werten abhängig sein, z. B. Höhe und Breite. Vektoren werden für Artikel und Bearbeitungen angelegt. |
| **Voraussetzungen** | Schlüssel für Preislisten und Vektoren sind angelegt. |
| **Zuschläge** | Bei Vektorpreisen können Zuschläge angegeben werden, z. B.:<br>- Größenzuschläge für Flächenartikel<br>- Kleinglaszuschläge<br>- Überlängenzuschläge. |

### Vektorpreise
Vektoren sind eindimensionale Preistabellen. Der Preis ist in der Regel von einer einzigen Eingabegröße abhängig, z. B. der Stückzahl eines Artikels. Je nach Preismethode unterscheiden sich die Angaben für die Vektorpreise:
- Vektorpreise für Artikel
- Vektorpreise für Bearbeitungen
- Vektorpreise für VSG
- Preise für Farbartikel
- Variantenpreise
- Preise für Verglasung

*Abb. C-37 Preisdefinition für Vektor (Beispiel Artikelvektor)*

- **A** Vektornummer
- **B** Ab-PLKZ
- **C** Preisart
- **D** Mindestberechnung, -kantenlänge
- **E** Staffelung
- **F** Maßrundung
- **G** Mindestpreis
- **H** Preistyp

In diesem Beispiel sehen Sie einen Preisvektor für einen Artikel:
- Im Kopfbereich des Dialogs sind die Schlüssel (A, B) und die Preisart (C) angegeben.
- Dazu können die Mindestwerte (D), die Maßrundung (F) für die Berechnung von Glaspreisen und ein Mindestpreis (G) festgelegt werden.
- Je nach Preisart können Sie Grenzwerte für Preisstufen (E) angeben, z. B. für die Menge. In einem Vektor können Sie bis zu 30 Stufen festlegen.

#### Vektorpreise für Artikel
Mit Artikelvektoren können die Preise für Einfachgläser, VSG oder Zubehörartikel berechnet werden.
Vektornummern können identisch mit Artikelnummern sein. Dadurch entfällt eine Zuordnung. Wenn aber mehrere Artikel mit demselben Preisvektor berechnet werden sollen, müssen die Artikel dem Vektor zugeordnet werden.

> **Unterscheidung von bearbeiteten und unbearbeiteten Festmaßen**
> Wird die Artikelstruktur nach Lagermaßen, Festmaßen und bearbeiteten Festmaßen verwendet, ist es z. B. nicht nötig, Vektoren zur Aufnahme von Preisen für bearbeitete Festmaße festzulegen. Diese haben die gleichen Preise wie die unbearbeiteten Festmaße. Durch Zuordnung eines Artikels zu einem Vektor kann in einem solchen Fall auf die Grundpreise der unbearbeiteten Festmaße zugegriffen werden.

Bei den Artikelvektoren steuern Sie die Preisberechnung, indem Sie die Preisart festlegen. Die Preisart bestimmt, aus welcher Preisstufe der Preis verwendet werden soll, z. B. bei Staffelpreisen.
⇨ "Preistyp" auf Seite C-574

#### Vektorpreise für Bearbeitungen
Für Bearbeitungen werden die Preise ebenfalls in Vektoren angelegt. Die Bearbeitungsvektoren bieten die Möglichkeit, die Bearbeitungspreise auch nach der Dicke des Glases zu staffeln.

*Abb. C-38 Beispiel Bearbeitungsvektor*

- **A** Vektornummer
- **B** 2 Dicken pro PLKZ
- **C** Unterschiedliche Preistypen pro Dicke und PLKZ

In diesem Beispiel sehen Sie, dass mehrere Definitionen zu einem Bearbeitungsvektor (A) angelegt sind. Diese Definitionen unterscheiden sich durch die zugeordnete Preisliste, durch die Dicke (B) des Glases und durch den Preistyp (C). Zusätzlich kann, wie bei den Artikelvektoren, pro Definition eine Staffelung angegeben werden.

#### Vektorpreise für VSG
Für VSG werden die Preise ebenfalls in Vektoren angelegt. Die Zuordnung der Artikelpreisvektoren erfolgt über die VSG-Grundpreise. Dazu muss das VSG-Glas als Artikel mit dem Artikeltyp 170 oder 183 eingerichtet sein. Den Artikeln dieser Artikeltypen muss die Preismethode PKZ-VSG zugeordnet sein.

*Abb. C-39 Beispiel VSG*

- **A** Artikelnummer, Vektornummer
- **B** PLKZ

In diesem Beispiel sehen Sie, dass der VSG-Artikel und der Vektor (A) dieselbe Nummer haben. Der Vektor wird für mehrere Preislisten (B) gepflegt.

#### Preise für Farbartikel
Für Farbartikel werden die Preise pro Artikel und Farbe angelegt. Dazu müssen die Artikel als Farbartikel eingerichtet sein. Den Artikeln muss eine gültige Farbe und die Preismethode PKZ-Farbartikel zugeordnet sein.

*Abb. C-40 Beispiel Farbartikel*

- **A** Artikelnummer
- **B** Farbnummer

In diesem Beispiel sehen Sie, dass der Preis pro Farbartikel (A) und Farbe (B) angegeben ist.

