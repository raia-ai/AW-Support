---
title: "EN-CONFIG-AW_Enterprise_1"
source: "EN-CONFIG-AW_Enterprise_1.pdf"
tags: ["A+W Enterprise", "Configuration", "Software for Glass", "EDI", "BOM", "Article Master Data", "iQuote", "ERP", "Technical Manual", "System Setup"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides detailed configuration instructions for the A+W Enterprise software, a comprehensive solution for the glass industry. It covers key concepts, article master data setup, exchange/additional rules, and various system modules."
long_description: "This is a comprehensive configuration manual for the A+W Enterprise software system, designed for internal use. The document details the setup and configuration of various modules and functionalities within the A+W ecosystem, which is a leading software solution for the glass processing industry. It begins with a change history, tracking updates from 2018 to 2025. The core of the manual is a detailed table of contents followed by in-depth chapters on system keys (languages, product keys), article master data (article types, bill of materials, IG units, spacers), and the application of exchange and additional rules (E/A rules). It explains how to configure elements like IG units, spacers, sealants, and muntins, and discusses the differences between fixed products and product sets. The guide also covers article dimensioning, stock management, supplier allocation, and the use of private fields and article remarks. This manual is essential for system administrators and technical consultants responsible for implementing and maintaining the A+W Enterprise system, ensuring correct data flow and process automation from order entry to production."
---

# A+W Configuration Instructions
---
## A+W Enterprise

**english**

**- -INTERNAL-**
**A+W - Software for Glass**

## Change history

| Date | Author | Comments | Version |
| :--- | :--- | :--- | :--- |
| 2018-02-20 | Anja Grünbacher | New layout | 1.0 |
| 2018-03-23 | Ralf Imhof | Route optimization | 1.1 |
| 2018-05-11 | Alexander Weil | ICE environment; A+W iQuote | 1.2 |
| 2018-06-25 | Alexander Weil | A+W iQuote | 1.3 |
| 2018-09-21 | Alexander Weil | A+W iQuote extension | 1.4 |
| 01/11/2018 | Ina Seifert | Postponement of delivery date/delivery date calculation | 1.5 |
| 2018-11-10 | Elena Tempelfeld | Discount logic / LG | 1.6 |
| 2018-12-20 | Elena Tempelfeld | Product groups | 1.7 |
| 2019-01-28 | Alexander Weil | ICE environment | 1.8 |
| 2019-02-06 | Silvia Höpp | SNLive, SNLive-Zoom, evaluation print-KZ, DXF import | 1.9 |
| 2019-03-08 | Elena Tempelfeld | Travel time per MP/address/route | 2.0 |
| 2019-03-15 | Ina Seifert | Field recording, Stock removal booking of stock dimensions, Size variants in stock | 2.1 |
| 2019-03-22 | Rainer Schepp | Release of locks on the No server | 2.2 |
| 2019-05-14 | Ina Seifert | Various points on the topic "stock" | 2.3 |
| 2019-07-16 | Elena Tempelfeld | Sash size sets, product sets | 2.4 |
| 2019-10-21 | Elena Tempelfeld | Chapter 17.4.4 Inheritable LAMI processings/reworking of product set chapter started | |
| 2019-11-28 | Ina Seifert | Cost Calculation | |
| 2019-12-13 | Elena Tempelfeld | Cost center logic | |
| 2020-01-13 | Elena Tempelfeld | Rack-related incoming goods | |
| 2020-01-27 | Elena Tempelfeld | Sash size sets, product sets | |
| 2020-02-18 | Elena Tempelfeld | Inheritance documents taken over | |
| 2020-02-28 | Elena Tempelfeld | Text supplements, Thiokol, spacers in stock | |
| 2020-03-09 | André Münch | ICE 3.7 Installation (Chapter 7.1) | |
| 2020-03-23 | Ina seifert | Reference tool | |
| 2020-06-17 | Anja Grünbacher | VAT adjustment | |
| 2020-09-01 | Ina Seifert | Pattern/test production procedure | |
| 2020-09-09 | Elena Tempelfeld | Rack booking (#459099) inserted and formatted. Author: Erika Wettstein | |
| 2020-10-30 | Ina Seifert | A+W CAD Designer (Bars) connection | |
| 2020-11-17 | Ina Seifert | Exchange rate for reference, E/A rules for internal EDI, Addresses for reference, Delivery date change log | |
| 2020-11-24 | Ina Seifert | Update "Rack-related shipping" | |
| 2020-12-08 | André Münch | Finding of the A+W service locator | |
| 2021-01-18 | Elena Tempelfeld | Intrastat (docu takeovers) | |
| 2021-01-29 | Ina Seifert | Order pool breakage | |
| 2021-04-08 | André Münch | Chapter 55: SmartCompanion | |
| 2021-05-19 | SVH | NVE logic | |
| 2021-06-23 | SVH | Background iTOE | |
| 2021-07-14 | Ina Seifert | Cancellation rights | |
| 2021-10-05 | Elena Tempelfeld | Autom. text creation -> Extended config. texts, "Intrastat" update | |
| 2021-11-16 | SVH | #448841 | |
| 2021-11-17 | Elena Tempelfeld | SQL queries with Excel transfer, Figure labeling added | |
| 2021-12-13 | Elena Tempelfeld | Intrastat shifted | |
| 2022-02-10 | Elena Tempelfeld | Reference to Intrastat document added | |
| 2022-02-10 | SVH | Receipt of goods/check, reference to extra document | |
| 2022-05-06 | Elena Tempelfeld | [AW-119029] – Selection of files via "Open file" dialog | |
| 2022-09-21 | SVH | Discount updated/Document change | |
| 2022-11-15 | IS | [AW-128380] – special characters in the file name for selection of files via "File open" dialog | |
| 21-11-2022 | SVH | Dynamic SR | |
| 2022-12-07 | IS | Receipt of goods | |
| 2023-04-03 | IS | Dispatch notification | |
| 2023-09-14 | IS | Delivery fee | |
| 2024-02-01 | IS | wlgetbitnr | |
| 2024-08-29 | SVH | [AW-111997] – "Electronic invoices" section | |
| 2024-11-14 | SVH | MODUL_ABKLEBEN | |
| 2025-06-06 | IS | | |

## Content

1.  **Schlüssel** 20
    1.1. Sprachen 20
        1.1.1.1. Sprachcode 20
    1.2. Produktschlüssel 20
        1.2.1.1. Maßvarianten 20
    1.3. Formelelemente 21
        1.3.1.1. Variablen 21
        1.3.1.2. Operatoren 22
2.  **Artikelstammdaten** 24
    2.1. Artikeltypen 24
        2.1.1.1. Übersicht 24
    2.2. Artikelart 25
    2.3. Stückliste 25
    2.4. ISO 26
        2.4.1.1. 4-fach-ISO (Erweiterung) 27
    2.5. Rahmen 27
        2.5.1.1. Abmessungen bei Bestellungen 28
        2.5.1.2. SZR in Rahmenbestellungen 28
        2.5.1.3. Montagerahmen 28
    2.1. Rahmentyp 29
    2.2. Dynamischer AHAM 30
    2.3. Versiegelungstyp 33
    2.4. Folientyp 33
    2.5. Beschlagstyp 34
    2.6. Sprossen 34
        2.6.1.1. Sprossentyp 34
    2.7. Fixierte Produkte vs. Produktsets 37
    2.8. Artikelvermaßung 38
        2.8.1.1. Restriktionsformel 38
    2.9. Bestandsänderung 40
    2.10. Produktionszeit / Wiederbeschaffungszeit (Fehler! Textmarke nicht definiert.)
    2.11. Lieferantenzuordnung 41
    2.12. Spezielle Konfigurierbare Felder 41
    2.13. Feste private Felder 42
    2.14. Artikelanmerkungen 42
3.  **Austausch-/Zusatzregeln** 43
    3.1. Register Austausch-/Zusatzregeln 43
        3.1.1.1. Linke Dialog-Seite 43
        3.1.1.2. Rechte Dialog-Seite 45
        3.1.1.3. Register Details 46
        3.1.1.4. Löschen über A/Z/D-Regel 47
    3.1.1.5. Übergabe der Maßparameter 48
    3.1.1.6. Möglichkeiten für Preissteuerung 49
    3.1.1.7. Austausch gegen sich selbst 49
    3.1.1.8. Auftragsänderung 49
    3.1.1.9. Interne DFÜ 50
    3.1.1.10. Austausch des Positionsartikels 50
    3.1.1.11. Austausch eines einfachen Elementes in der Stückliste 50
    3.1.1.12. Austausch der Bearbeitungsparameter 50
    3.1.1.13. Zusatzelement für den Positionsartikel/Produkttyp 51
    3.1.1.14. Beschaffungsart alcib - 13.04.10373 51
    3.1.1.15. Übergabe der Artikelbezeichnung 51
    3.1.1.16. Externe DFÜ 51
4.  **Artikelsuche** 52
5.  **Versandregion / Routen** 53
6.  **Marktpartnerstammdaten** 56
    6.1. Stornierte Marktpartner 56
    6.2. Adressen 56
        6.2.1.1. Niederländische Adresslogik 56
        6.2.1.2. Stornieren von Adressen 57
    6.3. Routen 58
    6.4. Abteilung 58
    6.5. E-Mail 58
    6.6. Typ der DFÜ 58
    6.7. Feste private Felder 59
    6.8. Umgebungsvariablen 59
7.  **Vorgangsarten** 60
8.  **Versiegelungstiefe** 61
    8.1. Motivation und Ziele dieser Entwicklung 61
    8.2. Zentrale Begriffe 61
    8.3. Einschränkungen, Abgrenzung, Gültigkeit 61
    8.4. Installation/Konfiguration, Umgebungsvariablen 62
    8.5. Funktionsbeschreibung 62
        8.5.1.1. Stammdaten 62
        8.5.1.2. Erfassung der Versiegelungstiefe 64
        8.5.1.3. Änderung des Abstandhalterabzugsmaßes 65
        8.5.1.4. Berechnung des neuen Abstandhalterabzugsmaßes 65
        8.5.1.5. Änderung der Versiegelungstiefe 66
        8.5.1.6. Sprossenberechnung 66
        8.5.1.7. Vertextung 66
        8.5.1.8. Auswirkung auf die OrderXML-Schnittstelle und den direkten Datenimport nach ALCIM 67
9.  **ITOE** 68
    9.1. Motivation und Ziele dieser Entwicklung 68
    9.2. Einschränkungen, Abgrenzung, Gültigkeit 68
    9.3. Installation/Konfiguration, Umgebungsvariablen 68
10. **Hintergrund-iTOE** 69
11. **Bearbeitungstypen mit spezieller Unterstützung durch den A+W CAD Designer (Shapes)** 70
    11.1. Bearbeitungen mit SN-Makros-Dateien 70
        11.1.1.1. Stammdaten 70
        11.1.1.2. Vorgangserfassung 71
        11.1.1.3. Generierung von Bestellungen 71
        11.1.1.4. Schnittstelle zu und von A+W Production 72
    11.2. Parametrische Makros 75
        11.2.1.1. Artikelstamm 75
        11.2.1.2. Auftragserfassung 76
        11.2.1.3. Interne Vorgangsübertragung 76
        11.2.1.4. Artikel-Stammdatenreplikation 76
    11.3. Bearbeitungen mit Motiv-Dateien 76
        11.3.1.1. Stammdaten 76
        11.3.1.2. Erfassung von skalierbaren Motiven bei Oberflächenbearbeitungen 78
        11.3.1.3. Interne Übertragung 79
        11.3.1.4. Artikelstammdaten-Replikation 79
        11.3.1.5. Schnittstelle zu und von A+W Production 79
        11.3.1.6. Konfigurationsmöglichkeiten im A+W CAD Designer (Shapes) 80
12. **Mitarbeiterstamm** 82
    12.1. Stornoberechtigungen 82
        12.1.1.1. Stornierung von Positionen und in lokaler Korrektur 82
        12.1.1.2. Versand 84
    12.2. Mitarbeiteranmerkungen 85
    12.3. Abteilung 85
13. **Bonus** 86
    13.1. Umgebungsvariablen 86
14. **Rabattlogik 2005** 87
    14.1. Motivation und Ziele dieser Entwicklung 87
    14.2. Zentrale Begriffe 87
    14.3. Einschränkungen, Abgrenzung, Gültigkeit 87
        14.3.1.1. Auftragskopplung 87
        14.3.1.2. Bestellübertragung 87
        14.3.1.3. Replikation 88
    14.4. Umgebungsvariablen 88
    14.5. Funktionsbeschreibung 92
        14.5.1.1. Aufbau der Rabattlogik 92
        14.5.1.2. Funktionale Beschreibung 92
        14.5.1.3. Stammdaten 94
        14.5.1.4. Rabattkriterium 97
        14.5.1.5. Rabattarten / Rabattwert 98
        14.5.1.6. Gewicht 99
        14.5.1.7. Rabatte im Vorgang 100
        14.5.1.8. Automatischer Kostensatz für Verpackungen 103
        14.5.1.9. Rabattinformationen auf der Positionsebene 103
        14.5.1.10. Tabellen und Felder 105
        14.5.1.11. Spezielle Funktionen 112
15. **Kleinlieferzuschlag / Anlieferpauschale** 114
    15.1. Datenstrukturen 114
    15.2. Stored Procedure 114
    15.3. Maskenlogik 115
    15.4. Ermittlung des Zuschlags 116
    15.5. Automatische Abarbeitung der offenen Rechnungen 116
    15.6. Umgebungsvariablen 116
    15.7. Installationsanleitung 117
16. **Konfiguration der ICE-Umgebung** 118
17. **Vorgangssuche** 119
18. **Erfassung mit Bezugnahme** 120
    18.1. Konfigurierte Bezugnahme 120
    18.2. Übernahme einzelner Positionen 124
    18.3. Adressen 125
    18.4. Aufträge mit Fremdwährung 126
        18.4.1.1. RECH_KURS_NEU 126
        18.4.1.2. BEZUG_KURS_NEU 127
        18.4.1.3. UMRECHNUNGSKURS_BEI_BEZUG 127
        18.4.1.4. WKURS_NEU 127
        18.4.1.5. Übersicht 128
    18.5. Zahlungsmodalitäten/Merkmale 130
    18.6. Vorgangsanmerkungen 130
        18.6.1.1. Übernahme von Vorgangsanmerkungen 130
        18.6.1.2. Kennzeichnung der Referenzaufträge von Reklamationsaufträgen 131
        18.6.1.3. Anmerkung bei Bezugnahme auf Angebote 131
    18.7. Mandantenzuordnung bei Interner Mandantentrennung 131
    18.8. Beschaffungsarten 132
    18.9. Umgebungsvariablen 132
19. **Gutschriftserfassung** 134
    19.1. Positionen Drucken 134
    19.1. Formulardruck 134
20. **Rechnungserzeugung** 135
    20.1. Änderungsprotokoll 135
    20.2. FIBU-Debitor 135
    20.3. Gruppierungskriterien für Sammelrechnungen 135
    20.4. Zahlungsplan (Abschlags- und Schlussrechnungen) 137
        20.4.1.1. Stammdaten 137
        20.4.1.2. Zahlungsplan 138
        20.4.1.3. Abschlagsrechnung 138
        20.4.1.4. Schlussrechnung 140
        20.4.1.5. Konfiguration 141
    20.5. Werteimport 143
    20.6. Formulardruck 143
    20.7. Einkaufsrechnungen für Ersatzbestellungen 143
    20.8. Elektronische Rechnungen 144
    20.9. Umgebungsvariablen 144
21. **Automatismen in der Auftragserfassung** 146
    21.1. Erfassungshilfe 146
    21.1.1.1. Emaillestreifen 146
    21.1.1.2. Stammdaten 146
    21.1.1.3. Erfassung 147
    21.1.1.4. Stufen-ISO 147
    21.1.1.5. Unterschiedlichen Rahmeneinstände 148
    21.1.1.6. Vertextung 148
    21.1.1.7. Interne Bestell-Übertragung 148
    21.1.1.8. Randentschichten 149
    21.1.1.9. Stammdaten 149
    21.1.1.10. Erfassung 149
    21.1.1.11. Stufen-ISO 150
    21.1.1.12. Unterschiedliche Rahmeneinstände 150
    21.1.1.13. Vertextung 150
    21.1.1.14. Interne Bestell-Übertragung 151
    21.1.1.15. Abkleben 151
    21.1.1.16. Stammdaten 151
    21.1.1.17. Erfassung 152
    21.1.1.18. Stufen-ISO 153
    21.1.1.19. Unterschiedlicher Randverbund 154
    21.1.1.20. Vertextung 154
    21.1.1.21. Interne Übertragung 154
    21.2. Änderung der Beschaffungsart 154
        21.2.1.1. Rahmenbeschaffung wie Sprossen 154
        21.2.1.2. Sprossenlieferant für den Innenrahmen 155
        21.2.1.3. Umstellung auf Bestellung bei der Verletzung der Maßrestriktionen 156
    21.3. Lageraufträge 156
        21.3.1.1. Manuelle Erfassung 156
    21.4. Vorgangssicherung 156
    21.5. Versandart vs. Route 158
        21.5.1.1. Automatische Änderung der Versandart bei Routenänderung (Versandart - Route) 158
        21.5.1.2. Automatische Änderung der Versandart bei Routenänderung (Route - Versandart) 158
        21.5.1. Doppelseitige Änderung von Route und Versandart 159
        21.5.1.1. Konfiguration 160
22. **Produktaustausch** 161
    22.1. Austausch der Stücklistenelemente bei ISO und VSG 161
    22.2. Austausch von SZR bei ISO-Austausch 162
    22.3. Produktaustausch bei ESG 162
    22.4. Zusatzbearbeitungen in der vorhandenen Stückliste 163
    22.5. Erweiterter Produktaustausch 164
23. **Erfassung mit Innenansicht** 166
24. **Stückliste in der Vorgangserfassung** 167
    24.1. Mehrere Bearbeitungen zwischen Stücklistenebenen auf einmal kopieren 167
    24.2. Beschaffungsart „* vor DFÜ“ 168
    24.3. Umgebungsvariablen 168
25. **Vorgangsanmerkungen** 169
    25.1. Menüpunkt „Auftragsinformation" 169
26. **Bestellpool (Bestpool)** 170
    26.1. Zugang 170
    26.2. Gruppierung 170
    26.3. Bruch 170
    26.4. Liefertermin 171
    26.5. Einkaufsinformation / Restriktionsanzeige 171
    26.6. Bestellungen für Packmittel (Kisten) 172
    26.7. Umgebungsvariablen 172
27. **Bestellverwaltung / Bestellerfassung** 173
    27.1. Warnmeldung bei Änderung in Bestellungen mit Auftragsbezug 173
28. **Lieferavis** 174
    28.1. Meldung bei Bestellterminverschiebung 174
29. **Fertigwarenlager** 177
    29.1. Konfiguration 177
    29.2. Versandsteuerung 178
        29.2.1.1. Lieferschein 178
        29.2.1.2. Verpacktmeldung 178
        29.2.1.3. Inventur Fertigwarenlager 179
    29.3. Wareneingangserfassung 179
        29.3.1.1. Manueller Wareneingangserzeugung /-storno 180
    29.4. Lagerabgangsbuchungen 180
30. **Lager** 181
    30.1. Artikelstammdaten 181
        30.1.1.1. Varianten 181
    30.2. Raum-Stammdaten 181
        30.2.1.1. Kistenlager 182
        30.2.1.2. Fachlager 182
    30.3. Lagereingangsbuchung 182
    30.4. Lagerinventur 182
    30.5. Lagerbewertung 183
        30.5.1.1. Durchschnittspreis 183
        30.5.1.2. FIFO und LIFO Werte 183
        30.5.1.3. Rückdatierung einer Lagerbewertung 184
    30.6. Korrektur von Lagerbuchungen 184
        30.6.1.1. WL_KORR_DURCH_GEGENBUCH 184
        30.6.1.2. Standartverfahren 185
    30.7. Lagerfüllaufträge 186
        30.7.1.1. Lagerzugangsbuchung bei Verpacktmeldung 186
        30.7.1.2. Manuelle Erfassung 186
    30.8. Rückmeldung von Lagerplatten 187
        30.8.1.1. Motivation dieser Funktionsbeschreibung 187
        30.8.1.2. Konfiguration 187
        30.8.1.3. Auflösen von Reservierungen (#289178) 188
    30.9. Größenvvarianten auf Lager 188
        30.9.1.1. Motivation dieser Funktionsbeschreibung 188
        30.9.1.2. Artikelstammdaten 188
        30.9.1.3. Lager-Artikelstammdaten 190
    30.10. Auslösen von Bestellvorschlägen 191
    30.10.1.1. Voraussetzungen 191
    30.10.1.2. Bestellmengenverfahren 191
    30.10.1.3. Standardmenge (WLBMV=1) 192
    30.10.1.4. Abgebuchte Menge (WLBMV=2) 192
    30.10.1.5. Bis Maximalbestand (WLBMV=3) 192
    30.10.1.6. Einmal bis Maximalbestand (WLBMV=4) 192
    30.10.1.7. Ν* Standardmenge bis zum Maximalbestand (WLBMV=5) 192
    30.10.1.8. Bestellprognose ohne Alarmbestand 193
    30.10.1.9. Variantengenaue Bestellprognose: 193
    30.10.1.10. Bestellprognose für fixierte Artikel 194
    30.10.1.11. Bestellprognose für Farb- oder Dickenvarianten mit Bestandsänderung AWP 194
    30.10.1.12. Umgebungsvariablen 195
    30.11. Abstandhalter/Thiokol im Lager 195
        30.11.1.1. Abstandhalter 195
        30.11.1.2. Trockenmittel 199
    30.12. Bestandsprüfung beim Import/Einlastung 203
    30.13. Ermittlung der Variantennummer 203
    30.14. Umgebung / Problemlösungen 204
31. **Routenoptimierung** 206
    31.1. Infrastruktur 206
    31.2. Voraussetzung 206
    31.3. ICE-Umgebung 206
        31.3.1.1. Unix 206
        31.3.1.2. Windows 206
    31.4. A+W Enterprise 207
        31.4.1.1. Schalter 207
        31.4.1.2. Stammdaten 207
        31.4.1.3. Tracing 207
        31.4.1.4. Datenbank 207
        31.4.1.5. Übertragung von Gestellinformationen 208
        31.4.1.6. Gestellausgang und Gestelleingang 208
        31.4.1.7. Packmittelmaße 208
    31.5. A+W Logistics Optimizer 209
        31.5.1.1. Datenbank 209
        31.5.1.2. A+W Produkte 210
        31.5.1.3. Installationspfad Application 210
32. **A+W iQuote** 211
    32.1. A+W iQuote Auftragsmerkmale in A+W Enterprise 211
33. **Feldprotokollierung** 212
    33.1. Verfügbare Dialoge 212
    33.2. Konfiguration 214
    33.3. Auswertung 214
34. **Feste private Felder in der Vorgangserfassung** 215
35. **Liefertermin** 216
    35.1. Konfigurationsmöglichkeiten in A+W Enterprise: 216
    35.2. Lieferterminverschiebung mit AWP 216
        35.2.1.1. Motivation dieser Funktionsbeschreibung 216
    35.2.1.2. Konfigurationsmöglichkeiten in A+W Production: 217
    35.2.1.3. A+W Enterprise: Auftragserfassung 218
    35.2.1.4. Lieferterminverschiebung durch A+W Produktion 219
    35.2.1.5. Auftragsumlastung in A+W Production 219
    35.2.1.6. Konfigurationsmöglichkeit in A+W Production 221
    35.2.1.7. A+W Enterprise: Versandsteuerung 221
    35.2.1.8. Liefertermin zurück in den Auftrag 223
    35.2.1.9. A+W Enterprise: Liefertermin pro Position-verschiedene Bestellungen 224
    35.2.1.10. A+W Production: Liefertermin pro Position 225
    35.3. Via plant 228
    35.4. Packmitteloptimierung 228
        35.4.1.1. Logische Gestelle (Produktionsgestelle): 228
        35.4.1.2. Physikalische Gestelle (Versandgestelle): 228
    35.5. Einfluss der MP-Fahrtdauer 228
        35.5.1.1. Fahrtdauer des Kunden 228
        35.5.1.2. Fahrtdauer des Lieferanten 229
        35.5.1.3. Fahrtdauer des Objektes 230
    35.6. Fahrtzeit in der Adresse 231
    35.7. Routen-Fahrtzeit 231
36. **Lieferterminänderungsprotokoll** 233
37. **VSG** 237
    37.1. VSG-Lagermaß 237
    37.2. VSG-Festmaßartikel 239
    37.3. Erfassung von VSG-Artikeln im Auftrag 240
        37.3.1.1. VSG-Paketbearbeitungen 240
        37.3.1.2. VSGs mit Bearbeitungen an Einzelscheiben 242
    37.4. Vererbte Bearbeitungen 243
        37.4.1.1. Zusatzinformation (21.05.2019) 245
        37.4.1.2. Beispiele einer Vererbung nach unten 246
        37.4.1.3. Kundenspezifische Logik Vererbung mit Druckkennzeichen 247
        37.4.1.4. Vererbte Bearbeitung in der internen DFÜ 249
        37.4.1.5. Bearbeitungen mit Beschaffungsart "Keine" 250
        37.4.1.6. Vererbbare VSG Bearbeitungen 250
        37.4.1.7. Umgebungsvariablen 251
    37.5. Definition der iTOE-Regeln für Vererbung nach oben 252
        37.5.1.1. Teil 1 - Für normal Bearbeitung wie Kantenbearbeitung, normal Bohrung und Ausschnitte 252
        37.5.1.2. Teil 2 - Für Stufenbohrung 257
        37.5.1.3. Teil 3 - Für Senkbohrung 263
38. **Limitprüfung** 270
    38.1.1.1. Protokoll 270
    38.2. Markpartnerstammdaten 271
    38.3. Prüfung inclusive Wechselobligo 271
    38.4. Individuelle Prüfung (Stored Procedure) 271
    38.5. Umgebungsvariablen 272
39. **Auftragsfreischaltung** 273
    39.1. Steuerung der Freischaltung per Stored procedure 273
40. **Freischaltepool** 274
    40.1. Konfiguration 275
    40.2. Freischaltbemerkung 276
    40.3. Wie kommt ein Auftrag in den Freischaltepool und was ist dort zu sehen (nicht vollständig) 277
41. **Vorgangsänderung** 280
    41.1. Aktualisieren der Rabatte 280
    41.2. Erneute Kostenkalkulation von Aufträgen 280
42. **Gewichtsberechnung** 281
    42.1. Artikelstamm 281
    42.2. Vorgangserfassung 281
    42.3. Modelle 281
    42.4. Umgebungsvariablen 282
43. **Darstellung Sprossenskizze** 283
44. **Vertextung** 284
    44.1. Umgebungsvariablen 284
    44.2. Artikeltexte 287
    44.3. Sprossen 287
        44.3.1.1. Konfiguration 288
    44.4. Artikelbezeichnungen und Zusatztexte für Bearbeitungen in Fremdsprachen 289
    44.5. Darstellung SL + Bearbeitungen 290
        44.5.1.1. Andruck der Beschichtung / Struktur 290
        44.5.1.2. Zusammenfassen von identischen Bearbeitungstexten 291
    44.6. Automatische Textgenerierung 291
        44.6.1.1. Variablen 293
        44.6.1.2. Textzusätze 294
        44.6.1.3. Anlegen fremdsprachiger Artikel-Vermaßungstexte 300
    44.7. Konfigurierbare Texte 301
        44.7.1.1. Bei Rechnungen und Gutschriften 301
        44.7.1.2. Automatische Textgenerierung - Erweiterung der konfigurierbaren Texte 302
        44.7.1.3. Variable Texte (kspectxt) 303
45. **Warengruppenlogik** 304
    45.1. Produktgruppen: Ober-/Unterwarengruppe 304
    45.2. Warengruppenstruktur 304
    45.3. Kundenspezifische Warengruppe (SCHOLL) 311
    45.4. Kundenspezifische Warengruppe (Pilkington) 312
    45.5. Kundenspezifische Warengruppe (Wernberg) 314
        45.5.1.1. Zielsetzung 315
        45.5.1.2. ISO: 5. Und 6.Stelle 315
        45.5.1.3. ESG und Festmaße 6. Stelle 316
    45.6. Erweiterung der Warengruppenlogik (Art 6) 317
46. **Kostenstellenlogik im A+W Enterprise:** 318
    46.1. Umgebungsvariable: DEFAULT_KOSTENST 318
    46.2. $ALDATPFAD/kostenspec.dat 319
    46.3. Einkauf 320
        46.3.1.1. Variable KOSTENSTELLE_EK 320
        46.3.1.2. Kundenindividuelle Lösung (Interpane) 320
    46.4. Manueller Eintrag in kauf.kostenst 321
    46.5. Kostenstellenermittlung bei der Übergabe in den Einkauf (Bestellerzeugung): 321
    46.6. Kostenstellenübertragung 321
        46.6.1.1. Allgemein 321
        46.6.1.2. Protokolle 322
    46.7. FIBU-Schnittstelle: Konten und Kostenstellen. 322
47. **Deco-Nummern bei Sonderkanten** 323
48. **DXF-Import** 324
    48.1. Konfiguration 324
        48.1.1.1. Umgebungsvariable SN_DXF_NONMODAL 324
        48.1.1.2. Stammdaten 324
    48.2. Funktionalität 325
        48.2.1.1. Auftragserfassung 325
        48.2.1.2. DFÜ 326
49. **SN-Interaktion / SNLive-Skizze allgemein** 327
    49.1. Weiterführende Dokumentation 327
    49.2. Ansicht in der SNLive-Skizze (#412076) 327
        49.2.1.1. Beispiel: Kopfteil EP 1 328
        49.2.1.2. Einschränkungen 331
        49.2.1.3. Dokumentation der SN.ini Schalter 331
    49.3. Konfiguration 332
        49.3.1.1. DATEI_REF_PFAD 332
        49.3.1.2. SNFILES_DIR 332
        49.3.1.3. SN_CADFILES_DIR 333
        49.3.1.4. SNLIVE_EVAL_PRINTFLAG 333
        49.3.1.5. Zu beachtende Einschränkungen 333
    49.4. Skizzen für Rahmen-Kopfteile 333
    49.5. SNLive-Zoom 334
        49.5.1.1. Konfiguration 334
        49.5.1.2. Funktionalität 334
    49.6. SNLive-Skizze im Print Service 334
        49.6.1.1. Auswertung des Druck-Kennzeichens 334
    49.7. Fehlerrecherche SNLive-Skizze 335
        49.7.1.1. Falsche Modellmaße in der SN-Skizze 335
50. **Anbindung an A+W CAD Designer (Bars)** 336
    50.1. Auftragserfassung 336
    50.2. Produktionsübergabe 336
    50.3. Ausdruck 336
    50.4. Umgebungsvariablen 336
51. **Deckungsbeitrag** 338
    51.1. Auftragserfassung 338
    51.2. Negativer / minimaler Deckungsbeitrag nach Kostenkalkulation 338
    51.2.1.1. Umgebungsvariablen (Fehler! Textmarke nicht definiert.)
52. **Kostenkalkulation** 340
    52.1. Voraussetzung 340
    52.2. Kostenarten 340
    52.3. Ablauf 341
    52.4. Materialkosten 341
    52.5. Fixkosten / interner Deckungsbeitrag 342
    52.6. Maschinen- und Personalkosten 342
    52.7. Vererbung manueller Änderungen in der Kostenkalkulation 342
    52.8. Mengeneinheit Laufmeter in der Materialkostenkalkulation 343
    52.9. Kosten für lagerführige Artikel 344
    52.10. Rückschreibung geänderter Kosten aus der Bestellung 344
        52.10.1.1. Reklamationsbestellung 344
        52.10.1.2. Kostenlose Bestellungen 345
        52.10.1.3. Verlängerte Werkbank 345
        52.10.1.4. Verwendung von EK-Rabatten 345
        52.10.1.5. Mehrstufige Kostenrückschreibung 345
    52.11. Kostenkalkulation nach Auftragsfreischaltung 346
    52.12. Spezielle Preise 347
    52.13. Umgebungsvariablen 347
53. **Preise** 350
    53.1. Rundungen 350
        53.1.1.1. Genauigkeit der Rundung 350
        53.1.1.2. Bearbeitungen 350
    53.2. Preisberechnung für Unterteile auf Basis der Positionsmaße 350
    53.3. Globale Preispflege 351
        53.3.1.1. Funktionen in der globalen Preispflege 351
    53.4. Bearbeitungspreise 352
        53.4.1.1. Keine Bearbeitungen berechnen 352
        53.4.1.2. Preisrelevante Artikeltypen 352
        53.4.1.3. Kantenlänge bei Modellen 353
        53.4.1.4. Bearbeitungsfaktoren 353
        53.4.1.5. Spezielle Bearbeitungspreise 354
        53.4.1.6. Mindestbearbeitungspreise 354
        53.4.1.7. Mindestberechnung 355
        53.4.1.8. Bearbeitungsgruppenzuschläge 356
        53.4.1.9. Größenzuschlage 357
        53.4.1.10. Parameterabhängige Bearbeitungspreise (Formeln) 357
    53.5. Mindestberechnung 358
    53.6. Mindestpreis 359
        53.6.1.1. Mindestpreis für Unterteile (Zubehör) 359
        53.6.1.2. Mindestpreis bei ISO 359
    53.7. Sprosse 359
        53.7.1.1. Preise bei bestellten Sprossen / Sprossengitter 359
        53.7.1.2. Berechnung der zu berechnenden LM-K-R 359
        53.7.1.3. Berechnungstyp 14 – „K oder LM" 359
    53.8. Austauschpreise 360
        53.8.1.1. Auftrags-Artikelpreise ohne Austauschpreise 360
        53.8.1.2. Austauschpreise nach Vektor 360
        53.8.1.3. ISO 360
        53.8.1.4. VSG 360
        53.8.1.5. Austauschpreis nach Matrix (Größenstaffel) 361
        53.8.1.6. Austauschfaktor 362
        53.8.1.7. VSG-Austauschpreise 362
        53.8.1.8. Gussaustausch 363
    53.9. Stufenzuschlag 363
    53.9.1.1. Erweiterte Möglichkeiten für VSG-Stufenpreisberechnung 363
    53.9.1.2. Anzahl Stufen 364
    53.10. SZR-Zuschlag 365
        53.10.1.1. Standard-Berechnung 365
        53.10.1.2. SZR-Zuschlag auf Austausch 365
        53.10.1.3. SZR-Zuschlag für 3-fach ISO 365
        53.10.1.4. Größenzuschläge auch auf SZR 366
    53.11. PKZ-Glastüren 366
    53.12. Modellzuschlag 366
        53.12.1.1. Kein Modellzuschlag für Artikel, mit Modell im Artikelstamm 366
        53.12.1.2. Modellzuschlag für Dichtstoffe 367
        53.12.1.3. Modellzuschlag pro Warengruppe 367
        53.12.1.4. Modellzuschlag / Mindestmodellzuschlag 367
    53.13. Größenzuschlag 368
        53.13.1.1. ISO / Austausch 368
        53.13.1.2. Größenzuschläge bei Bearbeitungen und Zubehör 368
        53.13.1.3. Seitenverhältniszuschlag 369
        53.13.1.4. Größenzuschläge auf SZR-Zuschlag 370
    53.14. Referenzpreis 370
    53.15. Konditionen im Auftrag 371
        53.15.1.1. Falsche Preise in der Bestellung 371
        53.15.1.2. ISO-Konditionen nicht als manuell kennzeichnen 372
    53.16. Druckbare Preise 372
        53.16.1.1. Voraussetzungen 372
        53.16.1.2. Faktor 373
        53.16.1.3. Preise 374
    53.17. Umgebungsvariablen 377
54. **NR-Server / Nummernkreise** 382
    54.1. Vergabe der Rechnungs- und Gutschriftennummern über SPs 382
    54.2. Sperren freigeben #416415 382
    54.3. Wiederverwendung von Rechnungsnummern ohne Rechnungsdokument 383
55. **Produkt- und Bemaßungssets** 384
    55.1. Bemaßungssets 384
    55.2. Produktsets 385
        55.2.1.1. MODUL_PRODSET=0 385
        55.2.1.2. MODUL_PRODSET=1 386
56. **Lieferscheinerzeugung aus dem Versand** 388
    56.1. Fehler-Status 388
    56.2. Versand von Lieferscheinen als EMail bei der Erzeugung im Versand 388
    56.3. Lieferscheindruck im Versand abhängig von einem konfigurierbaren Feld im Marktpartner-Stamm 389
    56.4. Plausibilitätsprüfung 390
    56.5. Konfiguration 390
57. **Automatische Lieferscheinerzeugung im Hintergrund** 391
    57.1. Allgemeiner Prozess 391
        57.1.1.1. Protokoll 391
        57.1.1.2. Verarbeitung der Übergabedatei 391
    57.2. Format der Übergabedatei 393
    57.3. Funktionen 393
        57.3.1.1. Sperren 393
    57.4. Umgebungsvariablen 394
58. **Wareneingänge** 395
    58.1. Rechnungsübertragung / automatischer Wareneingang 395
    58.2. Wareneingangskontrolle 395
        58.2.1.1. Automatischer Wareneingang/Lieferscheinerzeugung bei Direktauslieferung 395
        58.2.1.2. Interne Verrechnung (kundenspezifisch) 395
    58.3. Gestellbezogener Wareneingang 395
        58.3.1.1. Gestelllager 396
        58.3.1.2. Buchung eines Gestelllagereingangs 396
        58.3.1.3. Multi-site Erweiterung 400
    58.4. Externer Wareneingang (z.B. SAP) 402
59. **Leistungserklärung** 403
60. **Spezielle Intauf-Arten** 404
    60.1. Kostenkalkulation (KOSTENKALKEK -15) 404
    60.2. Neu Summieren (FORALL_SUM -20) 404
    60.3. ENERGIEZUCHLAG Update (-26) 404
    60.4. ENERGIEZUSCHLAG hinzufügen (-28) 405
    60.5. Rechnung buchen (-33 RECHNUNG_BUCHEN) 405
    60.6. Rabatte neu berechnen (-37) 406
        60.6.1.1. Relevante Umgebungsvariablen: 407
    60.7. Preise neu berechnen (FORALL_PREISE (-38)) 407
    60.8. Kapazitätsplanung (-39 ALCIM_UEBERGABE) 407
    60.9. Gestellrechnungen (-40 VORGANG_NEU) 408
    60.10. INTERN Vorgang kopieren (AUFTRAG_NEU (-45)) 409
    60.11. Vorgang zur Kostenkalkulation übergeben (ALCIM_UEBERGABE_KK -47) 410
    60.12. Elementenaustausch (SLKORREKTUR -52) 410
    60.13. EK_RUECKRECH_PLUS -117 411
61. **Spezielle Prozessbeschreibungen** 412
    61.1. Produktion von Mustern / Tests 412
    61.2. Handel mit Bestellungen ohne Produktion 412
62. **Customizing** 413
    62.1. Protokoll 413
63. **Späte Änderung** 414
    63.1. Lokale Korrektur durch Bestellung 414
    63.2. Übergabe der späten Änderungen an Produktion 414
        63.2.1.1. Freie Aufträge und Weitergabe an Produktion 415
        63.2.1.2. Auftragsweises Sperren. Weitergabe an Produktion für Sperre über Bestellung/WE und KAUFUPDATE_BEI_BEST aktiv 416
        63.2.1.3. Auftragsweises Sperren. Weitergabe an Produktion alle anderen Sperren ohne aktiven KAUFUPDATE_BEI_BEST 416
        63.2.1.4. Positionsweises Sperren 417
        63.2.1.5. Vergleich ALTE / NEUE Logik. 418
        63.2.1.6. Rückschreibung eines geänderten Liefertermins aus dem Versand 419
        63.2.1.7. Änderung der Kommission und der Kundenpossition ignorieren. 419
64. **MWST-Anpassung** 421
    64.1. Konzeptübersicht 421
    64.2. Stammdaten 421
    64.3. Funktionsbeschreibung 421
    64.4. Handlungsrichtlinien 421
65. **Mehrwertsteuerumstellung** 423
    65.1. Stammdaten 423
    65.2. Funktionsbeschreibung 423
    65.3. Handlungsrichtlinien 424
66. **Packmittelplanung** 425
    66.1. Stammdaten 425
        66.1.1.1. Marktpartnerstamm 425
        66.1.1.2. Gestelltypen = Packmitteltypen 425
    66.2. Vorgabe zur Packmittelplanung 426
        66.2.1.1. Warnung bei vergessener Packmittelplanung 426
        66.2.1.2. Individuelle Prüfung der Packmittelplanung 426
    66.3. Planungsalgorithmen 427
        66.3.1.1. GA - Gesamt-Algorithmus 427
        66.3.1.2. TA- Teil-Algorithmus 428
        66.3.1.3. M- Manuell 431
        66.3.1.4. PA - Prioritäts-Algorithmus 433
        66.3.1.5. EA – Equal Algorithmus 433
    66.4. Gestellhauptgruppe 434
    66.5. Preise 434
        66.5.1.1. Kistenlieferant 434
    66.6. Kosten 434
    66.7. Bestellungen für Packmittel (Kisten) 435
    66.8. Protokoll 435
        66.8.1.1. Standard 435
        66.8.1.2. Erweitert 435
        66.8.1.3. Ftest 436
    66.9. Problembehandlung 436
    66.10. Umgebungsvariablen 437
67. **Versandsteuerung (allgemein)** 438
    67.1. Abschalten der A+W Enterprise Versandsteuerung 438
    67.2. Umgebungsvariablen 438
68. **Gestellbezogener Versand** 439
    68.1. Voraussetzung 439
    68.2. Freie Gestelle 439
    68.3. Scheibenzuordnung 439
    68.4. Verschieben im Versand 442
        68.4.1.1. Verschieben von festgebuchten Gestellen 444
    68.5. Umbuchen der Gestellmengen 445
    68.6. Fehlmengenkontrolle 449
    68.7. Verpackte Menge korrigieren 450
    68.8. Lieferscheine aus Versand 450
    68.9. Korrektur von Fehlbuchungen 450
        68.9.1.1. Aus BDE gemeldete Gestellbuchungen 450
        68.9.1.2. Buchung/Zuordnung des Gestells, wenn die automatische Zuordnung nicht möglich war. 454
69. **Beenden von ALCIB nach längerer Inaktivität** 459
70. **Import von Positionen aus Microsoft Excel** 460
    70.1. In der Auftragserfassung 460
        70.1.1.1. Konfiguration 462
71. **Angebotskontrolle** 463
72. **Angebotsoptimierung** 464
73. **Angebots-Kostenkalkulation (#393543)** 465
74. **Lokale Korrektur** 466
    74.1. Bestellfreigabe 466
        74.1.1.1. Direktbestellungen (extern) 466
        74.1.1.2. Direktbestellungen (intern) 466
        74.1.1.3. Bestellpool (intern und extern) 466
    74.2. Bestellfreigabe zurücksetzen 466
    74.3. Umgebungsvariablen 466
75. **Auftrags- und Positionsstatus** 468
    75.1. Dialog „Auftragsinformation" 468
    75.2. Aktionen im Versand 469
    75.3. Aktionen in der Produktion 470
        75.3.1.1. Umgebungsvariablen 472
76. **Systemmeldungen** 473
77. **Smart Companion** 474
    77.1. Voraussetzungen 474
    77.2. Einrichtung 474
    77.3. Gebinde 475
    77.4. Inventurablauf 476
    77.5. Betrieb und Prüfung 476
78. **Standortübergreifende BDE** 477
    78.1. Produktionsrückmeldung 477
    78.2. Interne Bestellung 477
    78.3. Produktionsübergabe 477
    78.4. Einlastung 478
    78.5. Etikettnummernvergabe 478
    78.6. Einschränkungen 478
    78.7. Booking 478
79. **Vorablieferscheinerzeugung und Rechnungserzeugung mit NVE-Logik** 479
    79.1. Relevante Umgebungsvariablen 479
        79.1.1.1. LAPOOL_NVE_LOGIC 479
        79.1.1.2. NVE_GLN 479
    79.2. Auftragserfassung 479
    79.3. Versandsteuerung 480
    79.4. Report-Stammdaten 480
    79.5. Dokumentenexport 481
    79.6. Weitere Informationen zur Konfiguration 481
80. **Dokumentenzuordnung** 482
    80.1. Funktion 482
    80.2. Bedienung 483
    80.3. Konfiguration 484
    80.4. Bezugnahme 484
    80.5. Bestellerzeugung 485
    80.6. Bestellübertragung 485
    80.7. Produktsets bei externer DFÜ 485
    80.8. IQuote 486
81. **Statusrückmeldung aus der Finanzbuchhaltung** 487
    81.1. Ablauf: 487
    81.2. Dialog Rechnung / Gutschrift buchen 488
    81.3. Konfigurierbare Texte 488
    81.4. Druck 488
    81.5. Protokolle / EMail 488
        81.5.1.1. Status 489
    81.6. Voraussetzung: 489
    81.7. Dateiaufbau 489
    81.8. Umgebungsvariablen 490
82. **A+W Enterprise Statistik** 491
    82.1. Verkauf – Kunde-Rechnung (ykuauf) 491
    82.2. Verkauf – Kunde-Artikel (ykartikel) 491
83. **Zuordnung von Chargen zu Bearbeitungsmaschinen** 492
84. **SQL-Abfragen** 495
85. **Excel-Übergabe** 496
86. **Skontologik** 497
    86.1. Stammdaten 497
    86.2. Anwendung 498
    86.3. Datenbank-Struktur 502
    86.4. Umstellung bei Kunden 502
    86.5. Skonto vor Mehrwertsteuer 503
    86.6. Skonto nach Mehrwertsteuer 504
    86.7. Konfiguration 504
87. **Auswahl von Windows-Dateien über den Dialog „Datei öffnen"** 506
88. **ViaPlant /via Plant** 507
89. **Intrastat** 508
90. **Nachbucher** 509
91. **Datawarehouse** 510
    91.1. Konfiguration 510
    91.2. Schreiben des Ankersatzes 511
    91.3. Verarbeitung des Ankersatzes 511
    91.4. Buchung der Data-Warehouse-Tabellen für Auftragsdaten 512

# 1. Key
## 1.1. Languages
### 1.1.1. Language code
For the use of the multi-lingual capability in A+W iQuote, the "Master Data - Keys - System - Languages" dialog has been expanded to include the "Language code" column. Here, the language code borrowing from the ISO languages is entered, which is used in A+W iQuote for the language definition - e.g. en-GB for English or fr-FR for French. The currently possible language codes are displayed in the field as a tool tip. Each language code may only be assigned to one A+W Enterprise language. There is no check whether the language code entered is valid and supported by A+W iQuote.

Caution: the input and evaluation of the language codes is case-sensitive; that is, de-DE is something different than de-de.

## 1.2. Product keys
### 1.2.1. Size variants
In the definition of dimension variants, there is the field "Total dimensions." This specifies the factor, how much of the defined TQU is in a piece.

e.g., Variant 3 quantity unit 4 (qm) - Dimensions 4500 x 3210 = 14,445

The factor - here with 3 places after the decimal point - is taken over for the creation of the article variant in stock (wlsv) and used for the bookings. An after-the-fact change of the factor in the variant master data can cause problems in the inventory booking. In addition, a change of the factor in the variant master data has no effect on the factor in the stock master data (wlsv).

In the order/PO, by default the physical quantity with 2 places after the decimal point is calculated (kpos.phymestk).

Due to this, there can be differences in the display of inventories in the "Stock forecast" module. The difference will always cause problems if the document quantities are compared to the stock quantities.

If you are working with the stock, you must consider which value you enter in the variants - 3 places after the decimal point or 2 places after the decimal point. If 3 places after the decimal point are entered there, you should consider activating the environment variable `RUNDUNG_PHYMESTK_3STELLIG`, which will round kpos.phymestk to 3 places in the documents too.

Note: This is **NOT** the price-relevant quantity, but the physical quantity of the item. The environment variable `RUNDUNG_3NACHKOMMASTELLEN` is responsible for the price-relevant quantity.

## 1.3. Form elements
### 1.3.1. Variables
In A+W Enterprise, formulas can be used in various places, e.g., for text generation, installation restrictions, restrictions in the article dimensioning, dimension inheritance in the BOM, processing prices.

Here is an overview of the available variables and arithmetic operators. However, we would like to point out that not all variables make sense in all areas. For this, the descriptions in the special areas must be taken into consideration.

The variables $1 - $20 refer to the details on the "Mandatory dimensions" dialog in the article master data. These can be used in the assembly restrictions in the article. Here is the most common use.
- **$1** = width (kpos.laenge)
- **$2** = height (kpos.breite)
- **$3** = AIR1 (kpos.szr)
- **$4** = AIR2 (kposp.szr2 bei 3-fach - ISO)
- **$5** = AIR3 (kposp.szr3 bei 4-fach-ISO)
- **$11** = SR (kpos.aham)
- **$12** = SR2 (for triple IG)
- **$13** = SR3 (for quadruple IG)
- **$20** is frequently used for customer-specific checks (e.g. glass strength). ([AW-222496])

Within the text generation, formulas can be used in the environment variable `GEN_ARTBEZ` as follows
- **$A1 - $A3** - article names 1 to 3
- **$L1 - $L3** - long description 1 to 3
- **$K** - short name
- **$G1; $G2** - glass names for IGU

Text generation for article dimensioning:
- **$REFPUNKT/$REFPOINT** -reference point
- **$ZT** - additional text

For the formulas for the individual elements
- **$DFx** -global steps
- **$STx** - local steps
- **$BVEK** = processing vector (refers to the dimension parameters from the "article dimensioning" dialog in the article master data.)
- **$LEVEL** = level (refers to the dimension parameters from the "article dimensioning" dialog in the article master data).
- **$CORNER** = corners (refers to the dimension parameters from the "article dimensioning" dialog in the article master data.
- **$QUALI** = refers to the dimension parameters from the "article dimensioning" dialog in the article master data.
- **$AP** = price-relevant number (for the text generation)
- **$PA** = position number (for the price calculation)

The variables $W1 - $W13 refer to the dimension parameters from the "article dimensioning" dialog in the article master data and can be used within the texting, restriction formulas, and price master data.
e.g. $W1 = diameter of the drillings

- **max (x, y)** the greater value of the two
- **min (x, y)** the lesser value of the two
- **pi** constant Pi (3.1415926)

### 1.3.2. Operators
You can combine two variables with "&" or "and" (and) or "|" or "or" (or).

The following operators and comparison operators can be used:

- `+` Addition
- `-` Subtraction
- `*` Multiplication
- `/` Division
- `=` equal to
- `<` less than
- `>` greater than
- `<=` less than or equal to
- `>=` greater than or equal to
- **max (x, y)** the greater value of the two
- **min (x, y)** the lesser value of the two
- **pi** constant Pi (3.415926)

## 1.4. Text supplements
Text supplements are used at various points in the program (texting, notes in the release pool, messages in A+W iQuote). However, the main purpose is the customer-specific texting of product properties. Therefore, the text supplements are documented in the section "Texting" > "Automatic text generation" > "Text supplements".

# 2. Article master data
## 2.1. Article types
For the creation of processings with the parallel use of A+W iQuote, please consult "EN-CONFIG- A+E Enterprise iQuote" for special restrictions.

### 2.1.1. Overview
An x in the price calculation or production column means that this article type is treated specially in the price calculation or during production transfer. For more precise details, see the special documentation.
"EN-CONFIG-A+W Enterprise Production Interface"

| Article type | Bill of materials | Order entry | EDI | Prices | Production |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 110 | | Product group | | X Exchange | |
| 200 | Min 2 pieces of glass and a spacer | x | x | x | x |
| 210 / 211 Spacer/colored spacer | Installation in IGU, Consists of spacers (220) | Calculation of the SR, SN display, Muntin entry | | | X |
| 220 Spacer | | Calculation of the SR | | | X |
| 230 muntins | | | Must be meta element | | |
| 240 Sealants | Installation in IGU | Sealing Depth | | X, No shape surcharge | x |
| 350 Boxes | | Box P.O., In dispatch not displayed. (Configuration box PO) | | | |
| 400 Glass doors | Can include IGU, Can include spacer | No size transfer, Dimensions of the elements differ from the dimensions of the item | X, An exchange in the product set | | X¹ |
| 510 Step | | No meta element, Step reduction measurement | | X, Surcharge | |
| 800 Mounting frame | Around the outside of an IGU | Not for stepped IG, Automatically reduces the glass dimensions | | | |
| 999 Other articles | | Costs of the packaging as discount (RABATT_VERPACKKOSTEN) | | | |

1 - IGU does not work as sub element, therefore AWE individual logic for sub-orders (EDI configuration instructions)

## 2.2. Article type
Articles with the article type "Meta" must have a BOM. Meta articles without BOM can cause problems in order entry. Typical meta articles are gas - gas+gas filling; muntins - muntin bars+muntin grill).
Step article is **NOT** a meta.

## 2.3. Bill of materials
- **Dr (strukt.f_dru)**
The print identifier in field "D": determines which print identifier the article gets in the BOM.
  - **N** - No - No output
  - **Y** - Yes - Output on all papers
  - **V** - Sales - Output only on sales papers
  - **P** - Production - Output only on production papers
  - **Q** - A+W iQuote - Display in A+W iQuote but no output on papers (only for processings)

## 2.4. IG
For the input of IG, correct administration of master data is vital. The most important master data information is the assembly position of glass, spacers, and sealants. The assembly position of the spacer is not numbered in two steps as for glass, but the airspaces are simply numbered all the way through. Between the lites with AP1 (2) and AP 3(4), there is the internal spacer with AP 1, between the lites with AP 3(4) and AP 5(6) the internal spacer with AP 2, and so on...

Sizes are compulsory in article master data. IG requires the global variables:
- **$1** = width (kpos.laenge)
- **$2** = height (kpos.breite)
- **$3** = AIR1 (kpos.szr)
- **$4** = AIR2 (kposp.szr2 bei 3-fach - ISO)
- **$5** = AIR3 (kposp.szr3 bei 4-fach-ISO)
- **$11** = SR (kpos.aham)
- **$12** = SR2 (for triple IG)
- **$13** = SR3 (for quadruple IG)

The data for the airspaces and SRs can be preset.

The bill of material of an insulated glass (IG) must consist of at least 2 lites and a spacer. Here it is important that the assembly positions and formulas are maintained correctly. The glass has the assembly position 1 or 2 or 3 or 4. For the formulas, you must make sure that there is one formula with and one formula without steps. The spacer has the assembly position 1 and a formula for the calculation less SR.

A triple IG must have 3 lites and 2 spacers. Here, the lites have the assembly positions 1/2, 3/4, and 5/6 and formulas as desired; at least 1 lite must have a formula with step reduction. The spacers have the assembly positions 1 and 2. They have formulas for the calculation less SR. Formulas in the 2nd spacer must handle $3 und $11 if you have entry parameters for $1,$2,$3,$4,$11,$12.

The different internal spacers have to have different formulas. If the internal spacer for FP1 has the formula XX, the internal spacer for FP2 should have the amended formula XX1:
- Step reduction = YES
- $1 = $1 - $12
- $2 = $2 - $12
- $3 = $4
- $11 = $12

And the internal spacer for FP3 should have the formula XX2:
- Step reduction = YES
- $1 = $1 - $13
- $2 = $2-$13
- $3 = $5
- $11 = $13

If you use the module "Variable sealing depth", the same formula as for the corresponding internal spacers has to be entered for the meta elements for sealants as well. If no formula is entered for the spacer, the system either automatically uses the formulas 201/202 or the environment variable `FRAME_FORMULAS`.

With regard to the spacer, there are other aspects with regard to variants, dynamic SR, and stockkeeping.

### 2.4.1. Quadruple IG (upgrade)
ALBAT+WIRSAM product version 2011 can handle quadruple IG. From commercial order entry to production, data structures have been adapted and extended for quadruple IG. Please note that ALBAT+WIRSAM products can handle only "narrow" BOMs here. This means that quadruple IG is produced from four lites and spacers, and is not assembled from two double IG lites. For IG in IG, starting with A+W Enterprise 6, a special function for generating sub-orders is required (see "EN-CONFIG-A+W Enterprise EDI").

For the input of quadruple IG, correct administration of master data is vital. The most important master data information is the assembly position of spacers and sealants.

The new formulas have to be entered in the BOM. Please also check the formulas for triple IG.

If the BOM elements have an effect to the global variables $3 or $11 (e.g. in case of an exchange of the sealant), these articles do not have to be changed. If the dimensioning record for a sealant is defined with the instruction $11=+2 in master data, the spacer belonging to this article will be amended automatically.

**Effects on the OrderXML file interface in ALCIB**
The OrderXML file interface will consider quadruple IG. The airspace details will be adopted for the spacer thickness. This is based on the sequence in which the spacers are defined in the BOM. This means: AIR1 is used for the first spacer on the BOM, AIR2 for the second spacer on the BOM, and AIR3 for the third spacer on the BOM.

The assembly position which, as described above, has to be kept for IG with more than two lites, determines the actual sequence for the transfer (can therefore principally differ from the sequence on the BOM). It is also used for the correct allocation of muntin patterns and sealants.

**Price calculation**
There is no automatic pricing (exchange prices) for quadruple IG; prices shall be entered by hand for the time being.

Details on the handling of quadruple IG by other products (ALCIM, ALFAK) can be found in the corresponding RN 2011.

**ATTENTION:** External saving of quadruple IG will NOT be handled. External saving of orders that include quadruple IG may result in defective order data.

## 2.5. Spacer
How the IG frame has to be created in the A+W Enterprise article master data depends on many different aspects within the entire process chain. In addition, there has to be a distinction between frame, mounting frame (AWE6 QR 09-22), and spacers in the creation. Frames (article type 210/211) are composed of spacers (article type 220). The mounting frame is not a frame in the sense of an IG frame and therefore has the article type 800.

Since the topic of frames runs through the entire process chain, there are also notes about various aspects in the various configuration instructions.

a) **Quantity unit**
Whether the quantity unit 1 linear meters or 3 millimeters is set doesn't matter at all for stock-keeping. Which of the two quantity units is used decides in which quantity unit the article is ordered.

b) **Variants**
Which different frame variants are offered at the company? Here there are color and thickness variants. Whether you are working in the article master data without variants, with thickness variants or with color variants has a significant influence on the entire process chain (entry, purchasing, stock)

c) **Purchase order**
If complete frames are ordered or are the frames produced in-house from spacers. Currently, spacers cannot be ordered order-related as meter goods. Normally spacers are kept in stock.

d) **Cost calculation**
In general, the spacer If the basic quantity unit is 3 - length (mm), the quantities are converted into linear meters in the material cost calculation.
If the basic quantity unit is 1 - linear meters (Ifm), the quanitities are not converted in the material cost calculation. In this case, this must be done with an appropriate inheritance formula.

e) **Stock**
In A+W Enterprise, articles can be created as dimension, color or size variant. In order to treat articles with size variants correctly in the stock, several settings are required, which will be summarized in the "Size variants in stock" section in this document. The configuration is described using the example of the spacer (article type 220).

