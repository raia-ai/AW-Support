---
title: "DE_AWEnterprise_Ueberblick"
source: "DE_AWEnterprise_Ueberblick.pdf"
tags: ["A+W Enterprise", "ERP-System", "Flachglas", "Software", "Benutzerhandbuch", "Glasindustrie", "Fenster", "Türen", "Stammdaten", "Unternehmensprozesse"]
version: "1.0"
last_updated: "2025-10-03"
short_description: "This document provides a comprehensive overview of the A+W Enterprise ERP system, a software solution designed for the flat glass processing industry. It covers the system's architecture, key features, and modular structure, tailored for businesses ranging from glass traders to large corporate enterprises."
long_description: "This document, titled \"A+W Enterprise Überblick,\" serves as a detailed guide and tutorial for the A+W Enterprise software. A+W Enterprise is a fully integrated, multi-client capable ERP system for corporations and large medium-sized companies in the flat glass processing industry. The guide begins with an editorial section, revision history, and contact information. It then transitions into a detailed tutorial covering the system's core functionalities, including an introduction to the product, its benefits compared to A+W Business, and its specific applications for glass trading, glassworks, ISO/ESG/VSG manufacturers, and corporate structures. The document provides fundamental knowledge for working with the software, detailing user interface operations, dialogs, master data management (for market partners, articles, bills of materials), and supported business processes like sales, purchasing, production, logistics, and management. It concludes with an overview of the system's modules and information on using the online help. The guide is intended for end-users to gain a thorough understanding of the system's architecture and capabilities."
---

# A+W Überblick

---
## Vorspann

In diesem Teil der Dokumentation finden Sie editorische Notizen.

### Revisionsübersicht

| Part Version / Datum | Beschreibung |
| :--- | :--- |
| 1.00/10-2006 | Ersterstellung. |
| 1.01/02-2014 | Anpassung an neues CI. |
| 1.02/01-2017 | Produkt- und Firmennamen angepasst. |

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

### Urheberrechte
© 2017, A+W Software GmbH, alle Rechte, auch des Nachdrucks, der Herstellung von Kopien und der Übersetzung, bleiben vorbehalten.

Die Dokumentation darf nur gemäß dem Lizenzvertrag ganz oder in Teilen kopiert, in einem Archivierungssystem gespeichert oder in irgendeiner anderen Form übertragen werden. Ohne die vorherige schriftliche Genehmigung der A+W Software GmbH darf die Dokumentation weder elektronisch, mechanisch, per Aufzeichnung oder in sonstiger Form übertragen werden.

### Warenzeichen
Alle in der Dokumentation erwähnten Hard- und Softwarebezeichnungen können gleichzeitig auch eingetragene Marken oder sonstige gewerbliche Schutzrechte Dritter sein. Die Schutzrechte Dritter sind insoweit zu beachten.

### Kontakte
**A+W Software GmbH**

Am Pfahlgraben 4-10
35415 Pohlheim

- **Telefon:** +49 6404 2051-0
- **Fax:** +49 6404 2051 877
- **E-Mail:** Zentrale@a-w.com
- **Web:** http://www.a-w.com

## Tutorial

### Überblick

A+W Enterprise ist ein voll integriertes, mehrmandantenfähiges ERP-System für Konzerne und gehobene Mittelstandsunternehmen der Flachglas verarbeitenden Industrie.

Das Gesamtsystem umfasst die Bereiche Verkaufsmanagement, Vertriebsunterstützung, Einkaufsmanagement, Lagerführung und Versandplanung.

A+W Enterprise gliedert sich in drei Architekturschichten: Präsentation, Anwendungslogik und Datenbank. Diese können auf unterschiedlichen Rechnern installiert und betrieben werden. Dies erhöht die Skalierbarkeit und Ausfallsicherheit des Systems. Die Anwendung stützt sich auf eine relationale Datenbank und ist als LINUX-/ UNIX-Version verfügbar. Das Benutzer- Frontend kann auf MS Windows installiert werden.

A+W Enterprise kann in der gesamte Glasbranche vom typischen Handelsbetrieb über den ISO-, ESG- oder VSG-Produzenten bis hin zum konzernartigen Unternehmensverbund eingesetzt werden.

Ein gutes Verständnis für die Systemarchitektur und den modularen Aufbau von A+W Enterprise sind die Grundvoraussetzung für die Handhabung und Bedienung der einzelnen Bereiche und den hierfür notwendigen Wissenserwerb.

#### Themenblöcke
In diesem Tutorial finden Sie folgende Themenblöcke:
- A+W Enterprise stellt sich vor
- Grundlagen zur Arbeit mit A+W Enterprise
- Unterstützte Unternehmensprozesse

> **Vorausgesetzte Kenntnisse**
> EDV-Grundkenntnisse bzw. Windows-Kenntnisse werden bei den Anwendung von A+W Enterprise vorausgesetzt.

#### Aufbau des Tutorials
Dieses Tutorial besteht aus Themenblöcken mit jeweils mehreren Lerneinheiten. Jede Lerneinheit besteht aus folgenden Komponenten:

