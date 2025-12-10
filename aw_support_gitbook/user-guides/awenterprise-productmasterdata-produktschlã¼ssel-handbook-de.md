---
title: "DE-HB-AWEnterprise_4"
source: "DE-HB-AWEnterprise_4.pdf"
tags: ["A+W Enterprise", "Software Reference", "Product Master Data", "Produktschlüssel", "Configuration", "Variants", "Technical Data", "ERP", "Bill of Materials", "Technical Values"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference guide for the 'Produktschlüssel' (Product Key) module within the A+W Enterprise system. It details the configuration of product master data, including variants, technical specifications, and other product-related settings."
long_description: "This comprehensive software reference manual provides detailed instructions for configuring the 'Produktschlüssel' (Product Key) module in the A+W Enterprise software. It covers a wide range of master data settings essential for managing products throughout their lifecycle, from creation to production and sales. The document explains how to define dimensional variants, size variants, and measurement designations. It provides an in-depth look at setting up complex 'Austausch-/Zusatzregeln' (exchange/add-on rules) which allow for dynamic bill of materials (BOM) modifications based on customer-specific or product-specific criteria. Furthermore, the manual details the configuration of technical value groups (e.g., sound insulation dB-groups, thermal properties U-groups) and their corresponding vectors for calculating product characteristics. It also covers settings for product certification (CEKAL, CPIP), declaration of performance, and various other specific attributes like fitting types, foil types, and frame types. The guide is intended for system administrators and advanced users responsible for maintaining the product master data in A+W Enterprise."
---

# Produktschlüssel

---
## Maßbezeichnungen

Stammdaten > Schlüssel > Produkte > Varianten > Maße > Einzelne Bezeichnung
Stammdaten > Schlüssel > Produkte > Varianten > Maße > Alle Bezeichnung

*Abb. B-124 Maßbezeichnungen*

In diesem Dialog definieren Sie die einzelnen Maßvarianten in den verschiedenen Sprachen.

### Erläuterung der Felder

**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Mengeneinheit geben Sie die nächste freie Nummer ein.
Technische Info: `<F9>`, DB-Feld: xsprbez.id
view: xxvar.bitnr

**ME**
Auswahl der Mengeneinheit. Die Schlüssel werden im Menü Mengeneinheiten (Schlüssel > System) hinterlegt.
Technische Info: `<F9>`, DB-Feld: xsprbez.id2

**Spr**
Sprachkennzeichen.
Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz

**Variantentext**
Bezeichnung der Variante.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

**Lagerbez.**
Bezeichnung eines Stückes im Lager.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez2

### Ergänzende Informationen

⇨ "Mengeneinheitenbezeichnung" auf Seite B-247

## Größenvarianten

Stammdaten > Schlüssel > Produkte > Varianten > Größen > Größenvarianten

*Abb. B-125 Größenvarianten*

In diesem Dialog definieren Sie die einzelnen Größenvarianten.

### Erläuterung der Felder

**Nr**
Auswahl der Dicke-/Größenvariante im ISO. Zum Anlegen einer neuen Dickenvariante geben Sie die nächste freie Nummer ein.
Technische Info: Numerisches Feld, DB-Feld: xxdicke.dicke

**Bezeichnung**
Bezeichnung, z. B. 12 mm
Technische Info: Alphanumerisches Feld

**Dicke**
Dicke der Variante in der festgelegten Mengeneinheit.
Technische Info: Numerisches Feld, DB-Feld: xxdicke.dickenmass

### Ergänzende Informationen

⇨ “Größenbezeichnungen" auf Seite B-303

## Größenbezeichnungen

Stammdaten > Schlüssel > Produkte > Varianten > Größen > Einzelne Bezeichnung
Stammdaten > Schlüssel > Produkte > Varianten > Größen > Alle Bezeichnung

*Abb. B-126 Größenbezeichnungen*

In diesem Dialog definieren Sie die einzelnen Größenbezeichnungen in den verschiedenen Sprachen.

### Erläuterung der Felder

**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Qualität geben Sie die nächste freie Nummer ein.
Technische Info: `<F9>`, DB-Feld: xsprbez.id
view: xxvar.bitnr

**Spr**
Sprachkennzeichen.
Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz

**Bezeichnung**
Bezeichnung der Größe, z. B. 2 mm.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1
view: xxvar.atxt

### Ergänzende Informationen

⇨ "Größenbezeichnungen" auf Seite B-303

## Austausch-/Zusatzregeln

Stammdaten > Schlüssel > Produkte > Austausch-/Zusatzregeln

*Abb. B-127 Austausch-/Zusatzregeln*

Der Menüpunkt Austausch-/Zusatzregel ermöglicht es, kundenspezifische Regeln, nach denen im Auftrag die Stückliste ergänzt bzw. Teile ausgetauscht werden sollen, für einzelne Artikel oder Artikeltypen zu hinterlegen. Dabei wird auf der linken Dialogseite der Artikel bzw. der Artikeltyp ausgewählt, für den die auf der rechten Dialogseite festgelegte Regel gilt.

Der Dialog besteht aus den Registern:
- Austausch-/Zusatzregeln
- Details
- Testmodus

### Erläuterung der Felder im Bereich Es gilt für ...

**Knd-Artnr**
Wenn das Feld Kunden-Artikelnummer gefüllt ist, wird die Regel bei der Erfassung nur dann ausgewertet, wenn die Erfassung der Position über den Kundenartikel erfolgt. Auch dann, wenn zufällig für den A+W Enterprise-Artikel und Kunden eine eindeutige Zuordnung besteht.
Technische Info: `<F9>`, DB-Feld: kuaz.kuartnr

**ProdTyp**
Das Feld wird mit dem Artikeltyp vom Kopfartikel gefüllt. Das Feld muss nicht zwingend ausgefüllt werden, sondern nur, wenn die Regel spezifisch für den Artikeltyp anzuwenden ist.
Technische Info: `<F9>`, DB-Feld: kuaz.prodtyp

**Produkt**
Das Feld wird mit dem Kopfartikel gefüllt. Es muss nicht zwingend ausgefüllt werden, sondern nur, wenn die Regel spezifisch für den Artikel anzuwenden ist.
Technische Info: `<F9>`, DB-Feld: kuaz.prodnr

**1x**
Über die Checkbox steuern Sie, ob die Regel nur einmal oder immer angewendet wird.
- Die Regel wird nur einmal im Produkt ausgeführt. Dadurch können Sie ermöglichen, dass im ISO ein Float z. B. 110005 gegen ein bearbeitetes Float 150005 getauscht wird, auch wenn dieses bearbeitete Float selbst in der Stückliste den Artikel 110005 hat. Anschließend werden keine Austauschregeln angewendet.
- Die Regel wird immer angewendet.
Technische Info: Toggle-Feld, DB-Feld: kuaz.einmal

**Atyp**
Das Feld Artikeltyp ist ein Alternativ-Feld, das, welches Teil ausgetauscht werden soll oder wo ein Artikel ein zusätzliches Element bekommt oder ein Element entfernt wird.
Technische Info: `<F9>`, DB-Feld: kuaz.atyp

**Artikel**
Das Feld Artikel ist ein Alternativ-Feld, das angibt, welcher Artikel ausgetauscht werden soll oder wo ein Artikel ein zusätzliches Element bekommt oder ein Element entfernt wird. Hier können Sie auch durch besonders definierte Angaben die Regel noch allgemeiner darstellen. So gilt die Regel für alle FM-Artikel (Artikeltyp 100 bis 175), wenn in diesem Feld eine -1 steht. Für alle FM-Artikel ohne VSG (Artikeltyp 100 bis 160) bei -2 und FM-Artikel ohne VSG, ESG und Brandschutz (Artikeltyp 100 bis 140) bei -3.
Technische Info: `<F9>`, DB-Feld: kuaz.artnr

**EP**
Das Ausfüllen des Feldes Einbauposition hat eine enorme Bedeutung. Besonders bei Glasartikeln oder Rahmen. Diese Eingabe muss mit den Eingaben für EP auf der rechten Seite der Regel korrespondieren. Soll der Austausch allgemein gelten, unabhängig von der Einbauposition innerhalb der Stückliste, so kann EP auf der linke Seite weggelassen werden. Dann sollte aber auch die Eingabe auf der rechten Seite nicht folgen. Weiter ist es sehr wichtig, dass die Einbaupositionen im Stamm gut gepflegt sind. Für den Austausch von Rahmenartikel muss zwingend eine Einbauposition angegeben werden.
Technische Info: Numerisches Feld, DB-Feld: kuaz.orgpos

**Bereich**
Im Feld Bereich geben Sie an, wann eine Regel greifen soll: nur für einen Kopfartikel bzw. Unterteil, immer oder nie (leer). Bsp.: Es soll ein Artikel Stempel1 in ein ESG als Zusatzartikel eingefügt werden, aber nur, wenn das ESG als Kopfartikel erfasst wird (nicht wenn das ESG Bestandteil eines ISO ist). Oder es soll ein Artikel Stempel2 in ein ESG als Zusatzartikel eingefügt werden, aber nur wenn das ESG Bestandteil eines anderen Artikel ist (nicht wenn das ESG als Kopfartikel erfasst wird). Folgende Werte sind möglich:
- nur Kopf
- U-Teil
- immer
- leer.
Technische Info: `<F9>`, DB-Feld: kuaz.kopfflag

### Erläuterung der Felder im Bereich die Regel

**Artikel**
Wählen Sie den Artikel aus, der als Zusatz in die Stückliste eingefügt werden soll, bzw. als neuer Artikel eingetauscht werden oder auch gelöscht werden soll.
Technische Info: `<F9>`, DB-Feld: kuaz.azartnr

**A/Z**
Über das Toggle legen Sie die Aktion fest. Folgende Werte sind möglich:
- A: Austausch, tauscht einen Artikel gegen einen anderen Artikel.
- Z: Zusatz, fügt in die Stücklist des Artikels (linke Seite) einen neuen Artikel hinzu.
Technische Info: Toggle-Feld, DB-Feld: kuaz.azkz

**EP**
Das Ausfüllen dieses Feldes hat eine enorme Bedeutung. Besonders bei Glasartikeln oder Rahmen. Diese Eingabe muss mit den Eingaben für EP auf der rechten Seite der Regel korrespondieren. Soll der Austausch allgemein gelten, unabhängig von der Einbauposition innerhalb der Stückliste, so kann EP auf der linke Seite weggelassen werden. Dann sollte aber auch die Eingabe auf der rechten Seite nicht folgen. Weiter ist es sehr wichtig, dass die Einbaupositionen im Stamm gut gepflegt sind. Für den Austausch von Rahmenartikel muss zwingend eine Einbauposition angegeben werden. Folgende Werte sind mögliche:
- 1: Wetterseite: Struktur nach außen
- 2: Wetterseite: Struktur zum Luftzwischenraum
- 3: Innenseite: Struktur zum Luftzwischenraum
- 4: Innenseite: Struktur nach innen
Technische Info: Numerisches Feld, DB-Feld: kuaz.orgpos

**Struktur**
Falls ein Strukturglas eingetragen wurde, steuern Sie über das Toggle-Feld die Strukturrichtung:
- horizontal
- vertikal
- diagonal
- keine
Technische Info: Numerisches Feld, DB-Feld: kuaz.strukthb

**A1**
Benötigte Menge 1. Bei Sprossen wird hier die Menge der senkrechten Sprossen eingegeben. Bei Flächen-Bearbeitungen (z. B. Kanten schleifen) wird hier die Anzahl der Kanten eingetragen, die als Breite festgelegt werden. Bei Stück-Bearbeitungen (z. B. Bohrungen) wird die Anzahl der Bearbeitung eingetragen. Modelle sind besonders zu beachten (Kantenzuordnung).
Technische Info: Numerisches Feld, DB-Feld: kuaz.anz1

**A2**
Benötigte Menge 2. Bei Sprossen wird hier die Menge der waagerechten Sprossen eingegeben. Bei Flächen-Bearbeitungen (z. B. Kanten schleifen) wird hier die Anzahl der Kanten eingetragen, die als Höhe festgelegt werden. Bei Stück-Bearbeitungen (z. B. Bohrungen) wird hier nichts eingetragen. Modelle sind besonders zu beachten (Kantenzuordnung).
Technische Info: Numerisches Feld, DB-Feld: kuaz.anz2

**D**
Das Druck-Kennzeichen in diesem Feld bestimmt, welches Druck-Kennzeichen der Artikel in der Stückliste bekommt:
- N: Nein
- J: Ja
- V: Verkaufsseitige Papiere
- P: Produktionspapiere
Technische Info: Toggle-Feld, DB-Feld: kuaz.druckkz

**P**
Das Feld Preisauswirkung bestimmt, ob der Artikel ein Zusatz- Kennzeichen in der Stückliste bekommen soll und damit in die Preisberechnung einfließt. Die Ausprägung "O" bedeutet, dass das Original-Kennzeichen übernommen wird. Stand der ausgetauschte Artikel in der Stammstückliste wegen der Preisberechnung auf A/Z, so wird auch der neue Artikel das Kennzeichen erben. Folgende Werte sind möglich:
- Ο: Original-Kennzeichen wird übernommen. Bei einer Zusatzregel ist diese Einstellung nicht sinnvoll. Daher wird in solchen Fällen automatisch der Wert J (Ja) gesetzt.
- J: Ja
- N: Nein, nicht gesetzt.
- A: Austausch, A/Z-Preiskennzeichen Austausch
- Z: Zusatz, A/Z-Preiskennzeichen Zusatz
Technische Info: Toggle-Feld, DB-Feld: kuaz.azpreis

## Austausch-/Zusatzregel - Details

Stammdaten > Schlüssel > Produkte > Austausch-/Zusatzregeln > <F2>

*Abb. B-128 Austausch-/Zusatzregeln, Register Details*

In diesem Register werden Ihnen detaillierte Informationen zu den Austausch- bzw. Zusatzregeln angezeigt.
Sie können beim Anlegen einer Regel schon alle für den Artikel vorgesehenen Bearbeitungsparameter mitgeben. Neben jedem Parameterfeld befindet sich eine Checkbox, um auswählen zu können, ob der jeweilige Parameter ausgewertet werden soll. Das ist sehr wichtig, wenn durch eine Austausch-/Zusatzregel ein Artikel auch 0 als gültiges Bearbeitungsmaß (bzw. Anzahl) übernehmen kann.

> **Felder im unteren Bereich**
> In Abhängigkeit der eingegebenen Daten, können im unteren Bereich Felder und deren Bezeichnungen ein- oder ausgeblendet werden!

### Erläuterung der Felder

Die Felder im Bereich Es gilt für..., Zwischenebene und Hauptebene werden mit den Daten aus dem Register Austausch-/Zusatzregeln gefüllt.
**A/Z-Modus**
Über das Toggle legen Sie die Aktion fest. Folgende Werte sind möglich:
- A: Austausch, tauscht einen Artikel gegen einen anderen Artikel.
- Z: Zusatz, fügt in die Stücklist des Artikels (linke Seite) einen neuen Artikel hinzu.
Technische Info: Toggle-Feld, DB-Feld: kuaz.azkz

**Einbaupos**
Zeigt die Einbauposition, wie sie im Register Austausch-/Zusatzregeln definiert wurde.
Technische Info: Anzeige-Feld, DB-Feld: kuaz.pos

**Farbe**
Farbnummer.
Technische Info: Anzeige-Feld, DB-Feld: kuaz.farbnr

**Struktur**
Richtung bei Strukturglas.
Technische Info: Toggle-Feld, DB-Feld: kuaz.strukthb

**Drucken**
Druckkennzeichen, wie es im Register Austausch-/Zusatzregeln definiert wurde.
Technische Info: `<F9>`, DB-Feld: kuaz.druckkz

**A/Z-Preis**
Preisauswirkung, wie sie im Register Austausch-/Zusatzregeln definiert wurde.
Technische Info: `<F9>`, DB-Feld: kuaz.azpreis

**Beschaffart**
Die Beschaffungsart:
- 1: Bestellung vor DFÜ
- 2: Lagerentnahme vor DFÜ
- 3: Produktion vor DFÜ
- 4: Bestellung
- 5: Lagerentnahme
- 6: Produktion
- 7: Mitgeliefert
- 8: n. verfügbar
- 9: Mitgeliefert vor DFÜ
Technische Info: Numerisches Feld, DB-Feld: kuaz.beschaffart

**Lieferant**
Nummer des Lieferanten. Das Feld ist nur aktiv, wenn im Feld Beschaffart die Methode Bestellung vor DFÜ oder Bestellung gewählt wurde.
Technische Info: `<F9>`, DB-Feld: kuaz.linr

**Vermaßungstyp**
Der Vermaßungstyp sowie alle darunter liegenden Felder der mittleren und rechten Spalte sind abhängig von dem A+W Bearbeitungstyp. Weitere Informationen erhalten Sie im A+W Normierten Bearbeitungskatalog. Die Checkboxen hinter den jeweiligen Feldern steuern, ob die Parameter ausgewertet werden sollen oder nicht.
Technische Info: `<F9>`, DB-Feld: kuaz.mtyp

## Austausch-/Zusatzregel - Testmodus

Stammdaten > Schlüssel > Produkte > Austausch-/Zusatzregeln > <F2> <F2>

*Abb. B-129 Austausch-/Zusatzregel, Register Testmodus*

In diesem Register haben Sie die Möglichkeit, die Auswirkung der Austausch-/Zusatzregel zu überprüfen. Hierzu markieren Sie die zu überprüfende Regel in der letzten Spalte und starten den Test mit `<F5>` oder über die Schaltfläche [Test]. Es erscheint ein Werteingabe-Dialog in dem Sie den gewünschten Artikel eintragen.

*Abb. B-130 Testmodus*

Nach der Bestätigung der Nummer wird eine Pseudo-Erfassung simuliert und die Stückliste angezeigt.

*Abb. B-131 Testmodus, Stückliste*

Hier können Sie sofort kontrollieren, ob der Austausch (markierte Regel 1) und Zusatz (markierte Regel 2) durchgeführt wird. Wenn durch Austausch-/Zusatzregel auch die Bearbeitungsparameter bestimmt wurden, dann können Sie dies auch an der SN-Skizze sehen.

## dB-Gruppen

Stammdaten > Schlüssel > Produkte > Technische Werte > Gruppen > Schalldämmung (dB) > Einzelne Bezeichnung
Stammdaten > Schlüssel > Produkte > Technische Werte > Gruppen > Schalldämmung (dB) > Alle Bezeichnung

*Abb. B-132 Gruppen für Schalldämmung (dB)*

In diesem Bereich haben Sie die Möglichkeit, Gläser mit gleichen Schalldämmeigenschaften zu Gruppen zusammenzufassen.
Dieser Dialog enthält die dB-Gruppen in den jeweiligen Sprachen.

### Erläuterung der Felder

**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen dB-Gruppe geben Sie die nächste freie Nummer ein.
Technische Info: `<F9>`, DB-Feld: xsprbez.id

**Spr**
Sprachkennzeichen.
Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz

**Bezeichnung**
Bezeichnung der dB-Gruppe, z. B. nach DIN 12037.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

## U-Gruppen

Stammdaten > Schlüssel > Produkte > Technische Werte > Gruppen > Thermische Eigenschaften (U) > Einzelne Bezeichnung
Stammdaten > Schlüssel > Produkte > Technische Werte > Gruppen > Thermische Eigenschaften (U) > Alle Bezeichnung

*Abb. B-133 Gruppen für thermische Eigenschaften (U)*

In diesem Bereich haben Sie die Möglichkeit, Gläser mit gleichen thermischen Eigenschaften zu Gruppen zusammenzufassen. U-Gruppen werden zur Beschreibung technischer Werte verwendet.
Dieser Dialog enthält die U-Gruppen in den jeweiligen Sprachen.

### Erläuterung der Felder

**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen U-Gruppe geben Sie die nächste freie Nummer ein.
Technische Info: `<F9>`, DB-Feld: xsprbez.id

**Spr**
Sprachkennzeichen.
Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz

**Bezeichnung**
Bezeichnung der U-Gruppe, z. B. nach DIN 12041.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

## g-Gruppen

Stammdaten > Schlüssel > Produkte > Technische Werte > Gruppen > Gesamtenergiedurchlass (g) > Einzelne Bezeichnung
Stammdaten > Schlüssel > Produkte > Technische Werte > Gruppen > Gesamtenergiedurchlass (g) > Alle Bezeichnung

*Abb. B-134 Gruppen für Gesamtenergiedurchlass*

In diesem Bereich haben Sie die Möglichkeit, Gläser mit gleichem Gesamtenergiedurchlass zu Gruppen zusammenzufassen.
Dieser Dialog enthält die g-Gruppen in den jeweiligen Sprachen.

### Erläuterung der Felder

**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen g-Gruppe geben Sie die nächste freie Nummer ein.
Technische Info: `<F9>`, DB-Feld: xsprbez.id

**Spr**
Sprachkennzeichen.
Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz

**Bezeichnung**
Bezeichnung der g-Gruppe, z. B. nach DIN 37.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

## Transmissionsgruppen

Stammdaten > Schlüssel > Produkte > Technische Werte > Gruppen > Transmission > Einzelne Bezeichnung
Stammdaten > Schlüssel > Produkte > Technische Werte > Gruppen > Transmission > Alle Bezeichnung

*Abb. B-135 Transmissionsgruppen*

In diesem Bereich haben Sie die Möglichkeit, Gläser mit gleichen Lichtdurchlasseigenschaften zu Gruppen zusammenzufassen.
Dieser Dialog enthält die Transmissions-Gruppen in den jeweiligen Sprachen.

### Erläuterung der Felder

**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen T-Gruppe geben Sie die nächste freie Nummer ein.
Technische Info: `<F9>`, DB-Feld: xsprbez.id

**Spr**
Sprachkennzeichen.
Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz

**Bezeichnung**
Bezeichnung der Gruppe, z. B. Nach DIN 12037.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

## Maßrestriktions-Gruppen

Stammdaten > Schlüssel > Produkte > Technische Werte > Gruppen > Maßrestriktionen > Einzelne Bezeichnung
Stammdaten > Schlüssel > Produkte > Technische Werte > Gruppen > Maßrestriktionen > Alle Bezeichnung

*Abb. B-136 Maßrestriktions-Gruppen*

In diesem Bereich haben Sie die Möglichkeit, Gläser mit gleichen Maßrestriktionen zu Gruppen zusammenzufassen.
Dieser Dialog enthält die Maßrestriktions-Gruppen in den jeweiligen Sprachen.

### Erläuterung der Felder

**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Maßrestriktions-Gruppe geben Sie die nächste freie Nummer ein.
Technische Info: `<F9>`, DB-Feld: xsprbez.id

**Spr**
Sprachkennzeichen.
Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz

**Bezeichnung**
Bezeichnung der Maßrestriktions-Gruppe, z. B. Kategorie 8.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

## Dickengruppen

Stammdaten > Schlüssel > Produkte > Technische Werte > Gruppen > Dicken > Einzelne Bezeichnung
Stammdaten > Schlüssel > Produkte > Technische Werte > Gruppen > Dicken > Alle Bezeichnung

*Abb. B-137 Dickengruppen*

In diesem Bereich haben Sie die Möglichkeit, Gläser mit gleichen Dicken zu Gruppen zusammenzufassen.
Dieser Dialog enthält die Dicken-Gruppen in den jeweiligen Sprachen.

### Erläuterung der Felder

**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Dicken-Gruppe geben Sie die nächste freie Nummer ein.
Technische Info: `<F9>`, DB-Feld: xsprbez.id

**Spr**
Sprachkennzeichen.
Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz

**Bezeichnung**
Bezeichnung der Dicken-Gruppe, z. B. Dicke 1.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

## Biegefestigkeitsgruppen

Stammdaten > Schlüssel > Produkte > Technische Werte > Biegefestigkeit

*Abb. B-138 Biegefestigkeitsgruppen*

In diesem Bereich haben Sie die Biegefestigkeit der Gläser fest.

### Erläuterung der Felder

**Gruppe**
Schlüssel-Feld. Zum Anlegen einer neuen Biegefestigkeit-Gruppe geben Sie eine freie Nummer ein.
Technische Info: Nummerisches Feld, DB-Feld: xbfgrp.grp

**Bezeichnung**
Bezeichnung der Gruppe.
Technische Info: `<F9>`, DB-Feld: xbfgrp.bez

**Wert**
Wert der Biegefestigkeit-Gruppe.
Technische Info: Alphanumerisches Feld, DB-Feld: xbfgrp.wert

## Vektoren für Schalldämmung (dB)

Stammdaten > Schlüssel > Produkte > Technische Werte > Vektoren > Schalldämmung (dB)
Stammdaten > Schlüssel > Produkte > Technische Werte > Vektoren > Schalldämmung (dB) > F2

*Abb. B-139 Vektoren für Schalldämmung (dB)*

Die dB-Vektoren dienen der Ermittlung des Schalldämmwertes für einen bestimmten Produktaufbau, bei dem bis zu drei Scheiben miteinander kombiniert werden können.
Sie werden entweder für einen konkreten Glasaufbau oder pauschal für Gläser der jeweiligen Gruppe angelegt. Eine Kombination ist nicht möglich.

### Erläuterung der Felder

**Glas1**
Auswahl der dB-Gruppe oder Eingabe der Artikelnummer der Scheibe 1. Zum Anlegen eines neuen Vektors gehen Sie in die nächste freie Zeile (<Enter>).
Technische Info: `<F9>`, DB-Feld: xtechwdb.glas1

**Glas2**
Auswahl der dB-Gruppe oder Eingabe der Artikelnummer der Scheibe 2.
Technische Info: `<F9>`, DB-Feld: xtechwdb.glas2

**Glas3**
Auswahl der dB-Gruppe oder Eingabe der Artikelnummer der Scheibe 3.
Technische Info: `<F9>`, DB-Feld: xtechwdb.glas3

**SZR1/bis**
Hier können Sie für einen Scheibenzwischenraum einen Bereich von SZR 1 (untere Grenze) jeweils bis zum maximalen Scheibenzwischenraum (obere Grenze) eingeben.
Technische Info: Numerisches Feld, DB-Feld: xtechwdb.szr1

**SZR2/bis**
Bei dreifach-Produkten kann für einen Scheibenzwischenraum ein Bereich von SZR 2 (untere Grenze) jeweils bis zum maximalen Scheibenzwischenraum (obere Grenze) eingegeben werden.
Technische Info: Numerisches Feld, DB-Feld: xtechwdb.szr2

**Gas1/2**
Auswahl der Gas-Artikelnummer für die Zwischenräume.
Technische Info: `<F9>`, DB-Feld: xtechwdb.gas1/2

**RW-Wert**
Die Kombination dieser Faktoren ergibt den dB-Wert der Einheit (Dämpfung in dB).
Technische Info: `<F9>`, DB-Feld: xtechwdb.dbwert

**Schalldämmung c**
Eingabe der Schalldämmung c.
Technische Info: Numerisches Feld, DB-Feld: xtechwdb.cwert

**Schalldämmung ctr**
Eingabe der Schalldämmung ctr.
Technische Info: Numerisches Feld, DB-Feld: xtechwdb.ctrwert

## Vektoren für thermische Eigenschaften (U)

Stammdaten > Schlüssel > Produkte > Technische Werte > Vektoren > Thermische Eigenschaften (U)

*Abb. B-140 Thermische Eigenschaften (U)*

Die U-Vektoren dienen der Ermittlung des Wärmedurchgangskoeffizienten für einen bestimmten Produktaufbau, bei dem bis zu drei Scheiben miteinander kombiniert werden können.
Sie werden entweder für einen konkreten Glasaufbau oder pauschal für Gläser der jeweiligen Gruppe angelegt. Eine Kombination ist nicht möglich.

### Erläuterung der Felder

**Glas1**
Auswahl der U-Gruppe oder Eingabe der Artikelnummer der Scheibe 1. Zum Anlegen eines neuen Vektors gehen Sie in die nächste freie Zeile (<Enter>).
Technische Info: `<F9>`, DB-Feld: xtechwk.glas1

**Glas2**
Auswahl der U-Gruppe oder Eingabe der Artikelnummer der Scheibe 2.
Technische Info: `<F9>`, DB-Feld: xtechwk.glas2

**Glas3**
Auswahl der U-Gruppe oder Eingabe der Artikelnummer der Scheibe 3.
Technische Info: `<F9>`, DB-Feld: xtechwk.glas3
**SZR1/bis**
Hier können Sie für einen Scheibenzwischenraum einen Bereich von SZR 1 (untere Grenze) jeweils bis zum maximalen Scheibenzwischenraum (obere Grenze) eingeben.
Technische Info: Numerisches Feld, DB-Feld: xtechwk.szr1

**SZR2/bis**
Bei dreifach-Produkten kann für einen Scheibenzwischenraum ein Bereich von SZR 2 (untere Grenze) jeweils bis zum maximalen Scheibenzwischenraum (obere Grenze) eingegeben werden.
Technische Info: Numerisches Feld, DB-Feld: xtechwk.szr2

**Gas1/2**
Auswahl der Gas-Artikelnummer für die Zwischenräume.
Technische Info: `<F9>`, DB-Feld: xtechwk.gas1/2

**Ug-Wert**
Die Kombination dieser Faktoren ergibt den Ug-Wert der Einheit (Wärmedurchgangskoeffizient).
Technische Info: Numerisches Feld, DB-Feld: xtechwk.kwert

**k-Wert DIN**
Dieses Feld wird nicht mehr verwendet.

## Vektoren für Gesamtenergiedurchlass (g)

Stammdaten > Schlüssel > Produkte > Technische Werte > Vektoren > Gesamtenergiedurchlass (g)

*Abb. B-141 Gesamtenergiedurchlass (g)*

Die g-Vektoren dienen der Ermittlung des Energiedämmwertes für einen bestimmten Produktaufbau, bei dem bis zu drei Scheiben miteinander kombiniert werden können.
Sie werden entweder für einen konkreten Glasaufbau oder pauschal für Gläser der jeweiligen Gruppe angelegt. Eine Kombination ist nicht möglich.

### Erläuterung der Felder

**Glas1**
Auswahl der g-Gruppe oder Eingabe der Artikelnummer der Scheibe 1. Zum Anlegen eines neuen Vektors gehen Sie in die nächste freie Zeile (<Enter>).
Technische Info: `<F9>`, DB-Feld: xtechwg.glas1

**EP**
Eingabe der Einbauposition, d. h., wie das Glas im Produkt eingebaut ist.
Technische Info: Numerisches Feld, DB-Feld: xtechwg.glas1ep

**Glas2**
Auswahl der g-Gruppe oder Eingabe der Artikelnummer der Scheibe 2.
Technische Info: `<F9>`, DB-Feld: xtechwg.glas2

**EP**
Eingabe der Einbauposition, d. h., wie das Glas im Produkt eingebaut ist.
Technische Info: Numerisches Feld, DB-Feld: xtechwg.glas2ep

**Glas3**
Auswahl der g-Gruppe oder Eingabe der Artikelnummer der Scheibe 3.
Technische Info: `<F9>`, DB-Feld: xtechwg.glas3
**EP**
Eingabe der Einbauposition, d. h., wie das Glas im Produkt eingebaut ist.
Technische Info: Numerisches Feld, DB-Feld: xtechwg.glas3ep

**g-Wert**
Die Kombination dieser Faktoren ergibt den g-Wert der Einheit (Energiedämmwert).
Technische Info: Numerisches Feld, DB-Feld: xtechwg.gwert

## Vektoren für Transmission

Stammdaten > Schlüssel > Produkte > Technische Werte > Vektoren > Transmission

*Abb. B-142 Transmissions-Vektoren*

Die Transmissions-Vektoren dienen der Ermittlung des Lichtdurchlasswertes für einen bestimmten Produktaufbau, bei dem bis zu drei Scheiben miteinander kombiniert werden können.
Sie werden entweder für einen konkreten Glasaufbau oder pauschal für Gläser der jeweiligen Gruppe angelegt. Eine Kombination ist nicht möglich.

### Erläuterung der Felder

**Glas1**
Auswahl der Transmissions-Gruppe oder Eingabe der Artikelnummer der Scheibe 1. Zum Anlegen eines neuen Vektors gehen Sie in die nächste freie Zeile (<Enter>).
Technische Info: `<F9>`, DB-Feld: xtechwtr.glas1

**Glas2**
Auswahl der Transmissions-Gruppe oder Eingabe der Artikelnummer der Scheibe 2.
Technische Info: `<F9>`, DB-Feld: xtechwtr.glas2

**Glas3**
Auswahl der Transmissions-Gruppe oder Eingabe der Artikelnummer der Scheibe 3.
Technische Info: `<F9>`, DB-Feld: xtechwtr.glas3

**SZR1/bis**
Hier können Sie für einen Scheibenzwischenraum einen Bereich von SZR 1 (untere Grenze) jeweils bis zum maximalen Scheibenzwischenraum (obere Grenze) eingeben.
Technische Info: Numerisches Feld, DB-Feld: xtechwtr.szr1
**SZR2/bis**
Bei dreifach-Produkten kann für einen Scheibenzwischenraum ein Bereich von SZR 2 (untere Grenze) jeweils bis zum maximalen Scheibenzwischenraum (obere Grenze) eingegeben werden.
Technische Info: Numerisches Feld, DB-Feld: xtechwtr.szr2

**Gas1/2**
Auswahl der Gas-Artikelnummer für die Zwischenräume.
Technische Info: `<F9>`, DB-Feld: xtechwtr.gas1/2

**T-Wert**
Die Kombination dieser Faktoren ergibt den Transmissions-Wert der Einheit (Lichtdurchlasswert).
Technische Info: Numerisches Feld, DB-Feld: xtechwk.kwert

## Vektoren für Maßrestriktionen

Stammdaten > Schlüssel > Produkte > Technische Werte > Vektoren > Maßrestriktionen
Stammdaten > Schlüssel > Produkte > Technische Werte > Vektoren > Maßrestriktionen > F2

*Abb. B-143 Maßrestriktionen*

Die Maßrestriktions-Vektoren dienen der Ermittlung der Maximalgrößen für einen bestimmten Produktaufbau, bei dem bis zu drei Scheiben miteinander kombiniert werden können.
Sie werden entweder für einen konkreten Glasaufbau oder pauschal für Gläser der jeweiligen Gruppe angelegt. Eine Kombination ist nicht möglich.

### Erläuterung der Felder

**Glas1**
Auswahl der Maßrestriktions-Gruppe oder Eingabe der Artikelnummer der Scheibe 1. Zum Anlegen eines neuen Vektors gehen Sie in die nächste freie Zeile (<Enter>).
Technische Info: `<F9>`, DB-Feld: prodgrenz.glas1

**Glas2**
Auswahl der Maßrestriktions-Gruppe oder Eingabe der Artikelnummer der Scheibe 2.
Technische Info: `<F9>`, DB-Feld: prodgrenz.glas2

**Glas3**
Auswahl der Maßrestriktions-Gruppe oder Eingabe der Artikelnummer der Scheibe 3.
Technische Info: `<F9>`, DB-Feld: prodgrenz.glas3

**SZR1**
Entsprechend der Anzahl Scheiben kann ein Scheibenzwischenraum eingegeben werden.
Technische Info: Numerisches Feld, DB-Feld: prodgrenz.szr1

**SZR2**
Entsprechend der Anzahl Scheiben kann ein Scheibenzwischenraum eingegeben werden.
Technische Info: Numerisches Feld, DB-Feld: prodgrenz.szr2

**Gas1/2**
Auswahl der Gas-Artikelnummer für die Zwischenräume.
Technische Info: `<F9>`, DB-Feld: prodgrenz.gas1/2

**Breite**
Maximale und minimale Werte für die Breite.
Technische Info: Numerisches Feld, DB-Feld: prodgrenz.maxb/minb

**Höhe**
Maximale und minimale Werte für die Höhe.
Technische Info: Numerisches Feld, DB-Feld: prodgrenz.maxh/minh

**Fläche**
Maximale und minimale Werte für die Fläche.
Technische Info: Numerisches Feld, DB-Feld: prodgrenz.maxfl/minfl

**Seitenverhältnis**
Maximales und minimales Seitenverhältnis.
Technische Info: Numerisches Feld, DB-Feld: prodgrenz.maxsv/minsv

## Vektoren für Windlast

Stammdaten > Schlüssel > Produkte > Technische Werte > Vektoren > Windlast

*Abb. B-144 Windlast-Vektoren*

Die Windlast-Vektoren dienen der Ermittlung der Maximalgrößen für einen bestimmten Produktaufbau, bei dem bis zu drei Scheiben miteinander kombiniert werden können. Sie kommen insbesondere an Küsten oder Häfen zur Anwendung.
Sie werden entweder für einen konkreten Glasaufbau oder pauschal für Gläser der jeweiligen Gruppe angelegt. Eine Kombination ist nicht möglich.

### Erläuterung der Felder

**Glas1**
Auswahl der Dicken-Gruppe oder Eingabe der Artikelnummer der Scheibe 1. Zum Anlegen eines neuen Vektors gehen Sie in die nächste freie Zeile (<Enter>).
Technische Info: `<F9>`, DB-Feld: xtechwwl.dgrp1

**Glas2**
Auswahl der Dicken-Gruppe oder Eingabe der Artikelnummer der Scheibe 2.
Technische Info: `<F9>`, DB-Feld: xtechwwl.dgrp2

**Glas3**
Auswahl der Dicken-Gruppe oder Eingabe der Artikelnummer der Scheibe 3.
Technische Info: `<F9>`, DB-Feld: xtechwwl.dgrp3

**Bereich**
Einbaubereich:
- Zentral
- Rand
Das Feld wird nur ausgewertet, wenn es eine Auswahl enthält.
Technische Info: Toggle-Feld, DB-Feld: xtechwwl.bereich
**Fläche**
Scheibenfläche.
Technische Info: Numerisches Feld, DB-Feld: xtechwwl.qm

**Windlast**
Eingabe der Windlast.
Technische Info: Numerisches Feld, DB-Feld: xtechwwl.wlast

## Notifizierungsstellen

Stammdaten > Schlüssel > Produkte > Technische Werte > Notifizierungsstellen > Einzelne Bezeichnung
Stammdaten > Schlüssel > Produkte > Technische Werte > Notifizierungsstellen > Alle Bezeichnung

*Abb. B-145 Notifizierungsstellen*

In diesem Bereich beschreiben Sie die benötigte Notifizierungsstellen.
Dieser Dialog enthält die Bezeichnungen für die jeweiligen Notifizierungsstellen in den jeweiligen Sprachen.

### Erläuterung der Felder

**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Notifizierungsstellen geben Sie eine freie Nummer ein.
Technische Info: `<F9>`, DB-Feld: xsprbez.id

**Spr**
Sprachkennzeichen.
Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz

**Bezeichnung**
Bezeichnung der Notifizierungsstellen.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

## Produktnormen

Stammdaten > Schlüssel > Produkte > Technische Werte > Produktnormen > Einzelne Bezeichnung
Stammdaten > Schlüssel > Produkte > Technische Werte > Produktnormen > Alle Bezeichnung

*Abb. B-146 Einzelne Produktnormen*

Dieser Dialog enthält die unterschiedlichen Produktnormen, die für die Produktzertifizierung gelten sollen, in den jeweiligen Sprachen.

### Erläuterung der Felder

**Produktnorm**
Schlüssel-Nummer. Zum Anlegen einer neuen Norm geben Sie die nächste freie Nummer ein.
Technische Info: `<F9>`, DB-Feld: xsprbez.id

**Spr**
Sprachkennzeichen.
Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz

**Kurzbezeichnung**
Kurzbezeichnung der Produktnorm, z. B. CE1.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1
**Produktbeschreibung 1**
Bezeichnung der Produktnorm, z. B. CE-Norm 1.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez2

**Produktbeschreibung 2**
Weitere Bezeichnung der Produktnorm.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez3

## Prioritäten

Stammdaten > Schlüssel > Produkte > Technische Werte > Prioritäten

*Abb. B-147 Prioritäten*

Dieser Dialog enthält die Werte für unterschiedliche Prioritäten. Die Auswertung dieser Prioritäten erfolgt innerhalb der Produkt-CE-Kennzeichnung.

### Erläuterung der Felder

**Typ**
Auswahl des Typs:
- Brandverhalten
- Einbruchhemmung
- Pendelschlag
Technische Info: `<F9>`, DB-Feld: xtechwprio.typ

**Wert**
Technische Wert der Priorität.
Technische Info: Numerisches Feld, DB-Feld: xtechwprio.wert

**Priorität**
Priorität des technischen Wertes:
- 1: gering
- n: hoch.
Technische Info: Numerisches Feld, DB-Feld: xtechwprio.prio

## Produktkennzeichnung (CEKAL)

Stammdaten > Schlüssel > Produkte > Technische Werte > Produktkennzeichnung (CEKAL)

*Abb. B-148 Produktkennzeichnung*

In diesem Dialog ist es möglich, eine neue Produktkennzeichnung laut CEKAL-Richtlinien vorzunehmen. Die Produktkennzeichnung basiert auf den in den Stammdaten hinterlegten Restriktionen für zweifach ISO-Artikel.

### Erläuterung der Felder

**Typ**
Auswahl des Restriktions-Typs:
- CEKAL-Restriktion
- AR-Restriktion
Technische Info: Toggle-Feld, DB-Feld: artkennrestrikt.type

**SZR von/bis**
Angabe des SZR.
Technische Info: Numerisches Feld, DB-Feld: artkennrestrikt.vszr/bszr

**Breite von/bis**
Angabe der Breite. Dieses Feld ist nur aktiv, wenn es sich bei dem Typ um eine CEKAL-Restriktion handelt.
Technische Info: Numerisches Feld, DB-Feld: artkennrestrikt.vbreite/bbreite

**Höhe von/bis**
Angabe der Höhe. Dieses Feld ist nur aktiv, wenn es sich bei dem Typ um eine CEKAL-Restriktion handelt.
Technische Info: Numerisches Feld, DB-Feld: artkennrestrikt.vhoehe/bhoehe

**Dicke sum.**
Summe der Dicken beider Scheiben. Dieses Feld ist nur aktiv, wenn es sich bei dem Typ um eine AR-Restriktion handelt.
Technische Info: Numerisches Feld, DB-Feld: artkennrestrikt.sumdicke

**Dicke dif.**
Dickendifferenz von Scheiben. Dieses Feld ist nur aktiv, wenn es sich bei dem Typ um eine AR-Restriktion handelt.
Technische Info: Numerisches Feld, DB-Feld: artkennrestrikt.diffdicke
**CEKAL**
Hier steuern Sie, ob die Kennzeichnung CEKAL-relevant ist. Dieses Feld ist nur aktiv, wenn es sich bei dem Typ um eine CEKAL-Restriktion handelt.
- J: Ja
- N: Nein
Technische Info: Toggle-Feld, DB-Feld: artkennrestrikt.cekal

## CE-Kennzeichen (CPIP)

Stammdaten > Schlüssel > Produkte > Technische Werte > CE-Kennzeichen (CPIP) > Default-Werte

Bei dem Menüpunkt und den darin enthaltenen Untermenüs handelt es sich um eine kundenspezifische Umsetzung, die im Rahmen dieser Dokumentation nicht beschrieben wird.

## Leistungserklärung

Stammdaten > Schlüssel > Produkte > Technische Werte > Leistungserklärung (Dokumente)

*Abb. B-149 Leistungserklärung*

Hier können Sie unterschiedliche Leistungserklärungen (Dateien) für Produkte in verschiedenen Sprachen hinterlegen bzw. zuordnen. Eine Zuordnung kann nur von dem Mitarbeiter mit dem Recht KYLE='w' gemacht werden.

### Erläuterung der Felder

**Nummer**
Auswahl des Leistungserklärung. Zum Anlegen einer neuen Leistungserklärung geben Sie die gewünschten Daten ein.
Technische Info: Alphanumerisches Feld, DB-Feld: xlesprzu.lenr

**Beschreibung**
Beschreibung des Leistungserklärung.
Technische Info: Alphanumerisches Feld, DB-Feld: xlesprzu.lebez

**Produkt**
Produkt, dem die Leistungserklärung zugeordnet wird.
Technische Info: DB-Feld: xlesprzu.prodbez

**Produkttyp**
Produkttyp, dem die Leistungserklärung zugeordnet wird.
Technische Info: DB-Feld: xlesprzu.prodtypbez

**Verwendungszweck**
Verwendungszweck.
Technische Info: DB-Feld: xlesprzu.zweck
**Harmonisierte Produktnorm**
Technische Info: DB-Feld: xlesprzu.pnorm

**Nummer**
Anzeige des Sprachkennzeichens.
Technische Info: Numerisches Feld, DB-Feld: xlesprzu.sprkz

**Sprache**
Anzeige der Sprache.
Technische Info: Anzeigefeld

**Datei**
Wenn die Dokumente schon auf dem Server in dem Bereich `<DATEI_REF_PFAD>\dop` abgelegt sind, so kann die Zuordnung mit `<F9>` oder über Schaltfläche Datei auswählen erfolgen.
Technische Info: `<F9>`, DB-Feld: xlesprzu.datei

## Produktverschlüsselung

Stammdaten > Schlüssel > Produkte > Technische Werte > Produktverschlüsselung

*Abb. B-150 Produktverschlüsselung*

Eine Leistungserklärung spiegelt die technischen Merkmale und die Leistungsmerkmale eines Produktaufbaus wider. Um die Verwaltung und Zuordnung zu erleichtern, können Sie Regeln definieren, wie die Produkte in einer Leistungserklärung gespiegelt werden sollen. Dazu können Sie eine individuelle Verschlüsselung für Produkte sowie deren Stücklisten hinterlegen.

Der Grundgedanke dabei ist, dass nur bestimmte Merkmale und Elemente der Produktstückliste relevant für die Zuordnung zu einer Leistungserklärung sind (ein Abstandhalter in einem ISO beispielsweise nicht). Somit ist es möglich, für verschiedene Produkte mit ähnlichen Stücklisten, die gleiche Leistungserklärung automatisiert zuzuordnen. Die Codierung kann hierbei für Artikeltypen (global) oder für einzelne Artikel mit bestimmten Stücklistenelementen (spezifisch) angelegt werden. Maßgeblich für die Produktverschlüsslung ist immer der Positionsartikel bzw. dessen Artikeltyp.

### Erläuterung der Felder

**Art der Auswertung**
Auswahl der Art:
- Artikel-Typ
- Artikelnummer
Technische Info: Toggle-Feld, DB-Feld: xprodkeyart.prodmerktyp

**Nummer**
Auswahl der Artikelnummer oder des Artikeltyps.
Technische Info: `<F9>`, DB-Feld: xprodkeyart.prodmerk

**Codierung als**
Auswahl der Codierung:
- Artikelnummer
- Artikeltyp
Die Codierung bedeutet, dass ein Austausch von Rahmenartikel in der Stückliste zu gleichen Produktschlüsseln führt und keine neue LE benötigt wird. Die Codierung soll individuell nach Vorgaben des Betriebes angelegt werden. Je genauer der Schlüssel codiert ist, desto mehr LE werden benötigt.
Technische Info: `<F9>`, DB-Feld: xprodkeyart.prodtypkz

**Allgemeine Angaben**
Die Felder in diesem Bereich sind zusammenhängend zu betrachten. Wir versuchen dies anhand von drei Beispielen zu erläutern:
- **Beispiel 1:** Für alle Float-Gläser soll die gleiche Leistungserklärung (z. B. LE-FLOAT-STD) gelten. Nehmen Sie hierzu folgende Einstellungen vor: Art der Auswertung = Artikel-Typ, Nummer = 100, Codierung als = A-Typ, alle anderen Felder bleiben leer.
So bekommen alle Produkte vom Artikel-Typ = 100 (FLOAT Festmaß) den Produktschlüssel „|100<Einb. Pos>". Diesem Produktschlüssel kann nun die entsprechende Leistungserklärung zugewiesen werden.
- **Beispiel 2:** Wird für den Artikeltyp 150 (ESG) die Codierung als Artikelnummer gewählt, so erhält jeder ESG-Artikel als Produktschlüssel „|<Artikelnummer>-<Einbauposition>“ (z. B. „|350005-1“ oder „|350006-1“).
Ist für eine spezifische ESG-Bearbeitung eine abweichenden Leistungserklärung wichtig, so können Sie diese Bearbeitung unter Detaillierte Angaben entweder als Artikeltyp, A+W Bearbeitungstyp oder als Artikelnummer definieren und die entsprechende Art der Verschlüsselung für diese Bearbeitung hinterlegen. So kann z. B. eine Beschichtung mit Artikelnummer 198160 als Artikelnummer in den Produktschlüssel einfließen. In diesem Fall wird bei ESG mit dieser Beschichtung der Produktschlüssel „|350005-1|198160-0|" generiert.
- **Beispiel 3:** Wählen Sie unter Allgemeine Angaben > Alle Gläser, so werden alle Elemente der Stückliste mit Artikeltyp 100 bis 170 in die Verschlüsselung mit aufgenommen. Bei ISO-Artikeln kann man auch den SZR und weitere Elemente der Stückliste, die maßgebend für die Berechnung der technischen Werte sind, in die Verschlüsselung mit aufnehmen. Unter Detaillierte Angaben können Sie aber auch spezifische Gläser hinterlegen, wenn nicht alle Glastypen pauschal für die Zuordnung der Leistungserklärung wichtig sind.
Technische Info: Toggle-Feld, DB-Feld: xprodkeyart.allgl/typkzallg/allszr

### Erläuterung der Felder im Bereich Detaillierte Angaben

*Abb. B-151 Produktverschlüsselung, detaillierte Angaben*

Unter **Detaillierte Angaben** können Sie aber auch spezifische Gläser hinterlegen, wenn nicht alle Glastypen pauschal für die Zuordnung der Leistungserklärung wichtig sind.

**Art der Auswertung**
Auswahl der Art:
- Artikel-Typ
- Artikelnummer
- A+W Bearbeitungstyp
Technische Info: Toggle-Feld, DB-Feld: xprodkeyart.merktyp1

**Nummer**
Auswahl der Artikelnummer oder des Artikeltyps. Die Bezeichnung wird im Feld dahinter angezeigt.
Technische Info: `<F9>`, DB-Feld: xprodkeyart.merk1

**Code**
Auswahl der Codierung:
- A-Typ
- ArtNr
Technische Info: `<F9>`, DB-Feld: xprodkeyart.typkz1

## Bezeichnungen für Produktverwendungszwecke

Stammdaten > Schlüssel > Produkte > Technische Werte > Produktverwendungszwecke > Einzelne Bezeichnung
Stammdaten > Schlüssel > Produkte > Technische Werte > Produktverwendungszwecke > Alle Bezeichnung

*Abb. B-152 Bezeichnungen für Produktverwendungszwecke*

Dieser Dialog enthält die Verwendungszwecke in allen Sprachen, die später auf die Leistungserklärung gedruckt werden.

### Erläuterung der Felder

**Produktverwendungszwecke/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Dicken-Gruppe geben Sie die nächste freie Nummer ein.
Technische Info: `<F9>`, DB-Feld: xsprbez.id

**Spr**
Sprachkennzeichen.
Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz
**Kurzbezeichnung**
Kurzbezeichnung des Verwendungszwecks, z. B. ISO.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

**Text**
Bezeichnung des Verwendungszwecks, z. B. Mehrscheibenisolierglas.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez2

## Parameterbeschreibung

Stammdaten > Schlüssel > Produkte > Technische Werte > Parameterbeschreibung

*Abb. B-153 Parameterbeschreibung*

Hier werden die möglichen Parameterbeschreibungen, die für die Leistungserklärung verwendet werden, gepflegt.

### Erläuterung der Felder

**Nr**
Auswahl der möglichen Leistungen in der festgelegten Reihenfolge. Zum Anlegen einer neuen Leistung geben Sie die nächste freie Nummer ein.
Technische Info: `<F9>`, DB-Feld: xtechwnorm.id

**Spr**
Auswahl des Sprachkennzeichens.
Technische Info: `<F9>`, DB-Feld: xtechwnorm.sprkz

**Beschreibung**
Die Beschreibung wird aus der vorgegebenen Beschreibung geholt, kann aber individuell geändert werden, so wie diese dann in dem Dokument ausgegeben wird.
Technische Info: Alphanumerisches Feld, DB-Feld: xtechwnorm.bez1

**Einheit**
Eingabe der Maßeinheit, falls diese gedruckt werden soll.
Technische Info: Alphanumerisches Feld, DB-Feld: xtechwnorm.einheit

**Norm**
die eingetragene Norm wird in das Dokument für die entsprechende Leistung übernommen. Es wird jedoch nicht geprüft, ob die Norm für die einzelne Leistung in allen Sprachen identisch ist.
Technische Info: Alphanumerisches Feld, DB-Feld: xtechwnorm.norm

## Leistungserklärung (Erfassung)

Stammdaten > Schlüssel > Produkte > Technische Werte > Leistungserklärung (Erfassung)

*Abb. B-154 Leistungserklärung*

Im diesem Dialog können Sie die Leistungserklärung erfassen, um diese in anderen Mandanten zur Verfügung zu stellen. Der Dialog ist nur betretbar, wenn die Leistungserklärungen zentral erfasst werden. Dabei handelt es sich um eine kundenspezifische Funktion. Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Enterprise.

> **Dialogfelder**
> Die Felder in diesem Dialog sind identisch mit den Feldern der Auftragserfassung und werden hier nicht erläutert.

## Bezeichnungen für Analysegruppen

Stammdaten > Schlüssel > Produkte > Analysegruppen > Einzelne Bezeichnungen
Stammdaten > Schlüssel > Produkte > Analysegruppen > Alle Bezeichnungen

*Abb. B-155 Bezeichnungen für Analysegruppen*

Für eigene Auswertungen können Sie Analysegruppen anlegen, die anschließend im Artikelstamm Artikeln zugeordnet werden.

### Erläuterung der Felder

**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Analysegruppe geben Sie die nächste freie Nummer ein.
Technische Info: `<F9>`, DB-Feld: xsprbez.id

**Spr**
Sprachkennzeichen.
Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz

**Bezeichnung**
Bezeichnung der Gruppe, z. B. Pyrostop intern.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

## Bezeichnungen für Beschlagstypen

Stammdaten > Schlüssel > Produkte > Beschlagstypen > Beschlagstypen
Stammdaten > Schlüssel > Produkte > Beschlagstypen > Einzelne Bezeichnungen
Stammdaten > Schlüssel > Produkte > Beschlagstypen > Alle Bezeichnungen

*Abb. B-156*

Dieser Dialog enthält die unterschiedlichen Beschlagstypen, die bei der Erfassung vorkommen können.

### Erläuterung der Felder

**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen eines neuen Beschlagstypen geben Sie die nächste freie Nummer eingeben Sie die nächste freie Nummer ein.
Technische Info: `<F9>`, DB-Feld: xsprbez.id
View: xalbtyp.btyp

**Spr**
Sprachkennzeichen.
Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz

**Kurzbez.**
Kurzbezeichnung des Beschlagstyps.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

**Bezeichnung**
Bezeichnung des Beschlagstyps.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez2
xalbtyp.bez1

## Bezeichnungen für Folientypen

Stammdaten > Schlüssel > Produkte > Folientypen > Einzelne Bezeichnungen
Stammdaten > Schlüssel > Produkte > Folientypen > Alle Bezeichnungen

*Abb. B-157 Bezeichnungen für Folientypen*

Dieser Dialog enthält die unterschiedlichen Folientypen in den jeweiligen Sprachen. Sie werden dann im Artikelstamm den Folien zugeordnet.

### Erläuterung der Felder

**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Folie geben Sie die nächste freie Nummer ein.
Technische Info: `<F9>`, DB-Feld: xsprbez.id

**Spr**
Sprachkennzeichen.
Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz

**Bezeichnung**
Bezeichnung der Folie, z. B. VSG-Folie.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

## Produktionstypen

Stammdaten > Schlüssel > Produkte > Produktionstypen

*Abb. B-158 Produktionstypen*

Dieser Dialog enthält die unterschiedlichen Produktionstypen, in den jeweiligen Sprachen.

### Erläuterung der Felder

**Produktionstyp**
Schlüssel-Nummer. Zum Anlegen eines neuen Typs geben Sie die nächste freie Nummer ein.
Technische Info: Numerisches Feld, DB-Feld: pmstyp.ptyp

**Bezeichnung**
Bezeichnung des Produktions-Typs.
Technische Info: Alphanumerisches Feld, DB-Feld: pmstyp.ptypbez

**Kategorie**
Kategorie des PMS-Typs:
- Artikel
- Bearbeitung
Technische Info: Toggle-Feld, DB-Feld: pmstyp.ptypbez

## Bezeichnungen für Rahmentypen

Stammdaten > Schlüssel > Produkte > Rahmentypen > Rahmentypen
Stammdaten > Schlüssel > Produkte > Rahmentypen > Einzelne Bezeichnungen
Stammdaten > Schlüssel > Produkte > Rahmentypen > Alle Bezeichnungen

*Abb. B-159 Bezeichnungen für Rahmentypen*

Dieser Dialog enthält die unterschiedlichen Rahmentypen in den jeweiligen Sprachen, die dann im Artikelstamm den Rahmen zugeordnet werden.

### Erläuterung der Felder

**Rahmentyp**
Schlüssel-Nummer. Zum Anlegen eines neuen Rahmentyps geben Sie die nächste freie Nummer ein.
Technische Info: Numerisches Feld, DB-Feld: xxrahmentyp.rahmenid

**Bezeichnung**
Bezeichnung des Rahmens, z. B. TPS.
Technische Info: Alphanumerisches Feld, DB-Feld: xxrahmentyp.rahmenbez
**AWEnterprise Rahmentyp**
Auswahl des A+W Enterprise Rahmentyps:
- Stahl
- Aluminium
- TPS
- Kunststoff
Technische Info: Toggle-Feld, DB-Feld: xxrahmentyp.alcibrahmentyp

**Nummer**
Schlüssel-Nummer. Zum Anlegen eines neuen Typs geben Sie die nächste freie Nummer ein.
Technische Info: `<F9>`, DB-Feld: xsprbez.id

**Spr**
Sprachkennzeichen.
Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz

**Bezeichnung**
Bezeichnung des Rahmentyps, z. B. Stahl.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

## Bezeichnungen für Versiegelungstypen

Stammdaten > Schlüssel > Produkte > Versiegelungstypen > Einzelne Bezeichnungen
Stammdaten > Schlüssel > Produkte > Versiegelungstypen > Alle Bezeichnungen

*Abb. B-160 Bezeichnungen für Versiegelungstypen*

Alle Versiegelungstypen, die im Artikelstamm und später in der Auftragserfassung benötigt werden, müssen in dieser Schlüsseltabelle angelegt werden. Der Dialog enthält die einzelnen Versiegelungstypen in den jeweiligen Sprachen.

### Erläuterung der Felder

**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen eines neuen Typs geben Sie die nächste freie Nummer ein.
Technische Info: `<F9>`, DB-Feld: xsprbez.id

**Spr**
Sprachkennzeichen.
Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz

**Bezeichnung**
Bezeichnung des Versiegelungstyps, z. B. Butyl.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

## Motivzuordnung

Stammdaten > Schlüssel > Produkte > Motive

*Abb. B-161 Motivzuordnung*

Hier werden alle Motiv-Dateien, die für die Oberflächenbearbeitung verwendet werden, hinterlegt. Das Motiv muss in Form einer Bilddatei vorliegen (jpg, png, bmp, gif, tif(f) werden unterstützt). Sie können das Motiv durch die Vermaßungstypen des Bearbeitungstyps Oberfläche vermaßen und somit auf der Scheibe platzieren. Beim Öffnen werden die Abmessungen der Bilddatei 1:1 übernommen werden. Die Breite oder Höhe des Motivs können unter Berücksichtigung des Seitenverhältnisses angepasst werden. Das Motiv kann dann auf den Skizzen und dem Ausdruck ausgegeben werden.

### Erläuterung der Felder

**Nummer**
Nummer des zu beschreibenden Motivs. Zum Anlegen eines neuen Motivs geben Sie die nächste freie Nummer ein.
Technische Info: `<F9>`, DB-Feld: xsiebnr.siebnr

**Bezeichnung**
Bezeichnung des Motivs.
Technische Info: Alphanumerisches Feld, DB-Feld: xsiebnr.siebname

**MaxBreite**
Breite des Motivs in mm.
Technische Info: Numerisches Feld, DB-Feld: xsiebnr.maxbreite

**MaxHöhe**
Höhe des Motivs in mm.
Technische Info: Numerisches Feld, DB-Feld: xsiebnr.maxhoehe

**Datei**
Auswahl der Motivdatei.
Technische Info: `<F9>`, DB-Feld: xsiebnr.dateiname
**Datei neu**
Wenn Sie diese Schaltfläche drücken, öffnet sich der Dokumenten-Zuordnungsdialog, in den Sie mit gedrückter Maustaste eine ausgewählte Datei hinüber-ziehen können.

**Datei auswählen**
Wenn die Dokumente schon auf dem Server in dem Bereich `<DATEI_REF_PFAD>\motif` abgelegt sind, so kann die Zuordnung mit `<F9>` oder über Schaltfläche Datei auswählen erfolgen.

## Stapel

Stammdaten > Schlüssel > Produkte > Stapel >...

Bei dem Menü Stapel und die darin enthaltenen Unterpunkte handelt es sich um eine kundenspezifische Umsetzung, die im Rahmen dieser Dokumentation nicht beschrieben wird.

## Bezeichnungen für Kistensignatur

Stammdaten > Schlüssel > Produkte > Kistensignatur > Einzelne Bezeichnungen
Stammdaten > Schlüssel > Produkte > Kistensignatur > Alle Bezeichnungen

*Abb. B-162 Bezeichnungen für Kistensignatur*

In diesem Dialog weißen Sie einer Transportkiste eine Signatur zu. Die Signatur wird über eine Formel hinterlegt.
"Textformeln" auf Seite B-521

### Erläuterung der Felder

**KFZ Land**
Auswahl des Landeskennzeichens. Tippen Sie das Kennzeichen ein oder drücken Sie `<F9>` zum Öffnen des Auswahldialogs. Die entsprechenden Schlüssel werden über das Menü Länder (Schlüssel > Marktpartner) vergeben.
Technische Info: `<F9>`, DB-Feld: xkiformel.kfzcode
**Anordn.**
Druckposition der Signatur:
- oben
- vorne
- unten
- hinten
- links
- rechts.
Technische Info: Toggle-Feld, DB-Feld: xkiformel.txtpos

**Formel**
Auswahl der Formel. Tippen Sie die Nummer ein oder drücken Sie `<F9>` zum Öffnen des Auswahldialogs. Die entsprechenden Schlüssel werden über das Menü Textformeln (Textverwaltung > Textgenerierung) vergeben.
Technische Info: Numerisches Feld, DB-Feld: xkiformel.frnr

**Bezeichnung**
Formelbezeichnung erscheint automatisch, wenn Sie das Feld Formel verlassen.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez2

## Shaping/Nesting-Artikel

Stammdaten > Schlüssel > Produkte > Shaping/Nesting-Artikel

*Abb. B-163 Shaping/Nesting-Artikel*

In diesem Dialog ordnen Sie einer Artikel-Nummer die Shaping/Nesting-Artikel-Nummer zu.

> **Technische Auftragserfassung (ITOE)**
> Die Daten dieses Dialogs werden unter Verwendung der neuen Technischen Auftragserfassung (iTOE) nicht weiter verwendet.
> Die neue ITOE wertet die Daten aus den Stammdaten > Schlüssel > Produkte > ITOE Austauschregeln aus.

## Template Parameter

Stammdaten > Schlüssel > Produkte > Template Parameter

*Abb. B-164 Template Parameter*

In diesem Dialog legen Sie die Parameter für das jeweilige Template an und versehen diese mit einer Parameter-Nummer.
Die Template-Dateien müssen als Stammdaten im Verzeichnis `$DATEI_REF_PFAD/template` abgelegt werden. Das Programm A+W CAD Designer (Shapes) muss Zugriff auf das Verzeichnis haben.

### Erläuterung der Felder

**Templatename**
Name des Templates. Zum Anlegen eines neuen Templates gehen Sie in die nächste freie Zeile.
Technische Info: Alphanumerisches Feld, DB-Feld: xtempparam.tempname

**SN Parameter Name**
Templateparametername.
Technische Info: Alphanumerisches Feld, DB-Feld: xtempparam.snparamname

**Parameter**
Parameternummer (Reihenfolge).
Technische Info: Numerisches Feld, DB-Feld: xtempparam.paramnr

**Inch**
Mit diesem Feld steuern Sie, ob der Wert bei externer DFÜ von der Datei zur Datenbank konvertiert werden muss.
- Der Wert muss konvertiert werden.
- Der Wert muss nicht konvertiert werden.
Technische Info: `<Toggle>-Feld`, DB-Feld: xtempparam.convert

## iTOE-Austauschregeln

Stammdaten > Schlüssel > Produkte > iTOE - Austauschregeln
Stammdaten > Schlüssel > Produkte > iTOE - Austauschregeln > <F2>

*Abb. B-165 iTOE - Austauschregeln*

In diesem Dialog können Sie für alle A+W Bearbeitungstypen mindestens eine Austauschregel hinterlegen.
In der Grafik oben wird z. B. für A+W CAD Designer (Shapes) - Bearbeitung vom Typ 1305 (Eckabschnitt) immer auf der A+W Enterprise - Seite den Artikel 198130 (Kanten geschliffen) in die Stückliste hinzugefügt.

### Erläuterung der Felder im Register Austausch-/Zusatzregeln

**Produkttyp**
Eingabe des Produkttyps.
Technische Info: Numerisches Feld, DB-Feld: kuaz.prodtyp

**Produkt**
Eingabe des Produktes.
Technische Info: Numerisches Feld, DB-Feld: kuaz.prodnr

**Stücklisten Atyp**
Eingabe des Stücklisten-Artikeltyps.
Technische Info: Numerisches Feld, DB-Feld: kuaz.

**Stücklisten Artikel**
Eingabe des Stücklisten-Artikels.
Technische Info: Numerisches Feld, DB-Feld: kuaz.

**A+W Typ**
Auswahl des A+W Bearbeitungstyps.
Technische Info: `<F9>`, DB-Feld: kuaz.atyp

**Artikel**
Auswahl der Artikelnummer für den Austausch oder Zusatz. Die Bezeichnung wird im Feld dahinter angezeigt.
Technische Info: `<F9>`, DB-Feld: kuaz.azartnr

### Erläuterung der Felder im Register Details

Sind die Bearbeitungsartikel auch Parameter-relevant (z. B. Bohrung), so können Sie hier die Regel noch genauer spezifizieren.

**Farbe**
Eingabe des Farbnummer.
Technische Info: Numerisches Feld, DB-Feld: kuaz.farbnr

**Vermaßungstyp**
Der Vermaßungstyp ist abhängig von dem A+W Bearbeitungstyp. Weitere Informationen erhalten Sie im A+W Normierten Bearbeitungskatalog.
Folgende Auswahlmöglichkeiten stehen zur Verfügung:
- Absolute Koordinaten
- Abstände zu zwei Kanten
- Abstände zu Ecke und Kante
Technische Info: Toggle-Feld, DB-Feld: kuaz.mtyp

> **Unterschiedliche Maßparameter**
> In Abhängigkeit vom ausgewählten Bearbeitungstyp werden unterschiedliche Maßparameter eingeblendet.

## Bemaßungsset

Stammdaten > Schlüssel > Produkte > Bemaßungsset > Bemaßungsset
Stammdaten > Schlüssel > Produkte > Bemaßungsset > Klassifizierungscode
Stammdaten > Schlüssel > Produkte > Bemaßungsset > Herstellercode

Bei dem Menü Bemaßungsset und die darin enthaltenen Unterpunkte handelt es sich um eine kundenspezifische Umsetzung, die im Rahmen dieser Dokumentation nicht beschrieben wird.

## Kundenprodukte

Stammdaten > Schlüssel > Produkte > Kundenprodukte

*Abb. B-166 Kundenprodukte*

In diesem Dialog haben Sie die Möglichkeit, kundenspezifische Artikelaufbauten zu hinterlegen.

### Erläuterung der Felder

**Kundenprodukt**
Auswahl der kundenspezifischen Artikelnummer. Zum Anlegen einer neuen kundenspezifischen Artikelnummer geben Sie diese hier ein und füllen die restlichen Felder des Dialogs.
Technische Info: Alphanumerisches Feld, DB-Feld: kuartasscheck.kuartnr

**ALCIB-Artikelnummer**
Auswahl der A+W Enterprise-Artikelnummer.
Technische Info: Alphanumerisches Feld, DB-Feld: kuartasscheck.artnr

**Artikeltyp**
Das Feld wird automatisch gefüllt, wenn Sie das Feld ALCIB-Artikelnummer verlassen.

**Glas1**
Erste Scheibe.
Technische Info: `<F9>`, DB-Feld: kuartasscheck.glas1

**Glas2**
Zweite Scheibe.
Technische Info: `<F9>`, DB-Feld: kuartasscheck.glas2

**Glas3**
Dritte Scheibe.
Technische Info: `<F9>`, DB-Feld: kuartasscheck.glas2

**SZR1**
Erster Scheibenzwischenraum.
Technische Info: `<F9>`, DB-Feld: kuartasscheck.cavity1

**SZR2**
Zweiter Scheibenzwischenraum.
Technische Info: `<F9>`, DB-Feld: kuartasscheck.cavity2
**SZR3**
Dritter Scheibenzwischenraum.
Technische Info: `<F9>`, DB-Feld: kuartasscheck.cavity3

**Dichtst.**
Dichtstoff.
Technische Info: `<F9>`, DB-Feld: kuartasscheck.sealant

**Adapter**
Adapter.
Technische Info: `<F9>`, DB-Feld: kuartasscheck.adapter

**Suffix**
Suffix.
Technische Info: `<F9>`, DB-Feld: kuartasscheck.suffix

**I/O-Flag**
I/O-Flag.
Technische Info: `<F9>`, DB-Feld: kuartasscheck.ioflag

**Online**
Mit diesem Feld steuern Sie, ob das Kundenprodukt für die Online-Erfassung geeignet ist oder nicht.
- Das Kundenprodukt ist für die Online-Erfassung geeignet.
- Das Kundenprodukt ist nicht für die Online-Erfassung geeignet.
Technische Info: `<Toggle>-Feld`, DB-Feld: kuartasscheck.onlineflag

## Bestellte Bearbeitungen

Stammdaten > Schlüssel > Produkte > Bestellte Bearbeitungen

*Abb. B-167 Bestellte Bearbeitungen*

In diesem Dialog können Sie bei der entsprechenden Konfiguration die Zuordnung von Lieferant, zu bearbeitendem Glas und durchzuführender Bearbeitung zu einem bestellenden Produkt festlegen. Diese Angaben benötigen Sie, wenn Sie mit so genanntem "verlängerten Werkbank" arbeiten. Die Nutzung dieser Funktion ist mit dem Mitarbeiter der A+W Software GmbH zu klären.

### Erläuterung der Felder

**Marktpartner**
Marktpartnertyp. Sie können wählen zwischen:
- Kunde
- Lieferant
Im Feld dahinter wählen Sie die Nummer des Marktpartners aus oder geben Sie direkt ein.
Technische Info: `<Toggle>-Feld`, DB-Feld: bestbeaart.kuliflag/mpnr

**Glas**
Artikelnummer des zu bearbeitenden Glases aus der Stückliste. Alternativ kann auch der Artikeltyp verwendet werden.
Technische Info: `<F9>`, DB-Feld: bestbeaart.artnr

**Glastyp**
Artikeltyp des zu bearbeitenden Glases aus der Stückliste. Alternativ kann auch die Artikelnummer verwendet werden.
Technische Info: `<F9>`, DB-Feld: bestbeaart.atyp

**Bearbeitung**
Artikelnummer der zu bestellenden Bearbeitung.
Technische Info: `<F9>`, DB-Feld: bestbeaart.bearbnr

**Typ**
Artikeltyp der zu bestellenden Bearbeitung.
Technische Info: `<F9>`, DB-Feld: bestbeaart.bearbatyp

**A+W Bea-typ**
Bearbeitungstyp der zu bestellenden Bearbeitung.
Technische Info: `<F9>`, DB-Feld: bestbeaart.bearbawtyp

**Produkt**
Artikelnummer des als Positionsartikel zu verwendenden Artikels bei der Kombination Bearbeitung < zu bearbeitendes Glas.
Technische Info: `<F9>`, DB-Feld: bestbeaart.headartnr

> **Register Details**
> Das Register Details liefert Ihnen zusätzlich die Bezeichnung der einzelnen Felder, die Sie hier gefüllt haben.

## Hausspezifische Angaben

Stammdaten > Schlüssel > Produkte > Hausspezifische Angaben > Artikel
Stammdaten > Schlüssel > Produkte > Hausspezifische Angaben > Lieferanten
Stammdaten > Schlüssel > Produkte > Hausspezifische Angaben > Varianten
Stammdaten > Schlüssel > Produkte > Hausspezifische Angaben > Farben/Größen

In diesen Dialogen können Sie hausspezifische Angaben zu ausgewählten Artikeln, Lieferantenzuordnungen, Artikelmaß-, Farb- oder Größenvarianten ansehen bzw. pflegen. Diese Daten finden Sie auch im Artikelstamm.

Die oben genannten Dialoge werden an folgender Stelle ausführlich erläutert:
⇨ "Hausspezifische Artikel-Angaben" auf Seite B-475

Stammdaten > Schlüssel > Produkte > Hausspezifische Angaben > Warengruppen
In diesem Dialog können Sie hausspezifische Warengruppen-Angaben ansehen bzw. pflegen.
Der Dialog Warengruppen wird an folgender Stelle ausführlich erläutert:
⇨ "Hausspezifische Warengruppen" auf Seite B-495

## VSG/GH Vererbung

Stammdaten > Schlüssel > Produkte > VSG/GH Vererbung

*Abb. B-168 Austauschvorschriften für vererbbare Bearbeitungen*

In diesem Dialog können Sie die Regeln für die vererbte Bearbeitungen in VSG/GH-Gläser hinterlegen. Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

### Erläuterung der Felder im Register Austauschregeln

**Glastyp**
Eingabe des Produkttyps.
Technische Info: Numerisches Feld, DB-Feld: kuaz.prodtyp

**Glasnummer**
Eingabe der Scheibennummer aus der Stückliste (Einbauposition), für die die Regeln angewendet werden soll. Bleibt das Feld leer, gilt die Regeln für alle Glasscheiben in der Stückliste.
Technische Info: Numerisches Feld, DB-Feld: kuaz.prodepos

**Bearbeitung**
Eingabe der Bearbeitungsnummer.
Technische Info: Numerisches Feld, DB-Feld: kuaz.artnr

**Artikel**
Auswahl der Artikelnummer für den Austausch oder Zusatz. Die Bezeichnung wird im Feld dahinter angezeigt.
Technische Info: `<F9>`, DB-Feld: kuaz.azartnr

**Prod**
Checkbox zur Geometrie-Bestimmung, ob die erfasste Regeln berücksichtigt wird.
- Die Scheibengeometrie wird berücksichtigt.
- Die Scheibengeometrie wird nicht berücksichtigt.
Technische Info: `<F9>`, DB-Feld: kuaz.geometrie

## Artikelgruppen-Bezeichnungen

Stammdaten > Schlüssel > Produkte > A+W iQuote-spezifische Angaben > Artikelgruppen > Einzelne Bezeichnungen
Stammdaten > Schlüssel > Produkte > A+W iQuote-spezifische Angaben > Artikelgruppen > Alle Bezeichnungen

*Abb. B-169 Bezeichnungen für Versiegelungstypen*

Alle Artikelgruppen, die Artikeln zur Erfassung in online Shop A+W iQuote zusammenfassen, müssen in dieser Schlüsseltabelle angelegt werden. Der linke Dialog enthält die einzelnen Artikelgruppen in den jeweiligen Sprachen, der rechte Dialog enthält alle Artikelgruppen in Systemsprachen.

### Erläuterung der Felder

**Artikelgruppen für A+W iQuote/Nr**
Schlüssel-Nummer. Zum Anlegen eines neuen Typs ist die Verwendung der Artikeltyp-Nummern zu empfehlen.
Technische Info: `<F9>`, DB-Feld: xsprbez.id

**Spr**
Sprachkennzeichen.
Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz

**Kurzbezeichnung**
Kurzbezeichnung der Artikelgruppe, z. B. FLOAT. Diese Bezeichnung entspricht dem Ordnername, wo die Bilder für die entsprechende Artikel sich befinden. Die genaue Beschreibung über A+W iQuote erfragen Sie bitte bei einem Mitarbeiter der A+W Software GmbH.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

**Text**
Ausführliche Beschreibung zur Artikelgruppe.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez2

## Bearbeitungszuordnung

Stammdaten > Schlüssel > Produkte > A+W iQuote-spezifische Angaben > Bearbeitungszuordnung

*Abb. B-170 Bearbeitungszuordnung*

In diesem Dialog können Sie für die Bearbeitungen, die in online-Shop A+W iQuote erfasst werden, den A+W Enterprise Artikeln zuordnen. Die genaue Beschreibung über A+W iQuote erfragen Sie bitte bei einem Mitarbeiter der A+W Software GmbH.

### Erläuterung der Felder

**Produkttyp**
Eingabe des Produkttyps.
Technische Info: Numerisches Feld, DB-Feld: kuaz.prodtyp

**Bezeichnung**
Nach der Eingabe des Produkttypes wird hier die entsprechende Bezeichnung im Klartext dargestellt.
Technische Info: Numerisches Feld, DB-Feld: artnr.artbez1

**Bearbeitung**
Eingabe des Bearbeitungs-Artikels im A+W iQuote, für welche die Regel gelten soll.
Technische Info: Numerisches Feld, DB-Feld: kuaz.artnr

**Bezeichnung**
Nach der Eingabe der Bearbeitung wird in diesem Feld deren Bezeichnung im Klartext dargestellt.
Technische Info: `<F9>`, DB-Feld: artnr.artbez1
**Bearbeitung**
Eingabe der A+W Enterprise-Bearbeitung, die anstatt der A+W iQuote-Bearbeitung in die Auftragserfassung übernommen wird. Um die genaue Zuordnung zu gewährleisten, wird hier empfohlen, den Register Details mit entsprechenden Maßparameter zu hinterlegen. Die Bezeichnung wird im Feld dahinter angezeigt.
Technische Info: `<F9>`, DB-Feld: kuaz.azartnr

### Bearbeitungszuordnung - Details

Stammdaten > Schlüssel > Produkte > A+W iQuote-spezifische Angaben > Bearbeitungszuordnung > <F2>

*Abb. B-171 Bearbeitungszuordnung*

In diesem Dialog können Sie für die hinterlegte Bearbeitungszuordnung zusätzlich die Restriktionsparameter bestimmen.

**Glastyp**
Das Feld Glastyp entspricht dem Feld Produkttyp in dem Hauptdialog. Nach der Werteeingabe wird die Bezeichnung im Klartext angezeigt.
Technische Info: Numerisches Feld, DB-Feld: kuaz.prodtyp

**Bearbeitung**
In diesem Feld wird die Bearbeitung, für die die A+W iQuote-Zuordnung bestehen soll, angezeigt bzw. kann hier neue erfasst werden. Nach der Auswahl wird dahinten die Bearbeitungsbezeichnung im Klartext dargestellt.
Technische Info: Toggle-Feld, DB-Feld: kuaz.artnr

**Artikel**
Eingabe der Artikelnummer (A+W Enterprise-Bearbeitungsnummer), die anstelle der A+W iQuote-Bearbeitung in den Auftrag übernommen wird. Nach der Auswahl wird dahinten die Bearbeitungsbezeichnung im Klartext dargestellt.
Technische Info: Numerisches Feld, DB-Feld: kuaz.azartnr
> ### Restriktionen /ab Maß
> **Bearbeitungsmaß 1/2** In den beiden Parameterfelder können Restriktionen gemäß dem A+W Bearbeitungstyp hinterlegt werden.
> Technische Info: Numerisches Feld, DB-Feld: kuaz.dmess*
>
> **Unterschiedliche Maßparameter**
> In Abhängigkeit von der ausgewählten Bearbeitung werden unterschiedliche Maßparameter eingeblendet.

## Bearbeitungen für Modellkanten

Stammdaten > Schlüssel > Produkte > A+W iQuote-spezifische Angaben > Bearbeitungen für Modellkanten

*Abb. B-172 Bearbeitungen an Modellkanten*

In diesem Dialog legen Sie die iQuote-spezifische Regeln für die Erfassung der Modellscheiben. Die genaue Beschreibung über A+W iQuote erfragen Sie bitte bei einem Mitarbeiter der A+W Software GmbH.

### Erläuterung der Felder

**Bearbeitung**
Eingabe des Bearbeitungs-Artikels im A+W iQuote, für welche die Regel gelten soll.
Technische Info: Numerisches Feld, DB-Feld: kuaz.artnr

**Bezeichnung**
Nach der Eingabe der Bearbeitung wird in diesem Feld deren Bezeichnung im Klartext dargestellt.
Technische Info: `<F9>`, DB-Feld: artnr.artbez1

**Modell**
Auswahl der Modellnummer, für die die aktuelle Bearbeitung erfasst werden darf. Sie können somit eine abweichende Kantenbearbeitung für ggf. jedes Modell hinterlegen. Die Sonderkanten für ausgewählte Modelle werden unter folgendem Menüpunkt bestimmt werden:
⇨ "Kantenzuordnung" auf Seite B-249
Technische Info: `<F9>`, DB-Feld: kuaz.farbnr

> **Datenbank-Tabelle kuaz**
> Alle Austausch-/Zusatzregeln werden in der Datenbank-Tabelle `kuaz` gespeichert. Über das Feld `kuaz.kunr` wird u. A. auch die Verwendung der Austausch-/Zusatzregeln bestimmt. So bedeutet der Wert `kuaz.kunr=-3` die Auswertung für Modellkanten in A+W iQuote. In diesem Fall können andere Datenbank-Felder ebenfalls anderweitig interpretiert werden, z. B.: `kuaz.farbnr=Modelnummer`.

**SondK**
Über dieses Checkbox bestimmen Sie, ob die aktuelle Bearbeitung für Sonderkanten in A+W iQuote verwendet werden soll.
Technische Info: `<F9>`, DB-Feld: kuaz.geometrie (gilt für kuaz.kunr=-3)

**Artikel**
Eingabe der A+W Enterprise-Bearbeitung, die anstatt der A+W iQuote-Bearbeitung in die Auftragserfassung übernommen wird.
Technische Info: `<F9>`, DB-Feld: kuaz.azartnr

**Bezeichnung**
Nach der Eingabe der Artikelnummer wird in diesem Feld die Artikelbezeichnung im Klartext dargestellt.
Technische Info: `<F9>`, DB-Feld: artnr.artbez1

## Austauschgruppen-Bezeichnungen

Stammdaten > Schlüssel > Produkte > A+W iQuote-spezifische Angaben > Austauschgruppen > Einzelne Bezeichnungen
Stammdaten > Schlüssel > Produkte > A+W iQuote-spezifische Angaben > Austauschgruppen > Alle Bezeichnungen

*Abb. B-173 Bezeichnungen für Versiegelungstypen*

Alle Bezeichnungen für iQuote spezifische Austauschgruppen müssen in dieser Schlüsseltabelle angelegt werden. Der Dialog enthält die einzelnen Austauschgruppen in den jeweiligen Sprachen. Die genaue Beschreibung über A+W iQuote erfragen Sie bitte bei einem Mitarbeiter der A+W Software GmbH.

### Erläuterung der Felder

**Austauschgruppen/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Gruppe geben Sie die nächste freie Nummer ein.
Technische Info: `<F9>`, DB-Feld: xsprbez.id

**Spr**
Sprachkennzeichen.
Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz

**Kurzbezeichnung**
Bezeichnung der Austauschgruppe in Kurzform.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

**Text**
Bezeichnung der Austauschgruppe in Langform.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez2

## Gruppenzuordnung (Artikel)

Stammdaten > Schlüssel > Produkte > A+W iQuote-spezifische Angaben > Austauschgruppen > Gruppenzuordnung (Artikel)

*Abb. B-174 Gruppenzuordnung (Artikel)*

Alle Glas-Artikel, die in die iQuote Gruppen eingeteilt werden, müssen in dieser Schlüsseltabelle angelegt werden. Die genaue Beschreibung über A+W iQuote erfragen Sie bitte bei einem Mitarbeiter der A+W Software GmbH.

### Erläuterung der Felder

**Gruppe**
Schlüssel-Nummer. Sie können die Gruppe manuell eingeben oder mit `<F9>` auswählen. Bevor Sie die Artikel der richtigen Gruppen zuordnen können, müssen die Austauschgruppen hinterlegt werden.
⇨ "Austauschgruppen-Bezeichnungen" auf Seite B-374
Technische Info: `<F9>`, DB-Feld: xchangegrp.grp

**Artikel**
Angabe der Artikelnummer.
Technische Info: Alphanumerisches Feld, DB-Feld: xchangegrp.artnr

**Bezeichnung**
Bezeichnung wird für den ausgewählten Artikel in Klartext dargestellt.
Technische Info: Alphanumerisches Feld, DB-Feld: artikel.artbez1

## Gruppenzuordnung (Rahmen)

Stammdaten > Schlüssel > Produkte > A+W iQuote-spezifische Angaben > Austauschgruppen > Gruppenzuordnung (Rahmen)

*Abb. B-175 Kundenprodukte*

Alle Rahmen-Artikel für Isoliergläser, die in die iQuote Gruppen eingeteilt werden, müssen in dieser Schlüsseltabelle angelegt werden. Die genaue Beschreibung über A+W iQuote erfragen Sie bitte bei einem Mitarbeiter der A+W Software GmbH.

### Erläuterung der Felder

**Gruppe**
Schlüssel-Nummer. Sie können die Gruppe manuell eingeben oder mit `<F9>` auswählen. Bevor Sie die Artikel der richtigen Gruppen zuordnen können, müssen die Austauschgruppen hinterlegt werden.
⇨ "Austauschgruppen-Bezeichnungen" auf Seite B-374
Technische Info: `<F9>`, DB-Feld: xchangegrp.grp

**Artikel**
Angabe der Artikelnummer.
Technische Info: Alphanumerisches Feld, DB-Feld: xchangegrp.artnr

**Bezeichnung**
Bezeichnung wird für den ausgewählten Artikel in Klartext dargestellt.
Technische Info: Alphanumerisches Feld, DB-Feld: artikel.artbez1

**SZR**
Angabe der SZR.
Technische Info: Alphanumerisches Feld, DB-Feld: xchangegrp.szr

# Artikel

## Artikel

Stammdaten > Artikel

Im Artikelstamm werden Daten hinterlegt, die die Merkmale und Eigenschaften von Artikeln beschreiben. Diese Daten repräsentieren das jeweilige Produkt und nehmen Einfluss auf die verschiedensten Bereiche (z. B. Auftragserfassung, Produktion, Lager, etc.).

Die im Artikelstamm festgehaltenen Daten geben im wesentlichen Auskunft über die
- Beschaffenheit
- Verfügbarkeit
- Produzierbarkeit
- Buchhalterische Einschätzung
- Räumliche Maße
- Verwendung
- Identifizierung
- Zu-/Einordnung (in Gruppen, Typen, etc.) eines Artikels.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Artikel-Kopf" auf Seite B-378
- "Identifikation" auf Seite B-381
- "Physikalische Eigenschaften" auf Seite B-388
- "Maßrestriktionen" auf Seite B-394
- "Einbaurestriktionen" auf Seite B-396
- "Beschaffung" auf Seite B-398
- "Produktion" auf Seite B-401
- "Preise" auf Seite B-405
- "Lager" auf Seite B-409
- "Technische Werte" auf Seite B-412
- "Statistik" auf Seite B-415
- "Modifikation" auf Seite B-417
- "Privat" auf Seite B-418
- "Artikel - Kontextmenü" auf Seite B-379

## Artikel-Kopf

In diesem Dialog können Sie einen Artikel auswählen, um die Artikeldaten anschauen bzw. zu ändern, oder Sie können eine Nummer für einen neuen Artikel vergeben lassen.

`<F6>` gibt die nächste freie Nummer für die Artikelerfassung aus dem entsprechenden Nummernkreis. Wenn Sie die neue Artikelnummer nach bestimmten Kriterien vergeben, z. B. nach Artikeltyp, müssen Sie die Nummer selbst vergeben. Zur Neuerfassung können Sie einen Musterartikel verwenden. Das Programm führt Sie mithilfe einer Meldung hindurch. Sie können anschließend die benötigte Felder ändern.

Die Inhalte der einzelnen Register beziehen sich immer auf den im Kopf gewählten Artikel.

*Abb. B-176 Artikel - Kopf*

**Artikel**
Auswahl der Artikelnummer mit `<F9>`. Jeder Artikel wird über seine Artikelnummer eindeutig identifiziert. Eine Artikelnummer darf nur ein Mal vergeben werden. Die Hauptbezeichnung für den Artikel wird hinter dem Feld in Klartext dargestellt. Für die neuerfasste Artikel ohne Musterartikel wird die Bezeichnung erst nach dem anfänglichen Speichern dargestellt.
Technische Info: Pflichtfeld, Numerisches Feld, `<F9>`, DB-Feld: artikel.artnr

Der Dialog beinhaltet verschiedene Register. Die Inhalte der einzelnen Register können - abhängig von Auswahl und Konfiguration - unterschiedlich sein.
- ⇨"Identifikation" auf Seite B-381
- ⇨ "Physikalische Eigenschaften" auf Seite B-388
- ⇨ "Maßrestriktionen" auf Seite B-394
- ⇨ "Einbaurestriktionen" auf Seite B-396
- ⇨ "Beschaffung" auf Seite B-398
- ⇨ "Produktion" auf Seite B-401
- ⇨ "Preise" auf Seite B-405
- "Lager" auf Seite B-409
- "Technische Werte" auf Seite B-412
- "Statistik" auf Seite B-415
- ⇨ "Modifikation" auf Seite B-417
- "Privat" auf Seite B-418
- "Artikel - Kontextmenü" auf Seite B-379

## Artikel - Kontextmenü

Stammdaten > Artikel > <F4>

Über das Kontextmenü (<F4>) haben Sie Zugriff auf folgende Bereiche:

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Lieferanten | ⇨ "Lieferanten - Zuordnung" auf Seite B-419 |
| b | Marktpartnerangaben | ⇨ "Marktpartnerangaben" auf Seite B-421 |
| C | Varianten | ⇨ "Maßvarianten" auf Seite B-424 |
| d | Farben/Größen | "Farben- / Größenvarianten" auf Seite B-427 |
| ea | Vermaßung- Zwingende Maßangaben | ⇨ "Zwingende Maßangaben – Maßparameter-Auswahl" auf Seite B-431 |
| eb | Vermaßung - Artikel-Vermaßung | ⇨ "Artikel-Vermaßung – Maßparameter" auf Seite B-437 |
| ec | Vermaßung - Modell-Vermaßung | ⇨ "Modell-Vermaßung" auf Seite B-445 |
| ed | Vermaßung - Produktbemaßung löschen | ⇨ "Produktbemaßung löschen" auf Seite B-446 |
| f | Stückliste | ⇨ "Stückliste" auf Seite B-486 |
| g | Stücklisten-Restriktionen | "Stücklisten-Restriktionen" auf Seite B-448 |
| h | Preiseigenschaften | ⇨ "Preiseigenschaften" auf Seite B-449 |
| i | Weitere Bezeichnungen | ⇨ "Weitere Artikelbezeichnungen" auf Seite B-452 |
| ja | Artikeltexte | ⇨ "Artikeltexte" auf Seite B-454 |
| jb | Kunden-Artikeltexte | ⇨ “Kunden-Artikeltexte" auf Seite B-455 |
| jc | Objekt-Artikeltexte | ⇨ "Objekt-Artikeltexte" auf Seite B-456 |
| k | Beschaffungsarten | ⇨ "Beschaffungsarten" auf Seite B-459 |
| l | Artikel-Datenabgleich | ⇨ "Artikel an A+W CAD Designer (Bars) senden" auf Seite B-462<br>⇨ "Beschlagartikel-Abgleich" auf Seite B-463 |
| I c | Artikel-Datenabgleich - Replikationsdaten | ⇨ "Replikationsdaten" auf Seite B-464 |
| ma | Produktkennzeichnung | ⇨ "Produktkennzeichnung" auf Seite B-466 |
| mb | Erweiterte techn. Werte | "Artikelbilder" auf Seite B-473 |
| n | Konfigurierte Felder | ⇨ "Konfigurierte Felder" auf Seite B-472 |
| Ο | Artikelbilder | "Artikelbilder" auf Seite B-473 |
| pa | Hausspezifische Angaben - Artikel | "Hausspezifische Artikel-Angaben" auf Seite B-475 |
| pb | Hausspezifische Angaben - Lieferanten | ⇨ "Hausspezifische Lieferanten-Angaben" auf Seite B-480 |
| pc | Hausspezifische Angaben - Varianten | ⇨ "Hausspezifische Varianten-Angaben" auf Seite B-481 |
| pd | Hausspezifische Angaben - Farben/Größen | ⇨ "Hausspezifische Farben/Größen-Angaben" auf Seite B-483 |

## Identifikation

Stammdaten > Artikel > Identifikation

*Abb. B-177 Artikel - Identifikation*

Im Register Identifikation werden einem Artikel die wichtigsten Kriterien zugeordnet.
Mit `<F5>` öffnen Sie einen Dialog, in dem Sie Anmerkungstexte zu dem Artikel hinterlegen können.
Mit `<Shift><F5>` öffnen Sie einen Dialog, in dem Sie Artikel-Anmerkungstexte zu dem Marktpartner hinterlegen können.
⇨ "Artikel - Anmerkungstexte" auf Seite B-386

### Erläuterung der Felder

**Matchcode**
Der Matchcode eines Artikels erleichtert das Auffinden des Artikels mittels Matchcodesuche innerhalb des Systems. Wenn ein Artikel neu angelegt wird, muss der Matchcode eingegeben werden. Dies kann ein entsprechender Name für den Artikel sein, der aus Buchstaben und Zahlen bestehen kann. Der Matchcode kann für mehrere Artikel identisch sein.
Technische Info: Pflichtfeld, Alphanumerisches Feld, DB-Feld: artikel.artmc

**Artikelcode**
Dieses Feld dient dazu, eine zusätzliche, kundenindividuelle Bezeichnung zu hinterlegen (wird häufig im asiatischen Raum verwendet).
Technische Info: Alphanumerisches Feld, DB-Feld: artikel.artikelcode

**Hauptbezeichnung**
Hier wird die Bezeichnung oder der Name des Artikels eingetragen. Die Hauptbezeichnung des Artikels erscheint bei der Auftragserfassung, auf Ausdrucken usw.
Wenn der Artikel angelegt wurde, erscheint die Hauptbezeichnung hinter dem Feld Artikel und in der SELO-Suche hinter der Artikelnummer.
Mit `<F5>` öffnen Sie den Dialog Artikelbezeichnungen. Dort können Sie weitere und fremdsprachige Bezeichnungen für den Artikel hinterlegen.
⇨ "Weitere Artikelbezeichnungen" auf Seite B-452
Technische Info: Pflichtfeld, Alphanumerisches Feld, DB-Feld: artikel.artbez1

**Internbez.**
In diesen Feldern können interne Bezeichnungen des Artikels aufgenommen werden. Wenn Sie die Artikel über die BME CAT-Schnittstelle importieren, so wird die Artikelbezeichnung des Herstellers in dieses Feld mitübernommen.
In der erweiterten Artikelsuche kann ebenfalls nach dieser Bezeichnung gesucht werden.
Technische Info: alphanumerische Felder, DB-Felder: artikel.artbez2, artikel.artbez3

**Kurzbezeichnung**
Falls auf Papieren, die wenig Platz für die Artikelbezeichnung bieten (z. B. Etiketten), eine Kurzbezeichnung des Artikels erscheinen soll, kann diese hier festgehalten werden.
Technische Info: Alphanumerisches Feld, DB-Feld: artikel.kurzbez

**Warengruppe**
Jedem Artikel muss eine eindeutige Warengruppe zugeordnet werden. Die Warengruppe bestimmt die Preiskonditionen des Artikels und ist die Basis für statistische Auswertungen. Es können warengruppenorientierte Statistiken geführt werden.
Warengruppen werden im Menü Stammdaten > Warengruppen angelegt.
⇨ "Warengruppen" auf Seite B-492
Technische Info: Pflichtfeld, Alphanumerisches Feld, `<F9>`, DB-Feld: artikel.wagrp

**Bezeichnung**
Hier wird zur Information die gewählte Warengruppe in Klartext wiedergegeben (nicht auswählbar).
Technische Info: Alphanumerisches Feld, DB-Feld: wargrp.wgrbez

**Artikelart**
Hier müssen Sie die Artikelart für Ihren Artikel wählen. Folgende Auswahlmöglichkeiten stehen zur Verfügung:
- **Teil:** Teile sind alle A+W Enterprise-Artikel, die physisch existierendes Material beschreiben. Hierbei wird nicht zwischen Kopfteil (Produkt) und Unterteil unterschieden.
- **Meta-Teil:** Meta-Teile sind alle A+W Enterprise-Artikel, die der besseren Lesbarkeit oder der vereinfachten Handhabung von Stücklisten dienen. Sowie Teile, die der Einbringung von Formeln in bestehende Stücklisten dienen.
- **Bearbeitung:** Beim Artikel handelt es sich um eine Bearbeitung, beispielsweise Zuschnitt, Kanten schleifen, Entsorgung usw.
Technische Info: Toggle-Feld, DB-Feld: artikel.teilflag

**Bearbeitungsart**
Wenn im Feld Artikelart Bearbeitung gewählt wurde, muss hier ausgewählt werden, um was für eine Bearbeitung es sich handelt. Die Bearbeitungsart hat Auswirkungen auf Preise und Konditionen sowie auf die Ecken- und Kantendefinition in der Vorgangserfassung. Das Feld bestimmt den Aufbau des Bearbeitungsvektors.
Folgende Auswahlmöglichkeiten stehen zur Verfügung:
- **(leer):** Bei diesem Artikel handelt es sich um sonstige Bearbeitung, beispielsweise Bohren, Entsorgung, Fracht usw.
- **Ecken:** Bei diesem Artikel handelt es sich um eine Eckbearbeitung, beispielsweise Eckausschnitt.
- **Kanten:** Bei diesem Artikel handelt es sich um eine Kantenbearbeitung, beispielsweise Kanten schleifen.
- **Facetten:** Bei diesem Artikel handelt es sich um einen Facettenschliff.
Technische Info: Toggle-Feld, DB-Feld: artikel.ekflag

**Artikeltyp**
In diesem Feld muss der Artikeltyp ausgewählt werden. Der ausgewählte Artikeltyp wird hinter dem Feld in Klartext dargestellt. Unter einem Artikeltyp werden Artikel gleicher Art (und Maßangaben) zusammengefasst. Der Artikeltyp ist beispielsweise notwendig, um die Austausch-/Zusatzregeln richtig anwenden zu können und um Restriktionsprüfungen und Preisberechnungen durchzuführen.
Beim Austausch wird beispielsweise geprüft, welche gleichwertigen Artikeltypen in den Stücklisten gegeneinander ausgetauscht werden können und ein Hinweis ausgegeben, wenn diese nicht zusammenpassen.
So wird bei der Auftragserfassung vermieden, dass beispielsweise ein Glas gegen eine Sprosse ausgetauscht wird.
Wenn Sie bei der Artikelsuche mit `<F9>` oder `<F8>` einen Startwert für den Artikeltyp vorgeben, wird der Artikeltyp nach der Bezeichnung sortiert, nicht nach der Nummer.
Technische Info: Pflichtfeld, `<F9>`, DB-Feld: artikel.atyp

**A+W Bearbeit.typ**
In diesem Feld muss der A+W normierte Bearbeitungstyp ausgewählt werden, wenn im Feld Artikelart Bearbeitung gewählt wurde. Der A+W normierte Bearbeitungskatalog ist eine verbindliche Norm für die Beschreibung von Bearbeitungsdaten für die verschiedenen A+W Programmpakete. Der A+W normierte Bearbeitungskatalog definiert übergreifend, welche Bearbeitungen unterstützt werden und mit welchen beschreibenden Parametern diese zu versehen sind.
Der ausgewählte Bearbeitungstyp wird hinter dem Feld in Klartext dargestellt. Es wird eine Plausibilitätsprüfung durch A+W Enterprise vorgenommen und ein Hinweis ausgegeben, wenn der A+W Bearbeitungstyp nicht zum Artikeltyp passt.
Nachdem der Bearbeitungstyp ausgewählt wurde, wird der Dialog Artikel-Vermaßung eingeblendet. In diesem Dialog können die Maßparameter erfasst werden.
⇨ Softwarereferenz, "Artikel-Vermaßung - Maßparameter" auf Seite B-437
Technische Info: Pflichtfeld, Numerisches Feld, `<F9>`, DB-Feld: artikel.awtyp

**Beschlagstyp**
In diesem Feld können Sie den Beschlagstyp für Beschläge auswählen (Artikeltyp Beschläge). Der ausgewählte Beschlagstyp wird hinter dem Feld in Klartext dargestellt.
Beschlagstypen werden in den Stammdaten > Schlüssel > Produkte > Beschlagstypen angelegt.
Technische Info: `<F9>`, DB-Info: artikel.btyp

**Rahmentyp**
In diesem Feld können Sie den Rahmentyp für Abstandhalter und ISO-Rahmen auswählen (Artikeltyp Abstandshalter oder ISO-Rahmen). Die Auswahl des Rahmentyps wirkt in der Vorgangserfassung auf die Darstellung des Glasaufbaus: verschiedene Rahmentypen werden in unterschiedlichen Farben dargestellt.
Folgende Auswahlmöglichkeiten stehen zur Verfügung:
- **Stahl:** Es handelt sich um einen Stahlrahmen.
- **Alu:** Es handelt sich um einen Aluminiumrahmen.
- **TPS:** Es handelt sich um einen thermo plast spacer (TPS).
Rahmentypen werden in den Stammdaten > Schlüssel > Produkte > Rahmentypen angelegt.
⇨ "Bezeichnungen für Rahmentypen" auf Seite B-350
Technische Info: `<F9>`, DB-Feld: artikel.rtyp

**Versiegelungstyp**
In diesem Feld können Sie den Versiegelungstyp für die Dichtstoffe (Artikeltyp 240) auswählen.
Versiegelungstypen werden in den Stammdaten > Schlüssel > Produkte > Versiegelungstypen angelegt.
⇨ "Bezeichnungen für Versiegelungstypen" auf Seite B-352
Technische Info: `<F9>`, DB-Feld: artikel.versiegelungstyp

**Folientyp**
In diesem Feld können Sie den Folientyp für die Folien (Artikeltyp Folien) auswählen.
Folientypen werden in den Stammdaten > Schlüssel > Produkte > Folientypen angelegt.
⇨ "Bezeichnungen für Folientypen" auf Seite B-348
Technische Info: `<F9>`, DB-Feld: artikel.folienstyp

**EAN-Code**
Hier kann ein gültiger Barcode für den Artikel eingegeben werden.
Ein EAN-Code dient der gesamteuropäischen Identifikation von Artikeln und deren Zuordnung zu Artikelgruppen, Warengruppen oder Warenbereichen. Die beiden ersten Stellen des 13-stelligen Codes kennzeichnen das Herkunftsland, die nächsten 5 die bundeseinheitliche Betriebsnummer (bbn), die nächsten 5 die individuelle Artikelnummer des Herstellers und die letzte Ziffer dient als Prüfziffer.
Es müssen nur die ersten 12 Ziffern eingegeben werden, die Prüfziffer wird vom System berechnet.
Der EAN-Code erscheint dann auf Ausdrucken, wie beispielsweise den Etiketten.
Technische Info: Numerisches Feld, DB-Feld: artikel.eancode

**Diverser Artikel**
Hier kann angegeben werden, ob es sich um ein Kleinteil handelt. Bei Diversen Artikeln kann in der Vorgangserfassung der Artikeltext geändert werden. Er erhält dann in der Vorgangserfassung für jede Position eine neue Stücklistennummer. So muss nicht für jedes Kleinteil im Barverkauf eine eigene Artikelnummer existieren.
Folgende Auswahlmöglichkeiten stehen zur Verfügung:
- **nein:** Es handelt sich nicht um einen diversen Artikel.
- **ja:** Es handelt sich um einen diversen Artikel.
Technische Info: Toggle-Feld, DB-Feld: artikel.tmpartkz

**Anmerkungen**
Wenn Artikel-Anmerkungen hinterlegt sind, dann werden diese hier angezeigt.

### Ergänzende Informationen

- ⇨ "Artikel - Anmerkungstexte" auf Seite B-386
- ⇨ "Marktpartner - Anmerkungstexte" auf Seite B-106

## Artikel - Anmerkungstexte

Stammdaten > Artikel > <F5>

*Abb. B-178 Artikel - Anmerkungstexte*

In diesem Dialog können Sie Texte für Artikel hinterlegen, die in den verschiedensten Programmteilen als wichtiges Informationsmedium dienen. Oben im Dialog sehen Sie die Artikel-Nummer, für die der Text gilt.

> **Mehrsprachige Anmerkungen**
> Seit QR2209 können Sie in A+W Enterprise auch für Anmerkungen mehrsprachige Bezeichnungen hinterlegen. Diese Möglichkeit besteht jedoch nur, wenn Sie mit dem Modul Mehrsprachigkeit für Mitarbeiter innerhalb der internen Mandantentrennung arbeiten.

**Sprache**
Sprachkennzeichen.
Technische Info: Numerisches Feld, DB-Feld: xsprbez.sprkz

Geben Sie den Text in dem freien Feld ein und speichern Sie diesen mit `<F3>`.

Mit `<Shift><F9>` legen Sie den Info-Ort fest:
- **Stammdaten:** Der Text wird nur in den Stammdaten angezeigt.
- **Überall:** Der Text wird in den Stammdaten und in den Verkaufs- und Einkaufsvorgängen angezeigt, wenn dieser Artikel als Position erfasst wird. Oder wenn er im Feld Unterteil mit ja/mit Anmerkung markiert wurde.
- **VK-Auftrag:** Der Text wird im Verkaufsvorgang angezeigt, wenn der Artikel als Position im Vorgang erfasst wird. Oder wenn er im Feld Unterteil mit ja/mit Anmerkung markiert wurde.
- **EK-Auftrag:** Der Text wird im Einkaufsvorgang angezeigt, wenn der Artikel als Position im Vorgang erfasst wird. Oder wenn er im Feld Unterteil mit ja/mit Anmerkung markiert wurde.

Mit `<Shift><F10>` legen Sie die Priorität fest:
- **hoch:** Der Text wird an den festgelegten Info-Orten automatisch angezeigt, sobald nur eine Zeile die Prio-hoch hat.
- **niedrig:** Der Text wird nicht automatisch angezeigt, er muss bei der Vorgangserfassung über das Menü aufgerufen werden.

> **Priorität bei Info-Ort Stammdaten**
> Wenn Sie als Info-Ort Stammdaten gewählt haben, greift die Priorität niedrig nicht. Der Text wird immer in den Stammdaten des Artikels angezeigt.

Technische Info: Alphanumerisches Feld, DB-Feld: memo.txt
Sie können beliebig viele Textzeilen hinterlegen.

## Physikalische Eigenschaften

Stammdaten > Artikel > Register Phys. Eigenschaften

*Abb. B-179 Artikel - Register Physikalische Eigenschaften*

Im Register Phys. Eigenschaften werden die physikalischen Eigenschaften des Artikels angelegt.

### Erläuterung der Felder

**Modell**
Wenn es sich bei dem Artikel um einen Modellartikel handelt, können Sie hier ein Modell aus dem Modellkatalog auswählen.
Wenn ein Modell gewählt wurde, können Sie mit `<F5>` den Dialog Modellparameter öffnen, in dem Sie die Maße des Artikels eingeben können.
Technische Info: Numerisches Feld, `<F9>`, DB-Feld: artikel.modell

**ME**
In diesem Feld müssen Sie eine Mengeneinheit für den Artikel auswählen. Die gewählte Mengeneinheit wird hinter dem Feld in Klartext dargestellt. Die Mengeneinheit beispielsweise steuert bei der Vorgangserfassung die Art und Anzahl der Parameter, die eingegeben werden müssen, um das Produkt vollständig zu beschreiben. Wenn die gewählte Mengeneinheit beispielsweise Fläche ist, werden bei der Vorgangserfassung Breite und Höhe des Artikels abgefragt, bei Laufmeter die Länge usw.
Die gewählte Mengeneinheit beeinflusst außerdem die Gewichtsberechnung, die Preisberechnung, die Kostenrechnung und die Lagerabbuchungen.
Die entsprechenden Einheiten werden im Menü Mengeneinheiten (Stammdaten > Schlüssel > System) hinterlegt.
Technische Info: Numerisches Feld, Pflichtfeld, `<F9>`, DB-Feld: artikel.me

**Gewicht**
In diesem Feld kann das Gewicht pro Mengeneinheit eingetragen werden. Diese Information ist wichtig für die Berechnung des Gesamtgewichtes in der Auftragserfassung sowie für Versand, Packmittelplanung und die Rabattermittlung.
Technische Info: Numerisches Feld, DB-Feld: artikel.gew

**Produktgewicht**
In diesem Feld können Sie wählen, ob beim Ermitteln des Produktgewichts alle Teile der Stückliste berechnet werden sollen oder ob bei der Berechnung nur das Produktgewicht von diesem Artikel verwendet wird.
- Bei der Gewichtsermittlung wird nur dieser Artikel berücksichtigt.
- Das Gesamtgewicht aller Einzelteile in der Stückliste wird berechnet.
Wenn Sie die Checkbox aktivieren, können Sie durch eine zusätzliche Systemkonfiguration erreichen, dass das Produktgewicht trotzdem in die Berechnung einfließt, sofern dieser Artikel in die Stückliste eingetauscht wird.
Technische Info: Toggle-Feld, DB-Info: artikel.produktgew

**Dickenmaß**
In diesem Feld wird die Artikelstärke bzw. -dicke in mm angegeben. Anhand dieses Maßes werden die Betriebsmittel für die Produktionssteuerung und Packmittelplanung gewählt und die Preisberechnung für bestimmte Bearbeitungen durchgeführt. Ebenso wird aufgrund des Dickenmaßes die Berechnung der technischen Werte durchgeführt und die Stärke der ISO-Einheiten berechnet.
Technische Info: Numerisches Feld, DB-Feld: artikel.staerke

**Frästiefe**
Das Feld ist nur aktiv, wenn es sich bei dem Artikel um eine Sprosse handelt. Dann geben Sie hier die Frästiefe der Sprossen in mm ein.
Technische Info: Numerisches Feld, DB-Info: artikel.fraestiefe

**Trim-Wert**
Das Feld ist nur aktiv, wenn es sich bei dem Artikel um eine Sprosse handelt. Dann geben Sie hier den Trim-Wert der Sprossen in mm ein.
Technische Info: Numerisches Feld, DB-Info: artikel.trim_wert

**Profildicke**
Das Feld ist nur aktiv, wenn es sich bei dem Artikel um eine Sprosse handelt. Dann geben Sie hier die Profildicke der Sprossen in mm ein.
Technische Info: Numerisches Feld, DB-Info: artikel.dicke

**Maßvariante**
In diesem Feld können Sie bestimmen, ob dieser Artikel nur in bestimmten Maßvarianten verfügbar ist:
- Zu diesem Artikel existieren Maßvarianten.
- Zu diesem Artikel existieren keine Maßvarianten.
Wenn Sie Maßvarianten angewählt haben, gelangen Sie mit `<F5>` in den Dialog Varianten. In diesem Dialog können Sie Maßvarianten vorgeben und in einem weiteren Dialog die Beschaffungskriterien vergeben.
⇨ "Maßvarianten" auf Seite B-424
Technische Info: Toggle-Feld, DB-Info: artikel.varflag

**Farbenvariante/Größenvariante**
In diesem Feld können Sie wählen, ob zu diesem Artikel Farbvarianten oder Größenvarianten erfasst werden können oder nicht:
- **Farben:** Der Artikel ist in bestimmten Farben verfügbar.
- **Größen:** Der Artikel ist in bestimmten Größen verfügbar.
- **(keine):** Es wurde keine Auswahl getroffen oder es wurde Maßvariante gewählt.
Wenn Sie Farben oder Größen angewählt haben, gelangen Sie mit `<F5>` in den Dialog Farben/Größen.
"Maßvarianten" auf Seite B-424
In diesem Dialog können Sie Farb- oder Größenvarianten vorgeben und in einem weiteren Dialog die Beschaffungskriterien vergeben.
Technische Info: Toggle-Feld, DB-Feld: artikel.farbflag

**Oberfläche**
In diesem Feld können Sie Angaben zur Oberflächenbeschaffenheit von Gläsern machen. Dies ist beispielsweise bei der Zuschnittsreihenfolge oder für die Verlaufsrichtung einer Struktur wichtig:
- **keine:** Das Glas besitzt keine besondere Oberfläche.
- **Struktur einseitig:** Das Glas ist auf einer Seite strukturiert.
- **Struktur zweiseitig:** Das Glas ist auf beiden Seiten strukturiert.
- **Beschichtung:** Das Glas ist beschichtet.
- **Re/Li-Bezug:** Das Glas hat eine Struktur, deren Verlauf oder strukturierte Seite bei der Bearbeitung beachtet werden muss. Die Scheibe kann nicht gedreht werden!
Technische Info: Toggle-Feld, DB-Feld: artikel.strukseite

**Struktur**
Wenn im Feld Oberfläche eine Struktur oder Re/Li-Bezug gewählt wurde, kann in diesem Feld die Strukturrichtung oder die strukturierte Seite angegeben werden:
- **senk:** Die Struktur verläuft senkrecht.
- **waag:** Die Struktur verläuft waagerecht.
- **diag:** Die Struktur verläuft diagonal.
Folgende Auswahlmöglichkeiten stehen bei Re/Li-Bezug für seitenbezogene Artikel zur Verfügung:
- **rechts:** Strukturverlauf rechts.
- **links:** Strukturverlauf links.
Technische Info: Toggle-Feld, DB-Feld: artikel.strukhb

**Einbaupos**
Wenn im Feld Oberfläche eine Beschichtung, eine Struktur oder Re/Li-Bezug gewählt wurde, kann in diesem Feld die Einbauposition des Glases in den Rahmen angegeben werden.
Die Einbauposition wird gemäß der folgenden Abbildung bestimmt.
*Abb. B-180 Einbauposition der Gläser*

Technische Info: Numerisches Feld, DB-Feld: artikel.einbaupos

**Lage zum SZR**
Wenn Sie einen ISO-Artikel mit einer beschichteten oder strukturierten Scheibe erfassen, müssen Sie hier angeben, in welche Richtung diese Oberfläche eingebaut werden muss:
- **Vom SZR wegzeigend:** Die behandelte Oberfläche ist auf der Außenseite des ISO-Glases.
- **Zum SZR:** Die behandelte Oberfläche zeigt zum Scheibenzwischenraum.
Technische Info: Toggle-Feld, DB-Feld: artikel.einbauposstkl

**Verkaufs-Art.**
In diesem Feld können Sie festlegen, ob der Artikel zum Weiterverkauf (Einzelverkauf) vorgesehen ist oder nicht:
- **Ja:** Der Artikel ist als selbstständiger Artikel zum Weiterverkauf vorgesehen. Dieser Artikel kann in der Vorgangserfassung als Position erfasst werden.
- **Nein:** Der Artikel ist nicht zum Weiterverkauf vorgesehen. Dieser Artikel kann in der Vorgangserfassung nicht als Position erfasst werden. Dieser Artikel kann aber in einer Stückliste aufgenommen werden.
- **+Online:** Der Artikel ist zum Verkauf über Internet vorgesehen.
Technische Info: Toggle-Feld, DB-Feld: artikel.verkart

**Stückliste**
In diesem Feld können Sie hinterlegen, ob zum Artikel eine Stückliste vorhanden ist oder nicht:
- **nein:** Der Artikel besitzt keine Stückliste.
- **ja/änderbar:** Der Artikel besitzt eine Stückliste. In der Vorgangserfassung können an dieser Stückliste Änderungen vorgenommen werden. Es können dann beispielsweise in der Stückliste Artikel hinzugefügt oder ausgetauscht werden.
- **ja/starr:** Der Artikel besitzt eine Stückliste. In der Vorgangserfassung können an dieser Stückliste keine Änderungen vorgenommen werden.
Wenn Sie Stückliste ja gewählt haben, können Sie mit `<F5>` den Dialog Stückliste öffnen, um weitere Eingaben vorzunehmen.
Technische Info: Toggle-Feld, DB-Feld: artikel.stklst

**Unterteil**
In diesem Feld können Sie wählen, ob der Artikel in der Stückliste eines anderen Artikels vorkommen kann:
- **nein:** Der Artikel kann nicht als Unterteil einer Stückliste vorkommen.
- **ja:** Der Artikel kann als Unterteil einer Stückliste vorkommen.
- **ja/statistikrelevant:** Der Artikel muss als Unterteil einer Stückliste vorkommen. Der Artikel geht in die Teilverwendungsstatistik ein.
- **ja/mit Anmerkung:** Der Artikel kann als Unterteil einer Stückliste vorkommen. Wenn zu dem Artikel eine Anmerkung hinterlegt ist, wird diese in der Vorgangserfassung angezeigt.
Technische Info: Toggle-Feld, DB-Feld: artikel.uteil

**Stkl. Austausch**
Wenn im Feld Unterteil ja gewählt wurde, kann in diesem Feld bestimmt werden, ob der Artikel in der Stückliste gegen einen anderen Artikel ausgetauscht werden kann oder nicht.
- Der Artikel kann in einer Stückliste gegen einen anderen Artikel ausgetauscht werden.
- Der Artikel kann in einer Stückliste nicht gegen einen anderen Artikel ausgetauscht werden.
Technische Info: Toggle-Feld, DB-Info: artikel.azastkl

**Ausdruck**
In diesem Feld können Sie festlegen, welche Maßdaten des Artikels auf kundenseitigen Papieren ausgedruckt werden:
- **nein** Es werden keine Maßdaten gedruckt.
- **qm** Die Quadratmeter des Artikels werden gedruckt.
- **qm+umlfdm** Die Quadratmeter und umlaufenden Meter des Artikels werden gedruckt.
- **umlfdm** Die umlaufenden Meter des Artikels werden gedruckt.
- **B+H** Die Breite und die Höhe des Artikels werden gedruckt.
Technische Info: Toggle-Feld, DB-Feld: artikel.qmlfm

**Zusatzformel**
In diesem Feld können Sie eine Formel hinterlegen, die für den Artikel im Falle eines Austauschs oder Zusatzes gilt. Wenn im Vorgang der Artikel als Zusatz in eine Stückliste aufgenommen wird, wird diese Maßvererbungsformel verwendet.
Mit `<F5>` kann der Formeleditor aufgerufen und Formeln erfasst werden.
Technische Info: Numerisches Feld, `<F9>`, DB-Feld: artikel.azformel

**Verkaufspapiere**
In diesem Feld können Sie wählen, ob das Druckkennzeichen in der Stückliste der Vorgangserfassung beim Eintauschen des Artikels vorbelegt werden soll oder nicht.
- Das Druckkennzeichen wird in der Stückliste der Vorgangserfassung beim Eintauschen des Artikels vorbelegt.
- Das Druckkennzeichen wird in der Stückliste der Vorgangserfassung beim Eintauschen des Artikels nicht vorbelegt.
Technische Info: Toggle-Feld, DB-Info: artikel.vdruckkz

### Ergänzende Informationen

- ⇨ "Mengeneinheitenbezeichnung" auf Seite B-247
- "Maßvarianten" auf Seite B-424
- "Farben- / Größenvarianten" auf Seite B-427
- ⇨ "Artikel - Anmerkungstexte" auf Seite B-386
- ⇨ "Marktpartner - Anmerkungstexte" auf Seite B-106

## Maßrestriktionen

Stammdaten > Artikel > Register Maßrestriktionen

*Abb. B-181 Artikel - Register Maßrestriktionen*

Im Register Maßrestriktionen werden die Maßrestriktionen für den Artikel festgelegt. Wird bei der Vorgangserfassung das hier hinterlegte Grenzmaß unter- oder überschritten, erhält der Erfasser in der Vorgangserfassung eine Meldung. A+W Enterprise prüft dabei alle Stücklistenteile.

A+W Enterprise prüft ebenfalls beim Ausfüllen dieses Dialoges, ob die maximalen Maße größer sind als die minimalen Maße. Ist dies nicht der Fall, werden Sie zur Korrektur aufgefordert.

### Erläuterung der Felder

**Breite maximal**
In diesem Feld können Sie die maximale Breite des Artikels eingeben.
Technische Info: Numerisches Feld, DB-Feld: artikel.pmaxb

**Breite minimal**
In diesem Feld können Sie die minimale Breite des Artikels eingeben.
Technische Info: Numerisches Feld, DB-Feld: artikel.pminb

**Höhe maximal**
In diesem Feld können Sie die maximale Höhe des Artikels eingeben.
Technische Info: Numerisches Feld, DB-Feld: artikel.pmaxh

**Höhe minimal**
In diesem Feld können Sie die minimale Höhe des Artikels eingeben.
Technische Info: Numerisches Feld, DB-Feld: artikel.pminh

**Fläche maximal**
In diesem Feld können Sie die maximal mögliche Fläche des Artikels eingeben.
Technische Info: Numerisches Feld, DB-Feld: artikel.pmaxfl

**Fläche minimal**
In diesem Feld können Sie die minimal mögliche Fläche des Artikels eingeben.
Technische Info: Numerisches Feld, DB-Feld: artikel.pminfl

**Seitenverh. maximal**
In diesem Feld können Sie das Seitenverhältnis eines Artikels auf einen Maximalwert beschränken.
Technische Info: Numerisches Feld, DB-Feld: artikel.pmaxsv

**Seitenverh. minimal**
In diesem Feld können Sie das Seitenverhältnis eines Artikels auf einen Minimalwert beschränken.
Technische Info: Numerisches Feld, DB-Feld: artikel.pminsv

**Drehbar**
Dieses Feld ist je nach Konfiguration auswählbar. Drehbar bedeutet, dass ein Artikel beim Prüfen der Maßrestriktionen Breite/Höhe getauscht werden kann.
- Der Artikel ist drehbar.
- Der Artikel ist nicht drehbar.
Technische Info: Alphanumerisches Feld, DB-Feld: artikel.drehbar

### Ergänzende Informationen

- ⇨ "Artikel - Anmerkungstexte" auf Seite B-386
- ⇨ "Marktpartner - Anmerkungstexte" auf Seite B-106

## Einbaurestriktionen

Stammdaten > Artikel > Register Einbaurestriktionen

*Abb. B-182 Artikel - Register Einbaurestriktionen*

Im Register Einbaurestriktionen werden die Bearbeitungsrestriktionen eines Artikels festgelegt. Wird bei der Vorgangserfassung das hier hinterlegte Grenzmaß unter- oder überschritten oder die Einbauregel nicht eingehalten, erhält der Erfasser eine Meldung.

### Erläuterung der Felder

**Bohrdurchm. maximal**
In diesem Feld können Sie den maximalen Bohrdurchmesser für den Artikel eingeben.
Technische Info: Numerisches Feld, DB-Feld: artikel.maxbohrdm

**Bohrdurchm. minimal**
In diesem Feld können Sie den minimalen Bohrdurchmesser für den Artikel eingeben.
Technische Info: Numerisches Feld, DB-Feld: artikel.minbohrdm

**Nur einbauen, wenn**
Mithilfe dieser Felder können Sie eine gültige Formel für die Einbaurestriktionen hinterlegen. Zwei Restriktionen werden mit **UND** bzw. **ODER** miteinander verknüpft.
Im ersten und dritten Feld können Sie mit `<F9>` jeweils eine gültige Variable auswählen. Anschließend wird in diesen Feldern hinter der Variable ein Operator gesetzt und ein Wert eingegeben.
Es können folgende Operatoren und Vergleichsoperatoren gesetzt werden:
- `+` Addition
- `-` Subtraktion
- `*` Multiplikation
- `/` Division
- `=` gleich
- `<` kleiner als
- `>` größer als
- `<=` kleiner oder gleich
- `>=` größer oder gleich
- `!=` ungleich
- `&` logisch und
- `and` logisch und
- `|` logisch oder
- `or` logisch oder
- `!` logische Negation (Verneinung)
- `not` logische Negation (Verneinung)
- `max (x, y)` der größte Wert von zweien
- `min (x, y)` der kleinste Wert von zweien
- `pi` Konstante Pi (3,1415926)

**Beispiel**

Eine Sprosse darf nur eingebaut werden, wenn der Scheibenzwischenraum bei einem ISO-Glas mindestens 16 mm und höchstens 20 mm beträgt.
Wählen Sie hierzu im ersten **Feld** für den Scheibenzwischenraum die Variable **SZR ($3)**.
Fügen Sie hinter der Variable $3 den Operator `<=` für kleiner oder gleich ein. Tragen Sie anschließend den Wert **20** ein.
Die Formel im ersten Feld würde nun wie folgt aussehen: **$3<=20**.
Die Formel im dritten Feld würde wie folgt aussehen: **$3>=16**.
Verbinden Sie die Formeln im zweiten Feld mit der Verknüpfung **UND**.
Das bedeutet, der Scheibenzwischenraum muss mindestens 16 mm (oder dicker) und gleichzeitig höchstens 20 mm (oder weniger) betragen.

> **Feldinhalt tauschen**
> Bei diesem Beispiel würde es keine Rolle spielen, wenn Sie den Feldinhalt des ersten und dritten Feldes vertauschen.

Technische Info: 1. und 3. Feld: alphanumerische Felder, `<F9>`, DB-Felder: artikel.ebrestrikt1, artikel.ebrestrikt2
2. Feld: Toggle-Feld, DB-Feld: artikel.operator

### Ergänzende Informationen

- ⇨ "Artikel - Anmerkungstexte" auf Seite B-386
- ⇨ "Marktpartner - Anmerkungstexte" auf Seite B-106

## Beschaffung

Stammdaten > Artikel > Register Beschaffung

*Abb. B-183 Artikel - Register Beschaffung*

Im Register Beschaffung werden die Daten für die Beschaffung des Artikels hinterlegt.

### Erläuterung der Felder

**Beschaffungsart**
Im Feld Beschaffungsart können Sie eine Beschaffungsart für den Artikel wählen. Die Beschaffungsarten bestimmen die Priorität, mit denen der Artikel beschafft wird. Die Priorität 2 greift dann, wenn Priorität 1 nicht durchführbar ist.
Mit `<F9>` oder `<F5>` öffnen Sie den Dialog Beschaffungsarten, in dem Sie eine der Beschaffungskriterien auswählen können <mit Enter>.
Technische Info: Numerisches Feld, `<F9>`, DB-Feld: artikel.beschaffnr

**Priorität 1, 2, 3**
In diesen Feldern wird die gewählte Kombination der ausgewählten Beschaffungsart aus dem Feld Beschaffungsart in Klartext dargestellt. Diese Felder beschreiben die Prioritäten, mit der ein Artikel beschafft werden soll.
Die gewählte Beschaffungsart kann in der Vorgangserfassung überschrieben werden.
Folgende Beschaffungsarten stehen zur Verfügung:
- **Lager:** Der Artikel wird dem Lager entnommen, solange er vorrätig ist.
- **Bestellung:** Der Artikel wird beim Zulieferer bestellt.
- **Produktion:** Der Artikel wird in der eigenen Firma produziert.
- **Keine:** Dem Artikel wird die Beschaffungsart keine zugewiesen. Dies kann beispielsweise beim Artikeltyp Abschlagsrechnung der Fall sein.
Technische Info: alphanumerische Felder

**Prod-Dauer**
Dieses Feld wird dann aktiviert, wenn eine der ersten beiden Prioritäten der Beschaffungsart Produktion ist.
Hier kann die Produktionszeit für den Artikel in Werktagen hinterlegt werden. Die Produktionszeit hat jedoch keine Auswirkung auf die tatsächliche Produktionsplanung.
Technische Info: Numerisches Feld, DB-Feld: artikel.prodzeit

**Lieferant**
Dieses Feld wird dann aktiviert, wenn eine der ersten beiden Prioritäten der Beschaffungsart Bestellung ist.
Mit `<F5>` öffnen Sie den Dialog Lieferanten. Dort können Sie einen Standardlieferanten hinterlegen und weitere Lieferanten einfügen.
Der Standardlieferant wird dann in diesem Feld in Klartext dargestellt.
Technische Info: Numerisches Feld, DB-Feld: artikel.stdlinr

**Lieferzeit**
Wenn im Feld Lieferant ein Standardlieferant und eine Lieferzeit für den Artikel gewählt wurde, wird hier diese Lieferzeit in Tagen angezeigt.
Technische Info: Numerisches Feld, DB-Feld: artikel.stdiz

**EK-Abteilung**
In den Warengruppen sind die Einkaufsabteilungen hinterlegt. Wenn eine abweichende Einkaufsabteilung gewählt werden soll, kann diese hier ausgewählt werden. Die gewählte Einkaufsabteilung wird hinter diesem Feld in Klartext dargestellt.
Technische Info: Numerisches Feld, `<F9>`, DB-Feld: artikel.ekabt

**A/Z-Beschaffart**
Wenn ein Artikel als Stücklistenunterteil anders beschafft werden soll als wenn er als Positionsartikel erfasst wird, können folgende Einstellungen vorgenommen werden:
- **keine:** Es wird keine abweichende Austauch-/Zusatz-Beschaffungsart gewählt.
- **Bestellung vor DFÜ:** Das Unterteil wird im eigenen Haus bestellt, bevor die Gesamtstückliste zum betreffenden Produktionshaus übertragen wird. Dem Empfänger wird das Teil als mitgeliefert gemeldet.
- **Lagerentnahme vor DFÜ:** Das Unterteil wird dem Lager entnommen, bevor die Gesamtstückliste zum betreffenden Produktionshaus übertragen wird. Dem Empfänger wird das Teil als mitgeliefert gemeldet.
- **Produktion vor DFÜ:** Das Unterteil wird im eigenen Haus produziert, bevor die Gesamtstückliste zum betreffenden Produktionshaus übertragen wird. Dem Empfänger wird das Teil als mitgeliefert gemeldet.
- **Bestellung:** Der Artikel wird beim Zulieferer bestellt.
- **Lagerentnahme:** Der Artikel wird aus dem Lager entnommen.
- **Produktion:** Der Artikel wird in der eigenen Firma produziert.
- **Mitgeliefert:** Der Artikel wird vom Kunden/an den Lieferanten mitgeliefert.
- **Mitgeliefert vor DFÜ:** Bevor der Artikel per DFÜ in einem anderen Haus bestellt wird, wird die Beschaffungsart ausgewertet – der Artikel wird mitgeliefert.
Technische Info: Toggle-Feld, DB-Feld: artikel.bestellkz

### Ergänzende Informationen

- ⇨ "Beschaffungsarten" auf Seite B-459
- ⇨ "Lieferanten - Zuordnung" auf Seite B-419
