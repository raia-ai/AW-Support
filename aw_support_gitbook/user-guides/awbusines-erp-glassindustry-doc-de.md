---
title: "DE_AWBusines_Systemueberblick_5.21"
source: "DE_AWBusines_Systemueberblick_5.21.pdf"
tags: ["ERP", "A+W Business", "glass industry", "software manual", "Fenster", "Türen", "Glas", "Kapazitätsplanung", "Stammdaten", "production management"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides a comprehensive overview of the A+W Business ERP software, version 5.21. It details the system's architecture, modules, and core functionalities tailored for the glass, windows, and doors industry. The guide covers master data management, sales and purchasing processes, production planning (including A+W Business Pro), capacity management, inventory control, and reporting tools like A+W Discovery and A+W Dashboard. It also includes instructions for basic user operations, UI navigation, and a list of hotkeys."
long_description: "This is a detailed system overview (Überblick) for the A+W Business ERP software, a solution specifically designed for the flat glass industry, including manufacturers of windows and doors. The document, version 5.21 as of January 2017, serves as a comprehensive guide for end-users. It begins with an introduction to the A+W product portfolio, differentiating A+W Business from A+W Enterprise and outlining its 2-tier, MS SQL Server-based architecture. The core of the document explains the software's modular structure, covering key areas in depth. These include: Stammdaten (Master Data) for managing products, partners, bills of materials, and pricing; Dokumente for handling sales, quotes, and purchasing; Fertigung (Production) detailing the data transfer to production systems and the various expansion stages available; Kapazitätsplanung (Capacity Planning); Statistiken und Reports (Statistics and Reports), which covers integrated tools like Crystal Reports, A+W Discovery, and A+W Dashboard for business intelligence; and Lagerverwaltung (Inventory Management). Furthermore, the document provides a practical guide on 'Arbeit mit A+W Business' (Working with A+W Business), explaining how to start the application, navigate the user interface, and utilize standard menus and functions. A significant portion is dedicated to listing keyboard shortcuts (hotkeys) for efficient document and order entry. The manual concludes by explaining the available documentation and the context-sensitive online help system."
---

# A+W Überblick

---
## Vorspann
In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Version/Datum | Beschreibung |
| :--- | :--- |
| 1.00/03-1998 | Ersterstellung |
| 1.10/08-2000 | Überarbeitung |
| 1.20/04-2001 | Überarbeitung |
| 2.00/12-2003 | Struktureller Umbau auf Programmstruktur 4.0 |
| 3.00/12-2007 | Überarbeitung |
| 3.01/08-2008 | Abbildungen aktualisiert |
| 3.02/09-2010 | Layout an Doku-Konzept 2010 angepasst |
| 4.00/08-2013 | Anpassung der ALFAK-Dokumentation an A+W Business. |
| 5.00/05-2014 | Vollständige Überarbeitung des Parts Überblick. |
| 5.10/07-2014 | Aktualisierung der Ausbaustufen, Rechtschreibkorrekturen |
| 5.20/11-2015 | Liste der Hotkeys für die Auftragserfassung eingefügt. |
| 5.21/01-2017 | Produkt- und Firmennamen angepasst. |

### Editorial
Das Editorial enthält Informationen zu folgenden Themen:
- Anmerkungen zu diesem Dokument
- Urheberrechte
- Warenzeichen
- Kontakte

#### Anmerkungen zu diesem Dokument
Diese Veröffentlichung ist ausschließlich für Endanwender von A+W Business gedacht.
Diese Dokumentation und die darin beschriebene Software wird nur in Lizenz vergeben und darf nur gemäß dieser Lizenz verwendet und kopiert werden. Der Inhalt der Dokumentation dient nur der Information und kann jederzeit ohne Vorankündigung geändert werden. Bei der Zusammenstellung von Texten und Abbildungen wurde mit größter Sorgfalt vorgegangen. Trotzdem können Fehler nicht vollständig ausgeschlossen werden. A+W Software GmbH übernimmt keine Haftung für Fehler oder Ungenauigkeiten, es sei denn, diese beruhen auf vorsätzlichem oder grobfahrlässigem Handeln.
Dieses Dokument beschreibt die volle Ausbaustufe von A+W Business.

#### Urheberrechte
© 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.
Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung von A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

#### Warenzeichen
Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind zu beachten.

#### Kontakte
**A+W Software GmbH**
Am Pfahlgraben 4-10
D-35415 Pohlheim
- **Telefon**: +49 6404 2051-0
- **Fax**: +49 6404 2051-877
- **E-Mail**: zentrale@a-w.com
- **Web**: http://www.a-w.com

## Einleitung

### Vorbemerkung
A+W Business ist ein modernes ERP System, das auf die Anforderungen und Bedürfnisse der Flachglasindustrie ausgerichtet ist. A+W Business unterstützt die Erfassung von Dokumenten im Rahmen von Verkauf und Einkauf und ermöglicht die Steuerung und Kontrolle angrenzender Bereiche und Prozesse, z. B. Lagerverwaltung, Kapazitätsplanung, Versand etc.

Angebotswesen, Auftragsabwicklung, Einkauf, Lieferwesen und Fakturierung lassen sich mit A+W Business einfach und effizient steuern und überwachen.

A+W Business ist in das Produktportfolio der A+W Software GmbH eingebunden und kommuniziert mit den jeweiligen Produkten. Insgesamt stellt sich das Produktportfolio der A+W Software GmbH wie folgt dar:

**Produktportfolio Übersicht (Abb. A-1)**

- **ERP (ERP Solution)**
  - A+W Enterprise
  - A+W Business (Verkauf, Einkauf, Lager, Versand, Statistik, eCommerce)
- **PPS (PPS Solution)**
  - A+W Production
  - A+W Business Pro (Kapazitätsplanung, Produktionsplanung, Verschnittoptimierung)
- **Maschinensteuerung (Control Units)**
  - Production Terminal
  - Realtime Optimizer
  - Rack Optimizer
  - Dynopt
- **Maschinen (Machines)**
  - Zuschnittslinie, ISO Linie, VSG Linie, etc.
- **Produktionsmonitoring (Controlling & Monitoring)**
  - A+W Production Cockpit
  - A+W Dashboard
- **CAD Konstruktion (CAD Designer)**
- **Statistik & Analyse (A+W Discovery)**

In dieser Übersicht sind die Produkte der A+W Software GmbH mit den jeweiligen Kernkompetenzen dargestellt.

### A+W Business in Abgrenzung zu A+W Enterprise
Die A+W Software GmbH bietet zwei kaufmännische Software-Lösungen an: A+W Business und A+W Enterprise. Beide Systeme erfüllen die Anforderungen der Flachglasindustrie im kaufmännisch-administrativen Bereich. Ihr Einsatz richtet sich nach der Unternehmensgröße und -struktur:

- **A+W Business** ist für Einzelbetriebe konzipiert oder für Unternehmensgruppen, die wie Einzelbetriebe agieren. Das System setzt auf eine moderne, windows-basierte 2-Schichten-Architektur auf einer MS SQL Server-Datenbank auf.
- **A+W Enterprise** ist für größere Unternehmen mit einer ausgeprägten Niederlassungsstruktur konzipiert. Das System setzt auf eine UNIX-/LINUX-basierte 3-Schichten-Architektur auf einer Informix-Datenbank auf.

### Leistungsmerkmale von A+W Business
A+W Business ist mit seiner vollgrafischen Oberfläche leicht und schnell zu bedienen und vereinfacht die unternehmensinternen Prozesse rund um die Auftragsabwicklung.

#### Ergonomie, Transparenz und Übersichtlichkeit
A+W Business ist eine Multi-Dialog-Anwendung:
- Mehrere Dialoge, z. B. Angebots-, Auftrags- und Stammdatendialoge, können gleichzeitig geöffnet und bearbeitet werden.
- Die Dialoge sind frei positionierbar und können stufenlos skaliert werden.
- Mit einem Editor können Dokumente und Reports leicht und schnell formatiert und an die Ansprüche Ihres Unternehmens angepasst werden.

#### Hauptfunktionen
- Stammdatenverwaltung
- Angebotswesen
- Auftragsabwicklung mit Erstellung von Teillieferungen und Reklamationen
- Erstellung aller kaufmännischen Papiere, z. B. Auftragsbestätigung, Lieferschein usw.
- Routenplanung und -optimierung
- Lagermanagement
- Integrierte Produktionsplanung und -steuerung, z. B. Kapazitätsplanung, Lauf- und Feinplanung, Optimierung, Betriebsdatenerfassung.

#### Automatisierung bei Verkaufsdokumenten
Das System bietet umfangreiche technische Unterstützung bei der Bearbeitung von Aufträgen und Angeboten.
- Erfasste Elemente werden maßstabgetreu angezeigt und grafisch dargestellt, um Fehler bei der Eingabe zu vermeiden und um den Gesamtprozess zu beschleunigen.
- Die Preisberechnung ist sehr flexibel und ermöglicht eine vielfältige Einteilung in Standardpreise und kundenspezifische Konditionen. Die Berechnung wird systemübergreifend gesteuert, kann aber auch manuell angepasst werden.
- Lieferscheine und Rechnungen werden nach konfigurierbaren Einstellungen aus den Auftragsdaten erzeugt.

#### Anbindung an weitere Anwendungen
Das A+W Business-Paket kann durch weitere Anwendungen ergänzt werden:
- EDI-Lösung für den elektronischen Austausch von Aufträgen und Rechnungen.
- Erweiterte CAD-Funktionalitäten
- Interne Gestellverwaltung
- Microsoft Outlook Anbindung
- Schnittstellen zu diversen Finanzbuchhaltungs- und Dokumenten-Management-Systemen
- Auswertungen in Form von Berichten und Statistiken
- Erweiterte Produktionssteuerung und -kontrolle durch die Anbindung an das Premium PPS-System A+W Production
- Microsoft Sharepoint Anbindung zur integrierten Dokumentenverwaltung und -archivierung

### Systemumfeld
Um den grundlegenden Anforderungen eines leistungsfähigen IT-Systems gerecht zu werden, wurde auf folgende Bereiche besonders geachtet:
- Betriebssicherheit
- Systemverfügbarkeit
- Unterstützte Hardwareplattformen
- Erweiterbarkeit
- Vernetzungsmöglichkeiten
- Zugangsbeschränkung und -kontrolle

A+W Business kann aufgrund der Client-Server-Architektur den betrieblichen Erfordernissen schrittweise angepasst und erweitert werden.

(Abb. A-2 zeigt eine 2-Schichten-Architektur mit "Client-PC Windows" für die Logik- und Darstellungsschicht und einem "Server" für die Datenschicht.)

#### Systemarchitektur
A+W Business baut auf Windows-Betriebssystemen auf und kann auf modernen Microsoft Server-Client-Systemen betrieben werden.
Durch die klare Trennung von Datenhaltung, Datenverarbeitung und Oberfläche in der 2-Schichten-Architektur lässt sich das System sehr flexibel an die betrieblichen Erfordernisse anpassen. Damit ist es bei wachsender Benutzerzahl problemlos möglich, mehr Rechnerleistung in die Applikationsschicht einzubringen, ohne dass Datenbanken und Einstellungen an den Benutzer-PCs verändert werden müssen.
Für die Datenhaltung wird die relationale MS SQL Server-Datenbank eingesetzt. Das zugrunde liegende Datenmodell kann über eine Online-Dokumentation eingesehen werden. Dies dient insbesondere der Erweiterbarkeit und der Möglichkeit schnell und effizient Reports und Statistiken zu erstellen.
A+W Business unterstützt Sie hierbei mit einfachen Werkzeugen und integrierten Standardfunktionalitäten wie Crystal Reports.
A+W Business lässt sich in die bestehende Netzwerklandschaft einbinden. Schnittstellen zu E-Mail, Telefax und zu Telefonanlagen sind integrale Bestandteile.

#### Datensicherheit
Die Anwendung ist transaktionsgesichert. Dies bedeutet, dass das Programm Aktionen vollständig zu Ende führt, z. B. wenn Rechnungen erzeugt werden. Wenn dies nicht möglich ist, wird die begonnene Aktion vollständig abgebrochen. Damit ist ausgeschlossen, dass die Datenbank mit Fehlern oder Datenfragmenten gefüllt wird. Die eingesetzten Komponenten ermöglichen selbst im Falle eines Systemabsturzes, die Daten fast vollständig und in jedem Falle konsistent wieder herzustellen. Die Datensicherung erfolgt automatisch zur einstellbaren Uhrzeit oder parallel zum laufenden Betrieb.

#### Benutzeroberfläche
A+W Business steht auf einer vollgrafischen Benutzeroberfläche unter Windows-Plattformen zur Verfügung. Damit sind die Funktionen des Tagesgeschäfts intuitiv bedienbar.

#### Zugriffsrechte
Zur Basisversion von A+W Business gehört die Verwaltung von Zugriffsrechten: Sie können für jeden einzelnen Mitarbeiter oder für Mitarbeitergruppen festlegen, welche Programme ausgeführt werden dürfen.
Detailliertere Zugriffsrechte können Sie über die Rechteverwaltung definieren, z. B. das Recht, die Daten zu lesen aber nicht zu ändern.
Standardmäßig wird A+W Business mit vier vordefinierten Mitarbeitergruppen ausgeliefert. Sie können zusätzliche Gruppen und Profile anlegen, z. B. um Rechte zu entziehen oder zusätzlich zuzuordnen. Dies könnte z. B. für Mitarbeiter aus der Produktion sinnvoll sein, die nur produktionsrelevante Informationen aus A+W Business benötigen, aber keine Daten ändern dürfen.

#### Wartung und Pflege
Zu jeder A+W Business-Installation gehört ein leistungsfähiges Betreuungskonzept. Zur Betreuung gehören regelmäßige Updates, die über das Netz verschickt und außerhalb der normalen Betriebszeit installiert werden. Die Wartung erfolgt grundsätzlich über eine Netzwerkkopplung, so dass ein gleichzeitiger Datentransfer stattfinden kann. So ist ein sehr effektiver Support möglich.
Über den A+W Premium-Wartungs- und Servicevertrag Value+ können Sie zusätzlich auf eine Vielzahl von Dokumenten und Best-Practice-Schulungen, Tipps und Tricks zugreifen – und das kostenfrei.
Selbstverständlich bieten wir Ihnen diese Premium-Leistungen auch gern abgestimmt auf Ihre individuellen Bedürfnisse an.

### Modularer Aufbau
Der modulare Aufbau von A+W Business erlaubt eine flexible Abbildung und Steuerung der komplexen Geschäftsprozesse Ihres Unternehmens.

(Abb. A-3 zeigt ein Flussdiagramm des modularen Systems, das die Interaktion zwischen verschiedenen Modulen darstellt.)

**Zusammenspiel der Module:**
1.  **Stammdaten** (Basisdaten, Partner, Produkte, Preise etc.) bilden die Grundlage.
2.  **Angebotswesen** führt zur Erstellung von **Aufträgen**.
3.  Aufträge können zu **Routenoptimierung**, **Kapazitätsplanung**, und **Fertigung** führen.
4.  Aus der Fertigung (ggf. über **A+W Production**) gehen die Produkte in den **Versand** und die **Gestellverwaltung**.
5.  Der Prozess endet mit **Rechnungen/Gutschriften**, der **Übergabe an die FiBu** (Finanzbuchhaltung) und der Archivierung in **Archiv**.
6.  Parallel dazu existieren Module wie **Lager** (das mit dem **Einkauf** interagiert) und **Statistiken**.
7.  Alle Dokumente können am Ende gelöscht werden.

## A+W Business-Module
A+W Business unterscheidet zwischen Stammdaten und Bewegungsdaten:
- **Stammdaten** werden erfasst und danach nur selten geändert.
- **Bewegungsdaten** betreffen die kaufmännischen Vorgänge und ändern sich je nach erfasstem Vorgang.

Der ständige Datenaustausch sorgt für aktuelle Informationen zwischen den Modulen.
Die Basisversion Verkauf bietet die Möglichkeit zur Erfassung und Abwicklung von Kundenanfragen und -aufträgen bis zur Archivierung.
Mit den Zusatzmodulen erweitern Sie die Abwicklung der kaufmännischen Vorgänge um das Bestellwesen, die Lagerverwaltung und verschiedene Schnittstellen, z. B. zum elektronischen Datenaustausch mit Kunden und Lieferanten oder zur Produktion usw.

(Abb. A-4 zeigt die Programmoberfläche mit einer Navigationsleiste, die den modularen Aufbau widerspiegelt.)

**Modulbereiche in der Programmoberfläche:**
- **A Stammdaten:** Anlage und Pflege der Stammdaten (z. B. Produktverwaltung, Marktpartner).
- **B Dokumente:** Erfassung und Bearbeitung der kaufmännischen Vorgänge (z. B. Aufträge, Angebote, Bestellungen).
- **C Fertigung:** Übergabe der Auftragspositionen an die Kapazitätsplanung und die Produktion.
- **D Statistik:** Auswertung der kaufmännischen Vorgänge.
- **E Lagerwirtschaft:** Verwaltung und Beschaffung des Materiallagers.
- **F Kapazitätsplanung:** Verwaltung der Stammdaten für die Kapazitätsplanung.
- **G Utilities:** Systemübergreifende Einstellungen.

### Stammdaten
Die Organisation und Pflege der Stammdaten ist die Basis von A+W Business und seinen Modulen. Stammdaten werden in alle Bereiche des Systems übernommen: alle Geschäftsbereiche greifen auf die gleichen Stammdaten zu, z. B. Kunden, Produkte, Preise, Status, Währungen.
Übergreifende Parameter für Ihr Unternehmen oder pro Mandant Ihres Unternehmens legen Sie in den Firmendaten fest.
Über Schnittstellen können die Stammdaten auch an andere Programme übergeben werden, z. B. an A+W Production.

(Abb. A-5 zeigt ein Beispiel für die Kundenstammdaten-Maske.)

#### Basisdaten
Zu den Basisdaten gehören z. B. Nummernkreise und Statusverwaltung. Mit Hilfe der Statusverwaltung haben Sie die Möglichkeit, Ihre Firmenabläufe in A+W Business abzubilden. Bei der Vergabe von Status, Mindest-Status und Sperr-Status können Sie Ihre internen Prozesse und Arbeitsabläufe widerspiegeln.

#### Partner
In der Partnerverwaltung wird zwischen Kunden, Lieferanten und sonstigen Partnern unterschieden. Zu allen Partnern hinterlegen Sie neben den Adressen weitere Parameter, die Ihnen die Angebots- und Auftragserfassung erleichtern, z. B. die Liefertour, abweichende Rundungen, Mitarbeiter und Filialen, Zahlungsbedingungen, Objekte.
Eine integrierte Export-Funktion ermöglicht Ihnen, Ihre Kundendaten nach Microsoft Word zu exportieren, um Serienbriefe zu erstellen.

#### Produkte
In A+W Business können Sie Ihre firmeneigene Produktstruktur abbilden. Unter Produkt wird in A+W Business all das verstanden, was als eigene Position im Auftrag aufgeführt werden soll. Daraus folgt, dass Bearbeitungen, Anzahlungen und Zuschläge oder Ganzglasanlagen genau wie ISO-Einheiten oder Einfachgläser als Produkte angelegt werden.
Sie sind frei in der Vergabe sowohl der Artikelnummern, als auch eines alphanumerischen Matchcodes.

#### Stückliste
Ein Produkt kann aus mehreren Produkten zusammengesetzt sein, z. B. eine ISO-Scheibe mit zwei Gläsern, einem Rahmen und einer runden Form (Modell). Diese Komponenten bilden die Stückliste. Jede einzelne Komponente ist selbst ein Produkt.
Sie können Ihre Produkte also so gestalten, dass die Erfassung als Auftragsposition weitgehend automatisiert wird.

Die Stückliste ist die Grundlage für folgende Funktionen:
- Preisberechnung
- Produktbezeichnungen in Dokumenten, z. B. Bezeichnungen in der Auftragsbestätigung
- Planung der Lagerwirtschaft
- Organisation der Fertigungssteuerung
- Ermittlung von Fertigungszeiten

(Abb. A-6 zeigt die Stücklisten-Komponenten eines ISO-Produkts, bestehend aus Hauptprodukt, Einfachglas, Abstandhalter, Wärmeschutzglas, Modell und Stufung.)

Die Komponenten der Stücklisten können sowohl einzelne Produkte als auch Bearbeitungen oder weitere Stücklisten, sogenannte Baugruppen, sein. Alle Komponenten der Stückliste müssen als Produkte in den Stammdaten angelegt sein.
Die Stücklistenauflösung ist unbegrenzt offen: Mehrfach-ISO, Mehrfach-VSG oder ESG können in Stücklistenformat geführt werden. A+W Business geht sogar so weit, dass für jede Komponente einer Stückliste unterschiedliche Konditionen zur Preisberechnung herangezogen werden können.

#### Varianten
Da das Programm bei den Produkten mit Variantenunterscheidung arbeitet, existiert z. B. ein Float 4 mm nur einmal im System. Alle die Float 4 betreffenden Varianten werden unter der gleichen Nummer geführt und in der Auftragserfassung automatisch erkannt. Diese Varianten können sich auf Lagermaße, Festmaße, Kisten, Stückartikel, Farben usw. beziehen. Jede Variante kann eine andere Warengruppen zugeordnet werden.

#### Sprossen
In A+W Business werden in der Regel Sprossen für den SZR angelegt und nach Konstruktionstypen unterteilt. Alle Sprossen, Verbindungsstücke und Randstopfen werden als Produkt angelegt, damit sie im Auftrag erfasst werden können.
Sprossen können in Bezug auf die Felder oder auf die Bohrpunkte symmetrisch oder asymmetrisch erfasst werden.
- Für die Berechnung der Sprossenkonstruktion können eigene Maße eingegeben werden, so dass die Bohrungen bzw. die Felder asymmetrisch angelegt werden.
- Bei der automatischen Berechnung kann gewählt werden, ob die Symmetrie sich an den Bohrungen oder an den Feldern ausrichtet.

(Abb. A-7 zeigt zwei Beispiele für die symmetrische Berechnung von Sprossenkonstruktionen: "Bohrpunkt-symmetrisch" und "Feld-symmetrisch".)

#### Modelle
Für die Modellerfassung bietet A+W Business standardmäßig den A+W Modellkatalog an. Die Modellvorgaben aus dem Katalog sind ohne Maße und Glas als Produkt angelegt. In einer Auftragsposition weisen Sie einem Glasprodukt eine nicht-rechteckige Form aus dem Modellkatalog zu und ergänzen die gewünschten Maßen.

(Abb. A-8 zeigt schematisch die Darstellung eines Modells: Zuerst wird ein Modell ohne Maße angezeigt (A), und nach Erfassung der Maße im Auftrag wird die Anzeige aktualisiert (B).)

Sie können Ihre Modelle aber auch anhand des Modellkataloges von Bystronic oder Billco erfassen.

#### Organisation der Warengruppen
Alle Produkte werden Warengruppen zugeordnet. Diese werden in die drei Ebenen der Warenhaupt-, Warenober- und Warengruppe unterteilt.
Außer diesen Ebenen haben Sie die Möglichkeit, Kombinationen von Warengruppen zu definieren. Jeder Warengruppenebene können Sie außerdem TOP-Warengruppen zuordnen.

(Abb. A-9 zeigt den hierarchischen Aufbau der Warengruppen: WHG (Warenhauptgruppe), WOG (Warenobergruppe), WGR (Warengruppe).)

- Die **Warenhauptgruppe (WHG)** dient zur Rabattvergabe und zu statistischen Auswertungen.
- Die **Warenobergruppe (WOG)** dient zur Rabattvergabe und zu statistischen Auswertungen.
- Die **Warengruppe (WGR)** dient zur Rabattvergabe, Produktorganisation und Statistik. Nur dieser Ebene kann ein Produkt zugeordnet werden.

Wenn Sie mit einem Programm zur Finanzbuchhaltung arbeiten, werden die Konten über die Warengruppen zugeordnet.

#### Preise und Zuschläge
Keine andere Branche weist so komplexe Mechanismen für die Preisberechnung auf wie die Flachglasindustrie. Da wir diese Mechanismen nicht ändern können, soll zumindest die Pflege und Verwaltung der Preislisten und Tabellen so einfach wie möglich sein.
Aus diesem Grund ist die Preisberechnung in A+W Business aus flexiblen Bausteinen zusammengesetzt, die alle Berechnungsmöglichkeiten abdecken. Preismatrizen können für Handelsgläser genauso genutzt werden wie für Isoliergläser. Standard-Preislisten können importiert und exportiert werden.
Jedem Produkt ordnen Sie die gewünschte Preistabelle, Zuschläge und den gesetzlichen Steuersatz zu.

(Abb. A-10 zeigt die Produktverwaltung mit dem Fokus auf Preis- und Zuschlagseinstellungen.)

Preise und Zuschläge können als Standard oder individuell für Kunden oder Kundengruppen angelegt werden:
- **Preise:**
  - Matrizen, z. B. für Isolierglas, Ornamentglas
  - Vektoren, z. B. Mengenstaffelung pro Auftrag
  - Einzelpreise, z. B. für Einfachglas
  - Preis-Würfel, z. B. für Schleifmatrizen
- **Zuschläge auf Hauptprodukt:**
  - Sprossenzuschläge
  - Modellzuschläge
  - Gruppen-/Austauschzuschläge
- **Sonstige Zuschläge, z. B.:**
  - **Sonderrabatte und Teuerungszuschläge:** Standardmäßig sind Sonderrabatte/Teuerungszuschläge integriert.
  - **Energiezuschlag:** Energiekosten können an Kunden weitergegeben werden.
  - **Transport-/Mautkosten:** Berechnung pro Entfernungskilometer.
  - SZR-, Klein-/Übergrößen-, Mindestmengen-, Dickenzuschlag

**Neuen Preisjahrgang vorbereiten – einfach gemacht**
Zur Preisverwaltung gehört die Möglichkeit, Preise vollständig oder teilweise zu kopieren und absolut oder prozentual zu ändern. Sie können neue Preise in Ruhe vorbereiten, in einen neuen Preisjahrgang kopieren, anpassen und zu einem definierten Datum aktivieren.

**Automatische Preisberechnung**
Die Preise werden automatisch berechnet, egal ob Standard- oder Individual-Preise. Alle Angaben zur Berechnung der Positionen werden automatisch herangezogen. Preise können im Angebot oder Auftrag manuell übersteuert werden.

#### Rabatte
Die Rabattübersicht in Form eines Verzeichnisbaumes macht es Ihnen leicht, sich einen Überblick über die angelegten Rabatte zu verschaffen.
Rabatte können allgemein für ein Produkt oder pro Kunden/Lieferanten vergeben werden. Kunden oder Lieferanten, für die dieselben Preis- und Rabattkonditionen gelten, fassen Sie zu Kunden- bzw. Lieferantengruppen zusammen, was die Pflege der Rabatte enorm erleichtert.

Sie können unterschiedliche Rabatte verwalten:
- Standardrabatte für einen Preisjahrgang und Preisschlüssel (Tarif)
- Staffelrabatte mit einer Grenzmenge
- Austauschrabatte

Der Rabatt wird im Auftrag automatisch herangezogen. Ein manueller Rabatt kann im Auftragskopf (für den gesamten Auftrag) oder in der Positionserfassung eingetragen werden. Sie können auch einen globalen Rabatt für Warengruppenebenen anlegen.

### Dokumente
Zu den Bewegungsdaten gehören alle Daten der kaufmännischen Vorgänge und der Lagerverwaltung.
- Kaufmännische Vorgänge werden in Dokumenten erfasst und überwacht, z. B. vom Angebot über den Auftrag bis zur Rechnung und Archivierung.
- In der Lagerverwaltung können Sie zudem die Bestände Ihres Lagers kontrollieren und Warenwerte prüfen.

#### Verkauf - Aufträge und Angebote
Die Auftragsbearbeitung ist der zentrale Bestandteil von A+W Business. Hier fließen alle Daten aus den Stammdaten zusammen. Die Auftragsdaten werden je nach Ausbaustufe an Lager, Einkauf, Kapazitätsplanung und Produktion übergeben.

In der Auftragsbearbeitung wird zwischen folgenden Bereichen getrennt:
- **Auftragskopf:**
  - Name und Anschrift des Kunden, Lieferbedingungen und -termin, Zahlungsbedingungen.
  - Diese Angaben werden aus den Stammdaten des jeweiligen Kunden eingelesen und können pro Auftrag geändert werden.
- **Auftragspositionen:**
  - Produkt und Produktaufbau (z. B. Glas, ISO, Sprossen)
  - Maße und Bearbeitungen (z. B. Modellformen, Ausschnitte)
  - Preise und Rabatte
  - Makrosuche nach Produktaufbau
  - Zuschläge (z. B. für den Transport)

(Abb. A-12 zeigt die Auftragserfassung im Verkauf, geteilt in den Auftragskopf (A) und die Auftragspositionen (B).)

#### Erfassung von Modellen
Über die Standard-Modellerfassung hinaus bietet A+W Business die sogenannte Technische Auftragserfassung (TOE). Hierfür können Sie im A+W CAD Designer komplexe Templates und/oder Makros erstellen und diese über die Integration in A+W Business schnell in Aufträgen und Angeboten übernehmen. Dies spart Zeit und Geld.

(Abb. A-13 zeigt ein Template einer Studiotür im A+W CAD Designer (A) und die resultierende Auftragsposition (B).)

#### Automatisierte Geschäftsabläufe
Aus dem Auftrag heraus entstehen weitere Geschäftsabläufe, die so weit wie möglich automatisiert sind:
- Druck von weiteren Dokumenten (z. B. Auftragsbestätigung, Lieferschein, Rechnung)
- Bestellung durch den Einkauf
- Abruf der Lagerartikel für die Produktion
- Übergabe der Auftragsdaten an die Produktion
- Rückmeldung aus der Produktion, wenn der Auftrag fertig ist
- Auslieferung
- Prüfung der Zahlungen vom Kunden
- Übergabe von Rechnungen an die Finanzbuchhaltung

#### Kreditlimitprüfung
Sie können für jeden Kunden ein Kreditlimit festlegen und automatisch bei der Erfassung neuer Aufträge prüfen lassen.
Für die Prüfung des Kreditlimits müssen Sie folgende Entscheidungen treffen:
- Kreditlimit pro Kunde in den Kundendaten bestimmen.
- Reaktion bei Überschreitung des Kreditlimits festlegen (z. B. Statusänderung oder Warnmeldung).

Wenn Sie mit Filialen arbeiten, kann das Kreditlimit auf zwei Ebenen geprüft werden:
- Das Kreditlimit der Filiale selbst wird geprüft.
- Das Kreditlimit des Hauptkunden wird geprüft (je nach Einstellung).

#### Formulardruck
Alle kaufmännischen Papiere werden in Formulare gedruckt und können auf Papier oder elektronisch ausgegeben werden. Zusätzlich stehen weitere Druckfunktionen zur Verfügung, z. B.:
- Auflistung aller Aufträge des aktuellen Auftragsbestandes
- Vermaßte Skizzen
- Modelllisten
- Etiketten
- Ladelisten und Versandpapiere

#### Angebotswesen
Für ISO-Positionen im Angebot können mehrere Alternativvorschläge erstellt werden. Mit A+W Business haben Sie folgende Möglichkeiten:
- Für das ganze Angebot ein Alternativangebot erstellen.
- Nur für einige Positionen ein Alternativangebot erstellen.
- Alle Gläser und SZR austauschen.
- Modelle, Sprossen und Bearbeitungen zu Positionen hinzufügen oder ändern.
- Zusätzliche Texte erfassen oder andere Dokumente anhängen.

Wenn der Kunde sich für ein Angebot entschieden hat, können Sie das Angebot in einen Auftrag umwandeln.

#### Einkauf – Anfragen und Bestellungen
Anfragen und Bestellungen werden genau wie Angebote und Aufträge erfasst und bearbeitet. Zusätzlich stehen dabei folgende Funktionen zur Verfügung:
- Lieferterminkontrolle
- Preisvergleich bei mehreren möglichen Lieferanten
- Wareneingangskontrolle
- Mahnung ausstehender Lieferungen
- Preis- und Rechnungskontrolle

### Fertigung
Das Modul Fertigung dient der Datenaufbereitung und Übergabe an die Produktion. Nachdem die Daten übergeben wurden, werden von der Produktion Rückmeldungen an A+W Business gesendet.

A+W Business kann in verschiedenen System-Ausbaustufen verwendet werden:
- **Ausbaustufe 1:** A+W Business + Ankopplung an eine externe Produktionssoftware
- **Ausbaustufe 2:** A+W Business + A+W Business Pro (Produktionsplanung und -steuerung)
- **Ausbaustufe 3:** Ausbaustufe 2 + A+W Business Kapazitätsplanung
- **Ausbaustufe 4:** Ausbaustufe 3 + A+W Business BDE
- **Ausbaustufe 5:** A+W Business + A+W Production
- **Ausbaustufe 6:** Ausbaustufe 5 + A+W Production Kapazitätsplanung
- **Ausbaustufe 7:** Ausbaustufe 6 + A+W Production BDE

Die Wahl der Ausbaustufe hängt von Ihren Anforderungen ab. Die Lösungen bieten die Möglichkeit, langfristig zu wachsen und flexibel die Ausbaustufe zu erhöhen.

#### Datenübergabe und Produktions-Rückmeldungen
Mit Hilfe des ERP-Webservices werden die produktionsrelevanten Daten direkt an die Produktionssoftware A+W Production weitergeleitet und dort eingelesen.

(Abb. A-14 zeigt den Datenfluss: Der Auftrag in A+W Business geht zur Produktionsübergabe an A+W Production. Rückmeldungen aus der Produktion aktualisieren den Status im Auftrag. Bestellungen gehen an den Wareneingang und Tourenplanung an den Versand.)

Über den Auftragsstatus wird die korrekte Abfolge der Buchungen gesichert. Der aktuelle Stand der Produktion wird als Rückmeldung an A+W Business gesendet. Der Status wird pro Auftragsposition und für den gesamten Auftrag umgesetzt. Die Datenerfassung kann über Barcodes erfolgen, um Eingabefehler zu reduzieren.

#### Materialübersicht
Sie können sich pro Liefertermin eine Vorschau auf die Materialmengen anzeigen lassen, die für die Produktion von bestimmten Warengruppen benötigt werden. Mit dieser Übersicht können Sie prüfen, ob die Warenbestände an Rohmaterial ausreichend sind.

> **A+W Business Capacity Planner**
> Für die Planung der Produktionskapazitäten und Liefertermine stehen umfangreiche Funktionalitäten in der A+W Business Capacity Planner zur Verfügung.

#### Angebotsoptimierung
Wenn Sie in einem Angebot seltene Gläser erfasst haben, können Sie das Angebot an die Produktion übergeben, um den Zuschnitt zu planen und so den Glasbedarf und Verschnitt zu ermitteln. Nach der Übergabe der Angebote an A+W Production können Sie die Daten im Hinblick auf Produktionskapazitäten und Materialverbrauch analysieren. Dazu gehören folgende Prüfungen:
- Ist der gewünschte Liefertermin möglich?
- Kalkulation der Material- und Maschinen-Kosten.
- Berechnung der Glasausbeute unter verschiedenen Optimierungsgesichtspunkten.

#### Reservierungsaufträge
Aufträge können an die Produktion übergeben werden, ohne die Fertigung sofort anzustoßen. Diese Funktion wird über den Dokumententyp gesteuert:
- **Kalkulation:** Kalkulation der Material- und Maschinen-Kosten. Der Auftrag wird nicht zur Produktion freigegeben.
- **Reservation:** Reservierung von Kapazitäten. Der Auftrag wird in A+W Production gespeichert, aber nicht zur Produktion freigegeben.

Die so übergebenen Aufträge werden erst produziert, wenn sie als "normaler" Auftrag erneut an die Produktion übergeben werden.

#### A+W Business Pro (Produktionsmanager)
In der Programmversion A+W Business Pro sind der Produktionsmanager und die notwendigen Produktionsstammdaten integriert. Der Produktionsmanager unterstützt Sie im Planungs- und Vorbereitungsprozess für die Produktion, von der Laufbildung bis zum Erzeugen der Maschinencodes.

**Standardprozess für Produktionslösung (Abb. A-17):**
Auftrags-Teileselektion -> Laufbildung -> Abstellplatz-organisation -> Optimierung -> Freigabe

Die Aufträge werden automatisiert oder manuell für die interne Kapazitätsplanung freigegeben. Sie können den Produktionsmanager in zwei Modi nutzen:
- **Standardmodus:** Ein Assistent (Wizard) führt Sie durch den Prozess. Am Ende werden die Optimierungsergebnisse angezeigt.
- **Expertenmodus:** Sie führen die einzelnen Schritte manuell aus und haben detaillierten Einfluss auf die Prozessschritte.

#### Betriebsdatenerfassung (BDE)
Für die Verfolgung des Produktionsfortschritts stehen zwei Lösungen zur Verfügung:
- Die **integrierte BDE-Lösung (optional)** ermöglicht, den Produktionsfortschritt positionsgenau zu verfolgen, indem an Buchungspunkten der Status per Scanner erfasst wird.
- **Alternativ in Kopplung mit A+W Production** können erweiterte Funktionen genutzt werden, z.B. die Anzeige-Leitrechnersysteme von A+W Production Terminal.

Wenn eine Position fertig gemeldet wird, wird der Status der Auftragsposition in A+W Business umgesetzt. Den aktuellen Produktionsstand können Sie im Dialog Statusrückmeldungen prüfen.

(Abb. A-18 zeigt ein BDE-Menü für Wareneingang, Fertigmeldung, Lagerbewegung und Sonderfunktionen.)

#### Lieferwesen
Im Versand organisieren Sie die Auslieferung der Aufträge mit Ihrem eigenen Fuhrpark. Mit der Kommissionierung stellen Sie Touren- und Beladungslisten zusammen, bei denen die Fahrzeuge anhand des zugelassenen Gewichts und der Tour optimal beladen werden können.

#### Routenoptimierung
Der Optimizer for Transport Routes (OTR) bringt Ihre Zielorte in eine sinnvolle und effiziente Reihenfolge. Die Technik basiert auf Nokia Maps und berücksichtigt Streckeneinschränkungen, Gewichtsbeschränkungen und Höhenbeschränkungen. Sie können Routen so zusammenstellen, dass auf Hin- und Rückwegen z. B. Leergestelle mit aufgenommen werden.

**Standardprozess für die Optimierung (Abb. A-20):**
Planung -> Geolocation -> Optimierung -> Ergebnis

- **Planung:** Touren zusammenstellen und Haltepunkte bearbeiten.
- **Geolocation:** Prüfen, ob alle Wegpunkte bei Nokia Maps vorhanden sind.
- **Optimierung:** Die Strecke wird optimiert, mit Möglichkeit zum manuellen Tausch von Stationen.
- **Ergebnis:** Das Gesamtergebnis der Tour wird mit Tourenplan und Liste der Bestimmungsorte angezeigt.

OTR berücksichtigt mehrere LKWs, Fahrzeiten, Stauraum, Anlieferzeiten und Prioritäten, um das beste Ergebnis zu erzielen.

### Kapazitätsplanung
Mit der Kapazitätsplanung können Sie die Auslastung Ihrer Produktionskapazitäten vorplanen und Produktions- und Zeitkosten ermitteln, um Engpässe frühzeitig zu erkennen. Dazu stehen zwei Versionen zur Verfügung:
- **A+W Production Kapazitätsplanung:** Auftragsdaten werden an die Produktion übergeben und dort analysiert.
- **A+W Business Kapazitätsplanung:** Aufträge werden vor der Produktionsübergabe in die Kapazitätsplanung eingelastet (nur in Verbindung mit A+W Business Pro).

#### Hauptmerkmale von A+W Business Kapazitätsplanung
- Flexibles Anlegen der Stammdaten für die Kapazitätsplanung
- Ermittlung von Kapazitätsengpässen
- Prüfung des Liefertermins
- Kalkulation der Produktionskosten
- Leitstand mit Übersichten und Funktionen zum Umlasten

#### Abbildung der Produktionsabläufe
In den A+W Business-Stammdaten sind Basisprodukte (Einfachglas, VSG, ESG etc.) angelegt. Diesen Produkten werden Arbeitsarten und Maschinen zugeordnet, um die Reihenfolge der Produktion festzulegen.

(Abb. A-22 zeigt Beispiele für Zuordnungen von Arbeitsarten wie "Zuschneiden" und "Waschen" zu Produktarten wie "Einfachglas" und "VSG".)

Hierbei wird zwischen expliziten (direkten) und impliziten (indirekten) Zuordnungen unterschieden.

#### Zeit und Kosten pro Aggregat
Zu jedem Aggregat (Maschine) hinterlegen Sie Angaben, aus denen die Kosten für die Maschine und die Zeit errechnet werden. Die Kapazität des Aggregats ergibt sich aus:
- Einheiten pro Stunde
- Anzahl der Stunden pro Schicht
- Anzahl der Schichten, in denen das Aggregat arbeitet.

#### Basiskomponenten der Zeitplanung
In die Planung der Zeit fließen folgende Vorgaben ein:
- **Vorgabezeiten:** Zeit einer Arbeitsart an einer Maschine.
- **Zeitzuschläge:** Erhöhen die Vorgabezeiten unter bestimmten Voraussetzungen.
- **Verweiltage:** Wie lange eine Einheit in einem Produktionsbereich verweilt.
- **Übergangszeiten:** Zeit für den Wechsel zwischen Arbeitsarten oder Produktionsbereichen.
- **Rüstzeiten:** Zeit, um eine Maschine für den nächsten Arbeitsgang einzurichten.

#### Terminberechnung
Ausgangspunkt für die Planung ist der Liefertermin, von dem aus die Arbeitsgänge zurückgerechnet werden.
- **Rückwärtsterminierung:** Die Prüfung der freien Kapazitäten beginnt bei der letzten Arbeitsart vor dem Liefertermin und geht rückwärts.
- **Vorwärtsterminierung:** Wenn die Rückwärtsterminierung nicht erfolgreich ist, sucht das Programm nach einem neuen Liefertermin.

Berücksichtigt werden Fertigungs-, Verweil- und Übergangszeiten.

#### Einlastung der Aufträge in A+W Business Kapazitätsplanung
Die Aufträge werden in einem Workflow-Task kontinuierlich an die Produktion übergeben. Im Leitstand fließen die Daten der eingelasteten Aufträge zusammen, wo Termine und Aggregate geändert werden können.
Nachdem die Daten an die Produktion übergeben wurden, werden von der Produktion Rückmeldungen an A+W Business gesendet. Veränderungen des geplanten Produktionstermins werden automatisch in der Kapazitätsplanung umgebucht.

### Statistiken und Reports
Mit dem A+W Business-Modul Statistik werten Sie folgende Daten aus:
- Aktueller Auftragsbestand, Umsatz-, Reklamations- und Provisionsstatistik
- Über den Gupta-Report-Builder werden die Daten auch in grafischer Form ausgegeben.

#### Crystal Reports
Mit Crystal Reports erstellen Sie Berichte im RPT-Format. Die Ausführung der Reports kann über Mitarbeiterrechte gesteuert werden.

#### A+W Discovery
A+W Discovery ist das moderne Business Intelligence System der A+W Software GmbH. Es erlaubt, statistische Kennzahlen und Messgrößen aus verschiedenen Blickrichtungen zu betrachten, um strategische, kaufmännische oder produktionstechnische Entscheidungen abzuleiten. Sie können z. B. Daten zum Deckungsbeitrag und Umsatzvolumen von Standorten erheben. Über vordefinierte A+W Standard-Reports können ERP- und PPS-Daten aggregiert werden.

#### A+W Dashboard
A+W Dashboard ist ein Service mit einer Web-basierten Oberfläche, um KPI-Daten aus der Produktion anzuzeigen. Es ist ein Tool zur Visualisierung der Produktion und zeigt die aktuelle Leistung von Maschinen und Mitarbeitern in grafischer Form.
> **Korrekte Darstellung nur mit korrekten BDE-Buchungen**
> Voraussetzung für aussagekräftige Anzeigen sind lückenlose BDE-Buchungen.

### Lagerverwaltung
Im Modul Lagerwirtschaft von A+W Business können Sie Bandmaße, Lagermaße, Restblätter, Kisten, Beschläge etc. verwalten. Sie können die Lagerorganisation Ihres Unternehmens im Programm abbilden, indem Sie Standorte, Gänge, Regale und Fächer definieren.

**Abläufe in der Lagerwirtschaft (Abb. A-1):**
- **Auftrag:** Ein Kundenauftrag führt zur Reservierung von Lagerartikeln.
- **Übergabe Produktion:** Die benötigten Materialien werden reserviert und bei der Lieferung ausgebucht.
- **Lagerbestellung:** Bei Unterschreitung des Mindestbestands wird eine Bestellung an den Einkauf übergeben.
- **Lagerzugang:** Bei Wareneingang wird der Lagerbestand aktualisiert.
- **Inventur:** Bereinigung der Bestandszahlen.

#### Lagerinfo – Zukünftiger Lagerbestand
Schon bei der Erfassung von Auftragspositionen prüfen Sie, ob der aktuelle Bestand ausreicht, um gesicherte Terminzusagen zu machen. Die Vorschau des zukünftigen Lagerbestands zeigt den Bestand, Reservierungen und Bestellungen für einen definierbaren Zeitraum.

#### Lagerabfrage
Mit verschiedenen Abfragen können Sie sich einen Überblick verschaffen:
- **Buchungsjournal:** Auswertungen zu Lagerbuchungen.
- **Lagerhistorie:** Überblick über das Tagesgeschehen im Lager pro Produkt.
- **Lagerstatistik:** Gibt Aufschluss über Renner und Ladenhüter.
- **Lagerbewertung:** Der aktuelle Lagerwert des gesamten Lagers.
- **Reservierte Lagerartikel:** Listet Artikel auf, die durch Aufträge reserviert sind.

#### Inventur
Die Inventur stellt den Bestand des Vorratsvermögens nach Art, Menge und Wert fest. Für die Jahresinventur werden Inventurlisten erstellt. Die Inventur kann in Etappen und mit Hilfe von Barcode-Lesung durchgeführt werden. Mit dem Inventurabschluss werden die Bestandsmengen in A+W Business aktualisiert.

## Arbeit mit A+W Business
Durch die intuitive grafische Bedienoberfläche (GUI) ist die Arbeit mit A+W Business schnell und leicht zu erlernen.

### A+W Business starten und beenden
A+W Business kann auf verschiedene Arten gestartet werden:
1.  Wählen Sie **[Start] > Alle Programme > A+W > A+W Business**.
    oder
2.  Klicken Sie (doppelt) auf die Verknüpfung auf dem Desktop.

Wenn der Programmstart nicht an die Windows-Anmeldung gekoppelt ist, wird der Dialog **Datenbank Login** angezeigt.
1.  Geben Sie Ihren Benutzernamen und das Passwort ein.
2.  Klicken Sie auf **[OK]** um das Programm zu starten.

Um A+W Business zu beenden, klicken Sie in das Symbol **Schließen** (X) rechts oben im Programm-Fenster.

### Elemente des Programmfensters
Das Programmfenster ist in folgende Bereiche aufgeteilt:
- **A Multifunktionsleiste:** Anzeige der Menüs und Schaltflächen zum aktiven Dialog.
- **B Navigationsleiste:** Anzeige der Module. Mit einem Klick öffnen Sie das Modul, mit einem Doppelklick den Dialog.
- **C Bearbeitungsbereich:** Anzeige der Dialoge.

### Standard-Menüs
- **Start:** Schaltflächen zum Navigieren zwischen Datensätzen und Starten von Aktionen.
- **Funktionen:** Andere Dialoge öffnen, ohne den aktuellen zu schließen.
- **Optionen:** Standardeinstellungen des aktuellen Dialoges bestimmen.
- **Druck:** Ausgabe einer Liste oder Auswertung starten.
- **Kommunikation:** E-Mail oder Fax versenden.

### Standard-Schaltflächen
Die folgenden Schaltflächen werden angezeigt, wenn Sie einen Dialog geöffnet haben.

| Symbol | Funktion | Hotkey |
| :--- | :--- | :--- |
| **X** (Schließen) | Aktiven Dialog schließen. | `<Esc>` |
| **?** (Hilfe) | Online-Hilfe öffnen. | `<F1>` |
| **i** (Über) | Programminformationen anzeigen. | - |
| **<<** (Erster) | Ersten Datensatz einer Tabelle anzeigen. | `<F5>` |
| **<** (Vorheriger) | Vorherigen Datensatz einer Tabelle anzeigen. | `<F6>` |
| **>** (Nächster) | Nächsten Datensatz einer Tabelle anzeigen. | `<F7>` |
| **>>** (Letzter) | Letzten Datensatz einer Tabelle anzeigen. | `<F8>` |
| Filter | In den Suchmodus (QBE-Modus) wechseln. | `<Strg>+<A>` |
| Suchen | Suche starten. | `<Enter>` |
| Neu | Neuen Datensatz anlegen. | `<Strg>+<N>` |
| **X** (Löschen) | Aktuellen Datensatz löschen. | `<Strg>+<L>` |
| Speichern | Neuen Datensatz oder Änderungen speichern. | `<Strg>+<S>` |
| Ausführen | Aktion starten. | `<Enter>` |

### Hotkeys in der Dokumentenerfassung
Für die Erfassung von Dokumenten und Positionen stehen folgende Tastenkombinationen (Hotkeys) zur Verfügung.

#### Allgemeine Funktionen

| Funktion | Hotkey |
| :--- | :--- |
| Dokument anzeigen | `<Shift>+<Ctrl>+<D>` |
| E-Mail senden | `<Ctrl>+<M>` |
| Erster Datensatz | `<F5>` |
| Faxnachricht senden | `<Ctrl>+<F>` |
| Fenster schließen | `<Esc>` |
| Filterkriterien | `<Ctrl>+<A>` |
| Kundeninfo | `<Shift>+<Ctrl>+<C>` |
| Letzter Datensatz | `<F8>` |
| Löschen | `<Ctrl>+<L>` |
| Nächster Datensatz | `<F7>` |
| Neuen Datensatz anlegen | `<Ctrl>+<N>` |
| Online-Hilfe öffnen | `<F1>` |
| Produktionsübersicht | `<Ctrl>+<B>` |
| Speichern | `<Ctrl>+<S>` |
| Vorheriger Datensatz | `<F6>` |

#### Dokumentenkopf

| Funktion | Hotkey |
| :--- | :--- |
| Alternativangebotsübersicht | `<Ctrl>+<F>` |
| Anschrift ändern | `<F11>` |
| Anzahlungsübersicht | `<Ctrl>+<A>` |
| Artikel info | `<Shift>+<Ctrl>+<I>` |
| Auftrags-/Bestell-Info | `<Ctrl>+<I>` |
| Dokumentendaten | `<Shift>+<Ctrl>+<F12>` |
| Duplikate anzeigen | `<Shift>+<Ctrl>+<D>` |
| Historie | `<Ctrl>+<H>` |
| Kalkulatorische Frachtkosten | `<Ctrl>+<K>` |
| Kosten- und Aufschlagskalkulation | `<Ctrl>+<U>` |
| Lagersuche | `<Shift>+<Ctrl>+<F11>` |
| Lagervorschau | `<Shift>+<Ctrl>+<S>` |
| OP Abfrage | `<Ctrl>+<O>` |
| Positionserfassung | `<F9>` |
| Produktionsübersicht | `<Ctrl>+<B>` |
| Reklamationsübersicht | `<Ctrl>+<G>` |
| Teillieferungsübersicht | `<Ctrl>+<T>` |

#### Positionen

| Funktion | Hotkey |
| :--- | :--- |
| **Allgemein** | |
| Artikel Info | `<Shift>+<Ctrl>+<I>` |
| Bearbeitungserfassung | `<F11>` |
| Begründung für manuelle Preisvorgaben | `<Shift>+<Ctrl>+<F11>` |
| Gesperrte Position ändern | `<Shift>+<F12>` |
| Keine Rückrechnung der automatischen Zuschläge | `<Shift>+<Ctrl>+<O>` |
| Konditionen / Individuelle Preise | `<Shift>+<Ctrl>+<K>` |
| Kopie aus Position | `<Shift>+<Ctrl>+<Y>` |
| **Aufbau** | |
| Struktur 1. Scheibe drehen | `<Shift>+<F1>` |
| Struktur 2. Scheibe drehen | `<Shift>+<F2>` |
| Struktur 3. Scheibe drehen | `<Shift>+<F3>` |
| Beschichtung 1. Scheibe drehen | `<Ctrl>+<F1>` |
| Beschichtung 2. Scheibe drehen | `<Ctrl>+<F2>` |
| Beschichtung 3. Scheibe drehen | `<Ctrl>+<F3>` |
| Makro- Suche für Aufbau | `<Ctrl>+<Y>` |
| **Kosten- und Aufschlagskalkulation** | |
| Übersicht | `<Ctrl>+<U>` |
| Detail - Position | `<Ctrl>+<P>` |
| **Stückliste** | |
| Detail - Stückliste | `<Ctrl>+<D>` |
| Löschen und neu berechnen | `<Ctrl>+<U>` |
| **Weitere Funktionen** | |
| Lagersuche | `<F3>` |
| Mengeneingaben für aktuelle Position | `<Ctrl>+<Q>` |
| Modellerfassung | `<F9>` |
| Neue Position | `<Ctrl>+<N>` |
| Preisanzeige umschalten: EK, VK, FW, Euro | `<F2>` |
| Preisberechnung starten | `<Ctrl>+<Y>` |
| Preisrekorder | `<Shift>+<Ctrl>+<F10>` |
| Preisvorgaben auf nachfolgende Positionen übertragen | `<Shift>+<Ctrl>+<T>` |
| Produktionsübersicht | `<Ctrl>+<B>` |
| Reklamation | `<Shift>+<Ctrl>+<R>` |
| Schnellanfrage | `<Shift>+<Ctrl>+<S>` |
| SN Editor | `<F4>` |
| Sprossenerfassung | `<F10>` |
| **Sprossen** | |
| Bohrpunktsymmetrisch | `<Ctrl>+<Q>` |
| Feldsymmetrisch | `<Ctrl>+<W>` |
| Bohrpunkt-asymmetrisch | `<Ctrl>+<E>` |
| Feld-asymmetrisch | `<Ctrl>+<R>` |
| **Sonstiges** | |
| Versicherungspreise | `<F12>` |
| Vorgaben Position löschen | `<Shift>+<Ctrl>+<V>` |
| Vorgaben Positionspreis löschen | `<Shift>+<Ctrl>+<P>` |
| Vorgaben Stücklistenposition löschen | `<Shift>+<Ctrl>+<L>` |

### Dokumentation
Die Module und Prozesse von A+W Business sind jeweils in separaten Dokumenten beschrieben. Zu jedem dieser Parts gehören Schulungsunterlagen (Tutorials) und die Software-Referenzen:
- In den **Tutorials** werden die Funktionen der Software beschrieben.
- In der **Online-Hilfe** werden die Dialoge des Programms ausführlich beschrieben.
- Zusätzlich steht Ihnen die ausführliche **Datenbank-Dokumentation** zur Verfügung, z. B. zur Erstellung von Abfragen und Reports.

#### Online-Hilfe
Die A+W Business Online-Hilfe kann auf folgende Weise geöffnet werden:
- Schaltfläche [Hilfe]
- Taste `<F1>`

Die Online-Hilfe wird kontext-sensitiv geöffnet, also genau zu dem Dialog, den Sie aktuell geöffnet haben. Über die Register haben Sie verschiedene Möglichkeiten, nach Informationen zu suchen:
- **Inhalt:** Die einzelnen Parts werden als Navigationsbaum angezeigt.
- **Index:** Die Indexeinträge werden alphabetisch angezeigt.
- **Suche:** Über die Volltextsuche werden alle Themen gefunden.
- **Favoriten:** Hier können Sie Verknüpfungen zu Themen anlegen, die Sie häufiger benötigen.