- **Überblick**
  Jede Lerneinheit beginnt mit einem Überblick über die wichtigsten Inhalte:
  - **Lernziele:** Was soll vermittelt werden?
  - **Nutzen:** Wofür können Sie dieses Wissen einsetzen?
  - **Merksätze:** Welche Zusammenhänge müssen Sie sich merken?

- **Konzepte**
  Konzepte und Begriffe der jeweiligen Lerneinheit werden zunächst erläutert. Danach finden Sie Beispiele und Handlungsanleitungen.

- **Übungen**
  Zu einigen Lerneinheiten finden Sie Übungen mit Aufgabenstellungen und Lösungsvorschlägen. Die Übungen helfen Ihnen A+W Enterprise zu verstehen und anwenden zu lernen.

- **Querverweisteil**
  Am Ende jeder Lerneinheit finden Sie einen Abschnitt mit Querverweisen, die auf entsprechende Beschreibungen in der Softwarereferenz hinweisen. Damit können Sie das neu erworbene Wissen vertiefen.

> **Lesehinweis**
> Der Inhalt einer Lerneinheit baut auf den Kenntnissen auf, die in der vorausgegangenen Einheit vermittelt wurden. Es ist daher sinnvoll, keine Lerneinheiten zu überspringen.
> Sollten Sie mit einem Thema bereits vertraut sein, lesen Sie mindestens die Zusammenfassung am Beginn der Lerneinheit, um sich die wichtigsten Details zu vergegenwärtigen.
> Im Praxisteil jeder Schulungseinheit werden die Softwarereferenz und der Übungsteil über Querverweise systematisch einbezogen. Dadurch entsteht ein roter Faden durch die gesamte Dokumentation.

#### Darstellungskonventionen
Einzelne Satzteile werden in besonderer Form dargestellt. Diese haben folgende Bedeutung:

| Format | Bedeutung |
| :--- | :--- |
| *Kursiv* | sind Zeichenfolgen ausgezeichnet, die Elemente der Software bezeichnen, z. B. der Dialog *Muster senkrecht/waagerecht*. |
| **Fett** | sind Zeichenfolgen ausgezeichnet, die Sie über die Tastatur eingeben, z. B. geben Sie den Wert **0** ein. |
| > | Mit dem sogenannten Brotkrumenpfad ist der Weg gekennzeichnet, auf dem Sie einen Dialog öffnen, z. B. Datei > Importieren > Übergabedatei. |
| [] | Eckige Klammern bezeichnen Schaltflächen im Dialog, z. B, mit [OK] speichern Sie die Daten. |
| <> | Spitze Klammern bezeichnen Tasten oder Tastenkombinationen auf der Tastatur, z. B. mit `<F1>` öffnen Sie die Online-Hilfe. |

### A+W Enterprise stellt sich vor

Diese Einführung vermittelt Ihnen einen Überblick über A+W Enterprise. A+W Enterprise ist eine ERP-Softwarelösung für die flachglasverarbeitende Industrie.

Nachdem das Programm kurz beschrieben und auf seine Vorteile hingewiesen wird, wird im folgenden Abschnitt das Leistungsspektrum von A+W Enterprise dargestellt. Es wird skizziert, welche Unternehmen mit welchen Unternehmensstrukturen und mit welchen Tätigkeitsfeldern A+W Enterprise unterstützt.

Nach der allgemeinen Übersicht wird auf die Bedienung von A+W Enterprise mit seinen Besonderheiten eingegangen. Eine bedeutende Rolle spielt hier die Bedienung mit der Tastatur. Es stehen viele Tastaturbefehle zur Verfügung, die ein schnelles und effizientes Arbeiten ermöglichen.

Im Weiteren wird auf einige der Stammdaten eingegangen. Hier werden die Daten zu den Bereichen Marktpartner, Artikel, Stückliste, Warengruppe und Preise/Konditionen gepflegt. Alle Geschäftsbereiche (Verkauf, Einkauf, Produktion, Lager, Versand) greifen auf diese Daten zu. Sie bilden somit die Grundlage des Programmes.

Im Anschluss werden die Unternehmensprozesse die A+W Enterprise unterstützt beschrieben. Es sind viele Unternehmensprozesse in A+W Enterprise integriert und auch automatisiert. Damit entfallen die Überwachung und das Anstoßen einzelner Workflows.

Weiterführende Informationen zu A+W Enterprise finden Sie im A+W Enterprise Handbuch, in der A+W Enterprise Produktbeschreibung sowie in der Online-Hilfe.

#### A+W Enterprise Produktbeschreibung
A+W Enterprise ist ein datenbankgestütztes ERP-System (Enterprise-Resource-Planning), das sämtliche Prozesse eines flachglasveredelnden oder -produzierenden Betriebes unterstützt. A+W Enterprise kann in der gesamten Glasbranche eingesetzt werden, beginnend beim typischen Handelsbetrieb über den ISO-, ESG- oder VSG-Produzenten bis hin zum konzernartigen Unternehmensverbund.

