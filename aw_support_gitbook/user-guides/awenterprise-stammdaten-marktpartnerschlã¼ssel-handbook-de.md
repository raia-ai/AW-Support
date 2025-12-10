---
title: "DE-HB-AWEnterprise_3"
source: "DE-HB-AWEnterprise_3.pdf"
tags: ["A+W Enterprise", "Stammdaten", "Marktpartnerschlüssel", "Software Referenz", "Mandantenkalender", "Rabattmethoden", "Systemschlüssel", "Produktschlüssel", "ERP", "Benutzerhandbuch"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a software reference manual for A+W Enterprise, focusing on the 'Marktpartnerschlüssel' (Market Partner Keys) and 'Systemschlüssel' (System Keys) within the master data setup. It provides detailed instructions on configuring various system parameters, including client calendars, financial accounting clients (FIBU), country and region settings, quality scales, and discount methods."
long_description: "This excerpt from the A+W Enterprise software reference guide provides an in-depth look at configuring master data related to market partners and system-wide settings. It covers a wide range of functionalities accessible through the 'Schlüssel' (Keys) menu. Key topics include: 'Mandantenkalender' for managing client-specific trading and production days in a multi-site environment; 'FIBU-Mandanten' for setting up financial accounting clients; and defining geographical data such as 'Länder' (Countries), 'Wirtschaftsräume' (Economic Areas), and 'Regionen/Bundesländer' (Regions/Federal States). The guide also details the setup of various 'Qualitätsskalen' (Quality Scales) for evaluating suppliers based on delivery times, prices, and quantities. A significant portion is dedicated to 'Reklamationen' (Complaints), explaining how to define reasons, locations, and types. Furthermore, it explains the intricate system of 'Rabattmethoden' (Discount Methods) and how to configure them with various criteria, sequences, and calculation rules. The document concludes with a comprehensive section on 'Systemschlüssel' and 'Produktschlüssel', which are foundational settings for positions, languages, units of measure, production areas, and much more. Each section includes screenshots, menu paths, and detailed explanations of every field, including technical database information. This guide is essential for system administrators and power users responsible for the initial setup and ongoing maintenance of the A+W Enterprise system."
---

# Marktpartnerschlüssel

---
## Mandantenkalender

**Stammdaten > Schlüssel > Marktpartner > Kalender > Mandantenkalender**
**System-Menü (<Strg> + <F4>) > Infodienste > Kalender > Mandantenkalender**

*Abb. B-67 Mandantenkalender*

Nachdem Sie die Mandantennummer ausgewählt haben, öffnet sich der Kalender.

Diese Kalenderfunktion wird für das Mehr-Mandantensystem (Multi-Site) verwendet. Hier können Sie für jeden internen Mandanten im Betriebskalender eigene Daten hinterlegen. So können Sie mandantenspezifische Handels-, Produktions- und Feiertage hinterlegen.

Es stehen Ihnen zwei unterschiedliche Ansichten zur Verfügung:
*   Tagesansicht
*   Monatsansicht

### Erläuterung der Felder

**Datum** Hier wird Ihnen jedes einzelne Datum angezeigt.

**Tag** Hier wird Ihnen jeder einzelne Tag angezeigt.

**KW** Hier wird Ihnen die Kalenderwoche angezeigt.

**H** Hier sehen Sie, ob dieser Tag bei dem Hauptmandanten ein Handelstag ist oder nicht. Die hauptmandantenspezifischen Handelstage werden in System > Schlüssel > Marktpartner > Kalender > Kalender gepflegt und können hier nicht geändert werden.

**P** Hier sehen Sie, ob dieser Tag bei dem Hauptmandanten ein Produktionstag ist oder nicht. Die hauptmandantenspezifischen Produktionstage werden in System > Schlüssel > Marktpartner > Kalender > Kalender gepflegt und können hier nicht geändert werden

**H-MD** Auswahl, ob es sich bei dem Tag um einen Handelstag handelt.
Technische Info: Toggle-Feld, DB-Feld: alkal.htag

**P-MD** Auswahl, ob es sich bei dem Tag um einen Produktionstag handelt.
Technische Info: Toggle-Feld, DB-Feld: alkal.ptag

**Bemerkung** In diesem Feld können Sie eine entsprechende Bemerkung hinterlegen.
Technische Info: Alphanumerisches Feld, DB-Feld: alkal.bem

**Ergänzende Informationen**
"Kalender" auf Seite B-195

## FIBU-Mandanten

**Stammdaten > Schlüssel > Marktpartner > FIBU-Mandanten**

*Abb. B-68 FIBU-Mandanten*

In diesem Dialog legen Sie die FIBU-Mandanten fest. Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

## Länder

**Stammdaten > Schlüssel > Marktpartner > Länder > Länder**
**Stammdaten > Schlüssel > Marktpartner > Länder > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > Marktpartner > Länder > Alle Bezeichnungen**

*Abb. B-69 Länder*

Dieser Dialog enthält die unterschiedlichen Länder, die bei der Erfassung von Marktpartnern vorkommen können, in den jeweiligen Sprachen.

### Erläuterung der Felder

**KFZ Code/KFZ** KFZ-Codes, z. B. A (Österreich). Zum Anlegen eines neuen Landes geben Sie den entsprechenden Code ein.
Technische Info: <F9>, DB-Feld: xsprbez.cid
View: xland.kfz

**ISO** Ländercode nach ISO-Norm, z. B. AT (Österreich).
Technische Info: Alphanumerisches Feld, DB-Feld: xxland.iso

**Landesbezeichnung** Bezeichnung des Landes, z. B. Belgien.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1
View: xland.atxt

**Fibu** Dieses Feld enthält den entsprechenden Ländercode der Finanzbuchhaltung.
Technische Info: Alphanumerisches Feld, DB-Feld: xxland.fib

**Intracode** Dieses Feld enthält die entsprechende Vorgabe des Statistischen Bundesamtes für die Intrahandelsstatistik.
Technische Info: Alphanumerisches Feld, DB-Feld: xxland.intracode

**Spr** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

## Wirtschaftsraumbezeichnungen

**Stammdaten > Schlüssel > Marktpartner > Wirtschaftsräume > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > Marktpartner > Wirtschaftsräume > Alle Bezeichnungen**

*Abb. B-70 Wirtschaftsräume*

Die freie Aufteilung des Landes in Wirtschaftsräume gewährt die spätere Zuordnung von Marktpartnern zu einem Wirtschaftsraum, unabhängig vom Bundesland.
Dieser Dialog enthält die unterschiedlichen Wirtschaftsräume, die bei der Erfassung von Marktpartnern vorkommen können, in den jeweiligen Sprachen.

### Erläuterung der Felder

**Nummer/Nr** Schlüssel-Nummer. Zum Anlegen eines neuen Wirtschaftsraumes geben Sie die nächste freie Nummer ein.
Technische Info: <F9>, DB-Feld: xsprbez.id
View: xwrtraum.wrtnr

**Spr** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Bezeichnung** Bezeichnung des Wirtschaftsraumes, z. B. Mitte.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1
View: xwrtraum.wrtraum

## Regionen / Bundesländerbezeichnungen

**Stammdaten > Schlüssel > Marktpartner > Region/Bundesländer > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > Marktpartner > Region/Bundesländer > Alle Bezeichnungen**

*Abb. B-71 Regionen/Bundesländer*

Die hier erfassten Bundesländer können im Marktpartnerstamm den Kunden und Lieferanten zugeordnet werden. Die Vergabe der Schlüssel-Nr. sollte für die Intrahandelsstatistik gemäß der entsprechenden Vorgabe des statistischen Bundesamtes erfolgen.
Dieser Dialog enthält die unterschiedlichen Regionen und Bundesländer, in den jeweiligen Sprachen.

### Erläuterung der Felder

**Nummer/Nr** Schlüssel-Nummer. Zum Anlegen einer neuen Region geben Sie die nächste freie Nummer ein.
Technische Info: <F9>, DB-Feld: xsprbez.id
View: xregion.regnr

**Spr** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Region/Bundesland** Bezeichnung der Region, z. B. Mitte.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1
View: xregion.region

## Allgemeine Qualitätsskala

**Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Allgemein > Qualitätsskala**
**Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Allgemein > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Allgemein > Alle Bezeichnungen**

*Abb. B-72 Qualitätsskala*

In diesen Dialogen legen Sie die allgemeinen Qualitäts-Merkmale mit Prioritäten und in verschiedenen Sprachen an. Diese Schlüssel dienen der Beurteilung des Marktpartners und werden für alle Bewertungskriterien eingesetzt.

### Erläuterung der Felder

**Nr** Schlüssel-Nummer. Zum Anlegen einer neuen Qualität geben Sie die nächste freie Nummer ein.
Technische Info: Numerisches Feld, DB-Feld: xxqual.qualkz

**Spr** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Bezeichnung** Bezeichnung, z. B. sehr gute Qualität
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

**Rang** Der Rang, den die Bewertung innerhalb der Bewertungsskala einnimmt.
Technische Info: Alphanumerisches Feld, DB-Feld: xxqual.rang

## Termin-Qualitätsskala

**Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Termine > Qual.-Skala Termine**
**Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Termine > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Termine > Alle Bezeichnungen**

*Abb. B-73 Termin-Qualitätsskala*

Zur Bewertung der Lieferanten bezüglich der Einhaltung von Terminen werden freie Bezeichnungen angelegt und mit einem Rang skaliert.
Der Dialog zeigt Ihnen die angelegten Schlüssel, die zur manuellen Bewertung der Lieferanten im Marktpartnerstamm zur Verfügung stehen.

### Erläuterung der Felder

**Nr** Schlüsselnummer. Zum Anlegen einer neuen Schlüsselnummer geben Sie die nächste freie Nummer ein.
Technische Info: Numerisches Feld, DB-Feld: xsprbez.id
View: xtermin.terminkz

**Spr** Sprachkennzeichens.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Bezeichnung** Schlüsselbezeichnung, z. B. Termingerecht.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1
View: xtermin.atxt

**Rang** Der Rang, den die Bewertung innerhalb der Bewertungsskala einnimmt.
Technische Info: Alphanumerisches Feld, DB-Feld: xxtermin.rang

## Preise-Qualitätsskala

**Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Preise > Qual.-Skala Preise**
**Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Preise > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Preise > Alle Bezeichnungen**

*Abb. B-74 Preise-Qualitätsskala*

Zur Bewertung der Lieferanten bezüglich der Preise können ebenfalls freie Bezeichnungen angelegt und mit einem Rang skaliert werden.
Der Dialog zeigt Ihnen die angelegten Schlüssel, die zur manuellen Bewertung der Lieferanten im Marktpartnerstamm zur Verfügung stehen.

### Erläuterung der Felder

**Nr** Schlüsselnummer. Zum Anlegen einer neuen Schlüsselnummer geben Sie die nächste freie Nummer ein.
Technische Info: Numerisches Feld, DB-Feld: xsprbez.id
View: xpreis.preiskz

**Spr** Sprachkennzeichens.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Bezeichnung** Schlüsselbezeichnung, z. B. Preiswert.
Technische Info: Alphanumerisches Feld, DB-Feld: xxpreis.atxt

**Rang** Der Rang, den die Bewertung innerhalb der Bewertungsskala einnimmt.
Technische Info: Alphanumerisches Feld, DB-Feld: xxpreis.rang
View: xpreis.atxt

## Mengen-Qualitätsskala

**Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Mengen > Qual.-Skala Mengen**
**Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Mengen > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Mengen > Alle Bezeichnungen**

*Abb. B-75 Mengen-Qualitätsskala*

Zur Bewertung der Liefermengen einzelner Lieferanten werden freie Bezeichnungen angelegt und mit einem Rang skaliert.
Der Dialog zeigt Ihnen die angelegten Schlüssel, die zur Verfügung stehen.

### Erläuterung der Felder

**Nr** Schlüsselnummer. Zum Anlegen einer neuen Schlüsselnummer geben Sie die nächste freie Nummer ein.
Technische Info: Numerisches Feld, DB-Feld: xsprbez.id
View: xmenge.mengekz

**Spr** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Bezeichnung** Schlüsselbezeichnung, z. B. Guter Lagerbestand.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1
View: xmenge.atxt

**Rang** Der Rang, den die Bewertung innerhalb der Bewertungsskala einnimmt.
Technische Info: Alphanumerisches Feld, DB-Feld: xxmenge.rang

## Spezial-Qualitätsskala

**Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Spezial > Qual.-Skala Spezial**
**Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Spezial > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Spezial > Alle Bezeichnungen**

*Abb. B-76 Spezial-Qualitätsskala*

Die Qualitätsskala Spezial bietet eine zusätzliche individuelle Möglichkeit, Lieferanten anhand von frei definierbaren Bezeichnungen, denen ein Rang zugeordnet ist, zu beurteilen.
Der Dialog zeigt Ihnen die angelegten Schlüssel, die zur Verfügung stehen.

### Erläuterung der Felder

**Nummer** Schlüssel-Nummer. Zum Anlegen eines neuen Mengenniveaus geben Sie die nächste freie Nummer ein.
Technische Info: <F9>, DB-Feld: xsprbez.id
View: xspec.speckz

**Rang** Der Rang, den die Bewertung innerhalb der Bewertungsskala einnimmt.
Technische Info: Alphanumerisches Feld, DB-Feld: xxspec.rang

**Spr** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Bezeichnung** Bezeichnung des Mengenniveaus, z. B. Guter Lagerbestand.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1
View: xspec.atxt

## Reklamationsgründe

**Stammdaten > Schlüssel > Marktpartner > Reklamation > Gründe > Reklamationsgründe**
**Stammdaten > Schlüssel > Marktpartner > Reklamation > Gründe > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > Marktpartner > Reklamation > Gründe > Alle Bezeichnungen**

*Abb. B-77 Reklamationsgründe*

Hier werden die Reklamationsarten textuell hinterlegt und mit einem frei wählbaren Schlüssel versehen. Sie werden für die Erfassung und Auswertung von Reklamationen benötigt.
Darüber hinaus werden in dieser Tabelle die Codes der Geschäftsart für die Intrahandelsstatistik gepflegt.

### Erläuterung der Felder

**Nr** Schlüsselnummer. Zum Anlegen einer neuen Schlüsselnummer geben Sie die nächste freie Nummer ein.
Technische Info: Numerisches Feld, DB-Feld: xxrart.reklamart

**Reklamationsgrund** Schlüsselbezeichnung, z. B. Verpackung kaputt.
Technische Info: Alphanumerisches Feld, DB-Feld: xxrart.bez

**Intrastat** Der Code gemäß den Vorgaben des Statistischen Bundesamtes.
Technische Info: Alphanumerisches Feld, DB-Feld: xxrart.intrageschart

**Ohne Überschriften** Die beiden Spalten ohne Überschriften können Sie individuell über Umgebungsvariablen definieren.
Technische Info: Alphanumerisches Feld, DB-Feld: xxrart.private_long1/2

**S** Stilllegungskennzeichen.
Technische Info: <Toggle>-Feld, DB-Feld: xxrart.lustill

**Nummer** Auswahl der Schlüssel-Nummer Zum Anlegen einer neuen Schlüsselnummer geben Sie die nächste freie Nummer ein.
Technische Info: <F9>, DB-Feld: xsprbez.id
View: rart.reklamart

**Spr** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Reklamationsgrund** Bezeichnung des Reklamationsgrundes, z. B. Verpackung kaputt.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1
View: rart.atxt

## Reklamationsorte

**Stammdaten > Schlüssel > Marktpartner > Reklamation > Orte > Reklamationsorte**
**Stammdaten > Schlüssel > Marktpartner > Reklamation > Orte > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > Marktpartner > Reklamation > Orte > Einzelne Bezeichnungen**

*Abb. B-78 Reklamationsorte*

Die textuellen Vorgaben für den Reklamationsort können frei definiert werden. Sie sind für die Reklamationsbearbeitung und -statistik von Bedeutung.

### Erläuterung der Felder

**Nummer** Schlüssel-Nummer Zum Anlegen eines neuen Ortes geben Sie die nächste freie Nummer ein.
Technische Info: <F9>, DB-Feld: xsprbez.id
View: rort.reklamort

**Spr** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Reklamationsgrund** Schlüsselbezeichnung, z. B. Produktion.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1
View: rort.atxt

**S** Stilllegungskennzeichen.
Technische Info: <Toggle>-Feld, DB-Feld: xxrart.still

## Reklamationstypen

**Stammdaten > Schlüssel > Marktpartner > Reklamation > Typen > Reklamationstypen**
**Stammdaten > Schlüssel > Marktpartner > Reklamation > Typen > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > Marktpartner > Reklamation > Typen > Alle Bezeichnungen**

*Abb. B-79 Reklamationstypen*

In diesen Dialogen werden die Reklamationstypen textuell hinterlegt und mit einem frei wählbaren Schlüssel versehen. Sie werden für die Erfassung und Auswertung von Reklamationen benötigt.

### Erläuterung der Felder

**Nr/Nummer** Typnummer. Im Feld dahinter geben Sie die Bezeichnung ein. Zum Anlegen einer neuen Schlüsselnummer geben Sie die nächste freie Nummer ein.
Technische Info: Numerisches Feld, DB-Feld: xsprbez.id
View: xxrspec.reklamspec

**Bezeichnung/Reklamationstyp** Bezeichnung des Typs, z. B. Bruch.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1
View: xspec.atxt

**Spr** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Ohne Überschriften** Die beiden Spalten ohne Überschriften können Sie individuell über Umgebungsvariablen definieren.
Technische Info: Alphanumerisches Feld, DB-Feld: xxrspec.private_long1/2

**S** Stilllegungskennzeichen.
Technische Info: <Toggle>-Feld, DB-Feld: xxrspec.still

## Rabattmethoden

**Stammdaten > Schlüssel > Marktpartner > Vorgangsrabatte > Rabattmethoden > Rabattmethoden**
**Stammdaten > Schlüssel > Marktpartner > Vorgangsrabatte > Rabattmethoden > Einzelne Bezeichnung**
**Stammdaten > Schlüssel > Marktpartner > Vorgangsrabatte > Rabattmethoden > Alle Bezeichnung**

*Abb. B-80 Rabattmethoden*

Dieser Dialog dient zur Bestimmung gültiger Rabattmethoden, die mit unterschiedlichen Merkmalen beschrieben werden und anschließend als Vorgangs- bzw. Marktpartnerspezifische Rabatte definiert werden. In der Rabattmethode werden Informationen hinterlegt, die für die komplette Methode gültig sind.

> **Mehrsprachige Bezeichnungen**
> Seit QR2209 können Sie in A+W Enterprise auch für Rabattmethoden mehrsprachige Bezeichnungen hinterlegen.

### Erläuterung der Felder

**Methode** Methodennummer. Zum Anlegen einer neuen Methode wählen Sie die nächst freie Nummer.
Technische Info: Numerisches Feld, DB-Feld: rabattmeth.methode

**Name** Bezeichnung der Rabattmethode, z. B. Energiezuschlag.
Technische Info: Alphanumerisches Feld, DB-Feld: rabattmeth.methodenname

**Sequenz** Steuert bei mehreren gleichzeitigen Rabatten die Reihenfolge, in der die Rabatte zur Anwendung kommen.
Technische Info: Numerisches Feld, DB-Feld: rabattmeth.seqnr

**Kriterium** In diesem Feld legen Sie fest, welches Vorgangskriterium erfüllt sein muss, damit der Rabatt dieser Methode wirkt:
*   0: Keine Abhängigkeit
*   1: Eilauftrag
*   2: Route
*   3: Versandart
*   4: Verpackungsart
*   5: Lieferart
*   6: Zielland.
*   7: Rechnungsland
*   8: Online
*   9: Speziell
*   10: DFÜ
Technische Info: Numerisches Feld, DB-Feld: rabattmeth.qualfier

**Gutschr.** Mit diesem Feld steuern Sie, wie der Rabatt bei Gutschriften behandelt wird:
*   **Ja:** Der Rabatt wird automatisch in die Gutschriften übernommen.
*   **Nein:** Der Rabatt wird nicht in die Gutschrift übernommen.
*   **Frage:** Sie werden gefragt, ob der Rabatt in die Gutschrift übernommen werden soll.
Technische Info: Toggle-Feld, DB-Feld: rabattmeth.gutschrift

**Gewicht** Mit diesem Feld steuern Sie, wie der Rabatt bei Gutschriften behandelt wird:
*   **Nur fak. GGew:** Der Rabatt bezieht sich nur auf das fakturierte Glasgewicht.
*   **Fak. Glasgew.:** Der Rabatt bezieht sich auf das fakturierte Glasgewicht.
*   **Posgew.:** Der Rabatt bezieht sich auf das Positionsgewicht.
*   **Nur Glasgew.:** Der Rabatt bezieht sich nur auf das Positionsgewicht.
*   **Glasgew.:** Der Rabatt bezieht sich auf das Glasgewicht. Falls dieses aber Null ist, wird Positionsgewicht verwendet.
*   **Fak.Posgew.:** Der Rabatt bezieht sich auf das fakturierte Positionsgewicht.
Technische Info: Toggle-Feld, DB-Feld: rabattmeth.glasgewicht

**Lz.** Mit dieser Checkbox können Sie eine Rabattmethode so kennzeichnen, dass Rabatte dieser Methode bei der Lieferscheinerzeugung deaktiviert werden, wenn es schon einen Lieferschein innerhalb dieser Lieferung gibt.
Technische Info: Toggle-Feld, DB-Feld: rabattmeth.lieferzuschlag

**Rab.** Mit diesem Feld steuern Sie, ob spätere Rabatte auf den Rabatt dieses Rabattes wirken:
*   **Ja:** Der Betrag dieses Rabattes wird in den Grundbetrag nachfolgender Rabatte mit eingerechnet.
*   **Nein:** Der Betrag bleibt unberücksichtigt.
Technische Info: Toggle-Feld, DB-Feld: rabattmeth.rabattierbar

**Nul.** Mit diesem Feld steuern Sie, ob bei Mengenberechnungen Positionen mit einem Betrag von Null berücksichtigt werden:
*   **Ja:** Positionen mit Betrag Null werden berücksichtigt.
*   **Nein:** Positionen werden nicht berücksichtigt.
Technische Info: Toggle-Feld, DB-Feld: rabattmeth.nullpositionen

**All** Mit diesem Feld steuern Sie, ob diese Rabattmethode auf allgemeiner Ebene gepflegt werden kann.
*   **Ja:** Diese Methode kann auf allgemeiner Ebene gepflegt werden.
*   **Nein:** Diese Methode kann nicht auf allgemeiner Ebene gepflegt werden.
Technische Info: Toggle-Feld, DB-Feld: rabattmeth.allgemein

**Mp.** Mit diesem Feld steuern Sie, ob diese Rabattmethode auf Marktpartner-Ebene gepflegt werden kann.
*   **Ja:** Diese Methode kann auf Marktpartner-Ebene gepflegt werden.
*   **Nein:** Diese Methode kann nicht auf Marktpartner-Ebene gepflegt werden.
Technische Info: Toggle-Feld, DB-Feld: rabattmeth.marktpartner

**Obj.** Mit diesem Feld steuern Sie, ob diese Rabattmethode auf Objekt-Ebene gepflegt werden kann.
*   **Ja:** Diese Methode kann auf Objekt-Ebene gepflegt werden.
*   **Nein:** Diese Methode kann nicht auf Objekt-Ebene gepflegt werden.
Technische Info: Toggle-Feld, DB-Feld: rabattmeth.objekt

**Spr** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

## Rabatte

**Stammdaten > Schlüssel > Marktpartner > Vorgangsrabatte > Rabatte**

*Abb. B-81 Rabatte, Register Allgemein*

In den Rabattmethoden werden Informationen hinterlegt, die für die komplette Methode Gültigkeit haben. Diese Rabatte sind nicht als konkrete Rabatte zu verstehen, sondern vielmehr als eine bestimmte Gruppierung von Rabatten, z. B. Energiezuschlag oder Eilzuschlag. Im folgenden wird sprachlich nicht zwischen den Begriffen Zuschlag und Rabatt unterschieden. Es wird der im jeweiligen Zusammenhang verständlichere Begriff verwendet. Die konkreten Rabatte, die allgemein gültig oder marktpartnerabhängig sind, definieren Sie hier:

⇨ "Rabatte" auf Seite B-150

Der Dialog besteht aus den Registern:
*   Allgemein
*   Details

### Erläuterung der Felder

**Methode** Auswahl der Rabattmethode. Die entsprechenden Schlüssel werden über das Menü Rabattmethoden (Schlüssel > Marktpartner > Vorgangsrabatte) vergeben.
Technische Info: <F9>, DB-Feld: rabstamm.methode

**Name** Name der Rabattmethode. Dieser Eintrag kann hier überschrieben werden.
Technische Info: Alphanumerisches Feld, DB-Feld: rabstamm.rabatttext

**Kriterium** Hier wird das für die Methode hinterlegte Kriterium angezeigt.
Technische Info: <F9>, DB-Feld: rabstamm.qualifierwert

**Typ** Typ der Rabattmethode:
*   **Verkauf:** Verkaufsseitiger Rabatt.
*   **Kosten:** Kostenseitiger Rabatt.
*   **Einkauf:** Einkaufsseitiger Rabatt (nur im Menü Einkauf).
Technische Info: Toggle-Feld, DB-Feld: rabstamm.ekvkkz

**Wagrp.** Warengruppe der Rabattmethode. Die Rabattmethode wirkt nur auf die Produkte dieser Warengruppe im Auftrag.
Technische Info: <F9>, DB-Feld: rabstamm.wgrnr

**Wert** Der angegebene Wert wird je nach Rabattart unterschiedlich interpretiert und wird zur Berechnung des Rabattbetrags verwendet.
Technische Info: Numerisches Feld, DB-Feld: rabstamm.wert

**Satzart (Spalte ohne Bezeichnung)** Der angegebene Wert wird je nach Rabattart unterschiedlich interpretiert und wird zur Berechnung des Rabattbetrags verwendet. Mögliche Werte sind:
*   **+:** Zuschlag
*   **-:** Rabatt
Technische Info: Numerisches Feld, DB-Feld: rabstamm.satzart

**Rab.Art** Über die Rabattart wird angegeben, wie der Rabattbetrag berechnet werden soll:
*   **WE:** Fixer Wert
*   **%:** Prozentualer Wert
*   **WE/Stk.:** Wert pro Stück
*   **WE/qm:** Wert pro Quadratmeter Glas
*   **WE/kg:** Wert pro Kilogramm Glas
*   **%/VK:** Kostenrabatt auf Basis des Verkaufsbetrags. Dieser Rabatt wird mit dem Basiswert des Verkaufsbetrages berechnet.
*   **%/Kst:** Verkaufsrabatt auf Basis der Kosten. Dieser Rabatt wird mit dem Basiswert des Kostenbetrages berechnet.
*   **WE/G*E:** Wert pro Gewicht in kg multipliziert mit der Entfernung in km. Dieser Rabatt wird nur dann angewendet, wenn die Entfernung in den Adressen oder im Marktpartner hinterlegt wurde.
Technische Info: Numerisches Feld, DB-Feld: rabstamm.rabattart

**Pos.** Über diese Checkbox steuern Sie, ob der eingegebene Rabatt auf die einzelnen Positionen rückverteilt wird oder nicht.
☑ Der Rabatt wird auf die einzelnen Positionen rückverteilt.
☐ Der Rabatt wird nicht rückverteilt.
Technische Info: Toggle-Feld, DB-Feld: rabstamm.verteil

### Rabatte - Details

**Stammdaten > Schlüssel > Marktpartner > Vorgangsrabatte > Rabatte > Details <F2>**

*Abb. B-82 Rabatte, Register Details*

#### Erläuterung der Felder

**Methode** Auswahl der Rabattmethode. Die entsprechenden Schlüssel werden über das Menü Rabattmethoden (Schlüssel > Marktpartner > Vorgangsrabatte) vergeben.
Technische Info: <F9>, DB-Feld: rabstamm.methode

**Name** Name der Rabattmethode. Dieser Eintrag kann überschrieben werden.
Technische Info: Alphanumerisches Feld, DB-Feld: rabstamm.rabatttext

**Kriterium** Hier wird das für die Methode hinterlegte Kriterium angezeigt.
Technische Info: <F9>, DB-Feld: rabstamm.qualifierwert

**Typ** Typ der Rabattmethode:
*   **Verkauf:** Verkaufsseitiger Rabatt.
*   **Kosten:** Kostenseitiger Rabatt.
*   **Einkauf:** Einkaufsseitiger Rabatt (nur im Menü Einkauf).
Technische Info: Toggle-Feld, DB-Feld: rabstamm.ekvkkz

**Wagrp.** Warengruppe der Rabattmethode. Die Rabattmethode wirkt nur auf die Produkte dieser Warengruppe im Auftrag.
Technische Info: <F9>, DB-Feld: rabstamm.wgrnr

**Rabattwert** Der angegebene Wert wird - je nach Rabattart - unterschiedlich interpretiert und wird zur Berechnung des Rabattbetrages verwendet.
Technische Info: Numerisches Feld, DB-Feld: rabstamm.wert

**Staffelbasis** Auswahl der Staffelbasis. Falls Sie eine Staffelbasis angeben, müssen Sie anschließend über <F5> die Staffelstufen festlegen:
*   qm - Quadratmeter Glas
*   kg - Kilogramm Glas
*   km - Kilometer
*   St - Stück
*   WE - Wert
Technische Info: <F9>, DB-Feld: rabstamm.staffelbasis

**Minimalwert** Minimale Rabattsumme.
Technische Info: Numerisches Feld, DB-Feld: rabstamm.minbetrag

**Maximalwert** Maximale Rabattsumme.
Technische Info: Numerisches Feld, DB-Feld: rabstamm.maxbetrag

> **Minimaler oder Maximaler Betrag nur in 1. Teilvorgang**
> Wenn Zuschläge auf Basis von Qm/kg/Stück/% berechnet werden, für diese außerdem ein minimaler oder maximaler Betrag festgelegt ist, ist es zu empfehlen diese Zuschläge nur als "in 1. Teilvorgang" berechnen lassen. Da durch Grenzbeträge zu Differenzen zwischen dem bestätigten Zuschlag im Auftrag und der Summe der Zuschläge aus den einzelnen Teil-Lieferscheinen kommen kann, sollte der Zuschlag als "nur in den 1. Teilvorgang" definiert und berechnet werden und so nicht mehr in allen restlichen Teilvorgängen berücksichtigt.
>
> ⇨ "Teilvorgang" auf Seite B-232

**Rückverteilen** Rückverteilung des Rabatts auf die Positionen. Durch die Rückverteilung werden die Rabatte auf die jeweilige Position verteilt und vom Programm automatisch an die FIBU übermittelt. Wird keine Rückverteilung verwendet, dann müssen Sie die Rabatte manuell an die FIBU übergeben. Dafür müssen Sie die Angaben aus dem Feld **Stat. Warengruppe** und **Kostenstelle** an die FIBU übermitteln.
☑ Der Rabatt wird auf die einzelnen Positionen rückverteilt.
☐ Der Rabatt wird nicht rückverteilt.
Technische Info: Toggle-Feld, DB-Feld: rabstamm.verteil

**Stat. Warengruppe** Dieses Feld ist nur aktiv, wenn der aktuelle Satz nicht als rückverteilt gekennzeichnet ist. Dann muss hier eine statistische Warengruppe für Statistik-Buchungen angegeben werden.
Technische Info: <F9>, DB-Feld: rabstamm.statwgrnr

**Kostenstelle** Dieses Feld ist nur aktiv, wenn der aktuelle Satz nicht als rückverteilt gekennzeichnet ist. Dann muss hier eine Kostenstelle angegeben werden, auf die gebucht werden soll.
Technische Info: <F9>, DB-Feld: rabstamm.kstelle

**Konto** Dieses Feld ist nur aktiv, wenn der aktuelle Satz nicht als rückverteilt gekennzeichnet ist. Dann muss hier das Konto angegeben werden, auf das gebucht werden soll.
Technische Info: <F9>, DB-Feld: rabstamm.konto

**Rabatt gültig von** Datum, ab dem der Rabatt verwendet werden soll.
Technische Info: Numerisches Feld, DB-Feld: rabstamm.gueltigvon

**Rabatt gültig bis** Datum, bis zu dem der Rabatt verwendet werden soll. Bei entsprechender Systemkonfiguration können Sie bei der Auftragserfassung die Gültigkeits-Prüfung aktivieren. Die Konfiguration lässt folgende Möglichkeiten zu:
*   Es wird geprüft, ob Rabatte in den letzten X Tagen abgelaufen sind (die Anzahl der Tage ist ebenfalls konfigurierbar)
*   Es wird geprüft, ob die Rabatte in der Vergangenheit abgelaufen sind und zusätzlich wird eine Meldung ausgegeben, ob auch Rabatte vorhanden sind, die heute ablaufen.
*   Es wird nur gemeldet, wenn es Rabatte ermittelt werden, die heute ablaufen.
Technische Info: Numerisches Feld, DB-Feld: rabstamm.gueltigbis

**Teilvorgang** Bei Rabatten vom Typ WE muss entschieden werden, wie das Programm bei der Erzeugung von Teillieferscheinen bzw. Teilrechnungen vorgeht. Der Rabatt wird entweder in den ersten Teilvorgang übernommen, in alle Teilvorgänge übernommen oder in einen prozentualen Rabatt umgewandelt. Mögliche Werte sind:
*   **in 1. Tv:** Rabatt wird in den ersten Teilvorgang übernommen.
*   **in alle Tv:** Rabatt wird in alle Teilvorgänge übernommen.
*   **prozentual:** Es erfolgt die Umwandlung in einen prozentualen Rabatt.
Technische Info: Numerisches Feld, DB-Feld: rabstamm.fixerabatte

**Mehrwertsteuer** Auswahl des Mehrwertsteuersatzes. Dieses Feld ist nur aktiv, wenn der aktuelle Satz nicht als rückverteilt gekennzeichnet ist. Die Zuordnung zu den Mehrwertsteuersätzen wirkt sich nur dann aus, wenn die Logik für mehrere Mehrwertsteuern im System aktiviert ist.
Technische Info: <F9>, DB-Feld: rabstamm.steuerzu

**Skontierbar** Die Checkbox ist nur aktiv, wenn Rabatte nicht rückverteilt sind. Das Flag wirkt sich auf Rabatte vom Typ Kosten nicht aus.
☑ Der Rabatt ist skontofähig.
☐ Der Rabatt ist nicht skontofähig.
Technische Info: Toggle-Feld, DB-Feld: rabstamm.skonto

**openTRANS - Id** Dieses Feld ermöglicht die Zuordnung von Rabatten aus Einkaufsvorgängen, die via OpenTRANS empfangen wurden.
Technische Info: Numerisches Feld, DB-Feld: rabstamm.otrabattid

**Verglasung** Das Verglasungskennzeichen wird nur bei prozentualen Rabatten ausgewertet. Dort wird dann als Grundwert die Summe der Verglasungsbeträge der Positionen verwendet. Auf Kostenseite haben Verglasungsrabatte immer einen Betrag von 0.
☑ Der Rabatt bezieht sich nur auf Verglasungen.
☐ Der Rabatt bezieht sich auf alles.
Technische Info: Toggle-Feld, DB-Feld: rabstamm.verglkz

**Glasgewicht** Über dieses Feld können Sie steuern, auf welches Gewicht sich der Rabatt beziehen soll. Diese Information übersteuert die Information aus dem Methodenstamm, so dass Rabatte einer Methode unterschiedliche Bezugsgewichte haben können. Das Glasgewicht beeinflusst den Grundwert des Rabatttyps WE/kg sowie das Ziehen der Staffelstufe innerhalb der Vorgänge.
*   **Posgew.:** Positionsgewicht.
*   **Nur Glasgew.:** Reine Glasgewicht.
*   **Glasgew.:** Glasgewicht
*   **Fak. Posgew.:** Fakturierte Positionsgewicht.
*   **Nur fak. GGew:** Reine fakturierte Glasgewicht.
*   **fak. Glasgew.:** Fakturierte Glasgewicht.
Technische Info: Toggle-Feld, DB-Feld: rabstamm.glasgewicht

**Min. bei Nullbetrag** Über diese Checkbox steuern Sie, ob der Mindestbetrag auch dann gezogen wird, wenn der errechnete Betrag 0.0 WE ist.
☑ Der Rabatt wird auf die einzelnen Positionen zurück verteilt.
☐ Der Rabatt wird nicht auf die einzelnen Positionen zurück verteilt.
Technische Info: Toggle-Feld, DB-Feld: rabstamm.minbeinullbetragk

**Vorgang** Kennzeichen, ob die Stored Procedure rabattanpassung aufgerufen werden muss, die den Rabatt vorgangsindividuell anpasst.
☑ Die SP muss aufgerufen werden.
☐ Die SP wird nicht aufgerufen.
Technische Info: Toggle-Feld, DB-Feld: rabstamm.spaufrufkzkauf

**Position** Kennzeichen, ob die Stored Procedure rabattzuord aufgerufen werden soll, die dann entscheidet, welche Vorgangspositionen von diesem Rabatt berücksichtigt werden und welche nicht.
☑ Die SP wird aufgerufen.
☐ Die SP wird nicht aufgerufen.
Technische Info: Toggle-Feld, DB-Feld: rabstamm.spaufrufkz

**Rabatt-Id Zentrale** Diese Variable steuert die Replikation der Daten aus der Zentrale in die entsprechende Filiale.
Technische Info: Toggle-Feld, DB-Feld: rabstamm.rabattidz

**Rabatt-Id** Eindeutige Zuordnung zum Rabattsatz.
Technische Info: Numerisches Feld, DB-Feld: rabstamm.rabattid

## Hausspezifische Marktpartner-Angaben

**Stammdaten > Schlüssel > Marktpartner > Hausspezifische Angaben**

*Abb. B-83 Hausspezifische Marktpartner-Angaben*

In diesem Dialog können Sie mandantenspezifischen Angaben zu Marktpartnern hinterlegen. Der Dialog ist nur aktiv, wenn Sie mit dem Mehr-Mandantensystem (Multi-Site) arbeiten.

### Erläuterung der Felder

**Partnertyp** Auswahl des Partnertyps.
Technische Info: Toggle-Feld, DB-Feld: mpmdzu.kuliflag

**Marktpartner** Auswahl des Marktpartners.
Technische Info: <F9>, DB-Feld: mpmdzu.mpnr

**Haus** Auswahl der Hausnummer. Der Name wird im Feld dahinter angezeigt.
Technische Info: <F9>, DB-Feld: mpmdzu.hnr

**Vertr.(Erlös)** Auswahl des erlösmäßigen Vertreters. Für den hier eingetragenen Mitarbeiter werden dann die jeweiligen Provisionssätze gebucht und stehen zur Abrechnung bereit. Der Name wird im Feld dahinter angezeigt.
Technische Info: <F9>, DB-Feld: mpmdzu.lager

**Konditionsdebitor** Auswahl der Kundennummer, deren Konditionen für die erfassten Vorgänge gelten soll.
Technische Info: <F9>, DB-Feld: mpmdzu.konddebnr

# Systemschlüssel

**Stammdaten > Schlüssel > System**

Hier werden Werte für verschiedene Bereiche definiert, die später als Auswahl zur Verfügung stehen.
Es werden z. B. die lizenzierten Sprachen eingetragen, die für die Reporterzeugung in verschiedenen Sprachen benötigt werden.
Sie haben Zugriff auf folgende Bereiche:

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a a/b | Position | ⇨ "Positionsbezeichnungen" auf Seite B-238 |
| b | Postleitzahlen | ⇨ "Postleitzahlen" auf Seite B-239 |
| c | Sprachen | ⇨ "Sprachen" auf Seite B-241 |
| d a/b | Textzusätze | ⇨ "Textzusatzbezeichnungen" auf Seite B-244 |
| e | Dokumentenarten | ⇨ "Dokumentenarten" auf Seite B-245 |
| f a/b | Mengeneinheiten | ⇨ "Mengeneinheitenbezeichnung" auf Seite B-247 |
| g a | Modelle - Kantenzuordnung | ⇨ "Kantenzuordnung" auf Seite B-249 |
| g b/c | Modelle | ⇨ "Modellbezeichnungen" auf Seite B-251 |
| h | Produktionsbereich | ⇨ "Produktionsbereich" auf Seite B-253 |
| i a | Versand - Verpackungsart | ⇨ "Verpackungsart" auf Seite B-254 |
| i b | Versand - Gestell-Verpackungsarten | ⇨ "Gestell-Verpackungsarten" auf Seite B-255 |
| i c | Versand - Versandart | ⇨ "Versandart" auf Seite B-256 |
| i d | Versand - Lieferarten | ⇨ "Lieferarten" auf Seite B-258 |
| i e a | Versand - Routen | ⇨ "Routen" auf Seite B-259 |
| i e b | Versand - Tourenplan | ⇨ "Tourenplan" auf Seite B-263 |
| i f a/b | Versand - Versandregionen | ⇨ "Versandregionen-Bezeichnung" auf Seite B-264 |
| i g | Versand - Fahrzeuge | ⇨ "Fahrzeuge" auf Seite B-265 |
| i h | Versand - Ausgangszoll | ⇨ "Ausgangszoll" auf Seite B-266 |
| i i | Versand - Bestimmungszoll | ⇨ "Bestimmungszoll" auf Seite B-268 |
| i j | Versand - Versandgruppen | ⇨ "Versandgruppen" auf Seite B-269 |
| j a/b | Gestellstatus | ⇨ "Gestellstatusbezeichnungen" auf Seite B-270 |
| k a a/b | PMO - Gestellgruppen | ⇨ "Gestellgruppenbezeichnungen" auf Seite B-271 |
| k a a/b | PMO - Verpackungsmethoden | ⇨ "Verpackungsmethodenbezeichnung" auf Seite B-272 |
| k c | PMO - Gestell-Verpackungszuordnung | ⇨ "Gestell-Verpackungszuordnung" auf Seite B-273 |
| l | Währung | ⇨ "Währung" auf Seite B-274 |
| m a | Steuern - Steuertypen | ⇨ "Steuertypen" auf Seite B-277 |
| m b | Steuern - Steuersätze | ⇨ "Steuersätze" auf Seite B-279 |
| n | Zahlungsweise | ⇨ "Zahlungsweisebezeichnungen" auf Seite B-280 |
| o a | Skontogruppen | ⇨ "Skontogruppen" auf Seite B-282 |
| o b/c | Skontogruppenbezeichnungen | ⇨ "Skontogruppenbezeichnung" auf Seite B-284 |
| p | Periodenende | ⇨ "Periodenende" auf Seite B-285 |
| q a/b | Adhocsql - Gruppen | ⇨ "Adhocsql-Gruppenbezeichnungen" auf Seite B-286 |
| r | Report - Texte | ⇨ “Report-Texte" auf Seite B-287 |
| s a | Firmen/Gesellschaften | ⇨ "Firmen / Gesellschaften" auf Seite B-289 |
| s b | Firmen/Gesellschaften - Firmenzuordnung | ⇨ "Firmenzuordnung" auf Seite B-290 |

## Positionsbezeichnungen

**Stammdaten > Schlüssel > System > Position > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > System > Position > Alle Bezeichnungen**

*Abb. B-84 Positionsbezeichnungen*

In diesem Dialog definieren Sie die Positionen der Mitarbeiter im Unternehmen. Sie dienen dann später bei der Stammdatenerfassung als Spezifikation der Mitarbeiterposition.

### Erläuterung der Felder

**Nummer/Nr** Schlüssel-Nummer. Zum Anlegen einer neuen Position geben Sie die nächste freie Nummer ein.
Technische Info: Numerisches Feld, DB-Feld: xsprbez.id
View: xpos.posnr

**Spr** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Bezeichnung** Bezeichnung der Position, z. B. Geschäftsführer.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1
View: xpos.atxt

## Postleitzahlen

**Stammdaten > Schlüssel > System > Postleitzahlen**

*Abb. B-85 Postleitzahlen*

In diesem Dialog können Sie alle Postleitzahlen hinterlegen, die Sie später bei der Auftragserfassung benötigen. Die hier hinterlegten Postleitzahlen erleichtern die Erfassung von Adressen.
Im Bereich Auswahlmenge können Sie Suchkriterien eingeben und somit die Anzahl der Treffer eingrenzen. Ohne Auswahlmenge, werden alle Postleitzahlen angezeigt. * steht für alle Einträge.
Im unteren Bereich können Sie die Angaben korrigieren oder auch neue Einträge hinzufügen.

### Erläuterung der Felder für die Auswahlmenge

**Postleitzahl** Auswahl und Eingabe der Postleitzahl als Suchwert. Sie können die komplette Postleitzahl eingeben oder nur den Anfang. * steht für alle.
Technische Info: <F9>, DB-Feld: xplzk.plz

**Ort** Auswahl und neue Angabe des Ortes als Suchwert. Sie können den kompletten Ort eingeben oder nur den Anfang. * steht für alle.
Technische Info: <F9>, DB-Feld: xplzk.ort

**KFZ Land** Eingabe des KFZ-Landes als Suchwert. Sie können das komplette Land eingeben oder nur den Anfang. * steht für alle.
Technische Info: <F9>, DB-Feld: xplzk.kfz

**Versandregion** Auswahl der Versandregion als Suchwert. Sie können die Versandregion eingeben oder über <F9> auswählen. Versandregionen werden im gleichnamigen Menüpunkt Stammdaten > Schlüssel > System > Versand. -1 steht für keine Auswahl.
Technische Info: <F9>, DB-Feld: xplzk.vsregion

### Erläuterung der Felder für die Treffermenge

**PLZ** Postleitzahl. Zum Anlegen einer neuen Postleitzahl fügen Sie eine neue Zeile ein.
Technische Info: Numerisches Feld, DB-Feld: xplz.plz

**Ort** Der zur Postleitzahl gehörende Ort.
Technische Info: Alphanumerisches Feld, DB-Feld: xplz.ort

**KFZ** Das zur Postleitzahl gehörende Länderkennzeichen.
Technische Info: alphabetisches Feld, DB-Feld: xplz.kfz

**Versandregion** Auswahl der Versandregion mit <F9>. Im Feld dahinter wird die Versandregion angezeigt. Versandregionen werden im gleichnamigen Menüpunkt Stammdaten > Schlüssel > System > Versand.
Technische Info: Numerisches Feld, DB-Feld: xplz.vsregion

## Sprachen

**Stammdaten > Schlüssel > System > Sprachen**

*Abb. B-86 Sprachen*

Dieser Dialog dient zur Verwaltung der lizenzierten Sprachen. Die Sprachen werden über einen Sprachschlüssel definiert. Dieser dient z. B. dazu, Kunden-Reports in Landessprache auszudrucken und jedem Marktpartner seine eigene Sprache zuordnen zu können.
Die Nummer kann frei vergeben werden. In einem Konzern mit mehreren Datenbanken gilt jedoch, dass die Nummernzuordnung einheitlich erfolgen muss.
Das nachfolgende Beispiel soll dies verdeutlichen:
Ein Konzern mit Sitz in Frankreich hat Niederlassungen in Deutschland, England und Italien. Sowohl die Zentrale als auch die Niederlassungen ihrerseits haben Kunden im weiteren europäischen Ausland.

| Niederlassung | hat Kunden in |
| :--- | :--- |
| Zentrale Frankreich | Frankreich, Deutschland, Italien |
| Niederlassung Deutschland | Dänemark, Deutschland, Niederlande |
| Niederlassung England | England |
| Niederlassung Italien | Deutschland, Griechenland, Italien, Slowenien |

*Abb. B-87 Beispiel konzernweite Sprachlizenz*

Um alle Niederlassungen und deren Kunden sprachlich abzudecken, verfügt der Konzern über neun Sprachlizenzen.

> **Landesübergreifende Auftragsübertragung**
> Damit innerhalb des Konzerns eine landesübergreifende Auftragsübertragung möglich ist, muss die Schlüsselnummer einer lizenzierten Sprache konzernweit gleich sein. Die Reportsprachen-Nummer ist abhängig von der Gestaltung der Reports und muss entsprechend abgestimmt werden

Die nachfolgende Tabelle zeigt, wie in der Zentrale und in den Filialen die Sprachen angelegt sein könnten:

| A+W Enterprise Datenbank | hat Kunden in | Lizenzierte Sprachen | Schlüssel-Nr. | Reportsprache |
| :--- | :--- | :--- | :--- | :--- |
| **Zentrale Frankreich** | Frankreich | französisch | 1 | 1 |
| | Deutschland | deutsch | 2 | 2 |
| | Italien | italienisch | 3 | 3 |
| | Spanien | spanisch | 4 | 4 |
| | | dänisch | 5 | |
| | | englisch | 6 | |
| | | griechisch | 7 | |
| | | slowenisch | 8 | |
| | | niederländisch | 9 | |
| **Niederlassung Deutschland** | Dänemark | dänisch | 5 | 1 |
| | Deutschland | deutsch | 2 | 2 |
| | Niederlande | niederländisch | 9 | 3 |
| **Niederlassung England** | England | englisch | 6 | 1 |
| **Niederlassung Italien** | Deutschland | deutsch | 2 | 1 |
| | Griechenland | griechisch | 7 | 2 |
| | Italien | italienisch | 3 | 3 |
| | Slowenien | slowenisch | 8 | 4 |

### Erläuterung der Felder

**Nr.** Sprachkennzeichen. Zum Anlegen eines neuen Sprachkennzeichens wählen Sie die nächst freie Nummer.
Technische Info: Numerisches Feld, DB-Feld: xsprzu.sprkz

**Sprache** Sprachbezeichnung, z. B. Deutsch.
Technische Info: alphabetisches Feld, DB-Feld: xsprzu.atxt

**Reportsprache** Auswahl der Sprache, in der der Report erfolgen soll.
Technische Info: Numerisches Feld, DB-Feld: xsprzu.repsprkz

**A+W Enterprise Sprache** Auswahl der Sprache, in der das Programm angezeigt wird. Im Feld dahinter erscheint die Sprachbezeichnung.
Technische Info: Numerisches Feld, DB-Feld: xsprzu.alenvsprkz

## Textzusatzbezeichnungen

**Stammdaten > Schlüssel > System > Textzusätze > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > System > Textzusätze > Alle Bezeichnungen**

*Abb. B-88 Textzusatzbezeichnungen*

Die Textzusätze dienen der Artikel- und Produktvertextung bei der Auftragserfassung und bei der Erzeugung von Reports.Genaue Verwendung diesen Textzusätzen kann der A+W Enterprise - Konfigurationsanleitung entnommen werden.

### Erläuterung der Felder

**Nummer/Nr** Schlüssel-Nummer. Zum Anlegen eines neuen Textes geben Sie die nächste freie Nummer ein.
Technische Info: <F9>, DB-Feld: xzustxt.txtnr

**Spr** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xzustxt.sprkz

**Textkonstante** Bezeichnung des Textes, z. B. waagerecht.
Technische Info: Alphanumerisches Feld, DB-Feld: xzustxt.zustxt

## Dokumentenarten

**Stammdaten > Schlüssel > System > Dokumentenarten**

*Abb. B-89 Dokumentenarten*

In diesem Dialog können Sie verschiedene Dokumentenarten und die Art der Ausgabe hinterlegen. Für die Leistungserklärung(en) ist der Dokumententyp Leistungserklärung fest definiert und mit der Dokumentenart 1 verknüpft.

Über die Art der Ausgabe kann geregelt werden, ob der Marktpartner die Dokumente der gewählten Art per Email erhalten soll oder nicht. Der Emailversand benötigt weitere systemweite Einstellungen und Konfiguration.

### Erläuterung der Felder

**Art** Schlüsselnummer. Zum Anlegen einer neuen Schlüsselnummer wählen Sie die nächst freie Nummer.
Technische Info: Numerisches Feld, DB-Feld: xdokutype.dokuart

**Bezeichnung** Bezeichnung der Dokumentenart, z. B. Leistungserklärung.
Technische Info: alphabetisches Feld, DB-Feld: xdokutype.dokubez

**Dokumententyp** Zuordnung zu einem Dokumententyp.
Technische Info: alphabetisches Feld, DB-Feld: xdokutype.dokutyp

**Art der Ausgabe** Über dieses Feld steuern Sie die Ausgabeart. Bei der Leistungserklärung ist dieses Feld mit E-Mail vorbelegt:
*   **keine:** Der Marktpartner erhält keine Leistungserklärung.
*   **per E-Mail:** Der Marktpartner erhält die Leistungserklärung per Mail.
Technische Info: Toggle-Feld, DB-Feld: xdokutype.ausgabeart

**VF** Über dieses Feld steuern Sie, ob die Daten in den Vorgang übernommen werden sollen:
☑ Die Daten sollen übernommen werden.
☐ Die Daten sollen nicht übernommen werden.
Technische Info: Toggle-Feld, DB-Feld: xdokutype.vorgangflag

**Prod** Über dieses Feld steuern Sie, ob die Daten an die Produktion übergeben werden sollen:
☑ Die Daten sollen übernommen werden.
☐ Die Daten sollen nicht übernommen werden.
Technische Info: Toggle-Feld, DB-Feld: xdokutype.prodflag

## Mengeneinheitenbezeichnung

**Stammdaten > Schlüssel > System > Mengeneinheiten > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > System > Mengeneinheiten > Alle Bezeichnungen**

*Abb. B-90 Mengeneinheitenbezeichnung*

In diesem Dialog definieren Sie die Mengeneinheiten.

### Erläuterung der Felder

**Nummer/Nr** Auswahl der Schlüssel-Nummer. Zum Anlegen einer neuen Mengeneinheit geben Sie die nächste freie Nummer ein.
Technische Info: <F9>, DB-Feld: xsprbez.id
View: xme.symb

**Spr** Auswahl des Sprachkennzeichens.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**KBez** Kurzbezeichnung der Mengeneinheit, z. B. mtr.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1
View: xme.kurzbez

**Bezeichnung** Bezeichnung der Mengeneinheit, z. B. Meter.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez2
View: xme.atxt

**Dimension** Dimension der Mengeneinheit, z. B. Laufmeter (lfm).
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez3
View: xme.dim

## Kantenzuordnung

**Stammdaten > Schlüssel > System > Modelle > Kantenzuordnung**

*Abb. B-91 Kantenzuordnung*

In diesem Dialog legen Sie fest, wie die Modellkanten bei umschriebenen Rechtecken interpretiert werden. Bei Modell 7 (Bild oben) wird z. B. die schräge Kante als Höhe behandelt.

### Erläuterung der Felder

**Modell** Auswahl der Modellnummer, für die die preisrelevante Kante definiert werden soll. Im Feld dahinter wird die Bezeichnung angezeigt.
Technische Info: <F9>, DB-Feld: modkparam.modnr

**Kante** Für diese Kante soll definiert werden, ob sie als Höhe oder Breite in die Preisberechnung eingehen soll.
Technische Info: Numerisches Feld, DB-Feld: modkparam.kante

**Berechnung** Definiert, wie die Kante in die Preisberechnung eingeht:
*   0: keine Berechnung
*   1: als Höhe
*   2: als Breite
*   3: als Höhe + Breite
*   4: 2x Höhe + Breite
*   5: Höhe + 2x Breite
*   6: 2x Höhe + 2x Breite
Technische Info: Toggle-Feld, DB-Feld: modkparam.berechnung

**MK** Mit diesem Feld wird gesteuert, ob es sich bei der zu bearbeitenden Kante um eine Modellkante handelt.
☑ Bei dieser Kante handelt es sich um eine Modellkante.
☐ Diese Kante ist keine Modellkante.
Technische Info: Alphanumerisches Feld, DB-Feld: modkparam.modellkante

## Modellbezeichnungen

**Stammdaten > Schlüssel > System > Modelle > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > System > Modelle > Alle Bezeichnungen**

*Abb. B-92 Einzelne Modellbezeichnungen / Modellkatalog*

In diesem Dialog hinterlegen Sie die Bezeichnungen zu den zu bearbeitenden Modellen. Die hier für die Modelle hinterlegten Texte werden sowohl in der Auftragserfassung als auch für die Kundenpapiere und für die Erstellung der Scheibenetiketten benötigt.

> **Zur Verfügung stehende Modelle**
> Welche Modelle hier zur Verfügung stehen, ist von der Systemeinstellung Katalogart abhängig.

### Erläuterung der Felder

**Modellnummer/Nr** Auswahl der Modellnummer. Die Modellnummer entspricht den Modellen des A+W Modellkatalogs, bzw. des Modellkatalogs, der bei der Installation eingerichtet wurde.
Technische Info: <F9>, DB-Feld: modelle.modnr

**Sprache** Auswahl des Sprachkennzeichens.
Technische Info: <F9>, DB-Feld: modelle.sprkz

**Bezeichnung** Die Modellbezeichnung entspricht den Modellen des A+W Modellkatalogs, bzw. des Modellkatalogs, der bei der Installation eingerichtet wurde.
Technische Info: Alphanumerisches Feld, DB-Feld: modelle.bez

**Druckbezeichnung** Die Druckbezeichnung kann bei Bedarf geändert werden.
Technische Info: Alphanumerisches Feld, DB-Feld: modelle.drubez

**Erf** Über dieses Feld steuern Sie, ob das Modell erfassbar ist oder nicht. Es kann vorkommen, dass Sie zwar mit dem A+W Modellkatalog arbeiten, die Modell aber nicht bei Ihnen geschnitten werden.
*   **J:** Die Modellnummer kann erfasst werden.
*   **N:** Die Modellnummer kann nicht erfasst werden.
Technische Info: Toggle-Feld, DB-Feld: modelle.erfassbar

**Online** Dieses Feld ist für Online-Erfassungen relevant. Damit steuern Sie, ob das Modell online erfassbar ist oder nicht.
*   **J:** Die Modellnummer kann online erfasst werden.
*   **N:** Die Modellnummer kann nicht online erfasst werden.
Technische Info: Toggle-Feld, DB-Feld: modelle.online

**Kanten** Anzahl der Kanten.
Technische Info: Numerisches Feld, DB-Feld: modelle.kantanz

## Produktionsbereich

**Stammdaten > Schlüssel > System > Produktionsbereich**

*Abb. B-93 Produktionsbereich*

Dieser Dialog dient der Definition einzelner Produktionsbereiche, die in der Auftragserfassung zugeordnet werden können.

### Erläuterung der Felder

**Nr** Nummer des Produktionsbereiches.
Technische Info: Numerisches Feld, DB-Feld: xpbbereich.bereich

**Bereichsbezeichnung** Bezeichnung des Produktionsbereiches, z. B. Siebdruck.
Technische Info: Alphanumerisches Feld, DB-Feld: xpbbereich.bez

## Verpackungsart

**Stammdaten > Schlüssel > System > Versand > Verpackungsart**

*Abb. B-94 Verpackungsarten*

In diesem Dialog legen Sie die Verpackungsarten t in den jeweiligen Sprachen fes. So kann sie auf den Kunden-Papieren in Landessprache ausgewiesen werden.

### Erläuterung der Felder

**Nr** Die Schlüssel-Nummer kann frei gewählt werden. Dieselbe Nummer soll mehrmals vergeben werden, wenn die Verpackungsart in mehreren Sprachen angelegt wird. In diesem Fall bleibt die Nummer gleich, Sprachschlüssel und Bezeichnung ändern sich jeweils.
Technische Info: Numerisches Feld, DB-Feld: xverpack.verpnr

**Bezeichnung** Die Bezeichnung der Verpackungsart.
Technische Info: Alphanumerisches Feld, DB-Feld: xverpack.atxt

**mm** In Abhängigkeit der Konfiguration geben Sie hier die Dicke (in mm) des Verpackungsmaterials zwischen zwei Glasscheiben ein. Die Angabe ist optional.
Technische Info: Numerisches Feld, DB-Feld: xverpack.vdick

**Sprache** Auswahl der Sprache. Im Feld dahinter wird die ausgewählte Sprache angezeigt.
Technische Info: <F9>, DB-Feld: xverpack.sprkz

## Gestell-Verpackungsarten

**Stammdaten > Schlüssel > System > Versand > Gestell-Verpackungsarten**

*Abb. B-95 Gestell-Verpackungsarten*

In diesem Dialog können Sie einer Versandart (z. B. Spedition) in Abhängigkeit des Bestimmungslandes unterschiedliche Verpackungsarten zuweisen. Die Nutzung dieser Funktion ist extra konfigurierbar. Für weitere Information kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

### Erläuterung der Felder

**Versandart** Auswahl der Versandart, z. B. Spedition. Im Feld dahinter wird der Name angezeigt. Die entsprechenden Schlüssel können über das Menü Versandart (Stammdaten > Schlüssel > System > Versand) vergeben werden.
Technische Info: Numerisches Feld, DB-Feld: gverpack.versnr

**KFZ** Auswahl des Länderkennzeichens, z. B. D. Im Feld dahinter wird der Name angezeigt. Die entsprechenden Schlüssel können über das Menü Länder (Stammdaten > Schlüssel > Marktpartner > Länder) vergeben werden.
Technische Info: alphabetisches Feld, DB-Feld: gverpack.kfz

**Verpackungsart** Auswahl der Verpackungsart, z. B. L-Gestelle. Im Feld dahinter wird der Name angezeigt. Die entsprechenden Schlüssel können über das Menü Verpackungsart (Stammdaten > Schlüssel > System > Versand) vergeben werden.
Technische Info: Numerisches Feld, DB-Feld: gverpack.verpnr

**Ergänzende Informationen**
*   "Länder" auf Seite B-204
*   "Verpackungsart" auf Seite B-254
*   "Versandart" auf Seite B-256

## Versandart

**Stammdaten > Schlüssel > System > Versand > Versandart**

*Abb. B-96 Versandarten*

In diesem Dialog legen Sie die Versandarten in den jeweiligen Sprachen fest. So kann die Versandart auf den Kunden-Papieren in Landessprache ausgewiesen werden.

### Erläuterung der Felder

**Nr** Die Schlüssel-Nummer kann frei gewählt werden. Dieselbe Nummer kann mehrmals vergeben werden, wenn die Verpackungsart in mehreren Sprachen angelegt werden soll. In diesem Fall bleibt die Nummer gleich, Sprachschlüssel und Bezeichnung ändern sich jeweils.
Technische Info: Numerisches Feld, DB-Feld: xversand.versnr

**Bezeichnung** Die Bezeichnung der Verpackungsart in der jeweiligen Sprache.
Technische Info: Alphanumerisches Feld, DB-Feld: xversand.atxt

**Route** Die Auswahl einer Route ist optional. Im Feld dahinter wird die Route angezeigt.
Technische Info: <F9>, DB-Feld: xversand.routenr

**Verk** Auswahl des Codes für den Verkehrszweig laut Vorgabe des Statistischen Bundesamtes. Im Feld dahinter wird die Bezeichnung angezeigt.
Technische Info: <F9>, DB-Feld: xversand.intraverkehr

**Transportzuschlag** Der Transportzuschlag in Prozent ist ein Schätzwert, der für die Korrektur des statistischen Wertes benötigt wird.
Technische Info: Numerisches Feld, DB-Feld: xversand.intrasatz

**Sprache** Auswahl der Sprache. Im Feld dahinter wird die ausgewählte Sprache im Klartext angezeigt.
Technische Info: <F9>, DB-Feld: xversand.sprkz

## Lieferarten

**Stammdaten > Schlüssel > System > Versand > Lieferarten > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > System > Versand > Lieferarten > Alle Bezeichnung**

*Abb. B-97 Lieferarten*

Dieser Dialog zeigt Ihnen die definierten Lieferarten, in den jeweiligen Sprachen. So kann sie auf den Kunden-Papieren in Landessprache ausgewiesen werden.

> **Mehrsprachige Bezeichnungen**
> Seit QR2209 können Sie in A+W Enterprise auch für Lieferarten mehrsprachige Bezeichnungen hinterlegen.

### Erläuterung der Felder

**Nr/Lieferart** Die Schlüssel-Nummer kann frei gewählt werden. Dieselbe Nummer kann mehrmals vergeben werden, wenn die Verpackungsart in mehreren Sprachen angelegt werden soll. In diesem Fall bleibt die Nummer gleich, Sprachschlüssel und Bezeichnung ändern sich jeweils.
Technische Info: Numerisches Feld, DB-Feld: xlart.lanr

**Bezeichnung** Die Bezeichnung der Lieferart in der jeweiligen Sprache.
Technische Info: Alphanumerisches Feld, DB-Feld: xlart.labez

**Spr** Auswahl der Sprache (Sprachkennzeichen).
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

## Routen

**Stammdaten > Schlüssel > System > Versand > Routen > Routen > Routenangaben I**
**Stammdaten > Schlüssel > System > Versand > Routen > Routen > Einzelne Bezeichnung**
**Stammdaten > Schlüssel > System > Versand > Routen > Routen > Alle Bezeichnung**

*Abb. B-98 Routen*

In der Routenverwaltung werden die Auslieferungswege beschrieben. So kann bei der Auftragserfassung eine Lieferroute zugeordnet und bei der Berechnung des Liefertermins berücksichtigt werden.

> **Mehrsprachige Bezeichnungen**
> Seit QR2209 können Sie in A+W Enterprise auch für Routen mehrsprachige Bezeichnungen hinterlegen.

### Erläuterung der Felder

**Route** Eindeutige Nummer der Route.
Technische Info: Numerisches Feld, DB-Feld: route.routenr

**Routenbezeichnung** Die Bezeichnung der Route.
Technische Info: Alphanumerisches Feld, DB-Feld: route.routename

**Kürzel** Kürzel der Route.
Technische Info: Alphanumerisches Feld, DB-Feld: route.kurzbez

**Anfahrttage** Auswahl der Anfahrttage (Mo-So).
Technische Info: <F9>, DB-Feld: route.routentag

**Abfahrt** Abfahrtzeit für die Tour.
Technische Info: Numerisches Feld, DB-Feld: route.abfahrt

**AuswR** Die Ausweichroute verweist auf eine andere Zeile derselben Tabelle, in der eine Alternative zur aktuellen Route zu finden ist. Sie wird bei Sperrung dieser Route herangezogen.
Technische Info: Numerisches Feld, DB-Feld: route.aroutenr

**Art** Auswahl der Routenart:
*   **Route:** Tour mit mehreren Anfahrtpunkten.
*   **Direkt:** Ware wird vom Vorlieferanten direkt ausgeliefert.
*   **Abholung:** Ware wird vom Kunden abgeholt.
*   **Rückst.:** Ware befindet sich im Rückstand (Planungsroute).
*   **Intern:** Route zwischen zwei miteinander verbunden Unternehmen (viaPlant).
*   **Spezial:**
*   **Opti:** Optimierungsroute, die bei Verwendung A+W Logistics Optimizer entsteht.
*   **VWB-Direkt:** Routenart für die verlängerten Werkbank
*   **Klärung:** Diese Routenart wird in A+W Enterprise Experience Dispatch verwendet.
Technische Info: <F9>, DB-Feld: route.routenkz

**Haus** Auswahl der Hausnummer, zu der die Route gehört. Das Feld hat folgende Bedeutungen:
*   In einer A+W Enterprise-Instanz, in der mehrere Mandanten verwaltet werden, gibt die Hausnr. an, von welchem Haus aus eine Route gefahren wird.
*   Wird zwischen zwei verbundenen A+W Enterprise-Instanzen ein Auftrag mit Direktauslieferung übertragen, wo wird im empfangenden Haus die Route mit dem eigenen Routenstamm abgeglichen. Es wird diejenige Direktroute ausgewählt, deren Hausnr. mit der Hausnummer des sendenden Hauses übereinstimmt. In diesem Fall gibt die Hausnr. an, für welches Haus eine Direktauslieferung erfolgen soll.
*   Bleibt bei einer Route das Feld leer und das System für globale Routen konfiguriert, so wird diese Route als global bezeichnet. Globale Routen können in allen Häuser verwendet werden, z. B. bei Verschiebung. Es können jedoch keine neue Aufträge auf solche Routen erfasst werden.
Technische Info: <F9>, DB-Feld: route.hausnr

**Reg/Haus** Auswahl der Region, zu der die Route gehört. Die entsprechenden Schlüssel können über das Menü Versandregionen (Schlüssel > System > Versand) vergeben werden.
Technische Info: <F9>, DB-Feld: route.region

**Prio** Eingabe der Priorität innerhalb einer Region für via Plant.
Technische Info: Numerisches Feld, DB-Feld: route.prio

**Zeit** Eingabe der Fahrtzeit in Stunden.
Technische Info: Numerisches Feld, DB-Feld: route.fahrtzeit

**Kal** Mit diesem Feld steuern Sie, ob der Kalender ausgewertet werden soll oder nicht.
☑ Der Kalender wird ausgewertet.
☐ Der Kalender wird nicht ausgewertet.
Technische Info: Toggle-Feld, DB-Feld: route.mitkalender

**Spr** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Ergänzende Informationen**
⇨ "Routenangaben II" auf Seite B-262

## Routenangaben II

**Stammdaten > Schlüssel > System > Versand > Routen > Routen > F2**

*Abb. B-99 Routenangaben*

Die Felder in diesem Dialog sind mit Ausnahme des Feldes Versandart identisch mit den Feldern des Dialogs Routenangaben I.

> **Routenangaben II**
> Das Register Routenangaben II ist standardmäßig ausgeblendet. Die Freischaltung kann über einen Mitarbeiter der A+W Software GmbH erfolgen.

### Erläuterung der Felder

**Versandart** Auswahl der Versandart. Die entsprechenden Schlüssel können über das Menü Versandart (Stammdaten > Schlüssel > System > Versand) vergeben werden. Im weiteren Feld wird die Bezeichnung der Versandart im Klartext dargestellt.
Technische Info: <F9>, DB-Feld: route.versnr

**Ergänzende Informationen**
⇨ "Routen" auf Seite B-259

## Tourenplan

**Stammdaten > Schlüssel > System > Versand > Routen > Tourenplan**

*Abb. B-100 Tourenplan*

In diesem Dialog legen Sie die genauen Abfahrtszeiten für die einzelnen Routen fest. So können Sie z. B. für eine Route, die zwei Mal pro Tag gefahren wird, die unterschiedlichen Abfahrtszeiten definieren. Den Tourenplan können Sie dem Kundenauftrag entsprechend zuordnen.

### Erläuterung der Felder

**Route** Auswahl der Routennummer. Im Feld dahinter wird die ausgewählte Route angezeigt.
Technische Info: <F9>, DB-Feld: tourplan.routenr

**Datum** Datum, an dem die Tour gefahren wird.
Technische Info: Alphanumerisches Feld, DB-Feld: tourplan.tourdate

**Abfahrt** Abfahrtszeit für die Route.
Technische Info: Alphanumerisches Feld, DB-Feld: tourplan.abfahrt

## Versandregionen-Bezeichnung

**Stammdaten > Schlüssel > System > Versand > Versandregionen > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > System > Versand > Versandregionen > Alle Bezeichnungen**

*Abb. B-101 Versandregionen-Bezeichnung*

In diesem Dialog definieren Sie die einzelnen Versandregionen in den verschiedenen Sprachen.

### Erläuterung der Felder

**Nummer** Schlüssel-Nummer. Zum Anlegen einer neuen Versandregion geben Sie die nächste freie Nummer ein.
Technische Info: <F9>, DB-Feld: xsprbez.id

**Sprache** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Bezeichnung** Bezeichnung der Versandregion, z. B. Bayern.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

## Fahrzeuge

**Stammdaten > Schlüssel > System > Versand > Fahrzeuge**

*Abb. B-102 Fahrzeuge*

In diesem Dialog hinterlegen Sie alle Fahrzeuge, die zur Auslieferung der Waren zur Verfügung stehen.

### Erläuterung der Felder

**Fahrzeug** Schlüsselnummer des Fahrzeugs. Zum Anlegen einer neuen Schlüsselnummer wählen Sie die nächst freie Nummer.
Technische Info: Numerisches Feld, DB-Feld: Ikw.lkwnr

**Kennzeichen** Amtliches KFZ-Kennzeichen des Fahrzeugs.
Technische Info: Alphanumerisches Feld, DB-Feld: Ikw.kennz

**Fahrzeugart** Auswahl der Fahrzeugart:
*   LKW
*   Zugmaschine
*   Anhänger
Technische Info: Toggle-Feld, DB-Feld: Ikw.art

**Bezeichnung** Hierbei handelt es sich um eine freie, im Unternehmen gebräuchliche Bezeichnung für das Fahrzeug. Sie erscheint in der Versandsteuerung.
Technische Info: Alphanumerisches Feld, DB-Feld: Ikw.bezeichnung

**Tonnage** Hier wird die Nutzlast des Fahrzeugs eingetragen. Sie dient reinen Informationen und wird nicht ausgewertet.
Technische Info: Numerisches Feld, DB-Feld: Ikw.tonnage

## Ausgangszoll

**Stammdaten > Schlüssel > System > Versand > Ausgangszoll**

*Abb. B-103 Abgangszollstellen*

In diesem Dialog hinterlegen Sie die Abgangszollstellen an den Außengrenzen. Die Nutzung der Ausgang- /Bestimmungszollfunktion ist konfigurationspflichtig. Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

### Erläuterung der Felder

**Nr.** Schlüsselnummer der Zollstelle. Zum Anlegen einer neuen Schlüsselnummer wählen Sie die nächst freie Nummer.
Technische Info: Numerisches Feld, DB-Feld: xazstelle.azsnr

**Ausgangszollstelle** Bezeichnung der Abgangszollstelle gemäß der Zollbestimmungen.
Technische Info: alphabetisches Feld, DB-Feld: xazstelle.bez

**B.-Land** Auswahl des Bestimmungslandes. Im Feld dahinter wird die Bezeichnung angezeigt.
Technische Info: <F9>, DB-Feld: xazstelle.beland

**Zollamtsart** Auswahl der Zollamtsart. Im Feld dahinter wird die Bezeichnung angezeigt:
*   **HZA:** Hauptzollamt
*   **DZA:** Deutsches Zollamt
*   **ZA:** Zollamt
*   **AbfSt:** Abfertigungsstelle
Technische Info: <F9>, DB-Feld: xazstelle.zaart

**Verkehrszw** Auswahl des Verkehrszweiges. Im Feld dahinter wird die Bezeichnung angezeigt:
*   1 - Seeverkehr
*   2 - Eisenbahn
*   3 - Landstraße
*   4 - Luftverkehr
*   5 - Postsendung
*   7 - fest installiert
*   8 - Binnenschifffahrt
*   9 - eigener Antrieb
*   99 - sonstige
Technische Info: <F9>, DB-Feld: xazstelle.vkzweig

## Bestimmungszoll

**Stammdaten > Schlüssel > System > Versand > Bestimmungszoll**

*Abb. B-104 Bestimmungszollstellen*

In diesem Dialog hinterlegen Sie die Bestimmungszollstellen an den Außengrenzen. Die Nutzung der Ausgang-/Bestimmungszollfunktion ist konfigurationspflichtig. Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

### Erläuterung der Felder

**Nr.** Schlüsselnummer der Zollstelle. Zum Anlegen einer neuen Schlüsselnummer wählen Sie die nächst freie Nummer.
Technische Info: Numerisches Feld, DB-Feld: xbzstelle.bzsnr

**KFZ** Auswahl des Landes, in dem die Zollstelle liegt. Im Feld dahinter wird die Bezeichnung angezeigt
Technische Info: <F9>, DB-Feld: xbzstelle.kfz

**Bestimmungszollstelle** Bestimmungszollstelle gemäß den Zollbestimmungen.
Technische Info: alphabetisches Feld, DB-Feld: xazstelle.bez

## Versandgruppen

**Stammdaten > Schlüssel > System > Versand > Versandgruppen**

*Abb. B-105 Versandgruppen*

In diesem Dialog können Sie Versandgruppen definieren. Diese werden in der Versandsteuerung ausgewertet und dienen der Datenselektion.

### Erläuterung der Felder

**Versandgruppe** Schlüsselnummer der Versandgruppe. Zum Anlegen einer neuen Schlüsselnummer wählen Sie die nächst freie Nummer.
Technische Info: Numerisches Feld, DB-Feld: xvsgruppe.vsgruppenr

**Bezeichnung** Die Bezeichnung der Versandgruppe, z. B. ISO-Gruppe.
Technische Info: Alphanumerisches, DB-Feld: xvsgruppe.bez

**Standardgruppe** In diesem Feld definieren Sie, ob es sich bei der Versandgruppe um eine Standardgruppe handelt. Beim Start der Versandsteuerung wird das entsprechende Feld mit diesem Wert belegt.
☑ Bei dieser Versandgruppe handelt es sich um eine Standardgruppe.
☐ Diese Versandgruppe ist keine Standardgruppe.
Technische Info: alphabetisches Feld, DB-Feld: xvsgruppe.stdgruppe

## Gestellstatusbezeichnungen

**Stammdaten > Schlüssel > System > Gestellstatus > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > System > Gestellstatus > Alle Bezeichnungen**

*Abb. B-106 Gestellstatusbezeichnungen*

In diesem Dialog definieren Sie den Status für Gestelle in den verschiedenen Sprachen. Der Gestellstatus wird in der Gestellverwaltung benötigt.

### Erläuterung der Felder

**Nummer/Nr** Schlüssel-Nummer. Zum Anlegen eines neuen Gestellstatus geben Sie die nächste freie Nummer ein.
Technische Info: <F9>, DB-Feld: xsprbez.id

**Sprache** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Bezeichnung** Bezeichnung des Gestellstatus, z. B. verkauft.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

## Gestellgruppenbezeichnungen

**Stammdaten > Schlüssel > System > PMO > Gestellgruppen > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > System > PMO > Gestellgruppen > Alle Bezeichnungen**

*Abb. B-107 Gestellgruppenbezeichnungen*

In diesem Dialog definieren Sie Hauptgruppen für Gestelle in verschiedenen Sprachen. D. h, Sie können Gestelltypen zu Gestellhauptgruppen zusammenfassen.

### Erläuterung der Felder

**Nummer/Nr** Schlüssel-Nummer. Zum Anlegen einer neuen Gestellgruppe geben Sie die nächste freie Nummer ein.
Technische Info: <F9>, DB-Feld: xsprbez.id
View: xghgr.ghgrnr

**Sprache** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Kurzbez.** Die Kurzbezeichnung des Gestellhauptgruppe, z. B. GG.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1
View: xghgr.kurzbez

**Bezeichnung** Die Bezeichnung des Gestellhauptgruppe, z. B. große Gestelle.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez2
View: xghgr.bez

## Verpackungsmethodenbezeichnung

**Stammdaten > Schlüssel > System > PMO > Verpackungsmethoden > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > System > PMO > Verpackungsmethoden > Alle Bezeichnungen**

*Abb. B-108 Verpackungsmethodenbezeichnung*

In diesem Dialog definieren Sie die Verpackungsmethoden in den verschiedenen Sprachen.

### Erläuterung der Felder

**Nummer/Nr** Schlüssel-Nummer. Zum Anlegen einer neuen Verpackungsmethode geben Sie die nächste freie Nummer ein.
Technische Info: <F9>, DB-Feld: xsprbez.id

**Sprache** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Bezeichnung** Bezeichnung der Verpackungsmethode, z. B. PMO1.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

## Gestell-Verpackungszuordnung

**Stammdaten > Schlüssel > System > PMO > Gestell-Verpackungszuordnung**

*Abb. B-109 Gestell-Verpackungszuordnung*

In diesem Dialog können erlaubte Kombinationen aus Gestellgruppen und Verpackungsmethoden hinterlegt werden.

### Erläuterung der Felder

**Nr** Auswahl der Gestellgruppe. Im Feld dahinter wird die Gestellgruppe angezeigt.
Technische Info: <F9>, DB-Feld: pmogestverp.pmogestgrpid

**Nr** Auswahl der Verpackungsmethode. Im Feld dahinter wird die Verpackungsmethode angezeigt.
Technische Info: <F9>, DB-Feld: pmogestverp.pmoverpackid

**Parameter** In diesem Feld hinterlegen Sie die PMO-Parameter für diese Schlüsselkombination. Ein Schlüsselpaar darf jeweils nur einmal existieren.
Technische Info: Alphanumerisches Feld, DB-Feld: pmogestverp.pmoparameter

## Währung

**Stammdaten > Schlüssel > System > Währung > Währung**
**Stammdaten > Schlüssel > System > Währung > Einzelne Bezeichnung**
**Stammdaten > Schlüssel > System > Währung > Alle Bezeichnung**

*Abb. B-110 Währung*

In diesem Dialog pflegen Sie die Währungen und Umrechnungsfaktoren, in denen die Preise angezeigt werden. Die Währung ordnen Sie dem Marktpartner in den Stammdaten > Register Zahlung zu.

> **Voraussetzungen**
> Mit unterschiedlichen Währungen können Sie nur arbeiten, wenn das kostenpflichtiges Modul zur Mehrwährungsfähigkeit konfiguriert ist. Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

> **Mehrsprachige Bezeichnungen**
> Seit QR2209 können Sie in A+W Enterprise auch für Währung mehrsprachige Bezeichnungen hinterlegen.

### Erläuterung der Felder

**Nr** Der Währungsschlüssel wird bei der Definition von Preislisten (PLKZ) benötigt sowie bei der Kunden- und Lieferantenerfassung, um Auftragswerte in der Währung des Kunden ausweisen und berechnen zu können. Zum Anlegen eines neuen Währungsschlüssels geben Sie die nächste freie Nummer ein.
Technische Info: Numerisches Feld, DB-Feld: xwaehr.wnr

**Kürzel** Kürzel der Währung kann frei vergeben werden, z. B. KRW. Es ist jedoch ratsam, die internationale Kennzeichnung der Währung zu verwenden.
Technische Info: Alphanumerisches Feld, DB-Feld: xwaehr.kurzbez

**Bezeichnung** Bezeichnung der Währung kann frei vergeben werden, z. B. Koreanischer Won.
Technische Info: alphabetisches Feld, DB-Feld: xwaehr.bezeichn

**Kurs** Kurs, mit dem Beträge der Landeswährung in die Fremdwährung umgerechnet werden.
Technische Info: alphabetisches Feld, DB-Feld: xwaehr.kurs

**Faktor** Der Kurs multipliziert mit dem Faktor ergibt den eigentlichen Kurs. Das Feld kann zum Austausch mit der Finanzbuchhaltung verwendet werden.
Technische Info: Numerisches Feld, DB-Feld: xwaehr.faktor

**Min. WE** Kleinste Währungseinheit, z. B. 0,01 EUR.
Technische Info: Numerisches Feld, DB-Feld: xwaehr.min_we

**Rundung** Rundungsart:
*   **Keine:** Es erfolgt keine Rundung.
*   **Kau:** Es wird kaufmännisch gerundet.
*   **Auf:** Es wird aufgerundet.
*   **Ab:** Es wird abgerundet.
Technische Info: Toggle-Feld, DB-Feld: xwaehr.we_rund

**Eurofaktor** Umrechnungskurs zum EURO.
Technische Info: Numerisches Feld, DB-Feld: xwaehr.eurokurs

**Still** Währung ist stillgelegt. Eine stillgelegte Währung kann im Marktpartner nicht mehr ausgewählt werden. In den Aufträgen und Rechnungen kann die Währung dennoch verbleiben. Wird ein Vorgang erneut bearbeitet, werden Sie dann aufgefordert, die stillgelegte Währung zu ändern.
*   **Ja:** Die Währung ist stillgelegt, z. B. italienische Lire.
*   **Nein:** Die Währung existiert noch.
Technische Info: Numerisches Feld, DB-Feld: xwaehr.stillkz

**FIBU-Key** Das Feld kann zum Austausch mit der Finanzbuchhaltung verwendet werden.
Technische Info: Numerisches Feld, DB-Feld: xwaehr.fibuschl

**MwSt-Konto** Mehrwertsteuer-Konto. Das Feld kann zum Austausch mit der Finanzbuchhaltung verwendet werden.
Technische Info: Numerisches Feld, DB-Feld: xwaehr.mwstkto

**Erlös-Kto** Erlös-Konto. Das Feld kann zum Austausch mit der Finanzbuchhaltung verwendet werden.
Technische Info: Numerisches Feld, DB-Feld: xwaehr.erloeskto

**Spr** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

## Steuertypen

**Stammdaten > Schlüssel > System > Steuern > Steuertypen > Steuertypen**
**Stammdaten > Schlüssel > System > Steuern > Steuertypen > Einzelne Bezeichnung**
**Stammdaten > Schlüssel > System > Steuern > Steuertypen > Alle Bezeichnung**

*Abb. B-111 Steuertypen*

In diesem Dialog hinterlegen Sie die Steuertypen, die für die Erfassung der Marktpartner und für die Vorgangserzeugung notwendig sind.

> **Mehrsprachige Bezeichnungen**
> Seit QR2209 können Sie in A+W Enterprise auch für Steuertypen mehrsprachige Bezeichnungen hinterlegen.

### Erläuterung der Felder

**Nummer** Nummer des Steuertyps. Zum Anlegen eines neuen Währungsschlüssels wählen Sie die nächst freie Nummer.
Technische Info: Numerisches Feld, DB-Feld: xkukz.kukz

**Spr** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Bezeichnung** Bezeichnung des Steuertyps kann frei vergeben werden, z. B. Ausland (EG).
Technische Info: Alphanumerisches Feld, DB-Feld: xkukz.bez

## Steuersätze

**Stammdaten > Schlüssel > System > Steuern > Steuersätze**

*Abb. B-112 Steuersätze*

In diesem Dialog weißen Sie den einzelnen Steuertypen die entsprechenden Steuersätze zu.

### Erläuterung der Felder

**Nummer** Auswahl des Steuertyps. Im Feld dahinter wird der Steuertyp angezeigt.
Technische Info: <F9>, DB-Feld: xmwst.kukz

**Steuersatz** Hier hinterlegen Sie für den Steuertyp den entsprechenden Steuersatz in Prozent. Sollten Sie mehrerer Steuersätze benötigen, können Sie die Felder Steuersatz 1-3 verwenden.
Technische Info: Numerisches Feld, DB-Feld: xmwst.satz, satz1-3

**gültig ab** Hier hinterlegen Sie, ab wann der Steuersatz für den Steuertyp gültig ist.
Technische Info: Numerisches Feld, DB-Feld: xmwst.giltab

**MwSt-Konto** Mehrwertsteuer-Konto. Das Feld kann zum Austausch mit der Finanzbuchhaltung verwendet werden.
Technische Info: Numerisches Feld, DB-Feld: xmwst.mwstkto

**Vorsteuer-Konto** Vorsteuer-Konto. Das Feld kann zum Austausch mit der Finanzbuchhaltung verwendet werden.
Technische Info: Numerisches Feld, DB-Feld: xmwst.vstkto

## Zahlungsweisebezeichnungen

**Stammdaten > Schlüssel > System > Zahlungsweise > Zahlungsweise**
**Stammdaten > Schlüssel > System > Zahlungsweise > Einzelne Bezeichnung**
**Stammdaten > Schlüssel > System > Zahlungsweise > Alle Bezeichnung**

*Abb. B-113 Zahlungsweisebezeichnungen*

In diesen Dialogen hinterlegen Sie die einzelnen Zahlungsweisen, die in Ihrem Unternehmen vorkommen können.

### Erläuterung der Felder

**Nummer/Nr** Schlüssel-Nummer. Zum Anlegen einer neuen Zahlungsweise geben Sie die nächste freie Nummer ein.
Technische Info: <F9>, DB-Feld: xsprbez.id
View: xzahlm.zmnr

**Spr** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Bezeichnung** Bezeichnung des Zahlungsmerkmals, z. B. Vorauskasse.
Technische Info: alphabetisches Feld, DB-Feld: xsprbez.bez1
View: xzahlm.atxt

**FIBU** Kürzel für die Finanzbuchhaltung.
Technische Info: alphabetisches Feld, DB-Feld: xxzahlm.fib

## Skontogruppen

**Stammdaten > Schlüssel > System > Skontogruppen > Skontogruppen**

*Abb. B-114 Skontogruppen*

In diesem Dialog legen Sie die Skontogruppen an, die Sie den Marktpartnern zuordnen können. Die Gruppen stehen sowohl im Verkauf als auch im Einkauf zur Verfügung und sind dort noch änderbar.

### Erläuterung der Felder

**Zahlungsbedingung** Anzeige der Schlüssel-Nummer. Zum Anlegen eines neuen Ortes geben Sie die nächste freie Nummer ein.
Technische Info: Numerisches Feld, DB-Feld: xxxskonto.zahlbed

**Art** Bezeichnung der Skontoart. Text kann frei eingetragen werden.
Technische Info: Alphanumerisches Feld, DB-Feld: xxxskonto.art

**Monat** Mit diesem Feld steuern Sie, wie viele (volle) Monate zum Rechnungsdatum bzw. zum Fälligkeitsdatum addiert werden.
Technische Info: Numerisches Feld, DB-Feld: xxxskonto.monat

**Frist 1** Falls nötig, kann zusätzlich eine Frist addiert werden. Beispiel: Rechnungsdatum 14.02., Monat = 1, Frist = 15 Tage:
14.02. + 1 Monat = 14.03.
14.03. + 15 Tage = 29.03.
Technische Info: Numerisches Feld, DB-Feld: xxxskonto.frist1

**Legungstag 1-3/Frist 2** Die Legungstage (Legungstag 1 - Legungstag 3) und eine Frist 2 ermöglichen eine Ausweitung des Gültigkeitszeitraumes für den Skontoabzug. Diese Felder müssen nicht zwingend gefüllt sein. Das Legungsdatum 30 entspricht dem Monatsletzten.
Beispiel:
Rechnungsdatum 10.02., Monat = 1, Frist = 10 Tage, Legungsdatum 1 = 15, Legungsdatum 2 = 30:
10.02. + 1 Monat = 10.03.
10.03. + 10 Tage = 20.03.
Die Liste der möglichen Rechnungslegungstage führt zum 31.03. da ausgehend vom 20.3. der nächstmögliche Legungstag ermittelt wird.
31.03. + 5 Tage = 05.04.
Dies bedeutet, dass der Anspruch auf Skontoabzug bis zum 04.04. geltend zu machen ist.
Technische Info: Alphanumerisches Feld, DB-Feld: xxxskonto.rechlegtag1-3, frist2

**Skontosatz** Höhe des gewährten Skontos in Prozent.
Technische Info: Numerisches Feld, DB-Feld: xxxskonto.satz

**Bezeichnung** Definierte Zahlungsbedingung in Worten, z. B. 10 Tage 2 % Skonto.
Technische Info: Alphanumerisches Feld

**Folgebedingung** Die Folgebedingung verweist auf den Schlüssel einer weiteren Skontovereinbarung, die nach Ablauf der Frist für die erste Skontovereinbarung in Kraft tritt.
Technische Info: <F9>, DB-Feld: xxxskonto.folgezahlbed

## Skontogruppenbezeichnung

**Stammdaten > Schlüssel > System > Skontogruppen > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > System > Skontogruppen > Alle Bezeichnungen**

*Abb. B-115 Skontogruppenbezeichnung*

Diese Dialoge enthalten die Skontogruppen in den jeweiligen Sprachen.

### Erläuterung der Felder

**Nummer** Auswahl der Schlüssel-Nummer. Zum Anlegen einer neuen Gruppe geben Sie die nächste freie Nummer ein.
Technische Info: <F9>, DB-Feld: xsprbez.id

**Spr** Auswahl des Sprachkennzeichens.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Bezeichnung** Bezeichnung der Gruppe, z. B. 30 Tage Netto.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

## Periodenende

**Stammdaten > Schlüssel > System > Periodenende**

*Abb. B-116 Periodenende*

Das Periodenende dient in der FIBU als Abgrenzung der Buchungsperiode.

### Erläuterung der Felder

**Periodenende** Datum, an dem die aktuelle Buchungsperiode endet. In Abhängigkeit zur Konfiguration kann hier das EK-Periodenende, das VK-Periodenende oder beides eingetragen werden.
Technische Info: Numerisches Feld, DB-Feld: periode.ek_periode, vk_periode

**Geändert** Datum der Änderung. Das Feld wird automatisch mit dem heutigen Datum gefüllt.
Technische Info: Numerisches Feld, DB-Feld: periode.aenderdat

**Von** Name der Person, der die Änderung durchgeführt hat. Das Feld wird automatisch mit dem Namen der angemeldeten Person gefüllt.
Technische Info: Alphanumerisches Feld, DB-Feld: periode.aendermanr

## Adhocsql-Gruppenbezeichnungen

**Stammdaten > Schlüssel > System > Adhocsql-Gruppen > Einzelne Bezeichnungen**
**Stammdaten > Schlüssel > System > Adhocsql-Gruppen > Alle Bezeichnungen**

*Abb. B-117 Adhocsql-Gruppenbezeichnungen*

In diesen Dialogen legen Sie neue Adhocsql-Gruppen an oder nehmen Änderungen vor. Für diese Gruppen können Sie im Systemmenü <Strg> + <F4> ihre eigene Abfragen hinterlegen.

### Erläuterung der Felder

**Nummer/Nr** Schlüssel-Nummer. Zum Anlegen einer neuen Gruppe geben Sie die nächste freie Nummer ein.
Technische Info: <F9>, DB-Feld: xsprbez.id

**Spr** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Bezeichnung** Bezeichnung der Gruppe, z. B. 30 Tage Netto.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

## Report-Texte

**Stammdaten > Schlüssel > System > Report-Texte**

*Abb. B-118 Report-Texte*

Dieser Dialog zeigt Ihnen alle definierten Texte für Reports, in den jeweiligen Sprachen.

### Erläuterung der Felder

**Typ** Auswahlfeld für den Texttyp, um die Treffermenge zu begrenzen (optional).
Technische Info: Alphanumerisches Feld, DB-Feld: cr_repstrings.type

**Sprache** Auswahlfeld für die Sprache, um die Treffermenge zu begrenzen (optional).
Technische Info: Numerisches Feld, DB-Feld: cr_repstrings.sprkz

**Typ** Schlüsselbezeichnung des Textes. Diese wird im Report zum Referenzieren verwendet.
Technische Info: Numerisches Feld, DB-Feld: cr_repstrings.type

**Sprache** Sprachkennzeichen.
Technische Info: Numerisches Feld, DB-Feld: cr_repstrings.sprkz

**Bezeichnung** Sprachbezeichnung, z. B. englisch.
Technische Info: Numerisches Feld, DB-Feld: cr_repstrings.sprkz

**Text** Name des Reports.
Technische Info: Alphanumerisches Feld, DB-Feld: cr_repstrings.text

**A+W-Flag** Kennzeichen, ob der Text von A+W vorgegeben wird oder nicht.
☑ Der Text wird von A+W vorgegeben.
☐ Der Text wird nicht von A+W vorgegeben.
Technische Info: Alphanumerisches Feld, DB-Feld: cr_repstrings.awflag

## Firmen / Gesellschaften

**Stammdaten > Schlüssel > System > Firmen/Gesellschaften > Firmen/Gesellschaften**

*Abb. B-119 Firmen/Gesellschaften*

Dieser Dialog zeigt Ihnen alle definierten Firmen bzw. Gesellschaften, in den jeweiligen Sprachen. Der Dialog steht Ihnen nur bei der Verwendung der Multi-Site-Funktion. Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

### Erläuterung der Felder

**Firma** Firmen ID. Zum Anlegen einer neuen Firma geben Sie die nächste freie Nummer ein
Technische Info: Numerisches Feld, DB-Feld: xcompany.compid

**Name** Bezeichnung der Firma.
Technische Info: Alphanumerisches Feld, DB-Feld: xcompany.name

**Marktpartner** Auswahl des Marktpartners. Hier werden nur die Sonstigen Marktpartner vorgeschlagen, deren mp.private_long1 ist.
Technische Info: <F9>, DB-Feld: xcompany.mpnr

## Firmenzuordnung

**Stammdaten > Schlüssel > System > Firmen/Gesellschaften > Firmenzuordnung**

*Abb. B-120 Firmenzuordnung*

Hier können Sie den einzelnen Häusern/Mandanten (Tabelle xhaus) eine Firma/Gesellschaft zuordnen. Die Daten werden anschließend in allen Bereichen (Vorgangserfassung, EK, Produktion) ausgewertet, um die richtige Hauszuordnung zu gewährleisten.
In diesem Dialog können keine neuen Häuser erfasst, sondern nur für bestehende Häuser eine Zuordnung vorgenommen werden. Bitte beachten Sie, dass ein Haus ohne Firmenzuordnung als nicht existent gilt.
Der Dialog steht Ihnen nur bei der Verwendung der Multi-Site-Funktion. Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

> **Änderung der Zuordnung**
> Da eine Änderung der Zuordnung massive Folgen für das Vorgangshandling im gesamten System hat, wird bei jeder Änderung eine Sicherheitsabfrage gestellt, ob diese erwünscht ist.

### Erläuterung der Felder

**Nr** Mandantennummer. Der Name wird im Feld dahinter angezeigt.
Technische Info: Anzeige-Feld, DB-Feld:xhaus.name

**Haus** Hausnummer. Der Name wird im Feld dahinter angezeigt.
Technische Info: Anzeige-Feld, DB-Feld:site2comp.hausnr

**Firma** Auswahl der Firma oder Gesellschaft, die dem Mandanten zugeordnet werden soll. Die entsprechenden Schlüssel werden über das Menü Firmen/Gesellschaften (Stammdaten > Schlüssel > System > Firmen/Gesellschaften) vergeben.
Technische Info: <F9>, DB-Feld:site2comp.compid

**Kunde/Lieferant** Anzeige der Kunden- und Lieferantennummer. Diese gelten als interner Marktpartner. Interne Marktpartner müssen unbedingt im Stamm gepflegt werden. Beim Öffnen des Dialogs für diesen Marktpartner im Menü Stammdaten > Marktpartner, ändert sich die Überschrift auf Interne Marktpartner. Auch bei internen Marktpartnern kann ein abweichender FIBU-Debitor hinterlegt werden. Allerdings gelten hier stärkere Restriktionen: zulässig sind nur interne Marktpartner, die zur gleichen Firma/Gesellschaft gehören. Wenn bei einem internen Marktpartner ein abweichender FIBU-Debitor eingetragen wurde, so gilt ab diesem Zeitpunkt auch eine verstärkte Kontrolle bei der Änderung der Firmenzuordnung.
Die Firmenzuordnung eines internen Marktpartners kann nicht geändert werden, wenn der Marktpartner auch anderen internen Marktpartnern als FIBU-Debitor zugeordnet ist. In diesem Fall müssen diese Abhängigkeit zunächst aufgelöst werden (also der FIBU-Debitor der betroffenen anderen internen Marktpartner geändert werden), bevor eine neue Firmenzuordnung stattfinden kann.
Technische Info: Anzeige-Feld, DB-Feld: xhaus.kunr/linr

**Host** Hostname.
Technische Info: Anzeige-Feld, DB-Feld:xhaus.host

# Produktschlüssel

**Stammdaten > Schlüssel > Produkte**

Hier werden alle zulässigen Farben und Maßvarianten hinterlegt. Darüber hinaus ist es möglich, allgemeine Austauschregeln zu bilden, die den Produktaufbau generell verändern.
Für Isoliergläser kann die Ermittlung der technischen Werte über die Produktschlüssel gesteuert werden.
Sie haben Zugriff auf folgende Bereiche:

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a a a | Varianten - Farben | "Farbvarianten" auf Seite B-296 |
| a a b/c | Varianten -Farbbezeichnungen | ⇨ "Farbbezeichnungen" auf Seite B-298 |
| a b a | Maße- Maße | "Maßvarianten" auf Seite B-299 |
| a b b/c | Maße - Maßbezeichnungen | ⇨ "Maßbezeichnungen" auf Seite B-301 |
| a c a | Größen - Größenvarianten | ⇨ "Größenvarianten" auf Seite B-302 |
| a c b/c | Größen - Größenbezeichnungen | ⇨ “Größenbezeichnungen" auf Seite B-303 |
| b | Austausch-/Zusatzregeln | ⇨ "Austausch-/Zusatzregeln" auf Seite B-304 |
| c a | Technische Werte - Gruppen | ⇨ "Untermenü Technische Werte > Gruppen" auf Seite B-294 |
| c b | Technische Werte - Vektoren | "Untermenü Technische Werte > Vektoren" auf Seite B-294 |
| c | Technische Werte - Notifizierungs-stellen | ⇨ "Notifizierungsstellen" auf Seite B-330 |
| d | Technische Werte -Produktnormen | ⇨ "Produktnormen" auf Seite B-331 |
| e | Technische Werte -Prioritäten | ⇨ "Prioritäten" auf Seite B-333 |
| f | Technische Werte -Produkt-kennzeichnung | ⇨ "Produktkennzeichnung (CEKAL)" auf Seite B-334 |
| g | Technische Werte CE-Kennzeichen | ⇨ “CE-Kennzeichen (CPIP)" auf Seite B-336 |
| h | Technische Werte - Leistungserklärung | ⇨ "Leistungserklärung" auf Seite B-336 |
| i | Technische Werte -Produkt-verschlüsselung | ⇨ "Produktverschlüsselung" auf Seite B-338 |
| j | Technische Werte -Produktverwendungszwecke | ⇨ "Bezeichnungen für Produktverwendungszwecke" auf Seite B-341 |
| k | Technische Werte -Parameter-beschreibung | ⇨ "Parameterbeschreibung" auf Seite B-343 |
| l | Technische Werte - Leistungserklärung | ⇨ "Leistungserklärung (Erfassung)" auf Seite B-344 |
| d a/b | Analysegruppen | ⇨ "Bezeichnungen für Analysegruppen" auf Seite B-345 |
| e a/b/c | Beschlagstypen | ⇨ "Bezeichnungen für Beschlagstypen" auf Seite B-346 |
| f a/b | Folientypen | ⇨ "Bezeichnungen für Folientypen" auf Seite B-348 |
| g | Produktionstypen | ⇨ "Produktionstypen" auf Seite B-349 |
| h a/b/c | Rahmentypen | ⇨ "Bezeichnungen für Rahmentypen" auf Seite B-350 |
| i a/b | Versiegelungstypen | ⇨ "Bezeichnungen für Versiegelungstypen" auf Seite B-352 |
| j | Motive | ⇨ "Motivzuordnung" auf Seite B-353 |
| k | Stapel | Hierbei handelt es sich um eine kundenspezifische Funktion, die nicht Bestandteil des Handbuches ist. |
| l a/b | Kistensignatur | ⇨ "Bezeichnungen für Kistensignatur" auf Seite B-355 |
| m | Shaping/Nesting-Artikel | ⇨ "Shaping/Nesting-Artikel" auf Seite B-357 |
| n | Template Parameter | ⇨ "Template Parameter" auf Seite B-358 |
| o | ITOE - Austauschregeln | ⇨ "¡TOE-Austauschregeln" auf Seite B-359 |
| p | Bemaßungsset | Hierbei handelt es sich um eine kundenspezifische Funktion, die nicht Bestandteil des Handbuches ist. |
| q | Kundenprodukte | ⇨ “Kundenprodukte" auf Seite B-362 |
| r | Bestellte Bearbeitungen | ⇨ "Bestellte Bearbeitungen" auf Seite B-364 |
| s | Hausspezifische Angaben | ⇨ "Hausspezifische Angaben" auf Seite B-366 |
| t | VSG/GH Vererbung | ⇨ "VSG/GH Vererbung" auf Seite B-367 |
| u | A+W iQuote - spezifische Angaben | ⇨ "Untermenü A+W iQuote-spezifische Angaben" auf Seite B-295 |

## Untermenü Technische Werte > Gruppen

**Schlüssel > Produkte > Technische Werte > Gruppen**
Über dieses Menü legen Sie Gruppen, die für die Beschreibung der technischen Werte notwendig sind, fest.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Schalldämmung | ⇨ "dB-Gruppen" auf Seite B-312 |
| b | Thermische Eigenschaften | ⇨ "U-Gruppen" auf Seite B-313 |
| c | Gesamtenergiedurchlass | ⇨ "g-Gruppen" auf Seite B-314 |
| d | Transmission | ⇨ "Transmissionsgruppen" auf Seite B-315 |
| e | Maßrestriktionen | ⇨ "Maßrestriktions-Gruppen" auf Seite B-316 |
| f | Dicken | ⇨ "Dickengruppen" auf Seite B-317 |
| g | Biegefestigkeit) | ⇨ "Biegefestigkeitsgruppen" auf Seite B-318 |