### 2.5.1. Dimensions for POs
See "EN-CONFIG-A+W Enterprise EDI” and “EN-CONFIG-A+W EnterpriseProductionInterface”.
See also the environment variable `RAHMEN_BESTELLUNG_GLASMASS`.

### 2.5.2. Spacers in frame POs
See "EN-CONFIG-A+W Enterprise EDI"
See also the environment variable `RAHMEN_BESTELLUNG_SZR`

### 2.5.3. Mounting frame
[AW-102992] QR September 2022

External mounting frames are around the outside of the IG unit. They are not between the glass. External mounting frame should have the following structure in the article master data in order to be recognized as such:
- **Article type** = 800 (accessories)
- **Frame type** 1 (can be selected via toggle)
- **Thickness** >0 (artikel.staerke)

If an IG has this element in the BOM, then this item is recognized as IG with an external frame and the sub-elements (glass, frames) are reduced by the thickness of the mounting frame on all edges. For these parts (tuples) a shape record and a step record are stored.

A mounting frame cannot be used for stepped IG.

The thickness of the mounting frame is associated with the article and cannot be changed in the order. If another dimension is required, then another article with another thickness must be created. If the mounting frame in an existing BOM is exchanged or deleted, then the dimensions of the individual elements will be recalculated.

**Prerequisite:** important for this function is the presence of correct dimension inheritance formulas, especially for LAMI