A+W Enterprise ist eine umfassende Lösung für die Bereiche:
- Angebotswesen
- Auftragsbearbeitung
- Fakturierung
- Disposition
- Produktionsplanung und -steuerung (in Verbindung mit A+W Production)
- Bestellwesen und Einkauf
- Versandsteuerung
- Lager
- EDI und eCommerce
- Objektverwaltung
- A+W Rack Manager

Über die operativen Module hinaus stellt A+W Enterprise eine Vielzahl von Statistiken, Auswertungen und Informationssystemen zur Verfügung. Ebenfalls werden Schnittstellen zu externen Analysetools und Software bereitgestellt. Dadurch ist auch die Auswertung und Analyse mit Standardsoftware jederzeit möglich.

Welche Funktionen und Funktionalitäten im Einzelnen zur Verfügung stehen, hängt von der individuellen Konfiguration des A+W Enterprise-Systems ab. Zusätzliche Module können problemlos jederzeit nachträglich integriert werden. A+W Enterprise kann als kleines, schlankes System beginnen und es kann nach und nach zum Vollsystem ausgebaut werden.

#### Produktportfolio
In dieser Abbildung wird A+W Enterprise als ERP-System zu Beginn des Geschäftsprozesses im gesamten Unternehmensprozess dargestellt.

> **Diagramm: A+W Software GmbH Produktportfolio**
>
> Das Diagramm zeigt den Unternehmensprozess, der in mehrere Hauptkategorien unterteilt ist:
>
> 1.  **ERP (Enterprise Resource Planning)**
>     - ERP Solution: A+W Enterprise, A+W Business
>     - Bereiche: Verkauf, Einkauf, Lager, Versand, Statistik, eCommerce
> 2.  **PPS (Produktionsplanungs- und Steuerungssystem)**
>     - PPS Solution: A+W Production
>     - Bereiche: Kapazitätsplanung, Produktionsplanung (Grob- und Feinplanung), Verschnittoptimierung
> 3.  **Maschinensteuerung**
>     - Control Units: Production Terminal, Realtime Optimizer, Rack Optimizer, Dynopt
>     - Bereiche: Monitoring, Barcoding
> 4.  **Maschinen**
>     - Beispiele: ISO Linie, Zuschnittslinie, VSG Linie
> 5.  **Produktionsmonitoring**
>     - Controlling & Monitoring: A+W Dashboard, A+W Capa View
>
> Übergreifende Werkzeuge sind:
> - **CAD Konstruktion**: CAD Designer
> - **Statistik & Analyse**: A+W Analytics

#### Benefit von A+W Enterprise in Abgrenzung zu A+W Business
Im Hause der A+W Software GmbH gibt es zwei kaufmännische Softwarelösungen: A+W Enterprise und A+W Business. Beide Systeme sind auf die Flachglasindustrie ausgerichtet und erfüllen deren Anforderungen im kaufmännisch-administrativen Bereich in sehr guter Weise. Abhängig von der Unternehmensgröße und -struktur empfiehlt sich jedoch in einem Fall mehr die A+W Business- im anderen Fall die A+W Enterprise-Lösung.

Größere Unternehmen mit einer ausgeprägten Niederlassungsstruktur profitieren in der Regel eher von der Architektur des A+W Enterprise Systems. Für Einzelbetriebe oder Unternehmensgruppen, die wie Einzelbetriebe agieren, empfiehlt sich hingegen oft die A+W Business Lösung.

Unternehmen die eine integrierte und ggf. automatisierte Prozessverarbeitung wünschen, sind mit A+W Enterprise besser bedient, während sich für Betriebe die einen vom Benutzer getriebenen Workflow präferieren das A+W Business System besser eignet.

#### Leistungsmerkmale
In diesem Themenblock lernen Sie den Aufbau und das Systemumfeld von A+W Enterprise kennen.
- Skalierung - modularer Aufbau
- Glashandel
- Glashütten
- ISO-, ESG- oder VSG-Hersteller
- Konzernartige Unternehmen

> **Lernziele**
> - Unterschiedliche Unternehmensziele und -strukturen aus der Glasbranche kennenlernen und wissen wie A+W Enterprise diese mit seinem modularen Aufbau unterstützt
> - Das Softwarekonzept mit seiner Systemarchitektur kennenlernen
>
> **Nutzen**
> Ein gutes Verständnis für die Systemarchitektur und den modularen Aufbau von A+W Enterprise sind die Grundvoraussetzung für die Handhabung und Bedienung der einzelnen Bereiche und den hierfür notwendigen Wissenserwerb.
>
> **Definitionen**
> - **Bestellkopplung**: vollautomatische Handling von gruppeninternen Bestellungen zwischen verschiedenen A+W Enterprise Systemen (Mandanten). Änderungen werden bis zum Zeitpunkt des Sperrens automatisch über alle betroffenen Mandanten positionsgenau verbucht.
>
> **Merke**
> - **Skalierbarkeit**: A+W Enterprise besitzt durch seinen modularen Aufbau und seiner Systemarchitektur eine hohe Skalierbarkeit. Dadurch kann sich A+W Enterprise den sich ändernden Anforderungen an die Performance sowie an die Komplexität des Systems anpassen.
> - **Glashandelsbetriebe**: sind Unternehmen, die ESG, VSG und Isolierglas zukaufen und Zuschnitt sowie kleine Bearbeitungen selber durchführen. A+W Enterprise unterstütz hauptsächlich den kaufmännischen Ablauf des Betriebes.
> - **ISO-, ESG- oder VSG-Hersteller mit Glashandelshaus**: sind Unternehmen, die neben dem Handel zusätzlich Funktionsgläser produzieren. Diese Unternehmensart nutzt die kaufmännischen Funktionen aus A+W Enterprise und die Funktionalität des Produktionsplanungs- und Steuerungssystem A+W Production.

