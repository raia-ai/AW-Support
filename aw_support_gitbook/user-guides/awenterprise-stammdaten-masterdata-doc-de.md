---
title: "DE_AWEnterprise_Stammdaten_3.00"
source: "DE_AWEnterprise_Stammdaten_3.00.pdf"
tags: ["A+W Enterprise", "Stammdaten", "master data", "ERP", "glass industry", "windows", "doors", "software manual", "technical documentation", "Marktpartner"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document is a comprehensive user manual for the Master Data (Stammdaten) module of the A+W Enterprise software, version 3.0. It provides detailed descriptions of the various dialogs, functions, and data fields for managing core business data within the system."
long_description: "This technical documentation serves as a complete software reference guide for the 'Stammdaten' (Master Data) module of the A+W Enterprise software, a specialized ERP solution for the glass, windows, and doors industry. The manual is intended for end-users and administrators responsible for maintaining the foundational data that underpins the entire system. It covers the creation, management, and configuration of key data entities, including Market Partners (customers, suppliers), Articles (products), Employees, and various system-wide keys and parameters. The document is structured to follow the software's menu layout, providing detailed explanations for each section, such as Marktpartner (Market Partners), Artikel (Articles), Stückliste (Bill of Materials), and Warengruppen (Product Groups). It includes step-by-step guidance on navigating dialogs, context menus, and registers (tabs), explaining the purpose and technical details of each field. Special attention is given to configurations, pricing, conditions, and the interdependencies between different data sets. This manual is an essential tool for ensuring data integrity and leveraging the full functionality of the A+W Enterprise system."
---

# A+W Stammdaten B

---
## Vorspann
In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version / Datum | Beschreibung |
| :--- | :--- |
| 3.0 / 02-2023 | Erweitert um neue Dialoge im Bereich Schlüssel |
| 2.2 / 03-2022 | Feldbeschreibung in den Bereichen Marktpartner, Artikel, Anmerkungen und Rabatte aktualisiert |
| 2.1 / 11-2020 | Vollständige Überarbeitung |
| 1.11 / 08-2013 | Umsetzung auf CI 2013. |
| 1.10 / 01-2010 | Neu: Kapitel Preise und Konditionen. |
| 1.00 / 10-2006 | Ersterstellung. |

### Editorial
Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen
- Kontakte

#### Anmerkungen zu diesem Dokument
Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Enterprise gedacht.

Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden.

Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. Die A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.

Die Beschreibungen in dieser Dokumentation beruhen auf der vollen Ausbaustufe von A+W Enterprise.

#### Urheberrechte
© 2023, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

#### Warenzeichen
Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

#### Kontakte
**A+W Software GmbH**
Am Pfahlgraben 4-10
35415 Pohlheim
+49 6404 2051-0
+49 6404 2051 877
Zentrale@a-w.com
http://www.a-w.com

## Inhalt

- **Vorspann**
    - Revisionsübersicht
    - Editorial
- **Softwarereferenz**
    - **Stammdaten - Übersicht**
    - **Marktpartner**
        - Marktpartner-Kopf
        - Marktpartner - Kontextmenü
        - Marktpartnersuche
        - Register Adresse
        - Marktpartner - Anmerkungstexte
        - Register Identifikation
        - Register Bezüge
        - Register Auftrag
        - Register Lieferung
        - Register Rechnung
        - Register Kundenspezifisch
        - Register Zahlung
        - Register Ausdruck
        - Register Limits
        - Register Bewertung
        - Register Produktion
        - Register Modifikation
        - Register Privat
        - Ansprechpartner
        - Adressen
        - Hausspezifische Adressdaten
        - Bankverbindungen
        - E-Mailadressen
        - E-Mailadressen - Detail
        - Rabatte
        - Rabatte Details
        - Austausch-/Zusatzregeln
        - Gestelltypen
        - Gestelltypen - Details
        - Konfigurierte MP-Felder
        - Vertreterzuordnung
        - Erfasserzuordnung
        - Gruppenzuordnung
        - Objektzuordnung
        - Objekttexte
        - Farbzuordnung
        - Bonuszuordnung
        - Artikelzuordnung
        - Marktpartnertexte
        - Stammtexte
        - Marktpartner-Artikeltexte
        - Formulare
        - Dokumentenarten
        - Vorgangs-Recherche
        - Marktpartner-Info
        - Replikationsdaten
        - DFÜ-Konfiguration
        - Hausspezifische Angaben
    - **Mitarbeiter**
        - Mitarbeiter / Berechtigungsgruppen
        - Mitarbeiter - Rechte
    - **Abteilungen**
    - **Marktpartnerschlüssel**
        - Anreden-Bezeichnungen
        - Bonus
        - Gruppen
        - Gruppenbezeichnungen
        - Branchenbezeichnungen
        - Kalender
        - Etikettentexte
        - Spezielle Kalender
        - Kundenkalender
        - Mandantenkalender
        - FIBU-Mandanten
        - Länder
        - Wirtschaftsraumbezeichnungen
        - Regionen / Bundesländerbezeichnungen
        - Allgemeine Qualitätsskala
        - Termin-Qualitätsskala
        - Preise-Qualitätsskala
        - Mengen-Qualitätsskala
        - Spezial-Qualitätsskala
        - Reklamationsgründe
        - Reklamationsorte
        - Reklamationstypen
        - Rabattmethoden
        - Rabatte
        - Rabatte - Details
        - Hausspezifische Marktpartner-Angaben
    - **Systemschlüssel**
        - Positionsbezeichnungen
        - Postleitzahlen
        - Sprachen
        - Textzusatzbezeichnungen
        - Dokumentenarten
        - Mengeneinheitenbezeichnung
        - Kantenzuordnung
        - Modellbezeichnungen
        - Produktionsbereich
        - Verpackungsart
        - Gestell-Verpackungsarten
        - Versandart
        - Lieferarten
        - Routen
        - Routenangaben II
        - Tourenplan
        - Versandregionenbezeichnung
        - Fahrzeuge
        - Ausgangszoll
        - Bestimmungszoll
        - Versandgruppen
        - Gestellstatusbezeichnungen
        - Gestellgruppenbezeichnungen
        - Verpackungsmethodenbezeichnung
        - Gestell-Verpackungszuordnung
        - Währung
        - Steuertypen
        - Steuersätze
        - Zahlungsweisebezeichnungen
        - Skontogruppen
        - Skontogruppenbezeichnung
        - Periodenende
        - Adhocsql-Gruppenbezeichnungen
        - Report-Texte
        - Firmen / Gesellschaften
        - Firmenzuordnung
    - **Produktschlüssel**
        - Untermenü Technische Werte > Gruppen
        - Untermenü Technische Werte > Vektoren
        - Untermenü A+W iQuote-spezifische Angaben
        - Farbvarianten
        - Farbbezeichnungen
        - Maßvarianten
        - Maßbezeichnungen
        - Größenvarianten
        - Größenbezeichnungen
        - Austausch-/Zusatzregeln
        - Austausch-/Zusatzregel - Details
        - Austausch-/Zusatzregel - Testmodus
        - dB-Gruppen
        - U-Gruppen
        - g-Gruppen
        - Transmissionsgruppen
        - Maßrestriktions-Gruppen
        - Dickengruppen
        - Biegefestigkeitsgruppen
        - Vektoren für Schalldämmung (dB)
        - Vektoren für thermische Eigenschaften (U)
        - Vektoren für Gesamtenergiedurchlass (g)
        - Vektoren für Transmission
        - Vektoren für Maßrestriktionen
        - Vektoren für Windlast
        - Notifizierungsstellen
        - Produktnormen
        - Prioritäten
        - Produktkennzeichnung (CEKAL)
        - CE-Kennzeichen (CPIP)
        - Leistungserklärung
        - Produktverschlüsselung
        - Bezeichnungen für Produktverwendungszwecke
        - Parameterbeschreibung
        - Leistungserklärung (Erfassung)
        - Bezeichnungen für Analysegruppen
        - Bezeichnungen für Beschlagstypen
        - Bezeichnungen für Folientypen
        - Produktionstypen
        - Bezeichnungen für Rahmentypen
        - Bezeichnungen für Versiegelungstypen
        - Motivzuordnung
        - Stapel
        - Bezeichnungen für Kistensignatur
        - Shaping/Nesting-Artikel
        - Template Parameter
        - ¡TOE-Austauschregeln
        - Bemaßungsset
        - Kundenprodukte
        - Bestellte Bearbeitungen
        - Hausspezifische Angaben
        - VSG/GH Vererbung
        - Artikelgruppen-Bezeichnungen
        - Bearbeitungszuordnung
        - Bearbeitungszuordnung - Details
        - Bearbeitungen für Modellkanten
        - Austauschgruppen-Bezeichnungen
        - Gruppenzuordnung (Artikel)
        - Gruppenzuordnung (Rahmen)
    - **Artikel**
        - Artikel-Kopf
        - Artikel - Kontextmenü
        - Identifikation
        - Artikel - Anmerkungstexte
        - Physikalische Eigenschaften
        - Maßrestriktionen
        - Einbaurestriktionen
        - Beschaffung
        - Produktion
        - Preise
        - Lager
        - Technische Werte
        - Statistik
        - Modifikation
        - Privat
        - Lieferanten - Zuordnung
        - Marktpartnerangaben
        - Maßvarianten
        - Maßvarianten - Details
        - Farben- / Größenvarianten
        - Farben- / Größenvarianten - Details
        - Zwingende Maßangaben – Маßparameter-Auswahl
        - Zwingende Maßangaben – Ansicht 1
        - Zwingende Maßangaben – Ansicht 2
        - Defaultwertberechnung
        - Artikel-Vermaßung – Maßparameter
        - Artikel-Vermaßung – Texte
        - Artikel-Vermaßung - Positionsmaße
        - Artikel-Vermaßung - Sonstige Parameter
        - Modell-Vermaßung
        - Produktbemaßung löschen
        - Stückliste
        - Stücklisten-Restriktionen
        - Preiseigenschaften
        - Weitere Artikelbezeichnungen
        - Artikeltexte
        - Kunden-Artikeltexte
        - Objekt-Artikeltexte
        - Formulare
        - Stammtexte - Texteditor
        - Beschaffungsarten
        - Artikel an A+W CAD Designer (Bars) senden
        - Beschlagartikel-Abgleich
        - Replikationsdaten
        - Produktkennzeichnung
        - Technische Werte
        - Deklarierte Leistungen
        - Konfigurierte Felder
        - Artikelbilder
        - Hausspezifische Artikel-Angaben
        - Hausspezifische Artikelangaben – Details
        - Hausspezifische Lieferanten-Angaben
        - Hausspezifische Varianten-Angaben
        - Hausspezifische Farben/Größen-Angaben
    - **Stückliste**
        - Stückliste
        - Formeleditor
    - **Warengruppen**
        - Warengruppen
        - Einzelne Warengruppen
        - Hausspezifische Warengruppen
    - **Fertige Produkte**
        - Produktfixierung
        - Produktset
    - **Feldkonfiguration**
        - MP-Feldkonfiguration
        - Artikel-Feldkonfiguration
        - Vorgangs-Feldkonfiguration
        - Konfiguration Bezugnahme
    - **Provisionen**
        - Provisionskürzel
        - Provisionszuordnung
    - **Textverwaltung**
        - Aktuelle Texte
        - Gruppentexte
        - Objekttexte
        - Warengruppentexte
        - Konfigurierbare Texte
        - Floskeln
        - Variablenbezeichnung
        - Textformeln
    - **Kostenstamm**
        - Kostenarten
        - Kostenträger
        - Kostenstellen
    - **Preise**
    - **Konditionen**
    - **Listendruck**
- **Partindex**
- **Index**

# Softwarereferenz
## Stammdaten – Übersicht
Stammdaten sind zeitunabhängige Daten, die nie bzw. nur selten verändert werden. Sie sind der Dreh- und Angelpunkt des gesamten Systems, da Bezüge zu allen anderen Bereichen bestehen. Ziel der Stammdatenverwaltung ist es, einen einzigen, durchgängigen Datenbestand für alle im Einsatz befindlichen Anwendungen zu schaffen.

Alle Dialoge und Funktionen, die die Stammdaten betreffen, befinden sich in diesem Menü:

| Short Cut | Beschreibung |
| :--- | :--- |
| a | ⇨ "Marktpartner" auf Seite B-14 |
| b | ⇨ "Mitarbeiter" auf Seite B-92 |
| c | ⇨ "Abteilungen" auf Seite B-100 |
| da | ⇨ "Marktpartnerschlüssel" auf Seite B-102 |
| db | ⇨ "Systemschlüssel" auf Seite B-152 |
| dc | ⇨ "Produktschlüssel" auf Seite B-208 |
| dd | ⇨ Preisschlüssel finden Sie in einem separaten Dokument |
| e | ⇨ "Artikel" auf Seite B-293 |
| f | ⇨ "Stückliste" auf Seite B-400 |
| g | ⇨ "Warengruppen" auf Seite B-406 |
| h | ⇨ "Fertige Produkte" auf Seite B-412 |
| i | ⇨ "Feldkonfiguration" auf Seite B-416 |
| k | ⇨ "Provisionen" auf Seite B-425 |
| l | ⇨ "Textverwaltung" auf Seite B-428 |
| m | ⇨ "Kostenstamm" auf Seite B-437 |
| n | ⇨ "Preise" auf Seite B-443 |
| o | ⇨ "Konditionen" auf Seite B-444 |
| p | ⇨ "Listendruck" auf Seite B-445 |

> **Preise und Konditionen**
> Die Themen Preise, Konditionen und Listendruck sind in einem getrennten Dokument beschrieben!

## Marktpartner
Im Marktpartnerstamm werden alle kunden-, objekt- und lieferantenbezogenen Angaben hinterlegt sowie Einmal-Daten (Partnertyp Sonstiger).
Die Angaben reichen von der Erfassung der Firmenadresse bis hin zu Lieferanschriften, Routen, Zahlungskonditionen und Bewertungen.

### Marktpartner-Kopf
Nachdem Sie den Dialog geöffnet haben, müssen Sie zunächst im Kopfbereich den Marktpartner auswählen.
Die Inhalte der einzelnen Register beziehen sich immer auf den im Kopf gewählten Marktpartner.
Im A+W Enterprise werden folgende Marktpartnertypen unterschieden:
- Kunde
- Lieferant
- Sonstiger
- Objekt
- Eigentümer (Gestelle)

**Partnertyp**
Toggle-Feld für Marktpartnertyp. Folgende Auswahlmöglichkeiten stehen zur Verfügung:
- **Kunde:** Im Kundenstamm sind alle kundenbezogenen Angaben enthalten, inklusive der kundenindividuellen Artikeldefinitionen. Marktpartner vom Typ Kunde benötigen Sie vor allem in der Erfassung von Verkaufsvorgängen.
- **Lieferant:** Im Lieferantenstamm werden alle lieferantenbezogenen Angaben hinterlegt inklusive lieferantenindividueller Artikelangaben. Marktpartner vom Typ Lieferant benötigen Sie vor allem in der Erfassung von Einkaufsvorgängen. Lieferanten können direkt in Aufträgen und im Artikelstamm als Lieferanten für zu bestellende Artikel eingegeben werden.
- **Sonstiger:** Unter diesem Typ werden gewöhnlich Einmal-Kunden geführt, für die dann auch nur die Adresse angelegt wird. Innerhalb der erweiterten internen Mandantentrennung werden die Firmen als Sonstiges angelegt.
- **Objekt:** Unter einem Objekt wird üblicherweise ein größeres Bauvorhaben (Projekt) verstanden. Unter diesem Oberbegriff werden Definitionen technischer Art, Konditionen preislicher Art (EK und VK) und weitere geschäftliche Vereinbarungen (Mengen, Zeiten etc.) zusammengefasst. Hierzu kommt eine Planungs- und eine Informationskomponente. Objekte können Marktpartnern, Verkaufs- und Einkaufsvorgängen zugeordnet werden.
- **Eigentümer:** Eigentümer für Gestelle.
  *Technische Info: Toggle-Feld, DB-Feld: mp.kuliflag*

**Marktpartner**
Auswahl der Nummer oder wenn bekannt, Eingabe derselben. Soll ein neuer Marktpartner angelegt werden, drücken Sie `<F6>`.
⇨ "Marktpartnersuche" auf Seite B-17
*Technische Info: `<F9>`, DB-Feld: mp.kunr*

**Matchcode**
Bei der Wahl eines bestehenden Marktpartners wird der Matchcode angezeigt und bei der Erfassung eines neuen Marktpartners muss man einen Matchcode eingeben. Der Matchcode ist ein freies Textfeld in dem eine Kurzbezeichnung für den Marktpartner eingegeben wird. Der Matchcode dient vor allem der vereinfachten Suche.

### Register
Der Dialog beinhaltet verschiedene Register. Die Inhalte der einzelnen Register können - abhängig vom Partnertyp - unterschiedlich sein:
- ⇨ "Register Adresse" auf Seite B-20
- ⇨ "Register Identifikation" auf Seite B-25
- ⇨ "Register Bezüge" auf Seite B-28
- ⇨ "Register Auftrag" auf Seite B-30
- ⇨ "Register Lieferung" auf Seite B-33
- ⇨ "Register Rechnung" auf Seite B-37
- ⇨ "Register Kundenspezifisch" auf Seite B-39
- ⇨ "Register Zahlung" auf Seite B-41
- ⇨ "Register Ausdruck" auf Seite B-44
- ⇨ "Register Limits" auf Seite B-47
- ⇨ "Register Bewertung" auf Seite B-50
- ⇨ "Register Produktion" auf Seite B-52
- ⇨ "Register Modifikation" auf Seite B-53
- ⇨ "Register Privat" auf Seite B-54

### Marktpartner - Kontextmenü
*Stammdaten > Marktpartner > F4*

Über das Kontextmenü (`<F4>`) haben Sie Zugriff auf folgende Bereiche:

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Kontaktdaten | ⇨ "Ansprechpartner" auf Seite B-55<br>⇨ "Adressen" auf Seite B-57<br>⇨ "Bankverbindungen" auf Seite B-61<br>"E-Mailadressen" auf Seite B-62 |
| b | Rabatte | ⇨ "Rabatte" auf Seite B-66 |
| c | Austausch-/Zusatzregeln | ⇨ "Austausch-/Zusatzregeln" auf Seite B-68 |
| d | Gestelltypen | ⇨ "Gestelltypen" auf Seite B-69 |
| e | Konfigurierte MP-Felder | ⇨ "Konfigurierte MP-Felder" auf Seite B-71 |
| f | Mitarbeiterzuordnungen | ⇨ "Vertreterzuordnung" auf Seite B-72<br>⇨ "Erfasserzuordnung" auf Seite B-73 |
| g | Gruppenzuordnung<br>Objektzuordnung<br>Farbzuordnung | ⇨ "Gruppenzuordnung" auf Seite B-74<br>⇨ "Objektzuordnung" auf Seite B-75<br>⇨ "Farbzuordnung" auf Seite B-77 |
| h | Bonuszuordnung | ⇨ "Bonuszuordnung" auf Seite B-78 |
| i | Artikelzuordnung | ⇨ "Artikelzuordnung" auf Seite B-79 |
| k | Texte/Druck | ⇨ "Marktpartnertexte" auf Seite B-81<br>⇨ "Marktpartner-Artikeltexte" auf Seite B-83<br>⇨ "Formulare" auf Seite B-84<br>⇨ "Dokumentenarten" auf Seite B-85 |
| l | Vorgangs-Recherche | ⇨ "Vorgangs-Recherche" auf Seite B-86 |
| m | Marktpartner-Info | ⇨ "Marktpartner-Info" auf Seite B-87 |
| n | Replikationsdaten | ⇨ "Replikationsdaten" auf Seite B-88 |
| o | DFÜ-Konfiguration | ⇨ "DFÜ-Konfiguration" auf Seite B-90 |
| p | Hausspezifische Angaben | ⇨ "Hausspezifische Angaben" auf Seite B-91 |

> **Kontextmenü**
> Das Kontextmenü ist abhängig vom Marktpartnertyp aufgebaut.

### Marktpartnersuche
*Stammdaten > Marktpartner > Feld Marktpartner > `<F9>`*

In diesem Such-Dialog legen Sie die Auswahlkriterien für die Marktpartnersuche fest.
Sobald Sie in den Suchfeldern eine Eingabe machen, wird die Treffermenge automatisch angepasst.
Über die Schaltfläche Details starten Sie einen Dialog, der Ihnen die zugeordneten Häuser auflistet (für Multi-Site).

> **Daten**
> Die Daten dieses Suchdialogs werden in den Speicher geladen und sind nur zum Zeitpunkt des Ladens aktuell.
> Haben Sie im Marktpartnerstamm eine Änderung vorgenommen, müssen Sie die Schaltfläche [Refresh] drücken, um die angezeigten Daten im Suchdialog zu aktualisieren.

Die Register Adresse und Identifikation im Trefferbereich liefern Ihnen eine Übersicht zu häufig verwendete Daten der Marktpartner.

> **Anzahl der angezeigten Daten**
> Da die anzuzeigende Datenmenge extrem hoch sein kann (z. B. alle Kunden eines Landes) werden für die Suche nicht alle existierenden Daten automatisch in den Zwischenspeicher geladen. Eine Information hierzu liefern Ihnen die Zahlen rechts oberhalb der Treffermenge. Bsp.: Wenn in der Satzanzeige steht 1:100 (14873). Das bedeutet, dass es sich um den ersten Eintrag (der Treffermenge) von 100 geladenen (Zwischenspeicher) von insgesamt 14873 Einträgen handelt. Die Anzahl der zu ladenden Einträge (Zwischenspeicher) ist konfigurierbar.

> **Schaltflächen zum Blättern**
> Über die Schaltflächen `|<`, `<<`, `>>` und `>|` können Sie in der Treffermenge blättern. Mit der Schaltfläche `>>` blättern Sie seitenweise (16 Einträge) vor. Mit der Schaltfläche `<<` blättern Sie seitenweise (16 Einträge) zurück. Mit der Schaltfläche `>|` springen Sie an das Ende des Zwischenspeichers (100. Eintrag) und mit `|<` an den Anfang des Zwischenspeichers (1. Eintrag).
> Zum Laden weiterer Einträge, klicken Sie auf die Schaltfläche [Weitere Daten]. Dann wird wieder die konfigurierte Anzahl an Daten (in unserem Fall 100) in den Zwischenspeicher geladen.

#### Erläuterung der Suchfelder
**Ab Nummer**
Eingabe einer Nummer, ab der gesucht werden soll.
*Technische Info: Numerisches Feld, DB-Feld: mp.mpnr*

**Matchcode**
Eingabe des Matchcodes als Suchwert. Sie können den kompletten Matchcode eingeben oder nur einen Teil.
*Technische Info: Alphanumerisches Feld, DB-Feld: mp.mpmc*

**Typ**
Anzeige des Marktpartnertyps nach dem gerade gesucht wird. Er wird entsprechend der Auswahl im Marktpartnerdialog vorbelegt und ist nicht änderbar.

**Name**
Eingabe des Namens als Suchwert. Sie können den kompletten Namen eingeben oder nur einen Teil (Groß-/Kleinschreibung wird nicht berücksichtigt).
*Technische Info: Numerisches Feld, DB-Feld: mp.name*

**Vorname**
Eingabe des Vornamens als Suchwert. Sie können den kompletten Vornamen eingeben oder nur einen Teil.
*Technische Info: Alphanumerisches Feld, DB-Feld: mp.vname*

**Straße**
Eingabe der Straße als Suchwert. Sie können die komplette Straße eingeben oder nur einen Teil.
*Technische Info: Alphanumerisches Feld, DB-Feld: mp.strasse*

**Haus**
Auswahl und Eingabe der Hausnummer/Mandantennummer als Suchwert. Die Eingabe hier ist nur sinnvoll, wenn das erweiterte Mehrmandantensystem konfiguriert ist, da nur dann Marktpartner einem Mandanten zugeordnet werden können.
*Technische Info: Numerisches Feld, `<F9>`, DB-Feld: mp.hausnr*

**Land**
Auswahl und Eingabe des Landes als Suchwert. Die entsprechenden Schlüssel können über das Menü Länder (Schlüssel > Marktpartner) vergeben werden.
*Technische Info: Alphabetisches Feld, `<F9>`, DB-Feld: mp.kfz*

**PLZ**
Auswahl und Eingabe der Postleitzahl als Suchwert. Sie können die komplette Postleitzahl eingeben oder nur einen Teil.
*Technische Info: Numerisches Feld, `<F9>`, DB-Feld: mp.plz*

**Ort**
Auswahl und Eingabe des Ortes als Suchwert. Sie können den kompletten Ort eingeben oder nur einen Teil.
*Technische Info: Alphabetisches Feld, `<F9>`, DB-Feld: mp.ort*

**USt-Ident-Nr.**
Eingabe der Umsatzsteuer-Identifikationsnummer als Suchwert. Sie können die komplette Nummer eingeben oder nur einen Teil (Groß-/Kleinschreibung wird berücksichtigt).
*Technische Info: Numerisches Feld, DB-Feld: mp.steuernr*

**Art**
Auswahl der Art als Suchwert:
- **aktiv:** Es werden nur aktive Marktpartner angezeigt.
- **stillgelegt:** Es werden nur stillgelegte Marktpartner angezeigt.
- **alle:** Es werden alle Marktpartner angezeigt.
*Technische Info: Alphabetisches Feld, `<F9>`, DB-Feld: mp.still*

### Register Adresse
*Stammdaten > Marktpartner*

In diesem Register erfassen und/oder bearbeiten Sie die Rechnungsadresse des Marktpartners. Das Register ist in eine linke und eine rechte Seite aufgeteilt. Die linke Seite enthält die Adressdaten des Marktpartners und ist während des gesamten Bearbeitungsvorgangs präsent. Die rechte Seite zeigt die Daten aus den anderen Registern bzw. weitere Optionen.

Mit `<F5>` öffnen Sie einen Dialog, in dem Sie Anmerkungstexte zu dem Marktpartner hinterlegen können.
⇨ "Marktpartner - Anmerkungstexte" auf Seite B-23

Mit `<Shift><F5>` öffnen Sie einen Dialog, in dem Sie Artikel-Anmerkungstexte zu dem Marktpartner hinterlegen können.
⇨ "Artikel - Anmerkungstexte" auf Seite B-302

Mit `<Shift><F9>` springen Sie in das Feld Matchcode.

> **Asiatische Installationen**
> Die asiatischen Installationen beinhalten zusätzliche Textfelder zur Eingabe von Adressen.

**Name**
Name des Marktpartners.
*Technische Info: Alphanumerisches Feld, DB-Feld: mp.name*

**Vorname**
Vorname des Marktpartners an.
*Technische Info: Alphanumerisches Feld, DB-Feld: mp.vname*

**Anrede**
Auswahl der Anrede, z, B. Herr oder Frau (Stammdaten > Schlüssel > Marktpartner > Anreden).
*Technische Info: `<F9>`, DB-Feld: mp.anrede*

**z.Hd.**
zu Händen. Name des Postempfängers bei Firmenadressen.
*Technische Info: Alphabetisches Feld, DB-Feld: mp.zhd*

**Zusatz**
Feld für Zusatz, z. B. die Branche.
*Technische Info: Alphabetisches Feld, DB-Feld: mp.branche*

**Straße**
Straße zur Adresse.
*Technische Info: Alphanumerisches Feld, DB-Feld: mp.str*

**PLZ, Fach**
Die dem Postfach entsprechende Postleitzahl sowie die Nummer des Postfachs.
*Technische Info: Alphanumerisches Feld, DB-Feld: mp.pfplz / mp.postfach*

**PF Ort**
Der dem Postfach zugehörige Ort.
*Technische Info: Alphanumerisches Feld, DB-Feld: mp.pfort*

**PLZ, Ort**
Die dem Ort entsprechende Postleitzahl und der Ort
*Technische Info: Alphanumerisches Feld, DB-Feld: mp.plz / mp.ort*

**KFZ Land**
KFZ-Länderkennzeichen und das entsprechende Land.
*Technische Info: Alphanumerisches Feld, DB-Feld: mp.kfzcode / mp.land*
⇨ "Länder" auf Seite B-120

**Entfer.**
Die Entfernung zwischen Ihrer Firma und dem Marktpartner in Kilometer. Wird in der Rabatt/ Zuschlagsberechnung verwendet (z B Transportzuschlag) als Staffelbasis.
*Technische Info: Numerisches Feld, DB-Feld: mp.kilometer*

**Telefon**
Telefonnummer des Marktpartners.
*Technische Info: Numerisches Feld, DB-Feld: mp.telefon*

**Fax**
Faxnummer des Marktpartners. Mit dem Toggle-Feld dahinter steuern Sie, ob der Marktpartner die Dokumente per Fax haben möchte. Mögliche Werte: J/N. Wird im Formulardruck ausgewertet und ermöglicht bei entsprechender Konfiguration das automatische Faxen von Dokumenten zum Marktpartner.
*Technische Info: Numerisches Feld, DB-Feld: mp.faxnr*

**E-Mail**
E-Mail-Adresse des Marktpartners. Mit `<F5>` können Sie mehrere E-Mail-Adressen hinterlegen. Wird im Formulardruck ausgewertet und ermöglicht bei entsprechender Konfiguration das automatische versenden von Dokumenten zum Marktpartner per E-Mail.
*Technische Info: Alphanumerisches Feld, DB-Feld: mp.email*

**Webseite**
URL des Marktpartners. Mit `<F5>` starten Sie den Browser.
*Technische Info: Alphanumerisches Feld, DB-Feld: mp.website*

**Sprache**
Auswahl der Sprache, in der der Kunde seine Dokumente erhält, z, B. Deutsch oder Englisch (Stammdaten > System > Sprachen). Entsprechend dieser Definition werden die Texte bei der Vorgangserfassung generiert und bei entsprechender Konfiguration die Ausdrucke für Marktpartner in der angegebenen Sprache erstellt.
*Technische Info: `<F9>`, DB-Feld: mp.sprkz*

**Anmerkungen**
Diese Texte dienen in den verschiedensten Programmteilen als wichtiges Informationsmedium. So können die Einträge u. a. in der Auftragserfassung bei Auswahl des Kunden auf dem Bildschirm angezeigt werden. Es gibt zwei unterschiedliche Anmerkungstexte:
- `<F5>` startet den Dialog für allgemeine Anmerkungstexte des Marktpartners.
- `<Shift>` `<F5>` startet den Dialog für artikelbezogene Anmerkungstexte des Marktpartners.
*Technische Info: DB-Feld: memo.txt*

**Ergänzende Informationen**
- ⇨ "Marktpartner - Anmerkungstexte" auf Seite B-23
- ⇨ "Artikel - Anmerkungstexte" auf Seite B-302

### Marktpartner - Anmerkungstexte
*Stammdaten > Marktpartner > F5*

In diesem Dialog können Sie Texte für Marktpartner hinterlegen, die in den verschiedensten Programmteilen als wichtiges Informationsmedium dienen. Oben im Dialog sehen Sie die Marktpartner-Nummer, für die der Text gilt.

> **Mehrsprachige Anmerkungestexte**
> Seit QR2209 können Sie in A+W Enterprise auch für Anmerkungen mehrsprachige Bezeichnungen hinterlegen. Diese Möglichkeit besteht jedoch nur, wenn Sie mit dem Modul Mehrsprachigkeit für Mitarbeiter innerhalb der internen Mandantentrennung arbeiten.

**Sprache**
Sprachkennzeichen.
*Technische Info: Numerisches Feld, DB-Feld: xsprbez.sprkz*

Geben Sie den Text in dem freien Feld ein und speichern Sie diesen mit `<F3>`.
Mit `<Shift><F9>` legen Sie den Info-Ort fest:
- **Stammdaten:** Der Text wird nur in den Stammdaten angezeigt.
- **Überall:** Der Text wird in den Stammdaten und in den Verkaufs- und Einkaufsvorgängen angezeigt.
- **VK-Auftrag:** Der Text wird im Verkaufsvorgang angezeigt.
- **EK-Auftrag:** Der Text wird im Einkaufsvorgang angezeigt.

Mit `<Shift><F10>` legen Sie die Priorität fest:
- **hoch:** Der Text wird automatisch an den festgelegten Info-Orten angezeigt, sobald nur eine Zeile die Prio-hoch hat.
- **niedrig:** Der Text wird nicht automatisch angezeigt, er muss bei der Vorgangserfassung über das Menü aufgerufen werden.
*Technische Info: Alphanumerisches Feld, DB-Feld: memo.txt*

> **Priorität bei Info-Ort Stammdaten**
> Wenn Sie als Info-Ort Stammdaten gewählt haben, greift die Priorität niedrig nicht. Der Text wird immer in den Stammdaten des Marktpartners angezeigt.

### Register Identifikation
*Stammdaten > Marktpartner > Register Identifikation*

In diesem Register erfassen und/oder bearbeiten Sie alle steuerlichen und provisionsmäßigen Daten des Marktpartners.

> **Linker Dialogteil**
> Während der Bearbeitung der rechten Dialogseite bleiben die Stammdaten des Kunden im linken Dialogteil weiterhin sichtbar. Sind Änderungen notwendig, müssen diese im Register Adresse vorgenommen werden.

**USt-Identnr.**
EG-Steuernummer, d. h. die Umsatzsteueridentnummer. Bei der Eingabe der USt-Identnr. erfolgt eine länderspezifische Prüfung. Diese Nummer wird vorwiegend in der FIBU-Übergabe verwendet.
*Technische Info: Alphanumerisches Feld, DB-Feld: mp.steuernr*

**FA-Steuernr.**
Angabe zur Finanzamtssteuernummer, die vorwiegend in der FIBU-Übergabe verwendet wird. Es ist auch möglich, das System so zu konfigurieren, dass eine Erfassung von Gutschriften ohne FA-Steuernr nicht möglich ist.
*Technische Info: Alphanumerisches Feld, DB-Feld: mp.finstnr*

**Firmierung**
Vollständiger Firmenname des Marktpartners, z. B. Schmidt GmbH & Co. KG.
*Technische Info: Alphanumerisches Feld, DB-Feld: mp.firmname*

**Externe Liefnr.**
Falls der Marktpartner eine eigene Lieferantennummer vorgibt, können Sie diese hier hinterlegen. Das Feld wird vorwiegend in der FIBU-Übergabe verwendet.
*Technische Info: Alphanumerisches Feld, DB-Feld: mp.exlinr*

**Externe Kundennr.**
Falls der Marktpartner eine eigene Kundennummer vorgibt, können Sie diese hier hinterlegen. Das Feld wird vorwiegend in der FIBU-Übergabe verwendet.
*Technische Info: Alphanumerisches Feld, DB-Feld: mp.extkundnr*

**Externe Objektnr.**
Dieses Feld ist nur aktiv, wenn der Marktpartner vom Typ Objekt ist. Dann können Sie hier eine externe Objektnummer hinterlegen.
*Technische Info: Alphanumerisches Feld, DB-Feld: mp.extkundnr*

**Liefnr.**
Auswahl der Lieferantennummer. Wenn es sich bei dem Marktpartner um einen Kunden handelt, der auch als Lieferant fungiert, dann können Sie hier die Lieferantennummer zuordnen. Das Feld wird vorwiegend in der FIBU-Übergabe verwendet.
*Technische Info: `<F9>`, DB-Feld: mp.lieflinr*

**Matchcode**
Dieses Feld steht in Zusammenhang mit dem Feld Liefnr. und zeigt Ihnen den Matchcode des Lieferanten.
*Technische Info: Anzeige-Feld*

**Div.-Marktp.**
Hier handelt es sich um einen Marktpartner, der nur einmal bestellt bzw. beliefert wird. Bei diesem Kunden kann im Gegensatz zu den anderen Kunden in der Vorgangserfassung, die Rechnungsadresse geändert werden:
- **Ja:** Bei dem Marktpartner handelt es sich um einen diversen Marktpartner.
- **Nein:** Der Marktpartner wird als permanenter Kunde geführt.
*Technische Info: Toggle-Feld, DB-Feld: mp.divers*

**Provision**
Auswahl des Provisionsschlüssels. Steht die Höhe der Vertreterprovision in Abhängigkeit zum Kunden, muss hier ein numerischer Provisionsschlüssel eingegeben werden. Die Provisionssätze für die verschiedenen Schlüsselwerte werden im Menüpunkt Provisionskürzel (Stammdaten > Provisionen) hinterlegt. Das Feld ist nur bei entsprechender Systemkonfiguration verfügbar.
*Technische Info: `<F9>`, DB-Feld: mp.provnr*

**Vertr. (Erlös)**
Auswahl des erlösmäßigen Vertreters. Für den hier eingetragenen Mitarbeiter werden dann die jeweiligen Provisionssätze gebucht und stehen zur Abrechnung bereit. Diese Angaben können später im Auftrag geändert werden. Voraussetzung für die Auswahlmenge ist die Funktionszuordnung Vertreter in den Mitarbeiter-Stammdaten. Bei erweiterter interner Mandatentrennung kann diese Angabe auch mandantengenau erfolgen.
*Technische Info: `<F9>`, DB-Feld: mp.vertrerloe*

**Außendienst**
Auswahl des zuständigen Außendienstmitarbeiters. Diese Angaben werden in die Auftragserfassung übernommen und gegebenenfalls auf den kundenseitigen Papieren ausgegeben. Diese Angaben können später im Auftrag geändert werden.
*Technische Info: `<F9>`, DB-Feld: mp.aussenmanr*

**Innendienst**
Auswahl des zuständigen Innendienstmitarbeiters. Diese Angaben werden in die Auftragserfassung übernommen und gegebenenfalls auf den kundenseitigen Papieren ausgegeben. Diese Angaben können später im Auftrag geändert werden.
*Technische Info: `<F9>`, DB-Feld: mp.innenmanr*

**Sachbearbeiter**
Auswahl des zuständigen Mitarbeiters für die Auftragsbearbeitung. Er wird in den Auftrag übernommen und gegebenenfalls auf den kundenseitigen Papieren ausgedruckt. Diese Angaben können später im Auftrag geändert werden.
*Technische Info: `<F9>`, DB-Feld: mp.sachmanr*

**Ergänzende Informationen**
- ⇨ "Marktpartner - Anmerkungstexte" auf Seite B-23
- ⇨ "Artikel - Anmerkungstexte" auf Seite B-302

### Register Bezüge
*Stammdaten > Marktpartner > Register Bezüge*

In diesem Register erfassen und/oder bearbeiten Sie alle FIBU-technischen und ein Teil der preisrelevanten Daten des Marktpartners. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.

#### Erläuterung der Felder
**FIBU-Debitor**
Auswahl der FIBU-Debitorennummer. Sie ist ein Verweis auf den rechnungsempfangenden Kunden. Daher werden FIBU-Debitor und Kundennummer gleich sein. Im Falle einer zentralen Rechnungsverwaltung eines Unternehmens mit mehreren Zweigstellen muss der FIBU-Debitor mit der Kundennummer der Rechnungsstelle belegt werden, auf die dann die Rechnungen verbucht und ausgestellt werden.
*Technische Info: `<F9>`, DB-Feld: mp.stddebnr*

**Statistik-Debitor**
Auswahl des Statistik-Debitors. Unabhängig vom FIBU-Debitor können die statistischen Umsätze auf andere Statistik-Debitoren kumuliert werden. Das könnte z. B. die Kundennummer einer auftraggebenden Zweigstelle sein. Die statistischen Daten geben dann Aufschluss über die Umsatzentwicklung der einzelnen Filialen.
*Technische Info: `<F9>`, DB-Feld: mp.statdebnr*

**Konditions-Debitor**
Auswahl der Kundennummer, deren Konditionen für die erfassten Vorgänge gelten soll. Bei erweiterter interner Mandantentrennung kann der Konditions-Debitor auch mandantengenau erfolgen.
*Technische Info: `<F9>`, DB-Feld: mp.konddebnr*

**AZ-Debitor**
Auswahl der Kundennummer. Analog gelten die Austausch-Zusatz-Regeln in der Vorgangserfassung, die für den Kunden hinterlegt wurden, der in diesem Feld vermerkt wurde.
*Technische Info: `<F9>`, DB-Feld: mp.azdebnr*

**Debitor**
Auswahl, ob Debitor:
- **Ja:** Der Marktpartner ist ein Debitor.
- **Nein:** Der Marktpartner ist kein Debitor.
*Technische Info: `<F9>`, DB-Feld: mp.debitor*

**Debitor-Hausnr.**
Ist nur aktiv, wenn das Feld Debitor den Eintrag Ja hat. Dann können Sie dem Debitor ein Haus zuordnen. Diese Angaben sind nur bei erweiterten internen Mandantentrennung relevant. Nähere Information darüber kann der A+W Enterprise-Konfigurationsanleitung entnommen werden.
*Technische Info: `<F9>`, DB-Feld: mp.debhausnr*

**Kond. Branche**
Auswahl der Branche, z. B. Schreiner, Metallbau, etc. Die entsprechenden Konditionen werden im Menü Brance (Stammdaten > Schlüssel > Marktpartner > Branche) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: mp.kbranche*

**Wirtsch.-Raum**
Auswahl des Wirtschaftsraums, in dem sich der Marktpartner befindet, z. B. Frankreich, Niederlande, Belgien, etc.. Der Wirtschaftsraum wird sehr oft in die eigenen statistischen Auswertungen herangezogen.
*Technische Info: `<F9>`, DB-Feld: mp.kwrtraum*

**Region**
Auswahl der Region, in der sich der Marktpartner befindet, z. B. Hessen, Niedersachsen, Bayern, etc.. Die Regionen werden im Menü Region / Bundesländer (Stammdaten > Schlüssel > Marktpartner > Region / Bundesländer) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: mp.region*

**Kostenstelle**
Auswahl der Kostenstelle des Marktpartners, z. B. Isolierglas, ESG, Gestelle, etc.. Kostenstellen sind sinnvolle betriebliche Bereiche (Abteilungen, Gruppen), die eingrenzbare Kosten verursachen. Die gewählte Kostenstelle kann später ausgewertet werden. Kostenstellen werden im Menü Kostenstellen (Stammdaten > Kostenstamm > Kostenstellen) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: mp.kostenst*

**Abteilung**
Auswahl einer Abteilung, z. B. Zuschnitt, Versand, etc..
*Technische Info: `<F9>`, DB-Feld: mp.abtnr*

**Kalender**
Auswahl einer spezifischen Marktpartner-Kalendernummer.
*Technische Info: `<F9>`, DB-Feld: mp.kalnr*

**Ergänzende Informationen**
- ⇨ "Marktpartner - Anmerkungstexte" auf Seite B-23
- ⇨ "Artikel - Anmerkungstexte" auf Seite B-302

### Register Auftrag
*Stammdaten > Marktpartner > Register Auftrag*

In diesem Register werden alle auftragsbezogenen Informationen des Marktpartners hinterlegt. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.

#### Erläuterung der Felder
**Kantenschutz**
Auswahl des gewünschten Kantenschutzartikels, der bei ISO angebracht werden soll. Damit erfolgt automatisch ein entsprechender Eintrag bei den Kunden-Austausch-Zusatzregeln, die während der Auftragserfassung ausgewertet werden.
*Technische Info: `<F9>`, DB-Feld: mp.kantschutz*

**Stdverglasg**
Auswahl der gewünschten Verglasungsartikels, der bei ISO angebracht werden soll. Damit erfolgt automatisch ein entsprechender Eintrag bei den Kunden-Austausch-Zusatzregeln, die während der Auftragserfassung ausgewertet werden.
*Technische Info: `<F9>`, DB-Feld: mp.stdverglas*

**Verglasung**
Auswahl, wo die Verglasung angezeigt wird:
- In Position und Fuß ausweisen
- In Position einrechnen
- Nur im Fuß ausweisen
*Technische Info: Toggle-Feld, DB-Feld: mp.verglasung*

**Objektzwang**
Definition, ob dem Kunden im Auftrag zwingend ein Objekt zugeordnet werden muss:
- **Ja:** Dem Kunden muss im Auftrag immer ein Objekt zugeordnet werden.
- **Nein:** Eine Objektzuordnung ist optional.
*Technische Info: Toggle-Feld, DB-Feld: mp.objmuss*

**FremdnrZwang**
Definition, ob dem Kunden im Auftrag zwingend eine Fremdnummer zugeordnet werden muss:
- **Ja:** Dem Kunden muss im Auftrag immer eine Fremdnummer zugeordnet werden.
- **Nein:** Die Zuordnung einer Fremdnummer ist optional.
*Technische Info: Toggle-Feld, DB-Feld: mp.exaufmuss*

**KommissZwang**
Definition, ob dem Kunden im Auftrag zwingend eine Kommission zugeordnet werden muss:
- **Ja:** Dem Kunden muss im Auftrag immer eine Kommission zugeordnet werden.
- **Nein:** Die Zuordnung einer Kommission ist optional.
*Technische Info: Toggle-Feld, DB-Feld: mp.kommmuss*

**Maßheinheit**
Auswahl der Maßeinheit:
- Metrisch
- Imperial
Für die Nutzung der imperialen Maßeinheit muss das System entsprechend konfiguriert werden.
*Technische Info: Toggle-Feld, DB-Feld: mp.massystem*

**Standard-SZR**
Hier können Sie den Wert für einen Standard-Rahmen in mm hinterlegen. Dieser Wert wird dann als Vorbelegung in der Auftragserfassung bei ISO-Positionen ohne fixen SZR verwendet.
Ist für einen ISO Artikel in den Artikelstammdaten ein nicht änderbarer SZR definiert, so wird der SZR des Artikels verwendet. Ist der SZR jedoch als änderbar definiert, wird der kundenindividuelle SZR verwendet.
Wenn der SZR in den Artikelstammdaten als änderbar definiert ist, ist auch der kundenindividuelle SZR ist in der Positionserfassung änderbar.
*Technische Info: Numerisches Feld, DB-Feld: mp.defszr*

**min ISO ges. Stärke**
Hier können Sie die minimale Stärke einer gesamten ISO-Einheit hinterlegen.
*Technische Info: Numerisches Feld, DB-Feld: mp.minszr*

**max ISO ges. Stärke**
Hier können Sie die maximale Stärke einer gesamten ISO-Einheit hinterlegen.
Minimale und maximale Stärke werden innerhalb der Restriktionsprüfung in der Auftragserfassung geprüft. Wenn ein Auftrag Positionen, die diese Restriktion nicht erfüllen, enthält, kann der Auftrag nur von berechtigten Mitarbeitern erfasst werden. Die weiteren Information kann der A+W Enterprise - EDV-Modulbeschreibung entnommen werden.
*Technische Info: Numerisches Feld, DB-Feld: mp.maxszr*

**Mindestwert**
Hier können Sie einen Mindestauftragswert (Kunden) bzw. einen Mindestbestellwert (für Lieferanten) hinterlegen. Dieser Wert wird als Berechnungsgrundlage in den Auftrag übernommen. Ist der Auftragswert < Mindestwert, wird der Mindestwert berechnet.
Der Mindestauftragswert bzw. Mindestbestellwert müssen zwingend in Kundenwährung angegeben werden. Andernfalls, bei Währungsänderung im Auftrag, erfolgt keine Umrechnung des Mindestwertes.
*Technische Info: Numerisches Feld, DB-Feld: mp.relimwert*

**Ergänzende Informationen**
- ⇨ "Marktpartner - Anmerkungstexte" auf Seite B-23
- ⇨ "Artikel - Anmerkungstexte" auf Seite B-302

### Register Lieferung
*Stammdaten > Marktpartner > Register Lieferung*

In diesem Register werden alle Informationen, die die Lieferung an den Marktpartner betreffen, hinterlegt. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.

#### Erläuterung der Felder
**Std.-Route**
Auswahl der Route. Für die Versandplanung sollte jeder Kunde einer Route zugeordnet werden. Die Route wird in den Auftrag übernommen, die beim Bedarf geändert werden kann. Von dort aus wird die Route an das Versandsteuerungssystem weitergereicht. Im Menüpunkt Routen (Stammdaten > Schlüssel > System > Versand > Routen) werden die Routen hinterlegt.
*Technische Info: `<F9>`, DB-Feld: mp.routenr*

**Route 2-4**
Definition von Alternativ-Routen, die verwendet werden können, wenn die Standard-Route nicht optimal zum Kundenwunschtermin passt. Bei der Lieferterminbestimmung im Auftrag wird dann berechnet, ob eine Alternativroute günstiger ist. Die Felder Route 2-4 sind nur dann änderbar, wenn das System nicht für Routen aus den Adressenstamm konfiguriert ist.
*Technische Info: `<F9>`, DB-Feld: mp.routenr2, routenr3, routenr4*

**Ladefolge**
Definition der Ladefolge. Bei der Zusammenstellung einer Tour werden Auftragspositionen verschiedener Kunden auf ein Fahrzeug geladen. Die Reihenfolge der Beladung kann durch die Ladefolge vorgegeben werden. Der Eintrag erfolgt frei und wird im Versandsteuerungssystem angezeigt und kann auf den Ladepapieren ausgewertet werden. Über `<F9>` kann der Überblick verschaffen werden, welche Lagefolgen bereits vergeben wurden. Bei Verwendung des Moduls OTR wird die Ladereihenfolge aus OTR übernommen werden.
*Technische Info: `<F9>`, DB-Feld: mp.routeposnr*

**Versandart**
Auswahl der Versandart, z. B. LKW, Spedition, etc. Dieses Feld hat ausschließlich informativen Charakter für die Versandabteilung. Die Versandarten werden im Menü Verpackungsart (Stammdaten > Schlüssel > System > Versand > Versandart) angelegt.
*Technische Info: `<F9>`, DB-Feld: mp.versandart*

**Verpackart**
Auswahl der Verpackungsart, z. B. Gestell, Kiste, Gitterbox, etc. Dieses Feld hat ausschließlich informativen Charakter für die Versandabteilung. Die Versandarten werden im Menü Verpackungsart (Stammdaten > Schlüssel > System > Versand > Verpackungsart) angelegt.
*Technische Info: `<F9>`, DB-Feld: mp.verpackart*

**Lieferart**
Auswahl der Lieferbedingung, z. B. frei Haus, Selbstabholer, etc. Dieser Text ist für Ausdruck auf den Kundenpapieren vorgesehen. Die Lieferarten werden im Menü Verpackungsart (Stammdaten > Schlüssel > System > Versand > Lieferarten) angelegt
*Technische Info: `<F9>`, DB-Feld: mp.lieferart*

**Sammellieferschein**
Auswahl, ob für den Marktpartner ein Sammellieferschein möglich ist oder nicht:
- **Ja:** Ein Sammellieferschein ist möglich.
- **Nein:** Sammellieferschein ist nicht möglich.
*Technische Info: Toggle-Feld, DB-Feld: mp.lsammel*

**Teillieferung möglich**
Auswahl, ob der Marktpartner Teillieferungen erlaubt oder nicht:
- **Ja:** Teillieferungen sind erlaubt.
- **Nein:** Teillieferungen sind nicht erlaubt.
*Technische Info: Toggle-Feld,, DB-Feld: mp.teilliefkz*

**Handlingszeit**
Ist der Zeitraum zwischen der Fertigstellung des Produktes und dem Tag der Auslieferung. Eine solche Zeit kann notwendig werden, wenn der Kunde bestimmte Vorgaben für die Kommissionierung seiner Ware trifft. Sie wird als Frist eingetragen und damit von der Termin- und Kapazitätsplanung berücksichtigt. Die Zeit kann in Tagen oder in Stunden eingegeben werden (konfigurierbar).
*Technische Info: Numerisches Feld, DB-Feld: mp.hzeit*

**Anruf vor Auslieferung**
Auswahl, ob der Marktpartner vor der Auslieferung telefonisch kontaktiert werden soll oder nicht:
- **Ja:** Der Marktpartner möchte vor der Auslieferung angerufen werden.
- **Nein:** Ein Anruf ist nicht nötig.
*Technische Info: Toggle-Feld, DB-Feld: mp.anruf*

**Fahrtdauer**
Hier können Sie die Fahrtdauer zum Marktpartner in Tagen hinterlegen. Dieser Wert wird dann bei der Kalkulation des Liefertermins mit berücksichtigt.
*Technische Info: Numerisches Feld, DB-Feld: mp.anfahrt*

**Auslieferung via**
Auswahl, ob die Auslieferung über ein anderes Haus statt findet. Nähere Erläuterungen finden Sie in den Dokumenten zur via plant-Logik.
*Technische Info: `<F9>`, DB-Feld: mp.vsvia*

**Typ der DFÜ**
Handelt es sich bei diesem Marktpartner um einen internen Kunden, so kann hier definiert werden, wie interne Bestellungen per DFÜ ausgetauscht werden. Die Einstellung hat insbesondere Auswirkungen darauf, wie die Adressen in den erzeugten Bestellungen und Aufträgen behandelt werden:
- **keine:** Es erfolgt keine automatische interne Bestellübertragung.
- **VKKopplung:** Aus dem Auftrag im Handelshaus werden die zu bestellenden Teile bestellt. Es wird ein Auftrag direkt im System des Lieferanten erzeugt.
- **EK 1:1:** Aus dem Auftrag im Handelshaus werden die zu bestellenden Teile bestellt. Dabei wird erst eine entsprechende Bestellung im Handelshaus erzeugt und aus dieser wird ein Auftrag direkt im System des Lieferanten erzeugt. Eine Bestellung enthält bei dieser Einstellung immer nur Bestellteile aus einem Auftrag.
- **EK 1:n:** Aus dem Auftrag im Handelshaus werden die zu bestellenden Teile bestellt. Dabei wird erst eine entsprechende Bestellung im Handelshaus erzeugt und aus dieser wird ein Auftrag direkt im System des Lieferanten erzeugt. Eine Bestellung kann dabei Bestellteile aus mehreren Aufträgen enthalten.
*Technische Info: `<F9>`, DB-Feld: mp.dfuetyp*

**Direktbestellung**
Auswahl für Direktbestellung. Das Feld ist nur aktiv, wenn es sich bei dem Marktpartner und einen Lieferanten handelt. Damit steuern Sie, ob eine Bestellung bei diesem Lieferanten nach Auftragsfreischaltung sofort ausgelöst wird oder nicht:
- **Ja:** Bestellung wird sofort ausgelöst.
- **Nein:** Die Bestellung wird nicht sofort erzeugt, sondern wird zunächst in dem Bestellpool gestellt und kann später ausgelöst werden.
*Technische Info: Toggle-Feld, DB-Feld: mp.direktbestkz*

**Lieferscheinübertragung**
Über diese Checkbox steuern Sie die automatische Lieferscheinübertragung:
- `☑` Die Lieferscheinübertragung erfolgt automatisch per OpenTRANS.
- `☐` Es erfolgt keine Lieferscheinübertragung
*Technische Info: Toggle-Feld, DB-Feld: mp.liefdfuekz*

**Ergänzende Informationen**
- ⇨ "Marktpartner - Anmerkungstexte" auf Seite B-23
- ⇨ "Artikel - Anmerkungstexte" auf Seite B-302

### Register Rechnung
*Stammdaten > Marktpartner > Register Rechnung*

In diesem Register werden alle Informationen, die die Rechnung an den Marktpartner betreffen, hinterlegt. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.

#### Erläuterung der Felder
**Konto**
9stellige Kontonummer. Mit der Einführung der IBAN wird dieses Feld nicht mehr ausgewertet.
*Technische Info: Numerisches Feld, DB-Feld: mp.konto*

**Rechnungsart**
Auswahl der gewünschten Rechnungsform vom Marktpartner:
- Einzelrechnung
- Deckblattrechnung
- Sammelrechnung (wöchentlich, 14-tägig, monatlich)
*Technische Info: Toggle-Feld, DB-Feld: mp.rechnungsart*

**Sammelrechnungslimit**
Hier geben Sie ein, wie hoch das Rechnungslimit für die Sammelrechnungen ist.
*Technische Info: Numerisches Feld, DB-Feld: mp.srechlimit*

**Sammelrechnungsart**
Auswahl des Turnus, in dem die Sammelrechnungen geschrieben werden:
- wöchentlich
- 14-tägig
- monatlich
*Technische Info: Toggle-Feld, DB-Feld: mp.srechart*

**FIBU**
Falls die angebundene Finanzbuchhaltung die getrennte Übergabe verschiedener Zahlungsziele nicht erlaubt, kann dieses Feld alternativ mit einem beliebigen alphanumerischen Code versehen werden, der an die Finanzbuchhaltung übergeben wird. Die konkrete Nutzung der Felder ist maßgeblich vom verwendeten Fibu-System abhängig.
*Technische Info: Numerisches Feld, SELO (`<F9>`), DB-Feld: mp.fibukey*

**Rechnungsübertragung**
Auswahl, ob die Rechnungsübertragung im openTRANS-Format möglich ist.
- `☑`: Die Übertragung ist im openTRANS-Format möglich.
- `☐`: Die Übertragung ist nicht möglich.
*Technische Info: Toggle-Feld,*

**Gestelle berechnen**
Auswahl, ob der Marktpartner Teillieferungen erlaubt oder nicht:
- **Ja:** Gestelle werden in Rechnung gestellt.
- **Nein:** Gestelle werden nicht in Rechnung gestellt.
*Technische Info: Toggle-Feld, DB-Feld: mp.gsfaktura*

**Mietfreie Tage**
Wenn Sie Ihrem Kunden die Gestelle eine gewisse Anzahl von Tagen überlassen, an denen die Gestelle nichts kosten, können Sie hier diese Anzahl an Tagen eingeben.
*Technische Info: Numerisches Feld, DB-Feld: mp.gsmietfrei*

**Ergänzende Informationen**
- ⇨ "Marktpartner - Anmerkungstexte" auf Seite B-23
- ⇨ "Artikel - Anmerkungstexte" auf Seite B-302

### Register Kundenspezifisch
*Stammdaten > Marktpartner > Register Kundenspezifisch*

Das Register ist nur aktiv, wenn es sich bei dem Marktpartner um ein Objekt handelt und entsprechend konfiguriert ist. In diesem Register werden alle Informationen, die das Objekt betreffen zusammengefasst. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.

#### Erläuterung der Felder
**Vertr. (Erlös)**
Jedem Objekt kann ein Vertriebsmitarbeiter zugeordnet werden, der als erlösmäßiger Vertreter für alle am Objekt beteiligten Aufträge in die Vertreter-Provisionierung einfließt.
*Technische Info: `<F9>`, DB-Feld: mp.vertrerloe*

**Kostenstelle**
Ob die Kostenstelle objektindividuell in der Auftragsbearbeitung ersetzt werden soll, ist von dem gewählten Kostenstellenverfahren abhängig. Falls eine objektbezogene Kostenstellenvergabe gewünscht ist, kann dieses von A+W eingerichtet werden.
*Technische Info: `<F9>`, DB-Feld: mp.kostenst*

**Objektzwang**
Steht dieses Feld auf J, muss in der Auftragserfassung ein Objekt zwingend eingegeben werden.
*Technische Info: Toggle-Feld, DB-Feld: mp.kommmuss*

**Limitprüfung**
Objektorientierte Limitprüfung:
- **Fibu-Debitor:** Limitprüfung bei Auftragserfassung.
- **MP-Objekt:** Objektorientierte Limitprüfung.
*Technische Info: Toggle-Feld, DB-Feld: mp.objlimitpruef*

**Firmenlimit**
Dieses Feld kommt nur zum Tragen, wenn das Feld Limitprüfung auf J gesetzt ist. Überschreitet ein Auftragswert zuzüglich der offenen Posten und des offenen Auftragsbestandes das an dieser Stelle hinterlegte Firmenlimit, so erfolgt eine Warnung.
*Technische Info: Numerisches Feld, DB-Feld: mp.firmlimit*

**MWST**
Auswahl des Mehrwertsteuerkennzeichens. Die benötigten Steuerschlüssel werden im Menü Steuertypen (Schlüssel > System > Steuern) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: mp.mwst*

**Skonto 1/2**
Auswahl der Skontogruppenschlüssel. Die benötigten Skontoschlüssel werden im Menü Skontogruppen (Schlüssel > System > Skontogruppen) hinterlegt.
*Technische Info: Toggle-Feld, DB-Feld: mp.skonto1/2*

**Rechnungsart**
Auswahl der gewünschten Rechnungsform vom Objekt:
- Einzelrechnung
- Deckblattrechnung
- Sammelrechnung (wöchentlich, 14-tägig, monatlich)
*Technische Info: Toggle-Feld, DB-Feld: mp.rechnungsart*

**Std-Route**
Eine etwaige Objektroute greift übersteuernt in die Auftragsbearbeitung ein und ersetzt die im Kundenstamm hinterlegte Kundenroute.
*Technische Info: Toggle-Feld, DB-Feld: mp.routenr*

### Register Zahlung
*Stammdaten > Marktpartner > Register Zahlung*

In diesem Register werden alle Informationen, die die Zahlungsoptionen bezüglich der Marktpartner betreffen, hinterlegt. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.

#### Erläuterung der Felder
**Skonto 1-3**
In den Skontofeldern können die kundenindividuellen Skonti als Schlüssel zugewiesen werden. Bis zu drei gestaffelte Skonti sind möglich, deren Laufzeit und Prozentsatz entsprechend variieren muss. Die benötigten Skontoschlüssel werden im Menü Skontogruppen (Schlüssel > System) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: mp.skonto1-3*

**Urlaub berücksichtigen**
Auswahl, ob sich die Skontodauer verlängert, wenn der Rechnungsempfänger Urlaub hat:
- `☑` Die Skontodauer verlängert sich.
- `☐` Die Skontodauer verlängert sich nicht.
Voraussetzung ist, dass der Kalender für den jeweiligen Rechnungsempfänger gepflegt wird.
*Technische Info: Toggle-Feld, DB-Feld: mp.htag_skonto_rel*

**Zahlziel**
Hierunter versteht man den spätestmöglichen Zeitpunkt der Nettozahlung. Nach Ablauf des Zahlzieles beginnt die Mahnfrist. Die Eingabe erfolgt in Tagen.
*Technische Info: Numerisches Feld, DB-Feld: mp.zahlziel*

**Valuta**
Die Valutierung in Tagen bestimmt den Beginn der Skontofristen und des Zahlungszieles ab Rechnungsdatum (zuzüglich Postweg).
*Technische Info: Numerisches Feld, DB-Feld: mp.valuta*

**Merkmal**
Über die Schlüssel können Zahlungsmerkmale für Marktpartner vermerkt werden (Lastschrift, Abbuchung, etc.). Die Schlüssel werden im Menü Zahlungsmerkmal (Schlüssel > System) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: mp.zahlngmerk*

**Bonus**
Hier definieren Sie ob und in welcher Höhe sowie innerhalb welchen Zeitraumes der Kunde/Objekt einen Bonus erhält. Der Bonus wird nicht automatisch errechnet. Diese Angabe dient lediglich eigenen statistischen Anfragen. Die Bonusschlüssel werden im Menü Bonus (Schlüssel > System > Marktpartner) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: mp.bonus*

**Zahlungsverkehr**
Auswahl des Zahlungsverkehrs:
- Bankeinzug
- Vorauskasse
- Bei Lieferung
- Nach Vereinbarung
- Scheck
- Banklastschrift
*Technische Info: Toggle-Feld, DB-Feld: mp.azahlkz*

> **Zahlungsfelder für Marktpartnertyp=Objekt**
> Bei entsprechender Systemkonfiguration können die Felder Skonto1-Zahlungsverkehr auch für Objekte hinterlegt werden. Diese Zahlungskonditionen werden anschließend im Block in den Auftrag übernommen, sofern das Objekt erfasst wird. Bleiben die betroffene Felder für Objekt leer, wird die Information aus dem Kundenstamm übernommen.

**Mahnung**
Auswahl, ob im Verzugsfall eine Mahnung erfolgen soll.
- `☑` Der Kunde wird gemahnt.
- `☐` Der Kunde wird nicht gemahnt.
*Technische Info: Toggle-Feld, DB-Feld: mp.mahnkz*

**Gemahnt**
Zur Information kann notiert werden, wie viele Mahnungen bereits an den Kunden/Objekt ergangen sind. Dieser Wert kann ggf. an die Fibu übermittelt werden.
*Technische Info: Numerisches Feld, DB-Feld: mp.mahnanz*

**ltz. Schufa-Anfr.**
Hier können Sie das Datum der letzten Schufa-Anfrage eingeben.
*Technische Info: Datums-Feld, DB-Feld: mp.ltzschufa*

**Teilfakt. möglich**
Auswahl, ob der Marktpartner Teilfakturierungen erlaubt oder nicht:
- **Ja:** Teilfakturierungen sind erlaubt.
- **Nein:** Teilfakturierungen sind nicht erlaubt.
*Technische Info: Toggle-Feld, DB-Feld: mp.teilfakkz*

**Währung**
Das Mehrwährungssystem ist optional. Auswahl der Währung, in der der Marktpartner abgerechnet wird. Die Währungsschlüssel werden im Menü Währung (Stammdaten > Schlüssel > System) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: mp.waehrung*

**Kalkulat. in**
Das Mehrwährungssystem ist optional. Auswahl, in welcher Währung die Auftragsberechnung erfolgen soll:
- Eigenwährung der Firma
- Fremdwährung des Kunden, falls die Kundenwährung von der Eigenwährung der Firma abweicht, z. B. Kunde in der Schweiz.
*Technische Info: Toggle-Feld, DB-Feld: mp.waehrprs*

**Ausdruck in**
Haben Sie im Feld Kalkulat. in die Auswahl Fremdwährung getroffen, dann steuern Sie hier, in welcher Währung die kundenseitigen Papiere ausgegeben werden sollen. Mögliche Werte sind:
- kalkulierte Währung
- Fremdwährung im Fuß
- Fremdwährung in Pos. und Fuß
- Kalk. Währung + Euro im Fuß
- Kalk. Währung + Euro in Pos. und Fuß
- Fremdwährung + Euro im Fuß
- Fremdwährung + Euro in Pos. und Fuß
*Technische Info: Numerisches Feld, DB-Feld: mp.waehrdru*

> **Die Felder Kalkulation in und Ausdruck**
> Die Felder Kalkulation in und Ausdruck in sind nur zugänglich, wenn das Fremdwährungsmodul lizenziert und dem Kunden eine Währung zugeordnet wurde, die von der eigenen Währung abweicht.

### Register Ausdruck
*Stammdaten > Marktpartner > Register Ausdruck*

In diesem Register werden alle Informationen, die die Druckoptionen an den Marktpartner betreffen, hinterlegt. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.

#### Erläuterung der Felder
**Bruttopreis drucken**
Auswahl, ob der Bruttopreis ausgedruckt werden soll:
- Ja
- Nein
*Technische Info: Toggle-Feld, DB-Feld: mp.preisdrkz*

**MP-Faktor drucken**
Auswahl, ob der Marktpartner-Faktor ausgedruckt werden soll:
- Ja
- Nein
*Technische Info: Toggle-Feld, DB-Feld: mp.rabdrkz*

**Bearbeitungen drucken**
Mit diesem Feld steuern Sie, ob die Bearbeitungspreise bereits in der Vorgangserfassung in die zu druckenden Bearbeitungstexte generiert werden:
- Ja
- Nein
- P (Konfigurierbare Möglichkeit, die Preise für die Bearbeitungen nur dann in die Texte zu generieren, wenn diese vorhanden sind (Bearbeitungspreis > 0)).
*Technische Info: Toggle-Feld, DB-Feld: mp.explbearbkz*

**Zwischensumme**
Auswahl, ob eine kommissionsabhängige Zwischensumme gedruckt werden soll:
- Ja
- Nein
*Technische Info: Toggle-Feld, DB-Feld: mp.sumkomis*

**AB mit Sprossen**
Auswahl, ob der Sprossenaufbau mit der Auftragsbestätigung gedruckt werden sollen:
- Ja
- Nein
*Technische Info: `<F9>`, DB-Feld: mp.sprossenab*

**Bruttonettokennz.**
Auswahl für Brutto- oder Nettokennzeichen:
- **B:** Bruttokennzeichen
- **N:** Nettokennzeichen
*Technische Info: `<F9>`, DB-Feld: mp.brutnetkz*

**Kundenind. Positionen**
Auswahl für kundenindividuelle Positionsbezeichnungen, falls im Kundenstamm ein entsprechender Hinweis existiert:
- **Pos.:** Für Kunden, die diese Kennzeichnung tragen, wird in der Auftragsbearbeitung das Kundenpositionsfeld zugeschaltet, um die gewünschte Kunden-Positionsbezeichnung einzugeben. Diese Angaben erscheinen auf allen kundenseitigen Papieren und Etiketten.
- **Typ:** Hierbei handelt es sich um die Möglichkeit der typisierten Erfassung, wie es häufig bei Leistungsverzeichnissen öffentlicher Ausschreibungen gefordert wird. Bei dieser Vorgehensweise wird jedem Produkt eine vorgegebenen Typenbezeichnung im Rahmen der Auftragserfassung zugeordnet. Der Ausdruck einer solchen Auftragsbestätigung weist im Positionsteil nur die jeweilige Typbezeichnung aus, während im Fuß des Dokuments die genaue Produktbeschreibung dargestellt wird.
- **Keine**
*Technische Info: Toggle-Feld, DB-Feld: mp.kndposkz*

**Etikett**
Auswahl für Etikettentext. Die Schlüssel können über das Menü Etikettentexte (Stammdaten > Schlüssel > Marktpartner) vergeben werden.
*Technische Info: `<F9>`, DB-Feld: mp.etikett*

**Etikett-Text**
Wenn es sich bei dem Marktpartner um ein Objekt handelt können Sie hier einen weiteren Text für Etiketten eingeben.
*Technische Info: `<F9>`, DB-Feld: mp.etitxt1*

**Objekt-Kürzel**
Da auf Etiketten häufig nur wenig Platz zur Verfügung steht, kann auch das zweibuchstabige Objektkürzel auf dem Etikett ausgewiesen werden.
*Technische Info: Alphanumerisches Feld, DB-Feld: mp.etitxt2*

**Preisdarstellung**
Auswahl für die Preisdarstellung auf den Papieren nach Wunsch des Marktpartners:
- kein Preis
- ME-Preis
- Stückpreis
- ME-+Stückpreis
*Technische Info: `<F9>`, DB-Feld: mp.prsdarst*

**Textformeln**
Auswahl der Textformel.
*Technische Info: `<F9>`, DB-Feld: mp.artkennfrm*

**Max. E-Mailgröße**
Maximale Größe der E-Mail mit Anhang in MByte. Beim E-Mail-Versand wird standardmäßig der Anhang in das zip-Format komprimiert. Durch eine Systemkonfiguration können Sie einstellen, ob der gesamte Anhang komprimiert wird, oder nur, wenn der Anhang die hier im Feld eingegebene E-Mailgröße überschreitet.
*Technische Info: `<F9>`, DB-Feld: mp.mailsize*

### Register Limits
*Stammdaten > Marktpartner > Register Limits*

In diesem Register werden alle Informationen, die die Limits bezüglich der Marktpartner betreffen, hinterlegt. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.

#### Erläuterung der Felder
**Limitprüfung via**
Auswahl der Limitprüfung:
- **Fibu-Debitor:** Die Limitprüfung erfolgt bei der Auftragserfassung für den entsprechenden Kunden (Fibu-Debitor).
- **MP-Objekt:** Die Limitprüfung erfolgt bei der Auftragserfassung, wenn dieses Objekt dem Auftrag zugeordnet ist und das System entsprechend konfiguriert ist.
*Technische Info: `<F9>`, DB-Feld: mp.objlimitpruef*

**Firmenlimit**
Betrag in Eigenwährung bis zu dem die Firma dem Kunden Kredit gewährt. Bei entsprechender Konfiguration wird der Auftragswert zuzüglich der offenen Posten und der offenen Aufträge gegen das an dieser Stelle hinterlegte Firmenlimit geprüft.
*Technische Info: Numerisches Feld, DB-Feld: mp.firmlimit*

**Versichert bis**
In diesem Feld kann das Ablaufdatum der Kreditlimit hinterlegt werden.
*Technische Info: Numerisches Feld, DB-Feld: mp.firmlimverfall*

**AKV-Limit**
Betrag in Eigenwährung bis zu dem die Firma dem Kunden Kredit gewährt. Bei entsprechender Konfiguration wird der Auftragswert zuzüglich der offenen Posten und der offenen Aufträge gegen das an dieser Stelle hinterlegte AKV-Firmenlimit geprüft.
*Technische Info: Numerisches Feld, DB-Feld: mp.akvlimit*

**Versichert bis**
In diesem Feld kann das Ablaufdatum der Versicherung hinterlegt werden.
*Technische Info: Numerisches Feld, DB-Feld: mp.limverfall*

**Limitprüfung Auftrag**
Mit diesem Feld steuern Sie, was mit Aufträgen passiert, deren Auftragswert zuzüglich der offenen Posten und der offenen Aufträge das in den Feldern Firmenlimit und AKV-Limit hinterlegte Limit überschreitet. Verfügt der Mitarbeiter über entsprechende Rechte kann der Auftrag erfasst werden und landet anschließend in einem Freischaltpool (konfigurierbar). Aufträge, die sich im Freischaltpool befinden, können nur von autorisierten Personen freigegeben werden. Verfügt der Mitarbeiter nicht über diese Rechte, kann er den Auftrag nicht erfassen:
- **Firmen:** Es wird der im Feld Firmenlimit hinterlegte Wert verwendet.
- **AKV:** Es wird der im Feld AKV-Limit hinterlegte Wert verwendet.
- **AKV+Firmen:** Es werden die in den Feldern Firmenlimit und AKV-Limit hinterlegten Werte verwendet.
- **Keine:** Es erfolgt keine Limitprüfung.
*Technische Info: `<F9>`, DB-Feld: mp.limpruefkz*

**Erfassungsstopp**
Mit diesem Feld steuern Sie, ob beim Erreichen des Limits ein Vorgang für diesen Marktpartner erfasst werden darf oder nicht.
- **Nur Angebot:** Beim Erreichen des Limits kann kein Angebot mehr erfasst werden. Aufträge können für diesen Marktpartner noch erfasst werden.
- **Nur Auftrag:** Beim Erreichen des Limits kann kein Auftrag mehr erfasst werden. Angebote können für diesen Marktpartner noch erfasst werden.
- **Auftrag+Angebot:** Beim Erreichen des Limits können weder Angebote noch Aufträge erfasst werden.
- **Nein:** Für diesen Marktpartner wurde kein Erfassungsstopp hinterlegt.
*Technische Info: Toggle-Feld, DB-Feld: mp.erfasstop*

**Lieferstopp**
Mit diesem Feld steuern Sie, ob beim Erreichen des Limits ein Lieferschein für diesen Marktpartner gedruckt werden darf oder nicht.
- **Ja:** Beim Erreichen des Limits erfolgt keine Lieferung mehr.
- **Nein:** Beim Erreichen des Limits können Aufträge dennoch ausgeliefert werden.
*Technische Info: Toggle-Feld, DB-Feld: mp.lieferstop*

**Fakturastopp**
Mit diesem Feld steuern Sie, ob beim Erreichen des Limits eine Rechnung für diesen Marktpartner gedruckt werden darf oder nicht.
- **Ja:** Beim Erreichen des Limits kann keine Rechnung mehr ausgestellt werden.
- **Nein:** Beim Erreichen des Limits können Rechnungen dennoch ausgestellt werden.
*Technische Info: Toggle-Feld, DB-Feld: mp.fakturastop*

**MwSt**
Auswahl des Mehrwertsteuerkennzeichens. Die Steuerschlüssel werden im Menü Steuertypen (Stammdaten > Schlüssel > System > Steuern) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: mp.mwst*

**MwSt int.**
Interne Mehrwertsteuer. Das Feld ist nur aktiv, wenn es sich bei dem Marktpartner um einen Lieferanten handelt.
*Technische Info: `<F9>`, DB-Feld: mp.mwstint*

### Register Bewertung
*Stammdaten > Marktpartner > Register Bewertung*

In diesem Register können Sie die Zuverlässigkeit, Lieferzeit, Qualität, etc. bewerten. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.

#### Erläuterung der Felder
**Klasse**
Bewertung der Klasse. Die Bewertungsschlüssel werden im Menü Allgemein (Stammdaten > Schlüssel > Marktpartner > Qualitätsskala) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: mp.qklass*

**Zuverlässigkeit**
Bewertung der Zuverlässigkeit. Die Bewertungsschlüssel werden im Menü Allgemein (Stammdaten > Schlüssel > Marktpartner > Qualitätsskala) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: mp.qzuverl*

**Lieferzeit**
Bewertung der Lieferzeit. Die Bewertungsschlüssel werden im Menü Allgemein (Stammdaten > Schlüssel > Marktpartner > Qualitätsskala) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: mp.qzeit*

**Preise**
Bewertung der Preise. Die Bewertungsschlüssel werden im Menü Allgemein (Stammdaten > Schlüssel > Marktpartner > Qualitätsskala) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: mp.qpreis*

**Qualität**
Bewertung der Qualität. Die Bewertungsschlüssel werden im Menü Allgemein (Stammdaten > Schlüssel > Marktpartner > Qualitätsskala) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: mp.qqual*

**Service**
Bewertung des Services. Die Bewertungsschlüssel werden im Menü Allgemein (Stammdaten > Schlüssel > Marktpartner > Qualitätsskala) hinterlegt.
*Technische Info: F9>, DB-Feld: mp.qservice*

**Beratung**
Bewertung der Beratung. Die Bewertungsschlüssel werden im Menü Allgemein (Stammdaten > Schlüssel > Marktpartner > Qualitätsskala) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: mp.qberat*

**Kulanzverhalten**
Bewertung des Kulanzverhaltens. Die Bewertungsschlüssel werden im Menü Allgemein (Stammdaten > Schlüssel > Marktpartner > Qualitätsskala) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: mp.qkulanz*

**Bonität**
Bewertung der Bonität. Die Bewertungsschlüssel werden im Menü Allgemein (Stammdaten > Schlüssel > Marktpartner > Qualitätsskala) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: mp.qbonitaet*

### Register Produktion
*Stammdaten > Marktpartner > Register Produktion*

Die Felder dieses Dialogs dienten der Übergabe an PMS. Mit Einführung von A+W Production hat sich die Produktionsübergabe geändert. Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

#### Erläuterung der Felder
**Vorgabe der Produktionsfolge**
Auswahl, ob eine Produktionsfolge vorgegeben werden soll.
- **Ja:** Produktionsfolge soll vorgegeben werden
- **Nein:** Es wird keine Produktionsfolge vorgegeben.
*Technische Info: Toggle-Feld, DB-Feld: mp.prodfolge*

**Gestellbeladung**
Dieses Kriterium bestimmt die Sortierreihenfolge auf einem Gestell, abhängig von z. B. von Position, SZR, HM (Hardmaß), etc.
*Technische Info: Toggle-Feld, DB-Feld: mp.gbelad*

**Gestellgewicht (max)**
Das maximale Gestellgewicht kann eingegeben werden.
*Technische Info: F9>, DB-Feld: mp.gmaxgew*

### Register Modifikation
*Stammdaten > Marktpartner > Register Modifikation*

Dieses Register zeigt, wann und durch wen der Marktpartner angelegt wurde, wann und durch wen Änderungen vorgenommen wurden und wann der Marktpartner repliziert wurde. Auf der rechten Seite werden Ihnen die Adressinformationen angezeigt.
Im Bereich Replikationsdatum sehen Sie, an welche Häuser der Marktpartner repliziert wurde.

**Ergänzende Informationen**
- ⇨ "Marktpartner - Anmerkungstexte" auf Seite B-23
- ⇨ "Artikel - Anmerkungstexte" auf Seite B-302

### Register Privat
*Stammdaten > Marktpartner > Register Privat*

Für individuelle Auswertungen oder zusätzliche Kundeninformationen stehen zwei numerische und zwei alphanumerische Felder zur Verfügung. Auf Wunsch können diese mit einer eigenen Überschrift versehen und im System konfiguriert werden. Für kundenindividuelle Anpassungen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

**Ergänzende Informationen**
- ⇨ "Marktpartner - Anmerkungstexte" auf Seite B-23
- ⇨ "Artikel - Anmerkungstexte" auf Seite B-302

### Ansprechpartner
*Stammdaten > Marktpartner > `<F4>` > Kontaktdaten > Ansprechpartner*

In diesem Dialog können Sie für einen Marktpartner verschiedene Ansprechpartner hinterlegen. Dabei können mit `<F6>` weitere Datensätze hinzugefügt werden.
Bei mehreren hinterlegten Ansprechpartnern wird mit `<F5>` ein Hauptansprechpartner bestimmt.

#### Erläuterung der Felder
**Name**
Nachname des Ansprechpartners.
*Technische Info: Alphanumerisches Feld, DB-Feld: anspr.apname*

**Vorname**
Vorname des Ansprechpartners.
*Technische Info: Alphanumerisches Feld, DB-Feld: anspr.apvname*

**Anrede**
Auswahl der Anrede für den Ansprechpartner. Die entsprechenden Schlüssel können über das Menü Anreden (Stammdaten > Schlüssel > Marktpartner) vergeben werden.
*Technische Info: `<F9>`, DB-Feld: anspr.anrede*

**Abteilung**
Abteilung des Ansprechpartners.
*Technische Info: Alphanumerisches Feld, DB-Feld: anspr.abteilung*

**Position**
Position des Ansprechpartners.
*Technische Info: Alphanumerisches Feld, DB-Feld: anspr.position*

**Geburtsdatum**
Geburtsdatum des Ansprechpartners.
*Technische Info: Numerisches Feld, DB-Feld: anspr.gebdat*

**Telefon**
Telefonnummer des Ansprechpartners, z. B. +4964042051-0.
*Technische Info: Numerisches Feld, DB-Feld: anspr.telefon*

**Fax**
Faxnummer des Ansprechpartners, z. B. +4964042051-877.
*Technische Info: Numerisches Feld, DB-Feld: anspr.telefax*

**Mobil**
Mobilnummer des Ansprechpartners, z. B. +491777500000.
*Technische Info: Numerisches Feld, DB-Feld: anspr.telex*

**E-Mail**
Mailadresse des Ansprechpartners.
*Technische Info: Numerisches Feld, DB-Feld: anspr.email*

**Bemerkung**
Textuelle Bemerkungsfelder.
*Technische Info: Alphanumerisches Feld, DB-Feld: adr.text1-3*

### Adressen
*Stammdaten > Marktpartner > `<F4>` > Kontaktdaten > Adressen*

In diesem Dialog können Sie dem Marktpartner zusätzliche Adressen zuordnen. Die Rechnungsadresse ist die Hauptadresse und kann nicht verändert werden. Mit `<F6>` können weitere Datensätze hinzugefügt werden. Weicht die Lieferadresse von der Hauptanschrift ab, so ist der entsprechende Adresssatz mit `<F5>` als Standard-Anschrift zu bestimmen.

#### Erläuterung der Felder
**Name**
Nachname, bzw. Firmenname.
*Technische Info: Alphanumerisches Feld, DB-Feld: adr.adrname*

**Vorname**
Vorname.
*Technische Info: Alphanumerisches Feld, DB-Feld: adr.adrvname*

**Anrede**
Anrede, z. B. Herr, Frau, Firma. Die Schlüssel werden im Menü Anreden (Stammdaten > Schlüssel > Marktpartner) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: anspr.anrede*

**z. Hd.**
Zu Händen von (Nachname, Vorname).
*Technische Info: Alphanumerisches Feld, DB-Feld: adr.zhd*

**Zusatz**
Ermöglicht eine zusätzliche Adressinformation zur Ausgabe auf Kundenpapieren.
*Technische Info: Alphanumerisches Feld, DB-Feld: adr.branche*

**Straße**
Straßenname.
*Technische Info: Alphanumerisches Feld, DB-Feld: adr.str*

**PLZ, Fach**
Postleitzahl und das Postfach.
*Technische Info: numerisches/Alphanumerisches Feld, DB-Feld: adr.pfplz/ postfach*

**PF Ort**
Postfach und Ort.
*Technische Info: numerisches/Alphanumerisches Feld, DB-Feld: adr.pfort*

**PLZ, Ort**
Postleitzahl und der Ort.
*Technische Info: numerisches/Alphanumerisches Feld, DB-Feld: adr.plz/ort*

**Versandregion**
Auswahl der Versandregion. Die entsprechenden Schlüssel können über das Menü Versandregionen (Stammdaten > Schlüssel > System > Versand) vergeben werden.
*Technische Info: `<F9>`, DB-Feld:DB-Feld: adr.vsregion*

**KFZ Land**
Auswahl des Länder-Kfz-Kennzeichens. Die entsprechenden Schlüssel können über das Menü Länder (Stammdaten > Schlüssel > Marktpartner) vergeben werden.
*Technische Info: `<F9>`, DB-Feld: adr.kfzcode*

**Entfernung**
Entfernung zur Lieferadresse in km.
*Technische Info: Numerisches Feld, DB-Feld: adr.kilometer*

> **Hausspezifische Angaben zu Entfernung und Fahrtdauer**
> Angaben zu Entfernung und Fahrtdauer soll bei Verwendung interner Mandantentrennung pro Haus (Mandant) erfasst werden. Der Erfassungsdialog startet in solcher Konfiguration automatisch.
> ⇨ "Hausspezifische Adressdaten" auf Seite B-60

**Fahrtzeit**
Dauer der Fahrtzeit zur Lieferadresse in Tagen.
*Technische Info: Numerisches Feld, DB-Feld: adr.fahrtzeit*

> **Handlingszeit, Ankunfszeit und Anlieferstelle**
> Die Felder Handlingszeit, Ankunfszeit und Anlieferzeit sind nur bei entsprechenden Konfiguration freigeschaltet.

**Handlingszeit**
Ist der Zeitraum zwischen der Fertigstellung des Produktes und dem Tag der Auslieferung. Eine solche Zeit kann notwendig werden, wenn der Kunde bestimmte Vorgaben für die Kommissionierung seiner Ware trifft. Sie wird als Frist eingetragen und damit von der Termin- und Kapazitätsplanung berücksichtigt. Die Zeit kann in Tagen oder in Stunden eingegeben werden (konfigurierbar). Die Handlingszeit kann bei entsprechenden Konfiguration pro Lieferadresse hinterlegt werden.
*Technische Info: Numerisches Feld, DB-Feld: adr.handlingszeit*

**Ankunftszeit**
Ankunftszeit in HH:MM bei Anlieferung der Ware.
*Technische Info: Numerisches Feld, DB-Feld: adr.ankunftszeit*

**Anlieferstelle**
Platz, wo die Ware bei Anlieferung angefahren wird.
*Technische Info: Numerisches Feld, DB-Feld: adr.anlieferstelle*

**Fax, Tel.**
Faxnummer und Telefonnummer der Adresse.
*Technische Info: numerisches/alphanumerisches Feld, DB-Feld: adr.fax/telefon*

**E-Mail**
Mailadresse.
*Technische Info: Alphanumerisches Feld, DB-Feld: adr.email*

**Std. Route**
Selo-Feld. Falls die Lieferadresse nicht über die im Kundenstamm hinterlegte Standard-Route erreicht werden kann, besteht die Möglichkeit, die Anschrift einer gesonderten Route zuzuordnen.
*Technische Info: `<F9>`, DB-Feld: adr.routenr*

**Bemerkung**
Beliebige Informationen.
*Technische Info: Alphanumerisches Feld, DB-Feld: adr.text1*

> **Adressenlogik**
> Zum Zeitpunkt der Auftragserfassung wird für den betreffenden Kunden in der Regeln die hinterlegte Standard-Lieferanschrift mit der zugehörigen Routennummer übernommen. Wurde dem Kunden eine Standardlieferanschrift mit eigener Routennummer hinterlegt, so wird die im Kundenstamm eingetragene Routennummer übersteuert. Es existieren diverse Abweichungen in dieser Funktion, diese sind meistens konfigurationsabhängig. Bei Fragen, bzw. um weitere Information zu erhalten, wenden Sie sich an den zuständigen A+W Software GmbH Mitarbeiter.

### Hausspezifische Adressdaten
In diesem Dialog können Sie hausspezifische Adressdaten pro Haus hinterlegen. Dieser Dialog erscheint automatisch, wenn Sie die interne Mandantentrennung nutzen und im Dialog Adressen das Feld Entfernung betreten.
⇨ "Adressen" auf Seite B-57

#### Erläuterung der Felder
**Haus**
Auswahl der Hausnummer.
*Technische Info: `<F9>`, DB-Feld: mdzu.hnr*

**Name**
Der Hausbenennung wird im Klartext automatisch angezeigt, wenn Sie das Feld Haus verlassen.

**Entfernung**
Entfernung zur Lieferadresse in km für das aktuellen Haus.
*Technische Info: Numerisches Feld, DB-Feld: adr.kilometer*

**Fahrtzeit**
Dauer der Fahrtzeit zur Lieferadresse in Tagen oder Stunden für das aktuellen Haus.
*Technische Info: Numerisches Feld, DB-Feld: adr.fahrtzeit*

### Bankverbindungen
*Stammdaten > Marktpartner > `<F4>` > Kontaktdaten > Bankverbindungen*

In diesem Dialog werden die marktpartnerspezifischen Bankverbindungen hinterlegt. Dabei können durch `<F6>` weitere Datensätze hinzugefügt werden. Existieren mehrere Bankverbindungen, ist die Hauptbankverbindung mit `<F5>` zu bestimmen.

#### Erläuterung der Felder
**Bankname**
Name des Kreditinstituts.
*Technische Info: Alphanumerisches Feld, DB-Feld: bankv.bname*

**Banksitz**
Sitz des Kreditinstituts.
*Technische Info: Alphanumerisches Feld, DB-Feld: bankv.sitz*

**KFZ Land**
Selo-Feld. Das Länder Kfz-Kennzeichen.
*Technische Info: `<F9>`, DB-Feld: bankv.kfzcode*

**BLZ**
Bankleitzahl des Kreditinstituts.
*Technische Info: Numerisches Feld, DB-Feld: bankv.blz*

**Konto-Nr.**
Kontonummer bei dem Kreditinstitut.
*Technische Info: Numerisches Feld, DB-Feld: bankv.kontonr*

**BIC**
Business Identifier Code.
*Technische Info: Alphanumerisches Feld, DB-Feld: bankv.bic*

**IBAN**
Internationale Bank-Kontonummer.
*Technische Info: Alphanumerisches Feld, DB-Feld: bankv.iban*

### E-Mailadressen
*Stammdaten > Marktpartner > `<F4>` > Kontaktdaten > E-Mailadressen*

In diesem Dialog haben Sie die Möglichkeit, diverse E-Mailadressen zu hinterlegen. Die hinterlegten Daten werden in der zugehörigen Datenbank-Tabelle xemail gepflegt. Diese enthält die Angaben zur E-Mail-Versendung der Formulare. Hier können der MP-Typ, der Marktpartner, die Formularart, der Mitarbeiter bzw. die Abteilung und die E-Mail-Adressen eingegeben werden. Wird ein Mitarbeiter eingetragen, kann keine Abteilung eingetragen werden. Wird eine Abteilung eingegeben, kann kein Mitarbeiter hinterlegt werden. Es ist möglich Werte für einen Marktpartner und einen Mitarbeiter (bzw. eine Abteilung), für einen Marktpartner, eine Formularart und einen Mitarbeiter (bzw. eine Abteilung) oder nur für einen Marktpartner anzulegen. Genau in dieser Reihenfolge wird beim Versenden der Formulare auch die E-Mail-Adresse ermittelt, an die das zum Vorgang gehörige Formular versandt wird.
Die hier hinterlegten Daten beziehen sich immer auf den Vorgang, für den ein Formular versendet werden soll, d.h. die hier hinterlegte Mitarbeiternummer muss mit dem Vorgangserfasser übereinstimmen, damit die entsprechende E-Mail-Adresse ermittelt werden kann.

#### Erläuterung der Felder
**Formular**
Wählen Sie das gewünschte Formular (Angebot, Rechnung, etc.) aus.
*Technische Info: `<F9>`, DB-Feld: xemail.formart*

**Mitarb.**
Wählen Sie die gewünschte Mitarbeiter-Nummer aus. Wenn die E-Mail nicht an einen Mitarbeiters sondern an eine Abteilung gehen soll, dann lassen Sie dieses Feld leer und wählen im Feld Abteilung die entsprechende aus.
*Technische Info: `<F9>`, DB-Feld: xemail.manr*

**Abteilung**
Wählen Sie die Abteilung aus, an die die E-Mail gehen soll. Haben Sie im Feld Mitarb. eine Mitarbeiter-Nummer eingetragen, können Sie in diesem Feld keine Angabe machen.
*Technische Info: `<F9>`, DB-Feld: xemail.abtnr*

**E-Mail**
Geben Sie hier die entsprechende E-Mailadresse ein.
*Technische Info: Alphanumerisches Feld, DB-Feld: xemail.email*

**S**
Handelt es sich bei der E-Mailadresse um eine für diese Formularart stillgelegte E-Mailadresse:
- **J:** Die Mail-Adresse ist für diese Formularart stillgelegt.
- **N:** Die Mail-Adresse ist für diese Formularart aktiv.
*Technische Info: Toggle-Feld, DB-Feld: xemail.still*

**Ergänzende Informationen**
⇨"E-Mailadressen - Detail" auf Seite B-64

### E-Mailadressen - Detail
*Stammdaten > Marktpartner > `<F4>` > Kontaktdaten > E-Mailadressen > F2*

In diesem Dialog werden Ihnen weitere Informationen für zu der ausgewählten E-Mailadresse angezeigt.

#### Erläuterung der Felder
**Partnertyp**
Das Feld wird mit dem Partnertyp vorbelegt, aus dem Sie das Kontextmenü geöffnet haben. Sie können den Typ ändern.
*Technische Info: Toggle-Feld*

**Marktpart.**
Das Feld wird mit dem Marktpartner vorbelegt, aus dem Sie das Kontextmenü geöffnet haben. Sie können den Marktpartner ändern.
*Technische Info: `<F9>`, DB-Feld: xemail.mpnr*

**Formular**
Das Feld wird mit dem Formular vorbelegt, das Sie im Dialog zuvor ausgewählt haben. Sie können das Formular ändern.
*Technische Info: `<F9>`, DB-Feld: xemail.formart*

**Mitarbeiter**
Das Feld wird mit dem Mitarbeiter vorbelegt, den Sie im Dialog zuvor ausgewählt haben. Sie können den Mitarbeiter ändern.
*Technische Info: `<F9>`, DB-Feld: xemail.manr*

**Abteilung**
Das Feld wird mit der Abteilung vorbelegt, die Sie im Dialog zuvor ausgewählt haben. Sie können die Abteilung ändern.
*Technische Info: `<F9>`, DB-Feld: xemail.abtnr*

**E-Mail**
Das Feld wird mit der E-Mailadresse vorbelegt, die Sie im Dialog zuvor eingegeben haben. Sie können die Adresse ändern.
*Technische Info: Alphanumerisches Feld, DB-Feld: xemail.email*

**E-Mail von**
Abweichende Absenderadresse bei Verwendung dieser E-Mailadresse.
*Technische Info: Alphanumerisches Feld, DB-Feld: xemail.emailabs*

**cc**
Zusätzliche CC-Adresse bei Verwendung dieser E-Mailadresse.
*Technische Info: Alphanumerisches Feld, DB-Feld: xemail.cc*

**E-Mail**
Zusätzliche BCC-Adresse bei Verwendung dieser E-Mailadresse.
*Technische Info: Alphanumerisches Feld, DB-Feld: xemail.bcc*

**Versandart**
Versandart des Dateianhangs:
- **0 (Standard):** Pro E-Mail eine PDF-Datei
- **1:** Pro E-Mail mehrere Dateianhänge verwenden
- **2:** Alle Dateianhänge zu einem PDF zusammenfassen.
*Technische Info: Alphanumerisches Feld, DB-Feld: xemail.bcc*

**Passwort**
Hier können Sie ein Passwort vergeben.
*Technische Info: Alphanumerisches Feld, DB-Feld: xemail.passwort*

**Stillgelegt**
Das Feld wird mit dem Flag vorbelegt, das Sie im Dialog zuvor eingestellt haben. Sie können das Flag ändern.
*Technische Info: Toggle-Feld, DB-Feld: xemail.still*

### Rabatte
*Stammdaten > Marktpartner > `<F4>` > Rabatte*

Hier ordnen Sie dem ausgewählten Marktpartner Rabatte zu. Der Dialog wird an folgender Stelle im Schlüsselbereich ausführlich erläutert:
⇨ "Rabatte" auf Seite B-144
Die Werte für die jeweilige Rabattmethode kann pro Marktpartner individuell vereinbart und geändert werden.

### Rabatte - Details
*Stammdaten > Marktpartner > `<F4>` > Rabatte > Details*

Bei diesem Dialog handelt es sich um die Detail-Ansicht der Rabatte. Der Dialog wird an folgender Stelle ausführlich erläutert:
⇨ "Rabatte - Details" auf Seite B-146

### Austausch-/Zusatzregeln
*Stammdaten > Marktpartner > `<F4>` > Austausch-/Zusatzregeln*

Der Menüpunkt Austausch-/Zusatzregeln ermöglicht es, kundenspezifische Regeln, nach denen im Auftrag die Stückliste ergänzt bzw. Teile ausgetauscht werden sollen, für einzelne Artikel oder Artikeltypen zu hinterlegen.
Der Dialog wird an folgender Stelle ausführlich erläutert:
- ⇨"Austausch-/Zusatzregeln" auf Seite B-220
- ⇨"Austausch-/Zusatzregel - Details" auf Seite B-224
- ⇨ "Austausch-/Zusatzregel - Testmodus" auf Seite B-226

### Gestelltypen
*Stammdaten > Marktpartner > `<F4>` > Gestelltypen*

In diesem Dialog legen Sie fest, auf welchen Gestellen die Ware einem Kunden vorzugsweise auszuliefern ist.
Bei Nutzung der prioritätsgesteuerten Packmitteloptimierung kann zusätzlich eine Priorität festgelegt werden, welcher Gestelltyp für den Kunden der wünschenswerteste und welcher eher ungünstig ist. Die Prioritätszahl kann zwischen 1 und 100 gewählt werden und legt damit die Rangfolge der Gestelle fest. Größere Werte bewirken eine Bevorzugung dieses Gestelltyps vor anderen mit niedrigeren Prioritätswerten.
Die hier hinterlegten Informationen nutzt die automatischen Gestellplanung, um den Auftrag unter Beachtung von Scheibengrößen und Limitierungen der Gestelltypen bestmöglich auf vom Kunden bevorzugte Gestelle zu verladen. Für die automatische Gestellplanung kann hier entweder der Gestelltyp oder die Hauptgruppe hinterlegt werden.
Mit `<F2>` erreichen Sie den Gestelltypen-Details Dialog.
⇨ "Gestelltypen - Details" auf Seite B-70

#### Erläuterung der Felder
**Typ**
Auswahl des Gestelltyps. Die Gestelltypen werden im Menüpunkt Gestelltypen (Logistik > Gestellverwaltung > Gestellstamm) hinterlegt. Nach der Auswahl des Gestelltypes wird die dazugehörige Bezeichnung in dem zweiten Feld dargestellt.
*Technische Info: `<F9>`, DB-Feld: kugest.gtypnr*

**Hauptgruppe**
Auswahl der Hauptgruppe. Die Hauptgruppen werden im Menüpunkt Hauptgruppen (Logistik > Gestellverwaltung > Gestellstamm) hinterlegt. Nach der Auswahl der Hauptgruppe wird die dazugehörige Bezeichnung in dem letzten Feld dargestellt. Bei Verwendung der prioritätsgesteuerten Konfiguration ist die Eingabe der Hauptgruppe nicht möglich.
*Technische Info: `<F9>`, DB-Feld: kugest.gtypnr*

**Priorität**
Gestellpriorität aus Sicht des Kunden. Das Feld ist nur bei kundenspezifischen Konfiguration sichtbar.
*Technische Info: Numerisches Feld, DB-Feld: kugest.prioritat*

### Gestelltypen - Details
*Stammdaten > Marktpartner > `<F4>` > Gestelltypen > `<F2>`*

In diesem Dialog können Sie einen kundenspezifischen Packmitteltext hinterlegen und definieren, ob dieser auf der Packmittelbestellung gedruckt werden soll.
Mit `<F2>` kehren Sie zurück in den Hauptdialog:
⇨ "Gestelltypen" auf Seite B-69

#### Erläuterung der Felder
**Text**
Kundenspezifischer Packmitteltext.
*Technische Info: Alphanumerisches Feld, DB-Feld: kugest.kuspectxt/kuspectxt1*

**Bestell-KZ**
Soll der Text auf der Bestellung gedruckt werden:
- Ja
- Nein.
*Technische Info: Toggle-Feld, DB-Feld: kugest.bestelldru/bestelldru1*

### Konfigurierte MP-Felder
*Stammdaten > Marktpartner > `<F4>` > Konfigurierte MP-Felder*

In diesem Dialog wird jedes Feld kundenspezifisch konfiguriert und ausgewertet. Die Felder können unter dem Menüpunkt MP-Feldkonfiguration (Stammdaten > Feldkonfiguration) definiert werden.
⇨ "MP-Feldkonfiguration" auf Seite B-417
Die Auswertung der Felder kann nur individuell gestaltet werden. Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.
Die Daten in oben gezeigten Screenshot dienen an dieser Stelle nur als Beispiel.

### Vertreterzuordnung
*Stammdaten > Marktpartner > `<F4>` > Mitarbeiterzuordnung > Vertreterzuordnung*

In diesem Dialog ist es möglich, einem Kunden mehrere Vertreter (Mitarbeiter) zuzuordnen.
Die Auswahl erfolgt über `<F9>`. Zur Auswahl stehen nur die Mitarbeiter zur Verfügung, denen eine Vertreter-Funktion im Mitarbeiterstamm zugeordnet ist.
Mit `<F5>` kann ein Mitarbeiter als Hauptvertreter (= Außendienstmitarbeiter) festgelegt werden.

#### Erläuterung der Felder
**Pers-Nr**
Auswahl der Mitarbeiternummer. Der Name wird im Feld Vertreter angezeigt.
*Technische Info: `<F9>`, DB-Feld: mitarbzu.manr*

### Erfasserzuordnung
*Stammdaten > Marktpartner > `<F4>` > Mitarbeiterzuordnung > Erfasserzuordnung*

In diesem Dialog ist es möglich, einem Kunden mehrere Erfasser (Mitarbeiter) zuzuordnen. Die Auswahl erfolgt über `<F9>`.

#### Erläuterung der Felder
**Pers-Nr**
Auswahl der Mitarbeiternummer. Im Feld Erfasser wird Ihnen dann der Name angezeigt.
*Technische Info: `<F9>`, DB-Feld: mperfasszu.manr*

**AB-Empfang**
Über dieses Feld steuern Sie, wie der Mitarbeiter Kopien der AB an den Kunden erhalten soll. Folgende Werte sind möglich:
- **nein:** Der Mitarbeiter erhält keine Kopie der AB.
- **per Email:** Der Mitarbeiter erhält die Kopie per E-Mail.
- **per Fax:** Der Mitarbeiter erhält die Kopie per Fax.
*Technische Info: Toggle-Feld, DB-Feld: mperfasszu.abflag*

### Gruppenzuordnung
*Stammdaten > Marktpartner > `<F4>` > Gruppenzuordnung*

In diesem Dialog kann ein Kunde über `<F9>` verschiedenen Gruppen zugeordnet werden. Die Pflege der Gruppen-Schlüssel erfolgt im Menü Gruppen (Stammdaten > Marktpartner).
Den verschiedenen Marktpartnergruppen können im Rahmen der Textverarbeitung (Stammdaten > Textverwaltung > Gruppentexte) diverse Texte zugeordnet werden, die auf den marktpartnerseitigen Papieren ihre Ausgabe finden. Damit kann beispielsweise die Marktpartnergruppe der Fensterbauer über die Einführung eines neuen Isolierglasproduktes informiert werden.

#### Erläuterung der Felder
**Gruppe**
Auswahl des Gruppenschlüssels. Im Feld Bezeichnung wird Ihnen dann der Name angezeigt.
*Technische Info: `<F9>`, DB-Feld: grpzu.grpnr*

**Klasse**
Gruppenklassifikation. Über die definierte Klasse können Sie statistische Auswertungen durchführen.
*Technische Info: Numerisches Feld, DB-Feld: grpzu.klasskz*

### Objektzuordnung
*Stammdaten > Marktpartner > `<F4>` > Objektzuordnung*

In diesem Dialog können einem Kunden ein oder mehrere Objekte, (z. B. Großbaustellen) zugeordnet werden. Die Objekte werden über `<F9>` angezeigt und über ihre Objektnummer eingetragen.
Mit `<F3>` öffnen Sie den Dialog für die kundenindividuellen Objekttexte, in dem Sie die Objekttexte zuweisen und bestimmen, auf welchen Papieren der Text gedruckt wird.
Mit `<F5>` definieren Sie das Standard-Objekt.

#### Erläuterung der Felder
**Objekt**
Auswahl der Objektnummer. Im Feld Objektbezeichnung wird Ihnen der Name des Objekts angezeigt.
*Technische Info: `<F9>`, DB-Feld: okkond.objnr*

**Ergänzende Informationen**
⇨ "Objekttexte" auf Seite B-76

### Objekttexte
*Stammdaten > Marktpartner > `<F4>` > Objektzuordnung > `<F3>`*

In diesem Dialog weisen Sie einen Objekttext zu und bestimmen, auf welchen Papieren der Text gedruckt wird.

#### Erläuterung der Felder
**Datei**
Auswahl der Textdatei, in der die Texte gespeichert werden. Wenn Sie einen neuen Dateinamen eingeben, öffnet sich der Dialog Stammtexte, in dem Sie den neuen Text eingeben können.
*Technische Info: `<F9>`, DB-Feld: objtxtzu.datei*

**Nr**
Über dieses Feld steuern Sie die Reihenfolge, in der die Objekttexte gedruckt werden.
*Technische Info: `<F5>`, DB-Feld: objtxtzu.lfdnr*

**Druckposition**
Auswahl der Druckposition:
- Kopftext
- Fußtext
*Technische Info: Toggle-Feld, DB-Feld: objtxtzu.ludrupos*

> **Formulare**
> Mit `<F5>` legen Sie fest, auf welchen Formulararten (Auftragsbestätigung, Rechnung, etc.) die Dateien in der hier angegebenen Reihenfolge gedruckt wird.

**Ergänzende Informationen**
⇨ "Stammtexte" auf Seite B-82

### Farbzuordnung
*Stammdaten > Marktpartner > `<F4>` > Farbzuordnung*

Dieser Dialog ist nur für Marktpartnertyp=Lieferant verfügbar. Hier hinterlegten Daten sind für den BMECat-Stammdaten-Import relevant. Dabei handelt es sich um eine Applikation zum Import von Artikel-Stammdaten von Lieferante. Beim Import einer neuen Lieferanten-Stammdaten-Datei wird anhand der korrespondierenden Tabelle lieffarzu überprüft, ob die Farben eines zu importierenden Artikels bereits im System als AWE-Farben angelegt sind oder nicht. Wenn erkannt wird, dass eine Lieferanten-Farbe noch nicht als AWE-Farbe angelegt ist, wird sie während des Imports angelegt.
Der Dialog liefert dann dem Benutzer die Übersicht aller angelegten Lieferanten-Farben.
Es kann auch vorkommen, dass für eine Bestellung bei einem Lieferanten eine Farbe benötigt wird, die noch nicht angelegt ist, weil nach dem letzten Lieferanten-Stammdaten-Import vom Lieferanten noch neue Farben zur Verfügung gestellt wurden. In diesem Fall kann über den Dialog die neue Lieferanten-Farbe manuell angelegt werden, um die Bestellung zu erfassen.

#### Erläuterung der Felder
**Nr**
Farbnummer. Die Farben werden im Menüpunkt Farben (Stammdaten > Schlüssel > Produkte > Varianten > Farben) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: lieffarbzu.farbnr*

**AWE-Farbe**
AWE Farbbezeichnung. Nach der Farbnummerauswahl wird die entsprechenden Bezeichnung in diesem Feld angezeigt.
*Technische Info: `<F9>`, DB-Feld: lieffarbzu.farbnr*

**Nr**
Farbnummer des Lieferanten.
*Technische Info: `<F9>`, DB-Feld: lieffarbzu.lifarbnr*

**Lieferantenfarbe**
Farbbezeichnung des Lieferanten
*Technische Info: `<F9>`, DB-Feld: lieffarbzu.lifarbbez*

### Bonuszuordnung
*Stammdaten > Marktpartner > `<F4>` > Bonuszuordnung*

In diesem Dialog können Sie einem Marktpartner einen Bonus zuordnen.

#### Erläuterung der Felder
**Rang**
Angabe zur Priorität. Mit diesem Feld wird die Zuordnung in der Auftragserfassung zu den einzelnen Auftragsposition gesteuert. Die niedrigste Rangnummer mit den meisten übereinstimmenden Stellen in der Warengruppe wird hier herangezogen.
*Technische Info: Numerisches Feld, DB-Feld: bonuszu.rang*

**WagrpCode**
Über dieses Feld können Sie den Bonus einer bestimmten Warengruppe oder einem Warengruppen-Bereich zuordnen.
*Technische Info: `<F9>`, DB-Feld: bonuszu.wagrp*

**Bemerkung**
Hier kann eine Bemerkung hinterlegt werden, z. B. warum ein Bonus vergeben wurde.
*Technische Info: Alphanumerisches Feld, DB-Feld: bonuszu.txt*

**Bonus**
Auswahl des gewünschten Bonus. Die entsprechenden Schlüssel werden über das Menü Bonus (Schlüssel > Marktpartner > Bonus) vergeben.
*Technische Info: `<F9>`, DB-Feld: bonuszu.bonusnr*

### Artikelzuordnung
*Stammdaten > Marktpartner > `<F4>` > Artikelzuordnung*

In diesem Dialog können Sie einem Marktpartner mehrere Artikel mit spezifischen Angaben zuordnen. Die Artikel werden über `<SELO>` (`<F9>`) angezeigt und über ihre Artikelnummer eingetragen.

#### Erläuterung der Felder im Register Übersicht
**Artikel**
Auswahl der Artikelnummer.
*Technische Info: `<F9>`, DB-Feld: artkuzu.artnr*

**Bezeichnung**
Artikelbezeichnung.

**Artikeltyp**
Artikeltyp des ausgewählten Artikels.

**Ext.Artikel**
Artikelnummer des Marktpartners. Über diese Nummer kann die Auftragsposition direkt erfasst werden.
*Technische Info: Alphanumerisches Feld, DB-Feld: artkuzu.kuartnr*

**Externe Artikelbezeichnung**
Artikelbezeichnung des Marktpartners.
*Technische Info: Alphanumerisches Feld, DB-Feld: artkuzu.kuartbez*

**Preis**
Kundenartikelpreis. Je nach Preistyp wird dieser dann im Auftrag berechnet.
*Technische Info: Numerisches Feld, DB-Feld: artkuzu.preis*

**Preistyp**
Preistyp:
- **WE/Stück:** Währungseinheit je Stück.
- **WE/ME:** Währungseinheit je Mengeneinheit
*Technische Info: Toggle-Feld, DB-Feld: artkuzu.ptyp*

#### Erläuterung der Felder im Register Details
**Wunschlieferant**
In diesem Feld können Sie den Wunschlieferanten des Marktpartners für Zukaufsartikel wählen.
*Technische Info: `<F9>`, DB-Feld: artkuzu.liwunsch*

**Zusatzbezeichnung**
In diese Felder können Sie die marktpartnerspezifische Zusatzbezeichnung für den Artikel eingeben. Ihnen stehen hierfür drei Felder zur Verfügung. Das Feld betreten Sie mit `<Enter>`.
Die hier eingegebene Bezeichnung übersteuert für diesen Kunden die Artikelbezeichnung in der Vorgangsverwaltung.
*Technische Info: Alphanumerische Felder, DB-Felder: artkuzu.zusatz1, artkuzu.zusatz2, artkuzu.zusatz3*

**EAN-Code**
In diesem Feld können Sie den marktpartnerspezifischen EAN-Code für diesen Artikel hinterlegen. Dieser wird auf den kundenseitigen Papieren ausgedruckt. Der EAN-Code kann für die Umsetzung von externen Artikeln in A+W Enterprise-Artikel innerhalb der automatischen Auftragsübernahme genutzt werden.
*Technische Info: Numerisches Feld, DB-Feld: artkuzu.eancode*

**Rahmentextnummer**
In diesem Feld können Sie eine marktpartnerspezifische Rahmentextnummer für einen ISO-Artikel eingeben. Die Textformel wird im Menü Textverwaltung > Textgenerierung > Textformel hinterlegt.
Diese Formel wird in der Vorgangserfassung bei der Textgenerierung ausgewertet und auf den Rahmen gedruckt.
*Technische Info: Numerisches Feld, DB-Feld: artkuzu.rahmtxtnr*

**Maß 1-20**
In diesen Feldern können Sie marktpartnerspezifische Artikelbemaßungen hinterlegen. Diese übersteuern dann die Werte aus den Parametern, die bei der Artikel-Vermaßung für diesen Artikel eingegeben wurden.

> **Es findet keinerlei Plausibilitätsprüfung statt!**
> Die Eingaben, die Sie hier machen, müssen sinnvoll sein.

*Technische Info: numerische Felder, DB-Felder: artkuzu.gv1 – artkuzu.gv20*

### Marktpartnertexte
*Stammdaten > Marktpartner > `<F4>` > Texte / Druck > Marktpartnertexte*

In diesem Dialog ordnen Sie Marktpartnertexte für den Ausdruck auf den Formularen zu.
Mit `<F3>` öffnen Sie einen Dialog, in dem Sie die Stammtexte hinterlegen können.

> **Formulare**
> Mit `<F5>` legen Sie fest, auf welchen Formulararten (Auftragsbestätigung, Rechnung, etc.) diese Datei in der hier angegebenen Reihenfolge gedruckt wird.

#### Erläuterung der Felder
**Datei**
Auswahl oder Eingabe der Textdatei, in der die Texte gespeichert werden.
*Technische Info: `<F9>`, DB-Feld: kltxtzu.dateiname*

**Nr.**
Über dieses Feld steuern Sie die Reihenfolge, in der die Marktpartnertexte gedruckt werden.
*Technische Info: `<F5>`, DB-Feld: kltxtzu.lfdnr*

**Druckposition**
Auswahl der Druckposition:
- **Kopftext:** Die Datei wird im Formularkopf gedruckt.
- **Fußtext:** Die Datei wird im Formularfuß gedruckt.
*Technische Info: Toggle-Feld, DB-Feld: kltxtzu.ludrupos*

**Ergänzende Informationen**
⇨ "Stammtexte" auf Seite B-82

### Stammtexte
*Stammdaten > Marktpartner > `<F4>` > Texte / Druck > Marktpartnertexte > `<F3>`*

In diesem Dialog werden Textblöcke neu erfasst und gleichzeitig in mehreren Sprachen für den Ausdruck der Formulare verwaltet. Damit ist es beispielsweise möglich, Weihnachtsgrüße, allgemeine Kundenhinweise oder Werbeaktionen textuell zu hinterlegen, um sie auf den kundenseitigen Papieren auszugeben.

#### Erläuterung der Felder
**Datei**
Name der Textdatei, in der die Texte gespeichert werden.
*Technische Info: Alphanumerisches Feld, DB-Feld: xtxtnr.datei*

**Sprache**
Auswahl der Sprache. Es stehen nur die Sprachen zur Auswahl, die im Systemstammdaten hinterlegt sind (Stammdaten > Schlüssel > System > Sprachen)
*Technische Info: `<F9>`, DB-Feld: xtxtnr.sprkz*

**Text**
Eingabe des entsprechenden Textes. Mehrzeilige Eingaben sind möglich. Eingabe in einer Zeile ist maximale 160 Zeichen möglich. Die einzelne Zeilen werden mithilfe der Sequenznummer unterschieden.
*Technische Info: Alphanumerisches Feld, DB-Feld: stammtxt.stammtxt, stammtxt.seqnr*

**Ergänzende Informationen**
⇨ "Marktpartnertexte" auf Seite B-81

### Marktpartner-Artikeltexte
*Stammdaten > Marktpartner > `<F4>` > Texte / Druck > MP-Artikeltexte*

Dieser Dialog dient der Hinterlegung marktpartnerspezifischer Artikeltexte in verschiedenen Sprachen. Diese Texte können in Abhängigkeit des Kundensprachkennzeichens auf den Formularen ausgegeben werden.

#### Erläuterung der Felder
**Artikel**
Auswahl der entsprechenden Artikelnummer. Im Feld dahinter erscheint die Artikelbezeichnung.
*Technische Info: `<F9>`, DB-Feld: artxtzu.artnr*

**Datei**
Name der Textdatei, in der die Texte gespeichert werden. Mit `<F3>` wechseln Sie in den Dialog Stammdaten, in dem neue Texte hinterlegt werden können.
*Technische Info: Alphanumerisches Feld, DB-Feld: artxtzu.datei*

### Formulare
*Stammdaten > Marktpartner > `<F4>` > Texte / Druck > Formulare*

In diesem Dialog besteht die Möglichkeit, einen kundenindividueller Report für die bestehende Formularart zu hinterlegen.

#### Erläuterung der Felder
**Formular**
Wählen Sie die gewünschte Formularart (Angebot, Rechnung, etc.) aus. Die Bezeichnung wird im Feld Bezeichnung angezeigt.
*Technische Info: `<F9>`, DB-Feld: kundruckanz.formart*

**Exemplare**
bestimmt die kundenspezifische standardmäßige Ausgabenanzahl des Formulars.
*Technische Info: Numerisches Feld, DB-Feld: kundruckanz.anzahl*

**Komm**
Mit diesem Feld steuern Sie, ob Kommissionstexte ausgegeben werden sollen.
- `☑` Kommissionstexte werden gedruckt.
- `☐` Kommissionstexte werden nicht gedruckt.
*Technische Info: Toggle-Feld, DB-Feld: kundruckanz.kommdrkz*

**Reportname**
Abweichender, kundenspezifische Reportname.
*Technische Info: Alphanumerisches Feld, DB-Feld: kundruckanz.repname*

### Dokumentenarten
*Stammdaten > Marktpartner > `<F4>` > Texte / Druck > Dokumentenarten*

In diesem Dialog können Sie verschiedene Dokumentenarten und die Art der Ausgabe hinterlegen. Der Dialog wird an folgender Stelle ausführlich erläutert:
⇨ "Dokumentenarten" auf Seite B-161

### Vorgangs-Recherche
*Stammdaten > Marktpartner > `<F4>` > Vorgangsrecherche*

Die Benutzung der Vorgangs-Recherche wurde bereits ausführlich in den Kapiteln Verkauf und Einkauf behandelt, und kann dort nachgelesen werden!

### Marktpartner-Info
*Stammdaten > Marktpartner > `<F4>` > Marktpartner-Info*

Unter diesem Menüpunkt werden verschiedene statistische Informationen über den Marktpartner geführt:
- Beträge offene Posten bei einer FIBU-Anbindung
- Beträge nicht beglichener Rechnungen (offene Posten)
- Beträge noch nicht berechneter Aufträge
- Datum, Nummer, Haus und Betrag für den letzten Auftrag, das letzte Angebot und die letzte Rechnung
- Summe des aufgelaufenen Umsatz im aktuellen Jahr.

#### Erläuterung der Felder
**Kunde**
Auswahl der Kundennummer. Der Kundennamen wird nach der Nummerauswahl im Klartext angezeigt.
*Technische Info: `<F9>`, DB-Feld: kuplus.kunr*

> **Marktpartner-Info**
> Die Felder in diesem Dialog dienen der Information und sind nicht änderbar. Die Beträge werden aus der Datenbanktabelle kuplus entnommen. Die restliche Felder werden aktuell aus dem Tagesgeschäft ermittelt und angezeigt.

### Replikationsdaten
*Stammdaten > Marktpartner > `<F4>` > Replikationsdaten*

Je nach Konfiguration können Sie in diesem Dialog eine Limitverteilung für die einzelnen Niederlassungen vornehmen.

#### Erläuterung der Felder
**ges. Limit**
Anzeige des Firmenlimits. Der Wert kommt aus dem Feld Firmenlimit (Stammdaten > Marktpartner > Register Limits).
*Technische Info: Anzeigefeld*

**ges. AKV-Limit**
Anzeige des AKV-Limits. Der Wert kommt aus dem Feld AKV-Llimit (Stammdaten > Marktpartner > Register Limits).
*Technische Info: Anzeigefeld*

**Haus**
Auswahl des Mandanten, für den die Limitdaten gelten sollen.
*Technische Info: `<F9>`, DB-Feld: limits.hausnr*

**Limit**
Firmenlimit für den entsprechenden Mandanten. Wenn Sie das Feld verlassen, wird Ihnen im Feld dahinter der Prozentsatz angezeigt, den dieser Wert im Verhältnis zum gesamt Limit darstellt.
*Technische Info: `<F9>`, DB-Feld: limits.limit*

**AKV-Limit**
AKV-Firmenlimit für den entsprechenden Mandanten. Wenn Sie das Feld verlassen, wird Ihnen im Feld dahinter der Prozentsatz angezeigt, den dieser Wert im Verhältnis zum gesamten AKV-Limit darstellt.
*Technische Info: `<F9>`, DB-Feld: limits.akvlimit*

**Route**
Auswahl der Route. Im Feld dahinter wird Ihnen die Routenbezeichnung angezeigt. Die Routen und ihre Bezeichnungen werden unter Stammdaten > Schlüssel > System > Versand > Routen > Routen hinterlegt.
*Technische Info: `<F9>`, DB-Feld: limits.routenr*

**Def. Haus**
Default-Haus für den Mandaten. Mit `<F5>` können Sie das aktuelle Haus als Default-Haus für alle Einträge wählen.
*Technische Info: `<F9>`, DB-Feld: limits.defhausnr*

> **Gesamtwerte**
> Es können weder das gesamte Limit noch das gesamte AKV-Limit überschritten werden. Bei einer Überschreitung erfolgt eine entsprechende Meldung.

> **Unterer Dialogbereich**
> Am unteren Dialogbereich werden Ihnen die aufsummierten Werte sowohl für die Beträge als auch für die Prozentwerte angezeigt.

### DFÜ-Konfiguration
*Stammdaten > Marktpartner > `<F4>` > DFÜ-Konfiguration*

In diesem Dialog konfigurieren Sie die Steuerung der DFÜ.
Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH

#### Erläuterung der Felder
**Partnertyp**
Auswahl des Partnertyps.
*Technische Info: `<F9>`, DB-Feld: mpdfuectrl.kuliflag*

**Marktpartner**
Auswahl der Marktpartnernummer. Nach der Nummerauswahl wird der Kundenname im Klartext dargestellt.
*Technische Info: `<F9>`, DB-Feld: mpdfuectrl.mpnr*

**Typ der DFÜ**
Auswahl der DFÜ-Art. Im Feld dahinter wird Ihnen die Bezeichnung angezeigt. Typ der DFÜ entscheidet über die Art und Weise der Datenübertragung und soll somit sehr gewissenhaft bestimmt werden. Die Auswahl können Sie bereits im Dialogkopf treffen. In diesem Fall können neue Konfigurationseinträge auch nur für diesen Typ der DFÜ erfolgen.
*Technische Info: `<F9>`, DB-Feld: mpdfuectrl.dfuetyp*

**Steuerungstyp**
Steuerungstyp der DFÜ. Im Feld dahinter wird Ihnen die Bezeichnung angezeigt.
*Technische Info: `<F9>`, DB-Feld: mpdfuectrl.id*

**Wert**
Steuerungswert.
- `☑` Der DFÜ-Typ ist aktiv.
- `☐` Der DFÜ-Typ ist nicht aktiv.
*Technische Info: `<F9>`, DB-Feld: mpdfuectrl.value*

### Hausspezifische Angaben
*Stammdaten > Marktpartner > `<F4>` > Hausspezifische Angaben*

Die hausspezifischen Angaben werden für das Mehr-Mandantensystem (Multi-Site) verwendet. Hier können Sie den unterschiedlichen Häusern einzelne Vertreter und Konditionsdebitoren zuordnen.

#### Erläuterung der Felder
**Haus**
Auswahl der Hausnummer.
*Technische Info: `<F9>`, DB-Feld: mdzu.hnr*

**Name**
Der Hausbenennung wird im Klartext automatisch angezeigt, wenn Sie das Feld Haus verlassen.

**Vertr. (Erlös)**
Auswahl des erlösmäßigen Vertreters. Für den hier eingetragenen Mitarbeiter werden dann die jeweiligen Provisionssätze gebucht und stehen zur Abrechnung bereit.
*Technische Info: `<F9>`, DB-Feld: mpmdzu.lager*

**Name**
Der Name des erlösmäßigen Vertreters wird im Klartext automatisch angezeigt, wenn Sie das Feld Vertr. (Erlös) verlassen.

**Konditions-Debitor**
Auswahl der Kundennummer, deren Konditionen für die erfassten Vorgänge gelten soll.
*Technische Info: `<F9>`, DB-Feld: mpmdzu.konddebnr*

**Name**
Der Kundenname wird im Klartext automatisch angezeigt, wenn Sie das Feld Konditionsdebitor verlassen.
*Technische Info: `<F9>`, DB-Feld: mp.name*

**MwSt**
Auswahl einer Mehrwertsteuer. Wenn die Mandanten in verschiedenen Mwst-Bereiche befinden, kann hier für einen Marktpartner die abweichende Mwst festgelegt werden.
*Technische Info: `<F9>`, DB-Feld: mpmdzu.mwst*

**MwSt (%)**
Nach der MwSt-Auswahl wird hier die Bezeichnung im Klartext dargestellt.
*Technische Info: `<F9>`, Anzeige-Feld*

## Mitarbeiter
*Stammdaten > Mitarbeiter*

Im Mitarbeiterstamm werden alle identifizierenden Angaben (wie z B. Personalnummer, Name, Zeichen, etc.) für die Mitarbeiter, Systemdienste und Berechtigungsgruppen festgelegt.
Darüber hinaus werden alle EDV-Rechte und Einschränkungen, die den Mitarbeiter oder eine Berechtigungsgruppe betreffen, hinterlegt. So kann sichergestellt werden, dass die Mitarbeiter nur Zugang zu bestimmten Bereichen und entsprechende Berechtigungen in A+W Enterprise bekommen.
In diesem Kapitel finden Sie Informationen zu folgenden Themen:
- "Mitarbeiter / Berechtigungsgruppen" auf Seite B-93
- "Mitarbeiter - Rechte" auf Seite B-98

### Mitarbeiter / Berechtigungsgruppen
*Stammdaten > Mitarbeiter*

In diesem Dialog werden alle Angaben zu Mitarbeitern, Mitarbeitergruppen und System-Dienste hinterlegt.

#### Erläuterung der Felder im Bereich Personendaten
**Pers.-Nr.**
Auswahl der Personalnummer. Bei der Neuaufnahme geben Sie die gewünschte Nummer ein.
*Technische Info: `<F9>`, DB-Feld: mitarb.manr*

**Typ**
Dieses Feld spezifiziert die Art des Stammdatensatzes. Folgende Werte sind möglich:
- **Mitarbeiter:** Jede Personalnummer kann nur einmal vergeben werden. Mit der `<F6>`-Taste haben Sie die Möglichkeit, die nächsten freie Nummer durch das System zu vergeben.
- **Systemdienst:** Als Systemdienst sollte ein Mitarbeitersatz mit Personalnummer -1 angelegt werden. Die Existenz dieses Satzes ist notwendig, da sich alle A+W Enterprise-Hintergrundprozesse (z. B. Hintergrund-Auftragsbearbeitung, etc.) mit Mitarbeiternummer -1 melden.
- **Berechtigungsgruppe:** Eine Berechtigungsgruppe wird mit Programmzugangsrechten für einen bestimmten Personalbereich angelegt. Mitarbeitern des Aufgabengebietes wird daraufhin im Feld Berechtigungsgruppe die vergebene Gruppennummer zugeordnet. Damit entfällt die Vergabe der einzelnen gruppenspezifischen Modulzugangsberechtigungen für jeden einzelnen Mitarbeiter.
*Technische Info: Toggle-Feld, DB-Feld: mitarb.matyp*

**Name**
Nachname des Mitarbeiters. Mit `<F5>` öffnen Sie den Dialog Anmerkungstexte, in dem Sie die Informationen zu dem Mitarbeiter hinterlegen können. Mit `<F3>` öffnen Sie den Dialog für die Übersicht über Mitarbeiterrechte.
*Technische Info: alphabetisches Feld, DB-Feld: mitarb.maname*

> **Mitarbeiter- und Abteilungs-Anmerkungen**
> Mitarbeiter- und Abteilungs-Anmerkungen mit Priorität hoch und Ort überall können direkt beim Starten des A+W Enterprise-Hauptmenü oder beim Start des Moduls Versand angezeigt werden. So können wichtige mitarbeiterbezogene Informationen beim Start präsentiert werden. Ihr System muss entsprechend konfiguriert werden.

**Vorname**
Vorname des Mitarbeiters.
*Technische Info: alphabetisches Feld, DB-Feld: mitarb.mavname*

**Geschl.**
Toggle-Feld. Geschlecht des Mitarbeiters.
- weiblich
- männlich
*Technische Info: Toggle-Feld, DB-Feld: mitarb.sex*

**Anrede**
Auswahl der Anrede. Die entsprechenden Schlüssel werden über das Menü Anreden (Stammdaten > Schlüssel > Marktpartner) vergeben.
*Technische Info: `<F9>`, DB-Feld: mitarb.anrede*

**Geb.-Dat.**
Geburtsdatum des Mitarbeiters.
*Technische Info: Numerisches Feld, DB-Feld: mitarb.gebdat*

**Zeichen**
Schriftkürzel des Mitarbeiters.
*Technische Info: Alphanumerisches Feld, DB-Feld: mitarb.zeichen*

#### Erläuterung der Felder im Bereich Letzte Änderung
**Name**
In diesem Feld wird Ihnen der Mitarbeiter angezeigt, der den Stammdatensatz zuletzt geändert hat.

**Datum**
In diesem Feld wird Ihnen das Datum angezeigt, an dem der Stammdatensatz zuletzt geändert wurde.

#### Erläuterung der Felder im Bereich Anmeldeinformationen
**Login**
A+W Enterprise-Loginname, der zusammen mit dem Passwort zum Programmstart berechtigt. In der Nutzung von A+W Enterprise - Webanwendung sowie auch A+W iQuote wird hier eingetragener Name ebenfalls zur Anmeldung verwendet.
*Technische Info: Alphanumerisches Feld, DB-Feld: mitarb.loginname*

**Passwort**
Passwort, das zusammen mit dem A+W Enterprise-Loginname zum Programmstart berechtigt. Das Passwort kann nur vom Administrator eingetragen bzw. geändert werden. Für die Nutzung der A+W Enterprise - Standard-Anwendung wird das Passwort über die Unix bzw. Linux-Administrator vergeben. Das Passwort aus diesem Feld berechtigt zur Anmeldung in der A+W Enterprise - Webanwendung bzw. A+W iQuote.

#### Erläuterung der Felder im Bereich Einschränkungen
**Shell**
Shellberechtigung. Soll auch die Betriebssystemebene zugänglich sein, so aktivieren Sie bitte diese Checkbox.
*Technische Info: Toggle-Feld, DB-Feld: mitarb.shjn*

**Abteilungseinschränkung**
Ist diese Checkbox aktiv, werden diverse Auswertungen (z, B. Liste der unberechneten Aufträge, Produktionsfreigabe, etc.) auf die Vorgänge der dem Mitarbeiter zugeordneten Abteilung eingeschränkt.
*Technische Info: Toggle-Feld, DB-Feld: mitarb.abtview*

**Mandanteneinschränkung**
Ist diese Checkbox aktiv, werden diverse Auswertungen (z. B. Liste der unberechneten Aufträge, Produktionsfreigabe, etc.) auf die Vorgänge des Mandanten eingeschränkt.
*Technische Info: Toggle-Feld, DB-Feld: mitarb.hausview*

#### Erläuterung der Felder im Bereich Mitarbeiter-/Kontaktdaten
**Durchwahl**
Interne Telefondurchwahl.
*Technische Info: Numerisches Feld, DB-Feld: mitarb.durchw*

**Fax**
Nummer des Faxgerätes.
*Technische Info: Numerisches Feld, DB-Feld: mitarb.faxnr*

**E-Mail**
E-Mail-Adresse des Mitarbeiters.
*Technische Info: Alphanumerisches Feld, DB-Feld: mitarb.email*

**Mandant**
Werks- bzw. Niederlassungsnummer (Hauptmandant). Mit `<Umschalt>` + `<F5>` öffnen Sie den Dialog für die Hauszuordnung. Dort können Sie dann weitere Häuser dem Mitarbeiter zuordnen.
*Technische Info: Alphanumerisches Feld, DB-Feld: mitarb.hnr*

**Position**
Auswahl der Position des Mitarbeiters.
*Technische Info: `<F9>`, DB-Feld: mitarb.pos*

**Funktion**
Auswahl, ob der Mitarbeiter als Geschäftsführer oder Vertreter tätig ist. So können z. B. nur Personen, die als Vertreter gekennzeichnet sind, als solche im Kundenstamm einem Kunden zugeordnet werden.
*Technische Info: `<F9>`, DB-Feld: mitarb.funktion*

**Mail zu**
Auswahl der Mitarbeiter-Nummer für die Weiterleitung einer E-Mail.
*Technische Info: `<F9>`, DB-Feld: mitarb.vertretung*

**Aktivieren**
Über diese Checkbox aktivieren Sie die E-Mail Weiterleitung.
*Technische Info: Toggle-Feld, DB-Feld: mitarb.vertr_aktiv*

**Abteilung**
Nummer der Abteilung. Aus statistischen Programmzugriffsgründen sollte jeder Mitarbeiter einer Abteilung zugeordnet werden. Im Feld dahinter wird dann die Abteilung angezeigt. Die entsprechenden Abteilungen werden über das gleichnamige Menü vergeben.
*Technische Info: `<F9>`, DB-Feld: mitarb.abtnr*

**Kunde**
Hier können Sie dem Mitarbeiter einen Kunden zuordnen.
*Technische Info: `<F9>`, DB-Feld: mitarb.manrkunr*

**Externer Mitarbeiter**
Aktivieren Sie die Checkbox, wenn es sich bei dem Mitarbeiter um einen externen Mitarbeiter (mit eingeschränkten Rechten) handelt.
*Technische Info: Toggle-Feld, DB-Feld: mitarb.externflag*

**SQL-Berechtigungsgruppe**
Auswahl der Berechtigungsgruppe.
*Technische Info: `<F9>`, DB-Feld: mitarb.logingrp*

#### Erläuterung der Felder im Bereich Rechtegruppen
**Gruppe**
Auswahl der Gruppennummer. Im Feld dahinter wird die Bezeichnung angezeigt. Damit entfällt die Vergabe der einzelnen gruppenspezifischen Modulzugangsberechtigungen für jeden einzelnen Mitarbeiter.
*Technische Info: `<F9>`, DB-Feld: bengrpzu.grp*

**Haus**
Auswahl der zugeordneten Hausnummer.
*Technische Info: `<F9>`, DB-Feld: bengrpzu.hausnr*

#### Erläuterung der Felder im Bereich Rechte
**EDV-Modul**
Auswahl des EDV-Moduls, in dem der Mitarbeiter seine EDV-Rechte ausüben kann. `*` steht für alle Programm-Module. Im weiteren Feld wird die Modulbezeichnung im Klartext dargestellt. Mit `<F9>` können Sie nach bestimmten Modul suchen. Für die Übersicht über alle Modulen und deren Bedeutung wenden Sie sich an A+W Software GmbH - Mitarbeiter.
*Technische Info: `<F9>`, DB-Feld: login.modul*

**Terminal**
Auswahl des Terminals bzw der Terminalgruppe, an dem der Mitarbeiter für das jeweilige Modul zugelassen ist. `*` steht für alle Terminals.
*Technische Info: `<F9>`, DB-Feld: login.ort*

**Rechte**
Auswahl der Mitarbeiterrechte:
- **-:** Keine Rechte.
- **r:** Leserecht
- **w:** Schreibrecht
*Technische Info: Toggle-Feld, DB-Feld: login.rwx*

**Haus**
Auswahl der zugeordneten Hausnummer, in der diese Einschränkung gilt (für Multi-Site-Systeme). Die hausindividuelle Einschränkungen können nur bei lokalen Rechten vorgenommen werden. Für weitere Informationen wenden Sie sich an A+W Software GmbH - Mitarbeiter.
*Technische Info: `<F9>`, DB-Feld: login.hausnr*

### Mitarbeiter - Rechte
*Stammdaten > Mitarbeiter > Rechte (Übersicht) `<F3>`*

In diesem Dialog geben Sie die Mitarbeiternummer und die Hausnummer ein, zu dem Sie die Rechte sehen möchten.

#### Erläuterung der Felder
**Mitarbeiter**
Eingabe der Mitarbeiternummer.
*Technische Info: Numerisches Feld*

**Haus**
Eingabe der Hausnummer.
*Technische Info: Numerisches Feld*

Wenn Sie den Dialog mit [OK] verlassen, werden Ihnen im nächsten Dialog die gewünschten Informationen angezeigt:

#### Erläuterung der Felder
**Modul**
Anzeige der Modulnummer. Ein `*` kennzeichnet alle Module.
*Technische Info: Anzeige-Feld*

**Recht**
Anzeige des Rechtes:
- **-:** Keine Rechte.
- **r:** Leserecht
- **w:** Schreibrecht
*Technische Info: Anzeige-Feld*

**User/Gruppe**
Hier sehen Sie, ob es sich um ein User-Recht oder ein Gruppen-Recht handelt:
- **U:** User-Recht
- **G:** Gruppen-Recht
*Technische Info: Anzeige-Feld*

**Drucken**
Über diese Schaltfläche können Sie sich die Übersicht der Mitarbeiterrechten ausdrucken.

## Abteilungen
- Stammdaten > Abteilungen > Abteilungen
- Stammdaten > Abteilungen > Einzelne Bezeichnung
- Stammdaten > Abteilungen > Alle Bezeichnung

In diesem Dialog werden alle die identifizierenden Angaben (wie z. B. Bezeichnung, Kürzel usw.) für die Abteilungen im Unternehmen festgelegt.

> **Mehrsprachige Bezeichnungen**
> Seit QR2209 können Sie in A+W Enterprise auch für Abteilungen mehrsprachige Bezeichnungen hinterlegen.

Mit `<F5>` öffnen Sie den Dialog Anmerkungstexte, in dem Sie die Informationen zu der Abteilung hinterlegen können.

> **Mitarbeiter- und Abteilungs-Anmerkungen**
> Mitarbeiter- und Abteilungs-Anmerkungen mit Priorität hoch und Ort überall können direkt beim Starten des A+W Enterprise-Hauptmenü oder beim Start des Moduls Versand angezeigt werden. So können wichtige mitarbeiterbezogene Informationen beim Start präsentiert werden. Ihr System muss entsprechend konfiguriert werden.

### Erläuterung der Felder
**Abteilung**
Auswahl der Abteilung.
*Technische Info: `<F9>`, DB-Feld: abteilung.abtnr*

**Kürzel**
Stellt eine Abkürzung der Bezeichnung dar.
*Technische Info: Alphanumerisches Feld, DB-Feld: abteilung.abtid*

**Bezeichnung**
Abteilungsbezeichnung. Die Bezeichnung kann überschrieben werden.
*Technische Info: Alphanumerisches Feld, DB-Feld: abteilung.bez*

**Kostenstelle**
Auswahl der Kostenstelle. Der Eintrag kann zu statistischen Zwecken genutzt werden. Die entsprechenden Schlüssel werden über das Menü Kostenstelle (Stammdaten > Kostenstamm) vergeben.
*Technische Info: `<F9>`, DB-Feld: abteilung.kostenst*

**Meldungsempfänger**
Auswahl des Meldungsempfängers. Der System-Meldungsempfänger der Abteilung ist die Person oder die Personengruppe, die Meldungen anderer Mitarbeiter dieser Abteilung entgegennimmt.
*Technische Info: `<F9>`, DB-Feld: abteilung.manr*

**Formulargruppe**
Ein Eintrag der Formulargruppe, die diese Abteilung benutzt, wird beim Formulardruck berücksichtigt. In der Regel wird pro Abteilung eine Formulargruppe hinterlegt.
*Technische Info: Numerisches Feld, DB-Feld: abteilung.formgrp*

**Fax**
Existiert ein eigener Faxanschluss, kann diese Nummer hier hinterlegt werden.
*Technische Info: Numerisches Feld, abteilung.faxnr*

**Letzte Änderung**
Hier wird der Mitarbeiter angezeigt, der die Daten zuletzt geändert hat sowie das entsprechende Datum.

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

## Marktpartnerschlüssel
*Stammdaten > Schlüssel > Marktpartner*

In diesem Bereich werden Merkmale zur Beschreibung der Marktpartner (Kunden, Lieferanten, etc.) angelegt. Sie stehen dann bei der Erfassung der Marktpartner zur Verfügung. Die einzelnen Merkmale werden nachfolgend erläutert.

Sie haben Zugriff auf folgende Bereiche:

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a a/b | Anreden | ⇨ "Anreden-Bezeichnungen" auf Seite B-104 |
| b | Bonus | ⇨"Bonus" auf Seite B-105 |
| c a | Gruppen | ⇨ "Gruppen" auf Seite B-107 |
| c b/c | Gruppenbezeichnungen | ⇨ "Gruppenbezeichnungen" auf Seite B-108 |
| d a/b | Branchen | ⇨ "Branchenbezeichnungen" auf Seite B-109 |
| e | Etikettentexte | ⇨ "Etikettentexte" auf Seite B-110 |
| f a | Kalender | ⇨ "Kalender" auf Seite B-111 |
| f b | Spez. Kalender | ⇨ "Spezielle Kalender" auf Seite B-113 |
| f c | Kundenkalender | ⇨ "Kundenkalender" auf Seite B-115 |
| f d | Mandantenkalender | ⇨ "Mandantenkalender" auf Seite B-117 |
| g | FIBU-Mandanten | ⇨ "FIBU-Mandanten" auf Seite B-119 |
| h a | Länder | ⇨ "Länder" auf Seite B-120 |
| h b/c | Länderbezeichnungen | ⇨ "Länder" auf Seite B-120 |
| i a/b | Wirtschaftsräume | ⇨ "Wirtschaftsraumbezeichnungen" auf Seite B-122 |
| j a/b | Region/Bundesländer | ⇨ "Regionen / Bundesländerbezeichnungen" auf Seite B-123 |
| k a | Qualitätsskala | ⇨ "Allgemeine Qualitätsskala" auf Seite B-124 |
| k b | Qual.-Skala Termine | ⇨ "Termin-Qualitätsskala" auf Seite B-126 |
| k c | Qual.-Skala Preise | ⇨"Preise-Qualitätsskala" auf Seite B-128 |
| k d | Qual.-Skala Mengen | ⇨ "Mengen-Qualitätsskala" auf Seite B-130 |
| k e | Qual.-Skala Spezial | ⇨ "Spezial-Qualitätsskala" auf Seite B-132 |
| i a | Reklamationsgründe | ⇨ “Reklamationsgründe" auf Seite B-134 |
| i b | Reklamationsorte | ⇨ "Reklamationsorte" auf Seite B-136 |
| i c | Reklamationstypen | ⇨ "Reklamationstypen" auf Seite B-138 |
| m a | Rabattmethoden | ⇨ "Rabattmethoden" auf Seite B-140 |
| m a | Rabatte | ⇨ "Rabatte" auf Seite B-144<br>⇨ "Rabatte - Details" auf Seite B-146 |
| n | Hausspezifische Angaben | ⇨ "Hausspezifische Marktpartner-Angaben" auf Seite B-151 |

> **Mehrsprachigkeit**
> Alle sprachabhängigen Schlüsseldaten werden in der Tabelle xsprbez gespeichert. Für den jeweiligen Dialog, z. B. Marktpartner > Anreden, wird dann zur Laufzeit eine View gebaut, die die Daten für die Anreden beinhaltet. Auf diese View kann man auch auf der Datenbankebene zugreifen. Daher haben wir in den Dialogen, die das betrifft, die Information über die View mit angegeben. In einigen Fällen existieren auch sprachunabhängige Daten. Diese werden über xx*-View geführt.

### Anreden-Bezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Anreden > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Anreden > Alle Bezeichnungen

Diese beiden Dialoge enthalten die Anredeformen, die bei der Erfassung von Marktpartnern vorkommen können, in den jeweiligen Sprachen.

#### Erläuterung der Felder
**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Anrede geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id, View: xanrede.anrkz*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Bezeichnung der Anrede, z. B. Firma.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1, View: xanrede.anrkz*

### Bonus
- Stammdaten > Schlüssel > Marktpartner > Bonus > Bonus
- Stammdaten > Schlüssel > Marktpartner > Bonus > Einzelne Bezeichnung
- Stammdaten > Schlüssel > Marktpartner > Bonus > Alle Bezeichnung

In diesem Dialog verfassen Sie die Regeln für die Bonität. Die Zuweisung eines Bonusverfahrens kann im Marktpartnerstamm oder während der Auftragserfassung erfolgen.

> **Mehrsprachige Bezeichnungen**
> Seit QR2209 können Sie in A+W Enterprise auch für Bonus mehrsprachige Bezeichnungen hinterlegen.

#### Erläuterung der Felder
**Bonus/Nr**
Auswahl eines Verfahrens. Über die Eingabe einer neuen Nummer wird ein neues Verfahren angelegt.
*Technische Info: `<F9>`, DB-Feld: xbonus.bonusnr*

**Bezeichnung**
Textuelle Erläuterung des Verfahrens.
*Technische Info: Alphanumerisches Feld, DB-Feld: xbonus.bonbez*

**Art**
Auswahl der Kriterien, nach denen der Bonus gewährt werden soll. Erstes Feld:
- **WE:** Der Bonus wird nach dem Auftragsvolumen in der Währungseinheit gewährt.
- **QM:** Der Bonus wird nach der abgenommenen Menge in Quadratmetern gewährt.
*Technische Info: `<F9>`, DB-Feld: xbonus.bonart*
Zweites Feld:
- **WE/qm:** Hier steuern Sie, ob sich der Bonus nach der Währungseinheit pro qm errechnet.
- **Max %-Satz:** Hier steuern Sie, ob es sich bei dem Bonus um einen maximalen Prozentwert handelt.
*Technische Info: `<F9>`, DB-Feld: xbonus.bontyp*
Im Feld dahinter geben Sie den entsprechenden Berechnungswert ein.
*Technische Info: Numerisches Feld, DB-Feld: xbonus.satz*

**Abrechnungszeitraum**
Hier wird die maximale Höhe des gewährten Bonus als Information festgehalten, z. B. 3 bedeutet, alle 3 Monate.
*Technische Info: Numerisches Feld, DB-Feld: xbonus.zeitraum*

**im Monat**
Hier legen Sie fest, wann genau die Prüfung erfolgen soll. In dem gewünschten Monat tragen Sie ein j ein. In den Feldern, die mit einem n gekennzeichnet sind, erfolgt keine Berechnung.
*Technische Info: Toggle-Feld, DB-Feld: xbonus.zp1-12*

**Bonusstaffel**
Im Anschluss an den allgemeinen Bereich folgt die Bonusstaffel. Die Spalte Bonus zeigt die Zuweisung zum Bonusschlüssel an. Für die Staffelung stehen mehrere Zeilen zur Verfügung, in den beschrieben wird, ab welchem Umsatz bzw. welcher Abnahmemenge welcher %-Satz gewährt wird.

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

### Gruppen
*Stammdaten > Schlüssel > Marktpartner > Gruppen > Gruppen*

Dieser Dialog zeigt die Marktpartner-Gruppen in der Mandantensprache. Die Gruppen können zu informativen Zwecken in Klassen eingeteilt werden. Die Klasse hat jedoch keine Auswirkung.
Das Löschen einzelner Gruppen ist nur in diesem Dialog möglich.
*Technische Info: Tabelle xxgrp*

**Ergänzende Informationen**
⇨ "Gruppenbezeichnungen" auf Seite B-108

### Gruppenbezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Gruppen > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Gruppen > Alle Bezeichnungen

Diese beiden Dialoge enthalten die Marktpartner-Gruppen, die bei der Erfassung von Marktpartnern vorkommen können, in den jeweiligen Sprachen.

#### Erläuterung der Felder
**Gruppe**
Schlüssel-Nummer. Zum Anlegen einer neuen Gruppe geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id, View: xgrp.grpnr*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Bezeichnung der Gruppe, z. B. ISO-Fertigung.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1, View: xgrp.atxt*

### Branchenbezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Branchen > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Branchen > Alle Bezeichnungen

Dieser Dialog enthält die Branchen, die bei der Erfassung von Marktpartnern vorkommen können, in den jeweiligen Sprachen. Über diese Branchen können alle speziellen Konditionen gepflegt werden.

#### Erläuterung der Felder
**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Branche geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id, View: xbranche.branchenr*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Bezeichnung der Branche, z. B. ISO-Hersteller.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1, View: xbranche.branche*

### Etikettentexte
*Stammdaten > Schlüssel > Marktpartner > Etikettentexte > Etikettentexte*

In diesem Dialog hinterlegen Sie kundenspezifische Etikettentexte.
Der Eintrag im Feld Produktname erscheint als kundenspezifische Zusatzinformation auf den Scheibenetiketten. Über das frei wählbare Kürzel wird der Langtext referenziert.

#### Erläuterung der Felder
**Nummer**
Zum Anlegen einer neuen Etikettentextnummer wählen Sie die nächst freie Nummer.
*Technische Info: Numerisches Feld, DB-Feld: xetikett.txtnr*

**Produktname**
In diesem Feld ordnen Sie den Kunden bzw. das Objekt zu.
*Technische Info: Alphanumerisches Feld, DB-Feld: xetikett.etitxt1*

**Kürzel**
Über das Kürzel wird der Langtext referenziert.
*Technische Info: Numerisches Feld, DB-Feld: xetikett.etitxt2*

**Text**
Dieser Text erscheint als kundenspezifische Zusatzinformation auf den Scheibenetiketten.
*Technische Info: Alphanumerisches Feld, DB-Feld: xetikett.etitxt3*

### Kalender
- Stammdaten > Schlüssel > Marktpartner > Kalender
- System-Menü (`<Strg>` + `<F4>`) > Infodienste > Kalender > Kalender

In diesem Dialog pflegen Sie Ihren Betriebskalender.
Wenn Sie mit dem Mehr-Mandantensystem (Multi-Site) arbeiten, handelt es sich dabei um den Kalender des Hauptmandanten. Abweichende Mandantenkalender pflegen Sie unter "Mandantenkalender" auf Seite B-117.
Es stehen Ihnen zwei unterschiedliche Ansichten (`<F2>`) zur Verfügung:
- Tagesansicht
- Monatsansicht

#### Erläuterung der Felder
**Datum**
Hier wird Ihnen jedes einzelne Datum angezeigt.

**Tag**
Hier wird Ihnen jeder einzelne Tag angezeigt.

**KW**
Hier wird Ihnen die Kalenderwoche angezeigt.

**H**
Auswahl, ob es sich bei dem Tag um einen Handelstag handelt.
*Technische Info: Toggle-Feld, DB-Feld: alkal.htag*

**P**
Auswahl, ob es sich bei dem Tag um einen Produktionstag handelt.
*Technische Info: Toggle-Feld, DB-Feld: alkal.ptag*

**H-MD**
Hier sehen Sie, ob es sich bei diesem Tag um einen mandantenspezifischen Handelstag handelt. Der Eintrag hier übersteuert den Eintrag im Feld H. Die mandantenspezifischen Handelstage werden in System > Schlüssel > Marktpartner > Kalender > Mandantenkalender gepflegt und können hier nicht geändert werden.

**P-MD**
Hier sehen Sie, ob es sich bei diesem Tag um einen mandantenspezifischen Produktionstag handelt. Der Eintrag hier übersteuert den Eintrag im Feld P. Die mandantenspezifischen Produktionstage werden in System > Schlüssel > Marktpartner > Kalender > Mandantenkalender gepflegt und können hier nicht geändert werden.

**Bemerkung**
In diesem Feld können Sie eine entsprechende Bemerkung hinterlegen.
*Technische Info: Alphanumerisches Feld, DB-Feld: alkal.bem*

> **Arbeiten mit A+W Production**
> Sollten Sie mit A+W Production arbeiten, kann das System so konfiguriert werden, dass dieser Kalender auch in der Produktion ausgewertet wird. Diese Konfiguration erfolgt in A+W Production.

### Spezielle Kalender
- Stammdaten > Schlüssel > Marktpartner > Kalender > Spez. Kalender > Spez. Kalender
- Stammdaten > Schlüssel > Marktpartner > Kalender > Spez. Kalender > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Kalender > Spez. Kalender > Alle Bezeichnungen
- System-Menü (`<Strg>` + `<F4>`) > Infodienste > Kalender > Spez. Kalender
- System-Menü (`<Strg>` + `<F4>`) > Infodienste > Kalender > Spez. Kalender > Einzelne Bezeichnungen
- System-Menü (`<Strg>` + `<F4>`) > Infodienste > Kalender > Spez. Kalender > Alle Bezeichnungen

In diesem Kalender können Sie z. B. Daten für Ereignisse hinterlegen.

#### Erläuterung der Felder
**Kalender**
Auswahl der Kalendernummer.
*Technische Info: `<F9>`, DB-Feld: almpkal.kalnr*

**Datum**
Hier geben Sie das Datum ein.
*Technische Info: Numerisches Feld, DB-Feld: almpkal.datum*

**Tag**
Wenn Sie das Feld Datum verlassen, wird der Tag automatisch eingeblendet.

**KW**
Wenn Sie das Feld Datum verlassen, wird die Kalenderwoche automatisch eingeblendet.

**BHT**
Hier sehen Sie, ob es sich um einen Betriebshandelstag handelt oder nicht.

**H**
Über dieses Feld können Sie Tage, an denen normalerweise nicht gearbeitet wird (z. B. Sonntage) als Handelstage definieren.
*Technische Info: Toggle-Feld, DB-Feld: almpkal.htag*

**Bemerkung**
In diesem Feld können Sie eine entsprechende Bemerkung hinterlegen.
*Technische Info: Alphanumerisches Feld, DB-Feld: almpkal.bem*

**Kalender/Nr**
Schlüssel-Nummer. Zum Anlegen eines neuen Kalenders geben Sie die nächste freie Nummer ein.
*Technische Info: Numerisches Feld, DB-Feld: xsprbez.id, View: xkalender.kalnr*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Bezeichnung des Kalenders, z. B. Lieferanten.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1, View: xkalender.atxt*

### Kundenkalender
- Stammdaten > Schlüssel > Marktpartner > Kalender > Kundenkalender
- System-Menü (`<Strg>` + `<F4>`) > Infodienste > Kalender > Kundenkalender

Für Marktpartner vom Typ Kunde und Sonstige können im Kundenkalender eigene Daten hinterlegt werden. D. h. es können Marktpartner-spezifisch Handels-, Produktions- und Feiertage hinterlegt werden.

#### Erläuterung der Felder
**Partnertyp**
Auswahl des Partnertyps.
*Technische Info: `<F9>`, DB-Feld: almpkal.kuliflag*

**Marktpartner**
Auswahl der Marktpartnernummer.
*Technische Info: `<F9>`, DB-Feld: almpkal.mpnr*

**Datum**
Hier geben Sie das Datum ein.
*Technische Info: Numerisches Feld, DB-Feld: almpkal.datum*

**Tag**
Wenn Sie das Feld Datum verlassen, wird der Tag automatisch eingeblendet.

**KW**
Wenn Sie das Feld Datum verlassen, wird die Kalenderwoche automatisch eingeblendet.

**BHT**
Hier sehen Sie, ob es sich um einen Betriebshandelstag handelt oder nicht.

**H**
Über dieses Feld können Sie Tage, an denen normalerweise nicht gearbeitet wird (z. B. Sonntage) als Handelstage definieren.
*Technische Info: Toggle-Feld, DB-Feld: almpkal.htag*

**Bemerkung**
In diesem Feld können Sie eine entsprechende Bemerkung hinterlegen.
*Technische Info: Alphanumerisches Feld, DB-Feld: almpkal.bem*

### Mandantenkalender
- Stammdaten > Schlüssel > Marktpartner > Kalender > Mandantenkalender
- System-Menü (`<Strg>` + `<F4>`) > Infodienste > Kalender > Mandantenkalender

Nachdem Sie die Mandantennummer ausgewählt haben, öffnet sich der Kalender.
Diese Kalenderfunktion wird für das Mehr-Mandantensystem (Multi-Site) verwendet. Hier können Sie für jeden internen Mandanten im Betriebskalender eigene Daten hinterlegen. So können Sie mandantenspezifische Handels-, Produktions- und Feiertage hinterlegen.

Es stehen Ihnen zwei unterschiedliche Ansichten zur Verfügung:
- Tagesansicht
- Monatsansicht

#### Erläuterung der Felder
**Datum**
Hier wird Ihnen jedes einzelne Datum angezeigt.

**Tag**
Hier wird Ihnen jeder einzelne Tag angezeigt.

**KW**
Hier wird Ihnen die Kalenderwoche angezeigt.

**H**
Hier sehen Sie, ob dieser Tag bei dem Hauptmandanten ein Handelstag ist oder nicht. Die hauptmandantenspezifischen Handelstage werden in System > Schlüssel > Marktpartner > Kalender > Kalender gepflegt und können hier nicht geändert werden.

**P**
Hier sehen Sie, ob dieser Tag bei dem Hauptmandanten ein Produktionstag ist oder nicht. Die hauptmandantenspezifischen Produktionstage werden in System > Schlüssel > Marktpartner > Kalender > Kalender gepflegt und können hier nicht geändert werden

**H-MD**
Auswahl, ob es sich bei dem Tag um einen Handelstag handelt.
*Technische Info: Toggle-Feld, DB-Feld: alkal.htag*

**P-MD**
Auswahl, ob es sich bei dem Tag um einen Produktionstag handelt.
*Technische Info: Toggle-Feld, DB-Feld: alkal.ptag*

**Bemerkung**
In diesem Feld können Sie eine entsprechende Bemerkung hinterlegen.
*Technische Info: Alphanumerisches Feld, DB-Feld: alkal.bem*

**Ergänzende Informationen**
"Kalender" auf Seite B-111

### FIBU-Mandanten
*Stammdaten > Schlüssel > Marktpartner > FIBU-Mandanten*

In diesem Dialog legen Sie die FIBU-Mandanten fest. Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

### Länder
- Stammdaten > Schlüssel > Marktpartner > Länder > Länder
- Stammdaten > Schlüssel > Marktpartner > Länder > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Länder > Alle Bezeichnungen

Dieser Dialog enthält die unterschiedlichen Länder, die bei der Erfassung von Marktpartnern vorkommen können, in den jeweiligen Sprachen.

#### Erläuterung der Felder
**KFZ Code/KFZ**
KFZ-Codes, z. B. A (Österreich). Zum Anlegen eines neuen Landes geben Sie den entsprechenden Code ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.cid, View: xland.kfz*

**ISO**
Ländercode nach ISO-Norm, z. B. AT (Österreich).
*Technische Info: Alphanumerisches Feld, DB-Feld: xxland.iso*

**Landesbezeichnung**
Bezeichnung des Landes, z. B. Belgien.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1, View: xland.atxt*

**Fibu**
Dieses Feld enthält den entsprechenden Ländercode der Finanzbuchhaltung.
*Technische Info: Alphanumerisches Feld, DB-Feld: xxland.fib*

**Intracode**
Dieses Feld enthält die entsprechende Vorgabe des Statistischen Bundesamtes für die Intrahandelsstatistik.
*Technische Info: Alphanumerisches Feld, DB-Feld: xxland.intracode*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

### Wirtschaftsraumbezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Wirtschaftsräume > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Wirtschaftsräume > Alle Bezeichnungen

Die freie Aufteilung des Landes in Wirtschaftsräume gewährt die spätere Zuordnung von Marktpartnern zu einem Wirtschaftsraum, unabhängig vom Bundesland.
Dieser Dialog enthält die unterschiedlichen Wirtschaftsräume, die bei der Erfassung von Marktpartnern vorkommen können, in den jeweiligen Sprachen.

#### Erläuterung der Felder
**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen eines neuen Wirtschaftsraumes geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id, View: xwrtraum.wrtnr*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Bezeichnung des Wirtschaftsraumes, z. B. Mitte.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1, View: xwrtraum.wrtraum*

### Regionen / Bundesländerbezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Region/Bundesländer > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Region/Bundesländer > Alle Bezeichnungen

Die hier erfassten Bundesländer können im Marktpartnerstamm den Kunden und Lieferanten zugeordnet werden. Die Vergabe der Schlüssel-Nr. sollte für die Intrahandelsstatistik gemäß der entsprechenden Vorgabe des statistischen Bundesamtes erfolgen.
Dieser Dialog enthält die unterschiedlichen Regionen und Bundesländer, in den jeweiligen Sprachen.

#### Erläuterung der Felder
**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Region geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id, View: xregion.regnr*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Region/Bundesland**
Bezeichnung der Region, z. B. Mitte.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1, View: xregion.region*

### Allgemeine Qualitätsskala
- Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Allgemein > Qualitätsskala
- Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Allgemein > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Allgemein > Alle Bezeichnungen

In diesen Dialogen legen Sie die allgemeinen Qualitäts-Merkmale mit Prioritäten und in verschiedenen Sprachen an. Diese Schlüssel dienen der Beurteilung des Marktpartners und werden für alle Bewertungskriterien eingesetzt.

#### Erläuterung der Felder
**Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Qualität geben Sie die nächste freie Nummer ein.
*Technische Info: Numerisches Feld, DB-Feld: xxqual.qualkz*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Bezeichnung, z. B. sehr gute Qualität
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1*

**Rang**
Der Rang, den die Bewertung innerhalb der Bewertungsskala einnimmt.
*Technische Info: Alphanumerisches Feld, DB-Feld: xxqual.rang*

### Termin-Qualitätsskala
- Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Termine > Qual.-Skala Termine
- Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Termine > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Termine > Alle Bezeichnungen

Zur Bewertung der Lieferanten bezüglich der Einhaltung von Terminen werden freie Bezeichnungen angelegt und mit einem Rang skaliert.
Der Dialog zeigt Ihnen die angelegten Schlüssel, die zur manuellen Bewertung der Lieferanten im Marktpartnerstamm zur Verfügung stehen.

#### Erläuterung der Felder
**Nr**
Schlüsselnummer. Zum Anlegen einer neuen Schlüsselnummer geben Sie die nächste freie Nummer ein.
*Technische Info: Numerisches Feld, DB-Feld: xsprbez.id, View: xtermin.terminkz*

**Spr**
Sprachkennzeichens.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Schlüsselbezeichnung, z. B. Termingerecht.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1, View: xtermin.atxt*

**Rang**
Der Rang, den die Bewertung innerhalb der Bewertungsskala einnimmt.
*Technische Info: Alphanumerisches Feld, DB-Feld: xxtermin.rang*

### Preise-Qualitätsskala
- Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Preise > Qual.-Skala Preise
- Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Preise > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Preise > Alle Bezeichnungen

Zur Bewertung der Lieferanten bezüglich der Preise können ebenfalls freie Bezeichnungen angelegt und mit einem Rang skaliert werden.
Der Dialog zeigt Ihnen die angelegten Schlüssel, die zur manuellen Bewertung der Lieferanten im Marktpartnerstamm zur Verfügung stehen.

#### Erläuterung der Felder
**Nr**
Schlüsselnummer. Zum Anlegen einer neuen Schlüsselnummer geben Sie die nächste freie Nummer ein.
*Technische Info: Numerisches Feld, DB-Feld: xsprbez.id, View: xpreis.preiskz*

**Spr**
Sprachkennzeichens.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Schlüsselbezeichnung, z. B. Preiswert.
*Technische Info: Alphanumerisches Feld, DB-Feld: xxpreis.atxt*

**Rang**
Der Rang, den die Bewertung innerhalb der Bewertungsskala einnimmt.
*Technische Info: Alphanumerisches Feld, DB-Feld: xxpreis.rang, View: xpreis.atxt*

### Mengen-Qualitätsskala
- Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Mengen > Qual.-Skala Mengen
- Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Mengen > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Mengen > Alle Bezeichnungen

Zur Bewertung der Liefermengen einzelner Lieferanten werden freie Bezeichnungen angelegt und mit einem Rang skaliert.
Der Dialog zeigt Ihnen die angelegten Schlüssel, die zur Verfügung stehen.

#### Erläuterung der Felder
**Nr**
Schlüsselnummer. Zum Anlegen einer neuen Schlüsselnummer geben Sie die nächste freie Nummer ein.
*Technische Info: Numerisches Feld, DB-Feld: xsprbez.id, View: xmenge.mengekz*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Schlüsselbezeichnung, z. B. Guter Lagerbestand.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1, View: xmenge.atxt*

**Rang**
Der Rang, den die Bewertung innerhalb der Bewertungsskala einnimmt.
*Technische Info: Alphanumerisches Feld, DB-Feld: xxmenge.rang*

### Spezial-Qualitätsskala
- Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Spezial > Qual.-Skala Spezial
- Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Spezial > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Qualitätsskala > Spezial > Alle Bezeichnungen

Die Qualitätsskala Spezial bietet eine zusätzliche individuelle Möglichkeit, Lieferanten anhand von frei definierbaren Bezeichnungen, denen ein Rang zugeordnet ist, zu beurteilen.
Der Dialog zeigt Ihnen die angelegten Schlüssel, die zur Verfügung stehen.

#### Erläuterung der Felder
**Nummer**
Schlüssel-Nummer. Zum Anlegen eines neuen Mengenniveaus geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id, View: xspec.speckz*

**Rang**
Der Rang, den die Bewertung innerhalb der Bewertungsskala einnimmt.
*Technische Info: Alphanumerisches Feld, DB-Feld: xxspec.rang*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Bezeichnung des Mengenniveaus, z. B. Guter Lagerbestand.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1, View: xspec.atxt*

### Reklamationsgründe
- Stammdaten > Schlüssel > Marktpartner > Reklamation > Gründe > Reklamationsgründe
- Stammdaten > Schlüssel > Marktpartner > Reklamation > Gründe > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Reklamation > Gründe > Alle Bezeichnungen

Hier werden die Reklamationsarten textuell hinterlegt und mit einem frei wählbaren Schlüssel versehen. Sie werden für die Erfassung und Auswertung von Reklamationen benötigt.
Darüber hinaus werden in dieser Tabelle die Codes der Geschäftsart für die Intrahandelsstatistik gepflegt.

#### Erläuterung der Felder
**Nr**
Schlüsselnummer. Zum Anlegen einer neuen Schlüsselnummer geben Sie die nächste freie Nummer ein.
*Technische Info: Numerisches Feld, DB-Feld: xxrart.reklamart*

**Reklamationsgrund**
Schlüsselbezeichnung, z. B. Verpackung kaputt.
*Technische Info: Alphanumerisches Feld, DB-Feld: xxrart.bez*

**Intrastat**
Der Code gemäß den Vorgaben des Statistischen Bundesamtes.
*Technische Info: Alphanumerisches Feld, DB-Feld: xxrart.intrageschart*

**Ohne Überschriften**
Die beiden Spalten ohne Überschriften können Sie individuell über Umgebungsvariablen definieren.
*Technische Info: Alphanumerisches Feld, DB-Feld: xxrart.private_long1/2*

**S**
Stilllegungskennzeichen.
*Technische Info: `<Toggle>-Feld, DB-Feld: xxrart.lustill*

**Nummer**
Auswahl der Schlüssel-Nummer Zum Anlegen einer neuen Schlüsselnummer geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id, View: rart.reklamart*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Reklamationsgrund**
Bezeichnung des Reklamationsgrundes, z. B. Verpackung kaputt.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1, View: rart.atxt*

### Reklamationsorte
- Stammdaten > Schlüssel > Marktpartner > Reklamation > Orte > Reklamationsorte
- Stammdaten > Schlüssel > Marktpartner > Reklamation > Orte > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Reklamation > Orte > Einzelne Bezeichnungen

Die textuellen Vorgaben für den Reklamationsort können frei definiert werden. Sie sind für die Reklamationsbearbeitung und -statistik von Bedeutung.

#### Erläuterung der Felder
**Nummer**
Schlüssel-Nummer Zum Anlegen eines neuen Ortes geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id, View: rort.reklamort*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Reklamationsgrund**
Schlüsselbezeichnung, z. B. Produktion.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1, View: rort.atxt*

**S**
Stilllegungskennzeichen.
*Technische Info: `<Toggle>-Feld, DB-Feld: xxrart.still*

### Reklamationstypen
- Stammdaten > Schlüssel > Marktpartner > Reklamation > Typen > Reklamationstypen
- Stammdaten > Schlüssel > Marktpartner > Reklamation > Typen > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > Marktpartner > Reklamation > Typen > Alle Bezeichnungen

In diesen Dialogen werden die Reklamationstypen textuell hinterlegt und mit einem frei wählbaren Schlüssel versehen. Sie werden für die Erfassung und Auswertung von Reklamationen benötigt.

#### Erläuterung der Felder
**Nr/Nummer**
Typnummer. Im Feld dahinter geben Sie die Bezeichnung ein. Zum Anlegen einer neuen Schlüsselnummer geben Sie die nächste freie Nummer ein.
*Technische Info: Numerisches Feld, DB-Feld: xsprbez.id, View: xxrspec.reklamspec*

**Bezeichnung/Reklamationstyp**
Bezeichnung des Typs, z. B. Bruch.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1, View: xspec.atxt*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Ohne Überschriften**
Die beiden Spalten ohne Überschriften können Sie individuell über Umgebungsvariablen definieren.
*Technische Info: Alphanumerisches Feld, DB-Feld: xxrspec.private_long1/2*

**S**
Stilllegungskennzeichen.
*Technische Info: `<Toggle>-Feld, DB-Feld: xxrspec.still*

### Rabattmethoden
- Stammdaten > Schlüssel > Marktpartner > Vorgangsrabatte > Rabattmethoden > Rabattmethoden
- Stammdaten > Schlüssel > Marktpartner > Vorgangsrabatte > Rabattmethoden > Einzelne Bezeichnung
- Stammdaten > Schlüssel > Marktpartner > Vorgangsrabatte > Rabattmethoden > Alle Bezeichnung

Dieser Dialog dient zur Bestimmung gültiger Rabattmethoden, die mit unterschiedlichen Merkmalen beschrieben werden und anschließend als Vorgangs- bzw. Marktpartnerspezifische Rabatte definiert werden. In der Rabattmethode werden Informationen hinterlegt, die für die komplette Methode gültig sind.

> **Mehrsprachige Bezeichnungen**
> Seit QR2209 können Sie in A+W Enterprise auch für Rabattmethoden mehrsprachige Bezeichnungen hinterlegen.

#### Erläuterung der Felder
**Methode**
Methodennummer. Zum Anlegen einer neuen Methode wählen Sie die nächst freie Nummer.
*Technische Info: Numerisches Feld, DB-Feld: rabattmeth.methode*

**Name**
Bezeichnung der Rabattmethode, z. B. Energiezuschlag.
*Technische Info: Alphanumerisches Feld, DB-Feld: rabattmeth.methodenname*

**Sequenz**
Steuert bei mehreren gleichzeitigen Rabatten die Reihenfolge, in der die Rabatte zur Anwendung kommen.
*Technische Info: Numerisches Feld, DB-Feld: rabattmeth.seqnr*

**Kriterium**
In diesem Feld legen Sie fest, welches Vorgangskriterium erfüllt sein muss, damit der Rabatt dieser Methode wirkt:
- **0:** Keine Abhängigkeit
- **1:** Eilauftrag
- **2:** Route
- **3:** Versandart
- **4:** Verpackungsart
- **5:** Lieferart
- **6:** Zielland.
*Technische Info: Numerisches Feld, DB-Feld: rabattmeth.qualfier*

**Gutschr.**
Mit diesem Feld steuern Sie, wie der Rabatt bei Gutschriften behandelt wird:
- **Ja:** Der Rabatt wird automatisch in die Gutschriften übernommen.
- **Nein:** Der Rabatt wird nicht in die Gutschrift übernommen.
- **Frage:** Sie werden gefragt, ob der Rabatt in die Gutschrift übernommen werden soll.
*Technische Info: Toggle-Feld, DB-Feld: rabattmeth.gutschrift*

**Gewicht**
Mit diesem Feld steuern Sie, wie der Rabatt bei Gutschriften behandelt wird:
- **Nur fak. GGew:** Der Rabatt bezieht sich nur auf das fakturierte Glasgewicht.
- **Fak. Glasgew.:** Der Rabatt bezieht sich auf das fakturierte Glasgewicht.
- **Posgew.:** Der Rabatt bezieht sich auf das Positionsgewicht.
- **Nur Glasgew.:** Der Rabatt bezieht sich nur auf das Positionsgewicht.
- **Glasgew.:** Der Rabatt bezieht sich auf das Glasgewicht. Falls dieses aber Null ist, wird Positionsgewicht verwendet.
- **Fak.Posgew.:** Der Rabatt bezieht sich auf das fakturierte Positionsgewicht.
*Technische Info: Toggle-Feld, DB-Feld: rabattmeth.glasgewicht*

**Lz.**
Mit dieser Checkbox können Sie eine Rabattmethode so kennzeichnen, dass Rabatte dieser Methode bei der Lieferscheinerzeugung deaktiviert werden, wenn es schon einen Lieferschein innerhalb dieser Lieferung gibt.
*Technische Info: Toggle-Feld, DB-Feld: rabattmeth.lieferzuschlag*

**Rab.**
Mit diesem Feld steuern Sie, ob spätere Rabatte auf den Rabatt dieses Rabattes wirken:
- **Ja:** Der Betrag dieses Rabattes wird in den Grundbetrag nachfolgender Rabatte mit eingerechnet.
- **Nein:** Der Betrag bleibt unberücksichtigt.
*Technische Info: Toggle-Feld, DB-Feld: rabattmeth.rabattierbar*

**Nul.**
Mit diesem Feld steuern Sie, ob bei Mengenberechnungen Positionen mit einem Betrag von Null berücksichtigt werden:
- **Ja:** Positionen mit Betrag Null werden berücksichtigt.
- **Nein:** Positionen werden nicht berücksichtigt.
*Technische Info: Toggle-Feld, DB-Feld: rabattmeth.nullpositionen*

**All**
Mit diesem Feld steuern Sie, ob diese Rabattmethode auf allgemeiner Ebene gepflegt werden kann.
- **Ja:** Diese Methode kann auf allgemeiner Ebene gepflegt werden.
- **Nein:** Diese Methode kann nicht auf allgemeiner Ebene gepflegt werden.
*Technische Info: Toggle-Feld, DB-Feld: rabattmeth.allgemein*

**Mp.**
Mit diesem Feld steuern Sie, ob diese Rabattmethode auf Marktpartner-Ebene gepflegt werden kann.
- **Ja:** Diese Methode kann auf Marktpartner-Ebene gepflegt werden.
- **Nein:** Diese Methode kann nicht auf Marktpartner-Ebene gepflegt werden.
*Technische Info: Toggle-Feld, DB-Feld: rabattmeth.marktpartner*

**Obj.**
Mit diesem Feld steuern Sie, ob diese Rabattmethode auf Objekt-Ebene gepflegt werden kann.
- **Ja:** Diese Methode kann auf Objekt-Ebene gepflegt werden.
- **Nein:** Diese Methode kann nicht auf Objekt-Ebene gepflegt werden.
*Technische Info: Toggle-Feld, DB-Feld: rabattmeth.objekt*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

### Rabatte
*Stammdaten > Schlüssel > Marktpartner > Vorgangsrabatte > Rabatte*

In den Rabattmethoden werden Informationen hinterlegt, die für die komplette Methode Gültigkeit haben. Diese Rabatte sind nicht als konkrete Rabatte zu verstehen, sondern vielmehr als eine bestimmte Gruppierung von Rabatten, z. B. Energiezuschlag oder Eilzuschlag. Im folgenden wird sprachlich nicht zwischen den Begriffen Zuschlag und Rabatt unterschieden. Es wird der im jeweiligen Zusammenhang verständlichere Begriff verwendet. Die konkreten Rabatte, die allgemein gültig oder marktpartnerabhängig sind, definieren Sie hier:
⇨ "Rabatte" auf Seite B-66

Der Dialog besteht aus den Registern:
- Allgemein
- Details

#### Erläuterung der Felder
**Methode**
Auswahl der Rabattmethode. Die entsprechenden Schlüssel werden über das Menü Rabattmethoden (Schlüssel > Marktpartner > Vorgangsrabatte) vergeben.
*Technische Info: `<F9>`, DB-Feld: rabstamm.methode*

**Name**
Name der Rabattmethode. Dieser Eintrag kann hier überschrieben werden.
*Technische Info: Alphanumerisches Feld, DB-Feld: rabstamm.rabatttext*

**Kriterium**
Hier wird das für die Methode hinterlegte Kriterium angezeigt.
*Technische Info: `<F9>`, DB-Feld: rabstamm.qualifierwert*

**Typ**
Typ der Rabattmethode:
- **Verkauf:** Verkaufsseitiger Rabatt.
- **Kosten:** Kostenseitiger Rabatt.
- **Einkauf:** Einkaufsseitiger Rabatt (nur im Menü Einkauf).
*Technische Info: Toggle-Feld, DB-Feld: rabstamm.ekvkkz*

**Wagrp.**
Warengruppe der Rabattmethode. Die Rabattmethode wirkt nur auf die Produkte dieser Warengruppe im Auftrag.
*Technische Info: `<F9>`, DB-Feld: rabstamm.wgrnr*

**Wert**
Der angegebene Wert wird je nach Rabattart unterschiedlich interpretiert und wird zur Berechnung des Rabattbetrags verwendet.
*Technische Info: Numerisches Feld, DB-Feld: rabstamm.wert*

**Satzart (Spalte ohne Bezeichnung)**
Der angegebene Wert wird je nach Rabattart unterschiedlich interpretiert und wird zur Berechnung des Rabattbetrags verwendet. Mögliche Werte sind:
- **+:** Zuschlag
- **-:** Rabatt
*Technische Info: Numerisches Feld, DB-Feld: rabstamm.satzart*

**Rab.Art**
Über die Rabattart wird angegeben, wie der Rabattbetrag berechnet werden soll:
- **WE:** Fixer Wert
- **%:** Prozentualer Wert
- **WE/Stk.:** Wert pro Stück
- **WE/qm:** Wert pro Quadratmeter Glas
- **WE/kg:** Wert pro Kilogramm Glas
- **%VK:** Kostenrabatt auf Basis des Verlaufsbetrags. Dieser Rabatt wird wie %-Kostenrabatt mit dem Basiswert des Verkaufsbetrages berechnet
- **WE/G*E:** Wert pro Gewicht in kg multipliziert mit der Entfernung in km. Dieser Rabatt wird nur dann angewendet, wenn die Entfernung in den Adressen oder im Marktpartner hinterlegt wurde.
*Technische Info: Numerisches Feld, DB-Feld: rabstamm.rabattart*

**Pos.**
Über diese Checkbox steuern Sie, ob der eingegebene Rabatt auf die einzelnen Positionen rückverteilt wird oder nicht.
- `☑` Der Rabatt wird auf die einzelnen Positionen rückverteilt.
- `☐` Der Rabatt wird nicht rückverteilt.
*Technische Info: Toggle-Feld, DB-Feld: rabstamm.verteil*

### Rabatte - Details
*Stammdaten > Schlüssel > Marktpartner > Vorgangsrabatte > Rabatte > Details `<F2>`*

#### Erläuterung der Felder
**Methode**
Auswahl der Rabattmethode. Die entsprechenden Schlüssel werden über das Menü Rabattmethoden (Schlüssel > Marktpartner > Vorgangsrabatte) vergeben.
*Technische Info: `<F9>`, DB-Feld: rabstamm.methode*

**Name**
Name der Rabattmethode. Dieser Eintrag kann überschrieben werden.
*Technische Info: Alphanumerisches Feld, DB-Feld: rabstamm.rabatttext*

**Kriterium**
Hier wird das für die Methode hinterlegte Kriterium angezeigt.
*Technische Info: `<F9>`, DB-Feld: rabstamm.qualifierwert*

**Typ**
Typ der Rabattmethode:
- **Verkauf:** Verkaufsseitiger Rabatt.
- **Kosten:** Kostenseitiger Rabatt.
- **Einkauf:** Einkaufsseitiger Rabatt (nur im Menü Einkauf).
*Technische Info: Toggle-Feld, DB-Feld: rabstamm.ekvkkz*

**Wagrp.**
Warengruppe der Rabattmethode. Die Rabattmethode wirkt nur auf die Produkte dieser Warengruppe im Auftrag.
*Technische Info: `<F9>`, DB-Feld: rabstamm.wgrnr*

**Rabattwert**
Der angegebene Wert wird - je nach Rabattart - unterschiedlich interpretiert und wird zur Berechnung des Rabattbetrages verwendet.
*Technische Info: Numerisches Feld, DB-Feld: rabstamm.wert*

**Staffelbasis**
Auswahl der Staffelbasis. Falls Sie eine Staffelbasis angeben, müssen Sie anschließend über `<F5>` die Staffelstufen festlegen:
- qm - Quadratmeter Glas
- kg - Kilogramm Glas
- km - Kilometer
- St - Stück
- WE - Wert
*Technische Info: `<F9>`, DB-Feld: rabstamm.staffelbasis*

**Minimalwert**
Minimale Rabattsumme.
*Technische Info: Numerisches Feld, DB-Feld: rabstamm.minbetrag*

**Maximalwert**
Maximale Rabattsumme.
*Technische Info: Numerisches Feld, DB-Feld: rabstamm.maxbetrag*

**Rückverteilen**
Rückverteilung des Rabatts auf die Positionen. Durch die Rückverteilung werden die Rabatte auf die jeweilige Position verteilt und vom Programm automatisch an die FIBU übermittelt. Wird keine Rückverteilung verwendet, dann müssen Sie die Rabatte manuell an die FIBU übergeben. Dafür müssen Sie die Angaben aus dem Feld Stat. Warengruppe und Kostenstelle an die FIBU übermitteln.
- `☑` Der Rabatt wird auf die einzelnen Positionen rückverteilt.
- `☐` Der Rabatt wird nicht rückverteilt.
*Technische Info: Toggle-Feld, DB-Feld: rabstamm.verteil*

**Stat. Warengruppe**
Dieses Feld ist nur aktiv, wenn der aktuelle Satz nicht als rückverteilt gekennzeichnet ist. Dann muss hier eine statistische Warengruppe für Statistik-Buchungen angegeben werden.
*Technische Info: `<F9>`, DB-Feld: rabstamm.statwgrnr*

**Kostenstelle**
Dieses Feld ist nur aktiv, wenn der aktuelle Satz nicht als rückverteilt gekennzeichnet ist. Dann muss hier eine Kostenstelle angegeben werden, auf die gebucht werden soll.
*Technische Info: `<F9>`, DB-Feld: rabstamm.kstelle*

**Konto**
Dieses Feld ist nur aktiv, wenn der aktuelle Satz nicht als rückverteilt gekennzeichnet ist. Dann muss hier das Konto angegeben werden, auf das gebucht werden soll.
*Technische Info: `<F9>`, DB-Feld: rabstamm.konto*

**Rabatt gültig von**
Datum, ab dem der Rabatt verwendet werden soll.
*Technische Info: Numerisches Feld, DB-Feld: rabstamm.gueltigvon*

**Rabatt gültig bis**
Datum, bis zu dem der Rabatt verwendet werden soll. Bei entsprechender Systemkonfiguration können Sie bei der Auftragserfassung die Gültigkeits-Prüfung aktivieren. Die Konfiguration lässt folgende Möglichkeiten zu:
- Es wird geprüft, ob Rabatte in den letzten X Tagen abgelaufen sind (die Anzahl der Tage ist ebenfalls konfigurierbar)
- Es wird geprüft, ob die Rabatte in der Vergangenheit abgelaufen sind und zusätzlich wird eine Meldung ausgegeben, ob auch Rabatte vorhanden sind, die heute ablaufen.
- Es wird nur gemeldet, wenn es Rabatte ermittelt werden, die heute ablaufen.
*Technische Info: Numerisches Feld, DB-Feld: rabstamm.gueltigbis*

**Teilvorgang**
Bei Rabatten vom Typ WE muss entschieden werden, wie das Programm bei der Erzeugung von Teillieferscheinen bzw. Teilrechnungen vorgeht. Der Rabatt wird entweder in den ersten Teilvorgang übernommen, in alle Teilvorgänge übernommen oder in einen prozentualen Rabatt umgewandelt. Mögliche Werte sind:
- **in 1. Tv:** Rabatt wird in den ersten Teilvorgang übernommen.
- **in alle Tv:** Rabatt wird in alle Teilvorgänge übernommen.
- **prozentual:** Es erfolgt die Umwandlung in einen prozentualen Rabatt.
*Technische Info: Numerisches Feld, DB-Feld: rabstamm.fixerabatte*

**Mehrwertsteuer**
Auswahl des Mehrwertsteuersatzes. Dieses Feld ist nur aktiv, wenn der aktuelle Satz nicht als rückverteilt gekennzeichnet ist. Die Zuordnung zu den Mehrwertsteuersätzen wirkt sich nur dann aus, wenn die Logik für mehrere Mehrwertsteuern im System aktiviert ist.
*Technische Info: `<F9>`, DB-Feld: rabstamm.steuerzu*

**Skontierbar**
Die Checkbox ist nur aktiv, wenn Rabatte nicht rückverteilt sind. Das Flag wirkt sich auf Rabatte vom Typ Kosten nicht aus.
- `☑` Der Rabatt ist skontofähig.
- `☐` Der Rabatt ist nicht skontofähig.
*Technische Info: Toggle-Feld, DB-Feld: rabstamm.skonto*

**openTRANS - Id**
Dieses Feld ermöglicht die Zuordnung von Rabatten aus Einkaufsvorgängen, die via OpenTRANS empfangen wurden.
*Technische Info: Numerisches Feld, DB-Feld: rabstamm.otrabattid*

**Verglasung**
Das Verglasungskennzeichen wird nur bei prozentualen Rabatten ausgewertet. Dort wird dann als Grundwert die Summe der Verglasungsbeträge der Positionen verwendet. Auf Kostenseite haben Verglasungsrabatte immer einen Betrag von 0.
- `☑` Der Rabatt bezieht sich nur auf Verglasungen.
- `☐` Der Rabatt bezieht sich auf alles.
*Technische Info: Toggle-Feld, DB-Feld: rabstamm.verglkz*

**Glasgewicht**
Über dieses Feld können Sie steuern, auf welches Gewicht sich der Rabatt beziehen soll. Diese Information übersteuert die Information aus dem Methodenstamm, so dass Rabatte einer Methode unterschiedliche Bezugsgewichte haben können. Das Glasgewicht beeinflusst den Grundwert des Rabatttyps WE/kg sowie das Ziehen der Staffelstufe innerhalb der Vorgänge.
- **Posgew.:** Positionsgewicht.
- **Nur Glasgew.:** Reine Glasgewicht.
- **Glasgew.:** Glasgewicht
- **Fak.Posgew.:** Fakturierte Positionsgewicht.
- **Nur fak. GGew:** Reine fakturierte Glasgewicht.
- **fak. Glasgew.:** Fakturierte Glasgewicht.
*Technische Info: Toggle-Feld, DB-Feld: rabstamm.glasgewicht*

**Min. bei Nullbetrag**
Über diese Checkbox steuern Sie, ob der Mindestbetrag auch dann gezogen wird, wenn der errechnete Betrag 0.0 WE ist.
- `☑` Der Rabatt wird auf die einzelnen Positionen zurück verteilt.
- `☐` Der Rabatt wird nicht auf die einzelnen Positionen zurück verteilt.
*Technische Info: Toggle-Feld, DB-Feld: rabstamm.minbeinullbetragk*

**Vorgang**
Kennzeichen, ob die Stored Procedure rabattanpassung aufgerufen werden muss, die den Rabatt vorgangsindividuell anpasst.
- `☑` Die SP muss aufgerufen werden.
- `☐` Die SP wird nicht aufgerufen.
*Technische Info: Toggle-Feld, DB-Feld: rabstamm.spaufrufkzkauf*

**Position**
Kennzeichen, ob die Stored Procedure rabattzuord aufgerufen werden soll, die dann entscheidet, welche Vorgangspositionen von diesem Rabatt berücksichtigt werden und welche nicht.
- `☑` Die SP wird aufgerufen.
- `☐` Die SP wird nicht aufgerufen.
*Technische Info: Toggle-Feld, DB-Feld: rabstamm.spaufrufkz*

**Rabatt-Id Zentrale**
Diese Variable steuert die Replikation der Daten aus der Zentrale in die entsprechende Filiale.
*Technische Info: Toggle-Feld, DB-Feld: rabstamm.rabattidz*

**Rabatt-Id**
Eindeutige Zuordnung zum Rabattsatz.
*Technische Info: Numerisches Feld, DB-Feld: rabstamm.rabattid*

### Hausspezifische Marktpartner-Angaben
*Stammdaten > Schlüssel > Marktpartner > Hausspezifische Angaben*

In diesem Dialog können Sie mandantenspezifischen Angaben zu Marktpartnern hinterlegen. Der Dialog ist nur aktiv, wenn Sie mit dem Mehr-Mandantensystem (Multi-Site) arbeiten.

#### Erläuterung der Felder
**Partnertyp**
Auswahl des Partnertyps.
*Technische Info: Toggle-Feld, DB-Feld: mpmdzu.kuliflag*

**Marktpartner**
Auswahl des Marktpartners.
*Technische Info: `<F9>`, DB-Feld: mpmdzu.mpnr*

**Haus**
Auswahl der Hausnummer. Der Name wird im Feld dahinter angezeigt.
*Technische Info: `<F9>`, DB-Feld: mpmdzu.hnr*

**Vertr.(Erlös)**
Auswahl des erlösmäßigen Vertreters. Für den hier eingetragenen Mitarbeiter werden dann die jeweiligen Provisionssätze gebucht und stehen zur Abrechnung bereit. Der Name wird im Feld dahinter angezeigt.
*Technische Info: `<F9>`, DB-Feld: mpmdzu.lager*

**Konditionsdebitor**
Auswahl der Kundennummer, deren Konditionen für die erfassten Vorgänge gelten soll.
*Technische Info: `<F9>`, DB-Feld: mpmdzu.konddebnr*

## Systemschlüssel
*Stammdaten > Schlüssel > System*

Hier werden Werte für verschiedene Bereiche definiert, die später als Auswahl zur Verfügung stehen.
Es werden z. B. die lizenzierten Sprachen eingetragen, die für die Reporterzeugung in verschiedenen Sprachen benötigt werden.

Sie haben Zugriff auf folgende Bereiche:

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a a/b | Position | ⇨ "Positionsbezeichnungen" auf Seite B-154 |
| b | Postleitzahlen | ⇨ "Postleitzahlen" auf Seite B-155 |
| c | Sprachen | ⇨ "Sprachen" auf Seite B-157 |
| d a/b | Textzusätze | ⇨ "Textzusatzbezeichnungen" auf Seite B-160 |
| e | Dokumentenarten | ⇨ "Dokumentenarten" auf Seite B-161 |
| f a/b | Mengeneinheiten | ⇨ "Mengeneinheitenbezeichnung" auf Seite B-163 |
| g a | Modelle - Kantenzuordnung | ⇨ "Kantenzuordnung" auf Seite B-165 |
| g b/c | Modelle | ⇨ "Modellbezeichnungen" auf Seite B-167 |
| h | Produktionsbereich | ⇨ "Produktionsbereich" auf Seite B-169 |
| i a | Versand - Verpackungsart | ⇨ "Verpackungsart" auf Seite B-170 |
| i b | Versand - Gestell-Verpackungsarten | ⇨ "Gestell-Verpackungsarten" auf Seite B-171 |
| i c | Versand - Versandart | ⇨ "Versandart" auf Seite B-172 |
| i d | Versand - Lieferarten | ⇨ "Lieferarten" auf Seite B-174 |
| i e a | Versand - Routen | ⇨ "Routen" auf Seite B-175 |
| i e b | Versand - Tourenplan | ⇨ "Tourenplan" auf Seite B-179 |
| i f a/b | Versand - Versandregionen | ⇨ "Versandregionenbezeichnung" auf Seite B-180 |
| i g | Versand - Fahrzeuge | ⇨ "Fahrzeuge" auf Seite B-181 |
| i h | Versand - Ausgangszoll | ⇨ "Ausgangszoll" auf Seite B-182 |
| i i | Versand - Bestimmungszoll | ⇨ "Bestimmungszoll" auf Seite B-184 |
| i j | Versand - Versandgruppen | ⇨ "Versandgruppen" auf Seite B-185 |
| j a/b | Gestellstatus | ⇨ "Gestellstatusbezeichnungen" auf Seite B-186 |
| k a a/b | PMO - Gestellgruppen | ⇨ "Gestellgruppenbezeichnungen" auf Seite B-187 |
| k a a/b | PMO - Verpackungsmethoden | ⇨ "Verpackungsmethodenbezeichnung" auf Seite B-188 |
| k c | PMO - Gestell-Verpackungszuordnung | ⇨ "Gestell-Verpackungszuordnung" auf Seite B-189 |
| l | Währung | ⇨ "Währung" auf Seite B-190 |
| m a | Steuern - Steuertypen | ⇨ "Steuertypen" auf Seite B-193 |
| m b | Steuern - Steuersätze | ⇨ "Steuersätze" auf Seite B-195 |
| n | Zahlungsweise | ⇨ "Zahlungsweisebezeichnungen" auf Seite B-196 |
| o a | Skontogruppen | ⇨ "Skontogruppen" auf Seite B-198 |
| o b/c | Skontogruppenbezeichnungen | ⇨ "Skontogruppenbezeichnung" auf Seite B-200 |
| p | Periodenende | ⇨ "Periodenende" auf Seite B-201 |
| q a/b | Adhocsql - Gruppen | ⇨ "Adhocsql-Gruppenbezeichnungen" auf Seite B-202 |
| r | Report - Texte | ⇨ "Report-Texte" auf Seite B-203 |
| s a | Firmen/Gesellschaften | ⇨ "Firmen / Gesellschaften" auf Seite B-205 |
| s b | Firmen/Gesellschaften - Firmenzuordnung | ⇨ "Firmenzuordnung" auf Seite B-206 |

### Positionsbezeichnungen
- Stammdaten > Schlüssel > System > Position > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > System > Position > Alle Bezeichnungen

In diesem Dialog definieren Sie die Positionen der Mitarbeiter im Unternehmen. Sie dienen dann später bei der Stammdatenerfassung als Spezifikation der Mitarbeiterposition.

#### Erläuterung der Felder
**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Position geben Sie die nächste freie Nummer ein.
*Technische Info: Numerisches Feld, DB-Feld: xsprbez.id, View: xpos.posnr*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Bezeichnung der Position, z. B. Geschäftsführer.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1, View: xpos.atxt*

### Postleitzahlen
*Stammdaten > Schlüssel > System > Postleitzahlen*

In diesem Dialog können Sie alle Postleitzahlen hinterlegen, die Sie später bei der Auftragserfassung benötigen. Die hier hinterlegten Postleitzahlen erleichtern die Erfassung von Adressen.
Im Bereich Auswahlmenge können Sie Suchkriterien eingeben und somit die Anzahl der Treffer eingrenzen. Ohne Auswahlmenge, werden alle Postleitzahlen angezeigt. `*` steht für alle Einträge.
Im unteren Bereich können Sie die Angaben korrigieren oder auch neue Einträge hinzufügen.

#### Erläuterung der Felder für die Auswahlmenge
**Postleitzahl**
Auswahl und Eingabe der Postleitzahl als Suchwert. Sie können die komplette Postleitzahl eingeben oder nur den Anfang. `*` steht für alle.
*Technische Info: `<F9>`, DB-Feld: xplzk.plz*

**Ort**
Auswahl und neue Angabe des Ortes als Suchwert. Sie können den kompletten Ort eingeben oder nur den Anfang. `*` steht für alle.
*Technische Info: `<F9>`, DB-Feld: xplzk.ort*

**KFZ Land**
Eingabe des KFZ-Landes als Suchwert. Sie können das komplette Land eingeben oder nur den Anfang. `*` steht für alle.
*Technische Info: `<F9>`, DB-Feld: xplzk.kfz*

**Versandregion**
Auswahl der Versandregion als Suchwert. Sie können die Versandregion eingeben oder über `<F9>` auswählen. Versandregionen werden im gleichnamigen Menüpunkt Stammdaten > Schlüssel > System > Versand. -1 steht für keine Auswahl.
*Technische Info: `<F9>`, DB-Feld: xplzk.vsregion*

#### Erläuterung der Felder für die Treffermenge
**PLZ**
Postleitzahl. Zum Anlegen einer neuen Postleitzahl fügen Sie eine neue Zeile ein.
*Technische Info: Numerisches Feld, DB-Feld: xplz.plz*

**Ort**
Der zur Postleitzahl gehörende Ort.
*Technische Info: Alphanumerisches Feld, DB-Feld: xplz.ort*

**KFZ**
Das zur Postleitzahl gehörende Länderkennzeichen.
*Technische Info: alphabetisches Feld, DB-Feld: xplz.kfz*

**Versandregion**
Auswahl der Versandregion mit `<F9>`. Im Feld dahinter wird die Versandregion angezeigt. Versandregionen werden im gleichnamigen Menüpunkt Stammdaten > Schlüssel > System > Versand.
*Technische Info: Numerisches Feld, DB-Feld: xplz.vsregion*

### Sprachen
*Stammdaten > Schlüssel > System > Sprachen*

Dieser Dialog dient zur Verwaltung der lizenzierten Sprachen. Die Sprachen werden über einen Sprachschlüssel definiert. Dieser dient z. B. dazu, Kunden-Reports in Landessprache auszudrucken und jedem Marktpartner seine eigenen Sprache zuordnen zu können.
Die Nummer kann frei vergeben werden. In einem Konzern mit mehreren Datenbanken gilt jedoch, dass die Nummernzuordnung einheitlich erfolgen muss.
Das nachfolgende Beispiel soll dies verdeutlichen:
Ein Konzern mit Sitz in Frankreich hat Niederlassungen in Deutschland, England und Italien. Sowohl die Zentrale als auch die Niederlassungen ihrerseits haben Kunden im weiteren europäischen Ausland.

| Niederlassung | hat Kunden in |
| :--- | :--- |
| Zentrale Frankreich | Frankreich<br>Deutschland<br>Italien |
| Niederlassung Deutschland | Dänemark<br>Deutschland<br>Niederlande |
| Niederlassung England | England |
| Niederlassung Italien | Deutschland<br>Griechenland<br>Italien<br>Slowenien |

> **Landesübergreifende Auftragsübertragung**
> Damit innerhalb des Konzerns eine landesübergreifende Auftragsübertragung möglich ist, muss die Schlüsselnummer einer lizenzierten Sprache konzernweit gleich sein. Die Reportsprachen-Nummer ist abhängig von der Gestaltung der Reports und muss entsprechend abgestimmt werden

Die nachfolgende Tabelle zeigt, wie in der Zentrale und in den Filialen die Sprachen angelegt sein könnten:

| A+W Enterprise Datenbank | hat Kunden in | Lizenzierte Sprachen | Schlüssel-Nr. | Report-sprache |
| :--- | :--- | :--- | :--- | :--- |
| Zentrale Frankreich | Frankreich | französisch | 1 | 1 |
| | Deutschland | deutsch | 2 | 2 |
| | Italien | italienisch | 3 | 3 |
| | Spanien | spanisch | 4 | 4 |
| | | dänisch | 5 | |
| | | englisch | 6 | |
| | | griechisch | 7 | |
| | | slowenisch | 8 | |
| | | niederländisch | 9 | |
| Niederlassung Deutschland | Dänemark | dänisch | 5 | 1 |
| | Deutschland | deutsch | 2 | 2 |
| | Niederlande | niederländisch | 9 | 3 |
| Niederlassung England | England | englisch | 6 | 1 |
| Niederlassung Italien | Deutschland | deutsch | 2 | 1 |
| | Griechenland | griechisch | 7 | 2 |
| | Italien | italienisch | 3 | 3 |
| | Slowenien | slowenisch | 8 | 4 |

#### Erläuterung der Felder
**Nr.**
Sprachkennzeichen. Zum Anlegen eines neuen Sprachkennzeichens wählen Sie die nächst freie Nummer.
*Technische Info: Numerisches Feld, DB-Feld: xsprzu.sprkz*

**Sprache**
Sprachbezeichnung, z. B. Deutsch.
*Technische Info: alphabetisches Feld, DB-Feld: xsprzu.atxt*

**Reportsprache**
Auswahl der Sprache, in der der Report erfolgen soll.
*Technische Info: Numerisches Feld, DB-Feld: xsprzu.repsprkz*

**A+W Enterprise Sprache**
Auswahl der Sprache, in der das Programm angezeigt wird. Im Feld dahinter erscheint die Sprachbezeichnung.
*Technische Info: Numerisches Feld, DB-Feld: xsprzu.alenvsprkz*

### Textzusatzbezeichnungen
- Stammdaten > Schlüssel > System > Textzusätze > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > System > Textzusätze > Alle Bezeichnungen

Die Textzusätze dienen der Artikel- und Produktvertextung bei der Auftragserfassung und bei der Erzeugung von Reports. Genaue Verwendung diesen Textzusätzen kann der A+W Enterprise - Konfigurationsanleitung entnommen werden.

#### Erläuterung der Felder
**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen eines neuen Textes geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xzustxt.txtnr*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xzustxt.sprkz*

**Textkonstante**
Bezeichnung des Textes, z. B. waagerecht.
*Technische Info: Alphanumerisches Feld, DB-Feld: xzustxt.zustxt*

### Dokumentenarten
*Stammdaten > Schlüssel > System > Dokumentenarten*

In diesem Dialog können Sie verschiedene Dokumentenarten und die Art der Ausgabe hinterlegen. Für die Leistungserklärung(en) ist der Dokumententyp Leistungserklärung fest definiert und mit der Dokumentenart 1 verknüpft.
Über die Art der Ausgabe kann geregelt werden, ob der Marktpartner die Dokumente der gewählten Art per Email erhalten soll oder nicht. Der Emailversand benötigt weitere systemweite Einstellungen und Konfiguration.

#### Erläuterung der Felder
**Art**
Schlüsselnummer. Zum Anlegen einer neuen Schlüsselnummer wählen Sie die nächst freie Nummer.
*Technische Info: Numerisches Feld, DB-Feld: xdokutype.dokuart*

**Bezeichnung**
Bezeichnung der Dokumentenart, z. B. Leistungserklärung.
*Technische Info: alphabetisches Feld, DB-Feld: xdokutype.dokubez*

**Dokumententyp**
Zuordnung zu einem Dokumententyp.
*Technische Info: alphabetisches Feld, DB-Feld: xdokutype.dokutyp*

**Art der Ausgabe**
Über dieses Feld steuern Sie die Ausgabeart. Bei der Leistungserklärung ist dieses Feld mit E-Mail vorbelegt:
- **keine:** Der Marktpartner erhält keine Leistungserklärung.
- **per E-Mail:** Der Marktpartner erhält die Leistungserklärung per Mail.
*Technische Info: Toggle-Feld, DB-Feld: xdokutype.ausgabeart*

**VF**
Über dieses Feld steuern Sie, ob die Daten in den Vorgang übernommen werden sollen:
- `☑` Die Daten sollen übernommen werden.
- `☐` Die Daten sollen nicht übernommen werden.
*Technische Info: Toggle-Feld, DB-Feld: xdokutype.vorgangflag*

**Prod**
Über dieses Feld steuern Sie, ob die Daten an die Produktion übergeben werden sollen:
- `☑` Die Daten sollen übernommen werden.
- `☐` Die Daten sollen nicht übernommen werden.
*Technische Info: Toggle-Feld, DB-Feld: xdokutype.prodflag*

### Mengeneinheitenbezeichnung
- Stammdaten > Schlüssel > System > Mengeneinheiten > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > System > Mengeneinheiten> Alle Bezeichnungen

In diesem Dialog definieren Sie die Mengeneinheiten.

#### Erläuterung der Felder
**Nummer/Nr**
Auswahl der Schlüssel-Nummer. Zum Anlegen einer neuen Mengeneinheit geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id, View: xme.symb*

**Spr**
Auswahl des Sprachkennzeichens.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**KBez**
Kurzbezeichnung der Mengeneinheit, z. B. mtr.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1, View: xme.kurzbez*

**Bezeichnung**
Bezeichnung der Mengeneinheit, z. B. Meter.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez2, View: xme.atxt*

**Dimension**
Dimension der Mengeneinheit, z. B. Laufmeter (lfm).
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez3, View: xme.dim*

### Kantenzuordnung
*Stammdaten > Schlüssel > System > Modelle > Kantenzuordnung*

In diesem Dialog legen Sie fest, wie die Modellkanten bei umschriebenen Rechtecken interpretiert werden. Bei Modell 7 (Bild oben) wird z. B. die schräge Kante als Höhe behandelt.

#### Erläuterung der Felder
**Modell**
Auswahl der Modellnummer, für die die preisrelevante Kante definiert werden soll. Im Feld dahinter wird die Bezeichnung angezeigt.
*Technische Info: `<F9>`, DB-Feld: modkparam.modnr*

**Kante**
Für diese Kante soll definiert werden, ob sie als Höhe oder Breite in die Preisberechnung eingehen soll.
*Technische Info: Numerisches Feld, DB-Feld: modkparam.kante*

**Berechnung**
Definiert, wie die Kante in die Preisberechnung eingeht:
- 0: keine Berechnung
- 1: als Höhe
- 2: als Breite
- 3: als Höhe + Breite
- 4: 2x Höhe + Breite
- 5: Höhe + 2x Breite
- 6: 2x Höhe + 2x Breite
*Technische Info: Toggle-Feld, DB-Feld: modkparam.berechnung*

**MK**
Mit diesem Feld wird gesteuert, ob es sich bei der zu bearbeitenden Kante um eine Modellkante handelt.
- `☑` Bei dieser Kante handelt es sich um eine Modellkante.
- `☐` Diese Kante ist keine Modellkante.
*Technische Info: Alphanumerisches Feld, DB-Feld: modkparam.modellkante*

### Modellbezeichnungen
- Stammdaten > Schlüssel > System > Modelle > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > System > Modelle> Alle Bezeichnungen

In diesem Dialog hinterlegen Sie die Bezeichnungen zu den zu bearbeitenden Modellen. Die hier für die Modelle hinterlegten Texte werden sowohl in der Auftragserfassung als auch für die Kundenpapiere und für die Erstellung der Scheibenetiketten benötigt.

> **Zur Verfügung stehende Modelle**
> Welche Modelle hier zur Verfügung stehen, ist von der Systemeinstellung Katalogart abhängig.

#### Erläuterung der Felder
**Modellnummer/Nr**
Auswahl der Modellnummer. Die Modellnummer entspricht den Modellen des A+W Modellkatalogs, bzw. des Modellkatalogs, der bei der Installation eingerichtet wurde.
*Technische Info: `<F9>`, DB-Feld: modelle.modnr*

**Sprache**
Auswahl des Sprachkennzeichens.
*Technische Info: `<F9>`, DB-Feld: modelle.sprkz*

**Bezeichnung**
Die Modellbezeichnung entspricht den Modellen des A+W Modellkatalogs, bzw. des Modellkatalogs, der bei der Installation eingerichtet wurde.
*Technische Info: Alphanumerisches Feld, DB-Feld: modelle.bez*

**Druckbezeichnung**
Die Druckbezeichnung kann bei Bedarf geändert werden.
*Technische Info: Alphanumerisches Feld, DB-Feld: modelle.drubez*

**Erf**
Über dieses Feld steuern Sie, ob das Modell erfassbar ist oder nicht. Es kann vorkommen, dass Sie zwar mit dem A+W Modellkatalog arbeiten, die Modell aber nicht bei Ihnen geschnitten werden.
- **J:** Die Modellnummer kann erfasst werden.
- **N:** Die Modellnummer kann nicht erfasst werden.
*Technische Info: Toggle-Feld, DB-Feld: modelle.erfassbar*

**Online**
Dieses Feld ist für Online-Erfassungen relevant. Damit steuern Sie, ob das Modell online erfassbar ist oder nicht.
- **J:** Die Modellnummer kann online erfasst werden.
- **N:** Die Modellnummer kann nicht online erfasst werden.
*Technische Info: Toggle-Feld, DB-Feld: modelle.online*

**Kanten**
Anzahl der Kanten.
*Technische Info: Numerisches Feld, DB-Feld: modelle.kantanz*

### Produktionsbereich
*Stammdaten > Schlüssel > System > Produktionsbereich*

Dieser Dialog dient der Definition einzelner Produktionsbereiche, die in der Auftragserfassung zugeordnet werden können.

#### Erläuterung der Felder
**Nr**
Nummer des Produktionsbereiches.
*Technische Info: Numerisches Feld, DB-Feld: xpbbereich.bereich*

**Bereichsbezeichnung**
Bezeichnung des Produktionsbereiches, z. B. Siebdruck.
*Technische Info: Alphanumerisches Feld, DB-Feld: xpbbereich.bez*

### Verpackungsart
*Stammdaten > Schlüssel > System > Versand > Verpackungsart*

In diesem Dialog legen Sie die Verpackungsarten in den jeweiligen Sprachen fest. So kann sie auf den Kunden-Papieren in Landessprache ausgewiesen werden.

#### Erläuterung der Felder
**Nr**
Die Schlüssel-Nummer kann frei gewählt werden. Dieselbe Nummer soll mehrmals vergeben werden, wenn die Verpackungsart in mehreren Sprachen angelegt wird. In diesem Fall bleibt die Nummer gleich, Sprachschlüssel und Bezeichnung ändern sich jeweils.
*Technische Info: Numerisches Feld, DB-Feld: xverpack.verpnr*

**Bezeichnung**
Die Bezeichnung der Verpackungsart.
*Technische Info: Alphanumerisches Feld, DB-Feld: xverpack.atxt*

**mm**
In Abhängigkeit der Konfiguration geben Sie hier die Dicke (in mm) des Verpackungsmaterials zwischen zwei Glasscheiben ein. Die Angabe ist optional.
*Technische Info: Numerisches Feld, DB-Feld: xverpack.vdick*

**Sprache**
Auswahl der Sprache. Im Feld dahinter wird die ausgewählte Sprache angezeigt.
*Technische Info: `<F9>`, DB-Feld: xverpack.sprkz*

### Gestell-Verpackungsarten
*Stammdaten > Schlüssel > System > Versand> Gestell-Verpackungsarten*

In diesem Dialog können Sie einer Versandart (z. B. Spedition) in Abhängigkeit des Bestimmungslandes unterschiedliche Verpackungsarten zuweisen. Die Nutzung dieser Funktion ist extra konfigurierbar. Für weitere Information kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

#### Erläuterung der Felder
**Versandart**
Auswahl der Versandart, z. B. Spedition. Im Feld dahinter wird der Name angezeigt. Die entsprechenden Schlüssel können über das Menü Versandart (Stammdaten > Schlüssel > System > Versand) vergeben werden.
*Technische Info: Numerisches Feld, DB-Feld: gverpack.versnr*

**KFZ**
Auswahl des Länderkennzeichens, z. B. D. Im Feld dahinter wird der Name angezeigt. Die entsprechenden Schlüssel können über das Menü Länder (Stammdaten > Schlüssel > Marktpartner > Länder vergeben werden.
*Technische Info: alphabetisches Feld, DB-Feld: gverpack.kfz*

**Verpackungsart**
Auswahl der Verpackungsart, z. B. L-Gestelle. Im Feld dahinter wird der Name angezeigt. Die entsprechenden Schlüssel können über das Menü Verpackungsart (Stammdaten > Schlüssel > System > Versand) vergeben werden.
*Technische Info: Numerisches Feld, DB-Feld: gverpack.verpnr*

**Ergänzende Informationen**
- ⇨"Länder" auf Seite B-120
- ⇨ "Verpackungsart" auf Seite B-170
- ⇨ "Versandart" auf Seite B-172

### Versandart
*Stammdaten > Schlüssel > System > Versand> Versandart*

In diesem Dialog legen Sie die Versandarten in den jeweiligen Sprachen fest. So kann die Versandart auf den Kunden-Papieren in Landessprache ausgewiesen werden.

#### Erläuterung der Felder
**Nr**
Die Schlüssel-Nummer kann frei gewählt werden. Dieselbe Nummer kann mehrmals vergeben werden, wenn die Verpackungsart in mehreren Sprachen angelegt werden soll. In diesem Fall bleibt die Nummer gleich, Sprachschlüssel und Bezeichnung ändern sich jeweils.
*Technische Info: Numerisches Feld, DB-Feld: xversand.versnr*

**Bezeichnung**
Die Bezeichnung der Verpackungsart in der jeweiligen Sprache.
*Technische Info: Alphanumerisches Feld, DB-Feld: xversand.atxt*

**Route**
Die Auswahl einer Route ist optional. Im Feld dahinter wird die Route angezeigt.
*Technische Info: `<F9>`, DB-Feld: xversand.routenr*

**Verk**
Auswahl des Codes für den Verkehrszweig laut Vorgabe des Statistischen Bundesamtes. Im Feld dahinter wird die Bezeichnung angezeigt.
*Technische Info: `<F9>`, DB-Feld: xversand.intraverkehr*

**Transportzuschlag**
Der Transportzuschlag in Prozent ist ein Schätzwert, der für die Korrektur des statistischen Wertes benötigt wird.
*Technische Info: Numerisches Feld, DB-Feld: xversand.intrasatz*

**Sprache**
Auswahl der Sprache. Im Feld dahinter wird die ausgewählte Sprache im Klartext angezeigt.
*Technische Info: `<F9>`, DB-Feld: xversand.sprkz*

### Lieferarten
- Stammdaten > Schlüssel > System > Versand > Lieferarten > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > System > Versand > Lieferarten > Alle Bezeichnung

Dieser Dialog zeigt Ihnen die definierten Lieferarten, in den jeweiligen Sprachen. So kann sie auf den Kunden-Papieren in Landessprache ausgewiesen werden.

> **Mehrsprachige Bezeichnungen**
> Seit QR2209 können Sie in A+W Enterprise auch für Lieferarten mehrsprachige Bezeichnungen hinterlegen.

#### Erläuterung der Felder
**Nr/Lieferart**
Die Schlüssel-Nummer kann frei gewählt werden. Dieselbe Nummer kann mehrmals vergeben werden, wenn die Verpackungsart in mehreren Sprachen angelegt werden soll. In diesem Fall bleibt die Nummer gleich, Sprachschlüssel und Bezeichnung ändern sich jeweils.
*Technische Info: Numerisches Feld, DB-Feld: xlart.lanr*

**Bezeichnung**
Die Bezeichnung der Lieferart in der jeweiligen Sprache.
*Technische Info: Alphanumerisches Feld, DB-Feld: xlart.labez*

**Spr**
Auswahl der Sprache (Sprachkennzeichen).
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

### Routen
- Stammdaten > Schlüssel > System > Versand > Routen > Routen > Routenangaben I
- Stammdaten > Schlüssel > System > Versand > Routen > Routen > Einzelne Bezeichnung
- Stammdaten > Schlüssel > System > Versand > Routen > Routen > Alle Bezeichnung

In der Routenverwaltung werden die Auslieferungswege beschrieben. So kann bei der Auftragserfassung eine Lieferroute zugeordnet und bei der Berechnung des Liefertermins berücksichtigt werden.

> **Mehrsprachige Bezeichnungen**
> Seit QR2209 können Sie in A+W Enterprise auch für Routen mehrsprachige Bezeichnungen hinterlegen.

#### Erläuterung der Felder
**Route**
Eindeutige Nummer der Route.
*Technische Info: Numerisches Feld, DB-Feld: route.routenr*

**Routenbezeichnung**
Die Bezeichnung der Route.
*Technische Info: Alphanumerisches Feld, DB-Feld: route.routename*

**Kürzel**
Kürzel der Route.
*Technische Info: Alphanumerisches Feld, DB-Feld: route.kurzbez*

**Anfahrttage**
Auswahl der Anfahrttage (Mo-So).
*Technische Info: `<F9>`, DB-Feld: route.routentag*

**Abfahrt**
Abfahrtzeit für die Tour.
*Technische Info: Numerisches Feld, DB-Feld: route.abfahrt*

**AuswR**
Die Ausweichroute verweist auf eine andere Zeile derselben Tabelle, in der eine Alternative zur aktuellen Route zu finden ist. Sie wird bei Sperrung dieser Route herangezogen.
*Technische Info: Numerisches Feld, DB-Feld: route.aroutenr*

**Art**
Auswahl der Routenart:
- **Route:** Tour mit mehreren Anfahrtpunkten.
- **Direkt:** Ware wird vom Vorlieferanten direkt ausgeliefert.
- **Abholung:** Ware wird vom Kunden abgeholt.
- **Rückst.:** Ware befindet sich im Rückstand (Planungsroute).
- **Intern:** Route zwischen zwei miteinander verbunden Unternehmen (viaPlant).
*Technische Info: `<F9>`, DB-Feld: route.routenkz*

**Haus**
Auswahl der Hausnummer, zu der die Route gehört. Das Feld hat zwei Bedeutungen:
- In einer A+W Enterprise-Instanz, in der mehrere Mandanten verwaltet werden, gibt die Hausnr. an, von welchem Haus aus eine Route gefahren wird.
- Wird zwischen zwei verbundenen A+W Enterprise-Instanzen ein Auftrag mit Direktauslieferung übertragen, wo wird im empfangenden Haus die Route mit dem eigenen Routenstamm abgegelichen. Es wird diejenige Direktroute ausgewählt, deren Hausnr. mit der Hausnummer des sendenden Hauses übereinstimmt. In diesem Fall gibt die Hausnr. an, für welches Haus eine Direktauslieferung erfolgen soll.
*Technische Info: `<F9>`, DB-Feld: route.hausnr*

**Reg/Haus**
Auswahl der Region, zu der die Route gehört. Die entsprechenden Schlüssel können über das Menü Versandregionen (Schlüssel > System > Versand) vergeben werden.
*Technische Info: `<F9>`, DB-Feld: route.region*

**Prio**
Eingabe der Priorität innerhalb einer Region für via Plant.
*Technische Info: Numerisches Feld, DB-Feld: route.prio*

**Zeit**
Eingabe der Fahrtzeit in Stunden.
*Technische Info: Numerisches Feld, DB-Feld: route.fahrtzeit*

**Kal**
Mit diesem Feld steuern Sie, ob der Kalender ausgewertet werden soll oder nicht.
- `☑` Der Kalender wird ausgewertet.
- `☐` Der Kalender wird nicht ausgewertet.
*Technische Info: Toggle-Feld, DB-Feld: route.mitkalender*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Ergänzende Informationen**
⇨ "Routenangaben II" auf Seite B-178

### Routenangaben II
*Stammdaten > Schlüssel > System > Versand > Routen > Routen > F2*

Die Felder in diesem Dialog sind mit Ausnahme des Feldes Versandart identisch mit den Feldern des Dialogs Routenangaben I.

> **Routenangaben II**
> Das Register Routenangaben II ist standardmäßig ausgeblendet. Die Freischaltung kann über einen Mitarbeiter der A+W Software GmbH erfolgen.

#### Erläuterung der Felder
**Versandart**
Auswahl der Versandart. Die entsprechenden Schlüssel können über das Menü Versandart (Stammdaten > Schlüssel > System > Versand) vergeben werden. Im weiteren Feld wird die Bezeichnung der Versandart im Klartext dargestellt.
*Technische Info: `<F9>`, DB-Feld: route.versnr*

**Ergänzende Informationen**
⇨ "Routen" auf Seite B-175

### Tourenplan
*Stammdaten > Schlüssel > System > Versand > Routen > Tourenplan*

In diesem Dialog legen Sie die genauen Abfahrtszeiten für die einzelnen Routen fest. So können Sie z. B. für eine Route, die zwei Mal pro Tag gefahren wird, die unterschiedlichen Abfahrtszeiten definieren. Den Tourenplan können Sie dem Kundenauftrag entsprechend zuordnen.

#### Erläuterung der Felder
**Route**
Auswahl der Routennummer. Im Feld dahinter wird die ausgewählte Route angezeigt
*Technische Info: `<F9>`, DB-Feld: tourplan.routenr*

**Datum**
Datum, an dem die Tour gefahren wird.
*Technische Info: Alphanumerisches Feld, DB-Feld: tourplan.tourdate*

**Abfahrt**
Abfahrtszeit für die Route.
*Technische Info: Alphanumerisches Feld, DB-Feld: tourplan.abfahrt*

### Versandregionenbezeichnung
- Stammdaten > Schlüssel > System > Versand > Versandregionen > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > System > Versand > Versandregionen > Alle Bezeichnungen

In diesem Dialog definieren Sie die einzelnen Versandregionen in den verschiedenen Sprachen.

#### Erläuterung der Felder
**Nummer**
Schlüssel-Nummer. Zum Anlegen einer neuen Versandregion geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id*

**Sprache**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Bezeichnung der Versandregion, z. B. Bayern.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1*

### Fahrzeuge
*Stammdaten > Schlüssel > System > Versand > Fahrzeuge*

In diesem Dialog hinterlegen Sie alle Fahrzeuge, die zur Auslieferung der Waren zur Verfügung stehen.

#### Erläuterung der Felder
**Fahrzeug**
Schlüsselnummer des Fahrzeugs. Zum Anlegen einer neuen Schlüsselnummer wählen Sie die nächst freie Nummer.
*Technische Info: Numerisches Feld, DB-Feld: lkw.lkwnr*

**Kennzeichen**
Amtliches KFZ-Kennzeichen des Fahrzeugs.
*Technische Info: Alphanumerisches Feld, DB-Feld: lkw.kennz*

**Fahrzeugart**
Auswahl der Fahrzeugart:
- LKW
- Zugmaschine
- Anhänger
*Technische Info: Toggle-Feld, DB-Feld: lkw.art*

**Bezeichnung**
Hierbei handelt es sich um eine freie, im Unternehmen gebräuchliche Bezeichnung für das Fahrzeug. Sie erscheint in der Versandsteuerung.
*Technische Info: Alphanumerisches Feld, DB-Feld: lkw.bezeichnung*

**Tonnage**
Hier wird die Nutzlast des Fahrzeugs eingetragen. Sie dient reinen Informationen und wird nicht ausgewertet.
*Technische Info: Numerisches Feld, DB-Feld: lkw.tonnage*

### Ausgangszoll
*Stammdaten > Schlüssel > System > Versand > Ausgangszoll*

In diesem Dialog hinterlegen Sie die Abgangszollstellen an den Außengrenzen. Die Nutzung der Ausgang- /Bestimmungszollfunktion ist konfigurationspflichtig. Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

#### Erläuterung der Felder
**Nr.**
Schlüsselnummer der Zollstelle. Zum Anlegen einer neuen Schlüsselnummer wählen Sie die nächst freie Nummer.
*Technische Info: Numerisches Feld, DB-Feld: xazstelle.azsnr*

**Ausgangszollstelle**
Bezeichnung der Abgangszollstelle gemäß der Zollbestimmungen.
*Technische Info: alphabetisches Feld, DB-Feld: xazstelle.bez*

**B.-Land**
Auswahl des Bestimmungslandes. Im Feld dahinter wird die Bezeichnung angezeigt.
*Technische Info: `<F9>`, DB-Feld: xazstelle.beland*

**Zollamtsart**
Auswahl der Zollamtsart. Im Feld dahinter wird die Bezeichnung angezeigt:
- **HZA:** Hauptzollamt
- **DZA:** Deutsches Zollamt
- **ZA:** Zollamt
- **AbfSt:** Abfertigungsstelle
*Technische Info: `<F9>`, DB-Feld: xazstelle.zaart*

**Verkehrszw**
Auswahl des Verkehrszweiges. Im Feld dahinter wird die Bezeichnung angezeigt:
- 1 - Seeverkehr
- 2 - Eisenbahn
- 3 - Landstraße
- 4 - Luftverkehr
- 5 - Postsendung
- 7 - fest installiert
- 8 - Binnenschifffahrt
- 9 - eigener Antrieb
- 99 - sonstige
*Technische Info: `<F9>`, DB-Feld: xazstelle.vkzweig*

### Bestimmungszoll
*Stammdaten > Schlüssel > System > Versand > Bestimmungszoll*

In diesem Dialog hinterlegen Sie die Bestimmungszollstellen an den Außengrenzen. Die Nutzung der Ausgang- /Bestimmungszollfunktion ist konfigurationspflichtig. Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

#### Erläuterung der Felder
**Nr.**
Schlüsselnummer der Zollstelle. Zum Anlegen einer neuen Schlüsselnummer wählen Sie die nächst freie Nummer.
*Technische Info: Numerisches Feld, DB-Feld: xbzstelle.bzsnr*

**KFZ**
Auswahl des Landes, in dem die Zollstelle liegt. Im Feld dahinter wird die Bezeichnung angezeigt
*Technische Info: `<F9>`, DB-Feld: xbzstelle.kfz*

**Bestimmungszollstelle**
Bestimmungszollstelle gemäß den Zollbestimmungen.
*Technische Info: alphabetisches Feld, DB-Feld: xazstelle.bez*

### Versandgruppen
*Stammdaten > Schlüssel > System > Versand > Versandgruppen*

In diesem Dialog können Sie Versandgruppen definieren. Diese werden in der Versandsteuerung ausgewertet und dienen der Datenselektion.

#### Erläuterung der Felder
**Versandgruppe**
Schlüsselnummer der Versandgruppe. Zum Anlegen einer neuen Schlüsselnummer wählen Sie die nächst freie Nummer.
*Technische Info: Numerisches Feld, DB-Feld: xvsgruppe.vsgruppenr*

**Bezeichnung**
Die Bezeichnung der Versandgruppe, z. B. ISO-Gruppe.
*Technische Info: Alphanumerisches, DB-Feld: xvsgruppe.bez*

**Standardgruppe**
In diesem Feld definieren Sie, ob es sich bei der Versandgruppe um eine Standardgruppe handelt. Beim Start der Versandsteuerung wird das entsprechende Feld mit diesem Wert belegt.
- `☑` Bei dieser Versandgruppe handelt es sich um eine Standardgruppe.
- `☐` Diese Versandgruppe ist keine Standardgruppe.
*Technische Info: alphabetisches Feld, DB-Feld: xvsgruppe.stdgruppe*

### Gestellstatusbezeichnungen
- Stammdaten > Schlüssel > System > Gestellstatus > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > System > Gestellstatus > Alle Bezeichnungen

In diesem Dialog definieren Sie den Status für Gestelle in den verschiedenen Sprachen. Der Gestellstatus wird in der Gestellverwaltung benötigt.

#### Erläuterung der Felder
**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen eines neuen Gestellstatus geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id*

**Sprache**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Bezeichnung des Gestellstatus, z. B. verkauft.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1*

### Gestellgruppenbezeichnungen
- Stammdaten > Schlüssel > System > PMO > Gestellgruppen > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > System > PMO > Gestellgruppen > Alle Bezeichnungen

In diesem Dialog definieren Sie Hauptgruppen für Gestelle in verschiedenen Sprachen. D. h, Sie können Gestelltypen zu Gestellhauptgruppen zusammenfassen.

#### Erläuterung der Felder
**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Gestellgruppe geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id, View: xghgr.ghgrnr*

**Sprache**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Kurzbez.**
Die Kurzbezeichnung des Gestellhauptgruppe, z. B. GG.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1, View: xghgr.kurzbez*

**Bezeichnung**
Die Bezeichnung des Gestellhauptgruppe, z. B. große Gestelle.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez2, View: xghgr.bez*

### Verpackungsmethodenbezeichnung
- Stammdaten > Schlüssel > System > PMO > Verpackungsmethoden > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > System > PMO > Verpackungsmethoden > Alle Bezeichnungen

In diesem Dialog definieren Sie die Verpackungsmethoden in den verschiedenen Sprachen.

#### Erläuterung der Felder
**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Verpackungsmethode geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id*

**Sprache**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Bezeichnung der Verpackungsmethode, z. B. PMO1.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1*

### Gestell-Verpackungszuordnung
*Stammdaten > Schlüssel > System > PMO > Gestell-Verpackungszuordnung*

In diesem Dialog können erlaubte Kombinationen aus Gestellgruppen und Verpackungsmethoden hinterlegt werden.

#### Erläuterung der Felder
**Nr**
Auswahl der Gestellgruppe. Im Feld dahinter wird die Gestellgruppe angezeigt.
*Technische Info: `<F9>`, DB-Feld: pmogestverp.pmogestgrpid*

**Nr**
Auswahl der Verpackungsmethode. Im Feld dahinter wird die Verpackungsmethode angezeigt.
*Technische Info: `<F9>`, DB-Feld: pmogestverp.pmoverpackid*

**Parameter**
In diesem Feld hinterlegen Sie die PMO-Parameter für diese Schlüsselkombination. Ein Schlüsselpaar darf jeweils nur einmal existieren.
*Technische Info: Alphanumerisches Feld, DB-Feld: pmogestverp.pmoparameter*

### Währung
- Stammdaten > Schlüssel > System > Währung > Währung
- Stammdaten > Schlüssel > System > Währung > Einzelne Bezeichnung
- Stammdaten > Schlüssel > System > Währung > Alle Bezeichnung

In diesem Dialog pflegen Sie die Währungen und Umrechnungsfaktoren, in denen die Preise angezeigt werden. Die Währung ordnen Sie dem Marktpartner in den Stammdaten > Register Zahlung zu.

> **Voraussetzungen**
> Mit unterschiedlichen Währungen können Sie nur arbeiten, wenn das kostenpflichtiges Modul zur Mehrwährungsfähigkeit konfiguriert ist. Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

> **Mehrsprachige Bezeichnungen**
> Seit QR2209 können Sie in A+W Enterprise auch für Währung mehrsprachige Bezeichnungen hinterlegen.

#### Erläuterung der Felder
**Nr**
Der Währungsschlüssel wird bei der Definition von Preislisten (PLKZ) benötigt sowie bei der Kunden- und Lieferantenerfassung, um Auftragswerte in der Währung des Kunden ausweisen und berechnen zu können. Zum Anlegen eines neuen Währungsschlüssels geben Sie die nächste freie Nummer ein.
*Technische Info: Numerisches Feld, DB-Feld: xwaehr.wnr*

**Kürzel**
Kürzel der Währung kann frei vergeben werden, z. B. KRW. Es ist jedoch ratsam, die internationale Kennzeichnung der Währung zu verwenden.
*Technische Info: Alphanumerisches Feld, DB-Feld: xwaehr.kurzbez*

**Bezeichnung**
Bezeichnung der Währung kann frei vergeben werden, z. B. Koreanischer Won.
*Technische Info: alphabetisches Feld, DB-Feld: xwaehr.bezeichn*

**Kurs**
Kurs, mit dem Beträge der Landeswährung in die Fremdwährung umgerechnet werden.
*Technische Info: alphabetisches Feld, DB-Feld: xwaehr.kurs*

**Faktor**
Der Kurs multipliziert mit dem Faktor ergibt den eigentlichen Kurs. Das Feld kann zum Austausch mit der Finanzbuchhaltung verwendet werden.
*Technische Info: Numerisches Feld, DB-Feld: xwaehr.faktor*

**Min. WE**
Kleinste Währungseinheit, z. B. 0,01 EUR.
*Technische Info: Numerisches Feld, DB-Feld: xwaehr.min_we*

**Rundung**
Rundungsart:
- **Keine:** Es erfolgt keine Rundung.
- **Kau:** Es wird kaufmännisch gerundet.
- **Auf:** Es wird aufgerundet.
- **Ab:** Es wird abgerundet.
*Technische Info: Toggle-Feld, DB-Feld: xwaehr.we_rund*

**Eurofaktor**
Umrechnungskurs zum EURO.
*Technische Info: Numerisches Feld, DB-Feld: xwaehr.eurokurs*

**Still**
Währung ist stillgelegt. Eine stillgelegte Währung kann im Marktpartner nicht mehr ausgewählt werden. In den Aufträgen und Rechnungen kann die Währung dennoch verbleiben. Wird ein Vorgang erneut bearbeitet, werden Sie dann aufgefordert, die stillgelegte Währung zu ändern.
- **Ja:** Die Währung ist stillgelegt, z. B. italienische Lire.
- **Nein:** Die Währung existiert noch.
*Technische Info: Numerisches Feld, DB-Feld: xwaehr.stillkz*

**FIBU-Key**
Das Feld kann zum Austausch mit der Finanzbuchhaltung verwendet werden.
*Technische Info: Numerisches Feld, DB-Feld: xwaehr.fibuschl*

**MwSt-Konto**
Mehrwertsteuer-Konto. Das Feld kann zum Austausch mit der Finanzbuchhaltung verwendet werden.
*Technische Info: Numerisches Feld, DB-Feld: xwaehr.mwstkto*

**Erlös-Kto**
Erlös-Konto. Das Feld kann zum Austausch mit der Finanzbuchhaltung verwendet werden.
*Technische Info: Numerisches Feld, DB-Feld: xwaehr.erloeskto*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

### Steuertypen
- Stammdaten > Schlüssel > System > Steuern > Steuertypen > Steuertypen
- Stammdaten > Schlüssel > System > Steuertypen > Einzelne Bezeichnung
- Stammdaten > Schlüssel > System > Steuertypen > Alle Bezeichnung

In diesem Dialog hinterlegen Sie die Steuertypen, die für die Erfassung der Marktpartner und für die Vorgangserzeugung notwendig sind.

> **Mehrsprachige Bezeichnungen**
> Seit QR2209 können Sie in A+W Enterprise auch für Steuertypen mehrsprachige Bezeichnungen hinterlegen.

#### Erläuterung der Felder
**Nummer**
Nummer des Steuertyps. Zum Anlegen eines neuen Währungsschlüssels wählen Sie die nächst freie Nummer.
*Technische Info: Numerisches Feld, DB-Feld: xkukz.kukz*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Bezeichnung des Steuertyps kann frei vergeben werden, z. B. Ausland (EG).
*Technische Info: Alphanumerisches Feld, DB-Feld: xkukz.bez*

### Steuersätze
*Stammdaten > Schlüssel > System > Steuern > Steuersätze*

In diesem Dialog weißen Sie den einzelnen Steuertypen die entsprechenden Steuersätze zu.

#### Erläuterung der Felder
**Nummer**
Auswahl des Steuertyps. Im Feld dahinter wird der Steuertyp angezeigt.
*Technische Info: `<F9>`, DB-Feld: xmwst.kukz*

**Steuersatz**
Hier hinterlegen Sie für den Steuertyp den entsprechenden Steuersatz in Prozent. Sollten Sie mehrerer Steuersätze benötigen, können Sie die Felder Steuersatz 1-3 verwenden.
*Technische Info: Numerisches Feld, DB-Feld: xmwst.satz, satz1-3*

**gültig ab**
Hier hinterlegen Sie, ab wann der Steuersatz für den Steuertyp gültig ist.
*Technische Info: Numerisches Feld, DB-Feld: xmwst.giltab*

**MwSt-Konto**
Mehrwertsteuer-Konto. Das Feld kann zum Austausch mit der Finanzbuchhaltung verwendet werden.
*Technische Info: Numerisches Feld, DB-Feld: xmwst.mwstkto*

**Vorsteuer-Konto**
Vorsteuer-Konto. Das Feld kann zum Austausch mit der Finanzbuchhaltung verwendet werden.
*Technische Info: Numerisches Feld, DB-Feld: xmwst.vstkto*

### Zahlungsweisebezeichnungen
- Stammdaten > Schlüssel > System > Zahlungsweise > Zahlungsweise
- Stammdaten > Schlüssel > System > Zahlungsweise > Einzelne Bezeichnung
- Stammdaten > Schlüssel > System > Zahlungsweise > Alle Bezeichnung

In diesen Dialogen hinterlegen Sie die einzelnen Zahlungsweisen, die in Ihrem Unternehmen vorkommen können.

#### Erläuterung der Felder
**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Zahlungsweise geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id, View: xzahlm.zmnr*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Bezeichnung des Zahlungsmerkmals, z. B. Vorauskasse.
*Technische Info: alphabetisches Feld, DB-Feld: xsprbez.bez1, View: xzahlm.atxt*

**FIBU**
Kürzel für die Finanzbuchhaltung.
*Technische Info: alphabetisches Feld, DB-Feld: xxzahlm.fib*

### Skontogruppen
*Stammdaten > Schlüssel > System > Skontogruppen > Skontogruppen*

In diesem Dialog legen Sie die Skontogruppen an, die Sie den Marktpartnern zuordnen können. Die Gruppen stehen sowohl im Verkauf als auch im Einkauf zur Verfügung und sind dort noch änderbar.

#### Erläuterung der Felder
**Zahlungsbedingung**
Anzeige der Schlüssel-Nummer. Zum Anlegen eines neuen Ortes geben Sie die nächste freie Nummer ein.
*Technische Info: Numerisches Feld, DB-Feld: xxxskonto.zahlbed*

**Art**
Bezeichnung der Skontoart. Text kann frei eingetragen werden.
*Technische Info: Alphanumerisches Feld, DB-Feld: xxxskonto.art*

**Monat**
Mit diesem Feld steuern Sie, wie viele (volle) Monate zum Rechnungsdatum bzw. zum Fälligkeitsdatum addiert werden.
*Technische Info: Numerisches Feld, DB-Feld: xxxskonto.monat*

**Frist 1**
Falls nötig, kann zusätzlich eine Frist addiert werden. Beispiel: Rechnungsdatum 14.02., Monat = 1, Frist = 15 Tage:
14.02. + 1 Monat = 14.03.
14.03. + 15 Tage = 29.03.
*Technische Info: Numerisches Feld, DB-Feld: xxxskonto.frist1*

**Legungstag 1-3/Frist 2**
Die Legungstage (Legungstag 1 - Legungstag 3) und eine Frist 2 ermöglichen eine Ausweitung des Gültigkeitszeitraumes für den Skontoabzug. Diese Felder müssen nicht zwingend gefüllt sein. Das Legungsdatum 30 entspricht dem Monatsletzten.
Beispiel:
Rechnungsdatum 10.02., Monat = 1, Frist = 10 Tage, Legungsdatum 1 = 15, Legungsdatum 2 = 30:
10.02. + 1 Monat = 10.03.
10.03. + 10 Tage = 20.03.
Die Liste der möglichen Rechnungslegungstage führt zum 31.03. da ausgehend vom 20.3. der nächstmögliche Legungstag ermittelt wird.
31.03. + 5 Tage = 05.04.
Dies bedeutet, dass der Anspruch auf Skontoabzug bis zum 04.04. geltend zu machen ist.
*Technische Info: Alphanumerisches Feld, DB-Feld: xxxskonto.rechlegtag1-3, frist2*

**Skontosatz**
Höhe des gewährten Skontos in Prozent.
*Technische Info: Numerisches Feld, DB-Feld: xxxskonto.satz*

**Bezeichnung**
Definierte Zahlungsbedingung in Worten, z. B. 10 Tage 2% Skonto.
*Technische Info: Alphanumerisches Feld*

**Folgebedingung**
Die Folgebedingung verweist auf den Schlüssel einer weiteren Skontovereinbarung, die nach Ablauf der Frist für die erste Skontovereinbarung in Kraft tritt.
*Technische Info: `<F9>`, DB-Feld: xxxskonto.folgezahlbed*

### Skontogruppenbezeichnung
- Stammdaten > Schlüssel > System > Skontogruppen > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > System > Skontogruppen > Alle Bezeichnungen

Diese Dialoge enthalten die Skontogruppen in den jeweiligen Sprachen.

#### Erläuterung der Felder
**Nummer**
Auswahl der Schlüssel-Nummer Zum Anlegen einer neuen Gruppe geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id*

**Spr**
Auswahl des Sprachkennzeichens.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Bezeichnung der Gruppe, z. B. 30 Tage Netto.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1*

### Periodenende
*Stammdaten > Schlüssel > System > Periodenende*

Das Periodenende dient in der FIBU als Abgrenzung der Buchungsperiode.

#### Erläuterung der Felder
**Periodenende**
Datum, an dem die aktuelle Buchungsperiode endet. In Abhängigkeit zur Konfiguration kann hier das EK-Periodenende, das VK-Periodenende oder beides eingetragen werden.
*Technische Info: Numerisches Feld, DB-Feld: periode.ek_periode, vk_periode*

**Geändert**
Datum der Änderung. Das Feld wird automatisch mit dem heutigen Datum gefüllt.
*Technische Info: Numerisches Feld, DB-Feld: periode.aenderdat*

**Von**
Name der Person, der die Änderung durchgeführt hat. Das Feld wird automatisch mit dem Namen der angemeldeten Person gefüllt.
*Technische Info: Alphanumerisches Feld, DB-Feld: periode.aendermanr*

### Adhocsql-Gruppenbezeichnungen
- Stammdaten > Schlüssel > System > Adhocsql-Gruppen > Einzelne Bezeichnungen
- Stammdaten > Schlüssel > System > Adhocsql-Gruppen > Alle Bezeichnungen

In diesen Dialogen legen Sie neue Adhocsql-Gruppen an oder nehmen Änderungen vor. Für diese Gruppen können Sie im Systemmenü `<Strg>` + `<F4>` ihre eigene Abfragen hinterlegen.

#### Erläuterung der Felder
**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Gruppe geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Bezeichnung der Gruppe, z. B. 30 Tage Netto.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1*

### Report-Texte
*Stammdaten > Schlüssel > System > Report-Texte*

Dieser Dialog zeigt Ihnen alle definierten Texte für Reports, in den jeweiligen Sprachen.

#### Erläuterung der Felder
**Typ**
Auswahlfeld für den Texttyp, um die Treffermenge zu begrenzen (optional).
*Technische Info: Alphanumerisches Feld, DB-Feld: cr_repstrings.type*

**Sprache**
Auswahlfeld für die Sprache, um die Treffermenge zu begrenzen (optional).
*Technische Info: Numerisches Feld, DB-Feld: cr_repstrings.sprkz*

**Typ**
Schlüsselbezeichnung des Textes. Diese wird im Report zum Referenzieren verwendet.
*Technische Info: Numerisches Feld, DB-Feld: cr_repstrings.type*

**Sprache**
Sprachkennzeichen.
*Technische Info: Numerisches Feld, DB-Feld: cr_repstrings.sprkz*

**Bezeichnung**
Sprachbezeichnung, z. B. englisch.
*Technische Info: Numerisches Feld, DB-Feld: cr_repstrings.sprkz*

**Text**
Name des Reports.
*Technische Info: Alphanumerisches Feld, DB-Feld: cr_repstrings.text*

**A+W-Flag**
Kennzeichen, ob der Text von A+W vorgegeben wird oder nicht.
- `☑` Der Text wird von A+W vorgegeben.
- `☐` Der Text wird nicht von A+W vorgegeben.
*Technische Info: Alphanumerisches Feld, DB-Feld: cr_repstrings.awflag*

### Firmen / Gesellschaften
*Stammdaten > Schlüssel > System > Firmen/Gesellschaften > Firmen/Gesellschaften*

Dieser Dialog zeigt Ihnen alle definierten Firmen bzw. Gesellschaften, in den jeweiligen Sprachen. Der Dialog steht Ihnen nur bei der Verwendung der Multi-Site-Funktion. Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

#### Erläuterung der Felder
**Firma**
Firmen ID. Zum Anlegen einer neuen Firma geben Sie die nächste freie Nummer ein
*Technische Info: Numerisches Feld, DB-Feld: xcompany.compid*

**Name**
Bezeichnung der Firma.
*Technische Info: Alphanumerisches Feld, DB-Feld: xcompany.name*

**Marktpartner**
Auswahl des Marktpartners. Hier werden nur die Sonstigen Marktpartner vorgeschlagen, deren mp.private_long1 ist.
*Technische Info: `<F9>`, DB-Feld: xcompany.mpnr*

### Firmenzuordnung
*Stammdaten > Schlüssel > System > Firmen/Gesellschaften > Firmenzuordnung*

Hier können Sie den einzelnen Häusern/Mandanten (Tabelle xhaus) eine Firma/Gesellschaft zuordnen. Die Daten werden anschließend in allen Bereichen (Vorgangserfassung, EK, Produktion) ausgewertet, um die richtige Hauszuordnung zu gewährleisten.
In diesem Dialog können keine neuen Häuser erfasst, sondern nur für bestehende Häuser eine Zuordnung vorgenommen werden. Bitte beachten Sie, dass ein Haus ohne Firmenzuordnung als nicht existent gilt.
Der Dialog steht Ihnen nur bei der Verwendung der Multi-Site-Funktion. Für weitere Informationen kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

> **Änderung der Zuordnung**
> Da eine Änderung der Zuordnung massive Folgen für das Vorgangshandling im gesamten System hat, wird bei jeder Änderung eine Sicherheitsabfrage gestellt, ob diese erwünscht ist.

#### Erläuterung der Felder
**Nr**
Mandantennummer. Der Name wird im Feld dahinter angezeigt.
*Technische Info: Anzeige-Feld, DB-Feld:xhaus.name*

**Haus**
Hausnummer. Der Name wird im Feld dahinter angezeigt.
*Technische Info: Anzeige-Feld, DB-Feld:site2comp.hausnr*

**Firma**
Auswahl der Firma oder Gesellschaft, die dem Mandanten zugeordnet werden soll. Die entsprechenden Schlüssel werden über das Menü Firmen/Gesellschaften (Stammdaten > Schlüssel > System > Firmen/Gesellschaften) vergeben.
*Technische Info: `<F9>`, DB-Feld:site2comp.compid*

**Kunde/Lieferant**
Anzeige der Kunden- und Lieferantennummer. Diese gelten als interner Marktpartner. Interne Marktpartner müssen unbedingt im Stamm gepflegt werden. Beim Öffnen des Dialogs für diesen Marktpartner im Menü Stammdaten > Marktpartner, ändert sich die Überschrift auf Interne Marktpartner. Auch bei internen Marktpartnern kann ein abweichender FIBU-Debitor hinterlegt werden. Allerdings gelten hier stärkere Restriktionen: zulässig sind nur interne Marktpartner, die zur gleichen Firma/Gesellschaft gehören. Wenn bei einem internen Marktpartner ein abweichender FIBU-Debitor eingetragen wurde, so gilt ab diesem Zeitpunkt auch eine verstärkte Kontrolle bei der Änderung der Firmenzuordnung.
Die Firmenzuordnung eines internen Marktpartners kann nicht geändert werden, wenn der Marktpartner auch anderen internen Marktpartnern als FIBU-Debitor zugeordnet ist. In diesem Fall müssen diese Abhängigkeit zunächst aufgelöst werden (also der FIBU-Debitor der betroffenen anderen internen Marktpartner geändert werden), bevor eine neue Firmenzuordnung stattfinden kann.
*Technische Info: Anzeige-Feld, DB-Feld: xhaus.kunr/linr*

**Host**
Hostname.
*Technische Info: Anzeige-Feld, DB-Feld:xhaus.host*

## Produktschlüssel
*Stammdaten > Schlüssel > Produkte*

Hier werden alle zulässigen Farben und Maßvarianten hinterlegt. Darüber hinaus ist es möglich, allgemeine Austauschregeln zu bilden, die den Produktaufbau generell verändern.
Für Isoliergläser kann die Ermittlung der technischen Werte über die Produktschlüssel gesteuert werden.

Sie haben Zugriff auf folgende Bereiche:

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a a a | Varianten - Farben | "Farbvarianten" auf Seite B-212 |
| a a b/c | Varianten -Farbbezeichnungen | ⇨ "Farbbezeichnungen" auf Seite B-214 |
| a b a | Maße- Maße | "Maßvarianten" auf Seite B-215 |
| a b b/c | Maße - Maßbezeichnungen | ⇨ "Maßbezeichnungen" auf Seite B-217 |
| a c a | Größen - Größenvarianten | ⇨ "Größenvarianten" auf Seite B-218 |
| a c b/c | Größen - Größenbezeichnungen | ⇨ “Größenbezeichnungen" auf Seite B-219 |
| b | Austausch-/Zusatzregeln | ⇨ "Austausch-/Zusatzregeln" auf Seite B-220 |
| c a | Technische Werte - Gruppen | ⇨ "Untermenü Technische Werte > Gruppen" auf Seite B-210 |
| c b | Technische Werte - Vektoren | ⇨ "Untermenü Technische Werte > Vektoren" auf Seite B-210 |
| c | Technische Werte - Notifizierungsstellen | ⇨ "Notifizierungsstellen" auf Seite B-246 |
| d | Technische Werte -Produktnormen | ⇨ "Produktnormen" auf Seite B-247 |
| e | Technische Werte -Prioritäten | ⇨ "Prioritäten" auf Seite B-249 |
| f | Technische Werte -Produktkennzeichnung | ⇨ "Produktkennzeichnung (CEKAL)" auf Seite B-250 |
| g | Technische Werte CE-Kennzeichen | ⇨ "CE-Kennzeichen (CPIP)" auf Seite B-252 |
| h | Technische Werte - Leistungserklärung | ⇨ "Leistungserklärung" auf Seite B-252 |
| i | Technische Werte -Produktverschlüsselung | ⇨ "Produktverschlüsselung" auf Seite B-254 |
| j | Technische Werte -Produktverwendungszwecke | ⇨ "Bezeichnungen für Produktverwendungszwecke" auf Seite B-257 |
| k | Technische Werte -Parameterbeschreibung | ⇨ "Parameterbeschreibung" auf Seite B-259 |
| l | Technische Werte -Leistungserklärung | ⇨ "Leistungserklärung (Erfassung)" auf Seite B-260 |
| d a/b | Analysegruppen | ⇨ "Bezeichnungen für Analysegruppen" auf Seite B-261 |
| e a/b/c | Beschlagstypen | ⇨ "Bezeichnungen für Beschlagstypen" auf Seite B-262 |
| f a/b | Folientypen | ⇨ "Bezeichnungen für Folientypen" auf Seite B-264 |
| g | Produktionstypen | ⇨ "Produktionstypen" auf Seite B-265 |
| h a/b/c | Rahmentypen | ⇨ "Bezeichnungen für Rahmentypen" auf Seite B-266 |
| i a/b | Versiegelungstypen | ⇨ "Bezeichnungen für Versiegelungstypen" auf Seite B-268 |
| j | Motive | ⇨ "Motivzuordnung" auf Seite B-269 |
| k | Stapel | Hierbei handelt es sich um eine kundenspezifische Funktion, die nicht Bestandteil des Handbuches ist. |
| l a/b | Kistensignatur | ⇨ "Bezeichnungen für Kistensignatur" auf Seite B-271 |
| m | Shaping/Nesting-Artikel | ⇨ "Shaping/Nesting-Artikel" auf Seite B-273 |
| n | Template Parameter | ⇨ "Template Parameter" auf Seite B-274 |
| o | ¡TOE - Austauschregeln | ⇨ "¡TOE-Austauschregeln" auf Seite B-275 |
| p | Bemaßungsset | Hierbei handelt es sich um eine kundenspezifische Funktion, die nicht Bestandteil des Handbuches ist. |
| q | Kundenprodukte | ⇨ “Kundenprodukte" auf Seite B-278 |
| r | Bestellte Bearbeitungen | ⇨ "Bestellte Bearbeitungen" auf Seite B-280 |
| s | Hausspezifische Angaben | ⇨ "Hausspezifische Angaben" auf Seite B-282 |
| t | VSG/GH Vererbung | ⇨ "VSG/GH Vererbung" auf Seite B-283 |
| u | A+W iQuote - spezifische Angaben | ⇨ "Untermenü A+W iQuote-spezifische Angaben" auf Seite B-211 |

### Untermenü Technische Werte > Gruppen
*Schlüssel > Produkte > Technische Werte > Gruppen*

Über dieses Menü legen Sie Gruppen, die für die Beschreibung der technischen Werte notwendig sind, fest.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Schalldämmung | ⇨ "dB-Gruppen" auf Seite B-228 |
| b | Thermische Eigenschaften | ⇨ "U-Gruppen" auf Seite B-229 |
| c | Gesamtenergiedurchlass | ⇨ "g-Gruppen" auf Seite B-230 |
| d | Transmission | ⇨ "Transmissionsgruppen" auf Seite B-231 |
| e | Maßrestriktionen | ⇨ "Maßrestriktions-Gruppen" auf Seite B-232 |
| f | Dicken | ⇨ "Dickengruppen" auf Seite B-233 |
| g | Biegefestigkeit) | ⇨ "Biegefestigkeitsgruppen" auf Seite B-234 |

### Untermenü Technische Werte > Vektoren
*Schlüssel > Produkte > Technische Werte > Vektoren*

Über dieses Menü legen Sie Vektoren, die für die Beschreibung der technischen Werte notwendig sind, fest.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Schalldämmung | ⇨ "Vektoren für Schalldämmung (dB)" auf Seite B-235 |
| b | Thermische Eigenschaften | ⇨ "Vektoren für thermische Eigenschaften (U)" auf Seite B-237 |
| c | Gesamtenergiedurchlass | ⇨ "Vektoren für Gesamtenergiedurchlass (g)" auf Seite B-239 |
| d | Transmission | ⇨ "Vektoren für Transmission" auf Seite B-241 |
| e | Maßrestriktionen | ⇨ "Vektoren für Maßrestriktionen" auf Seite B-243 |
| f | Windlast | ⇨ "Vektoren für Windlast" auf Seite B-245 |

### Untermenü A+W iQuote-spezifische Angaben
*Schlüssel > Produkte > A+W iQuote-spezifische Angaben*

Über dieses Menü pflegen Sie Stammdaten, die für das Arbeiten mit A+W iQuote notwendig sind. Wenn Sie Information über dieses Produkt brauchen, kontaktieren Sie bitte einen Mitarbeiter der A+W Software GmbH.

| Short Cut | Eintrag | Beschreibung |
| :--- | :--- | :--- |
| a | Artikelgruppen | ⇨ "Artikelgruppen-Bezeichnungen" auf Seite B-284 |
| b | Bearbeitungszuordnung | ⇨ "Bearbeitungszuordnung" auf Seite B-285 |
| c | Bearbeitung für Modellkanten | ⇨ "Bearbeitungen für Modellkanten" auf Seite B-288 |
| d | Austauschgruppen | ⇨ "Austauschgruppen-Bezeichnungen" auf Seite B-290 |
| d c | Gruppenzuordnung (Artikel) | ⇨ "Gruppenzuordnung (Artikel)" auf Seite B-291 |
| d d | Gruppenzuordnung (Rahmen) | ⇨ "Gruppenzuordnung (Rahmen)" auf Seite B-292 |

### Farbvarianten
*Stammdaten > Schlüssel > Produkte > Varianten > Farben > Farben*

Alle Farben, die im Artikelstamm und später in der Auftragserfassung benötigt werden, müssen hier angelegt werden.

#### Erläuterung der Felder
**Nummer**
Nummer der Farbe.
*Technische Info: Numerisches Feld, DB-Feld: xxfarbe.farbnr*

**Bezeichnung**
Bezeichnung der Farbe.
*Technische Info: Alphanumerisches Feld, DB-Feld: xcompany.name*

**RAL-Nummer**
RAL-Nummer der Farbe.
*Technische Info: Numerisches Feld, DB-Feld: xxfarbe.ralnr*

**AWDesign-Farbcode**
A+W Farbcode, der im CAD Designer (Bars) benötigt wird.
*Technische Info: Alphanumerisches Feld, DB-Feld: xxfarbe.awfarbcode*

**RGB-Bezeichnung**
RGB-Farbname.
*Technische Info: Alphanumerisches Feld, DB-Feld: xxfarbe.rgbname*

**Rot**
Anteil Rot für RGB-Farbdefinition.
*Technische Info: Numerisches Feld, DB-Feld: xxfarbe.farbe_r*

**Grün**
Anteil Grün für RGB-Farbdefinition.
*Technische Info: Numerisches Feld, DB-Feld: xxfarbe.farbe_g*

**Blau**
Anteil Blau für RGB-Farbdefinition.
*Technische Info: Numerisches Feld, DB-Feld: xxfarbe.farbe_b*

**Ergänzende Informationen**
⇨ "Farbbezeichnungen" auf Seite B-214

### Farbbezeichnungen
- Stammdaten > Schlüssel > Produkte > Varianten > Farben > Einzelne Bezeichnung
- Stammdaten > Schlüssel > Produkte > Varianten > Farben > Alle Bezeichnung

In diesem Dialog definieren Sie die einzelnen Farben in den verschiedenen Sprachen.

#### Erläuterung der Felder
**Nummer**
Schlüssel-Nummer. Zum Anlegen einer neuen Farbe geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Farbbezeichnung, z. B. weiß.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1*

### Maßvarianten
*Stammdaten > Schlüssel > Produkte > Varianten > Maße > Maße*

In diesem Dialog werden alle Maßvarianten, abhängig von der Mengeneinheit gepflegt. Im Artikelstamm werden dann diese Maßvarianten zugeordnet. Die Maßvarianten sind auch Grundlage für die Lagerwirtschaft.

#### Erläuterung der Felder
**Nr**
Die Varianten-Nr ist der eindeutige Schlüssel innerhalb der jeweiligen Mengeneinheit (ME). Sie wird sowohl im Artikelstamm als auch im Rahmen der Auftragserfassung zur Identifikation der gewünschten Variante genutzt.
*Technische Info: Numerisches Feld, DB-Feld: xxvar.bitnr*

**ME**
Auswahl der Mengeneinheit. Die Schlüssel werden im Menü Mengeneinheiten (Schlüssel > System) hinterlegt.
*Technische Info: `<Selo>-Feld, DB-Feld: xxvar.meh*

**Bezeichnung**
Bezeichnung der Maßvariante kann frei gewählt werden.
*Technische Info: Alphanumerisches Feld*

**Lagerbez.**
Bezeichnung eines Stückes im Lager kann frei gewählt werden.
*Technische Info: Alphanumerisches Feld*

**Teilmaße 1-3**
Länge, Breite und Höhe werden in der jeweils kleinsten sinnvollen Einheit angegeben. Sie werden bei der Auftragserfassung automatisch eingeblendet.
*Technische Info: Numerisches Feld, DB-Feld: xxvar.mas1, mas2, mas3*

**Gesamtmaß**
Das Gesamtmaß gibt die Gesamtgröße der Variante in der jeweiligen Systemgrundeinheit an. In der Auftragserfassung wird das Gesamtmaß gemäß des hier eingetragenen Umrechnungsfaktors berechnet.
*Technische Info: Numerisches Feld, DB-Feld: xxvar.faktor*

**Ergänzende Informationen**
⇨ "Mengeneinheitenbezeichnung" auf Seite B-163

### Maßbezeichnungen
- Stammdaten > Schlüssel > Produkte > Varianten > Maße > Einzelne Bezeichnung
- Stammdaten > Schlüssel > Produkte > Varianten > Maße > Alle Bezeichnung

In diesem Dialog definieren Sie die einzelnen Maßvarianten in den verschiedenen Sprachen.

#### Erläuterung der Felder
**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Mengeneinheit geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id, view: xxvar.bitnr*

**ME**
Auswahl der Mengeneinheit. Die Schlüssel werden im Menü Mengeneinheiten (Schlüssel > System) hinterlegt.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id2*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Variantentext**
Bezeichnung der Variante.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1*

**Lagerbez.**
Bezeichnung eines Stückes im Lager.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez2*

**Ergänzende Informationen**
⇨ "Mengeneinheitenbezeichnung" auf Seite B-163

### Größenvarianten
*Stammdaten > Schlüssel > Produkte > Varianten > Größen > Größenvarianten*

In diesem Dialog definieren Sie die einzelnen Größenvarianten.

#### Erläuterung der Felder
**Nr**
Auswahl der Dicke-/Größenvariante im ISO. Zum Anlegen einer neuen Dickenvariante geben Sie die nächste freie Nummer ein.
*Technische Info: Numerisches Feld, DB-Feld: xxdicke.dicke*

**Bezeichnung**
Bezeichnung, z. B. 12 mm
*Technische Info: Alphanumerisches Feld*

**Dicke**
Dicke der Variante in der festgelegten Mengeneinheit.
*Technische Info: Numerisches Feld, DB-Feld: xxdicke.dickenmass*

**Ergänzende Informationen**
⇨ "Größenbezeichnungen" auf Seite B-219

### Größenbezeichnungen
- Stammdaten > Schlüssel > Produkte > Varianten > Größen > Einzelne Bezeichnung
- Stammdaten > Schlüssel > Produkte > Varianten > Größen > Alle Bezeichnung

In diesem Dialog definieren Sie die einzelnen Größenbezeichnungen in den verschiedenen Sprachen.

#### Erläuterung der Felder
**Nummer/Nr**
Schlüssel-Nummer. Zum Anlegen einer neuen Qualität geben Sie die nächste freie Nummer ein.
*Technische Info: `<F9>`, DB-Feld: xsprbez.id, view: xxvar.bitnr*

**Spr**
Sprachkennzeichen.
*Technische Info: `<F9>`, DB-Feld: xsprbez.sprkz*

**Bezeichnung**
Bezeichnung der Größe, z. B. 2 mm.
*Technische Info: Alphanumerisches Feld, DB-Feld: xsprbez.bez1, view: xxvar.atxt*

**Ergänzende Informationen**
⇨ "Größenbezeichnungen" auf Seite B-219

### Austausch-/Zusatzregeln
*Stammdaten > Schlüssel > Produkte > Austausch-/Zusatzregeln*

Der Menüpunkt Austausch-/Zusatzregel ermöglicht es, kundenspezifische Regeln, nach denen im Auftrag die Stückliste ergänzt bzw. Teile ausgetauscht werden sollen, für einzelne Artikel oder Artikeltypen zu hinterlegen. Dabei wird auf der linken Dialogseite der Artikel bzw. der Artikeltyp ausgewählt, für den die auf der rechten Dialogseite festgelegte Regel gilt.

Der Dialog besteht aus den Registern:
- Austausch-/Zusatzregeln
- Details
- Testmodus

#### Erläuterung der Felder im Bereich Es gilt für ...
**Knd-Artnr**
Wenn das Feld Kunden-Artikelnummer gefüllt ist, wird die Regel bei der Erfassung nur dann ausgewertet, wenn die Erfassung der Position über den Kundenartikel erfolgt. Auch dann, wenn zufällig für den A+W Enterprise-Artikel und Kunden eine eindeutige Zuordnung besteht.
*Technische Info: `<F9>`, DB-Feld: kuaz.kuartnr*

**ProdTyp**
Das Feld wird mit dem Artikeltyp vom Kopfartikel gefüllt. Das Feld muss nicht zwingend ausgefüllt werden, sondern nur, wenn die Regel spezifisch für den Artikeltyp anzuwenden ist.
*Technische Info: `<F9>`, DB-Feld: kuaz.prodtyp*

**Produkt**
Das Feld wird mit dem Kopfartikel gefüllt. Es muss nicht zwingend ausgefüllt werden, sondern nur, wenn die Regel spezifisch für den Artikel anzuwenden ist.
*Technische Info: `<F9>`, DB-Feld: kuaz.prodnr*

**1x**
Über die Checkbox steuern Sie, ob die Regel nur einmal oder immer angewendet wird.
- `☐` Die Regel wird nur einmal im Produkt ausgeführt. Dadurch können Sie ermöglichen, dass im ISO ein Float z. B. 110005 gegen ein bearbeitetes Float 150005 getauscht wird, auch wenn dieses bearbeitete Float selbst in der Stückliste den Artikel 110005 hat. Anschließend werden keine Austauschregeln angewendet.
- `☑` Die Regel wird immer angewendet.
*Technische Info: Toggle-Feld, DB-Feld: kuaz.einmal*

**Atyp**
Das Feld Artikeltyp ist ein Alternativ-Feld, das, welches Teil ausgetaus