**Restriction:** Within the item-spanning product exchange, the addition of mounting frames is not possible.

If the mounting frame should be produced in A+W Production as "non-glass article", then a generating processing is required.

This function has to be released with an environment variable:
`IGU_WITH_EXTERN_FRAME` (client reference: no)
Activates the opportunity of IG entry with a mounting frame.

## 2.6. Spacer type
Menu item `Master data > Keys > Products > Spacer types > Spacer types` can now be used to enter free Spacer types. An allocation to ALCIB spacer types can be made in the dialog. The ALCIB frame type is necessary for the correct display of the BOM picture at order entry.

The following options are available for selection:
- **Steel:** This is a steel spacer.
- **Alu:** This is an aluminum spacer.
- **TPS:** This is a thermo plast spacer (TPS).

The dialogs `Master data > Keys > Products > Spacer types > Individual names` and `Master data > Keys > Products > Spacer types > All names` can be used as always to enter translations for the existing spacer types.

In the item master data, in the Spacer type field, you can select the spacer type for spacer and IG spacer (item types 210 and 211).

Selection of the spacer type at document entry will influence the display of the glass structure: different spacer types are shown in different colors.

The spacer type number selected from item master data will be taken into account for production transfer via OrderXML interface (e.g. to ALCIM). Reports in the production system can also use it for the transfer to the machine driver. In this case, you will have to check with production before defining new spacer types.