> **Merke**
> - **Konzernartige Unternehmen**: sind Unternehmen in einem losen oder streng organisierten Verbund.
> - **Glashütten**: produzieren kontinuierlich und endlos Floatglas.
> - **Systemumfeld**: Das auf Unix basierende A+W Enterprise besitzt eine grafische Benutzeroberfläche und kann aufgrund der Client-Server-Architektur (3-Tier-Modell) den betrieblichen Erfordernissen schrittweise angepasst und jederzeit erweitert werden.

##### Skalierung - modularer Aufbau
Moderne Softwarepakete zeichnen sich durch eine tragfähige Systemarchitektur und fundierte fachliche Branchenkenntnisse aus.

A+W Enterprise ist durchgängig skalierbar. Das bedeutet, A+W Enterprise kann sehr genau auf die Anforderungen und die jeweilige Unternehmensgröße der Betriebe angepasst werden. Der modulare Aufbau des Systems erlaubt es, bestimmte Bausteine erst in einem späteren Projektabschnitt zu aktivieren.

So werden Glashändler, ISO-, ESG-, oder VSG-Produzenten und konzernartige Glasunternehmen in ihren jeweiligen Strukturen und Geschäftsprozessen optimal unterstützt.

> **Diagramm: A+W Enterprise für verschiedene Unternehmensgrößen**
>
> Das Diagramm zeigt drei Konfigurationen, die die Skalierbarkeit von A+W Enterprise demonstrieren:
>
> 1.  **Kleinere Konfiguration (z.B. Glashandel):**
>     - **A+W Enterprise** Kernmodule: Verkauf, Versand, Lager, Einkauf.
>     - Anbindung an [Fremdsysteme] möglich.
> 2.  **Mittlere Konfiguration (z.B. mit Produktion):**
>     - **A+W Enterprise** Kernmodule + **A+W Production**.
>     - Zusätzliche Module: [Management].
>     - Anbindung an [Fremdsysteme].
> 3.  **Große Konfiguration (z.B. Konzern):**
>     - **A+W Enterprise** Kernmodule + **A+W Production**.
>     - Zusätzliche Module: [Vertrieb], [Management].
>     - Anbindung an [Fremdsysteme].

Durch genaue Analyse der betrieblichen Situation und der daraus resultierenden Auswahl geeigneter Funktionen und Module kann mit A+W Enterprise eine Applikation konfektioniert werden, die sich an die unterschiedlichsten Unternehmensstrukturen flexibel anpasst - egal ob Handelsbetrieb, und ISO-ESG-, VSG-Hersteller oder großer integrierter Konzern.

##### Glashandel
Unter Handelsbetrieben verstehen wir Unternehmen, in denen ESG, VSG und Isolierglas zugekauft, Zuschnitte und einfache Bearbeitungen jedoch selbst durchführt werden.

In diesem Unternehmen bedeutet der Einsatz von A+W Enterprise und von weiteren A+W Produkten eine starke Unterstützung für die Bereiche Einkauf, Verkauf, Vorgangsverfolgung und Fakturierung. Für die Angebotsbearbeitung stehen komfortable Funktionen zur Bildung von Alternativangeboten, übergreifendem Produktaustausch und gezielter Neukalkulation zur Verfügung. Diese beinhalten:
- Vorgangserfassung
- Eingangs- und Ausgangsschnittstellen
- Zuschnittsoptimierung
- Lagerverwaltung
- Versandsteuerung
- Management-Informations-System (MIS)
- Anbindung von Verkaufsniederlassungen
- Workflow-Unterstützung

**Vorgangserfassung**
Bei immer kürzer werdenden Lieferfristen zum Kunden ist es von entscheidender Bedeutung, eingehende Aufträge schnell und einfach abzuwickeln. Aus diesem Grund unterstützt A+W Enterprise Ihre Vorgangserfassung mit Produkt- und Modellabbildungen, Auswahldialogen, Vorgabewerten und diversen technischen und logischen Plausibilitätsprüfungen. Der große Variantenreichtum, aufgrund unterschiedlicher Bearbeitungen, und die vielfältigen Kombinationsmöglichkeiten im Isolierglasbereich werden über eine Stücklistenbeschreibung sehr einfach abgebildet.

