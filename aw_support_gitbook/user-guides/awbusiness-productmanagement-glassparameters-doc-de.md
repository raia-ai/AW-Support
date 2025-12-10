---
title: "D-AWBusiness-HB_8"
source: "D-AWBusiness-HB_8.pdf"
tags: ["A+W Business", "Software Reference", "Product Management", "Glass Parameters", "Master Data", "ERP", "Technical Documentation", "German"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference manual for A+W Business, focusing on product management (Produktverwaltung). It details the configuration of various product parameters, particularly for glass manufacturing, including master data for articles, pricing, and technical specifications."
long_description: "This extensive technical document serves as a software reference guide for the A+W Business ERP system, specifically covering the 'Produktverwaltung' (Product Management) module. It provides a detailed breakdown of master data management for various articles, with a strong emphasis on glass products. The manual guides users through setting up A+W Production parameters, such as glass types, grinding groups, and processing times. It covers the management of technical specifications like U-values, g-values, and sound insulation ratings, as well as production-related settings for cutting tables and processing lines. The document also explains how to handle classifiers, attachments, pricing structures (including price lists, surcharges, and discounts), product variants, and bill of materials (BOM) components like mullions (Sprossen) and spacers (Abstandhalter). It is designed for system administrators and power users responsible for configuring and maintaining product data within the A+W Business environment to ensure accurate production planning, pricing, and order processing."
---

# Produktverwaltung

Die Felder im Bereich **Artikel** sind zum Register **Produkt** beschrieben.
⇨ "Produktverwaltung - Produkt" auf Seite B-600

---
## A+W Production Glasparameter

**Glasart**
Das aktuelle Glasprodukt ist einer Glasart zugeordnet. Über den Ordner öffnen Sie den Dialog Glasarten, in dem Sie Glasarten anlegen können.
⇨ "Glasarten" auf Seite B-644

**Schleifgruppe**
Beim Schleifen und Bearbeiten ist ein Maßzuschlag für die Kanten notwendig, damit die Scheibe auf das Nennmaß bearbeitet werden kann. Diese Schleifzuschläge sind von vier Faktoren abhängig:
- Glasart
- Maschine
- Bearbeitungsart
- Glasdicke

Um nicht für jede einzelne Glasart, Maschine und Bearbeitung einen eigenen Zuschlag erfassen zu müssen, werden diese Kriterien in A+W Production in Gruppen zusammengefasst. Es stehen folgende Gruppen zur Verfügung:
- Standard
- Artikelschleifgruppen
- Maschinenschleifgruppen
- Bearbeitungsschleifgruppen

**Übergangszeit**
Bei einigen Produkten muss zwischen dem Übergang von einem Produktionsbereich zum nächsten oder zum nachfolgenden Arbeitsgang eine Ruhezeit eingehalten werden, z. B. nach dem Härten. Die Zeit wird in ganzen Tagen angegeben. Dieser Wert wird von den Werten der eingesetzten Kapazitätsplanung überschrieben.

**[Glasart-Jumbos-Tische]**
Öffnet den Dialog Glasart-Jumbos-Tische. Die Schaltfläche ist nur bei Einfachglas freigeschaltet, das zugeschnitten wird.
⇨ "Glasart-Jumbos-Tische" auf Seite B-885

**Max. Traverenbreite**
Eingabe in mm. Die Breite der zu bildenden Traveren wird begrenzt. Der Wert ist abhängig von der Breite der Lagerplatte. Bei automatischen Brechanlagen gelten die Vorschriften des Herstellers.
Die Begrenzung ist zum einen notwendig, um das manuelle Brechen handlich zu machen, zum anderen können automatische Brechanlagen Traveren nur bis zu einer bestimmten Breite auf der dynamischen Brechstation verarbeiten.

**Min. Abst. X-Z Schnitte**
Mindestabstand zwischen X-Z-Schnitten. Ein Z-Schnitt verläuft zwischen zwei Y-Schnitten parallel zum X-Schnitt. Der Minimalabstand richtet sich in erster Linie nach der Glasdicke und ist für das manuelle Brechen notwendig.

**Reihenf. Opti.**
Reihenfolge, in der die Feinplanung die Optimierungen durchläuft. Je nach Einstellungen der Stammdaten auf- oder absteigend. Glasarten mit hohem Rang werden zuerst optimiert. Üblicherweise bekommen teure Glasarten einen hohen Rang.

**Min. Fläche automatische Opti.**
Fläche, ab der die Optimierung eingesetzt werden soll. Dieser Wert kann durch die Feinplanung überschrieben werden.

## Lage am Zuschnittstisch

**Strukturlage**
Lage der Struktur beim Zuschnitt. Diese Angabe ist wichtig, wenn das strukturierte Glas nur auf einer Seite geschnitten werden kann.

**Beschichtungslage**
Die Beschichtung muss in aller Regel oben liegen, um Beschädigungen durch die weitertransportierenden Rollen beim Zuschnitt zu vermeiden.

## Maschinenzentrum

Die Felder in diesem Bereich werden nicht ausgelesen, da die Zuordnung zu den Maschinen von A+W Production gesteuert wird.

**Nummer / logisch**
Zurzeit nicht genutzt.

**Dauer in Sekunden**
Zurzeit nicht genutzt.

## Bruchränder

Der Bruchrand gibt an, wie viel Rand auf der Platte mindestens vorhanden sein muss, damit die zugeschnittene Scheibe (ab)gebrochen werden kann.

**Modell**
Bruchrandwert für Modelle. Dieser Wert ist abhängig von der Glasdicke und der Form des Modells.

**Links, Rechts, Oben, Unten**
Bruchränder für Rechteckscheiben. Die Werte sind abhängig von der Glasdicke.

## A+W Production Bearbeitungsparameter

Die Felder dieser Gruppe sind nur bei Bearbeitungen freigeschaltet.

**Bearb.maße enthalten**
Insbesondere bei gestuften Scheiben muss beachtet werden, ob Bearbeitungsmaße enthalten sind, damit die Berechnung von weiteren Bearbeitungsmaßen zu korrekten Ergebnissen führt.

**Zuschnittsmaß korrigieren**
Zurzeit nicht genutzt.

**Explizite Planung**
Das Produkt kann explizit verplant werden. Wenn eine Bearbeitung als explizit gekennzeichnet ist, wird das zugehörige Produkt (Glas) als so genanntes Freigabeteil gekennzeichnet. In A+W Production können Freigabeteile aus der Stückliste gelöst und explizit verplant werden. In einer ISO-Einheit sind also die Scheiben Freigabeteile, an denen die Bearbeitung ausgeführt wird.

**Interne Bearbeitung**
Interne Bearbeitungen erzeugen ein neues (A+W Production-) Teil, z. B. Zuschnitt, Härten.

**Bearbeitung zukaufen**
Eine Bearbeitung kann zugekauft werden, wenn sie nicht im Betrieb durchgeführt werden kann. Dies muss bei der Produktionsplanung berücksichtigt werden, weil dabei der Produktionsprozess unterbrochen wird.

**Bearbeitungstyp**
Bearbeitungen werden in verschiedene Bearbeitungstypen zusammengefasst, z. B. Zuschnitt, Säumen, Polieren. Sie wählen den Bearbeitungstyp aus, zu dem die aktuelle Bearbeitung gehört.
Für den Stufungsartikel (Produktart Modell, Produktgruppe Stufung) muss der Bearbeitungstyp 99999 - Pseudobearbeitung ausgewählt werden.

**Schichtlage**
Einige Bearbeitungen können bei beschichteten Gläsern nur auf einer Seite ausgeführt werden. Dazu geben Sie an, wo die Schichtseite liegt.

**Plantext**
Der Plantext für Gläser wird in A+W Production angezeigt. Plantexte können auch mehrfach nach Priorität (Prio 1 ist hoch, 10 ist niedrig) übernommen werden.

**Planpriorität**
Priorität für die Übernahme des Plantextes.

**Sequenz**
Reihenfolge der Bearbeitung. Die Ziffer entscheidet, wann die Bearbeitung ausgeführt wird. Zuschneiden hat dabei die Ziffer 1, denn das ist immer der erste Arbeitsschritt bei einem Glas.

**Zuschlagsgruppe**
Zur Bearbeitung gehörende Maßzuschlagsgruppe für Kantenbearbeitungen. Die Zuschlagsgruppen werden in A+W Production angelegt und verwaltet.

**Zulässiger Teiletyp**
Zurzeit nicht genutzt.

## Produktverwaltung – Anlagen/Klassifikatoren

**Stammdaten > Produkte > Artikel > Artikel > Register Anlagen/Klassifikatoren**

_Abb. B-385: Produktverwaltung – Anlagen/Klassifikatoren_

In diesem Register binden Sie externe Dateien ein, um weitere Informationen zum Produkt zur Verfügung zu stellen. Außerdem können Sie Klassifikatoren bearbeiten.

Die Felder im Bereich **Artikel** sind zum Register **Produkt** beschrieben.
⇨ "Produktverwaltung - Produkt" auf Seite B-600

In der Produktsuche und in der Auftragssuche kann nach den Klassifikatoren gesucht werden.

Die Klassifikatoren werden immer auf der Ebene des Hauptprodukts angelegt. Sie werden bei der Erfassung mit in die Stücklistenelemente übernommen.

> **Beispiel**
> Wenn für das Float 104 der Klassifikator Geeignet für ISO mit dem Wert Ja eingetragen ist, übernehmen alle Produkte, die in der Stückliste das Produkt 104 enthalten, diesen Klassifikator, wenn im Auftrag eine entsprechende Position erfasst wird.

⇨ "Partnerverwaltung - Klassifikatoren" auf Seite B-784
⇨ Tutorial 1, "Klassifikator anlegen" auf Seite B-76

### Klassifikatoren

In der Übersicht werden alle Klassifikatoren angezeigt, die für das Produkt vergeben werden können.
- **A (alphanumerisch):** Um einen Wert einzutragen, öffnen Sie den Dialog **Klassifikatoren Wertzuordnung** mit einem Doppelklick in das Feld **Wert**.
⇨ "Klassifikatoren Wertzuordnung" auf Seite B-810
- **N (numerisch):** Den Wert können Sie direkt in das Feld **Wert** schreiben.
- **D (Datum):** Den Wert können Sie direkt in das Feld **Wert** schreiben.

### Dateianhang

In dieses Feld ziehen Sie die externe Datei, die Sie im Windows-Explorer markiert haben. Damit wird eine Verknüpfung hergestellt.
Die verknüpften Dateien dürfen nicht in einen anderen Ordner verschoben werden.

**Bemerkung** In dieser Spalte können Sie eine Bemerkung zur verknüpften Datei eintragen oder auswählen, z. B. über den Inhalt.

### Leistungserklärung

Sie können dem Produkt eine Leistungserklärung zuweisen, die als Standard (Default) gesendet werden soll. Im Auftrag können Sie diese Leistungserklärung an der Position manuell überschreiben, z. B. nach einem Glasaustausch.

**Nummer** Nummer der Leistungserklärung.

**Leistungserklärung erforderlich** Für bestimmte Produkte kann eine Leistungserklärung erforderlich sein.
- [ ] Die Leistungserklärung muss nicht gesendet werden.
- [x] Die Leistungserklärung muss gesendet werden.

## Produktverwaltung – Sprossen

**Stammdaten > Produkte > Artikel > Artikel > Register Sprossen**

_Abb. B-386: Sprossenkonstruktion im ISO-Produkt_

In diesem Register erfassen Sie eine Sprossenkonstruktion. Das gewählte Sprossenschema wird als Grafik angezeigt, sobald Sie in den Bereichen Waagerechte, Senkrechte Sprossen eine Sprosse ausgewählt haben.

Eine ausführliche Beschreibung der Daten, die Sie in diesem Register erfassen können, finden Sie im Part Verkauf:
⇨ Verkauf, "Positionen - Sprossen" auf Seite C-504

## Technische Parameter

**Stammdaten > Produkte > Artikel > Artikel > Menü Funktionen > Gruppe Technische Parameter > Technische Parameter allgemein, Technische Parameter Isolierglas**

_Abb. B-387: Technische Parameter_

In diesem Dialog tragen Sie die technischen Werte für Glas-Produkte ein.

### Abweichender Glasaufbau

**1. Glas, 2. Glas, 3. Glas**
Bei einfachen Glas-Produkten bleiben diese Felder leer. Bei ISO-Produkten werden die jeweiligen Gläser eingetragen.

**SZR, Gas**
Technische Werte pro ISO-Tabelle und SZR.

**Bezeichnung**
Namen des Glasaufbaus.

### Technische Werte

Die nachfolgenden Feldbezeichnungen können Sie im Dialog Systemtexte an die Anforderungen in Ihrem Unternehmen anpassen (Systemtexte Nr. 111-118). Die Bezeichnungen gelten in den technischen Parametern in der Produktverwaltung und in der Produktsuche.
⇨ "Systemtexte" auf Seite B-1060

**Ug-Wert in W/qm**
Wärmedurchgangskoeffizient (Systemtext 110). Der Ug-Wert ist die zentrale Maßeinheit beim Ermitteln des Wärmeverlusts eines Bauteils. Die Maßeinheit ist W/m² K. Je kleiner der Ug-Wert desto größer ist die Wärmedämmung.

**Ug-Wert nach DIN 4108-4**
Wärmedurchlasswiderstand

**Lichtdurchlässigkeit in %**
Lichtdurchlässigkeit. Die Lichtdurchlässigkeit drückt den direkt durchgelassenen sichtbaren Strahlungsanteil im Bereich der Wellenlänge von 280 bis 380 nm bezogen auf die Hellempfindlichkeit des menschlichen Auges aus. Die Bezugsgröße 100 % ist eine unverglaste Maueröffnung.

**g-Wert in %**
Gesamtenergiedurchlassgrad %. Die Größe setzt sich zusammen aus direkter Sonnenenergietransmission und sekundärer Wärmeabgabe nach innen infolge langwelliger Strahlung und Konvektion. Der g-Wert ist die sekundäre Kenngröße nach dem k-Wert.

**b-Faktor**
Mittlerer Durchlassfaktor. Er stellt den mittleren Durchlassfaktor der Sonnenenergie dar, bezogen auf den Gesamtenergiedurchlassgrad einer 4-mm-Scheibe. Er ist für die Kühllastberechnung eines Gebäudes notwendig.

**Schalldämmmaß in dB**
Das Schalldämmmaß ist die kennzeichnende Wirkung beim Schallschutz.

**Dickentoleranz in mm**
Die Dicke kann bei Isolierglas um wenige Millimeter differieren. Geben Sie den entsprechenden Wert für diese Toleranz mm an.

**Größentoleranz mm (<200 cm), (>=200 cm)**
Die Größe kann bei Isolierglas um wenige Zentimeter differieren. Geben Sie den entsprechenden Wert für die Toleranz in cm an.

**(Kombobox)**
Sie können einen Aufschlag auf den Ug-Wert aktivieren, wenn in der ISO-Scheibe Sprossen eingebaut werden.
Zur Auswahl stehen folgende Einstellungen:
- **Keine Sprossen im SZR:** Auf den Ug-Wert wird kein Aufschlag berechnet.
- **Sprossen im SZR, einfach (+0.1):** Bei einem einfachen ISO mit Sprossen wird der Ug-Wert um 0,1 erhöht.
- **Sprossen im SZR, mehrfach (+0.2):** Bei mehrfachem ISO mit Sprossen wird der Ug-Wert um 0,2 erhöht.
Der Ug-Wert wird in der Auftragserfassung automatisch an die Sprossenanzahl angepasst.

## Technische Parameter kopieren

**Stammdaten > Produkte > Artikel > Artikel > Menü Funktionen > Gruppe Technische Parameter > Technische Parameter kopieren**

_Abb. B-388: Technische Parameter kopieren_

In diesem Dialog kopieren Sie die technischen Werte und übertragen diese auf ein anderes Produkt.

### Optionen

Mit der Wahl der Option legen Sie fest, wie bereits vorhandene Parameter im Ziel-Produkt behandelt werden:

- **Vorhandene Parameter im Ziel updaten:** Wenn im Ziel-Produkt bereits Parameter vorhanden sind, werden diese überschrieben. Zusätzliche Parameter aus dem Quell-Produkt werden übernommen.
- **Alle Parameter im Ziel zuvor löschen:** Die Parameter im Ziel-Produkt werden gelöscht. Danach werden die Parameter aus dem Quell-Produkt eingetragen.

## Produktänderung

**Stammdaten > Produkte > Artikel > Artikel > Menü Funktionen > Selektierte Produkte ändern**

_Abb. B-389: Zuordnung der automatischen Zuschläge ändern_

In diesem Dialog ändern Sie die Zuordnung der automatischen Zuschläge. Die Zuordnungen gelten immer für alle Produkte, die im Register Tabelle angezeigt werden.

### Zuschläge/Rabatte

In diesem Bereich werden die Zuschläge und (Sonder-)Rabatte angezeigt, die im Dialog **Produktzuordnung Zuschläge** angelegt sind.
⇨ "Produktzuordnung Zuschläge" auf Seite B-1043

Mit der Wahl der Option legen Sie fest, was mit den markierten Zuschlägen/Rabatten gemacht werden soll:
- **Setzen:** Die markierten Zuschläge oder Rabatte werden in den allen Produkten aktiviert, die in der Produktverwaltung ausgewählt sind.
- **Löschen:** Die markierten Zuschläge oder Rabatte werden in den allen Produkten deaktiviert, die in der Produktverwaltung ausgewählt sind.

## Produktkennzeichen Verwaltung

**Stammdaten > Produkte > Artikel > Artikel > Register Lager/Einkauf [Abweichende Produktkennzeichen]**

In diesem Dialog definieren Sie abweichende Beschaffungsarten, wenn Sie mit internen Aufträgen und Verrechnungen arbeiten. Dazu müssen die entsprechenden Mandanten und/oder AV-Bereiche angelegt sein.
⇨ "Firmendaten - Mandant" auf Seite B-931
⇨ "AV-Bereiche" auf Seite B-1033

In diesem Dialog finden Sie folgende Register:
- Produktkennzeichen Verwaltung - Editieren
- Produktkennzeichen Verwaltung – Kopieren

### Produktkennzeichen Verwaltung – Editieren

**Stammdaten > Produkte > Artikel > Artikel > Register Lager/Einkauf [Abweichende Produktkennzeichen] > Editieren**

_Abb. B-390: Produktkennzeichen Verwaltung - Editieren_

In diesem Register können Sie die Produktkennzeichen anlegen und bearbeiten.

#### Produkt

In dieser Gruppe werden die Produktnummer und die Bezeichnungen des aktuellen Produkts angezeigt.

#### Bereich, Kennzeichen

Sie können die Beschaffungsart für unterschiedliche Mandanten und/oder AV-Bereiche festlegen.

> **Beispiel**
> Die AV-Bereiche ISO, VSG und ESG arbeiten untereinander mit internen Aufträgen. Alle AV-Bereiche benutzen dieselbe Datenbank mit denselben Stammdaten usw.
> Im AV-Bereich ISO wird ein Kundenauftrag erfasst, in dem ein VSG mit ESG, ein SZR und ein Float die Komponenten einer ISO-Einheit bilden.
> - Für den AV-Bereich ISO ist das ISO Produktion, das VSG eine Bestellung, das Float aber Zuschnitt.
> - Für den AV-Bereich VSG ist das VSG Produktion, das ESG eine Bestellung, das Float ebenfalls Zuschnitt.
> - Für den AV-Bereich ESG ist das ESG Produktion, das Float ebenfalls Zuschnitt.
> Die unterschiedlichen Beschaffungsarten für VSG und ESG müssen daher als abweichende Produktkennzeichen definiert werden.

**Mandant**
Mandant, für den die abweichenden Kennzeichen gelten.

**AV-Bereich**
AV-Bereich, für den die abweichenden Kennzeichen gelten.

**Beschaffungsart**
Abweichende Beschaffungsart für den eingestellten Mandanten oder AV-Bereich.

**Lagerbuchungsart**
Abweichende Lagerbuchungsart für den eingestellten Mandanten oder AV-Bereich.

**Gültig in**
Mit der Wahl der Option legen Sie fest, wo die Einstellungen gelten sollen:
- **Sonstige:** Die Zuordnung beschränkt sich nicht auf die eine der beiden anderen Optionen.
- **Auftragserfassung:** Die Einstellungen gelten für die Auftragserfassung. Siehe dazu das Beispiel.
- **Profitcenter:** Die Suche nach dem Kennzeichen beschränkt sich auf einen Mandanten oder einen AV-Bereich. Dazu muss in den Firmendaten > Register Produktion die Profit-Center-Abrechnung aktiviert sein.
- **Suche über alles:** Die Option ist nur im Auswahl-Modus freigeschaltet. Die Suche wird mit dieser Option nicht weiter eingeschränkt.

#### Übersicht

In der Übersicht werden alle Produkte angezeigt, für die abweichende Kennzeichen angegeben sind.

### Produktkennzeichen Verwaltung – Kopieren

**Stammdaten > Produkte > Artikel > Artikel > Register Lager/Einkauf [Abweichende Produktkennzeichen] > Kopieren**

_Abb. B-391: Produktkennzeichen Verwaltung – Kopieren_

In diesem Register kopieren Sie die Einstellungen eines Produktes zu einer Warengruppe und/oder zu einer Folge von Produkten.

#### Quelle

In diesem Bereich werden die Daten des ausgewählten Produkts angezeigt. Die Felder sind zum Register **Editieren** beschrieben.
⇨ "Produktkennzeichen Verwaltung - Editieren" auf Seite B-641

#### Ziel

In diesem Bereich geben Sie an, worauf das Produktkennzeichen übertragen werden soll. Sie müssen mindestens eine Warengruppe oder eine Produktart angeben.

**Warengruppe**
Sie können eine WGR, WHG oder WOG auswählen.

**Produktart, Produktgruppe**
Wenn Sie eine Produktart ausgewählt haben, können Sie zusätzlich eine Produktgruppe angeben.

**Produkt von, bis**
Sie können ein einzelnes Produkt auswählen, indem Sie in beiden Feldern dieselbe Produktnummer angeben. Wenn Sie unterschiedliche Produktnummern angeben, wird das Produktkennzeichen auf alle Produkte zwischen der ersten und der zweiten Nummer übertragen.

**Mandat**
Mandant, auf dessen Produkte das abweichende Kennzeichen übertragen werden soll.

**AV-Bereich**
AV-Bereich, auf dessen Produkte das abweichende Kennzeichen übertragen werden soll.

Zusätzlich können Sie die Zuordnung zu wählen:
- **Sonstige:** Die Zuordnung beschränkt sich nicht auf die eine der beiden anderen Optionen.
- **Auftragserfassung:** Die Einstellungen gelten für die Auftragserfassung.
- **Profitcenter:** Die Einstellungen gelten für einen Mandanten oder einen AV-Bereich. Dazu muss in den Firmendaten > Register Produktion die Profit-Center-Abrechnung aktiviert sein.

## Glasarten

**Stammdaten > Produkte > Artikel > Artikel > Register A+W Production > Ordner [Glasart]**

_Abb. B-392: Glasarten_

In diesem Dialog tragen Sie alle relevanten Daten zur aktuellen Glasart ein. Die Glasarten können in folgenden Dialogen zugeordnet werden:
- **Produktverwaltung:** Wenn Sie einem Glasprodukt eine Glasart zuordnen, werden die Felder Produktart und Produktgruppe deaktiviert und können nicht mehr verändert werden.
  ⇨ "Produktverwaltung - A+W Production" auf Seite B-630
- **Glasart-Jumbo-Tische:** Jeder Glasart kann ein Schneidetisch zugeordnet werden, damit die Schnitte korrekt ausgeführt werden. Einem VSG muss z. B. der Tisch zugeordnet werden, der diese Glasart schneiden kann.
  ⇨ "Glasart-Jumbos-Tische" auf Seite B-885

### Werte

**Glasart**
Nummer der Glasart. In der Regel entspricht die Glasartnummer der A+W Business-Artikelnummer.

**Bezeichnung**
Name der Glasart.

**Produktgruppe**
Produktgruppe und Produktart, zu der die Glasart gehört.

**Glasartgruppe**
Glasartgruppe, zu der die Glasart gehört.

**Struktur**
Strukturverlauf der Glasart.

**Beschichtung**
Beschichtungsart der Glasart.

### Tabelle

In der Übersicht werden alle definierten Glasarten (aus A+W Enterprise) aufgelistet.

# Artikel

**Stammdaten > Produkte > Artikel**

In A+W Business können Sie Ihre firmeneigenen Produkte definieren und Daten für die Produktion hinterlegen.

Im Menü **Artikel** finden Sie zusätzlich zur Produktverwaltung folgende Einträge:
- "Lagermaße" auf Seite B-646
- "Maßzuschlag" auf Seite B-650
- "Produktvarianten" auf Seite B-652
- "EK-Kalkulation" auf Seite B-656
- "Abstandhalterrestriktionen" auf Seite B-658
- "Template Editor" auf Seite B-660
- "ISO-Aufbau" auf Seite B-661
- "Bearbeitungsrestriktionen" auf Seite B-663
- "Motive" auf Seite B-664
- "Modellkantenqualitäten" auf Seite B-665
- "Beschlagszuordnung" auf Seite B-666
- "¡TOE Regeln" auf Seite B-668

## Lagermaße

**Stammdaten > Produkte > Artikel > Lagermaße**

Sie können für die Preisfindung die Lagermaße anlegen. Diese Lagermaße sind unabhängig von den Lagerartikeln, die in der Lagerverwaltung gepflegt werden.

In diesem Kapitel finden Sie folgende Informationen:
- Menü Funktionen
- Lagermaße - Produkt
- Lagermaße - Tabelle

### Menü Funktionen

Über dieses Menü können Sie den Dialog **Lagerverwaltung** öffnen, um das ausgewählte Produkt auch als Lagermaß (Lagerartikel) für die Lagerverwaltung anzulegen.
⇨ Lagerwirtschaft, "Lagerverwaltung" auf Seite G-188

## Lagermaße – Produkt

**Stammdaten > Produkte > Artikel > Lagermaße > Register Produkt**

_Abb. B-393: Produktverwaltung Lagermaße – Produkte_

> **i**
> In diesem Register legen Sie die Lagermaße für die Preisfindung an. Sie können hier auch Lagermaße anlegen, die im Lager selbst nicht geführt werden. Sie können jedem Lagermaß einen Preisschlüssel VK und EK sowie eine Warengruppe zuordnen.
> **Lagerverwaltung**
> Die Lagermaße für die Lagerverwaltung werden im Dialog **Lagerverwaltung** (Modul Lagerwirtschaft) angelegt. Eine ausführliche Beschreibung der Lagermaße finden Sie im Part Lagerwirtschaft:
> ⇨ Lagerwirtschaft, "Lagermaße" auf Seite G-42
> ⇨ Lagerwirtschaft, "Lagerverwaltung" auf Seite G-68

### Artikel

In dieser Gruppe werden die Artikelnummer (Produktnummer) und die Bezeichnung zum aktuellen Produkt angezeigt.

### Einheiten / Restriktionen

**Inh./Breite/Höhe**
Für Kisten geben Sie die Anzahl der Blätter an, Breite und Höhe tragen Sie in mm ein.

**WGR, WGR-Statistik**
Jedem Lagermaß bzw. jeder Kiste können unterschiedliche Warengruppen zugeordnet werden.
⇨ Tutorial 1, "Warengruppen" auf Seite B-144

### Preis

**Preisschl. VK, Preisschl. EK**
Zur Auswahl werden alle Preisschlüssel für den Verkauf (VK) und den Einkauf (EK) angeboten, die in den Stammdaten für Preise hinterlegt sind. Für Kisten sollte ein eigener Preisschlüssel angelegt sein.

**EK Suche Lager**
Ein Produkt kann in die Ermittlung des durchschnittlichen Einkaufspreises einbezogen werden.
- [ ] Bei der Ermittlung des Durchschnittspreises wird das Produkt nicht berücksichtigt.
- [x] Bei der Ermittlung des Durchschnittspreises wird das Produkt mitberücksichtigt.
⇨ Lagerwirtschaft, "Einkaufspreis und Durchschnitts-EK" auf Seite G-52

### Bezeichnung

**Bezeichnung, Kurzbezeichnung**
Name und Kurzbezeichnung zur (besseren) Unterscheidung vom Bandmaß. Die Bezeichnungen werden in der Auftragserfassung angezeigt, z. B. Kiste Float 4 LM. Dies wird als Produktname im Formular gedruckt.

### Kennzeichen

**Beschaffungsart**
Die Beschaffungsart legt fest, wie das Produkt für den Auftrag beschafft wird.
- **Produktion:** Das Lagermaß wird produziert. Wenn ein Hauptartikel mit dieser Beschaffungsart gekennzeichnet ist, können dessen Stücklisten-Komponenten als Lagerartikel oder als Bestellartikel definiert werden.
  ⇨ Tutorial 1, "Beschaffungsart" auf Seite B-173
- **Zuschnitt:** Das Glas wird aus Lagerplatten zugeschnitten.
- **Lagerentnahme:** Das Produkt wird als Lagerartikel mit seinen genauen Abmessungen oder als Stückartikel im Lager geführt.
- **Bearbeitung:** Die Bearbeitungen für eine Auftragsposition werden an die Produktion übergeben.
- **Kundeneigenes Glas:** Das Produkt wird vom Kunden angeliefert und für die Produktion seiner Aufträge verwendet.
- **Bestellung:** Nur das betreffende Produkt wird bestellt, ohne den Inhalt der Stückliste zu beachten.
- **Bestellung (komplett):** Das Produkt wird inklusive aller Bearbeitungen bestellt.
- **Lagerzugang durch Produktion:** Das Produkt soll nur in Produktionsaufträgen verwendet werden, um das Lager zu füllen. Die produzierten Positionen werden dem Lager zugebucht.
  ⇨ Tutorial, "Produktionsaufträge" auf Seite E-130

Die Beschaffungsarten sind ausführlich zu den Produktstammdaten erklärt.
⇨ "Produktverwaltung - Lager/Einkauf" auf Seite B-617

### Fremdschlüssel Statistik

**Fremdschlüssel**
Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für statistische Auswertungen.

### Verfügbare Lagermaße

In der Übersicht werden alle Lagermaße zur aktuellen Produktnummer angezeigt. Diese Lagermaße werden zur Preisfindung herangezogen.

## Lagermaße – Tabelle

**Stammdaten > Produkte > Artikel > Lagermaße > Register Tabelle**

_Abb. B-394: Produktverwaltung Lagermaße – Tabelle_

In diesem Register werden alle Produkte angezeigt, die den Suchkriterien im Auswahlmodus entsprechen. Die Beschreibungen der Felder gelten für beide Register.
Die Felder sind ausführlich zum Register Produkt beschrieben.
⇨ "Lagermaße – Produkt" auf Seite B-647

## Maßzuschlag

**Stammdaten > Produkte > Artikel > Maßzuschlag**

Sie können Tabellen für maßabhängige Zuschläge anlegen und pro Tabelle verschiedene Zuschlagsstufen angeben.

Im Dialog **Maßzuschlag** finden Sie folgende Register:
- Maßzuschlag – Maßzuschläge
- Maßzuschlag - Tabelle

### Maßzuschlag – Maßzuschläge

**Stammdaten > Produkte > Artikel > Maßzuschlag > Register Maßzuschläge**

_Abb. B-395: Produktverwaltung Maßzugaben/Maßabzüge - Maßzuschläge_

In diesem Register legen Sie die Stufen für maßabhängige Zu- und Abschläge an.

Mit der Wahl der Option legen Sie fest, wie die Tabelle ausgewertet werden soll.
- **Zugabentabelle:** Eine Maßzugabe gleicht den Materialverlust aus, der bei einer Bearbeitung entsteht. Diese Zugabe wird beim Zuschnitt berücksichtigt.
- **Abzugstabelle:** Ein Maßabzug wird z. B. bei Bilderrahmen gebraucht.

> **Beispiel**
> Durch Polieren aller vier Kanten reduziert sich ein Float von 1000 x 1000 mm auf die Maße 998 x 998 mm.
> Als Maßzuschlag müssen 2 mm zugegeben werden. Dieser Wert wird der zugeordneten Tabelle entnommen, wobei die Dicke des Glases berücksichtigt wird.

Die Maßzuschläge werden in der **Produktverwaltung** bei den Produkten der Produktart **Bearbeitung** zugewiesen (nicht bei den Gläsern).
⇨ "Produktverwaltung - Fertigung" auf Seite B-605

#### Tabelle (Übersicht)

**Bis Dicke**
Pro Tabelle können Sie stufenweise angeben, bis zu welcher Dicke ein bestimmter Wert zugegeben werden soll.

**Wert**
Der Wert gibt den Zuschlag in mm an, der bei der entsprechenden Dicke zu- oder abgerechnet werden muss.

### Maßzuschlag – Tabelle

**Stammdaten > Produkte > Artikel > Maßzuschlag > Register Tabelle**

_Abb. B-396: Produktverwaltung Maßzugaben/Maßabzüge - Tabelle_

In diesem Register legen Sie neue Tabellen für maßabhängige Zu- oder Abschläge an.

## Produktvarianten

**Stammdaten > Produkte > Artikel > Produktvarianten**

**Zu Dialogbeschreibung:**
⇨ "Varianten kopieren" auf Seite B-655

Sie können Produktvarianten zu den Produkten anlegen, z. B. zu Abstandhaltern, Sprossen, Stückartikeln. Gläsern werden keine Farben zugeordnet. Die verschiedenen Glasfarben werden über unterschiedliche Produkte abgebildet.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Funktionen" auf Seite B-652
- "Produktvarianten - Varianten" auf Seite B-652
- "Produktvarianten - Tabelle" auf Seite B-654

### Menü Funktionen

Über dieses Menü öffnen Sie den Dialog **Varianten kopieren**, in dem Sie die Produktvarianten eines Produktes auf ein anderes Produkt übertragen.
⇨ "Varianten kopieren" auf Seite B-655

### Produktvarianten – Varianten

**Stammdaten > Produkte > Artikel > Produktvarianten > Register Varianten**

_Abb. B-397: Produktvarianten - Varianten_

In diesem Register legen Sie zu den Produkten aus der Produktverwaltung verschiedene Varianten an, z. B. andere Farben, unterschiedliche Polierungen oder Mattierungen usw. Jeder Produktvariante können Sie eine Preistabelle zuweisen.
⇨ Tutorial 1, "Produktvariante anlegen" auf Seite B-210

#### Produkt

**Nummer**
Produktnummer oder Spanne von Produktnummern, für die die Farbe gilt.

**EAN**
Der EAN-Code wird nur angezeigt, wenn ein einzelnes Produkt markiert ist.

**Bezeichnung**
Anzeige von Name und Beschreibung des Produkts.

**Produktart, Produktgruppe**
Anzeige der Produktart und der Produktgruppe, die dem Produkt zugewiesen sind.
⇨ "Produktverwaltung - Produkt" auf Seite B-600

#### Variante

**Nr./Variante**
Nummer und Bezeichnung der Variante aus dem Dialog **Varianten**.
⇨ "Varianten" auf Seite B-580

**Preistabelle**
Sie können pro Produkt und Variante unterschiedliche Preistabellen angeben.
⇨ "Preise" auf Seite B-725

**Gewicht**
Spezifisches Gewicht der Variante, wenn sich das Gewicht der Variante von dem des Produktes unterscheidet. In der Regel spielt das Gewicht für die Produkte mit Varianten keine Rolle und steht daher standardmäßig auf null.

**Default**
Wenn eine bestimmte Produktvariante häufig verlangt wird, kann sie in der Auftragserfassung standardmäßig zuerst angezeigt werden.
- [ ] Die Produktvariante wird nicht standardmäßig zuerst angezeigt.
- [x] Die Produktvariante wird automatisch zur Erfassung vorgeschlagen. Der Vorschlag kann in der Auftragserfassung überschrieben werden.

**Gesperrt**
Eine Variante kann für die Erfassung in der Produktverwaltung und in den Dokumenten gesperrt werden, wenn sie nicht mehr benötigt wird.
- [ ] Die Variante kann zugewiesen werden.
- [x] Die Variante ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie Produkten und in Dokumenten zugewiesen ist, wird sie jedoch weiterhin angezeigt.
⇨ Tutorial 1, "Sperren" auf Seite B-35

**WGR, WGR-Statistik**
Jeder Produktvariante können unterschiedliche Warengruppen zugeordnet werden.
⇨ Tutorial 1, "Warengruppen" auf Seite B-144

**Kennzeichen, Beschaffungsart**
Die Beschaffungsart der Produktvariante kann sich von derjenigen des Produkts unterscheiden.
⇨ Tutorial 1, "Beschaffungsart" auf Seite B-173

#### Abstandhalterkennzeichen

Bei Produkten der Produktgruppe **Abstandhalter** können Sie weitere Kennzeichen festlegen. Das Abstandhalterkennzeichen aus den Varianten übersteuert das Kennzeichen aus den Produktstammdaten.

**Frei**
Zurzeit nicht genutzt.

**Farbe**
Die Farbe wird von A+W Production vorgegeben.

#### Verfügbare Produktvarianten

In der Übersicht werden pro Produkt alle Varianten mit den zugeordneten Preistabellen aufgelistet.

### Produktvarianten – Tabelle

**Stammdaten > Produkte > Artikel > Produktvarianten > Register Tabelle**

_Abb. B-398: Produktvarianten - Tabelle_

In diesem Register werden alle Produktvarianten angezeigt, die den Suchkriterien im Auswahlmodus entsprechen.

Die Felder sind zum Register Varianten beschrieben.
⇨ "Produktvarianten - Varianten" auf Seite B-652

## Varianten kopieren

**Stammdaten > Produkte > Artikel > Produktvarianten > Menü Funktionen > Varianten kopieren**

_Abb. B-399: Produktvarianten kopieren_

In diesem Dialog übertragen Sie die Varianten eines Produktes auf ein anderes Produkt.

### Quelle, Ziel

In diesen Feldern geben Sie an, aus welchem Produkt die Varianten kopiert und auf welches diese übertragen werden sollen.

**Vorhandene Einträge überschreiben**
Wenn zu dem Ziel-Produkt bereits Varianten angelegt sind, müssen Sie entscheiden, ob Sie diese behalten oder überschreiben wollen.
- [ ] Die vorhandenen Varianten werden beibehalten und durch die neuen Varianten aus dem Quell-Produkt ergänzt. Gleiche Variantennummern werden nicht überschrieben.
- [x] Die Varianten im Ziel-Produkt werden mit den Varianten aus dem Quell-Produkt überschrieben. Zusätzliche Varianten werden hinzugefügt. Vorhandene Varianten werden nicht gelöscht.

## EK-Kalkulation

**Stammdaten > Produkte > Artikel > EK-Kalkulation**

_Abb. B-400: EK-Kalkulationsvorgaben - Stückliste_

In diesem Dialog hinterlegen Sie Vorgaben für Kalkulation der Eigenkosten für Isolierglas (ISO). Pro Abstandhalter (SZR) legen Sie den durchschnittlichen Verbrauch von Butyl, Thiokol, etc. fest.

Im Register **Stückliste** geben Sie die Werte für die EK-Kalkulation an.

### SZR - Artikel

**Artikel/MCode, Bezeichnung**
Nummer, Matchcode und Bezeichnung des Abstandhalters, zu dem die Eigenkalkulation durchgeführt wird.

**Rückschnitt (einfach)**
Rückschnitt für den Abstandhalter.

**Entspannte Menge für Gas**
Entspannte Menge für das Schallschutzgas lt. Herstellerangaben.

### Stücklistenprodukt

In diesem Bereich werden die Details zu den Produkten angezeigt, die mit dem SZR zusammen verbraucht werden.

**Produkt**
Nummer des Produktes.

**Bezeichnung, Mengeneinheit**
Anzeige der Bezeichnung und der Mengeneinheit, z. B. für Butyl.

**Verbrauch pro - Bezugseinheit**
Menge und Einheit, auf die sich die verbrauchte Menge bezieht.

> **Beispiel**
> Mengeneinheit (Butyl): kg
> Verbrauch: 0,0055
> Bezugseinheit: Lfm
> **Berechnung:** Pro Meter Abstandhalter werden 0,0055 kg Butyl verbraucht.

⇨ Tutorial 2, "Komplexbeispiel: Kalkulation ISO" auf Seite B-555

### Stückliste

In der Übersicht sind alle Produkte aufgeführt, die als Komponenten zu einem Abstandhalter hinzugefügt wurden. Daten werden nur angezeigt, wenn im Bereich Tabelle ein Abstandhalter markiert ist.

### Tabelle (Übersicht)

Übersicht über alle Produkte, die den Suchkriterien im Auswahlmodus entsprechen, bzw. für die ein bestimmter Verbrauch an Butyl, Trockenmittel, Randverbund usw. hinterlegt wurde.

## Abstandhalterrestriktionen

**Stammdaten > Produkte > Artikel > Abstandhalterrestriktionen**

_Abb. B-401: Abstandhalterrestriktionen_

In diesem Dialog hinterlegen Sie die Einschränkungen (Restriktionen) für bestimmte Abstandhalter. Bei TPS-Isolierglas (Thermo Plastic Spacer) können nicht alle Aufbauten ausgeführt werden, die für das herkömmliche ISO-Glas verwendet werden.

Wenn bei der Erfassung eines Auftrags die Restriktionen verletzt werden, muss auf ein anderes Produkt ausgewichen werden.

### Identifikation

**Produktgruppe**
In der Regel sind die Abstandhalterrestriktionen für TPS-ISO notwendig. Es können jedoch auch andere Produktgruppen ausgewählt werden.

**Passwort**
Wenn ein Passwort hinterlegt ist, kann die Restriktion im Auftrag überschrieben werden. In diesem Fall wird das Passwort bei der Erfassung des Auftrags abgefragt.
Ist kein Passwort hinterlegt, wird im Auftrag automatisch auf den Ausweichartikel zugegriffen, der in der Gruppe **Bei Verletzung des Gültigkeitsbereichs ausweichen auf** angegeben ist.

**Regel**
Die hinterlegten Regeln sind mit Variablen definiert, deren Werte aus den Feldern für Parameter gezogen werden. Dabei gilt [N1], [N2] und [N3] für die Parameter 1 bis 3.
Die Regeln sind fest hinterlegt. Wenn Sie zusätzliche Regeln brauchen, wenden Sie sich an Ihren Service-Mitarbeiter bei der A+W Software GmbH.

### Gültigkeitsbereich

**Parameter 1 - 3**
Felder für die Werte, die über Variablen in die Regel eingefügt werden. Die Felder werden entsprechend der ausgewählten Regel freigeschaltet. Wenn eine Regel ohne Variablen ausgewählt wurde, sind keine Felder freigeschaltet, z. B. bei Regel 3114 - Bei Modellen darf keine Sprosse vorhanden sein.
Bei bestimmten Regeln steht für Parameter 1 eine Kombobox zur Verfügung, aus der die entsprechende Einschränkung ausgewählt werden kann.

### Bei Verletzung des Gültigkeitsbereichs ausweichen auf

Wenn die gesetzten Parameter verletzt werden, kann auf ein Ausweichprodukt zugegriffen werden.

**Produktgruppe**
Auswahlliste der Produktgruppe, auf die ausgewichen werden kann, wenn die Restriktion verletzt wird.

**Variante**
Zusätzlich zur Produktgruppe kann auch eine Variante für den Ausweichartikel festgelegt werden.

### Restriktionen

Übersicht über die definierten Restriktionen mit den hinterlegten Parametern.

## Template Editor

**Stammdaten > Produkte > Artikel > Template Editor**

_Abb. B-402: Template Editor_

In diesem Dialog können Sie ein Template für die Modellerfassung auswählen. Mit dem Editor können Sie Vorlagen von A+W CAD Designer (Shapes) bearbeiten oder neue Vorlagen für die Bearbeitung erstellen.

### Verzeichnis

Sie können die Templates (Vorlagen) in verschiedenen Verzeichnissen verwalten. Das jeweils zuletzt genutzte wird automatisch angezeigt.

### Templates

Die Templates werden angezeigt, die im ausgewählten Verzeichnis gespeichert sind.

> **i Handbuch für A+W CAD Designer**
> Für die Arbeiten mit A+W CAD Designer stehen eine separate Online-Hilfe und ein separates Handbuch zur Verfügung.

## ISO-Aufbau

**Stammdaten > Produkte > Artikel > ISO-Aufbau**

_Abb. B-403: ISO Aufbau_

In diesem Dialog hinterlegen Sie Schlüsselnummern für einen eindeutigen Aufbau von ISO-Scheiben.

Die Nummern können in den Rahmentext gedruckt werden. Anhand dieser Schlüsselnummer kann der Aufbau einer fertig produzierten ISO-Einheit unabhängig vom zugehörigen Auftrag ermittelt werden.

Der Dialog ist nur freigeschaltet, wenn in den Firmendaten > Register Dokumente die Funktion **Gütekennzeichen** aktiviert ist.
⇨ "Produktkennzeichnung" auf Seite B-946

**Schlüsselnummer**
Schlüsselnummer, die für den entsprechenden ISO-Aufbau vergeben werden soll.

### Glasaufbau

**1. Glas, 2. Glas, 3. Glas**
Produktnummern der Gläser, aus denen das 2-fach bzw. 3-fach Isolierglas zusammengesetzt ist.

**SZR Dicke**
Breite des Abstandhalters.

**Gas**
Gastyp, wenn der Scheibenzwischenraum des Isolierglases mit Gas gefüllt ist.

> **i Feldbezeichnungen anpassen**
> Die nachfolgenden Feldbezeichnungen können Sie im Dialog **Systemtexte** an die Anforderungen in Ihrem Unternehmen anpassen (Systemtexte Nr. 111 - 118).
> ⇨ "Systemtexte" auf Seite B-1060

**Ug-Wert in W/m²**
Wärmedurchgangskoeffizient
Der Ug-Wert ist die zentrale Maßeinheit beim Ermitteln des Wärmeverlustes eines Bauteils. Die Maßeinheit ist W/m² K. Je kleiner der Ug-Wert desto größer ist die Wärmedämmung.

**g-Wert in %**
Gesamtenergiedurchlassgrad in %.
Die Größe setzt sich zusammen aus direkter Sonnenenergietransmission und sekundärer Wärmeabgabe nach innen infolge langwelliger Strahlung und Konvektion.
Der g-Wert ist die sekundäre Kenngröße nach dem k-Wert.

**b-Faktor**
Mittlerer Durchlassfaktor
Er stellt den mittleren Durchlassfaktor der Sonnenenergie dar, bezogen auf den Gesamtenergiedurchlassgrad einer 4-mm-Scheibe. Die ist für die Kühllastberechnung eines Gebäudes notwendig.

### Tabelle (Übersicht)

Übersicht über alle Datensätze für ISO-Aufbauten. Wenn Sie einen Datensatz markieren, werden die Felder im Bereich Glasaufbau gefüllt.

## Bearbeitungsrestriktionen

**Stammdaten > Produkte > Artikel > Bearbeitungsrestriktionen**

_Abb. B-404: Bearbeitungsrestriktionen_

In diesem Dialog legen Sie die Regeln fest, die für Bearbeitungen bei bestimmten Produktgruppen gelten sollen.

Wenn bei der Erfassung eines Auftrags die Restriktionen verletzt werden, wird eine Meldung ausgegeben, auf die der Mitarbeiter in geeigneter Weise reagieren muss.

### Zuweisung

**Produktgruppe**
In der Regel gelten Restriktionen für Bearbeitungen von ESG- oder VSG-Scheiben. Es können jedoch auch andere Produktgruppen ausgewählt werden.

**Glasdicke**
Glasdicke, für die die Restriktion gilt. Wenn für eine Produktgruppe abhängig von der Glasdicke unterschiedliche Restriktionen gelten, müssen Sie für jede Glasdicke eine entsprechende Regel hinterlegen.

**Regel**
Die hinterlegten Regeln sind mit Variablen definiert, deren Werte aus den Feldern für Parameter gezogen werden.
Dabei gilt [p1], [p2] bis [p5] für die Parameter 1 bis 5.

**Parameter 1 - 5**
Felder für die Werte, die über die Variable in die Regel eingefügt werden. Die Felder werden entsprechend der ausgewählten Regel freigeschaltet. Wenn eine Regel ohne Variablen ausgewählt wurde, sind keine Felder freigeschaltet, z. B. bei Regel 201 - Rest der Kante >= Ausschnitttiefe.

**Level**
Mit der Wahl der Option legen Sie fest, wie A+W Business bei einer Verletzung der Restriktionen reagieren soll:
- **Info:** In der Positionserfassung wird nur eine Information angezeigt.
- **Warnung:** In der Positionserfassung wird eine Warnung angezeigt. Der Anwender sollte dann die Details der Bearbeitung oder das Glas ändern.
- **Fehler:** In der Positionserfassung wird eine Fehlermeldung angezeigt. Die Bearbeitung und die Position können nicht gespeichert werden. Der Anwender muss dann die Details der Bearbeitung oder das Glas ändern.

### Restriktionen

Übersicht der definierten Restriktionen mit den hinterlegten Parametern.

## Motive

**Stammdaten > Produkte > Artikel > Motive**

_Abb. B-405: Motive_

In diesem Dialog legen Sie Motive für Beschichtungen, Siebdrucke, Sandstrahlen, Emaillierungen, Kolorieren und Mattierungen an. Die angelegten Motive können Sie im Auftrag in der Positionserfassung im Register **Modelle/Bearbeitungen** über die Siebnummer einfügen.
⇨ "Beschichtung, Mattierung, Siebdruck, Flächen-Emaillierung, Sandstrahlen, Kolorieren" auf Seite C-489

### Motiv

**Siebnummer**
Nummer des Siebs.

**Name**
Name des Motivs. Er sollte eindeutig und sprechend sein.

**Datei**
Pfad und Name der Motivdatei. Eine Vorschau des Motivs wird in dem Rahmen in der rechten oberen Ecke des Dialogs angezeigt.

**Max. Abmessungen**
Angabe der maximalen Breite und Höhe des Siebs in mm. Sie können Breite und Höhe des Motivs im Auftrag in der Positionserfassung im Register **Modelle/Bearbeitungen** bis zu dem angegebenen Maximalwert anpassen.

### Tabelle

Übersicht der definierten Motive mit den hinterlegten Parametern.

## Modellkantenqualitäten

**Stammdaten > Produkte > Artikel > Modellkantenqualitäten**

_Abb. B-406: Modellkantenqualitäten_

In diesem Dialog weisen Sie den einzelnen Kanten der verschiedenen Modelle bestimmte Kantenqualitäten zu.

### Selektion

**Produkt**
Nummer und Bezeichnung der Bearbeitungsart.

**Modell**
Nummer des Modells, dessen Kanten bearbeitet werden sollen. Standardmodelle verwenden die Modell-Nr. 1-99, das Modell für Stufen-Isolierglas hat die Nummer 999.

### Kantenqualitäten

**Segment 1 - 8**
Angabe der Kantenqualität pro Modellsegment. Die Felder sind je nach Kantenanzahl des Modells freigeschaltet. Die zugehörige Nummerierung der Segmente wird in der Grafik mit den roten Zahlen angezeigt.

### Tabelle

Übersicht der definierten Modelle mit den hinterlegten Parametern.

## Beschlagszuordnung

**Stammdaten > Produkte > Artikel > Beschlagszuordnung**

_Abb. B-407: Beschlagszuordnung_

In diesem Dialog legen Sie die Bearbeitungen fest, die für die Anbringung von Beschlägen an einer Glasscheibe notwendig sind. Wenn ein Beschlag im Auftrag in der Positionserfassung in die Stückliste eingefügt wird, werden die zugehörigen Bearbeitungen und Bearbeitungsparameter in die Stückliste übernommen. Wenn der Beschlag im Auftrag aus der Stückliste gelöscht oder geändert wird, werden auch die zugehörigen Bearbeitungen gelöscht oder geändert.

### Identifikation

**Beschlag**
Nummer und Bezeichnung des Beschlags.

**Anbringung**
Anbringungstyp des Beschlags.

**Priorität Anbringung**
Reihenfolge, in der Beschläge mit derselben Produktnummer angebracht werden sollen. Wenn Beschläge im Auftrag in der Positionserfassung mehrfach in die Stückliste eingefügt werden, werden die Bearbeitungszuordnungen nach Priorität geordnet, z. B. wird Türband oben mit der Prioritätsnummer 1 an erster Stelle angezeigt, Türband mitte mit der Nummer 2 an zweiter Stelle, usw.

**Bandseite**
Seite, an der das Band angebracht werden soll. Sie können zwischen Links, Rechts und Beide wählen.
- **Links:** Das Band wird links angebracht.
- **Rechts:** Das Band wird rechts angebracht.
- **Beide:** Das Band kann an beiden Seiten angebracht werden.

**Bearbeitung**
Anzeige der Bearbeitungsart. Im Bereich **Parameter** können Sie die Bearbeitungsparameter ändern.

**Austausch**
Austauschbeschlag, der optional angegeben werden kann. Als Austauschbeschlag können z. B. Beschläge gewählt werden, die unterschiedliche Produktnummern für eine andere Bandseite haben. Die Bezeichnung des Austauschbeschlags wird nach Eingabe der Produktnummer automatisch angezeigt.

### Bearbeitungen

Über die Schaltfläche [Einfügen] können Sie Bearbeitungen an der Glasscheibe hinzufügen, die bei der Anbringung des ausgewählten Beschlags nötig werden. Im Bereich **Parameter** können Sie die zugehörigen Bearbeitungsparameter anpassen. Über die Schaltfläche [Löschen] können Sie Bearbeitungen entfernen.

### Parameter

Die angezeigten Felder unterscheiden sich je nach der Bearbeitung, die Sie gewählt haben.
Die Parameter sind ausführlich im Part Verkauf beschrieben.
⇨ Verkauf, "Parameter" auf Seite C-480

> **i Formeln statt Werte**
> Sie können in den Bearbeitungsparametern statt Werten auch Formeln eintragen.
> **Beispiel**
> Sie können z. B. für eine Griffstange in den Parametern **Bohrung 1 [x/y]**, **Bohrung 2 [x/y]** auch Formeln eintragen.
> Falls Sie Formeln einsetzen wollen, wenden Sie sich an Ihren Service-Mitarbeiter bei der A+W Software GmbH.

### Beschläge

In der Übersicht werden alle angelegten Beschläge angezeigt, die den Suchkriterien entsprechen.

## ¡TOE Regeln

**Stammdaten > Produkte > Artikel > ¡TOE Regeln**

_Abb. B-408: ¡TOE Regeln_

In diesem Dialog legen Sie die Regeln für den Import von SN-Dateien mit Bearbeitungen (TOE = Technical Order Entry) fest. Jeder Bearbeitung aus dem A+W CAD Designer muss die entsprechende Bearbeitung in A+W Business zugeordnet werden.

> **i Voraussetzungen**
> Das linzenzpflichtige TOE-Modul setzt das Datenbanksystem Microsoft SQL Server 2016 voraus. Wenn Sie sich an die A+W Software GmbH, wenn Sie das Modul einsetzen wollen.

### SN-Bearbeitungen

In diesem Bereich wählen Sie die Bearbeitungen aus, die in A+W CAD Designer definiert sind.
Pro ausgewählter Bearbeitung werden zusätzliche Felder angezeigt, um die Zuordnungen zu präzisieren. Eine ausführliche Beschreibung der Parameter finden Sie im Part **Verkauf** zur Positionserfassung.
⇨ Verkauf, "Positionen - Bearbeitungen" auf Seite C-479

**Bearbeitungstyp**
Nummer und Bezeichnung des Bearbeitungstyps aus A+W CAD Designer.

**Prio**
Wenn Sie zu einem Bearbeitungstyp mehrere Zuordnungen anlegen, müssen Sie angeben, mit welcher Priorität das System die Angaben auswerten soll.

**Auf Produktart**
Die Regel kann auf eine Produktart eingeschränkt werden.
- [x] Die Regel für die ausgewählte Bearbeitung kann an allen Produktarten angebracht werden.
- [ ] Die Regel soll nur gelten, wenn die ausgewählte Bearbeitung an einem bestimmten Produkt angebracht wird.
Das Feld zur Auswahl der in A+W CAD Designer hinterlegten Produkte wird freigeschaltet.

**Formel**
Die Regel kann auf eine Bearbeitung eingeschränkt werden, die durch eine Formel berechnet wird.
- [x] Die Regel gilt für die ausgewählte Bearbeitung.
- [ ] Die Regel gilt für die ausgewählte Bearbeitung nur dann, wenn die Bearbeitung durch eine Formel berechnet wird.
Das Feld zur Auswahl der in A+W CAD Designer hinterlegten Formel wird freigeschaltet.

**Kantenqualität**
Die Regel kann auf eine Bearbeitung eingeschränkt werden, wenn verschiedene Kantenqualitäten erzeugt werden können.
- [x] Die ausgewählte Bearbeitung bezieht sich nicht auf verschiedene Kantenqualitäten.
- [ ] Die Regel gilt für die ausgewählte Bearbeitung nur dann, wenn die Bearbeitung eine bestimmte Kantenqualität erzeugt.
Das Feld zur Auswahl der in A+W CAD Designer hinterlegten Kantenqualitäten wird freigeschaltet.

### Wird zu Produkt

**Produkt**
Nummer und Bezeichnung der Bearbeitung in A+W Business, die zugeordnet wird.

### Regeln

In der Übersicht werden die definierten Regeln angezeigt.

# Preise

**Stammdaten > Preise**

Für die Preisfindung im Auftrag stehen Preislisten, Rabatte und Zu- und Abschläge zur Verfügung. In diesem Abschnitt werden die Dialoge zu den Preislisten und zu den Zu- und Abschlägen beschrieben.

Die Beschreibung zu den Rabatten finden Sie im Abschnitt **Marktpartner**.
⇨ "Rabattverwaltung (Kunden, Lieferanten)" auf Seite B-815

> **i Reihenfolge der Dialogbeschreibungen**
> Die Dialogbeschreibungen in diesem Kapitel richten sich nicht vollständig nach der Reihenfolge der Dialoge in der Software. Die Preisverwaltung ist aus Gründen der Lesbarkeit in einem separaten Kapitel beschrieben.

Im Menü **Preise** finden Sie folgende Dialoge:
- "Preisjahrgang" auf Seite B-671
- "Preisschlüssel" auf Seite B-672
- "Tarife" auf Seite B-673
- "Preisverwaltung" auf Seite B-723
- "Sonstige Zuschläge" auf Seite B-675
- "Austauschzuschläge" auf Seite B-677
- "Preisgruppen" auf Seite B-695
- "Preisgruppenzuordnung" auf Seite B-696
- “Gruppenzuschläge" auf Seite B-698
- "Mischkalkulation" auf Seite B-707
- "Modellbearbeitungszuschläge" auf Seite B-708
- "Preis- und Mengeneinheit" auf Seite B-711
- “Versicherungspreise" auf Seite B-713
- "Sprossenpreiselemente" auf Seite B-720

## Preisjahrgang

**Stammdaten > Preise > Jahrgang**

_Abb. B-409: Preisjahrgang_

In diesem Dialog legen Sie die Jahrgänge an. Ein Jahrgang fasst eine Sammlung von Preislisten zusammen. Die Preisjahrgänge werden in der A+W Business-Preisberechnung fest mit den Preisschlüsseln zu einem Tarif verknüpft.
⇨ Tutorial 1, "Preisjahrgang" auf Seite B-225
⇨ "Tarife" auf Seite B-673

Sie müssen angeben, welche Preisliste als Standard-Preisliste für die automatische Preisfindung herangezogen werden soll, indem Sie entsprechende Checkbox (Stn) markieren. Diese Einstellungen werden in die Tarife übernommen.

**Stn VK**
Die Spalten ISO, EFG, Bearb. und Modell gelten für den Verkauf.

**Stn EK**
Die Spalten EK, Bearb. und Modell gelten für den Einkauf.

**Von, bis**
Zeitraum, in dem die Preisliste gültig sein soll. Diese Angaben haben keinen Einfluss auf die Verfügbarkeit der jeweiligen Preisliste.

**Gesperrt**
Ein Jahrgang kann für die Erfassung in der Produktverwaltung und in den Dokumenten gesperrt werden, wenn er nicht mehr benötigt wird.
- [ ] Der Jahrgang kann zugewiesen werden.
- [x] Der Jahrgang ist gesperrt und kann nicht mehr zugewiesen werden. Wenn er Produkten und in Dokumenten zugewiesen ist, wird er jedoch weiterhin angezeigt.

**Bemerkungen**
Kommentare, z. B. zu Besonderheiten der Preisliste.

## Preisschlüssel

**Stammdaten > Preise > Schlüssel**

_Abb. B-410: Preisschlüssel_

In diesem Dialog legen Sie Preisschlüssel an. Ein Preisschlüssel wird immer an eine Jahrgangspreisliste gekoppelt und stellt ihre Unterteilung dar.

Die Kombination eines Preisschlüssels mit einer oder mehreren Jahrgangspreislisten ergibt die Tarife, die zur Preisberechnung herangezogen werden.
⇨ Tutorial 1, "Preisschlüssel" auf Seite B-226
⇨ "Tarife" auf Seite B-673

**Gesperrt**
Ein Preisschlüssel kann für die Erfassung in der Produktverwaltung und in den Dokumenten gesperrt werden, wenn er nicht mehr benötigt wird.
- [ ] Der Preisschlüssel kann zugewiesen werden.
- [x] Der Preisschlüssel ist gesperrt und kann nicht mehr zugewiesen werden. Wenn er Produkten und in Dokumenten zugewiesen ist, wird er jedoch weiterhin angezeigt.

## Tarife

**Stammdaten > Preise > Tarife**

_Abb. B-411: Tarifzuordnung_

In diesem Dialog definieren Sie, welcher Preisschlüssel mit welcher Preisliste zu einem Tarif kombiniert wird. Diese Kombination wird in der Auftrags- und Bestellungserfassung (Verkauf, Einkauf) übernommen und kann jeweils überschrieben werden.

Erst wenn die Tarife festgelegt worden sind, können Sie in der Preisverwaltung die Preise hinterlegen.
⇨ Tutorial 1, "Tarifdefinition" auf Seite B-226

### Preisjahrgang

In diesem Bereich wird angezeigt, welche Preisliste im Preisjahrgang als Standard-Preisliste definiert ist. Auch die Preisliste <k.A.> kann zur Tarifkombination verwendet werden. Sie kann auch zur Definition von Preisen verwendet werden.

### Preisschlüssel

In diesem Bereich werden die angelegten Preisschlüssel angezeigt. Auch der Preisschlüssel <k.A.> kann zur Tarifkombination verwendet werden.

### Tarifzuordnung

In diesem Bereich kombinieren Sie die Jahrgangspreisliste und den Preisschlüssel, um einen Tarif zu erstellen.

Im Preisjahrgang selbst ist nur definiert, welche der Preislisten zur Standard-Preisberechnung herangezogen wird, z. B. für alle Verkaufspreise (VK) und Einkaufspreise (EK) dieselbe Preisliste.

Für den Tarif wird angegeben, dass z. B. für den VK ISO die Preisliste 07 mit dem Preisschlüssel Hütte 06 gültig ist, aber für den VK EFG (Einfachglas) die Preisliste 07 mit dem Preisschlüssel Festmaß.

> **i Nur definierte Tarife stehen zur Preisberechnung zur Verfügung**
> Beachten Sie, dass Sie für jede Kombination von Preisjahrgang und Preisschlüssel, die Sie im Verkauf oder im Einkauf verwenden wollen, ein Tarif definiert werden muss. Dieser Tarif muss auch dann definiert werden, wenn er nicht als Standard verwendet werden soll.

Die markierten Checkboxen zeigen an, welcher Tarif als Standard für die Verkaufs- bzw. Einkaufspreisberechnung verwendet wird.

**ISO-Basistabelle**
Standardmäßig werden in A+W Business die ISO-Preise auf der Basis je einer ISO-Matrix für die Standard-Aufbauten berechnet, z. B. für ISO mit 2 x Float 4 mm, 2 x Float 6 mm, 2 x Float 8 mm.

Wenn Sie die Preise mit einer einzigen Matrix aufbauen und mit prozentualen Zu- und Abschlägen für die unterschiedlichen Glasdicken und Austauschgläser arbeiten, muss eine neue, sogenannte ISO-Basistabelle angelegt werden. Pro Tarif geben Sie die Nummer dieser ISO-Basistabelle an, damit die Preise nach diesem Muster berechnet werden.

**Herstellkostenkalkulation**
Wenn Sie mit dem Modul Herstellkostenkalkulation arbeiten, müssen Sie angeben, welcher der Tarife bei der Berechnung der Herstellkosten herangezogen werden soll.
- [ ] Der Tarif wird nicht zur Kostenkalkulation herangezogen.
- [x] Der Tarif wird zur Kalkulation der Herstellkosten herangezogen.

## Sonstige Zuschläge

**Stammdaten > Preise > Sonstige Zuschläge**

_Abb. B-412: Sonstige Zuschläge_

In diesem Dialog legen Sie Preiszuschläge an und bearbeiten diese. Diese Zuschläge sind von der Länge, der Fläche, dem Gewicht, dem SZR usw. abhängig. Dabei können Sie für die Staffelung zwei Grenztypen verwenden.
⇨ Tutorial 1, "Zuschläge" auf Seite B-273
⇨ Tutorial 1, "Sonstigen Zuschlag anlegen" auf Seite B-326

> **i Reihenfolge der Zuschlagsstufen beachten**
> Eine neue Stufe wird immer nach der letzten Stufe eingefügt. Die Reihenfolge der Stufen wird bei der Preisfindung nicht geändert oder analysiert. Das bedeutet, dass der Grenzwert 1200 mm dann nicht berücksichtigt wird, wenn er nach dem Grenzwert 1800 mm eingetragen ist. Für alle Größen unter 1800 mm wird dann derselbe Zuschlag berechnet.

Bei der Zuschlagsberechnung wird die Reihenfolge nur innerhalb der gleichen Zuschlagseinheit geprüft. Die Reihenfolge ist dann entscheidend und wird berücksichtigt, wenn eine Zuschlagseinheit, z. B. Brutto%, für mehrere unterschiedliche Grenztypen, z. B. kleinste Kantenlänge oder größte Kantenlänge, gilt.
- Zuschläge auf einzelne Elemente der Stücklisten werden früher berechnet als die Zuschläge, die von der Position auf die Stückliste wirken. Dies gilt auch umgekehrt: Zuschläge auf die Position werden früher berechnet als die Zuschläge, die aus der Stückliste heraus auf die Position wirken.
- Zuschläge auf qm, lfm und Stück werden vor Brutto-, Netto %-Zuschlägen berechnet. Hierbei ist entscheidend, worauf sie wirken: den Preis pro Preiseinheit, den Bruttopreis oder den Nettopreis.

Dabei muss außerdem die Zuschlagsart berücksichtigt werden. Bei **nicht additiver** Berechnung wird für die Berechnung des nachfolgenden Zuschlags der vorausgegangene Zuschlag nicht mit in die Berechnung einbezogen.

> **Beispiel**
> **Basispreis 100,00 €**
>
> | | additiv | nicht additiv |
> | :--- | :--- | :--- |
> | Modellzuschlag + 20 % | + 20,00 € | + 20,00 € |
> | **Zwischensumme** | **= 120,00 €** | |
> | Beschichtung + 25 % | + 30,00 € | + 25,00 € |
> | **Gesamtsumme** | **= 150,00 €** | **= 145,00 €** |

### Register Zuschlag

In diesem Register werden die Staffelungen des Zuschlags angezeigt, der im Register **Tabelle** markiert ist.

#### Zuschlag für

**Nummer**
Nummer der Zuschlagstabelle.

**Bezeichnung**
Name der Zuschlagstabelle.

**Grenztyp 1, 2**
Mit Hilfe der Grenztypen können Sie die Zuschläge staffeln. Der Grenztyp legt die Maßeinheit für die Staffelung fest. Sie können unterschiedliche Maßeinheiten für die beiden Grenztypen auswählen, z. B. Höhe und Breite.

**Bis Grenze 1, 2**
Wert der Staffelung. Der Grenzwert bezieht sich auf den Grenztyp. Ist als Grenztyp <k.A.> angegeben, gilt der Zuschlag pro Preiseinheit.

**ODER**
Wenn Sie zwei unterschiedliche Grenztypen für die Staffelung verwenden wollen, müssen Sie angeben, ob diese gemeinsam oder alternativ ausgewertet werden sollen.
- [x] Beide Grenzwerte und Grenztypen werden bei der Berechnung des Zuschlags berücksichtigt.
- [ ] Nur einer von beiden Grenzwerten/Grenztypen wird berücksichtigt.

> **Beispiel**
> In der Preisverwaltung haben Sie für ein Ornamentglas eine Matrix angelegt, bei der Höhe und Breite nicht vertauscht werden dürfen.
> Für die Berechnung eines Zuschlags auf die Kantenlängen soll es keine Rolle spielen, ob die Höhe oder die Breite den Grenzwert erreicht.
> Sie tragen als Grenzwert 1 und 2 die Stufe 1200 ein.
> Als Grenztyp 1 wählen Sie Höhe und als Grenztyp 2 Breite.
> - Wenn Sie die Checkbox ODER markieren, wird jeweils die Kante berücksichtigt, die als erste die Stufe 1200 mm erreicht.
> - Wenn Sie die Checkbox nicht markieren, wird der Zuschlag erst erhoben, wenn beide Kanten mindestens die Länge 1200 mm erreichen.

**Zuschlag, Einheit**
Höhe und Einheit des Zuschlags, z. B. 2,5 % des Bruttopreises.

**Zuschlagsart**
Die Zuschlagsart bestimmt, auf welcher Basis der Zuschlag berechnet werden soll.
⇨ Tutorial 1, "Berechnungen nach Zuschlagsarten" auf Seite B-319

**Gültig bei Preisvorgabe**
Im Auftrag kann der Preis manuell überschrieben werden. Dabei kann der Zuschlag wahlweise berechnet werden. Die Einstellung gilt für alle Aufträge und kann im Auftrag nicht geändert werden.
- [ ] Der Zuschlag wird nicht berechnet, wenn der Preis im Auftrag manuell überschrieben wird.
- [x] Der Zuschlag wird immer berechnet.

### Register Tabelle

In der Tabelle werden alle sonstigen Zuschläge aufgeführt, die den Auswahlkriterien entsprechen.

## Austauschzuschläge

**Stammdaten > Preise > Austauschzuschläge**

**Zu Dialogbeschreibung:**
⇨ Auswahl - Austauschzuschlag

Die Austauschzuschläge sind gruppenunabhängig und beziehen sich auf die Gläser, die nicht in Gruppen zusammengefasst werden können oder sollen. Sie können Produkt für Produkt definieren, welchen Zuschlag Sie hinzufügen möchten, wenn in einem ISO oder einem VSG ein Glas getauscht wird.

Im Dialog **Austauschzuschläge** finden Sie folgende Register:
- Austauschzuschläge – Tabelle
- Austauschzuschläge - Allgemein, nach Dicke, nach Produkt
- Austauschzuschläge – Kunden-, Lieferantenpreise
⇨ Tutorial 1, "Austauschzuschläge" auf Seite B-295

### Menü Funktionen

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen**

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Dialog Austauschzuschläge zu schließen.

Das Menü ist in folgende Gruppen gegliedert:
- Gruppe Kopieren
- Gruppe Löschen
- Gruppe Ändern

#### Gruppe Kopieren

- **Allgemein:** Öffnet den Dialog **Austauschpreise kopieren allgemein**, um die Preise für Eintauschgläser zu kopieren.
  ⇨ "Austauschpreise kopieren" auf Seite B-684
- **Pro Austauschartikel komplett:** Öffnet den Dialog **Preise pro Austauschartikel komplett kopieren**, um die Preise für Austauschgläser zu kopieren.
  ⇨ "Preise pro Austauschartikel komplett kopieren" auf Seite B-688

#### Gruppe Löschen

- **Preise löschen:** Öffnet den Dialog **Austauschpreise löschen**, um einen Austauschzuschlag zu löschen.
  ⇨ "Austauschpreise löschen" auf Seite B-691

#### Gruppe Ändern

- **Preise ändern:** Öffnet den Dialog **Preise ändern**, um einen Austauschzuschlag zu ändern.
  ⇨ "Austauschpreise ändern" auf Seite B-692

### Austauschzuschläge – Tabelle

**Stammdaten > Preise > Austauschzuschläge > Register Tabelle**

_Abb. B-413: Austauschzuschläge – Tabelle_

In diesem Register prüfen Sie, welche Austauschzuschläge angelegt sind.
⇨ Tutorial 1, "Austauschzuschläge" auf Seite B-295
⇨ Tutorial 1, "Austauschzuschlag anlegen" auf Seite B-299

#### Identifikation - Tarif

**Tabelle**
In der Regel wird nur eine Tabelle (Nr. 0) angelegt. Wenn Sie unterschiedliche Tabellen für Austauschzuschläge anlegen, können Sie diese in den Produktstammdaten zuweisen.
⇨ "Tab. Austauschzuschl." auf Seite B-613

**Jahrgang, Schlüssel**
Preisjahrgang und Schlüssel (VK-Tarif), denen der Austauschzuschlag zugeordnet ist.

**ISO, VSG**
Produktart, bei der der Zuschlag erhoben wird. Nur in ISO oder VSG können Gläser ausgetauscht werden. Dabei spielt es keine Rolle, an welcher Stelle das Glas getauscht wird, also z. B. in einem Mehrfach-ISO das zweite oder dritte Glas.

#### Produkt

**Eintausch**
Stücklisten-Komponente, die eingebaut wird.

**Austausch**
Stücklisten-Komponente, die ausgebaut, also ersetzt wird. Das Feld wird bei einem allgemeinen und bei einem produktbezogenen Austauschzuschlag angezeigt.

**Dicke Austausch**
Dicke der Stücklisten-Komponente, die ausgebaut, also ersetzt wird. Dabei spielt es keine Rolle, zu welcher Produktart oder -gruppe das Glas gehört.
Das Feld wird bei einem dickenabhängigen Austauschzuschlag angezeigt.

#### Austauschpreise

Der Zuschlag kann in max. drei Stufen gestaffelt werden. Die Grenztypen werden dem Produkt entsprechend im Register **Allgemein** vorgegeben.

Die Grenzwerte der höchsten Stufe werden automatisch aus den Feldern der zweiten Stufe übernommen. Das bedeutet, dass nur noch der Zuschlagswert eingetragen werden kann. Dieser wird immer dann berechnet, wenn die Scheibe größer als die zweite Stufe.

**Zuschlag**
Zuschlagswert pro Stufe. Der Wert wird je nach Zuschlagstyp als prozentualer Zuschlag oder als Betrag interpretiert.
⇨ "Zuschlagstypen" auf Seite B-681

#### Austausch-Tabelle

In der Übersicht sind alle Zuschläge aufgeführt, die den Auswahlkriterien entsprechen.
- **Produkt, Nummer:** Produktnummer des Eintauschprodukts, z. B. Glas, Gießharz.
- **Eintausch:** Bezeichnung des Eintauschprodukts.
- **Austausch:** Bezeichnung des Austauschs, also Produkt oder Dicke.
- **Tab.:** Nummer der Austauschtabelle, in der Regel Nummer 0.
- **Schlüssel:** Preisschlüssel, dem der Zuschlag zugeordnet ist.
- **Tarif:** Preisliste, dem der Zuschlag zugeordnet ist.

### Austauschzuschläge – Allgemein, nach Dicke, nach Produkt

**Stammdaten > Preise > Austauschzuschläge > Register Allgemein, nach Dicke, nach Produkt**

_Abb. B-414: Austauschzuschläge – Allgemein_

In den Registern **Allgemein**, **nach Dicke** und **nach Produkt** legen Sie Austauschzuschläge für ISO- oder VSG-Scheiben an. Die Zuschläge beziehen sich immer auf Tarife für Verkaufspreise (VK).
⇨ Tutorial 1, "Austauschzuschläge" auf Seite B-295

Die Felder in den Bereichen **Identifikation - Tarif**, **Produkt** und **Austauschpreise** sind zum Register **Tabelle** erklärt.
⇨ "Austauschzuschläge - Tabelle" auf Seite B-679

#### Zuschlagstypen

Der Zuschlagstyp gibt an, wie der Wert im Feld **Zuschlag** interpretiert werden soll, z. B. als prozentualen Aufschlag auf den Preis, als Betrag pro Länge usw.

#### Sonstige Zuschläge

**Nummer, Tabelle**
Sie können zusätzlich zum Austauschzuschlag einen Sonstigen Zuschlag erheben, z. B. für Zuschnittskosten. Die Sonstigen Zuschläge werden im gleichnamigen Dialog angelegt:
⇨ "Sonstige Zuschläge" auf Seite B-675

#### Grenzmengentyp

Mit der Wahl der Option legen Sie fest, welche Grenztypen im Bereich **Austauschpreise** verwendet werden.
- **Breite x Höhe:** Die Grenztypen Breite und Höhe werden angezeigt.
- **Fläche tatsächlich:** Der Grenztyp qm (Quadratmeter) wird angezeigt. Als Fläche wird dabei die Fläche aus dem Auftrag herangezogen.
- **Kantenmaß:** Der Grenztyp Kante wird angezeigt.
- **Fläche gerundet:** Der Grenztyp qm (Quadratmeter) wird angezeigt. Für die Berechnung der Fläche werden dabei die Rundungen aus dem Auftrag und aus den Produktdaten herangezogen, in Deutschland meistens der Wert 30.
  ⇨ "Maßrundung Breite / Höhe" auf Seite B-615

#### Abw. Maßrundung

Sie können zur Berechnung der Fläche eine abweichende Maßrundung eingeben.

**Breite, Höhe**
Standardmäßig ist der Wert 0 eingetragen. Bei dieser Einstellung werden die Werte aus den Produktdaten übernommen.

#### Mindestangaben

Sie können Mindestwerte für die Berechnung des Zuschlags eingeben. Diese werden immer dann herangezogen, wenn die Werte im Auftrag darunterliegen.

**Mindestfläche**
Wenn Sie eine Mindestfläche für ein Eintauschglas angeben, wird diese Fläche in all den Fällen als Zuschlagsbasis herangezogen, in denen die Fläche im Auftrag kleiner ist.

**Preis brutto, netto**
Wenn Sie einen Mindestpreis angeben, wird dieser immer dann als Basis für den Zuschlag herangezogen, wenn der tatsächliche Preis des Eintauschproduktes darunterliegt.

### Austauschzuschläge – Kunden-, Lieferantenpreise

**Stammdaten > Preise > Austauschzuschläge > Register Kundenpreise, Lieferantenpreise**

_Abb. B-415: Austauschzuschläge – Kundenpreise_

In den Registern **Kundenpreise** und **Lieferantenpreise** legen Sie Austauschzuschläge an, die bei bestimmten Kunden oder Lieferanten berechnet werden sollen.
⇨ Tutorial 1, "Austauschzuschläge" auf Seite B-295

Die Felder im Bereich **Identifikation - Tarif** sind zum Register **Tabelle** erklärt.
⇨ "Austauschzuschläge - Tabelle" auf Seite B-679

#### Auswahl Kunden/Kundengruppe, Lieferanten/Lieferantengruppe

Mit der Wahl der Option legen Sie fest, für wen der Zuschlag gilt:
- **Allgemein:** Allgemeiner Zuschlag, der unabhängig von Marktpartnern oder Partner- gruppen berechnet wird (Standard-Austauschzuschlag).
- **Kundengruppe, Lieferantengruppe:** Zuschlag für die ausgewählte Gruppe von Kunden oder Lieferanten
- **Kunde, Lieferant:** Zuschlag für den ausgewählten Kunden oder Lieferanten

#### Objektauswahl

Der Zuschlag kann sich auf ein bestimmtes Objekt beziehen. Zur Auswahl werden alle Objekte angeboten.

#### Übersicht nach Kunden/Kundengruppen, Lieferanten/Lieferantengruppen

In der Übersicht werden alle Zuschläge angezeigt, die den Auswahlkriterien entsprechen.

### Auswahl – Austauschzuschlag

**Stammdaten > Preise > Austauschzuschläge > Menü Bearbeiten > Neu**

_Abb. B-416: Auswahl der Zuschlagsart_

In diesem Dialog wählen Sie die Art des Zuschlags, den Sie anlegen wollen.

## Austauschpreise kopieren

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Gruppe Kopieren > Allgemein**

Sie können einzelne oder mehrere Austauschzuschläge für Einbaugläser gemeinsam kopieren oder ändern.

In diesem Dialog finden Sie folgende Register:
- "Austauschpreise kopieren – Quelle, Ziel" auf Seite B-685
- "Austauschpreise kopieren – Preisänderung" auf Seite B-687

### Austauschpreise kopieren – Quelle, Ziel

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Gruppe Kopieren > Allgemein > Register Quelle**

_Abb. B-417: Austauschpreise kopieren 1 – Quelle, Ziel_

In den Registern kopieren Sie die Zuschläge einer Tabelle in eine andere Tabelle oder in einen anderen Tarif. Nur die Austauschzuschläge werden kopiert, die für Einbaugläser erhoben werden.
⇨ Tutorial 1, "Austauschzuschlag kopieren und ändern" auf Seite B-304

Wenn Sie die Zuschläge nur ändern wollen, geben als Quelle und Ziel dieselben Tabellen an. Im Register **Preisänderung** können Sie dann die Werte für die Änderung eintragen.
⇨ "Austauschpreise kopieren - Preisänderung" auf Seite B-687

#### Kopieren von, Kopieren nach

**Tabelle**
Nummer der Austauschtabelle.

**Eintauschnummer von, bis**
Nummern der Produkte, die eingebaut werden.

**Jahrgang, Schlüssel**
Preisjahrgang und Schlüssel (Tarif), denen der Austauschzuschlag zugeordnet ist.

**ISO, VSG, Beides**
Produktart, bei der der Zuschlag erhoben wird. Nur in ISO oder VSG können Gläser ausgetauscht werden. Dabei spielt es keine Rolle, an welcher Stelle das Glas getauscht wird, also in einem Mehrfach-ISO das zweite oder dritte Glas.
Mit der Option **Beides** werden die Austauschpreise für ISO und VSG kopiert.

**Preise überschreiben**
Wenn Sie die Zuschläge in eine gefüllte Tabelle übertragen wollen, müssen Sie entscheiden, ob die Zuschläge in der Ziel-Tabelle überschrieben werden sollen.
- [ ] Die Zuschläge der Ziel-Tabelle werden nicht überschrieben. Die zusätzlichen Zuschläge aus der Quell-Tabelle werden hinzugefügt.
- [x] Alle vorhandenen Zuschläge in der Ziel-Tabelle werden überschrieben.

**Preisart**
Mit der Wahl der Option legen Sie fest, für wen die Zuschläge gelten sollen:
- **Allgemein:** Allgemeiner Zuschlag, der unabhängig von Marktpartnern oder Partner- gruppen berechnet wird (Standard-Austauschzuschlag).
- **Kundengruppe, Lieferantengruppe:** Zuschlag für die ausgewählte Gruppe von Kunden oder Lieferanten
- **Kunde, Lieferant:** Zuschlag für den ausgewählten Kunden oder Lieferanten

**Objekt**
Das Feld ist gesperrt, wenn Sie die Option **Allgemein** gewählt haben. Bei der Auswahl einer Gruppe oder eines Partners können Sie zusätzlich angeben, für welches Objekt die Zuschlagstabelle geändert werden soll.

### Austauschpreise kopieren – Preisänderung

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Gruppe Kopieren > Allgemein > Register Preisänderung**

_Abb. B-418: Austauschpreise kopieren – Preisänderung_

In diesem Register geben Sie die Details für die Änderung an.
Wenn Sie als Quelle und Ziel dieselben Tabellen angegeben haben, werden die Zuschläge geändert, ohne sie in andere Tabellen zu kopieren.
Die Felder in den Bereichen **Kopieren von** und **Kopieren nach** sind zum Register **Quelle** beschrieben.
⇨ "Austauschpreise kopieren - Quelle, Ziel" auf Seite B-685

**Aufschlag, Abschlag**
Mit der Wahl der Option legen Sie fest, ob der eingegebene Wert auf die Zuschläge der Tabellen auf- oder abgeschlagen werden soll.

**Rundung**
Sie können die Rundung für die ausgewählte Tabelle ändern.

**Prozent, Absolut**
Wenn die Zuschläge selbst geändert werden sollen, geben Sie einen prozentualen oder absoluten Wert an.

## Preise pro Austauschartikel komplett kopieren

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Gruppe Kopieren > Pro Austauschartikel komplett**

Sie können einzelne oder mehrere Austauschzuschläge für Ausbaugläser gemeinsam kopieren oder ändern.

In diesem Dialog finden Sie folgende Register:
- "Preise pro Austauschartikel komplett kopieren – Quelle, Ziel" auf Seite B-688
- "Preise pro Austauschartikel komplett kopieren – Preisänderung" auf Seite B-690

### Preise pro Austauschartikel komplett kopieren – Quelle, Ziel

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Gruppe Kopieren > Pro Austauschartikel komplett > Register Quelle**

_Abb. B-419: Austauschpreise komplett Kopieren – Quelle_

In diesem Dialog kopieren Sie die Zuschläge einer Tabelle in eine andere Tabelle oder in einen anderen Tarif. Nur die Austauschzuschläge werden kopiert, die für Ausbaugläser erhoben werden.
⇨ Tutorial 1, "Austauschzuschlag kopieren und ändern" auf Seite B-304

Wenn Sie die Zuschläge nur ändern wollen, geben als Quelle und Ziel dieselben Tabellen an. Im Register **Preisänderung** können Sie dann die Werte für die Änderung eintragen.
⇨ "Preise pro Austauschartikel komplett kopieren – Preisänderung" auf Seite B-690

#### Kopieren von, Kopieren nach

**Tabelle**
Nummer der Austauschtabelle.

**Austausch**
Nummer des Produkts, das aus der Einheit entfernt wird.

**Jahrgang, Schlüssel**
Preisjahrgang und Schlüssel (Tarif), denen der Austauschzuschlag zugeordnet ist.

**ISO, VSG, Beides**
Produktart, bei der der Zuschlag erhoben wird. Nur in ISO oder VSG können Gläser ausgetauscht werden. Dabei spielt es keine Rolle, an welcher Stelle das Glas getauscht wird, also in einem Mehrfach-ISO das zweite oder dritte Glas.
Mit der Option **Beides** werden die Austauschpreise für ISO und VSG kopiert.

**Preise überschreiben**
Wenn Sie die Zuschläge in eine gefüllte Tabelle übertragen wollen, müssen Sie entscheiden, ob die Zuschläge in der Ziel-Tabelle überschrieben werden sollen.
- [ ] Die Zuschläge der Ziel-Tabelle werden nicht überschrieben. Die zusätzlichen Zuschläge aus der Quell-Tabelle werden hinzugefügt.
- [x] Alle vorhandenen Zuschläge in der Ziel-Tabelle werden überschrieben.

**Preisart**
Mit der Wahl der Option legen Sie fest, für wen die Zuschläge gelten sollen:
- **Allgemein:** Allgemeiner Zuschlag, der unabhängig von Marktpartnern oder Partner- gruppen berechnet wird (Standard-Austauschzuschlag).
- **Kundengruppe, Lieferantengruppe:** Zuschlag für die ausgewählte Gruppe von Kunden oder Lieferanten
- **Kunde, Lieferant:** Zuschlag für den ausgewählten Kunden oder Lieferanten

**Objekt**
Das Feld ist gesperrt, wenn Sie die Option **Allgemein** gewählt haben. Bei der Auswahl einer Gruppe oder eines Partners können Sie zusätzlich angeben, für welches Objekt die Zuschlagstabelle geändert werden soll.

### Preise pro Austauschartikel komplett kopieren – Preisänderung

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Gruppe Kopieren > Pro Austauschartikel komplett > Register Preisänderung**

_Abb. B-420: Austauschpreise komplett kopieren – Preisänderung_

In diesem Register geben Sie die Details für die Änderung an.
Wenn Sie als Quelle und Ziel dieselben Tabellen angegeben haben, werden die Zuschläge geändert, ohne sie in andere Tabellen zu kopieren.
Die Felder in den Bereichen **Kopieren von** und **Kopieren nach** sind zum Register **Quelle** beschrieben.
⇨ "Preise pro Austauschartikel komplett kopieren - Quelle, Ziel" auf Seite B-688

**Aufschlag, Abschlag**
Mit der Wahl der Option legen Sie fest, ob der eingegebene Wert auf die Zuschläge der Tabellen auf- oder abgeschlagen werden soll.

**Rundung**
Sie können die Rundung für die ausgewählte Tabelle ändern.

**Prozent, Absolut**
Wenn die Zuschläge selbst geändert werden sollen, geben Sie einen prozentualen oder absoluten Wert an.

## Austauschpreise löschen

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Preise löschen**

_Abb. B-421: Austauschzuschläge löschen_

In diesem Dialog löschen Sie Austauschzuschläge einzeln oder eine Folge von Austauschzuschlägen.

### Preisart

Mit der Wahl der Option legen Sie fest, für wen der Zuschlag gilt, den Sie löschen wollen:
- **Allgemein:** Allgemeiner Zuschlag, der unabhängig von Marktpartnern oder Partner- gruppen berechnet wird (Standard-Austauschzuschlag).
- **Kundengruppe, Lieferantengruppe:** Zuschlag für die ausgewählte Gruppe von Kunden oder Lieferanten
- **Kunde, Lieferant:** Zuschlag für den ausgewählten Kunden oder Lieferanten

### Objekt

Der Zuschlag kann sich auf ein bestimmtes Objekt beziehen. Zur Auswahl werden alle Objekte angeboten. Das Feld ist gesperrt, wenn Sie die Option **Allgemein** gewählt haben.

### Preisauswahl

**Tabelle**
Nummer der Austauschtabelle, die gelöscht werden soll.

**ISO, VSG, Beides**
Produktart, bei der der Zuschlag erhoben wird. Mit der Option **Beides** werden die Austauschpreise für ISO und VSG gelöscht.

**Eintausch von, bis**
Produktnummern der Eintauschgläser, zu denen der Austauschzuschlag definiert ist.

**Anzahl**
Anzahl der Datensätze, die gelöscht werden.

**Jahrgang, Schlüssel**
Preisjahrgang und Schlüssel (Tarif), denen der Austauschzuschlag zugeordnet ist.

## Austauschpreise ändern

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Preise ändern**

Sie können einzelne oder mehrere Austauschzuschläge gemeinsam ändern.

In diesem Dialog finden Sie folgende Register:
- "Austauschpreise ändern – Preisart" auf Seite B-692
- "Austauschpreise ändern – Preisänderung" auf Seite B-694

### Austauschpreise ändern – Preisart

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Preise ändern > Register Preisart**

_Abb. B-422: Austauschpreise ändern – Register Preisart_

In diesem Register wählen Sie die Austauschzuschläge aus, die Sie ändern wollen.
⇨ Tutorial 1, "Austauschzuschlag kopieren und ändern" auf Seite B-304

#### Preisauswahl

**Tabelle**
Nummer der Austauschtabelle, deren Preise geändert werden.

**Anzahl**
Anzahl der Datensätze.

**Nummer von, bis**
Nummern der Datensätze, die geändert werden.

**Jahrgang, Schlüssel**
Preisjahrgang und Schlüssel (Tarif), denen der Austauschzuschlag zugeordnet ist.

**ISO, VSG, Beides**
Produktart, bei der der Zuschlag erhoben wird. Nur in ISO oder VSG können Gläser ausgetauscht werden. Dabei spielt es keine Rolle, an welcher Stelle das Glas getauscht wird, also in einem Mehrfach-ISO das zweite oder dritte Glas.
Mit der Option **Beides** werden die Austauschpreise für ISO und VSG geändert.

#### Preisart

Mit der Wahl der Option legen Sie fest, für wen der Zuschlag gilt, den Sie ändern wollen:
- **Allgemein:** Allgemeiner Zuschlag, der unabhängig von Marktpartnern oder Partner- gruppen berechnet wird (Standard-Austauschzuschlag).
- **Kundengruppe, Lieferantengruppe:** Zuschlag für die ausgewählte Gruppe von Kunden oder Lieferanten
- **Kunde, Lieferant:** Zuschlag für den ausgewählten Kunden oder Lieferanten

**Objekt**
Das Feld ist gesperrt, wenn Sie die Option **Allgemein** gewählt haben. Bei der Auswahl einer Gruppe oder eines Partners können Sie zusätzlich angeben, für welches Objekt die Zuschläge geändert werden sollen.

### Austauschpreise ändern – Preisänderung

**Stammdaten > Preise > Austauschzuschläge > Menü Funktionen > Preise ändern > Register Preisänderung**

_Abb. B-423: Austauschpreise ändern – Register Preisänderung_

In diesem Register geben Sie die Details für die Änderung an.
Die Felder im Bereich **Preisauswahl** sind zum Register **Preisart** beschrieben.
⇨ "Austauschpreise ändern - Preisart" auf Seite B-692

**Aufschlag, Abschlag**
Mit der Wahl der Option legen Sie fest, ob der eingegebene Wert auf die Zuschläge der Tabellen auf- oder abgeschlagen werden soll.

**Rundung**
Sie können die Rundung für die ausgewählten Zuschläge ändern.

**Prozent, Absolut**
Wenn die Zuschläge selbst geändert werden sollen, geben Sie einen prozentualen oder absoluten Wert an.

## Preisgruppen

**Stammdaten > Preise > Preisgruppen**

_Abb. B-424: Preisgruppen_

In diesem Dialog hinterlegen Sie Preisgruppen. Die Preisgruppen verwenden Sie für die Berechnung von Preisen für Ornamentgläser und von Austauschzuschlägen, damit Sie nicht für jedes Produkt eine eigene Preistabelle pflegen müssen.

Die Produkte ordnen Sie den Preisgruppen im Dialog **Preisgruppenzuordnung** zu.
⇨ “Preisgruppenzuordnung" auf Seite B-696

**Bezeichnung**
In der Regel sind die Preisgruppen alphabetisch nummeriert.

**Bemerkung**
Ergänzende Bemerkung, z. B. zur Verwendung der Preisgruppe.

## Preisgruppenzuordnung

**Stammdaten > Preise > Preisgruppenzuordnung**

_Abb. B-425: Preisgruppenzuordnung_

In diesem Dialog ordnen Sie den Produkten eine Preisliste und eine Preisgruppe zu.

Jeder Preisgruppe können Sie dann im Dialog **Gruppenzuschläge** ein Austauschzuschlag zuweisen, wodurch die Verwaltung von Preisen und deren Zuschlägen erheblich vereinfacht ist.
⇨ Tutorial 1, "Preisgruppen zuordnen" auf Seite B-281

### Menü Funktionen

Über dieses Menü können Sie den Dialog **Schlüssel kopieren** öffnen, in dem Sie den Schlüssel eines Jahrgangs in einen anderen kopieren können.
⇨ "Preisgruppenzuordnung kopieren" auf Seite B-697

### Identifikation - Tarif

**Verkaufsliste, Einkaufsliste**
Mit der Wahl der Option legen Sie fest, welcher Art von Tarifen Sie Preisgruppen zuordnen wollen.

**Jahrgang, Schlüssel**
Preisjahrgang und Schlüssel (Tarif), in denen der Preis festgelegt ist.

### Produktauswahl

In diesem Bereich wählen Sie Produkte aus, die Sie in einem Isolierglas und/oder in einem VSG eintauschen können.

**Artikel/MCode, Bezeichnung**
Nummer, Matchcode und Bezeichnung des Produktes, das der Preisgruppe zugeordnet wird.

### Übersicht Zuordnungen

In der Übersicht werden alle Produkte angezeigt, die den Auswahlkriterien entsprechen.

**PG ISO, PG VSG**
In den Spalten PG ISO und PG VSG wählen Sie die Preisgruppen aus, zu denen das Eintauschprodukt gehören soll.

## Preisgruppenzuordnung kopieren (Schlüssel kopieren)

**Stammdaten > Preise > Preisgruppenzuordnung > Menü Funktionen > Kopieren**

_Abb. B-426: Preisgruppenzuordnung – Kopieren_

In diesem Dialog kopieren Sie Preisgruppenzuordnung in einen anderen Tarif.
Die Felder sind zum Dialog **Preisgruppenzuordnung** beschrieben.
⇨ "Preisgruppenzuordnung" auf Seite B-696

## Gruppenzuschläge

**Stammdaten > Preise > Gruppenzuschläge**

_Abb. B-427: Preisgruppenabhängige Zuschläge_

In diesem Dialog legen Sie allgemeine Zuschläge zu den Preisgruppen an, die beim Austausch eines Glases berechnet werden sollen. Im Unterschied zu den Austauschzuschlägen wird hier die Dicke des Glases als Grenztyp eingesetzt.
⇨ Tutorial 1, "Gruppenzuschlag anlegen" auf Seite B-284

### Menü Funktionen

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Dialog zu schließen. Folgende Einträge werden angezeigt:
- **Preise kopieren:** Öffnet den Dialog **Austauschpreise kopieren**, um Gruppenzuschläge zu kopieren.
  ⇨ "Austauschpreise kopieren" auf Seite B-684
- **Preis löschen:** Öffnet den Dialog **Preise nach Preisgruppen löschen**, um Gruppenzuschläge zu löschen.
  ⇨ "Gruppenzuschläge löschen" auf Seite B-703
- **Preis ändern:** Öffnet den Dialog **Preise ändern**, um einen oder eine Folge von Zuschlägen gleichzeitig zu ändern.
  ⇨ "Preise ändern" auf Seite B-736

### Identifikation - Tarif

**Verkaufsliste, Einkaufsliste**
Mit der Wahl der Option legen Sie fest, welcher Art von Tarifen Sie Gruppenzuschläge zuordnen wollen.

**Jahrgang, Schlüssel**
Preisjahrgang und Schlüssel (Tarif), denen der Gruppenzuschlag zugeordnet ist.

**Produktart ISO, VSG**
Produktart, bei der der Gruppenzuschlag erhoben wird. Nur in ISO oder VSG können Gläser ausgetauscht werden. Dabei spielt es keine Rolle, an welcher Stelle das Glas getauscht wird, also in einem Mehrfach-ISO das zweite oder dritte Glas.

**Dicke**
Dicke der auszutauschenden Scheibe. Das ist die Scheibe, die aus dem ISO oder VSG herausgenommen wird.

### Auswahl Kundengruppe/Kunden, Lieferantengruppe/Lieferanten

In diesem Bereich ordnen Sie einen Preisgruppenzuschlag einem Kunden, Lieferanten oder einer Kunden-, Lieferantengruppe zu.

Mit der Wahl der Option legen Sie fest, für wen der Zuschlag gelten soll:
- **Allgemein:** Allgemeiner Zuschlag
- **Kundengruppe, Lieferantengruppe:** Zuschlag für die ausgewählte Gruppe von Kunden oder Lieferanten
- **Kunde, Lieferant:** Zuschlag für den ausgewählten Kunden oder Lieferanten

**Name 1, Name 2**
Name der ausgewählten Partner.

### Übersicht

In der Übersicht werden alle Gruppenzuschläge angezeigt, die den Auswahlkriterien entsprechen.
- **Glasdicke:** Dicke der auszutauschenden Scheibe, das ist die Scheibe, die aus dem ISO oder VSG herausgenommen wird.
- **Preisgruppe:** Preisgruppe, für die der Zuschlag gilt.
- **Zuschlag:** Zuschlagswert pro Dicke. Der Wert wird je nach Zuschlagstyp als prozentualer Zuschlag oder als Betrag interpretiert.
- **Zuschlagstyp:** Der Zuschlagstyp gibt an, wie der Wert im Feld **Zuschlag** interpretiert werden soll, z. B. als prozentualer Aufschlag auf den Preis, als Betrag pro Länge usw.
- **Mindestfläche:** Wenn Sie eine Mindestfläche für ein Eintauschglas angeben, wird diese Fläche in all den Fällen als Zuschlagsbasis herangezogen, in denen die Fläche im Auftrag kleiner ist.
- **Brutto-Mindestpreis, Netto-Mindestpreis:** Wenn Sie einen Mindestpreis angeben, wird dieser immer dann als Basis für den Zuschlag herangezogen, wenn der Preis des Eintauschproduktes im Auftrag darunterliegt.
- **Rundung Breite, Rundung Höhe:** Sie können abweichende Rundungen für die Breite und Höhe angeben, die immer dann berechnet werden, wenn der Gruppenzuschlag zur Preisfindung herangezogen wird.
- **Sonstige Zuschläge:** Sie können zusätzlich zum Austauschzuschlag einen Sonstigen Zuschlag erheben, z. B. für Zuschnittskosten. Dieser Zuschlag wird für das Eintauschprodukt berechnet. Die Sonstigen Zuschläge werden im gleichnamigen Dialog angelegt:
  ⇨ "Sonstige Zuschläge" auf Seite B-675
- **Preisschlüssel, Preisliste:** Anzeige des zugeordneten Schlüssels und Jahrgangs.

### Objektauswahl

Der Zuschlag kann sich auf ein bestimmtes Objekt beziehen. Zur Auswahl werden alle Objekte angeboten.

### Tabelle

#### Übersicht nach Kunden/Kundengruppen, Lieferanten/Lieferantengruppen

In der Übersicht werden Kunden/Kundengruppen, Lieferanten/Lieferantengruppen oder Objekte angezeigt, zu denen Gruppenzuschläge in gewählten Tarif hinterlegt sind.

## Gruppenzuschläge kopieren

**Stammdaten > Preise > Gruppenzuschläge > Menü Funktionen > Preise kopieren**

Sie können einzelne oder mehrere Gruppenzuschläge gemeinsam ändern.

In diesem Dialog finden Sie folgende Register:
- "Gruppenzuschläge kopieren – Quelle, Ziel" auf Seite B-701
- "Gruppenzuschläge kopieren – Preisänderung" auf Seite B-702

### Gruppenzuschläge kopieren – Quelle, Ziel

**Stammdaten > Preise > Gruppenzuschläge > Menü Funktionen > Preise kopieren**

_Abb. B-428: Preisgruppenabhängige Zuschläge kopieren – Register Quelle_

In diesem Register kopieren Sie die Gruppenzuschläge, z. B. um die Zuschläge einer Dicke in einen anderen Tarif zu übertragen.
⇨ Tutorial 1, "Gruppenzuschlag kopieren" auf Seite B-291

#### Kopieren von, Kopieren nach

**Dicke von, bis**
Dicke der Gläser, für die ein Gruppenzuschlag berechnet wird.

**Jahrgang, Schlüssel**
Preisjahrgang und Schlüssel (Tarif), denen der Gruppenzuschlag zugeordnet ist.

**ISO, VSG, Beides**
Produktart, bei der der Gruppenzuschlag erhoben wird. Mit der Option **Beides** werden die Gruppenzuschläge für ISO und VSG kopiert.

**Preise überschreiben**
Wenn Sie die Zuschläge in eine gefüllte Tabelle übertragen wollen, müssen Sie entscheiden, ob die Zuschläge in der Ziel-Tabelle überschrieben werden sollen.
- [ ] Die Zuschläge der Ziel-Tabelle werden nicht überschrieben. Die zusätzlichen Zuschläge aus der Quell-Tabelle werden hinzugefügt.
- [x] Alle vorhandenen Zuschläge in der Ziel-Tabelle werden überschrieben.

**Preisart**
Mit der Wahl der Option legen Sie fest, für wen die Zuschläge gelten sollen:
- **Allgemein:** Allgemeiner Zuschlag, der unabhängig von Marktpartnern oder Partner- gruppen berechnet wird (Standard-Austauschzuschlag).
- **Kundengruppe, Lieferantengruppe:** Zuschlag für die ausgewählte Gruppe von Kunden oder Lieferanten
- **Kunde, Lieferant:** Zuschlag für den ausgewählten Kunden oder Lieferanten

**Objekt**
Das Feld ist gesperrt, wenn Sie die Option **Allgemein** gewählt haben. Bei der Auswahl einer Gruppe oder eines Partners können Sie zusätzlich angeben, für welches Objekt die Zuschlagstabelle geändert werden soll.

### Gruppenzuschläge kopieren – Preisänderung

**Stammdaten > Preise > Gruppenzuschläge > Menü Funktionen > Preise kopieren**

_Abb. B-429: Preisgruppenabhängige Zuschläge kopieren – Register Preisänderung_

In diesem Register geben Sie die Details für die Änderung an.
Die Felder in den Bereichen **Kopieren von** und **Kopieren nach** sind zum Register **Quelle** beschrieben.
⇨ "Gruppenzuschläge kopieren - Quelle, Ziel" auf Seite B-701

**Aufschlag, Abschlag**
Mit der Wahl der Option legen Sie fest, ob der eingegebene Wert auf die Zuschläge der Tabellen auf- oder abgeschlagen werden soll.

**Rundung**
Sie können die Rundung für die ausgewählten Zuschläge ändern.

**Prozent, Absolut**
Wenn die Zuschläge selbst geändert werden sollen, geben Sie einen prozentualen oder absoluten Wert an.

## Gruppenzuschläge löschen

**Stammdaten > Preise > Gruppenzuschläge > Menü Funktionen > Preise löschen**

_Abb. B-430: Preisgruppenabhängige Zuschläge löschen_

In diesem Dialog löschen Sie Gruppenzuschläge einzeln oder eine Folge von Gruppenzuschlägen.

### Preisart

Mit der Wahl der Option legen Sie fest, für wen der Zuschlag gilt:
- **Allgemein:** Allgemeiner Zuschlag, der unabhängig von Marktpartnern oder Partner- gruppen berechnet wird (Standard-Austauschzuschlag).
- **Kundengruppe, Lieferantengruppe:** Zuschlag für die ausgewählte Gruppe von Kunden oder Lieferanten
- **Kunde, Lieferant:** Zuschlag für den ausgewählten Kunden oder Lieferanten

### Objekt

Der Zuschlag kann sich auf ein bestimmtes Objekt beziehen. Zur Auswahl werden alle Objekte angeboten.

#### Preisauswahl

**Dicke von, Dicke bis**
Glasdicke, für die der Gruppenzuschlag angelegt ist.

**Anzahl**
Anzahl der Datensätze.

**ISO, VSG, Beides**
Produktart, bei der der Zuschlag erhoben wird. Mit der Option **Beides** werden die Zuschläge für ISO und VSG gelöscht.

**Anzahl**
Anzahl der Datensätze, die gelöscht werden.

**Jahrgang, Schlüssel**
Preisjahrgang und Schlüssel (Tarif), denen der Gruppenzuschlag zugeordnet ist.

## Gruppenzuschläge ändern

**Stammdaten > Preise > Gruppenzuschläge > Menü Funktionen > Preise ändern**

Sie können einzelne oder mehrere Gruppenzuschläge gemeinsam ändern.

In diesem Dialog finden Sie folgende Register:
- "Gruppenzuschläge ändern - Preisart" auf Seite B-704
- "Gruppenzuschläge ändern – Preisänderung" auf Seite B-706

### Gruppenzuschläge ändern – Preisart

**Stammdaten > Preise > Gruppenzuschläge > Menü Funktionen > Preise ändern**

_Abb. B-431: Preisgruppenabhängige Zuschläge ändern und Register Preisänderung_

In diesem Register wählen Sie Gruppenzuschläge aus, die Sie ändern wollen.
Gruppenzuschläge werden auf die gleiche Weise geändert wie Austauschzuschläge.
⇨ Tutorial 1, "Austauschzuschlag kopieren und ändern" auf Seite B-304

#### Preisauswahl

**Nummer von, Nummer bis**
Glasdicke, für die der Gruppenzuschlag angelegt ist.

**Anzahl**
Anzahl der Datensätze.

**Jahrgang, Schlüssel**
Preisjahrgang und Schlüssel (Tarif), denen der Gruppenzuschlag zugeordnet ist.

**ISO, VSG, Beides**
Produktart, bei der der Zuschlag erhoben wird. Mit der Option **Beides** werden die Zuschläge für ISO und VSG geändert.

#### Preisart

Mit der Wahl der Option legen Sie fest, für wen die Zuschläge gelten sollen:
- **Allgemein:** Allgemeiner Zuschlag, der unabhängig von Marktpartnern oder Partner- gruppen berechnet wird (Standard-Austauschzuschlag).
- **Kundengruppe, Lieferantengruppe:** Zuschlag für die ausgewählte Gruppe von Kunden oder Lieferanten
- **Kunde, Lieferant:** Zuschlag für den ausgewählten Kunden oder Lieferanten

**Objekt**
Das Feld ist gesperrt, wenn Sie die Option **Allgemein** gewählt haben. Bei der Auswahl einer Gruppe oder eines Partners können Sie zusätzlich angeben, für welches Objekt die Zuschläge geändert werden sollen.

### Gruppenzuschläge ändern – Preisänderung

**Stammdaten > Preise > Gruppenzuschläge > Menü Funktionen > Preise ändern**

_Abb. B-432: Preisgruppenabhängige Zuschläge ändern und Register Preisänderung_

In diesem Register geben Sie die Details für die Änderung an.

**Aufschlag, Abschlag**
Mit der Wahl der Option legen Sie fest, ob der eingegebene Wert auf die Zuschläge der Tabellen auf- oder abgeschlagen werden soll.

**Rundung**
Sie können die Rundung für die ausgewählten Zuschläge ändern.

**Prozent, Absolut**
Wenn die Zuschläge selbst geändert werden sollen, geben Sie einen prozentualen oder absoluten Wert an.

## Mischkalkulation

**Stammdaten > Preise > Mischkalkulation**

_Abb. B-433: Mischkalkulation_

Für spezielle Aufbauten in ISO- oder VSG-Scheiben können Sie auf gesonderte Preise verweisen, z. B. bei einem ISO 4/6.

Voraussetzung ist, dass in den Firmendaten der Preisanteil der Komponenten für die Kalkulation angegeben ist.
⇨ "Firmendaten - Dokumente" auf Seite B-941

In der Positionserfassung wird Isolierglas in Form von Mischkalkulation im Register **Zusatz** erfasst. Dabei muss die Position in einer bestimmten Reihenfolge eingegeben werden:
- Im Hauptprodukt selbst darf nichts eingetragen werden, sondern nur im Register **Zusatz > Mischkalkulation**.
- Die ISO-Produkte und ggf. der Mischfaktor werden von außen nach innen eintragen.
- Anschließend müssen im ersten Register die Stückzahl, Breite und Höhe und ggf. einen Austausch ergänzt werden.

Sonstige Zuschläge werden nur berücksichtigt, wenn sie in den Preisen hinterlegt sind.

## Modellbearbeitungszuschläge

**Stammdaten > Preise > Modellzuschläge**

**Zu Dialogbeschreibung:**
⇨ Zuschläge kopieren

_Abb. B-434: Modellbearbeitungszuschläge_

In diesem Dialog legen Sie Bearbeitungszuschläge für Modelle an. Diese Zuschläge können pro Preistabelle unterschiedlich sein, z. B. pro Modelle für die Kantenbearbeitungen und die Eckenbearbeitungen. Voraussetzung ist, dass für die unterschiedlichen Bearbeitungen jeweils eine Preistabelle angelegt ist.
⇨ Tutorial 1, "Modellbearbeitungszuschlag anlegen" auf Seite B-310

### Menü Funktionen

Über dieses Menü öffnen Sie den Dialog **Zuschläge kopieren**, in dem Sie die Modellzuschläge einer Zuschlagstabelle in eine andere Tabelle kopieren können.
⇨ "Zuschläge kopieren" auf Seite B-710

### Bearbeitung

**Preistabelle**
Nummer der Preistabelle für Bearbeitungen.

**Preisjahrgang, Preisschlüssel**
Preisjahrgang und -schlüssel (Tarif), die bei Bearbeitungen von Modellen herangezogen werden.

**Preis-Typ**
Der Preistyp gibt an, wie die Werte in den Feldern **Segment** interpretiert werden sollen, z. B. als prozentualen Aufschlag auf den Preis, als Betrag pro Länge oder pro Stück.

### Zuschläge

Je nach Modell werden die Felder Segment 1 bis Segment 8 freigeschaltet, in denen Sie die Werte für den Zuschlag eingeben können. Der Wert wird je nach Preistyp als prozentualer Zuschlag oder als Betrag interpretiert (für alle Segmente).

Je nach Schwierigkeit der Bearbeitung können die Werte unterschiedlich groß sein. So kann z. B. für die Bearbeitung einer gebogenen Kante ein höherer Zuschlag berechnet werden als für eine gerade Kante.

### Modell

**Nummer**
Nummer des Modells, für das der Zuschlag berechnet werden soll. Wenn Sie ein Modell angegeben haben, wird im Feld **Skizze** eine schematische Darstellung des Modells mit den Segmenten angezeigt, für die Werte eingegeben werden können.

**Skizze**
Schematische Darstellung des Modells, aus der Sie die Nummern der Segmente ablesen können. Die äußeren Nummern bezeichnen die Kanten, die inneren die Ecken.

### Mindest-Angaben

**Mindestpreis**
Wenn Sie einen Mindestpreis angeben, wird dieser immer dann als Basis für den Zuschlag herangezogen, wenn der Preis der Bearbeitung im Auftrag darunterliegt. Diese Angabe eignet sich nicht für den Preistyp **Stück**.

**Mindestmenge**
Wenn Sie eine Mindestmenge angeben, wird diese immer dann als Basis für den Zuschlag herangezogen, wenn der Preis der Bearbeitung im Auftrag darunterliegt. Diese Angabe eignet sich besonders für den Preistyp **Stück**.

### Tabelle

In der Übersicht werden alle Modellzuschläge aufgelistet, die den Auswahlkriterien entsprechen.

## Zuschläge kopieren

**Stammdaten > Preise > Modellzuschläge**

_Abb. B-435: Modellbearbeitungszuschläge kopieren_

In diesem Dialog kopieren Sie die Modellzuschläge einer Zuschlagstabelle in eine andere Tabelle.

### Quelle, Ziel

In diesen Feldern geben Sie an, aus welcher Preisliste die Zuschläge kopiert und auf welche diese übertragen werden sollen.

**Preisjahrgang, Preisschlüssel**
Preisjahrgang und -schlüssel (Tarif), denen die Zuschlagstabelle zugeordnet ist.

**Preistabelle auswählen**
Sie können die Übertragung auf eine Zuschlagstabelle einschränken.
- [x] Alle Modellbearbeitungszuschläge der gewählten Preisliste werden kopiert.
- [ ] Das Feld **Preistabelle** wird freigeschaltet, so dass Sie die Zuschlagstabelle auswählen können, die kopiert werden soll.

**Preistabelle**
Auswahl der Zuschlagstabelle, die kopiert werden soll. Das Feld ist nur freigeschaltet, wenn die Checkbox **Preistabelle auswählen** markiert ist.

**Vorhandene Einträge überschreiben**
Wenn in der Ziel-Tabelle bereits Modellbearbeitungszuschläge angelegt sind, müssen Sie entscheiden, ob Sie diese behalten oder überschreiben wollen.
- [ ] Die vorhandenen Zuschläge werden beibehalten und durch die neuen Zuschläge aus der Quell-Tabelle ergänzt.
- [x] Die Zuschläge in der Ziel-Tabelle werden mit den Zuschlägen aus der Quell-Tabelle überschrieben. Zusätzliche Zuschläge werden hinzugefügt.

## Preis- und Mengeneinheit

**Stammdaten > Preise > Preis/Menge**

> **i Dialog gesperrt**
> Dieser Dialog kann in der Regel nur vom Systemadministrator aufgerufen werden. Änderungen dürfen nur in Absprache mit der A+W Software GmbH vorgenommen werden.

Die Preis- und Mengeneinheiten sind fest vorgegeben. Sie können diese Einheiten nicht löschen. Sie können zwar Mengeneinheiten hinzufügen, diese werden vom System aber nicht berücksichtigt.

_Abb. B-436: Preis- und Mengeneinheiten_

In diesem Dialog können Sie die Preis- und Mengeneinheiten sperren oder bearbeiten, d. h., in andere Sprachen übersetzen.

Die Preiseinheiten werden in der Preisverwaltung den jeweiligen Preisen zugeordnet.
⇨ "Preisverwaltung" auf Seite B-723

Die Mengeneinheiten werden in der Produktverwaltung dem jeweiligen Produkt zugeordnet.
⇨ "Produktverwaltung" auf Seite B-596

### Sprache

Wenn Sie das Modul **Mehrsprachigkeit** einsetzen, müssen die Einheiten in allen Sprachregistern vorhanden sein.

Sie können im Dialog **Sprachen** über **Menü > Einheiten kopieren** die Preis- und Mengeneinheiten von der Basissprache in jede andere Sprache kopieren.
⇨ "Preis-/Mengeneinheit für Mehrsprachigkeit" auf Seite B-565

Nach dem Kopieren können die Texte in die Sprachen übersetzt werden. Achten Sie darauf, dass der Schlüssel der Basissprache im übersetzten Text nicht geändert ist.

### Übersicht

**Preiseinheit**
Die Einheiten können als Preis- und/oder als Mengeneinheit interpretiert werden, z. B. kann die Einheit **qm** sowohl als Mengeneinheit als auch als Preiseinheit genutzt werden, während die Einheit **Net-%** nur als Preiseinheit verwendet wird.

**Schlüssel**
Identifikationsnummer (ID) der Einheit. Sie ist vom System vorgegeben und darf nicht verändert werden.

**Bemerkung**
Diesen Text können Sie ändern.

**Inch**
Wenn Sie mit dem metrischen und dem imperialen Maßsystem arbeiten, gibt es für bestimmte Maßeinheiten zwei Einträge zum gleichen Schlüssel.
Die parallele Verwendung beider Maßsysteme sollte immer mit der A+W Software GmbH abgesprochen werden.

**Fremdschlüssel**
Fremdschlüssel für die Kommunikation mit anderen Programmen, z. B. für die Übergabe an die Produktion oder für statistische Auswertungen.

**Gesperrt**
Eine Einheit kann für die Erfassung in der Preisverwaltung und in den Dokumenten gesperrt werden, wenn sie nicht mehr benötigt wird.
- [ ] Die Einheit kann zugewiesen werden.
- [x] Die Einheit ist gesperrt und kann nicht mehr zugewiesen werden. Wenn sie Produkten und in Dokumenten zugewiesen ist, wird sie jedoch weiterhin angezeigt.

## Versicherungspreise

**Stammdaten > Preise > Versicherungspreise**

Mit Hilfe des Moduls **Versicherungspreise** können bei der Erfassung von Auftragspositionen Reparatur- oder Notverglasungen nach den Richtlinien der Preislisten der Frankfurter oder Gothaer Versicherung kalkuliert werden.

Grundsätzlich wird zwischen Reparatur- und Notverglasung unterschieden. In der Auftragserfassung wird abgefragt, ob Sie entweder eine Reparatur- oder eine Notverglasung erfassen möchten.

In diesem Dialog werden die entsprechenden Versicherungskonditionen verwaltet.

Im Dialog **Versicherungspreise** finden Sie folgende Register:
- Versicherungspreise - Reparaturverglasung
- Versicherungspreise – Notverglasung
- Versicherungspreise – Auf-/Abschläge
- Versicherungspreise – Zusatzleistungen

## Versicherungspreise – Reparaturverglasung

**Stammdaten > Preise > Versicherungspreise > Register Reparaturverglasung**

_Abb. B-437: Versicherungspreise - Reparaturverglasung_

In diesem Register hinterlegen Sie die Kalkulation von Reparaturen. Die Reparaturen, Entsorgungen und Arbeitszeitzuschläge müssen als Produkte mit der Produktart und -gruppe **Leistungen/Zuschläge** erfasst sein.

**Kalkulationsart**
Versicherungen, für die die Kalkulationsvorgaben gelten. Die in den Abbildungen gezeigten Beispiele gelten nur für Deutschland.

### Tarif

**Jahrgang**
Jahrgang der Versicherungspreise.

**Schlüssel**
Schlüssel der Versicherungspreise.

### Reparatur-/Entsorgungszuordnung

**Reparatur**
Reparatur-Produktnummer für die markierte Produktart bzw. Produktgruppe.

**Entsorgung**
Produktnummer der Entsorgung für die markierte Produktart bzw. Produktgruppe.

### Nach Produktart, nach Produktgruppe

**Produktart, Produktgruppe**
Produktart und Produktgruppe, der die Reparatur- bzw. Entsorgungsprodukte zugeordnet sind.

**Reparatur, Entsorgung**
In diesen beiden Tabellenfeldern werden die Produktnummern aus den Feldern **Reparatur** und **Entsorgung** angezeigt.

### Arbeiten außerhalb der regelmäßigen Arbeitszeit

**Nachtarbeit/Arbeit an Sonn-/Feiertagen**
Produktnummer der Leistung, die bei Nachtarbeit bzw. Arbeit an Sonn- und Feiertagen berechnet wird.

**Außerhalb der regelmäßigen Arbeitszeit**
Produktnummer der Leistung, die für Zeiten an Werktagen berechnet wird, die außerhalb der regelmäßigen Arbeitszeiten liegen.

### Tabelle

In der Übersicht werden alle Tabellen für Versicherungspreise angezeigt, die den Auswahlkriterien entsprechen.

## Versicherungspreise – Notverglasung

**Stammdaten > Preise > Versicherungspreise > Register Notverglasung**

_Abb. B-438: Versicherungspreise - Notverglasung_

In diesem Register hinterlegen Sie die Kalkulation von Notverglasungen.
Die Felder **Kalkulationsart** und **Tarif** sind zum Register **Reparaturverglasung** erklärt.
⇨ "Versicherungspreise – Reparaturverglasung" auf Seite B-714

### Notverglasung

**Notverglasung**
Zuschlagsprodukt für die Notverglasung.

**Mindestauftragswert**
Beträge, die als Mindestwert berechnet werden für:
- Notverglasung (Material)
- Nacht- und Feiertagsarbeit (Zuschlag)
- Arbeiten außerhalb der Betriebszeit
Wenn im Auftrag der tatsächliche Preis für die Notverglasung unter diesem Mindestwert liegt, wird automatisch der Mindestwert berechnet. Dabei wird jeder einzelne Wert geprüft.

**Nachtarbeit/Arbeit an Sonn-/Feiertagen**
Produktnummer der Leistung, die bei Nachtarbeit bzw. Arbeit an Sonn- und Feiertagen berechnet wird.

**Außerhalb der regelmäßigen Arbeitszeit**
Produktnummer der Leistung, die für Zeiten an Werktagen berechnet wird, die außerhalb der regelmäßigen Arbeitszeiten liegen.

**Entsorgung**
Produktnummer der Entsorgung.

## Versicherungspreise – Auf-/Abschläge

**Stammdaten > Preise > Versicherungspreise > Register Auf-/Abschläge**

_Abb. B-439: Versicherungspreise – Auf-/Abschläge_

In diesem Register legen Sie die Auf- und Abschläge fest, die für die jeweilige Versicherung gelten. Die Felder werden abhängig von der gewählten Versicherung freigeschaltet.
Die Felder **Kalkulationsart** und **Tarif** sind zum Register **Reparaturverglasung** erklärt.
⇨ "Versicherungspreise - Reparaturverglasung" auf Seite B-714

### Aufschläge für Scheiben

(Nur bei Frankfurter Versicherung)

**Bis ... qm ... Stk**
Sie können bis zu vier Stufen für die Zuschläge festlegen. Pro Stufe legen Sie den Zuschlag pro Stück fest.

> **Beispiel**
> Bis 0,25 qm werden pro Scheibe 80,00 € aufgeschlagen.
> Bis 0,80 qm werden pro Scheibe 60,00 € aufgeschlagen.
> usw.

**Für max. ... Scheiben**
Sie können die Scheibenzuschläge auf eine maximale Anzahl von Scheiben begrenzen. Wenn im Auftrag mehr Scheiben erfasst sind, werden Aufschläge nicht berücksichtigt.

### Fahrtkosten

**Produktnummer**
Produktnummer für die Fahrtkostenpauschale.

**Bis Nettoauftragswert**
Sie können einen Auftragswert (netto) eintragen, bis zu dem der Zuschlag berechnet wird. Wenn der Auftragswert darüberliegt, wird kein Zuschlag berechnet.

### Werkstattarbeit

**Einsetzkostenvergütung**
Prozentualer Zuschlag, der bei einer Reparatur für die Werkstattarbeiten berechnet wird. Der Zuschlag wird auf der Basis des Auftragswerts berechnet.

### Zuschlag für Dacharbeiten

**Zuschlag**
Prozentualen Zuschlag, der bei einer Reparatur für die Dacharbeiten berechnet wird. Der Zuschlag wird auf der Basis des Auftragswerts berechnet.

### Mengennachlässe pro Objekt

(Nur bei Gothaer Versicherung)

**Fenster-/Gussglas**
Fläche in qm, ab der ein Mengennachlass gewährt wird.

**Sonstige Gläser**
Anzahl in Stück, ab der ein Mengennachlass gewährt wird.

## Versicherungspreise – Zusatzleistungen

**Stammdaten > Preise > Versicherungspreise > Register Zusatzleistungen**

_Abb. B-440: Versicherungspreise - Zusatzleistungen_

In diesem Register geben Sie die Zusatzleistungen an, die für die jeweilige Versicherung gelten. Dazu müssen Kleber und Zement als Produkte angelegt sein.

Die Felder werden abhängig von der gewählten Versicherung freigeschaltet.
Die Felder **Kalkulationsart** und **Tarif** sind zum Register **Reparaturverglasung** erklärt.
⇨ "Versicherungspreise - Reparaturverglasung" auf Seite B-714

### Mindesteinsetzkosten

(Nur bei Gothaer Versicherung)

**Bei Vorortarbeit, bei Werkstattarbeit**
Sie können für die erste und für jede weitere Scheibe unterschiedliche Mindestbeträge definieren, die berechnet werden, wenn der tatsächliche Preis der Arbeit unter dem Mindestpreis liegt.

**Max. ... Scheiben**
Sie können die Mindesteinsetzkosten auf eine maximale Anzahl von Scheiben begrenzen. Wenn im Auftrag mehr Scheiben erfasst sind, werden die Mindestkosten nicht berücksichtigt.

### Kleber/Zement

(Alle Versicherungen)

**Kleber (inkl. Lösen, Reinigen, Kleben)**
Produktnummer für den Kleber.

**Zement (inkl. Lösen, Reinigen, Kleben)**
Produktnummer für den Zement.

**Kleber (ohne Lösen, Totalschaden)**
Produktnummer für den Kleber bei Totalschaden.

**Zement (ohne Lösen, Totalschaden)**
Produktnummer für den Zement bei Totalschaden.

## Sprossenpreiselemente

**Stammdaten > Preise > Sprossenpreiselemente**

_Abb. B-441: Sprossenpreiselemente_

In diesem Dialog sind die Sprossenelemente hinterlegt, die zur Preisberechnung im Auftrag herangezogen werden können.

Die Nummern der Elemente müssen mit den Nummern aus **A+W CAD Designer (Bars)** übereinstimmen. Sie können weitere Elemente hinzufügen. Diese müssen auch in **A+W CAD Designer(Bars)** definiert werden.

Die Preise für diese Sprossenelemente legen Sie im Dialog **Preise** an:
⇨ "Preise - Sprossen" auf Seite B-733

## ISO Preise

**Stammdaten > Preise > ISO Preise**

_Abb. B-442: ISO Preise_

In diesem Dialog können Sie für flexible Isolierglasaufbauten bis 3-fach-Isolierglas eine Preistabellenzuordnung definieren. In dieser Preistabelle steht der für diesen Aufbau gültige Preis. Es können auch unterschiedliche Preisschlüssel oder individuelle Preise herangezogen werden.

Jede Änderung der Preisezuordnung ist sofort in der Auftragserfassung gültig, dies erfolgt auch Rechnerübergreifend.

### Produkte

**Glas 1, Glas 2, Glas 3**
Hier geben Sie die entsprechenden Gläser für den Produktaufbau ein.

**Abstandhalter 1, Abstandhalter 2**
Hier geben Sie den bzw. die entsprechenden Abstandhalter für den Produktaufbau ein. Geben Sie beim Abstandhalter und beim Gas eine 0 ein, sind diese gültig für alle Produkte.

**Gas 1, Gas 2**
Hier geben Sie das bzw. die entsprechenden Gase für den Produktaufbau ein. Geben Sie beim Abstandhalter und beim Gas eine 0 ein, sind diese gültig für alle Produkte.

**Preistabelle**
Wählen Sie die Preistabelle aus, die für den Produktaufbau verwendet werden soll. Bitte denken Sie daran, dass im Produktstamm die entsprechende Checkbox aktiviert sein muss.
⇨ "ISO-Aufbau Preis" auf Seite B-616

**Reversibel**
Diese Checkbox steuert, ob der Preis auch für den gespiegelten Aufbau gültig ist.
- [ ] Der Preis ist nicht für den gespiegelten Aufbau gültig.
- [x] Der Preis ist auch für den gespiegelten Aufbau gültig.

## Preisverwaltung

**Stammdaten > Preise > Preise**

Mit der A+W Business-Preisverwaltung richten Sie die Preise für Ihre Produkte ein. Sie können z. B. Preise von Einfachgläsern in Preismatrizen verwalten, diejenigen von ISO-Aufbauten in Würfelform.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menüs in der Preisverwaltung" auf Seite B-723
- "Preise" auf Seite B-725
- "Preise ändern" auf Seite B-736
- "Preise kopieren" auf Seite B-738
- "Preise löschen" auf Seite B-740
- "Preismatrizenimport" auf Seite B-741

Bevor Sie die Preise anlegen, müssen Sie die Tarife eingerichtet haben. Die Beschreibung zu den entsprechenden Dialogen finden Sie im Abschnitt **Preise**:
⇨ "Preise" auf Seite B-670

## Menüs in der Preisverwaltung

**Stammdaten > Preise > Preise**

Über die Menüs der Preisverwaltung können Sie die Standardeinstellung des Dialoges bestimmen und andere Dialoge öffnen, ohne die Preisverwaltung zu schließen.

In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Menü Optionen" auf Seite B-723
- "Menü Funktionen" auf Seite B-724
- "Menü Historie" auf Seite B-724

> **i Menü Historie nur in Verbindung mit Gupta-Datenbank**
> Das Menü **Historie** steht nur in Verbindung mit der SQL Gupta-Datenbank zur Verfügung. In der MS SQL-Datenbank wird das Menü nicht angezeigt.

### Menü Optionen

**Stammdaten > Preise > Preise > Menü Optionen**

Über dieses Menü können Sie die Standardeinstellung des Dialoges bestimmen. Sie können die Option aktivieren oder deaktivieren.
- **Letzten Tarif vorblenden:** Zeigt in den Feldern **Jahrgang** und **Schlüssel** die Einträge des Tarifs an, der zuletzt ausgewählt war.

### Menü Funktionen

**Stammdaten > Preise > Preise > Menü Funktionen**

Über dieses Menü können Sie andere Dialoge öffnen, ohne den Dialog zu schließen.

Das Menü ist in folgende Gruppen gegliedert:
- "Gruppe Preise" auf Seite B-724
- "Gruppe Datenaustausch" auf Seite B-724

#### Gruppe Preise

- **Ändern:** Öffnet den Dialog **Preise ändern**, um einen oder eine Folge von Preisen gleichzeitig zu ändern.
  ⇨ "Preise ändern" auf Seite B-736
- **Kopieren:** Öffnet den Dialog **Preise kopieren**, um die Preise einer Preisliste oder eines Preisschlüssels auf eine andere zu übertragen.
  ⇨ "Preise kopieren" auf Seite B-738
- **Löschen:** Öffnet den Dialog **Preise löschen**, um Preise zu löschen.
  ⇨ "Preise löschen" auf Seite B-740

#### Gruppe Datenaustausch

- **Automatisch importieren:** Öffnet den Dialog **Preise** bzw. **Preismatrizenimport**, um die ISO-Preismatrix aus einer gespeicherten Datei zu importieren.
  ⇨ "Preismatrizenimport" auf Seite B-741
- **Interaktiv importieren:** Öffnet den Dialog **Preise** bzw. **Preismatrizenimport**, um die ISO-Preismatrix aus einer gespeicherten Datei zu importieren.
  ⇨ "Preismatrix importieren" auf Seite B-742
- **Preismatrix exportieren:** Öffnet den Dialog **Preismatrizenexport**, um die ISO-Preismatrix in einer Datei zu speichern.
  ⇨ "Preismatrix exportieren" auf Seite B-743

### Menü Historie

Über das Menü **Historie** können Sie festlegen, welche Änderungen von Stammdaten überwacht werden sollen. Die überwachten Änderungen können Sie sich anzeigen lassen.

> **i Menü Historie nur in Verbindung mit Gupta-Datenbank**
> Das Menü **Historie** steht nur in Verbindung mit der SQL Gupta-Datenbank zur Verfügung. In der MS SQL-Datenbank steht das Menü nicht zur Verfügung.

Dieses Menü steht in folgenden Dialogen zur Verfügung:
- Kundenverwaltung
- Lieferantenverwaltung
- Preisverwaltung
- Rabattverwaltung

Folgende Einträge werden angezeigt:
- **Auswertung:** Öffnet den Dialog **Änderungshistorie**, um die überwachten Änderungen auszuwerten.
  ⇨ "Änderungshistorie" auf Seite B-744

> **i Eintrag Auswertung**
> Der Eintrag **Auswertung** ist nur freigeschaltet, wenn die Änderungsüberwachung im Modul **Utilities > System > Änderungsüberwachung Verwaltung** aktiviert wurde.

## Preise

**Stammdaten > Preise > Preise**

**Zu Dialogbeschreibung:**
⇨ Preismatrizenimport
⇨ Preismatrix importieren
⇨ Preismatrix exportieren

Im Dialog **Preise** finden Sie folgende Register:
- Preise - Preisauswahl
- Preise - Matrix
- Preise - Vektor
- Preise - Einzelpreis
- Preise - Modell
- Preise - Sprossen
- Preise - Würfel
- Preise - Preisformel

In diesem Dialog pflegen Sie die Preise in den verschiedenen Tarifen und Preislisten.
⇨ Tutorial 1, "Preistabellen" auf Seite B-233

> **i Tipp**
> Neue Preislisten können schneller angelegt werden, wenn eine alte Preisliste kopiert und überarbeitet wird.
> ⇨ Tutorial 1, "Preise kopieren und ändern" auf Seite B-249

## Preise – Preisauswahl

**Stammdaten > Preise > Preise > Register Preisauswahl**

_Abb. B-443: Preise - Preisauswahl_

> **i**
> In diesem Register wählen Sie den Tarif aus und ordnen Gruppen, Zuschläge und Objekte zu. Außerdem können Sie festlegen, ob die Preise für Abweichungen gelten sollen.
> ⇨ Tutorial 1, "Einzelpreise anlegen" auf Seite B-239

### Auswahlmodus

Wenn Sie den Dialog öffnen, wird standardmäßig der Auswahlmodus angezeigt. Sie können die Suche nach Preislisten dann zusätzlich auf Kunden, Lieferanten, Gruppen und Objekte einschränken.

In der Übersicht werden alle Preistabellen anzeigt, die mit den Suchkriterien für **Jahrgang** und **Schlüssel** übereinstimmen.

Die Einträge werden je nach Auswahlkriterien in folgenden Gruppen angezeigt:
- Standard (allgemeine Preise)
- Kundengruppen oder Lieferantengruppen
- Kunde oder Lieferant

Die Preise sind jeweils nach Preislisten gruppiert. Wenn Sie eine Preisliste markieren, wird das Register freigeschaltet, in dem der Preis angelegt ist.

Mit einem Doppelklick auf den Eintrag **Zugeordnete Produkte** können Sie sich die Produkte anzeigen lassen, die nach dieser Preisliste berechnet werden.

### Identifikation

**Tabelle von, bis**
Nummer der Preistabelle. In der Regel haben die Tabellen die gleiche Nummer wie das Produkt, auf das sich die Tabelle bezieht.

**Jahrgang, Schlüssel**
Preisjahrgang und Preisschlüssel (Tarif), zu denen die Preise angelegt sind.
Die Felder werden in der Auftragserfassung angezeigt und können pro Position überschrieben werden, um einen anderen Tarif für die Preisberechnung heranzuziehen.

**Schlüsseltext**
Die Bezeichnung für den (Preis-)Schlüssel und der Schlüsseltext müssen identisch sein.

**Bemerkung**
Hinweis, z. B. zur Gültigkeit.

### Sonstige Zuschläge

**Tabelle**
Nummer der Zuschlagstabelle. Diese Zuschläge werden im Auftrag automatisch erhoben, können aber deaktiviert werden.

### Abweichungen

Sie können Abweichungen vom Standard-Produkt festlegen, die zu anderen Berechnungen der Preise führen.

**Modellgruppe**
Wenn im Auftrag ein Modell erfasst wird, das zu einer Modellgruppe gehört, sollen andere Werte für den Flächenpreis gelten.
Sie können z. B. für mehrere ISO-Preisschlüssel unterschiedliche Modellzuschläge verwenden. Um Modellzuschläge nicht für jeden Preisschlüssel anzulegen, können Sie die Abweichung auf eine Modellgruppe nutzen.
Die Modellzuschläge werden im Register **Modelle** angelegt.
⇨ "Preise - Modell" auf Seite B-732

**Rundg. Breite, Rundg. Höhe**
Werte für die Rundung von Breite und Höhe, die sich von der Standardrundung der Produkte unterscheidet.
Diese Rundungswerte gelten nur für die Preisberechnung. Für die Berechnung des Zuschnitts gelten die Werte aus der Produktdefinition.

**Min. Breite, Min. Höhe**
Werte für die Mindestbreite und Mindesthöhe, die von den Werten in der Produktdefinition abweichen.

**Folgeschlüssel**
Wenn Sie den Preis nur bis zu einem bestimmten Maß anlegen wollen, können Sie einen Folgeschlüssel angeben. Dieser legt fest, welche Preistabelle für die Preisberechnung herangezogen werden soll, wenn für das im Auftrag erfasste Maß in der Standard-Preistabelle keine Preise vorhanden sind.

### Preise für

Wenn Sie eine der Preistabellen in der Übersicht markieren, wird in diesem Bereich alle Produkte angezeigt, für welchen Kunden, Lieferanten oder Gruppen angelegt wurden.

Sie können die Suche auf partner- und objektspezifischen Preistabellen einschränken, indem Sie die entsprechenden Kriterien auswählen.

> **i Individuelle Preise**
> Bei der Preisfindung im Dokument haben Individualpreise immer Vorrang vor allen anderen Preisen und Rabatten.

## Preise – Matrix

**Stammdaten > Preise > Preise > Register Matrix**

_Abb. B-444: Preise - Matrix_

In diesem Register legen Sie eine Preismatrix fest, bei der bis zu 2 Grenztypen berücksichtigt werden können.
⇨ Tutorial 1, "Grenztypen für Staffelungen" auf Seite B-254
⇨ Tutorial 1, "Gestaffelten Preis mit Grenzwerten anlegen" auf Seite B-263

### Grenztyp 1, Grenztyp 2

Mit Hilfe der Grenztypen können Sie die Preise staffeln. Der Grenztyp legt die Maßeinheit für die Staffelung fest. Sie können unterschiedliche Maßeinheiten für die beiden Grenztypen auswählen, z. B. Dicke und Gewicht.

Das Eingabefeld für den Grenzwert wird freigeschaltet, wenn Sie eine neue Spalte einfügen. Der Grenzwert bezieht sich auf den Grenztyp. Ist als Grenztyp `<k.A.>` angegeben, gilt der Preis pro Preiseinheit.

### Mindestangaben

Die Mindestangaben werden bei der Auftragserfassung geprüft. Bei Unterschreitung der Preise oder der Menge wird eine Meldung angezeigt und/oder ein Zuschlag erhoben.

**Bruttopreis, Nettopreis**
Mindestpreis für eine Position im Auftrag.

**Menge**
Mindestmenge im Auftrag.

### Preisspezifikation

**Preiseinheit**
Die Preiseinheit bezieht sich auf die Angaben in der Matrix.

**Währung**
Wenn Sie mit mehreren Währungen arbeiten, müssen Sie angeben, für welche Währung die Angaben für den Brutto- oder Nettopreis gelten.

**Dreiecksform**
Sie können in einer Matrix oder in einem Würfel die Preise so erfassen, dass die angegebenen Grenzwerte vertauscht werden dürfen, z. B. Höhe und Breite.
- [ ] Die Grenztypen dürfen nicht vertauscht werden. In diesem Fall müssen Sie in allen Feldern pro Spalte/Zeile einen Preis eintragen. Wählen Sie diese Einstellung für Gläser, bei denen es wichtig ist, in welcher Richtung sie geschnitten werden.
- [x] Die Grenztypen dürfen vertauscht werden. Damit müssen Sie den Preis nur in jeweils einer der Kombinationen der Grenztypen eintragen.
⇨ Tutorial 1, "Dreiecksform" auf Seite B-261

### Matrix

In der Übersicht geben Sie in jedem Feld pro Zeile und Spalte den Preis ein, der bei dieser Kombination von Grenztypen gelten soll.
⇨ Tutorial 1, "Matrix" auf Seite B-260

> **i Kopieren & Einfügen von Preismatrizen aus Microsoft Excel®**
> Mit dieser Funktion können Matrizen und Ebenen des Würfels direkt per aus Excel übernommen werden. Die Kopieren & Einfügen Funktion befindet sich in der linken oberen Ecke der Tabelle, dort wo auch die Eigenschaften geändert werden können. Somit ist es möglich, den Inhalt der Tabelle mit ihren Überschriften direkt in Microsoft Excel® zu übernehmen.

## Preise – Vektor

**Stammdaten > Preise > Preise > Register Vektor**

_Abb. B-445: Preise – Vektor_

In diesem Register legen Sie den Preis mit einem Grenztyp fest.

Sie können die Preisberechnung z. B. auch nach der Anzahl der Scheiben staffeln. Die Grenzmenge **Scheibenzahl** ermittelt die Anzahl der Scheiben auf den Unterebenen des Vaterglases. Hat das Vaterglas keine Kindgläser, so wird die Anzahl 1 zurückgegeben. Diese Form der Staffelung ist z. B. für Zuschläge auf das Gas geeignet.
⇨ Tutorial 1, "Vektor" auf Seite B-259
⇨ Tutorial 1, "Gestaffelten Preis mit Grenzwerten anlegen" auf Seite B-263

Die Felder sind zum Register **Matrix** beschrieben.
⇨ "Preise - Matrix" auf Seite B-728