## Untermenü Technische Werte > Vektoren

**Schlüssel > Produkte > Technische Werte > Vektoren**
Über dieses Menü legen Sie Vektoren, die für die Beschreibung der technischen Werte notwendig sind, fest.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Schalldämmung | ⇨ "Vektoren für Schalldämmung (dB)" auf Seite B-319 |
| b | Thermische Eigenschaften | ⇨ "Vektoren für thermische Eigenschaften (U)" auf Seite B-321 |
| c | Gesamtenergiedurchlass | ⇨ "Vektoren für Gesamtenergiedurchlass (g)" auf Seite B-323 |
| d | Transmission | ⇨ "Vektoren für Transmission" auf Seite B-325 |
| e | Maßrestriktionen | ⇨ "Vektoren für Maßrestriktionen" auf Seite B-327 |
| f | Windlast | ⇨ "Vektoren für Windlast" auf Seite B-329 |

## Untermenü A+W iQuote-spezifische Angaben

**Schlüssel > Produkte > A+W iQuote-spezifische Angaben**
Über dieses Menü pflegen Sie Stammdaten, die für das Arbeiten mit A+W iQuote notwendig sind. Wenn Sie Information über dieses Produkt brauchen, kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Artikelgruppen | ⇨ "Artikelgruppen-Bezeichnungen" auf Seite B-368 |
| b | Bearbeitungszuordnung | ⇨ "Bearbeitungszuordnung" auf Seite B-369 |
| c | Bearbeitung für Modellkanten | ⇨ "Bearbeitungen für Modellkanten" auf Seite B-372 |
| d | Austauschgruppen | ⇨ "Austauschgruppen-Bezeichnungen" auf Seite B-374 |
| d c | Gruppenzuordnung (Artikel) | ⇨ "Gruppenzuordnung (Artikel)" auf Seite B-375 |
| d d | Gruppenzuordnung (Rahmen) | ⇨ "Gruppenzuordnung (Rahmen)" auf Seite B-376 |