We have made sure that the present item master data will not become inconsistent. For every of the four formerly existing spacer types, appropriate records were created in the database.

## 2.7. Dynamic SR
By default starting with Version AWE 6.0. In AWE 5.4, can be activated with the environment variable `AHAM_DYNAMISCH = ON`.

There is another possibility for calculating the SR dynamically in the IGU. The SR is now calculated in 3 stages:
1. Value from master data (mandatory dimension parameter) - musskenn
2. Collected from the BOM according to the new method
3. Collected from the BOM with formulas from item dimensioning

The last method has the highest priority.

**Master data:**
A configurable field "Sealing depth" of the type CHAR must be stored in the market partner master data. For customers with individual sealing depth, this must be entered here.

A configurable field "Sealing depth/Correction" of the type CHAR must be stored in the item master data. In an ENV switch `VTIEFE_TYP_TEST` you store the item types separated by "|" for which you would like to save specifications for the sealing depth. E.g. `240|870`. Header article (Atyp = 200 and spacer 210/211 are always evaluated)

If in the field of the value in shape "4.5" or "6.0" is entered, this counts as basic value. If the input is in the form "+0.5" or "-0.2", then this counts are a correction.

For IG header items, a dimension correction can be here as well.

**Evaluation on entry:**
If an IGU is entered, the SR is calculated as follows so the master data was maintained as above.
1. As basic value (default) for the sealing depth (VT) initially $11/2 – frame thickness is always used (thickness must be present for all frames in the master data). The basic value always applies only for frames that are defined via the assembly position.
2. If for the customer an individual VT is stored, it overwrites the default from point 1.
3. If for the associated item frame a value without leading sign is stored for VT, then this overwrites the default from points 1 and 2. If a value with leading sign + / - is stored there, it counts as correction.
4. If items in the BOM are defined with an item type that is stored in the ENV switch `VTIEFE_TYP_TEST` and if for this a value is defined without leading sign, then this overwrites the default from point 1, point 2, and point 3. The basic value for the spacer is overwritten in which these items exist (mapping child parts of spacer with spacer-IP or the spacer association with an individual assembly position). If the number of the frame cannot be determined, the associated value is not used.
5. Furthermore:
   a. possible increases or reduction from items of all item types from the ENV switch `VTIEFE_TYP_TEST` that have a correction value (+/-) in the master data,
   b. as well as any corrections are added directly from the header item (e.g. for 3-layer IGUs).