**Eingangs- und Ausgangsschnittstellen**
Neben der manuellen Erfassung bietet A+W Enterprise auch verschiedene Auftragseingangsschnittstellen, um Kundenaufträge direkt aus deren EDV-System zu übernehmen. Damit werden Erfassungszeiten und etwaige Eingabefehler deutlich vermindert, die Kundenbindung dagegen erhöht. Dabei A+W Enterprise stehen Innen beispielsweise A+W Standardschnittstelle oder A+W Cantor-Professional von A+W Software GmbH, zur Verfügung.
A+W Cantor-Professional ist eine vollständig grafische Softwarelösung für Fensterproduzenten und -händler aller Größenordnungen. Somit kann die Prozesskette Glashersteller-> Glasveredler -> Fensterproduzent vollständig durch Systemsoftware von A+W Software GmbH abgebildet werden.

Auch ein lieferantenseitiger Datentransfer kann mit A+W Enterprise erreicht werden. Unter der Voraussetzung, dass sich beim jeweiligen Lieferanten ebenfalls ein A+W Enterprise-System im Einsatz befindet, können auf bequeme Art und Weise Preisinformationen, Anfragen oder Bestellaufträge online übertragen werden.

Eine weitere Möglichkeit, die Kommunikation mit Kunden und Lieferanten zu beschleunigen, besteht in der integrierten Fax- oder E-Mail-Anbindung, die es Ihnen erlaubt, Angebote, Aufträge oder Bestellungen in höchster Qualität direkt aus der Anwendung zu erstellen und an die Kunden zu versenden.

**Lagerverwaltung**
Je nach Größe und Komplexität des Glashandelsbetriebes kann in einer weiteren Ausbaustufe das Lagerverwaltungsmodul eingesetzt werden. Es erlaubt die Lagerführung aller Gläser im Unternehmen und kann zusätzlich für Beschläge und sonstige Zubehörartikel eingesetzt werden.

**Versandsteuerung**
Zur Versandunterstützung steht Ihnen das A+W Enterprise-Versandplanungs- und Steuerungssystem zur Verfügung. Dieses Modul verschafft dem Touren-disponenten jederzeit detaillierte Informationen über geplante Touren, Mengen, Tonnagen und die dazu benötigten Transportmittel. Der Disponent kann auf jeder Ebene des Systems ganze Touren, einzelne Aufträge oder Teilpositionen verschieben bzw. stornieren. Auch die augenblicklich verfügbaren Einheiten werden dargestellt, und über eine Fehlmengenkontrolle können Rückstands- oder Bruchpositionen auf zukünftige Touren verschoben werden.

**Management-Informations-System (MIS)**
Zur Steuerung der Marktaktivitäten nutzt der Glashandel die vielfältigen Möglichkeiten des Management-Informations-Systems. Neben diversen vordefinierten Statistiken steht Ihnen als Anwender auch die freie SQL-Schnittstelle zur Formulierung eigener Abfragen zur Verfügung. Damit erhalten Sie wertvolle Informationen über die augenblickliche Marktsituation, das Kundenverhalten oder über die Entwicklung des Unternehmens. Mithilfe des integrierten Reportgenerators können alle Listen in individuellem Format ausgegeben werden.

**Anbindung von Verkaufsniederlassungen**
Nehmen wir an, dass unsere Glashandlung zur Verbesserung ihrer Marktpräsenz ein Verkaufsbüro in einer nahe gelegenen Kleinstadt eröffnet. Auch dort wird zur Abwicklung des Verkaufs eine geeignete EDV-Unterstützung benötigt. Die Vernetzungsmöglichkeiten erlauben es in diesem Fall, die Arbeitsplätze in der Filiale direkt an den im Firmenstammsitz befindlichen A+W Enterprise-Server zu koppeln.

Um die Filiale als separates Profitcenter zu führen, kann auch ein eigenständiges Filialsystem aufgebaut werden, das ebenfalls mit dem Hauptsitz verbunden ist. In diesem Fall sind beide Mandanten einzeln bewertbar, jedoch über eine automatische Vorgangsübertragung miteinander gekoppelt.

**Workflow-Unterstützung**
A+W Enterprise beinhaltet ein leistungsfähiges personen- und vorgangsbezogenes Wiedervorlagesystem mit periodischer und freier Vorlage. Mithilfe eines integrierten Mitteilungssystems können Nachrichten personen- oder abteilungsgenau eingestellt werden, die selbst bei Abwesenheit der entsprechenden Personen nicht verloren gehen können. Des Weiteren sorgt ein prioritätsgesteuertes Anmerkungssystem dafür, dass wichtige Informationen über Kunden, Lieferanten, Artikel, etc. arbeitsplatzbezogen präsentiert werden.

> **Hinweis**
> Management-System, Vertrieb und weitere Fremdsysteme: Teile der A+W Enterprise - Programm sind mit der Zeit weniger bzw., gar nicht mehr in der Benutzung. Bei eventuell entstehenden Fragen wenden Sie sich an zuständigen A+W - Mitarbeiter.