## Farbvarianten

**Stammdaten > Schlüssel > Produkte > Varianten > Farben > Farben**

*Abb. B-121 Farben*

Alle Farben, die im Artikelstamm und später in der Auftragserfassung benötigt werden, müssen hier angelegt werden.

### Erläuterung der Felder

**Nummer** Nummer der Farbe.
Technische Info: Numerisches Feld, DB-Feld: xxfarbe.farbnr

**Bezeichnung** Bezeichnung der Farbe.
Technische Info: Alphanumerisches Feld, DB-Feld: xcompany.name

**RAL-Nummer** RAL-Nummer der Farbe.
Technische Info: Numerisches Feld, DB-Feld: xxfarbe.ralnr

**AWDesign-Farbcode** A+W Farbcode, der im CAD Designer (Bars) benötigt wird.
Technische Info: Alphanumerisches Feld, DB-Feld: xxfarbe.awfarbcode

**RGB-Bezeichnung** RGB-Farbname.
Technische Info: Alphanumerisches Feld, DB-Feld: xxfarbe.rgbname

**Rot** Anteil Rot für RGB-Farbdefinition.
Technische Info: Numerisches Feld, DB-Feld: xxfarbe.farbe_r

**Grün** Anteil Grün für RGB-Farbdefinition.
Technische Info: Numerisches Feld, DB-Feld: xxfarbe.farbe_g