6. The evaluation in the BOM goes from top to bottom considering all sub-levels in the depth across each BOM element. First 1st glass incl. all child parts, then 1st frame, etc. depending on the structure of the BOM.
7. You cannot make the two possible corrections dependent on one another and exclude one or the other.
8. If the calculation of the VT is complete, then the SR of the item is calculated from `2 * VT + 2 * frame thickness`.

For the calculation, attention is always paid to the assembly position (IP) of the spacer and the sealing material. The data from the spacer and the sealing material with IP=1 is used for the calculation of kpos.aham (kposgv.gv11 if necessary). The data from the spacer and the sealing material with IP=2 is used for the calculation of kposgv.gv12, etc., corrections from the header item apply for all SRs. If a 3-layer IG in the master data is mapped with only one SR (only $11 variable), then data from the spacer and sealing materials with IP2 is not evaluated.

- If after the fact in an existing BOM one or several items are exchanged that bring a deviating VT correction, all affected items are recalculated.
- If the item (the IGU) was changed by the product exchange, then the VT is determined again.
- In case of change of the VT that occurred due to BOM change or product exchange, the muntin lengths (if muntin lengths are not calculated according to glass dimension) and the dimensions of the inner frame are recalculated. If the special logic for masking is active, the associated data must be checked and adjusted manually.
- A manually-changed SR remains valid until a BOM change that changes the VT is undertaken. It is also always taken over into the following items with the same BOM.
- If reference is made to an order or a quotation, the SRs from the original order are always taken over unless the customer in the new order is not the customer from the reference and an individual VT is stored for one of the two. In this case, all IG items are recalculated.