##### Glashütten
Eine Glashütte ist eine Produktionsstätte, in der endlos und kontinuierlich Floatglas hergestellt wird. Alle produzierten Gläser werden auf Stapeln gelagert. Diese Stapel werden in A+W Enterprise abgebildet. Somit ist ein Stapel das zentrale und durchgängige Objekt in A+W Enterprise.

Die Module Lager und Versand unterstützen Glashütten mit einer besonderen Ausprägung. Bei dieser Konfiguration besitzt A+W Enterprise keine Produktionsplanung jedoch Schnittstellen zu entsprechender Software.

A+W Enterprise wird in einer Glashütte mit dem gleichen modularen Aufbau eingesetzt wie in einem Glashandel, besitzt jedoch zusätzlich eine Stapellogik in den Bereichen:
- Auftragserfassung
- Versand
- Lager

**Auftragserfassung**
Aufträge werden ladungsbezogen erfasst und entsprechen einer LKW-Ladung. Bei der Zusammenstellung der Lieferung in der Auftragserfassung wird die Gestellart mit ihren Stapeleigenschaften, die Ankunftszeit beim Kunden sowie die Verfügbarkeitsprüfung des dispositiven Bestandes von Stapeln berücksichtigt.

**Versand**
Die Versandsteuerung bietet jederzeit einen genauen Überblick was, wann, wohin zu liefern ist. Im Versand werden alle Aufträge anhand einer Pickliste zusammengestellt. Gibt es das gewünschte Gestell nicht im Lager, wird es mittels des Stapelinformationssystemes gepackt und in das Auslieferungslager überführt.

**Lager**
Das Stapellager ist der zentrale Punkt an dem alle Lager- und Stapelinformationen zusammenlaufen. Es protokolliert lückenlos alle Aktionen von der Einbuchung bis zur Ausbuchung eines Stapels und bildet so einen wichtigen Bestandteil des Qualitätssystems.

##### ISO-, ESG- oder VSG-Hersteller
Ein typischer ISO-, ESG- oder VSG-Hersteller mit angeschlossenem Handelshaus nutzt im kaufmännischen Bereich sämtliche zuvor beschriebenen Funktionen wie beim Glashandel. Zusätzlich benötigt er eine detaillierte Produktions- und Kapazitätsplanung sowie eine flexible Produktionssteuerung. Als moderner Betrieb soll die Produktion per Betriebsdatenerfassung (BDE) überwacht werden.
- Freie Formen - Modelle
- Übergabe an Produktionsplanung und Fertigung (A+W Production)
- Fertigungssteuerung (A+W Production) und Betriebsdatenerfassung (BDE)

**Freie Formen- Modelle**
Da Betriebe einen wachsenden Anteil an Modellscheiben zu verzeichnen haben, kann zur fertigungstechnischen Beschreibung freier Formen A+W CAD Designer (Shapes) genutzt werden. Die enge Kopplung dieser CAD-Software zur A+W Enterprise -Vorgangsbearbeitung ermöglicht es, die Vermaßung beliebiger Modellscheiben direkt in der entsprechenden Auftragsposition vorzunehmen und mit dem zugehörigen Vorgang abzuspeichern. A+W Enterprise hält diese Daten bei einer anschließenden Übertragung zur Produktion stets zusammen und übergibt die Geometriedaten automatisch dem entsprechenden Optimierungslauf.

**Übergabe an A+W Production**
Für alle fertigungsrelevanten Aufträge führt das Produktionsplanungs- und Steuerungssystem (A+W Production), ausgehend vom Kundenwunschtermin, eine Rückwärtsterminierung durch. Die terminliche und kapazitive Produktionsvorplanung wird dabei von Maschinenrestriktionen, Auslastung, Durchlaufzeiten, technologischen Zuordnungen, Lager, Bestellwesen, usw. beeinflusst. Aufgrund der Durchlauf- und Beschaffungszeiten werden die einzelnen Arbeitsgänge schichtgenau vorterminiert und die benötigten Maschinenkapazitäten reserviert.

Die Länge einer Schicht oder die Vereinbarung von Sonderschichten können vom Betriebsleiter jederzeit verändert werden und stehen dem Planungssystem sofort zur Verfügung. Die Überschreitung von Produktionskapazitäten führt automatisch dazu, dass ganze Fertigungsaufträge verschoben werden. Wenn Maschinenrestriktionen nicht erfüllt werden können, dann wird automatisch auf Ausweichtechnologien zugegriffen. Ein Informationssystem gibt jederzeit online Auskunft über den aktuellen Stand der verplanten Technologien und Kapazitäten.

Mit dem Produktionsabruf werden die zuvor erzeugten Produktionsläufe zur Fertigung freigegeben. Dies ist sowohl automatisch als auch interaktiv möglich. Wenn die Optimierung durchgeführt ist, dann werden die Steuerdaten für die einzelnen Maschinen bereitgestellt.

Durch den Einsatz von Produktionsrückmeldung und BDE ist es im A+W Enterprise möglich den Status eines Vorgangs/Auftrags zu kontrollieren.