**Blau** Anteil Blau für RGB-Farbdefinition.
Technische Info: Numerisches Feld, DB-Feld: xxfarbe.farbe_b

**Ergänzende Informationen**
⇨ "Farbbezeichnungen" auf Seite B-298

## Farbbezeichnungen

**Stammdaten > Schlüssel > Produkte > Varianten > Farben > Einzelne Bezeichnung**
**Stammdaten > Schlüssel > Produkte > Varianten > Farben > Alle Bezeichnung**

*Abb. B-122 Einzelne Farben*

In diesem Dialog definieren Sie die einzelnen Farben in den verschiedenen Sprachen.

### Erläuterung der Felder

**Nummer** Schlüssel-Nummer. Zum Anlegen einer neuen Farbe geben Sie die nächste freie Nummer ein.
Technische Info: <F9>, DB-Feld: xsprbez.id

**Spr** Sprachkennzeichen.
Technische Info: <F9>, DB-Feld: xsprbez.sprkz

**Bezeichnung** Farbbezeichnung, z. B. weiß.
Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1

## Maßvarianten

**Stammdaten > Schlüssel > Produkte > Varianten > Maße > Maße**

*Abb. B-123 Maße*

In diesem Dialog werden alle Maßvarianten, abhängig von der Mengeneinheit gepflegt. Im Artikelstamm werden dann diese Maßvarianten zugeordnet. Die Maßvarianten sind auch Grundlage für die Lagerwirtschaft.