If the ENV switch `VERSIEGELUNG_ANZEIGEN` is active, then for each IG item in the middle dialog area below the product group over the character string "Rah x.xx / Ver x.xx" the distribution of the SRs is displayed.

The new logic can also be combined with the existing logic for SR inheritance, which can be controlled by an ENV switch. Thus the person entering the data is also informed by messages about the change of the SR e.g. during the BOM change.

`AHAM_VERERBEN_MIT_ABFRAGE = ON` controls the messages for SR changes. Caution, if manual SR changes are overwritten via SP in production.

`VTIEFE_TYP_TEST = xx|xx` List of the item types for which the data is sought.
`VERSIEGELUNG_ANZEIGEN`: display in the item.

Here are the brief instructions for the configuration:

**Environment variables**
- `AHAM_DYNAMISCH = ON` - activates the new logic (only required in AWE5)
- `MODUL_VERSIEGELUNGSTIEFE = ON` manual Sealing Depth in the order entry (since 2011, as basis for the new logic)
- `VTIEFE_TYP_TEST = 240` additional article types for which a sealing depth can be stored; separator |; not 200 and 210/211, special logic applies here.
- `AHAM_VERERBEN_MIT_ABFRAGE = ON` Message in case of change of the AHAMs in the order entry
- `IVERSIEGELUNG_ANZEIGEN = ON` for each IG item, the distribution of the SRs is displayed in the middle area of the dialog below the product group with the character string "Rah x.xx / Ver x.xx".
- `ISO_RAHMEN_MODELL = ON` Must be active