##### Konzernartige Unternehmen
Die zu unterstützende Struktur bei konzernartigen Unternehmen kann sehr unterschiedlich sein. Sie reicht vom losen Zusammenschluss selbstständiger Einzelbetriebe bis hin zum streng hierarchisch geführten Großunternehmen. Entsprechend unterschiedlich sind auch die Anforderungen an die eingesetzte Software. Zusätzlich zu den zuvor beschriebenen Funktionen für Glashandel und ISO-ESG-, VSG-Hersteller bietet A+W Enterprise darüber hinaus große Vorteile für konzernartige Unternehmen.
- Zentrale Stammdatenverwaltung
- Bestellkopplung
- Leistungsverrechnung beim gruppeninternen Geschäftsverkehr
- Konzern-Berichtswesen

**Zentrale Stammdatenverwaltung**
Die Stammdaten können innerhalb einer Unternehmensgruppe mit mehreren A+W Enterprise-Mandanten zentral verwaltet und verteilt werden. A+W Enterprise stellt dafür unterschiedliche Übertragungsfunktionen zur Verfügung, die es ermöglichen, bestimmte Stammdaten ganz oder teilweise, automatisiert oder interaktiv zu verteilen.

**Bestellkopplung**
Die Vorgangsübertragung vom Handelshaus zu den angeschlossenen Produktionsbetrieben sowie die Rückmeldung von Terminverschiebungen, Produktionsfreigaben und die Information über bereits verfügbare Stückzahlen kann über A+W Enterprise vollständig automatisiert erfolgen.

**Leistungsverrechnung beim gruppeninternen Geschäftsverkehr**
Darüber hinaus existieren Funktionen zur Verrechnung des gruppeninternen Geschäftsverkehrs. Für das Objektgeschäft wurde ein spezielles Informationssystem geschaffen, um zu vermeiden, dass einzelne Niederlassungen ungewollt als Konkurrenten am Markt agieren.

**Konzern-Berichtswesen**
Zur Erhöhung der marktpolitischen Reaktionsfähigkeit steht der Unternehmensleitung eine integrierte Konzernstatistik zur Verfügung, die statistische Daten der Einzelunternehmen übergreifend zusammenfasst.

#### Systemumfeld
Um den grundlegenden Anforderungen eines leistungsfähigen IT-Systems gerecht zu werden, wurden schon in der Planungsphase folgende Themen berücksichtigt:
- Betriebssicherheit
- Systemverfügbarkeit
- unterstützte Hardwareplattformen
- Erweiterbarkeit
- Vernetzungsmöglichkeiten
- Zugangsbeschränkung und -kontrolle

A+W Enterprise besitzt eine grafische Benutzeroberfläche und kann aufgrund der Client-Server-Architektur den betrieblichen Erfordernissen schrittweise angepasst und jederzeit erweitert werden.

> **Diagramm: 3-Schichten-Architektur**
>
> - **Client-PC (Windows) - Darstellungsschicht**: Die Benutzeroberfläche, die auf den PCs der Anwender läuft.
> - **Unix-Server**:
>   - **Logikschicht**: Die Anwendungslogik, die die Geschäftsprozesse verarbeitet.
>   - **Datenschicht**: Die Datenbank, in der die Daten gespeichert sind.
>
> Alle Schichten sind miteinander verbunden und bilden eine flexible, skalierbare Architektur.

Die gewählte Systemarchitektur dient der langfristigen Investitionssicherung und der Einsetzbarkeit in den unterschiedlichsten Unternehmen. In diesem Abschnitt finden Sie Informationen zu folgenden Punkten:
- Systemarchitektur
- Datensicherheit
- Benutzeroberfläche
- Wartung und Pflege

##### Systemarchitektur
A+W Enterprise baut auf dem Betriebssystem Unix auf und kann auf AIX bzw. Linux-Servern betrieben werden.

Durch die klare Trennung von Datenbank, Datenverarbeitung und Oberfläche (3-Schichten-Architektur) lässt sich das System sehr flexibel an die betrieblichen Erfordernisse anpassen. So ist es bei wachsender Benutzerzahl problemlos möglich, mehr Rechnerleistung in die Applikationsschicht einzubringen, ohne dass Datenbanken und Oberfläche (Benutzer-PCs) verändert werden müssen.

Als Datenhaltungssystem kommt die relationale Datenbank INFORMIX zum Einsatz. Das zugrunde liegende Datenmodell ist offen gelegt und kann über eine Online-Dokumentation eingesehen werden. Sie können die Daten jederzeit mit Standardsoftware auswerten und analysieren. Beispielsweise können Sie mit Microsoft Word oder Excel direkt auf den A+W Enterprise-Datenbestand lesend zugreifen. Im Gegenzug ist es möglich, aus jedem beliebigen Dialog des A+W Enterprise-Systems die Daten unmittelbar an Microsoft Excel oder Word zu übergeben.