### Erläuterung der Felder

**Nr** Die Varianten-Nr ist der eindeutige Schlüssel innerhalb der jeweiligen Mengeneinheit (ME). Sie wird sowohl im Artikelstamm als auch im Rahmen der Auftragserfassung zur Identifikation der gewünschten Variante genutzt.
Technische Info: Numerisches Feld, DB-Feld: xxvar.bitnr

**ME** Auswahl der Mengeneinheit. Die Schlüssel werden im Menü Mengeneinheiten (Schlüssel > System) hinterlegt.
Technische Info: <Selo>-Feld, DB-Feld: xxvar.meh

**Bezeichnung** Bezeichnung der Maßvariante kann frei gewählt werden.
Technische Info: Alphanumerisches Feld

**Lagerbez.** Bezeichnung eines Stückes im Lager kann frei gewählt werden.
Technische Info: Alphanumerisches Feld

**Teilmaße 1-3** Länge, Breite und Höhe werden in der jeweils kleinsten sinnvollen Einheit angegeben. Sie werden bei der Auftragserfassung automatisch eingeblendet.
Technische Info: Numerisches Feld, DB-Feld: xxvar.mas1, mas2, mas3

**Gesamtmaß** Das Gesamtmaß gibt die Gesamtgröße der Variante in der jeweiligen Systemgrundeinheit an. In der Auftragserfassung wird das Gesamtmaß gemäß des hier eingetragenen Umrechnungsfaktors berechnet.
Technische Info: Numerisches Feld, DB-Feld: xxvar.faktor

**Ergänzende Informationen**
⇨ "Mengeneinheitenbezeichnung" auf Seite B-247