**Master Data**
- Market partner master-configured field "Sealing depth", type CHAR
- Article master - configured field "Sealing depth/Correction", type CHAR

**Replication**
Replication of the configurable fields in the market partner and article master data deactivated.
- `RP_ARTPRVFLD ON`
- `RP_MPPRVFLD ON`

**Settings**
Places after the decimal point for BOM articles (frames):
- `MASSFELD_RUNDUNG 1`
- `IMP_CTRL_NTEL_MM 10`

**Stored Procedures**
`SP cupmawpvtiefe` must be deactivated on the Alcib side. Then update record for `SP cupmawpvtiefe` to frei = 0.
On the Alcim side, `SP cu_setkundenvtiefe` must be deactivated.

**Processes**
Restart of intauf, OrderXML service, and Alcim import (under some circumstances, several imports)

## 2.8. Sealant Type
In `Master Data - Keys - Products - Sealant types`, individual sealant types can be created. This sealant type can then be entered in the item master data of the sealant.

An OrderXML file for an item including an IG lite will contain sealant data such as article number, description, and sealant type (section SEALANT).

These data is determined based on a sealant article in the A-W Enterprise BOM. Preferably, the sealant article should be on the same BOM level as the spacer and have the same assembly position.

Sealant in a standard A+W Enterprise BOM has a predefined structure: The sealant itself is a META element (article type 240, element flag 2) the BOM of which includes an element (article type 240, element flag 1) and a processing step.