A+W Enterprise lässt sich vollständig in eine Netzwerklandschaft einbinden. Lokale Netze werden ebenso unterstützt wie Weitverkehrsnetze (WAN) unter Nutzung von Wählverbindungen oder Standleitungen. Schnittstellen zu E-Mail, Telefax und zu Telefonanlagen sind ebenfalls möglich.

##### Datensicherheit
Die Anwendung ist vollständig transaktionsgesichert. Dies bedeutet, dass A+W Enterprise Aktionen (z. B. Rechnungen erzeugen und Statistiken buchen) entweder vollständig oder gar nicht ausführt. Die eingesetzten Komponenten ermöglichen selbst im Falle eines Systemabsturzes, die Daten fast vollständig und in jedem Falle konsistent wieder herzustellen. Die Datensicherung erfolgt automatisch zur einstellbaren Uhrzeit oder parallel zum laufenden Betrieb.

##### Benutzeroberfläche
Die A+W Enterprise-Oberfläche wird von typischen Windows-Dialogen geprägt. Sie verfügen über Schaltflächen, Symbolleisten, Kontextmenüs, Icons und vielen weiteren Windows-Bedienelementen.

Da die Benutzeroberfläche in einer eigenen Windows-Applikation (FIX/Win) ausgeführt wird, während das eigentliche A+W Enterprise-Programm getrennt davon auf einem Applikations-Server läuft, erfordert das System nur geringe Rechenleistung am Benutzer-PC.

##### Wartung und Pflege
Zu jeder A+W Enterprise-Installation gehört ein leistungsfähiges Betreuungskonzept. Zur Betreuung gehören regelmäßige Updates, die über das Netz verschickt und außerhalb der normalen Betriebszeit installiert werden. Die Wartung erfolgt grundsätzlich über eine Netzwerkkopplung, so dass ein gleichzeitiger Datentransfer stattfinden kann. So ist ein sehr effektiver Support möglich.

### Grundlagen zur Arbeit mit A+W Enterprise

In diesem Themenblock lernen Sie, wie Sie mit A+W Enterprise arbeiten und wie Sie die Stammdaten einrichten.

Der Themenblock beinhaltet folgende Schulungseinheiten:
- Bedienen von A+W Enterprise
- Stammdaten

#### Bedienen von A+W Enterprise

> **Lernziele**
> - Aufbau des Programms verstehen
> - Aufbau der Dialoge mit seinen Icons kennenlernen
> - Arbeitsweise im Dialog beherrschen
> - Arbeitsprozesse zwischen Dialogen beherrschen
> - Tastaturbefehle erlernen
> - Die Bedienung von A+W Enterprise mit seinen Besonderheiten erlernen
>
> **Nutzen**
> Die Bedienung in A+W Enterprise ist geprägt durch spezielle Arbeitsweisen in Dialogen und dialogübergreifenden Prozessen. Das erlernen dieser Prinzipien ist die grundlegende Voraussetzung schnell und effizient mit A+W Enterprise zu arbeiten.
>
> **Definitionen**
> - **FIX/Win**: Grafische Oberfläche, in die A+W Enterprise eingebettet ist
> - **SELO**: Numerische Suchfunktionalität `<F9>`
> - **Matchcode**: Alphanumerische Suchfunktionalität `<F8>`
> - **Dialog**: Bezeichnung der Eingabeoberfläche in A+W Enterprise
>
> **Merke**
> - **Tastenkombinationen**: Im A+W Enterprise stehen viele Tastenkombinationen für die Bedienung der Anwendung zur Verfügung.

##### A+W Enterprise starten und beenden
In Anschluss wird erklärt wie das Programm A+W Enterprise gestartet und beendet wird.

**So starten Sie A+W Enterprise:**
1.  Um A+W Enterprise zu starten, öffnen Sie den A+W Ordner auf Ihrem Desktop. Wählen Sie A+W Enterprise in der gewünschten Konfiguration und starten Sie mit einem Doppelklick den Anmeldedialog.
2.  Wählen Sie in der Programm-Liste das Modul, welches Sie starten wollen. Geben Sie anschließend Ihren Benutzernamen und Ihr Passwort (wird vom Administrator vergeben) in die entsprechenden Felder ein.
3.  Betätigen Sie die Schaltfläche [Verbinden]. A+W Enterprise startet das gewählte Modul. A+W Enterprise öffnet das gewählte Modul in einem Programmfenster.

**So beenden Sie A+W Enterprise:**
1.  Um A+W Enterprise korrekt zu beenden, schließen Sie den Dialog mit der Taste `<Ende>` oder `<Pos1>` und betätigen Sie `<Ende>`, bis A+W Enterprise eine Sicherheitsabfrage anzeigt, ob Sie das Programm beenden möchten.
2.  Betätigen Sie die Schaltfläche [JA]. A+W Enterprise schließt die Anwendung auf Ihrem Rechner und meldet Sie auf der Datenbank ab.

##### Startbildschirm
Wenn Sie im Anmeldedialog A+W Enterprise ausgewählt haben, dann zeigt das Programmfenster den A+W Enterprise-Startbildschirm an.