> **Figure 1: Sealant meta element**
> The image shows a Bill of Materials (BOM) structure in German. It illustrates that a meta-element for a sealant (580205 Dichtstoff-Metateil) is composed of a sealant material (580211 Thiokol), a processing step (599005 Dichtmasse auflegen), and another processing step (599000 Isolierglasfertigung).

Generally, the sealant data for the OrderXML file is defined for the article number of the META element.

A new A+W Enterprise environment switch now defines that the data of the sealant's article number is defined by its BOM
If the determination of sealant data should be based on the element, the A+W Enterprise environment switch `ORDERXML_VERSIEGELUNGSDATEN` has to be enabled, and set to '1'.

The switch was introduced in versions 2009 and 2011 with a patch version for the ERP web service. The version code in the actual OrderXML file shows whether or not it is analyzed in the customer's system:
For Version 2009 it must be 3.5.13 or higher and for Version 2011, 3.6.2 or higher.

## 2.9. Foil type
Under the menu element `Master Data > Keys > Products > Foil types` all designations individual foil types can be created.

In the item master data, you can select the foil type for LAMI foils FD in the Foil type field (article type 176).

The item's article field provides a new opportunity to search for multi-lite units. Use the hotkey `<Shift>+<F8>` to start the search dialog. First select the article type you want to search for (IG/LAMI/cast resin). Now select one or two lites; this can be done by hand, by selo, or using the buttons. If the field for the first lite remains empty, the system automatically starts to search for the element.

For laminated glass, you can also enter the film type as a search criterion. The foil type has to be kept in `master data > Keys` and must be allocated in item master data.

You can use the AIR to search for an IG unit. If you enter the AIR, the system will find only products with the corresponding AIR1 or AIR2 or AIR3 as a compulsory size.

The minimum input for the search is the product type and the glass. The system will search for all products showing the glass element (or both) in their BOM. The sequence of the lites acc. to assembly position - does not matter.

Please note that for laminated glass, only the first foil will be checked. If the first lite of a laminated unit includes several foil layers, there will be no check. In this case, the airspace will be marked by an asterisk in the results table.

## 2.10. Fitting type
In the item master data, you can now store a fitting type for articles of the article type "Fittings (830)". The new Fitting type field is below the Article type field and can only be entered for fitting articles.

The fitting types that you can store in this field via `<SELO>` can be maintained under the product keys.

The fitting type goes into the generation of the SN key.

**Menu paths:** `Master data⇒Article`

**Creation of master data:**
- `MASTER DATA⇒KEYS⇒PRODUCT KEYS FITTING TYPES FITTING TYPES`,
- `MASTER DATA KEYS PRODUCT KEYS FITTING TYPES INDIVIDUAL DESCRIPTIONS`
- `MATER DATA KEYS PRODUCT KEYS FITTING TYPES ALL DESCRIPTIONS`

## 2.11. Muntins
### 2.11.1. Muntin type
The meaning of the muntin type for production is documented in the separate documentation of the production transfer "EN-CONFIG-A+W Enterprise Production Interface."

In addition, there is a definition of the terms in A+W Intranet:
`„KBase+ > A+W Clarity-General Information: > Glossaries > German / English > Muntin types"`

**CAD Designer (Bars) (AWDesign)**
A decision about how the muntin cross must look will be made in AWDesign about milling depth and trim value. Some of these values emerge from the ALCIB types. Only for special types is a specification in the master data actually necessary.

The following muntin types were previously specified:
- **Type 1** Muntins with double miter at the intersections
  > 